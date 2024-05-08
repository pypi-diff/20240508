# Comparing `tmp/viur_toolkit-0.1.0.dev7.tar.gz` & `tmp/viur_toolkit-0.1.0.dev8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "viur_toolkit-0.1.0.dev7.tar", last modified: Fri May  3 18:51:23 2024, max compression
+gzip compressed data, was "viur_toolkit-0.1.0.dev8.tar", last modified: Tue May  7 19:40:53 2024, max compression
```

## Comparing `viur_toolkit-0.1.0.dev7.tar` & `viur_toolkit-0.1.0.dev8.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:51:23.051939 viur_toolkit-0.1.0.dev7/
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-03 18:51:18.000000 viur_toolkit-0.1.0.dev7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-05-03 18:51:23.051939 viur_toolkit-0.1.0.dev7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-03 18:51:18.000000 viur_toolkit-0.1.0.dev7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-03 18:51:18.000000 viur_toolkit-0.1.0.dev7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-05-03 18:51:23.055939 viur_toolkit-0.1.0.dev7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 18:51:18.000000 viur_toolkit-0.1.0.dev7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:51:23.047939 viur_toolkit-0.1.0.dev7/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:51:23.047939 viur_toolkit-0.1.0.dev7/src/viur/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:51:23.051939 viur_toolkit-0.1.0.dev7/src/viur/toolkit/
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-03 18:51:18.000000 viur_toolkit-0.1.0.dev7/src/viur/toolkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-03 18:51:18.000000 viur_toolkit-0.1.0.dev7/src/viur/toolkit/checks.py
--rw-r--r--   0 runner    (1001) docker     (127)      977 2024-05-03 18:51:18.000000 viur_toolkit-0.1.0.dev7/src/viur/toolkit/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-05-03 18:51:18.000000 viur_toolkit-0.1.0.dev7/src/viur/toolkit/db.py
--rw-r--r--   0 runner    (1001) docker     (127)     7768 2024-05-03 18:51:18.000000 viur_toolkit-0.1.0.dev7/src/viur/toolkit/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     2772 2024-05-03 18:51:18.000000 viur_toolkit-0.1.0.dev7/src/viur/toolkit/memcache.py
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-03 18:51:18.000000 viur_toolkit-0.1.0.dev7/src/viur/toolkit/numeric.py
--rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-05-03 18:51:18.000000 viur_toolkit-0.1.0.dev7/src/viur/toolkit/property.py
--rw-r--r--   0 runner    (1001) docker     (127)     3905 2024-05-03 18:51:18.000000 viur_toolkit-0.1.0.dev7/src/viur/toolkit/report.py
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-03 18:51:18.000000 viur_toolkit-0.1.0.dev7/src/viur/toolkit/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-05-03 18:51:18.000000 viur_toolkit-0.1.0.dev7/src/viur/toolkit/viur.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:51:23.051939 viur_toolkit-0.1.0.dev7/src/viur_toolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-05-03 18:51:23.000000 viur_toolkit-0.1.0.dev7/src/viur_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-03 18:51:23.000000 viur_toolkit-0.1.0.dev7/src/viur_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 18:51:23.000000 viur_toolkit-0.1.0.dev7/src/viur_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-03 18:51:23.000000 viur_toolkit-0.1.0.dev7/src/viur_toolkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-03 18:51:23.000000 viur_toolkit-0.1.0.dev7/src/viur_toolkit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:40:53.811251 viur_toolkit-0.1.0.dev8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-07 19:40:49.000000 viur_toolkit-0.1.0.dev8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-05-07 19:40:53.811251 viur_toolkit-0.1.0.dev8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-07 19:40:49.000000 viur_toolkit-0.1.0.dev8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-07 19:40:49.000000 viur_toolkit-0.1.0.dev8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-07 19:40:53.811251 viur_toolkit-0.1.0.dev8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 19:40:49.000000 viur_toolkit-0.1.0.dev8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:40:53.807252 viur_toolkit-0.1.0.dev8/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:40:53.807252 viur_toolkit-0.1.0.dev8/src/viur/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:40:53.811251 viur_toolkit-0.1.0.dev8/src/viur/toolkit/
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-07 19:40:49.000000 viur_toolkit-0.1.0.dev8/src/viur/toolkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-07 19:40:49.000000 viur_toolkit-0.1.0.dev8/src/viur/toolkit/checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-05-07 19:40:49.000000 viur_toolkit-0.1.0.dev8/src/viur/toolkit/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-05-07 19:40:49.000000 viur_toolkit-0.1.0.dev8/src/viur/toolkit/db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7768 2024-05-07 19:40:49.000000 viur_toolkit-0.1.0.dev8/src/viur/toolkit/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4047 2024-05-07 19:40:49.000000 viur_toolkit-0.1.0.dev8/src/viur/toolkit/memcache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-07 19:40:49.000000 viur_toolkit-0.1.0.dev8/src/viur/toolkit/numeric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-05-07 19:40:49.000000 viur_toolkit-0.1.0.dev8/src/viur/toolkit/property.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3905 2024-05-07 19:40:49.000000 viur_toolkit-0.1.0.dev8/src/viur/toolkit/report.py
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-07 19:40:49.000000 viur_toolkit-0.1.0.dev8/src/viur/toolkit/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-05-07 19:40:49.000000 viur_toolkit-0.1.0.dev8/src/viur/toolkit/viur.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:40:53.811251 viur_toolkit-0.1.0.dev8/src/viur_toolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-05-07 19:40:53.000000 viur_toolkit-0.1.0.dev8/src/viur_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-07 19:40:53.000000 viur_toolkit-0.1.0.dev8/src/viur_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 19:40:53.000000 viur_toolkit-0.1.0.dev8/src/viur_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-07 19:40:53.000000 viur_toolkit-0.1.0.dev8/src/viur_toolkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-07 19:40:53.000000 viur_toolkit-0.1.0.dev8/src/viur_toolkit.egg-info/top_level.txt
```

### Comparing `viur_toolkit-0.1.0.dev7/LICENSE` & `viur_toolkit-0.1.0.dev8/LICENSE`

 * *Files identical despite different names*

### Comparing `viur_toolkit-0.1.0.dev7/PKG-INFO` & `viur_toolkit-0.1.0.dev8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: viur-toolkit
-Version: 0.1.0.dev7
+Version: 0.1.0.dev8
 Summary: A kit of helpers and tools to simplify more intensive use of ViUR
 Home-page: https://github.com/viur-framework/viur-toolkit
 Author: Sven Eberth
 Author-email: se@mausbrand.de
 Maintainer: Sven Eberth
 Maintainer-email: se@mausbrand.de
 Classifier: Intended Audience :: Developers
