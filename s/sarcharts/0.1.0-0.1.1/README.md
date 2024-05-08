# Comparing `tmp/sarcharts-0.1.0.tar.gz` & `tmp/sarcharts-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sarcharts-0.1.0.tar", last modified: Wed May  8 09:13:14 2024, max compression
+gzip compressed data, was "sarcharts-0.1.1.tar", last modified: Wed May  8 09:49:40 2024, max compression
```

## Comparing `sarcharts-0.1.0.tar` & `sarcharts-0.1.1.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:13:14.601783 sarcharts-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:13:14.593783 sarcharts-0.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:13:14.597783 sarcharts-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-08 09:13:03.000000 sarcharts-0.1.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3785 2024-05-08 09:13:03.000000 sarcharts-0.1.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-08 09:13:14.000000 sarcharts-0.1.0/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-08 09:13:14.000000 sarcharts-0.1.0/ChangeLog
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-08 09:13:03.000000 sarcharts-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-05-08 09:13:14.601783 sarcharts-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-08 09:13:03.000000 sarcharts-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:13:14.597783 sarcharts-0.1.0/doc/
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-08 09:13:03.000000 sarcharts-0.1.0/doc/README.md
--rw-r--r--   0 runner    (1001) docker     (127)   137178 2024-05-08 09:13:03.000000 sarcharts-0.1.0/doc/sarcharts.png
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-08 09:13:03.000000 sarcharts-0.1.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:13:14.597783 sarcharts-0.1.0/sarcharts/
--rw-r--r--   0 runner    (1001) docker     (127)     3751 2024-05-08 09:13:03.000000 sarcharts-0.1.0/sarcharts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:13:14.597783 sarcharts-0.1.0/sarcharts/bin/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 09:13:03.000000 sarcharts-0.1.0/sarcharts/bin/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      204 2024-05-08 09:13:03.000000 sarcharts-0.1.0/sarcharts/bin/sarcharts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:13:14.593783 sarcharts-0.1.0/sarcharts/html/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:13:14.597783 sarcharts-0.1.0/sarcharts/html/css/
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-08 09:13:03.000000 sarcharts-0.1.0/sarcharts/html/css/sarcharts.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:13:14.601783 sarcharts-0.1.0/sarcharts/html/js/
--rw-r--r--   0 runner    (1001) docker     (127)   205214 2024-05-08 09:13:03.000000 sarcharts-0.1.0/sarcharts/html/js/chart.umd.js
--rw-r--r--   0 runner    (1001) docker     (127)    12854 2024-05-08 09:13:03.000000 sarcharts-0.1.0/sarcharts/html/js/chartjs-plugin-zoom.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    20765 2024-05-08 09:13:03.000000 sarcharts-0.1.0/sarcharts/html/js/hammer.min.js
--rw-r--r--   0 runner    (1001) docker     (127)   271751 2024-05-08 09:13:03.000000 sarcharts-0.1.0/sarcharts/html/js/jquery.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:13:14.601783 sarcharts-0.1.0/sarcharts/lib/
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-08 09:13:03.000000 sarcharts-0.1.0/sarcharts/lib/chartjs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6983 2024-05-08 09:13:03.000000 sarcharts-0.1.0/sarcharts/lib/chartsconf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-05-08 09:13:03.000000 sarcharts-0.1.0/sarcharts/lib/progressbar.py
--rw-r--r--   0 runner    (1001) docker     (127)     5216 2024-05-08 09:13:03.000000 sarcharts-0.1.0/sarcharts/lib/sadf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2406 2024-05-08 09:13:03.000000 sarcharts-0.1.0/sarcharts/lib/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:13:14.601783 sarcharts-0.1.0/sarcharts/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-05-08 09:13:03.000000 sarcharts-0.1.0/sarcharts/templates/chart.html
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-08 09:13:03.000000 sarcharts-0.1.0/sarcharts/templates/header.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:13:14.601783 sarcharts-0.1.0/sarcharts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-05-08 09:13:14.000000 sarcharts-0.1.0/sarcharts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      873 2024-05-08 09:13:14.000000 sarcharts-0.1.0/sarcharts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 09:13:14.000000 sarcharts-0.1.0/sarcharts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-08 09:13:14.000000 sarcharts-0.1.0/sarcharts.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 09:13:14.000000 sarcharts-0.1.0/sarcharts.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-08 09:13:14.000000 sarcharts-0.1.0/sarcharts.egg-info/pbr.json
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-08 09:13:14.000000 sarcharts-0.1.0/sarcharts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-08 09:13:14.000000 sarcharts-0.1.0/sarcharts.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-08 09:13:14.601783 sarcharts-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-08 09:13:03.000000 sarcharts-0.1.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-08 09:13:03.000000 sarcharts-0.1.0/test-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      787 2024-05-08 09:13:03.000000 sarcharts-0.1.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:49:40.180184 sarcharts-0.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:49:40.172184 sarcharts-0.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:49:40.176184 sarcharts-0.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-08 09:49:35.000000 sarcharts-0.1.1/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3785 2024-05-08 09:49:35.000000 sarcharts-0.1.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-08 09:49:40.000000 sarcharts-0.1.1/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-08 09:49:40.000000 sarcharts-0.1.1/ChangeLog
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-08 09:49:35.000000 sarcharts-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-05-08 09:49:40.180184 sarcharts-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-08 09:49:35.000000 sarcharts-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:49:40.176184 sarcharts-0.1.1/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-08 09:49:35.000000 sarcharts-0.1.1/doc/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)   137178 2024-05-08 09:49:35.000000 sarcharts-0.1.1/doc/sarcharts.png
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-08 09:49:35.000000 sarcharts-0.1.1/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:49:40.176184 sarcharts-0.1.1/sarcharts/
+-rw-r--r--   0 runner    (1001) docker     (127)     3751 2024-05-08 09:49:35.000000 sarcharts-0.1.1/sarcharts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:49:40.176184 sarcharts-0.1.1/sarcharts/bin/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 09:49:35.000000 sarcharts-0.1.1/sarcharts/bin/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      204 2024-05-08 09:49:35.000000 sarcharts-0.1.1/sarcharts/bin/sarcharts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:49:40.172184 sarcharts-0.1.1/sarcharts/html/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:49:40.176184 sarcharts-0.1.1/sarcharts/html/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-08 09:49:35.000000 sarcharts-0.1.1/sarcharts/html/css/sarcharts.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:49:40.180184 sarcharts-0.1.1/sarcharts/html/js/
+-rw-r--r--   0 runner    (1001) docker     (127)   205214 2024-05-08 09:49:35.000000 sarcharts-0.1.1/sarcharts/html/js/chart.umd.js
+-rw-r--r--   0 runner    (1001) docker     (127)    12854 2024-05-08 09:49:35.000000 sarcharts-0.1.1/sarcharts/html/js/chartjs-plugin-zoom.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    20765 2024-05-08 09:49:35.000000 sarcharts-0.1.1/sarcharts/html/js/hammer.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)   271751 2024-05-08 09:49:35.000000 sarcharts-0.1.1/sarcharts/html/js/jquery.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:49:40.180184 sarcharts-0.1.1/sarcharts/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-08 09:49:35.000000 sarcharts-0.1.1/sarcharts/lib/chartjs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6983 2024-05-08 09:49:35.000000 sarcharts-0.1.1/sarcharts/lib/chartsconf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-05-08 09:49:35.000000 sarcharts-0.1.1/sarcharts/lib/progressbar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5215 2024-05-08 09:49:35.000000 sarcharts-0.1.1/sarcharts/lib/sadf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-05-08 09:49:35.000000 sarcharts-0.1.1/sarcharts/lib/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:49:40.180184 sarcharts-0.1.1/sarcharts/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-05-08 09:49:35.000000 sarcharts-0.1.1/sarcharts/templates/chart.html
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-08 09:49:35.000000 sarcharts-0.1.1/sarcharts/templates/header.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:49:40.180184 sarcharts-0.1.1/sarcharts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-05-08 09:49:40.000000 sarcharts-0.1.1/sarcharts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-05-08 09:49:40.000000 sarcharts-0.1.1/sarcharts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 09:49:40.000000 sarcharts-0.1.1/sarcharts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-08 09:49:40.000000 sarcharts-0.1.1/sarcharts.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 09:49:40.000000 sarcharts-0.1.1/sarcharts.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-08 09:49:40.000000 sarcharts-0.1.1/sarcharts.egg-info/pbr.json
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-08 09:49:40.000000 sarcharts-0.1.1/sarcharts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-08 09:49:40.000000 sarcharts-0.1.1/sarcharts.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-08 09:49:40.180184 sarcharts-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-08 09:49:35.000000 sarcharts-0.1.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-08 09:49:35.000000 sarcharts-0.1.1/test-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-05-08 09:49:35.000000 sarcharts-0.1.1/tox.ini
```

### Comparing `sarcharts-0.1.0/.github/workflows/python-publish.yml` & `sarcharts-0.1.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `sarcharts-0.1.0/.pylintrc` & `sarcharts-0.1.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `sarcharts-0.1.0/LICENSE` & `sarcharts-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sarcharts-0.1.0/PKG-INFO` & `sarcharts-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sarcharts
-Version: 0.1.0
+Version: 0.1.1
 Summary: SarCharts gets sysstat files from provided sarfilespaths and generates dynamic HTML Charts
 Home-page: https://github.com/pafernanr/sarcharts
 Author: Pablo Fernández Rodríguez
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `sarcharts-0.1.0/README.md` & `sarcharts-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `sarcharts-0.1.0/doc/README.md` & `sarcharts-0.1.1/doc/README.md`

 * *Files identical despite different names*

### Comparing `sarcharts-0.1.0/doc/sarcharts.png` & `sarcharts-0.1.1/doc/sarcharts.png`

 * *Files identical despite different names*

### Comparing `sarcharts-0.1.0/sarcharts/__init__.py` & `sarcharts-0.1.1/sarcharts/__init__.py`

 * *Files identical despite different names*

### Comparing `sarcharts-0.1.0/sarcharts/html/css/sarcharts.css` & `sarcharts-0.1.1/sarcharts/html/css/sarcharts.css`

 * *Files identical despite different names*

### Comparing `sarcharts-0.1.0/sarcharts/html/js/chart.umd.js` & `sarcharts-0.1.1/sarcharts/html/js/chart.umd.js`

 * *Files identical despite different names*

### Comparing `sarcharts-0.1.0/sarcharts/html/js/chartjs-plugin-zoom.min.js` & `sarcharts-0.1.1/sarcharts/html/js/chartjs-plugin-zoom.min.js`

 * *Files identical despite different names*

### Comparing `sarcharts-0.1.0/sarcharts/html/js/hammer.min.js` & `sarcharts-0.1.1/sarcharts/html/js/hammer.min.js`

 * *Files identical despite different names*

### Comparing `sarcharts-0.1.0/sarcharts/html/js/jquery.js` & `sarcharts-0.1.1/sarcharts/html/js/jquery.js`

 * *Files identical despite different names*

### Comparing `sarcharts-0.1.0/sarcharts/lib/chartjs.py` & `sarcharts-0.1.1/sarcharts/lib/chartjs.py`

 * *Files identical despite different names*

### Comparing `sarcharts-0.1.0/sarcharts/lib/chartsconf.py` & `sarcharts-0.1.1/sarcharts/lib/chartsconf.py`

 * *Files identical despite different names*

### Comparing `sarcharts-0.1.0/sarcharts/lib/progressbar.py` & `sarcharts-0.1.1/sarcharts/lib/progressbar.py`

 * *Files identical despite different names*

### Comparing `sarcharts-0.1.0/sarcharts/lib/sadf.py` & `sarcharts-0.1.1/sarcharts/lib/sadf.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from sarcharts.lib.progressbar import ProgressBar
 from sarcharts.lib import util
 
 
 class Sadf:
 
     def sar_to_csv(self, inputfile, arg, debuglevel):
