# Comparing `tmp/bot_station-0.3.0.tar.gz` & `tmp/bot_station-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bot_station-0.3.0.tar", last modified: Mon May  6 05:52:57 2024, max compression
+gzip compressed data, was "bot_station-0.3.1.tar", last modified: Wed May  8 19:14:51 2024, max compression
```

## Comparing `bot_station-0.3.0.tar` & `bot_station-0.3.1.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxr-xr-x   0 mmarashan (1826057312) LD\Domain Users (593637566)        0 2024-05-06 05:52:57.723927 bot_station-0.3.0/
--rw-r--r--   0 mmarashan (1826057312) LD\Domain Users (593637566)     1070 2024-05-05 19:58:38.000000 bot_station-0.3.0/LICENSE
--rw-r--r--   0 mmarashan (1826057312) LD\Domain Users (593637566)      707 2024-05-06 05:52:57.723743 bot_station-0.3.0/PKG-INFO
--rw-r--r--   0 mmarashan (1826057312) LD\Domain Users (593637566)       17 2024-05-05 19:58:38.000000 bot_station-0.3.0/README.md
-drwxr-xr-x   0 mmarashan (1826057312) LD\Domain Users (593637566)        0 2024-05-06 05:52:57.716646 bot_station-0.3.0/bot_station/
--rw-r--r--   0 mmarashan (1826057312) LD\Domain Users (593637566)        0 2024-05-05 19:58:38.000000 bot_station-0.3.0/bot_station/__init__.py
-drwxr-xr-x   0 mmarashan (1826057312) LD\Domain Users (593637566)        0 2024-05-06 05:52:57.717454 bot_station-0.3.0/bot_station/api/
--rw-r--r--   0 mmarashan (1826057312) LD\Domain Users (593637566)        0 2024-05-05 19:58:38.000000 bot_station-0.3.0/bot_station/api/__init__.py
-drwxr-xr-x   0 mmarashan (1826057312) LD\Domain Users (593637566)        0 2024-05-06 05:52:57.717665 bot_station-0.3.0/bot_station/api/rest/
--rw-r--r--   0 mmarashan (1826057312) LD\Domain Users (593637566)        0 2024-05-05 19:58:38.000000 bot_station-0.3.0/bot_station/api/rest/__init__.py
--rw-r--r--   0 mmarashan (1826057312) LD\Domain Users (593637566)     6751 2024-05-06 05:45:03.000000 bot_station-0.3.0/bot_station/api/rest/api.py
-drwxr-xr-x   0 mmarashan (1826057312) LD\Domain Users (593637566)        0 2024-05-06 05:52:57.718894 bot_station-0.3.0/bot_station/api/rest/model/
--rw-r--r--   0 mmarashan (1826057312) LD\Domain Users (593637566)        0 2024-05-05 19:58:38.000000 bot_station-0.3.0/bot_station/api/rest/model/__init__.py
--rw-r--r--   0 mmarashan (1826057312) LD\Domain Users (593637566)      257 2024-05-05 19:58:38.000000 bot_station-0.3.0/bot_station/api/rest/model/bot_call_dto.py
--rw-r--r--   0 mmarashan (1826057312) LD\Domain Users (593637566)      331 2024-05-05 19:58:38.000000 bot_station-0.3.0/bot_station/api/rest/model/bot_call_result.py
--rw-r--r--   0 mmarashan (1826057312) LD\Domain Users (593637566)      486 2024-05-06 05:44:47.000000 bot_station-0.3.0/bot_station/api/rest/model/bot_creation_dto.py
--rw-r--r--   0 mmarashan (1826057312) LD\Domain Users (593637566)      126 2024-05-05 19:58:38.000000 bot_station-0.3.0/bot_station/api/rest/model/bot_creation_result.py
--rw-r--r--   0 mmarashan (1826057312) LD\Domain Users (593637566)      433 2024-05-05 19:58:38.000000 bot_station-0.3.0/bot_station/api/rest/model/bot_dto.py
--rw-r--r--   0 mmarashan (1826057312) LD\Domain Users (593637566)      391 2024-05-05 19:58:38.000000 bot_station-0.3.0/bot_station/api/rest/model/bot_train_dto.py
--rw-r--r--   0 mmarashan (1826057312) LD\Domain Users (593637566)       90 2024-05-05 19:58:38.000000 bot_station-0.3.0/bot_station/api/rest/model/bot_train_result.py
--rw-r--r--   0 mmarashan (1826057312) LD\Domain Users (593637566)      204 2024-05-05 19:58:38.000000 bot_station-0.3.0/bot_station/api/rest/model/web_app_config.py
-drwxr-xr-x   0 mmarashan (1826057312) LD\Domain Users (593637566)        0 2024-05-06 05:52:57.719017 bot_station-0.3.0/bot_station/data/
--rw-r--r--   0 mmarashan (1826057312) LD\Domain Users (593637566)        0 2024-05-05 19:58:38.000000 bot_station-0.3.0/bot_station/data/__init__.py
-drwxr-xr-x   0 mmarashan (1826057312) LD\Domain Users (593637566)        0 2024-05-06 05:52:57.719120 bot_station-0.3.0/bot_station/data/base/
--rw-r--r--   0 mmarashan (1826057312) LD\Domain Users (593637566)        0 2024-05-05 19:58:38.000000 bot_station-0.3.0/bot_station/data/base/__init__.py
-drwxr-xr-x   0 mmarashan (1826057312) LD\Domain Users (593637566)        0 2024-05-06 05:52:57.719452 bot_station-0.3.0/bot_station/data/base/database/
--rw-r--r--   0 mmarashan (1826057312) LD\Domain Users (593637566)      975 2024-05-05 19:58:38.000000 bot_station-0.3.0/bot_station/data/base/database/UUID.py
--rw-r--r--   0 mmarashan (1826057312) LD\Domain Users (593637566)        0 2024-05-05 19:58:38.000000 bot_station-0.3.0/bot_station/data/base/database/__init__.py
--rw-r--r--   0 mmarashan (1826057312) LD\Domain Users (593637566)      428 2024-05-05 19:58:38.000000 bot_station-0.3.0/bot_station/data/base/database/base_db_dto.py
-drwxr-xr-x   0 mmarashan (1826057312) LD\Domain Users (593637566)        0 2024-05-06 05:52:57.719888 bot_station-0.3.0/bot_station/data/bot/
--rw-r--r--   0 mmarashan (1826057312) LD\Domain Users (593637566)        0 2024-05-05 19:58:38.000000 bot_station-0.3.0/bot_station/data/bot/__init__.py
--rw-r--r--   0 mmarashan (1826057312) LD\Domain Users (593637566)      992 2024-05-05 19:58:38.000000 bot_station-0.3.0/bot_station/data/bot/bot_factory_impl.py
--rw-r--r--   0 mmarashan (1826057312) LD\Domain Users (593637566)     7893 2024-05-05 19:58:38.000000 bot_station-0.3.0/bot_station/data/bot/bot_impl.py
--rw-r--r--   0 mmarashan (1826057312) LD\Domain Users (593637566)     2169 2024-05-05 19:58:38.000000 bot_station-0.3.0/bot_station/data/bot/chat_message_storage_impl.py
-drwxr-xr-x   0 mmarashan (1826057312) LD\Domain Users (593637566)        0 2024-05-06 05:52:57.720086 bot_station-0.3.0/bot_station/data/bot/mapper/
--rw-r--r--   0 mmarashan (1826057312) LD\Domain Users (593637566)        0 2024-05-05 19:58:38.000000 bot_station-0.3.0/bot_station/data/bot/mapper/__init__.py
--rw-r--r--   0 mmarashan (1826057312) LD\Domain Users (593637566)      887 2024-05-05 19:58:38.000000 bot_station-0.3.0/bot_station/data/bot/mapper/document_mapper.py
-drwxr-xr-x   0 mmarashan (1826057312) LD\Domain Users (593637566)        0 2024-05-06 05:52:57.720280 bot_station-0.3.0/bot_station/data/bot/model/
--rw-r--r--   0 mmarashan (1826057312) LD\Domain Users (593637566)        0 2024-05-05 19:58:38.000000 bot_station-0.3.0/bot_station/data/bot/model/__init__.py
--rw-r--r--   0 mmarashan (1826057312) LD\Domain Users (593637566)      238 2024-05-05 19:58:38.000000 bot_station-0.3.0/bot_station/data/bot/model/yandex_cloud_config.py
-drwxr-xr-x   0 mmarashan (1826057312) LD\Domain Users (593637566)        0 2024-05-06 05:52:57.720499 bot_station-0.3.0/bot_station/data/bot_station/
--rw-r--r--   0 mmarashan (1826057312) LD\Domain Users (593637566)      508 2024-05-05 19:58:38.000000 bot_station-0.3.0/bot_station/data/bot_station/__init__.py
--rw-r--r--   0 mmarashan (1826057312) LD\Domain Users (593637566)     3061 2024-05-06 05:42:48.000000 bot_station-0.3.0/bot_station/data/bot_station/bot_registry_impl.py
-drwxr-xr-x   0 mmarashan (1826057312) LD\Domain Users (593637566)        0 2024-05-06 05:52:57.720707 bot_station-0.3.0/bot_station/data/bot_station/model/
--rw-r--r--   0 mmarashan (1826057312) LD\Domain Users (593637566)        0 2024-05-05 19:58:38.000000 bot_station-0.3.0/bot_station/data/bot_station/model/__init__.py
--rw-r--r--   0 mmarashan (1826057312) LD\Domain Users (593637566)      853 2024-05-06 05:42:37.000000 bot_station-0.3.0/bot_station/data/bot_station/model/bot_info_dto.py
-drwxr-xr-x   0 mmarashan (1826057312) LD\Domain Users (593637566)        0 2024-05-06 05:52:57.720922 bot_station-0.3.0/bot_station/di/
--rw-r--r--   0 mmarashan (1826057312) LD\Domain Users (593637566)        0 2024-05-05 19:58:38.000000 bot_station-0.3.0/bot_station/di/__init__.py
--rw-r--r--   0 mmarashan (1826057312) LD\Domain Users (593637566)     1268 2024-05-05 19:58:38.000000 bot_station-0.3.0/bot_station/di/bot_station_module.py
-drwxr-xr-x   0 mmarashan (1826057312) LD\Domain Users (593637566)        0 2024-05-06 05:52:57.721036 bot_station-0.3.0/bot_station/domain/
--rw-r--r--   0 mmarashan (1826057312) LD\Domain Users (593637566)        0 2024-05-05 19:58:38.000000 bot_station-0.3.0/bot_station/domain/__init__.py
-drwxr-xr-x   0 mmarashan (1826057312) LD\Domain Users (593637566)        0 2024-05-06 05:52:57.721355 bot_station-0.3.0/bot_station/domain/base/
--rw-r--r--   0 mmarashan (1826057312) LD\Domain Users (593637566)        0 2024-05-05 19:58:38.000000 bot_station-0.3.0/bot_station/domain/base/__init__.py
--rw-r--r--   0 mmarashan (1826057312) LD\Domain Users (593637566)      544 2024-05-05 19:58:38.000000 bot_station-0.3.0/bot_station/domain/base/const.py
--rw-r--r--   0 mmarashan (1826057312) LD\Domain Users (593637566)      391 2024-05-05 19:58:38.000000 bot_station-0.3.0/bot_station/domain/base/utils.py
-drwxr-xr-x   0 mmarashan (1826057312) LD\Domain Users (593637566)        0 2024-05-06 05:52:57.721764 bot_station-0.3.0/bot_station/domain/bot/
--rw-r--r--   0 mmarashan (1826057312) LD\Domain Users (593637566)        0 2024-05-05 19:58:38.000000 bot_station-0.3.0/bot_station/domain/bot/__init__.py
--rw-r--r--   0 mmarashan (1826057312) LD\Domain Users (593637566)      673 2024-05-05 19:58:38.000000 bot_station-0.3.0/bot_station/domain/bot/bot.py
--rw-r--r--   0 mmarashan (1826057312) LD\Domain Users (593637566)      267 2024-05-05 19:58:38.000000 bot_station-0.3.0/bot_station/domain/bot/bot_factory.py
--rw-r--r--   0 mmarashan (1826057312) LD\Domain Users (593637566)      798 2024-05-05 19:58:38.000000 bot_station-0.3.0/bot_station/domain/bot/chat_message_storage.py
-drwxr-xr-x   0 mmarashan (1826057312) LD\Domain Users (593637566)        0 2024-05-06 05:52:57.722417 bot_station-0.3.0/bot_station/domain/bot/model/
--rw-r--r--   0 mmarashan (1826057312) LD\Domain Users (593637566)        0 2024-05-05 19:58:38.000000 bot_station-0.3.0/bot_station/domain/bot/model/__init__.py
--rw-r--r--   0 mmarashan (1826057312) LD\Domain Users (593637566)      143 2024-05-05 19:58:38.000000 bot_station-0.3.0/bot_station/domain/bot/model/document.py
--rw-r--r--   0 mmarashan (1826057312) LD\Domain Users (593637566)      350 2024-05-05 19:58:38.000000 bot_station-0.3.0/bot_station/domain/bot/model/lm_bot_meta_info.py
--rw-r--r--   0 mmarashan (1826057312) LD\Domain Users (593637566)      254 2024-05-05 19:58:38.000000 bot_station-0.3.0/bot_station/domain/bot/model/lm_call_result.py
--rw-r--r--   0 mmarashan (1826057312) LD\Domain Users (593637566)      361 2024-05-05 19:58:38.000000 bot_station-0.3.0/bot_station/domain/bot/model/lm_chat_message.py
--rw-r--r--   0 mmarashan (1826057312) LD\Domain Users (593637566)      379 2024-05-05 19:58:38.000000 bot_station-0.3.0/bot_station/domain/bot/model/lm_train_data.py
-drwxr-xr-x   0 mmarashan (1826057312) LD\Domain Users (593637566)        0 2024-05-06 05:52:57.722738 bot_station-0.3.0/bot_station/domain/bot_station/
--rw-r--r--   0 mmarashan (1826057312) LD\Domain Users (593637566)        0 2024-05-05 19:58:38.000000 bot_station-0.3.0/bot_station/domain/bot_station/__init__.py
--rw-r--r--   0 mmarashan (1826057312) LD\Domain Users (593637566)      692 2024-05-05 19:58:38.000000 bot_station-0.3.0/bot_station/domain/bot_station/bot_registry.py
--rw-r--r--   0 mmarashan (1826057312) LD\Domain Users (593637566)     2509 2024-05-05 19:58:38.000000 bot_station-0.3.0/bot_station/domain/bot_station/bot_station.py
-drwxr-xr-x   0 mmarashan (1826057312) LD\Domain Users (593637566)        0 2024-05-06 05:52:57.723031 bot_station-0.3.0/bot_station/domain/bot_station/model/
--rw-r--r--   0 mmarashan (1826057312) LD\Domain Users (593637566)        0 2024-05-05 19:58:38.000000 bot_station-0.3.0/bot_station/domain/bot_station/model/__init__.py
--rw-r--r--   0 mmarashan (1826057312) LD\Domain Users (593637566)      279 2024-05-06 05:37:14.000000 bot_station-0.3.0/bot_station/domain/bot_station/model/bot_creation_config.py
-drwxr-xr-x   0 mmarashan (1826057312) LD\Domain Users (593637566)        0 2024-05-06 05:52:57.723534 bot_station-0.3.0/bot_station.egg-info/
--rw-r--r--   0 mmarashan (1826057312) LD\Domain Users (593637566)      707 2024-05-06 05:52:57.000000 bot_station-0.3.0/bot_station.egg-info/PKG-INFO
--rw-r--r--   0 mmarashan (1826057312) LD\Domain Users (593637566)     2363 2024-05-06 05:52:57.000000 bot_station-0.3.0/bot_station.egg-info/SOURCES.txt
--rw-r--r--   0 mmarashan (1826057312) LD\Domain Users (593637566)        1 2024-05-06 05:52:57.000000 bot_station-0.3.0/bot_station.egg-info/dependency_links.txt
--rw-r--r--   0 mmarashan (1826057312) LD\Domain Users (593637566)      190 2024-05-06 05:52:57.000000 bot_station-0.3.0/bot_station.egg-info/requires.txt
--rw-r--r--   0 mmarashan (1826057312) LD\Domain Users (593637566)       18 2024-05-06 05:52:57.000000 bot_station-0.3.0/bot_station.egg-info/top_level.txt
--rw-r--r--   0 mmarashan (1826057312) LD\Domain Users (593637566)       38 2024-05-06 05:52:57.723964 bot_station-0.3.0/setup.cfg
--rw-r--r--   0 mmarashan (1826057312) LD\Domain Users (593637566)      778 2024-05-06 05:51:27.000000 bot_station-0.3.0/setup.py
-drwxr-xr-x   0 mmarashan (1826057312) LD\Domain Users (593637566)        0 2024-05-06 05:52:57.723368 bot_station-0.3.0/tests/
--rw-r--r--   0 mmarashan (1826057312) LD\Domain Users (593637566)        0 2024-05-05 19:58:38.000000 bot_station-0.3.0/tests/__init__.py
--rw-r--r--   0 mmarashan (1826057312) LD\Domain Users (593637566)     3334 2024-05-05 19:58:38.000000 bot_station-0.3.0/tests/bot_station_api_test.py
--rw-r--r--   0 mmarashan (1826057312) LD\Domain Users (593637566)     1051 2024-05-05 19:58:38.000000 bot_station-0.3.0/tests/test_bot_factory.py
+drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-08 19:14:51.177519 bot_station-0.3.1/
+-rw-r--r--   0 mmarashan (1826057312) 593637566     1070 2024-05-05 19:58:38.000000 bot_station-0.3.1/LICENSE
+-rw-r--r--   0 mmarashan (1826057312) 593637566      707 2024-05-08 19:14:51.177299 bot_station-0.3.1/PKG-INFO
+-rw-r--r--   0 mmarashan (1826057312) 593637566       17 2024-05-05 19:58:38.000000 bot_station-0.3.1/README.md
+drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-08 19:14:51.166216 bot_station-0.3.1/bot_station/
+-rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.3.1/bot_station/__init__.py
+drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-08 19:14:51.167618 bot_station-0.3.1/bot_station/api/
+-rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.3.1/bot_station/api/__init__.py
+drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-08 19:14:51.167965 bot_station-0.3.1/bot_station/api/rest/
+-rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.3.1/bot_station/api/rest/__init__.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566     6988 2024-05-08 06:14:06.000000 bot_station-0.3.1/bot_station/api/rest/api.py
+drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-08 19:14:51.170214 bot_station-0.3.1/bot_station/api/rest/model/
+-rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.3.1/bot_station/api/rest/model/__init__.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566      257 2024-05-05 19:58:38.000000 bot_station-0.3.1/bot_station/api/rest/model/bot_call_dto.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566      331 2024-05-05 19:58:38.000000 bot_station-0.3.1/bot_station/api/rest/model/bot_call_result.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566      486 2024-05-06 05:44:47.000000 bot_station-0.3.1/bot_station/api/rest/model/bot_creation_dto.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566      126 2024-05-05 19:58:38.000000 bot_station-0.3.1/bot_station/api/rest/model/bot_creation_result.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566      433 2024-05-05 19:58:38.000000 bot_station-0.3.1/bot_station/api/rest/model/bot_dto.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566      401 2024-05-08 05:52:39.000000 bot_station-0.3.1/bot_station/api/rest/model/bot_train_dto.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566       90 2024-05-05 19:58:38.000000 bot_station-0.3.1/bot_station/api/rest/model/bot_train_result.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566      204 2024-05-05 19:58:38.000000 bot_station-0.3.1/bot_station/api/rest/model/web_app_config.py
+drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-08 19:14:51.170404 bot_station-0.3.1/bot_station/data/
+-rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.3.1/bot_station/data/__init__.py
+drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-08 19:14:51.170523 bot_station-0.3.1/bot_station/data/base/
+-rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.3.1/bot_station/data/base/__init__.py
+drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-08 19:14:51.170916 bot_station-0.3.1/bot_station/data/base/database/
+-rw-r--r--   0 mmarashan (1826057312) 593637566      975 2024-05-05 19:58:38.000000 bot_station-0.3.1/bot_station/data/base/database/UUID.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.3.1/bot_station/data/base/database/__init__.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566      428 2024-05-05 19:58:38.000000 bot_station-0.3.1/bot_station/data/base/database/base_db_dto.py
+drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-08 19:14:51.171542 bot_station-0.3.1/bot_station/data/bot/
+-rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.3.1/bot_station/data/bot/__init__.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566      992 2024-05-05 19:58:38.000000 bot_station-0.3.1/bot_station/data/bot/bot_factory_impl.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566     7893 2024-05-05 19:58:38.000000 bot_station-0.3.1/bot_station/data/bot/bot_impl.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566     2169 2024-05-05 19:58:38.000000 bot_station-0.3.1/bot_station/data/bot/chat_message_storage_impl.py
+drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-08 19:14:51.171808 bot_station-0.3.1/bot_station/data/bot/mapper/
+-rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.3.1/bot_station/data/bot/mapper/__init__.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566      972 2024-05-08 05:40:36.000000 bot_station-0.3.1/bot_station/data/bot/mapper/document_mapper.py
+drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-08 19:14:51.172238 bot_station-0.3.1/bot_station/data/bot/model/
+-rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.3.1/bot_station/data/bot/model/__init__.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566      238 2024-05-05 19:58:38.000000 bot_station-0.3.1/bot_station/data/bot/model/yandex_cloud_config.py
+drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-08 19:14:51.172563 bot_station-0.3.1/bot_station/data/bot_station/
+-rw-r--r--   0 mmarashan (1826057312) 593637566      508 2024-05-05 19:58:38.000000 bot_station-0.3.1/bot_station/data/bot_station/__init__.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566     3061 2024-05-06 05:42:48.000000 bot_station-0.3.1/bot_station/data/bot_station/bot_registry_impl.py
+drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-08 19:14:51.172997 bot_station-0.3.1/bot_station/data/bot_station/model/
+-rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.3.1/bot_station/data/bot_station/model/__init__.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566      853 2024-05-06 05:42:37.000000 bot_station-0.3.1/bot_station/data/bot_station/model/bot_info_dto.py
+drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-08 19:14:51.173452 bot_station-0.3.1/bot_station/di/
+-rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.3.1/bot_station/di/__init__.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566     1268 2024-05-05 19:58:38.000000 bot_station-0.3.1/bot_station/di/bot_station_module.py
+drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-08 19:14:51.173621 bot_station-0.3.1/bot_station/domain/
+-rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.3.1/bot_station/domain/__init__.py
+drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-08 19:14:51.173957 bot_station-0.3.1/bot_station/domain/base/
+-rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.3.1/bot_station/domain/base/__init__.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566      544 2024-05-05 19:58:38.000000 bot_station-0.3.1/bot_station/domain/base/const.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566      391 2024-05-05 19:58:38.000000 bot_station-0.3.1/bot_station/domain/base/utils.py
+drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-08 19:14:51.174526 bot_station-0.3.1/bot_station/domain/bot/
+-rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.3.1/bot_station/domain/bot/__init__.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566      673 2024-05-05 19:58:38.000000 bot_station-0.3.1/bot_station/domain/bot/bot.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566      267 2024-05-05 19:58:38.000000 bot_station-0.3.1/bot_station/domain/bot/bot_factory.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566      798 2024-05-05 19:58:38.000000 bot_station-0.3.1/bot_station/domain/bot/chat_message_storage.py
+drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-08 19:14:51.175533 bot_station-0.3.1/bot_station/domain/bot/model/
+-rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.3.1/bot_station/domain/bot/model/__init__.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566      222 2024-05-08 05:38:32.000000 bot_station-0.3.1/bot_station/domain/bot/model/document.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566      350 2024-05-05 19:58:38.000000 bot_station-0.3.1/bot_station/domain/bot/model/lm_bot_meta_info.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566      254 2024-05-05 19:58:38.000000 bot_station-0.3.1/bot_station/domain/bot/model/lm_call_result.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566      361 2024-05-05 19:58:38.000000 bot_station-0.3.1/bot_station/domain/bot/model/lm_chat_message.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566      379 2024-05-05 19:58:38.000000 bot_station-0.3.1/bot_station/domain/bot/model/lm_train_data.py
+drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-08 19:14:51.175934 bot_station-0.3.1/bot_station/domain/bot_station/
+-rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.3.1/bot_station/domain/bot_station/__init__.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566      692 2024-05-05 19:58:38.000000 bot_station-0.3.1/bot_station/domain/bot_station/bot_registry.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566     2715 2024-05-08 06:12:30.000000 bot_station-0.3.1/bot_station/domain/bot_station/bot_station.py
+drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-08 19:14:51.176288 bot_station-0.3.1/bot_station/domain/bot_station/model/
+-rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.3.1/bot_station/domain/bot_station/model/__init__.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566      279 2024-05-06 05:37:14.000000 bot_station-0.3.1/bot_station/domain/bot_station/model/bot_creation_config.py
+drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-08 19:14:51.177036 bot_station-0.3.1/bot_station.egg-info/
+-rw-r--r--   0 mmarashan (1826057312) 593637566      707 2024-05-08 19:14:51.000000 bot_station-0.3.1/bot_station.egg-info/PKG-INFO
+-rw-r--r--   0 mmarashan (1826057312) 593637566     2363 2024-05-08 19:14:51.000000 bot_station-0.3.1/bot_station.egg-info/SOURCES.txt
+-rw-r--r--   0 mmarashan (1826057312) 593637566        1 2024-05-08 19:14:51.000000 bot_station-0.3.1/bot_station.egg-info/dependency_links.txt
+-rw-r--r--   0 mmarashan (1826057312) 593637566      190 2024-05-08 19:14:51.000000 bot_station-0.3.1/bot_station.egg-info/requires.txt
+-rw-r--r--   0 mmarashan (1826057312) 593637566       18 2024-05-08 19:14:51.000000 bot_station-0.3.1/bot_station.egg-info/top_level.txt
+-rw-r--r--   0 mmarashan (1826057312) 593637566       38 2024-05-08 19:14:51.177567 bot_station-0.3.1/setup.cfg
+-rw-r--r--   0 mmarashan (1826057312) 593637566      834 2024-05-08 19:12:16.000000 bot_station-0.3.1/setup.py
+drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-08 19:14:51.176810 bot_station-0.3.1/tests/
+-rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.3.1/tests/__init__.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566     4483 2024-05-08 05:55:27.000000 bot_station-0.3.1/tests/bot_station_api_test.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566     1051 2024-05-05 19:58:38.000000 bot_station-0.3.1/tests/test_bot_factory.py
```

### Comparing `bot_station-0.3.0/LICENSE` & `bot_station-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bot_station-0.3.0/PKG-INFO` & `bot_station-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bot_station
-Version: 0.3.0
+Version: 0.3.1
 Summary: Bot Station SDK + Web App
 Author: Maxim Marashan
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `bot_station-0.3.0/bot_station/api/rest/api.py` & `bot_station-0.3.1/bot_station/api/rest/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,16 +44,19 @@
 
 router = APIRouter(route_class=LoggingRoute)
 
 
 @router.post("/create", status_code=200, response_model=BotCreationResult)
 async def create(*, dto: BotCreationDto) -> Any:
     logging.debug(f"/create dto : {dto}")
-    bot_id: str = await BotStationWebApp.create(dto)
-    return BotCreationResult(id=bot_id)
+    bot_id: str | None = await BotStationWebApp.create(dto)
+    if bot_id is not None:
+        return BotCreationResult(id=bot_id)
+    else:
+        return Response(status_code=status.HTTP_500_INTERNAL_SERVER_ERROR)
 
 
 @router.post("/train", status_code=200)
 async def train(*, dto: BotTrainDto) -> Any:
     logging.debug(f"/train dto : {dto}")
     result: BotTrainResult = await BotStationWebApp.train(dto)
     if result is BotTrainResult.SUCCESS:
@@ -109,26 +112,30 @@
         BotStationWebApp.api.include_router(router)
 
     @staticmethod
     def launch():
         run_server()
 
     @staticmethod
-    async def create(dto: BotCreationDto) -> str:
+    async def create(dto: BotCreationDto) -> str | None:
         config = BotCreationConfig(
             id=dto.id,
             name=dto.name,
             description=dto.description,
             prompt_intro=dto.prompt_intro,
             add_external_context_to_prompt=dto.add_external_context_to_prompt,
             add_messages_history_to_prompt=dto.add_messages_history_to_prompt,
             temperature=dto.temperature,
         )
-        meta_info: LMBotMetaInfo = await BotStationWebApp.bot_station.create(config)
-        return meta_info.id
+        try:
+            meta_info: LMBotMetaInfo = await BotStationWebApp.bot_station.create(config)
+            return meta_info.id
+        except Exception as e:
+            logging.warning(e)
+            return None
 
     @staticmethod
     async def train(dto: BotTrainDto) -> BotTrainResult:
         bot: Bot | None = await BotStationWebApp.bot_station.get_bot(bot_id=dto.bot_id)
         if bot is None:
             return BotTrainResult.BOT_NOT_FOUND
         else:
```

