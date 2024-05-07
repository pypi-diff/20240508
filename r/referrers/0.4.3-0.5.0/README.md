# Comparing `tmp/referrers-0.4.3.tar.gz` & `tmp/referrers-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "referrers-0.4.3.tar", max compression
+gzip compressed data, was "referrers-0.5.0.tar", max compression
```

## Comparing `referrers-0.4.3.tar` & `referrers-0.5.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11357 2024-04-25 22:40:28.919484 referrers-0.4.3/LICENSE
--rw-r--r--   0        0        0     8135 2024-04-25 22:40:28.919484 referrers-0.4.3/README.md
--rw-r--r--   0        0        0      372 2024-04-25 22:40:28.919484 referrers-0.4.3/pyproject.toml
--rw-r--r--   0        0        0      130 2024-04-25 22:40:28.919484 referrers-0.4.3/src/referrers/__init__.py
--rw-r--r--   0        0        0    41140 2024-04-25 22:40:28.919484 referrers-0.4.3/src/referrers/impl.py
--rw-r--r--   0        0        0     8668 1970-01-01 00:00:00.000000 referrers-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-07 22:48:31.845692 referrers-0.5.0/LICENSE
+-rw-r--r--   0        0        0     7319 2024-05-07 22:48:31.845692 referrers-0.5.0/README.md
+-rw-r--r--   0        0        0      372 2024-05-07 22:48:31.845692 referrers-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      130 2024-05-07 22:48:31.845692 referrers-0.5.0/src/referrers/__init__.py
+-rw-r--r--   0        0        0    42056 2024-05-07 22:48:31.845692 referrers-0.5.0/src/referrers/impl.py
+-rw-r--r--   0        0        0     7852 1970-01-01 00:00:00.000000 referrers-0.5.0/PKG-INFO
```

### Comparing `referrers-0.4.3/LICENSE` & `referrers-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `referrers-0.4.3/README.md` & `referrers-0.5.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: referrers
+Version: 0.5.0
+Summary: Finds the graph of referrers for a Python object
+Author: Neil Ferguson
+Requires-Python: >=3.8
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: networkx (>=3.1.0)
+Description-Content-Type: text/markdown
+
 # Referrers
 
 Referrers is a Python package that helps to answer the question **"what is holding
 a reference to this object?"**, which is useful for debugging memory leaks and other
 issues. It tries to assign a meaningful name to each reference to an object and
 returns a graph of referrers (including indirect referrers).
 
@@ -107,19 +122,19 @@
 top_10_objects = (muppy.sort(muppy.get_objects()))[-10:]
 top_10_objects.reverse()
 
 for obj in top_10_objects:
     print(
         referrers.get_referrer_graph(
             obj,
-            search_for_untracked_objects=True,
             exclude_object_ids=[id(top_10_objects)],
         )
     )
 
+
 ```
 
 Note that this example sets the `search_for_untracked_objects` flag to `True` to try to find
 referrers for objects that are not tracked by the garbage collector. It also sets
 `exclude_object_ids` to exclude the `top_10_objects` variable from the graph.
 
 Here's how to find the referrers of all objects that have been created
@@ -140,15 +155,14 @@
 summary.print_(summary.get_diff(summary.summarize(o1), summary.summarize(o2)))
 
 for obj in diff:
     print(
         referrers.get_referrer_graph(
             obj,
             exclude_object_ids=[id(o1), id(o2), id(diff), id(o2_ids)],
-            search_for_untracked_objects=True,
         )
     )
 ```
 
 This will print a summary of the objects that have been created between o1 and o2,
 as well as the variable names that reference these objects. This can be useful for finding
 memory leaks.
@@ -186,65 +200,14 @@
         with_labels=True,
     )
     plt.show()
 
 my_function()
 ```
 
