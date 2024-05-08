# Comparing `tmp/pychute-0.0.6.tar.gz` & `tmp/pychute-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pychute-0.0.6.tar", last modified: Wed May  8 07:17:59 2024, max compression
+gzip compressed data, was "pychute-0.0.7.tar", last modified: Wed May  8 16:46:17 2024, max compression
```

## Comparing `pychute-0.0.6.tar` & `pychute-0.0.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 07:17:59.938634 pychute-0.0.6/
--rw-rw-rw-   0        0        0     1090 2024-05-07 10:43:46.000000 pychute-0.0.6/LICENSE
--rw-rw-rw-   0        0        0     3968 2024-05-08 07:17:59.935110 pychute-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     2022 2024-05-08 07:15:52.000000 pychute-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2024-05-08 07:17:59.915846 pychute-0.0.6/pychute/
--rw-rw-rw-   0        0        0      196 2024-05-07 16:42:55.000000 pychute-0.0.6/pychute/__init__.py
--rw-rw-rw-   0        0        0      110 2024-05-07 16:37:24.000000 pychute-0.0.6/pychute/config.py
--rw-rw-rw-   0        0        0      669 2024-05-07 10:59:12.000000 pychute-0.0.6/pychute/helpers.py
--rw-rw-rw-   0        0        0     4178 2024-05-07 23:06:47.000000 pychute-0.0.6/pychute/main.py
-drwxrwxrwx   0        0        0        0 2024-05-08 07:17:59.933467 pychute-0.0.6/pychute.egg-info/
--rw-rw-rw-   0        0        0     3968 2024-05-08 07:17:59.000000 pychute-0.0.6/pychute.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      318 2024-05-08 07:17:59.000000 pychute-0.0.6/pychute.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 07:17:59.000000 pychute-0.0.6/pychute.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2024-05-08 07:17:59.000000 pychute-0.0.6/pychute.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-08 07:17:59.000000 pychute-0.0.6/pychute.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      786 2024-05-08 07:16:57.000000 pychute-0.0.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-08 07:17:59.938634 pychute-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      643 2024-05-08 07:16:57.000000 pychute-0.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-08 07:17:59.930949 pychute-0.0.6/tests/
--rw-rw-rw-   0        0        0     1272 2024-05-07 23:15:03.000000 pychute-0.0.6/tests/test_functionality.py
--rw-rw-rw-   0        0        0      915 2024-05-07 16:44:38.000000 pychute-0.0.6/tests/test_helpers.py
+drwxrwxrwx   0        0        0        0 2024-05-08 16:46:17.868662 pychute-0.0.7/
+-rw-rw-rw-   0        0        0     1090 2024-05-07 10:43:46.000000 pychute-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0     3971 2024-05-08 16:46:17.865395 pychute-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     2046 2024-05-08 16:43:00.000000 pychute-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2024-05-08 16:46:17.840649 pychute-0.0.7/pychute/
+-rw-rw-rw-   0        0        0      196 2024-05-07 16:42:55.000000 pychute-0.0.7/pychute/__init__.py
+-rw-rw-rw-   0        0        0      110 2024-05-07 16:37:24.000000 pychute-0.0.7/pychute/config.py
+-rw-rw-rw-   0        0        0      669 2024-05-07 10:59:12.000000 pychute-0.0.7/pychute/helpers.py
+-rw-rw-rw-   0        0        0     3982 2024-05-08 16:40:03.000000 pychute-0.0.7/pychute/main.py
+drwxrwxrwx   0        0        0        0 2024-05-08 16:46:17.863539 pychute-0.0.7/pychute.egg-info/
+-rw-rw-rw-   0        0        0     3971 2024-05-08 16:46:17.000000 pychute-0.0.7/pychute.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      318 2024-05-08 16:46:17.000000 pychute-0.0.7/pychute.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 16:46:17.000000 pychute-0.0.7/pychute.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2024-05-08 16:46:17.000000 pychute-0.0.7/pychute.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-08 16:46:17.000000 pychute-0.0.7/pychute.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      760 2024-05-08 16:40:03.000000 pychute-0.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-08 16:46:17.868662 pychute-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      635 2024-05-08 16:40:03.000000 pychute-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 16:46:17.860091 pychute-0.0.7/tests/
+-rw-rw-rw-   0        0        0     1252 2024-05-08 16:43:00.000000 pychute-0.0.7/tests/test_functionality.py
+-rw-rw-rw-   0        0        0      915 2024-05-07 16:44:38.000000 pychute-0.0.7/tests/test_helpers.py
```

### Comparing `pychute-0.0.6/LICENSE` & `pychute-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pychute-0.0.6/PKG-INFO` & `pychute-0.0.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pychute
-Version: 0.0.6
+Version: 0.0.7
 Summary: A library that helps downloading videos from bitchute.com
 Home-page: http://github.com/paichiwo/pychute
 Author: Lukasz Zerucha
 Author-email: Lukasz Zerucha <lzerucha@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Lukasz Zerucha
