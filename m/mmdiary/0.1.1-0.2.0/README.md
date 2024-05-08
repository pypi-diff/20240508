# Comparing `tmp/mmdiary-0.1.1.tar.gz` & `tmp/mmdiary-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mmdiary-0.1.1.tar", last modified: Wed May  1 19:39:54 2024, max compression
+gzip compressed data, was "mmdiary-0.2.0.tar", last modified: Wed May  8 00:21:14 2024, max compression
```

## Comparing `mmdiary-0.1.1.tar` & `mmdiary-0.2.0.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)        0 2024-05-01 19:39:54.780954 mmdiary-0.1.1/
--rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)    35149 2024-05-01 19:37:11.000000 mmdiary-0.1.1/LICENSE
--rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)    43431 2024-05-01 19:39:54.780954 mmdiary-0.1.1/PKG-INFO
--rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)     1569 2024-05-01 19:37:11.000000 mmdiary-0.1.1/README.md
--rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)     2168 2024-05-01 19:39:01.000000 mmdiary-0.1.1/pyproject.toml
--rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)       38 2024-05-01 19:39:54.780954 mmdiary-0.1.1/setup.cfg
-drwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)        0 2024-05-01 19:39:54.772954 mmdiary-0.1.1/src/
-drwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)        0 2024-05-01 19:39:54.776954 mmdiary-0.1.1/src/mmdiary/
--rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)        0 2024-05-01 14:53:11.000000 mmdiary-0.1.1/src/mmdiary/__init__.py
-drwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)        0 2024-05-01 19:39:54.776954 mmdiary-0.1.1/src/mmdiary/notion/
--rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)        0 2024-05-01 14:53:17.000000 mmdiary-0.1.1/src/mmdiary/notion/__init__.py
--rwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)     4199 2024-05-01 14:40:07.000000 mmdiary-0.1.1/src/mmdiary/notion/cachedb.py
--rwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)     2158 2024-05-01 15:24:12.000000 mmdiary-0.1.1/src/mmdiary/notion/cleanup.py
--rwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)     8248 2024-05-01 18:50:11.000000 mmdiary-0.1.1/src/mmdiary/notion/uploader.py
-drwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)        0 2024-05-01 19:39:54.776954 mmdiary-0.1.1/src/mmdiary/telegrambot/
--rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)        0 2024-05-01 14:53:27.000000 mmdiary-0.1.1/src/mmdiary/telegrambot/__init__.py
--rwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)     7869 2024-05-01 16:58:22.000000 mmdiary-0.1.1/src/mmdiary/telegrambot/telegrambot_service.py
-drwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)        0 2024-05-01 19:39:54.780954 mmdiary-0.1.1/src/mmdiary/transcriber/
--rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)        0 2024-05-01 14:53:32.000000 mmdiary-0.1.1/src/mmdiary/transcriber/__init__.py
--rwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)     1308 2024-05-01 19:16:55.000000 mmdiary-0.1.1/src/mmdiary/transcriber/searcher.py
--rwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)     3654 2024-05-01 19:06:23.000000 mmdiary-0.1.1/src/mmdiary/transcriber/transcriber.py
--rwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)    10583 2024-05-01 19:05:26.000000 mmdiary-0.1.1/src/mmdiary/transcriber/verifier.py
-drwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)        0 2024-05-01 19:39:54.780954 mmdiary-0.1.1/src/mmdiary/utils/
--rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)        0 2024-05-01 15:08:11.000000 mmdiary-0.1.1/src/mmdiary/utils/__init__.py
--rwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)     6208 2024-05-01 15:30:50.000000 mmdiary-0.1.1/src/mmdiary/utils/datelib.py
--rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)     1004 2024-05-01 14:41:54.000000 mmdiary-0.1.1/src/mmdiary/utils/log.py
--rwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)     3275 2024-05-01 16:55:19.000000 mmdiary-0.1.1/src/mmdiary/utils/medialib.py
--rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)      368 2024-05-01 17:19:04.000000 mmdiary-0.1.1/src/mmdiary/utils/progressbar.py
-drwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)        0 2024-05-01 19:39:54.780954 mmdiary-0.1.1/src/mmdiary/video/
--rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)        0 2024-05-01 14:53:43.000000 mmdiary-0.1.1/src/mmdiary/video/__init__.py
--rwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)     3746 2024-05-01 17:10:58.000000 mmdiary-0.1.1/src/mmdiary/video/processor.py
--rwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)     8102 2024-05-01 17:10:01.000000 mmdiary-0.1.1/src/mmdiary/video/uploader.py
-drwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)        0 2024-05-01 19:39:54.776954 mmdiary-0.1.1/src/mmdiary.egg-info/
--rw-r--r--   0 sashacmc  (1000) sashacmc  (1000)    43431 2024-05-01 19:39:54.000000 mmdiary-0.1.1/src/mmdiary.egg-info/PKG-INFO
--rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)      858 2024-05-01 19:39:54.000000 mmdiary-0.1.1/src/mmdiary.egg-info/SOURCES.txt
--rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)        1 2024-05-01 19:39:54.000000 mmdiary-0.1.1/src/mmdiary.egg-info/dependency_links.txt
--rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)      536 2024-05-01 19:39:54.000000 mmdiary-0.1.1/src/mmdiary.egg-info/entry_points.txt
--rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)      145 2024-05-01 19:39:54.000000 mmdiary-0.1.1/src/mmdiary.egg-info/requires.txt
--rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)        8 2024-05-01 19:39:54.000000 mmdiary-0.1.1/src/mmdiary.egg-info/top_level.txt
+drwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)        0 2024-05-08 00:21:14.010244 mmdiary-0.2.0/
+-rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)    35149 2024-05-01 19:37:11.000000 mmdiary-0.2.0/LICENSE
+-rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)    43431 2024-05-08 00:21:14.010244 mmdiary-0.2.0/PKG-INFO
+-rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)     1569 2024-05-01 19:37:11.000000 mmdiary-0.2.0/README.md
+-rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)     2228 2024-05-08 00:11:48.000000 mmdiary-0.2.0/pyproject.toml
+-rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)       38 2024-05-08 00:21:14.010244 mmdiary-0.2.0/setup.cfg
+drwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)        0 2024-05-08 00:21:14.006244 mmdiary-0.2.0/src/
+drwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)        0 2024-05-08 00:21:14.006244 mmdiary-0.2.0/src/mmdiary/
+-rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)        0 2024-05-01 14:53:11.000000 mmdiary-0.2.0/src/mmdiary/__init__.py
+drwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)        0 2024-05-08 00:21:14.006244 mmdiary-0.2.0/src/mmdiary/notion/
+-rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)        0 2024-05-01 14:53:17.000000 mmdiary-0.2.0/src/mmdiary/notion/__init__.py
+-rwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)     3351 2024-05-07 10:50:37.000000 mmdiary-0.2.0/src/mmdiary/notion/cache.py
+-rwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)     2158 2024-05-01 15:24:12.000000 mmdiary-0.2.0/src/mmdiary/notion/cleanup.py
+-rwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)    15600 2024-05-07 15:35:35.000000 mmdiary-0.2.0/src/mmdiary/notion/uploader.py
+drwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)        0 2024-05-08 00:21:14.006244 mmdiary-0.2.0/src/mmdiary/telegrambot/
+-rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)        0 2024-05-01 14:53:27.000000 mmdiary-0.2.0/src/mmdiary/telegrambot/__init__.py
+-rwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)     7869 2024-05-01 16:58:22.000000 mmdiary-0.2.0/src/mmdiary/telegrambot/telegrambot_service.py
+drwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)        0 2024-05-08 00:21:14.010244 mmdiary-0.2.0/src/mmdiary/transcriber/
+-rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)        0 2024-05-01 14:53:32.000000 mmdiary-0.2.0/src/mmdiary/transcriber/__init__.py
+-rwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)     1011 2024-05-07 14:37:03.000000 mmdiary-0.2.0/src/mmdiary/transcriber/searcher.py
+-rwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)     4112 2024-05-07 21:37:56.000000 mmdiary-0.2.0/src/mmdiary/transcriber/transcriber.py
+-rwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)    10555 2024-05-08 00:00:16.000000 mmdiary-0.2.0/src/mmdiary/transcriber/verifier.py
+drwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)        0 2024-05-08 00:21:14.010244 mmdiary-0.2.0/src/mmdiary/utils/
+-rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)        0 2024-05-01 15:08:11.000000 mmdiary-0.2.0/src/mmdiary/utils/__init__.py
+-rwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)     7050 2024-05-06 23:38:25.000000 mmdiary-0.2.0/src/mmdiary/utils/datelib.py
+-rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)     1947 2024-05-07 22:50:14.000000 mmdiary-0.2.0/src/mmdiary/utils/jsoncache.py
+-rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)     1004 2024-05-01 14:41:54.000000 mmdiary-0.2.0/src/mmdiary/utils/log.py
+-rwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)     5358 2024-05-07 15:40:56.000000 mmdiary-0.2.0/src/mmdiary/utils/medialib.py
+-rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)      368 2024-05-01 17:19:04.000000 mmdiary-0.2.0/src/mmdiary/utils/progressbar.py
+drwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)        0 2024-05-08 00:21:14.010244 mmdiary-0.2.0/src/mmdiary/video/
+-rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)        0 2024-05-01 14:53:43.000000 mmdiary-0.2.0/src/mmdiary/video/__init__.py
+-rwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)     4665 2024-05-08 00:01:19.000000 mmdiary-0.2.0/src/mmdiary/video/processor.py
+-rwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)     8415 2024-05-07 23:11:01.000000 mmdiary-0.2.0/src/mmdiary/video/uploader.py
+drwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)        0 2024-05-08 00:21:14.006244 mmdiary-0.2.0/src/mmdiary.egg-info/
+-rw-r--r--   0 sashacmc  (1000) sashacmc  (1000)    43431 2024-05-08 00:21:13.000000 mmdiary-0.2.0/src/mmdiary.egg-info/PKG-INFO
+-rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)      887 2024-05-08 00:21:13.000000 mmdiary-0.2.0/src/mmdiary.egg-info/SOURCES.txt
+-rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)        1 2024-05-08 00:21:13.000000 mmdiary-0.2.0/src/mmdiary.egg-info/dependency_links.txt
+-rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)      583 2024-05-08 00:21:13.000000 mmdiary-0.2.0/src/mmdiary.egg-info/entry_points.txt
+-rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)      152 2024-05-08 00:21:13.000000 mmdiary-0.2.0/src/mmdiary.egg-info/requires.txt
+-rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)        8 2024-05-08 00:21:13.000000 mmdiary-0.2.0/src/mmdiary.egg-info/top_level.txt
```

### Comparing `mmdiary-0.1.1/LICENSE` & `mmdiary-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mmdiary-0.1.1/PKG-INFO` & `mmdiary-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmdiary
-Version: 0.1.1
+Version: 0.2.0
 Summary: Multimedia Diary Tools
 Author-email: Alexander Bushnev <Alexander@Bushnev.pro>
 Maintainer-email: Alexander Bushnev <Alexander@Bushnev.pro>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `mmdiary-0.1.1/README.md` & `mmdiary-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `mmdiary-0.1.1/pyproject.toml` & `mmdiary-0.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mmdiary"
