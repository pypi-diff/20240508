# Comparing `tmp/besser_bot_framework-1.1.0.tar.gz` & `tmp/besser_bot_framework-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "besser_bot_framework-1.1.0.tar", last modified: Wed May  8 08:35:52 2024, max compression
+gzip compressed data, was "besser_bot_framework-1.2.0.tar", last modified: Wed May  8 08:37:05 2024, max compression
```

## Comparing `besser_bot_framework-1.1.0.tar` & `besser_bot_framework-1.2.0.tar`

### file list

```diff
@@ -1,102 +1,105 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 08:35:52.842762 besser_bot_framework-1.1.0/
--rw-rw-rw-   0        0        0     1090 2023-10-24 13:11:01.000000 besser_bot_framework-1.1.0/LICENSE
--rw-rw-rw-   0        0        0     3136 2024-05-08 08:35:52.841762 besser_bot_framework-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1849 2024-01-22 15:17:03.000000 besser_bot_framework-1.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-08 08:35:52.748685 besser_bot_framework-1.1.0/besser/
--rw-rw-rw-   0        0        0        0 2023-10-24 13:15:57.000000 besser_bot_framework-1.1.0/besser/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-08 08:35:52.749685 besser_bot_framework-1.1.0/besser/bot/
--rw-rw-rw-   0        0        0        0 2023-10-24 13:15:57.000000 besser_bot_framework-1.1.0/besser/bot/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-08 08:35:52.758686 besser_bot_framework-1.1.0/besser/bot/core/
--rw-rw-rw-   0        0        0        0 2023-10-24 13:15:57.000000 besser_bot_framework-1.1.0/besser/bot/core/__init__.py
--rw-rw-rw-   0        0        0    18343 2024-05-08 08:23:08.000000 besser_bot_framework-1.1.0/besser/bot/core/bot.py
-drwxrwxrwx   0        0        0        0 2024-05-08 08:35:52.762684 besser_bot_framework-1.1.0/besser/bot/core/entity/
--rw-rw-rw-   0        0        0        0 2023-10-24 13:15:57.000000 besser_bot_framework-1.1.0/besser/bot/core/entity/__init__.py
--rw-rw-rw-   0        0        0     3098 2024-05-08 08:23:08.000000 besser_bot_framework-1.1.0/besser/bot/core/entity/entity.py
--rw-rw-rw-   0        0        0      820 2023-10-24 13:16:24.000000 besser_bot_framework-1.1.0/besser/bot/core/entity/entity_entry.py
--rw-rw-rw-   0        0        0     3855 2024-02-28 10:38:02.000000 besser_bot_framework-1.1.0/besser/bot/core/file.py
-drwxrwxrwx   0        0        0        0 2024-05-08 08:35:52.765684 besser_bot_framework-1.1.0/besser/bot/core/intent/
--rw-rw-rw-   0        0        0        0 2023-10-24 13:15:57.000000 besser_bot_framework-1.1.0/besser/bot/core/intent/__init__.py
--rw-rw-rw-   0        0        0     4815 2024-02-28 10:38:02.000000 besser_bot_framework-1.1.0/besser/bot/core/intent/intent.py
--rw-rw-rw-   0        0        0     1187 2023-10-24 13:16:24.000000 besser_bot_framework-1.1.0/besser/bot/core/intent/intent_parameter.py
--rw-rw-rw-   0        0        0     1077 2023-10-24 13:16:24.000000 besser_bot_framework-1.1.0/besser/bot/core/property.py
--rw-rw-rw-   0        0        0     6515 2024-05-08 08:23:08.000000 besser_bot_framework-1.1.0/besser/bot/core/session.py
--rw-rw-rw-   0        0        0    18203 2024-05-08 08:23:08.000000 besser_bot_framework-1.1.0/besser/bot/core/state.py
--rw-rw-rw-   0        0        0     5258 2023-10-24 13:16:24.000000 besser_bot_framework-1.1.0/besser/bot/core/transition.py
-drwxrwxrwx   0        0        0        0 2024-05-08 08:35:52.768708 besser_bot_framework-1.1.0/besser/bot/exceptions/
--rw-rw-rw-   0        0        0        0 2023-10-24 13:15:57.000000 besser_bot_framework-1.1.0/besser/bot/exceptions/__init__.py
--rw-rw-rw-   0        0        0     4814 2024-02-28 10:38:02.000000 besser_bot_framework-1.1.0/besser/bot/exceptions/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-05-08 08:35:52.769685 besser_bot_framework-1.1.0/besser/bot/library/
--rw-rw-rw-   0        0        0        0 2023-10-24 13:15:57.000000 besser_bot_framework-1.1.0/besser/bot/library/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-08 08:35:52.772684 besser_bot_framework-1.1.0/besser/bot/library/entity/
--rw-rw-rw-   0        0        0        0 2023-10-24 13:15:57.000000 besser_bot_framework-1.1.0/besser/bot/library/entity/__init__.py
--rw-rw-rw-   0        0        0     1423 2024-02-28 10:38:02.000000 besser_bot_framework-1.1.0/besser/bot/library/entity/base_entities.py
-drwxrwxrwx   0        0        0        0 2024-05-08 08:35:52.776685 besser_bot_framework-1.1.0/besser/bot/library/event/
--rw-rw-rw-   0        0        0        0 2023-10-24 13:15:57.000000 besser_bot_framework-1.1.0/besser/bot/library/event/__init__.py
--rw-rw-rw-   0        0        0     2729 2024-02-06 10:51:26.000000 besser_bot_framework-1.1.0/besser/bot/library/event/event_library.py
--rw-rw-rw-   0        0        0      315 2023-10-24 13:16:24.000000 besser_bot_framework-1.1.0/besser/bot/library/event/event_template.py
-drwxrwxrwx   0        0        0        0 2024-05-08 08:35:52.780684 besser_bot_framework-1.1.0/besser/bot/library/intent/
--rw-rw-rw-   0        0        0        0 2023-10-24 13:15:57.000000 besser_bot_framework-1.1.0/besser/bot/library/intent/__init__.py
--rw-rw-rw-   0        0        0     2859 2024-02-28 10:38:02.000000 besser_bot_framework-1.1.0/besser/bot/library/intent/intent_classifier_configuration_library.py
--rw-rw-rw-   0        0        0      239 2023-10-24 13:16:24.000000 besser_bot_framework-1.1.0/besser/bot/library/intent/intent_library.py
-drwxrwxrwx   0        0        0        0 2024-05-08 08:35:52.783685 besser_bot_framework-1.1.0/besser/bot/library/state/
--rw-rw-rw-   0        0        0        0 2023-10-24 13:15:57.000000 besser_bot_framework-1.1.0/besser/bot/library/state/__init__.py
--rw-rw-rw-   0        0        0      756 2024-02-19 15:24:24.000000 besser_bot_framework-1.1.0/besser/bot/library/state/state_library.py
-drwxrwxrwx   0        0        0        0 2024-05-08 08:35:52.787684 besser_bot_framework-1.1.0/besser/bot/nlp/
--rw-rw-rw-   0        0        0     5328 2024-02-28 10:38:02.000000 besser_bot_framework-1.1.0/besser/bot/nlp/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-08 08:35:52.794685 besser_bot_framework-1.1.0/besser/bot/nlp/intent_classifier/
--rw-rw-rw-   0        0        0        0 2023-10-24 13:15:57.000000 besser_bot_framework-1.1.0/besser/bot/nlp/intent_classifier/__init__.py
--rw-rw-rw-   0        0        0     2299 2023-10-24 13:16:24.000000 besser_bot_framework-1.1.0/besser/bot/nlp/intent_classifier/intent_classifier.py
--rw-rw-rw-   0        0        0     6907 2024-02-28 10:38:02.000000 besser_bot_framework-1.1.0/besser/bot/nlp/intent_classifier/intent_classifier_configuration.py
--rw-rw-rw-   0        0        0     2896 2023-10-24 13:16:24.000000 besser_bot_framework-1.1.0/besser/bot/nlp/intent_classifier/intent_classifier_prediction.py
--rw-rw-rw-   0        0        0    12208 2024-02-28 10:38:02.000000 besser_bot_framework-1.1.0/besser/bot/nlp/intent_classifier/llm_intent_classifier.py
--rw-rw-rw-   0        0        0     7722 2024-02-28 10:38:02.000000 besser_bot_framework-1.1.0/besser/bot/nlp/intent_classifier/simple_intent_classifier.py
-drwxrwxrwx   0        0        0        0 2024-05-08 08:35:52.801685 besser_bot_framework-1.1.0/besser/bot/nlp/ner/
--rw-rw-rw-   0        0        0        0 2023-10-24 13:15:57.000000 besser_bot_framework-1.1.0/besser/bot/nlp/ner/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-08 08:35:52.806687 besser_bot_framework-1.1.0/besser/bot/nlp/ner/base/
--rw-rw-rw-   0        0        0        0 2023-10-24 13:15:57.000000 besser_bot_framework-1.1.0/besser/bot/nlp/ner/base/__init__.py
--rw-rw-rw-   0        0        0      226 2023-10-24 13:16:24.000000 besser_bot_framework-1.1.0/besser/bot/nlp/ner/base/any.py
--rw-rw-rw-   0        0        0     7050 2023-10-24 13:16:24.000000 besser_bot_framework-1.1.0/besser/bot/nlp/ner/base/datetime.py
--rw-rw-rw-   0        0        0      975 2023-10-24 13:16:24.000000 besser_bot_framework-1.1.0/besser/bot/nlp/ner/base/number.py
--rw-rw-rw-   0        0        0      786 2023-10-24 13:16:24.000000 besser_bot_framework-1.1.0/besser/bot/nlp/ner/matched_parameter.py
--rw-rw-rw-   0        0        0     1576 2023-10-24 13:16:24.000000 besser_bot_framework-1.1.0/besser/bot/nlp/ner/ner.py
--rw-rw-rw-   0        0        0     1891 2023-10-24 13:16:24.000000 besser_bot_framework-1.1.0/besser/bot/nlp/ner/ner_prediction.py
--rw-rw-rw-   0        0        0    10536 2024-05-08 08:23:08.000000 besser_bot_framework-1.1.0/besser/bot/nlp/ner/simple_ner.py
--rw-rw-rw-   0        0        0     7010 2024-02-28 10:38:02.000000 besser_bot_framework-1.1.0/besser/bot/nlp/nlp_engine.py
-drwxrwxrwx   0        0        0        0 2024-05-08 08:35:52.810684 besser_bot_framework-1.1.0/besser/bot/nlp/preprocessing/
--rw-rw-rw-   0        0        0        0 2023-10-24 13:15:57.000000 besser_bot_framework-1.1.0/besser/bot/nlp/preprocessing/__init__.py
--rw-rw-rw-   0        0        0      909 2023-12-10 20:05:59.000000 besser_bot_framework-1.1.0/besser/bot/nlp/preprocessing/pipelines.py
--rw-rw-rw-   0        0        0     2787 2023-12-12 13:27:54.000000 besser_bot_framework-1.1.0/besser/bot/nlp/preprocessing/text_preprocessing.py
-drwxrwxrwx   0        0        0        0 2024-05-08 08:35:52.815684 besser_bot_framework-1.1.0/besser/bot/nlp/speech2text/
--rw-rw-rw-   0        0        0        0 2023-11-16 11:39:31.000000 besser_bot_framework-1.1.0/besser/bot/nlp/speech2text/__init__.py
--rw-rw-rw-   0        0        0     2294 2024-02-28 10:38:02.000000 besser_bot_framework-1.1.0/besser/bot/nlp/speech2text/api_speech2text.py
--rw-rw-rw-   0        0        0     2302 2024-02-28 10:38:02.000000 besser_bot_framework-1.1.0/besser/bot/nlp/speech2text/hf_speech2text.py
--rw-rw-rw-   0        0        0     1255 2023-11-16 11:39:31.000000 besser_bot_framework-1.1.0/besser/bot/nlp/speech2text/speech2text.py
--rw-rw-rw-   0        0        0     1234 2024-02-28 10:38:02.000000 besser_bot_framework-1.1.0/besser/bot/nlp/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-08 08:35:52.819684 besser_bot_framework-1.1.0/besser/bot/platforms/
--rw-rw-rw-   0        0        0        0 2023-10-24 13:15:57.000000 besser_bot_framework-1.1.0/besser/bot/platforms/__init__.py
--rw-rw-rw-   0        0        0     3535 2024-05-08 08:23:08.000000 besser_bot_framework-1.1.0/besser/bot/platforms/payload.py
--rw-rw-rw-   0        0        0     1787 2024-05-08 08:23:08.000000 besser_bot_framework-1.1.0/besser/bot/platforms/platform.py
-drwxrwxrwx   0        0        0        0 2024-05-08 08:35:52.821686 besser_bot_framework-1.1.0/besser/bot/platforms/telegram/
--rw-rw-rw-   0        0        0      364 2023-11-16 11:39:31.000000 besser_bot_framework-1.1.0/besser/bot/platforms/telegram/__init__.py
--rw-rw-rw-   0        0        0     8789 2024-05-08 08:23:08.000000 besser_bot_framework-1.1.0/besser/bot/platforms/telegram/telegram_platform.py
-drwxrwxrwx   0        0        0        0 2024-05-08 08:35:52.826688 besser_bot_framework-1.1.0/besser/bot/platforms/websocket/
--rw-rw-rw-   0        0        0     1546 2023-11-16 11:39:31.000000 besser_bot_framework-1.1.0/besser/bot/platforms/websocket/__init__.py
--rw-rw-rw-   0        0        0      793 2024-05-08 08:23:08.000000 besser_bot_framework-1.1.0/besser/bot/platforms/websocket/message.py
--rw-rw-rw-   0        0        0    10383 2024-05-08 08:23:08.000000 besser_bot_framework-1.1.0/besser/bot/platforms/websocket/streamlit_ui.py
--rw-rw-rw-   0        0        0     8806 2024-05-08 08:23:08.000000 besser_bot_framework-1.1.0/besser/bot/platforms/websocket/websocket_platform.py
-drwxrwxrwx   0        0        0        0 2024-05-08 08:35:52.827690 besser_bot_framework-1.1.0/besser/bot/test/
--rw-rw-rw-   0        0        0        0 2023-10-24 13:15:57.000000 besser_bot_framework-1.1.0/besser/bot/test/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-08 08:35:52.832689 besser_bot_framework-1.1.0/besser/bot/test/examples/
--rw-rw-rw-   0        0        0        0 2023-10-24 13:15:57.000000 besser_bot_framework-1.1.0/besser/bot/test/examples/__init__.py
--rw-rw-rw-   0        0        0     1875 2024-05-08 08:23:08.000000 besser_bot_framework-1.1.0/besser/bot/test/examples/greetings_bot.py
--rw-rw-rw-   0        0        0     3303 2024-05-08 07:50:07.000000 besser_bot_framework-1.1.0/besser/bot/test/examples/telegram_bot.py
--rw-rw-rw-   0        0        0     2075 2024-05-07 11:25:10.000000 besser_bot_framework-1.1.0/besser/bot/test/examples/weather_bot.py
-drwxrwxrwx   0        0        0        0 2024-05-08 08:35:52.840689 besser_bot_framework-1.1.0/besser_bot_framework.egg-info/
--rw-rw-rw-   0        0        0     3136 2024-05-08 08:35:52.000000 besser_bot_framework-1.1.0/besser_bot_framework.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2862 2024-05-08 08:35:52.000000 besser_bot_framework-1.1.0/besser_bot_framework.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 08:35:52.000000 besser_bot_framework-1.1.0/besser_bot_framework.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      389 2024-05-08 08:35:52.000000 besser_bot_framework-1.1.0/besser_bot_framework.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-08 08:35:52.000000 besser_bot_framework-1.1.0/besser_bot_framework.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       97 2023-10-24 13:11:01.000000 besser_bot_framework-1.1.0/pyproject.toml
--rw-rw-rw-   0        0        0      410 2024-05-08 08:35:30.000000 besser_bot_framework-1.1.0/requirements.txt
--rw-rw-rw-   0        0        0      711 2024-05-08 08:35:52.843763 besser_bot_framework-1.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-08 08:37:05.984097 besser_bot_framework-1.2.0/
+-rw-rw-rw-   0        0        0     1090 2023-10-24 13:11:01.000000 besser_bot_framework-1.2.0/LICENSE
+-rw-rw-rw-   0        0        0     3210 2024-05-08 08:37:05.984097 besser_bot_framework-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1849 2024-01-22 15:17:03.000000 besser_bot_framework-1.2.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-08 08:37:05.884907 besser_bot_framework-1.2.0/besser/
+-rw-rw-rw-   0        0        0        0 2023-10-24 13:15:57.000000 besser_bot_framework-1.2.0/besser/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 08:37:05.885907 besser_bot_framework-1.2.0/besser/bot/
+-rw-rw-rw-   0        0        0        0 2023-10-24 13:15:57.000000 besser_bot_framework-1.2.0/besser/bot/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 08:37:05.893907 besser_bot_framework-1.2.0/besser/bot/core/
+-rw-rw-rw-   0        0        0        0 2023-10-24 13:15:57.000000 besser_bot_framework-1.2.0/besser/bot/core/__init__.py
+-rw-rw-rw-   0        0        0    20671 2024-05-08 08:36:28.000000 besser_bot_framework-1.2.0/besser/bot/core/bot.py
+drwxrwxrwx   0        0        0        0 2024-05-08 08:37:05.896907 besser_bot_framework-1.2.0/besser/bot/core/entity/
+-rw-rw-rw-   0        0        0        0 2023-10-24 13:15:57.000000 besser_bot_framework-1.2.0/besser/bot/core/entity/__init__.py
+-rw-rw-rw-   0        0        0     3098 2024-05-08 08:36:28.000000 besser_bot_framework-1.2.0/besser/bot/core/entity/entity.py
+-rw-rw-rw-   0        0        0      820 2023-10-24 13:16:24.000000 besser_bot_framework-1.2.0/besser/bot/core/entity/entity_entry.py
+-rw-rw-rw-   0        0        0     3855 2024-02-28 10:38:02.000000 besser_bot_framework-1.2.0/besser/bot/core/file.py
+drwxrwxrwx   0        0        0        0 2024-05-08 08:37:05.900906 besser_bot_framework-1.2.0/besser/bot/core/intent/
+-rw-rw-rw-   0        0        0        0 2023-10-24 13:15:57.000000 besser_bot_framework-1.2.0/besser/bot/core/intent/__init__.py
+-rw-rw-rw-   0        0        0     4815 2024-02-28 10:38:02.000000 besser_bot_framework-1.2.0/besser/bot/core/intent/intent.py
+-rw-rw-rw-   0        0        0     1187 2023-10-24 13:16:24.000000 besser_bot_framework-1.2.0/besser/bot/core/intent/intent_parameter.py
+-rw-rw-rw-   0        0        0     1077 2023-10-24 13:16:24.000000 besser_bot_framework-1.2.0/besser/bot/core/property.py
+-rw-rw-rw-   0        0        0     6585 2024-05-08 08:36:28.000000 besser_bot_framework-1.2.0/besser/bot/core/session.py
+-rw-rw-rw-   0        0        0    18203 2024-05-08 08:36:28.000000 besser_bot_framework-1.2.0/besser/bot/core/state.py
+-rw-rw-rw-   0        0        0     5258 2023-10-24 13:16:24.000000 besser_bot_framework-1.2.0/besser/bot/core/transition.py
+drwxrwxrwx   0        0        0        0 2024-05-08 08:37:05.903906 besser_bot_framework-1.2.0/besser/bot/db/
+-rw-rw-rw-   0        0        0     1648 2024-05-08 08:36:28.000000 besser_bot_framework-1.2.0/besser/bot/db/__init__.py
+-rw-rw-rw-   0        0        0    10274 2024-05-08 08:36:28.000000 besser_bot_framework-1.2.0/besser/bot/db/monitoring_db.py
+drwxrwxrwx   0        0        0        0 2024-05-08 08:37:05.905908 besser_bot_framework-1.2.0/besser/bot/exceptions/
+-rw-rw-rw-   0        0        0        0 2023-10-24 13:15:57.000000 besser_bot_framework-1.2.0/besser/bot/exceptions/__init__.py
+-rw-rw-rw-   0        0        0     4814 2024-02-28 10:38:02.000000 besser_bot_framework-1.2.0/besser/bot/exceptions/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-05-08 08:37:05.907905 besser_bot_framework-1.2.0/besser/bot/library/
+-rw-rw-rw-   0        0        0        0 2023-10-24 13:15:57.000000 besser_bot_framework-1.2.0/besser/bot/library/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 08:37:05.909907 besser_bot_framework-1.2.0/besser/bot/library/entity/
+-rw-rw-rw-   0        0        0        0 2023-10-24 13:15:57.000000 besser_bot_framework-1.2.0/besser/bot/library/entity/__init__.py
+-rw-rw-rw-   0        0        0     1423 2024-02-28 10:38:02.000000 besser_bot_framework-1.2.0/besser/bot/library/entity/base_entities.py
+drwxrwxrwx   0        0        0        0 2024-05-08 08:37:05.913906 besser_bot_framework-1.2.0/besser/bot/library/event/
+-rw-rw-rw-   0        0        0        0 2023-10-24 13:15:57.000000 besser_bot_framework-1.2.0/besser/bot/library/event/__init__.py
+-rw-rw-rw-   0        0        0     2729 2024-02-06 10:51:26.000000 besser_bot_framework-1.2.0/besser/bot/library/event/event_library.py
+-rw-rw-rw-   0        0        0      315 2023-10-24 13:16:24.000000 besser_bot_framework-1.2.0/besser/bot/library/event/event_template.py
+drwxrwxrwx   0        0        0        0 2024-05-08 08:37:05.917906 besser_bot_framework-1.2.0/besser/bot/library/intent/
+-rw-rw-rw-   0        0        0        0 2023-10-24 13:15:57.000000 besser_bot_framework-1.2.0/besser/bot/library/intent/__init__.py
+-rw-rw-rw-   0        0        0     2859 2024-02-28 10:38:02.000000 besser_bot_framework-1.2.0/besser/bot/library/intent/intent_classifier_configuration_library.py
+-rw-rw-rw-   0        0        0      239 2023-10-24 13:16:24.000000 besser_bot_framework-1.2.0/besser/bot/library/intent/intent_library.py
+drwxrwxrwx   0        0        0        0 2024-05-08 08:37:05.920947 besser_bot_framework-1.2.0/besser/bot/library/state/
+-rw-rw-rw-   0        0        0        0 2023-10-24 13:15:57.000000 besser_bot_framework-1.2.0/besser/bot/library/state/__init__.py
+-rw-rw-rw-   0        0        0      756 2024-02-19 15:24:24.000000 besser_bot_framework-1.2.0/besser/bot/library/state/state_library.py
+drwxrwxrwx   0        0        0        0 2024-05-08 08:37:05.924945 besser_bot_framework-1.2.0/besser/bot/nlp/
+-rw-rw-rw-   0        0        0     5328 2024-02-28 10:38:02.000000 besser_bot_framework-1.2.0/besser/bot/nlp/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 08:37:05.933946 besser_bot_framework-1.2.0/besser/bot/nlp/intent_classifier/
+-rw-rw-rw-   0        0        0        0 2023-10-24 13:15:57.000000 besser_bot_framework-1.2.0/besser/bot/nlp/intent_classifier/__init__.py
+-rw-rw-rw-   0        0        0     2299 2023-10-24 13:16:24.000000 besser_bot_framework-1.2.0/besser/bot/nlp/intent_classifier/intent_classifier.py
+-rw-rw-rw-   0        0        0     6907 2024-02-28 10:38:02.000000 besser_bot_framework-1.2.0/besser/bot/nlp/intent_classifier/intent_classifier_configuration.py
+-rw-rw-rw-   0        0        0     2896 2023-10-24 13:16:24.000000 besser_bot_framework-1.2.0/besser/bot/nlp/intent_classifier/intent_classifier_prediction.py
+-rw-rw-rw-   0        0        0    12208 2024-02-28 10:38:02.000000 besser_bot_framework-1.2.0/besser/bot/nlp/intent_classifier/llm_intent_classifier.py
+-rw-rw-rw-   0        0        0     7722 2024-02-28 10:38:02.000000 besser_bot_framework-1.2.0/besser/bot/nlp/intent_classifier/simple_intent_classifier.py
+drwxrwxrwx   0        0        0        0 2024-05-08 08:37:05.940097 besser_bot_framework-1.2.0/besser/bot/nlp/ner/
+-rw-rw-rw-   0        0        0        0 2023-10-24 13:15:57.000000 besser_bot_framework-1.2.0/besser/bot/nlp/ner/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 08:37:05.945119 besser_bot_framework-1.2.0/besser/bot/nlp/ner/base/
+-rw-rw-rw-   0        0        0        0 2023-10-24 13:15:57.000000 besser_bot_framework-1.2.0/besser/bot/nlp/ner/base/__init__.py
+-rw-rw-rw-   0        0        0      226 2023-10-24 13:16:24.000000 besser_bot_framework-1.2.0/besser/bot/nlp/ner/base/any.py
+-rw-rw-rw-   0        0        0     7050 2023-10-24 13:16:24.000000 besser_bot_framework-1.2.0/besser/bot/nlp/ner/base/datetime.py
+-rw-rw-rw-   0        0        0      975 2023-10-24 13:16:24.000000 besser_bot_framework-1.2.0/besser/bot/nlp/ner/base/number.py
+-rw-rw-rw-   0        0        0      786 2023-10-24 13:16:24.000000 besser_bot_framework-1.2.0/besser/bot/nlp/ner/matched_parameter.py
+-rw-rw-rw-   0        0        0     1576 2023-10-24 13:16:24.000000 besser_bot_framework-1.2.0/besser/bot/nlp/ner/ner.py
+-rw-rw-rw-   0        0        0     1891 2023-10-24 13:16:24.000000 besser_bot_framework-1.2.0/besser/bot/nlp/ner/ner_prediction.py
+-rw-rw-rw-   0        0        0    10536 2024-05-08 08:36:28.000000 besser_bot_framework-1.2.0/besser/bot/nlp/ner/simple_ner.py
+-rw-rw-rw-   0        0        0     7010 2024-02-28 10:38:02.000000 besser_bot_framework-1.2.0/besser/bot/nlp/nlp_engine.py
+drwxrwxrwx   0        0        0        0 2024-05-08 08:37:05.949097 besser_bot_framework-1.2.0/besser/bot/nlp/preprocessing/
+-rw-rw-rw-   0        0        0        0 2023-10-24 13:15:57.000000 besser_bot_framework-1.2.0/besser/bot/nlp/preprocessing/__init__.py
+-rw-rw-rw-   0        0        0      909 2023-12-10 20:05:59.000000 besser_bot_framework-1.2.0/besser/bot/nlp/preprocessing/pipelines.py
+-rw-rw-rw-   0        0        0     2787 2023-12-12 13:27:54.000000 besser_bot_framework-1.2.0/besser/bot/nlp/preprocessing/text_preprocessing.py
+drwxrwxrwx   0        0        0        0 2024-05-08 08:37:05.955097 besser_bot_framework-1.2.0/besser/bot/nlp/speech2text/
+-rw-rw-rw-   0        0        0        0 2023-11-16 11:39:31.000000 besser_bot_framework-1.2.0/besser/bot/nlp/speech2text/__init__.py
+-rw-rw-rw-   0        0        0     2294 2024-02-28 10:38:02.000000 besser_bot_framework-1.2.0/besser/bot/nlp/speech2text/api_speech2text.py
+-rw-rw-rw-   0        0        0     2302 2024-02-28 10:38:02.000000 besser_bot_framework-1.2.0/besser/bot/nlp/speech2text/hf_speech2text.py
+-rw-rw-rw-   0        0        0     1255 2023-11-16 11:39:31.000000 besser_bot_framework-1.2.0/besser/bot/nlp/speech2text/speech2text.py
+-rw-rw-rw-   0        0        0     1234 2024-02-28 10:38:02.000000 besser_bot_framework-1.2.0/besser/bot/nlp/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-08 08:37:05.960096 besser_bot_framework-1.2.0/besser/bot/platforms/
+-rw-rw-rw-   0        0        0        0 2023-10-24 13:15:57.000000 besser_bot_framework-1.2.0/besser/bot/platforms/__init__.py
+-rw-rw-rw-   0        0        0     3790 2024-05-08 08:36:28.000000 besser_bot_framework-1.2.0/besser/bot/platforms/payload.py
+-rw-rw-rw-   0        0        0     1787 2024-05-08 08:36:28.000000 besser_bot_framework-1.2.0/besser/bot/platforms/platform.py
+drwxrwxrwx   0        0        0        0 2024-05-08 08:37:05.962099 besser_bot_framework-1.2.0/besser/bot/platforms/telegram/
+-rw-rw-rw-   0        0        0      364 2023-11-16 11:39:31.000000 besser_bot_framework-1.2.0/besser/bot/platforms/telegram/__init__.py
+-rw-rw-rw-   0        0        0    11876 2024-05-08 08:36:28.000000 besser_bot_framework-1.2.0/besser/bot/platforms/telegram/telegram_platform.py
+drwxrwxrwx   0        0        0        0 2024-05-08 08:37:05.968096 besser_bot_framework-1.2.0/besser/bot/platforms/websocket/
+-rw-rw-rw-   0        0        0     1546 2023-11-16 11:39:31.000000 besser_bot_framework-1.2.0/besser/bot/platforms/websocket/__init__.py
+-rw-rw-rw-   0        0        0      793 2024-05-08 08:36:28.000000 besser_bot_framework-1.2.0/besser/bot/platforms/websocket/message.py
+-rw-rw-rw-   0        0        0    11100 2024-05-08 08:36:28.000000 besser_bot_framework-1.2.0/besser/bot/platforms/websocket/streamlit_ui.py
+-rw-rw-rw-   0        0        0    10093 2024-05-08 08:36:28.000000 besser_bot_framework-1.2.0/besser/bot/platforms/websocket/websocket_platform.py
+drwxrwxrwx   0        0        0        0 2024-05-08 08:37:05.969097 besser_bot_framework-1.2.0/besser/bot/test/
+-rw-rw-rw-   0        0        0        0 2023-10-24 13:15:57.000000 besser_bot_framework-1.2.0/besser/bot/test/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 08:37:05.974096 besser_bot_framework-1.2.0/besser/bot/test/examples/
+-rw-rw-rw-   0        0        0        0 2023-10-24 13:15:57.000000 besser_bot_framework-1.2.0/besser/bot/test/examples/__init__.py
+-rw-rw-rw-   0        0        0     1876 2024-05-08 08:36:28.000000 besser_bot_framework-1.2.0/besser/bot/test/examples/greetings_bot.py
+-rw-rw-rw-   0        0        0     3303 2024-05-08 07:50:07.000000 besser_bot_framework-1.2.0/besser/bot/test/examples/telegram_bot.py
+-rw-rw-rw-   0        0        0     2075 2024-05-07 11:25:10.000000 besser_bot_framework-1.2.0/besser/bot/test/examples/weather_bot.py
+drwxrwxrwx   0        0        0        0 2024-05-08 08:37:05.982097 besser_bot_framework-1.2.0/besser_bot_framework.egg-info/
+-rw-rw-rw-   0        0        0     3210 2024-05-08 08:37:05.000000 besser_bot_framework-1.2.0/besser_bot_framework.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2919 2024-05-08 08:37:05.000000 besser_bot_framework-1.2.0/besser_bot_framework.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 08:37:05.000000 besser_bot_framework-1.2.0/besser_bot_framework.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      431 2024-05-08 08:37:05.000000 besser_bot_framework-1.2.0/besser_bot_framework.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-08 08:37:05.000000 besser_bot_framework-1.2.0/besser_bot_framework.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       97 2023-10-24 13:11:01.000000 besser_bot_framework-1.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0      454 2024-05-08 08:37:01.000000 besser_bot_framework-1.2.0/requirements.txt
+-rw-rw-rw-   0        0        0      711 2024-05-08 08:37:05.985096 besser_bot_framework-1.2.0/setup.cfg
```

### Comparing `besser_bot_framework-1.1.0/LICENSE` & `besser_bot_framework-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `besser_bot_framework-1.1.0/PKG-INFO` & `besser_bot_framework-1.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: besser-bot-framework
-Version: 1.1.0
+Version: 1.2.0
 Summary: BESSER Bot Framework (BBF)
 Author: Luxembourg Institute of Science and Technology
 License: MIT
 Project-URL: Documentation, https://besserbot-framework.readthedocs.io/
 Project-URL: Source Code, https://github.com/BESSER-PEARL/BESSER-Bot-Framework
 Project-URL: Bug Tracker, https://github.com/BESSER-PEARL/BESSER-Bot-Framework/issues
 Keywords: bot,framework,chatbot,state-machine,nlp
@@ -16,20 +16,22 @@
 Requires-Dist: keras==2.14.0
 Requires-Dist: librosa==0.10.1
 Requires-Dist: nltk==3.8.1
 Requires-Dist: numpy==1.26.1
 Requires-Dist: openai==1.8.0
 Requires-Dist: pandas==2.1.1
 Requires-Dist: plotly==5.18.0
+Requires-Dist: psycopg2-binary==2.9.9
 Requires-Dist: python-telegram-bot==20.6
 Requires-Dist: replicate==0.23.1
 Requires-Dist: requests==2.31.0
 Requires-Dist: snowballstemmer==2.2.0
 Requires-Dist: spacy==3.7.2
 Requires-Dist: SpeechRecognition==3.10.0
+Requires-Dist: sqlalchemy==2.0.29
 Requires-Dist: streamlit==1.27.2
 Requires-Dist: tensorflow==2.14.0
 Requires-Dist: text2num==2.5.0
 Requires-Dist: transformers==4.37.0
 Requires-Dist: websocket-client==1.6.4
 Requires-Dist: websockets==11.0.3
```

