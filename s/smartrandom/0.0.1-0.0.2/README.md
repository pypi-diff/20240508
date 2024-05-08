# Comparing `tmp/smartrandom-0.0.1.tar.gz` & `tmp/smartrandom-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartrandom-0.0.1.tar", last modified: Sun May 14 10:46:27 2023, max compression
+gzip compressed data, was "smartrandom-0.0.2.tar", last modified: Wed May  8 04:03:00 2024, max compression
```

## Comparing `smartrandom-0.0.1.tar` & `smartrandom-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 joker     (1000) joker     (1000)        0 2023-05-14 10:46:27.138396 smartrandom-0.0.1/
--rw-r--r--   0 joker     (1000) joker     (1000)     1498 2023-05-14 10:34:49.000000 smartrandom-0.0.1/LICENSE
--rw-r--r--   0 joker     (1000) joker     (1000)     2800 2023-05-14 10:46:27.138396 smartrandom-0.0.1/PKG-INFO
--rw-r--r--   0 joker     (1000) joker     (1000)     1875 2023-05-14 10:33:54.000000 smartrandom-0.0.1/README.md
--rw-r--r--   0 joker     (1000) joker     (1000)     1084 2023-05-14 10:46:27.138396 smartrandom-0.0.1/setup.cfg
--rw-r--r--   0 joker     (1000) joker     (1000)       84 2023-05-14 10:41:10.000000 smartrandom-0.0.1/setup.py
-drwxr-xr-x   0 joker     (1000) joker     (1000)        0 2023-05-14 10:46:27.138396 smartrandom-0.0.1/smartrandom/
--rw-r--r--   0 joker     (1000) joker     (1000)        0 2023-05-14 09:29:03.000000 smartrandom-0.0.1/smartrandom/__init__.py
--rw-r--r--   0 joker     (1000) joker     (1000)     1993 2023-05-14 10:31:15.000000 smartrandom-0.0.1/smartrandom/random_master.py
-drwxr-xr-x   0 joker     (1000) joker     (1000)        0 2023-05-14 10:46:27.138396 smartrandom-0.0.1/smartrandom.egg-info/
--rw-r--r--   0 joker     (1000) joker     (1000)     2800 2023-05-14 10:46:27.000000 smartrandom-0.0.1/smartrandom.egg-info/PKG-INFO
--rw-r--r--   0 joker     (1000) joker     (1000)      263 2023-05-14 10:46:27.000000 smartrandom-0.0.1/smartrandom.egg-info/SOURCES.txt
--rw-r--r--   0 joker     (1000) joker     (1000)        1 2023-05-14 10:46:27.000000 smartrandom-0.0.1/smartrandom.egg-info/dependency_links.txt
--rw-r--r--   0 joker     (1000) joker     (1000)        1 2023-05-14 10:46:27.000000 smartrandom-0.0.1/smartrandom.egg-info/not-zip-safe
--rw-r--r--   0 joker     (1000) joker     (1000)       12 2023-05-14 10:46:27.000000 smartrandom-0.0.1/smartrandom.egg-info/top_level.txt
+drwxr-xr-x   0 smart     (1000) smart     (1000)        0 2024-05-08 04:03:00.619456 smartrandom-0.0.2/
+-rw-r--r--   0 smart     (1000) smart     (1000)     1498 2024-05-08 03:52:29.000000 smartrandom-0.0.2/LICENSE
+-rw-r--r--   0 smart     (1000) smart     (1000)     2838 2024-05-08 04:03:00.619456 smartrandom-0.0.2/PKG-INFO
+-rw-r--r--   0 smart     (1000) smart     (1000)     1913 2024-05-08 03:58:36.000000 smartrandom-0.0.2/README.md
+-rw-r--r--   0 smart     (1000) smart     (1000)     1084 2024-05-08 04:03:00.619456 smartrandom-0.0.2/setup.cfg
+-rw-r--r--   0 smart     (1000) smart     (1000)       84 2024-05-08 03:52:29.000000 smartrandom-0.0.2/setup.py
+drwxr-xr-x   0 smart     (1000) smart     (1000)        0 2024-05-08 04:03:00.612789 smartrandom-0.0.2/smartrandom/
+-rw-r--r--   0 smart     (1000) smart     (1000)      377 2024-05-08 03:57:25.000000 smartrandom-0.0.2/smartrandom/__init__.py
+-rw-r--r--   0 smart     (1000) smart     (1000)     1987 2024-05-08 03:57:25.000000 smartrandom-0.0.2/smartrandom/random_master.py
+drwxr-xr-x   0 smart     (1000) smart     (1000)        0 2024-05-08 04:03:00.616123 smartrandom-0.0.2/smartrandom.egg-info/
+-rw-r--r--   0 smart     (1000) smart     (1000)     2838 2024-05-08 04:03:00.000000 smartrandom-0.0.2/smartrandom.egg-info/PKG-INFO
+-rw-r--r--   0 smart     (1000) smart     (1000)      263 2024-05-08 04:03:00.000000 smartrandom-0.0.2/smartrandom.egg-info/SOURCES.txt
+-rw-r--r--   0 smart     (1000) smart     (1000)        1 2024-05-08 04:03:00.000000 smartrandom-0.0.2/smartrandom.egg-info/dependency_links.txt
+-rw-r--r--   0 smart     (1000) smart     (1000)        1 2024-05-08 03:52:39.000000 smartrandom-0.0.2/smartrandom.egg-info/not-zip-safe
+-rw-r--r--   0 smart     (1000) smart     (1000)       12 2024-05-08 04:03:00.000000 smartrandom-0.0.2/smartrandom.egg-info/top_level.txt
```

### Comparing `smartrandom-0.0.1/LICENSE` & `smartrandom-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `smartrandom-0.0.1/PKG-INFO` & `smartrandom-0.0.2/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartrandom
-Version: 0.0.1
+Version: 0.0.2
 Summary: Random Data Generators
 Home-page: https://github.com/smartlegionlab/smartrandom/
 Author: A.A Suvorov
 Author-email: smartlegiondev@gmail.com
 License: BSD 3-Clause License
 Project-URL: Documentation, https://github.com/smartlegionlab/smartrandom/blob/master/README.md
 Project-URL: Release notes, https://github.com/smartlegionlab/smartrandom/releases
@@ -16,36 +16,35 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# smartrandom
-
+# smartrandom <sup>v0.0.2</sup>
 ---
 
 ## Random Data Generators:
 
 Allows you to generate random strings of a given length from letters, numbers, symbols.
 Helps to generate passwords, service codes (for example, for sending via SMS), hashes and much more.
 ---
 
 ## Help:
 
 ```python
 from smartrandom.random_master import RandomMaster
 
