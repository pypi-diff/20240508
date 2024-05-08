# Comparing `tmp/apluggy-0.9.9.tar.gz` & `tmp/apluggy-1.0.0.tar.gz`

## Comparing `apluggy-0.9.9.tar` & `apluggy-1.0.0.tar`

### file list

```diff
@@ -1,59 +1,60 @@
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 apluggy-0.9.9/setup.cfg
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 apluggy-0.9.9/.github/release.yml
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 apluggy-0.9.9/.github/workflows/pypi.yml
--rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 apluggy-0.9.9/.github/workflows/release.yml
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 apluggy-0.9.9/.github/workflows/type-check.yml
--rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 apluggy-0.9.9/.github/workflows/unit-test.yml
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 apluggy-0.9.9/.vscode/settings.json
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 apluggy-0.9.9/src/apluggy/__about__.py
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 apluggy-0.9.9/src/apluggy/__init__.py
--rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 apluggy-0.9.9/src/apluggy/_decorator.py
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 apluggy-0.9.9/src/apluggy/stack/__init__.py
--rw-r--r--   0        0        0     5850 2020-02-02 00:00:00.000000 apluggy-0.9.9/src/apluggy/stack/aexit.py
--rw-r--r--   0        0        0     3061 2020-02-02 00:00:00.000000 apluggy-0.9.9/src/apluggy/stack/async_.py
--rw-r--r--   0        0        0     4692 2020-02-02 00:00:00.000000 apluggy-0.9.9/src/apluggy/stack/sync.py
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 apluggy-0.9.9/src/apluggy/stack/types.py
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 apluggy-0.9.9/src/apluggy/test/__init__.py
--rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 apluggy-0.9.9/src/apluggy/test/probe.py
--rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 apluggy-0.9.9/src/apluggy/test/st.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 apluggy-0.9.9/src/apluggy/wrap/__init__.py
--rw-r--r--   0        0        0     1869 2020-02-02 00:00:00.000000 apluggy-0.9.9/src/apluggy/wrap/ext.py
--rw-r--r--   0        0        0     4394 2020-02-02 00:00:00.000000 apluggy-0.9.9/src/apluggy/wrap/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apluggy-0.9.9/tests/__init__.py
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 apluggy-0.9.9/tests/test_decorator.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apluggy-0.9.9/tests/plugins/__init__.py
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 apluggy-0.9.9/tests/plugins/module_plugin.py
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 apluggy-0.9.9/tests/plugins/spec.py
--rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 apluggy-0.9.9/tests/plugins/test_call.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apluggy-0.9.9/tests/stack/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apluggy-0.9.9/tests/stack/aexit/__init__.py
--rw-r--r--   0        0        0     3273 2020-02-02 00:00:00.000000 apluggy-0.9.9/tests/stack/aexit/test_aexit.py
--rw-r--r--   0        0        0     3787 2020-02-02 00:00:00.000000 apluggy-0.9.9/tests/stack/aexit/test_demo.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apluggy-0.9.9/tests/stack/async/__init__.py
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 apluggy-0.9.9/tests/stack/async/exc.py
--rw-r--r--   0        0        0     5408 2020-02-02 00:00:00.000000 apluggy-0.9.9/tests/stack/async/runner.py
--rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 apluggy-0.9.9/tests/stack/async/test_imp.py
--rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 apluggy-0.9.9/tests/stack/async/test_refs.py
--rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 apluggy-0.9.9/tests/stack/async/test_runner.py
--rw-r--r--   0        0        0     2246 2020-02-02 00:00:00.000000 apluggy-0.9.9/tests/stack/async/test_single.py
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 apluggy-0.9.9/tests/stack/async/refs/__init__.py
--rw-r--r--   0        0        0     6798 2020-02-02 00:00:00.000000 apluggy-0.9.9/tests/stack/async/refs/dunder.py
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 apluggy-0.9.9/tests/stack/async/refs/exit_.py
--rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 apluggy-0.9.9/tests/stack/async/refs/nested.py
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 apluggy-0.9.9/tests/stack/async/refs/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apluggy-0.9.9/tests/stack/sync/__init__.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 apluggy-0.9.9/tests/stack/sync/exc.py
--rw-r--r--   0        0        0     4984 2020-02-02 00:00:00.000000 apluggy-0.9.9/tests/stack/sync/runner.py
--rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 apluggy-0.9.9/tests/stack/sync/test_imp.py
--rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 apluggy-0.9.9/tests/stack/sync/test_refs.py
--rw-r--r--   0        0        0     2008 2020-02-02 00:00:00.000000 apluggy-0.9.9/tests/stack/sync/test_single.py
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 apluggy-0.9.9/tests/stack/sync/refs/__init__.py
--rw-r--r--   0        0        0     4829 2020-02-02 00:00:00.000000 apluggy-0.9.9/tests/stack/sync/refs/dunder.py
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 apluggy-0.9.9/tests/stack/sync/refs/exit_.py
--rw-r--r--   0        0        0     2666 2020-02-02 00:00:00.000000 apluggy-0.9.9/tests/stack/sync/refs/nested.py
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 apluggy-0.9.9/tests/stack/sync/refs/types.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 apluggy-0.9.9/.gitignore
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 apluggy-0.9.9/LICENSE.txt
--rw-r--r--   0        0        0     8328 2020-02-02 00:00:00.000000 apluggy-0.9.9/README.md
--rw-r--r--   0        0        0     2106 2020-02-02 00:00:00.000000 apluggy-0.9.9/pyproject.toml
--rw-r--r--   0        0        0     9395 2020-02-02 00:00:00.000000 apluggy-0.9.9/PKG-INFO
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 apluggy-1.0.0/setup.cfg
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 apluggy-1.0.0/.github/release.yml
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 apluggy-1.0.0/.github/workflows/pypi.yml
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 apluggy-1.0.0/.github/workflows/release.yml
+-rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 apluggy-1.0.0/.github/workflows/type-check.yml
+-rw-r--r--   0        0        0     1206 2020-02-02 00:00:00.000000 apluggy-1.0.0/.github/workflows/unit-test.yml
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 apluggy-1.0.0/.vscode/settings.json
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 apluggy-1.0.0/src/apluggy/__about__.py
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 apluggy-1.0.0/src/apluggy/__init__.py
+-rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 apluggy-1.0.0/src/apluggy/_decorator.py
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 apluggy-1.0.0/src/apluggy/stack/__init__.py
+-rw-r--r--   0        0        0     5850 2020-02-02 00:00:00.000000 apluggy-1.0.0/src/apluggy/stack/aexit.py
+-rw-r--r--   0        0        0     3061 2020-02-02 00:00:00.000000 apluggy-1.0.0/src/apluggy/stack/async_.py
+-rw-r--r--   0        0        0     4692 2020-02-02 00:00:00.000000 apluggy-1.0.0/src/apluggy/stack/sync.py
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 apluggy-1.0.0/src/apluggy/stack/types.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 apluggy-1.0.0/src/apluggy/wrap/__init__.py
+-rw-r--r--   0        0        0     1869 2020-02-02 00:00:00.000000 apluggy-1.0.0/src/apluggy/wrap/ext.py
+-rw-r--r--   0        0        0     4394 2020-02-02 00:00:00.000000 apluggy-1.0.0/src/apluggy/wrap/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apluggy-1.0.0/tests/__init__.py
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 apluggy-1.0.0/tests/test_decorator.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apluggy-1.0.0/tests/plugins/__init__.py
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 apluggy-1.0.0/tests/plugins/module_plugin.py
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 apluggy-1.0.0/tests/plugins/spec.py
+-rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 apluggy-1.0.0/tests/plugins/test_call.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apluggy-1.0.0/tests/stack/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apluggy-1.0.0/tests/stack/aexit/__init__.py
+-rw-r--r--   0        0        0     3272 2020-02-02 00:00:00.000000 apluggy-1.0.0/tests/stack/aexit/test_aexit.py
+-rw-r--r--   0        0        0     3787 2020-02-02 00:00:00.000000 apluggy-1.0.0/tests/stack/aexit/test_demo.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apluggy-1.0.0/tests/stack/async/__init__.py
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 apluggy-1.0.0/tests/stack/async/exc.py
+-rw-r--r--   0        0        0     5407 2020-02-02 00:00:00.000000 apluggy-1.0.0/tests/stack/async/runner.py
+-rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 apluggy-1.0.0/tests/stack/async/test_imp.py
+-rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 apluggy-1.0.0/tests/stack/async/test_refs.py
+-rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 apluggy-1.0.0/tests/stack/async/test_runner.py
+-rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 apluggy-1.0.0/tests/stack/async/test_single.py
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 apluggy-1.0.0/tests/stack/async/refs/__init__.py
+-rw-r--r--   0        0        0     6798 2020-02-02 00:00:00.000000 apluggy-1.0.0/tests/stack/async/refs/dunder.py
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 apluggy-1.0.0/tests/stack/async/refs/exit_.py
+-rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 apluggy-1.0.0/tests/stack/async/refs/nested.py
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 apluggy-1.0.0/tests/stack/async/refs/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apluggy-1.0.0/tests/stack/sync/__init__.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 apluggy-1.0.0/tests/stack/sync/exc.py
+-rw-r--r--   0        0        0     4983 2020-02-02 00:00:00.000000 apluggy-1.0.0/tests/stack/sync/runner.py
+-rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 apluggy-1.0.0/tests/stack/sync/test_imp.py
+-rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 apluggy-1.0.0/tests/stack/sync/test_refs.py
+-rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 apluggy-1.0.0/tests/stack/sync/test_single.py
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 apluggy-1.0.0/tests/stack/sync/refs/__init__.py
+-rw-r--r--   0        0        0     4829 2020-02-02 00:00:00.000000 apluggy-1.0.0/tests/stack/sync/refs/dunder.py
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 apluggy-1.0.0/tests/stack/sync/refs/exit_.py
+-rw-r--r--   0        0        0     2666 2020-02-02 00:00:00.000000 apluggy-1.0.0/tests/stack/sync/refs/nested.py
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 apluggy-1.0.0/tests/stack/sync/refs/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apluggy-1.0.0/tests/test/__init__.py
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 apluggy-1.0.0/tests/utils/__init__.py
+-rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 apluggy-1.0.0/tests/utils/probe.py
+-rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 apluggy-1.0.0/tests/utils/st.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 apluggy-1.0.0/.gitignore
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 apluggy-1.0.0/LICENSE.txt
+-rw-r--r--   0        0        0     8366 2020-02-02 00:00:00.000000 apluggy-1.0.0/README.md
+-rw-r--r--   0        0        0     2200 2020-02-02 00:00:00.000000 apluggy-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     9559 2020-02-02 00:00:00.000000 apluggy-1.0.0/PKG-INFO
```

