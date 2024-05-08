# Comparing `tmp/crawlipt-0.0.6.tar.gz` & `tmp/crawlipt-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crawlipt-0.0.6.tar", last modified: Tue May  7 11:02:28 2024, max compression
+gzip compressed data, was "crawlipt-0.0.7.tar", last modified: Wed May  8 11:28:42 2024, max compression
```

## Comparing `crawlipt-0.0.6.tar` & `crawlipt-0.0.7.tar`

### file list

```diff
@@ -1,41 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:02:28.764406 crawlipt-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-07 11:02:24.000000 crawlipt-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-07 11:02:24.000000 crawlipt-0.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3221 2024-05-07 11:02:28.764406 crawlipt-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-05-07 11:02:24.000000 crawlipt-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:02:28.760406 crawlipt-0.0.6/crawlipt/
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-07 11:02:24.000000 crawlipt-0.0.6/crawlipt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-07 11:02:24.000000 crawlipt-0.0.6/crawlipt/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-07 11:02:24.000000 crawlipt-0.0.6/crawlipt/action.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:02:28.764406 crawlipt-0.0.6/crawlipt/actions/
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-07 11:02:24.000000 crawlipt-0.0.6/crawlipt/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-05-07 11:02:24.000000 crawlipt-0.0.6/crawlipt/actions/click.py
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-05-07 11:02:24.000000 crawlipt-0.0.6/crawlipt/actions/get.py
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-07 11:02:24.000000 crawlipt-0.0.6/crawlipt/actions/input.py
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-07 11:02:24.000000 crawlipt-0.0.6/crawlipt/actions/redirect.py
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-07 11:02:24.000000 crawlipt-0.0.6/crawlipt/actions/scroll.py
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-07 11:02:24.000000 crawlipt-0.0.6/crawlipt/actions/select.py
--rw-r--r--   0 runner    (1001) docker     (127)      990 2024-05-07 11:02:24.000000 crawlipt-0.0.6/crawlipt/actions/slide.py
--rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-05-07 11:02:24.000000 crawlipt-0.0.6/crawlipt/actions/switch.py
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-07 11:02:24.000000 crawlipt-0.0.6/crawlipt/actions/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-05-07 11:02:24.000000 crawlipt-0.0.6/crawlipt/actions/window.py
--rw-r--r--   0 runner    (1001) docker     (127)     3388 2024-05-07 11:02:24.000000 crawlipt-0.0.6/crawlipt/annotation.py
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-07 11:02:24.000000 crawlipt-0.0.6/crawlipt/condition.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:02:28.764406 crawlipt-0.0.6/crawlipt/conditions/
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-07 11:02:24.000000 crawlipt-0.0.6/crawlipt/conditions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-05-07 11:02:24.000000 crawlipt-0.0.6/crawlipt/conditions/element.py
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-07 11:02:24.000000 crawlipt-0.0.6/crawlipt/conditions/frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-05-07 11:02:24.000000 crawlipt-0.0.6/crawlipt/conditions/presence.py
--rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-05-07 11:02:24.000000 crawlipt-0.0.6/crawlipt/conditions/text.py
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-05-07 11:02:24.000000 crawlipt-0.0.6/crawlipt/conditions/visibility.py
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-07 11:02:24.000000 crawlipt-0.0.6/crawlipt/error.py
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-07 11:02:24.000000 crawlipt-0.0.6/crawlipt/pojo.py
--rw-r--r--   0 runner    (1001) docker     (127)    20140 2024-05-07 11:02:24.000000 crawlipt-0.0.6/crawlipt/script.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:02:28.764406 crawlipt-0.0.6/crawlipt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3221 2024-05-07 11:02:28.000000 crawlipt-0.0.6/crawlipt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-07 11:02:28.000000 crawlipt-0.0.6/crawlipt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 11:02:28.000000 crawlipt-0.0.6/crawlipt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-07 11:02:28.000000 crawlipt-0.0.6/crawlipt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-07 11:02:28.000000 crawlipt-0.0.6/crawlipt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 11:02:28.764406 crawlipt-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3783 2024-05-07 11:02:24.000000 crawlipt-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:28:42.978835 crawlipt-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-08 11:28:35.000000 crawlipt-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-08 11:28:35.000000 crawlipt-0.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3220 2024-05-08 11:28:42.978835 crawlipt-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-05-08 11:28:35.000000 crawlipt-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:28:42.974835 crawlipt-0.0.7/crawlipt/
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-08 11:28:35.000000 crawlipt-0.0.7/crawlipt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-08 11:28:35.000000 crawlipt-0.0.7/crawlipt/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-08 11:28:35.000000 crawlipt-0.0.7/crawlipt/action.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:28:42.974835 crawlipt-0.0.7/crawlipt/actions/
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-08 11:28:35.000000 crawlipt-0.0.7/crawlipt/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-08 11:28:35.000000 crawlipt-0.0.7/crawlipt/actions/alert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-05-08 11:28:35.000000 crawlipt-0.0.7/crawlipt/actions/click.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-05-08 11:28:35.000000 crawlipt-0.0.7/crawlipt/actions/get.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-08 11:28:35.000000 crawlipt-0.0.7/crawlipt/actions/input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-08 11:28:35.000000 crawlipt-0.0.7/crawlipt/actions/redirect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-08 11:28:35.000000 crawlipt-0.0.7/crawlipt/actions/scroll.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-05-08 11:28:35.000000 crawlipt-0.0.7/crawlipt/actions/select.py
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-05-08 11:28:35.000000 crawlipt-0.0.7/crawlipt/actions/slide.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-05-08 11:28:35.000000 crawlipt-0.0.7/crawlipt/actions/switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-08 11:28:35.000000 crawlipt-0.0.7/crawlipt/actions/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-05-08 11:28:35.000000 crawlipt-0.0.7/crawlipt/actions/window.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3388 2024-05-08 11:28:35.000000 crawlipt-0.0.7/crawlipt/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-08 11:28:35.000000 crawlipt-0.0.7/crawlipt/condition.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:28:42.978835 crawlipt-0.0.7/crawlipt/conditions/
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-08 11:28:35.000000 crawlipt-0.0.7/crawlipt/conditions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-05-08 11:28:35.000000 crawlipt-0.0.7/crawlipt/conditions/element.py
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-08 11:28:35.000000 crawlipt-0.0.7/crawlipt/conditions/frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-05-08 11:28:35.000000 crawlipt-0.0.7/crawlipt/conditions/presence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-05-08 11:28:35.000000 crawlipt-0.0.7/crawlipt/conditions/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-05-08 11:28:35.000000 crawlipt-0.0.7/crawlipt/conditions/visibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-08 11:28:35.000000 crawlipt-0.0.7/crawlipt/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-08 11:28:35.000000 crawlipt-0.0.7/crawlipt/pojo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20140 2024-05-08 11:28:35.000000 crawlipt-0.0.7/crawlipt/script.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:28:42.978835 crawlipt-0.0.7/crawlipt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3220 2024-05-08 11:28:42.000000 crawlipt-0.0.7/crawlipt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-05-08 11:28:42.000000 crawlipt-0.0.7/crawlipt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 11:28:42.000000 crawlipt-0.0.7/crawlipt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-08 11:28:42.000000 crawlipt-0.0.7/crawlipt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-08 11:28:42.000000 crawlipt-0.0.7/crawlipt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 11:28:42.978835 crawlipt-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3783 2024-05-08 11:28:35.000000 crawlipt-0.0.7/setup.py
```

### Comparing `crawlipt-0.0.6/LICENSE` & `crawlipt-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `crawlipt-0.0.6/PKG-INFO` & `crawlipt-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crawlipt
-Version: 0.0.6
+Version: 0.0.7
 Summary: The script for selenium in python
 Home-page: https://github.com/WwwwwyDev/crawlipt
 Author: WwwwwyDev
 Author-email: wwy20001014@foxmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -49,15 +49,15 @@
 You can use Crawlipt to driver the selenium by script in python.The script adopts JSON format for better cross language operations and physical storage.
 
 ## installing
 You can use pip or pip3 to install the crawlipt
 
 `pip install crawlipt` or `pip3 install crawlipt`
 
-If you have already installed crawlelip, you may need to update to the latest version
+If you have already installed crawlipt, you may need to update to the latest version
 
 `pip install --upgrade crawlipt`
 
 ## quickly start
 ```python
 from webdriver_manager.chrome import ChromeDriverManager
 from selenium import webdriver as wd
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: crawlipt Version: 0.0.6 Summary: The script for
+Metadata-Version: 2.1 Name: crawlipt Version: 0.0.7 Summary: The script for
 selenium in python Home-page: https://github.com/WwwwwyDev/crawlipt Author:
 WwwwwyDev Author-email: wwy20001014@foxmail.com License: MIT Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
 Python Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python ::
 Implementation :: CPython Classifier: Programming Language :: Python ::
 Implementation :: PyPy Requires-Python: >=3.10.0 Description-Content-Type:
