# Comparing `tmp/utk_exodus-0.1.2.tar.gz` & `tmp/utk_exodus-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "utk_exodus-0.1.2.tar", max compression
+gzip compressed data, was "utk_exodus-0.1.3.tar", max compression
```

## Comparing `utk_exodus-0.1.2.tar` & `utk_exodus-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,21 @@
--rw-r--r--   0        0        0     1918 2024-05-07 19:02:36.432909 utk_exodus-0.1.2/README.md
--rw-r--r--   0        0        0      485 2024-05-07 19:42:25.331625 utk_exodus-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      291 2024-05-07 18:16:58.420598 utk_exodus-0.1.2/utk_exodus/__init__.py
--rw-r--r--   0        0        0       31 2024-05-07 18:16:58.412662 utk_exodus-0.1.2/utk_exodus/curate/__init__.py
--rw-r--r--   0        0        0     3927 2024-05-07 19:23:07.831658 utk_exodus-0.1.2/utk_exodus/curate/curate.py
--rw-r--r--   0        0        0     4306 2024-05-07 19:26:29.921054 utk_exodus-0.1.2/utk_exodus/exodus.py
--rw-r--r--   0        0        0       33 2024-04-30 19:26:23.807597 utk_exodus-0.1.2/utk_exodus/finder/__init__.py
--rw-r--r--   0        0        0    18718 2024-05-05 21:13:01.677173 utk_exodus-0.1.2/utk_exodus/finder/finder.py
--rw-r--r--   0        0        0      640 2024-05-06 19:12:23.968154 utk_exodus-0.1.2/utk_exodus/metadata/__init__.py
--rw-r--r--   0        0        0      135 2024-04-30 21:46:50.224208 utk_exodus-0.1.2/utk_exodus/metadata/base/__init__.py
--rw-r--r--   0        0        0     1280 2024-04-30 21:46:50.195943 utk_exodus-0.1.2/utk_exodus/metadata/base/base.py
--rw-r--r--   0        0        0    39221 2024-05-06 19:12:21.699513 utk_exodus-0.1.2/utk_exodus/metadata/metadata.py
--rw-r--r--   0        0        0       75 2024-05-01 12:54:48.901975 utk_exodus-0.1.2/utk_exodus/risearch/__init__.py
--rw-r--r--   0        0        0     7674 2024-05-01 12:51:59.027899 utk_exodus-0.1.2/utk_exodus/risearch/risearch.py
--rw-r--r--   0        0        0       71 2024-05-06 19:50:10.979729 utk_exodus-0.1.2/utk_exodus/validate/__init__.py
--rw-r--r--   0        0        0     6232 2024-05-07 15:31:28.330943 utk_exodus-0.1.2/utk_exodus/validate/validate.py
--rw-r--r--   0        0        0     2558 1970-01-01 00:00:00.000000 utk_exodus-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     2575 2024-05-08 21:11:48.505135 utk_exodus-0.1.3/README.md
+-rw-r--r--   0        0        0      576 2024-05-08 18:41:24.522141 utk_exodus-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      440 2024-05-08 14:55:57.119783 utk_exodus-0.1.3/utk_exodus/__init__.py
+-rw-r--r--   0        0        0       43 2024-05-08 14:32:31.650721 utk_exodus-0.1.3/utk_exodus/controller/__init__.py
+-rw-r--r--   0        0        0     4596 2024-05-08 21:37:32.451209 utk_exodus-0.1.3/utk_exodus/controller/controller.py
+-rw-r--r--   0        0        0       31 2024-05-07 18:16:58.412662 utk_exodus-0.1.3/utk_exodus/curate/__init__.py
+-rw-r--r--   0        0        0     3927 2024-05-07 19:23:07.831658 utk_exodus-0.1.3/utk_exodus/curate/curate.py
+-rw-r--r--   0        0        0     3943 2024-05-08 21:19:12.996464 utk_exodus-0.1.3/utk_exodus/exodus.py
+-rw-r--r--   0        0        0       32 2024-05-08 12:26:21.007671 utk_exodus-0.1.3/utk_exodus/fedora/__init__.py
+-rw-r--r--   0        0        0     1256 2024-05-08 21:08:02.300387 utk_exodus-0.1.3/utk_exodus/fedora/fedora.py
+-rw-r--r--   0        0        0       33 2024-04-30 19:26:23.807597 utk_exodus-0.1.3/utk_exodus/finder/__init__.py
+-rw-r--r--   0        0        0    18718 2024-05-05 21:13:01.677173 utk_exodus-0.1.3/utk_exodus/finder/finder.py
+-rw-r--r--   0        0        0      640 2024-05-06 19:12:23.968154 utk_exodus-0.1.3/utk_exodus/metadata/__init__.py
+-rw-r--r--   0        0        0      135 2024-04-30 21:46:50.224208 utk_exodus-0.1.3/utk_exodus/metadata/base/__init__.py
+-rw-r--r--   0        0        0     1280 2024-04-30 21:46:50.195943 utk_exodus-0.1.3/utk_exodus/metadata/base/base.py
+-rw-r--r--   0        0        0    39221 2024-05-06 19:12:21.699513 utk_exodus-0.1.3/utk_exodus/metadata/metadata.py
+-rw-r--r--   0        0        0       75 2024-05-01 12:54:48.901975 utk_exodus-0.1.3/utk_exodus/risearch/__init__.py
+-rw-r--r--   0        0        0     8833 2024-05-08 15:14:24.860576 utk_exodus-0.1.3/utk_exodus/risearch/risearch.py
+-rw-r--r--   0        0        0       71 2024-05-06 19:50:10.979729 utk_exodus-0.1.3/utk_exodus/validate/__init__.py
+-rw-r--r--   0        0        0     6236 2024-05-08 21:38:20.027155 utk_exodus-0.1.3/utk_exodus/validate/validate.py
+-rw-r--r--   0        0        0     3473 1970-01-01 00:00:00.000000 utk_exodus-0.1.3/PKG-INFO
```

### Comparing `utk_exodus-0.1.2/README.md` & `utk_exodus-0.1.3/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -4,30 +4,46 @@
 
 This application is a complete rewrite of the code used to migrate UTK content from Islandora 7 to Hyku.
 
 Unlike the previous code, this aims to be more flexible, easier to understand, and easier to use as a whole.
 
 ## Installing
 
