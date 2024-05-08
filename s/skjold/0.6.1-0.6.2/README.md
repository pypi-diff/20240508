# Comparing `tmp/skjold-0.6.1.tar.gz` & `tmp/skjold-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skjold-0.6.1.tar", max compression
+gzip compressed data, was "skjold-0.6.2.tar", max compression
```

## Comparing `skjold-0.6.1.tar` & `skjold-0.6.2.tar`

### file list

```diff
@@ -1,18 +1,17 @@
--rw-r--r--   0        0        0     1073 2022-12-11 18:06:17.491184 skjold-0.6.1/LICENSE
--rw-r--r--   0        0        0    10452 2022-12-11 18:06:17.491184 skjold-0.6.1/README.md
--rw-r--r--   0        0        0     3203 2022-12-11 18:06:17.491184 skjold-0.6.1/pyproject.toml
--rw-r--r--   0        0        0        0 2022-12-11 18:06:17.491184 skjold-0.6.1/src/skjold/__init__.py
--rw-r--r--   0        0        0     6940 2022-12-11 18:06:17.491184 skjold-0.6.1/src/skjold/cli.py
--rw-r--r--   0        0        0     4719 2022-12-11 18:06:17.491184 skjold-0.6.1/src/skjold/core.py
--rw-r--r--   0        0        0     5411 2022-12-11 18:06:17.491184 skjold-0.6.1/src/skjold/cvss.py
--rw-r--r--   0        0        0     3956 2022-12-11 18:06:17.491184 skjold-0.6.1/src/skjold/formats.py
--rw-r--r--   0        0        0     2267 2022-12-11 18:06:17.491184 skjold-0.6.1/src/skjold/ignore.py
--rw-r--r--   0        0        0      205 2022-12-11 18:06:17.491184 skjold-0.6.1/src/skjold/sources/__init__.py
--rw-r--r--   0        0        0     5304 2022-12-11 18:06:17.491184 skjold-0.6.1/src/skjold/sources/gemnasium.py
--rw-r--r--   0        0        0     6779 2022-12-11 18:06:17.491184 skjold-0.6.1/src/skjold/sources/github.py
--rw-r--r--   0        0        0     4792 2022-12-11 18:06:17.491184 skjold-0.6.1/src/skjold/sources/osv.py
--rw-r--r--   0        0        0     2566 2022-12-11 18:06:17.495183 skjold-0.6.1/src/skjold/sources/pypa.py
--rw-r--r--   0        0        0     4299 2022-12-11 18:06:17.495183 skjold-0.6.1/src/skjold/sources/pyup.py
--rw-r--r--   0        0        0     9985 2022-12-11 18:06:17.495183 skjold-0.6.1/src/skjold/tasks.py
--rw-r--r--   0        0        0    11613 1970-01-01 00:00:00.000000 skjold-0.6.1/setup.py
--rw-r--r--   0        0        0    12217 1970-01-01 00:00:00.000000 skjold-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-05-08 13:40:52.763535 skjold-0.6.2/LICENSE
+-rw-r--r--   0        0        0    10459 2024-05-08 13:40:52.763535 skjold-0.6.2/README.md
+-rw-r--r--   0        0        0     3201 2024-05-08 13:40:52.763535 skjold-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-08 13:40:52.763535 skjold-0.6.2/src/skjold/__init__.py
+-rw-r--r--   0        0        0     6940 2024-05-08 13:40:52.763535 skjold-0.6.2/src/skjold/cli.py
+-rw-r--r--   0        0        0     4719 2024-05-08 13:40:52.763535 skjold-0.6.2/src/skjold/core.py
+-rw-r--r--   0        0        0     5411 2024-05-08 13:40:52.763535 skjold-0.6.2/src/skjold/cvss.py
+-rw-r--r--   0        0        0     3956 2024-05-08 13:40:52.763535 skjold-0.6.2/src/skjold/formats.py
+-rw-r--r--   0        0        0     2267 2024-05-08 13:40:52.763535 skjold-0.6.2/src/skjold/ignore.py
+-rw-r--r--   0        0        0      205 2024-05-08 13:40:52.763535 skjold-0.6.2/src/skjold/sources/__init__.py
+-rw-r--r--   0        0        0     5384 2024-05-08 13:40:52.763535 skjold-0.6.2/src/skjold/sources/gemnasium.py
+-rw-r--r--   0        0        0     6779 2024-05-08 13:40:52.763535 skjold-0.6.2/src/skjold/sources/github.py
+-rw-r--r--   0        0        0     4792 2024-05-08 13:40:52.763535 skjold-0.6.2/src/skjold/sources/osv.py
+-rw-r--r--   0        0        0     2566 2024-05-08 13:40:52.763535 skjold-0.6.2/src/skjold/sources/pypa.py
+-rw-r--r--   0        0        0     4299 2024-05-08 13:40:52.763535 skjold-0.6.2/src/skjold/sources/pyup.py
+-rw-r--r--   0        0        0     9985 2024-05-08 13:40:52.763535 skjold-0.6.2/src/skjold/tasks.py
+-rw-r--r--   0        0        0    12023 1970-01-01 00:00:00.000000 skjold-0.6.2/PKG-INFO
```

### Comparing `skjold-0.6.1/LICENSE` & `skjold-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `skjold-0.6.1/README.md` & `skjold-0.6.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ![](https://img.shields.io/pypi/v/skjold?color=black&label=PyPI&style=flat-square)
-![](https://img.shields.io/github/workflow/status/twu/skjold/Python%20Package/master?color=black&label=Tests&style=flat-square)
+![](https://img.shields.io/github/actions/workflow/status/twu/skjold/test.yml?branch=master&color=black&label=Tests&style=flat-square)
 ![](https://img.shields.io/pypi/status/skjold?color=black&style=flat-square)
 ![](https://img.shields.io/pypi/pyversions/skjold?color=black&logo=python&logoColor=white&style=flat-square)
 ![](https://img.shields.io/pypi/l/skjold?color=black&label=License&style=flat-square)
 ![](https://img.shields.io/pypi/dm/skjold?color=black&label=Downloads&style=flat-square)
 [![](https://api.codeclimate.com/v1/badges/9f756df1ff145e6004a7/maintainability)](https://codeclimate.com/github/twu/skjold/maintainability)
 [![Test Coverage](https://api.codeclimate.com/v1/badges/9f756df1ff145e6004a7/test_coverage)](https://codeclimate.com/github/twu/skjold/test_coverage)
```

