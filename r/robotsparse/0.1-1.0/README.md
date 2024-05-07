# Comparing `tmp/robotsparse-0.1.tar.gz` & `tmp/robotsparse-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotsparse-0.1.tar", last modified: Mon Apr 29 06:57:02 2024, max compression
+gzip compressed data, was "robotsparse-1.0.tar", last modified: Tue May  7 22:30:22 2024, max compression
```

## Comparing `robotsparse-0.1.tar` & `robotsparse-1.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 xyz       (1000) xyz       (1000)        0 2024-04-29 06:57:02.144661 robotsparse-0.1/
--rw-r--r--   0 xyz       (1000) xyz       (1000)     1061 2024-04-29 06:52:35.000000 robotsparse-0.1/LICENSE
--rw-r--r--   0 xyz       (1000) xyz       (1000)       24 2024-04-29 06:55:12.000000 robotsparse-0.1/MANIFEST.in
--rw-r--r--   0 xyz       (1000) xyz       (1000)     1592 2024-04-29 06:57:02.144661 robotsparse-0.1/PKG-INFO
--rw-r--r--   0 xyz       (1000) xyz       (1000)     1014 2024-04-29 06:45:08.000000 robotsparse-0.1/README.md
--rw-r--r--   0 xyz       (1000) xyz       (1000)       13 2024-04-29 06:54:46.000000 robotsparse-0.1/requirements.txt
-drwxr-xr-x   0 xyz       (1000) xyz       (1000)        0 2024-04-29 06:57:02.143661 robotsparse-0.1/robotsparse/
--rw-r--r--   0 xyz       (1000) xyz       (1000)     1673 2024-04-27 13:36:11.000000 robotsparse-0.1/robotsparse/__init__.py
-drwxr-xr-x   0 xyz       (1000) xyz       (1000)        0 2024-04-29 06:57:02.143661 robotsparse-0.1/robotsparse/utils/
--rw-r--r--   0 xyz       (1000) xyz       (1000)      339 2024-04-26 02:18:06.000000 robotsparse-0.1/robotsparse/utils/_regex.py
--rw-r--r--   0 xyz       (1000) xyz       (1000)      152 2024-04-26 11:40:59.000000 robotsparse-0.1/robotsparse/utils/exceptions.py
--rw-r--r--   0 xyz       (1000) xyz       (1000)     2386 2024-04-29 06:42:34.000000 robotsparse-0.1/robotsparse/utils/parser.py
-drwxr-xr-x   0 xyz       (1000) xyz       (1000)        0 2024-04-29 06:57:02.143661 robotsparse-0.1/robotsparse.egg-info/
--rw-r--r--   0 xyz       (1000) xyz       (1000)     1592 2024-04-29 06:57:02.000000 robotsparse-0.1/robotsparse.egg-info/PKG-INFO
--rw-r--r--   0 xyz       (1000) xyz       (1000)      341 2024-04-29 06:57:02.000000 robotsparse-0.1/robotsparse.egg-info/SOURCES.txt
--rw-r--r--   0 xyz       (1000) xyz       (1000)        1 2024-04-29 06:57:02.000000 robotsparse-0.1/robotsparse.egg-info/dependency_links.txt
--rw-r--r--   0 xyz       (1000) xyz       (1000)       14 2024-04-29 06:57:02.000000 robotsparse-0.1/robotsparse.egg-info/requires.txt
--rw-r--r--   0 xyz       (1000) xyz       (1000)       12 2024-04-29 06:57:02.000000 robotsparse-0.1/robotsparse.egg-info/top_level.txt
--rw-r--r--   0 xyz       (1000) xyz       (1000)       38 2024-04-29 06:57:02.144661 robotsparse-0.1/setup.cfg
--rw-r--r--   0 xyz       (1000) xyz       (1000)      947 2024-04-29 06:56:57.000000 robotsparse-0.1/setup.py
+drwxr-xr-x   0 xyz       (1000) xyz       (1000)        0 2024-05-07 22:30:22.839282 robotsparse-1.0/
+-rw-r--r--   0 xyz       (1000) xyz       (1000)     1061 2024-04-29 06:52:35.000000 robotsparse-1.0/LICENSE
+-rw-r--r--   0 xyz       (1000) xyz       (1000)       24 2024-04-29 06:55:12.000000 robotsparse-1.0/MANIFEST.in
+-rw-r--r--   0 xyz       (1000) xyz       (1000)     2277 2024-05-07 22:30:22.839282 robotsparse-1.0/PKG-INFO
+-rw-r--r--   0 xyz       (1000) xyz       (1000)     1443 2024-05-07 22:22:05.000000 robotsparse-1.0/README.md
+-rw-r--r--   0 xyz       (1000) xyz       (1000)       13 2024-04-29 06:54:46.000000 robotsparse-1.0/requirements.txt
+drwxr-xr-x   0 xyz       (1000) xyz       (1000)        0 2024-05-07 22:30:22.838282 robotsparse-1.0/robotsparse/
+-rw-r--r--   0 xyz       (1000) xyz       (1000)     3191 2024-05-07 22:30:15.000000 robotsparse-1.0/robotsparse/__init__.py
+drwxr-xr-x   0 xyz       (1000) xyz       (1000)        0 2024-05-07 22:30:22.838282 robotsparse-1.0/robotsparse/utils/
+-rw-r--r--   0 xyz       (1000) xyz       (1000)      339 2024-04-26 02:18:06.000000 robotsparse-1.0/robotsparse/utils/_regex.py
+-rw-r--r--   0 xyz       (1000) xyz       (1000)      152 2024-04-26 11:40:59.000000 robotsparse-1.0/robotsparse/utils/exceptions.py
+-rw-r--r--   0 xyz       (1000) xyz       (1000)     3120 2024-05-07 21:37:58.000000 robotsparse-1.0/robotsparse/utils/parser.py
+drwxr-xr-x   0 xyz       (1000) xyz       (1000)        0 2024-05-07 22:30:22.838282 robotsparse-1.0/robotsparse.egg-info/
+-rw-r--r--   0 xyz       (1000) xyz       (1000)     2277 2024-05-07 22:30:22.000000 robotsparse-1.0/robotsparse.egg-info/PKG-INFO
+-rw-r--r--   0 xyz       (1000) xyz       (1000)      341 2024-05-07 22:30:22.000000 robotsparse-1.0/robotsparse.egg-info/SOURCES.txt
+-rw-r--r--   0 xyz       (1000) xyz       (1000)        1 2024-05-07 22:30:22.000000 robotsparse-1.0/robotsparse.egg-info/dependency_links.txt
+-rw-r--r--   0 xyz       (1000) xyz       (1000)       14 2024-05-07 22:30:22.000000 robotsparse-1.0/robotsparse.egg-info/requires.txt
+-rw-r--r--   0 xyz       (1000) xyz       (1000)       12 2024-05-07 22:30:22.000000 robotsparse-1.0/robotsparse.egg-info/top_level.txt
+-rw-r--r--   0 xyz       (1000) xyz       (1000)       38 2024-05-07 22:30:22.839282 robotsparse-1.0/setup.cfg
+-rw-r--r--   0 xyz       (1000) xyz       (1000)     1233 2024-05-07 22:29:27.000000 robotsparse-1.0/setup.py
```

### Comparing `robotsparse-0.1/LICENSE` & `robotsparse-1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `robotsparse-0.1/PKG-INFO` & `robotsparse-1.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,45 +1,60 @@
 Metadata-Version: 2.1
 Name: robotsparse
-Version: 0.1
+Version: 1.0
 Summary: A python package that enhances speed and simplicity of parsing robots files.
-Home-page: 
+Home-page: https://github.com/xyzpw/robotsparse/
 Author: xyzpw
 Maintainer: xyzpw
 License: MIT
-Keywords: parsing,parser,robots,web-crawling,crawlers,crawling
+Keywords: parsing,parser,robots,web-crawling,crawlers,crawling,sitemaps,sitemap
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Text Processing
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Intended Audience :: Developers
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests==2.*
 
 # robotsparse
+![Pepy Total Downlods](https://img.shields.io/pepy/dt/robotsparse)<br>
 A python package that enhances speed and simplicity of parsing robots files.
 
 ## Usage
 Basic usage, such as getting robots contents:
 ```python
 import robotsparse
 
 #NOTE: The `find_url` parameter will redirect the url to the default robots location.