-version = "0.1.1"
+version = "0.2.0"
 description = "Multimedia Diary Tools"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {file = "LICENSE"}
 keywords = ["audio", "video", "multimedia", "tool", "youtube", "notion", "transcriber", "uploader"]
 
 authors = [
@@ -37,14 +37,15 @@
 	"Programming Language :: Python :: 3.11",
 	"License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
 	"Topic :: Multimedia :: Video",
 	"Topic :: Utilities",
 ]
 
 dependencies = [
+	"pytest",
 	"notion_client",
 	"notion",
 	"progressbar2",
 	"python-telegram-bot",
 	"openai-whisper",
 	"photo_importer",
 	"mixvideoconcat",
@@ -57,14 +58,15 @@
 "Bug Reports" = "https://github.com/sashacmc/mmdiary/issues"
 "Source" = "https://github.com/sashacmc/mmdiary/"
 "Changelog" = "https://github.com/sashacmc/mmdiary/blob/master/CHANGELOG.md"
 
 [project.scripts]
 mmdiary-notion-upload = "mmdiary.notion.uploader:main"
 mmdiary-notion-cleanup = "mmdiary.notion.cleanup:main"
-mmdiary-notion-cachedb = "mmdiary.notion.cachedb:main"
+mmdiary-notion-cache = "mmdiary.notion.cache:main"
 mmdiary-telegrambot = "mmdiary.telegrambot.telegrambot_service:main"
 mmdiary-transcriber-run = "mmdiary.transcriber.transcriber:main"
 mmdiary-transcriber-verify = "mmdiary.transcriber.verifier:main"
 mmdiary-transcriber-search = "mmdiary.transcriber.searcher:main"
 mmdiary-video-concat = "mmdiary.video.processor:main"
 mmdiary-video-upload = "mmdiary.video.uploader:main"
+mmdiary-utils-datelib = "mmdiary.utils.datelib:main"
```

### Comparing `mmdiary-0.1.1/src/mmdiary/notion/cachedb.py` & `mmdiary-0.2.0/src/mmdiary/notion/cache.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,104 +1,76 @@
 #!/usr/bin/python3
 
 import argparse
 import atexit
 import os
-import sqlite3
-import threading
+import pickle
 
 from notion_client import Client
 from notion_client.helpers import iterate_paginated_api
 
-SCHEMA = '''
-CREATE TABLE IF NOT EXISTS existing_pages (
-    "filename" TEXT,
-    "processtime" TEXT,
-    "bid" TEXT
-);
-
-CREATE UNIQUE INDEX IF NOT EXISTS existing_pages_filename ON existing_pages (filename);
-'''
-
-
-class CacheDB:
-    def __init__(self, filename):
-        self.__conn = sqlite3.connect(os.path.expanduser(filename), check_same_thread=False)
-
-        self.__conn.executescript(SCHEMA)
-        self.__lock = threading.RLock()
-        atexit.register(self.commit)
-
-    def __del__(self):
-        self.commit()
-
-    def commit(self):
-        with self.__lock:
-            self.__conn.commit()
-
-    def rollback(self):
-        with self.__lock:
-            self.__conn.rollback()
+
+class Cache:
+    def __init__(self):
+        self.__filename = os.path.expanduser(os.getenv("MMDIARY_NOTION_CACHE"))
+        self.__data = {}
+        self.__load()
+        self.__changed = False
+        atexit.register(self.__save)
+
+    def __load(self):
+        if not os.path.exists(self.__filename):
+            self.__data = {}
+            return
+        with open(self.__filename, "rb") as f:
+            self.__data = pickle.load(f)
+
+    def __save(self):
+        if not self.__changed:
+            return
+        with open(self.__filename, "wb") as f:
+            pickle.dump(self.__data, f)
 
     def list_existing_pages(self):
-        with self.__lock:
-            self.commit()
-            c = self.__conn.cursor()
-            res = c.execute('SELECT filename, bid FROM existing_pages')
-            return res.fetchall()
+        return [(filename, bid) for filename, (processtime, bid) in self.__data.items()]
 
     def clean_existing_pages(self):
-        with self.__lock:
-            self.commit()
-            c = self.__conn.cursor()
-            c.execute('DELETE FROM existing_pages')
-            self.commit()
+        self.__data = {}
+        self.__changed = True
 
     def add_existing_page(self, filename, processtime, bid):
-        with self.__lock:
-            c = self.__conn.cursor()
-            c.execute(
-                'INSERT OR REPLACE \
-                 INTO existing_pages (filename, processtime, bid) \
-                 VALUES (?, ?, ?)',
-                (filename, processtime, bid),
-            )
+        self.__data[filename] = (processtime, bid)
+        self.__changed = True
 
     def check_existing_pages(self, filename):
-        with self.__lock:
-            c = self.__conn.cursor()
-            res = c.execute(
-                'SELECT processtime, bid FROM existing_pages\
-                             WHERE filename=?',
-                (filename,),
-            )
-            return res.fetchone()
+        return self.__data.get(filename)
 
     def remove_from_existing_pages(self, filename):
-        with self.__lock:
-            c = self.__conn.cursor()
-            c.execute('DELETE FROM existing_pages WHERE filename=?', (filename,))
+        if filename in self.__data:
+            del self.__data[filename]
 
     def __get_prop(self, row, name, default=""):
         try:
             rt = row["properties"][name]["rich_text"]
             if len(rt) != 0:
                 return rt[0]["plain_text"]
             return ""
         except IndexError:
             print(f"Property '{name}' not found in {row}")
             return default
 
-    def sync_existing_pages(self, notion_api, database_id):
+    def sync_existing_pages(self, notion_api, database_ids):
         self.clean_existing_pages()
 
-        res = iterate_paginated_api(
-            notion_api.databases.query,
-            database_id=database_id,
-        )
+        res = []
+        for database_id in set(database_ids):
+            res += iterate_paginated_api(
+                notion_api.databases.query,
+                database_id=database_id,
+            )
 
         duplicates = ""
 
         for r in res:
             source = self.__get_prop(r, "source")
             processtime = self.__get_prop(r, "processtime")
             rid = r["id"]
@@ -121,34 +93,31 @@
         choices=[
             'clean',
             'list',
             'remove',
             'sync',
         ],
     )