### Comparing `besser_bot_framework-1.1.0/README.md` & `besser_bot_framework-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `besser_bot_framework-1.1.0/besser/bot/core/bot.py` & `besser_bot_framework-1.2.0/besser/bot/core/bot.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 import logging
 import operator
 import threading
 from configparser import ConfigParser
 from typing import Any, Callable
 
+from besser.bot.core.transition import Transition
+from besser.bot.db import DB_MONITORING
+from besser.bot.db.monitoring_db import MonitoringDB
 from besser.bot.core.entity.entity import Entity
 from besser.bot.core.intent.intent import Intent
 from besser.bot.core.intent.intent_parameter import IntentParameter
 from besser.bot.core.property import Property
 from besser.bot.core.session import Session
 from besser.bot.core.state import State
 from besser.bot.core.file import File
@@ -32,15 +35,17 @@
         _platforms (list[Platform]): The bot platforms
         _platforms_threads (list[threading.Thread]): The threads where the platforms are run
         _nlp_engine (NLPEngine): The bot NLP engine
         _config (ConfigParser): The bot configuration parameters
         _default_ic_config (IntentClassifierConfiguration): the intent classifier configuration used by default for the
             bot states
         _sessions (dict[str, Session]): The bot sessions
-        _trained (bool): Weather the bot has been trained or not. It must be trained before it starts its execution.
+        _trained (bool): Whether the bot has been trained or not. It must be trained before it starts its execution.
+        _monitoring_db (MonitoringDB): The monitoring component of the bot that communicates with a database to store
+            usage information for later visualization or analysis
         states (list[State]): The bot states
         intents (list[Intent]): The bot intents
         entities (list[Entity]): The bot entities
         global_initial_states (list[State, Intent]): List of tuples of initial global states and their triggering intent
         global_state_component (dict[State, list[State]]): Dictionary of global state components, where key is initial
             global state and values is set of states in corresponding global component
     """
@@ -50,14 +55,15 @@
         self._platforms: list[Platform] = []
         self._platforms_threads: list[threading.Thread] = []
         self._nlp_engine = NLPEngine(self)
         self._config: ConfigParser = ConfigParser()
         self._default_ic_config: IntentClassifierConfiguration = SimpleIntentClassifierConfiguration()
         self._sessions: dict[str, Session] = {}
         self._trained: bool = False
+        self._monitoring_db: MonitoringDB = None
         self.states: list[State] = []
         self.intents: list[Intent] = []
         self.entities: list[Entity] = []
         self.global_initial_states: list[tuple[State, Intent]] = []
         self.global_state_component: dict[State, list[State]] = dict()
 
     @property
@@ -135,15 +141,15 @@
                   initial: bool = False,
                   ic_config: IntentClassifierConfiguration or None = None
                   ) -> State:
         """Create a new state in the bot.
 
         Args:
             name (str): the state name. It must be unique in the bot.
