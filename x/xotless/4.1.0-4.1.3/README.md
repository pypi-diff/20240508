# Comparing `tmp/xotless-4.1.0.tar.gz` & `tmp/xotless-4.1.3.tar.gz`

## Comparing `xotless-4.1.0.tar` & `xotless-4.1.3.tar`

### file list

```diff
@@ -1,53 +1,55 @@
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 xotless-4.1.0/.dir-locals.el
--rw-r--r--   0        0        0     5159 2020-02-02 00:00:00.000000 xotless-4.1.0/.gitlab-ci.yml
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 xotless-4.1.0/HISTORY.rst -> docs/source/history.rst
--rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 xotless-4.1.0/Makefile
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 xotless-4.1.0/conftest.py
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 xotless-4.1.0/mypy.ini
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 xotless-4.1.0/pytest.ini
--rw-r--r--   0        0        0     2360 2020-02-02 00:00:00.000000 xotless-4.1.0/requirements-dev-py312.lock
--rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 xotless-4.1.0/tox.ini
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 xotless-4.1.0/ci/cleanup.yml
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 xotless-4.1.0/docs/Makefile
--rw-r--r--   0        0        0     3371 2020-02-02 00:00:00.000000 xotless-4.1.0/docs/source/conf.py
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 xotless-4.1.0/docs/source/context.rst
--rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 xotless-4.1.0/docs/source/domains.rst
--rw-r--r--   0        0        0     6129 2020-02-02 00:00:00.000000 xotless-4.1.0/docs/source/history.rst
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 xotless-4.1.0/docs/source/immutables.rst
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 xotless-4.1.0/docs/source/index.rst
--rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 xotless-4.1.0/docs/source/itertools.rst
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 xotless-4.1.0/docs/source/pickablenv.rst
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 xotless-4.1.0/docs/source/ranges.rst
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 xotless-4.1.0/docs/source/testing.rst
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 xotless-4.1.0/docs/source/tracing.rst
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 xotless-4.1.0/docs/source/trees.rst
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 xotless-4.1.0/docs/source/walk.rst
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 xotless-4.1.0/docs/source/_static/custom.css
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 xotless-4.1.0/src/tests/__init__.py
--rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 xotless-4.1.0/src/tests/support.py
--rw-r--r--   0        0        0    26105 2020-02-02 00:00:00.000000 xotless-4.1.0/src/tests/test_domains.py
--rw-r--r--   0        0        0     2813 2020-02-02 00:00:00.000000 xotless-4.1.0/src/tests/test_immutables.py
--rw-r--r--   0        0        0     5704 2020-02-02 00:00:00.000000 xotless-4.1.0/src/tests/test_interval_tree.py
--rw-r--r--   0        0        0     7584 2020-02-02 00:00:00.000000 xotless-4.1.0/src/tests/test_lines.py
--rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 xotless-4.1.0/src/tests/test_walk.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 xotless-4.1.0/src/xotless/_version.py
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 xotless-4.1.0/src/xotless/context.py
--rw-r--r--   0        0        0    15897 2020-02-02 00:00:00.000000 xotless-4.1.0/src/xotless/domains.py
--rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 xotless-4.1.0/src/xotless/enums.py
--rw-r--r--   0        0        0    11774 2020-02-02 00:00:00.000000 xotless-4.1.0/src/xotless/immutables.py
--rw-r--r--   0        0        0    11569 2020-02-02 00:00:00.000000 xotless-4.1.0/src/xotless/itertools.py
--rw-r--r--   0        0        0     6159 2020-02-02 00:00:00.000000 xotless-4.1.0/src/xotless/pickablenv.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xotless-4.1.0/src/xotless/py.typed
--rw-r--r--   0        0        0    18128 2020-02-02 00:00:00.000000 xotless-4.1.0/src/xotless/ranges.py
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 xotless-4.1.0/src/xotless/release.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xotless-4.1.0/src/xotless/release.pyi
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 xotless-4.1.0/src/xotless/tracing.py
--rw-r--r--   0        0        0     8729 2020-02-02 00:00:00.000000 xotless-4.1.0/src/xotless/trees.py
--rw-r--r--   0        0        0     3769 2020-02-02 00:00:00.000000 xotless-4.1.0/src/xotless/types.py
--rw-r--r--   0        0        0     3299 2020-02-02 00:00:00.000000 xotless-4.1.0/src/xotless/walk.py
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 xotless-4.1.0/src/xotless/testing/strategies/__init__.py
--rw-r--r--   0        0        0    14098 2020-02-02 00:00:00.000000 xotless-4.1.0/src/xotless/testing/strategies/domains.py
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 xotless-4.1.0/.gitignore
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 xotless-4.1.0/README.rst
--rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 xotless-4.1.0/pyproject.toml
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 xotless-4.1.0/PKG-INFO
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 xotless-4.1.3/.dir-locals.el
+-rw-r--r--   0        0        0     5141 2020-02-02 00:00:00.000000 xotless-4.1.3/.gitlab-ci.yml
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 xotless-4.1.3/HISTORY.rst -> docs/source/history.rst
+-rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 xotless-4.1.3/Makefile
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 xotless-4.1.3/conftest.py
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 xotless-4.1.3/mypy.ini
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 xotless-4.1.3/pytest.ini
+-rw-r--r--   0        0        0     2447 2020-02-02 00:00:00.000000 xotless-4.1.3/requirements-dev-py312.lock
+-rw-r--r--   0        0        0     2757 2020-02-02 00:00:00.000000 xotless-4.1.3/requirements-dev-py38.lock
+-rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 xotless-4.1.3/tox.ini
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 xotless-4.1.3/docs/Makefile
+-rw-r--r--   0        0        0     3371 2020-02-02 00:00:00.000000 xotless-4.1.3/docs/source/conf.py
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 xotless-4.1.3/docs/source/context.rst
+-rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 xotless-4.1.3/docs/source/domains.rst
+-rw-r--r--   0        0        0     6310 2020-02-02 00:00:00.000000 xotless-4.1.3/docs/source/history.rst
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 xotless-4.1.3/docs/source/immutables.rst
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 xotless-4.1.3/docs/source/index.rst
+-rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 xotless-4.1.3/docs/source/itertools.rst
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 xotless-4.1.3/docs/source/pickablenv.rst
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 xotless-4.1.3/docs/source/ranges.rst
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 xotless-4.1.3/docs/source/testing.rst
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 xotless-4.1.3/docs/source/tracing.rst
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 xotless-4.1.3/docs/source/trees.rst
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 xotless-4.1.3/docs/source/types.rst
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 xotless-4.1.3/docs/source/walk.rst
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 xotless-4.1.3/docs/source/_static/custom.css
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 xotless-4.1.3/src/tests/__init__.py
+-rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 xotless-4.1.3/src/tests/support.py
+-rw-r--r--   0        0        0    26105 2020-02-02 00:00:00.000000 xotless-4.1.3/src/tests/test_domains.py
+-rw-r--r--   0        0        0     2813 2020-02-02 00:00:00.000000 xotless-4.1.3/src/tests/test_immutables.py
+-rw-r--r--   0        0        0     5704 2020-02-02 00:00:00.000000 xotless-4.1.3/src/tests/test_interval_tree.py
+-rw-r--r--   0        0        0     7584 2020-02-02 00:00:00.000000 xotless-4.1.3/src/tests/test_lines.py
+-rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 xotless-4.1.3/src/tests/test_walk.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 xotless-4.1.3/src/xotless/_version.py
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 xotless-4.1.3/src/xotless/context.py
+-rw-r--r--   0        0        0    15897 2020-02-02 00:00:00.000000 xotless-4.1.3/src/xotless/domains.py
+-rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 xotless-4.1.3/src/xotless/enums.py
+-rw-r--r--   0        0        0    11774 2020-02-02 00:00:00.000000 xotless-4.1.3/src/xotless/immutables.py
+-rw-r--r--   0        0        0    11569 2020-02-02 00:00:00.000000 xotless-4.1.3/src/xotless/itertools.py
+-rw-r--r--   0        0        0     6159 2020-02-02 00:00:00.000000 xotless-4.1.3/src/xotless/pickablenv.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xotless-4.1.3/src/xotless/py.typed
+-rw-r--r--   0        0        0    18128 2020-02-02 00:00:00.000000 xotless-4.1.3/src/xotless/ranges.py
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 xotless-4.1.3/src/xotless/release.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xotless-4.1.3/src/xotless/release.pyi
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 xotless-4.1.3/src/xotless/tracing.py
+-rw-r--r--   0        0        0     8729 2020-02-02 00:00:00.000000 xotless-4.1.3/src/xotless/trees.py
+-rw-r--r--   0        0        0     3982 2020-02-02 00:00:00.000000 xotless-4.1.3/src/xotless/types.py
+-rw-r--r--   0        0        0     2260 2020-02-02 00:00:00.000000 xotless-4.1.3/src/xotless/types.pyi
+-rw-r--r--   0        0        0     3299 2020-02-02 00:00:00.000000 xotless-4.1.3/src/xotless/walk.py
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 xotless-4.1.3/src/xotless/testing/strategies/__init__.py
+-rw-r--r--   0        0        0    14098 2020-02-02 00:00:00.000000 xotless-4.1.3/src/xotless/testing/strategies/domains.py
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 xotless-4.1.3/.gitignore
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 xotless-4.1.3/README.rst
+-rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 xotless-4.1.3/pyproject.toml
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 xotless-4.1.3/PKG-INFO
```

