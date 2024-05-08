# Comparing `tmp/anotify-0.0.4.tar.gz` & `tmp/anotify-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anotify-0.0.4.tar", last modified: Tue May  7 02:30:37 2024, max compression
+gzip compressed data, was "anotify-0.0.5.tar", last modified: Wed May  8 10:40:48 2024, max compression
```

## Comparing `anotify-0.0.4.tar` & `anotify-0.0.5.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:30:37.713216 anotify-0.0.4/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:30:37.713216 anotify-0.0.4/ANotify/
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-07 02:30:32.000000 anotify-0.0.4/ANotify/Nanpush.py
--rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-05-07 02:30:32.000000 anotify-0.0.4/ANotify/Nemail.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-07 02:30:32.000000 anotify-0.0.4/ANotify/Niyuu.py
--rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-05-07 02:30:32.000000 anotify-0.0.4/ANotify/Npushplus.py
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-07 02:30:32.000000 anotify-0.0.4/ANotify/Nserverchan.py
--rw-r--r--   0 runner    (1001) docker     (127)     6128 2024-05-07 02:30:32.000000 anotify-0.0.4/ANotify/Nwecom.py
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-05-07 02:30:32.000000 anotify-0.0.4/ANotify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-07 02:30:32.000000 anotify-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2718 2024-05-07 02:30:37.713216 anotify-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-05-07 02:30:32.000000 anotify-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:30:37.713216 anotify-0.0.4/anotify.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2718 2024-05-07 02:30:37.000000 anotify-0.0.4/anotify.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-07 02:30:37.000000 anotify-0.0.4/anotify.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 02:30:37.000000 anotify-0.0.4/anotify.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-07 02:30:37.000000 anotify-0.0.4/anotify.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-07 02:30:37.000000 anotify-0.0.4/anotify.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 02:30:37.713216 anotify-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-07 02:30:32.000000 anotify-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 10:40:48.795012 anotify-0.0.5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 10:40:48.795012 anotify-0.0.5/ANotify/
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-08 10:40:44.000000 anotify-0.0.5/ANotify/Nanpush.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-05-08 10:40:44.000000 anotify-0.0.5/ANotify/Nemail.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-08 10:40:44.000000 anotify-0.0.5/ANotify/Niyuu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-05-08 10:40:44.000000 anotify-0.0.5/ANotify/Npushplus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-08 10:40:44.000000 anotify-0.0.5/ANotify/Nserverchan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-05-08 10:40:44.000000 anotify-0.0.5/ANotify/Ntelegram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6128 2024-05-08 10:40:44.000000 anotify-0.0.5/ANotify/Nwecom.py
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-05-08 10:40:44.000000 anotify-0.0.5/ANotify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-08 10:40:44.000000 anotify-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-05-08 10:40:48.795012 anotify-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2971 2024-05-08 10:40:44.000000 anotify-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 10:40:48.795012 anotify-0.0.5/anotify.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-05-08 10:40:48.000000 anotify-0.0.5/anotify.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-08 10:40:48.000000 anotify-0.0.5/anotify.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 10:40:48.000000 anotify-0.0.5/anotify.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-08 10:40:48.000000 anotify-0.0.5/anotify.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-08 10:40:48.000000 anotify-0.0.5/anotify.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 10:40:48.795012 anotify-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-08 10:40:44.000000 anotify-0.0.5/setup.py
```

### Comparing `anotify-0.0.4/ANotify/Nanpush.py` & `anotify-0.0.5/ANotify/Nanpush.py`

 * *Files identical despite different names*

### Comparing `anotify-0.0.4/ANotify/Nemail.py` & `anotify-0.0.5/ANotify/Nemail.py`

 * *Files identical despite different names*

### Comparing `anotify-0.0.4/ANotify/Npushplus.py` & `anotify-0.0.5/ANotify/Npushplus.py`

 * *Files identical despite different names*

### Comparing `anotify-0.0.4/ANotify/Nserverchan.py` & `anotify-0.0.5/ANotify/Nserverchan.py`

 * *Files identical despite different names*

### Comparing `anotify-0.0.4/ANotify/Nwecom.py` & `anotify-0.0.5/ANotify/Nwecom.py`

 * *Files identical despite different names*

### Comparing `anotify-0.0.4/ANotify/__init__.py` & `anotify-0.0.5/ANotify/__init__.py`

 * *Files identical despite different names*

### Comparing `anotify-0.0.4/LICENSE` & `anotify-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `anotify-0.0.4/PKG-INFO` & `anotify-0.0.5/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anotify
-Version: 0.0.4
+Version: 0.0.5
 Summary: Send notifications by multiple channels.
 Home-page: https://github.com/TommyMerlin/ANotify
 Author: 7ommy
 Author-email: tommymerlin0920@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -79,14 +79,34 @@
 ```python
 from ANotify import Nserverchan
 TOKEN = ''
 serverchan = Nserverchan.ServerChanNotify(TOKEN)
 serverchan.send_msg("测试标题", "测试正文")
 ```
 
+### Telegram Bot
+[官网](https://core.telegram.org/bots)
+```python
+from ANotify import Ntelegram
+TOKEN = ''
+CHAT_ID = ''
+# 可选项
+proxy = {
+        "http": "http://127.0.0.1:1234",
+        "https": "http://127.0.0.1:1234"
+}
+telegram = Ntelegram.TelegramNotify(TOKEN, CHAT_ID)
+
+# https://core.telegram.org/bots/api#formatting-options
+telegram.send_msg("test message", Ntelegram.ParseMode.TEXT)   # 无代理
+telegram.send_msg("test message", Ntelegram.ParseMode.TEXT, proxy=proxy)
+telegram.send_msg("[link](https://www.example.com)", Ntelegram.ParseMode.Markdown, proxy=proxy)
+telegram.send_msg("<a href='https://www.example.com'>link</a>", Ntelegram.ParseMode.HTML, proxy=proxy)
+```
+
 ### Email
 ```python
 from ANotify import Nemail
 # 邮箱服务器地址
 MAIL_HOST = ''
 # 用户名
 MAIL_USER = ''
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: anotify Version: 0.0.4 Summary: Send notifications
+Metadata-Version: 2.1 Name: anotify Version: 0.0.5 Summary: Send notifications
 by multiple channels. Home-page: https://github.com/TommyMerlin/ANotify Author:
 7ommy Author-email: tommymerlin0920@gmail.com License: MIT Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Requires-Python: >=3.6 Description-Content-Type: text/markdown License-
 File: LICENSE Requires-Dist: requests>=2.15.1 ![Alt](https://
 repobeats.axiom.co/api/embed/e1ca45165d69b8370c78d60260a6474b49621fac.svg
 "Repobeats analytics image") ## å®è£ ```console pip install anotify ``` ##
