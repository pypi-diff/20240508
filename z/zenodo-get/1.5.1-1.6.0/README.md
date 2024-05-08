# Comparing `tmp/zenodo_get-1.5.1.tar.gz` & `tmp/zenodo_get-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zenodo_get-1.5.1.tar", last modified: Sat Oct 28 11:32:58 2023, max compression
+gzip compressed data, was "zenodo_get-1.6.0.tar", last modified: Wed May  8 06:44:17 2024, max compression
```

## Comparing `zenodo_get-1.5.1.tar` & `zenodo_get-1.6.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 dvolgyes  (1000) dvolgyes  (1000)        0 2023-10-28 11:32:58.503255 zenodo_get-1.5.1/
-drwxrwxr-x   0 dvolgyes  (1000) dvolgyes  (1000)        0 2023-10-28 11:32:58.502255 zenodo_get-1.5.1/.circleci/
--rw-rw-r--   0 dvolgyes  (1000) dvolgyes  (1000)     1428 2021-11-19 23:25:30.000000 zenodo_get-1.5.1/.circleci/config.yml
--rw-rw-r--   0 dvolgyes  (1000) dvolgyes  (1000)       40 2021-11-19 23:25:30.000000 zenodo_get-1.5.1/.coveragerc
--rw-rw-r--   0 dvolgyes  (1000) dvolgyes  (1000)     1009 2023-05-29 11:52:10.000000 zenodo_get-1.5.1/.pre-commit-config.yaml
--rw-rw-r--   0 dvolgyes  (1000) dvolgyes  (1000)      761 2021-11-19 23:25:30.000000 zenodo_get-1.5.1/.travis.yml
--rw-rw-r--   0 dvolgyes  (1000) dvolgyes  (1000)    34520 2021-11-19 23:25:30.000000 zenodo_get-1.5.1/LICENSE.txt
--rw-rw-r--   0 dvolgyes  (1000) dvolgyes  (1000)       70 2021-11-19 23:25:30.000000 zenodo_get-1.5.1/MANIFEST.in
--rw-rw-r--   0 dvolgyes  (1000) dvolgyes  (1000)      388 2021-11-19 23:25:30.000000 zenodo_get-1.5.1/Makefile
--rw-rw-r--   0 dvolgyes  (1000) dvolgyes  (1000)     1036 2023-10-28 11:32:58.503255 zenodo_get-1.5.1/PKG-INFO
--rw-rw-r--   0 dvolgyes  (1000) dvolgyes  (1000)     4227 2021-11-19 23:25:30.000000 zenodo_get-1.5.1/README.md
--rw-rw-r--   0 dvolgyes  (1000) dvolgyes  (1000)      746 2021-11-19 23:25:30.000000 zenodo_get-1.5.1/appveyor.yml
--rw-rw-r--   0 dvolgyes  (1000) dvolgyes  (1000)       14 2021-11-19 23:25:30.000000 zenodo_get-1.5.1/requirements.txt
--rw-rw-r--   0 dvolgyes  (1000) dvolgyes  (1000)       79 2023-10-28 11:32:58.503255 zenodo_get-1.5.1/setup.cfg
--rw-rw-r--   0 dvolgyes  (1000) dvolgyes  (1000)     1249 2023-10-18 11:04:24.000000 zenodo_get-1.5.1/setup.py
-drwxrwxr-x   0 dvolgyes  (1000) dvolgyes  (1000)        0 2023-10-28 11:32:58.502255 zenodo_get-1.5.1/tests/
--rw-rw-r--   0 dvolgyes  (1000) dvolgyes  (1000)       35 2021-11-19 23:25:30.000000 zenodo_get-1.5.1/tests/Makefile
--rwxrwxr-x   0 dvolgyes  (1000) dvolgyes  (1000)      473 2021-11-19 23:25:30.000000 zenodo_get-1.5.1/tests/test.sh
--rwxrwxr-x   0 dvolgyes  (1000) dvolgyes  (1000)      241 2021-11-19 23:25:30.000000 zenodo_get-1.5.1/tests/win-test.bat
-drwxrwxr-x   0 dvolgyes  (1000) dvolgyes  (1000)        0 2023-10-28 11:32:58.502255 zenodo_get-1.5.1/zenodo_get/
--rw-rw-r--   0 dvolgyes  (1000) dvolgyes  (1000)     1158 2023-10-28 11:31:23.000000 zenodo_get-1.5.1/zenodo_get/__init__.py
--rwxrwxr-x   0 dvolgyes  (1000) dvolgyes  (1000)       97 2023-05-29 11:52:10.000000 zenodo_get-1.5.1/zenodo_get/__main__.py
--rwxrwxr-x   0 dvolgyes  (1000) dvolgyes  (1000)    11889 2023-10-28 11:30:57.000000 zenodo_get-1.5.1/zenodo_get/zget.py
-drwxrwxr-x   0 dvolgyes  (1000) dvolgyes  (1000)        0 2023-10-28 11:32:58.503255 zenodo_get-1.5.1/zenodo_get.egg-info/
--rw-r--r--   0 dvolgyes  (1000) dvolgyes  (1000)     1036 2023-10-28 11:32:58.000000 zenodo_get-1.5.1/zenodo_get.egg-info/PKG-INFO
--rw-rw-r--   0 dvolgyes  (1000) dvolgyes  (1000)      491 2023-10-28 11:32:58.000000 zenodo_get-1.5.1/zenodo_get.egg-info/SOURCES.txt
--rw-rw-r--   0 dvolgyes  (1000) dvolgyes  (1000)        1 2023-10-28 11:32:58.000000 zenodo_get-1.5.1/zenodo_get.egg-info/dependency_links.txt
--rw-rw-r--   0 dvolgyes  (1000) dvolgyes  (1000)       58 2023-10-28 11:32:58.000000 zenodo_get-1.5.1/zenodo_get.egg-info/entry_points.txt
--rw-rw-r--   0 dvolgyes  (1000) dvolgyes  (1000)       14 2023-10-28 11:32:58.000000 zenodo_get-1.5.1/zenodo_get.egg-info/requires.txt
--rw-rw-r--   0 dvolgyes  (1000) dvolgyes  (1000)       11 2023-10-28 11:32:58.000000 zenodo_get-1.5.1/zenodo_get.egg-info/top_level.txt
--rwxrwxr-x   0 dvolgyes  (1000) dvolgyes  (1000)     8692 2023-05-29 11:52:10.000000 zenodo_get-1.5.1/zenodofs.py
+drwxrwxr-x   0 dvolgyes  (1000) dvolgyes  (1000)        0 2024-05-08 06:44:17.245372 zenodo_get-1.6.0/
+drwxrwxr-x   0 dvolgyes  (1000) dvolgyes  (1000)        0 2024-05-08 06:44:17.244372 zenodo_get-1.6.0/.circleci/
+-rw-rw-r--   0 dvolgyes  (1000) dvolgyes  (1000)     1428 2021-11-19 23:25:30.000000 zenodo_get-1.6.0/.circleci/config.yml
+-rw-rw-r--   0 dvolgyes  (1000) dvolgyes  (1000)       40 2021-11-19 23:25:30.000000 zenodo_get-1.6.0/.coveragerc
+-rw-rw-r--   0 dvolgyes  (1000) dvolgyes  (1000)      824 2024-05-08 06:38:08.000000 zenodo_get-1.6.0/.pre-commit-config.yaml
+-rw-rw-r--   0 dvolgyes  (1000) dvolgyes  (1000)      761 2021-11-19 23:25:30.000000 zenodo_get-1.6.0/.travis.yml
+-rw-rw-r--   0 dvolgyes  (1000) dvolgyes  (1000)    34520 2021-11-19 23:25:30.000000 zenodo_get-1.6.0/LICENSE.txt
+-rw-rw-r--   0 dvolgyes  (1000) dvolgyes  (1000)       70 2021-11-19 23:25:30.000000 zenodo_get-1.6.0/MANIFEST.in
+-rw-rw-r--   0 dvolgyes  (1000) dvolgyes  (1000)      388 2021-11-19 23:25:30.000000 zenodo_get-1.6.0/Makefile
+-rw-rw-r--   0 dvolgyes  (1000) dvolgyes  (1000)     1036 2024-05-08 06:44:17.245372 zenodo_get-1.6.0/PKG-INFO
+-rw-rw-r--   0 dvolgyes  (1000) dvolgyes  (1000)     3662 2024-05-08 06:36:00.000000 zenodo_get-1.6.0/README.md
+-rw-rw-r--   0 dvolgyes  (1000) dvolgyes  (1000)      742 2024-05-08 06:36:00.000000 zenodo_get-1.6.0/appveyor.yml
+-rw-rw-r--   0 dvolgyes  (1000) dvolgyes  (1000)       14 2021-11-19 23:25:30.000000 zenodo_get-1.6.0/requirements.txt
+-rw-rw-r--   0 dvolgyes  (1000) dvolgyes  (1000)       79 2024-05-08 06:44:17.245372 zenodo_get-1.6.0/setup.cfg
+-rw-rw-r--   0 dvolgyes  (1000) dvolgyes  (1000)     1203 2023-10-28 12:08:39.000000 zenodo_get-1.6.0/setup.py
+drwxrwxr-x   0 dvolgyes  (1000) dvolgyes  (1000)        0 2024-05-08 06:44:17.244372 zenodo_get-1.6.0/tests/
+-rw-rw-r--   0 dvolgyes  (1000) dvolgyes  (1000)       35 2021-11-19 23:25:30.000000 zenodo_get-1.6.0/tests/Makefile
+-rwxrwxr-x   0 dvolgyes  (1000) dvolgyes  (1000)      472 2024-05-08 06:36:00.000000 zenodo_get-1.6.0/tests/test.sh
+-rw-rw-r--   0 dvolgyes  (1000) dvolgyes  (1000)      240 2024-05-08 06:36:00.000000 zenodo_get-1.6.0/tests/win-test.bat
+drwxrwxr-x   0 dvolgyes  (1000) dvolgyes  (1000)        0 2024-05-08 06:44:17.244372 zenodo_get-1.6.0/zenodo_get/
+-rw-rw-r--   0 dvolgyes  (1000) dvolgyes  (1000)     1161 2024-05-08 06:42:06.000000 zenodo_get-1.6.0/zenodo_get/__init__.py
+-rwxrwxr-x   0 dvolgyes  (1000) dvolgyes  (1000)       97 2023-10-28 12:08:39.000000 zenodo_get-1.6.0/zenodo_get/__main__.py
+-rwxrwxr-x   0 dvolgyes  (1000) dvolgyes  (1000)    12367 2024-05-08 06:40:53.000000 zenodo_get-1.6.0/zenodo_get/zget.py
+drwxrwxr-x   0 dvolgyes  (1000) dvolgyes  (1000)        0 2024-05-08 06:44:17.245372 zenodo_get-1.6.0/zenodo_get.egg-info/
+-rw-r--r--   0 dvolgyes  (1000) dvolgyes  (1000)     1036 2024-05-08 06:44:17.000000 zenodo_get-1.6.0/zenodo_get.egg-info/PKG-INFO
+-rw-rw-r--   0 dvolgyes  (1000) dvolgyes  (1000)      491 2024-05-08 06:44:17.000000 zenodo_get-1.6.0/zenodo_get.egg-info/SOURCES.txt
+-rw-rw-r--   0 dvolgyes  (1000) dvolgyes  (1000)        1 2024-05-08 06:44:17.000000 zenodo_get-1.6.0/zenodo_get.egg-info/dependency_links.txt
+-rw-rw-r--   0 dvolgyes  (1000) dvolgyes  (1000)       58 2024-05-08 06:44:17.000000 zenodo_get-1.6.0/zenodo_get.egg-info/entry_points.txt
+-rw-rw-r--   0 dvolgyes  (1000) dvolgyes  (1000)       14 2024-05-08 06:44:17.000000 zenodo_get-1.6.0/zenodo_get.egg-info/requires.txt
+-rw-rw-r--   0 dvolgyes  (1000) dvolgyes  (1000)       11 2024-05-08 06:44:17.000000 zenodo_get-1.6.0/zenodo_get.egg-info/top_level.txt
+-rwxrwxr-x   0 dvolgyes  (1000) dvolgyes  (1000)     8882 2024-05-08 06:36:00.000000 zenodo_get-1.6.0/zenodofs.py
```

### Comparing `zenodo_get-1.5.1/.circleci/config.yml` & `zenodo_get-1.6.0/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `zenodo_get-1.5.1/.travis.yml` & `zenodo_get-1.6.0/.travis.yml`

 * *Files identical despite different names*

