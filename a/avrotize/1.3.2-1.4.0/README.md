# Comparing `tmp/avrotize-1.3.2.tar.gz` & `tmp/avrotize-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avrotize-1.3.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "avrotize-1.4.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `avrotize-1.3.2.tar` & `avrotize-1.4.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0    26753 2024-04-28 10:06:15.632197 avrotize-1.3.2/README.md
--rw-r--r--   0        0        0     1673 2024-04-28 10:06:15.632197 avrotize-1.3.2/avrotize/__init__.py
--rw-r--r--   0        0        0       88 2024-04-28 10:06:15.632197 avrotize-1.3.2/avrotize/__main__.py
--rw-r--r--   0        0        0      411 2024-04-28 10:06:20.164220 avrotize-1.3.2/avrotize/_version.py
--rw-r--r--   0        0        0     8386 2024-04-28 10:06:15.632197 avrotize-1.3.2/avrotize/asn1toavro.py
--rw-r--r--   0        0        0    15558 2024-04-28 10:06:15.632197 avrotize-1.3.2/avrotize/avrotize.py
--rw-r--r--   0        0        0    43143 2024-04-28 10:06:15.632197 avrotize-1.3.2/avrotize/avrotocsharp.py
--rw-r--r--   0        0        0    18563 2024-04-28 10:06:15.632197 avrotize-1.3.2/avrotize/avrotojava.py
--rw-r--r--   0        0        0    12117 2024-04-28 10:06:15.632197 avrotize-1.3.2/avrotize/avrotojs.py
--rw-r--r--   0        0        0    18104 2024-04-28 10:06:15.632197 avrotize-1.3.2/avrotize/avrotojsons.py
--rw-r--r--   0        0        0     5155 2024-04-28 10:06:15.632197 avrotize-1.3.2/avrotize/avrotokusto.py
--rw-r--r--   0        0        0     5481 2024-04-28 10:06:15.632197 avrotize-1.3.2/avrotize/avrotoparquet.py
--rw-r--r--   0        0        0    22200 2024-04-28 10:06:15.632197 avrotize-1.3.2/avrotize/avrotoproto.py
--rw-r--r--   0        0        0    13101 2024-04-28 10:06:15.632197 avrotize-1.3.2/avrotize/avrotopython.py
--rw-r--r--   0        0        0    10166 2024-04-28 10:06:15.632197 avrotize-1.3.2/avrotize/avrotots.py
--rw-r--r--   0        0        0     9514 2024-04-28 10:06:15.636197 avrotize-1.3.2/avrotize/avrototsql.py
--rw-r--r--   0        0        0    16313 2024-04-28 10:06:15.636197 avrotize-1.3.2/avrotize/avrotoxsd.py
--rw-r--r--   0        0        0    12889 2024-04-28 10:06:15.636197 avrotize-1.3.2/avrotize/common.py
--rw-r--r--   0        0        0    19374 2024-04-28 10:06:15.636197 avrotize-1.3.2/avrotize/dependency_resolver.py
--rw-r--r--   0        0        0     1272 2024-04-28 10:06:15.636197 avrotize-1.3.2/avrotize/generic/generic.avsc
--rw-r--r--   0        0        0    95346 2024-04-28 10:06:15.636197 avrotize-1.3.2/avrotize/jsonstoavro.py
--rw-r--r--   0        0        0     2112 2024-04-28 10:06:15.636197 avrotize-1.3.2/avrotize/kconnect.json
--rw-r--r--   0        0        0     2537 2024-04-28 10:06:15.636197 avrotize-1.3.2/avrotize/kstructtoavro.py
--rw-r--r--   0        0        0    19742 2024-04-28 10:06:15.636197 avrotize-1.3.2/avrotize/proto2parser.py
--rw-r--r--   0        0        0    15536 2024-04-28 10:06:15.636197 avrotize-1.3.2/avrotize/proto3parser.py
--rw-r--r--   0        0        0     8722 2024-04-28 10:06:15.636197 avrotize-1.3.2/avrotize/prototoavro.py
--rw-r--r--   0        0        0     3390 2024-04-28 10:06:15.636197 avrotize-1.3.2/avrotize/prototypes/any.avsc
--rw-r--r--   0        0        0     6521 2024-04-28 10:06:15.636197 avrotize-1.3.2/avrotize/prototypes/api.avsc
--rw-r--r--   0        0        0     1629 2024-04-28 10:06:15.636197 avrotize-1.3.2/avrotize/prototypes/duration.avsc
--rw-r--r--   0        0        0     3558 2024-04-28 10:06:15.636197 avrotize-1.3.2/avrotize/prototypes/field_mask.avsc
--rw-r--r--   0        0        0     2394 2024-04-28 10:06:15.636197 avrotize-1.3.2/avrotize/prototypes/struct.avsc
--rw-r--r--   0        0        0      792 2024-04-28 10:06:15.636197 avrotize-1.3.2/avrotize/prototypes/timestamp.avsc
--rw-r--r--   0        0        0     6296 2024-04-28 10:06:15.636197 avrotize-1.3.2/avrotize/prototypes/type.avsc
--rw-r--r--   0        0        0     2571 2024-04-28 10:06:15.636197 avrotize-1.3.2/avrotize/prototypes/wrappers.avsc
--rw-r--r--   0        0        0    17371 2024-04-28 10:06:15.636197 avrotize-1.3.2/avrotize/xsdtoavro.py
--rw-r--r--   0        0        0     1138 2024-04-28 10:06:15.636197 avrotize-1.3.2/pyproject.toml
--rw-r--r--   0        0        0    27420 1970-01-01 00:00:00.000000 avrotize-1.3.2/PKG-INFO
+-rw-r--r--   0        0        0    26753 2024-05-08 18:17:46.279981 avrotize-1.4.0/README.md
+-rw-r--r--   0        0        0     1673 2024-05-08 18:17:46.283981 avrotize-1.4.0/avrotize/__init__.py
+-rw-r--r--   0        0        0       88 2024-05-08 18:17:46.283981 avrotize-1.4.0/avrotize/__main__.py
+-rw-r--r--   0        0        0      411 2024-05-08 18:17:50.779965 avrotize-1.4.0/avrotize/_version.py
+-rw-r--r--   0        0        0     8386 2024-05-08 18:17:46.283981 avrotize-1.4.0/avrotize/asn1toavro.py
+-rw-r--r--   0        0        0    15557 2024-05-08 18:17:46.283981 avrotize-1.4.0/avrotize/avrotize.py
+-rw-r--r--   0        0        0    43143 2024-05-08 18:17:46.283981 avrotize-1.4.0/avrotize/avrotocsharp.py
+-rw-r--r--   0        0        0    50347 2024-05-08 18:17:46.283981 avrotize-1.4.0/avrotize/avrotojava.py
+-rw-r--r--   0        0        0    12117 2024-05-08 18:17:46.283981 avrotize-1.4.0/avrotize/avrotojs.py
+-rw-r--r--   0        0        0    18104 2024-05-08 18:17:46.283981 avrotize-1.4.0/avrotize/avrotojsons.py
+-rw-r--r--   0        0        0     5155 2024-05-08 18:17:46.283981 avrotize-1.4.0/avrotize/avrotokusto.py
+-rw-r--r--   0        0        0     5481 2024-05-08 18:17:46.283981 avrotize-1.4.0/avrotize/avrotoparquet.py
+-rw-r--r--   0        0        0    22200 2024-05-08 18:17:46.283981 avrotize-1.4.0/avrotize/avrotoproto.py
+-rw-r--r--   0        0        0    13101 2024-05-08 18:17:46.283981 avrotize-1.4.0/avrotize/avrotopython.py
+-rw-r--r--   0        0        0    10166 2024-05-08 18:17:46.283981 avrotize-1.4.0/avrotize/avrotots.py
+-rw-r--r--   0        0        0     9514 2024-05-08 18:17:46.283981 avrotize-1.4.0/avrotize/avrototsql.py
+-rw-r--r--   0        0        0    16313 2024-05-08 18:17:46.283981 avrotize-1.4.0/avrotize/avrotoxsd.py
+-rw-r--r--   0        0        0    13663 2024-05-08 18:17:46.283981 avrotize-1.4.0/avrotize/common.py
+-rw-r--r--   0        0        0    19374 2024-05-08 18:17:46.283981 avrotize-1.4.0/avrotize/dependency_resolver.py
+-rw-r--r--   0        0        0     1272 2024-05-08 18:17:46.283981 avrotize-1.4.0/avrotize/generic/generic.avsc
+-rw-r--r--   0        0        0    95346 2024-05-08 18:17:46.283981 avrotize-1.4.0/avrotize/jsonstoavro.py
+-rw-r--r--   0        0        0     2112 2024-05-08 18:17:46.283981 avrotize-1.4.0/avrotize/kconnect.json
+-rw-r--r--   0        0        0     2537 2024-05-08 18:17:46.283981 avrotize-1.4.0/avrotize/kstructtoavro.py
+-rw-r--r--   0        0        0    19742 2024-05-08 18:17:46.283981 avrotize-1.4.0/avrotize/proto2parser.py
+-rw-r--r--   0        0        0    15536 2024-05-08 18:17:46.283981 avrotize-1.4.0/avrotize/proto3parser.py
+-rw-r--r--   0        0        0     8722 2024-05-08 18:17:46.283981 avrotize-1.4.0/avrotize/prototoavro.py
+-rw-r--r--   0        0        0     3390 2024-05-08 18:17:46.283981 avrotize-1.4.0/avrotize/prototypes/any.avsc
+-rw-r--r--   0        0        0     6521 2024-05-08 18:17:46.283981 avrotize-1.4.0/avrotize/prototypes/api.avsc
+-rw-r--r--   0        0        0     1629 2024-05-08 18:17:46.283981 avrotize-1.4.0/avrotize/prototypes/duration.avsc
+-rw-r--r--   0        0        0     3558 2024-05-08 18:17:46.283981 avrotize-1.4.0/avrotize/prototypes/field_mask.avsc
+-rw-r--r--   0        0        0     2394 2024-05-08 18:17:46.283981 avrotize-1.4.0/avrotize/prototypes/struct.avsc
+-rw-r--r--   0        0        0      792 2024-05-08 18:17:46.283981 avrotize-1.4.0/avrotize/prototypes/timestamp.avsc
+-rw-r--r--   0        0        0     6296 2024-05-08 18:17:46.283981 avrotize-1.4.0/avrotize/prototypes/type.avsc
+-rw-r--r--   0        0        0     2571 2024-05-08 18:17:46.283981 avrotize-1.4.0/avrotize/prototypes/wrappers.avsc
+-rw-r--r--   0        0        0    17371 2024-05-08 18:17:46.283981 avrotize-1.4.0/avrotize/xsdtoavro.py
+-rw-r--r--   0        0        0     1138 2024-05-08 18:17:46.283981 avrotize-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0    27420 1970-01-01 00:00:00.000000 avrotize-1.4.0/PKG-INFO
```

### Comparing `avrotize-1.3.2/README.md` & `avrotize-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `avrotize-1.3.2/avrotize/__init__.py` & `avrotize-1.4.0/avrotize/__init__.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.3.2/avrotize/asn1toavro.py` & `avrotize-1.4.0/avrotize/asn1toavro.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.3.2/avrotize/avrotize.py` & `avrotize-1.4.0/avrotize/avrotize.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,15 +82,15 @@
     a2csharp_parser.add_argument('--system-text-json-annotation', action='store_true', help='Use System.Text.Json annotations', default=False)
     a2csharp_parser.add_argument('--newtonsoft-json-annotation', action='store_true', help='Use Newtonsoft.Json annotations', default=False)
     a2csharp_parser.add_argument('--pascal-properties', action='store_true', help='Use PascalCase properties', default=False)
     
     a2java_parser = subparsers.add_parser('a2java', help='Convert Avro schema to Java classes')
     a2java_parser.add_argument('--avsc', type=str, help='Path to the Avro schema file', required=True)
     a2java_parser.add_argument('--java', type=str, help='Output path for the Java classes', required=True)
-    a2java_parser.add_argument('--package', type=str, help='Java package name', required=False)
+    a2java_parser.add_argument('--package', type=str, help='Java package name', required=True)
     a2java_parser.add_argument('--avro-annotation', action='store_true', help='Use Avro annotations', default=False)
     a2java_parser.add_argument('--jackson-annotation', action='store_true', help='Use Jackson annotations', default=False)
     a2java_parser.add_argument('--pascal-properties', action='store_true', help='Use PascalCase properties', default=False)
     
     a2py_parser = subparsers.add_parser('a2py', help='Convert Avro schema to Python classes')
     a2py_parser.add_argument('--avsc', type=str, help='Path to the Avro schema file', required=True)
     a2py_parser.add_argument('--python', type=str, help='Output path for the Python classes', required=True)
```

