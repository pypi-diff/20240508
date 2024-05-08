# Comparing `tmp/h1parser-0.1.tar.gz` & `tmp/h1parser-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/h1parser-0.1.tar", last modified: Sun May  7 11:44:16 2023, max compression
+gzip compressed data, was "dist/h1parser-0.2.tar", last modified: Wed May  8 10:24:23 2024, max compression
```

## Comparing `h1parser-0.1.tar` & `h1parser-0.2.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-05-07 11:44:16.000000 h1parser-0.1/
--rw-r--r--   0 tux       (1000) users      (100)     1063 2023-02-10 23:35:19.000000 h1parser-0.1/LICENSE.txt
--rw-r--r--   0 tux       (1000) users      (100)      760 2023-05-07 11:44:16.000000 h1parser-0.1/PKG-INFO
--rw-r--r--   0 tux       (1000) users      (100)      333 2023-05-07 11:36:25.000000 h1parser-0.1/README.md
-drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-05-07 11:44:16.000000 h1parser-0.1/h1parser/
--rw-r--r--   0 tux       (1000) users      (100)       38 2023-05-07 11:24:03.000000 h1parser-0.1/h1parser/__init__.py
--rwxr-xr-x   0 tux       (1000) users      (100)     4954 2023-04-16 22:37:48.000000 h1parser-0.1/h1parser/parse_header.py
-drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-05-07 11:44:16.000000 h1parser-0.1/h1parser.egg-info/
--rw-r--r--   0 tux       (1000) users      (100)      760 2023-05-07 11:44:15.000000 h1parser-0.1/h1parser.egg-info/PKG-INFO
--rw-r--r--   0 tux       (1000) users      (100)      204 2023-05-07 11:44:15.000000 h1parser-0.1/h1parser.egg-info/SOURCES.txt
--rw-r--r--   0 tux       (1000) users      (100)        1 2023-05-07 11:44:15.000000 h1parser-0.1/h1parser.egg-info/dependency_links.txt
--rw-r--r--   0 tux       (1000) users      (100)        9 2023-05-07 11:44:15.000000 h1parser-0.1/h1parser.egg-info/top_level.txt
--rw-r--r--   0 tux       (1000) users      (100)       38 2023-05-07 11:44:16.000000 h1parser-0.1/setup.cfg
--rwxr-xr-x   0 tux       (1000) users      (100)      753 2023-05-07 11:28:38.000000 h1parser-0.1/setup.py
+drwxr-xr-x   0 tux       (1000) users      (100)        0 2024-05-08 10:24:23.000000 h1parser-0.2/
+-rw-r--r--   0 tux       (1000) users      (100)     1063 2024-05-08 10:07:59.000000 h1parser-0.2/LICENSE.txt
+-rw-r--r--   0 tux       (1000) users      (100)      760 2024-05-08 10:24:23.000000 h1parser-0.2/PKG-INFO
+-rw-r--r--   0 tux       (1000) users      (100)      333 2024-05-08 10:07:59.000000 h1parser-0.2/README.md
+drwxr-xr-x   0 tux       (1000) users      (100)        0 2024-05-08 10:24:23.000000 h1parser-0.2/h1parser/
+-rw-r--r--   0 tux       (1000) users      (100)       52 2024-05-08 10:16:28.000000 h1parser-0.2/h1parser/__init__.py
+-rw-r--r--   0 tux       (1000) users      (100)     6075 2024-04-11 07:58:51.000000 h1parser-0.2/h1parser/parse_header.py
+drwxr-xr-x   0 tux       (1000) users      (100)        0 2024-05-08 10:24:23.000000 h1parser-0.2/h1parser.egg-info/
+-rw-r--r--   0 tux       (1000) users      (100)      760 2024-05-08 10:24:22.000000 h1parser-0.2/h1parser.egg-info/PKG-INFO
+-rw-r--r--   0 tux       (1000) users      (100)      235 2024-05-08 10:24:22.000000 h1parser-0.2/h1parser.egg-info/SOURCES.txt
+-rw-r--r--   0 tux       (1000) users      (100)        1 2024-05-08 10:24:22.000000 h1parser-0.2/h1parser.egg-info/dependency_links.txt
+-rw-r--r--   0 tux       (1000) users      (100)       38 2024-05-08 10:24:22.000000 h1parser-0.2/h1parser.egg-info/requires.txt
+-rw-r--r--   0 tux       (1000) users      (100)        9 2024-05-08 10:24:22.000000 h1parser-0.2/h1parser.egg-info/top_level.txt
+-rw-r--r--   0 tux       (1000) users      (100)       38 2024-05-08 10:24:23.000000 h1parser-0.2/setup.cfg
+-rwxr-xr-x   0 tux       (1000) users      (100)      823 2024-05-08 10:23:05.000000 h1parser-0.2/setup.py
```

### Comparing `h1parser-0.1/LICENSE.txt` & `h1parser-0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `h1parser-0.1/PKG-INFO` & `h1parser-0.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: h1parser
-Version: 0.1
+Version: 0.2
 Summary: A simple, pure Python 2.7/3.x HTTP parser
 Home-page: https://github.com/nggit/h1parser
 Author: nggit
 Author-email: contact@anggit.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `h1parser-0.1/h1parser/parse_header.py` & `h1parser-0.2/h1parser/parse_header.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,40 @@
 # Copyright (c) 2023 nggit
 
