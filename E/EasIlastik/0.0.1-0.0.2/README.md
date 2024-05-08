# Comparing `tmp/EasIlastik-0.0.1.tar.gz` & `tmp/EasIlastik-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EasIlastik-0.0.1.tar", last modified: Thu Apr 11 17:35:24 2024, max compression
+gzip compressed data, was "EasIlastik-0.0.2.tar", last modified: Wed May  8 08:53:08 2024, max compression
```

## Comparing `EasIlastik-0.0.1.tar` & `EasIlastik-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 titouanlegourrierec   (501) staff       (20)        0 2024-04-11 17:35:24.978298 EasIlastik-0.0.1/
-drwxr-xr-x   0 titouanlegourrierec   (501) staff       (20)        0 2024-04-11 17:35:24.976637 EasIlastik-0.0.1/EasIlastik/
--rw-r--r--   0 titouanlegourrierec   (501) staff       (20)        0 2024-04-11 17:19:24.000000 EasIlastik-0.0.1/EasIlastik/__init__.py
--rw-r--r--   0 titouanlegourrierec   (501) staff       (20)     1494 2024-04-11 17:19:25.000000 EasIlastik-0.0.1/EasIlastik/find_ilastik.py
--rw-r--r--   0 titouanlegourrierec   (501) staff       (20)     4260 2024-04-11 17:19:26.000000 EasIlastik-0.0.1/EasIlastik/run_ilastik.py
--rw-r--r--   0 titouanlegourrierec   (501) staff       (20)      447 2024-04-11 17:19:24.000000 EasIlastik-0.0.1/EasIlastik/utils.py
-drwxr-xr-x   0 titouanlegourrierec   (501) staff       (20)        0 2024-04-11 17:35:24.977733 EasIlastik-0.0.1/EasIlastik.egg-info/
--rw-r--r--   0 titouanlegourrierec   (501) staff       (20)      593 2024-04-11 17:35:24.000000 EasIlastik-0.0.1/EasIlastik.egg-info/PKG-INFO
--rw-r--r--   0 titouanlegourrierec   (501) staff       (20)      237 2024-04-11 17:34:44.000000 EasIlastik-0.0.1/EasIlastik.egg-info/README.md
--rw-r--r--   0 titouanlegourrierec   (501) staff       (20)      288 2024-04-11 17:35:24.000000 EasIlastik-0.0.1/EasIlastik.egg-info/SOURCES.txt
--rw-r--r--   0 titouanlegourrierec   (501) staff       (20)        1 2024-04-11 17:35:24.000000 EasIlastik-0.0.1/EasIlastik.egg-info/dependency_links.txt
--rw-r--r--   0 titouanlegourrierec   (501) staff       (20)       11 2024-04-11 17:35:24.000000 EasIlastik-0.0.1/EasIlastik.egg-info/top_level.txt
--rw-r--r--   0 titouanlegourrierec   (501) staff       (20)    35146 2024-04-11 17:15:47.000000 EasIlastik-0.0.1/LICENCE
--rw-r--r--   0 titouanlegourrierec   (501) staff       (20)      593 2024-04-11 17:35:24.978023 EasIlastik-0.0.1/PKG-INFO
--rw-r--r--   0 titouanlegourrierec   (501) staff       (20)       12 2024-04-11 16:06:36.000000 EasIlastik-0.0.1/README.md
--rw-r--r--   0 titouanlegourrierec   (501) staff       (20)       38 2024-04-11 17:35:24.978352 EasIlastik-0.0.1/setup.cfg
--rw-r--r--   0 titouanlegourrierec   (501) staff       (20)      720 2024-04-11 17:19:26.000000 EasIlastik-0.0.1/setup.py
+drwxr-xr-x   0 titouanlegourrierec   (501) staff       (20)        0 2024-05-08 08:53:08.023916 EasIlastik-0.0.2/
+drwxr-xr-x   0 titouanlegourrierec   (501) staff       (20)        0 2024-05-08 08:53:08.022220 EasIlastik-0.0.2/EasIlastik/
+-rw-r--r--   0 titouanlegourrierec   (501) staff       (20)     2027 2024-05-08 08:36:58.000000 EasIlastik-0.0.2/EasIlastik/__init__.py
+-rw-r--r--   0 titouanlegourrierec   (501) staff       (20)     1494 2024-05-08 08:37:02.000000 EasIlastik-0.0.2/EasIlastik/find_ilastik.py
+-rw-r--r--   0 titouanlegourrierec   (501) staff       (20)    17667 2024-05-08 08:37:05.000000 EasIlastik-0.0.2/EasIlastik/run_ilastik.py
+-rw-r--r--   0 titouanlegourrierec   (501) staff       (20)      447 2024-05-08 08:37:09.000000 EasIlastik-0.0.2/EasIlastik/utils.py
+drwxr-xr-x   0 titouanlegourrierec   (501) staff       (20)        0 2024-05-08 08:53:08.023418 EasIlastik-0.0.2/EasIlastik.egg-info/
+-rw-r--r--   0 titouanlegourrierec   (501) staff       (20)      663 2024-05-08 08:53:07.000000 EasIlastik-0.0.2/EasIlastik.egg-info/PKG-INFO
+-rw-r--r--   0 titouanlegourrierec   (501) staff       (20)      237 2024-04-11 17:34:44.000000 EasIlastik-0.0.2/EasIlastik.egg-info/README.md
+-rw-r--r--   0 titouanlegourrierec   (501) staff       (20)      321 2024-05-08 08:53:07.000000 EasIlastik-0.0.2/EasIlastik.egg-info/SOURCES.txt
+-rw-r--r--   0 titouanlegourrierec   (501) staff       (20)        1 2024-05-08 08:53:07.000000 EasIlastik-0.0.2/EasIlastik.egg-info/dependency_links.txt
+-rw-r--r--   0 titouanlegourrierec   (501) staff       (20)       25 2024-05-08 08:53:07.000000 EasIlastik-0.0.2/EasIlastik.egg-info/requires.txt
+-rw-r--r--   0 titouanlegourrierec   (501) staff       (20)       11 2024-05-08 08:53:07.000000 EasIlastik-0.0.2/EasIlastik.egg-info/top_level.txt
+-rw-r--r--   0 titouanlegourrierec   (501) staff       (20)    35146 2024-04-11 17:15:47.000000 EasIlastik-0.0.2/LICENCE
+-rw-r--r--   0 titouanlegourrierec   (501) staff       (20)      663 2024-05-08 08:53:08.023697 EasIlastik-0.0.2/PKG-INFO
+-rw-r--r--   0 titouanlegourrierec   (501) staff       (20)       12 2024-04-11 16:06:36.000000 EasIlastik-0.0.2/README.md
+-rw-r--r--   0 titouanlegourrierec   (501) staff       (20)       38 2024-05-08 08:53:08.023962 EasIlastik-0.0.2/setup.cfg
+-rw-r--r--   0 titouanlegourrierec   (501) staff       (20)      836 2024-05-08 08:40:01.000000 EasIlastik-0.0.2/setup.py
```

### Comparing `EasIlastik-0.0.1/EasIlastik/find_ilastik.py` & `EasIlastik-0.0.2/EasIlastik/find_ilastik.py`

 * *Files identical despite different names*

### Comparing `EasIlastik-0.0.1/EasIlastik.egg-info/PKG-INFO` & `EasIlastik-0.0.2/EasIlastik.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 Metadata-Version: 2.1
 Name: EasIlastik
