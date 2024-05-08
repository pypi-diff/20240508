# Comparing `tmp/statsplotly-0.2.0.tar.gz` & `tmp/statsplotly-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "statsplotly-0.2.0.tar", max compression
+gzip compressed data, was "statsplotly-0.2.1.tar", max compression
```

## Comparing `statsplotly-0.2.0.tar` & `statsplotly-0.2.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0     1519 2024-05-02 08:47:42.198993 statsplotly-0.2.0/LICENSE
--rw-r--r--   0        0        0     6330 2024-05-02 08:47:42.198993 statsplotly-0.2.0/README.md
--rw-r--r--   0        0        0     2885 2024-05-02 08:48:11.478899 statsplotly-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      345 2024-05-02 08:47:42.266992 statsplotly-0.2.0/statsplotly/__init__.py
--rw-r--r--   0        0        0      182 2024-05-02 08:47:42.266992 statsplotly-0.2.0/statsplotly/_base.py
--rw-r--r--   0        0        0        0 2024-05-02 08:47:42.266992 statsplotly-0.2.0/statsplotly/_plotting/__init__.py
--rw-r--r--   0        0        0     8240 2024-05-02 08:47:42.266992 statsplotly-0.2.0/statsplotly/_plotting/_barplot.py
--rw-r--r--   0        0        0     8126 2024-05-02 08:47:42.266992 statsplotly-0.2.0/statsplotly/_plotting/_catplot.py
--rw-r--r--   0        0        0    11056 2024-05-02 08:47:42.266992 statsplotly-0.2.0/statsplotly/_plotting/_distplot.py
--rw-r--r--   0        0        0     7247 2024-05-02 08:47:42.266992 statsplotly-0.2.0/statsplotly/_plotting/_heatmap.py
--rw-r--r--   0        0        0    20026 2024-05-02 08:47:42.266992 statsplotly-0.2.0/statsplotly/_plotting/_jointplot.py
--rw-r--r--   0        0        0    11514 2024-05-02 08:47:42.266992 statsplotly-0.2.0/statsplotly/_plotting/_plot.py
--rw-r--r--   0        0        0     6959 2024-05-02 08:47:42.266992 statsplotly-0.2.0/statsplotly/_plotting/helpers.py
--rw-r--r--   0        0        0     4001 2024-05-02 08:47:42.266992 statsplotly-0.2.0/statsplotly/constants.py
--rw-r--r--   0        0        0      289 2024-05-02 08:47:42.266992 statsplotly-0.2.0/statsplotly/exceptions.py
--rw-r--r--   0        0        0      111 2024-05-02 08:47:42.266992 statsplotly-0.2.0/statsplotly/plot_objects/__init__.py
--rw-r--r--   0        0        0      484 2024-05-02 08:47:42.266992 statsplotly-0.2.0/statsplotly/plot_objects/layout/__init__.py
--rw-r--r--   0        0        0     1995 2024-05-02 08:47:42.266992 statsplotly-0.2.0/statsplotly/plot_objects/layout/_axis.py
--rw-r--r--   0        0        0     8458 2024-05-02 08:47:42.266992 statsplotly-0.2.0/statsplotly/plot_objects/layout/_layout.py
--rw-r--r--   0        0        0    31230 2024-05-02 08:47:42.266992 statsplotly-0.2.0/statsplotly/plot_objects/trace.py
--rw-r--r--   0        0        0      162 2024-05-02 08:47:42.266992 statsplotly-0.2.0/statsplotly/plot_specifiers/__init__.py
--rw-r--r--   0        0        0      248 2024-05-02 08:47:42.266992 statsplotly-0.2.0/statsplotly/plot_specifiers/color/__init__.py
--rw-r--r--   0        0        0     9518 2024-05-02 08:47:42.266992 statsplotly-0.2.0/statsplotly/plot_specifiers/color/_core.py
--rw-r--r--   0        0        0     7454 2024-05-02 08:47:42.266992 statsplotly-0.2.0/statsplotly/plot_specifiers/color/_utils.py
--rw-r--r--   0        0        0     1730 2024-05-02 08:47:42.266992 statsplotly-0.2.0/statsplotly/plot_specifiers/common.py
--rw-r--r--   0        0        0      862 2024-05-02 08:47:42.266992 statsplotly-0.2.0/statsplotly/plot_specifiers/data/__init__.py
--rw-r--r--   0        0        0    25557 2024-05-02 08:47:42.266992 statsplotly-0.2.0/statsplotly/plot_specifiers/data/_core.py
--rw-r--r--   0        0        0      448 2024-05-02 08:47:42.266992 statsplotly-0.2.0/statsplotly/plot_specifiers/data/_utils.py
--rw-r--r--   0        0        0     4829 2024-05-02 08:47:42.266992 statsplotly-0.2.0/statsplotly/plot_specifiers/data/statistics.py
--rw-r--r--   0        0        0      286 2024-05-02 08:47:42.266992 statsplotly-0.2.0/statsplotly/plot_specifiers/figure/__init__.py
--rw-r--r--   0        0        0     8166 2024-05-02 08:47:42.266992 statsplotly-0.2.0/statsplotly/plot_specifiers/figure/_core.py
--rw-r--r--   0        0        0    23625 2024-05-02 08:47:42.266992 statsplotly-0.2.0/statsplotly/plot_specifiers/figure/_utils.py
--rw-r--r--   0        0        0      595 2024-05-02 08:47:42.266992 statsplotly-0.2.0/statsplotly/plot_specifiers/layout/__init__.py
--rw-r--r--   0        0        0     8221 2024-05-02 08:47:42.266992 statsplotly-0.2.0/statsplotly/plot_specifiers/layout/_core.py
--rw-r--r--   0        0        0     5489 2024-05-02 08:47:42.266992 statsplotly-0.2.0/statsplotly/plot_specifiers/layout/_utils.py
--rw-r--r--   0        0        0    14743 2024-05-02 08:47:42.266992 statsplotly-0.2.0/statsplotly/plot_specifiers/trace.py
--rw-r--r--   0        0        0      111 2024-05-02 08:47:42.266992 statsplotly-0.2.0/statsplotly/utils.py
--rw-r--r--   0        0        0     7220 1970-01-01 00:00:00.000000 statsplotly-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1519 2024-05-08 16:59:57.948482 statsplotly-0.2.1/LICENSE
+-rw-r--r--   0        0        0     6330 2024-05-08 16:59:57.948482 statsplotly-0.2.1/README.md
+-rw-r--r--   0        0        0     2885 2024-05-08 17:00:28.856341 statsplotly-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      345 2024-05-08 16:59:58.544479 statsplotly-0.2.1/statsplotly/__init__.py
+-rw-r--r--   0        0        0      182 2024-05-08 16:59:58.544479 statsplotly-0.2.1/statsplotly/_base.py
+-rw-r--r--   0        0        0        0 2024-05-08 16:59:58.544479 statsplotly-0.2.1/statsplotly/_plotting/__init__.py
+-rw-r--r--   0        0        0     8240 2024-05-08 16:59:58.544479 statsplotly-0.2.1/statsplotly/_plotting/_barplot.py
+-rw-r--r--   0        0        0     8126 2024-05-08 16:59:58.544479 statsplotly-0.2.1/statsplotly/_plotting/_catplot.py
+-rw-r--r--   0        0        0    11056 2024-05-08 16:59:58.544479 statsplotly-0.2.1/statsplotly/_plotting/_distplot.py
+-rw-r--r--   0        0        0     7247 2024-05-08 16:59:58.544479 statsplotly-0.2.1/statsplotly/_plotting/_heatmap.py
+-rw-r--r--   0        0        0    20026 2024-05-08 16:59:58.544479 statsplotly-0.2.1/statsplotly/_plotting/_jointplot.py
+-rw-r--r--   0        0        0    11514 2024-05-08 16:59:58.544479 statsplotly-0.2.1/statsplotly/_plotting/_plot.py
+-rw-r--r--   0        0        0     6959 2024-05-08 16:59:58.544479 statsplotly-0.2.1/statsplotly/_plotting/helpers.py
+-rw-r--r--   0        0        0     4001 2024-05-08 16:59:58.544479 statsplotly-0.2.1/statsplotly/constants.py
+-rw-r--r--   0        0        0      289 2024-05-08 16:59:58.544479 statsplotly-0.2.1/statsplotly/exceptions.py
+-rw-r--r--   0        0        0      111 2024-05-08 16:59:58.544479 statsplotly-0.2.1/statsplotly/plot_objects/__init__.py
+-rw-r--r--   0        0        0      484 2024-05-08 16:59:58.544479 statsplotly-0.2.1/statsplotly/plot_objects/layout/__init__.py
+-rw-r--r--   0        0        0     1995 2024-05-08 16:59:58.544479 statsplotly-0.2.1/statsplotly/plot_objects/layout/_axis.py
+-rw-r--r--   0        0        0     8458 2024-05-08 16:59:58.544479 statsplotly-0.2.1/statsplotly/plot_objects/layout/_layout.py
+-rw-r--r--   0        0        0    31230 2024-05-08 16:59:58.544479 statsplotly-0.2.1/statsplotly/plot_objects/trace.py
+-rw-r--r--   0        0        0      162 2024-05-08 16:59:58.544479 statsplotly-0.2.1/statsplotly/plot_specifiers/__init__.py
+-rw-r--r--   0        0        0      333 2024-05-08 16:59:58.544479 statsplotly-0.2.1/statsplotly/plot_specifiers/color/__init__.py
+-rw-r--r--   0        0        0     9565 2024-05-08 16:59:58.544479 statsplotly-0.2.1/statsplotly/plot_specifiers/color/_core.py
+-rw-r--r--   0        0        0     7621 2024-05-08 16:59:58.544479 statsplotly-0.2.1/statsplotly/plot_specifiers/color/_utils.py
+-rw-r--r--   0        0        0     1730 2024-05-08 16:59:58.544479 statsplotly-0.2.1/statsplotly/plot_specifiers/common.py
+-rw-r--r--   0        0        0      862 2024-05-08 16:59:58.544479 statsplotly-0.2.1/statsplotly/plot_specifiers/data/__init__.py
+-rw-r--r--   0        0        0    25557 2024-05-08 16:59:58.544479 statsplotly-0.2.1/statsplotly/plot_specifiers/data/_core.py
+-rw-r--r--   0        0        0      448 2024-05-08 16:59:58.544479 statsplotly-0.2.1/statsplotly/plot_specifiers/data/_utils.py
+-rw-r--r--   0        0        0     4829 2024-05-08 16:59:58.544479 statsplotly-0.2.1/statsplotly/plot_specifiers/data/statistics.py
+-rw-r--r--   0        0        0      286 2024-05-08 16:59:58.544479 statsplotly-0.2.1/statsplotly/plot_specifiers/figure/__init__.py
+-rw-r--r--   0        0        0     8166 2024-05-08 16:59:58.544479 statsplotly-0.2.1/statsplotly/plot_specifiers/figure/_core.py
+-rw-r--r--   0        0        0    23625 2024-05-08 16:59:58.544479 statsplotly-0.2.1/statsplotly/plot_specifiers/figure/_utils.py
+-rw-r--r--   0        0        0      595 2024-05-08 16:59:58.544479 statsplotly-0.2.1/statsplotly/plot_specifiers/layout/__init__.py
+-rw-r--r--   0        0        0     8221 2024-05-08 16:59:58.544479 statsplotly-0.2.1/statsplotly/plot_specifiers/layout/_core.py
+-rw-r--r--   0        0        0     5489 2024-05-08 16:59:58.544479 statsplotly-0.2.1/statsplotly/plot_specifiers/layout/_utils.py
+-rw-r--r--   0        0        0    14743 2024-05-08 16:59:58.544479 statsplotly-0.2.1/statsplotly/plot_specifiers/trace.py
+-rw-r--r--   0        0        0      215 2024-05-08 16:59:58.544479 statsplotly-0.2.1/statsplotly/utils.py
+-rw-r--r--   0        0        0     7220 1970-01-01 00:00:00.000000 statsplotly-0.2.1/PKG-INFO
```

### Comparing `statsplotly-0.2.0/LICENSE` & `statsplotly-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `statsplotly-0.2.0/README.md` & `statsplotly-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `statsplotly-0.2.0/pyproject.toml` & `statsplotly-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "statsplotly"
-version = "0.2.0"
+version = "0.2.1"
 description = "Tidy API for statistical visualization with Plotly"
 authors = ["Benjamin Roland <benjamin.roland@hotmail.fr>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 homepage = "https://github.com/parici75/statsplotly"
 documentation = "https://parici75.github.io/statsplotly/"
```

### Comparing `statsplotly-0.2.0/statsplotly/_plotting/_barplot.py` & `statsplotly-0.2.1/statsplotly/_plotting/_barplot.py`

 * *Files identical despite different names*

### Comparing `statsplotly-0.2.0/statsplotly/_plotting/_catplot.py` & `statsplotly-0.2.1/statsplotly/_plotting/_catplot.py`

 * *Files identical despite different names*

### Comparing `statsplotly-0.2.0/statsplotly/_plotting/_distplot.py` & `statsplotly-0.2.1/statsplotly/_plotting/_distplot.py`

 * *Files identical despite different names*

### Comparing `statsplotly-0.2.0/statsplotly/_plotting/_heatmap.py` & `statsplotly-0.2.1/statsplotly/_plotting/_heatmap.py`

 * *Files identical despite different names*

### Comparing `statsplotly-0.2.0/statsplotly/_plotting/_jointplot.py` & `statsplotly-0.2.1/statsplotly/_plotting/_jointplot.py`

 * *Files identical despite different names*

### Comparing `statsplotly-0.2.0/statsplotly/_plotting/_plot.py` & `statsplotly-0.2.1/statsplotly/_plotting/_plot.py`

 * *Files identical despite different names*

### Comparing `statsplotly-0.2.0/statsplotly/_plotting/helpers.py` & `statsplotly-0.2.1/statsplotly/_plotting/helpers.py`

 * *Files identical despite different names*

### Comparing `statsplotly-0.2.0/statsplotly/constants.py` & `statsplotly-0.2.1/statsplotly/constants.py`

 * *Files identical despite different names*

### Comparing `statsplotly-0.2.0/statsplotly/plot_objects/layout/_axis.py` & `statsplotly-0.2.1/statsplotly/plot_objects/layout/_axis.py`

 * *Files identical despite different names*

### Comparing `statsplotly-0.2.0/statsplotly/plot_objects/layout/_layout.py` & `statsplotly-0.2.1/statsplotly/plot_objects/layout/_layout.py`

 * *Files identical despite different names*

### Comparing `statsplotly-0.2.0/statsplotly/plot_objects/trace.py` & `statsplotly-0.2.1/statsplotly/plot_objects/trace.py`

 * *Files identical despite different names*

### Comparing `statsplotly-0.2.0/statsplotly/plot_specifiers/color/_core.py` & `statsplotly-0.2.1/statsplotly/plot_specifiers/color/_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from statsplotly import constants
 from statsplotly._base import BaseModel
 from statsplotly.exceptions import StatsPlotSpecificationError
 from statsplotly.plot_objects.layout import ColorAxis
 from statsplotly.plot_specifiers.common import smart_legend
 from statsplotly.plot_specifiers.layout import BarMode, ColoraxisReference
 
-from ._utils import ColorSystem, compute_colorscale, get_rgb_discrete_array
+from ._utils import ColorSystem, compute_colorscale, rgb_string_array_from_colormap
 
 logger = logging.getLogger(__name__)
 
 
 class ColorSpecifier(BaseModel):
     barmode: BarMode | None = None
     coloraxis_reference: ColoraxisReference | None = None
@@ -69,15 +69,15 @@
     @staticmethod
     def _check_is_discrete_color_data_type(color_data: pd.Series) -> bool:
         return is_bool_dtype(color_data) or is_object_dtype(color_data)
 
     @staticmethod
     def _check_is_direct_color_specification(color_data: pd.Series) -> bool:
         if ColorSpecifier._check_is_discrete_color_data_type(color_data):
-            return all(color_data.map(is_color_like))
+            return all(color_data.replace("0|1", "", regex=True).map(is_color_like))
 
         return False
 
     @staticmethod
     def _check_is_datetime_color_data_type(color_data: pd.Series) -> bool:
         return is_datetime64_any_dtype(color_data)
 
@@ -225,15 +225,15 @@
         colorbar = self.build_colorbar(color_data) if colorscale is not None else None
 
         return ColorAxis(
             cmin=cmin, cmax=cmax, colorscale=colorscale, colorbar=colorbar, showscale=self.colorbar
         )
 
     def get_color_hues(self, n_colors: int) -> list[str]:
-        return get_rgb_discrete_array(color_palette=self.color_palette, n_colors=n_colors)
+        return rgb_string_array_from_colormap(color_palette=self.color_palette, n_colors=n_colors)
 
     @classmethod
     def build_from_color_data(
         cls,
         color_data: pd.Series,
         **kwargs: Any,
     ) -> ColorSpecifier:
```

### Comparing `statsplotly-0.2.0/statsplotly/plot_specifiers/color/_utils.py` & `statsplotly-0.2.1/statsplotly/plot_specifiers/color/_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from typing import Any, TypeAlias
 
 import matplotlib
 import matplotlib.pyplot as plt
 import numpy as np
 import plotly
 import seaborn as sns
+from matplotlib.colors import to_rgb
 from numpy.typing import NDArray
 
 from statsplotly import constants
 from statsplotly.exceptions import StatsPlotSpecificationError, UnsupportedColormapError
 
 logger = logging.getLogger(__name__)
 
@@ -79,20 +80,23 @@
         try:
             # Then matplotlib
             return get_colorarray_from_matplotlib(cmap, n_colors=n_colors)
         except ValueError as exc:
             raise UnsupportedColormapError(f"{cmap} is not a supported colormap") from exc
 
 
-def to_rgb_string(numeric_rgb: tuple[float, float, float]) -> str:
-    """Transforms a numeric rgb tuple into a rgb string"""
-    return "rgb" + str(tuple(int(color * 256) for color in numeric_rgb)[:3])
+def to_rgb_string(color_reference: tuple[float, float, float] | str) -> str:
+    """Transforms a color reference into a plotly-compatible rgb string"""
+    if isinstance(color_reference, str):
+        color_reference = to_rgb(color_reference)
 
+    return "rgb" + str(tuple(int(color * 256) for color in color_reference)[:3])
 
-def get_rgb_discrete_array(
+
+def rgb_string_array_from_colormap(
     n_colors: int, color_palette: Cmap_specs | matplotlib.colors.Colormap | None
 ) -> list[str]:
     """Color list/Seaborn color_palette wrapper."""
     rgb_array = cmap_to_array(n_colors, color_palette)
 
     # Convert the RGB value array to a RGB plotly_friendly string array
     return [to_rgb_string(rgb) for rgb in rgb_array]
```

### Comparing `statsplotly-0.2.0/statsplotly/plot_specifiers/common.py` & `statsplotly-0.2.1/statsplotly/plot_specifiers/common.py`

 * *Files identical despite different names*

### Comparing `statsplotly-0.2.0/statsplotly/plot_specifiers/data/__init__.py` & `statsplotly-0.2.1/statsplotly/plot_specifiers/data/__init__.py`

 * *Files identical despite different names*

### Comparing `statsplotly-0.2.0/statsplotly/plot_specifiers/data/_core.py` & `statsplotly-0.2.1/statsplotly/plot_specifiers/data/_core.py`

 * *Files identical despite different names*

### Comparing `statsplotly-0.2.0/statsplotly/plot_specifiers/data/statistics.py` & `statsplotly-0.2.1/statsplotly/plot_specifiers/data/statistics.py`

 * *Files identical despite different names*

### Comparing `statsplotly-0.2.0/statsplotly/plot_specifiers/figure/_core.py` & `statsplotly-0.2.1/statsplotly/plot_specifiers/figure/_core.py`

 * *Files identical despite different names*

### Comparing `statsplotly-0.2.0/statsplotly/plot_specifiers/figure/_utils.py` & `statsplotly-0.2.1/statsplotly/plot_specifiers/figure/_utils.py`

 * *Files identical despite different names*

### Comparing `statsplotly-0.2.0/statsplotly/plot_specifiers/layout/__init__.py` & `statsplotly-0.2.1/statsplotly/plot_specifiers/layout/__init__.py`

 * *Files identical despite different names*

### Comparing `statsplotly-0.2.0/statsplotly/plot_specifiers/layout/_core.py` & `statsplotly-0.2.1/statsplotly/plot_specifiers/layout/_core.py`

 * *Files identical despite different names*

### Comparing `statsplotly-0.2.0/statsplotly/plot_specifiers/layout/_utils.py` & `statsplotly-0.2.1/statsplotly/plot_specifiers/layout/_utils.py`

 * *Files identical despite different names*

### Comparing `statsplotly-0.2.0/statsplotly/plot_specifiers/trace.py` & `statsplotly-0.2.1/statsplotly/plot_specifiers/trace.py`

 * *Files identical despite different names*

### Comparing `statsplotly-0.2.0/PKG-INFO` & `statsplotly-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: statsplotly
-Version: 0.2.0
+Version: 0.2.1
 Summary: Tidy API for statistical visualization with Plotly
 Home-page: https://github.com/parici75/statsplotly
 License: BSD-3-Clause
 Author: Benjamin Roland
 Author-email: benjamin.roland@hotmail.fr
 Requires-Python: >=3.10,<3.13
 Classifier: License :: OSI Approved :: BSD License
```

