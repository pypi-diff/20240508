# Comparing `tmp/roff-0.4.2.tar.gz` & `tmp/roff-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roff-0.4.2.tar", last modified: Tue Apr 30 14:12:11 2024, max compression
+gzip compressed data, was "roff-0.4.3.tar", last modified: Wed May  8 08:54:23 2024, max compression
```

## Comparing `roff-0.4.2.tar` & `roff-0.4.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2024-04-30 14:12:11.174853 roff-0.4.2/
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1072 2024-04-23 10:39:23.000000 roff-0.4.2/LICENSE
--rw-r--r--   0 playerg9  (1000) playerg9  (1000)     3370 2024-04-30 14:12:11.174853 roff-0.4.2/PKG-INFO
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1673 2024-04-30 12:20:39.000000 roff-0.4.2/README.md
-drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2024-04-30 14:12:11.166848 roff-0.4.2/docs/
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1687 2024-04-30 14:06:36.000000 roff-0.4.2/docs/roff.1
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     2872 2024-04-30 14:07:40.000000 roff-0.4.2/docs/roff.5
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)       87 2024-04-23 10:39:23.000000 roff-0.4.2/pyproject.toml
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)       38 2024-04-30 14:12:11.174853 roff-0.4.2/setup.cfg
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     2155 2024-04-25 12:26:07.000000 roff-0.4.2/setup.py
-drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2024-04-30 14:12:11.166848 roff-0.4.2/src/
-drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2024-04-30 14:12:11.166848 roff-0.4.2/src/roff/
-drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2024-04-30 14:12:11.170851 roff-0.4.2/src/roff/__cli__/
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      114 2024-04-30 13:02:33.000000 roff-0.4.2/src/roff/__cli__/__init__.py
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      446 2024-04-25 12:31:14.000000 roff-0.4.2/src/roff/__cli__/convert.py
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1036 2024-04-27 11:58:51.000000 roff-0.4.2/src/roff/__cli__/template.py
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      403 2024-04-30 13:06:47.000000 roff-0.4.2/src/roff/__cli__/tree.py
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      747 2024-04-30 13:14:13.000000 roff-0.4.2/src/roff/__cli__/util.py
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1508 2024-04-30 14:12:01.000000 roff-0.4.2/src/roff/__init__.py
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     2112 2024-04-30 13:13:29.000000 roff-0.4.2/src/roff/__main__.py
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     2641 2024-04-25 14:11:43.000000 roff-0.4.2/src/roff/_images.py
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     2303 2024-04-27 11:58:51.000000 roff-0.4.2/src/roff/_markdown.py
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      901 2024-04-30 14:04:03.000000 roff-0.4.2/src/roff/_util.py
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)    10983 2024-04-30 14:06:15.000000 roff-0.4.2/src/roff/convert.py
-drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2024-04-30 14:12:11.170851 roff-0.4.2/src/roff.egg-info/
--rw-r--r--   0 playerg9  (1000) playerg9  (1000)     3370 2024-04-30 14:12:11.000000 roff-0.4.2/src/roff.egg-info/PKG-INFO
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      517 2024-04-30 14:12:11.000000 roff-0.4.2/src/roff.egg-info/SOURCES.txt
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)        1 2024-04-30 14:12:11.000000 roff-0.4.2/src/roff.egg-info/dependency_links.txt
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)       44 2024-04-30 14:12:11.000000 roff-0.4.2/src/roff.egg-info/entry_points.txt
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)       94 2024-04-30 14:12:11.000000 roff-0.4.2/src/roff.egg-info/requires.txt
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)        5 2024-04-30 14:12:11.000000 roff-0.4.2/src/roff.egg-info/top_level.txt
+drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2024-05-08 08:54:23.162333 roff-0.4.3/
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1072 2024-04-21 09:37:21.000000 roff-0.4.3/LICENSE
+-rw-r--r--   0 playerg9  (1000) playerg9  (1000)     3370 2024-05-08 08:54:23.162333 roff-0.4.3/PKG-INFO
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1673 2024-04-28 12:23:56.000000 roff-0.4.3/README.md
+drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2024-05-08 08:54:23.162333 roff-0.4.3/docs/
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1645 2024-04-29 10:43:42.000000 roff-0.4.3/docs/roff.1
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     2872 2024-04-30 19:29:45.000000 roff-0.4.3/docs/roff.5
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)       87 2024-04-21 09:38:29.000000 roff-0.4.3/pyproject.toml
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)       38 2024-05-08 08:54:23.162333 roff-0.4.3/setup.cfg
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     2155 2024-04-25 15:15:31.000000 roff-0.4.3/setup.py
+drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2024-05-08 08:54:23.158332 roff-0.4.3/src/
+drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2024-05-08 08:54:23.162333 roff-0.4.3/src/roff/
+drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2024-05-08 08:54:23.162333 roff-0.4.3/src/roff/__cli__/
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      114 2024-04-30 19:28:52.000000 roff-0.4.3/src/roff/__cli__/__init__.py
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      446 2024-04-25 15:15:31.000000 roff-0.4.3/src/roff/__cli__/convert.py
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1036 2024-04-27 11:45:13.000000 roff-0.4.3/src/roff/__cli__/template.py
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      403 2024-04-30 19:28:52.000000 roff-0.4.3/src/roff/__cli__/tree.py
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      747 2024-04-30 19:28:52.000000 roff-0.4.3/src/roff/__cli__/util.py
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1508 2024-05-08 08:54:12.000000 roff-0.4.3/src/roff/__init__.py
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     2112 2024-04-30 19:28:52.000000 roff-0.4.3/src/roff/__main__.py
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     2645 2024-04-30 19:28:52.000000 roff-0.4.3/src/roff/_images.py
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     2303 2024-04-27 11:04:01.000000 roff-0.4.3/src/roff/_markdown.py
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      909 2024-05-08 08:47:35.000000 roff-0.4.3/src/roff/_util.py
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)    11980 2024-05-08 08:51:57.000000 roff-0.4.3/src/roff/convert.py
+drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2024-05-08 08:54:23.162333 roff-0.4.3/src/roff.egg-info/
+-rw-r--r--   0 playerg9  (1000) playerg9  (1000)     3370 2024-05-08 08:54:23.000000 roff-0.4.3/src/roff.egg-info/PKG-INFO
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      517 2024-05-08 08:54:23.000000 roff-0.4.3/src/roff.egg-info/SOURCES.txt
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)        1 2024-05-08 08:54:23.000000 roff-0.4.3/src/roff.egg-info/dependency_links.txt
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)       44 2024-05-08 08:54:23.000000 roff-0.4.3/src/roff.egg-info/entry_points.txt
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)       94 2024-05-08 08:54:23.000000 roff-0.4.3/src/roff.egg-info/requires.txt
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)        5 2024-05-08 08:54:23.000000 roff-0.4.3/src/roff.egg-info/top_level.txt
```

### Comparing `roff-0.4.2/LICENSE` & `roff-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `roff-0.4.2/PKG-INFO` & `roff-0.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roff
-Version: 0.4.2
+Version: 0.4.3
 Summary: python-based cli to convert markdown to the roff (man-pages) format
 Home-page: https://github.com/utility-toolbox/roff
 Author: PlayerG9
 License: MIT
 Project-URL: Organisation Github, https://github.com/utility-toolbox
 Project-URL: Homepage, https://github.com/utility-toolbox/roff/
 Project-URL: Bug Tracker, https://github.com/utility-toolbox/roff/issues
```