-            initial (bool): weather the state is initial or not. A bot must have 1 initial state.
+            initial (bool): whether the state is initial or not. A bot must have 1 initial state.
             ic_config (IntentClassifierConfiguration or None): the intent classifier configuration for the state.
                 If None is provided, the bot's default one will be assigned to the state.
 
         Returns:
             State: the state
         """
         if not ic_config:
@@ -214,15 +220,15 @@
                    entries: dict[str, list[str]] or None = None,
                    description: str or None = None
                    ) -> Entity:
         """Create a new entity in the bot.
 
         Args:
             name (str): the entity name. It must be unique in the bot
-            base_entity (bool): weather the entity is a base entity or not (i.e. a custom entity)
+            base_entity (bool): whether the entity is a base entity or not (i.e. a custom entity)
             entries (dict[str, list[str]] or None): the entity entries
             description (str or None): a description of the entity, optional
 
         Returns:
             Entity: the entity
         """
         new_entity = Entity(name, base_entity, entries, description)
@@ -279,29 +285,37 @@
             thread.join()
         self._platforms_threads = []
 
     def run(self, train: bool = True, sleep: bool = True) -> None:
         """Start the execution of the bot.
 
         Args:
-            train (bool): weather to train the bot or not
-            sleep (bool): weather to sleep after running the bot or not, which means that this function will not return
+            train (bool): whether to train the bot or not
+            sleep (bool): whether to sleep after running the bot or not, which means that this function will not return
         """
         if train:
             self.train()
         if not self._trained:
             raise BotNotTrainedError(self)
+        if self.get_property(DB_MONITORING):
+            if not self._monitoring_db:
+                self._monitoring_db = MonitoringDB()
+            self._monitoring_db.connect_to_db(self)
+            if self._monitoring_db.connected:
+                self._monitoring_db.initialize_db()
         self._run_platforms()
         if sleep:
             idle = threading.Event()
             idle.wait()
 
     def stop(self) -> None:
         """Stop the bot execution."""
         self._stop_platforms()
+        if self.get_property(DB_MONITORING) and self._monitoring_db.connected:
+            self._monitoring_db.close_connection()
 
     def reset(self, session_id: str) -> Session or None:
         """Reset the bot current state and memory for the specified session. Then, restart the bot again for this session.
 
         Args:
             session_id (str): the session to reset
 
