# Comparing `tmp/slicerio-0.1.8.tar.gz` & `tmp/slicerio-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slicerio-0.1.8.tar", last modified: Sat Nov 12 03:28:46 2022, max compression
+gzip compressed data, was "slicerio-1.0.0.tar", last modified: Wed May  8 19:15:05 2024, max compression
```

## Comparing `slicerio-0.1.8.tar` & `slicerio-1.0.0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwxrwx   0        0        0        0 2022-11-12 03:28:46.959299 slicerio-0.1.8/
--rw-rw-rw-   0        0        0     7107 2022-11-12 03:28:46.960913 slicerio-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     4947 2022-11-12 03:28:17.000000 slicerio-0.1.8/README.md
--rw-rw-rw-   0        0        0      121 2022-11-12 03:28:46.963467 slicerio-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0     1816 2022-10-04 05:09:03.000000 slicerio-0.1.8/setup.py
-drwxrwxrwx   0        0        0        0 2022-11-12 03:28:46.918228 slicerio-0.1.8/slicerio/
--rw-rw-rw-   0        0        0      782 2022-10-05 04:32:30.000000 slicerio-0.1.8/slicerio/__init__.py
--rw-rw-rw-   0        0        0      182 2022-11-12 03:28:17.000000 slicerio-0.1.8/slicerio/_version.py
--rw-rw-rw-   0        0        0      682 2021-05-29 03:52:23.000000 slicerio-0.1.8/slicerio/data_helper.py
--rw-rw-rw-   0        0        0     5698 2021-06-01 23:54:15.000000 slicerio-0.1.8/slicerio/segmentation.py
--rw-rw-rw-   0        0        0     9143 2022-11-12 03:28:17.000000 slicerio-0.1.8/slicerio/server.py
-drwxrwxrwx   0        0        0        0 2022-11-12 03:28:46.955173 slicerio-0.1.8/slicerio/tests/
--rw-rw-rw-   0        0        0        0 2020-11-21 04:28:55.000000 slicerio-0.1.8/slicerio/tests/__init__.py
--rw-rw-rw-   0        0        0     2414 2021-05-29 03:52:23.000000 slicerio-0.1.8/slicerio/tests/test_segmentation.py
-drwxrwxrwx   0        0        0        0 2022-11-12 03:28:46.945759 slicerio-0.1.8/slicerio.egg-info/
--rw-rw-rw-   0        0        0     7107 2022-11-12 03:28:46.000000 slicerio-0.1.8/slicerio.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      360 2022-11-12 03:28:46.000000 slicerio-0.1.8/slicerio.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-12 03:28:46.000000 slicerio-0.1.8/slicerio.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2022-11-12 03:28:46.000000 slicerio-0.1.8/slicerio.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2022-11-12 03:28:46.000000 slicerio-0.1.8/slicerio.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-08 19:15:05.417981 slicerio-1.0.0/
+-rw-rw-rw-   0        0        0     1079 2021-05-29 02:56:33.000000 slicerio-1.0.0/LICENSE
+-rw-rw-rw-   0        0        0     9891 2024-05-08 19:15:05.418978 slicerio-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     8706 2024-05-08 17:00:26.000000 slicerio-1.0.0/README.md
+-rw-rw-rw-   0        0        0      121 2024-05-08 19:15:05.419998 slicerio-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1816 2022-10-04 05:09:03.000000 slicerio-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 19:15:05.404211 slicerio-1.0.0/slicerio/
+-rw-rw-rw-   0        0        0      817 2024-05-04 07:45:13.000000 slicerio-1.0.0/slicerio/__init__.py
+-rw-rw-rw-   0        0        0      182 2024-05-08 17:59:23.000000 slicerio-1.0.0/slicerio/_version.py
+-rw-rw-rw-   0        0        0      682 2021-05-29 03:52:23.000000 slicerio-1.0.0/slicerio/data_helper.py
+-rw-rw-rw-   0        0        0    38431 2024-05-08 18:04:25.000000 slicerio-1.0.0/slicerio/segmentation.py
+-rw-rw-rw-   0        0        0     9277 2023-02-27 18:21:01.000000 slicerio-1.0.0/slicerio/server.py
+drwxrwxrwx   0        0        0        0 2024-05-08 19:15:05.416993 slicerio-1.0.0/slicerio/tests/
+-rw-rw-rw-   0        0        0        0 2020-11-21 04:28:55.000000 slicerio-1.0.0/slicerio/tests/__init__.py
+-rw-rw-rw-   0        0        0     7995 2024-05-08 16:42:31.000000 slicerio-1.0.0/slicerio/tests/test_segmentation.py
+drwxrwxrwx   0        0        0        0 2024-05-08 19:15:05.414002 slicerio-1.0.0/slicerio.egg-info/
+-rw-rw-rw-   0        0        0     9891 2024-05-08 19:15:05.000000 slicerio-1.0.0/slicerio.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      368 2024-05-08 19:15:05.000000 slicerio-1.0.0/slicerio.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 19:15:05.000000 slicerio-1.0.0/slicerio.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2024-05-08 19:15:05.000000 slicerio-1.0.0/slicerio.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-08 19:15:05.000000 slicerio-1.0.0/slicerio.egg-info/top_level.txt
```

### Comparing `slicerio-0.1.8/setup.py` & `slicerio-1.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `slicerio-0.1.8/slicerio/__init__.py` & `slicerio-1.0.0/slicerio/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,20 +8,21 @@
 
 Any questions or need help? Post on 3D Slicer forum: https://discourse.slicer.org
 
 Bugs and other issues can be reported in the issue tracker: https://www.github.com/lassoan/slicerio
 
 """
 
-from .segmentation import extract_segments, read_segmentation_info, segment_from_name, segment_names
+from .segmentation import extract_segments, read_segmentation, write_segmentation, segment_from_name, segment_names
 from .data_helper import get_testdata_file
 from ._version import __version__, __version_info__
 
 __all__ = [
    'extract_segments',
    'get_testdata_file',
-   'read_segmentation_info',
+   'read_segmentation',
+   'write_segmentation',
    'segment_from_name',
    'segment_names',
    '__version__',
    '__version_info__'
    ]
```

