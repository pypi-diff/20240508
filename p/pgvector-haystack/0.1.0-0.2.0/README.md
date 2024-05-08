# Comparing `tmp/pgvector_haystack-0.1.0.tar.gz` & `tmp/pgvector_haystack-0.2.0.tar.gz`

## Comparing `pgvector_haystack-0.1.0.tar` & `pgvector_haystack-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,20 @@
--rw-r--r--   0        0        0     2517 2020-02-02 00:00:00.000000 pgvector_haystack-0.1.0/examples/example.py
--rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 pgvector_haystack-0.1.0/pydoc/config.yml
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 pgvector_haystack-0.1.0/src/haystack_integrations/components/retrievers/pgvector/__init__.py
--rw-r--r--   0        0        0     4536 2020-02-02 00:00:00.000000 pgvector_haystack-0.1.0/src/haystack_integrations/components/retrievers/pgvector/embedding_retriever.py
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 pgvector_haystack-0.1.0/src/haystack_integrations/document_stores/pgvector/__init__.py
--rw-r--r--   0        0        0    22749 2020-02-02 00:00:00.000000 pgvector_haystack-0.1.0/src/haystack_integrations/document_stores/pgvector/document_store.py
--rw-r--r--   0        0        0     8139 2020-02-02 00:00:00.000000 pgvector_haystack-0.1.0/src/haystack_integrations/document_stores/pgvector/filters.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 pgvector_haystack-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 pgvector_haystack-0.1.0/tests/conftest.py
--rw-r--r--   0        0        0     9199 2020-02-02 00:00:00.000000 pgvector_haystack-0.1.0/tests/test_document_store.py
--rw-r--r--   0        0        0     6009 2020-02-02 00:00:00.000000 pgvector_haystack-0.1.0/tests/test_embedding_retrieval.py
--rw-r--r--   0        0        0     8085 2020-02-02 00:00:00.000000 pgvector_haystack-0.1.0/tests/test_filters.py
--rw-r--r--   0        0        0     5304 2020-02-02 00:00:00.000000 pgvector_haystack-0.1.0/tests/test_retriever.py
--rw-r--r--   0        0        0     1866 2020-02-02 00:00:00.000000 pgvector_haystack-0.1.0/.gitignore
--rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 pgvector_haystack-0.1.0/LICENSE.txt
--rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 pgvector_haystack-0.1.0/README.md
--rw-r--r--   0        0        0     3871 2020-02-02 00:00:00.000000 pgvector_haystack-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 pgvector_haystack-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     2577 2020-02-02 00:00:00.000000 pgvector_haystack-0.2.0/examples/embedding_retrieval.py
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 pgvector_haystack-0.2.0/pydoc/config.yml
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 pgvector_haystack-0.2.0/src/haystack_integrations/components/retrievers/pgvector/__init__.py
+-rw-r--r--   0        0        0     6523 2020-02-02 00:00:00.000000 pgvector_haystack-0.2.0/src/haystack_integrations/components/retrievers/pgvector/embedding_retriever.py
+-rw-r--r--   0        0        0     4624 2020-02-02 00:00:00.000000 pgvector_haystack-0.2.0/src/haystack_integrations/components/retrievers/pgvector/keyword_retriever.py
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 pgvector_haystack-0.2.0/src/haystack_integrations/document_stores/pgvector/__init__.py
+-rw-r--r--   0        0        0    27011 2020-02-02 00:00:00.000000 pgvector_haystack-0.2.0/src/haystack_integrations/document_stores/pgvector/document_store.py
+-rw-r--r--   0        0        0     8212 2020-02-02 00:00:00.000000 pgvector_haystack-0.2.0/src/haystack_integrations/document_stores/pgvector/filters.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 pgvector_haystack-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 pgvector_haystack-0.2.0/tests/conftest.py
+-rw-r--r--   0        0        0     8745 2020-02-02 00:00:00.000000 pgvector_haystack-0.2.0/tests/test_document_store.py
+-rw-r--r--   0        0        0     6034 2020-02-02 00:00:00.000000 pgvector_haystack-0.2.0/tests/test_embedding_retrieval.py
+-rw-r--r--   0        0        0     7705 2020-02-02 00:00:00.000000 pgvector_haystack-0.2.0/tests/test_filters.py
+-rw-r--r--   0        0        0     2116 2020-02-02 00:00:00.000000 pgvector_haystack-0.2.0/tests/test_keyword_retrieval.py
+-rw-r--r--   0        0        0     9877 2020-02-02 00:00:00.000000 pgvector_haystack-0.2.0/tests/test_retrievers.py
+-rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 pgvector_haystack-0.2.0/.gitignore
+-rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 pgvector_haystack-0.2.0/LICENSE.txt
+-rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 pgvector_haystack-0.2.0/README.md
+-rw-r--r--   0        0        0     4002 2020-02-02 00:00:00.000000 pgvector_haystack-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 pgvector_haystack-0.2.0/PKG-INFO
```

### Comparing `pgvector_haystack-0.1.0/examples/example.py` & `pgvector_haystack-0.2.0/examples/embedding_retrieval.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,25 +7,25 @@
 # for Markdown conversion and embeddings generation. Use the following command:
 # pip install pgvector-haystack markdown-it-py mdit_plain "sentence-transformers>=2.2.0"
 
 # Download some Markdown files to index.
 # git clone https://github.com/anakin87/neural-search-pills
 
 import glob
-import os
 
 from haystack import Pipeline
 from haystack.components.converters import MarkdownToDocument
 from haystack.components.embedders import SentenceTransformersDocumentEmbedder, SentenceTransformersTextEmbedder
 from haystack.components.preprocessors import DocumentSplitter
 from haystack.components.writers import DocumentWriter
 from haystack_integrations.components.retrievers.pgvector import PgvectorEmbeddingRetriever
 from haystack_integrations.document_stores.pgvector import PgvectorDocumentStore
 
