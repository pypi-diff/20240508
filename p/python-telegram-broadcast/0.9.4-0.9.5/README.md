# Comparing `tmp/python_telegram_broadcast-0.9.4.tar.gz` & `tmp/python_telegram_broadcast-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_telegram_broadcast-0.9.4.tar", last modified: Tue May  7 09:49:42 2024, max compression
+gzip compressed data, was "python_telegram_broadcast-0.9.5.tar", last modified: Wed May  8 08:49:36 2024, max compression
```

## Comparing `python_telegram_broadcast-0.9.4.tar` & `python_telegram_broadcast-0.9.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 jonah     (1000) jonah     (1000)        0 2024-05-07 09:49:42.882277 python_telegram_broadcast-0.9.4/
--rw-rw-r--   0 jonah     (1000) jonah     (1000)     1067 2024-05-06 01:52:00.000000 python_telegram_broadcast-0.9.4/LICENSE
--rw-r--r--   0 jonah     (1000) jonah     (1000)     3920 2024-05-07 09:49:42.882277 python_telegram_broadcast-0.9.4/PKG-INFO
--rw-rw-r--   0 jonah     (1000) jonah     (1000)     3331 2024-05-07 02:48:22.000000 python_telegram_broadcast-0.9.4/README.md
-drwxrwxr-x   0 jonah     (1000) jonah     (1000)        0 2024-05-07 09:49:42.882277 python_telegram_broadcast-0.9.4/python_telegram_broadcast/
--rw-rw-r--   0 jonah     (1000) jonah     (1000)     4268 2024-05-07 07:01:41.000000 python_telegram_broadcast-0.9.4/python_telegram_broadcast/__init__.py
--rw-rw-r--   0 jonah     (1000) jonah     (1000)     4039 2024-05-07 06:58:19.000000 python_telegram_broadcast-0.9.4/python_telegram_broadcast/custom_dataclass.py
--rw-rw-r--   0 jonah     (1000) jonah     (1000)     1616 2024-05-06 08:35:01.000000 python_telegram_broadcast-0.9.4/python_telegram_broadcast/custom_exception.py
--rw-rw-r--   0 jonah     (1000) jonah     (1000)     3338 2024-05-07 06:58:49.000000 python_telegram_broadcast-0.9.4/python_telegram_broadcast/custom_util.py
--rw-rw-r--   0 jonah     (1000) jonah     (1000)     3859 2024-05-07 06:57:58.000000 python_telegram_broadcast-0.9.4/python_telegram_broadcast/main.py
--rw-rw-r--   0 jonah     (1000) jonah     (1000)    17721 2024-05-07 09:46:20.000000 python_telegram_broadcast-0.9.4/python_telegram_broadcast/send_method.py
--rw-rw-r--   0 jonah     (1000) jonah     (1000)    17860 2024-05-07 06:57:50.000000 python_telegram_broadcast-0.9.4/python_telegram_broadcast/strategy.py
-drwxrwxr-x   0 jonah     (1000) jonah     (1000)        0 2024-05-07 09:49:42.882277 python_telegram_broadcast-0.9.4/python_telegram_broadcast.egg-info/
--rw-r--r--   0 jonah     (1000) jonah     (1000)     3920 2024-05-07 09:49:42.000000 python_telegram_broadcast-0.9.4/python_telegram_broadcast.egg-info/PKG-INFO
--rw-rw-r--   0 jonah     (1000) jonah     (1000)      554 2024-05-07 09:49:42.000000 python_telegram_broadcast-0.9.4/python_telegram_broadcast.egg-info/SOURCES.txt
--rw-rw-r--   0 jonah     (1000) jonah     (1000)        1 2024-05-07 09:49:42.000000 python_telegram_broadcast-0.9.4/python_telegram_broadcast.egg-info/dependency_links.txt
--rw-rw-r--   0 jonah     (1000) jonah     (1000)       33 2024-05-07 09:49:42.000000 python_telegram_broadcast-0.9.4/python_telegram_broadcast.egg-info/requires.txt
--rw-rw-r--   0 jonah     (1000) jonah     (1000)       26 2024-05-07 09:49:42.000000 python_telegram_broadcast-0.9.4/python_telegram_broadcast.egg-info/top_level.txt
--rw-rw-r--   0 jonah     (1000) jonah     (1000)       38 2024-05-07 09:49:42.882277 python_telegram_broadcast-0.9.4/setup.cfg
--rw-rw-r--   0 jonah     (1000) jonah     (1000)      952 2024-05-07 09:49:29.000000 python_telegram_broadcast-0.9.4/setup.py
+drwxrwxr-x   0 jonah     (1000) jonah     (1000)        0 2024-05-08 08:49:36.720583 python_telegram_broadcast-0.9.5/
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)     1067 2024-05-06 01:52:00.000000 python_telegram_broadcast-0.9.5/LICENSE
+-rw-r--r--   0 jonah     (1000) jonah     (1000)     3920 2024-05-08 08:49:36.720583 python_telegram_broadcast-0.9.5/PKG-INFO
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)     3331 2024-05-07 02:48:22.000000 python_telegram_broadcast-0.9.5/README.md
+drwxrwxr-x   0 jonah     (1000) jonah     (1000)        0 2024-05-08 08:49:36.720583 python_telegram_broadcast-0.9.5/python_telegram_broadcast/
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)     4119 2024-05-08 08:48:37.000000 python_telegram_broadcast-0.9.5/python_telegram_broadcast/__init__.py
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)     4039 2024-05-07 06:58:19.000000 python_telegram_broadcast-0.9.5/python_telegram_broadcast/custom_dataclass.py
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)     1616 2024-05-06 08:35:01.000000 python_telegram_broadcast-0.9.5/python_telegram_broadcast/custom_exception.py
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)     3338 2024-05-07 06:58:49.000000 python_telegram_broadcast-0.9.5/python_telegram_broadcast/custom_util.py
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)     4223 2024-05-08 08:37:54.000000 python_telegram_broadcast-0.9.5/python_telegram_broadcast/main.py
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)    19099 2024-05-08 08:33:16.000000 python_telegram_broadcast-0.9.5/python_telegram_broadcast/send_method.py
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)    17860 2024-05-07 06:57:50.000000 python_telegram_broadcast-0.9.5/python_telegram_broadcast/strategy.py
+drwxrwxr-x   0 jonah     (1000) jonah     (1000)        0 2024-05-08 08:49:36.720583 python_telegram_broadcast-0.9.5/python_telegram_broadcast.egg-info/
+-rw-r--r--   0 jonah     (1000) jonah     (1000)     3920 2024-05-08 08:49:36.000000 python_telegram_broadcast-0.9.5/python_telegram_broadcast.egg-info/PKG-INFO
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)      554 2024-05-08 08:49:36.000000 python_telegram_broadcast-0.9.5/python_telegram_broadcast.egg-info/SOURCES.txt
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)        1 2024-05-08 08:49:36.000000 python_telegram_broadcast-0.9.5/python_telegram_broadcast.egg-info/dependency_links.txt
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)       33 2024-05-08 08:49:36.000000 python_telegram_broadcast-0.9.5/python_telegram_broadcast.egg-info/requires.txt
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)       26 2024-05-08 08:49:36.000000 python_telegram_broadcast-0.9.5/python_telegram_broadcast.egg-info/top_level.txt
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)       38 2024-05-08 08:49:36.720583 python_telegram_broadcast-0.9.5/setup.cfg
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)      952 2024-05-08 08:49:21.000000 python_telegram_broadcast-0.9.5/setup.py
```

### Comparing `python_telegram_broadcast-0.9.4/LICENSE` & `python_telegram_broadcast-0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `python_telegram_broadcast-0.9.4/PKG-INFO` & `python_telegram_broadcast-0.9.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python_telegram_broadcast
-Version: 0.9.4
+Version: 0.9.5
 Summary: Package that wraps the python-telegram-bot library to make broadcasting easier.
 Author: jonah_whaler_2348
 Author-email: jk_saga@proton.me
 License: MIT
 Keywords: python,telegram,broadcast,bot
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `python_telegram_broadcast-0.9.4/README.md` & `python_telegram_broadcast-0.9.5/README.md`

 * *Files identical despite different names*

### Comparing `python_telegram_broadcast-0.9.4/python_telegram_broadcast/__init__.py` & `python_telegram_broadcast-0.9.5/python_telegram_broadcast/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 
 __title__ = "python-telegram-broadcast"
 __author__ = "Jonah Whaler"
 __license__ = "MIT"
 __copyright__ = "Copyright (c) 2024 Jonah Whaler"
 
 import asyncio
