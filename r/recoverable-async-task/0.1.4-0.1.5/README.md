# Comparing `tmp/recoverable_async_task-0.1.4.tar.gz` & `tmp/recoverable_async_task-0.1.5.tar.gz`

## Comparing `recoverable_async_task-0.1.4.tar` & `recoverable_async_task-0.1.5.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    11243 2020-02-02 00:00:00.000000 recoverable_async_task-0.1.4/recoverable_async_task.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 recoverable_async_task-0.1.4/.gitignore
--rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 recoverable_async_task-0.1.4/README.md
--rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 recoverable_async_task-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     2864 2020-02-02 00:00:00.000000 recoverable_async_task-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0    11368 2020-02-02 00:00:00.000000 recoverable_async_task-0.1.5/recoverable_async_task.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 recoverable_async_task-0.1.5/.gitignore
+-rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 recoverable_async_task-0.1.5/README.md
+-rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 recoverable_async_task-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     2864 2020-02-02 00:00:00.000000 recoverable_async_task-0.1.5/PKG-INFO
```

### Comparing `recoverable_async_task-0.1.4/recoverable_async_task.py` & `recoverable_async_task-0.1.5/recoverable_async_task.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,29 +139,32 @@
             try:
                 yield done_task.result()
             except TaskException as e:
                 if e.error_num >= self.retry_n and self.raise_after_retry:
                     raise e
 
 
-class CheckpointData(TypedDict):
-    id: int | str
-    data: JSON
+ID_T = TypeVar("ID_T", bound=int | str)
+
+
+class CheckpointData(TypedDict, Generic[ID_T, T]):
+    id: ID_T
+    data: T
 
 
 def json_default_serializer(o: JSON_ITEM):
     logger.warning(
         f"Object {str(o)} of type {o.__class__.__name__} is not JSON serializable"
     )
     return str(o)
 
 
-class Checkpoint:
+class Checkpoint(Generic[ID_T, T]):
     @staticmethod
-    def load(checkpoint_path: str | Path) -> Iterator[CheckpointData]:
+    def load(checkpoint_path: str | Path) -> Iterator[CheckpointData[ID_T, T]]:
         logger.debug(f"load checkpoint from {checkpoint_path}")
         with Path(checkpoint_path).open() as f:
             for ln, line in enumerate(f):
                 line = line.strip()
                 try:
                     yield json.loads(line)
                 except json.JSONDecodeError as e:
@@ -183,21 +186,21 @@
         self.name = checkpoint_path_name
         self.checkpoint_path = Path(checkpoint_path_name).with_name(
             Path(checkpoint_path_name).stem + "-checkpoint.jsonl"
         )
         self.checkpoint_path.parent.mkdir(parents=True, exist_ok=True)
 
         self.checkpoint_path.touch(exist_ok=True)
-        self.datas: dict[int | str, JSON] = {
+        self.datas: dict[ID_T, T] = {
             ckpt["id"]: ckpt["data"] for ckpt in self.load(self.checkpoint_path)
         }
 
         self.saved = None
 
-    def add(self, data: JSON, id: int | str):
+    def add(self, data: T, id: ID_T):
         assert id not in self.datas, f"id {id} already exists"
         self.datas[id] = data
         with self.checkpoint_path.open("a") as f:
             json.dump(
                 CheckpointData(id=id, data=data),
                 f,
                 ensure_ascii=False,
@@ -213,17 +216,14 @@
             ),
             list(self.datas.values()),
         )
 
         return self.saved
 
 
-ID_T = TypeVar("ID_T", bound=int | str)
-
-
 class RecoverableAsyncTask(AsyncTask, Generic[ID_T, T]):
     """
     RecoverableAsyncTask extends the functionality of the AsyncTask class by adding checkpointing support.
 
     Parameters:
     - task_function: A coroutine function that takes an int or str as Task ID and returns a result.
     - max_workers: Maximum number of concurrent workers to execute tasks. Default is 10.
@@ -278,15 +278,17 @@
 
         Parameters:
         - task_function: A coroutine function that takes an int or str as input and returns a result.
         - max_workers: Maximum number of concurrent workers to execute tasks. Default is 10.
         - max_qps: Maximum queries per second limit. Default is 0 (no limit).
         - retry_n: Number of retries for failed tasks. Default is 3.
         """
-        self.checkpoint = Checkpoint(checkpoint_path_name or task_function.__name__)
+        self.checkpoint = Checkpoint[ID_T, T](
+            checkpoint_path_name or task_function.__name__
+        )
 
         @functools.wraps(task_function)
         async def _task_with_checkpoint(id: ID_T):
             result = await task_function(id)
             self.checkpoint.add(result, id=id)
             return result
 
@@ -346,8 +348,10 @@
 
         for i in range(17):
             re_async_task.push(i)
 
         async for result in re_async_task.collect_results():
             print(result)
 
+        print(f"Finished {len(re_async_task.checkpoint.datas)} tasks.")
+
     asyncio.run(main())
```

### Comparing `recoverable_async_task-0.1.4/README.md` & `recoverable_async_task-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `recoverable_async_task-0.1.4/pyproject.toml` & `recoverable_async_task-0.1.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `recoverable_async_task-0.1.4/PKG-INFO` & `recoverable_async_task-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: recoverable-async-task
-Version: 0.1.4
+Version: 0.1.5
 Summary: `recoverable-async-task` is a Python library that streamlines the handling of asynchronous tasks through its `RecoverableAsyncTask` class, with the added benefit of **supporting task checkpointing and resumption**. This feature ensures that tasks can pick up from where they left off in the event of unexpected failures.
 Project-URL: Homepage, https://github.com/Haskely/recoverable-async-task
 Project-URL: Bug Reports, https://github.com/Haskely/recoverable-async-task/issues
 Project-URL: Source, https://github.com/Haskely/recoverable-async-task
 Author-email: Haskely <Haskely@live.com>
 Requires-Python: >=3.8
 Requires-Dist: loguru>=0.7.2
```