### Comparing `apluggy-0.9.9/.github/workflows/pypi.yml` & `apluggy-1.0.0/.github/workflows/pypi.yml`

 * *Files 16% similar despite different names*

```diff
@@ -5,15 +5,17 @@
   #   types: [created]
   push:
     tags:
       - 'v*.*.*'
 jobs:
   deploy:
     runs-on: ubuntu-latest
-
+    environment: pypi
+    permissions:
+      id-token: write
     steps:
       - uses: actions/checkout@v3
         with:
           fetch-depth: 0
 
       - name: Set up Python
         uses: actions/setup-python@v4
@@ -21,14 +23,12 @@
           python-version: '3.10'
 
       - name: Install packages
         run: |
           pip install --upgrade pip
           pip install --upgrade hatch
 
-      - name:  Build
+      - name: Build
         run: hatch build
 
       - name: pypi-publish
-        uses: pypa/gh-action-pypi-publish@v1.6.4
-        with:
-          password: ${{ secrets.PYPI_API_TOKEN }}
+        uses: pypa/gh-action-pypi-publish@release/v1
```

### Comparing `apluggy-0.9.9/.github/workflows/release.yml` & `apluggy-1.0.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `apluggy-0.9.9/.github/workflows/type-check.yml` & `apluggy-1.0.0/.github/workflows/type-check.yml`

 * *Files identical despite different names*

