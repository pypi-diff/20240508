# Comparing `tmp/taskwarrior_flow-0.3.0.tar.gz` & `tmp/taskwarrior_flow-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskwarrior_flow-0.3.0.tar", max compression
+gzip compressed data, was "taskwarrior_flow-0.3.1.tar", max compression
```

## Comparing `taskwarrior_flow-0.3.0.tar` & `taskwarrior_flow-0.3.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11357 2024-05-07 05:43:01.918156 taskwarrior_flow-0.3.0/LICENSE
--rw-r--r--   0        0        0     1452 2024-05-07 05:43:01.918156 taskwarrior_flow-0.3.0/README.md
--rw-r--r--   0        0        0     1035 2024-05-07 05:43:01.918156 taskwarrior_flow-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      902 2024-05-07 05:43:01.918156 taskwarrior_flow-0.3.0/tools/__init__.py
--rw-r--r--   0        0        0     1842 2024-05-07 05:43:01.918156 taskwarrior_flow-0.3.0/tools/main.py
--rw-r--r--   0        0        0    20222 2024-05-07 05:43:01.918156 taskwarrior_flow-0.3.0/tools/utils.py
--rw-r--r--   0        0        0     2074 1970-01-01 00:00:00.000000 taskwarrior_flow-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-08 07:26:41.362267 taskwarrior_flow-0.3.1/LICENSE
+-rw-r--r--   0        0        0     1452 2024-05-08 07:26:41.362267 taskwarrior_flow-0.3.1/README.md
+-rw-r--r--   0        0        0     1035 2024-05-08 07:26:41.362267 taskwarrior_flow-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     1351 2024-05-08 07:26:41.362267 taskwarrior_flow-0.3.1/tools/__init__.py
+-rw-r--r--   0        0        0     3237 2024-05-08 07:26:41.362267 taskwarrior_flow-0.3.1/tools/main.py
+-rw-r--r--   0        0        0    20383 2024-05-08 07:26:41.362267 taskwarrior_flow-0.3.1/tools/utils.py
+-rw-r--r--   0        0        0     2074 1970-01-01 00:00:00.000000 taskwarrior_flow-0.3.1/PKG-INFO
```

### Comparing `taskwarrior_flow-0.3.0/LICENSE` & `taskwarrior_flow-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `taskwarrior_flow-0.3.0/README.md` & `taskwarrior_flow-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `taskwarrior_flow-0.3.0/pyproject.toml` & `taskwarrior_flow-0.3.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "taskwarrior_flow"
-version = "0.3.0"
+version = "0.3.1"
 description = "Set of helpers for improving Taskwarrior workflow"
 authors = ["Ben Trinh <huantrinh1802@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "tools" }]
 
 [tool.poetry.scripts]
 twf = 'tools.main:app'
```

### Comparing `taskwarrior_flow-0.3.0/tools/__init__.py` & `taskwarrior_flow-0.3.1/tools/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,22 +2,32 @@
 import os
 
 config_file = os.environ.get("TW_CONFIG", f'{os.path.expanduser("~")}/.local/share/nvim/m_taskwarrior_d.json')
 if os.path.isfile(config_file):
     with open(config_file, "r") as f:
         tw_config = json.load(f)
 else:
-    with open(config_file, "w") as f:
-        tw_config = {
-            "use_mtwd": False,
-            "flow_config": {"task": {"data": "~/.task", "config": "~/.taskrc"}},
-            "add_templates": {"date_fields": ["due", "scheduled"], "data": []},
-            "saved_queries": {"name_max_length": 0, "data": []},
-        }
-        f.write(json.dumps(tw_config))
+    if config_file == '/tmp/m_taskwarrior_d.json':
+        with open(config_file, "w") as f:
+            tw_config = {
+                "use_mtwd": False,
+                "flow_config": {"task": {"data": "~/.task", "config": "~/.taskrc"}},
+
+                "saved_queries": {"name_max_length": 0, "data": [{"query": "project:Test", "name": "Test"}]},
+            }
+            f.write(json.dumps(tw_config))
+    else:
+        with open(config_file, "w") as f:
+            tw_config = {
+                "use_mtwd": False,
+                "flow_config": {"task": {"data": "~/.task", "config": "~/.taskrc"}},
+                "add_templates": {"date_fields": ["due", "scheduled"], "data": []},
+                "saved_queries": {"name_max_length": 0, "data": []},
+            }
+            f.write(json.dumps(tw_config))
 group_mappings = {key: f'TASKDATA={value["data"]}' for key, value in tw_config["flow_config"].items()}
 
 
 def group_mappings_completion():
     autocompletions = []
     for key in group_mappings:
         autocompletions.append((key, f"Taskwarrior data group: {key}"))
```

### Comparing `taskwarrior_flow-0.3.0/tools/utils.py` & `taskwarrior_flow-0.3.1/tools/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,39 +9,30 @@
 import questionary
 import typer
 from prompt_toolkit.shortcuts import CompleteStyle
 from rich import print as rprint
 
 from tools import config_file, group_mappings, group_mappings_completion, tw_config
 
-utils = typer.Typer()
+utils_commands = typer.Typer()
 question_style = questionary.Style(
     [
         ("qmark", "fg:#007777 bold"),  # token in front of the question
         ("question", "bold"),  # question text
         ("answer", "fg:white bg:#007777 "),  # submitted answer text behind the question
         ("pointer", "fg:#007777 bold"),  # pointer used in select and checkbox prompts
         ("highlighted", "fg:#007777 bold"),  # pointed-at choice in select and checkbox prompts
         ("selected", "fg:white"),  # style for a selected item of a checkbox
         ("separator", "fg:#008888"),  # separator in lists
         ("instruction", "fg:#858585"),  # user instructions for select, rawselect, checkbox
         ("text", ""),  # plain text
         ("disabled", "fg:#858585 italic"),  # disabled choices for select and checkbox prompts
     ]
 )
-projects = subprocess.run("task _projects", shell=True, capture_output=True).stdout.decode().split("\n")
-tags = subprocess.run("task _tags", shell=True, capture_output=True).stdout.decode().split("\n")
-preset_questions = {
-    "project": questionary.autocomplete(
-        "Enter project", choices=projects, style=question_style, complete_style=CompleteStyle.MULTI_COLUMN
-    ),
-    "tags": questionary.autocomplete(
-        "Enter tags", choices=tags, style=question_style, complete_style=CompleteStyle.MULTI_COLUMN
-    ),
-}
+
 
 
 class FunctionsGroup(TypedDict):
     func: Callable
     help: str
 
 
@@ -119,32 +110,33 @@
     ]
     chosen_template = safe_ask(
         questionary.rawselect("Select template", choices=templates, use_jk_keys=True, style=question_style)
     )
     if chosen_template is None:
         return
     questions = {}