-robots = robotsparse.urlRobots("https://github.com/", find_url=True)
+robots = robotsparse.getRobots("https://github.com/", find_url=True)
 print(list(robots)) # output: ['user-agents']
 ```
 The `user-agents` key will contain each user-agent found in the robots file contents along with information associated with them.<br>
 
 Alternatively, we can assign the robots contents as an object, which allows faster accessability:
 ```python
 import robotsparse
 
 # This function returns a class.
-robots = robotsparse.getRobots("https://duckduckgo.com/", find_url=True)
+robots = robotsparse.getRobotsObject("https://duckduckgo.com/", find_url=True)
 assert isinstance(robots, object)
 print(robots.allow) # Prints allowed locations
 print(robots.disallow) # Prints disallowed locations
 print(robots.crawl_delay) # Prints found crawl-delays
 print(robots.robots) # This output is equivalent to the above example
 ```
 
+### Additional Features
+When parsing robots files, it sometimes may be useful to parse sitemap files:
+```python
+import robotsparse
+sitemap = robotsparse.getSitemap("https://pypi.org/", find_url=True)
+```
+The above code contains a variable named `sitemap` which contains information that looks like this:
+```python
+[{"url": "", "lastModified": ""}]
+```
```

### Comparing `robotsparse-0.1/README.md` & `robotsparse-1.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,38 @@
 # robotsparse