### Comparing `roff-0.4.2/README.md` & `roff-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `roff-0.4.2/docs/roff.1` & `roff-0.4.3/docs/roff.1`

 * *Files 15% similar despite different names*

```diff
@@ -1,44 +1,44 @@
-.\" generated with roff/v0.4.0
-.\" https://pypi.org/project/roff/0.4.0
+.\" generated with roff/v0.3.1
+.\" https://pypi.org/project/roff/0.3.1
 .\" https://github.com/utility-toolbox/roff/
 .\"
-.TH "ROFF" "1" "30 April 2024" "github.com/utility-toolbox/roff"
+.TH "ROFF" "1" "29 April 2024" "github.com/utility-toolbox/roff"
 .SH "NAME"
-\fBroff\fP • python\[em]based cli to convert markdown to the roff (man\[em]pages) format
+\fBroff\fP • python-based cli to convert markdown to the roff (man-pages) format
 .SH "SYNOPSIS"
 .sp
-• \fBroff\fP [\fB\-h\fP] [\fB\-v\fP] {\fIconvert\fP,\fItemplate\fP} ...
+• \fBroff\fP [\fB-h\fP] [\fB-v\fP] {\fIconvert\fP,\fItemplate\fP} ...
 .br
-• \fBroff\fP \fIconvert\fP [\fB\-h\fP] \fIsource\fP [\fIdest\fP]
+• \fBroff\fP \fIconvert\fP [\fB-h\fP] \fIsource\fP [\fIdest\fP]
 .br
-• \fBroff\fP \fItemplate\fP [\fB\-h\fP] \fIdest\fP
+• \fBroff\fP \fItemplate\fP [\fB-h\fP] \fIdest\fP
 .br
 .sp
 .SH "DESCRIPTION"
-python\[em]based cli to convert markdown to the roff (man\[em]pages) format.
+python-based cli to convert markdown to the roff (man-pages) format\.
 .sp
 .RS 2
 see roff(5) for more information about the file specification
 .RE
 .sp
 Support for all* Markdown features:
 .sp
 .RS 2
-*h1 is reserved for the head.
+*h1 is reserved for the head\.
 .RE
 .sp
 .sp
-• heading (h2\[em]h6)
+• heading (h2-h6)
 .br
 • Ordered Lists
 .br
 • Unordered Lists
 .br
-• Code\[em]Blocks
+• Code-Blocks
 .br
 • Inline
 .br
 .RS 2
 .br
 • Code
 .br
@@ -46,17 +46,17 @@
 .br
 • Emphasis
 .br
 • Links
 .br
 .br
 .RE
-• Images (rendered as braille\[em]art)
+• Images (rendered as braille-art)
 .br
-• Horizontal\[em]Rule
+• Horizontal-Rule
 .br
 .sp
 .SH "OPTIONS"
 .SS "\fBroff\fP \fIconvert\fP"
 .sp
 .RS 2
 Converts markdown files to roff files
@@ -81,15 +81,15 @@
 .sp
 Overwrite file if it exists
 .sp
 \fIdest\fP:
 .sp
 Target file that should be generated
 .SH "BUGS"
-https://github.com/utility\[em]toolbox/roff/issues
+https://github\.com/utility-toolbox/roff/issues
 .SH "AUTHOR"
-https://github.com/PlayerG9
+https://github\.com/PlayerG9
 .SH "SEE ALSO"
 .SS "Organisation:"
-https://github.com/utility\[em]toolbox
+https://github\.com/utility-toolbox
 .SS "Repository:"
-https://github.com/utility\[em]toolbox/roff
+https://github\.com/utility-toolbox/roff
```