-os.environ["PG_CONN_STR"] = "postgresql://postgres:postgres@localhost:5432/postgres"
+# Set an environment variable `PG_CONN_STR` with the connection string to your PostgreSQL database.
+# e.g., "postgresql://USER:PASSWORD@HOST:PORT/DB_NAME"
 
 # Initialize PgvectorDocumentStore
 document_store = PgvectorDocumentStore(
     table_name="haystack_test",
     embedding_dimension=768,
     vector_function="cosine_similarity",
     recreate_table=True,
```

### Comparing `pgvector_haystack-0.1.0/pydoc/config.yml` & `pgvector_haystack-0.2.0/pydoc/config.yml`

 * *Files 19% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 loaders:
   - type: haystack_pydoc_tools.loaders.CustomPythonLoader
     search_path: [../src]
     modules: [
       "haystack_integrations.components.retrievers.pgvector.embedding_retriever",
       "haystack_integrations.document_stores.pgvector.document_store",
-      "haystack_integrations.document_stores.pgvector.filters",
     ]
     ignore_when_discovered: ["__init__"]
 processors:
   - type: filter
     expression:
     documented_only: true
     do_not_filter_modules: false
     skip_empty_modules: true
   - type: smart
   - type: crossref
 renderer:
-  type: haystack_pydoc_tools.renderers.ReadmePreviewRenderer
+  type: haystack_pydoc_tools.renderers.ReadmeIntegrationRenderer
   excerpt: Pgvector integration for Haystack
-  category_slug: haystack-integrations
+  category_slug: integrations-api
   title: Pgvector
   slug: integrations-pgvector
-  order: 140
+  order: 190
   markdown:
     descriptive_class_title: false
+    classdef_code_block: false
     descriptive_module_title: true
     add_method_class_prefix: true
     add_member_class_prefix: false
     filename: _readme_pgvector.md
```

### Comparing `pgvector_haystack-0.1.0/src/haystack_integrations/document_stores/pgvector/document_store.py` & `pgvector_haystack-0.2.0/src/haystack_integrations/document_stores/pgvector/document_store.py`

 * *Files 9% similar despite different names*

```diff
@@ -49,91 +49,106 @@
 dataframe = EXCLUDED.dataframe,
 blob_data = EXCLUDED.blob_data,
 blob_meta = EXCLUDED.blob_meta,
 blob_mime_type = EXCLUDED.blob_mime_type,
 meta = EXCLUDED.meta
 """
 
+KEYWORD_QUERY = """
+SELECT {table_name}.*, ts_rank_cd(to_tsvector({language}, content), query) AS score
+FROM {table_name}, plainto_tsquery({language}, %s) query
+WHERE to_tsvector({language}, content) @@ query
+"""
+
 VALID_VECTOR_FUNCTIONS = ["cosine_similarity", "inner_product", "l2_distance"]
 
 VECTOR_FUNCTION_TO_POSTGRESQL_OPS = {
     "cosine_similarity": "vector_cosine_ops",
     "inner_product": "vector_ip_ops",
     "l2_distance": "vector_l2_ops",
 }
 
 HNSW_INDEX_CREATION_VALID_KWARGS = ["m", "ef_construction"]
 
 HNSW_INDEX_NAME = "haystack_hnsw_index"
 
+KEYWORD_INDEX_NAME = "haystack_keyword_index"
+
 
 class PgvectorDocumentStore:
+    """
+    A Document Store using PostgreSQL with the [pgvector extension](https://github.com/pgvector/pgvector) installed.
+    """
+
     def __init__(
         self,
         *,
         connection_string: Secret = Secret.from_env_var("PG_CONN_STR"),
         table_name: str = "haystack_documents",
+        language: str = "english",
         embedding_dimension: int = 768,
         vector_function: Literal["cosine_similarity", "inner_product", "l2_distance"] = "cosine_similarity",
         recreate_table: bool = False,
         search_strategy: Literal["exact_nearest_neighbor", "hnsw"] = "exact_nearest_neighbor",
         hnsw_recreate_index_if_exists: bool = False,
         hnsw_index_creation_kwargs: Optional[Dict[str, int]] = None,
         hnsw_ef_search: Optional[int] = None,
     ):
         """
         Creates a new PgvectorDocumentStore instance.
         It is meant to be connected to a PostgreSQL database with the pgvector extension installed.
         A specific table to store Haystack documents will be created if it doesn't exist yet.
 
         :param connection_string: The connection string to use to connect to the PostgreSQL database, defined as an
-            environment variable, e.g.: PG_CONN_STR="postgresql://USER:PASSWORD@HOST:PORT/DB_NAME"
-        :param table_name: The name of the table to use to store Haystack documents. Defaults to "haystack_documents".
-        :param embedding_dimension: The dimension of the embedding. Defaults to 768.
+            environment variable, e.g.: `PG_CONN_STR="postgresql://USER:PASSWORD@HOST:PORT/DB_NAME"`
+        :param table_name: The name of the table to use to store Haystack documents.
+        :param language: The language to be used to parse query and document content in keyword retrieval.
+            To see the list of available languages, you can run the following SQL query in your PostgreSQL database:
+            `SELECT cfgname FROM pg_ts_config;`.
+            More information can be found in this [StackOverflow answer](https://stackoverflow.com/a/39752553).
+        :param embedding_dimension: The dimension of the embedding.
         :param vector_function: The similarity function to use when searching for similar embeddings.
-            Defaults to "cosine_similarity". "cosine_similarity" and "inner_product" are similarity functions and
+            `"cosine_similarity"` and `"inner_product"` are similarity functions and
             higher scores indicate greater similarity between the documents.
-            "l2_distance" returns the straight-line distance between vectors,
+            `"l2_distance"` returns the straight-line distance between vectors,
             and the most similar documents are the ones with the smallest score.
-
-            Important: when using the "hnsw" search strategy, an index will be created that depends on the
+            **Important**: when using the `"hnsw"` search strategy, an index will be created that depends on the
             `vector_function` passed here. Make sure subsequent queries will keep using the same
             vector similarity function in order to take advantage of the index.
-        :type vector_function: Literal["cosine_similarity", "inner_product", "l2_distance"]
-        :param recreate_table: Whether to recreate the table if it already exists. Defaults to False.
+        :param recreate_table: Whether to recreate the table if it already exists.
         :param search_strategy: The search strategy to use when searching for similar embeddings.
-            Defaults to "exact_nearest_neighbor". "hnsw" is an approximate nearest neighbor search strategy,
+            `"exact_nearest_neighbor"` provides perfect recall but can be slow for large numbers of documents.
+            `"hnsw"` is an approximate nearest neighbor search strategy,
             which trades off some accuracy for speed; it is recommended for large numbers of documents.
-
-            Important: when using the "hnsw" search strategy, an index will be created that depends on the
+            **Important**: when using the `"hnsw"` search strategy, an index will be created that depends on the
             `vector_function` passed here. Make sure subsequent queries will keep using the same
             vector similarity function in order to take advantage of the index.
-        :type search_strategy: Literal["exact_nearest_neighbor", "hnsw"]
         :param hnsw_recreate_index_if_exists: Whether to recreate the HNSW index if it already exists.
-            Defaults to False. Only used if search_strategy is set to "hnsw".
+            Only used if search_strategy is set to `"hnsw"`.
         :param hnsw_index_creation_kwargs: Additional keyword arguments to pass to the HNSW index creation.
-            Only used if search_strategy is set to "hnsw". You can find the list of valid arguments in the
-            pgvector documentation: https://github.com/pgvector/pgvector?tab=readme-ov-file#hnsw
-        :param hnsw_ef_search: The ef_search parameter to use at query time. Only used if search_strategy is set to
-            "hnsw". You can find more information about this parameter in the pgvector documentation:
-            https://github.com/pgvector/pgvector?tab=readme-ov-file#hnsw
+            Only used if search_strategy is set to `"hnsw"`. You can find the list of valid arguments in the
+            [pgvector documentation](https://github.com/pgvector/pgvector?tab=readme-ov-file#hnsw)
+        :param hnsw_ef_search: The `ef_search` parameter to use at query time. Only used if search_strategy is set to
+            `"hnsw"`. You can find more information about this parameter in the
+            [pgvector documentation](https://github.com/pgvector/pgvector?tab=readme-ov-file#hnsw).
         """
 
         self.connection_string = connection_string
         self.table_name = table_name
         self.embedding_dimension = embedding_dimension
         if vector_function not in VALID_VECTOR_FUNCTIONS:
             msg = f"vector_function must be one of {VALID_VECTOR_FUNCTIONS}, but got {vector_function}"
             raise ValueError(msg)
         self.vector_function = vector_function
         self.recreate_table = recreate_table
         self.search_strategy = search_strategy
         self.hnsw_recreate_index_if_exists = hnsw_recreate_index_if_exists
         self.hnsw_index_creation_kwargs = hnsw_index_creation_kwargs or {}
         self.hnsw_ef_search = hnsw_ef_search
+        self.language = language
 
         connection = connect(self.connection_string.resolve_value())
         connection.autocommit = True
         self._connection = connection
 
         # we create a generic cursor and another one that returns dictionaries
         self._cursor = connection.cursor()
@@ -141,34 +156,50 @@
 
         connection.execute("CREATE EXTENSION IF NOT EXISTS vector")
         register_vector(connection)
 
         if recreate_table:
             self.delete_table()
         self._create_table_if_not_exists()
+        self._create_keyword_index_if_not_exists()
 
         if search_strategy == "hnsw":
             self._handle_hnsw()
 
     def to_dict(self) -> Dict[str, Any]:
+        """
+        Serializes the component to a dictionary.
+
+        :returns:
+            Dictionary with serialized data.
+        """
         return default_to_dict(
             self,
             connection_string=self.connection_string.to_dict(),
             table_name=self.table_name,
             embedding_dimension=self.embedding_dimension,
             vector_function=self.vector_function,
             recreate_table=self.recreate_table,
             search_strategy=self.search_strategy,
             hnsw_recreate_index_if_exists=self.hnsw_recreate_index_if_exists,
             hnsw_index_creation_kwargs=self.hnsw_index_creation_kwargs,
             hnsw_ef_search=self.hnsw_ef_search,
+            language=self.language,
         )
 
     @classmethod
     def from_dict(cls, data: Dict[str, Any]) -> "PgvectorDocumentStore":
+        """
+        Deserializes the component from a dictionary.
+
+        :param data:
+            Dictionary to deserialize from.
+        :returns:
+            Deserialized component.
+        """
         deserialize_secrets_inplace(data["init_parameters"], ["connection_string"])
         return default_from_dict(cls, data)
 
     def _execute_sql(
         self, sql_query: Query, params: Optional[tuple] = None, error_msg: str = "", cursor: Optional[Cursor] = None
     ):
         """
@@ -205,24 +236,48 @@
         )
 
         self._execute_sql(create_sql, error_msg="Could not create table in PgvectorDocumentStore")
 
     def delete_table(self):
         """
         Deletes the table used to store Haystack documents.
+        The name of the table (`table_name`) is defined when initializing the `PgvectorDocumentStore`.
         """
 
         delete_sql = SQL("DROP TABLE IF EXISTS {table_name}").format(table_name=Identifier(self.table_name))
 
         self._execute_sql(delete_sql, error_msg=f"Could not delete table {self.table_name} in PgvectorDocumentStore")
 
+    def _create_keyword_index_if_not_exists(self):
+        """
+        Internal method to create the keyword index if not exists.
+        """
+        index_exists = bool(
+            self._execute_sql(
+                "SELECT 1 FROM pg_indexes WHERE tablename = %s AND indexname = %s",
+                (self.table_name, KEYWORD_INDEX_NAME),
+                "Could not check if keyword index exists",
+            ).fetchone()
+        )
+
+        sql_create_index = SQL(
+            "CREATE INDEX {index_name} ON {table_name} USING GIN (to_tsvector({language}, content))"
+        ).format(
+            index_name=Identifier(KEYWORD_INDEX_NAME),
+            table_name=Identifier(self.table_name),
+            language=SQLLiteral(self.language),
+        )
+
+        if not index_exists:
+            self._execute_sql(sql_create_index, error_msg="Could not create keyword index on table")
+
     def _handle_hnsw(self):
         """
         Internal method to handle the HNSW index creation.
-        It also sets the hnsw.ef_search parameter for queries if it is specified.
+        It also sets the `hnsw.ef_search` parameter for queries if it is specified.
         """
 
         if self.hnsw_ef_search:
             sql_set_hnsw_ef_search = SQL("SET hnsw.ef_search = {hnsw_ef_search}").format(
                 hnsw_ef_search=SQLLiteral(self.hnsw_ef_search)
             )
             self._execute_sql(sql_set_hnsw_ef_search, error_msg="Could not set hnsw.ef_search")
@@ -291,15 +346,16 @@
         """
         Returns the documents that match the filters provided.
 
         For a detailed specification of the filters,
         refer to the [documentation](https://docs.haystack.deepset.ai/v2.0/docs/metadata-filtering)
 
         :param filters: The filters to apply to the document list.
-        :return: A list of Documents that match the given filters.
+        :raises TypeError: If `filters` is not a dictionary.
+        :returns: A list of Documents that match the given filters.
         """
         if filters:
             if not isinstance(filters, dict):
                 msg = "Filters must be a dictionary"
                 raise TypeError(msg)
             if "operator" not in filters and "conditions" not in filters:
                 filters = convert(filters)
@@ -320,21 +376,21 @@
 
         records = result.fetchall()
         docs = self._from_pg_to_haystack_documents(records)
         return docs
 
     def write_documents(self, documents: List[Document], policy: DuplicatePolicy = DuplicatePolicy.NONE) -> int:
         """
-        Writes documents into to PgvectorDocumentStore.
+        Writes documents to the document store.
 
         :param documents: A list of Documents to write to the document store.
         :param policy: The duplicate policy to use when writing documents.
         :raises DuplicateDocumentError: If a document with the same id already exists in the document store
-             and the policy is set to DuplicatePolicy.FAIL (or not specified).
-        :return: The number of documents written to the document store.
+             and the policy is set to `DuplicatePolicy.FAIL` (or not specified).
+        :returns: The number of documents written to the document store.
         """
 
         if len(documents) > 0:
             if not isinstance(documents[0], Document):
                 msg = "param 'documents' must contain a list of objects of type Document"
                 raise ValueError(msg)
 
@@ -394,14 +450,24 @@
             db_document["blob_data"] = blob.data if blob else None
             db_document["blob_meta"] = Jsonb(blob.meta) if blob and blob.meta else None
             db_document["blob_mime_type"] = blob.mime_type if blob and blob.mime_type else None
 
             db_document["dataframe"] = Jsonb(db_document["dataframe"]) if db_document["dataframe"] else None
             db_document["meta"] = Jsonb(db_document["meta"])
 
+            if "sparse_embedding" in db_document:
+                sparse_embedding = db_document.pop("sparse_embedding", None)
+                if sparse_embedding:
+                    logger.warning(
+                        "Document %s has the `sparse_embedding` field set,"
+                        "but storing sparse embeddings in Pgvector is not currently supported."
+                        "The `sparse_embedding` field will be ignored.",
+                        db_document["id"],
+                    )
+
             db_documents.append(db_document)
 
         return db_documents
 
     @staticmethod
     def _from_pg_to_haystack_documents(documents: List[Dict[str, Any]]) -> List[Document]:
         """
@@ -428,15 +494,15 @@
 
             haystack_documents.append(haystack_document)
 
         return haystack_documents
 
     def delete_documents(self, document_ids: List[str]) -> None:
         """
-        Deletes all documents with a matching document_ids from the document store.
+        Deletes documents that match the provided `document_ids` from the document store.
 
         :param document_ids: the document ids to delete
         """
 
         if not document_ids:
             return
 
@@ -444,30 +510,78 @@
 
         delete_sql = SQL("DELETE FROM {table_name} WHERE id IN ({document_ids_str})").format(
             table_name=Identifier(self.table_name), document_ids_str=SQL(document_ids_str)
         )
 
         self._execute_sql(delete_sql, error_msg="Could not delete documents from PgvectorDocumentStore")
 
+    def _keyword_retrieval(
+        self,
+        query: str,
+        *,
+        filters: Optional[Dict[str, Any]] = None,
+        top_k: int = 10,
+    ) -> List[Document]:
+        """
+        Retrieves documents that are most similar to the query using a full-text search.
+
+        This method is not meant to be part of the public interface of
+        `PgvectorDocumentStore` and it should not be called directly.
+        `PgvectorKeywordRetriever` uses this method directly and is the public interface for it.
+
+        :returns: List of Documents that are most similar to `query`
+        """
+        if not query:
+            msg = "query must be a non-empty string"
+            raise ValueError(msg)
+
+        sql_select = SQL(KEYWORD_QUERY).format(
+            table_name=Identifier(self.table_name),
+            language=SQLLiteral(self.language),
+            query=SQLLiteral(query),
+        )
+
+        where_params = ()
+        sql_where_clause = SQL("")
+        if filters:
+            sql_where_clause, where_params = _convert_filters_to_where_clause_and_params(
+                filters=filters, operator="AND"
+            )
+
+        sql_sort = SQL(" ORDER BY score DESC LIMIT {top_k}").format(top_k=SQLLiteral(top_k))
+
+        sql_query = sql_select + sql_where_clause + sql_sort
+
+        result = self._execute_sql(
+            sql_query,
+            (query, *where_params),
+            error_msg="Could not retrieve documents from PgvectorDocumentStore.",
+            cursor=self._dict_cursor,
+        )
+
+        records = result.fetchall()
+        docs = self._from_pg_to_haystack_documents(records)
+        return docs
+
     def _embedding_retrieval(
         self,
         query_embedding: List[float],
         *,
         filters: Optional[Dict[str, Any]] = None,
         top_k: int = 10,
         vector_function: Optional[Literal["cosine_similarity", "inner_product", "l2_distance"]] = None,
     ) -> List[Document]:
         """
         Retrieves documents that are most similar to the query embedding using a vector similarity metric.
 
         This method is not meant to be part of the public interface of
         `PgvectorDocumentStore` and it should not be called directly.
         `PgvectorEmbeddingRetriever` uses this method directly and is the public interface for it.
-        :raises ValueError
-        :return: List of Documents that are most similar to `query_embedding`
+
+        :returns: List of Documents that are most similar to `query_embedding`
         """
 
         if not query_embedding:
             msg = "query_embedding must be a non-empty list of floats"
             raise ValueError(msg)
         if len(query_embedding) != self.embedding_dimension:
             msg = (
```

### Comparing `pgvector_haystack-0.1.0/src/haystack_integrations/document_stores/pgvector/filters.py` & `pgvector_haystack-0.2.0/src/haystack_integrations/document_stores/pgvector/filters.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # SPDX-FileCopyrightText: 2023-present deepset GmbH <info@deepset.ai>
 #
 # SPDX-License-Identifier: Apache-2.0
 from datetime import datetime
 from itertools import chain
-from typing import Any, Dict, List
+from typing import Any, Dict, List, Literal, Tuple
 
 from haystack.errors import FilterError
 from pandas import DataFrame
 from psycopg.sql import SQL
 from psycopg.types.json import Jsonb
 
 # we need this mapping to cast meta values to the correct type,
@@ -18,30 +18,32 @@
     float: "real",
     bool: "boolean",
 }
 
 NO_VALUE = "no_value"
 
 
