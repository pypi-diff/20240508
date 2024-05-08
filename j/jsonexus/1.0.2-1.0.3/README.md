# Comparing `tmp/jsonexus-1.0.2.tar.gz` & `tmp/jsonexus-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsonexus-1.0.2.tar", last modified: Sun Mar 31 18:25:16 2024, max compression
+gzip compressed data, was "jsonexus-1.0.3.tar", last modified: Wed May  8 10:12:18 2024, max compression
```

## Comparing `jsonexus-1.0.2.tar` & `jsonexus-1.0.3.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-03-31 18:25:16.281952 jsonexus-1.0.2/
--rw-rw-rw-   0        0        0     2362 2024-03-31 18:25:16.281952 jsonexus-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1762 2024-03-09 10:32:17.000000 jsonexus-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-03-31 18:25:16.255054 jsonexus-1.0.2/jsonexus/
--rw-rw-rw-   0        0        0    13033 2024-03-31 18:24:09.000000 jsonexus-1.0.2/jsonexus/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-31 18:25:16.279957 jsonexus-1.0.2/jsonexus.egg-info/
--rw-rw-rw-   0        0        0     2362 2024-03-31 18:25:15.000000 jsonexus-1.0.2/jsonexus.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      167 2024-03-31 18:25:15.000000 jsonexus-1.0.2/jsonexus.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-31 18:25:15.000000 jsonexus-1.0.2/jsonexus.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-03-31 18:25:15.000000 jsonexus-1.0.2/jsonexus.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-31 18:25:16.282949 jsonexus-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      879 2024-03-31 18:25:06.000000 jsonexus-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 10:12:18.649678 jsonexus-1.0.3/
+-rw-rw-rw-   0        0        0     2385 2024-05-08 10:12:18.633091 jsonexus-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1762 2024-03-09 10:32:17.000000 jsonexus-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-08 10:12:18.599550 jsonexus-1.0.3/jsonexus/
+-rw-rw-rw-   0        0        0    14854 2024-05-08 09:39:46.000000 jsonexus-1.0.3/jsonexus/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 10:12:18.632090 jsonexus-1.0.3/jsonexus.egg-info/
+-rw-rw-rw-   0        0        0     2385 2024-05-08 10:12:18.000000 jsonexus-1.0.3/jsonexus.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      198 2024-05-08 10:12:18.000000 jsonexus-1.0.3/jsonexus.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 10:12:18.000000 jsonexus-1.0.3/jsonexus.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-05-08 10:12:18.000000 jsonexus-1.0.3/jsonexus.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-08 10:12:18.000000 jsonexus-1.0.3/jsonexus.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-08 10:12:18.649678 jsonexus-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      887 2024-05-08 10:10:45.000000 jsonexus-1.0.3/setup.py
```

### Comparing `jsonexus-1.0.2/PKG-INFO` & `jsonexus-1.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: jsonexus
-Version: 1.0.2
+Version: 1.0.3
 Summary: JSONexus is a lightweight and flexible database solution designed for modern applications. It provides a simple and intuitive way to store, query, and manipulate data using JSON documents.
 Home-page: https://github.com/rakibma7254/jsonexus
 Author: Rakib Hossain
 Author-email: rakib4ggp@gmail.com
 License: MIT
 Keywords: json-database
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/markdown
+Requires-Dist: orjson
 
 JSONexus
 ========
 
 JSONexus is a lightweight and flexible database solution designed for modern applications. It provides a simple and intuitive way to store, query, and manipulate data using JSON documents.
 
 Key Features
```

### Comparing `jsonexus-1.0.2/README.md` & `jsonexus-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `jsonexus-1.0.2/jsonexus.egg-info/PKG-INFO` & `jsonexus-1.0.3/jsonexus.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: jsonexus
-Version: 1.0.2
+Version: 1.0.3
 Summary: JSONexus is a lightweight and flexible database solution designed for modern applications. It provides a simple and intuitive way to store, query, and manipulate data using JSON documents.
 Home-page: https://github.com/rakibma7254/jsonexus
 Author: Rakib Hossain
 Author-email: rakib4ggp@gmail.com
 License: MIT
 Keywords: json-database
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/markdown
+Requires-Dist: orjson
 
 JSONexus
 ========
 
 JSONexus is a lightweight and flexible database solution designed for modern applications. It provides a simple and intuitive way to store, query, and manipulate data using JSON documents.
 
 Key Features
```

### Comparing `jsonexus-1.0.2/setup.py` & `jsonexus-1.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 
 with open("README.md", "r") as fh:
     l_description = fh.read()
 
 
 setup(
     name="jsonexus",
-    version="1.0.2",
+    version="1.0.3",
     packages=find_packages(),
     long_description=l_description,
     long_description_content_type="text/markdown",
     description="JSONexus is a lightweight and flexible database solution designed for modern applications. It provides a simple and intuitive way to store, query, and manipulate data using JSON documents.",
     author="Rakib Hossain",
     author_email="rakib4ggp@gmail.com",
     license="MIT",
     keywords="json-database",
     url="https://github.com/rakibma7254/jsonexus",
-    install_requires=[],
+    install_requires=["orjson"],
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
     ],
 )
```

