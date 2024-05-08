# Comparing `tmp/sarcharts-0.0.1.dev79.tar.gz` & `tmp/sarcharts-0.0.1.dev81.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sarcharts-0.0.1.dev79.tar", last modified: Tue May  7 14:50:51 2024, max compression
+gzip compressed data, was "sarcharts-0.0.1.dev81.tar", last modified: Wed May  8 08:32:52 2024, max compression
```

## Comparing `sarcharts-0.0.1.dev79.tar` & `sarcharts-0.0.1.dev81.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 pablofr   (1000) pablofr   (1000)        0 2024-05-07 14:50:51.758135 sarcharts-0.0.1.dev79/
-drwxr-xr-x   0 pablofr   (1000) pablofr   (1000)        0 2024-05-07 14:50:51.752135 sarcharts-0.0.1.dev79/.github/
-drwxr-xr-x   0 pablofr   (1000) pablofr   (1000)        0 2024-05-07 14:50:51.754135 sarcharts-0.0.1.dev79/.github/workflows/
--rw-r--r--   0 pablofr   (1000) pablofr   (1000)     1072 2024-05-07 13:57:28.000000 sarcharts-0.0.1.dev79/.github/workflows/python-publish.yml
--rw-r--r--   0 pablofr   (1000) pablofr   (1000)     3785 2024-05-06 13:29:25.000000 sarcharts-0.0.1.dev79/.pylintrc
--rw-r--r--   0 pablofr   (1000) pablofr   (1000)      162 2024-05-07 14:50:51.000000 sarcharts-0.0.1.dev79/AUTHORS
--rw-r--r--   0 pablofr   (1000) pablofr   (1000)     1364 2024-05-07 14:50:51.000000 sarcharts-0.0.1.dev79/ChangeLog
--rw-r--r--   0 pablofr   (1000) pablofr   (1000)    35149 2024-05-06 13:29:25.000000 sarcharts-0.0.1.dev79/LICENSE
--rw-r--r--   0 pablofr   (1000) pablofr   (1000)     1929 2024-05-07 14:50:51.758135 sarcharts-0.0.1.dev79/PKG-INFO
--rw-r--r--   0 pablofr   (1000) pablofr   (1000)     1075 2024-05-07 09:50:30.000000 sarcharts-0.0.1.dev79/README.md
-drwxr-xr-x   0 pablofr   (1000) pablofr   (1000)        0 2024-05-07 14:50:51.754135 sarcharts-0.0.1.dev79/doc/
--rw-r--r--   0 pablofr   (1000) pablofr   (1000)     1075 2024-05-07 09:50:30.000000 sarcharts-0.0.1.dev79/doc/README.md
--rw-r--r--   0 pablofr   (1000) pablofr   (1000)   137178 2024-05-06 13:29:25.000000 sarcharts-0.0.1.dev79/doc/sarcharts.png
--rw-r--r--   0 pablofr   (1000) pablofr   (1000)      294 2024-05-06 13:29:25.000000 sarcharts-0.0.1.dev79/requirements.txt
-drwxr-xr-x   0 pablofr   (1000) pablofr   (1000)        0 2024-05-07 14:50:51.754135 sarcharts-0.0.1.dev79/sarcharts/
--rw-r--r--   0 pablofr   (1000) pablofr   (1000)     3751 2024-05-07 13:57:15.000000 sarcharts-0.0.1.dev79/sarcharts/__init__.py
-drwxr-xr-x   0 pablofr   (1000) pablofr   (1000)        0 2024-05-07 14:50:51.756135 sarcharts-0.0.1.dev79/sarcharts/bin/
--rw-r--r--   0 pablofr   (1000) pablofr   (1000)        0 2024-05-07 12:04:23.000000 sarcharts-0.0.1.dev79/sarcharts/bin/__init__.py
--rwxr-xr-x   0 pablofr   (1000) pablofr   (1000)      204 2024-05-07 12:04:23.000000 sarcharts-0.0.1.dev79/sarcharts/bin/sarcharts.py
-drwxr-xr-x   0 pablofr   (1000) pablofr   (1000)        0 2024-05-07 14:50:51.752135 sarcharts-0.0.1.dev79/sarcharts/html/
-drwxr-xr-x   0 pablofr   (1000) pablofr   (1000)        0 2024-05-07 14:50:51.756135 sarcharts-0.0.1.dev79/sarcharts/html/css/
--rw-r--r--   0 pablofr   (1000) pablofr   (1000)     1034 2024-05-07 11:14:36.000000 sarcharts-0.0.1.dev79/sarcharts/html/css/sarcharts.css
-drwxr-xr-x   0 pablofr   (1000) pablofr   (1000)        0 2024-05-07 14:50:51.756135 sarcharts-0.0.1.dev79/sarcharts/html/js/
--rw-r--r--   0 pablofr   (1000) pablofr   (1000)   205214 2024-05-07 11:14:36.000000 sarcharts-0.0.1.dev79/sarcharts/html/js/chart.umd.js
--rw-r--r--   0 pablofr   (1000) pablofr   (1000)    12854 2024-05-07 11:14:36.000000 sarcharts-0.0.1.dev79/sarcharts/html/js/chartjs-plugin-zoom.min.js
--rw-r--r--   0 pablofr   (1000) pablofr   (1000)    20765 2024-05-07 11:14:36.000000 sarcharts-0.0.1.dev79/sarcharts/html/js/hammer.min.js
--rw-r--r--   0 pablofr   (1000) pablofr   (1000)   271751 2024-05-07 11:14:36.000000 sarcharts-0.0.1.dev79/sarcharts/html/js/jquery.js
-drwxr-xr-x   0 pablofr   (1000) pablofr   (1000)        0 2024-05-07 14:50:51.757135 sarcharts-0.0.1.dev79/sarcharts/lib/
--rw-r--r--   0 pablofr   (1000) pablofr   (1000)     1373 2024-05-07 11:14:36.000000 sarcharts-0.0.1.dev79/sarcharts/lib/chartjs.py
--rw-r--r--   0 pablofr   (1000) pablofr   (1000)     6983 2024-05-07 11:14:36.000000 sarcharts-0.0.1.dev79/sarcharts/lib/chartsconf.py
--rw-r--r--   0 pablofr   (1000) pablofr   (1000)     1957 2024-05-07 11:14:36.000000 sarcharts-0.0.1.dev79/sarcharts/lib/progressbar.py
--rw-r--r--   0 pablofr   (1000) pablofr   (1000)     5216 2024-05-07 11:14:36.000000 sarcharts-0.0.1.dev79/sarcharts/lib/sadf.py
--rw-r--r--   0 pablofr   (1000) pablofr   (1000)     2406 2024-05-07 13:57:15.000000 sarcharts-0.0.1.dev79/sarcharts/lib/util.py
-drwxr-xr-x   0 pablofr   (1000) pablofr   (1000)        0 2024-05-07 14:50:51.758135 sarcharts-0.0.1.dev79/sarcharts/templates/
--rw-r--r--   0 pablofr   (1000) pablofr   (1000)     2423 2024-05-07 11:14:36.000000 sarcharts-0.0.1.dev79/sarcharts/templates/chart.html
--rw-r--r--   0 pablofr   (1000) pablofr   (1000)      488 2024-05-07 11:14:36.000000 sarcharts-0.0.1.dev79/sarcharts/templates/header.html
-drwxr-xr-x   0 pablofr   (1000) pablofr   (1000)        0 2024-05-07 14:50:51.758135 sarcharts-0.0.1.dev79/sarcharts.egg-info/
--rw-r--r--   0 pablofr   (1000) pablofr   (1000)     1929 2024-05-07 14:50:51.000000 sarcharts-0.0.1.dev79/sarcharts.egg-info/PKG-INFO
--rw-r--r--   0 pablofr   (1000) pablofr   (1000)      873 2024-05-07 14:50:51.000000 sarcharts-0.0.1.dev79/sarcharts.egg-info/SOURCES.txt
--rw-r--r--   0 pablofr   (1000) pablofr   (1000)        1 2024-05-07 14:50:51.000000 sarcharts-0.0.1.dev79/sarcharts.egg-info/dependency_links.txt
--rw-r--r--   0 pablofr   (1000) pablofr   (1000)       59 2024-05-07 14:50:51.000000 sarcharts-0.0.1.dev79/sarcharts.egg-info/entry_points.txt
--rw-r--r--   0 pablofr   (1000) pablofr   (1000)        1 2024-05-07 10:10:55.000000 sarcharts-0.0.1.dev79/sarcharts.egg-info/not-zip-safe
--rw-r--r--   0 pablofr   (1000) pablofr   (1000)       47 2024-05-07 14:50:51.000000 sarcharts-0.0.1.dev79/sarcharts.egg-info/pbr.json
--rw-r--r--   0 pablofr   (1000) pablofr   (1000)       25 2024-05-07 14:50:51.000000 sarcharts-0.0.1.dev79/sarcharts.egg-info/requires.txt
--rw-r--r--   0 pablofr   (1000) pablofr   (1000)       10 2024-05-07 14:50:51.000000 sarcharts-0.0.1.dev79/sarcharts.egg-info/top_level.txt
--rw-r--r--   0 pablofr   (1000) pablofr   (1000)      769 2024-05-07 14:50:51.759135 sarcharts-0.0.1.dev79/setup.cfg
--rw-r--r--   0 pablofr   (1000) pablofr   (1000)      896 2024-05-07 14:50:46.000000 sarcharts-0.0.1.dev79/setup.py
--rw-r--r--   0 pablofr   (1000) pablofr   (1000)      246 2024-05-06 13:29:25.000000 sarcharts-0.0.1.dev79/test-requirements.txt
--rw-r--r--   0 pablofr   (1000) pablofr   (1000)      787 2024-05-06 13:29:25.000000 sarcharts-0.0.1.dev79/tox.ini
+drwxr-xr-x   0 pablofr   (1000) pablofr   (1000)        0 2024-05-08 08:32:52.520009 sarcharts-0.0.1.dev81/
+drwxr-xr-x   0 pablofr   (1000) pablofr   (1000)        0 2024-05-08 08:32:52.513008 sarcharts-0.0.1.dev81/.github/
+drwxr-xr-x   0 pablofr   (1000) pablofr   (1000)        0 2024-05-08 08:32:52.515009 sarcharts-0.0.1.dev81/.github/workflows/
+-rw-r--r--   0 pablofr   (1000) pablofr   (1000)     1072 2024-05-07 13:57:28.000000 sarcharts-0.0.1.dev81/.github/workflows/python-publish.yml
+-rw-r--r--   0 pablofr   (1000) pablofr   (1000)     3785 2024-05-06 13:29:25.000000 sarcharts-0.0.1.dev81/.pylintrc
+-rw-r--r--   0 pablofr   (1000) pablofr   (1000)      162 2024-05-08 08:32:52.000000 sarcharts-0.0.1.dev81/AUTHORS
+-rw-r--r--   0 pablofr   (1000) pablofr   (1000)     1413 2024-05-08 08:32:52.000000 sarcharts-0.0.1.dev81/ChangeLog
+-rw-r--r--   0 pablofr   (1000) pablofr   (1000)    35149 2024-05-06 13:29:25.000000 sarcharts-0.0.1.dev81/LICENSE
+-rw-r--r--   0 pablofr   (1000) pablofr   (1000)     1944 2024-05-08 08:32:52.520009 sarcharts-0.0.1.dev81/PKG-INFO
+-rw-r--r--   0 pablofr   (1000) pablofr   (1000)     1075 2024-05-07 09:50:30.000000 sarcharts-0.0.1.dev81/README.md
+drwxr-xr-x   0 pablofr   (1000) pablofr   (1000)        0 2024-05-08 08:32:52.516008 sarcharts-0.0.1.dev81/doc/
+-rw-r--r--   0 pablofr   (1000) pablofr   (1000)     1075 2024-05-07 09:50:30.000000 sarcharts-0.0.1.dev81/doc/README.md
+-rw-r--r--   0 pablofr   (1000) pablofr   (1000)   137178 2024-05-06 13:29:25.000000 sarcharts-0.0.1.dev81/doc/sarcharts.png
+-rw-r--r--   0 pablofr   (1000) pablofr   (1000)      294 2024-05-06 13:29:25.000000 sarcharts-0.0.1.dev81/requirements.txt
+drwxr-xr-x   0 pablofr   (1000) pablofr   (1000)        0 2024-05-08 08:32:52.516008 sarcharts-0.0.1.dev81/sarcharts/
+-rw-r--r--   0 pablofr   (1000) pablofr   (1000)     3751 2024-05-07 13:57:15.000000 sarcharts-0.0.1.dev81/sarcharts/__init__.py
+drwxr-xr-x   0 pablofr   (1000) pablofr   (1000)        0 2024-05-08 08:32:52.517009 sarcharts-0.0.1.dev81/sarcharts/bin/
+-rw-r--r--   0 pablofr   (1000) pablofr   (1000)        0 2024-05-07 12:04:23.000000 sarcharts-0.0.1.dev81/sarcharts/bin/__init__.py
+-rwxr-xr-x   0 pablofr   (1000) pablofr   (1000)      204 2024-05-07 12:04:23.000000 sarcharts-0.0.1.dev81/sarcharts/bin/sarcharts.py
+drwxr-xr-x   0 pablofr   (1000) pablofr   (1000)        0 2024-05-08 08:32:52.514009 sarcharts-0.0.1.dev81/sarcharts/html/
+drwxr-xr-x   0 pablofr   (1000) pablofr   (1000)        0 2024-05-08 08:32:52.518009 sarcharts-0.0.1.dev81/sarcharts/html/css/
+-rw-r--r--   0 pablofr   (1000) pablofr   (1000)     1034 2024-05-07 11:14:36.000000 sarcharts-0.0.1.dev81/sarcharts/html/css/sarcharts.css
+drwxr-xr-x   0 pablofr   (1000) pablofr   (1000)        0 2024-05-08 08:32:52.518009 sarcharts-0.0.1.dev81/sarcharts/html/js/
+-rw-r--r--   0 pablofr   (1000) pablofr   (1000)   205214 2024-05-07 11:14:36.000000 sarcharts-0.0.1.dev81/sarcharts/html/js/chart.umd.js
+-rw-r--r--   0 pablofr   (1000) pablofr   (1000)    12854 2024-05-07 11:14:36.000000 sarcharts-0.0.1.dev81/sarcharts/html/js/chartjs-plugin-zoom.min.js
+-rw-r--r--   0 pablofr   (1000) pablofr   (1000)    20765 2024-05-07 11:14:36.000000 sarcharts-0.0.1.dev81/sarcharts/html/js/hammer.min.js
+-rw-r--r--   0 pablofr   (1000) pablofr   (1000)   271751 2024-05-07 11:14:36.000000 sarcharts-0.0.1.dev81/sarcharts/html/js/jquery.js
+drwxr-xr-x   0 pablofr   (1000) pablofr   (1000)        0 2024-05-08 08:32:52.519008 sarcharts-0.0.1.dev81/sarcharts/lib/
+-rw-r--r--   0 pablofr   (1000) pablofr   (1000)     1373 2024-05-07 11:14:36.000000 sarcharts-0.0.1.dev81/sarcharts/lib/chartjs.py
+-rw-r--r--   0 pablofr   (1000) pablofr   (1000)     6983 2024-05-07 11:14:36.000000 sarcharts-0.0.1.dev81/sarcharts/lib/chartsconf.py
+-rw-r--r--   0 pablofr   (1000) pablofr   (1000)     1957 2024-05-07 11:14:36.000000 sarcharts-0.0.1.dev81/sarcharts/lib/progressbar.py
+-rw-r--r--   0 pablofr   (1000) pablofr   (1000)     5216 2024-05-07 11:14:36.000000 sarcharts-0.0.1.dev81/sarcharts/lib/sadf.py
+-rw-r--r--   0 pablofr   (1000) pablofr   (1000)     2406 2024-05-07 13:57:15.000000 sarcharts-0.0.1.dev81/sarcharts/lib/util.py
+drwxr-xr-x   0 pablofr   (1000) pablofr   (1000)        0 2024-05-08 08:32:52.519008 sarcharts-0.0.1.dev81/sarcharts/templates/
+-rw-r--r--   0 pablofr   (1000) pablofr   (1000)     2423 2024-05-07 11:14:36.000000 sarcharts-0.0.1.dev81/sarcharts/templates/chart.html
+-rw-r--r--   0 pablofr   (1000) pablofr   (1000)      488 2024-05-07 11:14:36.000000 sarcharts-0.0.1.dev81/sarcharts/templates/header.html
+drwxr-xr-x   0 pablofr   (1000) pablofr   (1000)        0 2024-05-08 08:32:52.520009 sarcharts-0.0.1.dev81/sarcharts.egg-info/
+-rw-r--r--   0 pablofr   (1000) pablofr   (1000)     1944 2024-05-08 08:32:52.000000 sarcharts-0.0.1.dev81/sarcharts.egg-info/PKG-INFO
+-rw-r--r--   0 pablofr   (1000) pablofr   (1000)      873 2024-05-08 08:32:52.000000 sarcharts-0.0.1.dev81/sarcharts.egg-info/SOURCES.txt
+-rw-r--r--   0 pablofr   (1000) pablofr   (1000)        1 2024-05-08 08:32:52.000000 sarcharts-0.0.1.dev81/sarcharts.egg-info/dependency_links.txt
+-rw-r--r--   0 pablofr   (1000) pablofr   (1000)       59 2024-05-08 08:32:52.000000 sarcharts-0.0.1.dev81/sarcharts.egg-info/entry_points.txt
+-rw-r--r--   0 pablofr   (1000) pablofr   (1000)        1 2024-05-07 10:10:55.000000 sarcharts-0.0.1.dev81/sarcharts.egg-info/not-zip-safe
+-rw-r--r--   0 pablofr   (1000) pablofr   (1000)       47 2024-05-08 08:32:52.000000 sarcharts-0.0.1.dev81/sarcharts.egg-info/pbr.json
+-rw-r--r--   0 pablofr   (1000) pablofr   (1000)       25 2024-05-08 08:32:52.000000 sarcharts-0.0.1.dev81/sarcharts.egg-info/requires.txt
+-rw-r--r--   0 pablofr   (1000) pablofr   (1000)       10 2024-05-08 08:32:52.000000 sarcharts-0.0.1.dev81/sarcharts.egg-info/top_level.txt
+-rw-r--r--   0 pablofr   (1000) pablofr   (1000)      784 2024-05-08 08:32:52.521009 sarcharts-0.0.1.dev81/setup.cfg
+-rw-r--r--   0 pablofr   (1000) pablofr   (1000)      917 2024-05-08 08:24:35.000000 sarcharts-0.0.1.dev81/setup.py
+-rw-r--r--   0 pablofr   (1000) pablofr   (1000)      246 2024-05-06 13:29:25.000000 sarcharts-0.0.1.dev81/test-requirements.txt
+-rw-r--r--   0 pablofr   (1000) pablofr   (1000)      787 2024-05-06 13:29:25.000000 sarcharts-0.0.1.dev81/tox.ini
```

### Comparing `sarcharts-0.0.1.dev79/.github/workflows/python-publish.yml` & `sarcharts-0.0.1.dev81/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `sarcharts-0.0.1.dev79/.pylintrc` & `sarcharts-0.0.1.dev81/.pylintrc`

 * *Files identical despite different names*

