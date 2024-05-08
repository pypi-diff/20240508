# Comparing `tmp/mkdocs-ansible-24.3.0.tar.gz` & `tmp/mkdocs_ansible-24.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-ansible-24.3.0.tar", last modified: Tue Mar 26 11:22:32 2024, max compression
+gzip compressed data, was "mkdocs_ansible-24.3.1.tar", last modified: Wed May  8 11:05:22 2024, max compression
```

## Comparing `mkdocs-ansible-24.3.0.tar` & `mkdocs_ansible-24.3.1.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:22:32.046122 mkdocs-ansible-24.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:22:32.042122 mkdocs-ansible-24.3.0/.config/
--rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-03-26 11:22:20.000000 mkdocs-ansible-24.3.0/.config/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-03-26 11:22:20.000000 mkdocs-ansible-24.3.0/.config/dictionary.txt
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-03-26 11:22:20.000000 mkdocs-ansible-24.3.0/.config/requirements.in
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:22:32.042122 mkdocs-ansible-24.3.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-03-26 11:22:20.000000 mkdocs-ansible-24.3.0/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-03-26 11:22:20.000000 mkdocs-ansible-24.3.0/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-03-26 11:22:20.000000 mkdocs-ansible-24.3.0/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:22:32.042122 mkdocs-ansible-24.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-03-26 11:22:20.000000 mkdocs-ansible-24.3.0/.github/workflows/ack.yml
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-03-26 11:22:20.000000 mkdocs-ansible-24.3.0/.github/workflows/push.yml
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-03-26 11:22:20.000000 mkdocs-ansible-24.3.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4736 2024-03-26 11:22:20.000000 mkdocs-ansible-24.3.0/.github/workflows/tox.yml
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-03-26 11:22:20.000000 mkdocs-ansible-24.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     3854 2024-03-26 11:22:20.000000 mkdocs-ansible-24.3.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-03-26 11:22:20.000000 mkdocs-ansible-24.3.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-03-26 11:22:20.000000 mkdocs-ansible-24.3.0/.yamllint
--rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-03-26 11:22:32.046122 mkdocs-ansible-24.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-03-26 11:22:20.000000 mkdocs-ansible-24.3.0/cspell.config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:22:32.042122 mkdocs-ansible-24.3.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-03-26 11:22:20.000000 mkdocs-ansible-24.3.0/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-03-26 11:22:20.000000 mkdocs-ansible-24.3.0/docs/macros.md
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-03-26 11:22:20.000000 mkdocs-ansible-24.3.0/linkcheckerrc
--rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-03-26 11:22:20.000000 mkdocs-ansible-24.3.0/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-03-26 11:22:20.000000 mkdocs-ansible-24.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-26 11:22:32.046122 mkdocs-ansible-24.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:22:32.038122 mkdocs-ansible-24.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:22:32.042122 mkdocs-ansible-24.3.0/src/mkdocs_ansible/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:22:32.042122 mkdocs-ansible-24.3.0/src/mkdocs_ansible/.icons/
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-03-26 11:22:20.000000 mkdocs-ansible-24.3.0/src/mkdocs_ansible/.icons/logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-03-26 11:22:20.000000 mkdocs-ansible-24.3.0/src/mkdocs_ansible/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-03-26 11:22:31.000000 mkdocs-ansible-24.3.0/src/mkdocs_ansible/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:22:32.038122 mkdocs-ansible-24.3.0/src/mkdocs_ansible/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:22:32.046122 mkdocs-ansible-24.3.0/src/mkdocs_ansible/assets/images/
--rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-03-26 11:22:20.000000 mkdocs-ansible-24.3.0/src/mkdocs_ansible/assets/images/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)    28235 2024-03-26 11:22:20.000000 mkdocs-ansible-24.3.0/src/mkdocs_ansible/assets/images/logo.png
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-03-26 11:22:20.000000 mkdocs-ansible-24.3.0/src/mkdocs_ansible/assets/images/logo.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:22:32.046122 mkdocs-ansible-24.3.0/src/mkdocs_ansible/assets/stylesheets/
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-03-26 11:22:20.000000 mkdocs-ansible-24.3.0/src/mkdocs_ansible/assets/stylesheets/ansible.css
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-03-26 11:22:20.000000 mkdocs-ansible-24.3.0/src/mkdocs_ansible/main.html
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-03-26 11:22:20.000000 mkdocs-ansible-24.3.0/src/mkdocs_ansible/mkdocs_theme.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:22:32.046122 mkdocs-ansible-24.3.0/src/mkdocs_ansible.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-03-26 11:22:32.000000 mkdocs-ansible-24.3.0/src/mkdocs_ansible.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-03-26 11:22:32.000000 mkdocs-ansible-24.3.0/src/mkdocs_ansible.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 11:22:32.000000 mkdocs-ansible-24.3.0/src/mkdocs_ansible.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-03-26 11:22:32.000000 mkdocs-ansible-24.3.0/src/mkdocs_ansible.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-03-26 11:22:32.000000 mkdocs-ansible-24.3.0/src/mkdocs_ansible.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-26 11:22:32.000000 mkdocs-ansible-24.3.0/src/mkdocs_ansible.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3346 2024-03-26 11:22:20.000000 mkdocs-ansible-24.3.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:05:22.735360 mkdocs_ansible-24.3.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:05:22.731360 mkdocs_ansible-24.3.1/.config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-05-08 11:05:12.000000 mkdocs_ansible-24.3.1/.config/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-05-08 11:05:12.000000 mkdocs_ansible-24.3.1/.config/dictionary.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-08 11:05:12.000000 mkdocs_ansible-24.3.1/.config/requirements.in
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:05:22.731360 mkdocs_ansible-24.3.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-08 11:05:12.000000 mkdocs_ansible-24.3.1/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-08 11:05:12.000000 mkdocs_ansible-24.3.1/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-08 11:05:12.000000 mkdocs_ansible-24.3.1/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:05:22.731360 mkdocs_ansible-24.3.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-08 11:05:12.000000 mkdocs_ansible-24.3.1/.github/workflows/ack.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-08 11:05:12.000000 mkdocs_ansible-24.3.1/.github/workflows/push.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-08 11:05:12.000000 mkdocs_ansible-24.3.1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     6025 2024-05-08 11:05:12.000000 mkdocs_ansible-24.3.1/.github/workflows/tox.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-08 11:05:12.000000 mkdocs_ansible-24.3.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-05-08 11:05:12.000000 mkdocs_ansible-24.3.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-08 11:05:12.000000 mkdocs_ansible-24.3.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-08 11:05:12.000000 mkdocs_ansible-24.3.1/.yamllint
+-rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-05-08 11:05:22.735360 mkdocs_ansible-24.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-08 11:05:12.000000 mkdocs_ansible-24.3.1/cspell.config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:05:22.731360 mkdocs_ansible-24.3.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-08 11:05:12.000000 mkdocs_ansible-24.3.1/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-08 11:05:12.000000 mkdocs_ansible-24.3.1/docs/macros.md
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-08 11:05:12.000000 mkdocs_ansible-24.3.1/linkcheckerrc
+-rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-05-08 11:05:12.000000 mkdocs_ansible-24.3.1/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-05-08 11:05:12.000000 mkdocs_ansible-24.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 11:05:22.735360 mkdocs_ansible-24.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:05:22.727359 mkdocs_ansible-24.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:05:22.731360 mkdocs_ansible-24.3.1/src/mkdocs_ansible/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:05:22.735360 mkdocs_ansible-24.3.1/src/mkdocs_ansible/.icons/
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-05-08 11:05:12.000000 mkdocs_ansible-24.3.1/src/mkdocs_ansible/.icons/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-05-08 11:05:12.000000 mkdocs_ansible-24.3.1/src/mkdocs_ansible/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-08 11:05:22.000000 mkdocs_ansible-24.3.1/src/mkdocs_ansible/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:05:22.727359 mkdocs_ansible-24.3.1/src/mkdocs_ansible/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:05:22.735360 mkdocs_ansible-24.3.1/src/mkdocs_ansible/assets/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-05-08 11:05:12.000000 mkdocs_ansible-24.3.1/src/mkdocs_ansible/assets/images/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)    28235 2024-05-08 11:05:12.000000 mkdocs_ansible-24.3.1/src/mkdocs_ansible/assets/images/logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-05-08 11:05:12.000000 mkdocs_ansible-24.3.1/src/mkdocs_ansible/assets/images/logo.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:05:22.735360 mkdocs_ansible-24.3.1/src/mkdocs_ansible/assets/stylesheets/
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-08 11:05:12.000000 mkdocs_ansible-24.3.1/src/mkdocs_ansible/assets/stylesheets/ansible.css
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-08 11:05:12.000000 mkdocs_ansible-24.3.1/src/mkdocs_ansible/main.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-05-08 11:05:12.000000 mkdocs_ansible-24.3.1/src/mkdocs_ansible/mkdocs_theme.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:05:22.735360 mkdocs_ansible-24.3.1/src/mkdocs_ansible.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-05-08 11:05:22.000000 mkdocs_ansible-24.3.1/src/mkdocs_ansible.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-05-08 11:05:22.000000 mkdocs_ansible-24.3.1/src/mkdocs_ansible.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 11:05:22.000000 mkdocs_ansible-24.3.1/src/mkdocs_ansible.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-08 11:05:22.000000 mkdocs_ansible-24.3.1/src/mkdocs_ansible.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-08 11:05:22.000000 mkdocs_ansible-24.3.1/src/mkdocs_ansible.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-08 11:05:22.000000 mkdocs_ansible-24.3.1/src/mkdocs_ansible.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3346 2024-05-08 11:05:12.000000 mkdocs_ansible-24.3.1/tox.ini
```

### Comparing `mkdocs-ansible-24.3.0/.config/constraints.txt` & `mkdocs_ansible-24.3.1/.config/constraints.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,65 +1,67 @@
 #
 # This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
 #    pip-compile --no-annotate --output-file=.config/constraints.txt --strip-extras --unsafe-package=ruamel-yaml-clib pyproject.toml
 #
