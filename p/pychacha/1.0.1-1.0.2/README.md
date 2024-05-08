# Comparing `tmp/pychacha-1.0.1.tar.gz` & `tmp/pychacha-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pychacha-1.0.1.tar", last modified: Wed May  8 16:03:31 2024, max compression
+gzip compressed data, was "pychacha-1.0.2.tar", last modified: Wed May  8 19:52:28 2024, max compression
```

## Comparing `pychacha-1.0.1.tar` & `pychacha-1.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 16:03:31.881389 pychacha-1.0.1/
--rw-rw-rw-   0        0        0    17098 2024-05-08 13:14:07.000000 pychacha-1.0.1/LICENSE
--rw-rw-rw-   0        0        0      482 2024-05-08 16:03:31.877390 pychacha-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      235 2024-05-08 13:57:08.000000 pychacha-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-08 16:03:31.741436 pychacha-1.0.1/pychacha/
--rw-rw-rw-   0        0        0      118 2024-05-08 16:01:09.000000 pychacha-1.0.1/pychacha/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-08 16:03:31.861395 pychacha-1.0.1/pychacha/classes/
--rw-rw-rw-   0        0        0       85 2024-05-08 13:14:07.000000 pychacha-1.0.1/pychacha/classes/__init__.py
--rw-rw-rw-   0        0        0    12232 2024-05-08 13:54:10.000000 pychacha-1.0.1/pychacha/classes/chacha.py
--rw-rw-rw-   0        0        0     4458 2024-05-08 13:14:07.000000 pychacha-1.0.1/pychacha/classes/rsachacha.py
-drwxrwxrwx   0        0        0        0 2024-05-08 16:03:31.875391 pychacha-1.0.1/pychacha.egg-info/
--rw-rw-rw-   0        0        0      482 2024-05-08 16:03:31.000000 pychacha-1.0.1/pychacha.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      261 2024-05-08 16:03:31.000000 pychacha-1.0.1/pychacha.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 16:03:31.000000 pychacha-1.0.1/pychacha.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-08 16:03:31.000000 pychacha-1.0.1/pychacha.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-08 16:03:31.881389 pychacha-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      535 2024-05-08 16:02:54.000000 pychacha-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 19:52:28.377811 pychacha-1.0.2/
+-rw-rw-rw-   0        0        0    17098 2024-05-08 13:14:07.000000 pychacha-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0      482 2024-05-08 19:52:28.375811 pychacha-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      235 2024-05-08 13:57:08.000000 pychacha-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-08 19:52:28.354770 pychacha-1.0.2/pychacha/
+-rw-rw-rw-   0        0        0      118 2024-05-08 16:01:09.000000 pychacha-1.0.2/pychacha/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 19:52:28.371822 pychacha-1.0.2/pychacha/classes/
+-rw-rw-rw-   0        0        0       85 2024-05-08 13:14:07.000000 pychacha-1.0.2/pychacha/classes/__init__.py
+-rw-rw-rw-   0        0        0    12238 2024-05-08 19:50:57.000000 pychacha-1.0.2/pychacha/classes/chacha.py
+-rw-rw-rw-   0        0        0     4458 2024-05-08 13:14:07.000000 pychacha-1.0.2/pychacha/classes/rsachacha.py
+drwxrwxrwx   0        0        0        0 2024-05-08 19:52:28.373822 pychacha-1.0.2/pychacha.egg-info/
+-rw-rw-rw-   0        0        0      482 2024-05-08 19:52:28.000000 pychacha-1.0.2/pychacha.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      261 2024-05-08 19:52:28.000000 pychacha-1.0.2/pychacha.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 19:52:28.000000 pychacha-1.0.2/pychacha.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-08 19:52:28.000000 pychacha-1.0.2/pychacha.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-08 19:52:28.377811 pychacha-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      535 2024-05-08 19:52:21.000000 pychacha-1.0.2/setup.py
```

### Comparing `pychacha-1.0.1/LICENSE` & `pychacha-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pychacha-1.0.1/pychacha/classes/chacha.py` & `pychacha-1.0.2/pychacha/classes/chacha.py`

 * *Files 0% similar despite different names*

```diff
@@ -379,15 +379,15 @@
 
         for root, dirs, files in os.walk(path):
 
             for filename in files:
                 name=os.path.join(root, filename)
                 try:
                     x=self.decrypt_file(name)
-                    print(f"decrypted {name}")
+                    print(f"decrypted {name} - {x}")
                 except PermissionError:
                     print(f"unable to decrypt {name} due to permissions")
                 if not x:
                     return False
         return True
```

### Comparing `pychacha-1.0.1/pychacha/classes/rsachacha.py` & `pychacha-1.0.2/pychacha/classes/rsachacha.py`

 * *Files identical despite different names*

### Comparing `pychacha-1.0.1/setup.py` & `pychacha-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as file:
     readme = file.read()
 
 setuptools.setup(
     name="pychacha",
-    version="1.0.1",
+    version="1.0.2",
     description="ChaCha20 encryption tools for Python.",
     url="https://github.com/thecodeforge/pychacha",
     py_modules=["pychacha"],
     install_requires=[],
     packages=setuptools.find_packages(),
     package_dir={
         "pychacha":"pychacha"
```

