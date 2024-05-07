# Comparing `tmp/suskabot-0.1.4.tar.gz` & `tmp/suskabot-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "suskabot-0.1.4.tar", max compression
+gzip compressed data, was "suskabot-0.1.5.tar", max compression
```

## Comparing `suskabot-0.1.4.tar` & `suskabot-0.1.5.tar`

### file list

```diff
@@ -1,37 +1,24 @@
--rw-r--r--   0        0        0     1072 2024-05-02 18:06:21.482636 suskabot-0.1.4/LICENSE
--rw-r--r--   0        0        0     1259 2024-05-02 18:41:14.923064 suskabot-0.1.4/README.md
--rw-r--r--   0        0        0      589 2024-05-02 19:45:38.198484 suskabot-0.1.4/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-02 18:06:21.485969 suskabot-0.1.4/suskabot/__init__.py
--rw-r--r--   0        0        0     2162 2024-05-02 18:15:27.733565 suskabot-0.1.4/suskabot/app/__pycache__/app.cpython-312.pyc
--rw-r--r--   0        0        0     1493 2024-05-02 18:15:26.120161 suskabot-0.1.4/suskabot/app/app.py
--rw-r--r--   0        0        0      193 2024-05-02 18:09:17.267217 suskabot-0.1.4/suskabot/config/.env.public
--rw-r--r--   0        0        0       11 2024-05-02 18:09:17.267217 suskabot-0.1.4/suskabot/config/.gitignore
--rw-r--r--   0        0        0        0 2024-05-02 18:09:17.267217 suskabot-0.1.4/suskabot/config/__init__.py
--rw-r--r--   0        0        0      172 2024-05-02 18:12:21.395386 suskabot-0.1.4/suskabot/config/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0     5089 2024-05-02 18:14:49.615231 suskabot-0.1.4/suskabot/config/__pycache__/config.cpython-312.pyc
--rw-r--r--   0        0        0     4353 2024-05-02 18:14:48.165167 suskabot-0.1.4/suskabot/config/config.py
--rw-r--r--   0        0        0     2289 2024-05-02 18:15:41.380828 suskabot-0.1.4/suskabot/controllers/telegram_api/__pycache__/bot.cpython-312.pyc
--rw-r--r--   0        0        0     1449 2024-05-02 18:15:39.770757 suskabot-0.1.4/suskabot/controllers/telegram_api/bot.py
--rw-r--r--   0        0        0     2190 2024-05-02 18:15:41.380828 suskabot-0.1.4/suskabot/controllers/telegram_api/handlers/__pycache__/app.cpython-312.pyc
--rw-r--r--   0        0        0     3056 2024-05-02 18:15:52.854662 suskabot-0.1.4/suskabot/controllers/telegram_api/handlers/__pycache__/translator.cpython-312.pyc
--rw-r--r--   0        0        0     9217 2024-05-02 18:23:46.271858 suskabot-0.1.4/suskabot/controllers/telegram_api/handlers/__pycache__/youtube_downloader.cpython-312.pyc
--rw-r--r--   0        0        0     1339 2024-05-02 18:09:17.267217 suskabot-0.1.4/suskabot/controllers/telegram_api/handlers/app.py
--rw-r--r--   0        0        0     1774 2024-05-02 18:15:51.074584 suskabot-0.1.4/suskabot/controllers/telegram_api/handlers/translator.py
--rw-r--r--   0        0        0     5900 2024-05-02 18:22:04.550799 suskabot-0.1.4/suskabot/controllers/telegram_api/handlers/youtube_downloader.py
--rw-r--r--   0        0        0      907 2024-05-02 18:15:09.899452 suskabot-0.1.4/suskabot/main.py
--rw-r--r--   0        0        0     4446 2024-05-02 18:09:50.008678 suskabot-0.1.4/suskabot/services/__pycache__/translator.cpython-312.pyc
--rw-r--r--   0        0        0     6867 2024-05-02 18:17:52.319867 suskabot-0.1.4/suskabot/services/__pycache__/youtube_downloader.cpython-312.pyc
--rw-r--r--   0        0        0     4050 2024-05-02 18:09:17.267217 suskabot-0.1.4/suskabot/services/translator.py
--rw-r--r--   0        0        0     4901 2024-05-02 18:17:45.622909 suskabot-0.1.4/suskabot/services/youtube_downloader.py
--rw-r--r--   0        0        0        0 2024-05-02 18:09:17.267217 suskabot-0.1.4/suskabot/tests/__init__.py
--rw-r--r--   0        0        0      171 2024-05-02 18:09:50.008678 suskabot-0.1.4/suskabot/tests/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0     2385 2024-05-02 18:09:50.008678 suskabot-0.1.4/suskabot/tests/__pycache__/test_translator.cpython-312-pytest-7.4.4.pyc
--rw-r--r--   0        0        0     3285 2024-05-02 18:09:50.338692 suskabot-0.1.4/suskabot/tests/__pycache__/test_youtube_downloader.cpython-312-pytest-7.4.4.pyc
--rw-r--r--   0        0        0  1550800 2024-05-02 18:09:17.267217 suskabot-0.1.4/suskabot/tests/resources/cats.mp4
--rw-r--r--   0        0        0     1028 2024-05-02 18:09:17.267217 suskabot-0.1.4/suskabot/tests/test_translator.py
--rw-r--r--   0        0        0     1622 2024-05-02 18:09:17.267217 suskabot-0.1.4/suskabot/tests/test_youtube_downloader.py
--rw-r--r--   0        0        0        0 2024-05-02 18:14:03.413206 suskabot-0.1.4/suskabot/utils/__init__.py
--rw-r--r--   0        0        0      171 2024-05-02 18:14:49.708568 suskabot-0.1.4/suskabot/utils/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0     1410 2024-05-02 18:09:50.355360 suskabot-0.1.4/suskabot/utils/__pycache__/utils.cpython-312.pyc
--rw-r--r--   0        0        0      861 2024-05-02 18:09:17.267217 suskabot-0.1.4/suskabot/utils/utils.py
--rw-r--r--   0        0        0     1984 1970-01-01 00:00:00.000000 suskabot-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-07 22:15:25.148151 suskabot-0.1.5/LICENSE
+-rw-r--r--   0        0        0     1764 2024-05-07 22:15:25.148151 suskabot-0.1.5/README.md
+-rw-r--r--   0        0        0      779 2024-05-07 22:15:25.155151 suskabot-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-07 22:15:25.181151 suskabot-0.1.5/suskabot/__init__.py
+-rw-r--r--   0        0        0      862 2024-05-07 22:15:25.155151 suskabot-0.1.5/suskabot/__main__.py
+-rw-r--r--   0        0        0        0 2024-05-07 22:15:25.181151 suskabot-0.1.5/suskabot/app/__init__.py
+-rw-r--r--   0        0        0     1529 2024-05-07 22:15:25.155151 suskabot-0.1.5/suskabot/app/app.py
+-rw-r--r--   0        0        0      295 2024-05-07 22:15:25.155151 suskabot-0.1.5/suskabot/config/.env.example
+-rw-r--r--   0        0        0        4 2024-05-07 22:15:25.156151 suskabot-0.1.5/suskabot/config/.gitignore
+-rw-r--r--   0        0        0        0 2024-05-07 22:15:25.181151 suskabot-0.1.5/suskabot/config/__init__.py
+-rw-r--r--   0        0        0     4658 2024-05-07 22:15:25.156151 suskabot-0.1.5/suskabot/config/config.py
+-rw-r--r--   0        0        0        0 2024-05-07 22:15:25.181151 suskabot-0.1.5/suskabot/controllers/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-07 22:15:25.181151 suskabot-0.1.5/suskabot/controllers/telegram_api/__init__.py
+-rw-r--r--   0        0        0     1494 2024-05-07 22:15:25.156151 suskabot-0.1.5/suskabot/controllers/telegram_api/bot.py
+-rw-r--r--   0        0        0        0 2024-05-07 22:15:25.181151 suskabot-0.1.5/suskabot/controllers/telegram_api/handlers/__init__.py
+-rw-r--r--   0        0        0     1339 2024-05-07 22:15:25.156151 suskabot-0.1.5/suskabot/controllers/telegram_api/handlers/app.py
+-rw-r--r--   0        0        0     1783 2024-05-07 22:15:25.156151 suskabot-0.1.5/suskabot/controllers/telegram_api/handlers/translator.py
+-rw-r--r--   0        0        0     5917 2024-05-07 22:15:25.156151 suskabot-0.1.5/suskabot/controllers/telegram_api/handlers/youtube_downloader.py
+-rw-r--r--   0        0        0        0 2024-05-07 22:15:25.181151 suskabot-0.1.5/suskabot/services/__init__.py
+-rw-r--r--   0        0        0     4050 2024-05-07 22:15:25.156151 suskabot-0.1.5/suskabot/services/translator.py
+-rw-r--r--   0        0        0     4908 2024-05-07 22:15:25.156151 suskabot-0.1.5/suskabot/services/youtube_downloader.py
+-rw-r--r--   0        0        0        0 2024-05-07 22:15:25.181151 suskabot-0.1.5/suskabot/utils/__init__.py
+-rw-r--r--   0        0        0      861 2024-05-07 22:15:25.156151 suskabot-0.1.5/suskabot/utils/utils.py
+-rw-r--r--   0        0        0     2481 1970-01-01 00:00:00.000000 suskabot-0.1.5/PKG-INFO
```

### Comparing `suskabot-0.1.4/LICENSE` & `suskabot-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `suskabot-0.1.4/suskabot/app/app.py` & `suskabot-0.1.5/suskabot/app/app.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from telegram.ext import ApplicationBuilder, Application
 
-from config.config import Config
-from controllers.telegram_api.bot import TGBot
-from services.translator import TranslatorService
-from services.youtube_downloader import YTDownloaderService
+from suskabot.config.config import Config
+from suskabot.controllers.telegram_api.bot import TGBot
+from suskabot.services.translator import TranslatorService
+from suskabot.services.youtube_downloader import YTDownloaderService
 
 
 class App:
     _translator_service: TranslatorService
     _youtube_downloader_service: YTDownloaderService
 
     _ptb_app: Application
```