@@ -15,14 +15,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: Deprecated
+Requires-Dist: viur-core>=3.6
 
 # viur-toolkit
 
 <div align="center">
     <h1>viur-toolkit (WIP)</h1>
     <a href="https://pypi.org/project/viur-toolkit/">
         <img alt="Badge showing current PyPI version" title="PyPI" src="https://img.shields.io/pypi/v/viur-toolkit">
```

#### html2text {}

```diff
@@ -1,14 +1,15 @@
-Metadata-Version: 2.1 Name: viur-toolkit Version: 0.1.0.dev7 Summary: A kit of
+Metadata-Version: 2.1 Name: viur-toolkit Version: 0.1.0.dev8 Summary: A kit of
 helpers and tools to simplify more intensive use of ViUR Home-page: https://
 github.com/viur-framework/viur-toolkit Author: Sven Eberth Author-email:
 se@mausbrand.de Maintainer: Sven Eberth Maintainer-email: se@mausbrand.de
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: MIT License Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
 Topic :: Software Development :: Libraries :: Python Modules Requires-Python:
 >=3.10 Description-Content-Type: text/markdown License-File: LICENSE Requires-
-Dist: requests Requires-Dist: Deprecated # viur-toolkit
+Dist: requests Requires-Dist: Deprecated Requires-Dist: viur-core>=3.6 # viur-
+toolkit
                        ************ vviiuurr--ttoooollkkiitt ((WWIIPP)) ************
       _[_B_a_d_g_e_ _s_h_o_w_i_n_g_ _c_u_r_r_e_n_t_ _P_y_P_I_ _v_e_r_s_i_o_n_]_[_B_a_d_g_e_ _d_i_s_p_l_a_y_i_n_g_ _t_h_e_ _l_i_c_e_n_s_e_]
        A kit of helpers and tools to simplify more intensive use of ViUR
```

### Comparing `viur_toolkit-0.1.0.dev7/setup.cfg` & `viur_toolkit-0.1.0.dev8/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -21,12 +21,13 @@
 [options]
 python_requires = >=3.10
 package_dir = 
 	= src
 install_requires = 
 	requests
 	Deprecated
