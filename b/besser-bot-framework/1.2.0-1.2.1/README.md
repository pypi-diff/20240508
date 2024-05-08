# Comparing `tmp/besser_bot_framework-1.2.0.tar.gz` & `tmp/besser_bot_framework-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "besser_bot_framework-1.2.0.tar", last modified: Wed May  8 08:37:05 2024, max compression
+gzip compressed data, was "besser_bot_framework-1.2.1.tar", last modified: Wed May  8 12:13:01 2024, max compression
```

## Comparing `besser_bot_framework-1.2.0.tar` & `besser_bot_framework-1.2.1.tar`

### file list

```diff
@@ -1,105 +1,105 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 08:37:05.984097 besser_bot_framework-1.2.0/
--rw-rw-rw-   0        0        0     1090 2023-10-24 13:11:01.000000 besser_bot_framework-1.2.0/LICENSE
--rw-rw-rw-   0        0        0     3210 2024-05-08 08:37:05.984097 besser_bot_framework-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     1849 2024-01-22 15:17:03.000000 besser_bot_framework-1.2.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-08 08:37:05.884907 besser_bot_framework-1.2.0/besser/
--rw-rw-rw-   0        0        0        0 2023-10-24 13:15:57.000000 besser_bot_framework-1.2.0/besser/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-08 08:37:05.885907 besser_bot_framework-1.2.0/besser/bot/
--rw-rw-rw-   0        0        0        0 2023-10-24 13:15:57.000000 besser_bot_framework-1.2.0/besser/bot/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-08 08:37:05.893907 besser_bot_framework-1.2.0/besser/bot/core/
--rw-rw-rw-   0        0        0        0 2023-10-24 13:15:57.000000 besser_bot_framework-1.2.0/besser/bot/core/__init__.py
--rw-rw-rw-   0        0        0    20671 2024-05-08 08:36:28.000000 besser_bot_framework-1.2.0/besser/bot/core/bot.py
-drwxrwxrwx   0        0        0        0 2024-05-08 08:37:05.896907 besser_bot_framework-1.2.0/besser/bot/core/entity/
--rw-rw-rw-   0        0        0        0 2023-10-24 13:15:57.000000 besser_bot_framework-1.2.0/besser/bot/core/entity/__init__.py
--rw-rw-rw-   0        0        0     3098 2024-05-08 08:36:28.000000 besser_bot_framework-1.2.0/besser/bot/core/entity/entity.py
--rw-rw-rw-   0        0        0      820 2023-10-24 13:16:24.000000 besser_bot_framework-1.2.0/besser/bot/core/entity/entity_entry.py
--rw-rw-rw-   0        0        0     3855 2024-02-28 10:38:02.000000 besser_bot_framework-1.2.0/besser/bot/core/file.py
-drwxrwxrwx   0        0        0        0 2024-05-08 08:37:05.900906 besser_bot_framework-1.2.0/besser/bot/core/intent/
--rw-rw-rw-   0        0        0        0 2023-10-24 13:15:57.000000 besser_bot_framework-1.2.0/besser/bot/core/intent/__init__.py
--rw-rw-rw-   0        0        0     4815 2024-02-28 10:38:02.000000 besser_bot_framework-1.2.0/besser/bot/core/intent/intent.py
--rw-rw-rw-   0        0        0     1187 2023-10-24 13:16:24.000000 besser_bot_framework-1.2.0/besser/bot/core/intent/intent_parameter.py
--rw-rw-rw-   0        0        0     1077 2023-10-24 13:16:24.000000 besser_bot_framework-1.2.0/besser/bot/core/property.py
--rw-rw-rw-   0        0        0     6585 2024-05-08 08:36:28.000000 besser_bot_framework-1.2.0/besser/bot/core/session.py
--rw-rw-rw-   0        0        0    18203 2024-05-08 08:36:28.000000 besser_bot_framework-1.2.0/besser/bot/core/state.py
--rw-rw-rw-   0        0        0     5258 2023-10-24 13:16:24.000000 besser_bot_framework-1.2.0/besser/bot/core/transition.py
-drwxrwxrwx   0        0        0        0 2024-05-08 08:37:05.903906 besser_bot_framework-1.2.0/besser/bot/db/
--rw-rw-rw-   0        0        0     1648 2024-05-08 08:36:28.000000 besser_bot_framework-1.2.0/besser/bot/db/__init__.py
--rw-rw-rw-   0        0        0    10274 2024-05-08 08:36:28.000000 besser_bot_framework-1.2.0/besser/bot/db/monitoring_db.py
-drwxrwxrwx   0        0        0        0 2024-05-08 08:37:05.905908 besser_bot_framework-1.2.0/besser/bot/exceptions/
--rw-rw-rw-   0        0        0        0 2023-10-24 13:15:57.000000 besser_bot_framework-1.2.0/besser/bot/exceptions/__init__.py
--rw-rw-rw-   0        0        0     4814 2024-02-28 10:38:02.000000 besser_bot_framework-1.2.0/besser/bot/exceptions/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-05-08 08:37:05.907905 besser_bot_framework-1.2.0/besser/bot/library/
--rw-rw-rw-   0        0        0        0 2023-10-24 13:15:57.000000 besser_bot_framework-1.2.0/besser/bot/library/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-08 08:37:05.909907 besser_bot_framework-1.2.0/besser/bot/library/entity/
--rw-rw-rw-   0        0        0        0 2023-10-24 13:15:57.000000 besser_bot_framework-1.2.0/besser/bot/library/entity/__init__.py
--rw-rw-rw-   0        0        0     1423 2024-02-28 10:38:02.000000 besser_bot_framework-1.2.0/besser/bot/library/entity/base_entities.py
-drwxrwxrwx   0        0        0        0 2024-05-08 08:37:05.913906 besser_bot_framework-1.2.0/besser/bot/library/event/
--rw-rw-rw-   0        0        0        0 2023-10-24 13:15:57.000000 besser_bot_framework-1.2.0/besser/bot/library/event/__init__.py
--rw-rw-rw-   0        0        0     2729 2024-02-06 10:51:26.000000 besser_bot_framework-1.2.0/besser/bot/library/event/event_library.py
--rw-rw-rw-   0        0        0      315 2023-10-24 13:16:24.000000 besser_bot_framework-1.2.0/besser/bot/library/event/event_template.py
-drwxrwxrwx   0        0        0        0 2024-05-08 08:37:05.917906 besser_bot_framework-1.2.0/besser/bot/library/intent/
--rw-rw-rw-   0        0        0        0 2023-10-24 13:15:57.000000 besser_bot_framework-1.2.0/besser/bot/library/intent/__init__.py
--rw-rw-rw-   0        0        0     2859 2024-02-28 10:38:02.000000 besser_bot_framework-1.2.0/besser/bot/library/intent/intent_classifier_configuration_library.py
--rw-rw-rw-   0        0        0      239 2023-10-24 13:16:24.000000 besser_bot_framework-1.2.0/besser/bot/library/intent/intent_library.py
-drwxrwxrwx   0        0        0        0 2024-05-08 08:37:05.920947 besser_bot_framework-1.2.0/besser/bot/library/state/
--rw-rw-rw-   0        0        0        0 2023-10-24 13:15:57.000000 besser_bot_framework-1.2.0/besser/bot/library/state/__init__.py
--rw-rw-rw-   0        0        0      756 2024-02-19 15:24:24.000000 besser_bot_framework-1.2.0/besser/bot/library/state/state_library.py
-drwxrwxrwx   0        0        0        0 2024-05-08 08:37:05.924945 besser_bot_framework-1.2.0/besser/bot/nlp/
--rw-rw-rw-   0        0        0     5328 2024-02-28 10:38:02.000000 besser_bot_framework-1.2.0/besser/bot/nlp/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-08 08:37:05.933946 besser_bot_framework-1.2.0/besser/bot/nlp/intent_classifier/
--rw-rw-rw-   0        0        0        0 2023-10-24 13:15:57.000000 besser_bot_framework-1.2.0/besser/bot/nlp/intent_classifier/__init__.py
--rw-rw-rw-   0        0        0     2299 2023-10-24 13:16:24.000000 besser_bot_framework-1.2.0/besser/bot/nlp/intent_classifier/intent_classifier.py
--rw-rw-rw-   0        0        0     6907 2024-02-28 10:38:02.000000 besser_bot_framework-1.2.0/besser/bot/nlp/intent_classifier/intent_classifier_configuration.py
--rw-rw-rw-   0        0        0     2896 2023-10-24 13:16:24.000000 besser_bot_framework-1.2.0/besser/bot/nlp/intent_classifier/intent_classifier_prediction.py
--rw-rw-rw-   0        0        0    12208 2024-02-28 10:38:02.000000 besser_bot_framework-1.2.0/besser/bot/nlp/intent_classifier/llm_intent_classifier.py
--rw-rw-rw-   0        0        0     7722 2024-02-28 10:38:02.000000 besser_bot_framework-1.2.0/besser/bot/nlp/intent_classifier/simple_intent_classifier.py
-drwxrwxrwx   0        0        0        0 2024-05-08 08:37:05.940097 besser_bot_framework-1.2.0/besser/bot/nlp/ner/
--rw-rw-rw-   0        0        0        0 2023-10-24 13:15:57.000000 besser_bot_framework-1.2.0/besser/bot/nlp/ner/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-08 08:37:05.945119 besser_bot_framework-1.2.0/besser/bot/nlp/ner/base/
--rw-rw-rw-   0        0        0        0 2023-10-24 13:15:57.000000 besser_bot_framework-1.2.0/besser/bot/nlp/ner/base/__init__.py
--rw-rw-rw-   0        0        0      226 2023-10-24 13:16:24.000000 besser_bot_framework-1.2.0/besser/bot/nlp/ner/base/any.py
--rw-rw-rw-   0        0        0     7050 2023-10-24 13:16:24.000000 besser_bot_framework-1.2.0/besser/bot/nlp/ner/base/datetime.py
--rw-rw-rw-   0        0        0      975 2023-10-24 13:16:24.000000 besser_bot_framework-1.2.0/besser/bot/nlp/ner/base/number.py
--rw-rw-rw-   0        0        0      786 2023-10-24 13:16:24.000000 besser_bot_framework-1.2.0/besser/bot/nlp/ner/matched_parameter.py
--rw-rw-rw-   0        0        0     1576 2023-10-24 13:16:24.000000 besser_bot_framework-1.2.0/besser/bot/nlp/ner/ner.py
--rw-rw-rw-   0        0        0     1891 2023-10-24 13:16:24.000000 besser_bot_framework-1.2.0/besser/bot/nlp/ner/ner_prediction.py
--rw-rw-rw-   0        0        0    10536 2024-05-08 08:36:28.000000 besser_bot_framework-1.2.0/besser/bot/nlp/ner/simple_ner.py
--rw-rw-rw-   0        0        0     7010 2024-02-28 10:38:02.000000 besser_bot_framework-1.2.0/besser/bot/nlp/nlp_engine.py
-drwxrwxrwx   0        0        0        0 2024-05-08 08:37:05.949097 besser_bot_framework-1.2.0/besser/bot/nlp/preprocessing/
--rw-rw-rw-   0        0        0        0 2023-10-24 13:15:57.000000 besser_bot_framework-1.2.0/besser/bot/nlp/preprocessing/__init__.py
--rw-rw-rw-   0        0        0      909 2023-12-10 20:05:59.000000 besser_bot_framework-1.2.0/besser/bot/nlp/preprocessing/pipelines.py
--rw-rw-rw-   0        0        0     2787 2023-12-12 13:27:54.000000 besser_bot_framework-1.2.0/besser/bot/nlp/preprocessing/text_preprocessing.py
-drwxrwxrwx   0        0        0        0 2024-05-08 08:37:05.955097 besser_bot_framework-1.2.0/besser/bot/nlp/speech2text/
--rw-rw-rw-   0        0        0        0 2023-11-16 11:39:31.000000 besser_bot_framework-1.2.0/besser/bot/nlp/speech2text/__init__.py
--rw-rw-rw-   0        0        0     2294 2024-02-28 10:38:02.000000 besser_bot_framework-1.2.0/besser/bot/nlp/speech2text/api_speech2text.py
--rw-rw-rw-   0        0        0     2302 2024-02-28 10:38:02.000000 besser_bot_framework-1.2.0/besser/bot/nlp/speech2text/hf_speech2text.py
--rw-rw-rw-   0        0        0     1255 2023-11-16 11:39:31.000000 besser_bot_framework-1.2.0/besser/bot/nlp/speech2text/speech2text.py
--rw-rw-rw-   0        0        0     1234 2024-02-28 10:38:02.000000 besser_bot_framework-1.2.0/besser/bot/nlp/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-08 08:37:05.960096 besser_bot_framework-1.2.0/besser/bot/platforms/
--rw-rw-rw-   0        0        0        0 2023-10-24 13:15:57.000000 besser_bot_framework-1.2.0/besser/bot/platforms/__init__.py
--rw-rw-rw-   0        0        0     3790 2024-05-08 08:36:28.000000 besser_bot_framework-1.2.0/besser/bot/platforms/payload.py
--rw-rw-rw-   0        0        0     1787 2024-05-08 08:36:28.000000 besser_bot_framework-1.2.0/besser/bot/platforms/platform.py
-drwxrwxrwx   0        0        0        0 2024-05-08 08:37:05.962099 besser_bot_framework-1.2.0/besser/bot/platforms/telegram/
--rw-rw-rw-   0        0        0      364 2023-11-16 11:39:31.000000 besser_bot_framework-1.2.0/besser/bot/platforms/telegram/__init__.py
--rw-rw-rw-   0        0        0    11876 2024-05-08 08:36:28.000000 besser_bot_framework-1.2.0/besser/bot/platforms/telegram/telegram_platform.py
-drwxrwxrwx   0        0        0        0 2024-05-08 08:37:05.968096 besser_bot_framework-1.2.0/besser/bot/platforms/websocket/
--rw-rw-rw-   0        0        0     1546 2023-11-16 11:39:31.000000 besser_bot_framework-1.2.0/besser/bot/platforms/websocket/__init__.py
--rw-rw-rw-   0        0        0      793 2024-05-08 08:36:28.000000 besser_bot_framework-1.2.0/besser/bot/platforms/websocket/message.py
--rw-rw-rw-   0        0        0    11100 2024-05-08 08:36:28.000000 besser_bot_framework-1.2.0/besser/bot/platforms/websocket/streamlit_ui.py
--rw-rw-rw-   0        0        0    10093 2024-05-08 08:36:28.000000 besser_bot_framework-1.2.0/besser/bot/platforms/websocket/websocket_platform.py
-drwxrwxrwx   0        0        0        0 2024-05-08 08:37:05.969097 besser_bot_framework-1.2.0/besser/bot/test/
--rw-rw-rw-   0        0        0        0 2023-10-24 13:15:57.000000 besser_bot_framework-1.2.0/besser/bot/test/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-08 08:37:05.974096 besser_bot_framework-1.2.0/besser/bot/test/examples/
--rw-rw-rw-   0        0        0        0 2023-10-24 13:15:57.000000 besser_bot_framework-1.2.0/besser/bot/test/examples/__init__.py
--rw-rw-rw-   0        0        0     1876 2024-05-08 08:36:28.000000 besser_bot_framework-1.2.0/besser/bot/test/examples/greetings_bot.py
--rw-rw-rw-   0        0        0     3303 2024-05-08 07:50:07.000000 besser_bot_framework-1.2.0/besser/bot/test/examples/telegram_bot.py
--rw-rw-rw-   0        0        0     2075 2024-05-07 11:25:10.000000 besser_bot_framework-1.2.0/besser/bot/test/examples/weather_bot.py
-drwxrwxrwx   0        0        0        0 2024-05-08 08:37:05.982097 besser_bot_framework-1.2.0/besser_bot_framework.egg-info/
--rw-rw-rw-   0        0        0     3210 2024-05-08 08:37:05.000000 besser_bot_framework-1.2.0/besser_bot_framework.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2919 2024-05-08 08:37:05.000000 besser_bot_framework-1.2.0/besser_bot_framework.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 08:37:05.000000 besser_bot_framework-1.2.0/besser_bot_framework.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      431 2024-05-08 08:37:05.000000 besser_bot_framework-1.2.0/besser_bot_framework.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-08 08:37:05.000000 besser_bot_framework-1.2.0/besser_bot_framework.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       97 2023-10-24 13:11:01.000000 besser_bot_framework-1.2.0/pyproject.toml
--rw-rw-rw-   0        0        0      454 2024-05-08 08:37:01.000000 besser_bot_framework-1.2.0/requirements.txt
--rw-rw-rw-   0        0        0      711 2024-05-08 08:37:05.985096 besser_bot_framework-1.2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-08 12:13:01.452528 besser_bot_framework-1.2.1/
+-rw-rw-rw-   0        0        0     1090 2023-10-24 13:11:01.000000 besser_bot_framework-1.2.1/LICENSE
+-rw-rw-rw-   0        0        0     3204 2024-05-08 12:13:01.452528 besser_bot_framework-1.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1849 2024-01-22 15:17:03.000000 besser_bot_framework-1.2.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-08 12:13:01.361421 besser_bot_framework-1.2.1/besser/
+-rw-rw-rw-   0        0        0        0 2023-10-24 13:15:57.000000 besser_bot_framework-1.2.1/besser/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 12:13:01.362421 besser_bot_framework-1.2.1/besser/bot/
+-rw-rw-rw-   0        0        0        0 2023-10-24 13:15:57.000000 besser_bot_framework-1.2.1/besser/bot/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 12:13:01.370420 besser_bot_framework-1.2.1/besser/bot/core/
+-rw-rw-rw-   0        0        0        0 2023-10-24 13:15:57.000000 besser_bot_framework-1.2.1/besser/bot/core/__init__.py
+-rw-rw-rw-   0        0        0    20671 2024-05-08 08:36:28.000000 besser_bot_framework-1.2.1/besser/bot/core/bot.py
+drwxrwxrwx   0        0        0        0 2024-05-08 12:13:01.374424 besser_bot_framework-1.2.1/besser/bot/core/entity/
+-rw-rw-rw-   0        0        0        0 2023-10-24 13:15:57.000000 besser_bot_framework-1.2.1/besser/bot/core/entity/__init__.py
+-rw-rw-rw-   0        0        0     3098 2024-05-08 08:36:28.000000 besser_bot_framework-1.2.1/besser/bot/core/entity/entity.py
+-rw-rw-rw-   0        0        0      820 2023-10-24 13:16:24.000000 besser_bot_framework-1.2.1/besser/bot/core/entity/entity_entry.py
+-rw-rw-rw-   0        0        0     3855 2024-02-28 10:38:02.000000 besser_bot_framework-1.2.1/besser/bot/core/file.py
+drwxrwxrwx   0        0        0        0 2024-05-08 12:13:01.378423 besser_bot_framework-1.2.1/besser/bot/core/intent/
+-rw-rw-rw-   0        0        0        0 2023-10-24 13:15:57.000000 besser_bot_framework-1.2.1/besser/bot/core/intent/__init__.py
+-rw-rw-rw-   0        0        0     4815 2024-02-28 10:38:02.000000 besser_bot_framework-1.2.1/besser/bot/core/intent/intent.py
+-rw-rw-rw-   0        0        0     1187 2023-10-24 13:16:24.000000 besser_bot_framework-1.2.1/besser/bot/core/intent/intent_parameter.py
+-rw-rw-rw-   0        0        0     1077 2023-10-24 13:16:24.000000 besser_bot_framework-1.2.1/besser/bot/core/property.py
+-rw-rw-rw-   0        0        0     6585 2024-05-08 08:36:28.000000 besser_bot_framework-1.2.1/besser/bot/core/session.py
+-rw-rw-rw-   0        0        0    18203 2024-05-08 08:36:28.000000 besser_bot_framework-1.2.1/besser/bot/core/state.py
+-rw-rw-rw-   0        0        0     5258 2023-10-24 13:16:24.000000 besser_bot_framework-1.2.1/besser/bot/core/transition.py
+drwxrwxrwx   0        0        0        0 2024-05-08 12:13:01.380421 besser_bot_framework-1.2.1/besser/bot/db/
+-rw-rw-rw-   0        0        0     1648 2024-05-08 08:36:28.000000 besser_bot_framework-1.2.1/besser/bot/db/__init__.py
+-rw-rw-rw-   0        0        0    10274 2024-05-08 12:10:29.000000 besser_bot_framework-1.2.1/besser/bot/db/monitoring_db.py
+drwxrwxrwx   0        0        0        0 2024-05-08 12:13:01.383421 besser_bot_framework-1.2.1/besser/bot/exceptions/
+-rw-rw-rw-   0        0        0        0 2023-10-24 13:15:57.000000 besser_bot_framework-1.2.1/besser/bot/exceptions/__init__.py
+-rw-rw-rw-   0        0        0     4814 2024-02-28 10:38:02.000000 besser_bot_framework-1.2.1/besser/bot/exceptions/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-05-08 12:13:01.384421 besser_bot_framework-1.2.1/besser/bot/library/
+-rw-rw-rw-   0        0        0        0 2023-10-24 13:15:57.000000 besser_bot_framework-1.2.1/besser/bot/library/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 12:13:01.387421 besser_bot_framework-1.2.1/besser/bot/library/entity/
+-rw-rw-rw-   0        0        0        0 2023-10-24 13:15:57.000000 besser_bot_framework-1.2.1/besser/bot/library/entity/__init__.py
+-rw-rw-rw-   0        0        0     1423 2024-02-28 10:38:02.000000 besser_bot_framework-1.2.1/besser/bot/library/entity/base_entities.py
+drwxrwxrwx   0        0        0        0 2024-05-08 12:13:01.390422 besser_bot_framework-1.2.1/besser/bot/library/event/
+-rw-rw-rw-   0        0        0        0 2023-10-24 13:15:57.000000 besser_bot_framework-1.2.1/besser/bot/library/event/__init__.py
+-rw-rw-rw-   0        0        0     2729 2024-02-06 10:51:26.000000 besser_bot_framework-1.2.1/besser/bot/library/event/event_library.py
+-rw-rw-rw-   0        0        0      315 2023-10-24 13:16:24.000000 besser_bot_framework-1.2.1/besser/bot/library/event/event_template.py
+drwxrwxrwx   0        0        0        0 2024-05-08 12:13:01.394422 besser_bot_framework-1.2.1/besser/bot/library/intent/
+-rw-rw-rw-   0        0        0        0 2023-10-24 13:15:57.000000 besser_bot_framework-1.2.1/besser/bot/library/intent/__init__.py
+-rw-rw-rw-   0        0        0     2859 2024-02-28 10:38:02.000000 besser_bot_framework-1.2.1/besser/bot/library/intent/intent_classifier_configuration_library.py
+-rw-rw-rw-   0        0        0      239 2023-10-24 13:16:24.000000 besser_bot_framework-1.2.1/besser/bot/library/intent/intent_library.py
+drwxrwxrwx   0        0        0        0 2024-05-08 12:13:01.397425 besser_bot_framework-1.2.1/besser/bot/library/state/
+-rw-rw-rw-   0        0        0        0 2023-10-24 13:15:57.000000 besser_bot_framework-1.2.1/besser/bot/library/state/__init__.py
+-rw-rw-rw-   0        0        0      756 2024-02-19 15:24:24.000000 besser_bot_framework-1.2.1/besser/bot/library/state/state_library.py
+drwxrwxrwx   0        0        0        0 2024-05-08 12:13:01.400422 besser_bot_framework-1.2.1/besser/bot/nlp/
+-rw-rw-rw-   0        0        0     5328 2024-02-28 10:38:02.000000 besser_bot_framework-1.2.1/besser/bot/nlp/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 12:13:01.408422 besser_bot_framework-1.2.1/besser/bot/nlp/intent_classifier/
+-rw-rw-rw-   0        0        0        0 2023-10-24 13:15:57.000000 besser_bot_framework-1.2.1/besser/bot/nlp/intent_classifier/__init__.py
+-rw-rw-rw-   0        0        0     2299 2023-10-24 13:16:24.000000 besser_bot_framework-1.2.1/besser/bot/nlp/intent_classifier/intent_classifier.py
+-rw-rw-rw-   0        0        0     6907 2024-02-28 10:38:02.000000 besser_bot_framework-1.2.1/besser/bot/nlp/intent_classifier/intent_classifier_configuration.py
+-rw-rw-rw-   0        0        0     2896 2023-10-24 13:16:24.000000 besser_bot_framework-1.2.1/besser/bot/nlp/intent_classifier/intent_classifier_prediction.py
+-rw-rw-rw-   0        0        0    12208 2024-02-28 10:38:02.000000 besser_bot_framework-1.2.1/besser/bot/nlp/intent_classifier/llm_intent_classifier.py
+-rw-rw-rw-   0        0        0     7722 2024-02-28 10:38:02.000000 besser_bot_framework-1.2.1/besser/bot/nlp/intent_classifier/simple_intent_classifier.py
+drwxrwxrwx   0        0        0        0 2024-05-08 12:13:01.414455 besser_bot_framework-1.2.1/besser/bot/nlp/ner/
+-rw-rw-rw-   0        0        0        0 2023-10-24 13:15:57.000000 besser_bot_framework-1.2.1/besser/bot/nlp/ner/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 12:13:01.419429 besser_bot_framework-1.2.1/besser/bot/nlp/ner/base/
+-rw-rw-rw-   0        0        0        0 2023-10-24 13:15:57.000000 besser_bot_framework-1.2.1/besser/bot/nlp/ner/base/__init__.py
+-rw-rw-rw-   0        0        0      226 2023-10-24 13:16:24.000000 besser_bot_framework-1.2.1/besser/bot/nlp/ner/base/any.py
+-rw-rw-rw-   0        0        0     7050 2023-10-24 13:16:24.000000 besser_bot_framework-1.2.1/besser/bot/nlp/ner/base/datetime.py
+-rw-rw-rw-   0        0        0      975 2023-10-24 13:16:24.000000 besser_bot_framework-1.2.1/besser/bot/nlp/ner/base/number.py
+-rw-rw-rw-   0        0        0      786 2023-10-24 13:16:24.000000 besser_bot_framework-1.2.1/besser/bot/nlp/ner/matched_parameter.py
+-rw-rw-rw-   0        0        0     1576 2023-10-24 13:16:24.000000 besser_bot_framework-1.2.1/besser/bot/nlp/ner/ner.py
+-rw-rw-rw-   0        0        0     1891 2023-10-24 13:16:24.000000 besser_bot_framework-1.2.1/besser/bot/nlp/ner/ner_prediction.py
+-rw-rw-rw-   0        0        0    10536 2024-05-08 08:36:28.000000 besser_bot_framework-1.2.1/besser/bot/nlp/ner/simple_ner.py
+-rw-rw-rw-   0        0        0     7010 2024-02-28 10:38:02.000000 besser_bot_framework-1.2.1/besser/bot/nlp/nlp_engine.py
+drwxrwxrwx   0        0        0        0 2024-05-08 12:13:01.422447 besser_bot_framework-1.2.1/besser/bot/nlp/preprocessing/
+-rw-rw-rw-   0        0        0        0 2023-10-24 13:15:57.000000 besser_bot_framework-1.2.1/besser/bot/nlp/preprocessing/__init__.py
+-rw-rw-rw-   0        0        0      909 2023-12-10 20:05:59.000000 besser_bot_framework-1.2.1/besser/bot/nlp/preprocessing/pipelines.py
+-rw-rw-rw-   0        0        0     2787 2023-12-12 13:27:54.000000 besser_bot_framework-1.2.1/besser/bot/nlp/preprocessing/text_preprocessing.py
+drwxrwxrwx   0        0        0        0 2024-05-08 12:13:01.427527 besser_bot_framework-1.2.1/besser/bot/nlp/speech2text/
+-rw-rw-rw-   0        0        0        0 2023-11-16 11:39:31.000000 besser_bot_framework-1.2.1/besser/bot/nlp/speech2text/__init__.py
+-rw-rw-rw-   0        0        0     2294 2024-02-28 10:38:02.000000 besser_bot_framework-1.2.1/besser/bot/nlp/speech2text/api_speech2text.py
+-rw-rw-rw-   0        0        0     2302 2024-02-28 10:38:02.000000 besser_bot_framework-1.2.1/besser/bot/nlp/speech2text/hf_speech2text.py
+-rw-rw-rw-   0        0        0     1255 2023-11-16 11:39:31.000000 besser_bot_framework-1.2.1/besser/bot/nlp/speech2text/speech2text.py
+-rw-rw-rw-   0        0        0     1234 2024-02-28 10:38:02.000000 besser_bot_framework-1.2.1/besser/bot/nlp/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-08 12:13:01.430527 besser_bot_framework-1.2.1/besser/bot/platforms/
+-rw-rw-rw-   0        0        0        0 2023-10-24 13:15:57.000000 besser_bot_framework-1.2.1/besser/bot/platforms/__init__.py
+-rw-rw-rw-   0        0        0     3790 2024-05-08 08:36:28.000000 besser_bot_framework-1.2.1/besser/bot/platforms/payload.py
+-rw-rw-rw-   0        0        0     1787 2024-05-08 08:36:28.000000 besser_bot_framework-1.2.1/besser/bot/platforms/platform.py
+drwxrwxrwx   0        0        0        0 2024-05-08 12:13:01.433528 besser_bot_framework-1.2.1/besser/bot/platforms/telegram/
+-rw-rw-rw-   0        0        0      364 2023-11-16 11:39:31.000000 besser_bot_framework-1.2.1/besser/bot/platforms/telegram/__init__.py
+-rw-rw-rw-   0        0        0    11876 2024-05-08 08:36:28.000000 besser_bot_framework-1.2.1/besser/bot/platforms/telegram/telegram_platform.py
+drwxrwxrwx   0        0        0        0 2024-05-08 12:13:01.437531 besser_bot_framework-1.2.1/besser/bot/platforms/websocket/
+-rw-rw-rw-   0        0        0     1546 2023-11-16 11:39:31.000000 besser_bot_framework-1.2.1/besser/bot/platforms/websocket/__init__.py
+-rw-rw-rw-   0        0        0      793 2024-05-08 08:36:28.000000 besser_bot_framework-1.2.1/besser/bot/platforms/websocket/message.py
+-rw-rw-rw-   0        0        0    11100 2024-05-08 08:36:28.000000 besser_bot_framework-1.2.1/besser/bot/platforms/websocket/streamlit_ui.py
+-rw-rw-rw-   0        0        0    10093 2024-05-08 08:36:28.000000 besser_bot_framework-1.2.1/besser/bot/platforms/websocket/websocket_platform.py
+drwxrwxrwx   0        0        0        0 2024-05-08 12:13:01.439531 besser_bot_framework-1.2.1/besser/bot/test/
+-rw-rw-rw-   0        0        0        0 2023-10-24 13:15:57.000000 besser_bot_framework-1.2.1/besser/bot/test/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 12:13:01.443527 besser_bot_framework-1.2.1/besser/bot/test/examples/
+-rw-rw-rw-   0        0        0        0 2023-10-24 13:15:57.000000 besser_bot_framework-1.2.1/besser/bot/test/examples/__init__.py
+-rw-rw-rw-   0        0        0     1876 2024-05-08 08:36:28.000000 besser_bot_framework-1.2.1/besser/bot/test/examples/greetings_bot.py
+-rw-rw-rw-   0        0        0     3303 2024-05-08 07:50:07.000000 besser_bot_framework-1.2.1/besser/bot/test/examples/telegram_bot.py
+-rw-rw-rw-   0        0        0     2075 2024-05-07 11:25:10.000000 besser_bot_framework-1.2.1/besser/bot/test/examples/weather_bot.py
+drwxrwxrwx   0        0        0        0 2024-05-08 12:13:01.451529 besser_bot_framework-1.2.1/besser_bot_framework.egg-info/
+-rw-rw-rw-   0        0        0     3204 2024-05-08 12:13:01.000000 besser_bot_framework-1.2.1/besser_bot_framework.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2919 2024-05-08 12:13:01.000000 besser_bot_framework-1.2.1/besser_bot_framework.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 12:13:01.000000 besser_bot_framework-1.2.1/besser_bot_framework.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      431 2024-05-08 12:13:01.000000 besser_bot_framework-1.2.1/besser_bot_framework.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-08 12:13:01.000000 besser_bot_framework-1.2.1/besser_bot_framework.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       97 2023-10-24 13:11:01.000000 besser_bot_framework-1.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0      454 2024-05-08 12:12:35.000000 besser_bot_framework-1.2.1/requirements.txt
+-rw-rw-rw-   0        0        0      704 2024-05-08 12:13:01.454527 besser_bot_framework-1.2.1/setup.cfg
```

### Comparing `besser_bot_framework-1.2.0/LICENSE` & `besser_bot_framework-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `besser_bot_framework-1.2.0/PKG-INFO` & `besser_bot_framework-1.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: besser-bot-framework
-Version: 1.2.0
+Version: 1.2.1
 Summary: BESSER Bot Framework (BBF)
 Author: Luxembourg Institute of Science and Technology
 License: MIT
 Project-URL: Documentation, https://besserbot-framework.readthedocs.io/
 Project-URL: Source Code, https://github.com/BESSER-PEARL/BESSER-Bot-Framework
 Project-URL: Bug Tracker, https://github.com/BESSER-PEARL/BESSER-Bot-Framework/issues
 Keywords: bot,framework,chatbot,state-machine,nlp
-Requires-Python: <3.12,>=3.11
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: audio-recorder-streamlit==0.0.8
 Requires-Dist: dateparser==1.1.8
 Requires-Dist: keras==2.14.0
 Requires-Dist: librosa==0.10.1
 Requires-Dist: nltk==3.8.1
```

