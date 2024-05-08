# Comparing `tmp/netbox-ipv4-tools-1.0.3.tar.gz` & `tmp/netbox_ipv4_tools-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox-ipv4-tools-1.0.3.tar", last modified: Mon Jun 12 08:17:03 2023, max compression
+gzip compressed data, was "netbox_ipv4_tools-1.0.4.tar", last modified: Wed May  8 15:00:26 2024, max compression
```

## Comparing `netbox-ipv4-tools-1.0.3.tar` & `netbox_ipv4_tools-1.0.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 08:17:03.358089 netbox-ipv4-tools-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-12 08:16:45.000000 netbox-ipv4-tools-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-12 08:16:45.000000 netbox-ipv4-tools-1.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-06-12 08:17:03.358089 netbox-ipv4-tools-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-06-12 08:16:45.000000 netbox-ipv4-tools-1.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 08:17:03.358089 netbox-ipv4-tools-1.0.3/netbox_ipv4_tools/
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-12 08:16:45.000000 netbox-ipv4-tools-1.0.3/netbox_ipv4_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-12 08:16:45.000000 netbox-ipv4-tools-1.0.3/netbox_ipv4_tools/navigation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 08:17:03.354089 netbox-ipv4-tools-1.0.3/netbox_ipv4_tools/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 08:17:03.354089 netbox-ipv4-tools-1.0.3/netbox_ipv4_tools/static/netbox_ipv4_tools/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 08:17:03.358089 netbox-ipv4-tools-1.0.3/netbox_ipv4_tools/static/netbox_ipv4_tools/js/
--rw-r--r--   0 runner    (1001) docker     (123)     6814 2023-06-12 08:16:45.000000 netbox-ipv4-tools-1.0.3/netbox_ipv4_tools/static/netbox_ipv4_tools/js/netmask.js
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-06-12 08:16:45.000000 netbox-ipv4-tools-1.0.3/netbox_ipv4_tools/static/netbox_ipv4_tools/js/range.js
--rw-r--r--   0 runner    (1001) docker     (123)     3329 2023-06-12 08:16:45.000000 netbox-ipv4-tools-1.0.3/netbox_ipv4_tools/static/netbox_ipv4_tools/js/supernet.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 08:17:03.358089 netbox-ipv4-tools-1.0.3/netbox_ipv4_tools/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 08:17:03.358089 netbox-ipv4-tools-1.0.3/netbox_ipv4_tools/templates/netbox_ipv4_tools/
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-06-12 08:16:45.000000 netbox-ipv4-tools-1.0.3/netbox_ipv4_tools/templates/netbox_ipv4_tools/cidr-to-range.html
--rw-r--r--   0 runner    (1001) docker     (123)     7381 2023-06-12 08:16:45.000000 netbox-ipv4-tools-1.0.3/netbox_ipv4_tools/templates/netbox_ipv4_tools/cidr.html
--rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-06-12 08:16:45.000000 netbox-ipv4-tools-1.0.3/netbox_ipv4_tools/templates/netbox_ipv4_tools/supernet-calculator.html
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-12 08:16:45.000000 netbox-ipv4-tools-1.0.3/netbox_ipv4_tools/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-06-12 08:16:45.000000 netbox-ipv4-tools-1.0.3/netbox_ipv4_tools/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 08:17:03.358089 netbox-ipv4-tools-1.0.3/netbox_ipv4_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-06-12 08:17:03.000000 netbox-ipv4-tools-1.0.3/netbox_ipv4_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-06-12 08:17:03.000000 netbox-ipv4-tools-1.0.3/netbox_ipv4_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 08:17:03.000000 netbox-ipv4-tools-1.0.3/netbox_ipv4_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-12 08:17:03.000000 netbox-ipv4-tools-1.0.3/netbox_ipv4_tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 08:17:03.358089 netbox-ipv4-tools-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-06-12 08:16:45.000000 netbox-ipv4-tools-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:00:26.599211 netbox_ipv4_tools-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-08 15:00:22.000000 netbox_ipv4_tools-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-08 15:00:22.000000 netbox_ipv4_tools-1.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-05-08 15:00:26.595211 netbox_ipv4_tools-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-05-08 15:00:22.000000 netbox_ipv4_tools-1.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:00:26.595211 netbox_ipv4_tools-1.0.4/netbox_ipv4_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-08 15:00:22.000000 netbox_ipv4_tools-1.0.4/netbox_ipv4_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-05-08 15:00:22.000000 netbox_ipv4_tools-1.0.4/netbox_ipv4_tools/navigation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:00:26.595211 netbox_ipv4_tools-1.0.4/netbox_ipv4_tools/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:00:26.595211 netbox_ipv4_tools-1.0.4/netbox_ipv4_tools/static/netbox_ipv4_tools/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:00:26.595211 netbox_ipv4_tools-1.0.4/netbox_ipv4_tools/static/netbox_ipv4_tools/js/
+-rw-r--r--   0 runner    (1001) docker     (127)     6814 2024-05-08 15:00:22.000000 netbox_ipv4_tools-1.0.4/netbox_ipv4_tools/static/netbox_ipv4_tools/js/netmask.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-05-08 15:00:22.000000 netbox_ipv4_tools-1.0.4/netbox_ipv4_tools/static/netbox_ipv4_tools/js/range.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-05-08 15:00:22.000000 netbox_ipv4_tools-1.0.4/netbox_ipv4_tools/static/netbox_ipv4_tools/js/supernet.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:00:26.595211 netbox_ipv4_tools-1.0.4/netbox_ipv4_tools/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:00:26.595211 netbox_ipv4_tools-1.0.4/netbox_ipv4_tools/templates/netbox_ipv4_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-05-08 15:00:22.000000 netbox_ipv4_tools-1.0.4/netbox_ipv4_tools/templates/netbox_ipv4_tools/cidr-to-range.html
+-rw-r--r--   0 runner    (1001) docker     (127)     7381 2024-05-08 15:00:22.000000 netbox_ipv4_tools-1.0.4/netbox_ipv4_tools/templates/netbox_ipv4_tools/cidr.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-05-08 15:00:22.000000 netbox_ipv4_tools-1.0.4/netbox_ipv4_tools/templates/netbox_ipv4_tools/supernet-calculator.html
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-08 15:00:22.000000 netbox_ipv4_tools-1.0.4/netbox_ipv4_tools/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-08 15:00:22.000000 netbox_ipv4_tools-1.0.4/netbox_ipv4_tools/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:00:26.595211 netbox_ipv4_tools-1.0.4/netbox_ipv4_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-05-08 15:00:26.000000 netbox_ipv4_tools-1.0.4/netbox_ipv4_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-05-08 15:00:26.000000 netbox_ipv4_tools-1.0.4/netbox_ipv4_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 15:00:26.000000 netbox_ipv4_tools-1.0.4/netbox_ipv4_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-08 15:00:26.000000 netbox_ipv4_tools-1.0.4/netbox_ipv4_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 15:00:26.599211 netbox_ipv4_tools-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-05-08 15:00:22.000000 netbox_ipv4_tools-1.0.4/setup.py
```

### Comparing `netbox-ipv4-tools-1.0.3/LICENSE` & `netbox_ipv4_tools-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox-ipv4-tools-1.0.3/PKG-INFO` & `netbox_ipv4_tools-1.0.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-ipv4-tools
-Version: 1.0.3
+Version: 1.0.4
 Summary: Work with ipv4 in NetBox
 Home-page: https://github.com/mlongo4290/netbox-ipv4-tools
 Author: Michael Longo
 License: Apache 2.0
 Project-URL: Source, https://github.com/mlongo4290/netbox-ipv4-tools
 Keywords: netbox-plugin
 Classifier: Programming Language :: Python