+    preset_questions = get_preset_questions(group)
     for name, field in tw_config["add_templates"]["data"][chosen_template]["fields"].items():
         if name in preset_questions:
             questions[name] = preset_questions[name]
-        elif name in tw_config['add_templates']['date_fields']:
+        elif name in tw_config["add_templates"]["date_fields"]:
             questions[name] = questionary.text(f"Enter {name}", style=question_style, validate=DateValidator)
         else:
             questions[name] = questionary.text(f"Enter {name}", instruction="Use ';' for list\n", style=question_style)
     answers = safe_ask(questionary.form(**questions))
     if answers is None:
         return
     parts = ""
     annotations: None | list[str] = None
     for name, field in tw_config["add_templates"]["data"][chosen_template]["fields"].items():
         value = answers.get(name, "")
         if len(value) != 0 or answers[name] != " ":
             if name in "annotations":
                 annotations = [annotation for annotation in answers[name].split(";")]
-            elif name in tw_config['add_templates']['date_fields']:
+            elif name in tw_config["add_templates"]["date_fields"]:
                 date_str = dateparser.parse(answers[name])
                 if date_str is not None:
                     date_str = date_str.strftime("%Y-%m-%dT%H:%M:%S")
                     parts += " " + field.replace("%s", date_str)
             else:
                 parts += " " + " ".join(
                     field.replace("%s", item) if item != "" else "" for item in answers[name].split(";")
@@ -200,15 +192,15 @@
 def create_group_completion():
     auto_completions = []
     for key, value in create_groups.items():
         auto_completions.append((key, value["help"]))
     return auto_completions
 
 
-@utils.command("add", help="Add task, query, and template")
+@utils_commands.command("add", help="Add task, query, and template")
 def task_create(
     name: Annotated[str, typer.Argument(autocompletion=create_group_completion)] = "task",
     group: Annotated[str, typer.Option("--group", "-g", autocompletion=group_mappings_completion)] = "task",
 ):
     create_groups[name]["func"](group)
 
 
@@ -346,15 +338,15 @@
 def edit_group_completion():
     auto_completions = []
     for group, group_info in edit_groups.items():
         auto_completions.append((group, group_info["help"]))
     return auto_completions
 
 
-@utils.command("edit", help="Edit query, and template")
+@utils_commands.command("edit", help="Edit query, and template")
 def task_edit(
     name: Annotated[str, typer.Argument(autocompletion=edit_group_completion)] = "template",
 ):
     edit_groups[name]["func"]()
 
 
 def view_task():
@@ -405,15 +397,15 @@
 def view_group_completion():
     auto_completions = []
     for key, value in view_groups.items():
         auto_completions.append((key, value["help"]))
     return auto_completions
 
 
-@utils.command("view", help="View task and template")
+@utils_commands.command("view", help="View task and template")
 def task_view(
     name: Annotated[str, typer.Argument(autocompletion=view_group_completion)] = "task",
 ):
     view_groups[name]["func"]()
 
 
 def delete_template():
@@ -514,10 +506,24 @@
 def delete_group_completion():
     auto_completions = []
     for key, value in delete_groups.items():
         auto_completions.append((key, value["help"]))
     return auto_completions
 
 
-@utils.command("delete", help="Delete task, query, template, and group")
+@utils_commands.command("delete", help="Delete task, query, template, and group")
 def task_delete(name: Annotated[str, typer.Argument(autocompletion=edit_group_completion)] = "template"):
     delete_groups[name]["func"]()
+
+
+def get_preset_questions(group):
+    projects = subprocess.run("task _projects", shell=True, capture_output=True).stdout.decode().split("\n")
+    tags = subprocess.run("task _tags", shell=True, capture_output=True).stdout.decode().split("\n")
+    return {
+        "project": questionary.autocomplete(
+            "Enter project", choices=projects, style=question_style, complete_style=CompleteStyle.MULTI_COLUMN
+        ),
+        "tags": questionary.autocomplete(
+            "Enter tags", choices=tags, style=question_style, complete_style=CompleteStyle.MULTI_COLUMN
+        ),
+    }
+
```

### Comparing `taskwarrior_flow-0.3.0/PKG-INFO` & `taskwarrior_flow-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taskwarrior_flow
-Version: 0.3.0
+Version: 0.3.1
 Summary: Set of helpers for improving Taskwarrior workflow
 Author: Ben Trinh
 Author-email: huantrinh1802@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

