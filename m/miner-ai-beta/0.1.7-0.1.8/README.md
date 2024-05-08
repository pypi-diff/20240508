# Comparing `tmp/miner_ai_beta-0.1.7.tar.gz` & `tmp/miner_ai_beta-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "miner_ai_beta-0.1.7.tar", max compression
+gzip compressed data, was "miner_ai_beta-0.1.8.tar", max compression
```

## Comparing `miner_ai_beta-0.1.7.tar` & `miner_ai_beta-0.1.8.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0    11357 2024-05-04 16:49:23.857900 miner_ai_beta-0.1.7/LICENSE
--rw-r--r--   0        0        0      242 2024-05-04 16:59:21.199649 miner_ai_beta-0.1.7/miner_ai_beta/loader/__init__.py
--rw-r--r--   0        0        0      473 2024-05-04 16:04:57.185499 miner_ai_beta-0.1.7/miner_ai_beta/loader/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0     3042 2024-05-04 15:17:18.873214 miner_ai_beta-0.1.7/miner_ai_beta/loader/__pycache__/docs.cpython-311.pyc
--rw-r--r--   0        0        0     2372 2024-05-04 16:04:57.189700 miner_ai_beta-0.1.7/miner_ai_beta/loader/__pycache__/docs.cpython-312.pyc
--rw-r--r--   0        0        0     2299 2024-05-04 16:04:58.283790 miner_ai_beta-0.1.7/miner_ai_beta/loader/__pycache__/excels.cpython-312.pyc
--rw-r--r--   0        0        0     3252 2024-05-04 15:17:18.945722 miner_ai_beta-0.1.7/miner_ai_beta/loader/__pycache__/pages.cpython-311.pyc
--rw-r--r--   0        0        0     2566 2024-05-04 15:17:18.984762 miner_ai_beta-0.1.7/miner_ai_beta/loader/__pycache__/pages.cpython-312.pyc
--rw-r--r--   0        0        0     3161 2024-05-04 15:17:19.027542 miner_ai_beta-0.1.7/miner_ai_beta/loader/__pycache__/pdfs.cpython-311.pyc
--rw-r--r--   0        0        0     2309 2024-05-04 16:05:00.319553 miner_ai_beta-0.1.7/miner_ai_beta/loader/__pycache__/pdfs.cpython-312.pyc
--rw-r--r--   0        0        0     2165 2024-05-04 16:05:00.402279 miner_ai_beta-0.1.7/miner_ai_beta/loader/__pycache__/ppts.cpython-312.pyc
--rw-r--r--   0        0        0     2343 2024-05-04 16:05:00.331906 miner_ai_beta-0.1.7/miner_ai_beta/loader/__pycache__/tubes.cpython-312.pyc
--rw-r--r--   0        0        0      711 2024-05-04 16:05:00.626643 miner_ai_beta-0.1.7/miner_ai_beta/loader/__pycache__/union.cpython-312.pyc
--rw-r--r--   0        0        0     2455 2024-05-04 16:05:00.139759 miner_ai_beta-0.1.7/miner_ai_beta/loader/__pycache__/web_pages.cpython-312.pyc
--rw-r--r--   0        0        0     2928 2024-05-04 15:17:19.188416 miner_ai_beta-0.1.7/miner_ai_beta/loader/__pycache__/xlss.cpython-311.pyc
--rw-r--r--   0        0        0     2490 2024-05-04 15:17:19.226637 miner_ai_beta-0.1.7/miner_ai_beta/loader/__pycache__/xlss.cpython-312.pyc
--rw-r--r--   0        0        0     1753 2024-05-06 15:23:37.641122 miner_ai_beta-0.1.7/miner_ai_beta/loader/docs.py
--rw-r--r--   0        0        0     1833 2024-05-06 17:03:34.920234 miner_ai_beta-0.1.7/miner_ai_beta/loader/excels.py
--rw-r--r--   0        0        0     1713 2024-05-06 15:23:39.870469 miner_ai_beta-0.1.7/miner_ai_beta/loader/pdfs.py
--rw-r--r--   0        0        0     1798 2024-05-06 15:23:36.444442 miner_ai_beta-0.1.7/miner_ai_beta/loader/ppts.py
--rw-r--r--   0        0        0     1821 2024-05-06 15:23:35.159300 miner_ai_beta-0.1.7/miner_ai_beta/loader/tubes.py
--rw-r--r--   0        0        0      361 2024-05-04 15:52:12.917924 miner_ai_beta-0.1.7/miner_ai_beta/loader/union.py
--rw-r--r--   0        0        0     1873 2024-05-06 15:23:32.901218 miner_ai_beta-0.1.7/miner_ai_beta/loader/web_pages.py
--rw-r--r--   0        0        0      668 2024-05-06 17:04:00.394568 miner_ai_beta-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     3966 2024-05-05 07:06:38.721971 miner_ai_beta-0.1.7/README.md
--rw-r--r--   0        0        0     4832 1970-01-01 00:00:00.000000 miner_ai_beta-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-04 16:49:23.857900 miner_ai_beta-0.1.8/LICENSE
+-rw-r--r--   0        0        0      242 2024-05-04 16:59:21.199649 miner_ai_beta-0.1.8/miner_ai_beta/loader/__init__.py
+-rw-r--r--   0        0        0      473 2024-05-04 16:04:57.185499 miner_ai_beta-0.1.8/miner_ai_beta/loader/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0     3042 2024-05-04 15:17:18.873214 miner_ai_beta-0.1.8/miner_ai_beta/loader/__pycache__/docs.cpython-311.pyc
+-rw-r--r--   0        0        0     2372 2024-05-04 16:04:57.189700 miner_ai_beta-0.1.8/miner_ai_beta/loader/__pycache__/docs.cpython-312.pyc
+-rw-r--r--   0        0        0     2299 2024-05-04 16:04:58.283790 miner_ai_beta-0.1.8/miner_ai_beta/loader/__pycache__/excels.cpython-312.pyc
+-rw-r--r--   0        0        0     3252 2024-05-04 15:17:18.945722 miner_ai_beta-0.1.8/miner_ai_beta/loader/__pycache__/pages.cpython-311.pyc
+-rw-r--r--   0        0        0     2566 2024-05-04 15:17:18.984762 miner_ai_beta-0.1.8/miner_ai_beta/loader/__pycache__/pages.cpython-312.pyc
+-rw-r--r--   0        0        0     3161 2024-05-04 15:17:19.027542 miner_ai_beta-0.1.8/miner_ai_beta/loader/__pycache__/pdfs.cpython-311.pyc
+-rw-r--r--   0        0        0     2309 2024-05-04 16:05:00.319553 miner_ai_beta-0.1.8/miner_ai_beta/loader/__pycache__/pdfs.cpython-312.pyc
+-rw-r--r--   0        0        0     2165 2024-05-04 16:05:00.402279 miner_ai_beta-0.1.8/miner_ai_beta/loader/__pycache__/ppts.cpython-312.pyc
+-rw-r--r--   0        0        0     2343 2024-05-04 16:05:00.331906 miner_ai_beta-0.1.8/miner_ai_beta/loader/__pycache__/tubes.cpython-312.pyc
+-rw-r--r--   0        0        0      711 2024-05-04 16:05:00.626643 miner_ai_beta-0.1.8/miner_ai_beta/loader/__pycache__/union.cpython-312.pyc
+-rw-r--r--   0        0        0     2455 2024-05-04 16:05:00.139759 miner_ai_beta-0.1.8/miner_ai_beta/loader/__pycache__/web_pages.cpython-312.pyc
+-rw-r--r--   0        0        0     2928 2024-05-04 15:17:19.188416 miner_ai_beta-0.1.8/miner_ai_beta/loader/__pycache__/xlss.cpython-311.pyc
+-rw-r--r--   0        0        0     2490 2024-05-04 15:17:19.226637 miner_ai_beta-0.1.8/miner_ai_beta/loader/__pycache__/xlss.cpython-312.pyc
+-rw-r--r--   0        0        0     1804 2024-05-08 02:22:00.293266 miner_ai_beta-0.1.8/miner_ai_beta/loader/docs.py
+-rw-r--r--   0        0        0     1915 2024-05-08 02:22:00.295487 miner_ai_beta-0.1.8/miner_ai_beta/loader/excels.py
+-rw-r--r--   0        0        0     1760 2024-05-08 02:22:00.298503 miner_ai_beta-0.1.8/miner_ai_beta/loader/pdfs.py
+-rw-r--r--   0        0        0     1805 2024-05-08 02:22:00.299662 miner_ai_beta-0.1.8/miner_ai_beta/loader/ppts.py
+-rw-r--r--   0        0        0     1895 2024-05-08 02:22:00.300684 miner_ai_beta-0.1.8/miner_ai_beta/loader/tubes.py
+-rw-r--r--   0        0        0      361 2024-05-04 15:52:12.917924 miner_ai_beta-0.1.8/miner_ai_beta/loader/union.py
+-rw-r--r--   0        0        0     1873 2024-05-06 15:23:32.901218 miner_ai_beta-0.1.8/miner_ai_beta/loader/web_pages.py
+-rw-r--r--   0        0        0      668 2024-05-08 02:23:26.746441 miner_ai_beta-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     3966 2024-05-05 07:06:38.721971 miner_ai_beta-0.1.8/README.md
+-rw-r--r--   0        0        0     4883 1970-01-01 00:00:00.000000 miner_ai_beta-0.1.8/PKG-INFO
```

### Comparing `miner_ai_beta-0.1.7/LICENSE` & `miner_ai_beta-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `miner_ai_beta-0.1.7/miner_ai_beta/loader/__pycache__/docs.cpython-311.pyc` & `miner_ai_beta-0.1.8/miner_ai_beta/loader/__pycache__/docs.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `miner_ai_beta-0.1.7/miner_ai_beta/loader/__pycache__/docs.cpython-312.pyc` & `miner_ai_beta-0.1.8/miner_ai_beta/loader/__pycache__/docs.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `miner_ai_beta-0.1.7/miner_ai_beta/loader/__pycache__/excels.cpython-312.pyc` & `miner_ai_beta-0.1.8/miner_ai_beta/loader/__pycache__/excels.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `miner_ai_beta-0.1.7/miner_ai_beta/loader/__pycache__/pages.cpython-311.pyc` & `miner_ai_beta-0.1.8/miner_ai_beta/loader/__pycache__/pages.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `miner_ai_beta-0.1.7/miner_ai_beta/loader/__pycache__/pages.cpython-312.pyc` & `miner_ai_beta-0.1.8/miner_ai_beta/loader/__pycache__/pages.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `miner_ai_beta-0.1.7/miner_ai_beta/loader/__pycache__/pdfs.cpython-311.pyc` & `miner_ai_beta-0.1.8/miner_ai_beta/loader/__pycache__/pdfs.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `miner_ai_beta-0.1.7/miner_ai_beta/loader/__pycache__/pdfs.cpython-312.pyc` & `miner_ai_beta-0.1.8/miner_ai_beta/loader/__pycache__/pdfs.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `miner_ai_beta-0.1.7/miner_ai_beta/loader/__pycache__/ppts.cpython-312.pyc` & `miner_ai_beta-0.1.8/miner_ai_beta/loader/__pycache__/ppts.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `miner_ai_beta-0.1.7/miner_ai_beta/loader/__pycache__/tubes.cpython-312.pyc` & `miner_ai_beta-0.1.8/miner_ai_beta/loader/__pycache__/tubes.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `miner_ai_beta-0.1.7/miner_ai_beta/loader/__pycache__/union.cpython-312.pyc` & `miner_ai_beta-0.1.8/miner_ai_beta/loader/__pycache__/union.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `miner_ai_beta-0.1.7/miner_ai_beta/loader/__pycache__/web_pages.cpython-312.pyc` & `miner_ai_beta-0.1.8/miner_ai_beta/loader/__pycache__/web_pages.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `miner_ai_beta-0.1.7/miner_ai_beta/loader/__pycache__/xlss.cpython-311.pyc` & `miner_ai_beta-0.1.8/miner_ai_beta/loader/__pycache__/xlss.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `miner_ai_beta-0.1.7/miner_ai_beta/loader/__pycache__/xlss.cpython-312.pyc` & `miner_ai_beta-0.1.8/miner_ai_beta/loader/__pycache__/xlss.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `miner_ai_beta-0.1.7/miner_ai_beta/loader/docs.py` & `miner_ai_beta-0.1.8/miner_ai_beta/loader/docs.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,45 +1,45 @@
-import os
-import docx
-from langchain.text_splitter import RecursiveCharacterTextSplitter
-from langchain.docstore.document import Document
-from tqdm import tqdm
-
-
-def IndexFromDocs(folder_path: str, embeddings, vectorstore, chunk_size: int = 2000):
-    """
-    ### Load documents from folder
-    This function loads documents from a folder and creates a Fass index (db).\n
-    - folder_path: Path to folder containing PDFs\n
-    - chunk_size: Chunk size in characters (default 2000)\n
-    - embeddings: Embeddings object from langchain.embeddings\n
-    - vectorstore: could be FAISS or ChromaDB\n
-    """
-
-    # Assuming your PDFs are in a folder named 'test_pdfs'
-    doc_files = [f for f in os.listdir(folder_path) if f.endswith('.docx')]
-
-    documents = []
-    # Process each PDF file and split into chunks of 24000 characters
-    text_splitter = RecursiveCharacterTextSplitter(chunk_size=chunk_size, chunk_overlap=0, length_function=len, is_separator_regex=False) # FIXED
-
-    super_text = ""
-    documents = []
-    # Process each PDF file
-    for doc_file in tqdm(doc_files, "Parsing docs"):
-        doc = docx.Document(os.path.join(folder_path, doc_file))
-        fullText = []
-        for para in doc.paragraphs:
-            fullText.append(para.text)
-        super_text += '\n'.join(fullText)   
-        print(f"Doc '{doc_file}' ingested")
-
-        texts = text_splitter.split_text(super_text)
-
-        for text in texts:
-            document = Document(page_content=text, metadata={"title": doc_file, "link": "", "type": "document"})
-            documents.append(document)
-
-    # Store Embeddings in FAISS
-    for i in tqdm(range(0,1), "Creating db from documents"):
-        db = vectorstore.from_documents(documents, embeddings)
-    return db
+import os
+import docx
+from langchain.text_splitter import RecursiveCharacterTextSplitter
+from langchain.docstore.document import Document
+from tqdm import tqdm
+
+
+def IndexFromDocs(folder_path: str, embeddings, vectorstore, chunk_size: int = 2000):
+    """
+    ### Load documents from folder
+    This function loads documents from a folder and creates a Fass index (db).\n
+    - folder_path: Path to folder containing PDFs\n
+    - chunk_size: Chunk size in characters (default 2000)\n
+    - embeddings: Embeddings object from langchain.embeddings\n
+    - vectorstore: could be FAISS or ChromaDB\n
+    """
+
+    # Assuming your PDFs are in a folder named 'test_pdfs'
+    doc_files = [f for f in os.listdir(folder_path) if f.endswith('.docx')]
+
+    documents = []
+    # Process each PDF file and split into chunks of 24000 characters
+    text_splitter = RecursiveCharacterTextSplitter(chunk_size=chunk_size, chunk_overlap=0, length_function=len, is_separator_regex=False) # FIXED
+
+    super_text = ""
+    documents = []
+    # Process each PDF file
+    for doc_file in tqdm(doc_files, "Parsing docs"):
+        doc = docx.Document(os.path.join(folder_path, doc_file))
+        fullText = []
+        for para in doc.paragraphs:
+            fullText.append(para.text)
+        super_text += '\n'.join(fullText)   
+        print(f"Doc '{doc_file}' ingested")
+
+        texts = text_splitter.split_text(super_text)
+
+        for text in texts:
+            document = Document(page_content=text, metadata={"title": doc_file, "type": "docx", "tags": ["document"]})
+            documents.append(document)
+
+    # Store Embeddings in FAISS
+    for i in tqdm(range(0,1), "Creating db from documents"):
+        db = vectorstore.from_documents(documents, embeddings)
+    return db
```

### Comparing `miner_ai_beta-0.1.7/miner_ai_beta/loader/excels.py` & `miner_ai_beta-0.1.8/miner_ai_beta/loader/excels.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,47 +1,47 @@
-import os
-from langchain.text_splitter import RecursiveCharacterTextSplitter
-from langchain.docstore.document import Document
-import pandas as pd
-from tqdm import tqdm
-import re
-
-def IndexFromXlss(folder_path: str, embeddings, vectorstore, chunk_size: int = 2000):
-    """
-    ## Load excel from folder
-    This function loads documents from a folder and creates a Fass index (db).\n
-    - folder_path: Path to folder containing PDFs\n
-    - chunk_size: Chunk size in characters (default 2000)\n
-    - embeddings: Embeddings object from langchain.embeddings\n
-    - vectorstore: could be FAISS or ChromaDB\n
-    """
-
-
-    # Assuming your PDFs are in a folder named 'test_pdfs'
-    xls_files = [f for f in os.listdir(folder_path) if f.endswith('.xlsx')]
-
-    documents = []
-    # Process each PDF file and split into chunks of 24000 characters
-    text_splitter = RecursiveCharacterTextSplitter(chunk_size=chunk_size, chunk_overlap=0, length_function=len, is_separator_regex=False) # FIXED
-
-    documents = []
-    # Process each PDF file
-    for xls_file in tqdm(xls_files, "Parsing excels"):
-        super_text = ""
-        sheets_dict = pd.read_excel(os.path.join(folder_path, xls_file), sheet_name=None)
-        for sheet_name, df in sheets_dict.items():
-            total_text = df.to_string()
-            super_text += total_text   
-
-        super_text = re.sub('[\s+]', ' ', super_text) 
-        print(super_text)       
-        texts = text_splitter.split_text(super_text)
-
-        for text in texts:
-            document = Document(page_content=text, metadata={"title": xls_file, "link": "", "type": "document"})
-            documents.append(document)
-
-
-    # Store Embeddings in FAISS
-    for i in tqdm(range(0,1), "Creating db from documents"):  
-        db = vectorstore.from_documents(documents, embeddings)
-    return db
+import os
+from langchain.text_splitter import RecursiveCharacterTextSplitter
+from langchain.docstore.document import Document
+import pandas as pd
+from tqdm import tqdm
+import re
+
+def IndexFromXlss(folder_path: str, embeddings, vectorstore, chunk_size: int = 2000):
+    """
+    ## Load excel from folder
+    This function loads documents from a folder and creates a Fass index (db).\n
+    - folder_path: Path to folder containing PDFs\n
+    - chunk_size: Chunk size in characters (default 2000)\n
+    - embeddings: Embeddings object from langchain.embeddings\n
+    - vectorstore: could be FAISS or ChromaDB\n
+    """
+
+
+    # Assuming your PDFs are in a folder named 'test_pdfs'
+    xls_files = [f for f in os.listdir(folder_path) if f.endswith('.xlsx')]
+
+    documents = []
+    # Process each PDF file and split into chunks of 24000 characters
+    text_splitter = RecursiveCharacterTextSplitter(chunk_size=chunk_size, chunk_overlap=0, length_function=len, is_separator_regex=False) # FIXED
+
+    documents = []
+    # Process each PDF file
+    for xls_file in tqdm(xls_files, "Parsing excels"):
+        super_text = ""
+        sheets_dict = pd.read_excel(os.path.join(folder_path, xls_file), sheet_name=None)
+        for sheet_name, df in sheets_dict.items():
+            total_text = df.to_string()
+            super_text += total_text   
+
+        super_text = re.sub('[\s+]', ' ', super_text) 
+        print(super_text)       
+        texts = text_splitter.split_text(super_text)
+
+        for text in texts:
+            document = Document(page_content=text, metadata={"title": xls_file, "sheet": sheet_name, "type": "xls", "tags": ["document", "table"]})
+            documents.append(document)
+
+
+    # Store Embeddings in FAISS
+    for i in tqdm(range(0,1), "Creating db from documents"):  
+        db = vectorstore.from_documents(documents, embeddings)
+    return db
```

### Comparing `miner_ai_beta-0.1.7/miner_ai_beta/loader/pdfs.py` & `miner_ai_beta-0.1.8/miner_ai_beta/loader/pdfs.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-import os
-import pdfplumber
-from langchain.text_splitter import RecursiveCharacterTextSplitter
-from langchain.docstore.document import Document
-from tqdm import tqdm
-
-def IndexFromPdfs(folder_path: str, embeddings, vectorstore, chunk_size: int = 2000):
-    """
-    ### Load pdf from folder
-    this function loads documents from a folder and creates a Fass index (db).\n
-    - folder_path: Path to folder containing PDFs\n
-    - chunk_size: Chunk size in characters (default 2000)\n
-    - embeddings: Embeddings object from langchain.embeddings\n
-    - vectorstore: could be FAISS or ChromaDB\n
-    """
-
-    # Assuming your PDFs are in a folder named 'test_pdfs'
-    pdf_files = [f for f in os.listdir(folder_path) if f.endswith('.pdf')]
-
-    documents = []
-    # Process each PDF file and split into chunks of 24000 characters
-    text_splitter = RecursiveCharacterTextSplitter(chunk_size=chunk_size, chunk_overlap=0, length_function=len, is_separator_regex=False) # FIXED
-
-    documents = []
-    # Process each PDF file
-    for pdf_file in tqdm(pdf_files, "Parsing pdfs"):
-        with pdfplumber.open(os.path.join(folder_path, pdf_file)) as pdf:
-            total_text = ''
-            for page in pdf.pages:
-                total_text += page.extract_text() or ''  # Extract text from each page
-        
-        texts = text_splitter.split_text(total_text)
-
-        for text in texts:
-            document = Document(page_content=text, metadata={"title": pdf_file, "link": "", "type": "document"})
-            documents.append(document)
-
-
-    # Store Embeddings in FAISS
-    for i in tqdm(range(0,1), "Creating db from documents"):
-        db = vectorstore.from_documents(documents, embeddings)
-    return db
+import os
+import pdfplumber
+from langchain.text_splitter import RecursiveCharacterTextSplitter
+from langchain.docstore.document import Document
+from tqdm import tqdm
+
+def IndexFromPdfs(folder_path: str, embeddings, vectorstore, chunk_size: int = 2000):
+    """
+    ### Load pdf from folder
+    this function loads documents from a folder and creates a Fass index (db).\n
+    - folder_path: Path to folder containing PDFs\n
+    - chunk_size: Chunk size in characters (default 2000)\n
+    - embeddings: Embeddings object from langchain.embeddings\n
+    - vectorstore: could be FAISS or ChromaDB\n
+    """
+
+    # Assuming your PDFs are in a folder named 'test_pdfs'
+    pdf_files = [f for f in os.listdir(folder_path) if f.endswith('.pdf')]
+
+    documents = []
+    # Process each PDF file and split into chunks of 24000 characters
+    text_splitter = RecursiveCharacterTextSplitter(chunk_size=chunk_size, chunk_overlap=0, length_function=len, is_separator_regex=False) # FIXED
+
+    documents = []
+    # Process each PDF file
+    for pdf_file in tqdm(pdf_files, "Parsing pdfs"):
+        with pdfplumber.open(os.path.join(folder_path, pdf_file)) as pdf:
+            total_text = ''
+            for page in pdf.pages:
+                total_text += page.extract_text() or ''  # Extract text from each page
+        
+        texts = text_splitter.split_text(total_text)
+
+        for text in texts:
+            document = Document(page_content=text, metadata={"title": pdf_file, "type": "pdf", "tags": ["document"]})
+            documents.append(document)
+
+
+    # Store Embeddings in FAISS
+    for i in tqdm(range(0,1), "Creating db from documents"):
+        db = vectorstore.from_documents(documents, embeddings)
+    return db
```

### Comparing `miner_ai_beta-0.1.7/miner_ai_beta/loader/ppts.py` & `miner_ai_beta-0.1.8/miner_ai_beta/loader/ppts.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,15 +30,15 @@
             for shape in slide.shapes:
                 if shape.has_text_frame:
                     total_text += str(shape.text) # Extract text from each page
         
         texts = text_splitter.split_text(total_text)
 
         for text in texts:
-            document = Document(page_content=text, metadata={"title": ppt_file, "link": "", "type": "document"})
+            document = Document(page_content=text, metadata={"title": ppt_file, "type": "pptx", "tags" : ["document"]})
             documents.append(document)
 
 
     # Store Embeddings in FAISS
     for i in tqdm(range(0,1), "Creating db from documents"):
         db = vectorstore.from_documents(documents, embeddings)
     return db
```

### Comparing `miner_ai_beta-0.1.7/miner_ai_beta/loader/tubes.py` & `miner_ai_beta-0.1.8/miner_ai_beta/loader/tubes.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,46 +1,46 @@
-from langchain.text_splitter import RecursiveCharacterTextSplitter
-from langchain.docstore.document import Document
-from pytube import YouTube
-from youtube_transcript_api import YouTubeTranscriptApi
-import datetime
-from tqdm import tqdm
-
-def IndexFromTubes(tubes: list[str], embeddings, vectorstore, chunk_size: int = 2000):
-    """
-    ### Load pdf from folder
-    This function loads documents from a folder and creates a Fass index (db).\n
-    - pages: webpage ('https') to load inside index\n
-    - chunk_size: Chunk size in characters (default 2000)\n
-    - embeddings: Embeddings object from langchain.embeddings\n
-    - vectorstore: could be FAISS or ChromaDB\n
-    """
-
-    documents = []
-    # Process each PDF file and split into chunks of 24000 characters
-    text_splitter = RecursiveCharacterTextSplitter(chunk_size=chunk_size, chunk_overlap=0, length_function=len, is_separator_regex=False) # FIXED
-
-    
-    documents = []
-    total_text = ""
-
-    # Example usage
-    for tube in tqdm(tubes,"Parsing videos"):
-        title = YouTube(tube).title
-        tube_id = tube.split("https://www.youtube.com/watch?v=")[1] 
-        transcripts = YouTubeTranscriptApi.get_transcript(tube_id)
-        for transcript in transcripts:
-            time = datetime.timedelta(0,transcript["start"])
-            current_text = transcript["text"]
-            total_text += f"text: {current_text}, at: {time}\n"
-            
-        texts = text_splitter.split_text(total_text)
-
-        for text in texts:
-            document = Document(page_content=text, metadata={"title": title, "link": tube, "type": "video"})
-            documents.append(document)
-
-
-    # Store Embeddings in FAISS
-    for i in tqdm(range(0,1), "Creating db from documents"):
-        db = vectorstore.from_documents(documents, embeddings)
-    return db
+from langchain.text_splitter import RecursiveCharacterTextSplitter
+from langchain.docstore.document import Document
+from pytube import YouTube
+from youtube_transcript_api import YouTubeTranscriptApi
+import datetime
+from tqdm import tqdm
+
+def IndexFromTubes(tubes: list[str], embeddings, vectorstore, chunk_size: int = 2000):
+    """
+    ### Load pdf from folder
+    This function loads documents from a folder and creates a Fass index (db).\n
+    - pages: webpage ('https') to load inside index\n
+    - chunk_size: Chunk size in characters (default 2000)\n
+    - embeddings: Embeddings object from langchain.embeddings\n
+    - vectorstore: could be FAISS or ChromaDB\n
+    """
+
+    documents = []
+    # Process each PDF file and split into chunks of 24000 characters
+    text_splitter = RecursiveCharacterTextSplitter(chunk_size=chunk_size, chunk_overlap=0, length_function=len, is_separator_regex=False) # FIXED
+
+    
+    documents = []
+    total_text = ""
+
+    # Example usage
+    for tube in tqdm(tubes,"Parsing videos"):
+        title = YouTube(tube).title
+        tube_id = tube.split("https://www.youtube.com/watch?v=")[1] 
+        transcripts = YouTubeTranscriptApi.get_transcript(tube_id)
+        for transcript in transcripts:
+            time = datetime.timedelta(0,transcript["start"])
+            current_text = transcript["text"]
+            total_text += f"text: {current_text}, at: {time}\n"
+            
+        texts = text_splitter.split_text(total_text)
+
+        for text in texts:
+            document = Document(page_content=text, metadata={"title": title, "link": tube, "type": "mp4", "tags": ["video", "caption"]})
+            documents.append(document)
+
+
+    # Store Embeddings in FAISS
+    for i in tqdm(range(0,1), "Creating db from documents"):
+        db = vectorstore.from_documents(documents, embeddings)
+    return db
```

### Comparing `miner_ai_beta-0.1.7/miner_ai_beta/loader/web_pages.py` & `miner_ai_beta-0.1.8/miner_ai_beta/loader/web_pages.py`

 * *Files identical despite different names*

### Comparing `miner_ai_beta-0.1.7/pyproject.toml` & `miner_ai_beta-0.1.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "miner-ai-beta"
-version = "0.1.7"
+version = "0.1.8"
 description = ""
 license = "MIT"
 authors = ["Valerio Domenici <valeriodomenici93@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/Valerio357/miner-ai"
 keywords = ["langchain", "documents_mining", "web_scraping"]
 
 
 [tool.poetry.dependencies]
-python = "^3.12"
+python = "^3.11"
 tqdm = "^4.66.4"
 python-pptx = "^0.6.23"
 pytube = "^15.0.0"
 youtube-transcript-api = "^0.6.2"
 langchain-openai = "^0.1.6"
 langchain = "^0.1.17"
 bs4 = "^0.0.2"
```

### Comparing `miner_ai_beta-0.1.7/README.md` & `miner_ai_beta-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `miner_ai_beta-0.1.7/PKG-INFO` & `miner_ai_beta-0.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: miner-ai-beta
-Version: 0.1.7
+Version: 0.1.8
 Summary: 
 Home-page: https://github.com/Valerio357/miner-ai
 License: MIT
 Keywords: langchain,documents_mining,web_scraping
 Author: Valerio Domenici
 Author-email: valeriodomenici93@gmail.com
-Requires-Python: >=3.12,<4.0
+Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: bs4 (>=0.0.2,<0.0.3)
 Requires-Dist: langchain (>=0.1.17,<0.2.0)
 Requires-Dist: langchain-openai (>=0.1.6,<0.2.0)
 Requires-Dist: openpyxl (>=3.1.2,<4.0.0)
 Requires-Dist: python-docx (>=1.1.2,<2.0.0)
 Requires-Dist: python-pptx (>=0.6.23,<0.7.0)
```

