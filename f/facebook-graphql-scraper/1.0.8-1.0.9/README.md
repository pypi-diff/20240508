# Comparing `tmp/facebook-graphql-scraper-1.0.8.tar.gz` & `tmp/facebook-graphql-scraper-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "facebook-graphql-scraper-1.0.8.tar", last modified: Tue Apr 30 07:27:06 2024, max compression
+gzip compressed data, was "facebook-graphql-scraper-1.0.9.tar", last modified: Wed May  8 02:58:50 2024, max compression
```

## Comparing `facebook-graphql-scraper-1.0.8.tar` & `facebook-graphql-scraper-1.0.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-30 07:27:06.139473 facebook-graphql-scraper-1.0.8/
--rw-r--r--   0 renren     (501) staff       (20)     1055 2024-04-02 15:04:14.000000 facebook-graphql-scraper-1.0.8/LICENSE
--rw-r--r--   0 renren     (501) staff       (20)     7036 2024-04-30 07:27:06.139157 facebook-graphql-scraper-1.0.8/PKG-INFO
--rw-r--r--   0 renren     (501) staff       (20)     6548 2024-04-26 08:56:24.000000 facebook-graphql-scraper-1.0.8/README.md
-drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-30 07:27:06.134889 facebook-graphql-scraper-1.0.8/facebook_graphql_scraper.egg-info/
--rw-r--r--   0 renren     (501) staff       (20)     7036 2024-04-30 07:27:06.000000 facebook-graphql-scraper-1.0.8/facebook_graphql_scraper.egg-info/PKG-INFO
--rw-r--r--   0 renren     (501) staff       (20)      657 2024-04-30 07:27:06.000000 facebook-graphql-scraper-1.0.8/facebook_graphql_scraper.egg-info/SOURCES.txt
--rw-r--r--   0 renren     (501) staff       (20)        1 2024-04-30 07:27:06.000000 facebook-graphql-scraper-1.0.8/facebook_graphql_scraper.egg-info/dependency_links.txt
--rw-r--r--   0 renren     (501) staff       (20)       19 2024-04-30 07:27:06.000000 facebook-graphql-scraper-1.0.8/facebook_graphql_scraper.egg-info/top_level.txt
-drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-30 07:27:06.135604 facebook-graphql-scraper-1.0.8/fb_graphql_scraper/
--rw-r--r--   0 renren     (501) staff       (20)        0 2024-04-26 08:56:24.000000 facebook-graphql-scraper-1.0.8/fb_graphql_scraper/__init__.py
-drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-30 07:27:06.136175 facebook-graphql-scraper-1.0.8/fb_graphql_scraper/base/
--rw-r--r--   0 renren     (501) staff       (20)        0 2024-04-03 07:27:32.000000 facebook-graphql-scraper-1.0.8/fb_graphql_scraper/base/__init__.py
--rw-r--r--   0 renren     (501) staff       (20)      822 2024-04-03 07:55:30.000000 facebook-graphql-scraper-1.0.8/fb_graphql_scraper/base/base_page.py
--rw-r--r--   0 renren     (501) staff       (20)     1367 2024-04-26 08:56:24.000000 facebook-graphql-scraper-1.0.8/fb_graphql_scraper/example.py
--rw-r--r--   0 renren     (501) staff       (20)     9759 2024-04-30 07:26:22.000000 facebook-graphql-scraper-1.0.8/fb_graphql_scraper/facebook_graphql_scraper.py
-drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-30 07:27:06.136927 facebook-graphql-scraper-1.0.8/fb_graphql_scraper/pages/
--rw-r--r--   0 renren     (501) staff       (20)        0 2024-04-03 06:55:07.000000 facebook-graphql-scraper-1.0.8/fb_graphql_scraper/pages/__init__.py
--rw-r--r--   0 renren     (501) staff       (20)     4746 2024-04-26 08:56:24.000000 facebook-graphql-scraper-1.0.8/fb_graphql_scraper/pages/page_optional.py
-drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-30 07:27:06.137334 facebook-graphql-scraper-1.0.8/fb_graphql_scraper/tests/
--rw-r--r--   0 renren     (501) staff       (20)        0 2024-04-03 06:55:08.000000 facebook-graphql-scraper-1.0.8/fb_graphql_scraper/tests/__init__.py
-drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-30 07:27:06.138419 facebook-graphql-scraper-1.0.8/fb_graphql_scraper/utils/
--rw-r--r--   0 renren     (501) staff       (20)        0 2024-04-03 06:55:08.000000 facebook-graphql-scraper-1.0.8/fb_graphql_scraper/utils/__init__.py
--rw-r--r--   0 renren     (501) staff       (20)     2883 2024-04-26 08:56:24.000000 facebook-graphql-scraper-1.0.8/fb_graphql_scraper/utils/locator.py
--rw-r--r--   0 renren     (501) staff       (20)     3813 2024-04-26 08:56:24.000000 facebook-graphql-scraper-1.0.8/fb_graphql_scraper/utils/parser.py
--rw-r--r--   0 renren     (501) staff       (20)     6324 2024-04-26 08:56:24.000000 facebook-graphql-scraper-1.0.8/fb_graphql_scraper/utils/utils.py
--rw-r--r--   0 renren     (501) staff       (20)       38 2024-04-30 07:27:06.139548 facebook-graphql-scraper-1.0.8/setup.cfg
--rw-r--r--   0 renren     (501) staff       (20)      863 2024-04-30 07:26:22.000000 facebook-graphql-scraper-1.0.8/setup.py
+drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-05-08 02:58:50.156451 facebook-graphql-scraper-1.0.9/
+-rw-r--r--   0 renren     (501) staff       (20)     1055 2024-04-02 15:04:14.000000 facebook-graphql-scraper-1.0.9/LICENSE
+-rw-r--r--   0 renren     (501) staff       (20)     7416 2024-05-08 02:58:50.156136 facebook-graphql-scraper-1.0.9/PKG-INFO
+-rw-r--r--   0 renren     (501) staff       (20)     6928 2024-05-08 02:57:31.000000 facebook-graphql-scraper-1.0.9/README.md
+drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-05-08 02:58:50.152578 facebook-graphql-scraper-1.0.9/facebook_graphql_scraper.egg-info/
+-rw-r--r--   0 renren     (501) staff       (20)     7416 2024-05-08 02:58:50.000000 facebook-graphql-scraper-1.0.9/facebook_graphql_scraper.egg-info/PKG-INFO
+-rw-r--r--   0 renren     (501) staff       (20)      657 2024-05-08 02:58:50.000000 facebook-graphql-scraper-1.0.9/facebook_graphql_scraper.egg-info/SOURCES.txt
+-rw-r--r--   0 renren     (501) staff       (20)        1 2024-05-08 02:58:50.000000 facebook-graphql-scraper-1.0.9/facebook_graphql_scraper.egg-info/dependency_links.txt
+-rw-r--r--   0 renren     (501) staff       (20)       19 2024-05-08 02:58:50.000000 facebook-graphql-scraper-1.0.9/facebook_graphql_scraper.egg-info/top_level.txt
+drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-05-08 02:58:50.153588 facebook-graphql-scraper-1.0.9/fb_graphql_scraper/
+-rw-r--r--   0 renren     (501) staff       (20)        0 2024-04-26 08:56:24.000000 facebook-graphql-scraper-1.0.9/fb_graphql_scraper/__init__.py
+drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-05-08 02:58:50.154090 facebook-graphql-scraper-1.0.9/fb_graphql_scraper/base/
+-rw-r--r--   0 renren     (501) staff       (20)        0 2024-04-03 07:27:32.000000 facebook-graphql-scraper-1.0.9/fb_graphql_scraper/base/__init__.py
+-rw-r--r--   0 renren     (501) staff       (20)      899 2024-05-08 02:57:31.000000 facebook-graphql-scraper-1.0.9/fb_graphql_scraper/base/base_page.py
+-rw-r--r--   0 renren     (501) staff       (20)     1367 2024-04-26 08:56:24.000000 facebook-graphql-scraper-1.0.9/fb_graphql_scraper/example.py
+-rw-r--r--   0 renren     (501) staff       (20)    10661 2024-05-08 02:57:31.000000 facebook-graphql-scraper-1.0.9/fb_graphql_scraper/facebook_graphql_scraper.py
+drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-05-08 02:58:50.154457 facebook-graphql-scraper-1.0.9/fb_graphql_scraper/pages/
+-rw-r--r--   0 renren     (501) staff       (20)        0 2024-04-03 06:55:07.000000 facebook-graphql-scraper-1.0.9/fb_graphql_scraper/pages/__init__.py
+-rw-r--r--   0 renren     (501) staff       (20)     5272 2024-05-08 02:57:31.000000 facebook-graphql-scraper-1.0.9/fb_graphql_scraper/pages/page_optional.py
+drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-05-08 02:58:50.154697 facebook-graphql-scraper-1.0.9/fb_graphql_scraper/tests/
+-rw-r--r--   0 renren     (501) staff       (20)        0 2024-04-03 06:55:08.000000 facebook-graphql-scraper-1.0.9/fb_graphql_scraper/tests/__init__.py
+drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-05-08 02:58:50.155648 facebook-graphql-scraper-1.0.9/fb_graphql_scraper/utils/
+-rw-r--r--   0 renren     (501) staff       (20)        0 2024-04-03 06:55:08.000000 facebook-graphql-scraper-1.0.9/fb_graphql_scraper/utils/__init__.py
+-rw-r--r--   0 renren     (501) staff       (20)     2883 2024-04-26 08:56:24.000000 facebook-graphql-scraper-1.0.9/fb_graphql_scraper/utils/locator.py
+-rw-r--r--   0 renren     (501) staff       (20)     3814 2024-05-08 02:57:31.000000 facebook-graphql-scraper-1.0.9/fb_graphql_scraper/utils/parser.py
+-rw-r--r--   0 renren     (501) staff       (20)     6562 2024-05-08 02:57:31.000000 facebook-graphql-scraper-1.0.9/fb_graphql_scraper/utils/utils.py
+-rw-r--r--   0 renren     (501) staff       (20)       38 2024-05-08 02:58:50.156522 facebook-graphql-scraper-1.0.9/setup.cfg
+-rw-r--r--   0 renren     (501) staff       (20)      863 2024-05-08 02:57:31.000000 facebook-graphql-scraper-1.0.9/setup.py
```

### Comparing `facebook-graphql-scraper-1.0.8/LICENSE` & `facebook-graphql-scraper-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `facebook-graphql-scraper-1.0.8/facebook_graphql_scraper.egg-info/SOURCES.txt` & `facebook-graphql-scraper-1.0.9/facebook_graphql_scraper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `facebook-graphql-scraper-1.0.8/fb_graphql_scraper/base/base_page.py` & `facebook-graphql-scraper-1.0.9/fb_graphql_scraper/base/base_page.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 class BasePage(object):
     def __init__(self, driver_path):
         chrome_options = webdriver.ChromeOptions()
         chrome_options.add_argument("--disable-blink-features")
         chrome_options.add_argument("--disable-notifications")
         chrome_options.add_argument("--disable-blink-features=AutomationControlled")
         chrome_options.add_argument("--headless=new")