### Comparing `zenodo_get-1.5.1/LICENSE.txt` & `zenodo_get-1.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zenodo_get-1.5.1/PKG-INFO` & `zenodo_get-1.6.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: zenodo_get
-Version: 1.5.1
+Version: 1.6.0
 Summary: Zenodo_get - a downloader for Zenodo records
-Home-page: https://gitlab.com/dvolgyes/zenodo_get
+Home-page: https://github.com/dvolgyes/zenodo_get
 Author: David Völgyes
 Author-email: david.volgyes@ieee.org
 License: AGPL v3
 Keywords: zenodo download
 Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
```

### Comparing `zenodo_get-1.5.1/README.md` & `zenodo_get-1.6.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,45 +1,39 @@
 zenodo_get: a downloader for Zenodo records
 ===========================================
-Travis:[![Build Status](https://travis-ci.org/dvolgyes/zenodo_get.svg?branch=master)](https://travis-ci.org/dvolgyes/zenodo_get)
-CircleCI:[![Build status](https://circleci.com/gh/dvolgyes/zenodo_get.svg?style=svg)](https://circleci.com/gh/dvolgyes/zenodo_get)
-SemaphoreCI:[![Build Status](https://semaphoreci.com/api/v1/dvolgyes/zenodo_get/branches/master/badge.svg)](https://semaphoreci.com/dvolgyes/zenodo_get)
 
 AppVeyor:[![Build status](https://ci.appveyor.com/api/projects/status/f6hw96rhdl104ch9?svg=true)](https://ci.appveyor.com/project/dvolgyes/zenodo-get)
-GitlabCI:[![pipeline status](https://gitlab.com/dvolgyes/zenodo_get/badges/master/pipeline.svg)](https://gitlab.com/dvolgyes/zenodo_get/commits/master)
 
 
 Coveralls:[![Coverage Status](https://img.shields.io/coveralls/github/dvolgyes/zenodo_get/master)](https://coveralls.io/github/dvolgyes/zenodo_get?branch=master)
 Codecov:[![codecov](https://codecov.io/gh/dvolgyes/zenodo_get/branch/master/graph/badge.svg)](https://codecov.io/gh/dvolgyes/zenodo_get)
 Snyk:[![Known Vulnerabilities](https://snyk.io/test/github/dvolgyes/zenodo_get/badge.svg)](https://snyk.io/test/github/dvolgyes/zenodo_get)
 
 
-This is a Python3 tool which can mass-download files from Zenodo records.
+This is a Python3 tool that can mass-download files from Zenodo records.
 
 [![pyversion](https://img.shields.io/pypi/pyversions/zenodo_get.svg)](https://pypi.org/project/zenodo-get/)
-[![PyPI - License](https://img.shields.io/pypi/l/zenodo_get.svg)](https://gitlab.com/dvolgyes/zenodo_get/raw/master/LICENSE.txt)
+[![PyPI - License](https://img.shields.io/pypi/l/zenodo_get.svg)](https://github.com/dvolgyes/zenodo_get/raw/master/LICENSE.txt)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.1261812.svg)](https://doi.org/10.5281/zenodo.1261812)
 
 Source code
 -----------
 
-The code is hosted at Github and GitLab too, with the exact content.
-(except some temporary differences until synchronization)
+The code is hosted at Github, former Gitlab hosting is discontinued.
 
 Install
 -------
 
 From PyPI:
 ```
 pip3 install zenodo_get
 ```
 
-Or from Gitlab/Github:
+Or from Github:
 ```
-pip3 install git+https://gitlab.com/dvolgyes/zenodo_get
 pip3 install git+https://github.com/dvolgyes/zenodo_get
 ```
 
 
 Afterwards, you can query the command line options:
 ```
 zenodo_get -h
@@ -66,28 +60,30 @@
 zenodo_get RECORD_ID_OR_DOI
 ```
 
 Special parameters:
 - ``-m`` : generate md5sums.txt for verification. Beware, if `md5sums.txt` is
   present in the dataset, it will overwrite this generated file. Verification example:
   `md5sum -c md5sums.txt`
+- ``-g GLOB`` : A [glob](https://docs.python.org/3/library/fnmatch.html) expression to
+   select a subset of record files.
 - ``-w FILE`` : instead of downloading the record files, it will
    generate a FILE which contains direct links to the Zenodo site. These links
    could be downloaded with any download manager, e.g. with wget:
    `wget -i urls.txt`
 - ``-e`` : continue on error. It will skip the files with errors, but it will
     try to download the rest of the files.
 - ``-k`` : keep files: it will keep files with invalid md5 checksum. The main purpose
    is debugging.
 - ``-R N``: retry on error N times.
 - ``-p N``: Waiting time in sec before retry attempt. Default: 0.5 sec.
 - ``-n`` : do not continue. The default behaviour is to download only the files
    which are not yet download or where the checksum does not match with the file.
    This flag disables this feature, and it will force download existing files,
-   and assigining a new name to the files (e.g. file(1).ext )
+   and assigning a new name to the files (e.g. file(1).ext )
 
 
 Remark for batch processing: the program always exits with non-zero exit code, if any error has happened,
 for instance, checksum mismatch, download error, time-out, etc. Only perfectly correct
 downloads end with 0 exit code.
 
 Citation
```

### Comparing `zenodo_get-1.5.1/appveyor.yml` & `zenodo_get-1.6.0/appveyor.yml`

 * *Files 19% similar despite different names*

```diff
@@ -12,15 +12,15 @@
           NUMPY_VERSION: "stable"
 
 matrix:
     fast_finish: true
 
 platform:
     -x64
-    
+
 install:
     - "SET PATH=C:\\Python38-x64;%PATH%"
     - "python -m pip install -r requirements.txt"
     - "python -m pip install git+https://github.com/dvolgyes/zenodo_get"
     - choco install --accept-license wget
 
 build: off
```

### Comparing `zenodo_get-1.5.1/setup.py` & `zenodo_get-1.6.0/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,33 +5,31 @@
 
 setuptools.setup(
     name=zget.__title__,
     version=zget.__version__,
     author=zget.__author__,
     author_email=zget.__email__,
     description=zget.__summary__,
-    description_content_type='text/plain',
+    description_content_type="text/plain",
     long_description=zget.__description__,
-    long_description_content_type='text/markdown',
+    long_description_content_type="text/markdown",
     url=zget.__uri__,
     license=zget.__license__,
     packages=setuptools.find_packages(),
-    entry_points={'console_scripts': [
-                      'zenodo_get = zenodo_get.zget:zenodo_get'
-                      ]},
-    python_requires='>=3.8',
+    entry_points={"console_scripts": ["zenodo_get = zenodo_get.zget:zenodo_get"]},
+    python_requires=">=3.8",
     setup_requires=[],
-    install_requires=['requests', 'wget'],
-    keywords='zenodo download',
+    install_requires=["requests", "wget"],
+    keywords="zenodo download",
     classifiers=[
-        'Development Status :: 4 - Beta',
-        'Operating System :: OS Independent',
-        'Programming Language :: Python',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10',
-        'Programming Language :: Python :: 3.11',
-        'Programming Language :: Python :: 3.12',
-        'Intended Audience :: Science/Research',
-        'License :: OSI Approved :: GNU Affero General Public License v3',
+        "Development Status :: 4 - Beta",
+        "Operating System :: OS Independent",
+        "Programming Language :: Python",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
+        "Intended Audience :: Science/Research",
+        "License :: OSI Approved :: GNU Affero General Public License v3",
     ],
 )
```

### Comparing `zenodo_get-1.5.1/zenodo_get/zget.py` & `zenodo_get-1.6.0/zenodo_get/zget.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,71 +1,73 @@
 #!/usr/bin/env python3
-import zenodo_get as zget
-import requests
 import hashlib
-import sys
 import os
-from optparse import OptionParser
-import wget
-import time
+import requests
 import signal
-from pathlib import Path
+import sys
+import time
+import wget
+import zenodo_get as zget
 from contextlib import contextmanager
-import os
+from fnmatch import fnmatch
+from optparse import OptionParser
+from pathlib import Path
 from urllib.parse import unquote
 
-#see https://stackoverflow.com/questions/431684/how-do-i-change-the-working-directory-in-python/24176022#24176022
+
+# see https://stackoverflow.com/questions/431684/how-do-i-change-the-working-directory-in-python/24176022#24176022
 @contextmanager
 def cd(newdir):
     prevdir = os.getcwd()
     os.chdir(os.path.expanduser(newdir))
     try:
         yield
     finally:
         os.chdir(prevdir)
 
+
 def eprint(*args, **kwargs):
     print(*args, file=sys.stderr, **kwargs)
 
 
 def ctrl_c(func):
-
     signal.signal(signal.SIGINT, func)
     return func
 
 
 abort_signal = False
 abort_counter = 0
 exceptions = False
 
+
 @ctrl_c
 def handle_ctrl_c(*args, **kwargs):
     global abort_signal
     global abort_counter
     global exceptions
 
     abort_signal = True
     abort_counter += 1
 
     if abort_counter >= 2:
         eprint()
-        eprint('Immediate abort. There might be unfinished files.')
+        eprint("Immediate abort. There might be unfinished files.")
         if exceptions:
-            raise Exception('Immediate abort')
+            raise Exception("Immediate abort")
         else:
             sys.exit(1)
 
 
 def check_hash(filename, checksum):
-    algorithm = 'md5'
+    algorithm = "md5"
     value = checksum.strip()
     if not os.path.exists(filename):
-        return value, 'invalid'
+        return value, "invalid"
     h = hashlib.new(algorithm)
-    with open(filename, 'rb') as f:
+    with open(filename, "rb") as f:
         while True:
             data = f.read(4096)
             if not data:
                 break
             h.update(data)
     digest = h.hexdigest()
     return value, digest
@@ -77,169 +79,178 @@
     if argv is None:
         argv = sys.argv[1:]
         exceptions = False
     else:
         exceptions = True
 
     parser = OptionParser(
-        usage='%prog [options] RECORD_OR_DOI',
-        version=f'%prog {zget.__version__}'
+        usage="%prog [options] RECORD_OR_DOI", version=f"%prog {zget.__version__}"
     )
 
     parser.add_option(
-        '-c',
-        '--cite',
-        dest='cite',
-        action='store_true',
+        "-c",
+        "--cite",
+        dest="cite",
+        action="store_true",
         default=False,
-        help='print citation information',
+        help="print citation information",
     )
 
     parser.add_option(
-        '-r',
-        '--record',
-        action='store',
-        type='string',
-        dest='record',
-        help='Zenodo record ID',
+        "-r",
+        "--record",
+        action="store",
+        type="string",
+        dest="record",
+        help="Zenodo record ID",
         default=None,
     )
 
     parser.add_option(
-        '-d',
-        '--doi',
-        action='store',
-        type='string',
-        dest='doi',
-        help='Zenodo DOI',
+        "-d",
+        "--doi",
+        action="store",
+        type="string",
+        dest="doi",
+        help="Zenodo DOI",
         default=None,
     )
 
     parser.add_option(
-        '-m',
-        '--md5',
-        action='store_true',
+        "-m",
+        "--md5",
+        action="store_true",
         # ~type=bool,
-        dest='md5',
-        help='Create md5sums.txt for verification.',
+        dest="md5",
+        help="Create md5sums.txt for verification.",
         default=False,
     )
 
     parser.add_option(
-        '-w',
-        '--wget',
-        action='store',
-        type='string',
-        dest='wget',
-        help='Create URL list for download managers. '
-        '(Files will not be downloaded.)',
+        "-w",
+        "--wget",
+        action="store",
+        type="string",
+        dest="wget",
+        help="Create URL list for download managers. "
+        "(Files will not be downloaded.)",
         default=None,
     )
 
     parser.add_option(
-        '-e',
-        '--continue-on-error',
-        action='store_true',
-        dest='error',
-        help='Continue with next file if error happens.',
+        "-e",
+        "--continue-on-error",
+        action="store_true",
+        dest="error",
+        help="Continue with next file if error happens.",
         default=False,
     )
 
     parser.add_option(
-        '-k',
-        '--keep',
-        action='store_true',
-        dest='keep',
-        help='Keep files with invalid checksum.' ' (Default: delete them.)',
+        "-k",
+        "--keep",
+        action="store_true",
+        dest="keep",
+        help="Keep files with invalid checksum." " (Default: delete them.)",
         default=False,
     )
 
     parser.add_option(
-        '-n',
-        '--do-not-continue',
-        action='store_false',
-        dest='cont',
-        help='Do not continue previous download attempt. (Default: continue.)',
+        "-n",
+        "--do-not-continue",
+        action="store_false",
+        dest="cont",
+        help="Do not continue previous download attempt. (Default: continue.)",
         default=True,
     )
 
     parser.add_option(
-        '-R',
-        '--retry',
-        action='store',
+        "-R",
+        "--retry",
+        action="store",
         type=int,
-        dest='retry',
-        help='Retry on error N more times.',
+        dest="retry",
+        help="Retry on error N more times.",
         default=0,
     )
 
     parser.add_option(
-        '-p',
-        '--pause',
-        action='store',
+        "-p",
+        "--pause",
+        action="store",
         type=float,
-        dest='pause',
-        help='Wait N second before retry attempt, e.g. 0.5',
+        dest="pause",
+        help="Wait N second before retry attempt, e.g. 0.5",
         default=0.5,
     )
 
     parser.add_option(
-        '-t',
-        '--time-out',
-        action='store',
+        "-t",
+        "--time-out",
+        action="store",
         type=float,
-        dest='timeout',
-        help='Set connection time-out. Default: 15 [sec].',
-        default=15.,
+        dest="timeout",
+        help="Set connection time-out. Default: 15 [sec].",
+        default=15.0,
     )
 
     parser.add_option(
-        '-o',
-        '--output-dir',
-        action='store',
+        "-o",
+        "--output-dir",
+        action="store",
         type=str,
-        dest='outdir',
-        default='.',
-        help='Output directory, created if necessary. Default: current directory.',
+        dest="outdir",
+        default=".",
+        help="Output directory, created if necessary. Default: current directory.",
     )
 
     parser.add_option(
-        '-s',
-        '--sandbox',
-        action='store_true',
-        dest='sandbox',
-        help='Use Zenodo Sandbox URL.',
+        "-s",
+        "--sandbox",
+        action="store_true",
+        dest="sandbox",
+        help="Use Zenodo Sandbox URL.",
         default=False,
     )
 
     parser.add_option(
-        '-a',
-        '--access-token',
-        action='store',
+        "-a",
+        "--access-token",
+        action="store",
         type=str,
-        dest='access_token',
+        dest="access_token",
         default=None,
-        help='Optional access token for the requests query.',
+        help="Optional access token for the requests query.",
+    )
+
+    parser.add_option(
+        "-g",
+        "--glob",
+        action="store",
+        type=str,
+        dest="glob",
+        default="*",
+        help="Optional glob expression for files.",
     )
 
     (options, args) = parser.parse_args(argv)
 
     if options.cite:
-        print('Reference for this software:')
+        print("Reference for this software:")
         print(zget.__reference__)
         print()
-        print('Bibtex format:')
+        print("Bibtex format:")
         print(zget.__bibtex__)
         if exceptions:
             return
         else:
             sys.exit(0)
 
     # create directory, if necessary, then change to it
-    options.outdir=Path(options.outdir)
+    options.outdir = Path(options.outdir)
     options.outdir.mkdir(parents=True, exist_ok=True)
     with cd(options.outdir):
         if len(args) > 0:
             try:
                 options.record = str(int(args[0]))
             except ValueError:
                 options.doi = args[0]
@@ -248,160 +259,167 @@
             if exceptions:
                 return
             else:
                 sys.exit(0)
 
         if options.doi is not None:
             url = options.doi
-            if not url.startswith('http'):
-                url = 'https://doi.org/' + url
+            if not url.startswith("http"):
+                url = "https://doi.org/" + url
             try:
                 r = requests.get(url, timeout=options.timeout)
             except requests.exceptions.ConnectTimeout:
-                eprint('Connection timeout.')
+                eprint("Connection timeout.")
                 if exceptions:
                     raise
                 else:
                     sys.exit(1)
             except Exception:
-                eprint('Connection error.')
+                eprint("Connection error.")
                 if exceptions:
                     raise
                 else:
                     sys.exit(1)
             if not r.ok:
-                eprint('DOI could not be resolved. Try again, or use record ID.')
+                eprint("DOI could not be resolved. Try again, or use record ID.")
                 if exceptions:
-                    raise ValueError('DOI', options.doi)
+                    raise ValueError("DOI", options.doi)
                 else:
                     sys.exit(1)
 
-            recordID = r.url.split('/')[-1]
+            recordID = r.url.split("/")[-1]
         else:
             recordID = options.record
         recordID = recordID.strip()
 
         if not options.sandbox:
-            url = 'https://zenodo.org/api/records/'
+            url = "https://zenodo.org/api/records/"
         else:
-            url = 'https://sandbox.zenodo.org/api/records/'
+            url = "https://sandbox.zenodo.org/api/records/"
 
         params = {}
         if options.access_token:
-            params['access_token'] = options.access_token
+            params["access_token"] = options.access_token
 
         try:
             r = requests.get(url + recordID, params=params, timeout=options.timeout)
         except requests.exceptions.ConnectTimeout:
-            eprint('Connection timeout during metadata reading.')
+            eprint("Connection timeout during metadata reading.")
             if exceptions:
                 raise
             else:
                 sys.exit(1)
         except Exception:
-            eprint('Connection error during metadata reading.')
+            eprint("Connection error during metadata reading.")
             if exceptions:
                 raise
             else:
                 sys.exit(1)
 
         if r.ok:
             js = r.json()
-            files = js['files']
-            total_size = sum((f.get('filesize') or f['size']) for f in files)
+            files = [
+                f
+                for f in js["files"]
+                if fnmatch(f.get("filename") or f["key"], options.glob)
+            ]
+            if not files:
+                eprint("Files {} not found in metadata".format(options.glob))
+
+            total_size = sum((f.get("filesize") or f["size"]) for f in files)
 
             if options.md5 is not None:
-                with open('md5sums.txt', 'wt') as md5file:
+                with open("md5sums.txt", "wt") as md5file:
                     for f in files:
-                        fname = (f.get('filename') or f['key'])
-                        checksum = f['checksum'].split(':')[-1]
-                        md5file.write(f'{checksum}  {fname}\n')
+                        fname = f.get("filename") or f["key"]
+                        checksum = f["checksum"].split(":")[-1]
+                        md5file.write(f"{checksum}  {fname}\n")
 
             if options.wget is not None:
-                if options.wget == '-':
+                if options.wget == "-":
                     for f in files:
-                        fname = (f.get('filename') or f['key'])
-                        link = 'https://zenodo.org/record/{}/files/{}'.format(
+                        fname = f.get("filename") or f["key"]
+                        link = "https://zenodo.org/records/{}/files/{}".format(
                             recordID, fname
                         )
                         print(link)
                 else:
-                    with open(options.wget, 'wt') as wgetfile:
+                    with open(options.wget, "wt") as wgetfile:
                         for f in files:
-                            fname = (f.get('filename') or f['key'])
-                            link = 'https://zenodo.org/record/{}/files/{}'.format(
+                            fname = f.get("filename") or f["key"]
+                            link = "https://zenodo.org/records/{}/files/{}".format(
                                 recordID, fname
                             )
-                            wgetfile.write(link + '\n')
+                            wgetfile.write(link + "\n")
             else:
-                eprint('Title: {}'.format(js['metadata']['title']))
-                eprint('Keywords: ' +
-                       (', '.join(js['metadata'].get('keywords', []))))
-                eprint('Publication date: ' + js['metadata']['publication_date'])
-                eprint('DOI: ' + js['metadata']['doi'])
-                eprint('Total size: {:.1f} MB'.format(total_size / 2 ** 20))
+                eprint("Title: {}".format(js["metadata"]["title"]))
+                eprint("Keywords: " + (", ".join(js["metadata"].get("keywords", []))))
+                eprint("Publication date: " + js["metadata"]["publication_date"])
+                eprint("DOI: " + js["metadata"]["doi"])
+                eprint("Total size: {:.1f} MB".format(total_size / 2**20))
 
                 for f in files:
                     if abort_signal:
-                        eprint('Download aborted with CTRL+C.')
-                        eprint('Already successfully downloaded files are kept.')
+                        eprint("Download aborted with CTRL+C.")
+                        eprint("Already successfully downloaded files are kept.")
                         break
 
-                    fname = (f.get('filename') or f['key'])
-                    link = 'https://zenodo.org/record/{}/files/{}'.format(
+                    fname = f.get("filename") or f["key"]
+                    link = "https://zenodo.org/records/{}/files/{}".format(
                         recordID, fname
                     )
 
-
-                    size = (f.get('filesize') or f['size']) / 2 ** 20
+                    size = (f.get("filesize") or f["size"]) / 2**20
                     eprint()
-                    eprint(f'Link: {link}   size: {size:.1f} MB')
-                    fname = (f.get('filename') or f['key'])
-                    checksum = f['checksum'].split(':')[-1]
+                    eprint(f"Link: {link}   size: {size:.1f} MB")
+                    fname = f.get("filename") or f["key"]
+                    checksum = f["checksum"].split(":")[-1]
 
                     remote_hash, local_hash = check_hash(fname, checksum)
 
                     if remote_hash == local_hash and options.cont:
-                        eprint(f'{fname} is already downloaded correctly.')
+                        eprint(f"{fname} is already downloaded correctly.")
                         continue
 
                     for _ in range(options.retry + 1):
                         try:
                             link = url = unquote(link)
-                            filename = wget.download(f"{link}?access_token={options.access_token}")
+                            filename = wget.download(
+                                f"{link}?access_token={options.access_token}"
+                            )
                         except Exception:
-                            eprint(f'  Download error. Original link: {link}')
+                            eprint(f"  Download error. Original link: {link}")
                             time.sleep(options.pause)
                         else:
                             break
                     else:
-                        eprint('  Too many errors.')
+                        eprint("  Too many errors.")
                         if not options.error:
-                            eprint('  Download is aborted.')
+                            eprint("  Download is aborted.")
                             if exceptions:
-                                raise Exception('too  many errors')
+                                raise Exception("too  many errors")
                             else:
                                 sys.exit(1)
-                        eprint('  Download continues with the next file.')
+                        eprint("  Download continues with the next file.")
                         continue
 
                     eprint()
                     h1, h2 = check_hash(filename, checksum)
                     if h1 == h2:
-                        eprint(f'Checksum is correct. ({h1})')
+                        eprint(f"Checksum is correct. ({h1})")
                     else:
-                        eprint(f'Checksum is INCORRECT!({h1} got:{h2})')
+                        eprint(f"Checksum is INCORRECT!({h1} got:{h2})")
                         if not options.keep:
-                            eprint('  File is deleted.')
+                            eprint("  File is deleted.")
                             os.remove(filename)
                         else:
-                            eprint('  File is NOT deleted!')
+                            eprint("  File is NOT deleted!")
                         if not options.error:
                             sys.exit(1)
                 else:
-                    eprint('All files have been downloaded.')
+                    eprint("All files have been downloaded.")
         else:
-            eprint('Record could not get accessed.')
+            eprint("Record could not get accessed.")
             if exceptions:
-                raise Exception('Record could not get accessed.')
+                raise Exception("Record could not get accessed.")
             else:
-                sys.exit(1)
+                sys.exit(1)
```

### Comparing `zenodo_get-1.5.1/zenodo_get.egg-info/PKG-INFO` & `zenodo_get-1.6.0/zenodo_get.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: zenodo-get
-Version: 1.5.1
+Version: 1.6.0
 Summary: Zenodo_get - a downloader for Zenodo records
-Home-page: https://gitlab.com/dvolgyes/zenodo_get
+Home-page: https://github.com/dvolgyes/zenodo_get
 Author: David Völgyes
 Author-email: david.volgyes@ieee.org
 License: AGPL v3
 Keywords: zenodo download
 Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
```

### Comparing `zenodo_get-1.5.1/zenodofs.py` & `zenodo_get-1.6.0/zenodofs.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 try:
     import requests
     from box import SBox
     from fuse import FUSE, Operations, LoggingMixIn
 except ImportError as e:
     logging.getLogger().critical(e)
-    logging.getLogger().critical('You need to install python-box, requests and fusepy.')
+    logging.getLogger().critical("You need to install python-box, requests and fusepy.")
     sys.exit(1)
 
 
 class WebFile:
 
     def __init__(self, url, size, chunksize=64, largefile=1024):
         self.url = url
@@ -80,24 +80,25 @@
 
             start = domain.start - self.last_offset
             response = response + self.last_page[start:end]
 
             N = max(end - start, 0)
 
             if domain.start + N < domain.stop:
-                response = response + self[domain.start + N:domain.stop]
+                response = response + self[domain.start + N : domain.stop]
         return response
 
 
 class ZenodoFS(LoggingMixIn, Operations):
 
     def __init__(self, recordIDs, sandbox_recordIDs, chunksize=64, largefile=1024):
-        self.records = {'sandbox': [],
-                        'zenodo': [],
-                        }
+        self.records = {
+            "sandbox": [],
+            "zenodo": [],
+        }
         self.attr_cache = SBox(default_box=True)
         self.dir_cache = SBox(default_box=True)
         self.open_files = {}
         self.content = {}
         self.chunksize = chunksize
         self.largefile = largefile
         self.logger = logging.getLogger()
@@ -105,144 +106,186 @@
             self.get_metadata(rid, sandbox=False)
         for rid in sandbox_recordIDs:
             self.get_metadata(rid, sandbox=True)
 
     @cache(maxsize=1024)
     def get_metadata(self, recordID, sandbox=False, exceptions=True, timeout=15):
         if not sandbox:
-            url = 'https://zenodo.org/api/records/'
+            url = "https://zenodo.org/api/records/"
         else:
-            url = 'https://sandbox.zenodo.org/api/records/'
+            url = "https://sandbox.zenodo.org/api/records/"
 
         try:
             r = requests.get(url + recordID, timeout=timeout)
         except requests.exceptions.ConnectTimeout:
-            self.logger.critical('Connection timeout during metadata reading.')
+            self.logger.critical("Connection timeout during metadata reading.")
             raise
         except Exception:
-            self.logger.critical('Connection error during metadata reading.')
+            self.logger.critical("Connection error during metadata reading.")
             raise
 
         js = {}
         if r.ok:
-            js = json.loads(r.text)['files']
-            for f in json.loads(r.text)['files']:
-                path = 'zenodo' if not sandbox else 'sandbox'
+            js = json.loads(r.text)["files"]
+            for f in json.loads(r.text)["files"]:
+                path = "zenodo" if not sandbox else "sandbox"
                 self.attr_cache[f'/{path}/{recordID}/{f["key"]}'] = SBox(
-                    f, default_box=True)
+                    f, default_box=True
+                )
 
-            self.content[f"/{path}/{recordID}.json"] = (SBox(metadata=js).to_json() + "\n").encode()
-            self.content[f"/{path}/{recordID}.yaml"] = SBox(metadata=js).to_yaml().encode()
+            self.content[f"/{path}/{recordID}.json"] = (
+                SBox(metadata=js).to_json() + "\n"
+            ).encode()
+            self.content[f"/{path}/{recordID}.yaml"] = (
+                SBox(metadata=js).to_yaml().encode()
+            )
         return js
 
     def readdir(self, path, fh):
-        level = len(path.split('/'))
-        content = [name for name in self.attr_cache.keys()
-                   if name.startswith(path)]
-        if path == '/':
-            return ['.', 'sandbox', 'zenodo']
-
-        elif path in ('/sandbox', '/zenodo'):
-            content = [name for name in self.attr_cache.keys()
-                       if name.startswith(path)]
+        level = len(path.split("/"))
+        content = [name for name in self.attr_cache.keys() if name.startswith(path)]
+        if path == "/":
+            return [".", "sandbox", "zenodo"]
+
+        elif path in ("/sandbox", "/zenodo"):
+            content = [name for name in self.attr_cache.keys() if name.startswith(path)]
         else:
-            parts = path.split('/')
+            parts = path.split("/")
             if len(parts) >= 3:
                 recordID = parts[2]
                 self.get_metadata(recordID)
-                content = [name for name in self.attr_cache.keys()
-                           if name.startswith(path)]
+                content = [
+                    name for name in self.attr_cache.keys() if name.startswith(path)
+                ]
 
         N = len(path) + 1
-        content = list({name[N:].split('/')[0] for name in content if len(name) > N and name[N-1] == '/'})
+        content = list(
+            {
+                name[N:].split("/")[0]
+                for name in content
+                if len(name) > N and name[N - 1] == "/"
+            }
+        )
         if level == 2:
-            content = content + [f"{name}.yaml" for name in content if name.find('.') == -1] + [f"{name}.json" for name in content if name.find('.') == -1]
+            content = (
+                content
+                + [f"{name}.yaml" for name in content if name.find(".") == -1]
+                + [f"{name}.json" for name in content if name.find(".") == -1]
+            )
         return list(set(content))
 
     def getattr(self, path, fh=None):
-        parts = path.split('/')
+        parts = path.split("/")
         level = len(parts)
         st = {}
-        if path in ['/', '/sandbox', '/zenodo']:
-            st['st_mode'] = (S_IFDIR | 0o755)
-            st['st_nlink'] = 2
+        if path in ["/", "/sandbox", "/zenodo"]:
+            st["st_mode"] = S_IFDIR | 0o755
+            st["st_nlink"] = 2
         elif level == 3:
-            if path.find('.') > -1:
+            if path.find(".") > -1:
                 size = len(self.content[path])
-                st = {'st_mode': (S_IFREG | 0o444), 'st_size': size}
+                st = {"st_mode": (S_IFREG | 0o444), "st_size": size}
             else:
-                st['st_mode'] = (S_IFDIR | 0o755)
-                st['st_nlink'] = 2
+                st["st_mode"] = S_IFDIR | 0o755
+                st["st_nlink"] = 2
         else:
             size = 0
-            st = {'st_mode': (S_IFREG | 0o444), 'st_size': size}
+            st = {"st_mode": (S_IFREG | 0o444), "st_size": size}
             if level >= 3:
                 recordID = parts[2]
                 self.get_metadata(recordID)
 
             if level == 4:
                 fn = self.attr_cache[path]
-                if 'size' in fn:
-                    st['st_size'] = fn['size']
-        st['st_ctime'] = st['st_mtime'] = st['st_atime'] = time()
+                if "size" in fn:
+                    st["st_size"] = fn["size"]
+        st["st_ctime"] = st["st_mtime"] = st["st_atime"] = time()
         return st
 
     def open(self, path, mode):
         if path not in self.open_files:
-            url = self.attr_cache[path]['links'].get('self')
-            size = self.attr_cache[path].get('size', 0)
+            url = self.attr_cache[path]["links"].get("self")
+            size = self.attr_cache[path].get("size", 0)
             self.open_files[path] = WebFile(url, size, self.chunksize, self.largefile)
         return 0
 
     def read(self, path, size, offset, fh):
         if path in self.content:
-            return self.content[path][offset:offset + size]
+            return self.content[path][offset : offset + size]
 
-        return self.open_files[path][offset:offset + size]
+        return self.open_files[path][offset : offset + size]
 
     def release(self, path, fh):
         if path in self.open_files:
             wf = self.open_files.pop(path)
             wf.close()
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
 
     import argparse
+
     parser = argparse.ArgumentParser()
     parser.add_argument("mountpoint", type=str, help="mount point")
-    parser.add_argument("-r", "--record", nargs='+', action='extend', default=[],
-                        help='record ID(s)')
-    parser.add_argument("-s", "--sandbox", nargs='+', action='extend', default=[],
-                        help='sandbox record ID(s)')
-    parser.add_argument("-c", "--chunk_size", type=int, default=64,
-                        help='chunk size [KB] for network download (default: 64)')
-    parser.add_argument("-l", "--large_file_limit", type=int, default=256,
-                        help='file size [KB] which is downloaded without splitting into chunks (default: 256)')
-
-    parser.add_argument("-L", "--log_level",
-                        default='error',
-                        const='error',
-                        nargs='?',
-                        choices=['critical', 'error', 'warning', 'info', 'debug'],
-                        help='log level (default: error)')
+    parser.add_argument(
+        "-r", "--record", nargs="+", action="extend", default=[], help="record ID(s)"
+    )
+    parser.add_argument(
+        "-s",
+        "--sandbox",
+        nargs="+",
+        action="extend",
+        default=[],
+        help="sandbox record ID(s)",
+    )
+    parser.add_argument(
+        "-c",
+        "--chunk_size",
+        type=int,
+        default=64,
+        help="chunk size [KB] for network download (default: 64)",
+    )
+    parser.add_argument(
+        "-l",
+        "--large_file_limit",
+        type=int,
+        default=256,
+        help="file size [KB] which is downloaded without splitting into chunks (default: 256)",
+    )
+
+    parser.add_argument(
+        "-L",
+        "--log_level",
+        default="error",
+        const="error",
+        nargs="?",
+        choices=["critical", "error", "warning", "info", "debug"],
+        help="log level (default: error)",
+    )
 
     parser.add_argument("-f", "--foreground", action="store_true", default=False)
     parser.add_argument("-d", "--debug", action="store_true", default=False)
 
     args = parser.parse_args()
 
-    level = {'critical': logging.CRITICAL,
-             'error':    logging.ERROR,
-             'warning':  logging.WARNING,
-             'info':     logging.INFO,
-             'debug':    logging.DEBUG,
-             }[args.log_level]
+    level = {
+        "critical": logging.CRITICAL,
+        "error": logging.ERROR,
+        "warning": logging.WARNING,
+        "info": logging.INFO,
+        "debug": logging.DEBUG,
+    }[args.log_level]
 
     logging.basicConfig(level=level)
 
-    fuse = FUSE(ZenodoFS(args.record, args.sandbox, chunksize=args.chunk_size, largefile=args.large_file_limit),
-                args.mountpoint,
-                foreground=args.foreground,
-                nothreads=True,
-                debug=args.debug
-                )
+    fuse = FUSE(
+        ZenodoFS(
+            args.record,
+            args.sandbox,
+            chunksize=args.chunk_size,
+            largefile=args.large_file_limit,
+        ),
+        args.mountpoint,
+        foreground=args.foreground,
+        nothreads=True,
+        debug=args.debug,
+    )
```

