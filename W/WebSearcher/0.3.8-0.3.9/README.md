# Comparing `tmp/WebSearcher-0.3.8.tar.gz` & `tmp/WebSearcher-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "WebSearcher-0.3.8.tar", last modified: Tue Feb 13 09:53:47 2024, max compression
+gzip compressed data, was "WebSearcher-0.3.9.tar", last modified: Mon Feb 26 03:35:46 2024, max compression
```

## Comparing `WebSearcher-0.3.8.tar` & `WebSearcher-0.3.9.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:53:47.562722 WebSearcher-0.3.8/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-02-13 09:53:29.000000 WebSearcher-0.3.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-02-13 09:53:29.000000 WebSearcher-0.3.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-02-13 09:53:47.562722 WebSearcher-0.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12321 2024-02-13 09:53:29.000000 WebSearcher-0.3.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:53:47.554722 WebSearcher-0.3.8/WebSearcher/
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-02-13 09:53:29.000000 WebSearcher-0.3.8/WebSearcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10710 2024-02-13 09:53:29.000000 WebSearcher-0.3.8/WebSearcher/component_classifier.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:53:47.562722 WebSearcher-0.3.8/WebSearcher/component_parsers/
--rw-r--r--   0 runner    (1001) docker     (127)     3008 2024-02-13 09:53:29.000000 WebSearcher-0.3.8/WebSearcher/component_parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3565 2024-02-13 09:53:29.000000 WebSearcher-0.3.8/WebSearcher/component_parsers/ads.py
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-02-13 09:53:29.000000 WebSearcher-0.3.8/WebSearcher/component_parsers/available_on.py
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-02-13 09:53:29.000000 WebSearcher-0.3.8/WebSearcher/component_parsers/banner.py
--rw-r--r--   0 runner    (1001) docker     (127)     5004 2024-02-13 09:53:29.000000 WebSearcher-0.3.8/WebSearcher/component_parsers/footer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7547 2024-02-13 09:53:29.000000 WebSearcher-0.3.8/WebSearcher/component_parsers/general.py
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-02-13 09:53:29.000000 WebSearcher-0.3.8/WebSearcher/component_parsers/general_questions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-02-13 09:53:29.000000 WebSearcher-0.3.8/WebSearcher/component_parsers/images.py
--rw-r--r--   0 runner    (1001) docker     (127)     3482 2024-02-13 09:53:29.000000 WebSearcher-0.3.8/WebSearcher/component_parsers/knowledge.py
--rw-r--r--   0 runner    (1001) docker     (127)     3425 2024-02-13 09:53:29.000000 WebSearcher-0.3.8/WebSearcher/component_parsers/knowledge_rhs.py
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-02-13 09:53:29.000000 WebSearcher-0.3.8/WebSearcher/component_parsers/latest_from.py
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-02-13 09:53:29.000000 WebSearcher-0.3.8/WebSearcher/component_parsers/local_news.py
--rw-r--r--   0 runner    (1001) docker     (127)     2518 2024-02-13 09:53:29.000000 WebSearcher-0.3.8/WebSearcher/component_parsers/local_results.py
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-02-13 09:53:29.000000 WebSearcher-0.3.8/WebSearcher/component_parsers/map_results.py
--rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-02-13 09:53:29.000000 WebSearcher-0.3.8/WebSearcher/component_parsers/news_quotes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-02-13 09:53:29.000000 WebSearcher-0.3.8/WebSearcher/component_parsers/people_also_ask.py
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-02-13 09:53:29.000000 WebSearcher-0.3.8/WebSearcher/component_parsers/perspectives.py
--rw-r--r--   0 runner    (1001) docker     (127)      980 2024-02-13 09:53:29.000000 WebSearcher-0.3.8/WebSearcher/component_parsers/scholarly_articles.py
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-02-13 09:53:29.000000 WebSearcher-0.3.8/WebSearcher/component_parsers/searches_related.py
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-02-13 09:53:29.000000 WebSearcher-0.3.8/WebSearcher/component_parsers/shopping_ads.py
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-02-13 09:53:29.000000 WebSearcher-0.3.8/WebSearcher/component_parsers/top_image_carousel.py
--rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-02-13 09:53:29.000000 WebSearcher-0.3.8/WebSearcher/component_parsers/top_stories.py
--rw-r--r--   0 runner    (1001) docker     (127)     3407 2024-02-13 09:53:29.000000 WebSearcher-0.3.8/WebSearcher/component_parsers/twitter_cards.py
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-02-13 09:53:29.000000 WebSearcher-0.3.8/WebSearcher/component_parsers/twitter_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     3405 2024-02-13 09:53:29.000000 WebSearcher-0.3.8/WebSearcher/component_parsers/videos.py
--rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-02-13 09:53:29.000000 WebSearcher-0.3.8/WebSearcher/component_parsers/view_more_news.py
--rw-r--r--   0 runner    (1001) docker     (127)     6023 2024-02-13 09:53:29.000000 WebSearcher-0.3.8/WebSearcher/extractors.py
--rw-r--r--   0 runner    (1001) docker     (127)     3978 2024-02-13 09:53:29.000000 WebSearcher-0.3.8/WebSearcher/locations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3722 2024-02-13 09:53:29.000000 WebSearcher-0.3.8/WebSearcher/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)      985 2024-02-13 09:53:29.000000 WebSearcher-0.3.8/WebSearcher/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     3917 2024-02-13 09:53:29.000000 WebSearcher-0.3.8/WebSearcher/parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3618 2024-02-13 09:53:29.000000 WebSearcher-0.3.8/WebSearcher/result_collector.py
--rw-r--r--   0 runner    (1001) docker     (127)     8400 2024-02-13 09:53:29.000000 WebSearcher-0.3.8/WebSearcher/searchers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-02-13 09:53:29.000000 WebSearcher-0.3.8/WebSearcher/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7038 2024-02-13 09:53:29.000000 WebSearcher-0.3.8/WebSearcher/webutils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:53:47.558722 WebSearcher-0.3.8/WebSearcher.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-02-13 09:53:47.000000 WebSearcher-0.3.8/WebSearcher.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-02-13 09:53:47.000000 WebSearcher-0.3.8/WebSearcher.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-13 09:53:47.000000 WebSearcher-0.3.8/WebSearcher.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-02-13 09:53:47.000000 WebSearcher-0.3.8/WebSearcher.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-02-13 09:53:47.000000 WebSearcher-0.3.8/WebSearcher.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-13 09:53:47.562722 WebSearcher-0.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-02-13 09:53:29.000000 WebSearcher-0.3.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 03:35:46.266890 WebSearcher-0.3.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-02-26 03:35:28.000000 WebSearcher-0.3.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-02-26 03:35:28.000000 WebSearcher-0.3.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-02-26 03:35:46.266890 WebSearcher-0.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12321 2024-02-26 03:35:28.000000 WebSearcher-0.3.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 03:35:46.262890 WebSearcher-0.3.9/WebSearcher/
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-02-26 03:35:28.000000 WebSearcher-0.3.9/WebSearcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10710 2024-02-26 03:35:28.000000 WebSearcher-0.3.9/WebSearcher/component_classifier.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 03:35:46.266890 WebSearcher-0.3.9/WebSearcher/component_parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)     3008 2024-02-26 03:35:28.000000 WebSearcher-0.3.9/WebSearcher/component_parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3565 2024-02-26 03:35:28.000000 WebSearcher-0.3.9/WebSearcher/component_parsers/ads.py
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-02-26 03:35:28.000000 WebSearcher-0.3.9/WebSearcher/component_parsers/available_on.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-02-26 03:35:28.000000 WebSearcher-0.3.9/WebSearcher/component_parsers/banner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5004 2024-02-26 03:35:28.000000 WebSearcher-0.3.9/WebSearcher/component_parsers/footer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7547 2024-02-26 03:35:28.000000 WebSearcher-0.3.9/WebSearcher/component_parsers/general.py
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-02-26 03:35:28.000000 WebSearcher-0.3.9/WebSearcher/component_parsers/general_questions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-02-26 03:35:28.000000 WebSearcher-0.3.9/WebSearcher/component_parsers/images.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3482 2024-02-26 03:35:28.000000 WebSearcher-0.3.9/WebSearcher/component_parsers/knowledge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3425 2024-02-26 03:35:28.000000 WebSearcher-0.3.9/WebSearcher/component_parsers/knowledge_rhs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-02-26 03:35:28.000000 WebSearcher-0.3.9/WebSearcher/component_parsers/latest_from.py
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-02-26 03:35:28.000000 WebSearcher-0.3.9/WebSearcher/component_parsers/local_news.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2518 2024-02-26 03:35:28.000000 WebSearcher-0.3.9/WebSearcher/component_parsers/local_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-02-26 03:35:28.000000 WebSearcher-0.3.9/WebSearcher/component_parsers/map_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-02-26 03:35:28.000000 WebSearcher-0.3.9/WebSearcher/component_parsers/news_quotes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-02-26 03:35:28.000000 WebSearcher-0.3.9/WebSearcher/component_parsers/people_also_ask.py
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-02-26 03:35:28.000000 WebSearcher-0.3.9/WebSearcher/component_parsers/perspectives.py
+-rw-r--r--   0 runner    (1001) docker     (127)      980 2024-02-26 03:35:28.000000 WebSearcher-0.3.9/WebSearcher/component_parsers/scholarly_articles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-02-26 03:35:28.000000 WebSearcher-0.3.9/WebSearcher/component_parsers/searches_related.py
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-02-26 03:35:28.000000 WebSearcher-0.3.9/WebSearcher/component_parsers/shopping_ads.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-02-26 03:35:28.000000 WebSearcher-0.3.9/WebSearcher/component_parsers/top_image_carousel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-02-26 03:35:28.000000 WebSearcher-0.3.9/WebSearcher/component_parsers/top_stories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3407 2024-02-26 03:35:28.000000 WebSearcher-0.3.9/WebSearcher/component_parsers/twitter_cards.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-02-26 03:35:28.000000 WebSearcher-0.3.9/WebSearcher/component_parsers/twitter_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3488 2024-02-26 03:35:28.000000 WebSearcher-0.3.9/WebSearcher/component_parsers/videos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-02-26 03:35:28.000000 WebSearcher-0.3.9/WebSearcher/component_parsers/view_more_news.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6023 2024-02-26 03:35:28.000000 WebSearcher-0.3.9/WebSearcher/extractors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3978 2024-02-26 03:35:28.000000 WebSearcher-0.3.9/WebSearcher/locations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3722 2024-02-26 03:35:28.000000 WebSearcher-0.3.9/WebSearcher/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-02-26 03:35:28.000000 WebSearcher-0.3.9/WebSearcher/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3917 2024-02-26 03:35:28.000000 WebSearcher-0.3.9/WebSearcher/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3618 2024-02-26 03:35:28.000000 WebSearcher-0.3.9/WebSearcher/result_collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8400 2024-02-26 03:35:28.000000 WebSearcher-0.3.9/WebSearcher/searchers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-02-26 03:35:28.000000 WebSearcher-0.3.9/WebSearcher/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7038 2024-02-26 03:35:28.000000 WebSearcher-0.3.9/WebSearcher/webutils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 03:35:46.266890 WebSearcher-0.3.9/WebSearcher.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-02-26 03:35:46.000000 WebSearcher-0.3.9/WebSearcher.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-02-26 03:35:46.000000 WebSearcher-0.3.9/WebSearcher.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-26 03:35:46.000000 WebSearcher-0.3.9/WebSearcher.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-02-26 03:35:46.000000 WebSearcher-0.3.9/WebSearcher.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-02-26 03:35:46.000000 WebSearcher-0.3.9/WebSearcher.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-26 03:35:46.266890 WebSearcher-0.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-02-26 03:35:28.000000 WebSearcher-0.3.9/setup.py
```

### Comparing `WebSearcher-0.3.8/LICENSE` & `WebSearcher-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `WebSearcher-0.3.8/PKG-INFO` & `WebSearcher-0.3.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WebSearcher
-Version: 0.3.8
+Version: 0.3.9
 Summary: WebSearcher
 Home-page: http://github.com/gitronald/WebSearcher
 Author: Ronald E. Robertson
 Author-email: rer@acm.org
 License: BSD-3-Clause
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `WebSearcher-0.3.8/README.md` & `WebSearcher-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `WebSearcher-0.3.8/WebSearcher/component_classifier.py` & `WebSearcher-0.3.9/WebSearcher/component_classifier.py`

 * *Files identical despite different names*