### Comparing `apluggy-0.9.9/src/apluggy/_decorator.py` & `apluggy-1.0.0/src/apluggy/_decorator.py`

 * *Files identical despite different names*

### Comparing `apluggy-0.9.9/src/apluggy/stack/aexit.py` & `apluggy-1.0.0/src/apluggy/stack/aexit.py`

 * *Files identical despite different names*

### Comparing `apluggy-0.9.9/src/apluggy/stack/async_.py` & `apluggy-1.0.0/src/apluggy/stack/async_.py`

 * *Files identical despite different names*

### Comparing `apluggy-0.9.9/src/apluggy/stack/sync.py` & `apluggy-1.0.0/src/apluggy/stack/sync.py`

 * *Files identical despite different names*

### Comparing `apluggy-0.9.9/src/apluggy/test/probe.py` & `apluggy-1.0.0/tests/utils/probe.py`

 * *Files identical despite different names*

### Comparing `apluggy-0.9.9/src/apluggy/test/st.py` & `apluggy-1.0.0/tests/utils/st.py`

 * *Files identical despite different names*

### Comparing `apluggy-0.9.9/src/apluggy/wrap/ext.py` & `apluggy-1.0.0/src/apluggy/wrap/ext.py`

 * *Files identical despite different names*

### Comparing `apluggy-0.9.9/src/apluggy/wrap/main.py` & `apluggy-1.0.0/src/apluggy/wrap/main.py`

 * *Files identical despite different names*