-babel==2.14.0
+babel==2.15.0
 beautifulsoup4==4.12.3
-cairocffi==1.6.1
+cairocffi==1.7.0
 cairosvg==2.7.1
 certifi==2024.2.2
 cffi==1.16.0
 charset-normalizer==3.3.2
 click==8.1.7
 colorama==0.4.6
 csscompressor==0.9.5
 cssselect2==0.7.0
 defusedxml==0.7.1
 dnspython==2.6.1
 ghp-import==2.1.0
-griffe==0.41.3
+griffe==0.44.0
 htmlmin2==0.1.13
-idna==3.6
+idna==3.7
 jinja2==3.1.3
 jsmin==3.0.1
 linkchecker==10.4.0
-markdown==3.5.2
-markdown-exec==1.8.0
+markdown==3.6
+markdown-exec==1.8.1
 markdown-include==0.8.1
 markupsafe==2.1.5
 mergedeep==1.3.4
-mkdocs==1.5.3
+mkdocs==1.6.0
 mkdocs-autorefs==1.0.1
 mkdocs-gen-files==0.5.0
-mkdocs-htmlproofer-plugin==1.2.0
+mkdocs-get-deps==0.2.0
+mkdocs-htmlproofer-plugin==1.2.1
 mkdocs-macros-plugin==1.0.5