### Comparing `sarcharts-0.0.1.dev79/ChangeLog` & `sarcharts-0.0.1.dev81/ChangeLog`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 CHANGES
 =======
 
+* Change package license and fix author lastname
 * cli enhacements
 * Create python-publish.yml
 * package generation fixes
 * minor fixes
 * update README
 * Added ProgressBar and update README
 * sort data by field datetime instead of sa file mtime
```

### Comparing `sarcharts-0.0.1.dev79/LICENSE` & `sarcharts-0.0.1.dev81/LICENSE`

 * *Files identical despite different names*

### Comparing `sarcharts-0.0.1.dev79/PKG-INFO` & `sarcharts-0.0.1.dev81/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: sarcharts
-Version: 0.0.1.dev79
+Version: 0.0.1.dev81
 Summary: Generates Charts from sar files using Chart.js
 Home-page: https://github.com/pafernanr/sarcharts
-Author: Pablo Ferández Rodríguez
+Author: Pablo Fernández Rodríguez
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
-Classifier: License :: OSI Approved :: Apache Software License
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `sarcharts-0.0.1.dev79/README.md` & `sarcharts-0.0.1.dev81/README.md`

 * *Files identical despite different names*

### Comparing `sarcharts-0.0.1.dev79/doc/README.md` & `sarcharts-0.0.1.dev81/doc/README.md`

 * *Files identical despite different names*

