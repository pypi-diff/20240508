# Comparing `tmp/xmonkey_namonica-0.1.7.tar.gz` & `tmp/xmonkey_namonica-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xmonkey_namonica-0.1.7.tar", last modified: Fri May  3 07:06:36 2024, max compression
+gzip compressed data, was "xmonkey_namonica-0.1.8.tar", last modified: Wed May  8 06:21:05 2024, max compression
```

## Comparing `xmonkey_namonica-0.1.7.tar` & `xmonkey_namonica-0.1.8.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 ovalenzuela   (501) staff       (20)        0 2024-05-03 07:06:36.350431 xmonkey_namonica-0.1.7/
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    11357 2024-04-25 02:09:33.000000 xmonkey_namonica-0.1.7/LICENSE
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      129 2024-05-03 07:06:36.350264 xmonkey_namonica-0.1.7/PKG-INFO
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2356 2024-05-02 22:56:57.000000 xmonkey_namonica-0.1.7/README.md
--rw-r--r--   0 ovalenzuela   (501) staff       (20)       38 2024-05-03 07:06:36.350468 xmonkey_namonica-0.1.7/setup.cfg
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      343 2024-05-03 07:06:11.000000 xmonkey_namonica-0.1.7/setup.py
-drwxr-xr-x   0 ovalenzuela   (501) staff       (20)        0 2024-05-03 07:06:36.346481 xmonkey_namonica-0.1.7/xmonkey_namonica/
--rw-r--r--   0 ovalenzuela   (501) staff       (20)        0 2024-04-25 06:28:08.000000 xmonkey_namonica-0.1.7/xmonkey_namonica/__init__.py
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2509 2024-05-02 22:56:57.000000 xmonkey_namonica-0.1.7/xmonkey_namonica/cli.py
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     3953 2024-05-02 06:31:44.000000 xmonkey_namonica-0.1.7/xmonkey_namonica/common.py
-drwxr-xr-x   0 ovalenzuela   (501) staff       (20)        0 2024-05-03 07:06:36.349950 xmonkey_namonica-0.1.7/xmonkey_namonica/handlers/
--rw-r--r--   0 ovalenzuela   (501) staff       (20)        0 2024-04-25 06:28:41.000000 xmonkey_namonica-0.1.7/xmonkey_namonica/handlers/__init__.py
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      956 2024-04-25 07:37:41.000000 xmonkey_namonica-0.1.7/xmonkey_namonica/handlers/base_handler.py
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2159 2024-05-02 08:06:57.000000 xmonkey_namonica-0.1.7/xmonkey_namonica/handlers/cargo_handler.py
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     3513 2024-05-02 22:56:57.000000 xmonkey_namonica-0.1.7/xmonkey_namonica/handlers/conda_handler.py
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     5123 2024-05-02 22:56:57.000000 xmonkey_namonica-0.1.7/xmonkey_namonica/handlers/gem_handler.py
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     4022 2024-05-02 08:06:57.000000 xmonkey_namonica-0.1.7/xmonkey_namonica/handlers/gen_handler.py
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     3707 2024-05-02 08:06:57.000000 xmonkey_namonica-0.1.7/xmonkey_namonica/handlers/github_handler.py
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     5124 2024-05-02 08:06:57.000000 xmonkey_namonica-0.1.7/xmonkey_namonica/handlers/golang_handler.py
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2211 2024-05-02 08:06:57.000000 xmonkey_namonica-0.1.7/xmonkey_namonica/handlers/npm_handler.py
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2159 2024-05-02 08:06:57.000000 xmonkey_namonica-0.1.7/xmonkey_namonica/handlers/nuget_handler.py
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2229 2024-05-02 08:06:57.000000 xmonkey_namonica-0.1.7/xmonkey_namonica/handlers/pypi_handler.py
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     3447 2024-05-02 22:56:57.000000 xmonkey_namonica-0.1.7/xmonkey_namonica/utils.py
-drwxr-xr-x   0 ovalenzuela   (501) staff       (20)        0 2024-05-03 07:06:36.350113 xmonkey_namonica-0.1.7/xmonkey_namonica.egg-info/
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      129 2024-05-03 07:06:36.000000 xmonkey_namonica-0.1.7/xmonkey_namonica.egg-info/PKG-INFO
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      836 2024-05-03 07:06:36.000000 xmonkey_namonica-0.1.7/xmonkey_namonica.egg-info/SOURCES.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)        1 2024-05-03 07:06:36.000000 xmonkey_namonica-0.1.7/xmonkey_namonica.egg-info/dependency_links.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)       63 2024-05-03 07:06:36.000000 xmonkey_namonica-0.1.7/xmonkey_namonica.egg-info/entry_points.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)       17 2024-05-03 07:06:36.000000 xmonkey_namonica-0.1.7/xmonkey_namonica.egg-info/requires.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)       17 2024-05-03 07:06:36.000000 xmonkey_namonica-0.1.7/xmonkey_namonica.egg-info/top_level.txt
+drwxr-xr-x   0 ovalenzuela   (501) staff       (20)        0 2024-05-08 06:21:05.167772 xmonkey_namonica-0.1.8/
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    11357 2024-04-25 02:09:33.000000 xmonkey_namonica-0.1.8/LICENSE
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      322 2024-05-08 06:21:05.167598 xmonkey_namonica-0.1.8/PKG-INFO
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2349 2024-05-08 06:21:00.000000 xmonkey_namonica-0.1.8/README.md
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)       38 2024-05-08 06:21:05.167818 xmonkey_namonica-0.1.8/setup.cfg
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      498 2024-05-08 06:21:00.000000 xmonkey_namonica-0.1.8/setup.py
+drwxr-xr-x   0 ovalenzuela   (501) staff       (20)        0 2024-05-08 06:21:05.164998 xmonkey_namonica-0.1.8/xmonkey_namonica/
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)        0 2024-04-25 06:28:08.000000 xmonkey_namonica-0.1.8/xmonkey_namonica/__init__.py
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2509 2024-05-02 22:56:57.000000 xmonkey_namonica-0.1.8/xmonkey_namonica/cli.py
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     4244 2024-05-08 06:21:00.000000 xmonkey_namonica-0.1.8/xmonkey_namonica/common.py
+drwxr-xr-x   0 ovalenzuela   (501) staff       (20)        0 2024-05-08 06:21:05.167165 xmonkey_namonica-0.1.8/xmonkey_namonica/handlers/
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)        0 2024-04-25 06:28:41.000000 xmonkey_namonica-0.1.8/xmonkey_namonica/handlers/__init__.py
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1091 2024-05-08 06:21:00.000000 xmonkey_namonica-0.1.8/xmonkey_namonica/handlers/base_handler.py
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2977 2024-05-08 06:21:00.000000 xmonkey_namonica-0.1.8/xmonkey_namonica/handlers/cargo_handler.py
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     4064 2024-05-08 06:21:00.000000 xmonkey_namonica-0.1.8/xmonkey_namonica/handlers/conda_handler.py
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     5853 2024-05-08 06:21:00.000000 xmonkey_namonica-0.1.8/xmonkey_namonica/handlers/gem_handler.py
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     4148 2024-05-08 06:21:00.000000 xmonkey_namonica-0.1.8/xmonkey_namonica/handlers/gen_handler.py
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     4544 2024-05-08 06:21:00.000000 xmonkey_namonica-0.1.8/xmonkey_namonica/handlers/github_handler.py
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     6040 2024-05-08 06:21:00.000000 xmonkey_namonica-0.1.8/xmonkey_namonica/handlers/golang_handler.py
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2793 2024-05-08 06:21:00.000000 xmonkey_namonica-0.1.8/xmonkey_namonica/handlers/npm_handler.py
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     3011 2024-05-08 06:21:00.000000 xmonkey_namonica-0.1.8/xmonkey_namonica/handlers/nuget_handler.py
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     3160 2024-05-08 06:21:00.000000 xmonkey_namonica-0.1.8/xmonkey_namonica/handlers/pypi_handler.py
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     3481 2024-05-07 21:08:49.000000 xmonkey_namonica-0.1.8/xmonkey_namonica/utils.py
+drwxr-xr-x   0 ovalenzuela   (501) staff       (20)        0 2024-05-08 06:21:05.167423 xmonkey_namonica-0.1.8/xmonkey_namonica.egg-info/
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      322 2024-05-08 06:21:05.000000 xmonkey_namonica-0.1.8/xmonkey_namonica.egg-info/PKG-INFO
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      836 2024-05-08 06:21:05.000000 xmonkey_namonica-0.1.8/xmonkey_namonica.egg-info/SOURCES.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)        1 2024-05-08 06:21:05.000000 xmonkey_namonica-0.1.8/xmonkey_namonica.egg-info/dependency_links.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)       63 2024-05-08 06:21:05.000000 xmonkey_namonica-0.1.8/xmonkey_namonica.egg-info/entry_points.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)       82 2024-05-08 06:21:05.000000 xmonkey_namonica-0.1.8/xmonkey_namonica.egg-info/requires.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)       17 2024-05-08 06:21:05.000000 xmonkey_namonica-0.1.8/xmonkey_namonica.egg-info/top_level.txt
```

### Comparing `xmonkey_namonica-0.1.7/LICENSE` & `xmonkey_namonica-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `xmonkey_namonica-0.1.7/README.md` & `xmonkey_namonica-0.1.8/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 xmonkey-namonica "pkg:npm/tslib@2.6.2/"
 ```
 
 ### nuget
 Sample NuGet purl is provided below:
 
 ```
-xmonkey-namonica "pkg:nuget/Nirvana.MongoProvider@2.1.154"
+xmonkey-namonica "pkg:nuget/Newtonsoft.json@13.0.3"
 ```
 
 ### PyPI
 Sample PyPI purl is provided below:
 
 ```
 xmonkey-namonica "pkg:pypi/flask@3.0.3/"
```

