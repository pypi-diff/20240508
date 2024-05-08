# Comparing `tmp/poetry_plugin_dotenv-2.1.2.tar.gz` & `tmp/poetry_plugin_dotenv-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry_plugin_dotenv-2.1.2.tar", max compression
+gzip compressed data, was "poetry_plugin_dotenv-2.1.3.tar", max compression
```

## Comparing `poetry_plugin_dotenv-2.1.2.tar` & `poetry_plugin_dotenv-2.1.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1077 2024-05-08 20:07:23.245219 poetry_plugin_dotenv-2.1.2/LICENSE
--rw-r--r--   0        0        0     9687 2024-05-08 20:07:23.245219 poetry_plugin_dotenv-2.1.2/README.md
--rw-r--r--   0        0        0     6955 2024-05-08 20:07:43.821416 poetry_plugin_dotenv-2.1.2/pyproject.toml
--rw-r--r--   0        0        0      778 2024-05-08 20:07:43.825416 poetry_plugin_dotenv-2.1.2/src/poetry_plugin_dotenv/__init__.py
--rw-r--r--   0        0        0     3051 2024-05-08 20:07:23.257219 poetry_plugin_dotenv-2.1.2/src/poetry_plugin_dotenv/config.py
--rw-r--r--   0        0        0      335 2024-05-08 20:07:23.257219 poetry_plugin_dotenv-2.1.2/src/poetry_plugin_dotenv/dotenv/__init__.py
--rw-r--r--   0        0        0     5421 2024-05-08 20:07:23.257219 poetry_plugin_dotenv-2.1.2/src/poetry_plugin_dotenv/dotenv/core.py
--rw-r--r--   0        0        0     6005 2024-05-08 20:07:23.257219 poetry_plugin_dotenv-2.1.2/src/poetry_plugin_dotenv/dotenv/parsers.py
--rw-r--r--   0        0        0     1572 2024-05-08 20:07:23.257219 poetry_plugin_dotenv-2.1.2/src/poetry_plugin_dotenv/dotenv/variables.py
--rw-r--r--   0        0        0     1558 2024-05-08 20:07:23.257219 poetry_plugin_dotenv-2.1.2/src/poetry_plugin_dotenv/logger.py
--rw-r--r--   0        0        0     1999 2024-05-08 20:07:23.257219 poetry_plugin_dotenv-2.1.2/src/poetry_plugin_dotenv/plugin.py
--rw-r--r--   0        0        0        0 2024-05-08 20:07:23.257219 poetry_plugin_dotenv-2.1.2/src/poetry_plugin_dotenv/py.typed
--rw-r--r--   0        0        0    11690 1970-01-01 00:00:00.000000 poetry_plugin_dotenv-2.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1077 2024-05-08 20:13:45.333645 poetry_plugin_dotenv-2.1.3/LICENSE
+-rw-r--r--   0        0        0     8718 2024-05-08 20:13:45.333645 poetry_plugin_dotenv-2.1.3/README.md
+-rw-r--r--   0        0        0     6955 2024-05-08 20:14:07.785750 poetry_plugin_dotenv-2.1.3/pyproject.toml
+-rw-r--r--   0        0        0      778 2024-05-08 20:14:07.785750 poetry_plugin_dotenv-2.1.3/src/poetry_plugin_dotenv/__init__.py
+-rw-r--r--   0        0        0     3051 2024-05-08 20:13:45.345646 poetry_plugin_dotenv-2.1.3/src/poetry_plugin_dotenv/config.py
+-rw-r--r--   0        0        0      335 2024-05-08 20:13:45.345646 poetry_plugin_dotenv-2.1.3/src/poetry_plugin_dotenv/dotenv/__init__.py
+-rw-r--r--   0        0        0     5421 2024-05-08 20:13:45.345646 poetry_plugin_dotenv-2.1.3/src/poetry_plugin_dotenv/dotenv/core.py
+-rw-r--r--   0        0        0     6005 2024-05-08 20:13:45.345646 poetry_plugin_dotenv-2.1.3/src/poetry_plugin_dotenv/dotenv/parsers.py
+-rw-r--r--   0        0        0     1572 2024-05-08 20:13:45.345646 poetry_plugin_dotenv-2.1.3/src/poetry_plugin_dotenv/dotenv/variables.py
+-rw-r--r--   0        0        0     1558 2024-05-08 20:13:45.345646 poetry_plugin_dotenv-2.1.3/src/poetry_plugin_dotenv/logger.py
+-rw-r--r--   0        0        0     1999 2024-05-08 20:13:45.345646 poetry_plugin_dotenv-2.1.3/src/poetry_plugin_dotenv/plugin.py
+-rw-r--r--   0        0        0        0 2024-05-08 20:13:45.345646 poetry_plugin_dotenv-2.1.3/src/poetry_plugin_dotenv/py.typed
+-rw-r--r--   0        0        0    10721 1970-01-01 00:00:00.000000 poetry_plugin_dotenv-2.1.3/PKG-INFO
```

### Comparing `poetry_plugin_dotenv-2.1.2/LICENSE` & `poetry_plugin_dotenv-2.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `poetry_plugin_dotenv-2.1.2/README.md` & `poetry_plugin_dotenv-2.1.3/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 <div align="center">
     <img alt="logo" src="https://github.com/pivoshenko/poetry-plugin-dotenv/blob/main/docs/assets/logo.svg?raw=True" height=300>
 </div>
 
 <p align="center">
+    <a href="https://python-poetry.org">
+        <img alt="poetry" src="https://img.shields.io/endpoint?url=https://python-poetry.org/badge/v0.json">
+    </a>
     <a href="https://opensource.org/licenses/MIT">
         <img alt="license" src="https://img.shields.io/pypi/l/poetry-plugin-dotenv?logo=opensourceinitiative">
     </a>
     <a href="https://pypi.org/project/poetry-plugin-dotenv">
         <img alt="python" src="https://img.shields.io/pypi/pyversions/poetry-plugin-dotenv?logo=python">
     </a>
     <a href="https://pypi.org/project/poetry-plugin-dotenv">
@@ -29,35 +32,26 @@
     </a>
     <a href="https://mypy.readthedocs.io/en/stable/index.html">
         <img alt="mypy" src="https://img.shields.io/badge/mypy-checked-success.svg?logo=python">
     </a>
     <a href="https://github.com/semantic-release/semantic-release">
         <img alt="semantic_release" src="https://img.shields.io/badge/semantic_release-angular-e10079?logo=semantic-release">
     </a>
-    <a href="https://python-poetry.org">
-        <img alt="poetry" src="https://img.shields.io/endpoint?url=https://python-poetry.org/badge/v0.json">
-    </a>
-    <a href="https://numpydoc.readthedocs.io/en/latest/format.html">
-        <img alt="numpydoc" src="https://img.shields.io/badge/docstrings-numpy-1f425f.svg?logo=numpy">
-    </a>
 </p>
 
 <p align="center">
     <a href="https://github.com/dependabot">
         <img alt="dependabot" src="https://img.shields.io/badge/dependabot-enable-success?logo=Dependabot">
     </a>
     <a href="https://github.com/pivoshenko/poetry-plugin-dotenv/actions/workflows/ci.yaml">
         <img alt="CI" src="https://img.shields.io/github/actions/workflow/status/pivoshenko/poetry-plugin-dotenv/ci.yaml?label=CI&logo=github">
     </a>
     <a href="https://github.com/pivoshenko/poetry-plugin-dotenv/actions/workflows/cd.yaml">
         <img alt="CD" src="https://img.shields.io/github/actions/workflow/status/pivoshenko/poetry-plugin-dotenv/cd.yaml?label=CD&logo=github">
     </a>
-    <a href="https://github.com/pivoshenko/poetry-plugin-dotenv/actions/workflows/dependency-review.yaml">
-        <img alt="Dependency Review" src="https://img.shields.io/github/actions/workflow/status/pivoshenko/poetry-plugin-dotenv/dependency-review.yaml?label=Dependency%20Review&logo=github">
-    </a>
     <a href="https://github.com/pivoshenko/poetry-plugin-dotenv/blob/main/.pre-commit-config.yaml">
         <img alt="hooks" src="https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit">
     </a>
     <a href="https://pypi.org/project/poetry-plugin-dotenv">
         <img alt="wheel" src="https://img.shields.io/pypi/wheel/poetry-plugin-dotenv?logo=pypi">
     </a>
 </p>
@@ -71,23 +65,17 @@
     </a>
     <a href="https://pypi.org/project/poetry-plugin-dotenv">
         <img alt="downloads" src="https://img.shields.io/pypi/dm/poetry-plugin-dotenv?logo=pypi">
     </a>
     <a href="https://github.com/pivoshenko/poetry-plugin-dotenv/">
         <img alt="stars" src="https://img.shields.io/github/stars/pivoshenko/poetry-plugin-dotenv?style=flat&logo=github">
     </a>
-    <a href="https://wakatime.com/badge/user/9862508c-0a86-427a-929c-46186f2d191a/project/36344bbb-7f11-4dcd-a36d-e54c81551119">
-        <img alt="wakatime" src="https://wakatime.com/badge/user/9862508c-0a86-427a-929c-46186f2d191a/project/36344bbb-7f11-4dcd-a36d-e54c81551119.svg">
-    </a>
 </p>
 
 <p align="center">
-    <a href="https://www.buymeacoffee.com/pivoshenko" target="_blank">
-        <img alt="buymeacoffee" src="https://img.shields.io/badge/buy_me_-a_coffee-ff6964?logo=buymeacoffee">
-    </a>
     <a href="https://stand-with-ukraine.pp.ua/">
         <img alt="standwithukraine" src="https://img.shields.io/badge/Support-Ukraine-FFD500?style=flat&labelColor=005BBB">
     </a>
     <a href="https://stand-with-ukraine.pp.ua">
         <img alt="standwithukraine" src="https://img.shields.io/badge/made_in-Ukraine-ffd700.svg?labelColor=0057b7">
     </a>
 </p>
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
                                     [logo]
-                       _[_l_i_c_e_n_s_e_]_[_p_y_t_h_o_n_]_[_p_y_p_i_]_[_r_e_l_e_a_s_e_]
-        _[_b_l_a_c_k_]_[_i_s_o_r_t_]_[_r_u_f_f_]_[_m_y_p_y_]_[_s_e_m_a_n_t_i_c___r_e_l_e_a_s_e_]_[_p_o_e_t_r_y_]_[_n_u_m_p_y_d_o_c_]
-             _[_d_e_p_e_n_d_a_b_o_t_]_[_C_I_]_[_C_D_]_[_D_e_p_e_n_d_e_n_c_y_ _R_e_v_i_e_w_]_[_h_o_o_k_s_]_[_w_h_e_e_l_]
-              _[_c_o_d_e_c_o_v_]_[_c_o_d_e_c_l_i_m_a_t_e_]_[_d_o_w_n_l_o_a_d_s_]_[_s_t_a_r_s_]_[_w_a_k_a_t_i_m_e_]
-              _[_b_u_y_m_e_a_c_o_f_f_e_e_]_[_s_t_a_n_d_w_i_t_h_u_k_r_a_i_n_e_]_[_s_t_a_n_d_w_i_t_h_u_k_r_a_i_n_e_]
+                   _[_p_o_e_t_r_y_]_[_l_i_c_e_n_s_e_]_[_p_y_t_h_o_n_]_[_p_y_p_i_]_[_r_e_l_e_a_s_e_]
+                 _[_b_l_a_c_k_]_[_i_s_o_r_t_]_[_r_u_f_f_]_[_m_y_p_y_]_[_s_e_m_a_n_t_i_c___r_e_l_e_a_s_e_]
+                      _[_d_e_p_e_n_d_a_b_o_t_]_[_C_I_]_[_C_D_]_[_h_o_o_k_s_]_[_w_h_e_e_l_]
+                   _[_c_o_d_e_c_o_v_]_[_c_o_d_e_c_l_i_m_a_t_e_]_[_d_o_w_n_l_o_a_d_s_]_[_s_t_a_r_s_]
+                     _[_s_t_a_n_d_w_i_t_h_u_k_r_a_i_n_e_]_[_s_t_a_n_d_w_i_t_h_u_k_r_a_i_n_e_]
 - [Overview](#overview) - [Features](#features) - [Installation](#installation)
 - [Usage and Configuration](#usage-and-configuration) - [Configuration via
 file](#configuration-via-file) - [Configuration via environment variables]
 (#configuration-via-environment-variables) - [Lookup hierarchy](#lookup-
 hierarchy) - [Examples](#examples) ## Overview `poetry-plugin-dotenv` - is the
 plugin that automatically loads environment variables from a dotenv file into
 the environment before `poetry` commands are run. ### Features - Doesn't
```