### Comparing `slicerio-0.1.8/slicerio/data_helper.py` & `slicerio-1.0.0/slicerio/data_helper.py`

 * *Files identical despite different names*

### Comparing `slicerio-0.1.8/slicerio/server.py` & `slicerio-1.0.0/slicerio/server.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,23 +27,23 @@
         if time.time() - start > timeoutSec:
             raise requests.exceptions.ConnectTimeout("Timeout while waiting for application to start")
     return p
 
 def stop_server():
     """Stop local Slicer server.
     """
-    response = requests.delete(f"http://localhost:{SERVER_PORT}/system")
+    response = requests.delete(f"http://127.0.0.1:{SERVER_PORT}/system")
     return response.json()
 
 def is_server_running():
     """Check if a local Slicer server is running.
     Returns true if a responsive Slicer instance is found with Web Server and Slicer API enabled.
     """
     try:
-        response = requests.get(f"http://localhost:{SERVER_PORT}/slicer/system/version", timeout=3)
+        response = requests.get(f"http://127.0.0.1:{SERVER_PORT}/slicer/system/version", timeout=3)
         if 'applicationName' in response.json():
             # Found a responsive Slicer
             return True
     except Exception as e:
         logging.debug("Application is not available: "+str(e))
     return False
 
@@ -66,80 +66,84 @@
             raise RuntimeError(response.json()["message"])
     raise RuntimeError("Request failed")
 
 def node_remove(name=None, id=None, class_name=None):
     """Remove data nodes from the local Slicer server.
     Nodes can be selected using name, id, and/or class_name.
     """
-    api_url = f"http://localhost:{SERVER_PORT}/slicer/mrml"
+    api_url = f"http://127.0.0.1:{SERVER_PORT}/slicer/mrml"
     node_query = _node_query_parameters(name, id, class_name)
     if node_query:
         api_url += "?" + node_query
     response = requests.delete(api_url)
     _report_error(response)
 
 def node_reload(name=None, id=None, class_name=None):
     """Reload the node from that file it was originally loaded from.
     This can be used for updating a node that was loaded using `file_load()`,
     to prevent proliferation of displayed nodes.
     Nodes can be selected using name, id, and/or class_name.
     """
-    api_url = f"http://localhost:{SERVER_PORT}/slicer/mrml"
+    api_url = f"http://127.0.0.1:{SERVER_PORT}/slicer/mrml"
     node_query = _node_query_parameters(name, id, class_name)
     if node_query:
         api_url += "?" + node_query
     response = requests.put(api_url)
     _report_error(response)
 
 def node_properties(name=None, id=None, class_name=None):
     """Get properties of data nodes on the local Slicer server.
     Nodes can be selected using name, id, and/or class_name.
     """
