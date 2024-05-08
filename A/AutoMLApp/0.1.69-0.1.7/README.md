# Comparing `tmp/automlapp-0.1.69.tar.gz` & `tmp/automlapp-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "automlapp-0.1.69.tar", last modified: Wed May  8 06:02:34 2024, max compression
+gzip compressed data, was "automlapp-0.1.7.tar", last modified: Wed May  8 06:39:26 2024, max compression
```

## Comparing `automlapp-0.1.69.tar` & `automlapp-0.1.7.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 06:02:34.204736 automlapp-0.1.69/
-drwxrwxrwx   0        0        0        0 2024-05-08 06:02:34.201790 automlapp-0.1.69/AutoMLApp.egg-info/
--rw-rw-rw-   0        0        0     5052 2024-05-08 06:02:34.000000 automlapp-0.1.69/AutoMLApp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      805 2024-05-08 06:02:34.000000 automlapp-0.1.69/AutoMLApp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 06:02:34.000000 automlapp-0.1.69/AutoMLApp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2024-05-08 06:02:34.000000 automlapp-0.1.69/AutoMLApp.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      268 2024-05-08 06:02:34.000000 automlapp-0.1.69/AutoMLApp.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-08 06:02:34.000000 automlapp-0.1.69/AutoMLApp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1088 2024-05-03 11:39:36.000000 automlapp-0.1.69/LICENSE
--rw-rw-rw-   0        0        0     5052 2024-05-08 06:02:34.202788 automlapp-0.1.69/PKG-INFO
--rw-rw-rw-   0        0        0     3993 2024-04-12 09:40:36.000000 automlapp-0.1.69/README.md
-drwxrwxrwx   0        0        0        0 2024-05-08 06:02:34.183619 automlapp-0.1.69/automlapp/
--rw-rw-rw-   0        0        0       44 2024-05-07 10:07:08.000000 automlapp-0.1.69/automlapp/__init__.py
--rw-rw-rw-   0        0        0    60983 2024-05-08 05:51:07.000000 automlapp-0.1.69/automlapp/app.py
--rw-rw-rw-   0        0        0      207 2024-05-08 05:56:14.000000 automlapp-0.1.69/automlapp/launcher.py
--rw-rw-rw-   0        0        0   109179 2024-02-26 11:55:20.000000 automlapp-0.1.69/automlapp/logo.png
-drwxrwxrwx   0        0        0        0 2024-05-08 06:02:34.196962 automlapp-0.1.69/automlapp/modules/
--rw-rw-rw-   0        0        0        0 2024-05-07 11:09:32.000000 automlapp-0.1.69/automlapp/modules/__init__.py
--rw-rw-rw-   0        0        0     5469 2024-05-07 11:23:48.000000 automlapp-0.1.69/automlapp/modules/data_cleaning.py
--rw-rw-rw-   0        0        0     2511 2024-05-07 11:23:57.000000 automlapp-0.1.69/automlapp/modules/data_input.py
--rw-rw-rw-   0        0        0     3332 2024-05-07 11:24:04.000000 automlapp-0.1.69/automlapp/modules/data_preprocessing.py
--rw-rw-rw-   0        0        0     1074 2024-05-07 11:24:45.000000 automlapp-0.1.69/automlapp/modules/data_summarization.py
--rw-rw-rw-   0        0        0     3433 2024-05-07 11:24:56.000000 automlapp-0.1.69/automlapp/modules/data_visualization.py
--rw-rw-rw-   0        0        0     3650 2024-05-07 11:25:02.000000 automlapp-0.1.69/automlapp/modules/data_woeiv.py
--rw-rw-rw-   0        0        0     9481 2024-05-07 11:25:23.000000 automlapp-0.1.69/automlapp/modules/hyperparameter_tuning.py
--rw-rw-rw-   0        0        0    14623 2024-05-07 11:26:02.000000 automlapp-0.1.69/automlapp/modules/model_evaluation.py
--rw-rw-rw-   0        0        0     5534 2024-05-07 11:26:09.000000 automlapp-0.1.69/automlapp/modules/model_training.py
--rw-rw-rw-   0        0        0     6455 2024-05-07 11:29:20.000000 automlapp-0.1.69/automlapp/modules/train_user_params.py
-drwxrwxrwx   0        0        0        0 2024-05-08 06:02:34.200792 automlapp-0.1.69/automlapp/utils/
--rw-rw-rw-   0        0        0        0 2024-05-07 11:09:13.000000 automlapp-0.1.69/automlapp/utils/__init__.py
--rw-rw-rw-   0        0        0      199 2024-05-07 11:32:57.000000 automlapp-0.1.69/automlapp/utils/print_utils.py
--rw-rw-rw-   0        0        0      857 2024-05-07 11:32:56.000000 automlapp-0.1.69/automlapp/utils/streamlit_utils.py
--rw-rw-rw-   0        0        0       42 2024-05-08 06:02:34.204736 automlapp-0.1.69/setup.cfg
--rw-rw-rw-   0        0        0     1512 2024-05-08 06:02:28.000000 automlapp-0.1.69/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 06:39:26.782178 automlapp-0.1.7/
+drwxrwxrwx   0        0        0        0 2024-05-08 06:39:26.772848 automlapp-0.1.7/AutoMLApp.egg-info/
+-rw-rw-rw-   0        0        0     5051 2024-05-08 06:39:26.000000 automlapp-0.1.7/AutoMLApp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      827 2024-05-08 06:39:26.000000 automlapp-0.1.7/AutoMLApp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 06:39:26.000000 automlapp-0.1.7/AutoMLApp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2024-05-08 06:39:26.000000 automlapp-0.1.7/AutoMLApp.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      268 2024-05-08 06:39:26.000000 automlapp-0.1.7/AutoMLApp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-08 06:39:26.000000 automlapp-0.1.7/AutoMLApp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1088 2024-05-03 11:39:36.000000 automlapp-0.1.7/LICENSE
+-rw-rw-rw-   0        0        0     5051 2024-05-08 06:39:26.781179 automlapp-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     3993 2024-04-12 09:40:36.000000 automlapp-0.1.7/README.md
+drwxrwxrwx   0        0        0        0 2024-05-08 06:39:26.642321 automlapp-0.1.7/automlapp/
+-rw-rw-rw-   0        0        0       42 2024-05-08 06:36:50.000000 automlapp-0.1.7/automlapp/__init__.py
+-rw-rw-rw-   0        0        0    60971 2024-05-08 06:34:59.000000 automlapp-0.1.7/automlapp/app.py
+-rw-rw-rw-   0        0        0      212 2024-05-08 06:29:45.000000 automlapp-0.1.7/automlapp/launcher.py
+-rw-rw-rw-   0        0        0   109179 2024-02-26 11:55:20.000000 automlapp-0.1.7/automlapp/logo.png
+drwxrwxrwx   0        0        0        0 2024-05-08 06:39:26.749413 automlapp-0.1.7/automlapp/modules/
+-rw-rw-rw-   0        0        0        0 2024-05-07 11:09:32.000000 automlapp-0.1.7/automlapp/modules/__init__.py
+-rw-rw-rw-   0        0        0     5467 2024-05-08 06:33:17.000000 automlapp-0.1.7/automlapp/modules/data_cleaning.py
+-rw-rw-rw-   0        0        0     2509 2024-05-08 06:33:24.000000 automlapp-0.1.7/automlapp/modules/data_input.py
+-rw-rw-rw-   0        0        0     3330 2024-05-08 06:33:30.000000 automlapp-0.1.7/automlapp/modules/data_preprocessing.py
+-rw-rw-rw-   0        0        0     1072 2024-05-08 06:33:34.000000 automlapp-0.1.7/automlapp/modules/data_summarization.py
+-rw-rw-rw-   0        0        0     3431 2024-05-08 06:33:50.000000 automlapp-0.1.7/automlapp/modules/data_visualization.py
+-rw-rw-rw-   0        0        0     3648 2024-05-08 06:34:07.000000 automlapp-0.1.7/automlapp/modules/data_woeiv.py
+-rw-rw-rw-   0        0        0     9479 2024-05-08 06:34:12.000000 automlapp-0.1.7/automlapp/modules/hyperparameter_tuning.py
+-rw-rw-rw-   0        0        0    14621 2024-05-08 06:34:22.000000 automlapp-0.1.7/automlapp/modules/model_evaluation.py
+-rw-rw-rw-   0        0        0     5532 2024-05-08 06:34:28.000000 automlapp-0.1.7/automlapp/modules/model_training.py
+-rw-rw-rw-   0        0        0     6453 2024-05-08 06:34:32.000000 automlapp-0.1.7/automlapp/modules/train_user_params.py
+-rwxrwxrwx   0        0        0      266 2024-05-08 06:32:01.000000 automlapp-0.1.7/automlapp/runtool.bat
+drwxrwxrwx   0        0        0        0 2024-05-08 06:39:26.772848 automlapp-0.1.7/automlapp/utils/
+-rw-rw-rw-   0        0        0        0 2024-05-07 11:09:13.000000 automlapp-0.1.7/automlapp/utils/__init__.py
+-rw-rw-rw-   0        0        0      197 2024-05-08 06:34:51.000000 automlapp-0.1.7/automlapp/utils/print_utils.py
+-rw-rw-rw-   0        0        0      857 2024-05-07 11:32:56.000000 automlapp-0.1.7/automlapp/utils/streamlit_utils.py
+-rw-rw-rw-   0        0        0       42 2024-05-08 06:39:26.782178 automlapp-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0     1528 2024-05-08 06:38:34.000000 automlapp-0.1.7/setup.py
```

### Comparing `automlapp-0.1.69/AutoMLApp.egg-info/PKG-INFO` & `automlapp-0.1.7/AutoMLApp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AutoMLApp
-Version: 0.1.69
+Version: 0.1.7
 Summary: An automated machine learning application designed for efficient model training, evaluation, and hyperparameter tuning.
 Author: Shivam Nikam
 Author-email: shivam.nikam@think360.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `automlapp-0.1.69/AutoMLApp.egg-info/SOURCES.txt` & `automlapp-0.1.7/AutoMLApp.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 AutoMLApp.egg-info/entry_points.txt
 AutoMLApp.egg-info/requires.txt
 AutoMLApp.egg-info/top_level.txt
 automlapp/__init__.py
 automlapp/app.py
 automlapp/launcher.py
 automlapp/logo.png
+automlapp/runtool.bat
 automlapp/modules/__init__.py
 automlapp/modules/data_cleaning.py
 automlapp/modules/data_input.py
 automlapp/modules/data_preprocessing.py
 automlapp/modules/data_summarization.py
 automlapp/modules/data_visualization.py
 automlapp/modules/data_woeiv.py
```

