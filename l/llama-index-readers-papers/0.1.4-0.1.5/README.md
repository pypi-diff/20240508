# Comparing `tmp/llama_index_readers_papers-0.1.4.tar.gz` & `tmp/llama_index_readers_papers-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_readers_papers-0.1.4.tar", max compression
+gzip compressed data, was "llama_index_readers_papers-0.1.5.tar", max compression
```

## Comparing `llama_index_readers_papers-0.1.4.tar` & `llama_index_readers_papers-0.1.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     2398 2024-03-28 16:18:25.476516 llama_index_readers_papers-0.1.4/README.md
--rw-r--r--   0        0        0      186 2024-03-28 16:18:25.476516 llama_index_readers_papers-0.1.4/llama_index/readers/papers/__init__.py
--rw-r--r--   0        0        0      186 2024-03-28 16:18:25.476516 llama_index_readers_papers-0.1.4/llama_index/readers/papers/arxiv/__init__.py
--rw-r--r--   0        0        0     6214 2024-03-28 16:18:25.476516 llama_index_readers_papers-0.1.4/llama_index/readers/papers/arxiv/base.py
--rw-r--r--   0        0        0       17 2024-03-28 16:18:25.476516 llama_index_readers_papers-0.1.4/llama_index/readers/papers/pubmed/__init__.py
--rw-r--r--   0        0        0     6330 2024-03-28 16:18:25.476516 llama_index_readers_papers-0.1.4/llama_index/readers/papers/pubmed/base.py
--rw-r--r--   0        0        0     1517 2024-03-28 16:18:25.476516 llama_index_readers_papers-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     3015 1970-01-01 00:00:00.000000 llama_index_readers_papers-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     2008 2024-05-08 15:19:55.056380 llama_index_readers_papers-0.1.5/README.md
+-rw-r--r--   0        0        0      186 2024-05-08 15:19:55.056380 llama_index_readers_papers-0.1.5/llama_index/readers/papers/__init__.py
+-rw-r--r--   0        0        0      186 2024-05-08 15:19:55.056380 llama_index_readers_papers-0.1.5/llama_index/readers/papers/arxiv/__init__.py
+-rw-r--r--   0        0        0     6302 2024-05-08 15:19:55.056380 llama_index_readers_papers-0.1.5/llama_index/readers/papers/arxiv/base.py
+-rw-r--r--   0        0        0       17 2024-05-08 15:19:55.056380 llama_index_readers_papers-0.1.5/llama_index/readers/papers/pubmed/__init__.py
+-rw-r--r--   0        0        0     6330 2024-05-08 15:19:55.056380 llama_index_readers_papers-0.1.5/llama_index/readers/papers/pubmed/base.py
+-rw-r--r--   0        0        0     1517 2024-05-08 15:19:55.056380 llama_index_readers_papers-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     2625 1970-01-01 00:00:00.000000 llama_index_readers_papers-0.1.5/PKG-INFO
```

### Comparing `llama_index_readers_papers-0.1.4/README.md` & `llama_index_readers_papers-0.1.5/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+Metadata-Version: 2.1
+Name: llama-index-readers-papers
+Version: 0.1.5
+Summary: llama-index readers papers integration
+License: MIT
+Author: Your Name
+Author-email: you@example.com
+Maintainer: thejessezhang
+Requires-Python: >=3.8.1,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: arxiv (>=2.1.0,<3.0.0)
+Requires-Dist: llama-index-core (>=0.10.1,<0.11.0)
+Description-Content-Type: text/markdown
+
 # Papers Loaders
 
 ```bash
 pip install llama-index-readers-papers
 ```
 
 ## Arxiv Papers Loader
@@ -26,15 +44,15 @@
 
 loader = ArxivReader()
 documents, abstracts = loader.load_papers_and_abstracts(
     search_query="au:Karpathy"
 )
 ```
 
-This loader is designed to be used as a way to load data into [LlamaIndex](https://github.com/run-llama/llama_index/tree/main/llama_index) and/or subsequently used as a Tool in a [LangChain](https://github.com/hwchase17/langchain) Agent. See [here](https://github.com/emptycrown/llama-hub/tree/main) for examples.
+This loader is designed to be used as a way to load data into [LlamaIndex](https://github.com/run-llama/llama_index/).
 
 ## Pubmed Papers Loader
 
 This loader fetches the text from the most relevant scientific papers on Pubmed specified by a search query (e.g. "Alzheimers"). For each paper, the abstract is included in the `Document`. The search query may be any string.
 
 ## Usage
 
@@ -43,8 +61,9 @@
 ```python
 from llama_index.readers.papers import PubmedReader
 
 loader = PubmedReader()
 documents = loader.load_data(search_query="amyloidosis")
 ```
 
-This loader is designed to be used as a way to load data into [LlamaIndex](https://github.com/run-llama/llama_index/tree/main/llama_index) and/or subsequently used as a Tool in a [LangChain](https://github.com/hwchase17/langchain) Agent. See [here](https://github.com/emptycrown/llama-hub/tree/main) for examples.
+This loader is designed to be used as a way to load data into [LlamaIndex](https://github.com/run-llama/llama_index/).
+
```

### Comparing `llama_index_readers_papers-0.1.4/llama_index/readers/papers/arxiv/base.py` & `llama_index_readers_papers-0.1.5/llama_index/readers/papers/arxiv/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,15 +69,17 @@
             paper.download_pdf(dirpath=papers_dir, filename=filename)
             logging.debug(f"> Downloading {filename}...")
 
         def get_paper_metadata(filename):
             return paper_lookup[os.path.basename(filename)]
 
         arxiv_documents = SimpleDirectoryReader(
-            papers_dir, file_metadata=get_paper_metadata
+            papers_dir,
+            file_metadata=get_paper_metadata,
+            exclude_hidden=False,  # default directory is hidden ".papers"
         ).load_data()
         # Include extra documents containing the abstracts
         abstract_documents = []
         for paper in search_results:
             d = (
                 f"The following is a summary of the paper: {paper.title}\n\nSummary:"
                 f" {paper.summary}"
```

### Comparing `llama_index_readers_papers-0.1.4/llama_index/readers/papers/pubmed/base.py` & `llama_index_readers_papers-0.1.5/llama_index/readers/papers/pubmed/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_readers_papers-0.1.4/pyproject.toml` & `llama_index_readers_papers-0.1.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 authors = ["Your Name <you@example.com>"]
 description = "llama-index readers papers integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 maintainers = ["thejessezhang"]
 name = "llama-index-readers-papers"
 readme = "README.md"
-version = "0.1.4"
+version = "0.1.5"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.1"
 arxiv = "^2.1.0"
 
 [tool.poetry.group.dev.dependencies]
```