### Comparing `besser_bot_framework-1.2.0/README.md` & `besser_bot_framework-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `besser_bot_framework-1.2.0/besser/bot/core/bot.py` & `besser_bot_framework-1.2.1/besser/bot/core/bot.py`

 * *Files identical despite different names*

### Comparing `besser_bot_framework-1.2.0/besser/bot/core/entity/entity.py` & `besser_bot_framework-1.2.1/besser/bot/core/entity/entity.py`

 * *Files identical despite different names*

### Comparing `besser_bot_framework-1.2.0/besser/bot/core/entity/entity_entry.py` & `besser_bot_framework-1.2.1/besser/bot/core/entity/entity_entry.py`

 * *Files identical despite different names*

### Comparing `besser_bot_framework-1.2.0/besser/bot/core/file.py` & `besser_bot_framework-1.2.1/besser/bot/core/file.py`

 * *Files identical despite different names*

### Comparing `besser_bot_framework-1.2.0/besser/bot/core/intent/intent.py` & `besser_bot_framework-1.2.1/besser/bot/core/intent/intent.py`

 * *Files identical despite different names*

### Comparing `besser_bot_framework-1.2.0/besser/bot/core/intent/intent_parameter.py` & `besser_bot_framework-1.2.1/besser/bot/core/intent/intent_parameter.py`

 * *Files identical despite different names*