### Comparing `automlapp-0.1.69/LICENSE` & `automlapp-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `automlapp-0.1.69/PKG-INFO` & `automlapp-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AutoMLApp
-Version: 0.1.69
+Version: 0.1.7
 Summary: An automated machine learning application designed for efficient model training, evaluation, and hyperparameter tuning.
 Author: Shivam Nikam
 Author-email: shivam.nikam@think360.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `automlapp-0.1.69/README.md` & `automlapp-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `automlapp-0.1.69/automlapp/app.py` & `automlapp-0.1.7/automlapp/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from streamlit_extras.colored_header import colored_header
 import pandas as pd
 import plotly.express as px
 from scipy.stats import skew
 from sklearn.decomposition import PCA
 from sklearn.model_selection import train_test_split
-from .utils.streamlit_utils import hide_icons, remove_whitespaces, st
-from .utils.print_utils import print_shape
+from utils.streamlit_utils import hide_icons, remove_whitespaces, st
+from utils.print_utils import print_shape
 from streamlit_modal import Modal
 import pickle
 import os, warnings, zipfile
 
-from .modules.data_input import DataInput
-from .modules.data_summarization import DataSummarization
-from .modules.data_cleaning import DataCleaning
-from .modules.data_visualization import DataVisualization
-from .modules.data_woeiv import DataWOEIV
-from .modules.data_preprocessing import DataPreprocessing
-from .modules.model_training import ModelTraining
-from .modules.model_evaluation import ModelEvaluation
-from .modules.hyperparameter_tuning import HyperparameterTuning
-from .modules.train_user_params import ModelTrainingWithUserParams
+from modules.data_input import DataInput
+from modules.data_summarization import DataSummarization
+from modules.data_cleaning import DataCleaning
+from modules.data_visualization import DataVisualization
+from modules.data_woeiv import DataWOEIV
+from modules.data_preprocessing import DataPreprocessing
+from modules.model_training import ModelTraining
+from modules.model_evaluation import ModelEvaluation
+from modules.hyperparameter_tuning import HyperparameterTuning
+from modules.train_user_params import ModelTrainingWithUserParams
 
 warnings.filterwarnings("ignore")
 
 plot_colors = px.colors.sequential.Blues[::-2]
 
 st.set_page_config(layout="wide")
 hide_icons()