### Comparing `bot_station-0.3.0/bot_station/data/base/database/UUID.py` & `bot_station-0.3.1/bot_station/data/base/database/UUID.py`

 * *Files identical despite different names*

### Comparing `bot_station-0.3.0/bot_station/data/bot/bot_factory_impl.py` & `bot_station-0.3.1/bot_station/data/bot/bot_factory_impl.py`

 * *Files identical despite different names*

### Comparing `bot_station-0.3.0/bot_station/data/bot/bot_impl.py` & `bot_station-0.3.1/bot_station/data/bot/bot_impl.py`

 * *Files identical despite different names*

### Comparing `bot_station-0.3.0/bot_station/data/bot/chat_message_storage_impl.py` & `bot_station-0.3.1/bot_station/data/bot/chat_message_storage_impl.py`

 * *Files identical despite different names*

### Comparing `bot_station-0.3.0/bot_station/data/bot_station/bot_registry_impl.py` & `bot_station-0.3.1/bot_station/data/bot_station/bot_registry_impl.py`

 * *Files identical despite different names*

### Comparing `bot_station-0.3.0/bot_station/data/bot_station/model/bot_info_dto.py` & `bot_station-0.3.1/bot_station/data/bot_station/model/bot_info_dto.py`

 * *Files identical despite different names*