### Comparing `besser_bot_framework-1.2.0/besser/bot/core/property.py` & `besser_bot_framework-1.2.1/besser/bot/core/property.py`

 * *Files identical despite different names*

### Comparing `besser_bot_framework-1.2.0/besser/bot/core/session.py` & `besser_bot_framework-1.2.1/besser/bot/core/session.py`

 * *Files identical despite different names*

### Comparing `besser_bot_framework-1.2.0/besser/bot/core/state.py` & `besser_bot_framework-1.2.1/besser/bot/core/state.py`

 * *Files identical despite different names*

### Comparing `besser_bot_framework-1.2.0/besser/bot/core/transition.py` & `besser_bot_framework-1.2.1/besser/bot/core/transition.py`

 * *Files identical despite different names*

### Comparing `besser_bot_framework-1.2.0/besser/bot/db/__init__.py` & `besser_bot_framework-1.2.1/besser/bot/db/__init__.py`

 * *Files identical despite different names*

### Comparing `besser_bot_framework-1.2.0/besser/bot/db/monitoring_db.py` & `besser_bot_framework-1.2.1/besser/bot/db/monitoring_db.py`

 * *Files identical despite different names*

### Comparing `besser_bot_framework-1.2.0/besser/bot/exceptions/exceptions.py` & `besser_bot_framework-1.2.1/besser/bot/exceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `besser_bot_framework-1.2.0/besser/bot/library/entity/base_entities.py` & `besser_bot_framework-1.2.1/besser/bot/library/entity/base_entities.py`

 * *Files identical despite different names*