### Comparing `xotless-4.1.0/Makefile` & `xotless-4.1.3/Makefile`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 RYE_EXEC ?= rye run
-PYTHON_VERSION ?= 3.12
+PYTHON_VERSION ?= 3.8
 PATH := $(HOME)/.rye/shims:$(PATH)
 
 SHELL := /bin/bash
 PYTHON_FILES := $(shell find src/ -type f -name '*.py' -o -name '*.pyi')
 
 USE_UV ?= true
 install:
@@ -46,21 +46,29 @@
 .PHONY: test
 
 doctest:
 	@$(RYE_EXEC) tox -e system-doctest
 .PHONY: test
 
 mypy:
-	@$(RYE_EXEC) mypy -p xotless --config mypy.ini
+	@$(RYE_EXEC) tox -e system-staticcheck
 .PHONY: mypy
 
-docs:
-	make SPHINXBUILD="$(RYE_EXEC) sphinx-build" -C docs html
-.PHONY: docs
-
-
-CADDY_SERVER_PORT ?= 9999
-caddy: docs
-	@docker run --rm -p $(CADDY_SERVER_PORT):$(CADDY_SERVER_PORT) \
-         -v $(PWD)/docs/build/html:/var/www -it caddy \
-         caddy file-server --browse --listen :$(CADDY_SERVER_PORT) --root /var/www
-.PHONY: caddy
+pyright:
+	@$(RYE_EXEC) pyright src/xotless
+.PHONY: pyright
+
+
+SPHINXOPTS ?= -W
+docs/build:
+	make SPHINXOPTS=$(SPHINXOPTS) SPHINXBUILD="$(RYE_EXEC) sphinx-build" -C docs html
+.PHONY: docs/build
+
+
+CADDY_IMAGE ?= caddy:2.7-alpine
+CADDY_SERVER_PORT ?= 6942
+docs/browse: docs/build
+	@docker run --rm --network host \
+        -v $(PWD)/docs/build/html/:/var/www \
+        -it $(CADDY_IMAGE) \
+	    caddy file-server --browse --listen :$(CADDY_SERVER_PORT) --root /var/www
+.PHONY: docs/browse
```

### Comparing `xotless-4.1.0/requirements-dev-py312.lock` & `xotless-4.1.3/requirements-dev-py312.lock`

 * *Files 3% similar despite different names*

```diff
@@ -57,14 +57,16 @@
     # via pygls
     # via ruff-lsp
 markupsafe==2.1.5
     # via jinja2
 mypy==1.10.0
 mypy-extensions==1.0.0
     # via mypy
