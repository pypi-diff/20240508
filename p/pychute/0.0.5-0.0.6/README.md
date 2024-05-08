# Comparing `tmp/pychute-0.0.5.tar.gz` & `tmp/pychute-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pychute-0.0.5.tar", last modified: Tue May  7 17:49:40 2024, max compression
+gzip compressed data, was "pychute-0.0.6.tar", last modified: Wed May  8 07:17:59 2024, max compression
```

## Comparing `pychute-0.0.5.tar` & `pychute-0.0.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 17:49:40.530773 pychute-0.0.5/
--rw-rw-rw-   0        0        0     1090 2024-05-07 10:43:46.000000 pychute-0.0.5/LICENSE
--rw-rw-rw-   0        0        0     3914 2024-05-07 17:49:40.528085 pychute-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     1968 2024-05-07 17:37:40.000000 pychute-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2024-05-07 17:49:40.505893 pychute-0.0.5/pychute/
--rw-rw-rw-   0        0        0      196 2024-05-07 16:42:55.000000 pychute-0.0.5/pychute/__init__.py
--rw-rw-rw-   0        0        0      110 2024-05-07 16:37:24.000000 pychute-0.0.5/pychute/config.py
--rw-rw-rw-   0        0        0      669 2024-05-07 10:59:12.000000 pychute-0.0.5/pychute/helpers.py
--rw-rw-rw-   0        0        0     3732 2024-05-07 17:48:46.000000 pychute-0.0.5/pychute/main.py
-drwxrwxrwx   0        0        0        0 2024-05-07 17:49:40.525066 pychute-0.0.5/pychute.egg-info/
--rw-rw-rw-   0        0        0     3914 2024-05-07 17:49:40.000000 pychute-0.0.5/pychute.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      318 2024-05-07 17:49:40.000000 pychute-0.0.5/pychute.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 17:49:40.000000 pychute-0.0.5/pychute.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2024-05-07 17:49:40.000000 pychute-0.0.5/pychute.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-07 17:49:40.000000 pychute-0.0.5/pychute.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      786 2024-05-07 17:49:13.000000 pychute-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-07 17:49:40.530773 pychute-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      643 2024-05-07 17:49:13.000000 pychute-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-07 17:49:40.522066 pychute-0.0.5/tests/
--rw-rw-rw-   0        0        0      937 2024-05-07 16:42:56.000000 pychute-0.0.5/tests/test_functionality.py
--rw-rw-rw-   0        0        0      915 2024-05-07 16:44:38.000000 pychute-0.0.5/tests/test_helpers.py
+drwxrwxrwx   0        0        0        0 2024-05-08 07:17:59.938634 pychute-0.0.6/
+-rw-rw-rw-   0        0        0     1090 2024-05-07 10:43:46.000000 pychute-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0     3968 2024-05-08 07:17:59.935110 pychute-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2022 2024-05-08 07:15:52.000000 pychute-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-08 07:17:59.915846 pychute-0.0.6/pychute/
+-rw-rw-rw-   0        0        0      196 2024-05-07 16:42:55.000000 pychute-0.0.6/pychute/__init__.py
+-rw-rw-rw-   0        0        0      110 2024-05-07 16:37:24.000000 pychute-0.0.6/pychute/config.py
+-rw-rw-rw-   0        0        0      669 2024-05-07 10:59:12.000000 pychute-0.0.6/pychute/helpers.py
+-rw-rw-rw-   0        0        0     4178 2024-05-07 23:06:47.000000 pychute-0.0.6/pychute/main.py
+drwxrwxrwx   0        0        0        0 2024-05-08 07:17:59.933467 pychute-0.0.6/pychute.egg-info/
+-rw-rw-rw-   0        0        0     3968 2024-05-08 07:17:59.000000 pychute-0.0.6/pychute.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      318 2024-05-08 07:17:59.000000 pychute-0.0.6/pychute.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 07:17:59.000000 pychute-0.0.6/pychute.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2024-05-08 07:17:59.000000 pychute-0.0.6/pychute.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-08 07:17:59.000000 pychute-0.0.6/pychute.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      786 2024-05-08 07:16:57.000000 pychute-0.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-08 07:17:59.938634 pychute-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      643 2024-05-08 07:16:57.000000 pychute-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 07:17:59.930949 pychute-0.0.6/tests/
+-rw-rw-rw-   0        0        0     1272 2024-05-07 23:15:03.000000 pychute-0.0.6/tests/test_functionality.py
+-rw-rw-rw-   0        0        0      915 2024-05-07 16:44:38.000000 pychute-0.0.6/tests/test_helpers.py
```

### Comparing `pychute-0.0.5/LICENSE` & `pychute-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pychute-0.0.5/PKG-INFO` & `pychute-0.0.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pychute
-Version: 0.0.5
+Version: 0.0.6
 Summary: A library that helps downloading videos from bitchute.com
 Home-page: http://github.com/paichiwo/pychute
 Author: Lukasz Zerucha
 Author-email: Lukasz Zerucha <lzerucha@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Lukasz Zerucha
