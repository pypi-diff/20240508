# Comparing `tmp/USJ_dsptools-2024.5.2.tar.gz` & `tmp/USJ_dsptools-2024.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "USJ_dsptools-2024.5.2.tar", last modified: Thu May  2 09:53:30 2024, max compression
+gzip compressed data, was "USJ_dsptools-2024.5.8.tar", last modified: Wed May  8 14:14:18 2024, max compression
```

## Comparing `USJ_dsptools-2024.5.2.tar` & `USJ_dsptools-2024.5.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-05-02 09:53:30.322053 USJ_dsptools-2024.5.2/
--rw-rw-rw-   0        0        0    35823 2024-04-12 07:46:08.000000 USJ_dsptools-2024.5.2/LICENSE
--rw-rw-rw-   0        0        0     1607 2024-05-02 09:53:30.321059 USJ_dsptools-2024.5.2/PKG-INFO
--rw-rw-rw-   0        0        0      788 2024-05-02 08:33:20.000000 USJ_dsptools-2024.5.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-02 09:53:30.308740 USJ_dsptools-2024.5.2/USJ_dsptools.egg-info/
--rw-rw-rw-   0        0        0     1607 2024-05-02 09:53:29.000000 USJ_dsptools-2024.5.2/USJ_dsptools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      357 2024-05-02 09:53:30.000000 USJ_dsptools-2024.5.2/USJ_dsptools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-02 09:53:29.000000 USJ_dsptools-2024.5.2/USJ_dsptools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-05-02 09:53:29.000000 USJ_dsptools-2024.5.2/USJ_dsptools.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       65 2024-05-02 09:53:29.000000 USJ_dsptools-2024.5.2/USJ_dsptools.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-02 09:53:29.000000 USJ_dsptools-2024.5.2/USJ_dsptools.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-02 09:53:30.319061 USJ_dsptools-2024.5.2/dsptools/
--rw-rw-rw-   0        0        0     1162 2024-05-02 08:33:20.000000 USJ_dsptools-2024.5.2/dsptools/__init__.py
--rw-rw-rw-   0        0        0      777 2024-04-24 05:03:47.000000 USJ_dsptools-2024.5.2/dsptools/frequency.py
--rw-rw-rw-   0        0        0     8711 2024-05-02 08:33:20.000000 USJ_dsptools-2024.5.2/dsptools/graph.py
--rw-rw-rw-   0        0        0     1540 2024-04-24 05:03:25.000000 USJ_dsptools-2024.5.2/dsptools/operations.py
--rw-rw-rw-   0        0        0     8270 2024-05-02 08:33:20.000000 USJ_dsptools-2024.5.2/dsptools/ztransform.py
--rw-rw-rw-   0        0        0       86 2024-05-02 09:53:30.326040 USJ_dsptools-2024.5.2/setup.cfg
--rw-rw-rw-   0        0        0     1476 2024-05-02 09:53:12.000000 USJ_dsptools-2024.5.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 14:14:18.782236 USJ_dsptools-2024.5.8/
+-rw-rw-rw-   0        0        0    35823 2024-04-12 07:46:08.000000 USJ_dsptools-2024.5.8/LICENSE
+-rw-rw-rw-   0        0        0     1770 2024-05-08 14:14:18.781238 USJ_dsptools-2024.5.8/PKG-INFO
+-rw-rw-rw-   0        0        0      953 2024-05-08 14:11:09.000000 USJ_dsptools-2024.5.8/README.md
+drwxrwxrwx   0        0        0        0 2024-05-08 14:14:18.766183 USJ_dsptools-2024.5.8/USJ_dsptools.egg-info/
+-rw-rw-rw-   0        0        0     1770 2024-05-08 14:14:18.000000 USJ_dsptools-2024.5.8/USJ_dsptools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      357 2024-05-08 14:14:18.000000 USJ_dsptools-2024.5.8/USJ_dsptools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 14:14:18.000000 USJ_dsptools-2024.5.8/USJ_dsptools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-05-02 09:53:29.000000 USJ_dsptools-2024.5.8/USJ_dsptools.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       65 2024-05-08 14:14:18.000000 USJ_dsptools-2024.5.8/USJ_dsptools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-08 14:14:18.000000 USJ_dsptools-2024.5.8/USJ_dsptools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-08 14:14:18.779247 USJ_dsptools-2024.5.8/dsptools/
+-rw-rw-rw-   0        0        0     1329 2024-05-08 14:13:47.000000 USJ_dsptools-2024.5.8/dsptools/__init__.py
+-rw-rw-rw-   0        0        0      777 2024-04-24 05:03:47.000000 USJ_dsptools-2024.5.8/dsptools/frequency.py
+-rw-rw-rw-   0        0        0     8717 2024-05-08 14:11:09.000000 USJ_dsptools-2024.5.8/dsptools/graph.py
+-rw-rw-rw-   0        0        0     1540 2024-04-24 05:03:25.000000 USJ_dsptools-2024.5.8/dsptools/operations.py
+-rw-rw-rw-   0        0        0     8270 2024-05-02 08:33:20.000000 USJ_dsptools-2024.5.8/dsptools/ztransform.py
+-rw-rw-rw-   0        0        0       86 2024-05-08 14:14:18.785227 USJ_dsptools-2024.5.8/setup.cfg
+-rw-rw-rw-   0        0        0     1478 2024-05-08 14:11:09.000000 USJ_dsptools-2024.5.8/setup.py
```

### Comparing `USJ_dsptools-2024.5.2/LICENSE` & `USJ_dsptools-2024.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `USJ_dsptools-2024.5.2/PKG-INFO` & `USJ_dsptools-2024.5.8/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: USJ_dsptools
-Version: 2024.5.2
+Version: 2024.5.8
 Summary: A Python package to provide easy to use tools to learn and teach digital signal processing with Python.
 Home-page: https://github.com/aalcaineo/dsptools
 Author: Alejandro Alcaine, PhD
 Author-email: lalcaine@usj.es
 License: GNU General Public License v2.0
 Keywords: Digital Signal Processing
 Classifier: Development Status :: 3 - Alpha
@@ -20,27 +20,37 @@
 Provides-Extra: dev
 Requires-Dist: twine>=4.0.2; extra == "dev"
 
 # DSPTools
 Digital Signal Processing Tools is a Python package to provide easy to use tools to learn
 and teach digital signal processing with Python.
 
-#### Version: 2024.05.02
+#### Version: 2024.05.08
 
 ## Modules:
 * graph: Provides functionality to easily visualise signals. `plot_signal()` is already 
          available by direct import.
 * operations: Provides basic operations on the independent variable of signals.
 * frequency: Provides frequency analysis tools.
 * ztransform: Provides tools for working with z-transform.
 
+## Installation and usage:
+
+Please install this package using PiP by typing:
+
+`pip install USJ_dsptools`
+
+Import this module as:
+
+`import dsptools as dsp`
+
 ## Author:
 Alejandro Alcaine, Ph.D\
 CoMBA research group\
 MESC Working Group on e-Cardiology\
 MESC European Association of Cardiovascular Imaging (EACVI)\
 lalcaine@usj.es
 
 Faculty of Health Sciences\
 University San Jorge\
-Villanueva de GÃ¡llego (Zaragoza)\
+Villanueva de Gallego (Zaragoza)\
 Spain
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `USJ_dsptools-2024.5.2/USJ_dsptools.egg-info/PKG-INFO` & `USJ_dsptools-2024.5.8/USJ_dsptools.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: USJ-dsptools
-Version: 2024.5.2
+Version: 2024.5.8
 Summary: A Python package to provide easy to use tools to learn and teach digital signal processing with Python.
 Home-page: https://github.com/aalcaineo/dsptools
 Author: Alejandro Alcaine, PhD
 Author-email: lalcaine@usj.es
 License: GNU General Public License v2.0
 Keywords: Digital Signal Processing
 Classifier: Development Status :: 3 - Alpha
