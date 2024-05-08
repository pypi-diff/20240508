# Comparing `tmp/nonebot_plugin_with_ai_agents-0.1.7.tar.gz` & `tmp/nonebot_plugin_with_ai_agents-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_with_ai_agents-0.1.7.tar", max compression
+gzip compressed data, was "nonebot_plugin_with_ai_agents-0.1.8.tar", max compression
```

## Comparing `nonebot_plugin_with_ai_agents-0.1.7.tar` & `nonebot_plugin_with_ai_agents-0.1.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0      510 2024-05-08 08:28:49.886180 nonebot_plugin_with_ai_agents-0.1.7/nonebot_plugin_with_ai_agents/__init__.py
--rw-r--r--   0        0        0      439 2024-05-08 09:38:16.947093 nonebot_plugin_with_ai_agents-0.1.7/nonebot_plugin_with_ai_agents/handler.py
--rw-r--r--   0        0        0        2 2024-05-06 07:05:33.777069 nonebot_plugin_with_ai_agents-0.1.7/nonebot_plugin_with_ai_agents/llm/__init__.py
--rw-r--r--   0        0        0     4529 2024-05-08 09:00:09.567226 nonebot_plugin_with_ai_agents-0.1.7/nonebot_plugin_with_ai_agents/llm/agents.py
--rw-r--r--   0        0        0     3184 2024-05-08 09:53:49.782564 nonebot_plugin_with_ai_agents-0.1.7/nonebot_plugin_with_ai_agents/llm/central_brain.py
--rw-r--r--   0        0        0     1083 2024-05-08 09:54:00.100650 nonebot_plugin_with_ai_agents-0.1.7/nonebot_plugin_with_ai_agents/llm/config.py
--rw-r--r--   0        0        0      131 2024-05-06 07:05:33.778077 nonebot_plugin_with_ai_agents-0.1.7/nonebot_plugin_with_ai_agents/llm/llms/__init__.py
--rw-r--r--   0        0        0      453 2024-05-07 11:12:58.483693 nonebot_plugin_with_ai_agents-0.1.7/nonebot_plugin_with_ai_agents/llm/llms/base.py
--rw-r--r--   0        0        0     2277 2024-05-07 11:13:28.157800 nonebot_plugin_with_ai_agents-0.1.7/nonebot_plugin_with_ai_agents/llm/llms/dashscope.py
--rw-r--r--   0        0        0     1942 2024-05-07 11:13:28.219069 nonebot_plugin_with_ai_agents-0.1.7/nonebot_plugin_with_ai_agents/llm/llms/glm.py
--rw-r--r--   0        0        0     2046 2024-05-07 11:13:28.141789 nonebot_plugin_with_ai_agents-0.1.7/nonebot_plugin_with_ai_agents/llm/llms/openai.py
--rw-r--r--   0        0        0       19 2024-05-06 07:05:33.780198 nonebot_plugin_with_ai_agents-0.1.7/nonebot_plugin_with_ai_agents/llm/mem_stores.py
--rw-r--r--   0        0        0      338 2024-05-07 08:06:18.016313 nonebot_plugin_with_ai_agents-0.1.7/nonebot_plugin_with_ai_agents/llm/services.py
--rw-r--r--   0        0        0        0 2024-05-06 07:05:33.780198 nonebot_plugin_with_ai_agents-0.1.7/nonebot_plugin_with_ai_agents/llm/utils/__init__.py
--rw-r--r--   0        0        0     4648 2024-05-06 07:05:33.780198 nonebot_plugin_with_ai_agents-0.1.7/nonebot_plugin_with_ai_agents/llm/utils/prompts.py
--rw-r--r--   0        0        0     3358 2024-05-07 10:03:19.714495 nonebot_plugin_with_ai_agents-0.1.7/nonebot_plugin_with_ai_agents/llm/utils/retrievers.py
--rw-r--r--   0        0        0      694 2024-05-08 09:55:14.702971 nonebot_plugin_with_ai_agents-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     6811 2024-05-08 09:06:10.571877 nonebot_plugin_with_ai_agents-0.1.7/README.md
--rw-r--r--   0        0        0     7616 1970-01-01 00:00:00.000000 nonebot_plugin_with_ai_agents-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0      510 2024-05-08 08:28:49.886180 nonebot_plugin_with_ai_agents-0.1.8/nonebot_plugin_with_ai_agents/__init__.py
+-rw-r--r--   0        0        0      743 2024-05-08 16:28:31.442912 nonebot_plugin_with_ai_agents-0.1.8/nonebot_plugin_with_ai_agents/handler.py
+-rw-r--r--   0        0        0        2 2024-05-06 07:05:33.777069 nonebot_plugin_with_ai_agents-0.1.8/nonebot_plugin_with_ai_agents/llm/__init__.py
+-rw-r--r--   0        0        0     4623 2024-05-08 15:59:57.148477 nonebot_plugin_with_ai_agents-0.1.8/nonebot_plugin_with_ai_agents/llm/agents.py
+-rw-r--r--   0        0        0     3266 2024-05-08 16:32:46.821602 nonebot_plugin_with_ai_agents-0.1.8/nonebot_plugin_with_ai_agents/llm/central_brain.py
+-rw-r--r--   0        0        0     1083 2024-05-08 09:54:00.100650 nonebot_plugin_with_ai_agents-0.1.8/nonebot_plugin_with_ai_agents/llm/config.py
+-rw-r--r--   0        0        0      131 2024-05-06 07:05:33.778077 nonebot_plugin_with_ai_agents-0.1.8/nonebot_plugin_with_ai_agents/llm/llms/__init__.py
+-rw-r--r--   0        0        0      520 2024-05-08 14:21:20.414475 nonebot_plugin_with_ai_agents-0.1.8/nonebot_plugin_with_ai_agents/llm/llms/base.py
+-rw-r--r--   0        0        0     2277 2024-05-07 11:13:28.157800 nonebot_plugin_with_ai_agents-0.1.8/nonebot_plugin_with_ai_agents/llm/llms/dashscope.py
+-rw-r--r--   0        0        0     1942 2024-05-07 11:13:28.219069 nonebot_plugin_with_ai_agents-0.1.8/nonebot_plugin_with_ai_agents/llm/llms/glm.py
+-rw-r--r--   0        0        0     2046 2024-05-07 11:13:28.141789 nonebot_plugin_with_ai_agents-0.1.8/nonebot_plugin_with_ai_agents/llm/llms/openai.py
+-rw-r--r--   0        0        0       19 2024-05-08 15:39:53.681731 nonebot_plugin_with_ai_agents-0.1.8/nonebot_plugin_with_ai_agents/llm/mem_stores.py
+-rw-r--r--   0        0        0     1727 2024-05-08 16:28:10.356972 nonebot_plugin_with_ai_agents-0.1.8/nonebot_plugin_with_ai_agents/llm/services.py
+-rw-r--r--   0        0        0        0 2024-05-06 07:05:33.780198 nonebot_plugin_with_ai_agents-0.1.8/nonebot_plugin_with_ai_agents/llm/utils/__init__.py
+-rw-r--r--   0        0        0     4576 2024-05-08 16:32:46.840606 nonebot_plugin_with_ai_agents-0.1.8/nonebot_plugin_with_ai_agents/llm/utils/prompts.py
+-rw-r--r--   0        0        0     3358 2024-05-07 10:03:19.714495 nonebot_plugin_with_ai_agents-0.1.8/nonebot_plugin_with_ai_agents/llm/utils/retrievers.py
+-rw-r--r--   0        0        0      679 2024-05-08 16:35:10.830362 nonebot_plugin_with_ai_agents-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     7057 2024-05-08 16:30:07.456483 nonebot_plugin_with_ai_agents-0.1.8/README.md
+-rw-r--r--   0        0        0     7842 1970-01-01 00:00:00.000000 nonebot_plugin_with_ai_agents-0.1.8/PKG-INFO
```

### Comparing `nonebot_plugin_with_ai_agents-0.1.7/nonebot_plugin_with_ai_agents/llm/agents.py` & `nonebot_plugin_with_ai_agents-0.1.8/nonebot_plugin_with_ai_agents/llm/agents.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,16 @@
     async def summarize_weblink_content(
             llm: Union[DashscopeModel, BaseLLMModel, GLMModel],
             question: str
     ):
         # 从问题中提取 URL
         url = Type1.extract_url_without_llm(question=question)
         print(f"type1 model res：{url}")
