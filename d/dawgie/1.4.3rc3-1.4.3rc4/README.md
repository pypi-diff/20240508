# Comparing `tmp/dawgie-1.4.3rc3.tar.gz` & `tmp/dawgie-1.4.3rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dawgie-1.4.3rc3.tar", last modified: Tue Apr 30 17:23:48 2024, max compression
+gzip compressed data, was "dawgie-1.4.3rc4.tar", last modified: Tue May  7 18:33:39 2024, max compression
```

## Comparing `dawgie-1.4.3rc3.tar` & `dawgie-1.4.3rc4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2024-04-30 17:23:48.070226 dawgie-1.4.3rc3/
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1615 2024-04-30 17:23:47.000000 dawgie-1.4.3rc3/LICENSE
--rw-r--r--   0 niessner  (1000) niessner  (1000)     9940 2024-04-30 17:23:48.070226 dawgie-1.4.3rc3/PKG-INFO
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     8906 2024-04-30 17:23:47.000000 dawgie-1.4.3rc3/README.md
-drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2024-04-30 17:23:48.066226 dawgie-1.4.3rc3/dawgie.egg-info/
--rw-r--r--   0 niessner  (1000) niessner  (1000)     9940 2024-04-30 17:23:48.000000 dawgie-1.4.3rc3/dawgie.egg-info/PKG-INFO
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     6632 2024-04-30 17:23:48.000000 dawgie-1.4.3rc3/dawgie.egg-info/SOURCES.txt
--rw-rw-r--   0 niessner  (1000) niessner  (1000)        1 2024-04-30 17:23:48.000000 dawgie-1.4.3rc3/dawgie.egg-info/dependency_links.txt
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      245 2024-04-30 17:23:48.000000 dawgie-1.4.3rc3/dawgie.egg-info/requires.txt
--rw-rw-r--   0 niessner  (1000) niessner  (1000)        7 2024-04-30 17:23:48.000000 dawgie-1.4.3rc3/dawgie.egg-info/top_level.txt
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       38 2024-04-30 17:23:48.070226 dawgie-1.4.3rc3/setup.cfg
--rwxrwxr-x   0 niessner  (1000) niessner  (1000)     6410 2024-04-30 17:17:50.000000 dawgie-1.4.3rc3/setup.py
+drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2024-05-07 18:33:39.132957 dawgie-1.4.3rc4/
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1615 2024-05-07 18:33:38.000000 dawgie-1.4.3rc4/LICENSE
+-rw-r--r--   0 niessner  (1000) niessner  (1000)     9940 2024-05-07 18:33:39.132957 dawgie-1.4.3rc4/PKG-INFO
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     8906 2024-05-07 18:33:38.000000 dawgie-1.4.3rc4/README.md
+drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2024-05-07 18:33:39.132957 dawgie-1.4.3rc4/dawgie.egg-info/
+-rw-r--r--   0 niessner  (1000) niessner  (1000)     9940 2024-05-07 18:33:39.000000 dawgie-1.4.3rc4/dawgie.egg-info/PKG-INFO
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     6632 2024-05-07 18:33:39.000000 dawgie-1.4.3rc4/dawgie.egg-info/SOURCES.txt
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)        1 2024-05-07 18:33:39.000000 dawgie-1.4.3rc4/dawgie.egg-info/dependency_links.txt
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      245 2024-05-07 18:33:39.000000 dawgie-1.4.3rc4/dawgie.egg-info/requires.txt
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)        7 2024-05-07 18:33:39.000000 dawgie-1.4.3rc4/dawgie.egg-info/top_level.txt
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       38 2024-05-07 18:33:39.132957 dawgie-1.4.3rc4/setup.cfg
+-rwxrwxr-x   0 niessner  (1000) niessner  (1000)     6410 2024-05-07 18:28:07.000000 dawgie-1.4.3rc4/setup.py
```

### Comparing `dawgie-1.4.3rc3/LICENSE` & `dawgie-1.4.3rc4/LICENSE`

 * *Files identical despite different names*

### Comparing `dawgie-1.4.3rc3/PKG-INFO` & `dawgie-1.4.3rc4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dawgie
-Version: 1.4.3rc3
+Version: 1.4.3rc4
 Summary: Data and Algorithm Work-flow Generation, Introspection, and Execution (DAWGIE)
 Home-page: https://github.com/al-niessner/DAWGIE
 Author: Al Niessner
 Author-email: Al.Niessner@jpl.nasa.gov
 License: see LICENSE file for details
 Keywords: adaptive pipeline
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dawgie-1.4.3rc3/README.md` & `dawgie-1.4.3rc4/README.md`

 * *Files identical despite different names*

### Comparing `dawgie-1.4.3rc3/dawgie.egg-info/PKG-INFO` & `dawgie-1.4.3rc4/dawgie.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dawgie
-Version: 1.4.3rc3
+Version: 1.4.3rc4
 Summary: Data and Algorithm Work-flow Generation, Introspection, and Execution (DAWGIE)
 Home-page: https://github.com/al-niessner/DAWGIE
 Author: Al Niessner
 Author-email: Al.Niessner@jpl.nasa.gov
 License: see LICENSE file for details
 Keywords: adaptive pipeline
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dawgie-1.4.3rc3/dawgie.egg-info/SOURCES.txt` & `dawgie-1.4.3rc4/dawgie.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,121 +1,121 @@
 LICENSE
 README.md
 setup.py
 ../LICENSE.txt
