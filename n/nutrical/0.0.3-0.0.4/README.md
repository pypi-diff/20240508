# Comparing `tmp/nutrical-0.0.3.tar.gz` & `tmp/nutrical-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nutrical-0.0.3.tar", last modified: Fri May  3 02:10:09 2024, max compression
+gzip compressed data, was "nutrical-0.0.4.tar", last modified: Wed May  8 03:53:42 2024, max compression
```

## Comparing `nutrical-0.0.3.tar` & `nutrical-0.0.4.tar`

### file list

```diff
@@ -1,21 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-05-03 02:10:09.637336 nutrical-0.0.3/
--rw-rw-rw-   0        0        0     3132 2024-05-03 02:10:09.635050 nutrical-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1843 2024-05-03 00:57:09.000000 nutrical-0.0.3/README.md
--rw-rw-rw-   0        0        0        2 2024-05-03 02:10:08.000000 nutrical-0.0.3/VERSION
-drwxrwxrwx   0        0        0        0 2024-05-03 02:10:09.631109 nutrical-0.0.3/data/
--rw-rw-rw-   0        0        0     3509 2024-05-02 05:10:03.000000 nutrical-0.0.3/data/TW_FDA_nutrition_items.csv
-drwxrwxrwx   0        0        0        0 2024-05-03 02:10:09.602264 nutrical-0.0.3/nutrical/
--rw-rw-rw-   0        0        0       24 2024-05-03 01:55:26.000000 nutrical-0.0.3/nutrical/__init__.py
--rw-rw-rw-   0        0        0     3955 2024-05-03 01:55:45.000000 nutrical-0.0.3/nutrical/nutrical.py
--rw-rw-rw-   0        0        0       95 2024-05-02 07:08:54.000000 nutrical-0.0.3/nutrical/taiwan-fda.py
--rw-rw-rw-   0        0        0     1408 2024-05-03 00:52:10.000000 nutrical-0.0.3/nutrical/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-03 02:10:09.619820 nutrical-0.0.3/nutrical.egg-info/
--rw-rw-rw-   0        0        0     3132 2024-05-03 02:10:09.000000 nutrical-0.0.3/nutrical.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      337 2024-05-03 02:10:09.000000 nutrical-0.0.3/nutrical.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-03 02:10:09.000000 nutrical-0.0.3/nutrical.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-05-03 02:10:09.000000 nutrical-0.0.3/nutrical.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-03 02:10:09.000000 nutrical-0.0.3/nutrical.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-03 02:10:09.638397 nutrical-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      929 2024-05-03 02:10:02.000000 nutrical-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-03 02:10:09.634048 nutrical-0.0.3/test/
--rw-rw-rw-   0        0        0      988 2024-05-03 02:09:09.000000 nutrical-0.0.3/test/test.py
+drwxrwxrwx   0        0        0        0 2024-05-08 03:53:42.356691 nutrical-0.0.4/
+-rw-rw-rw-   0        0        0    16887 2024-05-08 03:53:42.355281 nutrical-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0    12094 2024-05-08 03:50:00.000000 nutrical-0.0.4/README.md
+-rw-rw-rw-   0        0        0        2 2024-05-08 03:53:41.000000 nutrical-0.0.4/VERSION
+drwxrwxrwx   0        0        0        0 2024-05-08 03:53:42.349355 nutrical-0.0.4/data/
+-rw-rw-rw-   0        0        0     3509 2024-05-02 05:10:03.000000 nutrical-0.0.4/data/TW_FDA_nutrition_items.csv
+drwxrwxrwx   0        0        0        0 2024-05-08 03:53:42.320999 nutrical-0.0.4/nutrical/
+-rw-rw-rw-   0        0        0       42 2024-05-03 05:46:07.000000 nutrical-0.0.4/nutrical/__init__.py
+-rw-rw-rw-   0        0        0     1499 2024-05-08 03:45:36.000000 nutrical-0.0.4/nutrical/io.py
+-rw-rw-rw-   0        0        0     6202 2024-05-08 03:36:52.000000 nutrical-0.0.4/nutrical/nutrical.py
+-rw-rw-rw-   0        0        0       95 2024-05-02 07:08:54.000000 nutrical-0.0.4/nutrical/taiwan-fda.py
+-rw-rw-rw-   0        0        0     1840 2024-05-05 23:54:15.000000 nutrical-0.0.4/nutrical/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-08 03:53:42.340289 nutrical-0.0.4/nutrical.egg-info/
+-rw-rw-rw-   0        0        0    16887 2024-05-08 03:53:42.000000 nutrical-0.0.4/nutrical.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      339 2024-05-08 03:53:42.000000 nutrical-0.0.4/nutrical.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 03:53:42.000000 nutrical-0.0.4/nutrical.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-05-08 03:53:42.000000 nutrical-0.0.4/nutrical.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-08 03:53:42.000000 nutrical-0.0.4/nutrical.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-08 03:53:42.357687 nutrical-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      949 2024-05-03 02:55:53.000000 nutrical-0.0.4/setup.py
```

### Comparing `nutrical-0.0.3/data/TW_FDA_nutrition_items.csv` & `nutrical-0.0.4/data/TW_FDA_nutrition_items.csv`

 * *Files identical despite different names*

### Comparing `nutrical-0.0.3/nutrical/utils.py` & `nutrical-0.0.4/nutrical/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,52 +1,66 @@
 import pint