@@ -327,14 +341,15 @@
             session_id (str): the session that sends the message to the bot
             message (str): the message sent to the bot
         """
         session = self._sessions[session_id]
         # TODO: Raise exception SessionNotFound
         session.message = message
         session.predicted_intent = self._nlp_engine.predict_intent(session)
+        self._monitoring_db_insert_intent_prediction(session)
         logging.info(f'Received message: {message}')
         logging.info(f'Detected intent: {session.predicted_intent.intent.name}')
         for parameter in session.predicted_intent.matched_parameters:
             logging.info(f"Parameter '{parameter.name}': {parameter.value}, info = {parameter.info}")
         session.current_state.receive_intent(session)
 
     def receive_file(self, session_id: str, file: File) -> None:
@@ -379,15 +394,15 @@
         self._init_global_states()
         self._nlp_engine.initialize()
         logging.info(f'{self._name} training started')
         self._nlp_engine.train()
         logging.info(f'{self._name} training finished')
         self._trained = True
 
-    def get_session(self, session_id: str) -> Session or None:
+    def _get_session(self, session_id: str) -> Session or None:
         """Get a bot session.
 
         Args:
             session_id (str): the session id
 
         Returns:
             Session or None: the session, if exists, or None
@@ -415,17 +430,18 @@
             pass
         session = Session(session_id, self, platform)
         self._sessions[session_id] = session
         session.current_state.run(session)
         return session
 
     def get_or_create_session(self, session_id: str, platform: Platform) -> Session:
-        session = self.get_session(session_id)
+        session = self._get_session(session_id)
         if session is None:
             session = self._new_session(session_id, platform)
+            self._monitoring_db_insert_session(session)
         return session
 
     def delete_session(self, session_id: str) -> None:
         """Delete an existing bot session.
 
         Args:
             session_id (str): the session id
@@ -450,7 +466,37 @@
 
         Returns:
             TelegramPlatform: the telegram platform
         """
         telegram_platform = TelegramPlatform(self)
         self._platforms.append(telegram_platform)
         return telegram_platform
