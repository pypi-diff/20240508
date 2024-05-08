# Comparing `tmp/nonebot_plugin_bilichat-5.9.2.tar.gz` & `tmp/nonebot_plugin_bilichat-5.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_bilichat-5.9.2.tar", last modified: Sat May  4 06:53:07 2024, max compression
+gzip compressed data, was "nonebot_plugin_bilichat-5.9.3.tar", last modified: Mon May  6 09:45:26 2024, max compression
```

## Comparing `nonebot_plugin_bilichat-5.9.2.tar` & `nonebot_plugin_bilichat-5.9.3.tar`

### file list

```diff
@@ -1,81 +1,81 @@
--rw-r--r--   0        0        0    34523 2024-05-04 06:53:03.549994 nonebot_plugin_bilichat-5.9.2/LICENSE
--rw-r--r--   0        0        0    18173 2024-05-04 06:53:03.549994 nonebot_plugin_bilichat-5.9.2/README.md
--rw-r--r--   0        0        0     2718 2024-05-04 06:53:03.569994 nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/__init__.py
--rw-r--r--   0        0        0     1120 2024-05-04 06:53:03.569994 nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/api/__init__.py
--rw-r--r--   0        0        0      740 2024-05-04 06:53:03.569994 nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/api/base.py
--rw-r--r--   0        0        0     2176 2024-05-04 06:53:03.569994 nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/api/bilibili_auth.py
--rw-r--r--   0        0        0     1622 2024-05-04 06:53:03.569994 nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/api/subs_config.py
--rw-r--r--   0        0        0     2655 2024-05-04 06:53:03.569994 nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/api/webui.py
--rw-r--r--   0        0        0     7996 2024-05-04 06:53:03.569994 nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/base_content_parsing.py
--rw-r--r--   0        0        0       60 2024-05-04 06:53:03.569994 nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/commands/__init__.py
--rw-r--r--   0        0        0     1280 2024-05-04 06:53:03.569994 nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/commands/auto_delete_subs.py
--rw-r--r--   0        0        0     1063 2024-05-04 06:53:03.569994 nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/commands/base.py
--rw-r--r--   0        0        0     4200 2024-05-04 06:53:03.569994 nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/commands/functions.py
--rw-r--r--   0        0        0     3848 2024-05-04 06:53:03.569994 nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/commands/login.py
--rw-r--r--   0        0        0     5196 2024-05-04 06:53:03.569994 nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/commands/subs.py
--rw-r--r--   0        0        0     4996 2024-05-04 06:53:03.569994 nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/commands/subs_cfg.py
--rw-r--r--   0        0        0     9296 2024-05-04 06:53:03.569994 nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/config.py
--rw-r--r--   0        0        0       81 2024-05-04 06:53:03.569994 nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/content/__init__.py
--rw-r--r--   0        0        0     3568 2024-05-04 06:53:03.569994 nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/content/column.py
--rw-r--r--   0        0        0     6385 2024-05-04 06:53:03.569994 nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/content/dynamic.py
--rw-r--r--   0        0        0     4462 2024-05-04 06:53:03.569994 nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/content/video.py
--rw-r--r--   0        0        0      494 2024-05-04 06:53:03.569994 nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/lib/b23_extract.py
--rw-r--r--   0        0        0     6142 2024-05-04 06:53:03.569994 nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/lib/bcut_asr.py
--rw-r--r--   0        0        0      506 2024-05-04 06:53:03.569994 nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/lib/bilibili_request/__init__.py
--rw-r--r--   0        0        0     2346 2024-05-04 06:53:03.569994 nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/lib/bilibili_request/auth.py
--rw-r--r--   0        0        0      966 2024-05-04 06:53:03.569994 nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/lib/bilibili_request/gRPC.py
--rw-r--r--   0        0        0     2653 2024-05-04 06:53:03.569994 nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/lib/bilibili_request/restAPI.py
--rw-r--r--   0        0        0     2657 2024-05-04 06:53:03.569994 nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/lib/browser.py
--rw-r--r--   0        0        0      456 2024-05-04 06:53:03.573994 nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/lib/cache/__init__.py
--rw-r--r--   0        0        0      366 2024-05-04 06:53:03.573994 nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/lib/cache/cache.py
--rw-r--r--   0        0        0      871 2024-05-04 06:53:03.573994 nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/lib/cache/json_cache.py
--rw-r--r--   0        0        0      531 2024-05-04 06:53:03.573994 nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/lib/cache/mongo_cache.py
--rw-r--r--   0        0        0      521 2024-05-04 06:53:03.573994 nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/lib/draw/__init__.py
--rw-r--r--   0        0        0      217 2024-05-04 06:53:03.573994 nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/lib/draw/column/__init__.py
--rw-r--r--   0        0        0     3379 2024-05-04 06:53:03.573994 nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/lib/draw/column/browser_shot.py
--rw-r--r--   0        0        0      220 2024-05-04 06:53:03.573994 nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/lib/draw/dynamic/__init__.py
--rw-r--r--   0        0        0     5145 2024-05-04 06:53:03.573994 nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/lib/draw/dynamic/browser_shot.py
--rw-r--r--   0        0        0     1136 2024-05-04 06:53:03.573994 nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/lib/draw/dynamic/dynamicrender.py
--rw-r--r--   0        0        0     7275 2024-05-04 06:53:03.573994 nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/lib/draw/video/__init__.py
--rw-r--r--   0        0        0     6326 2024-05-04 06:53:03.573994 nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/lib/draw/video/bbot_default.py
--rw-r--r--   0        0        0     3040 2024-05-04 06:53:03.573994 nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/lib/draw/video/style_blue.py
--rw-r--r--   0        0        0     3187 2024-05-04 06:53:03.573994 nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/lib/fetch_dynamic.py
--rw-r--r--   0        0        0     3376 2024-05-04 06:53:03.573994 nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/lib/fonts_provider.py
--rw-r--r--   0        0        0      525 2024-05-04 06:53:03.573994 nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/lib/store.py
--rw-r--r--   0        0        0     3091 2024-05-04 06:53:03.573994 nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/lib/strings.py
--rw-r--r--   0        0        0     3329 2024-05-04 06:53:03.573994 nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/lib/text_to_image.py
--rw-r--r--   0        0        0     1701 2024-05-04 06:53:03.573994 nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/lib/tools.py
--rw-r--r--   0        0        0     1739 2024-05-04 06:53:03.573994 nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/lib/uid_extract.py
--rw-r--r--   0        0        0     3988 2024-05-04 06:53:03.573994 nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/lib/video_subtitle.py
--rw-r--r--   0        0        0      552 2024-05-04 06:53:03.573994 nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/model/api/__init__.py
--rw-r--r--   0        0        0      184 2024-05-04 06:53:03.573994 nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/model/api/bilibili_auth.py
--rw-r--r--   0        0        0      809 2024-05-04 06:53:03.573994 nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/model/api/subs_config.py
--rw-r--r--   0        0        0      532 2024-05-04 06:53:03.573994 nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/model/arguments.py
--rw-r--r--   0        0        0     3030 2024-05-04 06:53:03.573994 nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/model/bcut_asr.py
--rw-r--r--   0        0        0     1326 2024-05-04 06:53:03.573994 nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/model/bilibili/live.py
--rw-r--r--   0        0        0     1016 2024-05-04 06:53:03.573994 nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/model/bilibili/summary.py
--rw-r--r--   0        0        0      596 2024-05-04 06:53:03.573994 nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/model/const.py
--rw-r--r--   0        0        0     1163 2024-05-04 06:53:03.573994 nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/model/exception.py
--rw-r--r--   0        0        0      291 2024-05-04 06:53:03.573994 nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/model/openai.py
--rw-r--r--   0        0        0      270 2024-05-04 06:53:03.573994 nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/optional.py
--rw-r--r--   0        0        0     9390 2024-05-04 06:53:03.573994 nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/static/browser/mobile_style.js
--rw-r--r--   0        0        0     1187 2024-05-04 06:53:03.573994 nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/static/style_blue/assets/business.png
--rw-r--r--   0        0        0     1200 2024-05-04 06:53:03.573994 nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/static/style_blue/assets/personal.png
--rw-r--r--   0        0        0    93905 2024-05-04 06:53:03.573994 nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/static/style_blue/assets/video_bottom.png
--rw-r--r--   0        0        0     7545 2024-05-04 06:53:03.573994 nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/static/style_blue/video-details.html
--rw-r--r--   0        0        0     5777 2024-05-04 06:53:03.573994 nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/static/summary/bilibili.png
--rw-r--r--   0        0        0     2098 2024-05-04 06:53:03.573994 nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/static/summary/index.html
--rw-r--r--   0        0        0    47433 2024-05-04 06:53:03.573994 nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/static/summary/marked.min.js
--rw-r--r--   0        0        0    59199 2024-05-04 06:53:03.573994 nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/static/summary/openai.png
--rw-r--r--   0        0        0     9556 2024-05-04 06:53:03.573994 nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/static/upload-webui.html
--rw-r--r--   0        0        0   300664 2024-05-04 06:53:03.573994 nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/static/webui.tar.gz
--rw-r--r--   0        0        0     3111 2024-05-04 06:53:03.573994 nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/subscribe/__init__.py
--rw-r--r--   0        0        0     7187 2024-05-04 06:53:03.573994 nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/subscribe/dynamic.py
--rw-r--r--   0        0        0     4023 2024-05-04 06:53:03.573994 nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/subscribe/live.py
--rw-r--r--   0        0        0    16430 2024-05-04 06:53:03.573994 nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/subscribe/manager.py
--rw-r--r--   0        0        0      478 2024-05-04 06:53:03.573994 nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/summary/__init__.py
--rw-r--r--   0        0        0     4894 2024-05-04 06:53:03.573994 nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/summary/openai.py
--rw-r--r--   0        0        0     2243 2024-05-04 06:53:03.573994 nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/summary/openai_summarise.py
--rw-r--r--   0        0        0     1578 2024-05-04 06:53:03.573994 nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/wordcloud.py
--rw-r--r--   0        0        0     1647 2024-05-04 06:53:07.865996 nonebot_plugin_bilichat-5.9.2/pyproject.toml
--rw-r--r--   0        0        0    19870 1970-01-01 00:00:00.000000 nonebot_plugin_bilichat-5.9.2/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-05-06 09:45:23.435805 nonebot_plugin_bilichat-5.9.3/LICENSE
+-rw-r--r--   0        0        0    18166 2024-05-06 09:45:23.435805 nonebot_plugin_bilichat-5.9.3/README.md
+-rw-r--r--   0        0        0     2718 2024-05-06 09:45:23.455805 nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/__init__.py
+-rw-r--r--   0        0        0     1120 2024-05-06 09:45:23.455805 nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/api/__init__.py
+-rw-r--r--   0        0        0      740 2024-05-06 09:45:23.455805 nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/api/base.py
+-rw-r--r--   0        0        0     2176 2024-05-06 09:45:23.455805 nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/api/bilibili_auth.py
+-rw-r--r--   0        0        0     1622 2024-05-06 09:45:23.455805 nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/api/subs_config.py
+-rw-r--r--   0        0        0     2655 2024-05-06 09:45:23.455805 nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/api/webui.py
+-rw-r--r--   0        0        0     8002 2024-05-06 09:45:23.455805 nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/base_content_parsing.py
+-rw-r--r--   0        0        0       60 2024-05-06 09:45:23.455805 nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/commands/__init__.py
+-rw-r--r--   0        0        0     1280 2024-05-06 09:45:23.455805 nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/commands/auto_delete_subs.py
+-rw-r--r--   0        0        0     1063 2024-05-06 09:45:23.455805 nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/commands/base.py
+-rw-r--r--   0        0        0     4200 2024-05-06 09:45:23.455805 nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/commands/functions.py
+-rw-r--r--   0        0        0     3848 2024-05-06 09:45:23.455805 nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/commands/login.py
+-rw-r--r--   0        0        0     5196 2024-05-06 09:45:23.455805 nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/commands/subs.py
+-rw-r--r--   0        0        0     4996 2024-05-06 09:45:23.455805 nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/commands/subs_cfg.py
+-rw-r--r--   0        0        0     9296 2024-05-06 09:45:23.455805 nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/config.py
+-rw-r--r--   0        0        0       81 2024-05-06 09:45:23.455805 nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/content/__init__.py
+-rw-r--r--   0        0        0     3568 2024-05-06 09:45:23.455805 nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/content/column.py
+-rw-r--r--   0        0        0     6385 2024-05-06 09:45:23.455805 nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/content/dynamic.py
+-rw-r--r--   0        0        0     4462 2024-05-06 09:45:23.455805 nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/content/video.py
+-rw-r--r--   0        0        0      494 2024-05-06 09:45:23.455805 nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/lib/b23_extract.py
+-rw-r--r--   0        0        0     6142 2024-05-06 09:45:23.455805 nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/lib/bcut_asr.py
+-rw-r--r--   0        0        0      506 2024-05-06 09:45:23.455805 nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/lib/bilibili_request/__init__.py
+-rw-r--r--   0        0        0     2346 2024-05-06 09:45:23.455805 nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/lib/bilibili_request/auth.py
+-rw-r--r--   0        0        0      966 2024-05-06 09:45:23.455805 nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/lib/bilibili_request/gRPC.py
+-rw-r--r--   0        0        0     2653 2024-05-06 09:45:23.455805 nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/lib/bilibili_request/restAPI.py
+-rw-r--r--   0        0        0     2657 2024-05-06 09:45:23.455805 nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/lib/browser.py
+-rw-r--r--   0        0        0      456 2024-05-06 09:45:23.455805 nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/lib/cache/__init__.py
+-rw-r--r--   0        0        0      366 2024-05-06 09:45:23.455805 nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/lib/cache/cache.py
+-rw-r--r--   0        0        0      871 2024-05-06 09:45:23.455805 nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/lib/cache/json_cache.py
+-rw-r--r--   0        0        0      531 2024-05-06 09:45:23.455805 nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/lib/cache/mongo_cache.py
+-rw-r--r--   0        0        0      521 2024-05-06 09:45:23.455805 nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/lib/draw/__init__.py
+-rw-r--r--   0        0        0      217 2024-05-06 09:45:23.455805 nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/lib/draw/column/__init__.py
+-rw-r--r--   0        0        0     3255 2024-05-06 09:45:23.455805 nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/lib/draw/column/browser_shot.py
+-rw-r--r--   0        0        0      220 2024-05-06 09:45:23.455805 nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/lib/draw/dynamic/__init__.py
+-rw-r--r--   0        0        0     4990 2024-05-06 09:45:23.455805 nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/lib/draw/dynamic/browser_shot.py
+-rw-r--r--   0        0        0     1136 2024-05-06 09:45:23.455805 nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/lib/draw/dynamic/dynamicrender.py
+-rw-r--r--   0        0        0     7275 2024-05-06 09:45:23.455805 nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/lib/draw/video/__init__.py
+-rw-r--r--   0        0        0     6326 2024-05-06 09:45:23.455805 nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/lib/draw/video/bbot_default.py
+-rw-r--r--   0        0        0     3040 2024-05-06 09:45:23.455805 nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/lib/draw/video/style_blue.py
+-rw-r--r--   0        0        0     3187 2024-05-06 09:45:23.455805 nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/lib/fetch_dynamic.py
+-rw-r--r--   0        0        0     3376 2024-05-06 09:45:23.455805 nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/lib/fonts_provider.py
+-rw-r--r--   0        0        0      525 2024-05-06 09:45:23.455805 nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/lib/store.py
+-rw-r--r--   0        0        0     3091 2024-05-06 09:45:23.455805 nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/lib/strings.py
+-rw-r--r--   0        0        0     3329 2024-05-06 09:45:23.455805 nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/lib/text_to_image.py
+-rw-r--r--   0        0        0     1701 2024-05-06 09:45:23.455805 nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/lib/tools.py
+-rw-r--r--   0        0        0     1739 2024-05-06 09:45:23.455805 nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/lib/uid_extract.py
+-rw-r--r--   0        0        0     3988 2024-05-06 09:45:23.455805 nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/lib/video_subtitle.py
+-rw-r--r--   0        0        0      552 2024-05-06 09:45:23.455805 nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/model/api/__init__.py
+-rw-r--r--   0        0        0      184 2024-05-06 09:45:23.455805 nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/model/api/bilibili_auth.py
+-rw-r--r--   0        0        0      809 2024-05-06 09:45:23.455805 nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/model/api/subs_config.py
+-rw-r--r--   0        0        0      532 2024-05-06 09:45:23.455805 nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/model/arguments.py
+-rw-r--r--   0        0        0     3030 2024-05-06 09:45:23.455805 nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/model/bcut_asr.py
+-rw-r--r--   0        0        0     1326 2024-05-06 09:45:23.455805 nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/model/bilibili/live.py
+-rw-r--r--   0        0        0     1016 2024-05-06 09:45:23.455805 nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/model/bilibili/summary.py
+-rw-r--r--   0        0        0      596 2024-05-06 09:45:23.455805 nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/model/const.py
+-rw-r--r--   0        0        0     1163 2024-05-06 09:45:23.455805 nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/model/exception.py
+-rw-r--r--   0        0        0      291 2024-05-06 09:45:23.455805 nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/model/openai.py
+-rw-r--r--   0        0        0      270 2024-05-06 09:45:23.455805 nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/optional.py
+-rw-r--r--   0        0        0     9390 2024-05-06 09:45:23.455805 nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/static/browser/mobile_style.js
+-rw-r--r--   0        0        0     1187 2024-05-06 09:45:23.455805 nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/static/style_blue/assets/business.png
+-rw-r--r--   0        0        0     1200 2024-05-06 09:45:23.455805 nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/static/style_blue/assets/personal.png
+-rw-r--r--   0        0        0    93905 2024-05-06 09:45:23.455805 nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/static/style_blue/assets/video_bottom.png
+-rw-r--r--   0        0        0     7545 2024-05-06 09:45:23.459805 nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/static/style_blue/video-details.html
+-rw-r--r--   0        0        0     5777 2024-05-06 09:45:23.459805 nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/static/summary/bilibili.png
+-rw-r--r--   0        0        0     2098 2024-05-06 09:45:23.459805 nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/static/summary/index.html
+-rw-r--r--   0        0        0    47433 2024-05-06 09:45:23.459805 nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/static/summary/marked.min.js
+-rw-r--r--   0        0        0    59199 2024-05-06 09:45:23.459805 nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/static/summary/openai.png
+-rw-r--r--   0        0        0     9556 2024-05-06 09:45:23.459805 nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/static/upload-webui.html
+-rw-r--r--   0        0        0   300664 2024-05-06 09:45:23.459805 nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/static/webui.tar.gz
+-rw-r--r--   0        0        0     3111 2024-05-06 09:45:23.459805 nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/subscribe/__init__.py
+-rw-r--r--   0        0        0     7187 2024-05-06 09:45:23.459805 nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/subscribe/dynamic.py
+-rw-r--r--   0        0        0     4023 2024-05-06 09:45:23.459805 nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/subscribe/live.py
+-rw-r--r--   0        0        0    16430 2024-05-06 09:45:23.459805 nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/subscribe/manager.py
+-rw-r--r--   0        0        0      478 2024-05-06 09:45:23.459805 nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/summary/__init__.py
+-rw-r--r--   0        0        0     4894 2024-05-06 09:45:23.459805 nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/summary/openai.py
+-rw-r--r--   0        0        0     2243 2024-05-06 09:45:23.459805 nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/summary/openai_summarise.py
+-rw-r--r--   0        0        0     1578 2024-05-06 09:45:23.459805 nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/wordcloud.py
+-rw-r--r--   0        0        0     1622 2024-05-06 09:45:26.967847 nonebot_plugin_bilichat-5.9.3/pyproject.toml
+-rw-r--r--   0        0        0    19863 1970-01-01 00:00:00.000000 nonebot_plugin_bilichat-5.9.3/PKG-INFO
```

### Comparing `nonebot_plugin_bilichat-5.9.2/LICENSE` & `nonebot_plugin_bilichat-5.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.9.2/README.md` & `nonebot_plugin_bilichat-5.9.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
   <img alt="PyPI - Downloads" src="https://img.shields.io/pypi/dm/nonebot-plugin-bilichat">
 </a>
 
 <a href="https://pypi.python.org/pypi/nonebot-plugin-bilichat">
     <img src="https://img.shields.io/pypi/v/nonebot-plugin-bilichat.svg" alt="pypi">
 </a>
 
