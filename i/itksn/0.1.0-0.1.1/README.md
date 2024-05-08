# Comparing `tmp/itksn-0.1.0.tar.gz` & `tmp/itksn-0.1.1.tar.gz`

## Comparing `itksn-0.1.0.tar` & `itksn-0.1.1.tar`

### file list

```diff
@@ -1,45 +1,46 @@
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 itksn-0.1.0/.bumpversion.cfg
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 itksn-0.1.0/.coveragerc
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 itksn-0.1.0/.git_archival.txt
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 itksn-0.1.0/.gitattributes
--rw-r--r--   0        0        0     2155 2020-02-02 00:00:00.000000 itksn-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 itksn-0.1.0/.zenodo.json
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 itksn-0.1.0/CITATION.cff
--rw-r--r--   0        0        0     3217 2020-02-02 00:00:00.000000 itksn-0.1.0/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 itksn-0.1.0/MANIFEST.in
--rw-r--r--   0        0        0     4227 2020-02-02 00:00:00.000000 itksn-0.1.0/mkdocs.yml
--rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 itksn-0.1.0/tbump.toml
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 itksn-0.1.0/.github/dependabot.yml
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 itksn-0.1.0/.github/matchers/pylint.json
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 itksn-0.1.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 itksn-0.1.0/.github/workflows/docs.yml
--rw-r--r--   0        0        0     3376 2020-02-02 00:00:00.000000 itksn-0.1.0/.github/workflows/publish-package.yml
--rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 itksn-0.1.0/docs/gen_ref_nav.py
--rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 itksn-0.1.0/docs/index.md
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 itksn-0.1.0/docs/install.md
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 itksn-0.1.0/docs/.overrides/main.html
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 itksn-0.1.0/docs/.snippets/abbrs.txt
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 itksn-0.1.0/docs/.snippets/links.txt
--rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 itksn-0.1.0/docs/assets/css/custom.css
--rw-r--r--   0        0        0    12804 2020-02-02 00:00:00.000000 itksn-0.1.0/docs/assets/images/logo.svg
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 itksn-0.1.0/docs/cli/about.md
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 itksn-0.1.0/docs/cli/reference.md
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 itksn-0.1.0/docs/meta/authors.md
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 itksn-0.1.0/docs/meta/faq.md
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 itksn-0.1.0/src/itksn/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 itksn-0.1.0/src/itksn/_version.py
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 itksn-0.1.0/src/itksn/_version.pyi
--rw-r--r--   0        0        0     6110 2020-02-02 00:00:00.000000 itksn-0.1.0/src/itksn/core.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 itksn-0.1.0/src/itksn/py.typed
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 itksn-0.1.0/src/itksn/cli/__init__.py
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 itksn-0.1.0/src/itksn/cli/__main__.py
--rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 itksn-0.1.0/src/itksn/cli/main.py
--rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 itksn-0.1.0/tests/test_cli.py
--rw-r--r--   0        0        0     3831 2020-02-02 00:00:00.000000 itksn-0.1.0/tests/test_core.py
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 itksn-0.1.0/tests/test_import.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 itksn-0.1.0/tests/test_package.py
--rw-r--r--   0        0        0     2071 2020-02-02 00:00:00.000000 itksn-0.1.0/.gitignore
--rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 itksn-0.1.0/LICENSE
--rw-r--r--   0        0        0     6022 2020-02-02 00:00:00.000000 itksn-0.1.0/README.md
--rw-r--r--   0        0        0     6216 2020-02-02 00:00:00.000000 itksn-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     7814 2020-02-02 00:00:00.000000 itksn-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 itksn-0.1.1/.coveragerc
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 itksn-0.1.1/.git_archival.txt
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 itksn-0.1.1/.gitattributes
+-rw-r--r--   0        0        0     2254 2020-02-02 00:00:00.000000 itksn-0.1.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 itksn-0.1.1/.zenodo.json
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 itksn-0.1.1/CITATION.cff
+-rw-r--r--   0        0        0     3217 2020-02-02 00:00:00.000000 itksn-0.1.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 itksn-0.1.1/MANIFEST.in
+-rw-r--r--   0        0        0     4227 2020-02-02 00:00:00.000000 itksn-0.1.1/mkdocs.yml
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 itksn-0.1.1/run.py
+-rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 itksn-0.1.1/tbump.toml
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 itksn-0.1.1/.github/dependabot.yml
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 itksn-0.1.1/.github/matchers/pylint.json
+-rw-r--r--   0        0        0     2067 2020-02-02 00:00:00.000000 itksn-0.1.1/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 itksn-0.1.1/.github/workflows/docs.yml
+-rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 itksn-0.1.1/docs/gen_ref_nav.py
+-rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 itksn-0.1.1/docs/index.md
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 itksn-0.1.1/docs/install.md
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 itksn-0.1.1/docs/.overrides/main.html
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 itksn-0.1.1/docs/.snippets/abbrs.txt
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 itksn-0.1.1/docs/.snippets/links.txt
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 itksn-0.1.1/docs/assets/css/custom.css
+-rw-r--r--   0        0        0    12804 2020-02-02 00:00:00.000000 itksn-0.1.1/docs/assets/images/logo.svg
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 itksn-0.1.1/docs/cli/about.md
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 itksn-0.1.1/docs/cli/reference.md
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 itksn-0.1.1/docs/meta/authors.md
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 itksn-0.1.1/docs/meta/faq.md
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 itksn-0.1.1/src/itksn/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 itksn-0.1.1/src/itksn/_version.py
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 itksn-0.1.1/src/itksn/_version.pyi
+-rw-r--r--   0        0        0     3131 2020-02-02 00:00:00.000000 itksn-0.1.1/src/itksn/common.py
+-rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 itksn-0.1.1/src/itksn/core.py
+-rw-r--r--   0        0        0     4927 2020-02-02 00:00:00.000000 itksn-0.1.1/src/itksn/pixels.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 itksn-0.1.1/src/itksn/py.typed
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 itksn-0.1.1/src/itksn/cli/__init__.py
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 itksn-0.1.1/src/itksn/cli/__main__.py
+-rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 itksn-0.1.1/src/itksn/cli/main.py
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 itksn-0.1.1/tests/test_cli.py
+-rw-r--r--   0        0        0     3834 2020-02-02 00:00:00.000000 itksn-0.1.1/tests/test_core.py
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 itksn-0.1.1/tests/test_import.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 itksn-0.1.1/tests/test_package.py
+-rw-r--r--   0        0        0     2071 2020-02-02 00:00:00.000000 itksn-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 itksn-0.1.1/LICENSE
+-rw-r--r--   0        0        0     6022 2020-02-02 00:00:00.000000 itksn-0.1.1/README.md
+-rw-r--r--   0        0        0     6013 2020-02-02 00:00:00.000000 itksn-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     7765 2020-02-02 00:00:00.000000 itksn-0.1.1/PKG-INFO
```

