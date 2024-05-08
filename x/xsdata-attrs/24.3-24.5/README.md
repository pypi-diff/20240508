# Comparing `tmp/xsdata_attrs-24.3.tar.gz` & `tmp/xsdata_attrs-24.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xsdata_attrs-24.3.tar", last modified: Sun Mar 10 14:31:06 2024, max compression
+gzip compressed data, was "xsdata_attrs-24.5.tar", last modified: Wed May  8 17:20:12 2024, max compression
```

## Comparing `xsdata_attrs-24.3.tar` & `xsdata_attrs-24.5.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 14:31:06.322114 xsdata_attrs-24.3/
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-03-10 14:31:01.000000 xsdata_attrs-24.3/CHANGES.md
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-03-10 14:31:01.000000 xsdata_attrs-24.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-03-10 14:31:01.000000 xsdata_attrs-24.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4697 2024-03-10 14:31:06.322114 xsdata_attrs-24.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-03-10 14:31:01.000000 xsdata_attrs-24.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 14:31:06.314113 xsdata_attrs-24.3/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-03-10 14:31:01.000000 xsdata_attrs-24.3/docs/bindings.md
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-03-10 14:31:01.000000 xsdata_attrs-24.3/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-03-10 14:31:01.000000 xsdata_attrs-24.3/docs/codegen.md
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-03-10 14:31:01.000000 xsdata_attrs-24.3/docs/favicon.png
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-03-10 14:31:01.000000 xsdata_attrs-24.3/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-03-10 14:31:01.000000 xsdata_attrs-24.3/docs/installation.md
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-03-10 14:31:01.000000 xsdata_attrs-24.3/docs/logo-small.svg
--rw-r--r--   0 runner    (1001) docker     (127)     5535 2024-03-10 14:31:01.000000 xsdata_attrs-24.3/docs/logo.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 14:31:06.314113 xsdata_attrs-24.3/docs/overrides/
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-03-10 14:31:01.000000 xsdata_attrs-24.3/docs/overrides/main.html
--rw-r--r--   0 runner    (1001) docker     (127)     2430 2024-03-10 14:31:01.000000 xsdata_attrs-24.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-10 14:31:06.322114 xsdata_attrs-24.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 14:31:06.314113 xsdata_attrs-24.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-10 14:31:01.000000 xsdata_attrs-24.3/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 14:31:06.314113 xsdata_attrs-24.3/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-10 14:31:01.000000 xsdata_attrs-24.3/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-03-10 14:31:01.000000 xsdata_attrs-24.3/tests/fixtures/attrs.conf.xml
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-03-10 14:31:01.000000 xsdata_attrs-24.3/tests/fixtures/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 14:31:06.314113 xsdata_attrs-24.3/tests/fixtures/po/
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-03-10 14:31:01.000000 xsdata_attrs-24.3/tests/fixtures/po/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4052 2024-03-10 14:31:01.000000 xsdata_attrs-24.3/tests/fixtures/po/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 14:31:06.314113 xsdata_attrs-24.3/tests/fixtures/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-03-10 14:31:01.000000 xsdata_attrs-24.3/tests/fixtures/schemas/po.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     3385 2024-03-10 14:31:01.000000 xsdata_attrs-24.3/tests/test_bindings.py
--rw-r--r--   0 runner    (1001) docker     (127)     2743 2024-03-10 14:31:01.000000 xsdata_attrs-24.3/tests/test_compat.py
--rw-r--r--   0 runner    (1001) docker     (127)     3890 2024-03-10 14:31:01.000000 xsdata_attrs-24.3/tests/test_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 14:31:06.318114 xsdata_attrs-24.3/xsdata_attrs/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-10 14:31:01.000000 xsdata_attrs-24.3/xsdata_attrs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4173 2024-03-10 14:31:01.000000 xsdata_attrs-24.3/xsdata_attrs/bindings.py
--rw-r--r--   0 runner    (1001) docker     (127)     3570 2024-03-10 14:31:01.000000 xsdata_attrs-24.3/xsdata_attrs/compat.py
--rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-03-10 14:31:01.000000 xsdata_attrs-24.3/xsdata_attrs/generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 14:31:06.318114 xsdata_attrs-24.3/xsdata_attrs/hooks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-10 14:31:01.000000 xsdata_attrs-24.3/xsdata_attrs/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-03-10 14:31:01.000000 xsdata_attrs-24.3/xsdata_attrs/hooks/class_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-03-10 14:31:01.000000 xsdata_attrs-24.3/xsdata_attrs/hooks/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-10 14:31:01.000000 xsdata_attrs-24.3/xsdata_attrs/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 14:31:06.318114 xsdata_attrs-24.3/xsdata_attrs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4697 2024-03-10 14:31:06.000000 xsdata_attrs-24.3/xsdata_attrs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-03-10 14:31:06.000000 xsdata_attrs-24.3/xsdata_attrs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-10 14:31:06.000000 xsdata_attrs-24.3/xsdata_attrs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-03-10 14:31:06.000000 xsdata_attrs-24.3/xsdata_attrs.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-03-10 14:31:06.000000 xsdata_attrs-24.3/xsdata_attrs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-10 14:31:06.000000 xsdata_attrs-24.3/xsdata_attrs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:20:12.308046 xsdata_attrs-24.5/
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-08 17:20:08.000000 xsdata_attrs-24.5/CHANGES.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-08 17:20:08.000000 xsdata_attrs-24.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-08 17:20:08.000000 xsdata_attrs-24.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4661 2024-05-08 17:20:12.308046 xsdata_attrs-24.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-05-08 17:20:08.000000 xsdata_attrs-24.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:20:12.304046 xsdata_attrs-24.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-05-08 17:20:08.000000 xsdata_attrs-24.5/docs/bindings.md
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-08 17:20:08.000000 xsdata_attrs-24.5/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-08 17:20:08.000000 xsdata_attrs-24.5/docs/codegen.md
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-08 17:20:08.000000 xsdata_attrs-24.5/docs/favicon.png
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-05-08 17:20:08.000000 xsdata_attrs-24.5/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-08 17:20:08.000000 xsdata_attrs-24.5/docs/installation.md
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-05-08 17:20:08.000000 xsdata_attrs-24.5/docs/logo-small.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     5535 2024-05-08 17:20:08.000000 xsdata_attrs-24.5/docs/logo.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:20:12.304046 xsdata_attrs-24.5/docs/overrides/
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-08 17:20:08.000000 xsdata_attrs-24.5/docs/overrides/main.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2430 2024-05-08 17:20:08.000000 xsdata_attrs-24.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 17:20:12.308046 xsdata_attrs-24.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:20:12.304046 xsdata_attrs-24.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 17:20:08.000000 xsdata_attrs-24.5/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:20:12.304046 xsdata_attrs-24.5/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 17:20:08.000000 xsdata_attrs-24.5/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-05-08 17:20:08.000000 xsdata_attrs-24.5/tests/fixtures/attrs.conf.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-08 17:20:08.000000 xsdata_attrs-24.5/tests/fixtures/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:20:12.304046 xsdata_attrs-24.5/tests/fixtures/po/
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-08 17:20:08.000000 xsdata_attrs-24.5/tests/fixtures/po/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4052 2024-05-08 17:20:08.000000 xsdata_attrs-24.5/tests/fixtures/po/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:20:12.304046 xsdata_attrs-24.5/tests/fixtures/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-05-08 17:20:08.000000 xsdata_attrs-24.5/tests/fixtures/schemas/po.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-05-08 17:20:08.000000 xsdata_attrs-24.5/tests/test_bindings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2743 2024-05-08 17:20:08.000000 xsdata_attrs-24.5/tests/test_compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-08 17:20:08.000000 xsdata_attrs-24.5/tests/test_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:20:12.304046 xsdata_attrs-24.5/xsdata_attrs/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-08 17:20:08.000000 xsdata_attrs-24.5/xsdata_attrs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4173 2024-05-08 17:20:08.000000 xsdata_attrs-24.5/xsdata_attrs/bindings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3570 2024-05-08 17:20:08.000000 xsdata_attrs-24.5/xsdata_attrs/compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-05-08 17:20:08.000000 xsdata_attrs-24.5/xsdata_attrs/generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:20:12.308046 xsdata_attrs-24.5/xsdata_attrs/hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 17:20:08.000000 xsdata_attrs-24.5/xsdata_attrs/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-08 17:20:08.000000 xsdata_attrs-24.5/xsdata_attrs/hooks/class_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-08 17:20:08.000000 xsdata_attrs-24.5/xsdata_attrs/hooks/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 17:20:08.000000 xsdata_attrs-24.5/xsdata_attrs/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:20:12.308046 xsdata_attrs-24.5/xsdata_attrs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4661 2024-05-08 17:20:12.000000 xsdata_attrs-24.5/xsdata_attrs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-05-08 17:20:12.000000 xsdata_attrs-24.5/xsdata_attrs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 17:20:12.000000 xsdata_attrs-24.5/xsdata_attrs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-08 17:20:12.000000 xsdata_attrs-24.5/xsdata_attrs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-08 17:20:12.000000 xsdata_attrs-24.5/xsdata_attrs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-08 17:20:12.000000 xsdata_attrs-24.5/xsdata_attrs.egg-info/top_level.txt
```

### Comparing `xsdata_attrs-24.3/LICENSE` & `xsdata_attrs-24.5/LICENSE`

 * *Files identical despite different names*

### Comparing `xsdata_attrs-24.3/PKG-INFO` & `xsdata_attrs-24.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xsdata_attrs
-Version: 24.3
+Version: 24.5
 Summary: xsdata attrs plugin
 Author-email: Christodoulos Tsoulloftas <chris@komposta.net>
 License: MIT
 Project-URL: Homepage, https://github.com/tefra/xsdata-attrs
 Project-URL: Source, https://github.com/tefra/xsdata-attrs
 Project-URL: Documentation, https://xsdata-attrs.readthedocs.io/
 Project-URL: Changelog, https://xsdata-attrs.readthedocs.io/en/latest/changelog/
