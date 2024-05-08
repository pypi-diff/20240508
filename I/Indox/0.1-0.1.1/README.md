# Comparing `tmp/Indox-0.1.tar.gz` & `tmp/Indox-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Indox-0.1.tar", last modified: Fri Apr 19 19:12:20 2024, max compression
+gzip compressed data, was "Indox-0.1.1.tar", last modified: Wed May  8 13:36:50 2024, max compression
```

## Comparing `Indox-0.1.tar` & `Indox-0.1.1.tar`

### file list

```diff
@@ -1,22 +1,31 @@
-drwxrwxrwx   0        0        0        0 2024-04-19 19:12:20.942990 Indox-0.1/
-drwxrwxrwx   0        0        0        0 2024-04-19 19:12:20.940307 Indox-0.1/Indox/
--rw-rw-rw-   0        0        0     6312 2024-04-17 12:16:41.000000 Indox-0.1/Indox/Clustering.py
--rw-rw-rw-   0        0        0     2148 2024-04-17 12:16:41.000000 Indox-0.1/Indox/Embedding.py
--rw-rw-rw-   0        0        0     8364 2024-04-19 08:28:13.000000 Indox-0.1/Indox/Indox.py
--rw-rw-rw-   0        0        0     2493 2024-04-17 12:16:41.000000 Indox-0.1/Indox/QAModels.py
--rw-rw-rw-   0        0        0     2297 2024-04-17 16:18:06.000000 Indox-0.1/Indox/Summary.py
--rw-rw-rw-   0        0        0       68 2024-04-16 13:31:54.000000 Indox-0.1/Indox/__init__.py
--rw-rw-rw-   0        0        0      428 2024-04-19 18:48:48.000000 Indox-0.1/Indox/config.yaml
--rw-rw-rw-   0        0        0     5701 2024-04-19 10:22:25.000000 Indox-0.1/Indox/utils.py
--rw-rw-rw-   0        0        0     5941 2024-04-18 08:32:40.000000 Indox-0.1/Indox/vectorstore.py
-drwxrwxrwx   0        0        0        0 2024-04-19 19:12:20.938132 Indox-0.1/Indox.egg-info/
--rw-rw-rw-   0        0        0      683 2024-04-19 19:12:20.000000 Indox-0.1/Indox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      335 2024-04-19 19:12:20.000000 Indox-0.1/Indox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 19:12:20.000000 Indox-0.1/Indox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      152 2024-04-19 19:12:20.000000 Indox-0.1/Indox.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-04-19 19:12:20.000000 Indox-0.1/Indox.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       44 2024-04-19 10:39:00.000000 Indox-0.1/MANIFEST.in
--rw-rw-rw-   0        0        0      683 2024-04-19 19:12:20.940475 Indox-0.1/PKG-INFO
--rw-rw-rw-   0        0        0     3596 2024-04-19 09:06:28.000000 Indox-0.1/README.md
--rw-rw-rw-   0        0        0       42 2024-04-19 19:12:20.944023 Indox-0.1/setup.cfg
--rw-rw-rw-   0        0        0     1266 2024-04-19 19:08:17.000000 Indox-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 13:36:50.042721 Indox-0.1.1/
+drwxrwxrwx   0        0        0        0 2024-05-08 13:36:49.925356 Indox-0.1.1/Indox/
+-rw-rw-rw-   0        0        0     3548 2024-05-08 10:23:44.000000 Indox-0.1.1/Indox/Embedding.py
+-rw-rw-rw-   0        0        0     2453 2024-05-08 10:23:44.000000 Indox-0.1.1/Indox/Graph.py
+-rw-rw-rw-   0        0        0    12884 2024-05-08 10:23:44.000000 Indox-0.1.1/Indox/Indox.py
+-rw-rw-rw-   0        0        0     5666 2024-05-08 13:25:13.000000 Indox-0.1.1/Indox/QAModels.py
+-rw-rw-rw-   0        0        0    12574 2024-05-08 10:23:44.000000 Indox-0.1.1/Indox/Splitter.py
+-rw-rw-rw-   0        0        0     2959 2024-05-08 10:23:44.000000 Indox-0.1.1/Indox/Summary.py
+-rw-rw-rw-   0        0        0       66 2024-05-08 13:01:56.000000 Indox-0.1.1/Indox/__init__.py
+-rw-rw-rw-   0        0        0      593 2024-05-08 10:23:44.000000 Indox-0.1.1/Indox/clean.py
+drwxrwxrwx   0        0        0        0 2024-05-08 13:36:50.022400 Indox-0.1.1/Indox/cluster/
+-rw-rw-rw-   0        0        0     6348 2024-05-08 10:23:44.000000 Indox-0.1.1/Indox/cluster/Clustering.py
+-rw-rw-rw-   0        0        0     4685 2024-05-08 10:23:44.000000 Indox-0.1.1/Indox/cluster/EmbedClusterSummarize.py
+-rw-rw-rw-   0        0        0        0 2024-05-08 13:08:42.000000 Indox-0.1.1/Indox/cluster/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 13:36:50.037432 Indox-0.1.1/Indox/metrics/
+-rw-rw-rw-   0        0        0        0 2024-05-08 13:08:54.000000 Indox-0.1.1/Indox/metrics/__init__.py
+-rw-rw-rw-   0        0        0     4114 2024-05-08 10:23:44.000000 Indox-0.1.1/Indox/metrics/metrics.py
+-rw-rw-rw-   0        0        0    10055 2024-05-08 13:08:27.000000 Indox-0.1.1/Indox/metrics/unieval.py
+-rw-rw-rw-   0        0        0     8837 2024-05-08 10:23:44.000000 Indox-0.1.1/Indox/utils.py
+-rw-rw-rw-   0        0        0     5358 2024-05-08 10:23:44.000000 Indox-0.1.1/Indox/vectorstore.py
+drwxrwxrwx   0        0        0        0 2024-05-08 13:36:49.952967 Indox-0.1.1/Indox.egg-info/
+-rw-rw-rw-   0        0        0      685 2024-05-08 13:36:49.000000 Indox-0.1.1/Indox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      514 2024-05-08 13:36:49.000000 Indox-0.1.1/Indox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 13:36:49.000000 Indox-0.1.1/Indox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      440 2024-05-08 13:36:49.000000 Indox-0.1.1/Indox.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-08 13:36:49.000000 Indox-0.1.1/Indox.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       44 2024-05-08 10:23:44.000000 Indox-0.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      685 2024-05-08 13:36:50.037432 Indox-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     8204 2024-05-08 10:23:44.000000 Indox-0.1.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-08 13:36:50.043746 Indox-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1023 2024-05-08 13:36:43.000000 Indox-0.1.1/setup.py
```

### Comparing `Indox-0.1/Indox/Clustering.py` & `Indox-0.1.1/Indox/cluster/Clustering.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 import umap
 from sklearn.mixture import GaussianMixture
 
 RANDOM_SEED = 42  # Fixed seed for reproducibility
 
 
 def global_cluster_embeddings(
-    embeddings: np.ndarray,
-    dim: int,
-    n_neighbors: Optional[int] = None,
-    metric: str = "cosine",
+        embeddings: np.ndarray,
+        dim: int,
+        n_neighbors: Optional[int] = None,
+        metric: str = "cosine",
 ) -> np.ndarray:
     """
     Perform global dimensionality reduction on the embeddings using UMAP.
 
     Parameters:
     - embeddings: The input embeddings as a numpy array.
     - dim: The target dimensionality for the reduced space.
@@ -29,15 +29,15 @@
         n_neighbors = int((len(embeddings) - 1) ** 0.5)
     return umap.UMAP(
         n_neighbors=n_neighbors, n_components=dim, metric=metric
     ).fit_transform(embeddings)
 
 
 def local_cluster_embeddings(
-    embeddings: np.ndarray, dim: int, num_neighbors: int = 10, metric: str = "cosine"
+        embeddings: np.ndarray, dim: int, num_neighbors: int = 10, metric: str = "cosine"
 ) -> np.ndarray:
     """
     Perform local dimensionality reduction on the embeddings using UMAP, typically after global clustering.
 
     Parameters:
     - embeddings: The input embeddings as a numpy array.
     - dim: The target dimensionality for the reduced space.