@@ -20,27 +20,37 @@
 Provides-Extra: dev
 Requires-Dist: twine>=4.0.2; extra == "dev"
 
 # DSPTools
 Digital Signal Processing Tools is a Python package to provide easy to use tools to learn
 and teach digital signal processing with Python.
 
-#### Version: 2024.05.02
+#### Version: 2024.05.08
 
 ## Modules:
 * graph: Provides functionality to easily visualise signals. `plot_signal()` is already 
          available by direct import.
 * operations: Provides basic operations on the independent variable of signals.
 * frequency: Provides frequency analysis tools.
 * ztransform: Provides tools for working with z-transform.
 
+## Installation and usage:
+
+Please install this package using PiP by typing:
+
+`pip install USJ_dsptools`
+
+Import this module as:
+
+`import dsptools as dsp`
+
 ## Author:
 Alejandro Alcaine, Ph.D\
 CoMBA research group\
 MESC Working Group on e-Cardiology\
 MESC European Association of Cardiovascular Imaging (EACVI)\
 lalcaine@usj.es
 
 Faculty of Health Sciences\
 University San Jorge\
-Villanueva de GÃ¡llego (Zaragoza)\
+Villanueva de Gallego (Zaragoza)\
 Spain
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `USJ_dsptools-2024.5.2/dsptools/__init__.py` & `USJ_dsptools-2024.5.8/dsptools/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,37 +1,47 @@
 """
 -----------------------------------------------------------------------------------------
 DSPTools
 -----------------------------------------------------------------------------------------
 Digital Signal Processing Tools is a Python package to provide easy to use tools to learn
 and teach digital signal processing with Python.
 
-Version: 2024.05.02
+Version: 2024.05.08
 
 ### Modules:
 * graph: Provides functionality to easily visualise signals. `plot_signal()` is already 
          available by direct import.
 * operations: Provides basic operations on the independent variable of signals.
 * frequency: Provides frequency analysis tools.
 * ztransform: Provides tools for working with z-transform.
 
+### Installation and usage:
+
+Please install this package using PiP by typing:
+
+`pip install USJ_dsptools`
+
+Import this module as:
+
+`import dsptools as dsp`
+
 ### Author:
 Alejandro Alcaine, Ph.D\\
 CoMBA research group\\
 MESC Working Group on e-Cardiology\\
 MESC European Association of Cardiovascular Imaging (EACVI)\\
 lalcaine@usj.es
 
 Faculty of Health Sciences\\
 University San Jorge\\
 Villanueva de Gállego (Zaragoza)\\
 Spain
 """
 
-__version__ = "2024.05.02"
+__version__ = "2024.05.08"
 
 from dsptools.graph import plot_signal
 
 import dsptools.operations
 import dsptools.graph
 import dsptools.frequency
 import dsptools.ztransform
```

