# Comparing `tmp/mibanco_auto_web-1.0.0.tar.gz` & `tmp/mibanco_auto_web-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mibanco_auto_web-1.0.0.tar", last modified: Mon May  6 17:23:54 2024, max compression
+gzip compressed data, was "mibanco_auto_web-1.0.1.tar", last modified: Wed May  8 21:22:17 2024, max compression
```

## Comparing `mibanco_auto_web-1.0.0.tar` & `mibanco_auto_web-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 17:23:54.927904 mibanco_auto_web-1.0.0/
--rw-rw-rw-   0        0        0       46 2024-04-30 04:05:30.000000 mibanco_auto_web-1.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     3180 2024-05-06 17:23:54.924330 mibanco_auto_web-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     2231 2024-05-06 17:12:14.000000 mibanco_auto_web-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-06 17:23:54.870313 mibanco_auto_web-1.0.0/mibanco_auto_web/
--rw-rw-rw-   0        0        0       63 2024-04-29 20:52:26.000000 mibanco_auto_web-1.0.0/mibanco_auto_web/__init__.py
--rw-rw-rw-   0        0        0     4315 2024-05-02 21:27:42.000000 mibanco_auto_web-1.0.0/mibanco_auto_web/functions.py
--rw-rw-rw-   0        0        0     1686 2024-05-02 20:47:00.000000 mibanco_auto_web-1.0.0/mibanco_auto_web/main.py
--rw-rw-rw-   0        0        0      102 2024-05-06 17:14:00.000000 mibanco_auto_web-1.0.0/mibanco_auto_web/variables.py
-drwxrwxrwx   0        0        0        0 2024-05-06 17:23:54.921323 mibanco_auto_web-1.0.0/mibanco_auto_web.egg-info/
--rw-rw-rw-   0        0        0     3180 2024-05-06 17:23:54.000000 mibanco_auto_web-1.0.0/mibanco_auto_web.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      386 2024-05-06 17:23:54.000000 mibanco_auto_web-1.0.0/mibanco_auto_web.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 17:23:54.000000 mibanco_auto_web-1.0.0/mibanco_auto_web.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       64 2024-05-06 17:23:54.000000 mibanco_auto_web-1.0.0/mibanco_auto_web.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      286 2024-05-06 17:23:54.000000 mibanco_auto_web-1.0.0/mibanco_auto_web.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-05-06 17:23:54.000000 mibanco_auto_web-1.0.0/mibanco_auto_web.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-06 17:23:54.927904 mibanco_auto_web-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1495 2024-05-06 17:23:41.000000 mibanco_auto_web-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 21:22:17.014733 mibanco_auto_web-1.0.1/
+-rw-rw-rw-   0        0        0       46 2024-04-30 04:05:30.000000 mibanco_auto_web-1.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     3256 2024-05-08 21:22:17.008476 mibanco_auto_web-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2231 2024-05-06 17:12:14.000000 mibanco_auto_web-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-08 21:22:16.906823 mibanco_auto_web-1.0.1/mibanco_auto_web/
+-rw-rw-rw-   0        0        0       63 2024-04-29 20:52:26.000000 mibanco_auto_web-1.0.1/mibanco_auto_web/__init__.py
+-rw-rw-rw-   0        0        0     4346 2024-05-08 21:17:28.000000 mibanco_auto_web-1.0.1/mibanco_auto_web/functions.py
+-rw-rw-rw-   0        0        0     1686 2024-05-02 20:47:00.000000 mibanco_auto_web-1.0.1/mibanco_auto_web/main.py
+-rw-rw-rw-   0        0        0      102 2024-05-08 21:16:35.000000 mibanco_auto_web-1.0.1/mibanco_auto_web/variables.py
+drwxrwxrwx   0        0        0        0 2024-05-08 21:22:17.003342 mibanco_auto_web-1.0.1/mibanco_auto_web.egg-info/
+-rw-rw-rw-   0        0        0     3256 2024-05-08 21:22:15.000000 mibanco_auto_web-1.0.1/mibanco_auto_web.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      386 2024-05-08 21:22:15.000000 mibanco_auto_web-1.0.1/mibanco_auto_web.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 21:22:15.000000 mibanco_auto_web-1.0.1/mibanco_auto_web.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       64 2024-05-08 21:22:15.000000 mibanco_auto_web-1.0.1/mibanco_auto_web.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      322 2024-05-08 21:22:15.000000 mibanco_auto_web-1.0.1/mibanco_auto_web.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-05-08 21:22:15.000000 mibanco_auto_web-1.0.1/mibanco_auto_web.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-08 21:22:17.014733 mibanco_auto_web-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1563 2024-05-08 21:16:24.000000 mibanco_auto_web-1.0.1/setup.py
```

### Comparing `mibanco_auto_web-1.0.0/PKG-INFO` & `mibanco_auto_web-1.0.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 Metadata-Version: 2.1
 Name: mibanco_auto_web
