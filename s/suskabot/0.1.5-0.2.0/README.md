# Comparing `tmp/suskabot-0.1.5.tar.gz` & `tmp/suskabot-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "suskabot-0.1.5.tar", max compression
+gzip compressed data, was "suskabot-0.2.0.tar", max compression
```

## Comparing `suskabot-0.1.5.tar` & `suskabot-0.2.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1072 2024-05-07 22:15:25.148151 suskabot-0.1.5/LICENSE
--rw-r--r--   0        0        0     1764 2024-05-07 22:15:25.148151 suskabot-0.1.5/README.md
--rw-r--r--   0        0        0      779 2024-05-07 22:15:25.155151 suskabot-0.1.5/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-07 22:15:25.181151 suskabot-0.1.5/suskabot/__init__.py
--rw-r--r--   0        0        0      862 2024-05-07 22:15:25.155151 suskabot-0.1.5/suskabot/__main__.py
--rw-r--r--   0        0        0        0 2024-05-07 22:15:25.181151 suskabot-0.1.5/suskabot/app/__init__.py
--rw-r--r--   0        0        0     1529 2024-05-07 22:15:25.155151 suskabot-0.1.5/suskabot/app/app.py
--rw-r--r--   0        0        0      295 2024-05-07 22:15:25.155151 suskabot-0.1.5/suskabot/config/.env.example
--rw-r--r--   0        0        0        4 2024-05-07 22:15:25.156151 suskabot-0.1.5/suskabot/config/.gitignore
--rw-r--r--   0        0        0        0 2024-05-07 22:15:25.181151 suskabot-0.1.5/suskabot/config/__init__.py
--rw-r--r--   0        0        0     4658 2024-05-07 22:15:25.156151 suskabot-0.1.5/suskabot/config/config.py
--rw-r--r--   0        0        0        0 2024-05-07 22:15:25.181151 suskabot-0.1.5/suskabot/controllers/__init__.py
--rw-r--r--   0        0        0        0 2024-05-07 22:15:25.181151 suskabot-0.1.5/suskabot/controllers/telegram_api/__init__.py
--rw-r--r--   0        0        0     1494 2024-05-07 22:15:25.156151 suskabot-0.1.5/suskabot/controllers/telegram_api/bot.py
--rw-r--r--   0        0        0        0 2024-05-07 22:15:25.181151 suskabot-0.1.5/suskabot/controllers/telegram_api/handlers/__init__.py
--rw-r--r--   0        0        0     1339 2024-05-07 22:15:25.156151 suskabot-0.1.5/suskabot/controllers/telegram_api/handlers/app.py
--rw-r--r--   0        0        0     1783 2024-05-07 22:15:25.156151 suskabot-0.1.5/suskabot/controllers/telegram_api/handlers/translator.py
--rw-r--r--   0        0        0     5917 2024-05-07 22:15:25.156151 suskabot-0.1.5/suskabot/controllers/telegram_api/handlers/youtube_downloader.py
--rw-r--r--   0        0        0        0 2024-05-07 22:15:25.181151 suskabot-0.1.5/suskabot/services/__init__.py
--rw-r--r--   0        0        0     4050 2024-05-07 22:15:25.156151 suskabot-0.1.5/suskabot/services/translator.py
--rw-r--r--   0        0        0     4908 2024-05-07 22:15:25.156151 suskabot-0.1.5/suskabot/services/youtube_downloader.py
--rw-r--r--   0        0        0        0 2024-05-07 22:15:25.181151 suskabot-0.1.5/suskabot/utils/__init__.py
--rw-r--r--   0        0        0      861 2024-05-07 22:15:25.156151 suskabot-0.1.5/suskabot/utils/utils.py
--rw-r--r--   0        0        0     2481 1970-01-01 00:00:00.000000 suskabot-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-08 00:36:47.241516 suskabot-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1706 2024-05-08 00:36:47.241516 suskabot-0.2.0/README.md
+-rw-r--r--   0        0        0      779 2024-05-08 00:36:47.248516 suskabot-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-08 00:36:47.277516 suskabot-0.2.0/suskabot/__init__.py
+-rw-r--r--   0        0        0      914 2024-05-08 00:36:47.248516 suskabot-0.2.0/suskabot/__main__.py
+-rw-r--r--   0        0        0        0 2024-05-08 00:36:47.277516 suskabot-0.2.0/suskabot/app/__init__.py
+-rw-r--r--   0        0        0     1529 2024-05-08 00:36:47.248516 suskabot-0.2.0/suskabot/app/app.py
+-rw-r--r--   0        0        0      295 2024-05-08 00:36:47.248516 suskabot-0.2.0/suskabot/config/.env.example
+-rw-r--r--   0        0        0        4 2024-05-08 00:36:47.248516 suskabot-0.2.0/suskabot/config/.gitignore
+-rw-r--r--   0        0        0        0 2024-05-08 00:36:47.277516 suskabot-0.2.0/suskabot/config/__init__.py
+-rw-r--r--   0        0        0     4915 2024-05-08 00:36:47.248516 suskabot-0.2.0/suskabot/config/config.py
+-rw-r--r--   0        0        0        0 2024-05-08 00:36:47.277516 suskabot-0.2.0/suskabot/controllers/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-08 00:36:47.277516 suskabot-0.2.0/suskabot/controllers/telegram_api/__init__.py
+-rw-r--r--   0        0        0     1494 2024-05-08 00:36:47.248516 suskabot-0.2.0/suskabot/controllers/telegram_api/bot.py
+-rw-r--r--   0        0        0        0 2024-05-08 00:36:47.277516 suskabot-0.2.0/suskabot/controllers/telegram_api/handlers/__init__.py
+-rw-r--r--   0        0        0     1339 2024-05-08 00:36:47.248516 suskabot-0.2.0/suskabot/controllers/telegram_api/handlers/app.py
+-rw-r--r--   0        0        0     1783 2024-05-08 00:36:47.248516 suskabot-0.2.0/suskabot/controllers/telegram_api/handlers/translator.py
+-rw-r--r--   0        0        0     5917 2024-05-08 00:36:47.249516 suskabot-0.2.0/suskabot/controllers/telegram_api/handlers/youtube_downloader.py
+-rw-r--r--   0        0        0        0 2024-05-08 00:36:47.277516 suskabot-0.2.0/suskabot/services/__init__.py
+-rw-r--r--   0        0        0     4158 2024-05-08 00:36:47.249516 suskabot-0.2.0/suskabot/services/translator.py
+-rw-r--r--   0        0        0     5948 2024-05-08 00:36:47.249516 suskabot-0.2.0/suskabot/services/youtube_downloader.py
+-rw-r--r--   0        0        0        0 2024-05-08 00:36:47.277516 suskabot-0.2.0/suskabot/utils/__init__.py
+-rw-r--r--   0        0        0      861 2024-05-08 00:36:47.249516 suskabot-0.2.0/suskabot/utils/utils.py
+-rw-r--r--   0        0        0     2423 1970-01-01 00:00:00.000000 suskabot-0.2.0/PKG-INFO
```

### Comparing `suskabot-0.1.5/LICENSE` & `suskabot-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `suskabot-0.1.5/README.md` & `suskabot-0.2.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Suskabot
 Telegram Bot that really can do it all!
 
-There's a [PyPi package](https://pypi.org/project/suskabot/) I'm too lazy to automate the build for (yet) :)
+[PyPi package](https://pypi.org/project/suskabot/)
 
 
 ## Current functionality
 ### YouTube video downloader
   Send a link, get a video!
 
 ### Translator
```