### Comparing `WebSearcher-0.3.8/WebSearcher/component_parsers/__init__.py` & `WebSearcher-0.3.9/WebSearcher/component_parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `WebSearcher-0.3.8/WebSearcher/component_parsers/ads.py` & `WebSearcher-0.3.9/WebSearcher/component_parsers/ads.py`

 * *Files identical despite different names*

### Comparing `WebSearcher-0.3.8/WebSearcher/component_parsers/available_on.py` & `WebSearcher-0.3.9/WebSearcher/component_parsers/available_on.py`

 * *Files identical despite different names*

### Comparing `WebSearcher-0.3.8/WebSearcher/component_parsers/banner.py` & `WebSearcher-0.3.9/WebSearcher/component_parsers/banner.py`

 * *Files identical despite different names*

### Comparing `WebSearcher-0.3.8/WebSearcher/component_parsers/footer.py` & `WebSearcher-0.3.9/WebSearcher/component_parsers/footer.py`

 * *Files identical despite different names*

### Comparing `WebSearcher-0.3.8/WebSearcher/component_parsers/general.py` & `WebSearcher-0.3.9/WebSearcher/component_parsers/general.py`

 * *Files identical despite different names*

### Comparing `WebSearcher-0.3.8/WebSearcher/component_parsers/general_questions.py` & `WebSearcher-0.3.9/WebSearcher/component_parsers/general_questions.py`

 * *Files identical despite different names*