### Comparing `besser_bot_framework-1.2.0/besser/bot/library/event/event_library.py` & `besser_bot_framework-1.2.1/besser/bot/library/event/event_library.py`

 * *Files identical despite different names*

### Comparing `besser_bot_framework-1.2.0/besser/bot/library/intent/intent_classifier_configuration_library.py` & `besser_bot_framework-1.2.1/besser/bot/library/intent/intent_classifier_configuration_library.py`

 * *Files identical despite different names*

### Comparing `besser_bot_framework-1.2.0/besser/bot/library/state/state_library.py` & `besser_bot_framework-1.2.1/besser/bot/library/state/state_library.py`

 * *Files identical despite different names*

### Comparing `besser_bot_framework-1.2.0/besser/bot/nlp/__init__.py` & `besser_bot_framework-1.2.1/besser/bot/nlp/__init__.py`

 * *Files identical despite different names*

### Comparing `besser_bot_framework-1.2.0/besser/bot/nlp/intent_classifier/intent_classifier.py` & `besser_bot_framework-1.2.1/besser/bot/nlp/intent_classifier/intent_classifier.py`

 * *Files identical despite different names*

### Comparing `besser_bot_framework-1.2.0/besser/bot/nlp/intent_classifier/intent_classifier_configuration.py` & `besser_bot_framework-1.2.1/besser/bot/nlp/intent_classifier/intent_classifier_configuration.py`

 * *Files identical despite different names*