+
 class Headers(dict):
     def getlist(self, name):
         values = self.get(name, [])
 
         if isinstance(values, list):
             result = []
 
             for v in values:
-                result.extend(v.replace(b', ', b',').split(b','))
+                result.extend(v.replace(b', ', b',').split(b',', 100))
 
             return result
 
-        return values.replace(b', ', b',').split(b',')
+        return values.replace(b', ', b',').split(b',', 100)
+
 
 class ParseHeader:
+    __slots__ = ('is_request',
+                 'is_response',
+                 'is_valid_request',
+                 'is_valid_response',
+                 '_data',
+                 'headers',
+                 '_headers',
+                 '_header_size')
+
     def __init__(self, data=bytearray(), **kwargs):
         self.parse(data, **kwargs)
 
-    def parse(self, data, header_size=None, excludes=[]):
+    def parse(self, data, header_size=None, excludes=[],
+              max_lines=100, max_line_size=8190):
         self.is_request = False
         self.is_response = False
         self.is_valid_request = False
         self.is_valid_response = False
 
         self._data = data
         self.headers = Headers()
@@ -51,83 +63,106 @@
 
         while True:
             end = header.find(b'\r\n', start)
 
             if end == -1:
                 break
 
+            max_lines -= 1
             line = header[start:end]
-            colon_pos = line.find(b':', 1)
 
-            if colon_pos > 0:
-                name = line[:colon_pos]
-                name_lc = bytes(name.lower())
-                value = line[colon_pos + 1:]
+            if max_lines < 0 or end - start > max_line_size or b'\n' in line:
+                self.is_valid_request = False
+                self.is_valid_response = False
 
-                if value.startswith(b' '):
-                    value = value[1:]
+                return self
 
-                if name_lc in self.headers and isinstance(self.headers[name_lc], list):
-                    self.headers[name_lc].append(value)
-                else:
-                    if name_lc in self.headers:
-                        self.headers[name_lc] = [self.headers[name_lc], value]
-                    else:
-                        self.headers[name_lc] = value
+            colon_pos = line.find(b':', 1)
 
-                if name_lc not in excludes:
-                    self._headers.append((name_lc, value))
-            elif start == 0:
+            if start == 0:
                 if line.startswith(b'HTTP/'):
                     self.is_response = True
 
                     try:
-                        _, self.headers[b'_version'], _status, self.headers[b'_message'] = line.replace(b'/', b' ').split(None, 3)
+                        (
+                            _,
+                            self.headers[b'_version'],
+                            _status,
+                            self.headers[b'_message']
+                        ) = line.replace(b'/', b' ').split(None, 3)
                         self.headers[b'_status'] = int(_status)
                         self.is_valid_response = True
                     except ValueError:
                         self.headers[b'_version'] = b''
                         self.headers[b'_status'] = 0
                         self.headers[b'_message'] = b''
                 else:
                     url_end_pos = line.find(b' HTTP/')
 
                     if url_end_pos > 0:
                         self.is_request = True
 
                         try:
-                            self.headers[b'_method'], self.headers[b'_url'] = line[:url_end_pos].split(b' ', 1)
-                            self.headers[b'_version'] = line[url_end_pos + len(' HTTP/'):]
+                            (
+                                self.headers[b'_method'],
+                                self.headers[b'_url']
+                            ) = line[:url_end_pos].split(b' ', 1)
+                            self.headers[b'_version'] = line[url_end_pos + 6:]
                             self.is_valid_request = True
                         except ValueError:
                             self.headers[b'_method'] = b''
                             self.headers[b'_url'] = b''
                             self.headers[b'_version'] = b''
 
                 self.headers[b'_line'] = line
+            elif colon_pos > 0 and line[colon_pos - 1] != 32:
+                name = line[:colon_pos]
+                name_lc = bytes(name.lower())
+                value = line[colon_pos + 1:]
+
+                if value.startswith(b' '):
+                    value = value[1:]
+
+                if name_lc in self.headers and isinstance(
+                        self.headers[name_lc], list):
+                    self.headers[name_lc].append(value)
+                else:
+                    if name_lc in self.headers:
+                        self.headers[name_lc] = [self.headers[name_lc], value]
+                    else:
+                        self.headers[name_lc] = value
+
+                if name_lc not in excludes:
+                    self._headers.append((name_lc, value))
             else:
                 self.is_valid_request = False
                 self.is_valid_response = False
 
                 break
 
             start = end + 2
 
-        if self.is_valid_request and self.headers[b'_version'] == b'1.1' and b'host' not in self.headers:
+        if self.is_request and b'host' not in self.headers:
             self.headers[b'host'] = b''
-            self.is_valid_request = False
+
+            if self.is_valid_request and self.headers[b'_version'] == b'1.1':
+                self.is_valid_request = False
 
         return self
 
     def remove(self, *args):
         if not args:
             return self
 
-        for i, v in enumerate(self._headers):
-            if v[0] in args:
+        i = len(self._headers)
+
+        while i > 0:
+            i -= 1
+
+            if self._headers[i][0] in args:
                 del self._headers[i]
 
         return self
 
     def append(self, *args):
         for v in args:
             if isinstance(v, tuple):
@@ -152,11 +187,20 @@
 
     def getstatus(self):
         return self.headers.get(b'_status')
 
     def getmessage(self):
         return self.headers.get(b'_message')
 
-    def save(self):
+    def save(self, body=False):
+        if self._header_size in (None, -1):
+            return self._data
+
+        if body:
+            data = self._data[self._header_size:]
+        else:
+            data = self._data[self._header_size:self._header_size + 4]
+
         return bytearray(b'\r\n').join(
-                [self.headers.get(b'_line', b'')] + [bytearray(b': ').join(v) for v in self._headers]
-            ) + self._data[self._header_size:]
+            [self.headers.get(b'_line', b'')] +
+            [bytearray(b': ').join(v) for v in self._headers]
+        ) + data
```

### Comparing `h1parser-0.1/h1parser.egg-info/PKG-INFO` & `h1parser-0.2/h1parser.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: h1parser
-Version: 0.1
+Version: 0.2
 Summary: A simple, pure Python 2.7/3.x HTTP parser
 Home-page: https://github.com/nggit/h1parser
 Author: nggit
 Author-email: contact@anggit.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