### Comparing `apluggy-0.9.9/tests/test_decorator.py` & `apluggy-1.0.0/tests/test_decorator.py`

 * *Files identical despite different names*

### Comparing `apluggy-0.9.9/tests/plugins/test_call.py` & `apluggy-1.0.0/tests/plugins/test_call.py`

 * *Files identical despite different names*

### Comparing `apluggy-0.9.9/tests/stack/aexit/test_aexit.py` & `apluggy-1.0.0/tests/stack/aexit/test_aexit.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import sys
 from collections.abc import AsyncGenerator, Generator
 
 from hypothesis import given
 from hypothesis import strategies as st
 
 from apluggy.stack import patch_aexit
-from apluggy.test import RecordReturns, ReplayReturns, st_none_or
+from tests.utils import RecordReturns, ReplayReturns, st_none_or
 
 
 @given(st.data())
 async def test_patch_aexit(data: st.DataObject) -> None:
     '''`patch_aexit()` makes an async context manager propagate the exception
     in the same way as a context manager does.
```

### Comparing `apluggy-0.9.9/tests/stack/aexit/test_demo.py` & `apluggy-1.0.0/tests/stack/aexit/test_demo.py`

 * *Files identical despite different names*

### Comparing `apluggy-0.9.9/tests/stack/async/runner.py` & `apluggy-1.0.0/tests/stack/async/runner.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import contextlib
 from collections.abc import AsyncGenerator, MutableSequence
 from typing import Any, TypeVar
 
 from hypothesis import strategies as st
 
 from apluggy.stack import AGenCtxMngr
-from apluggy.test import Probe, st_none_or
+from tests.utils import Probe, st_none_or
 
 from .exc import GenRaised, Thrown, WithRaised
 from .refs import AStack
 
 T = TypeVar('T')
```

### Comparing `apluggy-0.9.9/tests/stack/async/test_imp.py` & `apluggy-1.0.0/tests/stack/async/test_imp.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from functools import partial
 
 from hypothesis import given, settings
 from hypothesis import strategies as st
 
 from apluggy import async_stack_gen_ctxs
-from apluggy.test import RecordReturns, ReplayReturns
+from tests.utils import RecordReturns, ReplayReturns
 
 from .refs import dunder_enter
 from .runner import run
 
 
 @given(st.data())
 @settings(max_examples=200, deadline=1000)
```

### Comparing `apluggy-0.9.9/tests/stack/async/test_refs.py` & `apluggy-1.0.0/tests/stack/async/test_refs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from functools import partial
 
 from hypothesis import given, settings
 from hypothesis import strategies as st
 
-from apluggy.test import RecordReturns, ReplayReturns
+from tests.utils import RecordReturns, ReplayReturns
 
 from .refs import dunder_enter, exit_stack, nested_with
 from .runner import run
 
 
 @given(st.data())
 @settings(max_examples=200, deadline=1000)
```

### Comparing `apluggy-0.9.9/tests/stack/async/test_runner.py` & `apluggy-1.0.0/tests/stack/async/test_runner.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Any
 
 from hypothesis import given, settings
 from hypothesis import strategies as st
 
-from apluggy.test import Probe, RecordReturns
+from tests.utils import Probe, RecordReturns
 
 from .exc import GenRaised, Thrown, WithRaised
 from .runner import mock_async_context, run_async_generator_context
 
 
 async def run_mock_async_context(
     draw: st.DrawFn, n_sends: int
```

### Comparing `apluggy-0.9.9/tests/stack/async/test_single.py` & `apluggy-1.0.0/tests/stack/async/test_single.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from collections.abc import MutableSequence
 from typing import Any, TypeVar
 
 from hypothesis import given, settings
 from hypothesis import strategies as st
 
 from apluggy.stack import AGenCtxMngr
-from apluggy.test import Probe, RecordReturns, ReplayReturns
+from tests.utils import Probe, RecordReturns, ReplayReturns
 
 from .exc import GenRaised, Thrown, WithRaised
 from .refs.dunder import dunder_enter_single
 from .runner import mock_async_context, run_async_generator_context
 
 T = TypeVar('T')
```

### Comparing `apluggy-0.9.9/tests/stack/async/refs/dunder.py` & `apluggy-1.0.0/tests/stack/async/refs/dunder.py`

 * *Files identical despite different names*

### Comparing `apluggy-0.9.9/tests/stack/async/refs/exit_.py` & `apluggy-1.0.0/tests/stack/async/refs/exit_.py`

 * *Files identical despite different names*

### Comparing `apluggy-0.9.9/tests/stack/async/refs/nested.py` & `apluggy-1.0.0/tests/stack/async/refs/nested.py`

 * *Files identical despite different names*

### Comparing `apluggy-0.9.9/tests/stack/sync/runner.py` & `apluggy-1.0.0/tests/stack/sync/runner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import contextlib
 from collections.abc import Generator, MutableSequence
 from typing import Any, TypeVar
 
 from hypothesis import strategies as st
 
 from apluggy.stack import GenCtxMngr
-from apluggy.test import Probe, st_none_or
+from tests.utils import Probe, st_none_or
 
 from .exc import Raised, Thrown
 from .refs import Stack
 
 T = TypeVar('T')
```

### Comparing `apluggy-0.9.9/tests/stack/sync/test_imp.py` & `apluggy-1.0.0/tests/stack/sync/test_imp.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from hypothesis import given, settings
 from hypothesis import strategies as st
 
 from apluggy import stack_gen_ctxs
-from apluggy.test import RecordReturns, ReplayReturns
+from tests.utils import RecordReturns, ReplayReturns
 
 from .refs import dunder_enter
 from .runner import run
 
 
 @given(st.data())
 @settings(max_examples=200, deadline=1000)
```

### Comparing `apluggy-0.9.9/tests/stack/sync/test_refs.py` & `apluggy-1.0.0/tests/stack/sync/test_refs.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from hypothesis import given, settings
 from hypothesis import strategies as st
 
-from apluggy.test import RecordReturns, ReplayReturns
+from tests.utils import RecordReturns, ReplayReturns
 
 from .refs import dunder_enter, exit_stack, nested_with
 from .runner import run
 
 
 @given(st.data())
 @settings(max_examples=200, deadline=1000)
```

### Comparing `apluggy-0.9.9/tests/stack/sync/test_single.py` & `apluggy-1.0.0/tests/stack/sync/test_single.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from collections.abc import MutableSequence
 from typing import Any, TypeVar
 
 from hypothesis import given, settings
 from hypothesis import strategies as st
 
 from apluggy.stack import GenCtxMngr
-from apluggy.test import Probe, RecordReturns, ReplayReturns
+from tests.utils import Probe, RecordReturns, ReplayReturns
 
 from .exc import Raised, Thrown
 from .refs.nested import nested_with_single
 from .runner import mock_context, run_generator_context
 
 T = TypeVar('T')
```

### Comparing `apluggy-0.9.9/tests/stack/sync/refs/dunder.py` & `apluggy-1.0.0/tests/stack/sync/refs/dunder.py`

 * *Files identical despite different names*

### Comparing `apluggy-0.9.9/tests/stack/sync/refs/nested.py` & `apluggy-1.0.0/tests/stack/sync/refs/nested.py`

 * *Files identical despite different names*

### Comparing `apluggy-0.9.9/.gitignore` & `apluggy-1.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `apluggy-0.9.9/LICENSE.txt` & `apluggy-1.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `apluggy-0.9.9/README.md` & `apluggy-1.0.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # apluggy
 
 [![PyPI - Version](https://img.shields.io/pypi/v/apluggy.svg)](https://pypi.org/project/apluggy)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/apluggy.svg)](https://pypi.org/project/apluggy)
+
 [![Test Status](https://github.com/simonsobs/apluggy/actions/workflows/unit-test.yml/badge.svg)](https://github.com/simonsobs/apluggy/actions/workflows/unit-test.yml)
 [![Test Status](https://github.com/simonsobs/apluggy/actions/workflows/type-check.yml/badge.svg)](https://github.com/simonsobs/apluggy/actions/workflows/type-check.yml)
 [![codecov](https://codecov.io/gh/simonsobs/apluggy/branch/main/graph/badge.svg)](https://codecov.io/gh/simonsobs/apluggy)
 
 A wrapper of [pluggy](https://pluggy.readthedocs.io/) to support asyncio and context managers.
 
 This package provides a subclass of
@@ -15,20 +16,28 @@
 - allows async functions, context managers, and async context managers to be hooks
 - and accepts plugin factories in addition to plugin instances for registration.
 
 ---
 
 **Table of Contents**
 
-- [apluggy](#apluggy)
-  - [Installation](#installation)
-  - [How to use](#how-to-use)
-  - [Links](#links)
-  - [License](#license)
-  - [Contact](#contact)
+- [Installation](#installation)
+- [How to use](#how-to-use)
+  - [Start Python](#start-python)
+  - [Import packages](#import-packages)
+  - [Create hook specification and implementation decorators](#create-hook-specification-and-implementation-decorators)
+  - [Define hook specifications](#define-hook-specifications)
+  - [Define plugins](#define-plugins)
+  - [Create a plugin manager and register plugins](#create-a-plugin-manager-and-register-plugins)
+  - [Call hooks](#call-hooks)
+    - [Async function](#async-function)
+    - [Context manager](#context-manager)
+    - [Async context manager](#async-context-manager)
+- [Links](#links)
+- [License](#license)
 
 ---
 
 ## Installation
 
 You can install apluggy with pip:
 
@@ -278,19 +287,7 @@
 - [decorator](https://pypi.org/project/decorator/)
 
 ---
 
 ## License
 
 - _apluggy_ is licensed under the [MIT](https://spdx.org/licenses/MIT.html) license.
-
----
-
-## Contact
-
-- [Tai Sakuma](https://github.com/TaiSakuma) <span itemscope
-  itemtype="https://schema.org/Person"><a itemprop="sameAs"
-  content="https://orcid.org/0000-0003-3225-9861"
-  href="https://orcid.org/0000-0003-3225-9861" target="orcid.widget" rel="me
-  noopener noreferrer" style="vertical-align:text-top;"><img
-  src="https://orcid.org/sites/default/files/images/orcid_16x16.png"
-  style="width:1em;margin-right:.5em;" alt="ORCID iD icon"></a></span>
```

### Comparing `apluggy-0.9.9/pyproject.toml` & `apluggy-1.0.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -7,34 +7,36 @@
 description = 'A wrapper of "pluggy" to support asyncio and context managers'
 readme = "README.md"
 requires-python = ">=3.10"
 license = "MIT"
 keywords = []
 authors = [{ name = "Tai Sakuma", email = "tai.sakuma@gmail.com" }]
 classifiers = [
-  "Development Status :: 4 - Beta",
+  "Development Status :: 5 - Production/Stable",
+  "Intended Audience :: Developers",
+  "License :: OSI Approved :: MIT License",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
 ]
 dependencies = [
   "pluggy>=1.0",
   "decorator>=5.1",
   "types-decorator>=5.1",
-  "hypothesis>=6.68",
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 tests = [
   "pytest-asyncio>=0.18",
   "pytest-cov>=3.0",
   "pytest-timeout>=2.1",
   "pytest>=7.0",
+  "hypothesis>=6.68",
 ]
 
 [project.urls]
 Documentation = "https://github.com/simonsobs/apluggy#readme"
 Issues = "https://github.com/simonsobs/apluggy/issues"
 Source = "https://github.com/simonsobs/apluggy"
```

### Comparing `apluggy-0.9.9/PKG-INFO` & `apluggy-1.0.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,38 +1,41 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: apluggy
-Version: 0.9.9
+Version: 1.0.0
 Summary: A wrapper of "pluggy" to support asyncio and context managers
 Project-URL: Documentation, https://github.com/simonsobs/apluggy#readme
 Project-URL: Issues, https://github.com/simonsobs/apluggy/issues
 Project-URL: Source, https://github.com/simonsobs/apluggy
 Author-email: Tai Sakuma <tai.sakuma@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.10
 Requires-Dist: decorator>=5.1
-Requires-Dist: hypothesis>=6.68
 Requires-Dist: pluggy>=1.0
 Requires-Dist: types-decorator>=5.1
 Provides-Extra: tests
+Requires-Dist: hypothesis>=6.68; extra == 'tests'
 Requires-Dist: pytest-asyncio>=0.18; extra == 'tests'
 Requires-Dist: pytest-cov>=3.0; extra == 'tests'
 Requires-Dist: pytest-timeout>=2.1; extra == 'tests'
 Requires-Dist: pytest>=7.0; extra == 'tests'
 Description-Content-Type: text/markdown
 
 # apluggy
 
 [![PyPI - Version](https://img.shields.io/pypi/v/apluggy.svg)](https://pypi.org/project/apluggy)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/apluggy.svg)](https://pypi.org/project/apluggy)
+
 [![Test Status](https://github.com/simonsobs/apluggy/actions/workflows/unit-test.yml/badge.svg)](https://github.com/simonsobs/apluggy/actions/workflows/unit-test.yml)
 [![Test Status](https://github.com/simonsobs/apluggy/actions/workflows/type-check.yml/badge.svg)](https://github.com/simonsobs/apluggy/actions/workflows/type-check.yml)
 [![codecov](https://codecov.io/gh/simonsobs/apluggy/branch/main/graph/badge.svg)](https://codecov.io/gh/simonsobs/apluggy)
 
 A wrapper of [pluggy](https://pluggy.readthedocs.io/) to support asyncio and context managers.
 
 This package provides a subclass of
@@ -42,20 +45,28 @@
 - allows async functions, context managers, and async context managers to be hooks
 - and accepts plugin factories in addition to plugin instances for registration.
 
 ---
 
 **Table of Contents**
 
-- [apluggy](#apluggy)
-  - [Installation](#installation)
-  - [How to use](#how-to-use)
-  - [Links](#links)
-  - [License](#license)
-  - [Contact](#contact)
+- [Installation](#installation)
+- [How to use](#how-to-use)
+  - [Start Python](#start-python)
+  - [Import packages](#import-packages)
+  - [Create hook specification and implementation decorators](#create-hook-specification-and-implementation-decorators)
+  - [Define hook specifications](#define-hook-specifications)
+  - [Define plugins](#define-plugins)
+  - [Create a plugin manager and register plugins](#create-a-plugin-manager-and-register-plugins)
+  - [Call hooks](#call-hooks)
+    - [Async function](#async-function)
+    - [Context manager](#context-manager)
+    - [Async context manager](#async-context-manager)
+- [Links](#links)
+- [License](#license)
 
 ---
 
 ## Installation
 
 You can install apluggy with pip:
 
@@ -305,19 +316,7 @@
 - [decorator](https://pypi.org/project/decorator/)
 
 ---
 
 ## License
 
 - _apluggy_ is licensed under the [MIT](https://spdx.org/licenses/MIT.html) license.
-
----
-
-## Contact
-
-- [Tai Sakuma](https://github.com/TaiSakuma) <span itemscope
-  itemtype="https://schema.org/Person"><a itemprop="sameAs"
-  content="https://orcid.org/0000-0003-3225-9861"
-  href="https://orcid.org/0000-0003-3225-9861" target="orcid.widget" rel="me
-  noopener noreferrer" style="vertical-align:text-top;"><img
-  src="https://orcid.org/sites/default/files/images/orcid_16x16.png"
-  style="width:1em;margin-right:.5em;" alt="ORCID iD icon"></a></span>
```

