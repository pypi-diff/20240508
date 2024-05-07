# Comparing `tmp/beepy_web-0.9.9.tar.gz` & `tmp/beepy_web-10.0.0.tar.gz`

## Comparing `beepy_web-0.9.9.tar` & `beepy_web-10.0.0.tar`

### file list

```diff
@@ -1,56 +1,58 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 beepy_web-0.9.9/.env.template
--rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 beepy_web-0.9.9/.pre-commit-config.yaml
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 beepy_web-0.9.9/.python-version
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 beepy_web-0.9.9/.readthedocs.yml
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 beepy_web-0.9.9/requirements.txt
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 beepy_web-0.9.9/beepy/__init__.py
--rw-r--r--   0        0        0    14637 2020-02-02 00:00:00.000000 beepy_web-0.9.9/beepy/attrs.py
--rw-r--r--   0        0        0     7171 2020-02-02 00:00:00.000000 beepy_web-0.9.9/beepy/children.py
--rw-r--r--   0        0        0    12814 2020-02-02 00:00:00.000000 beepy_web-0.9.9/beepy/components.py
--rw-r--r--   0        0        0     8577 2020-02-02 00:00:00.000000 beepy_web-0.9.9/beepy/context.py
--rw-r--r--   0        0        0    21072 2020-02-02 00:00:00.000000 beepy_web-0.9.9/beepy/framework.py
--rw-r--r--   0        0        0     5423 2020-02-02 00:00:00.000000 beepy_web-0.9.9/beepy/listeners.py
--rw-r--r--   0        0        0     4598 2020-02-02 00:00:00.000000 beepy_web-0.9.9/beepy/router.py
--rw-r--r--   0        0        0     8083 2020-02-02 00:00:00.000000 beepy_web-0.9.9/beepy/style.py
--rw-r--r--   0        0        0     5310 2020-02-02 00:00:00.000000 beepy_web-0.9.9/beepy/tags.py
--rw-r--r--   0        0        0     6671 2020-02-02 00:00:00.000000 beepy_web-0.9.9/beepy/trackable.py
--rw-r--r--   0        0        0     4631 2020-02-02 00:00:00.000000 beepy_web-0.9.9/beepy/types.py
--rwxr-xr-x   0        0        0     5190 2020-02-02 00:00:00.000000 beepy_web-0.9.9/beepy/dev/__init__.py
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 beepy_web-0.9.9/beepy/dev/__main__.py
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 beepy_web-0.9.9/beepy/dev/example.html
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 beepy_web-0.9.9/beepy/dev/example.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 beepy_web-0.9.9/beepy/modules/__init__.py
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 beepy_web-0.9.9/beepy/modules/actions.py
--rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 beepy_web-0.9.9/beepy/modules/context_menu.py
--rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 beepy_web-0.9.9/beepy/modules/local_storage.py
--rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 beepy_web-0.9.9/beepy/modules/modal.py
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 beepy_web-0.9.9/beepy/modules/plot.py
--rw-r--r--   0        0        0     5067 2020-02-02 00:00:00.000000 beepy_web-0.9.9/beepy/modules/table.py
--rw-r--r--   0        0        0     4845 2020-02-02 00:00:00.000000 beepy_web-0.9.9/beepy/modules/tabs.py
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 beepy_web-0.9.9/beepy/utils/__init__.py
--rw-r--r--   0        0        0     2088 2020-02-02 00:00:00.000000 beepy_web-0.9.9/beepy/utils/api.py
--rw-r--r--   0        0        0     2489 2020-02-02 00:00:00.000000 beepy_web-0.9.9/beepy/utils/asyncio.py
--rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 beepy_web-0.9.9/beepy/utils/common.py
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 beepy_web-0.9.9/beepy/utils/dev.py
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 beepy_web-0.9.9/beepy/utils/import_hooks.py
--rw-r--r--   0        0        0     2560 2020-02-02 00:00:00.000000 beepy_web-0.9.9/beepy/utils/internal.py
--rw-r--r--   0        0        0     8427 2020-02-02 00:00:00.000000 beepy_web-0.9.9/beepy/utils/js.py
--rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 beepy_web-0.9.9/beepy/utils/js_py.py
--rwxr-xr-x   0        0        0      163 2020-02-02 00:00:00.000000 beepy_web-0.9.9/scripts/dev.sh
--rwxr-xr-x   0        0        0      691 2020-02-02 00:00:00.000000 beepy_web-0.9.9/scripts/publish.sh
--rw-r--r--   0        0        0   179387 2020-02-02 00:00:00.000000 beepy_web-0.9.9/web/package-lock.json
--rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 beepy_web-0.9.9/web/package.json
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 beepy_web-0.9.9/web/webpack.dev.js
--rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 beepy_web-0.9.9/web/webpack.prod.js
--rw-r--r--   0        0        0     7650 2020-02-02 00:00:00.000000 beepy_web-0.9.9/web/src/beepy.js
--rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 beepy_web-0.9.9/web/src/dev-server.js
--rw-r--r--   0        0        0     3027 2020-02-02 00:00:00.000000 beepy_web-0.9.9/web/src/files.js
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 beepy_web-0.9.9/web/src/index.js
--rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 beepy_web-0.9.9/web/src/main.css
--rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 beepy_web-0.9.9/web/src/python.js
--rw-r--r--   0        0        0     2487 2020-02-02 00:00:00.000000 beepy_web-0.9.9/web/src/utils.js
--rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 beepy_web-0.9.9/.gitignore
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 beepy_web-0.9.9/LICENSE
--rw-r--r--   0        0        0     2816 2020-02-02 00:00:00.000000 beepy_web-0.9.9/README.md
--rw-r--r--   0        0        0     3304 2020-02-02 00:00:00.000000 beepy_web-0.9.9/pyproject.toml
--rw-r--r--   0        0        0     3996 2020-02-02 00:00:00.000000 beepy_web-0.9.9/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 beepy_web-10.0.0/.env.template
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 beepy_web-10.0.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 beepy_web-10.0.0/.python-version
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 beepy_web-10.0.0/.readthedocs.yml
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 beepy_web-10.0.0/requirements.txt
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 beepy_web-10.0.0/beepy/__init__.py
+-rw-r--r--   0        0        0    14637 2020-02-02 00:00:00.000000 beepy_web-10.0.0/beepy/attrs.py
+-rw-r--r--   0        0        0     7171 2020-02-02 00:00:00.000000 beepy_web-10.0.0/beepy/children.py
+-rw-r--r--   0        0        0    12814 2020-02-02 00:00:00.000000 beepy_web-10.0.0/beepy/components.py
+-rw-r--r--   0        0        0     9757 2020-02-02 00:00:00.000000 beepy_web-10.0.0/beepy/context.py
+-rw-r--r--   0        0        0    21327 2020-02-02 00:00:00.000000 beepy_web-10.0.0/beepy/framework.py
+-rw-r--r--   0        0        0     5423 2020-02-02 00:00:00.000000 beepy_web-10.0.0/beepy/listeners.py
+-rw-r--r--   0        0        0     5036 2020-02-02 00:00:00.000000 beepy_web-10.0.0/beepy/router.py
+-rw-r--r--   0        0        0     8083 2020-02-02 00:00:00.000000 beepy_web-10.0.0/beepy/style.py
+-rw-r--r--   0        0        0     5453 2020-02-02 00:00:00.000000 beepy_web-10.0.0/beepy/tags.py
+-rw-r--r--   0        0        0     6671 2020-02-02 00:00:00.000000 beepy_web-10.0.0/beepy/trackable.py
+-rw-r--r--   0        0        0     4631 2020-02-02 00:00:00.000000 beepy_web-10.0.0/beepy/types.py
+-rwxr-xr-x   0        0        0     5461 2020-02-02 00:00:00.000000 beepy_web-10.0.0/beepy/dev/__init__.py
+-rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 beepy_web-10.0.0/beepy/dev/__main__.py
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 beepy_web-10.0.0/beepy/dev/example.html
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 beepy_web-10.0.0/beepy/dev/example.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 beepy_web-10.0.0/beepy/modules/__init__.py
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 beepy_web-10.0.0/beepy/modules/actions.py
+-rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 beepy_web-10.0.0/beepy/modules/context_menu.py
+-rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 beepy_web-10.0.0/beepy/modules/local_storage.py
+-rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 beepy_web-10.0.0/beepy/modules/modal.py
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 beepy_web-10.0.0/beepy/modules/plot.py
+-rw-r--r--   0        0        0     5067 2020-02-02 00:00:00.000000 beepy_web-10.0.0/beepy/modules/table.py
+-rw-r--r--   0        0        0     4845 2020-02-02 00:00:00.000000 beepy_web-10.0.0/beepy/modules/tabs.py
+-rw-r--r--   0        0        0     2806 2020-02-02 00:00:00.000000 beepy_web-10.0.0/beepy/ssr/__init__.py
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 beepy_web-10.0.0/beepy/ssr/extra.js
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 beepy_web-10.0.0/beepy/utils/__init__.py
+-rw-r--r--   0        0        0     2088 2020-02-02 00:00:00.000000 beepy_web-10.0.0/beepy/utils/api.py
+-rw-r--r--   0        0        0     2489 2020-02-02 00:00:00.000000 beepy_web-10.0.0/beepy/utils/asyncio.py
+-rw-r--r--   0        0        0     3500 2020-02-02 00:00:00.000000 beepy_web-10.0.0/beepy/utils/common.py
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 beepy_web-10.0.0/beepy/utils/dev.py
+-rw-r--r--   0        0        0     2058 2020-02-02 00:00:00.000000 beepy_web-10.0.0/beepy/utils/import_hooks.py
+-rw-r--r--   0        0        0     2959 2020-02-02 00:00:00.000000 beepy_web-10.0.0/beepy/utils/internal.py
+-rw-r--r--   0        0        0     9145 2020-02-02 00:00:00.000000 beepy_web-10.0.0/beepy/utils/js.py
+-rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 beepy_web-10.0.0/beepy/utils/js_py.py
+-rwxr-xr-x   0        0        0      163 2020-02-02 00:00:00.000000 beepy_web-10.0.0/scripts/dev.sh
+-rwxr-xr-x   0        0        0      688 2020-02-02 00:00:00.000000 beepy_web-10.0.0/scripts/publish.sh
+-rw-r--r--   0        0        0   179389 2020-02-02 00:00:00.000000 beepy_web-10.0.0/web/package-lock.json
+-rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 beepy_web-10.0.0/web/package.json
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 beepy_web-10.0.0/web/webpack.dev.js
+-rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 beepy_web-10.0.0/web/webpack.prod.js
+-rw-r--r--   0        0        0     8414 2020-02-02 00:00:00.000000 beepy_web-10.0.0/web/src/beepy.js
+-rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 beepy_web-10.0.0/web/src/dev-server.js
+-rw-r--r--   0        0        0     3300 2020-02-02 00:00:00.000000 beepy_web-10.0.0/web/src/files.js
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 beepy_web-10.0.0/web/src/index.js
+-rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 beepy_web-10.0.0/web/src/main.css
+-rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 beepy_web-10.0.0/web/src/python.js
+-rw-r--r--   0        0        0     2700 2020-02-02 00:00:00.000000 beepy_web-10.0.0/web/src/utils.js
+-rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 beepy_web-10.0.0/.gitignore
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 beepy_web-10.0.0/LICENSE
+-rw-r--r--   0        0        0     2823 2020-02-02 00:00:00.000000 beepy_web-10.0.0/README.md
+-rw-r--r--   0        0        0     3432 2020-02-02 00:00:00.000000 beepy_web-10.0.0/pyproject.toml
+-rw-r--r--   0        0        0     4116 2020-02-02 00:00:00.000000 beepy_web-10.0.0/PKG-INFO
```