```

### Comparing `automlapp-0.1.69/automlapp/logo.png` & `automlapp-0.1.7/automlapp/logo.png`

 * *Files identical despite different names*

### Comparing `automlapp-0.1.69/automlapp/modules/data_cleaning.py` & `automlapp-0.1.7/automlapp/modules/data_cleaning.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import numpy as np
 import pandas as pd
-from ..utils.streamlit_utils import hide_icons, remove_whitespaces, st
+from utils.streamlit_utils import hide_icons, remove_whitespaces, st
 
 class DataCleaning:
     def __init__(_self, df):
         _self.df = df.copy()
 
     def detect_outliers(_self, lower_percentile=5, upper_percentile=95):
         lower_bound, upper_bound = _self.df.quantile(lower_percentile/100), _self.df.quantile(upper_percentile/100)
```

### Comparing `automlapp-0.1.69/automlapp/modules/data_input.py` & `automlapp-0.1.7/automlapp/modules/data_input.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from ..utils.streamlit_utils import st
+from utils.streamlit_utils import st
 import os, io
 import pandas as pd
 import zipfile
 
 class DataInput:
     def __init__(_self, uploaded_file, key_suffix = None):
         _self.uploaded_file = uploaded_file
```

### Comparing `automlapp-0.1.69/automlapp/modules/data_preprocessing.py` & `automlapp-0.1.7/automlapp/modules/data_preprocessing.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from ..utils.streamlit_utils import st
+from utils.streamlit_utils import st
 import pandas as pd
 import numpy as np
 from scipy.stats import skew, boxcox
 from imblearn.over_sampling import RandomOverSampler
 from imblearn.under_sampling import RandomUnderSampler
 from imblearn.combine import SMOTEENN
 from sklearn.preprocessing import StandardScaler, MinMaxScaler, RobustScaler
