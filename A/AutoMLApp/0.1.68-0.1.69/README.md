# Comparing `tmp/automlapp-0.1.68.tar.gz` & `tmp/automlapp-0.1.69.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "automlapp-0.1.68.tar", last modified: Wed May  8 06:00:48 2024, max compression
+gzip compressed data, was "automlapp-0.1.69.tar", last modified: Wed May  8 06:02:34 2024, max compression
```

## Comparing `automlapp-0.1.68.tar` & `automlapp-0.1.69.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 06:00:48.756996 automlapp-0.1.68/
-drwxrwxrwx   0        0        0        0 2024-05-08 06:00:48.756996 automlapp-0.1.68/AutoMLApp.egg-info/
--rw-rw-rw-   0        0        0     5052 2024-05-08 06:00:48.000000 automlapp-0.1.68/AutoMLApp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      805 2024-05-08 06:00:48.000000 automlapp-0.1.68/AutoMLApp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 06:00:48.000000 automlapp-0.1.68/AutoMLApp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2024-05-08 06:00:48.000000 automlapp-0.1.68/AutoMLApp.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      268 2024-05-08 06:00:48.000000 automlapp-0.1.68/AutoMLApp.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-08 06:00:48.000000 automlapp-0.1.68/AutoMLApp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1088 2024-05-03 11:39:36.000000 automlapp-0.1.68/LICENSE
--rw-rw-rw-   0        0        0     5052 2024-05-08 06:00:48.756996 automlapp-0.1.68/PKG-INFO
--rw-rw-rw-   0        0        0     3993 2024-04-12 09:40:36.000000 automlapp-0.1.68/README.md
-drwxrwxrwx   0        0        0        0 2024-05-08 06:00:48.740795 automlapp-0.1.68/automlapp/
--rw-rw-rw-   0        0        0       44 2024-05-07 10:07:08.000000 automlapp-0.1.68/automlapp/__init__.py
--rw-rw-rw-   0        0        0    60983 2024-05-08 05:51:07.000000 automlapp-0.1.68/automlapp/app.py
--rw-rw-rw-   0        0        0      207 2024-05-08 05:56:14.000000 automlapp-0.1.68/automlapp/launcher.py
--rw-rw-rw-   0        0        0   109179 2024-02-26 11:55:20.000000 automlapp-0.1.68/automlapp/logo.png
-drwxrwxrwx   0        0        0        0 2024-05-08 06:00:48.752757 automlapp-0.1.68/automlapp/modules/
--rw-rw-rw-   0        0        0        0 2024-05-07 11:09:32.000000 automlapp-0.1.68/automlapp/modules/__init__.py
--rw-rw-rw-   0        0        0     5469 2024-05-07 11:23:48.000000 automlapp-0.1.68/automlapp/modules/data_cleaning.py
--rw-rw-rw-   0        0        0     2511 2024-05-07 11:23:57.000000 automlapp-0.1.68/automlapp/modules/data_input.py
--rw-rw-rw-   0        0        0     3332 2024-05-07 11:24:04.000000 automlapp-0.1.68/automlapp/modules/data_preprocessing.py
--rw-rw-rw-   0        0        0     1074 2024-05-07 11:24:45.000000 automlapp-0.1.68/automlapp/modules/data_summarization.py
--rw-rw-rw-   0        0        0     3433 2024-05-07 11:24:56.000000 automlapp-0.1.68/automlapp/modules/data_visualization.py
--rw-rw-rw-   0        0        0     3650 2024-05-07 11:25:02.000000 automlapp-0.1.68/automlapp/modules/data_woeiv.py
--rw-rw-rw-   0        0        0     9481 2024-05-07 11:25:23.000000 automlapp-0.1.68/automlapp/modules/hyperparameter_tuning.py
--rw-rw-rw-   0        0        0    14623 2024-05-07 11:26:02.000000 automlapp-0.1.68/automlapp/modules/model_evaluation.py
--rw-rw-rw-   0        0        0     5534 2024-05-07 11:26:09.000000 automlapp-0.1.68/automlapp/modules/model_training.py
--rw-rw-rw-   0        0        0     6455 2024-05-07 11:29:20.000000 automlapp-0.1.68/automlapp/modules/train_user_params.py
-drwxrwxrwx   0        0        0        0 2024-05-08 06:00:48.756996 automlapp-0.1.68/automlapp/utils/
--rw-rw-rw-   0        0        0        0 2024-05-07 11:09:13.000000 automlapp-0.1.68/automlapp/utils/__init__.py
--rw-rw-rw-   0        0        0      199 2024-05-07 11:32:57.000000 automlapp-0.1.68/automlapp/utils/print_utils.py
--rw-rw-rw-   0        0        0      857 2024-05-07 11:32:56.000000 automlapp-0.1.68/automlapp/utils/streamlit_utils.py
--rw-rw-rw-   0        0        0       42 2024-05-08 06:00:48.756996 automlapp-0.1.68/setup.cfg
--rw-rw-rw-   0        0        0     1513 2024-05-08 06:00:44.000000 automlapp-0.1.68/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 06:02:34.204736 automlapp-0.1.69/
+drwxrwxrwx   0        0        0        0 2024-05-08 06:02:34.201790 automlapp-0.1.69/AutoMLApp.egg-info/
+-rw-rw-rw-   0        0        0     5052 2024-05-08 06:02:34.000000 automlapp-0.1.69/AutoMLApp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      805 2024-05-08 06:02:34.000000 automlapp-0.1.69/AutoMLApp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 06:02:34.000000 automlapp-0.1.69/AutoMLApp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2024-05-08 06:02:34.000000 automlapp-0.1.69/AutoMLApp.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      268 2024-05-08 06:02:34.000000 automlapp-0.1.69/AutoMLApp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-08 06:02:34.000000 automlapp-0.1.69/AutoMLApp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1088 2024-05-03 11:39:36.000000 automlapp-0.1.69/LICENSE
+-rw-rw-rw-   0        0        0     5052 2024-05-08 06:02:34.202788 automlapp-0.1.69/PKG-INFO
+-rw-rw-rw-   0        0        0     3993 2024-04-12 09:40:36.000000 automlapp-0.1.69/README.md
+drwxrwxrwx   0        0        0        0 2024-05-08 06:02:34.183619 automlapp-0.1.69/automlapp/
+-rw-rw-rw-   0        0        0       44 2024-05-07 10:07:08.000000 automlapp-0.1.69/automlapp/__init__.py
+-rw-rw-rw-   0        0        0    60983 2024-05-08 05:51:07.000000 automlapp-0.1.69/automlapp/app.py
+-rw-rw-rw-   0        0        0      207 2024-05-08 05:56:14.000000 automlapp-0.1.69/automlapp/launcher.py
+-rw-rw-rw-   0        0        0   109179 2024-02-26 11:55:20.000000 automlapp-0.1.69/automlapp/logo.png
+drwxrwxrwx   0        0        0        0 2024-05-08 06:02:34.196962 automlapp-0.1.69/automlapp/modules/
+-rw-rw-rw-   0        0        0        0 2024-05-07 11:09:32.000000 automlapp-0.1.69/automlapp/modules/__init__.py
+-rw-rw-rw-   0        0        0     5469 2024-05-07 11:23:48.000000 automlapp-0.1.69/automlapp/modules/data_cleaning.py
+-rw-rw-rw-   0        0        0     2511 2024-05-07 11:23:57.000000 automlapp-0.1.69/automlapp/modules/data_input.py
+-rw-rw-rw-   0        0        0     3332 2024-05-07 11:24:04.000000 automlapp-0.1.69/automlapp/modules/data_preprocessing.py
+-rw-rw-rw-   0        0        0     1074 2024-05-07 11:24:45.000000 automlapp-0.1.69/automlapp/modules/data_summarization.py
+-rw-rw-rw-   0        0        0     3433 2024-05-07 11:24:56.000000 automlapp-0.1.69/automlapp/modules/data_visualization.py
+-rw-rw-rw-   0        0        0     3650 2024-05-07 11:25:02.000000 automlapp-0.1.69/automlapp/modules/data_woeiv.py
+-rw-rw-rw-   0        0        0     9481 2024-05-07 11:25:23.000000 automlapp-0.1.69/automlapp/modules/hyperparameter_tuning.py
+-rw-rw-rw-   0        0        0    14623 2024-05-07 11:26:02.000000 automlapp-0.1.69/automlapp/modules/model_evaluation.py
+-rw-rw-rw-   0        0        0     5534 2024-05-07 11:26:09.000000 automlapp-0.1.69/automlapp/modules/model_training.py
+-rw-rw-rw-   0        0        0     6455 2024-05-07 11:29:20.000000 automlapp-0.1.69/automlapp/modules/train_user_params.py
+drwxrwxrwx   0        0        0        0 2024-05-08 06:02:34.200792 automlapp-0.1.69/automlapp/utils/
+-rw-rw-rw-   0        0        0        0 2024-05-07 11:09:13.000000 automlapp-0.1.69/automlapp/utils/__init__.py
+-rw-rw-rw-   0        0        0      199 2024-05-07 11:32:57.000000 automlapp-0.1.69/automlapp/utils/print_utils.py
+-rw-rw-rw-   0        0        0      857 2024-05-07 11:32:56.000000 automlapp-0.1.69/automlapp/utils/streamlit_utils.py
+-rw-rw-rw-   0        0        0       42 2024-05-08 06:02:34.204736 automlapp-0.1.69/setup.cfg
+-rw-rw-rw-   0        0        0     1512 2024-05-08 06:02:28.000000 automlapp-0.1.69/setup.py
```

### Comparing `automlapp-0.1.68/AutoMLApp.egg-info/PKG-INFO` & `automlapp-0.1.69/AutoMLApp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AutoMLApp
-Version: 0.1.68
+Version: 0.1.69
 Summary: An automated machine learning application designed for efficient model training, evaluation, and hyperparameter tuning.
 Author: Shivam Nikam
 Author-email: shivam.nikam@think360.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `automlapp-0.1.68/AutoMLApp.egg-info/SOURCES.txt` & `automlapp-0.1.69/AutoMLApp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `automlapp-0.1.68/LICENSE` & `automlapp-0.1.69/LICENSE`

 * *Files identical despite different names*

### Comparing `automlapp-0.1.68/PKG-INFO` & `automlapp-0.1.69/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AutoMLApp
-Version: 0.1.68
+Version: 0.1.69
 Summary: An automated machine learning application designed for efficient model training, evaluation, and hyperparameter tuning.
 Author: Shivam Nikam
 Author-email: shivam.nikam@think360.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `automlapp-0.1.68/README.md` & `automlapp-0.1.69/README.md`

 * *Files identical despite different names*