-To install, simply:
+To install for use, ideally use `pipx`:
+
+```shell
+pipx install utk_exodus
+```
+
+The above will install the application in a virtual environment and make it available to you where ever you are in your
+path so you can use it from anywhere without needing to understand the intricacies of Python. 
+
+If you don't want to use `pipx`, you can install the whole library with the following command but do so mindfully:
 
 ```shell
 pip install utk_exodus
 ```
 
 ## Using
 
 There are several interfaces for the application.
 
-If you want to get works and files, use:
+If you want to get works and files, and you have metadata files, use::
 
 ```shell
 exodus works_and_files --path /path/to/metadata -o /path/to/directory/to/store/files
 ```
 
+If you want to get works and files, and you don't have metadata files, you need to specify
+a collection and a work type:
+
+```shell
+exodus works_and_files --collection "namespace:identifier" --model book -o /path/to/output/directory
+```
+
 If you just want works, use:
 
 ```shell
 exodus works --path /path/to/metadata
 ```
 
 If for some reason you need to create a files sheet for  works after the fact, use:
```

### Comparing `utk_exodus-0.1.2/utk_exodus/curate/curate.py` & `utk_exodus-0.1.3/utk_exodus/curate/curate.py`

 * *Files identical despite different names*

### Comparing `utk_exodus-0.1.2/utk_exodus/finder/finder.py` & `utk_exodus-0.1.3/utk_exodus/finder/finder.py`

 * *Files identical despite different names*

### Comparing `utk_exodus-0.1.2/utk_exodus/metadata/__init__.py` & `utk_exodus-0.1.3/utk_exodus/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `utk_exodus-0.1.2/utk_exodus/metadata/base/base.py` & `utk_exodus-0.1.3/utk_exodus/metadata/base/base.py`

 * *Files identical despite different names*

### Comparing `utk_exodus-0.1.2/utk_exodus/metadata/metadata.py` & `utk_exodus-0.1.3/utk_exodus/metadata/metadata.py`

 * *Files identical despite different names*

### Comparing `utk_exodus-0.1.2/utk_exodus/risearch/risearch.py` & `utk_exodus-0.1.3/utk_exodus/risearch/risearch.py`

 * *Files 5% similar despite different names*