-mkdocs-material==9.5.13
+mkdocs-material==9.5.21
 mkdocs-material-extensions==1.3.1
 mkdocs-minify-plugin==0.8.0
 mkdocs-monorepo-plugin==1.1.0
-mkdocstrings==0.24.1
-mkdocstrings-python==1.8.0
+mkdocstrings==0.25.1
+mkdocstrings-python==1.10.0
 packaging==24.0
 paginate==0.5.6
 pathspec==0.12.1
-pillow==10.2.0
-pipdeptree==2.16.1
-platformdirs==4.2.0
-pycparser==2.21
-pygments==2.17.2
-pymdown-extensions==10.7.1
+pillow==10.3.0
+pip==24.0
+pipdeptree==2.19.1
+platformdirs==4.2.1
+pycparser==2.22
+pygments==2.18.0
+pymdown-extensions==10.8.1
 python-dateutil==2.9.0.post0
 python-slugify==8.0.4
 pyyaml==6.0.1
 pyyaml-env-tag==0.1
-regex==2023.12.25
+regex==2024.4.28
 requests==2.31.0
 six==1.16.0
 soupsieve==2.5
 termcolor==2.4.0
 text-unidecode==1.3
-tinycss2==1.2.1
+tinycss2==1.3.0
 urllib3==2.2.1
 watchdog==4.0.0
 webencodings==0.5.1
```

### Comparing `mkdocs-ansible-24.3.0/.github/workflows/release.yml` & `mkdocs_ansible-24.3.1/.github/workflows/release.yml`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
       - name: Check out src from Git
         uses: actions/checkout@v4
         with:
           fetch-depth: 0 # needed by setuptools-scm
           submodules: true
 
       - name: Build dists
-        run: python -m tox
+        run: python3 -m tox
 
       - name: Publish to pypi.org
         if: >- # "create" workflows run separately from "push" & "pull_request"
           github.event_name == 'release'
         uses: pypa/gh-action-pypi-publish@release/v1
         with:
           password: ${{ secrets.pypi_password }}
```