-    parser.add_argument(
-        '-d',
-        '--database',
-        help='Database file',
-        default=os.getenv("NOTION_CACHE_DB_FILE"),
-    )
     parser.add_argument('-f', '--file', help='File name')
     return parser.parse_args()
 
 
 def main():
     args = args_parse()
-    db = CacheDB(args.database)
+    db = Cache()
 
     if args.action == 'clean':
         db.clean_existing_pages()
     if args.action == 'list':
         for f in db.list_existing_pages():
             print(f)
     elif args.action == 'remove':
         db.remove_from_existing_pages(args.file)
     elif args.action == 'sync':
-        db.sync_existing_pages(Client(auth=os.getenv("NOTION_API_KEY")), os.getenv("NOTION_DB_ID"))
+        db.sync_existing_pages(
+            Client(auth=os.getenv("NOTION_API_KEY")),
+            (os.getenv("NOTION_AUDIO_DB_ID"), os.getenv("NOTION_VIDEO_DB_ID")),
+        )
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `mmdiary-0.1.1/src/mmdiary/notion/cleanup.py` & `mmdiary-0.2.0/src/mmdiary/notion/cleanup.py`

 * *Files identical despite different names*

### Comparing `mmdiary-0.1.1/src/mmdiary/telegrambot/telegrambot_service.py` & `mmdiary-0.2.0/src/mmdiary/telegrambot/telegrambot_service.py`

 * *Files identical despite different names*

### Comparing `mmdiary-0.1.1/src/mmdiary/transcriber/transcriber.py` & `mmdiary-0.2.0/src/mmdiary/transcriber/transcriber.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,28 +12,33 @@
 from mmdiary.utils.medialib import TIME_OUT_FORMAT
 
 from mmdiary.transcriber.verifier import check_text
 
 DESCRIPTION = """
 Transcribes audio/video file(s).
 Result will be saved to json file along with the original file.
+Optional environment variables:
+    MMDIARY_TRANSCRIBE_MODEL - Transcribe model (default: "medium")
+        See details: https://github.com/openai/whisper?tab=readme-ov-file#available-models-and-languages
+    MMDIARY_TRANSCRIBE_LANGUAGE - Transcribe language (default: "ru")
 """
 
 
 class Transcriber:
-    def __init__(self, model):
+    def __init__(self, model, language):
         import whisper
 
         logging.info("Transcriber initialization...")
         self.__model = whisper.load_model(model)
         self.__modelname = "whisper/" + model
+        self.__language = language
         logging.info("Transcriber inited")
 
     def __transcribe(self, file):
-        return self.__model.transcribe(file.name(), language="ru")
+        return self.__model.transcribe(file.name(), language=self.__language)
 
     def __extract_caption(self, text):
         res = ""
         if len(text) != 0:
             res = text[0].upper()
             for ch in text[1:]:
                 res += ch
@@ -63,15 +68,15 @@
             tp = "video"
         else:
             logging.info("Not audio file, skip")
             return
 
         res = self.__transcribe(file)
         text = self.__to_text(res)
