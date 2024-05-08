# Comparing `tmp/nl_matcher-0.0.3.tar.gz` & `tmp/nl_matcher-0.0.4.tar.gz`

## Comparing `nl_matcher-0.0.3.tar` & `nl_matcher-0.0.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 nl_matcher-0.0.3/main.py
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 nl_matcher-0.0.3/requirements.txt
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 nl_matcher-0.0.3/requirements_dev.txt
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 nl_matcher-0.0.3/src/nl_matcher/__init__.py
--rw-r--r--   0        0        0     3015 2020-02-02 00:00:00.000000 nl_matcher-0.0.3/src/nl_matcher/location_matcher.py
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 nl_matcher-0.0.3/src/nl_matcher/rules/cfg
--rw-r--r--   0        0        0   703364 2020-02-02 00:00:00.000000 nl_matcher-0.0.3/src/nl_matcher/rules/patterns.jsonl
--rw-r--r--   0        0        0     6890 2020-02-02 00:00:00.000000 nl_matcher-0.0.3/tests/test_location_matcher.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 nl_matcher-0.0.3/.gitignore
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 nl_matcher-0.0.3/README.md
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 nl_matcher-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 nl_matcher-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 nl_matcher-0.0.4/requirements.txt
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 nl_matcher-0.0.4/requirements_dev.txt
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 nl_matcher-0.0.4/src/nlmatcher/__init__.py
+-rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 nl_matcher-0.0.4/src/nlmatcher/location_matcher.py
+-rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 nl_matcher-0.0.4/src/nlmatcher/patterns.py
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 nl_matcher-0.0.4/src/nlmatcher/rules/cfg
+-rw-r--r--   0        0        0   703364 2020-02-02 00:00:00.000000 nl_matcher-0.0.4/src/nlmatcher/rules/patterns.jsonl
+-rw-r--r--   0        0        0     8493 2020-02-02 00:00:00.000000 nl_matcher-0.0.4/tests/test_location_matcher.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 nl_matcher-0.0.4/.gitignore
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 nl_matcher-0.0.4/README.md
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 nl_matcher-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 nl_matcher-0.0.4/PKG-INFO
```

### Comparing `nl_matcher-0.0.3/src/nl_matcher/rules/patterns.jsonl` & `nl_matcher-0.0.4/src/nlmatcher/rules/patterns.jsonl`

 * *Files identical despite different names*

### Comparing `nl_matcher-0.0.3/pyproject.toml` & `nl_matcher-0.0.4/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
+[tool.hatch.build.targets.wheel]
+packages = ["src/nlmatcher"]
+
 [project]
 name = "nl-matcher"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Diego Da'Silva", email="smartcrashomg@gmail.com" },
 ]
 description = "A simple library to match locations in text using SpaCy"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `nl_matcher-0.0.3/PKG-INFO` & `nl_matcher-0.0.4/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,44 @@
 Metadata-Version: 2.3
 Name: nl-matcher
-Version: 0.0.3
+Version: 0.0.4
 Summary: A simple library to match locations in text using SpaCy
 Project-URL: Homepage, https://github.com/smartcrash/nlmatcher
 Project-URL: Issues, https://github.com/smartcrash/nlmatcher/issues
 Author-email: Diego Da'Silva <smartcrashomg@gmail.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Requires-Dist: spacy
 Description-Content-Type: text/markdown
 
 # NL Matcher
 
 A simple library to match locations in text using SpaCy
+
+## Installation
+
+```bash
+pip install nlmatcher
+```
+
+## Usage
+
+```python
+import nlmatcher
+
+matcher = nlmatcher.LocationMatcher()
+
+text = "I live in Amsterdam and work in Utrecht"
+matches = matcher.match(text)
+
+for match in matches:
+    print(match.text)
+```
+
+## Output
+
+```
+Amsterdam
+Utrecht
+```
```

