# Comparing `tmp/ppatch-0.0.3.tar.gz` & `tmp/ppatch-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ppatch-0.0.3.tar", last modified: Mon Apr  8 09:16:57 2024, max compression
+gzip compressed data, was "ppatch-0.0.4.tar", last modified: Wed May  8 10:10:05 2024, max compression
```

## Comparing `ppatch-0.0.3.tar` & `ppatch-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,18 @@
--rw-r--r--   0        0        0     1066 2024-01-25 10:42:24.584919 ppatch-0.0.3/LICENSE
--rw-r--r--   0        0        0    11981 2024-04-08 08:34:31.003741 ppatch-0.0.3/README.md
--rw-r--r--   0        0        0      499 2024-04-08 09:16:57.991465 ppatch-0.0.3/pyproject.toml
--rw-r--r--   0        0        0       21 2024-03-13 07:54:26.926711 ppatch-0.0.3/src/ppatch/__init__.py
--rw-r--r--   0        0        0      335 2024-04-03 09:07:58.028939 ppatch-0.0.3/src/ppatch/app.py
--rw-r--r--   0        0        0     1622 2024-04-03 12:39:04.843779 ppatch-0.0.3/src/ppatch/commands/apply.py
--rw-r--r--   0        0        0     3003 2024-03-25 11:47:38.380836 ppatch-0.0.3/src/ppatch/commands/auto.py
--rw-r--r--   0        0        0     1590 2024-03-25 06:28:43.676959 ppatch-0.0.3/src/ppatch/commands/get.py
--rw-r--r--   0        0        0      870 2024-03-25 06:28:43.239945 ppatch-0.0.3/src/ppatch/commands/show.py
--rw-r--r--   0        0        0     5020 2024-04-03 12:27:11.745378 ppatch-0.0.3/src/ppatch/commands/trace.py
--rw-r--r--   0        0        0     1535 2024-04-03 12:14:16.362389 ppatch-0.0.3/src/ppatch/model.py
--rw-r--r--   0        0        0     2290 2024-04-03 09:44:38.712738 ppatch-0.0.3/src/ppatch/utils/common.py
--rw-r--r--   0        0        0     2802 2024-03-12 09:59:06.670493 ppatch-0.0.3/src/ppatch/utils/parse.py
--rw-r--r--   0        0        0     7293 2024-04-03 11:22:08.504525 ppatch-0.0.3/src/ppatch/utils/resolve.py
--rw-r--r--   0        0        0    12293 1970-01-01 00:00:00.000000 ppatch-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-01-25 10:42:24.584919 ppatch-0.0.4/LICENSE
+-rw-r--r--   0        0        0      649 2024-04-11 09:30:45.056874 ppatch-0.0.4/README.md
+-rw-r--r--   0        0        0      563 2024-05-08 10:10:05.716832 ppatch-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0       21 2024-03-13 07:54:26.926711 ppatch-0.0.4/src/ppatch/__init__.py
+-rw-r--r--   0        0        0       28 2024-05-08 10:07:04.820507 ppatch-0.0.4/src/ppatch/__main__.py
+-rw-r--r--   0        0        0      281 2024-04-11 08:42:18.488669 ppatch-0.0.4/src/ppatch/app.py
+-rw-r--r--   0        0        0     1693 2024-05-08 10:07:04.829507 ppatch-0.0.4/src/ppatch/commands/apply.py
+-rw-r--r--   0        0        0     4646 2024-05-08 10:07:04.829507 ppatch-0.0.4/src/ppatch/commands/auto.py
+-rw-r--r--   0        0        0     1644 2024-05-08 10:07:04.829507 ppatch-0.0.4/src/ppatch/commands/get.py
+-rw-r--r--   0        0        0      172 2024-04-11 08:42:18.909675 ppatch-0.0.4/src/ppatch/commands/help.py
+-rw-r--r--   0        0        0      870 2024-04-11 09:03:57.269830 ppatch-0.0.4/src/ppatch/commands/show.py
+-rw-r--r--   0        0        0     4782 2024-05-08 10:07:04.829507 ppatch-0.0.4/src/ppatch/commands/trace.py
+-rw-r--r--   0        0        0      759 2024-04-11 09:04:40.900874 ppatch-0.0.4/src/ppatch/config.py
+-rw-r--r--   0        0        0     1499 2024-05-08 10:07:04.829507 ppatch-0.0.4/src/ppatch/model.py
+-rw-r--r--   0        0        0     2300 2024-05-08 10:07:04.829507 ppatch-0.0.4/src/ppatch/utils/common.py
+-rw-r--r--   0        0        0     2802 2024-03-12 09:59:06.670493 ppatch-0.0.4/src/ppatch/utils/parse.py
+-rw-r--r--   0        0        0     9810 2024-05-08 10:07:04.829507 ppatch-0.0.4/src/ppatch/utils/resolve.py
+-rw-r--r--   0        0        0     1033 1970-01-01 00:00:00.000000 ppatch-0.0.4/PKG-INFO
```

### Comparing `ppatch-0.0.3/LICENSE` & `ppatch-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ppatch-0.0.3/src/ppatch/commands/apply.py` & `ppatch-0.0.4/src/ppatch/commands/apply.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
 
 @app.command()
 def apply(
     filename: str,
     patch_path: str,
     reverse: Annotated[bool, typer.Option("-R", "--reverse")] = False,
+    fuzz: Annotated[int, typer.Option("-F", "--fuzz")] = 0,
 ):
     """
     Apply a patch to a file.
     """
     if not os.path.exists(filename):
         typer.echo(f"Warning: {filename} not found!")
         return
