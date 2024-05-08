# Comparing `tmp/automlapp-0.1.65.tar.gz` & `tmp/automlapp-0.1.66.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "automlapp-0.1.65.tar", last modified: Tue May  7 12:02:55 2024, max compression
+gzip compressed data, was "automlapp-0.1.66.tar", last modified: Wed May  8 05:53:25 2024, max compression
```

## Comparing `automlapp-0.1.65.tar` & `automlapp-0.1.66.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 12:02:55.052802 automlapp-0.1.65/
-drwxrwxrwx   0        0        0        0 2024-05-07 12:02:55.045553 automlapp-0.1.65/AutoMLApp.egg-info/
--rw-rw-rw-   0        0        0     5052 2024-05-07 12:02:54.000000 automlapp-0.1.65/AutoMLApp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      805 2024-05-07 12:02:54.000000 automlapp-0.1.65/AutoMLApp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 12:02:54.000000 automlapp-0.1.65/AutoMLApp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       69 2024-05-07 12:02:54.000000 automlapp-0.1.65/AutoMLApp.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      268 2024-05-07 12:02:54.000000 automlapp-0.1.65/AutoMLApp.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-07 12:02:54.000000 automlapp-0.1.65/AutoMLApp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1088 2024-05-03 11:39:36.000000 automlapp-0.1.65/LICENSE
--rw-rw-rw-   0        0        0     5052 2024-05-07 12:02:55.045553 automlapp-0.1.65/PKG-INFO
--rw-rw-rw-   0        0        0     3993 2024-04-12 09:40:36.000000 automlapp-0.1.65/README.md
-drwxrwxrwx   0        0        0        0 2024-05-07 12:02:55.021369 automlapp-0.1.65/automlapp/
--rw-rw-rw-   0        0        0       44 2024-05-07 10:07:08.000000 automlapp-0.1.65/automlapp/__init__.py
--rw-rw-rw-   0        0        0    61023 2024-05-07 11:44:25.000000 automlapp-0.1.65/automlapp/app.py
--rw-rw-rw-   0        0        0      469 2024-05-07 12:02:01.000000 automlapp-0.1.65/automlapp/launcher.py
--rw-rw-rw-   0        0        0   109179 2024-02-26 11:55:20.000000 automlapp-0.1.65/automlapp/logo.png
-drwxrwxrwx   0        0        0        0 2024-05-07 12:02:55.040903 automlapp-0.1.65/automlapp/modules/
--rw-rw-rw-   0        0        0        0 2024-05-07 11:09:32.000000 automlapp-0.1.65/automlapp/modules/__init__.py
--rw-rw-rw-   0        0        0     5469 2024-05-07 11:23:48.000000 automlapp-0.1.65/automlapp/modules/data_cleaning.py
--rw-rw-rw-   0        0        0     2511 2024-05-07 11:23:57.000000 automlapp-0.1.65/automlapp/modules/data_input.py
--rw-rw-rw-   0        0        0     3332 2024-05-07 11:24:04.000000 automlapp-0.1.65/automlapp/modules/data_preprocessing.py
--rw-rw-rw-   0        0        0     1074 2024-05-07 11:24:45.000000 automlapp-0.1.65/automlapp/modules/data_summarization.py
--rw-rw-rw-   0        0        0     3433 2024-05-07 11:24:56.000000 automlapp-0.1.65/automlapp/modules/data_visualization.py
--rw-rw-rw-   0        0        0     3650 2024-05-07 11:25:02.000000 automlapp-0.1.65/automlapp/modules/data_woeiv.py
--rw-rw-rw-   0        0        0     9481 2024-05-07 11:25:23.000000 automlapp-0.1.65/automlapp/modules/hyperparameter_tuning.py
--rw-rw-rw-   0        0        0    14623 2024-05-07 11:26:02.000000 automlapp-0.1.65/automlapp/modules/model_evaluation.py
--rw-rw-rw-   0        0        0     5534 2024-05-07 11:26:09.000000 automlapp-0.1.65/automlapp/modules/model_training.py
--rw-rw-rw-   0        0        0     6455 2024-05-07 11:29:20.000000 automlapp-0.1.65/automlapp/modules/train_user_params.py
-drwxrwxrwx   0        0        0        0 2024-05-07 12:02:55.045553 automlapp-0.1.65/automlapp/utils/
--rw-rw-rw-   0        0        0        0 2024-05-07 11:09:13.000000 automlapp-0.1.65/automlapp/utils/__init__.py
--rw-rw-rw-   0        0        0      199 2024-05-07 11:32:57.000000 automlapp-0.1.65/automlapp/utils/print_utils.py
--rw-rw-rw-   0        0        0      857 2024-05-07 11:32:56.000000 automlapp-0.1.65/automlapp/utils/streamlit_utils.py
--rw-rw-rw-   0        0        0       42 2024-05-07 12:02:55.052802 automlapp-0.1.65/setup.cfg
--rw-rw-rw-   0        0        0     1529 2024-05-07 12:02:35.000000 automlapp-0.1.65/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 05:53:25.912598 automlapp-0.1.66/
+drwxrwxrwx   0        0        0        0 2024-05-08 05:53:25.909596 automlapp-0.1.66/AutoMLApp.egg-info/
+-rw-rw-rw-   0        0        0     5052 2024-05-08 05:53:25.000000 automlapp-0.1.66/AutoMLApp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      805 2024-05-08 05:53:25.000000 automlapp-0.1.66/AutoMLApp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 05:53:25.000000 automlapp-0.1.66/AutoMLApp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2024-05-08 05:53:25.000000 automlapp-0.1.66/AutoMLApp.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      268 2024-05-08 05:53:25.000000 automlapp-0.1.66/AutoMLApp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-08 05:53:25.000000 automlapp-0.1.66/AutoMLApp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1088 2024-05-03 11:39:36.000000 automlapp-0.1.66/LICENSE
+-rw-rw-rw-   0        0        0     5052 2024-05-08 05:53:25.911605 automlapp-0.1.66/PKG-INFO
+-rw-rw-rw-   0        0        0     3993 2024-04-12 09:40:36.000000 automlapp-0.1.66/README.md
+drwxrwxrwx   0        0        0        0 2024-05-08 05:53:25.885240 automlapp-0.1.66/automlapp/
+-rw-rw-rw-   0        0        0       44 2024-05-07 10:07:08.000000 automlapp-0.1.66/automlapp/__init__.py
+-rw-rw-rw-   0        0        0    60983 2024-05-08 05:51:07.000000 automlapp-0.1.66/automlapp/app.py
+-rw-rw-rw-   0        0        0      581 2024-05-08 05:49:46.000000 automlapp-0.1.66/automlapp/launcher.py
+-rw-rw-rw-   0        0        0   109179 2024-02-26 11:55:20.000000 automlapp-0.1.66/automlapp/logo.png
+drwxrwxrwx   0        0        0        0 2024-05-08 05:53:25.903029 automlapp-0.1.66/automlapp/modules/
+-rw-rw-rw-   0        0        0        0 2024-05-07 11:09:32.000000 automlapp-0.1.66/automlapp/modules/__init__.py
+-rw-rw-rw-   0        0        0     5469 2024-05-07 11:23:48.000000 automlapp-0.1.66/automlapp/modules/data_cleaning.py
+-rw-rw-rw-   0        0        0     2511 2024-05-07 11:23:57.000000 automlapp-0.1.66/automlapp/modules/data_input.py
+-rw-rw-rw-   0        0        0     3332 2024-05-07 11:24:04.000000 automlapp-0.1.66/automlapp/modules/data_preprocessing.py
+-rw-rw-rw-   0        0        0     1074 2024-05-07 11:24:45.000000 automlapp-0.1.66/automlapp/modules/data_summarization.py
+-rw-rw-rw-   0        0        0     3433 2024-05-07 11:24:56.000000 automlapp-0.1.66/automlapp/modules/data_visualization.py
+-rw-rw-rw-   0        0        0     3650 2024-05-07 11:25:02.000000 automlapp-0.1.66/automlapp/modules/data_woeiv.py
+-rw-rw-rw-   0        0        0     9481 2024-05-07 11:25:23.000000 automlapp-0.1.66/automlapp/modules/hyperparameter_tuning.py
+-rw-rw-rw-   0        0        0    14623 2024-05-07 11:26:02.000000 automlapp-0.1.66/automlapp/modules/model_evaluation.py
+-rw-rw-rw-   0        0        0     5534 2024-05-07 11:26:09.000000 automlapp-0.1.66/automlapp/modules/model_training.py
+-rw-rw-rw-   0        0        0     6455 2024-05-07 11:29:20.000000 automlapp-0.1.66/automlapp/modules/train_user_params.py
+drwxrwxrwx   0        0        0        0 2024-05-08 05:53:25.907596 automlapp-0.1.66/automlapp/utils/
+-rw-rw-rw-   0        0        0        0 2024-05-07 11:09:13.000000 automlapp-0.1.66/automlapp/utils/__init__.py
+-rw-rw-rw-   0        0        0      199 2024-05-07 11:32:57.000000 automlapp-0.1.66/automlapp/utils/print_utils.py
+-rw-rw-rw-   0        0        0      857 2024-05-07 11:32:56.000000 automlapp-0.1.66/automlapp/utils/streamlit_utils.py
+-rw-rw-rw-   0        0        0       42 2024-05-08 05:53:25.912598 automlapp-0.1.66/setup.cfg
+-rw-rw-rw-   0        0        0     1523 2024-05-08 05:53:13.000000 automlapp-0.1.66/setup.py
```

### Comparing `automlapp-0.1.65/AutoMLApp.egg-info/PKG-INFO` & `automlapp-0.1.66/AutoMLApp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AutoMLApp
-Version: 0.1.65
+Version: 0.1.66
 Summary: An automated machine learning application designed for efficient model training, evaluation, and hyperparameter tuning.
 Author: Shivam Nikam
 Author-email: shivam.nikam@think360.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `automlapp-0.1.65/AutoMLApp.egg-info/SOURCES.txt` & `automlapp-0.1.66/AutoMLApp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `automlapp-0.1.65/LICENSE` & `automlapp-0.1.66/LICENSE`

 * *Files identical despite different names*

### Comparing `automlapp-0.1.65/PKG-INFO` & `automlapp-0.1.66/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AutoMLApp
-Version: 0.1.65
+Version: 0.1.66
 Summary: An automated machine learning application designed for efficient model training, evaluation, and hyperparameter tuning.
 Author: Shivam Nikam
 Author-email: shivam.nikam@think360.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `automlapp-0.1.65/README.md` & `automlapp-0.1.66/README.md`

 * *Files identical despite different names*

