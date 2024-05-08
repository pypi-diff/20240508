# Comparing `tmp/llm_perplexity-0.5.tar.gz` & `tmp/llm_perplexity-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm_perplexity-0.5.tar", last modified: Fri Apr 19 07:29:45 2024, max compression
+gzip compressed data, was "llm_perplexity-0.6.tar", last modified: Wed May  8 07:33:55 2024, max compression
```

## Comparing `llm_perplexity-0.5.tar` & `llm_perplexity-0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 07:29:45.509863 llm_perplexity-0.5/
--rw-r--r--   0 runner    (1001) docker     (127)    11324 2024-04-19 07:29:36.000000 llm_perplexity-0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-04-19 07:29:45.509863 llm_perplexity-0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-04-19 07:29:36.000000 llm_perplexity-0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 07:29:45.509863 llm_perplexity-0.5/llm_perplexity.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-04-19 07:29:45.000000 llm_perplexity-0.5/llm_perplexity.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-19 07:29:45.000000 llm_perplexity-0.5/llm_perplexity.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 07:29:45.000000 llm_perplexity-0.5/llm_perplexity.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-19 07:29:45.000000 llm_perplexity-0.5/llm_perplexity.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-19 07:29:45.000000 llm_perplexity-0.5/llm_perplexity.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-19 07:29:45.000000 llm_perplexity-0.5/llm_perplexity.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6901 2024-04-19 07:29:36.000000 llm_perplexity-0.5/llm_perplexity.py
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-19 07:29:36.000000 llm_perplexity-0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 07:29:45.509863 llm_perplexity-0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:33:55.333947 llm_perplexity-0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    11324 2024-05-08 07:33:48.000000 llm_perplexity-0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-05-08 07:33:55.333947 llm_perplexity-0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-05-08 07:33:48.000000 llm_perplexity-0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:33:55.333947 llm_perplexity-0.6/llm_perplexity.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-05-08 07:33:55.000000 llm_perplexity-0.6/llm_perplexity.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-08 07:33:55.000000 llm_perplexity-0.6/llm_perplexity.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 07:33:55.000000 llm_perplexity-0.6/llm_perplexity.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-08 07:33:55.000000 llm_perplexity-0.6/llm_perplexity.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-08 07:33:55.000000 llm_perplexity-0.6/llm_perplexity.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-08 07:33:55.000000 llm_perplexity-0.6/llm_perplexity.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5806 2024-05-08 07:33:48.000000 llm_perplexity-0.6/llm_perplexity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-08 07:33:48.000000 llm_perplexity-0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 07:33:55.333947 llm_perplexity-0.6/setup.cfg
```

### Comparing `llm_perplexity-0.5/LICENSE` & `llm_perplexity-0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `llm_perplexity-0.5/PKG-INFO` & `llm_perplexity-0.6/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm-perplexity
-Version: 0.5
+Version: 0.6
 Summary: LLM access to pplx-api 3 by Perplexity Labs
 Author: hex
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/hex/llm-perplexity
 Project-URL: Changelog, https://github.com/hex/llm-perplexity/releases
 Project-URL: Issues, https://github.com/hex/llm-perplexity/issues
 Project-URL: CI, https://github.com/hex/llm-perplexity/actions
@@ -40,20 +40,20 @@
 ```
 
 Run `llm models` to list the models, and `llm models --options` to include a list of their options.
 
 Run prompts like this:
 
 ```bash
-llm -m sonar-small-chat 'Fun facts about pelicans'
-llm -m sonar-small-online 'Fun facts about walruses'
-llm -m sonar-medium-chat 'Fun facts about wolves'
-llm -m sonar-medium-online 'Fun facts about foxes'
-llm -m codellama-70b-instruct 'Fun facts about lemurs'
-llm -m mistral-7b-instruct 'Fun facts about coyotes'
+llm -m llama-3-sonar-small-32k-chat 'Fun facts about pelicans'
+llm -m llama-3-sonar-small-32k-online 'Fun facts about walruses'
+llm -m llama-3-sonar-large-32k-chat 'Fun facts about wolves'
+llm -m llama-3-sonar-large-32k-online 'Fun facts about foxes'
+llm -m llama-3-8b-instruct 'Fun facts about lemurs'
+llm -m llama-3-70b-instruct 'Fun facts about coyotes'
 llm -m mixtral-8x7b-instruct 'Fun facts about tigers'
 ```
 
 ## Development
 
 To set up this plugin locally, first checkout the code. Then create a new virtual environment:
```

### Comparing `llm_perplexity-0.5/README.md` & `llm_perplexity-0.6/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -24,20 +24,20 @@
 ```
 
 Run `llm models` to list the models, and `llm models --options` to include a list of their options.
 
 Run prompts like this:
 
 ```bash
-llm -m sonar-small-chat 'Fun facts about pelicans'
-llm -m sonar-small-online 'Fun facts about walruses'
-llm -m sonar-medium-chat 'Fun facts about wolves'
-llm -m sonar-medium-online 'Fun facts about foxes'
-llm -m codellama-70b-instruct 'Fun facts about lemurs'
-llm -m mistral-7b-instruct 'Fun facts about coyotes'
+llm -m llama-3-sonar-small-32k-chat 'Fun facts about pelicans'
+llm -m llama-3-sonar-small-32k-online 'Fun facts about walruses'
+llm -m llama-3-sonar-large-32k-chat 'Fun facts about wolves'
+llm -m llama-3-sonar-large-32k-online 'Fun facts about foxes'
+llm -m llama-3-8b-instruct 'Fun facts about lemurs'
+llm -m llama-3-70b-instruct 'Fun facts about coyotes'
 llm -m mixtral-8x7b-instruct 'Fun facts about tigers'
 ```
 
 ## Development
 
 To set up this plugin locally, first checkout the code. Then create a new virtual environment:
```

### Comparing `llm_perplexity-0.5/llm_perplexity.egg-info/PKG-INFO` & `llm_perplexity-0.6/llm_perplexity.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm-perplexity
-Version: 0.5
+Version: 0.6
 Summary: LLM access to pplx-api 3 by Perplexity Labs
 Author: hex
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/hex/llm-perplexity
 Project-URL: Changelog, https://github.com/hex/llm-perplexity/releases
 Project-URL: Issues, https://github.com/hex/llm-perplexity/issues
 Project-URL: CI, https://github.com/hex/llm-perplexity/actions
@@ -40,20 +40,20 @@
 ```
 
 Run `llm models` to list the models, and `llm models --options` to include a list of their options.
 
 Run prompts like this:
 
 ```bash
-llm -m sonar-small-chat 'Fun facts about pelicans'
-llm -m sonar-small-online 'Fun facts about walruses'
-llm -m sonar-medium-chat 'Fun facts about wolves'
-llm -m sonar-medium-online 'Fun facts about foxes'
-llm -m codellama-70b-instruct 'Fun facts about lemurs'
-llm -m mistral-7b-instruct 'Fun facts about coyotes'
+llm -m llama-3-sonar-small-32k-chat 'Fun facts about pelicans'
+llm -m llama-3-sonar-small-32k-online 'Fun facts about walruses'
+llm -m llama-3-sonar-large-32k-chat 'Fun facts about wolves'
+llm -m llama-3-sonar-large-32k-online 'Fun facts about foxes'
+llm -m llama-3-8b-instruct 'Fun facts about lemurs'
+llm -m llama-3-70b-instruct 'Fun facts about coyotes'
 llm -m mixtral-8x7b-instruct 'Fun facts about tigers'
 ```
 
 ## Development
 
 To set up this plugin locally, first checkout the code. Then create a new virtual environment:
```

### Comparing `llm_perplexity-0.5/pyproject.toml` & `llm_perplexity-0.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "llm-perplexity"
-version = "0.5"
+version = "0.6"
 description = "LLM access to pplx-api 3 by Perplexity Labs"
 readme = "README.md"
 authors = [{name = "hex"}]
 license = {text = "Apache-2.0"}
 classifiers = [
     "License :: OSI Approved :: Apache Software License"
 ]
```