### Comparing `xmonkey_namonica-0.1.7/xmonkey_namonica/cli.py` & `xmonkey_namonica-0.1.8/xmonkey_namonica/cli.py`

 * *Files identical despite different names*

### Comparing `xmonkey_namonica-0.1.7/xmonkey_namonica/common.py` & `xmonkey_namonica-0.1.8/xmonkey_namonica/common.py`

 * *Files 7% similar despite different names*

```diff
@@ -85,22 +85,28 @@
         pattern = "[^0-9<>,.()@a-zA-Z-\s]+"
         for root, _, files in os.walk(temp_dir):
             for file in files:
                 file_path = os.path.join(root, file)
                 try:
                     with open(file_path, 'r', encoding='utf-8') as f:
                         for line in f:
-                            if ("copyright" in line.lower() and
-                                    len(line) <= 50):
-                                copyhit = line.strip()
-                                copyhit = re.sub(pattern, "", line.strip())
-                                copyrights.append({
-                                    "file": file_path,
-                                    "line": copyhit.strip()
-                                })
+                            clean_line = line.strip().lower()
+                            if (
+                                "copyright " in clean_line
+                                and len(clean_line) <= 50
+                            ):
+                                clean_line = re.sub(pattern, "", clean_line)
+                                if (
+                                    clean_line.startswith('copyright')
+                                    or " copyright" in clean_line
+                                ):
+                                    copyrights.append({
+                                        "file": file_path,
+                                        "line": clean_line
+                                    })
                 except UnicodeDecodeError:
                     continue
         return copyrights
 
     @staticmethod
     def serialize_output(data):
         return json.dumps(data, indent=4)
```

