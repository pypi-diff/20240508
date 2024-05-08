# Comparing `tmp/movoid_robotframework_selenium-1.2.3.tar.gz` & `tmp/movoid_robotframework_selenium-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "movoid_robotframework_selenium-1.2.3.tar", last modified: Tue May  7 13:35:21 2024, max compression
+gzip compressed data, was "movoid_robotframework_selenium-1.2.4.tar", last modified: Wed May  8 15:01:02 2024, max compression
```

## Comparing `movoid_robotframework_selenium-1.2.3.tar` & `movoid_robotframework_selenium-1.2.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 13:35:21.819282 movoid_robotframework_selenium-1.2.3/
--rw-rw-rw-   0        0        0       10 2024-04-24 13:42:41.000000 movoid_robotframework_selenium-1.2.3/MANIFEST.in
--rw-rw-rw-   0        0        0      439 2024-05-07 13:35:21.818273 movoid_robotframework_selenium-1.2.3/PKG-INFO
--rw-rw-rw-   0        0        0       44 2024-01-07 14:19:32.000000 movoid_robotframework_selenium-1.2.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-07 13:35:21.796605 movoid_robotframework_selenium-1.2.3/RobotFrameworkSelenium/
--rw-rw-rw-   0        0        0      311 2024-02-20 17:47:42.000000 movoid_robotframework_selenium-1.2.3/RobotFrameworkSelenium/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-07 13:35:21.799664 movoid_robotframework_selenium-1.2.3/RobotFrameworkSelenium/action/
--rw-rw-rw-   0        0        0      218 2024-02-20 05:59:20.000000 movoid_robotframework_selenium-1.2.3/RobotFrameworkSelenium/action/__init__.py
--rw-rw-rw-   0        0        0    12876 2024-04-20 10:51:34.000000 movoid_robotframework_selenium-1.2.3/RobotFrameworkSelenium/action/action.py
--rw-rw-rw-   0        0        0     6393 2024-04-20 15:50:56.000000 movoid_robotframework_selenium-1.2.3/RobotFrameworkSelenium/action/action.pyi
--rw-rw-rw-   0        0        0     9778 2024-05-07 13:18:52.000000 movoid_robotframework_selenium-1.2.3/RobotFrameworkSelenium/common.py
--rw-rw-rw-   0        0        0     2596 2024-05-06 09:57:55.000000 movoid_robotframework_selenium-1.2.3/RobotFrameworkSelenium/common.pyi
--rw-rw-rw-   0        0        0      268 2024-02-20 05:59:20.000000 movoid_robotframework_selenium-1.2.3/RobotFrameworkSelenium/main.py
-drwxrwxrwx   0        0        0        0 2024-05-07 13:35:21.817267 movoid_robotframework_selenium-1.2.3/movoid_robotframework_selenium.egg-info/
--rw-rw-rw-   0        0        0      439 2024-05-07 13:35:21.000000 movoid_robotframework_selenium-1.2.3/movoid_robotframework_selenium.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      555 2024-05-07 13:35:21.000000 movoid_robotframework_selenium-1.2.3/movoid_robotframework_selenium.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 13:35:21.000000 movoid_robotframework_selenium-1.2.3/movoid_robotframework_selenium.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      115 2024-05-07 13:35:21.000000 movoid_robotframework_selenium-1.2.3/movoid_robotframework_selenium.egg-info/requires.txt
--rw-rw-rw-   0        0        0       28 2024-05-07 13:35:21.000000 movoid_robotframework_selenium-1.2.3/movoid_robotframework_selenium.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-07 13:35:21.819282 movoid_robotframework_selenium-1.2.3/setup.cfg
--rw-rw-rw-   0        0        0      748 2024-05-07 13:33:07.000000 movoid_robotframework_selenium-1.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 15:01:02.950703 movoid_robotframework_selenium-1.2.4/
+-rw-rw-rw-   0        0        0       10 2024-04-24 13:42:41.000000 movoid_robotframework_selenium-1.2.4/MANIFEST.in
+-rw-rw-rw-   0        0        0      439 2024-05-08 15:01:02.949683 movoid_robotframework_selenium-1.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0       44 2024-01-07 14:19:32.000000 movoid_robotframework_selenium-1.2.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-08 15:01:02.928758 movoid_robotframework_selenium-1.2.4/RobotFrameworkSelenium/
+-rw-rw-rw-   0        0        0      311 2024-02-20 17:47:42.000000 movoid_robotframework_selenium-1.2.4/RobotFrameworkSelenium/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 15:01:02.932885 movoid_robotframework_selenium-1.2.4/RobotFrameworkSelenium/action/
+-rw-rw-rw-   0        0        0      218 2024-02-20 05:59:20.000000 movoid_robotframework_selenium-1.2.4/RobotFrameworkSelenium/action/__init__.py
+-rw-rw-rw-   0        0        0    12876 2024-04-20 10:51:34.000000 movoid_robotframework_selenium-1.2.4/RobotFrameworkSelenium/action/action.py
+-rw-rw-rw-   0        0        0     6393 2024-05-08 14:59:24.000000 movoid_robotframework_selenium-1.2.4/RobotFrameworkSelenium/action/action.pyi
+-rw-rw-rw-   0        0        0     9778 2024-05-07 13:18:52.000000 movoid_robotframework_selenium-1.2.4/RobotFrameworkSelenium/common.py
+-rw-rw-rw-   0        0        0     2717 2024-05-08 14:59:18.000000 movoid_robotframework_selenium-1.2.4/RobotFrameworkSelenium/common.pyi
+-rw-rw-rw-   0        0        0      268 2024-02-20 05:59:20.000000 movoid_robotframework_selenium-1.2.4/RobotFrameworkSelenium/main.py
+drwxrwxrwx   0        0        0        0 2024-05-08 15:01:02.941174 movoid_robotframework_selenium-1.2.4/movoid_robotframework_selenium.egg-info/
+-rw-rw-rw-   0        0        0      439 2024-05-08 15:01:02.000000 movoid_robotframework_selenium-1.2.4/movoid_robotframework_selenium.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      555 2024-05-08 15:01:02.000000 movoid_robotframework_selenium-1.2.4/movoid_robotframework_selenium.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 15:01:02.000000 movoid_robotframework_selenium-1.2.4/movoid_robotframework_selenium.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      115 2024-05-08 15:01:02.000000 movoid_robotframework_selenium-1.2.4/movoid_robotframework_selenium.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       28 2024-05-08 15:01:02.000000 movoid_robotframework_selenium-1.2.4/movoid_robotframework_selenium.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-08 15:01:02.951715 movoid_robotframework_selenium-1.2.4/setup.cfg
+-rw-rw-rw-   0        0        0      748 2024-05-08 15:00:49.000000 movoid_robotframework_selenium-1.2.4/setup.py
```

### Comparing `movoid_robotframework_selenium-1.2.3/RobotFrameworkSelenium/action/action.py` & `movoid_robotframework_selenium-1.2.4/RobotFrameworkSelenium/action/action.py`

 * *Files identical despite different names*

### Comparing `movoid_robotframework_selenium-1.2.3/RobotFrameworkSelenium/action/action.pyi` & `movoid_robotframework_selenium-1.2.4/RobotFrameworkSelenium/action/action.pyi`

 * *Files identical despite different names*

### Comparing `movoid_robotframework_selenium-1.2.3/RobotFrameworkSelenium/common.py` & `movoid_robotframework_selenium-1.2.4/RobotFrameworkSelenium/common.py`

 * *Files identical despite different names*

### Comparing `movoid_robotframework_selenium-1.2.3/RobotFrameworkSelenium/common.pyi` & `movoid_robotframework_selenium-1.2.4/RobotFrameworkSelenium/common.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 ##################################################
 # This is auto generated by code.
 ##################################################
 