-/tmp/tmp.cS53uDDIXP/Python/dawgie/__init__.py
-/tmp/tmp.cS53uDDIXP/Python/dawgie/context.py
-/tmp/tmp.cS53uDDIXP/Python/dawgie/security.py
-/tmp/tmp.cS53uDDIXP/Python/dawgie/db/__init__.py
-/tmp/tmp.cS53uDDIXP/Python/dawgie/db/lockview.py
-/tmp/tmp.cS53uDDIXP/Python/dawgie/db/post.py
-/tmp/tmp.cS53uDDIXP/Python/dawgie/db/test.py
-/tmp/tmp.cS53uDDIXP/Python/dawgie/db/testdata.py
-/tmp/tmp.cS53uDDIXP/Python/dawgie/db/shelve/__init__.py
-/tmp/tmp.cS53uDDIXP/Python/dawgie/db/shelve/comms.py
-/tmp/tmp.cS53uDDIXP/Python/dawgie/db/shelve/enums.py
-/tmp/tmp.cS53uDDIXP/Python/dawgie/db/shelve/model.py
-/tmp/tmp.cS53uDDIXP/Python/dawgie/db/shelve/state.py
-/tmp/tmp.cS53uDDIXP/Python/dawgie/db/shelve/util.py
-/tmp/tmp.cS53uDDIXP/Python/dawgie/db/tools/__init__.py
-/tmp/tmp.cS53uDDIXP/Python/dawgie/db/tools/dbsinfo.py
-/tmp/tmp.cS53uDDIXP/Python/dawgie/db/tools/extract.py
-/tmp/tmp.cS53uDDIXP/Python/dawgie/db/tools/inter.py
-/tmp/tmp.cS53uDDIXP/Python/dawgie/db/tools/list.py
-/tmp/tmp.cS53uDDIXP/Python/dawgie/db/tools/post2shelve.py
-/tmp/tmp.cS53uDDIXP/Python/dawgie/db/tools/purge.py
-/tmp/tmp.cS53uDDIXP/Python/dawgie/db/tools/sandbox.py
-/tmp/tmp.cS53uDDIXP/Python/dawgie/db/tools/util.py
-/tmp/tmp.cS53uDDIXP/Python/dawgie/db/tools/worm.py
-/tmp/tmp.cS53uDDIXP/Python/dawgie/db/util/__init__.py
-/tmp/tmp.cS53uDDIXP/Python/dawgie/db/util/aspect.py
-/tmp/tmp.cS53uDDIXP/Python/dawgie/de/__init__.py
-/tmp/tmp.cS53uDDIXP/Python/dawgie/de/html.py
-/tmp/tmp.cS53uDDIXP/Python/dawgie/fe/__init__.py
-/tmp/tmp.cS53uDDIXP/Python/dawgie/fe/__main__.py
-/tmp/tmp.cS53uDDIXP/Python/dawgie/fe/app.py
-/tmp/tmp.cS53uDDIXP/Python/dawgie/fe/requirements.txt
-/tmp/tmp.cS53uDDIXP/Python/dawgie/fe/submit.py
-/tmp/tmp.cS53uDDIXP/Python/dawgie/fe/svrender.py
-/tmp/tmp.cS53uDDIXP/Python/dawgie/fe/fonts/open-sans-v13-latin-300.eot
-/tmp/tmp.cS53uDDIXP/Python/dawgie/fe/fonts/open-sans-v13-latin-300.svg
-/tmp/tmp.cS53uDDIXP/Python/dawgie/fe/fonts/open-sans-v13-latin-300.ttf
-/tmp/tmp.cS53uDDIXP/Python/dawgie/fe/fonts/open-sans-v13-latin-300.woff
-/tmp/tmp.cS53uDDIXP/Python/dawgie/fe/fonts/open-sans-v13-latin-300.woff2
-/tmp/tmp.cS53uDDIXP/Python/dawgie/fe/fonts/open-sans-v13-latin-700.eot
-/tmp/tmp.cS53uDDIXP/Python/dawgie/fe/fonts/open-sans-v13-latin-700.svg
-/tmp/tmp.cS53uDDIXP/Python/dawgie/fe/fonts/open-sans-v13-latin-700.ttf
-/tmp/tmp.cS53uDDIXP/Python/dawgie/fe/fonts/open-sans-v13-latin-700.woff
-/tmp/tmp.cS53uDDIXP/Python/dawgie/fe/fonts/open-sans-v13-latin-700.woff2
-/tmp/tmp.cS53uDDIXP/Python/dawgie/fe/fonts/open-sans-v13-latin-regular.eot
-/tmp/tmp.cS53uDDIXP/Python/dawgie/fe/fonts/open-sans-v13-latin-regular.svg
-/tmp/tmp.cS53uDDIXP/Python/dawgie/fe/fonts/open-sans-v13-latin-regular.ttf
-/tmp/tmp.cS53uDDIXP/Python/dawgie/fe/fonts/open-sans-v13-latin-regular.woff
-/tmp/tmp.cS53uDDIXP/Python/dawgie/fe/fonts/open-sans-v13-latin-regular.woff2
-/tmp/tmp.cS53uDDIXP/Python/dawgie/fe/fonts/bootstrap/glyphicons-halflings-regular.eot
-/tmp/tmp.cS53uDDIXP/Python/dawgie/fe/fonts/bootstrap/glyphicons-halflings-regular.svg
-/tmp/tmp.cS53uDDIXP/Python/dawgie/fe/fonts/bootstrap/glyphicons-halflings-regular.ttf
-/tmp/tmp.cS53uDDIXP/Python/dawgie/fe/fonts/bootstrap/glyphicons-halflings-regular.woff
-/tmp/tmp.cS53uDDIXP/Python/dawgie/fe/fonts/bootstrap/glyphicons-halflings-regular.woff2
-/tmp/tmp.cS53uDDIXP/Python/dawgie/fe/images/loading.gif
-/tmp/tmp.cS53uDDIXP/Python/dawgie/fe/javascripts/algorithms_table.js
-/tmp/tmp.cS53uDDIXP/Python/dawgie/fe/javascripts/application.js
-/tmp/tmp.cS53uDDIXP/Python/dawgie/fe/javascripts/db.js
-/tmp/tmp.cS53uDDIXP/Python/dawgie/fe/javascripts/schedule.js
-/tmp/tmp.cS53uDDIXP/Python/dawgie/fe/javascripts/tasks_table.js
-/tmp/tmp.cS53uDDIXP/Python/dawgie/fe/javascripts/welcome.js
-/tmp/tmp.cS53uDDIXP/Python/dawgie/fe/pages/index.html
-/tmp/tmp.cS53uDDIXP/Python/dawgie/fe/pages/about/index.html
-/tmp/tmp.cS53uDDIXP/Python/dawgie/fe/pages/algorithms/index.html
-/tmp/tmp.cS53uDDIXP/Python/dawgie/fe/pages/command/index.html
-/tmp/tmp.cS53uDDIXP/Python/dawgie/fe/pages/database/index.html
-/tmp/tmp.cS53uDDIXP/Python/dawgie/fe/pages/database/primary_table/index.html
-/tmp/tmp.cS53uDDIXP/Python/dawgie/fe/pages/database/targets/index.html
-/tmp/tmp.cS53uDDIXP/Python/dawgie/fe/pages/database/tasks/index.html
-/tmp/tmp.cS53uDDIXP/Python/dawgie/fe/pages/database/versions/index.html
-/tmp/tmp.cS53uDDIXP/Python/dawgie/fe/pages/exoplanet_systems/index.html
-/tmp/tmp.cS53uDDIXP/Python/dawgie/fe/pages/logs/index.html
-/tmp/tmp.cS53uDDIXP/Python/dawgie/fe/pages/pipelines/index.html
-/tmp/tmp.cS53uDDIXP/Python/dawgie/fe/pages/schedule/index.html
-/tmp/tmp.cS53uDDIXP/Python/dawgie/fe/pages/search/index.html
-/tmp/tmp.cS53uDDIXP/Python/dawgie/fe/pages/tasks/index.html
-/tmp/tmp.cS53uDDIXP/Python/dawgie/fe/stylesheets/application.css
-/tmp/tmp.cS53uDDIXP/Python/dawgie/pl/__init__.py
-/tmp/tmp.cS53uDDIXP/Python/dawgie/pl/__main__.py
-/tmp/tmp.cS53uDDIXP/Python/dawgie/pl/dag.py
-/tmp/tmp.cS53uDDIXP/Python/dawgie/pl/farm.py
-/tmp/tmp.cS53uDDIXP/Python/dawgie/pl/jobinfo.py
-/tmp/tmp.cS53uDDIXP/Python/dawgie/pl/message.py
-/tmp/tmp.cS53uDDIXP/Python/dawgie/pl/promotion.py
-/tmp/tmp.cS53uDDIXP/Python/dawgie/pl/resources.py
-/tmp/tmp.cS53uDDIXP/Python/dawgie/pl/scan.py
-/tmp/tmp.cS53uDDIXP/Python/dawgie/pl/schedule.py
-/tmp/tmp.cS53uDDIXP/Python/dawgie/pl/snapshot.py
-/tmp/tmp.cS53uDDIXP/Python/dawgie/pl/state.dot
-/tmp/tmp.cS53uDDIXP/Python/dawgie/pl/state.py
-/tmp/tmp.cS53uDDIXP/Python/dawgie/pl/util.py
-/tmp/tmp.cS53uDDIXP/Python/dawgie/pl/version.py
-/tmp/tmp.cS53uDDIXP/Python/dawgie/pl/logger/__init__.py
-/tmp/tmp.cS53uDDIXP/Python/dawgie/pl/logger/fe.py
-/tmp/tmp.cS53uDDIXP/Python/dawgie/pl/worker/__init__.py
-/tmp/tmp.cS53uDDIXP/Python/dawgie/pl/worker/__main__.py
-/tmp/tmp.cS53uDDIXP/Python/dawgie/pl/worker/aws.py
-/tmp/tmp.cS53uDDIXP/Python/dawgie/pl/worker/cluster.py
-/tmp/tmp.cS53uDDIXP/Python/dawgie/tools/__init__.py
-/tmp/tmp.cS53uDDIXP/Python/dawgie/tools/compliant.py
-/tmp/tmp.cS53uDDIXP/Python/dawgie/tools/dag.py
-/tmp/tmp.cS53uDDIXP/Python/dawgie/tools/detach.py
-/tmp/tmp.cS53uDDIXP/Python/dawgie/tools/logfile.py
-/tmp/tmp.cS53uDDIXP/Python/dawgie/tools/resources.py
-/tmp/tmp.cS53uDDIXP/Python/dawgie/tools/submit.py
-/tmp/tmp.cS53uDDIXP/Python/dawgie/tools/trace.py
-/tmp/tmp.cS53uDDIXP/Python/dawgie/util/__init__.py
-/tmp/tmp.cS53uDDIXP/Python/dawgie/util/args.py
-/tmp/tmp.cS53uDDIXP/Python/dawgie/util/fifo.py
-/tmp/tmp.cS53uDDIXP/Python/dawgie/util/metrics.py
-/tmp/tmp.cS53uDDIXP/Python/dawgie/util/names.py
-/tmp/tmp.cS53uDDIXP/Python/dawgie/util/refs.py
+/tmp/tmp.sNon0OqH0B/Python/dawgie/__init__.py
+/tmp/tmp.sNon0OqH0B/Python/dawgie/context.py
+/tmp/tmp.sNon0OqH0B/Python/dawgie/security.py
+/tmp/tmp.sNon0OqH0B/Python/dawgie/db/__init__.py
+/tmp/tmp.sNon0OqH0B/Python/dawgie/db/lockview.py
+/tmp/tmp.sNon0OqH0B/Python/dawgie/db/post.py
+/tmp/tmp.sNon0OqH0B/Python/dawgie/db/test.py
+/tmp/tmp.sNon0OqH0B/Python/dawgie/db/testdata.py
+/tmp/tmp.sNon0OqH0B/Python/dawgie/db/shelve/__init__.py
+/tmp/tmp.sNon0OqH0B/Python/dawgie/db/shelve/comms.py
+/tmp/tmp.sNon0OqH0B/Python/dawgie/db/shelve/enums.py
+/tmp/tmp.sNon0OqH0B/Python/dawgie/db/shelve/model.py
+/tmp/tmp.sNon0OqH0B/Python/dawgie/db/shelve/state.py
+/tmp/tmp.sNon0OqH0B/Python/dawgie/db/shelve/util.py
+/tmp/tmp.sNon0OqH0B/Python/dawgie/db/tools/__init__.py
+/tmp/tmp.sNon0OqH0B/Python/dawgie/db/tools/dbsinfo.py
+/tmp/tmp.sNon0OqH0B/Python/dawgie/db/tools/extract.py
+/tmp/tmp.sNon0OqH0B/Python/dawgie/db/tools/inter.py
+/tmp/tmp.sNon0OqH0B/Python/dawgie/db/tools/list.py
+/tmp/tmp.sNon0OqH0B/Python/dawgie/db/tools/post2shelve.py
+/tmp/tmp.sNon0OqH0B/Python/dawgie/db/tools/purge.py
+/tmp/tmp.sNon0OqH0B/Python/dawgie/db/tools/sandbox.py
+/tmp/tmp.sNon0OqH0B/Python/dawgie/db/tools/util.py
+/tmp/tmp.sNon0OqH0B/Python/dawgie/db/tools/worm.py
+/tmp/tmp.sNon0OqH0B/Python/dawgie/db/util/__init__.py
+/tmp/tmp.sNon0OqH0B/Python/dawgie/db/util/aspect.py
+/tmp/tmp.sNon0OqH0B/Python/dawgie/de/__init__.py
+/tmp/tmp.sNon0OqH0B/Python/dawgie/de/html.py
+/tmp/tmp.sNon0OqH0B/Python/dawgie/fe/__init__.py
+/tmp/tmp.sNon0OqH0B/Python/dawgie/fe/__main__.py
+/tmp/tmp.sNon0OqH0B/Python/dawgie/fe/app.py
+/tmp/tmp.sNon0OqH0B/Python/dawgie/fe/requirements.txt
+/tmp/tmp.sNon0OqH0B/Python/dawgie/fe/submit.py
+/tmp/tmp.sNon0OqH0B/Python/dawgie/fe/svrender.py
+/tmp/tmp.sNon0OqH0B/Python/dawgie/fe/fonts/open-sans-v13-latin-300.eot
+/tmp/tmp.sNon0OqH0B/Python/dawgie/fe/fonts/open-sans-v13-latin-300.svg
+/tmp/tmp.sNon0OqH0B/Python/dawgie/fe/fonts/open-sans-v13-latin-300.ttf
+/tmp/tmp.sNon0OqH0B/Python/dawgie/fe/fonts/open-sans-v13-latin-300.woff
+/tmp/tmp.sNon0OqH0B/Python/dawgie/fe/fonts/open-sans-v13-latin-300.woff2
+/tmp/tmp.sNon0OqH0B/Python/dawgie/fe/fonts/open-sans-v13-latin-700.eot
+/tmp/tmp.sNon0OqH0B/Python/dawgie/fe/fonts/open-sans-v13-latin-700.svg
+/tmp/tmp.sNon0OqH0B/Python/dawgie/fe/fonts/open-sans-v13-latin-700.ttf
+/tmp/tmp.sNon0OqH0B/Python/dawgie/fe/fonts/open-sans-v13-latin-700.woff
+/tmp/tmp.sNon0OqH0B/Python/dawgie/fe/fonts/open-sans-v13-latin-700.woff2
+/tmp/tmp.sNon0OqH0B/Python/dawgie/fe/fonts/open-sans-v13-latin-regular.eot
+/tmp/tmp.sNon0OqH0B/Python/dawgie/fe/fonts/open-sans-v13-latin-regular.svg
+/tmp/tmp.sNon0OqH0B/Python/dawgie/fe/fonts/open-sans-v13-latin-regular.ttf
+/tmp/tmp.sNon0OqH0B/Python/dawgie/fe/fonts/open-sans-v13-latin-regular.woff
+/tmp/tmp.sNon0OqH0B/Python/dawgie/fe/fonts/open-sans-v13-latin-regular.woff2
+/tmp/tmp.sNon0OqH0B/Python/dawgie/fe/fonts/bootstrap/glyphicons-halflings-regular.eot
+/tmp/tmp.sNon0OqH0B/Python/dawgie/fe/fonts/bootstrap/glyphicons-halflings-regular.svg
+/tmp/tmp.sNon0OqH0B/Python/dawgie/fe/fonts/bootstrap/glyphicons-halflings-regular.ttf
+/tmp/tmp.sNon0OqH0B/Python/dawgie/fe/fonts/bootstrap/glyphicons-halflings-regular.woff
+/tmp/tmp.sNon0OqH0B/Python/dawgie/fe/fonts/bootstrap/glyphicons-halflings-regular.woff2
+/tmp/tmp.sNon0OqH0B/Python/dawgie/fe/images/loading.gif
+/tmp/tmp.sNon0OqH0B/Python/dawgie/fe/javascripts/algorithms_table.js
+/tmp/tmp.sNon0OqH0B/Python/dawgie/fe/javascripts/application.js
+/tmp/tmp.sNon0OqH0B/Python/dawgie/fe/javascripts/db.js
+/tmp/tmp.sNon0OqH0B/Python/dawgie/fe/javascripts/schedule.js
+/tmp/tmp.sNon0OqH0B/Python/dawgie/fe/javascripts/tasks_table.js
+/tmp/tmp.sNon0OqH0B/Python/dawgie/fe/javascripts/welcome.js
+/tmp/tmp.sNon0OqH0B/Python/dawgie/fe/pages/index.html
+/tmp/tmp.sNon0OqH0B/Python/dawgie/fe/pages/about/index.html
+/tmp/tmp.sNon0OqH0B/Python/dawgie/fe/pages/algorithms/index.html
+/tmp/tmp.sNon0OqH0B/Python/dawgie/fe/pages/command/index.html
+/tmp/tmp.sNon0OqH0B/Python/dawgie/fe/pages/database/index.html
+/tmp/tmp.sNon0OqH0B/Python/dawgie/fe/pages/database/primary_table/index.html
+/tmp/tmp.sNon0OqH0B/Python/dawgie/fe/pages/database/targets/index.html
+/tmp/tmp.sNon0OqH0B/Python/dawgie/fe/pages/database/tasks/index.html
+/tmp/tmp.sNon0OqH0B/Python/dawgie/fe/pages/database/versions/index.html
+/tmp/tmp.sNon0OqH0B/Python/dawgie/fe/pages/exoplanet_systems/index.html
+/tmp/tmp.sNon0OqH0B/Python/dawgie/fe/pages/logs/index.html
+/tmp/tmp.sNon0OqH0B/Python/dawgie/fe/pages/pipelines/index.html
+/tmp/tmp.sNon0OqH0B/Python/dawgie/fe/pages/schedule/index.html
+/tmp/tmp.sNon0OqH0B/Python/dawgie/fe/pages/search/index.html
+/tmp/tmp.sNon0OqH0B/Python/dawgie/fe/pages/tasks/index.html
+/tmp/tmp.sNon0OqH0B/Python/dawgie/fe/stylesheets/application.css
+/tmp/tmp.sNon0OqH0B/Python/dawgie/pl/__init__.py
+/tmp/tmp.sNon0OqH0B/Python/dawgie/pl/__main__.py
+/tmp/tmp.sNon0OqH0B/Python/dawgie/pl/dag.py
+/tmp/tmp.sNon0OqH0B/Python/dawgie/pl/farm.py
+/tmp/tmp.sNon0OqH0B/Python/dawgie/pl/jobinfo.py
+/tmp/tmp.sNon0OqH0B/Python/dawgie/pl/message.py
+/tmp/tmp.sNon0OqH0B/Python/dawgie/pl/promotion.py
+/tmp/tmp.sNon0OqH0B/Python/dawgie/pl/resources.py
+/tmp/tmp.sNon0OqH0B/Python/dawgie/pl/scan.py
+/tmp/tmp.sNon0OqH0B/Python/dawgie/pl/schedule.py
+/tmp/tmp.sNon0OqH0B/Python/dawgie/pl/snapshot.py
+/tmp/tmp.sNon0OqH0B/Python/dawgie/pl/state.dot
+/tmp/tmp.sNon0OqH0B/Python/dawgie/pl/state.py
+/tmp/tmp.sNon0OqH0B/Python/dawgie/pl/util.py
+/tmp/tmp.sNon0OqH0B/Python/dawgie/pl/version.py
+/tmp/tmp.sNon0OqH0B/Python/dawgie/pl/logger/__init__.py
+/tmp/tmp.sNon0OqH0B/Python/dawgie/pl/logger/fe.py
+/tmp/tmp.sNon0OqH0B/Python/dawgie/pl/worker/__init__.py
+/tmp/tmp.sNon0OqH0B/Python/dawgie/pl/worker/__main__.py
+/tmp/tmp.sNon0OqH0B/Python/dawgie/pl/worker/aws.py
+/tmp/tmp.sNon0OqH0B/Python/dawgie/pl/worker/cluster.py
+/tmp/tmp.sNon0OqH0B/Python/dawgie/tools/__init__.py
+/tmp/tmp.sNon0OqH0B/Python/dawgie/tools/compliant.py
+/tmp/tmp.sNon0OqH0B/Python/dawgie/tools/dag.py
+/tmp/tmp.sNon0OqH0B/Python/dawgie/tools/detach.py
+/tmp/tmp.sNon0OqH0B/Python/dawgie/tools/logfile.py
+/tmp/tmp.sNon0OqH0B/Python/dawgie/tools/resources.py
+/tmp/tmp.sNon0OqH0B/Python/dawgie/tools/submit.py
+/tmp/tmp.sNon0OqH0B/Python/dawgie/tools/trace.py
+/tmp/tmp.sNon0OqH0B/Python/dawgie/util/__init__.py
+/tmp/tmp.sNon0OqH0B/Python/dawgie/util/args.py
+/tmp/tmp.sNon0OqH0B/Python/dawgie/util/fifo.py
+/tmp/tmp.sNon0OqH0B/Python/dawgie/util/metrics.py
+/tmp/tmp.sNon0OqH0B/Python/dawgie/util/names.py
+/tmp/tmp.sNon0OqH0B/Python/dawgie/util/refs.py
 dawgie.egg-info/PKG-INFO
 dawgie.egg-info/SOURCES.txt
 dawgie.egg-info/dependency_links.txt
 dawgie.egg-info/requires.txt
 dawgie.egg-info/top_level.txt
```

### Comparing `dawgie-1.4.3rc3/setup.py` & `dawgie-1.4.3rc4/setup.py`

 * *Files identical despite different names*

