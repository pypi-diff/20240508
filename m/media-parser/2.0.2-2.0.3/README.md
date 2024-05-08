# Comparing `tmp/media_parser-2.0.2.tar.gz` & `tmp/media_parser-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "media_parser-2.0.2.tar", max compression
+gzip compressed data, was "media_parser-2.0.3.tar", max compression
```

## Comparing `media_parser-2.0.2.tar` & `media_parser-2.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1062 2024-05-08 02:10:42.871271 media_parser-2.0.2/LICENSE
--rw-r--r--   0        0        0     1080 2024-05-08 02:10:42.871271 media_parser-2.0.2/README.md
--rw-r--r--   0        0        0      239 2024-05-08 02:10:42.875271 media_parser-2.0.2/media_parser/__init__.py
--rw-r--r--   0        0        0      258 2024-05-08 02:10:42.875271 media_parser-2.0.2/media_parser/context.py
--rw-r--r--   0        0        0       42 2024-05-08 02:10:42.875271 media_parser-2.0.2/media_parser/database/__init__.py
--rw-r--r--   0        0        0     3249 2024-05-08 02:10:42.875271 media_parser-2.0.2/media_parser/database/base.py
--rw-r--r--   0        0        0      451 2024-05-08 02:10:42.875271 media_parser-2.0.2/media_parser/database/models.py
--rw-r--r--   0        0        0      127 2024-05-08 02:10:42.875271 media_parser-2.0.2/media_parser/models/__init__.py
--rw-r--r--   0        0        0     4859 2024-05-08 02:10:42.875271 media_parser-2.0.2/media_parser/models/medias.py
--rw-r--r--   0        0        0      171 2024-05-08 02:10:42.875271 media_parser-2.0.2/media_parser/parsers/__init__.py
--rw-r--r--   0        0        0     5208 2024-05-08 02:10:42.875271 media_parser-2.0.2/media_parser/parsers/base.py
--rw-r--r--   0        0        0     5824 2024-05-08 02:10:42.875271 media_parser-2.0.2/media_parser/parsers/instagram.py
--rw-r--r--   0        0        0     4195 2024-05-08 02:10:42.875271 media_parser-2.0.2/media_parser/parsers/reddit.py
--rw-r--r--   0        0        0     9815 2024-05-08 02:10:42.875271 media_parser-2.0.2/media_parser/parsers/tiktok.py
--rw-r--r--   0        0        0     3169 2024-05-08 02:10:42.875271 media_parser-2.0.2/media_parser/parsers/twitter.py
--rw-r--r--   0        0        0     3348 2024-05-08 02:10:42.875271 media_parser-2.0.2/media_parser/parsers/youtube.py
--rw-r--r--   0        0        0      862 2024-05-08 02:10:42.875271 media_parser-2.0.2/media_parser/utils.py
--rw-r--r--   0        0        0     2755 2024-05-08 02:10:42.875271 media_parser-2.0.2/pyproject.toml
--rw-r--r--   0        0        0     2616 1970-01-01 00:00:00.000000 media_parser-2.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1062 2024-05-08 02:14:13.823843 media_parser-2.0.3/LICENSE
+-rw-r--r--   0        0        0      897 2024-05-08 02:14:13.823843 media_parser-2.0.3/README.md
+-rw-r--r--   0        0        0      239 2024-05-08 02:14:13.823843 media_parser-2.0.3/media_parser/__init__.py
+-rw-r--r--   0        0        0      258 2024-05-08 02:14:13.823843 media_parser-2.0.3/media_parser/context.py
+-rw-r--r--   0        0        0       42 2024-05-08 02:14:13.823843 media_parser-2.0.3/media_parser/database/__init__.py
+-rw-r--r--   0        0        0     3249 2024-05-08 02:14:13.823843 media_parser-2.0.3/media_parser/database/base.py
+-rw-r--r--   0        0        0      451 2024-05-08 02:14:13.827843 media_parser-2.0.3/media_parser/database/models.py
+-rw-r--r--   0        0        0      127 2024-05-08 02:14:13.827843 media_parser-2.0.3/media_parser/models/__init__.py
+-rw-r--r--   0        0        0     4859 2024-05-08 02:14:13.827843 media_parser-2.0.3/media_parser/models/medias.py
+-rw-r--r--   0        0        0      171 2024-05-08 02:14:13.827843 media_parser-2.0.3/media_parser/parsers/__init__.py
+-rw-r--r--   0        0        0     5208 2024-05-08 02:14:13.827843 media_parser-2.0.3/media_parser/parsers/base.py
+-rw-r--r--   0        0        0     5824 2024-05-08 02:14:13.827843 media_parser-2.0.3/media_parser/parsers/instagram.py
+-rw-r--r--   0        0        0     4195 2024-05-08 02:14:13.827843 media_parser-2.0.3/media_parser/parsers/reddit.py
+-rw-r--r--   0        0        0     9815 2024-05-08 02:14:13.827843 media_parser-2.0.3/media_parser/parsers/tiktok.py
+-rw-r--r--   0        0        0     3169 2024-05-08 02:14:13.827843 media_parser-2.0.3/media_parser/parsers/twitter.py
+-rw-r--r--   0        0        0     3348 2024-05-08 02:14:13.827843 media_parser-2.0.3/media_parser/parsers/youtube.py
+-rw-r--r--   0        0        0      862 2024-05-08 02:14:13.827843 media_parser-2.0.3/media_parser/utils.py
+-rw-r--r--   0        0        0     2755 2024-05-08 02:14:13.827843 media_parser-2.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2433 1970-01-01 00:00:00.000000 media_parser-2.0.3/PKG-INFO
```

### Comparing `media_parser-2.0.2/LICENSE` & `media_parser-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `media_parser-2.0.2/media_parser/database/base.py` & `media_parser-2.0.3/media_parser/database/base.py`

 * *Files identical despite different names*