+        chrome_options.add_argument("--blink-settings=imagesEnabled=false")
         svc = Service(driver_path)
         self.driver = webdriver.Chrome(service=svc,options=chrome_options)
         self.driver.maximize_window()
 
 # from selenium.webdriver.chrome.service import Service
 # svc = Service(BasePage.driver_path)
 # self.driver = webdriver.Chrome(service=svc, options=chrome_options)
```

### Comparing `facebook-graphql-scraper-1.0.8/fb_graphql_scraper/example.py` & `facebook-graphql-scraper-1.0.9/fb_graphql_scraper/example.py`

 * *Files identical despite different names*

### Comparing `facebook-graphql-scraper-1.0.8/fb_graphql_scraper/facebook_graphql_scraper.py` & `facebook-graphql-scraper-1.0.9/fb_graphql_scraper/facebook_graphql_scraper.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,84 +1,90 @@
 # -*- coding: utf-8 -*-
 import pandas as pd
 import time
 import json
 from bs4 import BeautifulSoup
 import requests
-from fb_graphql_scraper.base.base_page import *
-from fb_graphql_scraper.pages.page_optional import *
+from fb_graphql_scraper.base.base_page import BasePage
+from fb_graphql_scraper.pages.page_optional import PageOptional
+from fb_graphql_scraper.utils.parser import RequestsParser
 from fb_graphql_scraper.utils.locator import *
 from fb_graphql_scraper.utils.utils import *