-        text = check_text(text)
+        text = check_text(text, self.__language)
 
         cont = {
             "caption": self.__extract_caption(text),
             "text": text,
             "model": self.__modelname,
             "type": tp,
             "source": os.path.split(file.name())[1],
@@ -106,15 +111,18 @@
         lib = medialib.MediaLib(args.inpath)
         fileslist = lib.get_all() if args.update else lib.get_new()
 
     if len(fileslist) == 0:
         return
 
     print("Model loading... ", end='', flush=True)
-    tr = Transcriber("medium")
+    tr = Transcriber(
+        os.getenv("MMDIARY_TRANSCRIBE_MODEL", "medium"),
+        os.getenv("MMDIARY_TRANSCRIBE_LANGUAGE", "ru"),
+    )
     print("done")
 
     pbar = progressbar.start("Transcribe", len(fileslist))
 
     for af in fileslist:
         try:
             tr.process(af)
```

### Comparing `mmdiary-0.1.1/src/mmdiary/transcriber/verifier.py` & `mmdiary-0.2.0/src/mmdiary/transcriber/verifier.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,86 +1,83 @@
 #!/usr/bin/python3
+# pylint: disable=too-many-instance-attributes
 
 import argparse
-import json
 import logging
 import os
+import re
 from datetime import datetime
 
 from notion.client import NotionClient
 
-from mmdiary.utils import log
-from mmdiary.notion import cachedb
-from mmdiary.utils.medialib import JSON_EXT, TIME_OUT_FORMAT
+from mmdiary.utils import medialib, log
+from mmdiary.notion import cache
 
 DESCRIPTION = """
 Verify transcribed file(s).
 Check recognized text/caption for neural network hallucination markers.
 
 If sync option specified the script will addionally check sync with notion:
     local - check local files and remove missed files from notion 
     notion - check notion cache and remove missed local files 
     all - include `local` and `notion`
 
+Optional environment variables:
+    MMDIARY_TRANSCRIBE_LANGUAGE - Transcribe language (default: "ru")
+
 Sync check require following environment variables:
     NOTION_TOKEN - Notion web auth token
-    NOTION_CACHE_DB_FILE - Cachedb file
+    MMDIARY_NOTION_CACHE_FILE - Cache file
 """
 
-HALLUCINATION_TEXTS = [
-    "Игорь Негода",
-    "Валерий Курас",
-    "Редактор субтитров",
-    "Реактор субтитров",
-    "Субтитры субтитров",
-    "Спасибо за субтитры",
-    "Субтитры подготовлены",
-    "Субтитры делал",
-    "Субтитры сделаны",
-    "Благодарю за внимание",
-    "Спасибо за внимание",
-    "Фондю любит тебя",
-    "одпишись на канал",
-    "одпишитесь на канал",
-    "одпишитесь на наш канал",
-    "одписывайтесь на канал",
-    "одписывайтесь на наш канал",
-    "одписывайтесь на мой канал",
-    "одписывайтесь на этот канал",
-    "обро пожаловать в наш канал",
-    "обро пожаловать на наш канал",
-    "обро пожаловать на мой канал",
-    "обро пожаловать на канал",
-    "тавьте лайк",
-    "тавь лайк",
-    "Найдите лайки",
-    "Спасибо за просмотр",
-    "Большое спасибо за просмотр",
-    "Благодарю за просмотр",
-    "И не забудьте поставить лайк",
-    "ФактФронт",
-    "ПОДПИСЫВАЕТСЯ",
-    "ПРОДОЛЖЕНИЕ",
-    "Продолжение в следующей части",
-]
+HALLUCINATION_TEXTS = {
+    "ru": [
+        re.compile("Игорь Негода"),
+        re.compile("Валерий Курас"),
+        re.compile("Фондю любит тебя"),
+        re.compile("ФактФронт"),
+        re.compile("не пропустить новые видео"),
+        re.compile("[Пп]родолжение в следующей части"),
+        re.compile("[Рр]е(д)?актор субтитров"),
+        re.compile("Субтитры субтитров"),
+        re.compile("Спасибо за субтитры"),
+        re.compile("[Сс]убтитры (подготов|делал|сделаны)"),
+        re.compile("[Бб]лагодарю( (тебя|вас|всех))? за (внимание|просмотр)"),
+        re.compile("[Сс]пасибо( (тебе|вам|всем))? за (внимание|просмотр)"),
+        re.compile("[Пп](одписаться|одписывайся|одписывайтесь) на( (мой|наш|этот))? канал"),
+        re.compile("[Пп](одпишись|одпишитесь|одпишите) на( (мой|наш|этот))? канал"),
+        re.compile("[Дд]обро пожаловать (на|в)( (мой|наш|этот))? канал"),
+        re.compile("[Сс]тавь(те)? лайк(и)?"),
+        re.compile("[Жж]ми(те)? лайк(и)?"),
+        re.compile("[Пп]остав(ь|те|ить) лайк(и)?"),
+        re.compile("[Дд](л)?ай(те)? лайк(и)?"),
+        re.compile("Найдите лайки"),
+        # exclude all capitalised except some key words
+        re.compile(r"^(?!.*(?:МУЗЫКА|СМЕХ|КАШЕЛЬ|ПЕСНЯ|ПОЮТ|ПОЕТ|КРИК))[А-Я\s]{4,}$"),
+    ]
+}
 
 RES_OK = 0
 RES_TO_UPDATE = 1
 RES_TO_DELETE = 2
 
 
-def has_hall_text(s):
-    for hall_text in HALLUCINATION_TEXTS:
-        if hall_text in s:
+def has_hall_text(s, language):
+    if language not in HALLUCINATION_TEXTS:
+        return False
+    for hall_text in HALLUCINATION_TEXTS[language]:
+        if hall_text.search(s) is not None:
             logging.debug("Has hall_text: %s", s)
             return True
     return False
 
 
-def clean_wrong_symbols(s):
+def clean_wrong_symbols(s, language):
+    if language != "ru":
+        return s
     res = ''
     for ch in s:
         if (
             ('а' <= ch <= 'я')
             or ('А' <= ch <= 'Я')
             or ch == 'ё'
             or ch == 'Ё'
@@ -98,61 +95,57 @@
         res = ""
 
     if res != s:
         logging.debug("Has incorrect symbols: '%s'->'%s'", s, res)
     return res
 
 
-def check_text(text):
+def check_text(text, language):
     if text == "":
         return text
 
     src = text.split("\n")
     res = []
     for t in src:
-        if not has_hall_text(t):
-            s = clean_wrong_symbols(t)
+        if not has_hall_text(t, language):
+            s = clean_wrong_symbols(t, language)
             if s == "":
                 logging.debug("Has empty string (was '%s')", t)
             else:
                 res.append(s)
     return "\n".join(res)
 
 
 class Verifier:
     def __init__(self, dryrun, force, sync):
         self.__dryrun = dryrun
         self.__force = force
         self.__sync_local = sync in ('all', 'local')
         self.__sync_notion = sync in ('all', 'notion')
-        self.__cache = cachedb.CacheDB(os.getenv("NOTION_CACHE_DB_FILE"))
+        self.__cache = cache.Cache()
         self.__notion = NotionClient(token_v2=os.getenv("NOTION_TOKEN"))
+        self.__language = os.getenv("MMDIARY_TRANSCRIBE_LANGUAGE", "ru")
 
         self.__local_sources = {}
 
         if len(self.__cache.list_existing_pages()) == 0:
             logging.warning("Empty cache")
 
-    def __load_json(self, file):
-        with open(file, "r", encoding="utf-8") as f:
-            return json.load(f)
-
-    def __save_json(self, file, cont):
-        cont["processtime"] = datetime.now().strftime(TIME_OUT_FORMAT)
-        with open(file, "w", encoding="utf-8") as f:
-            json.dump(cont, f, ensure_ascii=False, indent=2)
+    def __save(self, file, cont):
+        cont["processtime"] = datetime.now().strftime(medialib.TIME_OUT_FORMAT)
+        file.update_fields(cont)
 
     def __check_update_data(self, data):
         res = False
-        new_caption = check_text(data["caption"])
+        new_caption = check_text(data["caption"], self.__language)
         if new_caption != data["caption"]:
             res = True
             data["caption"] = new_caption
 
-        new_text = check_text(data["text"])
+        new_text = check_text(data["text"], self.__language)
         if new_text != data["text"]:
             res = True
             data["text"] = new_text
 
         return res
 
     def __check_audio_json(self, data):
@@ -174,17 +167,14 @@
         return RES_OK
 
     def __check_video_json(self, data):
         if self.__check_update_data(data):
             return RES_TO_UPDATE
         return RES_OK
 
-    def __get_source_file(self, in_file, src_file):
-        return os.path.join(os.path.dirname(in_file), src_file)
-
     def __ask_for_delete(self):
         return self.__ask_for("Delete files")
 
     def __ask_for_cleanup(self):
         return self.__ask_for("Cleanup file")
 
     def __ask_for(self, action):
@@ -202,74 +192,73 @@
 
     def __delete_from_notion(self, source, bid):
         self.__cache.remove_from_existing_pages(source)
         block = self.__notion.get_block(bid)
         block.remove()
         logging.info("removed from notion")
 
-    def __delete_from_fs(self, source, file):
-        if os.path.isfile(source):
-            os.unlink(source)
+    def __delete_from_fs(self, file):
+        if os.path.isfile(file.name()):
+            os.unlink(file.name())
         else:
-            logging.warning("File %s don't exists", source)
-        os.unlink(file)
+            logging.warning("File %s don't exists", file.name())
+        os.unlink(file.json_name())
         logging.info("removed from fs")
 
     def process(self, file):
-        data = self.__load_json(file)
-        tp = data["type"]
+        tp = file.type()
         if tp == "audio":
-            return self.__process_audio(file, data)
+            return self.__process_audio(file)
         if tp == "video":
-            return self.__process_video(file, data)
+            return self.__process_video(file)
         logging.warning("Unsupported type: '%s' in file: %s", tp, file)
         return RES_OK
 
-    def __process_audio(self, file, data):
+    def __process_audio(self, file):
+        data = file.json()
         res = True
         uploaded = self.__cache.check_existing_pages(data.get("source", ""))
-        source = self.__get_source_file(file, data.get("source", ""))
         check_res = self.__check_audio_json(data)
         if check_res != RES_OK:
             res = False
-            print(file)
-            print(source)
+            print(file.json_name())
+            print(file.name())
             print("notion:", uploaded)
             if check_res == RES_TO_DELETE and self.__ask_for_delete():
                 if uploaded is not None:
                     self.__delete_from_notion(data["source"], uploaded[1])
-                self.__delete_from_fs(source, file)
+                self.__delete_from_fs(file)
             elif check_res == RES_TO_UPDATE and self.__ask_for_cleanup():
-                self.__save_json(file, data)
+                self.__save(file, data)
                 print("cleaned")
 
             print()
 
         if not self.__sync_notion:
             return res
 
         if uploaded is None:
             print("Deleted from notion:")
-            print(file)
-            print(source)
+            print(file.json_name())
+            print(file.name())
             if self.__ask_for_delete():
-                self.__delete_from_fs(source, file)
+                self.__delete_from_fs(file)
             print()
         return res
 
-    def __process_video(self, file, data):
+    def __process_video(self, file):
+        data = file.json()
         res = True
-        source = self.__get_source_file(file, data.get("source", ""))
         check_res = self.__check_video_json(data)
         if check_res != RES_OK:
             res = False
-            print(file)
-            print(source)
+            print(file.json_name())
+            print(file.name())
             if self.__ask_for_cleanup():
-                self.__save_json(file, data)
+                self.__save(file, data)
                 print("cleaned")
             print()
         return res
 
     def process_list(self, fileslist):
         self.__local_sources = {}
         errors = 0
@@ -286,25 +275,14 @@
             if source not in self.__local_sources:
                 print("Deleted local:")
                 print("notion:", source, bid)
                 if self.__ask_for_delete():
                     self.__delete_from_notion(source, bid)
 
 
-def scan_files(inpath):
-    res = []
-    for root, _, files in os.walk(inpath):
-        for fname in files:
-            if os.path.splitext(fname)[1] == JSON_EXT:
-                res.append(os.path.join(root, fname))
-
-    res.sort()
-    return res
-
-
 def __args_parse():
     parser = argparse.ArgumentParser(
         description=DESCRIPTION, formatter_class=argparse.RawTextHelpFormatter
     )
     parser.add_argument('inpath', nargs="+", help='Input path(s)')
     parser.add_argument(
         '-d', '--dryrun', help='Dry run (just check without any modifications)', action='store_true'
@@ -335,15 +313,16 @@
     logging.getLogger("urllib3").setLevel(logging.ERROR)
 
     vf = Verifier(args.dryrun, args.force, args.sync)
     fileslist = []
     for path in args.inpath:
         print(f"Start: {path}")
         if os.path.isfile(path):
-            fileslist = (path,)
+            fileslist = (medialib.MediaFile(None, path),)
         elif os.path.isdir(path):
-            fileslist = scan_files(path)
+            lib = medialib.MediaLib(path)
+            fileslist = lib.get_processed(should_have_file=False)
         vf.process_list(fileslist)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `mmdiary-0.1.1/src/mmdiary/utils/datelib.py` & `mmdiary-0.2.0/src/mmdiary/utils/datelib.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,223 +1,221 @@
 #!/usr/bin/python3
 
 import argparse
 import logging
 import os
-import sqlite3
 
-from mmdiary.utils import log, medialib
-from mmdiary.utils.medialib import get_date_from_timestring
+from collections import defaultdict
 
-PROCESSED_NONE = 0
-PROCESSED_IN_PROCESS = 1
-PROCESSED_CONVERTED = 2
-PROCESSED_UPLOADED = 3
-
-SCHEMA = '''
-CREATE TABLE IF NOT EXISTS files (
-    "date" TEXT,
-    "filename" TEXT
-);
-
-CREATE UNIQUE INDEX IF NOT EXISTS files_filename ON files (filename);
-
-CREATE TABLE IF NOT EXISTS dates (
-    "date" TEXT,
-    "url" TEXT,
-    "processed" INTEGER
-);
+from mmdiary.utils import log, medialib
 
-CREATE UNIQUE INDEX IF NOT EXISTS dates_date ON dates (date);
-'''
+DESCRIPTION = """
+Diary video dates DB manipulation tool
+Please declare enviromnent variables before use:
+    VIDEO_LIB_ROOTS - List of video library root dirs
+    VIDEO_PROCESSOR_RES_DIR - Video processor result dir
+
+Possible actions:
+    list_dates - Print all dates with starus
+    disable_video - Set a flag for video file to disable concatenneting and uploading,
+                    also mark corresponded date as not processed for future regeneration
+    set_reupload - Mark a video as not uploaded for future reupload
+                   (e.g. if video was deleted on the YouTube)
+"""
+
+STATE_NONE = "none"
+STATE_INPROCESS = "inprocess"
+STATE_CONVERTED = "converted"
+STATE_UPLOADED = "uploaded"
 
 
 class DateLib:
-    def __init__(self, scan_paths=None, db_file=None):
-        if scan_paths is None:
-            scan_paths = list(
-                filter(
-                    None,
-                    os.getenv("VIDEO_LIB_ROOTS").split(":"),
-                ),
-            )
-        if db_file is None:
-            db_file = os.getenv("VIDEO_LIB_DB")
-
-        self.__conn = sqlite3.connect(os.path.expanduser(db_file))
-        self.__conn.executescript(SCHEMA)
-
-        self.__scan_paths = scan_paths
-
-    def __del__(self):
-        self.__conn.commit()
-
-    def check_file(self, filename):
-        c = self.__conn.cursor()
-        res = c.execute(
-            "SELECT date FROM files\
-                         WHERE filename=?",
-            (filename,),
+    def __init__(self):
+        self.__scan_paths = list(
+            filter(
+                None,
+                os.getenv("VIDEO_LIB_ROOTS").split(":"),
+            ),
         )
-        res = res.fetchall()
-        if len(res) == 0:
-            return None
-        return res[0][0]
-
-    def add_file(self, date, filename):
-        logging.debug("Add: %s to %s", filename, date)
-        c = self.__conn.cursor()
-        try:
-            c.execute(
-                "INSERT \
-                 INTO dates (date, processed) \
-                 VALUES (?, ?) \
-                 ON CONFLICT(date) \
-                 DO UPDATE \
-                 SET processed=?",
-                (date, PROCESSED_NONE, PROCESSED_NONE),
-            )
-            c.execute(
-                "INSERT \
-                 INTO files (date, filename) \
-                 VALUES (?, ?)",
-                (date, filename),
-            )
-        except Exception:
-            logging.exception("add_file failed")
+        self.__res_dir = os.getenv("VIDEO_PROCESSOR_RES_DIR")
+        self.__results = None
+        self.__sources = None
+
+    def __load_results(self):
+        res = {}
+        logging.debug("Process results: %s", self.__res_dir)
+        lib = medialib.MediaLib(self.__res_dir)
+        for mf in lib.get_processed(should_have_file=False):
+            res[mf.recorddate()] = mf
+        return res
 
-    def __set_processed(self, date, processed, url):
-        c = self.__conn.cursor()
-        c.execute("begin")
-        try:
-            c = self.__conn.cursor()
-            res = c.execute(
-                "SELECT processed FROM dates \
-                                  WHERE date=? ",
-                (date,),
-            )
-            res = res.fetchall()
-            if len(res) != 1:
-                raise UserWarning(f"checks processed failed: {res}")
-            if res[0][0] == processed:
-                c.execute("rollback")
-                return False
-
-            if url is None:
-                c.execute(
-                    "UPDATE dates \
-                     SET processed=? \
-                     WHERE date=?",
-                    (processed, date),
-                )
-            else:
-                c.execute(
-                    "UPDATE dates \
-                     SET processed=?, url=? \
-                     WHERE date=?",
-                    (processed, url, date),
-                )
-            if c.rowcount != 1:
-                raise UserWarning(f"set processed failed: {c.rowcount}")
-
-            c.execute("commit")
-            return True
-        except Exception:
-            c.execute("rollback")
-            logging.exception("__set_processed failed")
-            raise
+    def __load_sources(self):
+        res = defaultdict(lambda: [])
+        for path in self.__scan_paths:
+            logging.debug("Process sources: %s", path)
+            lib = medialib.MediaLib(path)
+            for mf in lib.get_processed():
+                res[mf.recorddate()].append(mf)
+        return res
+
+    def results(self):
+        if self.__results is None:
+            self.__results = self.__load_results()
+        return self.__results
+
+    def sources(self):
+        if self.__sources is None:
+            self.__sources = self.__load_sources()
+        return self.__sources
+
+    def get_state(self, date):
+        if date in self.results():
+            return self.results()[date].state()
+        return STATE_NONE
 
     def set_not_processed(self, date):
-        return self.__set_processed(date, PROCESSED_NONE, None)
+        self.results()[date].update_fields({"state": STATE_NONE})
 
     def set_in_progress(self, date):
-        return self.__set_processed(date, PROCESSED_IN_PROCESS, None)
-
-    def set_converted(self, date):
-        return self.__set_processed(date, PROCESSED_CONVERTED, None)
+        fields = {"state": STATE_INPROCESS}
+        if date not in self.results():
+            self.results()[date] = medialib.MediaFile(
+                os.path.join(self.__res_dir, date + medialib.MP4_EXT),
+                os.path.join(self.__res_dir, date + medialib.JSON_EXT),
+            )
+            fields["recordtime"] = date
+            fields["type"] = "mergedvideo"
+        self.results()[date].update_fields(fields)
+
+    def set_converted(self, date, fields):
+        new_fields = {}
+        new_fields.update(fields)
+        new_fields["state"] = STATE_CONVERTED
+        self.results()[date].update_fields(new_fields)
 
     def set_uploaded(self, date, url):
-        return self.__set_processed(date, PROCESSED_UPLOADED, url)
-
-    def __get_by_state(self, processed):
-        c = self.__conn.cursor()
-        res = c.execute(
-            "SELECT date, url FROM dates \
-                              WHERE processed=? \
-                              ORDER BY date",
-            (processed,),
-        )
-        return res.fetchall()
+        self.results()[date].update_fields({"state": STATE_UPLOADED, "url": url})
 
     def get_nonprocessed(self):
-        return self.__get_by_state(PROCESSED_NONE)
+        all_dates = set(self.sources().keys())
+        processed_dates = set(self.__get_results_dates_by_state(STATE_NONE))
+        return all_dates - processed_dates
+
+    def __get_results_dates_by_state(self, state):
+        res = []
+        for date, mf in self.results().items():
+            if mf.state() == state:
+                res.append(date)
+        res.sort()
+        return res
 
     def get_converted(self):
-        return self.__get_by_state(PROCESSED_CONVERTED)
+        return self.__get_results_dates_by_state(STATE_CONVERTED)
+
+    def get_uploaded(self):
+        return self.__get_results_dates_by_state(STATE_UPLOADED)
 
     def get_files_by_date(self, date, for_upload=False):
-        c = self.__conn.cursor()
-        res = c.execute(
-            "SELECT filename FROM files \
-                             WHERE date=?",
-            (date,),
-        )
-        afs = [medialib.MediaFile(row[0]) for row in res.fetchall()]
-        afs.sort(key=lambda af: af.json()["recordtime"])
+        mfs = self.sources()[date]
         if for_upload:
-            afs = list(filter(lambda af: af.json().get("upload", True), afs))
-        return afs
-
-    def scan(self):
-        for path in self.__scan_paths:
-            logging.info("Process: %s", path)
-            al = medialib.MediaLib(path)
-            for af in al.get_processed():
-                fname = af.name()
-                if self.check_file(fname) is None:
-                    self.add_file(
-                        get_date_from_timestring(af.json()["recordtime"]),
-                        fname,
-                    )
+            mfs = list(filter(lambda mf: mf.json().get("upload", True), mfs))
+        mfs.sort(key=lambda mf: mf.recordtime())
+        return mfs
+
+    def __find_in_sources(self, subfilename):
+        """
+        Find source file by part of name or by full name
+        If part matched for many files, returns None
+        """
+        res = None
+        for mfs in self.sources().values():
+            for mf in mfs:
+                if subfilename == mf.name():
+                    return mf
+                if subfilename in mf.name():
+                    if res is None:
+                        res = mf
+                    else:
+                        return None
+        return res
 
     def disable_video(self, filename):
-        date = self.check_file(filename)
-        if date is None:
-            logging.warning("File not in DB")
-
-        af = medialib.MediaFile(filename)
-        data = af.json()
-        data["upload"] = False
-        af.save_json(data)
-
-        self.set_not_processed(date)
+        if filename is None:
+            logging.warning("File not specified")
+            return
+        mf = self.__find_in_sources(filename)
+        if mf is None:
+            logging.warning("File not found or matched to many")
+            return
+
+        mf.update_fields({"upload": False})
+
+        self.set_not_processed(mf.recorddate())
+        logging.info("Video file %s disabled", mf.name())
+
+    def list_dates(self, state):
+        if state is None:
+            res = {date: STATE_NONE for date in set(self.sources().keys())}
+            res.update({date: mf.state() for date, mf in self.results().items()})
+            res = list(res.items())
+            res.sort()
+            return res
+
+        if state == STATE_NONE:
+            return [(date, STATE_NONE) for date in self.get_nonprocessed()]
+
+        return [(date, state) for date in self.__get_results_dates_by_state(state)]
+
+    def list_disabled_videos(self):
+        res = []
+        for mfs in self.sources().values():
+            for mf in mfs:
+                if not mf.json().get("upload", True):
+                    res.append(mf.name())
+        res.sort()
+        return res
 
 
 def __args_parse():
-    parser = argparse.ArgumentParser()
+    parser = argparse.ArgumentParser(
+        description=DESCRIPTION, formatter_class=argparse.RawTextHelpFormatter
+    )
     parser.add_argument(
-        '-a',
-        '--action',
-        help='Action',
+        "-a",
+        "--action",
+        help="Action",
         required=True,
         choices=[
-            'scan',
-            'disable_video',
+            "list_dates",
+            "list_disabled_videos",
+            "disable_video",
+            "set_reupload",
         ],
     )
-    parser.add_argument('-f', '--file', help='File name')
+    parser.add_argument("-f", "--file", help="File name (for disable_video)")
+    parser.add_argument("-e", "--date", help="Date (for set_reupload)")
+    parser.add_argument("-s", "--state", help="State for (list_dates)")
     return parser.parse_args()
 
 
 def main():
     args = __args_parse()
     log.init_logger(level=logging.DEBUG)
     lib = DateLib()
 
-    if args.action == 'scan':
-        lib.scan()
-    if args.action == 'disable_video':
+    if args.action == "list_dates":
+        for date, state in lib.list_dates(args.state):
+            print(date, state)
+    elif args.action == "list_disabled_videos":
+        for filename in lib.list_disabled_videos():
+            print(filename)
+    elif args.action == "disable_video":
         lib.disable_video(args.file)
+    elif args.action == "set_reupload":
+        if lib.get_state(args.date) != STATE_UPLOADED:
+            logging.warning("Specified date not yet uploaded: %s", args.date)
+        lib.set_converted(args.date, {})
+    logging.info("Done.")
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `mmdiary-0.1.1/src/mmdiary/utils/log.py` & `mmdiary-0.2.0/src/mmdiary/utils/log.py`

 * *Files identical despite different names*

### Comparing `mmdiary-0.1.1/src/mmdiary/video/processor.py` & `mmdiary-0.2.0/src/mmdiary/video/processor.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,116 +1,141 @@
 #!/usr/bin/python3
+# pylint: disable=too-many-arguments
 
 import argparse
-import json
 import logging
 import os
-import random
 from datetime import datetime
 
 import mixvideoconcat
 
 from mmdiary.utils import log, datelib, progressbar
 from mmdiary.utils.medialib import TIME_OUT_FORMAT
 
 
+DESCRIPTION = """
+Concatente siary videos and generate aggregated JSON file
+Please declare enviromnent variables before use:
+    VIDEO_LIB_ROOTS - List of video library root dirs
+    VIDEO_PROCESSOR_WORK_DIR - Work dir for temp files (can be huge!) 
+    VIDEO_PROCESSOR_RES_DIR - Result dir
+"""
+
+
 class VideoProcessor:
-    def __init__(self, update_existing):
+    def __init__(self, update_existing, json_only):
         self.__update_existing = update_existing
+        self.__json_only = json_only
         self.__work_dir = os.getenv("VIDEO_PROCESSOR_WORK_DIR")
+        if not self.__work_dir:
+            raise UserWarning("VIDEO_PROCESSOR_WORK_DIR not defined")
         os.makedirs(self.__work_dir, exist_ok=True)
         self.__res_dir = os.getenv("VIDEO_PROCESSOR_RES_DIR")
+        if not self.__res_dir:
+            raise UserWarning("VIDEO_PROCESSOR_WORK_DIR not defined")
         os.makedirs(self.__res_dir, exist_ok=True)
 
         self.__lib = datelib.DateLib()
 
-        logging.debug("Update existing (not used): %s", self.__update_existing)
-
-    def __save_json(self, videos_info, processduration, filename):
-        data = {
-            "videos": videos_info,
-            "processduration": processduration,
-            "processtime": datetime.now().strftime(TIME_OUT_FORMAT),
-            "type": "mergedvideo",
-        }
-        with open(filename, "w", encoding="utf-8") as f:
-            json.dump(data, f, ensure_ascii=False, indent=2)
-
     def __process_date(self, date):
         logging.info("Start: %s", date)
+        res_mf = self.__lib.results()[date]
         starttime = datetime.now()
-        afiles = self.__lib.get_files_by_date(date, for_upload=True)
-        fnames = [af.name() for af in afiles]
+        mfiles = self.__lib.get_files_by_date(date, for_upload=True)
+        fnames = [mf.name() for mf in mfiles]
         logging.info("found %i files", len(fnames))
 
-        resfilename = os.path.join(self.__res_dir, f"{date}.mp4")
-        resfilename_json = os.path.join(self.__res_dir, f"{date}.json")
-        fileinfos = mixvideoconcat.concat(fnames, resfilename, self.__work_dir, dry_run=False)
+        if os.path.exists(res_mf.name()) and not self.__json_only:
+            logging.debug("Remove existing result: %s", res_mf.name())
+            os.unlink(res_mf.name())
+
+        fileinfos = mixvideoconcat.concat(
+            fnames, res_mf.name(), self.__work_dir, dry_run=self.__json_only
+        )
 
         videos_info = []
-        for af, info in zip(afiles, fileinfos):
-            af_info = af.load_json()
-            info["caption"] = af_info["caption"].strip()
-            info["text"] = af_info["text"].strip()
-            info["timestamp"] = af.prop().time().strftime(TIME_OUT_FORMAT)
+        for mf, info in zip(mfiles, fileinfos):
+            mf_info = mf.json()
+            info["caption"] = mf_info["caption"].strip()
+            info["text"] = mf_info["text"].strip()
+            info["timestamp"] = mf.prop().time().strftime(TIME_OUT_FORMAT)
             videos_info.append(info)
 
         processduration = (datetime.now() - starttime).total_seconds()
-        self.__save_json(videos_info, processduration, resfilename_json)
 
-        logging.info("Done: %s", date)
+        fields = {
+            "videos": videos_info,
+            "processduration": processduration,
+            "processtime": datetime.now().strftime(TIME_OUT_FORMAT),
+            "source": os.path.split(res_mf.name())[1],
+            "recordtime": date,
+            "type": "mergedvideo",
+        }
+        self.__lib.set_converted(date, fields)
+
+        logging.info("Done: %s: %s", date, res_mf.json_name())
 
     def process_date(self, date):
-        if not self.__lib.set_in_progress(date):
-            logging.warning("date: %s already in progress", date)
-            return
+        if not self.__update_existing and not self.__json_only:
+            if self.__lib.get_state(date) != datelib.STATE_NONE:
+                logging.warning("date: %s already processed, skip", date)
+                return
 
+        self.__lib.set_in_progress(date)
         try:
             self.__process_date(date)
-            self.__lib.set_converted(date)
         except (Exception, KeyboardInterrupt):
             self.__lib.set_not_processed(date)
             raise
 
     def process_all(self):
-        nonprocessed = list(self.__lib.get_nonprocessed())
-        random.shuffle(nonprocessed)
+        toprocess = []
+        if self.__json_only:
+            toprocess = list(self.__lib.get_converted()) + list(self.__lib.get_uploaded())
+        else:
+            toprocess = list(self.__lib.get_nonprocessed())
 
-        pbar = progressbar.start("Process", len(nonprocessed))
-        for date, _ in nonprocessed:
+        pbar = progressbar.start("Process", len(toprocess))
+        for date in toprocess:
             try:
                 self.process_date(date)
             except Exception:
                 logging.exception("Video processing failed")
             pbar.increment()
         pbar.finish()
 
 
 def __args_parse():
-    parser = argparse.ArgumentParser()
-    parser.add_argument("dates", nargs="*", help="Date to process")
+    parser = argparse.ArgumentParser(
+        description=DESCRIPTION, formatter_class=argparse.RawTextHelpFormatter
+    )
+    parser.add_argument(
+        "dates", nargs="*", help="Date to process (otherwise all dates will be processed)"
+    )
     parser.add_argument('-l', '--logfile', help='Log file', default=None)
     parser.add_argument('-u', '--update', help='Update existing', action='store_true')
+    parser.add_argument(
+        '--json-only',
+        help='Only regenerate existing JSONs without video files regeneration',
+        action='store_true',
+    )
     return parser.parse_args()
 
 
 def main():
     args = __args_parse()
     log.init_logger(args.logfile, logging.DEBUG)
     logging.getLogger("py.warnings").setLevel(logging.ERROR)
 
-    vp = VideoProcessor(args.update)
+    vp = VideoProcessor(args.update, args.json_only)
 
     if len(args.dates) == 0:
         vp.process_all()
     else:
         for date in args.dates:
             vp.process_date(date)
 
     logging.info("Processor done.")
 
 
 if __name__ == "__main__":
-    try:
-        main()
-    except Exception:
-        logging.exception("Video processor main failed")
+    main()
```

### Comparing `mmdiary-0.1.1/src/mmdiary/video/uploader.py` & `mmdiary-0.2.0/src/mmdiary/video/uploader.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,33 @@
 #!/usr/bin/python3
 # pylint: disable=import-outside-toplevel,no-member # because of false positive on Resource
 
 import argparse
-import json
 import logging
 import os
 from datetime import datetime
 
 import googleapiclient.discovery
 
 from mmdiary.utils import log, datelib, progressbar
 from mmdiary.utils.medialib import TIME_OUT_FORMAT, split_large_text
 
 YOUTUBE_MAX_DESCRIPTION = 5000
 YOUTUBE_MAX_COMMENT = 5000
 YOUTUBE_URL = "https://www.youtube.com/watch?v="
 
 
+def generate_video_url(video_id):
+    return YOUTUBE_URL + video_id
+
+
+def extract_video_id(video_url):
+    return video_url.split("v=")[1]
+
+
 def get_youtube_credentials(client_secrets, token_file):
     scopes = [
         "https://www.googleapis.com/auth/youtube.upload",
         "https://www.googleapis.com/auth/youtube.force-ssl",
     ]
 
     if os.path.exists(token_file):
@@ -97,18 +104,17 @@
 class VideoUploader:
     def __init__(self):
         self.__res_dir = os.getenv("VIDEO_PROCESSOR_RES_DIR")
         os.makedirs(self.__res_dir, exist_ok=True)
 
         self.__lib = datelib.DateLib()
         self.__credentials = get_youtube_credentials("client_secrets.json", "token.json")
-
-    def __load_json(self, filename):
-        with open(filename, "r", encoding="utf-8") as f:
-            return json.load(f)
+        self.__youtube = googleapiclient.discovery.build(
+            "youtube", "v3", credentials=self.__credentials
+        )
 
     def __gen_time_labels(self, data, text_field, delimiter=" ", skip_empty=False):
         time_labels = []
         for info in data["videos"]:
             time = datetime.strptime(info["timestamp"], TIME_OUT_FORMAT).strftime("%H: %M: %S")
             caption = info[text_field]
             if len(caption) == 0 and skip_empty:
@@ -118,29 +124,26 @@
 
     def __gen_comments(self, data):
         time_labels = self.__gen_time_labels(data, "text", delimiter="\n", skip_empty=True)
         comment_text = generate_description_full(time_labels)
         return split_large_text(comment_text, YOUTUBE_MAX_COMMENT)
 
     def upload_video(self, fname, title, time_labels):
-        youtube = googleapiclient.discovery.build("youtube", "v3", credentials=self.__credentials)
-
-        # Upload video
         request_body = {
             "snippet": {
                 "title": title,
                 "description": generate_description(time_labels),
                 "tags": ["daily"],
             },
             "status": {"privacyStatus": "unlisted"},
         }
 
         try:
             media_file = googleapiclient.http.MediaFileUpload(fname, chunksize=-1, resumable=True)
-            request = youtube.videos().insert(
+            request = self.__youtube.videos().insert(
                 part="snippet,status", body=request_body, media_body=media_file
             )
             logging.debug("Upload started: %s", request_body)
             response = request.execute()
             video_id = response["id"]
             return video_id
         except googleapiclient.errors.ResumableUploadError as ex:
@@ -150,75 +153,83 @@
             if ex.status_code == 400 and ex.error_details[0]["reason"] == "uploadLimitExceeded":
                 logging.error("uploadLimitExceeded")
                 return None
 
             raise
 
     def add_comment(self, video_id, comment_text):
-        youtube = googleapiclient.discovery.build("youtube", "v3", credentials=self.__credentials)
-
-        # Add a comment to the video
-        request = youtube.commentThreads().insert(
+        request = self.__youtube.commentThreads().insert(
             part="snippet",
             body={
                 "snippet": {
                     "videoId": video_id,
                     "topLevelComment": {"snippet": {"textOriginal": comment_text}},
                 }
             },
         )
 
         logging.debug("Comment started")
         response = request.execute()
         logging.debug(response)
 
+    def delete_video(self, video_id):
+        logging.info("Delete: %s", video_id)
+        self.__youtube.videos().delete(id=video_id).execute()
+
     def process_date(self, date):
+        mf = self.__lib.results()[date]
+        data = mf.json()
         logging.info("Upload: %s", date)
 
-        resfilename = os.path.join(self.__res_dir, f"{date}.mp4")
-        if not os.path.exists(resfilename):
-            raise FileNotFoundError(resfilename)
-        resfilename_json = os.path.join(self.__res_dir, f"{date}.json")
-        if not os.path.exists(resfilename_json):
-            raise FileNotFoundError(resfilename_json)
+        if not mf.have_file():
+            raise FileNotFoundError("Source video file not exists")
+        if not mf.have_json():
+            raise FileNotFoundError("Json file not exists")
+
+        if "url" in data:
+            try:
+                self.delete_video(extract_video_id(data["url"]))
+            except Exception:
+                logging.exception("Video deletion failed")
 
-        data = self.__load_json(resfilename_json)
         time_labels = self.__gen_time_labels(data, "caption")
         comments_text = self.__gen_comments(data)
         logging.debug(comments_text)
 
-        video_id = self.upload_video(resfilename, date, time_labels)
+        video_id = self.upload_video(mf.name(), date, time_labels)
         if video_id is None:
             return False
 
         for comment_text in comments_text:
             try:
                 self.add_comment(video_id, comment_text)
             except Exception:
                 logging.exception("Add comment failed")
 
-        url = YOUTUBE_URL + video_id
+        url = generate_video_url(video_id)
         logging.info("Video uploaded: %s", url)
         self.__lib.set_uploaded(date, url)
-
         logging.info("Upload done: %s", date)
         return True
 
     def process_all(self):
         converted = list(self.__lib.get_converted())
 
         pbar = progressbar.start("Upload", len(converted))
-        for date, _ in converted:
+        err_count = 0
+        for date in converted:
             try:
                 if not self.process_date(date):
-                    return
+                    return pbar.value, err_count
             except Exception:
+                err_count += 1
                 logging.exception("Video uploading failed")
+
             pbar.increment()
-        pbar.finish()
+        return pbar.value, err_count
 
 
 def __args_parse():
     parser = argparse.ArgumentParser()
     parser.add_argument("dates", nargs="*", help="Date to process")
     parser.add_argument('-l', '--logfile', help='Log file', default=None)
     return parser.parse_args()
@@ -227,21 +238,24 @@
 def main():
     args = __args_parse()
     log.init_logger(args.logfile, logging.DEBUG)
     logging.getLogger("py.warnings").setLevel(logging.ERROR)
 
     vup = VideoUploader()
 
+    res_count = 0
+    err_count = 0
     if len(args.dates) == 0:
-        vup.process_all()
+        res_count, err_count = vup.process_all()
     else:
         for date in args.dates:
             vup.process_date(date)
+            res_count += 1
 
-    logging.info("Uploader done.")
+    logging.info("Uploader done: %s, errors: %s", res_count, err_count)
 
 
 if __name__ == "__main__":
     try:
         main()
     except Exception:
         logging.exception("Video uploader main failed")
```

### Comparing `mmdiary-0.1.1/src/mmdiary.egg-info/PKG-INFO` & `mmdiary-0.2.0/src/mmdiary.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmdiary
-Version: 0.1.1
+Version: 0.2.0
 Summary: Multimedia Diary Tools
 Author-email: Alexander Bushnev <Alexander@Bushnev.pro>
 Maintainer-email: Alexander Bushnev <Alexander@Bushnev.pro>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `mmdiary-0.1.1/src/mmdiary.egg-info/SOURCES.txt` & `mmdiary-0.2.0/src/mmdiary.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -5,24 +5,25 @@
 src/mmdiary.egg-info/PKG-INFO
 src/mmdiary.egg-info/SOURCES.txt
 src/mmdiary.egg-info/dependency_links.txt
 src/mmdiary.egg-info/entry_points.txt
 src/mmdiary.egg-info/requires.txt
 src/mmdiary.egg-info/top_level.txt
 src/mmdiary/notion/__init__.py
-src/mmdiary/notion/cachedb.py
+src/mmdiary/notion/cache.py
 src/mmdiary/notion/cleanup.py
 src/mmdiary/notion/uploader.py
 src/mmdiary/telegrambot/__init__.py
 src/mmdiary/telegrambot/telegrambot_service.py
 src/mmdiary/transcriber/__init__.py
 src/mmdiary/transcriber/searcher.py
 src/mmdiary/transcriber/transcriber.py
 src/mmdiary/transcriber/verifier.py
 src/mmdiary/utils/__init__.py
 src/mmdiary/utils/datelib.py
+src/mmdiary/utils/jsoncache.py
 src/mmdiary/utils/log.py
 src/mmdiary/utils/medialib.py
 src/mmdiary/utils/progressbar.py
 src/mmdiary/video/__init__.py
 src/mmdiary/video/processor.py
 src/mmdiary/video/uploader.py
```

### Comparing `mmdiary-0.1.1/src/mmdiary.egg-info/entry_points.txt` & `mmdiary-0.2.0/src/mmdiary.egg-info/entry_points.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 [console_scripts]
-mmdiary-notion-cachedb = mmdiary.notion.cachedb:main
+mmdiary-notion-cache = mmdiary.notion.cache:main
 mmdiary-notion-cleanup = mmdiary.notion.cleanup:main
 mmdiary-notion-upload = mmdiary.notion.uploader:main
 mmdiary-telegrambot = mmdiary.telegrambot.telegrambot_service:main
 mmdiary-transcriber-run = mmdiary.transcriber.transcriber:main
 mmdiary-transcriber-search = mmdiary.transcriber.searcher:main
 mmdiary-transcriber-verify = mmdiary.transcriber.verifier:main
+mmdiary-utils-datelib = mmdiary.utils.datelib:main
 mmdiary-video-concat = mmdiary.video.processor:main
 mmdiary-video-upload = mmdiary.video.uploader:main
```