-Version: 1.0.0
+Version: 1.0.1
 Summary: A simple functional test library using Python and Selenium
 Author: Linda Lopez
 Keywords: selenium,testing,web,chrome
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 Requires-Dist: allure-behave==2.13.5
 Requires-Dist: allure-python-commons==2.13.5
 Requires-Dist: behave==1.2.6
 Requires-Dist: behave-html-formatter==0.9.10
 Requires-Dist: behave2cucumber==1.0.3
 Requires-Dist: docxcompose==1.4.0
 Requires-Dist: docxtpl==0.16.8
 Requires-Dist: playwright==1.42.0
 Requires-Dist: psutil==5.9.2
+Requires-Dist: pillow==10.3.0
+Requires-Dist: customtkinter==5.2.2
 Requires-Dist: PyPDF2==3.0.1
 Requires-Dist: python-docx==1.1.0
 Requires-Dist: pycparser==2.21
 Requires-Dist: screeninfo==0.8
 Requires-Dist: selenium==4.20.0
 Requires-Dist: keyboard==0.13.5
```

### Comparing `mibanco_auto_web-1.0.0/README.md` & `mibanco_auto_web-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `mibanco_auto_web-1.0.0/mibanco_auto_web/functions.py` & `mibanco_auto_web-1.0.1/mibanco_auto_web/functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,15 @@
     if repository_type == "Github":
         repository_name = select_repository_name()
         branch_name = select_brach_name()
         url_repository = f"https://github.com/aariverar/{repository_name}.git"
     elif repository_type == "Azure Repos":
         repository_name = select_repository_name()
         branch_name = select_brach_name()
-        url_repository = f"https://github.com/aariverar/{repository_name}.git"
+        url_repository = f"https://mibanco-devops@dev.azure.com/mibanco-devops/DevOps/_git/{repository_name}"
     else: 
         url_repository = None
 
     if url_repository is not None:
         # Verificar si la rama existe en el repositorio remoto
         result = subprocess.run(f'git ls-remote --heads {url_repository} {branch_name}', shell=True, capture_output=True, text=True)
         if branch_name in result.stdout:
```

### Comparing `mibanco_auto_web-1.0.0/mibanco_auto_web/main.py` & `mibanco_auto_web-1.0.1/mibanco_auto_web/main.py`

 * *Files identical despite different names*

### Comparing `mibanco_auto_web-1.0.0/mibanco_auto_web.egg-info/PKG-INFO` & `mibanco_auto_web-1.0.1/mibanco_auto_web.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 Metadata-Version: 2.1
 Name: mibanco_auto_web
-Version: 1.0.0
+Version: 1.0.1
 Summary: A simple functional test library using Python and Selenium
 Author: Linda Lopez
 Keywords: selenium,testing,web,chrome
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 Requires-Dist: allure-behave==2.13.5
 Requires-Dist: allure-python-commons==2.13.5
 Requires-Dist: behave==1.2.6
 Requires-Dist: behave-html-formatter==0.9.10
 Requires-Dist: behave2cucumber==1.0.3
 Requires-Dist: docxcompose==1.4.0
 Requires-Dist: docxtpl==0.16.8
 Requires-Dist: playwright==1.42.0
 Requires-Dist: psutil==5.9.2
+Requires-Dist: pillow==10.3.0
+Requires-Dist: customtkinter==5.2.2
 Requires-Dist: PyPDF2==3.0.1
 Requires-Dist: python-docx==1.1.0
 Requires-Dist: pycparser==2.21
 Requires-Dist: screeninfo==0.8
 Requires-Dist: selenium==4.20.0
 Requires-Dist: keyboard==0.13.5
```

### Comparing `mibanco_auto_web-1.0.0/setup.py` & `mibanco_auto_web-1.0.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,16 @@
         "behave==1.2.6",
         "behave-html-formatter==0.9.10",
         "behave2cucumber==1.0.3",
         "docxcompose==1.4.0",
         "docxtpl==0.16.8",
         "playwright==1.42.0",
         "psutil==5.9.2",
+        "pillow==10.3.0",
+        "customtkinter==5.2.2",
         "PyPDF2==3.0.1",
         "python-docx==1.1.0",
         "pycparser==2.21",
         "screeninfo==0.8",
         "selenium==4.20.0",
         "keyboard==0.13.5"
     ],
@@ -34,13 +36,13 @@
             'mibanco_auto_web=mibanco_auto_web.main:main',
         ],
     },
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
-        'Programming Language :: Python',
+        'Programming Language :: Python :: 3.12',
     ],
     keywords=['selenium', 'testing', 'web', 'chrome'],
     long_description=long_description,
     long_description_content_type="text/markdown",
 )
```

