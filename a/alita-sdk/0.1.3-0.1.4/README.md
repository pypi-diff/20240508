# Comparing `tmp/alita_sdk-0.1.3.tar.gz` & `tmp/alita_sdk-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alita_sdk-0.1.3.tar", last modified: Thu May  2 10:28:55 2024, max compression
+gzip compressed data, was "alita_sdk-0.1.4.tar", last modified: Wed May  8 14:04:53 2024, max compression
```

## Comparing `alita_sdk-0.1.3.tar` & `alita_sdk-0.1.4.tar`

### file list

```diff
@@ -1,41 +1,43 @@
-drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-05-02 10:28:55.933297 alita_sdk-0.1.3/
--rw-r--r--   0 arozumenko   (501) staff       (20)    11357 2024-03-08 11:24:37.000000 alita_sdk-0.1.3/LICENSE
--rw-r--r--   0 arozumenko   (501) staff       (20)     4063 2024-05-02 10:28:55.932967 alita_sdk-0.1.3/PKG-INFO
--rw-r--r--   0 arozumenko   (501) staff       (20)     3200 2024-03-10 12:01:09.000000 alita_sdk-0.1.3/README.md
--rw-r--r--   0 arozumenko   (501) staff       (20)      705 2024-05-02 10:28:50.000000 alita_sdk-0.1.3/pyproject.toml
--rw-r--r--   0 arozumenko   (501) staff       (20)      175 2024-04-30 17:55:06.000000 alita_sdk-0.1.3/requirements.txt
--rw-r--r--   0 arozumenko   (501) staff       (20)       38 2024-05-02 10:28:55.933351 alita_sdk-0.1.3/setup.cfg
-drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-05-02 10:28:55.928022 alita_sdk-0.1.3/src/
--rw-r--r--   0 arozumenko   (501) staff       (20)        0 2024-03-08 11:25:38.000000 alita_sdk-0.1.3/src/__init__.py
-drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-05-02 10:28:55.928123 alita_sdk-0.1.3/src/alita_sdk/
--rw-r--r--   0 arozumenko   (501) staff       (20)        0 2024-03-08 11:25:50.000000 alita_sdk-0.1.3/src/alita_sdk/__init__.py
-drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-05-02 10:28:55.929469 alita_sdk-0.1.3/src/alita_sdk/agents/
--rw-r--r--   0 arozumenko   (501) staff       (20)     2412 2024-03-18 10:31:52.000000 alita_sdk-0.1.3/src/alita_sdk/agents/__init__.py
--rw-r--r--   0 arozumenko   (501) staff       (20)     3122 2024-04-30 17:52:10.000000 alita_sdk-0.1.3/src/alita_sdk/agents/alita_openai.py
--rw-r--r--   0 arozumenko   (501) staff       (20)        0 2024-03-10 11:28:03.000000 alita_sdk-0.1.3/src/alita_sdk/agents/base_actions.py
--rw-r--r--   0 arozumenko   (501) staff       (20)     3095 2024-04-30 17:52:10.000000 alita_sdk-0.1.3/src/alita_sdk/agents/mixedAgentParser.py
--rw-r--r--   0 arozumenko   (501) staff       (20)     2283 2024-03-18 10:31:02.000000 alita_sdk-0.1.3/src/alita_sdk/agents/mixedAgentRenderes.py
--rw-r--r--   0 arozumenko   (501) staff       (20)     1169 2024-04-30 17:52:10.000000 alita_sdk-0.1.3/src/alita_sdk/agents/utils.py
-drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-05-02 10:28:55.929710 alita_sdk-0.1.3/src/alita_sdk/clients/
--rw-r--r--   0 arozumenko   (501) staff       (20)       31 2024-03-09 15:53:40.000000 alita_sdk-0.1.3/src/alita_sdk/clients/__init__.py
--rw-r--r--   0 arozumenko   (501) staff       (20)    20661 2024-05-01 13:48:52.000000 alita_sdk-0.1.3/src/alita_sdk/clients/client.py
-drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-05-02 10:28:55.930396 alita_sdk-0.1.3/src/alita_sdk/llms/
--rw-r--r--   0 arozumenko   (501) staff       (20)       33 2024-03-09 14:45:23.000000 alita_sdk-0.1.3/src/alita_sdk/llms/__init__.py
--rw-r--r--   0 arozumenko   (501) staff       (20)     8851 2024-05-02 10:28:32.000000 alita_sdk-0.1.3/src/alita_sdk/llms/alita.py
-drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-05-02 10:28:55.930912 alita_sdk-0.1.3/src/alita_sdk/toolkits/
--rw-r--r--   0 arozumenko   (501) staff       (20)        0 2024-04-12 11:47:05.000000 alita_sdk-0.1.3/src/alita_sdk/toolkits/__init__.py
--rw-r--r--   0 arozumenko   (501) staff       (20)     1985 2024-04-12 12:00:03.000000 alita_sdk-0.1.3/src/alita_sdk/toolkits/datasource.py
--rw-r--r--   0 arozumenko   (501) staff       (20)      734 2024-04-12 11:47:16.000000 alita_sdk-0.1.3/src/alita_sdk/toolkits/prompt.py
-drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-05-02 10:28:55.931385 alita_sdk-0.1.3/src/alita_sdk/tools/
--rw-r--r--   0 arozumenko   (501) staff       (20)        0 2024-03-11 07:45:42.000000 alita_sdk-0.1.3/src/alita_sdk/tools/__init__.py
--rw-r--r--   0 arozumenko   (501) staff       (20)      743 2024-04-12 14:28:55.000000 alita_sdk-0.1.3/src/alita_sdk/tools/datasource.py
--rw-r--r--   0 arozumenko   (501) staff       (20)      281 2024-04-12 14:28:45.000000 alita_sdk-0.1.3/src/alita_sdk/tools/prompt.py
-drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-05-02 10:28:55.931726 alita_sdk-0.1.3/src/alita_sdk/utils/
--rw-r--r--   0 arozumenko   (501) staff       (20)        0 2024-03-13 15:14:37.000000 alita_sdk-0.1.3/src/alita_sdk/utils/__init__.py
--rw-r--r--   0 arozumenko   (501) staff       (20)    10148 2024-04-04 04:14:44.000000 alita_sdk-0.1.3/src/alita_sdk/utils/streamlit.py
-drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-05-02 10:28:55.932455 alita_sdk-0.1.3/src/alita_sdk.egg-info/
--rw-r--r--   0 arozumenko   (501) staff       (20)     4063 2024-05-02 10:28:55.000000 alita_sdk-0.1.3/src/alita_sdk.egg-info/PKG-INFO
--rw-r--r--   0 arozumenko   (501) staff       (20)      887 2024-05-02 10:28:55.000000 alita_sdk-0.1.3/src/alita_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 arozumenko   (501) staff       (20)        1 2024-05-02 10:28:55.000000 alita_sdk-0.1.3/src/alita_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 arozumenko   (501) staff       (20)      176 2024-05-02 10:28:55.000000 alita_sdk-0.1.3/src/alita_sdk.egg-info/requires.txt
--rw-r--r--   0 arozumenko   (501) staff       (20)       19 2024-05-02 10:28:55.000000 alita_sdk-0.1.3/src/alita_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-05-08 14:04:53.031705 alita_sdk-0.1.4/
+-rw-r--r--   0 arozumenko   (501) staff       (20)    11357 2024-03-08 11:24:37.000000 alita_sdk-0.1.4/LICENSE
+-rw-r--r--   0 arozumenko   (501) staff       (20)     4063 2024-05-08 14:04:53.030514 alita_sdk-0.1.4/PKG-INFO
+-rw-r--r--   0 arozumenko   (501) staff       (20)     3200 2024-03-10 12:01:09.000000 alita_sdk-0.1.4/README.md
+-rw-r--r--   0 arozumenko   (501) staff       (20)      705 2024-05-08 14:04:47.000000 alita_sdk-0.1.4/pyproject.toml
+-rw-r--r--   0 arozumenko   (501) staff       (20)      175 2024-05-08 13:44:16.000000 alita_sdk-0.1.4/requirements.txt
+-rw-r--r--   0 arozumenko   (501) staff       (20)       38 2024-05-08 14:04:53.031885 alita_sdk-0.1.4/setup.cfg
+drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-05-08 14:04:53.012296 alita_sdk-0.1.4/src/
+-rw-r--r--   0 arozumenko   (501) staff       (20)        0 2024-03-08 11:25:38.000000 alita_sdk-0.1.4/src/__init__.py
+drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-05-08 14:04:53.012652 alita_sdk-0.1.4/src/alita_sdk/
+-rw-r--r--   0 arozumenko   (501) staff       (20)        0 2024-03-08 11:25:50.000000 alita_sdk-0.1.4/src/alita_sdk/__init__.py
+drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-05-08 14:04:53.020284 alita_sdk-0.1.4/src/alita_sdk/agents/
+-rw-r--r--   0 arozumenko   (501) staff       (20)     2412 2024-03-18 10:31:52.000000 alita_sdk-0.1.4/src/alita_sdk/agents/__init__.py
+-rw-r--r--   0 arozumenko   (501) staff       (20)     3122 2024-04-30 17:52:10.000000 alita_sdk-0.1.4/src/alita_sdk/agents/alita_openai.py
+-rw-r--r--   0 arozumenko   (501) staff       (20)        0 2024-03-10 11:28:03.000000 alita_sdk-0.1.4/src/alita_sdk/agents/base_actions.py
+-rw-r--r--   0 arozumenko   (501) staff       (20)     3095 2024-04-30 17:52:10.000000 alita_sdk-0.1.4/src/alita_sdk/agents/mixedAgentParser.py
+-rw-r--r--   0 arozumenko   (501) staff       (20)     2283 2024-03-18 10:31:02.000000 alita_sdk-0.1.4/src/alita_sdk/agents/mixedAgentRenderes.py
+-rw-r--r--   0 arozumenko   (501) staff       (20)     1169 2024-04-30 17:52:10.000000 alita_sdk-0.1.4/src/alita_sdk/agents/utils.py
+drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-05-08 14:04:53.021612 alita_sdk-0.1.4/src/alita_sdk/clients/
+-rw-r--r--   0 arozumenko   (501) staff       (20)       31 2024-03-09 15:53:40.000000 alita_sdk-0.1.4/src/alita_sdk/clients/__init__.py
+-rw-r--r--   0 arozumenko   (501) staff       (20)    21757 2024-05-08 13:31:09.000000 alita_sdk-0.1.4/src/alita_sdk/clients/client.py
+drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-05-08 14:04:53.023862 alita_sdk-0.1.4/src/alita_sdk/llms/
+-rw-r--r--   0 arozumenko   (501) staff       (20)       33 2024-03-09 14:45:23.000000 alita_sdk-0.1.4/src/alita_sdk/llms/__init__.py
+-rw-r--r--   0 arozumenko   (501) staff       (20)     8851 2024-05-02 10:28:32.000000 alita_sdk-0.1.4/src/alita_sdk/llms/alita.py
+drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-05-08 14:04:53.026216 alita_sdk-0.1.4/src/alita_sdk/toolkits/
+-rw-r--r--   0 arozumenko   (501) staff       (20)        0 2024-04-12 11:47:05.000000 alita_sdk-0.1.4/src/alita_sdk/toolkits/__init__.py
+-rw-r--r--   0 arozumenko   (501) staff       (20)      798 2024-05-08 13:59:31.000000 alita_sdk-0.1.4/src/alita_sdk/toolkits/application.py
+-rw-r--r--   0 arozumenko   (501) staff       (20)     1985 2024-04-12 12:00:03.000000 alita_sdk-0.1.4/src/alita_sdk/toolkits/datasource.py
+-rw-r--r--   0 arozumenko   (501) staff       (20)      734 2024-04-12 11:47:16.000000 alita_sdk-0.1.4/src/alita_sdk/toolkits/prompt.py
+drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-05-08 14:04:53.027931 alita_sdk-0.1.4/src/alita_sdk/tools/
+-rw-r--r--   0 arozumenko   (501) staff       (20)        0 2024-03-11 07:45:42.000000 alita_sdk-0.1.4/src/alita_sdk/tools/__init__.py
+-rw-r--r--   0 arozumenko   (501) staff       (20)      530 2024-05-08 13:59:34.000000 alita_sdk-0.1.4/src/alita_sdk/tools/application.py
+-rw-r--r--   0 arozumenko   (501) staff       (20)      743 2024-04-12 14:28:55.000000 alita_sdk-0.1.4/src/alita_sdk/tools/datasource.py
+-rw-r--r--   0 arozumenko   (501) staff       (20)      281 2024-04-12 14:28:45.000000 alita_sdk-0.1.4/src/alita_sdk/tools/prompt.py
+drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-05-08 14:04:53.028864 alita_sdk-0.1.4/src/alita_sdk/utils/
+-rw-r--r--   0 arozumenko   (501) staff       (20)        0 2024-03-13 15:14:37.000000 alita_sdk-0.1.4/src/alita_sdk/utils/__init__.py
+-rw-r--r--   0 arozumenko   (501) staff       (20)    10148 2024-04-04 04:14:44.000000 alita_sdk-0.1.4/src/alita_sdk/utils/streamlit.py
+drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-05-08 14:04:53.029564 alita_sdk-0.1.4/src/alita_sdk.egg-info/
+-rw-r--r--   0 arozumenko   (501) staff       (20)     4063 2024-05-08 14:04:52.000000 alita_sdk-0.1.4/src/alita_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 arozumenko   (501) staff       (20)      960 2024-05-08 14:04:53.000000 alita_sdk-0.1.4/src/alita_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 arozumenko   (501) staff       (20)        1 2024-05-08 14:04:52.000000 alita_sdk-0.1.4/src/alita_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 arozumenko   (501) staff       (20)      176 2024-05-08 14:04:52.000000 alita_sdk-0.1.4/src/alita_sdk.egg-info/requires.txt
+-rw-r--r--   0 arozumenko   (501) staff       (20)       19 2024-05-08 14:04:52.000000 alita_sdk-0.1.4/src/alita_sdk.egg-info/top_level.txt
```

### Comparing `alita_sdk-0.1.3/LICENSE` & `alita_sdk-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `alita_sdk-0.1.3/PKG-INFO` & `alita_sdk-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alita_sdk
-Version: 0.1.3
+Version: 0.1.4
 Summary: SDK for building langchain agents using resouces from Alita
 Author-email: Artem Rozumenko <support@analysta.ai>
 Project-URL: Homepage, https://projectalita.ai
 Project-URL: Issues, https://github.com/ProjectAlita/alita-sdk/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -12,15 +12,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: langchain_core~=0.1.30
 Requires-Dist: langchain~=0.1.12
 Requires-Dist: tiktoken~=0.6.0
 Requires-Dist: openai==1.13.3
 Requires-Dist: python-dotenv~=1.0.1
-Requires-Dist: alita_tools>=0.0.10
+Requires-Dist: alita_tools>=0.0.11
 Requires-Dist: jinja2~=3.1.3
 Requires-Dist: pillow~=10.2.0
 Requires-Dist: requests~=2.31.0
 Requires-Dist: pydantic~=1.10.9
 
 Alita SDK
 =========
```

