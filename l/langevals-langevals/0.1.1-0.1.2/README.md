# Comparing `tmp/langevals_langevals-0.1.1.tar.gz` & `tmp/langevals_langevals-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langevals_langevals-0.1.1.tar", max compression
+gzip compressed data, was "langevals_langevals-0.1.2.tar", max compression
```

## Comparing `langevals_langevals-0.1.1.tar` & `langevals_langevals-0.1.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     2186 2024-04-28 19:56:44.504808 langevals_langevals-0.1.1/langevals_langevals/competitor_blocklist.py
--rw-r--r--   0        0        0     6375 2024-04-28 19:56:44.504808 langevals_langevals-0.1.1/langevals_langevals/competitor_llm.py
--rw-r--r--   0        0        0     6710 2024-04-28 19:56:44.504808 langevals_langevals-0.1.1/langevals_langevals/off_topic.py
--rw-r--r--   0        0        0      470 2024-04-28 19:57:20.820565 langevals_langevals-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      533 1970-01-01 00:00:00.000000 langevals_langevals-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     2186 2024-05-07 14:19:44.470403 langevals_langevals-0.1.2/langevals_langevals/competitor_blocklist.py
+-rw-r--r--   0        0        0     6375 2024-05-07 14:19:44.470403 langevals_langevals-0.1.2/langevals_langevals/competitor_llm.py
+-rw-r--r--   0        0        0     6710 2024-05-07 14:19:44.470403 langevals_langevals-0.1.2/langevals_langevals/off_topic.py
+-rw-r--r--   0        0        0      470 2024-05-07 14:20:42.986794 langevals_langevals-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      533 1970-01-01 00:00:00.000000 langevals_langevals-0.1.2/PKG-INFO
```

### Comparing `langevals_langevals-0.1.1/langevals_langevals/competitor_blocklist.py` & `langevals_langevals-0.1.2/langevals_langevals/competitor_blocklist.py`

 * *Files identical despite different names*

### Comparing `langevals_langevals-0.1.1/langevals_langevals/competitor_llm.py` & `langevals_langevals-0.1.2/langevals_langevals/competitor_llm.py`

 * *Files identical despite different names*

### Comparing `langevals_langevals-0.1.1/langevals_langevals/off_topic.py` & `langevals_langevals-0.1.2/langevals_langevals/off_topic.py`

 * *Files identical despite different names*

### Comparing `langevals_langevals-0.1.1/PKG-INFO` & `langevals_langevals-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: langevals-langevals
-Version: 0.1.1
+Version: 0.1.2
 Summary: LangEvals house-made classification.
 License: MIT
 Author: Yevhenii Budnyk
 Author-email: y.budnyk789@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: langevals-core (>=0.1.2,<0.2.0)
+Requires-Dist: langevals-core (>=0.1.3,<0.2.0)
 Requires-Dist: litellm (>=1.31.3,<2.0.0)
 Requires-Dist: openai (==1.13.3)
```

