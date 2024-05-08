# Comparing `tmp/nonebot_plugin_with_ai_agents-0.1.6.tar.gz` & `tmp/nonebot_plugin_with_ai_agents-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_with_ai_agents-0.1.6.tar", max compression
+gzip compressed data, was "nonebot_plugin_with_ai_agents-0.1.7.tar", max compression
```

## Comparing `nonebot_plugin_with_ai_agents-0.1.6.tar` & `nonebot_plugin_with_ai_agents-0.1.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0      510 2024-05-08 08:28:49.886180 nonebot_plugin_with_ai_agents-0.1.6/nonebot_plugin_with_ai_agents/__init__.py
--rw-r--r--   0        0        0      439 2024-05-08 09:38:16.947093 nonebot_plugin_with_ai_agents-0.1.6/nonebot_plugin_with_ai_agents/handler.py
--rw-r--r--   0        0        0        2 2024-05-06 07:05:33.777069 nonebot_plugin_with_ai_agents-0.1.6/nonebot_plugin_with_ai_agents/llm/__init__.py
--rw-r--r--   0        0        0     4529 2024-05-08 09:00:09.567226 nonebot_plugin_with_ai_agents-0.1.6/nonebot_plugin_with_ai_agents/llm/agents.py
--rw-r--r--   0        0        0     3001 2024-05-08 09:00:09.568229 nonebot_plugin_with_ai_agents-0.1.6/nonebot_plugin_with_ai_agents/llm/central_brain.py
--rw-r--r--   0        0        0      849 2024-05-08 09:00:09.568229 nonebot_plugin_with_ai_agents-0.1.6/nonebot_plugin_with_ai_agents/llm/config.py
--rw-r--r--   0        0        0      131 2024-05-06 07:05:33.778077 nonebot_plugin_with_ai_agents-0.1.6/nonebot_plugin_with_ai_agents/llm/llms/__init__.py
--rw-r--r--   0        0        0      453 2024-05-07 11:12:58.483693 nonebot_plugin_with_ai_agents-0.1.6/nonebot_plugin_with_ai_agents/llm/llms/base.py
--rw-r--r--   0        0        0     2277 2024-05-07 11:13:28.157800 nonebot_plugin_with_ai_agents-0.1.6/nonebot_plugin_with_ai_agents/llm/llms/dashscope.py
--rw-r--r--   0        0        0     1942 2024-05-07 11:13:28.219069 nonebot_plugin_with_ai_agents-0.1.6/nonebot_plugin_with_ai_agents/llm/llms/glm.py
--rw-r--r--   0        0        0     2046 2024-05-07 11:13:28.141789 nonebot_plugin_with_ai_agents-0.1.6/nonebot_plugin_with_ai_agents/llm/llms/openai.py
--rw-r--r--   0        0        0       19 2024-05-06 07:05:33.780198 nonebot_plugin_with_ai_agents-0.1.6/nonebot_plugin_with_ai_agents/llm/mem_stores.py
--rw-r--r--   0        0        0      338 2024-05-07 08:06:18.016313 nonebot_plugin_with_ai_agents-0.1.6/nonebot_plugin_with_ai_agents/llm/services.py
--rw-r--r--   0        0        0        0 2024-05-06 07:05:33.780198 nonebot_plugin_with_ai_agents-0.1.6/nonebot_plugin_with_ai_agents/llm/utils/__init__.py
--rw-r--r--   0        0        0     4648 2024-05-06 07:05:33.780198 nonebot_plugin_with_ai_agents-0.1.6/nonebot_plugin_with_ai_agents/llm/utils/prompts.py
--rw-r--r--   0        0        0     3358 2024-05-07 10:03:19.714495 nonebot_plugin_with_ai_agents-0.1.6/nonebot_plugin_with_ai_agents/llm/utils/retrievers.py
--rw-r--r--   0        0        0      694 2024-05-08 09:42:51.226092 nonebot_plugin_with_ai_agents-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     6811 2024-05-08 09:06:10.571877 nonebot_plugin_with_ai_agents-0.1.6/README.md
--rw-r--r--   0        0        0     7616 1970-01-01 00:00:00.000000 nonebot_plugin_with_ai_agents-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0      510 2024-05-08 08:28:49.886180 nonebot_plugin_with_ai_agents-0.1.7/nonebot_plugin_with_ai_agents/__init__.py
+-rw-r--r--   0        0        0      439 2024-05-08 09:38:16.947093 nonebot_plugin_with_ai_agents-0.1.7/nonebot_plugin_with_ai_agents/handler.py
+-rw-r--r--   0        0        0        2 2024-05-06 07:05:33.777069 nonebot_plugin_with_ai_agents-0.1.7/nonebot_plugin_with_ai_agents/llm/__init__.py
+-rw-r--r--   0        0        0     4529 2024-05-08 09:00:09.567226 nonebot_plugin_with_ai_agents-0.1.7/nonebot_plugin_with_ai_agents/llm/agents.py
+-rw-r--r--   0        0        0     3184 2024-05-08 09:53:49.782564 nonebot_plugin_with_ai_agents-0.1.7/nonebot_plugin_with_ai_agents/llm/central_brain.py
+-rw-r--r--   0        0        0     1083 2024-05-08 09:54:00.100650 nonebot_plugin_with_ai_agents-0.1.7/nonebot_plugin_with_ai_agents/llm/config.py
+-rw-r--r--   0        0        0      131 2024-05-06 07:05:33.778077 nonebot_plugin_with_ai_agents-0.1.7/nonebot_plugin_with_ai_agents/llm/llms/__init__.py
+-rw-r--r--   0        0        0      453 2024-05-07 11:12:58.483693 nonebot_plugin_with_ai_agents-0.1.7/nonebot_plugin_with_ai_agents/llm/llms/base.py
+-rw-r--r--   0        0        0     2277 2024-05-07 11:13:28.157800 nonebot_plugin_with_ai_agents-0.1.7/nonebot_plugin_with_ai_agents/llm/llms/dashscope.py
+-rw-r--r--   0        0        0     1942 2024-05-07 11:13:28.219069 nonebot_plugin_with_ai_agents-0.1.7/nonebot_plugin_with_ai_agents/llm/llms/glm.py
+-rw-r--r--   0        0        0     2046 2024-05-07 11:13:28.141789 nonebot_plugin_with_ai_agents-0.1.7/nonebot_plugin_with_ai_agents/llm/llms/openai.py
+-rw-r--r--   0        0        0       19 2024-05-06 07:05:33.780198 nonebot_plugin_with_ai_agents-0.1.7/nonebot_plugin_with_ai_agents/llm/mem_stores.py
+-rw-r--r--   0        0        0      338 2024-05-07 08:06:18.016313 nonebot_plugin_with_ai_agents-0.1.7/nonebot_plugin_with_ai_agents/llm/services.py
+-rw-r--r--   0        0        0        0 2024-05-06 07:05:33.780198 nonebot_plugin_with_ai_agents-0.1.7/nonebot_plugin_with_ai_agents/llm/utils/__init__.py
+-rw-r--r--   0        0        0     4648 2024-05-06 07:05:33.780198 nonebot_plugin_with_ai_agents-0.1.7/nonebot_plugin_with_ai_agents/llm/utils/prompts.py
+-rw-r--r--   0        0        0     3358 2024-05-07 10:03:19.714495 nonebot_plugin_with_ai_agents-0.1.7/nonebot_plugin_with_ai_agents/llm/utils/retrievers.py
+-rw-r--r--   0        0        0      694 2024-05-08 09:55:14.702971 nonebot_plugin_with_ai_agents-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     6811 2024-05-08 09:06:10.571877 nonebot_plugin_with_ai_agents-0.1.7/README.md
+-rw-r--r--   0        0        0     7616 1970-01-01 00:00:00.000000 nonebot_plugin_with_ai_agents-0.1.7/PKG-INFO
```

### Comparing `nonebot_plugin_with_ai_agents-0.1.6/nonebot_plugin_with_ai_agents/llm/agents.py` & `nonebot_plugin_with_ai_agents-0.1.7/nonebot_plugin_with_ai_agents/llm/agents.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_with_ai_agents-0.1.6/nonebot_plugin_with_ai_agents/llm/central_brain.py` & `nonebot_plugin_with_ai_agents-0.1.7/nonebot_plugin_with_ai_agents/llm/central_brain.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,19 +25,21 @@
         llm.model = model
 
     return llm
 
 
 async def ask_central_brain(raw_question: str):
     """向中心智脑提问"""
