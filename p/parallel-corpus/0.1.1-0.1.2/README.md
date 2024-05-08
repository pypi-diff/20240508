# Comparing `tmp/parallel_corpus-0.1.1.tar.gz` & `tmp/parallel_corpus-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parallel_corpus-0.1.1.tar", last modified: Tue May  7 06:56:15 2024, max compression
+gzip compressed data, was "parallel_corpus-0.1.2.tar", last modified: Wed May  8 11:01:14 2024, max compression
```

## Comparing `parallel_corpus-0.1.1.tar` & `parallel_corpus-0.1.2.tar`

### file list

```diff
@@ -1,31 +1,32 @@
--rw-r--r--   0        0        0     1069 2024-05-07 06:56:01.413518 parallel_corpus-0.1.1/LICENSE
--rw-r--r--   0        0        0     3001 2024-05-07 06:56:01.413518 parallel_corpus-0.1.1/README.md
--rw-r--r--   0        0        0     1382 2024-05-07 06:56:15.877604 parallel_corpus-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-07 06:56:01.413518 parallel_corpus-0.1.1/src/parallel_corpus/__init__.py
--rw-r--r--   0        0        0    13388 2024-05-07 06:56:01.413518 parallel_corpus-0.1.1/src/parallel_corpus/graph.py
--rw-r--r--   0        0        0      468 2024-05-07 06:56:01.413518 parallel_corpus-0.1.1/src/parallel_corpus/shared/__init__.py
--rw-r--r--   0        0        0      701 2024-05-07 06:56:01.413518 parallel_corpus-0.1.1/src/parallel_corpus/shared/dicts.py
--rw-r--r--   0        0        0     4351 2024-05-07 06:56:01.417518 parallel_corpus-0.1.1/src/parallel_corpus/shared/diffs.py
--rw-r--r--   0        0        0      306 2024-05-07 06:56:01.417518 parallel_corpus-0.1.1/src/parallel_corpus/shared/functional.py
--rw-r--r--   0        0        0      565 2024-05-07 06:56:01.417518 parallel_corpus-0.1.1/src/parallel_corpus/shared/ids.py
--rw-r--r--   0        0        0     1500 2024-05-07 06:56:01.417518 parallel_corpus-0.1.1/src/parallel_corpus/shared/lists.py
--rw-r--r--   0        0        0     1414 2024-05-07 06:56:01.417518 parallel_corpus-0.1.1/src/parallel_corpus/shared/ranges.py
--rw-r--r--   0        0        0      170 2024-05-07 06:56:01.417518 parallel_corpus-0.1.1/src/parallel_corpus/shared/str_map.py
--rw-r--r--   0        0        0     3349 2024-05-07 06:56:01.417518 parallel_corpus-0.1.1/src/parallel_corpus/shared/union_find.py
--rw-r--r--   0        0        0      911 2024-05-07 06:56:01.417518 parallel_corpus-0.1.1/src/parallel_corpus/shared/unique_check.py
--rw-r--r--   0        0        0      649 2024-05-07 06:56:01.417518 parallel_corpus-0.1.1/src/parallel_corpus/source_target.py
--rw-r--r--   0        0        0     2056 2024-05-07 06:56:01.417518 parallel_corpus-0.1.1/src/parallel_corpus/token.py
--rw-r--r--   0        0        0        0 2024-05-07 06:56:01.417518 parallel_corpus-0.1.1/tests/__init__.py
--rw-r--r--   0        0        0     2527 2024-05-07 06:56:01.417518 parallel_corpus-0.1.1/tests/__snapshots__/test_graph.ambr
--rw-r--r--   0        0        0      514 2024-05-07 06:56:01.417518 parallel_corpus-0.1.1/tests/__snapshots__/test_token.ambr
--rw-r--r--   0        0        0    21049 2024-05-07 06:56:01.417518 parallel_corpus-0.1.1/tests/requirements-testing.lock
--rw-r--r--   0        0        0     7921 2024-05-07 06:56:01.417518 parallel_corpus-0.1.1/tests/test_graph.py
--rw-r--r--   0        0        0      965 2024-05-07 06:56:01.417518 parallel_corpus-0.1.1/tests/test_shared/__snapshots__/test_ranges.ambr
--rw-r--r--   0        0        0      470 2024-05-07 06:56:01.417518 parallel_corpus-0.1.1/tests/test_shared/test_diffs.py
--rw-r--r--   0        0        0      393 2024-05-07 06:56:01.417518 parallel_corpus-0.1.1/tests/test_shared/test_functional.py
--rw-r--r--   0        0        0      225 2024-05-07 06:56:01.417518 parallel_corpus-0.1.1/tests/test_shared/test_ids.py
--rw-r--r--   0        0        0      377 2024-05-07 06:56:01.417518 parallel_corpus-0.1.1/tests/test_shared/test_lists.py
--rw-r--r--   0        0        0      484 2024-05-07 06:56:01.417518 parallel_corpus-0.1.1/tests/test_shared/test_ranges.py
--rw-r--r--   0        0        0     1143 2024-05-07 06:56:01.417518 parallel_corpus-0.1.1/tests/test_shared/test_union_find.py
--rw-r--r--   0        0        0      867 2024-05-07 06:56:01.417518 parallel_corpus-0.1.1/tests/test_token.py
--rw-r--r--   0        0        0     4121 1970-01-01 00:00:00.000000 parallel_corpus-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-08 11:01:02.211826 parallel_corpus-0.1.2/LICENSE
+-rw-r--r--   0        0        0     3001 2024-05-08 11:01:02.211826 parallel_corpus-0.1.2/README.md
+-rw-r--r--   0        0        0     1382 2024-05-08 11:01:14.455782 parallel_corpus-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-08 11:01:02.211826 parallel_corpus-0.1.2/src/parallel_corpus/__init__.py
+-rw-r--r--   0        0        0    15099 2024-05-08 11:01:02.211826 parallel_corpus-0.1.2/src/parallel_corpus/graph.py
+-rw-r--r--   0        0        0        0 2024-05-08 11:01:02.211826 parallel_corpus-0.1.2/src/parallel_corpus/py.typed
+-rw-r--r--   0        0        0      468 2024-05-08 11:01:02.211826 parallel_corpus-0.1.2/src/parallel_corpus/shared/__init__.py
+-rw-r--r--   0        0        0      701 2024-05-08 11:01:02.211826 parallel_corpus-0.1.2/src/parallel_corpus/shared/dicts.py
+-rw-r--r--   0        0        0     4351 2024-05-08 11:01:02.211826 parallel_corpus-0.1.2/src/parallel_corpus/shared/diffs.py
+-rw-r--r--   0        0        0      306 2024-05-08 11:01:02.211826 parallel_corpus-0.1.2/src/parallel_corpus/shared/functional.py
+-rw-r--r--   0        0        0      565 2024-05-08 11:01:02.211826 parallel_corpus-0.1.2/src/parallel_corpus/shared/ids.py
+-rw-r--r--   0        0        0     1500 2024-05-08 11:01:02.211826 parallel_corpus-0.1.2/src/parallel_corpus/shared/lists.py
+-rw-r--r--   0        0        0     1414 2024-05-08 11:01:02.211826 parallel_corpus-0.1.2/src/parallel_corpus/shared/ranges.py
+-rw-r--r--   0        0        0      170 2024-05-08 11:01:02.211826 parallel_corpus-0.1.2/src/parallel_corpus/shared/str_map.py
+-rw-r--r--   0        0        0     3349 2024-05-08 11:01:02.211826 parallel_corpus-0.1.2/src/parallel_corpus/shared/union_find.py
+-rw-r--r--   0        0        0      911 2024-05-08 11:01:02.211826 parallel_corpus-0.1.2/src/parallel_corpus/shared/unique_check.py
+-rw-r--r--   0        0        0      649 2024-05-08 11:01:02.211826 parallel_corpus-0.1.2/src/parallel_corpus/source_target.py
+-rw-r--r--   0        0        0     2056 2024-05-08 11:01:02.211826 parallel_corpus-0.1.2/src/parallel_corpus/token.py
+-rw-r--r--   0        0        0        0 2024-05-08 11:01:02.211826 parallel_corpus-0.1.2/tests/__init__.py
+-rw-r--r--   0        0        0     2527 2024-05-08 11:01:02.215826 parallel_corpus-0.1.2/tests/__snapshots__/test_graph.ambr
+-rw-r--r--   0        0        0      514 2024-05-08 11:01:02.215826 parallel_corpus-0.1.2/tests/__snapshots__/test_token.ambr
+-rw-r--r--   0        0        0    21049 2024-05-08 11:01:02.215826 parallel_corpus-0.1.2/tests/requirements-testing.lock
+-rw-r--r--   0        0        0     9500 2024-05-08 11:01:02.215826 parallel_corpus-0.1.2/tests/test_graph.py
+-rw-r--r--   0        0        0      965 2024-05-08 11:01:02.215826 parallel_corpus-0.1.2/tests/test_shared/__snapshots__/test_ranges.ambr
+-rw-r--r--   0        0        0      470 2024-05-08 11:01:02.215826 parallel_corpus-0.1.2/tests/test_shared/test_diffs.py
+-rw-r--r--   0        0        0      393 2024-05-08 11:01:02.215826 parallel_corpus-0.1.2/tests/test_shared/test_functional.py
+-rw-r--r--   0        0        0      225 2024-05-08 11:01:02.215826 parallel_corpus-0.1.2/tests/test_shared/test_ids.py
+-rw-r--r--   0        0        0      377 2024-05-08 11:01:02.215826 parallel_corpus-0.1.2/tests/test_shared/test_lists.py
+-rw-r--r--   0        0        0      484 2024-05-08 11:01:02.215826 parallel_corpus-0.1.2/tests/test_shared/test_ranges.py
+-rw-r--r--   0        0        0     1143 2024-05-08 11:01:02.215826 parallel_corpus-0.1.2/tests/test_shared/test_union_find.py
+-rw-r--r--   0        0        0      867 2024-05-08 11:01:02.215826 parallel_corpus-0.1.2/tests/test_token.py
+-rw-r--r--   0        0        0     4121 1970-01-01 00:00:00.000000 parallel_corpus-0.1.2/PKG-INFO
```

### Comparing `parallel_corpus-0.1.1/LICENSE` & `parallel_corpus-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `parallel_corpus-0.1.1/README.md` & `parallel_corpus-0.1.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 pdm add parallel-corpus
 ```
 
 To add `parallel-corpus` manually to `pyproject.toml`:
 
 ```toml
 [project]
-dependencies = ["parallel-corpus>=0.1.1"]
+dependencies = ["parallel-corpus>=0.1.2"]
 ```
 
 ## Usage
 
 ```python
 first = "Jonathan saknades ."
```

