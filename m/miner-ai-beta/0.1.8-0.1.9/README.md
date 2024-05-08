# Comparing `tmp/miner_ai_beta-0.1.8.tar.gz` & `tmp/miner_ai_beta-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "miner_ai_beta-0.1.8.tar", max compression
+gzip compressed data, was "miner_ai_beta-0.1.9.tar", max compression
```

## Comparing `miner_ai_beta-0.1.8.tar` & `miner_ai_beta-0.1.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0    11357 2024-05-04 16:49:23.857900 miner_ai_beta-0.1.8/LICENSE
--rw-r--r--   0        0        0      242 2024-05-04 16:59:21.199649 miner_ai_beta-0.1.8/miner_ai_beta/loader/__init__.py
--rw-r--r--   0        0        0      473 2024-05-04 16:04:57.185499 miner_ai_beta-0.1.8/miner_ai_beta/loader/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0     3042 2024-05-04 15:17:18.873214 miner_ai_beta-0.1.8/miner_ai_beta/loader/__pycache__/docs.cpython-311.pyc
--rw-r--r--   0        0        0     2372 2024-05-04 16:04:57.189700 miner_ai_beta-0.1.8/miner_ai_beta/loader/__pycache__/docs.cpython-312.pyc
--rw-r--r--   0        0        0     2299 2024-05-04 16:04:58.283790 miner_ai_beta-0.1.8/miner_ai_beta/loader/__pycache__/excels.cpython-312.pyc
--rw-r--r--   0        0        0     3252 2024-05-04 15:17:18.945722 miner_ai_beta-0.1.8/miner_ai_beta/loader/__pycache__/pages.cpython-311.pyc
--rw-r--r--   0        0        0     2566 2024-05-04 15:17:18.984762 miner_ai_beta-0.1.8/miner_ai_beta/loader/__pycache__/pages.cpython-312.pyc
--rw-r--r--   0        0        0     3161 2024-05-04 15:17:19.027542 miner_ai_beta-0.1.8/miner_ai_beta/loader/__pycache__/pdfs.cpython-311.pyc
--rw-r--r--   0        0        0     2309 2024-05-04 16:05:00.319553 miner_ai_beta-0.1.8/miner_ai_beta/loader/__pycache__/pdfs.cpython-312.pyc
--rw-r--r--   0        0        0     2165 2024-05-04 16:05:00.402279 miner_ai_beta-0.1.8/miner_ai_beta/loader/__pycache__/ppts.cpython-312.pyc
--rw-r--r--   0        0        0     2343 2024-05-04 16:05:00.331906 miner_ai_beta-0.1.8/miner_ai_beta/loader/__pycache__/tubes.cpython-312.pyc
--rw-r--r--   0        0        0      711 2024-05-04 16:05:00.626643 miner_ai_beta-0.1.8/miner_ai_beta/loader/__pycache__/union.cpython-312.pyc
--rw-r--r--   0        0        0     2455 2024-05-04 16:05:00.139759 miner_ai_beta-0.1.8/miner_ai_beta/loader/__pycache__/web_pages.cpython-312.pyc
--rw-r--r--   0        0        0     2928 2024-05-04 15:17:19.188416 miner_ai_beta-0.1.8/miner_ai_beta/loader/__pycache__/xlss.cpython-311.pyc
--rw-r--r--   0        0        0     2490 2024-05-04 15:17:19.226637 miner_ai_beta-0.1.8/miner_ai_beta/loader/__pycache__/xlss.cpython-312.pyc
--rw-r--r--   0        0        0     1804 2024-05-08 02:22:00.293266 miner_ai_beta-0.1.8/miner_ai_beta/loader/docs.py
--rw-r--r--   0        0        0     1915 2024-05-08 02:22:00.295487 miner_ai_beta-0.1.8/miner_ai_beta/loader/excels.py
--rw-r--r--   0        0        0     1760 2024-05-08 02:22:00.298503 miner_ai_beta-0.1.8/miner_ai_beta/loader/pdfs.py
--rw-r--r--   0        0        0     1805 2024-05-08 02:22:00.299662 miner_ai_beta-0.1.8/miner_ai_beta/loader/ppts.py
--rw-r--r--   0        0        0     1895 2024-05-08 02:22:00.300684 miner_ai_beta-0.1.8/miner_ai_beta/loader/tubes.py
--rw-r--r--   0        0        0      361 2024-05-04 15:52:12.917924 miner_ai_beta-0.1.8/miner_ai_beta/loader/union.py
--rw-r--r--   0        0        0     1873 2024-05-06 15:23:32.901218 miner_ai_beta-0.1.8/miner_ai_beta/loader/web_pages.py
--rw-r--r--   0        0        0      668 2024-05-08 02:23:26.746441 miner_ai_beta-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     3966 2024-05-05 07:06:38.721971 miner_ai_beta-0.1.8/README.md
--rw-r--r--   0        0        0     4883 1970-01-01 00:00:00.000000 miner_ai_beta-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-04 16:49:23.857900 miner_ai_beta-0.1.9/LICENSE
+-rw-r--r--   0        0        0      242 2024-05-04 16:59:21.199649 miner_ai_beta-0.1.9/miner_ai_beta/loader/__init__.py
+-rw-r--r--   0        0        0      473 2024-05-04 16:04:57.185499 miner_ai_beta-0.1.9/miner_ai_beta/loader/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0     3042 2024-05-04 15:17:18.873214 miner_ai_beta-0.1.9/miner_ai_beta/loader/__pycache__/docs.cpython-311.pyc
+-rw-r--r--   0        0        0     2372 2024-05-04 16:04:57.189700 miner_ai_beta-0.1.9/miner_ai_beta/loader/__pycache__/docs.cpython-312.pyc
+-rw-r--r--   0        0        0     2299 2024-05-04 16:04:58.283790 miner_ai_beta-0.1.9/miner_ai_beta/loader/__pycache__/excels.cpython-312.pyc
+-rw-r--r--   0        0        0     3252 2024-05-04 15:17:18.945722 miner_ai_beta-0.1.9/miner_ai_beta/loader/__pycache__/pages.cpython-311.pyc
+-rw-r--r--   0        0        0     2566 2024-05-04 15:17:18.984762 miner_ai_beta-0.1.9/miner_ai_beta/loader/__pycache__/pages.cpython-312.pyc
+-rw-r--r--   0        0        0     3161 2024-05-04 15:17:19.027542 miner_ai_beta-0.1.9/miner_ai_beta/loader/__pycache__/pdfs.cpython-311.pyc
+-rw-r--r--   0        0        0     2309 2024-05-04 16:05:00.319553 miner_ai_beta-0.1.9/miner_ai_beta/loader/__pycache__/pdfs.cpython-312.pyc
+-rw-r--r--   0        0        0     2165 2024-05-04 16:05:00.402279 miner_ai_beta-0.1.9/miner_ai_beta/loader/__pycache__/ppts.cpython-312.pyc
+-rw-r--r--   0        0        0     2343 2024-05-04 16:05:00.331906 miner_ai_beta-0.1.9/miner_ai_beta/loader/__pycache__/tubes.cpython-312.pyc
+-rw-r--r--   0        0        0      711 2024-05-04 16:05:00.626643 miner_ai_beta-0.1.9/miner_ai_beta/loader/__pycache__/union.cpython-312.pyc
+-rw-r--r--   0        0        0     2455 2024-05-04 16:05:00.139759 miner_ai_beta-0.1.9/miner_ai_beta/loader/__pycache__/web_pages.cpython-312.pyc
+-rw-r--r--   0        0        0     2928 2024-05-04 15:17:19.188416 miner_ai_beta-0.1.9/miner_ai_beta/loader/__pycache__/xlss.cpython-311.pyc
+-rw-r--r--   0        0        0     2490 2024-05-04 15:17:19.226637 miner_ai_beta-0.1.9/miner_ai_beta/loader/__pycache__/xlss.cpython-312.pyc
+-rw-r--r--   0        0        0     1804 2024-05-08 02:22:00.293266 miner_ai_beta-0.1.9/miner_ai_beta/loader/docs.py
+-rw-r--r--   0        0        0     1962 2024-05-08 02:33:45.134979 miner_ai_beta-0.1.9/miner_ai_beta/loader/excels.py
+-rw-r--r--   0        0        0     1760 2024-05-08 02:22:00.298503 miner_ai_beta-0.1.9/miner_ai_beta/loader/pdfs.py
+-rw-r--r--   0        0        0     1805 2024-05-08 02:22:00.299662 miner_ai_beta-0.1.9/miner_ai_beta/loader/ppts.py
+-rw-r--r--   0        0        0     1895 2024-05-08 02:22:00.300684 miner_ai_beta-0.1.9/miner_ai_beta/loader/tubes.py
+-rw-r--r--   0        0        0      361 2024-05-04 15:52:12.917924 miner_ai_beta-0.1.9/miner_ai_beta/loader/union.py
+-rw-r--r--   0        0        0     1873 2024-05-06 15:23:32.901218 miner_ai_beta-0.1.9/miner_ai_beta/loader/web_pages.py
+-rw-r--r--   0        0        0      668 2024-05-08 02:34:33.567384 miner_ai_beta-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     3966 2024-05-05 07:06:38.721971 miner_ai_beta-0.1.9/README.md
+-rw-r--r--   0        0        0     4883 1970-01-01 00:00:00.000000 miner_ai_beta-0.1.9/PKG-INFO
```

### Comparing `miner_ai_beta-0.1.8/LICENSE` & `miner_ai_beta-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `miner_ai_beta-0.1.8/miner_ai_beta/loader/__pycache__/docs.cpython-311.pyc` & `miner_ai_beta-0.1.9/miner_ai_beta/loader/__pycache__/docs.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `miner_ai_beta-0.1.8/miner_ai_beta/loader/__pycache__/docs.cpython-312.pyc` & `miner_ai_beta-0.1.9/miner_ai_beta/loader/__pycache__/docs.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `miner_ai_beta-0.1.8/miner_ai_beta/loader/__pycache__/excels.cpython-312.pyc` & `miner_ai_beta-0.1.9/miner_ai_beta/loader/__pycache__/excels.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `miner_ai_beta-0.1.8/miner_ai_beta/loader/__pycache__/pages.cpython-311.pyc` & `miner_ai_beta-0.1.9/miner_ai_beta/loader/__pycache__/pages.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `miner_ai_beta-0.1.8/miner_ai_beta/loader/__pycache__/pages.cpython-312.pyc` & `miner_ai_beta-0.1.9/miner_ai_beta/loader/__pycache__/pages.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `miner_ai_beta-0.1.8/miner_ai_beta/loader/__pycache__/pdfs.cpython-311.pyc` & `miner_ai_beta-0.1.9/miner_ai_beta/loader/__pycache__/pdfs.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `miner_ai_beta-0.1.8/miner_ai_beta/loader/__pycache__/pdfs.cpython-312.pyc` & `miner_ai_beta-0.1.9/miner_ai_beta/loader/__pycache__/pdfs.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `miner_ai_beta-0.1.8/miner_ai_beta/loader/__pycache__/ppts.cpython-312.pyc` & `miner_ai_beta-0.1.9/miner_ai_beta/loader/__pycache__/ppts.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `miner_ai_beta-0.1.8/miner_ai_beta/loader/__pycache__/tubes.cpython-312.pyc` & `miner_ai_beta-0.1.9/miner_ai_beta/loader/__pycache__/tubes.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `miner_ai_beta-0.1.8/miner_ai_beta/loader/__pycache__/union.cpython-312.pyc` & `miner_ai_beta-0.1.9/miner_ai_beta/loader/__pycache__/union.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `miner_ai_beta-0.1.8/miner_ai_beta/loader/__pycache__/web_pages.cpython-312.pyc` & `miner_ai_beta-0.1.9/miner_ai_beta/loader/__pycache__/web_pages.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `miner_ai_beta-0.1.8/miner_ai_beta/loader/__pycache__/xlss.cpython-311.pyc` & `miner_ai_beta-0.1.9/miner_ai_beta/loader/__pycache__/xlss.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `miner_ai_beta-0.1.8/miner_ai_beta/loader/__pycache__/xlss.cpython-312.pyc` & `miner_ai_beta-0.1.9/miner_ai_beta/loader/__pycache__/xlss.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `miner_ai_beta-0.1.8/miner_ai_beta/loader/docs.py` & `miner_ai_beta-0.1.9/miner_ai_beta/loader/docs.py`

 * *Files identical despite different names*

### Comparing `miner_ai_beta-0.1.8/miner_ai_beta/loader/excels.py` & `miner_ai_beta-0.1.9/miner_ai_beta/loader/excels.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,20 +24,21 @@
     text_splitter = RecursiveCharacterTextSplitter(chunk_size=chunk_size, chunk_overlap=0, length_function=len, is_separator_regex=False) # FIXED
 
     documents = []
     # Process each PDF file
     for xls_file in tqdm(xls_files, "Parsing excels"):
         super_text = ""
         sheets_dict = pd.read_excel(os.path.join(folder_path, xls_file), sheet_name=None)