+	viur-core>=3.6
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `viur_toolkit-0.1.0.dev7/src/viur/toolkit/checks.py` & `viur_toolkit-0.1.0.dev8/src/viur/toolkit/checks.py`

 * *Files identical despite different names*

### Comparing `viur_toolkit-0.1.0.dev7/src/viur/toolkit/context.py` & `viur_toolkit-0.1.0.dev8/src/viur/toolkit/context.py`

 * *Files identical despite different names*

### Comparing `viur_toolkit-0.1.0.dev7/src/viur/toolkit/db.py` & `viur_toolkit-0.1.0.dev8/src/viur/toolkit/db.py`

 * *Files identical despite different names*

### Comparing `viur_toolkit-0.1.0.dev7/src/viur/toolkit/decorators.py` & `viur_toolkit-0.1.0.dev8/src/viur/toolkit/decorators.py`

 * *Files identical despite different names*

### Comparing `viur_toolkit-0.1.0.dev7/src/viur/toolkit/property.py` & `viur_toolkit-0.1.0.dev8/src/viur/toolkit/property.py`

 * *Files identical despite different names*

### Comparing `viur_toolkit-0.1.0.dev7/src/viur/toolkit/report.py` & `viur_toolkit-0.1.0.dev8/src/viur/toolkit/report.py`

 * *Files identical despite different names*

### Comparing `viur_toolkit-0.1.0.dev7/src/viur/toolkit/viur.py` & `viur_toolkit-0.1.0.dev8/src/viur/toolkit/viur.py`

 * *Files identical despite different names*

### Comparing `viur_toolkit-0.1.0.dev7/src/viur_toolkit.egg-info/PKG-INFO` & `viur_toolkit-0.1.0.dev8/src/viur_toolkit.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: viur-toolkit
-Version: 0.1.0.dev7
+Version: 0.1.0.dev8
 Summary: A kit of helpers and tools to simplify more intensive use of ViUR
 Home-page: https://github.com/viur-framework/viur-toolkit
 Author: Sven Eberth
 Author-email: se@mausbrand.de
 Maintainer: Sven Eberth
 Maintainer-email: se@mausbrand.de
 Classifier: Intended Audience :: Developers
@@ -15,14 +15,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: Deprecated
+Requires-Dist: viur-core>=3.6
 
 # viur-toolkit
 
 <div align="center">
     <h1>viur-toolkit (WIP)</h1>
     <a href="https://pypi.org/project/viur-toolkit/">
         <img alt="Badge showing current PyPI version" title="PyPI" src="https://img.shields.io/pypi/v/viur-toolkit">
```

#### html2text {}

```diff
@@ -1,14 +1,15 @@
-Metadata-Version: 2.1 Name: viur-toolkit Version: 0.1.0.dev7 Summary: A kit of
+Metadata-Version: 2.1 Name: viur-toolkit Version: 0.1.0.dev8 Summary: A kit of
 helpers and tools to simplify more intensive use of ViUR Home-page: https://
 github.com/viur-framework/viur-toolkit Author: Sven Eberth Author-email:
 se@mausbrand.de Maintainer: Sven Eberth Maintainer-email: se@mausbrand.de
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: MIT License Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
 Topic :: Software Development :: Libraries :: Python Modules Requires-Python:
 >=3.10 Description-Content-Type: text/markdown License-File: LICENSE Requires-
-Dist: requests Requires-Dist: Deprecated # viur-toolkit
+Dist: requests Requires-Dist: Deprecated Requires-Dist: viur-core>=3.6 # viur-
+toolkit
                        ************ vviiuurr--ttoooollkkiitt ((WWIIPP)) ************
       _[_B_a_d_g_e_ _s_h_o_w_i_n_g_ _c_u_r_r_e_n_t_ _P_y_P_I_ _v_e_r_s_i_o_n_]_[_B_a_d_g_e_ _d_i_s_p_l_a_y_i_n_g_ _t_h_e_ _l_i_c_e_n_s_e_]
        A kit of helpers and tools to simplify more intensive use of ViUR
```

### Comparing `viur_toolkit-0.1.0.dev7/src/viur_toolkit.egg-info/SOURCES.txt` & `viur_toolkit-0.1.0.dev8/src/viur_toolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