```

### Comparing `automlapp-0.1.69/automlapp/modules/data_summarization.py` & `automlapp-0.1.7/automlapp/modules/data_summarization.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from ..utils.streamlit_utils import st
+from utils.streamlit_utils import st
 
 class DataSummarization:
     def __init__(_self, df):
         _self.df = df
 
     def summarize(_self):
         if _self.df is not None:
```

### Comparing `automlapp-0.1.69/automlapp/modules/data_visualization.py` & `automlapp-0.1.7/automlapp/modules/data_visualization.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from ..utils.streamlit_utils import st
+from utils.streamlit_utils import st
 import plotly.express as px
 
 class DataVisualization:
     def __init__(self, df):
         self.df = df
         self.plot_colors = px.colors.sequential.YlOrRd[::-2]
```

### Comparing `automlapp-0.1.69/automlapp/modules/data_woeiv.py` & `automlapp-0.1.7/automlapp/modules/data_woeiv.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from ..utils.streamlit_utils import st
+from utils.streamlit_utils import st
 import pandas as pd
 import numpy as np
 import scorecardpy as sc
 import io
 
 class DataWOEIV:
     def __init__(_self, df):
```

### Comparing `automlapp-0.1.69/automlapp/modules/hyperparameter_tuning.py` & `automlapp-0.1.7/automlapp/modules/hyperparameter_tuning.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from ..utils.streamlit_utils import st
+from utils.streamlit_utils import st
 import pandas as pd
 from sklearn.linear_model import LogisticRegression
 from sklearn.tree import DecisionTreeClassifier
 from sklearn.ensemble import RandomForestClassifier, AdaBoostClassifier
 from xgboost import XGBClassifier
 from lightgbm import LGBMClassifier
 from sklearn.model_selection import GridSearchCV, RandomizedSearchCV