-## Untracked Objects
-
-By default, `get_referrer_graph` will raise an error if the object passed to it is not
-tracked by the garbage collector. In CPython, for example, immutable objects and some
-containers that contain only immutable objects (like dicts and tuples) are not tracked
-by the garbage collector.
-
-However, the `search_for_untracked_objects` flag can be set to `True` when calling
-`get_referrer_graph` to try to find referrers for objects are not tracked by the garbage
-collector. This option is experimental and may not work well in all cases.
-
-For example, here we find the referrers of an untracked object (a `dict` containing only
-immutable objects):
-
-```python
-import dataclasses
-import gc
-from typing import Dict
-
-import referrers
-
-@dataclasses.dataclass
-class ParentClass:
-    member_variable: Dict
-
-def my_func():
-    local_variable = ParentClass({"a": 1})
-    assert not gc.is_tracked(local_variable.member_variable)
-    print(referrers.get_referrer_graph(local_variable.member_variable, search_for_untracked_objects=True))
-
-my_func()
-```
-
-This will output something like:
-
-```plaintext
-╙── dict instance (id=4483928640)
-    └─╼ ParentClass.member_variable (instance attribute) (id=4482048576)
-        └─╼ my_func.local_variable (local) (id=4482048576)
-```
-
-### Known limitations with untracked objects
-
-* The depth of the search for untracked objects is limited by the `max_untracked_search_depth`
-  parameter. If this is set too low, some untracked objects may be missing from the graph.
-  Try setting this to a higher value if you think this is happening
-* Sometimes internal references (from within `referrers`) may be included in the graph when
-  finding untracked objects. It should be possible to get rid of these, but I'm not sure if I've
-  found them all yet.
-* Finding untracked objects may be slow.
-
 ## Multi-threading
 
 Referrers works well with multiple threads. For example, you can have a separate thread that
 prints the referrers of objects that have references in other threads.
 
 In the following example, there is a thread that prints the referrers of all instances of
 `ChildClass` every second (using [Pympler](https://pympler.readthedocs.io/en/latest/) to find
@@ -278,10 +241,49 @@
     child_variable = ChildClass()
     container_variable = ContainerClass(child_variable)
     sleep(1000)
 
 my_function()
 ```
 
+## Untracked Objects
+
+This library will try to find referrers for objects that are not tracked by the garbage
+collector. For example, mutable objects, and collections containing only immutable objects in
+CPython. However, this may be slower than for tracked objects, and is limited by the
+`max_untracked_search_depth` parameter. Try setting this to a higher value if you think there
+are referrers missing from the graph.
+
+For example, here we find the referrers of an untracked object (a `dict` containing only
+immutable objects):
+
+```python
+import dataclasses
+import gc
+from typing import Dict
+
+import referrers
+
+@dataclasses.dataclass
+class ParentClass:
+    member_variable: Dict
+
+def my_func():
+    local_variable = ParentClass({"a": 1})
+    assert not gc.is_tracked(local_variable.member_variable)
+    print(referrers.get_referrer_graph(local_variable.member_variable))
+
+my_func()
+```
+
+This will output something like:
+
+```plaintext
+╙── dict instance (id=4483928640)
+    └─╼ ParentClass.member_variable (instance attribute) (id=4482048576)
+        └─╼ my_func.local_variable (local) (id=4482048576)
+```
+
 ## Source
 
 See [https://github.com/nfergu/referrers](https://github.com/nfergu/referrers) for the Github repo.
+
```

### Comparing `referrers-0.4.3/src/referrers/impl.py` & `referrers-0.5.0/src/referrers/impl.py`

 * *Files 5% similar despite different names*

```diff
@@ -111,89 +111,84 @@
 
 
 def get_referrer_graph(
     target_object: Any,
     max_depth: Optional[int] = 10,
     exclude_object_ids: Optional[Sequence[int]] = None,
     module_prefixes: Optional[Collection[str]] = None,
-    search_for_untracked_objects: bool = False,
-    max_untracked_search_depth: int = 10,
+    max_untracked_search_depth: int = 30,
 ) -> ReferrerGraph:
     """
     Gets a graph of referrers for the target object.
 
     To analyze a list of objects, use `get_referrer_graph_for_list` instead.
 
+    Note: This function forces a garbage collection.
+
     :param target_object: The object to analyze.
     :param max_depth: The maximum depth to search for referrers. The default is 10. Specify
         `None` to search to unlimited depth (but be careful with this: it may take a long time).
     :param exclude_object_ids: A list of object IDs to exclude from the referrer graph.
     :param module_prefixes: The prefixes of the modules to search for module-level variables.
         If this is not specified, the top-level package of the calling code is used.
-    :param search_for_untracked_objects: Whether to search for referrers of objects that are
-        not tracked by the garbage collector. By default, this is `False` because it can be
-        slow to search for untracked objects, and it is not reliable in all cases. If this is
-        set to `False` and `target_object` is untracked, an error will be raised. If this is
-        set to `True` then `max_untracked_search_depth` is used to control the depth of the
-        search.
     :param max_untracked_search_depth: The maximum depth to search for referrers of untracked
         objects. This is the depth that referents will be searched from the roots (locals and
-        globals). The default is 10. If you are missing referrers of untracked objects, you
+        globals). The default is 30. If you are missing referrers of untracked objects, you
         can increase this value.
 
     :return: An ObjectGraph containing `ReferrerGraphNode`s, representing the referrers of
         `target_object`.
     """
+    gc.collect()
+
     exclude_object_ids = exclude_object_ids or []
     exclude_object_ids = list(exclude_object_ids)
 
     return get_referrer_graph_for_list(
         [target_object],
         max_depth=max_depth,
         exclude_object_ids=exclude_object_ids,
         module_prefixes=module_prefixes,
-        search_for_untracked_objects=search_for_untracked_objects,
         max_untracked_search_depth=max_untracked_search_depth,
     )
 
 
 def get_referrer_graph_for_list(
     target_objects: List[Any],
     max_depth: Optional[int] = 10,
     exclude_object_ids: Optional[Sequence[int]] = None,
     module_prefixes: Optional[Collection[str]] = None,
-    search_for_untracked_objects: bool = False,
-    max_untracked_search_depth: int = 10,
+    max_untracked_search_depth: int = 30,
 ) -> ReferrerGraph:
     """
     Gets a graph of referrers for the list of target objects. All objects in the
     list are analyzed. To analyze a single object, use `get_referrer_graph`.
 
-    The `target_objects` list is excluded from the referrer grap.
+    The `target_objects` list is excluded from the referrer graph.
+
+    Note: This function forces a garbage collection.
 
     :param target_objects: The objects to analyze. This must be a list.
     :param max_depth: The maximum depth to search for referrers. The default is 10. Specify
         `None` to search to unlimited depth (but be careful with this: it may take a long time).
     :param exclude_object_ids: A list of object IDs to exclude from the referrer graph.
     :param module_prefixes: The prefixes of the modules to search for module-level variables.
         If this is `None`, the top-level package of the calling code is used.
-    :param search_for_untracked_objects: Whether to search for referrers of objects that are
-        not tracked by the garbage collector. By default, this is `False` because it can be
-        slow to search for untracked objects, and it is not reliable in all cases. If this is
-        set to `False` and any of `target_objects` are untracked, an error will be raised. If
-        this is set to `True` then `max_untracked_search_depth` is used to control the depth of
-        the search.
     :param max_untracked_search_depth: The maximum depth to search for referrers of untracked
         objects. This is the depth that referents will be searched from the roots (locals and
-        globals). The default is 10. If you are missing referrers of untracked objects, you
+        globals). The default is 30. If you are missing referrers of untracked objects, you
         can increase this value.
 
     :return: An ObjectGraph containing `ReferrerGraphNode`s, representing the referrers of
         the target objects.
     """
+    # Garbage collect before we start, otherwise repeated calls to this function may identify
+    # referrers that are internal to this module.
+    gc.collect()
+
     # We don't allow any iterable, only lists. This is because it's easy to accidentally
     # pass a single big object (like a Pandas dataframe) that is iterable and would be
     # very slow to analyze.
     if not isinstance(target_objects, list):
         raise ValueError("target_objects must be a list")
 
     exclude_object_ids = exclude_object_ids or []
@@ -203,24 +198,14 @@
     # references to the same objects (once as a local or global, and once as a referrer from
     # the locals or globals dict).
     for thread_frames in _get_frames_for_all_threads().values():
         for frame in thread_frames:
             exclude_object_ids.append(id(frame.f_locals))
             exclude_object_ids.append(id(frame.f_globals))
 
-    if not search_for_untracked_objects:
-        untracked_objects = [obj for obj in target_objects if not gc.is_tracked(obj)]
-        if untracked_objects:
-            raise ValueError(
-                "Some target objects are not tracked by the garbage collector. "
-                "Set search_for_untracked_objects to True to search for referrers of "
-                "these objects, but bear in mind that this can be slow and may not be "
-                "reliable in all cases."
-            )
-
     builder = _ReferrerGraphBuilder(
         target_objects,
         module_prefixes,
         max_untracked_search_depth=max_untracked_search_depth,
         exclude_object_ids=exclude_object_ids,
     )
     return builder.build(max_depth=max_depth)
@@ -319,20 +304,20 @@
                         # Don't go any further down the stack for this thread if we've found some
                         # names for the object in this frame.
                         if frame_names:
                             names.update(frame_names)
                             break
         return names
 
-    def _get_frame_names(self, frame: FrameType, target_object: Any) -> Set[str]:
+    def _get_frame_names(self, frame: FrameType, target_object: Any) -> Iterable[str]:
         """
         Gets the local_names of the target object in the local variables of the frame.
         :param frame: The frame to search.
         :param target_object: The object to search for.
-        :return: A set of local_names of the target object in the frame.
+        :return: The local names of the target object in the frame.
         """
         return _filter_container(
             frame.f_locals,
             extractor_func=lambda x: x.items(),
             filter_func=lambda x: x[1] is target_object,
             selector_func=lambda x: f"{frame.f_code.co_name}.{x[0]} ({_TYPE_LOCAL})",
         )
@@ -365,20 +350,20 @@
                     # Don't go any further down the stack for this thread if we've found some
                     # names for the object in this frame.
                     if frame_names:
                         names.update(frame_names)
                         break
         return names
 
-    def _get_frame_names(self, frame: FrameType, target_object: Any) -> Set[str]:
+    def _get_frame_names(self, frame: FrameType, target_object: Any) -> Iterable[str]:
         """
         Gets the local_names of the target object in the local variables of the frame.
         :param frame: The frame to search.
         :param target_object: The object to search for.
-        :return: A set of local_names of the target object in the frame.
+        :return: The global names of the target object in the frame.
         """
         return _filter_container(
             frame.f_globals,
             extractor_func=lambda x: x.items(),
             filter_func=lambda x: x[1] is target_object,
             selector_func=self._selector_func,
         )
@@ -616,34 +601,44 @@
                     module_prefixes = [f"{frame_module.split('.')[0]}."]
                     break
         if not module_prefixes:
             raise ValueError(
                 "Could not determine the top-level package of the calling code. "
                 "Please specify the module_prefixes parameter to set this explicitly."
             )
+
+        # Populate a dict of object IDs to the closures that enclose them.
+        # This is used for finding referrers that are closures, and identifying
+        # the name of the variable that is enclosed.
         self._id_to_enclosing_closure = self._get_closure_functions()
+
+        self._target_objects = target_objects
+
         excluded_id_set = {
             id(self),
             id(self.__dict__),
             id(target_objects),
             id(self._id_to_enclosing_closure),
         } | set(exclude_object_ids)
-        self._target_objects = target_objects
+
+        # Get the referrers of the target objects that are not tracked by the garbage collector.
         (
             self._untracked_objects_referrers,
             extra_exclusions,
         ) = self._get_untracked_object_referrers(
             target_objects,
             excluded_id_set=excluded_id_set,
             max_depth=max_untracked_search_depth,
             module_prefixes=module_prefixes,
         )
+
         # Note: when we create the name finders is important because some implementations
         # start to track the objects that are in the environment when they are created.
         self._name_finders = _get_name_finders(module_prefixes)
+
         # Exclude the builder and its attributes from the referrer name finders, since we
         # store a reference to the target objects. Also exclude the target objects container.
         self._referrer_name_finders = _get_referrer_name_finders(
             excluded_id_set | extra_exclusions
         )
 
     def build(self, max_depth: Optional[int]) -> ReferrerGraph:
@@ -777,19 +772,17 @@
         do_not_visit = copy(excluded_id_set)
         do_not_visit.add(id(return_dict))
 
         untracked_target_object_ids = {
             id(obj) for obj in target_objects if not gc.is_tracked(obj)
         }
 
-        # Look through the referents of all locals and globals to try and find
-        # untracked objects.
         if len(untracked_target_object_ids) > 0:
 
-            roots = self._get_roots_from_locals_globals_and_modules(
+            roots = self._get_untracked_search_roots(
                 do_not_visit=do_not_visit,
                 module_prefixes=module_prefixes,
             )
             # Make sure we don't visit the roots list, or very strange things will happen!
             do_not_visit.add(id(roots))
             # Also add the roots to the excluded set. It's not clear why this is necessary,
             # but it seems to be.
@@ -820,76 +813,112 @@
         do_not_visit: Set[int],
         untracked_object_referrers: Dict[int, List],
         untracked_target_object_ids: Set[int],
         untracked_stack: Deque[Any],
         depth: int,
         max_depth: int,
     ):
-        # This method is pretty horrible. It can maybe be made less complex.
+        """
+        Populates the referrers of untracked objects, where the object chain leads to one of
+        the target objects we are looking for. This is a recursive function that walks the
+        object graph, starting from the roots.
+        """
+        # This method is a bit horrible. It can maybe be made less complex.
+        # The fact that we're using a stack *and* recursing is a bit weird, so
+        # I'm pretty sure that can be fixed.
         obj_id = id(obj)
         if inspect.isframe(obj) or obj_id in do_not_visit or depth >= max_depth:
             return
         else:
             do_not_visit.add(obj_id)
             for referent in gc.get_referents(obj):
-                referent_id = id(referent)
-                is_tracked = gc.is_tracked(referent)
-                pop = False
-                # Push untracked objects or objects that are referred to by untracked objects
-                # onto the stack (though I'm not sure if this is possible).
-                if (not is_tracked) or len(untracked_stack) > 0:
+                if not gc.is_tracked(referent):
+                    referent_id = id(referent)
+                    # Push the referrer of the untracked object on to the stack.
+                    # We will pop this off when we return from the recursion.
                     untracked_stack.append(obj)
-                    pop = True
-                # If we find one of the target objects, add the current object to the
-                # referrers list for the target object. We also walk back up the untracked
-                # object stack and add any other untracked objects that refer indirectly
-                # to the target object.
-                if referent_id in untracked_target_object_ids:
-                    id_to_add = referent_id
-                    for untracked_obj in reversed(untracked_stack):
-                        untracked_object_referrers[id_to_add].append(untracked_obj)
-                        id_to_add = id(untracked_obj)
-                # Recurse into the referent. The exit condition is when we find a referent
-                # that is in the do_not_visit set, or when we reach the maximum depth.
-                self._populate_untracked_object_referrers(
-                    obj=referent,
-                    do_not_visit=do_not_visit,
-                    untracked_object_referrers=untracked_object_referrers,
-                    untracked_target_object_ids=untracked_target_object_ids,
-                    untracked_stack=untracked_stack,
-                    depth=depth + 1,
-                    max_depth=max_depth,
-                )
-                if pop:
+                    # If we find one of the target objects, add the current object to the
+                    # referrers list for the target object. We also walk back up the untracked
+                    # object stack and add any other objects that refer indirectly
+                    # to the target object.
+                    if referent_id in untracked_target_object_ids:
+                        id_to_add = referent_id
+                        for untracked_obj in reversed(untracked_stack):
+                            untracked_object_referrers[id_to_add].append(untracked_obj)
+                            id_to_add = id(untracked_obj)
+                    # Recurse into the referent. The exit condition is when we encounter an
+                    # object in the do_not_visit list, we hit the max depth, or we find a
+                    # tracked object (but I'm not sure that untracked objects can refer
+                    # to tracked objects, so this last case may not happen in practice).
+                    self._populate_untracked_object_referrers(
+                        obj=referent,
+                        do_not_visit=do_not_visit,
+                        untracked_object_referrers=untracked_object_referrers,
+                        untracked_target_object_ids=untracked_target_object_ids,
+                        untracked_stack=untracked_stack,
+                        depth=depth + 1,
+                        max_depth=max_depth,
+                    )
                     untracked_stack.pop()
 
-    def _get_roots_from_locals_globals_and_modules(
+    def _contains_untracked_objects(self, obj: Any):
+        return any(not gc.is_tracked(referent) for referent in gc.get_referents(obj))
+
+    def _get_untracked_search_roots(
         self, do_not_visit: Set[int], module_prefixes: Optional[Collection[str]] = None
     ) -> List[Any]:
+        """
+        Gets "root" objects from which to search for untracked objects. We search in all
+        objects that have untracked referents, from within:
+
+         * The result of gc.get_objects()
+         * Local variables
+         * Global variables
+         * Module-level variables that are no global variables.
+        """
         roots = []
+
+        for obj in gc.get_objects():
+            if self._contains_untracked_objects(obj):
+                roots.append(obj)
+
         for thread_frames in _get_frames_for_all_threads().values():
             for frame in thread_frames:
                 # Exclude the locals and globals themselves from the search.
                 do_not_visit.add(id(frame.f_locals))
                 do_not_visit.add(id(frame.f_globals))
-                for var_value in chain(
-                    frame.f_locals.values(), frame.f_globals.values()
-                ):
-                    roots.append(var_value)
+                roots.extend(
+                    _filter_container(
+                        frame.f_locals,
+                        extractor_func=lambda x: x.values(),
+                        filter_func=lambda x: self._contains_untracked_objects(x),
+                        selector_func=lambda x: x,
+                    )
+                )
+                roots.extend(
+                    _filter_container(
+                        frame.f_globals,
+                        extractor_func=lambda x: x.values(),
+                        filter_func=lambda x: self._contains_untracked_objects(x),
+                        selector_func=lambda x: x,
+                    )
+                )
+
+        self._global_vars = _get_global_vars()
         self._modules = [
             module
             for name, module in sys.modules.items()
             if self._matches_prefixes(name, module_prefixes)
         ]
-        self._global_vars = _get_global_vars()
         for module in self._modules:
             if hasattr(module, "__dict__"):
                 for var_name, var_value in module.__dict__.items():
                     if (
-                        _GlobalVariable(var_name, id(var_value), id(module))
+                        self._contains_untracked_objects(var_value)
+                        and _GlobalVariable(var_name, id(var_value), id(module))
                         not in self._global_vars
                     ):
                         roots.append(var_value)
         return roots
 
     def _matches_prefixes(self, module_name: str, module_prefixes: Collection[str]):
         return any(module_name.startswith(prefix) for prefix in module_prefixes)
@@ -956,15 +985,24 @@
     """
     Gets the names and IDs of all global variables in the current environment.
     :return: A set of `_GlobalVariable`s
     """
     global_vars: Set[_GlobalVariable] = set()
     for thread_frames in _get_frames_for_all_threads().values():
         for frame in thread_frames:
-            for var_name, var_value in frame.f_globals.items():
+            # We use filter_container here just to be more robust to modification of
+            # f_globals during iteration. I've never seen this in practice, but I
+            # *think* it's a possibility.
+            global_tuples = _filter_container(
+                frame.f_globals,
+                extractor_func=lambda x: x.items(),
+                filter_func=lambda x: True,
+                selector_func=lambda x: x,
+            )
+            for var_name, var_value in global_tuples:
                 module = inspect.getmodule(var_value)
                 if module:
                     global_vars.add(
                         _GlobalVariable(var_name, id(var_value), id(module))
                     )
                 else:
                     global_vars.add(_GlobalVariable(var_name, id(var_value), None))
@@ -991,38 +1029,38 @@
 
 
 def _filter_container(
     container: Any,
     extractor_func: Callable[[Any], Iterable[_T]],
     filter_func: Callable[[_T], bool],
     selector_func: Callable,
-) -> Set[_V]:
+) -> Iterable[_V]:
     """
     Filters a container using the given functions.
 
     This function is robust to containers being modified while we're iterating over them.
     If a RuntimeError is raised, we make a copy of the container and try again.
 
     :param container: The container to filter.
     :param extractor_func: A function that creates an iterable from the container
     :param filter_func: A function that filters items from the iterable
     :param selector_func: A function that selects items from the iterable
-    :return: A set of selected items.
+    :return: The selected items.
     """
     try:
-        return {
+        return [
             selector_func(item)
             for item in extractor_func(container)
             if filter_func(item)
-        }
+        ]
     except RuntimeError as e:
         # If we get a RuntimeError, it's likely that the iterable is being modified while
         # we're iterating over it. In this case we make a copy of the container and try again.
         logger.warning(
             f"Runtime error encountered while iterating over a container: {e}"
             f"Retrying with a copy."
         )
-        return {
+        return [
             selector_func(item)
             for item in extractor_func(copy(container))
             if filter_func(item)
-        }
+        ]
```

### Comparing `referrers-0.4.3/PKG-INFO` & `referrers-0.5.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: referrers
-Version: 0.4.3
-Summary: Finds the graph of referrers for a Python object
-Author: Neil Ferguson
-Requires-Python: >=3.8
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: networkx (>=3.1.0)
-Description-Content-Type: text/markdown
-
 # Referrers
 
 Referrers is a Python package that helps to answer the question **"what is holding
 a reference to this object?"**, which is useful for debugging memory leaks and other
 issues. It tries to assign a meaningful name to each reference to an object and
 returns a graph of referrers (including indirect referrers).
 
@@ -122,19 +107,19 @@
 top_10_objects = (muppy.sort(muppy.get_objects()))[-10:]
 top_10_objects.reverse()
 
 for obj in top_10_objects:
     print(
         referrers.get_referrer_graph(
             obj,
-            search_for_untracked_objects=True,
             exclude_object_ids=[id(top_10_objects)],
         )
     )
 
+
 ```
 
 Note that this example sets the `search_for_untracked_objects` flag to `True` to try to find
 referrers for objects that are not tracked by the garbage collector. It also sets
 `exclude_object_ids` to exclude the `top_10_objects` variable from the graph.
 
 Here's how to find the referrers of all objects that have been created
@@ -155,15 +140,14 @@
 summary.print_(summary.get_diff(summary.summarize(o1), summary.summarize(o2)))
 
 for obj in diff:
     print(
         referrers.get_referrer_graph(
             obj,
             exclude_object_ids=[id(o1), id(o2), id(diff), id(o2_ids)],
-            search_for_untracked_objects=True,
         )
     )
 ```
 
 This will print a summary of the objects that have been created between o1 and o2,
 as well as the variable names that reference these objects. This can be useful for finding
 memory leaks.
@@ -201,65 +185,14 @@
         with_labels=True,
     )
     plt.show()
 
 my_function()
 ```
 
-## Untracked Objects
-
-By default, `get_referrer_graph` will raise an error if the object passed to it is not
-tracked by the garbage collector. In CPython, for example, immutable objects and some
-containers that contain only immutable objects (like dicts and tuples) are not tracked
-by the garbage collector.
-
-However, the `search_for_untracked_objects` flag can be set to `True` when calling
-`get_referrer_graph` to try to find referrers for objects are not tracked by the garbage
-collector. This option is experimental and may not work well in all cases.
-
-For example, here we find the referrers of an untracked object (a `dict` containing only
-immutable objects):
-
-```python
-import dataclasses
-import gc
-from typing import Dict
-
-import referrers
-
-@dataclasses.dataclass
-class ParentClass:
-    member_variable: Dict
-
-def my_func():
-    local_variable = ParentClass({"a": 1})
-    assert not gc.is_tracked(local_variable.member_variable)
-    print(referrers.get_referrer_graph(local_variable.member_variable, search_for_untracked_objects=True))
-
-my_func()
-```
-
-This will output something like:
-
-```plaintext
-╙── dict instance (id=4483928640)
-    └─╼ ParentClass.member_variable (instance attribute) (id=4482048576)
-        └─╼ my_func.local_variable (local) (id=4482048576)
-```
-
-### Known limitations with untracked objects
-
-* The depth of the search for untracked objects is limited by the `max_untracked_search_depth`
-  parameter. If this is set too low, some untracked objects may be missing from the graph.
-  Try setting this to a higher value if you think this is happening
-* Sometimes internal references (from within `referrers`) may be included in the graph when
-  finding untracked objects. It should be possible to get rid of these, but I'm not sure if I've
-  found them all yet.
-* Finding untracked objects may be slow.
-
 ## Multi-threading
 
 Referrers works well with multiple threads. For example, you can have a separate thread that
 prints the referrers of objects that have references in other threads.
 
 In the following example, there is a thread that prints the referrers of all instances of
 `ChildClass` every second (using [Pympler](https://pympler.readthedocs.io/en/latest/) to find
@@ -293,11 +226,48 @@
     child_variable = ChildClass()
     container_variable = ContainerClass(child_variable)
     sleep(1000)
 
 my_function()
 ```
 
+## Untracked Objects
+
+This library will try to find referrers for objects that are not tracked by the garbage
+collector. For example, mutable objects, and collections containing only immutable objects in
+CPython. However, this may be slower than for tracked objects, and is limited by the
+`max_untracked_search_depth` parameter. Try setting this to a higher value if you think there
+are referrers missing from the graph.
+
+For example, here we find the referrers of an untracked object (a `dict` containing only
+immutable objects):
+
+```python
+import dataclasses
+import gc
+from typing import Dict
+
+import referrers
+
+@dataclasses.dataclass
+class ParentClass:
+    member_variable: Dict
+
+def my_func():
+    local_variable = ParentClass({"a": 1})
+    assert not gc.is_tracked(local_variable.member_variable)
+    print(referrers.get_referrer_graph(local_variable.member_variable))
+
+my_func()
+```
+
+This will output something like:
+
+```plaintext
+╙── dict instance (id=4483928640)
+    └─╼ ParentClass.member_variable (instance attribute) (id=4482048576)
+        └─╼ my_func.local_variable (local) (id=4482048576)
+```
+
 ## Source
 
 See [https://github.com/nfergu/referrers](https://github.com/nfergu/referrers) for the Github repo.
-
```

