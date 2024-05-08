# Comparing `tmp/markcli-0.1.3.tar.gz` & `tmp/markcli-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "markcli-0.1.3.tar", last modified: Tue May  7 06:19:45 2024, max compression
+gzip compressed data, was "markcli-0.1.4.tar", last modified: Wed May  8 06:37:58 2024, max compression
```

## Comparing `markcli-0.1.3.tar` & `markcli-0.1.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 06:19:45.381658 markcli-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-07 06:19:38.000000 markcli-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    17698 2024-05-07 06:19:45.381658 markcli-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    17107 2024-05-07 06:19:38.000000 markcli-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 06:19:45.381658 markcli-0.1.3/markcli/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-07 06:19:38.000000 markcli-0.1.3/markcli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5620 2024-05-07 06:19:38.000000 markcli-0.1.3/markcli/markcli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 06:19:45.381658 markcli-0.1.3/markcli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    17698 2024-05-07 06:19:45.000000 markcli-0.1.3/markcli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-07 06:19:45.000000 markcli-0.1.3/markcli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 06:19:45.000000 markcli-0.1.3/markcli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-07 06:19:45.000000 markcli-0.1.3/markcli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-07 06:19:45.000000 markcli-0.1.3/markcli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-07 06:19:45.000000 markcli-0.1.3/markcli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 06:19:45.381658 markcli-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-07 06:19:38.000000 markcli-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:37:58.214984 markcli-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-08 06:37:54.000000 markcli-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    18012 2024-05-08 06:37:58.214984 markcli-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    17421 2024-05-08 06:37:54.000000 markcli-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:37:58.214984 markcli-0.1.4/markcli/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-08 06:37:54.000000 markcli-0.1.4/markcli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5865 2024-05-08 06:37:54.000000 markcli-0.1.4/markcli/markcli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:37:58.214984 markcli-0.1.4/markcli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    18012 2024-05-08 06:37:58.000000 markcli-0.1.4/markcli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-08 06:37:58.000000 markcli-0.1.4/markcli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 06:37:58.000000 markcli-0.1.4/markcli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-08 06:37:58.000000 markcli-0.1.4/markcli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-08 06:37:58.000000 markcli-0.1.4/markcli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-08 06:37:58.000000 markcli-0.1.4/markcli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 06:37:58.214984 markcli-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-08 06:37:54.000000 markcli-0.1.4/setup.py
```

### Comparing `markcli-0.1.3/LICENSE` & `markcli-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `markcli-0.1.3/PKG-INFO` & `markcli-0.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: markcli
-Version: 0.1.3
+Version: 0.1.4
 Summary: A Jupyter-inspired tool to create documentation of CLI tools.
 Home-page: UNKNOWN
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -14,41 +14,41 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # `markcli` - An Jupyter-inspired CLI Documentation Tool
 
 ## Description
-Run markcli to fill a template that results from running the cli command included inside.
+Run `markcli` to fill a template that results from running the cli command included inside.
 
-CLI commands are written in html comments (here with spaces added to avoid rendering) using the following syntax:
+CLI commands are written in `html` comments (here with spaces added to avoid rendering) using the following syntax:
 
 ```
 < ! - - 
 command_object
 - ->
 ```
 
-Where `command_object` is a json string object. The minimal object, where all parameters are defaulted is:
+Where `command_object` is a `json` string object. The minimal object, where all parameters are defaulted is:
 ```json
 {
     "command": "some bash command"
 }
 ```
 
  with the following properties (the first option mentioned is the default)
 ```javascript
 {
     "command": "ls -lt",
     "print_command": false/true             // print the command in the document
-    "output-format": "bash"/code block id   // Any value supported by md code blocks (e.g. json, python, etc.)
+    "output-format": "bash"/code block id   // Any value supported by md code blocks (e.g. json, python, etc.) using markdown with write the output not as a code block
     "limit": 0/any number                   // limit the number of lines printed
     "error-strategy": "ignore"\"exit",      // Behavior on error
     "skip": false/true,                     // If true, this command is not run. If true, it is run, and if the following block is an output (of a previous command), it is updated.
-     "object-type": N/A                     // Used internally by markcli to mark output blocks
+     "object-type": N/A                     // Used internally by `markcli` to mark output blocks
 }
 ```
 
 Example: running the previous will result in:
 
 <!--
 {
@@ -57,20 +57,21 @@
 }
 -->
 <!-- { "object-type": "command-output-start" } -->
 ```bash
 ls -lt
 ```
 ```bash