### Comparing `roff-0.4.2/docs/roff.5` & `roff-0.4.3/docs/roff.5`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-.\" generated with roff/v0.4.0
-.\" https://pypi.org/project/roff/0.4.0
+.\" generated with roff/v0.4.2
+.\" https://pypi.org/project/roff/0.4.2
 .\" https://github.com/utility-toolbox/roff/
 .\"
 .TH "ROFF" "5" "30 April 2024" "github.com/utility-toolbox/roff"
 .SH "NAME"
 \fBroff\fP • python\[em]based cli to convert markdown to the roff (man\[em]pages) format
 .SH "DESCRIPTION"
 see roff(1) for more information about the CLI.
```

### Comparing `roff-0.4.2/setup.py` & `roff-0.4.3/setup.py`

 * *Files identical despite different names*

### Comparing `roff-0.4.2/src/roff/__cli__/template.py` & `roff-0.4.3/src/roff/__cli__/template.py`

 * *Files identical despite different names*

### Comparing `roff-0.4.2/src/roff/__cli__/util.py` & `roff-0.4.3/src/roff/__cli__/util.py`

 * *Files identical despite different names*

### Comparing `roff-0.4.2/src/roff/__init__.py` & `roff-0.4.3/src/roff/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,9 +27,9 @@
 __copyright__ = "Copyright 2024, utility-toolbox"
 __credits__ = ["PlayerG9"]
 __license__ = "MIT"
 __maintainer__ = "PlayerG9"
 __email__ = None
 __status__ = "Prototype"  # Prototype, Development, Production
 __description__ = "python-based cli to convert markdown to the roff (man-pages) format"
-__version_info__ = (0, 4, 2)
+__version_info__ = (0, 4, 3)
 __version__ = '.'.join(str(_) for _ in __version_info__)
```

### Comparing `roff-0.4.2/src/roff/__main__.py` & `roff-0.4.3/src/roff/__main__.py`

 * *Files identical despite different names*

### Comparing `roff-0.4.2/src/roff/_images.py` & `roff-0.4.3/src/roff/_images.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
     content_type = response.headers.get('content-type', None)
     if content_type is None:
         raise RuntimeError("missing content-type header")
     maintype, subtype = content_type.split('/', 1)
 
     if maintype != 'image':
         raise TypeError(f"unsupported content type: '{content_type}'")