### Comparing `parallel_corpus-0.1.1/pyproject.toml` & `parallel_corpus-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "parallel-corpus"
-version = "0.1.1"
+version = "0.1.2"
 description = "Parallel corpus as a graph."
 authors = [
     { name = "Språkbanken Text", email = "sb-info@svenska.gu.se" },
     { name = "Kristoffer Andersson", email = "kristoffer.andersson@gu.se" },
 ]
 dependencies = [
     "diff-match-patch>=20230430",
```

### Comparing `parallel_corpus-0.1.1/src/parallel_corpus/graph.py` & `parallel_corpus-0.1.2/src/parallel_corpus/graph.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Parallel corpus as a graph."""
 
 import itertools
 import logging
 import re
 from dataclasses import dataclass
-from typing import Dict, Iterable, List, Optional, TypeVar
+from typing import Dict, Iterable, List, Optional, TypedDict, TypeVar
 
 import parallel_corpus.shared.ranges
 import parallel_corpus.shared.str_map
 import parallel_corpus.shared.union_find
 from parallel_corpus import shared, token
 from parallel_corpus.shared import dicts, diffs, ids, lists
 from parallel_corpus.shared.unique_check import UniqueCheck
@@ -83,30 +83,85 @@
     return {e.id: e for e in es}
 
 
 def init(s: str, *, manual: bool = False) -> Graph:
     return init_from(token.tokenize(s), manual=manual)
 
 
+def init_with_source_and_target(source: str, target: str, *, manual: bool = False) -> Graph:
+    return init_from_source_and_target(
+        source=token.tokenize(source), target=token.tokenize(target), manual=manual
+    )
+
+
 def init_from(tokens: List[str], *, manual: bool = False) -> Graph:
     return align(
         Graph(
             source=token.identify(tokens, "s"),
             target=token.identify(tokens, "t"),
             edges=edge_record(
                 (edge([f"s{i}", f"t{i}"], [], manual=manual) for i, _ in enumerate(tokens))
             ),
         )
     )
 
 
+def init_from_source_and_target(
+    source: List[str], target: List[str], *, manual: bool = False
+) -> Graph:
+    source_tokens = token.identify(source, "s")
+    target_tokens = token.identify(target, "t")
+    return align(
+        Graph(
+            source=source_tokens,
+            target=target_tokens,
+            edges=edge_record(
+                itertools.chain(
+                    (edge([s.id], [], manual=manual) for s in source_tokens),
+                    (edge([t.id], [], manual=manual) for t in target_tokens),
+                )
+            ),
+        )
+    )
+
+
+class TextLabels(TypedDict):
+    text: str
+    labels: List[str]
+
+
+def from_unaligned(st: SourceTarget[List[TextLabels]]) -> Graph:
+    """Initialize a graph from unaligned tokens"""
+    edges: Dict[str, Edge] = {}
+
+    def proto_token_to_token(tok: TextLabels, i: int, prefix: str) -> Token:
+        id_ = f"{prefix}{i}"
+        e = edge([id_], tok["labels"], manual=False)
+        edges[id_] = e
+        return Token(tok["text"], id_)
+
+    def proto_tokens_to_tokens(toks: List[TextLabels], side: Side) -> List[Token]:
+        return [
+            proto_token_to_token(tok, i, "s" if side == Side.source else "t")
+            for i, tok in enumerate(toks)
+        ]
+
+    g = map_sides(st, proto_tokens_to_tokens)
+
+    return align(Graph(source=g.source, target=g.target, edges=edges))
+
+
 def modify(g: Graph, from_: int, to: int, text: str, side: Side = Side.target) -> Graph:
     return align(unaligned_modify(g, from_, to, text, side))
 
 
+def set_source(g: Graph, text: str) -> Graph:
+    return align(unaligned_set_side(g, Side.source, text))
+
+
 def set_target(g: Graph, text: str) -> Graph:
     return align(unaligned_set_side(g, Side.target, text))
 
 
 def merge_edges(*es) -> Edge:
     ids = []
     labels = []
```

### Comparing `parallel_corpus-0.1.1/src/parallel_corpus/shared/dicts.py` & `parallel_corpus-0.1.2/src/parallel_corpus/shared/dicts.py`

 * *Files identical despite different names*

### Comparing `parallel_corpus-0.1.1/src/parallel_corpus/shared/diffs.py` & `parallel_corpus-0.1.2/src/parallel_corpus/shared/diffs.py`

 * *Files identical despite different names*

### Comparing `parallel_corpus-0.1.1/src/parallel_corpus/shared/ids.py` & `parallel_corpus-0.1.2/src/parallel_corpus/shared/ids.py`

 * *Files identical despite different names*

### Comparing `parallel_corpus-0.1.1/src/parallel_corpus/shared/lists.py` & `parallel_corpus-0.1.2/src/parallel_corpus/shared/lists.py`

 * *Files identical despite different names*

### Comparing `parallel_corpus-0.1.1/src/parallel_corpus/shared/ranges.py` & `parallel_corpus-0.1.2/src/parallel_corpus/shared/ranges.py`

 * *Files identical despite different names*

### Comparing `parallel_corpus-0.1.1/src/parallel_corpus/shared/union_find.py` & `parallel_corpus-0.1.2/src/parallel_corpus/shared/union_find.py`

 * *Files identical despite different names*

### Comparing `parallel_corpus-0.1.1/src/parallel_corpus/shared/unique_check.py` & `parallel_corpus-0.1.2/src/parallel_corpus/shared/unique_check.py`

 * *Files identical despite different names*

### Comparing `parallel_corpus-0.1.1/src/parallel_corpus/source_target.py` & `parallel_corpus-0.1.2/src/parallel_corpus/source_target.py`

 * *Files identical despite different names*

### Comparing `parallel_corpus-0.1.1/src/parallel_corpus/token.py` & `parallel_corpus-0.1.2/src/parallel_corpus/token.py`

 * *Files identical despite different names*

### Comparing `parallel_corpus-0.1.1/tests/__snapshots__/test_graph.ambr` & `parallel_corpus-0.1.2/tests/__snapshots__/test_graph.ambr`

 * *Files identical despite different names*

### Comparing `parallel_corpus-0.1.1/tests/__snapshots__/test_token.ambr` & `parallel_corpus-0.1.2/tests/__snapshots__/test_token.ambr`

 * *Files identical despite different names*

### Comparing `parallel_corpus-0.1.1/tests/requirements-testing.lock` & `parallel_corpus-0.1.2/tests/requirements-testing.lock`

 * *Files 1% similar despite different names*

```diff
@@ -229,17 +229,17 @@
     --hash=sha256:f7b63ef50f1b690dddf550d03497b66d609393b40b564ed0d674909a68ebf16a
 questionary==2.0.1 \
     --hash=sha256:8ab9a01d0b91b68444dff7f6652c1e754105533f083cbe27597c8110ecc230a2 \
     --hash=sha256:bcce898bf3dbb446ff62830c86c5c6fb9a22a54146f0f5597d3da43b10d8fc8b
 rich==13.7.1 \
     --hash=sha256:4edbae314f59eb482f54e9e30bf00d33350aaa94f4bfcd4e9e3110e64d0d7222 \
     --hash=sha256:9be308cb1fe2f1f57d67ce99e95af38a1e2bc71ad9813b0e247cf7ffbcc3a432
-rich-click==1.8.0 \
-    --hash=sha256:846f504eb83a948d864888b2d73c71e52c310490c2babceac57e388aead086e2 \
-    --hash=sha256:f8cad0d67d286d6cd6fc9f69f2d6f25c6c4c2d99fb9d6cb3b8987b593dbe6fa8
+rich-click==1.8.1 \
+    --hash=sha256:0cf0bf84404e78379bd2722db88cb07ffd0535440e20a05943d5b02249d90f8a \
+    --hash=sha256:73c2ec88a66d7bf6b8c32783539d1c9c92c7c75847f14186092d27f83b206e8a
 ruff==0.4.3 \
     --hash=sha256:08a0d6a22918ab2552ace96adeaca308833873a4d7d1d587bb1d37bae8728eb3 \
     --hash=sha256:0bfc9e955e6dc6359eb6f82ea150c4f4e82b660e5b58d9a20a0e42ec3bb6342b \
     --hash=sha256:18b00e0bcccf0fc8d7186ed21e311dffd19761cb632241a6e4fe4477cc80ef6e \
     --hash=sha256:25cacda2155778beb0d064e0ec5a3944dcca9c12715f7c4634fd9d93ac33fd30 \
     --hash=sha256:262f5635e2c74d80b7507fbc2fac28fe0d4fef26373bbc62039526f7722bca1b \
     --hash=sha256:29efff25bf9ee685c2c8390563a5b5c006a3fee5230d28ea39f4f75f9d0b6f2f \
```

### Comparing `parallel_corpus-0.1.1/tests/test_graph.py` & `parallel_corpus-0.1.2/tests/test_graph.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,63 @@
 from typing import List
 
 import pytest
 from parallel_corpus import graph, token
-from parallel_corpus.source_target import Side
+from parallel_corpus.source_target import Side, SourceTarget
 
 
 def test_graph_init() -> None:
     g = graph.init("w1 w2")
     source = [token.Token(text="w1 ", id="s0"), token.Token(text="w2 ", id="s1")]
     target = [token.Token(text="w1 ", id="t0"), token.Token(text="w2 ", id="t1")]
     edges = graph.edge_record([graph.edge(["s0", "t0"], []), graph.edge(["s1", "t1"], [])])
 
     assert g.source == source
     assert g.target == target
     assert g.edges == edges
 
 
+def test_init_from_source_and_target_1() -> None:
+    g = graph.init_with_source_and_target(source="apa", target="apa")
+    assert g == graph.init("apa")
+
+
+def test_init_from_source_and_target_2() -> None:
+    g = graph.init_with_source_and_target(source="apa bepa", target="apa")
+    expected_source = token.identify(token.tokenize("apa bepa"), "s")
+    expected_target = token.identify(token.tokenize("apa"), "t")
+    g_expected = graph.Graph(
+        source=expected_source,
+        target=expected_target,
+        edges=graph.edge_record([graph.edge(["s0", "t0"], []), graph.edge(["s1"], [])]),
+    )
+    assert g == g_expected
+
+
+def test_init_from_source_and_target_3() -> None:
+    g = graph.init_with_source_and_target(source="apa", target="bepa apa")
+    expected_source = token.identify(token.tokenize("apa"), "s")
+    expected_target = token.identify(token.tokenize("bepa apa"), "t")
+    g_expected = graph.Graph(
+        source=expected_source,
+        target=expected_target,
+        edges=graph.edge_record([graph.edge(["s0", "t1"], []), graph.edge(["t0"], [])]),
+    )
+    assert g == g_expected
+
+
+def test_from_unaligned() -> None:
+    g = graph.from_unaligned(
+        SourceTarget(
+            source=[{"text": "apa ", "labels": []}], target=[{"text": "apa ", "labels": []}]
+        )
+    )
+    assert g == graph.init("apa")
+
+
 def test_graph_case1() -> None:
     first = "Jonathan saknades , emedan han , med sin vapendragare , redan på annat håll sökt och anträffat fienden ."  # noqa: E501
     second = "Jonat han saknades , emedan han , med sin vapendragare , redan på annat håll sökt och anträffat fienden ."  # noqa: E501
 
     g = graph.init(first)
 
     gm = graph.set_target(g, second)
@@ -34,14 +72,25 @@
     g = graph.init(first)
 
     gm = graph.set_target(g, second)
     print(f"{gm=}")
     assert "e-s0-s1-t20" in gm.edges
 
 
+def test_set_source() -> None:
+    source = "Jonat han saknades"
+    target = "Jonathan saknaes"
+
+    g = graph.init(target)
+
+    gm = graph.set_source(g, source)
+    print(f"{gm=}")
+    assert "e-s2-s3-t0" in gm.edges
+
+
 def test_unaligned_set_side() -> None:
     g0 = graph.init("a bc d")
     print(">>> test_unaligned_set_side")
     g = graph.unaligned_set_side(g0, Side.target, "ab c d")
     print("<<< test_unaligned_set_side")
 
     expected_source = [
```

### Comparing `parallel_corpus-0.1.1/tests/test_shared/__snapshots__/test_ranges.ambr` & `parallel_corpus-0.1.2/tests/test_shared/__snapshots__/test_ranges.ambr`

 * *Files identical despite different names*

### Comparing `parallel_corpus-0.1.1/tests/test_shared/test_union_find.py` & `parallel_corpus-0.1.2/tests/test_shared/test_union_find.py`

 * *Files identical despite different names*

### Comparing `parallel_corpus-0.1.1/tests/test_token.py` & `parallel_corpus-0.1.2/tests/test_token.py`

 * *Files identical despite different names*

### Comparing `parallel_corpus-0.1.1/PKG-INFO` & `parallel_corpus-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parallel-corpus
-Version: 0.1.1
+Version: 0.1.2
 Summary: Parallel corpus as a graph.
 Author-Email: =?utf-8?q?Spr=C3=A5kbanken_Text?= <sb-info@svenska.gu.se>, Kristoffer Andersson <kristoffer.andersson@gu.se>
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix
@@ -58,15 +58,15 @@
 pdm add parallel-corpus
 ```
 
 To add `parallel-corpus` manually to `pyproject.toml`:
 
 ```toml
 [project]
-dependencies = ["parallel-corpus>=0.1.1"]
+dependencies = ["parallel-corpus>=0.1.2"]
 ```
 
 ## Usage
 
 ```python
 first = "Jonathan saknades ."
```