### Comparing `suskabot-0.1.5/pyproject.toml` & `suskabot-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 package-mode = true
 name = "suskabot"
-version = "0.1.5"
+version = "0.2.0"
 description = "telegram bot with various functions"
 authors = ["vinyl_summer <vinyl6428@gmail.dotcom>"]
 readme = "README.md"
 license = "LICENSE"
 
 [[tool.poetry.source]]
 name = "gitlab"
```

### Comparing `suskabot-0.1.5/suskabot/app/app.py` & `suskabot-0.2.0/suskabot/app/app.py`

 * *Files identical despite different names*

### Comparing `suskabot-0.1.5/suskabot/config/config.py` & `suskabot-0.2.0/suskabot/config/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -105,14 +105,22 @@
         default=True
     )
 
     # TODO: having a config for yt video downloads directory seems like a nice idea
 
 
 def load_config() -> Optional[Config]:
+    """
+    Loads configurations from os.environ first and /project_name/config/.env file second,
+    then validates them using pydantic
+
+    :return: Config instance or None
+
+    :raises pydantic.ValidationError: If some configurations are invalid
+    """
     env_file_config: Dict[str, str | None] = dotenv.dotenv_values("./suskabot/config/.env")
 
     config_data: Dict[str, str | None] = {}
 
     configurations: set[str] = get_config_attributes()
     configuration: str
     for configuration in configurations:
```

### Comparing `suskabot-0.1.5/suskabot/controllers/telegram_api/bot.py` & `suskabot-0.2.0/suskabot/controllers/telegram_api/bot.py`

 * *Files identical despite different names*

### Comparing `suskabot-0.1.5/suskabot/controllers/telegram_api/handlers/app.py` & `suskabot-0.2.0/suskabot/controllers/telegram_api/handlers/app.py`

 * *Files identical despite different names*

### Comparing `suskabot-0.1.5/suskabot/controllers/telegram_api/handlers/translator.py` & `suskabot-0.2.0/suskabot/controllers/telegram_api/handlers/translator.py`

 * *Files identical despite different names*

### Comparing `suskabot-0.1.5/suskabot/controllers/telegram_api/handlers/youtube_downloader.py` & `suskabot-0.2.0/suskabot/controllers/telegram_api/handlers/youtube_downloader.py`

 * *Files identical despite different names*

### Comparing `suskabot-0.1.5/suskabot/services/translator.py` & `suskabot-0.2.0/suskabot/services/translator.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,18 @@
 
         language_to_translate_to: str = translation_rules.get(language_code, default_language_to_translate_to)
 
         logger.debug(f"Will translate from {language_code} to {language_to_translate_to}")
         return language_to_translate_to
 
     def translate(self, text_to_translate: str) -> str:
+        """
+        Translate a string from auto-detected language using defined set of rules.
+
+        """
         supported_languages: List[Language] = [Language.ENGLISH, Language.RUSSIAN, Language.UKRAINIAN]
 
         language_detector: LanguageDetector = LanguageDetectorBuilder.from_languages(*supported_languages).build()
         language_to_translate_from: str = language_detector.detect_language_of(text_to_translate).name.lower()[0:2]
         logger.debug(f"Detected {language_to_translate_from} language from \"{text_to_translate}\"")
 
         translation_services: List[str] = self._translation_services
```

### Comparing `suskabot-0.1.5/suskabot/services/youtube_downloader.py` & `suskabot-0.2.0/suskabot/services/youtube_downloader.py`

 * *Files 14% similar despite different names*

```diff
@@ -71,14 +71,26 @@
                 return video_stream
         else:
             logger.debug("No video stream fits the requirements")
             return None
 
     # all the stream availability exceptions are raised here!
     def get_youtube_video_stream(self, video_url: str) -> Optional[Stream]:
+        """
+        Gets YouTube video stream under set limits from a valid video url.
+
+        :param video_url: valid YouTube video url
+
+        :return: pytube Stream object, right now only progressive streams are supported
+
+        :raises RegexMatchError: If video url is invalid
+        :raises VideoUnavailable: If the video is unavailable for some reason
+        :raises VideoTooLarge: If video file size exceeds set limits
+        """
+
         try:
             video_data = YouTube(url=video_url)
             video_data.check_availability()
         except RegexMatchError as e:
             raise e
         except VideoUnavailable as e:
             raise e
@@ -95,14 +107,27 @@
         return video_stream
 
     def download_youtube_video_stream(
             self,
             video_stream: Stream,
             progress_callback: Callable[[Stream, bytes, int], None] | None = None
     ) -> bytes | None:
+        """
+        Download YouTube video from given stream and get bytes of it!
+        :param video_stream: pytube Stream object, needs to be obtained from get_youtube_video_stream
+        :param progress_callback: optional on_progress callback,
+        needs to have these three parameters:
+        1) Stream, video stream that is being downloaded
+        2) bytes, chunk of bytes downloaded
+        3) int, number of bytes remaining
+
+        :return: Bytes of the downloaded video or none
+
+        :raises OSError: If save_to_drive is enabled and output file couldn't be opened
+        """
         # the only way to register a callback is at the moment of YouTube object creation.
         # since this function only has a stream object to work with,
         # registering a callback is impossible by normal means.
         # one more reason to migrate from pytube, lol
         video_stream._monostate.on_progress = progress_callback
 
         if self._save_to_drive:
```

### Comparing `suskabot-0.1.5/suskabot/utils/utils.py` & `suskabot-0.2.0/suskabot/utils/utils.py`

 * *Files identical despite different names*

### Comparing `suskabot-0.1.5/PKG-INFO` & `suskabot-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: suskabot
-Version: 0.1.5
+Version: 0.2.0
 Summary: telegram bot with various functions
 License: LICENSE
 Author: vinyl_summer
 Author-email: vinyl6428@gmail.dotcom
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -17,15 +17,15 @@
 Requires-Dist: pytube (==15.0.1)
 Requires-Dist: translators (>=5.9.1,<6.0.0)
 Description-Content-Type: text/markdown
 
 # Suskabot
 Telegram Bot that really can do it all!
 
-There's a [PyPi package](https://pypi.org/project/suskabot/) I'm too lazy to automate the build for (yet) :)
+[PyPi package](https://pypi.org/project/suskabot/)
 
 
 ## Current functionality
 ### YouTube video downloader
   Send a link, get a video!
 
 ### Translator
```

