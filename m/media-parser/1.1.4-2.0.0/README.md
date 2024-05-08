# Comparing `tmp/media_parser-1.1.4.tar.gz` & `tmp/media_parser-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "media_parser-1.1.4.tar", max compression
+gzip compressed data, was "media_parser-2.0.0.tar", max compression
```

## Comparing `media_parser-1.1.4.tar` & `media_parser-2.0.0.tar`

### file list

```diff
@@ -1,9 +1,19 @@
--rw-r--r--   0        0        0     1062 2023-10-18 22:06:59.227941 media_parser-1.1.4/LICENSE
--rw-r--r--   0        0        0     3802 2023-10-18 22:06:59.227941 media_parser-1.1.4/README.md
--rw-r--r--   0        0        0      275 2023-10-18 22:06:59.227941 media_parser-1.1.4/media_parser/__init__.py
--rw-r--r--   0        0        0     3369 2023-10-18 22:06:59.227941 media_parser-1.1.4/media_parser/client.py
--rw-r--r--   0        0        0      307 2023-10-18 22:06:59.231941 media_parser-1.1.4/media_parser/models/__init__.py
--rw-r--r--   0        0        0     4853 2023-10-18 22:06:59.231941 media_parser-1.1.4/media_parser/models/medias.py
--rw-r--r--   0        0        0     2297 2023-10-18 22:06:59.231941 media_parser-1.1.4/media_parser/models/server.py
--rw-r--r--   0        0        0     3310 2023-10-18 22:06:59.231941 media_parser-1.1.4/pyproject.toml
--rw-r--r--   0        0        0     5747 1970-01-01 00:00:00.000000 media_parser-1.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1062 2024-05-08 01:54:48.776787 media_parser-2.0.0/LICENSE
+-rw-r--r--   0        0        0     3802 2024-05-08 01:54:48.776787 media_parser-2.0.0/README.md
+-rw-r--r--   0        0        0      239 2024-05-08 01:54:48.780787 media_parser-2.0.0/media_parser/__init__.py
+-rw-r--r--   0        0        0      258 2024-05-08 01:54:48.780787 media_parser-2.0.0/media_parser/context.py
+-rw-r--r--   0        0        0       42 2024-05-08 01:54:48.780787 media_parser-2.0.0/media_parser/database/__init__.py
+-rw-r--r--   0        0        0     3249 2024-05-08 01:54:48.780787 media_parser-2.0.0/media_parser/database/base.py
+-rw-r--r--   0        0        0      451 2024-05-08 01:54:48.780787 media_parser-2.0.0/media_parser/database/models.py
+-rw-r--r--   0        0        0      127 2024-05-08 01:54:48.780787 media_parser-2.0.0/media_parser/models/__init__.py
+-rw-r--r--   0        0        0     4859 2024-05-08 01:54:48.780787 media_parser-2.0.0/media_parser/models/medias.py
+-rw-r--r--   0        0        0      171 2024-05-08 01:54:48.780787 media_parser-2.0.0/media_parser/parsers/__init__.py
+-rw-r--r--   0        0        0     5208 2024-05-08 01:54:48.780787 media_parser-2.0.0/media_parser/parsers/base.py
+-rw-r--r--   0        0        0     5824 2024-05-08 01:54:48.780787 media_parser-2.0.0/media_parser/parsers/instagram.py
+-rw-r--r--   0        0        0     4195 2024-05-08 01:54:48.780787 media_parser-2.0.0/media_parser/parsers/reddit.py
+-rw-r--r--   0        0        0     9815 2024-05-08 01:54:48.780787 media_parser-2.0.0/media_parser/parsers/tiktok.py
+-rw-r--r--   0        0        0     3169 2024-05-08 01:54:48.780787 media_parser-2.0.0/media_parser/parsers/twitter.py
+-rw-r--r--   0        0        0     3348 2024-05-08 01:54:48.780787 media_parser-2.0.0/media_parser/parsers/youtube.py
+-rw-r--r--   0        0        0      862 2024-05-08 01:54:48.780787 media_parser-2.0.0/media_parser/utils.py
+-rw-r--r--   0        0        0     2755 2024-05-08 01:54:48.784787 media_parser-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     5338 1970-01-01 00:00:00.000000 media_parser-2.0.0/PKG-INFO
```

### Comparing `media_parser-1.1.4/LICENSE` & `media_parser-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `media_parser-1.1.4/README.md` & `media_parser-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `media_parser-1.1.4/media_parser/models/medias.py` & `media_parser-2.0.0/media_parser/models/medias.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-from enum import Enum
+from enum import StrEnum
 from typing import Self
 
 from pydantic import BaseModel, Field
 
 __all__ = (
     "ParserType",
     "Media",
     "Video",
     "Image",
     "Audio",
     "GroupedMedia",
 )
 
 
