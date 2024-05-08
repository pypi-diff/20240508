# Comparing `tmp/suql-1.1.7a3.tar.gz` & `tmp/suql-1.1.7a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "suql-1.1.7a3.tar", last modified: Tue May  7 05:23:46 2024, max compression
+gzip compressed data, was "suql-1.1.7a4.tar", last modified: Wed May  8 07:12:58 2024, max compression
```

## Comparing `suql-1.1.7a3.tar` & `suql-1.1.7a4.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwx------   0 oval      (1000) users      (100)        0 2024-05-07 05:23:46.020330 suql-1.1.7a3/
--rw-------   0 oval      (1000) users      (100)    11356 2024-04-03 06:02:28.000000 suql-1.1.7a3/LICENSE
--rw-------   0 oval      (1000) users      (100)     5021 2024-05-07 05:23:46.020330 suql-1.1.7a3/PKG-INFO
--rw-------   0 oval      (1000) users      (100)     4415 2024-04-30 04:28:53.000000 suql-1.1.7a3/README.md
--rw-------   0 oval      (1000) users      (100)       38 2024-05-07 05:23:46.020330 suql-1.1.7a3/setup.cfg
--rw-------   0 oval      (1000) users      (100)     1541 2024-05-07 05:23:38.000000 suql-1.1.7a3/setup.py
-drwx------   0 oval      (1000) users      (100)        0 2024-05-07 05:23:46.016330 suql-1.1.7a3/src/
-drwx------   0 oval      (1000) users      (100)        0 2024-05-07 05:23:46.020330 suql-1.1.7a3/src/suql/
--rw-------   0 oval      (1000) users      (100)       73 2024-04-03 06:02:28.000000 suql-1.1.7a3/src/suql/__init__.py
--rw-------   0 oval      (1000) users      (100)    17393 2024-05-02 21:44:59.000000 suql-1.1.7a3/src/suql/agent.py
--rw-------   0 oval      (1000) users      (100)    20887 2024-05-07 05:23:38.000000 suql-1.1.7a3/src/suql/faiss_embedding.py
--rw-------   0 oval      (1000) users      (100)     8792 2024-04-17 07:27:02.000000 suql-1.1.7a3/src/suql/free_text_fcns_server.py
--rw-------   0 oval      (1000) users      (100)     3563 2024-05-06 21:19:43.000000 suql-1.1.7a3/src/suql/postgresql_connection.py
--rw-------   0 oval      (1000) users      (100)     9612 2024-04-17 08:33:05.000000 suql-1.1.7a3/src/suql/prompt_continuation.py
-drwx------   0 oval      (1000) users      (100)        0 2024-05-07 05:23:46.020330 suql-1.1.7a3/src/suql/prompts/
--rw-------   0 oval      (1000) users      (100)        0 2024-04-04 04:29:18.000000 suql-1.1.7a3/src/suql/prompts/__init__.py
--rw-------   0 oval      (1000) users      (100)      169 2024-04-03 06:02:28.000000 suql-1.1.7a3/src/suql/prompts/answer_qa.prompt
--rw-------   0 oval      (1000) users      (100)      451 2024-04-03 06:02:28.000000 suql-1.1.7a3/src/suql/prompts/field_classification.prompt
--rw-------   0 oval      (1000) users      (100)     2945 2024-04-03 06:02:28.000000 suql-1.1.7a3/src/suql/prompts/if_db_classification.prompt
--rw-------   0 oval      (1000) users      (100)     1305 2024-04-03 06:02:28.000000 suql-1.1.7a3/src/suql/prompts/opening_hours.prompt
--rw-------   0 oval      (1000) users      (100)     5574 2024-04-03 06:02:28.000000 suql-1.1.7a3/src/suql/prompts/parser_suql.prompt
--rw-------   0 oval      (1000) users      (100)      227 2024-04-03 06:02:28.000000 suql-1.1.7a3/src/suql/prompts/verification.prompt
--rw-------   0 oval      (1000) users      (100)     2983 2024-04-03 06:02:28.000000 suql-1.1.7a3/src/suql/prompts/yelp_response_SQL.prompt
--rw-------   0 oval      (1000) users      (100)     1454 2024-04-03 06:02:28.000000 suql-1.1.7a3/src/suql/prompts/yelp_response_no_results.prompt
-drwx------   0 oval      (1000) users      (100)        0 2024-05-07 05:23:46.020330 suql-1.1.7a3/src/suql/sql_free_text_support/
--rw-------   0 oval      (1000) users      (100)        0 2024-04-04 04:29:11.000000 suql-1.1.7a3/src/suql/sql_free_text_support/__init__.py
--rw-------   0 oval      (1000) users      (100)    71135 2024-05-07 05:12:07.000000 suql-1.1.7a3/src/suql/sql_free_text_support/execute_free_text_sql.py
--rw-------   0 oval      (1000) users      (100)     6455 2024-04-03 06:02:28.000000 suql-1.1.7a3/src/suql/utils.py
-drwx------   0 oval      (1000) users      (100)        0 2024-05-07 05:23:46.020330 suql-1.1.7a3/src/suql.egg-info/
--rw-r--r--   0 oval      (1000) users      (100)     5021 2024-05-07 05:23:45.000000 suql-1.1.7a3/src/suql.egg-info/PKG-INFO
--rw-------   0 oval      (1000) users      (100)      824 2024-05-07 05:23:45.000000 suql-1.1.7a3/src/suql.egg-info/SOURCES.txt
--rw-------   0 oval      (1000) users      (100)        1 2024-05-07 05:23:45.000000 suql-1.1.7a3/src/suql.egg-info/dependency_links.txt
--rw-------   0 oval      (1000) users      (100)      206 2024-05-07 05:23:45.000000 suql-1.1.7a3/src/suql.egg-info/requires.txt
--rw-------   0 oval      (1000) users      (100)        5 2024-05-07 05:23:45.000000 suql-1.1.7a3/src/suql.egg-info/top_level.txt
+drwx------   0 oval      (1000) users      (100)        0 2024-05-08 07:12:58.295307 suql-1.1.7a4/
+-rw-------   0 oval      (1000) users      (100)    11356 2024-04-03 06:02:28.000000 suql-1.1.7a4/LICENSE
+-rw-------   0 oval      (1000) users      (100)     5021 2024-05-08 07:12:58.295307 suql-1.1.7a4/PKG-INFO
+-rw-------   0 oval      (1000) users      (100)     4415 2024-04-30 04:28:53.000000 suql-1.1.7a4/README.md
+-rw-------   0 oval      (1000) users      (100)       38 2024-05-08 07:12:58.295307 suql-1.1.7a4/setup.cfg
+-rw-------   0 oval      (1000) users      (100)     1541 2024-05-08 07:04:13.000000 suql-1.1.7a4/setup.py
+drwx------   0 oval      (1000) users      (100)        0 2024-05-08 07:12:58.291307 suql-1.1.7a4/src/
+drwx------   0 oval      (1000) users      (100)        0 2024-05-08 07:12:58.291307 suql-1.1.7a4/src/suql/
+-rw-------   0 oval      (1000) users      (100)       73 2024-04-03 06:02:28.000000 suql-1.1.7a4/src/suql/__init__.py
+-rw-------   0 oval      (1000) users      (100)    17372 2024-05-08 07:07:27.000000 suql-1.1.7a4/src/suql/agent.py
+-rw-------   0 oval      (1000) users      (100)    20887 2024-05-07 05:23:38.000000 suql-1.1.7a4/src/suql/faiss_embedding.py
+-rw-------   0 oval      (1000) users      (100)     8792 2024-04-17 07:27:02.000000 suql-1.1.7a4/src/suql/free_text_fcns_server.py
+-rw-------   0 oval      (1000) users      (100)     3563 2024-05-06 21:19:43.000000 suql-1.1.7a4/src/suql/postgresql_connection.py
+-rw-------   0 oval      (1000) users      (100)     9612 2024-04-17 08:33:05.000000 suql-1.1.7a4/src/suql/prompt_continuation.py
+drwx------   0 oval      (1000) users      (100)        0 2024-05-08 07:12:58.295307 suql-1.1.7a4/src/suql/prompts/
+-rw-------   0 oval      (1000) users      (100)        0 2024-04-04 04:29:18.000000 suql-1.1.7a4/src/suql/prompts/__init__.py
+-rw-------   0 oval      (1000) users      (100)      169 2024-04-03 06:02:28.000000 suql-1.1.7a4/src/suql/prompts/answer_qa.prompt
+-rw-------   0 oval      (1000) users      (100)      451 2024-04-03 06:02:28.000000 suql-1.1.7a4/src/suql/prompts/field_classification.prompt
+-rw-------   0 oval      (1000) users      (100)     2945 2024-04-03 06:02:28.000000 suql-1.1.7a4/src/suql/prompts/if_db_classification.prompt
+-rw-------   0 oval      (1000) users      (100)     1305 2024-04-03 06:02:28.000000 suql-1.1.7a4/src/suql/prompts/opening_hours.prompt
+-rw-------   0 oval      (1000) users      (100)     5671 2024-05-08 07:10:13.000000 suql-1.1.7a4/src/suql/prompts/parser_suql.prompt
+-rw-------   0 oval      (1000) users      (100)      227 2024-04-03 06:02:28.000000 suql-1.1.7a4/src/suql/prompts/verification.prompt
+-rw-------   0 oval      (1000) users      (100)     2983 2024-04-03 06:02:28.000000 suql-1.1.7a4/src/suql/prompts/yelp_response_SQL.prompt
+-rw-------   0 oval      (1000) users      (100)     1454 2024-04-03 06:02:28.000000 suql-1.1.7a4/src/suql/prompts/yelp_response_no_results.prompt
+drwx------   0 oval      (1000) users      (100)        0 2024-05-08 07:12:58.295307 suql-1.1.7a4/src/suql/sql_free_text_support/
+-rw-------   0 oval      (1000) users      (100)        0 2024-04-04 04:29:11.000000 suql-1.1.7a4/src/suql/sql_free_text_support/__init__.py
+-rw-------   0 oval      (1000) users      (100)    71135 2024-05-08 07:04:05.000000 suql-1.1.7a4/src/suql/sql_free_text_support/execute_free_text_sql.py
+-rw-------   0 oval      (1000) users      (100)     6455 2024-04-03 06:02:28.000000 suql-1.1.7a4/src/suql/utils.py
+drwx------   0 oval      (1000) users      (100)        0 2024-05-08 07:12:58.291307 suql-1.1.7a4/src/suql.egg-info/
+-rw-r--r--   0 oval      (1000) users      (100)     5021 2024-05-08 07:12:58.000000 suql-1.1.7a4/src/suql.egg-info/PKG-INFO
+-rw-------   0 oval      (1000) users      (100)      824 2024-05-08 07:12:58.000000 suql-1.1.7a4/src/suql.egg-info/SOURCES.txt
+-rw-------   0 oval      (1000) users      (100)        1 2024-05-08 07:12:58.000000 suql-1.1.7a4/src/suql.egg-info/dependency_links.txt
+-rw-------   0 oval      (1000) users      (100)      206 2024-05-08 07:12:58.000000 suql-1.1.7a4/src/suql.egg-info/requires.txt
+-rw-------   0 oval      (1000) users      (100)        5 2024-05-08 07:12:58.000000 suql-1.1.7a4/src/suql.egg-info/top_level.txt
```

### Comparing `suql-1.1.7a3/LICENSE` & `suql-1.1.7a4/LICENSE`

 * *Files identical despite different names*

### Comparing `suql-1.1.7a3/PKG-INFO` & `suql-1.1.7a4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: suql
-Version: 1.1.7a3
+Version: 1.1.7a4
 Summary: Structured and Unstructured Query Language (SUQL) Python API
 Home-page: https://github.com/stanford-oval/suql
 Author: Shicheng Liu
 Author-email: shicheng@cs.stanford.edu
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: suql Version: 1.1.7a3 Summary: Structured and
+Metadata-Version: 2.1 Name: suql Version: 1.1.7a4 Summary: Structured and
 Unstructured Query Language (SUQL) Python API Home-page: https://github.com/
 stanford-oval/suql Author: Shicheng Liu Author-email: shicheng@cs.stanford.edu
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Description-Content-Type: text/markdown License-File: LICENSE
```

### Comparing `suql-1.1.7a3/README.md` & `suql-1.1.7a4/README.md`

 * *Files identical despite different names*

### Comparing `suql-1.1.7a3/setup.py` & `suql-1.1.7a4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 # Package metadata
 name = "suql"
