# Comparing `tmp/opencf-0.3.1.tar.gz` & `tmp/opencf-0.3.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opencf-0.3.1.tar", max compression
+gzip compressed data, was "opencf-0.3.1a0.tar", max compression
```

## Comparing `opencf-0.3.1.tar` & `opencf-0.3.1a0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     5030 2024-04-22 22:29:52.576924 opencf-0.3.1/README.md
--rw-r--r--   0        0        0       29 2024-04-29 11:56:13.924976 opencf-0.3.1/opencf/__init__.py
--rw-r--r--   0        0        0     2026 2024-04-29 11:29:55.833368 opencf-0.3.1/opencf/app.py
--rw-r--r--   0        0        0      671 2024-04-29 10:24:31.696290 opencf-0.3.1/opencf/converters/__init__.py
--rw-r--r--   0        0        0     7058 2024-05-08 09:50:24.453227 opencf-0.3.1/opencf/converters/document.py
--rw-r--r--   0        0        0        0 2024-04-22 22:28:19.435526 opencf-0.3.1/opencf/converters/image.py
--rw-r--r--   0        0        0     1027 2024-05-08 09:50:24.453227 opencf-0.3.1/opencf/converters/markup.py
--rw-r--r--   0        0        0     2877 2024-05-08 09:50:24.453227 opencf-0.3.1/opencf/converters/structured.py
--rw-r--r--   0        0        0     3162 2024-05-08 09:50:24.453227 opencf-0.3.1/opencf/converters/video.py
--rw-r--r--   0        0        0      419 2024-04-29 11:55:19.000013 opencf-0.3.1/opencf/import_script.py
--rw-r--r--   0        0        0      347 2024-04-22 22:28:19.439526 opencf-0.3.1/opencf/io_handlers/__init__.py
--rw-r--r--   0        0        0     2124 2024-04-22 22:42:11.740523 opencf-0.3.1/opencf/io_handlers/img_opencv.py
--rw-r--r--   0        0        0     2311 2024-04-22 22:42:11.744523 opencf-0.3.1/opencf/io_handlers/img_pillow.py
--rw-r--r--   0        0        0     2444 2024-04-22 22:42:11.740523 opencf-0.3.1/opencf/io_handlers/pdf.py
--rw-r--r--   0        0        0     2344 2024-04-22 22:42:11.740523 opencf-0.3.1/opencf/io_handlers/spreadsheet.py
--rw-r--r--   0        0        0     5596 2024-04-22 23:19:10.399407 opencf-0.3.1/opencf/io_handlers/video.py
--rw-r--r--   0        0        0     3620 2024-04-22 22:28:19.439526 opencf-0.3.1/opencf/utils/image_to_video.py
--rw-r--r--   0        0        0     1886 2024-05-08 09:51:35.522403 opencf-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     6703 1970-01-01 00:00:00.000000 opencf-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     5030 2024-04-22 22:29:52.576924 opencf-0.3.1a0/README.md
+-rw-r--r--   0        0        0       29 2024-04-29 11:56:13.924976 opencf-0.3.1a0/opencf/__init__.py
+-rw-r--r--   0        0        0     2026 2024-04-29 11:29:55.833368 opencf-0.3.1a0/opencf/app.py
+-rw-r--r--   0        0        0      671 2024-04-29 10:24:31.696290 opencf-0.3.1a0/opencf/converters/__init__.py
+-rw-r--r--   0        0        0     7058 2024-04-29 11:16:57.206075 opencf-0.3.1a0/opencf/converters/document.py
+-rw-r--r--   0        0        0        0 2024-04-22 22:28:19.435526 opencf-0.3.1a0/opencf/converters/image.py
+-rw-r--r--   0        0        0     1027 2024-04-22 22:42:11.744523 opencf-0.3.1a0/opencf/converters/markup.py
+-rw-r--r--   0        0        0     2877 2024-04-22 22:42:11.748523 opencf-0.3.1a0/opencf/converters/structured.py
+-rw-r--r--   0        0        0     3162 2024-04-22 23:19:10.399407 opencf-0.3.1a0/opencf/converters/video.py
+-rw-r--r--   0        0        0      419 2024-04-29 11:55:19.000013 opencf-0.3.1a0/opencf/import_script.py
+-rw-r--r--   0        0        0      347 2024-04-22 22:28:19.439526 opencf-0.3.1a0/opencf/io_handlers/__init__.py
+-rw-r--r--   0        0        0     2124 2024-04-22 22:42:11.740523 opencf-0.3.1a0/opencf/io_handlers/img_opencv.py
+-rw-r--r--   0        0        0     2311 2024-04-22 22:42:11.744523 opencf-0.3.1a0/opencf/io_handlers/img_pillow.py
+-rw-r--r--   0        0        0     2444 2024-04-22 22:42:11.740523 opencf-0.3.1a0/opencf/io_handlers/pdf.py
+-rw-r--r--   0        0        0     2344 2024-04-22 22:42:11.740523 opencf-0.3.1a0/opencf/io_handlers/spreadsheet.py
+-rw-r--r--   0        0        0     5596 2024-04-22 23:19:10.399407 opencf-0.3.1a0/opencf/io_handlers/video.py
+-rw-r--r--   0        0        0     3620 2024-04-22 22:28:19.439526 opencf-0.3.1a0/opencf/utils/image_to_video.py
+-rw-r--r--   0        0        0     1888 2024-04-30 14:37:40.978845 opencf-0.3.1a0/pyproject.toml
+-rw-r--r--   0        0        0     6705 1970-01-01 00:00:00.000000 opencf-0.3.1a0/PKG-INFO
```

### Comparing `opencf-0.3.1/README.md` & `opencf-0.3.1a0/README.md`

 * *Files identical despite different names*

### Comparing `opencf-0.3.1/opencf/app.py` & `opencf-0.3.1a0/opencf/app.py`

 * *Files identical despite different names*

### Comparing `opencf-0.3.1/opencf/converters/__init__.py` & `opencf-0.3.1a0/opencf/converters/__init__.py`

 * *Files identical despite different names*

### Comparing `opencf-0.3.1/opencf/converters/document.py` & `opencf-0.3.1a0/opencf/converters/document.py`

 * *Files identical despite different names*

### Comparing `opencf-0.3.1/opencf/converters/markup.py` & `opencf-0.3.1a0/opencf/converters/markup.py`

 * *Files identical despite different names*

### Comparing `opencf-0.3.1/opencf/converters/structured.py` & `opencf-0.3.1a0/opencf/converters/structured.py`

 * *Files identical despite different names*

### Comparing `opencf-0.3.1/opencf/converters/video.py` & `opencf-0.3.1a0/opencf/converters/video.py`

 * *Files identical despite different names*

### Comparing `opencf-0.3.1/opencf/io_handlers/img_opencv.py` & `opencf-0.3.1a0/opencf/io_handlers/img_opencv.py`

 * *Files identical despite different names*

### Comparing `opencf-0.3.1/opencf/io_handlers/img_pillow.py` & `opencf-0.3.1a0/opencf/io_handlers/img_pillow.py`

 * *Files identical despite different names*

### Comparing `opencf-0.3.1/opencf/io_handlers/pdf.py` & `opencf-0.3.1a0/opencf/io_handlers/pdf.py`

 * *Files identical despite different names*

### Comparing `opencf-0.3.1/opencf/io_handlers/spreadsheet.py` & `opencf-0.3.1a0/opencf/io_handlers/spreadsheet.py`

 * *Files identical despite different names*

### Comparing `opencf-0.3.1/opencf/io_handlers/video.py` & `opencf-0.3.1a0/opencf/io_handlers/video.py`

 * *Files identical despite different names*

### Comparing `opencf-0.3.1/opencf/utils/image_to_video.py` & `opencf-0.3.1a0/opencf/utils/image_to_video.py`

 * *Files identical despite different names*

### Comparing `opencf-0.3.1/pyproject.toml` & `opencf-0.3.1a0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "opencf"
 packages = [
     {include = "opencf"}
 ]
-version = "0.3.1"
+version = "0.3.1a0"
 description = "A collection of Python scripts for file conversion tasks, built on top of the opencf-core framework."
 authors = ["Hermann Agossou <agossouhermann7@gmail.com>"]
 readme = "README.md"
 maintainers = [
     "Hermann Agossou <agossouhermann7@gmail.com>"
 ]
 license = "MIT"
```

### Comparing `opencf-0.3.1/PKG-INFO` & `opencf-0.3.1a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opencf
-Version: 0.3.1
+Version: 0.3.1a0
 Summary: A collection of Python scripts for file conversion tasks, built on top of the opencf-core framework.
 Home-page: https://github.com/Hermann-web/opencf
 License: MIT
 Keywords: file conversion,data processing,file formats
 Author: Hermann Agossou
 Author-email: agossouhermann7@gmail.com
 Maintainer: Hermann Agossou
```

