# Comparing `tmp/mkdocs-annexes-integration-0.1.6.tar.gz` & `tmp/mkdocs-annexes-integration-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-annexes-integration-0.1.6.tar", last modified: Mon Apr 29 14:41:55 2024, max compression
+gzip compressed data, was "mkdocs-annexes-integration-0.1.7.tar", last modified: Wed May  8 15:16:52 2024, max compression
```

## Comparing `mkdocs-annexes-integration-0.1.6.tar` & `mkdocs-annexes-integration-0.1.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)        0 2024-04-29 14:40:40.973576 mkdocs-annexes-integration-0.1.6/
--rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)       77 2024-04-29 08:29:27.000000 mkdocs-annexes-integration-0.1.6/MANIFEST.in
--rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)     4150 2024-04-29 14:41:55.846781 mkdocs-annexes-integration-0.1.6/PKG-INFO
--rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)     1428 2024-04-29 14:33:40.000000 mkdocs-annexes-integration-0.1.6/changelog.md
--rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)     1075 2024-04-29 08:29:27.000000 mkdocs-annexes-integration-0.1.6/license
-drwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)        0 2024-04-29 14:40:40.865490 mkdocs-annexes-integration-0.1.6/mkdocs_annexes_integration/
--rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)        0 2024-04-29 08:29:27.000000 mkdocs-annexes-integration-0.1.6/mkdocs_annexes_integration/__init__.py
--rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)     8553 2024-04-29 14:36:11.000000 mkdocs-annexes-integration-0.1.6/mkdocs_annexes_integration/plugin.py
-drwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)        0 2024-04-29 14:41:55.831885 mkdocs-annexes-integration-0.1.6/mkdocs_annexes_integration.egg-info/
--rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)     4150 2024-04-29 14:41:55.000000 mkdocs-annexes-integration-0.1.6/mkdocs_annexes_integration.egg-info/PKG-INFO
--rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)      441 2024-04-29 14:41:55.000000 mkdocs-annexes-integration-0.1.6/mkdocs_annexes_integration.egg-info/SOURCES.txt
--rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)        1 2024-04-29 14:41:55.000000 mkdocs-annexes-integration-0.1.6/mkdocs_annexes_integration.egg-info/dependency_links.txt
--rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)       93 2024-04-29 14:41:55.000000 mkdocs-annexes-integration-0.1.6/mkdocs_annexes_integration.egg-info/entry_points.txt
--rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)       32 2024-04-29 14:41:55.000000 mkdocs-annexes-integration-0.1.6/mkdocs_annexes_integration.egg-info/requires.txt
--rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)       27 2024-04-29 14:41:55.000000 mkdocs-annexes-integration-0.1.6/mkdocs_annexes_integration.egg-info/top_level.txt
--rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)     3536 2024-04-29 14:38:48.000000 mkdocs-annexes-integration-0.1.6/readme.md
--rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)       38 2024-04-29 14:41:55.850778 mkdocs-annexes-integration-0.1.6/setup.cfg
--rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)     1201 2024-04-29 14:37:54.000000 mkdocs-annexes-integration-0.1.6/setup.py
+drwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)        0 2024-05-08 15:16:52.787699 mkdocs-annexes-integration-0.1.7/
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)       77 2024-04-29 08:29:27.000000 mkdocs-annexes-integration-0.1.7/MANIFEST.in
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)     4447 2024-05-08 15:16:52.784699 mkdocs-annexes-integration-0.1.7/PKG-INFO
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)     1620 2024-05-08 15:11:41.000000 mkdocs-annexes-integration-0.1.7/changelog.md
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)     1075 2024-04-29 08:29:27.000000 mkdocs-annexes-integration-0.1.7/license
+drwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)        0 2024-05-08 15:16:52.669559 mkdocs-annexes-integration-0.1.7/mkdocs_annexes_integration/
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)        0 2024-04-29 08:29:27.000000 mkdocs-annexes-integration-0.1.7/mkdocs_annexes_integration/__init__.py
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)    10452 2024-05-06 11:44:19.000000 mkdocs-annexes-integration-0.1.7/mkdocs_annexes_integration/plugin.py
+drwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)        0 2024-05-08 15:16:52.767583 mkdocs-annexes-integration-0.1.7/mkdocs_annexes_integration.egg-info/
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)     4447 2024-05-08 15:16:52.000000 mkdocs-annexes-integration-0.1.7/mkdocs_annexes_integration.egg-info/PKG-INFO
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)      441 2024-05-08 15:16:52.000000 mkdocs-annexes-integration-0.1.7/mkdocs_annexes_integration.egg-info/SOURCES.txt
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)        1 2024-05-08 15:16:52.000000 mkdocs-annexes-integration-0.1.7/mkdocs_annexes_integration.egg-info/dependency_links.txt
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)       93 2024-05-08 15:16:52.000000 mkdocs-annexes-integration-0.1.7/mkdocs_annexes_integration.egg-info/entry_points.txt
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)       32 2024-05-08 15:16:52.000000 mkdocs-annexes-integration-0.1.7/mkdocs_annexes_integration.egg-info/requires.txt
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)       27 2024-05-08 15:16:52.000000 mkdocs-annexes-integration-0.1.7/mkdocs_annexes_integration.egg-info/top_level.txt
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)     3835 2024-05-08 15:15:35.000000 mkdocs-annexes-integration-0.1.7/readme.md
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)       38 2024-05-08 15:16:52.788702 mkdocs-annexes-integration-0.1.7/setup.cfg
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)     1201 2024-05-08 15:16:09.000000 mkdocs-annexes-integration-0.1.7/setup.py
```

### Comparing `mkdocs-annexes-integration-0.1.6/PKG-INFO` & `mkdocs-annexes-integration-0.1.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-annexes-integration
-Version: 0.1.6
+Version: 0.1.7
 Summary: A MkDocs plugin transforming annexes files into images to be integrated in markdown pages
 Home-page: https://gitlab.com/cfpt-mkdocs-plugins/mkdocs-annexes-integration
 Author: Thibaud Briard
 Author-email: thibaud.brrd@eduge.ch
 License: MIT
 Keywords: mkdocs
 Platform: UNKNOWN