-    api_url = f"http://localhost:{SERVER_PORT}/slicer/mrml/properties"
+    api_url = f"http://127.0.0.1:{SERVER_PORT}/slicer/mrml/properties"
     node_query = _node_query_parameters(name, id, class_name)
     if node_query:
         api_url += "?" + node_query
     response = requests.get(api_url)
     _report_error(response)
     response_json = response.json()
     properties = [response_json[key] for key in response_json]
     return properties
 
 def node_ids(name=None, id=None, class_name=None):
     """Get list of ids of nodes availalbe on the local Slicer server.
     Nodes can be selected using name, id, and/or class_name.
     """
-    api_url = f"http://localhost:{SERVER_PORT}/slicer/mrml/ids"
+    api_url = f"http://127.0.0.1:{SERVER_PORT}/slicer/mrml/ids"
     node_query = _node_query_parameters(name, id, class_name)
     if node_query:
         api_url += "?" + node_query
     response = requests.get(api_url)
     _report_error(response)
     return response.json()
 
 def node_names(name=None, id=None, class_name=None):
     """Get list of names of nodes availalbe on the local Slicer server.
     Nodes can be selected using name, id, and/or class_name.
     """
-    api_url = f"http://localhost:{SERVER_PORT}/slicer/mrml/names"
+    api_url = f"http://127.0.0.1:{SERVER_PORT}/slicer/mrml/names"
     node_query = _node_query_parameters(name, id, class_name)
     if node_query:
         api_url += "?" + node_query
     response = requests.get(api_url)
     _report_error(response)
     return response.json()
 
 def file_save(file_path, name=None, id=None, class_name=None, properties=None):
     """Save node into file on the local Slicer server.
     :param path: local filename or URL of the file to write
     :param properties: dictionary of additional properties. For example, `useCompression` specifies if the written file will be compressed.
     """
     import urllib
+
+    if file_path is not None:
+        file_path = str(file_path)
+
     url_encoded_path = urllib.request.quote(file_path, safe='')
-    api_url = f"http://localhost:{SERVER_PORT}/slicer/mrml/file?localfile={url_encoded_path}"
+    api_url = f"http://127.0.0.1:{SERVER_PORT}/slicer/mrml/file?localfile={url_encoded_path}"
     node_query = _node_query_parameters(name, id, "")
     if node_query:
         api_url += "&" + node_query
     if properties:
         for key in properties:
             url_encoded_key = urllib.request.quote(key.encode(), safe='')
             url_encoded_value = urllib.request.quote(str(properties[key]).encode(), safe='')
@@ -158,27 +162,31 @@
     :param auto_start: automatically start a Slicer application if a server not found at the specified port. Requires slicer_executable
         argument or `SLICER_EXECUTABLE` environment variable to be set to a Slicer executable (version 5.2 or later),
         such as `/Applications/Slicer.app/Contents/MacOS/Slicer` or `c:/Users/username/appdata/Local/NA-MIC/Slicer 5.2.0/Slicer.exe`
     :param slicer_executable: Slicer application main executable. Used if `auto_start` is enabled.
     :return: list of loaded node IDs (they can be used in further queries).
     """
     import urllib
+
+    if file_path is not None:
+        file_path = str(file_path)
+
     if file_type is None:
         file_type = "VolumeFile"
     p = urllib.parse.urlparse(file_path)
     if p.scheme == 'slicer':
         # Slicer URL - use it as is. For example:
         # slicer://viewer/?studyUID=1.2.826.0.1.3680043.8.498.77209180964150541470378654317482622226&dicomweb_endpoint=http%3A%2F%2F130.15.7.119:2016%2Fdicom&bulk_retrieve=0
         url_encoded_path = urllib.request.quote(file_path, safe='')
-        api_url = f"http://localhost:{SERVER_PORT}/slicer/open?url={url_encoded_path}"
+        api_url = f"http://127.0.0.1:{SERVER_PORT}/slicer/open?url={url_encoded_path}"
     else:
         # Local file path or remote download path
         path_type = 'url' if p.scheme in ['http', 'https'] else 'localfile'
         url_encoded_path = urllib.request.quote(file_path, safe='')
-        api_url = f"http://localhost:{SERVER_PORT}/slicer/mrml?{path_type}={url_encoded_path}&filetype={file_type}"
+        api_url = f"http://127.0.0.1:{SERVER_PORT}/slicer/mrml?{path_type}={url_encoded_path}&filetype={file_type}"
         if properties:
             for key in properties:
                 url_encoded_key = urllib.request.quote(key.encode(), safe='')
                 url_encoded_value = urllib.request.quote(str(properties[key]).encode(), safe='')
                 api_url += f"&{url_encoded_key}={url_encoded_value}"
 
     retry_after_starting_server = True
```