+from typing import Tuple
 from .main import handle_broadcast, get_file_id
 from .send_method import BroadcastMethodType, select_broadcast_method, string_to_BroadcastMethodType
 from .strategy import BroadcastStrategyType, select_broadcast_strategy, string_to_BroadcastStrategyType
 from .custom_util import write_sent_result, evaluate_broadcast_stats
 from .custom_dataclass import JobResponse, BroadcastStats, ErrorInformation
 
 __all__ = [
@@ -64,31 +65,24 @@
             use_multiproc=False, use_nproc=1, seconds=0.0, max_retry=5
         )
     )
 
 
 # CLI: python3 -m python_telegram_broadcast.__init__
 if __name__ == "__main__":
-    bot_token: str = "TELEGRAM_BOT_TOKEN"   # << Change to your bot token
-    user_telegram_id: int = 123456789       # << Change to your telegram id
-    file_path: str = ""                     # << Change to your file path or the URL of your file
+    bot_token: str = ""                             # << Change to your bot token
+    user_telegram_id: int = 12345678                # << Change to your telegram id
+    file_path: str = "./asset/sample_photo.jpeg"    # << Change to your file path or the URL of your file
 
     broadcast_method = select_broadcast_method(BroadcastMethodType.PHOTO)
 
-    # If file_path is a URL
-    if "://" in file_path:
-        file_id = wrapper(bot_token, broadcast_method, user_telegram_id, file_path)
-    else:
-        # Otherwise
-        file_id = wrapper(bot_token, broadcast_method, user_telegram_id, open(file_path, "rb"))
-
-    print(file_id)
+    file_id = wrapper(bot_token, broadcast_method, user_telegram_id, file_path)
 
     # Use bot_token, broadcast_method, file_path from the previous example!!!
