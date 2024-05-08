# Comparing `tmp/marksocket-0.2.tar.gz` & `tmp/marksocket-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "marksocket-0.2.tar", last modified: Wed May  8 12:26:36 2024, max compression
+gzip compressed data, was "marksocket-0.3.tar", last modified: Wed May  8 14:12:58 2024, max compression
```

## Comparing `marksocket-0.2.tar` & `marksocket-0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 aapo      (1001) aapo      (1001)        0 2024-05-08 12:26:36.174536 marksocket-0.2/
--rw-r--r--   0 aapo      (1001) aapo      (1001)     7652 2024-05-08 11:42:29.000000 marksocket-0.2/LICENSE
--rw-r--r--   0 aapo      (1001) aapo      (1001)      370 2024-05-08 12:26:36.174536 marksocket-0.2/PKG-INFO
-drwxr-xr-x   0 aapo      (1001) aapo      (1001)        0 2024-05-08 12:26:36.170536 marksocket-0.2/marksocket.egg-info/
--rw-r--r--   0 aapo      (1001) aapo      (1001)      370 2024-05-08 12:26:36.000000 marksocket-0.2/marksocket.egg-info/PKG-INFO
--rw-r--r--   0 aapo      (1001) aapo      (1001)      252 2024-05-08 12:26:36.000000 marksocket-0.2/marksocket.egg-info/SOURCES.txt
--rw-r--r--   0 aapo      (1001) aapo      (1001)        1 2024-05-08 12:26:36.000000 marksocket-0.2/marksocket.egg-info/dependency_links.txt
--rw-r--r--   0 aapo      (1001) aapo      (1001)       47 2024-05-08 12:26:36.000000 marksocket-0.2/marksocket.egg-info/entry_points.txt
--rw-r--r--   0 aapo      (1001) aapo      (1001)       49 2024-05-08 12:26:36.000000 marksocket-0.2/marksocket.egg-info/requires.txt
--rw-r--r--   0 aapo      (1001) aapo      (1001)       11 2024-05-08 12:26:36.000000 marksocket-0.2/marksocket.egg-info/top_level.txt
--rw-r-xr-x   0 aapo      (1001) aapo      (1001)     5957 2024-05-08 10:40:00.000000 marksocket-0.2/marksocket.py
--rw-r--r--   0 aapo      (1001) aapo      (1001)      530 2024-05-08 12:07:41.000000 marksocket-0.2/pyproject.toml
--rw-r--r--   0 aapo      (1001) aapo      (1001)     4336 2024-05-08 09:23:22.000000 marksocket-0.2/readme.md
--rw-r--r--   0 aapo      (1001) aapo      (1001)       38 2024-05-08 12:26:36.174536 marksocket-0.2/setup.cfg
+drwxr-xr-x   0 aapo      (1001) aapo      (1001)        0 2024-05-08 14:12:58.779684 marksocket-0.3/
+-rw-r--r--   0 aapo      (1001) aapo      (1001)     7652 2024-05-08 11:42:29.000000 marksocket-0.3/LICENSE
+-rw-r--r--   0 aapo      (1001) aapo      (1001)      452 2024-05-08 14:12:58.779684 marksocket-0.3/PKG-INFO
+drwxr-xr-x   0 aapo      (1001) aapo      (1001)        0 2024-05-08 14:12:58.775684 marksocket-0.3/marksocket.egg-info/
+-rw-r--r--   0 aapo      (1001) aapo      (1001)      452 2024-05-08 14:12:58.000000 marksocket-0.3/marksocket.egg-info/PKG-INFO
+-rw-r--r--   0 aapo      (1001) aapo      (1001)      252 2024-05-08 14:12:58.000000 marksocket-0.3/marksocket.egg-info/SOURCES.txt
+-rw-r--r--   0 aapo      (1001) aapo      (1001)        1 2024-05-08 14:12:58.000000 marksocket-0.3/marksocket.egg-info/dependency_links.txt
+-rw-r--r--   0 aapo      (1001) aapo      (1001)       47 2024-05-08 14:12:58.000000 marksocket-0.3/marksocket.egg-info/entry_points.txt
+-rw-r--r--   0 aapo      (1001) aapo      (1001)       80 2024-05-08 14:12:58.000000 marksocket-0.3/marksocket.egg-info/requires.txt
+-rw-r--r--   0 aapo      (1001) aapo      (1001)       11 2024-05-08 14:12:58.000000 marksocket-0.3/marksocket.egg-info/top_level.txt
+-rw-r-xr-x   0 aapo      (1001) aapo      (1001)     5957 2024-05-08 10:40:00.000000 marksocket-0.3/marksocket.py
+-rw-r--r--   0 aapo      (1001) aapo      (1001)      566 2024-05-08 13:41:52.000000 marksocket-0.3/pyproject.toml
+-rw-r--r--   0 aapo      (1001) aapo      (1001)     6838 2024-05-08 14:04:04.000000 marksocket-0.3/readme.md
+-rw-r--r--   0 aapo      (1001) aapo      (1001)       38 2024-05-08 14:12:58.779684 marksocket-0.3/setup.cfg
```

### Comparing `marksocket-0.2/LICENSE` & `marksocket-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `marksocket-0.2/marksocket.py` & `marksocket-0.3/marksocket.py`

 * *Files identical despite different names*