+
+    def _monitoring_db_insert_session(self, session: Session) -> None:
+        """Insert a session record into the monitoring database.
+
+        Args:
+            session (Session): the session of the current user
+        """
+        if self.get_property(DB_MONITORING) and self._monitoring_db.connected:
+            thread = threading.Thread(target=self._monitoring_db.insert_session, args=(session,))
+            thread.start()
+
+    def _monitoring_db_insert_intent_prediction(self, session: Session) -> None:
+        """Insert an intent prediction record into the monitoring database.
+
+        Args:
+            session (Session): the session of the current user
+        """
+        if self.get_property(DB_MONITORING) and self._monitoring_db.connected:
+            thread = threading.Thread(target=self._monitoring_db.insert_intent_prediction, args=(session,))
+            thread.start()
+
+    def _monitoring_db_insert_transition(self, session: Session, transition: Transition) -> None:
+        """Insert a transition record into the monitoring database.
+
+        Args:
+            session (Session): the session of the current user
+        """
+        if self.get_property(DB_MONITORING) and self._monitoring_db.connected:
+            thread = threading.Thread(target=self._monitoring_db.insert_transition, args=(session, transition))
+            thread.start()
```

### Comparing `besser_bot_framework-1.1.0/besser/bot/core/entity/entity.py` & `besser_bot_framework-1.2.0/besser/bot/core/entity/entity.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,21 +11,21 @@
     """The Entity core component of a bot.
 
     Entities are used to specify the type of information to extract from user inputs. These entities are embedded in
     intent parameters.
 
     Args:
         name (str): the entity's name
-        base_entity (bool): weather the entity is base or not (i.e. custom)
+        base_entity (bool): whether the entity is base or not (i.e. custom)
         entries (dict[str, list[str]] or None): the entity entries. If base_entity, there are no entries (i.e. None)
         description (str or None): a description of the entity, optional
 
     Attributes:
         name (str): The entity's name
-        base_entity (bool): Weather the entity is base or not (i.e. custom)
+        base_entity (bool): Whether the entity is base or not (i.e. custom)
         entries (list[EntityEntry] or None): The entity entries. If base_entity, there are no entries (i.e. None)
         description (str or None): a description of the entity, optional
     """
 
     def __init__(
             self,
             name: str,
```

### Comparing `besser_bot_framework-1.1.0/besser/bot/core/entity/entity_entry.py` & `besser_bot_framework-1.2.0/besser/bot/core/entity/entity_entry.py`

 * *Files identical despite different names*

### Comparing `besser_bot_framework-1.1.0/besser/bot/core/file.py` & `besser_bot_framework-1.2.0/besser/bot/core/file.py`

 * *Files identical despite different names*

### Comparing `besser_bot_framework-1.1.0/besser/bot/core/intent/intent.py` & `besser_bot_framework-1.2.0/besser/bot/core/intent/intent.py`

 * *Files identical despite different names*

### Comparing `besser_bot_framework-1.1.0/besser/bot/core/intent/intent_parameter.py` & `besser_bot_framework-1.2.0/besser/bot/core/intent/intent_parameter.py`

 * *Files identical despite different names*

### Comparing `besser_bot_framework-1.1.0/besser/bot/core/property.py` & `besser_bot_framework-1.2.0/besser/bot/core/property.py`

 * *Files identical despite different names*

### Comparing `besser_bot_framework-1.1.0/besser/bot/core/session.py` & `besser_bot_framework-1.2.0/besser/bot/core/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -156,14 +156,15 @@
     def move(self, transition: Transition):
         """Move to another bot state.
 
         Args:
             transition (Transition): the transition that points to the bot state to move
         """
         logging.info(transition.log())
+        self._bot._monitoring_db_insert_transition(self, transition)
         if any(transition.dest is global_state for global_state in self._bot.global_state_component):
             self.set("prev_state", self.current_state)
         self._current_state = transition.dest
         self._current_state.run(self)
 
     def reply(self, message: str) -> None:
         """A bot message (usually a reply to a user message) is sent to the session platform to show it to the user.
```

### Comparing `besser_bot_framework-1.1.0/besser/bot/core/state.py` & `besser_bot_framework-1.2.0/besser/bot/core/state.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,21 +25,21 @@
 
     The bot relies on a state machine to define its execution logic. Each state can run a set of actions, and the bot
     can navigate to other states through transitions that are triggered when events occur (e.g. an intent is matched).
 
     Args:
         bot (Bot): the bot the state belongs to
         name (str): the state's name
-        initial (bool): weather the state is initial or not
+        initial (bool): whether the state is initial or not
         ic_config (IntentClassifierConfiguration): the intent classifier configuration of the state
 
     Attributes:
         _bot (Bot): The bot the state belongs to
         _name (str): The state name
-        _initial (bool): Weather the state is initial or not
+        _initial (bool): Whether the state is initial or not
         _body (Callable[[Session], None]): The state body. It is a callable that takes as argument a
             :class:`~besser.bot.core.session.Session`. It will be run whenever the bot moves to this state.
         _fallback_body (Callable[[Session], None]): The state fallback body. It is a callable that takes as argument a
             :class:`~besser.bot.core.session.Session`. It will be run whenever the bot tries to move to another state,
             but it can't (e.g. an intent is matched but none of the current state's transitions are triggered on that
             intent)
         _ic_config (IntentClassifierConfiguration): the intent classifier configuration of the state
@@ -342,15 +342,15 @@
             self._fallback_body(session)
         except Exception as _:
             logging.error(f"An error occurred while executing '{self._fallback_body.__name__}' of state"
                           f"'{self._name}' in bot '{self._bot.name}'. See the attached exception:")
             traceback.print_exc()
 
     def _check_next_transition(self, session: Session) -> None:
-        """Check weather the first defined transition of the state is an `auto` transition, and if so, move to its
+        """Check whether the first defined transition of the state is an `auto` transition, and if so, move to its
         destination state.
 
         This method is intended to be called after running the body of a state.
 
         Args:
             session (Session): the user session
         """
```

### Comparing `besser_bot_framework-1.1.0/besser/bot/core/transition.py` & `besser_bot_framework-1.2.0/besser/bot/core/transition.py`

 * *Files identical despite different names*

### Comparing `besser_bot_framework-1.1.0/besser/bot/exceptions/exceptions.py` & `besser_bot_framework-1.2.0/besser/bot/exceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `besser_bot_framework-1.1.0/besser/bot/library/entity/base_entities.py` & `besser_bot_framework-1.2.0/besser/bot/library/entity/base_entities.py`

 * *Files identical despite different names*

### Comparing `besser_bot_framework-1.1.0/besser/bot/library/event/event_library.py` & `besser_bot_framework-1.2.0/besser/bot/library/event/event_library.py`

 * *Files identical despite different names*

### Comparing `besser_bot_framework-1.1.0/besser/bot/library/intent/intent_classifier_configuration_library.py` & `besser_bot_framework-1.2.0/besser/bot/library/intent/intent_classifier_configuration_library.py`

 * *Files identical despite different names*

### Comparing `besser_bot_framework-1.1.0/besser/bot/library/state/state_library.py` & `besser_bot_framework-1.2.0/besser/bot/library/state/state_library.py`

 * *Files identical despite different names*

### Comparing `besser_bot_framework-1.1.0/besser/bot/nlp/__init__.py` & `besser_bot_framework-1.2.0/besser/bot/nlp/__init__.py`

 * *Files identical despite different names*

### Comparing `besser_bot_framework-1.1.0/besser/bot/nlp/intent_classifier/intent_classifier.py` & `besser_bot_framework-1.2.0/besser/bot/nlp/intent_classifier/intent_classifier.py`

 * *Files identical despite different names*

### Comparing `besser_bot_framework-1.1.0/besser/bot/nlp/intent_classifier/intent_classifier_configuration.py` & `besser_bot_framework-1.2.0/besser/bot/nlp/intent_classifier/intent_classifier_configuration.py`

 * *Files identical despite different names*

### Comparing `besser_bot_framework-1.1.0/besser/bot/nlp/intent_classifier/intent_classifier_prediction.py` & `besser_bot_framework-1.2.0/besser/bot/nlp/intent_classifier/intent_classifier_prediction.py`

 * *Files identical despite different names*

### Comparing `besser_bot_framework-1.1.0/besser/bot/nlp/intent_classifier/llm_intent_classifier.py` & `besser_bot_framework-1.2.0/besser/bot/nlp/intent_classifier/llm_intent_classifier.py`

 * *Files identical despite different names*

### Comparing `besser_bot_framework-1.1.0/besser/bot/nlp/intent_classifier/simple_intent_classifier.py` & `besser_bot_framework-1.2.0/besser/bot/nlp/intent_classifier/simple_intent_classifier.py`

 * *Files identical despite different names*

### Comparing `besser_bot_framework-1.1.0/besser/bot/nlp/ner/base/datetime.py` & `besser_bot_framework-1.2.0/besser/bot/nlp/ner/base/datetime.py`

 * *Files identical despite different names*

### Comparing `besser_bot_framework-1.1.0/besser/bot/nlp/ner/base/number.py` & `besser_bot_framework-1.2.0/besser/bot/nlp/ner/base/number.py`

 * *Files identical despite different names*

### Comparing `besser_bot_framework-1.1.0/besser/bot/nlp/ner/matched_parameter.py` & `besser_bot_framework-1.2.0/besser/bot/nlp/ner/matched_parameter.py`

 * *Files identical despite different names*

### Comparing `besser_bot_framework-1.1.0/besser/bot/nlp/ner/ner.py` & `besser_bot_framework-1.2.0/besser/bot/nlp/ner/ner.py`

 * *Files identical despite different names*

### Comparing `besser_bot_framework-1.1.0/besser/bot/nlp/ner/ner_prediction.py` & `besser_bot_framework-1.2.0/besser/bot/nlp/ner/ner_prediction.py`

 * *Files identical despite different names*

### Comparing `besser_bot_framework-1.1.0/besser/bot/nlp/ner/simple_ner.py` & `besser_bot_framework-1.2.0/besser/bot/nlp/ner/simple_ner.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     a tuple with: 1 - the intent parameters where `v` could be a match and 2 - the main value of `v` (if `v` is not a
     synonym and it is the main value, it will be duplicated):
 
     {value/synonym: ([intent_parameters], value)}
 
     Args:
         intent (Intent): the target intent
