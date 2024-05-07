# Comparing `tmp/mkdocs_inline_svg_plugin-0.1.3.tar.gz` & `tmp/mkdocs_inline_svg_plugin-0.1.4.tar.gz`

## Comparing `mkdocs_inline_svg_plugin-0.1.3.tar` & `mkdocs_inline_svg_plugin-0.1.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 mkdocs_inline_svg_plugin-0.1.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 mkdocs_inline_svg_plugin-0.1.3/CHANGELOG.md
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 mkdocs_inline_svg_plugin-0.1.3/mkdocs.yml
--rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 mkdocs_inline_svg_plugin-0.1.3/.github/workflows/python-publish-test.yml
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 mkdocs_inline_svg_plugin-0.1.3/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 mkdocs_inline_svg_plugin-0.1.3/.github/workflows/python-test.yml
--rw-r--r--   0        0        0     7099 2020-02-02 00:00:00.000000 mkdocs_inline_svg_plugin-0.1.3/docs/index.md
--rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 mkdocs_inline_svg_plugin-0.1.3/docs/css/extra.css
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs_inline_svg_plugin-0.1.3/src/inline_svg/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 mkdocs_inline_svg_plugin-0.1.3/src/inline_svg/__version__.py
--rw-r--r--   0        0        0     1240 2020-02-02 00:00:00.000000 mkdocs_inline_svg_plugin-0.1.3/src/inline_svg/config.py
--rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 mkdocs_inline_svg_plugin-0.1.3/src/inline_svg/plugin.py
--rw-r--r--   0        0        0     6159 2020-02-02 00:00:00.000000 mkdocs_inline_svg_plugin-0.1.3/src/inline_svg/util.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 mkdocs_inline_svg_plugin-0.1.3/tests/__init__.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 mkdocs_inline_svg_plugin-0.1.3/.gitignore
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 mkdocs_inline_svg_plugin-0.1.3/LICENSE.txt
--rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 mkdocs_inline_svg_plugin-0.1.3/README.md
--rw-r--r--   0        0        0     2874 2020-02-02 00:00:00.000000 mkdocs_inline_svg_plugin-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     2529 2020-02-02 00:00:00.000000 mkdocs_inline_svg_plugin-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 mkdocs_inline_svg_plugin-0.1.4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 mkdocs_inline_svg_plugin-0.1.4/CHANGELOG.md
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 mkdocs_inline_svg_plugin-0.1.4/mkdocs.yml
+-rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 mkdocs_inline_svg_plugin-0.1.4/.github/workflows/python-publish-test.yml
+-rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 mkdocs_inline_svg_plugin-0.1.4/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 mkdocs_inline_svg_plugin-0.1.4/.github/workflows/python-test.yml
+-rw-r--r--   0        0        0     7099 2020-02-02 00:00:00.000000 mkdocs_inline_svg_plugin-0.1.4/docs/index.md
+-rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 mkdocs_inline_svg_plugin-0.1.4/docs/css/extra.css
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs_inline_svg_plugin-0.1.4/src/inline_svg/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 mkdocs_inline_svg_plugin-0.1.4/src/inline_svg/__version__.py
+-rw-r--r--   0        0        0     1240 2020-02-02 00:00:00.000000 mkdocs_inline_svg_plugin-0.1.4/src/inline_svg/config.py
+-rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 mkdocs_inline_svg_plugin-0.1.4/src/inline_svg/plugin.py
+-rw-r--r--   0        0        0     6213 2020-02-02 00:00:00.000000 mkdocs_inline_svg_plugin-0.1.4/src/inline_svg/util.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 mkdocs_inline_svg_plugin-0.1.4/tests/__init__.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 mkdocs_inline_svg_plugin-0.1.4/.gitignore
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 mkdocs_inline_svg_plugin-0.1.4/LICENSE.txt
+-rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 mkdocs_inline_svg_plugin-0.1.4/README.md
+-rw-r--r--   0        0        0     2874 2020-02-02 00:00:00.000000 mkdocs_inline_svg_plugin-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     2529 2020-02-02 00:00:00.000000 mkdocs_inline_svg_plugin-0.1.4/PKG-INFO
```

### Comparing `mkdocs_inline_svg_plugin-0.1.3/.pre-commit-config.yaml` & `mkdocs_inline_svg_plugin-0.1.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `mkdocs_inline_svg_plugin-0.1.3/mkdocs.yml` & `mkdocs_inline_svg_plugin-0.1.4/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `mkdocs_inline_svg_plugin-0.1.3/.github/workflows/python-publish-test.yml` & `mkdocs_inline_svg_plugin-0.1.4/.github/workflows/python-publish-test.yml`

 * *Files identical despite different names*

### Comparing `mkdocs_inline_svg_plugin-0.1.3/.github/workflows/python-publish.yml` & `mkdocs_inline_svg_plugin-0.1.4/.github/workflows/python-publish.yml`

 * *Files 11% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         - name: Install Hatch
           run: pip install --upgrade hatch
 
         - name: Build package
           run: hatch build
 
         - name: Gather changes
-          run: sed -n '/^## '"${{ env.GITHUB_REF_NAME }}"'/,/^## .*/p' CHANGELOG.md > RELEASE_NOTES.md
+          run: sed -n '/^## '"${{ github.ref_name }}"'/,/^## .*/{/^## .*/d;p;}' CHANGELOG.md > RELEASE_NOTES.md
 
         - name: Create Release
           uses: softprops/action-gh-release@9d7c94cfd0a1f3ed45544c887983e9fa900f0564
                 # softprops/action-gh-release@v2
           with:
             body_path: RELEASE_NOTES.md
```

