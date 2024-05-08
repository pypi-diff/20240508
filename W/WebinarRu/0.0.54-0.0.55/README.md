# Comparing `tmp/webinarru-0.0.54.tar.gz` & `tmp/webinarru-0.0.55.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webinarru-0.0.54.tar", max compression
+gzip compressed data, was "webinarru-0.0.55.tar", max compression
```

## Comparing `webinarru-0.0.54.tar` & `webinarru-0.0.55.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      935 2023-09-23 05:40:20.990000 webinarru-0.0.54/README.md
--rw-r--r--   0        0        0       58 2023-09-23 09:37:15.780000 webinarru-0.0.54/WebinarRu/__init__.py
--rw-r--r--   0        0        0     5656 2024-03-22 08:25:55.281533 webinarru-0.0.54/WebinarRu/base_api.py
--rw-r--r--   0        0        0    31561 2024-05-06 09:40:32.544259 webinarru-0.0.54/WebinarRu/models.py
--rw-r--r--   0        0        0    60799 2024-04-08 16:00:36.071910 webinarru-0.0.54/WebinarRu/webinar_api.py
--rw-r--r--   0        0        0      515 2024-05-06 09:55:12.800722 webinarru-0.0.54/pyproject.toml
--rw-r--r--   0        0        0     1454 1970-01-01 00:00:00.000000 webinarru-0.0.54/PKG-INFO
+-rw-r--r--   0        0        0      935 2023-09-23 05:40:20.990000 webinarru-0.0.55/README.md
+-rw-r--r--   0        0        0       58 2023-09-23 09:37:15.780000 webinarru-0.0.55/WebinarRu/__init__.py
+-rw-r--r--   0        0        0     5656 2024-03-22 08:25:55.281533 webinarru-0.0.55/WebinarRu/base_api.py
+-rw-r--r--   0        0        0    31569 2024-05-08 09:21:39.581454 webinarru-0.0.55/WebinarRu/models.py
+-rw-r--r--   0        0        0    60798 2024-05-08 09:37:54.835897 webinarru-0.0.55/WebinarRu/webinar_api.py
+-rw-r--r--   0        0        0      515 2024-05-08 09:39:36.214230 webinarru-0.0.55/pyproject.toml
+-rw-r--r--   0        0        0     1454 1970-01-01 00:00:00.000000 webinarru-0.0.55/PKG-INFO
```

### Comparing `webinarru-0.0.54/README.md` & `webinarru-0.0.55/README.md`

 * *Files identical despite different names*

### Comparing `webinarru-0.0.54/WebinarRu/base_api.py` & `webinarru-0.0.55/WebinarRu/base_api.py`

 * *Files identical despite different names*

### Comparing `webinarru-0.0.54/WebinarRu/models.py` & `webinarru-0.0.55/WebinarRu/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -274,15 +274,15 @@
     thumbnails: Optional[list | dict] = None  # — миниатюры картинок;
     size: Optional[int] = None  # — размер файла в байтах;
     format: Optional[str] = None  # — расширение файла;
     isHidden: Optional[bool] = None  # — доступность файла. В пользовательских сценариях не используется;
     isSystem: Optional[bool] = None  # — принадлежность файла системе. В пользовательских сценариях не используется;
     mimeType: Optional[str] = None  # — MIME тип файла. В пользовательских сценариях не используется;
     typeFile: Optional[
-        Literal['video', 'presentation', 'slide', 'test', 'record', 'ConvertedRecord']
+        Literal['file', 'video', 'presentation', 'slide', 'test', 'record', 'ConvertedRecord']
     ] = None  # — тип файла.
     uri: Optional[str] = None  # — uri файла. В пользовательских сценариях не используется;
     thumbnailUri: Optional[str] = None  # — ссылка на миниатюру картинки. В пользовательских сценариях не используется.
 
     duration: Optional[int | float] = None  # — длительность видео или теста;
     description: Optional[str] = None  # — описание. Для видео Yotube/Vimeo:
     src: Optional[str] = None  # — ссылка на видео;
```

### Comparing `webinarru-0.0.54/WebinarRu/webinar_api.py` & `webinarru-0.0.55/WebinarRu/webinar_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -775,15 +775,15 @@
         :param event_id: Идентификатор мероприятия
         :param file_id: ID файла
         :return: коллекция файлов
         """
         params = {}
         params.update({"fileId": file_id}) if file_id is not None else ...
         files = await self.get_json(f"/events/{event_id}/files", params)
-        # pprint(files)
+        # print(files)
         if files is not None:
             return [File(**file['file']) for file in files]
 
     async def get_event_session_files(
             self,
             event_session_id: int,  # eventsessionsID
             file_id: Optional[int] = None,  # fileId
```

### Comparing `webinarru-0.0.54/pyproject.toml` & `webinarru-0.0.55/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "WebinarRu"
-version = "0.0.54"
+version = "0.0.55"
 description = "Python client for webinar.ru platform"
 authors = ["gulyaeve <gulyaev.e@icloud.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "WebinarRu"}]
 
 [tool.poetry.dependencies]
```

### Comparing `webinarru-0.0.54/PKG-INFO` & `webinarru-0.0.55/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WebinarRu
-Version: 0.0.54
+Version: 0.0.55
 Summary: Python client for webinar.ru platform
 License: MIT
 Author: gulyaeve
 Author-email: gulyaev.e@icloud.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