@@ -35,15 +36,15 @@
     with open(patch_path, mode="r", encoding="utf-8") as (f):
         diffes = whatthepatch.parse_patch(f.read())
 
         for diff_ in diffes:
             diff = Diff(**unpack(diff_))
             if diff.header.old_path == filename or diff.header.new_path == filename:
                 apply_result = apply_change(
-                    diff.changes, new_line_list, reverse=reverse
+                    diff.changes, new_line_list, reverse=reverse, fuzz=fuzz
                 )
                 # TODO: 检查失败数
                 new_line_list = apply_result.new_line_list
             else:
                 typer.echo(f"Do not match with {filename}, skip")
     # new_line_list, _ = _apply(patch_path, filename, new_line_list, "default")
```

### Comparing `ppatch-0.0.3/src/ppatch/commands/auto.py` & `ppatch-0.0.4/src/ppatch/utils/common.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,91 +1,80 @@
-import os
-import re
 import subprocess
 
-import typer
+# import typer
+# import whatthepatch
 
-from ppatch.app import BASE_DIR, PATCH_STORE_DIR, app
-from ppatch.commands.get import getpatches
-from ppatch.commands.trace import trace
-from ppatch.utils.common import process_title
-
-
-@app.command()
-def auto(filename: str):
-    """Automatic do ANYTHING"""
-    if not os.path.exists(filename):
-        typer.echo(f"Warning: {filename} not found!")
-        return
-
-    # "patch -R -p1 -F 3 -i {filename}"
-    # TODO: 令 apply patch 支持 -R -F 参数，将此处切换为自行实现的版本
-    output: str = subprocess.run(
-        ["patch", "-R", "-p1", "-F", "3", "-i", filename], capture_output=True
-    ).stdout.decode("utf-8", errors="ignore")
-
-    # 首先按照 patching file，将输出分割为几块
-    output_parts: list[str] = []
-    for line in output.splitlines():
-        if line.startswith("patching file "):
-            output_parts.append(line + "\n")
-        else:
-            output_parts[-1] += line + "\n"
-
-    output_parts = [part for part in output_parts if "FAILED" in part]
-    if len(output_parts) == 0:
-        typer.echo("No failed patch")
-        return
-
-    # 确定每个 Part 里，有哪些文件，第几个 hunk 失败了
-    fail_file_list: dict[str, list[int]] = {}
-    for part in output_parts:
-        file_name = part.splitlines()[0].split(" ")[-1]
-
-        fail_hunk_list = []
-        for line in part.splitlines():
-            # 使用正则表达式匹配 hunk
-            # Hunk #1 FAILED at 1.
-            match = re.search(r"Hunk #(\d+) FAILED at (\d+).", line)
-            if match:
-                fail_hunk_list.append(int(match.group(1)))
-
-        fail_file_list[file_name] = fail_hunk_list
-
-    content = ""
-    with open(filename, mode="r", encoding="utf-8") as (f):
-        content = f.read()
-
-    from ppatch.utils.parse import parse_patch
-
-    subject = parse_patch(content).subject
-    for file_name, hunk_list in fail_file_list.items():
-        typer.echo(
-            f"{len(hunk_list)} hunk(s) failed in {file_name} with subject {subject}"
-        )
-
-        sha_list = getpatches(file_name, subject, save=True)
-        sha_for_sure = None
-
-        for sha in sha_list:
-            with open(
-                os.path.join(
-                    BASE_DIR, PATCH_STORE_DIR, f"{sha}-{process_title(file_name)}.patch"
-                ),
-                mode="r",
-                encoding="utf-8",
-            ) as (f):
-                text = f.read()
-                if parse_patch(text).subject == subject:
-                    sha_for_sure = sha
-                    break
-
-        if sha_for_sure is None:
-            typer.echo(f"Error: No patch found for {file_name}")
-            return
-
-        typer.echo(f"Found correspond patch {sha_for_sure} to {file_name}")
-        typer.echo(f"Hunk list: {hunk_list}")
-
-        for hunk in hunk_list:
-            conflict_list = trace(file_name, from_commit=sha_for_sure, flag_hunk=hunk)
-            typer.echo(f"Conflict list: {conflict_list}")
+# from ppatch.model import Line
+# from .resolve import apply_change
+
+
+def clean_repo():
+    subprocess.run(["git", "clean", "-df"])
+    subprocess.run(["git", "reset", "--hard"])
+
+
+# def _apply(
+#     patch_path: str,
+#     filename: str,
+#     new_line_list: list[Line],
+#     from_commit_sha: str,
+#     flag: bool = False,
+# ) -> tuple[list[Line], list[Line]]:
+#     for diff in whatthepatch.parse_patch(
+#         open(patch_path, mode="r", encoding="utf-8").read()
+#     ):
+#         if diff.header.old_path == filename or diff.header.new_path == filename:
+#             try:
+#                 new_line_list, flag_line_list = apply_change(
+#                     diff.changes, new_line_list, flag=flag
+#                 )
+#             except Exception as e:
+#                 typer.echo(f"Apply patch {from_commit_sha} failed")
+#                 typer.echo(f"Error: {e}")
+#                 return [], []
+
+#             return new_line_list, flag_line_list
+
+#         else:
+#             typer.echo(f"Do not match with {filename}, skip")
+
+
+def process_title(filename: str):
+    """
+    Process the file name to make it suitable for path
+    """
+    return "".join([letter for letter in filename if letter.isalnum()])
+
+
+def find_list_positions(main_list: list[str], sublist: list[str]) -> list[int]:
+    sublist_length = len(sublist)
+    positions = []
+
+    for i in range(len(main_list) - sublist_length + 1):
+        if main_list[i : i + sublist_length] == sublist:
+            positions.append(i)
+
+    return positions
+
+
+def isnamedtupleinstance(x):
+    _type = type(x)
+    bases = _type.__bases__
+    if len(bases) != 1 or bases[0] != tuple:
+        return False
+    fields = getattr(_type, "_fields", None)
+    if not isinstance(fields, tuple):
+        return False
+    return all(type(i) == str for i in fields)
+
+
+def unpack(obj):
+    if isinstance(obj, dict):
+        return {key: unpack(value) for key, value in obj.items()}
+    elif isinstance(obj, list):
+        return [unpack(value) for value in obj]
+    elif isnamedtupleinstance(obj):
+        return {key: unpack(value) for key, value in obj._asdict().items()}
+    elif isinstance(obj, tuple):
+        return tuple(unpack(value) for value in obj)
+    else:
+        return obj
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `ppatch-0.0.3/src/ppatch/commands/get.py` & `ppatch-0.0.4/src/ppatch/commands/get.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 import os
 import re
 import subprocess
 
 import typer
 
-from ppatch.app import BASE_DIR, PATCH_STORE_DIR, app
+from ppatch.app import app
+from ppatch.config import settings
 from ppatch.utils.common import process_title
 
 
 @app.command("get")
 def getpatches(filename: str, expression: str = None, save: bool = True) -> list[str]:
     """
     Get patches of a file.
     """
     if not os.path.exists(filename):
         typer.echo(f"Warning: {filename} not found!")
-        return
+        return []
 
     typer.echo(f"Get patches of {filename}")
 
     output: str = subprocess.run(
         ["git", "log", "-p", "--", filename], capture_output=True
     ).stdout.decode("utf-8", errors="ignore")
 
@@ -40,15 +41,17 @@
         sha = patch.splitlines()[0].split(" ")[1]
 
         if pattern is not None and pattern.search(patch) is not None:
             sha_list.append(sha)
             typer.echo(f"Patch {sha} found with expression {expression}")
 
         patch_path = os.path.join(
-            BASE_DIR, PATCH_STORE_DIR, f"{sha}-{process_title(filename)}.patch"
+            settings.base_dir,
+            settings.patch_store_dir,
+            f"{sha}-{process_title(filename)}.patch",
         )
 
         if save:
             if not os.path.exists(patch_path):
                 with open(patch_path, mode="w+", encoding="utf-8") as (f):
                     f.write(patch)
```