### Comparing `bot_station-0.3.0/bot_station/di/bot_station_module.py` & `bot_station-0.3.1/bot_station/di/bot_station_module.py`

 * *Files identical despite different names*

### Comparing `bot_station-0.3.0/bot_station/domain/base/const.py` & `bot_station-0.3.1/bot_station/domain/base/const.py`

 * *Files identical despite different names*

### Comparing `bot_station-0.3.0/bot_station/domain/bot/bot.py` & `bot_station-0.3.1/bot_station/domain/bot/bot.py`

 * *Files identical despite different names*

### Comparing `bot_station-0.3.0/bot_station/domain/bot/chat_message_storage.py` & `bot_station-0.3.1/bot_station/domain/bot/chat_message_storage.py`

 * *Files identical despite different names*

### Comparing `bot_station-0.3.0/bot_station/domain/bot_station/bot_registry.py` & `bot_station-0.3.1/bot_station/domain/bot_station/bot_registry.py`

 * *Files identical despite different names*

### Comparing `bot_station-0.3.0/bot_station/domain/bot_station/bot_station.py` & `bot_station-0.3.1/bot_station/domain/bot_station/bot_station.py`

 * *Files 7% similar despite different names*

```diff
@@ -40,16 +40,20 @@
             bot_factory: BotFactory,
     ):
         self.bot_registry = bot_registry
         self.bot_factory = bot_factory
 
     async def create(self, config: BotCreationConfig) -> LMBotMetaInfo:
         logging.debug(f"create {config}")
-        meta_info = await self.bot_registry.create(config)
-        return meta_info
+        bot_with_same_id = await self.bot_registry.get(bot_id=config.id)
+        if bot_with_same_id is None:
+            meta_info = await self.bot_registry.create(config)
+            return meta_info
+        else:
+            raise Exception(f"Bot with id '{config.id}' already exists!")
 
     async def get_bot(self, bot_id: str) -> Bot | None:
         logging.debug(f"get bot_id)")
         if bot_id is None:
             raise Exception("Bot id is None!")
         bot = self.__in_memory_bots.get(bot_id, None)
         if bot is not None:
```

### Comparing `bot_station-0.3.0/bot_station.egg-info/PKG-INFO` & `bot_station-0.3.1/bot_station.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bot_station
-Version: 0.3.0
+Version: 0.3.1
 Summary: Bot Station SDK + Web App
 Author: Maxim Marashan
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `bot_station-0.3.0/bot_station.egg-info/SOURCES.txt` & `bot_station-0.3.1/bot_station.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bot_station-0.3.0/setup.py` & `bot_station-0.3.1/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,17 +2,21 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
+with open('version.txt') as f:
+    version = f.read()
+
+
 setuptools.setup(
     name="bot_station",
-    version="0.3.0",
+    version=version,
     author="Maxim Marashan",
     # author_email="ericjaychi@gmail.com",
     description="Bot Station SDK + Web App",
     long_description=long_description,
     long_description_content_type="text/markdown",
     # url="https://github.com/ericjaychi/sample-pypi-package",
     packages=setuptools.find_packages(),
```

### Comparing `bot_station-0.3.0/tests/test_bot_factory.py` & `bot_station-0.3.1/tests/test_bot_factory.py`

 * *Files identical despite different names*