@@ -23,14 +23,23 @@
 "success" } pushplus.send_msg("æµè¯æ é¢", msg_json,
 Npushplus.TemplateType.json) pushplus.send_msg("æµè¯æ é¢",
 "**æµè¯åå®¹**\n- test1\n- [ANotify](https://github.com/TommyMerlin/
 ANotify)", Npushplus.TemplateType.markdown) pushplus.send_msg("æµè¯æ é¢",
 "æµè¯åå®¹_A_N_o_t_i_f_y", Npushplus.TemplateType.html) ``` ### Serveré± [å®ç½]
 (https://sct.ftqq.com/) ```python from ANotify import Nserverchan TOKEN = ''
 serverchan = Nserverchan.ServerChanNotify(TOKEN) serverchan.send_msg
-("æµè¯æ é¢", "æµè¯æ­£æ") ``` ### Email ```python from ANotify import
-Nemail # é®ç®±æå¡å¨å°å MAIL_HOST = '' # ç¨æ·å MAIL_USER = '' #
-å¯ç (é¨åé®ç®±ä¸ºææç ) MAIL_PASS = '' # é®ä»¶åéæ¹é®ç®±å°å
-SENDER = '' email_notify = Nemail.EmailNotify(MAIL_HOST, MAIL_USER, MAIL_PASS,
-SENDER) if email_notify.send_email("æµè¯æ é¢", "æµè¯æ­£æ",
-attachment_filename=None, receiver='123@example.com'): print
-("é®ä»¶åéæåâ") else: print("é®ä»¶åéå¤±è´¥Ã") ```
+("æµè¯æ é¢", "æµè¯æ­£æ") ``` ### Telegram Bot [å®ç½](https://
+core.telegram.org/bots) ```python from ANotify import Ntelegram TOKEN = ''
+CHAT_ID = '' # å¯éé¡¹ proxy = { "http": "http://127.0.0.1:1234", "https":
+"http://127.0.0.1:1234" } telegram = Ntelegram.TelegramNotify(TOKEN, CHAT_ID) #
+https://core.telegram.org/bots/api#formatting-options telegram.send_msg("test
+message", Ntelegram.ParseMode.TEXT) # æ ä»£ç telegram.send_msg("test
+message", Ntelegram.ParseMode.TEXT, proxy=proxy) telegram.send_msg("[link]
+(https://www.example.com)", Ntelegram.ParseMode.Markdown, proxy=proxy)
+telegram.send_msg("_l_i_n_k", Ntelegram.ParseMode.HTML, proxy=proxy) ``` ### Email
+```python from ANotify import Nemail # é®ç®±æå¡å¨å°å MAIL_HOST = '' #
+ç¨æ·å MAIL_USER = '' # å¯ç (é¨åé®ç®±ä¸ºææç ) MAIL_PASS = '' #
+é®ä»¶åéæ¹é®ç®±å°å SENDER = '' email_notify = Nemail.EmailNotify
+(MAIL_HOST, MAIL_USER, MAIL_PASS, SENDER) if email_notify.send_email
+("æµè¯æ é¢", "æµè¯æ­£æ", attachment_filename=None,
+receiver='123@example.com'): print("é®ä»¶åéæåâ") else: print
+("é®ä»¶åéå¤±è´¥Ã") ```
```

### Comparing `anotify-0.0.4/README.md` & `anotify-0.0.5/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -64,14 +64,34 @@
 ```python
 from ANotify import Nserverchan
 TOKEN = ''
 serverchan = Nserverchan.ServerChanNotify(TOKEN)
 serverchan.send_msg("测试标题", "测试正文")
 ```
 
