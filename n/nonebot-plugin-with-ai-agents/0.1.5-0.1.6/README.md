# Comparing `tmp/nonebot_plugin_with_ai_agents-0.1.5.tar.gz` & `tmp/nonebot_plugin_with_ai_agents-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_with_ai_agents-0.1.5.tar", max compression
+gzip compressed data, was "nonebot_plugin_with_ai_agents-0.1.6.tar", max compression
```

## Comparing `nonebot_plugin_with_ai_agents-0.1.5.tar` & `nonebot_plugin_with_ai_agents-0.1.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0      510 2024-05-08 02:53:03.922341 nonebot_plugin_with_ai_agents-0.1.5/nonebot_plugin_with_ai_agents/__init__.py
--rw-r--r--   0        0        0      519 2024-05-06 07:05:33.777069 nonebot_plugin_with_ai_agents-0.1.5/nonebot_plugin_with_ai_agents/handler.py
--rw-r--r--   0        0        0        2 2024-05-06 07:05:33.777069 nonebot_plugin_with_ai_agents-0.1.5/nonebot_plugin_with_ai_agents/llm/__init__.py
--rw-r--r--   0        0        0     4529 2024-05-07 10:03:19.704778 nonebot_plugin_with_ai_agents-0.1.5/nonebot_plugin_with_ai_agents/llm/agents.py
--rw-r--r--   0        0        0     3019 2024-05-07 16:48:48.395458 nonebot_plugin_with_ai_agents-0.1.5/nonebot_plugin_with_ai_agents/llm/central_brain.py
--rw-r--r--   0        0        0      675 2024-05-06 07:05:33.778077 nonebot_plugin_with_ai_agents-0.1.5/nonebot_plugin_with_ai_agents/llm/config.py
--rw-r--r--   0        0        0      131 2024-05-06 07:05:33.778077 nonebot_plugin_with_ai_agents-0.1.5/nonebot_plugin_with_ai_agents/llm/llms/__init__.py
--rw-r--r--   0        0        0      453 2024-05-07 11:12:58.483693 nonebot_plugin_with_ai_agents-0.1.5/nonebot_plugin_with_ai_agents/llm/llms/base.py
--rw-r--r--   0        0        0     2277 2024-05-07 11:13:28.157800 nonebot_plugin_with_ai_agents-0.1.5/nonebot_plugin_with_ai_agents/llm/llms/dashscope.py
--rw-r--r--   0        0        0     1942 2024-05-07 11:13:28.219069 nonebot_plugin_with_ai_agents-0.1.5/nonebot_plugin_with_ai_agents/llm/llms/glm.py
--rw-r--r--   0        0        0     2046 2024-05-07 11:13:28.141789 nonebot_plugin_with_ai_agents-0.1.5/nonebot_plugin_with_ai_agents/llm/llms/openai.py
--rw-r--r--   0        0        0       19 2024-05-06 07:05:33.780198 nonebot_plugin_with_ai_agents-0.1.5/nonebot_plugin_with_ai_agents/llm/mem_stores.py
--rw-r--r--   0        0        0      338 2024-05-07 08:06:18.016313 nonebot_plugin_with_ai_agents-0.1.5/nonebot_plugin_with_ai_agents/llm/services.py
--rw-r--r--   0        0        0        0 2024-05-06 07:05:33.780198 nonebot_plugin_with_ai_agents-0.1.5/nonebot_plugin_with_ai_agents/llm/utils/__init__.py
--rw-r--r--   0        0        0     4648 2024-05-06 07:05:33.780198 nonebot_plugin_with_ai_agents-0.1.5/nonebot_plugin_with_ai_agents/llm/utils/prompts.py
--rw-r--r--   0        0        0     3358 2024-05-07 10:03:19.714495 nonebot_plugin_with_ai_agents-0.1.5/nonebot_plugin_with_ai_agents/llm/utils/retrievers.py
--rw-r--r--   0        0        0      715 2024-05-08 03:03:31.048823 nonebot_plugin_with_ai_agents-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     4571 2024-05-08 03:00:06.458396 nonebot_plugin_with_ai_agents-0.1.5/README.md
--rw-r--r--   0        0        0     5421 1970-01-01 00:00:00.000000 nonebot_plugin_with_ai_agents-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      510 2024-05-08 08:28:49.886180 nonebot_plugin_with_ai_agents-0.1.6/nonebot_plugin_with_ai_agents/__init__.py
+-rw-r--r--   0        0        0      439 2024-05-08 09:38:16.947093 nonebot_plugin_with_ai_agents-0.1.6/nonebot_plugin_with_ai_agents/handler.py
+-rw-r--r--   0        0        0        2 2024-05-06 07:05:33.777069 nonebot_plugin_with_ai_agents-0.1.6/nonebot_plugin_with_ai_agents/llm/__init__.py
+-rw-r--r--   0        0        0     4529 2024-05-08 09:00:09.567226 nonebot_plugin_with_ai_agents-0.1.6/nonebot_plugin_with_ai_agents/llm/agents.py
+-rw-r--r--   0        0        0     3001 2024-05-08 09:00:09.568229 nonebot_plugin_with_ai_agents-0.1.6/nonebot_plugin_with_ai_agents/llm/central_brain.py
+-rw-r--r--   0        0        0      849 2024-05-08 09:00:09.568229 nonebot_plugin_with_ai_agents-0.1.6/nonebot_plugin_with_ai_agents/llm/config.py
+-rw-r--r--   0        0        0      131 2024-05-06 07:05:33.778077 nonebot_plugin_with_ai_agents-0.1.6/nonebot_plugin_with_ai_agents/llm/llms/__init__.py
+-rw-r--r--   0        0        0      453 2024-05-07 11:12:58.483693 nonebot_plugin_with_ai_agents-0.1.6/nonebot_plugin_with_ai_agents/llm/llms/base.py
+-rw-r--r--   0        0        0     2277 2024-05-07 11:13:28.157800 nonebot_plugin_with_ai_agents-0.1.6/nonebot_plugin_with_ai_agents/llm/llms/dashscope.py
+-rw-r--r--   0        0        0     1942 2024-05-07 11:13:28.219069 nonebot_plugin_with_ai_agents-0.1.6/nonebot_plugin_with_ai_agents/llm/llms/glm.py
+-rw-r--r--   0        0        0     2046 2024-05-07 11:13:28.141789 nonebot_plugin_with_ai_agents-0.1.6/nonebot_plugin_with_ai_agents/llm/llms/openai.py
+-rw-r--r--   0        0        0       19 2024-05-06 07:05:33.780198 nonebot_plugin_with_ai_agents-0.1.6/nonebot_plugin_with_ai_agents/llm/mem_stores.py
+-rw-r--r--   0        0        0      338 2024-05-07 08:06:18.016313 nonebot_plugin_with_ai_agents-0.1.6/nonebot_plugin_with_ai_agents/llm/services.py
+-rw-r--r--   0        0        0        0 2024-05-06 07:05:33.780198 nonebot_plugin_with_ai_agents-0.1.6/nonebot_plugin_with_ai_agents/llm/utils/__init__.py
+-rw-r--r--   0        0        0     4648 2024-05-06 07:05:33.780198 nonebot_plugin_with_ai_agents-0.1.6/nonebot_plugin_with_ai_agents/llm/utils/prompts.py
+-rw-r--r--   0        0        0     3358 2024-05-07 10:03:19.714495 nonebot_plugin_with_ai_agents-0.1.6/nonebot_plugin_with_ai_agents/llm/utils/retrievers.py
+-rw-r--r--   0        0        0      694 2024-05-08 09:42:51.226092 nonebot_plugin_with_ai_agents-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     6811 2024-05-08 09:06:10.571877 nonebot_plugin_with_ai_agents-0.1.6/README.md
+-rw-r--r--   0        0        0     7616 1970-01-01 00:00:00.000000 nonebot_plugin_with_ai_agents-0.1.6/PKG-INFO
```

### Comparing `nonebot_plugin_with_ai_agents-0.1.5/nonebot_plugin_with_ai_agents/llm/agents.py` & `nonebot_plugin_with_ai_agents-0.1.6/nonebot_plugin_with_ai_agents/llm/agents.py`

 * *Files 4% similar despite different names*

```diff
@@ -74,16 +74,16 @@
         {question}
         """
         '''
         llm_res = await llm.ask_model(question=prompt)
         print(f"需要联网搜索，llm_res={llm_res}")
 
         # 联网搜索
-        if config.TAVILY_API_KEY:
-            search_result = await retrievers.search_tavily(query=llm_res, api_key=config.TAVILY_API_KEY)
+        if config.tavily_api_key:
+            search_result = await retrievers.search_tavily(query=llm_res, api_key=config.tavily_api_key)
         else:
             search_result = await retrievers.search_baidu(query=llm_res)
         result = f"\"{llm_res}\" 在搜索引擎的搜索结果是：{search_result}"
         return result
 
 
 class Type4:
```

### Comparing `nonebot_plugin_with_ai_agents-0.1.5/nonebot_plugin_with_ai_agents/llm/central_brain.py` & `nonebot_plugin_with_ai_agents-0.1.6/nonebot_plugin_with_ai_agents/llm/central_brain.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     return llm
 
 
 async def ask_central_brain(raw_question: str):
     """向中心智脑提问"""
 
     # 选择智脑使用的大模型
-    llm = get_llm_model(config.AI_AGENT_PLATFORM, config.AI_AGENT_KEY, config.AI_AGENT_MODEL)
+    llm = get_llm_model(config.platform, config.api_key, config.model_name)
     if not llm:
         return "大模型获取失败，请检查配置。配置文档参考：https://github.com/yejue/nonebot-plugin-with-ai-agents"
 
     # 获取聊天历史
     chat_history_list = ChatService.get_history_list()
 
     # 将用户提问发送到大模型分类器，获取分类列表
```

### Comparing `nonebot_plugin_with_ai_agents-0.1.5/nonebot_plugin_with_ai_agents/llm/llms/dashscope.py` & `nonebot_plugin_with_ai_agents-0.1.6/nonebot_plugin_with_ai_agents/llm/llms/dashscope.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_with_ai_agents-0.1.5/nonebot_plugin_with_ai_agents/llm/llms/glm.py` & `nonebot_plugin_with_ai_agents-0.1.6/nonebot_plugin_with_ai_agents/llm/llms/glm.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_with_ai_agents-0.1.5/nonebot_plugin_with_ai_agents/llm/llms/openai.py` & `nonebot_plugin_with_ai_agents-0.1.6/nonebot_plugin_with_ai_agents/llm/llms/openai.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_with_ai_agents-0.1.5/nonebot_plugin_with_ai_agents/llm/utils/prompts.py` & `nonebot_plugin_with_ai_agents-0.1.6/nonebot_plugin_with_ai_agents/llm/utils/prompts.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_with_ai_agents-0.1.5/nonebot_plugin_with_ai_agents/llm/utils/retrievers.py` & `nonebot_plugin_with_ai_agents-0.1.6/nonebot_plugin_with_ai_agents/llm/utils/retrievers.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_with_ai_agents-0.1.5/pyproject.toml` & `nonebot_plugin_with_ai_agents-0.1.6/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "nonebot-plugin-with-ai-agents"
-version = "0.1.5"
-description = "nonebot_plugin_with_ai_agents 是一个基于基本原理实现的 AI Agents（智能体），拥有联网搜索能力（实时搜索等）、页面内容提取并学习回答、命令执行等功能"
+version = "0.1.6"
+description = "nonebot_plugin_with_ai_agents 是一个基于基本原理实现的 AI Agents（智能体），拥有联网搜索能力、页面内容提取并学习回答、命令执行等功能"
 authors = ["yejue <1145331931@qq.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 nonebot2 = "^2.0"
 beautifulsoup4 = "*"
```