### Comparing `WebSearcher-0.3.8/WebSearcher/component_parsers/images.py` & `WebSearcher-0.3.9/WebSearcher/component_parsers/images.py`

 * *Files identical despite different names*

### Comparing `WebSearcher-0.3.8/WebSearcher/component_parsers/knowledge.py` & `WebSearcher-0.3.9/WebSearcher/component_parsers/knowledge.py`

 * *Files identical despite different names*

### Comparing `WebSearcher-0.3.8/WebSearcher/component_parsers/knowledge_rhs.py` & `WebSearcher-0.3.9/WebSearcher/component_parsers/knowledge_rhs.py`

 * *Files identical despite different names*

### Comparing `WebSearcher-0.3.8/WebSearcher/component_parsers/local_results.py` & `WebSearcher-0.3.9/WebSearcher/component_parsers/local_results.py`

 * *Files identical despite different names*

### Comparing `WebSearcher-0.3.8/WebSearcher/component_parsers/map_results.py` & `WebSearcher-0.3.9/WebSearcher/component_parsers/map_results.py`

 * *Files identical despite different names*

### Comparing `WebSearcher-0.3.8/WebSearcher/component_parsers/news_quotes.py` & `WebSearcher-0.3.9/WebSearcher/component_parsers/news_quotes.py`

 * *Files identical despite different names*