### Comparing `mkdocs_inline_svg_plugin-0.1.3/.github/workflows/python-test.yml` & `mkdocs_inline_svg_plugin-0.1.4/.github/workflows/python-test.yml`

 * *Files identical despite different names*

### Comparing `mkdocs_inline_svg_plugin-0.1.3/docs/index.md` & `mkdocs_inline_svg_plugin-0.1.4/docs/index.md`

 * *Files identical despite different names*

### Comparing `mkdocs_inline_svg_plugin-0.1.3/docs/css/extra.css` & `mkdocs_inline_svg_plugin-0.1.4/docs/css/extra.css`

 * *Files identical despite different names*

### Comparing `mkdocs_inline_svg_plugin-0.1.3/src/inline_svg/config.py` & `mkdocs_inline_svg_plugin-0.1.4/src/inline_svg/config.py`

 * *Files identical despite different names*

### Comparing `mkdocs_inline_svg_plugin-0.1.3/src/inline_svg/plugin.py` & `mkdocs_inline_svg_plugin-0.1.4/src/inline_svg/plugin.py`

 * *Files identical despite different names*

### Comparing `mkdocs_inline_svg_plugin-0.1.3/src/inline_svg/util.py` & `mkdocs_inline_svg_plugin-0.1.4/src/inline_svg/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,15 +77,17 @@
                 element.attrs["style"] = element.attrs["style"].replace(color, replacement)
 
         if element.name == "text" and "fill" not in element.attrs:
             element.attrs["fill"] = "var(--md-default-fg-color)"
 
 
 def _get_local_file_from_url(url: str, files: MkDocsFiles, config: InlineSvgConfig) -> MkDocsFile | None:
-    return files.get_file_from_path(url.removeprefix(config.site_url))
+    if config.site_url is not None:
+        url = url.removeprefix(config.site_url)
+    return files.get_file_from_path(url)
 
 
 def get_svg_data(url: str, files: MkDocsFiles, config: InlineSvgConfig) -> str | None:
     static_file = _get_local_file_from_url(url, files, config)
     log.debug("_get_local_file_from_url(url, files, config): %s", static_file)
     if static_file:
         with open(static_file.abs_src_path) as file:
```

### Comparing `mkdocs_inline_svg_plugin-0.1.3/.gitignore` & `mkdocs_inline_svg_plugin-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `mkdocs_inline_svg_plugin-0.1.3/LICENSE.txt` & `mkdocs_inline_svg_plugin-0.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mkdocs_inline_svg_plugin-0.1.3/README.md` & `mkdocs_inline_svg_plugin-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs_inline_svg_plugin-0.1.3/pyproject.toml` & `mkdocs_inline_svg_plugin-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "mkdocs-inline-svg-plugin"
-version = "0.1.3"
+version = "0.1.4"
 description = 'MkDocs plugin for inlining svg-href img tags'
 readme = "README.md"
 requires-python = ">=3.8"
 license = "MIT"
 keywords = ["MkDocs"]
 authors = [
   { name = "Oni Boni", email = "oniboni@mailbox.org" },
@@ -106,13 +106,13 @@
 # exclude_lines = [
 #   "no cov",
 #   "if __name__ == .__main__.:",
 #   "if TYPE_CHECKING:",
 # ]
 
 [tool.commitizen]
-version = "0.1.3"
+version = "0.1.4"
 tag_format = "v$version"
 version_files = [
   "pyproject.toml:version",
   "src/inline_svg/__init__.py",
 ]
```

### Comparing `mkdocs_inline_svg_plugin-0.1.3/PKG-INFO` & `mkdocs_inline_svg_plugin-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: mkdocs-inline-svg-plugin
-Version: 0.1.3
+Version: 0.1.4
 Summary: MkDocs plugin for inlining svg-href img tags
 Project-URL: Documentation, https://github.com/oniboni/mkdocs-inline-svg-plugin#readme
 Project-URL: Issues, https://github.com/oniboni/mkdocs-inline-svg-plugin/issues
 Project-URL: Source, https://github.com/oniboni/mkdocs-inline-svg-plugin
 Author-email: Oni Boni <oniboni@mailbox.org>
 License-Expression: MIT
 License-File: LICENSE.txt
```