@@ -98,15 +98,15 @@
 
 ```python
 from pychute import PyChute
 
 url = "bitchute url"
 
 pc = PyChute(url=url)
-output_path = f"D:\\Downloads/{pc.title()}"
+output_path = f"D:\\Downloads/{pc.title()}.mp4"
 
 pc.download()
 ```
 
 ---
 
 #### Other data
@@ -114,15 +114,15 @@
 
 ```python
 from pychute import PyChute
 
 url = "bitchute url"
 
 pc = PyChute(url=url)
-output_path = f"D:\\Downloads/{pc.title()}"
+output_path = f"D:\\Downloads/{pc.title()}.mp4"
 
 # video title
 print(pc.title())
 
 # channel name
 print(pc.channel())
 
@@ -136,8 +136,11 @@
 print(pc.subscriptions())
 
 # video likes
 print(pc.likes())
 
 # video views
 print(pc.views())
+
+# file size in bytes
+print(pc.filesize())
 ```
```

### Comparing `pychute-0.0.5/README.md` & `pychute-0.0.6/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 
 ```python
 from pychute import PyChute
 
 url = "bitchute url"
 
 pc = PyChute(url=url)
-output_path = f"D:\\Downloads/{pc.title()}"
+output_path = f"D:\\Downloads/{pc.title()}.mp4"
 
 pc.download()
 ```
 
 ---
 
 #### Other data
@@ -74,15 +74,15 @@
 
 ```python
 from pychute import PyChute
 
 url = "bitchute url"
 
 pc = PyChute(url=url)
-output_path = f"D:\\Downloads/{pc.title()}"
+output_path = f"D:\\Downloads/{pc.title()}.mp4"
 
 # video title
 print(pc.title())
 
 # channel name
 print(pc.channel())
 
@@ -96,8 +96,11 @@
 print(pc.subscriptions())
 
 # video likes
 print(pc.likes())
 
 # video views
 print(pc.views())
+
+# file size in bytes
+print(pc.filesize())
 ```
```

### Comparing `pychute-0.0.5/pychute/helpers.py` & `pychute-0.0.6/pychute/helpers.py`

 * *Files identical despite different names*

### Comparing `pychute-0.0.5/pychute/main.py` & `pychute-0.0.6/pychute/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -83,14 +83,24 @@
     def length(self) -> str:
         result = self.__soup.find('meta', {'name': 'duration'}).get('content')
         if result:
             return format_duration_string(result)
         else:
             raise Exception('Video length could not be fetched')
 
+    def filesize(self) -> int:
+        result = self.__tree.xpath('//*[@id="player"]/source')
+        if len(result) != 0:
+            target = result[0].get('src')
+            request = urllib.request.Request(target, method='HEAD')
+            response = urllib.request.urlopen(request)
+            return int(response.headers.get('Content-Length', 0))
+        else:
+            raise Exception('Source for the video does not exist')
+
     def download(self, on_progress_callback=None, filename=None):
         result = self.__tree.xpath('//*[@id="player"]/source')
 
         if len(result) != 0:
             target = result[0].get('src')
             output_filename = f'{filename if filename else self.title()}.mp4'  # add extension