-<img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">
+<img src="https://img.shields.io/badge/python-3.10+-blue.svg" alt="python">
 
 <a href="https://pdm.fming.dev">
     <img src="https://img.shields.io/badge/pdm-managed-blueviolet" alt="pdm-managed">
 </a>
 
 <a href="https://github.com/psf/black">
     <img src="https://img.shields.io/badge/code%20style-black-000000.svg" alt="Code style: black">
@@ -325,15 +325,15 @@
 |    unsub     |  主人  |  群聊  |      UP 主的昵称或 UID，或 `all`       |         移除订阅，all 时为全移除         |
 |    check     | 无限制 |  群聊  |       UP 主的昵称或 UID，或留空        |    查看本群订阅列表或指定 UP 主的配置    |
 |    reset     |  主人  |  群聊  |      UP 主的昵称或 UID，或 `all`       | 重置指定 UP 主的推送配置，all 时为全重置 |
 |    atall     |  主人  |  群聊  | UP 主的昵称或 UID `全局` `动态` `直播` |           设置是否 at 全体成员           |
 |   dynamic    |  主人  |  群聊  |           UP 主的昵称或 UID            |         是否开启该 UP 的动态通知         |
 |     live     |  主人  |  群聊  |           UP 主的昵称或 UID            |         是否开启该 UP 的直播通知         |
 | checkdynamic | 无限制 | 无限制 |           UP 主的昵称或 UID            |       查看指定 UP 主的最新一条动态       |