@@ -66,23 +66,25 @@
         - Title of the annex B1: path/B/to/an/annex1.pdf # Another path to an annex but in different folder as the first two
         - Title of the annex:
             src: ../src/path/to/an/annex/file1.py
             dest: dest/path/to/an/annex/file1.py
         # others annexes...
       temp_dir: "folder_name" # Optional --> Default : temp_annexes
       enabled_if_env: ENABLE_PDF_EXPORT # Optional
+      placeholders_when_disabled: true # Optional --> Default : false
 ```
 
 As you can see, there are two possible ways to integrate an annex: using a simple path or a source path and a destination path. **Both paths need to be relative to `docs_dir`, though**.
 
 Set at least one annex to use this plugin. If you don't have any annex don't add this plugin to the mkdocs plugins list in config file mkdocs.yml
 
 - `annexes` - A list of all the annexes documents. The path from `docs_dir` to an annex file associated to it's title
 - `temp_dir` - The temp directory used to generate markdown file for each annex before rendering to HTML. Only set this option if you already have a temp_annexes folder in the root directory (same as mkdocs.yml), which, you should not normally.
 - `enabled_if_env` - Setting this option will enable the build only if there is an environment variable set to 1. Integrations of PDF can slow down build process and it's pretty useful to be fast when doing modification to mkdocs files when doing mkdocs serve.
+- `placeholders_when_disabled` - This option will generate an mock file at the place of the integrated file to prevent warning from unreferenced link to the page by other pages. It is intended to be used with `enabled_if_env`.
 
 ## Usage
 
 Using the command `mkdocs build` or `mkdocs serve` will trigger the plugin if it as been set correctly in config file.
 
 This plugin is intended to be used with `mkdocs-with-pdf` plugin but can be used as it is.
```

### Comparing `mkdocs-annexes-integration-0.1.6/changelog.md` & `mkdocs-annexes-integration-0.1.7/changelog.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,24 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on Keep a Changelog, and this project adheres to Semantic Versioning.
 