-class ParserType(str, Enum):
+class ParserType(StrEnum):
     """
-    BaseParser types. Using for identify parsers and .
+    BaseParser types. Using for identify parsers.
     """
 
     TIKTOK = "TikTok"
     TWITTER = "Twitter"
     YOUTUBE = "YouTube"
     REDDIT = "Reddit"
     INSTAGRAM = "Instagram"
@@ -60,21 +60,21 @@
         return hash(self.original_url)
 
 
 class Video(Media):
     """
     Video media.
 
-    :param max_quality_url: URL to max quality video
-    :info max_quality_url: If max quality video is not available, max_quality_url is equal to url
-    :param audio_url: URL to audio from video
+    :param max_quality_url: URL to max quality video.
+    :info max_quality_url: If max quality video is not available, max_quality_url is equal to url.
+    :param audio_url: URL to audio from video.
     :info audio_url: Is it necessary?
-    :param height: Height of video
-    :param width: Width of video
-    :param duration: Duration of video
+    :param height: Height of video.
+    :param width: Width of video.
+    :param duration: Duration of video.
     """
 
     max_quality_url: str | None = None
     audio_url: str | None = None  # Is it necessary?
     mime_type: str = "video/mp4"
 
     height: int | None = None
@@ -85,18 +85,18 @@
         return bool(self.url)
 
 
 class Image(Media):
     """
     Image media.
 
-    :param max_quality_url: URL to max quality image
-    :info max_quality_url: If max quality image is not available, max_quality_url is equal to url
-    :param height: Height of image
-    :param width: Width of image
+    :param max_quality_url: URL to max quality image.
+    :info max_quality_url: If max quality image is not available, max_quality_url is equal to url.
+    :param height: Height of image.
+    :param width: Width of image.
     """
 
     max_quality_url: str | None = None
     mime_type: str = "image/jpeg"
     height: int | None = None
     width: int | None = None
 
@@ -107,15 +107,15 @@
         return bool(self.url)
 
 
 class Audio(Media):
     """
     Audio media.
 
-    :param mime_type: MIME type of audio
+    :param mime_type: MIME type of audio.
     """
 
     mime_type: str = "audio/mpeg"
 
     def __bool__(self) -> bool:
         """
         Return True if Audio has url.
@@ -127,18 +127,18 @@
     audios: list[Audio] = Field(default_factory=list)
     images: list[Image] = Field(default_factory=list)
     videos: list[Video] = Field(default_factory=list)
 
     @classmethod
     def from_medias(cls, medias: list[Media]) -> Self:
         """
-        Generate GroupedMedia from list of Media.
+        Generate GroupedMedia from a list of Media.
 
-        :param medias: list of Media
-        :return: GroupedMedia
+        :param medias: List of Media.
+        :return: Grouped Media.
         """
 
         return cls(
             audios=[m for m in medias if isinstance(m, Audio)],
             images=[m for m in medias if isinstance(m, Image)],
             videos=[m for m in medias if isinstance(m, Video)],
         )
@@ -148,41 +148,41 @@
         Return True if GroupedMedia has any medias.
         """
 
         return bool(self.audios or self.images or self.videos)
 
     def flat(self) -> list[Media]:
         """
-        Makes list of Media from GroupedMedia.
+        Makes a list of Media from GroupedMedia.
         """
 
         return self.audios + self.images + self.videos
 
     def __len__(self) -> int:
         """
         Return count of all medias.
         """