@@ -49,15 +49,15 @@
     """
     return umap.UMAP(
         n_neighbors=num_neighbors, n_components=dim, metric=metric
     ).fit_transform(embeddings)
 
 
 def get_optimal_clusters(
-    embeddings: np.ndarray, max_clusters: int = 50, random_state: int = RANDOM_SEED
+        embeddings: np.ndarray, max_clusters: int = 50, random_state: int = RANDOM_SEED
 ):
     """
     Determine the optimal number of clusters using the Bayesian Information Criterion (BIC) with a Gaussian Mixture Model.
 
     Parameters:
     - embeddings: The input embeddings as a numpy array.
     - max_clusters: The maximum number of clusters to consider.
@@ -74,15 +74,15 @@
         gm.fit(embeddings)
         bics.append(gm.bic(embeddings))
     return n_clusters[np.argmin(bics)]
 
 
 def GMM_cluster(embeddings: np.ndarray, threshold: float, random_state: int = 0):
     """
-    Cluster embeddings using a Gaussian Mixture Model (GMM) based on a probability threshold.
+    cluster embeddings using a Gaussian Mixture Model (GMM) based on a probability threshold.
 
     Parameters:
     - embeddings: The input embeddings as a numpy array.
     - threshold: The probability threshold for assigning an embedding to a cluster.
     - random_state: Seed for reproducibility.
 
     Returns:
@@ -93,17 +93,17 @@
     gm.fit(embeddings)
     probs = gm.predict_proba(embeddings)
     labels = [np.where(prob > threshold)[0] for prob in probs]
     return labels, n_clusters
 
 
 def perform_clustering(
-    embeddings: np.ndarray,
-    dim: int,
-    threshold: float,
+        embeddings: np.ndarray,
+        dim: int,
+        threshold: float,
 ) -> List[np.ndarray]:
     """
     Perform clustering on the embeddings by first reducing their dimensionality globally, then clustering
     using a Gaussian Mixture Model, and finally performing local clustering within each global cluster.
 
     Parameters:
     - embeddings: The input embeddings as a numpy array.
