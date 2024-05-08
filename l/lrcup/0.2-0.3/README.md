# Comparing `tmp/lrcup-0.2.tar.gz` & `tmp/lrcup-0.3.tar.gz`

## Comparing `lrcup-0.2.tar` & `lrcup-0.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 lrcup-0.2/lrcup/__init__.py
--rw-r--r--   0        0        0     4423 2020-02-02 00:00:00.000000 lrcup-0.2/lrcup/__main__.py
--rw-r--r--   0        0        0     3727 2020-02-02 00:00:00.000000 lrcup-0.2/lrcup/controller.py
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 lrcup-0.2/.gitignore
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 lrcup-0.2/LICENSE.txt
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 lrcup-0.2/README.md
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 lrcup-0.2/pyproject.toml
--rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 lrcup-0.2/PKG-INFO
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 lrcup-0.3/lrcup/__init__.py
+-rw-r--r--   0        0        0     4683 2020-02-02 00:00:00.000000 lrcup-0.3/lrcup/__main__.py
+-rw-r--r--   0        0        0     3727 2020-02-02 00:00:00.000000 lrcup-0.3/lrcup/controller.py
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 lrcup-0.3/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 lrcup-0.3/LICENSE.txt
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 lrcup-0.3/README.md
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 lrcup-0.3/pyproject.toml
+-rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 lrcup-0.3/PKG-INFO
```

### Comparing `lrcup-0.2/lrcup/__main__.py` & `lrcup-0.3/lrcup/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -100,14 +100,22 @@
         synced_lyrics
     )
     if not success:
         return click.secho("\nFailed to upload to LRCLIB.", fg = "red")
 
     click.secho("\nUploaded to LRCLIB successfully.", fg = "green")
 
+@lrcup.command(help = "Embed an LRC file into an audio file")
+@click.argument("lrc")
+@click.argument("destination")
+def embed(lrc: str, destination: str) -> None:
+    file = mutagen.File(destination)
+    file["LYRICS"] = Path(lrc).read_text()
+    file.save()
+
 @lrcup.command(help = "Search for specific lyrics by query")
 @click.argument("query", nargs = -1, required = True)
 def search(query: str) -> None:
     results = []
     for i in lrclib.search(" ".join(query)):
         if not (i["plainLyrics"] or i["syncedLyrics"]):
             continue  # Ignore instrumentals
```

### Comparing `lrcup-0.2/lrcup/controller.py` & `lrcup-0.3/lrcup/controller.py`

 * *Files identical despite different names*

### Comparing `lrcup-0.2/LICENSE.txt` & `lrcup-0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lrcup-0.2/README.md` & `lrcup-0.3/README.md`

 * *Files identical despite different names*

### Comparing `lrcup-0.2/pyproject.toml` & `lrcup-0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -28,8 +28,8 @@
 Homepage = "https://github.com/iiPythonx/lrcup"
 Issues = "https://github.com/iiPythonx/lrcup/issues"
 
 [tool.hatch.version]
 path = "lrcup/__init__.py"
 
 [project.scripts]
-lrcup = "lrcup.__main__:main"
+lrcup = "lrcup.__main__:lrcup"
```

### Comparing `lrcup-0.2/PKG-INFO` & `lrcup-0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: lrcup
-Version: 0.2
+Version: 0.3
 Summary: Python module and CLI for the LRCLIB API
 Project-URL: Homepage, https://github.com/iiPythonx/lrcup
 Project-URL: Issues, https://github.com/iiPythonx/lrcup/issues
 Author-email: iiPython <ben@iipython.dev>
 License-File: LICENSE.txt
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