### Comparing `itksn-0.1.0/.pre-commit-config.yaml` & `itksn-0.1.1/.pre-commit-config.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 ci:
   autoupdate_commit_msg: "chore: update pre-commit hooks"
   autofix_commit_msg: "style: pre-commit fixes"
 
 repos:
   - repo: https://github.com/psf/black
-    rev: "23.1.0"
+    rev: "24.3.0"
     hooks:
       - id: black-jupyter
 
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: "v4.4.0"
+    rev: "v4.6.0"
     hooks:
       - id: check-added-large-files
       - id: check-case-conflict
       - id: check-merge-conflict
       - id: check-symlinks
       - id: check-yaml
         exclude: mkdocs.yml
@@ -33,47 +33,48 @@
     rev: "v1.10.0"
     hooks:
       - id: rst-backticks
       - id: rst-directive-colons
       - id: rst-inline-touching-normal
 
   - repo: https://github.com/pre-commit/mirrors-prettier
-    rev: "v3.0.0-alpha.4"
+    rev: "v4.0.0-alpha.8"
     hooks:
       - id: prettier
+        entry: env PRETTIER_LEGACY_CLI=1 prettier  #  https://github.com/prettier/prettier/issues/15742
         types_or: [yaml, markdown, html, css, scss, javascript, json]
         args: [--prose-wrap=always]
 
   - repo: https://github.com/asottile/blacken-docs
-    rev: "1.13.0"
+    rev: "1.16.0"
     hooks:
       - id: blacken-docs
         additional_dependencies: [black==22.8.0]
 
-  - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: v0.0.246
+  - repo: https://github.com/astral-sh/ruff-pre-commit
+    rev: v0.3.5
     hooks:
       - id: ruff
         args: ["--fix", "--show-fixes"]
 
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: "v1.0.0"
+    rev: "v1.9.0"
     hooks:
       - id: mypy
         files: src
         args: []
         additional_dependencies: ["typer", "construct-typing"]
 
   - repo: https://github.com/codespell-project/codespell