### Comparing `WebSearcher-0.3.8/WebSearcher/component_parsers/people_also_ask.py` & `WebSearcher-0.3.9/WebSearcher/component_parsers/people_also_ask.py`

 * *Files identical despite different names*

### Comparing `WebSearcher-0.3.8/WebSearcher/component_parsers/scholarly_articles.py` & `WebSearcher-0.3.9/WebSearcher/component_parsers/scholarly_articles.py`

 * *Files identical despite different names*

### Comparing `WebSearcher-0.3.8/WebSearcher/component_parsers/searches_related.py` & `WebSearcher-0.3.9/WebSearcher/component_parsers/searches_related.py`

 * *Files identical despite different names*

### Comparing `WebSearcher-0.3.8/WebSearcher/component_parsers/shopping_ads.py` & `WebSearcher-0.3.9/WebSearcher/component_parsers/shopping_ads.py`

 * *Files identical despite different names*

### Comparing `WebSearcher-0.3.8/WebSearcher/component_parsers/top_image_carousel.py` & `WebSearcher-0.3.9/WebSearcher/component_parsers/top_image_carousel.py`

 * *Files identical despite different names*

### Comparing `WebSearcher-0.3.8/WebSearcher/component_parsers/top_stories.py` & `WebSearcher-0.3.9/WebSearcher/component_parsers/top_stories.py`

 * *Files identical despite different names*

