# Comparing `tmp/media_parser-2.0.0.tar.gz` & `tmp/media_parser-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "media_parser-2.0.0.tar", max compression
+gzip compressed data, was "media_parser-2.0.1.tar", max compression
```

## Comparing `media_parser-2.0.0.tar` & `media_parser-2.0.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1062 2024-05-08 01:54:48.776787 media_parser-2.0.0/LICENSE
--rw-r--r--   0        0        0     3802 2024-05-08 01:54:48.776787 media_parser-2.0.0/README.md
--rw-r--r--   0        0        0      239 2024-05-08 01:54:48.780787 media_parser-2.0.0/media_parser/__init__.py
--rw-r--r--   0        0        0      258 2024-05-08 01:54:48.780787 media_parser-2.0.0/media_parser/context.py
--rw-r--r--   0        0        0       42 2024-05-08 01:54:48.780787 media_parser-2.0.0/media_parser/database/__init__.py
--rw-r--r--   0        0        0     3249 2024-05-08 01:54:48.780787 media_parser-2.0.0/media_parser/database/base.py
--rw-r--r--   0        0        0      451 2024-05-08 01:54:48.780787 media_parser-2.0.0/media_parser/database/models.py
--rw-r--r--   0        0        0      127 2024-05-08 01:54:48.780787 media_parser-2.0.0/media_parser/models/__init__.py
--rw-r--r--   0        0        0     4859 2024-05-08 01:54:48.780787 media_parser-2.0.0/media_parser/models/medias.py
--rw-r--r--   0        0        0      171 2024-05-08 01:54:48.780787 media_parser-2.0.0/media_parser/parsers/__init__.py
--rw-r--r--   0        0        0     5208 2024-05-08 01:54:48.780787 media_parser-2.0.0/media_parser/parsers/base.py
--rw-r--r--   0        0        0     5824 2024-05-08 01:54:48.780787 media_parser-2.0.0/media_parser/parsers/instagram.py
--rw-r--r--   0        0        0     4195 2024-05-08 01:54:48.780787 media_parser-2.0.0/media_parser/parsers/reddit.py
--rw-r--r--   0        0        0     9815 2024-05-08 01:54:48.780787 media_parser-2.0.0/media_parser/parsers/tiktok.py
--rw-r--r--   0        0        0     3169 2024-05-08 01:54:48.780787 media_parser-2.0.0/media_parser/parsers/twitter.py
--rw-r--r--   0        0        0     3348 2024-05-08 01:54:48.780787 media_parser-2.0.0/media_parser/parsers/youtube.py
--rw-r--r--   0        0        0      862 2024-05-08 01:54:48.780787 media_parser-2.0.0/media_parser/utils.py
--rw-r--r--   0        0        0     2755 2024-05-08 01:54:48.784787 media_parser-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     5338 1970-01-01 00:00:00.000000 media_parser-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1062 2024-05-08 02:02:11.133474 media_parser-2.0.1/LICENSE
+-rw-r--r--   0        0        0     1080 2024-05-08 02:02:11.133474 media_parser-2.0.1/README.md
+-rw-r--r--   0        0        0      239 2024-05-08 02:02:11.133474 media_parser-2.0.1/media_parser/__init__.py
+-rw-r--r--   0        0        0      258 2024-05-08 02:02:11.133474 media_parser-2.0.1/media_parser/context.py
+-rw-r--r--   0        0        0       42 2024-05-08 02:02:11.137474 media_parser-2.0.1/media_parser/database/__init__.py
+-rw-r--r--   0        0        0     3249 2024-05-08 02:02:11.137474 media_parser-2.0.1/media_parser/database/base.py
+-rw-r--r--   0        0        0      451 2024-05-08 02:02:11.137474 media_parser-2.0.1/media_parser/database/models.py
+-rw-r--r--   0        0        0      127 2024-05-08 02:02:11.137474 media_parser-2.0.1/media_parser/models/__init__.py
+-rw-r--r--   0        0        0     4859 2024-05-08 02:02:11.137474 media_parser-2.0.1/media_parser/models/medias.py
+-rw-r--r--   0        0        0      171 2024-05-08 02:02:11.137474 media_parser-2.0.1/media_parser/parsers/__init__.py
+-rw-r--r--   0        0        0     5208 2024-05-08 02:02:11.137474 media_parser-2.0.1/media_parser/parsers/base.py
+-rw-r--r--   0        0        0     5824 2024-05-08 02:02:11.137474 media_parser-2.0.1/media_parser/parsers/instagram.py
+-rw-r--r--   0        0        0     4195 2024-05-08 02:02:11.137474 media_parser-2.0.1/media_parser/parsers/reddit.py
+-rw-r--r--   0        0        0     9815 2024-05-08 02:02:11.137474 media_parser-2.0.1/media_parser/parsers/tiktok.py
+-rw-r--r--   0        0        0     3169 2024-05-08 02:02:11.137474 media_parser-2.0.1/media_parser/parsers/twitter.py
+-rw-r--r--   0        0        0     3348 2024-05-08 02:02:11.137474 media_parser-2.0.1/media_parser/parsers/youtube.py
+-rw-r--r--   0        0        0      862 2024-05-08 02:02:11.137474 media_parser-2.0.1/media_parser/utils.py
+-rw-r--r--   0        0        0     2755 2024-05-08 02:02:11.137474 media_parser-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2616 1970-01-01 00:00:00.000000 media_parser-2.0.1/PKG-INFO
```

### Comparing `media_parser-2.0.0/LICENSE` & `media_parser-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `media_parser-2.0.0/media_parser/database/base.py` & `media_parser-2.0.1/media_parser/database/base.py`

 * *Files identical despite different names*

### Comparing `media_parser-2.0.0/media_parser/models/medias.py` & `media_parser-2.0.1/media_parser/models/medias.py`

 * *Files identical despite different names*

### Comparing `media_parser-2.0.0/media_parser/parsers/base.py` & `media_parser-2.0.1/media_parser/parsers/base.py`

 * *Files identical despite different names*

### Comparing `media_parser-2.0.0/media_parser/parsers/instagram.py` & `media_parser-2.0.1/media_parser/parsers/instagram.py`

 * *Files identical despite different names*

### Comparing `media_parser-2.0.0/media_parser/parsers/reddit.py` & `media_parser-2.0.1/media_parser/parsers/reddit.py`

 * *Files identical despite different names*

### Comparing `media_parser-2.0.0/media_parser/parsers/tiktok.py` & `media_parser-2.0.1/media_parser/parsers/tiktok.py`

 * *Files identical despite different names*

### Comparing `media_parser-2.0.0/media_parser/parsers/twitter.py` & `media_parser-2.0.1/media_parser/parsers/twitter.py`

 * *Files identical despite different names*

### Comparing `media_parser-2.0.0/media_parser/parsers/youtube.py` & `media_parser-2.0.1/media_parser/parsers/youtube.py`

 * *Files identical despite different names*

### Comparing `media_parser-2.0.0/media_parser/utils.py` & `media_parser-2.0.1/media_parser/utils.py`

 * *Files identical despite different names*

### Comparing `media_parser-2.0.0/pyproject.toml` & `media_parser-2.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "media-parser"
-version = "2.0.0"
+version = "2.0.1"
 description = "API for parsing media from social networks"
 authors = ["Jag_k <me@jagk.dev>"]
 maintainers = ["Jag_k <me@jagk.dev>"]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Framework :: FastAPI",
     "Framework :: Pydantic",
```

