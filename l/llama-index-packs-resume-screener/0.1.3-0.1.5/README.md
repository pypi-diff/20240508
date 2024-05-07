# Comparing `tmp/llama_index_packs_resume_screener-0.1.3.tar.gz` & `tmp/llama_index_packs_resume_screener-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_packs_resume_screener-0.1.3.tar", max compression
+gzip compressed data, was "llama_index_packs_resume_screener-0.1.5.tar", max compression
```

## Comparing `llama_index_packs_resume_screener-0.1.3.tar` & `llama_index_packs_resume_screener-0.1.5.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     2023 2024-02-13 13:53:02.232873 llama_index_packs_resume_screener-0.1.3/README.md
--rw-r--r--   0        0        0      104 2024-02-13 13:53:02.233121 llama_index_packs_resume_screener-0.1.3/llama_index/packs/resume_screener/__init__.py
--rw-r--r--   0        0        0     2775 2024-02-13 13:53:02.233190 llama_index_packs_resume_screener-0.1.3/llama_index/packs/resume_screener/base.py
--rw-r--r--   0        0        0     1633 2024-02-22 01:34:11.904425 llama_index_packs_resume_screener-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     2859 1970-01-01 00:00:00.000000 llama_index_packs_resume_screener-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     2023 2024-05-07 22:47:11.086521 llama_index_packs_resume_screener-0.1.5/README.md
+-rw-r--r--   0        0        0      104 2024-05-07 22:47:11.086521 llama_index_packs_resume_screener-0.1.5/llama_index/packs/resume_screener/__init__.py
+-rw-r--r--   0        0        0     2799 2024-05-07 22:47:11.086521 llama_index_packs_resume_screener-0.1.5/llama_index/packs/resume_screener/base.py
+-rw-r--r--   0        0        0     1635 2024-05-07 22:47:11.086521 llama_index_packs_resume_screener-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     2810 1970-01-01 00:00:00.000000 llama_index_packs_resume_screener-0.1.5/PKG-INFO
```

### Comparing `llama_index_packs_resume_screener-0.1.3/README.md` & `llama_index_packs_resume_screener-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `llama_index_packs_resume_screener-0.1.3/llama_index/packs/resume_screener/base.py` & `llama_index_packs_resume_screener-0.1.5/llama_index/packs/resume_screener/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from llama_index.core import ServiceContext
 from llama_index.core.llama_pack.base import BaseLlamaPack
 from llama_index.core.response_synthesizers import TreeSummarize
 from llama_index.core.schema import NodeWithScore
 from llama_index.llms.openai import OpenAI
 from llama_index.readers.file import PDFReader
-from pydantic import BaseModel, Field
+from llama_index.core.bridge.pydantic import BaseModel, Field
 
 # backwards compatibility
 try:
     from llama_index.core.llms.llm import LLM
 except ImportError:
     from llama_index.core.llms.base import LLM
```

### Comparing `llama_index_packs_resume_screener-0.1.3/pyproject.toml` & `llama_index_packs_resume_screener-0.1.5/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -25,22 +25,22 @@
 description = "llama-index packs resume_screener integration"
 exclude = ["**/BUILD"]
 keywords = ["document", "pdf", "resume", "structured output"]
 license = "MIT"
 maintainers = ["Disiok"]
 name = "llama-index-packs-resume-screener"
 readme = "README.md"
-version = "0.1.3"
+version = "0.1.5"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
-llama-index-core = "^0.10.1"
+llama-index-core = "^0.10.24"
 pypdf = "^4.0.1"
 llama-index-readers-file = "^0.1.1"
-llama-index-llms-openai = "^0.1.1"
+llama-index-llms-openai = "^0.1.13"
 
 [tool.poetry.group.dev.dependencies]
 ipython = "8.10.0"
 jupyter = "^1.0.0"
 mypy = "0.991"
 pre-commit = "3.2.0"
 pylint = "2.15.10"
```

### Comparing `llama_index_packs_resume_screener-0.1.3/PKG-INFO` & `llama_index_packs_resume_screener-0.1.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: llama-index-packs-resume-screener
-Version: 0.1.3
+Version: 0.1.5
 Summary: llama-index packs resume_screener integration
 License: MIT
 Keywords: document,pdf,resume,structured output
 Author: Your Name
 Author-email: you@example.com
 Maintainer: Disiok
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: llama-index-core (>=0.10.1,<0.11.0)
-Requires-Dist: llama-index-llms-openai (>=0.1.1,<0.2.0)
+Requires-Dist: llama-index-core (>=0.10.24,<0.11.0)
+Requires-Dist: llama-index-llms-openai (>=0.1.13,<0.2.0)
 Requires-Dist: llama-index-readers-file (>=0.1.1,<0.2.0)
 Requires-Dist: pypdf (>=4.0.1,<5.0.0)
 Description-Content-Type: text/markdown
 
 # Resumer Screener Pack
 
 This LlamaPack loads a resume file, and review it against a user specified job description and screening criteria.
```

