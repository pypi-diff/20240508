# Comparing `tmp/sarcharts-0.0.1.dev83.tar.gz` & `tmp/sarcharts-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sarcharts-0.0.1.dev83.tar", last modified: Wed May  8 08:52:33 2024, max compression
+gzip compressed data, was "sarcharts-0.1.0.tar", last modified: Wed May  8 09:13:14 2024, max compression
```

## Comparing `sarcharts-0.0.1.dev83.tar` & `sarcharts-0.1.0.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 pablofr   (1000) pablofr   (1000)        0 2024-05-08 08:52:33.392340 sarcharts-0.0.1.dev83/
-drwxr-xr-x   0 pablofr   (1000) pablofr   (1000)        0 2024-05-08 08:52:33.383340 sarcharts-0.0.1.dev83/.github/
-drwxr-xr-x   0 pablofr   (1000) pablofr   (1000)        0 2024-05-08 08:52:33.386340 sarcharts-0.0.1.dev83/.github/workflows/
--rw-r--r--   0 pablofr   (1000) pablofr   (1000)     1072 2024-05-07 13:57:28.000000 sarcharts-0.0.1.dev83/.github/workflows/python-publish.yml
--rw-r--r--   0 pablofr   (1000) pablofr   (1000)     3785 2024-05-06 13:29:25.000000 sarcharts-0.0.1.dev83/.pylintrc
--rw-r--r--   0 pablofr   (1000) pablofr   (1000)      162 2024-05-08 08:52:33.000000 sarcharts-0.0.1.dev83/AUTHORS
--rw-r--r--   0 pablofr   (1000) pablofr   (1000)     1438 2024-05-08 08:52:33.000000 sarcharts-0.0.1.dev83/ChangeLog
--rw-r--r--   0 pablofr   (1000) pablofr   (1000)    35149 2024-05-06 13:29:25.000000 sarcharts-0.0.1.dev83/LICENSE
--rw-r--r--   0 pablofr   (1000) pablofr   (1000)     1988 2024-05-08 08:52:33.392340 sarcharts-0.0.1.dev83/PKG-INFO
--rw-r--r--   0 pablofr   (1000) pablofr   (1000)     1075 2024-05-07 09:50:30.000000 sarcharts-0.0.1.dev83/README.md
-drwxr-xr-x   0 pablofr   (1000) pablofr   (1000)        0 2024-05-08 08:52:33.386340 sarcharts-0.0.1.dev83/doc/
--rw-r--r--   0 pablofr   (1000) pablofr   (1000)     1075 2024-05-07 09:50:30.000000 sarcharts-0.0.1.dev83/doc/README.md
--rw-r--r--   0 pablofr   (1000) pablofr   (1000)   137178 2024-05-06 13:29:25.000000 sarcharts-0.0.1.dev83/doc/sarcharts.png
--rw-r--r--   0 pablofr   (1000) pablofr   (1000)      294 2024-05-06 13:29:25.000000 sarcharts-0.0.1.dev83/requirements.txt
-drwxr-xr-x   0 pablofr   (1000) pablofr   (1000)        0 2024-05-08 08:52:33.387340 sarcharts-0.0.1.dev83/sarcharts/
--rw-r--r--   0 pablofr   (1000) pablofr   (1000)     3751 2024-05-07 13:57:15.000000 sarcharts-0.0.1.dev83/sarcharts/__init__.py
-drwxr-xr-x   0 pablofr   (1000) pablofr   (1000)        0 2024-05-08 08:52:33.388340 sarcharts-0.0.1.dev83/sarcharts/bin/
--rw-r--r--   0 pablofr   (1000) pablofr   (1000)        0 2024-05-07 12:04:23.000000 sarcharts-0.0.1.dev83/sarcharts/bin/__init__.py
--rwxr-xr-x   0 pablofr   (1000) pablofr   (1000)      204 2024-05-07 12:04:23.000000 sarcharts-0.0.1.dev83/sarcharts/bin/sarcharts.py
-drwxr-xr-x   0 pablofr   (1000) pablofr   (1000)        0 2024-05-08 08:52:33.383340 sarcharts-0.0.1.dev83/sarcharts/html/
-drwxr-xr-x   0 pablofr   (1000) pablofr   (1000)        0 2024-05-08 08:52:33.388340 sarcharts-0.0.1.dev83/sarcharts/html/css/
--rw-r--r--   0 pablofr   (1000) pablofr   (1000)     1034 2024-05-07 11:14:36.000000 sarcharts-0.0.1.dev83/sarcharts/html/css/sarcharts.css
-drwxr-xr-x   0 pablofr   (1000) pablofr   (1000)        0 2024-05-08 08:52:33.390340 sarcharts-0.0.1.dev83/sarcharts/html/js/
--rw-r--r--   0 pablofr   (1000) pablofr   (1000)   205214 2024-05-07 11:14:36.000000 sarcharts-0.0.1.dev83/sarcharts/html/js/chart.umd.js
--rw-r--r--   0 pablofr   (1000) pablofr   (1000)    12854 2024-05-07 11:14:36.000000 sarcharts-0.0.1.dev83/sarcharts/html/js/chartjs-plugin-zoom.min.js
--rw-r--r--   0 pablofr   (1000) pablofr   (1000)    20765 2024-05-07 11:14:36.000000 sarcharts-0.0.1.dev83/sarcharts/html/js/hammer.min.js
--rw-r--r--   0 pablofr   (1000) pablofr   (1000)   271751 2024-05-07 11:14:36.000000 sarcharts-0.0.1.dev83/sarcharts/html/js/jquery.js
-drwxr-xr-x   0 pablofr   (1000) pablofr   (1000)        0 2024-05-08 08:52:33.391340 sarcharts-0.0.1.dev83/sarcharts/lib/
--rw-r--r--   0 pablofr   (1000) pablofr   (1000)     1373 2024-05-07 11:14:36.000000 sarcharts-0.0.1.dev83/sarcharts/lib/chartjs.py
--rw-r--r--   0 pablofr   (1000) pablofr   (1000)     6983 2024-05-07 11:14:36.000000 sarcharts-0.0.1.dev83/sarcharts/lib/chartsconf.py
--rw-r--r--   0 pablofr   (1000) pablofr   (1000)     1957 2024-05-07 11:14:36.000000 sarcharts-0.0.1.dev83/sarcharts/lib/progressbar.py
--rw-r--r--   0 pablofr   (1000) pablofr   (1000)     5216 2024-05-07 11:14:36.000000 sarcharts-0.0.1.dev83/sarcharts/lib/sadf.py
--rw-r--r--   0 pablofr   (1000) pablofr   (1000)     2406 2024-05-07 13:57:15.000000 sarcharts-0.0.1.dev83/sarcharts/lib/util.py
-drwxr-xr-x   0 pablofr   (1000) pablofr   (1000)        0 2024-05-08 08:52:33.391340 sarcharts-0.0.1.dev83/sarcharts/templates/
--rw-r--r--   0 pablofr   (1000) pablofr   (1000)     2423 2024-05-07 11:14:36.000000 sarcharts-0.0.1.dev83/sarcharts/templates/chart.html
--rw-r--r--   0 pablofr   (1000) pablofr   (1000)      488 2024-05-07 11:14:36.000000 sarcharts-0.0.1.dev83/sarcharts/templates/header.html
-drwxr-xr-x   0 pablofr   (1000) pablofr   (1000)        0 2024-05-08 08:52:33.391340 sarcharts-0.0.1.dev83/sarcharts.egg-info/
--rw-r--r--   0 pablofr   (1000) pablofr   (1000)     1988 2024-05-08 08:52:33.000000 sarcharts-0.0.1.dev83/sarcharts.egg-info/PKG-INFO
--rw-r--r--   0 pablofr   (1000) pablofr   (1000)      873 2024-05-08 08:52:33.000000 sarcharts-0.0.1.dev83/sarcharts.egg-info/SOURCES.txt
--rw-r--r--   0 pablofr   (1000) pablofr   (1000)        1 2024-05-08 08:52:33.000000 sarcharts-0.0.1.dev83/sarcharts.egg-info/dependency_links.txt
--rw-r--r--   0 pablofr   (1000) pablofr   (1000)       59 2024-05-08 08:52:33.000000 sarcharts-0.0.1.dev83/sarcharts.egg-info/entry_points.txt
--rw-r--r--   0 pablofr   (1000) pablofr   (1000)        1 2024-05-07 10:10:55.000000 sarcharts-0.0.1.dev83/sarcharts.egg-info/not-zip-safe
--rw-r--r--   0 pablofr   (1000) pablofr   (1000)       47 2024-05-08 08:52:33.000000 sarcharts-0.0.1.dev83/sarcharts.egg-info/pbr.json
--rw-r--r--   0 pablofr   (1000) pablofr   (1000)       25 2024-05-08 08:52:33.000000 sarcharts-0.0.1.dev83/sarcharts.egg-info/requires.txt
--rw-r--r--   0 pablofr   (1000) pablofr   (1000)       10 2024-05-08 08:52:33.000000 sarcharts-0.0.1.dev83/sarcharts.egg-info/top_level.txt
--rw-r--r--   0 pablofr   (1000) pablofr   (1000)      828 2024-05-08 08:52:33.393340 sarcharts-0.0.1.dev83/setup.cfg
--rw-r--r--   0 pablofr   (1000) pablofr   (1000)      917 2024-05-08 08:24:35.000000 sarcharts-0.0.1.dev83/setup.py
--rw-r--r--   0 pablofr   (1000) pablofr   (1000)      246 2024-05-06 13:29:25.000000 sarcharts-0.0.1.dev83/test-requirements.txt
--rw-r--r--   0 pablofr   (1000) pablofr   (1000)      787 2024-05-06 13:29:25.000000 sarcharts-0.0.1.dev83/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:13:14.601783 sarcharts-0.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:13:14.593783 sarcharts-0.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:13:14.597783 sarcharts-0.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-08 09:13:03.000000 sarcharts-0.1.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3785 2024-05-08 09:13:03.000000 sarcharts-0.1.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-08 09:13:14.000000 sarcharts-0.1.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-08 09:13:14.000000 sarcharts-0.1.0/ChangeLog
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-08 09:13:03.000000 sarcharts-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-05-08 09:13:14.601783 sarcharts-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-08 09:13:03.000000 sarcharts-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:13:14.597783 sarcharts-0.1.0/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-08 09:13:03.000000 sarcharts-0.1.0/doc/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)   137178 2024-05-08 09:13:03.000000 sarcharts-0.1.0/doc/sarcharts.png
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-08 09:13:03.000000 sarcharts-0.1.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:13:14.597783 sarcharts-0.1.0/sarcharts/
+-rw-r--r--   0 runner    (1001) docker     (127)     3751 2024-05-08 09:13:03.000000 sarcharts-0.1.0/sarcharts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:13:14.597783 sarcharts-0.1.0/sarcharts/bin/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 09:13:03.000000 sarcharts-0.1.0/sarcharts/bin/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      204 2024-05-08 09:13:03.000000 sarcharts-0.1.0/sarcharts/bin/sarcharts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:13:14.593783 sarcharts-0.1.0/sarcharts/html/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:13:14.597783 sarcharts-0.1.0/sarcharts/html/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-08 09:13:03.000000 sarcharts-0.1.0/sarcharts/html/css/sarcharts.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:13:14.601783 sarcharts-0.1.0/sarcharts/html/js/
+-rw-r--r--   0 runner    (1001) docker     (127)   205214 2024-05-08 09:13:03.000000 sarcharts-0.1.0/sarcharts/html/js/chart.umd.js
+-rw-r--r--   0 runner    (1001) docker     (127)    12854 2024-05-08 09:13:03.000000 sarcharts-0.1.0/sarcharts/html/js/chartjs-plugin-zoom.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    20765 2024-05-08 09:13:03.000000 sarcharts-0.1.0/sarcharts/html/js/hammer.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)   271751 2024-05-08 09:13:03.000000 sarcharts-0.1.0/sarcharts/html/js/jquery.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:13:14.601783 sarcharts-0.1.0/sarcharts/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-08 09:13:03.000000 sarcharts-0.1.0/sarcharts/lib/chartjs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6983 2024-05-08 09:13:03.000000 sarcharts-0.1.0/sarcharts/lib/chartsconf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-05-08 09:13:03.000000 sarcharts-0.1.0/sarcharts/lib/progressbar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5216 2024-05-08 09:13:03.000000 sarcharts-0.1.0/sarcharts/lib/sadf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2406 2024-05-08 09:13:03.000000 sarcharts-0.1.0/sarcharts/lib/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:13:14.601783 sarcharts-0.1.0/sarcharts/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-05-08 09:13:03.000000 sarcharts-0.1.0/sarcharts/templates/chart.html
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-08 09:13:03.000000 sarcharts-0.1.0/sarcharts/templates/header.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:13:14.601783 sarcharts-0.1.0/sarcharts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-05-08 09:13:14.000000 sarcharts-0.1.0/sarcharts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-05-08 09:13:14.000000 sarcharts-0.1.0/sarcharts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 09:13:14.000000 sarcharts-0.1.0/sarcharts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-08 09:13:14.000000 sarcharts-0.1.0/sarcharts.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 09:13:14.000000 sarcharts-0.1.0/sarcharts.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-08 09:13:14.000000 sarcharts-0.1.0/sarcharts.egg-info/pbr.json
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-08 09:13:14.000000 sarcharts-0.1.0/sarcharts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-08 09:13:14.000000 sarcharts-0.1.0/sarcharts.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-08 09:13:14.601783 sarcharts-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-08 09:13:03.000000 sarcharts-0.1.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-08 09:13:03.000000 sarcharts-0.1.0/test-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-05-08 09:13:03.000000 sarcharts-0.1.0/tox.ini
```

### Comparing `sarcharts-0.0.1.dev83/.github/workflows/python-publish.yml` & `sarcharts-0.1.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `sarcharts-0.0.1.dev83/.pylintrc` & `sarcharts-0.1.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `sarcharts-0.0.1.dev83/LICENSE` & `sarcharts-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sarcharts-0.0.1.dev83/PKG-INFO` & `sarcharts-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sarcharts
-Version: 0.0.1.dev83
+Version: 0.1.0
 Summary: SarCharts gets sysstat files from provided sarfilespaths and generates dynamic HTML Charts
 Home-page: https://github.com/pafernanr/sarcharts
 Author: Pablo Fernández Rodríguez
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `sarcharts-0.0.1.dev83/README.md` & `sarcharts-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `sarcharts-0.0.1.dev83/doc/README.md` & `sarcharts-0.1.0/doc/README.md`

 * *Files identical despite different names*

### Comparing `sarcharts-0.0.1.dev83/doc/sarcharts.png` & `sarcharts-0.1.0/doc/sarcharts.png`

 * *Files identical despite different names*

### Comparing `sarcharts-0.0.1.dev83/sarcharts/__init__.py` & `sarcharts-0.1.0/sarcharts/__init__.py`

 * *Files identical despite different names*

### Comparing `sarcharts-0.0.1.dev83/sarcharts/html/css/sarcharts.css` & `sarcharts-0.1.0/sarcharts/html/css/sarcharts.css`

 * *Files identical despite different names*

### Comparing `sarcharts-0.0.1.dev83/sarcharts/html/js/chart.umd.js` & `sarcharts-0.1.0/sarcharts/html/js/chart.umd.js`

 * *Files identical despite different names*

### Comparing `sarcharts-0.0.1.dev83/sarcharts/html/js/chartjs-plugin-zoom.min.js` & `sarcharts-0.1.0/sarcharts/html/js/chartjs-plugin-zoom.min.js`

 * *Files identical despite different names*

### Comparing `sarcharts-0.0.1.dev83/sarcharts/html/js/hammer.min.js` & `sarcharts-0.1.0/sarcharts/html/js/hammer.min.js`

 * *Files identical despite different names*

### Comparing `sarcharts-0.0.1.dev83/sarcharts/html/js/jquery.js` & `sarcharts-0.1.0/sarcharts/html/js/jquery.js`

 * *Files identical despite different names*

### Comparing `sarcharts-0.0.1.dev83/sarcharts/lib/chartjs.py` & `sarcharts-0.1.0/sarcharts/lib/chartjs.py`

 * *Files identical despite different names*

### Comparing `sarcharts-0.0.1.dev83/sarcharts/lib/chartsconf.py` & `sarcharts-0.1.0/sarcharts/lib/chartsconf.py`

 * *Files identical despite different names*

### Comparing `sarcharts-0.0.1.dev83/sarcharts/lib/progressbar.py` & `sarcharts-0.1.0/sarcharts/lib/progressbar.py`

 * *Files identical despite different names*

### Comparing `sarcharts-0.0.1.dev83/sarcharts/lib/sadf.py` & `sarcharts-0.1.0/sarcharts/lib/sadf.py`

 * *Files identical despite different names*

### Comparing `sarcharts-0.0.1.dev83/sarcharts/lib/util.py` & `sarcharts-0.1.0/sarcharts/lib/util.py`

 * *Files identical despite different names*

### Comparing `sarcharts-0.0.1.dev83/sarcharts/templates/chart.html` & `sarcharts-0.1.0/sarcharts/templates/chart.html`

 * *Files identical despite different names*

### Comparing `sarcharts-0.0.1.dev83/sarcharts.egg-info/PKG-INFO` & `sarcharts-0.1.0/sarcharts.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sarcharts
-Version: 0.0.1.dev83
+Version: 0.1.0
 Summary: SarCharts gets sysstat files from provided sarfilespaths and generates dynamic HTML Charts
 Home-page: https://github.com/pafernanr/sarcharts
 Author: Pablo Fernández Rodríguez
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `sarcharts-0.0.1.dev83/sarcharts.egg-info/SOURCES.txt` & `sarcharts-0.1.0/sarcharts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sarcharts-0.0.1.dev83/setup.cfg` & `sarcharts-0.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `sarcharts-0.0.1.dev83/setup.py` & `sarcharts-0.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `sarcharts-0.0.1.dev83/tox.ini` & `sarcharts-0.1.0/tox.ini`

 * *Files identical despite different names*