@@ -10,15 +10,15 @@
                                   _[_c_r_a_w_l_i_s_t_]
                  # crawlipt The script for selenium in python
                          _[_p_y_p_i_][python]_[_G_i_t_H_u_b_ _s_t_a_r_s_]
 ## introduction You can use Crawlipt to driver the selenium by script in
 python.The script adopts JSON format for better cross language operations and
 physical storage. ## installing You can use pip or pip3 to install the crawlipt
 `pip install crawlipt` or `pip3 install crawlipt` If you have already installed
-crawlelip, you may need to update to the latest version `pip install --upgrade
+crawlipt, you may need to update to the latest version `pip install --upgrade
 crawlipt` ## quickly start ```python from webdriver_manager.chrome import
 ChromeDriverManager from selenium import webdriver as wd from
 selenium.webdriver.chrome.service import Service import crawlipt as cpt option
 = wd.ChromeOptions() option.add_argument("start-maximized") option.add_argument
 ("window-size=1920x3000") agent = 'user-agent="Mozilla/5.0 (Macintosh; Intel
 Mac OS X 10_14_1) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/70.0.3538.77
 Safari/537.36"' option.add_argument(agent) webdriver = wd.Chrome
```

### Comparing `crawlipt-0.0.6/README.md` & `crawlipt-0.0.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 You can use Crawlipt to driver the selenium by script in python.The script adopts JSON format for better cross language operations and physical storage.
 
 ## installing
 You can use pip or pip3 to install the crawlipt
 
 `pip install crawlipt` or `pip3 install crawlipt`
 