+    if not config:
+        return "WITH_AI_AGENTS 配置获取失败，请检查配置。配置文档参考：https://github.com/yejue/nonebot-plugin-with-ai-agents"
 
     # 选择智脑使用的大模型
     llm = get_llm_model(config.platform, config.api_key, config.model_name)
     if not llm:
-        return "大模型获取失败，请检查配置。配置文档参考：https://github.com/yejue/nonebot-plugin-with-ai-agents"
+        return "WITH_AI_AGENTS 大模型获取失败，请检查配置。配置文档参考：https://github.com/yejue/nonebot-plugin-with-ai-agents"
 
     # 获取聊天历史
     chat_history_list = ChatService.get_history_list()
 
     # 将用户提问发送到大模型分类器，获取分类列表
     prompt = prompts.get_classifier_prompt(question=raw_question)
     s = prompts.get_classifier_master_prompt()
```

### Comparing `nonebot_plugin_with_ai_agents-0.1.6/nonebot_plugin_with_ai_agents/llm/config.py` & `nonebot_plugin_with_ai_agents-0.1.7/nonebot_plugin_with_ai_agents/llm/config.py`

 * *Files 20% similar despite different names*

```diff
@@ -13,14 +13,21 @@
 
 
 class Config(BaseModel):
     """AI Agents"""
     with_ai_agents: ScopedConfig
 
 