-        processed_values (bool): weather to retrieve the entities processed values or not
+        processed_values (bool): whether to retrieve the entities processed values or not
 
     Returns:
         dict[str, tuple[list[IntentParameter], str]]: the dictionary
     """
     all_entity_values: dict[str, tuple[list[IntentParameter], str]] = {}
     intent_parameters_dict: dict[Entity, list[IntentParameter]] = {}
     for intent_parameter in intent.parameters:
```

### Comparing `besser_bot_framework-1.1.0/besser/bot/nlp/nlp_engine.py` & `besser_bot_framework-1.2.0/besser/bot/nlp/nlp_engine.py`

 * *Files identical despite different names*

### Comparing `besser_bot_framework-1.1.0/besser/bot/nlp/preprocessing/pipelines.py` & `besser_bot_framework-1.2.0/besser/bot/nlp/preprocessing/pipelines.py`

 * *Files identical despite different names*

### Comparing `besser_bot_framework-1.1.0/besser/bot/nlp/preprocessing/text_preprocessing.py` & `besser_bot_framework-1.2.0/besser/bot/nlp/preprocessing/text_preprocessing.py`

 * *Files identical despite different names*

### Comparing `besser_bot_framework-1.1.0/besser/bot/nlp/speech2text/api_speech2text.py` & `besser_bot_framework-1.2.0/besser/bot/nlp/speech2text/api_speech2text.py`

 * *Files identical despite different names*

### Comparing `besser_bot_framework-1.1.0/besser/bot/nlp/speech2text/hf_speech2text.py` & `besser_bot_framework-1.2.0/besser/bot/nlp/speech2text/hf_speech2text.py`

 * *Files identical despite different names*

### Comparing `besser_bot_framework-1.1.0/besser/bot/nlp/speech2text/speech2text.py` & `besser_bot_framework-1.2.0/besser/bot/nlp/speech2text/speech2text.py`

 * *Files identical despite different names*

### Comparing `besser_bot_framework-1.1.0/besser/bot/nlp/utils.py` & `besser_bot_framework-1.2.0/besser/bot/nlp/utils.py`

 * *Files identical despite different names*

### Comparing `besser_bot_framework-1.1.0/besser/bot/platforms/payload.py` & `besser_bot_framework-1.2.0/besser/bot/platforms/payload.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,41 +42,46 @@
     """
 
     BOT_REPLY_OPTIONS = 'bot_reply_options'
     """PayloadAction: Indicates that the payload's purpose is to send a bot reply containing a list of strings, where 
     the user should select 1 of them.
     """
 
+    BOT_REPLY_LOCATION = 'bot_reply_location'
+    """PayloadAction: Indicates that the payload's purpose is to send a bot reply containing a location, which is a
+    dictionary composed by a latitude and a longitude.
+    """
+
 
 class Payload:
     """Represents a payload object used for encoding and decoding messages between a bot and any other external agent.
     """
 
     @staticmethod
     def decode(payload_str):
         """Decode a JSON payload string into a :class:`Payload` object.
 
         Args:
-            payload_str (str): A JSON-encoded payload string.
+            payload_str (str or dict): A JSON-encoded payload string.
 
         Returns:
             Payload or None: A Payload object if the decoding is successful,
             None otherwise.
         """
         payload_dict = json.loads(payload_str)
         payload_action = payload_dict['action']
         payload_message = payload_dict['message']
         for action in PayloadAction:
             if action.value == payload_action:
                 return Payload(action, payload_message)
         return None
 
-    def __init__(self, action: PayloadAction, message: str = None):
+    def __init__(self, action: PayloadAction, message: str or dict = None):
         self.action: str = action.value
-        self.message: str = message
+        self.message: str or dict = message
 
 
 class PayloadEncoder(json.JSONEncoder):
     """Encoder for the :class:`Payload` class.
 
     Example:
         .. code::
```

### Comparing `besser_bot_framework-1.1.0/besser/bot/platforms/platform.py` & `besser_bot_framework-1.2.0/besser/bot/platforms/platform.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
     A platform defines the methods the bot can use to interact with a particular communication channel
     (e.g. Telegram, Slack...) for instance, sending and receiving messages.
 
     This class serves as a template to implement platforms.
 
      Attributes:
-        running (bool): Weather the platform is running or not
+        running (bool): Whether the platform is running or not
     """
 
     def __init__(self):
         self.running = False
 
     def run(self) -> None:
         """Run the platform."""
```

### Comparing `besser_bot_framework-1.1.0/besser/bot/platforms/telegram/telegram_platform.py` & `besser_bot_framework-1.2.0/besser/bot/platforms/telegram/telegram_platform.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import asyncio
 import base64
 import logging
+import threading
+from concurrent.futures import Future
 from typing import TYPE_CHECKING
 
 from telegram import Update
 from telegram.ext import Application, ApplicationBuilder, BaseHandler, CommandHandler, ContextTypes, MessageHandler, \
     filters
 
 from besser.bot.core.session import Session
@@ -14,19 +16,32 @@
 from besser.bot.platforms.payload import Payload, PayloadAction
 from besser.bot.platforms.platform import Platform
 
 if TYPE_CHECKING:
     from besser.bot.core.bot import Bot
 
 
