# Comparing `tmp/typst_pyimage-0.0.3.tar.gz` & `tmp/typst_pyimage-0.0.4.tar.gz`

## Comparing `typst_pyimage-0.0.3.tar` & `typst_pyimage-0.0.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 typst_pyimage-0.0.3/typst_pyimage/__init__.py
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 typst_pyimage-0.0.3/typst_pyimage/__main__.py
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 typst_pyimage-0.0.3/typst_pyimage/pyimage.typ
--rw-r--r--   0        0        0     5866 2020-02-02 00:00:00.000000 typst_pyimage-0.0.3/typst_pyimage/run.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 typst_pyimage-0.0.3/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 typst_pyimage-0.0.3/LICENSE
--rw-r--r--   0        0        0     4012 2020-02-02 00:00:00.000000 typst_pyimage-0.0.3/README.md
--rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 typst_pyimage-0.0.3/pyproject.toml
--rw-r--r--   0        0        0    17692 2020-02-02 00:00:00.000000 typst_pyimage-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 typst_pyimage-0.0.4/typst_pyimage/__init__.py
+-rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 typst_pyimage-0.0.4/typst_pyimage/__main__.py
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 typst_pyimage-0.0.4/typst_pyimage/pyimage.typ
+-rw-r--r--   0        0        0     6095 2020-02-02 00:00:00.000000 typst_pyimage-0.0.4/typst_pyimage/run.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 typst_pyimage-0.0.4/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 typst_pyimage-0.0.4/LICENSE
+-rw-r--r--   0        0        0     4105 2020-02-02 00:00:00.000000 typst_pyimage-0.0.4/README.md
+-rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 typst_pyimage-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0    17785 2020-02-02 00:00:00.000000 typst_pyimage-0.0.4/PKG-INFO
```

### Comparing `typst_pyimage-0.0.3/typst_pyimage/run.py` & `typst_pyimage-0.0.4/typst_pyimage/run.py`

 * *Files 2% similar despite different names*

```diff
@@ -150,26 +150,32 @@
     shutil.copy(installpath / "pyimage.typ", dirpath / "pyimage.typ")
     init_code, init_scope = _make_images(
         filepath, dirpath, figcache, contentcache, "", {}
     )
     return filepath, dirpath, init_code, init_scope
 
 
-def watch(filename: Union[str, pathlib.Path], timeout_s: Optional[int] = None):
+def watch(
+    filename: Union[str, pathlib.Path],
+    extra_args: Optional[list[str]] = None,
+    timeout_s: Optional[int] = None,
+):
+    if extra_args is None:
+        extra_args = []
     figcache = {}
     contentcache = {}
     filepath, dirpath, init_code, init_scope = _initial(
         filename, contentcache, figcache
     )
     del filename
     start_time = time.time()
     file_time = last_time = _get_file_time(filepath)
     keep_running = True
     need_update = False
-    process = subprocess.Popen(["typst", "watch", str(filepath)])
+    process = subprocess.Popen(["typst", "watch"] + extra_args + [str(filepath)])
     try:
         while keep_running:
             if need_update:
                 last_time = file_time
                 init_code, init_scope = _make_images(
                     filepath, dirpath, figcache, contentcache, init_code, init_scope
                 )
@@ -180,10 +186,12 @@
                 keep_running = time.time() < start_time + timeout_s
     except KeyboardInterrupt:
         pass
     finally:
         process.kill()
 
 
-def compile(filename: Union[str, pathlib.Path]):
+def compile(filename: Union[str, pathlib.Path], extra_args: Optional[list[str]] = None):
+    if extra_args is None:
+        extra_args = []
     filepath, _, _, _ = _initial(filename, figcache=None, contentcache=None)