### Comparing `marksocket-0.2/pyproject.toml` & `marksocket-0.3/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "marksocket"
-version = "0.2"
+version = "0.3"
 
 authors = [
     { name = "rauaap" }
 ]
 
 dependencies = [
     "markdown >= 3.4.1"
@@ -14,14 +14,15 @@
 
 classifiers = [
     "License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)"
 ]
 
 [project.optional-dependencies]
 mermaid = ["markdown-mermaid >= 0.1"]
+highlights = ["Pygments >= 2.14.0"]
 
 [project.scripts]
 marksocket = "marksocket:main"
 
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
```

### Comparing `marksocket-0.2/readme.md` & `marksocket-0.3/readme.md`

 * *Files 26% similar despite different names*

```diff
@@ -2,61 +2,93 @@
 
 ![](logo.svg)
 
 ## What
 
 A python script to parse and serve markdown documents to a browser with live reload.
 
+- Only one required external Python dependency: The markdown parser. The rest are optional Python-Markdown extensions.<br>
+- Only ~200 lines of python powered by the standard library.
+- Uses sockets under the hood to deliver the documents, no full fledged HTTP server needed.
+- It even serves the images!
+- Doesn't work on Windows however. Not my problem.
+
 ## Why
 
-Because people are out there importing entire HTTP servers and 300 npm packages just to have a markdown document reload in their browsers. I'm not about that life.
+Because most of the pre-existing solutions were either gargantuan in size, shipping with over 400 npm packages as dependencies, or weren't modular enough.
 
-## How
+## Installation
 
-- One external dependency: The markdown parser.<br>
-`sudo apt install python3-markdown`
-- Only ~140 lines of python powered by the standard library.
-- Uses sockets, no HTTP server needed.
-- It even serves the images!
-- Doesn't work on Windows though. Not my problem.
+To install without any Python-Markdown extensions:
+
+```bash
+pip install marksocket
+```
+
+With Markdown-Extensions:
+
+```bash
+pip install marksocket[mermaid, highlights]
+```
+
+You can choose any or none of the extensions, mix them as you wish.
 
 ## Usage
 
-`marksocket [-h] [-c CONFIG_FILE] [-p PORT] [-s STYLESHEET]... [-j JAVASCRIPT]... markdown_file`
+```
+marksocket [-h] [-c CONFIG_FILE] [-p PORT] -x [EXTENSION]... [-s STYLESHEET]... [-j JAVASCRIPT]... markdown_file`
+```
 
 ### Example
 
-`marksocket -p 8001 -s style.css readme.md`
+```bash
+marksocket -p 8001 -s style.css readme.md`
+```
 
 ### Options
 
 - -h: Help.
 - -c: Configuration file.
 - -p: The port to serve at. Command line argument takes precedence over the port specified in the configuration file. Defaults to 44444 if not specified on the command line or in the configuration file.
-- -x: A [Python-Markdown extension](https://python-markdown.github.io/extensions/) to be loaded by the markdown parser. Multiple extensions can be specified like so:<br>
-`marksocket -x fenced_code -x codehilite -x markdown_mermaid readme.md`
-- -s: A stylesheet containing css to be inserted in-line into the HTML parsed from the markdown. Multiple stylesheets are inserted in the order they are given on the command line and can be specified like so:<br>`marksocket -s style1.css -s style2.css readme.md`
-- -j: A file containing JavaScript to be inserted in-line into the head tags of the HTML document. Multiple files are inserted in the order they are given on the command line and can be specified like so:<br>`marksocket -j script1.js -j script2.js readme.md`
+- -x: A [Python-Markdown extension](https://python-markdown.github.io/extensions/) to be loaded by the markdown parser. Multiple extensions can be specified like so:
+
+```
+marksocket -x fenced_code -x markdown_mermaid readme.md
+```
+
+- -s: A stylesheet containing css to be inserted in-line into the HTML parsed from the markdown. Multiple stylesheets are inserted in the order they are given on the command line and can be specified like so:
+
+```
+marksocket -s style1.css -s style2.css readme.md
+```
+
+- -j: A file containing JavaScript to be inserted in-line into the head tags of the HTML document. Multiple files are inserted in the order they are given on the command line and can be specified like so:
+
+```
+marksocket -j script1.js -j script2.js readme.md
+```
 
 ## Configuration file
 
 Allows specifying the port, stylesheet and javascript options. If the path to a configuration file is not given as a command line argument with the `-c` option, `~/.config/marksocket/config.toml` is looked for one. However both are optional and no configuration file is required to use the program. The command line option takes precedence over the default location, so the default configuration file in `~/.config/marksocket/config.toml` will not be loaded if the configuration file option `-c` is specified.
 
 The configuration file is written in TOML. All values in it are optional. You can specify any or none of them. It has the following schema:
 
 ```
 port = int
+extension = [ str ]
 javascript = [ str ]
 stylesheet = [ str ]
 ```
 
 Example:
 
 ```toml
 port = 8000
+extension = [ 'markdown_mermaid', 'fenced_code' ]
 javascript = [ 'mermaid.min.js', 'reload-mermaid.js' ]
 stylesheet = [ 'style.css' ]
 ```
 
 ### Order of the javascript and stylesheet files
 
 Command line options for loading javascript files (`-j`) and stylesheet files (`-s`) can both be used simultaneously with `javascript` and `stylesheet` options in the configuration file. The order the files are loaded in is as follows:
@@ -64,17 +96,46 @@
 1. JavaScript files specified in the configuration file, in the order they are specified.
 2. JavaScript files specified on the command line, in the order they are specified.
 3. Stylesheet files specified in the configuration file, in the order they are specified.
 4. Stylesheet files specified on the command line, in the order they are specified.
 
 ## Extensions
 
-If the [markdown-mermaid](https://github.com/rauaap/markdown-mermaid) extension is found it is loaded automatically. Note that the extension itself will not render the Mermaid graphs. Include the Mermaid JavaScript library and an additional script that runs Mermaid when the document is reloaded.
+### Mermaid
 
-### Example
+```mermaid
+graph TB
+    a(A)
+    x{X}
+    b(B)
+    c(C)
+
+    a --> x
+    x -->|True| b
+    x -->|False| c
+
+    style x fill:#fcf;
+    style a fill:#ccf;
+    style b fill:#cfc;
+    style c fill:#fcc;
+```
+*Example of a Mermaid graph*
+
+If the optional dependency `mermaid` is specified during installation:
+
+```bash
+pip install marksocket[mermaid]
+```
+
+The Markdown-Python extension [markdown-mermaid](https://github.com/rauaap/markdown-mermaid) is installed. Note that the extension itself will not render the Mermaid graphs. Include the Mermaid JavaScript library and an additional script that runs Mermaid when the document is reloaded.
+
+> [!NOTE]
+> If you're writing a markdown document for Github, it supports the Mermaid syntax out of the box, so once you're done editing your document with Marksocket, it's good to go and no additional work is required. Just push your document and the graphs will be rendered on Github too!
+
+#### Configuration
 
 Assume we have downloaded `mermaid.min.js` from a [CDN](https://cdn.jsdelivr.net/npm/mermaid/dist/) and also created a file `reload-mermaid.js` with the following contents:
 
 ```javascript
 let scrollPos;
 
 window.addEventListener('scroll', (e) => {
@@ -92,9 +153,55 @@
         window.scrollTo(0, scrollPos);
     });
 
     observer.observe(document.body, {childList: true});
 });
 ```
 
-Now marksocket could be called with said files to enable Mermaid graph rendering:<br>
-`marksocket -j mermaid.min.js -j reload-mermaid.js readme.md`
+Now marksocket could be called with said files to enable Mermaid graph rendering:
+
+```bash
+marksocket -x markdown_mermaid -j mermaid.min.js -j reload-mermaid.js readme.md`
+```
+
+Or better yet, include it in your configuration file:
+
+```TOML
+extension = [ 'markdown_mermaid' ]
+javascript = [ 'mermaid.min.js', 'reload-mermaid.js' ]
+```
+
+### Code Highlights
+
+If the optional dependency `highlights` is specified during installation:
+
+```bash
+pip install marksocket[highlights]
+```
+
+An additional dependency [Pygments](https://pygments.org/) is installed. The Markdown-Python extension `codehilite` uses it for code highlighting (this extensions is included with Python-Markdown).
+
+#### Configuration
+
+Use Pygments to generate a stylesheet:
+
+```bash
+pygmentize -S default -f html -a .codehilite > highlights.css
+```
+
+> *More options can be found in the [Pygments documentation](https://pygments.org/docs/)*
+
+And then include the codehilite extension with the `-x` flag and the stylesheet that was generated with the `-s` flag:
+
+```bash
+marksocket -x codehilite -x fenced_code -s highlights.css readme.md
+```
+
+Or include them in your configuration:
+
+```TOML
+extension = [ 'codehilite', 'fenced_code' ]
+stylesheet = [ 'highlights.css' ]
+```
+
+> ![NOTE]
+> You most likely want the [Fenced Code Blocks extension](https://python-markdown.github.io/extensions/fenced_code_blocks/) too when including code in your documents, which is why it was included in the examples. This extension ships with Python-Markdown so no additional configuration or installations are required.
```

