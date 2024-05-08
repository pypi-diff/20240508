# Comparing `tmp/pybib2web-0.5.1.tar.gz` & `tmp/pybib2web-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybib2web-0.5.1.tar", last modified: Mon Jul  3 15:01:36 2023, max compression
+gzip compressed data, was "pybib2web-0.6.tar", last modified: Wed May  8 17:07:54 2024, max compression
```

## Comparing `pybib2web-0.5.1.tar` & `pybib2web-0.6.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 15:01:36.251294 pybib2web-0.5.1/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 15:01:36.247294 pybib2web-0.5.1/LICENSES/
--rw-rw-rw-   0 root         (0) root         (0)    11358 2023-06-25 02:17:30.000000 pybib2web-0.5.1/LICENSES/Apache-2.0.txt
--rw-r--r--   0 root         (0) root         (0)     3238 2023-07-03 15:01:36.251294 pybib2web-0.5.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2370 2023-06-25 02:17:30.000000 pybib2web-0.5.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 15:01:36.247294 pybib2web-0.5.1/pybib2web/
--rw-rw-rw-   0 root         (0) root         (0)     2589 2023-06-25 02:17:30.000000 pybib2web-0.5.1/pybib2web/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1412 2023-06-25 02:17:30.000000 pybib2web-0.5.1/pybib2web/bibexport.py
--rw-rw-rw-   0 root         (0) root         (0)     3435 2023-06-25 02:17:30.000000 pybib2web-0.5.1/pybib2web/bibparser.py
--rw-rw-rw-   0 root         (0) root         (0)     6128 2023-06-25 02:17:30.000000 pybib2web-0.5.1/pybib2web/categories.py
--rw-rw-rw-   0 root         (0) root         (0)     1786 2023-06-25 02:17:30.000000 pybib2web-0.5.1/pybib2web/config.py
--rw-rw-rw-   0 root         (0) root         (0)    29638 2023-07-03 14:48:12.000000 pybib2web-0.5.1/pybib2web/htmlexport.py
--rw-rw-rw-   0 root         (0) root         (0)     2657 2023-06-25 02:17:30.000000 pybib2web-0.5.1/pybib2web/util.py
--rw-rw-rw-   0 root         (0) root         (0)      249 2023-07-03 14:53:09.000000 pybib2web-0.5.1/pybib2web/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 15:01:36.251294 pybib2web-0.5.1/pybib2web.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3238 2023-07-03 15:01:36.000000 pybib2web-0.5.1/pybib2web.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      529 2023-07-03 15:01:36.000000 pybib2web-0.5.1/pybib2web.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 15:01:36.000000 pybib2web-0.5.1/pybib2web.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       45 2023-07-03 15:01:36.000000 pybib2web-0.5.1/pybib2web.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       30 2023-07-03 15:01:36.000000 pybib2web-0.5.1/pybib2web.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-07-03 15:01:36.000000 pybib2web-0.5.1/pybib2web.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 15:01:36.000000 pybib2web-0.5.1/pybib2web.egg-info/zip-safe
--rw-rw-rw-   0 root         (0) root         (0)      378 2023-06-25 02:17:30.000000 pybib2web-0.5.1/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1353 2023-07-03 15:01:36.251294 pybib2web-0.5.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 15:01:36.251294 pybib2web-0.5.1/tests/
--rw-rw-rw-   0 root         (0) root         (0)     2016 2023-06-25 02:17:30.000000 pybib2web-0.5.1/tests/test_bibparser.py
--rw-rw-rw-   0 root         (0) root         (0)      860 2023-06-25 02:17:30.000000 pybib2web-0.5.1/tests/test_htmlexport.py
--rw-rw-rw-   0 root         (0) root         (0)     2315 2023-06-25 02:17:30.000000 pybib2web-0.5.1/tests/test_util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 17:07:54.345941 pybib2web-0.6/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 17:07:54.337941 pybib2web-0.6/LICENSES/
+-rw-rw-rw-   0 root         (0) root         (0)    11358 2024-03-17 03:09:33.000000 pybib2web-0.6/LICENSES/Apache-2.0.txt
+-rw-r--r--   0 root         (0) root         (0)     3296 2024-05-08 17:07:54.345941 pybib2web-0.6/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2370 2024-03-17 03:09:33.000000 pybib2web-0.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 17:07:54.341941 pybib2web-0.6/pybib2web/
+-rw-rw-rw-   0 root         (0) root         (0)     2589 2024-03-17 03:09:33.000000 pybib2web-0.6/pybib2web/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1412 2024-03-17 03:09:33.000000 pybib2web-0.6/pybib2web/bibexport.py
+-rw-rw-rw-   0 root         (0) root         (0)     4464 2024-05-08 16:41:12.000000 pybib2web-0.6/pybib2web/bibparser.py
+-rw-rw-rw-   0 root         (0) root         (0)     6128 2024-03-17 03:09:33.000000 pybib2web-0.6/pybib2web/categories.py
+-rw-rw-rw-   0 root         (0) root         (0)     1786 2024-03-17 03:09:33.000000 pybib2web-0.6/pybib2web/config.py
+-rw-rw-rw-   0 root         (0) root         (0)    29739 2024-05-08 16:56:54.000000 pybib2web-0.6/pybib2web/htmlexport.py
+-rw-rw-rw-   0 root         (0) root         (0)     2657 2024-03-17 03:09:33.000000 pybib2web-0.6/pybib2web/util.py
+-rw-rw-rw-   0 root         (0) root         (0)      247 2024-05-08 17:00:31.000000 pybib2web-0.6/pybib2web/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 17:07:54.345941 pybib2web-0.6/pybib2web.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3296 2024-05-08 17:07:54.000000 pybib2web-0.6/pybib2web.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      529 2024-05-08 17:07:54.000000 pybib2web-0.6/pybib2web.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-08 17:07:54.000000 pybib2web-0.6/pybib2web.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       45 2024-05-08 17:07:54.000000 pybib2web-0.6/pybib2web.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       30 2024-05-08 17:07:54.000000 pybib2web-0.6/pybib2web.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2024-05-08 17:07:54.000000 pybib2web-0.6/pybib2web.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-08 17:07:54.000000 pybib2web-0.6/pybib2web.egg-info/zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)      378 2024-03-17 03:09:33.000000 pybib2web-0.6/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1353 2024-05-08 17:07:54.345941 pybib2web-0.6/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 17:07:54.341941 pybib2web-0.6/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     2016 2024-03-17 03:09:33.000000 pybib2web-0.6/tests/test_bibparser.py
+-rw-rw-rw-   0 root         (0) root         (0)      860 2024-03-17 03:09:33.000000 pybib2web-0.6/tests/test_htmlexport.py
+-rw-rw-rw-   0 root         (0) root         (0)     2315 2024-03-17 03:09:33.000000 pybib2web-0.6/tests/test_util.py
```

### Comparing `pybib2web-0.5.1/LICENSES/Apache-2.0.txt` & `pybib2web-0.6/LICENSES/Apache-2.0.txt`

 * *Files identical despite different names*

### Comparing `pybib2web-0.5.1/PKG-INFO` & `pybib2web-0.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybib2web
-Version: 0.5.1
+Version: 0.6
 Summary: A translator of BibTeX to HTML.
 Home-page: https://gitlab.com/sosy-lab/software/pybib2web
 Author: Dirk Beyer
 Author-email: dirk.beyer@sosy-lab.org
 License: Apache-2.0
 Project-URL: Changelog, https://gitlab.com/sosy-lab/software/pybib2web/-/blob/main/CHANGELOG.md
 Project-URL: Issue Tracker, https://gitlab.com/sosy-lab/software/pybib2web/-/issues