### Comparing `avrotize-1.3.2/avrotize/avrotocsharp.py` & `avrotize-1.4.0/avrotize/avrotocsharp.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.3.2/avrotize/avrotojs.py` & `avrotize-1.4.0/avrotize/avrotojs.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.3.2/avrotize/avrotojsons.py` & `avrotize-1.4.0/avrotize/avrotojsons.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.3.2/avrotize/avrotokusto.py` & `avrotize-1.4.0/avrotize/avrotokusto.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.3.2/avrotize/avrotoparquet.py` & `avrotize-1.4.0/avrotize/avrotoparquet.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.3.2/avrotize/avrotoproto.py` & `avrotize-1.4.0/avrotize/avrotoproto.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.3.2/avrotize/avrotopython.py` & `avrotize-1.4.0/avrotize/avrotopython.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.3.2/avrotize/avrotots.py` & `avrotize-1.4.0/avrotize/avrotots.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.3.2/avrotize/avrototsql.py` & `avrotize-1.4.0/avrotize/avrototsql.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.3.2/avrotize/avrotoxsd.py` & `avrotize-1.4.0/avrotize/avrotoxsd.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.3.2/avrotize/common.py` & `avrotize-1.4.0/avrotize/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -317,8 +317,31 @@
     elif string[0].isupper():
         # PascalCase
         words = re.findall(r'[A-Z][a-z0-9_]*\.?', string)
     else:
         # camelCase
         words = re.findall(r'[a-z0-9]+\.?|[A-Z][a-z0-9_]*\.?', string)
     result = ''.join(word.capitalize() for word in words)