@@ -48,12 +48,12 @@
 ```bash
 cd /opt/netbox/netbox
 pip3 install netbox-ipv4-tools
 python3 manage.py collectstatic --no-input
 ```
 
 ### Versions
-This plugin requires netbox >= 3.4.0
+This plugin requires netbox >= 4.0.0
 
 ### Thanks
 Thanks to [rs](https://github.com/rs) for the work on [netmask](https://github.com/rs/node-netmask)  
 Thanks to [mattieserver](https://github.com/mattieserver) and his project [netbox-topology-view](https://github.com/mattieserver/netbox-topology-views). I used his work to get a working plugin and to publish it to pypi
```

### Comparing `netbox-ipv4-tools-1.0.3/README.md` & `netbox_ipv4_tools-1.0.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -33,12 +33,12 @@
 ```bash
 cd /opt/netbox/netbox
 pip3 install netbox-ipv4-tools
 python3 manage.py collectstatic --no-input
 ```
 
 ### Versions
-This plugin requires netbox >= 3.4.0
+This plugin requires netbox >= 4.0.0
 
 ### Thanks
 Thanks to [rs](https://github.com/rs) for the work on [netmask](https://github.com/rs/node-netmask)  
 Thanks to [mattieserver](https://github.com/mattieserver) and his project [netbox-topology-view](https://github.com/mattieserver/netbox-topology-views). I used his work to get a working plugin and to publish it to pypi
```

### Comparing `netbox-ipv4-tools-1.0.3/netbox_ipv4_tools/navigation.py` & `netbox_ipv4_tools-1.0.4/netbox_ipv4_tools/navigation.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from extras.plugins import PluginMenu, PluginMenuItem
+from netbox.plugins import PluginMenu, PluginMenuItem
 
 menu = PluginMenu(
     label='IPv4 Tools',
     groups=(
         (
             'TOOLS',
             (
```

### Comparing `netbox-ipv4-tools-1.0.3/netbox_ipv4_tools/static/netbox_ipv4_tools/js/netmask.js` & `netbox_ipv4_tools-1.0.4/netbox_ipv4_tools/static/netbox_ipv4_tools/js/netmask.js`

 * *Files identical despite different names*

### Comparing `netbox-ipv4-tools-1.0.3/netbox_ipv4_tools/static/netbox_ipv4_tools/js/range.js` & `netbox_ipv4_tools-1.0.4/netbox_ipv4_tools/static/netbox_ipv4_tools/js/range.js`

 * *Files identical despite different names*

### Comparing `netbox-ipv4-tools-1.0.3/netbox_ipv4_tools/static/netbox_ipv4_tools/js/supernet.js` & `netbox_ipv4_tools-1.0.4/netbox_ipv4_tools/static/netbox_ipv4_tools/js/supernet.js`

 * *Files identical despite different names*

### Comparing `netbox-ipv4-tools-1.0.3/netbox_ipv4_tools/templates/netbox_ipv4_tools/cidr-to-range.html` & `netbox_ipv4_tools-1.0.4/netbox_ipv4_tools/templates/netbox_ipv4_tools/cidr-to-range.html`

 * *Files identical despite different names*

### Comparing `netbox-ipv4-tools-1.0.3/netbox_ipv4_tools/templates/netbox_ipv4_tools/cidr.html` & `netbox_ipv4_tools-1.0.4/netbox_ipv4_tools/templates/netbox_ipv4_tools/cidr.html`

 * *Files identical despite different names*

### Comparing `netbox-ipv4-tools-1.0.3/netbox_ipv4_tools/templates/netbox_ipv4_tools/supernet-calculator.html` & `netbox_ipv4_tools-1.0.4/netbox_ipv4_tools/templates/netbox_ipv4_tools/supernet-calculator.html`

 * *Files identical despite different names*

### Comparing `netbox-ipv4-tools-1.0.3/netbox_ipv4_tools/views.py` & `netbox_ipv4_tools-1.0.4/netbox_ipv4_tools/views.py`

 * *Files identical despite different names*

### Comparing `netbox-ipv4-tools-1.0.3/netbox_ipv4_tools.egg-info/PKG-INFO` & `netbox_ipv4_tools-1.0.4/netbox_ipv4_tools.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-ipv4-tools
-Version: 1.0.3
+Version: 1.0.4
 Summary: Work with ipv4 in NetBox
 Home-page: https://github.com/mlongo4290/netbox-ipv4-tools
 Author: Michael Longo
 License: Apache 2.0
 Project-URL: Source, https://github.com/mlongo4290/netbox-ipv4-tools
 Keywords: netbox-plugin
 Classifier: Programming Language :: Python
@@ -48,12 +48,12 @@
 ```bash
 cd /opt/netbox/netbox
 pip3 install netbox-ipv4-tools
 python3 manage.py collectstatic --no-input
 ```
 
 ### Versions
-This plugin requires netbox >= 3.4.0
+This plugin requires netbox >= 4.0.0
 
 ### Thanks
 Thanks to [rs](https://github.com/rs) for the work on [netmask](https://github.com/rs/node-netmask)  
 Thanks to [mattieserver](https://github.com/mattieserver) and his project [netbox-topology-view](https://github.com/mattieserver/netbox-topology-views). I used his work to get a working plugin and to publish it to pypi
```

### Comparing `netbox-ipv4-tools-1.0.3/netbox_ipv4_tools.egg-info/SOURCES.txt` & `netbox_ipv4_tools-1.0.4/netbox_ipv4_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `netbox-ipv4-tools-1.0.3/setup.py` & `netbox_ipv4_tools-1.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import find_packages, setup
 
 readme = Path(__file__).parent / "README.md"
 long_description = readme.read_text()
 
 setup(
     name="netbox-ipv4-tools",
-    version="1.0.3",
+    version="1.0.4",
     description="Work with ipv4 in NetBox",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/mlongo4290/netbox-ipv4-tools",
     author="Michael Longo",
     license="Apache 2.0",
     install_requires=[],
```

