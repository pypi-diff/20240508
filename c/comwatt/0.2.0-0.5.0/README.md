# Comparing `tmp/comwatt-0.2.0.tar.gz` & `tmp/comwatt-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "comwatt-0.2.0.tar", last modified: Sun May  5 16:57:08 2024, max compression
+gzip compressed data, was "comwatt-0.5.0.tar", last modified: Wed May  8 16:31:49 2024, max compression
```

## Comparing `comwatt-0.2.0.tar` & `comwatt-0.5.0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 christophe  (1000) christophe  (1000)        0 2024-05-05 16:57:08.960744 comwatt-0.2.0/
--rw-r--r--   0 christophe  (1000) christophe  (1000)     1074 2023-04-15 15:46:41.000000 comwatt-0.2.0/LICENSE
--rw-r--r--   0 christophe  (1000) christophe  (1000)      273 2024-05-05 16:57:08.960744 comwatt-0.2.0/PKG-INFO
-drwxr-xr-x   0 christophe  (1000) christophe  (1000)        0 2024-05-05 16:57:08.960744 comwatt-0.2.0/comwatt/
--rwxr-xr-x   0 christophe  (1000) christophe  (1000)     4341 2024-05-04 19:08:31.000000 comwatt-0.2.0/comwatt/__init__.py
-drwxr-xr-x   0 christophe  (1000) christophe  (1000)        0 2024-05-05 16:57:08.960744 comwatt-0.2.0/comwatt.egg-info/
--rw-r--r--   0 christophe  (1000) christophe  (1000)      273 2024-05-05 16:57:08.000000 comwatt-0.2.0/comwatt.egg-info/PKG-INFO
--rw-r--r--   0 christophe  (1000) christophe  (1000)      205 2024-05-05 16:57:08.000000 comwatt-0.2.0/comwatt.egg-info/SOURCES.txt
--rw-r--r--   0 christophe  (1000) christophe  (1000)        1 2024-05-05 16:57:08.000000 comwatt-0.2.0/comwatt.egg-info/dependency_links.txt
--rw-r--r--   0 christophe  (1000) christophe  (1000)        9 2024-05-05 16:57:08.000000 comwatt-0.2.0/comwatt.egg-info/requires.txt
--rw-r--r--   0 christophe  (1000) christophe  (1000)        8 2024-05-05 16:57:08.000000 comwatt-0.2.0/comwatt.egg-info/top_level.txt
--rw-r--r--   0 christophe  (1000) christophe  (1000)       81 2023-04-16 19:12:44.000000 comwatt-0.2.0/pyproject.toml
--rw-r--r--   0 christophe  (1000) christophe  (1000)       38 2024-05-05 16:57:08.960744 comwatt-0.2.0/setup.cfg
--rw-r--r--   0 christophe  (1000) christophe  (1000)      370 2024-05-05 16:56:44.000000 comwatt-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:31:49.223131 comwatt-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-08 16:31:45.000000 comwatt-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-08 16:31:49.223131 comwatt-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-08 16:31:45.000000 comwatt-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:31:49.219131 comwatt-0.5.0/comwatt/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5433 2024-05-08 16:31:45.000000 comwatt-0.5.0/comwatt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:31:49.223131 comwatt-0.5.0/comwatt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-08 16:31:49.000000 comwatt-0.5.0/comwatt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-08 16:31:49.000000 comwatt-0.5.0/comwatt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 16:31:49.000000 comwatt-0.5.0/comwatt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-08 16:31:49.000000 comwatt-0.5.0/comwatt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-08 16:31:49.000000 comwatt-0.5.0/comwatt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-08 16:31:45.000000 comwatt-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 16:31:49.223131 comwatt-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-08 16:31:45.000000 comwatt-0.5.0/setup.py
```

### Comparing `comwatt-0.2.0/LICENSE` & `comwatt-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `comwatt-0.2.0/comwatt/__init__.py` & `comwatt-0.5.0/comwatt/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import re
+import time
 
 from selenium import webdriver
 from selenium.webdriver.common.by import By
 from selenium.webdriver.common.keys import Keys
 from selenium.webdriver.firefox.options import Options
 from selenium.webdriver.support.wait import WebDriverWait
 
@@ -12,14 +13,21 @@
     "withdrawal",
     "sun",
     "hotwatertank",
     "plug"
 ]
 
 
+URL_LOGIN = "https://energy.comwatt.com/#/login/"
+
+
+class LoginError(Exception):
+    pass
+
+
 class Zone(object):
 
     def __init__(self, title):
 
         self.title = title
         self.devices = []
 
@@ -39,48 +47,84 @@
         self.zone = None
         self.value_instant = 0
         self.initialized = False
 
 
 class PowerGEN4(webdriver.Firefox):
 
-    def __init__(self, debug = False):
+    def __init__(self, email, password, debug = False):
 
         options = Options()
 
         if not debug:
             options.add_argument("-headless")
 
         super().__init__(options=options)
     
         self.zones = []
 
         self.default_site = None
 
-    def login(self, email, password):
+        self.email = email
+        self.password = password
+
+        self.login()
+
+        self.last_refresh_time = 0
+
+    # def wait_element_by_name(self, name):
+    #     try:
+    #         WebDriverWait(self, timeout=20).until(lambda d: d.find_element(By.NAME, name))
+    #     except:
+
+    def login(self):
 
         # Get the login page
-        self.get('https://energy.comwatt.com/#/login/')
+        super().get('https://energy.comwatt.com/#/login/')
 
         WebDriverWait(self, timeout=20).until(lambda d: d.find_element(By.NAME, 'email'))
 
+        # Enter email and password
         elem = self.find_element(By.NAME, 'email')  # Find the search box
-        elem.send_keys(email + Keys.RETURN)
+        elem.send_keys(self.email + Keys.RETURN)
 
         elem = self.find_element(By.NAME, 'password')  # Find the search box
-        elem.send_keys(password + Keys.RETURN)
+        elem.send_keys(self.password + Keys.RETURN)
+
+        # Wait for next page
+        for i in range(20):
+            if self.current_url != URL_LOGIN:
+               break
+            time.sleep(1)
+
+        # Still on the login page -> login error
+        if self.current_url == URL_LOGIN:
+            raise LoginError
 
         # Wait home page
         WebDriverWait(self, timeout=20).until(lambda d: d.find_element(By.CLASS_NAME, 'css-3kduam'))
 
         m = re.match("https://energy.comwatt.com/#/sites/([abcdef0123456789]+)/home", self.current_url)
         
         self.default_site = m.group(1)
 
 
+    def get(self, url, title=None):
+        
+        # First try
+        super().get(url)
+
+        # Back to login page -> retry logins
+        if self.current_url == URL_LOGIN:
+            self.login()
+
+            # Second try
+            super().get(url)
+
+
     def meter(self, site=None):
 
         if not site:
             site = self.default_site
 
         self.get('https://energy.comwatt.com/#/sites/%s/meter/' % site)
         WebDriverWait(self, timeout=20).until(lambda d: d.find_element(By.CLASS_NAME, 'css-3kduam'))
@@ -88,15 +132,16 @@
         elem = self.find_element(By.CLASS_NAME, 'css-3kduam')
 
         data = elem.text
         assert data[-1] == "%"
         assert data[:-1].isdigit()
         return int(data[:-1])
 
-    def devices(self, site=None):
+
+    def refresh(self, site=None):
 
         if not site:
             site = self.default_site
 
         self.zones = []
 
         self.get('https://energy.comwatt.com/#/sites/%s/devices/' % site)
@@ -141,17 +186,24 @@
                     
                     if unit == "kW":
                         value *= 1000
 
                     device.initialized = True
                     device.value_instant = value
 
-        return self.zones
 
     def get_devices(self, device_type):
 
+        now = time.time()
+
+        if self.last_refresh_time + 1 < now:
+            self.refresh()
+            self.last_refresh_time = now
+
         list_devices = []
+
         for zone in self.zones:
             for device in zone.devices:
                 if device.type == device_type:
                     list_devices.append(device)
+
         return list_devices
```