-|    fetch     | 无限制 | 无限制 | 视频或动态 ID，或回复包含此内容的消息  |       解析动态包含的图片或视频直链       |
+|    fetch     | 无限制 | 无限制 |    动态 ID，或回复包含此内容的消息     |            解析动态包含的图片            |
 |  checklogin  |  主人  | 无限制 |                   无                   |         查看当前已登录的全部账号         |
 |   qrlogin    |  主人  | 无限制 |                   无                   |      使用二维码登录 B 站，防止风控       |
 |    logout    |  主人  | 无限制 |               账号的 UID               |              登出指定的账号              |
 
 ## 🙏 感谢
 
 在此感谢以下开发者(项目)对本项目做出的贡献：
```

#### html2text {}

```diff
@@ -169,19 +169,19 @@
 ä¸»äºº | ç¾¤è | UP ä¸»çæµç§°æ UIDï¼æ `all` | éç½®æå® UP
 ä¸»çæ¨ééç½®ï¼all æ¶ä¸ºå¨éç½® | | atall | ä¸»äºº | ç¾¤è | UP
 ä¸»çæµç§°æ UID `å¨å±` `å¨æ` `ç´æ­` | è®¾ç½®æ¯å¦ at å¨ä½æå |
 | dynamic | ä¸»äºº | ç¾¤è | UP ä¸»çæµç§°æ UID | æ¯å¦å¼å¯è¯¥ UP
 çå¨æéç¥ | | live | ä¸»äºº | ç¾¤è | UP ä¸»çæµç§°æ UID |
 æ¯å¦å¼å¯è¯¥ UP çç´æ­éç¥ | | checkdynamic | æ éå¶ | æ éå¶ |
 UP ä¸»çæµç§°æ UID | æ¥çæå® UP ä¸»çææ°ä¸æ¡å¨æ | | fetch |