-    subprocess.run(["typst", "compile", str(filepath)])
+    subprocess.run(["typst", "compile"] + extra_args + [str(filepath)])
```

### Comparing `typst_pyimage-0.0.3/LICENSE` & `typst_pyimage-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `typst_pyimage-0.0.3/README.md` & `typst_pyimage-0.0.4/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -57,36 +57,41 @@
 
 ## Usage
 
 1. Import `pyimage.typ`. At the start of your `.typ` file, add the line `#import ".typst_pyimage/pyimage.typ": pyimage, pycontent, pyinit`.
 
 2. Use these functions.
 
-    a. `pyimage(string, ..arguments) -> content`. The positional string should be a Python program that creates a single matplotlib figure. Any named arguments are forwarded on to Typst's built-in `image` function. You can use it just like the normal `image` function, e.g. `#align(center, pyimage("..."))`.
+   a. `pyimage(string, ..arguments) -> content`. The positional string should be a Python program that creates a single matplotlib figure. Any named arguments are forwarded on to Typst's built-in `image` function. You can use it just like the normal `image` function, e.g. `#align(center, pyimage("..."))`.
 
-    b. `pycontent(string)`. The positional string should be a Python program that produces a string on its final line. This will be treated as Typst code.
+   b. `pycontent(string)`. The positional string should be a Python program that produces a string on its final line. This string will be treated as Typst code.
 
-    c. `pyinit(string)`. The positional string should be a Python program. This will be evaluated before all `pyimage` or `pycontent` calls, e.g. to do import or perform setup.
+   c. `pyinit(string)`. The positional string should be a Python program. This will be evaluated before all `pyimage` or `pycontent` calls, e.g. to perform imports or other setup.
 
 3. Compile or watch. Run either of the following two commands:
-    ```
-    python -m typst_pyimage compile your_file.typ
-    python -m typst_pyimage watch your_file.typ
-    ```
-    This will extract and run all your Python code. In addition it will call either `typst compile your_file.typ` or `typst watch your_file.typ`.
 
-    The resulting images are saved in the `.typst_pyimage` folder.
+   ```
+   python -m typst_pyimage compile your_file.typ
+   python -m typst_pyimage watch your_file.typ
+   ```
+
+   This will extract and run all your Python code. In addition it will call either `typst compile your_file.typ` or `typst watch your_file.typ`.
+
+   The resulting images are saved in the `.typst_pyimage` folder.
+
+   For more information on the available arguments, run `python -m typst_pyimage -h`.
 
 ## Notes
 
 It's common to have an initial block of code that is in common to all `#pyimage("...")` and `#pycontent("...")` calls (such as import statements, defining helpers etc). These can be placed in a `#pyinit("...")` directive.
 
 Each `#pyimage("...")` block is executed as a fresh module (i.e. as if each was a separate Python file), but with the same Python interpreter.
 
 Overall, this is essentially equivalent to the following Python code:
+
 ```
 # main.py
 import pyinit
 import pyimage1
 import pyimage2
 
 # pyinit.py
@@ -96,14 +101,15 @@
 from pyinit import *
 ...  # your first #pyimage("...") code
 
 # pyimage2.py
 from pyinit import *
 ...  # your second #pyimage("...") code
 ```
+
 This means that e.g. any global caches will be shared across all `#pyimage("...")` calls. (Useful when using a library like JAX, which has a JIT compilation cache.)
 
 ## Limitations
 
 1. The watcher just extracts all the `pyimage("...")` etc. blocks via regex, and runs them in the order that they appear in the file. This means that (a) the `"` character may not appear anywhere in the Python code (even if escaped), and (b) trying to call `pyimage` etc. dynamically (i.e. not with a literal string at the top level of your program) will not work.
 2. Only `pyimage("...")` etc. calls inside the single watched file are tracked.
```

### Comparing `typst_pyimage-0.0.3/pyproject.toml` & `typst_pyimage-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "typst_pyimage"
-version = "0.0.3"
+version = "0.0.4"
 description = "Typst extension, adding support for generating figures using inline Python code"
 readme = "README.md"
 requires-python = "~=3.8"
 license = {file = "LICENSE"}
 authors = [
   {name = "Patrick Kidger", email = "contact@kidger.site"},
 ]