-        command = f"sadf -dt {inputfile} -- {arg}"
+        command = f"sadf -d {inputfile} -- {arg}"
         [stdout, stderr] = util.exec_command(debuglevel, command)
         if stderr:
             if "Try to convert it to current format" in stderr:
                 # tf = tempfile.NamedTemporaryFile(prefix="sarcharts")
                 command = f"sadf -c {inputfile} > /tmp/sarcharts.tmp"
                 [stdout, stderr] = util.exec_command(debuglevel, command)
                 return self.sar_to_csv(
```

### Comparing `sarcharts-0.1.0/sarcharts/lib/util.py` & `sarcharts-0.1.1/sarcharts/lib/util.py`

 * *Files 4% similar despite different names*

```diff
@@ -72,22 +72,22 @@
     try:
         return datetime.datetime.strptime(s, "%Y-%m-%d %H:%M:%S")
     except ValueError:
         return False
 
 
 def is_valid_date(debuglevel, d):
-    if re.match(r'\d{4}-\d{2}-\d{2} \d{2}:\d{2}:\d{2}', d):
+    if re.match(r'\d{4}-\d{2}-\d{2} \d{2}:\d{2}:\d{2} UTC', d):
         return True
     else:
         debug(debuglevel, 'E', "ERROR: date '" + d
-              + "' doesn't match %Y-%m-%d %H:%M:%S")
+              + "' doesn't match %Y-%m-%d %H:%M:%S UTC")
 
 
 def in_date_range(debuglevel, dfrom, dto, d):
     if is_valid_date(debuglevel, d):