### Comparing `USJ_dsptools-2024.5.2/dsptools/frequency.py` & `USJ_dsptools-2024.5.8/dsptools/frequency.py`

 * *Files identical despite different names*

### Comparing `USJ_dsptools-2024.5.2/dsptools/graph.py` & `USJ_dsptools-2024.5.8/dsptools/graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -168,17 +168,17 @@
 
 
 def iplot_signal(
     t: np.ndarray,
     x: np.ndarray,
     x_lim: tuple = None,
     y_lim: tuple = None,
+    x_label: str = "Time (s)",
+    y_label: str = "Amplitude (a.u.)",
     fig_title: str = "",
-    xlabel: str = "Time (s)",
-    ylabel: str = "Amplitude (a.u.)",
     legend: str = None,
     plot_width: int = 700,
     plot_height: int = 450,
     line_width: float = 1.5,
     to_notebook: bool = True,
 ) -> None:
     """Signal interactive plot.
@@ -190,23 +190,23 @@
 
         x_lim (tuple, optional): Horizontal axis span limitation.
         Defaults to None.
 
         y_lim (tuple, optional): Vertical axis span limitation.
         Defaults to None.
 
-        fig_title (str, optional): Title of the figure.
-        Defaults to "".
-
         xlabel (str, optional): Label for the horizontal axis.
         Defaults to "Time (s)".
 
         ylabel (str, optional): Label for the vertical axis.
         Defaults to "Amplitude (a.u.)".
 
+        fig_title (str, optional): Title of the figure.
+        Defaults to "".
+
         legend (str, optional): Legend to be displayed if multple signals are plotted.
         Defaults to None (no legend).
 
         plot_width (int, optional): Width of the plot.
         Defaults to 700.
 
         plot_height (int, optional): Height of the plot.
@@ -230,16 +230,16 @@
     if y_lim is None:
         y_lim = (x.min() * 1.05, x.max() * 1.05)
     else:
         y_lim
 
     plot = figure(
         title=fig_title,
-        x_axis_label=xlabel,
-        y_axis_label=ylabel,
+        x_axis_label=x_label,
+        y_axis_label=y_label,
         x_range=x_lim,
         y_range=y_lim,
         width=plot_width,
         height=plot_height,
         toolbar_location="below",
     )
 
@@ -264,15 +264,15 @@
 
             plot.add_layout(plot.legend[0], "right")
 
         plot.add_tools(
             HoverTool(
                 line_policy="nearest",
                 point_policy="snap_to_data",
-                tooltips=[(ylabel, "$y{0.00}"), (xlabel, "$x{0.00}")],
+                tooltips=[(y_label, "$y{0.00}"), (x_label, "$x{0.00}")],
             )
         )
 
         show(plot, notebook_handle=to_notebook)
 
     except Exception as error:
         print("Error:" + str(error))
```

### Comparing `USJ_dsptools-2024.5.2/dsptools/operations.py` & `USJ_dsptools-2024.5.8/dsptools/operations.py`

 * *Files identical despite different names*

### Comparing `USJ_dsptools-2024.5.2/dsptools/ztransform.py` & `USJ_dsptools-2024.5.8/dsptools/ztransform.py`

 * *Files identical despite different names*

### Comparing `USJ_dsptools-2024.5.2/setup.py` & `USJ_dsptools-2024.5.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 with open(os.path.join(this_directory,PACKAGE_NAME,"__init__.py"), "r") as f:
     version = ""
     while not version:
         version = re.findall('\t*\s*^__version__\s*=\s*"(\d*\.\d*\.\d*)"\n+', f.readline())
 
 setup(
-    name="USJ_"+PACKAGE_NAME,
+    name="USJ_" + PACKAGE_NAME,
     packages=find_packages(exclude=['*tests*']),
     version=version[0],
     license="GNU General Public License v2.0",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
     author=AUTHOR,
```