+def _wait_future(future: Future):
+    """
+    Wait for a future (an asynchronous coroutine) to be finished.
+
+    Args:
+        future (Future): the Future to wait for
+    """
+    event = threading.Event()
+    future.add_done_callback((lambda ft: event.set()))
+    event.wait()
+
+
 class TelegramPlatform(Platform):
     """The Telegram Platform allows a bot to interact via Telegram.
 
-    It includes a `message handler` to handle all text inputs except commands (i.e. messages starting with '/')
-    and a `reset handler`, triggered by the `/reset` command, to reset the bot session.
+    It includes a `message handler` to handle all text inputs except commands (i.e. messages starting with '/'),
+    `voice`, `file` and `image` handlers and a `reset handler`, triggered by the `/reset` command, to reset the bot
+    session.
 
     Args:
         bot (Bot): the bot the platform belongs to
 
     Attributes:
         _bot (Bot): The bot the platform belongs to
         _telegram_app (Application): The Telegram Application
@@ -39,78 +54,101 @@
         self._telegram_app: Application = None
         self._event_loop: asyncio.AbstractEventLoop = None
         self._handlers: list[BaseHandler] = []
 
         # Handler for text messages
         async def message(update: Update, context: ContextTypes.DEFAULT_TYPE):
             session_id = str(update.effective_chat.id)
-            session = self._bot.get_or_create_session(session_id, self)
+            session = await asyncio.to_thread(self._bot.get_or_create_session, session_id, self)
             text = update.message.text
-            self._bot.receive_message(session.id, text)
+            await asyncio.to_thread(self._bot.receive_message, session.id, text)
 
-        message_handler = MessageHandler(filters.TEXT & (~filters.COMMAND), message)
+        message_handler = MessageHandler(filters.TEXT & (~filters.COMMAND), message, block=False)
         self._handlers.append(message_handler)
 
         # Handler for reset command
         async def reset(update: Update, context: ContextTypes.DEFAULT_TYPE):
             session_id = str(update.effective_chat.id)
-            self._bot.reset(session_id)
+            await asyncio.to_thread(self._bot.reset, session_id)
 
-        reset_handler = CommandHandler('reset', reset)
+        reset_handler = CommandHandler('reset', reset, block=False)
         self._handlers.append(reset_handler)
 
         # Handler for voice messages
         async def voice(update: Update, context: ContextTypes.DEFAULT_TYPE):
             session_id = str(update.effective_chat.id)
-            session = self._bot.get_or_create_session(session_id, self)
+            session = await asyncio.to_thread(self._bot.get_or_create_session, session_id, self)
             voice_file = await context.bot.get_file(update.message.voice.file_id)
             voice_data = await voice_file.download_as_bytearray()
             text = self._bot.nlp_engine.speech2text(bytes(voice_data))
-            self._bot.receive_message(session.id, text)
+            await asyncio.to_thread(self._bot.receive_message, session.id, text)
 
-        voice_handler = MessageHandler(filters.VOICE, voice)
+        voice_handler = MessageHandler(filters.VOICE, voice, block=False)
         self._handlers.append(voice_handler)
 
         # Handler for file messages
         async def file(update: Update, context: ContextTypes.DEFAULT_TYPE):
             session_id = str(update.effective_chat.id)
-            session = self._bot.get_or_create_session(session_id, self)
+            session = await asyncio.to_thread(self._bot.get_or_create_session, session_id, self)
             file_object = await context.bot.get_file(update.message.document.file_id)
             file_data = await file_object.download_as_bytearray()
             base64_data = base64.b64encode(file_data).decode()
-            file = File(file_name=update.message.document.file_name, file_type=update.message.document.mime_type, 
-                        file_base64=base64_data)
-            self._bot.receive_file(session.id, file=file)
+            f = File(
+                file_name=update.message.document.file_name, file_type=update.message.document.mime_type,
+                file_base64=base64_data
+            )
+            await asyncio.to_thread(self._bot.receive_file, session.id, file=f)
 
-        file_handler = MessageHandler(filters.ATTACHMENT & (~filters.PHOTO), file)
+        file_handler = MessageHandler(filters.ATTACHMENT & (~filters.PHOTO), file, block=False)
         self._handlers.append(file_handler)
 
         # Handler for image messages
         async def image(update: Update, context: ContextTypes.DEFAULT_TYPE):
             session_id = str(update.effective_chat.id)
-            session = self._bot.get_or_create_session(session_id, self)
+            session = await asyncio.to_thread(self._bot.get_or_create_session, session_id, self)
             image_object = await context.bot.get_file(update.message.photo[-1].file_id)
             image_data = await image_object.download_as_bytearray()
             base64_data = base64.b64encode(image_data).decode()
-            file = File(file_name=update.message.photo[-1].file_id + ".jpg", file_type="image/jpeg", 
-                        file_base64=base64_data)
-            self._bot.receive_file(session.id, file=file)
+            f = File(
+                file_name=update.message.photo[-1].file_id + ".jpg", file_type="image/jpeg",
+                file_base64=base64_data
+            )
+            await asyncio.to_thread(self._bot.receive_file, session.id, file=f)
 
-        image_handler = MessageHandler(filters.PHOTO, image)
+        image_handler = MessageHandler(filters.PHOTO, image, block=False)
         self._handlers.append(image_handler)
 
+    def __getattr__(self, name: str):
+        """All methods in :class:`telegram.ext._extbot.ExtBot` (that extends :class:`telegram._bot.Bot`) can be used
+        from the TelegramPlatform.
+
+        Args:
+            name (str): the name of the function to call
+        """
+        def method_proxy(*args, **kwargs):
+            # Forward the method call to the (telegram) bot
+            method = getattr(self._telegram_app.bot, name, None)
+            if method:
+                future = asyncio.run_coroutine_threadsafe(method(*args, **kwargs), self._event_loop)
+                _wait_future(future)
+                return future.result()
+            else:
+                raise AttributeError(f"'{self._telegram_app.bot.__class__}' object has no attribute '{name}'")
+        return method_proxy
+
     @property
     def telegram_app(self):
         """telegram.ext._application.Application: The Telegram app."""
         return self._telegram_app
 
-    def initialize(self) -> None: # Hide Info logging messages
+    def initialize(self) -> None:
+        # Hide Info logging messages
         logging.getLogger("httpx").setLevel(logging.WARNING)
         self._telegram_app = ApplicationBuilder().token(
-            self._bot.get_property(telegram.TELEGRAM_TOKEN)).build()
+            self._bot.get_property(telegram.TELEGRAM_TOKEN)).concurrent_updates(True).build()
         self._telegram_app.add_handlers(self._handlers)
         self._event_loop = asyncio.new_event_loop()
         asyncio.set_event_loop(self._event_loop)
 
     def start(self) -> None:
         logging.info(f'{self._bot.name}\'s TelegramPlatform starting')
         self.running = True
@@ -118,26 +156,54 @@
 
     def stop(self):
         self._event_loop.stop()
         self.running = False
         logging.info(f'{self._bot.name}\'s TelegramPlatform stopped')
 
     def _send(self, session_id: str, payload: Payload) -> None:
-        loop = asyncio.get_event_loop()
         if payload.action == PayloadAction.BOT_REPLY_STR.value:
-            asyncio.run_coroutine_threadsafe(self._telegram_app.bot.send_message(chat_id=session_id,
-                                                                                 text=payload.message), loop)
+            future = asyncio.run_coroutine_threadsafe(
+                self._telegram_app.bot.send_message(
+                    chat_id=session_id,
+                    text=payload.message
+                ),
+                self._event_loop
+            )
         elif payload.action == PayloadAction.BOT_REPLY_FILE.value:
-            asyncio.run_coroutine_threadsafe(self._telegram_app.bot.send_document(
-                chat_id=session_id, document=base64.b64decode(payload.message["base64"]),
-                filename=payload.message["name"], caption=payload.message["caption"]), loop)
+            future = asyncio.run_coroutine_threadsafe(
+                self._telegram_app.bot.send_document(
+                    chat_id=session_id,
+                    document=base64.b64decode(payload.message["base64"]),
+                    filename=payload.message["name"],
+                    caption=payload.message["caption"]
+                ),
+                self._event_loop
+            )
         elif payload.action == PayloadAction.BOT_REPLY_IMAGE.value:
-            asyncio.run_coroutine_threadsafe(self._telegram_app.bot.send_photo(
-                chat_id=session_id, photo=base64.b64decode(payload.message["base64"]),
-                caption=payload.message["caption"]), loop)
+            future = asyncio.run_coroutine_threadsafe(
+                self._telegram_app.bot.send_photo(
+                    chat_id=session_id,
+                    photo=base64.b64decode(payload.message["base64"]),
+                    caption=payload.message["caption"]
+                ),
+                self._event_loop
+            )
+        elif payload.action == PayloadAction.BOT_REPLY_LOCATION.value:
+            future = asyncio.run_coroutine_threadsafe(
+                self._telegram_app.bot.send_location(
+                    chat_id=session_id,
+                    latitude=payload.message['latitude'],
+                    longitude=payload.message['longitude'],
+                ),
+                self._event_loop
+            )
+        else:
+            future = None
+        if future is not None:
+            _wait_future(future)
 
     def reply(self, session: Session, message: str) -> None:
         if session.platform is not self:
             raise PlatformMismatchError(self, session)
         session.chat_history.append((message, 0))
         payload = Payload(action=PayloadAction.BOT_REPLY_STR,
                           message=message)
@@ -179,14 +245,30 @@
             file_dict["caption"] = message
         else:
             file_dict["caption"] = ""
         payload = Payload(action=PayloadAction.BOT_REPLY_IMAGE,
                           message=file_dict)
         self._send(session.id, payload)
 
+    def reply_location(self, session: Session, latitude: float, longitude: float) -> None:
+        """Send a location reply to a specific user.
+
+        Args:
+            session (Session): the user session
+            latitude (str): the latitude of the location
+            longitude (str): the longitude of the location
+        """
+        if session.platform is not self:
+            raise PlatformMismatchError(self, session)
+        location_dict = {'latitude': latitude, 'longitude': longitude}
+        session.chat_history.append((str(location_dict), 0))
+        payload = Payload(action=PayloadAction.BOT_REPLY_LOCATION,
+                          message=location_dict)
+        self._send(session.id, payload)
+
     def add_handler(self, handler: BaseHandler) -> None:
         """
         Add a custom Telegram handler for the bot.
 
         Args:
             handler (telegram.ext.BaseHandler): the handler to add
         """
```

### Comparing `besser_bot_framework-1.1.0/besser/bot/platforms/websocket/__init__.py` & `besser_bot_framework-1.2.0/besser/bot/platforms/websocket/__init__.py`

 * *Files identical despite different names*

### Comparing `besser_bot_framework-1.1.0/besser/bot/platforms/websocket/message.py` & `besser_bot_framework-1.2.0/besser/bot/platforms/websocket/message.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,19 +2,19 @@
     """
     A conversation message. It is used by the streamlit UI to display the messages properly, depending on the sender
     (i.e., user or chatbot) and the type (string, audio, file, DataFrame, plot, etc.)
 
     Args:
         t (str): The type of the message
         content (Any): The message content
-        is_user (bool): Weather the message comes from the user (true) or the chatbot (false)
+        is_user (bool): Whether the message comes from the user (true) or the chatbot (false)
 
     Attributes:
         type (str): The type of the message
         content (Any): The message content
-        is_user (bool): Weather the message comes from the user (true) or the chatbot (false)
+        is_user (bool): Whether the message comes from the user (true) or the chatbot (false)
     """
 
     def __init__(self, t: str, content, is_user: bool):
         self.type: str = t
         self.content = content
         self.is_user: bool = is_user
```

### Comparing `besser_bot_framework-1.1.0/besser/bot/platforms/websocket/streamlit_ui.py` & `besser_bot_framework-1.2.0/besser/bot/platforms/websocket/streamlit_ui.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,15 +41,21 @@
         if not runtime.is_active_session(session.id):
             runtime.close_session(session.id)
             session.session_state['websocket'].close()
             break
 
 
 def main():
-    st.header("Chat Demo")
+    try:
+        # We get the websocket host and port from the script arguments
+        bot_name = sys.argv[1]
+    except Exception as e:
+        # If they are not provided, we use default values
+        bot_name = 'Chatbot Demo'
+    st.header(bot_name)
     st.markdown("[Github](https://github.com/BESSER-PEARL/BESSER-Bot-Framework)")
     # User input component. Must be declared before history writing
     user_input = st.chat_input("What is up?")
 
     def on_message(ws, payload_str):
         # https://github.com/streamlit/streamlit/issues/2838
         streamlit_session = get_streamlit_session()
@@ -62,14 +68,20 @@
             t = 'file'
         elif payload.action == PayloadAction.BOT_REPLY_DF.value:
             content = pd.read_json(payload.message)
             t = 'dataframe'
         elif payload.action == PayloadAction.BOT_REPLY_PLOTLY.value:
             content = plotly.io.from_json(payload.message)
             t = 'plotly'
+        elif payload.action == PayloadAction.BOT_REPLY_LOCATION.value:
+            content = {
+                'latitude': [payload.message['latitude']],
+                'longitude': [payload.message['longitude']]
+            }
+            t = 'location'
         elif payload.action == PayloadAction.BOT_REPLY_OPTIONS.value:
             t = 'options'
             d = json.loads(payload.message)
             content = []
             for button in d.values():
                 content.append(button)
         message = Message(t, content, is_user=False)
@@ -101,16 +113,16 @@
 
     if 'queue' not in st.session_state:
         st.session_state['queue'] = queue.Queue()
 
     if 'websocket' not in st.session_state:
         try:
             # We get the websocket host and port from the script arguments
-            host = sys.argv[1]
-            port = sys.argv[2]
+            host = sys.argv[2]
+            port = sys.argv[3]
         except Exception as e:
             # If they are not provided, we use default values
             host = 'localhost'
             port = '8765'
         ws = websocket.WebSocketApp(f"ws://{host}:{port}/",
                                     on_open=on_open,
                                     on_message=on_message,
@@ -171,14 +183,16 @@
             elif message.type == 'file':
                 file: File = File.from_dict(message.content)
                 file_name = file.name
                 file_type = file.type
                 file_data = base64.b64decode(file.base64.encode('utf-8'))
                 st.download_button(label='Download ' + file_name, file_name=file_name, data=file_data, mime=file_type,
                                    key=file_name + str(time.time()))
+            elif message.type == 'location':
+                st.map(message.content)
             else:
                 st.write(message.content)
 
     first_message = True
     while not st.session_state['queue'].empty():
         message = st.session_state['queue'].get()
         if hasattr(message, '__len__'):
@@ -199,14 +213,17 @@
                     time.sleep(t)
                 file: File = File.from_dict(message.content)
                 file_name = file.name
                 file_type = file.type
                 file_data = base64.b64decode(file.base64.encode('utf-8'))
                 st.download_button(label='Download ' + file_name, file_name=file_name, data=file_data, mime=file_type,
                                    key=file_name + str(time.time()))
+        elif message.type == 'location':
+            st.session_state['history'].append(message)
+            st.map(message.content)
         else:
             st.session_state['history'].append(message)
             with st.chat_message("assistant"):
                 with st.spinner(''):
                     time.sleep(t)
                 st.write(message.content)
```

### Comparing `besser_bot_framework-1.1.0/besser/bot/platforms/websocket/websocket_platform.py` & `besser_bot_framework-1.2.0/besser/bot/platforms/websocket/websocket_platform.py`

 * *Files 14% similar despite different names*

```diff
@@ -33,21 +33,21 @@
 
     Note:
         We provide a UI (:doc:`streamlit_ui`) implementing a WebSocket client to communicate with the bot, though you
         can use or create your own UI as long as it has a WebSocket client that connects to the bot's WebSocket server.
 
     Args:
         bot (Bot): the bot the platform belongs to
-        use_ui (bool): weather to use the built-in UI or not
+        use_ui (bool): whether to use the built-in UI or not
 
     Attributes:
         _bot (Bot): The bot the platform belongs to
         _host (str): The WebSocket host address (e.g. `localhost`)
         _port (int): The WebSocket port (e.g. `8765`)
-        _use_ui (bool): Weather to use the built-in UI or not
+        _use_ui (bool): Whether to use the built-in UI or not
         _connections (dict[str, ServerConnection]): The list of active connections (i.e. users connected to the bot)
         _websocket_server (WebSocketServer or None): The WebSocket server instance
         _message_handler (Callable[[ServerConnection], None]): The function that handles the user connections
             (sessions) and incoming messages
     """
 
     def __init__(self, bot: 'Bot', use_ui: bool = True):
