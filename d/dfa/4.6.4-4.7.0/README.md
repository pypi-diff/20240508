# Comparing `tmp/dfa-4.6.4.tar.gz` & `tmp/dfa-4.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dfa-4.6.4.tar", max compression
+gzip compressed data, was "dfa-4.7.0.tar", max compression
```

## Comparing `dfa-4.6.4.tar` & `dfa-4.7.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1082 2024-03-10 00:27:29.678094 dfa-4.6.4/LICENSE
--rw-r--r--   0        0        0     7737 2024-03-10 00:27:29.678094 dfa-4.6.4/README.md
--rw-r--r--   0        0        0      230 2024-03-10 00:27:29.678094 dfa-4.6.4/dfa/__init__.py
--rw-r--r--   0        0        0    11108 2024-04-29 01:46:33.514822 dfa-4.6.4/dfa/dfa.py
--rw-r--r--   0        0        0      649 2024-03-10 00:27:29.679094 dfa-4.6.4/dfa/draw.py
--rw-r--r--   0        0        0     5695 2024-03-10 00:27:29.679094 dfa-4.6.4/dfa/utils.py
--rw-r--r--   0        0        0      670 2024-04-29 02:01:18.341259 dfa-4.6.4/pyproject.toml
--rw-r--r--   0        0        0     8629 1970-01-01 00:00:00.000000 dfa-4.6.4/PKG-INFO
+-rw-r--r--   0        0        0     1082 2024-04-06 21:02:22.520870 dfa-4.7.0/LICENSE
+-rw-r--r--   0        0        0     7737 2024-04-06 21:02:22.520870 dfa-4.7.0/README.md
+-rw-r--r--   0        0        0      230 2024-04-06 21:02:22.521870 dfa-4.7.0/dfa/__init__.py
+-rw-r--r--   0        0        0    11108 2024-05-03 04:23:29.638050 dfa-4.7.0/dfa/dfa.py
+-rw-r--r--   0        0        0      649 2024-04-06 21:02:22.521870 dfa-4.7.0/dfa/draw.py
+-rw-r--r--   0        0        0     6752 2024-05-08 03:32:12.192184 dfa-4.7.0/dfa/utils.py
+-rw-r--r--   0        0        0      670 2024-05-08 03:32:47.472021 dfa-4.7.0/pyproject.toml
+-rw-r--r--   0        0        0     8629 1970-01-01 00:00:00.000000 dfa-4.7.0/PKG-INFO
```

### Comparing `dfa-4.6.4/LICENSE` & `dfa-4.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dfa-4.6.4/README.md` & `dfa-4.7.0/README.md`

 * *Files identical despite different names*

### Comparing `dfa-4.6.4/dfa/dfa.py` & `dfa-4.7.0/dfa/dfa.py`

 * *Files identical despite different names*

### Comparing `dfa-4.6.4/dfa/draw.py` & `dfa-4.7.0/dfa/draw.py`

 * *Files identical despite different names*

### Comparing `dfa-4.6.4/dfa/utils.py` & `dfa-4.7.0/dfa/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import funcy as fn
 import itertools
 import random
-from collections import deque
+from collections import deque, defaultdict
 from bidict import bidict
 
 from dfa import DFA, State, Letter
 from collections import defaultdict
 
 
 DFADict = dict[State, tuple[Letter, dict[Letter, State]]]
@@ -164,7 +164,36 @@
     return DFA(
         start=orig.start,
         inputs=orig.inputs,
         outputs=orig.outputs,
         label=orig._label,
         transition=lambda s, c: state2rep[orig._transition(s, c)]
     ).normalize()
+
+
+def min_distance_to_accept_by_state(d: DFA):
+    """Returns a dictionary mapping states to the minimum number
+    of tokens necessary to reach an accepting state.
+
+    Note: If a state cannot reach an accepting state, the distance
+          is taken to be infinity.
+    """
+    # Construct inverse transition function.
+    inv_transition = defaultdict(set)
+    for state in d.states():
+        for token in d.inputs:
+            state2 = d._transition(state, token)
+            inv_transition[state2].add((state, token))
+
+    # BFS from the accepting states to the start state.
+    oo = -float('inf')
+    queue = deque([s for s in d.states() if d._label(s)])
+    depths = defaultdict(lambda: -oo, {s: 0 for s in queue})
+    while queue:
+        state = queue.pop()
+        depth = depths[state]
+        for (state2, token) in inv_transition[state]:
+            if state2 in depths:
+                continue  # Visited in BFS -> already have depth.
+            depths[state2] = depth + 1
+            queue.appendleft(state2)
+    return depths
```

### Comparing `dfa-4.6.4/pyproject.toml` & `dfa-4.7.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "dfa"
 readme="README.md"
-version = "4.6.4"
+version = "4.7.0"
 description = "Python library for modeling DFAs, Moore Machines, and Transition Systems."
 authors = ["Marcell Vazquez-Chanlatte <marcell.vc@eecs.berkeley.edu>"]
 repository = "https://github.com/mvcisback/dfa"
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `dfa-4.6.4/PKG-INFO` & `dfa-4.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dfa
-Version: 4.6.4
+Version: 4.7.0
 Summary: Python library for modeling DFAs, Moore Machines, and Transition Systems.
 Home-page: https://github.com/mvcisback/dfa
 License: MIT
 Author: Marcell Vazquez-Chanlatte
 Author-email: marcell.vc@eecs.berkeley.edu
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