```

### Comparing `pychute-0.0.5/pychute.egg-info/PKG-INFO` & `pychute-0.0.6/pychute.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pychute
-Version: 0.0.5
+Version: 0.0.6
 Summary: A library that helps downloading videos from bitchute.com
 Home-page: http://github.com/paichiwo/pychute
 Author: Lukasz Zerucha
 Author-email: Lukasz Zerucha <lzerucha@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Lukasz Zerucha
@@ -98,15 +98,15 @@
 
 ```python
 from pychute import PyChute
 
 url = "bitchute url"
 
 pc = PyChute(url=url)
-output_path = f"D:\\Downloads/{pc.title()}"
+output_path = f"D:\\Downloads/{pc.title()}.mp4"
 
 pc.download()
 ```
 
 ---
 
 #### Other data
@@ -114,15 +114,15 @@
 
 ```python
 from pychute import PyChute
 
 url = "bitchute url"
 
 pc = PyChute(url=url)
-output_path = f"D:\\Downloads/{pc.title()}"
+output_path = f"D:\\Downloads/{pc.title()}.mp4"
 
 # video title
 print(pc.title())
 
 # channel name
 print(pc.channel())
 
@@ -136,8 +136,11 @@
 print(pc.subscriptions())
 
 # video likes
 print(pc.likes())
 
 # video views
 print(pc.views())
+
+# file size in bytes
+print(pc.filesize())
 ```
```

### Comparing `pychute-0.0.5/pyproject.toml` & `pychute-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pychute"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Lukasz Zerucha", email="lzerucha@gmail.com" },
 ]
 description = "A library that helps downloading videos from bitchute.com"
 readme = "README.md"
 requires-python = ">=3.8"
 license={file="LICENSE"}
```

### Comparing `pychute-0.0.5/setup.py` & `pychute-0.0.6/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_desc = f.read()
 
 setup(
     name='pychute',
-    version='0.0.5',
+    version='0.0.6',
     packages=setuptools.find_packages(),
     url='http://github.com/paichiwo/pychute',
     author='Lukasz Zerucha',
     author_email='lzerucha@gmail.com',
     description='A library that helps downloading videos from bitchute.com',
     long_description=long_desc,
     long_description_content_type='text/markdown',
```

### Comparing `pychute-0.0.5/tests/test_functionality.py` & `pychute-0.0.6/tests/test_functionality.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,39 @@
 import time
 from pychute.main import PyChute
 
 if __name__ == '__main__':
 
     start_time = time.time()
 
+    def format_file_size(size_bytes) -> str:
+        """Convert bytes to MB / GB"""
+        if size_bytes >= 1024 ** 3:
+            return f'{(size_bytes / (1024 ** 3)):.2f} GB'
+        else:
+            return f'{(size_bytes / (1024 ** 2)):.2f} MB'
+
     def report_hook(count, block_size, total_size):
+        print(total_size)
         # progress percentage
         progress = min(1.0, float(count * block_size) / total_size)
         print(progress)
 
         # download speed
         elapsed_time = time.time() - start_time
         if elapsed_time > 0:
             speed = (count * block_size) / (1024 * elapsed_time)  # speed in KB/s
             print(f'Download speed: {speed:.2f} KB/s')
 
     link1 = 'https://www.bitchute.com/video/n75YV5it6lHm/'
     link2 = 'https://www.bitchute.com/video/C8dHQCDlRlvY/'
 
-    pc = PyChute(url=link2)
-    pc.download(on_progress_callback=report_hook, filename='d:\\test')
+    pc = PyChute(url=link1)
+    # pc.download(on_progress_callback=report_hook, filename='d:\\test_a')
     print(pc.title())
     print(pc.channel())
     print(pc.publish_date())
     print(pc.length())
     print(pc.subscriptions())
     print(pc.likes())
-    print(pc.views())
+    print(pc.views())
+    print(format_file_size(pc.filesize()))
```

### Comparing `pychute-0.0.5/tests/test_helpers.py` & `pychute-0.0.6/tests/test_helpers.py`

 * *Files identical despite different names*

