# Comparing `tmp/sarcharts-0.1.4.tar.gz` & `tmp/sarcharts-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sarcharts-0.1.4.tar", last modified: Wed May  8 14:23:40 2024, max compression
+gzip compressed data, was "sarcharts-0.1.5.tar", last modified: Wed May  8 15:02:12 2024, max compression
```

## Comparing `sarcharts-0.1.4.tar` & `sarcharts-0.1.5.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:23:40.823120 sarcharts-0.1.4/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:23:40.815120 sarcharts-0.1.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:23:40.819120 sarcharts-0.1.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-08 14:23:35.000000 sarcharts-0.1.4/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3785 2024-05-08 14:23:35.000000 sarcharts-0.1.4/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-08 14:23:40.000000 sarcharts-0.1.4/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-08 14:23:40.000000 sarcharts-0.1.4/ChangeLog
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-08 14:23:35.000000 sarcharts-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-05-08 14:23:40.823120 sarcharts-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-08 14:23:35.000000 sarcharts-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:23:40.819120 sarcharts-0.1.4/doc/
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-08 14:23:35.000000 sarcharts-0.1.4/doc/README.md
--rw-r--r--   0 runner    (1001) docker     (127)   137178 2024-05-08 14:23:35.000000 sarcharts-0.1.4/doc/sarcharts.png
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-08 14:23:35.000000 sarcharts-0.1.4/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:23:40.819120 sarcharts-0.1.4/sarcharts/
--rw-r--r--   0 runner    (1001) docker     (127)     3751 2024-05-08 14:23:35.000000 sarcharts-0.1.4/sarcharts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:23:40.823120 sarcharts-0.1.4/sarcharts/bin/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 14:23:35.000000 sarcharts-0.1.4/sarcharts/bin/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      204 2024-05-08 14:23:35.000000 sarcharts-0.1.4/sarcharts/bin/sarcharts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:23:40.815120 sarcharts-0.1.4/sarcharts/html/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:23:40.823120 sarcharts-0.1.4/sarcharts/html/css/
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-08 14:23:35.000000 sarcharts-0.1.4/sarcharts/html/css/sarcharts.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:23:40.823120 sarcharts-0.1.4/sarcharts/html/js/
--rw-r--r--   0 runner    (1001) docker     (127)   205214 2024-05-08 14:23:35.000000 sarcharts-0.1.4/sarcharts/html/js/chart.umd.js
--rw-r--r--   0 runner    (1001) docker     (127)    12854 2024-05-08 14:23:35.000000 sarcharts-0.1.4/sarcharts/html/js/chartjs-plugin-zoom.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    20765 2024-05-08 14:23:35.000000 sarcharts-0.1.4/sarcharts/html/js/hammer.min.js
--rw-r--r--   0 runner    (1001) docker     (127)   271751 2024-05-08 14:23:35.000000 sarcharts-0.1.4/sarcharts/html/js/jquery.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:23:40.823120 sarcharts-0.1.4/sarcharts/lib/
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-08 14:23:35.000000 sarcharts-0.1.4/sarcharts/lib/chartjs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6983 2024-05-08 14:23:35.000000 sarcharts-0.1.4/sarcharts/lib/chartsconf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-05-08 14:23:35.000000 sarcharts-0.1.4/sarcharts/lib/progressbar.py
--rw-r--r--   0 runner    (1001) docker     (127)     5143 2024-05-08 14:23:35.000000 sarcharts-0.1.4/sarcharts/lib/sadf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-05-08 14:23:35.000000 sarcharts-0.1.4/sarcharts/lib/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:23:40.823120 sarcharts-0.1.4/sarcharts/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-05-08 14:23:35.000000 sarcharts-0.1.4/sarcharts/templates/chart.html
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-08 14:23:35.000000 sarcharts-0.1.4/sarcharts/templates/header.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:23:40.823120 sarcharts-0.1.4/sarcharts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-05-08 14:23:40.000000 sarcharts-0.1.4/sarcharts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      873 2024-05-08 14:23:40.000000 sarcharts-0.1.4/sarcharts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 14:23:40.000000 sarcharts-0.1.4/sarcharts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-08 14:23:40.000000 sarcharts-0.1.4/sarcharts.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 14:23:40.000000 sarcharts-0.1.4/sarcharts.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-08 14:23:40.000000 sarcharts-0.1.4/sarcharts.egg-info/pbr.json
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-08 14:23:40.000000 sarcharts-0.1.4/sarcharts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-08 14:23:40.000000 sarcharts-0.1.4/sarcharts.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-08 14:23:40.827120 sarcharts-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-08 14:23:35.000000 sarcharts-0.1.4/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-08 14:23:35.000000 sarcharts-0.1.4/test-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      787 2024-05-08 14:23:35.000000 sarcharts-0.1.4/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:02:12.836882 sarcharts-0.1.5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:02:12.828882 sarcharts-0.1.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:02:12.828882 sarcharts-0.1.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-08 15:02:07.000000 sarcharts-0.1.5/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3785 2024-05-08 15:02:07.000000 sarcharts-0.1.5/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-08 15:02:12.000000 sarcharts-0.1.5/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-08 15:02:12.000000 sarcharts-0.1.5/ChangeLog
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-08 15:02:07.000000 sarcharts-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-05-08 15:02:12.836882 sarcharts-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-08 15:02:07.000000 sarcharts-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:02:12.828882 sarcharts-0.1.5/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-08 15:02:07.000000 sarcharts-0.1.5/doc/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)   137178 2024-05-08 15:02:07.000000 sarcharts-0.1.5/doc/sarcharts.png
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-08 15:02:07.000000 sarcharts-0.1.5/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:02:12.832882 sarcharts-0.1.5/sarcharts/
+-rw-r--r--   0 runner    (1001) docker     (127)     3751 2024-05-08 15:02:07.000000 sarcharts-0.1.5/sarcharts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:02:12.832882 sarcharts-0.1.5/sarcharts/bin/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 15:02:07.000000 sarcharts-0.1.5/sarcharts/bin/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      204 2024-05-08 15:02:07.000000 sarcharts-0.1.5/sarcharts/bin/sarcharts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:02:12.828882 sarcharts-0.1.5/sarcharts/html/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:02:12.832882 sarcharts-0.1.5/sarcharts/html/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-08 15:02:07.000000 sarcharts-0.1.5/sarcharts/html/css/sarcharts.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:02:12.832882 sarcharts-0.1.5/sarcharts/html/js/
+-rw-r--r--   0 runner    (1001) docker     (127)   205214 2024-05-08 15:02:07.000000 sarcharts-0.1.5/sarcharts/html/js/chart.umd.js
+-rw-r--r--   0 runner    (1001) docker     (127)    12854 2024-05-08 15:02:07.000000 sarcharts-0.1.5/sarcharts/html/js/chartjs-plugin-zoom.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    20765 2024-05-08 15:02:07.000000 sarcharts-0.1.5/sarcharts/html/js/hammer.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)   271751 2024-05-08 15:02:07.000000 sarcharts-0.1.5/sarcharts/html/js/jquery.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:02:12.836882 sarcharts-0.1.5/sarcharts/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-08 15:02:07.000000 sarcharts-0.1.5/sarcharts/lib/chartjs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6983 2024-05-08 15:02:07.000000 sarcharts-0.1.5/sarcharts/lib/chartsconf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-05-08 15:02:07.000000 sarcharts-0.1.5/sarcharts/lib/progressbar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5168 2024-05-08 15:02:07.000000 sarcharts-0.1.5/sarcharts/lib/sadf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-05-08 15:02:07.000000 sarcharts-0.1.5/sarcharts/lib/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:02:12.836882 sarcharts-0.1.5/sarcharts/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-05-08 15:02:07.000000 sarcharts-0.1.5/sarcharts/templates/chart.html
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-08 15:02:07.000000 sarcharts-0.1.5/sarcharts/templates/header.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:02:12.836882 sarcharts-0.1.5/sarcharts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-05-08 15:02:12.000000 sarcharts-0.1.5/sarcharts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-05-08 15:02:12.000000 sarcharts-0.1.5/sarcharts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 15:02:12.000000 sarcharts-0.1.5/sarcharts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-08 15:02:12.000000 sarcharts-0.1.5/sarcharts.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 15:02:12.000000 sarcharts-0.1.5/sarcharts.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-08 15:02:12.000000 sarcharts-0.1.5/sarcharts.egg-info/pbr.json
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-08 15:02:12.000000 sarcharts-0.1.5/sarcharts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-08 15:02:12.000000 sarcharts-0.1.5/sarcharts.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-08 15:02:12.836882 sarcharts-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-08 15:02:07.000000 sarcharts-0.1.5/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-08 15:02:07.000000 sarcharts-0.1.5/test-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-05-08 15:02:07.000000 sarcharts-0.1.5/tox.ini
```

### Comparing `sarcharts-0.1.4/.github/workflows/python-publish.yml` & `sarcharts-0.1.5/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `sarcharts-0.1.4/.pylintrc` & `sarcharts-0.1.5/.pylintrc`

 * *Files identical despite different names*