### Comparing `besser_bot_framework-1.2.0/besser/bot/nlp/intent_classifier/intent_classifier_prediction.py` & `besser_bot_framework-1.2.1/besser/bot/nlp/intent_classifier/intent_classifier_prediction.py`

 * *Files identical despite different names*

### Comparing `besser_bot_framework-1.2.0/besser/bot/nlp/intent_classifier/llm_intent_classifier.py` & `besser_bot_framework-1.2.1/besser/bot/nlp/intent_classifier/llm_intent_classifier.py`

 * *Files identical despite different names*

### Comparing `besser_bot_framework-1.2.0/besser/bot/nlp/intent_classifier/simple_intent_classifier.py` & `besser_bot_framework-1.2.1/besser/bot/nlp/intent_classifier/simple_intent_classifier.py`

 * *Files identical despite different names*

### Comparing `besser_bot_framework-1.2.0/besser/bot/nlp/ner/base/datetime.py` & `besser_bot_framework-1.2.1/besser/bot/nlp/ner/base/datetime.py`

 * *Files identical despite different names*

### Comparing `besser_bot_framework-1.2.0/besser/bot/nlp/ner/base/number.py` & `besser_bot_framework-1.2.1/besser/bot/nlp/ner/base/number.py`

 * *Files identical despite different names*