-## [0.1.5] - 2024-04-29
+## [0.1.7] - 2024-05-08
+
+### Added
+
+- Support for a placeholder file generation option for when plugin is disable
+
+### Fixed
+
+- Size of image to big to be used in `mkdocs-with-pdf`
+
+## [0.1.6] - 2024-04-29
 
 ### Removed
 
 - Support for code files as it is already supported by `mkdocs-material`
 
 ### Fixed
```

### Comparing `mkdocs-annexes-integration-0.1.6/license` & `mkdocs-annexes-integration-0.1.7/license`

 * *Files identical despite different names*

### Comparing `mkdocs-annexes-integration-0.1.6/mkdocs_annexes_integration/plugin.py` & `mkdocs-annexes-integration-0.1.7/mkdocs_annexes_integration/plugin.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from mkdocs.plugins import BasePlugin as base_plugin # used to create an MkDocs plugin class derived from MkDocs plugin base
 from mkdocs.config import config_options as c # used for config schema type safety
 from mkdocs.structure.files import File # used to create File in documentation
 
 # The plugin config options
 class AnnexesIntegrationConfig(base_config):
     enabled_if_env = c.Type(str, default='')
+    placeholders_when_disabled = c.Type(bool, default=False)
     enable = c.Type(bool, default=True)
     temp_dir = c.Type(str, default='temp_annexes')
     annexes = c.ListOfItems(c.Type(dict))
 
 # The plugin itself
 class AnnexesIntegration(base_plugin[AnnexesIntegrationConfig]):
 
@@ -52,41 +53,42 @@
         if self.enabled:
             self.config.temp_dir = os.path.join(os.path.dirname(config.docs_dir), self.config.temp_dir)
             if not os.path.exists(self.config.temp_dir):
                 os.mkdir(self.config.temp_dir)
         return config
 
     def on_files(self, files, config):
-        if self.enabled:
+        try:
             # Generate markdown files for each annex
-            try:
-                for annex in self.config.annexes:
-                    title, path = list(annex.items())[0]
-                    self._logger.info(f'Integrating annex "{title}"')
-                    # Determine source and destination path from path option
-                    src, dest = self.get_src_and_dest(path)
-                    # Get extension of file
-                    extension = os.path.splitext(src)[1][1:]
-                    # Get absolute path to original file
-                    original = os.path.join(config.docs_dir, src)
-                    # Get absolute path to generated markdown
+            for annex in self.config.annexes:
+                # Get absolute path to generated markdown
+                title, path = list(annex.items())[0]
+                # Determine source and destination path from path option
+                src, dest = self.get_src_and_dest(path)
+                # Get absolute path for PDF directory
+                root = os.path.join(self.config.temp_dir, os.path.splitext(dest)[0])
+                # Create a root folder containing the annex
+                if not os.path.exists(root):
+                    os.makedirs(root)
+                # Get extension of file
+                extension = os.path.splitext(src)[1][1:]
+                # Get absolute path to original file
+                original = os.path.join(config.docs_dir, src)
+                # skip if original file don't exist
+                if os.path.exists(original):
                     embedded = f'{os.path.join(self.config.temp_dir, os.path.splitext(dest)[0])}.md'
-                    # skip if original file don't exist
-                    if os.path.exists(original):
+                    
+                    if self.enabled:
+                        self._logger.info(f'Integrating annex "{title}"')
                         # Check if file is a PDF
                         if extension in ['pdf']:
                             # For PDF files each page are transformed into images
                             self._logger.info(f'    With each pages as images')
-                            # Get absolute path for PDF directory
-                            root = os.path.join(self.config.temp_dir, os.path.splitext(dest)[0])
                             # Get absolute path for PDF images directory
                             source = os.path.join(root, 'source')
-                            # Create a root folder containing the annex
-                            if not os.path.exists(root):
-                                os.makedirs(root)
                             # Save pages as images in the pdf
                             images = convert_from_path(original, size=(None, 800))
                             # Create source folder to save images
                             if not os.path.exists(source):
                                 os.mkdir(source)
                             # Create a markdown file that take care of showing PDF annex
                             with open(embedded, 'w') as f:
@@ -107,22 +109,41 @@
                         if os.path.isfile(os.path.join(config.docs_dir, dest)):
                             self._logger.info(f'    Remvoing original annex {src} from processed files list')
                             files.remove(files.get_file_from_path(src))
                         # Adding embedded files in list of mkdocs files
                         path = f'{os.path.splitext(dest)[0]}.md'
                         self._logger.info(f'    Adding embedded annex {dest} to processed files list')
                         files.append(File(path, src_dir=self.config.temp_dir, dest_dir=config.site_dir, use_directory_urls=config.use_directory_urls))
-                    else:
-                        self._logger.warning(f'{src} file doesn\'t exist at {original} --> skipped')
-            except Exception as e:
-                # Remove temp directory in case of any error before raising error
-                self._logger.error(f'error with the annexes-integration plugin : {e}')
-                if os.path.exists(self.config.temp_dir):
-                    shutil.rmtree(self.config.temp_dir)
-                raise e
+                    elif self.config['placeholders_when_disabled']:
+                        # Create a markdown file that take care of showing PDF annex
+                        with open(embedded, 'w') as f:
+                            # Write the title to the file
+                            f.write(f'# {title}\n\n')
+                            f.write(f'The annex at `{src}` was not integrated because annexes integration plugin was not enable.\n\n')
+                            f.write(f'To enable the plugin functionnality please do one of the following action:\n\n')
+                            f.write(f' - set environment variable `{self.config["enabled_if_env"]}` to 1 before mkdocs command: `{self.config["enabled_if_env"]}=1 mkdocs {{build|serve}}`\n')
+                            f.write(f' - remove `enabled_if_env` option in mkdocs.yml under the `plugins > annexes-integration` section\n\n')
+                            f.write(f'To disable the creation of placeholders when plugin is disable, remove or set to false the `placeholders_when_disabled` option in mkdocs.yml under the `plugins > annexes-integration` section\n\n')
+                        # Removing originals files from list of mkdocs files if they were in the docs directory originaly
+                        if os.path.isfile(os.path.join(config.docs_dir, dest)):
+                            self._logger.debug(f'    Remvoing original annex {src} from processed files list')
+                            files.remove(files.get_file_from_path(src))
+                        # Adding embedded files in list of mkdocs files
+                        path = f'{os.path.splitext(dest)[0]}.md'
+                        self._logger.debug(f'    Adding embedded annex {dest} to processed files list')
+                        files.append(File(path, src_dir=self.config.temp_dir, dest_dir=config.site_dir, use_directory_urls=config.use_directory_urls))
+                else:
+                    self._logger.warning(f'{src} file doesn\'t exist at {original} --> skipped')
+
+        except Exception as e:
+            # Remove temp directory in case of any error before raising error
+            self._logger.error(f'error with the annexes-integration plugin : {e}')
+            if os.path.exists(self.config.temp_dir):
+                shutil.rmtree(self.config.temp_dir)
+            raise e
         return files
     
     def on_post_build(self, config):
         if self.enabled:
             # Removing temp_dir directory
             self._logger.info(f'Removin annexes temporary directory {self.config.temp_dir}')
             if os.path.exists(self.config.temp_dir):
```

### Comparing `mkdocs-annexes-integration-0.1.6/mkdocs_annexes_integration.egg-info/PKG-INFO` & `mkdocs-annexes-integration-0.1.7/mkdocs_annexes_integration.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-annexes-integration
-Version: 0.1.6
+Version: 0.1.7
 Summary: A MkDocs plugin transforming annexes files into images to be integrated in markdown pages
 Home-page: https://gitlab.com/cfpt-mkdocs-plugins/mkdocs-annexes-integration
 Author: Thibaud Briard
 Author-email: thibaud.brrd@eduge.ch
 License: MIT
 Keywords: mkdocs
 Platform: UNKNOWN
@@ -66,23 +66,25 @@
         - Title of the annex B1: path/B/to/an/annex1.pdf # Another path to an annex but in different folder as the first two
         - Title of the annex:
             src: ../src/path/to/an/annex/file1.py
             dest: dest/path/to/an/annex/file1.py
         # others annexes...
       temp_dir: "folder_name" # Optional --> Default : temp_annexes
       enabled_if_env: ENABLE_PDF_EXPORT # Optional