```

### Comparing `automlapp-0.1.69/automlapp/modules/model_evaluation.py` & `automlapp-0.1.7/automlapp/modules/model_evaluation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from ..utils.streamlit_utils import st
+from utils.streamlit_utils import st
 import pandas as pd
 import numpy as np
 import plotly.express as px
 from sklearn.metrics import confusion_matrix, accuracy_score, confusion_matrix, precision_score, recall_score, f1_score, auc, roc_curve
 from sklearn.metrics import ConfusionMatrixDisplay
 
 class ModelEvaluation:
```

### Comparing `automlapp-0.1.69/automlapp/modules/model_training.py` & `automlapp-0.1.7/automlapp/modules/model_training.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from ..utils.streamlit_utils import st
+from utils.streamlit_utils import st
 import pandas as pd
 from sklearn.linear_model import LogisticRegression
 from sklearn.tree import DecisionTreeClassifier
 from sklearn.ensemble import RandomForestClassifier, AdaBoostClassifier
 from xgboost import XGBClassifier
 from lightgbm import LGBMClassifier
```

### Comparing `automlapp-0.1.69/automlapp/modules/train_user_params.py` & `automlapp-0.1.7/automlapp/modules/train_user_params.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from ..utils.streamlit_utils import st
+from utils.streamlit_utils import st
 import numpy as np
 from sklearn.linear_model import LogisticRegression
 from sklearn.tree import DecisionTreeClassifier
 from sklearn.ensemble import RandomForestClassifier, AdaBoostClassifier
 from xgboost import XGBClassifier
 from lightgbm import LGBMClassifier
 from sklearn.model_selection import GridSearchCV, RandomizedSearchCV
```

### Comparing `automlapp-0.1.69/automlapp/utils/streamlit_utils.py` & `automlapp-0.1.7/automlapp/utils/streamlit_utils.py`

 * *Files identical despite different names*

### Comparing `automlapp-0.1.69/setup.py` & `automlapp-0.1.7/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="AutoMLApp",
-    version="0.1.69",
+    version="0.1.7",
     author="Shivam Nikam",
     author_email="shivam.nikam@think360.ai",
     description="An automated machine learning application designed for efficient model training, evaluation, and hyperparameter tuning.",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     #url="https://github.com/YourGithub/AutoMLApp",
     packages=find_packages(),
@@ -34,15 +34,15 @@
         "dev": [
             "pytest>=5.2",
             "check-manifest",
             "twine",
         ],
     },
     package_data={
-        'automlapp': ['logo.png'],  # Specify relative path to package root
+        'automlapp': ['logo.png', 'runtool.bat'],  # Specify relative path to package root
     },
     entry_points={
         "console_scripts": [
-            "runtool=automlapp.launcher:main",
+            "fetchdir=automlapp.launcher:fetch",
         ],
     }
 )
```