-    export_path = ""
+    export_path = "./asset"
     broadcast_strategy = select_broadcast_strategy(BroadcastStrategyType.ASYNCIO_SEQUENTIAL)
     # Read subscriber list from file, but you can also read from database of your choice
     subscriber_list: list[Tuple[int, str]] = []
     with open("./asset/subscriber.txt", "r") as file:
         header = file.readline()
         while True:
             line = file.readline()
```

### Comparing `python_telegram_broadcast-0.9.4/python_telegram_broadcast/custom_dataclass.py` & `python_telegram_broadcast-0.9.5/python_telegram_broadcast/custom_dataclass.py`

 * *Files identical despite different names*

### Comparing `python_telegram_broadcast-0.9.4/python_telegram_broadcast/custom_exception.py` & `python_telegram_broadcast-0.9.5/python_telegram_broadcast/custom_exception.py`

 * *Files identical despite different names*

### Comparing `python_telegram_broadcast-0.9.4/python_telegram_broadcast/custom_util.py` & `python_telegram_broadcast-0.9.5/python_telegram_broadcast/custom_util.py`

 * *Files identical despite different names*

### Comparing `python_telegram_broadcast-0.9.4/python_telegram_broadcast/main.py` & `python_telegram_broadcast-0.9.5/python_telegram_broadcast/main.py`

 * *Files 14% similar despite different names*

```diff
@@ -36,17 +36,24 @@
 
 async def get_file_id(
         bot_token: str, broadcast_method: BroadcastMethodTypeHint, dummy_user: int,
         content: str, caption: str, seconds: float, max_retry: int
 ) -> str:
     try:
         bot = telegram.Bot(token=bot_token)