+    return result
+
+def camel(string):
+    """ Convert a string to camelCase """
+    if '::' in string:
+        strings = string.split('::')
+        return strings[0] + '::' + '::'.join(camel(s) for s in strings[1:])
+    if '.' in string:
+        strings = string.split('.')
+        return '.'.join(camel(s) for s in strings)
+    if not string or len(string) == 0:
+        return string
+    words = []
+    if '_' in string:
+        # snake_case
+        words = re.split(r'_', string)
+    elif string[0].isupper():
+        # PascalCase
+        words = re.findall(r'[A-Z][a-z0-9_]*\.?', string)
+    else:
+        # camelCase
+        words = re.findall(r'[a-z0-9]+\.?|[A-Z][a-z0-9_]*\.?', string)
+    result = words[0].lower() + ''.join(word.capitalize() for word in words[1:])
     return result
```

### Comparing `avrotize-1.3.2/avrotize/dependency_resolver.py` & `avrotize-1.4.0/avrotize/dependency_resolver.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.3.2/avrotize/generic/generic.avsc` & `avrotize-1.4.0/avrotize/generic/generic.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.3.2/avrotize/jsonstoavro.py` & `avrotize-1.4.0/avrotize/jsonstoavro.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.3.2/avrotize/kconnect.json` & `avrotize-1.4.0/avrotize/kconnect.json`

 * *Files identical despite different names*

### Comparing `avrotize-1.3.2/avrotize/kstructtoavro.py` & `avrotize-1.4.0/avrotize/kstructtoavro.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.3.2/avrotize/proto2parser.py` & `avrotize-1.4.0/avrotize/proto2parser.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.3.2/avrotize/proto3parser.py` & `avrotize-1.4.0/avrotize/proto3parser.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.3.2/avrotize/prototoavro.py` & `avrotize-1.4.0/avrotize/prototoavro.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.3.2/avrotize/prototypes/any.avsc` & `avrotize-1.4.0/avrotize/prototypes/any.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.3.2/avrotize/prototypes/api.avsc` & `avrotize-1.4.0/avrotize/prototypes/api.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.3.2/avrotize/prototypes/duration.avsc` & `avrotize-1.4.0/avrotize/prototypes/duration.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.3.2/avrotize/prototypes/field_mask.avsc` & `avrotize-1.4.0/avrotize/prototypes/field_mask.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.3.2/avrotize/prototypes/struct.avsc` & `avrotize-1.4.0/avrotize/prototypes/struct.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.3.2/avrotize/prototypes/timestamp.avsc` & `avrotize-1.4.0/avrotize/prototypes/timestamp.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.3.2/avrotize/prototypes/type.avsc` & `avrotize-1.4.0/avrotize/prototypes/type.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.3.2/avrotize/prototypes/wrappers.avsc` & `avrotize-1.4.0/avrotize/prototypes/wrappers.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.3.2/avrotize/xsdtoavro.py` & `avrotize-1.4.0/avrotize/xsdtoavro.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.3.2/pyproject.toml` & `avrotize-1.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `avrotize-1.3.2/PKG-INFO` & `avrotize-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avrotize
-Version: 1.3.2
+Version: 1.4.0
 Summary: Tools to convert from and to Avro Schema from various other schema languages.
 Author-email: Clemens Vasters <clemensv@microsoft.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

