# Comparing `tmp/mytiktok-0.0.4.tar.gz` & `tmp/mytiktok-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mytiktok-0.0.4.tar", last modified: Sat May  4 07:03:29 2024, max compression
+gzip compressed data, was "mytiktok-0.0.5.tar", last modified: Wed May  8 19:50:18 2024, max compression
```

## Comparing `mytiktok-0.0.4.tar` & `mytiktok-0.0.5.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 07:03:29.500765 mytiktok-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-04 07:03:25.000000 mytiktok-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-04 07:03:25.000000 mytiktok-0.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4727 2024-05-04 07:03:29.500765 mytiktok-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2447 2024-05-04 07:03:25.000000 mytiktok-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-05-04 07:03:25.000000 mytiktok-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 07:03:29.500765 mytiktok-0.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 07:03:29.496765 mytiktok-0.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 07:03:29.500765 mytiktok-0.0.4/src/mytiktok/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 07:03:29.500765 mytiktok-0.0.4/src/mytiktok/Data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 07:03:25.000000 mytiktok-0.0.4/src/mytiktok/Data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-04 07:03:25.000000 mytiktok-0.0.4/src/mytiktok/Data/cookie_names.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-05-04 07:03:25.000000 mytiktok-0.0.4/src/mytiktok/Data/cookies_analysis copy.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-05-04 07:03:25.000000 mytiktok-0.0.4/src/mytiktok/Data/cookies_analysis.txt
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-04 07:03:25.000000 mytiktok-0.0.4/src/mytiktok/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4829 2024-05-04 07:03:25.000000 mytiktok-0.0.4/src/mytiktok/account_videos.py
--rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-05-04 07:03:25.000000 mytiktok-0.0.4/src/mytiktok/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3510 2024-05-04 07:03:25.000000 mytiktok-0.0.4/src/mytiktok/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3179 2024-05-04 07:03:25.000000 mytiktok-0.0.4/src/mytiktok/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2828 2024-05-04 07:03:25.000000 mytiktok-0.0.4/src/mytiktok/login.py
--rw-r--r--   0 runner    (1001) docker     (127)     6462 2024-05-04 07:03:25.000000 mytiktok-0.0.4/src/mytiktok/tiktok.py
--rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-05-04 07:03:25.000000 mytiktok-0.0.4/src/mytiktok/video.py
--rw-r--r--   0 runner    (1001) docker     (127)     3817 2024-05-04 07:03:25.000000 mytiktok-0.0.4/src/mytiktok/videos.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 07:03:29.500765 mytiktok-0.0.4/src/mytiktok.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4727 2024-05-04 07:03:29.000000 mytiktok-0.0.4/src/mytiktok.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-04 07:03:29.000000 mytiktok-0.0.4/src/mytiktok.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 07:03:29.000000 mytiktok-0.0.4/src/mytiktok.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-04 07:03:29.000000 mytiktok-0.0.4/src/mytiktok.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-04 07:03:29.000000 mytiktok-0.0.4/src/mytiktok.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:50:18.585936 mytiktok-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-08 19:50:13.000000 mytiktok-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-08 19:50:13.000000 mytiktok-0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5582 2024-05-08 19:50:18.585936 mytiktok-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3302 2024-05-08 19:50:13.000000 mytiktok-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-05-08 19:50:13.000000 mytiktok-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 19:50:18.585936 mytiktok-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:50:18.581936 mytiktok-0.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:50:18.585936 mytiktok-0.0.5/src/mytiktok/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:50:18.585936 mytiktok-0.0.5/src/mytiktok/Data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 19:50:13.000000 mytiktok-0.0.5/src/mytiktok/Data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-08 19:50:13.000000 mytiktok-0.0.5/src/mytiktok/Data/cookie_names.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-05-08 19:50:13.000000 mytiktok-0.0.5/src/mytiktok/Data/cookies_analysis copy.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-05-08 19:50:13.000000 mytiktok-0.0.5/src/mytiktok/Data/cookies_analysis.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-08 19:50:13.000000 mytiktok-0.0.5/src/mytiktok/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4829 2024-05-08 19:50:13.000000 mytiktok-0.0.5/src/mytiktok/account_videos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-05-08 19:50:13.000000 mytiktok-0.0.5/src/mytiktok/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3510 2024-05-08 19:50:13.000000 mytiktok-0.0.5/src/mytiktok/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-05-08 19:50:13.000000 mytiktok-0.0.5/src/mytiktok/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2828 2024-05-08 19:50:13.000000 mytiktok-0.0.5/src/mytiktok/login.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6485 2024-05-08 19:50:13.000000 mytiktok-0.0.5/src/mytiktok/tiktok.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-05-08 19:50:13.000000 mytiktok-0.0.5/src/mytiktok/video.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3817 2024-05-08 19:50:13.000000 mytiktok-0.0.5/src/mytiktok/videos.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:50:18.585936 mytiktok-0.0.5/src/mytiktok.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5582 2024-05-08 19:50:18.000000 mytiktok-0.0.5/src/mytiktok.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-08 19:50:18.000000 mytiktok-0.0.5/src/mytiktok.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 19:50:18.000000 mytiktok-0.0.5/src/mytiktok.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-08 19:50:18.000000 mytiktok-0.0.5/src/mytiktok.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-08 19:50:18.000000 mytiktok-0.0.5/src/mytiktok.egg-info/top_level.txt
```

### Comparing `mytiktok-0.0.4/LICENSE` & `mytiktok-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mytiktok-0.0.4/PKG-INFO` & `mytiktok-0.0.5/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mytiktok
-Version: 0.0.4
+Version: 0.0.5
 Summary: A Simple Python Package for Scarping and Downloading Tiktok Videos
 Author-email: Dragoneyes <yolo89381@gmail.com>
 Project-URL: Homepage, https://github.com/geovanigaldemsugar/Mytiktok
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -73,14 +73,24 @@
 
 ### Linux/Unix 
 -  **`pip3 install mytiktok`**
 
 ### Windows
 -  **`pip install mytiktok`**
 