-        res: Union[telegram.Document, telegram.PhotoSize, telegram.Video] = await broadcast_method(
-            bot, dummy_user, content, caption, seconds, seconds, max_retry
-        )
+        if os.path.isfile(content):
+            with open(content, "rb") as payload:
+                res: Union[telegram.Document, telegram.PhotoSize, telegram.Video] = await broadcast_method(
+                    bot, dummy_user, payload.read(), caption, seconds, seconds, max_retry
+                )
+        else:
+            payload = content
+            res: Union[telegram.Document, telegram.PhotoSize, telegram.Video] = await broadcast_method(
+                bot, dummy_user, payload, caption, seconds, seconds, max_retry
+            )
         if seconds > 0:
             await asyncio.sleep(seconds)
         return res.file_id
     except Exception:
         raise
```

### Comparing `python_telegram_broadcast-0.9.4/python_telegram_broadcast/send_method.py` & `python_telegram_broadcast-0.9.5/python_telegram_broadcast/send_method.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 
 import asyncio
+import os.path
 import time
 import traceback
 from enum import Enum
 
 import telegram
 from telegram import Message, PhotoSize, Document, Video
 from telegram.constants import ParseMode
@@ -160,20 +161,27 @@
     - If the `sent_time` is < `seconds`, the function will sleep for `seconds - sent_time` seconds.
     - Return the last element of the `message.photo` list, the highest resolution photo.
     - Default timeout is 60 seconds.
     """
     timeout = 60
     t1 = time.time()
     try:
-        res = await bot.sendPhoto(
-            chat_id=target_id, photo=filename_or_url, caption=caption,
-            allow_sending_without_reply=True, protect_content=False,
-            read_timeout=timeout, write_timeout=timeout, connect_timeout=timeout, pool_timeout=timeout,
-            parse_mode=ParseMode.HTML,
-        )
+        if os.path.isfile(filename_or_url):
+            with open(filename_or_url, "rb") as payload:
+                res = await bot.sendPhoto(
+                    chat_id=target_id, photo=payload, caption=caption,
+                    allow_sending_without_reply=True, protect_content=False,
+                    read_timeout=timeout, write_timeout=timeout, connect_timeout=timeout, pool_timeout=timeout,
+                )
+        else:
+            res = await bot.sendPhoto(
+                chat_id=target_id, photo=filename_or_url, caption=caption,
+                allow_sending_without_reply=True, protect_content=False,
+                read_timeout=timeout, write_timeout=timeout, connect_timeout=timeout, pool_timeout=timeout,
+            )
         t2 = time.time()
         sent_time = t2 - t1
         if sent_time < seconds:
             await asyncio.sleep(seconds - sent_time)
         print(f"sendPhoto: {round(sent_time, 2)} seconds.")
 
         return res.photo[-1]
@@ -236,19 +244,27 @@
     Notes:
     - If the `sent_time` is < `seconds`, the function will sleep for `seconds - sent_time` seconds.
     - Default timeout is 300 seconds.
     """
     timeout = 300
     t1 = time.time()
     try:
-        res = await bot.sendVideo(
-            chat_id=target_id, video=filename_or_url, caption=caption,
-            allow_sending_without_reply=True, protect_content=False,
-            read_timeout=timeout, write_timeout=timeout, connect_timeout=timeout, pool_timeout=timeout,
-        )
+        if os.path.isfile(filename_or_url):
+            with open(filename_or_url, "rb") as payload:
+                res = await bot.sendVideo(
+                    chat_id=target_id, video=payload, caption=caption,
+                    allow_sending_without_reply=True, protect_content=False,
+                    read_timeout=timeout, write_timeout=timeout, connect_timeout=timeout, pool_timeout=timeout,
+                )
+        else:
+            res = await bot.sendVideo(
+                chat_id=target_id, video=filename_or_url, caption=caption,
+                allow_sending_without_reply=True, protect_content=False,
+                read_timeout=timeout, write_timeout=timeout, connect_timeout=timeout, pool_timeout=timeout,
+            )
         t2 = time.time()
         sent_time = t2 - t1
         if sent_time < seconds:
             await asyncio.sleep(seconds - sent_time)
         return res.video
     except FileNotFoundError as _:
         raise FileNotFoundError(f"payload: {filename_or_url}")
@@ -313,20 +329,28 @@
     -------
     - If the `sent_time` is < `seconds`, the function will sleep for `seconds - sent_time` seconds.
     - Default timeout is 120 seconds.
     """
     timeout = 120
     t1 = time.time()
     try:
-        res = await bot.sendDocument(
-            chat_id=target_id,
-            document=filename_or_url, caption=caption,
-            allow_sending_without_reply=True, protect_content=False,
-            read_timeout=timeout, write_timeout=timeout, connect_timeout=timeout, pool_timeout=timeout,
-        )
+        if os.path.isfile(filename_or_url):
+            with open(filename_or_url, "rb") as payload:
+                res = await bot.sendDocument(
+                    chat_id=target_id, document=payload, caption=caption,
+                    allow_sending_without_reply=True, protect_content=False,
+                    read_timeout=timeout, write_timeout=timeout, connect_timeout=timeout, pool_timeout=timeout,
+                )
+        else:
+            res = await bot.sendDocument(
+                chat_id=target_id,
+                document=filename_or_url, caption=caption,
+                allow_sending_without_reply=True, protect_content=False,
+                read_timeout=timeout, write_timeout=timeout, connect_timeout=timeout, pool_timeout=timeout,
+            )
         t2 = time.time()
         sent_time = t2 - t1
         if sent_time < seconds:
             await asyncio.sleep(seconds < sent_time)
         return res.document
     except FileNotFoundError as _:
         raise FileNotFoundError(f"payload: {filename_or_url}")
```

### Comparing `python_telegram_broadcast-0.9.4/python_telegram_broadcast/strategy.py` & `python_telegram_broadcast-0.9.5/python_telegram_broadcast/strategy.py`

 * *Files identical despite different names*

### Comparing `python_telegram_broadcast-0.9.4/python_telegram_broadcast.egg-info/PKG-INFO` & `python_telegram_broadcast-0.9.5/python_telegram_broadcast.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-telegram-broadcast
-Version: 0.9.4
+Version: 0.9.5
 Summary: Package that wraps the python-telegram-bot library to make broadcasting easier.
 Author: jonah_whaler_2348
 Author-email: jk_saga@proton.me
 License: MIT
 Keywords: python,telegram,broadcast,bot
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `python_telegram_broadcast-0.9.4/python_telegram_broadcast.egg-info/SOURCES.txt` & `python_telegram_broadcast-0.9.5/python_telegram_broadcast.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python_telegram_broadcast-0.9.4/setup.py` & `python_telegram_broadcast-0.9.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 DESCRIPTION = 'Package that wraps the python-telegram-bot library to make broadcasting easier.'
 
 # python3 setup.py sdist bdist_wheel
 # twine upload --skip-existing dist/*
 
-VERSION = '0.9.4'
+VERSION = '0.9.5'
 
 setup(
     name='python_telegram_broadcast',
     version=VERSION,
     packages=find_packages(),
     description=DESCRIPTION,
     long_description=open('README.md').read(),
```