-random_string = RandomMaster.string.get(length=10)
-random_number_string = RandomMaster.number.get(length=10)
-password = RandomMaster.password.get(length=10)
-random_hash = RandomMaster.hash.get(text='give me hash')
-random_number_code = RandomMaster.get_code(length=10, number_flag=True)
-random_string_code = RandomMaster.get_code(length=10, string_flag=True)
-random_symbol_code = RandomMaster.get_code(length=10, symbol_flag=True)
+random_string = RandomMaster.string.create(length=10)
+random_number_string = RandomMaster.number.create(length=10)
+password = RandomMaster.password.create(length=10)
+random_hash = RandomMaster.hash.create(text='give me hash')
+random_number_code = RandomMaster.create_code(length=10, number_flag=True)
+random_string_code = RandomMaster.create_code(length=10, string_flag=True)
+random_symbol_code = RandomMaster.create_code(length=10, symbol_flag=True)
 
 ```
 
 ***
 
 ## Disclaimer of liability:
 
@@ -62,10 +61,10 @@
 
 ***
 
 ## Copyright:
     --------------------------------------------------------
     Licensed under the terms of the BSD 3-Clause License
     (see LICENSE for details).
-    Copyright © 2018-2023, A.A Suvorov
+    Copyright © 2018-2024, A.A Suvorov
     All rights reserved.
     --------------------------------------------------------
```

### Comparing `smartrandom-0.0.1/README.md` & `smartrandom-0.0.2/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,28 @@
-# smartrandom
-
+# smartrandom <sup>v0.0.2</sup>
 ---
 
 ## Random Data Generators:
 
 Allows you to generate random strings of a given length from letters, numbers, symbols.
 Helps to generate passwords, service codes (for example, for sending via SMS), hashes and much more.
 ---
 
 ## Help:
 
 ```python
 from smartrandom.random_master import RandomMaster
 
-random_string = RandomMaster.string.get(length=10)
-random_number_string = RandomMaster.number.get(length=10)
-password = RandomMaster.password.get(length=10)
-random_hash = RandomMaster.hash.get(text='give me hash')
-random_number_code = RandomMaster.get_code(length=10, number_flag=True)
-random_string_code = RandomMaster.get_code(length=10, string_flag=True)
-random_symbol_code = RandomMaster.get_code(length=10, symbol_flag=True)
+random_string = RandomMaster.string.create(length=10)
+random_number_string = RandomMaster.number.create(length=10)
+password = RandomMaster.password.create(length=10)
+random_hash = RandomMaster.hash.create(text='give me hash')
+random_number_code = RandomMaster.create_code(length=10, number_flag=True)
+random_string_code = RandomMaster.create_code(length=10, string_flag=True)
+random_symbol_code = RandomMaster.create_code(length=10, symbol_flag=True)
 
 ```
 
 ***
 
 ## Disclaimer of liability:
 
@@ -40,10 +39,10 @@
 
 ***
 
 ## Copyright:
     --------------------------------------------------------
     Licensed under the terms of the BSD 3-Clause License
     (see LICENSE for details).
-    Copyright © 2018-2023, A.A Suvorov
+    Copyright © 2018-2024, A.A Suvorov
     All rights reserved.
     --------------------------------------------------------
```

### Comparing `smartrandom-0.0.1/setup.cfg` & `smartrandom-0.0.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = smartrandom
-version = 0.0.1
+version = 0.0.2
 author = A.A Suvorov
 author_email = smartlegiondev@gmail.com
 description = Random Data Generators
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/smartlegionlab/smartrandom/
 project_urls =