@@ -24,15 +24,15 @@
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Code Generators
 Classifier: Topic :: Text Processing :: Markup :: XML
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: attrs>=19.2.0
-Requires-Dist: xsdata>=24.3
+Requires-Dist: xsdata>=24.5
 Provides-Extra: cli
 Requires-Dist: xsdata[cli]>=23.5; extra == "cli"
 Provides-Extra: docs
 Requires-Dist: mkdocs; extra == "docs"
 Requires-Dist: mkdocs-gen-files; extra == "docs"
 Requires-Dist: mkdocs-literate-nav; extra == "docs"
 Requires-Dist: mkdocs-material; extra == "docs"
@@ -114,11 +114,10 @@
 >>> result.channel.item[2].pub_date
 'Sat, 03 Jul 2021 16:37:14 GMT'
 >>> result.channel.item[2].link
 'https://www.cnn.com/2021/07/03/europe/vatican-financial-scandal-intl/index.html'
 
 ```
 
-## Changelog: 24.3 (2024-03-10)
+## Changelog: 24.5 (2024-05-08)
 
-- Add missing parser/serializer shortcuts
-- General project maintenance
+- Bump xsdata minimum version v24.5
```

### Comparing `xsdata_attrs-24.3/README.md` & `xsdata_attrs-24.5/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -61,11 +61,10 @@
 >>> result.channel.item[2].pub_date
 'Sat, 03 Jul 2021 16:37:14 GMT'
 >>> result.channel.item[2].link
 'https://www.cnn.com/2021/07/03/europe/vatican-financial-scandal-intl/index.html'
 
 ```
 
-## Changelog: 24.3 (2024-03-10)
+## Changelog: 24.5 (2024-05-08)
 
-- Add missing parser/serializer shortcuts
-- General project maintenance
+- Bump xsdata minimum version v24.5
```

