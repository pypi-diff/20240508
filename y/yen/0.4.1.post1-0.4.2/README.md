# Comparing `tmp/yen-0.4.1.post1.tar.gz` & `tmp/yen-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yen-0.4.1.post1.tar", last modified: Tue Jan 16 08:00:26 2024, max compression
+gzip compressed data, was "yen-0.4.2.tar", last modified: Wed May  8 21:41:19 2024, max compression
```

## Comparing `yen-0.4.1.post1.tar` & `yen-0.4.2.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 tusharsadhwani   (501) staff       (20)        0 2024-01-16 08:00:26.124495 yen-0.4.1.post1/
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)     1072 2023-09-22 18:55:35.000000 yen-0.4.1.post1/LICENSE
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)     2425 2024-01-16 08:00:26.124607 yen-0.4.1.post1/PKG-INFO
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)     1533 2024-01-16 07:52:19.000000 yen-0.4.1.post1/README.md
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)     1223 2024-01-16 08:00:26.125044 yen-0.4.1.post1/setup.cfg
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)       37 2023-09-22 18:55:35.000000 yen-0.4.1.post1/setup.py
-drwxr-xr-x   0 tusharsadhwani   (501) staff       (20)        0 2024-01-16 08:00:26.120370 yen-0.4.1.post1/src/
-drwxr-xr-x   0 tusharsadhwani   (501) staff       (20)        0 2024-01-16 08:00:26.122996 yen-0.4.1.post1/src/yen/
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)     3273 2024-01-16 07:52:19.000000 yen-0.4.1.post1/src/yen/__init__.py
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)      120 2023-09-22 18:55:35.000000 yen-0.4.1.post1/src/yen/__main__.py
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)     1280 2024-01-16 07:52:34.000000 yen-0.4.1.post1/src/yen/cli.py
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)     1712 2023-12-13 09:36:38.000000 yen-0.4.1.post1/src/yen/downloader.py
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)     3274 2024-01-16 07:52:19.000000 yen-0.4.1.post1/src/yen/github.py
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)       59 2023-09-22 18:55:35.000000 yen-0.4.1.post1/src/yen/py.typed
-drwxr-xr-x   0 tusharsadhwani   (501) staff       (20)        0 2024-01-16 08:00:26.124232 yen-0.4.1.post1/src/yen.egg-info/
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)     2425 2024-01-16 08:00:26.000000 yen-0.4.1.post1/src/yen.egg-info/PKG-INFO
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)      336 2024-01-16 08:00:26.000000 yen-0.4.1.post1/src/yen.egg-info/SOURCES.txt
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)        1 2024-01-16 08:00:26.000000 yen-0.4.1.post1/src/yen.egg-info/dependency_links.txt
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)       36 2024-01-16 08:00:26.000000 yen-0.4.1.post1/src/yen.egg-info/entry_points.txt
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)       73 2024-01-16 08:00:26.000000 yen-0.4.1.post1/src/yen.egg-info/requires.txt
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)        4 2024-01-16 08:00:26.000000 yen-0.4.1.post1/src/yen.egg-info/top_level.txt
+drwxr-xr-x   0 tusharsadhwani   (501) staff       (20)        0 2024-05-08 21:41:19.213081 yen-0.4.2/
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)     1072 2024-03-30 13:10:26.000000 yen-0.4.2/LICENSE
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)     2670 2024-05-08 21:41:19.213015 yen-0.4.2/PKG-INFO
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)     1533 2024-03-30 13:10:26.000000 yen-0.4.2/README.md
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)     1246 2024-05-08 21:41:19.213396 yen-0.4.2/setup.cfg
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)       37 2024-03-30 13:10:26.000000 yen-0.4.2/setup.py
+drwxr-xr-x   0 tusharsadhwani   (501) staff       (20)        0 2024-05-08 21:41:19.207470 yen-0.4.2/src/
+drwxr-xr-x   0 tusharsadhwani   (501) staff       (20)        0 2024-05-08 21:41:19.211322 yen-0.4.2/src/yen/
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)     3325 2024-05-08 21:39:24.000000 yen-0.4.2/src/yen/__init__.py
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)      120 2024-03-30 13:10:26.000000 yen-0.4.2/src/yen/__main__.py
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)     1317 2024-05-08 21:39:29.000000 yen-0.4.2/src/yen/cli.py
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)     1748 2024-05-08 21:39:33.000000 yen-0.4.2/src/yen/downloader.py
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)  1047789 2024-03-30 13:10:26.000000 yen-0.4.2/src/yen/fallback_release_data.json
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)     3848 2024-05-08 21:39:38.000000 yen-0.4.2/src/yen/github.py
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)       59 2024-03-30 13:10:26.000000 yen-0.4.2/src/yen/py.typed
+drwxr-xr-x   0 tusharsadhwani   (501) staff       (20)        0 2024-05-08 21:41:19.212508 yen-0.4.2/src/yen.egg-info/
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)     2670 2024-05-08 21:41:19.000000 yen-0.4.2/src/yen.egg-info/PKG-INFO
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)      371 2024-05-08 21:41:19.000000 yen-0.4.2/src/yen.egg-info/SOURCES.txt
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)        1 2024-05-08 21:41:19.000000 yen-0.4.2/src/yen.egg-info/dependency_links.txt
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)       36 2024-05-08 21:41:19.000000 yen-0.4.2/src/yen.egg-info/entry_points.txt
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)       73 2024-05-08 21:41:19.000000 yen-0.4.2/src/yen.egg-info/requires.txt
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)        4 2024-05-08 21:41:19.000000 yen-0.4.2/src/yen.egg-info/top_level.txt
```

### Comparing `yen-0.4.1.post1/LICENSE` & `yen-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `yen-0.4.1.post1/PKG-INFO` & `yen-0.4.2/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,31 +1,7 @@
-Metadata-Version: 2.1
-Name: yen
-Version: 0.4.1.post1
-Summary: Yet another Python environment manager.
-Home-page: https://github.com/tusharsadhwani/yen
-Author: Tushar Sadhwani
-Author-email: tushar.sadhwani000@gmail.com
-License: MIT
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
 # yen
 
 The easiest Python environment manager. Create virtual environments for any Python version, without needing Python pre-installed.
 
 ## Installation
 
 Get the tool by running the following command:
```