### Comparing `beepy_web-0.9.9/.pre-commit-config.yaml` & `beepy_web-10.0.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.9/beepy/__init__.py` & `beepy_web-10.0.0/beepy/__init__.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.9/beepy/attrs.py` & `beepy_web-10.0.0/beepy/attrs.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.9/beepy/children.py` & `beepy_web-10.0.0/beepy/children.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.9/beepy/components.py` & `beepy_web-10.0.0/beepy/components.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.9/beepy/context.py` & `beepy_web-10.0.0/beepy/context.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import enum
 from abc import ABCMeta
 from typing import TYPE_CHECKING, Self
 
 import beepy
 from beepy.attrs import attr, html_attr, state, state_move_on
-from beepy.utils import js
+from beepy.utils import js, __config__, IN_BROWSER
 from beepy.utils.common import get_random_name, log10_ceil, to_kebab_case
 from beepy.utils.js_py import Interval, create_once_callable
 
 if TYPE_CHECKING:
     from beepy.types import AttrType
 
 _base_obj_dir = (*dir(object()), '__abstractmethods__')
@@ -98,27 +98,66 @@
                 extra = {key: value for key, value in extra.items() if key not in namespace}
                 namespace.update(extra)
 
     @classmethod
     def _top_mount(mcs, element):
         parent = element._root_parent
         root = parent.mount_element
-        root.style = 'visibility: hidden'
+        using_ssr = __config__['server_side'] == 'client'
+        if not using_ssr:
+            root.style = 'visibility: hidden'
 
         mcs._current_render[parent] = []
-        element.__mount__(root, parent)
+
+        if using_ssr:
+            element.__mount__(js.beepy.addElement(root, 'template'), parent)
+            element.mount_parent = root
+        else:
+            element.__mount__(root, parent)
 
         mcs._wait_onload_interval[parent] = Interval(mcs._wait_onload, (element,), period=0.2)
 
+        if not IN_BROWSER:
+            mcs._ssr2__finish()
+
+    @classmethod
+    def _ssr2__finish(mcs):
+        # SSR implementation without selenium
+        # I want to try using bs4 instead of js.py mock
+        # Not really working right now
+        import time
+
+        mcs._to_load_before_top_render.clear()
+
+        time.sleep(1)
+
+        for thread in js.threads_to_join:
+            thread.join()
+        js.threads_to_join.clear()
+        for thread in (*js.threads['timeout'].values(), *js.threads['interval'].values()):
+            thread.join()
+
+        print(js.document.documentElement.outerHTML)
+
     @classmethod
     def _top_render(mcs, element):