### Comparing `besser_bot_framework-1.2.0/besser/bot/nlp/ner/matched_parameter.py` & `besser_bot_framework-1.2.1/besser/bot/nlp/ner/matched_parameter.py`

 * *Files identical despite different names*

### Comparing `besser_bot_framework-1.2.0/besser/bot/nlp/ner/ner.py` & `besser_bot_framework-1.2.1/besser/bot/nlp/ner/ner.py`

 * *Files identical despite different names*

### Comparing `besser_bot_framework-1.2.0/besser/bot/nlp/ner/ner_prediction.py` & `besser_bot_framework-1.2.1/besser/bot/nlp/ner/ner_prediction.py`

 * *Files identical despite different names*

### Comparing `besser_bot_framework-1.2.0/besser/bot/nlp/ner/simple_ner.py` & `besser_bot_framework-1.2.1/besser/bot/nlp/ner/simple_ner.py`

 * *Files identical despite different names*

### Comparing `besser_bot_framework-1.2.0/besser/bot/nlp/nlp_engine.py` & `besser_bot_framework-1.2.1/besser/bot/nlp/nlp_engine.py`

 * *Files identical despite different names*

### Comparing `besser_bot_framework-1.2.0/besser/bot/nlp/preprocessing/pipelines.py` & `besser_bot_framework-1.2.1/besser/bot/nlp/preprocessing/pipelines.py`

 * *Files identical despite different names*