+      placeholders_when_disabled: true # Optional --> Default : false
 ```
 
 As you can see, there are two possible ways to integrate an annex: using a simple path or a source path and a destination path. **Both paths need to be relative to `docs_dir`, though**.
 
 Set at least one annex to use this plugin. If you don't have any annex don't add this plugin to the mkdocs plugins list in config file mkdocs.yml
 
 - `annexes` - A list of all the annexes documents. The path from `docs_dir` to an annex file associated to it's title
 - `temp_dir` - The temp directory used to generate markdown file for each annex before rendering to HTML. Only set this option if you already have a temp_annexes folder in the root directory (same as mkdocs.yml), which, you should not normally.
 - `enabled_if_env` - Setting this option will enable the build only if there is an environment variable set to 1. Integrations of PDF can slow down build process and it's pretty useful to be fast when doing modification to mkdocs files when doing mkdocs serve.
+- `placeholders_when_disabled` - This option will generate an mock file at the place of the integrated file to prevent warning from unreferenced link to the page by other pages. It is intended to be used with `enabled_if_env`.
 
 ## Usage
 
 Using the command `mkdocs build` or `mkdocs serve` will trigger the plugin if it as been set correctly in config file.
 
 This plugin is intended to be used with `mkdocs-with-pdf` plugin but can be used as it is.
```

### Comparing `mkdocs-annexes-integration-0.1.6/readme.md` & `mkdocs-annexes-integration-0.1.7/readme.md`

 * *Files 4% similar despite different names*

```diff
@@ -47,23 +47,25 @@
         - Title of the annex B1: path/B/to/an/annex1.pdf # Another path to an annex but in different folder as the first two
         - Title of the annex:
             src: ../src/path/to/an/annex/file1.py
             dest: dest/path/to/an/annex/file1.py
         # others annexes...
       temp_dir: "folder_name" # Optional --> Default : temp_annexes
       enabled_if_env: ENABLE_PDF_EXPORT # Optional
+      placeholders_when_disabled: true # Optional --> Default : false
 ```
 
 As you can see, there are two possible ways to integrate an annex: using a simple path or a source path and a destination path. **Both paths need to be relative to `docs_dir`, though**.
 
 Set at least one annex to use this plugin. If you don't have any annex don't add this plugin to the mkdocs plugins list in config file mkdocs.yml
 
 - `annexes` - A list of all the annexes documents. The path from `docs_dir` to an annex file associated to it's title
 - `temp_dir` - The temp directory used to generate markdown file for each annex before rendering to HTML. Only set this option if you already have a temp_annexes folder in the root directory (same as mkdocs.yml), which, you should not normally.
 - `enabled_if_env` - Setting this option will enable the build only if there is an environment variable set to 1. Integrations of PDF can slow down build process and it's pretty useful to be fast when doing modification to mkdocs files when doing mkdocs serve.
+- `placeholders_when_disabled` - This option will generate an mock file at the place of the integrated file to prevent warning from unreferenced link to the page by other pages. It is intended to be used with `enabled_if_env`.
 
 ## Usage
 
 Using the command `mkdocs build` or `mkdocs serve` will trigger the plugin if it as been set correctly in config file.
 
 This plugin is intended to be used with `mkdocs-with-pdf` plugin but can be used as it is.
```

### Comparing `mkdocs-annexes-integration-0.1.6/setup.py` & `mkdocs-annexes-integration-0.1.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import io
 
 from setuptools import setup, find_packages
 
 setup(
     name='mkdocs-annexes-integration',
-    version='0.1.6',
+    version='0.1.7',
     description='A MkDocs plugin transforming annexes files into images to be integrated in markdown pages',
     long_description=io.open('readme.md', encoding='utf8').read(),
     long_description_content_type='text/markdown',
     keywords='mkdocs',
     url='https://gitlab.com/cfpt-mkdocs-plugins/mkdocs-annexes-integration',
     author='Thibaud Briard',
     author_email='thibaud.brrd@eduge.ch',
```