-from typing import Number
+from numbers import Number
 
 UREG = pint.UnitRegistry()
 
 
-def add_dollar(a, b):
-    try:
-        return a + b
-    except:
-        return None
-
-
-def add_portion(a, b):
-    """Portion addition
+def add_amount(a, b):
+    """amount addition
 
     Returns
     -------
     pint.Quantity
         Addition is only defined when both inputs are pint.Quantity.
         For str and Number, the unit is unrecognized and thus addition
         cannot be performed.
     """
     if isinstance(a, pint.Quantity) and isinstance(b, pint.Quantity):
-        return a + b
+        try:
+            return a + b
+        except:
+            return None
     return None
 
 
-def parse_portion(x):
-    """Parse portion
+def parse_amount(x):
+    """Parse amount
 
     Returns
     -------
     Number | str | pint.Quantity
         Depending on the input and whether the parsing succeeded, the 
         returned value could either be `Number`, `str`, or `pint.Quantity`.
 
         When input x is `str`, the returned value is either 
         `pint.Quantity` or `str`, depending on whether pint recognizes the
         unit in the passed in value.
 
         If the input x is `pint.Quantity` or `Number`, no parsing is done 
         and the input is returned as output.
     """
-    if isinstance(x, pint.Quantity) or isinstance(x, Number):
+    if isinstance(x, pint.Quantity) or isinstance(x, Number) or x is None:
         return x
     if isinstance(x, str):
         try:
             return UREG(x)
         except:
             return x
     raise Exception("Unsupported input type. Only (str|Number|pint.Quantity) are allowed.")
+
+
+def parse_unit(x):
+    if isinstance(x, pint.Quantity) or x is None:
+        return x
+    if isinstance(x, str):
+        try:
+            return UREG(x)
+        except:
+            Warning("Failed to parse unit. Return None.")
+            return None
+    raise Exception("Unsupported input type. Only (str|pint.Quantity) are allowed.")
+
+
+
+def round2(x, ndigits=None):
+    if x is None: return None
+    return round(x, ndigits=ndigits)
```

### Comparing `nutrical-0.0.3/setup.py` & `nutrical-0.0.4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/liao961120/nutrical",
     # package_dir = {'': 'src'},
     packages=['nutrical'],
     install_requires=[
         'Pint',
+        'tabulate',
     ],
     package_data={
         "": ["../data/TW_FDA_nutrition_items.csv", "../VERSION"],
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
```