### Comparing `suskabot-0.1.4/suskabot/config/config.py` & `suskabot-0.1.5/suskabot/config/config.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,114 +1,138 @@
 import logging
 import os
+import enum
 from typing import Self, Dict, Optional
 
 import telegram.constants
 import pydantic
 import dotenv
 
-# from suskabot.utils import utils
-from utils import utils
-
+from suskabot.utils import utils
 
 logger = logging.getLogger(__name__)
 
 
-POSSIBLE_VIDEO_RESOLUTIONS = [
-    144,
-    240,
-    360,
-    480,
-    720,
-    1080,
-    1440,
-    2160
-]
+class VideoResolution(enum.Enum):
+    RES_144 = 144
+    RES_240 = 240
+    RES_360 = 360
+    RES_480 = 480
+    RES_720 = 720
+    RES_1080 = 1080
+    RES_1440 = 1440
+    RES_2160 = 2160
+
+
+def get_lowest_resolution_value() -> int:
+    return VideoResolution.RES_144.value
+
+
+def get_highest_resolution_value() -> int:
+    return VideoResolution.RES_2160.value
 
 
+# it is assumed that every valid configuration is type annotated
+# I tried really hard, but there's no easier way to achieve the same functionality without repeating config names
+def get_config_attributes() -> set[str]:
+    return vars(Config)['__annotations__'].keys()
+
+
+# every configuration must be type annotated, else it won't be loaded!!!
 class Config(pydantic.BaseModel):
-    tg_bot_api_token: str = pydantic.Field(pattern=r"^[0-9]{8,10}:[a-zA-Z0-9_-]{35}$")
+    tg_bot_api_token: str
+
+    comma_separated_translation_services: str
+    user_language: str
+    default_language_to_translate_to: str
+
+    minimum_video_resolution: int
+    maximum_video_resolution: int
+    file_size_limit_mb: int
+    save_to_drive: bool
+
+    tg_bot_api_token = pydantic.Field(
+        pattern=r"^[0-9]+:[a-zA-Z0-9_-]+$"
+    )
 
