# Comparing `tmp/lusid_express-1.0.9.tar.gz` & `tmp/lusid_express-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lusid_express-1.0.9.tar", last modified: Sat Apr 27 22:22:16 2024, max compression
+gzip compressed data, was "lusid_express-1.1.2.tar", last modified: Wed May  8 12:56:33 2024, max compression
```

## Comparing `lusid_express-1.0.9.tar` & `lusid_express-1.1.2.tar`

### file list

```diff
@@ -1,25 +1,27 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 22:22:16.803777 lusid_express-1.0.9/
--rw-rw-rw-   0 root         (0) root         (0)     1062 2024-04-27 22:21:34.000000 lusid_express-1.0.9/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       85 2024-04-27 22:21:34.000000 lusid_express-1.0.9/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     6659 2024-04-27 22:22:16.803777 lusid_express-1.0.9/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     6019 2024-04-27 22:21:34.000000 lusid_express-1.0.9/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-27 22:22:16.803777 lusid_express-1.0.9/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1536 2024-04-27 22:21:34.000000 lusid_express-1.0.9/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 22:22:16.797777 lusid_express-1.0.9/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 22:22:16.799777 lusid_express-1.0.9/src/lusid_express/
--rw-rw-rw-   0 root         (0) root         (0)       30 2024-04-27 22:21:34.000000 lusid_express-1.0.9/src/lusid_express/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5616 2024-04-27 22:21:34.000000 lusid_express-1.0.9/src/lusid_express/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 22:22:16.800777 lusid_express-1.0.9/src/lusid_express/apis/
--rw-rw-rw-   0 root         (0) root         (0)  2240138 2024-04-27 22:22:16.000000 lusid_express-1.0.9/src/lusid_express/apis/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 22:22:16.802777 lusid_express-1.0.9/src/lusid_express/config/
--rw-rw-rw-   0 root         (0) root         (0)      369 2024-04-27 22:21:34.000000 lusid_express-1.0.9/src/lusid_express/config/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 22:22:16.803777 lusid_express-1.0.9/src/lusid_express/display/
--rw-rw-rw-   0 root         (0) root         (0)      518 2024-04-27 22:21:34.000000 lusid_express-1.0.9/src/lusid_express/display/PRELOADED_VARS.md
--rw-rw-rw-   0 root         (0) root         (0)    11383 2024-04-27 22:21:34.000000 lusid_express-1.0.9/src/lusid_express/display/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2352 2024-04-27 22:21:34.000000 lusid_express-1.0.9/src/lusid_express/load.le
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 22:22:16.800777 lusid_express-1.0.9/src/lusid_express.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6659 2024-04-27 22:22:16.000000 lusid_express-1.0.9/src/lusid_express.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      482 2024-04-27 22:22:16.000000 lusid_express-1.0.9/src/lusid_express.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-27 22:22:16.000000 lusid_express-1.0.9/src/lusid_express.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      479 2024-04-27 22:22:16.000000 lusid_express-1.0.9/src/lusid_express.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2024-04-27 22:22:16.000000 lusid_express-1.0.9/src/lusid_express.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 12:56:33.276624 lusid_express-1.1.2/
+-rw-rw-rw-   0 root         (0) root         (0)     1062 2024-05-08 12:55:44.000000 lusid_express-1.1.2/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       85 2024-05-08 12:55:44.000000 lusid_express-1.1.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     8202 2024-05-08 12:56:33.276624 lusid_express-1.1.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     7562 2024-05-08 12:55:44.000000 lusid_express-1.1.2/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-08 12:56:33.276624 lusid_express-1.1.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1536 2024-05-08 12:55:44.000000 lusid_express-1.1.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 12:56:33.270624 lusid_express-1.1.2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 12:56:33.272624 lusid_express-1.1.2/src/lusid_express/
+-rw-rw-rw-   0 root         (0) root         (0)       46 2024-05-08 12:55:44.000000 lusid_express-1.1.2/src/lusid_express/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5913 2024-05-08 12:55:44.000000 lusid_express-1.1.2/src/lusid_express/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 12:56:33.273624 lusid_express-1.1.2/src/lusid_express/apis/
+-rw-rw-rw-   0 root         (0) root         (0)  2240138 2024-05-08 12:56:32.000000 lusid_express-1.1.2/src/lusid_express/apis/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 12:56:33.275624 lusid_express-1.1.2/src/lusid_express/config/
+-rw-rw-rw-   0 root         (0) root         (0)      369 2024-05-08 12:55:44.000000 lusid_express-1.1.2/src/lusid_express/config/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 12:56:33.275624 lusid_express-1.1.2/src/lusid_express/display/
+-rw-rw-rw-   0 root         (0) root         (0)      518 2024-05-08 12:55:44.000000 lusid_express-1.1.2/src/lusid_express/display/PRELOADED_VARS.md
+-rw-rw-rw-   0 root         (0) root         (0)    11360 2024-05-08 12:55:44.000000 lusid_express-1.1.2/src/lusid_express/display/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3156 2024-05-08 12:55:44.000000 lusid_express-1.1.2/src/lusid_express/load.le
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 12:56:33.275624 lusid_express-1.1.2/src/lusid_express/utils/
+-rw-rw-rw-   0 root         (0) root         (0)     2172 2024-05-08 12:55:44.000000 lusid_express-1.1.2/src/lusid_express/utils/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 12:56:33.273624 lusid_express-1.1.2/src/lusid_express.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8202 2024-05-08 12:56:33.000000 lusid_express-1.1.2/src/lusid_express.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      518 2024-05-08 12:56:33.000000 lusid_express-1.1.2/src/lusid_express.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-08 12:56:33.000000 lusid_express-1.1.2/src/lusid_express.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      479 2024-05-08 12:56:33.000000 lusid_express-1.1.2/src/lusid_express.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2024-05-08 12:56:33.000000 lusid_express-1.1.2/src/lusid_express.egg-info/top_level.txt
```

### Comparing `lusid_express-1.0.9/LICENSE` & `lusid_express-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lusid_express-1.0.9/PKG-INFO` & `lusid_express-1.1.2/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,59 +1,47 @@
-Metadata-Version: 2.1
-Name: lusid_express
-Version: 1.0.9
-Summary: lusid-express is a python package that makes it quick and easy to get started using Lusid and Luminesce.
-Home-page: https://gitlab.com/orlando.calvo1/lusid-express
-Author: Orlando Calvo
-Author-email: orlando.calvo@finbourne.com
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
 