-        element._root_parent.mount_element.style = ''
-        js.beepy.stopLoading()
+        root = element._root_parent.mount_element
+        using_ssr = __config__['server_side'] == 'client'
+
+        if not using_ssr:
+            root.style = ''
+            js.beepy.stopLoading()
+
         element.__render__()
 
+        if using_ssr:
+            template = element.mount_element.parentElement
+            root.replaceChild(element.mount_element, root.children[0])
+            template.remove()
+
     @classmethod
     def _clean_namespace(mcs, namespace):
         base_obj_dir = _base_obj_dir + mcs.__clean_class_attribute_names
         for key, value in tuple(namespace.items()):
             if key not in base_obj_dir:
                 yield key, value
```

### Comparing `beepy_web-0.9.9/beepy/framework.py` & `beepy_web-10.0.0/beepy/framework.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 from __future__ import annotations
 
 import traceback
 from collections.abc import Callable, Iterable
 from functools import cache
 from types import MethodType
-from typing import ClassVar
+from typing import TYPE_CHECKING
 
 from beepy.attrs import state, state_move_on
 from beepy.children import ChildRef, Children, ContentWrapper, CustomWrapper, StringWrapper, TagRef
 from beepy.components import Component, _MetaComponent
 from beepy.context import SpecialChild
 from beepy.types import AttrType, ContentType, Mounter, Renderer
 from beepy.utils import __config__, js, log
 from beepy.utils.common import NONE_TYPE, get_random_name, to_kebab_case
 from beepy.utils.dev import _debugger
 from beepy.utils.internal import _py_tag_attribute
 
-__version__ = '0.9.9'  # For internal development set to 0.0a0
+if TYPE_CHECKING:
+    from typing import Any, ClassVar
+
+__version__ = '10.0.0'  # For internal development set to 0.0a0
 __config__['version'] = __version__
 
 
 _tag_initialized = False
 
 
 class _MetaTag(_MetaComponent):
@@ -153,24 +156,22 @@
         else:
             cls._static_children = [SpecialChild.CONTENT]
 
         cls._tags = []
 
         mcs._tag_classes.append(cls)
 
-        if initialized and 'mount' in kwargs:
+        # TODO: move logic with `mount=` to StandaloneTag
+        if 'mount' in kwargs:
             cls._root_parent = None
             setattr(cls.mount_element, _py_tag_attribute, cls())
 
-        if cls._meta_root:
-            cls.__root_declared__()
-        else:
-            cls.__class_declared__()
+        result = cls.__root_declared__() if cls._meta_root else cls.__class_declared__()
 
-        return cls
+        return cls if result is None else result
 
 
 class Tag(Component, metaclass=_MetaTag, _root=True):
     # TODO: add docstrings
 
     __slots__ = (
         '_content',
@@ -200,19 +201,19 @@
     _static_children_tag: Tag
     _children_tag: Tag
     _mount_finished_: bool
 
     children: ClassVar[Component | state | SpecialChild | str]
 
     @classmethod
-    def __root_declared__(cls):
+    def __root_declared__(cls) -> Any:
         """This method is called, when root Tag is defined"""
 
     @classmethod
-    def __class_declared__(cls):
+    def __class_declared__(cls) -> Any:
         """This method is called, when common Tag is defined"""
 
     def __mount__(self, *args, **kwargs):
         self.__class__._tags.append(self)
 
         self._mount_finished_ = False
 
@@ -522,25 +523,31 @@
 
 
 def mount(element: Tag, root_element: str, *, clear=False):
     root = js.document.querySelector(root_element)
     if root is None:
         raise NameError('Mount point not found')
 
+    using_ssr = __config__['server_side'] == 'client'
     js.beepy.stopLoading()
     if clear or js.beepy.dev_server.started:
         root.innerHTML = ''
-    js.beepy.startLoading(mountPoint=root)
+
+    if not using_ssr:
+        js.beepy.startLoading(mountPoint=root)
 
     name = root.tagName.lower()
     parent = _MetaTag(name, (Tag,), {'_root_parent': state_move_on(type=Tag)}, name=name, content_tag=None)()
     parent._attrs_defaults['_root_parent'] = parent.__class__._root_parent._default = parent
     parent.mount_element = root
     element._link_parent_attrs(parent)
 
+    if not using_ssr:
+        root.innerHTML = ''
+
     _MetaTag._top_mount(element)
 
     if not js.document.title:
         js.document.title = 'BeePy'
         log.warn(f'Document title is not set, use default title: {js.document.title}')
```

### Comparing `beepy_web-0.9.9/beepy/listeners.py` & `beepy_web-10.0.0/beepy/listeners.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.9/beepy/router.py` & `beepy_web-10.0.0/beepy/router.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import re
 from dataclasses import dataclass
 from re import Match
 
 from beepy import Tag, html_attr, on, state, state_move_on
 from beepy.tags import a
 from beepy.types import Children
-from beepy.utils import js
+from beepy.utils import js, __config__
 from beepy.utils.dev import _debugger
 from beepy.utils.internal import lazy_import_cls, reload_requirements
 from beepy.utils.js_py import push_url
 
 
 class WithRouter:
     match: Match = state_move_on()
@@ -86,26 +86,30 @@
         Path.parse(self.router.basename + self.to).push_state()
         await self.router._history_refresh()
 
 
 class Router(Tag):
     basename = ''
     routes: dict[str, str | type[Tag]] = {
-        # r'/$': Tag,
-        # r'/app/(?P<id>.*)$': 'app.App',  # lazy import!
+        # '/': Root,
+        # '/app/': 'app.App',  # lazy import!
     }
 
     fallback_tag_cls = None
     single_tag = True
+    add_trailing_slash = True
 
     children = [
         components := Children(),
     ]
 
     def pre_mount(self):
+        if __config__['server_side'] == 'server':
+            js.beepy.config._ssr_all_routes.extend([self.basename + route for route in self.routes])
+
         self._load_children()
 
     @on('popstate')
     async def _history_refresh(self):
         js.beepy.startLoading(mountPoint=self._root_parent.mount_element)
         await reload_requirements()
         self._load_children()
@@ -129,26 +133,31 @@
         self._current_render.clear()
 
         old_components = list(self.components)
 
         with self.components.onchange_locker:  # can Locker also be descriptor with auto-replace as in last two lines?
             self.components.clear()
 
+            location = js.location.pathname
+            if self.add_trailing_slash and not location.endswith('/'):
+                location += '/'
+
             for path, tag_cls in self.routes.items():
-                if match := re.search(self.basename + path, js.location.pathname):
+                # TODO: consider support re in some format  /  allow using re.compile() too
+                if match := re.search(f'^{self.basename}{path}$', location):
                     self.add_tag_component(tag_cls, match=match, path=path)
                     if self.single_tag:
                         break
 
             if not self.components:
                 if fallback := self.fallback_tag_cls:
                     self.add_tag_component(fallback, match=None, path=None)
                 else:
                     # TODO: maybe create BeePyError?
                     raise ValueError('No route to use!')
 
-            for child in self.components:
+            for child in self.components:  # TODO: simplify this
                 child._link_parent_attrs(self)
                 child.init(*child._args, _load_children=False, **(child._attrs_defaults | child._kwargs))
 
             new_components, self.components = list(self.components), old_components
         self.components[:] = new_components  # triggers correct onchange handlers
```

### Comparing `beepy_web-0.9.9/beepy/style.py` & `beepy_web-10.0.0/beepy/style.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.9/beepy/tags.py` & `beepy_web-10.0.0/beepy/tags.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any
+from typing import Any, Self
 
 from boltons.typeutils import make_sentinel
 
 from beepy.attrs import attr, html_attr, state
 from beepy.framework import Tag
 from beepy.types import Children
 from beepy.utils import __config__, js
@@ -202,25 +202,29 @@
 
     @classmethod
     def with_items(cls, items: dict[str, Any], **kwargs):
         return cls(options=[option(label=label_, value=value) for value, label_ in items.items()], **kwargs)
 
 
 class StandaloneTag(html_tag, _root=True):
+    @classmethod
+    def __class_declared__(cls) -> Self:
+        return cls()
+
     def __init__(self, *args, **kwargs):
         kwargs['_load_children'] = True
         super().__init__(*args, **kwargs)
 
     def _mount_(self, element, parent: Tag, index=None):  # noqa: ARG002 - unused `index`
         # too many copy-paste?
         self.parent = parent
         self.mount_parent = element
         self.pre_mount()
 
-    def _clone(self, parent=None):  # noqa: ARG002 - arguments for overriding
+    def _clone(self, parent=None):  # noqa: ARG002 - unused `parent`
         return self
 
     def _as_child(self, parent: Tag | None, *, exists_ok=False, inline_def=False):  # noqa: ARG002 - args for overriding
         return super()._as_child(parent, exists_ok=True, inline_def=inline_def)
 
 
 class Head(StandaloneTag, name='head', mount=js.document.head):
@@ -228,22 +232,22 @@
 
     @title.on('change')
     def _upd_title(self):
         if self.title:
             js.document.title = self.title
 
 
-Head = Head()
-
-
 class Body(StandaloneTag, name='body', mount=js.document.body):
-    style = html_attr()
+    pass
 
 
-Body = Body()
+# Fun things are doing inside `mount=` Tags...
+# For type-checking be correct :)
+Head: Head
+Body: Body
 
 
 # TODO: add all HTML tags
 
 
 __all__ = ['html_tag', 'div', 'a', 'p', 'b', 'i', 'ul', 'li', 'span', 'form', 'h1', 'h2', 'h3', 'h4', 'h5', 'h6']
-__all__ += ['input_', 'textarea', 'header', 'main', 'footer', 'nav', 'button', 'option', 'select', 'Head']
+__all__ += ['input_', 'textarea', 'header', 'main', 'footer', 'nav', 'button', 'option', 'select', 'Head', 'Body']
```

### Comparing `beepy_web-0.9.9/beepy/trackable.py` & `beepy_web-10.0.0/beepy/trackable.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.9/beepy/types.py` & `beepy_web-10.0.0/beepy/types.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.9/beepy/dev/__init__.py` & `beepy_web-10.0.0/beepy/dev/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 
 import dotenv
 from watchdog.events import FileSystemEventHandler
 from watchdog.observers import Observer
 from websockets.exceptions import ConnectionClosedOK
 from websockets.server import serve
 
+from beepy.ssr import get_server_html
+
 dotenv.load_dotenv()
 BASE_DIR = Path(__file__).resolve().parent
 
 
 class MonitorFolder(FileSystemEventHandler):
     def __init__(self, server):
         self.server = server
@@ -33,79 +35,86 @@
             or event.src_path.endswith(('~', '.tmp'))
             or re.search(r'/(__pycache__|.git|.idea|dist|build)/', event.src_path)
         ):
             self.server._handle_file_event(event)
 
 
 class DevServer:
-    def __init__(self, *, root_path=None, parse_cmd=True):
+    def __init__(self, *, root=None, port=8888, create=False, ssr=False):
         self.websockets = []
-        self.root_path = root_path
+        self.root = (root or Path.cwd()).resolve()
+        self.port = port
+        self.ssr = ssr
+
         self.observer = None
         self.developer_mode = os.environ.get('DEVELOPMENT') == '1'
-        if parse_cmd:
-            self._handle_cmd_args()
-
-    def _handle_cmd_args(self):
-        parser = argparse.ArgumentParser(prog='beepy.dev', description='Simple dev server for BeePy')
-        parser.add_argument(
-            '-d', '--root-dir', default=Path.cwd(), help='Root directory to start server and watch file changes'
-        )
-        parser.add_argument(
-            '--create', action='store_true', help='Create a default .html, .py and .env files before start'
-        )
-        args = parser.parse_args()
 
-        if not self.root_path:
-            self.root_path = Path(args.root_dir)
+        if create:
+            self._create_default_files()
 
-        if not args.create:
-            return
-
-        dst = self.root_path / 'index.html'
+    def _create_default_files(self):
+        dst = self.root / 'index.html'
 
         if dst.exists():
             print('[BeePy] Warning: File "index.html" already exists, skipping creating default files')
             return
 
         shutil.copyfile(BASE_DIR / 'example.html', dst)
-        shutil.copyfile(BASE_DIR / 'example.py', self.root_path / '__init__.py')
-        shutil.copyfile(BASE_DIR / '../.env', self.root_path / '.env')
+        shutil.copyfile(BASE_DIR / 'example.py', self.root / '__init__.py')
+        shutil.copyfile((BASE_DIR / '../.env').resolve(), self.root / '.env')
         print('[BeePy] Created default files in root directory')
 
+    def _ssr_create_dist(self):
+        if not self.ssr:
+            return
+
+        dist = Path(self.root / 'dist')
+        dist.mkdir(parents=True, exist_ok=True)
+
+        # TODO: add support for Router (load_all_routes=True)
+        ssr_data = get_server_html(f'http://localhost:{self.port}', '/')
+        (dist / 'index.html').write_text(ssr_data)
+        shutil.copyfile(self.root / '__init__.py', dist / '__init__.py')
+        print(f'[BeePy] [SSR] dist is done. Visit: http://localhost:{self.port}')
+
+    def _cleanup(self):
+        if self.ssr:
+            shutil.rmtree(self.root / 'dist', ignore_errors=True)
+
     async def ws_send(self, message):
         await asyncio.sleep(1)  # Hack for Django autoreload
 
         for ws in self.websockets[:]:
             try:
                 await ws.send(message)
             except ConnectionClosedOK:
                 self.websockets.remove(ws)
 
         if not self.websockets:
             print('[BeePy] No clients connected! Please, restart your page to connect to the dev server')
 
     def _handle_file_event(self, event):
-        path: str = event.src_path.removeprefix(str(self.root_path)).removeprefix('/')
+        path: str = event.src_path.removeprefix(str(self.root)).removeprefix('/')
 
         print(f'[BeePy] Found file change: {path}')
         if self.developer_mode:
             if path.endswith('.py'):
                 subprocess.call('hatch build', shell=True)
             elif path.endswith('.js'):
-                subprocess.call(f'cd {self.root_path}/web; npm run build; cd -', shell=True)  # rebuild dist
-            asyncio.run(self.ws_send('__'))
-        else:
-            asyncio.run(self.ws_send(path))
+                subprocess.call(f'cd {self.root}/web; npm run build; cd -', shell=True)  # rebuild dist
+            path = '__'
+
+        self._ssr_create_dist()
+        asyncio.run(self.ws_send(path))
 
     def _watcher_start(self):
         event_handler = MonitorFolder(self)
         observer = Observer()