-        d = datetime.datetime.strptime(d, '%Y-%m-%d %H:%M:%S')
+        d = datetime.datetime.strptime(d, '%Y-%m-%d %H:%M:%S UTC')
         if dfrom and dto:
             if d >= dfrom and d <= dto:
                 return True
         else:
             return True
```

### Comparing `sarcharts-0.1.0/sarcharts/templates/chart.html` & `sarcharts-0.1.1/sarcharts/templates/chart.html`

 * *Files identical despite different names*

### Comparing `sarcharts-0.1.0/sarcharts.egg-info/PKG-INFO` & `sarcharts-0.1.1/sarcharts.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sarcharts
-Version: 0.1.0
+Version: 0.1.1
 Summary: SarCharts gets sysstat files from provided sarfilespaths and generates dynamic HTML Charts
 Home-page: https://github.com/pafernanr/sarcharts
 Author: Pablo Fernández Rodríguez
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `sarcharts-0.1.0/sarcharts.egg-info/SOURCES.txt` & `sarcharts-0.1.1/sarcharts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sarcharts-0.1.0/setup.cfg` & `sarcharts-0.1.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `sarcharts-0.1.0/setup.py` & `sarcharts-0.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `sarcharts-0.1.0/tox.ini` & `sarcharts-0.1.1/tox.ini`

 * *Files identical despite different names*