-total 24
--rw-r--r-- 1 runner docker     0 May  7 06:18 README.md
--rw-r--r-- 1 runner docker 11357 May  7 06:18 LICENSE
-drwxr-xr-x 2 runner docker  4096 May  7 06:18 markcli
--rw-r--r-- 1 runner docker  1065 May  7 06:18 setup.py
--rw-r--r-- 1 runner docker  3036 May  7 06:18 template.md
+total 28
+-rw-r--r-- 1 runner docker     0 May  8 06:36 README.md
+-rw-r--r-- 1 runner docker 11357 May  8 06:36 LICENSE
+-rw-r--r-- 1 runner docker   121 May  8 06:36 installation.md
+drwxr-xr-x 2 runner docker  4096 May  8 06:36 markcli
+-rw-r--r-- 1 runner docker  1065 May  8 06:36 setup.py
+-rw-r--r-- 1 runner docker  3064 May  8 06:36 template.md
 ```
 <!-- { "object-type": "command-output-end" } -->
 
 
 Commands can use environment variables, the parser assumes that any capitalized word is an environment variable. Example:
 <!--
 {
@@ -131,22 +132,31 @@
     parser = jsonargparse.ArgumentParser(
         description="A command line tool for generating templated documentation from clis",
     )
 ```
 <!-- { "object-type": "command-output-end" } -->
 
 
+<!--
+{
+    "command": "cat installation.md",
+    "output-format": "markdown"
+}
+-->
+<!-- { "object-type": "command-output-start" } -->
 # Installation
 
-To install markcli, run:
+To install `markcli`, run:
 ```bash
 pip install markcli
 ```
 
 Then the command `markcli` will be available.
+<!-- { "object-type": "command-output-end" } -->
+
 
 # A real-world example: document the valint command:
 <!--
 Some other commented text
 -->
 ## Install valint
 To install valint run (Note that the -- 2>&1 is required to capture the output in this setting, but is not required in a normal shell):
@@ -166,17 +176,18 @@
 scribe info Trying to download, tool=valint, version=latest
 scribe info Using dev artifacts, subpath='dev/valint/linux/amd64', ENV=dev
 scribe info Downloading, Version=1.4.0-6
   % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                  Dload  Upload   Total   Spent    Left  Speed
 
   0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0
-  0 28.5M    0 34028    0     0  75650      0  0:06:36 --:--:--  0:06:36 75617
- 69 28.5M   69 19.9M    0     0  14.1M      0  0:00:02  0:00:01  0:00:01 14.1M
-100 28.5M  100 28.5M    0     0  17.0M      0  0:00:01  0:00:01 --:--:-- 17.0M
+  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0
+
+  0 28.5M    0 17735    0     0  40073      0  0:12:27 --:--:--  0:12:27 40073
+100 28.5M  100 28.5M    0     0  40.8M      0 --:--:-- --:--:-- --:--:--  111M
 scribe info Installed /home/runner/.scribe/bin/valint
 
 ```
 <!-- { "object-type": "command-output-end" } -->
 
 
 ## General options
```

### Comparing `markcli-0.1.3/README.md` & `markcli-0.1.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 # `markcli` - An Jupyter-inspired CLI Documentation Tool
 
 ## Description
-Run markcli to fill a template that results from running the cli command included inside.
+Run `markcli` to fill a template that results from running the cli command included inside.
 
