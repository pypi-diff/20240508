# Comparing `tmp/crawlist-0.0.8.tar.gz` & `tmp/crawlist-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crawlist-0.0.8.tar", last modified: Tue May  7 09:14:33 2024, max compression
+gzip compressed data, was "crawlist-0.0.9.tar", last modified: Wed May  8 11:10:04 2024, max compression
```

## Comparing `crawlist-0.0.8.tar` & `crawlist-0.0.9.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:14:33.604374 crawlist-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-07 09:14:29.000000 crawlist-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-07 09:14:29.000000 crawlist-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4418 2024-05-07 09:14:33.604374 crawlist-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3619 2024-05-07 09:14:29.000000 crawlist-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:14:33.600374 crawlist-0.0.8/crawlist/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-07 09:14:29.000000 crawlist-0.0.8/crawlist/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-07 09:14:29.000000 crawlist-0.0.8/crawlist/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:14:33.600374 crawlist-0.0.8/crawlist/analyzers/
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-07 09:14:29.000000 crawlist-0.0.8/crawlist/analyzers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3996 2024-05-07 09:14:29.000000 crawlist-0.0.8/crawlist/analyzers/analyzer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2942 2024-05-07 09:14:29.000000 crawlist-0.0.8/crawlist/analyzers/driver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:14:33.604374 crawlist-0.0.8/crawlist/analyzers/pager/
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-07 09:14:29.000000 crawlist-0.0.8/crawlist/analyzers/pager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11674 2024-05-07 09:14:29.000000 crawlist-0.0.8/crawlist/analyzers/pager/dynamic_pager.py
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-07 09:14:29.000000 crawlist-0.0.8/crawlist/analyzers/pager/pager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2947 2024-05-07 09:14:29.000000 crawlist-0.0.8/crawlist/analyzers/pager/static_pager.py
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-07 09:14:29.000000 crawlist-0.0.8/crawlist/analyzers/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3146 2024-05-07 09:14:29.000000 crawlist-0.0.8/crawlist/analyzers/selector.py
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-07 09:14:29.000000 crawlist-0.0.8/crawlist/analyzers/trie.py
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-05-07 09:14:29.000000 crawlist-0.0.8/crawlist/analyzers/valid.py
--rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-05-07 09:14:29.000000 crawlist-0.0.8/crawlist/annotation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:14:33.604374 crawlist-0.0.8/crawlist/processings/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-07 09:14:29.000000 crawlist-0.0.8/crawlist/processings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4186 2024-05-07 09:14:29.000000 crawlist-0.0.8/crawlist/processings/action.py
--rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-05-07 09:14:29.000000 crawlist-0.0.8/crawlist/processings/script.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:14:33.604374 crawlist-0.0.8/crawlist.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4418 2024-05-07 09:14:33.000000 crawlist-0.0.8/crawlist.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-05-07 09:14:33.000000 crawlist-0.0.8/crawlist.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 09:14:33.000000 crawlist-0.0.8/crawlist.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-07 09:14:33.000000 crawlist-0.0.8/crawlist.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-07 09:14:33.000000 crawlist-0.0.8/crawlist.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 09:14:33.604374 crawlist-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3845 2024-05-07 09:14:29.000000 crawlist-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:10:04.670817 crawlist-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-08 11:09:59.000000 crawlist-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-08 11:09:59.000000 crawlist-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4436 2024-05-08 11:10:04.670817 crawlist-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3637 2024-05-08 11:09:59.000000 crawlist-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:10:04.666817 crawlist-0.0.9/crawlist/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-08 11:09:59.000000 crawlist-0.0.9/crawlist/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-08 11:09:59.000000 crawlist-0.0.9/crawlist/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:10:04.666817 crawlist-0.0.9/crawlist/analyzers/
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-08 11:09:59.000000 crawlist-0.0.9/crawlist/analyzers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3996 2024-05-08 11:09:59.000000 crawlist-0.0.9/crawlist/analyzers/analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2942 2024-05-08 11:09:59.000000 crawlist-0.0.9/crawlist/analyzers/driver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:10:04.670817 crawlist-0.0.9/crawlist/analyzers/pager/
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-08 11:09:59.000000 crawlist-0.0.9/crawlist/analyzers/pager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12214 2024-05-08 11:09:59.000000 crawlist-0.0.9/crawlist/analyzers/pager/dynamic_pager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-08 11:09:59.000000 crawlist-0.0.9/crawlist/analyzers/pager/pager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2947 2024-05-08 11:09:59.000000 crawlist-0.0.9/crawlist/analyzers/pager/static_pager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-08 11:09:59.000000 crawlist-0.0.9/crawlist/analyzers/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3146 2024-05-08 11:09:59.000000 crawlist-0.0.9/crawlist/analyzers/selector.py
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-08 11:09:59.000000 crawlist-0.0.9/crawlist/analyzers/trie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-05-08 11:09:59.000000 crawlist-0.0.9/crawlist/analyzers/valid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-05-08 11:09:59.000000 crawlist-0.0.9/crawlist/annotation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:10:04.670817 crawlist-0.0.9/crawlist/processings/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-08 11:09:59.000000 crawlist-0.0.9/crawlist/processings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4186 2024-05-08 11:09:59.000000 crawlist-0.0.9/crawlist/processings/action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-05-08 11:09:59.000000 crawlist-0.0.9/crawlist/processings/script.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:10:04.670817 crawlist-0.0.9/crawlist.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4436 2024-05-08 11:10:04.000000 crawlist-0.0.9/crawlist.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-05-08 11:10:04.000000 crawlist-0.0.9/crawlist.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 11:10:04.000000 crawlist-0.0.9/crawlist.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-08 11:10:04.000000 crawlist-0.0.9/crawlist.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-08 11:10:04.000000 crawlist-0.0.9/crawlist.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 11:10:04.670817 crawlist-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3845 2024-05-08 11:09:59.000000 crawlist-0.0.9/setup.py
```

### Comparing `crawlist-0.0.8/LICENSE` & `crawlist-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `crawlist-0.0.8/PKG-INFO` & `crawlist-0.0.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crawlist
-Version: 0.0.8
+Version: 0.0.9
 Summary: A universal solution for web crawling lists
 Home-page: https://github.com/WwwwwyDev/crawlist
 Author: WwyDev
 Author-email: wwy20001014@foxmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -50,17 +50,22 @@
 
 
 ## introduction
 
 You can use Crawlist to crawl websites containing lists, and with some simple configurations, you can obtain all the list data.Of course, in the face of some special websites that cannot be crawled, you can also customize the configuration of that website.
 
 ## installing
-You can use pip or pip3 to install the crawlist\
+You can use pip or pip3 to install the crawlist
+
 `pip install crawlist` or `pip3 install crawlist`
 
+If you have already installed crawlist, you may need to update to the latest version
+
+`pip install --upgrade crawlist`
+
 ## quickly start
 This is a static website demo. It does not use the JavaScript to load the data.
 ```python
 import crawlist as cl
 
 if __name__ == '__main__':
     # Initialize a pager to implement page flipping 
