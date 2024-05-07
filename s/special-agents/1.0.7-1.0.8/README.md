# Comparing `tmp/special_agents-1.0.7.tar.gz` & `tmp/special_agents-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "special_agents-1.0.7.tar", last modified: Tue May  7 22:26:26 2024, max compression
+gzip compressed data, was "special_agents-1.0.8.tar", last modified: Tue May  7 22:42:05 2024, max compression
```

## Comparing `special_agents-1.0.7.tar` & `special_agents-1.0.8.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 22:26:26.837930 special_agents-1.0.7/
--rw-rw-rw-   0        0        0     4307 2024-05-07 11:00:25.000000 special_agents-1.0.7/CONTRIBUTING.md
--rw-rw-rw-   0        0        0     1065 2024-05-06 10:26:56.000000 special_agents-1.0.7/LICENSE
--rw-rw-rw-   0        0        0       47 2024-05-06 13:58:26.000000 special_agents-1.0.7/MANIFEST.in
--rw-rw-rw-   0        0        0     8185 2024-05-07 22:26:26.837930 special_agents-1.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     7441 2024-05-07 22:22:28.000000 special_agents-1.0.7/README.md
--rw-rw-rw-   0        0        0       14 2024-05-07 11:14:15.000000 special_agents-1.0.7/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-05-07 22:26:26.837930 special_agents-1.0.7/setup.cfg
--rw-rw-rw-   0        0        0      939 2024-05-07 22:25:39.000000 special_agents-1.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-07 22:26:26.731569 special_agents-1.0.7/src/
-drwxrwxrwx   0        0        0        0 2024-05-07 22:26:26.785876 special_agents-1.0.7/src/special_agents/
--rw-rw-rw-   0        0        0     1563 2024-05-07 22:23:13.000000 special_agents-1.0.7/src/special_agents/Agent.py
--rw-rw-rw-   0        0        0       85 2024-05-07 19:55:13.000000 special_agents-1.0.7/src/special_agents/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-07 22:26:26.837930 special_agents-1.0.7/src/special_agents/agents/
--rw-rw-rw-   0        0        0     5103 2024-05-07 19:55:13.000000 special_agents-1.0.7/src/special_agents/agents/ContentCreator.py
--rw-rw-rw-   0        0        0     4149 2024-05-07 19:55:13.000000 special_agents-1.0.7/src/special_agents/agents/FullStackDeveloper.py
--rw-rw-rw-   0        0        0     5938 2024-05-07 19:55:13.000000 special_agents-1.0.7/src/special_agents/agents/ProductManager.py
--rw-rw-rw-   0        0        0       95 2024-05-07 11:09:17.000000 special_agents-1.0.7/src/special_agents/agents/__init__.py
--rw-rw-rw-   0        0        0      310 2024-05-06 21:25:26.000000 special_agents-1.0.7/src/special_agents/config.py
--rw-rw-rw-   0        0        0     4330 2024-05-07 19:55:13.000000 special_agents-1.0.7/src/special_agents/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-07 22:26:26.837930 special_agents-1.0.7/src/special_agents.egg-info/
--rw-rw-rw-   0        0        0     8185 2024-05-07 22:26:26.000000 special_agents-1.0.7/src/special_agents.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      570 2024-05-07 22:26:26.000000 special_agents-1.0.7/src/special_agents.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 22:26:26.000000 special_agents-1.0.7/src/special_agents.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-05-07 22:26:26.000000 special_agents-1.0.7/src/special_agents.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-05-07 22:26:26.000000 special_agents-1.0.7/src/special_agents.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-07 22:42:05.665403 special_agents-1.0.8/
+-rw-rw-rw-   0        0        0     4307 2024-05-07 11:00:25.000000 special_agents-1.0.8/CONTRIBUTING.md
+-rw-rw-rw-   0        0        0     1065 2024-05-06 10:26:56.000000 special_agents-1.0.8/LICENSE
+-rw-rw-rw-   0        0        0       47 2024-05-06 13:58:26.000000 special_agents-1.0.8/MANIFEST.in
+-rw-rw-rw-   0        0        0     8185 2024-05-07 22:42:05.662628 special_agents-1.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     7441 2024-05-07 22:22:28.000000 special_agents-1.0.8/README.md
+-rw-rw-rw-   0        0        0       14 2024-05-07 11:14:15.000000 special_agents-1.0.8/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-07 22:42:05.665403 special_agents-1.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      939 2024-05-07 22:41:53.000000 special_agents-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 22:42:05.571579 special_agents-1.0.8/src/
+drwxrwxrwx   0        0        0        0 2024-05-07 22:42:05.616264 special_agents-1.0.8/src/special_agents/
+-rw-rw-rw-   0        0        0     1563 2024-05-07 22:23:13.000000 special_agents-1.0.8/src/special_agents/Agent.py
+-rw-rw-rw-   0        0        0       85 2024-05-07 19:55:13.000000 special_agents-1.0.8/src/special_agents/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-07 22:42:05.657614 special_agents-1.0.8/src/special_agents/agents/
+-rw-rw-rw-   0        0        0     5103 2024-05-07 19:55:13.000000 special_agents-1.0.8/src/special_agents/agents/ContentCreator.py
+-rw-rw-rw-   0        0        0     4149 2024-05-07 19:55:13.000000 special_agents-1.0.8/src/special_agents/agents/FullStackDeveloper.py
+-rw-rw-rw-   0        0        0     5938 2024-05-07 19:55:13.000000 special_agents-1.0.8/src/special_agents/agents/ProductManager.py
+-rw-rw-rw-   0        0        0       95 2024-05-07 11:09:17.000000 special_agents-1.0.8/src/special_agents/agents/__init__.py
+-rw-rw-rw-   0        0        0      310 2024-05-06 21:25:26.000000 special_agents-1.0.8/src/special_agents/config.py
+-rw-rw-rw-   0        0        0     4699 2024-05-07 22:41:37.000000 special_agents-1.0.8/src/special_agents/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-07 22:42:05.660624 special_agents-1.0.8/src/special_agents.egg-info/
+-rw-rw-rw-   0        0        0     8185 2024-05-07 22:42:05.000000 special_agents-1.0.8/src/special_agents.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      570 2024-05-07 22:42:05.000000 special_agents-1.0.8/src/special_agents.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 22:42:05.000000 special_agents-1.0.8/src/special_agents.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-05-07 22:42:05.000000 special_agents-1.0.8/src/special_agents.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-05-07 22:42:05.000000 special_agents-1.0.8/src/special_agents.egg-info/top_level.txt
```

### Comparing `special_agents-1.0.7/CONTRIBUTING.md` & `special_agents-1.0.8/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `special_agents-1.0.7/LICENSE` & `special_agents-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `special_agents-1.0.7/PKG-INFO` & `special_agents-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: special-agents
-Version: 1.0.7
+Version: 1.0.8
 Summary: An Open-source Library for pre-defined LLM powered specialized agents
 Home-page: https://github.com/IhabTag/special-agents
 Author: Ihab Tag
 Author-email: contact@ihabtag.com
 License: MIT license
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `special_agents-1.0.7/README.md` & `special_agents-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `special_agents-1.0.7/setup.py` & `special_agents-1.0.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     
 with open("requirements.txt", "r", encoding="utf-8") as f:
     req = f.readlines()
 req = [x.strip() for x in req if x.strip()]
 
 setup(
     name="special-agents", 
-    version="1.0.7",
+    version="1.0.8",
     author="Ihab Tag",
     author_email="contact@ihabtag.com",
     description="An Open-source Library for pre-defined LLM powered specialized agents",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/IhabTag/special-agents",
     classifiers=[
```

### Comparing `special_agents-1.0.7/src/special_agents/Agent.py` & `special_agents-1.0.8/src/special_agents/Agent.py`

 * *Files identical despite different names*

### Comparing `special_agents-1.0.7/src/special_agents/agents/ContentCreator.py` & `special_agents-1.0.8/src/special_agents/agents/ContentCreator.py`

 * *Files identical despite different names*

### Comparing `special_agents-1.0.7/src/special_agents/agents/FullStackDeveloper.py` & `special_agents-1.0.8/src/special_agents/agents/FullStackDeveloper.py`

 * *Files identical despite different names*

### Comparing `special_agents-1.0.7/src/special_agents/agents/ProductManager.py` & `special_agents-1.0.8/src/special_agents/agents/ProductManager.py`

 * *Files identical despite different names*

### Comparing `special_agents-1.0.7/src/special_agents/utils.py` & `special_agents-1.0.8/src/special_agents/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -68,32 +68,43 @@
             system_content = f"""
                 ROLE: You are a {role}. 
                 Your competencies are: {competencies}. 
                 Your capabilities are: {capabilities}. 
                 CONTEXT: {context}.
                 TASK: {task}.
                 INSTRUCTIONS:
-                - Answer in the {lang} language.
                 - Make your answer in a {tone} tone.
                 {extra_instructions}"""
         else:
             system_content = f"""
                 ROLE: You are a {role}. 
                 Your competencies are: {competencies}. 
                 Your capabilities are: {capabilities}. 
                 TASK: {task}
                 INSTRUCTIONS:
-                - Answer in the {lang} language.
                 - Make your answer in a {tone} tone.
                 {extra_instructions}"""
         
+        
         response = client.chat.completions.create(
             model = model,
             temperature = temperature,
             messages = [
                 {"role": "system", "content": system_content},
                 {"role": "user", "content": question}
             ]
         )
-        return response.choices[0].message.content
+        if lang == 'same':
+            return response.choices[0].message.content
+        else:
+            translated_response = client.chat.completions.create(
+            model = model,
+            temperature = temperature,
+            messages = [
+                {"role": "system", "content": f'You are a translator, translate the following into the {lang} language'},
+                {"role": "user", "content": response}
+            ]
+            )
+            return translated_response
+            
     except Exception as err:
         return(f"Unexpected {err=}, {type(err)=}")
```

### Comparing `special_agents-1.0.7/src/special_agents.egg-info/PKG-INFO` & `special_agents-1.0.8/src/special_agents.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: special-agents
-Version: 1.0.7
+Version: 1.0.8
 Summary: An Open-source Library for pre-defined LLM powered specialized agents
 Home-page: https://github.com/IhabTag/special-agents
 Author: Ihab Tag
 Author-email: contact@ihabtag.com
 License: MIT license
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `special_agents-1.0.7/src/special_agents.egg-info/SOURCES.txt` & `special_agents-1.0.8/src/special_agents.egg-info/SOURCES.txt`

 * *Files identical despite different names*