-Version: 0.0.1
+Version: 0.0.2
 Summary: This package provides seamless integration of pre-trained image segmentation models from Ilastik into Python workflows, empowering users with efficient and intuitive image segmentation capabilities for diverse applications.
 Home-page: https://github.com/titouanlegourrierec/EasIlastik
 Author: Titouan Le Gourrierec
 Author-email: titouanlegourrierec@icloud.com
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 License-File: LICENCE
+Requires-Dist: numpy
+Requires-Dist: h5py
+Requires-Dist: opencv-python
```

### Comparing `EasIlastik-0.0.1/LICENCE` & `EasIlastik-0.0.2/LICENCE`

 * *Files identical despite different names*

### Comparing `EasIlastik-0.0.1/PKG-INFO` & `EasIlastik-0.0.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 Metadata-Version: 2.1
 Name: EasIlastik
-Version: 0.0.1
+Version: 0.0.2
 Summary: This package provides seamless integration of pre-trained image segmentation models from Ilastik into Python workflows, empowering users with efficient and intuitive image segmentation capabilities for diverse applications.
 Home-page: https://github.com/titouanlegourrierec/EasIlastik
 Author: Titouan Le Gourrierec
 Author-email: titouanlegourrierec@icloud.com
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 License-File: LICENCE
+Requires-Dist: numpy
+Requires-Dist: h5py
+Requires-Dist: opencv-python
```

### Comparing `EasIlastik-0.0.1/setup.py` & `EasIlastik-0.0.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,23 @@
 from setuptools import setup, find_packages
 
 setup(
     name='EasIlastik',
-    version='0.0.1',
+    version='0.0.2',
     author='Titouan Le Gourrierec',
     author_email='titouanlegourrierec@icloud.com',
     url='https://github.com/titouanlegourrierec/EasIlastik',
+    README='README.md',
+    CHANGELOG='CHANGELOG.md',
     description='This package provides seamless integration of pre-trained image segmentation models from Ilastik into Python workflows, empowering users with efficient and intuitive image segmentation capabilities for diverse applications.',
     packages=find_packages(),
-    install_requires=[],
+    install_requires=[
+        'numpy',
+        'h5py',
+        'opencv-python'
+    ],
     python_requires='>=3.6',
     classifiers=[
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
         'Programming Language :: Python :: 3',
     ],
 )
```