### Comparing `yen-0.4.1.post1/setup.cfg` & `yen-0.4.2/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = yen
-version = 0.4.1post1
+version = 0.4.2
 description = Yet another Python environment manager.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/tusharsadhwani/yen
 author = Tushar Sadhwani
 author_email = tushar.sadhwani000@gmail.com
 license = MIT
@@ -45,14 +45,15 @@
 	pytest-cov
 	tox
 
 [options.package_data]
 yen = 
 	py.typed
 	activate.sh
+	fallback_release_data.json
 
 [tool:pytest]
 addopts = --cov --cov-report=term-missing
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `yen-0.4.1.post1/src/yen/__init__.py` & `yen-0.4.2/src/yen/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,11 @@
 """yen - Yet another Python environment manager."""
+
+from __future__ import annotations
+
 import hashlib
 import os
 import os.path
 import subprocess
 import tarfile
 
 from yen.downloader import download, read_url
@@ -44,15 +47,15 @@
         python_bin_path = os.path.join(download_directory, "python/python.exe")
     else:
         python_bin_path = os.path.join(download_directory, "python/bin/python3")
     if os.path.exists(python_bin_path):
         # already installed
         return python_version, python_bin_path
 
-    os.makedirs(download_directory)
+    os.makedirs(download_directory, exist_ok=True)
     downloaded_filepath = download(
         download_link,
         f"Downloading {python_version}",
         download_directory,
     )
     # Calculate checksum
     with open(downloaded_filepath, "rb") as python_zip:
```

