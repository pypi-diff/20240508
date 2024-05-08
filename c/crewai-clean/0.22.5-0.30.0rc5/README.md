# Comparing `tmp/crewai_clean-0.22.5.tar.gz` & `tmp/crewai_clean-0.30.0rc5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crewai_clean-0.22.5.tar", max compression
+gzip compressed data, was "crewai_clean-0.30.0rc5.tar", max compression
```

## Comparing `crewai_clean-0.22.5.tar` & `crewai_clean-0.30.0rc5.tar`

### file list

```diff
@@ -1,54 +1,72 @@
--rw-r--r--   0        0        0     1073 2024-03-30 22:31:12.151095 crewai_clean-0.22.5/LICENSE
--rw-r--r--   0        0        0    12085 2024-03-30 22:31:12.151095 crewai_clean-0.22.5/README.md
--rw-r--r--   0        0        0     1738 2024-03-30 22:31:12.387095 crewai_clean-0.22.5/pyproject.toml
--rw-r--r--   0        0        0      124 2024-03-30 22:31:12.159095 crewai_clean-0.22.5/src/crewai/__init__.py
--rw-r--r--   0        0        0    12809 2024-03-30 22:31:12.159095 crewai_clean-0.22.5/src/crewai/agent.py
--rw-r--r--   0        0        0      162 2024-03-30 22:31:12.159095 crewai_clean-0.22.5/src/crewai/agents/__init__.py
--rw-r--r--   0        0        0       40 2024-03-30 22:31:12.159095 crewai_clean-0.22.5/src/crewai/agents/cache/__init__.py
--rw-r--r--   0        0        0      356 2024-03-30 22:31:12.159095 crewai_clean-0.22.5/src/crewai/agents/cache/cache_handler.py
--rw-r--r--   0        0        0     8750 2024-03-30 22:31:12.159095 crewai_clean-0.22.5/src/crewai/agents/executor.py
--rw-r--r--   0        0        0     3662 2024-03-30 22:31:12.159095 crewai_clean-0.22.5/src/crewai/agents/parser.py
--rw-r--r--   0        0        0      793 2024-03-30 22:31:12.159095 crewai_clean-0.22.5/src/crewai/agents/tools_handler.py
--rw-r--r--   0        0        0        0 2024-03-30 22:31:12.159095 crewai_clean-0.22.5/src/crewai/cli/__init__.py
--rw-r--r--   0        0        0      307 2024-03-30 22:31:12.159095 crewai_clean-0.22.5/src/crewai/cli/cli.py
--rw-r--r--   0        0        0     2882 2024-03-30 22:31:12.159095 crewai_clean-0.22.5/src/crewai/cli/create_crew.py
--rw-r--r--   0        0        0       18 2024-03-30 22:31:12.159095 crewai_clean-0.22.5/src/crewai/cli/templates/.gitignore
--rw-r--r--   0        0        0     2476 2024-03-30 22:31:12.159095 crewai_clean-0.22.5/src/crewai/cli/templates/README.md
--rw-r--r--   0        0        0        0 2024-03-30 22:31:12.159095 crewai_clean-0.22.5/src/crewai/cli/templates/__init__.py
--rw-r--r--   0        0        0      739 2024-03-30 22:31:12.159095 crewai_clean-0.22.5/src/crewai/cli/templates/config/agents.yaml
--rw-r--r--   0        0        0      636 2024-03-30 22:31:12.159095 crewai_clean-0.22.5/src/crewai/cli/templates/config/tasks.yaml
--rw-r--r--   0        0        0     1521 2024-03-30 22:31:12.163095 crewai_clean-0.22.5/src/crewai/cli/templates/crew.py
--rw-r--r--   0        0        0      286 2024-03-30 22:31:12.163095 crewai_clean-0.22.5/src/crewai/cli/templates/main.py
--rw-r--r--   0        0        0      393 2024-03-30 22:31:12.163095 crewai_clean-0.22.5/src/crewai/cli/templates/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-30 22:31:12.163095 crewai_clean-0.22.5/src/crewai/cli/templates/tools/__init__.py
--rw-r--r--   0        0        0      383 2024-03-30 22:31:12.163095 crewai_clean-0.22.5/src/crewai/cli/templates/tools/custom_tool.py
--rw-r--r--   0        0        0    11902 2024-03-30 22:31:12.163095 crewai_clean-0.22.5/src/crewai/crew.py
--rw-r--r--   0        0        0      249 2024-03-30 22:31:12.163095 crewai_clean-0.22.5/src/crewai/process.py
--rw-r--r--   0        0        0       75 2024-03-30 22:31:12.163095 crewai_clean-0.22.5/src/crewai/project/__init__.py
--rw-r--r--   0        0        0     1568 2024-03-30 22:31:12.163095 crewai_clean-0.22.5/src/crewai/project/annotations.py
--rw-r--r--   0        0        0     1395 2024-03-30 22:31:12.163095 crewai_clean-0.22.5/src/crewai/project/crew_base.py
--rw-r--r--   0        0        0     8820 2024-03-30 22:31:12.163095 crewai_clean-0.22.5/src/crewai/task.py
--rw-r--r--   0        0        0        0 2024-03-30 22:31:12.163095 crewai_clean-0.22.5/src/crewai/tasks/__init__.py
--rw-r--r--   0        0        0      746 2024-03-30 22:31:12.163095 crewai_clean-0.22.5/src/crewai/tasks/task_output.py
--rw-r--r--   0        0        0       33 2024-03-30 22:31:12.163095 crewai_clean-0.22.5/src/crewai/telemetry/__init__.py
--rw-r--r--   0        0        0    11091 2024-03-30 22:31:12.163095 crewai_clean-0.22.5/src/crewai/telemetry/telemetry.py
--rw-r--r--   0        0        0        0 2024-03-30 22:31:12.163095 crewai_clean-0.22.5/src/crewai/tools/__init__.py
--rw-r--r--   0        0        0     2540 2024-03-30 22:31:12.163095 crewai_clean-0.22.5/src/crewai/tools/agent_tools.py
--rw-r--r--   0        0        0      857 2024-03-30 22:31:12.163095 crewai_clean-0.22.5/src/crewai/tools/cache_tools.py
--rw-r--r--   0        0        0      719 2024-03-30 22:31:12.163095 crewai_clean-0.22.5/src/crewai/tools/tool_calling.py
--rw-r--r--   0        0        0     1593 2024-03-30 22:31:12.163095 crewai_clean-0.22.5/src/crewai/tools/tool_output_parser.py
--rw-r--r--   0        0        0    11666 2024-03-30 22:31:12.163095 crewai_clean-0.22.5/src/crewai/tools/tool_usage.py
--rw-r--r--   0        0        0     6511 2024-03-30 22:31:12.163095 crewai_clean-0.22.5/src/crewai/translations/el.json
--rw-r--r--   0        0        0     5583 2024-03-30 22:31:12.163095 crewai_clean-0.22.5/src/crewai/translations/en.json
--rw-r--r--   0        0        0      234 2024-03-30 22:31:12.163095 crewai_clean-0.22.5/src/crewai/utilities/__init__.py
--rw-r--r--   0        0        0     3088 2024-03-30 22:31:12.163095 crewai_clean-0.22.5/src/crewai/utilities/converter.py
--rw-r--r--   0        0        0     1731 2024-03-30 22:31:12.163095 crewai_clean-0.22.5/src/crewai/utilities/crew_pydantic_output_parser.py
--rw-r--r--   0        0        0     1647 2024-03-30 22:31:12.163095 crewai_clean-0.22.5/src/crewai/utilities/i18n.py
--rw-r--r--   0        0        0     1635 2024-03-30 22:31:12.163095 crewai_clean-0.22.5/src/crewai/utilities/instructor.py
--rw-r--r--   0        0        0      552 2024-03-30 22:31:12.163095 crewai_clean-0.22.5/src/crewai/utilities/logger.py
--rw-r--r--   0        0        0      789 2024-03-30 22:31:12.163095 crewai_clean-0.22.5/src/crewai/utilities/printer.py
--rw-r--r--   0        0        0     1725 2024-03-30 22:31:12.163095 crewai_clean-0.22.5/src/crewai/utilities/prompts.py
--rw-r--r--   0        0        0     1468 2024-03-30 22:31:12.163095 crewai_clean-0.22.5/src/crewai/utilities/pydantic_schema_parser.py
--rw-r--r--   0        0        0     1786 2024-03-30 22:31:12.163095 crewai_clean-0.22.5/src/crewai/utilities/rpm_controller.py
--rw-r--r--   0        0        0     1974 2024-03-30 22:31:12.163095 crewai_clean-0.22.5/src/crewai/utilities/token_counter_callback.py
--rw-r--r--   0        0        0    13451 1970-01-01 00:00:00.000000 crewai_clean-0.22.5/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-05-08 08:15:12.145169 crewai_clean-0.30.0rc5/LICENSE
+-rw-r--r--   0        0        0    11847 2024-05-08 08:15:12.145169 crewai_clean-0.30.0rc5/README.md
+-rw-r--r--   0        0        0     1688 2024-05-08 08:15:12.429172 crewai_clean-0.30.0rc5/pyproject.toml
+-rw-r--r--   0        0        0      124 2024-05-08 08:15:12.157169 crewai_clean-0.30.0rc5/src/crewai/__init__.py
+-rw-r--r--   0        0        0    14603 2024-05-08 08:15:12.157169 crewai_clean-0.30.0rc5/src/crewai/agent.py
+-rw-r--r--   0        0        0      162 2024-05-08 08:15:12.157169 crewai_clean-0.30.0rc5/src/crewai/agents/__init__.py
+-rw-r--r--   0        0        0       40 2024-05-08 08:15:12.161169 crewai_clean-0.30.0rc5/src/crewai/agents/cache/__init__.py
+-rw-r--r--   0        0        0      356 2024-05-08 08:15:12.161169 crewai_clean-0.30.0rc5/src/crewai/agents/cache/cache_handler.py
+-rw-r--r--   0        0        0    12514 2024-05-08 08:15:12.161169 crewai_clean-0.30.0rc5/src/crewai/agents/executor.py
+-rw-r--r--   0        0        0     3661 2024-05-08 08:15:12.161169 crewai_clean-0.30.0rc5/src/crewai/agents/parser.py
+-rw-r--r--   0        0        0      978 2024-05-08 08:15:12.161169 crewai_clean-0.30.0rc5/src/crewai/agents/tools_handler.py
+-rw-r--r--   0        0        0        0 2024-05-08 08:15:12.161169 crewai_clean-0.30.0rc5/src/crewai/cli/__init__.py
+-rw-r--r--   0        0        0      307 2024-05-08 08:15:12.161169 crewai_clean-0.30.0rc5/src/crewai/cli/cli.py
+-rw-r--r--   0        0        0     2882 2024-05-08 08:15:12.161169 crewai_clean-0.30.0rc5/src/crewai/cli/create_crew.py
+-rw-r--r--   0        0        0       18 2024-05-08 08:15:12.161169 crewai_clean-0.30.0rc5/src/crewai/cli/templates/.gitignore
+-rw-r--r--   0        0        0     2480 2024-05-08 08:15:12.161169 crewai_clean-0.30.0rc5/src/crewai/cli/templates/README.md
+-rw-r--r--   0        0        0        0 2024-05-08 08:15:12.161169 crewai_clean-0.30.0rc5/src/crewai/cli/templates/__init__.py
+-rw-r--r--   0        0        0      739 2024-05-08 08:15:12.161169 crewai_clean-0.30.0rc5/src/crewai/cli/templates/config/agents.yaml
+-rw-r--r--   0        0        0      636 2024-05-08 08:15:12.161169 crewai_clean-0.30.0rc5/src/crewai/cli/templates/config/tasks.yaml
+-rw-r--r--   0        0        0     1521 2024-05-08 08:15:12.161169 crewai_clean-0.30.0rc5/src/crewai/cli/templates/crew.py
+-rw-r--r--   0        0        0      286 2024-05-08 08:15:12.161169 crewai_clean-0.30.0rc5/src/crewai/cli/templates/main.py
+-rw-r--r--   0        0        0      393 2024-05-08 08:15:12.161169 crewai_clean-0.30.0rc5/src/crewai/cli/templates/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-08 08:15:12.161169 crewai_clean-0.30.0rc5/src/crewai/cli/templates/tools/__init__.py
+-rw-r--r--   0        0        0      383 2024-05-08 08:15:12.161169 crewai_clean-0.30.0rc5/src/crewai/cli/templates/tools/custom_tool.py
+-rw-r--r--   0        0        0    15337 2024-05-08 08:15:12.161169 crewai_clean-0.30.0rc5/src/crewai/crew.py
+-rw-r--r--   0        0        0      160 2024-05-08 08:15:12.161169 crewai_clean-0.30.0rc5/src/crewai/memory/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-08 08:15:12.161169 crewai_clean-0.30.0rc5/src/crewai/memory/contextual/__init__.py
+-rw-r--r--   0        0        0     2409 2024-05-08 08:15:12.161169 crewai_clean-0.30.0rc5/src/crewai/memory/contextual/contextual_memory.py
+-rw-r--r--   0        0        0        0 2024-05-08 08:15:12.161169 crewai_clean-0.30.0rc5/src/crewai/memory/entity/__init__.py
+-rw-r--r--   0        0        0      791 2024-05-08 08:15:12.161169 crewai_clean-0.30.0rc5/src/crewai/memory/entity/entity_memory.py
+-rw-r--r--   0        0        0      301 2024-05-08 08:15:12.161169 crewai_clean-0.30.0rc5/src/crewai/memory/entity/entity_memory_item.py
+-rw-r--r--   0        0        0        0 2024-05-08 08:15:12.161169 crewai_clean-0.30.0rc5/src/crewai/memory/long_term/__init__.py
+-rw-r--r--   0        0        0     1132 2024-05-08 08:15:12.161169 crewai_clean-0.30.0rc5/src/crewai/memory/long_term/long_term_memory.py
+-rw-r--r--   0        0        0      507 2024-05-08 08:15:12.161169 crewai_clean-0.30.0rc5/src/crewai/memory/long_term/long_term_memory_item.py
+-rw-r--r--   0        0        0      598 2024-05-08 08:15:12.161169 crewai_clean-0.30.0rc5/src/crewai/memory/memory.py
+-rw-r--r--   0        0        0        0 2024-05-08 08:15:12.161169 crewai_clean-0.30.0rc5/src/crewai/memory/short_term/__init__.py
+-rw-r--r--   0        0        0      926 2024-05-08 08:15:12.161169 crewai_clean-0.30.0rc5/src/crewai/memory/short_term/short_term_memory.py
+-rw-r--r--   0        0        0      255 2024-05-08 08:15:12.161169 crewai_clean-0.30.0rc5/src/crewai/memory/short_term/short_term_memory_item.py
+-rw-r--r--   0        0        0      261 2024-05-08 08:15:12.161169 crewai_clean-0.30.0rc5/src/crewai/memory/storage/interface.py
+-rw-r--r--   0        0        0     3384 2024-05-08 08:15:12.161169 crewai_clean-0.30.0rc5/src/crewai/memory/storage/ltm_sqlite_storage.py
+-rw-r--r--   0        0        0     2988 2024-05-08 08:15:12.161169 crewai_clean-0.30.0rc5/src/crewai/memory/storage/rag_storage.py
+-rw-r--r--   0        0        0      249 2024-05-08 08:15:12.161169 crewai_clean-0.30.0rc5/src/crewai/process.py
+-rw-r--r--   0        0        0       75 2024-05-08 08:15:12.161169 crewai_clean-0.30.0rc5/src/crewai/project/__init__.py
+-rw-r--r--   0        0        0     1867 2024-05-08 08:15:12.161169 crewai_clean-0.30.0rc5/src/crewai/project/annotations.py
+-rw-r--r--   0        0        0     1395 2024-05-08 08:15:12.161169 crewai_clean-0.30.0rc5/src/crewai/project/crew_base.py
+-rw-r--r--   0        0        0    10943 2024-05-08 08:15:12.161169 crewai_clean-0.30.0rc5/src/crewai/task.py
+-rw-r--r--   0        0        0        0 2024-05-08 08:15:12.161169 crewai_clean-0.30.0rc5/src/crewai/tasks/__init__.py
+-rw-r--r--   0        0        0      746 2024-05-08 08:15:12.161169 crewai_clean-0.30.0rc5/src/crewai/tasks/task_output.py
+-rw-r--r--   0        0        0       33 2024-05-08 08:15:12.161169 crewai_clean-0.30.0rc5/src/crewai/telemetry/__init__.py
+-rw-r--r--   0        0        0    13021 2024-05-08 08:15:12.161169 crewai_clean-0.30.0rc5/src/crewai/telemetry/telemetry.py
+-rw-r--r--   0        0        0        0 2024-05-08 08:15:12.161169 crewai_clean-0.30.0rc5/src/crewai/tools/__init__.py
+-rw-r--r--   0        0        0     2705 2024-05-08 08:15:12.161169 crewai_clean-0.30.0rc5/src/crewai/tools/agent_tools.py
+-rw-r--r--   0        0        0      857 2024-05-08 08:15:12.161169 crewai_clean-0.30.0rc5/src/crewai/tools/cache_tools.py
+-rw-r--r--   0        0        0      719 2024-05-08 08:15:12.161169 crewai_clean-0.30.0rc5/src/crewai/tools/tool_calling.py
+-rw-r--r--   0        0        0     1593 2024-05-08 08:15:12.161169 crewai_clean-0.30.0rc5/src/crewai/tools/tool_output_parser.py
+-rw-r--r--   0        0        0    14895 2024-05-08 08:15:12.161169 crewai_clean-0.30.0rc5/src/crewai/tools/tool_usage.py
+-rw-r--r--   0        0        0     5685 2024-05-08 08:15:12.161169 crewai_clean-0.30.0rc5/src/crewai/translations/en.json
+-rw-r--r--   0        0        0      271 2024-05-08 08:15:12.161169 crewai_clean-0.30.0rc5/src/crewai/utilities/__init__.py
+-rw-r--r--   0        0        0     3088 2024-05-08 08:15:12.161169 crewai_clean-0.30.0rc5/src/crewai/utilities/converter.py
+-rw-r--r--   0        0        0     1731 2024-05-08 08:15:12.161169 crewai_clean-0.30.0rc5/src/crewai/utilities/crew_pydantic_output_parser.py
+-rw-r--r--   0        0        0     2446 2024-05-08 08:15:12.161169 crewai_clean-0.30.0rc5/src/crewai/utilities/evaluators/task_evaluator.py
+-rw-r--r--   0        0        0      709 2024-05-08 08:15:12.161169 crewai_clean-0.30.0rc5/src/crewai/utilities/fileHandler.py
+-rw-r--r--   0        0        0     1629 2024-05-08 08:15:12.161169 crewai_clean-0.30.0rc5/src/crewai/utilities/i18n.py
+-rw-r--r--   0        0        0     1635 2024-05-08 08:15:12.161169 crewai_clean-0.30.0rc5/src/crewai/utilities/instructor.py
+-rw-r--r--   0        0        0      552 2024-05-08 08:15:12.161169 crewai_clean-0.30.0rc5/src/crewai/utilities/logger.py
+-rw-r--r--   0        0        0      567 2024-05-08 08:15:12.161169 crewai_clean-0.30.0rc5/src/crewai/utilities/paths.py
+-rw-r--r--   0        0        0      789 2024-05-08 08:15:12.161169 crewai_clean-0.30.0rc5/src/crewai/utilities/printer.py
+-rw-r--r--   0        0        0     2297 2024-05-08 08:15:12.161169 crewai_clean-0.30.0rc5/src/crewai/utilities/prompts.py
+-rw-r--r--   0        0        0     1468 2024-05-08 08:15:12.161169 crewai_clean-0.30.0rc5/src/crewai/utilities/pydantic_schema_parser.py
+-rw-r--r--   0        0        0     1786 2024-05-08 08:15:12.161169 crewai_clean-0.30.0rc5/src/crewai/utilities/rpm_controller.py
+-rw-r--r--   0        0        0     1974 2024-05-08 08:15:12.161169 crewai_clean-0.30.0rc5/src/crewai/utilities/token_counter_callback.py
+-rw-r--r--   0        0        0    13256 1970-01-01 00:00:00.000000 crewai_clean-0.30.0rc5/PKG-INFO
```

### Comparing `crewai_clean-0.22.5/LICENSE` & `crewai_clean-0.30.0rc5/LICENSE`

 * *Files identical despite different names*

### Comparing `crewai_clean-0.22.5/README.md` & `crewai_clean-0.30.0rc5/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -26,15 +26,14 @@
   - [Quick Tutorial](#quick-tutorial)
   - [Write Job Descriptions](#write-job-descriptions)
   - [Trip Planner](#trip-planner)
   - [Stock Analysis](#stock-analysis)
 - [Connecting Your Crew to a Model](#connecting-your-crew-to-a-model)
 - [How CrewAI Compares](#how-crewai-compares)
 - [Contribution](#contribution)
-- [Hire CrewAI](#hire-crewai)
 - [Telemetry](#telemetry)
 - [License](#license)
 
 ## Why CrewAI?
 
 The power of AI collaboration has too much to offer.
 CrewAI is designed to enable AI agents to assume roles, share goals, and operate in a cohesive unit - much like a well-oiled crew. Whether you're building a smart assistant platform, an automated customer service ensemble, or a multi-agent research team, CrewAI provides the backbone for sophisticated multi-agent interactions.
@@ -45,15 +44,15 @@
 
 ### 1. Installation
 
 ```shell
 pip install crewai
 ```
 
-If you want to also install crewai-tools, which is a package with tools that can be used by the agents, but more dependencies, you can install it with, example below uses it:
+If you want to install the 'crewai' package along with its optional features that include additional tools for agents, you can do so by using the following command: pip install 'crewai[tools]'. This command installs the basic package and also adds extra components which require more dependencies to function."
 
 ```shell
 pip install 'crewai[tools]'
 ```
 
 ### 2. Setting Up Your Crew
 
@@ -79,15 +78,15 @@
   goal='Uncover cutting-edge developments in AI and data science',
   backstory="""You work at a leading tech think tank.
   Your expertise lies in identifying emerging trends.
   You have a knack for dissecting complex data and presenting actionable insights.""",
   verbose=True,
   allow_delegation=False,
   tools=[search_tool]
-  # You can pass an optional llm attribute specifying what mode you wanna use.
+  # You can pass an optional llm attribute specifying what model you wanna use.
   # It can be a local model through Ollama / LM Studio or a remote
   # model like OpenAI, Mistral, Antrophic or others (https://docs.crewai.com/how-to/LLM-Connections/)
   #
   # import os
   # os.environ['OPENAI_MODEL_NAME'] = 'gpt-3.5-turbo'
   #
   # OR
@@ -243,26 +242,22 @@
 
 ### Installing Locally
 
 ```bash
 pip install dist/*.tar.gz
 ```
 
-## Hire CrewAI
-
-We're a company developing crewAI and crewAI Enterprise, we for a limited time are offer consulting with selected customers, to get them early access to our enterprise solution
-If you are interested on having access to it and hiring weekly hours with our team, feel free to email us at [joao@crewai.com](mailto:joao@crewai.com).
-
 ## Telemetry
 
 CrewAI uses anonymous telemetry to collect usage data with the main purpose of helping us improve the library by focusing our efforts on the most used features, integrations and tools.
 
 There is NO data being collected on the prompts, tasks descriptions agents backstories or goals nor tools usage, no API calls, nor responses nor any data that is being processed by the agents, nor any secrets and env vars.
 
 Data collected includes:
+
 - Version of crewAI
   - So we can understand how many users are using the latest version
 - Version of Python
   - So we can decide on what versions to better support
 - General OS (e.g. number of CPUs, macOS/Windows/Linux)
   - So we know what OS we should focus on and if we could build specific OS related features
 - Number of agents and tasks in a crew
```

### Comparing `crewai_clean-0.22.5/pyproject.toml` & `crewai_clean-0.30.0rc5/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "crewai-clean"
-version = "0.22.5"
+version = "0.30.0rc5"
 description = "Cutting-edge framework for orchestrating role-playing, autonomous AI agents. By fostering collaborative intelligence, CrewAI empowers agents to work together seamlessly, tackling complex tasks."
 authors = ["Joao Moura <joao@crewai.com>"]
 readme = "README.md"
 packages = [
     { include = "crewai", from = "src" },
 ]
 
@@ -14,46 +14,47 @@
 Repository = "https://github.com/joaomdmoura/crewai"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<=3.13"
 pydantic = "^2.4.2"
 langchain = "^0.1.10"
 openai = "^1.13.3"
-langchain-openai = "^0.0.5"
 opentelemetry-api = "^1.22.0"
 opentelemetry-sdk = "^1.22.0"
 opentelemetry-exporter-otlp-proto-http = "^1.22.0"
 instructor = "^0.5.2"
 regex = "^2023.12.25"
-crewai-tools = { version = "^0.0.15", optional = true }
+crewai-tools = { version = "^0.2.3", optional = true }
 click = "^8.1.7"
-python-dotenv = "1.0.0"
+python-dotenv = "^1.0.0"
+embedchain = "^0.1.98"
+appdirs = "^1.4.4"
 
 [tool.poetry.extras]
 tools = ["crewai-tools"]
 
 [tool.poetry.group.dev.dependencies]
 isort = "^5.13.2"
 pyright = ">=1.1.350,<2.0.0"
-black = {git = "https://github.com/psf/black.git", rev = "stable"}
 autoflake = "^2.2.1"
 pre-commit = "^3.6.0"
 mkdocs = "^1.4.3"
 mkdocstrings = "^0.22.0"
 mkdocstrings-python = "^1.1.2"
 mkdocs-material = {extras = ["imaging"], version = "^9.5.7"}
 mkdocs-material-extensions = "^1.3.1"
 pillow = "^10.2.0"
 cairosvg = "^2.7.1"
-crewai_tools = "^0.0.15"
+crewai-tools = "^0.2.3"
 
 [tool.isort]
 profile = "black"
 known_first_party = ["crewai"]
 
+
 [tool.poetry.group.test.dependencies]
 pytest = "^8.0.0"
 pytest-vcr = "^1.0.2"
 python-dotenv = "1.0.0"
 
 [tool.poetry.scripts]
 crewai = "crewai.cli.cli:crewai"
```

### Comparing `crewai_clean-0.22.5/src/crewai/agent.py` & `crewai_clean-0.30.0rc5/src/crewai/agent.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import os
 import uuid
 from typing import Any, Dict, List, Optional, Tuple
 
 from langchain.agents.agent import RunnableAgent
 from langchain.agents.tools import tool as LangChainTool
-from langchain.memory import ConversationSummaryMemory
 from langchain.tools.render import render_text_description
 from langchain_core.agents import AgentAction
 from langchain_core.callbacks import BaseCallbackHandler
 from langchain_openai import ChatOpenAI
 from pydantic import (
     UUID4,
     BaseModel,
@@ -18,14 +17,15 @@
     PrivateAttr,
     field_validator,
     model_validator,
 )
 from pydantic_core import PydanticCustomError
 
 from crewai.agents import CacheHandler, CrewAgentExecutor, CrewAgentParser, ToolsHandler
+from crewai.memory.contextual.contextual_memory import ContextualMemory
 from crewai.utilities import I18N, Logger, Prompts, RPMController
 from crewai.utilities.token_counter_callback import TokenCalcHandler, TokenProcess
 
 
 class Agent(BaseModel):
     """Represents an agent in a system.
 
@@ -62,45 +62,51 @@
         default_factory=uuid.uuid4,
         frozen=True,
         description="Unique identifier for the object, not set by user.",
     )
     role: str = Field(description="Role of the agent")
     goal: str = Field(description="Objective of the agent")
     backstory: str = Field(description="Backstory of the agent")
+    cache: bool = Field(
+        default=True,
+        description="Whether the agent should use a cache for tool usage.",
+    )
     config: Optional[Dict[str, Any]] = Field(
         description="Configuration for the agent",
         default=None,
     )
     max_rpm: Optional[int] = Field(
         default=None,
         description="Maximum number of requests per minute for the agent execution to be respected.",
     )
-    memory: bool = Field(
-        default=False, description="Whether the agent should have memory or not"
-    )
     verbose: bool = Field(
         default=False, description="Verbose mode for the Agent Execution"
     )
     allow_delegation: bool = Field(
         default=True, description="Allow delegation of tasks to agents"
     )
     tools: Optional[List[Any]] = Field(
         default_factory=list, description="Tools at agents disposal"
     )
     max_iter: Optional[int] = Field(
-        default=15, description="Maximum iterations for an agent to execute a task"
+        default=25, description="Maximum iterations for an agent to execute a task"
+    )
+    max_execution_time: Optional[int] = Field(
+        default=None,
+        description="Maximum execution time for an agent to execute a task",
     )
     agent_executor: InstanceOf[CrewAgentExecutor] = Field(
         default=None, description="An instance of the CrewAgentExecutor class."
     )
+    crew: Any = Field(default=None, description="Crew to which the agent belongs.")
     tools_handler: InstanceOf[ToolsHandler] = Field(
         default=None, description="An instance of the ToolsHandler class."
     )
     cache_handler: InstanceOf[CacheHandler] = Field(
-        default=CacheHandler(), description="An instance of the CacheHandler class."
+        default=None, description="An instance of the CacheHandler class."
     )
     step_callback: Optional[Any] = Field(
         default=None,
         description="Callback to be executed after each step of the agent execution.",
     )
     i18n: I18N = Field(default=I18N(), description="Internationalization settings.")
     llm: Any = Field(
@@ -111,14 +117,23 @@
     )
     function_calling_llm: Optional[Any] = Field(
         description="Language model that will run the agent.", default=None
     )
     callbacks: Optional[List[InstanceOf[BaseCallbackHandler]]] = Field(
         default=None, description="Callback to be executed"
     )
+    system_template: Optional[str] = Field(
+        default=None, description="System format for the agent."
+    )
+    prompt_template: Optional[str] = Field(
+        default=None, description="Prompt format for the agent."
+    )
+    response_template: Optional[str] = Field(
+        default=None, description="Response format for the agent."
+    )
 
     _original_role: str | None = None
     _original_goal: str | None = None
     _original_backstory: str | None = None
 
     def __init__(__pydantic_self__, **data):
         config = data.pop("config", {})
@@ -150,18 +165,29 @@
             )
         return self
 
     @model_validator(mode="after")
     def set_agent_executor(self) -> "Agent":
         """set agent executor is set."""
         if hasattr(self.llm, "model_name"):
-            self.llm.callbacks = [
-                TokenCalcHandler(self.llm.model_name, self._token_process)
-            ]
+            token_handler = TokenCalcHandler(self.llm.model_name, self._token_process)
+
+            # Ensure self.llm.callbacks is a list
+            if not isinstance(self.llm.callbacks, list):
+                self.llm.callbacks = []
+
+            # Check if an instance of TokenCalcHandler already exists in the list
+            if not any(
+                isinstance(handler, TokenCalcHandler) for handler in self.llm.callbacks
+            ):
+                self.llm.callbacks.append(token_handler)
+
         if not self.agent_executor:
+            if not self.cache_handler:
+                self.cache_handler = CacheHandler()
             self.set_cache_handler(self.cache_handler)
         return self
 
     def execute_task(
         self,
         task: Any,
         context: Optional[str] = None,
@@ -173,30 +199,43 @@
             task: Task to execute.
             context: Context to execute the task in.
             tools: Tools to use for the task.
 
         Returns:
             Output of the agent
         """
-        self.tools_handler.last_used_tool = {}
+        if self.tools_handler:
+            self.tools_handler.last_used_tool = {}
 
         task_prompt = task.prompt()
 
         if context:
             task_prompt = self.i18n.slice("task_with_context").format(
                 task=task_prompt, context=context
             )
 
-        tools = self._parse_tools(tools or self.tools)
+        if self.crew and self.crew.memory:
+            contextual_memory = ContextualMemory(
+                self.crew._short_term_memory,
+                self.crew._long_term_memory,
+                self.crew._entity_memory,
+            )
+            memory = contextual_memory.build_context_for_task(task, context)
+            if memory.strip() != "":
+                task_prompt += self.i18n.slice("memory").format(memory=memory)
+
+        tools = tools or self.tools
+        parsed_tools = self._parse_tools(tools)
+
         self.create_agent_executor(tools=tools)
-        self.agent_executor.tools = tools
+        self.agent_executor.tools = parsed_tools
         self.agent_executor.task = task
 
-        self.agent_executor.tools_description = render_text_description(tools)
-        self.agent_executor.tools_names = self.__tools_names(tools)
+        self.agent_executor.tools_description = render_text_description(parsed_tools)
+        self.agent_executor.tools_names = self.__tools_names(parsed_tools)
 
         result = self.agent_executor.invoke(
             {
                 "input": task_prompt,
                 "tool_names": self.agent_executor.tools_names,
                 "tools": self.agent_executor.tools_description,
             }
@@ -209,16 +248,18 @@
 
     def set_cache_handler(self, cache_handler: CacheHandler) -> None:
         """Set the cache handler for the agent.
 
         Args:
             cache_handler: An instance of the CacheHandler class.
         """
-        self.cache_handler = cache_handler
-        self.tools_handler = ToolsHandler(cache=self.cache_handler)
+        self.tools_handler = ToolsHandler()
+        if self.cache:
+            self.cache_handler = cache_handler
+            self.tools_handler.cache = cache_handler
         self.create_agent_executor()
 
     def set_rpm_controller(self, rpm_controller: RPMController) -> None:
         """Set the rpm controller for the agent.
 
         Args:
             rpm_controller: An instance of the RPMController class.
@@ -243,46 +284,54 @@
                 x["intermediate_steps"]
             ),
         }
 
         executor_args = {
             "llm": self.llm,
             "i18n": self.i18n,
+            "crew": self.crew,
+            "crew_agent": self,
             "tools": self._parse_tools(tools),
             "verbose": self.verbose,
+            "original_tools": tools,
             "handle_parsing_errors": True,
             "max_iterations": self.max_iter,
+            "max_execution_time": self.max_execution_time,
             "step_callback": self.step_callback,
             "tools_handler": self.tools_handler,
             "function_calling_llm": self.function_calling_llm,
             "callbacks": self.callbacks,
         }
 
         if self._rpm_controller:
             executor_args[
                 "request_within_rpm_limit"
             ] = self._rpm_controller.check_or_wait
 
-        if self.memory:
-            summary_memory = ConversationSummaryMemory(
-                llm=self.llm, input_key="input", memory_key="chat_history"
-            )
-            executor_args["memory"] = summary_memory
-            agent_args["chat_history"] = lambda x: x["chat_history"]
-            prompt = Prompts(i18n=self.i18n, tools=tools).task_execution_with_memory()
-        else:
-            prompt = Prompts(i18n=self.i18n, tools=tools).task_execution()
+        prompt = Prompts(
+            i18n=self.i18n,
+            tools=tools,
+            system_template=self.system_template,
+            prompt_template=self.prompt_template,
+            response_template=self.response_template,
+        ).task_execution()
 
         execution_prompt = prompt.partial(
             goal=self.goal,
             role=self.role,
             backstory=self.backstory,
         )
 
-        bind = self.llm.bind(stop=[self.i18n.slice("observation")])
+        stop_words = [self.i18n.slice("observation")]
+        if self.response_template:
+            stop_words.append(
+                self.response_template.split("{{ .Response }}")[1].strip()
+            )
+
+        bind = self.llm.bind(stop=stop_words)
         inner_agent = agent_args | execution_prompt | bind | CrewAgentParser(agent=self)
         self.agent_executor = CrewAgentExecutor(
             agent=RunnableAgent(runnable=inner_agent), **executor_args
         )
 
     def interpolate_inputs(self, inputs: Dict[str, Any]) -> None:
         """Interpolate inputs into the agent description and backstory."""
```

### Comparing `crewai_clean-0.22.5/src/crewai/agents/executor.py` & `crewai_clean-0.30.0rc5/src/crewai/agents/executor.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,67 +1,131 @@
+import threading
 import time
 from typing import Any, Dict, Iterator, List, Optional, Tuple, Union
 
 from langchain.agents import AgentExecutor
 from langchain.agents.agent import ExceptionTool
 from langchain.callbacks.manager import CallbackManagerForChainRun
 from langchain_core.agents import AgentAction, AgentFinish, AgentStep
 from langchain_core.exceptions import OutputParserException
 from langchain_core.pydantic_v1 import root_validator
 from langchain_core.tools import BaseTool
 from langchain_core.utils.input import get_color_mapping
 from pydantic import InstanceOf
 
 from crewai.agents.tools_handler import ToolsHandler
+from crewai.memory.entity.entity_memory_item import EntityMemoryItem
+from crewai.memory.long_term.long_term_memory_item import LongTermMemoryItem
+from crewai.memory.short_term.short_term_memory_item import ShortTermMemoryItem
 from crewai.tools.tool_usage import ToolUsage, ToolUsageErrorException
 from crewai.utilities import I18N
+from crewai.utilities.converter import ConverterError
+from crewai.utilities.evaluators.task_evaluator import TaskEvaluator
 
 
 class CrewAgentExecutor(AgentExecutor):
     _i18n: I18N = I18N()
+    should_ask_for_human_input: bool = False
     llm: Any = None
     iterations: int = 0
     task: Any = None
     tools_description: str = ""
     tools_names: str = ""
+    original_tools: List[Any] = []
+    crew_agent: Any = None
+    crew: Any = None
     function_calling_llm: Any = None
     request_within_rpm_limit: Any = None
     tools_handler: InstanceOf[ToolsHandler] = None
     max_iterations: Optional[int] = 15
     have_forced_answer: bool = False
     force_answer_max_iterations: Optional[int] = None
     step_callback: Optional[Any] = None
+    system_template: Optional[str] = None
+    prompt_template: Optional[str] = None
+    response_template: Optional[str] = None
 
     @root_validator()
     def set_force_answer_max_iterations(cls, values: Dict) -> Dict:
         values["force_answer_max_iterations"] = values["max_iterations"] - 2
         return values
 
     def _should_force_answer(self) -> bool:
         return (
             self.iterations == self.force_answer_max_iterations
         ) and not self.have_forced_answer
 
+    def _create_short_term_memory(self, output) -> None:
+        if (
+            self.crew
+            and self.crew.memory
+            and "Action: Delegate work to co-worker" not in output.log
+        ):
+            memory = ShortTermMemoryItem(
+                data=output.log,
+                agent=self.crew_agent.role,
+                metadata={
+                    "observation": self.task.description,
+                },
+            )
+            self.crew._short_term_memory.save(memory)
+
+    def _create_long_term_memory(self, output) -> None:
+        if self.crew and self.crew.memory:
+            ltm_agent = TaskEvaluator(self.crew_agent)
+            evaluation = ltm_agent.evaluate(self.task, output.log)
+
+            if isinstance(evaluation, ConverterError):
+                return
+
+            long_term_memory = LongTermMemoryItem(
+                task=self.task.description,
+                agent=self.crew_agent.role,
+                quality=evaluation.quality,
+                datetime=str(time.time()),
+                expected_output=self.task.expected_output,
+                metadata={
+                    "suggestions": evaluation.suggestions,
+                    "quality": evaluation.quality,
+                },
+            )
+            self.crew._long_term_memory.save(long_term_memory)
+
+            for entity in evaluation.entities:
+                entity_memory = EntityMemoryItem(
+                    name=entity.name,
+                    type=entity.type,
+                    description=entity.description,
+                    relationships="\n".join([f"- {r}" for r in entity.relationships]),
+                )
+                self.crew._entity_memory.save(entity_memory)
+
     def _call(
         self,
         inputs: Dict[str, str],
         run_manager: Optional[CallbackManagerForChainRun] = None,
     ) -> Dict[str, Any]:
         """Run text through and get agent response."""
         # Construct a mapping of tool name to tool for easy lookup
         name_to_tool_map = {tool.name: tool for tool in self.tools}
         # We construct a mapping from each tool to a color, used for logging.
         color_mapping = get_color_mapping(
-            [tool.name for tool in self.tools], excluded_colors=["green", "red"]
+            [tool.name.casefold() for tool in self.tools],
+            excluded_colors=["green", "red"],
         )
         intermediate_steps: List[Tuple[AgentAction, str]] = []
+        # Allowing human input given task setting
+        if self.task.human_input:
+            self.should_ask_for_human_input = True
+
         # Let's start tracking the number of iterations and time elapsed
         self.iterations = 0
         time_elapsed = 0.0
         start_time = time.time()
+
         # We now enter the agent loop (until it returns something).
         while self._should_continue(self.iterations, time_elapsed):
             if not self.request_within_rpm_limit or self.request_within_rpm_limit():
                 next_step_output = self._take_next_step(
                     name_to_tool_map,
                     color_mapping,
                     inputs,
@@ -69,32 +133,41 @@
                     run_manager=run_manager,
                 )
 
                 if self.step_callback:
                     self.step_callback(next_step_output)
 
                 if isinstance(next_step_output, AgentFinish):
+                    # Creating long term memory
+                    create_long_term_memory = threading.Thread(
+                        target=self._create_long_term_memory, args=(next_step_output,)
+                    )
+                    create_long_term_memory.start()
+
                     return self._return(
                         next_step_output, intermediate_steps, run_manager=run_manager
                     )
 
                 intermediate_steps.extend(next_step_output)
+
                 if len(next_step_output) == 1:
                     next_step_action = next_step_output[0]
                     # See if tool should return directly
                     tool_return = self._get_tool_return(next_step_action)
                     if tool_return is not None:
                         return self._return(
                             tool_return, intermediate_steps, run_manager=run_manager
                         )
+
                 self.iterations += 1
                 time_elapsed = time.time() - start_time
         output = self.agent.return_stopped_response(
             self.early_stopping_method, intermediate_steps, **inputs
         )
+
         return self._return(output, intermediate_steps, run_manager=run_manager)
 
     def _iter_next_step(
         self,
         name_to_tool_map: Dict[str, BaseTool],
         color_mapping: Dict[str, str],
         inputs: Dict[str, str],
@@ -110,14 +183,15 @@
                 error = self._i18n.errors("force_final_answer")
                 output = AgentAction("_Exception", error, error)
                 self.have_forced_answer = True
                 yield AgentStep(action=output, observation=error)
                 return
 
             intermediate_steps = self._prepare_intermediate_steps(intermediate_steps)
+
             # Call the LLM to see what to do.
             output = self.agent.plan(
                 intermediate_steps,
                 callbacks=run_manager.get_child() if run_manager else None,
                 **inputs,
             )
 
@@ -143,16 +217,18 @@
             elif isinstance(self.handle_parsing_errors, str):
                 observation = f"\n{self.handle_parsing_errors}"
             elif callable(self.handle_parsing_errors):
                 observation = f"\n{self.handle_parsing_errors(e)}"
             else:
                 raise ValueError("Got unexpected type of `handle_parsing_errors`")
             output = AgentAction("_Exception", observation, "")
+
             if run_manager:
                 run_manager.on_agent_action(output, color="green")
+
             tool_run_kwargs = self.agent.tool_run_logging_kwargs()
             observation = ExceptionTool().run(
                 output.tool_input,
                 verbose=False,
                 color=None,
                 callbacks=run_manager.get_child() if run_manager else None,
                 **tool_run_kwargs,
@@ -165,41 +241,67 @@
                 return
 
             yield AgentStep(action=output, observation=observation)
             return
 
         # If the tool chosen is the finishing tool, then we end and return.
         if isinstance(output, AgentFinish):
-            yield output
-            return
+            if self.should_ask_for_human_input:
+                # Making sure we only ask for it once, so disabling for the next thought loop
+                self.should_ask_for_human_input = False
+                human_feedback = self._ask_human_input(output.return_values["output"])
+                action = AgentAction(
+                    tool="Human Input", tool_input=human_feedback, log=output.log
+                )
+                yield AgentStep(
+                    action=action,
+                    observation=self._i18n.slice("human_feedback").format(
+                        human_feedback=human_feedback
+                    ),
+                )
+                return
+
+            else:
+                yield output
+                return
+
+        self._create_short_term_memory(output)
 
         actions: List[AgentAction]
         actions = [output] if isinstance(output, AgentAction) else output
         yield from actions
+
         for agent_action in actions:
             if run_manager:
                 run_manager.on_agent_action(agent_action, color="green")
-            # Otherwise we lookup the tool
+
             tool_usage = ToolUsage(
                 tools_handler=self.tools_handler,
                 tools=self.tools,
+                original_tools=self.original_tools,
                 tools_description=self.tools_description,
                 tools_names=self.tools_names,
                 function_calling_llm=self.function_calling_llm,
                 task=self.task,
                 action=agent_action,
             )
             tool_calling = tool_usage.parse(agent_action.log)
 
             if isinstance(tool_calling, ToolUsageErrorException):
                 observation = tool_calling.message
             else:
-                if tool_calling.tool_name.lower().strip() in [
-                    name.lower().strip() for name in name_to_tool_map
+                if tool_calling.tool_name.casefold().strip() in [
+                    name.casefold().strip() for name in name_to_tool_map
                 ]:
                     observation = tool_usage.use(tool_calling, agent_action.log)
                 else:
                     observation = self._i18n.errors("wrong_tool_name").format(
                         tool=tool_calling.tool_name,
-                        tools=", ".join([tool.name for tool in self.tools]),
+                        tools=", ".join([tool.name.casefold() for tool in self.tools]),
                     )
             yield AgentStep(action=agent_action, observation=observation)
+
+    def _ask_human_input(self, final_answer: dict) -> str:
+        """Get human input."""
+        return input(
+            self._i18n.slice("getting_input").format(final_answer=final_answer)
+        )
```

### Comparing `crewai_clean-0.22.5/src/crewai/agents/parser.py` & `crewai_clean-0.30.0rc5/src/crewai/agents/parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,14 @@
                 raise OutputParserException(
                     f"{FINAL_ANSWER_AND_PARSABLE_ACTION_ERROR_MESSAGE}: {text}"
                 )
             action = action_match.group(1).strip()
             action_input = action_match.group(2)
             tool_input = action_input.strip(" ")
             tool_input = tool_input.strip('"')
-
             return AgentAction(action, tool_input, text)
 
         elif includes_answer:
             return AgentFinish(
                 {"output": text.split(FINAL_ANSWER_ACTION)[-1].strip()}, text
             )
```

### Comparing `crewai_clean-0.22.5/src/crewai/agents/tools_handler.py` & `crewai_clean-0.30.0rc5/src/crewai/agents/tools_handler.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,32 @@
-from typing import Any
+from typing import Any, Optional, Union
 
 from ..tools.cache_tools import CacheTools
-from ..tools.tool_calling import ToolCalling
+from ..tools.tool_calling import InstructorToolCalling, ToolCalling
 from .cache.cache_handler import CacheHandler
 
 
 class ToolsHandler:
     """Callback handler for tool usage."""
 
     last_used_tool: ToolCalling = {}
     cache: CacheHandler
 
-    def __init__(self, cache: CacheHandler):
+    def __init__(self, cache: Optional[CacheHandler] = None):
         """Initialize the callback handler."""
         self.cache = cache
         self.last_used_tool = {}
 
-    def on_tool_use(self, calling: ToolCalling, output: str) -> Any:
+    def on_tool_use(
+        self,
+        calling: Union[ToolCalling, InstructorToolCalling],
+        output: str,
+        should_cache: bool = True,
+    ) -> Any:
         """Run when tool ends running."""
         self.last_used_tool = calling
-        if calling.tool_name != CacheTools().name:
+        if self.cache and should_cache and calling.tool_name != CacheTools().name:
             self.cache.add(
                 tool=calling.tool_name,
                 input=calling.arguments,
                 output=output,
             )
```

### Comparing `crewai_clean-0.22.5/src/crewai/cli/create_crew.py` & `crewai_clean-0.30.0rc5/src/crewai/cli/create_crew.py`

 * *Files identical despite different names*

### Comparing `crewai_clean-0.22.5/src/crewai/cli/templates/README.md` & `crewai_clean-0.30.0rc5/src/crewai/cli/templates/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 poetry lock
 ```
 ```bash
 poetry install
 ```
 ### Customizing
 
-**Add you `OPENAI_API_KEY` on the `.env` file**
+**Add your `OPENAI_API_KEY` into the `.env` file**
 
 - Modify `src/{{folder_name}}/config/agents.yaml` to define your agents
 - Modify `src/{{folder_name}}/config/tasks.yaml` to define your tasks
 - Modify `src/{{folder_name}}/crew.py` to add your own logic, tools and specific args
 - Modify `src/{{folder_name}}/main.py` to add custom inputs for your agents and tasks
 
 ## Running the Project
@@ -36,22 +36,22 @@
 
 ```bash
 poetry run {{folder_name}}
 ```
 
 This command initializes the {{name}} Crew, assembling the agents and assigning them tasks as defined in your configuration.
 
-This example, unmodified, will run the create a `report.md` file with the output of a research on LLMs in the root folser
+This example, unmodified, will run the create a `report.md` file with the output of a research on LLMs in the root folder.
 
 ## Understanding Your Crew
 
 The {{name}} Crew is composed of multiple AI agents, each with unique roles, goals, and tools. These agents collaborate on a series of tasks, defined in `config/tasks.yaml`, leveraging their collective skills to achieve complex objectives. The `config/agents.yaml` file outlines the capabilities and configurations of each agent in your crew.
 
 ## Support
 
 For support, questions, or feedback regarding the {{crew_name}} Crew or crewAI.
 - Visit our [documentation](https://docs.crewai.com)
 - Reach out to us through our [GitHub repository](https://github.com/joaomdmoura/crewai)
-- [Joing our Discord](https://discord.com/invite/X4JWnZnxPb)
-- [Chat wtih our docs](https://chatg.pt/DWjSBZn)
+- [Join our Discord](https://discord.com/invite/X4JWnZnxPb)
+- [Chat with our docs](https://chatg.pt/DWjSBZn)
 
-Let's create wonders together with the power and simplicity of crewAI.
+Let's create wonders together with the power and simplicity of crewAI.
```

### Comparing `crewai_clean-0.22.5/src/crewai/cli/templates/config/agents.yaml` & `crewai_clean-0.30.0rc5/src/crewai/cli/templates/config/agents.yaml`

 * *Files identical despite different names*

### Comparing `crewai_clean-0.22.5/src/crewai/cli/templates/config/tasks.yaml` & `crewai_clean-0.30.0rc5/src/crewai/cli/templates/config/tasks.yaml`

 * *Files identical despite different names*

### Comparing `crewai_clean-0.22.5/src/crewai/cli/templates/crew.py` & `crewai_clean-0.30.0rc5/src/crewai/cli/templates/crew.py`

 * *Files identical despite different names*

### Comparing `crewai_clean-0.22.5/src/crewai/crew.py` & `crewai_clean-0.30.0rc5/src/crewai/crew.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,83 +14,116 @@
     field_validator,
     model_validator,
 )
 from pydantic_core import PydanticCustomError
 
 from crewai.agent import Agent
 from crewai.agents.cache import CacheHandler
+from crewai.memory.entity.entity_memory import EntityMemory
+from crewai.memory.long_term.long_term_memory import LongTermMemory
+from crewai.memory.short_term.short_term_memory import ShortTermMemory
 from crewai.process import Process
 from crewai.task import Task
 from crewai.telemetry import Telemetry
 from crewai.tools.agent_tools import AgentTools
-from crewai.utilities import I18N, Logger, RPMController
+from crewai.utilities import I18N, FileHandler, Logger, RPMController
 
 
 class Crew(BaseModel):
     """
     Represents a group of agents, defining how they should collaborate and the tasks they should perform.
 
     Attributes:
         tasks: List of tasks assigned to the crew.
         agents: List of agents part of this crew.
         manager_llm: The language model that will run manager agent.
+        manager_agent: Custom agent that will be used as manager.
+        memory: Whether the crew should use memory to store memories of it's execution.
         manager_callbacks: The callback handlers to be executed by the manager agent when hierarchical process is used
+        cache: Whether the crew should use a cache to store the results of the tools execution.
         function_calling_llm: The language model that will run the tool calling for all the agents.
-        process: The process flow that the crew will follow (e.g., sequential).
+        process: The process flow that the crew will follow (e.g., sequential, hierarchical).
         verbose: Indicates the verbosity level for logging during execution.
         config: Configuration settings for the crew.
         max_rpm: Maximum number of requests per minute for the crew execution to be respected.
+        prompt_file: Path to the prompt json file to be used for the crew.
         id: A unique identifier for the crew instance.
         full_output: Whether the crew should return the full output with all tasks outputs or just the final output.
+        task_callback: Callback to be executed after each task for every agents execution.
         step_callback: Callback to be executed after each step for every agents execution.
         share_crew: Whether you want to share the complete crew infromation and execution with crewAI to make the library better, and allow us to train models.
     """
 
     __hash__ = object.__hash__  # type: ignore
     _execution_span: Any = PrivateAttr()
     _rpm_controller: RPMController = PrivateAttr()
     _logger: Logger = PrivateAttr()
+    _file_handler: FileHandler = PrivateAttr()
     _cache_handler: InstanceOf[CacheHandler] = PrivateAttr(default=CacheHandler())
+    _short_term_memory: Optional[InstanceOf[ShortTermMemory]] = PrivateAttr()
+    _long_term_memory: Optional[InstanceOf[LongTermMemory]] = PrivateAttr()
+    _entity_memory: Optional[InstanceOf[EntityMemory]] = PrivateAttr()
+
+    cache: bool = Field(default=True)
     model_config = ConfigDict(arbitrary_types_allowed=True)
     tasks: List[Task] = Field(default_factory=list)
     agents: List[Agent] = Field(default_factory=list)
     process: Process = Field(default=Process.sequential)
     verbose: Union[int, bool] = Field(default=0)
+    memory: bool = Field(
+        default=False,
+        description="Whether the crew should use memory to store memories of it's execution",
+    )
+    embedder: Optional[dict] = Field(
+        default={"provider": "openai"},
+        description="Configuration for the embedder to be used for the crew.",
+    )
     usage_metrics: Optional[dict] = Field(
         default=None,
         description="Metrics for the LLM usage during all tasks execution.",
     )
     full_output: Optional[bool] = Field(
         default=False,
         description="Whether the crew should return the full output with all tasks outputs or just the final output.",
     )
     manager_llm: Optional[Any] = Field(
         description="Language model that will run the agent.", default=None
     )
+    manager_agent: Optional[Any] = Field(
+        description="Custom agent that will be used as manager.", default=None
+    )
     manager_callbacks: Optional[List[InstanceOf[BaseCallbackHandler]]] = Field(
         default=None,
         description="A list of callback handlers to be executed by the manager agent when hierarchical process is used",
     )
     function_calling_llm: Optional[Any] = Field(
         description="Language model that will run the agent.", default=None
     )
     config: Optional[Union[Json, Dict[str, Any]]] = Field(default=None)
     id: UUID4 = Field(default_factory=uuid.uuid4, frozen=True)
     share_crew: Optional[bool] = Field(default=False)
     step_callback: Optional[Any] = Field(
         default=None,
         description="Callback to be executed after each step for all agents execution.",
     )
+    task_callback: Optional[Any] = Field(
+        default=None,
+        description="Callback to be executed after each task for all agents execution.",
+    )
     max_rpm: Optional[int] = Field(
         default=None,
         description="Maximum number of requests per minute for the crew execution to be respected.",
     )
-    language: str = Field(
-        default="en",
-        description="Language used for the crew, defaults to English.",
+    prompt_file: str = Field(
+        default=None,
+        description="Path to the prompt json file to be used for the crew.",
+    )
+    output_log_file: Optional[Union[bool, str]] = Field(
+        default=False,
+        description="output_log_file",
     )
 
     @field_validator("id", mode="before")
     @classmethod
     def _deny_user_set_id(cls, v: Optional[UUID4]) -> None:
         """Prevent manual setting of the 'id' field by users."""
         if v:
@@ -114,27 +147,40 @@
         return json.loads(v) if isinstance(v, Json) else v  # type: ignore
 
     @model_validator(mode="after")
     def set_private_attrs(self) -> "Crew":
         """Set private attributes."""
         self._cache_handler = CacheHandler()
         self._logger = Logger(self.verbose)
+        if self.output_log_file:
+            self._file_handler = FileHandler(self.output_log_file)
         self._rpm_controller = RPMController(max_rpm=self.max_rpm, logger=self._logger)
         self._telemetry = Telemetry()
         self._telemetry.set_tracer()
         self._telemetry.crew_creation(self)
         return self
 
     @model_validator(mode="after")
+    def create_crew_memory(self) -> "Crew":
+        """Set private attributes."""
+        if self.memory:
+            self._long_term_memory = LongTermMemory()
+            self._short_term_memory = ShortTermMemory(embedder_config=self.embedder)
+            self._entity_memory = EntityMemory(embedder_config=self.embedder)
+        return self
+
+    @model_validator(mode="after")
     def check_manager_llm(self):
         """Validates that the language model is set when using hierarchical process."""
-        if self.process == Process.hierarchical and not self.manager_llm:
+        if self.process == Process.hierarchical and (
+            not self.manager_llm and not self.manager_agent
+        ):
             raise PydanticCustomError(
-                "missing_manager_llm",
-                "Attribute `manager_llm` is required when using hierarchical process.",
+                "missing_manager_llm_or_manager_agent",
+                "Attribute `manager_llm` or `manager_agent` is required when using hierarchical process.",
                 {},
             )
         return self
 
     @model_validator(mode="after")
     def check_config(self):
         """Validates that the crew is properly configured with agents and tasks."""
@@ -146,15 +192,16 @@
             )
 
         if self.config:
             self._setup_from_config()
 
         if self.agents:
             for agent in self.agents:
-                agent.set_cache_handler(self._cache_handler)
+                if self.cache:
+                    agent.set_cache_handler(self._cache_handler)
                 if self.max_rpm:
                     agent.set_rpm_controller(self._rpm_controller)
         return self
 
     def _setup_from_config(self):
         assert self.config is not None, "Config should not be None."
 
@@ -183,24 +230,28 @@
         del task_config["agent"]
         return Task(**task_config, agent=task_agent)
 
     def kickoff(self, inputs: Optional[Dict[str, Any]] = {}) -> str:
         """Starts the crew to work on its assigned tasks."""
         self._execution_span = self._telemetry.crew_execution_span(self)
         self._interpolate_inputs(inputs)
+        self._set_tasks_callbacks()
+
+        i18n = I18N(prompt_file=self.prompt_file)
 
         for agent in self.agents:
-            agent.i18n = I18N(language=self.language)
+            agent.i18n = i18n
+            agent.crew = self
 
             if not agent.function_calling_llm:
                 agent.function_calling_llm = self.function_calling_llm
-                agent.create_agent_executor()
             if not agent.step_callback:
                 agent.step_callback = self.step_callback
-                agent.create_agent_executor()
+
+            agent.create_agent_executor()
 
         metrics = []
 
         if self.process == Process.sequential:
             result = self._run_sequential_process()
         elif self.process == Process.hierarchical:
             result, manager_metrics = self._run_hierarchical_process()
@@ -228,56 +279,86 @@
                 agents_for_delegation = [
                     agent for agent in self.agents if agent != task.agent
                 ]
                 if len(self.agents) > 1 and len(agents_for_delegation) > 0:
                     task.tools += AgentTools(agents=agents_for_delegation).tools()
 
             role = task.agent.role if task.agent is not None else "None"
-            self._logger.log("debug", f"== Working Agent: {role}", color="bold_yellow")
+            self._logger.log("debug", f"== Working Agent: {role}", color="bold_purple")
             self._logger.log(
-                "info", f"== Starting Task: {task.description}", color="bold_yellow"
+                "info", f"== Starting Task: {task.description}", color="bold_purple"
             )
 
+            if self.output_log_file:
+                self._file_handler.log(
+                    agent=role, task=task.description, status="started"
+                )
+
             output = task.execute(context=task_output)
             if not task.async_execution:
                 task_output = output
 
             role = task.agent.role if task.agent is not None else "None"
             self._logger.log("debug", f"== [{role}] Task output: {task_output}\n\n")
 
+            if self.output_log_file:
+                self._file_handler.log(agent=role, task=task_output, status="completed")
+
         self._finish_execution(task_output)
         return self._format_output(task_output)
 
     def _run_hierarchical_process(self) -> str:
         """Creates and assigns a manager agent to make sure the crew completes the tasks."""
 
-        i18n = I18N(language=self.language)
-        manager = Agent(
-            role=i18n.retrieve("hierarchical_manager_agent", "role"),
-            goal=i18n.retrieve("hierarchical_manager_agent", "goal"),
-            backstory=i18n.retrieve("hierarchical_manager_agent", "backstory"),
-            tools=AgentTools(agents=self.agents).tools(),
-            llm=self.manager_llm,
-            verbose=True,
-        )
+        i18n = I18N(prompt_file=self.prompt_file)
+        try:
+            self.manager_agent.allow_delegation = (
+                True  # Forcing Allow delegation to the manager
+            )
+            manager = self.manager_agent
+        except:
+            manager = Agent(
+                role=i18n.retrieve("hierarchical_manager_agent", "role"),
+                goal=i18n.retrieve("hierarchical_manager_agent", "goal"),
+                backstory=i18n.retrieve("hierarchical_manager_agent", "backstory"),
+                tools=AgentTools(agents=self.agents).tools(),
+                llm=self.manager_llm,
+                verbose=True,
+            )
 
         task_output = ""
         for task in self.tasks:
             self._logger.log("debug", f"Working Agent: {manager.role}")
             self._logger.log("info", f"Starting Task: {task.description}")
 
+            if self.output_log_file:
+                self._file_handler.log(
+                    agent=manager.role, task=task.description, status="started"
+                )
+
             task_output = task.execute(
                 agent=manager, context=task_output, tools=manager.tools
             )
 
             self._logger.log("debug", f"[{manager.role}] Task output: {task_output}")
 
+            if self.output_log_file:
+                self._file_handler.log(
+                    agent=manager.role, task=task_output, status="completed"
+                )
+
         self._finish_execution(task_output)
         return self._format_output(task_output), manager._token_process.get_summary()
 
+    def _set_tasks_callbacks(self) -> str:
+        """Sets callback for every task suing task_callback"""
+        for task in self.tasks:
+            if not task.callback:
+                task.callback = self.task_callback
+
     def _interpolate_inputs(self, inputs: Dict[str, Any]) -> str:
         """Interpolates the inputs in the tasks and agents."""
         [task.interpolate_inputs(inputs) for task in self.tasks]
         [agent.interpolate_inputs(inputs) for agent in self.agents]
 
     def _format_output(self, output: str) -> str:
         """Formats the output of the crew execution."""
```

### Comparing `crewai_clean-0.22.5/src/crewai/project/annotations.py` & `crewai_clean-0.30.0rc5/src/crewai/project/annotations.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,32 @@
 tasks_order = []
 
 
+def memoize(func):
+    cache = {}
+
+    def memoized_func(*args, **kwargs):
+        key = (args, tuple(kwargs.items()))
+        if key not in cache:
+            cache[key] = func(*args, **kwargs)
+        return cache[key]
+
+    return memoized_func
+
+
 def task(func):
     func.is_task = True
     tasks_order.append(func.__name__)
+    func = memoize(func)
     return func
 
 
 def agent(func):
     func.is_agent = True
+    func = memoize(func)
     return func
 
 
 def crew(func):
     def wrapper(self, *args, **kwargs):
         instantiated_tasks = []
         instantiated_agents = []
```

### Comparing `crewai_clean-0.22.5/src/crewai/project/crew_base.py` & `crewai_clean-0.30.0rc5/src/crewai/project/crew_base.py`

 * *Files identical despite different names*

### Comparing `crewai_clean-0.22.5/src/crewai/task.py` & `crewai_clean-0.30.0rc5/src/crewai/task.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,33 +1,52 @@
+import re
 import threading
 import uuid
 from typing import Any, Dict, List, Optional, Type
+import os
 
 from langchain_openai import ChatOpenAI
 from pydantic import UUID4, BaseModel, Field, field_validator, model_validator
 from pydantic_core import PydanticCustomError
 
 from crewai.agent import Agent
 from crewai.tasks.task_output import TaskOutput
 from crewai.utilities import I18N, Converter, ConverterError, Printer
 from crewai.utilities.pydantic_schema_parser import PydanticSchemaParser
 
 
 class Task(BaseModel):
-    """Class that represent a task to be executed."""
+    """Class that represents a task to be executed.
+
+    Each task must have a description, an expected output and an agent responsible for execution.
+
+    Attributes:
+        agent: Agent responsible for task execution. Represents entity performing task.
+        async_execution: Boolean flag indicating asynchronous task execution.
+        callback: Function/object executed post task completion for additional actions.
+        config: Dictionary containing task-specific configuration parameters.
+        context: List of Task instances providing task context or input data.
+        description: Descriptive text detailing task's purpose and execution.
+        expected_output: Clear definition of expected task outcome.
+        output_file: File path for storing task output.
+        output_json: Pydantic model for structuring JSON output.
+        output_pydantic: Pydantic model for task output.
+        tools: List of tools/resources limited for task execution.
+    """
 
     class Config:
         arbitrary_types_allowed = True
 
     __hash__ = object.__hash__  # type: ignore
     used_tools: int = 0
     tools_errors: int = 0
     delegations: int = 0
     i18n: I18N = I18N()
     thread: threading.Thread = None
+    prompt_context: Optional[str] = None
     description: str = Field(description="Description of the actual task.")
     expected_output: str = Field(
         description="Clear definition of expected output for the task."
     )
     config: Optional[Dict[str, Any]] = Field(
         description="Configuration for the agent",
         default=None,
@@ -66,14 +85,18 @@
         description="Tools the agent is limited to use for this task.",
     )
     id: UUID4 = Field(
         default_factory=uuid.uuid4,
         frozen=True,
         description="Unique identifier for the object, not set by user.",
     )
+    human_input: Optional[bool] = Field(
+        description="Whether the task should have a human review the final answer of the agent",
+        default=False,
+    )
 
     _original_description: str | None = None
     _original_expected_output: str | None = None
 
     def __init__(__pydantic_self__, **data):
         config = data.pop("config", {})
         super().__init__(**config, **data)
@@ -136,14 +159,15 @@
             for task in self.context:
                 if task.async_execution:
                     task.thread.join()
                 if task and task.output:
                     context.append(task.output.raw_output)
             context = "\n".join(context)
 
+        self.prompt_context = context
         tools = tools or self.tools
 
         if self.async_execution:
             self.thread = threading.Thread(
                 target=self._execute, args=(agent, self, context, tools)
             )
             self.thread.start()
@@ -211,14 +235,33 @@
 
     def _export_output(self, result: str) -> Any:
         exported_result = result
         instructions = "I'm gonna convert this raw text into valid JSON."
 
         if self.output_pydantic or self.output_json:
             model = self.output_pydantic or self.output_json
+
+            # try to convert task_output directly to pydantic/json
+            try:
+                exported_result = model.model_validate_json(result)
+                if self.output_json:
+                    return exported_result.model_dump()
+                return exported_result
+            except Exception:
+              # sometimes the response contains valid JSON in the middle of text
+              match = re.search(r"({.*})", result, re.DOTALL)
+              if match:
+                  try:
+                      exported_result = model.model_validate_json(match.group(0))
+                      if self.output_json:
+                          return exported_result.model_dump()
+                      return exported_result
+                  except Exception:
+                      pass
+
             llm = self.agent.function_calling_llm or self.agent.llm
 
             if not self._is_gpt(llm):
                 model_schema = PydanticSchemaParser(model=model).get_schema()
                 instructions = f"{instructions}\n\nThe json should have the following structure, with the following keys:\n{model_schema}"
 
             converter = Converter(
@@ -245,13 +288,18 @@
 
         return exported_result
 
     def _is_gpt(self, llm) -> bool:
         return isinstance(llm, ChatOpenAI) and llm.openai_api_base == None
 
     def _save_file(self, result: Any) -> None:
+        directory = os.path.dirname(self.output_file)
+
+        if not os.path.exists(directory):
+            os.makedirs(directory)
+
         with open(self.output_file, "w") as file:
             file.write(result)
         return None
 
     def __repr__(self):
         return f"Task(description={self.description}, expected_output={self.expected_output})"
```

### Comparing `crewai_clean-0.22.5/src/crewai/tasks/task_output.py` & `crewai_clean-0.30.0rc5/src/crewai/tasks/task_output.py`

 * *Files identical despite different names*

### Comparing `crewai_clean-0.22.5/src/crewai/telemetry/telemetry.py` & `crewai_clean-0.30.0rc5/src/crewai/telemetry/telemetry.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import asyncio
 import json
 import os
 import platform
 from typing import Any
 
 import pkg_resources
 from opentelemetry import trace
@@ -35,36 +36,49 @@
 
     Users can opt-in to sharing more complete data suing the `share_crew`
     attribute in the Crew class.
     """
 
     def __init__(self):
         self.ready = False
+        self.trace_set = False
         try:
             if os.environ.get("CREWAI_TELEMETRY_OPT_OUT", False):
                 return
-            telemetry_endpoint = "http://telemetry.crewai.com:4318"
+            telemetry_endpoint = "https://telemetry.crewai.com:4319"
             self.resource = Resource(
                 attributes={SERVICE_NAME: "crewAI-telemetry"},
             )
             self.provider = TracerProvider(resource=self.resource)
+
             processor = BatchSpanProcessor(
-                OTLPSpanExporter(endpoint=f"{telemetry_endpoint}/v1/traces", timeout=15)
+                OTLPSpanExporter(
+                    endpoint=f"{telemetry_endpoint}/v1/traces",
+                    timeout=30,
+                )
             )
+
             self.provider.add_span_processor(processor)
             self.ready = True
-        except Exception:
-            pass
+        except BaseException as e:
+            if isinstance(
+                e,
+                (SystemExit, KeyboardInterrupt, GeneratorExit, asyncio.CancelledError),
+            ):
+                raise  # Re-raise the exception to not interfere with system signals
+            self.ready = False
 
     def set_tracer(self):
-        if self.ready:
+        if self.ready and not self.trace_set:
             try:
                 trace.set_tracer_provider(self.provider)
+                self.trace_set = True
             except Exception:
-                pass
+                self.ready = False
+                self.trace_set = False
 
     def crew_creation(self, crew):
         """Records the creation of a crew."""
         if self.ready:
             try:
                 tracer = trace.get_tracer("crewai.telemetry")
                 span = tracer.start_span("Crew Created")
@@ -72,48 +86,54 @@
                     span,
                     "crewai_version",
                     pkg_resources.get_distribution("crewai").version,
                 )
                 self._add_attribute(span, "python_version", platform.python_version())
                 self._add_attribute(span, "crew_id", str(crew.id))
                 self._add_attribute(span, "crew_process", crew.process)
-                self._add_attribute(span, "crew_language", crew.language)
+                self._add_attribute(
+                    span, "crew_language", crew.prompt_file if crew.i18n else "None"
+                )
+                self._add_attribute(span, "crew_memory", crew.memory)
                 self._add_attribute(span, "crew_number_of_tasks", len(crew.tasks))
                 self._add_attribute(span, "crew_number_of_agents", len(crew.agents))
                 self._add_attribute(
                     span,
                     "crew_agents",
                     json.dumps(
                         [
                             {
                                 "id": str(agent.id),
                                 "role": agent.role,
-                                "memory_enabled?": agent.memory,
                                 "verbose?": agent.verbose,
                                 "max_iter": agent.max_iter,
                                 "max_rpm": agent.max_rpm,
-                                "i18n": agent.i18n.language,
+                                "i18n": agent.i18n.prompt_file,
                                 "llm": json.dumps(self._safe_llm_attributes(agent.llm)),
                                 "delegation_enabled?": agent.allow_delegation,
-                                "tools_names": [tool.name for tool in agent.tools],
+                                "tools_names": [
+                                    tool.name.casefold() for tool in agent.tools
+                                ],
                             }
                             for agent in crew.agents
                         ]
                     ),
                 )
                 self._add_attribute(
                     span,
                     "crew_tasks",
                     json.dumps(
                         [
                             {
                                 "id": str(task.id),
                                 "async_execution?": task.async_execution,
                                 "agent_role": task.agent.role if task.agent else "None",
-                                "tools_names": [tool.name for tool in task.tools],
+                                "tools_names": [
+                                    tool.name.casefold() for tool in task.tools
+                                ],
                             }
                             for task in crew.tasks
                         ]
                     ),
                 )
                 self._add_attribute(span, "platform", platform.platform())
                 self._add_attribute(span, "platform_release", platform.release())
@@ -127,81 +147,105 @@
 
     def tool_repeated_usage(self, llm: Any, tool_name: str, attempts: int):
         """Records the repeated usage 'error' of a tool by an agent."""
         if self.ready:
             try:
                 tracer = trace.get_tracer("crewai.telemetry")
                 span = tracer.start_span("Tool Repeated Usage")
-                self._add_attribute(span, "tool_name", tool_name)
-                self._add_attribute(span, "attempts", attempts)
                 self._add_attribute(
-                    span, "llm", json.dumps(self._safe_llm_attributes(llm))
+                    span,
+                    "crewai_version",
+                    pkg_resources.get_distribution("crewai").version,
                 )
+                self._add_attribute(span, "tool_name", tool_name)
+                self._add_attribute(span, "attempts", attempts)
+                if llm:
+                    self._add_attribute(
+                        span, "llm", json.dumps(self._safe_llm_attributes(llm))
+                    )
                 span.set_status(Status(StatusCode.OK))
                 span.end()
             except Exception:
                 pass
 
     def tool_usage(self, llm: Any, tool_name: str, attempts: int):
         """Records the usage of a tool by an agent."""
         if self.ready:
             try:
                 tracer = trace.get_tracer("crewai.telemetry")
                 span = tracer.start_span("Tool Usage")
-                self._add_attribute(span, "tool_name", tool_name)
-                self._add_attribute(span, "attempts", attempts)
                 self._add_attribute(
-                    span, "llm", json.dumps(self._safe_llm_attributes(llm))
+                    span,
+                    "crewai_version",
+                    pkg_resources.get_distribution("crewai").version,
                 )
+                self._add_attribute(span, "tool_name", tool_name)
+                self._add_attribute(span, "attempts", attempts)
+                if llm:
+                    self._add_attribute(
+                        span, "llm", json.dumps(self._safe_llm_attributes(llm))
+                    )
                 span.set_status(Status(StatusCode.OK))
                 span.end()
             except Exception:
                 pass
 
     def tool_usage_error(self, llm: Any):
         """Records the usage of a tool by an agent."""
         if self.ready:
             try:
                 tracer = trace.get_tracer("crewai.telemetry")
                 span = tracer.start_span("Tool Usage Error")
                 self._add_attribute(
-                    span, "llm", json.dumps(self._safe_llm_attributes(llm))
+                    span,
+                    "crewai_version",
+                    pkg_resources.get_distribution("crewai").version,
                 )
+                if llm:
+                    self._add_attribute(
+                        span, "llm", json.dumps(self._safe_llm_attributes(llm))
+                    )
                 span.set_status(Status(StatusCode.OK))
                 span.end()
             except Exception:
                 pass
 
     def crew_execution_span(self, crew):
         """Records the complete execution of a crew.
         This is only collected if the user has opted-in to share the crew.
         """
         if (self.ready) and (crew.share_crew):
             try:
                 tracer = trace.get_tracer("crewai.telemetry")
                 span = tracer.start_span("Crew Execution")
+                self._add_attribute(
+                    span,
+                    "crewai_version",
+                    pkg_resources.get_distribution("crewai").version,
+                )
                 self._add_attribute(span, "crew_id", str(crew.id))
                 self._add_attribute(
                     span,
                     "crew_agents",
                     json.dumps(
                         [
                             {
                                 "id": str(agent.id),
                                 "role": agent.role,
                                 "goal": agent.goal,
                                 "backstory": agent.backstory,
-                                "memory_enabled?": agent.memory,
                                 "verbose?": agent.verbose,
                                 "max_iter": agent.max_iter,
                                 "max_rpm": agent.max_rpm,
-                                "i18n": agent.i18n.language,
+                                "i18n": agent.i18n.prompt_file,
                                 "llm": json.dumps(self._safe_llm_attributes(agent.llm)),
                                 "delegation_enabled?": agent.allow_delegation,
-                                "tools_names": [tool.name for tool in agent.tools],
+                                "tools_names": [
+                                    tool.name.casefold() for tool in agent.tools
+                                ],
                             }
                             for agent in crew.agents
                         ]
                     ),
                 )
                 self._add_attribute(
                     span,
@@ -213,27 +257,34 @@
                                 "description": task.description,
                                 "async_execution?": task.async_execution,
                                 "output": task.expected_output,
                                 "agent_role": task.agent.role if task.agent else "None",
                                 "context": [task.description for task in task.context]
                                 if task.context
                                 else "None",
-                                "tools_names": [tool.name for tool in task.tools],
+                                "tools_names": [
+                                    tool.name.casefold() for tool in task.tools
+                                ],
                             }
                             for task in crew.tasks
                         ]
                     ),
                 )
                 return span
             except Exception:
                 pass
 
     def end_crew(self, crew, output):
         if (self.ready) and (crew.share_crew):
             try:
+                self._add_attribute(
+                    crew._execution_span,
+                    "crewai_version",
+                    pkg_resources.get_distribution("crewai").version,
+                )
                 self._add_attribute(crew._execution_span, "crew_output", output)
                 self._add_attribute(
                     crew._execution_span,
                     "crew_tasks_output",
                     json.dumps(
                         [
                             {
@@ -255,10 +306,12 @@
         try:
             return span.set_attribute(key, value)
         except Exception:
             pass
 
     def _safe_llm_attributes(self, llm):
         attributes = ["name", "model_name", "base_url", "model", "top_k", "temperature"]
-        safe_attributes = {k: v for k, v in vars(llm).items() if k in attributes}
-        safe_attributes["class"] = llm.__class__.__name__
-        return safe_attributes
+        if llm:
+            safe_attributes = {k: v for k, v in vars(llm).items() if k in attributes}
+            safe_attributes["class"] = llm.__class__.__name__
+            return safe_attributes
+        return {}
```

### Comparing `crewai_clean-0.22.5/src/crewai/tools/agent_tools.py` & `crewai_clean-0.30.0rc5/src/crewai/tools/agent_tools.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,57 +11,62 @@
 class AgentTools(BaseModel):
     """Default tools around agent delegation"""
 
     agents: List[Agent] = Field(description="List of agents in this crew.")
     i18n: I18N = Field(default=I18N(), description="Internationalization settings.")
 
     def tools(self):
-        return [
+        tools = [
             StructuredTool.from_function(
                 func=self.delegate_work,
                 name="Delegate work to co-worker",
                 description=self.i18n.tools("delegate_work").format(
-                    coworkers=[f"{agent.role}" for agent in self.agents]
+                    coworkers=f"[{', '.join([f'{agent.role}' for agent in self.agents])}]"
                 ),
             ),
             StructuredTool.from_function(
                 func=self.ask_question,
                 name="Ask question to co-worker",
                 description=self.i18n.tools("ask_question").format(
-                    coworkers=[f"{agent.role}" for agent in self.agents]
+                    coworkers=f"[{', '.join([f'{agent.role}' for agent in self.agents])}]"
                 ),
             ),
         ]
+        return tools
 
     def delegate_work(self, coworker: str, task: str, context: str):
-        """Useful to delegate a specific task to a coworker passing all necessary context and names."""
+        """Useful to delegate a specific task to a co-worker passing all necessary context and names."""
         return self._execute(coworker, task, context)
 
     def ask_question(self, coworker: str, question: str, context: str):
-        """Useful to ask a question, opinion or take from a coworker passing all necessary context and names."""
+        """Useful to ask a question, opinion or take from a co-worker passing all necessary context and names."""
         return self._execute(coworker, question, context)
 
     def _execute(self, agent, task, context):
         """Execute the command."""
         try:
             agent = [
                 available_agent
                 for available_agent in self.agents
-                if available_agent.role.strip().lower() == agent.strip().lower()
+                if available_agent.role.casefold().strip() == agent.casefold().strip()
             ]
         except:
             return self.i18n.errors("agent_tool_unexsiting_coworker").format(
-                coworkers="\n".join([f"- {agent.role}" for agent in self.agents])
+                coworkers="\n".join(
+                    [f"- {agent.role.casefold()}" for agent in self.agents]
+                )
             )
 
         if not agent:
             return self.i18n.errors("agent_tool_unexsiting_coworker").format(
-                coworkers="\n".join([f"- {agent.role}" for agent in self.agents])
+                coworkers="\n".join(
+                    [f"- {agent.role.casefold()}" for agent in self.agents]
+                )
             )
 
         agent = agent[0]
         task = Task(
             description=task,
             agent=agent,
-            expected_output="Your best answer to your coworker asking you this, accounting for the context shared.",
+            expected_output="Your best answer to your co-worker asking you this, accounting for the context shared.",
         )
         return agent.execute_task(task, context)
```

### Comparing `crewai_clean-0.22.5/src/crewai/tools/cache_tools.py` & `crewai_clean-0.30.0rc5/src/crewai/tools/cache_tools.py`

 * *Files identical despite different names*

### Comparing `crewai_clean-0.22.5/src/crewai/tools/tool_calling.py` & `crewai_clean-0.30.0rc5/src/crewai/tools/tool_calling.py`

 * *Files identical despite different names*

### Comparing `crewai_clean-0.22.5/src/crewai/tools/tool_output_parser.py` & `crewai_clean-0.30.0rc5/src/crewai/tools/tool_output_parser.py`

 * *Files identical despite different names*

### Comparing `crewai_clean-0.22.5/src/crewai/tools/tool_usage.py` & `crewai_clean-0.30.0rc5/src/crewai/tools/tool_usage.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import ast
+from difflib import SequenceMatcher
 from textwrap import dedent
 from typing import Any, List, Union
 
 from langchain_core.tools import BaseTool
 from langchain_openai import ChatOpenAI
 
 from crewai.agents.tools_handler import ToolsHandler
@@ -22,26 +23,28 @@
 
 
 class ToolUsage:
     """
     Class that represents the usage of a tool by an agent.
 
     Attributes:
-        task: Task being executed.
-        tools_handler: Tools handler that will manage the tool usage.
-        tools: List of tools available for the agent.
-        tools_description: Description of the tools available for the agent.
-        tools_names: Names of the tools available for the agent.
-        function_calling_llm: Language model to be used for the tool usage.
+      task: Task being executed.
+      tools_handler: Tools handler that will manage the tool usage.
+      tools: List of tools available for the agent.
+      original_tools: Original tools available for the agent before being converted to BaseTool.
+      tools_description: Description of the tools available for the agent.
+      tools_names: Names of the tools available for the agent.
+      function_calling_llm: Language model to be used for the tool usage.
     """
 
     def __init__(
         self,
         tools_handler: ToolsHandler,
         tools: List[BaseTool],
+        original_tools: List[Any],
         tools_description: str,
         tools_names: str,
         task: Any,
         function_calling_llm: Any,
         action: Any,
     ) -> None:
         self._i18n: I18N = I18N()
@@ -49,14 +52,15 @@
         self._telemetry: Telemetry = Telemetry()
         self._run_attempts: int = 1
         self._max_parsing_attempts: int = 3
         self._remember_format_after_usages: int = 3
         self.tools_description = tools_description
         self.tools_names = tools_names
         self.tools_handler = tools_handler
+        self.original_tools = original_tools
         self.tools = tools
         self.task = task
         self.action = action
         self.function_calling_llm = function_calling_llm
 
         # Set the maximum parsing attempts for bigger models
         if (isinstance(self.function_calling_llm, ChatOpenAI)) and (
@@ -94,28 +98,31 @@
         calling: Union[ToolCalling, InstructorToolCalling],
     ) -> None:
         if self._check_tool_repeated_usage(calling=calling):
             try:
                 result = self._i18n.errors("task_repeated_usage").format(
                     tool_names=self.tools_names
                 )
-                self._printer.print(content=f"\n\n{result}\n", color="yellow")
+                self._printer.print(content=f"\n\n{result}\n", color="purple")
                 self._telemetry.tool_repeated_usage(
                     llm=self.function_calling_llm,
                     tool_name=tool.name,
                     attempts=self._run_attempts,
                 )
                 result = self._format_result(result=result)
                 return result
             except Exception:
                 self.task.increment_tools_errors()
 
-        result = self.tools_handler.cache.read(
-            tool=calling.tool_name, input=calling.arguments
-        )
+        result = None
+
+        if self.tools_handler.cache:
+            result = self.tools_handler.cache.read(
+                tool=calling.tool_name, input=calling.arguments
+            )
 
         if not result:
             try:
                 if calling.tool_name in [
                     "Delegate work to co-worker",
                     "Ask question to co-worker",
                 ]:
@@ -151,17 +158,32 @@
                     ).message
                     self.task.increment_tools_errors()
                     self._printer.print(content=f"\n\n{error_message}\n", color="red")
                     return error
                 self.task.increment_tools_errors()
                 return self.use(calling=calling, tool_string=tool_string)
 
-            self.tools_handler.on_tool_use(calling=calling, output=result)
+            if self.tools_handler:
+                should_cache = True
+                original_tool = next(
+                    (ot for ot in self.original_tools if ot.name == tool.name), None
+                )
+                if (
+                    hasattr(original_tool, "cache_function")
+                    and original_tool.cache_function
+                ):
+                    should_cache = original_tool.cache_function(
+                        calling.arguments, result
+                    )
 
-        self._printer.print(content=f"\n\n{result}\n", color="yellow")
+                self.tools_handler.on_tool_use(
+                    calling=calling, output=result, should_cache=should_cache
+                )
+
+        self._printer.print(content=f"\n\n{result}\n", color="purple")
         self._telemetry.tool_usage(
             llm=self.function_calling_llm,
             tool_name=tool.name,
             attempts=self._run_attempts,
         )
         result = self._format_result(result=result)
         return result
@@ -181,27 +203,35 @@
             tools=self.tools_description, tool_names=self.tools_names
         )
         return result
 
     def _check_tool_repeated_usage(
         self, calling: Union[ToolCalling, InstructorToolCalling]
     ) -> None:
+        if not self.tools_handler:
+            return False
         if last_tool_usage := self.tools_handler.last_used_tool:
             return (calling.tool_name == last_tool_usage.tool_name) and (
                 calling.arguments == last_tool_usage.arguments
             )
 
     def _select_tool(self, tool_name: str) -> BaseTool:
         for tool in self.tools:
-            if tool.name.lower().strip() == tool_name.lower().strip():
+            if (
+                tool.name.lower().strip() == tool_name.lower().strip()
+                or SequenceMatcher(
+                    None, tool.name.lower().strip(), tool_name.lower().strip()
+                ).ratio()
+                > 0.9
+            ):
                 return tool
         self.task.increment_tools_errors()
         if tool_name and tool_name != "":
             raise Exception(
-                f"Action '{tool_name}' don't exist, these are the only available Actions: {self.tools_description}"
+                f"Action '{tool_name}' don't exist, these are the only available Actions:\n {self.tools_description}"
             )
         else:
             raise Exception(
                 f"I forgot the Action name, these are the only available Actions: {self.tools_description}"
             )
 
     def _render(self) -> str:
@@ -233,37 +263,38 @@
             if self.function_calling_llm:
                 model = (
                     InstructorToolCalling
                     if self._is_gpt(self.function_calling_llm)
                     else ToolCalling
                 )
                 converter = Converter(
-                    text=f"Only tools available:\n###\n{self._render()}\n\nReturn a valid schema for the tool, the tool name must be exactly equal one of the options, use this text to inform the valid ouput schema:\n\n{tool_string}```",
+                    text=f"Only tools available:\n###\n{self._render()}\n\nReturn a valid schema for the tool, the tool name must be exactly equal one of the options, use this text to inform the valid output schema:\n\n{tool_string}```",
                     llm=self.function_calling_llm,
                     model=model,
                     instructions=dedent(
                         """\
-                                            The schema should have the following structure, only two keys:
-                                            - tool_name: str
-                                            - arguments: dict (with all arguments being passed)
+              The schema should have the following structure, only two keys:
+              - tool_name: str
+              - arguments: dict (with all arguments being passed)
 
-                                            Example:
-                                            {"tool_name": "tool name", "arguments": {"arg_name1": "value", "arg_name2": 2}}""",
+              Example:
+              {"tool_name": "tool name", "arguments": {"arg_name1": "value", "arg_name2": 2}}""",
                     ),
                     max_attemps=1,
                 )
                 calling = converter.to_pydantic()
 
                 if isinstance(calling, ConverterError):
                     raise calling
             else:
                 tool_name = self.action.tool
                 tool = self._select_tool(tool_name)
                 try:
-                    arguments = ast.literal_eval(self.action.tool_input)
+                    tool_input = self._validate_tool_input(self.action.tool_input)
+                    arguments = ast.literal_eval(tool_input)
                 except Exception:
                     return ToolUsageErrorException(
                         f'{self._i18n.errors("tool_arguments_error")}'
                     )
                 if not isinstance(arguments, dict):
                     return ToolUsageErrorException(
                         f'{self._i18n.errors("tool_arguments_error")}'
@@ -281,7 +312,58 @@
                 self._printer.print(content=f"\n\n{e}\n", color="red")
                 return ToolUsageErrorException(
                     f'{self._i18n.errors("tool_usage_error").format(error=e)}\nMoving on then. {self._i18n.slice("format").format(tool_names=self.tools_names)}'
                 )
             return self._tool_calling(tool_string)
 
         return calling
+
+    def _validate_tool_input(self, tool_input: str) -> str:
+        try:
+            ast.literal_eval(tool_input)
+            return tool_input
+        except Exception:
+            # Clean and ensure the string is properly enclosed in braces
+            tool_input = tool_input.strip()
+            if not tool_input.startswith("{"):
+                tool_input = "{" + tool_input
+            if not tool_input.endswith("}"):
+                tool_input += "}"
+
+            # Manually split the input into key-value pairs
+            entries = tool_input.strip("{} ").split(",")
+            formatted_entries = []
+
+            for entry in entries:
+                if ":" not in entry:
+                    continue  # Skip malformed entries
+                key, value = entry.split(":", 1)
+
+                # Remove extraneous white spaces and quotes, replace single quotes
+                key = key.strip().strip('"').replace("'", '"')
+                value = value.strip()
+
+                # Handle replacement of single quotes at the start and end of the value string
+                if value.startswith("'") and value.endswith("'"):
+                    value = value[1:-1]  # Remove single quotes
+                    value = (
+                        '"' + value.replace('"', '\\"') + '"'
+                    )  # Re-encapsulate with double quotes
+                elif value.isdigit():  # Check if value is a digit, hence integer
+                    formatted_value = value
+                elif value.lower() in [
+                    "true",
+                    "false",
+                    "null",
+                ]:  # Check for boolean and null values
+                    formatted_value = value.lower()
+                else:
+                    # Assume the value is a string and needs quotes
+                    formatted_value = '"' + value.replace('"', '\\"') + '"'
+
+                # Rebuild the entry with proper quoting
+                formatted_entry = f'"{key}": {formatted_value}'
+                formatted_entries.append(formatted_entry)
+
+            # Reconstruct the JSON string
+            new_json_string = "{" + ", ".join(formatted_entries) + "}"
+            return new_json_string
```

### Comparing `crewai_clean-0.22.5/src/crewai/translations/en.json` & `crewai_clean-0.30.0rc5/src/crewai/translations/en.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8786057692307692%*

 * *Differences: {"'errors'": "{delete: ['unexpected_format']}",*

 * * "'slices'": "{'task': '\\nCurrent Task: {input}\\n\\nBegin! This is VERY important to you, use "*

 * *             'the tools available and give your best Final Answer, your job depends on '*

 * *             "it!\\n\\nThought:', 'memory': '\\n\\n# Useful context: \\n{memory}', 'tools': "*

 * *             "'\\nYou ONLY have access to the following tools, and should NEVER make up tools that "*

 * *             'are not listed here:\\n\\n{tools}\\n\\nUse the following format:\\n\ […]*

```diff
@@ -2,33 +2,34 @@
     "errors": {
         "agent_tool_unexsiting_coworker": "\nError executing tool. Co-worker mentioned not found, it must to be one of the following options:\n{coworkers}\n",
         "force_final_answer": "Tool won't be use because it's time to give your final answer. Don't use tools and just your absolute BEST Final answer.",
         "task_repeated_usage": "I tried reusing the same input, I must stop using this action input. I'll try something else instead.\n\n",
         "tool_arguments_error": "Error: the Action Input is not a valid key, value dictionary.",
         "tool_usage_error": "I encountered an error: {error}",
         "tool_usage_exception": "I encountered an error while trying to use the tool. This was the error: {error}.\n Tool {tool} accepts these inputs: {tool_inputs}",
-        "unexpected_format": "\nSorry, I didn't use the expected format, I MUST either use a tool (use one at time) OR give my best final answer.\n",
         "wrong_tool_name": "You tried to use the tool {tool}, but it doesn't exist. You must use one of the following tools, use one at time: {tools}."
     },
     "hierarchical_manager_agent": {
         "backstory": "You are a seasoned manager with a knack for getting the best out of your team.\nYou are also known for your ability to delegate work to the right people, and to ask the right questions to get the best out of your team.\nEven though you don't perform tasks by yourself, you have a lot of experience in the field, which allows you to properly evaluate the work of your team members.",
         "goal": "Manage the team to complete the task in the best way possible.",
         "role": "Crew Manager"
     },
     "slices": {
         "expected_output": "\nThis is the expect criteria for your final answer: {expected_output} \n you MUST return the actual complete content as the final answer, not a summary.",
         "final_answer_format": "If you don't need to use any more tools, you must give your best complete final answer, make sure it satisfy the expect criteria, use the EXACT format below:\n\nThought: I now can give a great answer\nFinal Answer: my best complete final answer to the task.\n\n",
-        "format": "I MUST either use a tool (use one at time) OR give my best final answer. To Use the following format:\n\nThought: you should always think about what to do\nAction: the action to take, should be one of [{tool_names}]\nAction Input: the input to the action, dictionary\nObservation: the result of the action\n... (this Thought/Action/Action Input/Observation can repeat N times)\nThought: I now can give a great answer\nFinal Answer: my best complete final answer to the task.\nYour final answer must be the great and the most complete as possible, it must be outcome described\n\n ",
+        "format": "I MUST either use a tool (use one at time) OR give my best final answer. To Use the following format:\n\nThought: you should always think about what to do\nAction: the action to take, should be one of [{tool_names}]\nAction Input: the input to the action, dictionary enclosed in curly braces\nObservation: the result of the action\n... (this Thought/Action/Action Input/Observation can repeat N times)\nThought: I now can give a great answer\nFinal Answer: my best complete final answer to the task.\nYour final answer must be the great and the most complete as possible, it must be outcome described\n\n ",
         "format_without_tools": "\nSorry, I didn't use the right format. I MUST either use a tool (among the available ones), OR give my best final answer.\nI just remembered the expected format I must follow:\n\nQuestion: the input question you must answer\nThought: you should always think about what to do\nAction: the action to take, should be one of [{tool_names}]\nAction Input: the input to the action\nObservation: the result of the action\n... (this Thought/Action/Action Input/Observation can repeat N times)\nThought: I now can give a great answer\nFinal Answer: my best complete final answer to the task\nYour final answer must be the great and the most complete as possible, it must be outcome described\n\n",
-        "memory": "This is the summary of your work so far:\n{chat_history}",
-        "no_tools": "To give my best complete final answer to the task use the exact following format:\n\nThought: I now can give a great answer\nFinal Answer: my best complete final answer to the task.\nYour final answer must be the great and the most complete as possible, it must be outcome described.\n\nI MUST use these formats, my job depends on it!\n\nThought: ",
+        "getting_input": "This is the agent final answer: {final_answer}\nPlease provide a feedback: ",
+        "human_feedback": "You got human feedback on your work, re-avaluate it and give a new Final Answer when ready.\n {human_feedback}",
+        "memory": "\n\n# Useful context: \n{memory}",
+        "no_tools": "To give my best complete final answer to the task use the exact following format:\n\nThought: I now can give a great answer\nFinal Answer: my best complete final answer to the task.\nYour final answer must be the great and the most complete as possible, it must be outcome described.\n\nI MUST use these formats, my job depends on it!",
         "observation": "\nObservation",
         "role_playing": "You are {role}. {backstory}\nYour personal goal is: {goal}",
-        "task": "\n\nCurrent Task: {input}\n\nBegin! This is VERY important to you, use the tools available and give your best Final Answer, your job depends on it!\n\nThought: ",
+        "task": "\nCurrent Task: {input}\n\nBegin! This is VERY important to you, use the tools available and give your best Final Answer, your job depends on it!\n\nThought:",
         "task_with_context": "{task}\n\nThis is the context you're working with:\n{context}",
-        "tools": "\n\nYou ONLY have access to the following tools, and should NEVER make up tools that are not listed here:\n\n{tools}\n\nUse the following format:\n\nThought: you should always think about what to do\nAction: the action to take, only one name of [{tool_names}], just the name, exactly as it's written.\nAction Input: the input to the action, just a simple a python dictionary using \" to wrap keys and values.\nObservation: the result of the action\n\nOnce all necessary information is gathered:\n\nThought: I now know the final answer\nFinal Answer: the final answer to the original input question\n"
+        "tools": "\nYou ONLY have access to the following tools, and should NEVER make up tools that are not listed here:\n\n{tools}\n\nUse the following format:\n\nThought: you should always think about what to do\nAction: the action to take, only one name of [{tool_names}], just the name, exactly as it's written.\nAction Input: the input to the action, just a simple a python dictionary, enclosed in curly braces, using \" to wrap keys and values.\nObservation: the result of the action\n\nOnce all necessary information is gathered:\n\nThought: I now know the final answer\nFinal Answer: the final answer to the original input question\n"
     },
     "tools": {
-        "ask_question": "Ask a specific question to one of the following co-workers: {coworkers}\nThe input to this tool should be the coworker, the question you have for them, and ALL necessary context to ask the question properly, they know nothing about the question, so share absolute everything you know, don't reference things but instead explain them.",
-        "delegate_work": "Delegate a specific task to one of the following co-workers: {coworkers}\nThe input to this tool should be the coworker, the task you want them to do, and ALL necessary context to exectue the task, they know nothing about the task, so share absolute everything you know, don't reference things but instead explain them."
+        "ask_question": "Ask a specific question to one of the following co-workers: {coworkers}\nThe input to this tool should be the co-worker, the question you have for them, and ALL necessary context to ask the question properly, they know nothing about the question, so share absolute everything you know, don't reference things but instead explain them.",
+        "delegate_work": "Delegate a specific task to one of the following co-workers: {coworkers}\nThe input to this tool should be the co-worker, the task you want them to do, and ALL necessary context to exectue the task, they know nothing about the task, so share absolute everything you know, don't reference things but instead explain them."
     }
 }
```

### Comparing `crewai_clean-0.22.5/src/crewai/utilities/converter.py` & `crewai_clean-0.30.0rc5/src/crewai/utilities/converter.py`

 * *Files identical despite different names*

### Comparing `crewai_clean-0.22.5/src/crewai/utilities/crew_pydantic_output_parser.py` & `crewai_clean-0.30.0rc5/src/crewai/utilities/crew_pydantic_output_parser.py`

 * *Files identical despite different names*

### Comparing `crewai_clean-0.22.5/src/crewai/utilities/instructor.py` & `crewai_clean-0.30.0rc5/src/crewai/utilities/instructor.py`

 * *Files identical despite different names*

### Comparing `crewai_clean-0.22.5/src/crewai/utilities/logger.py` & `crewai_clean-0.30.0rc5/src/crewai/utilities/logger.py`

 * *Files identical despite different names*

### Comparing `crewai_clean-0.22.5/src/crewai/utilities/printer.py` & `crewai_clean-0.30.0rc5/src/crewai/utilities/printer.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 class Printer:
     def print(self, content: str, color: str):
-        if color == "yellow":
-            self._print_yellow(content)
+        if color == "purple":
+            self._print_purple(content)
         elif color == "red":
             self._print_red(content)
         elif color == "bold_green":
             self._print_bold_green(content)
-        elif color == "bold_yellow":
-            self._print_bold_yellow(content)
+        elif color == "bold_purple":
+            self._print_bold_purple(content)
         else:
             print(content)
 
-    def _print_bold_yellow(self, content):
-        print("\033[1m\033[93m {}\033[00m".format(content))
+    def _print_bold_purple(self, content):
+        print("\033[1m\033[95m {}\033[00m".format(content))
 
     def _print_bold_green(self, content):
         print("\033[1m\033[92m {}\033[00m".format(content))
 
-    def _print_yellow(self, content):
-        print("\033[93m {}\033[00m".format(content))
+    def _print_purple(self, content):
+        print("\033[95m {}\033[00m".format(content))
 
     def _print_red(self, content):
         print("\033[91m {}\033[00m".format(content))
```

### Comparing `crewai_clean-0.22.5/src/crewai/utilities/pydantic_schema_parser.py` & `crewai_clean-0.30.0rc5/src/crewai/utilities/pydantic_schema_parser.py`

 * *Files identical despite different names*

### Comparing `crewai_clean-0.22.5/src/crewai/utilities/rpm_controller.py` & `crewai_clean-0.30.0rc5/src/crewai/utilities/rpm_controller.py`

 * *Files identical despite different names*

### Comparing `crewai_clean-0.22.5/src/crewai/utilities/token_counter_callback.py` & `crewai_clean-0.30.0rc5/src/crewai/utilities/token_counter_callback.py`

 * *Files identical despite different names*

### Comparing `crewai_clean-0.22.5/PKG-INFO` & `crewai_clean-0.30.0rc5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 Metadata-Version: 2.1
 Name: crewai-clean
-Version: 0.22.5
+Version: 0.30.0rc5
 Summary: Cutting-edge framework for orchestrating role-playing, autonomous AI agents. By fostering collaborative intelligence, CrewAI empowers agents to work together seamlessly, tackling complex tasks.
 Author: Joao Moura
 Author-email: joao@crewai.com
 Requires-Python: >=3.10,<=3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: tools
+Requires-Dist: appdirs (>=1.4.4,<2.0.0)
 Requires-Dist: click (>=8.1.7,<9.0.0)
-Requires-Dist: crewai-tools (>=0.0.15,<0.0.16) ; extra == "tools"
+Requires-Dist: crewai-tools (>=0.2.3,<0.3.0) ; extra == "tools"
+Requires-Dist: embedchain (>=0.1.98,<0.2.0)
 Requires-Dist: instructor (>=0.5.2,<0.6.0)
 Requires-Dist: langchain (>=0.1.10,<0.2.0)
-Requires-Dist: langchain-openai (>=0.0.5,<0.0.6)
 Requires-Dist: openai (>=1.13.3,<2.0.0)
 Requires-Dist: opentelemetry-api (>=1.22.0,<2.0.0)
 Requires-Dist: opentelemetry-exporter-otlp-proto-http (>=1.22.0,<2.0.0)
 Requires-Dist: opentelemetry-sdk (>=1.22.0,<2.0.0)
 Requires-Dist: pydantic (>=2.4.2,<3.0.0)
-Requires-Dist: python-dotenv (==1.0.0)
+Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: regex (>=2023.12.25,<2024.0.0)
 Project-URL: Documentation, https://github.com/joaomdmoura/CrewAI/wiki/Index
 Project-URL: Homepage, https://crewai.com
 Project-URL: Repository, https://github.com/joaomdmoura/crewai
 Description-Content-Type: text/markdown
 
 <div align="center">
@@ -55,15 +56,14 @@
   - [Quick Tutorial](#quick-tutorial)
   - [Write Job Descriptions](#write-job-descriptions)
   - [Trip Planner](#trip-planner)
   - [Stock Analysis](#stock-analysis)
 - [Connecting Your Crew to a Model](#connecting-your-crew-to-a-model)
 - [How CrewAI Compares](#how-crewai-compares)
 - [Contribution](#contribution)
-- [Hire CrewAI](#hire-crewai)
 - [Telemetry](#telemetry)
 - [License](#license)
 
 ## Why CrewAI?
 
 The power of AI collaboration has too much to offer.
 CrewAI is designed to enable AI agents to assume roles, share goals, and operate in a cohesive unit - much like a well-oiled crew. Whether you're building a smart assistant platform, an automated customer service ensemble, or a multi-agent research team, CrewAI provides the backbone for sophisticated multi-agent interactions.
@@ -74,15 +74,15 @@
 
 ### 1. Installation
 
 ```shell
 pip install crewai
 ```
 
-If you want to also install crewai-tools, which is a package with tools that can be used by the agents, but more dependencies, you can install it with, example below uses it:
+If you want to install the 'crewai' package along with its optional features that include additional tools for agents, you can do so by using the following command: pip install 'crewai[tools]'. This command installs the basic package and also adds extra components which require more dependencies to function."
 
 ```shell
 pip install 'crewai[tools]'
 ```
 
 ### 2. Setting Up Your Crew
 
@@ -108,15 +108,15 @@
   goal='Uncover cutting-edge developments in AI and data science',
   backstory="""You work at a leading tech think tank.
   Your expertise lies in identifying emerging trends.
   You have a knack for dissecting complex data and presenting actionable insights.""",
   verbose=True,
   allow_delegation=False,
   tools=[search_tool]
-  # You can pass an optional llm attribute specifying what mode you wanna use.
+  # You can pass an optional llm attribute specifying what model you wanna use.
   # It can be a local model through Ollama / LM Studio or a remote
   # model like OpenAI, Mistral, Antrophic or others (https://docs.crewai.com/how-to/LLM-Connections/)
   #
   # import os
   # os.environ['OPENAI_MODEL_NAME'] = 'gpt-3.5-turbo'
   #
   # OR
@@ -272,26 +272,22 @@
 
 ### Installing Locally
 
 ```bash
 pip install dist/*.tar.gz
 ```
 
-## Hire CrewAI
-
-We're a company developing crewAI and crewAI Enterprise, we for a limited time are offer consulting with selected customers, to get them early access to our enterprise solution
-If you are interested on having access to it and hiring weekly hours with our team, feel free to email us at [joao@crewai.com](mailto:joao@crewai.com).
-
 ## Telemetry
 
 CrewAI uses anonymous telemetry to collect usage data with the main purpose of helping us improve the library by focusing our efforts on the most used features, integrations and tools.
 
 There is NO data being collected on the prompts, tasks descriptions agents backstories or goals nor tools usage, no API calls, nor responses nor any data that is being processed by the agents, nor any secrets and env vars.
 
 Data collected includes:
+
 - Version of crewAI
   - So we can understand how many users are using the latest version
 - Version of Python
   - So we can decide on what versions to better support
 - General OS (e.g. number of CPUs, macOS/Windows/Linux)
   - So we know what OS we should focus on and if we could build specific OS related features
 - Number of agents and tasks in a crew
```