### Comparing `ppatch-0.0.3/src/ppatch/commands/show.py` & `ppatch-0.0.4/src/ppatch/commands/show.py`

 * *Files identical despite different names*

### Comparing `ppatch-0.0.3/src/ppatch/commands/trace.py` & `ppatch-0.0.4/src/ppatch/commands/trace.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 import os
 import subprocess
 
 import typer
 import whatthepatch
 
-from ppatch.app import BASE_DIR, PATCH_STORE_DIR, app
-from ppatch.model import Diff, File, Line
+from ppatch.app import app
+from ppatch.config import settings
+from ppatch.model import ApplyResult, Diff, File, Line
 from ppatch.utils.common import process_title, unpack
 from ppatch.utils.resolve import apply_change
 
 
 @app.command()
-def trace(filename: str, from_commit: str = "", flag_hunk: int = -1):
+def trace(filename: str, from_commit: str = "", flag_hunk_list: list[int] = None):
+    flag_hunk_list = [] if flag_hunk_list is None else flag_hunk_list
+
     if not os.path.exists(filename):
         typer.echo(f"Warning: {filename} not found!")
         return
 
     typer.echo(f"tracing patch {filename} from {from_commit}")
 
     output: str = subprocess.run(
@@ -51,93 +54,87 @@
     origin_file = File(file_path=filename)
     new_line_list = []
     # 首先将最后一个 patch 以 flag=True 的方式 apply
     from_commit_sha = sha_list.pop()
     assert from_commit_sha == from_commit
     typer.echo(f"Apply patch {from_commit_sha} to {filename}")
     patch_path = os.path.join(
-        BASE_DIR, PATCH_STORE_DIR, f"{from_commit_sha}-{process_title(filename)}.patch"
+        settings.base_dir,
+        settings.patch_store_dir,
+        f"{from_commit_sha}-{process_title(filename)}.patch",
     )
 
     for diff_ in whatthepatch.parse_patch(
         open(patch_path, mode="r", encoding="utf-8").read()
     ):
         diff = Diff(**unpack(diff_))
         if diff.header.old_path == filename or diff.header.new_path == filename:
             try:
                 apply_result = apply_change(
-                    diff.changes, origin_file.line_list, flag=True, flag_hunk=flag_hunk
+                    diff.changes,
+                    origin_file.line_list,
+                    flag=True,
+                    flag_hunk_list=flag_hunk_list,
                 )
                 # TODO: 检查失败数
                 new_line_list = apply_result.new_line_list
             except Exception as e:
                 typer.echo(f"Failed to apply patch {from_commit_sha}")
                 typer.echo(f"Error: {e}")
                 return
         else:
             typer.echo(f"Do not match with {filename}, skip")
 
-    confict_list: dict[str, list[Line]] = {}
+    confict_list: dict[str, ApplyResult] = {}
 
     # 注意这里需要反向
     sha_list.reverse()
     for sha in sha_list:
         patch_path = os.path.join(
-            BASE_DIR, PATCH_STORE_DIR, f"{sha}-{process_title(filename)}.patch"
+            settings.base_dir,
+            settings.patch_store_dir,
+            f"{sha}-{process_title(filename)}.patch",
         )
 
-        flag_line_list = []
+        apply_result: ApplyResult = ApplyResult()
         with open(patch_path, mode="r", encoding="utf-8") as (f):
             diffes = whatthepatch.parse_patch(f.read())
 
             for diff_ in diffes:
                 diff = Diff(**unpack(diff_))
                 if diff.header.old_path == filename or diff.header.new_path == filename:
                     try:
-                        apply_result = apply_change(diff.changes, new_line_list)
-                        # TODO: 检查失败数
-                        new_line_list, flag_line_list = (
-                            apply_result.new_line_list,
-                            apply_result.flag_line_list,
+                        apply_result = apply_change(
+                            diff.changes, new_line_list, trace=True, flag=True
                         )
+                        new_line_list = apply_result.new_line_list
 
                         typer.echo(
                             f"Apply patch {sha} to {filename}: {len(new_line_list)}"
                         )
                     except Exception as e:
                         typer.echo(f"Failed to apply patch {sha}")
                         typer.echo(f"Error: {e}")
 
-                        with open(
-                            filename + f".{sha}", mode="w+", encoding="utf-8"
-                        ) as (f):
-                            for line in new_line_list:
-                                if line.status:
-                                    f.write(line.content + "\n")
-
                         return
                 else:
                     typer.echo(f"Do not match with {filename}, skip")
 
-        assert isinstance(flag_line_list, list)
-
-        if len(flag_line_list) > 0:
-            confict_list[sha] = flag_line_list
+        if len(apply_result.conflict_hunk_num_list) > 0:
+            confict_list[sha] = apply_result
             typer.echo(f"Conflict found in {sha}")
-            for line in flag_line_list:
-                typer.echo(f"{line.index + 1}: {line.content}")
+            typer.echo(f"Conflict hunk list: {apply_result.conflict_hunk_num_list}")
 
     # 写入文件
     with open(filename, mode="w+", encoding="utf-8") as (f):
         for line in new_line_list:
             if line.status:
                 f.write(line.content + "\n")
 
     with open(filename + ".ppatch", mode="a+", encoding="utf-8") as (f):
         for line in new_line_list:
             if line.status:
                 f.write(f"{line.index + 1}: {line.content} {line.flag}\n")
 
     typer.echo(f"Conflict count: {len(confict_list)}")
-    typer.echo(f"Conflict list: {confict_list}")
 
     return confict_list
```

### Comparing `ppatch-0.0.3/src/ppatch/model.py` & `ppatch-0.0.4/src/ppatch/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,10 +56,9 @@
     header: Header
     changes: list[Change]
     text: str
 
 
 class ApplyResult(BaseModel):
     new_line_list: list[Line] = []
-    flag_line_list: list[Line] = []
     conflict_hunk_num_list: list[int] = []
     failed_hunk_list: list[Hunk] = []
```

### Comparing `ppatch-0.0.3/src/ppatch/utils/parse.py` & `ppatch-0.0.4/src/ppatch/utils/parse.py`

 * *Files identical despite different names*

### Comparing `ppatch-0.0.3/src/ppatch/utils/resolve.py` & `ppatch-0.0.4/src/ppatch/utils/resolve.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,39 @@
-from ppatch.app import MAX_DIFF_LINES
+import typer
+
+from ppatch.config import settings
 from ppatch.model import ApplyResult, Change, Hunk, Line
 from ppatch.utils.common import find_list_positions
 
 
 def apply_change(
     changes: list[Change],
     target: list[Line],
     reverse: bool = False,
     flag: bool = False,
-    flag_hunk: int = -1,
+    trace: bool = False,
+    flag_hunk_list: list[int] = None,
+    fuzz: int = 0,
 ) -> ApplyResult:
     """Apply a diff to a target string."""
 
+    flag_hunk_list = [] if flag_hunk_list is None else flag_hunk_list
+
+    if fuzz > settings.max_diff_lines or fuzz < 0:
+        raise Exception(f"fuzz value should be less than {settings.max_diff_lines}")
+
     # 如果反向，则交换所有的 old 和 new
+    # reverse 不支持 flag trace
     if reverse:
+        if flag:
+            raise Exception("flag is not supported with reverse")
+
         for change in changes:
             change.old, change.new = change.new, change.old
 
-    # 这里有个巨大的问题：diff 信息中的行号与实际行号不一致
-    # 一种修复方式：搜索 diff 每个 hunk 的上下文行，然后修改标记
-
     # 首先统计 Hunk 数
     hunk_indexes = []
     for change in changes:
         if change.hunk not in hunk_indexes:
             hunk_indexes.append(change.hunk)
 
     # TODO: 支持 -F 参数
@@ -48,159 +58,220 @@
         # 然后反向遍历，获取后置上下文
         for change in reversed(hunk_changes):
             if change.old is not None and change.new is not None:
                 hunk_post.append(change)
             else:
                 break
 
-        # 注意把后置上下文反转回来
-        hunk_post = list(reversed(hunk_post))
-
-        assert len(hunk_context) <= MAX_DIFF_LINES
-        assert len(hunk_post) <= MAX_DIFF_LINES
+        assert len(hunk_context) <= settings.max_diff_lines
+        assert len(hunk_post) <= settings.max_diff_lines
 
         # 最后获取中间代码
         for change in hunk_changes:
             if change not in hunk_context and change not in hunk_post:
                 hunk_middle.append(change)
 
+        hunk_context = hunk_context[0 : 3 - fuzz]
+        hunk_post = hunk_post[0 : 3 - fuzz]
+
+        # 注意把后置上下文反转回来
+        hunk_post = list(reversed(hunk_post))
+
         hunk_list.append(
             Hunk(
                 index=hunk_index,
                 context=hunk_context,
                 middle=hunk_middle,
                 post=hunk_post,
                 all_=hunk_changes,
             )
         )
 
     # 然后对每个hunk进行处理，添加偏移
     changes: list[Change] = []
     for hunk in hunk_list:
+        changes_to_search = hunk.context + hunk.middle + hunk.post
+        pos_list = find_list_positions(
+            [line.content for line in target],
+            [change.line for change in changes_to_search if change.old is not None],
+        )
 
-        def cal_offsets(target: list[Line], changes: list[Change]) -> list[int]:
-            pos_list = find_list_positions(
-                [line.content for line in target],
-                [change.line for change in changes],
-            )
-            if len(pos_list) == 0:
-                return []  # 这样使得下面计算交集时一定为空
-                # raise Exception(f"context lines do not exist in source")
-
-            offset_list = []
-            if len(changes) == 0:
-                offset_list = pos_list
-            else:
-                for position in pos_list:
-                    offset = position + 1 - changes[0].old
-                    offset_list.append(offset)
+        # 初始位置是 context 的第一个
+        # 注意，前几个有可能是空
+        pos_origin = None
+        for change in changes_to_search:
+            if change.old is not None:
+                pos_origin = change.old
+                break
 
-            return offset_list
+        # TODO: 这里不太对，要想一下怎么处理，不应该是加入 failed hunk list
+        # 仅在 -F 3 且只有添加行 的情况下出现
+        # 也可以看一下这样的情况有多少
+        if pos_origin is None:
+            failed_hunk_list.append(hunk)
+            hunk_list.remove(hunk)
+            continue
 
-        offset_context = cal_offsets(target, hunk.context)
-        offset_post = cal_offsets(target, hunk.post)
+        offset_list = [pos + 1 - pos_origin for pos in pos_list]  # 确认这里是否需要 1？
 
-        offset_list = list(set(offset_context) & set(offset_post))
         if len(offset_list) == 0:
             failed_hunk_list.append(hunk)
-            hunk_list.remove(hunk)
+            typer.echo(f"Apply failed with hunk {hunk.index}")
+            # hunk_list.remove(hunk)
             continue
             # raise Exception("offsets do not intersect")
 
         # 计算最小 offset
         min_offset = None
         for offset in offset_list:
             if min_offset is None or abs(offset) < abs(min_offset):
                 min_offset = offset
 
-        for change in hunk.middle:
-            changes.append(
-                Change(
-                    hunk=change.hunk,
-                    old=change.old + min_offset if change.old is not None else None,
-                    new=change.new + min_offset if change.new is not None else None,
-                    line=change.line,
-                )
+        # 如果 reverse 为 True，则直接替换，不进行 flag 追踪
+        if reverse:
+            # 直接按照 pos 进行替换
+            # 选择 offset 最小的 pos
+            pos_new = pos_origin + min_offset - 1
+
+            old_lines = [
+                change.line
+                for change in hunk.context + hunk.middle + hunk.post
+                if change.old is not None
+            ]
+            new_lines = [
+                change.line
+                for change in hunk.context + hunk.middle + hunk.post
+                if change.new is not None
+            ]
+
+            # 检查 pos_new 位置的行是否和 old_lines 一致
+            for i in range(len(old_lines)):
+                if target[pos_new + i].content != old_lines[i]:
+                    raise Exception(
+                        f'line {pos_new + i}, "{target[pos_new + i].content}" does not match "{new_lines[i]}"'
+                    )
+
+            # 以切片的方式进行替换
+            target = (
+                target[:pos_new]
+                + [
+                    Line(index=pos_new + i, content=new_lines[i])
+                    for i in range(len(new_lines))
+                ]
+                + target[pos_new + len(old_lines) :]
             )
 
+        else:
+            for change in hunk.middle:
+                changes.append(
+                    Change(
+                        hunk=change.hunk,
+                        old=change.old + min_offset if change.old is not None else None,
+                        new=change.new + min_offset if change.new is not None else None,
+                        line=change.line,
+                    )
+                )
+
+    if reverse:
+        return ApplyResult(
+            new_line_list=target,
+            conflict_hunk_num_list=[],
+            failed_hunk_list=failed_hunk_list,
+        )
+
     # 注意这里的 changes 应该使用从 hunk_list 中拼接出来的（也就是修改过行号的）
     for change in changes:
         if change.old is not None and change.line is not None:
             if change.old > len(target):
                 raise Exception(
                     f'context line {change.old}, "{change.line}" does not exist in source'
                 )
             if target[change.old - 1].content != change.line:
                 raise Exception(
                     f'context line {change.old}, "{change.line}" does not match "{target[change.old - 1]}"'
                 )
 
-    flag_line_list = []
     add_count = 0
     del_count = 0
 
     for change in changes:
         # 只修改新增行和删除行（只有这些行是被修改的）
         if change.old is None and change.new is not None:
             target.insert(
                 change.new - 1,
                 Line(
                     index=change.new - 1,
                     content=change.line,
                     changed=True,
                     status=True,
-                    flag=True
-                    if flag and (change.hunk == flag_hunk or flag_hunk == -1)
-                    else False,
+                    flag=True if change.hunk in flag_hunk_list and flag else False,
                     hunk=change.hunk,
                 ),
             )
             add_count += 1
 
         elif change.new is None and change.old is not None:
             index = change.old - 1 - del_count + add_count
 
-            # 如果被修改行有标记，则将其添加进标记列表
+            # 如果被修改行有标记，则标记将其删除的 hunk
             if target[index].flag:
-                flag_line_list.append(target[index])
+                conflict_hunk_num_list.append(change.hunk)
 
             del target[index]
             del_count += 1
 
-            conflict_hunk_num_list.append(change.hunk)
-
         else:
             # 对其他行也要标记 flag
             index = change.old - 1 - del_count + add_count
-            assert index == change.new - 1
+
+            try:
+                assert index == change.new - 1  # TODO: but why? 44733
+            except AssertionError:
+                typer.echo(
+                    f"index: {index}, change.new: {change.new}, hunk: {change.hunk}"
+                )
+
             target[index].flag = (
-                True
-                if flag and (change.hunk == flag_hunk or flag_hunk == -1)
-                else target[index].flag
-            )
+                True if flag and change.hunk in flag_hunk_list else target[index].flag
+            )  # 加点注释解释一下 # TODO: 确认这个条件是否是正确的
 
-    new_line_list = []
+    new_line_list: list[Line] = []
     for index, line in enumerate(target):
         # 判断是否在 Flag 行附近进行了修改
         # 如果该行为 changed，且前后行为flag，则也加入标记列表
-        if line.changed and not line.flag:
-            if index > 0 and target[index - 1].flag:
-                line.flag = True
-            if index < len(target) - 1 and target[index + 1].flag:
+        if flag and line.changed and not line.flag:
+            before_flag = (
+                index > 0 and target[index - 1].flag and not target[index - 1].changed
+            )
+            after_flag = (
+                index < len(target) - 1
+                and target[index + 1].flag
+                and not target[index + 1].changed
+            )
+
+            if before_flag or after_flag:
                 line.flag = True
 
             if line.flag:
-                flag_line_list.append(line)
                 conflict_hunk_num_list.append(line.hunk)
 
+            # 当 trace 为 True 时，将所有 conflict hunk 的行都标记为冲突
+            if trace and line.hunk in conflict_hunk_num_list:
+                line.flag = True
+
         new_line_list.append(
-            Line(
-                index=index, content=line.content, changed=line.changed, flag=line.flag
-            )
-        )
+            Line(index=index, content=line.content, flag=line.flag)
+        )  # 注意洗掉 hunk changed
+
+    failed_hunk_list.extend(
+        [
+            hunk
+            for hunk in hunk_list
+            if hunk.index in conflict_hunk_num_list and hunk not in failed_hunk_list
+        ]
+    )
 
     return ApplyResult(
         new_line_list=new_line_list,
-        flag_line_list=flag_line_list,
         conflict_hunk_num_list=conflict_hunk_num_list,
         failed_hunk_list=failed_hunk_list,
     )
```