+        if not url:
+            return f"\"{url}\" 的大致内容是：内容提取失败"
 
         # 提取页面内容
         url_content = await retrievers.get_url_content(url)
         url_content = url_content[:3000]
         result = f"\"{url}\" 的大致内容是：{url_content}"
         return result
```

### Comparing `nonebot_plugin_with_ai_agents-0.1.7/nonebot_plugin_with_ai_agents/llm/central_brain.py` & `nonebot_plugin_with_ai_agents-0.1.8/nonebot_plugin_with_ai_agents/llm/central_brain.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,17 +33,14 @@
         return "WITH_AI_AGENTS 配置获取失败，请检查配置。配置文档参考：https://github.com/yejue/nonebot-plugin-with-ai-agents"
 
     # 选择智脑使用的大模型
     llm = get_llm_model(config.platform, config.api_key, config.model_name)
     if not llm:
         return "WITH_AI_AGENTS 大模型获取失败，请检查配置。配置文档参考：https://github.com/yejue/nonebot-plugin-with-ai-agents"
 
-    # 获取聊天历史
-    chat_history_list = ChatService.get_history_list()
-
     # 将用户提问发送到大模型分类器，获取分类列表
     prompt = prompts.get_classifier_prompt(question=raw_question)
     s = prompts.get_classifier_master_prompt()
     classifier_res = await llm.ask_model(question=prompt, system_prompt=s)
     print(f"raw_classifier_res: {classifier_res}")
     classifier_res = json.loads(classifier_res)
     print(f"智脑分类结果：{classifier_res}")
