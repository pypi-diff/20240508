# Comparing `tmp/taskgen_ai-1.4.0.tar.gz` & `tmp/taskgen_ai-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskgen_ai-1.4.0.tar", last modified: Sun May  5 03:58:00 2024, max compression
+gzip compressed data, was "taskgen_ai-2.0.0.tar", last modified: Wed May  8 16:03:44 2024, max compression
```

## Comparing `taskgen_ai-1.4.0.tar` & `taskgen_ai-2.0.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 tanchongmin   (501) staff       (20)        0 2024-05-05 03:58:00.177910 taskgen_ai-1.4.0/
--rw-rw-r--   0 tanchongmin   (501) staff       (20)     1073 2024-02-26 00:45:10.000000 taskgen_ai-1.4.0/LICENSE
--rw-r--r--   0 tanchongmin   (501) staff       (20)    21112 2024-05-05 03:58:00.177183 taskgen_ai-1.4.0/PKG-INFO
--rw-rw-r--   0 tanchongmin   (501) staff       (20)    20503 2024-05-05 03:56:28.000000 taskgen_ai-1.4.0/README.md
--rw-rw-r--   0 tanchongmin   (501) staff       (20)      664 2024-05-05 03:55:46.000000 taskgen_ai-1.4.0/pyproject.toml
--rw-r--r--   0 tanchongmin   (501) staff       (20)       38 2024-05-05 03:58:00.178118 taskgen_ai-1.4.0/setup.cfg
--rw-rw-r--   0 tanchongmin   (501) staff       (20)      202 2024-05-05 03:56:40.000000 taskgen_ai-1.4.0/setup.py
-drwxr-xr-x   0 tanchongmin   (501) staff       (20)        0 2024-05-05 03:58:00.172915 taskgen_ai-1.4.0/taskgen/
--rw-rw-r--   0 tanchongmin   (501) staff       (20)      170 2024-03-14 09:43:26.000000 taskgen_ai-1.4.0/taskgen/__init__.py
--rw-r--r--   0 tanchongmin   (501) staff       (20)    33494 2024-05-05 03:45:48.000000 taskgen_ai-1.4.0/taskgen/agent.py
--rw-r--r--   0 tanchongmin   (501) staff       (20)    36833 2024-05-05 03:45:51.000000 taskgen_ai-1.4.0/taskgen/base.py
-drwxr-xr-x   0 tanchongmin   (501) staff       (20)        0 2024-05-05 03:58:00.176609 taskgen_ai-1.4.0/taskgen_ai.egg-info/
--rw-r--r--   0 tanchongmin   (501) staff       (20)    21112 2024-05-05 03:58:00.000000 taskgen_ai-1.4.0/taskgen_ai.egg-info/PKG-INFO
--rw-r--r--   0 tanchongmin   (501) staff       (20)      263 2024-05-05 03:58:00.000000 taskgen_ai-1.4.0/taskgen_ai.egg-info/SOURCES.txt
--rw-r--r--   0 tanchongmin   (501) staff       (20)        1 2024-05-05 03:58:00.000000 taskgen_ai-1.4.0/taskgen_ai.egg-info/dependency_links.txt
--rw-r--r--   0 tanchongmin   (501) staff       (20)       26 2024-05-05 03:58:00.000000 taskgen_ai-1.4.0/taskgen_ai.egg-info/requires.txt
--rw-r--r--   0 tanchongmin   (501) staff       (20)        8 2024-05-05 03:58:00.000000 taskgen_ai-1.4.0/taskgen_ai.egg-info/top_level.txt
+drwxr-xr-x   0 tanchongmin   (501) staff       (20)        0 2024-05-08 16:03:44.659650 taskgen_ai-2.0.0/
+-rw-rw-r--   0 tanchongmin   (501) staff       (20)     1073 2024-02-26 00:45:10.000000 taskgen_ai-2.0.0/LICENSE
+-rw-r--r--   0 tanchongmin   (501) staff       (20)    21462 2024-05-08 16:03:44.659149 taskgen_ai-2.0.0/PKG-INFO
+-rw-rw-r--   0 tanchongmin   (501) staff       (20)    20853 2024-05-08 15:52:00.000000 taskgen_ai-2.0.0/README.md
+-rw-rw-r--   0 tanchongmin   (501) staff       (20)      664 2024-05-08 16:02:47.000000 taskgen_ai-2.0.0/pyproject.toml
+-rw-r--r--   0 tanchongmin   (501) staff       (20)       38 2024-05-08 16:03:44.659757 taskgen_ai-2.0.0/setup.cfg
+-rw-rw-r--   0 tanchongmin   (501) staff       (20)      202 2024-05-08 15:52:13.000000 taskgen_ai-2.0.0/setup.py
+drwxr-xr-x   0 tanchongmin   (501) staff       (20)        0 2024-05-08 16:03:44.656329 taskgen_ai-2.0.0/taskgen/
+-rw-rw-r--   0 tanchongmin   (501) staff       (20)      213 2024-05-08 15:44:50.000000 taskgen_ai-2.0.0/taskgen/__init__.py
+-rw-r--r--   0 tanchongmin   (501) staff       (20)    32568 2024-05-08 15:59:25.000000 taskgen_ai-2.0.0/taskgen/agent.py
+-rw-r--r--   0 tanchongmin   (501) staff       (20)    48876 2024-05-08 15:40:35.000000 taskgen_ai-2.0.0/taskgen/base.py
+drwxr-xr-x   0 tanchongmin   (501) staff       (20)        0 2024-05-08 16:03:44.658577 taskgen_ai-2.0.0/taskgen_ai.egg-info/
+-rw-r--r--   0 tanchongmin   (501) staff       (20)    21462 2024-05-08 16:03:44.000000 taskgen_ai-2.0.0/taskgen_ai.egg-info/PKG-INFO
+-rw-r--r--   0 tanchongmin   (501) staff       (20)      263 2024-05-08 16:03:44.000000 taskgen_ai-2.0.0/taskgen_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 tanchongmin   (501) staff       (20)        1 2024-05-08 16:03:44.000000 taskgen_ai-2.0.0/taskgen_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 tanchongmin   (501) staff       (20)       26 2024-05-08 16:03:44.000000 taskgen_ai-2.0.0/taskgen_ai.egg-info/requires.txt
+-rw-r--r--   0 tanchongmin   (501) staff       (20)        8 2024-05-08 16:03:44.000000 taskgen_ai-2.0.0/taskgen_ai.egg-info/top_level.txt
```

### Comparing `taskgen_ai-1.4.0/LICENSE` & `taskgen_ai-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `taskgen_ai-1.4.0/PKG-INFO` & `taskgen_ai-2.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,8 @@
-Metadata-Version: 2.1
-Name: taskgen-ai
-Version: 1.4.0
-Summary: A Task-based agentic framework building on StrictJSON outputs by LLM agents
-Author-email: John Tan Chong Min <tanchongmin@gmail.com>
-Project-URL: Homepage, https://github.com/simbianai/taskgen
-Project-URL: Issues, https://github.com/simbianai/taskgen/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: openai>=1.3.6
-Requires-Dist: dill>=0.3.7
-
-# TaskGen v1.4.0
+# TaskGen v2.0.0
 ### A Task-based agentic framework building on StrictJSON outputs by LLM agents
 - Related Repositories: StrictJSON (https://github.com/tanchongmin/strictjson)
 - Video (Part 1): https://www.youtube.com/watch?v=O_XyTT7QGH4
 - Video (Part 2): https://www.youtube.com/watch?v=OWk7moRfTPE
 
 ### Creator's Preamble
 Happy to share that the task-based agentic framework I have been working on - TaskGen - is largely complete! 
@@ -55,14 +39,19 @@
 - Discussion Channel (my discord - John's AI Group): [https://discord.gg/bzp87AHJy5](https://discord.gg/bzp87AHJy5)
 
 ## How do I use this? 
 1. Download package via command line ```pip install taskgen-ai```
 2. Set up your OpenAPI API Key
 3. Import the required functions from ```taskgen``` and use them!
 
+## Differences in LLM for Agentic Framework
+- ChatGPT (gpt-3.5-turbo) is consistent only if you specify very clearly what you want the Agent to do and give examples of what you want
+- gpt-4-turbo and more advanced models can perform better zero-shot without much examples
+- TaskGen is compatible with ChatGPT and similar models, but for more robust use, consider using gpt-4-turbo and better models
+
 # Agent Basics - See Tutorial 1
 - Create an agent by entering your agent's name and description
 - Agents are task-based, so they will help generate subtasks to fulfil your main task
 - Agents are made to be non-verbose, so they will just focus only on task instruction (Much more efficient compared to conversational-based agentic frameworks like AutoGen)
     
 ## Example Agent Creation
 ```python
