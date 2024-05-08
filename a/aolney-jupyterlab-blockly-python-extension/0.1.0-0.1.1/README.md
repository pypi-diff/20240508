# Comparing `tmp/aolney_jupyterlab_blockly_python_extension-0.1.0.tar.gz` & `tmp/aolney_jupyterlab_blockly_python_extension-0.1.1.tar.gz`

## Comparing `aolney_jupyterlab_blockly_python_extension-0.1.0.tar` & `aolney_jupyterlab_blockly_python_extension-0.1.1.tar`

### file list

```diff
@@ -1,52 +1,53 @@
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.0/.copier-answers.yml
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.0/.prettierignore
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.0/.yarnrc.yml
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.0/CHANGELOG.md
--rw-r--r--   0        0        0     3951 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.0/RELEASE.md
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.0/babel.config.js
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.0/environment.yml
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.0/install.json
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.0/jest.config.js
--rw-r--r--   0        0        0   634891 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.0/package-lock.json
--rw-r--r--   0        0        0     6791 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.0/package.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.0/setup.py
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.0/tsconfig.json
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.0/tsconfig.test.json
--rwxr-xr-x   0        0        0       44 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.0/watch.sh
--rw-r--r--   0        0        0   378847 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.0/yarn.lock
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.0/aolney_jupyterlab_blockly_python_extension/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.0/aolney_jupyterlab_blockly_python_extension/_version.py
--rw-r--r--   0        0        0     6031 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.0/aolney_jupyterlab_blockly_python_extension/labextension/package.json
--rw-r--r--   0        0        0    29983 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.0/aolney_jupyterlab_blockly_python_extension/labextension/static/203.1521356dd3eabef73aae.js
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.0/aolney_jupyterlab_blockly_python_extension/labextension/static/203.1521356dd3eabef73aae.js.LICENSE.txt
--rw-r--r--   0        0        0    31898 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.0/aolney_jupyterlab_blockly_python_extension/labextension/static/369.5f4ab4479184dd6b56b7.js
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.0/aolney_jupyterlab_blockly_python_extension/labextension/static/369.5f4ab4479184dd6b56b7.js.LICENSE.txt
--rw-r--r--   0        0        0     4064 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.0/aolney_jupyterlab_blockly_python_extension/labextension/static/728.ea6e1ffef3f6bcb3b003.js
--rw-r--r--   0        0        0    45064 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.0/aolney_jupyterlab_blockly_python_extension/labextension/static/788.ac8ed33ecdaba7af1017.js
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.0/aolney_jupyterlab_blockly_python_extension/labextension/static/788.ac8ed33ecdaba7af1017.js.LICENSE.txt
--rw-r--r--   0        0        0   666972 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.0/aolney_jupyterlab_blockly_python_extension/labextension/static/88.f12ddff976fd53bc3a6c.js
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.0/aolney_jupyterlab_blockly_python_extension/labextension/static/88.f12ddff976fd53bc3a6c.js.LICENSE.txt
--rw-r--r--   0        0        0     7904 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.0/aolney_jupyterlab_blockly_python_extension/labextension/static/remoteEntry.8cc4b66a67cd4b700f08.js
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.0/aolney_jupyterlab_blockly_python_extension/labextension/static/style.js
--rw-r--r--   0        0        0     2581 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.0/aolney_jupyterlab_blockly_python_extension/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0     6815 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.0/src/SearchDropdown.ts
--rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.0/src/field_minus.ts
--rw-r--r--   0        0        0     2054 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.0/src/field_plus.ts
--rw-r--r--   0        0        0    17692 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.0/src/index.ts
--rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.0/src/logging.ts
--rw-r--r--   0        0        0    54321 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.0/src/toolbox.ts
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.0/src/__tests__/aolney_jupyterlab_blockly_python_extension.spec.ts
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.0/style/base.css
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.0/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.0/style/index.js
--rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.0/ui-tests/README.md
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.0/ui-tests/jupyter_server_test_config.py
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.0/ui-tests/package.json
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.0/ui-tests/playwright.config.js
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.0/ui-tests/yarn.lock
--rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.0/ui-tests/tests/aolney_jupyterlab_blockly_python_extension.spec.ts
--rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.0/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.0/LICENSE
--rw-r--r--   0        0        0     4663 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.0/README.md
--rw-r--r--   0        0        0     2615 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.0/pyproject.toml
--rw-r--r--   0        0        0    18879 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.1/.copier-answers.yml
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.1/.prettierignore
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.1/.yarnrc.yml
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.1/CHANGELOG.md
+-rw-r--r--   0        0        0     3951 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.1/RELEASE.md
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.1/babel.config.js
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.1/environment.yml
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.1/install.json
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.1/jest.config.js
+-rw-r--r--   0        0        0   634891 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.1/package-lock.json
+-rw-r--r--   0        0        0     6791 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.1/package.json
+-rw-r--r--   0        0        0    14745 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.1/python-test.ipynb
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.1/setup.py
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.1/tsconfig.json
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.1/tsconfig.test.json
+-rwxr-xr-x   0        0        0       44 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.1/watch.sh
+-rw-r--r--   0        0        0   378847 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.1/yarn.lock
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.1/aolney_jupyterlab_blockly_python_extension/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.1/aolney_jupyterlab_blockly_python_extension/_version.py
+-rw-r--r--   0        0        0     6031 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.1/aolney_jupyterlab_blockly_python_extension/labextension/package.json
+-rw-r--r--   0        0        0    29983 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.1/aolney_jupyterlab_blockly_python_extension/labextension/static/203.1521356dd3eabef73aae.js
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.1/aolney_jupyterlab_blockly_python_extension/labextension/static/203.1521356dd3eabef73aae.js.LICENSE.txt
+-rw-r--r--   0        0        0    31898 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.1/aolney_jupyterlab_blockly_python_extension/labextension/static/369.5f4ab4479184dd6b56b7.js
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.1/aolney_jupyterlab_blockly_python_extension/labextension/static/369.5f4ab4479184dd6b56b7.js.LICENSE.txt
+-rw-r--r--   0        0        0    46479 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.1/aolney_jupyterlab_blockly_python_extension/labextension/static/603.4a974815d784d1ce9ced.js
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.1/aolney_jupyterlab_blockly_python_extension/labextension/static/603.4a974815d784d1ce9ced.js.LICENSE.txt
+-rw-r--r--   0        0        0     4064 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.1/aolney_jupyterlab_blockly_python_extension/labextension/static/728.ea6e1ffef3f6bcb3b003.js
+-rw-r--r--   0        0        0   666972 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.1/aolney_jupyterlab_blockly_python_extension/labextension/static/88.f12ddff976fd53bc3a6c.js
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.1/aolney_jupyterlab_blockly_python_extension/labextension/static/88.f12ddff976fd53bc3a6c.js.LICENSE.txt
+-rw-r--r--   0        0        0     7904 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.1/aolney_jupyterlab_blockly_python_extension/labextension/static/remoteEntry.49e44ba8d7266e1def33.js
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.1/aolney_jupyterlab_blockly_python_extension/labextension/static/style.js
+-rw-r--r--   0        0        0     2581 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.1/aolney_jupyterlab_blockly_python_extension/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0     6815 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.1/src/SearchDropdown.ts
+-rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.1/src/field_minus.ts
+-rw-r--r--   0        0        0     2054 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.1/src/field_plus.ts
+-rw-r--r--   0        0        0    19571 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.1/src/index.ts
+-rw-r--r--   0        0        0     1939 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.1/src/logging.ts
+-rw-r--r--   0        0        0    54321 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.1/src/toolbox.ts
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.1/src/__tests__/aolney_jupyterlab_blockly_python_extension.spec.ts
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.1/style/base.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.1/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.1/style/index.js
+-rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.1/ui-tests/README.md
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.1/ui-tests/jupyter_server_test_config.py
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.1/ui-tests/package.json
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.1/ui-tests/playwright.config.js
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.1/ui-tests/yarn.lock
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.1/ui-tests/tests/aolney_jupyterlab_blockly_python_extension.spec.ts
+-rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.1/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.1/LICENSE
+-rw-r--r--   0        0        0     4929 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.1/README.md
+-rw-r--r--   0        0        0     2615 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0    19145 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_python_extension-0.1.1/PKG-INFO
```

### Comparing `aolney_jupyterlab_blockly_python_extension-0.1.0/.copier-answers.yml` & `aolney_jupyterlab_blockly_python_extension-0.1.1/.copier-answers.yml`

 * *Files identical despite different names*

### Comparing `aolney_jupyterlab_blockly_python_extension-0.1.0/RELEASE.md` & `aolney_jupyterlab_blockly_python_extension-0.1.1/RELEASE.md`

 * *Files identical despite different names*

### Comparing `aolney_jupyterlab_blockly_python_extension-0.1.0/jest.config.js` & `aolney_jupyterlab_blockly_python_extension-0.1.1/jest.config.js`

 * *Files identical despite different names*

### Comparing `aolney_jupyterlab_blockly_python_extension-0.1.0/package-lock.json` & `aolney_jupyterlab_blockly_python_extension-0.1.1/package-lock.json`

 * *Files identical despite different names*

### Comparing `aolney_jupyterlab_blockly_python_extension-0.1.0/package.json` & `aolney_jupyterlab_blockly_python_extension-0.1.1/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9791666666666666%*

 * *Differences: {"'version'": "'0.1.1'"}*

```diff
@@ -189,9 +189,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": "^([a-z][A-z\\d]*)(-[A-z\\d]+)*$",
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.1.0"
+    "version": "0.1.1"
 }
```

### Comparing `aolney_jupyterlab_blockly_python_extension-0.1.0/tsconfig.json` & `aolney_jupyterlab_blockly_python_extension-0.1.1/tsconfig.json`

 * *Files identical despite different names*

### Comparing `aolney_jupyterlab_blockly_python_extension-0.1.0/yarn.lock` & `aolney_jupyterlab_blockly_python_extension-0.1.1/yarn.lock`

 * *Files identical despite different names*

### Comparing `aolney_jupyterlab_blockly_python_extension-0.1.0/aolney_jupyterlab_blockly_python_extension/__init__.py` & `aolney_jupyterlab_blockly_python_extension-0.1.1/aolney_jupyterlab_blockly_python_extension/__init__.py`

 * *Files identical despite different names*

### Comparing `aolney_jupyterlab_blockly_python_extension-0.1.0/aolney_jupyterlab_blockly_python_extension/labextension/package.json` & `aolney_jupyterlab_blockly_python_extension-0.1.1/aolney_jupyterlab_blockly_python_extension/labextension/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9785879629629629%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.49e44ba8d7266e1def33.js'}}",*

 * * "'version'": "'0.1.1'"}*