### Comparing `sarcharts-0.0.1.dev79/doc/sarcharts.png` & `sarcharts-0.0.1.dev81/doc/sarcharts.png`

 * *Files identical despite different names*

### Comparing `sarcharts-0.0.1.dev79/sarcharts/__init__.py` & `sarcharts-0.0.1.dev81/sarcharts/__init__.py`

 * *Files identical despite different names*

### Comparing `sarcharts-0.0.1.dev79/sarcharts/html/css/sarcharts.css` & `sarcharts-0.0.1.dev81/sarcharts/html/css/sarcharts.css`

 * *Files identical despite different names*

### Comparing `sarcharts-0.0.1.dev79/sarcharts/html/js/chart.umd.js` & `sarcharts-0.0.1.dev81/sarcharts/html/js/chart.umd.js`

 * *Files identical despite different names*

### Comparing `sarcharts-0.0.1.dev79/sarcharts/html/js/chartjs-plugin-zoom.min.js` & `sarcharts-0.0.1.dev81/sarcharts/html/js/chartjs-plugin-zoom.min.js`

 * *Files identical despite different names*

### Comparing `sarcharts-0.0.1.dev79/sarcharts/html/js/hammer.min.js` & `sarcharts-0.0.1.dev81/sarcharts/html/js/hammer.min.js`

 * *Files identical despite different names*