### Comparing `xmonkey_namonica-0.1.7/xmonkey_namonica/handlers/base_handler.py` & `xmonkey_namonica-0.1.8/xmonkey_namonica/handlers/base_handler.py`

 * *Files 20% similar despite different names*

```diff
@@ -25,12 +25,17 @@
         pass
 
     @abstractmethod
     def generate_report(self):
         """Generate a report from the scanned data."""
         pass
 
+    @abstractmethod
+    def get_license(self, pkg_name):
+        """Obtain the license from repo or package metadata."""
+        pass
+
     def cleanup(self):
         """Remove the temporary directory created for package handling."""
         if self.temp_dir and os.path.exists(self.temp_dir):
             shutil.rmtree(self.temp_dir)
             print(f"Cleaned up temporary directory: {self.temp_dir}")
```

### Comparing `xmonkey_namonica-0.1.7/xmonkey_namonica/handlers/conda_handler.py` & `xmonkey_namonica-0.1.8/xmonkey_namonica/handlers/conda_handler.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import os
 import magic
 import logging
+import requests
 from .base_handler import BaseHandler
 from urllib.parse import urlparse, parse_qs
 from ..common import PackageManager, temp_directory
 from ..utils import download_file, temp_directory, check_and_extract
 from ..utils import extract_zip, extract_tar, extract_bz2
 
 