@@ -108,35 +108,37 @@
             def run_streamlit() -> None:
                 """Run the Streamlit UI in a dedicated thread."""
                 subprocess.run([
                     "streamlit", "run",
                     "--server.address", self._bot.get_property(websocket.STREAMLIT_HOST),
                     "--server.port", str(self._bot.get_property(websocket.STREAMLIT_PORT)),
                     os.path.abspath(inspect.getfile(streamlit_ui)),
+                    self._bot.name,
                     self._bot.get_property(websocket.WEBSOCKET_HOST),
                     str(self._bot.get_property(websocket.WEBSOCKET_PORT))
                 ])
 
             thread = threading.Thread(target=run_streamlit)
             logging.info(f'Running Streamlit UI in another thread')
             thread.start()
-            #
+            # To avoid re-running the streamlit process, set self._use_ui to False
             self._use_ui = False
         logging.info(f'{self._bot.name}\'s WebSocketPlatform starting at ws://{self._host}:{self._port}')
         self.running = True
         self._websocket_server.serve_forever()
 
     def stop(self):
         self._websocket_server.shutdown()
         self.running = False
         logging.info(f'{self._bot.name}\'s WebSocketPlatform stopped')
 
     def _send(self, session_id, payload: Payload) -> None:
-        conn = self._connections[session_id]
-        conn.send(json.dumps(payload, cls=PayloadEncoder))
+        if session_id in self._connections:
+            conn = self._connections[session_id]
+            conn.send(json.dumps(payload, cls=PayloadEncoder))
 
     def reply(self, session: Session, message: str) -> None:
         if session.platform is not self:
             raise PlatformMismatchError(self, session)
         session.chat_history.append((message, 0))
         payload = Payload(action=PayloadAction.BOT_REPLY_STR,
                           message=message)
@@ -145,39 +147,45 @@
     def reply_file(self, session: Session, file: File) -> None:
         """Send a file reply to a specific user
 
         Args:
             session (Session): the user session
             file (File): the file to send
         """
+        if session.platform is not self:
+            raise PlatformMismatchError(self, session)
         session.chat_history.append((file.get_json_string(), 0))
         payload = Payload(action=PayloadAction.BOT_REPLY_FILE,
                           message=file.to_dict())
         self._send(session.id, payload)
 
     def reply_dataframe(self, session: Session, df: DataFrame) -> None:
         """Send a DataFrame bot reply, i.e. a table, to a specific user.
 
         Args:
             session (Session): the user session
             df (pandas.DataFrame): the message to send to the user
         """
+        if session.platform is not self:
+            raise PlatformMismatchError(self, session)
         message = df.to_json()
         session.chat_history.append((message, 0))
         payload = Payload(action=PayloadAction.BOT_REPLY_DF,
                           message=message)
         self._send(session.id, payload)
 
     def reply_options(self, session: Session, options: list[str]):
         """Send a list of options as a reply. They can be used to let the user choose one of them
 
         Args:
             session (Session): the user session
             options (list[str]): the list of options to send to the user
         """
+        if session.platform is not self:
+            raise PlatformMismatchError(self, session)
         d = {}
         for i, button in enumerate(options):
             d[i] = button
         message = json.dumps(d)
         session.chat_history.append((message, 0))
         payload = Payload(action=PayloadAction.BOT_REPLY_OPTIONS,
                           message=message)
@@ -186,12 +194,30 @@
     def reply_plotly(self, session: Session, plot: plotly.graph_objs.Figure) -> None:
         """Send a Plotly figure as a bot reply, to a specific user.
 
         Args:
             session (Session): the user session
             plot (plotly.graph_objs.Figure): the message to send to the user
         """
+        if session.platform is not self:
+            raise PlatformMismatchError(self, session)
         message = plotly.io.to_json(plot)
         session.chat_history.append((message, 0))
         payload = Payload(action=PayloadAction.BOT_REPLY_PLOTLY,
                           message=message)
         self._send(session.id, payload)
+
+    def reply_location(self, session: Session, latitude: float, longitude: float) -> None:
+        """Send a location reply to a specific user.
+
+        Args:
+            session (Session): the user session
+            latitude (str): the latitude of the location
+            longitude (str): the longitude of the location
+        """
+        if session.platform is not self:
+            raise PlatformMismatchError(self, session)
+        location_dict = {'latitude': latitude, 'longitude': longitude}
+        session.chat_history.append((str(location_dict), 0))
+        payload = Payload(action=PayloadAction.BOT_REPLY_LOCATION,
+                          message=location_dict)
+        self._send(session.id, payload)
```

### Comparing `besser_bot_framework-1.1.0/besser/bot/test/examples/greetings_bot.py` & `besser_bot_framework-1.2.0/besser/bot/test/examples/greetings_bot.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 ])
 
 good_intent = bot.new_intent('good_intent', [
     'good',
     'fine',
 ])
 
-bad_intent= bot.new_intent('bad_intent', [
+bad_intent = bot.new_intent('bad_intent', [
     'bad',
     'awful',
 ])
 
 
 # STATES BODIES' DEFINITION + TRANSITIONS
```

### Comparing `besser_bot_framework-1.1.0/besser/bot/test/examples/telegram_bot.py` & `besser_bot_framework-1.2.0/besser/bot/test/examples/telegram_bot.py`

 * *Files identical despite different names*

### Comparing `besser_bot_framework-1.1.0/besser/bot/test/examples/weather_bot.py` & `besser_bot_framework-1.2.0/besser/bot/test/examples/weather_bot.py`

 * *Files identical despite different names*

### Comparing `besser_bot_framework-1.1.0/besser_bot_framework.egg-info/PKG-INFO` & `besser_bot_framework-1.2.0/besser_bot_framework.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: besser-bot-framework
-Version: 1.1.0
+Version: 1.2.0
 Summary: BESSER Bot Framework (BBF)
 Author: Luxembourg Institute of Science and Technology
 License: MIT
 Project-URL: Documentation, https://besserbot-framework.readthedocs.io/
 Project-URL: Source Code, https://github.com/BESSER-PEARL/BESSER-Bot-Framework
 Project-URL: Bug Tracker, https://github.com/BESSER-PEARL/BESSER-Bot-Framework/issues
 Keywords: bot,framework,chatbot,state-machine,nlp
@@ -16,20 +16,22 @@
 Requires-Dist: keras==2.14.0
 Requires-Dist: librosa==0.10.1
 Requires-Dist: nltk==3.8.1
 Requires-Dist: numpy==1.26.1
 Requires-Dist: openai==1.8.0
 Requires-Dist: pandas==2.1.1
 Requires-Dist: plotly==5.18.0
+Requires-Dist: psycopg2-binary==2.9.9
 Requires-Dist: python-telegram-bot==20.6
 Requires-Dist: replicate==0.23.1
 Requires-Dist: requests==2.31.0
 Requires-Dist: snowballstemmer==2.2.0
 Requires-Dist: spacy==3.7.2
 Requires-Dist: SpeechRecognition==3.10.0
+Requires-Dist: sqlalchemy==2.0.29
 Requires-Dist: streamlit==1.27.2
 Requires-Dist: tensorflow==2.14.0
 Requires-Dist: text2num==2.5.0
 Requires-Dist: transformers==4.37.0
 Requires-Dist: websocket-client==1.6.4
 Requires-Dist: websockets==11.0.3
```

### Comparing `besser_bot_framework-1.1.0/besser_bot_framework.egg-info/SOURCES.txt` & `besser_bot_framework-1.2.0/besser_bot_framework.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 besser/bot/core/transition.py
 besser/bot/core/entity/__init__.py
 besser/bot/core/entity/entity.py
 besser/bot/core/entity/entity_entry.py
 besser/bot/core/intent/__init__.py
 besser/bot/core/intent/intent.py
 besser/bot/core/intent/intent_parameter.py
+besser/bot/db/__init__.py
+besser/bot/db/monitoring_db.py
 besser/bot/exceptions/__init__.py
 besser/bot/exceptions/exceptions.py
 besser/bot/library/__init__.py
 besser/bot/library/entity/__init__.py
 besser/bot/library/entity/base_entities.py
 besser/bot/library/event/__init__.py
 besser/bot/library/event/event_library.py
```

### Comparing `besser_bot_framework-1.1.0/setup.cfg` & `besser_bot_framework-1.2.0/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2062 6573 7365 722d 626f 742d 6672   = besser-bot-fr
 00000020: 616d 6577 6f72 6b0d 0a76 6572 7369 6f6e  amework..version
-00000030: 203d 2031 2e31 2e30 0d0a 6175 7468 6f72   = 1.1.0..author
+00000030: 203d 2031 2e32 2e30 0d0a 6175 7468 6f72   = 1.2.0..author
 00000040: 203d 204c 7578 656d 626f 7572 6720 496e   = Luxembourg In
 00000050: 7374 6974 7574 6520 6f66 2053 6369 656e  stitute of Scien
 00000060: 6365 2061 6e64 2054 6563 686e 6f6c 6f67  ce and Technolog
 00000070: 790d 0a64 6573 6372 6970 7469 6f6e 203d  y..description =
 00000080: 2042 4553 5345 5220 426f 7420 4672 616d   BESSER Bot Fram
 00000090: 6577 6f72 6b20 2842 4246 290d 0a6c 6f6e  ework (BBF)..lon
 000000a0: 675f 6465 7363 7269 7074 696f 6e20 3d20  g_description =
```