### Comparing `besser_bot_framework-1.2.0/besser/bot/nlp/preprocessing/text_preprocessing.py` & `besser_bot_framework-1.2.1/besser/bot/nlp/preprocessing/text_preprocessing.py`

 * *Files identical despite different names*

### Comparing `besser_bot_framework-1.2.0/besser/bot/nlp/speech2text/api_speech2text.py` & `besser_bot_framework-1.2.1/besser/bot/nlp/speech2text/api_speech2text.py`

 * *Files identical despite different names*

### Comparing `besser_bot_framework-1.2.0/besser/bot/nlp/speech2text/hf_speech2text.py` & `besser_bot_framework-1.2.1/besser/bot/nlp/speech2text/hf_speech2text.py`

 * *Files identical despite different names*

### Comparing `besser_bot_framework-1.2.0/besser/bot/nlp/speech2text/speech2text.py` & `besser_bot_framework-1.2.1/besser/bot/nlp/speech2text/speech2text.py`

 * *Files identical despite different names*

### Comparing `besser_bot_framework-1.2.0/besser/bot/nlp/utils.py` & `besser_bot_framework-1.2.1/besser/bot/nlp/utils.py`

 * *Files identical despite different names*

### Comparing `besser_bot_framework-1.2.0/besser/bot/platforms/payload.py` & `besser_bot_framework-1.2.1/besser/bot/platforms/payload.py`

 * *Files identical despite different names*

### Comparing `besser_bot_framework-1.2.0/besser/bot/platforms/platform.py` & `besser_bot_framework-1.2.1/besser/bot/platforms/platform.py`

 * *Files identical despite different names*

### Comparing `besser_bot_framework-1.2.0/besser/bot/platforms/telegram/telegram_platform.py` & `besser_bot_framework-1.2.1/besser/bot/platforms/telegram/telegram_platform.py`

 * *Files identical despite different names*

### Comparing `besser_bot_framework-1.2.0/besser/bot/platforms/websocket/__init__.py` & `besser_bot_framework-1.2.1/besser/bot/platforms/websocket/__init__.py`

 * *Files identical despite different names*

