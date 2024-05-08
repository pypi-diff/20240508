# Comparing `tmp/mpl_bsic-1.4.0a1.tar.gz` & `tmp/mpl_bsic-1.4.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpl_bsic-1.4.0a1.tar", max compression
+gzip compressed data, was "mpl_bsic-1.4.0a2.tar", max compression
```

## Comparing `mpl_bsic-1.4.0a1.tar` & `mpl_bsic-1.4.0a2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1095 2023-11-28 19:36:34.844975 mpl_bsic-1.4.0a1/LICENSE.md
--rw-r--r--   0        0        0      542 2024-05-07 07:59:34.165462 mpl_bsic-1.4.0a1/mpl_bsic/__init__.py
--rw-r--r--   0        0        0     4670 2024-05-05 00:44:11.362885 mpl_bsic-1.4.0a1/mpl_bsic/add_title_subtitle.py
--rw-r--r--   0        0        0     6019 2024-05-05 00:44:11.363885 mpl_bsic-1.4.0a1/mpl_bsic/apply_bsic_logo.py
--rw-r--r--   0        0        0     8147 2024-05-08 15:36:44.338906 mpl_bsic-1.4.0a1/mpl_bsic/apply_bsic_style.py
--rw-r--r--   0        0        0     4882 2023-11-30 23:26:30.042432 mpl_bsic-1.4.0a1/mpl_bsic/check_figsize.py
--rw-r--r--   0        0        0     1979 2024-05-08 15:38:17.699328 mpl_bsic-1.4.0a1/mpl_bsic/constants.py
--rw-r--r--   0        0        0     1457 2024-05-05 00:44:11.368385 mpl_bsic-1.4.0a1/mpl_bsic/export_figure.py
--rw-r--r--   0        0        0   198072 2023-12-01 10:47:04.227181 mpl_bsic-1.4.0a1/mpl_bsic/fonts/garamond/Garamond.TTF
--rw-r--r--   0        0        0   199772 2023-12-01 10:47:04.235181 mpl_bsic-1.4.0a1/mpl_bsic/fonts/garamond/Garamond_Bold.TTF
--rw-r--r--   0        0        0   189464 2023-12-01 10:47:04.247681 mpl_bsic-1.4.0a1/mpl_bsic/fonts/garamond/Garamond_Italic.TTF
--rw-r--r--   0        0        0    60160 2023-12-01 10:47:04.249182 mpl_bsic-1.4.0a1/mpl_bsic/fonts/gill_sans_mt/GillSansMT_Base.ttf
--rw-r--r--   0        0        0    68304 2023-12-01 10:47:04.250181 mpl_bsic-1.4.0a1/mpl_bsic/fonts/gill_sans_mt/GillSansMT_Bold.TTF
--rw-r--r--   0        0        0    71496 2023-12-01 10:47:04.251683 mpl_bsic-1.4.0a1/mpl_bsic/fonts/gill_sans_mt/GillSansMT_BoldItalic.TTF
--rw-r--r--   0        0        0    69436 2023-12-01 10:47:04.252681 mpl_bsic-1.4.0a1/mpl_bsic/fonts/gill_sans_mt/GillSansMT_Italic.TTF
--rw-r--r--   0        0        0     1966 2023-11-30 16:41:49.328724 mpl_bsic-1.4.0a1/mpl_bsic/format_timeseries_axis.py
--rw-r--r--   0        0        0    10489 2023-12-01 00:50:58.631581 mpl_bsic-1.4.0a1/mpl_bsic/plot_trade.py
--rw-r--r--   0        0        0      779 2023-11-14 09:45:21.027794 mpl_bsic-1.4.0a1/mpl_bsic/preprocess_dataframe.py
--rw-r--r--   0        0        0   282980 2023-11-30 11:27:50.191357 mpl_bsic-1.4.0a1/mpl_bsic/static/bsic_logo_formal_1x.png
--rw-r--r--   0        0        0   921240 2023-11-30 11:27:50.197859 mpl_bsic-1.4.0a1/mpl_bsic/static/bsic_logo_formal_2x.png
--rw-r--r--   0        0        0  1910183 2023-11-30 11:27:50.209859 mpl_bsic-1.4.0a1/mpl_bsic/static/bsic_logo_formal_3x.png
--rw-r--r--   0        0        0   164720 2023-11-30 11:27:50.211358 mpl_bsic-1.4.0a1/mpl_bsic/static/bsic_logo_square_1x.png
--rw-r--r--   0        0        0   576512 2023-11-30 11:27:50.215358 mpl_bsic-1.4.0a1/mpl_bsic/static/bsic_logo_square_2x.png
--rw-r--r--   0        0        0  1208390 2023-11-30 11:27:50.223357 mpl_bsic-1.4.0a1/mpl_bsic/static/bsic_logo_square_3x.png
--rw-r--r--   0        0        0    10342 2024-02-24 18:34:47.481627 mpl_bsic-1.4.0a1/mpl_bsic/style_excel.py
--rw-r--r--   0        0        0     1022 2024-05-08 15:41:35.932524 mpl_bsic-1.4.0a1/pyproject.toml
--rw-r--r--   0        0        0     4320 2023-12-01 14:37:36.997369 mpl_bsic-1.4.0a1/README.md
--rw-r--r--   0        0        0        0 2023-11-30 22:39:19.895120 mpl_bsic-1.4.0a1/utils/__init__.py
--rw-r--r--   0        0        0     1473 2023-12-01 10:47:04.254182 mpl_bsic-1.4.0a1/utils/add_fonts.py
--rw-r--r--   0        0        0      469 2024-05-05 00:44:11.374886 mpl_bsic-1.4.0a1/utils/logger.py
--rw-r--r--   0        0        0      529 2023-11-30 23:26:30.044933 mpl_bsic-1.4.0a1/utils/run_animations.py
--rw-r--r--   0        0        0      414 2023-11-30 14:02:43.673722 mpl_bsic-1.4.0a1/utils/set_animations.py
--rw-r--r--   0        0        0     4848 1970-01-01 00:00:00.000000 mpl_bsic-1.4.0a1/PKG-INFO
+-rw-r--r--   0        0        0     1095 2023-11-28 19:36:34.844975 mpl_bsic-1.4.0a2/LICENSE.md
+-rw-r--r--   0        0        0      542 2024-05-07 07:59:34.165462 mpl_bsic-1.4.0a2/mpl_bsic/__init__.py
+-rw-r--r--   0        0        0     4734 2024-05-08 16:06:40.249036 mpl_bsic-1.4.0a2/mpl_bsic/add_title_subtitle.py
+-rw-r--r--   0        0        0     6019 2024-05-05 00:44:11.363885 mpl_bsic-1.4.0a2/mpl_bsic/apply_bsic_logo.py
+-rw-r--r--   0        0        0     8147 2024-05-08 15:36:44.338906 mpl_bsic-1.4.0a2/mpl_bsic/apply_bsic_style.py
+-rw-r--r--   0        0        0     4882 2023-11-30 23:26:30.042432 mpl_bsic-1.4.0a2/mpl_bsic/check_figsize.py
+-rw-r--r--   0        0        0     1979 2024-05-08 15:38:17.699328 mpl_bsic-1.4.0a2/mpl_bsic/constants.py
+-rw-r--r--   0        0        0     1457 2024-05-05 00:44:11.368385 mpl_bsic-1.4.0a2/mpl_bsic/export_figure.py
+-rw-r--r--   0        0        0   198072 2023-12-01 10:47:04.227181 mpl_bsic-1.4.0a2/mpl_bsic/fonts/garamond/Garamond.TTF
+-rw-r--r--   0        0        0   199772 2023-12-01 10:47:04.235181 mpl_bsic-1.4.0a2/mpl_bsic/fonts/garamond/Garamond_Bold.TTF
+-rw-r--r--   0        0        0   189464 2023-12-01 10:47:04.247681 mpl_bsic-1.4.0a2/mpl_bsic/fonts/garamond/Garamond_Italic.TTF
+-rw-r--r--   0        0        0    60160 2023-12-01 10:47:04.249182 mpl_bsic-1.4.0a2/mpl_bsic/fonts/gill_sans_mt/GillSansMT_Base.ttf
+-rw-r--r--   0        0        0    68304 2023-12-01 10:47:04.250181 mpl_bsic-1.4.0a2/mpl_bsic/fonts/gill_sans_mt/GillSansMT_Bold.TTF
+-rw-r--r--   0        0        0    71496 2023-12-01 10:47:04.251683 mpl_bsic-1.4.0a2/mpl_bsic/fonts/gill_sans_mt/GillSansMT_BoldItalic.TTF
+-rw-r--r--   0        0        0    69436 2023-12-01 10:47:04.252681 mpl_bsic-1.4.0a2/mpl_bsic/fonts/gill_sans_mt/GillSansMT_Italic.TTF
+-rw-r--r--   0        0        0     1966 2023-11-30 16:41:49.328724 mpl_bsic-1.4.0a2/mpl_bsic/format_timeseries_axis.py
+-rw-r--r--   0        0        0    10489 2023-12-01 00:50:58.631581 mpl_bsic-1.4.0a2/mpl_bsic/plot_trade.py
+-rw-r--r--   0        0        0      779 2023-11-14 09:45:21.027794 mpl_bsic-1.4.0a2/mpl_bsic/preprocess_dataframe.py
+-rw-r--r--   0        0        0   282980 2023-11-30 11:27:50.191357 mpl_bsic-1.4.0a2/mpl_bsic/static/bsic_logo_formal_1x.png
+-rw-r--r--   0        0        0   921240 2023-11-30 11:27:50.197859 mpl_bsic-1.4.0a2/mpl_bsic/static/bsic_logo_formal_2x.png
+-rw-r--r--   0        0        0  1910183 2023-11-30 11:27:50.209859 mpl_bsic-1.4.0a2/mpl_bsic/static/bsic_logo_formal_3x.png
+-rw-r--r--   0        0        0   164720 2023-11-30 11:27:50.211358 mpl_bsic-1.4.0a2/mpl_bsic/static/bsic_logo_square_1x.png
+-rw-r--r--   0        0        0   576512 2023-11-30 11:27:50.215358 mpl_bsic-1.4.0a2/mpl_bsic/static/bsic_logo_square_2x.png
+-rw-r--r--   0        0        0  1208390 2023-11-30 11:27:50.223357 mpl_bsic-1.4.0a2/mpl_bsic/static/bsic_logo_square_3x.png
+-rw-r--r--   0        0        0    10342 2024-02-24 18:34:47.481627 mpl_bsic-1.4.0a2/mpl_bsic/style_excel.py
+-rw-r--r--   0        0        0     1022 2024-05-08 16:07:21.742029 mpl_bsic-1.4.0a2/pyproject.toml
+-rw-r--r--   0        0        0     4320 2023-12-01 14:37:36.997369 mpl_bsic-1.4.0a2/README.md
+-rw-r--r--   0        0        0        0 2023-11-30 22:39:19.895120 mpl_bsic-1.4.0a2/utils/__init__.py
+-rw-r--r--   0        0        0     1473 2023-12-01 10:47:04.254182 mpl_bsic-1.4.0a2/utils/add_fonts.py
+-rw-r--r--   0        0        0      469 2024-05-05 00:44:11.374886 mpl_bsic-1.4.0a2/utils/logger.py
+-rw-r--r--   0        0        0      529 2023-11-30 23:26:30.044933 mpl_bsic-1.4.0a2/utils/run_animations.py
+-rw-r--r--   0        0        0      414 2023-11-30 14:02:43.673722 mpl_bsic-1.4.0a2/utils/set_animations.py
+-rw-r--r--   0        0        0     4848 1970-01-01 00:00:00.000000 mpl_bsic-1.4.0a2/PKG-INFO
```

### Comparing `mpl_bsic-1.4.0a1/LICENSE.md` & `mpl_bsic-1.4.0a2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mpl_bsic-1.4.0a1/mpl_bsic/__init__.py` & `mpl_bsic-1.4.0a2/mpl_bsic/__init__.py`

 * *Files identical despite different names*

### Comparing `mpl_bsic-1.4.0a1/mpl_bsic/add_title_subtitle.py` & `mpl_bsic-1.4.0a2/mpl_bsic/add_title_subtitle.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from .constants import SUBTITLE_STYLE, TITLE_STYLE
 import numpy as np
 from utils.logger import get_logger
 
 logger = get_logger(__name__)
 
 