### Comparing `skjold-0.6.1/pyproject.toml` & `skjold-0.6.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = 'skjold'
-version = '0.6.1'
+version = '0.6.2'
 description = 'Security audit Python project dependencies against security advisory databases.'
 authors = ["Thomas Wurmitzer <stdin@twu.codes>"]
 packages = [{ include="skjold/**/*.py", from = "src" }]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/twu/skjold"
 repository = "https://github.com/twu/skjold"
@@ -41,28 +41,28 @@
 
 [tool.poetry.scripts]
 skjold = 'skjold.cli:cli'
 
 [tool.poetry.dependencies]
 python = "^3.7"
 click = ">=8,<9"
-packaging = ">=21,<23"
+packaging = ">=21,<24"
 pyyaml = "^6.0"
 toml = ">=0.10.0"
 
 [tool.poetry.dev-dependencies]
 pytest-watch = "^4.2.0"
-pytest-sugar = "^0.9.6"
+pytest-sugar = "^0.9.7"
 pytest-mock = "^3.10.0"
 pre-commit = ">=2.2.0"
 black = ">=22.1.0"
-mypy = "^0.991"
-coverage = {extras = ["toml"], version = "^6"}
+mypy = "^1.3"
+coverage = {extras = ["toml"], version = "^7"}
 pytest-cov = "^4.0.0"
-pytest = "^7.2.0"
+pytest = "^7.4.2"
 types-toml = "^0.10.8"
 types-PyYAML = "^6.0.12"
 
 [tool.skjold]
 report_only = false
 report_format = 'cli'
 sources = ["pyup", "github", "gemnasium", "osv", "pypa"]
```

### Comparing `skjold-0.6.1/src/skjold/cli.py` & `skjold-0.6.2/src/skjold/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #!/usr/bin/env python
-__version__ = "0.6.1"
+__version__ = "0.6.2"
 
 import datetime
 import os
 import sys
 from typing import List, TextIO
 
 import click
```

### Comparing `skjold-0.6.1/src/skjold/core.py` & `skjold-0.6.2/src/skjold/core.py`

 * *Files identical despite different names*

### Comparing `skjold-0.6.1/src/skjold/cvss.py` & `skjold-0.6.2/src/skjold/cvss.py`

 * *Files identical despite different names*

### Comparing `skjold-0.6.1/src/skjold/formats.py` & `skjold-0.6.2/src/skjold/formats.py`

 * *Files identical despite different names*

### Comparing `skjold-0.6.1/src/skjold/ignore.py` & `skjold-0.6.2/src/skjold/ignore.py`

 * *Files identical despite different names*

### Comparing `skjold-0.6.1/src/skjold/sources/gemnasium.py` & `skjold-0.6.2/src/skjold/sources/gemnasium.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,14 @@
 
     @property
     def source(self) -> str:
         return "gemnasium"
 
     @property
     def severity(self) -> str:
-
         for field in ["cvss_v3", "cvss_v2"]:
             vector = self._json.get(field, None)
             if vector:
                 cvss = parse_cvss(vector)
                 return cvss.severity
 
         return "UNKNOWN"
@@ -67,29 +66,32 @@
     def summary(self) -> str:
         return f"{self._json['title']}. {self._json['description']}"
 
     @property
     def vulnerable_version_range(self) -> List[specifiers.SpecifierSet]:
         affected_range = self._json["affected_range"]
 
+        # Gemnasium sometimes uses spaces instead of commas for ranges
+        affected_range = affected_range.strip().replace(" ", ",")
+
         # Gemnasium seems to invalidate/withdraw advisories by marking them this way.
         # See pypi/pyspark/CVE-2020-27218.yml#L11 in gemnasium-db.
         if affected_range in {"(,0)"}:
             return []
 
         if not affected_range:
             return [specifiers.SpecifierSet(">=0.0.0", prereleases=True)]
 
         vulnerable_versions = []
 
         for spec in affected_range.split("||"):
-            # Hotfix for invalid/legacy version specifier: '<2.2.' according to CVE description.
-            # See pypi/Django/CVE-2019-14233.yml#L10 in gemnasium-db.
-            if self.canonical_name == "django" and self.identifier == "CVE-2019-14233":
-                spec = "<2.2.4"
+            # Workaround to ensure that we strip any trailing dots from ranges/specs e.g. >=1.2.,<=2.0.
+            spec = spec.replace(".,", ",")
+            if "," in spec and spec.endswith("."):
+                spec = spec[:-1]
 
             vulnerable_versions.append(specifiers.SpecifierSet(spec, prereleases=True))
         return vulnerable_versions
 
     @property
     def vulnerable_versions(self) -> str:
         return ",".join([str(x) for x in self.vulnerable_version_range])
@@ -100,15 +102,14 @@
             lambda x: True if version_ in x else False
         )
         affected_versions = map(allows_, self.vulnerable_version_range)
         return any(affected_versions)
 
 
 class Gemnasium(SecurityAdvisorySource):
-
     _url = "https://gitlab.com/gitlab-org/security-products/gemnasium-db/-/archive/master/gemnasium-db-master.tar.gz"
     _name = "gemnasium"
 
     @property
     def name(self) -> str:
         return self._name