-        return len(self.audios + self.images + self.videos)
+        return len(self.audios) + len(self.images) + len(self.videos)
 
     def __add__(self, other: Self) -> Self:
         """
         Concatenate two GroupedMedia.
 
-        :param other: GroupedMedia
-        :return: GroupedMedia
+        :param other: GroupedMedia.
+        :return: GroupedMedia.
         """
 
         return GroupedMedia(
             audios=self.audios + other.audios,
             images=self.images + other.images,
             videos=self.videos + other.videos,
         )
 
     @classmethod
-    def merge(cls, *grouped_medias: "GroupedMedia") -> "GroupedMedia":
+    def merge(cls, *grouped_medias: Self) -> Self:
         return GroupedMedia(
             audios=[audio for groups in grouped_medias for audio in groups.audios],
             images=[image for groups in grouped_medias for image in groups.images],
             videos=[video for groups in grouped_medias for video in groups.videos],
         )
```

### Comparing `media_parser-1.1.4/pyproject.toml` & `media_parser-2.0.0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "media-parser"
-version = "1.1.4"
+version = "2.0.0"
 description = "API for parsing media from social networks"
 authors = ["Jag_k <me@jagk.dev>"]
 maintainers = ["Jag_k <me@jagk.dev>"]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Framework :: FastAPI",
     "Framework :: Pydantic",
@@ -22,44 +22,36 @@
 homepage = "https://github.com/jag-k/media-parser#readme"
 repository = "https://github.com/jag-k/media-parser"
 documentation = "https://media-parser.rtfd.io"
 readme = "README.md"
 license = "MIT"
 keywords = ["media-parser", "poetry", "tiktok", "youtube", "reddit", "twitter"]
 packages = [
-    { include = "media_parser/client.py" },
-    { include = "media_parser/models" },
-    { include = "media_parser/__init__.py" },
+    {include = "media_parser"}
 ]
 
 [tool.poetry.dependencies]
-python = "^3.11"
-fastapi = "^0.104.0"
-aiohttp = "^3.8.6"
-sentry-sdk = { version = "^1.32.0", extras = ["fastapi", "httpx", "pure_eval", "pymongo"] }
+python = "^3.12"
+aiohttp = "^3.9.5"
 contextvars = "^2.4"
-pydantic = { version = "^1.10.9", extras = ["dotenv"] }
+pydantic = "^2"
 jsonref = "^1.1.0"
 pytube = "^15.0.0"
-uvicorn = "^0.23.1"
 motor = "^3.3.1"
 async-lru = "^2.0.2"
 pyyaml = "^6.0.1"
+httpx = "^0.27.0"
+pydantic-settings = "^2.2.1"
 
-[tool.poetry.extras]
-server = ["uvicorn", "motor", "fastapi", "contextvars", "pytube", "jsonref", "async-lru"]
-sentry = ["sentry-sdk"]
-all = ["uvicorn", "motor", "fastapi", "contextvars", "pytube", "jsonref", "async-lru", "sentry-sdk"]
 
 [tool.poetry.group.dev.dependencies]
-ruff = "^0.1.0"
-pre-commit = "^3.3.2"
+ruff = "*"
+pre-commit = "*"
 motor-types = "^1.0.0b2"
-black = { version = "^23.7.0", extras = ["d"] }
-ruff-lsp = "^0.0.41"
+ruff-lsp = "*"
 
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 sphinx = "7.1.1"
@@ -67,36 +59,29 @@
 sphinxext-opengraph = "^0.8.2"
 sphinx-copybutton = "^0.5.2"
 sphinx-inline-tabs = "^2023.4.21"
 myst-parser = "^2.0.0"
 #sphinxcontrib-openapi = {git = "https://github.com/david-i-berry/sphinxcontrib-openapi.git"}
 #swagger-plugin-for-sphinx = "^3.2.0"
 #sphinxcontrib-redoc = "^1.6.0"
+#sphinx-autodoc2 = {git = "https://github.com/jag-k/sphinx-autodoc2.git"}
+#astroid = "2.15.8"  # sphinx-autodoc2 deps
 sphinx-autodoc2 = {git = "https://github.com/jag-k/sphinx-autodoc2.git"}