-def _convert_filters_to_where_clause_and_params(filters: Dict[str, Any]) -> tuple[SQL, tuple]:
+def _convert_filters_to_where_clause_and_params(
+    filters: Dict[str, Any], operator: Literal["WHERE", "AND"] = "WHERE"
+) -> Tuple[SQL, Tuple]:
     """
     Convert Haystack filters to a WHERE clause and a tuple of params to query PostgreSQL.
     """
     if "field" in filters:
         query, values = _parse_comparison_condition(filters)
     else:
         query, values = _parse_logical_condition(filters)
 
-    where_clause = SQL(" WHERE ") + SQL(query)
+    where_clause = SQL(f" {operator} ") + SQL(query)
     params = tuple(value for value in values if value != NO_VALUE)
 
     return where_clause, params
 
 
-def _parse_logical_condition(condition: Dict[str, Any]) -> tuple[str, List[Any]]:
+def _parse_logical_condition(condition: Dict[str, Any]) -> Tuple[str, List[Any]]:
     if "operator" not in condition:
         msg = f"'operator' key missing in {condition}"
         raise FilterError(msg)
     if "conditions" not in condition:
         msg = f"'conditions' key missing in {condition}"
         raise FilterError(msg)
 
@@ -73,15 +75,15 @@
     else:
         msg = f"Unknown logical operator '{operator}'"
         raise FilterError(msg)
 
     return sql_query, values
 
 
-def _parse_comparison_condition(condition: Dict[str, Any]) -> tuple[str, List[Any]]:
+def _parse_comparison_condition(condition: Dict[str, Any]) -> Tuple[str, List[Any]]:
     field: str = condition["field"]
     if "operator" not in condition:
         msg = f"'operator' key missing in {condition}"
         raise FilterError(msg)
     if "value" not in condition:
         msg = f"'value' key missing in {condition}"
         raise FilterError(msg)
@@ -128,28 +130,28 @@
 
     if type_value:
         field = f"({field})::{type_value}"
 
     return field
 
 
-def _equal(field: str, value: Any) -> tuple[str, Any]:
+def _equal(field: str, value: Any) -> Tuple[str, Any]:
     if value is None:
         # NO_VALUE is a placeholder that will be removed in _convert_filters_to_where_clause_and_params
         return f"{field} IS NULL", NO_VALUE
     return f"{field} = %s", value
 
 