+nodeenv==1.8.0
+    # via pyright
 packaging==23.2
     # via pyproject-api
     # via pytest
     # via ruff-lsp
     # via sphinx
     # via tox
     # via xotl-tools
@@ -78,24 +80,27 @@
 pygls==1.3.0
     # via ruff-lsp
 pygments==2.17.2
     # via furo
     # via sphinx
 pyproject-api==1.6.1
     # via tox
+pyright==1.1.361
 pytest==8.0.1
     # via pytest-cov
     # via pytest-xdist
 pytest-cov==4.1.0
 pytest-xdist==3.5.0
 requests==2.31.0
     # via sphinx
-ruff==0.4.2
+ruff==0.4.3
     # via ruff-lsp
 ruff-lsp==0.0.52
+setuptools==69.5.1
+    # via nodeenv
 snowballstemmer==2.2.0
     # via sphinx
 sortedcontainers==2.4.0
     # via hypothesis
 soupsieve==2.5
     # via beautifulsoup4
 sphinx==7.1.2
```

### Comparing `xotless-4.1.0/tox.ini` & `xotless-4.1.3/tox.ini`

 * *Files 14% similar despite different names*

```diff
@@ -16,15 +16,15 @@
        hypothesis~=6.98.6
        ipdb
        pytest-xdist~=2.1
        coverage[toml]>=7.4.0
        pytest-cov~=2.10
 	   sentry-sdk~=1.5
        doctest: sphinx~=7.1.2