-        observer.schedule(event_handler, path=self.root_path, recursive=True)
-        print(f'[BeePy] Monitoring started for {self.root_path}')
+        observer.schedule(event_handler, path=str(self.root), recursive=True)
+        print(f'[BeePy] Monitoring started for {self.root}')
         observer.start()
         self.observer = observer
         try:
             while True:
                 time.sleep(1)
         except KeyboardInterrupt:
             observer.stop()
@@ -121,38 +130,42 @@
         print('[BeePy] WebSockets started')
         async with serve(self._ws_echo, 'localhost', 8998):
             await asyncio.Future()  # run forever
 
     def _ws_start(self):
         asyncio.run(self._ws_main())
 
-    def _simple_http_start(self, port=8888):
+    def _simple_http_start(self):
         # Fixes "Address already in use"
         socketserver.TCPServer.allow_reuse_address = True
 
         with socketserver.TCPServer(
-            ('', port), functools.partial(http.server.SimpleHTTPRequestHandler, directory=self.root_path)
+            ('', self.port), functools.partial(http.server.SimpleHTTPRequestHandler, directory=self.root)
         ) as httpd:
-            print(f'[BeePy] Serving at port {port}\nOpen server: http://localhost:{port}')
-            httpd.serve_forever()
+            print(f'[BeePy] Serving at port {self.port}\nOpen server: http://localhost:{self.port}')
+            try:
+                httpd.serve_forever()
+            finally:
+                self._cleanup()
 
-    def start(self, *, start_http=True, forever=True):
+    def start(self, *, start_http=False, forever=True):
         if self.observer is not None:
             print('[BeePy] Server is already started')
             return
 
         Thread(target=self._ws_start, daemon=True).start()
         Thread(target=self._watcher_start, daemon=True).start()
 
         if not start_http:
             return
 
         if start_http is True:
             start_http = self._simple_http_start
 
+        thread = Thread(target=start_http, daemon=True)
+        thread.start()
+        self._ssr_create_dist()
         if forever:
-            start_http()
-        else:
-            Thread(target=start_http, daemon=True).start()
+            thread.join()
 
 
 __all__ = ['DevServer']
```

### Comparing `beepy_web-0.9.9/beepy/modules/context_menu.py` & `beepy_web-10.0.0/beepy/modules/context_menu.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.9/beepy/modules/local_storage.py` & `beepy_web-10.0.0/beepy/modules/local_storage.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.9/beepy/modules/modal.py` & `beepy_web-10.0.0/beepy/modules/modal.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.9/beepy/modules/table.py` & `beepy_web-10.0.0/beepy/modules/table.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.9/beepy/modules/tabs.py` & `beepy_web-10.0.0/beepy/modules/tabs.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.9/beepy/utils/api.py` & `beepy_web-10.0.0/beepy/utils/api.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.9/beepy/utils/asyncio.py` & `beepy_web-10.0.0/beepy/utils/asyncio.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.9/beepy/utils/common.py` & `beepy_web-10.0.0/beepy/utils/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import inspect
 import math
-import random
 import re
 import string
 
 from boltons.typeutils import make_sentinel
 
+from beepy.utils.internal import rnd
+
 NONE_TYPE = type(None)
 MISSING = make_sentinel(var_name='MISSING')
 
 
 def log10_ceil(num):
     return math.ceil(math.log10(num or 1)) or 1
 
@@ -56,15 +57,15 @@
     return s
 
 
 _w = string.ascii_letters + string.digits + '_'
 
 
 def get_random_name(length=6):
-    return ''.join(random.choice(_w) for _ in range(length))
+    return ''.join(rnd.choice(_w) for _ in range(length))
 
 
 def safe_issubclass(type_or_Any, class_or_tuple_to_check):
     try:
         return issubclass(type_or_Any, class_or_tuple_to_check)
     except TypeError:
         return False
```

### Comparing `beepy_web-0.9.9/beepy/utils/dev.py` & `beepy_web-10.0.0/beepy/utils/dev.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.9/beepy/utils/import_hooks.py` & `beepy_web-10.0.0/beepy/utils/import_hooks.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from importlib.util import spec_from_file_location
 from pathlib import Path
 
 from pyodide.ffi import JsException
 
 from beepy.utils.dev import _debugger
 from beepy.utils.internal import __config__, _beepy_root_package