```

### Comparing `Indox-0.1/Indox/vectorstore.py` & `Indox-0.1.1/Indox/vectorstore.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,160 +1,140 @@
 from abc import ABC, abstractmethod
 from typing import Iterable
 from langchain_community.vectorstores.pgvector import PGVector
+from langchain_community.vectorstores.pgvector import DistanceStrategy as PGDistancesTRATEGY
 from langchain_community.vectorstores.chroma import Chroma
+from langchain_community.vectorstores.faiss import FAISS
+from langchain_community.vectorstores.utils import DistanceStrategy
+from langchain.docstore.in_memory import InMemoryDocstore
+import faiss
 import logging
 from .utils import read_config, construct_postgres_connection_string
 
 logging.basicConfig(
     format="%(asctime)s - %(levelname)s - %(message)s", level=logging.INFO
 )
 
+
 class VectorStoreBase(ABC):
     """Abstract base class defining the interface for vector-based document stores."""
 
     @abstractmethod
-    def add_document(self, texts):
-        """Add documents to the vector store.
-
-        Args:
-            texts (Iterable[str]): An iterable containing the text of the documents to be added.
-        
-        Raises:
-            RuntimeError: If there's an issue adding documents to the vector store.
-        """
+    def add_document(self, texts, unstructured):
+        """Add documents to the vector store."""
         pass
 
     @abstractmethod
-    def retrieve(self, query: str):
-        """Retrieve documents similar to the given query from the vector store.
-
-        Args:
-            query (str): The query text.
-            top_k (int, optional): The number of top similar documents to retrieve. Defaults to 5.
-
-        Returns:
-            tuple: A tuple containing lists of retrieved document contexts and their similarity scores.
-        """
+    def retrieve(self, query: str, top_k: int = 5):
+        """Retrieve documents similar to the given query from the vector store."""
         pass
 
+    def as_retriever(self, ):
+        """Return the vectorstore as retriever."""
+        return self.db.as_retriever()
 
-class PGVectorStore(VectorStoreBase):
-    """A concrete implementation of VectorStoreBase using PostgreSQL for storage."""
 
-    def __init__(self, conn_string, collection_name, embedding) -> None:
-        """Initialize the PGVectorStore.
+class PGVectorStore(VectorStoreBase):
+    """A concrete implementation using PostgreSQL for storage."""
 
-        Args:
-            conn_string (str): Connection string for PostgreSQL database.
-            collection_name (str): Name of the collection/table in the database.
-            embedding: Embedding function for vectorization.
-        """
-        
+    def __init__(self, conn_string, collection_name, embedding):
         super().__init__()
-        self.db = PGVector(
-                embedding_function=embedding,
-                collection_name=collection_name,
-                connection_string=conn_string,
-            )
-
-    def add_document(self, texts: Iterable[str]):
-        """Add documents to the PostgreSQL vector store.
-
-        Args:
-            texts (Iterable[str]): An iterable containing the text of the documents to be added.
-        
-        Raises:
-            RuntimeError: If there's an issue adding documents to the vector store.
-        """
+        self.db = PGVector(embedding_function=embedding, collection_name=collection_name,
+                           connection_string=conn_string, distance_strategy=PGDistancesTRATEGY.COSINE)
 
