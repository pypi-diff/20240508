# Comparing `tmp/wm_topicgpt-0.1.3.tar.gz` & `tmp/wm_topicgpt-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wm_topicgpt-0.1.3.tar", last modified: Tue May  7 14:46:18 2024, max compression
+gzip compressed data, was "wm_topicgpt-0.1.4.tar", last modified: Wed May  8 19:41:16 2024, max compression
```

## Comparing `wm_topicgpt-0.1.3.tar` & `wm_topicgpt-0.1.4.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-05-07 14:46:18.971609 wm_topicgpt-0.1.3/
--rw-r--r--   0 y0h07pr    (503) staff       (20)     7118 2024-05-07 14:46:18.971016 wm_topicgpt-0.1.3/PKG-INFO
--rw-r--r--   0 y0h07pr    (503) staff       (20)       38 2024-05-07 14:46:18.971668 wm_topicgpt-0.1.3/setup.cfg
--rw-r--r--   0 y0h07pr    (503) staff       (20)      601 2024-05-07 14:45:56.000000 wm_topicgpt-0.1.3/setup.py
-drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-05-07 14:46:18.938168 wm_topicgpt-0.1.3/topicgpt/
--rw-r--r--   0 y0h07pr    (503) staff       (20)      209 2024-05-07 14:20:30.000000 wm_topicgpt-0.1.3/topicgpt/__init__.py
--rw-r--r--   0 y0h07pr    (503) staff       (20)      312 2024-05-05 05:35:46.000000 wm_topicgpt-0.1.3/topicgpt/_config.py
--rw-r--r--   0 y0h07pr    (503) staff       (20)      276 2024-05-04 00:03:35.000000 wm_topicgpt-0.1.3/topicgpt/base.py
-drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-05-07 14:46:18.943948 wm_topicgpt-0.1.3/topicgpt/clustering/
--rw-r--r--   0 y0h07pr    (503) staff       (20)      191 2024-05-05 22:35:15.000000 wm_topicgpt-0.1.3/topicgpt/clustering/__init__.py
--rw-r--r--   0 y0h07pr    (503) staff       (20)      428 2024-05-06 03:49:21.000000 wm_topicgpt-0.1.3/topicgpt/clustering/_base_cluster.py
--rw-r--r--   0 y0h07pr    (503) staff       (20)     3035 2024-05-06 14:14:30.000000 wm_topicgpt-0.1.3/topicgpt/clustering/_hdbscan.py
--rw-r--r--   0 y0h07pr    (503) staff       (20)    10045 2024-05-06 18:24:02.000000 wm_topicgpt-0.1.3/topicgpt/clustering/_kmeans.py
--rw-r--r--   0 y0h07pr    (503) staff       (20)     2285 2024-05-05 03:15:39.000000 wm_topicgpt-0.1.3/topicgpt/clustering/_sampling.py
-drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-05-07 14:46:18.948934 wm_topicgpt-0.1.3/topicgpt/generation/
--rw-r--r--   0 y0h07pr    (503) staff       (20)      138 2024-05-06 16:56:29.000000 wm_topicgpt-0.1.3/topicgpt/generation/__init__.py
--rw-r--r--   0 y0h07pr    (503) staff       (20)     2910 2024-05-07 01:27:18.000000 wm_topicgpt-0.1.3/topicgpt/generation/_keywords.py
--rw-r--r--   0 y0h07pr    (503) staff       (20)     5501 2024-05-06 19:42:11.000000 wm_topicgpt-0.1.3/topicgpt/generation/_topic.py
-drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-05-07 14:46:18.952970 wm_topicgpt-0.1.3/topicgpt/persistence/
--rw-r--r--   0 y0h07pr    (503) staff       (20)      330 2024-05-07 01:26:00.000000 wm_topicgpt-0.1.3/topicgpt/persistence/__init__.py
--rw-r--r--   0 y0h07pr    (503) staff       (20)     1012 2024-05-06 03:42:53.000000 wm_topicgpt-0.1.3/topicgpt/persistence/_plot.py
--rw-r--r--   0 y0h07pr    (503) staff       (20)     4297 2024-05-07 03:09:02.000000 wm_topicgpt-0.1.3/topicgpt/persistence/_save.py
--rw-r--r--   0 y0h07pr    (503) staff       (20)     5375 2024-05-07 14:43:13.000000 wm_topicgpt-0.1.3/topicgpt/pipeline.py
-drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-05-07 14:46:18.956369 wm_topicgpt-0.1.3/topicgpt/preprocessing/
--rw-r--r--   0 y0h07pr    (503) staff       (20)      108 2024-05-03 23:14:55.000000 wm_topicgpt-0.1.3/topicgpt/preprocessing/__init__.py
--rw-r--r--   0 y0h07pr    (503) staff       (20)     2854 2024-05-03 23:14:55.000000 wm_topicgpt-0.1.3/topicgpt/preprocessing/_data.py
--rw-r--r--   0 y0h07pr    (503) staff       (20)      412 2024-05-06 00:04:30.000000 wm_topicgpt-0.1.3/topicgpt/utils.py
-drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-05-07 14:46:18.963163 wm_topicgpt-0.1.3/topicgpt/walmart_llm/
--rw-r--r--   0 y0h07pr    (503) staff       (20)      153 2024-05-03 23:24:30.000000 wm_topicgpt-0.1.3/topicgpt/walmart_llm/__init__.py
--rw-r--r--   0 y0h07pr    (503) staff       (20)     9052 2024-05-03 23:35:49.000000 wm_topicgpt-0.1.3/topicgpt/walmart_llm/_chat_model.py
--rw-r--r--   0 y0h07pr    (503) staff       (20)     8079 2024-05-03 20:57:39.000000 wm_topicgpt-0.1.3/topicgpt/walmart_llm/_embed_model.py
--rw-r--r--   0 y0h07pr    (503) staff       (20)     7922 2024-05-03 23:35:53.000000 wm_topicgpt-0.1.3/topicgpt/walmart_llm/_llm_client.py
-drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-05-07 14:46:18.970179 wm_topicgpt-0.1.3/wm_topicgpt.egg-info/
--rw-r--r--   0 y0h07pr    (503) staff       (20)     7118 2024-05-07 14:46:18.000000 wm_topicgpt-0.1.3/wm_topicgpt.egg-info/PKG-INFO
--rw-r--r--   0 y0h07pr    (503) staff       (20)      841 2024-05-07 14:46:18.000000 wm_topicgpt-0.1.3/wm_topicgpt.egg-info/SOURCES.txt
--rw-r--r--   0 y0h07pr    (503) staff       (20)        1 2024-05-07 14:46:18.000000 wm_topicgpt-0.1.3/wm_topicgpt.egg-info/dependency_links.txt
--rw-r--r--   0 y0h07pr    (503) staff       (20)      360 2024-05-07 14:46:18.000000 wm_topicgpt-0.1.3/wm_topicgpt.egg-info/requires.txt
--rw-r--r--   0 y0h07pr    (503) staff       (20)        9 2024-05-07 14:46:18.000000 wm_topicgpt-0.1.3/wm_topicgpt.egg-info/top_level.txt
+drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-05-08 19:41:16.188835 wm_topicgpt-0.1.4/
+-rw-r--r--   0 y0h07pr    (503) staff       (20)     7213 2024-05-08 19:41:16.188302 wm_topicgpt-0.1.4/PKG-INFO
+-rw-r--r--   0 y0h07pr    (503) staff       (20)       38 2024-05-08 19:41:16.188911 wm_topicgpt-0.1.4/setup.cfg
+-rw-r--r--   0 y0h07pr    (503) staff       (20)      601 2024-05-08 19:39:39.000000 wm_topicgpt-0.1.4/setup.py
+drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-05-08 19:41:16.167557 wm_topicgpt-0.1.4/topicgpt/
+-rw-r--r--   0 y0h07pr    (503) staff       (20)      209 2024-05-08 19:39:47.000000 wm_topicgpt-0.1.4/topicgpt/__init__.py
+-rw-r--r--   0 y0h07pr    (503) staff       (20)      312 2024-05-05 05:35:46.000000 wm_topicgpt-0.1.4/topicgpt/_config.py
+-rw-r--r--   0 y0h07pr    (503) staff       (20)      276 2024-05-04 00:03:35.000000 wm_topicgpt-0.1.4/topicgpt/base.py
+drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-05-08 19:41:16.170571 wm_topicgpt-0.1.4/topicgpt/clustering/
+-rw-r--r--   0 y0h07pr    (503) staff       (20)      191 2024-05-05 22:35:15.000000 wm_topicgpt-0.1.4/topicgpt/clustering/__init__.py
+-rw-r--r--   0 y0h07pr    (503) staff       (20)      428 2024-05-06 03:49:21.000000 wm_topicgpt-0.1.4/topicgpt/clustering/_base_cluster.py
+-rw-r--r--   0 y0h07pr    (503) staff       (20)     3035 2024-05-06 14:14:30.000000 wm_topicgpt-0.1.4/topicgpt/clustering/_hdbscan.py
+-rw-r--r--   0 y0h07pr    (503) staff       (20)    10045 2024-05-06 18:24:02.000000 wm_topicgpt-0.1.4/topicgpt/clustering/_kmeans.py
+-rw-r--r--   0 y0h07pr    (503) staff       (20)     2285 2024-05-05 03:15:39.000000 wm_topicgpt-0.1.4/topicgpt/clustering/_sampling.py
+drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-05-08 19:41:16.173455 wm_topicgpt-0.1.4/topicgpt/generation/
+-rw-r--r--   0 y0h07pr    (503) staff       (20)      138 2024-05-06 16:56:29.000000 wm_topicgpt-0.1.4/topicgpt/generation/__init__.py
+-rw-r--r--   0 y0h07pr    (503) staff       (20)     2910 2024-05-07 01:27:18.000000 wm_topicgpt-0.1.4/topicgpt/generation/_keywords.py
+-rw-r--r--   0 y0h07pr    (503) staff       (20)     5765 2024-05-07 18:47:15.000000 wm_topicgpt-0.1.4/topicgpt/generation/_topic.py
+drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-05-08 19:41:16.175996 wm_topicgpt-0.1.4/topicgpt/persistence/
+-rw-r--r--   0 y0h07pr    (503) staff       (20)      330 2024-05-07 01:26:00.000000 wm_topicgpt-0.1.4/topicgpt/persistence/__init__.py
+-rw-r--r--   0 y0h07pr    (503) staff       (20)     1012 2024-05-06 03:42:53.000000 wm_topicgpt-0.1.4/topicgpt/persistence/_plot.py
+-rw-r--r--   0 y0h07pr    (503) staff       (20)     4297 2024-05-07 03:09:02.000000 wm_topicgpt-0.1.4/topicgpt/persistence/_save.py
+-rw-r--r--   0 y0h07pr    (503) staff       (20)     5375 2024-05-07 14:43:13.000000 wm_topicgpt-0.1.4/topicgpt/pipeline.py
+drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-05-08 19:41:16.178175 wm_topicgpt-0.1.4/topicgpt/preprocessing/
+-rw-r--r--   0 y0h07pr    (503) staff       (20)      108 2024-05-03 23:14:55.000000 wm_topicgpt-0.1.4/topicgpt/preprocessing/__init__.py
+-rw-r--r--   0 y0h07pr    (503) staff       (20)     2854 2024-05-03 23:14:55.000000 wm_topicgpt-0.1.4/topicgpt/preprocessing/_data.py
+-rw-r--r--   0 y0h07pr    (503) staff       (20)      412 2024-05-06 00:04:30.000000 wm_topicgpt-0.1.4/topicgpt/utils.py
+drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-05-08 19:41:16.180258 wm_topicgpt-0.1.4/topicgpt/walmart_llm/
+-rw-r--r--   0 y0h07pr    (503) staff       (20)      153 2024-05-03 23:24:30.000000 wm_topicgpt-0.1.4/topicgpt/walmart_llm/__init__.py
+-rw-r--r--   0 y0h07pr    (503) staff       (20)     9052 2024-05-03 23:35:49.000000 wm_topicgpt-0.1.4/topicgpt/walmart_llm/_chat_model.py
+-rw-r--r--   0 y0h07pr    (503) staff       (20)     8079 2024-05-03 20:57:39.000000 wm_topicgpt-0.1.4/topicgpt/walmart_llm/_embed_model.py
+-rw-r--r--   0 y0h07pr    (503) staff       (20)     7922 2024-05-03 23:35:53.000000 wm_topicgpt-0.1.4/topicgpt/walmart_llm/_llm_client.py
+drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-05-08 19:41:16.187433 wm_topicgpt-0.1.4/wm_topicgpt.egg-info/
+-rw-r--r--   0 y0h07pr    (503) staff       (20)     7213 2024-05-08 19:41:16.000000 wm_topicgpt-0.1.4/wm_topicgpt.egg-info/PKG-INFO
+-rw-r--r--   0 y0h07pr    (503) staff       (20)      841 2024-05-08 19:41:16.000000 wm_topicgpt-0.1.4/wm_topicgpt.egg-info/SOURCES.txt
+-rw-r--r--   0 y0h07pr    (503) staff       (20)        1 2024-05-08 19:41:16.000000 wm_topicgpt-0.1.4/wm_topicgpt.egg-info/dependency_links.txt
+-rw-r--r--   0 y0h07pr    (503) staff       (20)      360 2024-05-08 19:41:16.000000 wm_topicgpt-0.1.4/wm_topicgpt.egg-info/requires.txt
+-rw-r--r--   0 y0h07pr    (503) staff       (20)        9 2024-05-08 19:41:16.000000 wm_topicgpt-0.1.4/wm_topicgpt.egg-info/top_level.txt
```

### Comparing `wm_topicgpt-0.1.3/PKG-INFO` & `wm_topicgpt-0.1.4/wm_topicgpt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: wm_topicgpt
-Version: 0.1.3
+Name: wm-topicgpt
+Version: 0.1.4
 Summary: This is a package to generate topics for the text corpus.
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: numpy==1.26.4
 Requires-Dist: pandas==2.2.1
 Requires-Dist: tqdm==4.66.2
 Requires-Dist: azure-ai-textanalytics==5.3.0