@@ -55,24 +52,29 @@
         if int(num) == 1:    # 提取页面内容
             agent_data += await agents.type1.summarize_weblink_content(llm=llm, question=raw_question) + "\n"
         elif int(num) == 2:  # 联网搜索能力
             agent_data += await agents.type2.get_search_result(llm=llm, question=raw_question)
         elif int(num) == 3:  # 某地天气
             pass
         elif int(num) == 4:  # 执行指令
-            agent_data += await agents.type4.get_command_result(llm=llm, question=raw_question)
+            # agent_data += await agents.type4.get_command_result(llm=llm, question=raw_question)
+            pass
         elif int(num) == 5:  # who are you
             agent_data += agents.type5.get_who_you_are() + "\n"
         elif int(num) == 6:  # 功能列表
             agent_data += agents.type6.get_ai_abilities() + "\n"
 
     # 携带 context 向大模型提问 raw_question
     assemble_prompt = prompts.get_assemble_prompt(question=raw_question, agent_data=agent_data)
     print("assemble_prompt", assemble_prompt)
+
+    # Chat History 策略获取
+    chat_history_list = ChatService.get_strategically_chat_history(assemble_prompt, max_length=llm.max_length)
+
     s = prompts.get_kurisu_prompt()
     assemble_res = await llm.ask_model(question=assemble_prompt, system_prompt=s, message_history=chat_history_list)
 
     # 将 AI 回答追加到历史