### Comparing `xsdata_attrs-24.3/docs/bindings.md` & `xsdata_attrs-24.5/docs/bindings.md`

 * *Files identical despite different names*

### Comparing `xsdata_attrs-24.3/docs/codegen.md` & `xsdata_attrs-24.5/docs/codegen.md`

 * *Files identical despite different names*

### Comparing `xsdata_attrs-24.3/docs/logo-small.svg` & `xsdata_attrs-24.5/docs/logo-small.svg`

 * *Files identical despite different names*

### Comparing `xsdata_attrs-24.3/docs/logo.svg` & `xsdata_attrs-24.5/docs/logo.svg`

 * *Files identical despite different names*

### Comparing `xsdata_attrs-24.3/pyproject.toml` & `xsdata_attrs-24.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     "Topic :: Software Development :: Code Generators",
     "Topic :: Text Processing :: Markup :: XML",
 ]
 keywords = ["xsd", "wsdl", "schema", "dtd", "binding", "xml", "json", "dataclasses", "generator", "cli", "attrs"]
 requires-python = ">=3.8"
 dependencies = [
     "attrs>=19.2.0",
-    "xsdata>=24.3",
+    "xsdata>=24.5",
 ]
 dynamic = ["version"]
 
 [project.readme]
 file = "README.md"
 content-type = "text/markdown"