```

### Comparing `smartrandom-0.0.1/smartrandom/random_master.py` & `smartrandom-0.0.2/smartrandom/random_master.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,72 +1,71 @@
-# -*- coding: utf-8 -*-
 # --------------------------------------------------------
 # Licensed under the terms of the BSD 3-Clause License
 # (see LICENSE for details).
-# Copyright © 2018-2023, A.A Suvorov
+# Copyright © 2018-2024, A.A Suvorov
 # All rights reserved.
 # --------------------------------------------------------
 # https://github.com/smartlegionlab
 # --------------------------------------------------------
 import hashlib
 import random
 import string
 
 
 class RandomStringMaster:
     letters = string.ascii_letters
 
     @classmethod
-    def get(cls, length=10):
+    def create(cls, length=10):
         return ''.join((random.choice(cls.letters) for _ in range(length)))
 
 
 class RandomNumberMaster:
     numbers = string.digits
 
     @classmethod
-    def get(cls, length=10):
+    def create(cls, length=10):
         return ''.join((random.choice(cls.numbers) for _ in range(length)))
 
 
 class RandomSymbolMaster:
     symbols = '@$!%*#?&-'
 
     @classmethod
-    def get(cls, length=10):
+    def create(cls, length=10):
         return ''.join((random.choice(cls.symbols) for _ in range(length)))
 
 
 class RandomPasswordMaster:
     letters = string.ascii_letters
     numbers = string.digits
     symbols = '@$!%*#?&-'
 
     @classmethod
-    def get(cls, length=10):
+    def create(cls, length=10):
         return ''.join((random.choice(cls.letters + cls.numbers + cls.symbols) for _ in range(length)))
 
 
 class RandomHashMaster:
     @classmethod
-    def get(cls, text):
+    def create(cls, text):
         sha = hashlib.sha3_512(text.encode('utf-8'))
         new_hash = sha.hexdigest()
         return new_hash
 
 
 class RandomMaster:
     string = RandomStringMaster()
     number = RandomNumberMaster()
     symbol = RandomSymbolMaster()
     password = RandomPasswordMaster()
     hash = RandomHashMaster()
 
     @classmethod
-    def get_code(cls, length=10, number_flag=False, string_flag=False, symbol_flag=False):
+    def create_code(cls, length=10, number_flag=False, string_flag=False, symbol_flag=False):
         data = ''
         if string_flag:
             data += cls.string.letters
         if number_flag:
             data += cls.number.numbers
         if symbol_flag:
             data += cls.symbol.symbols
```

### Comparing `smartrandom-0.0.1/smartrandom.egg-info/PKG-INFO` & `smartrandom-0.0.2/smartrandom.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartrandom
-Version: 0.0.1
+Version: 0.0.2
 Summary: Random Data Generators
 Home-page: https://github.com/smartlegionlab/smartrandom/
 Author: A.A Suvorov
 Author-email: smartlegiondev@gmail.com
 License: BSD 3-Clause License
 Project-URL: Documentation, https://github.com/smartlegionlab/smartrandom/blob/master/README.md
 Project-URL: Release notes, https://github.com/smartlegionlab/smartrandom/releases
@@ -16,36 +16,35 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# smartrandom
-
+# smartrandom <sup>v0.0.2</sup>
 ---
 
 ## Random Data Generators:
 
 Allows you to generate random strings of a given length from letters, numbers, symbols.
 Helps to generate passwords, service codes (for example, for sending via SMS), hashes and much more.
 ---
 
 ## Help:
 
 ```python
 from smartrandom.random_master import RandomMaster
 
-random_string = RandomMaster.string.get(length=10)
-random_number_string = RandomMaster.number.get(length=10)
-password = RandomMaster.password.get(length=10)
-random_hash = RandomMaster.hash.get(text='give me hash')
-random_number_code = RandomMaster.get_code(length=10, number_flag=True)
-random_string_code = RandomMaster.get_code(length=10, string_flag=True)
-random_symbol_code = RandomMaster.get_code(length=10, symbol_flag=True)
+random_string = RandomMaster.string.create(length=10)
+random_number_string = RandomMaster.number.create(length=10)
+password = RandomMaster.password.create(length=10)
+random_hash = RandomMaster.hash.create(text='give me hash')
+random_number_code = RandomMaster.create_code(length=10, number_flag=True)
+random_string_code = RandomMaster.create_code(length=10, string_flag=True)
+random_symbol_code = RandomMaster.create_code(length=10, symbol_flag=True)
 
 ```
 
 ***
 
 ## Disclaimer of liability:
 
@@ -62,10 +61,10 @@
 
 ***
 
 ## Copyright:
     --------------------------------------------------------
     Licensed under the terms of the BSD 3-Clause License
     (see LICENSE for details).
-    Copyright © 2018-2023, A.A Suvorov
+    Copyright © 2018-2024, A.A Suvorov
     All rights reserved.
     --------------------------------------------------------
```

