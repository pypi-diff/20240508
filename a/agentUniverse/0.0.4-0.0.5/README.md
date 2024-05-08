# Comparing `tmp/agentUniverse-0.0.4.tar.gz` & `tmp/agentuniverse-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agentUniverse-0.0.4.tar", last modified: Fri Apr 26 09:36:05 2024, max compression
+gzip compressed data, was "agentuniverse-0.0.5.tar", last modified: Wed May  8 15:59:53 2024, max compression
```

## Comparing `agentUniverse-0.0.4.tar` & `agentuniverse-0.0.5.tar`

### file list

```diff
@@ -1,334 +1,242 @@
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:05.006355 agentUniverse-0.0.4/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)    11335 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/LICENSE
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     2701 2024-04-26 09:36:05.006088 agentUniverse-0.0.4/PKG-INFO
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     2713 2024-04-26 09:03:49.000000 agentUniverse-0.0.4/README.md
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:05.005705 agentUniverse-0.0.4/agentUniverse.egg-info/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     2701 2024-04-26 09:36:04.000000 agentUniverse-0.0.4/agentUniverse.egg-info/PKG-INFO
--rw-r--r--   0 jerry.zzw   (501) staff       (20)    12853 2024-04-26 09:36:04.000000 agentUniverse-0.0.4/agentUniverse.egg-info/SOURCES.txt
--rw-r--r--   0 jerry.zzw   (501) staff       (20)        1 2024-04-26 09:36:04.000000 agentUniverse-0.0.4/agentUniverse.egg-info/dependency_links.txt
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      362 2024-04-26 09:36:04.000000 agentUniverse-0.0.4/agentUniverse.egg-info/requires.txt
--rw-r--r--   0 jerry.zzw   (501) staff       (20)       88 2024-04-26 09:36:04.000000 agentUniverse-0.0.4/agentUniverse.egg-info/top_level.txt
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.946788 agentUniverse-0.0.4/agentuniverse/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 03:12:13.000000 agentUniverse-0.0.4/agentuniverse/__init__.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.949625 agentUniverse-0.0.4/agentuniverse/agent/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/agentuniverse/agent/__init__.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.949900 agentUniverse-0.0.4/agentuniverse/agent/action/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/agentuniverse/agent/action/__init__.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.950793 agentUniverse-0.0.4/agentuniverse/agent/action/knowledge/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/agentuniverse/agent/action/knowledge/__init__.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.951580 agentUniverse-0.0.4/agentuniverse/agent/action/knowledge/embedding/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/agentuniverse/agent/action/knowledge/embedding/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      972 2024-04-26 07:36:14.000000 agentUniverse-0.0.4/agentuniverse/agent/action/knowledge/embedding/embedding.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     4473 2024-04-26 07:36:14.000000 agentUniverse-0.0.4/agentuniverse/agent/action/knowledge/embedding/openai_embedding.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     3097 2024-04-26 03:46:54.000000 agentUniverse-0.0.4/agentuniverse/agent/action/knowledge/knowledge.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      655 2024-04-26 03:46:54.000000 agentUniverse-0.0.4/agentuniverse/agent/action/knowledge/knowledge_manager.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.952004 agentUniverse-0.0.4/agentuniverse/agent/action/knowledge/reader/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/agentuniverse/agent/action/knowledge/reader/__init__.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.953455 agentUniverse-0.0.4/agentuniverse/agent/action/knowledge/reader/file/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/agentuniverse/agent/action/knowledge/reader/file/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1160 2024-04-26 03:46:54.000000 agentUniverse-0.0.4/agentuniverse/agent/action/knowledge/reader/file/docx_reader.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1651 2024-04-26 07:36:14.000000 agentUniverse-0.0.4/agentuniverse/agent/action/knowledge/reader/file/file_reader.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1568 2024-04-26 03:46:54.000000 agentUniverse-0.0.4/agentuniverse/agent/action/knowledge/reader/file/pdf_reader.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1460 2024-04-26 03:46:54.000000 agentUniverse-0.0.4/agentuniverse/agent/action/knowledge/reader/file/pptx_reader.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1478 2024-04-26 07:36:14.000000 agentUniverse-0.0.4/agentuniverse/agent/action/knowledge/reader/file/web_pdf_reader.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      552 2024-04-26 03:46:54.000000 agentUniverse-0.0.4/agentuniverse/agent/action/knowledge/reader/reader.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.954383 agentUniverse-0.0.4/agentuniverse/agent/action/knowledge/store/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/agentuniverse/agent/action/knowledge/store/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     4674 2024-04-26 07:36:14.000000 agentUniverse-0.0.4/agentuniverse/agent/action/knowledge/store/chroma_store.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1997 2024-04-26 07:36:14.000000 agentUniverse-0.0.4/agentuniverse/agent/action/knowledge/store/document.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      662 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/agentuniverse/agent/action/knowledge/store/query.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     3190 2024-04-26 03:46:54.000000 agentUniverse-0.0.4/agentuniverse/agent/action/knowledge/store/store.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.955193 agentUniverse-0.0.4/agentuniverse/agent/action/tool/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/agentuniverse/agent/action/tool/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      276 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/agentuniverse/agent/action/tool/enum.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     3868 2024-04-26 07:36:14.000000 agentUniverse-0.0.4/agentuniverse/agent/action/tool/tool.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      626 2024-04-26 03:46:54.000000 agentUniverse-0.0.4/agentuniverse/agent/action/tool/tool_manager.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     5371 2024-04-26 03:44:06.000000 agentUniverse-0.0.4/agentuniverse/agent/agent.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      639 2024-04-26 03:44:12.000000 agentUniverse-0.0.4/agentuniverse/agent/agent_manager.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      526 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/agentuniverse/agent/agent_model.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.957938 agentUniverse-0.0.4/agentuniverse/agent/default/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      156 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/agentuniverse/agent/default/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     3034 2024-04-26 03:46:54.000000 agentUniverse-0.0.4/agentuniverse/agent/default/executing_agent.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      369 2024-04-26 09:03:49.000000 agentUniverse-0.0.4/agentuniverse/agent/default/executing_agent.yaml
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1937 2024-04-26 03:46:54.000000 agentUniverse-0.0.4/agentuniverse/agent/default/expressing_agent.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      366 2024-04-26 09:03:49.000000 agentUniverse-0.0.4/agentuniverse/agent/default/expressing_agent.yaml
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1532 2024-04-26 03:46:54.000000 agentUniverse-0.0.4/agentuniverse/agent/default/planning_agent.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      356 2024-04-26 09:03:49.000000 agentUniverse-0.0.4/agentuniverse/agent/default/planning_agent.yaml
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1247 2024-04-26 03:46:54.000000 agentUniverse-0.0.4/agentuniverse/agent/default/rag_agent.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      284 2024-04-26 09:03:49.000000 agentUniverse-0.0.4/agentuniverse/agent/default/rag_agent.yaml
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1862 2024-04-26 03:46:54.000000 agentUniverse-0.0.4/agentuniverse/agent/default/reviewing_agent.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      361 2024-04-26 09:03:49.000000 agentUniverse-0.0.4/agentuniverse/agent/default/reviewing_agent.yaml
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      657 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/agentuniverse/agent/input_object.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.960279 agentUniverse-0.0.4/agentuniverse/agent/memory/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-04-09 07:08:39.000000 agentUniverse-0.0.4/agentuniverse/agent/memory/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     3907 2024-04-26 09:03:49.000000 agentUniverse-0.0.4/agentuniverse/agent/memory/chat_memory.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.960873 agentUniverse-0.0.4/agentuniverse/agent/memory/default/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      174 2024-04-26 09:03:49.000000 agentUniverse-0.0.4/agentuniverse/agent/memory/default/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      845 2024-04-26 09:03:49.000000 agentUniverse-0.0.4/agentuniverse/agent/memory/default/default_memory.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      321 2024-04-26 09:03:49.000000 agentUniverse-0.0.4/agentuniverse/agent/memory/default/default_memory.yaml
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      402 2024-04-01 06:19:56.000000 agentUniverse-0.0.4/agentuniverse/agent/memory/enum.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     7689 2024-04-26 09:03:49.000000 agentUniverse-0.0.4/agentuniverse/agent/memory/langchain_instance.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     3054 2024-04-26 07:36:14.000000 agentUniverse-0.0.4/agentuniverse/agent/memory/memory.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      635 2024-04-26 03:46:54.000000 agentUniverse-0.0.4/agentuniverse/agent/memory/memory_manager.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      508 2024-04-09 16:15:17.000000 agentUniverse-0.0.4/agentuniverse/agent/memory/message.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      754 2024-04-26 09:03:49.000000 agentUniverse-0.0.4/agentuniverse/agent/memory/summarizer_cn_prompt.yaml
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      896 2024-04-26 09:03:49.000000 agentUniverse-0.0.4/agentuniverse/agent/memory/summarizer_en_prompt.yaml
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      572 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/agentuniverse/agent/output_object.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.961045 agentUniverse-0.0.4/agentuniverse/agent/plan/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      156 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/agentuniverse/agent/plan/__init__.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.961798 agentUniverse-0.0.4/agentuniverse/agent/plan/planner/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      156 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/agentuniverse/agent/plan/planner/__init__.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.962818 agentUniverse-0.0.4/agentuniverse/agent/plan/planner/executing_planner/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      157 2024-04-09 16:15:17.000000 agentUniverse-0.0.4/agentuniverse/agent/plan/planner/executing_planner/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1227 2024-04-26 09:03:49.000000 agentUniverse-0.0.4/agentuniverse/agent/plan/planner/executing_planner/default_cn_prompt.yaml
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1421 2024-04-26 09:03:49.000000 agentUniverse-0.0.4/agentuniverse/agent/plan/planner/executing_planner/default_en_prompt.yaml
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     3393 2024-04-26 09:03:49.000000 agentUniverse-0.0.4/agentuniverse/agent/plan/planner/executing_planner/executing_planner.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      195 2024-04-26 03:46:54.000000 agentUniverse-0.0.4/agentuniverse/agent/plan/planner/executing_planner/executing_planner.yaml
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.963840 agentUniverse-0.0.4/agentuniverse/agent/plan/planner/expressing_planner/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      157 2024-04-09 16:15:17.000000 agentUniverse-0.0.4/agentuniverse/agent/plan/planner/expressing_planner/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1471 2024-04-26 09:03:49.000000 agentUniverse-0.0.4/agentuniverse/agent/plan/planner/expressing_planner/default_cn_prompt.yaml
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1841 2024-04-26 09:03:49.000000 agentUniverse-0.0.4/agentuniverse/agent/plan/planner/expressing_planner/default_en_prompt.yaml
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     3330 2024-04-26 09:03:49.000000 agentUniverse-0.0.4/agentuniverse/agent/plan/planner/expressing_planner/expressing_planner.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      200 2024-04-26 03:46:54.000000 agentUniverse-0.0.4/agentuniverse/agent/plan/planner/expressing_planner/expressing_planner.yaml
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.964713 agentUniverse-0.0.4/agentuniverse/agent/plan/planner/peer_planner/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      158 2024-04-09 16:15:17.000000 agentUniverse-0.0.4/agentuniverse/agent/plan/planner/peer_planner/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     8675 2024-04-26 09:03:49.000000 agentUniverse-0.0.4/agentuniverse/agent/plan/planner/peer_planner/peer_planner.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      170 2024-04-26 03:46:54.000000 agentUniverse-0.0.4/agentuniverse/agent/plan/planner/peer_planner/peer_planner.yaml
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     6396 2024-04-26 07:36:14.000000 agentUniverse-0.0.4/agentuniverse/agent/plan/planner/planner.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      659 2024-04-26 03:46:54.000000 agentUniverse-0.0.4/agentuniverse/agent/plan/planner/planner_manager.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.965905 agentUniverse-0.0.4/agentuniverse/agent/plan/planner/planning_planner/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      157 2024-04-09 16:15:17.000000 agentUniverse-0.0.4/agentuniverse/agent/plan/planner/planning_planner/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1315 2024-04-26 09:03:49.000000 agentUniverse-0.0.4/agentuniverse/agent/plan/planner/planning_planner/default_cn_prompt.yaml
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1586 2024-04-26 09:03:49.000000 agentUniverse-0.0.4/agentuniverse/agent/plan/planner/planning_planner/default_en_prompt.yaml
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     3276 2024-04-26 09:03:49.000000 agentUniverse-0.0.4/agentuniverse/agent/plan/planner/planning_planner/planning_planner.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      190 2024-04-26 03:46:54.000000 agentUniverse-0.0.4/agentuniverse/agent/plan/planner/planning_planner/planning_planner.yaml
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.966898 agentUniverse-0.0.4/agentuniverse/agent/plan/planner/rag_planner/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      157 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/agentuniverse/agent/plan/planner/rag_planner/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      741 2024-04-26 09:03:49.000000 agentUniverse-0.0.4/agentuniverse/agent/plan/planner/rag_planner/default_cn_prompt.yaml
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      859 2024-04-26 09:03:49.000000 agentUniverse-0.0.4/agentuniverse/agent/plan/planner/rag_planner/default_en_prompt.yaml
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     3074 2024-04-26 09:03:49.000000 agentUniverse-0.0.4/agentuniverse/agent/plan/planner/rag_planner/rag_planner.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      165 2024-04-26 03:46:54.000000 agentUniverse-0.0.4/agentuniverse/agent/plan/planner/rag_planner/rag_planner.yaml
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.967825 agentUniverse-0.0.4/agentuniverse/agent/plan/planner/reviewing_planner/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      157 2024-04-09 16:15:17.000000 agentUniverse-0.0.4/agentuniverse/agent/plan/planner/reviewing_planner/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1194 2024-04-26 09:03:49.000000 agentUniverse-0.0.4/agentuniverse/agent/plan/planner/reviewing_planner/default_cn_prompt.yaml
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1387 2024-04-26 09:03:49.000000 agentUniverse-0.0.4/agentuniverse/agent/plan/planner/reviewing_planner/default_en_prompt.yaml
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     3331 2024-04-26 09:03:49.000000 agentUniverse-0.0.4/agentuniverse/agent/plan/planner/reviewing_planner/reviewing_planner.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      195 2024-04-26 03:46:54.000000 agentUniverse-0.0.4/agentuniverse/agent/plan/planner/reviewing_planner/reviewing_planner.yaml
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.968896 agentUniverse-0.0.4/agentuniverse/agent_serve/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)        0 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/agentuniverse/agent_serve/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1944 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/agentuniverse/agent_serve/service.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     3152 2024-04-26 03:46:54.000000 agentUniverse-0.0.4/agentuniverse/agent_serve/service_configer.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1161 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/agentuniverse/agent_serve/service_instance.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      402 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/agentuniverse/agent_serve/service_manager.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.970768 agentUniverse-0.0.4/agentuniverse/agent_serve/web/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/agentuniverse/agent_serve/web/__init__.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.971202 agentUniverse-0.0.4/agentuniverse/agent_serve/web/dal/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/agentuniverse/agent_serve/web/dal/__init__.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.971690 agentUniverse-0.0.4/agentuniverse/agent_serve/web/dal/entity/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/agentuniverse/agent_serve/web/dal/entity/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1075 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/agentuniverse/agent_serve/web/dal/entity/request_do.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     5473 2024-04-26 09:28:07.000000 agentUniverse-0.0.4/agentuniverse/agent_serve/web/dal/request_library.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     5327 2024-04-26 09:28:07.000000 agentUniverse-0.0.4/agentuniverse/agent_serve/web/flask_server.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     2351 2024-04-26 09:28:07.000000 agentUniverse-0.0.4/agentuniverse/agent_serve/web/gunicorn_server.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     9311 2024-04-26 09:03:49.000000 agentUniverse-0.0.4/agentuniverse/agent_serve/web/request_task.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.972159 agentUniverse-0.0.4/agentuniverse/agent_serve/web/rpc/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-26 09:03:49.000000 agentUniverse-0.0.4/agentuniverse/agent_serve/web/rpc/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1224 2024-04-26 09:03:49.000000 agentUniverse-0.0.4/agentuniverse/agent_serve/web/rpc/rpc_server.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1146 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/agentuniverse/agent_serve/web/thread_with_result.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      822 2024-04-26 09:28:07.000000 agentUniverse-0.0.4/agentuniverse/agent_serve/web/web_booster.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     2679 2024-04-26 09:28:07.000000 agentUniverse-0.0.4/agentuniverse/agent_serve/web/web_util.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.972573 agentUniverse-0.0.4/agentuniverse/base/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/agentuniverse/base/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)    10614 2024-04-26 09:28:07.000000 agentUniverse-0.0.4/agentuniverse/base/agentuniverse.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.973044 agentUniverse-0.0.4/agentuniverse/base/annotation/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/agentuniverse/base/annotation/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      515 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/agentuniverse/base/annotation/singleton.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.974530 agentUniverse-0.0.4/agentuniverse/base/component/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/agentuniverse/base/component/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1081 2024-04-26 03:46:54.000000 agentUniverse-0.0.4/agentuniverse/base/component/application_component_manager.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1264 2024-04-26 03:46:54.000000 agentUniverse-0.0.4/agentuniverse/base/component/component_base.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     4380 2024-04-26 09:03:49.000000 agentUniverse-0.0.4/agentuniverse/base/component/component_configer_util.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      626 2024-04-26 09:03:49.000000 agentUniverse-0.0.4/agentuniverse/base/component/component_enum.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     2576 2024-04-26 03:46:54.000000 agentUniverse-0.0.4/agentuniverse/base/component/component_manager_base.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.975498 agentUniverse-0.0.4/agentuniverse/base/config/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/agentuniverse/base/config/__init__.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.976476 agentUniverse-0.0.4/agentuniverse/base/config/application_configer/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      165 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/agentuniverse/base/config/application_configer/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     4173 2024-04-26 09:03:49.000000 agentUniverse-0.0.4/agentuniverse/base/config/application_configer/app_configer.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1006 2024-04-26 03:46:54.000000 agentUniverse-0.0.4/agentuniverse/base/config/application_configer/application_config_manager.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.977774 agentUniverse-0.0.4/agentuniverse/base/config/component_configer/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      165 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/agentuniverse/base/config/component_configer/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     2811 2024-04-26 09:03:49.000000 agentUniverse-0.0.4/agentuniverse/base/config/component_configer/component_configer.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.980164 agentUniverse-0.0.4/agentuniverse/base/config/component_configer/configers/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      165 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/agentuniverse/base/config/component_configer/configers/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     2599 2024-04-26 03:46:54.000000 agentUniverse-0.0.4/agentuniverse/base/config/component_configer/configers/agent_configer.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     2053 2024-04-26 03:46:54.000000 agentUniverse-0.0.4/agentuniverse/base/config/component_configer/configers/knowledge_configer.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     3272 2024-04-26 03:46:54.000000 agentUniverse-0.0.4/agentuniverse/base/config/component_configer/configers/llm_configer.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     2540 2024-04-26 03:46:54.000000 agentUniverse-0.0.4/agentuniverse/base/config/component_configer/configers/memory_configer.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     2392 2024-04-26 03:46:54.000000 agentUniverse-0.0.4/agentuniverse/base/config/component_configer/configers/planner_configer.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1889 2024-04-26 09:03:49.000000 agentUniverse-0.0.4/agentuniverse/base/config/component_configer/configers/prompt_configer.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     2192 2024-04-26 03:46:54.000000 agentUniverse-0.0.4/agentuniverse/base/config/component_configer/configers/tool_configer.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      423 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/agentuniverse/base/config/config_type_enum.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     4846 2024-04-26 09:28:07.000000 agentUniverse-0.0.4/agentuniverse/base/config/configer.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.980684 agentUniverse-0.0.4/agentuniverse/base/config/custom_configer/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      163 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/agentuniverse/base/config/custom_configer/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      707 2024-04-26 03:55:12.000000 agentUniverse-0.0.4/agentuniverse/base/config/custom_configer/custom_key_configer.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.981491 agentUniverse-0.0.4/agentuniverse/base/context/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/agentuniverse/base/context/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1447 2024-04-26 03:46:54.000000 agentUniverse-0.0.4/agentuniverse/base/context/framework_context.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     2768 2024-04-26 03:46:54.000000 agentUniverse-0.0.4/agentuniverse/base/context/framework_context_manager.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.982816 agentUniverse-0.0.4/agentuniverse/base/prompt/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      174 2024-04-26 09:03:49.000000 agentUniverse-0.0.4/agentuniverse/base/prompt/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      286 2024-04-26 09:03:49.000000 agentUniverse-0.0.4/agentuniverse/base/prompt/combine_cn_prompt.yaml
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      318 2024-04-26 09:03:49.000000 agentUniverse-0.0.4/agentuniverse/base/prompt/combine_en_prompt.yaml
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      253 2024-04-26 09:03:49.000000 agentUniverse-0.0.4/agentuniverse/base/prompt/summary_cn_prompt.yaml
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      272 2024-04-26 09:03:49.000000 agentUniverse-0.0.4/agentuniverse/base/prompt/summary_en_prompt.yaml
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.984168 agentUniverse-0.0.4/agentuniverse/base/util/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/agentuniverse/base/util/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      307 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/agentuniverse/base/util/env_util.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.985307 agentUniverse-0.0.4/agentuniverse/base/util/logging/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/agentuniverse/base/util/logging/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     6600 2024-04-26 03:42:29.000000 agentUniverse-0.0.4/agentuniverse/base/util/logging/general_logger.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     5132 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/agentuniverse/base/util/logging/logging_config.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     6395 2024-04-26 03:42:21.000000 agentUniverse-0.0.4/agentuniverse/base/util/logging/logging_util.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      502 2024-04-26 03:42:41.000000 agentUniverse-0.0.4/agentuniverse/base/util/memory_util.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     6644 2024-04-26 09:03:49.000000 agentUniverse-0.0.4/agentuniverse/base/util/prompt_util.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      715 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/agentuniverse/base/util/system_util.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.986802 agentUniverse-0.0.4/agentuniverse/llm/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/agentuniverse/llm/__init__.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.987443 agentUniverse-0.0.4/agentuniverse/llm/default/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/agentuniverse/llm/default/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1352 2024-04-26 09:03:49.000000 agentUniverse-0.0.4/agentuniverse/llm/default/default_openai_llm.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      223 2024-04-26 09:03:49.000000 agentUniverse-0.0.4/agentuniverse/llm/default/default_openai_llm.yaml
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     2892 2024-04-26 09:03:49.000000 agentUniverse-0.0.4/agentuniverse/llm/langchain_instance.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     5508 2024-04-26 09:03:49.000000 agentUniverse-0.0.4/agentuniverse/llm/llm.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      619 2024-04-26 03:46:54.000000 agentUniverse-0.0.4/agentuniverse/llm/llm_manager.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      408 2024-04-26 09:03:49.000000 agentUniverse-0.0.4/agentuniverse/llm/llm_output.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     6482 2024-04-26 09:03:49.000000 agentUniverse-0.0.4/agentuniverse/llm/openai_llm.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.988521 agentUniverse-0.0.4/agentuniverse/prompt/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      156 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/agentuniverse/prompt/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      548 2024-04-26 07:36:14.000000 agentUniverse-0.0.4/agentuniverse/prompt/enum.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     3105 2024-04-26 09:03:49.000000 agentUniverse-0.0.4/agentuniverse/prompt/prompt.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      741 2024-04-26 09:03:49.000000 agentUniverse-0.0.4/agentuniverse/prompt/prompt_manager.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      834 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/agentuniverse/prompt/prompt_model.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.988691 agentUniverse-0.0.4/agentuniverse_connector/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 03:12:13.000000 agentUniverse-0.0.4/agentuniverse_connector/__init__.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.988967 agentUniverse-0.0.4/agentuniverse_extension/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 03:13:12.000000 agentUniverse-0.0.4/agentuniverse_extension/__init__.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.989401 agentUniverse-0.0.4/agentuniverse_extension/logger/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/agentuniverse_extension/logger/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     7321 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/agentuniverse_extension/logger/sls_sink.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     2162 2024-04-26 09:31:08.000000 agentUniverse-0.0.4/pyproject.toml
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.989590 agentUniverse-0.0.4/sample_standard_app/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-24 09:17:13.000000 agentUniverse-0.0.4/sample_standard_app/__init__.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.989863 agentUniverse-0.0.4/sample_standard_app/app/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-24 09:17:13.000000 agentUniverse-0.0.4/sample_standard_app/app/__init__.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.990118 agentUniverse-0.0.4/sample_standard_app/app/biz/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-24 09:17:13.000000 agentUniverse-0.0.4/sample_standard_app/app/biz/__init__.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.990521 agentUniverse-0.0.4/sample_standard_app/app/bootstrap/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-24 09:17:13.000000 agentUniverse-0.0.4/sample_standard_app/app/bootstrap/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      524 2024-04-24 09:17:13.000000 agentUniverse-0.0.4/sample_standard_app/app/bootstrap/server_application.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.990718 agentUniverse-0.0.4/sample_standard_app/app/core/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-24 09:17:13.000000 agentUniverse-0.0.4/sample_standard_app/app/core/__init__.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.990900 agentUniverse-0.0.4/sample_standard_app/app/core/agent/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-24 09:17:13.000000 agentUniverse-0.0.4/sample_standard_app/app/core/agent/__init__.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.992327 agentUniverse-0.0.4/sample_standard_app/app/core/agent/peer_agent_case/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-24 09:17:13.000000 agentUniverse-0.0.4/sample_standard_app/app/core/agent/peer_agent_case/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1360 2024-04-24 09:17:13.000000 agentUniverse-0.0.4/sample_standard_app/app/core/agent/peer_agent_case/demo_executing_agent.yaml
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1562 2024-04-24 09:17:13.000000 agentUniverse-0.0.4/sample_standard_app/app/core/agent/peer_agent_case/demo_expressing_agent.yaml
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      793 2024-04-24 09:17:13.000000 agentUniverse-0.0.4/sample_standard_app/app/core/agent/peer_agent_case/demo_peer_agent.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      430 2024-04-24 09:17:13.000000 agentUniverse-0.0.4/sample_standard_app/app/core/agent/peer_agent_case/demo_peer_agent.yaml
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      485 2024-04-24 09:17:13.000000 agentUniverse-0.0.4/sample_standard_app/app/core/agent/peer_agent_case/demo_planning_agent.yaml
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      325 2024-04-24 09:17:13.000000 agentUniverse-0.0.4/sample_standard_app/app/core/agent/peer_agent_case/demo_reviewing_agent.yaml
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.992956 agentUniverse-0.0.4/sample_standard_app/app/core/agent/rag_agent_case/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-24 09:17:13.000000 agentUniverse-0.0.4/sample_standard_app/app/core/agent/rag_agent_case/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      725 2024-04-24 09:17:13.000000 agentUniverse-0.0.4/sample_standard_app/app/core/agent/rag_agent_case/demo_rag_agent.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      341 2024-04-24 09:17:13.000000 agentUniverse-0.0.4/sample_standard_app/app/core/agent/rag_agent_case/demo_rag_agent.yaml
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.993501 agentUniverse-0.0.4/sample_standard_app/app/core/knowledge/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-24 09:17:13.000000 agentUniverse-0.0.4/sample_standard_app/app/core/knowledge/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     2474 2024-04-24 09:17:13.000000 agentUniverse-0.0.4/sample_standard_app/app/core/knowledge/demo_knowledge.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-04-24 09:17:13.000000 agentUniverse-0.0.4/sample_standard_app/app/core/knowledge/demo_knowledge.yaml
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.993856 agentUniverse-0.0.4/sample_standard_app/app/core/llm/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-24 09:17:13.000000 agentUniverse-0.0.4/sample_standard_app/app/core/llm/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      212 2024-04-24 09:17:13.000000 agentUniverse-0.0.4/sample_standard_app/app/core/llm/demo_llm.yaml
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.994032 agentUniverse-0.0.4/sample_standard_app/app/core/memory/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-24 09:17:13.000000 agentUniverse-0.0.4/sample_standard_app/app/core/memory/__init__.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.994221 agentUniverse-0.0.4/sample_standard_app/app/core/planner/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-24 09:17:13.000000 agentUniverse-0.0.4/sample_standard_app/app/core/planner/__init__.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.994573 agentUniverse-0.0.4/sample_standard_app/app/core/service/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-04-24 09:17:13.000000 agentUniverse-0.0.4/sample_standard_app/app/core/service/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      114 2024-04-24 09:17:13.000000 agentUniverse-0.0.4/sample_standard_app/app/core/service/demo_service.yaml
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.995177 agentUniverse-0.0.4/sample_standard_app/app/core/tool/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-24 09:17:13.000000 agentUniverse-0.0.4/sample_standard_app/app/core/tool/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      857 2024-04-24 09:17:13.000000 agentUniverse-0.0.4/sample_standard_app/app/core/tool/demo_tool.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      182 2024-04-24 09:17:13.000000 agentUniverse-0.0.4/sample_standard_app/app/core/tool/demo_tool.yaml
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.995909 agentUniverse-0.0.4/sample_standard_app/app/test/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-24 09:17:13.000000 agentUniverse-0.0.4/sample_standard_app/app/test/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)    15065 2024-04-24 09:17:13.000000 agentUniverse-0.0.4/sample_standard_app/app/test/test_peer_agents.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      943 2024-04-24 09:17:13.000000 agentUniverse-0.0.4/sample_standard_app/app/test/test_rag_agent.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      325 2024-04-24 09:17:13.000000 agentUniverse-0.0.4/sample_standard_app/app/test/test_server_application.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.996092 agentUniverse-0.0.4/sample_standard_app/app/web/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-24 09:17:13.000000 agentUniverse-0.0.4/sample_standard_app/app/web/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)       38 2024-04-26 09:36:05.006405 agentUniverse-0.0.4/setup.cfg
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1176 2024-04-26 09:31:08.000000 agentUniverse-0.0.4/setup.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.996261 agentUniverse-0.0.4/tests/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 03:13:12.000000 agentUniverse-0.0.4/tests/__init__.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.996608 agentUniverse-0.0.4/tests/test_agentuniverse/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/tests/test_agentuniverse/__init__.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.996913 agentUniverse-0.0.4/tests/test_agentuniverse/mock/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      163 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/tests/test_agentuniverse/mock/__init__.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.998167 agentUniverse-0.0.4/tests/test_agentuniverse/mock/agent_serve/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-26 09:03:49.000000 agentUniverse-0.0.4/tests/test_agentuniverse/mock/agent_serve/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      535 2024-04-26 09:03:49.000000 agentUniverse-0.0.4/tests/test_agentuniverse/mock/agent_serve/mock_agent.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      475 2024-04-26 09:03:49.000000 agentUniverse-0.0.4/tests/test_agentuniverse/mock/agent_serve/mock_application_config_manager.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      896 2024-04-26 09:03:49.000000 agentUniverse-0.0.4/tests/test_agentuniverse/mock/agent_serve/mock_service_manager.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      509 2024-04-26 09:03:49.000000 agentUniverse-0.0.4/tests/test_agentuniverse/mock/agent_serve/mock_simple_service.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.998375 agentUniverse-0.0.4/tests/test_agentuniverse/unit/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      163 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/tests/test_agentuniverse/unit/__init__.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.998849 agentUniverse-0.0.4/tests/test_agentuniverse/unit/agent/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/tests/test_agentuniverse/unit/agent/__init__.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.999108 agentUniverse-0.0.4/tests/test_agentuniverse/unit/agent/action/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/tests/test_agentuniverse/unit/agent/action/__init__.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.999502 agentUniverse-0.0.4/tests/test_agentuniverse/unit/agent/action/knowledge/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/tests/test_agentuniverse/unit/agent/action/knowledge/__init__.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:04.999991 agentUniverse-0.0.4/tests/test_agentuniverse/unit/agent/action/knowledge/embedding/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/tests/test_agentuniverse/unit/agent/action/knowledge/embedding/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1097 2024-04-19 04:33:11.000000 agentUniverse-0.0.4/tests/test_agentuniverse/unit/agent/action/knowledge/embedding/test_embedding.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1566 2024-04-19 04:33:11.000000 agentUniverse-0.0.4/tests/test_agentuniverse/unit/agent/action/knowledge/test_knowledge.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:05.000460 agentUniverse-0.0.4/tests/test_agentuniverse/unit/agent/memory/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/tests/test_agentuniverse/unit/agent/memory/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     3894 2024-04-19 04:33:11.000000 agentUniverse-0.0.4/tests/test_agentuniverse/unit/agent/memory/test_memory.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      820 2024-04-26 09:28:07.000000 agentUniverse-0.0.4/tests/test_agentuniverse/unit/agent/test_rag_agent.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:05.002005 agentUniverse-0.0.4/tests/test_agentuniverse/unit/agent_serve/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      163 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/tests/test_agentuniverse/unit/agent_serve/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1237 2024-04-19 04:34:47.000000 agentUniverse-0.0.4/tests/test_agentuniverse/unit/agent_serve/test_service.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      920 2024-04-19 04:34:47.000000 agentUniverse-0.0.4/tests/test_agentuniverse/unit/agent_serve/test_service_instance.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1613 2024-04-19 04:34:47.000000 agentUniverse-0.0.4/tests/test_agentuniverse/unit/agent_serve/test_service_manager.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      390 2024-04-26 09:28:07.000000 agentUniverse-0.0.4/tests/test_agentuniverse/unit/agent_serve/test_web_booster.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:05.002240 agentUniverse-0.0.4/tests/test_agentuniverse/unit/base/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      163 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/tests/test_agentuniverse/unit/base/__init__.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:05.002761 agentUniverse-0.0.4/tests/test_agentuniverse/unit/base/context/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      163 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/tests/test_agentuniverse/unit/base/context/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1442 2024-04-19 04:34:47.000000 agentUniverse-0.0.4/tests/test_agentuniverse/unit/base/context/test_framework_context.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:05.003039 agentUniverse-0.0.4/tests/test_agentuniverse/unit/base/util/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      163 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/tests/test_agentuniverse/unit/base/util/__init__.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:05.003387 agentUniverse-0.0.4/tests/test_agentuniverse/unit/base/util/logging/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      163 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/tests/test_agentuniverse/unit/base/util/logging/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1670 2024-04-19 04:33:11.000000 agentUniverse-0.0.4/tests/test_agentuniverse/unit/base/util/logging/test_logging_util.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:05.003833 agentUniverse-0.0.4/tests/test_agentuniverse/unit/llm/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/tests/test_agentuniverse/unit/llm/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1264 2024-04-19 04:33:11.000000 agentUniverse-0.0.4/tests/test_agentuniverse/unit/llm/test_llm.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:05.004091 agentUniverse-0.0.4/tests/test_agentuniverse_connector/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/tests/test_agentuniverse_connector/__init__.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:05.004257 agentUniverse-0.0.4/tests/test_agentuniverse_extension/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/tests/test_agentuniverse_extension/__init__.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:05.004419 agentUniverse-0.0.4/tests/test_agentuniverse_extension/mock/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      163 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/tests/test_agentuniverse_extension/mock/__init__.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:05.004819 agentUniverse-0.0.4/tests/test_agentuniverse_extension/mock/logger/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      163 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/tests/test_agentuniverse_extension/mock/logger/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      620 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/tests/test_agentuniverse_extension/mock/logger/mock_log_client.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:05.004992 agentUniverse-0.0.4/tests/test_agentuniverse_extension/unit/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      163 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/tests/test_agentuniverse_extension/unit/__init__.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-26 09:36:05.005379 agentUniverse-0.0.4/tests/test_agentuniverse_extension/unit/logger/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      163 2024-04-02 12:08:01.000000 agentUniverse-0.0.4/tests/test_agentuniverse_extension/unit/logger/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1288 2024-04-19 04:49:33.000000 agentUniverse-0.0.4/tests/test_agentuniverse_extension/unit/logger/test_sls_sink.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-05-08 15:59:53.719728 agentuniverse-0.0.5/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     2560 2024-05-08 14:09:08.000000 agentuniverse-0.0.5/CHANGELOG.md
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     2183 2024-05-08 14:07:58.000000 agentuniverse-0.0.5/CHANGELOG_zh.md
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)    11335 2024-04-02 12:08:01.000000 agentuniverse-0.0.5/LICENSE
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      304 2024-05-08 15:07:57.000000 agentuniverse-0.0.5/MANIFEST.in
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     2633 2024-05-08 15:59:53.719138 agentuniverse-0.0.5/PKG-INFO
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     3210 2024-05-07 11:44:48.000000 agentuniverse-0.0.5/README.md
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     2908 2024-05-07 11:44:48.000000 agentuniverse-0.0.5/README_zh.md
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-05-08 15:59:53.718674 agentuniverse-0.0.5/agentUniverse.egg-info/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     2633 2024-05-08 15:59:53.000000 agentuniverse-0.0.5/agentUniverse.egg-info/PKG-INFO
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     9373 2024-05-08 15:59:53.000000 agentuniverse-0.0.5/agentUniverse.egg-info/SOURCES.txt
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)        1 2024-05-08 15:59:53.000000 agentuniverse-0.0.5/agentUniverse.egg-info/dependency_links.txt
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      324 2024-05-08 15:59:53.000000 agentuniverse-0.0.5/agentUniverse.egg-info/requires.txt
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)       62 2024-05-08 15:59:53.000000 agentuniverse-0.0.5/agentUniverse.egg-info/top_level.txt
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-05-08 15:59:53.662506 agentuniverse-0.0.5/agentuniverse/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 03:12:13.000000 agentuniverse-0.0.5/agentuniverse/__init__.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-05-08 15:59:53.663708 agentuniverse-0.0.5/agentuniverse/agent/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentuniverse-0.0.5/agentuniverse/agent/__init__.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-05-08 15:59:53.663886 agentuniverse-0.0.5/agentuniverse/agent/action/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-04-02 12:08:01.000000 agentuniverse-0.0.5/agentuniverse/agent/action/__init__.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-05-08 15:59:53.664363 agentuniverse-0.0.5/agentuniverse/agent/action/knowledge/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-04-02 12:08:01.000000 agentuniverse-0.0.5/agentuniverse/agent/action/knowledge/__init__.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-05-08 15:59:53.664835 agentuniverse-0.0.5/agentuniverse/agent/action/knowledge/embedding/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-04-02 12:08:01.000000 agentuniverse-0.0.5/agentuniverse/agent/action/knowledge/embedding/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      972 2024-04-26 07:36:14.000000 agentuniverse-0.0.5/agentuniverse/agent/action/knowledge/embedding/embedding.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     4270 2024-05-07 11:44:48.000000 agentuniverse-0.0.5/agentuniverse/agent/action/knowledge/embedding/openai_embedding.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     3097 2024-04-26 03:46:54.000000 agentuniverse-0.0.5/agentuniverse/agent/action/knowledge/knowledge.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      655 2024-04-26 03:46:54.000000 agentuniverse-0.0.5/agentuniverse/agent/action/knowledge/knowledge_manager.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-05-08 15:59:53.665150 agentuniverse-0.0.5/agentuniverse/agent/action/knowledge/reader/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-04-02 12:08:01.000000 agentuniverse-0.0.5/agentuniverse/agent/action/knowledge/reader/__init__.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-05-08 15:59:53.666084 agentuniverse-0.0.5/agentuniverse/agent/action/knowledge/reader/file/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-04-02 12:08:01.000000 agentuniverse-0.0.5/agentuniverse/agent/action/knowledge/reader/file/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1160 2024-04-26 03:46:54.000000 agentuniverse-0.0.5/agentuniverse/agent/action/knowledge/reader/file/docx_reader.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1651 2024-04-26 07:36:14.000000 agentuniverse-0.0.5/agentuniverse/agent/action/knowledge/reader/file/file_reader.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1568 2024-04-26 03:46:54.000000 agentuniverse-0.0.5/agentuniverse/agent/action/knowledge/reader/file/pdf_reader.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1460 2024-04-26 03:46:54.000000 agentuniverse-0.0.5/agentuniverse/agent/action/knowledge/reader/file/pptx_reader.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1478 2024-04-26 07:36:14.000000 agentuniverse-0.0.5/agentuniverse/agent/action/knowledge/reader/file/web_pdf_reader.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      552 2024-04-26 03:46:54.000000 agentuniverse-0.0.5/agentuniverse/agent/action/knowledge/reader/reader.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-05-08 15:59:53.666861 agentuniverse-0.0.5/agentuniverse/agent/action/knowledge/store/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-04-02 12:08:01.000000 agentuniverse-0.0.5/agentuniverse/agent/action/knowledge/store/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     5872 2024-05-07 11:44:48.000000 agentuniverse-0.0.5/agentuniverse/agent/action/knowledge/store/chroma_store.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     2206 2024-05-07 11:44:48.000000 agentuniverse-0.0.5/agentuniverse/agent/action/knowledge/store/document.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      662 2024-04-02 12:08:01.000000 agentuniverse-0.0.5/agentuniverse/agent/action/knowledge/store/query.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     3842 2024-05-07 11:44:48.000000 agentuniverse-0.0.5/agentuniverse/agent/action/knowledge/store/store.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-05-08 15:59:53.667475 agentuniverse-0.0.5/agentuniverse/agent/action/tool/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-04-02 12:08:01.000000 agentuniverse-0.0.5/agentuniverse/agent/action/tool/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      276 2024-04-02 12:08:01.000000 agentuniverse-0.0.5/agentuniverse/agent/action/tool/enum.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     3868 2024-04-26 07:36:14.000000 agentuniverse-0.0.5/agentuniverse/agent/action/tool/tool.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      626 2024-04-26 03:46:54.000000 agentuniverse-0.0.5/agentuniverse/agent/action/tool/tool_manager.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     5469 2024-05-08 13:44:50.000000 agentuniverse-0.0.5/agentuniverse/agent/agent.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      639 2024-04-26 03:44:12.000000 agentuniverse-0.0.5/agentuniverse/agent/agent_manager.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      526 2024-04-02 12:08:01.000000 agentuniverse-0.0.5/agentuniverse/agent/agent_model.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-05-08 15:59:53.667631 agentuniverse-0.0.5/agentuniverse/agent/default/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      156 2024-04-02 12:08:01.000000 agentuniverse-0.0.5/agentuniverse/agent/default/__init__.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-05-08 15:59:53.668760 agentuniverse-0.0.5/agentuniverse/agent/default/executing_agent/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-05-08 13:44:50.000000 agentuniverse-0.0.5/agentuniverse/agent/default/executing_agent/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1257 2024-05-08 13:44:50.000000 agentuniverse-0.0.5/agentuniverse/agent/default/executing_agent/default_cn_prompt.yaml
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1446 2024-05-08 13:44:50.000000 agentuniverse-0.0.5/agentuniverse/agent/default/executing_agent/default_en_prompt.yaml
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     3126 2024-05-08 13:44:50.000000 agentuniverse-0.0.5/agentuniverse/agent/default/executing_agent/executing_agent.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      367 2024-05-08 13:44:50.000000 agentuniverse-0.0.5/agentuniverse/agent/default/executing_agent/executing_agent.yaml
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-05-08 15:59:53.669575 agentuniverse-0.0.5/agentuniverse/agent/default/expressing_agent/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-05-08 13:44:50.000000 agentuniverse-0.0.5/agentuniverse/agent/default/expressing_agent/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1499 2024-05-08 13:44:50.000000 agentuniverse-0.0.5/agentuniverse/agent/default/expressing_agent/default_cn_prompt.yaml
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1866 2024-05-08 13:44:50.000000 agentuniverse-0.0.5/agentuniverse/agent/default/expressing_agent/default_en_prompt.yaml
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     2030 2024-05-08 13:44:50.000000 agentuniverse-0.0.5/agentuniverse/agent/default/expressing_agent/expressing_agent.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      365 2024-05-08 13:44:50.000000 agentuniverse-0.0.5/agentuniverse/agent/default/expressing_agent/expressing_agent.yaml
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-05-08 15:59:53.670039 agentuniverse-0.0.5/agentuniverse/agent/default/peer_agent/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-05-08 13:44:50.000000 agentuniverse-0.0.5/agentuniverse/agent/default/peer_agent/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1289 2024-05-08 13:44:50.000000 agentuniverse-0.0.5/agentuniverse/agent/default/peer_agent/peer_agent.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      374 2024-05-08 13:44:50.000000 agentuniverse-0.0.5/agentuniverse/agent/default/peer_agent/peer_agent.yaml
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-05-08 15:59:53.670805 agentuniverse-0.0.5/agentuniverse/agent/default/planning_agent/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-05-08 13:44:50.000000 agentuniverse-0.0.5/agentuniverse/agent/default/planning_agent/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1343 2024-05-08 13:44:50.000000 agentuniverse-0.0.5/agentuniverse/agent/default/planning_agent/default_cn_prompt.yaml
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1613 2024-05-08 13:44:50.000000 agentuniverse-0.0.5/agentuniverse/agent/default/planning_agent/default_en_prompt.yaml
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1623 2024-05-08 13:44:50.000000 agentuniverse-0.0.5/agentuniverse/agent/default/planning_agent/planning_agent.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      353 2024-05-08 13:44:50.000000 agentuniverse-0.0.5/agentuniverse/agent/default/planning_agent/planning_agent.yaml
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-05-08 15:59:53.671564 agentuniverse-0.0.5/agentuniverse/agent/default/rag_agent/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-05-08 13:44:50.000000 agentuniverse-0.0.5/agentuniverse/agent/default/rag_agent/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      769 2024-05-08 13:44:50.000000 agentuniverse-0.0.5/agentuniverse/agent/default/rag_agent/default_cn_prompt.yaml
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      884 2024-05-08 13:44:50.000000 agentuniverse-0.0.5/agentuniverse/agent/default/rag_agent/default_en_prompt.yaml
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1333 2024-05-08 13:44:50.000000 agentuniverse-0.0.5/agentuniverse/agent/default/rag_agent/rag_agent.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      276 2024-05-08 13:44:50.000000 agentuniverse-0.0.5/agentuniverse/agent/default/rag_agent/rag_agent.yaml
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-05-08 15:59:53.672317 agentuniverse-0.0.5/agentuniverse/agent/default/reviewing_agent/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-05-08 13:44:50.000000 agentuniverse-0.0.5/agentuniverse/agent/default/reviewing_agent/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1222 2024-05-08 13:44:50.000000 agentuniverse-0.0.5/agentuniverse/agent/default/reviewing_agent/default_cn_prompt.yaml
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1412 2024-05-08 13:44:50.000000 agentuniverse-0.0.5/agentuniverse/agent/default/reviewing_agent/default_en_prompt.yaml
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1954 2024-05-08 13:44:50.000000 agentuniverse-0.0.5/agentuniverse/agent/default/reviewing_agent/reviewing_agent.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      359 2024-05-08 13:44:50.000000 agentuniverse-0.0.5/agentuniverse/agent/default/reviewing_agent/reviewing_agent.yaml
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      657 2024-04-02 12:08:01.000000 agentuniverse-0.0.5/agentuniverse/agent/input_object.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-05-08 15:59:53.674184 agentuniverse-0.0.5/agentuniverse/agent/memory/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-04-09 07:08:39.000000 agentuniverse-0.0.5/agentuniverse/agent/memory/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     3907 2024-04-26 09:03:49.000000 agentuniverse-0.0.5/agentuniverse/agent/memory/chat_memory.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-05-08 15:59:53.674696 agentuniverse-0.0.5/agentuniverse/agent/memory/default/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      174 2024-04-26 09:03:49.000000 agentuniverse-0.0.5/agentuniverse/agent/memory/default/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      845 2024-04-26 09:03:49.000000 agentuniverse-0.0.5/agentuniverse/agent/memory/default/default_memory.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      321 2024-04-26 09:03:49.000000 agentuniverse-0.0.5/agentuniverse/agent/memory/default/default_memory.yaml
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      402 2024-04-01 06:19:56.000000 agentuniverse-0.0.5/agentuniverse/agent/memory/enum.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     7689 2024-04-26 09:03:49.000000 agentuniverse-0.0.5/agentuniverse/agent/memory/langchain_instance.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     3054 2024-04-26 07:36:14.000000 agentuniverse-0.0.5/agentuniverse/agent/memory/memory.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      635 2024-04-26 03:46:54.000000 agentuniverse-0.0.5/agentuniverse/agent/memory/memory_manager.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      508 2024-04-09 16:15:17.000000 agentuniverse-0.0.5/agentuniverse/agent/memory/message.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      754 2024-04-26 09:03:49.000000 agentuniverse-0.0.5/agentuniverse/agent/memory/summarizer_cn_prompt.yaml
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      896 2024-04-26 09:03:49.000000 agentuniverse-0.0.5/agentuniverse/agent/memory/summarizer_en_prompt.yaml
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      572 2024-04-02 12:08:01.000000 agentuniverse-0.0.5/agentuniverse/agent/output_object.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-05-08 15:59:53.674862 agentuniverse-0.0.5/agentuniverse/agent/plan/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      156 2024-04-02 12:08:01.000000 agentuniverse-0.0.5/agentuniverse/agent/plan/__init__.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-05-08 15:59:53.675352 agentuniverse-0.0.5/agentuniverse/agent/plan/planner/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      156 2024-04-02 12:08:01.000000 agentuniverse-0.0.5/agentuniverse/agent/plan/planner/__init__.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-05-08 15:59:53.675837 agentuniverse-0.0.5/agentuniverse/agent/plan/planner/executing_planner/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      157 2024-04-09 16:15:17.000000 agentuniverse-0.0.5/agentuniverse/agent/plan/planner/executing_planner/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     3670 2024-05-08 13:44:50.000000 agentuniverse-0.0.5/agentuniverse/agent/plan/planner/executing_planner/executing_planner.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      195 2024-04-26 03:46:54.000000 agentuniverse-0.0.5/agentuniverse/agent/plan/planner/executing_planner/executing_planner.yaml
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-05-08 15:59:53.676319 agentuniverse-0.0.5/agentuniverse/agent/plan/planner/expressing_planner/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      157 2024-04-09 16:15:17.000000 agentuniverse-0.0.5/agentuniverse/agent/plan/planner/expressing_planner/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     3599 2024-05-08 13:44:50.000000 agentuniverse-0.0.5/agentuniverse/agent/plan/planner/expressing_planner/expressing_planner.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      200 2024-04-26 03:46:54.000000 agentuniverse-0.0.5/agentuniverse/agent/plan/planner/expressing_planner/expressing_planner.yaml
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-05-08 15:59:53.676832 agentuniverse-0.0.5/agentuniverse/agent/plan/planner/peer_planner/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      158 2024-04-09 16:15:17.000000 agentuniverse-0.0.5/agentuniverse/agent/plan/planner/peer_planner/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     8919 2024-05-08 13:44:50.000000 agentuniverse-0.0.5/agentuniverse/agent/plan/planner/peer_planner/peer_planner.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      170 2024-04-26 03:46:54.000000 agentuniverse-0.0.5/agentuniverse/agent/plan/planner/peer_planner/peer_planner.yaml
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     6438 2024-05-08 13:44:50.000000 agentuniverse-0.0.5/agentuniverse/agent/plan/planner/planner.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      659 2024-04-26 03:46:54.000000 agentuniverse-0.0.5/agentuniverse/agent/plan/planner/planner_manager.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-05-08 15:59:53.677311 agentuniverse-0.0.5/agentuniverse/agent/plan/planner/planning_planner/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      157 2024-04-09 16:15:17.000000 agentuniverse-0.0.5/agentuniverse/agent/plan/planner/planning_planner/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     3599 2024-05-08 13:44:50.000000 agentuniverse-0.0.5/agentuniverse/agent/plan/planner/planning_planner/planning_planner.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      190 2024-04-26 03:46:54.000000 agentuniverse-0.0.5/agentuniverse/agent/plan/planner/planning_planner/planning_planner.yaml
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-05-08 15:59:53.677797 agentuniverse-0.0.5/agentuniverse/agent/plan/planner/rag_planner/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      157 2024-04-02 12:08:01.000000 agentuniverse-0.0.5/agentuniverse/agent/plan/planner/rag_planner/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     3397 2024-05-08 13:44:50.000000 agentuniverse-0.0.5/agentuniverse/agent/plan/planner/rag_planner/rag_planner.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      165 2024-04-26 03:46:54.000000 agentuniverse-0.0.5/agentuniverse/agent/plan/planner/rag_planner/rag_planner.yaml
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-05-08 15:59:53.678271 agentuniverse-0.0.5/agentuniverse/agent/plan/planner/reviewing_planner/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      157 2024-04-09 16:15:17.000000 agentuniverse-0.0.5/agentuniverse/agent/plan/planner/reviewing_planner/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     3603 2024-05-08 13:44:50.000000 agentuniverse-0.0.5/agentuniverse/agent/plan/planner/reviewing_planner/reviewing_planner.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      195 2024-04-26 03:46:54.000000 agentuniverse-0.0.5/agentuniverse/agent/plan/planner/reviewing_planner/reviewing_planner.yaml
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-05-08 15:59:53.679047 agentuniverse-0.0.5/agentuniverse/agent_serve/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)        0 2024-04-02 12:08:01.000000 agentuniverse-0.0.5/agentuniverse/agent_serve/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1944 2024-04-02 12:08:01.000000 agentuniverse-0.0.5/agentuniverse/agent_serve/service.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     3152 2024-04-26 03:46:54.000000 agentuniverse-0.0.5/agentuniverse/agent_serve/service_configer.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1161 2024-04-02 12:08:01.000000 agentuniverse-0.0.5/agentuniverse/agent_serve/service_instance.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      402 2024-04-02 12:08:01.000000 agentuniverse-0.0.5/agentuniverse/agent_serve/service_manager.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-05-08 15:59:53.680191 agentuniverse-0.0.5/agentuniverse/agent_serve/web/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentuniverse-0.0.5/agentuniverse/agent_serve/web/__init__.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-05-08 15:59:53.680603 agentuniverse-0.0.5/agentuniverse/agent_serve/web/dal/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentuniverse-0.0.5/agentuniverse/agent_serve/web/dal/__init__.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-05-08 15:59:53.681033 agentuniverse-0.0.5/agentuniverse/agent_serve/web/dal/entity/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentuniverse-0.0.5/agentuniverse/agent_serve/web/dal/entity/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1075 2024-04-02 12:08:01.000000 agentuniverse-0.0.5/agentuniverse/agent_serve/web/dal/entity/request_do.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     5473 2024-04-26 15:29:30.000000 agentuniverse-0.0.5/agentuniverse/agent_serve/web/dal/request_library.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     5327 2024-04-26 15:29:30.000000 agentuniverse-0.0.5/agentuniverse/agent_serve/web/flask_server.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     2351 2024-04-26 15:29:30.000000 agentuniverse-0.0.5/agentuniverse/agent_serve/web/gunicorn_server.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     9311 2024-04-26 09:03:49.000000 agentuniverse-0.0.5/agentuniverse/agent_serve/web/request_task.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-05-08 15:59:53.681342 agentuniverse-0.0.5/agentuniverse/agent_serve/web/rpc/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-26 09:03:49.000000 agentuniverse-0.0.5/agentuniverse/agent_serve/web/rpc/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1224 2024-04-26 09:03:49.000000 agentuniverse-0.0.5/agentuniverse/agent_serve/web/rpc/rpc_server.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1146 2024-04-02 12:08:01.000000 agentuniverse-0.0.5/agentuniverse/agent_serve/web/thread_with_result.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      822 2024-04-26 15:29:30.000000 agentuniverse-0.0.5/agentuniverse/agent_serve/web/web_booster.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     2679 2024-04-26 15:29:30.000000 agentuniverse-0.0.5/agentuniverse/agent_serve/web/web_util.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-05-08 15:59:53.681647 agentuniverse-0.0.5/agentuniverse/base/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentuniverse-0.0.5/agentuniverse/base/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)    11112 2024-05-07 11:44:48.000000 agentuniverse-0.0.5/agentuniverse/base/agentuniverse.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-05-08 15:59:53.681966 agentuniverse-0.0.5/agentuniverse/base/annotation/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentuniverse-0.0.5/agentuniverse/base/annotation/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      515 2024-04-02 12:08:01.000000 agentuniverse-0.0.5/agentuniverse/base/annotation/singleton.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-05-08 15:59:53.682919 agentuniverse-0.0.5/agentuniverse/base/component/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentuniverse-0.0.5/agentuniverse/base/component/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1081 2024-04-26 03:46:54.000000 agentuniverse-0.0.5/agentuniverse/base/component/application_component_manager.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1264 2024-04-26 03:46:54.000000 agentuniverse-0.0.5/agentuniverse/base/component/component_base.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     4380 2024-04-26 09:03:49.000000 agentuniverse-0.0.5/agentuniverse/base/component/component_configer_util.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      626 2024-04-26 09:03:49.000000 agentuniverse-0.0.5/agentuniverse/base/component/component_enum.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     2576 2024-04-26 03:46:54.000000 agentuniverse-0.0.5/agentuniverse/base/component/component_manager_base.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-05-08 15:59:53.683382 agentuniverse-0.0.5/agentuniverse/base/config/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentuniverse-0.0.5/agentuniverse/base/config/__init__.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-05-08 15:59:53.683926 agentuniverse-0.0.5/agentuniverse/base/config/application_configer/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      165 2024-04-02 12:08:01.000000 agentuniverse-0.0.5/agentuniverse/base/config/application_configer/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     4173 2024-04-26 09:03:49.000000 agentuniverse-0.0.5/agentuniverse/base/config/application_configer/app_configer.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1006 2024-04-26 03:46:54.000000 agentuniverse-0.0.5/agentuniverse/base/config/application_configer/application_config_manager.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-05-08 15:59:53.684501 agentuniverse-0.0.5/agentuniverse/base/config/component_configer/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      165 2024-04-02 12:08:01.000000 agentuniverse-0.0.5/agentuniverse/base/config/component_configer/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     2811 2024-04-26 09:03:49.000000 agentuniverse-0.0.5/agentuniverse/base/config/component_configer/component_configer.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-05-08 15:59:53.685816 agentuniverse-0.0.5/agentuniverse/base/config/component_configer/configers/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      165 2024-04-02 12:08:01.000000 agentuniverse-0.0.5/agentuniverse/base/config/component_configer/configers/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     2599 2024-04-26 03:46:54.000000 agentuniverse-0.0.5/agentuniverse/base/config/component_configer/configers/agent_configer.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     2053 2024-04-26 03:46:54.000000 agentuniverse-0.0.5/agentuniverse/base/config/component_configer/configers/knowledge_configer.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     3272 2024-04-26 03:46:54.000000 agentuniverse-0.0.5/agentuniverse/base/config/component_configer/configers/llm_configer.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     2540 2024-04-26 03:46:54.000000 agentuniverse-0.0.5/agentuniverse/base/config/component_configer/configers/memory_configer.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     2392 2024-04-26 03:46:54.000000 agentuniverse-0.0.5/agentuniverse/base/config/component_configer/configers/planner_configer.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1889 2024-04-26 09:03:49.000000 agentuniverse-0.0.5/agentuniverse/base/config/component_configer/configers/prompt_configer.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     2192 2024-04-26 03:46:54.000000 agentuniverse-0.0.5/agentuniverse/base/config/component_configer/configers/tool_configer.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      423 2024-04-02 12:08:01.000000 agentuniverse-0.0.5/agentuniverse/base/config/config_type_enum.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     4846 2024-04-26 15:29:30.000000 agentuniverse-0.0.5/agentuniverse/base/config/configer.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-05-08 15:59:53.686127 agentuniverse-0.0.5/agentuniverse/base/config/custom_configer/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      163 2024-04-02 12:08:01.000000 agentuniverse-0.0.5/agentuniverse/base/config/custom_configer/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      707 2024-04-26 03:55:12.000000 agentuniverse-0.0.5/agentuniverse/base/config/custom_configer/custom_key_configer.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-05-08 15:59:53.686580 agentuniverse-0.0.5/agentuniverse/base/context/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentuniverse-0.0.5/agentuniverse/base/context/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1447 2024-04-26 03:46:54.000000 agentuniverse-0.0.5/agentuniverse/base/context/framework_context.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     2768 2024-04-26 03:46:54.000000 agentuniverse-0.0.5/agentuniverse/base/context/framework_context_manager.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-05-08 15:59:53.687953 agentuniverse-0.0.5/agentuniverse/base/prompt/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      174 2024-04-26 09:03:49.000000 agentuniverse-0.0.5/agentuniverse/base/prompt/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      286 2024-04-26 09:03:49.000000 agentuniverse-0.0.5/agentuniverse/base/prompt/combine_cn_prompt.yaml
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      318 2024-04-26 09:03:49.000000 agentuniverse-0.0.5/agentuniverse/base/prompt/combine_en_prompt.yaml
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      253 2024-04-26 09:03:49.000000 agentuniverse-0.0.5/agentuniverse/base/prompt/summary_cn_prompt.yaml
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      272 2024-04-26 09:03:49.000000 agentuniverse-0.0.5/agentuniverse/base/prompt/summary_en_prompt.yaml
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-05-08 15:59:53.694604 agentuniverse-0.0.5/agentuniverse/base/util/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentuniverse-0.0.5/agentuniverse/base/util/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      307 2024-04-02 12:08:01.000000 agentuniverse-0.0.5/agentuniverse/base/util/env_util.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-05-08 15:59:53.700024 agentuniverse-0.0.5/agentuniverse/base/util/logging/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentuniverse-0.0.5/agentuniverse/base/util/logging/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     6600 2024-04-26 03:42:29.000000 agentuniverse-0.0.5/agentuniverse/base/util/logging/general_logger.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     5132 2024-04-02 12:08:01.000000 agentuniverse-0.0.5/agentuniverse/base/util/logging/logging_config.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     6395 2024-04-26 03:42:21.000000 agentuniverse-0.0.5/agentuniverse/base/util/logging/logging_util.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      502 2024-04-26 03:42:41.000000 agentuniverse-0.0.5/agentuniverse/base/util/memory_util.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     6776 2024-05-08 13:44:50.000000 agentuniverse-0.0.5/agentuniverse/base/util/prompt_util.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      715 2024-04-02 12:08:01.000000 agentuniverse-0.0.5/agentuniverse/base/util/system_util.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-05-08 15:59:53.705713 agentuniverse-0.0.5/agentuniverse/llm/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentuniverse-0.0.5/agentuniverse/llm/__init__.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-05-08 15:59:53.706733 agentuniverse-0.0.5/agentuniverse/llm/default/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-04-02 12:08:01.000000 agentuniverse-0.0.5/agentuniverse/llm/default/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1352 2024-04-26 09:03:49.000000 agentuniverse-0.0.5/agentuniverse/llm/default/default_openai_llm.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      223 2024-04-26 09:03:49.000000 agentuniverse-0.0.5/agentuniverse/llm/default/default_openai_llm.yaml
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     5625 2024-05-08 13:44:50.000000 agentuniverse-0.0.5/agentuniverse/llm/langchain_instance.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     5601 2024-05-08 13:44:50.000000 agentuniverse-0.0.5/agentuniverse/llm/llm.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      619 2024-04-26 03:46:54.000000 agentuniverse-0.0.5/agentuniverse/llm/llm_manager.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      408 2024-04-26 09:03:49.000000 agentuniverse-0.0.5/agentuniverse/llm/llm_output.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     8063 2024-05-08 13:44:50.000000 agentuniverse-0.0.5/agentuniverse/llm/openai_llm.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-05-08 15:59:53.713913 agentuniverse-0.0.5/agentuniverse/prompt/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      156 2024-04-02 12:08:01.000000 agentuniverse-0.0.5/agentuniverse/prompt/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      548 2024-04-26 07:36:14.000000 agentuniverse-0.0.5/agentuniverse/prompt/enum.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     2891 2024-05-08 13:44:50.000000 agentuniverse-0.0.5/agentuniverse/prompt/prompt.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      741 2024-04-26 09:03:49.000000 agentuniverse-0.0.5/agentuniverse/prompt/prompt_manager.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1127 2024-05-08 13:44:50.000000 agentuniverse-0.0.5/agentuniverse/prompt/prompt_model.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-05-08 15:59:53.714276 agentuniverse-0.0.5/agentuniverse_connector/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 03:12:13.000000 agentuniverse-0.0.5/agentuniverse_connector/__init__.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-05-08 15:59:53.717872 agentuniverse-0.0.5/agentuniverse_extension/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 03:13:12.000000 agentuniverse-0.0.5/agentuniverse_extension/__init__.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-05-08 15:59:53.718360 agentuniverse-0.0.5/agentuniverse_extension/logger/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentuniverse-0.0.5/agentuniverse_extension/logger/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     7321 2024-04-02 12:08:01.000000 agentuniverse-0.0.5/agentuniverse_extension/logger/sls_sink.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     2162 2024-05-08 13:45:55.000000 agentuniverse-0.0.5/pyproject.toml
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      323 2024-05-08 15:15:20.000000 agentuniverse-0.0.5/requirements.txt
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)       38 2024-05-08 15:59:53.719851 agentuniverse-0.0.5/setup.cfg
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1230 2024-05-08 15:57:57.000000 agentuniverse-0.0.5/setup.py
```

### Comparing `agentUniverse-0.0.4/LICENSE` & `agentuniverse-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.4/PKG-INFO` & `agentuniverse-0.0.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agentUniverse
-Version: 0.0.4
+Version: 0.0.5
 Summary: agentUniverse is a framework for developing applications powered by multi-agent base on large language model.
 Home-page: https://gitee.com/agentUniverse/agentUniverse
 Author: AntGroup
 Author-email: jerry.zzw@antgroup.com
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -20,16 +20,14 @@
 Requires-Dist: tiktoken>=0.5.2
 Requires-Dist: loguru>=0.7.2
 Requires-Dist: flask_cors>=4.0.0
 Requires-Dist: SQLAlchemy>=2.0.25
 Requires-Dist: pydantic>=2.6.4
 Requires-Dist: gunicorn>=21.2.0
 Requires-Dist: chromadb>=0.4.24