-    rev: v2.2.2
+    rev: v2.2.6
     hooks:
       - id: codespell
 
   - repo: https://github.com/shellcheck-py/shellcheck-py
-    rev: "v0.9.0.2"
+    rev: "v0.10.0.1"
     hooks:
       - id: shellcheck
 
   - repo: local
     hooks:
       - id: disallow-caps
         name: Disallow improper capitalization
```

### Comparing `itksn-0.1.0/.zenodo.json` & `itksn-0.1.1/.zenodo.json`

 * *Files 25% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8796296296296297%*

 * *Differences: {"'related_identifiers'": "{0: {'identifier': 'https://github.com/kratsg/itksn/tree/v0.1.1'}}",*

 * * "'title'": "'itksn: v0.1.1'",*

 * * "'version'": "'v0.1.1'"}*

```diff
@@ -13,16 +13,16 @@
         "physics",
         "construct",
         "parsing"
     ],
     "license": "BSD-3.0",
     "related_identifiers": [
         {
-            "identifier": "https://github.com/kratsg/itksn/tree/v0.1.0",
+            "identifier": "https://github.com/kratsg/itksn/tree/v0.1.1",
             "relation": "isSupplementTo",
             "scheme": "url"
         }
     ],
-    "title": "itksn: v0.1.0",
+    "title": "itksn: v0.1.1",
     "upload_type": "software",
-    "version": "v0.1.0"
+    "version": "v0.1.1"
 }
```

### Comparing `itksn-0.1.0/CITATION.cff` & `itksn-0.1.1/CITATION.cff`

 * *Files 20% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 message: "Please cite the following works when using this software."
 type: software
 authors:
 - family-names: "Stark"
   given-names: "Giordon"
   orcid: "https://orcid.org/0000-0001-6616-3433"
   affiliation: "SCIPP, University of California, Santa Cruz"
-title: "itksn: v0.1.0"
-version: 0.1.0
+title: "itksn: v0.1.1"
+version: 0.1.1
 doi: 10.5281/zenodo.7644145
-repository-code: "https://github.com/kratsg/itksn/releases/tag/v0.1.0"
-url: "https://kratsg.github.io/itksn/0.1.0/"
+repository-code: "https://github.com/kratsg/itksn/releases/tag/v0.1.1"
+url: "https://kratsg.github.io/itksn/0.1.1/"
 keywords:
   - python
   - physics
   - construct
   - parsing
 license: "BSD-3.0"
 abstract: |
```

### Comparing `itksn-0.1.0/CODE_OF_CONDUCT.md` & `itksn-0.1.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `itksn-0.1.0/mkdocs.yml` & `itksn-0.1.1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `itksn-0.1.0/tbump.toml` & `itksn-0.1.1/tbump.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 github_url = "https://github.com/kratsg/itksn/"
 
 [version]
-current = "0.1.0"
+current = "0.1.1"
 
 # Example of a semver regexp.
 # Make sure this matches current_version before
 # using tbump
 regex = '''
   (?P<major>\d+)
   \.
@@ -15,15 +15,15 @@
   (rc
     (?P<candidate>\d+)
   )?
   '''
 
 [git]
 # The current version will get updated when tbump is run
-message_template = "Bump version: 0.1.0 → {new_version}"
+message_template = "Bump version: 0.1.1 → {new_version}"
 tag_template = "v{new_version}"
 
 # For each file to patch, add a [[file]] config
 # section containing the path of the file, relative to the
 # tbump.toml location.
 [[file]]
 src = "tbump.toml"