### Comparing `besser_bot_framework-1.2.0/besser/bot/platforms/websocket/message.py` & `besser_bot_framework-1.2.1/besser/bot/platforms/websocket/message.py`

 * *Files identical despite different names*

### Comparing `besser_bot_framework-1.2.0/besser/bot/platforms/websocket/streamlit_ui.py` & `besser_bot_framework-1.2.1/besser/bot/platforms/websocket/streamlit_ui.py`

 * *Files identical despite different names*

### Comparing `besser_bot_framework-1.2.0/besser/bot/platforms/websocket/websocket_platform.py` & `besser_bot_framework-1.2.1/besser/bot/platforms/websocket/websocket_platform.py`

 * *Files identical despite different names*

### Comparing `besser_bot_framework-1.2.0/besser/bot/test/examples/greetings_bot.py` & `besser_bot_framework-1.2.1/besser/bot/test/examples/greetings_bot.py`

 * *Files identical despite different names*

### Comparing `besser_bot_framework-1.2.0/besser/bot/test/examples/telegram_bot.py` & `besser_bot_framework-1.2.1/besser/bot/test/examples/telegram_bot.py`

 * *Files identical despite different names*

### Comparing `besser_bot_framework-1.2.0/besser/bot/test/examples/weather_bot.py` & `besser_bot_framework-1.2.1/besser/bot/test/examples/weather_bot.py`

 * *Files identical despite different names*

### Comparing `besser_bot_framework-1.2.0/besser_bot_framework.egg-info/PKG-INFO` & `besser_bot_framework-1.2.1/besser_bot_framework.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: besser-bot-framework
-Version: 1.2.0
+Version: 1.2.1
 Summary: BESSER Bot Framework (BBF)
 Author: Luxembourg Institute of Science and Technology
 License: MIT
 Project-URL: Documentation, https://besserbot-framework.readthedocs.io/
 Project-URL: Source Code, https://github.com/BESSER-PEARL/BESSER-Bot-Framework
 Project-URL: Bug Tracker, https://github.com/BESSER-PEARL/BESSER-Bot-Framework/issues
 Keywords: bot,framework,chatbot,state-machine,nlp
-Requires-Python: <3.12,>=3.11
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: audio-recorder-streamlit==0.0.8
 Requires-Dist: dateparser==1.1.8
 Requires-Dist: keras==2.14.0
 Requires-Dist: librosa==0.10.1
 Requires-Dist: nltk==3.8.1
```

### Comparing `besser_bot_framework-1.2.0/besser_bot_framework.egg-info/SOURCES.txt` & `besser_bot_framework-1.2.1/besser_bot_framework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `besser_bot_framework-1.2.0/setup.cfg` & `besser_bot_framework-1.2.1/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2062 6573 7365 722d 626f 742d 6672   = besser-bot-fr
 00000020: 616d 6577 6f72 6b0d 0a76 6572 7369 6f6e  amework..version
-00000030: 203d 2031 2e32 2e30 0d0a 6175 7468 6f72   = 1.2.0..author
+00000030: 203d 2031 2e32 2e31 0d0a 6175 7468 6f72   = 1.2.1..author
 00000040: 203d 204c 7578 656d 626f 7572 6720 496e   = Luxembourg In
 00000050: 7374 6974 7574 6520 6f66 2053 6369 656e  stitute of Scien
 00000060: 6365 2061 6e64 2054 6563 686e 6f6c 6f67  ce and Technolog
 00000070: 790d 0a64 6573 6372 6970 7469 6f6e 203d  y..description =
 00000080: 2042 4553 5345 5220 426f 7420 4672 616d   BESSER Bot Fram
 00000090: 6577 6f72 6b20 2842 4246 290d 0a6c 6f6e  ework (BBF)..lon
 000000a0: 675f 6465 7363 7269 7074 696f 6e20 3d20  g_description = 
@@ -31,15 +31,14 @@
 000001e0: 6672 616d 6577 6f72 6b2c 2063 6861 7462  framework, chatb
 000001f0: 6f74 2c20 7374 6174 652d 6d61 6368 696e  ot, state-machin
 00000200: 652c 206e 6c70 0d0a 6c69 6365 6e73 6520  e, nlp..license 
 00000210: 3d20 4d49 540d 0a6c 6963 656e 7365 5f66  = MIT..license_f
 00000220: 696c 6573 203d 204c 4943 454e 5345 0d0a  iles = LICENSE..
 00000230: 0d0a 5b6f 7074 696f 6e73 5d0d 0a70 7974  ..[options]..pyt
 00000240: 686f 6e5f 7265 7175 6972 6573 203d 203e  hon_requires = >
-00000250: 3d33 2e31 312c 203c 332e 3132 0d0a 7061  =3.11, <3.12..pa
-00000260: 636b 6167 6573 203d 2066 696e 643a 0d0a  ckages = find:..
-00000270: 696e 7374 616c 6c5f 7265 7175 6972 6573  install_requires
-00000280: 203d 2066 696c 653a 2072 6571 7569 7265   = file: require
-00000290: 6d65 6e74 732e 7478 740d 0a0d 0a5b 6567  ments.txt....[eg
-000002a0: 675f 696e 666f 5d0d 0a74 6167 5f62 7569  g_info]..tag_bui
-000002b0: 6c64 203d 200d 0a74 6167 5f64 6174 6520  ld = ..tag_date 
-000002c0: 3d20 300d 0a0d 0a                        = 0....
+00000250: 3d33 2e31 300d 0a70 6163 6b61 6765 7320  =3.10..packages 
+00000260: 3d20 6669 6e64 3a0d 0a69 6e73 7461 6c6c  = find:..install
+00000270: 5f72 6571 7569 7265 7320 3d20 6669 6c65  _requires = file
+00000280: 3a20 7265 7175 6972 656d 656e 7473 2e74  : requirements.t
+00000290: 7874 0d0a 0d0a 5b65 6767 5f69 6e66 6f5d  xt....[egg_info]
+000002a0: 0d0a 7461 675f 6275 696c 6420 3d20 0d0a  ..tag_build = ..
+000002b0: 7461 675f 6461 7465 203d 2030 0d0a 0d0a  tag_date = 0....
```

