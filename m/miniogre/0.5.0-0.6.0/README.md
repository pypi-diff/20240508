# Comparing `tmp/miniogre-0.5.0.tar.gz` & `tmp/miniogre-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "miniogre-0.5.0.tar", max compression
+gzip compressed data, was "miniogre-0.6.0.tar", max compression
```

## Comparing `miniogre-0.5.0.tar` & `miniogre-0.6.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     7173 2024-04-19 06:43:53.709826 miniogre-0.5.0/.env
--rw-r--r--   0        0        0    11357 2024-04-19 06:43:53.709826 miniogre-0.5.0/LICENSE
--rw-r--r--   0        0        0     4134 2024-04-19 06:43:53.709826 miniogre-0.5.0/README.md
--rw-r--r--   0        0        0      125 2024-04-19 06:43:53.709826 miniogre-0.5.0/miniogre/__init__.py
--rw-r--r--   0        0        0    19542 2024-04-19 06:43:53.709826 miniogre-0.5.0/miniogre/actions.py
--rw-r--r--   0        0        0     4564 2024-04-19 06:43:53.709826 miniogre-0.5.0/miniogre/config.py
--rw-r--r--   0        0        0    10297 2024-04-19 06:43:53.709826 miniogre-0.5.0/miniogre/constants.py
--rw-r--r--   0        0        0     2630 2024-04-19 06:43:53.709826 miniogre-0.5.0/miniogre/main.py
--rw-r--r--   0        0        0      793 2024-04-19 06:43:53.713826 miniogre-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     5229 1970-01-01 00:00:00.000000 miniogre-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     7173 2024-05-08 05:44:36.958871 miniogre-0.6.0/.env
+-rw-r--r--   0        0        0    11357 2024-05-08 05:44:36.958871 miniogre-0.6.0/LICENSE
+-rw-r--r--   0        0        0     4134 2024-05-08 05:44:36.958871 miniogre-0.6.0/README.md
+-rw-r--r--   0        0        0      125 2024-05-08 05:44:36.958871 miniogre-0.6.0/miniogre/__init__.py
+-rw-r--r--   0        0        0    20236 2024-05-08 05:44:36.958871 miniogre-0.6.0/miniogre/actions.py
+-rw-r--r--   0        0        0     4564 2024-05-08 05:44:36.958871 miniogre-0.6.0/miniogre/config.py
+-rw-r--r--   0        0        0    10561 2024-05-08 05:44:36.958871 miniogre-0.6.0/miniogre/constants.py
+-rw-r--r--   0        0        0     3044 2024-05-08 05:44:36.958871 miniogre-0.6.0/miniogre/main.py
+-rw-r--r--   0        0        0      792 2024-05-08 05:44:36.958871 miniogre-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     5222 1970-01-01 00:00:00.000000 miniogre-0.6.0/PKG-INFO
```

### Comparing `miniogre-0.5.0/.env` & `miniogre-0.6.0/.env`

 * *Files identical despite different names*

### Comparing `miniogre-0.5.0/LICENSE` & `miniogre-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `miniogre-0.5.0/README.md` & `miniogre-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `miniogre-0.5.0/miniogre/actions.py` & `miniogre-0.6.0/miniogre/actions.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,548 +1,645 @@
-import os
 import ast
-import emoji
+import os
 import platform
 import subprocess
-from openai import OpenAI
-from octoai.client import Client as OctoAiClient
-from groq.cloud.core import Completion
+
+import emoji
+from groq import Groq
+# from groq.cloud.core import Completion
 from mistralai.client import MistralClient
 from mistralai.models.chat_completion import ChatMessage
+from octoai.client import Client as OctoAiClient
+from openai import OpenAI
 from pyfiglet import Figlet
 from rich import print as rprint
 from yaspin import yaspin
+
 from .constants import *
 
 
 def starting_emoji():
-    print(emoji.emojize(':ogre: Starting miniogre...'))
+    print(emoji.emojize(":ogre: Starting miniogre..."))
+
 
 def end_emoji():
-    print(emoji.emojize(':hourglass_done: Done.'))
+    print(emoji.emojize(":hourglass_done: Done."))
+
 
 def build_emoji():
-    print(emoji.emojize(':spouting_whale: Building Docker image...'))
+    print(emoji.emojize(":spouting_whale: Building Docker image..."))
+
 
 def spinup_emoji():
-    print(emoji.emojize(':rocket: Spinning up container...'))
+    print(emoji.emojize(":rocket: Spinning up container..."))
+
 
 def requirements_emoji():
-    print(emoji.emojize(':thinking_face: Generating requirements...'))
+    print(emoji.emojize(":thinking_face: Generating requirements..."))
+
 
 def cleaning_requirements_emoji():
-    print(emoji.emojize(':cooking: Refining...'))
+    print(emoji.emojize(":cooking: Refining..."))
+
 
 def generate_context_emoji():
-    print(emoji.emojize(':magnifying_glass_tilted_left: Generating context...'))
+    print(emoji.emojize(":magnifying_glass_tilted_left: Generating context..."))
+
 
 def readme_emoji():
-    print(emoji.emojize(':notebook: Generating new README.md...'))
+    print(emoji.emojize(":notebook: Generating new README.md..."))
+
 
 def list_files(project_path):
     # List all files in current directory and subdirectories
     files = []
     for root, dirs, filenames in os.walk(project_path):
-        if '.git' in dirs:
-            dirs.remove('.git')
-        if '__pycache__' in dirs:
-            dirs.remove('__pycache__')
+        if ".git" in dirs:
+            dirs.remove(".git")
+        if "__pycache__" in dirs:
+            dirs.remove("__pycache__")
         for filename in filenames:
             files.append(os.path.join(root, filename))
     return files
 
+
 # Get file extensions
 def get_extensions(files):
     extensions = [os.path.splitext(f)[1] for f in files]
     return extensions
 
+
 # Count file extensions
 def count_extensions(extensions):
     counts = {}
     for ext in extensions:
         if ext in counts:
             counts[ext] += 1
         else:
             counts[ext] = 1
     return counts
 
+
 # Get most prevalent extension for code files
 def determine_most_ext(counts):
-    #TODO: implement logic to determine the codebase.    
-    return '.py'
+    # TODO: implement logic to determine the codebase.
+    return ".py"
+
 
 def find_readme(project_path):
     files = list_files(project_path)
-    readme_files = [f for f in files if os.path.basename(f).lower().startswith('readme')]
+    readme_files = [
+        f for f in files if os.path.basename(f).lower().startswith("readme")
+    ]
 
     if readme_files:
         return readme_files[0]
     else:
         return None
 
+
 def read_file_contents(path_to_file):
     if path_to_file == None:
-        return ''
+        return ""
     else:
         if os.path.exists(path_to_file):