+### Telegram Bot
+[官网](https://core.telegram.org/bots)
+```python
+from ANotify import Ntelegram
+TOKEN = ''
+CHAT_ID = ''
+# 可选项
+proxy = {
+        "http": "http://127.0.0.1:1234",
+        "https": "http://127.0.0.1:1234"
+}
+telegram = Ntelegram.TelegramNotify(TOKEN, CHAT_ID)
+
+# https://core.telegram.org/bots/api#formatting-options
+telegram.send_msg("test message", Ntelegram.ParseMode.TEXT)   # 无代理
+telegram.send_msg("test message", Ntelegram.ParseMode.TEXT, proxy=proxy)
+telegram.send_msg("[link](https://www.example.com)", Ntelegram.ParseMode.Markdown, proxy=proxy)
+telegram.send_msg("<a href='https://www.example.com'>link</a>", Ntelegram.ParseMode.HTML, proxy=proxy)
+```
+
 ### Email
 ```python
 from ANotify import Nemail
 # 邮箱服务器地址
 MAIL_HOST = ''
 # 用户名
 MAIL_USER = ''
```

#### html2text {}

```diff
@@ -17,15 +17,24 @@
 msg_json = { "status": 200, "msg": "success" } pushplus.send_msg
 ("æµè¯æ é¢", msg_json, Npushplus.TemplateType.json) pushplus.send_msg
 ("æµè¯æ é¢", "**æµè¯åå®¹**\n- test1\n- [ANotify](https://github.com/
 TommyMerlin/ANotify)", Npushplus.TemplateType.markdown) pushplus.send_msg
 ("æµè¯æ é¢", "æµè¯åå®¹_A_N_o_t_i_f_y", Npushplus.TemplateType.html) ``` ###
 Serveré± [å®ç½](https://sct.ftqq.com/) ```python from ANotify import
 Nserverchan TOKEN = '' serverchan = Nserverchan.ServerChanNotify(TOKEN)
-serverchan.send_msg("æµè¯æ é¢", "æµè¯æ­£æ") ``` ### Email ```python
-from ANotify import Nemail # é®ç®±æå¡å¨å°å MAIL_HOST = '' # ç¨æ·å
+serverchan.send_msg("æµè¯æ é¢", "æµè¯æ­£æ") ``` ### Telegram Bot
+[å®ç½](https://core.telegram.org/bots) ```python from ANotify import
+Ntelegram TOKEN = '' CHAT_ID = '' # å¯éé¡¹ proxy = { "http": "http://
+127.0.0.1:1234", "https": "http://127.0.0.1:1234" } telegram =
+Ntelegram.TelegramNotify(TOKEN, CHAT_ID) # https://core.telegram.org/bots/
+api#formatting-options telegram.send_msg("test message",
+Ntelegram.ParseMode.TEXT) # æ ä»£ç telegram.send_msg("test message",
+Ntelegram.ParseMode.TEXT, proxy=proxy) telegram.send_msg("[link](https://
+www.example.com)", Ntelegram.ParseMode.Markdown, proxy=proxy) telegram.send_msg
+("_l_i_n_k", Ntelegram.ParseMode.HTML, proxy=proxy) ``` ### Email ```python from
+ANotify import Nemail # é®ç®±æå¡å¨å°å MAIL_HOST = '' # ç¨æ·å
 MAIL_USER = '' # å¯ç (é¨åé®ç®±ä¸ºææç ) MAIL_PASS = '' #
 é®ä»¶åéæ¹é®ç®±å°å SENDER = '' email_notify = Nemail.EmailNotify
 (MAIL_HOST, MAIL_USER, MAIL_PASS, SENDER) if email_notify.send_email
 ("æµè¯æ é¢", "æµè¯æ­£æ", attachment_filename=None,
 receiver='123@example.com'): print("é®ä»¶åéæåâ") else: print
 ("é®ä»¶åéå¤±è´¥Ã") ```
```