### Comparing `automlapp-0.1.68/automlapp/app.py` & `automlapp-0.1.69/automlapp/app.py`

 * *Files identical despite different names*

### Comparing `automlapp-0.1.68/automlapp/logo.png` & `automlapp-0.1.69/automlapp/logo.png`

 * *Files identical despite different names*

### Comparing `automlapp-0.1.68/automlapp/modules/data_cleaning.py` & `automlapp-0.1.69/automlapp/modules/data_cleaning.py`

 * *Files identical despite different names*

### Comparing `automlapp-0.1.68/automlapp/modules/data_input.py` & `automlapp-0.1.69/automlapp/modules/data_input.py`

 * *Files identical despite different names*

### Comparing `automlapp-0.1.68/automlapp/modules/data_preprocessing.py` & `automlapp-0.1.69/automlapp/modules/data_preprocessing.py`

 * *Files identical despite different names*

### Comparing `automlapp-0.1.68/automlapp/modules/data_summarization.py` & `automlapp-0.1.69/automlapp/modules/data_summarization.py`

 * *Files identical despite different names*

### Comparing `automlapp-0.1.68/automlapp/modules/data_visualization.py` & `automlapp-0.1.69/automlapp/modules/data_visualization.py`

 * *Files identical despite different names*

### Comparing `automlapp-0.1.68/automlapp/modules/data_woeiv.py` & `automlapp-0.1.69/automlapp/modules/data_woeiv.py`

 * *Files identical despite different names*