@@ -255,26 +244,26 @@
 # Define your meta-agent
 my_agent = Agent('Menu Creator', 
                  'Creates a menu for a restaurant. Menu item includes Name, Description, Ingredients, Pricing.')
 
 # Define your agent list. Note you can just assign functions to the agent in place using .assign_functions(function_list)
 agent_list = [
     Agent('Chef', 'Takes in dish names and comes up with ingredients for each of them. Does not generate prices.'),
-    Agent('Boss', 'Takes in menu items and curates them according to price'),
+    Agent('Boss', ''Does final quality check on menu items'),
     Agent('Creative Writer', 'Takes in a cuisine type and generates interesting dish names and descriptions. Does not generate prices or ingredients.', max_subtasks = 2),
     Agent('Economist', 'Takes in dish names and comes up with fictitious pricing for each of them')
     ]
 
 my_agent.assign_agents(agent_list)
 ```
 
 ## Run the Meta Agent
 - Let us run the agent and see the interactions between the Meta Agent and Inner Agents to solve the task!
 ```python
-output = my_agent.run('Give me 5 menu items with name, description, ingredients and price based on Italian food choices.')
+output = my_agent.run('Give me 5 menu items with name, description, ingredients and price based on Italian food choices. Ensure all parts of menu are generated.')
 ```
 
 # Shared Variables - See Tutorial 3
 
 *"Because text is not enough"* - Anonymous
 
 - `shared_variables` is a dictionary, that is initialised in Agent (default empty dictionary), and can be referenced by any function of the agent (including Inner Agents and their functions)
@@ -310,20 +299,20 @@
 
 ## Example External Function Accessing Shared Variables (Advanced)
 ```python
 # Use shared_variables as input to your external function to access and modify the shared variables
 def generate_quotes(shared_variables, number_of_quotes: int, category: str):
     ''' Generates number_of_quotes quotes about category '''
     # Retrieve from shared variables
-    my_quote_list = shared_variables['s_quote_list']
+    my_quote_list = shared_variables['quote_list']
     
     ### Add your function code here ###
     
     # Store back to shared variables
-    shared_variables['s_quote_list'] = my_quote_list
+    shared_variables['quote_list'] = my_quote_list
 
 generate_quote_fn = Function(output_format = {}, external_fn = generate_quotes)
 ```
 
 # Memory - See Tutorial 4
 
 ## Key Philosophy
@@ -370,17 +359,18 @@
 <br></br>
 - Implementing your own specific instructions to the default planner prompt
     - Implement your own memory-based RAG / global prompt instruction if you need more than what the default prompt can achieve
 <br></br>
 - Avoid Multiple Similar Subtasks in `subtasks_history`
     - If you have multiple similar subtask names, then it is likely the Agent can be confused and think it has already done the subtask
     - In this case, you can disambiguate by resetting the agent and store the persistent information in `shared_variables` and provide it to the agent using `get_global_context`
+    - Has the benefit of shifting the Start State closer to End State desired by resetting the Agent's planning cycle
 
 # Known Limitations
-1. As the agent uses the term "Overall Plan" for its internal planning, try not to use the word "plan" in your query or context, if not it might confuse the agent. Use alternative words like "schedule"
+- To be added
 
 # Contributing to the project
 
 ## Test locally
 1. Clone the repository
 2. If using a virtual environment, activate it
 3. `cd` into taskgen repository
```

### Comparing `taskgen_ai-1.4.0/README.md` & `taskgen_ai-2.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,24 @@
-# TaskGen v1.4.0
+Metadata-Version: 2.1
+Name: taskgen-ai
+Version: 2.0.0
+Summary: A Task-based agentic framework building on StrictJSON outputs by LLM agents
+Author-email: John Tan Chong Min <tanchongmin@gmail.com>
+Project-URL: Homepage, https://github.com/simbianai/taskgen
+Project-URL: Issues, https://github.com/simbianai/taskgen/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: openai>=1.3.6
+Requires-Dist: dill>=0.3.7
+
+# TaskGen v2.0.0
 ### A Task-based agentic framework building on StrictJSON outputs by LLM agents
 - Related Repositories: StrictJSON (https://github.com/tanchongmin/strictjson)
 - Video (Part 1): https://www.youtube.com/watch?v=O_XyTT7QGH4
 - Video (Part 2): https://www.youtube.com/watch?v=OWk7moRfTPE
 
 ### Creator's Preamble
 Happy to share that the task-based agentic framework I have been working on - TaskGen - is largely complete! 
@@ -39,14 +55,19 @@
 - Discussion Channel (my discord - John's AI Group): [https://discord.gg/bzp87AHJy5](https://discord.gg/bzp87AHJy5)
 
 ## How do I use this? 
 1. Download package via command line ```pip install taskgen-ai```
 2. Set up your OpenAPI API Key
 3. Import the required functions from ```taskgen``` and use them!
 
+## Differences in LLM for Agentic Framework
+- ChatGPT (gpt-3.5-turbo) is consistent only if you specify very clearly what you want the Agent to do and give examples of what you want
+- gpt-4-turbo and more advanced models can perform better zero-shot without much examples
+- TaskGen is compatible with ChatGPT and similar models, but for more robust use, consider using gpt-4-turbo and better models
+
 # Agent Basics - See Tutorial 1
 - Create an agent by entering your agent's name and description
 - Agents are task-based, so they will help generate subtasks to fulfil your main task
 - Agents are made to be non-verbose, so they will just focus only on task instruction (Much more efficient compared to conversational-based agentic frameworks like AutoGen)
     
 ## Example Agent Creation
 ```python
@@ -239,26 +260,26 @@
 # Define your meta-agent
 my_agent = Agent('Menu Creator', 
                  'Creates a menu for a restaurant. Menu item includes Name, Description, Ingredients, Pricing.')
 
 # Define your agent list. Note you can just assign functions to the agent in place using .assign_functions(function_list)
 agent_list = [
     Agent('Chef', 'Takes in dish names and comes up with ingredients for each of them. Does not generate prices.'),
-    Agent('Boss', 'Takes in menu items and curates them according to price'),
+    Agent('Boss', ''Does final quality check on menu items'),
     Agent('Creative Writer', 'Takes in a cuisine type and generates interesting dish names and descriptions. Does not generate prices or ingredients.', max_subtasks = 2),
     Agent('Economist', 'Takes in dish names and comes up with fictitious pricing for each of them')
     ]
 
 my_agent.assign_agents(agent_list)
 ```
 
 ## Run the Meta Agent
 - Let us run the agent and see the interactions between the Meta Agent and Inner Agents to solve the task!
 ```python
-output = my_agent.run('Give me 5 menu items with name, description, ingredients and price based on Italian food choices.')
+output = my_agent.run('Give me 5 menu items with name, description, ingredients and price based on Italian food choices. Ensure all parts of menu are generated.')
 ```
 
 # Shared Variables - See Tutorial 3
 
 *"Because text is not enough"* - Anonymous
 
 - `shared_variables` is a dictionary, that is initialised in Agent (default empty dictionary), and can be referenced by any function of the agent (including Inner Agents and their functions)
@@ -294,20 +315,20 @@
 
 ## Example External Function Accessing Shared Variables (Advanced)
 ```python
 # Use shared_variables as input to your external function to access and modify the shared variables
 def generate_quotes(shared_variables, number_of_quotes: int, category: str):
     ''' Generates number_of_quotes quotes about category '''
     # Retrieve from shared variables
-    my_quote_list = shared_variables['s_quote_list']
+    my_quote_list = shared_variables['quote_list']
     
     ### Add your function code here ###
     
     # Store back to shared variables
-    shared_variables['s_quote_list'] = my_quote_list
+    shared_variables['quote_list'] = my_quote_list
 
 generate_quote_fn = Function(output_format = {}, external_fn = generate_quotes)
 ```
 
 # Memory - See Tutorial 4
 
 ## Key Philosophy
@@ -354,17 +375,18 @@
 <br></br>
 - Implementing your own specific instructions to the default planner prompt
     - Implement your own memory-based RAG / global prompt instruction if you need more than what the default prompt can achieve
 <br></br>
 - Avoid Multiple Similar Subtasks in `subtasks_history`
     - If you have multiple similar subtask names, then it is likely the Agent can be confused and think it has already done the subtask
     - In this case, you can disambiguate by resetting the agent and store the persistent information in `shared_variables` and provide it to the agent using `get_global_context`
+    - Has the benefit of shifting the Start State closer to End State desired by resetting the Agent's planning cycle
 
 # Known Limitations
-1. As the agent uses the term "Overall Plan" for its internal planning, try not to use the word "plan" in your query or context, if not it might confuse the agent. Use alternative words like "schedule"
+- To be added
 
 # Contributing to the project
 
 ## Test locally
 1. Clone the repository
 2. If using a virtual environment, activate it
 3. `cd` into taskgen repository
```

### Comparing `taskgen_ai-1.4.0/pyproject.toml` & `taskgen_ai-2.0.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "taskgen-ai"
-version = "1.4.0"
+version = "2.0.0"
 authors = [
   { name="John Tan Chong Min", email="tanchongmin@gmail.com" },
 ]
 description = "A Task-based agentic framework building on StrictJSON outputs by LLM agents"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `taskgen_ai-1.4.0/taskgen/agent.py` & `taskgen_ai-2.0.0/taskgen/agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -259,15 +259,15 @@
             for name, function in self.function_map.items():
                 if function.is_compulsory:
                     filtered_fn_list.append(function)
                 
         # add in global context to the prompt
         global_context = ''
         if self.get_global_context is not None:
-            global_context = 'Global Context:' + self.get_global_context(self) + '\n'
+            global_context = 'Global Context:\n```\n' + self.get_global_context(self) + '\n```\n'
         
         system_prompt = f"You are an agent named {self.agent_name} with the following description: ```{self.agent_description}```\n"
         if provide_function_list:
             system_prompt += f"You have the following Equipped Functions available:\n```{self.list_functions(filtered_fn_list)}```\n"
         system_prompt += global_context
         system_prompt += query
         
@@ -376,15 +376,15 @@
             for name in self.memory_bank.keys():
                 # Function is done separately
                 if name == 'Function': continue
                 # Do not need to add to context if the memory item is empty
                 if self.memory_bank[name].isempty(): continue
                 rag_info += f'Related {name}: ```{self.memory_bank[name].retrieve(subtask)}```\n'
 
-            res = self.query(query = f'{rag_info}Overall Task:```{self.overall_task}```\nContext:```{self.subtasks_completed}```\nAssigned Subtask: ```{function_params["instruction"]}```\nPerform the Assigned Subtask only - do not just state what has or can be done - actually generate the outcome of Assigned Subtask fully but only within your Agent Capabilities', 
+            res = self.query(query = f'{rag_info}Context:```{self.overall_task}\n{self.subtasks_completed}```\nAssigned Subtask: ```{function_params["instruction"]}```\nGenerate a response for Assigned Subtask only - do not just state what has or can be done or apologise or repeat Assigned Subtask - actually generate the outcome of Assigned Subtask fully according to your Agent Capabilities.', 
                             output_format = {"Output": "Generate a full response to the Assigned Subtask"},
                             provide_function_list = False)
             
             res = res["Output"]
             
             if self.verbose: 
                 print('>', res)
@@ -412,55 +412,54 @@
                 res = {'Status': 'Completed'}
             
             self.add_subtask_result(subtask, res)
 
         return res
    
     def get_next_subtask(self, task = ''):
-        ''' Based on what the task is and the subtasks completed, we get the next subtask, function and input parameters'''
+        ''' Based on what the task is and the subtasks completed, we get the next subtask, function and input parameters. Supports user-given task as well if user wants to use this function directly'''
         
         if task == '':
-                background_info = f"Assigned Task:```{self.task}```\nAssigned Plan: ```{self.overall_plan}```\nPast Subtasks Completed: ```{self.subtasks_completed}```\n"
+                background_info = f"Assigned Task:```{self.task}```\nSubtasks Completed: ```{self.subtasks_completed}```\n"
         else:
             background_info = f"Assigned Task:```{task}```\n"
                 
-        # only add overall plan if there is and not evaluating for single task
-        if task == '':
-            task = ', '.join(self.overall_plan) if self.overall_plan is not None else task
+        # use default agent plan if task is not given
         task = self.task if task == '' else task
             
         # Add in memory to the Agent
         rag_info = ''
         for name in self.memory_bank.keys():
             # Function RAG is done separately in self.query()
             if name == 'Function': continue
             # Do not need to add to context if the memory item is empty
             if self.memory_bank[name].isempty(): continue
             else:
                 rag_info += f'Related {name}: ```{self.memory_bank[name].retrieve(task)}```\n'
                 
         # First select the Equipped Function
-        res = self.query(query = f'''{background_info}{rag_info}First create an Overall Plan modified from Assigned Plan with an array of steps to do Assigned Task from beginning to end, including uncompleted steps. Then, reflect on Past Subtasks Completed (note not all past subtasks are relevant to Assigned Task) to see what steps in Overall Plan are already completed. Then, generate Overall Plan Completed that outputs True for array elements of Overall Plan that are complete and False otherwise. Then, generate the Next Step to fulfil the Assigned Task that can be performed by a single Equipped Function. If Assigned Task is completed, output end_task for Equipped Function''',
-                         output_format = {"Thoughts": "How to do Assigned Task", "Overall Plan": "Array of steps to complete Assigned Task from beginning to end, type: list", "Reflection": "What has been done and what is still left to do", "Overall Plan Completed": "Whether array elements in Overall Plan are already completed, type: List[bool]", "Next Step": "First non-completed element in Overall Plan", "Equipped Function": f"Name of Equipped Function to use for Next Step, type: Enum{list(self.function_map.keys())}", "Instruction": "Instruction for the Equipped Function if any"},
+        res = self.query(query = f'''{background_info}{rag_info}\nBased on Context and Subtasks Completed, provide the Current Subtask and Equipped Function to complete part of Assigned Task. If Assigned Task is completed, Current Subtask is End Task and Equipped Function is end_task''',
+                         output_format = {"Thoughts": "How to complete Assigned Task, End Task if completed", "Observation": "Reflect on what has been done so far for Assigned Task", "Current Subtask": "What to do now in detail, End Task if completed", "Equipped Function": "Name of Equipped Function to use for Current Subtask, end_task if completed"},
                          provide_function_list = True,
                          task = task)
         
         # end task if equipped function is incorrect
         if res["Equipped Function"] not in self.function_map:
             res["Equipped Function"] = "end_task"
                 
         # If equipped function is use_llm, or end_task, we don't need to do another query
         cur_function = self.function_map[res["Equipped Function"]]
+        
         if res["Equipped Function"] == 'use_llm':
-            res['Equipped Function Input'] = {'instruction': res['Next Step']}
+            res['Equipped Function Inputs'] = {'instruction': res['Current Subtask']}
         elif res['Equipped Function'] == 'end_task':
-            res['Equipped Function Input'] = {}
+            res['Equipped Function Inputs'] = {}
         # Otherwise, if it is only the instruction, no type check needed, so just take the instruction
         elif len(cur_function.variable_names) == 1 and cur_function.variable_names[0].lower() == "instruction":
-            res['Equipped Function Input'] = {'instruction': res['Instruction']}
+            res['Equipped Function Inputs'] = {'instruction': res['Current Subtask']}
             
         # Otherwise, do another query to get type-checked input parameters and ensure all input fields are present
         else:
             input_format = {}
             fn_description = cur_function.fn_description
             matches = re.findall(r'<(.*?)>', fn_description)
             
@@ -470,36 +469,23 @@
                     first_part, second_part = match.split(':', 1)
                     input_format[first_part] = f'A suitable value, type: {second_part}'
                 else:
                     input_format[match] = 'A suitable value'
                     
             # if there is no input, then do not need LLM to extract out function's input
             if input_format == {}:
-                res["Equipped Function Input"] = {}
+                res["Equipped Function Inputs"] = {}
                     
             else:    
-                res2 = self.query(query = f'''{background_info}{rag_info}Current Subtask: {res["Next Step"]}\nEquipped Function Name: {res["Equipped Function"]}\nEquipped Function Details: {str(cur_function)}\nOutput suitable values for the input parameters of the Equipped Function to fulfil Current Subtask''',
+                res2 = self.query(query = f'''{background_info}{rag_info}\nCurrent Subtask: {res["Current Subtask"]}\nEquipped Function Details: {str(cur_function)}\nOutput suitable values for the input parameters of the Equipped Function to fulfil Current Subtask''',
                              output_format = input_format,
                              provide_function_list = False)
-                res["Equipped Function Input"] = res2
-
-        ## End Task Overrides
-        # if the next step is already done before, then end the task. Unless it is in OS mode, then allow it
-        if res["Next Step"] in self.subtasks_completed and self.default_to_llm is True:
-            res["Equipped Function"] = "end_task"
-
-        # if whole plan is completed, end task
-        if False not in res['Overall Plan Completed']:
-            res['Equipped Function'] = 'end_task'
-
-        # save overall plan
-        if len(res['Overall Plan']) > 0:
-            self.overall_plan = res['Overall Plan']
+                res["Equipped Function Inputs"] = res2
             
-        return res["Next Step"], res["Equipped Function"], res["Equipped Function Input"]
+        return res["Current Subtask"], res["Equipped Function"], res["Equipped Function Inputs"]
         
     def add_subtask_result(self, subtask, result):
         ''' Adds the subtask and result to subtasks_completed
         Keep adding (num) to subtask str if there is duplicate '''
         subtask_str = str(subtask)
         count = 2
         
@@ -526,16 +512,16 @@
         
     def reply_user(self, query: str = '', stateful: bool = True):
         ''' Generate a reply to the user based on the query / agent task and subtasks completed
         If stateful, also store this interaction into the subtasks_completed'''
         
         my_query = self.task if query == '' else query
             
-        res = self.query(query = f'Context: ```{self.subtasks_completed}```\nAssigned Task: ```{my_query}```\nGenerate a response to the Assigned Task using the Context only', 
-                                    output_format = {"Response to Assigned Task": "Use the Context as ground truth to respond to as many parts of the Assigned Task as possible. Do not respond with any information not from Context."},
+        res = self.query(query = f'Subtasks Completed: ```{self.subtasks_completed}```\nAssigned Task: ```{my_query}```\nRespond to the Assigned Task in detail using information from Subtasks Completed only. Do not generate anything new.', 
+                                    output_format = {"Response to Assigned Task": "Detailed Response"},
                                     provide_function_list = False)
         
         res = res["Response to Assigned Task"]
         
         if self.verbose:
             print(res)
         
@@ -547,14 +533,19 @@
     def run(self, task: str = '', overall_task: str = '', num_subtasks: int = 0) -> list:
         ''' Attempts to do the task using LLM and available functions
         Loops through and performs either a function call or LLM call up to num_subtasks number of times
         If overall_task is filled, then we store it to pass to the inner agents for more context '''
             
         # Assign the task
         if task != '':
+            ### TODO: Add in Planner here to split the task into steps if sequential generation is required
+            ### Planner can also infuse diverse views if the task is more creative
+            ### Planner can also be rule-based like MCTS if it is an explore-exploit RL-style problem
+            ### Planner can also be rule-based shortest path algo if it is a navigation problem
+            
             self.task_completed = False
             # If meta agent's task is here as well, assign it too
             if overall_task != '':
                 self.assign_task(task, overall_task)
             else:
                 self.assign_task(task)
```

### Comparing `taskgen_ai-1.4.0/taskgen/base.py` & `taskgen_ai-2.0.0/taskgen/base.py`

 * *Files 18% similar despite different names*

```diff
@@ -363,14 +363,66 @@
     if verbose:
         print('System prompt:', system_prompt)
         print('\nUser prompt:', user_prompt)
         print('\nGPT response:', res)
             
     return res
 
+
+async def chat_async(system_prompt: str, user_prompt: str, model: str = 'gpt-3.5-turbo', temperature: float = 0, verbose: bool = False, host: str = 'openai', llm_async = None, **kwargs):
+    '''Performs a chat with the host's LLM model with system prompt, user prompt, model, verbose and kwargs
+    Returns the output string res
+    - system_prompt: String. Write in whatever you want the LLM to become. e.g. "You are a \<purpose in life\>"
+    - user_prompt: String. The user input. Later, when we use it as a function, this is the function input
+    - model: String. The LLM model to use for json generation
+    - verbose: Boolean (default: False). Whether or not to print out the system prompt, user prompt, GPT response
+    - host: String. The provider of the LLM
+    - llm: User-made llm function.
+        - Inputs:
+            - system_prompt: String. Write in whatever you want the LLM to become. e.g. "You are a \<purpose in life\>"
+            - user_prompt: String. The user input. Later, when we use it as a function, this is the function input
+        - Output:
+            - res: String. The response of the LLM call
+    - **kwargs: Dict. Additional arguments for LLM chat
+    
+    TODO: Incorporate other open-sourced LLMs in the future'''
+    if llm_async is not None:
+        ''' If you specified your own LLM, then we just feed in the system and user prompt 
+        LLM function should take in system prompt (str) and user prompt (str), and output a response (str) '''
+        res = await llm_async(system_prompt = system_prompt, user_prompt = user_prompt)
+    
+    ## This part here is for llms that are OpenAI based
+    elif host == 'openai':
+        # additional checks for openai json mode
+        if 'response_format' in kwargs and kwargs['response_format'] == {"type": "json_object"}:
+            # if model fails, default to gpt-3.5-turbo-1106
+            try:
+                assert(model in ['gpt-4-1106-preview', 'gpt-3.5-turbo-1106'])
+            except Exception as e:
+                model = 'gpt-3.5-turbo-1106'
+                
+        client = OpenAI()
+        response = client.chat.completions.create(
+            model=model,
+            temperature = temperature,
+            messages=[
+                {"role": "system", "content": system_prompt},
+                {"role": "user", "content": user_prompt}
+            ],
+            **kwargs
+        )
+        res = response.choices[0].message.content
+
+    if verbose:
+        print('System prompt:', system_prompt)
+        print('\nUser prompt:', user_prompt)
+        print('\nGPT response:', res)
+            
+    return res
+
 def get_fn_description(my_function) -> (str, list):
     ''' Returns the modified docstring of my_function, that takes into account input variable names and types in angle brackets
     Also returns the list of input parameters to the function in sequence
     e.g.: Adds numbers x and y -> Adds numbers <x: int> and <y: int>
     Input variables that are optional (already assigned a default value) need not be in the docstring
     args and kwargs variables are not parsed '''
      
@@ -518,24 +570,129 @@
 
             except Exception as e:
                 error_msg = f"\n\nPrevious json: {res}\njson error: {str(e)}\nFix the error."                
                 print("An exception occurred:", str(e))
                 print("Current invalid json format:", res)
 
         return {}
+    
+    
+async def strict_json_async(system_prompt: str, user_prompt: str, output_format: dict, return_as_json = False, custom_checks: dict = dict(), check_data = None, delimiter: str = '###', num_tries: int = 3, openai_json_mode: bool = False, **kwargs):
+    ''' Ensures that OpenAI will always adhere to the desired output JSON format defined in output_format. 
+    Uses rule-based iterative feedback to ask GPT to self-correct.
+    Keeps trying up to num_tries it it does not. Returns empty JSON if unable to after num_tries iterations.
+    
+    Inputs (compulsory):
+    - system_prompt: String. Write in whatever you want GPT to become. e.g. "You are a \<purpose in life\>"
+    - user_prompt: String. The user input. Later, when we use it as a function, this is the function input
+    - output_format: Dict. JSON format with the key as the output key, and the value as the output description
+    
+    Inputs (optional):
+    - return_as_json: Bool. Default: False. Whether to return the output as a json. If False, returns as Python dict. If True, returns as json string
+    - custom_checks: Dict. Key is output key, value is function which does checking of content for output field
+    - check_data: Any data type. The additional data for custom_checks to use if required
+    - delimiter: String (Default: '###'). This is the delimiter to surround the keys. With delimiter ###, key becomes ###key###
+    - num_tries: Integer (default: 3). The number of tries to iteratively prompt GPT to generate correct json format
+    - openai_json_mode: Boolean (default: False). Whether or not to use OpenAI JSON Mode
+    - **kwargs: Dict. Additional arguments for LLM chat
+    
+    Output:
+    - res: Dict. The JSON output of the model. Returns {} if JSON parsing failed.
+    '''
+    # If OpenAI JSON mode is selected, then just let OpenAI do the processing
+    if openai_json_mode:
+        # add in code to warn user if type is defined for external function
+        type_check = False
+        for value in output_format.values():
+            if 'type:' in str(value):
+                type_check = True
+        if type_check:
+            print('Note: Type checking (type:) not done for OpenAI JSON Mode')
+        
+        output_format_prompt = "\nOutput in the following json string format: " + str(output_format) + "\nBe concise."
+            
+        my_system_prompt = str(system_prompt) + output_format_prompt
+        my_user_prompt = str(user_prompt) 
+            
+        res = await chat_async(my_system_prompt, my_user_prompt, response_format = {"type": "json_object"}, **kwargs)
+        
+        if return_as_json:
+            return res
+        else:
+            try:
+                loaded_json = json.loads(res)
+            except Exception as e:
+                loaded_json = {}
+            return loaded_json
+        
+    # Otherwise, implement JSON parsing using Strict JSON
+    else:
+        # start off with no error message
+        error_msg = ''
+
+        # wrap the values with angle brackets and wrap keys with delimiter to encourage LLM to modify it
+        new_output_format = wrap_with_angle_brackets(output_format, delimiter, 1)
+        
+        output_format_prompt = f'''\nOutput in the following json string format: {new_output_format}
+Update text enclosed in <>. Output only a valid json string beginning with {{ and ending with }}'''
+
+        for i in range(num_tries):
+            my_system_prompt = str(system_prompt) + output_format_prompt + error_msg
+            my_user_prompt = str(user_prompt) 
+
+            # Use OpenAI to get a response
+            res = chat(my_system_prompt, my_user_prompt, **kwargs)
+            
+            # extract only the chunk including the opening and closing braces
+            startindex = res.find('{')
+            endindex = res.rfind('}')
+            res = res[startindex: endindex+1]
+
+            # try-catch block to ensure output format is adhered to
+            try:
+                # check that res is a json string
+                if res[0] != '{' or res[-1] != '}':
+                    raise Exception('Ensure output must be a json string beginning with { and ending with }')
+                
+                # do checks for keys and output format, remove escape characters so code can be run
+                end_dict = check_key(res, output_format, new_output_format, delimiter, delimiter_num = 1, **kwargs)
+                
+                # run user defined custom checks now
+                for key in end_dict:
+                    if key in custom_checks:
+                        for check in custom_checks[key]:
+                            requirement, requirement_met, action_needed = check(end_dict[key], check_data)
+                            print(f'Running check for "{requirement}" on output field of "{key}"')
+                            if not requirement_met:
+                                print(f'Requirement not met. Action needed: "{action_needed}"\n\n')
+                                raise Exception(f'Output field of "{key}" does not meet requirement "{requirement}". Action needed: "{action_needed}"')
+                            else:
+                                print('Requirement met\n\n')
+                if return_as_json:
+                    return json.dumps(end_dict, ensure_ascii=False)
+                else:
+                    return end_dict
+
+            except Exception as e:
+                error_msg = f"\n\nPrevious json: {res}\njson error: {str(e)}\nFix the error."                
+                print("An exception occurred:", str(e))
+                print("Current invalid json format:", res)
+
+        return {}
 
 class Function:
     def __init__(self,
                  fn_description: str = '', 
                  output_format: dict = {},
                  examples = None,
                  external_fn = None,
                  is_compulsory = False,
                  fn_name = None,
                  llm = None,
+                 llm_async = None,
                  **kwargs):
         ''' 
         Creates an LLM-based function or wraps an external function using fn_description and outputs JSON based on output_format. 
         (Optional) Can define the function based on examples (list of Dict containing input and output variables for each example)
         (Optional) If you would like greater specificity in your function's input, you can describe the variable after the : in the input variable name, e.g. `<var1: an integer from 10 to 30`. Here, `var1` is the input variable and `an integer from 10 to 30` is the description.
         
         Inputs (primary):
@@ -582,14 +739,15 @@
 
         self.output_format = output_format
         self.examples = examples
         self.external_fn = external_fn
         self.is_compulsory = is_compulsory
         self.fn_name = fn_name
         self.llm = llm
+        self.llm_async = llm_async
         self.kwargs = kwargs
         
         self.variable_names = []
         self.shared_variable_names = []
         # use regex to extract variables from function description
         matches = re.findall(r'<(.*?)>', self.fn_description)
             
@@ -677,14 +835,88 @@
                             **self.kwargs, **strict_json_kwargs)
             
         # Else run the external function
         else:
             res = {}
             # if external function uses shared_variables, pass it in
             argspec = inspect.getfullargspec(self.external_fn)
+            if 'shared_variables' in argspec.args:
+                fn_output = self.external_fn(shared_variables = shared_variables, **function_kwargs)
+            else:
+                fn_output = self.external_fn(**function_kwargs)
+                
+            # if there is nothing in fn_output, skip this part
+            if fn_output is not None:
+                output_keys = list(self.output_format.keys())
+                # convert the external function into a tuple format to parse it through the JSON dictionary output format
+                if not isinstance(fn_output, tuple):
+                    fn_output = [fn_output]
+
+                for i in range(len(fn_output)):
+                    res[output_keys[i]] = fn_output[i]
+        
+        # check if any of the output variables have a s_, which means we update the shared_variables and not output it
+        keys = list(res.keys())
+        for each in keys:
+            if each[:2] == 's_':
+                shared_variables[each] = res[each]
+                del res[each]
+                
+        if res == {}:
+            res = {'Status': 'Completed'}
+
+        return res
+    
+    async def async_call(self, *args, **kwargs):
+        ''' Describes the function, and inputs the relevant parameters as either unnamed variables (args) or named variables (kwargs)
+        
+        Inputs:
+        - shared_varables: Dict. Default: empty dict. The variables which will be shared between functions. Only passed in if required by function 
+        - *args: Tuple. Unnamed input variables of the function. Will be processed to var1, var2 and so on based on order in the tuple
+        - **kwargs: Dict. Named input variables of the function. Can also be variables to pass into strict_json
+        
+        Output:
+        - res: Dict. JSON containing the output variables'''
+        
+        # get the shared_variables if there are any
+        shared_variables = kwargs.get('shared_variables', {})
+        # remove the mention of shared_variables in kwargs
+        if 'shared_variables' in kwargs:
+            del kwargs['shared_variables']
+        
+        # extract out only variables listed in variable_list from kwargs
+        function_kwargs = {my_key: kwargs[my_key] for my_key in kwargs if my_key in self.variable_names}
+        # additionally, if function references something in shared_variables, add that in
+        for variable in self.shared_variable_names:
+            if variable in shared_variables:
+                function_kwargs[variable] = shared_variables[variable]
+        
+        # extract out only variables not listed in variable list
+        strict_json_kwargs = {my_key: kwargs[my_key] for my_key in kwargs if my_key not in self.variable_names}
+        
+        # Do the auto-naming of variables as var1, var2, or as variable names defined in variable_names
+        for num, arg in enumerate(args):
+            if len(self.variable_names) > num:
+                function_kwargs[self.variable_names[num]] = arg
+            else:
+                function_kwargs['var'+str(num+1)] = arg
+                
+        # If strict_json function, do the function. 
+        if self.external_fn is None:
+            res = await strict_json_async(system_prompt = self.fn_description,
+                            user_prompt = function_kwargs,
+                            output_format = self.output_format,
+                            llm_async = self.llm_async,
+                            **self.kwargs, **strict_json_kwargs)
+            
+        # Else run the external function
+        else:
+            res = {}
+            # if external function uses shared_variables, pass it in
+            argspec = inspect.getfullargspec(self.external_fn)
             if 'shared_variables' in argspec.args:
                 fn_output = self.external_fn(shared_variables = shared_variables, **function_kwargs)
             else:
                 fn_output = self.external_fn(**function_kwargs)
                 
             # if there is nothing in fn_output, skip this part
             if fn_output is not None:
```

### Comparing `taskgen_ai-1.4.0/taskgen_ai.egg-info/PKG-INFO` & `taskgen_ai-2.0.0/taskgen_ai.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: taskgen-ai
-Version: 1.4.0
+Version: 2.0.0
 Summary: A Task-based agentic framework building on StrictJSON outputs by LLM agents
 Author-email: John Tan Chong Min <tanchongmin@gmail.com>
 Project-URL: Homepage, https://github.com/simbianai/taskgen
 Project-URL: Issues, https://github.com/simbianai/taskgen/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: openai>=1.3.6
 Requires-Dist: dill>=0.3.7
 
-# TaskGen v1.4.0
+# TaskGen v2.0.0
 ### A Task-based agentic framework building on StrictJSON outputs by LLM agents
 - Related Repositories: StrictJSON (https://github.com/tanchongmin/strictjson)
 - Video (Part 1): https://www.youtube.com/watch?v=O_XyTT7QGH4
 - Video (Part 2): https://www.youtube.com/watch?v=OWk7moRfTPE
 
 ### Creator's Preamble
 Happy to share that the task-based agentic framework I have been working on - TaskGen - is largely complete! 
@@ -55,14 +55,19 @@
 - Discussion Channel (my discord - John's AI Group): [https://discord.gg/bzp87AHJy5](https://discord.gg/bzp87AHJy5)
 
 ## How do I use this? 
 1. Download package via command line ```pip install taskgen-ai```
 2. Set up your OpenAPI API Key
 3. Import the required functions from ```taskgen``` and use them!
 
+## Differences in LLM for Agentic Framework
+- ChatGPT (gpt-3.5-turbo) is consistent only if you specify very clearly what you want the Agent to do and give examples of what you want
+- gpt-4-turbo and more advanced models can perform better zero-shot without much examples
+- TaskGen is compatible with ChatGPT and similar models, but for more robust use, consider using gpt-4-turbo and better models
+
 # Agent Basics - See Tutorial 1
 - Create an agent by entering your agent's name and description
 - Agents are task-based, so they will help generate subtasks to fulfil your main task
 - Agents are made to be non-verbose, so they will just focus only on task instruction (Much more efficient compared to conversational-based agentic frameworks like AutoGen)
     
 ## Example Agent Creation
 ```python
@@ -255,26 +260,26 @@
 # Define your meta-agent
 my_agent = Agent('Menu Creator', 
                  'Creates a menu for a restaurant. Menu item includes Name, Description, Ingredients, Pricing.')
 
 # Define your agent list. Note you can just assign functions to the agent in place using .assign_functions(function_list)
 agent_list = [
     Agent('Chef', 'Takes in dish names and comes up with ingredients for each of them. Does not generate prices.'),
-    Agent('Boss', 'Takes in menu items and curates them according to price'),
+    Agent('Boss', ''Does final quality check on menu items'),
     Agent('Creative Writer', 'Takes in a cuisine type and generates interesting dish names and descriptions. Does not generate prices or ingredients.', max_subtasks = 2),
     Agent('Economist', 'Takes in dish names and comes up with fictitious pricing for each of them')
     ]
 
 my_agent.assign_agents(agent_list)
 ```
 
 ## Run the Meta Agent
 - Let us run the agent and see the interactions between the Meta Agent and Inner Agents to solve the task!
 ```python
-output = my_agent.run('Give me 5 menu items with name, description, ingredients and price based on Italian food choices.')
+output = my_agent.run('Give me 5 menu items with name, description, ingredients and price based on Italian food choices. Ensure all parts of menu are generated.')
 ```
 
 # Shared Variables - See Tutorial 3
 
 *"Because text is not enough"* - Anonymous
 
 - `shared_variables` is a dictionary, that is initialised in Agent (default empty dictionary), and can be referenced by any function of the agent (including Inner Agents and their functions)
@@ -310,20 +315,20 @@
 
 ## Example External Function Accessing Shared Variables (Advanced)
 ```python
 # Use shared_variables as input to your external function to access and modify the shared variables
 def generate_quotes(shared_variables, number_of_quotes: int, category: str):
     ''' Generates number_of_quotes quotes about category '''
     # Retrieve from shared variables
-    my_quote_list = shared_variables['s_quote_list']
+    my_quote_list = shared_variables['quote_list']
     
     ### Add your function code here ###
     
     # Store back to shared variables
-    shared_variables['s_quote_list'] = my_quote_list
+    shared_variables['quote_list'] = my_quote_list
 
 generate_quote_fn = Function(output_format = {}, external_fn = generate_quotes)
 ```
 
 # Memory - See Tutorial 4
 
 ## Key Philosophy
@@ -370,17 +375,18 @@
 <br></br>
 - Implementing your own specific instructions to the default planner prompt
     - Implement your own memory-based RAG / global prompt instruction if you need more than what the default prompt can achieve
 <br></br>
 - Avoid Multiple Similar Subtasks in `subtasks_history`
     - If you have multiple similar subtask names, then it is likely the Agent can be confused and think it has already done the subtask
     - In this case, you can disambiguate by resetting the agent and store the persistent information in `shared_variables` and provide it to the agent using `get_global_context`
+    - Has the benefit of shifting the Start State closer to End State desired by resetting the Agent's planning cycle
 
 # Known Limitations
-1. As the agent uses the term "Overall Plan" for its internal planning, try not to use the word "plan" in your query or context, if not it might confuse the agent. Use alternative words like "schedule"
+- To be added
 
 # Contributing to the project
 
 ## Test locally
 1. Clone the repository
 2. If using a virtual environment, activate it
 3. `cd` into taskgen repository
```