-       staticcheck: mypy==1.8.0
+       staticcheck: mypy==1.10.0
        immutables: immutables
 
 sitepackages = False
 
 allowlist_externals = /usr/bin/make
 
 commands=
```

### Comparing `xotless-4.1.0/docs/Makefile` & `xotless-4.1.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `xotless-4.1.0/docs/source/conf.py` & `xotless-4.1.3/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `xotless-4.1.0/docs/source/domains.rst` & `xotless-4.1.3/docs/source/domains.rst`

 * *Files identical despite different names*

### Comparing `xotless-4.1.0/docs/source/history.rst` & `xotless-4.1.3/docs/source/history.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 =========
  History
 =========
 
 Releases 4.x
 ============
 
+2024-05-08.  Release 4.1.3
+--------------------------
+
+- Make the types of `~xotless.types.EqTypeClass`:class: and
+  `~xotless.types.OrdTypeClass`:class: compatible with pyright.
+
+
 2024-05-05.  Release 4.1.0
 --------------------------
 
 - Make `~xotless.domains.EquivalentSet`:class: type hint be compatible with
   iterables.
```

### Comparing `xotless-4.1.0/docs/source/index.rst` & `xotless-4.1.3/docs/source/index.rst`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 ===================================
 
 .. toctree::
    :maxdepth: 2
    :caption: Contents:
 
    ranges
+   types
    domains
    trees
    itertools
    pickablenv
    immutables
    walk
    context
```

### Comparing `xotless-4.1.0/docs/source/pickablenv.rst` & `xotless-4.1.3/docs/source/pickablenv.rst`

 * *Files identical despite different names*

### Comparing `xotless-4.1.0/docs/source/ranges.rst` & `xotless-4.1.3/docs/source/ranges.rst`

 * *Files identical despite different names*

### Comparing `xotless-4.1.0/docs/source/testing.rst` & `xotless-4.1.3/docs/source/testing.rst`

 * *Files identical despite different names*

### Comparing `xotless-4.1.0/docs/source/trees.rst` & `xotless-4.1.3/docs/source/trees.rst`

 * *Files identical despite different names*

### Comparing `xotless-4.1.0/src/tests/support.py` & `xotless-4.1.3/src/tests/support.py`

 * *Files identical despite different names*

### Comparing `xotless-4.1.0/src/tests/test_domains.py` & `xotless-4.1.3/src/tests/test_domains.py`

 * *Files identical despite different names*

### Comparing `xotless-4.1.0/src/tests/test_immutables.py` & `xotless-4.1.3/src/tests/test_immutables.py`

 * *Files identical despite different names*

### Comparing `xotless-4.1.0/src/tests/test_interval_tree.py` & `xotless-4.1.3/src/tests/test_interval_tree.py`

 * *Files identical despite different names*

### Comparing `xotless-4.1.0/src/tests/test_lines.py` & `xotless-4.1.3/src/tests/test_lines.py`

 * *Files identical despite different names*

### Comparing `xotless-4.1.0/src/tests/test_walk.py` & `xotless-4.1.3/src/tests/test_walk.py`

 * *Files identical despite different names*