@@ -52,20 +53,34 @@
         logging.info("Scanning package contents...")
         files = PackageManager.scan_for_files(
             self.temp_dir, ['COPYRIGHT', 'NOTICES', 'LICENSE', 'COPYING']
         )
         results['license_files'] = files
         copyhits = PackageManager.scan_for_copyright(self.temp_dir)
         results['copyrights'] = copyhits
+        pkg_name = self.purl_details['name']
+        results['license'] = self.get_license(pkg_name)
         self.results = results
 
     def generate_report(self):
         logging.info("Generating report based on the scanned data...")
         return self.results
 
+    def get_license(self, pkg_name):
+        channel = 'conda-forge'
+        url = f"https://api.anaconda.org/package/{channel}/{pkg_name}"
+        response = requests.get(url)
+        if response.status_code == 200:
+            data = response.json()
+            license_info = data.get('license', '')
+            return license_info
+        else:
+            logging.error("Can't obtain data from Crates.IO")
+            return ''
+
     def construct_download_url(self):
         base_url = "https://anaconda.org/conda-forge/"
         package_name = self.purl_details['name']
         version = self.purl_details['version']
         qualifiers = self.purl_details['qualifiers']
         if 'build' in qualifiers:
             build = qualifiers['build'][0]
```

### Comparing `xmonkey_namonica-0.1.7/xmonkey_namonica/handlers/gem_handler.py` & `xmonkey_namonica-0.1.8/xmonkey_namonica/handlers/gem_handler.py`

 * *Files 9% similar despite different names*

```diff
@@ -94,20 +94,39 @@
         logging.info("Scanning package contents...")
         files = PackageManager.scan_for_files(
             self.temp_dir, ['COPYRIGHT', 'NOTICES', 'LICENSE', 'COPYING']
         )
         results['license_files'] = files
         copyhits = PackageManager.scan_for_copyright(self.temp_dir)
         results['copyrights'] = copyhits
+        pkg_name = self.purl_details['name']
+        results['license'] = self.get_license(pkg_name)
         self.results = results
 
     def generate_report(self):
         logging.info("Generating report based on the scanned data...")
         return self.results
 