-def _not_equal(field: str, value: Any) -> tuple[str, Any]:
+def _not_equal(field: str, value: Any) -> Tuple[str, Any]:
     # we use IS DISTINCT FROM to correctly handle NULL values
     # (not handled by !=)
     return f"{field} IS DISTINCT FROM %s", value
 
 
-def _greater_than(field: str, value: Any) -> tuple[str, Any]:
+def _greater_than(field: str, value: Any) -> Tuple[str, Any]:
     if isinstance(value, str):
         try:
             datetime.fromisoformat(value)
         except (ValueError, TypeError) as exc:
             msg = (
                 "Can't compare strings using operators '>', '>=', '<', '<='. "
                 "Strings are only comparable if they are ISO formatted dates."
@@ -158,15 +160,15 @@
     if type(value) in [list, Jsonb]:
         msg = f"Filter value can't be of type {type(value)} using operators '>', '>=', '<', '<='"
         raise FilterError(msg)
 
     return f"{field} > %s", value
 
 
-def _greater_than_equal(field: str, value: Any) -> tuple[str, Any]:
+def _greater_than_equal(field: str, value: Any) -> Tuple[str, Any]:
     if isinstance(value, str):
         try:
             datetime.fromisoformat(value)
         except (ValueError, TypeError) as exc:
             msg = (
                 "Can't compare strings using operators '>', '>=', '<', '<='. "
                 "Strings are only comparable if they are ISO formatted dates."
@@ -175,15 +177,15 @@
     if type(value) in [list, Jsonb]:
         msg = f"Filter value can't be of type {type(value)} using operators '>', '>=', '<', '<='"
         raise FilterError(msg)
 
     return f"{field} >= %s", value
 
 
-def _less_than(field: str, value: Any) -> tuple[str, Any]:
+def _less_than(field: str, value: Any) -> Tuple[str, Any]:
     if isinstance(value, str):
         try:
             datetime.fromisoformat(value)
         except (ValueError, TypeError) as exc:
             msg = (
                 "Can't compare strings using operators '>', '>=', '<', '<='. "
                 "Strings are only comparable if they are ISO formatted dates."
@@ -192,15 +194,15 @@
     if type(value) in [list, Jsonb]:
         msg = f"Filter value can't be of type {type(value)} using operators '>', '>=', '<', '<='"
         raise FilterError(msg)
 
     return f"{field} < %s", value
 
 
-def _less_than_equal(field: str, value: Any) -> tuple[str, Any]:
+def _less_than_equal(field: str, value: Any) -> Tuple[str, Any]:
     if isinstance(value, str):
         try:
             datetime.fromisoformat(value)
         except (ValueError, TypeError) as exc:
             msg = (
                 "Can't compare strings using operators '>', '>=', '<', '<='. "
                 "Strings are only comparable if they are ISO formatted dates."
@@ -209,23 +211,23 @@
     if type(value) in [list, Jsonb]:
         msg = f"Filter value can't be of type {type(value)} using operators '>', '>=', '<', '<='"
         raise FilterError(msg)
 
     return f"{field} <= %s", value
 
 
-def _not_in(field: str, value: Any) -> tuple[str, List]:
+def _not_in(field: str, value: Any) -> Tuple[str, List]:
     if not isinstance(value, list):
         msg = f"{field}'s value must be a list when using 'not in' comparator in Pinecone"
         raise FilterError(msg)
 
     return f"{field} IS NULL OR {field} != ALL(%s)", [value]
 
 
-def _in(field: str, value: Any) -> tuple[str, List]:
+def _in(field: str, value: Any) -> Tuple[str, List]:
     if not isinstance(value, list):
         msg = f"{field}'s value must be a list when using 'in' comparator in Pinecone"
         raise FilterError(msg)
 
     # see https://www.psycopg.org/psycopg3/docs/basic/adapt.html#lists-adaptation
     return f"{field} = ANY(%s)", [value]
```

### Comparing `pgvector_haystack-0.1.0/tests/test_document_store.py` & `pgvector_haystack-0.2.0/tests/test_document_store.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,211 +9,221 @@
 from haystack.document_stores.errors import DuplicateDocumentError
 from haystack.document_stores.types import DuplicatePolicy
 from haystack.testing.document_store import CountDocumentsTest, DeleteDocumentsTest, WriteDocumentsTest
 from haystack_integrations.document_stores.pgvector import PgvectorDocumentStore
 from pandas import DataFrame
 
 
+@pytest.mark.integration
 class TestDocumentStore(CountDocumentsTest, WriteDocumentsTest, DeleteDocumentsTest):
     def test_write_documents(self, document_store: PgvectorDocumentStore):
         docs = [Document(id="1")]
         assert document_store.write_documents(docs) == 1
         with pytest.raises(DuplicateDocumentError):
             document_store.write_documents(docs, DuplicatePolicy.FAIL)
 
     def test_write_blob(self, document_store: PgvectorDocumentStore):
         bytestream = ByteStream(b"test", meta={"meta_key": "meta_value"}, mime_type="mime_type")
         docs = [Document(id="1", blob=bytestream)]
         document_store.write_documents(docs)
 
-        # TODO: update when filters are implemented
         retrieved_docs = document_store.filter_documents()
         assert retrieved_docs == docs
 
     def test_write_dataframe(self, document_store: PgvectorDocumentStore):
         dataframe = DataFrame({"col1": [1, 2], "col2": [3, 4]})
         docs = [Document(id="1", dataframe=dataframe)]
 
         document_store.write_documents(docs)
 
-        # TODO: update when filters are implemented
         retrieved_docs = document_store.filter_documents()
         assert retrieved_docs == docs
 
-    def test_init(self):
-        document_store = PgvectorDocumentStore(
-            table_name="my_table",
-            embedding_dimension=512,
-            vector_function="l2_distance",
-            recreate_table=True,
-            search_strategy="hnsw",
-            hnsw_recreate_index_if_exists=True,
-            hnsw_index_creation_kwargs={"m": 32, "ef_construction": 128},
-            hnsw_ef_search=50,
-        )
-
-        assert document_store.table_name == "my_table"
-        assert document_store.embedding_dimension == 512
-        assert document_store.vector_function == "l2_distance"
-        assert document_store.recreate_table
-        assert document_store.search_strategy == "hnsw"
-        assert document_store.hnsw_recreate_index_if_exists
-        assert document_store.hnsw_index_creation_kwargs == {"m": 32, "ef_construction": 128}
-        assert document_store.hnsw_ef_search == 50
-
-    def test_to_dict(self):
-        document_store = PgvectorDocumentStore(
-            table_name="my_table",
-            embedding_dimension=512,
-            vector_function="l2_distance",
-            recreate_table=True,
-            search_strategy="hnsw",
-            hnsw_recreate_index_if_exists=True,
-            hnsw_index_creation_kwargs={"m": 32, "ef_construction": 128},
-            hnsw_ef_search=50,
-        )
-
-        assert document_store.to_dict() == {
-            "type": "haystack_integrations.document_stores.pgvector.document_store.PgvectorDocumentStore",
-            "init_parameters": {
-                "connection_string": {"env_vars": ["PG_CONN_STR"], "strict": True, "type": "env_var"},
-                "table_name": "my_table",
-                "embedding_dimension": 512,
-                "vector_function": "l2_distance",
-                "recreate_table": True,
-                "search_strategy": "hnsw",
-                "hnsw_recreate_index_if_exists": True,
-                "hnsw_index_creation_kwargs": {"m": 32, "ef_construction": 128},
-                "hnsw_ef_search": 50,
-            },
-        }
-
-    def test_from_haystack_to_pg_documents(self):
-        haystack_docs = [
-            Document(
-                id="1",
-                content="This is a text",
-                meta={"meta_key": "meta_value"},
-                embedding=[0.1, 0.2, 0.3],
-                score=0.5,
-            ),
-            Document(
-                id="2",
-                dataframe=DataFrame({"col1": [1, 2], "col2": [3, 4]}),
-                meta={"meta_key": "meta_value"},
-                embedding=[0.4, 0.5, 0.6],
-                score=0.6,
-            ),
-            Document(
-                id="3",
-                blob=ByteStream(b"test", meta={"blob_meta_key": "blob_meta_value"}, mime_type="mime_type"),
-                meta={"meta_key": "meta_value"},
-                embedding=[0.7, 0.8, 0.9],
-                score=0.7,
-            ),
-        ]
-
-        with patch(
-            "haystack_integrations.document_stores.pgvector.document_store.PgvectorDocumentStore.__init__"
-        ) as mock_init:
-            mock_init.return_value = None
-            ds = PgvectorDocumentStore(connection_string="test")
-
-        pg_docs = ds._from_haystack_to_pg_documents(haystack_docs)
-
-        assert pg_docs[0]["id"] == "1"
-        assert pg_docs[0]["content"] == "This is a text"
-        assert pg_docs[0]["dataframe"] is None
-        assert pg_docs[0]["blob_data"] is None
-        assert pg_docs[0]["blob_meta"] is None
-        assert pg_docs[0]["blob_mime_type"] is None
-        assert pg_docs[0]["meta"].obj == {"meta_key": "meta_value"}
-        assert pg_docs[0]["embedding"] == [0.1, 0.2, 0.3]
-        assert "score" not in pg_docs[0]
-
-        assert pg_docs[1]["id"] == "2"
-        assert pg_docs[1]["content"] is None
-        assert pg_docs[1]["dataframe"].obj == DataFrame({"col1": [1, 2], "col2": [3, 4]}).to_json()
-        assert pg_docs[1]["blob_data"] is None
-        assert pg_docs[1]["blob_meta"] is None
-        assert pg_docs[1]["blob_mime_type"] is None
-        assert pg_docs[1]["meta"].obj == {"meta_key": "meta_value"}
-        assert pg_docs[1]["embedding"] == [0.4, 0.5, 0.6]
-        assert "score" not in pg_docs[1]
-
-        assert pg_docs[2]["id"] == "3"
-        assert pg_docs[2]["content"] is None
-        assert pg_docs[2]["dataframe"] is None
-        assert pg_docs[2]["blob_data"] == b"test"
-        assert pg_docs[2]["blob_meta"].obj == {"blob_meta_key": "blob_meta_value"}
-        assert pg_docs[2]["blob_mime_type"] == "mime_type"
-        assert pg_docs[2]["meta"].obj == {"meta_key": "meta_value"}
-        assert pg_docs[2]["embedding"] == [0.7, 0.8, 0.9]
-        assert "score" not in pg_docs[2]
-
-    def test_from_pg_to_haystack_documents(self):
-        pg_docs = [
-            {
-                "id": "1",
-                "content": "This is a text",
-                "dataframe": None,
-                "blob_data": None,
-                "blob_meta": None,
-                "blob_mime_type": None,
-                "meta": {"meta_key": "meta_value"},
-                "embedding": "[0.1, 0.2, 0.3]",
-            },
-            {
-                "id": "2",
-                "content": None,
-                "dataframe": DataFrame({"col1": [1, 2], "col2": [3, 4]}).to_json(),
-                "blob_data": None,
-                "blob_meta": None,
-                "blob_mime_type": None,
-                "meta": {"meta_key": "meta_value"},
-                "embedding": "[0.4, 0.5, 0.6]",
-            },
-            {
-                "id": "3",
-                "content": None,
-                "dataframe": None,
-                "blob_data": b"test",
-                "blob_meta": {"blob_meta_key": "blob_meta_value"},
-                "blob_mime_type": "mime_type",
-                "meta": {"meta_key": "meta_value"},
-                "embedding": "[0.7, 0.8, 0.9]",
-            },
-        ]
-
-        with patch(
-            "haystack_integrations.document_stores.pgvector.document_store.PgvectorDocumentStore.__init__"
-        ) as mock_init:
-            mock_init.return_value = None
-            ds = PgvectorDocumentStore(connection_string="test")
-
-        haystack_docs = ds._from_pg_to_haystack_documents(pg_docs)
-
-        assert haystack_docs[0].id == "1"
-        assert haystack_docs[0].content == "This is a text"
-        assert haystack_docs[0].dataframe is None
-        assert haystack_docs[0].blob is None
-        assert haystack_docs[0].meta == {"meta_key": "meta_value"}
-        assert haystack_docs[0].embedding == [0.1, 0.2, 0.3]
-        assert haystack_docs[0].score is None
-
-        assert haystack_docs[1].id == "2"
-        assert haystack_docs[1].content is None
-        assert haystack_docs[1].dataframe.equals(DataFrame({"col1": [1, 2], "col2": [3, 4]}))
-        assert haystack_docs[1].blob is None
-        assert haystack_docs[1].meta == {"meta_key": "meta_value"}
-        assert haystack_docs[1].embedding == [0.4, 0.5, 0.6]
-        assert haystack_docs[1].score is None
-
-        assert haystack_docs[2].id == "3"
-        assert haystack_docs[2].content is None
-        assert haystack_docs[2].dataframe is None
-        assert haystack_docs[2].blob.data == b"test"
-        assert haystack_docs[2].blob.meta == {"blob_meta_key": "blob_meta_value"}
-        assert haystack_docs[2].blob.mime_type == "mime_type"
-        assert haystack_docs[2].meta == {"meta_key": "meta_value"}
-        assert haystack_docs[2].embedding == [0.7, 0.8, 0.9]
-        assert haystack_docs[2].score is None
+
+@pytest.mark.usefixtures("patches_for_unit_tests")
+def test_init(monkeypatch):
+    monkeypatch.setenv("PG_CONN_STR", "some_connection_string")
+
+    document_store = PgvectorDocumentStore(
+        table_name="my_table",
+        embedding_dimension=512,
+        vector_function="l2_distance",
+        recreate_table=True,
+        search_strategy="hnsw",
+        hnsw_recreate_index_if_exists=True,
+        hnsw_index_creation_kwargs={"m": 32, "ef_construction": 128},
+        hnsw_ef_search=50,
+    )
+
+    assert document_store.table_name == "my_table"
+    assert document_store.embedding_dimension == 512
+    assert document_store.vector_function == "l2_distance"
+    assert document_store.recreate_table
+    assert document_store.search_strategy == "hnsw"
+    assert document_store.hnsw_recreate_index_if_exists
+    assert document_store.hnsw_index_creation_kwargs == {"m": 32, "ef_construction": 128}
+    assert document_store.hnsw_ef_search == 50
+
+
+@pytest.mark.usefixtures("patches_for_unit_tests")
+def test_to_dict(monkeypatch):
+    monkeypatch.setenv("PG_CONN_STR", "some_connection_string")
+
+    document_store = PgvectorDocumentStore(
+        table_name="my_table",
+        embedding_dimension=512,
+        vector_function="l2_distance",
+        recreate_table=True,
+        search_strategy="hnsw",
+        hnsw_recreate_index_if_exists=True,
+        hnsw_index_creation_kwargs={"m": 32, "ef_construction": 128},
+        hnsw_ef_search=50,
+    )
+
+    assert document_store.to_dict() == {
+        "type": "haystack_integrations.document_stores.pgvector.document_store.PgvectorDocumentStore",
+        "init_parameters": {
+            "connection_string": {"env_vars": ["PG_CONN_STR"], "strict": True, "type": "env_var"},
+            "table_name": "my_table",
+            "embedding_dimension": 512,
+            "vector_function": "l2_distance",
+            "recreate_table": True,
+            "search_strategy": "hnsw",
+            "hnsw_recreate_index_if_exists": True,
+            "language": "english",
+            "hnsw_index_creation_kwargs": {"m": 32, "ef_construction": 128},
+            "hnsw_ef_search": 50,
+        },
+    }
+
+
+def test_from_haystack_to_pg_documents():
+    haystack_docs = [
+        Document(
+            id="1",
+            content="This is a text",
+            meta={"meta_key": "meta_value"},
+            embedding=[0.1, 0.2, 0.3],
+            score=0.5,
+        ),
+        Document(
+            id="2",
+            dataframe=DataFrame({"col1": [1, 2], "col2": [3, 4]}),
+            meta={"meta_key": "meta_value"},
+            embedding=[0.4, 0.5, 0.6],
+            score=0.6,
+        ),
+        Document(
+            id="3",
+            blob=ByteStream(b"test", meta={"blob_meta_key": "blob_meta_value"}, mime_type="mime_type"),
+            meta={"meta_key": "meta_value"},
+            embedding=[0.7, 0.8, 0.9],
+            score=0.7,
+        ),
+    ]
+
+    with patch(
+        "haystack_integrations.document_stores.pgvector.document_store.PgvectorDocumentStore.__init__"
+    ) as mock_init:
+        mock_init.return_value = None
+        ds = PgvectorDocumentStore(connection_string="test")
+
+    pg_docs = ds._from_haystack_to_pg_documents(haystack_docs)
+
+    assert pg_docs[0]["id"] == "1"
+    assert pg_docs[0]["content"] == "This is a text"
+    assert pg_docs[0]["dataframe"] is None
+    assert pg_docs[0]["blob_data"] is None
+    assert pg_docs[0]["blob_meta"] is None
+    assert pg_docs[0]["blob_mime_type"] is None
+    assert pg_docs[0]["meta"].obj == {"meta_key": "meta_value"}
+    assert pg_docs[0]["embedding"] == [0.1, 0.2, 0.3]
+    assert "score" not in pg_docs[0]
+
+    assert pg_docs[1]["id"] == "2"
+    assert pg_docs[1]["content"] is None
+    assert pg_docs[1]["dataframe"].obj == DataFrame({"col1": [1, 2], "col2": [3, 4]}).to_json()
+    assert pg_docs[1]["blob_data"] is None
+    assert pg_docs[1]["blob_meta"] is None
+    assert pg_docs[1]["blob_mime_type"] is None
+    assert pg_docs[1]["meta"].obj == {"meta_key": "meta_value"}
+    assert pg_docs[1]["embedding"] == [0.4, 0.5, 0.6]
+    assert "score" not in pg_docs[1]
+
+    assert pg_docs[2]["id"] == "3"
+    assert pg_docs[2]["content"] is None
+    assert pg_docs[2]["dataframe"] is None
+    assert pg_docs[2]["blob_data"] == b"test"
+    assert pg_docs[2]["blob_meta"].obj == {"blob_meta_key": "blob_meta_value"}
+    assert pg_docs[2]["blob_mime_type"] == "mime_type"
+    assert pg_docs[2]["meta"].obj == {"meta_key": "meta_value"}
+    assert pg_docs[2]["embedding"] == [0.7, 0.8, 0.9]
+    assert "score" not in pg_docs[2]
+
+
+def test_from_pg_to_haystack_documents():
+    pg_docs = [
+        {
+            "id": "1",
+            "content": "This is a text",
+            "dataframe": None,
+            "blob_data": None,
+            "blob_meta": None,
+            "blob_mime_type": None,
+            "meta": {"meta_key": "meta_value"},
+            "embedding": "[0.1, 0.2, 0.3]",
+        },
+        {
+            "id": "2",
+            "content": None,
+            "dataframe": DataFrame({"col1": [1, 2], "col2": [3, 4]}).to_json(),
+            "blob_data": None,
+            "blob_meta": None,
+            "blob_mime_type": None,
+            "meta": {"meta_key": "meta_value"},
+            "embedding": "[0.4, 0.5, 0.6]",
+        },
+        {
+            "id": "3",
+            "content": None,
+            "dataframe": None,
+            "blob_data": b"test",
+            "blob_meta": {"blob_meta_key": "blob_meta_value"},
+            "blob_mime_type": "mime_type",
+            "meta": {"meta_key": "meta_value"},
+            "embedding": "[0.7, 0.8, 0.9]",
+        },
+    ]
+
+    with patch(
+        "haystack_integrations.document_stores.pgvector.document_store.PgvectorDocumentStore.__init__"
+    ) as mock_init:
+        mock_init.return_value = None
+        ds = PgvectorDocumentStore(connection_string="test")
+
+    haystack_docs = ds._from_pg_to_haystack_documents(pg_docs)
+
+    assert haystack_docs[0].id == "1"
+    assert haystack_docs[0].content == "This is a text"
+    assert haystack_docs[0].dataframe is None
+    assert haystack_docs[0].blob is None
+    assert haystack_docs[0].meta == {"meta_key": "meta_value"}
+    assert haystack_docs[0].embedding == [0.1, 0.2, 0.3]
+    assert haystack_docs[0].score is None
+
+    assert haystack_docs[1].id == "2"
+    assert haystack_docs[1].content is None
+    assert haystack_docs[1].dataframe.equals(DataFrame({"col1": [1, 2], "col2": [3, 4]}))
+    assert haystack_docs[1].blob is None
+    assert haystack_docs[1].meta == {"meta_key": "meta_value"}
+    assert haystack_docs[1].embedding == [0.4, 0.5, 0.6]
+    assert haystack_docs[1].score is None
+
+    assert haystack_docs[2].id == "3"
+    assert haystack_docs[2].content is None
+    assert haystack_docs[2].dataframe is None
+    assert haystack_docs[2].blob.data == b"test"
+    assert haystack_docs[2].blob.meta == {"blob_meta_key": "blob_meta_value"}
+    assert haystack_docs[2].blob.mime_type == "mime_type"
+    assert haystack_docs[2].meta == {"meta_key": "meta_value"}
+    assert haystack_docs[2].embedding == [0.7, 0.8, 0.9]
+    assert haystack_docs[2].score is None
```

### Comparing `pgvector_haystack-0.1.0/tests/test_embedding_retrieval.py` & `pgvector_haystack-0.2.0/tests/test_embedding_retrieval.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 import pytest
 from haystack.dataclasses.document import Document
 from haystack_integrations.document_stores.pgvector import PgvectorDocumentStore
 from numpy.random import rand
 
 
+@pytest.mark.integration
 class TestEmbeddingRetrieval:
     @pytest.fixture
     def document_store_w_hnsw_index(self, request):
         connection_string = "postgresql://postgres:postgres@localhost:5432/postgres"
         table_name = f"haystack_hnsw_{request.node.name}"
         embedding_dimension = 768
         vector_function = "cosine_similarity"
```

### Comparing `pgvector_haystack-0.1.0/tests/test_filters.py` & `pgvector_haystack-0.2.0/tests/test_filters.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     _treat_meta_field,
 )
 from pandas import DataFrame
 from psycopg.sql import SQL
 from psycopg.types.json import Jsonb
 
 
+@pytest.mark.integration
 class TestFilters(FilterDocumentsTest):
     def assert_documents_are_equal(self, received: List[Document], expected: List[Document]):
         """
         This overrides the default assert_documents_are_equal from FilterDocumentsTest.
         It is needed because the embeddings are not exactly the same when they are retrieved from Postgres.
         """
 
@@ -31,14 +32,17 @@
                 assert expected_doc.embedding is None
             else:
                 assert received_doc.embedding == pytest.approx(expected_doc.embedding)
 
             received_doc.embedding, expected_doc.embedding = None, None
             assert received_doc == expected_doc
 
+    @pytest.mark.skip(reason="NOT operator is not supported in PgvectorDocumentStore")
+    def test_not_operator(self, document_store, filterable_docs): ...
+
     def test_complex_filter(self, document_store, filterable_docs):
         document_store.write_documents(filterable_docs)
         filters = {
             "operator": "OR",
             "conditions": [
                 {
                     "operator": "AND",
@@ -65,115 +69,123 @@
                 d
                 for d in filterable_docs
                 if (d.meta.get("number") == 100 and d.meta.get("chapter") == "intro")
                 or (d.meta.get("page") == "90" and d.meta.get("chapter") == "conclusion")
             ],
         )
 
-    @pytest.mark.skip(reason="NOT operator is not supported in PgvectorDocumentStore")
-    def test_not_operator(self, document_store, filterable_docs): ...
 
-    def test_treat_meta_field(self):
-        assert _treat_meta_field(field="meta.number", value=9) == "(meta->>'number')::integer"
-        assert _treat_meta_field(field="meta.number", value=[1, 2, 3]) == "(meta->>'number')::integer"
-        assert _treat_meta_field(field="meta.name", value="my_name") == "meta->>'name'"
-        assert _treat_meta_field(field="meta.name", value=["my_name"]) == "meta->>'name'"
-        assert _treat_meta_field(field="meta.number", value=1.1) == "(meta->>'number')::real"
-        assert _treat_meta_field(field="meta.number", value=[1.1, 2.2, 3.3]) == "(meta->>'number')::real"
-        assert _treat_meta_field(field="meta.bool", value=True) == "(meta->>'bool')::boolean"
-        assert _treat_meta_field(field="meta.bool", value=[True, False, True]) == "(meta->>'bool')::boolean"
-
-        # do not cast the field if its value is not one of the known types, an empty list or None
-        assert _treat_meta_field(field="meta.other", value={"a": 3, "b": "example"}) == "meta->>'other'"
-        assert _treat_meta_field(field="meta.empty_list", value=[]) == "meta->>'empty_list'"
-        assert _treat_meta_field(field="meta.name", value=None) == "meta->>'name'"
-
-    def test_comparison_condition_dataframe_jsonb_conversion(self):
-        dataframe = DataFrame({"a": [1, 2, 3], "b": ["a", "b", "c"]})
-        condition = {"field": "meta.df", "operator": "==", "value": dataframe}
-        field, values = _parse_comparison_condition(condition)
-        assert field == "(meta.df)::jsonb = %s"
-
-        # we check each slot of the Jsonb object because it does not implement __eq__
-        assert values[0].obj == Jsonb(dataframe.to_json()).obj
-        assert values[0].dumps == Jsonb(dataframe.to_json()).dumps
-
-    def test_comparison_condition_missing_operator(self):
-        condition = {"field": "meta.type", "value": "article"}
-        with pytest.raises(FilterError):
-            _parse_comparison_condition(condition)
-
-    def test_comparison_condition_missing_value(self):
-        condition = {"field": "meta.type", "operator": "=="}
-        with pytest.raises(FilterError):
-            _parse_comparison_condition(condition)
-
-    def test_comparison_condition_unknown_operator(self):
-        condition = {"field": "meta.type", "operator": "unknown", "value": "article"}
-        with pytest.raises(FilterError):
-            _parse_comparison_condition(condition)
-
-    def test_logical_condition_missing_operator(self):
-        condition = {"conditions": []}
-        with pytest.raises(FilterError):
-            _parse_logical_condition(condition)
-
-    def test_logical_condition_missing_conditions(self):
-        condition = {"operator": "AND"}
-        with pytest.raises(FilterError):
-            _parse_logical_condition(condition)
-
-    def test_logical_condition_unknown_operator(self):
-        condition = {"operator": "unknown", "conditions": []}
-        with pytest.raises(FilterError):
-            _parse_logical_condition(condition)
-
-    def test_logical_condition_nested(self):
-        condition = {
-            "operator": "AND",
-            "conditions": [
-                {
-                    "operator": "OR",
-                    "conditions": [
-                        {"field": "meta.domain", "operator": "!=", "value": "science"},
-                        {"field": "meta.chapter", "operator": "in", "value": ["intro", "conclusion"]},
-                    ],
-                },
-                {
-                    "operator": "OR",
-                    "conditions": [
-                        {"field": "meta.number", "operator": ">=", "value": 90},
-                        {"field": "meta.author", "operator": "not in", "value": ["John", "Jane"]},
-                    ],
-                },
-            ],
-        }
-        query, values = _parse_logical_condition(condition)
-        assert query == (
-            "((meta->>'domain' IS DISTINCT FROM %s OR meta->>'chapter' = ANY(%s)) "
-            "AND ((meta->>'number')::integer >= %s OR meta->>'author' IS NULL OR meta->>'author' != ALL(%s)))"
-        )
-        assert values == ["science", [["intro", "conclusion"]], 90, [["John", "Jane"]]]
-
-    def test_convert_filters_to_where_clause_and_params(self):
-        filters = {
-            "operator": "AND",
-            "conditions": [
-                {"field": "meta.number", "operator": "==", "value": 100},
-                {"field": "meta.chapter", "operator": "==", "value": "intro"},
-            ],
-        }
-        where_clause, params = _convert_filters_to_where_clause_and_params(filters)
-        assert where_clause == SQL(" WHERE ") + SQL("((meta->>'number')::integer = %s AND meta->>'chapter' = %s)")
-        assert params == (100, "intro")
-
-    def test_convert_filters_to_where_clause_and_params_handle_null(self):
-        filters = {
-            "operator": "AND",
-            "conditions": [
-                {"field": "meta.number", "operator": "==", "value": None},
-                {"field": "meta.chapter", "operator": "==", "value": "intro"},
-            ],
-        }
-        where_clause, params = _convert_filters_to_where_clause_and_params(filters)
-        assert where_clause == SQL(" WHERE ") + SQL("(meta->>'number' IS NULL AND meta->>'chapter' = %s)")
-        assert params == ("intro",)
+def test_treat_meta_field():
+    assert _treat_meta_field(field="meta.number", value=9) == "(meta->>'number')::integer"
+    assert _treat_meta_field(field="meta.number", value=[1, 2, 3]) == "(meta->>'number')::integer"
+    assert _treat_meta_field(field="meta.name", value="my_name") == "meta->>'name'"
+    assert _treat_meta_field(field="meta.name", value=["my_name"]) == "meta->>'name'"
+    assert _treat_meta_field(field="meta.number", value=1.1) == "(meta->>'number')::real"
+    assert _treat_meta_field(field="meta.number", value=[1.1, 2.2, 3.3]) == "(meta->>'number')::real"
+    assert _treat_meta_field(field="meta.bool", value=True) == "(meta->>'bool')::boolean"
+    assert _treat_meta_field(field="meta.bool", value=[True, False, True]) == "(meta->>'bool')::boolean"
+
+    # do not cast the field if its value is not one of the known types, an empty list or None
+    assert _treat_meta_field(field="meta.other", value={"a": 3, "b": "example"}) == "meta->>'other'"
+    assert _treat_meta_field(field="meta.empty_list", value=[]) == "meta->>'empty_list'"
+    assert _treat_meta_field(field="meta.name", value=None) == "meta->>'name'"
+
+
+def test_comparison_condition_dataframe_jsonb_conversion():
+    dataframe = DataFrame({"a": [1, 2, 3], "b": ["a", "b", "c"]})
+    condition = {"field": "meta.df", "operator": "==", "value": dataframe}
+    field, values = _parse_comparison_condition(condition)
+    assert field == "(meta.df)::jsonb = %s"
+
+    # we check each slot of the Jsonb object because it does not implement __eq__
+    assert values[0].obj == Jsonb(dataframe.to_json()).obj
+    assert values[0].dumps == Jsonb(dataframe.to_json()).dumps
+
+
+def test_comparison_condition_missing_operator():
+    condition = {"field": "meta.type", "value": "article"}
+    with pytest.raises(FilterError):
+        _parse_comparison_condition(condition)
+
+
+def test_comparison_condition_missing_value():
+    condition = {"field": "meta.type", "operator": "=="}
+    with pytest.raises(FilterError):
+        _parse_comparison_condition(condition)
+
+
+def test_comparison_condition_unknown_operator():
+    condition = {"field": "meta.type", "operator": "unknown", "value": "article"}
+    with pytest.raises(FilterError):
+        _parse_comparison_condition(condition)
+
+
+def test_logical_condition_missing_operator():
+    condition = {"conditions": []}
+    with pytest.raises(FilterError):
+        _parse_logical_condition(condition)
+
+
+def test_logical_condition_missing_conditions():
+    condition = {"operator": "AND"}
+    with pytest.raises(FilterError):
+        _parse_logical_condition(condition)
+
+
+def test_logical_condition_unknown_operator():
+    condition = {"operator": "unknown", "conditions": []}
+    with pytest.raises(FilterError):
+        _parse_logical_condition(condition)
+
+
+def test_logical_condition_nested():
+    condition = {
+        "operator": "AND",
+        "conditions": [
+            {
+                "operator": "OR",
+                "conditions": [
+                    {"field": "meta.domain", "operator": "!=", "value": "science"},
+                    {"field": "meta.chapter", "operator": "in", "value": ["intro", "conclusion"]},
+                ],
+            },
+            {
+                "operator": "OR",
+                "conditions": [
+                    {"field": "meta.number", "operator": ">=", "value": 90},
+                    {"field": "meta.author", "operator": "not in", "value": ["John", "Jane"]},
+                ],
+            },
+        ],
+    }
+    query, values = _parse_logical_condition(condition)
+    assert query == (
+        "((meta->>'domain' IS DISTINCT FROM %s OR meta->>'chapter' = ANY(%s)) "
+        "AND ((meta->>'number')::integer >= %s OR meta->>'author' IS NULL OR meta->>'author' != ALL(%s)))"
+    )
+    assert values == ["science", [["intro", "conclusion"]], 90, [["John", "Jane"]]]
+
+
+def test_convert_filters_to_where_clause_and_params():
+    filters = {
+        "operator": "AND",
+        "conditions": [
+            {"field": "meta.number", "operator": "==", "value": 100},
+            {"field": "meta.chapter", "operator": "==", "value": "intro"},
+        ],
+    }
+    where_clause, params = _convert_filters_to_where_clause_and_params(filters)
+    assert where_clause == SQL(" WHERE ") + SQL("((meta->>'number')::integer = %s AND meta->>'chapter' = %s)")
+    assert params == (100, "intro")
+
+
+def test_convert_filters_to_where_clause_and_params_handle_null():
+    filters = {
+        "operator": "AND",
+        "conditions": [
+            {"field": "meta.number", "operator": "==", "value": None},
+            {"field": "meta.chapter", "operator": "==", "value": "intro"},
+        ],
+    }
+    where_clause, params = _convert_filters_to_where_clause_and_params(filters)
+    assert where_clause == SQL(" WHERE ") + SQL("(meta->>'number' IS NULL AND meta->>'chapter' = %s)")
+    assert params == ("intro",)
```

### Comparing `pgvector_haystack-0.1.0/tests/test_retriever.py` & `pgvector_haystack-0.2.0/tests/test_retrievers.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,65 +1,69 @@
 # SPDX-FileCopyrightText: 2023-present deepset GmbH <info@deepset.ai>
 #
 # SPDX-License-Identifier: Apache-2.0
 from unittest.mock import Mock
 
+import pytest
 from haystack.dataclasses import Document
 from haystack.utils.auth import EnvVarSecret
-from haystack_integrations.components.retrievers.pgvector import PgvectorEmbeddingRetriever
+from haystack_integrations.components.retrievers.pgvector import PgvectorEmbeddingRetriever, PgvectorKeywordRetriever
 from haystack_integrations.document_stores.pgvector import PgvectorDocumentStore
 
 
-class TestRetriever:
-    def test_init_default(self, document_store: PgvectorDocumentStore):
-        retriever = PgvectorEmbeddingRetriever(document_store=document_store)
-        assert retriever.document_store == document_store
+class TestEmbeddingRetriever:
+    def test_init_default(self, mock_store):
+        retriever = PgvectorEmbeddingRetriever(document_store=mock_store)
+        assert retriever.document_store == mock_store
         assert retriever.filters == {}
         assert retriever.top_k == 10
-        assert retriever.vector_function == document_store.vector_function
+        assert retriever.vector_function == mock_store.vector_function
 
-    def test_init(self, document_store: PgvectorDocumentStore):
+    def test_init(self, mock_store):
         retriever = PgvectorEmbeddingRetriever(
-            document_store=document_store, filters={"field": "value"}, top_k=5, vector_function="l2_distance"
+            document_store=mock_store, filters={"field": "value"}, top_k=5, vector_function="l2_distance"
         )
-        assert retriever.document_store == document_store
+        assert retriever.document_store == mock_store
         assert retriever.filters == {"field": "value"}
         assert retriever.top_k == 5
         assert retriever.vector_function == "l2_distance"
 
-    def test_to_dict(self, document_store: PgvectorDocumentStore):
+    def test_to_dict(self, mock_store):
         retriever = PgvectorEmbeddingRetriever(
-            document_store=document_store, filters={"field": "value"}, top_k=5, vector_function="l2_distance"
+            document_store=mock_store, filters={"field": "value"}, top_k=5, vector_function="l2_distance"
         )
         res = retriever.to_dict()
         t = "haystack_integrations.components.retrievers.pgvector.embedding_retriever.PgvectorEmbeddingRetriever"
         assert res == {
             "type": t,
             "init_parameters": {
                 "document_store": {
                     "type": "haystack_integrations.document_stores.pgvector.document_store.PgvectorDocumentStore",
                     "init_parameters": {
                         "connection_string": {"env_vars": ["PG_CONN_STR"], "strict": True, "type": "env_var"},
-                        "table_name": "haystack_test_to_dict",
+                        "table_name": "haystack",
                         "embedding_dimension": 768,
                         "vector_function": "cosine_similarity",
                         "recreate_table": True,
                         "search_strategy": "exact_nearest_neighbor",
                         "hnsw_recreate_index_if_exists": False,
+                        "language": "english",
                         "hnsw_index_creation_kwargs": {},
                         "hnsw_ef_search": None,
                     },
                 },
                 "filters": {"field": "value"},
                 "top_k": 5,
                 "vector_function": "l2_distance",
             },
         }
 
-    def test_from_dict(self):
+    @pytest.mark.usefixtures("patches_for_unit_tests")
+    def test_from_dict(self, monkeypatch):
+        monkeypatch.setenv("PG_CONN_STR", "some-connection-string")
         t = "haystack_integrations.components.retrievers.pgvector.embedding_retriever.PgvectorEmbeddingRetriever"
         data = {
             "type": t,
             "init_parameters": {
                 "document_store": {
                     "type": "haystack_integrations.document_stores.pgvector.document_store.PgvectorDocumentStore",
                     "init_parameters": {
@@ -107,7 +111,103 @@
         res = retriever.run(query_embedding=[0.3, 0.5])
 
         mock_store._embedding_retrieval.assert_called_once_with(
             query_embedding=[0.3, 0.5], filters={}, top_k=10, vector_function="l2_distance"
         )
 
         assert res == {"documents": [doc]}
+
+
+class TestKeywordRetriever:
+    def test_init_default(self, mock_store):
+        retriever = PgvectorKeywordRetriever(document_store=mock_store)
+        assert retriever.document_store == mock_store
+        assert retriever.filters == {}
+        assert retriever.top_k == 10
+
+    def test_init(self, mock_store):
+        retriever = PgvectorKeywordRetriever(document_store=mock_store, filters={"field": "value"}, top_k=5)
+        assert retriever.document_store == mock_store
+        assert retriever.filters == {"field": "value"}
+        assert retriever.top_k == 5
+
+    def test_to_dict(self, mock_store):
+        retriever = PgvectorKeywordRetriever(document_store=mock_store, filters={"field": "value"}, top_k=5)
+        res = retriever.to_dict()
+        t = "haystack_integrations.components.retrievers.pgvector.keyword_retriever.PgvectorKeywordRetriever"
+        assert res == {
+            "type": t,
+            "init_parameters": {
+                "document_store": {
+                    "type": "haystack_integrations.document_stores.pgvector.document_store.PgvectorDocumentStore",
+                    "init_parameters": {
+                        "connection_string": {"env_vars": ["PG_CONN_STR"], "strict": True, "type": "env_var"},
+                        "table_name": "haystack",
+                        "embedding_dimension": 768,
+                        "vector_function": "cosine_similarity",
+                        "recreate_table": True,
+                        "search_strategy": "exact_nearest_neighbor",
+                        "hnsw_recreate_index_if_exists": False,
+                        "language": "english",
+                        "hnsw_index_creation_kwargs": {},
+                        "hnsw_ef_search": None,
+                    },
+                },
+                "filters": {"field": "value"},
+                "top_k": 5,
+            },
+        }
+
+    @pytest.mark.usefixtures("patches_for_unit_tests")
+    def test_from_dict(self, monkeypatch):
+        monkeypatch.setenv("PG_CONN_STR", "some-connection-string")
+        t = "haystack_integrations.components.retrievers.pgvector.keyword_retriever.PgvectorKeywordRetriever"
+        data = {
+            "type": t,
+            "init_parameters": {
+                "document_store": {
+                    "type": "haystack_integrations.document_stores.pgvector.document_store.PgvectorDocumentStore",
+                    "init_parameters": {
+                        "connection_string": {"env_vars": ["PG_CONN_STR"], "strict": True, "type": "env_var"},
+                        "table_name": "haystack_test_to_dict",
+                        "embedding_dimension": 768,
+                        "vector_function": "cosine_similarity",
+                        "recreate_table": True,
+                        "search_strategy": "exact_nearest_neighbor",
+                        "hnsw_recreate_index_if_exists": False,
+                        "hnsw_index_creation_kwargs": {},
+                        "hnsw_ef_search": None,
+                    },
+                },
+                "filters": {"field": "value"},
+                "top_k": 5,
+            },
+        }
+
+        retriever = PgvectorKeywordRetriever.from_dict(data)
+        document_store = retriever.document_store
+
+        assert isinstance(document_store, PgvectorDocumentStore)
+        assert isinstance(document_store.connection_string, EnvVarSecret)
+        assert document_store.table_name == "haystack_test_to_dict"
+        assert document_store.embedding_dimension == 768
+        assert document_store.vector_function == "cosine_similarity"
+        assert document_store.recreate_table
+        assert document_store.search_strategy == "exact_nearest_neighbor"
+        assert not document_store.hnsw_recreate_index_if_exists
+        assert document_store.hnsw_index_creation_kwargs == {}
+        assert document_store.hnsw_ef_search is None
+
+        assert retriever.filters == {"field": "value"}
+        assert retriever.top_k == 5
+
+    def test_run(self):
+        mock_store = Mock(spec=PgvectorDocumentStore)
+        doc = Document(content="Test doc", embedding=[0.1, 0.2])
+        mock_store._keyword_retrieval.return_value = [doc]
+
+        retriever = PgvectorKeywordRetriever(document_store=mock_store)
+        res = retriever.run(query="test query")
+
+        mock_store._keyword_retrieval.assert_called_once_with(query="test query", filters={}, top_k=10)
+
+        assert res == {"documents": [doc]}
```

### Comparing `pgvector_haystack-0.1.0/.gitignore` & `pgvector_haystack-0.2.0/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -130,7 +130,8 @@
 .pyre/
 
 # IDEs
 .vscode
 
 # Docs generation artifacts
 _readme_*.md
+.idea
```

### Comparing `pgvector_haystack-0.1.0/LICENSE.txt` & `pgvector_haystack-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pgvector_haystack-0.1.0/README.md` & `pgvector_haystack-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pgvector_haystack-0.1.0/pyproject.toml` & `pgvector_haystack-0.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 requires-python = ">=3.8"
 license = "Apache-2.0"
 keywords = []
 authors = [
   { name = "deepset GmbH", email = "info@deepset.ai" },
 ]
 classifiers = [
+  "License :: OSI Approved :: Apache Software License",
   "Development Status :: 4 - Beta",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
@@ -47,15 +48,15 @@
 git_describe_command = 'git describe --tags --match="integrations/pgvector-v[0-9]*"'
 
 [tool.hatch.envs.default]
 dependencies = [
   "coverage[toml]>=6.5",
   "pytest",
   "ipython",
-  "haystack-pydoc-tools",  
+  "haystack-pydoc-tools",
 ]
 [tool.hatch.envs.default.scripts]
 test = "pytest {args:tests}"
 test-cov = "coverage run -m pytest {args:tests}"
 cov-report = [
   "- coverage combine",
   "coverage report",
@@ -91,20 +92,20 @@
 ]
 all = [
   "style",
   "typing",
 ]
 
 [tool.black]
-target-version = ["py37"]
+target-version = ["py38"]
 line-length = 120
 skip-string-normalization = true
 
 [tool.ruff]
-target-version = "py37"
+target-version = "py38"
 line-length = 120
 select = [
   "A",
   "ARG",
   "B",
   "C",
   "DTZ",
@@ -158,25 +159,30 @@
 # examples can contain "print" commands
 "examples/**/*" = ["T201"]
 
 
 [tool.coverage.run]
 source = ["haystack_integrations"]
 branch = true
-parallel = true
+parallel = false
 
 [tool.coverage.report]
 omit = ["*/tests/*", "*/__init__.py"]
 show_missing=true
 exclude_lines = [
   "no cov",
   "if __name__ == .__main__.:",
   "if TYPE_CHECKING:",
 ]
 
+[tool.pytest.ini_options]
+markers = [
+  "integration: integration tests"
+]
+
 
 [[tool.mypy.overrides]]
 module = [
   "haystack.*",
   "haystack_integrations.*",
   "pgvector.*",
   "psycopg.*",
```

### Comparing `pgvector_haystack-0.1.0/PKG-INFO` & `pgvector_haystack-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: pgvector-haystack
-Version: 0.1.0
+Version: 0.2.0
 Summary: An integration of pgvector (vector search extension for Postgres) with Haystack
 Project-URL: Source, https://github.com/deepset-ai/haystack-core-integrations
 Project-URL: Documentation, https://github.com/deepset-ai/haystack-core-integrations/blob/main/integrations/pgvector/README.md
 Project-URL: Issues, https://github.com/deepset-ai/haystack-core-integrations/issues
 Author-email: deepset GmbH <info@deepset.ai>
 License-Expression: Apache-2.0
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
```