### Comparing `alita_sdk-0.1.3/README.md` & `alita_sdk-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `alita_sdk-0.1.3/pyproject.toml` & `alita_sdk-0.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "alita_sdk"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
   { name="Artem Rozumenko", email="support@analysta.ai" },
 ]
 description = "SDK for building langchain agents using resouces from Alita"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `alita_sdk-0.1.3/src/alita_sdk/agents/__init__.py` & `alita_sdk-0.1.4/src/alita_sdk/agents/__init__.py`

 * *Files identical despite different names*

### Comparing `alita_sdk-0.1.3/src/alita_sdk/agents/alita_openai.py` & `alita_sdk-0.1.4/src/alita_sdk/agents/alita_openai.py`

 * *Files identical despite different names*

### Comparing `alita_sdk-0.1.3/src/alita_sdk/agents/mixedAgentParser.py` & `alita_sdk-0.1.4/src/alita_sdk/agents/mixedAgentParser.py`

 * *Files identical despite different names*

### Comparing `alita_sdk-0.1.3/src/alita_sdk/agents/mixedAgentRenderes.py` & `alita_sdk-0.1.4/src/alita_sdk/agents/mixedAgentRenderes.py`

 * *Files identical despite different names*

### Comparing `alita_sdk-0.1.3/src/alita_sdk/agents/utils.py` & `alita_sdk-0.1.4/src/alita_sdk/agents/utils.py`

 * *Files identical despite different names*