### Comparing `yen-0.4.1.post1/src/yen/cli.py` & `yen-0.4.2/src/yen/cli.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,11 @@
 """CLI interface for yen."""
+
+from __future__ import annotations
+
 import argparse
 from typing import Literal
 
 from yen import create_symlink, ensure_python, create_venv
 from yen.github import list_pythons
```

### Comparing `yen-0.4.1.post1/src/yen/downloader.py` & `yen-0.4.2/src/yen/downloader.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 """Taken from https://github.com/textualize/rich/blob/ec91917/examples/downloader.py"""
 
+from __future__ import annotations
+
 import os.path
 import signal
 from functools import partial
 from threading import Event
 from typing import Iterable
 from urllib.request import urlopen
```

### Comparing `yen-0.4.1.post1/src/yen/github.py` & `yen-0.4.2/src/yen/github.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,15 @@
+from __future__ import annotations
+
 import json
+import os.path
 import platform
 import re
+import urllib.error
+from typing import Any
 from urllib.request import urlopen
 
 MACHINE_SUFFIX = {
     "Darwin": {
         "arm64": "aarch64-apple-darwin-install_only.tar.gz",
         "x86_64": "x86_64-apple-darwin-install_only.tar.gz",
     },
@@ -18,27 +23,40 @@
             "musl": "x86_64_v3-unknown-linux-musl-install_only.tar.gz",
         },
     },
     "Windows": {"AMD64": "x86_64-pc-windows-msvc-shared-install_only.tar.gz"},
 }
 
 GITHUB_API_URL = (
-    f"https://api.github.com/repos/indygreg/python-build-standalone/releases/latest"
+    "https://api.github.com/repos/indygreg/python-build-standalone/releases/latest"
 )
 PYTHON_VERSION_REGEX = re.compile(r"cpython-(\d+\.\d+\.\d+)")
 
 
+def fallback_release_data() -> dict[str, Any]:
+    """Returns the fallback release data, for when GitHub API gives an error."""
+    print("\033[33mWarning: GitHub unreachable. Using fallback release data.\033[m")
+    data_file = os.path.join(os.path.dirname(__file__), "fallback_release_data.json")
+    with open(data_file) as data:
+        return json.load(data)
+
+
 class NotAvailable(Exception):
     """Raised when the asked Python version is not available."""
 
 
 def get_latest_python_releases() -> list[str]:
     """Returns the list of python download links from the latest github release."""
-    with urlopen(GITHUB_API_URL) as response:
-        release_data = json.load(response)
+    try:
+        with urlopen(GITHUB_API_URL) as response:
+            release_data = json.load(response)
+
+    except urllib.error.URLError:
+        # raise
+        release_data = fallback_release_data()
 
     return [asset["browser_download_url"] for asset in release_data["assets"]]
 
 
 def list_pythons() -> dict[str, str]:
     """Returns available python versions for your machine and their download links."""
     system, machine = platform.system(), platform.machine()
```

### Comparing `yen-0.4.1.post1/src/yen.egg-info/PKG-INFO` & `yen-0.4.2/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yen
-Version: 0.4.1.post1
+Version: 0.4.2
 Summary: Yet another Python environment manager.
 Home-page: https://github.com/tusharsadhwani/yen
 Author: Tushar Sadhwani
 Author-email: tushar.sadhwani000@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -15,16 +15,23 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Provides-Extra: dev
 License-File: LICENSE
+Requires-Dist: microvenv>=2023.2.0
+Requires-Dist: rich>=13.5.3
+Provides-Extra: dev
+Requires-Dist: black; extra == "dev"
+Requires-Dist: mypy; extra == "dev"
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: pytest-cov; extra == "dev"
+Requires-Dist: tox; extra == "dev"
 
 # yen
 
 The easiest Python environment manager. Create virtual environments for any Python version, without needing Python pre-installed.
 
 ## Installation
```