-    ChatService.add_message_to_history(text=assemble_prompt, role="user")
+    ChatService.add_message_to_history(text=raw_question, role="user")
     ChatService.add_message_to_history(text=assemble_res, role="assistant")
 
     return assemble_res
```

### Comparing `nonebot_plugin_with_ai_agents-0.1.7/nonebot_plugin_with_ai_agents/llm/config.py` & `nonebot_plugin_with_ai_agents-0.1.8/nonebot_plugin_with_ai_agents/llm/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_with_ai_agents-0.1.7/nonebot_plugin_with_ai_agents/llm/llms/dashscope.py` & `nonebot_plugin_with_ai_agents-0.1.8/nonebot_plugin_with_ai_agents/llm/llms/dashscope.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_with_ai_agents-0.1.7/nonebot_plugin_with_ai_agents/llm/llms/glm.py` & `nonebot_plugin_with_ai_agents-0.1.8/nonebot_plugin_with_ai_agents/llm/llms/glm.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_with_ai_agents-0.1.7/nonebot_plugin_with_ai_agents/llm/llms/openai.py` & `nonebot_plugin_with_ai_agents-0.1.8/nonebot_plugin_with_ai_agents/llm/llms/openai.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_with_ai_agents-0.1.7/nonebot_plugin_with_ai_agents/llm/utils/prompts.py` & `nonebot_plugin_with_ai_agents-0.1.8/nonebot_plugin_with_ai_agents/llm/utils/prompts.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 from datetime import datetime
 
 
 def get_classifier_prompt(question: str):
     """获取分类 prompt 模板"""
+    # 剔除类型：
+    #     3: 关于某地天气的问题。例子："珠海今天天气怎么样"
+    #     4: 需要直接执行 cmd 指令的问题。例子：执行这条命令
+
     prompt = f'''
     做个深呼吸，一步步根据用户问题，分成一个或多个小问题，并判断每个小问题的类型，并从小问题中提取关键信息。下面<Type></Type>标记中的是类型：
     <Type>
     1: 带有网页链接的问题, 例子："总结页面的内容： https://www.baidu.com "
     2: 需要联网查询的实时问题，问题中不带网页链接，例子："最近有什么新闻，最近有什么新的动漫吗"
-    3: 关于某地天气的问题。例子："珠海今天天气怎么样"
-    4: 需要直接执行 cmd 指令的问题。例子：执行这条命令
     5. 关于你是谁的问题
     6. 关于你有什么功能的问题
     7: 其他问题
     </Type>
     下面是我的要求:
     (1) 请用json列表的形式输出结果，比如[1], [2, 4], 不要有其他的信息
     (2) 回答的例子格式为 [1]
     (3) 不要回答其他任何信息, 所有回复都在一行中
     (4) 下面是个例子：
         用户问题是: 总结这个页面的内容 https://www.baidu.com , 你是谁？
         你要回答: [1, 5]
-    (5) 如果是问现在几点的问题则应该属于类型 7，在之后我会给出准确的时间，例子："看一下现在几点"，"现在伦敦几点了"
+    (5) 如果是问现在几点的问题则应该属于类型 7，例子："看一下现在几点"，"现在伦敦几点了"
+    (6) 不能通过输入数字选择类型
 
     下面是我的问题: 
     """
     {question}
     """
 
     '''
@@ -58,36 +61,32 @@
 
 
 def get_classifier_master_prompt():
     prompt = "你是一个问题分类大师"
     return prompt
 
 