```

### Comparing `xsdata_attrs-24.3/tests/fixtures/attrs.conf.xml` & `xsdata_attrs-24.5/tests/fixtures/attrs.conf.xml`

 * *Files identical despite different names*

### Comparing `xsdata_attrs-24.3/tests/fixtures/po/models.py` & `xsdata_attrs-24.5/tests/fixtures/po/models.py`

 * *Files identical despite different names*

### Comparing `xsdata_attrs-24.3/tests/fixtures/schemas/po.xsd` & `xsdata_attrs-24.5/tests/fixtures/schemas/po.xsd`

 * *Files identical despite different names*

### Comparing `xsdata_attrs-24.3/tests/test_bindings.py` & `xsdata_attrs-24.5/tests/test_bindings.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 from datetime import datetime
 from unittest import TestCase
 
-from xsdata.formats.dataclass.serializers.config import SerializerConfig
 
 from tests.fixtures.common import TypeC
-from xsdata_attrs.bindings import JsonParser
-from xsdata_attrs.bindings import JsonSerializer
 from xsdata_attrs.bindings import XmlParser
 from xsdata_attrs.bindings import XmlSerializer
 from xsdata_attrs.compat import AnyElement
 from xsdata_attrs.compat import DerivedElement
 
 
 class BindingsTests(TestCase):
@@ -51,50 +48,7 @@
             "  <foo>bar</foo>\n"
             '  <bar xsi:type="xs:string">1</bar>\n'
             '  <bar xsi:type="xs:short">2</bar>\n'
             "</TypeC>\n"
         )
         self.assertEqual(expected, serializer.render(self.obj, ns_map))
         self.assertEqual(self.obj, parser.from_string(expected))
-
-    def test_serialize_json(self):
-        serializer = JsonSerializer(config=SerializerConfig(indent="  "))
-        parser = JsonParser()
-
-        expected = (
-            "{\n"
-            '  "one": "first",\n'
-            '  "two": 1.1,\n'
-            '  "three": true,\n'
-            '  "four": [\n'
-            '    "01 January 2002 12:01",\n'
-            '    "05 February 2003 13:05"\n'
-            "  ],\n"
-            '  "any": {\n'
-            '    "qname": null,\n'
-            '    "text": null,\n'
-            '    "tail": null,\n'
-            '    "children": [\n'
-            "      {\n"
-            '        "qname": "foo",\n'
-            '        "text": "bar",\n'
-            '        "tail": null,\n'
-            '        "children": [],\n'
-            '        "attributes": {}\n'
-            "      },\n"
-            "      {\n"
-            '        "qname": "bar",\n'
-            '        "value": "1",\n'
-            '        "type": null\n'
-            "      },\n"
-            "      {\n"
-            '        "qname": "bar",\n'
-            '        "value": 2,\n'
-            '        "type": null\n'
-            "      }\n"
-            "    ],\n"
-            '    "attributes": {}\n'
-            "  }\n"
-            "}"
-        )
-        self.assertEqual(expected, serializer.render(self.obj))
-        self.assertEqual(self.obj, parser.from_string(expected, TypeC))
```

### Comparing `xsdata_attrs-24.3/tests/test_compat.py` & `xsdata_attrs-24.5/tests/test_compat.py`

 * *Files identical despite different names*

### Comparing `xsdata_attrs-24.3/xsdata_attrs/bindings.py` & `xsdata_attrs-24.5/xsdata_attrs/bindings.py`

 * *Files identical despite different names*

### Comparing `xsdata_attrs-24.3/xsdata_attrs/compat.py` & `xsdata_attrs-24.5/xsdata_attrs/compat.py`

 * *Files identical despite different names*

### Comparing `xsdata_attrs-24.3/xsdata_attrs/generator.py` & `xsdata_attrs-24.5/xsdata_attrs/generator.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from typing import Dict
-from typing import List
 from typing import Optional
 