### Comparing `xotless-4.1.0/src/xotless/context.py` & `xotless-4.1.3/src/xotless/context.py`

 * *Files identical despite different names*

### Comparing `xotless-4.1.0/src/xotless/domains.py` & `xotless-4.1.3/src/xotless/domains.py`

 * *Files identical despite different names*

### Comparing `xotless-4.1.0/src/xotless/immutables.py` & `xotless-4.1.3/src/xotless/immutables.py`

 * *Files identical despite different names*

### Comparing `xotless-4.1.0/src/xotless/itertools.py` & `xotless-4.1.3/src/xotless/itertools.py`

 * *Files identical despite different names*

### Comparing `xotless-4.1.0/src/xotless/pickablenv.py` & `xotless-4.1.3/src/xotless/pickablenv.py`

 * *Files identical despite different names*

### Comparing `xotless-4.1.0/src/xotless/ranges.py` & `xotless-4.1.3/src/xotless/ranges.py`

 * *Files identical despite different names*

### Comparing `xotless-4.1.0/src/xotless/release.py` & `xotless-4.1.3/src/xotless/release.py`

 * *Files identical despite different names*

### Comparing `xotless-4.1.0/src/xotless/tracing.py` & `xotless-4.1.3/src/xotless/tracing.py`

 * *Files identical despite different names*

### Comparing `xotless-4.1.0/src/xotless/trees.py` & `xotless-4.1.3/src/xotless/trees.py`

 * *Files identical despite different names*

### Comparing `xotless-4.1.0/src/xotless/types.py` & `xotless-4.1.3/src/xotless/types.py`

 * *Files 19% similar despite different names*

```diff
@@ -7,105 +7,108 @@
 # This is free software; you can do what the LICENCE file allows you to.
 #
 # The idea is to support instances registration; then the inspector can be
 # improved to find the right widget for the given instance of a typeclass
 # annotation.
 import typing as t
 
+from typing_extensions import Self
+
 
 class TypeClass(t.Protocol):
     pass
 
 
 # fmt: off
 class EqTypeClass(TypeClass, t.Protocol):  # pragma: no cover
+    """The protocol of the types that can be compared for equality."""
     def __eq__(self, other) -> bool: ...
     def __ne__(self, other) -> bool: ...
 
 
 class OrdTypeClass(EqTypeClass, t.Protocol):  # pragma: no cover
+    """The protocol of the types that have a partial or total order."""
     def __le__(self, other) -> bool: ...
     def __lt__(self, other) -> bool: ...
     def __ge__(self, other) -> bool: ...
     def __gt__(self, other) -> bool: ...
 
 
 # fmt: on
 
 
 T = t.TypeVar("T")
-S = t.TypeVar("S", bound="Domain")
 TEq = t.TypeVar("TEq", bound=EqTypeClass)
 TOrd = t.TypeVar("TOrd", bound=OrdTypeClass)
 
 
 @t.runtime_checkable
 class Domain(t.Protocol[T]):  # pragma: no cover
-    r"""A domain is a generalized type for homogeneous sets.
+    """The protocol for domains: a generalized type for homogeneous sets.
 
     It's not iterable because some sets are not iterable (e.g. the open
     interval ``(0-1)``).  There's also no notion of 'the next element'.
     Domains can also represent infinite sets (which are not representable by
     Python's sets).
 
-    All values of a domain are of the same type `T`.  It's an error to mix
+    All values of a domain are of the same type ``T``.  It's an error to mix
     domains of different types of values (``T``) in the operations below.
 
     """
 
     @property
-    def sample(self: S) -> t.Optional[T]:
+    def sample(self) -> t.Optional[T]:
         """Produces a value which is a member of the domain.
 
         Some non-empty domains cannot produce a sample.  For instance,
         `~xotless.domains.IntervalSet`:class: comprising only open ranges
         cannot produce a sample.  They return None.
 
         Different calls to `sample` should produce the same value.
 
         """
         ...
 
-    def union(self: S, *others: S) -> S:
+    def union(self: Self, *others: Self) -> Self:
         "Return a domain containing elements of `self` or `other`."
         ...
 
     def __contains__(self, which: T) -> bool:
         "Return True if `which` is a member."
         ...
 
-    def __sub__(self: S, other: S) -> S:
+    def __sub__(self: Self, other: Self) -> Self:
         "Return a domain containing elements of `self` which are not members of `other`."
         ...
 
-    def __or__(self: S, other: S) -> S:
+    def __or__(self: Self, other: Self) -> Self:
         "Equivalent to `union`:meth:."
         ...
 
-    def __le__(self: S, other: S) -> bool:
+    def __le__(self: Self, other: Self) -> bool:
         "Return True if `self` is sub-set of `other`"
         ...
 
-    def __lt__(self: S, other: S) -> bool:
+    def __lt__(self: Self, other: Self) -> bool:
         "Return True if `self` is a proper sub-set of `other`"
         ...
 
-    def __ge__(self: S, other: S) -> bool:
+    def __ge__(self: Self, other: Self) -> bool:
         "Return True if `other` is a sub-set of `self`"
         ...
 
-    def __gt__(self: S, other: S) -> bool:
+    def __gt__(self: Self, other: Self) -> bool:
         "Return True if `other` is a proper sub-set of `self`"
         ...
 
-    def __and__(self: S, other: S) -> S:
+    def __and__(self: Self, other: Self) -> Self:
         "Return a domain containing common elements of `self` and `other`."
         ...
 
-    def __bool__(self: S) -> bool:
+    def __bool__(self) -> bool:
         "Return True if the domain is not empty."
         ...
 
 
 if t.TYPE_CHECKING:
     from datetime import datetime, timedelta
```

