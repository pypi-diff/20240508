# Comparing `tmp/nonebot_plugin_with_ai_agents-0.1.4.tar.gz` & `tmp/nonebot_plugin_with_ai_agents-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_with_ai_agents-0.1.4.tar", max compression
+gzip compressed data, was "nonebot_plugin_with_ai_agents-0.1.5.tar", max compression
```

## Comparing `nonebot_plugin_with_ai_agents-0.1.4.tar` & `nonebot_plugin_with_ai_agents-0.1.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0      414 2024-05-07 08:17:46.045650 nonebot_plugin_with_ai_agents-0.1.4/nonebot_plugin_with_ai_agents/__init__.py
--rw-r--r--   0        0        0      519 2024-05-06 07:05:33.777069 nonebot_plugin_with_ai_agents-0.1.4/nonebot_plugin_with_ai_agents/handler.py
--rw-r--r--   0        0        0        2 2024-05-06 07:05:33.777069 nonebot_plugin_with_ai_agents-0.1.4/nonebot_plugin_with_ai_agents/llm/__init__.py
--rw-r--r--   0        0        0     4529 2024-05-07 10:03:19.704778 nonebot_plugin_with_ai_agents-0.1.4/nonebot_plugin_with_ai_agents/llm/agents.py
--rw-r--r--   0        0        0     3019 2024-05-07 16:48:48.395458 nonebot_plugin_with_ai_agents-0.1.4/nonebot_plugin_with_ai_agents/llm/central_brain.py
--rw-r--r--   0        0        0      675 2024-05-06 07:05:33.778077 nonebot_plugin_with_ai_agents-0.1.4/nonebot_plugin_with_ai_agents/llm/config.py
--rw-r--r--   0        0        0      131 2024-05-06 07:05:33.778077 nonebot_plugin_with_ai_agents-0.1.4/nonebot_plugin_with_ai_agents/llm/llms/__init__.py
--rw-r--r--   0        0        0      453 2024-05-07 11:12:58.483693 nonebot_plugin_with_ai_agents-0.1.4/nonebot_plugin_with_ai_agents/llm/llms/base.py
--rw-r--r--   0        0        0     2277 2024-05-07 11:13:28.157800 nonebot_plugin_with_ai_agents-0.1.4/nonebot_plugin_with_ai_agents/llm/llms/dashscope.py
--rw-r--r--   0        0        0     1942 2024-05-07 11:13:28.219069 nonebot_plugin_with_ai_agents-0.1.4/nonebot_plugin_with_ai_agents/llm/llms/glm.py
--rw-r--r--   0        0        0     2046 2024-05-07 11:13:28.141789 nonebot_plugin_with_ai_agents-0.1.4/nonebot_plugin_with_ai_agents/llm/llms/openai.py
--rw-r--r--   0        0        0       19 2024-05-06 07:05:33.780198 nonebot_plugin_with_ai_agents-0.1.4/nonebot_plugin_with_ai_agents/llm/mem_stores.py
--rw-r--r--   0        0        0      338 2024-05-07 08:06:18.016313 nonebot_plugin_with_ai_agents-0.1.4/nonebot_plugin_with_ai_agents/llm/services.py
--rw-r--r--   0        0        0        0 2024-05-06 07:05:33.780198 nonebot_plugin_with_ai_agents-0.1.4/nonebot_plugin_with_ai_agents/llm/utils/__init__.py
--rw-r--r--   0        0        0     4648 2024-05-06 07:05:33.780198 nonebot_plugin_with_ai_agents-0.1.4/nonebot_plugin_with_ai_agents/llm/utils/prompts.py
--rw-r--r--   0        0        0     3358 2024-05-07 10:03:19.714495 nonebot_plugin_with_ai_agents-0.1.4/nonebot_plugin_with_ai_agents/llm/utils/retrievers.py
--rw-r--r--   0        0        0      715 2024-05-08 02:41:07.029205 nonebot_plugin_with_ai_agents-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     4310 2024-05-07 15:18:47.979516 nonebot_plugin_with_ai_agents-0.1.4/README.md
--rw-r--r--   0        0        0     5175 1970-01-01 00:00:00.000000 nonebot_plugin_with_ai_agents-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      510 2024-05-08 02:53:03.922341 nonebot_plugin_with_ai_agents-0.1.5/nonebot_plugin_with_ai_agents/__init__.py
+-rw-r--r--   0        0        0      519 2024-05-06 07:05:33.777069 nonebot_plugin_with_ai_agents-0.1.5/nonebot_plugin_with_ai_agents/handler.py
+-rw-r--r--   0        0        0        2 2024-05-06 07:05:33.777069 nonebot_plugin_with_ai_agents-0.1.5/nonebot_plugin_with_ai_agents/llm/__init__.py
+-rw-r--r--   0        0        0     4529 2024-05-07 10:03:19.704778 nonebot_plugin_with_ai_agents-0.1.5/nonebot_plugin_with_ai_agents/llm/agents.py
+-rw-r--r--   0        0        0     3019 2024-05-07 16:48:48.395458 nonebot_plugin_with_ai_agents-0.1.5/nonebot_plugin_with_ai_agents/llm/central_brain.py
+-rw-r--r--   0        0        0      675 2024-05-06 07:05:33.778077 nonebot_plugin_with_ai_agents-0.1.5/nonebot_plugin_with_ai_agents/llm/config.py
+-rw-r--r--   0        0        0      131 2024-05-06 07:05:33.778077 nonebot_plugin_with_ai_agents-0.1.5/nonebot_plugin_with_ai_agents/llm/llms/__init__.py
+-rw-r--r--   0        0        0      453 2024-05-07 11:12:58.483693 nonebot_plugin_with_ai_agents-0.1.5/nonebot_plugin_with_ai_agents/llm/llms/base.py
+-rw-r--r--   0        0        0     2277 2024-05-07 11:13:28.157800 nonebot_plugin_with_ai_agents-0.1.5/nonebot_plugin_with_ai_agents/llm/llms/dashscope.py
+-rw-r--r--   0        0        0     1942 2024-05-07 11:13:28.219069 nonebot_plugin_with_ai_agents-0.1.5/nonebot_plugin_with_ai_agents/llm/llms/glm.py
+-rw-r--r--   0        0        0     2046 2024-05-07 11:13:28.141789 nonebot_plugin_with_ai_agents-0.1.5/nonebot_plugin_with_ai_agents/llm/llms/openai.py
+-rw-r--r--   0        0        0       19 2024-05-06 07:05:33.780198 nonebot_plugin_with_ai_agents-0.1.5/nonebot_plugin_with_ai_agents/llm/mem_stores.py
+-rw-r--r--   0        0        0      338 2024-05-07 08:06:18.016313 nonebot_plugin_with_ai_agents-0.1.5/nonebot_plugin_with_ai_agents/llm/services.py
+-rw-r--r--   0        0        0        0 2024-05-06 07:05:33.780198 nonebot_plugin_with_ai_agents-0.1.5/nonebot_plugin_with_ai_agents/llm/utils/__init__.py
+-rw-r--r--   0        0        0     4648 2024-05-06 07:05:33.780198 nonebot_plugin_with_ai_agents-0.1.5/nonebot_plugin_with_ai_agents/llm/utils/prompts.py
+-rw-r--r--   0        0        0     3358 2024-05-07 10:03:19.714495 nonebot_plugin_with_ai_agents-0.1.5/nonebot_plugin_with_ai_agents/llm/utils/retrievers.py
+-rw-r--r--   0        0        0      715 2024-05-08 03:03:31.048823 nonebot_plugin_with_ai_agents-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     4571 2024-05-08 03:00:06.458396 nonebot_plugin_with_ai_agents-0.1.5/README.md
+-rw-r--r--   0        0        0     5421 1970-01-01 00:00:00.000000 nonebot_plugin_with_ai_agents-0.1.5/PKG-INFO
```

### Comparing `nonebot_plugin_with_ai_agents-0.1.4/nonebot_plugin_with_ai_agents/handler.py` & `nonebot_plugin_with_ai_agents-0.1.5/nonebot_plugin_with_ai_agents/handler.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_with_ai_agents-0.1.4/nonebot_plugin_with_ai_agents/llm/agents.py` & `nonebot_plugin_with_ai_agents-0.1.5/nonebot_plugin_with_ai_agents/llm/agents.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_with_ai_agents-0.1.4/nonebot_plugin_with_ai_agents/llm/central_brain.py` & `nonebot_plugin_with_ai_agents-0.1.5/nonebot_plugin_with_ai_agents/llm/central_brain.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_with_ai_agents-0.1.4/nonebot_plugin_with_ai_agents/llm/config.py` & `nonebot_plugin_with_ai_agents-0.1.5/nonebot_plugin_with_ai_agents/llm/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_with_ai_agents-0.1.4/nonebot_plugin_with_ai_agents/llm/llms/dashscope.py` & `nonebot_plugin_with_ai_agents-0.1.5/nonebot_plugin_with_ai_agents/llm/llms/dashscope.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_with_ai_agents-0.1.4/nonebot_plugin_with_ai_agents/llm/llms/glm.py` & `nonebot_plugin_with_ai_agents-0.1.5/nonebot_plugin_with_ai_agents/llm/llms/glm.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_with_ai_agents-0.1.4/nonebot_plugin_with_ai_agents/llm/llms/openai.py` & `nonebot_plugin_with_ai_agents-0.1.5/nonebot_plugin_with_ai_agents/llm/llms/openai.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_with_ai_agents-0.1.4/nonebot_plugin_with_ai_agents/llm/utils/prompts.py` & `nonebot_plugin_with_ai_agents-0.1.5/nonebot_plugin_with_ai_agents/llm/utils/prompts.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_with_ai_agents-0.1.4/nonebot_plugin_with_ai_agents/llm/utils/retrievers.py` & `nonebot_plugin_with_ai_agents-0.1.5/nonebot_plugin_with_ai_agents/llm/utils/retrievers.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_with_ai_agents-0.1.4/pyproject.toml` & `nonebot_plugin_with_ai_agents-0.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-with-ai-agents"
-version = "0.1.4"
+version = "0.1.5"
 description = "nonebot_plugin_with_ai_agents 是一个基于基本原理实现的 AI Agents（智能体），拥有联网搜索能力（实时搜索等）、页面内容提取并学习回答、命令执行等功能"
 authors = ["yejue <1145331931@qq.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 nonebot2 = "^2.0"
```

### Comparing `nonebot_plugin_with_ai_agents-0.1.4/README.md` & `nonebot_plugin_with_ai_agents-0.1.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -16,17 +16,32 @@
   </a>
   <img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">
 </p>
 
 
 ## 快速安装
 
+### nb-cli
+
 ```shell
-待更新
+nb plugin install nonebot-plugin-with-ai-agents
 ```
+### pip
+
+```shell
+pip install nonebot-plugin-with-ai-agents
+```
+
+### git
+
+```shell
+cd /your-nonebot-project-home/plugins/
+git clone https://github.com/yejue/nonebot-plugin-with-ai-agents.git
+```
+
 
 ## 功能描述
 AI Agents 功能包括不限于以下功能：
 1. 联网搜索：即当 AI 认为当前应该使用网络搜索时，进行搜索后回答
 2. 页面提取：在问题中自动提取 url，将 url 的内容提取学习后进行回答
 3. 天气预报：暂时是没有了，等下个版本更新
 4. 新闻内容：目前 AI 可以根据需要对某个事件来搜索到大概信息，例如：”了解下珠海暴雨“，再进行回答，之后会做成专门的新闻模块。
```

#### html2text {}

```diff
@@ -1,15 +1,18 @@
                                    _[_n_o_n_e_b_o_t_]
                          ************ WWiitthh--AAII--AAggeennttss ************
 _â¨ NoneBot AI
 å©çæä»¶ï¼æé¡µé¢åå®¹å­¦ä¹ ãé¡µé¢åå®¹æåãèç½å®æ¶æ¥è¯¢åç­ãå¤©æ°æ¥è¯¢ãå½ä»¤æ§è¡ç­åè½
 â¨_
                             _[_l_i_c_e_n_s_e_]_[_p_y_p_i_][python]
-## å¿«éå®è£ ```shell å¾æ´æ° ``` ## åè½æè¿° AI Agents
-åè½åæ¬ä¸éäºä»¥ä¸åè½ï¼ 1. èç½æç´¢ï¼å³å½ AI
+## å¿«éå®è£ ### nb-cli ```shell nb plugin install nonebot-plugin-with-ai-
+agents ``` ### pip ```shell pip install nonebot-plugin-with-ai-agents ``` ###
+git ```shell cd /your-nonebot-project-home/plugins/ git clone https://
+github.com/yejue/nonebot-plugin-with-ai-agents.git ``` ## åè½æè¿° AI
+Agents åè½åæ¬ä¸éäºä»¥ä¸åè½ï¼ 1. èç½æç´¢ï¼å³å½ AI
 è®¤ä¸ºå½ååºè¯¥ä½¿ç¨ç½ç»æç´¢æ¶ï¼è¿è¡æç´¢ååç­ 2.
 é¡µé¢æåï¼å¨é®é¢ä¸­èªå¨æå urlï¼å° url
 çåå®¹æåå­¦ä¹ åè¿è¡åç­ 3.
 å¤©æ°é¢æ¥ï¼ææ¶æ¯æ²¡æäºï¼ç­ä¸ä¸ªçæ¬æ´æ° 4.
 æ°é»åå®¹ï¼ç®å AI
 å¯ä»¥æ ¹æ®éè¦å¯¹æä¸ªäºä»¶æ¥æç´¢å°å¤§æ¦ä¿¡æ¯ï¼ä¾å¦ï¼âäºè§£ä¸ç æµ·æ´é¨âï¼åè¿è¡åç­ï¼ä¹åä¼åæä¸é¨çæ°é»æ¨¡åã
 5. å½ä»¤æ§è¡ï¼AI
```

### Comparing `nonebot_plugin_with_ai_agents-0.1.4/PKG-INFO` & `nonebot_plugin_with_ai_agents-0.1.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-with-ai-agents
-Version: 0.1.4
+Version: 0.1.5
 Summary: nonebot_plugin_with_ai_agents 是一个基于基本原理实现的 AI Agents（智能体），拥有联网搜索能力（实时搜索等）、页面内容提取并学习回答、命令执行等功能
 Author: yejue
 Author-email: 1145331931@qq.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -36,17 +36,32 @@
   </a>
   <img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">
 </p>
 
 
 ## 快速安装
 
+### nb-cli
+
 ```shell
-待更新
+nb plugin install nonebot-plugin-with-ai-agents
 ```
+### pip
+
+```shell
+pip install nonebot-plugin-with-ai-agents
+```
+
+### git
+
+```shell
+cd /your-nonebot-project-home/plugins/
+git clone https://github.com/yejue/nonebot-plugin-with-ai-agents.git
+```
+
 
 ## 功能描述
 AI Agents 功能包括不限于以下功能：
 1. 联网搜索：即当 AI 认为当前应该使用网络搜索时，进行搜索后回答
 2. 页面提取：在问题中自动提取 url，将 url 的内容提取学习后进行回答
 3. 天气预报：暂时是没有了，等下个版本更新
 4. 新闻内容：目前 AI 可以根据需要对某个事件来搜索到大概信息，例如：”了解下珠海暴雨“，再进行回答，之后会做成专门的新闻模块。
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-with-ai-agents Version: 0.1.4
+Metadata-Version: 2.1 Name: nonebot-plugin-with-ai-agents Version: 0.1.5
 Summary: nonebot_plugin_with_ai_agents æ¯ä¸ä¸ªåºäºåºæ¬åçå®ç°ç AI
 Agentsï¼æºè½ä½ï¼ï¼æ¥æèç½æç´¢è½åï¼å®æ¶æç´¢ç­ï¼ãé¡µé¢åå®¹æåå¹¶å­¦ä¹ åç­ãå½ä»¤æ§è¡ç­åè½
 Author: yejue Author-email: 1145331931@qq.com Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
@@ -12,16 +12,19 @@
 nonebot-plugin-with-ai-agents Description-Content-Type: text/markdown
                                    _[_n_o_n_e_b_o_t_]
                          ************ WWiitthh--AAII--AAggeennttss ************
 _â¨ NoneBot AI
 å©çæä»¶ï¼æé¡µé¢åå®¹å­¦ä¹ ãé¡µé¢åå®¹æåãèç½å®æ¶æ¥è¯¢åç­ãå¤©æ°æ¥è¯¢ãå½ä»¤æ§è¡ç­åè½
 â¨_
                             _[_l_i_c_e_n_s_e_]_[_p_y_p_i_][python]
-## å¿«éå®è£ ```shell å¾æ´æ° ``` ## åè½æè¿° AI Agents
-åè½åæ¬ä¸éäºä»¥ä¸åè½ï¼ 1. èç½æç´¢ï¼å³å½ AI
+## å¿«éå®è£ ### nb-cli ```shell nb plugin install nonebot-plugin-with-ai-
+agents ``` ### pip ```shell pip install nonebot-plugin-with-ai-agents ``` ###
+git ```shell cd /your-nonebot-project-home/plugins/ git clone https://
+github.com/yejue/nonebot-plugin-with-ai-agents.git ``` ## åè½æè¿° AI
+Agents åè½åæ¬ä¸éäºä»¥ä¸åè½ï¼ 1. èç½æç´¢ï¼å³å½ AI
 è®¤ä¸ºå½ååºè¯¥ä½¿ç¨ç½ç»æç´¢æ¶ï¼è¿è¡æç´¢ååç­ 2.
 é¡µé¢æåï¼å¨é®é¢ä¸­èªå¨æå urlï¼å° url
 çåå®¹æåå­¦ä¹ åè¿è¡åç­ 3.
 å¤©æ°é¢æ¥ï¼ææ¶æ¯æ²¡æäºï¼ç­ä¸ä¸ªçæ¬æ´æ° 4.
 æ°é»åå®¹ï¼ç®å AI
 å¯ä»¥æ ¹æ®éè¦å¯¹æä¸ªäºä»¶æ¥æç´¢å°å¤§æ¦ä¿¡æ¯ï¼ä¾å¦ï¼âäºè§£ä¸ç æµ·æ´é¨âï¼åè¿è¡åç­ï¼ä¹åä¼åæä¸é¨çæ°é»æ¨¡åã
 5. å½ä»¤æ§è¡ï¼AI
```