### Comparing `alita_sdk-0.1.3/src/alita_sdk/clients/client.py` & `alita_sdk-0.1.4/src/alita_sdk/clients/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,18 +16,20 @@
 from langchain.agents import AgentExecutor
 from langchain_core.utils.function_calling import convert_to_openai_function
 
 from ..agents import create_mixed_agent
 from ..agents.alita_openai import AlitaAssistantRunnable
 from ..toolkits.prompt import PromptToolkit
 from ..toolkits.datasource import DatasourcesToolkit
+from ..toolkits.application import ApplicationToolkit
 from alita_tools.github import AlitaGitHubToolkit
 from alita_tools.openapi import AlitaOpenAPIToolkit
 from alita_tools.jira import JiraToolkit
 from alita_tools.confluence import ConfluenceToolkit
+from alita_tools.browser import BrowserToolkit
 from pydantic import create_model
 
 logger = logging.getLogger(__name__)
 
 
 class Jinja2TemplatedChatMessagesTemplate(ChatPromptTemplate):
 
@@ -163,14 +165,15 @@
         }
         self.predict_url = f"{self.base_url}{self.api_path}/prompt_lib/predict/prompt_lib/{self.project_id}"
         self.prompt_versions = f"{self.base_url}{self.api_path}/prompt_lib/version/prompt_lib/{self.project_id}"
         self.prompts = f"{self.base_url}{self.api_path}/prompt_lib/prompt/prompt_lib/{self.project_id}"
         self.datasources = f"{self.base_url}{self.api_path}/datasources/datasource/prompt_lib/{self.project_id}"
         self.datasources_predict = f"{self.base_url}{self.api_path}/datasources/predict/prompt_lib/{self.project_id}"
         self.datasources_search = f"{self.base_url}{self.api_path}/datasources/search/prompt_lib/{self.project_id}"