+import base64
 import math
 import os
 import cv2
+import np
 import robot
 import selenium
 import RobotFrameworkBasic.main
 import robot.libraries.BuiltIn
 import selenium.webdriver.chrome.webdriver
 import typing
 import selenium.webdriver.remote.webelement
@@ -23,23 +25,24 @@
 		self.driver: selenium.webdriver.chrome.webdriver.WebDriver =  getattr(self, 'driver', None)
 		self.action_chains: ActionChains =  getattr(self, 'action_chains', None)
 		self.screenshot_root: str =  getattr(self, 'screenshot_root', None)
 		self.outer_coordinate: typing.Tuple[float] =  getattr(self, 'outer_coordinate', None)
 		self.inner_coordinate: typing.Tuple[float] =  getattr(self, 'inner_coordinate', None)
 		self.window_x: float =  getattr(self, 'window_x', None)
 		self.window_y: float =  getattr(self, 'window_y', None)
-	def selenium_init(self):	...
+	def selenium_init(self, screenshot_log: bool = False):	...
 	def selenium_analyse_locator(self, locator: str) -> typing.Tuple[str, str]:	...
 	def selenium_find_elements_by_locator(self, locator) -> typing.List[selenium.webdriver.remote.webelement.WebElement]:	...
 	def selenium_find_element_by_locator(self, locator) -> selenium.webdriver.remote.webelement.WebElement:	...
 	def selenium_execute_js_script(self, js_code: str, args):	...
 	def analyse_color_function(self, color_function):	...
 	def exchange_list3_to_color_function(self, formula_list):	...
 	def selenium_get_full_screenshot_path(self, screenshot_name):	...
 	def selenium_cut_screenshot(self, screenshot_locator, image_name = 'element-cut-image.png'):	...
 	def selenium_take_screenshot(self, screenshot_locator = None, image_name = 'python-screenshot.png', rename = True):	...
-	def selenium_log_screenshot(self, screenshot_locator=None):	...
+	def selenium_log_screenshot(self, screenshot_locator = None):	...
+	def selenium_log_screenshot_path(self, screenshot_name):	...
 	def selenium_analyse_image(self, image):	...
 	def selenium_analyse_element(self, locator: typing.Union[selenium.webdriver.remote.webelement.WebElement, str]) -> selenium.webdriver.remote.webelement.WebElement:	...
 	def selenium_analyse_elements(self, locator: typing.Union[typing.List[selenium.webdriver.remote.webelement.WebElement], str]) -> typing.List[selenium.webdriver.remote.webelement.WebElement]:	...
 	...
```

### Comparing `movoid_robotframework_selenium-1.2.3/movoid_robotframework_selenium.egg-info/SOURCES.txt` & `movoid_robotframework_selenium-1.2.4/movoid_robotframework_selenium.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `movoid_robotframework_selenium-1.2.3/setup.py` & `movoid_robotframework_selenium-1.2.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='movoid_robotframework_selenium',
-    version='1.2.3',
+    version='1.2.4',
     packages=find_packages(),
     url='',
     license='',
     author='movoid',
     author_email='bobrobotsun@163.com',
     description='',
     long_description=long_description,
```