-            with open(path_to_file, 'r') as f:
+            with open(path_to_file, "r") as f:
                 contents = f.read()
             return contents
         else:
-            return ''
+            return ""
+
 
 def conform_to_pep8(filename):
 
-    pep8_cmd = 'autopep8 --in-place --aggressive {}'.format(filename)
-    
-    p = subprocess.Popen(pep8_cmd, stdout=subprocess.PIPE, stderr=subprocess.PIPE, shell=True)
+    pep8_cmd = "autopep8 --in-place --aggressive {}".format(filename)
+
+    p = subprocess.Popen(
+        pep8_cmd, stdout=subprocess.PIPE, stderr=subprocess.PIPE, shell=True
+    )
     (out, err) = p.communicate()
     p_status = p.wait()
 
     return 0
 
+
 def extract_external_imports(code):
 
     external_imports = []
-    
+
     tree = ast.parse(code)
-    
+
     for node in ast.walk(tree):
         if isinstance(node, ast.Import):
             for name in node.names:
-                if not name.name.startswith('.'):
+                if not name.name.startswith("."):
                     external_imports.append(name.name)
         elif isinstance(node, ast.ImportFrom):
-            if not node.module.startswith('.'):
+            if not node.module.startswith("."):
                 external_imports.append(node.module)
-   
+
     return external_imports
 
-def extract_requirements_from_code(project_path, ext, generate = True):
+
+def extract_requirements_from_code(project_path, ext, generate=True):
 
     requirements_emoji()
 
     if generate:
         files = list_files(project_path)
         matching = [f for f in files if os.path.splitext(f)[1] == ext]
 
         external_imports = []
         for filename in matching:
             i = 0
             while i < 2:
-                with open(os.path.join(project_path, filename), 'r') as readfile:
+                with open(os.path.join(project_path, filename), "r") as readfile:
                     content = readfile.read()
                     try:
                         external_imports.append(extract_external_imports(content))
                         i = 2
                     except Exception as e:
                         if i == 1:
                             i = 2
                             print(e)
-                            print("External imports extraction failed for file {}: {}".format(filename, Exception))
+                            print(
+                                "External imports extraction failed for file {}: {}".format(
+                                    filename, Exception
+                                )
+                            )
                         else:
                             conform_to_pep8(filename)
                             i += 1
-                
-        external_imports = [imp.split('.')[0] for sublist in external_imports for imp in sublist]
+
+        external_imports = [
+            imp.split(".")[0] for sublist in external_imports for imp in sublist
+        ]
         external_imports = list(set(external_imports))
 
-        requirements = '\n'.join(external_imports)
+        requirements = "\n".join(external_imports)
     else:
-        with open('{}/requirements.txt'.format(os.getenv('OGRE_DIR', OGRE_DIR)), 'r') as f:
+        with open(
+            "{}/requirements.txt".format(os.getenv("OGRE_DIR", OGRE_DIR)), "r"
+        ) as f:
             requirements = f.read()
     return requirements
 
 
-
 def append_files_with_ext(project_path, ext, limit, output_file):
     files = list_files(project_path)
     matching = [f for f in files if os.path.splitext(f)[1] == ext]
-    
+
     if limit < len(matching):
         matching = matching[:limit]
-        
-    contents = ''
-    with open(output_file, 'a') as outfile:
+
+    contents = ""
+    with open(output_file, "a") as outfile:
         for filename in matching:
-            with open(os.path.join(project_path, filename), 'r') as readfile:
+            with open(os.path.join(project_path, filename), "r") as readfile:
                 contents += readfile.read()
 
     return contents
 
+
 def generate_context_file(readme_text, source_text, output_file):
     """
-    Generates the context file by appending the README and the source code text. 
+    Generates the context file by appending the README and the source code text.
     The content of this file will be used to extract the dependencies.
     """
     out_text = readme_text + source_text
-    
-    with open(output_file, 'w') as out:
+
+    with open(output_file, "w") as out:
         out.write(out_text)
-    
-    with open(output_file, 'r') as f:
+
+    with open(output_file, "r") as f:
         return f.read()
 
+
 def read_context(path_to_context_file):
-    with open(path_to_context_file, 'r') as f:
+    with open(path_to_context_file, "r") as f:
         contents = f.read()
     return contents
 
+
 def extract_requirements(provider, contents):
     requirements_emoji()
-    if provider == 'openai':
+    if provider == "openai":
         res = extract_requirements_openai(contents)
-    elif provider == 'octoai':
+    elif provider == "octoai":
         res = extract_requirements_octoai(contents)
-    elif provider == 'groq':
+    elif provider == "groq":
         res = extract_requirements_groq(contents)
     return res
 
+
 def extract_requirements_openai(contents):
-    model = os.getenv('OPENAI_MODEL', OPENAI_MODEL)
-    prompt = os.getenv('OPENAI_SECRET_PROMPT', OPENAI_SECRET_PROMPT)
+    model = os.getenv("OPENAI_MODEL", OPENAI_MODEL)
+    prompt = os.getenv("OPENAI_SECRET_PROMPT", OPENAI_SECRET_PROMPT)
     client = OpenAI()
     completion = client.chat.completions.create(
-                  model=model,
-                  messages=[
-                      {"role": "system", "content": prompt},
-                      {"role": "user", "content": contents}
-                  ]
-              )
+        model=model,
+        messages=[
+            {"role": "system", "content": prompt},
+            {"role": "user", "content": contents},
+        ],
+    )
     requirements = completion.choices[0].message.content
-    
+
     return requirements
 
+
 def extract_requirements_octoai(contents):
-    model = os.getenv('OCTOAI_MODEL', OCTOAI_MODEL)
-    prompt = os.getenv('OCTOAI_SECRET_PROMPT', OCTOAI_SECRET_PROMPT)
+    model = os.getenv("OCTOAI_MODEL", OCTOAI_MODEL)
+    prompt = os.getenv("OCTOAI_SECRET_PROMPT", OCTOAI_SECRET_PROMPT)
     client = OctoAiClient()
 
     completion = client.chat.completions.create(
-    messages=[
-            {
-                "role": "system",
-                "content": prompt
-            },
-            {
-                "role": "user",
-                "content": contents
-            }
+        messages=[
+            {"role": "system", "content": prompt},
+            {"role": "user", "content": contents},
         ],
-    model=model,
-    max_tokens=20000,
-    presence_penalty=0,
-    temperature=0.1,
-    top_p=0.9)
+        model=model,
+        max_tokens=20000,
+        presence_penalty=0,
+        temperature=0.1,
+        top_p=0.9,
+    )
 
     requirements = completion.choices[0].message.content
 
     return requirements
 