+        self.app = f"{self.base_url}{self.api_path}/applications/application/prompt_lib/{self.project_id}"
         self.application_versions = f"{self.base_url}{self.api_path}/applications/version/prompt_lib/{self.project_id}"
 
     def prompt(self, prompt_id, prompt_version_id, chat_history=None, return_tool=False):
         url = f"{self.prompt_versions}/{prompt_id}/{prompt_version_id}"
         data = requests.get(url, headers=self.headers).json()
         model_settings = data['model_settings']
         messages = [SystemMessage(content=data['context'])]
@@ -199,14 +202,19 @@
         if not return_tool:
             return template
         else:
             url = f"{self.prompts}/{prompt_id}"
             data = requests.get(url, headers=self.headers).json()
             return AlitaPrompt(self, template, data['name'], data['description'], model_settings)
 
+    def get_app_details(self, application_id: int):
+        url = f"{self.app}/{application_id}"
+        data = requests.get(url, headers=self.headers).json()
+        return data
+        
     def application(self, client: Any, application_id: int, application_version_id: int, tools: Optional[list] = None):
         if tools is None:
             tools = []
         url = f"{self.application_versions}/{application_id}/{application_version_id}"
         data = requests.get(url, headers=self.headers).json()
         messages = [SystemMessage(content=data['instructions'])]
         variables = {}