+    def add_document(self, docs, unstructured):
         try:
-            self.db.add_texts(texts)
-            logging.info(f"document added successfuly to the vector store")
-        except:
-            raise RuntimeError("Can't add document to the vector store")
-        
-    def retrieve(self, query: str, top_k: int = 5):
-        """Retrieve documents similar to the given query from the PostgreSQL vector store.
-
-        Args:
-            query (str): The query text.
-            top_k (int, optional): The number of top similar documents to retrieve. Defaults to 5.
-
-        Returns:
-            tuple: A tuple containing lists of retrieved document contexts and their similarity scores.
-        """
+            if unstructured:
+                self.db.add_documents(docs)
+            elif not unstructured:
+                self.db.add_texts(docs)
+            logging.info("Document added successfully to the vector store.")
+        except Exception as e:
+            logging.error(f"Failed to add document: {e}")
+            raise RuntimeError(f"Can't add document to the vector store: {e}")
 
+    def retrieve(self, query: str, top_k: int = 5):
         retrieved = self.db.similarity_search_with_score(query, k=top_k)
         context = [d[0].page_content for d in retrieved]
         scores = [d[1] for d in retrieved]
         return context, scores
 
+
 class ChromaVectorStore(VectorStoreBase):
-    """A concrete implementation of VectorStoreBase using Chroma for storage."""
-    def __init__(self, collection_name, embedding) -> None:
-        """Initialize the ChromaVectorStore.
-
-        Args:
-            collection_name (str): Name of the collection/table in Chroma.
-            embedding: Embedding function for vectorization.
-        """
+    """A concrete implementation using Chroma for storage."""
 
+    def __init__(self, collection_name, embedding):
         super().__init__()
-        self.db = Chroma(collection_name=collection_name,
-                          embedding_function=embedding)
-    
-    def add_document(self, texts: Iterable[str]):
-        """Add documents to the Chroma vector store.
-
-        Args:
-            texts (Iterable[str]): An iterable containing the text of the documents to be added.
-        
-        Raises:
-            RuntimeError: If there's an issue adding documents to the vector store.
-        """
+        self.db = Chroma(collection_name=collection_name, embedding_function=embedding)
 
+    def add_document(self, docs, unstructured):
         try:
-            self.db.add_texts(texts)
-            logging.info(f"document added successfuly to the vector store")
-        except:
-            raise RuntimeError("Can't add document to the vector store")
-    
+            if unstructured:
+                self.db.add_documents(documents=docs)
+            elif not unstructured:
+                self.db.add_texts(texts=docs)
+            logging.info("Document added successfully to the vector store.")
+        except Exception as e:
+            logging.error(f"Failed to add document: {e}")
+            raise RuntimeError(f"Can't add document to the vector store: {e}")
+
     def retrieve(self, query: str, top_k: int = 5):
-        """Retrieve documents similar to the given query from the Chroma vector store.
+        retrieved = self.db.similarity_search_with_score(query, k=top_k)
+        context = [d[0].page_content for d in retrieved]
+        scores = [d[1] for d in retrieved]
+        return context, scores
+
+
+class FAISSVectorStore(VectorStoreBase):
+    """implementation using FAISS for storage."""
+    def __init__(self, embedding) -> None:
+
+        super().__init__()
+
+        embedding_dim = len(embedding.embed_query(""))
+
+        index = faiss.IndexFlatL2(embedding_dim)
 
-        Args:
-            query (str): The query text.
-            top_k (int, optional): The number of top similar documents to retrieve. Defaults to 5.
-
-        Returns:
-            tuple: A tuple containing lists of retrieved document contexts and their similarity scores.
-        """
+        docstore = InMemoryDocstore({})
 
+        index_to_docstore_id = {}
+
+        self.db = FAISS(
+            embedding,
+            index,
+            docstore,
+            index_to_docstore_id,
+            relevance_score_fn=None,
+            normalize_L2=False,
+            distance_strategy=DistanceStrategy.COSINE
+        )
+
+    def add_document(self, docs, unstructured):
+
+        try:
+            if unstructured:
+                self.db.add_documents(docs)
+            elif not unstructured:
+                self.db.add_texts(docs)
+            logging.info("Document added successfully to the vector store.")
+        except Exception as e:
+            logging.error(f"Failed to add document: {e}")
+            raise RuntimeError(f"Can't add document to the vector store: {e}")
+
+    def retrieve(self, query: str, top_k: int = 5):
         retrieved = self.db.similarity_search_with_score(query, k=top_k)
         context = [d[0].page_content for d in retrieved]
         scores = [d[1] for d in retrieved]
         return context, scores
 