-If you have already installed crawlelip, you may need to update to the latest version
+If you have already installed crawlipt, you may need to update to the latest version
 
 `pip install --upgrade crawlipt`
 
 ## quickly start
 ```python
 from webdriver_manager.chrome import ChromeDriverManager
 from selenium import webdriver as wd
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
                                   _[_c_r_a_w_l_i_s_t_]
                  # crawlipt The script for selenium in python
                          _[_p_y_p_i_][python]_[_G_i_t_H_u_b_ _s_t_a_r_s_]
 ## introduction You can use Crawlipt to driver the selenium by script in
 python.The script adopts JSON format for better cross language operations and
 physical storage. ## installing You can use pip or pip3 to install the crawlipt
 `pip install crawlipt` or `pip3 install crawlipt` If you have already installed
-crawlelip, you may need to update to the latest version `pip install --upgrade
+crawlipt, you may need to update to the latest version `pip install --upgrade
 crawlipt` ## quickly start ```python from webdriver_manager.chrome import
 ChromeDriverManager from selenium import webdriver as wd from
 selenium.webdriver.chrome.service import Service import crawlipt as cpt option
 = wd.ChromeOptions() option.add_argument("start-maximized") option.add_argument
 ("window-size=1920x3000") agent = 'user-agent="Mozilla/5.0 (Macintosh; Intel
 Mac OS X 10_14_1) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/70.0.3538.77
 Safari/537.36"' option.add_argument(agent) webdriver = wd.Chrome