### Comparing `mkdocs-ansible-24.3.0/.github/workflows/tox.yml` & `mkdocs_ansible-24.3.1/.github/workflows/tox.yml`

 * *Files 19% similar despite different names*

```diff
@@ -121,21 +121,59 @@
             # shellcheck disable=SC2016
             echo -n '::error file=git-status::'
             printf '### Failed as git reported modified and/or untracked files\n```\n%s\n```\n' "$(git status -s)" | tee -a "$GITHUB_STEP_SUMMARY"
             exit 99
           fi
         # https://github.com/actions/toolkit/issues/193
 
+  codeql:
+    name: codeql
+    runs-on: ubuntu-latest
+    permissions:
+      actions: read
+      contents: read
+      security-events: write
+
+    strategy:
+      fail-fast: false
+      matrix:
+        language: ["python"]
+
+    steps:
+      - name: Checkout repository
+        uses: actions/checkout@v4
+
+      # Initializes the CodeQL tools for scanning.
+      - name: Initialize CodeQL
+        uses: github/codeql-action/init@v3
+        with:
+          languages: ${{ matrix.language }}
+          # If you wish to specify custom queries, you can do so here or in a config file.
+          # By default, queries listed here will override any specified in a config file.
+          # Prefix the list here with "+" to use these queries and those in the config file.
+
+          # Details on CodeQL's query packs refer to : https://docs.github.com/en/code-security/code-scanning/automatically-scanning-your-code-for-vulnerabilities-and-errors/configuring-code-scanning#using-queries-in-ql-packs
+          # queries: security-extended,security-and-quality
+
+      - name: Autobuild
+        uses: github/codeql-action/autobuild@v3
+
+      - name: Perform CodeQL Analysis
+        uses: github/codeql-action/analyze@v3
+        with:
+          category: "/language:${{matrix.language}}"
+
   check: # This job does nothing and is only used for the branch protection
     if: always()
     permissions:
       pull-requests: write # allow codenotify to comment on pull-request
 
     needs:
       - build
+      - codeql
 
     runs-on: ubuntu-latest
 
     steps:
       - name: Decide whether the needed jobs succeeded or failed
         uses: re-actors/alls-green@release/v1
         with:
```

### Comparing `mkdocs-ansible-24.3.0/.pre-commit-config.yaml` & `mkdocs_ansible-24.3.1/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -22,26 +22,26 @@
       - id: prettier
         always_run: true
         additional_dependencies:
           - prettier
           - prettier-plugin-toml
           - prettier-plugin-sort-json
   - repo: https://github.com/streetsidesoftware/cspell-cli
-    rev: v8.6.0
+    rev: v8.8.0
     hooks:
       - id: cspell
         # entry: codespell --relative
         args: [--relative, --no-progress, --no-summary]
         name: Spell check with cspell
   - repo: https://github.com/python-jsonschema/check-jsonschema
-    rev: 0.28.0
+    rev: 0.28.2
     hooks:
       - id: check-github-workflows
   - repo: https://github.com/pre-commit/pre-commit-hooks.git
-    rev: v4.5.0
+    rev: v4.6.0
     hooks:
       - id: end-of-file-fixer
       - id: trailing-whitespace
       - id: mixed-line-ending
       - id: fix-byte-order-marker
       - id: check-executables-have-shebangs
       - id: check-merge-conflict
@@ -68,26 +68,26 @@
     rev: 5.13.2
     hooks:
       - id: isort
         args:
           # https://github.com/pre-commit/mirrors-isort/issues/9#issuecomment-624404082
           - --filter-files
   - repo: https://github.com/psf/black
-    rev: 24.3.0
+    rev: 24.4.2
     hooks:
       - id: black
         language_version: python3
   - repo: https://github.com/asottile/pyupgrade
     # keep it after flake8
     rev: v3.15.2
     hooks:
       - id: pyupgrade
         args: ["--py39-plus"]
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v1.9.0
+    rev: v1.10.0
     hooks:
       - id: mypy
         # empty args needed in order to match mypy cli behavior
         args: []
         additional_dependencies: ["mkdocs-macros-plugin"]
   - repo: https://github.com/pycqa/pylint
     rev: v3.1.0