-
-# lusid-express
-##### *`lusid-express` is a python package that makes it quick and easy to get started using Lusid and Luminesce.*
+# 1. lusid-express
+##### 1.0.0.0.1. *`lusid-express` is a python package that makes it quick and easy to get started using Lusid and Luminesce.*
 
 
 
 <!-- vscode-markdown-toc -->
 * 1. [Getting Started](#GettingStarted)
 	* 1.1. [Requirements](#Requirements)
 		* 1.1.1. [Environmental Variable setup](#EnvironmentalVariablesetup)
 	* 1.2. [Installation](#Installation)
 * 2. [Convenience package installations](#Conveniencepackageinstallations)
 * 3. [Luminesce Magic Command](#LuminesceMagicCommand)
 	* 3.1. [Why use this?](#Whyusethis)
 * 4. [Pre-loaded Variables](#Pre-loadedVariables)
+* 5. [Formatting](#Formatting)
+	* 5.1. [Lusid Objects](#LusidObjects)
+	* 5.2. [Copy to Clipboard](#CopytoClipboard)
 
 <!-- vscode-markdown-toc-config
 	numbering=true
 	autoSave=true
 	/vscode-markdown-toc-config -->
 <!-- /vscode-markdown-toc -->
 
 
+
+
 This repository holds the source code for lusid-express, a python package that makes it quick and easy to get started using Lusid and Luminesce. The package provides convenience in 3 distinct ways.
 
 1. Ease of installation of finbourne packages.
 2.  `%%luminesce` cell magic in your local jupyter installation.
 3.  Preset variables that make it possible to ommit boiler plate code.
 
 ##  1. <a name='GettingStarted'></a>Getting Started
 ###  1.1. <a name='Requirements'></a>Requirements
 In order to authenticate the lusid api clients you will need to have generated a secrets file. furthermore, you will need to have an environmental variable named `FBN_SECRETS_PATH` set to the full path to your secrets file. 
 
 ####  1.1.1. <a name='EnvironmentalVariablesetup'></a>Environmental Variable setup
-##### Mac OS
+##### 1.1.1.1.1. Mac OS
 Assuming `~/.secret/secrets.json` exists
 ```bash
 echo 'export FBN_SECRETS_PATH="~/.secret/secrets.json"' >> ~/.zshrc
 ```
 
 
 NOTE: Your secrets file needs to include the lumi api url under the key: `lumiApiUrl`. This url usually takes the form `https://{your-domain}.lusid.com/honeycomb`.
@@ -106,16 +94,21 @@
     lusidtools["lusidtools==1.0.14"]
     dve_lumipy_preview["dve-lumipy-preview==0.1.1075"]
 
 ```
 
 
 ##  3. <a name='LuminesceMagicCommand'></a>Luminesce Magic Command
+
+```bash
+python -m lusid_express -e magic
+```
+
 ###  3.1. <a name='Whyusethis'></a>Why use this?
-The main motivation to use this cell magic is to enable the use of `SQL` jupyter cells. That is, rather than display a cell on a notebook that holds an SQL string such as:
+The main motivation to use this cell magic is to enable SQL syntax highlighting through the use of SQL jupyter cells. That is, rather than display a cell on a notebook that holds an SQL string such as:
 ```python
 sql_string = """
 @raw_equities =
 SELECT *,
     'training' as Scope,
     Currency as domCcy,
     Ticker as DisplayName
@@ -148,18 +141,33 @@
 WHERE toWrite = @raw_equities;
 ```
 VSCode allows the SQL auto-formatting of Jupyter cells. This query runs when the cell is excecuted.
 
 
 
 ##  4. <a name='Pre-loadedVariables'></a>Pre-loaded Variables
+```bash
+python -m lusid_express -e vars
+```
 Enabling this feature provides the convenience of automatically loading important variables into python notebooks. This allows us to omit boler-plate code from each notebook. It also allows for reduce complexity as token management, authentication, and api client instantiations have all been abstracted away.
 
 | Variable Name | Statement         | Description                          |
 |---------------|-------------------|--------------------------------------|
 | lu          | `import lusid as lu` | Main LUSID package                   |
 | lm          | `import lusid.models as lm` | LUSID models module                  |
 | apis         | `import lusid_express.apis as apis` | convenience package providing pre-authenticated api access.                 |
 
 
+##  5. <a name='Formatting'></a>Formatting
+
+```bash
+python -m lusid_express -e format
+```
+When enabled, `format` overrides default rendering of certain types of objects.
+
+###  5.1. <a name='LusidObjects'></a>Lusid Objects
+Lusid Objects are rendered as tables, displaying the object type as the table's title, and its properties in the table's rows
 
+<h4>Equity</h4> <table id='DATA_TABLE-f8224859-f897-42c9-ae2a-df56f52dda23'><tr><th>Property</th><th>Value</th></tr><tr><td class='indent-0 '><strong>identifiers</strong></td><td></td></tr><tr><td class='indent-1 muted-text'>&nbsp;&nbsp;&nbsp;&nbsp;<strong>isin</strong></td><td class='muted-text'>US0378331005</td></tr><tr><td class='indent-1 muted-text'>&nbsp;&nbsp;&nbsp;&nbsp;<strong>figi</strong></td><td class='muted-text'>BBG000B9XVV8</td></tr><tr><td class='indent-1 muted-text'>&nbsp;&nbsp;&nbsp;&nbsp;<strong>ticker</strong></td><td class='muted-text'>AAPL</td></tr><tr><td class='indent-0 '><strong>dom_ccy</strong></td><td class=''>USD</td></tr><tr><td class='indent-0 '><strong>instrument_type</strong></td><td class=''>Equity</td></tr></table> 
 
+###  5.2. <a name='CopytoClipboard'></a>Copy to Clipboard
+With every table or Pandas DataFrame a `Copy to Clipboard` button is available for excel friendly copy/pasting.
```

### Comparing `lusid_express-1.0.9/setup.py` & `lusid_express-1.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 # List of requirements
 requirements = [
     'pyyaml',
 'luminesce-sdk-preview==1.14.758',
 'lusid-jam==0.1.2',
-'lusid-sdk-preview==1.1.120',
+'lusid-sdk-preview==1.1.220',
 'fbnlab-preview==0.1.108',
 'finbourne-access-sdk==0.0.3751',
 'finbourne-identity-sdk==0.0.2834',
 'finbourne-insights-sdk-preview==0.0.763',
 'finbourne-sdk-utilities==0.0.10',
 'lusid-configuration-sdk-preview==0.1.514',
 'lusid-drive-sdk-preview==0.1.617',
@@ -23,15 +23,15 @@
 ]
 
 
 
 
 setup(
     name='lusid_express',
-    version='1.0.9',
+    version='1.1.2',
     package_dir={'': 'src'},  # tells setuptools that packages are under src
     packages=find_packages(where='src'),  # tells setuptools to look for packages in src
     install_requires=requirements,
     description='lusid-express is a python package that makes it quick and easy to get started using Lusid and Luminesce.',
     long_description=open('README.md').read(),
     include_package_data=True,  
     long_description_content_type='text/markdown',
```

### Comparing `lusid_express-1.0.9/src/lusid_express/__main__.py` & `lusid_express-1.1.2/src/lusid_express/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,14 +32,23 @@
     new_content = [
         "'if \"apis\" in globals():',",
         "'    apis = apis',",
         "'if \"lm\" in globals():',",
         "'    lm = lm',",
         "'if \"lu\" in globals():',",
         "'    lu = lu',",
+        "'if \"lumi\" in globals():',",
+        # "'    from lumipy.client import Client as __Client',",
+        # "'    lumi = __Client(api_secrets_filename=__os.environ.get('FBN_SECRETS_PATH', None))',",
+        "'    lumi = lumi',",        
+        
+        
+        
+                
+        
     ]
 
 
     
     config_content = []
     if os.path.exists(ipython_config_path):
         with open(ipython_config_path, 'r') as file:
```

### Comparing `lusid_express-1.0.9/src/lusid_express/apis/__init__.py` & `lusid_express-1.1.2/src/lusid_express/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `lusid_express-1.0.9/src/lusid_express/display/PRELOADED_VARS.md` & `lusid_express-1.1.2/src/lusid_express/display/PRELOADED_VARS.md`

 * *Files identical despite different names*

### Comparing `lusid_express-1.0.9/src/lusid_express/display/__init__.py` & `lusid_express-1.1.2/src/lusid_express/display/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -312,15 +312,14 @@
     table = ""
     for key, value in data.items():
         table += get_rows(key, value)
 
     # Ensure the table ID is correctly set and used in the COPY_SCRIPT
     table_id = f"DATA_TABLE-{__uuid.uuid4()}"  # Unique ID for each table instance
     html_output = f"""<h1>{title}</h1> <table id='{table_id}'><tr><th>{col_name_key}</th><th>{col_name_value}</th></tr>{table}</table>{COPY_SCRIPT.replace('REPLACEMENT_HOOK', table_id)}"""
-    print(html_output)
     return html_output
 
 def render_table(data, col_name_key="Key", col_name_value="Value", title="table"):
     """
     Renders table from data.
 
     Parameters:
```

### Comparing `lusid_express-1.0.9/src/lusid_express/load.le` & `lusid_express-1.1.2/src/lusid_express/load.le`

 * *Files 25% similar despite different names*

```diff
@@ -1,37 +1,66 @@
 from typing import Dict, List
+import uuid
+import os as __os
 
+def load_environment(FBN_SECRETS_PATH:str):
+    """_summary_
 
-def initialize_ipython(config:Dict[str,List[str]]):
+    Args:
+        FBN_SECRETS_PATH (str): _description_
+    """
+    __os.environ['FBN_SECRETS_PATH'] =  FBN_SECRETS_PATH
+    D = __os.environ.get('FBN_SECRETS_PATH')
+    from IPython import get_ipython
+    ipython = get_ipython()
+    
+    # Perform imports and assign them to variables
+    import lusid as lu
+    import lusid.models as lm
+    import lusid_express.apis as apis
+    from lumipy.client import Client as __Client
+    
+    
+    lumi = __Client(api_secrets_filename=__os.environ.get('FBN_SECRETS_PATH'))
+    
+
+
+    # Assign the modules to the IPython user namespace
+    ipython.user_ns['lu'] = lu
+    ipython.user_ns['lm'] = lm
+    ipython.user_ns['apis'] = apis
+    ipython.user_ns['lumi'] = lumi
+
+    
+
+
+def __initialize_ipython(config:Dict[str,List[str]]):
+    
     
     features = config.get('features', [])
     do_vars = 'vars' in features
     do_magic = 'magic' in features
     do_format = 'format' in features
     if do_vars:
-        from IPython import get_ipython
-        ipython = get_ipython()
-        
-        # Perform imports and assign them to variables
-        import lusid as lu
-        import lusid.models as lm
-        import lusid_express.apis as apis
-
-        # Assign the modules to the IPython user namespace
-        ipython.user_ns['lu'] = lu
-        ipython.user_ns['lm'] = lm
-        ipython.user_ns['apis'] = apis
+        load_environment(__os.environ.get('FBN_SECRETS_PATH','~/.secret/secrets.json'))
+
     if do_magic:
         from IPython.core.magic import register_line_cell_magic
         import os
         from lumipy.client import Client
+        
         @register_line_cell_magic
         def luminesce(line, cell=None):
+            ipython = get_ipython()
             query = cell if cell is not None else line
             lm_client = Client(api_secrets_filename=os.environ.get('FBN_SECRETS_PATH',None))
+            # Using the user's namespace to replace variables in the query
+            user_ns = ipython.user_ns
+            query = query.format(**user_ns)
+            
             df = lm_client.query_and_fetch(query)
             return df
 
         def load_ipython_extension(ipython):
             ipython.register_magic_function(luminesce, 'line_cell', 'luminesce')
 
         del luminesce
@@ -46,26 +75,27 @@
                 try:
                     return render_table(x)
                 except Exception as e:
                     return None
             return None
         ipython.display_formatter.formatters['text/html'].for_type(object,safe_render_html)
         def custom_dataframe_display(df):
+            table_id = f"DATA_TABLE-{uuid.uuid4()}"
             # Combine the CSS, HTML table, JavaScript, and button
-            full_html = f"{STYLES['table']}\n{df.to_html(index=False, border=0, table_id='table')}\n{COPY_SCRIPT}"
+            full_html = f"{STYLES['table']}\n{df.to_html(index=False, border=0, table_id=table_id)}\n{COPY_SCRIPT.replace('REPLACEMENT_HOOK', table_id)}"
             return full_html
         ipython.display_formatter.formatters['text/html'].for_type(DataFrame, custom_dataframe_display)
 
     
 
     
 try:
     from lusid_express.config import load
     config = load()
     if config is None:
         pass
     else:
-        initialize_ipython(config)
+        __initialize_ipython(config)
 except Exception as e:
     print(e)
     pass
```