```

### Comparing `itksn-0.1.0/.github/matchers/pylint.json` & `itksn-0.1.1/.github/matchers/pylint.json`

 * *Files identical despite different names*

### Comparing `itksn-0.1.0/.github/workflows/ci.yml` & `itksn-0.1.1/.github/workflows/ci.yml`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
   cancel-in-progress: true
 
 jobs:
   pre-commit:
     name: Format
     runs-on: ubuntu-latest
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
         with:
           fetch-depth: 0
       - uses: actions/setup-python@v4
         with:
           python-version: "3.x"
       - uses: pre-commit/action@v3.0.0
         with:
@@ -38,23 +38,23 @@
   checks:
     name: Check Python ${{ matrix.python-version }} on ${{ matrix.runs-on }}
     runs-on: ${{ matrix.runs-on }}
     needs: [pre-commit]
     strategy:
       fail-fast: false
       matrix:
-        python-version: ["3.7", "3.10"]
+        python-version: ["3.8", "3.11"]
         runs-on: [ubuntu-latest, macos-latest, windows-latest]
 
         include:
           - python-version: pypy3.8
             runs-on: ubuntu-latest
 
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
         with:
           fetch-depth: 0
 
       - uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
 
@@ -63,24 +63,24 @@
 
   dist:
     name: Distribution build
     runs-on: ubuntu-latest
     needs: [pre-commit]
 
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
         with:
           fetch-depth: 0
 
       - name: Build sdist and wheel; and check products
         run: pipx run hatch run build-check
 
       - uses: actions/upload-artifact@v3
         with:
           path: dist
 
-      - uses: pypa/gh-action-pypi-publish@v1.6.4
+      - uses: pypa/gh-action-pypi-publish@v1.8.10
         if: github.event_name == 'release' && github.event.action == 'published'
         with:
           user: __token__
           # Remember to generate this and set it in "GitHub Secrets"
           password: ${{ secrets.pypi_password }}
```

### Comparing `itksn-0.1.0/.github/workflows/docs.yml` & `itksn-0.1.1/.github/workflows/docs.yml`

 * *Files 4% similar despite different names*

```diff
@@ -15,29 +15,29 @@
   group: ${{ github.workflow }}-${{ github.ref }}
   cancel-in-progress: true
 
 jobs:
   build:
     runs-on: ubuntu-latest
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
         with:
           fetch-depth: 0
       - uses: actions/setup-python@v4
         with:
           python-version: "3.x"
 
       - name: Check documentation
         run: pipx run hatch run docs:build-check
 
   publish:
     runs-on: ubuntu-latest
     needs: [build]
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
         with:
           fetch-depth: 0
       - uses: actions/setup-python@v4
         with:
           python-version: "3.x"
 
       - name: Configure Git for GitHub Actions bot
```

### Comparing `itksn-0.1.0/docs/gen_ref_nav.py` & `itksn-0.1.1/docs/gen_ref_nav.py`

 * *Files identical despite different names*

### Comparing `itksn-0.1.0/docs/index.md` & `itksn-0.1.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `itksn-0.1.0/docs/install.md` & `itksn-0.1.1/docs/install.md`

 * *Files 4% similar despite different names*