### Comparing `media_parser-2.0.2/media_parser/models/medias.py` & `media_parser-2.0.3/media_parser/models/medias.py`

 * *Files identical despite different names*

### Comparing `media_parser-2.0.2/media_parser/parsers/base.py` & `media_parser-2.0.3/media_parser/parsers/base.py`

 * *Files identical despite different names*

### Comparing `media_parser-2.0.2/media_parser/parsers/instagram.py` & `media_parser-2.0.3/media_parser/parsers/instagram.py`

 * *Files identical despite different names*

### Comparing `media_parser-2.0.2/media_parser/parsers/reddit.py` & `media_parser-2.0.3/media_parser/parsers/reddit.py`

 * *Files identical despite different names*

### Comparing `media_parser-2.0.2/media_parser/parsers/tiktok.py` & `media_parser-2.0.3/media_parser/parsers/tiktok.py`

 * *Files identical despite different names*

### Comparing `media_parser-2.0.2/media_parser/parsers/twitter.py` & `media_parser-2.0.3/media_parser/parsers/twitter.py`

 * *Files identical despite different names*

### Comparing `media_parser-2.0.2/media_parser/parsers/youtube.py` & `media_parser-2.0.3/media_parser/parsers/youtube.py`

 * *Files identical despite different names*

### Comparing `media_parser-2.0.2/media_parser/utils.py` & `media_parser-2.0.3/media_parser/utils.py`

 * *Files identical despite different names*

### Comparing `media_parser-2.0.2/pyproject.toml` & `media_parser-2.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "media-parser"
-version = "2.0.2"
+version = "2.0.3"
 description = "API for parsing media from social networks"
 authors = ["Jag_k <me@jagk.dev>"]
 maintainers = ["Jag_k <me@jagk.dev>"]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Framework :: FastAPI",
     "Framework :: Pydantic",
```

### Comparing `media_parser-2.0.2/PKG-INFO` & `media_parser-2.0.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: media-parser
-Version: 2.0.2
+Version: 2.0.3
 Summary: API for parsing media from social networks
 Home-page: https://github.com/jag-k/media-parser#readme
 License: MIT
 Keywords: media-parser,poetry,tiktok,youtube,reddit,twitter
 Author: Jag_k
 Author-email: me@jagk.dev
 Maintainer: Jag_k
@@ -38,15 +38,14 @@
 Project-URL: Repository, https://github.com/jag-k/media-parser
 Description-Content-Type: text/markdown
 
 # Media Parser
 
 [![Poetry](https://img.shields.io/endpoint?url=https://python-poetry.org/badge/v0.json)](https://python-poetry.org/)
 [![Documentation Status](https://readthedocs.org/projects/media-parser/badge/?version=latest)](https://media-parser.readthedocs.io/?badge=latest)
-[![Build Docker image](https://github.com/jag-k/media-parser/actions/workflows/docker-image.yml/badge.svg)](https://github.com/jag-k/media-parser/actions/workflows/docker-image.yml)
 [![PyPI publish](https://github.com/jag-k/media-parser/actions/workflows/pypi-publish.yml/badge.svg)](https://github.com/jag-k/media-parser/actions/workflows/pypi-publish.yml)
 [![PyPI version](https://img.shields.io/pypi/v/media-parser?logo=pypi&label=media-parser)](https://pypi.org/project/media-parsers/)
 
 Server for parse Media by URL.
 
 ## Supported medias
 
@@ -60,12 +59,11 @@
 
 ## Installation
 
 ```bash
 poetry add media-parser  # or pip install media-parser
 ```
 
-
 ## License
 
 [MIT](https://github.com/jag-k/media-parser/blob/main/LICENSE)
```