-def extract_requirements_groq(contents):
-    prompt = os.getenv('GROQ_SECRET_PROMPT', GROQ_SECRET_PROMPT)
-    with Completion() as completion:
-        full_prompt = prompt + " " + contents
-        response, id, stats = completion.send_prompt("llama2-70b-4096", user_prompt=full_prompt)
-        if response != "":
-            print(f"\nPrompt: {prompt}\n")
-            print(f"Request ID: {id}")
-            print(f"Output:\n {response}\n")
-            print(f"Stats:\n {stats}\n")
-    return response
+
+# def extract_requirements_groq(contents):
+#    prompt = os.getenv("GROQ_SECRET_PROMPT", GROQ_SECRET_PROMPT)
+#    with Completion() as completion:
+#        full_prompt = prompt + " " + contents
+#        response, id, stats = completion.send_prompt(
+#            "llama2-70b-4096", user_prompt=full_prompt
+#        )
+#        if response != "":
+#            print(f"\nPrompt: {prompt}\n")
+#            print(f"Request ID: {id}")
+#            print(f"Output:\n {response}\n")
+#            print(f"Stats:\n {stats}\n")
+#    return response
+
 
 def clean_requirements(provider, requirements):
     cleaning_requirements_emoji()
-    if provider == 'openai':
+    if provider == "openai":
         res = clean_requirements_openai(requirements)
-    elif provider == 'ollama':
+    elif provider == "ollama":
         res = clean_requirements_ollama(requirements)
-    elif provider == 'octoai':
+    elif provider == "octoai":
         res = clean_requirements_octoai(requirements)
-    elif provider == 'groq':
+    elif provider == "groq":
         res = clean_requirements_groq(requirements)
-    elif provider == 'mistral':
+    elif provider == "mistral":
         res = clean_requirements_mistral(requirements)
     return res
 
+
 def clean_requirements_ollama(requirements):
-    model = os.getenv('OLLAMA_MODEL', OLLAMA_MODEL)
-    prompt = os.getenv('CLEAN_REQUIREMENTS_SECRET_PROMPT', CLEAN_REQUIREMENTS_SECRET_PROMPT)
-    api_server = os.getenv('OLLAMA_API_SERVER', OLLAMA_API_SERVER)
+    model = os.getenv("OLLAMA_MODEL", OLLAMA_MODEL)
+    prompt = os.getenv(
+        "CLEAN_REQUIREMENTS_SECRET_PROMPT", CLEAN_REQUIREMENTS_SECRET_PROMPT
+    )
+    api_server = os.getenv("OLLAMA_API_SERVER", OLLAMA_API_SERVER)
     # print(f"{api_server=} {model=} {prompt=}")
-    client = OpenAI(base_url=api_server, api_key='ollama')
+    client = OpenAI(base_url=api_server, api_key="ollama")
     completion = client.chat.completions.create(
-                  model=model,
-                  messages=[
-                      {"role": "system", "content": prompt},
-                      {"role": "user", "content": requirements}
-                  ]
-              )
+        model=model,
+        messages=[
+            {"role": "system", "content": prompt},
+            {"role": "user", "content": requirements},
+        ],
+    )
     requirements = completion.choices[0].message.content
 
     return requirements
 
+
 def clean_requirements_openai(requirements):
-    model = os.getenv('OPENAI_MODEL', OPENAI_MODEL)
-    prompt = os.getenv('CLEAN_REQUIREMENTS_SECRET_PROMPT', CLEAN_REQUIREMENTS_SECRET_PROMPT)
+    model = os.getenv("OPENAI_MODEL", OPENAI_MODEL)
+    prompt = os.getenv(
+        "CLEAN_REQUIREMENTS_SECRET_PROMPT", CLEAN_REQUIREMENTS_SECRET_PROMPT
+    )
     # print(f"{model=} {prompt=}")
     client = OpenAI()
     completion = client.chat.completions.create(
-                  model=model,
-                  messages=[
-                      {"role": "system", "content": prompt},
-                      {"role": "user", "content": requirements}
-                  ]
-              )
+        model=model,
+        messages=[
+            {"role": "system", "content": prompt},
+            {"role": "user", "content": requirements},
+        ],
+    )
     requirements = completion.choices[0].message.content
 
     return requirements
 
+
 def clean_requirements_mistral(requirements):
-    model = os.getenv('MISTRAL_MODEL', MISTRAL_MODEL)
-    prompt = os.getenv('CLEAN_REQUIREMENTS_SECRET_PROMPT', CLEAN_REQUIREMENTS_SECRET_PROMPT)
+    model = os.getenv("MISTRAL_MODEL", MISTRAL_MODEL)
+    prompt = os.getenv(
+        "CLEAN_REQUIREMENTS_SECRET_PROMPT", CLEAN_REQUIREMENTS_SECRET_PROMPT
+    )
     api_key = os.environ["MISTRAL_API_KEY"]
     client = MistralClient(api_key=api_key)
-    content = prompt + '\n' + requirements
+    content = prompt + "\n" + requirements
     messages = [ChatMessage(role="user", content=content)]
 
     # No streaming
     chat_response = client.chat(
         model=model,
         messages=messages,
     )
     requirements = chat_response.choices[0].message.content
 
     return requirements
 
+
 def clean_requirements_groq(requirements):
-    model = os.getenv('GROQ_MODEL', GROQ_MODEL)
-    prompt = os.getenv('GROQ_CLEAN_REQUIREMENTS_SECRET_PROMPT', GROQ_CLEAN_REQUIREMENTS_SECRET_PROMPT)
-    with Completion() as completion:
-        full_prompt = prompt + " " + requirements
-        response, id, stats = completion.send_prompt(model, user_prompt=full_prompt)
-        
+    model = os.getenv("GROQ_MODEL", GROQ_MODEL)
+    prompt = os.getenv(
+        "GROQ_CLEAN_REQUIREMENTS_SECRET_PROMPT", GROQ_CLEAN_REQUIREMENTS_SECRET_PROMPT
+    )
+
+    client = Groq(
+        api_key=os.environ.get("GROQ_API_KEY"),
+    )
+
+    chat_completion = client.chat.completions.create(
+        messages=[
+            {
+                "role": "user",
+                "content": prompt,
+            }
+        ],
+        model=model,
+    )
+
+    response = chat_completion.choices[0].message.content
+    #    with Completion() as completion:
+    #        full_prompt = prompt + " " + requirements
+    #        response, id, stats = completion.send_prompt(model, user_prompt=full_prompt)
+
     return response
 
+
 def clean_requirements_octoai(requirements):