+    def get_license(self, pkg_name):
+        url = f"https://rubygems.org/api/v1/gems/{pkg_name}.json"
+        response = requests.get(url)
+        if response.status_code == 200:
+            data = response.json()
+            print('data:', data)
+            license_info = data.get('licenses') or data.get('license')
+            if license_info:
+                if isinstance(license_info, list):
+                    return ', '.join(license_info)
+                return license_info
+            else:
+                return ''
+        else:
+            logging.error("Can't obtain data from Crates.IO")
+            return ''
+
     def fetch_file(self, url):
         response = requests.get(url)
         if response.status_code == 200:
             file_data = response.content
             package_file_path = os.path.join(
                 self.temp_dir,
                 "downloaded_file"
```

### Comparing `xmonkey_namonica-0.1.7/xmonkey_namonica/handlers/gen_handler.py` & `xmonkey_namonica-0.1.8/xmonkey_namonica/handlers/gen_handler.py`

 * *Files 8% similar despite different names*

```diff
@@ -49,20 +49,25 @@
         logging.info("Scanning package contents...")
         files = PackageManager.scan_for_files(
             self.temp_dir, ['COPYRIGHT', 'NOTICES', 'LICENSE', 'COPYING']
         )
         results['license_files'] = files
         copyhits = PackageManager.scan_for_copyright(self.temp_dir)
         results['copyrights'] = copyhits
+        # Needs OSLiLi implementation
+        results['license'] = ''
         self.results = results
 
     def generate_report(self):
         logging.info("Generating report based on the scanned data...")
         return self.results
 
+    def get_license(self, file_url):
+        return ''
+
     def verify_checksum(self, data, provided_checksum):
         if ':' in provided_checksum:
             _, provided_checksum = provided_checksum.split(':', 1)
         hash_sha256 = hashlib.sha256()
         hash_sha256.update(data)
         full_checksum = hash_sha256.hexdigest()
         return full_checksum.startswith(provided_checksum)
```

### Comparing `xmonkey_namonica-0.1.7/xmonkey_namonica/handlers/github_handler.py` & `xmonkey_namonica-0.1.8/xmonkey_namonica/handlers/github_handler.py`

 * *Files 24% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from ..utils import download_file, temp_directory, extract_tar
 
 
 class GithubHandler(BaseHandler):
     def fetch(self):
         self.base_url = "https://github.com/"
         repo_url = self.construct_repo_url()
+        self.repo_url = repo_url
         with temp_directory() as temp_dir:
             self.temp_dir = temp_dir
             if self.purl_details['subpath']:
                 self.fetch_file(repo_url)
                 logging.info(f"File downloaded in {self.temp_dir}")
                 self.unpack()
             else:
@@ -54,20 +55,41 @@
         logging.info("Scanning package contents...")
         files = PackageManager.scan_for_files(
             self.temp_dir, ['COPYRIGHT', 'NOTICES', 'LICENSE', 'COPYING']
         )
         results['license_files'] = files
         copyhits = PackageManager.scan_for_copyright(self.temp_dir)
         results['copyrights'] = copyhits
+        results['license'] = self.get_license(self.repo_url)
         self.results = results
 
     def generate_report(self):
         logging.info("Generating report based on the scanned data...")
         return self.results
 
+    def get_license(self, repo_url):
+        repo_url = repo_url[0]
+        if repo_url.endswith('.git'):
+            repo_url = repo_url[:-4]
+        repo_path = repo_url.split("github.com/")[1]
+        api_url = f"https://api.github.com/repos/{repo_path}/license"
+        response = requests.get(api_url)
+        if response.status_code == 200:
+            data = response.json()
+            license_name = data.get('license', {}).get('name', '')
+            return license_name
+        elif response.status_code == 404:
+            logging.error("License file not found in repository")
+            return ''
+        else:
+            logging.error(
+                "Failed: HTTP {response.status_code}"
+            )
+            return ''
+
     def fetch_file(self, url):
         response = requests.get(url)
         if response.status_code == 200:
             file_data = response.content
             package_file_path = os.path.join(
                 self.temp_dir,
                 "downloaded_file"
```

### Comparing `xmonkey_namonica-0.1.7/xmonkey_namonica/handlers/golang_handler.py` & `xmonkey_namonica-0.1.8/xmonkey_namonica/handlers/golang_handler.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from ..utils import download_file, temp_directory, extract_tar
 
 
 class GolangHandler(BaseHandler):
     def fetch(self):
         self.base_url = "https://github.com/"
         repo_url = self.construct_repo_url()
+        self.repo_url = repo_url
         with temp_directory() as temp_dir:
             self.temp_dir = temp_dir
             if self.purl_details['subpath']:
                 self.fetch_file(repo_url)
                 logging.info(f"File downloaded in {self.temp_dir}")
                 self.unpack()
             else:
@@ -91,20 +92,39 @@
         logging.info("Scanning package contents...")
         files = PackageManager.scan_for_files(
             self.temp_dir, ['COPYRIGHT', 'NOTICES', 'LICENSE', 'COPYING']
         )
         results['license_files'] = files
         copyhits = PackageManager.scan_for_copyright(self.temp_dir)
         results['copyrights'] = copyhits
+        results['license'] = self.get_license(self.repo_url)
         self.results = results
 
     def generate_report(self):
         logging.info("Generating report based on the scanned data...")
         return self.results
 
+    def get_license(self, repo_url):
+        repo_url = repo_url[0]
+        if repo_url.endswith('.git'):
+            repo_url = repo_url[:-4]
+        repo_path = repo_url.split("github.com/")[1]
+        api_url = f"https://api.github.com/repos/{repo_path}/license"
+        response = requests.get(api_url)
+        if response.status_code == 200:
+            data = response.json()
+            license_name = data.get('license', {}).get('name', '')
+            return license_name
+        elif response.status_code == 404:
+            logging.error("License file not found in repository")
+            return ''
+        else:
+            logging.error("Failed: HTTP {response.status_code}")
+            return ''
+
     def fetch_file(self, url):
         response = requests.get(url)
         if response.status_code == 200:
             file_data = response.content
             package_file_path = os.path.join(
                 self.temp_dir,
                 "downloaded_file"
@@ -120,14 +140,16 @@
         try:
             subprocess.run(
                 ["git", "clone", repo, self.temp_dir],
                 check=True,
                 stdout=subprocess.DEVNULL,
                 stderr=subprocess.DEVNULL
             )
+            if 'latest' in self.purl_details['version']:
+                self.purl_details['version'] = None
             if self.purl_details['version']:
                 version = self.purl_details['version']
                 subprocess.run(
                     ["git", "-C", self.temp_dir, "checkout", version],
                     check=True,
                     stdout=subprocess.DEVNULL,
                     stderr=subprocess.DEVNULL
```

### Comparing `xmonkey_namonica-0.1.7/xmonkey_namonica/handlers/npm_handler.py` & `xmonkey_namonica-0.1.8/xmonkey_namonica/handlers/npm_handler.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
 import logging
+import requests
 from .base_handler import BaseHandler
 from ..common import PackageManager, temp_directory
 from ..utils import download_file, temp_directory, extract_tar
 
 
 class NpmHandler(BaseHandler):
     def fetch(self):
@@ -41,20 +42,34 @@
         logging.info("Scanning package contents...")
         files = PackageManager.scan_for_files(
             self.temp_dir, ['COPYRIGHT', 'NOTICES', 'LICENSE', 'COPYING']
         )
         results['license_files'] = files
         copyhits = PackageManager.scan_for_copyright(self.temp_dir)
         results['copyrights'] = copyhits
+        pkg_name = self.purl_details['name']
+        results['license'] = self.get_license(pkg_name)
         self.results = results
 
     def generate_report(self):
         logging.info("Generating report based on the scanned data...")
         return self.results
 
+    def get_license(self, pkg_name):
+        url = f"https://registry.npmjs.org/{pkg_name}"
+        response = requests.get(url)
+        if response.status_code == 200:
+            data = response.json()
+            latest_version = data['dist-tags']['latest']
+            license_info = data['versions'][latest_version].get('license', '')
+            return license_info
+        else:
+            logging.error("Can't obtain data from NPM")
+            return ''
+
     def construct_download_url(self):
         namespace = (
             self.purl_details['namespace'].replace('%40', '@') + '/' +
             self.purl_details['name']
             if self.purl_details['namespace']
             else self.purl_details['name']
         )
```

### Comparing `xmonkey_namonica-0.1.7/xmonkey_namonica/handlers/nuget_handler.py` & `xmonkey_namonica-0.1.8/xmonkey_namonica/handlers/pypi_handler.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import os
 import logging
+import requests
 from .base_handler import BaseHandler
 from ..common import PackageManager, temp_directory
-from ..utils import download_file, temp_directory, extract_zip
+from ..utils import download_file, temp_directory, extract_tar
 
 
-class NugetHandler(BaseHandler):
+class PypiHandler(BaseHandler):
     def fetch(self):
         download_url = self.construct_download_url()
         with temp_directory() as temp_dir:
             filename = (
                 f"{self.purl_details['name']}-"
-                f"{self.purl_details['version']}.zip"
+                f"{self.purl_details['version']}.tgz"
             )
             package_file_path = os.path.join(
                 temp_dir,
                 filename
             )
             download_file(download_url, package_file_path)
             logging.info(f"Downloaded package to {package_file_path}")
@@ -23,42 +24,65 @@
             self.unpack()
             self.scan()
 
     def unpack(self):
         if self.temp_dir:
             filename = (
                 f"{self.purl_details['name']}-"
-                f"{self.purl_details['version']}.zip"
+                f"{self.purl_details['version']}.tgz"
             )
             package_file_path = os.path.join(
                 self.temp_dir,
                 filename
             )
-            extract_zip(package_file_path, self.temp_dir)
+            extract_tar(package_file_path, self.temp_dir)
             logging.info(f"Unpacked package in {self.temp_dir}")
 
     def scan(self):
         results = {}
         logging.info("Scanning package contents...")
         files = PackageManager.scan_for_files(
             self.temp_dir, ['COPYRIGHT', 'NOTICES', 'LICENSE', 'COPYING']
         )
         results['license_files'] = files
         copyhits = PackageManager.scan_for_copyright(self.temp_dir)
         results['copyrights'] = copyhits
+        pkg_name = self.purl_details['name']
+        results['license'] = self.get_license(pkg_name)
         self.results = results
 
     def generate_report(self):
         logging.info("Generating report based on the scanned data...")
         return self.results
 
+    def get_license(self, pkg_name):
+        url = f"https://pypi.org/pypi/{pkg_name}/json"
+        response = requests.get(url)
+        if response.status_code == 200:
+            data = response.json()
+            print(data)
+            license_info = data['info'].get('license')
+            if not license_info:
+                classifiers = data['info'].get('classifiers', [])
+                for classifier in classifiers:
+                    if "License ::" in classifier:
+                        license_info = classifier.split(" :: ")[-1]
+                        break
+            if not license_info:
+                license_info = 'License information not available'
+            return license_info
+        else:
+            logging.error("Can't obtain data from Nuget Registry")
+            return ''
+
     def construct_download_url(self):
         namespace = (
             self.purl_details['namespace'].replace('%40', '@')
             if self.purl_details['namespace']
             else self.purl_details['name']
         )
+        iniName = namespace[0].lower()
         return (
-            f"https://www.nuget.org/api/v2/package/"
-            f"{self.purl_details['name']}/"
-            f"{self.purl_details['version']}"
+            f"https://pypi.python.org/packages/source/{iniName}/{namespace}/"
+            f"{self.purl_details['name']}-"
+            f"{self.purl_details['version']}.tar.gz"
         )
```

### Comparing `xmonkey_namonica-0.1.7/xmonkey_namonica/handlers/pypi_handler.py` & `xmonkey_namonica-0.1.8/xmonkey_namonica/handlers/nuget_handler.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import os
 import logging
+import requests
 from .base_handler import BaseHandler
 from ..common import PackageManager, temp_directory
-from ..utils import download_file, temp_directory, extract_tar
+from ..utils import download_file, temp_directory, extract_zip
 
 
-class PypiHandler(BaseHandler):
+class NugetHandler(BaseHandler):
     def fetch(self):
         download_url = self.construct_download_url()
         with temp_directory() as temp_dir:
             filename = (
                 f"{self.purl_details['name']}-"
-                f"{self.purl_details['version']}.tgz"
+                f"{self.purl_details['version']}.zip"
             )
             package_file_path = os.path.join(
                 temp_dir,
                 filename
             )
             download_file(download_url, package_file_path)
             logging.info(f"Downloaded package to {package_file_path}")
@@ -23,43 +24,63 @@
             self.unpack()
             self.scan()
 
     def unpack(self):
         if self.temp_dir:
             filename = (
                 f"{self.purl_details['name']}-"
-                f"{self.purl_details['version']}.tgz"
+                f"{self.purl_details['version']}.zip"
             )
             package_file_path = os.path.join(
                 self.temp_dir,
                 filename
             )
-            extract_tar(package_file_path, self.temp_dir)
+            extract_zip(package_file_path, self.temp_dir)
             logging.info(f"Unpacked package in {self.temp_dir}")
 
     def scan(self):
         results = {}
         logging.info("Scanning package contents...")
         files = PackageManager.scan_for_files(
             self.temp_dir, ['COPYRIGHT', 'NOTICES', 'LICENSE', 'COPYING']
         )
         results['license_files'] = files
         copyhits = PackageManager.scan_for_copyright(self.temp_dir)
         results['copyrights'] = copyhits
+        pkg_name = self.purl_details['name']
+        results['license'] = self.get_license(pkg_name)
         self.results = results
 
     def generate_report(self):
         logging.info("Generating report based on the scanned data...")
         return self.results
 
+    def get_license(self, pkg_name):
+        pkg_name = pkg_name.lower()
+        url = (
+            "https://api.nuget.org/v3/registration5-semver1/"
+            f"{pkg_name}/index.json"
+        )
+        response = requests.get(url)
+        if response.status_code == 200:
+            data = response.json()
+            l_vdata = data['items'][-1]['items'][-1]['catalogEntry']
+            license_expression = l_vdata.get('licenseExpression', '')
+            license_url = l_vdata.get('licenseUrl', '')
+            if not license_expression:
+                license_expression = license_url
+            return license_expression
+        else:
+            logging.error("Can't obtain data from Nuget Registry")
+            return ''
+
     def construct_download_url(self):
         namespace = (
             self.purl_details['namespace'].replace('%40', '@')
             if self.purl_details['namespace']
             else self.purl_details['name']
         )
-        iniName = namespace[0].lower()
         return (
-            f"https://pypi.python.org/packages/source/{iniName}/{namespace}/"
-            f"{self.purl_details['name']}-"
-            f"{self.purl_details['version']}.tar.gz"
+            f"https://www.nuget.org/api/v2/package/"
+            f"{self.purl_details['name']}/"
+            f"{self.purl_details['version']}"
         )
```

### Comparing `xmonkey_namonica-0.1.7/xmonkey_namonica/utils.py` & `xmonkey_namonica-0.1.8/xmonkey_namonica/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,18 @@
         raise
 
 
 def extract_bz2(file_path, extract_to):
     try:
         if not os.path.exists(extract_to):
             os.makedirs(extract_to)
-        output_file_path = os.path.join(extract_to, os.path.basename(file_path).replace('.bz2', ''))
+        output_file_path = os.path.join(
+            extract_to,
+            os.path.basename(file_path).replace('.bz2', '')
+        )
         with bz2.BZ2File(file_path, 'rb') as file:
             decompressed_data = file.read()
             with open(output_file_path, 'wb') as f_out:
                 f_out.write(decompressed_data)
         remove(file_path)
         logging.info(f"Extracted BZ2 file {file_path} to {output_file_path}")
     except OSError as e:
```

### Comparing `xmonkey_namonica-0.1.7/xmonkey_namonica.egg-info/SOURCES.txt` & `xmonkey_namonica-0.1.8/xmonkey_namonica.egg-info/SOURCES.txt`

 * *Files identical despite different names*