-version = "1.1.7a3"
+version = "1.1.7a4"
 description = "Structured and Unstructured Query Language (SUQL) Python API"
 author = "Shicheng Liu"
 author_email = "shicheng@cs.stanford.edu"
 url = "https://github.com/stanford-oval/suql"
 
 # Specify the packages to include. You can use `find_packages` to automatically discover them.
 packages = find_packages(where="src")
```

### Comparing `suql-1.1.7a3/src/suql/agent.py` & `suql-1.1.7a4/src/suql/agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -366,15 +366,15 @@
                 max_tokens=200,
                 temperature=0.0,
                 stop_tokens=["\n"],
                 postprocess=False,
             )
             return response
 
-        pattern = r"'([^']*)'\s*=\s*ANY\(CAST opening_hours AS ARRAY\)"
+        pattern = r"'([^']*)'\s*=\s*opening_hours"
 
         def replacer(match):
             opening_hours_query = match.group(0).split(" = ")[0]
             opening_hours_translated = convert_opening_hours_query(opening_hours_query)
             return (
                 'search_by_opening_hours("opening_hours", '
                 + "'"
```

### Comparing `suql-1.1.7a3/src/suql/faiss_embedding.py` & `suql-1.1.7a4/src/suql/faiss_embedding.py`

 * *Files identical despite different names*

### Comparing `suql-1.1.7a3/src/suql/free_text_fcns_server.py` & `suql-1.1.7a4/src/suql/free_text_fcns_server.py`

 * *Files identical despite different names*

### Comparing `suql-1.1.7a3/src/suql/postgresql_connection.py` & `suql-1.1.7a4/src/suql/postgresql_connection.py`

 * *Files identical despite different names*

### Comparing `suql-1.1.7a3/src/suql/prompt_continuation.py` & `suql-1.1.7a4/src/suql/prompt_continuation.py`

 * *Files identical despite different names*

### Comparing `suql-1.1.7a3/src/suql/prompts/if_db_classification.prompt` & `suql-1.1.7a4/src/suql/prompts/if_db_classification.prompt`

 * *Files identical despite different names*

### Comparing `suql-1.1.7a3/src/suql/prompts/opening_hours.prompt` & `suql-1.1.7a4/src/suql/prompts/opening_hours.prompt`

 * *Files identical despite different names*

### Comparing `suql-1.1.7a3/src/suql/prompts/parser_suql.prompt` & `suql-1.1.7a4/src/suql/prompts/parser_suql.prompt`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     reviews FREE_TEXT,
     opening_hours TEXT,
     location TEXT
 );
 
 Do not generate fields beyond the given fields. The `answer` function can be used on FREE_TEXT fields. 
 Use `location = 'some place'` to search restaurants that are geographically close, don't use other operations on the location field.
+Use `'some string' = opening_hours` to search restaurants open at certain time, don't use other operations on the opening_hours field.
 
 {# Basic example #}
 User: Where is Burguer King?
 Target: SELECT _id, name, location, summary(reviews) FROM restaurants WHERE name = 'Wesley''s Steakhouse' LIMIT 1;
 --
 {# Basic example for cuisine, and follow up with restaurant names #}
 User: what are some good-reviewed japanese restaurants in downtown Kansas City?
@@ -63,19 +64,19 @@
 Results: [{'_id': 53, 'name': "Daigo"}]
 Agent: I found the 4.5 star Daigo. It is a family-owned business that serves traditional Japanese cuisine.
 User: Show me something else.
 Target: SELECT *, answer(popular_dishes, 'does this restaurant serve salmon?'), summary(reviews) FROM restaurants WHERE NOT(_id = 53) AND answer(popular_dishes, 'does this restaurant serve salmon?') = 'Yes' AND location = 'Chicago' LIMIT 1;
 --
 {# How to search by opening hours #}
 User: What restaurants are open after 2pm on Monday?
-Target: SELECT * FROM restaurants WHERE 'after 2pm on Monday' = ANY(CAST opening_hours AS ARRAY);
+Target: SELECT * FROM restaurants WHERE 'after 2pm on Monday' = opening_hours;
 __
 {# How to search by opening hours - segments #}
 User: restaurants open after 3am and before 7am on Monday?
-Target: SELECT * FROM restaurants WHERE 'after 3am and before 7am on Monday' = ANY(CAST opening_hours AS ARRAY);
+Target: SELECT * FROM restaurants WHERE 'after 3am and before 7am on Monday' = opening_hours;
 __
 
 {% for dlg_turn in dlg[:-1] %}
 {% if dlg_turn.db_results is not none %}
 User: {{ dlg_turn.user_utterance }}
 Target: {{ dlg_turn.user_target }}
 Agent: {{ dlg_turn.agent_utterance }}
```

### Comparing `suql-1.1.7a3/src/suql/prompts/yelp_response_SQL.prompt` & `suql-1.1.7a4/src/suql/prompts/yelp_response_SQL.prompt`

 * *Files identical despite different names*

### Comparing `suql-1.1.7a3/src/suql/prompts/yelp_response_no_results.prompt` & `suql-1.1.7a4/src/suql/prompts/yelp_response_no_results.prompt`

 * *Files identical despite different names*

### Comparing `suql-1.1.7a3/src/suql/sql_free_text_support/execute_free_text_sql.py` & `suql-1.1.7a4/src/suql/sql_free_text_support/execute_free_text_sql.py`

 * *Files identical despite different names*

### Comparing `suql-1.1.7a3/src/suql/utils.py` & `suql-1.1.7a4/src/suql/utils.py`

 * *Files identical despite different names*

### Comparing `suql-1.1.7a3/src/suql.egg-info/PKG-INFO` & `suql-1.1.7a4/src/suql.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: suql
-Version: 1.1.7a3
+Version: 1.1.7a4
 Summary: Structured and Unstructured Query Language (SUQL) Python API
 Home-page: https://github.com/stanford-oval/suql
 Author: Shicheng Liu
 Author-email: shicheng@cs.stanford.edu
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: suql Version: 1.1.7a3 Summary: Structured and
+Metadata-Version: 2.1 Name: suql Version: 1.1.7a4 Summary: Structured and
 Unstructured Query Language (SUQL) Python API Home-page: https://github.com/
 stanford-oval/suql Author: Shicheng Liu Author-email: shicheng@cs.stanford.edu
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Description-Content-Type: text/markdown License-File: LICENSE
```

### Comparing `suql-1.1.7a3/src/suql.egg-info/SOURCES.txt` & `suql-1.1.7a4/src/suql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