-    model = os.getenv('OCTOAI_MODEL', OCTOAI_MODEL)
-    prompt = os.getenv('CLEAN_REQUIREMENTS_SECRET_PROMPT', CLEAN_REQUIREMENTS_SECRET_PROMPT)
+    model = os.getenv("OCTOAI_MODEL", OCTOAI_MODEL)
+    prompt = os.getenv(
+        "CLEAN_REQUIREMENTS_SECRET_PROMPT", CLEAN_REQUIREMENTS_SECRET_PROMPT
+    )
     client = OctoAiClient()
 
     completion = client.chat.completions.create(
         messages=[
-                {
-                    "role": "system",
-                    "content": prompt
-                },
-                {
-                    "role": "user",
-                    "content": requirements
-                }
-            ],
+            {"role": "system", "content": prompt},
+            {"role": "user", "content": requirements},
+        ],
         model=model,
         max_tokens=20000,
         presence_penalty=0,
         temperature=0.1,
-        top_p=0.9)
+        top_p=0.9,
+    )
 
     requirements = completion.choices[0].message.content
 
     return requirements
 
+
 def save_requirements(requirements, ogre_dir_path):
-    requirements_fullpath = os.path.join(ogre_dir_path, 'requirements.txt')
-    with open(requirements_fullpath, 'w') as f:
+    requirements_fullpath = os.path.join(ogre_dir_path, "requirements.txt")
+    with open(requirements_fullpath, "w") as f:
         f.write(requirements)
-    return requirements_fullpath 
+    return requirements_fullpath
+
 
 def rewrite_readme(provider, readme):
     readme_emoji()
-    
-    if provider == 'openai':
+
+    if provider == "openai":
         res = rewrite_readme_openai(readme)
-    elif provider == 'ollama':
+    elif provider == "ollama":
         res = rewrite_readme_ollama(readme)
-    elif provider == 'octoai':
+    elif provider == "octoai":
         res = rewrite_readme_octoai(readme)
-    elif provider == 'groq':
+    elif provider == "groq":
         res = rewrite_readme_groq(readme)
-    elif provider == 'mistral':
+    elif provider == "mistral":
         res = rewrite_readme_mistral(readme)
     return res
 
+
 def rewrite_readme_openai(readme):
-    model = os.getenv('OPENAI_MODEL', OPENAI_MODEL)
-    prompt = os.getenv('REWRITE_README_PROMPT', REWRITE_README_PROMPT)
+    model = os.getenv("OPENAI_MODEL", OPENAI_MODEL)
+    prompt = os.getenv("REWRITE_README_PROMPT", REWRITE_README_PROMPT)
     client = OpenAI()
-    if 'OPENAI_API_KEY' not in os.environ:
+    if "OPENAI_API_KEY" not in os.environ:
         raise EnvironmentError("OPENAI_API_KEY environment variable not defined")
-    
+
     try:
         completion = client.chat.completions.create(
-                        model=model,
-                        messages=[
-                            {"role": "system", "content": prompt},
-                            {"role": "user", "content": readme}
-                        ]
-                    )
+            model=model,
+            messages=[
+                {"role": "system", "content": prompt},
+                {"role": "user", "content": readme},
+            ],
+        )
         # print(completion)
         new_readme = completion.choices[0].message.content
     except Exception as e:
         print(e)
 
     return new_readme
 
+
 def rewrite_readme_ollama(readme):
-    model = os.getenv('OLLAMA_MODEL', OLLAMA_MODEL)
-    prompt = os.getenv('REWRITE_README_PROMPT', REWRITE_README_PROMPT)
-    api_server = os.getenv('OLLAMA_API_SERVER', OLLAMA_API_SERVER)
+    model = os.getenv("OLLAMA_MODEL", OLLAMA_MODEL)
+    prompt = os.getenv("REWRITE_README_PROMPT", REWRITE_README_PROMPT)
+    api_server = os.getenv("OLLAMA_API_SERVER", OLLAMA_API_SERVER)
     # print(f"{api_server=} {model=} {prompt=}")
-    client = OpenAI(base_url=api_server, api_key='ollama')
+    client = OpenAI(base_url=api_server, api_key="ollama")
     completion = client.chat.completions.create(
-                  model=model,
-                  messages=[
-                      {"role": "system", "content": prompt},
-                      {"role": "user", "content": readme}
-                  ]
-              )
+        model=model,
+        messages=[
+            {"role": "system", "content": prompt},
+            {"role": "user", "content": readme},
+        ],
+    )
     new_readme = completion.choices[0].message.content
 
     return new_readme
 
+
 def rewrite_readme_octoai(readme):
     raise NotImplementedError("rewrite_readme_octoai is not implemented.")
 
+
 def rewrite_readme_groq(readme):
-    raise NotImplementedError("rewrite_readme_groq is not implemented.")
+    model = os.getenv("GROQ_MODEL", GROQ_MODEL)
+    prompt = os.getenv("REWRITE_README_PROMPT", REWRITE_README_PROMPT)
+
+    client = Groq(
+        api_key=os.environ.get("GROQ_API_KEY"),
+    )
+
+    chat_completion = client.chat.completions.create(
+        messages=[
+            {"role": "system", "content": prompt},
+            {"role": "user", "content": readme},
+        ],
+        model=model,
+    )
+
+    response = chat_completion.choices[0].message.content
+
+    return response
+
 
 def rewrite_readme_mistral(readme):
-    model = os.getenv('MISTRAL_MODEL', MISTRAL_MODEL)
-    prompt = os.getenv('REWRITE_README_PROMPT', REWRITE_README_PROMPT)
+    model = os.getenv("MISTRAL_MODEL", MISTRAL_MODEL)
+    prompt = os.getenv("REWRITE_README_PROMPT", REWRITE_README_PROMPT)
     api_key = os.environ["MISTRAL_API_KEY"]
     client = MistralClient(api_key=api_key)
-    content = prompt + '\n' + readme
+    content = prompt + "\n" + readme
     messages = [ChatMessage(role="user", content=content)]
-    
+
     # No streaming
     chat_response = client.chat(
         model=model,
         messages=messages,
     )
     new_readme = chat_response.choices[0].message.content
 
     return new_readme
 
+
 def save_readme(readme, ogre_dir_path):
-    readme_fullpath = os.path.join(ogre_dir_path, 'README.md')
-    with open(readme_fullpath, 'w') as f:
+    readme_fullpath = os.path.join(ogre_dir_path, "README.md")
+    with open(readme_fullpath, "w") as f:
         f.write(readme)
-    return readme_fullpath 
+    return readme_fullpath
+
 
-def build_docker_image(dockerfile, image_name, verbose = False):
+def build_docker_image(dockerfile, image_name, verbose=False, cache=False):
     # build docker image
-    
+
     platform_name = "linux/{}".format(platform.machine())
     image_name = "miniogre/{}:{}".format(image_name.lower(), "latest")
 
     build_emoji()