@@ -30,42 +30,41 @@
 Project-URL: Issues, https://github.com/paichiwo/pychute/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: lxml
 Requires-Dist: selenium
 Requires-Dist: beautifulsoup4
 
-# pychute
+# PyChute
 
 
 ### A library that helps download videos from BitChute website
 
 
----
 
 ### Installation:
 `pip install pychute`
 
 ### How to use:
 ```python
 from pychute import PyChute
 
 url = "bitchute url"
 
 pc = PyChute(url=url)
 pc.download()
 ```
----
+
 
 ### Additional features:
 
+
 #### Progress callback
 If you need to get progress like percentage or download speed, you can create a function 
 and pass as a parameter in the download method.
 
 ```python
 import time
 from pychute import PyChute
@@ -86,61 +85,63 @@
 
 
 url = "bitchute url"
 
 pc = PyChute(url=url)
 pc.download(on_progress_callback=show_progress)
 ```
-___
+
 
 #### Filename
 You can pass filename as a parameter in the form of a string to specify download location.
 Using download method without the `filename` parameter will save the file to where your script is located.
 
 ```python
 from pychute import PyChute
 
 url = "bitchute url"
 
 pc = PyChute(url=url)
-output_path = f"D:\\Downloads/{pc.title()}.mp4"
+output_path = f"D:\\Downloads/{pc.title()}"
 
 pc.download()
 ```
 
----
 
 #### Other data
 Apart from downloading, you can access other data about BitChute video:
 
 ```python
 from pychute import PyChute
 
 url = "bitchute url"
 
 pc = PyChute(url=url)
-output_path = f"D:\\Downloads/{pc.title()}.mp4"
+output_path = f"D:\\Downloads/{pc.title()}"
 
 # video title
 print(pc.title())
 
 # channel name
 print(pc.channel())
 
 # video publish date
 print(pc.publish_date())
 
 # video duration
-print(pc.length())
+print(pc.duration())
 
 # subscriptions number
 print(pc.subscriptions())
 
 # video likes
 print(pc.likes())
 
 # video views
 print(pc.views())
 
 # file size in bytes
 print(pc.filesize())
+
+# thumbnail image
+print(pc.thumbnail())
 ```
```

### Comparing `pychute-0.0.6/README.md` & `pychute-0.0.7/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-# pychute
+# PyChute
 
 
 ### A library that helps download videos from BitChute website
 
 
----
 
 ### Installation:
 `pip install pychute`
 
 ### How to use:
 ```python
 from pychute import PyChute
 
 url = "bitchute url"
 
 pc = PyChute(url=url)
 pc.download()
 ```
----
+
 
 ### Additional features:
 
+
 #### Progress callback
 If you need to get progress like percentage or download speed, you can create a function 
 and pass as a parameter in the download method.
 
 ```python
 import time
 from pychute import PyChute
@@ -46,61 +46,63 @@
 
 
 url = "bitchute url"
 
 pc = PyChute(url=url)
 pc.download(on_progress_callback=show_progress)
 ```
-___
+
 
 #### Filename
 You can pass filename as a parameter in the form of a string to specify download location.
 Using download method without the `filename` parameter will save the file to where your script is located.
 
 ```python
 from pychute import PyChute
 
 url = "bitchute url"
 
 pc = PyChute(url=url)
-output_path = f"D:\\Downloads/{pc.title()}.mp4"
+output_path = f"D:\\Downloads/{pc.title()}"
 
 pc.download()
 ```
 
----
 
 #### Other data
 Apart from downloading, you can access other data about BitChute video:
 
 ```python
 from pychute import PyChute
 
 url = "bitchute url"
 
 pc = PyChute(url=url)
-output_path = f"D:\\Downloads/{pc.title()}.mp4"
+output_path = f"D:\\Downloads/{pc.title()}"
 
 # video title
 print(pc.title())
 
 # channel name
 print(pc.channel())
 
 # video publish date
 print(pc.publish_date())
 
 # video duration
-print(pc.length())
+print(pc.duration())
 
 # subscriptions number
 print(pc.subscriptions())
 
 # video likes
 print(pc.likes())
 
 # video views
 print(pc.views())
 
 # file size in bytes
 print(pc.filesize())
+
+# thumbnail image
+print(pc.thumbnail())
 ```