```

### Comparing `typst_pyimage-0.0.3/PKG-INFO` & `typst_pyimage-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: typst_pyimage
-Version: 0.0.3
+Version: 0.0.4
 Summary: Typst extension, adding support for generating figures using inline Python code
 Project-URL: repository, https://github.com/patrick-kidger/typst_pyimage
 Author-email: Patrick Kidger <contact@kidger.site>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -276,36 +276,41 @@
 
 ## Usage
 
 1. Import `pyimage.typ`. At the start of your `.typ` file, add the line `#import ".typst_pyimage/pyimage.typ": pyimage, pycontent, pyinit`.
 
 2. Use these functions.
 
-    a. `pyimage(string, ..arguments) -> content`. The positional string should be a Python program that creates a single matplotlib figure. Any named arguments are forwarded on to Typst's built-in `image` function. You can use it just like the normal `image` function, e.g. `#align(center, pyimage("..."))`.
+   a. `pyimage(string, ..arguments) -> content`. The positional string should be a Python program that creates a single matplotlib figure. Any named arguments are forwarded on to Typst's built-in `image` function. You can use it just like the normal `image` function, e.g. `#align(center, pyimage("..."))`.
 
-    b. `pycontent(string)`. The positional string should be a Python program that produces a string on its final line. This will be treated as Typst code.
+   b. `pycontent(string)`. The positional string should be a Python program that produces a string on its final line. This string will be treated as Typst code.
 
-    c. `pyinit(string)`. The positional string should be a Python program. This will be evaluated before all `pyimage` or `pycontent` calls, e.g. to do import or perform setup.
+   c. `pyinit(string)`. The positional string should be a Python program. This will be evaluated before all `pyimage` or `pycontent` calls, e.g. to perform imports or other setup.
 
 3. Compile or watch. Run either of the following two commands:
-    ```
-    python -m typst_pyimage compile your_file.typ
-    python -m typst_pyimage watch your_file.typ
-    ```
-    This will extract and run all your Python code. In addition it will call either `typst compile your_file.typ` or `typst watch your_file.typ`.
 
-    The resulting images are saved in the `.typst_pyimage` folder.
+   ```
+   python -m typst_pyimage compile your_file.typ
+   python -m typst_pyimage watch your_file.typ
+   ```
+
+   This will extract and run all your Python code. In addition it will call either `typst compile your_file.typ` or `typst watch your_file.typ`.
+
+   The resulting images are saved in the `.typst_pyimage` folder.
+
+   For more information on the available arguments, run `python -m typst_pyimage -h`.
 
 ## Notes
 
 It's common to have an initial block of code that is in common to all `#pyimage("...")` and `#pycontent("...")` calls (such as import statements, defining helpers etc). These can be placed in a `#pyinit("...")` directive.
 
 Each `#pyimage("...")` block is executed as a fresh module (i.e. as if each was a separate Python file), but with the same Python interpreter.
 
 Overall, this is essentially equivalent to the following Python code:
+
 ```
 # main.py
 import pyinit
 import pyimage1
 import pyimage2
 
 # pyinit.py
@@ -315,14 +320,15 @@
 from pyinit import *
 ...  # your first #pyimage("...") code
 
 # pyimage2.py
 from pyinit import *
 ...  # your second #pyimage("...") code
 ```
+
 This means that e.g. any global caches will be shared across all `#pyimage("...")` calls. (Useful when using a library like JAX, which has a JIT compilation cache.)
 
 ## Limitations
 
 1. The watcher just extracts all the `pyimage("...")` etc. blocks via regex, and runs them in the order that they appear in the file. This means that (a) the `"` character may not appear anywhere in the Python code (even if escaped), and (b) trying to call `pyimage` etc. dynamically (i.e. not with a literal string at the top level of your program) will not work.
 2. Only `pyimage("...")` etc. calls inside the single watched file are tracked.
```