### Comparing `sarcharts-0.1.4/LICENSE` & `sarcharts-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sarcharts-0.1.4/PKG-INFO` & `sarcharts-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sarcharts
-Version: 0.1.4
+Version: 0.1.5
 Summary: SarCharts gets sysstat files from provided sarfilespaths and generates dynamic HTML Charts
 Home-page: https://github.com/pafernanr/sarcharts
 Author: Pablo Fernández Rodríguez
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `sarcharts-0.1.4/README.md` & `sarcharts-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `sarcharts-0.1.4/doc/README.md` & `sarcharts-0.1.5/doc/README.md`

 * *Files identical despite different names*

### Comparing `sarcharts-0.1.4/doc/sarcharts.png` & `sarcharts-0.1.5/doc/sarcharts.png`

 * *Files identical despite different names*

### Comparing `sarcharts-0.1.4/sarcharts/__init__.py` & `sarcharts-0.1.5/sarcharts/__init__.py`

 * *Files identical despite different names*

### Comparing `sarcharts-0.1.4/sarcharts/html/css/sarcharts.css` & `sarcharts-0.1.5/sarcharts/html/css/sarcharts.css`

 * *Files identical despite different names*

### Comparing `sarcharts-0.1.4/sarcharts/html/js/chart.umd.js` & `sarcharts-0.1.5/sarcharts/html/js/chart.umd.js`

 * *Files identical despite different names*

### Comparing `sarcharts-0.1.4/sarcharts/html/js/chartjs-plugin-zoom.min.js` & `sarcharts-0.1.5/sarcharts/html/js/chartjs-plugin-zoom.min.js`

 * *Files identical despite different names*

### Comparing `sarcharts-0.1.4/sarcharts/html/js/hammer.min.js` & `sarcharts-0.1.5/sarcharts/html/js/hammer.min.js`

 * *Files identical despite different names*

### Comparing `sarcharts-0.1.4/sarcharts/html/js/jquery.js` & `sarcharts-0.1.5/sarcharts/html/js/jquery.js`

 * *Files identical despite different names*

### Comparing `sarcharts-0.1.4/sarcharts/lib/chartjs.py` & `sarcharts-0.1.5/sarcharts/lib/chartjs.py`

 * *Files identical despite different names*

### Comparing `sarcharts-0.1.4/sarcharts/lib/chartsconf.py` & `sarcharts-0.1.5/sarcharts/lib/chartsconf.py`

 * *Files identical despite different names*

### Comparing `sarcharts-0.1.4/sarcharts/lib/progressbar.py` & `sarcharts-0.1.5/sarcharts/lib/progressbar.py`

 * *Files identical despite different names*

### Comparing `sarcharts-0.1.4/sarcharts/lib/sadf.py` & `sarcharts-0.1.5/sarcharts/lib/sadf.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,15 +38,16 @@
         for k, v in charts.items():
             content = []
             csvfile = f"{outputpath}/{k}.csv"
             out = False
             for inputfile in sarfiles:
                 pbi += 1
                 pb.print_bar(
-                    pbi, f"Get data from {inputfile.split("/")[-1]} {k}.")
+                    pbi,
+                    "Get data from " + inputfile.split("/")[-1] + " " + k)
                 out = self.sar_to_csv(inputfile, v['arg'], debuglevel)
                 if out:
                     headers = out.pop(0)
                     util.debug(debuglevel, 'D',
                                f"Merge {inputfile} to {csvfile}")
                     content = content + out
             if out:
```

### Comparing `sarcharts-0.1.4/sarcharts/lib/util.py` & `sarcharts-0.1.5/sarcharts/lib/util.py`

 * *Files identical despite different names*

### Comparing `sarcharts-0.1.4/sarcharts/templates/chart.html` & `sarcharts-0.1.5/sarcharts/templates/chart.html`

 * *Files identical despite different names*

### Comparing `sarcharts-0.1.4/sarcharts.egg-info/PKG-INFO` & `sarcharts-0.1.5/sarcharts.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sarcharts
-Version: 0.1.4
+Version: 0.1.5
 Summary: SarCharts gets sysstat files from provided sarfilespaths and generates dynamic HTML Charts
 Home-page: https://github.com/pafernanr/sarcharts
 Author: Pablo Fernández Rodríguez
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `sarcharts-0.1.4/sarcharts.egg-info/SOURCES.txt` & `sarcharts-0.1.5/sarcharts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sarcharts-0.1.4/setup.cfg` & `sarcharts-0.1.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `sarcharts-0.1.4/setup.py` & `sarcharts-0.1.5/setup.py`

 * *Files identical despite different names*

### Comparing `sarcharts-0.1.4/tox.ini` & `sarcharts-0.1.5/tox.ini`

 * *Files identical despite different names*