```

### Comparing `mkdocs-ansible-24.3.0/PKG-INFO` & `mkdocs_ansible-24.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-ansible
-Version: 24.3.0
+Version: 24.3.1
 Summary: Ansible MkDocs Theme based on mkdocs-material
 Author-email: Ansible by Red Hat <info@ansible.com>
 Maintainer-email: Ansible by Red Hat <info@ansible.com>
 License: MIT
 Project-URL: homepage, https://github.com/ansible/mkdocs-ansible
 Project-URL: documentation, https://ansible.readthedocs.io/projects/mkdocs-ansible/
 Project-URL: repository, https://github.com/ansible/mkdocs-ansible
```

### Comparing `mkdocs-ansible-24.3.0/docs/README.md` & `mkdocs_ansible-24.3.1/docs/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs-ansible-24.3.0/docs/macros.md` & `mkdocs_ansible-24.3.1/docs/macros.md`

 * *Files identical despite different names*

### Comparing `mkdocs-ansible-24.3.0/mkdocs.yml` & `mkdocs_ansible-24.3.1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `mkdocs-ansible-24.3.0/pyproject.toml` & `mkdocs_ansible-24.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mkdocs-ansible-24.3.0/src/mkdocs_ansible/.icons/logo.svg` & `mkdocs_ansible-24.3.1/src/mkdocs_ansible/.icons/logo.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-ansible-24.3.0/src/mkdocs_ansible/__init__.py` & `mkdocs_ansible-24.3.1/src/mkdocs_ansible/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,17 +17,17 @@
 
 def install_from_adt(name: str) -> str:
     """install_from_adt macro."""
     result = f"""!!! Recommendation
 
     The **recommended** approach to install `{name}` is using the
     `ansible-dev-tools` package.
-    [Ansible Development Tools (ADT)](https://ansible.readthedocs.io/projects/dev-tools/)
+    [Ansible Development Tools](https://ansible.readthedocs.io/projects/dev-tools/)
     aims to streamline the setup and usage of several tools needed in order to
-    create [Ansible](https://www.ansible.com) content. ADT combines critical Ansible
+    create [Ansible](https://www.ansible.com) content. It combines critical Ansible
     development packages into a unified Python package.
 
     ```bash
     # This also installs ansible-core if it is not already installed
     pip3 install ansible-dev-tools
     ```
     """
```

### Comparing `mkdocs-ansible-24.3.0/src/mkdocs_ansible/assets/images/favicon.ico` & `mkdocs_ansible-24.3.1/src/mkdocs_ansible/assets/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `mkdocs-ansible-24.3.0/src/mkdocs_ansible/assets/images/logo.png` & `mkdocs_ansible-24.3.1/src/mkdocs_ansible/assets/images/logo.png`

 * *Files identical despite different names*

### Comparing `mkdocs-ansible-24.3.0/src/mkdocs_ansible/assets/images/logo.svg` & `mkdocs_ansible-24.3.1/src/mkdocs_ansible/assets/images/logo.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-ansible-24.3.0/src/mkdocs_ansible/mkdocs_theme.yml` & `mkdocs_ansible-24.3.1/src/mkdocs_ansible/mkdocs_theme.yml`

 * *Files identical despite different names*

### Comparing `mkdocs-ansible-24.3.0/src/mkdocs_ansible.egg-info/PKG-INFO` & `mkdocs_ansible-24.3.1/src/mkdocs_ansible.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-ansible
-Version: 24.3.0
+Version: 24.3.1
 Summary: Ansible MkDocs Theme based on mkdocs-material
 Author-email: Ansible by Red Hat <info@ansible.com>
 Maintainer-email: Ansible by Red Hat <info@ansible.com>
 License: MIT
 Project-URL: homepage, https://github.com/ansible/mkdocs-ansible
 Project-URL: documentation, https://ansible.readthedocs.io/projects/mkdocs-ansible/
 Project-URL: repository, https://github.com/ansible/mkdocs-ansible
```

### Comparing `mkdocs-ansible-24.3.0/src/mkdocs_ansible.egg-info/SOURCES.txt` & `mkdocs_ansible-24.3.1/src/mkdocs_ansible.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mkdocs-ansible-24.3.0/tox.ini` & `mkdocs_ansible-24.3.1/tox.ini`

 * *Files identical despite different names*