-from fb_graphql_scraper.utils.parser import RequestsParser
-
 
 class FacebookSettings:
+    """ How to use:
+    from fb_graphql_scraper.facebook_graphql_scraper import FacebookGraphqlScraper as fb_graphql_scraper
+    
+    # >> Example.1 - without logging in
+    if __name__ == "__main__":
+        facebook_user_name = "love.yuweishao"
+        facebook_user_id = "100044253168423"
+        days_limit = 30 # Number of days within which to scrape posts
+        driver_path = "/Users/renren/Desktop/FB_graphql_scraper拷貝/fb_graphql_scraper/resources/chromedriver-mac-arm64/chromedriver" 
+        fb_spider = fb_graphql_scraper(driver_path=driver_path)
+        res = fb_spider.get_user_posts(fb_username_or_userid=facebook_user_name, days_limit=days_limit,display_progress=True)
+        print(res)
+
+    # >> Example.2 - login in your facebook account to collect data
+    # if __name__ == "__main__":
+        # facebook_user_name = "love.yuweishao"
+        # facebook_user_id = "100044253168423"
+        # fb_account = "facebook_account"
+        # fb_pwd = "facebook_paswword"
+        # days_limit = 30 # Number of days within which to scrape posts
+        # driver_path = "/Users/renren/Desktop/FB_graphql_scraper拷貝/fb_graphql_scraper/resources/chromedriver-mac-arm64/chromedriver" 
+        # fb_spider = fb_graphql_scraper(fb_account=fb_account,fb_pwd=fb_pwd,driver_path=driver_path)
+        # res = fb_spider.get_user_posts(fb_username_or_userid=facebook_user_name, days_limit=days_limit,display_progress=True)
+        # print(res)
+    """
     def __init__(self, fb_account: str = None, fb_pwd: str = None, driver_path: str = None):
         super().__init__()
         self.fb_account = fb_account
         self.fb_pwd = fb_pwd
         self.driver_path = driver_path