-    if subtype == 'svg':
+    if subtype == 'svg+xml':
         if cairosvg is None:
             raise RuntimeError("svg-image rendering is not supported (`pip3 install roff[images-svg]`)")
         buffer = io.BytesIO()
         cairosvg.svg2png(file_obj=response, write_to=buffer, output_width=max_width)
         buffer.seek(0)
         response = buffer  # noqa
```

### Comparing `roff-0.4.2/src/roff/_markdown.py` & `roff-0.4.3/src/roff/_markdown.py`

 * *Files identical despite different names*

### Comparing `roff-0.4.2/src/roff/_util.py` & `roff-0.4.3/src/roff/_util.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,22 +15,22 @@
     parser = markdown_it.MarkdownIt()
     parser.use(markdown_plugin_command)
     return parser
 
 
 ESCAPE_RULES = {
     re.compile(r'\\'): r"\\\\",  # backslash
-    re.compile(r'\''): r"\[aq]",  # apostrophe
-    re.compile(r'\"'): r"\[dq]",  # double-quotation
-    re.compile(r'(?<=\d)-(?=\d)'): r"\[en]",  # en-dash
-    re.compile(r'(?<=\w)-(?=\w)'): r"\[em]",  # em-dash
-    re.compile(r'`'): r"\[ga]",  # grave accent
-    re.compile(r'\^'): r"\[ha]",  # circumflex accent
-    re.compile(r'~'): r"\[ti]",  # tilde
-    re.compile(r'-'): r"\-",  # minus sign
+    re.compile(r'\''): r"\\[aq]",  # apostrophe
+    re.compile(r'\"'): r"\\[dq]",  # double-quotation
+    re.compile(r'(?<=\d)-(?=\d)'): r"\\[en]",  # en-dash
+    re.compile(r'(?<=\w)-(?=\w)'): r"\\[em]",  # em-dash
+    re.compile(r'`'): r"\\[ga]",  # grave accent
+    re.compile(r'\^'): r"\\[ha]",  # circumflex accent
+    re.compile(r'~'): r"\\[ti]",  # tilde
+    re.compile(r'-'): r"\\-",  # minus sign
 }
 
 
 def escape(text: str) -> str:
     for rule, replacement in ESCAPE_RULES.items():
         text = rule.sub(replacement, text)
     return text
```

### Comparing `roff-0.4.2/src/roff/convert.py` & `roff-0.4.3/src/roff/convert.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 class Converter:
     _stream: io.StringIO
     _had_head: bool
     _fp: Path
     _root: Path
     manpage_area: int
 
+    # yes. I know that 80 won't fit the default terminal size of 80 because the section offset
     width: int = int(os.getenv('ROFF_WIDTH', 80))
     ascii: bool = os.getenv('ROFF_ASCII', "no").lower() in {"yes", "true", "1"}
 
     def __init__(self, fp: t.Union[str, os.PathLike]) -> None:
         self._stream = io.StringIO()
         self._had_head = False
         self._fp = Path(fp).absolute()
@@ -98,17 +99,17 @@
                 chunks.append(' ')
             elif child.type == 'hardbreak':
                 chunks.append('\n.br\n')
             elif child.type == 'link':
                 href = child.attrGet('href')
                 text = self._render_inline(node=child)
                 if href == text:
-                    chunks.append(escape(text))
+                    chunks.append(text)
                 else:
-                    chunks.append(f'\n.UR {href}\n{escape(text)}\n.UE')
+                    chunks.append(f'\n.UR {href}\n{text}\n.UE')
             elif child.type == 'image':
                 href = child.attrGet('src')
                 hyperref_re = re.compile(r'^\w+://')  # checks for http://, https://, data://, file://
                 if hyperref_re.match(href) is None:  # relative path to a file
                     href = f'file://{self._root.joinpath(href).absolute()}'  # make it absolute to our root directory
                 braille = render_image(url=href, max_dimensions=(self.width, self.width * 3))
                 content = textwrap.indent(braille, '.br\n')  # ensure line-wraps
@@ -187,24 +188,34 @@
     def _parse_p(self, node: markdown_it.tree.SyntaxTreeNode) -> None:
         content = self._render_inline(node=node.children[0])
         content = re.sub(r'\n{2,}', '\n.sp\n', content)
         # if node.level > 0:  # destroys the structure
         #     self._stream.write('.P\n')
         self._stream.write(f'{content}\n')
 