```diff
@@ -2,50 +2,50 @@
 
 ---
 
 ## pip
 
 itksn is available on PyPI and can be installed with [pip](https://pip.pypa.io).
 
-```
+```bash
 pip install itksn
 ```
 
 <!-- prettier-ignore -->
 !!! warning
     This method modifies the Python environment in which you choose to install. Consider instead using [pipx](#pipx) or virtual environments to avoid dependency conflicts.
 
 ## pipx
 
 [pipx](https://github.com/pypa/pipx) allows for the global installation of
 Python applications in isolated environments.
 
-```
+```bash
 pipx install itksn
 ```
 
 ## virtual environment
 
-```
+```bash
 python -m venv venv
 source venv/bin/activate
 python -m pip install itksn
 ```
 
 ## Conda
 
 See the [feedstock](https://github.com/conda-forge/itksn-feedstock) for more
 details.
 
-```
+```bash
 conda install -c conda-forge itksn
 ```
 
 or with [mamba](https://github.com/mamba-org/mamba):
 
-```
+```bash
 mamba install itksn
 ```
 
 <!-- prettier-ignore -->
 !!! warning
     This method modifies the Conda environment in which you choose to install. Consider instead using [pipx](#pipx) or [condax](https://github.com/mariusvniekerk/condax) to avoid dependency conflicts.
```

### Comparing `itksn-0.1.0/docs/assets/css/custom.css` & `itksn-0.1.1/docs/assets/css/custom.css`

 * *Files identical despite different names*

### Comparing `itksn-0.1.0/docs/assets/images/logo.svg` & `itksn-0.1.1/docs/assets/images/logo.svg`

 * *Files identical despite different names*

### Comparing `itksn-0.1.0/src/itksn/cli/main.py` & `itksn-0.1.1/src/itksn/cli/main.py`

 * *Files identical despite different names*

### Comparing `itksn-0.1.0/tests/test_cli.py` & `itksn-0.1.1/tests/test_cli.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,21 +5,21 @@
 
 import itksn
 
 
 def test_version(script_runner):
     command = "itksn --version"
     start = time.time()
-    ret = script_runner.run(*shlex.split(command))
+    ret = script_runner.run(shlex.split(command))
     end = time.time()
     elapsed = end - start
     assert ret.success
     assert itksn.__version__ in ret.stdout
-    assert ret.stderr == ""
-    # make sure it took less than a second
-    assert elapsed < 1.0
+    assert not ret.stderr
+    # make sure it took less than 1.5s
+    assert elapsed < 1.5
 
 
 def test_parse(script_runner):
     command = "itksn parse 20Uxxyynnnnnnn"
-    ret = script_runner.run(*shlex.split(command))
+    ret = script_runner.run(shlex.split(command))
     assert ret.success
```

### Comparing `itksn-0.1.0/tests/test_core.py` & `itksn-0.1.1/tests/test_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,45 +6,45 @@
 
 import itksn
 from itksn.core import EnumStr
 
 
 def test_enumstr():
     myenum = EnumStr(Bytes(2), itsaa=b"aa", itsbb=b"bb", itsyy=b"yy")
-    assert myenum.parse(b"yy").intvalue == b"yy"
+    assert myenum.parse(b"yy").bytevalue == b"yy"
     assert myenum.parse(b"yy") == "itsyy"
-    assert myenum.parse(b"xx").intvalue == b"xx"
-    assert myenum.parse(b"xx") == ""
+    assert myenum.parse(b"xx").bytevalue == b"xx"
+    assert not myenum.parse(b"xx")
 
 
 def test_parse_example1():
     parsed = itksn.parse(b"20Uxxyynnnnnnn")
     assert parsed.atlas_project == "atlas_detector"
     assert parsed.system_code == "phaseII_upgrade"
-    assert parsed.project_code == ""
-    assert parsed.subproject_code == ""
+    assert not parsed.project_code
+    assert parsed.subproject_code == "yy"
     assert parsed.identifier == b"nnnnnnn"
 
 
 def test_parse_example2():
     parsed = itksn.parse(b"20UPIyynnnnnnn")
     assert parsed.atlas_project == "atlas_detector"
     assert parsed.system_code == "phaseII_upgrade"
     assert parsed.project_code == "inner_pixel"
-    assert parsed.subproject_code == ""
+    assert not parsed.subproject_code
     assert parsed.identifier == b"nnnnnnn"
 
 
 def test_parse_fe_wafer():
     parsed = itksn.parse(b"20UPGFW2123456")
     assert parsed.atlas_project == "atlas_detector"
     assert parsed.system_code == "phaseII_upgrade"
     assert parsed.project_code == "pixel_general"
     assert parsed.subproject_code == "FE_chip_wafer"
-    assert parsed.identifier.batch_number == "CROC"
+    assert parsed.identifier.batch_number == "ITkpix_v2"
     assert parsed.identifier.number == b"123456"
 
 
 def test_parse_sensor():
     parsed = itksn.parse(b"20UPGW34212345")
     assert parsed.atlas_project == "atlas_detector"
     assert parsed.system_code == "phaseII_upgrade"
```

### Comparing `itksn-0.1.0/.gitignore` & `itksn-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `itksn-0.1.0/LICENSE` & `itksn-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `itksn-0.1.0/README.md` & `itksn-0.1.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# itksn v0.1.0
+# itksn v0.1.1
 
 Helper utility for parsing ITk Serial Numbers
 
 ---
 
 <!-- sync the following div with docs/index.md -->
 <div align="center">
```

### Comparing `itksn-0.1.0/pyproject.toml` & `itksn-0.1.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -4,35 +4,34 @@
 [project]
 name = "itksn"
 authors = [
   { name = "Giordon Stark", email = "kratsg@gmail.com" },
 ]
 description = "ITk Serial Number parser"
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 classifiers = [
   "Development Status :: 1 - Planning",
   "Intended Audience :: Science/Research",
   "Intended Audience :: Developers",
   "License :: OSI Approved :: BSD License",
   "Operating System :: OS Independent",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3 :: Only",
-  "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Topic :: Scientific/Engineering",
   "Typing :: Typed",
 ]
 dynamic = ["version"]
 dependencies = [
-  "typing_extensions >=3.7; python_version<'3.8'",
+  "typing_extensions >=3.8; python_version<'3.11'",
   "typer",
   "construct>=2.10"
 ]
 
 [project.optional-dependencies]
 test = [
   "pytest >=6",
@@ -98,15 +97,15 @@
     "pytest-mock>=3.0",
 ]
 
 [tool.hatch.envs.dev.scripts]
 test = "pytest -ra"
 
 [[tool.hatch.envs.dev.matrix]]
-python = ["3.7", "3.8", "3.9", "3.10", "3.11", "pypy3.8"]
+python = ["3.8", "3.9", "3.10", "3.11", "pypy3.8"]
 
 [tool.hatch.envs.docs]
 template = "docs"
 dependencies = [
     "mkdocs>=1.4.0",
     "mkdocs-material>=8.5.6",
     # Plugins
@@ -156,36 +155,28 @@
 testpaths = [
   "tests",
 ]
 
 
 [tool.mypy]
 files = "src"
-python_version = "3.7"
+python_version = "3.8"
 warn_unused_configs = true
 strict = true
 show_error_codes = true
 enable_error_code = ["ignore-without-code", "redundant-expr", "truthy-bool"]
 warn_unreachable = true
 
-[[tool.mypy.overrides]]
-module = 'construct'
-ignore_missing_imports = true
-
-[[tool.mypy.overrides]]
-module = ['itksn.core']
-ignore_errors = true
-
 [tool.ruff]
 select = [
   "E", "F", "W", # flake8
   "B",  "B904",  # flake8-bugbear
   "I",           # isort
   "ARG",         # flake8-unused-arguments
-  "C4",          # flake8-comprehensions
+  "C40",         # flake8-comprehensions
   "EM",          # flake8-errmsg
   "ICN",         # flake8-import-conventions
   "ISC",         # flake8-implicit-str-concat
   "PGH",         # pygrep-hooks
   "PIE",         # flake8-pie
   "PL",          # pylint
   "PT",          # flake8-pytest-style
@@ -195,27 +186,27 @@
   "SIM",         # flake8-simplify
   "T20",         # flake8-print
   "UP",          # pyupgrade
   "YTT",         # flake8-2020
 ]
 extend-ignore = ["PLR", "E501"]
 target-version = "py37"
-typing-modules = ["itksn._compat.typing"]
+typing-modules = ["itksn.typing"]
 src = ["src"]
 unfixable = ["T20", "F841"]
 exclude = []
 isort.required-imports = ["from __future__ import annotations"]
 
 [tool.ruff.per-file-ignores]
 "tests/**" = ["T20"]
 "src/itksn/cli/main.py" = ["B008"]
 
 
 [tool.pylint]
-py-version = "3.7"
+py-version = "3.8"
 ignore-paths= ["src/itksn/_version.py"]
 reports.output-format = "colorized"
 similarities.ignore-imports = "yes"
 messages_control.disable = [
   "design",
   "fixme",
   "line-too-long",
```

### Comparing `itksn-0.1.0/PKG-INFO` & `itksn-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: itksn
-Version: 0.1.0
+Version: 0.1.1
 Summary: ITk Serial Number parser
 Project-URL: Homepage, https://github.com/kratsg/itksn
 Project-URL: Documentation, https://kratsg.github.io/itksn/0.1/
 Project-URL: Tracker, https://github.com/kratsg/itksn/issues
 Project-URL: Discussions, https://github.com/kratsg/itksn/discussions
 Project-URL: Changelog, https://github.com/kratsg/itksn/releases
 Author-email: Giordon Stark <kratsg@gmail.com>
@@ -13,39 +13,38 @@
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Typing :: Typed
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Requires-Dist: construct>=2.10
 Requires-Dist: typer
-Requires-Dist: typing-extensions>=3.7; python_version < '3.8'
+Requires-Dist: typing-extensions>=3.8; python_version < '3.11'
 Provides-Extra: dev
 Requires-Dist: pytest-cov>=3; extra == 'dev'
 Requires-Dist: pytest>=6; extra == 'dev'
 Provides-Extra: docs
 Requires-Dist: myst-parser>=0.13; extra == 'docs'
 Requires-Dist: sphinx-book-theme>=0.1.0; extra == 'docs'
 Requires-Dist: sphinx-copybutton; extra == 'docs'
 Requires-Dist: sphinx>=4.0; extra == 'docs'
 Provides-Extra: test
 Requires-Dist: pytest-cov>=3; extra == 'test'
 Requires-Dist: pytest>=6; extra == 'test'
 Description-Content-Type: text/markdown
 
-# itksn v0.1.0
+# itksn v0.1.1
 
 Helper utility for parsing ITk Serial Numbers
 
 ---
 
 <!-- sync the following div with docs/index.md -->
 <div align="center">
```