### Comparing `xotless-4.1.0/src/xotless/walk.py` & `xotless-4.1.3/src/xotless/walk.py`

 * *Files identical despite different names*

### Comparing `xotless-4.1.0/src/xotless/testing/strategies/domains.py` & `xotless-4.1.3/src/xotless/testing/strategies/domains.py`

 * *Files identical despite different names*

### Comparing `xotless-4.1.0/pyproject.toml` & `xotless-4.1.3/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -7,15 +7,21 @@
 dependencies = [
     "xotl.tools>=2.2.1,<4.0; python_version <= '3.11'",
     "xotl.tools>=3.0.0a5,<4.0; python_version > '3.11'",
 ]
 readme = "README.rst"
 requires-python = ">=3.8"
 license = "MIT"
-dynamic = ["urls", "version"]
+dynamic = ["version"]
+
+
+[project.urls]
+Documentation = "https://merchise-autrement.gitlab.io/xotless/"
+Repository = "https://gitlab.merchise.org/mercurio-2018/xotless/"
+
 
 [project.optional-dependencies]
 immutables = [
     "immutables>=0.20",
 ]
 
 [build-system]
@@ -33,25 +39,26 @@
 
 [tool.hatch.metadata.hooks.vcs]
 
 [tool.rye]
 managed = true
 dev-dependencies = [
     "sphinx~=7.1.2",
-    "ruff==0.4.2",
+    "ruff==0.4.3",
     "ruff-lsp>=0.0.52",
     "furo~=2024.1.29",
     "hypothesis~=6.98.6",
     "tox>=4.12.1",
     "isort>=5.13.2",
     "pip>=24.0",
     "mypy==1.10.0",
     "pytest>=8.0.1",
     "pytest-cov>=4.1.0",
     "pytest-xdist>=3.5.0",
+    "pyright==1.1.361",
 ]
 
 [tool.ruff]
 line-length = 100
 target-version = "py311"
 
 [tool.ruff.lint]
```

### Comparing `xotless-4.1.0/PKG-INFO` & `xotless-4.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: xotless
-Version: 4.1.0
+Version: 4.1.3
 Summary: Collection of small utilities that have not yet being promoted to xotl.tools.
 Author-email: "Merchise Autrement [~º/~]" <info@merchise.de>
 License-Expression: MIT
 Requires-Python: >=3.8
 Requires-Dist: xotl-tools<4.0,>=2.2.1; python_version <= '3.11'
 Requires-Dist: xotl-tools<4.0,>=3.0.0a5; python_version > '3.11'
 Provides-Extra: immutables
```