+## Visual Output
+The package itself uses undetected-chromedriver for webautomation which controls whether the chrome instance to renders or not  hence the `headless` option. Using headless mode increases the chances of a capthca being raised and scraping failed. So far in testing captcha is only noticed at `Login()`  but once login successful cookies are created and you should be fine in successive usage of the package until the cookies expire.
+
+So implementing Retries is important if your planning on using this package for a project.
+
+> [!NOTE]
+> I recommend using `headless = True` after you've aleady passed Login and generated cookies, and after you can use `headless = False` but alternatively you can just always set `headless = True`
+
+
+
 
 ## Example Usages
 ### Search for tiktok videos
 
 ```python 
 from mytiktok import Tiktok
 
@@ -115,15 +125,15 @@
 ]
 
 #the package needs an account login details to create cookie sessions 
 tiktok  = Tiktok(email=email, password=password)
 
 #returns a videos object
 videos  = tiktok.accounts(accounts=accounts, amnt=14)
-print(video.info_dict)
+print(videos.info_dict)
 
 ```
 ### Downloading Videos
 
 #### Downloads videos via Search  or Accounts
 
 ```python         
@@ -134,15 +144,15 @@
 
 ```python
 from mytiktok.video import Video
 
 url = 'https://www.tiktok.com/@calebbpartain/video/7363384781024906538'
 
 video  = Video(url = url)
-video.download(file_name='test.mp4')
+video.download(file_name='video.mp4')
 
 ```
 #### Download via Videos Class
 ```python
 from mytiktok.videos import Videos
 
 
@@ -157,16 +167,20 @@
 videos.download(folder_name='Test_videos')
 
 ```
 
 ## Limitations
 - **Uses Chrome Instances**
 - **Login attempts Frequently Fail**
-- **Download atempts can fail from time to time**
+- **Download attempts can fail from time to time**
+
+## Issues
+- [x] https://github.com/geovanigaldemsugar/Mytiktok/issues/1
+- [ ] Slow 
 
-#### If your planning to download in bulk ensure to save urls and use `Videos` class instead
+#### If you are planning to download in bulk ensure to save URLs and use the `Videos` class instead
 
 > [!NOTE]
-> If using this package headlessy, is important to your needs try running your script in a Docker
+> If using this package headlessly, is important to your needs try running your script in a Docker
 
 > [!IMPORTANT]
-> Proxing has not been implemented so there is possiblity of snaptik.app blocking you and or slowing down connection but just dont download excessively, keep the rates low and you should be fine
+> Proxing has not been implemented so there is a possibility of snaptik.app blocking you and or slowing down your connection but just don't download excessively, keep the rates low and you should be fine
```