```

### Comparing `crawlipt-0.0.6/crawlipt/actions/click.py` & `crawlipt-0.0.7/crawlipt/actions/click.py`

 * *Files identical despite different names*

### Comparing `crawlipt-0.0.6/crawlipt/actions/get.py` & `crawlipt-0.0.7/crawlipt/actions/get.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,45 +6,47 @@
 
 class Get:
 
     @staticmethod
     @check(exclude="driver")
     def getInnerText(driver: WebDriver, xpath: str) -> str:
         """
-        Handling keyboard input events
+        get inner text of element
         :param driver: selenium webdriver
         :param xpath: The xpath path of the element
         """
         element = driver.find_element(By.XPATH, xpath)
         res = element.get_attribute('innerText')
         if res is None:
             res = ""
         return res
 
     @staticmethod
     @check(exclude="driver")
     def getTextContent(driver: WebDriver, xpath: str) -> str:
         """
-        Handling keyboard input events
+        get text content of element
         :param driver: selenium webdriver
         :param xpath: The xpath path of the element
         """
         element = driver.find_element(By.XPATH, xpath)
         res = element.get_attribute('textContent')
         if res is None:
             res = ""
         return res
 
     @staticmethod
     @check(exclude="driver")
     def getAttribute(driver: WebDriver, xpath: str, name: str) -> str:
         """
-        Handling keyboard input events
+        get the attribute of an element
         :param driver: selenium webdriver
         :param xpath: The xpath path of the element
         :param name: The name of the attribute
         """
         element = driver.find_element(By.XPATH, xpath)
         res = element.get_attribute(name)
         if res is None:
             res = ""
         return res
+
+
```

### Comparing `crawlipt-0.0.6/crawlipt/actions/input.py` & `crawlipt-0.0.7/crawlipt/actions/input.py`

 * *Files identical despite different names*

### Comparing `crawlipt-0.0.6/crawlipt/actions/redirect.py` & `crawlipt-0.0.7/crawlipt/actions/redirect.py`

 * *Files identical despite different names*

### Comparing `crawlipt-0.0.6/crawlipt/actions/scroll.py` & `crawlipt-0.0.7/crawlipt/actions/scroll.py`

 * *Files identical despite different names*

### Comparing `crawlipt-0.0.6/crawlipt/actions/select.py` & `crawlipt-0.0.7/crawlipt/actions/select.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,38 +5,38 @@
 
 
 class Select:
     @staticmethod
     @check(exclude="driver")
     def selectByText(driver: WebDriver, xpath: str, text: str) -> None:
         """
-        Handling click events
+        Handling select events
         :param driver: selenium webdriver
         :param xpath: the xpath path of the select element
         :param text: the text of selecting
         """
         select = WebSelect(driver.find_element(By.XPATH, xpath))
         select.select_by_visible_text(text)
 
     @staticmethod
     @check(exclude="driver")
     def selectByValue(driver: WebDriver, xpath: str, value: str) -> None:
         """
-        Handling click events
+        Handling select events
         :param driver: selenium webdriver
         :param xpath: the xpath path of the select element
         :param value: the value of selecting
         """
         select = WebSelect(driver.find_element(By.XPATH, xpath))
         select.select_by_value(value)
 
     @staticmethod
     @check(exclude="driver")
     def selectByIndex(driver: WebDriver, xpath: str, index: int) -> None:
         """
-        Handling click events
+        Handling select events
         :param driver: selenium webdriver
         :param xpath: the xpath path of the select element
         :param index: the index of selecting
         """
         select = WebSelect(driver.find_element(By.XPATH, xpath))
         select.select_by_index(index)