### Comparing `anotify-0.0.4/anotify.egg-info/PKG-INFO` & `anotify-0.0.5/anotify.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anotify
-Version: 0.0.4
+Version: 0.0.5
 Summary: Send notifications by multiple channels.
 Home-page: https://github.com/TommyMerlin/ANotify
 Author: 7ommy
 Author-email: tommymerlin0920@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -79,14 +79,34 @@
 ```python
 from ANotify import Nserverchan
 TOKEN = ''
 serverchan = Nserverchan.ServerChanNotify(TOKEN)
 serverchan.send_msg("测试标题", "测试正文")
 ```
 
+### Telegram Bot
+[官网](https://core.telegram.org/bots)
+```python
+from ANotify import Ntelegram
+TOKEN = ''
+CHAT_ID = ''
+# 可选项
+proxy = {
+        "http": "http://127.0.0.1:1234",
+        "https": "http://127.0.0.1:1234"
+}
+telegram = Ntelegram.TelegramNotify(TOKEN, CHAT_ID)
+
+# https://core.telegram.org/bots/api#formatting-options
+telegram.send_msg("test message", Ntelegram.ParseMode.TEXT)   # 无代理
+telegram.send_msg("test message", Ntelegram.ParseMode.TEXT, proxy=proxy)
+telegram.send_msg("[link](https://www.example.com)", Ntelegram.ParseMode.Markdown, proxy=proxy)
+telegram.send_msg("<a href='https://www.example.com'>link</a>", Ntelegram.ParseMode.HTML, proxy=proxy)
+```
+
 ### Email
 ```python
 from ANotify import Nemail
 # 邮箱服务器地址
 MAIL_HOST = ''
 # 用户名
 MAIL_USER = ''
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: anotify Version: 0.0.4 Summary: Send notifications
+Metadata-Version: 2.1 Name: anotify Version: 0.0.5 Summary: Send notifications
 by multiple channels. Home-page: https://github.com/TommyMerlin/ANotify Author:
 7ommy Author-email: tommymerlin0920@gmail.com License: MIT Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Requires-Python: >=3.6 Description-Content-Type: text/markdown License-
 File: LICENSE Requires-Dist: requests>=2.15.1 ![Alt](https://
 repobeats.axiom.co/api/embed/e1ca45165d69b8370c78d60260a6474b49621fac.svg
 "Repobeats analytics image") ## å®è£ ```console pip install anotify ``` ##
@@ -23,14 +23,23 @@
 "success" } pushplus.send_msg("æµè¯æ é¢", msg_json,
 Npushplus.TemplateType.json) pushplus.send_msg("æµè¯æ é¢",
 "**æµè¯åå®¹**\n- test1\n- [ANotify](https://github.com/TommyMerlin/
 ANotify)", Npushplus.TemplateType.markdown) pushplus.send_msg("æµè¯æ é¢",
 "æµè¯åå®¹_A_N_o_t_i_f_y", Npushplus.TemplateType.html) ``` ### Serveré± [å®ç½]
 (https://sct.ftqq.com/) ```python from ANotify import Nserverchan TOKEN = ''
 serverchan = Nserverchan.ServerChanNotify(TOKEN) serverchan.send_msg
-("æµè¯æ é¢", "æµè¯æ­£æ") ``` ### Email ```python from ANotify import
-Nemail # é®ç®±æå¡å¨å°å MAIL_HOST = '' # ç¨æ·å MAIL_USER = '' #
-å¯ç (é¨åé®ç®±ä¸ºææç ) MAIL_PASS = '' # é®ä»¶åéæ¹é®ç®±å°å
-SENDER = '' email_notify = Nemail.EmailNotify(MAIL_HOST, MAIL_USER, MAIL_PASS,
-SENDER) if email_notify.send_email("æµè¯æ é¢", "æµè¯æ­£æ",
-attachment_filename=None, receiver='123@example.com'): print
-("é®ä»¶åéæåâ") else: print("é®ä»¶åéå¤±è´¥Ã") ```
+("æµè¯æ é¢", "æµè¯æ­£æ") ``` ### Telegram Bot [å®ç½](https://
+core.telegram.org/bots) ```python from ANotify import Ntelegram TOKEN = ''
+CHAT_ID = '' # å¯éé¡¹ proxy = { "http": "http://127.0.0.1:1234", "https":
+"http://127.0.0.1:1234" } telegram = Ntelegram.TelegramNotify(TOKEN, CHAT_ID) #
+https://core.telegram.org/bots/api#formatting-options telegram.send_msg("test
+message", Ntelegram.ParseMode.TEXT) # æ ä»£ç telegram.send_msg("test
+message", Ntelegram.ParseMode.TEXT, proxy=proxy) telegram.send_msg("[link]
+(https://www.example.com)", Ntelegram.ParseMode.Markdown, proxy=proxy)
+telegram.send_msg("_l_i_n_k", Ntelegram.ParseMode.HTML, proxy=proxy) ``` ### Email
+```python from ANotify import Nemail # é®ç®±æå¡å¨å°å MAIL_HOST = '' #
+ç¨æ·å MAIL_USER = '' # å¯ç (é¨åé®ç®±ä¸ºææç ) MAIL_PASS = '' #
+é®ä»¶åéæ¹é®ç®±å°å SENDER = '' email_notify = Nemail.EmailNotify
+(MAIL_HOST, MAIL_USER, MAIL_PASS, SENDER) if email_notify.send_email
+("æµè¯æ é¢", "æµè¯æ­£æ", attachment_filename=None,
+receiver='123@example.com'): print("é®ä»¶åéæåâ") else: print
+("é®ä»¶åéå¤±è´¥Ã") ```
```

### Comparing `anotify-0.0.4/setup.py` & `anotify-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='anotify',
-    version='0.0.4',
+    version='0.0.5',
     packages=find_packages(),
     install_requires=[
         'requests>=2.15.1',
     ],
     author='7ommy',
     author_email='tommymerlin0920@gmail.com',
     description='Send notifications by multiple channels.',
```