-def add_title_subtitle(fig: Figure, title: str, subtitle: str, wrapping_factor: float = 0.8):
+def add_title_subtitle(fig: Figure, title: str, subtitle: str, wrapping_factor: float = 0.8, subtitle_bottom_margin: float = 20):
     """Add title and subtitle to the plot.
 
     Adds a title (Franklin Gothic Bold) and subtitle (Franklin Gothic Medium Italic, smaller
     font size) to the top of the plot. Wraps the subtitle automatically inserting newlines,
     in order to not make it overflow.
 
     If you specified a title for the plot, this function will remove it and substitute with the title you specify
@@ -97,15 +97,15 @@
     }
     bbox_params = {
         'pad': 0,
         'alpha': 0
     }
 
     # draw the subtitle annotation
-    subtitle_bottom_margin = 20  # give it a bit of distance from the top
+    # subtitle_bottom_margin = 20  # give it a bit of distance from the top # THIS IS NOW A PARAMETER
     subtitle_xytext = (0, subtitle_bottom_margin) # define position of subtitle
     subtitle_annotation = ax.annotate(
         subtitle,
         xytext=subtitle_xytext,
         **annotate_params,
         **SUBTITLE_STYLE,
         bbox=bbox_params)
```

### Comparing `mpl_bsic-1.4.0a1/mpl_bsic/apply_bsic_logo.py` & `mpl_bsic-1.4.0a2/mpl_bsic/apply_bsic_logo.py`

 * *Files identical despite different names*

### Comparing `mpl_bsic-1.4.0a1/mpl_bsic/apply_bsic_style.py` & `mpl_bsic-1.4.0a2/mpl_bsic/apply_bsic_style.py`

 * *Files identical despite different names*

### Comparing `mpl_bsic-1.4.0a1/mpl_bsic/check_figsize.py` & `mpl_bsic-1.4.0a2/mpl_bsic/check_figsize.py`

 * *Files identical despite different names*

### Comparing `mpl_bsic-1.4.0a1/mpl_bsic/constants.py` & `mpl_bsic-1.4.0a2/mpl_bsic/constants.py`

 * *Files identical despite different names*

### Comparing `mpl_bsic-1.4.0a1/mpl_bsic/export_figure.py` & `mpl_bsic-1.4.0a2/mpl_bsic/export_figure.py`

 * *Files identical despite different names*

### Comparing `mpl_bsic-1.4.0a1/mpl_bsic/fonts/garamond/Garamond.TTF` & `mpl_bsic-1.4.0a2/mpl_bsic/fonts/garamond/Garamond.TTF`

 * *Files identical despite different names*

### Comparing `mpl_bsic-1.4.0a1/mpl_bsic/fonts/garamond/Garamond_Bold.TTF` & `mpl_bsic-1.4.0a2/mpl_bsic/fonts/garamond/Garamond_Bold.TTF`

 * *Files identical despite different names*

### Comparing `mpl_bsic-1.4.0a1/mpl_bsic/fonts/garamond/Garamond_Italic.TTF` & `mpl_bsic-1.4.0a2/mpl_bsic/fonts/garamond/Garamond_Italic.TTF`

 * *Files identical despite different names*

### Comparing `mpl_bsic-1.4.0a1/mpl_bsic/fonts/gill_sans_mt/GillSansMT_Base.ttf` & `mpl_bsic-1.4.0a2/mpl_bsic/fonts/gill_sans_mt/GillSansMT_Base.ttf`

 * *Files identical despite different names*

### Comparing `mpl_bsic-1.4.0a1/mpl_bsic/fonts/gill_sans_mt/GillSansMT_Bold.TTF` & `mpl_bsic-1.4.0a2/mpl_bsic/fonts/gill_sans_mt/GillSansMT_Bold.TTF`

 * *Files identical despite different names*

### Comparing `mpl_bsic-1.4.0a1/mpl_bsic/fonts/gill_sans_mt/GillSansMT_BoldItalic.TTF` & `mpl_bsic-1.4.0a2/mpl_bsic/fonts/gill_sans_mt/GillSansMT_BoldItalic.TTF`

 * *Files identical despite different names*

### Comparing `mpl_bsic-1.4.0a1/mpl_bsic/fonts/gill_sans_mt/GillSansMT_Italic.TTF` & `mpl_bsic-1.4.0a2/mpl_bsic/fonts/gill_sans_mt/GillSansMT_Italic.TTF`

 * *Files identical despite different names*

### Comparing `mpl_bsic-1.4.0a1/mpl_bsic/format_timeseries_axis.py` & `mpl_bsic-1.4.0a2/mpl_bsic/format_timeseries_axis.py`

 * *Files identical despite different names*

### Comparing `mpl_bsic-1.4.0a1/mpl_bsic/plot_trade.py` & `mpl_bsic-1.4.0a2/mpl_bsic/plot_trade.py`

 * *Files identical despite different names*

### Comparing `mpl_bsic-1.4.0a1/mpl_bsic/preprocess_dataframe.py` & `mpl_bsic-1.4.0a2/mpl_bsic/preprocess_dataframe.py`

 * *Files identical despite different names*

### Comparing `mpl_bsic-1.4.0a1/mpl_bsic/static/bsic_logo_formal_1x.png` & `mpl_bsic-1.4.0a2/mpl_bsic/static/bsic_logo_formal_1x.png`

 * *Files identical despite different names*

### Comparing `mpl_bsic-1.4.0a1/mpl_bsic/static/bsic_logo_formal_2x.png` & `mpl_bsic-1.4.0a2/mpl_bsic/static/bsic_logo_formal_2x.png`

 * *Files identical despite different names*

### Comparing `mpl_bsic-1.4.0a1/mpl_bsic/static/bsic_logo_formal_3x.png` & `mpl_bsic-1.4.0a2/mpl_bsic/static/bsic_logo_formal_3x.png`

 * *Files identical despite different names*

### Comparing `mpl_bsic-1.4.0a1/mpl_bsic/static/bsic_logo_square_1x.png` & `mpl_bsic-1.4.0a2/mpl_bsic/static/bsic_logo_square_1x.png`

 * *Files identical despite different names*

### Comparing `mpl_bsic-1.4.0a1/mpl_bsic/static/bsic_logo_square_2x.png` & `mpl_bsic-1.4.0a2/mpl_bsic/static/bsic_logo_square_2x.png`

 * *Files identical despite different names*

### Comparing `mpl_bsic-1.4.0a1/mpl_bsic/static/bsic_logo_square_3x.png` & `mpl_bsic-1.4.0a2/mpl_bsic/static/bsic_logo_square_3x.png`

 * *Files identical despite different names*

### Comparing `mpl_bsic-1.4.0a1/mpl_bsic/style_excel.py` & `mpl_bsic-1.4.0a2/mpl_bsic/style_excel.py`

 * *Files identical despite different names*

### Comparing `mpl_bsic-1.4.0a1/pyproject.toml` & `mpl_bsic-1.4.0a2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "mpl_bsic"
 description = "BSIC Plotting Library"
 authors = ["Andrea Franceschini <andrea.franceschini2@studbocconi.it>"]
 readme = "README.md"
-version = "1.4.0a1"    
+version = "1.4.0a2"    
 packages = [{include = "mpl_bsic"}, {include = "utils"}]
 # testpypi v1.2.1
 
 [tool.poetry.dependencies]
 python = ">=3.9"
 matplotlib = "^3.7"
 numpy = "^1.25"
```

### Comparing `mpl_bsic-1.4.0a1/README.md` & `mpl_bsic-1.4.0a2/README.md`

 * *Files identical despite different names*

### Comparing `mpl_bsic-1.4.0a1/utils/add_fonts.py` & `mpl_bsic-1.4.0a2/utils/add_fonts.py`

 * *Files identical despite different names*

### Comparing `mpl_bsic-1.4.0a1/utils/run_animations.py` & `mpl_bsic-1.4.0a2/utils/run_animations.py`

 * *Files identical despite different names*

### Comparing `mpl_bsic-1.4.0a1/PKG-INFO` & `mpl_bsic-1.4.0a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpl_bsic
-Version: 1.4.0a1
+Version: 1.4.0a2
 Summary: BSIC Plotting Library
 Author: Andrea Franceschini
 Author-email: andrea.franceschini2@studbocconi.it
 Requires-Python: >=3.9
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mpl_bsic Version: 1.4.0a1 Summary: BSIC Plotting
+Metadata-Version: 2.1 Name: mpl_bsic Version: 1.4.0a2 Summary: BSIC Plotting
 Library Author: Andrea Franceschini Author-email:
 andrea.franceschini2@studbocconi.it Requires-Python: >=3.9 Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
 Python :: 3.12 Requires-Dist: matplotlib (>=3.7,<4.0) Requires-Dist: numpy
 (>=1.25,<2.0) Requires-Dist: pandas (>=2,<3) Requires-Dist: xlsxwriter
```