-Requires-Dist: sphinx>=7.2.6
-Requires-Dist: sphinx-rtd-theme>=2.0.0
 Requires-Dist: aliyun-log-python-sdk>=0.8.8
 Requires-Dist: googleapis-common-protos>=1.63.0
 Requires-Dist: myst-parser>=2.0.0
 Requires-Dist: pdfminer.six
 
 # agentUniverse
```

### Comparing `agentUniverse-0.0.4/README.md` & `agentuniverse-0.0.5/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # agentUniverse
 ****************************************
 Language version: [English](./README.md) | [中文](./README_zh.md)
 
 ![](https://img.shields.io/badge/framework-agentUniverse-pink)
 ![](https://img.shields.io/badge/python-3.10%2B-blue?logo=Python)
 [![](https://img.shields.io/badge/%20license-Apache--2.0-yellow)](LICENSE)
-[![Static Badge](https://img.shields.io/badge/pypi-v0.0.3-blue?logo=pypi)](https://pypi.org/project/agentUniverse/)
+[![Static Badge](https://img.shields.io/badge/pypi-v0.0.4-blue?logo=pypi)](https://pypi.org/project/agentUniverse/)
 
 ![](docs/guidebook/_picture/logo_bar.jpg)
 ****************************************
 
 ## Overview
 agentUniverse is a framework for developing applications powered by multi-agent base on large language model.  It provides all the essential components for building a single agent, and a multi-agent collaboration mechanism which  serves as a pattern factory that allowing developers to buid and customize multi-agent collaboration patterns. With this framework,  developers can easily construct multi-agent applications, and share the pattern practices from different technical  and business fields.
 
@@ -42,7 +42,20 @@
 * Use pattern components to complete multi-agent collaboration
 * Test and optimize the performance of the agent
 * Quickly serve the agent
 For details, please read [Quick Start](docs/guidebook/en/1_3_Quick_Start.md).
 
 ## Guidebook
 For more detailed information, please refer to the [Guidebook](docs/guidebook/en/0_index.md).
+
+## API Reference
+[readthedocs](https://agentuniverse.readthedocs.io/en/latest/)
+
+## More Ways to Contact Us
+* github: https://github.com/alipay/agentUniverse
+* gitee: https://gitee.com/agentUniverse/agentUniverse
+* gitcode: https://gitcode.com/agentUniverse
+* Stack Overflow: https://stackoverflowteams.com/c/agentuniverse/questions
+* Discord: https://discord.gg/VfhEvJzQ
+* WeChat Official Account: agentUniverse智多星
+* DingTalk Group:
+![](./docs/guidebook/_picture/dingtalk_util20250429.png)
```

### Comparing `agentUniverse-0.0.4/agentUniverse.egg-info/PKG-INFO` & `agentuniverse-0.0.5/agentUniverse.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agentUniverse
-Version: 0.0.4
+Version: 0.0.5
 Summary: agentUniverse is a framework for developing applications powered by multi-agent base on large language model.
 Home-page: https://gitee.com/agentUniverse/agentUniverse
 Author: AntGroup
 Author-email: jerry.zzw@antgroup.com
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -20,16 +20,14 @@
 Requires-Dist: tiktoken>=0.5.2
 Requires-Dist: loguru>=0.7.2
 Requires-Dist: flask_cors>=4.0.0
 Requires-Dist: SQLAlchemy>=2.0.25
 Requires-Dist: pydantic>=2.6.4
 Requires-Dist: gunicorn>=21.2.0
 Requires-Dist: chromadb>=0.4.24
-Requires-Dist: sphinx>=7.2.6
-Requires-Dist: sphinx-rtd-theme>=2.0.0
 Requires-Dist: aliyun-log-python-sdk>=0.8.8
 Requires-Dist: googleapis-common-protos>=1.63.0
 Requires-Dist: myst-parser>=2.0.0
 Requires-Dist: pdfminer.six
 
 # agentUniverse
```

### Comparing `agentUniverse-0.0.4/agentuniverse/agent/action/knowledge/embedding/embedding.py` & `agentuniverse-0.0.5/agentuniverse/agent/action/knowledge/embedding/embedding.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.4/agentuniverse/agent/action/knowledge/embedding/openai_embedding.py` & `agentuniverse-0.0.5/agentuniverse/agent/action/knowledge/embedding/openai_embedding.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,22 +20,14 @@
 
     openai_client_args: Optional[dict] = None
     openai_api_key: Optional[str] = Field(default_factory=lambda: get_from_env("OPENAI_API_KEY"))
     client: Any = None
     async_client: Any = None
     dimensions: Optional[int] = None
 
-    def __init__(self, **kwargs):
-        """Initialize the openai embedding class."""
-        super().__init__(**kwargs)
-        if self.client is None:
-            self.client = OpenAI(api_key=self.openai_api_key, **self.openai_client_args or {})
-        if self.async_client is None:
-            self.async_client = AsyncOpenAI(api_key=self.openai_api_key, **self.openai_client_args or {})
-
     def get_embeddings(self, texts: List[str]) -> List[List[float]]:
         """Get the OpenAI embeddings.
 
         Note:
             The `embedding_model_name` parameter of the openai embedding class must be provided.
             The `dimensions` parameter of the openai embedding class is optional.
 
@@ -44,15 +36,15 @@
 
          Returns:
              List[List[float]]: Each text gets a float list, and the result is a list of the results for each text.
 
          Raises:
              ValueError: If texts exceed the embedding model token limit or missing some required parameters.
          """
-
+        self.client = OpenAI(api_key=self.openai_api_key, **self.openai_client_args or {})
         if self.embedding_model_name is None:
             raise ValueError("Must provide `embedding_model_name`")
         try:
             if self.dimensions:
                 response = self.client.embeddings.create(input=texts, model=self.embedding_model_name,
                                                          dimensions=self.dimensions)
             else:
@@ -77,15 +69,15 @@
              texts (List[str]): A list of texts that need to be embedded.
 
          Returns:
              List[List[float]]: Each text gets a float list, and the result is a list of the results for each text.
          Raises:
              ValueError: If texts exceed the embedding model token limit or missing some required parameters.
          """
-
+        self.async_client = AsyncOpenAI(api_key=self.openai_api_key, **self.openai_client_args or {})
         if self.embedding_model_name is None:
             raise ValueError("Must provide `embedding_model_name`")
         try:
             if self.dimensions:
                 response = await self.async_client.embeddings.create(input=texts, model=self.embedding_model_name,
                                                                      dimensions=self.dimensions)
             else:
```

### Comparing `agentUniverse-0.0.4/agentuniverse/agent/action/knowledge/knowledge.py` & `agentuniverse-0.0.5/agentuniverse/agent/action/knowledge/knowledge.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.4/agentuniverse/agent/action/knowledge/knowledge_manager.py` & `agentuniverse-0.0.5/agentuniverse/agent/action/knowledge/knowledge_manager.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.4/agentuniverse/agent/action/knowledge/reader/file/docx_reader.py` & `agentuniverse-0.0.5/agentuniverse/agent/action/knowledge/reader/file/docx_reader.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.4/agentuniverse/agent/action/knowledge/reader/file/file_reader.py` & `agentuniverse-0.0.5/agentuniverse/agent/action/knowledge/reader/file/file_reader.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.4/agentuniverse/agent/action/knowledge/reader/file/pdf_reader.py` & `agentuniverse-0.0.5/agentuniverse/agent/action/knowledge/reader/file/pdf_reader.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.4/agentuniverse/agent/action/knowledge/reader/file/pptx_reader.py` & `agentuniverse-0.0.5/agentuniverse/agent/action/knowledge/reader/file/pptx_reader.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.4/agentuniverse/agent/action/knowledge/reader/file/web_pdf_reader.py` & `agentuniverse-0.0.5/agentuniverse/agent/action/knowledge/reader/file/web_pdf_reader.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.4/agentuniverse/agent/action/knowledge/reader/reader.py` & `agentuniverse-0.0.5/agentuniverse/agent/action/knowledge/reader/reader.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.4/agentuniverse/agent/action/knowledge/store/chroma_store.py` & `agentuniverse-0.0.5/agentuniverse/agent/action/knowledge/store/chroma_store.py`

 * *Files 17% similar despite different names*

```diff
@@ -95,14 +95,40 @@
             self.collection.add(
                 documents=[document.text],
                 metadatas=[document.metadata],
                 embeddings=[embedding] if embedding is not None else None,
                 ids=[document.id]
             )
 
+    def upsert_document(self, documents: List[Document], **kwargs):
+        """Upsert document into the store."""
+        for document in documents:
+            embedding = document.embedding
+            if self.embedding_model is not None and len(embedding) == 0:
+                embedding = self.embedding_model.get_embeddings([document.text])[0]
+            self.collection.upsert(
+                documents=[document.text],
+                metadatas=[document.metadata],
+                embeddings=[embedding] if embedding is not None else None,
+                ids=[document.id]
+            )
+
+    def update_document(self, documents: List[Document], **kwargs):
+        """Update document into the store."""
+        for document in documents:
+            embedding = document.embedding
+            if self.embedding_model is not None and len(embedding) == 0:
+                embedding = self.embedding_model.get_embeddings([document.text])[0]
+            self.collection.update(
+                documents=[document.text],
+                metadatas=[document.metadata],
+                embeddings=[embedding] if embedding is not None else None,
+                ids=[document.id]
+            )
+
     @staticmethod
     def to_documents(query_result: QueryResult) -> List[Document]:
         """Convert the query results of ChromaDB to the AgentUniverse(AU) document format."""
 
         if query_result is None:
             return []
         documents = []
```

### Comparing `agentUniverse-0.0.4/agentuniverse/agent/action/knowledge/store/document.py` & `agentuniverse-0.0.5/agentuniverse/agent/action/knowledge/store/document.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,32 +4,39 @@
 # @Author  : wangchongshi
 # @Email   : wangchongshi.wcs@antgroup.com
 # @FileName: document.py
 import uuid
 from typing import Dict, Any, Optional, List
 
 from langchain_core.documents.base import Document as LCDocument
-from pydantic import BaseModel, Field
+from pydantic import BaseModel, Field, model_validator
 
 
 class Document(BaseModel):
     """The basic class for the document.
 
     Attributes:
         id (str): Unique identifier for the document.
         text (Optional[str]): The content of the document.
         metadata (Dict[str, Any]): Metadata associated with the document.
         embedding (List[float]): Embedding data associated with the document
     """
 
-    id: str = Field(default_factory=lambda: str(uuid.uuid4()))
+    id: str = None
     text: Optional[str] = ""
     metadata: Optional[Dict[str, Any]] = None
     embedding: List[float] = Field(default_factory=list)
 
+    @model_validator(mode='before')
+    def create_id(cls, values):
+        text: str = values.get('text', '')
+        if not values.get('id'):
+            values['id'] = str(uuid.uuid5(uuid.NAMESPACE_URL, text))
+        return values
+
     def as_langchain(self) -> LCDocument:
         """Convert to LangChain document format."""
         metadata = self.metadata or {}
         return LCDocument(page_content=self.text, metadata=metadata)
 
     @staticmethod
     def as_langchain_list(document_list) -> List[LCDocument]:
```

### Comparing `agentUniverse-0.0.4/agentuniverse/agent/action/knowledge/store/query.py` & `agentuniverse-0.0.5/agentuniverse/agent/action/knowledge/store/query.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.4/agentuniverse/agent/action/knowledge/store/store.py` & `agentuniverse-0.0.5/agentuniverse/agent/action/knowledge/store/store.py`

 * *Files 21% similar despite different names*

```diff
@@ -83,7 +83,23 @@
     def delete_document(self, document_id: str, **kwargs):
         """Delete the specific document by the document id."""
         raise NotImplementedError
 
     async def async_delete_document(self, document_id: str, **kwargs):
         """Asynchronously delete the specific document by the document id."""
         raise NotImplementedError
+
+    def upsert_document(self, documents: List[Document], **kwargs):
+        """Upsert document into the store."""
+        raise NotImplementedError
+
+    async def async_upsert_document(self, documents: List[Document], **kwargs):
+        """Asynchronously upsert documents into the store."""
+        raise NotImplementedError
+
+    def update_document(self, documents: List[Document], **kwargs):
+        """Update document into the store."""
+        raise NotImplementedError
+
+    async def async_update_document(self, documents: List[Document], **kwargs):
+        """Asynchronously update documents into the store."""
+        raise NotImplementedError
```

### Comparing `agentUniverse-0.0.4/agentuniverse/agent/action/tool/tool.py` & `agentuniverse-0.0.5/agentuniverse/agent/action/tool/tool.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.4/agentuniverse/agent/action/tool/tool_manager.py` & `agentuniverse-0.0.5/agentuniverse/agent/action/tool/tool_manager.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.4/agentuniverse/agent/agent.py` & `agentuniverse-0.0.5/agentuniverse/agent/agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 # @Time    : 2024/3/12 19:36
 # @Author  : heji
 # @Email   : lc299034@antgroup.com
 # @FileName: agent.py
 """The definition of agent paradigm."""
 from abc import abstractmethod
+from datetime import datetime
 from typing import Optional
 
 from agentuniverse.agent.agent_model import AgentModel
 from agentuniverse.agent.input_object import InputObject
 from agentuniverse.agent.output_object import OutputObject
 from agentuniverse.agent.plan.planner.planner import Planner
 from agentuniverse.agent.plan.planner.planner_manager import PlannerManager
@@ -100,14 +101,15 @@
         Args: input_object(InputObject): agent parameter object
         Returns:
             dict: Planner input
         """
         planner_input = dict()
         planner_input['chat_history'] = input_object.get_data('chat_history') or ''
         planner_input['background'] = input_object.get_data('background') or ''
+        planner_input['date'] = datetime.now().strftime('%Y-%m-%d')
 
         self.parse_input(input_object, planner_input)
         return planner_input
 
     def get_instance_code(self) -> str:
         """Return the full name of the agent."""
         appname = ApplicationConfigManager().app_configer.base_info_appname
```

### Comparing `agentUniverse-0.0.4/agentuniverse/agent/agent_manager.py` & `agentuniverse-0.0.5/agentuniverse/agent/agent_manager.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.4/agentuniverse/agent/agent_model.py` & `agentuniverse-0.0.5/agentuniverse/agent/agent_model.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.4/agentuniverse/agent/default/executing_agent.py` & `agentuniverse-0.0.5/agentuniverse/agent/default/executing_agent/executing_agent.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,14 +33,15 @@
             input_object(InputObject): agent parameter object
             planner_input(dict): Planner input
         Returns:
             dict: Planner input
         """
         planner_input['input'] = input_object.get_data('input')
         planner_input['framework'] = input_object.get_data('planning_result').get_data('framework')
+        self.agent_model.profile.setdefault('prompt_version', 'default_executing_agent.cn')
         return planner_input
 
     def parse_result(self, planner_result: dict) -> dict:
         """Planner result parser.
 
         Args:
             planner_result(dict): Planner result
```

### Comparing `agentUniverse-0.0.4/agentuniverse/agent/default/expressing_agent.py` & `agentuniverse-0.0.5/agentuniverse/agent/default/expressing_agent/expressing_agent.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,14 +27,15 @@
             input_object(InputObject): agent parameter object
             planner_input(dict): Planner input
         Returns:
             dict: Planner input
         """
         planner_input['input'] = input_object.get_data('input')
         planner_input['background'] = self.build_background(input_object)
+        self.agent_model.profile.setdefault('prompt_version', 'default_expressing_agent.cn')
         return planner_input
 
     def parse_result(self, planner_result: dict) -> dict:
         """Planner result parser.
 
         Args:
             planner_result(dict): Planner result
```

### Comparing `agentUniverse-0.0.4/agentuniverse/agent/default/planning_agent.py` & `agentuniverse-0.0.5/agentuniverse/agent/default/planning_agent/planning_agent.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,14 +28,15 @@
             input_object(InputObject): agent parameter object
             planner_input(dict): Planner input
         Returns:
             dict: Planner input
         """
         planner_input['input'] = input_object.get_data('input')
         planner_input['expert_framework'] = input_object.get_data('expert_framework')
+        self.agent_model.profile.setdefault('prompt_version', 'default_planning_agent.cn')
         return planner_input
 
     def parse_result(self, planner_result: dict) -> dict:
         """Planner result parser.
 
         Args:
             planner_result(dict): Planner result
```

### Comparing `agentUniverse-0.0.4/agentuniverse/agent/default/rag_agent.py` & `agentuniverse-0.0.5/agentuniverse/agent/default/rag_agent/rag_agent.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,14 +27,15 @@
             input_object(InputObject): agent parameter object
             planner_input(dict): Planner input
         Returns:
             dict: Planner input
         """
         input = input_object.get_data('input')
         planner_input['input'] = input
+        self.agent_model.profile.setdefault('prompt_version', 'default_rag_agent.cn')
         return planner_input
 
     def parse_result(self, planner_result: dict) -> dict:
         """Planner result parser.
 
         Args:
             planner_result(dict): Planner result
```

### Comparing `agentUniverse-0.0.4/agentuniverse/agent/default/reviewing_agent.py` & `agentuniverse-0.0.5/agentuniverse/agent/default/reviewing_agent/reviewing_agent.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,14 +28,15 @@
             input_object(InputObject): agent parameter object
             planner_input(dict): Planner input
         Returns:
             dict: Planner parameter.
         """
         planner_input['input'] = input_object.get_data('input')
         planner_input['expressing_result'] = input_object.get_data('expressing_result').get_data('output')
+        self.agent_model.profile.setdefault('prompt_version', 'default_reviewing_agent.cn')
         return planner_input
 
     def parse_result(self, planner_result: dict) -> dict:
         """Planner result parser.
 
         Args:
             planner_result(dict): Planner result
@@ -47,15 +48,15 @@
         output = planner_result.get('output')
         output = json.loads(output)
         is_useful = output.get('is_useful')
         if is_useful is None:
             is_useful = False
         is_useful = bool(is_useful)
         if is_useful:
-            score = 60
+            score = 80
         else:
             score = 0
 
         agent_result['output'] = output
         agent_result['score'] = score
         agent_result['suggestion'] = output.get('suggestion')
         return agent_result
```

### Comparing `agentUniverse-0.0.4/agentuniverse/agent/input_object.py` & `agentuniverse-0.0.5/agentuniverse/agent/input_object.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.4/agentuniverse/agent/memory/chat_memory.py` & `agentuniverse-0.0.5/agentuniverse/agent/memory/chat_memory.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.4/agentuniverse/agent/memory/default/default_memory.py` & `agentuniverse-0.0.5/agentuniverse/agent/memory/default/default_memory.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.4/agentuniverse/agent/memory/langchain_instance.py` & `agentuniverse-0.0.5/agentuniverse/agent/memory/langchain_instance.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.4/agentuniverse/agent/memory/memory.py` & `agentuniverse-0.0.5/agentuniverse/agent/memory/memory.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.4/agentuniverse/agent/memory/memory_manager.py` & `agentuniverse-0.0.5/agentuniverse/agent/memory/memory_manager.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.4/agentuniverse/agent/memory/summarizer_cn_prompt.yaml` & `agentuniverse-0.0.5/agentuniverse/agent/memory/summarizer_cn_prompt.yaml`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.4/agentuniverse/agent/memory/summarizer_en_prompt.yaml` & `agentuniverse-0.0.5/agentuniverse/agent/memory/summarizer_en_prompt.yaml`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.4/agentuniverse/agent/output_object.py` & `agentuniverse-0.0.5/agentuniverse/agent/output_object.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.4/agentuniverse/agent/plan/planner/executing_planner/default_cn_prompt.yaml` & `agentuniverse-0.0.5/agentuniverse/agent/default/executing_agent/default_cn_prompt.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -16,16 +16,18 @@
   
   之前的对话:
   {chat_history}
   
   背景信息是:
   {background}
   
+  今天的日期是: {date}
+  
   开始!
   我的问题是: {input}
   
   --------------------------------------------------------------
   必须使用中文进行详细的回答。你需要聚焦在我的问题上，不要延伸这个问题。
   让我们一步一步来。
 metadata:
   type: 'PROMPT'
-  version: 'executing_planner.default_cn'
+  version: 'default_executing_agent.cn'
```

### Comparing `agentUniverse-0.0.4/agentuniverse/agent/plan/planner/executing_planner/default_en_prompt.yaml` & `agentuniverse-0.0.5/agentuniverse/agent/default/executing_agent/default_en_prompt.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -16,16 +16,18 @@
   
   Previous conversation:
   {chat_history}
   
   Background Information:
   {background}
   
+  Today's date is: {date}
+
   Let's begin!
   My question is: {input}
   
   --------------------------------------------------------------
   You must provide a detailed response in English. Focus on my question and do not digress from it.
   Let's take it step by step.
 metadata:
   type: 'PROMPT'
-  version: 'executing_planner.default_en'
+  version: 'default_executing_agent.en'
```

### Comparing `agentUniverse-0.0.4/agentuniverse/agent/plan/planner/executing_planner/executing_planner.py` & `agentuniverse-0.0.5/agentuniverse/agent/plan/planner/rag_planner/rag_planner.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,79 +1,80 @@
 # !/usr/bin/env python3
 # -*- coding:utf-8 -*-
-# @Time    : 2024/3/18 10:42
+# @Time    : 2024/3/25 14:58
 # @Author  : heji
 # @Email   : lc299034@antgroup.com
-# @FileName: executing_planner.py
-"""Execution planner module."""
+# @FileName: rag_planner.py
+"""Rag planner module."""
 import asyncio
+
 from langchain.chains import LLMChain
 from langchain_core.memory import BaseMemory
-from langchain_core.prompts import PromptTemplate
+
 from agentuniverse.agent.agent_model import AgentModel
 from agentuniverse.agent.input_object import InputObject
 from agentuniverse.agent.plan.planner.planner import Planner
 from agentuniverse.base.util.prompt_util import process_llm_token
 from agentuniverse.llm.llm import LLM
 from agentuniverse.prompt.prompt import Prompt
 from agentuniverse.prompt.prompt_manager import PromptManager
 from agentuniverse.prompt.prompt_model import AgentPromptModel
 
 
-class ExecutingPlanner(Planner):
-    """Executing planner class."""
+class RagPlanner(Planner):
+    """Rag planner class."""
 
-    def invoke(self, agent_model: AgentModel, planner_input: dict, input_object: InputObject) -> dict:
+    def invoke(self, agent_model: AgentModel, planner_input: dict,
+               input_object: InputObject) -> dict:
         """Invoke the planner.
 
         Args:
             agent_model (AgentModel): Agent model object.
             planner_input (dict): Planner input object.
             input_object (InputObject): Agent input object.
         Returns:
             dict: The planner result.
         """
-
         memory: BaseMemory = self.handle_memory(agent_model, planner_input)
 
-        self.handle_action(agent_model, planner_input, input_object)
+        self.handle_all_actions(agent_model, planner_input, input_object)
 
         llm: LLM = self.handle_llm(agent_model)
 
-        self.handle_prompt(agent_model, planner_input)
+        prompt: Prompt = self.handle_prompt(agent_model, planner_input)
+        process_llm_token(llm, prompt.as_langchain(), agent_model.profile, planner_input)
 
         llm_chain = LLMChain(llm=llm.as_langchain(),
-                             prompt=self.prompt.as_langchain(),
+                             prompt=prompt.as_langchain(),
                              output_key=self.output_key, memory=memory)
         return asyncio.run(llm_chain.acall(inputs=planner_input))
 
-    def handle_prompt(self, agent_model: AgentModel, planner_input: dict):
+    def handle_prompt(self, agent_model: AgentModel, planner_input: dict) -> Prompt:
         """Prompt module processing.
 
         Args:
             agent_model (AgentModel): Agent model object.
             planner_input (dict): Planner input object.
         Returns:
-            PromptTemplate: The prompt template.
+            Prompt: The prompt instance.
         """
-        expert_framework = planner_input.pop('expert_framework', '') or ''
-
         profile: dict = agent_model.profile
 
-        origin_instruction = profile.get('instruction')
-        user_instruction = expert_framework + origin_instruction if origin_instruction else origin_instruction
-
-        user_prompt_model: AgentPromptModel = AgentPromptModel(introduction=profile.get('introduction'),
-                                                               target=profile.get('target'),
-                                                               instruction=user_instruction)
+        profile_prompt_model: AgentPromptModel = AgentPromptModel(introduction=profile.get('introduction'),
+                                                                  target=profile.get('target'),
+                                                                  instruction=profile.get('instruction'))
 
         # get the prompt by the prompt version
-        prompt_version: str = profile.get('prompt_version') or 'executing_planner.default_cn'
-        prompt: Prompt = PromptManager().get_instance_obj(prompt_version)
+        prompt_version: str = profile.get('prompt_version')
+        version_prompt: Prompt = PromptManager().get_instance_obj(prompt_version)
+
+        if version_prompt is None and not profile_prompt_model:
+            raise Exception("Either the `prompt_version` or `introduction & target & instruction`"
+                            " in agent profile configuration should be provided.")
+        if version_prompt:
+            version_prompt_model: AgentPromptModel = AgentPromptModel(
+                introduction=getattr(version_prompt, 'introduction', ''),
+                target=getattr(version_prompt, 'target', ''),
+                instruction=getattr(version_prompt, 'instruction', ''))
+            profile_prompt_model = profile_prompt_model + version_prompt_model
 
-        system_prompt_model: AgentPromptModel = AgentPromptModel(introduction=prompt.introduction,
-                                                                 target=prompt.target,
-                                                                 instruction=expert_framework + prompt.instruction)
-
-        self.prompt.build_prompt(user_prompt_model, system_prompt_model,
-                                 self.prompt_assemble_order)
-        process_llm_token(self.prompt.as_langchain(), profile, planner_input)
+        return Prompt().build_prompt(profile_prompt_model, self.prompt_assemble_order)
```

### Comparing `agentUniverse-0.0.4/agentuniverse/agent/plan/planner/expressing_planner/default_cn_prompt.yaml` & `agentuniverse-0.0.5/agentuniverse/agent/default/expressing_agent/default_cn_prompt.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,17 @@
   
   之前的对话:
   {chat_history}
   
   背景信息是:
   {background}
   
+  今天的日期是: {date}
+
   开始!
   必须使用中文回答用户提出的问题。
   需要回答的问题是: {input}
   --------------------------------------------------------------
   请根据规则要求做出回答。
 metadata:
   type: 'PROMPT'
-  version: 'expressing_planner.default_cn'
+  version: 'default_expressing_agent.cn'
```

### Comparing `agentUniverse-0.0.4/agentuniverse/agent/plan/planner/expressing_planner/default_en_prompt.yaml` & `agentuniverse-0.0.5/agentuniverse/agent/default/expressing_agent/default_en_prompt.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,17 @@
   
   Previous conversation:
   {chat_history}
   
   Background information:
   {background}
   
+  Today's date is: {date}
+
   Let's begin!
   You must answer user questions in English.
   The question that needs answering is: {input}
   --------------------------------------------------------------
   Please provide your response according to to these rules.
 metadata:
   type: 'PROMPT'
-  version: 'expressing_planner.default_en'
+  version: 'default_expressing_agent.en'
```

### Comparing `agentUniverse-0.0.4/agentuniverse/agent/plan/planner/expressing_planner/expressing_planner.py` & `agentuniverse-0.0.5/agentuniverse/agent/plan/planner/executing_planner/executing_planner.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,79 +1,85 @@
 # !/usr/bin/env python3
 # -*- coding:utf-8 -*-
-# @Time    : 2024/3/18 10:50
+# @Time    : 2024/3/18 10:42
 # @Author  : heji
 # @Email   : lc299034@antgroup.com
-# @FileName: expressing_planner.py
-"""Expressing planner module."""
+# @FileName: executing_planner.py
+"""Execution planner module."""
 import asyncio
 
 from langchain.chains import LLMChain
 from langchain_core.memory import BaseMemory
-from langchain_core.prompts import PromptTemplate
 
 from agentuniverse.agent.agent_model import AgentModel
 from agentuniverse.agent.input_object import InputObject
 from agentuniverse.agent.plan.planner.planner import Planner
 from agentuniverse.base.util.prompt_util import process_llm_token
 from agentuniverse.llm.llm import LLM
 from agentuniverse.prompt.prompt import Prompt
 from agentuniverse.prompt.prompt_manager import PromptManager
 from agentuniverse.prompt.prompt_model import AgentPromptModel
 
 
-class ExpressingPlanner(Planner):
-    """Expressing planner class."""
+class ExecutingPlanner(Planner):
+    """Executing planner class."""
 
     def invoke(self, agent_model: AgentModel, planner_input: dict, input_object: InputObject) -> dict:
         """Invoke the planner.
 
         Args:
             agent_model (AgentModel): Agent model object.
             planner_input (dict): Planner input object.
             input_object (InputObject): Agent input object.
         Returns:
             dict: The planner result.
         """
+
         memory: BaseMemory = self.handle_memory(agent_model, planner_input)
 
+        self.handle_all_actions(agent_model, planner_input, input_object)
+
         llm: LLM = self.handle_llm(agent_model)
 
-        self.handle_prompt(agent_model, planner_input)
+        prompt: Prompt = self.handle_prompt(agent_model, planner_input)
+        process_llm_token(llm, prompt.as_langchain(), agent_model.profile, planner_input)
 
         llm_chain = LLMChain(llm=llm.as_langchain(),
-                             prompt=self.prompt.as_langchain(),
+                             prompt=prompt.as_langchain(),
                              output_key=self.output_key, memory=memory)
-
         return asyncio.run(llm_chain.acall(inputs=planner_input))
 
-    def handle_prompt(self, agent_model: AgentModel, planner_input: dict):
+    def handle_prompt(self, agent_model: AgentModel, planner_input: dict) -> Prompt:
         """Prompt module processing.
 
         Args:
             agent_model (AgentModel): Agent model object.
             planner_input (dict): Planner input object.
         Returns:
-            PromptTemplate: The prompt template.
+            Prompt: The prompt instance.
         """
         expert_framework = planner_input.pop('expert_framework', '') or ''
 
         profile: dict = agent_model.profile
 
-        origin_instruction = profile.get('instruction')
-        user_instruction = expert_framework + origin_instruction if origin_instruction else origin_instruction
+        profile_instruction = profile.get('instruction')
+        profile_instruction = expert_framework + profile_instruction if profile_instruction else profile_instruction
 
-        user_prompt_model: AgentPromptModel = AgentPromptModel(introduction=profile.get('introduction'),
-                                                               target=profile.get('target'),
-                                                               instruction=user_instruction)
+        profile_prompt_model: AgentPromptModel = AgentPromptModel(introduction=profile.get('introduction'),
+                                                                  target=profile.get('target'),
+                                                                  instruction=profile_instruction)
 
         # get the prompt by the prompt version
-        prompt_version: str = profile.get('prompt_version') or 'expressing_planner.default_cn'
-        prompt: Prompt = PromptManager().get_instance_obj(prompt_version)
+        prompt_version: str = profile.get('prompt_version')
+        version_prompt: Prompt = PromptManager().get_instance_obj(prompt_version)
+
+        if version_prompt is None and not profile_prompt_model:
+            raise Exception("Either the `prompt_version` or `introduction & target & instruction`"
+                            " in agent profile configuration should be provided.")
+        if version_prompt:
+            version_prompt_model: AgentPromptModel = AgentPromptModel(
+                introduction=getattr(version_prompt, 'introduction', ''),
+                target=getattr(version_prompt, 'target', ''),
+                instruction=expert_framework + getattr(version_prompt, 'instruction', ''))
+            profile_prompt_model = profile_prompt_model + version_prompt_model
 
-        system_prompt_model: AgentPromptModel = AgentPromptModel(introduction=prompt.introduction,
-                                                                 target=prompt.target,
-                                                                 instruction=expert_framework + prompt.instruction)
-
-        self.prompt.build_prompt(user_prompt_model, system_prompt_model,
-                                 self.prompt_assemble_order)
-        process_llm_token(self.prompt.as_langchain(), profile, planner_input)
+        return Prompt().build_prompt(profile_prompt_model, self.prompt_assemble_order)
```

### Comparing `agentUniverse-0.0.4/agentuniverse/agent/plan/planner/peer_planner/peer_planner.py` & `agentuniverse-0.0.5/agentuniverse/agent/plan/planner/peer_planner/peer_planner.py`

 * *Files 4% similar despite different names*

```diff
@@ -104,34 +104,36 @@
 
         planningAgent = agents.get('planning')
         executingAgent = agents.get('executing')
         expressingAgent = agents.get('expressing')
         reviewingAgent = agents.get('reviewing')
 
         for _ in range(retry_count):
-            LOGGER.info(f"Start execution sub agents, retry_count is {_}.")
+            LOGGER.info(f"Starting peer agents, retry_count is {_}.")
             if not planning_result or jump_step == "planning":
                 if not planningAgent:
                     LOGGER.warn("no planning agent, use default.")
                     planning_result = OutputObject({"framework": [agent_input.get('input')]})
                 else:
+                    LOGGER.info(f"Starting planning agent.")
                     planning_result = planningAgent.run(**input_object.to_dict())
 
                 input_object.add_data('planning_result', planning_result)
                 # add planning agent log info
                 logger_info = f"\nPlanning agent execution result is :\n"
                 for index, one_framework in enumerate(planning_result.get_data('framework')):
                     logger_info += f"[{index + 1}] {one_framework} \n"
                 LOGGER.info(logger_info)
 
             if not executing_result or jump_step in ["planning", "executing"]:
                 if not executingAgent:
                     LOGGER.warn("no executing agent, use default.")
                     executing_result = OutputObject({})
                 else:
+                    LOGGER.info(f"Starting executing agent.")
                     executing_result = executingAgent.run(**input_object.to_dict())
 
                 input_object.add_data('executing_result', executing_result)
                 # add executing agent log info
                 logger_info = f"\nExecuting agent execution result is :\n"
                 for index, one_exec_res in enumerate(executing_result.get_data('executing_result')):
                     one_exec_log_info = f"[{index + 1}] input: {one_exec_res['input']}\n"
@@ -140,14 +142,15 @@
                 LOGGER.info(logger_info)
 
             if not expressing_result or jump_step in ["planning", "executing", "expressing"]:
                 if not expressingAgent:
                     LOGGER.warn("no expression agent, use default.")
                     expressing_result = OutputObject({})
                 else:
+                    LOGGER.info(f"Starting expressing agent.")
                     expressing_result = expressingAgent.run(**input_object.to_dict())
 
                 input_object.add_data('expressing_result', expressing_result)
                 # add expressing agent log info
                 logger_info = f"\nExpressing agent execution result is :\n"
                 logger_info += f"{expressing_result.get_data('output')}"
                 LOGGER.info(logger_info)
@@ -160,21 +163,22 @@
                         "executing_result": executing_result,
                         "expressing_result": expressing_result,
                         "reviewing_result": reviewing_result
                     })
                     result['result'] = loopResults
                     return result
                 else:
+                    LOGGER.info(f"Starting reviewing agent.")
                     reviewing_result = reviewingAgent.run(**input_object.to_dict())
                     input_object.add_data('evaluator_result', reviewing_result)
 
                     # add reviewing agent log info
                     logger_info = f"\nReviewing agent execution result is :\n"
                     reviewing_info_str = f"review suggestion: {reviewing_result.get_data('suggestion')} \n"
-                    reviewing_info_str += f"useful: {reviewing_result.get_data('is_useful')} \n"
+                    reviewing_info_str += f"review score: {reviewing_result.get_data('score')} \n"
                     LOGGER.info(logger_info + reviewing_info_str)
 
                     if reviewing_result.get_data('score') and reviewing_result.get_data('score') >= eval_threshold:
                         loopResults.append({
                             "planning_result": planning_result,
                             "executing_result": executing_result,
                             "expressing_result": expressing_result,
```

### Comparing `agentUniverse-0.0.4/agentuniverse/agent/plan/planner/planner.py` & `agentuniverse-0.0.5/agentuniverse/agent/plan/planner/planner.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 # !/usr/bin/env python3
 # -*- coding:utf-8 -*-
 # @Time    : 2024/3/13 10:42
 # @Author  : heji
 # @Email   : lc299034@antgroup.com
 # @FileName: planner.py
 """Base class for Planner."""
-import json
+import copy
 from abc import abstractmethod
 from typing import Optional, List
 
 from langchain_core.memory import BaseMemory
-from langchain_core.prompts import PromptTemplate
 
 from agentuniverse.agent.action.knowledge.knowledge import Knowledge
 from agentuniverse.agent.action.knowledge.knowledge_manager import KnowledgeManager
 from agentuniverse.agent.action.knowledge.store.document import Document
 from agentuniverse.agent.action.knowledge.store.query import Query
 from agentuniverse.agent.action.tool.tool_manager import ToolManager
 from agentuniverse.agent.agent_model import AgentModel
@@ -38,15 +37,14 @@
     All planners should inherit from this class
     """
     name: Optional[str] = None
     description: Optional[str] = None
     output_key: str = 'output'
     input_key: str = 'input'
     prompt_assemble_order: list = ['introduction', 'target', 'instruction']
-    prompt: Prompt = Prompt()
 
     def __init__(self):
         """Initialize the ComponentBase."""
         super().__init__(component_type=ComponentEnum.PLANNER)
 
     @abstractmethod
     def invoke(self, agent_model: AgentModel, planner_input: dict,
@@ -83,22 +81,23 @@
         params['llm'] = llm
         params['input_key'] = self.input_key
         params['output_key'] = self.output_key
 
         memory: Memory = MemoryManager().get_instance_obj(memory_name)
         if memory is None:
             return None
-        memory.set_by_agent_model(**params)
-        langchain_memory: BaseMemory = memory.as_langchain()
+        copied_memory = copy.deepcopy(memory)
+        copied_memory.set_by_agent_model(**params)
+        langchain_memory: BaseMemory = copied_memory.as_langchain()
 
         planner_input['chat_history'] = langchain_memory.load_memory_str
         return langchain_memory
 
-    def handle_action(self, agent_model: AgentModel, planner_input: dict, input_object: InputObject):
-        """Tool or knowledge processing.
+    def handle_all_actions(self, agent_model: AgentModel, planner_input: dict, input_object: InputObject):
+        """Tool and knowledge processing.
 
         Args:
             agent_model (AgentModel): Agent model object.
             planner_input (dict): Planner input object.
             input_object (InputObject): Agent input object.
         """
         action: dict = agent_model.action or dict()
@@ -121,37 +120,38 @@
             knowledge_res: List[Document] = knowledge.store.query(
                 Query(query_str=input_object.get_data(self.input_key), similarity_top_k=2), **input_object.to_dict())
             for document in knowledge_res:
                 action_result.append(document.text)
 
         planner_input['background'] = planner_input['background'] or '' + "\n".join(action_result)
 
-    def handle_prompt(self, agent_model: AgentModel, planner_input: dict):
+    def handle_prompt(self, agent_model: AgentModel, planner_input: dict) -> Prompt:
         """Prompt module processing.
 
         Args:
             agent_model (AgentModel): Agent model object.
             planner_input (dict): Planner input object.
         Returns:
-            PromptTemplate: The prompt template.
+            Prompt: The prompt instance.
         """
         pass
 
     def handle_llm(self, agent_model: AgentModel) -> LLM:
         """Language model module processing.
 
         Args:
             agent_model (AgentModel): Agent model object.
         Returns:
             LLM: The language model.
         """
         llm_name = agent_model.profile.get('llm_model').get('name')
         llm: LLM = LLMManager().get_instance_obj(llm_name)
-        llm.set_by_agent_model(**agent_model.profile.get('llm_model'))
-        return llm
+        copied_llm = copy.deepcopy(llm)
+        copied_llm.set_by_agent_model(**agent_model.profile.get('llm_model'))
+        return copied_llm
 
     def initialize_by_component_configer(self, component_configer: PlannerConfiger) -> 'Planner':
         """Initialize the planner by the PlannerConfiger object.
 
         Args:
             component_configer(PlannerConfiger): the PlannerConfiger object
         Returns:
```

### Comparing `agentUniverse-0.0.4/agentuniverse/agent/plan/planner/planner_manager.py` & `agentuniverse-0.0.5/agentuniverse/agent/plan/planner/planner_manager.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.4/agentuniverse/agent/plan/planner/planning_planner/default_cn_prompt.yaml` & `agentuniverse-0.0.5/agentuniverse/agent/default/planning_agent/default_cn_prompt.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -18,13 +18,15 @@
   
   之前的对话:
   {chat_history}
   
   背景信息是:
   {background}
   
+  今天的日期是: {date}
+
   开始!
   必须使用中文回答用户提出的问题。
   需要回答的问题是: {input}
 metadata:
   type: 'PROMPT'
-  version: 'planning_planner.default_cn'
+  version: 'default_planning_agent.cn'
```

### Comparing `agentUniverse-0.0.4/agentuniverse/agent/plan/planner/planning_planner/default_en_prompt.yaml` & `agentuniverse-0.0.5/agentuniverse/agent/default/planning_agent/default_en_prompt.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -18,13 +18,15 @@
   
   Previous conversations.
   {chat_history}
   
   Background information is.
   {background}
   
+  Today's date is: {date}
+  
   Start!
   You must answer user questions in English.
   The question that needs to be answered is: {input}
 metadata:
   type: 'PROMPT'
-  version: 'planning_planner.default_en'
+  version: 'default_planning_agent.en'
```

### Comparing `agentUniverse-0.0.4/agentuniverse/agent/plan/planner/planning_planner/planning_planner.py` & `agentuniverse-0.0.5/agentuniverse/agent/plan/planner/reviewing_planner/reviewing_planner.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,77 +1,83 @@
 # !/usr/bin/env python3
 # -*- coding:utf-8 -*-
-# @Time    : 2024/3/14 16:02
+# @Time    : 2024/3/18 10:55
 # @Author  : heji
 # @Email   : lc299034@antgroup.com
-# @FileName: planning_planner.py
-"""Planning planner module."""
+# @FileName: reviewing_planner.py
+"""Reviewing planner module."""
 import asyncio
+
 from langchain.chains import LLMChain
 from langchain_core.memory import BaseMemory
 
 from agentuniverse.agent.agent_model import AgentModel
 from agentuniverse.agent.input_object import InputObject
 from agentuniverse.agent.plan.planner.planner import Planner
 from agentuniverse.base.util.prompt_util import process_llm_token
 from agentuniverse.llm.llm import LLM
 from agentuniverse.prompt.prompt import Prompt
 from agentuniverse.prompt.prompt_manager import PromptManager
 from agentuniverse.prompt.prompt_model import AgentPromptModel
 
 
-class PlanningPlanner(Planner):
-    """Planning planner class."""
+class ReviewingPlanner(Planner):
+    """Reviewing planner class."""
 
-    def invoke(self, agent_model: AgentModel, planner_input: dict,
-               input_object: InputObject) -> dict:
+    def invoke(self, agent_model: AgentModel, planner_input: dict, input_object: InputObject) -> dict:
         """Invoke the planner.
 
         Args:
             agent_model (AgentModel): Agent model object.
             planner_input (dict): Planner input object.
             input_object (InputObject): Agent input object.
         Returns:
             dict: The planner result.
         """
         memory: BaseMemory = self.handle_memory(agent_model, planner_input)
 
         llm: LLM = self.handle_llm(agent_model)
 
-        self.handle_prompt(agent_model, planner_input)
+        prompt: Prompt = self.handle_prompt(agent_model, planner_input)
+        process_llm_token(llm, prompt.as_langchain(), agent_model.profile, planner_input)
 
         llm_chain = LLMChain(llm=llm.as_langchain(),
-                             prompt=self.prompt.as_langchain(),
+                             prompt=prompt.as_langchain(),
                              output_key=self.output_key, memory=memory)
 
-        return asyncio.run(llm_chain.acall(planner_input))
+        return asyncio.run(llm_chain.acall(inputs=planner_input))
 
-    def handle_prompt(self, agent_model: AgentModel, planner_input: dict):
-        """Prompt module processing.
+    def handle_prompt(self, agent_model: AgentModel, planner_input: dict) -> Prompt:
+        """Generate prompt template for the planner.
 
         Args:
-            agent_model (AgentModel): Agent model object.
-            planner_input (dict): Planner input object.
+            agent_model (AgentModel): The agent model.
+            planner_input (dict): The agent input.
         Returns:
-            PromptTemplate: The prompt template.
+            Prompt: The prompt instance.
         """
         expert_framework = planner_input.pop('expert_framework', '') or ''
 
         profile: dict = agent_model.profile
 
-        origin_instruction = profile.get('instruction')
-        user_instruction = expert_framework + origin_instruction if origin_instruction else origin_instruction
+        profile_instruction = profile.get('instruction')
+        profile_instruction = expert_framework + profile_instruction if profile_instruction else profile_instruction
 
-        user_prompt_model: AgentPromptModel = AgentPromptModel(introduction=profile.get('introduction'),
-                                                               target=profile.get('target'),
-                                                               instruction=user_instruction)
+        profile_prompt_model: AgentPromptModel = AgentPromptModel(introduction=profile.get('introduction'),
+                                                                  target=profile.get('target'),
+                                                                  instruction=profile_instruction)
 
         # get the prompt by the prompt version
-        prompt_version: str = profile.get('prompt_version') or 'planning_planner.default_cn'
-        prompt: Prompt = PromptManager().get_instance_obj(prompt_version)
+        prompt_version: str = profile.get('prompt_version')
+        version_prompt: Prompt = PromptManager().get_instance_obj(prompt_version)
+
+        if version_prompt is None and not profile_prompt_model:
+            raise Exception("Either the `prompt_version` or `introduction & target & instruction`"
+                            " in agent profile configuration should be provided.")
+        if version_prompt:
+            version_prompt_model: AgentPromptModel = AgentPromptModel(
+                introduction=getattr(version_prompt, 'introduction', ''),
+                target=getattr(version_prompt, 'target', ''),
+                instruction=expert_framework + getattr(version_prompt, 'instruction', ''))
+            profile_prompt_model = profile_prompt_model + version_prompt_model
 
-        system_prompt_model: AgentPromptModel = AgentPromptModel(introduction=prompt.introduction,
-                                                                 target=prompt.target,
-                                                                 instruction=expert_framework + prompt.instruction)
-        self.prompt.build_prompt(user_prompt_model, system_prompt_model,
-                                 self.prompt_assemble_order)
-        process_llm_token(self.prompt.as_langchain(), profile, planner_input)
+        return Prompt().build_prompt(profile_prompt_model, self.prompt_assemble_order)
```

### Comparing `agentUniverse-0.0.4/agentuniverse/agent/plan/planner/rag_planner/default_cn_prompt.yaml` & `agentuniverse-0.0.5/agentuniverse/agent/default/rag_agent/default_cn_prompt.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -12,13 +12,15 @@
 
   之前的对话:
   {chat_history}
 
   背景信息是:
   {background}
 
+  今天的日期是: {date}
+
   开始!
 
   需要回答的问题是: {input}
 metadata:
   type: 'PROMPT'
-  version: 'rag_planner.default_cn'
+  version: 'default_rag_agent.cn'
```

### Comparing `agentUniverse-0.0.4/agentuniverse/agent/plan/planner/rag_planner/default_en_prompt.yaml` & `agentuniverse-0.0.5/agentuniverse/agent/default/rag_agent/default_en_prompt.yaml`

 * *Files 22% similar despite different names*

```diff
@@ -12,13 +12,15 @@
   
   Previous conversation:
   {chat_history}
   
   Background information:
   {background}
   
+  Today's date is: {date}
+
   Let's get started!
   
   The question that needs to be answered is: {input}
 metadata:
   type: 'PROMPT'
-  version: 'rag_planner.default_en'
+  version: 'default_rag_agent.en'
```

### Comparing `agentUniverse-0.0.4/agentuniverse/agent/plan/planner/rag_planner/rag_planner.py` & `agentuniverse-0.0.5/agentuniverse/agent/plan/planner/planning_planner/planning_planner.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,73 +1,84 @@
 # !/usr/bin/env python3
 # -*- coding:utf-8 -*-
-# @Time    : 2024/3/25 14:58
+# @Time    : 2024/3/14 16:02
 # @Author  : heji
 # @Email   : lc299034@antgroup.com
-# @FileName: rag_planner.py
-"""Rag planner module."""
+# @FileName: planning_planner.py
+"""Planning planner module."""
 import asyncio
+
 from langchain.chains import LLMChain
 from langchain_core.memory import BaseMemory
+
 from agentuniverse.agent.agent_model import AgentModel
 from agentuniverse.agent.input_object import InputObject
 from agentuniverse.agent.plan.planner.planner import Planner
 from agentuniverse.base.util.prompt_util import process_llm_token
 from agentuniverse.llm.llm import LLM
 from agentuniverse.prompt.prompt import Prompt
 from agentuniverse.prompt.prompt_manager import PromptManager
 from agentuniverse.prompt.prompt_model import AgentPromptModel
 
 
-class RagPlanner(Planner):
-    """Rag planner class."""
+class PlanningPlanner(Planner):
+    """Planning planner class."""
 
     def invoke(self, agent_model: AgentModel, planner_input: dict,
                input_object: InputObject) -> dict:
         """Invoke the planner.
 
         Args:
             agent_model (AgentModel): Agent model object.
             planner_input (dict): Planner input object.
             input_object (InputObject): Agent input object.
         Returns:
             dict: The planner result.
         """
         memory: BaseMemory = self.handle_memory(agent_model, planner_input)
 
-        self.handle_action(agent_model, planner_input, input_object)
-
         llm: LLM = self.handle_llm(agent_model)
 
-        self.handle_prompt(agent_model, planner_input)
+        prompt: Prompt = self.handle_prompt(agent_model, planner_input)
+        process_llm_token(llm, prompt.as_langchain(), agent_model.profile, planner_input)
 
         llm_chain = LLMChain(llm=llm.as_langchain(),
-                             prompt=self.prompt.as_langchain(),
+                             prompt=prompt.as_langchain(),
                              output_key=self.output_key, memory=memory)
-        return asyncio.run(llm_chain.acall(inputs=planner_input))
 
-    def handle_prompt(self, agent_model: AgentModel, planner_input: dict):
+        return asyncio.run(llm_chain.acall(planner_input))
+
+    def handle_prompt(self, agent_model: AgentModel, planner_input: dict) -> Prompt:
         """Prompt module processing.
 
         Args:
             agent_model (AgentModel): Agent model object.
             planner_input (dict): Planner input object.
         Returns:
-            PromptTemplate: The prompt template.
+            Prompt: The prompt instance.
         """
+        expert_framework = planner_input.pop('expert_framework', '') or ''
+
         profile: dict = agent_model.profile
 
-        user_prompt_model: AgentPromptModel = AgentPromptModel(introduction=profile.get('introduction'),
-                                                               target=profile.get('target'),
-                                                               instruction=profile.get('instruction'))
+        profile_instruction = profile.get('instruction')
+        profile_instruction = expert_framework + profile_instruction if profile_instruction else profile_instruction
+
+        profile_prompt_model: AgentPromptModel = AgentPromptModel(introduction=profile.get('introduction'),
+                                                                  target=profile.get('target'),
+                                                                  instruction=profile_instruction)
 
         # get the prompt by the prompt version
-        prompt_version: str = profile.get('prompt_version') or 'rag_planner.default_cn'
-        prompt: Prompt = PromptManager().get_instance_obj(prompt_version)
+        prompt_version: str = profile.get('prompt_version')
+        version_prompt: Prompt = PromptManager().get_instance_obj(prompt_version)
+
+        if version_prompt is None and not profile_prompt_model:
+            raise Exception("Either the `prompt_version` or `introduction & target & instruction`"
+                            " in agent profile configuration should be provided.")
+        if version_prompt:
+            version_prompt_model: AgentPromptModel = AgentPromptModel(
+                introduction=getattr(version_prompt, 'introduction', ''),
+                target=getattr(version_prompt, 'target', ''),
+                instruction=expert_framework + getattr(version_prompt, 'instruction', ''))
+            profile_prompt_model = profile_prompt_model + version_prompt_model
 
-        system_prompt_model: AgentPromptModel = AgentPromptModel(introduction=prompt.introduction,
-                                                                 target=prompt.target,
-                                                                 instruction=prompt.instruction)
-
-        self.prompt.build_prompt(user_prompt_model, system_prompt_model,
-                                 self.prompt_assemble_order)
-        process_llm_token(self.prompt.as_langchain(), profile, planner_input)
+        return Prompt().build_prompt(profile_prompt_model, self.prompt_assemble_order)
```

### Comparing `agentUniverse-0.0.4/agentuniverse/agent/plan/planner/reviewing_planner/default_cn_prompt.yaml` & `agentuniverse-0.0.5/agentuniverse/agent/default/reviewing_agent/default_cn_prompt.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -15,14 +15,16 @@
   
   之前的对话:
   {chat_history}
   
   背景信息是:
   {background}
   
+  今天的日期是: {date}
+
   开始!
   必须使用中文回答用户提出的问题。
   指定的问题是: {input}
   给出的答案是: {expressing_result}
 metadata:
   type: 'PROMPT'
-  version: 'reviewing_planner.default_cn'
+  version: 'default_reviewing_agent.cn'
```

### Comparing `agentUniverse-0.0.4/agentuniverse/agent/plan/planner/reviewing_planner/default_en_prompt.yaml` & `agentuniverse-0.0.5/agentuniverse/agent/default/reviewing_agent/default_en_prompt.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,16 @@
   
   Previous conversation:
   {chat_history}
   
   Background information:
   {background}
   
+  Today's date is: {date}
+
   Let's begin!
   You must answer user questions in English.
   The specified question is: {input}
   The provided answer is: {expressing_result}
 metadata:
   type: 'PROMPT'
-  version: 'reviewing_planner.default_en'
+  version: 'default_reviewing_agent.en'
```

### Comparing `agentUniverse-0.0.4/agentuniverse/agent/plan/planner/reviewing_planner/reviewing_planner.py` & `agentuniverse-0.0.5/agentuniverse/agent/plan/planner/expressing_planner/expressing_planner.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 # !/usr/bin/env python3
 # -*- coding:utf-8 -*-
-# @Time    : 2024/3/18 10:55
+# @Time    : 2024/3/18 10:50
 # @Author  : heji
 # @Email   : lc299034@antgroup.com
-# @FileName: reviewing_planner.py
-"""Reviewing planner module."""
+# @FileName: expressing_planner.py
+"""Expressing planner module."""
 import asyncio
+
 from langchain.chains import LLMChain
 from langchain_core.memory import BaseMemory
-from langchain_core.prompts import PromptTemplate
+
 from agentuniverse.agent.agent_model import AgentModel
 from agentuniverse.agent.input_object import InputObject
 from agentuniverse.agent.plan.planner.planner import Planner
 from agentuniverse.base.util.prompt_util import process_llm_token
 from agentuniverse.llm.llm import LLM
 from agentuniverse.prompt.prompt import Prompt
 from agentuniverse.prompt.prompt_manager import PromptManager
 from agentuniverse.prompt.prompt_model import AgentPromptModel
 
 
-class ReviewingPlanner(Planner):
-    """Reviewing planner class."""
+class ExpressingPlanner(Planner):
+    """Expressing planner class."""
 
     def invoke(self, agent_model: AgentModel, planner_input: dict, input_object: InputObject) -> dict:
         """Invoke the planner.
 
         Args:
             agent_model (AgentModel): Agent model object.
             planner_input (dict): Planner input object.
@@ -32,46 +33,51 @@
         Returns:
             dict: The planner result.
         """
         memory: BaseMemory = self.handle_memory(agent_model, planner_input)
 
         llm: LLM = self.handle_llm(agent_model)
 
-        self.handle_prompt(agent_model, planner_input)
+        prompt: Prompt = self.handle_prompt(agent_model, planner_input)
+        process_llm_token(llm, prompt.as_langchain(), agent_model.profile, planner_input)
 
         llm_chain = LLMChain(llm=llm.as_langchain(),
-                             prompt=self.prompt.as_langchain(),
+                             prompt=prompt.as_langchain(),
                              output_key=self.output_key, memory=memory)
 
         return asyncio.run(llm_chain.acall(inputs=planner_input))
 
-    def handle_prompt(self, agent_model: AgentModel, planner_input: dict):
-        """Generate prompt template for the planner.
+    def handle_prompt(self, agent_model: AgentModel, planner_input: dict) -> Prompt:
+        """Prompt module processing.
 
         Args:
-            agent_model (AgentModel): The agent model.
-            planner_input (dict): The agent input.
+            agent_model (AgentModel): Agent model object.
+            planner_input (dict): Planner input object.
         Returns:
-            PromptTemplate: The prompt template.
+            Prompt: The prompt instance.
         """
         expert_framework = planner_input.pop('expert_framework', '') or ''
 
         profile: dict = agent_model.profile
 
-        origin_instruction = profile.get('instruction')
-        user_instruction = expert_framework + origin_instruction if origin_instruction else origin_instruction
+        profile_instruction = profile.get('instruction')
+        profile_instruction = expert_framework + profile_instruction if profile_instruction else profile_instruction
 
-        user_prompt_model: AgentPromptModel = AgentPromptModel(introduction=profile.get('introduction'),
-                                                               target=profile.get('target'),
-                                                               instruction=user_instruction)
+        profile_prompt_model: AgentPromptModel = AgentPromptModel(introduction=profile.get('introduction'),
+                                                                  target=profile.get('target'),
+                                                                  instruction=profile_instruction)
 
         # get the prompt by the prompt version
-        prompt_version: str = profile.get('prompt_version') or 'reviewing_planner.default_cn'
-        prompt: Prompt = PromptManager().get_instance_obj(prompt_version)
+        prompt_version: str = profile.get('prompt_version')
+        version_prompt: Prompt = PromptManager().get_instance_obj(prompt_version)
+
+        if version_prompt is None and not profile_prompt_model:
+            raise Exception("Either the `prompt_version` or `introduction & target & instruction`"
+                            " in agent profile configuration should be provided.")
+        if version_prompt:
+            version_prompt_model: AgentPromptModel = AgentPromptModel(
+                introduction=getattr(version_prompt, 'introduction', ''),
+                target=getattr(version_prompt, 'target', ''),
+                instruction=expert_framework + getattr(version_prompt, 'instruction', ''))
+            profile_prompt_model = profile_prompt_model + version_prompt_model
 
-        system_prompt_model: AgentPromptModel = AgentPromptModel(introduction=prompt.introduction,
-                                                                 target=prompt.target,
-                                                                 instruction=expert_framework + prompt.instruction)
-
-        self.prompt.build_prompt(user_prompt_model, system_prompt_model,
-                                 self.prompt_assemble_order)
-        process_llm_token(self.prompt.as_langchain(), profile, planner_input)
+        return Prompt().build_prompt(profile_prompt_model, self.prompt_assemble_order)
```

### Comparing `agentUniverse-0.0.4/agentuniverse/agent_serve/service.py` & `agentuniverse-0.0.5/agentuniverse/agent_serve/service.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.4/agentuniverse/agent_serve/service_configer.py` & `agentuniverse-0.0.5/agentuniverse/agent_serve/service_configer.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.4/agentuniverse/agent_serve/service_instance.py` & `agentuniverse-0.0.5/agentuniverse/agent_serve/service_instance.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.4/agentuniverse/agent_serve/web/dal/entity/request_do.py` & `agentuniverse-0.0.5/agentuniverse/agent_serve/web/dal/entity/request_do.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.4/agentuniverse/agent_serve/web/dal/request_library.py` & `agentuniverse-0.0.5/agentuniverse/agent_serve/web/dal/request_library.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.4/agentuniverse/agent_serve/web/flask_server.py` & `agentuniverse-0.0.5/agentuniverse/agent_serve/web/flask_server.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.4/agentuniverse/agent_serve/web/gunicorn_server.py` & `agentuniverse-0.0.5/agentuniverse/agent_serve/web/gunicorn_server.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.4/agentuniverse/agent_serve/web/request_task.py` & `agentuniverse-0.0.5/agentuniverse/agent_serve/web/request_task.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.4/agentuniverse/agent_serve/web/rpc/rpc_server.py` & `agentuniverse-0.0.5/agentuniverse/agent_serve/web/rpc/rpc_server.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.4/agentuniverse/agent_serve/web/thread_with_result.py` & `agentuniverse-0.0.5/agentuniverse/agent_serve/web/thread_with_result.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.4/agentuniverse/agent_serve/web/web_booster.py` & `agentuniverse-0.0.5/agentuniverse/agent_serve/web/web_booster.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.4/agentuniverse/agent_serve/web/web_util.py` & `agentuniverse-0.0.5/agentuniverse/agent_serve/web/web_util.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.4/agentuniverse/base/agentuniverse.py` & `agentuniverse-0.0.5/agentuniverse/base/agentuniverse.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,15 +29,19 @@
 class AgentUniverse(object):
     """AgentUniverse framework object, responsible for the framework initialization,
        system variables management, etc."""
 
     def __init__(self):
         self.__application_container = ApplicationComponentManager()
         self.__config_container: ApplicationConfigManager = ApplicationConfigManager()
-        self.__system_default_package = ['agentuniverse']
+        self.__system_default_agent_package = ['agentuniverse.agent.default']
+        self.__system_default_llm_package = ['agentuniverse.llm.default']
+        self.__system_default_planner_package = ['agentuniverse.agent.plan.planner']
+        self.__system_default_memory_package = ['agentuniverse.agent.memory.default']
+        self.__system_default_prompt_package = ['agentuniverse.agent', 'agentuniverse.base.prompt']
 
     def start(self, config_path: str = None):
         """Start the agentUniverse framework."""
         # get default config path
         project_root_path = get_project_root_path()
         sys.path.append(str(project_root_path.parent))
         app_path = project_root_path / 'app'
@@ -88,22 +92,27 @@
 
     def __scan_and_register(self, app_configer: AppConfiger):
         """Scan the component directory and register the components.
 
         Args:
             app_configer(AppConfiger): the AppConfiger object
         """
-        core_agent_package_list = app_configer.core_agent_package_list or app_configer.core_default_package_list + self.__system_default_package
-        core_knowledge_package_list = app_configer.core_knowledge_package_list or app_configer.core_default_package_list + self.__system_default_package
-        core_llm_package_list = app_configer.core_llm_package_list or app_configer.core_default_package_list + self.__system_default_package
-        core_planner_package_list = app_configer.core_planner_package_list or app_configer.core_default_package_list + self.__system_default_package
-        core_tool_package_list = app_configer.core_tool_package_list or app_configer.core_default_package_list + self.__system_default_package
-        core_service_package_list = app_configer.core_service_package_list or app_configer.core_default_package_list + self.__system_default_package
-        core_memory_package_list = app_configer.core_memory_package_list or app_configer.core_default_package_list + self.__system_default_package
-        core_prompt_package_list = app_configer.core_prompt_package_list or app_configer.core_default_package_list + self.__system_default_package
+        core_agent_package_list = ((app_configer.core_agent_package_list or app_configer.core_default_package_list)
+                                   + self.__system_default_agent_package)
+        core_knowledge_package_list = app_configer.core_knowledge_package_list or app_configer.core_default_package_list
+        core_llm_package_list = ((app_configer.core_llm_package_list or app_configer.core_default_package_list)
+                                 + self.__system_default_llm_package)
+        core_planner_package_list = ((app_configer.core_planner_package_list or app_configer.core_default_package_list)
+                                     + self.__system_default_planner_package)
+        core_tool_package_list = app_configer.core_tool_package_list or app_configer.core_default_package_list
+        core_service_package_list = app_configer.core_service_package_list or app_configer.core_default_package_list
+        core_memory_package_list = ((app_configer.core_memory_package_list or app_configer.core_default_package_list)
+                                    + self.__system_default_memory_package)
+        core_prompt_package_list = ((app_configer.core_prompt_package_list or app_configer.core_default_package_list)
+                                    + self.__system_default_prompt_package)
 
         component_package_map = {
             ComponentEnum.AGENT: core_agent_package_list,
             ComponentEnum.KNOWLEDGE: core_knowledge_package_list,
             ComponentEnum.LLM: core_llm_package_list,
             ComponentEnum.PLANNER: core_planner_package_list,
             ComponentEnum.TOOL: core_tool_package_list,
```

### Comparing `agentUniverse-0.0.4/agentuniverse/base/annotation/singleton.py` & `agentuniverse-0.0.5/agentuniverse/base/annotation/singleton.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.4/agentuniverse/base/component/application_component_manager.py` & `agentuniverse-0.0.5/agentuniverse/base/component/application_component_manager.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.4/agentuniverse/base/component/component_base.py` & `agentuniverse-0.0.5/agentuniverse/base/component/component_base.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.4/agentuniverse/base/component/component_configer_util.py` & `agentuniverse-0.0.5/agentuniverse/base/component/component_configer_util.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.4/agentuniverse/base/component/component_enum.py` & `agentuniverse-0.0.5/agentuniverse/base/component/component_enum.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.4/agentuniverse/base/component/component_manager_base.py` & `agentuniverse-0.0.5/agentuniverse/base/component/component_manager_base.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.4/agentuniverse/base/config/application_configer/app_configer.py` & `agentuniverse-0.0.5/agentuniverse/base/config/application_configer/app_configer.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.4/agentuniverse/base/config/application_configer/application_config_manager.py` & `agentuniverse-0.0.5/agentuniverse/base/config/application_configer/application_config_manager.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.4/agentuniverse/base/config/component_configer/component_configer.py` & `agentuniverse-0.0.5/agentuniverse/base/config/component_configer/component_configer.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.4/agentuniverse/base/config/component_configer/configers/agent_configer.py` & `agentuniverse-0.0.5/agentuniverse/base/config/component_configer/configers/agent_configer.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.4/agentuniverse/base/config/component_configer/configers/knowledge_configer.py` & `agentuniverse-0.0.5/agentuniverse/base/config/component_configer/configers/knowledge_configer.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.4/agentuniverse/base/config/component_configer/configers/llm_configer.py` & `agentuniverse-0.0.5/agentuniverse/base/config/component_configer/configers/llm_configer.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.4/agentuniverse/base/config/component_configer/configers/memory_configer.py` & `agentuniverse-0.0.5/agentuniverse/base/config/component_configer/configers/memory_configer.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.4/agentuniverse/base/config/component_configer/configers/planner_configer.py` & `agentuniverse-0.0.5/agentuniverse/base/config/component_configer/configers/planner_configer.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.4/agentuniverse/base/config/component_configer/configers/prompt_configer.py` & `agentuniverse-0.0.5/agentuniverse/base/config/component_configer/configers/prompt_configer.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.4/agentuniverse/base/config/component_configer/configers/tool_configer.py` & `agentuniverse-0.0.5/agentuniverse/base/config/component_configer/configers/tool_configer.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.4/agentuniverse/base/config/configer.py` & `agentuniverse-0.0.5/agentuniverse/base/config/configer.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.4/agentuniverse/base/config/custom_configer/custom_key_configer.py` & `agentuniverse-0.0.5/agentuniverse/base/config/custom_configer/custom_key_configer.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.4/agentuniverse/base/context/framework_context.py` & `agentuniverse-0.0.5/agentuniverse/base/context/framework_context.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.4/agentuniverse/base/context/framework_context_manager.py` & `agentuniverse-0.0.5/agentuniverse/base/context/framework_context_manager.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.4/agentuniverse/base/util/logging/general_logger.py` & `agentuniverse-0.0.5/agentuniverse/base/util/logging/general_logger.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.4/agentuniverse/base/util/logging/logging_config.py` & `agentuniverse-0.0.5/agentuniverse/base/util/logging/logging_config.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.4/agentuniverse/base/util/logging/logging_util.py` & `agentuniverse-0.0.5/agentuniverse/base/util/logging/logging_util.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.4/agentuniverse/base/util/prompt_util.py` & `agentuniverse-0.0.5/agentuniverse/base/util/prompt_util.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,39 +15,34 @@
 from agentuniverse.llm.llm import LLM
 from agentuniverse.llm.llm_manager import LLMManager
 from agentuniverse.prompt.prompt_manager import PromptManager
 from agentuniverse.prompt.prompt_model import AgentPromptModel
 from agentuniverse.prompt.enum import PromptProcessEnum
 
 
-def summarize_by_stuff(texts: List[str], llm: LLM, summary_prompt_version: str):
+def summarize_by_stuff(texts: List[str], llm: LLM, summary_prompt):
     """
     stuff summarization -- general method
     """
-    summary_prompt = PromptManager().get_instance_obj(summary_prompt_version)
     stuff_chain = load_summarize_chain(llm.as_langchain(), chain_type='stuff', verbose=True,
                                        prompt=summary_prompt.as_langchain())
-    return asyncio.run(stuff_chain.arun([Document(page_content=text) for text in texts]))
+    return stuff_chain.run([Document(page_content=text) for text in texts])
 
 
-def summarize_by_map_reduce(texts: List[str], llm: LLM, agent_llm: LLM, summary_prompt_version: str,
-                            combine_prompt_version: str):
+def summarize_by_map_reduce(texts: List[str], llm: LLM, summary_prompt, combine_prompt):
     """
     map reduce summarization -- general method
     """
-    texts = split_texts(texts, agent_llm)
-    summary_prompt = PromptManager().get_instance_obj(summary_prompt_version)
-    combine_prompt = PromptManager().get_instance_obj(combine_prompt_version)
     map_reduce_chain = load_summarize_chain(llm.as_langchain(), chain_type='map_reduce', verbose=True,
                                             map_prompt=summary_prompt.as_langchain(),
                                             combine_prompt=combine_prompt.as_langchain())
-    return asyncio.run(map_reduce_chain.arun([Document(page_content=text) for text in texts]))
+    return map_reduce_chain.run([Document(page_content=text) for text in texts])
 
 
-def split_text_on_tokens(text: str, text_token, chunk_size=800, chunk_overlap=100) -> List[str]:
+def split_text_on_tokens(text: str, text_token: int, chunk_size=800, chunk_overlap=100) -> List[str]:
     """Split incoming text and return chunks using tokenizer."""
     # calculate the number of characters represented by each token.
     char_per_token = len(text) / text_token
     chunk_char_size = int(chunk_size * char_per_token)
     chunk_char_overlap = int(chunk_overlap * char_per_token)
 
     result = []
@@ -58,40 +53,43 @@
             chunk = text[current_position:]
         else:
             chunk = text[current_position:current_position + chunk_char_size]
 
         result.append(chunk)
         current_position += chunk_char_size - chunk_char_overlap
 
+    if len(result) == 0:
+        result.append(text[current_position:])
+
     return result
 
 
-def split_texts(texts: list[str], agent_llm: LLM, chunk_size=800, chunk_overlap=100, retry=True) -> list[str]:
+def split_texts(texts: list[str], llm: LLM, chunk_size=800, chunk_overlap=100, retry=True) -> list[str]:
     """
     split texts into chunks with the fixed token length -- general method
     """
     try:
         split_texts_res = []
         for text in texts:
-            text_token = agent_llm.get_num_tokens(text)
+            text_token = llm.get_num_tokens(text)
             split_texts_res.extend(
                 split_text_on_tokens(text=text, text_token=text_token, chunk_size=chunk_size,
                                      chunk_overlap=chunk_overlap))
         return split_texts_res
     except Exception as e:
         if retry:
-            return split_texts(texts=texts, agent_llm=agent_llm, retry=False)
+            return split_texts(texts=texts, llm=llm, retry=False)
         raise ValueError("split text failed, exception=" + str(e))
 
 
-def truncate_content(content: str, token_length: int, agent_llm: LLM) -> str:
+def truncate_content(content: str, token_length: int, llm: LLM) -> str:
     """
     truncate the content based on the llm token limit
     """
-    return str(split_texts(texts=[content], chunk_size=token_length, agent_llm=agent_llm)[0])
+    return str(split_texts(texts=[content], chunk_size=token_length, llm=llm)[0])
 
 
 def generate_template(agent_prompt_model: AgentPromptModel, prompt_assemble_order: list[str]) -> str:
     """Convert the agent prompt model to an ordered list.
 
     Args:
         agent_prompt_model (AgentPromptModel): The agent prompt model.
@@ -104,53 +102,60 @@
         value = getattr(agent_prompt_model, attr, None)
         if value is not None:
             values.append(value)
 
     return "\n".join(values)
 
 
-def process_llm_token(prompt_template: PromptTemplate, profile: dict, planner_input: dict):
+def process_llm_token(agent_llm: LLM, prompt_template: PromptTemplate, profile: dict, planner_input: dict):
     """Process the prompt template based on the prompt processor.
 
     Args:
+        agent_llm (LLM): The agent llm.
         prompt_template (PromptTemplate): The prompt template.
         profile (dict): The profile.
         planner_input (dict): The planner input.
     """
     llm_model: dict = profile.get('llm_model')
-    llm_name: str = llm_model.get('name')
 
     # get the prompt processor configuration
     prompt_processor: dict = llm_model.get('prompt_processor') or dict()
     prompt_processor_type: str = prompt_processor.get('type') or PromptProcessEnum.TRUNCATE.value
-    prompt_processor_llm: str = prompt_processor.get('llm') or llm_name
+    prompt_processor_llm: str = prompt_processor.get('llm')
 
     # get the summary and combine prompt versions
     summary_prompt_version: str = prompt_processor.get('summary_prompt_version') or 'prompt_processor.summary_cn'
     combine_prompt_version: str = prompt_processor.get('combine_prompt_version') or 'prompt_processor.combine_cn'
 
     prompt_input_dict = {key: planner_input[key] for key in prompt_template.input_variables if key in planner_input}
 
-    agent_llm: LLM = LLMManager().get_instance_obj(llm_name)
     # get the llm instance for prompt compression
     prompt_llm: LLM = LLMManager().get_instance_obj(prompt_processor_llm)
 
+    if prompt_llm is None:
+        prompt_llm = agent_llm
+
     prompt = prompt_template.format(**prompt_input_dict)
     # get the number of tokens in the prompt
     prompt_tokens: int = agent_llm.get_num_tokens(prompt)
 
-    remaining_tokens = agent_llm.max_context_length() - agent_llm.max_tokens
+    input_tokens = agent_llm.max_context_length() - agent_llm.max_tokens
 
-    if prompt_tokens <= remaining_tokens:
+    if prompt_tokens <= input_tokens:
         return
 
     process_prompt_type_enum = PromptProcessEnum.from_value(prompt_processor_type)
 
     # compress the background in the prompt
     content = planner_input.get('background')
     if process_prompt_type_enum == PromptProcessEnum.TRUNCATE:
-        planner_input['background'] = truncate_content(content, remaining_tokens, agent_llm)
+        planner_input['background'] = truncate_content(content, input_tokens, agent_llm)
     elif process_prompt_type_enum == PromptProcessEnum.STUFF:
-        planner_input['background'] = summarize_by_stuff([content], prompt_llm, summary_prompt_version)
+        planner_input['background'] = summarize_by_stuff(texts=[content], llm=prompt_llm,
+                                                         summary_prompt=PromptManager().get_instance_obj(
+                                                             summary_prompt_version))
     elif process_prompt_type_enum == PromptProcessEnum.MAP_REDUCE:
-        planner_input['background'] = summarize_by_map_reduce([content], prompt_llm,
-                                                              agent_llm, summary_prompt_version, combine_prompt_version)
+        planner_input['background'] = summarize_by_map_reduce(texts=split_texts([content], agent_llm), llm=prompt_llm,
+                                                              summary_prompt=PromptManager().get_instance_obj(
+                                                                  summary_prompt_version),
+                                                              combine_prompt=PromptManager().get_instance_obj(
+                                                                  combine_prompt_version))
```

### Comparing `agentUniverse-0.0.4/agentuniverse/base/util/system_util.py` & `agentuniverse-0.0.5/agentuniverse/base/util/system_util.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.4/agentuniverse/llm/default/default_openai_llm.py` & `agentuniverse-0.0.5/agentuniverse/llm/default/default_openai_llm.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.4/agentuniverse/llm/llm.py` & `agentuniverse-0.0.5/agentuniverse/llm/llm.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding:utf-8 -*-
 
 # @Time    : 2024/4/2 16:04
 # @Author  : wangchongshi
 # @Email   : wangchongshi.wcs@antgroup.com
 # @FileName: llm.py
 from abc import abstractmethod
-from typing import Optional, Any
+from typing import Optional, Any, AsyncIterator, Iterator, Union
 from langchain_core.language_models.base import BaseLanguageModel
 
 from agentuniverse.base.component.component_base import ComponentBase
 from agentuniverse.base.component.component_enum import ComponentEnum
 from agentuniverse.base.config.application_configer.application_config_manager import ApplicationConfigManager
 from agentuniverse.base.config.component_configer.configers.llm_configer import LLMConfiger
 from agentuniverse.llm.llm_output import LLMOutput
@@ -54,19 +54,19 @@
         pass
 
     def _new_async_client(self):
         """Initialize the async client."""
         pass
 
     @abstractmethod
-    def call(self, *args: Any, **kwargs: Any) -> LLMOutput:
+    def call(self, *args: Any, **kwargs: Any) -> Union[LLMOutput, Iterator[LLMOutput]]:
         """Run the LLM."""
 
     @abstractmethod
-    async def acall(self, *args: Any, **kwargs: Any) -> LLMOutput:
+    async def acall(self, *args: Any, **kwargs: Any) -> Union[LLMOutput, AsyncIterator[LLMOutput]]:
         """Asynchronously run the LLM."""
 
     def as_langchain(self) -> BaseLanguageModel:
         """Convert to the langchain llm class."""
         pass
 
     def get_instance_code(self) -> str:
```

### Comparing `agentUniverse-0.0.4/agentuniverse/llm/llm_manager.py` & `agentuniverse-0.0.5/agentuniverse/llm/llm_manager.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.4/agentuniverse/llm/openai_llm.py` & `agentuniverse-0.0.5/agentuniverse/llm/openai_llm.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # !/usr/bin/env python3
 # -*- coding:utf-8 -*-
 
 # @Time    : 2024/4/2 16:15
 # @Author  : wangchongshi
 # @Email   : wangchongshi.wcs@antgroup.com
 # @FileName: openai_llm.py
-from typing import Any, Optional
+from typing import Any, Optional, AsyncIterator, Iterator, Union
 
 import httpx
 from langchain_core.language_models.base import BaseLanguageModel
 from openai import OpenAI, AsyncOpenAI
 from pydantic import Field
 import tiktoken
 
@@ -22,20 +22,22 @@
     "gpt-3.5-turbo-0301": 4096,
     "gpt-3.5-turbo-0613": 4096,
     "gpt-3.5-turbo-16k": 16384,
     "gpt-3.5-turbo-16k-0613": 16384,
     "gpt-35-turbo": 4096,
     "gpt-35-turbo-16k": 16384,
     "gpt-3.5-turbo-1106": 16384,
+    "gpt-3.5-turbo-0125": 16384,
     "gpt-4-0314": 8192,
     "gpt-4": 8192,
     "gpt-4-32k": 32768,
-    "gpt-4-32k-0314": 32768,
+    "gpt-4-32k-0613": 32768,
     "gpt-4-0613": 8192,
     "gpt-4-1106-preview": 128000,
+    "gpt-4-turbo": 128000,
 }
 
 
 class OpenAILLM(LLM):
     """The openai llm class.
 
     Attributes:
@@ -77,52 +79,57 @@
             base_url=self.openai_api_base,
             timeout=self.request_timeout,
             max_retries=self.max_retries,
             http_client=httpx.AsyncClient(proxy=self.openai_proxy) if self.openai_proxy else None,
             **(self.openai_client_args or {}),
         )
 
-    def call(self, messages: list, **kwargs: Any) -> LLMOutput:
+    def call(self, messages: list, **kwargs: Any) -> Union[LLMOutput, Iterator[LLMOutput]]:
         """Run the OpenAI LLM.
 
         Args:
             messages (list): The messages to send to the LLM.
             **kwargs: Arbitrary keyword arguments.
         """
+        streaming = kwargs.pop("streaming") if "streaming" in kwargs else self.streaming
         self.client = self._new_client()
         chat_completion = self.client.chat.completions.create(
             messages=messages,
             model=kwargs.pop('model', self.model_name),
             temperature=kwargs.pop('temperature', self.temperature),
-            stream=kwargs.pop('stream', self.streaming),
+            stream=kwargs.pop('stream', streaming),
             max_tokens=kwargs.pop('max_tokens', self.max_tokens),
             **kwargs,
         )
-        text = chat_completion.choices[0].message.content
-        return LLMOutput(text=text, raw=chat_completion.model_dump())
+        if not streaming:
+            text = chat_completion.choices[0].message.content
+            return LLMOutput(text=text, raw=chat_completion.model_dump())
+        return self.generate_stream_result(chat_completion)
 
-    async def acall(self, messages: list, **kwargs: Any) -> LLMOutput:
+    async def acall(self, messages: list, **kwargs: Any) -> Union[LLMOutput, AsyncIterator[LLMOutput]]:
         """Asynchronously run the OpenAI LLM.
 
         Args:
             messages (list): The messages to send to the LLM.
             **kwargs: Arbitrary keyword arguments.
         """
-
+        streaming = kwargs.pop("streaming") if "streaming" in kwargs else self.streaming
         self.async_client = self._new_async_client()
         chat_completion = await self.async_client.chat.completions.create(
             messages=messages,
             model=kwargs.pop('model', self.model_name),
             temperature=kwargs.pop('temperature', self.temperature),
-            stream=kwargs.pop('stream', self.streaming),
+            stream=kwargs.pop('stream', streaming),
             max_tokens=kwargs.pop('max_tokens', self.max_tokens),
             **kwargs,
         )
-        text = chat_completion.choices[0].message.content
-        return LLMOutput(text=text, raw=chat_completion.model_dump())
+        if not streaming:
+            text = chat_completion.choices[0].message.content
+            return LLMOutput(text=text, raw=chat_completion.model_dump())
+        return self.agenerate_stream_result(chat_completion)
 
     def as_langchain(self) -> BaseLanguageModel:
         """Convert the AgentUniverse(AU) openai llm class to the langchain openai llm class."""
         return LangchainOpenAI(self)
 
     def set_by_agent_model(self, **kwargs) -> None:
         """ Assign values of parameters to the OpenAILLM model in the agent configuration."""
@@ -155,7 +162,38 @@
             The integer number of tokens in the text.
         """
         try:
             encoding = tiktoken.encoding_for_model(self.model_name)
         except KeyError:
             encoding = tiktoken.get_encoding("cl100k_base")
         return len(encoding.encode(text))
+
+    @staticmethod
+    def parse_result(chunk):
+        """Generate the result of the stream."""
+        chat_completion = chunk
+        if not isinstance(chunk, dict):
+            chunk = chunk.dict()
+        if len(chunk["choices"]) == 0:
+            return
+        choice = chunk["choices"][0]
+        message = choice.get("delta")
+        text = message.get("content")
+        if not text:
+            return
+        return LLMOutput(text=text, raw=chat_completion.model_dump())
+
+    @classmethod
+    def generate_stream_result(cls, stream: Iterator) -> Iterator[LLMOutput]:
+        """Generate the result of the stream."""
+        for chunk in stream:
+            llm_output = cls.parse_result(chunk)
+            if llm_output:
+                yield llm_output
+
+    @classmethod
+    async def agenerate_stream_result(cls, stream: AsyncIterator) -> AsyncIterator[LLMOutput]:
+        """Generate the result of the stream."""
+        async for chunk in stream:
+            llm_output = cls.parse_result(chunk)
+            if llm_output:
+                yield llm_output
```

### Comparing `agentUniverse-0.0.4/agentuniverse/prompt/enum.py` & `agentuniverse-0.0.5/agentuniverse/prompt/enum.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.4/agentuniverse/prompt/prompt.py` & `agentuniverse-0.0.5/agentuniverse/prompt/prompt.py`

 * *Files 11% similar despite different names*

```diff
@@ -32,29 +32,27 @@
 
         Returns:
             PromptTemplate: The prompt template.
         """
         return PromptTemplate(template=self.prompt_template,
                               input_variables=self.input_variables)
 
-    def build_prompt(self, user_agent_prompt_model: AgentPromptModel, system_agent_prompt_model: AgentPromptModel,
-                     prompt_assemble_order: list[str]):
+    def build_prompt(self, agent_prompt_model: AgentPromptModel, prompt_assemble_order: list[str]) -> 'Prompt':
         """Build the prompt class.
 
         Args:
-            user_agent_prompt_model (AgentPromptModel): The user agent prompt model.
-            system_agent_prompt_model (AgentPromptModel): The system agent prompt model.
+            agent_prompt_model (AgentPromptModel): The user agent prompt model.
             prompt_assemble_order (list[str]): The prompt assemble ordered list.
 
         Returns:
             PromptTemplate: The prompt template.
         """
-        agent_prompt_model = user_agent_prompt_model + system_agent_prompt_model
         self.prompt_template = generate_template(agent_prompt_model, prompt_assemble_order)
         self.input_variables = re.findall(r'\{(.*?)}', self.prompt_template)
+        return self
 
     def get_instance_code(self) -> str:
         """Return the prompt version of the current prompt."""
         return self.prompt_version
 
     def initialize_by_component_configer(self, component_configer: PromptConfiger) -> 'Prompt':
         """Initialize the prompt by the PromptConfiger object.
```

### Comparing `agentUniverse-0.0.4/agentuniverse/prompt/prompt_manager.py` & `agentuniverse-0.0.5/agentuniverse/prompt/prompt_manager.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.4/agentuniverse_extension/logger/sls_sink.py` & `agentuniverse-0.0.5/agentuniverse_extension/logger/sls_sink.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.4/pyproject.toml` & `agentuniverse-0.0.5/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "agentUniverse"
-version = "0.0.4"
+version = "0.0.5"
 description = "agentUniverse is a framework for developing applications powered by multi-agent base on large language model."
 authors = ["AntGroup <AntGroup>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 requests = "^2.31.0"
```

### Comparing `agentUniverse-0.0.4/setup.py` & `agentuniverse-0.0.5/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,23 +18,23 @@
         requirements = content.split('\n')
 
     return requirements
 
 
 setuptools.setup(
     name="agentUniverse",
-    version="0.0.4",
+    version="0.0.5",
     author="AntGroup",
     author_email="jerry.zzw@antgroup.com",
     description="agentUniverse is a framework for developing applications powered "
                 "by multi-agent base on large language model.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitee.com/agentUniverse/agentUniverse",
-    packages=setuptools.find_packages(),
+    packages=setuptools.find_packages(exclude=["*sample_standard_app*", "*docs*", "*tests*"]),
     package_data={
             '': ['*.yaml'],
         },
     install_requires=read_requirements(),
     classifiers=[
         'Programming Language :: Python :: 3.10',
         "License :: OSI Approved :: Apache Software License",
```