@@ -14,14 +14,16 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Text Processing :: Markup :: LaTeX
 Description-Content-Type: text/markdown
 License-File: LICENSES/Apache-2.0.txt
+Requires-Dist: bibtexparser>=1.2
+Requires-Dist: PyYAML>=5.3
 
 <!--
 This file is part of pybib2web, a translator of BibTeX to HTML.
 https://gitlab.com/sosy-lab/software/pybib2web
 
 SPDX-FileCopyrightText: 2021 Dirk Beyer <https://www.sosy-lab.org>
```

### Comparing `pybib2web-0.5.1/README.md` & `pybib2web-0.6/README.md`

 * *Files identical despite different names*

### Comparing `pybib2web-0.5.1/pybib2web/__init__.py` & `pybib2web-0.6/pybib2web/__init__.py`

 * *Files identical despite different names*

### Comparing `pybib2web-0.5.1/pybib2web/bibexport.py` & `pybib2web-0.6/pybib2web/bibexport.py`

 * *Files identical despite different names*

### Comparing `pybib2web-0.5.1/pybib2web/bibparser.py` & `pybib2web-0.6/pybib2web/bibparser.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,30 @@
 # This file is part of pybib2web, a translator of BibTeX to HTML.
 # https://gitlab.com/sosy-lab/software/pybib2web
 #
 # SPDX-FileCopyrightText: 2021 Dirk Beyer <https://www.sosy-lab.org>
 #
 # SPDX-License-Identifier: Apache-2.0
-
+import itertools
 import logging
 import os
 import re
 import subprocess
 
 import bibtexparser
 from bibtexparser.bparser import BibTexParser
 from bibtexparser.customization import convert_to_unicode, keyword
 
+from bibtexparser.latexenc import (
+    _replace_all_latex,
+    unicode_to_crappy_latex1,
+    unicode_to_latex,
+    unicode_to_crappy_latex2,
+)
+
 from . import util
 
 
 def parse(*files, do_detex=True) -> bibtexparser.bibdatabase.BibDatabase:
     def concat_files(files):
         concatenated_content = b""
         for f in files:
@@ -29,28 +36,51 @@
     parser.customization = get_customization_func(
         do_detex=do_detex, add_pdf_for_doi=True
     )
     parser.ignore_nonstandard_types = False
     return bibtexparser.loads(concat_files(files), parser=parser)
 
 