```

### Comparing `crawlipt-0.0.6/crawlipt/actions/slide.py` & `crawlipt-0.0.7/crawlipt/actions/slide.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 
 class Slide:
     @staticmethod
     @check(exclude="driver")
     def slide(driver: WebDriver, xpath: str, position: list) -> None:
         """
-        Handling click events
+        Handling slide events
         :param driver: selenium webdriver
         :param xpath: The element to be slid
         :param position: The x, y position
         """
         assert len(position) == 2
         slider = driver.find_element(By.XPATH, xpath)
         x, y = position
```

### Comparing `crawlipt-0.0.6/crawlipt/actions/switch.py` & `crawlipt-0.0.7/crawlipt/actions/switch.py`

 * *Files identical despite different names*

### Comparing `crawlipt-0.0.6/crawlipt/actions/util.py` & `crawlipt-0.0.7/crawlipt/actions/util.py`

 * *Files 16% similar despite different names*

```diff
@@ -20,15 +20,15 @@
             return
         print(msg)
 
     @staticmethod
     @check(exclude="driver")
     def interval(driver: WebDriver, num: str | int) -> None:
         """
-        log the msg on the console
+        delay num seconds
         :param driver: selenium webdriver
         :param num: the interval number
         """
         if not driver:
             return
         if isinstance(num, str):
             num = int(num)
```

### Comparing `crawlipt-0.0.6/crawlipt/actions/window.py` & `crawlipt-0.0.7/crawlipt/actions/window.py`

 * *Files identical despite different names*

### Comparing `crawlipt-0.0.6/crawlipt/annotation.py` & `crawlipt-0.0.7/crawlipt/annotation.py`

 * *Files identical despite different names*

### Comparing `crawlipt-0.0.6/crawlipt/conditions/element.py` & `crawlipt-0.0.7/crawlipt/conditions/element.py`

 * *Files identical despite different names*

### Comparing `crawlipt-0.0.6/crawlipt/conditions/frame.py` & `crawlipt-0.0.7/crawlipt/conditions/frame.py`

 * *Files identical despite different names*

### Comparing `crawlipt-0.0.6/crawlipt/conditions/presence.py` & `crawlipt-0.0.7/crawlipt/conditions/presence.py`

 * *Files 10% similar despite different names*

```diff
@@ -32,7 +32,20 @@
         try:
             WebDriverWait(driver, wait).until(
                 EC.presence_of_all_elements_located((By.XPATH, xpath)))
             return True
         except Exception:
             return False
 
+    @staticmethod
+    @check(exclude="driver")
+    def alert_is_present(driver: WebDriver, wait: float = 1) -> bool:
+        """
+        An expectation for checking whether the given frame is available to switch to.
+        """
+        try:
+            WebDriverWait(driver, wait).until(
+                EC.alert_is_present())
+            return True
+        except Exception:
+            return False
+
```

### Comparing `crawlipt-0.0.6/crawlipt/conditions/text.py` & `crawlipt-0.0.7/crawlipt/conditions/text.py`

 * *Files identical despite different names*

### Comparing `crawlipt-0.0.6/crawlipt/conditions/visibility.py` & `crawlipt-0.0.7/crawlipt/conditions/visibility.py`

 * *Files identical despite different names*

### Comparing `crawlipt-0.0.6/crawlipt/pojo.py` & `crawlipt-0.0.7/crawlipt/pojo.py`

 * *Files identical despite different names*

### Comparing `crawlipt-0.0.6/crawlipt/script.py` & `crawlipt-0.0.7/crawlipt/script.py`

 * *Files identical despite different names*

### Comparing `crawlipt-0.0.6/crawlipt.egg-info/PKG-INFO` & `crawlipt-0.0.7/crawlipt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crawlipt
-Version: 0.0.6
+Version: 0.0.7
 Summary: The script for selenium in python
 Home-page: https://github.com/WwwwwyDev/crawlipt
 Author: WwwwwyDev
 Author-email: wwy20001014@foxmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -49,15 +49,15 @@
 You can use Crawlipt to driver the selenium by script in python.The script adopts JSON format for better cross language operations and physical storage.
 
 ## installing
 You can use pip or pip3 to install the crawlipt
 
 `pip install crawlipt` or `pip3 install crawlipt`
 