@@ -235,14 +243,21 @@
                 ])
             elif tool['type'] == 'datasource':
                 tools.extend(DatasourcesToolkit.get_toolkit(
                     self,
                     datasource_ids=[int(tool['settings']['datasource_id'])],
                     selected_tools=tool['settings']['selected_tools']
                 ).get_tools())
+            elif tool['type'] == 'application':
+                tools.extend(ApplicationToolkit.get_toolkit(
+                    self,
+                    application_id=int(tool['settings']['application_id']),
+                    application_version_id=int(tool['settings']['application_version_id']),
+                    selected_tools=[]
+                ).get_tools())
             elif tool['type'] == 'openapi':
                 headers = {}
                 if tool['settings'].get('authentication'):
                     if tool['settings']['authentication']['type'] == 'api_key':
                         auth_type = tool['settings']['authentication']['settings']['auth_type']
                         auth_key = tool["settings"]["authentication"]["settings"]["api_key"]
                         if auth_type.lower() == 'bearer':
@@ -286,14 +301,20 @@
                     api_key=tool['settings'].get('api_key', None),
                     username=tool['settings'].get('username', None),
                     token=tool['settings'].get('token', None),
                     limit=tool['settings'].get('limit', 5),
                     additional_fields=tool['settings'].get('additional_fields', []),
                     verify_ssl=tool['settings'].get('verify_ssl', True))
                 tools.extend(confluence_tools.get_tools())