@@ -105,12 +110,13 @@
     print(len(res))
     # After completion, you need to close the webdriver, otherwise it will occupy your memory resources
     pager.webdriver.quit()
 
 ```
 
 ## Documenting
-If you are interested and would like to see more detailed documentation, please click on the picture below.\
- <a href="https://wwydev.gitbook.io/crawlist/"><img src="https://s2.loli.net/2024/04/12/5gOBimSY4oklGys.png" alt="crawlist" style="width:287px; height:123px" ></a>
+If you are interested and would like to see more detailed documentation, please click on the link below.
+
+[English](https://wwydev.gitbook.io/crawlist "English Document")
 
 ## Contributing
 Please submit pull requests to the develop branch
```

### Comparing `crawlist-0.0.8/README.md` & `crawlist-0.0.9/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -25,17 +25,22 @@
 
 
 ## introduction
 
 You can use Crawlist to crawl websites containing lists, and with some simple configurations, you can obtain all the list data.Of course, in the face of some special websites that cannot be crawled, you can also customize the configuration of that website.
 
 ## installing
-You can use pip or pip3 to install the crawlist\
+You can use pip or pip3 to install the crawlist
+
 `pip install crawlist` or `pip3 install crawlist`
 
+If you have already installed crawlist, you may need to update to the latest version
+
+`pip install --upgrade crawlist`
+
 ## quickly start
 This is a static website demo. It does not use the JavaScript to load the data.
 ```python
 import crawlist as cl
 
 if __name__ == '__main__':
     # Initialize a pager to implement page flipping 
@@ -80,12 +85,13 @@
     print(len(res))
     # After completion, you need to close the webdriver, otherwise it will occupy your memory resources
     pager.webdriver.quit()
 
 ```
 
 ## Documenting