+from beepy.utils.common import get_random_name
 from beepy.utils.js_py import IN_BROWSER, js
 
 requirements = __config__['requirements']
 _modules_not_existing_on_server = [
     _beepy_root_package,
     *(requirements() if callable(requirements) else requirements),
     '_hashlib',  # TODO: FIX THIS...
@@ -52,20 +53,23 @@
     def find_spec(self, fullname, path, target=None):  # noqa: ARG002 - override of MetaPathFinder
         if path and any(p.startswith('/lib') for p in path):
             return
 
         if Path(f'/lib/python3.11/site-packages/{fullname}').exists() or fullname in _modules_not_existing_on_server:
             return
 
-        current_path = js.beepy.files._lastLoadedFile
+        Files = js.beepy.files
+        current_path = Files._lastLoadedFile
+        Files._devExtraQuery = get_random_name(3)
 
         try:
             js.beepy.loadModule(fullname)
         except JsException as err:
-            js.beepy.files._lastLoadedFile = current_path
+            Files._lastLoadedFile = current_path
+            Files._devExtraQuery = ''
             _debugger(err)
             _modules_not_existing_on_server.append(fullname)
             return
 
         return spec_from_file_location(fullname)
```

### Comparing `beepy_web-0.9.9/beepy/utils/internal.py` & `beepy_web-10.0.0/beepy/utils/internal.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import asyncio
 import os
+import random
 import sys
 from importlib import import_module
 from typing import TYPE_CHECKING
 
 import dotenv
 import micropip
 
@@ -13,23 +14,26 @@
     from collections.abc import Callable
 
 _beepy_root_package = '__beepy_root__'
 _py_tag_attribute = '__PYTHON_TAG__'
 
 dotenv.load_dotenv(f'{_beepy_root_package}/.env' if IN_BROWSER else '.env')
 
-# TODO: make it with dataclass
+# TODO: make it with dataclass?
+# TODO: consider using .toml/.yaml usage instead of .env + window.beepy.config
 __config__ = {
     'debug': os.environ.get('DEBUG') == '1',
     'development': os.environ.get('DEVELOPMENT') == '1',
     'style_head': True,
     'api_url': '/',
     'default_datetime_format': '%Y-%m-%dT%H:%M:%S.%f%Z',
     'inputs_auto_id': True,
     'html_replace_whitespaces': True,
+    'random_seed': int(os.environ.get('RANDOM_SEED', 0)),
+    'server_side': '',
     'requirements': [],
 }
 
 
 def merge_configs():
     __config__.update(js.beepy.config.to_py())
     js.beepy.config = to_js(__config__)
@@ -65,19 +69,26 @@
 
 def lazy_import_cls(cls):
     if isinstance(cls, str):
         return import_string(cls)
     return cls
 
 
+def get_seed():
+    if not __config__['random_seed']:
+        __config__['random_seed'] = int.from_bytes(os.urandom(8), 'big')
+    return __config__['random_seed']
+
+
 def _init_js():
     from beepy import __version__
 
     js.console.log(f'%cBeePy version: {__version__}', 'color: lightgreen; font-size: 35px')
     merge_configs()
+    rnd.seed(get_seed())
 
 
 class _BeePyGlobals(dict):
     def __getitem__(self, key):
         result = super().__getitem__(key)
         for handler in __beepy_global_handlers__:
             result = handler(self, key, result)
@@ -87,19 +98,21 @@
 def _default_global_handlers(locals_dict, key, result):
     if key.startswith('_p__'):
         return result(locals_dict)
     return result
 
 
 __beepy_global_handlers__ = [_default_global_handlers]
+rnd = random.Random()
 
 
 __all__ = [
     '_py_tag_attribute',
     '__config__',
     'merge_configs',
     'lazy_import',
     'import_string',
     'lazy_import_cls',
     'reload_requirements',
     '__beepy_global_handlers__',
+    'rnd',
 ]
```

### Comparing `beepy_web-0.9.9/beepy/utils/js.py` & `beepy_web-10.0.0/beepy/utils/js.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,80 +20,90 @@
     __PYTHON_TAG__: Tag
 
     def __init__(self, tag_name, *, _parent=None):
         self.attributes = {}
         self.data = []
         self.listeners = defaultdict(list)
         self.tagName = tag_name
-        self.shadowRoot = None
         self.clientWidth = self.clientHeight = self.scrollWidth = self.scrollHeight = 1
         self.parentElement = _parent
 
     def getAttribute(self, name):
         return self.attributes.get(name)
 
     def setAttribute(self, name, value):
         self.attributes[name] = value
 
     def removeAttribute(self, name):
         self.attributes.pop(name, None)
 
     def append(self, string: str):
         self.data.append(string)
-        print(self)
 
     def appendChild(self, el: HTMLElement):
+        el.parentElement = self
         self.data.append(el)
-        print(self)
 
     def insertChild(self, el: HTMLElement | str, index: int = None):
         if not isinstance(el, str):
             el.parentElement = self
 
         if index is None:
             self.data.append(el)
         else:
             self.data.insert(index, el)
-        print(self)
 
     def removeChild(self, child: HTMLElement):
         self.data.remove(child)
 
     def safeRemoveChild(self, child: HTMLElement):
         if child in self.data:
             self.data.remove(child)
 
+    def replaceChild(self, newChild: HTMLElement, oldChild: HTMLElement):
+        self.data[self.data.index(oldChild)] = newChild
+
+    def remove(self):
+        self.parentElement.removeChild(self)
+
     def addEventListener(self, name, js_proxy):
         self.listeners[name].append(js_proxy)
 
-    def attachShadow(self, **kwargs):
-        self.shadowRoot = HTMLElement('-')
-        return self.shadowRoot
-
     @property
     def innerHTML(self):
-        return repr(self)
+        return ''.join(map(str, self.data))
 
     @innerHTML.setter
     def innerHTML(self, value):
         self.data = [value]
-        print(self)
+
+    @property
+    def outerHTML(self) -> str:
+        return repr(self)
 
     def __repr__(self):
         attrs = ' '
         for key, value in self.attributes.items():
             attrs += f'{key}="{value}" '
         attrs = attrs.strip(' ')
         if attrs:
             attrs = ' ' + attrs
         if not self.data:
             return f'<{self.tagName}{attrs}/>'
         return f"<{self.tagName}{attrs}>{''.join(map(str, self.data))}</{self.tagName}>"
 
 
+class Fragment(HTMLElement):
+    def __init__(self, *args, **kwargs):
+        super().__init__(None, *args, **kwargs)
+
+    def __repr__(self):
+        return self.innerHTML
+
+
 class Element(HTMLElement):
     pass
 
 
 class Console:
     def log(self, *a):
         _ = (self,)
@@ -104,23 +114,31 @@
 
 class Document:
     el_cls = Element
 
     head = el_cls('head')
     body = el_cls('body')
 
+    documentElement = el_cls('html')
+    documentElement.appendChild(head)
+    documentElement.appendChild(body)
+
     title = 'BeePy'
 
     def createElement(self, tag_name):
         return self.el_cls(tag_name)
 
-    querySelector = createElement
+    # Actually, this just creates strange elements, like <#root>, but it's not very cool HTML emulator :)
+    def querySelector(self, query):
+        el = self.el_cls(query)
+        self.body.appendChild(el)
+        return el
 
     def createDocumentFragment(self):
-        return self.createElement('-')
+        return Fragment()
 
 
 class Location:
     pathname = '/e/'  # must be dynamic
     href = f'http://localhost:9000/{pathname}'
     search = ''
     hash = ''
@@ -209,14 +227,15 @@
 
 def _DEBUGGER(error=None):
     print(error)
 
 
 max_id = {'interval': 1, 'timeout': 1}
 threads = {'interval': {}, 'timeout': {}}
+threads_to_join = []
 listeners = defaultdict(lambda: defaultdict(list))
 intervals = {}
 
 
 def _js_func(fn):
     fn.name = fn.__qualname__
     return fn
@@ -232,47 +251,53 @@
     listeners[element][name].remove(proxy)
 
 
 @_js_func
 def setInterval(callback, ms):
     def interval():
         while True:
+            if t in threads_to_join:
+                break
             time.sleep(ms / 1000)
             callback()
 
     id = max_id['interval']
     max_id['interval'] += 1
 
     threads['interval'][id] = t = Thread(target=interval, daemon=True)
     t.start()
 
+    return id
+
 
 @_js_func
 def clearInterval(interval_id):
     if interval_id in threads['interval']:
-        threads['interval'][interval_id].join()
+        threads_to_join.append(threads['interval'].pop(interval_id))
 
 
 @_js_func
 def setTimeout(callback, ms):
     def timeout():
         time.sleep(ms / 1000)
         callback()
 
     id = max_id['timeout']
     max_id['timeout'] += 1
 
     threads['timeout'][id] = t = Thread(target=timeout, daemon=True)
     t.start()
 
+    return id
+
 
 @_js_func
 def clearTimeout(timeout_id):
     if timeout_id in threads['timeout']:
-        threads['timeout'][timeout_id].join()
+        threads_to_join.append(threads['timeout'].pop(timeout_id))
 
 
 if TYPE_CHECKING:
     from beepy.framework import Tag
 
 
 class BeePyModule:
```

### Comparing `beepy_web-0.9.9/beepy/utils/js_py.py` & `beepy_web-10.0.0/beepy/utils/js_py.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.9/scripts/publish.sh` & `beepy_web-10.0.0/scripts/publish.sh`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 #!/bin/bash
 
 ### Prepare part ###
-# Replace dot with escaped dot :)
-old_version=${1//\./\\.}
-new_version=${2//\./\\.}
+old_version=${1//\./\\.}  # Replace dot with escaped dot
+new_version=$2
 
 declare -a files=(
     "web/src/beepy.js" "web/package.json"
     "beepy/framework.py"
     "beepy/dev/example.html" "docs/live-examples.md"
 )
 
 # Update version in main files
 for file in "${files[@]}"; do
     sed -i "s/$old_version/$new_version/g" $file
 done
 
-
 ### JS part ###
 cd web
 # Update version in package-lock.json
 npm i
 # Create dist/beepy.js
 npm run build
 # Temporary copy README.md  +  Actual publishing
@@ -28,8 +26,8 @@
 cd ..
 
 
 ### Python part ###
 # Create dist/* files
 hatch build
 # Actual publishing
-twine upload "dist/*$2[-.]*"
+twine upload "dist/*$new_version[-.]*"
```

### Comparing `beepy_web-0.9.9/web/package-lock.json` & `beepy_web-10.0.0/web/package-lock.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.899982970027248%*

 * *Differences: {"'packages'": "{'': {'version': '10.0.0'}}", "'version'": "'10.0.0'"}*

```diff
@@ -12,15 +12,15 @@
                 "webpack": "^5.89.0",
                 "webpack-cli": "^5.1.4",
                 "webpack-dev-server": "^4.15.1",
                 "webpack-merge": "^5.10.0"
             },
             "license": "MIT",
             "name": "@kor0p/beepy",
-            "version": "0.9.9"
+            "version": "10.0.0"
         },
         "node_modules/@discoveryjs/json-ext": {
             "dev": true,
             "engines": {
                 "node": ">=10.0.0"
             },
             "integrity": "sha512-dBVuXR082gk3jsFp7Rd/JI4kytwGHecnCoTtXFb7DB6CNHp4rg5k1bhg0nWdLGLnOV71lmDzGQaLMy8iPLY0pw==",
@@ -4174,9 +4174,9 @@
             "dev": true,
             "integrity": "sha512-3wdGidZyq5PB084XLES5TpOSRA3wjXAlIWMhum2kRcv/41Sn2emQ0dycQW4uZXLejwKvg6EsvbdlVL+FYEct7A==",
             "resolved": "https://registry.npmjs.org/yallist/-/yallist-4.0.0.tgz",
             "version": "4.0.0"
         }
     },
     "requires": true,
-    "version": "0.9.9"
+    "version": "10.0.0"
 }
```

### Comparing `beepy_web-0.9.9/web/package.json` & `beepy_web-10.0.0/web/package.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.95%*

 * *Differences: {"'version'": "'10.0.0'"}*

```diff
@@ -31,9 +31,9 @@
     "name": "@kor0p/beepy",
     "scripts": {
         "build": "webpack --config webpack.prod.js",
         "start": "webpack serve --config webpack.dev.js",
         "test": "echo \"Error: no test specified\" && exit 1",
         "watch": "webpack --watch"
     },
-    "version": "0.9.9"
+    "version": "10.0.0"
 }
```

### Comparing `beepy_web-0.9.9/web/webpack.prod.js` & `beepy_web-10.0.0/web/webpack.prod.js`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.9/web/src/beepy.js` & `beepy_web-10.0.0/web/src/beepy.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,13 @@
 import {
     _debugger,
     _lstrip,
     addHTMLElement,
+    get_meta,
+    isObjectEmpty,
     mergeDeep
 } from './utils'
 import {
     AsyncFiles,
     Files,
     rootFolder,
     SyncFiles,
@@ -21,42 +23,58 @@
 const _script = document.currentScript
 let localConfig = {}
 if (!!window.beepy) {
     localConfig = window.beepy
 }
 
 class BeePy {
-    __version__ = '0.9.9'
+    __version__ = '10.0.0'
 
     pyodideIndexURL = null
     globals = null
     dev_server = dev_server
     dev_path = ''
     python_api = python
 
     static _default_config = {
         include: ['.env'],
         pyodideVersion: '0.25.1',
+        random_seed: get_meta('beepy::config:random_seed') || 0,
+        server_side: get_meta('beepy::config:server_side') || '',
         requirements: [], // also could be function
     }
 
     // aliases for PythonAPI
     addElement = addHTMLElement
     files = Files
 
     constructor(localConfig) {
-        if (!localConfig) {
+        if (isObjectEmpty(localConfig)) {
             console.log(`
 No beepy config found! Default config will be used
 If you have config, you must define it before loading beepy script
             `)
         }
 
         this.config = mergeDeep(BeePy._default_config, localConfig.config || {})
-        this._loadPyodideScript()
+
+        if (!window.navigator.webdriver) {
+            this._updateConfig()
+        }
+
+        // Here never will be 'server' (this is set a little later). But it's fine
+        if (this.config.server_side !== 'client') {
+            this._loadPyodideScript()
+        }
+    }
+
+    _updateConfig() {
+        if (this.config.server_side === 'server') {
+            this.config._ssr_all_routes = []
+        }
 
         const path = _script.src.substring(0, _script.src.indexOf('beepy.js') - 1).replace(/\/+$/, '')
         this.dev_path = path.split('/').slice(0, -2).join('/')
     }
 
     startLoading({
         mountPoint = document.body,
@@ -227,15 +245,21 @@
                 await AsyncFiles._writeFile('.env', await AsyncFiles.loadFile(`${this.dev_path}/.env`))
             } catch (e) {}
         }
     }
 
     async _load() {
         window.removeEventListener('load', this._load)
-        this.startLoading()
+        if (window.navigator.webdriver) {
+            this._updateConfig()
+        }
+
+        if (this.config.server_side !== 'client') {
+            this.startLoading()
+        }
 
         window.pyodide = await window.loadPyodide({
             indexURL: this.pyodideIndexURL
         })
 
         pyodide.FS.mkdir(rootFolder)
 
@@ -263,8 +287,11 @@
         await this._main()
         this.dev_server.init()
     }
 }
 
 export const beepy = new BeePy(window.beepy || {})
 
-window.addEventListener('load', () => beepy._load())
+window.addEventListener(
+    window.navigator.webdriver ? 'beepy::server_side:load' : 'load',
+    () => beepy._load(),
+)
```

### Comparing `beepy_web-0.9.9/web/src/dev-server.js` & `beepy_web-10.0.0/web/src/dev-server.js`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.9/web/src/files.js` & `beepy_web-10.0.0/web/src/files.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -4,14 +4,15 @@
 
 export const rootFolder = '__beepy_root__'
 
 
 export class Files {
     static _enteringModule = ''
     static _lastLoadedFile = ''
+    static _devExtraQuery = ''
 
     static mkDirPath(path, removeFileName = false) {
         const pathParts = path.split('/')
         let maxLength = pathParts.length
         if (removeFileName) maxLength -= 1
 
         for (let length = 1; length <= maxLength; length++) {
@@ -59,14 +60,15 @@
 
 
 export class SyncFiles {
     static loadFile(filePath) {
         filePath = _lstrip(filePath)
         Files._lastLoadedFile = filePath
         if (!filePath.includes('http')) filePath = `${window.location.origin}/${filePath}`
+        filePath = `${filePath}${Files._devExtraQuery ? (filePath.includes('?') ? '&':'?') : ''}${Files._devExtraQuery}`
 
         const req = new XMLHttpRequest()
         req.open('GET', filePath, false)
         req.send(null)
         if (req.status >= 400 && req.status < 500) {
             throw new Error('File not found')
         }
@@ -80,14 +82,15 @@
 }
 
 
 export class AsyncFiles {
     static async loadFile(filePath) {
         Files._lastLoadedFile = filePath
         if (!filePath.includes('http')) filePath = `${window.location.origin}/${filePath}`
+        filePath = `${filePath}${Files._devExtraQuery ? (filePath.includes('?') ? '&':'?') : ''}${Files._devExtraQuery}`
 
         const r = await fetch(filePath, {
             method: 'GET'
         })
         if (r.status >= 400 && r.status < 500) {
             throw new Error('File not found')
         }
```

### Comparing `beepy_web-0.9.9/web/src/main.css` & `beepy_web-10.0.0/web/src/main.css`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.9/web/src/python.js` & `beepy_web-10.0.0/web/src/python.js`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.9/web/src/utils.js` & `beepy_web-10.0.0/web/src/utils.js`

 * *Files 7% similar despite different names*

#### js-beautify {}

```diff
@@ -41,14 +41,18 @@
     for (const [optionName, optionValue] of Object.entries(options)) {
         element[optionName] = optionValue
     }
     mountPoint.insertChild(element, index)
     return element
 }
 
+export function isObjectEmpty(obj) {
+    return Object.keys(obj).length === 0;
+}
+
 export function isObject(obj) {
     return obj && typeof obj === 'object'
 }
 
 export function mergeDeep(...objects) {
     return objects.reduce((acc, obj) => {
         Object.entries(obj).forEach(([key, objValue]) => {
@@ -72,14 +76,19 @@
 }
 
 
 export function _lstrip(text) {
     return text.replace(/^\/+/, '')
 }
 
+export function get_meta(name) {
+    const el = document.querySelector(`meta[name="${name}"]`)
+    return el ? el.content : ''
+}
+
 export const _py_tag_attribute = '__PYTHON_TAG__'
 
 function getPyTag(i) {
     /**
      * usage:
      * > py0
      * evaluates $0.__PYTHON_TAG__
```

### Comparing `beepy_web-0.9.9/.gitignore` & `beepy_web-10.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.9/LICENSE` & `beepy_web-10.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.9/README.md` & `beepy_web-10.0.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 ## Join our community at [Telegram chat](https://t.me/bee_py/)
 ## [Documentation](https://kor0p.github.io/BeePy-examples/sandbox) | [PyPI](https://pypi.org/project/beepy-web/) | [NPM](https://www.npmjs.com/package/@kor0p/beepy)
 
 ## Local development:
 ### Install BeePy
 ### `pip install -U beepy-web[dev]`
 ### Then just start local server
-### `python -m beepy.dev --create`
+### `python -m beepy.dev server --create`
 ### And that's it!
 
 ### Now, click on link in console to visit your server
 ### and change code to see updates in browser in no time!
 
 Code (custom_url.py from examples):
 ```python
```

### Comparing `beepy_web-0.9.9/pyproject.toml` & `beepy_web-10.0.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -20,20 +20,24 @@
 "Docs" = "https://bee-py.readthedocs.io/en/latest/"
 "Community" = "https://t.me/bee_py/"
 "Sandbox" = "https://kor0p.github.io/BeePy-examples/sandbox"
 "NPM" = "https://www.npmjs.com/package/@kor0p/beepy"
 
 [project.optional-dependencies]
 dev = [
+    "click==8.1.3",  # Easy cli commands
     "pyodide-py==0.25.1", # Pyodide package
     "micropip==0.3.0", # A lightweight Python package installer for the web
     "watchdog==3.0.0", # watcher for files that changes for Hot reload
     "websockets==11.0.3", # Hot reload is working using simple WebSockets server
     "requests==2.31.0", # HTTP synchronous requests lib
 ]
+ssr = [
+    "selenium==4.19.0", # Rendering HTML on server side to start faster
+]
 docs = [
     "mkdocs-material==9.5.17",
 ]
 contributing = [
     "pre-commit", # for pre-commit git hooks
 ]
 
@@ -112,13 +116,13 @@
 
 [tool.ruff.lint.pycodestyle]
 ignore-overlong-task-comments = true
 
 [tool.ruff.lint.pydocstyle]
 convention = "google"
 
-[tool.ruff.pylint]
+[tool.ruff.lint.pylint]
 max-args = 7
 
 [tool.ruff.lint.mccabe]
 # Flag errors (`C901`) whenever the complexity level exceeds 11.
 max-complexity = 11
```

### Comparing `beepy_web-0.9.9/PKG-INFO` & `beepy_web-10.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beepy-web
-Version: 0.9.9
+Version: 10.0.0
 Summary: The modern frontend web framework for Python
 Project-URL: Homepage, https://beepy-web-ba63e5a12994.herokuapp.com/e/
 Project-URL: Repository, https://github.com/kor0p/BeePy
 Project-URL: Docs, https://bee-py.readthedocs.io/en/latest/
 Project-URL: Community, https://t.me/bee_py/
 Project-URL: Sandbox, https://kor0p.github.io/BeePy-examples/sandbox
 Project-URL: NPM, https://www.npmjs.com/package/@kor0p/beepy
@@ -14,21 +14,24 @@
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10.10
 Requires-Dist: boltons==23.1.1
 Requires-Dist: python-dotenv==1.0.0
 Provides-Extra: contributing
 Requires-Dist: pre-commit; extra == 'contributing'
 Provides-Extra: dev
+Requires-Dist: click==8.1.3; extra == 'dev'
 Requires-Dist: micropip==0.3.0; extra == 'dev'
 Requires-Dist: pyodide-py==0.25.1; extra == 'dev'
 Requires-Dist: requests==2.31.0; extra == 'dev'
 Requires-Dist: watchdog==3.0.0; extra == 'dev'
 Requires-Dist: websockets==11.0.3; extra == 'dev'
 Provides-Extra: docs
 Requires-Dist: mkdocs-material==9.5.17; extra == 'docs'
+Provides-Extra: ssr
+Requires-Dist: selenium==4.19.0; extra == 'ssr'
 Description-Content-Type: text/markdown
 
 # 🐝 BeePy
 
 [![NPM Package](https://img.shields.io/npm/v/@kor0p/beepy)](https://www.npmjs.com/package/@kor0p/beepy)
 [![PyPI Package](https://img.shields.io/pypi/v/beepy-web.svg)](https://pypi.org/project/beepy-web/)
 [![Documentation](https://cdn.jsdelivr.net/gh/Andre601/devins-badges@v3.x-mkdocs-material/assets/compact-minimal/built-with/mkdocs-material_vector.svg)](https://bee-py.readthedocs.io/en/latest/)
@@ -42,15 +45,15 @@
 ## Join our community at [Telegram chat](https://t.me/bee_py/)
 ## [Documentation](https://kor0p.github.io/BeePy-examples/sandbox) | [PyPI](https://pypi.org/project/beepy-web/) | [NPM](https://www.npmjs.com/package/@kor0p/beepy)
 
 ## Local development:
 ### Install BeePy
 ### `pip install -U beepy-web[dev]`
 ### Then just start local server
-### `python -m beepy.dev --create`
+### `python -m beepy.dev server --create`
 ### And that's it!
 
 ### Now, click on link in console to visit your server
 ### and change code to see updates in browser in no time!
 
 Code (custom_url.py from examples):
 ```python
```

