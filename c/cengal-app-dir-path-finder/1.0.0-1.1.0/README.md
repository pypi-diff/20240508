# Comparing `tmp/cengal_app_dir_path_finder-1.0.0.tar.gz` & `tmp/cengal_app_dir_path_finder-1.1.0.tar.gz`

## Comparing `cengal_app_dir_path_finder-1.0.0.tar` & `cengal_app_dir_path_finder-1.1.0.tar`

### file list

```diff
@@ -1,7 +1,9 @@
--rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 cengal_app_dir_path_finder-1.0.0/cengal_app_dir_path_finder/__init__.py
--rw-r--r--   0        0        0     4135 2020-02-02 00:00:00.000000 cengal_app_dir_path_finder-1.0.0/.gitignore
--rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 cengal_app_dir_path_finder-1.0.0/LICENSE.md
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 cengal_app_dir_path_finder-1.0.0/NOTICE
--rw-r--r--   0        0        0     9159 2020-02-02 00:00:00.000000 cengal_app_dir_path_finder-1.0.0/README.md
--rw-r--r--   0        0        0     3925 2020-02-02 00:00:00.000000 cengal_app_dir_path_finder-1.0.0/pyproject.toml
--rw-r--r--   0        0        0    12934 2020-02-02 00:00:00.000000 cengal_app_dir_path_finder-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 cengal_app_dir_path_finder-1.1.0/cengal_app_dir_path_finder/__init__.py
+-rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 cengal_app_dir_path_finder-1.1.0/cengal_app_dir_path_finder/versions/__init__.py
+-rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 cengal_app_dir_path_finder-1.1.0/cengal_app_dir_path_finder/versions/v_0/__init__.py
+-rw-r--r--   0        0        0     4135 2020-02-02 00:00:00.000000 cengal_app_dir_path_finder-1.1.0/.gitignore
+-rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 cengal_app_dir_path_finder-1.1.0/LICENSE.md
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 cengal_app_dir_path_finder-1.1.0/NOTICE
+-rw-r--r--   0        0        0    62800 2020-02-02 00:00:00.000000 cengal_app_dir_path_finder-1.1.0/README.md
+-rw-r--r--   0        0        0     4091 2020-02-02 00:00:00.000000 cengal_app_dir_path_finder-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0    66757 2020-02-02 00:00:00.000000 cengal_app_dir_path_finder-1.1.0/PKG-INFO
```

### Comparing `cengal_app_dir_path_finder-1.0.0/cengal_app_dir_path_finder/__init__.py` & `cengal_app_dir_path_finder-1.1.0/cengal_app_dir_path_finder/versions/v_0/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # coding=utf-8
 
-# Copyright © 2012-2023 ButenkoMS. All rights reserved. Contacts: <gtalk@butenkoms.space>
+# Copyright © 2012-2024 ButenkoMS. All rights reserved. Contacts: <gtalk@butenkoms.space>
 # 
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 # 
 #     http://www.apache.org/licenses/LICENSE-2.0
 # 
@@ -19,17 +19,17 @@
 """
 Module Docstring
 Docstrings: http://www.python.org/dev/peps/pep-0257/
 """
 
 
 __author__ = "ButenkoMS <gtalk@butenkoms.space>"
-__copyright__ = "Copyright © 2012-2023 ButenkoMS. All rights reserved. Contacts: <gtalk@butenkoms.space>"
+__copyright__ = "Copyright © 2012-2024 ButenkoMS. All rights reserved. Contacts: <gtalk@butenkoms.space>"
 __credits__ = ["ButenkoMS <gtalk@butenkoms.space>", ]
 __license__ = "Apache License, Version 2.0"
-__version__ = "1.0.0"
+__version__ = "1.1.0"
 __maintainer__ = "ButenkoMS <gtalk@butenkoms.space>"
 __email__ = "gtalk@butenkoms.space"
 __status__ = "Production"
 
 
 from cengal.file_system.app_fs_structure.app_dir_path.versions.v_0 import *
```

### Comparing `cengal_app_dir_path_finder-1.0.0/.gitignore` & `cengal_app_dir_path_finder-1.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `cengal_app_dir_path_finder-1.0.0/LICENSE.md` & `cengal_app_dir_path_finder-1.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `cengal_app_dir_path_finder-1.0.0/NOTICE` & `cengal_app_dir_path_finder-1.1.0/NOTICE`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright © 2012-2023 ButenkoMS. All rights reserved. Contacts: <gtalk@butenkoms.space>
+Copyright © 2012-2024 ButenkoMS. All rights reserved. Contacts: <gtalk@butenkoms.space>
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cengal_app_dir_path_finder-1.0.0/pyproject.toml` & `cengal_app_dir_path_finder-1.1.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -87,15 +87,17 @@
     'Topic :: Software Development :: Libraries :: Python Modules',
     'Topic :: System',
     'Topic :: System :: Filesystems',
     'Topic :: System :: Logging',
     'Typing :: Typed',
 ]
 dependencies = [
-    "pyobjc; platform_system == 'Darwin'",
+    "typing_extensions",
+    "pyobjc; platform_system == 'Darwin' and platform_python_implementation == 'CPython'",
+    "pywin32; platform_system == 'Windows' and platform_python_implementation == 'CPython'",
     "cengal_light",
 ]
 
 [project.urls]
 Homepage = "https://github.com/FI-Mihej/cengal_app_dir_path_finder"
 
 [tool.hatch.version]
```