+        print(f"Processing: {xls_file}")
         for sheet_name, df in sheets_dict.items():
+            print(f" - {sheet_name}")
             total_text = df.to_string()
             super_text += total_text   
 
         super_text = re.sub('[\s+]', ' ', super_text) 
-        print(super_text)       
         texts = text_splitter.split_text(super_text)
 
         for text in texts:
             document = Document(page_content=text, metadata={"title": xls_file, "sheet": sheet_name, "type": "xls", "tags": ["document", "table"]})
             documents.append(document)
```

### Comparing `miner_ai_beta-0.1.8/miner_ai_beta/loader/pdfs.py` & `miner_ai_beta-0.1.9/miner_ai_beta/loader/pdfs.py`

 * *Files identical despite different names*

### Comparing `miner_ai_beta-0.1.8/miner_ai_beta/loader/ppts.py` & `miner_ai_beta-0.1.9/miner_ai_beta/loader/ppts.py`

 * *Files identical despite different names*

### Comparing `miner_ai_beta-0.1.8/miner_ai_beta/loader/tubes.py` & `miner_ai_beta-0.1.9/miner_ai_beta/loader/tubes.py`

 * *Files identical despite different names*

### Comparing `miner_ai_beta-0.1.8/miner_ai_beta/loader/web_pages.py` & `miner_ai_beta-0.1.9/miner_ai_beta/loader/web_pages.py`

 * *Files identical despite different names*

### Comparing `miner_ai_beta-0.1.8/pyproject.toml` & `miner_ai_beta-0.1.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "miner-ai-beta"
-version = "0.1.8"
+version = "0.1.9"
 description = ""
 license = "MIT"
 authors = ["Valerio Domenici <valeriodomenici93@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/Valerio357/miner-ai"
 keywords = ["langchain", "documents_mining", "web_scraping"]
```

### Comparing `miner_ai_beta-0.1.8/README.md` & `miner_ai_beta-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `miner_ai_beta-0.1.8/PKG-INFO` & `miner_ai_beta-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miner-ai-beta
-Version: 0.1.8
+Version: 0.1.9
 Summary: 
 Home-page: https://github.com/Valerio357/miner-ai
 License: MIT
 Keywords: langchain,documents_mining,web_scraping
 Author: Valerio Domenici
 Author-email: valeriodomenici93@gmail.com
 Requires-Python: >=3.11,<4.0
```