```

### Comparing `pychute-0.0.6/pychute/helpers.py` & `pychute-0.0.7/pychute/helpers.py`

 * *Files identical despite different names*

### Comparing `pychute-0.0.6/pychute/main.py` & `pychute-0.0.7/pychute/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,22 @@
 import os
 import urllib.request
-from lxml import html
 from bs4 import BeautifulSoup
 from selenium import webdriver
 from pychute.config import USER_AGENT
 from pychute.helpers import format_duration_string, format_date_string
 
 
 class PyChute:
     def __init__(self, url):
         """Lightweight Bitchute wrapper """
 
         # Initial setup for the wrapper
         if url:
 
-            # --------- urllib -----------
-            headers = {'User-Agent': USER_AGENT}
-            request = urllib.request.Request(url, headers=headers)
-            html_page = urllib.request.urlopen(request).read()
-            if html_page:
-                self.__tree = html.document_fromstring(html_page)
-            else:
-                raise Exception('URL could not be fetched')
-
-            # -------- selenium ----------
             options = webdriver.ChromeOptions()
             options.add_argument('headless')
             options.add_argument(f'user-agent={USER_AGENT}')
             driver = webdriver.Chrome(options=options)
             driver.get(url)
             page = driver.page_source
             if page:
@@ -76,40 +65,47 @@
     def subscriptions(self) -> str:
         result = self.__soup.find('span', {'id': 'subscriber_count'}).text
         if result:
             return result
         else:
             raise Exception('Subscriptions could not be fetched')
 
-    def length(self) -> str:
+    def duration(self) -> str:
         result = self.__soup.find('meta', {'name': 'duration'}).get('content')
         if result:
             return format_duration_string(result)
         else:
-            raise Exception('Video length could not be fetched')
+            raise Exception('Video duration could not be fetched')
 
     def filesize(self) -> int:
-        result = self.__tree.xpath('//*[@id="player"]/source')
+        result = self.__soup.find('div', {'id': 'player'})
+
         if len(result) != 0:
-            target = result[0].get('src')
+            target = result.find('source').get('src')
             request = urllib.request.Request(target, method='HEAD')
             response = urllib.request.urlopen(request)
             return int(response.headers.get('Content-Length', 0))
         else:
             raise Exception('Source for the video does not exist')
 
+    def thumbnail(self) -> str:
+        result = self.__soup.find('div', {'id': 'player'})
+        if len(result) != 0:
+            return result.find('img').get('src')
+        else:
+            raise Exception('Thumbnail could not be fetched')
+
     def download(self, on_progress_callback=None, filename=None):
-        result = self.__tree.xpath('//*[@id="player"]/source')
+        result = self.__soup.find('div', {'id': 'player'})
 
         if len(result) != 0:
-            target = result[0].get('src')
+            target = result.find('source').get('src')
             output_filename = f'{filename if filename else self.title()}.mp4'  # add extension
 
             if not os.path.exists(output_filename):
                 print('Downloading...')
                 urllib.request.urlretrieve(target, output_filename, reporthook=on_progress_callback)
-
             else:
                 print('File already downloaded')
 
         else:
             raise Exception('Source for the video does not exist')
```

### Comparing `pychute-0.0.6/pychute.egg-info/PKG-INFO` & `pychute-0.0.7/pychute.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pychute
-Version: 0.0.6
+Version: 0.0.7
 Summary: A library that helps downloading videos from bitchute.com
 Home-page: http://github.com/paichiwo/pychute
 Author: Lukasz Zerucha
 Author-email: Lukasz Zerucha <lzerucha@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Lukasz Zerucha
@@ -30,42 +30,41 @@
 Project-URL: Issues, https://github.com/paichiwo/pychute/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: lxml
 Requires-Dist: selenium
 Requires-Dist: beautifulsoup4
 
-# pychute
+# PyChute
 
 
 ### A library that helps download videos from BitChute website
 
 
----
 
 ### Installation:
 `pip install pychute`
 
 ### How to use:
 ```python
 from pychute import PyChute
 
 url = "bitchute url"
 
 pc = PyChute(url=url)
 pc.download()
 ```