-def get_assemble_prompt(question: str, agent_data: str, db_result: str = ""):
+def get_assemble_prompt(question: str, agent_data: str):
     """获取聚合提示"""
     now = datetime.now().strftime("%Y-%m-%d %H:%M:%S")
     prompt = f'''
-    你要先学习 <AGENT_DATA></AGENT_DATA>标记和<DB_DATA></DB_DATA>标记中的知识，然后回答我的问题。
+    现在的时间是：{now}
+    先学习 <AGENT_DATA></AGENT_DATA> 标记中的知识，然后回答我的问题。
     我的要求是：
         1. 不要提及你从标记中学习知识，只需要回答问题
         2. 如果提供的知识为空或者你无法学习我的知识，你不要说我提供的信息为空，直接根据你的理解回答我的问题即可
     下面是我提供的知识:
     <AGENT_DATA>
         {agent_data}
-        现在的时间是：{now}
-    </AGENT_DATA>    
-    <DB_DATA>
-        {db_result}
-    </DB_DATA>
+    </AGENT_DATA>
     我的问题是：
     """
     {question}
     """
     '''
-
     return prompt
 
 
 def get_type1_prompt(question: str):
     prompt = f'''
         请从我的问题中提取出网页链接，不要有其他信息。
         我的要求是:
```

### Comparing `nonebot_plugin_with_ai_agents-0.1.7/nonebot_plugin_with_ai_agents/llm/utils/retrievers.py` & `nonebot_plugin_with_ai_agents-0.1.8/nonebot_plugin_with_ai_agents/llm/utils/retrievers.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_with_ai_agents-0.1.7/pyproject.toml` & `nonebot_plugin_with_ai_agents-0.1.8/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "nonebot-plugin-with-ai-agents"
-version = "0.1.7"
-description = "nonebot_plugin_with_ai_agents 是一个基于基本原理实现的 AI Agents（智能体），拥有联网搜索能力、页面内容提取并学习回答、命令执行等功能"
+version = "0.1.8"
+description = "nonebot_plugin_with_ai_agents 是一个基于基本原理实现的 AI Agents（智能体），拥有联网搜索能力、页面内容提取并学习回答等功能"
 authors = ["yejue <1145331931@qq.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 nonebot2 = "^2.0"
 beautifulsoup4 = "*"
```

### Comparing `nonebot_plugin_with_ai_agents-0.1.7/README.md` & `nonebot_plugin_with_ai_agents-0.1.8/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -54,20 +54,25 @@
 
 
 
 ## TODOs
 ”！！“ 为近期要做的事情
 ”~~“ 为可能会鸽的更新，慢慢来
 
+待解决问题:
+
  - [ ] ！！命令执行安全问题，方案：对特定 ID 可用，并提供可关停配置。
  - [ ] 新闻查询增强，方案：从各类新闻网获取聚合数据。
  - [ ] Prompt 调整，方案：优化和精简 Prompt。
  - [ ] AI 聊天历史对群聊和私聊做区分（考虑中，如果加的话可能会使用数据库）。
+ - [x] <del>主动清理聊天历史指令，`清空AI记录`</del>
  - [ ] ~~天气预报，没有很大兴趣。
  - [ ] ~~知识库，采用 Embeddings + PGVector 完成数据向量化和存储搜索。对于一个插件来说，体量可能过大。
+ - [x] <del>聊天历史过长的问题。方案：策略性选取历史。</del>
+ - [x] <del>聊天历史存入优化，方案：压缩存入策略</del>
 
 
 
 ## 一些说明
 
 1. 本 plugin 采用 Agents 基本原理实现。
 2. 本 plugin 中的联网能力基于百度、bing（暂时忽略不计）、或者 Tavily，推荐只使用百度。Tavily 确实提供了良好的聚合搜索，但是有可能会出现“50万”内容。
```

#### html2text {}

```diff
@@ -18,24 +18,27 @@
 æ°é»åå®¹ï¼ç®å AI
 å¯ä»¥æ ¹æ®éè¦å¯¹æä¸ªäºä»¶æ¥æç´¢å°å¤§æ¦ä¿¡æ¯ï¼ä¾å¦ï¼âäºè§£ä¸ç æµ·æ´é¨âï¼åè¿è¡åç­ï¼ä¹åä¼åæä¸é¨çæ°é»æ¨¡åã
 5. å½ä»¤æ§è¡ï¼AI
 ä»æ¥æ¶å°çä¿¡æ¯è¯­ä¹ä¸­è§£æåºè¦æ§è¡çæä»¤ï¼æ§è¡å®æå°ç»æè½¬è¾¾ãæ§è¡å½ä»¤ä½¿ç¨çæ¯
 subprocess æ¨¡åã
 æ³¨æï¼ç±äºæªåä»»ä½çæéæ§å¶ï¼è¿ä¸ªåè½æéå¸¸é«çé£é©ã
 ## TODOs âï¼ï¼â ä¸ºè¿æè¦åçäºæ â~~â
-ä¸ºå¯è½ä¼é¸½çæ´æ°ï¼æ¢æ¢æ¥ - [ ]
+ä¸ºå¯è½ä¼é¸½çæ´æ°ï¼æ¢æ¢æ¥ å¾è§£å³é®é¢: - [ ]
 ï¼ï¼å½ä»¤æ§è¡å®å¨é®é¢ï¼æ¹æ¡ï¼å¯¹ç¹å® ID
 å¯ç¨ï¼å¹¶æä¾å¯å³åéç½®ã - [ ]
 æ°é»æ¥è¯¢å¢å¼ºï¼æ¹æ¡ï¼ä»åç±»æ°é»ç½è·åèåæ°æ®ã - [ ]
 Prompt è°æ´ï¼æ¹æ¡ï¼ä¼ååç²¾ç® Promptã - [ ] AI
 èå¤©åå²å¯¹ç¾¤èåç§èååºåï¼èèä¸­ï¼å¦æå çè¯å¯è½ä¼ä½¿ç¨æ°æ®åºï¼ã
-- [ ] ~~å¤©æ°é¢æ¥ï¼æ²¡æå¾å¤§å´è¶£ã - [ ] ~~ç¥è¯åºï¼éç¨
-Embeddings + PGVector
+- [x] ä¸»å¨æ¸çèå¤©åå²æä»¤ï¼`æ¸ç©ºAIè®°å½` - [ ]
+~~å¤©æ°é¢æ¥ï¼æ²¡æå¾å¤§å´è¶£ã - [ ] ~~ç¥è¯åºï¼éç¨ Embeddings +
+PGVector
 å®ææ°æ®åéååå­å¨æç´¢ãå¯¹äºä¸ä¸ªæä»¶æ¥è¯´ï¼ä½éå¯è½è¿å¤§ã
-## ä¸äºè¯´æ 1. æ¬ plugin éç¨ Agents åºæ¬åçå®ç°ã 2. æ¬ plugin
+- [x] èå¤©åå²è¿é¿çé®é¢ãæ¹æ¡ï¼ç­ç¥æ§éååå²ã - [x]
+èå¤©åå²å­å¥ä¼åï¼æ¹æ¡ï¼åç¼©å­å¥ç­ç¥ ## ä¸äºè¯´æ 1. æ¬
+plugin éç¨ Agents åºæ¬åçå®ç°ã 2. æ¬ plugin
 ä¸­çèç½è½ååºäºç¾åº¦ãbingï¼ææ¶å¿½ç¥ä¸è®¡ï¼ãæè
 Tavilyï¼æ¨èåªä½¿ç¨ç¾åº¦ãTavily
 ç¡®å®æä¾äºè¯å¥½çèåæç´¢ï¼ä½æ¯æå¯è½ä¼åºç°â50ä¸âåå®¹ã
 3. æ¬ plugin ä¸­å¯ä»¥éç½®æ¥å¥å¹¶ä¸éäºè¿äºå¤§æ¨¡åï¼ChatGLM
 ç³»åãéä¹åé®ç³»åãChatGPT ç³»åãä»¥åé­å¡ç¤¾åº Dashscope
 æä¾çæææ¨¡åï¼ç¾å·ãLlama3ç­ï¼ãæä»¶å¼åæ¶ä½¿ç¨çæ¯
 **dashscope** ç **qwen-turbo** æ¨¡åï¼å¨è°æ´äº **temperature**
```

### Comparing `nonebot_plugin_with_ai_agents-0.1.7/PKG-INFO` & `nonebot_plugin_with_ai_agents-0.1.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-with-ai-agents
-Version: 0.1.7
-Summary: nonebot_plugin_with_ai_agents 是一个基于基本原理实现的 AI Agents（智能体），拥有联网搜索能力、页面内容提取并学习回答、命令执行等功能
+Version: 0.1.8
+Summary: nonebot_plugin_with_ai_agents 是一个基于基本原理实现的 AI Agents（智能体），拥有联网搜索能力、页面内容提取并学习回答等功能
 Author: yejue
 Author-email: 1145331931@qq.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -74,20 +74,25 @@
 
 
 
 ## TODOs
 ”！！“ 为近期要做的事情
 ”~~“ 为可能会鸽的更新，慢慢来
 
+待解决问题:
+
  - [ ] ！！命令执行安全问题，方案：对特定 ID 可用，并提供可关停配置。
  - [ ] 新闻查询增强，方案：从各类新闻网获取聚合数据。
  - [ ] Prompt 调整，方案：优化和精简 Prompt。
  - [ ] AI 聊天历史对群聊和私聊做区分（考虑中，如果加的话可能会使用数据库）。
+ - [x] <del>主动清理聊天历史指令，`清空AI记录`</del>
  - [ ] ~~天气预报，没有很大兴趣。
  - [ ] ~~知识库，采用 Embeddings + PGVector 完成数据向量化和存储搜索。对于一个插件来说，体量可能过大。
+ - [x] <del>聊天历史过长的问题。方案：策略性选取历史。</del>
+ - [x] <del>聊天历史存入优化，方案：压缩存入策略</del>
 
 
 
 ## 一些说明
 
 1. 本 plugin 采用 Agents 基本原理实现。
 2. 本 plugin 中的联网能力基于百度、bing（暂时忽略不计）、或者 Tavily，推荐只使用百度。Tavily 确实提供了良好的聚合搜索，但是有可能会出现“50万”内容。
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-with-ai-agents Version: 0.1.7
+Metadata-Version: 2.1 Name: nonebot-plugin-with-ai-agents Version: 0.1.8
 Summary: nonebot_plugin_with_ai_agents æ¯ä¸ä¸ªåºäºåºæ¬åçå®ç°ç AI
-Agentsï¼æºè½ä½ï¼ï¼æ¥æèç½æç´¢è½åãé¡µé¢åå®¹æåå¹¶å­¦ä¹ åç­ãå½ä»¤æ§è¡ç­åè½
+Agentsï¼æºè½ä½ï¼ï¼æ¥æèç½æç´¢è½åãé¡µé¢åå®¹æåå¹¶å­¦ä¹ åç­ç­åè½
 Author: yejue Author-email: 1145331931@qq.com Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: beautifulsoup4 Requires-Dist: httpx (>=0.20.0) Requires-Dist:
 nonebot2 (>=2.0,<3.0) Project-URL: homepage, https://github.com/yejue/nonebot-
@@ -30,24 +30,27 @@
 æ°é»åå®¹ï¼ç®å AI
 å¯ä»¥æ ¹æ®éè¦å¯¹æä¸ªäºä»¶æ¥æç´¢å°å¤§æ¦ä¿¡æ¯ï¼ä¾å¦ï¼âäºè§£ä¸ç æµ·æ´é¨âï¼åè¿è¡åç­ï¼ä¹åä¼åæä¸é¨çæ°é»æ¨¡åã
 5. å½ä»¤æ§è¡ï¼AI
 ä»æ¥æ¶å°çä¿¡æ¯è¯­ä¹ä¸­è§£æåºè¦æ§è¡çæä»¤ï¼æ§è¡å®æå°ç»æè½¬è¾¾ãæ§è¡å½ä»¤ä½¿ç¨çæ¯
 subprocess æ¨¡åã
 æ³¨æï¼ç±äºæªåä»»ä½çæéæ§å¶ï¼è¿ä¸ªåè½æéå¸¸é«çé£é©ã
 ## TODOs âï¼ï¼â ä¸ºè¿æè¦åçäºæ â~~â
-ä¸ºå¯è½ä¼é¸½çæ´æ°ï¼æ¢æ¢æ¥ - [ ]
+ä¸ºå¯è½ä¼é¸½çæ´æ°ï¼æ¢æ¢æ¥ å¾è§£å³é®é¢: - [ ]
 ï¼ï¼å½ä»¤æ§è¡å®å¨é®é¢ï¼æ¹æ¡ï¼å¯¹ç¹å® ID
 å¯ç¨ï¼å¹¶æä¾å¯å³åéç½®ã - [ ]
 æ°é»æ¥è¯¢å¢å¼ºï¼æ¹æ¡ï¼ä»åç±»æ°é»ç½è·åèåæ°æ®ã - [ ]
 Prompt è°æ´ï¼æ¹æ¡ï¼ä¼ååç²¾ç® Promptã - [ ] AI
 èå¤©åå²å¯¹ç¾¤èåç§èååºåï¼èèä¸­ï¼å¦æå çè¯å¯è½ä¼ä½¿ç¨æ°æ®åºï¼ã
-- [ ] ~~å¤©æ°é¢æ¥ï¼æ²¡æå¾å¤§å´è¶£ã - [ ] ~~ç¥è¯åºï¼éç¨
-Embeddings + PGVector
+- [x] ä¸»å¨æ¸çèå¤©åå²æä»¤ï¼`æ¸ç©ºAIè®°å½` - [ ]
+~~å¤©æ°é¢æ¥ï¼æ²¡æå¾å¤§å´è¶£ã - [ ] ~~ç¥è¯åºï¼éç¨ Embeddings +
+PGVector
 å®ææ°æ®åéååå­å¨æç´¢ãå¯¹äºä¸ä¸ªæä»¶æ¥è¯´ï¼ä½éå¯è½è¿å¤§ã
-## ä¸äºè¯´æ 1. æ¬ plugin éç¨ Agents åºæ¬åçå®ç°ã 2. æ¬ plugin
+- [x] èå¤©åå²è¿é¿çé®é¢ãæ¹æ¡ï¼ç­ç¥æ§éååå²ã - [x]
+èå¤©åå²å­å¥ä¼åï¼æ¹æ¡ï¼åç¼©å­å¥ç­ç¥ ## ä¸äºè¯´æ 1. æ¬
+plugin éç¨ Agents åºæ¬åçå®ç°ã 2. æ¬ plugin
 ä¸­çèç½è½ååºäºç¾åº¦ãbingï¼ææ¶å¿½ç¥ä¸è®¡ï¼ãæè
 Tavilyï¼æ¨èåªä½¿ç¨ç¾åº¦ãTavily
 ç¡®å®æä¾äºè¯å¥½çèåæç´¢ï¼ä½æ¯æå¯è½ä¼åºç°â50ä¸âåå®¹ã
 3. æ¬ plugin ä¸­å¯ä»¥éç½®æ¥å¥å¹¶ä¸éäºè¿äºå¤§æ¨¡åï¼ChatGLM
 ç³»åãéä¹åé®ç³»åãChatGPT ç³»åãä»¥åé­å¡ç¤¾åº Dashscope
 æä¾çæææ¨¡åï¼ç¾å·ãLlama3ç­ï¼ãæä»¶å¼åæ¶ä½¿ç¨çæ¯
 **dashscope** ç **qwen-turbo** æ¨¡åï¼å¨è°æ´äº **temperature**
```