+![Pepy Total Downlods](https://img.shields.io/pepy/dt/robotsparse)<br>
 A python package that enhances speed and simplicity of parsing robots files.
 
 ## Usage
 Basic usage, such as getting robots contents:
 ```python
 import robotsparse
 
 #NOTE: The `find_url` parameter will redirect the url to the default robots location.
-robots = robotsparse.urlRobots("https://github.com/", find_url=True)
+robots = robotsparse.getRobots("https://github.com/", find_url=True)
 print(list(robots)) # output: ['user-agents']
 ```
 The `user-agents` key will contain each user-agent found in the robots file contents along with information associated with them.<br>
 
 Alternatively, we can assign the robots contents as an object, which allows faster accessability:
 ```python
 import robotsparse
 
 # This function returns a class.
-robots = robotsparse.getRobots("https://duckduckgo.com/", find_url=True)
+robots = robotsparse.getRobotsObject("https://duckduckgo.com/", find_url=True)
 assert isinstance(robots, object)
 print(robots.allow) # Prints allowed locations
 print(robots.disallow) # Prints disallowed locations
 print(robots.crawl_delay) # Prints found crawl-delays
 print(robots.robots) # This output is equivalent to the above example
 ```
 
+### Additional Features
+When parsing robots files, it sometimes may be useful to parse sitemap files:
+```python
+import robotsparse
+sitemap = robotsparse.getSitemap("https://pypi.org/", find_url=True)
+```
+The above code contains a variable named `sitemap` which contains information that looks like this:
+```python
+[{"url": "", "lastModified": ""}]
+```
```

### Comparing `robotsparse-0.1/robotsparse/utils/parser.py` & `robotsparse-1.0/robotsparse/utils/parser.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import re
 from .exceptions import *
+from ._regex import searchForGroup
 
-def getRobotsContents(robotsContent: str) -> dict:
+def getRobotsInfo(robotsContent: str) -> dict:
     robotsContent = re.sub(r"\n{1,}", "\n", robotsContent)
     robots = {}
     userAgents = {}
     userAgentIter = re.finditer(
         r"^user-agent: (?P<ua>.*?)(?:$|\s?#)\n(?P<rules>.*?)(?=user-agent|\Z)",
         robotsContent,
         flags=(re.MULTILINE | re.DOTALL | re.IGNORECASE),
@@ -30,18 +31,40 @@
         robotsContent,
         flags=(re.MULTILINE | re.DOTALL | re.IGNORECASE),
     )
     if userAgents != {}: robots["user-agents"] = userAgents
     if sitemaps != []: robots["sitemaps"] = list(set(sitemaps))
     return robots if robots != {} else None
 
+def getXmlSitemapInfo(sitemapContent: str) -> dict:
+    sitemapContent = re.sub(r"\n{1,}", "", sitemapContent, flags=(re.DOTALL | re.MULTILINE))
+    innerUrls = re.findall(
+        r"<\s*(sitemap|url).*?>(.*?)<\s*/\s*\1\s*>",
+        sitemapContent,
+        re.DOTALL | re.MULTILINE
+    )
+    sitemapInfo = []
+    for i in innerUrls:
+        loc = searchForGroup(
+            r"<\s*loc\s*>(.*?)<\s*/\s*loc\s*>",
+            i[1],
+            1
+        )
+        lastmod = searchForGroup(
+            r"<\s*lastmod\s*>(.*?)<\s*/\s*lastmod\s*>",
+            i[1],
+            1
+        )
+        sitemapInfo.append({"url": loc, "lastModified": lastmod})
+    return sitemapInfo if bool(sitemapInfo) else None
+
 class Robots:
     """Contains parsed robots information."""
     def __init__(self, fileContents: str):
-        self.robots = getRobotsContents(fileContents)
+        self.robots = getRobotsInfo(fileContents)
         if self.robots == None:
             return
         self.user_agents = list(self.robots.get("user-agents"))
         self.sitemaps = self.robots.get("sitemaps")
         if self.user_agents != None:
             keysToSearch = ["allow", "disallow", "crawl-delay"]
             for ua in self.user_agents:
```

### Comparing `robotsparse-0.1/robotsparse.egg-info/PKG-INFO` & `robotsparse-1.0/robotsparse.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,45 +1,60 @@
 Metadata-Version: 2.1
 Name: robotsparse
-Version: 0.1
+Version: 1.0
 Summary: A python package that enhances speed and simplicity of parsing robots files.
-Home-page: 
+Home-page: https://github.com/xyzpw/robotsparse/
 Author: xyzpw
 Maintainer: xyzpw
 License: MIT
-Keywords: parsing,parser,robots,web-crawling,crawlers,crawling
+Keywords: parsing,parser,robots,web-crawling,crawlers,crawling,sitemaps,sitemap
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Text Processing
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Intended Audience :: Developers
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests==2.*
 
 # robotsparse
+![Pepy Total Downlods](https://img.shields.io/pepy/dt/robotsparse)<br>
 A python package that enhances speed and simplicity of parsing robots files.
 
 ## Usage
 Basic usage, such as getting robots contents:
 ```python
 import robotsparse
 
 #NOTE: The `find_url` parameter will redirect the url to the default robots location.
-robots = robotsparse.urlRobots("https://github.com/", find_url=True)
+robots = robotsparse.getRobots("https://github.com/", find_url=True)
 print(list(robots)) # output: ['user-agents']
 ```
 The `user-agents` key will contain each user-agent found in the robots file contents along with information associated with them.<br>
 
 Alternatively, we can assign the robots contents as an object, which allows faster accessability:
 ```python
 import robotsparse
 
 # This function returns a class.
-robots = robotsparse.getRobots("https://duckduckgo.com/", find_url=True)
+robots = robotsparse.getRobotsObject("https://duckduckgo.com/", find_url=True)
 assert isinstance(robots, object)
 print(robots.allow) # Prints allowed locations
 print(robots.disallow) # Prints disallowed locations
 print(robots.crawl_delay) # Prints found crawl-delays
 print(robots.robots) # This output is equivalent to the above example
 ```
 
+### Additional Features
+When parsing robots files, it sometimes may be useful to parse sitemap files:
+```python
+import robotsparse
+sitemap = robotsparse.getSitemap("https://pypi.org/", find_url=True)
+```
+The above code contains a variable named `sitemap` which contains information that looks like this:
+```python
+[{"url": "", "lastModified": ""}]
+```
```