-astroid = "2.15.8"  # sphinx-autodoc2 deps
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
-[tool.black]
-line-length = 120
-include = '\.pyi?$'
-exclude = '''
-/(
-    \.git
-  | \.pytest_cache
-  | \.mypy_cache
-  | config
-)/
-'''
 
 [tool.ruff]
 line-length = 120
-target-version = "py311"
+target-version = "py312"
+src = ["media_parser"]
+
+[tool.ruff.lint]
 select = [
     "E", # pyflakes
     "F", # pycodestyle errors
     "W", # pycodestyle warnings
     "UP", # pyupgrade
     "I", # isort
     "C4", # flake8-comprehensions
@@ -104,16 +89,15 @@
     "ASYNC", # flake8-async
     "S", # flake8-bandit
     "INT", # flake8-gettext
     "PTH", # flake8-use-pathlib
     "FLY", # flynt
     "RUF", # ruff-specific rules
 ]
-src = ["media_parser"]
 
-[tool.ruff.flake8-quotes]
+[tool.ruff.lint.flake8-quotes]
 docstring-quotes = "double"
 
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint.per-file-ignores]
 "__init__.py" = ["E402", "F401", "F403", "F405", "F811", "N999"]
 "__main__.py" = ["E402", "F401", "F403", "F405", "F811", "N999"]
 "docs/conf.py" = ["E402"]
```

### Comparing `media_parser-1.1.4/PKG-INFO` & `media_parser-2.0.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,46 +1,43 @@
 Metadata-Version: 2.1
 Name: media-parser
-Version: 1.1.4
+Version: 2.0.0
 Summary: API for parsing media from social networks
 Home-page: https://github.com/jag-k/media-parser#readme
 License: MIT
 Keywords: media-parser,poetry,tiktok,youtube,reddit,twitter
 Author: Jag_k
 Author-email: me@jagk.dev
 Maintainer: Jag_k
 Maintainer-email: me@jagk.dev
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.12,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: FastAPI
 Classifier: Framework :: Pydantic
 Classifier: Framework :: Pydantic :: 1
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Natural Language :: Russian
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
-Provides-Extra: all
-Provides-Extra: sentry
-Provides-Extra: server
-Requires-Dist: aiohttp (>=3.8.6,<4.0.0)
-Requires-Dist: async-lru (>=2.0.2,<3.0.0) ; extra == "server" or extra == "all"
-Requires-Dist: contextvars (>=2.4,<3.0) ; extra == "server" or extra == "all"
-Requires-Dist: fastapi (>=0.104.0,<0.105.0) ; extra == "server" or extra == "all"
-Requires-Dist: jsonref (>=1.1.0,<2.0.0) ; extra == "server" or extra == "all"
-Requires-Dist: motor (>=3.3.1,<4.0.0) ; extra == "server" or extra == "all"
-Requires-Dist: pydantic[dotenv] (>=1.10.9,<2.0.0)
-Requires-Dist: pytube (>=15.0.0,<16.0.0) ; extra == "server" or extra == "all"
+Requires-Dist: aiohttp (>=3.9.5,<4.0.0)
+Requires-Dist: async-lru (>=2.0.2,<3.0.0)
+Requires-Dist: contextvars (>=2.4,<3.0)
+Requires-Dist: httpx (>=0.27.0,<0.28.0)
+Requires-Dist: jsonref (>=1.1.0,<2.0.0)
+Requires-Dist: motor (>=3.3.1,<4.0.0)
+Requires-Dist: pydantic (>=2,<3)
+Requires-Dist: pydantic-settings (>=2.2.1,<3.0.0)
+Requires-Dist: pytube (>=15.0.0,<16.0.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
-Requires-Dist: sentry-sdk[fastapi,httpx,pure-eval,pymongo] (>=1.32.0,<2.0.0) ; extra == "sentry" or extra == "all"
-Requires-Dist: uvicorn (>=0.23.1,<0.24.0) ; extra == "server" or extra == "all"
 Project-URL: Documentation, https://media-parser.rtfd.io
 Project-URL: Repository, https://github.com/jag-k/media-parser
 Description-Content-Type: text/markdown
 
 # Media Parser
 
 [![Poetry](https://img.shields.io/endpoint?url=https://python-poetry.org/badge/v0.json)](https://python-poetry.org/)
```