```diff
@@ -161,18 +161,41 @@
         for item in cleaned:
             if item != '"pid","page"' and item != "":
                 all_pages.append(
                     {"pid": item.split(",")[0], "page": item.split(",")[1]}
                 )
         return all_pages
 
+    @staticmethod
+    def __lookup_work_type(work_type):
+        work_types = {
+            "book": "info:fedora/islandora:bookCModel",
+            "image": "info:fedora/islandora:sp_basic_image",
+            "compound": "info:fedora/islandora:compoundCModel",
+            "audio": "info:fedora/islandora:sp-audioCModel",
+            "video": "info:fedora/islandora:sp_videoCModel",
+            "pdf": "info:fedora/islandora:sp_pdf",
+        }
+        return work_types.get(work_type, "unknown")
+
+    def get_works_based_on_type_and_collection(self, work_type, collection):
+        iri = self.__lookup_work_type(work_type).strip()
+        query = quote(
+            f"PREFIX rels-ext: <info:fedora/fedora-system:def/relations-external#>"
+            f"PREFIX model: <info:fedora/fedora-system:def/model#>"
+            f"SELECT ?pid WHERE {{ ?pid rels-ext:isMemberOfCollection <info:fedora/{collection}> ;"
+            f"model:hasModel <{iri}> ."
+            f"}}"
+        )
+        results = requests.get(f"{self.base_url}&query={query}").content.decode("utf-8")
+        return [result for result in results.split("\n") if result != "" and result != '"pid"']
+
 
 if __name__ == "__main__":
     import argparse
-
     parser = argparse.ArgumentParser(description="Find things to download.")
     parser.add_argument(
         "-c",
         "--sheet",
         dest="collection",
         help="Specify collection pid.",
         required=True,
```

### Comparing `utk_exodus-0.1.2/utk_exodus/validate/validate.py` & `utk_exodus-0.1.3/utk_exodus/validate/validate.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,18 +141,18 @@
             self.validate_model(row)
             self.validate_values(row)
             self.validate_license(row)
             self.check_required_fields_are_present(row)
         separator = "\n"
         if len(self.all_exceptions) > 0:
             raise Exception(
-                f"Migration spreadsheet has at least {len(self.all_exceptions)} problems: {separator.join(self.all_exceptions)}"
+                f"\tMigration spreadsheet has at least {len(self.all_exceptions)} problems: {separator.join(self.all_exceptions)}"
             )
         else:
-            print("Sheet passes all tests.")
+            print("\tSheet passes all tests.")
 
 
 if __name__ == "__main__":
     import argparse
     parser = argparse.ArgumentParser(description="Choose sheet to validate..")
     parser.add_argument(
         "-s", "--sheet", dest="sheet", help="Specify csv to test.", required=True
```

### Comparing `utk_exodus-0.1.2/PKG-INFO` & `utk_exodus-0.1.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 Metadata-Version: 2.1
 Name: utk-exodus
-Version: 0.1.2
-Summary: 
+Version: 0.1.3
+Summary: A tool for building import sheets from UTK legacy systems
 Author: Mark Baggett
 Author-email: mbagget1@utk.edu
-Requires-Python: >=3.12,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: black (>=24.4.2,<25.0.0)
 Requires-Dist: click (>=8.1.7,<9.0.0)
 Requires-Dist: lxml (>=5.2.1,<6.0.0)
 Requires-Dist: pytest (>=8.2.0,<9.0.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
@@ -24,30 +28,46 @@
 
 This application is a complete rewrite of the code used to migrate UTK content from Islandora 7 to Hyku.
 
 Unlike the previous code, this aims to be more flexible, easier to understand, and easier to use as a whole.
 
 ## Installing
 
-To install, simply:
+To install for use, ideally use `pipx`:
+
+```shell
+pipx install utk_exodus
+```
+
+The above will install the application in a virtual environment and make it available to you where ever you are in your
+path so you can use it from anywhere without needing to understand the intricacies of Python. 
+
+If you don't want to use `pipx`, you can install the whole library with the following command but do so mindfully:
 
 ```shell
 pip install utk_exodus
 ```
 
 ## Using
 
 There are several interfaces for the application.
 
-If you want to get works and files, use:
+If you want to get works and files, and you have metadata files, use::
 
 ```shell
 exodus works_and_files --path /path/to/metadata -o /path/to/directory/to/store/files
 ```
 
+If you want to get works and files, and you don't have metadata files, you need to specify
+a collection and a work type:
+
+```shell
+exodus works_and_files --collection "namespace:identifier" --model book -o /path/to/output/directory
+```
+
 If you just want works, use:
 
 ```shell
 exodus works --path /path/to/metadata
 ```
 
 If for some reason you need to create a files sheet for  works after the fact, use:
```