-plugin_config = get_plugin_config(Config).with_ai_agents
-config = plugin_config
+def get_config():
+    try:
+        plugin_config = get_plugin_config(Config).with_ai_agents
+        print("With_AI_Agents: api_key=", plugin_config.api_key)
+        print("With_AI_Agents: platform=", plugin_config.platform)
+        print("With_AI_Agents: model_name=", plugin_config.model_name)
+        print("With_AI_Agents：tavily_api_key=", plugin_config.tavily_api_key)
+        return plugin_config
+    except Exception as e:
+        print(f"WITH_AI_AGENTS 配置获取失败 {e}")
+        return None
 
-print("With_AI_Agents: api_key=", config.api_key)
-print("With_AI_Agents: platform=", config.platform)
-print("With_AI_Agents: model_name=", config.model_name)
-print("With_AI_Agents：tavily_api_key=", config.tavily_api_key)
+
+config = get_config()
```

### Comparing `nonebot_plugin_with_ai_agents-0.1.6/nonebot_plugin_with_ai_agents/llm/llms/dashscope.py` & `nonebot_plugin_with_ai_agents-0.1.7/nonebot_plugin_with_ai_agents/llm/llms/dashscope.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_with_ai_agents-0.1.6/nonebot_plugin_with_ai_agents/llm/llms/glm.py` & `nonebot_plugin_with_ai_agents-0.1.7/nonebot_plugin_with_ai_agents/llm/llms/glm.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_with_ai_agents-0.1.6/nonebot_plugin_with_ai_agents/llm/llms/openai.py` & `nonebot_plugin_with_ai_agents-0.1.7/nonebot_plugin_with_ai_agents/llm/llms/openai.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_with_ai_agents-0.1.6/nonebot_plugin_with_ai_agents/llm/utils/prompts.py` & `nonebot_plugin_with_ai_agents-0.1.7/nonebot_plugin_with_ai_agents/llm/utils/prompts.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_with_ai_agents-0.1.6/nonebot_plugin_with_ai_agents/llm/utils/retrievers.py` & `nonebot_plugin_with_ai_agents-0.1.7/nonebot_plugin_with_ai_agents/llm/utils/retrievers.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_with_ai_agents-0.1.6/pyproject.toml` & `nonebot_plugin_with_ai_agents-0.1.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-with-ai-agents"
-version = "0.1.6"
+version = "0.1.7"
 description = "nonebot_plugin_with_ai_agents 是一个基于基本原理实现的 AI Agents（智能体），拥有联网搜索能力、页面内容提取并学习回答、命令执行等功能"
 authors = ["yejue <1145331931@qq.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 nonebot2 = "^2.0"
```

### Comparing `nonebot_plugin_with_ai_agents-0.1.6/README.md` & `nonebot_plugin_with_ai_agents-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_with_ai_agents-0.1.6/PKG-INFO` & `nonebot_plugin_with_ai_agents-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-with-ai-agents
-Version: 0.1.6
+Version: 0.1.7
 Summary: nonebot_plugin_with_ai_agents 是一个基于基本原理实现的 AI Agents（智能体），拥有联网搜索能力、页面内容提取并学习回答、命令执行等功能
 Author: yejue
 Author-email: 1145331931@qq.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-with-ai-agents Version: 0.1.6
+Metadata-Version: 2.1 Name: nonebot-plugin-with-ai-agents Version: 0.1.7
 Summary: nonebot_plugin_with_ai_agents æ¯ä¸ä¸ªåºäºåºæ¬åçå®ç°ç AI
 Agentsï¼æºè½ä½ï¼ï¼æ¥æèç½æç´¢è½åãé¡µé¢åå®¹æåå¹¶å­¦ä¹ åç­ãå½ä»¤æ§è¡ç­åè½
 Author: yejue Author-email: 1145331931@qq.com Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
```