### Comparing `mytiktok-0.0.4/pyproject.toml` & `mytiktok-0.0.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires  = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name  = "mytiktok"
-version  = "0.0.4"
+version  = "0.0.5"
 authors  = [
 {name = "Dragoneyes", email =  "yolo89381@gmail.com"}]
 description  = "A Simple Python Package for Scarping and Downloading Tiktok Videos"
 readme  = "README.md"
 classifiers  = [ 
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: MIT License",
```

### Comparing `mytiktok-0.0.4/src/mytiktok/Data/cookies_analysis copy.txt` & `mytiktok-0.0.5/src/mytiktok/Data/cookies_analysis copy.txt`

 * *Files identical despite different names*

### Comparing `mytiktok-0.0.4/src/mytiktok/Data/cookies_analysis.txt` & `mytiktok-0.0.5/src/mytiktok/Data/cookies_analysis.txt`

 * *Files identical despite different names*

### Comparing `mytiktok-0.0.4/src/mytiktok/account_videos.py` & `mytiktok-0.0.5/src/mytiktok/account_videos.py`

 * *Files identical despite different names*

### Comparing `mytiktok-0.0.4/src/mytiktok/base.py` & `mytiktok-0.0.5/src/mytiktok/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,19 +22,20 @@
 
         #define options
         options = uc.ChromeOptions()
         options.add_argument('--no-sandbox') #prevents slenium from not accessing system resources
         # options.add_argument(f'--proxy-server={proxy}')
         # options.add_argument(f'user-agent={random_ua}')
         options.add_argument("--disable-blink-features=AutomationControlled")
+        options.add_argument('--disable-gpu')
+
 
         # set driver to headless mode
         if headless:
             options.add_argument('--headless')
-            options.add_argument('--disable-gpu')
 
         self.options = options
 
     def driver(self):
         self.driver = uc.Chrome(options = self.options)
         
         return self.driver
```

### Comparing `mytiktok-0.0.4/src/mytiktok/exceptions.py` & `mytiktok-0.0.5/src/mytiktok/exceptions.py`

 * *Files identical despite different names*

### Comparing `mytiktok-0.0.4/src/mytiktok/helper.py` & `mytiktok-0.0.5/src/mytiktok/helper.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,22 +71,22 @@
 
             if name in important_cookies:
                     expiry  = cookie.get('expiry')
                     cookies_expiry_to_test.append(expiry)
                     
             todays_date = time.time()
             
-            earliest_expiry  = min(cookies_expiry_to_test)
+        earliest_expiry  = min(cookies_expiry_to_test)
 
-            if earliest_expiry <= todays_date: 
-                expired = True
-            else:
-                expired = False
+        if earliest_expiry <= todays_date: 
+            expired = True
+        else:
+            expired = False
 
-            return expired
+        return expired
 
     
     @staticmethod
     def __cookies_exist(file_path):
        return os.path.exists(file_path)
             
     @staticmethod
```

### Comparing `mytiktok-0.0.4/src/mytiktok/login.py` & `mytiktok-0.0.5/src/mytiktok/login.py`

 * *Files identical despite different names*

### Comparing `mytiktok-0.0.4/src/mytiktok/tiktok.py` & `mytiktok-0.0.5/src/mytiktok/tiktok.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,17 +119,17 @@
             
             self.login._login(page=account_page) 
 
             time.sleep(1)            
 
             if save and not os.path.exists(save_folder): 
                 os.makedirs(save_folder)
-
+            print(acct)
             urls  = self.__get_urls_base (save=save, save_path=save_path,load_time=load_time, amnt = amnt)
-            print(urls)
+            # print(urls)
             urls_of_accounts[acct]  = urls
         
         #finished scraped now quitting
         self.driver.quit()
         print("All Accounts found!!")
 
         
@@ -153,15 +153,15 @@
             scroll = self.wait.until(EC.presence_of_element_located((By.TAG_NAME, 'body') ))
             scroll.send_keys(Keys.END)
             
             #Give time for elements to load 
             time.sleep(load_time)  
 
             #find link elements containing links
-            link_elements = self.wait.until(EC.visibility_of_all_elements_located((By.XPATH,  '//div[@class=" css-1as5cen-DivWrapper e1cg0wnj1"]//a')))
+            link_elements = self.wait.until(EC.presence_of_all_elements_located((By.XPATH,  '//div[@class=" css-1as5cen-DivWrapper e1cg0wnj1"]//a')))
 
 
             posts = [element.get_attribute('href') for element in link_elements]
 
             #get those links
             for url in posts:
                 media_type  = url.split('/')[-2]
```

### Comparing `mytiktok-0.0.4/src/mytiktok/video.py` & `mytiktok-0.0.5/src/mytiktok/video.py`

 * *Files identical despite different names*

### Comparing `mytiktok-0.0.4/src/mytiktok/videos.py` & `mytiktok-0.0.5/src/mytiktok/videos.py`

 * *Files identical despite different names*

### Comparing `mytiktok-0.0.4/src/mytiktok.egg-info/PKG-INFO` & `mytiktok-0.0.5/src/mytiktok.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mytiktok
-Version: 0.0.4
+Version: 0.0.5
 Summary: A Simple Python Package for Scarping and Downloading Tiktok Videos
 Author-email: Dragoneyes <yolo89381@gmail.com>
 Project-URL: Homepage, https://github.com/geovanigaldemsugar/Mytiktok
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -73,14 +73,24 @@
 
 ### Linux/Unix 
 -  **`pip3 install mytiktok`**
 
 ### Windows
 -  **`pip install mytiktok`**
 
+## Visual Output
+The package itself uses undetected-chromedriver for webautomation which controls whether the chrome instance to renders or not  hence the `headless` option. Using headless mode increases the chances of a capthca being raised and scraping failed. So far in testing captcha is only noticed at `Login()`  but once login successful cookies are created and you should be fine in successive usage of the package until the cookies expire.
+
+So implementing Retries is important if your planning on using this package for a project.
+
+> [!NOTE]
+> I recommend using `headless = True` after you've aleady passed Login and generated cookies, and after you can use `headless = False` but alternatively you can just always set `headless = True`
+
+
+
 
 ## Example Usages
 ### Search for tiktok videos
 
 ```python 
 from mytiktok import Tiktok
 
@@ -115,15 +125,15 @@
 ]
 
 #the package needs an account login details to create cookie sessions 
 tiktok  = Tiktok(email=email, password=password)
 
 #returns a videos object
 videos  = tiktok.accounts(accounts=accounts, amnt=14)
-print(video.info_dict)
+print(videos.info_dict)
 
 ```
 ### Downloading Videos
 
 #### Downloads videos via Search  or Accounts
 
 ```python         
@@ -134,15 +144,15 @@
 
 ```python
 from mytiktok.video import Video
 
 url = 'https://www.tiktok.com/@calebbpartain/video/7363384781024906538'
 
 video  = Video(url = url)
-video.download(file_name='test.mp4')
+video.download(file_name='video.mp4')
 
 ```
 #### Download via Videos Class
 ```python
 from mytiktok.videos import Videos
 
 
@@ -157,16 +167,20 @@
 videos.download(folder_name='Test_videos')
 
 ```
 
 ## Limitations
 - **Uses Chrome Instances**
 - **Login attempts Frequently Fail**
-- **Download atempts can fail from time to time**
+- **Download attempts can fail from time to time**
+
+## Issues
+- [x] https://github.com/geovanigaldemsugar/Mytiktok/issues/1
+- [ ] Slow 
 
-#### If your planning to download in bulk ensure to save urls and use `Videos` class instead
+#### If you are planning to download in bulk ensure to save URLs and use the `Videos` class instead
 
 > [!NOTE]
-> If using this package headlessy, is important to your needs try running your script in a Docker
+> If using this package headlessly, is important to your needs try running your script in a Docker
 
 > [!IMPORTANT]
-> Proxing has not been implemented so there is possiblity of snaptik.app blocking you and or slowing down connection but just dont download excessively, keep the rates low and you should be fine
+> Proxing has not been implemented so there is a possibility of snaptik.app blocking you and or slowing down your connection but just don't download excessively, keep the rates low and you should be fine
```

### Comparing `mytiktok-0.0.4/src/mytiktok.egg-info/SOURCES.txt` & `mytiktok-0.0.5/src/mytiktok.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mytiktok-0.0.4/src/mytiktok.egg-info/requires.txt` & `mytiktok-0.0.5/src/mytiktok.egg-info/requires.txt`

 * *Files identical despite different names*