### Comparing `automlapp-0.1.65/automlapp/app.py` & `automlapp-0.1.66/automlapp/app.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 from .modules.data_visualization import DataVisualization
 from .modules.data_woeiv import DataWOEIV
 from .modules.data_preprocessing import DataPreprocessing
 from .modules.model_training import ModelTraining
 from .modules.model_evaluation import ModelEvaluation
 from .modules.hyperparameter_tuning import HyperparameterTuning
 from .modules.train_user_params import ModelTrainingWithUserParams
-from .launcher import launch_streamlit
 
 warnings.filterwarnings("ignore")
 
 plot_colors = px.colors.sequential.Blues[::-2]
 
 st.set_page_config(layout="wide")
 hide_icons()
```

### Comparing `automlapp-0.1.65/automlapp/logo.png` & `automlapp-0.1.66/automlapp/logo.png`

 * *Files identical despite different names*

### Comparing `automlapp-0.1.65/automlapp/modules/data_cleaning.py` & `automlapp-0.1.66/automlapp/modules/data_cleaning.py`

 * *Files identical despite different names*

### Comparing `automlapp-0.1.65/automlapp/modules/data_input.py` & `automlapp-0.1.66/automlapp/modules/data_input.py`

 * *Files identical despite different names*

### Comparing `automlapp-0.1.65/automlapp/modules/data_preprocessing.py` & `automlapp-0.1.66/automlapp/modules/data_preprocessing.py`

 * *Files identical despite different names*

### Comparing `automlapp-0.1.65/automlapp/modules/data_summarization.py` & `automlapp-0.1.66/automlapp/modules/data_summarization.py`

 * *Files identical despite different names*

### Comparing `automlapp-0.1.65/automlapp/modules/data_visualization.py` & `automlapp-0.1.66/automlapp/modules/data_visualization.py`

 * *Files identical despite different names*

### Comparing `automlapp-0.1.65/automlapp/modules/data_woeiv.py` & `automlapp-0.1.66/automlapp/modules/data_woeiv.py`

 * *Files identical despite different names*

### Comparing `automlapp-0.1.65/automlapp/modules/hyperparameter_tuning.py` & `automlapp-0.1.66/automlapp/modules/hyperparameter_tuning.py`

 * *Files identical despite different names*

### Comparing `automlapp-0.1.65/automlapp/modules/model_evaluation.py` & `automlapp-0.1.66/automlapp/modules/model_evaluation.py`

 * *Files identical despite different names*

### Comparing `automlapp-0.1.65/automlapp/modules/model_training.py` & `automlapp-0.1.66/automlapp/modules/model_training.py`

 * *Files identical despite different names*

### Comparing `automlapp-0.1.65/automlapp/modules/train_user_params.py` & `automlapp-0.1.66/automlapp/modules/train_user_params.py`

 * *Files identical despite different names*

### Comparing `automlapp-0.1.65/automlapp/utils/streamlit_utils.py` & `automlapp-0.1.66/automlapp/utils/streamlit_utils.py`

 * *Files identical despite different names*

### Comparing `automlapp-0.1.65/setup.py` & `automlapp-0.1.66/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="AutoMLApp",
-    version="0.1.65",
+    version="0.1.66",
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
-            "runautomlapp=automlapp.launcher:launch_streamlit",
+            "streamlit_run_tool=automlapp.launcher:main",
         ],
     }
 )
```