-CLI commands are written in html comments (here with spaces added to avoid rendering) using the following syntax:
+CLI commands are written in `html` comments (here with spaces added to avoid rendering) using the following syntax:
 
 ```
 < ! - - 
 command_object
 - ->
 ```
 
-Where `command_object` is a json string object. The minimal object, where all parameters are defaulted is:
+Where `command_object` is a `json` string object. The minimal object, where all parameters are defaulted is:
 ```json
 {
     "command": "some bash command"
 }
 ```
 
  with the following properties (the first option mentioned is the default)
 ```javascript
 {
     "command": "ls -lt",
     "print_command": false/true             // print the command in the document
-    "output-format": "bash"/code block id   // Any value supported by md code blocks (e.g. json, python, etc.)
+    "output-format": "bash"/code block id   // Any value supported by md code blocks (e.g. json, python, etc.) using markdown with write the output not as a code block
     "limit": 0/any number                   // limit the number of lines printed
     "error-strategy": "ignore"\"exit",      // Behavior on error
     "skip": false/true,                     // If true, this command is not run. If true, it is run, and if the following block is an output (of a previous command), it is updated.
-     "object-type": N/A                     // Used internally by markcli to mark output blocks
+     "object-type": N/A                     // Used internally by `markcli` to mark output blocks
 }
 ```
 
 Example: running the previous will result in:
 
 <!--
 {
@@ -40,20 +40,21 @@
 }
 -->
 <!-- { "object-type": "command-output-start" } -->
 ```bash
 ls -lt
 ```
 ```bash
-total 24
--rw-r--r-- 1 runner docker     0 May  7 06:18 README.md
--rw-r--r-- 1 runner docker 11357 May  7 06:18 LICENSE
-drwxr-xr-x 2 runner docker  4096 May  7 06:18 markcli
--rw-r--r-- 1 runner docker  1065 May  7 06:18 setup.py
--rw-r--r-- 1 runner docker  3036 May  7 06:18 template.md
+total 28
+-rw-r--r-- 1 runner docker     0 May  8 06:36 README.md
+-rw-r--r-- 1 runner docker 11357 May  8 06:36 LICENSE
+-rw-r--r-- 1 runner docker   121 May  8 06:36 installation.md
+drwxr-xr-x 2 runner docker  4096 May  8 06:36 markcli
+-rw-r--r-- 1 runner docker  1065 May  8 06:36 setup.py
+-rw-r--r-- 1 runner docker  3064 May  8 06:36 template.md
 ```
 <!-- { "object-type": "command-output-end" } -->
 
 
 Commands can use environment variables, the parser assumes that any capitalized word is an environment variable. Example:
 <!--
 {
@@ -114,22 +115,31 @@
     parser = jsonargparse.ArgumentParser(
         description="A command line tool for generating templated documentation from clis",
     )
 ```
 <!-- { "object-type": "command-output-end" } -->
 
 
+<!--
+{
+    "command": "cat installation.md",
+    "output-format": "markdown"
+}
+-->
+<!-- { "object-type": "command-output-start" } -->
 # Installation
 
-To install markcli, run:
+To install `markcli`, run:
 ```bash
 pip install markcli
 ```
 
 Then the command `markcli` will be available.
+<!-- { "object-type": "command-output-end" } -->
+
 
 # A real-world example: document the valint command:
 <!--
 Some other commented text
 -->
 ## Install valint
 To install valint run (Note that the -- 2>&1 is required to capture the output in this setting, but is not required in a normal shell):
@@ -149,17 +159,18 @@
 scribe info Trying to download, tool=valint, version=latest
 scribe info Using dev artifacts, subpath='dev/valint/linux/amd64', ENV=dev
 scribe info Downloading, Version=1.4.0-6
   % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                  Dload  Upload   Total   Spent    Left  Speed
 
   0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0
-  0 28.5M    0 34028    0     0  75650      0  0:06:36 --:--:--  0:06:36 75617
- 69 28.5M   69 19.9M    0     0  14.1M      0  0:00:02  0:00:01  0:00:01 14.1M
-100 28.5M  100 28.5M    0     0  17.0M      0  0:00:01  0:00:01 --:--:-- 17.0M
+  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0
+
+  0 28.5M    0 17735    0     0  40073      0  0:12:27 --:--:--  0:12:27 40073
+100 28.5M  100 28.5M    0     0  40.8M      0 --:--:-- --:--:-- --:--:--  111M
 scribe info Installed /home/runner/.scribe/bin/valint
 
 ```
 <!-- { "object-type": "command-output-end" } -->
 
 
 ## General options
```

### Comparing `markcli-0.1.3/markcli/markcli.py` & `markcli-0.1.4/markcli/markcli.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,14 +32,15 @@
     else:
         exit(1)
 
 def create_doc(dargs):
     # Read input file to string
     template_filename = dargs["input"]
     output_filename = dargs["output"]
+    print(f"Creating documentation from {template_filename} to {output_filename}")
     same_file = False
     if template_filename == output_filename:
         same_file = True
         orig_output_filename = output_filename
         output_filename = f"tmp-{output_filename}"
     with open(template_filename, "r") as f:
         template = f.read()
@@ -79,26 +80,30 @@
         if object_type == "command":
             remove_previous = False
             skip = command_obj.get("skip", False)
             if skip:
                 o.write(f'<!--\n{command}\n-->\n')
                 continue
 
+            print(f"Running command: {command_obj['command']}")
             output = run_command(command_obj)
             # Handle printing:
             # Retain original object in order to allow for re runs and debugging:
             o.write(f'<!--\n{command}\n-->\n') 
             o.write('<!-- { "object-type": "command-output-start" } -->\n')
             if command_obj.get("print_command", False):
                 o.write(f"```bash\n{command_obj['command']}\n```\n")
             format = command_obj.get("output-format", 'bash')
             limit = command_obj.get("limit", 0)
             if limit > 0:
                 output = '\n'.join(output.split('\n')[:limit]) + '\n'
-            o.write(f"```{format}\n{output}```\n")
+            if format == 'markdown':
+                o.write(f"{output}\n")
+            else:
+                o.write(f"```{format}\n{output}```\n")
             o.write('<!-- { "object-type": "command-output-end" } -->\n')
             o.write(tail)
             remove_previous = True
         elif object_type == "command-output-start":
             if remove_previous:
                 continue
             else:
```

### Comparing `markcli-0.1.3/markcli.egg-info/PKG-INFO` & `markcli-0.1.4/markcli.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: markcli
-Version: 0.1.3
+Version: 0.1.4
 Summary: A Jupyter-inspired tool to create documentation of CLI tools.
 Home-page: UNKNOWN
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -14,41 +14,41 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # `markcli` - An Jupyter-inspired CLI Documentation Tool
 
 ## Description
-Run markcli to fill a template that results from running the cli command included inside.
+Run `markcli` to fill a template that results from running the cli command included inside.
 
-CLI commands are written in html comments (here with spaces added to avoid rendering) using the following syntax:
+CLI commands are written in `html` comments (here with spaces added to avoid rendering) using the following syntax:
 
 ```
 < ! - - 
 command_object
 - ->
 ```
 
-Where `command_object` is a json string object. The minimal object, where all parameters are defaulted is:
+Where `command_object` is a `json` string object. The minimal object, where all parameters are defaulted is:
 ```json
 {
     "command": "some bash command"
 }
 ```
 
  with the following properties (the first option mentioned is the default)
 ```javascript
 {
     "command": "ls -lt",
     "print_command": false/true             // print the command in the document
-    "output-format": "bash"/code block id   // Any value supported by md code blocks (e.g. json, python, etc.)
+    "output-format": "bash"/code block id   // Any value supported by md code blocks (e.g. json, python, etc.) using markdown with write the output not as a code block
     "limit": 0/any number                   // limit the number of lines printed
     "error-strategy": "ignore"\"exit",      // Behavior on error
     "skip": false/true,                     // If true, this command is not run. If true, it is run, and if the following block is an output (of a previous command), it is updated.
-     "object-type": N/A                     // Used internally by markcli to mark output blocks
+     "object-type": N/A                     // Used internally by `markcli` to mark output blocks
 }
 ```
 
 Example: running the previous will result in:
 
 <!--
 {
@@ -57,20 +57,21 @@
 }
 -->
 <!-- { "object-type": "command-output-start" } -->
 ```bash
 ls -lt
 ```
 ```bash
-total 24
--rw-r--r-- 1 runner docker     0 May  7 06:18 README.md
--rw-r--r-- 1 runner docker 11357 May  7 06:18 LICENSE
-drwxr-xr-x 2 runner docker  4096 May  7 06:18 markcli
--rw-r--r-- 1 runner docker  1065 May  7 06:18 setup.py
--rw-r--r-- 1 runner docker  3036 May  7 06:18 template.md
+total 28
+-rw-r--r-- 1 runner docker     0 May  8 06:36 README.md
+-rw-r--r-- 1 runner docker 11357 May  8 06:36 LICENSE
+-rw-r--r-- 1 runner docker   121 May  8 06:36 installation.md
+drwxr-xr-x 2 runner docker  4096 May  8 06:36 markcli
+-rw-r--r-- 1 runner docker  1065 May  8 06:36 setup.py
+-rw-r--r-- 1 runner docker  3064 May  8 06:36 template.md
 ```
 <!-- { "object-type": "command-output-end" } -->
 
 
 Commands can use environment variables, the parser assumes that any capitalized word is an environment variable. Example:
 <!--
 {
@@ -131,22 +132,31 @@
     parser = jsonargparse.ArgumentParser(
         description="A command line tool for generating templated documentation from clis",
     )
 ```
 <!-- { "object-type": "command-output-end" } -->
 
 
+<!--
+{
+    "command": "cat installation.md",
+    "output-format": "markdown"
+}
+-->
+<!-- { "object-type": "command-output-start" } -->
 # Installation
 
-To install markcli, run:
+To install `markcli`, run:
 ```bash
 pip install markcli
 ```
 
 Then the command `markcli` will be available.
+<!-- { "object-type": "command-output-end" } -->
+
 
 # A real-world example: document the valint command:
 <!--
 Some other commented text
 -->
 ## Install valint
 To install valint run (Note that the -- 2>&1 is required to capture the output in this setting, but is not required in a normal shell):
@@ -166,17 +176,18 @@
 scribe info Trying to download, tool=valint, version=latest
 scribe info Using dev artifacts, subpath='dev/valint/linux/amd64', ENV=dev
 scribe info Downloading, Version=1.4.0-6
   % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                  Dload  Upload   Total   Spent    Left  Speed
 
   0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0
-  0 28.5M    0 34028    0     0  75650      0  0:06:36 --:--:--  0:06:36 75617
- 69 28.5M   69 19.9M    0     0  14.1M      0  0:00:02  0:00:01  0:00:01 14.1M
-100 28.5M  100 28.5M    0     0  17.0M      0  0:00:01  0:00:01 --:--:-- 17.0M
+  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0
+
+  0 28.5M    0 17735    0     0  40073      0  0:12:27 --:--:--  0:12:27 40073
+100 28.5M  100 28.5M    0     0  40.8M      0 --:--:-- --:--:-- --:--:--  111M
 scribe info Installed /home/runner/.scribe/bin/valint
 
 ```
 <!-- { "object-type": "command-output-end" } -->
 
 
 ## General options
```

### Comparing `markcli-0.1.3/setup.py` & `markcli-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md") as readme:
         description = readme.read()
 
 setup(
     name='markcli',
-    version='0.1.3',
+    version='0.1.4',
     packages=find_packages(),
     install_requires=[
         'jsonargparse',
     ],
     python_requires='>=3.8',
     description="A Jupyter-inspired tool to create documentation of CLI tools.",
     license='Apache License 2.0',
```

