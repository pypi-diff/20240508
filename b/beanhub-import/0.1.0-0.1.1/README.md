# Comparing `tmp/beanhub_import-0.1.0.tar.gz` & `tmp/beanhub_import-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beanhub_import-0.1.0.tar", max compression
+gzip compressed data, was "beanhub_import-0.1.1.tar", max compression
```

## Comparing `beanhub_import-0.1.0.tar` & `beanhub_import-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1072 2024-05-07 02:15:06.507897 beanhub_import-0.1.0/LICENSE
--rw-r--r--   0        0        0      174 2024-05-07 02:15:06.507897 beanhub_import-0.1.0/README.md
--rw-r--r--   0        0        0        0 2024-05-07 02:15:06.507897 beanhub_import-0.1.0/beanhub_import/__init__.py
--rw-r--r--   0        0        0       28 2024-05-07 02:15:06.507897 beanhub_import-0.1.0/beanhub_import/constants.py
--rw-r--r--   0        0        0     3645 2024-05-07 02:15:06.507897 beanhub_import-0.1.0/beanhub_import/data_types.py
--rw-r--r--   0        0        0     6771 2024-05-07 02:15:06.507897 beanhub_import-0.1.0/beanhub_import/post_processor.py
--rw-r--r--   0        0        0     8883 2024-05-07 02:15:06.507897 beanhub_import-0.1.0/beanhub_import/processor.py
--rw-r--r--   0        0        0      725 2024-05-07 02:15:06.507897 beanhub_import-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1097 1970-01-01 00:00:00.000000 beanhub_import-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-08 17:54:23.508348 beanhub_import-0.1.1/LICENSE
+-rw-r--r--   0        0        0      174 2024-05-08 17:54:23.508348 beanhub_import-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2024-05-08 17:54:23.508348 beanhub_import-0.1.1/beanhub_import/__init__.py
+-rw-r--r--   0        0        0       58 2024-05-08 17:54:23.508348 beanhub_import-0.1.1/beanhub_import/constants.py
+-rw-r--r--   0        0        0     3771 2024-05-08 17:54:23.508348 beanhub_import-0.1.1/beanhub_import/data_types.py
+-rw-r--r--   0        0        0     6928 2024-05-08 17:54:23.508348 beanhub_import-0.1.1/beanhub_import/post_processor.py
+-rw-r--r--   0        0        0     9218 2024-05-08 17:54:23.508348 beanhub_import-0.1.1/beanhub_import/processor.py
+-rw-r--r--   0        0        0      725 2024-05-08 17:54:23.508348 beanhub_import-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1097 1970-01-01 00:00:00.000000 beanhub_import-0.1.1/PKG-INFO
```

### Comparing `beanhub_import-0.1.0/LICENSE` & `beanhub_import-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `beanhub_import-0.1.0/beanhub_import/data_types.py` & `beanhub_import-0.1.1/beanhub_import/data_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,16 +94,18 @@
     amount: Amount | None = None
     price: Amount | None = None
     cost: str | None = None
 
 
 class GeneratedTransaction(ImportBaseModel):
     file: str
-    # the import-id for de-duplication
+    # the `import-id` metadata field for de-duplication
     id: str
+    # the `import-src` metadata field for annotating the source file(s)
+    sources: list[str] | None = None
     date: str
     flag: str
     narration: str
     payee: str | None = None
     postings: list[GeneratedPosting]
```

### Comparing `beanhub_import-0.1.0/beanhub_import/post_processor.py` & `beanhub_import-0.1.1/beanhub_import/post_processor.py`

 * *Files 4% similar despite different names*

```diff
@@ -111,47 +111,55 @@
         columns.append(posting.cost)
     if posting.price is not None:
         columns.append(f"@ {posting.price.number} {posting.price.currency}")
     return (" " * 2) + " ".join(columns)
 
 
 def txn_to_text(
-    txn: GeneratedTransaction, import_id_key: str = constants.IMPORT_ID_KEY
+    txn: GeneratedTransaction,
 ) -> str:
     columns = [
         txn.date,
         txn.flag,
         *((json.dumps(txn.payee),) if txn.payee is not None else ()),
         json.dumps(txn.narration),
     ]
     line = " ".join(columns)
+    import_src = None
+    if txn.sources is not None:
+        import_src = ":".join(txn.sources)
     return "\n".join(
         [
             line,
-            f"  {import_id_key}: {json.dumps(txn.id)}",
+            f"  {constants.IMPORT_ID_KEY}: {json.dumps(txn.id)}",
+            *(
+                (f"  {constants.IMPORT_SRC_KEY}: {json.dumps(import_src)}",)
+                if import_src is not None
+                else ()
+            ),
             *(map(posting_to_text, txn.postings)),
         ]
     )
 
 
 def apply_change_set(
-    tree: Lark, change_set: ChangeSet, import_id_key: str = constants.IMPORT_ID_KEY
+    tree: Lark,
+    change_set: ChangeSet,
 ) -> Lark:
     if tree.data != "start":
         raise ValueError("expected start as the root rule")
     parser = make_parser()
 
     lines_to_remove = [txn.lineno for txn in change_set.remove]
     line_to_entries = {
         lineno: to_parser_entry(parser, txn_to_text(txn))
         for lineno, txn in change_set.update.items()
     }
     entries_to_add = [
-        to_parser_entry(parser, txn_to_text(txn, import_id_key=import_id_key))
-        for txn in change_set.add
+        to_parser_entry(parser, txn_to_text(txn)) for txn in change_set.add
     ]
 
     new_tree = copy.deepcopy(tree)
     entries, tail_comments = collect_entries(new_tree)
 
     tailing_comments_entry: typing.Optional[Entry] = None
     if tail_comments:
```

### Comparing `beanhub_import-0.1.0/beanhub_import/processor.py` & `beanhub_import-0.1.1/beanhub_import/processor.py`

 * *Files 3% similar despite different names*

```diff
@@ -169,14 +169,18 @@
                     import_rule,
                 )
                 raise ValueError(
                     f"Output file not defined when generating transaction with rule {import_rule}"
                 )
             processed = True
             yield GeneratedTransaction(
+                # We don't add line number here because sources it is going to be added as `import-src` metadata field.
+                # Otherwise provided CSV's lineno may change every time we run import if the date order is desc and
+                # there are new transactions added since then.
+                sources=[txn.file],
                 file=render_str(output_file),
                 postings=generated_postings,
                 **{key: render_str(value) for key, value in template_values.items()},
             )
             # TODO: make it possible to generate multiple transaction by changing rule config if there's
             #       a valid use case
         break
```

### Comparing `beanhub_import-0.1.0/pyproject.toml` & `beanhub_import-0.1.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "beanhub-import"
-version = "0.1.0"
+version = "0.1.1"
 description = "The simple library for import extracted transactions provided by beanhub-extract and generate corresponding Beancount transactions based on predefined rules"
 authors = ["Fang-Pen Lin <fangpen@launchplatform.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `beanhub_import-0.1.0/PKG-INFO` & `beanhub_import-0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beanhub-import
-Version: 0.1.0
+Version: 0.1.1
 Summary: The simple library for import extracted transactions provided by beanhub-extract and generate corresponding Beancount transactions based on predefined rules
 License: MIT
 Author: Fang-Pen Lin
 Author-email: fangpen@launchplatform.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