```diff
@@ -108,15 +108,15 @@
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "src/**/*.{ts,tsx}"
     ],
     "homepage": "https://github.com/aolney/jupyterlab-blockly-python-extension",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.8cc4b66a67cd4b700f08.js",
+            "load": "static/remoteEntry.49e44ba8d7266e1def33.js",
             "style": "./style"
         },
         "extension": true,
         "outputDir": "aolney_jupyterlab_blockly_python_extension/labextension"
     },
     "keywords": [
         "jupyter",
@@ -194,9 +194,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": "^([a-z][A-z\\d]*)(-[A-z\\d]+)*$",
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.1.0"
+    "version": "0.1.1"
 }
```

### Comparing `aolney_jupyterlab_blockly_python_extension-0.1.0/aolney_jupyterlab_blockly_python_extension/labextension/static/203.1521356dd3eabef73aae.js` & `aolney_jupyterlab_blockly_python_extension-0.1.1/aolney_jupyterlab_blockly_python_extension/labextension/static/203.1521356dd3eabef73aae.js`

 * *Files identical despite different names*

### Comparing `aolney_jupyterlab_blockly_python_extension-0.1.0/aolney_jupyterlab_blockly_python_extension/labextension/static/369.5f4ab4479184dd6b56b7.js` & `aolney_jupyterlab_blockly_python_extension-0.1.1/aolney_jupyterlab_blockly_python_extension/labextension/static/369.5f4ab4479184dd6b56b7.js`

 * *Files identical despite different names*

### Comparing `aolney_jupyterlab_blockly_python_extension-0.1.0/aolney_jupyterlab_blockly_python_extension/labextension/static/728.ea6e1ffef3f6bcb3b003.js` & `aolney_jupyterlab_blockly_python_extension-0.1.1/aolney_jupyterlab_blockly_python_extension/labextension/static/728.ea6e1ffef3f6bcb3b003.js`

 * *Files identical despite different names*