-        
-def get_vector_store(collection_name, embeddings):
-    """Factory function to get an instance of VectorStoreBase based on configuration.
-
-    Args:
-        collection_name (str): Name of the collection/table in the database.
-        embeddings: Embedding function for vectorization.
-
-    Returns:
-        VectorStoreBase: An instance of VectorStoreBase.
-    """
 
+def get_vector_store(embeddings, collection_name: str):
     config = read_config()
-    if config['vector_store'] == 'pgvector':
+    if config['vector_store'].lower() == 'pgvector':
         conn_string = construct_postgres_connection_string()
-        db = PGVectorStore(conn_string=conn_string,
-                                collection_name=collection_name,
-                                embedding=embeddings)
+        return PGVectorStore(conn_string=conn_string, collection_name=collection_name,
+                             embedding=embeddings)
+    elif config['vector_store'].lower() == 'chroma':
+        return ChromaVectorStore(collection_name=collection_name, embedding=embeddings)
+    elif config['vector_store'].lower() == 'faiss':
+        db = FAISSVectorStore(embedding=embeddings)
         return db
-    elif config['vector_store'] == 'chroma':
-        db = ChromaVectorStore(collection_name=collection_name,
-                                embedding=embeddings)
-        return db
```

### Comparing `Indox-0.1/Indox.egg-info/PKG-INFO` & `Indox-0.1.1/Indox.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Indox
-Version: 0.1
+Version: 0.1.1
 Summary: Indox Retrieval Augmentation
 Home-page: https://github.com/osllmai/inDox
 Author: nerdstudio
 Author-email: Mohammad@nematifamilyfundation.onmicrosoft.com
 License: MIT
 Keywords: RAG,LLM
 Platform: UNKNOWN
```

### Comparing `Indox-0.1/PKG-INFO` & `Indox-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Indox
-Version: 0.1
+Version: 0.1.1
 Summary: Indox Retrieval Augmentation
 Home-page: https://github.com/osllmai/inDox
 Author: nerdstudio
 Author-email: Mohammad@nematifamilyfundation.onmicrosoft.com
 License: MIT
 Keywords: RAG,LLM
 Platform: UNKNOWN
```

### Comparing `Indox-0.1/setup.py` & `Indox-0.1.1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,42 +1,30 @@
 from setuptools import setup, find_packages
+with open('requirements.txt') as f:
+    requirements = f.read().splitlines()
+
+packages = [req.split('==')[0] for req in requirements]
 
 setup(
-  name = 'Indox',        
-  version = '0.1',      
-  license='MIT',      
+  name='Indox',
+  version='0.1.1',
+  license='MIT',
   packages=find_packages(),
   package_data={'Indox': ['config.yaml']},
-  include_package_data=True,  
-  description = 'Indox Retrieval Augmentation',   
-  author = 'nerdstudio',                  
-  author_email = 'Mohammad@nematifamilyfundation.onmicrosoft.com',    
-  url = 'https://github.com/osllmai/inDox',   
-  keywords = ['RAG', 'LLM'],   
-  install_requires=[           
-          'langchain_community',
-        'numpy',
-        'openai',
-        'pandas',
-        'PyPDF2',
-        'scikit_learn',
-        'tenacity',
-        'tiktoken',
-        'umap_learn',
-        'transformers',
-        'black',
-        'chromadb',
-        'psycopg2',
-        'pgvector',
-        'langchain-openai'
-      ],
+  include_package_data=True,
+  description='Indox Retrieval Augmentation',
+  author='nerdstudio',
+  author_email='Mohammad@nematifamilyfundation.onmicrosoft.com',
+  url='https://github.com/osllmai/inDox',
+  keywords=['RAG', 'LLM'],
+  install_requires=packages,  # Use extracted packages from requirements.txt
   classifiers=[
-    'Development Status :: 3 - Alpha',     
-    'Intended Audience :: Developers',     
+    'Development Status :: 3 - Alpha',
+    'Intended Audience :: Developers',
     'Topic :: Software Development :: Build Tools',
-    'License :: OSI Approved :: MIT License',   
-    'Programming Language :: Python :: 3',     
+    'License :: OSI Approved :: MIT License',
+    'Programming Language :: Python :: 3',
     'Programming Language :: Python :: 3.4',
     'Programming Language :: Python :: 3.5',
     'Programming Language :: Python :: 3.6',
   ],
 )
```