### Comparing `automlapp-0.1.68/automlapp/modules/hyperparameter_tuning.py` & `automlapp-0.1.69/automlapp/modules/hyperparameter_tuning.py`

 * *Files identical despite different names*

### Comparing `automlapp-0.1.68/automlapp/modules/model_evaluation.py` & `automlapp-0.1.69/automlapp/modules/model_evaluation.py`

 * *Files identical despite different names*

### Comparing `automlapp-0.1.68/automlapp/modules/model_training.py` & `automlapp-0.1.69/automlapp/modules/model_training.py`

 * *Files identical despite different names*

### Comparing `automlapp-0.1.68/automlapp/modules/train_user_params.py` & `automlapp-0.1.69/automlapp/modules/train_user_params.py`

 * *Files identical despite different names*

### Comparing `automlapp-0.1.68/automlapp/utils/streamlit_utils.py` & `automlapp-0.1.69/automlapp/utils/streamlit_utils.py`

 * *Files identical despite different names*

### Comparing `automlapp-0.1.68/setup.py` & `automlapp-0.1.69/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="AutoMLApp",
-    version="0.1.68",
+    version="0.1.69",
     author="Shivam Nikam",
     author_email="shivam.nikam@think360.ai",
     description="An automated machine learning application designed for efficient model training, evaluation, and hyperparameter tuning.",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     #url="https://github.com/YourGithub/AutoMLApp",
     packages=find_packages(),
@@ -38,11 +38,11 @@
         ],
     },
     package_data={
         'automlapp': ['logo.png'],  # Specify relative path to package root
     },
     entry_points={
         "console_scripts": [
-            "run_tool=automlapp.launcher:main",
+            "runtool=automlapp.launcher:main",
         ],
     }
 )
```