-If you have already installed crawlelip, you may need to update to the latest version
+If you have already installed crawlipt, you may need to update to the latest version
 
 `pip install --upgrade crawlipt`
 
 ## quickly start
 ```python
 from webdriver_manager.chrome import ChromeDriverManager
 from selenium import webdriver as wd
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: crawlipt Version: 0.0.6 Summary: The script for
+Metadata-Version: 2.1 Name: crawlipt Version: 0.0.7 Summary: The script for
 selenium in python Home-page: https://github.com/WwwwwyDev/crawlipt Author:
 WwwwwyDev Author-email: wwy20001014@foxmail.com License: MIT Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
 Python Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python ::
 Implementation :: CPython Classifier: Programming Language :: Python ::
 Implementation :: PyPy Requires-Python: >=3.10.0 Description-Content-Type:
@@ -10,15 +10,15 @@
                                   _[_c_r_a_w_l_i_s_t_]
                  # crawlipt The script for selenium in python
                          _[_p_y_p_i_][python]_[_G_i_t_H_u_b_ _s_t_a_r_s_]
 ## introduction You can use Crawlipt to driver the selenium by script in
 python.The script adopts JSON format for better cross language operations and
 physical storage. ## installing You can use pip or pip3 to install the crawlipt
 `pip install crawlipt` or `pip3 install crawlipt` If you have already installed
-crawlelip, you may need to update to the latest version `pip install --upgrade
+crawlipt, you may need to update to the latest version `pip install --upgrade
 crawlipt` ## quickly start ```python from webdriver_manager.chrome import
 ChromeDriverManager from selenium import webdriver as wd from
 selenium.webdriver.chrome.service import Service import crawlipt as cpt option
 = wd.ChromeOptions() option.add_argument("start-maximized") option.add_argument
 ("window-size=1920x3000") agent = 'user-agent="Mozilla/5.0 (Macintosh; Intel
 Mac OS X 10_14_1) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/70.0.3538.77
 Safari/537.36"' option.add_argument(agent) webdriver = wd.Chrome
```

### Comparing `crawlipt-0.0.6/crawlipt.egg-info/SOURCES.txt` & `crawlipt-0.0.7/crawlipt.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 crawlipt/script.py
 crawlipt.egg-info/PKG-INFO
 crawlipt.egg-info/SOURCES.txt
 crawlipt.egg-info/dependency_links.txt
 crawlipt.egg-info/requires.txt
 crawlipt.egg-info/top_level.txt
 crawlipt/actions/__init__.py
+crawlipt/actions/alert.py
 crawlipt/actions/click.py
 crawlipt/actions/get.py
 crawlipt/actions/input.py
 crawlipt/actions/redirect.py
 crawlipt/actions/scroll.py
 crawlipt/actions/select.py
 crawlipt/actions/slide.py
```

### Comparing `crawlipt-0.0.6/setup.py` & `crawlipt-0.0.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'crawlipt'
 DESCRIPTION = 'The script for selenium in python'
 URL = 'https://github.com/WwwwwyDev/crawlipt'
 EMAIL = 'wwy20001014@foxmail.com'
 AUTHOR = 'WwwwwyDev'
 REQUIRES_PYTHON = '>=3.10.0'
-VERSION = '0.0.6'
+VERSION = '0.0.7'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     "selenium>=4.0.0"
 ]
 
 # What packages are optional?
```