-        self.set_spider(driver_path=driver_path)
-        self.set_container()
-        self.set_stop_point()
+        self._set_spider(driver_path=driver_path)
+        self._set_container()
+        self._set_stop_point()
 
-    def set_spider(self, driver_path):
+    def _set_spider(self, driver_path):
         """Description: Auto login account or click "X" button to continue,
         but some accounts cannot display info if you don't login account
         Args: url (str): target user which you want to collect data."""
         self.base_page = BasePage(driver_path=driver_path)
         self.page_optional = PageOptional(
             driver=self.base_page.driver,
             fb_account=self.fb_account,
             fb_pwd=self.fb_pwd
         )
         time.sleep(3)
         self.requests_parser = RequestsParser(driver=self.page_optional.driver)
 
-    def set_container(self):
+    def _set_container(self):
         self.post_id_list = []
         self.reaction_count_list = []
         self.profile_feed = []
         self.res = {
             "post_caption": [],
             "post_date": [],
             "post_likes": [],
             "comment_share_type": [],
             "comment_share_value": []
         }
 
-    def set_stop_point(self):
+    def _set_stop_point(self):
         self.pre_diff_days = float("-inf")
         self.counts_of_same_diff_days = 0
 
 
 class FacebookGraphqlScraper(FacebookSettings):
     def __init__(self, fb_account: str = None, fb_pwd: str = None, driver_path: str = None):
         super().__init__(fb_account=fb_account, fb_pwd=fb_pwd, driver_path=driver_path)
 