+def convert_characters_to_unicode(record):
+    """
+    Converts LaTeX representations of special characters to unicode.
+
+    This is a customied version of convert_to_unicode that does not remove curly braces.
+
+    :param record: the record.
+    :type record: dict
+    :returns: dict -- the modified record.
+    """
+    for val in record:
+        record[val] = _replace_all_latex(
+            record[val], itertools.chain(unicode_to_crappy_latex1, unicode_to_latex)
+        )
+        record[val] = _replace_all_latex(record[val], unicode_to_crappy_latex2)
+    return record
+
+
 def get_customization_func(*, do_detex: bool, add_pdf_for_doi: bool):
     if do_detex and not _which("detex"):
         logging.warning(
             "No executable 'detex' found on system. Not detexifying publication titles"
         )
         do_detex = False
 
     def customize(entry):
         copy = dict(entry.items())
 
         entry = {k: v for k, v in entry.items() if v.strip()}
-        entry = convert_to_unicode(keyword(entry))
+
+        # The following customized version of convert_to_unicode does not remove curly braces.
+        entry = convert_characters_to_unicode(entry)
+        # do remaining LaTeX normalization
         if do_detex:
             entry = detex(entry)
+        # Do remaining normalization of LaTeX (must be done after detex as it removes curly braces)
+        entry = convert_to_unicode(keyword(entry))
         if add_pdf_for_doi:
             entry = add_pdf(entry)
         entry = split_lists(entry)
         entry["original"] = copy
         return entry
 
     return customize
```

### Comparing `pybib2web-0.5.1/pybib2web/categories.py` & `pybib2web-0.6/pybib2web/categories.py`

 * *Files identical despite different names*

### Comparing `pybib2web-0.5.1/pybib2web/config.py` & `pybib2web-0.6/pybib2web/config.py`

 * *Files identical despite different names*

### Comparing `pybib2web-0.5.1/pybib2web/htmlexport.py` & `pybib2web-0.6/pybib2web/htmlexport.py`

 * *Files 1% similar despite different names*

```diff
@@ -546,28 +546,30 @@
     config,
     head=None,
     header_title=None,
 ) -> str:
     def gen():
         if head:
             yield head
+        next_start_index = 1
         for category, entries in categorized_entries.items():
             if category.link:
                 yield internal_link(
                     f"<h3>{category.name}</h3>", f"../{category.link}", config
                 )
             else:
                 yield f"<h3>{category.name}</h3>"
             yield ""
-            yield f'<ol class="list-{header_title.lower().replace(" ", "-")}">'
+            yield f'<ol class="list-{header_title.lower().replace(" ", "-")}" start="{next_start_index}">'
             yield ""
             for entry in entries:
                 yield to_html(entry, config=config)
                 yield ""
             yield "</ol>"
+            next_start_index += len(entries)
         tail = config.tail
         if tail:
             yield tail
 
     return "\n".join(gen())
```

### Comparing `pybib2web-0.5.1/pybib2web/util.py` & `pybib2web-0.6/pybib2web/util.py`

 * *Files identical despite different names*

### Comparing `pybib2web-0.5.1/pybib2web.egg-info/PKG-INFO` & `pybib2web-0.6/pybib2web.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybib2web
-Version: 0.5.1
+Version: 0.6
 Summary: A translator of BibTeX to HTML.
 Home-page: https://gitlab.com/sosy-lab/software/pybib2web
 Author: Dirk Beyer
 Author-email: dirk.beyer@sosy-lab.org
 License: Apache-2.0
 Project-URL: Changelog, https://gitlab.com/sosy-lab/software/pybib2web/-/blob/main/CHANGELOG.md
 Project-URL: Issue Tracker, https://gitlab.com/sosy-lab/software/pybib2web/-/issues
@@ -14,14 +14,16 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Text Processing :: Markup :: LaTeX
 Description-Content-Type: text/markdown
 License-File: LICENSES/Apache-2.0.txt
+Requires-Dist: bibtexparser>=1.2
+Requires-Dist: PyYAML>=5.3
 
 <!--
 This file is part of pybib2web, a translator of BibTeX to HTML.
 https://gitlab.com/sosy-lab/software/pybib2web
 
 SPDX-FileCopyrightText: 2021 Dirk Beyer <https://www.sosy-lab.org>
```

### Comparing `pybib2web-0.5.1/pybib2web.egg-info/SOURCES.txt` & `pybib2web-0.6/pybib2web.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pybib2web-0.5.1/setup.cfg` & `pybib2web-0.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `pybib2web-0.5.1/tests/test_bibparser.py` & `pybib2web-0.6/tests/test_bibparser.py`

 * *Files identical despite different names*

### Comparing `pybib2web-0.5.1/tests/test_htmlexport.py` & `pybib2web-0.6/tests/test_htmlexport.py`

 * *Files identical despite different names*

### Comparing `pybib2web-0.5.1/tests/test_util.py` & `pybib2web-0.6/tests/test_util.py`

 * *Files identical despite different names*