-    comma_separated_translation_services: str = pydantic.Field(
+    comma_separated_translation_services = pydantic.Field(
         default="google,yandex,bing,argos",
         pattern=r"^([a-zA-Z]+,?)+"
     )
-    user_language: str = pydantic.Field(
+    user_language = pydantic.Field(
         default="ru",
         pattern=r"^[^-]{2,3}(-[^-]{2,3})?(-[^-]{2,3})?$"
     )
-    default_language_to_translate_to: str = pydantic.Field(
+    default_language_to_translate_to = pydantic.Field(
         default="en",
         pattern=r"^[^-]{2,3}(-[^-]{2,3})?(-[^-]{2,3})?$",
     )
 
     # right now only progressive videos are supported, so video quality is 720p max.
     # it also looks like 360p and 720p are the only available options
-    minimum_video_resolution: int = POSSIBLE_VIDEO_RESOLUTIONS[0]
-    maximum_video_resolution: int = POSSIBLE_VIDEO_RESOLUTIONS[-1]
+    minimum_video_resolution = pydantic.Field(
+        default=get_lowest_resolution_value(),
+    )
+    maximum_video_resolution = pydantic.Field(
+        default=get_highest_resolution_value(),
+    )
 
     @pydantic.field_validator("maximum_video_resolution", "minimum_video_resolution")
-    def validate_option(cls, v):
-        assert v in POSSIBLE_VIDEO_RESOLUTIONS, ("this does not look like a valid resolution. "
-                                                 f"supported resolutions: {POSSIBLE_VIDEO_RESOLUTIONS}")
+    def validate_resolution(cls, v):
+        valid_video_resolutions = [res.value for res in VideoResolution]
+        assert v in valid_video_resolutions, ("this does not look like a valid resolution. "
+                                              f"supported resolutions: {valid_video_resolutions}")
         return v
 
     @pydantic.model_validator(mode='after')
     def check_if_valid_video_resolution_preferences(self) -> Self:
         if self.minimum_video_resolution > self.maximum_video_resolution:
             raise ValueError("minimum video resolution can't be higher than maximum video resolution")
         if self.minimum_video_resolution > 720:
             logger.warning("Since only progressive videos are supported right now,"
                            " 720p is the maximum possible resolution")
         return self
 
     # setting the limit higher than the default will break telegram api controller!
-    file_size_limit_mb: int = pydantic.Field(
+    file_size_limit_mb = pydantic.Field(
         default=utils.bytes_to_megabytes(
             telegram.constants.FileSizeLimit.FILESIZE_UPLOAD.value
         ),
         gt=0,
         validate_default=True
     )
 
-    save_to_drive: bool = pydantic.Field(
+    save_to_drive = pydantic.Field(
         default=True
     )
 
     # TODO: having a config for yt video downloads directory seems like a nice idea
 
 
 def load_config() -> Optional[Config]:
-    if not os.path.exists("./suskabot/config/.env.secret"):
-        with open("./suskabot/config/.env.secret", "w") as f:
-            f.write("TG_BOT_API_TOKEN=")
-        logger.info("Created .env.secret file")
-
-    public_env_file_config: Dict[str, str | None] = dotenv.dotenv_values("./suskabot/config/.env.public")
-
-    secret_env_file_config: Dict[str, str | None] = dotenv.dotenv_values("./suskabot/config/.env.secret")
+    env_file_config: Dict[str, str | None] = dotenv.dotenv_values("./suskabot/config/.env")
 
     config_data: Dict[str, str | None] = {}
-    # it is assumed that every valid configuration is type annotated
-    # I tried really hard, but there's no easier way to achieve the same functionality without repeating config names
-    configurations: set[str] = vars(Config)['__annotations__'].keys()
+
+    configurations: set[str] = get_config_attributes()
     configuration: str
     for configuration in configurations:
         configuration_value: str | None
-        configuration_upper = configuration.upper()
+        configuration_upper: str = configuration.upper()
+
         logger.debug(f"Getting {configuration}..")
-        if configuration_upper in os.environ:
+
+        if configuration_upper in os.environ and os.environ.get(configuration_upper) is not None:
             configuration_value = os.environ[configuration_upper]
             logger.debug(f"Got {configuration} from environ")
-        elif configuration_upper in secret_env_file_config:
-            configuration_value = secret_env_file_config[configuration_upper]
-            logger.debug(f"Got {configuration} from env.secret")
-        elif configuration_upper in public_env_file_config:
-            configuration_value = public_env_file_config[configuration_upper]
-            logger.debug(f"Got {configuration} from env.public")
+
+        elif configuration_upper in env_file_config and env_file_config.get(configuration_upper) != "":
+            configuration_value = env_file_config[configuration_upper]
+            logger.debug(f"Got {configuration} from .env")
+
         else:
             logger.debug(f"Couldn't find {configuration} anywhere, will try to use the default value")
             continue
 
         config_data[configuration] = configuration_value
         logger.info(f"{configuration} set to {configuration_value}")
```

### Comparing `suskabot-0.1.4/suskabot/controllers/telegram_api/bot.py` & `suskabot-0.1.5/suskabot/controllers/telegram_api/bot.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import logging
 
 from telegram.ext import Application
 
-from controllers.telegram_api.handlers.app import AppHandlers
-from controllers.telegram_api.handlers.translator import TranslatorHandlers
-from controllers.telegram_api.handlers.youtube_downloader import YTDownloaderHandlers
-from services.translator import TranslatorService
-from services.youtube_downloader import YTDownloaderService
+from suskabot.controllers.telegram_api.handlers.app import AppHandlers
+from suskabot.controllers.telegram_api.handlers.translator import TranslatorHandlers
+from suskabot.controllers.telegram_api.handlers.youtube_downloader import YTDownloaderHandlers
+from suskabot.services.translator import TranslatorService
+from suskabot.services.youtube_downloader import YTDownloaderService
 
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
 class TGBot:
     _application: Application
```

### Comparing `suskabot-0.1.4/suskabot/controllers/telegram_api/handlers/app.py` & `suskabot-0.1.5/suskabot/controllers/telegram_api/handlers/app.py`

 * *Files identical despite different names*

### Comparing `suskabot-0.1.4/suskabot/controllers/telegram_api/handlers/translator.py` & `suskabot-0.1.5/suskabot/controllers/telegram_api/handlers/translator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 
 from telegram import Update
 from telegram.ext import ContextTypes, Application, MessageHandler, filters
 from translators.server import TranslatorError
 
-from services.translator import TranslatorService
+from suskabot.services.translator import TranslatorService
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
 class TranslatorHandlers:
     _application: Application
     _translator_service: TranslatorService
```

### Comparing `suskabot-0.1.4/suskabot/controllers/telegram_api/handlers/youtube_downloader.py` & `suskabot-0.1.5/suskabot/controllers/telegram_api/handlers/youtube_downloader.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import asyncio
 import logging
 import concurrent.futures
+
 from asyncio import AbstractEventLoop
-from typing import  Set
+from typing import Set
 
 import telegram.error
 from pytube import Stream
 from pytube.exceptions import RegexMatchError, VideoUnavailable, PytubeError
 from telegram import Update, Message
 from telegram.ext import ContextTypes, Application, MessageHandler, filters
 
-from services.youtube_downloader import YTDownloaderService, VideoTooLarge
-
-from utils import utils
+from suskabot.services.youtube_downloader import YTDownloaderService, VideoTooLarge
+from suskabot.utils import utils
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
 class YTDownloaderHandlers:
     _application: Application
     _yt_downloader_service: YTDownloaderService
```

### Comparing `suskabot-0.1.4/suskabot/main.py` & `suskabot-0.1.5/suskabot/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import logging
 import sys
 
 from typing import Optional
 from contextlib import suppress
 
-from config import config
+from suskabot.config import config
 
-from app import app
+from suskabot.app import app
 
 
 logging.basicConfig(
     format='%(asctime)s - %(name)s - %(levelname)s - %(message)s',
     level=logging.INFO,
     force=True
 )
@@ -18,19 +18,18 @@
     # prevents log spam from infinite polling
     logging.getLogger("httpx").setLevel(logging.WARNING)
 
 
 logger = logging.getLogger(__name__)
 
 
-if __name__ == '__main__':
-    # somehow pydantic raises an attribute error when I'm trying to access config.Config for the type hint
-    # removing the type hint solves the issue, but I'd rather just suppress the pydantic error
-    with suppress(AttributeError):
-        config: Optional[config.Config] = config.load_config()
-    if not config:
-        logger.error("Couldn't load config file")
-        sys.exit(1)
+# somehow pydantic raises an attribute error when I'm trying to access config.Config for the type hint
+# removing the type hint solves the issue, but I'd rather just suppress the pydantic error
+with suppress(AttributeError):
+    config: Optional[config.Config] = config.load_config()
+if not config:
+    logger.error("Couldn't load config file")
+    sys.exit(1)
 
-    app = app.App(config)
+app = app.App(config)
 
-    app.run()
+app.run()
```

### Comparing `suskabot-0.1.4/suskabot/services/__pycache__/translator.cpython-312.pyc` & `suskabot-0.1.5/suskabot/services/translator.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,278 +1,254 @@
-00000000: cb0d 0d0a 0000 0000 cdd6 3366 d20f 0000  ..........3f....
-00000010: e300 0000 0000 0000 0000 0000 0004 0000  ................
-00000020: 0000 0000 00f3 7c00 0000 9700 6400 6401  ......|.....d.d.
-00000030: 6c00 5a00 6400 6402 6c01 6d02 5a02 6d03  l.Z.d.d.l.m.Z.m.
-00000040: 5a03 0100 6400 6401 6c04 5a04 6400 6403  Z...d.d.l.Z.d.d.
-00000050: 6c05 6d06 5a06 6d07 5a07 6d08 5a08 0100  l.m.Z.m.Z.m.Z...
-00000060: 6400 6404 6c09 6d0a 5a0a 0100 0200 6500  d.d.l.m.Z.....e.
-00000070: 6a16 0000 0000 0000 0000 0000 0000 0000  j...............
-00000080: 0000 0000 650c ab01 0000 0000 0000 5a0d  ....e.........Z.
-00000090: 0200 4700 6405 8400 6406 ab02 0000 0000  ..G.d...d.......
-000000a0: 0000 5a0e 7901 2907 e900 0000 004e 2902  ..Z.y.)......N).
-000000b0: da04 4c69 7374 da04 4469 6374 2903 da08  ..List..Dict)...
-000000c0: 4c61 6e67 7561 6765 da10 4c61 6e67 7561  Language..Langua
-000000d0: 6765 4465 7465 6374 6f72 da17 4c61 6e67  geDetector..Lang
-000000e0: 7561 6765 4465 7465 6374 6f72 4275 696c  uageDetectorBuil
-000000f0: 6465 7229 01da 0f54 7261 6e73 6c61 746f  der)...Translato
-00000100: 7245 7272 6f72 6300 0000 0000 0000 0000  rErrorc.........
-00000110: 0000 0008 0000 0000 0000 00f3 6a00 0000  ............j...
-00000120: 9700 6500 5a01 6400 5a02 5500 6503 6504  ..e.Z.d.Z.U.e.e.
-00000130: 1900 0000 6505 6401 3c00 0000 6504 6505  ....e.d.<...e.e.
-00000140: 6402 3c00 0000 6504 6505 6403 3c00 0000  d.<...e.e.d.<...
-00000150: 6404 6504 6405 6504 6406 6504 6407 6408  d.e.d.e.d.e.d.d.
-00000160: 6608 6409 8404 5a06 640a 6504 6407 6504  f.d...Z.d.e.d.e.
-00000170: 6604 640b 8404 5a07 640c 6504 6407 6504  f.d...Z.d.e.d.e.
-00000180: 6604 640d 8404 5a08 7908 290e da11 5472  f.d...Z.y.)...Tr
-00000190: 616e 736c 6174 6f72 5365 7276 6963 65da  anslatorService.
-000001a0: 155f 7472 616e 736c 6174 696f 6e5f 7365  ._translation_se
-000001b0: 7276 6963 6573 da0e 5f75 7365 725f 6c61  rvices.._user_la
-000001c0: 6e67 7561 6765 da21 5f64 6566 6175 6c74  nguage.!_default
-000001d0: 5f6c 616e 6775 6167 655f 746f 5f74 7261  _language_to_tra
-000001e0: 6e73 6c61 7465 5f74 6fda 2463 6f6d 6d61  nslate_to.$comma
-000001f0: 5f73 6570 6172 6174 6564 5f74 7261 6e73  _separated_trans
-00000200: 6c61 7469 6f6e 5f73 6572 7669 6365 73da  lation_services.
-00000210: 0d75 7365 725f 6c61 6e67 7561 6765 da1c  .user_language..
-00000220: 6465 6661 756c 745f 6c61 6e67 5f74 6f5f  default_lang_to_
-00000230: 7472 616e 736c 6174 655f 746f da06 7265  translate_to..re
-00000240: 7475 726e 4e63 0400 0000 0000 0000 0000  turnNc..........
-00000250: 0000 0300 0000 0300 0000 f36c 0000 0097  ...........l....
-00000260: 007c 016a 0100 0000 0000 0000 0000 0000  .|.j............
-00000270: 0000 0000 0000 00ab 0000 0000 0000 006a  ...............j
-00000280: 0300 0000 0000 0000 0000 0000 0000 0000  ................
-00000290: 0000 0064 01ab 0100 0000 0000 007d 047c  ...d.........}.|
-000002a0: 047c 005f 0200 0000 0000 0000 007c 027c  .|._.........|.|
-000002b0: 005f 0300 0000 0000 0000 007c 037c 005f  ._.........|.|._
-000002c0: 0400 0000 0000 0000 0079 0029 024e fa01  .........y.).N..
-000002d0: 2c29 05da 0573 7472 6970 da05 7370 6c69  ,)...strip..spli
-000002e0: 7472 0b00 0000 720c 0000 0072 0d00 0000  tr....r....r....
-000002f0: 2905 da04 7365 6c66 720e 0000 0072 0f00  )...selfr....r..
-00000300: 0000 7210 0000 00da 1474 7261 6e73 6c61  ..r......transla
-00000310: 7469 6f6e 5f73 6572 7669 6365 7373 0500  tion_servicess..
-00000320: 0000 2020 2020 20fa 4f2f 686f 6d65 2f76  ..     .O/home/v
-00000330: 696e 796c 2f50 726f 6a65 6374 732f 5079  inyl/Projects/Py
-00000340: 6368 6172 6d50 726f 6a65 6374 732f 7375  charmProjects/su
-00000350: 736b 615f 7465 7374 2f73 7573 6b61 626f  ska_test/suskabo
-00000360: 742f 7365 7276 6963 6573 2f74 7261 6e73  t/services/trans
-00000370: 6c61 746f 722e 7079 da08 5f5f 696e 6974  lator.py..__init
-00000380: 5f5f 7a1a 5472 616e 736c 6174 6f72 5365  __z.TranslatorSe
-00000390: 7276 6963 652e 5f5f 696e 6974 5f5f 1100  rvice.__init__..
-000003a0: 0000 7338 0000 0080 00f0 0c00 2b4f 01d7  ..s8........+O..
-000003b0: 2a54 d12a 54d3 2a56 d72a 5cd1 2a5c d05d  *T.*T.*V.*\.*\.]
-000003c0: 60d3 2a61 d008 1cd8 2539 8804 d408 22e0  `.*a....%9....".
-000003d0: 1e2b 8804 d408 1bd8 314d 8804 d508 2ef3  .+......1M......
-000003e0: 0000 0000 da0d 6c61 6e67 7561 6765 5f63  ......language_c
-000003f0: 6f64 6563 0200 0000 0000 0000 0000 0000  odec............
-00000400: 0600 0000 0300 0000 f3a8 0000 0097 007c  ...............|
-00000410: 006a 0000 0000 0000 0000 0000 0000 0000  .j..............
-00000420: 0000 0000 007c 006a 0200 0000 0000 0000  .....|.j........
-00000430: 0000 0000 0000 0000 0000 0069 017d 027c  ...........i.}.|
-00000440: 006a 0000 0000 0000 0000 0000 0000 0000  .j..............
-00000450: 0000 0000 007d 037c 026a 0500 0000 0000  .....}.|.j......
-00000460: 0000 0000 0000 0000 0000 0000 007c 017c  .............|.|
-00000470: 03ab 0200 0000 0000 007d 0474 0600 0000  .........}.t....
-00000480: 0000 0000 006a 0900 0000 0000 0000 0000  .....j..........
-00000490: 0000 0000 0000 0000 0064 017c 019b 0064  .........d.|...d
-000004a0: 027c 049b 009d 04ab 0100 0000 0000 0001  .|..............
-000004b0: 007c 0453 0029 034e 7a14 5769 6c6c 2074  .|.S.).Nz.Will t
-000004c0: 7261 6e73 6c61 7465 2066 726f 6d20 fa04  ranslate from ..
-000004d0: 2074 6f20 2905 720d 0000 0072 0c00 0000   to ).r....r....
-000004e0: da03 6765 74da 066c 6f67 6765 72da 0564  ..get..logger..d
-000004f0: 6562 7567 2905 7216 0000 0072 1b00 0000  ebug).r....r....
-00000500: da11 7472 616e 736c 6174 696f 6e5f 7275  ..translation_ru
-00000510: 6c65 73da 2064 6566 6175 6c74 5f6c 616e  les. default_lan
-00000520: 6775 6167 655f 746f 5f74 7261 6e73 6c61  guage_to_transla
-00000530: 7465 5f74 6fda 186c 616e 6775 6167 655f  te_to..language_
-00000540: 746f 5f74 7261 6e73 6c61 7465 5f74 6f73  to_translate_tos
-00000550: 0500 0000 2020 2020 2072 1800 0000 da1e  ....     r......
-00000560: 5f5f 6765 745f 6c61 6e67 7561 6765 5f74  __get_language_t
-00000570: 6f5f 7472 616e 736c 6174 655f 746f 7a30  o_translate_toz0
-00000580: 5472 616e 736c 6174 6f72 5365 7276 6963  TranslatorServic
-00000590: 652e 5f5f 6765 745f 6c61 6e67 7561 6765  e.__get_language
-000005a0: 5f74 6f5f 7472 616e 736c 6174 655f 746f  _to_translate_to
-000005b0: 1d00 0000 7361 0000 0080 00f0 0600 0d11  ....sa..........
-000005c0: d70c 32d1 0c32 b044 d734 47d1 3447 f003  ..2..2.D.4G.4G..
-000005d0: 022d 0ad0 0819 f006 0031 35d7 3056 d130  .-.......15.0V.0
-000005e0: 56d0 0828 e028 39d7 283d d128 3db8 6dd0  V..(.(9.(=.(=.m.
-000005f0: 4d6d d328 6ed0 0820 e408 0e8f 0c89 0cd0  Mm.(n.. ........
-00000600: 172b a84d a83f b824 d03f 57d0 3e58 d015  .+.M.?.$.?W.>X..
-00000610: 59d4 085a d80f 27d0 0827 721a 0000 00da  Y..Z..'..'r.....
-00000620: 1174 6578 745f 746f 5f74 7261 6e73 6c61  .text_to_transla
-00000630: 7465 6302 0000 0000 0000 0000 0000 000f  tec.............
-00000640: 0000 0003 0000 00f3 9003 0000 9700 7400  ..............t.
-00000650: 0000 0000 0000 0000 6a02 0000 0000 0000  ........j.......
-00000660: 0000 0000 0000 0000 0000 0000 7400 0000  ............t...
-00000670: 0000 0000 0000 6a04 0000 0000 0000 0000  ......j.........
-00000680: 0000 0000 0000 0000 0000 7400 0000 0000  ..........t.....
-00000690: 0000 0000 6a06 0000 0000 0000 0000 0000  ....j...........
-000006a0: 0000 0000 0000 0000 6703 7d02 7409 0000  ........g.}.t...
-000006b0: 0000 0000 0000 6a0a 0000 0000 0000 0000  ......j.........
-000006c0: 0000 0000 0000 0000 0000 7c02 8e00 6a0d  ..........|...j.
-000006d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000006e0: 0000 ab00 0000 0000 0000 7d03 7c03 6a0f  ..........}.|.j.
-000006f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000700: 0000 7c01 ab01 0000 0000 0000 6a10 0000  ..|.........j...
-00000710: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000720: 6a13 0000 0000 0000 0000 0000 0000 0000  j...............
-00000730: 0000 0000 ab00 0000 0000 0000 6401 6402  ............d.d.
-00000740: 1a00 7d04 7414 0000 0000 0000 0000 6a17  ..}.t.........j.
-00000750: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000760: 0000 6403 7c04 9b00 6404 7c01 9b00 6405  ..d.|...d.|...d.
-00000770: 9d05 ab01 0000 0000 0000 0100 7c00 6a18  ............|.j.
-00000780: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000790: 0000 7d05 7c00 6a1b 0000 0000 0000 0000  ..}.|.j.........
-000007a0: 0000 0000 0000 0000 0000 7c04 ab01 0000  ..........|.....
-000007b0: 0000 0000 7d06 7414 0000 0000 0000 0000  ....}.t.........
-000007c0: 6a17 0000 0000 0000 0000 0000 0000 0000  j...............
-000007d0: 0000 0000 6406 7c05 9b00 9d02 ab01 0000  ....d.|.........
-000007e0: 0000 0000 0100 7c05 4400 5d5c 0000 7d07  ......|.D.]\..}.
-000007f0: 7414 0000 0000 0000 0000 6a17 0000 0000  t.........j.....
-00000800: 0000 0000 0000 0000 0000 0000 0000 6407  ..............d.
-00000810: 7c07 9b00 6408 9d03 ab01 0000 0000 0000  |...d...........
-00000820: 0100 0900 741d 0000 0000 0000 0000 6a1e  ....t.........j.
-00000830: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000840: 0000 7c01 7c07 7c04 7c06 6409 ac0a ab05  ..|.|.|.|.d.....
-00000850: 0000 0000 0000 7d08 7414 0000 0000 0000  ......}.t.......
-00000860: 0000 6a27 0000 0000 0000 0000 0000 0000  ..j'............
-00000870: 0000 0000 0000 6411 7c01 9b00 640d 7c08  ......d.|...d.|.
-00000880: 9b00 640c 7c04 9b00 640d 7c06 9b00 640e  ..d.|...d.|...d.
-00000890: 7c07 9b00 9d0a ab01 0000 0000 0000 0100  |...............
-000008a0: 0100 7c08 5300 0400 7414 0000 0000 0000  ..|.S...t.......
-000008b0: 0000 6a23 0000 0000 0000 0000 0000 0000  ..j#............
-000008c0: 0000 0000 0000 6412 7c01 9b00 6413 7c04  ......d.|...d.|.
-000008d0: 9b00 6414 7c06 9b00 6415 9d07 ab01 0000  ..d.|...d.......
-000008e0: 0000 0000 0100 7421 0000 0000 0000 0000  ......t!........
-000008f0: 6416 ab01 0000 0000 0000 8201 2300 7420  d...........#.t 
-00000900: 0000 0000 0000 0000 2400 722e 7d09 7414  ........$.r.}.t.
-00000910: 0000 0000 0000 0000 6a23 0000 0000 0000  ........j#......
-00000920: 0000 0000 0000 0000 0000 0000 7c09 9b00  ............|...
-00000930: 640b 7c01 9b00 640c 7c04 9b00 640d 7c06  d.|...d.|...d.|.
-00000940: 9b00 640e 7c07 9b00 640f 9d0a ab01 0000  ..d.|...d.......
-00000950: 0000 0000 0100 5900 6400 7d09 7e09 8cbb  ......Y.d.}.~...
-00000960: 6400 7d09 7e09 7701 7424 0000 0000 0000  d.}.~.w.t$......
-00000970: 0000 2400 722f 7d09 7414 0000 0000 0000  ..$.r/}.t.......
-00000980: 0000 6a23 0000 0000 0000 0000 0000 0000  ..j#............
-00000990: 0000 0000 0000 6410 7c09 9b00 640b 7c01  ......d.|...d.|.
-000009a0: 9b00 640c 7c04 9b00 640d 7c06 9b00 640e  ..d.|...d.|...d.
-000009b0: 7c07 9b00 640f 9d0b ab01 0000 0000 0000  |...d...........
-000009c0: 0100 5900 6400 7d09 7e09 8cf1 6400 7d09  ..Y.d.}.~...d.}.
-000009d0: 7e09 7701 7700 7803 5900 7701 2917 4e72  ~.w.w.x.Y.w.).Nr
-000009e0: 0200 0000 e902 0000 007a 0944 6574 6563  .........z.Detec
-000009f0: 7465 6420 7a10 206c 616e 6775 6167 6520  ted z. language 
-00000a00: 6672 6f6d 2022 fa01 227a 2c57 696c 6c20  from ".."z,Will 
-00000a10: 7573 6520 7468 6973 206c 6973 7420 6f66  use this list of
-00000a20: 2074 7261 6e73 6c61 7469 6f6e 2073 6572   translation ser
-00000a30: 7669 6365 733a 207a 1a54 7279 696e 6720  vices: z.Trying 
-00000a40: 746f 2074 7261 6e73 6c61 7465 2075 7369  to translate usi
-00000a50: 6e67 207a 022e 2e46 2905 da0a 7175 6572  ng z...F)...quer
-00000a60: 795f 7465 7874 da0a 7472 616e 736c 6174  y_text..translat
-00000a70: 6f72 da0d 6672 6f6d 5f6c 616e 6775 6167  or..from_languag
-00000a80: 65da 0b74 6f5f 6c61 6e67 7561 6765 da16  e..to_language..
-00000a90: 6966 5f75 7365 5f70 7265 6163 6365 6c65  if_use_preaccele
-00000aa0: 7261 7469 6f6e 7a24 206f 6363 7572 7265  rationz$ occurre
-00000ab0: 6420 7768 656e 2074 7279 696e 6720 746f  d when trying to
-00000ac0: 2074 7261 6e73 6c61 7465 2022 7a08 2220   translate "z." 
-00000ad0: 6672 6f6d 2022 7a06 2220 746f 2022 7a08  from "z." to "z.
-00000ae0: 2220 7573 696e 6720 7a08 2073 6572 7669  " using z. servi
-00000af0: 6365 7a14 416e 2075 6e65 7870 6563 7465  cez.An unexpecte
-00000b00: 6420 6572 726f 7220 7a19 5375 6363 6573  d error z.Succes
-00000b10: 7366 756c 6c79 2074 7261 6e73 6c61 7465  sfully translate
-00000b20: 6420 227a 1343 6f75 6c64 6e27 7420 7472  d "z.Couldn't tr
-00000b30: 616e 736c 6174 6520 7a06 2066 726f 6d20  anslate z. from 
-00000b40: 721d 0000 007a 1220 7573 696e 6720 616e  r....z. using an
-00000b50: 7920 7365 7276 6963 657a 3241 6c6c 2074  y servicez2All t
-00000b60: 6865 2073 7065 6369 6669 6564 2074 7261  he specified tra
-00000b70: 6e73 6c61 7469 6f6e 2073 6572 7669 6365  nslation service
-00000b80: 7320 6572 726f 7265 6420 6f75 7429 1472  s errored out).r
-00000b90: 0500 0000 da07 454e 474c 4953 48da 0752  ......ENGLISH..R
-00000ba0: 5553 5349 414e da09 554b 5241 494e 4941  USSIAN..UKRAINIA
-00000bb0: 4e72 0700 0000 da0e 6672 6f6d 5f6c 616e  Nr......from_lan
-00000bc0: 6775 6167 6573 da05 6275 696c 64da 1264  guages..build..d
-00000bd0: 6574 6563 745f 6c61 6e67 7561 6765 5f6f  etect_language_o
-00000be0: 66da 046e 616d 65da 056c 6f77 6572 721f  f..name..lowerr.
-00000bf0: 0000 0072 2000 0000 720b 0000 00da 305f  ...r ...r.....0_
-00000c00: 5472 616e 736c 6174 6f72 5365 7276 6963  TranslatorServic
-00000c10: 655f 5f67 6574 5f6c 616e 6775 6167 655f  e__get_language_
-00000c20: 746f 5f74 7261 6e73 6c61 7465 5f74 6fda  to_translate_to.
-00000c30: 0b74 7261 6e73 6c61 746f 7273 da0e 7472  .translators..tr
-00000c40: 616e 736c 6174 655f 7465 7874 7208 0000  anslate_textr...
-00000c50: 00da 0777 6172 6e69 6e67 da09 4578 6365  ...warning..Exce
-00000c60: 7074 696f 6eda 0469 6e66 6f29 0a72 1600  ption..info).r..
-00000c70: 0000 7225 0000 00da 1373 7570 706f 7274  ..r%.....support
-00000c80: 6564 5f6c 616e 6775 6167 6573 da11 6c61  ed_languages..la
-00000c90: 6e67 7561 6765 5f64 6574 6563 746f 72da  nguage_detector.
-00000ca0: 1a6c 616e 6775 6167 655f 746f 5f74 7261  .language_to_tra
-00000cb0: 6e73 6c61 7465 5f66 726f 6d72 1700 0000  nslate_fromr....
-00000cc0: 7223 0000 00da 1374 7261 6e73 6c61 7469  r#.....translati
-00000cd0: 6f6e 5f73 6572 7669 6365 da0b 7472 616e  on_service..tran
-00000ce0: 736c 6174 696f 6eda 0165 730a 0000 0020  slation..es.... 
-00000cf0: 2020 2020 2020 2020 2072 1800 0000 da09           r......
-00000d00: 7472 616e 736c 6174 657a 1b54 7261 6e73  translatez.Trans
-00000d10: 6c61 746f 7253 6572 7669 6365 2e74 7261  latorService.tra
-00000d20: 6e73 6c61 7465 2900 0000 7352 0200 0080  nslate)...sR....
-00000d30: 00dc 2f37 d72f 3fd1 2f3f c418 d741 51d1  ../7./?./?...AQ.
-00000d40: 4151 d453 5bd7 5365 d153 65d0 2e66 d008  AQ.S[.Se.Se..f..
-00000d50: 1be4 2e45 d72e 54d1 2e54 d056 69d0 2e6a  ...E..T..T.Vi..j
-00000d60: d72e 70d1 2e70 d32e 72d0 0819 d82a 3bd7  ..p..p..r....*;.
-00000d70: 2a4e d12a 4ed0 4f60 d32a 61d7 2a66 d12a  *N.*N.O`.*a.*f.*
-00000d80: 66d7 2a6c d12a 6cd3 2a6e d06f 70d0 7172  f.*l.*l.*n.op.qr
-00000d90: d02a 73d0 0822 dc08 0e8f 0c89 0c90 79d0  .*s.."........y.
-00000da0: 213b d020 3cd0 3c4d d04e 5fd0 4d60 d060  !;. <.<M.N_.M`.`
-00000db0: 62d0 1563 d408 64e0 2a2e d72a 44d1 2a44  b..c..d.*..*D.*D
-00000dc0: d008 1ce0 282c d728 4bd1 284b d04c 66d3  ....(,.(K.(K.Lf.
-00000dd0: 2867 d008 20e4 080e 8f0c 890c d017 43d0  (g.. .........C.
-00000de0: 4458 d043 59d0 155a d408 5bd8 2337 f200  DX.CY..Z..[.#7..
-00000df0: 1f09 5801 d00c 1fdc 0c12 8f4c 894c d01b  ..X........L.L..
-00000e00: 35d0 3649 d035 4ac8 22d0 194d d40c 4ef0  5.6I.5J."..M..N.
-00000e10: 0213 0d19 dc23 2ed7 233d d123 3dd8 1f30  .....#..#=.#=..0
-00000e20: d81f 32d8 223c d820 38d8 2b30 f40b 0624  ..2."<. 8.+0...$
-00000e30: 1290 0bf4 2800 0d13 8f4b 894b d01a 34d0  ....(....K.K..4.
-00000e40: 3546 d034 47c0 78d0 505b c87d f000 015d  5F.4G.x.P[.}...]
-00000e50: 0122 d822 3cd0 213d f000 013e 20d8 2038  ."."<.!=...> . 8
-00000e60: d01f 39f0 0001 3a21 d821 34d0 2035 f007  ..9...:!.!4. 5..
-00000e70: 0319 37f4 0003 0d38 f008 000d 12f0 0c00  ..7....8........
-00000e80: 101b d008 1af0 4301 1f09 5801 f43a 000d  ......C...X..:..
-00000e90: 138f 4e89 4ed0 1d30 d031 42d0 3043 c036  ..N.N..0.1B.0C.6
-00000ea0: d04a 64d0 4965 f000 0166 0121 d821 39d0  .Jd.Ie...f.!.!9.
-00000eb0: 203a d03a 4cf0 0301 1c4e 01f4 0001 0d4f   :.:L....N.....O
-00000ec0: 01e4 1221 d022 56d3 1257 d00c 57f8 f42b  ...!."V..W..W..+
-00000ed0: 0014 23f2 0005 0d19 dc10 1697 0e91 0ea0  ..#.............
-00000ee0: 21a0 13d0 2449 d04a 5bd0 495c f000 015d  !...$I.J[.I\...]
-00000ef0: 0129 d829 43d0 2844 f000 0145 0127 d827  .).)C.(D...E.'.'
-00000f00: 3fd0 2640 f000 0141 0128 d828 3bd0 273c  ?.&@...A.(.(;.'<
-00000f10: b848 f007 0320 4601 f400 0311 4701 f408  .H... F.....G...
-00000f20: 0011 19fb dc13 1cf2 0005 0d19 dc10 1697  ................
-00000f30: 0e91 0ed0 2135 b061 b053 d038 5dd0 5e6f  ....!5.a.S.8].^o
-00000f40: d05d 70f0 0001 7101 29d8 2943 d028 44f0  .]p...q.).)C.(D.
-00000f50: 0001 4501 27d8 273f d026 40f0 0001 4101  ..E.'.'?.&@...A.
-00000f60: 28d8 283b d027 3cb8 48f0 0703 2046 01f4  (.(;.'<.H... F..
-00000f70: 0003 1147 01f4 0800 1119 fbf0 0b05 0d19  ...G............
-00000f80: fa73 2400 0000 c32c 1a45 1802 c518 0947  .s$....,.E.....G
-00000f90: 0505 c521 2446 0a05 c60a 0c47 0505 c616  ...!$F.....G....
-00000fa0: 2547 0005 c700 0547 0505 2909 da08 5f5f  %G.....G..)...__
-00000fb0: 6e61 6d65 5f5f da0a 5f5f 6d6f 6475 6c65  name__..__module
-00000fc0: 5f5f da0c 5f5f 7175 616c 6e61 6d65 5f5f  __..__qualname__
-00000fd0: 7203 0000 00da 0373 7472 da0f 5f5f 616e  r......str..__an
-00000fe0: 6e6f 7461 7469 6f6e 735f 5f72 1900 0000  notations__r....
-00000ff0: 7236 0000 0072 4200 0000 a900 721a 0000  r6...rB.....r...
-00001000: 0072 1800 0000 720a 0000 0072 0a00 0000  .r....r....r....
-00001010: 0c00 0000 736e 0000 0085 00d8 1b1f a003  ....sn..........
-00001020: 9939 d304 24d8 1417 d304 17d8 272a d304  .9..$.......'*..
-00001030: 2af0 040a 054e 01e0 3235 f005 0a05 4e01  *....N..25....N.
-00001040: f006 001c 1ff0 070a 054e 01f0 0800 2b2e  .........N....+.
-00001050: f009 0a05 4e01 f00a 000a 0ef3 0b0a 054e  ....N..........N
-00001060: 01f0 180a 0528 b843 f000 0a05 28c0 43f3  .....(.C....(.C.
-00001070: 000a 0528 f018 2d05 1ba8 33f0 002d 051b  ...(..-...3..-..
-00001080: b033 f400 2d05 1b72 1a00 0000 720a 0000  .3..-..r....r...
-00001090: 0029 0fda 076c 6f67 6769 6e67 da06 7479  .)...logging..ty
-000010a0: 7069 6e67 7203 0000 0072 0400 0000 7237  pingr....r....r7
-000010b0: 0000 00da 066c 696e 6775 6172 0500 0000  .....linguar....
-000010c0: 7206 0000 0072 0700 0000 da12 7472 616e  r....r......tran
-000010d0: 736c 6174 6f72 732e 7365 7276 6572 7208  slators.serverr.
-000010e0: 0000 00da 0967 6574 4c6f 6767 6572 7243  .....getLoggerrC
-000010f0: 0000 0072 1f00 0000 720a 0000 0072 4800  ...r....r....rH.
-00001100: 0000 721a 0000 0072 1800 0000 fa08 3c6d  ..r....r......<m
-00001110: 6f64 756c 653e 724e 0000 0001 0000 0073  odule>rN.......s
-00001120: 3500 0000 f003 0101 01db 000e df00 1de3  5...............
-00001130: 0012 e700 46d1 0046 dd00 2ee0 091a 8817  ....F..F........
-00001140: d709 1ad1 091a 9838 d309 2480 06f7 064a  .......8..$....J
-00001150: 0101 1bf2 004a 0101 1b72 1a00 0000       .....J...r....
+00000000: 696d 706f 7274 206c 6f67 6769 6e67 0a66  import logging.f
+00000010: 726f 6d20 7479 7069 6e67 2069 6d70 6f72  rom typing impor
+00000020: 7420 4c69 7374 2c20 4469 6374 0a0a 696d  t List, Dict..im
+00000030: 706f 7274 2074 7261 6e73 6c61 746f 7273  port translators
+00000040: 0a0a 6672 6f6d 206c 696e 6775 6120 696d  ..from lingua im
+00000050: 706f 7274 204c 616e 6775 6167 652c 204c  port Language, L
+00000060: 616e 6775 6167 6544 6574 6563 746f 722c  anguageDetector,
+00000070: 204c 616e 6775 6167 6544 6574 6563 746f   LanguageDetecto
+00000080: 7242 7569 6c64 6572 0a66 726f 6d20 7472  rBuilder.from tr
+00000090: 616e 736c 6174 6f72 732e 7365 7276 6572  anslators.server
+000000a0: 2069 6d70 6f72 7420 5472 616e 736c 6174   import Translat
+000000b0: 6f72 4572 726f 720a 0a6c 6f67 6765 7220  orError..logger 
+000000c0: 3d20 6c6f 6767 696e 672e 6765 744c 6f67  = logging.getLog
+000000d0: 6765 7228 5f5f 6e61 6d65 5f5f 290a 0a0a  ger(__name__)...
+000000e0: 636c 6173 7320 5472 616e 736c 6174 6f72  class Translator
+000000f0: 5365 7276 6963 653a 0a20 2020 205f 7472  Service:.    _tr
+00000100: 616e 736c 6174 696f 6e5f 7365 7276 6963  anslation_servic
+00000110: 6573 3a20 4c69 7374 5b73 7472 5d0a 2020  es: List[str].  
+00000120: 2020 5f75 7365 725f 6c61 6e67 7561 6765    _user_language
+00000130: 3a20 7374 720a 2020 2020 5f64 6566 6175  : str.    _defau
+00000140: 6c74 5f6c 616e 6775 6167 655f 746f 5f74  lt_language_to_t
+00000150: 7261 6e73 6c61 7465 5f74 6f3a 2073 7472  ranslate_to: str
+00000160: 0a0a 2020 2020 6465 6620 5f5f 696e 6974  ..    def __init
+00000170: 5f5f 280a 2020 2020 2020 2020 2020 2020  __(.            
+00000180: 7365 6c66 2c0a 2020 2020 2020 2020 2020  self,.          
+00000190: 2020 636f 6d6d 615f 7365 7061 7261 7465    comma_separate
+000001a0: 645f 7472 616e 736c 6174 696f 6e5f 7365  d_translation_se
+000001b0: 7276 6963 6573 3a20 7374 722c 0a20 2020  rvices: str,.   
+000001c0: 2020 2020 2020 2020 2075 7365 725f 6c61           user_la
+000001d0: 6e67 7561 6765 3a20 7374 722c 0a20 2020  nguage: str,.   
+000001e0: 2020 2020 2020 2020 2064 6566 6175 6c74           default
+000001f0: 5f6c 616e 675f 746f 5f74 7261 6e73 6c61  _lang_to_transla
+00000200: 7465 5f74 6f3a 2073 7472 0a20 2020 2029  te_to: str.    )
+00000210: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
+00000220: 2020 7472 616e 736c 6174 696f 6e5f 7365    translation_se
+00000230: 7276 6963 6573 3a20 4c69 7374 5b73 7472  rvices: List[str
+00000240: 5d20 3d20 636f 6d6d 615f 7365 7061 7261  ] = comma_separa
+00000250: 7465 645f 7472 616e 736c 6174 696f 6e5f  ted_translation_
+00000260: 7365 7276 6963 6573 2e73 7472 6970 2829  services.strip()
+00000270: 2e73 706c 6974 2827 2c27 290a 2020 2020  .split(',').    
+00000280: 2020 2020 7365 6c66 2e5f 7472 616e 736c      self._transl
+00000290: 6174 696f 6e5f 7365 7276 6963 6573 203d  ation_services =
+000002a0: 2074 7261 6e73 6c61 7469 6f6e 5f73 6572   translation_ser
+000002b0: 7669 6365 730a 0a20 2020 2020 2020 2073  vices..        s
+000002c0: 656c 662e 5f75 7365 725f 6c61 6e67 7561  elf._user_langua
+000002d0: 6765 203d 2075 7365 725f 6c61 6e67 7561  ge = user_langua
+000002e0: 6765 0a20 2020 2020 2020 2073 656c 662e  ge.        self.
+000002f0: 5f64 6566 6175 6c74 5f6c 616e 6775 6167  _default_languag
+00000300: 655f 746f 5f74 7261 6e73 6c61 7465 5f74  e_to_translate_t
+00000310: 6f20 3d20 6465 6661 756c 745f 6c61 6e67  o = default_lang
+00000320: 5f74 6f5f 7472 616e 736c 6174 655f 746f  _to_translate_to
+00000330: 0a0a 2020 2020 6465 6620 5f5f 6765 745f  ..    def __get_
+00000340: 6c61 6e67 7561 6765 5f74 6f5f 7472 616e  language_to_tran
+00000350: 736c 6174 655f 746f 2873 656c 662c 206c  slate_to(self, l
+00000360: 616e 6775 6167 655f 636f 6465 3a20 7374  anguage_code: st
+00000370: 7229 202d 3e20 7374 723a 0a20 2020 2020  r) -> str:.     
+00000380: 2020 2023 2064 6574 6563 7465 6420 6c61     # detected la
+00000390: 6e67 7561 6765 3a20 6c61 6e67 7561 6765  nguage: language
+000003a0: 2074 6f20 7472 616e 736c 6174 6520 746f   to translate to
+000003b0: 0a20 2020 2020 2020 2074 7261 6e73 6c61  .        transla
+000003c0: 7469 6f6e 5f72 756c 6573 3a20 4469 6374  tion_rules: Dict
+000003d0: 5b73 7472 2c20 7374 725d 203d 207b 0a20  [str, str] = {. 
+000003e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000003f0: 5f64 6566 6175 6c74 5f6c 616e 6775 6167  _default_languag
+00000400: 655f 746f 5f74 7261 6e73 6c61 7465 5f74  e_to_translate_t
+00000410: 6f3a 2073 656c 662e 5f75 7365 725f 6c61  o: self._user_la
+00000420: 6e67 7561 6765 2c0a 2020 2020 2020 2020  nguage,.        
+00000430: 7d0a 2020 2020 2020 2020 6465 6661 756c  }.        defaul
+00000440: 745f 6c61 6e67 7561 6765 5f74 6f5f 7472  t_language_to_tr
+00000450: 616e 736c 6174 655f 746f 3a20 7374 7220  anslate_to: str 
+00000460: 3d20 7365 6c66 2e5f 6465 6661 756c 745f  = self._default_
+00000470: 6c61 6e67 7561 6765 5f74 6f5f 7472 616e  language_to_tran
+00000480: 736c 6174 655f 746f 0a0a 2020 2020 2020  slate_to..      
+00000490: 2020 6c61 6e67 7561 6765 5f74 6f5f 7472    language_to_tr
+000004a0: 616e 736c 6174 655f 746f 3a20 7374 7220  anslate_to: str 
+000004b0: 3d20 7472 616e 736c 6174 696f 6e5f 7275  = translation_ru
+000004c0: 6c65 732e 6765 7428 6c61 6e67 7561 6765  les.get(language
+000004d0: 5f63 6f64 652c 2064 6566 6175 6c74 5f6c  _code, default_l
+000004e0: 616e 6775 6167 655f 746f 5f74 7261 6e73  anguage_to_trans
+000004f0: 6c61 7465 5f74 6f29 0a0a 2020 2020 2020  late_to)..      
+00000500: 2020 6c6f 6767 6572 2e64 6562 7567 2866    logger.debug(f
+00000510: 2257 696c 6c20 7472 616e 736c 6174 6520  "Will translate 
+00000520: 6672 6f6d 207b 6c61 6e67 7561 6765 5f63  from {language_c
+00000530: 6f64 657d 2074 6f20 7b6c 616e 6775 6167  ode} to {languag
+00000540: 655f 746f 5f74 7261 6e73 6c61 7465 5f74  e_to_translate_t
+00000550: 6f7d 2229 0a20 2020 2020 2020 2072 6574  o}").        ret
+00000560: 7572 6e20 6c61 6e67 7561 6765 5f74 6f5f  urn language_to_
+00000570: 7472 616e 736c 6174 655f 746f 0a0a 2020  translate_to..  
+00000580: 2020 6465 6620 7472 616e 736c 6174 6528    def translate(
+00000590: 7365 6c66 2c20 7465 7874 5f74 6f5f 7472  self, text_to_tr
+000005a0: 616e 736c 6174 653a 2073 7472 2920 2d3e  anslate: str) ->
+000005b0: 2073 7472 3a0a 2020 2020 2020 2020 7375   str:.        su
+000005c0: 7070 6f72 7465 645f 6c61 6e67 7561 6765  pported_language
+000005d0: 733a 204c 6973 745b 4c61 6e67 7561 6765  s: List[Language
+000005e0: 5d20 3d20 5b4c 616e 6775 6167 652e 454e  ] = [Language.EN
+000005f0: 474c 4953 482c 204c 616e 6775 6167 652e  GLISH, Language.
+00000600: 5255 5353 4941 4e2c 204c 616e 6775 6167  RUSSIAN, Languag
+00000610: 652e 554b 5241 494e 4941 4e5d 0a0a 2020  e.UKRAINIAN]..  
+00000620: 2020 2020 2020 6c61 6e67 7561 6765 5f64        language_d
+00000630: 6574 6563 746f 723a 204c 616e 6775 6167  etector: Languag
+00000640: 6544 6574 6563 746f 7220 3d20 4c61 6e67  eDetector = Lang
+00000650: 7561 6765 4465 7465 6374 6f72 4275 696c  uageDetectorBuil
+00000660: 6465 722e 6672 6f6d 5f6c 616e 6775 6167  der.from_languag
+00000670: 6573 282a 7375 7070 6f72 7465 645f 6c61  es(*supported_la
+00000680: 6e67 7561 6765 7329 2e62 7569 6c64 2829  nguages).build()
+00000690: 0a20 2020 2020 2020 206c 616e 6775 6167  .        languag
+000006a0: 655f 746f 5f74 7261 6e73 6c61 7465 5f66  e_to_translate_f
+000006b0: 726f 6d3a 2073 7472 203d 206c 616e 6775  rom: str = langu
+000006c0: 6167 655f 6465 7465 6374 6f72 2e64 6574  age_detector.det
+000006d0: 6563 745f 6c61 6e67 7561 6765 5f6f 6628  ect_language_of(
+000006e0: 7465 7874 5f74 6f5f 7472 616e 736c 6174  text_to_translat
+000006f0: 6529 2e6e 616d 652e 6c6f 7765 7228 295b  e).name.lower()[
+00000700: 303a 325d 0a20 2020 2020 2020 206c 6f67  0:2].        log
+00000710: 6765 722e 6465 6275 6728 6622 4465 7465  ger.debug(f"Dete
+00000720: 6374 6564 207b 6c61 6e67 7561 6765 5f74  cted {language_t
+00000730: 6f5f 7472 616e 736c 6174 655f 6672 6f6d  o_translate_from
+00000740: 7d20 6c61 6e67 7561 6765 2066 726f 6d20  } language from 
+00000750: 5c22 7b74 6578 745f 746f 5f74 7261 6e73  \"{text_to_trans
+00000760: 6c61 7465 7d5c 2222 290a 0a20 2020 2020  late}\"")..     
+00000770: 2020 2074 7261 6e73 6c61 7469 6f6e 5f73     translation_s
+00000780: 6572 7669 6365 733a 204c 6973 745b 7374  ervices: List[st
+00000790: 725d 203d 2073 656c 662e 5f74 7261 6e73  r] = self._trans
+000007a0: 6c61 7469 6f6e 5f73 6572 7669 6365 730a  lation_services.
+000007b0: 0a20 2020 2020 2020 206c 616e 6775 6167  .        languag
+000007c0: 655f 746f 5f74 7261 6e73 6c61 7465 5f74  e_to_translate_t
+000007d0: 6f3a 2073 7472 203d 2073 656c 662e 5f5f  o: str = self.__
+000007e0: 6765 745f 6c61 6e67 7561 6765 5f74 6f5f  get_language_to_
+000007f0: 7472 616e 736c 6174 655f 746f 286c 616e  translate_to(lan
+00000800: 6775 6167 655f 746f 5f74 7261 6e73 6c61  guage_to_transla
+00000810: 7465 5f66 726f 6d29 0a0a 2020 2020 2020  te_from)..      
+00000820: 2020 6c6f 6767 6572 2e64 6562 7567 2866    logger.debug(f
+00000830: 2257 696c 6c20 7573 6520 7468 6973 206c  "Will use this l
+00000840: 6973 7420 6f66 2074 7261 6e73 6c61 7469  ist of translati
+00000850: 6f6e 2073 6572 7669 6365 733a 207b 7472  on services: {tr
+00000860: 616e 736c 6174 696f 6e5f 7365 7276 6963  anslation_servic
+00000870: 6573 7d22 290a 2020 2020 2020 2020 666f  es}").        fo
+00000880: 7220 7472 616e 736c 6174 696f 6e5f 7365  r translation_se
+00000890: 7276 6963 6520 696e 2074 7261 6e73 6c61  rvice in transla
+000008a0: 7469 6f6e 5f73 6572 7669 6365 733a 0a20  tion_services:. 
+000008b0: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
+000008c0: 722e 6465 6275 6728 6622 5472 7969 6e67  r.debug(f"Trying
+000008d0: 2074 6f20 7472 616e 736c 6174 6520 7573   to translate us
+000008e0: 696e 6720 7b74 7261 6e73 6c61 7469 6f6e  ing {translation
+000008f0: 5f73 6572 7669 6365 7d2e 2e22 290a 2020  _service}..").  
+00000900: 2020 2020 2020 2020 2020 7472 793a 0a20            try:. 
+00000910: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+00000920: 7261 6e73 6c61 7469 6f6e 3a20 7374 7220  ranslation: str 
+00000930: 3d20 7472 616e 736c 6174 6f72 732e 7472  = translators.tr
+00000940: 616e 736c 6174 655f 7465 7874 280a 2020  anslate_text(.  
+00000950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000960: 2020 7175 6572 795f 7465 7874 3d74 6578    query_text=tex
+00000970: 745f 746f 5f74 7261 6e73 6c61 7465 2c0a  t_to_translate,.
+00000980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000990: 2020 2020 7472 616e 736c 6174 6f72 3d74      translator=t
+000009a0: 7261 6e73 6c61 7469 6f6e 5f73 6572 7669  ranslation_servi
+000009b0: 6365 2c0a 2020 2020 2020 2020 2020 2020  ce,.            
+000009c0: 2020 2020 2020 2020 6672 6f6d 5f6c 616e          from_lan
+000009d0: 6775 6167 653d 6c61 6e67 7561 6765 5f74  guage=language_t
+000009e0: 6f5f 7472 616e 736c 6174 655f 6672 6f6d  o_translate_from
+000009f0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00000a00: 2020 2020 2020 746f 5f6c 616e 6775 6167        to_languag
+00000a10: 653d 6c61 6e67 7561 6765 5f74 6f5f 7472  e=language_to_tr
+00000a20: 616e 736c 6174 655f 746f 2c0a 2020 2020  anslate_to,.    
+00000a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000a40: 6966 5f75 7365 5f70 7265 6163 6365 6c65  if_use_preaccele
+00000a50: 7261 7469 6f6e 3d46 616c 7365 0a20 2020  ration=False.   
+00000a60: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
+00000a70: 2020 2020 2020 2020 2020 2065 7863 6570             excep
+00000a80: 7420 5472 616e 736c 6174 6f72 4572 726f  t TranslatorErro
+00000a90: 7220 6173 2065 3a0a 2020 2020 2020 2020  r as e:.        
+00000aa0: 2020 2020 2020 2020 6c6f 6767 6572 2e77          logger.w
+00000ab0: 6172 6e69 6e67 2866 227b 657d 206f 6363  arning(f"{e} occ
+00000ac0: 7572 7265 6420 7768 656e 2074 7279 696e  urred when tryin
+00000ad0: 6720 746f 2074 7261 6e73 6c61 7465 205c  g to translate \
+00000ae0: 227b 7465 7874 5f74 6f5f 7472 616e 736c  "{text_to_transl
+00000af0: 6174 657d 5c22 2022 0a20 2020 2020 2020  ate}\" ".       
+00000b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000b10: 2020 2020 2020 2020 6622 6672 6f6d 205c          f"from \
+00000b20: 227b 6c61 6e67 7561 6765 5f74 6f5f 7472  "{language_to_tr
+00000b30: 616e 736c 6174 655f 6672 6f6d 7d5c 2220  anslate_from}\" 
+00000b40: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+00000b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000b60: 2066 2274 6f20 5c22 7b6c 616e 6775 6167   f"to \"{languag
+00000b70: 655f 746f 5f74 7261 6e73 6c61 7465 5f74  e_to_translate_t
+00000b80: 6f7d 5c22 2022 0a20 2020 2020 2020 2020  o}\" ".         
+00000b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000ba0: 2020 2020 2020 6622 7573 696e 6720 7b74        f"using {t
+00000bb0: 7261 6e73 6c61 7469 6f6e 5f73 6572 7669  ranslation_servi
+00000bc0: 6365 7d20 7365 7276 6963 6522 290a 2020  ce} service").  
+00000bd0: 2020 2020 2020 2020 2020 2020 2020 636f                co
+00000be0: 6e74 696e 7565 0a20 2020 2020 2020 2020  ntinue.         
+00000bf0: 2020 2065 7863 6570 7420 4578 6365 7074     except Except
+00000c00: 696f 6e20 6173 2065 3a0a 2020 2020 2020  ion as e:.      
+00000c10: 2020 2020 2020 2020 2020 6c6f 6767 6572            logger
+00000c20: 2e77 6172 6e69 6e67 2866 2241 6e20 756e  .warning(f"An un
+00000c30: 6578 7065 6374 6564 2065 7272 6f72 207b  expected error {
+00000c40: 657d 206f 6363 7572 7265 6420 7768 656e  e} occurred when
+00000c50: 2074 7279 696e 6720 746f 2074 7261 6e73   trying to trans
+00000c60: 6c61 7465 205c 227b 7465 7874 5f74 6f5f  late \"{text_to_
+00000c70: 7472 616e 736c 6174 657d 5c22 2022 0a20  translate}\" ". 
+00000c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000c90: 2020 2020 2020 2020 2020 2020 2020 6622                f"
+00000ca0: 6672 6f6d 205c 227b 6c61 6e67 7561 6765  from \"{language
+00000cb0: 5f74 6f5f 7472 616e 736c 6174 655f 6672  _to_translate_fr
+00000cc0: 6f6d 7d5c 2220 220a 2020 2020 2020 2020  om}\" ".        
+00000cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000ce0: 2020 2020 2020 2066 2274 6f20 5c22 7b6c         f"to \"{l
+00000cf0: 616e 6775 6167 655f 746f 5f74 7261 6e73  anguage_to_trans
+00000d00: 6c61 7465 5f74 6f7d 5c22 2022 0a20 2020  late_to}\" ".   
+00000d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000d20: 2020 2020 2020 2020 2020 2020 6622 7573              f"us
+00000d30: 696e 6720 7b74 7261 6e73 6c61 7469 6f6e  ing {translation
+00000d40: 5f73 6572 7669 6365 7d20 7365 7276 6963  _service} servic
+00000d50: 6522 290a 2020 2020 2020 2020 2020 2020  e").            
+00000d60: 2020 2020 636f 6e74 696e 7565 0a0a 2020      continue..  
+00000d70: 2020 2020 2020 2020 2020 6c6f 6767 6572            logger
+00000d80: 2e69 6e66 6f28 6622 5375 6363 6573 7366  .info(f"Successf
+00000d90: 756c 6c79 2074 7261 6e73 6c61 7465 6420  ully translated 
+00000da0: 5c22 7b74 6578 745f 746f 5f74 7261 6e73  \"{text_to_trans
+00000db0: 6c61 7465 7d5c 2220 746f 205c 227b 7472  late}\" to \"{tr
+00000dc0: 616e 736c 6174 696f 6e7d 5c22 2022 0a20  anslation}\" ". 
+00000dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000de0: 2020 2020 2020 2066 2266 726f 6d20 5c22         f"from \"
+00000df0: 7b6c 616e 6775 6167 655f 746f 5f74 7261  {language_to_tra
+00000e00: 6e73 6c61 7465 5f66 726f 6d7d 5c22 2022  nslate_from}\" "
+00000e10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000e20: 2020 2020 2020 2020 2066 2274 6f20 5c22           f"to \"
+00000e30: 7b6c 616e 6775 6167 655f 746f 5f74 7261  {language_to_tra
+00000e40: 6e73 6c61 7465 5f74 6f7d 5c22 2022 0a20  nslate_to}\" ". 
+00000e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000e60: 2020 2020 2020 2066 2275 7369 6e67 207b         f"using {
+00000e70: 7472 616e 736c 6174 696f 6e5f 7365 7276  translation_serv
+00000e80: 6963 657d 2229 0a20 2020 2020 2020 2020  ice}").         
+00000e90: 2020 2062 7265 616b 0a20 2020 2020 2020     break.       
+00000ea0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+00000eb0: 2020 206c 6f67 6765 722e 7761 726e 696e     logger.warnin
+00000ec0: 6728 6622 436f 756c 646e 2774 2074 7261  g(f"Couldn't tra
+00000ed0: 6e73 6c61 7465 207b 7465 7874 5f74 6f5f  nslate {text_to_
+00000ee0: 7472 616e 736c 6174 657d 2066 726f 6d20  translate} from 
+00000ef0: 7b6c 616e 6775 6167 655f 746f 5f74 7261  {language_to_tra
+00000f00: 6e73 6c61 7465 5f66 726f 6d7d 2022 0a20  nslate_from} ". 
+00000f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000f20: 2020 2020 2020 2020 2020 6622 746f 207b            f"to {
+00000f30: 6c61 6e67 7561 6765 5f74 6f5f 7472 616e  language_to_tran
+00000f40: 736c 6174 655f 746f 7d20 7573 696e 6720  slate_to} using 
+00000f50: 616e 7920 7365 7276 6963 6522 290a 2020  any service").  
+00000f60: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+00000f70: 5472 616e 736c 6174 6f72 4572 726f 7228  TranslatorError(
+00000f80: 2241 6c6c 2074 6865 2073 7065 6369 6669  "All the specifi
+00000f90: 6564 2074 7261 6e73 6c61 7469 6f6e 2073  ed translation s
+00000fa0: 6572 7669 6365 7320 6572 726f 7265 6420  ervices errored 
+00000fb0: 6f75 7422 290a 0a20 2020 2020 2020 2072  out")..        r
+00000fc0: 6574 7572 6e20 7472 616e 736c 6174 696f  eturn translatio
+00000fd0: 6e0a                                     n.
```

### Comparing `suskabot-0.1.4/suskabot/services/youtube_downloader.py` & `suskabot-0.1.5/suskabot/services/youtube_downloader.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from io import BytesIO
 
 from typing import Optional, Callable
 
 from pytube import YouTube, StreamQuery, Stream
 from pytube.exceptions import RegexMatchError, VideoUnavailable
 
-from utils import utils
+from suskabot.utils import utils
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
 class VideoTooLarge(Exception):
     """Raise if a video file size exceeds set limits"""
 
@@ -47,15 +47,15 @@
             save_to_drive: bool
     ) -> None:
         self._minimum_video_resolution = min_video_res
         self._maximum_video_resolution = max_video_res
         self._file_size_limit_mb = file_size_limit_mb
         self._save_to_drive = save_to_drive
 
-    def __get_best_quality_stream_under_limits(self, video_streams: StreamQuery) -> Optional[Stream]:
+    def _get_best_quality_stream_under_limits(self, video_streams: StreamQuery) -> Optional[Stream]:
         ordered_video_streams: StreamQuery = video_streams.order_by("resolution").desc()
         logger.debug(f"Trying to find a stream under {self._file_size_limit_mb} MB, between "
                      f"{self._minimum_video_resolution}p and {self._maximum_video_resolution}p")
 
         video_stream: Stream
         for video_stream in ordered_video_streams:
             video_resolution: int = utils.pytube_video_resolution_to_int(video_stream.resolution)
@@ -82,15 +82,15 @@
             raise e
         except VideoUnavailable as e:
             raise e
 
         progressive_video_streams: StreamQuery = video_data.streams.filter(progressive=True)
         logger.debug(f"Found progressive streams:\n{progressive_video_streams}")
 
-        video_stream: Stream | None = self.__get_best_quality_stream_under_limits(progressive_video_streams)
+        video_stream: Stream | None = self._get_best_quality_stream_under_limits(progressive_video_streams)
         logger.debug(f"Selected video stream:\n{video_stream}")
 
         if not video_stream:
             raise VideoTooLarge(f"Can't download videos larger than {self._file_size_limit_mb}MB")
 
         return video_stream
```

### Comparing `suskabot-0.1.4/suskabot/utils/utils.py` & `suskabot-0.1.5/suskabot/utils/utils.py`

 * *Files identical despite different names*