-If you are interested and would like to see more detailed documentation, please click on the picture below.\
- <a href="https://wwydev.gitbook.io/crawlist/"><img src="https://s2.loli.net/2024/04/12/5gOBimSY4oklGys.png" alt="crawlist" style="width:287px; height:123px" ></a>
+If you are interested and would like to see more detailed documentation, please click on the link below.
+
+[English](https://wwydev.gitbook.io/crawlist "English Document")
 
 ## Contributing
 Please submit pull requests to the develop branch
```

### Comparing `crawlist-0.0.8/crawlist/analyzers/analyzer.py` & `crawlist-0.0.9/crawlist/analyzers/analyzer.py`

 * *Files identical despite different names*

### Comparing `crawlist-0.0.8/crawlist/analyzers/driver.py` & `crawlist-0.0.9/crawlist/analyzers/driver.py`

 * *Files identical despite different names*

### Comparing `crawlist-0.0.8/crawlist/analyzers/pager/dynamic_pager.py` & `crawlist-0.0.9/crawlist/analyzers/pager/dynamic_pager.py`

 * *Files 3% similar despite different names*

```diff
@@ -119,22 +119,23 @@
         uri = self.uris[self.index]
         self.webdriver.get(uri)
         return self.webdriver.page_source
 
 
 class DynamicScrollPager(DynamicPager):
     @check
-    def __init__(self, uri: str, webdriver: Driver | WebDriver = None, interval: float = 1) -> None:
+    def __init__(self, uri: str = "", webdriver: Driver | WebDriver = None, interval: float = 1) -> None:
         """
         Based on dynamic web page analyzer (scrolling and flipping)
         :param uri: webpage link, which is a scrolling page
         :param webdriver: WebDriver object for selenium
         :param interval: Grab the list frequency and adjust it according to the actual situation of the webpage
         """
-        assert Valid.is_valid_url(uri)
+        if uri:
+            assert Valid.is_valid_url(uri)
         self.uri = uri
         super().__init__(webdriver=webdriver, interval=interval)
         self.pre_load(self.webdriver)
         self.sleep()
 
     js_code = '''he = setInterval(() => {
                         document.documentElement.scrollTop += document.documentElement.scrollHeight
@@ -156,76 +157,84 @@
         self.sleep()
 
     @property
     def html(self) -> str:
         return self.webdriver.page_source
 
     def pre_load(self, webdriver: WebDriver) -> None:
-        webdriver.get(self.uri)
+        if self.uri:
+            webdriver.get(self.uri)
 
 
 class DynamicLineButtonPager(DynamicPager):
     @check
-    def __init__(self, uri: str, button_selector: WebElementSelector, webdriver: Driver | WebDriver = None,
+    def __init__(self, button_selector: WebElementSelector, uri: str = "", webdriver: Driver | WebDriver = None,
                  interval: float = 1) -> None:
         """
         Based on dynamic web page analyzer (row button page flipping)
-        :param uri: webpage link, which is a row button for flipping pages
         :param button.selector: row button selector
+        :param uri: webpage link, which is a row button for flipping pages
         :param webdriver: WebDriver object for selenium
         :param interval: Grab the list frequency and adjust it according to the actual situation of the webpage
         """
-        assert Valid.is_valid_url(uri)
+        if uri:
+            assert Valid.is_valid_url(uri)
         self.uri = uri
         super().__init__(webdriver=webdriver, interval=interval)
         self.pre_load(self.webdriver)
         self.sleep()
-        assert len(button_selector(self.webdriver, interval=interval)) > 0
+        if uri:
+            assert len(button_selector(self.webdriver, interval=interval)) > 0
         self.button = button_selector
 
     def next(self) -> None:
         button_element = self.button(self.webdriver, interval=self.interval)[0]
         self.click_safety(button_element)
         self.sleep()
 
     @property
     def html(self) -> str:
         return self.webdriver.page_source
 
     def pre_load(self, webdriver: WebDriver) -> None:
-        webdriver.get(self.uri)
+        if self.uri:
+            webdriver.get(self.uri)
 
 
 class DynamicNumButtonPager(DynamicPager):
     @check
-    def __init__(self, uri: str, button_selector: WebElementSelector, webdriver: Driver | WebDriver = None, start: int = 1,
+    def __init__(self, button_selector: WebElementSelector, uri: str = "", webdriver: Driver | WebDriver = None,
+                 start: int = 1,
                  offset: int = 1, interval: float = 1) -> None:
         """
         Based on dynamic web page analyzer (digital button flipping)
-        :param uri: webpage link, which is a numeric button for flipping pages
         :param button.selector: numeric button selector
+        :param uri: webpage link, which is a numeric button for flipping pages
         :param webdriver: WebDriver object for selenium
         :param start: Start page
         :param offset: pagination interval
         :param interval: Grab the list frequency and adjust it according to the actual situation of the webpage
         """
-        assert Valid.is_valid_url(uri)
+        if uri:
+            assert Valid.is_valid_url(uri)
         self.uri = uri
         super().__init__(webdriver=webdriver, interval=interval)
         self.pre_load(self.webdriver)
         self.sleep()
-        assert len(button_selector(self.webdriver, interval=interval)) > 0
+        if uri:
+            assert len(button_selector(self.webdriver, interval=interval)) > 0
         self.index = 1
         self.offset = offset
         self.button = button_selector
-        while start - 1:
-            start -= 1
-            self.next_one()
+        self.start = start
 
     def next(self) -> None:
+        while self.start - 1:
+            self.start -= 1
+            self.next_one()
         offset = self.offset
         while offset:
             self.next_one()
             offset -= 1
         self.sleep()
 
     def next_one(self) -> None:
@@ -234,14 +243,17 @@
         button = DynamicNumButtonPager.find_num_button(num_button_elements, num=self.index)
         if button:
             self.click_safety(button)
         self.sleep()
 
     @property
     def html(self) -> str:
+        while self.start - 1:
+            self.start -= 1
+            self.next_one()
         return self.webdriver.page_source
 
     @staticmethod
     def check_num_button(element: WebElement, num: int = 1) -> bool:
         """
         Find if there are numbers in the inner_text of an element
         :param element: selenium WebElement
@@ -267,54 +279,63 @@
         """
         for element in elements:
             if DynamicNumButtonPager.check_num_button(element, num):
                 return element
         return None
 
     def pre_load(self, webdriver: WebDriver) -> None:
-        webdriver.get(self.uri)
+        if self.uri:
+            webdriver.get(self.uri)
 
 
 class DynamicNextButtonPager(DynamicPager):
     @check
-    def __init__(self, uri: str, button_selector: WebElementSelector, webdriver: Driver | WebDriver = None, start: int = 1,
+    def __init__(self, button_selector: WebElementSelector, uri: str = "", webdriver: Driver | WebDriver = None,
+                 start: int = 1,
                  offset: int = 1, interval: float = 1) -> None:
         """
         Based on dynamic web page analyzer (click the next page button to page)
-        :param uri: Web page link, which is a page that can be flipped by clicking the next page button
         :param button.selector: Click on the next page button selector
+        :param uri: Web page link, which is a page that can be flipped by clicking the next page button
         :param webdriver: WebDriver object for selenium
         :param start: Start page
         :param offset: pagination interval
         :param interval: Grab the list frequency and adjust it according to the actual situation of the webpage
         """
-        assert Valid.is_valid_url(uri)
+        if uri:
+            assert Valid.is_valid_url(uri)
         self.uri = uri
         super().__init__(webdriver=webdriver, interval=interval)
         self.pre_load(self.webdriver)
         self.sleep()
-        assert len(button_selector(self.webdriver, interval=interval)) > 0
+        if uri:
+            assert len(button_selector(self.webdriver, interval=interval)) > 0
         self.offset = offset
         self.button = button_selector
-        while start - 1:
-            start -= 1
-            self.next_one()
+        self.start = start
 
     def next(self) -> None:
+        while self.start - 1:
+            self.start -= 1
+            self.next_one()
         offset = self.offset
         while offset:
             self.next_one()
             offset -= 1
         self.sleep()
 
     def next_one(self) -> None:
         button = self.button(self.webdriver, interval=self.interval)[0]
         if button:
             self.click_safety(button)
         self.sleep()
 
     @property
     def html(self) -> str:
+        while self.start - 1:
+            self.start -= 1
+            self.next_one()
         return self.webdriver.page_source
 
     def pre_load(self, webdriver: WebDriver) -> None:
-        webdriver.get(self.uri)
+        if self.uri:
+            webdriver.get(self.uri)
```

### Comparing `crawlist-0.0.8/crawlist/analyzers/pager/pager.py` & `crawlist-0.0.9/crawlist/analyzers/pager/pager.py`

 * *Files identical despite different names*

### Comparing `crawlist-0.0.8/crawlist/analyzers/pager/static_pager.py` & `crawlist-0.0.9/crawlist/analyzers/pager/static_pager.py`

 * *Files identical despite different names*

### Comparing `crawlist-0.0.8/crawlist/analyzers/request.py` & `crawlist-0.0.9/crawlist/analyzers/request.py`

 * *Files identical despite different names*

### Comparing `crawlist-0.0.8/crawlist/analyzers/selector.py` & `crawlist-0.0.9/crawlist/analyzers/selector.py`

 * *Files identical despite different names*

### Comparing `crawlist-0.0.8/crawlist/analyzers/trie.py` & `crawlist-0.0.9/crawlist/analyzers/trie.py`

 * *Files identical despite different names*

### Comparing `crawlist-0.0.8/crawlist/analyzers/valid.py` & `crawlist-0.0.9/crawlist/analyzers/valid.py`

 * *Files identical despite different names*

### Comparing `crawlist-0.0.8/crawlist/annotation.py` & `crawlist-0.0.9/crawlist/annotation.py`

 * *Files identical despite different names*

### Comparing `crawlist-0.0.8/crawlist/processings/action.py` & `crawlist-0.0.9/crawlist/processings/action.py`

 * *Files identical despite different names*

### Comparing `crawlist-0.0.8/crawlist/processings/script.py` & `crawlist-0.0.9/crawlist/processings/script.py`

 * *Files identical despite different names*

### Comparing `crawlist-0.0.8/crawlist.egg-info/PKG-INFO` & `crawlist-0.0.9/crawlist.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crawlist
-Version: 0.0.8
+Version: 0.0.9
 Summary: A universal solution for web crawling lists
 Home-page: https://github.com/WwwwwyDev/crawlist
 Author: WwyDev
 Author-email: wwy20001014@foxmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -50,17 +50,22 @@
 
 
 ## introduction
 
 You can use Crawlist to crawl websites containing lists, and with some simple configurations, you can obtain all the list data.Of course, in the face of some special websites that cannot be crawled, you can also customize the configuration of that website.
 
 ## installing
-You can use pip or pip3 to install the crawlist\
+You can use pip or pip3 to install the crawlist
+
 `pip install crawlist` or `pip3 install crawlist`
 
+If you have already installed crawlist, you may need to update to the latest version
+
+`pip install --upgrade crawlist`
+
 ## quickly start
 This is a static website demo. It does not use the JavaScript to load the data.
 ```python
 import crawlist as cl
 
 if __name__ == '__main__':
     # Initialize a pager to implement page flipping 
@@ -105,12 +110,13 @@
     print(len(res))
     # After completion, you need to close the webdriver, otherwise it will occupy your memory resources
     pager.webdriver.quit()
 
 ```
 
 ## Documenting
-If you are interested and would like to see more detailed documentation, please click on the picture below.\
- <a href="https://wwydev.gitbook.io/crawlist/"><img src="https://s2.loli.net/2024/04/12/5gOBimSY4oklGys.png" alt="crawlist" style="width:287px; height:123px" ></a>
+If you are interested and would like to see more detailed documentation, please click on the link below.
+
+[English](https://wwydev.gitbook.io/crawlist "English Document")
 
 ## Contributing
 Please submit pull requests to the develop branch
```

### Comparing `crawlist-0.0.8/crawlist.egg-info/SOURCES.txt` & `crawlist-0.0.9/crawlist.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crawlist-0.0.8/setup.py` & `crawlist-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'crawlist'
 DESCRIPTION = 'A universal solution for web crawling lists'
 URL = 'https://github.com/WwwwwyDev/crawlist'
 EMAIL = 'wwy20001014@foxmail.com'
 AUTHOR = 'WwyDev'
 REQUIRES_PYTHON = '>=3.10.0'
-VERSION = '0.0.8'
+VERSION = '0.0.9'
 # What packages are required for this module to be executed?
 REQUIRED = [
     'parsel', 'selenium>=4.0.0', 'cssselect', 'lxml', 'requests', 'webdriver-manager'
 ]
 
 # What packages are optional?
 EXTRAS = {
```