-    print("   platform = {}".format(platform_name)) 
+    print("   platform = {}".format(platform_name))
     print("   image name = {}".format(image_name))
-    
+
     if verbose:
         stderr = None
-        progress = 'plain'
+        progress = "plain"
     else:
         stderr = subprocess.PIPE
-        progress = 'auto'
+        progress = "auto"
 
-    build_cmd = (
-        "DOCKER_BUILDKIT=1 docker buildx build --no-cache --load --progress={} --platform {} -t {} -f {} .".format(
-            progress, platform_name, image_name, dockerfile
-        )
+    if cache:
+        cache_option = ""
+    else:
+        cache_option = "--no-cache"
+
+    build_cmd = "DOCKER_BUILDKIT=1 docker buildx build {} --load --progress={} --platform {} -t {} -f {} .".format(
+        cache_option, progress, platform_name, image_name, dockerfile
     )
     print("   build command = {}".format(build_cmd))
 
     if verbose:
-        p = subprocess.Popen(build_cmd, stdout=subprocess.PIPE, stderr=stderr, shell=True)
+        p = subprocess.Popen(
+            build_cmd, stdout=subprocess.PIPE, stderr=stderr, shell=True
+        )
         (out, err) = p.communicate()
         p_status = p.wait()
     else:
         with yaspin().aesthetic as sp:
-            sp.text = "generating ogre environment" 
-            p = subprocess.Popen(build_cmd, stdout=subprocess.PIPE, stderr=stderr, shell=True)
+            sp.text = "generating ogre environment"
+            p = subprocess.Popen(
+                build_cmd, stdout=subprocess.PIPE, stderr=stderr, shell=True
+            )
             (out, err) = p.communicate()
             p_status = p.wait()
     return out
 
-def spin_up_container(image_name, project_path, port):
+
+def spin_up_container(image_name, project_path, port_map):
     # spin up container
     spinup_emoji()
 
     project_name = image_name
     container_name = "miniogre-{}".format(image_name.lower())
     image_name = "miniogre/{}:{}".format(image_name.lower(), "latest")
-    #cmd = "uv venv; source .venv/bin/activate; cat ./{}/requirements.txt | xargs -L 1 uv pip install; exit 0;"
-    #cmd = "cat ./ogre_dir/requirements.txt | xargs -L 1 uv pip install; exit 0"
-    spin_up_cmd = (
-        "docker run -it --rm -v {}:/opt/{} -p {}:{} --name {} {}".format(project_path, project_name, port, port, container_name, image_name)  
+    # cmd = "uv venv; source .venv/bin/activate; cat ./{}/requirements.txt | xargs -L 1 uv pip install; exit 0;"
+    # cmd = "cat ./ogre_dir/requirements.txt | xargs -L 1 uv pip install; exit 0"
+    spin_up_cmd = "docker run -it --rm -v {}:/opt/{} -p {} --name {} {}".format(
+        project_path, project_name, port_map, container_name, image_name
     )
 
     print("   spin up command = {}".format(spin_up_cmd))
     subprocess.call(spin_up_cmd.split())
-    #p = subprocess.Popen(spin_up_cmd, stdout=subprocess.PIPE, shell=True)
-    #(out, err) = p.communicate()
-    #p_status = p.wait()
+    # p = subprocess.Popen(spin_up_cmd, stdout=subprocess.PIPE, shell=True)
+    # (out, err) = p.communicate()
+    # p_status = p.wait()
 
     return 0
 
-def create_sbom(image_name, project_path, format, verbose = False):
+
+def create_sbom(image_name, project_path, format, verbose=False):
     # Create SBOM from inside the container
-    print(emoji.emojize(':desktop_computer:  Generating SBOM...'))
+    print(emoji.emojize(":desktop_computer:  Generating SBOM..."))
 
     project_name = image_name
     container_name = "miniogre-{}".format(image_name.lower())
     image_name = "miniogre/{}:{}".format(image_name.lower(), "latest")
 
-    if format == 'cyclonedx':
+    if format == "cyclonedx":
         sbom_format_cmd = "cyclonedx-py requirements ./ogre_dir/requirements.txt &> ./ogre_dir/sbom.json"
-    elif format == 'pip-licenses':
+    elif format == "pip-licenses":
         sbom_format_cmd = "pip-licenses --with-authors --with-maintainers --with-urls --with-description -l --format json --output-file ./ogre_dir/sbom.json"
 
     # sbom_cmd = (
-    #     "   docker run -d --rm -v {}:/opt/{} --name {}_sbom {} bash -c '{}; wait'".format(project_path, project_name, container_name, image_name, sbom_format_cmd)  
+    #     "   docker run -d --rm -v {}:/opt/{} --name {}_sbom {} bash -c '{}; wait'".format(project_path, project_name, container_name, image_name, sbom_format_cmd)
     # )
     sbom_cmd = sbom_format_cmd
-    
+
     if verbose:
         stderr = None
         print(sbom_cmd)
     else:
         stderr = subprocess.PIPE
     p = subprocess.Popen(sbom_cmd, stdout=subprocess.PIPE, stderr=stderr, shell=True)
     p.communicate()
     p.wait()
 
     return 0
-    
+
+
 def display_figlet():
     # Display Ogre figlet
     f = Figlet(font="slant")
     # Get version
     # ogre_version = pkg_resources.get_distribution('miniogre').version
     rprint("[cyan] {} [/cyan]".format(f.renderText("miniogre")))
     rprint("[blue bold]miniogre - {}[/blue bold]".format("https://ogre.run"))
     print("\n")
 
+
 # def create_virtualenv(requirements, python_version):
-  
+
 #     env_name = 'miniogre-env'
 
 #     venv_cmd = "python -m venv {}".format(env_name)
-#     # venv_activate_cmd = 'source {}/bin/activate'.format(env_name) 
+#     # venv_activate_cmd = 'source {}/bin/activate'.format(env_name)
 
 #     #os.popen(venv_cmd)
 #     #os.popen(venv_activate_cmd)
 #     p = subprocess.Popen(venv_cmd, stdout=subprocess.PIPE, shell=True)
 #     (out, err) = p.communicate()
 #     p_status = p.wait()
 
@@ -553,34 +650,38 @@
 
 #     pip_cmd = '{}/bin/pip'.format(env_name)
 #     with open(requirements) as f:
 #         requirements_list = []
 #         for line in f:
 #             requirements_list.append(line.strip('\n'))
 
-#         pip_cmd = 'pip' 
+#         pip_cmd = 'pip'
 #         for req in requirements_list:
 #             print(req)
 #             input()
 #             subprocess.call([pip_cmd, 'install', req.strip()])
 
+
 def run_gptify(repo_path):
 
     generate_context_emoji()
-    
+
     if not os.path.exists("ogre_dir"):
         os.mkdir("ogre_dir")
 
     gptrepo_cmd = 'gptify {} --output "ogre_dir/gptify_output.txt"'.format(repo_path)
-    p = subprocess.Popen(gptrepo_cmd, stdout=subprocess.PIPE, stderr=subprocess.PIPE, shell=True)
+    p = subprocess.Popen(
+        gptrepo_cmd, stdout=subprocess.PIPE, stderr=subprocess.PIPE, shell=True
+    )
     (out, err) = p.communicate()
     p_status = p.wait()
 
-    with open('ogre_dir/gptify_output.txt', 'r') as f:
+    with open("ogre_dir/gptify_output.txt", "r") as f:
         return f.read()
 
+
 def cleanup():
     """
     Delete unnecessary files
     """
-    if os.path.exists('ogre_dir/gptify_output.txt'):
-        os.remove('ogre_dir/gptify_output.txt')
+    if os.path.exists("ogre_dir/gptify_output.txt"):
+        os.remove("ogre_dir/gptify_output.txt")
```

### Comparing `miniogre-0.5.0/miniogre/config.py` & `miniogre-0.6.0/miniogre/config.py`

 * *Files identical despite different names*

### Comparing `miniogre-0.5.0/miniogre/constants.py` & `miniogre-0.6.0/miniogre/constants.py`

 * *Files 16% similar despite different names*

```diff
@@ -68,136 +68,191 @@
 # echo -e "\e[m"
 
 # Aliases
 alias python="python3"
 """
 
 FILE_EXTENSIONS = {
-    'python': ['.py'],
-    'javascript': ['.js'],
-    'c++': ['.cpp', '.cxx', '.cc', '.c', '.hpp', '.hxx', '.hh', '.h'],
-    'java': ['.java'],
-    'c#': ['.cs'],
-    'ruby': ['.rb'],
-    'php': ['.php'],
-    'go': ['.go'],
-    'rust': ['.rs'],
-    'swift': ['.swift'],
-    'kotlin': ['.kt'],
-    'scala': ['.scala'],
-    'clojure': ['.clj'],
-    'haskell': ['.hs'],
-    'erlang': ['.erl'],
-    'elixir': ['.ex', '.exs'],
-    'lua': ['.lua'],
-    'perl': ['.pl'],
-    'r': ['.r'],
-    'julia': ['.jl'],
-    'dart': ['.dart'],
-    'typescript': ['.ts'],
-    'coffeescript': ['.coffee'],
-    'ocaml': ['.ml', '.mli'],
-    'f#': ['.fs', '.fsi', '.fsx'],
-    'scheme': ['.scm', '.ss'],
-    'common lisp': ['.lisp', '.lsp'],
-    'racket': ['.rkt'],
-    'nim': ['.nim'],
-    'crystal': ['.cr'],
-    'groovy': ['.groovy'],
-    'd': ['.d'],
-    'fortran': ['.f', '.f90', '.f95'],
-    'cobol': ['.cbl', '.cob', '.cpy'],
-    'jupyter': ['.ipynb']
+    "python": [".py"],
+    "javascript": [".js"],
+    "c++": [".cpp", ".cxx", ".cc", ".c", ".hpp", ".hxx", ".hh", ".h"],
+    "java": [".java"],
+    "c#": [".cs"],
+    "ruby": [".rb"],
+    "php": [".php"],
+    "go": [".go"],
+    "rust": [".rs"],
+    "swift": [".swift"],
+    "kotlin": [".kt"],
+    "scala": [".scala"],
+    "clojure": [".clj"],
+    "haskell": [".hs"],
+    "erlang": [".erl"],
+    "elixir": [".ex", ".exs"],
+    "lua": [".lua"],
+    "perl": [".pl"],
+    "r": [".r"],
+    "julia": [".jl"],
+    "dart": [".dart"],
+    "typescript": [".ts"],
+    "coffeescript": [".coffee"],
+    "ocaml": [".ml", ".mli"],
+    "f#": [".fs", ".fsi", ".fsx"],
+    "scheme": [".scm", ".ss"],
+    "common lisp": [".lisp", ".lsp"],
+    "racket": [".rkt"],
+    "nim": [".nim"],
+    "crystal": [".cr"],
+    "groovy": [".groovy"],
+    "d": [".d"],
+    "fortran": [".f", ".f90", ".f95"],
+    "cobol": [".cbl", ".cob", ".cpy"],
+    "jupyter": [".ipynb"],
 }
 
-ALL_EXTENSIONS = ['.py', '.js', '.cpp', '.cxx', '.cc', '.c', '.hpp', '.hxx', '.hh', '.h', '.java', '.cs', '.rb', '.php', '.go', '.rs', '.swift', '.kt', '.scala', '.clj', '.hs', '.erl', '.ex', '.exs', '.lua', '.pl', '.r', '.jl', '.dart', '.ts', '.coffee', '.ml', '.mli', '.fs', '.fsi', '.fsx', '.scm', '.ss', '.lisp', '.lsp', '.rkt', '.nim', '.cr', '.groovy', '.d', '.f', '.f90', '.f95', '.cbl', '.cob', '.cpy', '.ipynb']
+ALL_EXTENSIONS = [
+    ".py",
+    ".js",
+    ".cpp",
+    ".cxx",
+    ".cc",
+    ".c",
+    ".hpp",
+    ".hxx",
+    ".hh",
+    ".h",
+    ".java",
+    ".cs",
+    ".rb",
+    ".php",
+    ".go",
+    ".rs",
+    ".swift",
+    ".kt",
+    ".scala",
+    ".clj",
+    ".hs",
+    ".erl",
+    ".ex",
+    ".exs",
+    ".lua",
+    ".pl",
+    ".r",
+    ".jl",
+    ".dart",
+    ".ts",
+    ".coffee",
+    ".ml",
+    ".mli",
+    ".fs",
+    ".fsi",
+    ".fsx",
+    ".scm",
+    ".ss",
+    ".lisp",
+    ".lsp",
+    ".rkt",
+    ".nim",
+    ".cr",
+    ".groovy",
+    ".d",
+    ".f",
+    ".f90",
+    ".f95",
+    ".cbl",
+    ".cob",
+    ".cpy",
+    ".ipynb",
+]
 
-OGRE_DIR = 'ogre_dir'
-OGRE_BASEIMAGE = 'ogrerun/base:ubuntu22.04-{}'
+OGRE_DIR = "ogre_dir"
+OGRE_BASEIMAGE = "ogrerun/base:ubuntu22.04-{}"
 
-OPENAI_MODEL = 'gpt-4-turbo-preview'
-OPENAI_SECRET_PROMPT = '''You are a Python requirements generator.
+OPENAI_MODEL = "gpt-4-turbo"
+OPENAI_SECRET_PROMPT = """You are a Python requirements generator.
 You should generate the contents of a Python requirements file (raw text only) taking into account the text sent by the user.
 The raw text sent by the user consists of a combination of the README file contents and the source code contents.
 You generate only the file contents as answer.
 If the text sent by the user is invalid or is empty, just generate an empty content.
 You should ignore the Python version 2 or 3.
 The python package should not be included in the requirements file.
 Note that some packages do not exist in the PyPi repository, they are only local, and thus shouldnt be added to the requirements.txt file.
 Ignore the following Python packages: git, jittor, cuda, shihong, nvdiffrast: they do not exist on the PyPi repository.
-Your output should be a raw ASCII text file.'''
+Your output should be a raw ASCII text file."""
 
-OLLAMA_MODEL = 'mistral:7b'
-OLLAMA_API_SERVER = 'http://localhost:11434/v1'
+# OLLAMA_MODEL = "mistral:7b"
+OLLAMA_MODEL = "phi3"
+OLLAMA_API_SERVER = "http://localhost:11434/v1"
 # OLLAMA_SECRET_PROMPT = '''You are a Python requirements generator.
 # You should generate the contents of a Python requirements file (raw text only) taking into account the text sent by the user.
 # The raw text sent by the user consists of a combination of the README file contents and the source code contents.
 # You generate only the file contents as answer.
 # If the text sent by the user is invalid or is empty, just generate an empty content.
 # You should ignore the Python version 2 or 3.
 # The python package should not be included in the requirements file.
 # Note that some packages do not exist in the PyPi repository, they are only local, and thus shouldnt be added to the requirements.txt file.
 # Ignore the following Python packages: git, jittor, cuda, shihong, nvdiffrast: they do not exist on the PyPi repository.
 # Your output should be a raw ASCII text file.'''
 
-OCTOAI_MODEL = 'mistral-7b-instruct-fp16'
-OCTOAI_SECRET_PROMPT = '''You are a Python requirements generator.
+OCTOAI_MODEL = "mistral-7b-instruct-fp16"
+OCTOAI_SECRET_PROMPT = """You are a Python requirements generator.
 You should generate the contents of a Python requirements file (raw text only) taking into account the text sent by the user.
 The raw text sent by the user consists of a combination of the README file contents and the source code contents.
 If the text sent by the user is invalid or is empty, just generate an empty content.
 You should ignore the Python version 2 or 3.
 The python package should not be included in the requirements file.
 Some packages do not exist in the PyPi repository, they are only local, and thus shouldnt be added to the requirements.txt file.
 Ignore the following Python packages: git, jittor, cuda, shihong, nvdiffrast: they do not exist on the PyPi repository.
 Your output should be a raw ASCII text file.
 Do not return parts of the text sent by the user. We just want the requirements list.
-Only return the list of requirements. No other text like the filename at the top of the response or symbols are allowed.'''
+Only return the list of requirements. No other text like the filename at the top of the response or symbols are allowed."""
 
-REWRITE_README_PROMPT = '''You are a specialist in understanding and explaining source code. 
+REWRITE_README_PROMPT = """You are a specialist in understanding and explaining source code. 
 You are also a specialist in writing clear documentation (e.g README files) that helps people to understand the source code.
 Your task is to take a text input containing the current README and the code and use it to write an updated version of the README file.
-The README file should highlight the actual requirements that need to be installed.'''
+The README file should highlight the actual requirements that need to be installed."""
 
-GROQ_MODEL = 'mixtral-8x7b-32768'
-GROQ_SECRET_PROMPT = '''You are a Python requirements generator.
+#GROQ_MODEL = "mixtral-8x7b-32768"
+GROQ_MODEL = "llama3-70b-8192"
+GROQ_SECRET_PROMPT = """You are a Python requirements generator.
 You should generate the contents of a Python requirements file (raw text only) taking into account the text sent by the user.
 The raw text sent by the user consists of a combination of the README file contents and the source code contents.
 If the text sent by the user is invalid or is empty, just generate an empty content.
 You should ignore the Python version 2 or 3.
 The python package should not be included in the requirements file.
 Some packages do not exist in the PyPi repository, they are only local, and thus shouldnt be added to the requirements.txt file.
 Ignore the following Python packages: git, jittor, cuda, shihong, nvdiffrast: they do not exist on the PyPi repository.
 Your output should be a raw ASCII text file containg only the list of requirements. Do not return sentences. 
-Do not return parts of the text sent by the user. We just want the requirements list.'''
+Do not return parts of the text sent by the user. We just want the requirements list."""
 
-MISTRAL_MODEL = 'mistral-large-latest'
+MISTRAL_MODEL = "mistral-large-latest"
 # MISTRAL_SECRET_PROMPT = '''You are a Python requirements generator.
 # You should generate the contents of a Python requirements file (raw text only) taking into account the text sent by the user.
 # The raw text sent by the user consists of a combination of the README file contents and the source code contents.
 # You generate only the file contents as answer.
 # If the text sent by the user is invalid or is empty, just generate an empty content.
 # You should ignore the Python version 2 or 3.
 # The python package should not be included in the requirements file.
 # Note that some packages do not exist in the PyPi repository, they are only local, and thus shouldnt be added to the requirements.txt file.
 # Ignore the following Python packages: git, jittor, cuda, shihong, nvdiffrast: they do not exist on the PyPi repository.
 # Your output should be a raw ASCII text file.'''
 
-CLEAN_REQUIREMENTS_SECRET_PROMPT='''Here is the content of a requirements.txt file. 
+CLEAN_REQUIREMENTS_SECRET_PROMPT = """Here is the content of a requirements.txt file. 
 It is a list of Python libraries to be installed in the a Python environment. 
 Not all entries in the list are actual Python libraries available on the PyPi repository. 
 Identify those that arent available on PyPi and remove them from the list.
 Get the remaining entries (those that are available on PypI) and generate an updated list of requirements.
 If any of the packages in the updated list is represented by a name under which it can not be found on PyPi, change the name to the one that is available on PyPi.
 For example, the library `PIL` is not available under that name in PyPi, but `Pillow` is.
 Do not explain how the new list is generated. Do not provide any context related to how you proceeded.
 Your response must contain only the list of packages to be installed.
-Remove any blank lines.'''
+Remove any blank lines."""
 
-GROQ_CLEAN_REQUIREMENTS_SECRET_PROMPT='''Here is the content of a requirements.txt file. 
+GROQ_CLEAN_REQUIREMENTS_SECRET_PROMPT = """Here is the content of a requirements.txt file. 
 It is a list of Python libraries to be installed in the a Python environment. 
 Not all entries in the list are actual Python libraries available on the PyPi repository. 
 Identify those that arent available on PyPi and remove them from the list.
 Get the remaining entries (those that are available on PypI) and generate an updated list of requirements.
 If any of the packages in the updated list is represented by a name under which it can not be found on PyPi, change the name to the one that is available on PyPi.
 For example, the library `PIL` is not available under that name in PyPi, but `Pillow` is.
 No explanation notes on your reasoning are allowed. Nobody wants to know which packages were removed. Your response must contain only the list of packages to be installed.
-Remove any blank lines.'''
+Remove any blank lines."""
```

### Comparing `miniogre-0.5.0/miniogre/main.py` & `miniogre-0.6.0/miniogre/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,52 +9,58 @@
 from .config import *
 
 app = typer.Typer()
 load_dotenv()
 
 project_path = os.getcwd()
 
+
 @app.command()
 def version():
     """
     Display version
     """
-    version_string = importlib.metadata.version('miniogre')
+    version_string = importlib.metadata.version("miniogre")
     print("{}".format(version_string))
 
     return 0
 
+
 @app.command()
 def readme(provider: str = "openai"):
     """
     Rewrite readme
     """
 
     display_figlet()
     starting_emoji()
 
-    ogre_dir_path = config_ogre_dir(os.path.join(project_path, os.getenv("OGRE_DIR", OGRE_DIR)))
+    ogre_dir_path = config_ogre_dir(
+        os.path.join(project_path, os.getenv("OGRE_DIR", OGRE_DIR))
+    )
     context_contents = run_gptify(os.getcwd())
     new_readme = rewrite_readme(provider, context_contents)
     readme_path = save_readme(new_readme, ogre_dir_path)
     end_emoji()
 
     return 0
 
+
 @app.command()
 def run(
     provider: str = "openai",
     baseimage: str = "auto",
-    port: str = "8001",
+    port_map: str = "8001:8001",
     dry: bool = False,
     force_requirements_generation: bool = True,
     sbom_format: str = "pip-licenses",
     no_container: bool = False,
     verbose: bool = False,
-    with_readme: bool = False
+    cache: bool = False,
+    with_readme: bool = False,
 ):
     """
     Run full miniogre pipeline
     """
 
     display_figlet()
     starting_emoji()
@@ -64,28 +70,50 @@
 
     project_name = os.path.basename(project_path)
 
     files = list_files(project_path)
     extensions = get_extensions(files)
     counts = count_extensions(extensions)
     most_ext = determine_most_ext(counts)
-    ogre_dir_path = config_ogre_dir(os.path.join(project_path, os.getenv("OGRE_DIR", OGRE_DIR)))
+    ogre_dir_path = config_ogre_dir(
+        os.path.join(project_path, os.getenv("OGRE_DIR", OGRE_DIR))
+    )
     if with_readme:
         context_contents = run_gptify(os.getcwd())
         new_readme = rewrite_readme(provider, context_contents)
         readme_path = save_readme(new_readme, ogre_dir_path)
-    generate_requirements = config_requirements(project_path, ogre_dir_path, force_requirements_generation)
-    local_requirements = extract_requirements_from_code(project_path, most_ext, generate_requirements)
+    generate_requirements = config_requirements(
+        project_path, ogre_dir_path, force_requirements_generation
+    )
+    local_requirements = extract_requirements_from_code(
+        project_path, most_ext, generate_requirements
+    )
     final_requirements = clean_requirements(provider, local_requirements)
     requirements_fullpath = save_requirements(final_requirements, ogre_dir_path)
     config_bashrc(project_path, ogre_dir_path, None, None, None)
     config_dockerfile(project_path, project_name, ogre_dir_path, baseimage, dry)
     create_sbom(project_name, project_path, sbom_format, verbose)
     if no_container == False:
         build_docker_image(
-            os.path.join(ogre_dir_path, "Dockerfile"), project_name, verbose
+            os.path.join(ogre_dir_path, "Dockerfile"), project_name, verbose, cache
         )
-        spin_up_container(project_name, project_path, port)
+        spin_up_container(project_name, project_path, port_map)
+    end_emoji()
+
+
+@app.command()
+def spinup(port_map: str = "8001:8001"):
+    """
+    Spin up container if image was previously built with `run`
+    """
+
+    display_figlet()
+    starting_emoji()
+
+    project_name = os.path.basename(project_path)
+    spin_up_container(project_name, project_path, port_map)
+
     end_emoji()
 
+
 if __name__ == "__main__":
     app()
```

### Comparing `miniogre-0.5.0/pyproject.toml` & `miniogre-0.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "miniogre"
-version = "0.5.0"
+version = "0.6.0"
 description = "miniogre: from source code to reproducible environment, in seconds."
 readme = "README.md"
 authors = ["Wilder Lopes <wilder@ogre.run>"]
 include = [".env"]
 homepage = "https://github.com/ogre-run/miniogre"
 
 [tool.poetry.dependencies]
@@ -12,15 +12,15 @@
 typer = "0.9.0"
 docker = "^5.0.0"
 python-dotenv = "^0.19.0"
 openai = "1.21.2"
 emoji = "^2.10.1"
 pyfiglet = "^1.0.2"
 rich = "^13.7.0"
-groq = "^0.3.0"
+groq = "0.5.0"
 yaspin = "^3.0.1"
 octoai-sdk = "^0.9.0"
 mistralai = "^0.1.3"
 autopep8 = "^2.0.4"
 cyclonedx-py = "^1.0.1"
 pip-licenses = "^4.3.4"
 gptify = "0.3.2"
```

### Comparing `miniogre-0.5.0/PKG-INFO` & `miniogre-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: miniogre
-Version: 0.5.0
+Version: 0.6.0
 Summary: miniogre: from source code to reproducible environment, in seconds.
 Home-page: https://github.com/ogre-run/miniogre
 Author: Wilder Lopes
 Author-email: wilder@ogre.run
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: autopep8 (>=2.0.4,<3.0.0)
 Requires-Dist: cyclonedx-py (>=1.0.1,<2.0.0)
 Requires-Dist: docker (>=5.0.0,<6.0.0)
 Requires-Dist: emoji (>=2.10.1,<3.0.0)
 Requires-Dist: gptify (==0.3.2)
-Requires-Dist: groq (>=0.3.0,<0.4.0)
+Requires-Dist: groq (==0.5.0)
 Requires-Dist: mistralai (>=0.1.3,<0.2.0)
 Requires-Dist: octoai-sdk (>=0.9.0,<0.10.0)
 Requires-Dist: openai (==1.21.2)
 Requires-Dist: pip-licenses (>=4.3.4,<5.0.0)
 Requires-Dist: pyfiglet (>=1.0.2,<2.0.0)
 Requires-Dist: python-dotenv (>=0.19.0,<0.20.0)
 Requires-Dist: rich (>=13.7.0,<14.0.0)
```