### Comparing `poetry_plugin_dotenv-2.1.2/pyproject.toml` & `poetry_plugin_dotenv-2.1.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "poetry-plugin-dotenv"
-version = "2.1.2"
+version = "2.1.3"
 description = "poetry-plugin-dotenv - is the plugin that automatically loads environment variables from a dotenv file into the environment before poetry commands are run."
 license = "MIT"
 authors = ["Volodymyr Pivoshenko <volodymyr.pivoshenko@gmail.com>"]
 maintainers = ["Volodymyr Pivoshenko <volodymyr.pivoshenko@gmail.com>"]
 keywords = [
   "python",
   "pypi",
```

### Comparing `poetry_plugin_dotenv-2.1.2/src/poetry_plugin_dotenv/__init__.py` & `poetry_plugin_dotenv-2.1.3/src/poetry_plugin_dotenv/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """poetry-plugin-dotenv - is the plugin that automatically loads environment variables from a dotenv file into the environment before poetry commands are run."""
 
 __title__ = "poetry-plugin-dotenv"
 __summary__ = "poetry-plugin-dotenv - is the plugin that automatically loads environment variables from a dotenv file into the environment before poetry commands are run."
 __uri__ = "https://github.com/pivoshenko/poetry-plugin-dotenv"
 
-__version__ = "2.1.2"
+__version__ = "2.1.3"
 
 __author__ = "Volodymyr Pivoshenko"
 __email__ = "volodymyr.pivoshenko@gmail.com"
 
 __license__ = "MIT"
 __copyright__ = "Copyright 2023, Volodymyr Pivoshenko"
```

### Comparing `poetry_plugin_dotenv-2.1.2/src/poetry_plugin_dotenv/config.py` & `poetry_plugin_dotenv-2.1.3/src/poetry_plugin_dotenv/config.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_dotenv-2.1.2/src/poetry_plugin_dotenv/dotenv/core.py` & `poetry_plugin_dotenv-2.1.3/src/poetry_plugin_dotenv/dotenv/core.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_dotenv-2.1.2/src/poetry_plugin_dotenv/dotenv/parsers.py` & `poetry_plugin_dotenv-2.1.3/src/poetry_plugin_dotenv/dotenv/parsers.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_dotenv-2.1.2/src/poetry_plugin_dotenv/dotenv/variables.py` & `poetry_plugin_dotenv-2.1.3/src/poetry_plugin_dotenv/dotenv/variables.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_dotenv-2.1.2/src/poetry_plugin_dotenv/logger.py` & `poetry_plugin_dotenv-2.1.3/src/poetry_plugin_dotenv/logger.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_dotenv-2.1.2/src/poetry_plugin_dotenv/plugin.py` & `poetry_plugin_dotenv-2.1.3/src/poetry_plugin_dotenv/plugin.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_dotenv-2.1.2/PKG-INFO` & `poetry_plugin_dotenv-2.1.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poetry-plugin-dotenv
-Version: 2.1.2
+Version: 2.1.3
 Summary: poetry-plugin-dotenv - is the plugin that automatically loads environment variables from a dotenv file into the environment before poetry commands are run.
 Home-page: https://github.com/pivoshenko/poetry-plugin-dotenv
 License: MIT
 Keywords: python,pypi,poetry,plugin,plugins,poetry-plugin,poetry-plugins,env,dotenv,config,configuration,configuration-management,cross-platform,hacktoberfest
 Author: Volodymyr Pivoshenko
 Author-email: volodymyr.pivoshenko@gmail.com
 Maintainer: Volodymyr Pivoshenko
@@ -37,14 +37,17 @@
 Description-Content-Type: text/markdown
 
 <div align="center">
     <img alt="logo" src="https://github.com/pivoshenko/poetry-plugin-dotenv/blob/main/docs/assets/logo.svg?raw=True" height=300>
 </div>
 
 <p align="center">
+    <a href="https://python-poetry.org">
+        <img alt="poetry" src="https://img.shields.io/endpoint?url=https://python-poetry.org/badge/v0.json">
+    </a>
     <a href="https://opensource.org/licenses/MIT">
         <img alt="license" src="https://img.shields.io/pypi/l/poetry-plugin-dotenv?logo=opensourceinitiative">
     </a>
     <a href="https://pypi.org/project/poetry-plugin-dotenv">
         <img alt="python" src="https://img.shields.io/pypi/pyversions/poetry-plugin-dotenv?logo=python">
     </a>
     <a href="https://pypi.org/project/poetry-plugin-dotenv">
@@ -67,35 +70,26 @@
     </a>
     <a href="https://mypy.readthedocs.io/en/stable/index.html">
         <img alt="mypy" src="https://img.shields.io/badge/mypy-checked-success.svg?logo=python">
     </a>
     <a href="https://github.com/semantic-release/semantic-release">
         <img alt="semantic_release" src="https://img.shields.io/badge/semantic_release-angular-e10079?logo=semantic-release">
     </a>
-    <a href="https://python-poetry.org">
-        <img alt="poetry" src="https://img.shields.io/endpoint?url=https://python-poetry.org/badge/v0.json">
-    </a>
-    <a href="https://numpydoc.readthedocs.io/en/latest/format.html">
-        <img alt="numpydoc" src="https://img.shields.io/badge/docstrings-numpy-1f425f.svg?logo=numpy">
-    </a>
 </p>
 
 <p align="center">
     <a href="https://github.com/dependabot">
         <img alt="dependabot" src="https://img.shields.io/badge/dependabot-enable-success?logo=Dependabot">
     </a>
     <a href="https://github.com/pivoshenko/poetry-plugin-dotenv/actions/workflows/ci.yaml">
         <img alt="CI" src="https://img.shields.io/github/actions/workflow/status/pivoshenko/poetry-plugin-dotenv/ci.yaml?label=CI&logo=github">
     </a>
     <a href="https://github.com/pivoshenko/poetry-plugin-dotenv/actions/workflows/cd.yaml">
         <img alt="CD" src="https://img.shields.io/github/actions/workflow/status/pivoshenko/poetry-plugin-dotenv/cd.yaml?label=CD&logo=github">
     </a>
-    <a href="https://github.com/pivoshenko/poetry-plugin-dotenv/actions/workflows/dependency-review.yaml">
-        <img alt="Dependency Review" src="https://img.shields.io/github/actions/workflow/status/pivoshenko/poetry-plugin-dotenv/dependency-review.yaml?label=Dependency%20Review&logo=github">
-    </a>
     <a href="https://github.com/pivoshenko/poetry-plugin-dotenv/blob/main/.pre-commit-config.yaml">
         <img alt="hooks" src="https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit">
     </a>
     <a href="https://pypi.org/project/poetry-plugin-dotenv">
         <img alt="wheel" src="https://img.shields.io/pypi/wheel/poetry-plugin-dotenv?logo=pypi">
     </a>
 </p>
@@ -109,23 +103,17 @@
     </a>
     <a href="https://pypi.org/project/poetry-plugin-dotenv">
         <img alt="downloads" src="https://img.shields.io/pypi/dm/poetry-plugin-dotenv?logo=pypi">
     </a>
     <a href="https://github.com/pivoshenko/poetry-plugin-dotenv/">
         <img alt="stars" src="https://img.shields.io/github/stars/pivoshenko/poetry-plugin-dotenv?style=flat&logo=github">
     </a>
-    <a href="https://wakatime.com/badge/user/9862508c-0a86-427a-929c-46186f2d191a/project/36344bbb-7f11-4dcd-a36d-e54c81551119">
-        <img alt="wakatime" src="https://wakatime.com/badge/user/9862508c-0a86-427a-929c-46186f2d191a/project/36344bbb-7f11-4dcd-a36d-e54c81551119.svg">
-    </a>
 </p>
 
 <p align="center">
-    <a href="https://www.buymeacoffee.com/pivoshenko" target="_blank">
-        <img alt="buymeacoffee" src="https://img.shields.io/badge/buy_me_-a_coffee-ff6964?logo=buymeacoffee">
-    </a>
     <a href="https://stand-with-ukraine.pp.ua/">
         <img alt="standwithukraine" src="https://img.shields.io/badge/Support-Ukraine-FFD500?style=flat&labelColor=005BBB">
     </a>
     <a href="https://stand-with-ukraine.pp.ua">
         <img alt="standwithukraine" src="https://img.shields.io/badge/made_in-Ukraine-ffd700.svg?labelColor=0057b7">
     </a>
 </p>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: poetry-plugin-dotenv Version: 2.1.2 Summary:
+Metadata-Version: 2.1 Name: poetry-plugin-dotenv Version: 2.1.3 Summary:
 poetry-plugin-dotenv - is the plugin that automatically loads environment
 variables from a dotenv file into the environment before poetry commands are
 run. Home-page: https://github.com/pivoshenko/poetry-plugin-dotenv License: MIT
 Keywords: python,pypi,poetry,plugin,plugins,poetry-plugin,poetry-
 plugins,env,dotenv,config,configuration,configuration-management,cross-
 platform,hacktoberfest Author: Volodymyr Pivoshenko Author-email:
 volodymyr.pivoshenko@gmail.com Maintainer: Volodymyr Pivoshenko Maintainer-
@@ -22,19 +22,19 @@
 (>=1.5.1) Project-URL: Documentation, https://github.com/pivoshenko/poetry-
 plugin-dotenv Project-URL: Issues, https://github.com/pivoshenko/poetry-plugin-
 dotenv/issues Project-URL: Repository, https://github.com/pivoshenko/poetry-
 plugin-dotenv Project-URL: Releases, https://github.com/pivoshenko/poetry-
 plugin-dotenv/releases Project-URL: Say Thanks!, https://www.buymeacoffee.com/
 pivoshenko Description-Content-Type: text/markdown
                                     [logo]
-                       _[_l_i_c_e_n_s_e_]_[_p_y_t_h_o_n_]_[_p_y_p_i_]_[_r_e_l_e_a_s_e_]
-        _[_b_l_a_c_k_]_[_i_s_o_r_t_]_[_r_u_f_f_]_[_m_y_p_y_]_[_s_e_m_a_n_t_i_c___r_e_l_e_a_s_e_]_[_p_o_e_t_r_y_]_[_n_u_m_p_y_d_o_c_]
-             _[_d_e_p_e_n_d_a_b_o_t_]_[_C_I_]_[_C_D_]_[_D_e_p_e_n_d_e_n_c_y_ _R_e_v_i_e_w_]_[_h_o_o_k_s_]_[_w_h_e_e_l_]
-              _[_c_o_d_e_c_o_v_]_[_c_o_d_e_c_l_i_m_a_t_e_]_[_d_o_w_n_l_o_a_d_s_]_[_s_t_a_r_s_]_[_w_a_k_a_t_i_m_e_]
-              _[_b_u_y_m_e_a_c_o_f_f_e_e_]_[_s_t_a_n_d_w_i_t_h_u_k_r_a_i_n_e_]_[_s_t_a_n_d_w_i_t_h_u_k_r_a_i_n_e_]
+                   _[_p_o_e_t_r_y_]_[_l_i_c_e_n_s_e_]_[_p_y_t_h_o_n_]_[_p_y_p_i_]_[_r_e_l_e_a_s_e_]
+                 _[_b_l_a_c_k_]_[_i_s_o_r_t_]_[_r_u_f_f_]_[_m_y_p_y_]_[_s_e_m_a_n_t_i_c___r_e_l_e_a_s_e_]
+                      _[_d_e_p_e_n_d_a_b_o_t_]_[_C_I_]_[_C_D_]_[_h_o_o_k_s_]_[_w_h_e_e_l_]
+                   _[_c_o_d_e_c_o_v_]_[_c_o_d_e_c_l_i_m_a_t_e_]_[_d_o_w_n_l_o_a_d_s_]_[_s_t_a_r_s_]
+                     _[_s_t_a_n_d_w_i_t_h_u_k_r_a_i_n_e_]_[_s_t_a_n_d_w_i_t_h_u_k_r_a_i_n_e_]
 - [Overview](#overview) - [Features](#features) - [Installation](#installation)
 - [Usage and Configuration](#usage-and-configuration) - [Configuration via
 file](#configuration-via-file) - [Configuration via environment variables]
 (#configuration-via-environment-variables) - [Lookup hierarchy](#lookup-
 hierarchy) - [Examples](#examples) ## Overview `poetry-plugin-dotenv` - is the
 plugin that automatically loads environment variables from a dotenv file into
 the environment before `poetry` commands are run. ### Features - Doesn't
```