----
+
 
 ### Additional features:
 
+
 #### Progress callback
 If you need to get progress like percentage or download speed, you can create a function 
 and pass as a parameter in the download method.
 
 ```python
 import time
 from pychute import PyChute
@@ -86,61 +85,63 @@
 
 
 url = "bitchute url"
 
 pc = PyChute(url=url)
 pc.download(on_progress_callback=show_progress)
 ```
-___
+
 
 #### Filename
 You can pass filename as a parameter in the form of a string to specify download location.
 Using download method without the `filename` parameter will save the file to where your script is located.
 
 ```python
 from pychute import PyChute
 
 url = "bitchute url"
 
 pc = PyChute(url=url)
-output_path = f"D:\\Downloads/{pc.title()}.mp4"
+output_path = f"D:\\Downloads/{pc.title()}"
 
 pc.download()
 ```
 
----
 
 #### Other data
 Apart from downloading, you can access other data about BitChute video:
 
 ```python
 from pychute import PyChute
 
 url = "bitchute url"
 
 pc = PyChute(url=url)
-output_path = f"D:\\Downloads/{pc.title()}.mp4"
+output_path = f"D:\\Downloads/{pc.title()}"
 
 # video title
 print(pc.title())
 
 # channel name
 print(pc.channel())
 
 # video publish date
 print(pc.publish_date())
 
 # video duration
-print(pc.length())
+print(pc.duration())
 
 # subscriptions number
 print(pc.subscriptions())
 
 # video likes
 print(pc.likes())
 
 # video views
 print(pc.views())
 
 # file size in bytes
 print(pc.filesize())
+
+# thumbnail image
+print(pc.thumbnail())
 ```
```

### Comparing `pychute-0.0.6/pyproject.toml` & `pychute-0.0.7/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,34 +1,32 @@
 [project]
 name = "pychute"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Lukasz Zerucha", email="lzerucha@gmail.com" },
 ]
 description = "A library that helps downloading videos from bitchute.com"
 readme = "README.md"
 requires-python = ">=3.8"
 license={file="LICENSE"}
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-    "lxml",
     "selenium",
     "beautifulsoup4"
 ]
 
 [project.urls]
 Homepage = "https://github.com/paichiwo/pychute"
 Issues = "https://github.com/paichiwo/pychute/issues"
 
 [build-system]
 requires = [
     "setuptools>=42",
     "wheel",
-    "lxml",
     "selenium",
     "beautifulsoup4",
 ]
 build-backend = "setuptools.build_meta"
```

### Comparing `pychute-0.0.6/setup.py` & `pychute-0.0.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_desc = f.read()
 
 setup(
     name='pychute',
-    version='0.0.6',
+    version='0.0.7',
     packages=setuptools.find_packages(),
     url='http://github.com/paichiwo/pychute',
     author='Lukasz Zerucha',
     author_email='lzerucha@gmail.com',
     description='A library that helps downloading videos from bitchute.com',
     long_description=long_desc,
     long_description_content_type='text/markdown',
     keywords=['bitchute', 'downloader', 'youtube-dl', 'pytube', 'video']
 )
 
-install_requires = ['lxml', 'beautifulsoup4', 'selenium']
+install_requires = ['beautifulsoup4', 'selenium']
```

### Comparing `pychute-0.0.6/tests/test_functionality.py` & `pychute-0.0.7/tests/test_functionality.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,31 +9,31 @@
         """Convert bytes to MB / GB"""
         if size_bytes >= 1024 ** 3:
             return f'{(size_bytes / (1024 ** 3)):.2f} GB'
         else:
             return f'{(size_bytes / (1024 ** 2)):.2f} MB'
 
     def report_hook(count, block_size, total_size):
-        print(total_size)
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
 
-    pc = PyChute(url=link1)
-    # pc.download(on_progress_callback=report_hook, filename='d:\\test_a')
+    pc = PyChute(url=link2)
+    pc.download(on_progress_callback=report_hook, filename='d:\\test')
     print(pc.title())
     print(pc.channel())
     print(pc.publish_date())
-    print(pc.length())
+    print(pc.duration())
     print(pc.subscriptions())
     print(pc.likes())
     print(pc.views())
-    print(format_file_size(pc.filesize()))
+    print(pc.filesize())
+    print(pc.thumbnail())
```

### Comparing `pychute-0.0.6/tests/test_helpers.py` & `pychute-0.0.7/tests/test_helpers.py`

 * *Files identical despite different names*