### Comparing `sarcharts-0.0.1.dev79/sarcharts/html/js/jquery.js` & `sarcharts-0.0.1.dev81/sarcharts/html/js/jquery.js`

 * *Files identical despite different names*

### Comparing `sarcharts-0.0.1.dev79/sarcharts/lib/chartjs.py` & `sarcharts-0.0.1.dev81/sarcharts/lib/chartjs.py`

 * *Files identical despite different names*

### Comparing `sarcharts-0.0.1.dev79/sarcharts/lib/chartsconf.py` & `sarcharts-0.0.1.dev81/sarcharts/lib/chartsconf.py`

 * *Files identical despite different names*

### Comparing `sarcharts-0.0.1.dev79/sarcharts/lib/progressbar.py` & `sarcharts-0.0.1.dev81/sarcharts/lib/progressbar.py`

 * *Files identical despite different names*

### Comparing `sarcharts-0.0.1.dev79/sarcharts/lib/sadf.py` & `sarcharts-0.0.1.dev81/sarcharts/lib/sadf.py`

 * *Files identical despite different names*

### Comparing `sarcharts-0.0.1.dev79/sarcharts/lib/util.py` & `sarcharts-0.0.1.dev81/sarcharts/lib/util.py`

 * *Files identical despite different names*

### Comparing `sarcharts-0.0.1.dev79/sarcharts/templates/chart.html` & `sarcharts-0.0.1.dev81/sarcharts/templates/chart.html`

 * *Files identical despite different names*