@@ -22,14 +22,20 @@
 Requires-Dist: gradio==4.28.3
 Requires-Dist: appscript==1.2.5
 Requires-Dist: keybert==0.8.4
 Requires-Dist: pyarrow==16.0.0
 
 # TopicGPT package
 
+## Create a virtual environment
+```python
+conda create -n your_env_name
+conda install pip
+```
+
 ## How to install this package?
 ```python
 pip install wm_topicgpt
 ```
 
 ## How to use this package?
```

### Comparing `wm_topicgpt-0.1.3/setup.py` & `wm_topicgpt-0.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     install_requires = f.read().splitlines()
 
 with open("topicgpt/README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name='wm_topicgpt',
-    version='0.1.3',
+    version='0.1.4',
     description='This is a package to generate topics for the text corpus.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     install_requires=install_requires,
     python_requires='>=3.9',
 )
```

### Comparing `wm_topicgpt-0.1.3/topicgpt/clustering/_hdbscan.py` & `wm_topicgpt-0.1.4/topicgpt/clustering/_hdbscan.py`

 * *Files identical despite different names*

### Comparing `wm_topicgpt-0.1.3/topicgpt/clustering/_kmeans.py` & `wm_topicgpt-0.1.4/topicgpt/clustering/_kmeans.py`

 * *Files identical despite different names*

### Comparing `wm_topicgpt-0.1.3/topicgpt/clustering/_sampling.py` & `wm_topicgpt-0.1.4/topicgpt/clustering/_sampling.py`

 * *Files identical despite different names*

### Comparing `wm_topicgpt-0.1.3/topicgpt/generation/_keywords.py` & `wm_topicgpt-0.1.4/topicgpt/generation/_keywords.py`

 * *Files identical despite different names*

### Comparing `wm_topicgpt-0.1.3/topicgpt/generation/_topic.py` & `wm_topicgpt-0.1.4/topicgpt/generation/_topic.py`

 * *Files 6% similar despite different names*

```diff
@@ -67,18 +67,23 @@
         # summary_responses = self.model.batch_completion(summary_prompts)
         for cluster, topic_response in zip(clusters, topic_responses):
             try:
                 cluster.topic = eval(topic_response)['topic']
                 cluster.description = eval(topic_response)['description']
                 cluster.summary = eval(topic_response)['summary']
             except:
-                topic_response= self.process_exception(cluster)
-                cluster.topic = eval(topic_response)['topic']
-                cluster.description = eval(topic_response)['description']
-                cluster.summary = eval(topic_response)['summary']
+                try:
+                    topic_response= self.process_exception(cluster)
+                    cluster.topic = eval(topic_response)['topic']
+                    cluster.description = eval(topic_response)['description']
+                    cluster.summary = eval(topic_response)['summary']
+                except:
+                    cluster.topic = "OpenAI's poilicy Violation"
+                    cluster.description = "OpenAI's poilicy Violation"
+                    cluster.summary = "OpenAI's poilicy Violation"
 
     def process_exception(self, cluster):
         ranked_idx = cluster.ranked_idx.copy()
         np.random.shuffle(ranked_idx)
         text = ""
         for idx in ranked_idx[:self.topk]:
             tmp_text = cluster.data.iloc[idx]['input']
```

### Comparing `wm_topicgpt-0.1.3/topicgpt/persistence/_plot.py` & `wm_topicgpt-0.1.4/topicgpt/persistence/_plot.py`

 * *Files identical despite different names*

### Comparing `wm_topicgpt-0.1.3/topicgpt/persistence/_save.py` & `wm_topicgpt-0.1.4/topicgpt/persistence/_save.py`

 * *Files identical despite different names*

### Comparing `wm_topicgpt-0.1.3/topicgpt/pipeline.py` & `wm_topicgpt-0.1.4/topicgpt/pipeline.py`

 * *Files identical despite different names*

### Comparing `wm_topicgpt-0.1.3/topicgpt/preprocessing/_data.py` & `wm_topicgpt-0.1.4/topicgpt/preprocessing/_data.py`

 * *Files identical despite different names*

### Comparing `wm_topicgpt-0.1.3/topicgpt/walmart_llm/_chat_model.py` & `wm_topicgpt-0.1.4/topicgpt/walmart_llm/_chat_model.py`

 * *Files identical despite different names*

### Comparing `wm_topicgpt-0.1.3/topicgpt/walmart_llm/_embed_model.py` & `wm_topicgpt-0.1.4/topicgpt/walmart_llm/_embed_model.py`

 * *Files identical despite different names*

### Comparing `wm_topicgpt-0.1.3/topicgpt/walmart_llm/_llm_client.py` & `wm_topicgpt-0.1.4/topicgpt/walmart_llm/_llm_client.py`

 * *Files identical despite different names*

### Comparing `wm_topicgpt-0.1.3/wm_topicgpt.egg-info/PKG-INFO` & `wm_topicgpt-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: wm-topicgpt
-Version: 0.1.3
+Name: wm_topicgpt
+Version: 0.1.4
 Summary: This is a package to generate topics for the text corpus.
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: numpy==1.26.4
 Requires-Dist: pandas==2.2.1
 Requires-Dist: tqdm==4.66.2
 Requires-Dist: azure-ai-textanalytics==5.3.0
@@ -22,14 +22,20 @@
 Requires-Dist: gradio==4.28.3
 Requires-Dist: appscript==1.2.5
 Requires-Dist: keybert==0.8.4
 Requires-Dist: pyarrow==16.0.0
 
 # TopicGPT package
 
+## Create a virtual environment
+```python
+conda create -n your_env_name
+conda install pip
+```
+
 ## How to install this package?
 ```python
 pip install wm_topicgpt
 ```
 
 ## How to use this package?
```

### Comparing `wm_topicgpt-0.1.3/wm_topicgpt.egg-info/SOURCES.txt` & `wm_topicgpt-0.1.4/wm_topicgpt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