+            elif tool['type'] == 'browser':
+                browser_tools = BrowserToolkit().get_toolkit(
+                    google_api_key=tool['settings'].get('google_api_key'), 
+                    google_cse_id=tool['settings'].get("google_cse_id")
+                )
+                tools.extend(browser_tools.get_tools())
             else:
                 if tool.get("module"):
                     try:
                         mod = import_module(tool.get("module"))
                         tkitclass = getattr(mod, tool.get("class"))
                         toolkit = tkitclass.get_toolkit(**tool["settings"])
                         tools.extend(toolkit.get_tools())
```

### Comparing `alita_sdk-0.1.3/src/alita_sdk/llms/alita.py` & `alita_sdk-0.1.4/src/alita_sdk/llms/alita.py`

 * *Files identical despite different names*

### Comparing `alita_sdk-0.1.3/src/alita_sdk/toolkits/datasource.py` & `alita_sdk-0.1.4/src/alita_sdk/toolkits/datasource.py`

 * *Files identical despite different names*

### Comparing `alita_sdk-0.1.3/src/alita_sdk/toolkits/prompt.py` & `alita_sdk-0.1.4/src/alita_sdk/toolkits/prompt.py`

 * *Files identical despite different names*

### Comparing `alita_sdk-0.1.3/src/alita_sdk/tools/datasource.py` & `alita_sdk-0.1.4/src/alita_sdk/tools/datasource.py`

 * *Files identical despite different names*

### Comparing `alita_sdk-0.1.3/src/alita_sdk/utils/streamlit.py` & `alita_sdk-0.1.4/src/alita_sdk/utils/streamlit.py`

 * *Files identical despite different names*

### Comparing `alita_sdk-0.1.3/src/alita_sdk.egg-info/PKG-INFO` & `alita_sdk-0.1.4/src/alita_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alita_sdk
-Version: 0.1.3
+Version: 0.1.4
 Summary: SDK for building langchain agents using resouces from Alita
 Author-email: Artem Rozumenko <support@analysta.ai>
 Project-URL: Homepage, https://projectalita.ai
 Project-URL: Issues, https://github.com/ProjectAlita/alita-sdk/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -12,15 +12,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: langchain_core~=0.1.30
 Requires-Dist: langchain~=0.1.12
 Requires-Dist: tiktoken~=0.6.0
 Requires-Dist: openai==1.13.3
 Requires-Dist: python-dotenv~=1.0.1
-Requires-Dist: alita_tools>=0.0.10
+Requires-Dist: alita_tools>=0.0.11
 Requires-Dist: jinja2~=3.1.3
 Requires-Dist: pillow~=10.2.0
 Requires-Dist: requests~=2.31.0
 Requires-Dist: pydantic~=1.10.9
 
 Alita SDK
 =========
```

### Comparing `alita_sdk-0.1.3/src/alita_sdk.egg-info/SOURCES.txt` & `alita_sdk-0.1.4/src/alita_sdk.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 src/alita_sdk/agents/mixedAgentRenderes.py
 src/alita_sdk/agents/utils.py
 src/alita_sdk/clients/__init__.py
 src/alita_sdk/clients/client.py
 src/alita_sdk/llms/__init__.py
 src/alita_sdk/llms/alita.py
 src/alita_sdk/toolkits/__init__.py
+src/alita_sdk/toolkits/application.py
 src/alita_sdk/toolkits/datasource.py
 src/alita_sdk/toolkits/prompt.py
 src/alita_sdk/tools/__init__.py
+src/alita_sdk/tools/application.py
 src/alita_sdk/tools/datasource.py
 src/alita_sdk/tools/prompt.py
 src/alita_sdk/utils/__init__.py
 src/alita_sdk/utils/streamlit.py
```