-    def move_to_next_kol(self, url: str):
-        """>> Move on to target facebook user page,
-        before moving, clean driver's requests first,
-        or driver would store previous account's data.
-        Args: url (str): user(kol) links"""
-        clear_limit = 5
-        i = 0
-        while i <= clear_limit:
-            self.page_optional.clean_requests()
-            if len(self.page_optional.driver.requests) == 0:
-                print("Clear all driver requests already!")
-                break
-            i += 1
-        self.page_optional.driver.get(url=url)
-
-    def pause(self, pause_time: int = 1):
-        time.sleep(pause_time)
-
     def check_progress(self, days_limit: int = 61, display_progress:bool=True):
-        """Check collected data date"""
+        """Check the published date of collected posts"""
         driver_requests = self.page_optional.driver.requests
         tmp_creation_array = []
         # 取得當前頁面最底部貼文
         for i in range(len(driver_requests)-1, -1, -1):
             req = driver_requests[i]
             req_response, req_url = req.response, req.url
             body_out = self.requests_parser.get_graphql_body_content(
@@ -154,19 +160,19 @@
             processed_reactions = self.requests_parser.process_reactions(
                 reactions_in=each_reactions)
             reactions_out.append(processed_reactions)
         return reactions_out
 
     def get_user_posts(self, fb_username_or_userid: str, days_limit: int = 61, display_progress:bool=True) -> dict:
         url = "https://www.facebook.com/"+fb_username_or_userid # 建立完整user連結
-        self.move_to_next_kol(url=url)# driver 跳至該連結
-        self.move_to_next_kol(url=url)# 徹底清除requests避免參雜上一用戶資料
-        self.requests_parser.clean_res() # 清空所有用於儲存結果的array
-        self.set_container() # 清空用於儲存貼文資訊的array
-        self.set_stop_point() # 設置/重置停止條件 | 停止條件: 瀏覽器無法往下取得更多貼文(n次) or 已取得目標天數內貼文
+        self.page_optional.load_next_page(url=url, clear_limit=20)# driver 跳至該連結
+        self.page_optional.load_next_page(url=url, clear_limit=20)# 徹底清除requests避免參雜上一用戶資料
+        self.requests_parser._clean_res() # 清空所有用於儲存結果的array
+        self._set_container() # 清空用於儲存貼文資訊的array
+        self._set_stop_point() # 設置/重置停止條件 | 停止條件: 瀏覽器無法往下取得更多貼文(n次) or 已取得目標天數內貼文
 
         # If you did not login, click X button
         if self.fb_account == None: self.page_optional.click_reject_login_button()
         
         # Get profile information
         try:
             profile_feed = self.get_profile_feed()
@@ -188,15 +194,15 @@
                     break
                 elif self.counts_of_same_diff_days >= 3:  # 如果找到的最遠日連續三次都是同一天表示頁面可能滾到底了
                     break
                 else:
                     counts_of_round = 0
 
             counts_of_round += 1
-            self.pause(0.3)
+            pause(0.3)
 
         # Collect data, 利用driver請求列表當中的GraphQL來取得資料
         driver_requests = self.page_optional.driver.requests
         for req in driver_requests:
             req_response, req_url = req.response, req.url
             body_out = self.requests_parser.get_graphql_body_content(
                 req_response=req_response, req_url=req_url)
```

### Comparing `facebook-graphql-scraper-1.0.8/fb_graphql_scraper/pages/page_optional.py` & `facebook-graphql-scraper-1.0.9/fb_graphql_scraper/pages/page_optional.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,14 +63,28 @@
         zoom_percent = str(zoom_percent)
         self.driver.execute_script(
             f"document.body.style.zoom='{zoom_percent}%'")
 
     def move_to_element(self, element_in):
         ActionChains(self.driver).move_to_element(element_in).perform()
 
+    def load_next_page(self, url:str, clear_limit:int=20):
+        """>> Move on to target facebook user page,
+        before moving, clean driver's requests first,
+        or driver would store previous account's data.
+        Args: url (str): user(kol) links"""
+        i = 0
+        while i <= clear_limit:
+            self.clean_requests()
+            if len(self.driver.requests) == 0:
+                print("Clear all driver requests already!")
+                break
+            i += 1
+        self.driver.get(url=url)
+
     def click_display_button(self):
         elements = self.driver.find_elements(self.locator.DISPLAY_MORE)
         for _ in range(10):
             for each_element in elements:
                 if each_element.text == self.page_text.DISPLAY_MORE or each_element.text == self.page_text.DISPLAY_MORE2:
                     self.move_to_element(element_in=each_element)
                     self.scroll_window_with_parameter(parameter_in="500")
```

### Comparing `facebook-graphql-scraper-1.0.8/fb_graphql_scraper/utils/locator.py` & `facebook-graphql-scraper-1.0.9/fb_graphql_scraper/utils/locator.py`

 * *Files identical despite different names*

### Comparing `facebook-graphql-scraper-1.0.8/fb_graphql_scraper/utils/parser.py` & `facebook-graphql-scraper-1.0.9/fb_graphql_scraper/utils/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
             response = req_response
             body = decode(response.body, response.headers.get(
                 'Content-Encoding', 'identity'))
             body_content = body.decode("utf-8").split("\n")
             return body_content
         return None
     
-    def clean_res(self):
+    def _clean_res(self):
         self.res_new = []
         self.feedback_list = []
         self.context_list = []
         self.creation_list = []
         self.author_id_list = []
         self.author_id_list2 = []
         self.owning_profile = []
```

### Comparing `facebook-graphql-scraper-1.0.8/fb_graphql_scraper/utils/utils.py` & `facebook-graphql-scraper-1.0.9/fb_graphql_scraper/utils/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # -*- coding: utf-8 -*-
 import concurrent.futures as futures
 from datetime import datetime
 import pytz
+import time
 
 
 # if key: 'subscription_target_id' in feedback, store this feedback
 def find_feedback_with_subscription_target_id(data):
     if isinstance(data, dict):
         if 'feedback' in data and isinstance(data['feedback'], dict):
             feedback = data['feedback']
@@ -154,18 +155,29 @@
     target_timezone = pytz.timezone(timezone)
     target_current_time = current_time_utc.replace(
         tzinfo=pytz.utc).astimezone(target_timezone)
     return target_current_time
 
 
 def days_difference_from_now(tmp_creation_array: list) -> int:
+    """計算第一次發文日期與當前日間隔天數
+
+    Args:
+        tmp_creation_array (list): _description_
+
+    Returns:
+        int: 間隔天數
+    """
     timestamp = min(tmp_creation_array)
     current_date_time = datetime.now()
     date_time_obj = datetime.fromtimestamp(timestamp)
     difference = current_date_time - date_time_obj
     return difference.days
 
 
 def is_date_exceed_limit(max_days_ago, days_limit: int = 61):
     if max_days_ago > days_limit:
         return True
     return False
+
+def pause(pause_time: int = 1):
+    time.sleep(pause_time)
```

### Comparing `facebook-graphql-scraper-1.0.8/setup.py` & `facebook-graphql-scraper-1.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 import setuptools
 from setuptools import setup, find_packages
 
 setup(
     name='facebook-graphql-scraper',
-    version='1.0.8',
+    version='1.0.9',
     packages=[
         "fb_graphql_scraper",
         "fb_graphql_scraper.pages",
         "fb_graphql_scraper.base",
         "fb_graphql_scraper.tests", 
         "fb_graphql_scraper.utils",
         ],
```