### Comparing `WebSearcher-0.3.8/WebSearcher/component_parsers/twitter_cards.py` & `WebSearcher-0.3.9/WebSearcher/component_parsers/twitter_cards.py`

 * *Files identical despite different names*

### Comparing `WebSearcher-0.3.8/WebSearcher/component_parsers/twitter_result.py` & `WebSearcher-0.3.9/WebSearcher/component_parsers/twitter_result.py`

 * *Files identical despite different names*

### Comparing `WebSearcher-0.3.8/WebSearcher/component_parsers/view_more_news.py` & `WebSearcher-0.3.9/WebSearcher/component_parsers/view_more_news.py`

 * *Files identical despite different names*

### Comparing `WebSearcher-0.3.8/WebSearcher/extractors.py` & `WebSearcher-0.3.9/WebSearcher/extractors.py`

 * *Files identical despite different names*

### Comparing `WebSearcher-0.3.8/WebSearcher/locations.py` & `WebSearcher-0.3.9/WebSearcher/locations.py`

 * *Files identical despite different names*

### Comparing `WebSearcher-0.3.8/WebSearcher/logger.py` & `WebSearcher-0.3.9/WebSearcher/logger.py`

 * *Files identical despite different names*

### Comparing `WebSearcher-0.3.8/WebSearcher/models.py` & `WebSearcher-0.3.9/WebSearcher/models.py`

 * *Files identical despite different names*

### Comparing `WebSearcher-0.3.8/WebSearcher/parsers.py` & `WebSearcher-0.3.9/WebSearcher/parsers.py`

 * *Files identical despite different names*

### Comparing `WebSearcher-0.3.8/WebSearcher/result_collector.py` & `WebSearcher-0.3.9/WebSearcher/result_collector.py`

 * *Files identical despite different names*

### Comparing `WebSearcher-0.3.8/WebSearcher/searchers.py` & `WebSearcher-0.3.9/WebSearcher/searchers.py`

 * *Files identical despite different names*

### Comparing `WebSearcher-0.3.8/WebSearcher/utils.py` & `WebSearcher-0.3.9/WebSearcher/utils.py`

 * *Files identical despite different names*

### Comparing `WebSearcher-0.3.8/WebSearcher/webutils.py` & `WebSearcher-0.3.9/WebSearcher/webutils.py`

 * *Files identical despite different names*

### Comparing `WebSearcher-0.3.8/WebSearcher.egg-info/PKG-INFO` & `WebSearcher-0.3.9/WebSearcher.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WebSearcher
-Version: 0.3.8
+Version: 0.3.9
 Summary: WebSearcher
 Home-page: http://github.com/gitronald/WebSearcher
 Author: Ronald E. Robertson
 Author-email: rer@acm.org
 License: BSD-3-Clause
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `WebSearcher-0.3.8/WebSearcher.egg-info/SOURCES.txt` & `WebSearcher-0.3.9/WebSearcher.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `WebSearcher-0.3.8/setup.py` & `WebSearcher-0.3.9/setup.py`

 * *Files identical despite different names*