+    @staticmethod
+    def _check_newline(text: str) -> bool:
+        r""" checks the output of _render_inline if it won't fit into one line """
+        return (
+            # len(text) >= self.width  # won't fit in one line (good in theory. bad in praxis)
+            '\n.br\n' in text  # line-break
+            or '\n.sp\n' in text  # vertical space
+        )
+
     def _check_inline_text_list(self, node: markdown_it.tree.SyntaxTreeNode) -> bool:
         r""" Better do not touch this function. It's a mess. But at least it works """
         assert node.tag in {'ul', 'ol'}
         return all((
             (len(li.children)  # any children
              and li.children[0].type == 'paragraph'  # first is paragraph
              and len(li.children[0].children) == 1  # with one child
              and li.children[0].children[0].type == 'inline'  # which is inline
-             and '\n' not in self._render_inline(node=li.children[0].children[0]))  # and not over multiple lines
-            for li in node.children
+             and not self._check_newline(
+                        self._render_inline(node=li.children[0].children[0])  # and not over multiple lines
+            )) for li in node.children
         ))
 
     def _parse_ul(self, node: markdown_it.tree.SyntaxTreeNode) -> None:
         r""" unordered list """
         deep = node.level > 0
         self._stream.write('.br\n' if deep else '.sp\n')
         bullet = '*' if self.ascii else '•'
@@ -239,20 +250,30 @@
             for i, list_item in enumerate(node.children):
                 self._stream.write(f'{i+1}.\n.RS 2\n')
                 self._parse_children(children=list_item.children)
                 self._stream.write(f'.RE\n')
         self._stream.write('.br\n' if deep else '.sp\n')
 
     def _parse_blockquote(self, node: markdown_it.tree.SyntaxTreeNode) -> None:
+        # todo: prefix each line with '|' somehow
         self._stream.write(f'.sp\n.RS 2\n')
         self._parse_children(children=node.children)
         self._stream.write(f'.RE\n.sp\n')
 
     def _parse_code(self, node: markdown_it.tree.SyntaxTreeNode) -> None:
-        content = re.sub(r'\n{2,}', '\n.sp\n', node.content.expandtabs(4).strip())
+        content = node.content.expandtabs(4).strip()
         content = textwrap.dedent(content)  # left-align
-        content = textwrap.indent(content, prefix='.br\n')  # ensures newlines
-        self._stream.write(f'.sp\n.RS 2\n.EX\n\\fI\n{content}\n\\fP\n.EE\n.RE\n.sp\n')
+        if node.info in {'', 'text', 'txt'}:  # print with left-offset
+            content = re.sub(r'\n{2,}', '\n.sp\n', escape(content))
+            content = textwrap.indent(content, prefix='.br\n')  # ensures newlines
+            self._stream.write(f'.sp\n.RS 2\n.EX\n\\fI\n{content}\n\\fP\n.EE\n.RE\n.sp\n')
+        else:  # prints with line-numbers
+            self._stream.write(f'.sp\n')
+            lines = content.splitlines()
+            num_width = len(lines) // 10
+            for i, line in enumerate(lines):
+                self._stream.write(f'{str(i+1).rjust(num_width)} | \\fI{escape(line)}\\fP\n.br\n')
+            self._stream.write(f'.sp\n')
 
     def _parse_hr(self, _node: markdown_it.tree.SyntaxTreeNode) -> None:
         character = "-" if self.ascii else "━"
         self._stream.write(f".sp\n{character * self.width}\n.sp\n")
```

### Comparing `roff-0.4.2/src/roff.egg-info/PKG-INFO` & `roff-0.4.3/src/roff.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roff
-Version: 0.4.2
+Version: 0.4.3
 Summary: python-based cli to convert markdown to the roff (man-pages) format
 Home-page: https://github.com/utility-toolbox/roff
 Author: PlayerG9
 License: MIT
 Project-URL: Organisation Github, https://github.com/utility-toolbox
 Project-URL: Homepage, https://github.com/utility-toolbox/roff/
 Project-URL: Bug Tracker, https://github.com/utility-toolbox/roff/issues
```

### Comparing `roff-0.4.2/src/roff.egg-info/SOURCES.txt` & `roff-0.4.3/src/roff.egg-info/SOURCES.txt`

 * *Files identical despite different names*

