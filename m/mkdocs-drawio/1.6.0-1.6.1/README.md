# Comparing `tmp/mkdocs_drawio-1.6.0.tar.gz` & `tmp/mkdocs_drawio-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs_drawio-1.6.0.tar", max compression
+gzip compressed data, was "mkdocs_drawio-1.6.1.tar", max compression
```

## Comparing `mkdocs_drawio-1.6.0.tar` & `mkdocs_drawio-1.6.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1052 2024-03-24 14:46:27.186280 mkdocs_drawio-1.6.0/LICENSE
--rw-r--r--   0        0        0     1954 2024-03-24 14:46:27.186280 mkdocs_drawio-1.6.0/README.md
--rw-r--r--   0        0        0     3789 2024-03-24 14:46:27.186280 mkdocs_drawio-1.6.0/mkdocs_drawio/plugin.py
--rw-r--r--   0        0        0      840 2024-03-24 14:46:27.186280 mkdocs_drawio-1.6.0/pyproject.toml
--rw-r--r--   0        0        0     2966 1970-01-01 00:00:00.000000 mkdocs_drawio-1.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1052 2024-05-07 23:30:18.113949 mkdocs_drawio-1.6.1/LICENSE
+-rw-r--r--   0        0        0     2313 2024-05-07 23:30:18.113949 mkdocs_drawio-1.6.1/README.md
+-rw-r--r--   0        0        0     3789 2024-05-07 23:30:18.117949 mkdocs_drawio-1.6.1/mkdocs_drawio/plugin.py
+-rw-r--r--   0        0        0      840 2024-05-07 23:30:18.117949 mkdocs_drawio-1.6.1/pyproject.toml
+-rw-r--r--   0        0        0     3325 1970-01-01 00:00:00.000000 mkdocs_drawio-1.6.1/PKG-INFO
```

### Comparing `mkdocs_drawio-1.6.0/LICENSE` & `mkdocs_drawio-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs_drawio-1.6.0/README.md` & `mkdocs_drawio-1.6.1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # MkDocs Plugin for embedding Drawio files
 [![Publish Badge](https://github.com/tuunit/mkdocs-drawio/workflows/Publish/badge.svg)](https://github.com/tuunit/mkdocs-drawio/actions)
 [![PyPI](https://img.shields.io/pypi/v/mkdocs-drawio)](https://pypi.org/project/mkdocs-drawio/)
 
-[Buy Sergey a 🍜](https://www.buymeacoffee.com/SergeyLukin) 
-Sergey (onixpro) is the original creator of this plugin. Repo can be found [here.](https://github.com/onixpro/mkdocs-drawio-file)
+[Buy Sergey a ☕](https://www.buymeacoffee.com/SergeyLukin) 
+
+Sergey ([onixpro](https://github.com/onixpro)) is the original creator of this plugin. Repo can be found [here.](https://github.com/onixpro/mkdocs-drawio-file)
 
 ## Features
-This plugin enables you to embed interactive drawio diagrams in your documentation. Simply add your files like you would any other image:
+This plugin enables you to embed interactive drawio diagrams in your documentation. Simply add your diagrams like you would any other image:
 
 ```markdown
 ![](my-diagram.drawio)
 ```
 
 Additionally this plugin supports multi page diagrams by using the `alt` text to select the pages by name:
 
@@ -32,28 +33,32 @@
 ```yaml
 plugins:
   - drawio
 ```
 
 ### Configuration
 
-To use a custom source for the drawio viewer JavaScript file you can overwritte the url.
+By default the plugin uses the official url for the minified drawio javascript library. To use a custom source for the drawio viewer you can overwritte the url. This might be useful in airlocked environments.
 
 ```yaml
 plugins:
   - drawio:
       viewer_js: "https://viewer.diagrams.net/js/viewer-static.min.js"
 ```
 
 ## How it works
 
-After mkdocs has generated the html for your documentation, this plugin adds the necessary drawio javascript library. Searches for `img` tags with a file ending of `*.drawio` and replaces them with the appropiate `mxgraph` html block. For further details, please have a look at the [official drawio.com documentation](https://www.drawio.com/doc/faq/embed-html).
+1. mkdocs generates the html per page
+2. `mkdocs-drawio` attaches to the `on_post_page` event. For more details, please have a look at the [event lifecycle documentation](https://www.mkdocs.org/dev-guide/plugins/#events)
+3. Adds the drawio viewer library
+4. Searches through the generated html for all `img` tags that have a source of type `.drawio`
+5. Replaces the found `img` tags with `mxgraph` html blocks (actual drawio diagram content). For more details, please have a look at the [official drawio.com documentation](https://www.drawio.com/doc/faq/embed-html).
 
 
 ## Contribution guide
 
 1. Either use the devcontainer or setup a venv with mkdocs installed
 2. Install your current local version: `pip install -e .`
 3. Add a test for your changes in the `example` directory
 4. Test your changes by starting `mkdocs serve` in the `example` directory
 5. Increase the version `pyproject.toml` and `setup.py`
-6. Open pull request
+6. Open pull request
```

### Comparing `mkdocs_drawio-1.6.0/mkdocs_drawio/plugin.py` & `mkdocs_drawio-1.6.1/mkdocs_drawio/plugin.py`

 * *Files identical despite different names*

### Comparing `mkdocs_drawio-1.6.0/pyproject.toml` & `mkdocs_drawio-1.6.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mkdocs-drawio"
-version = "1.6.0"
+version = "1.6.1"
 description = "MkDocs plugin for embedding Drawio files"
 authors = [
     "Sergey Lukin <onixpro@gmail.com>",
     "Jan Larwig <jan@larwig.com>"
 ]
 license = "MIT"
 readme = "README.md"
@@ -15,22 +15,22 @@
 ]
 packages = [
     { include = "mkdocs_drawio/plugin.py" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.7.0"
-requests = "^2.27.1"
-Jinja2 = "^3.0.3"
-beautifulsoup4 = "^4.11.0"
-lxml = "^4.9.0"
-mkdocs = "^1.4.0"
+requests = "^2.31.0"
+Jinja2 = "^3.1.0"
+beautifulsoup4 = "^4.12.0"
+lxml = "^5.0.0"
+mkdocs = "^1.5.0"
 
 [tool.poetry.dev-dependencies]
-black = "^22.1.0"
+black = "^24.4.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.plugins."mkdocs.plugins"]
 drawio = 'mkdocs_drawio.plugin:DrawioPlugin'
```

### Comparing `mkdocs_drawio-1.6.0/PKG-INFO` & `mkdocs_drawio-1.6.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-drawio
-Version: 1.6.0
+Version: 1.6.1
 Summary: MkDocs plugin for embedding Drawio files
 Home-page: https://github.com/tuunit/mkdocs-drawio/
 License: MIT
 Keywords: mkdocs,plugin,markdown,drawio
 Author: Sergey Lukin
 Author-email: onixpro@gmail.com
 Requires-Python: >=3.7.0,<4.0.0
@@ -12,31 +12,32 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: Jinja2 (>=3.0.3,<4.0.0)
-Requires-Dist: beautifulsoup4 (>=4.11.0,<5.0.0)
-Requires-Dist: lxml (>=4.9.0,<5.0.0)
-Requires-Dist: mkdocs (>=1.4.0,<2.0.0)
-Requires-Dist: requests (>=2.27.1,<3.0.0)
+Requires-Dist: Jinja2 (>=3.1.0,<4.0.0)
+Requires-Dist: beautifulsoup4 (>=4.12.0,<5.0.0)
+Requires-Dist: lxml (>=5.0.0,<6.0.0)
+Requires-Dist: mkdocs (>=1.5.0,<2.0.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
 Project-URL: Repository, https://github.com/tuunit/mkdocs-drawio/
 Description-Content-Type: text/markdown
 
 # MkDocs Plugin for embedding Drawio files
 [![Publish Badge](https://github.com/tuunit/mkdocs-drawio/workflows/Publish/badge.svg)](https://github.com/tuunit/mkdocs-drawio/actions)
 [![PyPI](https://img.shields.io/pypi/v/mkdocs-drawio)](https://pypi.org/project/mkdocs-drawio/)
 
-[Buy Sergey a 🍜](https://www.buymeacoffee.com/SergeyLukin) 
-Sergey (onixpro) is the original creator of this plugin. Repo can be found [here.](https://github.com/onixpro/mkdocs-drawio-file)
+[Buy Sergey a ☕](https://www.buymeacoffee.com/SergeyLukin) 
+
+Sergey ([onixpro](https://github.com/onixpro)) is the original creator of this plugin. Repo can be found [here.](https://github.com/onixpro/mkdocs-drawio-file)
 
 ## Features
-This plugin enables you to embed interactive drawio diagrams in your documentation. Simply add your files like you would any other image:
+This plugin enables you to embed interactive drawio diagrams in your documentation. Simply add your diagrams like you would any other image:
 
 ```markdown
 ![](my-diagram.drawio)
 ```
 
 Additionally this plugin supports multi page diagrams by using the `alt` text to select the pages by name:
 
@@ -58,28 +59,33 @@
 ```yaml
 plugins:
   - drawio
 ```
 
 ### Configuration
 
-To use a custom source for the drawio viewer JavaScript file you can overwritte the url.
+By default the plugin uses the official url for the minified drawio javascript library. To use a custom source for the drawio viewer you can overwritte the url. This might be useful in airlocked environments.
 
 ```yaml
 plugins:
   - drawio:
       viewer_js: "https://viewer.diagrams.net/js/viewer-static.min.js"
 ```
 
 ## How it works
 
-After mkdocs has generated the html for your documentation, this plugin adds the necessary drawio javascript library. Searches for `img` tags with a file ending of `*.drawio` and replaces them with the appropiate `mxgraph` html block. For further details, please have a look at the [official drawio.com documentation](https://www.drawio.com/doc/faq/embed-html).
+1. mkdocs generates the html per page
+2. `mkdocs-drawio` attaches to the `on_post_page` event. For more details, please have a look at the [event lifecycle documentation](https://www.mkdocs.org/dev-guide/plugins/#events)
+3. Adds the drawio viewer library
+4. Searches through the generated html for all `img` tags that have a source of type `.drawio`
+5. Replaces the found `img` tags with `mxgraph` html blocks (actual drawio diagram content). For more details, please have a look at the [official drawio.com documentation](https://www.drawio.com/doc/faq/embed-html).
 
 
 ## Contribution guide
 
 1. Either use the devcontainer or setup a venv with mkdocs installed
 2. Install your current local version: `pip install -e .`
 3. Add a test for your changes in the `example` directory
 4. Test your changes by starting `mkdocs serve` in the `example` directory
 5. Increase the version `pyproject.toml` and `setup.py`
 6. Open pull request
+
```