```

### Comparing `skjold-0.6.1/src/skjold/sources/github.py` & `skjold-0.6.2/src/skjold/sources/github.py`

 * *Files identical despite different names*

### Comparing `skjold-0.6.1/src/skjold/sources/osv.py` & `skjold-0.6.2/src/skjold/sources/osv.py`

 * *Files identical despite different names*

### Comparing `skjold-0.6.1/src/skjold/sources/pypa.py` & `skjold-0.6.2/src/skjold/sources/pypa.py`

 * *Files identical despite different names*

### Comparing `skjold-0.6.1/src/skjold/sources/pyup.py` & `skjold-0.6.2/src/skjold/sources/pyup.py`

 * *Files identical despite different names*

### Comparing `skjold-0.6.1/src/skjold/tasks.py` & `skjold-0.6.2/src/skjold/tasks.py`

 * *Files identical despite different names*

### Comparing `skjold-0.6.1/setup.py` & `skjold-0.6.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,38 +1,253 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: skjold
+Version: 0.6.2
+Summary: Security audit Python project dependencies against security advisory databases.
+Home-page: https://github.com/twu/skjold
+License: MIT
+Keywords: security,security-vulnerability,vulnerability-scanners,vulnerabilities,vulnerability-detection
+Author: Thomas Wurmitzer
+Author-email: stdin@twu.codes
+Requires-Python: >=3.7,<4.0
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Topic :: Security
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: Topic :: Software Development :: Quality Assurance
+Classifier: Topic :: Utilities
+Classifier: Typing :: Typed
+Requires-Dist: click (>=8,<9)
+Requires-Dist: packaging (>=21,<24)
+Requires-Dist: pyyaml (>=6.0,<7.0)
+Requires-Dist: toml (>=0.10.0)
+Project-URL: Bug Tracker, https://github.com/twu/skjold/issues
+Project-URL: Changelog, https://github.com/twu/skjold/releases
+Project-URL: Repository, https://github.com/twu/skjold
+Description-Content-Type: text/markdown
+
+![](https://img.shields.io/pypi/v/skjold?color=black&label=PyPI&style=flat-square)
+![](https://img.shields.io/github/actions/workflow/status/twu/skjold/test.yml?branch=master&color=black&label=Tests&style=flat-square)
+![](https://img.shields.io/pypi/status/skjold?color=black&style=flat-square)
+![](https://img.shields.io/pypi/pyversions/skjold?color=black&logo=python&logoColor=white&style=flat-square)
+![](https://img.shields.io/pypi/l/skjold?color=black&label=License&style=flat-square)
+![](https://img.shields.io/pypi/dm/skjold?color=black&label=Downloads&style=flat-square)
+[![](https://api.codeclimate.com/v1/badges/9f756df1ff145e6004a7/maintainability)](https://codeclimate.com/github/twu/skjold/maintainability)
+[![Test Coverage](https://api.codeclimate.com/v1/badges/9f756df1ff145e6004a7/test_coverage)](https://codeclimate.com/github/twu/skjold/test_coverage)
+
+```
+        .         .    .      Skjold /skjɔl/
+    ,-. | , . ,-. |  ,-|
+    `-. |<  | | | |  | |      Security audit python project dependencies
+    `-' ' ` | `-' `' `-´      against several security advisory databases.
+           `'
+```
+
+## Introduction
+It currently supports fetching advisories from the following sources:
+
+| Source | Name | Notes |
+| ------:|:----:|:------|
+| [GitHub Advisory Database](https://github.com/advisories) | `github` | Requires Access Token (See [Github](#github)). |
+| [PyUP.io safety-db](https://github.com/pyupio/safety-db) | `pyup` | |
+| [GitLab gemnasium-db](https://gitlab.com/gitlab-org/security-products/gemnasium-db) | `gemnasium` | |
+| [PYPA Advisory Database](https://github.com/pypa/advisory-db) | `pypa` | Only supports `ECOSYSTEM`! |
+| [OSV.dev Database](https://osv.dev) | `osv` | Only supports `ECOSYSTEM`!<br/> Sends package information to [OSV.dev](https://osv.dev) API. |
+
+No source is enabled by default! Sources can be enabled by setting `sources` list (see [Configuration](#configuration)). There is (currently) no de-duplication meaning that using too many sources at once will result in _a lot_ of duplicates. `skjold` also requires _all_ dependencies to be passed as it *will not* resolve any dependencies at runtime!
+
+## Motivation
+Skjold was initially created for myself to replace `safety`. ~Which appears to no longer receive monthly updates (see [pyupio/safety-db #2282](https://github.com/pyupio/safety-db/issues/2282))~. I wanted something I can run locally and use for my local or private projects/scripts.
+
+I currently also use it during CI builds and before deploying/publishing containers or packages.
+
+## Installation
+`skjold` can be installed from either [PyPI](https://pypi.org/project/skjold/) or directly from [Github](https://github.com/twu/skjold) using `pip`:
+
+```sh
+pip install skjold                                        # Install from PyPI
+pip install git+https://github.com/twu/skjold.git@vX.X.X  # Install from Github
+```
+
+This should provide a script named `skjold` that can then be invoked. See [Usage](#usage).
+
+## Usage
+```sh
+$ pip list --format=freeze | skjold -v audit --sources gemnasium -
+```
+
+When running `audit` one can either provide a path to a _frozen_ `requirements.txt`, a `poetry.lock` or a `Pipfile.lock` file. Alternatively, dependencies can also be passed in via `stdin`  (formatted as `package==version`).
+
+`skjold` will maintain a local cache (under `cache_dir`) that will expire automatically after `cache_expires` has passed. The `cache_dir` and `cache_expires` can be adjusted by setting them in  `tools.skjold` section of the projects `pyproject.toml` (see [Configuration](#configuration) for more details). The `cache_dir`will be created automatically, and by default unless otherwise specified will be located under `$HOME/.skjold/cache`.
+
+For further options please read `skjold --help` and/or `skjold audit --help`.
+
+### Examples
+
+All examples involving `github` assume that `SKJOLD_GITHUB_API_TOKEN` is already set (see [Github](#github)).
+
+```sh
+# Using pip list. Checking against GitHub only.
+$ pip list --format=freeze | skjold audit -s github -
+
+# Be verbose. Read directly from supported formats.
+$ skjold -v audit requirements.txt
+$ skjold -v audit poetry.lock
+$ skjold -v audit Pipenv.lock
+
+# Specify specify multiple inputs at once.
+$ skjold -v audit Pipenv.lock poetry.lock requirements.txt
+
+# Using poetry.
+$ poetry export -f requirements.txt | skjold audit -s github -s gemnasium -s pyup -
+
+# Using poetry, format output as json and pass it on to jq for additional filtering.
+$ poetry export -f requirements.txt | skjold audit -o json -s github - | jq '.[0]'
+
+# Using Pipenv, checking against Github
+$ pipenv run pip list --format=freeze | skjold audit -s github -
+
+# Checking a single package via stdin against Github and format findings as json.
+$ echo "urllib3==1.23" | skjold audit -o json -r -s github -
+[
+  {
+    "severity": "HIGH",
+    "name": "urllib3",
+    "version": "1.23",
+    "versions": "<1.24.2",
+    "source": "github",
+    "summary": "High severity vulnerability that affects urllib3",
+    "references": [
+      "https://nvd.nist.gov/vuln/detail/CVE-2019-11324"
+    ],
+    "url": "https://github.com/advisories/GHSA-mh33-7rrq-662w"
+  }
+]
+
+# Checking a single package via stdin against Gemnasium and report findings (`-o cli`).
+$ echo "urllib3==1.23" | skjold audit -o cli -r -s gemnasium -
+
+urllib3==1.23 (<=1.24.2) via gemnasium
+
+CRLF injection. In the urllib3 library for Python, CRLF injection is possible
+if the attacker controls the request parameter.
+https://nvd.nist.gov/vuln/detail/CVE-2019-11236
+--
+
+urllib3==1.23 (<1.24.2) via gemnasium
+
+Weak Authentication Caused By Improper Certificate Validation. The urllib3
+library for Python mishandles certain cases where the desired set of CA
+certificates is different from the OS store of CA certificates, which results
+in SSL connections succeeding in situations where a verification failure is the
+correct outcome. This is related to use of the `ssl_context`, `ca_certs`, or
+`ca_certs_dir` argument.
+https://nvd.nist.gov/vuln/detail/CVE-2019-11324
+--
+
+urllib3==1.23 (<1.25.9) via gemnasium
+
+Injection Vulnerability. urllib3 allows CRLF injection if the attacker controls
+the HTTP request method, as demonstrated by inserting `CR` and `LF` control
+characters in the first argument of `putrequest()`. NOTE: this is similar to
+CVE-2020-26116.
+https://nvd.nist.gov/vuln/detail/CVE-2020-26137
+--
+```
+
+#### Ignore Findings
+
+Findings can be ignored either by manually adding an entry using the sources identifier to a file named `.skjoldignore` (See [Example](https://github.com/twu/skjold/blob/master/.skjoldignore)) or by using in the CLI. Below are a few possible usage examples.
+
+```
+# Ignore PYSEC-2020-148 finding from PyPA source until a certain date with a specific reason.
+$ skjold ignore urllib3 PYSEC-2020-148 --reason "Very good reason." --expires "2021-01-01T00:00:00+00:00"
+Ignore urllib3 in PYSEC-2020-148 until 2021-01-01 00:00:00+00:00?
+Very good reason.
+--
+Add to '.skjoldignore'? [y/N]: y
+
+# Ignore PYSEC-2020-148 finding from PyPA source for 7 days with "No immediate remediation." reason.
+$ skjold ignore urllib3 PYSEC-2020-148
+Ignore urllib3 in PYSEC-2020-148 until ...?
+No immediate remediation.
+--
+Add to '.skjoldignore'? [y/N]: y
+
+# Audit `poetry.lock` using a custom `.skjoldignore` file location via `ENV`...
+$ SKJOLD_IGNORE_FILE=<path-to-file> skjold audit -s pyup poetry.lock
+
+# ... or using -i/--ignore-file
+$ skjold audit -s pyup -i <path-to-file> poetry.lock
+```
+
+### Configuration
+
+`skjold` can read its configuration from the `tools.skjold` section of a projects  `pyproject.toml`. Arguments specified via the command-line should take precedence over any configured or default value.
+
+```toml
+[tool.skjold]
+sources = ["github", "pyup", "gemnasium"]  # Sources to check against.
+report_only = false                        # Exit with non-zero exit code on findings.
+report_format = 'json'                     # Output findings as `json`. Default is 'cli'.
+cache_dir = '.skjold_cache'                # Cache location (default: `~/.skjold/cache`).
+cache_expires = 86400                      # Cache max. age.
+ignore_file = '.skjoldignore'              # Ignorefile location (default `.skjoldignore`).
+verbose = true                             # Be verbose.
+```
+
+To take a look at the current configuration / defaults run:
+```shell
+$ skjold config
+sources: ['pyup', 'github', 'gemnasium']
+report_only: False
+report_format: json
+verbose: False
+cache_dir: .skjold_cache
+cache_expires: 86400
+ignore_file = '.skjoldignore'
+```
+
+#### Github
+
+For the `github` source to work you'll need to provide a Github API Token via an `ENV` variable named `SKJOLD_GITHUB_API_TOKEN`. You can [create a new Github Access Token here](https://github.com/settings/tokens). You *do not* have to give it *any* permissions as it is only required to query the [GitHub GraphQL API v4](https://developer.github.com/v4/) API.
+
+### Version Control Integration
+To use `skjold` with the excellent [pre-commit](https://pre-commit.com/) framework add the following to the projects `.pre-commit-config.yaml` after [installation](https://pre-commit.com/#install).
+
+```yaml
+repos:
+  - repo: https://github.com/twu/skjold
+    rev: vX.X.X
+    hooks:
+    - id: skjold
+      verbose: true  # Important if used with `report_only`, see below.
+```
+
+After running `pre-commit install` the hook should be good to go. To configure `skjold` in this scenario I recommend adding the entire configuration to the projects `pyproject.toml` instead of manipulating the hook `args`. See this projects [pyproject.toml](./pyproject.toml) for an example.
+
+> **Important!**: When using `skjold` as a `pre-commit`-hook it only gets triggered if you want to commit changed dependency files (e.g. `Pipenv.lock`, `poetry.lock`, `requirements.txt`,...).
+> It will not continuously check your dependencies on _every_ commit!
+
+You could run `pre-commit run skjold --all-files` manually in your workflow/scripts or run `skjold` manually.
+If you have a better solution please let me know!
+
+> **Important!**: If you use `report_only` in any way make sure that you add `verbose: true` to your hook configuration
+otherwise `pre-commit` won't show you any output since the hook is always returning with a zero exit code due
+to `report_only` being set!
 
-package_dir = \
-{'': 'src'}
+## Contributing
+Pull requests are welcome! For major changes, please open an issue first to discuss what you would like to change.
 
-packages = \
-['skjold', 'skjold.sources']
+Please make sure to update tests as appropriate.
 
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['click>=8,<9', 'packaging>=21,<23', 'pyyaml>=6.0,<7.0', 'toml>=0.10.0']
-
-entry_points = \
-{'console_scripts': ['skjold = skjold.cli:cli']}
-
-setup_kwargs = {
-    'name': 'skjold',
-    'version': '0.6.1',
-    'description': 'Security audit Python project dependencies against security advisory databases.',
-    'long_description': '![](https://img.shields.io/pypi/v/skjold?color=black&label=PyPI&style=flat-square)\n![](https://img.shields.io/github/workflow/status/twu/skjold/Python%20Package/master?color=black&label=Tests&style=flat-square)\n![](https://img.shields.io/pypi/status/skjold?color=black&style=flat-square)\n![](https://img.shields.io/pypi/pyversions/skjold?color=black&logo=python&logoColor=white&style=flat-square)\n![](https://img.shields.io/pypi/l/skjold?color=black&label=License&style=flat-square)\n![](https://img.shields.io/pypi/dm/skjold?color=black&label=Downloads&style=flat-square)\n[![](https://api.codeclimate.com/v1/badges/9f756df1ff145e6004a7/maintainability)](https://codeclimate.com/github/twu/skjold/maintainability)\n[![Test Coverage](https://api.codeclimate.com/v1/badges/9f756df1ff145e6004a7/test_coverage)](https://codeclimate.com/github/twu/skjold/test_coverage)\n\n```\n        .         .    .      Skjold /skjɔl/\n    ,-. | , . ,-. |  ,-|\n    `-. |<  | | | |  | |      Security audit python project dependencies\n    `-\' \' ` | `-\' `\' `-´      against several security advisory databases.\n           `\'\n```\n\n## Introduction\nIt currently supports fetching advisories from the following sources:\n\n| Source | Name | Notes |\n| ------:|:----:|:------|\n| [GitHub Advisory Database](https://github.com/advisories) | `github` | Requires Access Token (See [Github](#github)). |\n| [PyUP.io safety-db](https://github.com/pyupio/safety-db) | `pyup` | |\n| [GitLab gemnasium-db](https://gitlab.com/gitlab-org/security-products/gemnasium-db) | `gemnasium` | |\n| [PYPA Advisory Database](https://github.com/pypa/advisory-db) | `pypa` | Only supports `ECOSYSTEM`! |\n| [OSV.dev Database](https://osv.dev) | `osv` | Only supports `ECOSYSTEM`!<br/> Sends package information to [OSV.dev](https://osv.dev) API. |\n\nNo source is enabled by default! Sources can be enabled by setting `sources` list (see [Configuration](#configuration)). There is (currently) no de-duplication meaning that using too many sources at once will result in _a lot_ of duplicates. `skjold` also requires _all_ dependencies to be passed as it *will not* resolve any dependencies at runtime!\n\n## Motivation\nSkjold was initially created for myself to replace `safety`. ~Which appears to no longer receive monthly updates (see [pyupio/safety-db #2282](https://github.com/pyupio/safety-db/issues/2282))~. I wanted something I can run locally and use for my local or private projects/scripts.\n\nI currently also use it during CI builds and before deploying/publishing containers or packages.\n\n## Installation\n`skjold` can be installed from either [PyPI](https://pypi.org/project/skjold/) or directly from [Github](https://github.com/twu/skjold) using `pip`:\n\n```sh\npip install skjold                                        # Install from PyPI\npip install git+https://github.com/twu/skjold.git@vX.X.X  # Install from Github\n```\n\nThis should provide a script named `skjold` that can then be invoked. See [Usage](#usage).\n\n## Usage\n```sh\n$ pip list --format=freeze | skjold -v audit --sources gemnasium -\n```\n\nWhen running `audit` one can either provide a path to a _frozen_ `requirements.txt`, a `poetry.lock` or a `Pipfile.lock` file. Alternatively, dependencies can also be passed in via `stdin`  (formatted as `package==version`).\n\n`skjold` will maintain a local cache (under `cache_dir`) that will expire automatically after `cache_expires` has passed. The `cache_dir` and `cache_expires` can be adjusted by setting them in  `tools.skjold` section of the projects `pyproject.toml` (see [Configuration](#configuration) for more details). The `cache_dir`will be created automatically, and by default unless otherwise specified will be located under `$HOME/.skjold/cache`.\n\nFor further options please read `skjold --help` and/or `skjold audit --help`.\n\n### Examples\n\nAll examples involving `github` assume that `SKJOLD_GITHUB_API_TOKEN` is already set (see [Github](#github)).\n\n```sh\n# Using pip list. Checking against GitHub only.\n$ pip list --format=freeze | skjold audit -s github -\n\n# Be verbose. Read directly from supported formats.\n$ skjold -v audit requirements.txt\n$ skjold -v audit poetry.lock\n$ skjold -v audit Pipenv.lock\n\n# Specify specify multiple inputs at once.\n$ skjold -v audit Pipenv.lock poetry.lock requirements.txt\n\n# Using poetry.\n$ poetry export -f requirements.txt | skjold audit -s github -s gemnasium -s pyup -\n\n# Using poetry, format output as json and pass it on to jq for additional filtering.\n$ poetry export -f requirements.txt | skjold audit -o json -s github - | jq \'.[0]\'\n\n# Using Pipenv, checking against Github\n$ pipenv run pip list --format=freeze | skjold audit -s github -\n\n# Checking a single package via stdin against Github and format findings as json.\n$ echo "urllib3==1.23" | skjold audit -o json -r -s github -\n[\n  {\n    "severity": "HIGH",\n    "name": "urllib3",\n    "version": "1.23",\n    "versions": "<1.24.2",\n    "source": "github",\n    "summary": "High severity vulnerability that affects urllib3",\n    "references": [\n      "https://nvd.nist.gov/vuln/detail/CVE-2019-11324"\n    ],\n    "url": "https://github.com/advisories/GHSA-mh33-7rrq-662w"\n  }\n]\n\n# Checking a single package via stdin against Gemnasium and report findings (`-o cli`).\n$ echo "urllib3==1.23" | skjold audit -o cli -r -s gemnasium -\n\nurllib3==1.23 (<=1.24.2) via gemnasium\n\nCRLF injection. In the urllib3 library for Python, CRLF injection is possible\nif the attacker controls the request parameter.\nhttps://nvd.nist.gov/vuln/detail/CVE-2019-11236\n--\n\nurllib3==1.23 (<1.24.2) via gemnasium\n\nWeak Authentication Caused By Improper Certificate Validation. The urllib3\nlibrary for Python mishandles certain cases where the desired set of CA\ncertificates is different from the OS store of CA certificates, which results\nin SSL connections succeeding in situations where a verification failure is the\ncorrect outcome. This is related to use of the `ssl_context`, `ca_certs`, or\n`ca_certs_dir` argument.\nhttps://nvd.nist.gov/vuln/detail/CVE-2019-11324\n--\n\nurllib3==1.23 (<1.25.9) via gemnasium\n\nInjection Vulnerability. urllib3 allows CRLF injection if the attacker controls\nthe HTTP request method, as demonstrated by inserting `CR` and `LF` control\ncharacters in the first argument of `putrequest()`. NOTE: this is similar to\nCVE-2020-26116.\nhttps://nvd.nist.gov/vuln/detail/CVE-2020-26137\n--\n```\n\n#### Ignore Findings\n\nFindings can be ignored either by manually adding an entry using the sources identifier to a file named `.skjoldignore` (See [Example](https://github.com/twu/skjold/blob/master/.skjoldignore)) or by using in the CLI. Below are a few possible usage examples.\n\n```\n# Ignore PYSEC-2020-148 finding from PyPA source until a certain date with a specific reason.\n$ skjold ignore urllib3 PYSEC-2020-148 --reason "Very good reason." --expires "2021-01-01T00:00:00+00:00"\nIgnore urllib3 in PYSEC-2020-148 until 2021-01-01 00:00:00+00:00?\nVery good reason.\n--\nAdd to \'.skjoldignore\'? [y/N]: y\n\n# Ignore PYSEC-2020-148 finding from PyPA source for 7 days with "No immediate remediation." reason.\n$ skjold ignore urllib3 PYSEC-2020-148\nIgnore urllib3 in PYSEC-2020-148 until ...?\nNo immediate remediation.\n--\nAdd to \'.skjoldignore\'? [y/N]: y\n\n# Audit `poetry.lock` using a custom `.skjoldignore` file location via `ENV`...\n$ SKJOLD_IGNORE_FILE=<path-to-file> skjold audit -s pyup poetry.lock\n\n# ... or using -i/--ignore-file\n$ skjold audit -s pyup -i <path-to-file> poetry.lock\n```\n\n### Configuration\n\n`skjold` can read its configuration from the `tools.skjold` section of a projects  `pyproject.toml`. Arguments specified via the command-line should take precedence over any configured or default value.\n\n```toml\n[tool.skjold]\nsources = ["github", "pyup", "gemnasium"]  # Sources to check against.\nreport_only = false                        # Exit with non-zero exit code on findings.\nreport_format = \'json\'                     # Output findings as `json`. Default is \'cli\'.\ncache_dir = \'.skjold_cache\'                # Cache location (default: `~/.skjold/cache`).\ncache_expires = 86400                      # Cache max. age.\nignore_file = \'.skjoldignore\'              # Ignorefile location (default `.skjoldignore`).\nverbose = true                             # Be verbose.\n```\n\nTo take a look at the current configuration / defaults run:\n```shell\n$ skjold config\nsources: [\'pyup\', \'github\', \'gemnasium\']\nreport_only: False\nreport_format: json\nverbose: False\ncache_dir: .skjold_cache\ncache_expires: 86400\nignore_file = \'.skjoldignore\'\n```\n\n#### Github\n\nFor the `github` source to work you\'ll need to provide a Github API Token via an `ENV` variable named `SKJOLD_GITHUB_API_TOKEN`. You can [create a new Github Access Token here](https://github.com/settings/tokens). You *do not* have to give it *any* permissions as it is only required to query the [GitHub GraphQL API v4](https://developer.github.com/v4/) API.\n\n### Version Control Integration\nTo use `skjold` with the excellent [pre-commit](https://pre-commit.com/) framework add the following to the projects `.pre-commit-config.yaml` after [installation](https://pre-commit.com/#install).\n\n```yaml\nrepos:\n  - repo: https://github.com/twu/skjold\n    rev: vX.X.X\n    hooks:\n    - id: skjold\n      verbose: true  # Important if used with `report_only`, see below.\n```\n\nAfter running `pre-commit install` the hook should be good to go. To configure `skjold` in this scenario I recommend adding the entire configuration to the projects `pyproject.toml` instead of manipulating the hook `args`. See this projects [pyproject.toml](./pyproject.toml) for an example.\n\n> **Important!**: When using `skjold` as a `pre-commit`-hook it only gets triggered if you want to commit changed dependency files (e.g. `Pipenv.lock`, `poetry.lock`, `requirements.txt`,...).\n> It will not continuously check your dependencies on _every_ commit!\n\nYou could run `pre-commit run skjold --all-files` manually in your workflow/scripts or run `skjold` manually.\nIf you have a better solution please let me know!\n\n> **Important!**: If you use `report_only` in any way make sure that you add `verbose: true` to your hook configuration\notherwise `pre-commit` won\'t show you any output since the hook is always returning with a zero exit code due\nto `report_only` being set!\n\n## Contributing\nPull requests are welcome! For major changes, please open an issue first to discuss what you would like to change.\n\nPlease make sure to update tests as appropriate.\n\n',
-    'author': 'Thomas Wurmitzer',
-    'author_email': 'stdin@twu.codes',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/twu/skjold',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.7,<4.0',
-}
 
-
-setup(**setup_kwargs)
```