-from xsdata.codegen.models import Attr
+from xsdata.codegen.models import Attr, Class
 from xsdata.formats.dataclass.filters import Filters
 from xsdata.formats.dataclass.generator import DataclassGenerator
 from xsdata.models.config import GeneratorConfig
 from xsdata.models.config import OutputFormat
 
 
 class AttrsGenerator(DataclassGenerator):
@@ -36,21 +35,20 @@
         result = super().build_class_annotation(format)
         result = result.replace("unsafe_hash=", "hash=")
         result = result.replace("@dataclass", "@attr.s")
         return result
 
     def field_definition(
         self,
+        obj: Class,
         attr: Attr,
-        ns_map: Dict,
         parent_namespace: Optional[str],
-        parents: List[str],
     ) -> str:
         """Return the field definition with any extra metadata."""
-        result = super().field_definition(attr, ns_map, parent_namespace, parents)
+        result = super().field_definition(obj, attr, parent_namespace)
         return result.replace("field(", "attr.ib(")
 
     @classmethod
     def build_import_patterns(cls) -> Dict[str, Dict]:
         """Build import search patterns."""
         patterns = {"attr": {"__module__": [" attr.ib", "@attr.s"]}}
         patterns.update(super().build_import_patterns())
```

### Comparing `xsdata_attrs-24.3/xsdata_attrs.egg-info/PKG-INFO` & `xsdata_attrs-24.5/xsdata_attrs.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xsdata_attrs
-Version: 24.3
+Version: 24.5
 Summary: xsdata attrs plugin
 Author-email: Christodoulos Tsoulloftas <chris@komposta.net>
 License: MIT
 Project-URL: Homepage, https://github.com/tefra/xsdata-attrs
 Project-URL: Source, https://github.com/tefra/xsdata-attrs
 Project-URL: Documentation, https://xsdata-attrs.readthedocs.io/
 Project-URL: Changelog, https://xsdata-attrs.readthedocs.io/en/latest/changelog/
@@ -24,15 +24,15 @@
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Code Generators
 Classifier: Topic :: Text Processing :: Markup :: XML
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: attrs>=19.2.0
-Requires-Dist: xsdata>=24.3
+Requires-Dist: xsdata>=24.5
 Provides-Extra: cli
 Requires-Dist: xsdata[cli]>=23.5; extra == "cli"
 Provides-Extra: docs
 Requires-Dist: mkdocs; extra == "docs"
 Requires-Dist: mkdocs-gen-files; extra == "docs"
 Requires-Dist: mkdocs-literate-nav; extra == "docs"
 Requires-Dist: mkdocs-material; extra == "docs"
@@ -114,11 +114,10 @@
 >>> result.channel.item[2].pub_date
 'Sat, 03 Jul 2021 16:37:14 GMT'
 >>> result.channel.item[2].link
 'https://www.cnn.com/2021/07/03/europe/vatican-financial-scandal-intl/index.html'
 
 ```
 
-## Changelog: 24.3 (2024-03-10)
+## Changelog: 24.5 (2024-05-08)
 
-- Add missing parser/serializer shortcuts
-- General project maintenance
+- Bump xsdata minimum version v24.5
```

### Comparing `xsdata_attrs-24.3/xsdata_attrs.egg-info/SOURCES.txt` & `xsdata_attrs-24.5/xsdata_attrs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