-æ éå¶ | æ éå¶ | è§é¢æå¨æ IDï¼æåå¤åå«æ­¤åå®¹çæ¶æ¯
-| è§£æå¨æåå«çå¾çæè§é¢ç´é¾ | | checklogin | ä¸»äºº |
-æ éå¶ | æ  | æ¥çå½åå·²ç»å½çå¨é¨è´¦å· | | qrlogin | ä¸»äºº |
-æ éå¶ | æ  | ä½¿ç¨äºç»´ç ç»å½ B ç«ï¼é²æ­¢é£æ§ | | logout |
-ä¸»äºº | æ éå¶ | è´¦å·ç UID | ç»åºæå®çè´¦å· | ## ð æè°¢
+æ éå¶ | æ éå¶ | å¨æ IDï¼æåå¤åå«æ­¤åå®¹çæ¶æ¯ |
+è§£æå¨æåå«çå¾ç | | checklogin | ä¸»äºº | æ éå¶ | æ  |
+æ¥çå½åå·²ç»å½çå¨é¨è´¦å· | | qrlogin | ä¸»äºº | æ éå¶ | æ  |
+ä½¿ç¨äºç»´ç ç»å½ B ç«ï¼é²æ­¢é£æ§ | | logout | ä¸»äºº | æ éå¶ |
+è´¦å·ç UID | ç»åºæå®çè´¦å· | ## ð æè°¢
 å¨æ­¤æè°¢ä»¥ä¸å¼åè(é¡¹ç®)å¯¹æ¬é¡¹ç®ååºçè´¡ç®ï¼ - [BibiGPT]
 (https://github.com/JimmyLv/BibiGPT) é¡¹ç®çµææ¥æº - [bilibili-API-
 collect](https://github.com/SocialSisterYi/bilibili-API-collect)
 æå§æ¶éçåç§ BiliBili Api åå¶æä¾ç gRPC Api è°ç¨æ¹æ¡ -
 [HarukaBot](https://github.com/SK-415/HarukaBot) åè½æ¥æº - [BBot-Graia]
 (https://github.com/djkcyl/BBot-Graia) åè½æ¥æº ~~(æ ç æ èª å·±)~~ -
 [ABot-Graia](https://github.com/djkcyl/ABot-Graia) æ°¸è¿æå¿µæå¥½ç ABot
```

### Comparing `nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/__init__.py` & `nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/api/__init__.py` & `nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/api/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/api/base.py` & `nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/api/base.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/api/bilibili_auth.py` & `nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/api/bilibili_auth.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/api/subs_config.py` & `nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/api/subs_config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/api/webui.py` & `nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/api/webui.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/base_content_parsing.py` & `nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/base_content_parsing.py`

 * *Files 0% similar despite different names*

```diff
@@ -163,15 +163,15 @@
     if plugin_config.bilichat_basic_info:
         content_image = await content.get_image(plugin_config.bilichat_basic_info_style)
 
         msgs = UniMessage()
         msgs.append(reply)
         if content_image:
             msgs.append(Image(raw=content_image))
-        msgs.append(content.url if plugin_config.bilichat_basic_info_url else content.bili_id)
+        msgs.append(Text(content.url if plugin_config.bilichat_basic_info_url else content.bili_id))
         receipt = await msgs.send()
         reply = receipt.get_reply() if plugin_config.bilichat_reply_to_basic_info else reply
 
     if not isinstance(content, (Video, Column)):
         return
 
     future_msg = UniMessage()
```

### Comparing `nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/commands/auto_delete_subs.py` & `nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/commands/auto_delete_subs.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/commands/base.py` & `nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/commands/base.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/commands/functions.py` & `nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/commands/functions.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/commands/login.py` & `nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/commands/login.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/commands/subs.py` & `nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/commands/subs.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/commands/subs_cfg.py` & `nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/commands/subs_cfg.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/config.py` & `nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/content/column.py` & `nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/content/column.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/content/dynamic.py` & `nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/content/dynamic.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/content/video.py` & `nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/content/video.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/lib/bcut_asr.py` & `nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/lib/bcut_asr.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/lib/bilibili_request/auth.py` & `nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/lib/bilibili_request/auth.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/lib/bilibili_request/gRPC.py` & `nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/lib/bilibili_request/gRPC.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/lib/bilibili_request/restAPI.py` & `nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/lib/bilibili_request/restAPI.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/lib/browser.py` & `nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/lib/browser.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/lib/cache/json_cache.py` & `nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/lib/cache/json_cache.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/lib/cache/mongo_cache.py` & `nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/lib/cache/mongo_cache.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/lib/draw/__init__.py` & `nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/lib/draw/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/lib/draw/column/browser_shot.py` & `nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/lib/draw/column/browser_shot.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,14 @@
 import asyncio
 import re
 
 from nonebot.log import logger
+from playwright.async_api import TimeoutError
 
 from ....config import plugin_config
-
-try:
-    from playwright._impl._errors import TimeoutError  # type: ignore
-except ImportError:
-    from playwright._impl._api_types import TimeoutError  # type: ignore
-
 from ....model.exception import AbortError, CaptchaAbortError, NotFindAbortError
 from ....optional import capture_exception
 from ...browser import get_new_page, network_requestfailed, pw_font_injecter
 
 
 async def screenshot(cvid: str, retry: bool = True, **kwargs):
     logger.info(f"正在截图专栏：{cvid}")
```

### Comparing `nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/lib/draw/dynamic/browser_shot.py` & `nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/lib/draw/dynamic/browser_shot.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,12 @@
 import asyncio
 import re
 
 from nonebot.log import logger
-from playwright.async_api import Page, Response
-
-try:
-    from playwright._impl._errors import TimeoutError  # type: ignore
-except ImportError:
-    from playwright._impl._api_types import TimeoutError  # type: ignore
+from playwright.async_api import Page, Response, TimeoutError
 
 from ....config import plugin_config
 from ....model.exception import AbortError, CaptchaAbortError, NotFindAbortError
 from ....optional import capture_exception
 from ...browser import get_new_page, mobile_style_js, network_requestfailed, pw_font_injecter
```

### Comparing `nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/lib/draw/dynamic/dynamicrender.py` & `nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/lib/draw/dynamic/dynamicrender.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/lib/draw/video/__init__.py` & `nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/lib/draw/video/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/lib/draw/video/bbot_default.py` & `nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/lib/draw/video/bbot_default.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/lib/draw/video/style_blue.py` & `nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/lib/draw/video/style_blue.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/lib/fetch_dynamic.py` & `nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/lib/fetch_dynamic.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/lib/fonts_provider.py` & `nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/lib/fonts_provider.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/lib/store.py` & `nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/lib/store.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/lib/strings.py` & `nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/lib/strings.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/lib/text_to_image.py` & `nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/lib/text_to_image.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/lib/tools.py` & `nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/lib/tools.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/lib/uid_extract.py` & `nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/lib/uid_extract.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/lib/video_subtitle.py` & `nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/lib/video_subtitle.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/model/api/__init__.py` & `nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/model/api/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/model/api/subs_config.py` & `nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/model/api/subs_config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/model/arguments.py` & `nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/model/arguments.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/model/bcut_asr.py` & `nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/model/bcut_asr.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/model/bilibili/live.py` & `nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/model/bilibili/live.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/model/bilibili/summary.py` & `nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/model/bilibili/summary.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/model/const.py` & `nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/model/const.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/model/exception.py` & `nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/model/exception.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/static/browser/mobile_style.js` & `nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/static/browser/mobile_style.js`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/static/style_blue/assets/business.png` & `nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/static/style_blue/assets/business.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/static/style_blue/assets/personal.png` & `nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/static/style_blue/assets/personal.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/static/style_blue/assets/video_bottom.png` & `nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/static/style_blue/assets/video_bottom.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/static/style_blue/video-details.html` & `nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/static/style_blue/video-details.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/static/summary/bilibili.png` & `nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/static/summary/bilibili.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/static/summary/index.html` & `nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/static/summary/index.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/static/summary/marked.min.js` & `nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/static/summary/marked.min.js`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/static/summary/openai.png` & `nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/static/summary/openai.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/static/upload-webui.html` & `nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/static/upload-webui.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/static/webui.tar.gz` & `nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/static/webui.tar.gz`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/subscribe/__init__.py` & `nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/subscribe/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/subscribe/dynamic.py` & `nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/subscribe/dynamic.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/subscribe/live.py` & `nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/subscribe/live.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/subscribe/manager.py` & `nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/subscribe/manager.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/summary/openai.py` & `nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/summary/openai.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/summary/openai_summarise.py` & `nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/summary/openai_summarise.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.9.2/nonebot_plugin_bilichat/wordcloud.py` & `nonebot_plugin_bilichat-5.9.3/nonebot_plugin_bilichat/wordcloud.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.9.2/pyproject.toml` & `nonebot_plugin_bilichat-5.9.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-bilichat"
-version = "5.9.2"
+version = "5.9.3"
 description = "多种B站链接解析，视频词云，AI总结，你想要的都在 bilichat"
 authors = [
     { name = "djkcyl", email = "cyl@cyllive.cn" },
     { name = "Well404", email = "well_404@outlook.com" },
 ]
 dependencies = [
     "bilireq>=0.2.13",
@@ -56,15 +56,14 @@
 target-version = "py310"
 
 [tool.pdm.dev-dependencies]
 dev = [
     "nonebot-adapter-onebot>=2.2.4",
     "nonebot-adapter-mirai2>=0.0.22",
     "nonebot-adapter-qq>=1.0.1",
-    "viztracer>=0.16.1",
     "nonebot-adapter-satori>=0.10.3",
 ]
 
 [build-system]
 requires = [
     "pdm-backend",
 ]
```

### Comparing `nonebot_plugin_bilichat-5.9.2/PKG-INFO` & `nonebot_plugin_bilichat-5.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-bilichat
-Version: 5.9.2
+Version: 5.9.3
 Summary: 多种B站链接解析，视频词云，AI总结，你想要的都在 bilichat
 Author-Email: djkcyl <cyl@cyllive.cn>, Well404 <well_404@outlook.com>
 License: AGPL3.0
 Requires-Python: <4.0,>=3.10
 Requires-Dist: bilireq>=0.2.13
 Requires-Dist: qrcode>=7.4.2
 Requires-Dist: pillow>=9.5.0
@@ -58,15 +58,15 @@
   <img alt="PyPI - Downloads" src="https://img.shields.io/pypi/dm/nonebot-plugin-bilichat">
 </a>
 
 <a href="https://pypi.python.org/pypi/nonebot-plugin-bilichat">
     <img src="https://img.shields.io/pypi/v/nonebot-plugin-bilichat.svg" alt="pypi">
 </a>
 
-<img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">
+<img src="https://img.shields.io/badge/python-3.10+-blue.svg" alt="python">
 
 <a href="https://pdm.fming.dev">
     <img src="https://img.shields.io/badge/pdm-managed-blueviolet" alt="pdm-managed">
 </a>
 
 <a href="https://github.com/psf/black">
     <img src="https://img.shields.io/badge/code%20style-black-000000.svg" alt="Code style: black">
@@ -365,15 +365,15 @@
 |    unsub     |  主人  |  群聊  |      UP 主的昵称或 UID，或 `all`       |         移除订阅，all 时为全移除         |
 |    check     | 无限制 |  群聊  |       UP 主的昵称或 UID，或留空        |    查看本群订阅列表或指定 UP 主的配置    |
 |    reset     |  主人  |  群聊  |      UP 主的昵称或 UID，或 `all`       | 重置指定 UP 主的推送配置，all 时为全重置 |
 |    atall     |  主人  |  群聊  | UP 主的昵称或 UID `全局` `动态` `直播` |           设置是否 at 全体成员           |
 |   dynamic    |  主人  |  群聊  |           UP 主的昵称或 UID            |         是否开启该 UP 的动态通知         |
 |     live     |  主人  |  群聊  |           UP 主的昵称或 UID            |         是否开启该 UP 的直播通知         |
 | checkdynamic | 无限制 | 无限制 |           UP 主的昵称或 UID            |       查看指定 UP 主的最新一条动态       |
-|    fetch     | 无限制 | 无限制 | 视频或动态 ID，或回复包含此内容的消息  |       解析动态包含的图片或视频直链       |
+|    fetch     | 无限制 | 无限制 |    动态 ID，或回复包含此内容的消息     |            解析动态包含的图片            |
 |  checklogin  |  主人  | 无限制 |                   无                   |         查看当前已登录的全部账号         |
 |   qrlogin    |  主人  | 无限制 |                   无                   |      使用二维码登录 B 站，防止风控       |
 |    logout    |  主人  | 无限制 |               账号的 UID               |              登出指定的账号              |
 
 ## 🙏 感谢
 
 在此感谢以下开发者(项目)对本项目做出的贡献：
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-bilichat Version: 5.9.2 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-bilichat Version: 5.9.3 Summary:
 å¤ç§Bç«é¾æ¥è§£æï¼è§é¢è¯äºï¼AIæ»ç»ï¼ä½ æ³è¦çé½å¨ bilichat
 Author-Email: djkcyl
 cyllive.cn>, Well404
 outlook.com> License: AGPL3.0 Requires-Python: <4.0,>=3.10 Requires-Dist:
 bilireq>=0.2.13 Requires-Dist: qrcode>=7.4.2 Requires-Dist: pillow>=9.5.0
 Requires-Dist: lxml>=4.9.2 Requires-Dist: nonebot-plugin-localstore>=0.4.1
 Requires-Dist: nonebot2[fastapi,websockets]>=2.0.0 Requires-Dist: httpx>=0.24.1
@@ -193,19 +193,19 @@
 ä¸»äºº | ç¾¤è | UP ä¸»çæµç§°æ UIDï¼æ `all` | éç½®æå® UP
 ä¸»çæ¨ééç½®ï¼all æ¶ä¸ºå¨éç½® | | atall | ä¸»äºº | ç¾¤è | UP
 ä¸»çæµç§°æ UID `å¨å±` `å¨æ` `ç´æ­` | è®¾ç½®æ¯å¦ at å¨ä½æå |
 | dynamic | ä¸»äºº | ç¾¤è | UP ä¸»çæµç§°æ UID | æ¯å¦å¼å¯è¯¥ UP
 çå¨æéç¥ | | live | ä¸»äºº | ç¾¤è | UP ä¸»çæµç§°æ UID |
 æ¯å¦å¼å¯è¯¥ UP çç´æ­éç¥ | | checkdynamic | æ éå¶ | æ éå¶ |
 UP ä¸»çæµç§°æ UID | æ¥çæå® UP ä¸»çææ°ä¸æ¡å¨æ | | fetch |
-æ éå¶ | æ éå¶ | è§é¢æå¨æ IDï¼æåå¤åå«æ­¤åå®¹çæ¶æ¯
-| è§£æå¨æåå«çå¾çæè§é¢ç´é¾ | | checklogin | ä¸»äºº |
-æ éå¶ | æ  | æ¥çå½åå·²ç»å½çå¨é¨è´¦å· | | qrlogin | ä¸»äºº |
-æ éå¶ | æ  | ä½¿ç¨äºç»´ç ç»å½ B ç«ï¼é²æ­¢é£æ§ | | logout |
-ä¸»äºº | æ éå¶ | è´¦å·ç UID | ç»åºæå®çè´¦å· | ## ð æè°¢
+æ éå¶ | æ éå¶ | å¨æ IDï¼æåå¤åå«æ­¤åå®¹çæ¶æ¯ |
+è§£æå¨æåå«çå¾ç | | checklogin | ä¸»äºº | æ éå¶ | æ  |
+æ¥çå½åå·²ç»å½çå¨é¨è´¦å· | | qrlogin | ä¸»äºº | æ éå¶ | æ  |
+ä½¿ç¨äºç»´ç ç»å½ B ç«ï¼é²æ­¢é£æ§ | | logout | ä¸»äºº | æ éå¶ |
+è´¦å·ç UID | ç»åºæå®çè´¦å· | ## ð æè°¢
 å¨æ­¤æè°¢ä»¥ä¸å¼åè(é¡¹ç®)å¯¹æ¬é¡¹ç®ååºçè´¡ç®ï¼ - [BibiGPT]
 (https://github.com/JimmyLv/BibiGPT) é¡¹ç®çµææ¥æº - [bilibili-API-
 collect](https://github.com/SocialSisterYi/bilibili-API-collect)
 æå§æ¶éçåç§ BiliBili Api åå¶æä¾ç gRPC Api è°ç¨æ¹æ¡ -
 [HarukaBot](https://github.com/SK-415/HarukaBot) åè½æ¥æº - [BBot-Graia]
 (https://github.com/djkcyl/BBot-Graia) åè½æ¥æº ~~(æ ç æ èª å·±)~~ -
 [ABot-Graia](https://github.com/djkcyl/ABot-Graia) æ°¸è¿æå¿µæå¥½ç ABot
```