### Comparing `aolney_jupyterlab_blockly_python_extension-0.1.0/aolney_jupyterlab_blockly_python_extension/labextension/static/788.ac8ed33ecdaba7af1017.js` & `aolney_jupyterlab_blockly_python_extension-0.1.1/aolney_jupyterlab_blockly_python_extension/labextension/static/603.4a974815d784d1ce9ced.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -1,45 +1,45 @@
-/*! For license information please see 788.ac8ed33ecdaba7af1017.js.LICENSE.txt */
+/*! For license information please see 603.4a974815d784d1ce9ced.js.LICENSE.txt */
 "use strict";
 (self.webpackChunk_aolney_jupyterlab_blockly_python_extension = self.webpackChunk_aolney_jupyterlab_blockly_python_extension || []).push([
-    [788], {
-        788: (e, t, n) => {
+    [603], {
+        603: (e, t, n) => {
             n.r(t), n.d(t, {
-                BlocklyWidget_$ctor_A44FDC6: () => H,
-                BlocklyWidget__ActiveCellSerializedBlocksWorkspaceOption: () => $,
-                BlocklyWidget__RenderBlocks: () => te,
-                BlocklyWidget__RenderCode: () => ee,
-                BlocklyWidget__RenderCodeToLastCell: () => ne,
-                BlocklyWidget__clearBlocks: () => oe,
-                BlocklyWidget__get_Notebooks: () => j,
-                BlocklyWidget__get_blocksRendered: () => Y,
-                BlocklyWidget__get_lastCell: () => Z,
-                BlocklyWidget__get_notHooked: () => z,
-                BlocklyWidget__get_onActiveCellChanged: () => Q,
-                BlocklyWidget__get_onKernelExecuted: () => J,
-                BlocklyWidget__get_workspace: () => W,
-                BlocklyWidget__set_blocksRendered_Z1FBCCD16: () => X,
-                BlocklyWidget__set_lastCell_Z4422E5A0: () => q,
-                BlocklyWidget__set_notHooked_Z1FBCCD16: () => K,
-                BlocklyWidget__set_workspace_Z1D3C0780: () => G,
-                attachWidget: () => le,
-                createMainAreaWidget: () => ie,
-                default: () => ce,
-                onKernelChanged: () => ae,
-                onNotebookChanged: () => se,
-                runCommandOnNotebookChanged: () => re
+                BlocklyWidget_$ctor_A44FDC6: () => K,
+                BlocklyWidget__ActiveCellSerializedBlocksWorkspaceOption: () => oe,
+                BlocklyWidget__RenderBlocks: () => ie,
+                BlocklyWidget__RenderCode: () => le,
+                BlocklyWidget__RenderCodeToLastCell: () => ae,
+                BlocklyWidget__clearBlocks: () => se,
+                BlocklyWidget__get_Notebooks: () => z,
+                BlocklyWidget__get_blocksRendered: () => J,
+                BlocklyWidget__get_lastCell: () => $,
+                BlocklyWidget__get_notHooked: () => q,
+                BlocklyWidget__get_onActiveCellChanged: () => ne,
+                BlocklyWidget__get_onKernelExecuted: () => te,
+                BlocklyWidget__get_workspace: () => Y,
+                BlocklyWidget__set_blocksRendered_Z1FBCCD16: () => Z,
+                BlocklyWidget__set_lastCell_Z4422E5A0: () => ee,
+                BlocklyWidget__set_notHooked_Z1FBCCD16: () => Q,
+                BlocklyWidget__set_workspace_Z1D3C0780: () => X,
+                attachWidget: () => re,
+                createMainAreaWidget: () => ce,
+                default: () => pe,
+                onKernelChanged: () => ue,
+                onNotebookChanged: () => de,
+                runCommandOnNotebookChanged: () => he
             });
-            var o = n(465),
-                l = n(638),
-                i = n(315),
+            var o = n(626),
+                l = n(923),
+                i = n(206),
                 a = n(256),
-                s = n(372),
+                s = n(291),
                 r = n(983),
                 c = n(203),
-                u = n(723);
+                u = n(236);
 
             function d(e) {
                 const t = e.getSourceBlock();
                 if (t.isInFlyout) return;
                 r.Events.setGroup(!0);
                 const n = t.mutationToDom(),
                     o = n && r.Xml.domToText(n);
@@ -197,15 +197,15 @@
                 r.Blocks[e] = {
                     init: function() {
                         this.appendDummyInput().appendField(t).appendField(new r.FieldTextInput("some library"), "libraryName").appendField(n).appendField(new r.FieldVariable("variable name"), "libraryAlias"), this.setNextStatement(!0), this.setPreviousStatement(!0), this.setColour(230), this.setTooltip("Import a python package to access functions in that package"), this.setHelpUrl("https://docs.python.org/3/reference/import.html")
                     }
                 }, c.pythonGenerator[e] = e => t + " " + e.getFieldValue("libraryName") + " " + n + " " + c.pythonGenerator.getVariableName(e.getFieldValue("libraryAlias")) + "\n"
             }
 
-            function I(e, t, n, o, l, i) {
+            function w(e, t, n, o, l, i) {
                 r.Blocks[e] = {
                     init: function() {
                         console.log(e + " init"), this.appendValueInput("x").setCheck(null).appendField(t), this.setInputsInline(!0), this.setOutput(!0, n), this.setColour(230), this.setTooltip(o), this.setHelpUrl(l)
                     }
                 }, c.pythonGenerator[e] = e => [i + "(" + c.pythonGenerator.valueToCode(e, "x", c.pythonGenerator.ORDER_MEMBER).replace("^\\[|\\]$", "") + ")", c.pythonGenerator.ORDER_FUNCTION_CALL]
             }
             c.pythonGenerator.finish = e => {
@@ -244,20 +244,20 @@
                 init: function() {
                     console.log("openWriteFile_Python init"), this.appendValueInput("FILENAME").setCheck("String").appendField("open file for writing"), this.setOutput(!0, null), this.setColour(230), this.setTooltip("Use this to write to a file. It will output a file, not a string."), this.setHelpUrl("https://docs.python.org/3/tutorial/inputoutput.html")
                 }
             }, c.pythonGenerator.openWriteFile_Python = e => ["open(" + c.pythonGenerator.valueToCode(e, "FILENAME", c.pythonGenerator.ORDER_ATOMIC) + ",'w',encoding='utf-8')", c.pythonGenerator.ORDER_FUNCTION_CALL], v("dummyOutputCodeBlock_Python", !1, !0), v("dummyNoOutputCodeBlock_Python", !1, !1), v("valueOutputCodeBlock_Python", !0, !0), v("valueNoOutputCodeBlock_Python", !0, !1), E("dummyOutputCommentBlock_Python", !1, !0), E("dummyNoOutputCommentBlock_Python", !1, !1), E("valueOutputCommentBlock_Python", !0, !0), E("valueNoOutputCommentBlock_Python", !0, !1), C("importAs_Python", "import", "as"), C("importFrom_Python", "from", "import"), r.Blocks.indexer_Python = {
                 init: function() {
                     this.appendValueInput("INDEX").appendField(new r.FieldVariable("{dictVariable}"), "VAR").appendField("["), this.appendDummyInput().appendField("]"), this.setInputsInline(!0), this.setOutput(!0), this.setColour(230), this.setTooltip("Gets an item from the variable at a given index. Not supported for all variables."), this.setHelpUrl("https://docs.python.org/3/reference/datamodel.html#object.__getitem__")
                 }
-            }, c.pythonGenerator.indexer_Python = e => [c.pythonGenerator.getVariableName(e.getFieldValue("VAR")) + "[" + c.pythonGenerator.valueToCode(e, "INDEX", c.pythonGenerator.ORDER_ATOMIC) + "]", c.pythonGenerator.ORDER_ATOMIC], I("reversedBlock_Python", "reversed", "None", "Create a reversed iterator to reverse a list or a tuple; wrap it in a new list or tuple.", "https://docs.python.org/3/library/functions.html#reversed", "reversed"), I("tupleConstructorBlock_Python", "tuple", "None", "Create a tuple from a list, e.g. ['a','b'] becomes ('a','b')", "https://docs.python.org/3/library/stdtypes.html#tuple", "tuple"), I("dictBlock_Python", "dict", "None", "Create a dictionary from a list of tuples, e.g. [('a',1),('b',2)...]", "https://docs.python.org/3/tutorial/datastructures.html#dictionaries", "dict"), I("listBlock_Python", "list", "None", "Create a list from an iterable, e.g. list(zip(...))", "https://docs.python.org/3/library/stdtypes.html#typesseq-list", "list"), I("zipBlock_Python", "zip", "Array", "Zip together two or more lists", "https://docs.python.org/3.3/library/functions.html#zip", "zip"), I("sortedBlock_Python", "as sorted", "Array", "Sort lists of stuff", "https://docs.python.org/3.3/library/functions.html#sorted", "sorted"), I("setBlock_Python", "set", "Array", "Make a set with unique members of a list.", "https://docs.python.org/2/library/sets.html", "set"), I("boolConversion_Python", "as bool", "Boolean", "Convert something to Boolean.", "https://docs.python.org/3/library/stdtypes.html#boolean-values", "bool"), I("strConversion_Python", "as str", "String", "Convert something to String.", "https://docs.python.org/3/library/stdtypes.html#str", "str"), I("floatConversion_Python", "as float", "Number", "Convert something to Float.", "https://docs.python.org/3/library/functions.html#float", "float"), I("intConversion_Python", "as int", "Number", "Convert something to Int.", "https://docs.python.org/3/library/functions.html#int", "int"), I("getInput_Python", "input", "String", "Present the given prompt to the user and wait for their typed input response.", "https://docs.python.org/3/library/functions.html#input", "input"), r.Blocks.tupleBlock_Python = {
+            }, c.pythonGenerator.indexer_Python = e => [c.pythonGenerator.getVariableName(e.getFieldValue("VAR")) + "[" + c.pythonGenerator.valueToCode(e, "INDEX", c.pythonGenerator.ORDER_ATOMIC) + "]", c.pythonGenerator.ORDER_ATOMIC], w("reversedBlock_Python", "reversed", "None", "Create a reversed iterator to reverse a list or a tuple; wrap it in a new list or tuple.", "https://docs.python.org/3/library/functions.html#reversed", "reversed"), w("tupleConstructorBlock_Python", "tuple", "None", "Create a tuple from a list, e.g. ['a','b'] becomes ('a','b')", "https://docs.python.org/3/library/stdtypes.html#tuple", "tuple"), w("dictBlock_Python", "dict", "None", "Create a dictionary from a list of tuples, e.g. [('a',1),('b',2)...]", "https://docs.python.org/3/tutorial/datastructures.html#dictionaries", "dict"), w("listBlock_Python", "list", "None", "Create a list from an iterable, e.g. list(zip(...))", "https://docs.python.org/3/library/stdtypes.html#typesseq-list", "list"), w("zipBlock_Python", "zip", "Array", "Zip together two or more lists", "https://docs.python.org/3.3/library/functions.html#zip", "zip"), w("sortedBlock_Python", "as sorted", "Array", "Sort lists of stuff", "https://docs.python.org/3.3/library/functions.html#sorted", "sorted"), w("setBlock_Python", "set", "Array", "Make a set with unique members of a list.", "https://docs.python.org/2/library/sets.html", "set"), w("boolConversion_Python", "as bool", "Boolean", "Convert something to Boolean.", "https://docs.python.org/3/library/stdtypes.html#boolean-values", "bool"), w("strConversion_Python", "as str", "String", "Convert something to String.", "https://docs.python.org/3/library/stdtypes.html#str", "str"), w("floatConversion_Python", "as float", "Number", "Convert something to Float.", "https://docs.python.org/3/library/functions.html#float", "float"), w("intConversion_Python", "as int", "Number", "Convert something to Int.", "https://docs.python.org/3/library/functions.html#int", "int"), w("getInput_Python", "input", "String", "Present the given prompt to the user and wait for their typed input response.", "https://docs.python.org/3/library/functions.html#input", "input"), r.Blocks.tupleBlock_Python = {
                 init: function() {
                     this.appendValueInput("FIRST").setCheck(null).appendField("("), this.appendValueInput("SECOND").setCheck(null).appendField(","), this.appendDummyInput().appendField(")"), this.setInputsInline(!0), this.setOutput(!0, null), this.setColour(230), this.setTooltip("Use this to create a two-element tuple"), this.setHelpUrl("https://docs.python.org/3/tutorial/datastructures.html#tuples-and-sequences")
                 }
             }, c.pythonGenerator.tupleBlock_Python = e => ["(" + c.pythonGenerator.valueToCode(e, "FIRST", c.pythonGenerator.ORDER_ATOMIC) + "," + c.pythonGenerator.valueToCode(e, "SECOND", c.pythonGenerator.ORDER_ATOMIC) + ")", c.pythonGenerator.ORDER_NONE];
-            class w {
+            class I {
                 constructor(e, t, n, o) {
                     this.Name = e, this.Info = t, this.isFunction = n, this.isClass = o
                 }
             }
             class T {
                 constructor(e, t) {
                     this.VariableEntry = e, this.ChildEntries = t
@@ -316,22 +316,22 @@
             }
             const O = new Map([]);
 
             function D(e) {
                 return e.includes("Signature:") && e.includes("function")
             }
 
-            function A(e) {
+            function R(e) {
                 return e.includes("signature:") && e.includes("class")
             }
 
-            function R(e, t) {
+            function A(e, t) {
                 return "" === t || e.isInFlyout || function(e, t) {
                     N(t).then((n => {
-                        const o = new w(t, n, D(n), A(n));
+                        const o = new I(t, n, D(n), R(n));
                         let l, i = new T(o, []);
                         const a = [O.has(o.Name), i];
                         if (a[0]) {
                             const e = a[1];
                             l = e.VariableEntry.Info !== o.Info || 0 === e.ChildEntries.length
                         } else l = !0;
                         l ? function(e) {
@@ -355,15 +355,15 @@
                                     }), 100)
                                 }))
                             }
                         }(t + ".").then((e => {
                             const n = e.filter((e => 0 !== o.Info.indexOf("Signature: DataFrame") || !(0 === e.indexOf("_") || 0 === e.indexOf("style")))),
                                 l = n.map((e => N(t + "." + e)));
                             return Promise.all(l).then((e => {
-                                const l = new T(o, n.map(((t, n) => new w(t, e[n], D(e[n]), A(e[n])))));
+                                const l = new T(o, n.map(((t, n) => new I(t, e[n], D(e[n]), R(e[n])))));
                                 O.has(t) ? O.set(t, l) : function(e, t, n) {
                                     if (e.has(t)) throw new Error("An item with the same key has already been added. Key: " + t);
                                     e.set(t, n)
                                 }(O, t, l)
                             }))
                         })).then((function() {
                             const t = new r.Events.BlockChange(e, "field", "VAR", 0, 1);
@@ -379,30 +379,30 @@
                 ] : "" !== t && O.has(t) ? [
                     ["!Waiting for kernel to respond with options.", "!Waiting for kernel to respond with options."]
                 ] : [
                     ["!Not defined until you execute code.", "!Not defined until you execute code."]
                 ]
             }
 
-            function B(e, t) {
+            function P(e, t) {
                 var n;
                 const o = (i = e, null, (l = O).has(i) ? [!0, l.get(i)] : [!1, null]);
                 var l, i;
                 if (o[0]) {
                     const e = null === (n = o[1]) || void 0 === n ? void 0 : n.ChildEntries.find((e => e.Name === t));
                     return null == e ? "!Not defined until you execute code." : e.Info
                 }
                 return "!Not defined until you execute code."
             }
 
-            function P() {
+            function B() {
                 const e = r.getMainWorkspace(),
                     t = e.getBlocksByType("varGetProperty_Python", !1);
                 e.getBlocksByType("varDoMethod_Python", !1).forEach((e => t.push(e))), t.forEach((e => {
-                    e.updateIntellisense(e, null, (t => R(e, t)))
+                    e.updateIntellisense(e, null, (t => A(e, t)))
                 })), e.registerToolboxCategoryCallback("VARIABLE", r.Variables.flyoutCategoryBlocks)
             }
 
             function F(e, t, n) {
                 const o = e.getField(t),
                     l = e.getInput(n);
                 o && (l ? l.removeField(t) : console.log("error removing (" + t + ") from block; input (" + n + ") does not exist"))
@@ -433,24 +433,24 @@
                             i = n(l).map((e => e[0])),
                             a = e.data ? e.data : "",
                             s = a.indexOf(":") >= 0 ? a.split(":")[1] : "";
                         if (o) {
                             let t = new g.FieldFilter(s, i, (function(t) {
                                 const n = "" === t ? s : this.WORDS[t];
                                 let o;
-                                return this.setTooltip(B(l, n)), e.selectedMember = (o = [0 === n.indexOf("!"), this.selectedMember], "" === o[1] ? n : o[0] ? this.selectedMember : n), "" !== l && "" !== e.selectedMember && (e.data = l + ":" + e.selectedMember), n
+                                return this.setTooltip(P(l, n)), e.selectedMember = (o = [0 === n.indexOf("!"), this.selectedMember], "" === o[1] ? n : o[0] ? this.selectedMember : n), "" !== l && "" !== e.selectedMember && (e.data = l + ":" + e.selectedMember), n
                             }));
                             o.appendField(t, "MEMBER")
                         }
                         void 0 !== e.data && null !== e.data || (e.data = l + ":" + e.selectedMember);
                         const r = e.getField("MEMBER");
-                        r && r.setTooltip(B(l, r.getText()))
+                        r && r.setTooltip(P(l, r.getText()))
                     },
                     init: function() {
-                        console.log(e + " init"), this.appendDummyInput("INPUT").appendField(t).appendField(new r.FieldVariable("variable name", (e => (this.updateIntellisense(this, e, (e => R(this, e))), e))), "VAR").appendField(n), this.updateIntellisense(this, null, (e => R(this, e))), this.setOutput(!0), this.setColour(230), this.setTooltip("!Not defined until you execute code."), this.setHelpUrl(""), l && (this.appendDummyInput("EMPTY"), r.Extensions.apply("intelliblockMutator_Python", this, !0))
+                        console.log(e + " init"), this.appendDummyInput("INPUT").appendField(t).appendField(new r.FieldVariable("variable name", (e => (this.updateIntellisense(this, e, (e => A(this, e))), e))), "VAR").appendField(n), this.updateIntellisense(this, null, (e => A(this, e))), this.setOutput(!0), this.setColour(230), this.setTooltip("!Not defined until you execute code."), this.setHelpUrl(""), l && (this.appendDummyInput("EMPTY"), r.Extensions.apply("intelliblockMutator_Python", this, !0))
                     },
                     onchange: function(e) {
                         if (this.workspace && !this.isInFlyout && "INTELLISENSE" === e.group) {
                             const e = this.data ? this.data.toString().split(":") : "";
                             this.updateIntellisense(this, null, (e => function(e, t) {
                                 const n = O.get(t);
                                 return n ? !n.VariableEntry.isFunction && n.ChildEntries.length > 0 ? n.ChildEntries.filter(e).map((e => [e.Name, e.Name])) : "UNDEFINED" === n.VariableEntry.Info ? [
@@ -575,177 +575,225 @@
                             l.setAttribute("type", "variables_get"), l.setAttribute("gap", "8"), l.appendChild(r.Variables.generateVariableFieldDom(o)), n.push(l), e++
                         }
                     }
                 }
                 return n
             }))), n(499);
             var L = n(808);
+
+            function V(e, t) {
+                return {
+                    schema: "jle050824",
+                    name: e,
+                    payload: t
+                }
+            }
+            let G, W;
+
+            function j(e) {
+                if (G) {
+                    let l = window.location.href;
+                    W && (l = W), window.fetch(G, {
+                        method: "POST",
+                        headers: {
+                            "Content-Type": "application/json"
+                        },
+                        body: JSON.stringify({
+                            username: l,
+                            json: (t = e, 0 === (null === (o = null === (n = null == t ? void 0 : t.object) || void 0 === n ? void 0 : n.element) || void 0 === o ? void 0 : o.toString().indexOf("drag")) && (t.object.newValue = void 0, t.object.oldValue = void 0), t)
+                        })
+                    }).then((e => {
+                        e.ok || console.log(e.statusText)
+                    }))
+                }
+                var t, n, o
+            }
             r.setLocale(L);
-            class V extends a.Widget {
+            class H extends a.Widget {
                 constructor(e) {
                     super(), this.onResize = e => {
                             let t = e.width,
                                 n = e.width;
                             const o = document.getElementById("blocklyDivPython"),
                                 l = document.getElementById("buttonDivPython"),
                                 i = e.height - 30;
-                            o.setAttribute("style", "width: " + (t = e.width, t.toString() + "px; height: ") + i.toString() + "px"), l.setAttribute("style", "position: absolute; top: " + i.toString() + "px; left: 0px; width: " + (n = e.width, n.toString() + "px; height: 30px")), r.svgResize(W(this))
-                        }, this.notebooks = e, this.generator = c.pythonGenerator, this.notebooks.activeCellChanged.connect(Q(this), this),
+                            o.setAttribute("style", "width: " + (t = e.width, t.toString() + "px; height: ") + i.toString() + "px"), l.setAttribute("style", "position: absolute; top: " + i.toString() + "px; left: 0px; width: " + (n = e.width, n.toString() + "px; height: 30px")), r.svgResize(Y(this))
+                        }, this.notebooks = e, this.generator = c.pythonGenerator, this.notebooks.activeCellChanged.connect(ne(this), this),
                         function(e) {
                             x = e
                         }(this.notebooks), this.div = document.createElement("div"), this.div.id = "blocklyDivPython", this.node.appendChild(this.div);
                     const t = document.createElement("div");
                     t.id = "buttonDivPython";
                     const n = document.createElement("button");
                     n.innerText = "Blocks to Code", t.appendChild(n), n.addEventListener("click", (e => {
-                        ee(this)
+                        le(this)
                     }));
                     const o = document.createElement("button");
                     o.innerText = "Code to Blocks", o.addEventListener("click", (e => {
-                        te(this)
+                        ie(this)
                     })), t.appendChild(o);
                     const l = document.createElement("button");
                     l.innerText = "Report Bug", l.addEventListener("click", (e => {
                         const t = window.open("https://github.com/aolney/jupyterlab-blockly-python-extension/issues", "_blank");
                         t && t.focus()
                     })), t.appendChild(l);
                     const i = document.createElement("input");
                     i.setAttribute("type", "checkbox"), i.checked = !0, i.id = "syncCheckboxPython";
                     const a = document.createElement("label");
                     a.innerText = "Notebook Sync", a.setAttribute("for", "syncCheckboxPython"), t.appendChild(i), t.appendChild(a), this.node.appendChild(t), this["blocksRendered@"] = !1, this["notHooked@"] = !0, this["init@34"] = 1
                 }
                 onAfterAttach() {
                     const e = this;
-                    G(e, r.inject("blocklyDivPython", {
+                    X(e, r.inject("blocklyDivPython", {
                         toolbox: '<xml xmlns="https://developers.google.com/blockly/xml" id="toolbox" style="display: none">\n    <category name="IMPORT" colour="255">\n      <block type="importAs_Python"></block>\n      <block type="importFrom_Python"></block>\n    </category>\n    <category name="FREESTYLE" colour="290">\n      <block type="dummyOutputCodeBlock_Python"></block>\n      <block type="dummyNoOutputCodeBlock_Python"></block>\n      <block type="valueOutputCodeBlock_Python"></block>\n      <block type="valueNoOutputCodeBlock_Python"></block>\n    </category>\n    <category name="COMMENT" colour="%{BKY_COLOUR_HUE}">\n      <block type="dummyOutputCommentBlock_Python"></block>\n      <block type="dummyNoOutputCommentBlock_Python"></block>\n      <block type="valueOutputCommentBlock_Python"></block>\n      <block type="valueNoOutputCommentBlock_Python"></block>\n    </category>\n    <category name="LOGIC" colour="%{BKY_LOGIC_HUE}">\n      <block type="controls_if"></block>\n      <block type="logic_compare"></block>\n      <block type="logic_operation"></block>\n      <block type="logic_negate"></block>\n      <block type="logic_boolean"></block>\n      <block type="logic_null"></block>\n      <block type="logic_ternary"></block>\n    </category>\n    <category name="LOOPS" colour="%{BKY_LOOPS_HUE}">\n      <block type="controls_repeat_ext">\n        <value name="TIMES">\n          <shadow type="math_number">\n            <field name="NUM">10</field>\n          </shadow>\n        </value>\n      </block>\n      <block type="controls_whileUntil"></block>\n      <block type="controls_for">\n        <value name="FROM">\n          <shadow type="math_number">\n            <field name="NUM">1</field>\n          </shadow>\n        </value>\n        <value name="TO">\n          <shadow type="math_number">\n            <field name="NUM">10</field>\n          </shadow>\n        </value>\n        <value name="BY">\n          <shadow type="math_number">\n            <field name="NUM">1</field>\n          </shadow>\n        </value>\n      </block>\n      <block type="comprehensionForEach_Python"></block>\n      <block type="controls_forEach"></block>\n      <block type="controls_flow_statements"></block>\n    </category>\n    <category name="MATH" colour="%{BKY_MATH_HUE}">\n      <block type="math_number">\n        <field name="NUM">123</field>\n      </block>\n      <block type="math_arithmetic">\n        <value name="A">\n          <shadow type="math_number">\n            <field name="NUM">1</field>\n          </shadow>\n        </value>\n        <value name="B">\n          <shadow type="math_number">\n            <field name="NUM">1</field>\n          </shadow>\n        </value>\n      </block>\n      <block type="math_single">\n        <value name="NUM">\n          <shadow type="math_number">\n            <field name="NUM">9</field>\n          </shadow>\n        </value>\n      </block>\n      <block type="math_trig">\n        <value name="NUM">\n          <shadow type="math_number">\n            <field name="NUM">45</field>\n          </shadow>\n        </value>\n      </block>\n      <block type="math_constant"></block>\n      <block type="math_number_property">\n        <value name="NUMBER_TO_CHECK">\n          <shadow type="math_number">\n            <field name="NUM">0</field>\n          </shadow>\n        </value>\n      </block>\n      <block type="math_round">\n        <value name="NUM">\n          <shadow type="math_number">\n            <field name="NUM">3.1</field>\n          </shadow>\n        </value>\n      </block>\n      <block type="math_on_list"></block>\n      <block type="math_modulo">\n        <value name="DIVIDEND">\n          <shadow type="math_number">\n            <field name="NUM">64</field>\n          </shadow>\n        </value>\n        <value name="DIVISOR">\n          <shadow type="math_number">\n            <field name="NUM">10</field>\n          </shadow>\n        </value>\n      </block>\n      <block type="math_constrain">\n        <value name="VALUE">\n          <shadow type="math_number">\n            <field name="NUM">50</field>\n          </shadow>\n        </value>\n        <value name="LOW">\n          <shadow type="math_number">\n            <field name="NUM">1</field>\n          </shadow>\n        </value>\n        <value name="HIGH">\n          <shadow type="math_number">\n            <field name="NUM">100</field>\n          </shadow>\n        </value>\n      </block>\n      <block type="math_random_int">\n        <value name="FROM">\n          <shadow type="math_number">\n            <field name="NUM">1</field>\n          </shadow>\n        </value>\n        <value name="TO">\n          <shadow type="math_number">\n            <field name="NUM">100</field>\n          </shadow>\n        </value>\n      </block>\n      <block type="math_random_float"></block>\n      <block type="math_atan2">\n        <value name="X">\n          <shadow type="math_number">\n            <field name="NUM">1</field>\n          </shadow>\n        </value>\n        <value name="Y">\n          <shadow type="math_number">\n            <field name="NUM">1</field>\n          </shadow>\n        </value>\n      </block>\n    </category>\n    <category name="TEXT" colour="%{BKY_TEXTS_HUE}">\n      <block type="text"></block>\n      <block type="text_join"></block>\n      <block type="text_append">\n        <value name="TEXT">\n          <shadow type="text"></shadow>\n        </value>\n      </block>\n      <block type="text_length">\n        <value name="VALUE">\n          <shadow type="text">\n            <field name="TEXT">abc</field>\n          </shadow>\n        </value>\n      </block>\n      <block type="text_isEmpty">\n        <value name="VALUE">\n          <shadow type="text">\n            <field name="TEXT"></field>\n          </shadow>\n        </value>\n      </block>\n      <block type="text_indexOf">\n        <value name="VALUE">\n          <block type="variables_get">\n            <field name="VAR">{textVariable}</field>\n          </block>\n        </value>\n        <value name="FIND">\n          <shadow type="text">\n            <field name="TEXT">abc</field>\n          </shadow>\n        </value>\n      </block>\n      <block type="text_charAt">\n        <value name="VALUE">\n          <block type="variables_get">\n            <field name="VAR">{textVariable}</field>\n          </block>\n        </value>\n      </block>\n      <block type="text_getSubstring">\n        <value name="STRING">\n          <block type="variables_get">\n            <field name="VAR">{textVariable}</field>\n          </block>\n        </value>\n      </block>\n      <block type="text_changeCase">\n        <value name="TEXT">\n          <shadow type="text">\n            <field name="TEXT">abc</field>\n          </shadow>\n        </value>\n      </block>\n      <block type="text_trim">\n        <value name="TEXT">\n          <shadow type="text">\n            <field name="TEXT">abc</field>\n          </shadow>\n        </value>\n      </block>\n      <block type="text_print">\n        <value name="TEXT">\n          <shadow type="text">\n            <field name="TEXT">abc</field>\n          </shadow>\n        </value>\n      </block>\n      <block type="text_prompt_ext">\n        <value name="TEXT">\n          <shadow type="text">\n            <field name="TEXT">abc</field>\n          </shadow>\n        </value>\n      </block>\n      \x3c!-- <block type="getInput">\n        <value name="x">\n          <shadow type="text">\n            <field name="TEXT">The prompt shown to the user</field>\n          </shadow>\n        </value>\n      </block> --\x3e\n    </category>\n    <category name="LISTS" colour="%{BKY_LISTS_HUE}">\n      <block type="lists_create_with">\n        <mutation items="0"></mutation>\n      </block>\n      <block type="lists_create_with"></block>\n      <block type="lists_repeat">\n        <value name="NUM">\n          <shadow type="math_number">\n            <field name="NUM">5</field>\n          </shadow>\n        </value>\n      </block>\n      <block type="lists_length"></block>\n      <block type="lists_isEmpty"></block>\n      <block type="lists_indexOf">\n        <value name="VALUE">\n          <block type="variables_get">\n            <field name="VAR">{listVariable}</field>\n          </block>\n        </value>\n      </block>\n      <block type="lists_getIndex">\n        <value name="VALUE">\n          <block type="variables_get">\n            <field name="VAR">{listVariable}</field>\n          </block>\n        </value>\n      </block>\n      <block type="lists_setIndex">\n        <value name="LIST">\n          <block type="variables_get">\n            <field name="VAR">{listVariable}</field>\n          </block>\n        </value>\n      </block>\n      <block type="lists_getSublist">\n        <value name="LIST">\n          <block type="variables_get">\n            <field name="VAR">{listVariable}</field>\n          </block>\n        </value>\n      </block>\n      <block type="indexer_Python"></block>\n      <block type="lists_split">\n        <value name="DELIM">\n          <shadow type="text">\n            <field name="TEXT">,</field>\n          </shadow>\n        </value>\n      </block>\n      <block type="lists_sort"></block>\n      <block type="setBlock_Python"></block>\n      <block type="sortedBlock_Python"></block>\n      <block type="zipBlock_Python"></block>\n      <block type="dictBlock_Python"></block>\n      <block type="listBlock_Python"></block>\n      <block type="tupleBlock_Python"></block>\n      <block type="tupleConstructorBlock_Python"></block>\n      <block type="reversedBlock_Python"></block>\n    </category>\n    <category name="COLOUR" colour="%{BKY_COLOUR_HUE}">\n      <block type="colour_picker"></block>\n      <block type="colour_random"></block>\n      <block type="colour_rgb">\n        <value name="RED">\n          <shadow type="math_number">\n            <field name="NUM">100</field>\n          </shadow>\n        </value>\n        <value name="GREEN">\n          <shadow type="math_number">\n            <field name="NUM">50</field>\n          </shadow>\n        </value>\n        <value name="BLUE">\n          <shadow type="math_number">\n            <field name="NUM">0</field>\n          </shadow>\n        </value>\n      </block>\n      <block type="colour_blend">\n        <value name="COLOUR1">\n          <shadow type="colour_picker">\n            <field name="COLOUR">#ff0000</field>\n          </shadow>\n        </value>\n        <value name="COLOUR2">\n          <shadow type="colour_picker">\n            <field name="COLOUR">#3333ff</field>\n          </shadow>\n        </value>\n        <value name="RATIO">\n          <shadow type="math_number">\n            <field name="NUM">0.5</field>\n          </shadow>\n        </value>\n      </block>Conversion\n    </category>\n    <category name="CONVERSION" colour="120">\n      <block type="boolConversion_Python">\n      </block>\n      <block type="intConversion_Python">\n      </block>\n      <block type="floatConversion_Python">\n      </block>\n      <block type="strConversion_Python">\n      </block>\n    </category>\n    <category name="I/O" colour="190">\n      <block type="withAs_Python">\n      </block>\n      <block type="textFromFile_Python">\n        <value name="FILENAME">\n          <shadow type="text">\n            <field name="TEXT">name of file</field>\n          </shadow>\n        </value>\n      </block>\n      <block type="openReadFile_Python">\n              <value name="FILENAME">\n          <shadow type="text">\n            <field name="TEXT">name of file</field>\n          </shadow>\n        </value>\n      </block>\n      <block type="openWriteFile_Python">\n              <value name="FILENAME">\n          <shadow type="text">\n            <field name="TEXT">name of file</field>\n          </shadow>\n        </value>\n      </block>\n    </category>\n    <sep></sep>\n    <category name="VARIABLES" colour="%{BKY_VARIABLES_HUE}" custom="VARIABLE"></category>\n    <category name="FUNCTIONS" colour="%{BKY_PROCEDURES_HUE}" custom="PROCEDURE"></category>\n  </xml>'
                     })), console.log("jupyterlab_blockly_extension_python: blockly palette initialized");
                     const t = t => {
-                        "create" === t.type && X(e, !1), "finished_loading" === t.type && X(e, !0)
+                        "create" === t.type && Z(e, !1), "finished_loading" === t.type && Z(e, !0), j({
+                            schema: "ble050824",
+                            name: t.type,
+                            object: t.toJson()
+                        })
                     };
-                    W(e).removeChangeListener(t), W(e).addChangeListener(t)
+                    Y(e).removeChangeListener(t), Y(e).addChangeListener(t)
                 }
             }
 
-            function G(e, t) {
+            function X(e, t) {
                 e["workspace@"] = t
             }
 
-            function W(e) {
+            function Y(e) {
                 return e["workspace@"]
             }
 
-            function j(e) {
+            function z(e) {
                 return e.notebooks
             }
 
-            function H(e) {
-                return new V(e)
+            function K(e) {
+                return new H(e)
             }
 
-            function X(e, t) {
+            function Z(e, t) {
                 e["blocksRendered@"] = t
             }
 
-            function Y(e) {
+            function J(e) {
                 return e["blocksRendered@"]
             }
 
-            function z(e) {
+            function q(e) {
                 return e["notHooked@"]
             }
 
-            function K(e, t) {
+            function Q(e, t) {
                 e["notHooked@"] = t
             }
 
-            function Z(e) {
+            function $(e) {
                 return e["lastCell@"]
             }
 
-            function q(e, t) {
+            function ee(e, t) {
                 e["lastCell@"] = t
             }
 
-            function J(e) {
-                return (e, t) => (e.name.indexOf("python") >= 0 && "execute_input" === t.header.msg_type.toString() && (console.log("jupyterlab_blockly_extension_python: kernel executed code, updating intellisense"), P()), !0)
+            function te(e) {
+                return (e, t) => {
+                    if (e.name.indexOf("python") >= 0) switch (t.header.msg_type.toString()) {
+                        case "execute_input":
+                            console.log("jupyterlab_blockly_extension_python: kernel executed code, updating intellisense"), j(V("execute-code", t.content)), B();
+                            break;
+                        case "error":
+                            j(V("execute-code-error", t.content))
+                    }
+                    return !0
+                }
             }
 
-            function Q(e) {
+            function ne(e) {
                 return (t, n) => {
                     if (n) {
+                        j(V("active-cell-change", {
+                            cell_text: n.node.outerText
+                        }));
                         const t = document.getElementById("syncCheckboxPython"),
                             o = document.getElementById("autosaveCheckboxPython"),
                             l = e => !!e && e.checked;
-                        l(t) && e.notebooks.activeCell && (Y(e) && null == $(e) ? oe() : te(e), P()), l(o) && e.notebooks.activeCell && (ne(e), q(e, n))
+                        l(t) && e.notebooks.activeCell && (J(e) && null == oe(e) ? se() : ie(e), B()), l(o) && e.notebooks.activeCell && (ae(e), ee(e, n))
                     }
                     return !0
                 }
             }
 
-            function $(e) {
+            function oe(e) {
                 if (e.notebooks.activeCell) {
                     const t = e.notebooks.activeCell.model.sharedModel.getSource();
                     if (!(t.indexOf("xmlns") >= 0)) return null;
                     {
                         const e = /(<xml[\s\S]+<\/xml>)/;
                         let n = t.match(e);
                         if (n && n[0]) return n[0]
                     }
                 }
                 return null
             }
 
-            function ee(e) {
+            function le(e) {
                 let t;
-                const n = e.generator.workspaceToCode(W(e));
-                e.notebooks.activeCell ? (t = e.notebooks.activeCell.model, i.isMarkdownCellModel(t) ? window.alert("You are calling 'Blocks to Code' on a MARKDOWN cell. Select an empty CODE cell and try again.") : (e.notebooks.activeCell.model.sharedModel.setSource(n + "\n#" + f()), console.log("jupyterlab_blockly_extension_python: wrote to active cell\n" + n + "\n"), X(e, !0))) : console.log("jupyterlab_blockly_extension_python: no cell active, flushed\n" + n + "\n")
+                const n = e.generator.workspaceToCode(Y(e));
+                e.notebooks.activeCell ? (t = e.notebooks.activeCell.model, i.isMarkdownCellModel(t) ? window.alert("You are calling 'Blocks to Code' on a MARKDOWN cell. Select an empty CODE cell and try again.") : (e.notebooks.activeCell.model.sharedModel.setSource(n + "\n#" + f()), console.log("jupyterlab_blockly_extension_python: wrote to active cell\n" + n + "\n"), j(V("blocks-to-code", {
+                    code: e.notebooks.activeCell.model.toJSON().source.toString()
+                })), Z(e, !0))) : console.log("jupyterlab_blockly_extension_python: no cell active, flushed\n" + n + "\n")
             }
 
-            function te(e) {
+            function ie(e) {
                 if (e.notebooks.activeCell) {
                     const t = /(<xml[\s\S]+<\/xml>)/;
                     let n = e.notebooks.activeCell.model.sharedModel.getSource().match(t);
                     try {
                         if (n && n[1]) {
                             const e = n[1];
-                            oe(),
+                            se(),
                                 function(e) {
                                     const t = (new DOMParser).parseFromString(e, "application/xml").documentElement;
                                     r.Xml.domToWorkspace(t, r.getMainWorkspace())
-                                }(e)
+                                }(e), j(V("xml-to-blocks", {
+                                    xml: e
+                                }))
                         }
                     } catch (e) {
                         window.alert("Unable to perform 'Code to Blocks': XML is either invald or renames existing variables. Specific error message is: " + e.message), console.log("jupyterlab_blockly_extension_python: unable to decode blocks, last line is invald xml")
                     }
                 } else console.log("jupyterlab_blockly_extension_python: unable to decode blocks, active cell is null")
             }
 
-            function ne(e) {
+            function ae(e) {
                 let t;
-                const n = e.generator.workspaceToCode(W(e));
-                Z(e) ? Z(e).model && (t = Z(e).model, i.isCodeCellModel(t) && (() => {
+                const n = e.generator.workspaceToCode(Y(e));
+                $(e) ? $(e).model && (t = $(e).model, i.isCodeCellModel(t) && (() => {
                     try {
-                        const t = Z(e).model.sharedModel.getSource();
+                        const t = $(e).model.sharedModel.getSource();
                         if (t.indexOf("xmlns") >= 0) {
                             const e = /(<xml[\s\S]+<\/xml>)/;
                             let n = t.match(e);
                             if (n && n[0]) return n[0]
                         }
                     } catch (e) {
                         return !1
                     }
-                })()) && W(e).getAllBlocks(!1).length > 0 && (Z(e).model.sharedModel.setSource(n + "\n#" + f()), console.log("jupyterlab_blockly_extension_python: wrote to active cell\n" + n + "\n")) : console.log("jupyterlab_blockly_extension_python: no cell active, flushed instead of autosave\n" + n + "\n")
+                })()) && Y(e).getAllBlocks(!1).length > 0 && ($(e).model.sharedModel.setSource(n + "\n#" + f()), console.log("jupyterlab_blockly_extension_python: wrote to active cell\n" + n + "\n"), e.notebooks.activeCell && j(V("blocks-to-code-autosave", e.notebooks.activeCell.model.toJSON()))) : console.log("jupyterlab_blockly_extension_python: no cell active, flushed instead of autosave\n" + n + "\n")
             }
 
-            function oe(e) {
+            function se(e) {
                 const t = r.getMainWorkspace().getAllBlocks(!1);
                 for (let e = 0; e < t.length; e++) t[e].dispose(!1)
             }
 
-            function le(e, t, n) {
+            function re(e, t, n) {
                 if (!n.isAttached) {
                     const o = t.currentWidget;
                     if (null == o) e.shell.add(n, "main");
                     else {
                         const e = o,
                             t = {
                                 ref: e.id,
@@ -753,72 +801,84 @@
                             };
                         e.context.addSibling(n, t)
                     }
                 }
                 e.shell.activateById(n.id)
             }
 
-            function ie(e) {
+            function ce(e) {
                 const t = new l.MainAreaWidget({
                     content: e
                 });
                 return t.id = "blockly-jupyterlab-python", t.title.label = "Blockly Python", t.title.closable = !0, t
             }
 
-            function ae(e, t) {
+            function ue(e, t) {
                 var n;
                 const o = this;
-                if (z(o)) {
+                if (q(o)) {
                     const t = null === (n = e.session) || void 0 === n ? void 0 : n.kernel;
                     if (null == t || null == t);
                     else {
                         const e = t;
-                        e.name.indexOf("python") >= 0 && (e.iopubMessage.connect(J(), o), console.log("jupyterlab_blockly_extension_python: Listening for kernel messages"), K(o, !1))
+                        e.name.indexOf("python") >= 0 && (e.iopubMessage.connect(te(), o), console.log("jupyterlab_blockly_extension_python: Listening for kernel messages"), Q(o, !1))
                     }
                     return !0
                 }
                 return !1
             }
 
-            function se(e, t) {
+            function de(e, t) {
                 const n = this,
                     o = e.currentWidget;
                 if (null == o);
                 else {
                     const e = o;
-                    console.log("jupyterlab_blockly_extension_python: notebook changed to " + e.context.path), e.sessionContext.kernelChanged.connect(ae, n)
+                    console.log("jupyterlab_blockly_extension_python: notebook changed to " + e.context.path), j(V("notebook-changed", {
+                        path: e.context.path
+                    })), e.sessionContext.kernelChanged.connect(ue, n)
                 }
                 return !0
             }
-            const re = (e, t, n) => {
-                    const o = e;
-                    return null == t.currentWidget || (console.log("jupyterlab_blockly_extension_python: notebook changed, autorunning blockly python command"), o.commands.execute("blockly_python:open")), !0
-                },
-                ce = {
-                    id: "jupyterlab-apod",
-                    description: "blockly extension for jupyter lab.",
-                    autoStart: !0,
-                    requires: [l.ICommandPalette, s.INotebookTracker, o.ILayoutRestorer],
-                    activate: async function(e, t, n, o, i) {
-                        console.log("jupyterlab_blockly_extension_python: extension is activated!");
-                        const a = H(n);
-                        let s = ie(a);
-                        const r = new l.WidgetTracker({
-                            namespace: "blockly_python"
-                        });
-                        o && o.restore(r, {
-                            command: "blockly_python:open",
-                            name: () => "blockly_python"
-                        }), n.currentChanged.connect(se, a), e.commands.addCommand("blockly_python:open", {
-                            label: "Blockly Python",
-                            execute: () => {
-                                s && !s.isDisposed || (s = ie(a)), le(e, n, s), r.has(s) || r.add(s)
-                            }
-                        }), t.addItem({
-                            command: "blockly_python:open",
-                            category: "Blockly"
-                        })
-                    }
+
+            function he(e, t) {
+                return null == e.currentWidget || (console.log("jupyterlab_blockly_extension_python: notebook changed, autorunning blockly python command"), this.commands.execute("blockly_python:open")), !0
+            }
+            const pe = {
+                id: "jupyterlab-apod",
+                description: "blockly python extension for jupyter lab.",
+                autoStart: !0,
+                requires: [l.ICommandPalette, s.INotebookTracker, o.ILayoutRestorer],
+                activate: async function(e, t, n, o, i) {
+                    console.log("jupyterlab_blockly_extension_python: extension is activated!");
+                    const a = K(n);
+                    let s = ce(a);
+                    const r = new l.WidgetTracker({
+                        namespace: "blockly_python"
+                    });
+                    o && o.restore(r, {
+                        command: "blockly_python:open",
+                        name: () => "blockly_python"
+                    }), n.currentChanged.connect(de, a), e.commands.addCommand("blockly_python:open", {
+                        label: "Blockly Python",
+                        execute: () => {
+                            s && !s.isDisposed || (s = ce(a)), re(e, n, s), r.has(s) || r.add(s)
+                        }
+                    }), t.addItem({
+                        command: "blockly_python:open",
+                        category: "Blockly"
+                    });
+                    const c = new URLSearchParams(window.location.search);
+                    "py" === c.get("bl") && (console.log("jupyterlab_blockly_extension_python: openning blockly, bl=py"), e.restored.then((() => {
+                        n.currentChanged.connect(he, e), s.title.closable = !1
+                    })));
+                    let u = c.get("id");
+                    u && (function(e) {
+                        W = e
+                    }(u), console.log("jupyterlab_blockly_extension_py: using id=" + u + " for logging"));
+                    let d = c.get("log");
+                    d && (G = d, console.log("jupyterlab_blockly_extension_py: using log=" + d + " for logging"))
                 }
+            }
         }
     }
 ]);
```

### Comparing `aolney_jupyterlab_blockly_python_extension-0.1.0/aolney_jupyterlab_blockly_python_extension/labextension/static/88.f12ddff976fd53bc3a6c.js` & `aolney_jupyterlab_blockly_python_extension-0.1.1/aolney_jupyterlab_blockly_python_extension/labextension/static/88.f12ddff976fd53bc3a6c.js`

 * *Files identical despite different names*

### Comparing `aolney_jupyterlab_blockly_python_extension-0.1.0/aolney_jupyterlab_blockly_python_extension/labextension/static/remoteEntry.8cc4b66a67cd4b700f08.js` & `aolney_jupyterlab_blockly_python_extension-0.1.1/aolney_jupyterlab_blockly_python_extension/labextension/static/remoteEntry.49e44ba8d7266e1def33.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -1,15 +1,15 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, o, a, i, l, u, s, f, d, c, p, h, b, v, y, m, g, w, j, k, S, x = {
+    var e, r, t, n, o, a, i, l, u, s, f, d, p, c, h, b, v, y, m, g, w, j, k, S, x = {
             459: (e, r, t) => {
                 var n = {
-                        "./index": () => Promise.all([t.e(88), t.e(203), t.e(788)]).then((() => () => t(788))),
-                        "./extension": () => Promise.all([t.e(88), t.e(203), t.e(788)]).then((() => () => t(788))),
+                        "./index": () => Promise.all([t.e(88), t.e(203), t.e(603)]).then((() => () => t(603))),
+                        "./extension": () => Promise.all([t.e(88), t.e(203), t.e(603)]).then((() => () => t(603))),
                         "./style": () => t.e(728).then((() => () => t(728)))
                     },
                     o = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
                     a = (e, r) => {
                         if (t.S) {
@@ -46,22 +46,22 @@
             enumerable: !0,
             get: r[t]
         })
     }, P.f = {}, P.e = e => Promise.all(Object.keys(P.f).reduce(((r, t) => (P.f[t](e, r), r)), [])), P.u = e => e + "." + {
         88: "f12ddff976fd53bc3a6c",
         203: "1521356dd3eabef73aae",
         369: "5f4ab4479184dd6b56b7",
-        728: "ea6e1ffef3f6bcb3b003",
-        788: "ac8ed33ecdaba7af1017"
+        603: "4a974815d784d1ce9ced",
+        728: "ea6e1ffef3f6bcb3b003"
     } [e] + ".js?v=" + {
         88: "f12ddff976fd53bc3a6c",
         203: "1521356dd3eabef73aae",
         369: "5f4ab4479184dd6b56b7",
-        728: "ea6e1ffef3f6bcb3b003",
-        788: "ac8ed33ecdaba7af1017"
+        603: "4a974815d784d1ce9ced",
+        728: "ea6e1ffef3f6bcb3b003"
     } [e], P.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
@@ -75,19 +75,19 @@
                     if (f.getAttribute("src") == t || f.getAttribute("data-webpack") == r + o) {
                         i = f;
                         break
                     }
                 }
             i || (l = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, P.nc && i.setAttribute("nonce", P.nc), i.setAttribute("data-webpack", r + o), i.src = t), e[t] = [n];
             var d = (r, n) => {
-                    i.onerror = i.onload = null, clearTimeout(c);
+                    i.onerror = i.onload = null, clearTimeout(p);
                     var o = e[t];
                     if (delete e[t], i.parentNode && i.parentNode.removeChild(i), o && o.forEach((e => e(n))), r) return r(n)
                 },
-                c = setTimeout(d.bind(null, void 0, {
+                p = setTimeout(d.bind(null, void 0, {
                     type: "timeout",
                     target: i
                 }), 12e4);
             i.onerror = d.bind(null, i.onerror), i.onload = d.bind(null, i.onload), l && document.head.appendChild(i)
         }
     }, P.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
@@ -113,15 +113,15 @@
                         (!l || !l.loaded && (!n != !l.eager ? n : i > l.from)) && (o[r] = {
                             get: t,
                             from: i,
                             eager: !!n
                         })
                     },
                     u = [];
-                return "default" === t && (l("@aolney/jupyterlab-blockly-python-extension", "0.1.0", (() => Promise.all([P.e(88), P.e(203), P.e(788)]).then((() => () => P(788))))), l("blockly", "10.4.3", (() => Promise.all([P.e(88), P.e(369)]).then((() => () => P(369)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                return "default" === t && (l("@aolney/jupyterlab-blockly-python-extension", "0.1.1", (() => Promise.all([P.e(88), P.e(203), P.e(603)]).then((() => () => P(603))))), l("blockly", "10.4.3", (() => Promise.all([P.e(88), P.e(369)]).then((() => () => P(369)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         P.g.importScripts && (e = P.g.location + "");
         var r = P.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -192,60 +192,60 @@
                     u = !1, l--
                 } else {
                     if (l <= n || f < d != o) return !1;
                     u = !1
                 } else "s" != d && "n" != d && (u = !1, l--)
             }
         }
-        var c = [],
-            p = c.pop.bind(c);
+        var p = [],
+            c = p.pop.bind(p);
         for (i = 1; i < e.length; i++) {
             var h = e[i];
-            c.push(1 == h ? p() | p() : 2 == h ? p() & p() : h ? a(h, r) : !p())
+            p.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? a(h, r) : !c())
         }
-        return !!p()
+        return !!c()
     }, i = (e, r) => {
         var t = P.S[e];
         if (!t || !P.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, l = (e, r) => {
         var t = e[r];
         return (r = Object.keys(t).reduce(((e, r) => !e || n(e, r) ? r : e), 0)) && t[r]
     }, u = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
     }, s = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(n) + ")", f = (e, r, t, n) => {
         var o = u(e, t);
-        return a(n, o) || p(s(e, t, o, n)), b(e[t][o])
+        return a(n, o) || c(s(e, t, o, n)), b(e[t][o])
     }, d = (e, r, t) => {
         var o = e[r];
         return (r = Object.keys(o).reduce(((e, r) => !a(t, r) || e && !n(e, r) ? e : r), 0)) && o[r]
-    }, c = (e, r, t, n) => {
+    }, p = (e, r, t, n) => {
         var a = e[t];
         return "No satisfying version (" + o(n) + ") of shared module " + t + " found in shared scope " + r + ".\nAvailable versions: " + Object.keys(a).map((e => e + " from " + a[e].from)).join(", ")
-    }, p = e => {
+    }, c = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
     }, h = (e, r, t, n) => {
-        p(c(e, r, t, n))
+        c(p(e, r, t, n))
     }, b = e => (e.loaded = 1, e.get()), y = (v = e => function(r, t, n, o) {
         var a = P.I(r);
         return a && a.then ? a.then(e.bind(e, r, P.S[r], t, n, o)) : e(r, P.S[r], t, n, o)
     })(((e, r, t, n) => (i(e, t), b(d(r, t, n) || h(r, e, t, n) || l(r, t))))), m = v(((e, r, t, n) => (i(e, t), f(r, 0, t, n)))), g = v(((e, r, t, n, o) => {
         var a = r && P.o(r, t) && d(r, t, n);
         return a ? b(a) : o()
     })), w = {}, j = {
+        206: () => y("default", "@jupyterlab/cells", [1, 4, 2, 0]),
+        236: () => m("default", "@jupyterlab/rendermime", [1, 4, 2, 0]),
         256: () => m("default", "@lumino/widgets", [1, 2, 3, 1, , "alpha", 0]),
-        315: () => y("default", "@jupyterlab/cells", [1, 4, 1, 6]),
-        372: () => m("default", "@jupyterlab/notebook", [1, 4, 1, 6]),
-        465: () => m("default", "@jupyterlab/application", [1, 4, 1, 6]),
+        291: () => m("default", "@jupyterlab/notebook", [1, 4, 2, 0]),
         569: () => g("default", "blockly", [1, 10, 4, 3], (() => P.e(369).then((() => () => P(369))))),
-        638: () => m("default", "@jupyterlab/apputils", [1, 4, 2, 6]),
-        723: () => m("default", "@jupyterlab/rendermime", [1, 4, 1, 6])
+        626: () => m("default", "@jupyterlab/application", [1, 4, 2, 0]),
+        923: () => m("default", "@jupyterlab/apputils", [1, 4, 3, 0])
     }, k = {
-        788: [256, 315, 372, 465, 569, 638, 723]
+        603: [206, 236, 256, 291, 569, 626, 923]
     }, S = {}, P.f.consumes = (e, r) => {
         P.o(k, e) && k[e].forEach((e => {
             if (P.o(w, e)) return r.push(w[e]);
             if (!S[e]) {
                 var t = r => {
                     w[e] = 0, P.m[e] = t => {
                         delete P.c[e], t.exports = r()
```

### Comparing `aolney_jupyterlab_blockly_python_extension-0.1.0/aolney_jupyterlab_blockly_python_extension/labextension/static/third-party-licenses.json` & `aolney_jupyterlab_blockly_python_extension-0.1.1/aolney_jupyterlab_blockly_python_extension/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `aolney_jupyterlab_blockly_python_extension-0.1.0/src/SearchDropdown.ts` & `aolney_jupyterlab_blockly_python_extension-0.1.1/src/SearchDropdown.ts`

 * *Files identical despite different names*

### Comparing `aolney_jupyterlab_blockly_python_extension-0.1.0/src/field_minus.ts` & `aolney_jupyterlab_blockly_python_extension-0.1.1/src/field_minus.ts`

 * *Files identical despite different names*

### Comparing `aolney_jupyterlab_blockly_python_extension-0.1.0/src/field_plus.ts` & `aolney_jupyterlab_blockly_python_extension-0.1.1/src/field_plus.ts`

 * *Files identical despite different names*

### Comparing `aolney_jupyterlab_blockly_python_extension-0.1.0/src/index.ts` & `aolney_jupyterlab_blockly_python_extension-0.1.1/src/index.ts`

 * *Files 12% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 import { DocumentRegistry } from "@jupyterlab/docregistry";
 import { Kernel, KernelMessage, Session } from "@jupyterlab/services"
 import { toolbox, encodeWorkspace, decodeWorkspace, UpdateAllIntellisense_Python, setNotebooksInstance as notebooks_1 } from './toolbox';
 import * as Blockly from 'blockly/core';
 import * as libraryBlocks from 'blockly/blocks';
 import { pythonGenerator } from 'blockly/python';
 import * as En from 'blockly/msg/en';
+import * as Logging from './logging'
+
 Blockly.setLocale(En);
 
 class BlocklyWidget extends Widget {
   readonly notebooks: INotebookTracker;
   readonly generator: typeof pythonGenerator;
   "lastCell@": Cell;
   "blocksRendered@": boolean;
@@ -90,14 +92,15 @@
       if (e.type === "create") {
           BlocklyWidget__set_blocksRendered_Z1FBCCD16(this$, false);
       }
       if (e.type === "finished_loading") {
           BlocklyWidget__set_blocksRendered_Z1FBCCD16(this$, true);
       }
       //LogToServer(BlocklyLogEntry082720_Create<Blockly.Events.BlockBase>(e.type, e));
+      Logging.LogToServer(Logging.createBlocklyLogEntry(e.type, e.toJson()));
     }
     BlocklyWidget__get_workspace(this$).removeChangeListener(logListener);
     BlocklyWidget__get_workspace(this$).addChangeListener(logListener);
   }
   onResize = (msg: Widget.ResizeMessage): void => {
     let copyOfStruct: number = msg.width;
     let copyOfStruct_1: number = msg.width;
@@ -158,32 +161,36 @@
   return (sender: Kernel.IKernelConnection, args: KernelMessage.IIOPubMessage<any>): boolean => {
     if (sender.name.indexOf("python") >= 0) {
       const messageType: string = args.header.msg_type.toString();
       switch (messageType) {
         case "execute_input": {
           console.log("jupyterlab_blockly_extension_python: kernel executed code, updating intellisense");
           // LogToServer(JupyterLogEntry082720_Create("execute-code", args.content.code));
+          //TODO: make sure code is getting logged here
+          Logging.LogToServer(Logging.createJupyterLogEntry("execute-code", args.content ));
           UpdateAllIntellisense_Python();
           break;
         }
         case "error": {
           // LogToServer(JupyterLogEntry082720_Create("execute-code-error", JSON.stringify(args.content)));
+          Logging.LogToServer(Logging.createJupyterLogEntry("execute-code-error", args.content ));
           break;
         }
         default: 0;
       }
     }
     return true;
   };
 };
 
 export function BlocklyWidget__get_onActiveCellChanged(this$: BlocklyWidget): (arg0: INotebookTracker, arg1: Cell<ICellModel> | null) => boolean {
   return (sender: INotebookTracker, args: Cell<ICellModel> | null): boolean => {
     if(args){
       // LogToServer(JupyterLogEntry082720_Create("active-cell-change", args.node.outerText));
+      Logging.LogToServer(Logging.createJupyterLogEntry("active-cell-change", { cell_text : args.node.outerText} ));
       const syncCheckbox: HTMLElement | null = document.getElementById("syncCheckboxPython");
       const autosaveCheckbox: HTMLElement | null = document.getElementById("autosaveCheckboxPython");
 
       const isChecked = (aCheckbox: any): boolean => {
         if (aCheckbox) {
           return aCheckbox.checked;
         }
@@ -239,14 +246,16 @@
     if ((model = this$.notebooks.activeCell.model, cells.isMarkdownCellModel(model))) {
       window.alert("You are calling \'Blocks to Code\' on a MARKDOWN cell. Select an empty CODE cell and try again.");
     }
     else {
       this$.notebooks.activeCell.model.sharedModel.setSource(code + "\n#" + encodeWorkspace());
       console.log(("jupyterlab_blockly_extension_python: wrote to active cell\n" + code) + "\n");
       // LogToServer(JupyterLogEntry082720_Create("blocks-to-code", this$.notebooks.activeCell.model.value.text));
+      // TODO check this is logging correctly
+      Logging.LogToServer(Logging.createJupyterLogEntry("blocks-to-code", { code: this$.notebooks.activeCell.model.toJSON().source.toString() } ));
       BlocklyWidget__set_blocksRendered_Z1FBCCD16(this$, true);
     }
   }
   else {
     console.log(("jupyterlab_blockly_extension_python: no cell active, flushed\n" + code) + "\n");
   }
 
@@ -262,14 +271,15 @@
     let xmlStringOption = xmlString.match(regex);
     try {
       if(xmlStringOption && xmlStringOption[1]){
         const xmlString: string = xmlStringOption[1];
         BlocklyWidget__clearBlocks(this$);
         decodeWorkspace(xmlString);
         // LogToServer(JupyterLogEntry082720_Create("xml-to-blocks", xmlString));
+        Logging.LogToServer(Logging.createJupyterLogEntry("xml-to-blocks", { xml: xmlString }));
       }
     } catch (e: any) {
       window.alert("Unable to perform \'Code to Blocks\': XML is either invald or renames existing variables. Specific error message is: " + e.message);
       console.log("jupyterlab_blockly_extension_python: unable to decode blocks, last line is invald xml");
     }
   }
   else {
@@ -303,14 +313,18 @@
         })()) {
           // const workspace: Blockly.Workspace = BlocklyWidget__get_workspace(this$);
           const blocks: Blockly.Block[] = BlocklyWidget__get_workspace(this$).getAllBlocks(false);
           if (blocks.length > 0) {
             BlocklyWidget__get_lastCell(this$).model.sharedModel.setSource(code + "\n#" + encodeWorkspace());
             console.log(("jupyterlab_blockly_extension_python: wrote to active cell\n" + code) + "\n");
             // LogToServer(JupyterLogEntry082720_Create("blocks-to-code-autosave", this$.notebooks.activeCell.model.value.text));
+            if(this$.notebooks.activeCell) {
+              // TODO check if logging correctly
+              Logging.LogToServer(Logging.createJupyterLogEntry("blocks-to-code-autosave", this$.notebooks.activeCell.model.toJSON() ));
+            }
           }
         }
       }
     }
   }
   else {
     console.log(("jupyterlab_blockly_extension_python: no cell active, flushed instead of autosave\n" + code) + "\n");
@@ -385,21 +399,22 @@
   const blocklyWidget: BlocklyWidget = this;
   const matchValue: NotebookPanel | null = sender.currentWidget;
   if (matchValue == null) {}
   else {
     const notebook: NotebookPanel = matchValue;
     console.log("jupyterlab_blockly_extension_python: notebook changed to " + notebook.context.path);
     // LogToServer(JupyterLogEntry082720_Create("notebook-changed", notebook.context.path));
+    Logging.LogToServer(Logging.createJupyterLogEntry("notebook-changed", { path: notebook.context.path }));
     notebook.sessionContext.kernelChanged.connect(onKernelChanged, blocklyWidget);
   }
   return true;
 };
 
-export const runCommandOnNotebookChanged = (app: JupyterFrontEnd, sender: IWidgetTracker<NotebookPanel>, args: NotebookPanel | null): boolean => {
-  const appContext = app;  
+export function runCommandOnNotebookChanged (this: any, sender: IWidgetTracker<NotebookPanel>, args: NotebookPanel | null): boolean  {
+  const appContext = this;  
   const matchValue = sender.currentWidget;
   if (matchValue == null) {}
   else {
     console.log("jupyterlab_blockly_extension_python: notebook changed, autorunning blockly python command");
     appContext.commands.execute("blockly_python:open");
   }
   return true;
@@ -438,19 +453,40 @@
   } as CommandRegistry.ICommandOptions);
 
   palette.addItem({
     command: "blockly_python:open",
     category: "Blockly",
   });
 
+  // process query string parameters
+  const searchParams: any = new URLSearchParams(window.location.search);
+  if( searchParams.get("bl") === "py") {
+    console.log("jupyterlab_blockly_extension_python: openning blockly, bl=py");
+    app.restored.then<void>((): void => {
+      notebooks.currentChanged.connect(runCommandOnNotebookChanged, app);
+      widget.title.closable = false;
+    });
+  }
+
+  let id = searchParams.get("id")
+  if( id ) {
+    Logging.set_id( id );
+    console.log( "jupyterlab_blockly_extension_py: using id=" + id + " for logging" ) ;
+  }
+
+  let log_url = searchParams.get("log") 
+  if( log_url ) {
+    Logging.set_log_url( log_url );
+    console.log( "jupyterlab_blockly_extension_py: using log=" + log_url + " for logging" ) ;
+  }
 
 };
 
 const plugin: JupyterFrontEndPlugin<void> = {
   id: 'jupyterlab-apod',
-  description: 'blockly extension for jupyter lab.',
+  description: 'blockly python extension for jupyter lab.',
   autoStart: true,
   requires: [ICommandPalette, INotebookTracker, ILayoutRestorer],
   activate: activate
 };
 
 export default plugin;
```

### Comparing `aolney_jupyterlab_blockly_python_extension-0.1.0/src/logging.ts` & `aolney_jupyterlab_blockly_python_extension-0.1.1/src/logging.ts`

 * *Files 23% similar despite different names*

```diff
@@ -1,49 +1,82 @@
 export interface LogEntry {
     username: string;
     json: string;
   }
   
-  export interface BlocklyLogEntry {
+  export interface BlocklyLogEntry050824 {
     schema: string;
     name: string;
     object: any;
   }
   
-  export interface JupyterLogEntry {
+  export interface JupyterLogEntry050824 {
     schema: string;
     name: string;
-    payload?: string | null;
+    // payload?: string | null;
+    payload: object;
   }
   
-  export function createBlocklyLogEntry(name: string, object: any): BlocklyLogEntry {
+  export function createBlocklyLogEntry(name: string, object: any): BlocklyLogEntry050824 {
+    // let encoded_object = btoa(object);
+    // // DEBUG
+    // encoded_object = (object);
     return {
-      schema: "ble082720",
+      schema: "ble050824",
       name: name,
       object: object
     };
   }
   
-  export function createJupyterLogEntry(name: string, payload: string | null): JupyterLogEntry {
+  export function createJupyterLogEntry(name: string, payload: object): JupyterLogEntry050824 {
+    // let encoded_payload = "";
+    // if( payload ) { 
+    //   // DEBUG
+    //   encoded_payload = payload; //btoa(payload); 
+    // }
     return {
-      schema: "jle082720",
+      schema: "jle050824",
       name: name,
       payload: payload
     };
   }
   
-  export let logUrl: string | undefined = undefined;
-  export let idOption: string | undefined = undefined;
+  let logUrl: string | undefined = undefined;
+  export function set_log_url( url: string) {
+    logUrl = url;
+  }
+  let idOption: string | undefined = undefined;
+  export function set_id( id: string) {
+    idOption = id;
+  }
   
-  export function filterJson<T>(o: any): T {
+  export function filterJson(o: any): string {
     if (o?.object?.element?.toString().indexOf("drag") === 0) {
       o.object.newValue = undefined;
       o.object.oldValue = undefined;
     }
-    throw 1;
+    return o; //JSON.stringify(o);
   }
   
   
   export function LogToServer(logObject: any): void {
-    
-  
+    if(logUrl) {
+      let id =  window.location.href;
+      if( idOption ) { id = idOption; }
+      window.fetch(logUrl, {
+        method: "POST",
+        headers: {
+          "Content-Type": "application/json",
+        },
+        body: JSON.stringify({
+          username:id,
+          //TODO btoa(json)
+          json:filterJson(logObject) 
+          
+        })
+      }).then(response => {
+        if (!response.ok) {
+          console.log(response.statusText);
+        }
+      })
+    }
   }
```

### Comparing `aolney_jupyterlab_blockly_python_extension-0.1.0/src/toolbox.ts` & `aolney_jupyterlab_blockly_python_extension-0.1.1/src/toolbox.ts`

 * *Files identical despite different names*

### Comparing `aolney_jupyterlab_blockly_python_extension-0.1.0/ui-tests/README.md` & `aolney_jupyterlab_blockly_python_extension-0.1.1/ui-tests/README.md`

 * *Files identical despite different names*

### Comparing `aolney_jupyterlab_blockly_python_extension-0.1.0/ui-tests/tests/aolney_jupyterlab_blockly_python_extension.spec.ts` & `aolney_jupyterlab_blockly_python_extension-0.1.1/ui-tests/tests/aolney_jupyterlab_blockly_python_extension.spec.ts`

 * *Files identical despite different names*

### Comparing `aolney_jupyterlab_blockly_python_extension-0.1.0/.gitignore` & `aolney_jupyterlab_blockly_python_extension-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `aolney_jupyterlab_blockly_python_extension-0.1.0/LICENSE` & `aolney_jupyterlab_blockly_python_extension-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aolney_jupyterlab_blockly_python_extension-0.1.0/README.md` & `aolney_jupyterlab_blockly_python_extension-0.1.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,18 @@
 The following query string parameters enable functionality:
 
 - bl=py forces the extension to display on load (it is already active)
 - log=xxx specifies a url for a logging endpoint (e.g. https://yourdomain.com/log)
 - id=xxx adds an identifier for logging
 
 
+> [!WARNING]  
+> Currently there appears to be a conflict between the Python and R extensions, so we recommend that only one be installed at a time.
+> Additionally the current version of nbgitpuller is removing the query strings above before they can be processed.
+
 ## Requirements
 
 - JupyterLab >= 4.0.0
 
 *An earlier version targets JupyterLab 1.2x. You can find that version on [npm](https://www.npmjs.com/package/@aolney/jupyterlab-blockly-python-extension) and in the commit history of this repository ([final tag](https://github.com/aolney/jupyterlab-blockly-python-extension/releases/tag/0.5.6))*
 
 ## Install
```

### Comparing `aolney_jupyterlab_blockly_python_extension-0.1.0/pyproject.toml` & `aolney_jupyterlab_blockly_python_extension-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aolney_jupyterlab_blockly_python_extension-0.1.0/PKG-INFO` & `aolney_jupyterlab_blockly_python_extension-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: aolney_jupyterlab_blockly_python_extension
-Version: 0.1.0
+Version: 0.1.1
 Dynamic: Keywords
 Summary: A JupyterLab extension that creates a Blockly palette for Python.
 Project-URL: Homepage, https://github.com/aolney/jupyterlab-blockly-python-extension
 Project-URL: Bug Tracker, https://github.com/aolney/jupyterlab-blockly-python-extension/issues
 Project-URL: Repository, https://github.com/aolney/jupyterlab-blockly-python-extension.git
 Author-email: "Andrew M. Olney" <aolney@memphis.edu>
 License:                                  Apache License
@@ -235,14 +235,18 @@
 The following query string parameters enable functionality:
 
 - bl=py forces the extension to display on load (it is already active)
 - log=xxx specifies a url for a logging endpoint (e.g. https://yourdomain.com/log)
 - id=xxx adds an identifier for logging
 
 
+> [!WARNING]  
+> Currently there appears to be a conflict between the Python and R extensions, so we recommend that only one be installed at a time.
+> Additionally the current version of nbgitpuller is removing the query strings above before they can be processed.
+
 ## Requirements
 
 - JupyterLab >= 4.0.0
 
 *An earlier version targets JupyterLab 1.2x. You can find that version on [npm](https://www.npmjs.com/package/@aolney/jupyterlab-blockly-python-extension) and in the commit history of this repository ([final tag](https://github.com/aolney/jupyterlab-blockly-python-extension/releases/tag/0.5.6))*
 
 ## Install
```