### Comparing `sarcharts-0.0.1.dev79/sarcharts.egg-info/PKG-INFO` & `sarcharts-0.0.1.dev81/sarcharts.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: sarcharts
-Version: 0.0.1.dev79
+Version: 0.0.1.dev81
 Summary: Generates Charts from sar files using Chart.js
 Home-page: https://github.com/pafernanr/sarcharts
-Author: Pablo Ferández Rodríguez
+Author: Pablo Fernández Rodríguez
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
-Classifier: License :: OSI Approved :: Apache Software License
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `sarcharts-0.0.1.dev79/sarcharts.egg-info/SOURCES.txt` & `sarcharts-0.0.1.dev81/sarcharts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sarcharts-0.0.1.dev79/setup.cfg` & `sarcharts-0.0.1.dev81/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [metadata]
 name = sarcharts
 summary = Generates Charts from sar files using Chart.js
 description_file = 
 	README.md
-author = Pablo Ferández Rodríguez
+author = Pablo Fernández Rodríguez
 home_page = https://github.com/pafernanr/sarcharts
 classifier = 
 	Intended Audience :: Information Technology
 	Intended Audience :: System Administrators
-	License :: OSI Approved :: Apache Software License
+	License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 	Operating System :: POSIX :: Linux
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
```

### Comparing `sarcharts-0.0.1.dev79/setup.py` & `sarcharts-0.0.1.dev81/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,11 +12,12 @@
 # implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import setuptools
 
 setuptools.setup(
+    version="0.0.2",
     setup_requires=['pbr>=2.0.0'],
     long_description="SarCharts gets [sysstat](https://sysstat.github.io/) files from provided `sarfilespaths` and generates dynamic HTML Charts.",
     long_description_content_type='text/markdown',
     pbr=True)
```

### Comparing `sarcharts-0.0.1.dev79/tox.ini` & `sarcharts-0.0.1.dev81/tox.ini`

 * *Files identical despite different names*

