# Comparing `tmp/aerospace_chatbot-0.0.5.tar.gz` & `tmp/aerospace_chatbot-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aerospace_chatbot-0.0.5.tar", max compression
+gzip compressed data, was "aerospace_chatbot-0.0.6.tar", max compression
```

## Comparing `aerospace_chatbot-0.0.5.tar` & `aerospace_chatbot-0.0.6.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1068 2024-04-11 05:19:38.306973 aerospace_chatbot-0.0.5/LICENSE
--rw-r--r--   0        0        0      506 2024-04-14 01:32:23.236876 aerospace_chatbot-0.0.5/README.md
--rw-r--r--   0        0        0     1290 2024-04-26 14:27:49.251082 aerospace_chatbot-0.0.5/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-31 15:24:34.392942 aerospace_chatbot-0.0.5/src/aerospace_chatbot/__init__.py
--rw-r--r--   0        0        0    39473 2024-04-26 14:27:49.252138 aerospace_chatbot-0.0.5/src/aerospace_chatbot/admin.py
--rw-r--r--   0        0        0    40050 2024-04-26 14:27:49.252611 aerospace_chatbot-0.0.5/src/aerospace_chatbot/data_processing.py
--rw-r--r--   0        0        0      919 2024-03-31 15:24:34.393743 aerospace_chatbot-0.0.5/src/aerospace_chatbot/prompts.py
--rw-r--r--   0        0        0    13109 2024-04-26 14:27:49.253020 aerospace_chatbot-0.0.5/src/aerospace_chatbot/queries.py
--rw-r--r--   0        0        0     2601 1970-01-01 00:00:00.000000 aerospace_chatbot-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-04-11 05:19:38.306973 aerospace_chatbot-0.0.6/LICENSE
+-rw-r--r--   0        0        0      506 2024-04-14 01:32:23.236876 aerospace_chatbot-0.0.6/README.md
+-rw-r--r--   0        0        0     1266 2024-05-08 15:42:28.133504 aerospace_chatbot-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-31 15:24:34.392942 aerospace_chatbot-0.0.6/src/aerospace_chatbot/__init__.py
+-rw-r--r--   0        0        0    39365 2024-05-08 15:26:25.250350 aerospace_chatbot-0.0.6/src/aerospace_chatbot/admin.py
+-rw-r--r--   0        0        0    42763 2024-05-08 15:28:32.185362 aerospace_chatbot-0.0.6/src/aerospace_chatbot/data_processing.py
+-rw-r--r--   0        0        0      968 2024-05-08 15:18:39.071804 aerospace_chatbot-0.0.6/src/aerospace_chatbot/prompts.py
+-rw-r--r--   0        0        0    15047 2024-05-08 15:26:25.251310 aerospace_chatbot-0.0.6/src/aerospace_chatbot/queries.py
+-rw-r--r--   0        0        0     2550 1970-01-01 00:00:00.000000 aerospace_chatbot-0.0.6/PKG-INFO
```

### Comparing `aerospace_chatbot-0.0.5/LICENSE` & `aerospace_chatbot-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `aerospace_chatbot-0.0.5/pyproject.toml` & `aerospace_chatbot-0.0.6/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aerospace-chatbot"
-version = "0.0.5"
+version = "0.0.6"
 description = "Aerospace engineering chatbot and AI tools."
 authors = ["dsmueller <dsm@danmueller.pro>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/dan-s-mueller/aerospace_chatbot/tree/main"
 repository = "https://github.com/dan-s-mueller/aerospace_chatbot/tree/main"
 
@@ -33,17 +33,16 @@
 streamlit-authenticator = "^0.3.1"
 langchain = "^0.1.13"
 langchain-core = "^0.1.36"
 langchainhub = "^0.1.15"
 langchain-pinecone = "^0.0.3"
 langchain-community = "^0.0.29"
 langchain-openai = "^0.1.1"
-renumics-spotlight = "^1.6.8"
 ragas = "^0.1.6"
 sphinxawesome-theme = "^5.1.1"
 sphinx-design = "^0.5.0"
 langchain-voyageai = "^0.1.0"
-ragxplorer = "^0.1.10"
+renumics-spotlight = "1.6.5"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `aerospace_chatbot-0.0.5/src/aerospace_chatbot/admin.py` & `aerospace_chatbot-0.0.6/src/aerospace_chatbot/admin.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import data_processing
 from prompts import TEST_QUERY_PROMPT
 
 import inspect
 import os
-import logging
 import json
 import streamlit as st
 from dotenv import load_dotenv,find_dotenv
 
 import openai
 from pinecone import Pinecone
 import chromadb
@@ -40,27 +39,27 @@
     def __init__(self, message, id):
         super().__init__(message)
         self.id = id
 def load_sidebar(config_file,
                  vector_database=False,
                  embeddings=False,
                  rag_type=False,
-                 index_name=False,
+                 index_selected=False,
                  llm=False,
                  model_options=False,
                  secret_keys=False):
     """
     Loads the sidebar configuration for the chatbot.
 
     Args:
         config_file (str): The path to the configuration file.
         vector_database (bool, optional): Whether to include the vector database in the sidebar. Defaults to False.
         embeddings (bool, optional): Whether to include embeddings in the sidebar. Defaults to False.
         rag_type (bool, optional): Whether to include RAG type in the sidebar. Defaults to False.
-        index_name (bool, optional): Whether to include index name in the sidebar. Defaults to False.
+        index_selected (bool, optional): Whether to include index name in the sidebar. Defaults to False.
         llm (bool, optional): Whether to include LLM in the sidebar. Defaults to False.
         model_options (bool, optional): Whether to include model options in the sidebar. Defaults to False.
         secret_keys (bool, optional): Whether to include secret keys in the sidebar. Defaults to False.
 
     Returns:
         dict: The sidebar configuration.
     """
@@ -76,15 +75,14 @@
         # This is the case where the .env file is not in the directory
         raise SecretKeyException('Local Database Path is required. Use an absolute path for local, or /data for hugging face spaces.','LOCAL_DB_PATH_MISSING')
 
     # Vector databases
     if vector_database:
         st.sidebar.title('Vector database')
         sb_out['index_type']=st.sidebar.selectbox('Index type', list(databases.keys()), index=1,help='Select the type of index to use.')
-        logging.info('Index type: '+sb_out['index_type'])
 
         if embeddings:
             # Embeddings
             st.sidebar.title('Embeddings',help='See embedding leaderboard here for performance overview: https://huggingface.co/spaces/mteb/leaderboard')
             if sb_out['index_type']=='RAGatouille':    # Default to selecting hugging face model for RAGatouille, otherwise select alternates
                 sb_out['query_model']=st.sidebar.selectbox('Hugging face rag models', 
                                                         databases[sb_out['index_type']]['embedding_models'], 
@@ -119,74 +117,79 @@
                                                                 help='Select the Hugging Face model for RAG.')
                         sb_out['rag_hf_endpoint']='https://api-inference.huggingface.co/v1'
                     elif sb_out['rag_llm_source']=='LM Studio (local)':
                         sb_out['rag_llm_model']=st.sidebar.text_input('Local host URL',
                                                                 'http://localhost:1234/v1',
                                                                 help='See LM studio configuration for local host URL.')
                         st.sidebar.warning('You must load a model in LM studio first for this to work.')
-            logging.info('RAG type: '+sb_out['rag_type'])
-        if index_name:
+        if index_selected:
             if embeddings and rag_type:
                 # Index Name 
-                st.sidebar.title('Index Name')  
-                sb_out['index_name'] = (sb_out['index_type'] + '-' + sb_out['embedding_name'].replace('/', '-')).lower()
-                st.sidebar.markdown('Index base name: '+sb_out['index_name'],help='An index appendix is added on creation under Database Processing.')
-                logging.info('Index name: '+sb_out['index_name'])
-                
+                st.sidebar.title('Index Selected')  
+                name=[]
                 # For each index type, list indices available for the base name
                 if sb_out['index_type']=='ChromaDB':
                     indices=show_chroma_collections(format=False)
                     if indices['status']:
-                        name=[]
                         for index in indices['message']:
                             # Be compatible with embedding types already used. Pinecone only supports lowercase.
-                            if index.name.startswith((sb_out['index_type'] + '-' + sb_out['embedding_name'].replace('/', '-')).lower()):    
-                                if sb_out['rag_type']=='Parent-Child':
-                                    if index.name.endswith('-parent-child'):
+                            if index.name.startswith((sb_out['embedding_name'].replace('/', '-')).lower()):    
+                                if not index.name.endswith('-queries'): # Don't list query database as selectable
+                                    if sb_out['rag_type']=='Parent-Child':
+                                        if index.name.endswith('-parent-child'):
+                                            name.append(index.name)
+                                    elif sb_out['rag_type']=='Summary':
+                                        if index.name.endswith('-summary'):
+                                            name.append(index.name)
+                                    else:
                                         name.append(index.name)
-                                elif sb_out['rag_type']=='Summary':
-                                    if index.name.endswith('-summary'):
-                                        name.append(index.name)
-                                else:
-                                    name.append(index.name)
                         sb_out['index_selected']=st.sidebar.selectbox('Index selected',name,index=0,help='Select the index to use for the application.')
-                        try:
-                            if len(name) == 0:
-                                raise DatabaseException('No collections found for the selected index type/embedding. Create a new database, or select another index type/embedding.','NO_COMPATIBLE_COLLECTIONS')
-                        except DatabaseException as e:
-                            st.warning(f"{e}")
-                            st.stop()
                     else:
                         st.sidebar.markdown('No collections found.',help='Check the status on Home.')
                 elif sb_out['index_type']=='Pinecone':
                     indices=show_pinecone_indexes(format=False)
                     if indices['status']:
-                        name=[]
                         for index in indices['message']:
-                            if index['status']['state']=='Ready':
-                                name.append(index['name'])
+                            # if index['status']['state']=='Ready':
+                            #     name.append(index['name'])
+                            if index['name'].startswith((sb_out['embedding_name'].replace('/', '-')).lower()):    
+                                if not index['name'].endswith('-queries'): # Don't list query database as selectable
+                                    if sb_out['rag_type']=='Parent-Child':
+                                        if index['name'].endswith('-parent-child'):
+                                            name.append(index['name'])
+                                    elif sb_out['rag_type']=='Summary':
+                                        if index['name'].endswith('-summary'):
+                                            name.append(index['name'])
+                                    else:
+                                        name.append(index['name'])
                         sb_out['index_selected']=st.sidebar.selectbox('Index selected',name,index=0,help='Select the index to use for the application.')
                 elif sb_out['index_type']=='RAGatouille':
                     indices=show_ragatouille_indexes(format=False)
                     if len(indices)>0:
-                        name=[]
                         for index in indices['message']:
                             # Be compatible with embedding types already used. Pinecone only supports lowercase.
-                            if index.startswith((sb_out['index_type'] + '-' + sb_out['embedding_name'].replace('/', '-')).lower()):    
+                            if index.startswith((sb_out['embedding_name'].replace('/', '-')).lower()):    
                                 name.append(index)
                         sb_out['index_selected']=st.sidebar.selectbox('Index selected',name,index=0,help='Select the index to use for the application.')
                     else:
                         st.sidebar.markdown('No collections found.',help='Check the status on Home.')
+                else:
+                    raise NotImplementedError
+                try:
+                    if not name:
+                        raise DatabaseException('No collections found for the selected index type/embedding. Create a new database, or select another index type/embedding.','NO_COMPATIBLE_COLLECTIONS')
+                except DatabaseException as e:
+                    st.warning(f"{e}")
+                    st.stop()
             else:
                 raise ValueError('Embeddings must be enabled to select an index name.')
         if llm:
             # LLM
             st.sidebar.title('LLM',help='See LLM leaderboard here for performance overview: https://huggingface.co/spaces/lmsys/chatbot-arena-leaderboard')
             sb_out['llm_source']=st.sidebar.selectbox('LLM model', list(llms.keys()), index=0,help='Select the LLM model for the application.')
-            logging.info('LLM source: '+sb_out['llm_source'])
             if sb_out['llm_source']=='OpenAI':
                 sb_out['llm_model']=st.sidebar.selectbox('OpenAI model', llms[sb_out['llm_source']]['models'], index=0,help='Select the OpenAI model for the application.')
             elif sb_out['llm_source']=='Hugging Face':
                 sb_out['llm_model']=st.sidebar.selectbox('Hugging Face model', 
                                                         llms['Hugging Face']['models'], 
                                                         index=0,
                                                         help='Select the Hugging Face model for the application.')
@@ -214,15 +217,15 @@
                                             'temperature':temperature}
                 else:
                     sb_out['model_options']={'output_level':output_level,
                                              'k':k,
                                             'search_type':None,
                                             'temperature':temperature}
     else:
-        if embeddings or rag_type or index_name or llm or model_options:
+        if embeddings or rag_type or index_selected or llm or model_options:
             # Must have vector database for any of this functionality.
             raise ValueError('Vector database must be enabled to use these options.')
 
     # Secret keys, which does not rely on vector_database
     if secret_keys:
         sb_out['keys']={}
         # Add a section for secret keys
@@ -406,15 +409,14 @@
         format (bool, optional): Specifies whether to format the output. Defaults to True.
 
     Returns:
         dict or str: If format is True, returns a formatted string representation of the Pinecone status.
                     If format is False, returns a dictionary containing the Pinecone status.
 
     """
-    print(os.getenv('PINECONE_API_KEY'))
     if os.getenv('PINECONE_API_KEY') is None or os.getenv('PINECONE_API_KEY')=='':
         pinecone_status = {'status': False, 'message': 'Pinecone API Key is not set.'}
     else:
         pc=Pinecone(api_key=os.getenv('PINECONE_API_KEY'))
         indexes=pc.list_indexes()
         if len(indexes)==0:
             pinecone_status = {'status': False, 'message': 'No indexes found'}
@@ -505,15 +507,15 @@
         expanded (bool, optional): Whether the expander is initially expanded or collapsed. Only intended with account access. Defaults to True.
         delete_buttons (bool, optional): Whether to display delete buttons for Pinecone and Chroma DB indexes. Defaults to False.
         set_secrets (bool, optional): Whether to set the secrets. Defaults to False.
     """
     with st.expander("Connection Status", expanded=expanded):
         # Set secrets and assign to environment variables
         if set_secrets:
-            st.markdown("**Set API keyss**:")
+            st.markdown("**Set API keys**:")
             keys={}
             # OPENAI_API_KEY
             keys['OPENAI_API_KEY'] = st.text_input('OpenAI API Key', type='password',help='OpenAI API Key: https://platform.openai.com/api-keys')
             if keys['OPENAI_API_KEY']!='':
                 os.environ['OPENAI_API_KEY'] = keys['OPENAI_API_KEY'] 
             
             # VOYAGE_API_KEY
@@ -681,27 +683,14 @@
     Formats the key status dictionary into a formatted string.
 
     Args:
         key_status (str): The dictionary containing the key status information.
 
     Returns:
         str: The formatted string representing the key status.
-
-    Example:
-        key_status = {
-            'key1': {'status': True},
-            'key2': {'status': False},
-            'key3': {'status': True}
-        }
-        formatted_status = _format_key_status(key_status)
-        print(formatted_status)
-        # Output:
-        # - key1: :heavy_check_mark:
-        # - key2: :x:
-        # - key3: :heavy_check_mark:
     """
     formatted_status = ""
     for key, value in key_status.items():
         status = value['status']
         if status:
             formatted_status += f"- {key}: :heavy_check_mark:\n"
         else:
```

### Comparing `aerospace_chatbot-0.0.5/src/aerospace_chatbot/data_processing.py` & `aerospace_chatbot-0.0.6/src/aerospace_chatbot/data_processing.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from prompts import SUMMARIZE_TEXT
 
-import os, re, shutil, random
+import os, re, shutil
 import hashlib
-import uuid
 from pathlib import Path
 from typing import List, Union
 
 from tenacity import retry, stop_after_attempt, wait_exponential
 
 from pinecone import Pinecone as pinecone_client
 from pinecone import PodSpec
@@ -33,17 +32,25 @@
 from langchain_community.document_loaders import PyPDFLoader
 
 from langchain_core.documents import Document
 from langchain_core.output_parsers import StrOutputParser
 
 from ragatouille import RAGPretrainedModel
 
-from ragxplorer import RAGxplorer, rag
+from renumics import spotlight
+from renumics.spotlight import dtypes as spotlight_dtypes
+
 import pandas as pd
+import numpy as np
+from sklearn.cluster import KMeans
+
+from datasets import Dataset
 
+import admin
+from prompts import CLUSTER_LABEL
 
 def load_docs(index_type:str,
               docs:List[str],
               query_model:object,
               rag_type:str='Standard',
               index_name:str=None,
               n_merge_pages:int=None,
@@ -147,16 +154,14 @@
     """
     if show_progress:
         progress_text = "Chunking in progress..."
         my_bar = st.progress(0, text=progress_text)
     pages=[]
     chunks=[]
     
-    merged_docs = []
-    
     # Parse doc pages
     for i, doc in enumerate(docs):
         
         loader = PyPDFLoader(doc)
         doc_page_data = loader.load()
 
         # Clean up page info, update some metadata
@@ -174,30 +179,28 @@
             for i in range(0, len(doc_pages), n_merge_pages):
                 group = doc_pages[i:i+n_merge_pages]
                 group_page_content=' '.join([doc.page_content for doc in group])
                 group_metadata = {'page': str([doc.metadata['page'] for doc in group]), 
                                   'source': str([doc.metadata['source'] for doc in group])}
                 merged_doc = Document(page_content=group_page_content, metadata=group_metadata)
                 pages.append(merged_doc)
-            # pages = merged_docs
         else:
             pages.extend(doc_pages)
     
     # Process pages
     if rag_type=='Standard': 
         if chunk_method=='character_recursive':
             text_splitter = RecursiveCharacterTextSplitter(chunk_size=chunk_size, 
                                                            chunk_overlap=chunk_overlap,
                                                            add_start_index=True)
             page_chunks = text_splitter.split_documents(pages)
             for i, chunk in enumerate(page_chunks):
                 if show_progress:
                     progress_percentage = i / len(page_chunks)
                     my_bar.progress(progress_percentage, text=f'Chunking documents...{progress_percentage*100:.2f}%')
-                # chunk.page_content += str(chunk.metadata)    # Add metadata to the end of the page content, some RAG models don't have metadata.
                 chunks.append(chunk)    # Not sanitized because the page already was
         elif chunk_method=='None':
             text_splitter = None
             chunks = pages  # No chunking, take whole pages as documents
         else:
             raise NotImplementedError
         
@@ -332,20 +335,34 @@
                                         embedding=query_model,
                                         text_key='page_content',
                                         pinecone_api_key=os.getenv('PINECONE_API_KEY'))
         if show_progress:
             progress_percentage = 1
             my_bar.progress(progress_percentage, text=f'{progress_text}{progress_percentage*100:.2f}%')
     elif index_type == "ChromaDB":
+        # TODO add in collection metadata like this:
+        #         collection_metadata = {}
+        # if embeddings_model is not None:
+        #     model_name, model_type = get_embeddings_model_config(embeddings_model)
+        #     collection_metadata["model_name"] = model_name
+        #     collection_metadata["model_type"] = model_type
+
+        # if isinstance(relevance_score_fn, str):
+        #     assert relevance_score_fn in get_args(PredefinedRelevanceScoreFn)
+        #     collection_metadata["hnsw:space"] = relevance_score_fn
+        # else:
+        #     kwargs["relevance_score_fn"] = relevance_score_fn
+        # kwargs["collection_metadata"] = collection_metadata
+        # return Chroma(**kwargs)
         if clear:
             delete_index(index_type, index_name, rag_type, local_db_path=local_db_path)
         persistent_client = chromadb.PersistentClient(path=os.path.join(local_db_path,'chromadb'))            
         vectorstore = Chroma(client=persistent_client,
                                 collection_name=index_name,
-                                embedding_function=query_model)     
+                                embedding_function=query_model) 
         if show_progress:
             progress_percentage = 1
             my_bar.progress(progress_percentage, text=f'{progress_text}{progress_percentage*100:.2f}%')   
     elif index_type == "RAGatouille":
         if clear:
             delete_index(index_type, index_name, rag_type, local_db_path=local_db_path)
         if init_ragatouille:    
@@ -429,15 +446,15 @@
                 index_name: str,
                 vectorstore: any, 
                 chunker: dict, 
                 batch_size: int = 50, 
                 show_progress: bool = False,
                 local_db_path: str = '.'):
     """
-    Upserts documents into the specified index. Uses tenacity with exponential backoff to retry upserting documents.
+    Upserts documents into the specified index.
 
     Args:
         index_type (str): The type of index to upsert the documents into.
         index_name (str): The name of the index.
         vectorstore (any): The vectorstore object to add documents to.
         chunker (dict): The chunker dictionary containing the documents to upsert.
         batch_size (int, optional): The batch size for upserting documents. Defaults to 50.
@@ -613,170 +630,14 @@
             ragatouille_path = os.path.join(local_db_path, '.ragatouille/colbert/indexes', index_name)
             shutil.rmtree(ragatouille_path)
         except Exception as e:
             # print(f"Error occurred while deleting RAGatouille index: {e}")
             pass
     else:
         raise NotImplementedError
-def reduce_vector_query_size(rx_client:RAGxplorer,
-                             chroma_client:chromadb,
-                             vector_qty:int,
-                             verbose:bool=False):
-    """
-    Reduces the number of vectors in the RAGxplorer client to a specified quantity.
-
-    Args:
-        rx_client (RAGxplorer): The RAGxplorer client.
-        chroma_client (chromadb): The chromadb client.
-        vector_qty (int): The desired number of vectors.
-        verbose (bool, optional): Whether to print verbose output. Defaults to False.
-
-    Returns:
-        RAGxplorer: The updated RAGxplorer client with the reduced number of vectors.
-    """
-
-    ids = rx_client._vectordb.get()['ids']
-    embeddings = rag.get_doc_embeddings(rx_client._vectordb)
-    text = rag.get_docs(rx_client._vectordb)
-
-    if verbose:
-        print('Reducing the number of vectors from '+str(len(embeddings))+' to '+str(vector_qty)+'...')
-    indices = random.sample(range(len(embeddings)), vector_qty)
-    id = str(uuid.uuid4())[:8]
-    temp_index_name=rx_client._vectordb.name+'-'+id
-    
-    # Create a temporary index with the reduced number of vectors
-    chroma_client.create_collection(name=temp_index_name,embedding_function=rx_client._chosen_embedding_model)
-    temp_collection = chroma_client.get_collection(name=temp_index_name,embedding_function=rx_client._chosen_embedding_model)
-    temp_collection.add(
-        ids=[ids[i] for i in indices],
-        embeddings=[embeddings[i] for i in indices],
-        documents=[text[i] for i in indices]
-    )
-
-    # Replace the original index with the temporary one
-    rx_client._vectordb = temp_collection
-    rx_client._documents.embeddings = rag.get_doc_embeddings(rx_client._vectordb)
-    rx_client._documents.text = rag.get_docs(rx_client._vectordb)
-    rx_client._documents.ids = rx_client._vectordb.get()['ids']
-
-    if verbose:
-        print('Reduced number of vectors to '+str(len(rx_client._documents.embeddings))+' ✓')
-    return rx_client
-def export_data_viz(rx_client: RAGxplorer, df_export_path: str):
-    """
-    Exports the visualization data to a JSON file.
-
-    Args:
-        rx_client (RAGxplorer): The RAGxplorer object containing the visualization data.
-        df_export_path (str): The file path to export the JSON data.
-
-    Returns:
-        None
-    """
-    export_data = {
-        'visualization_index_name': rx_client._vectordb.name,
-        'umap_params': rx_client._projector.get_params(),
-        'viz_data': rx_client._VizData.base_df.to_json(orient='split')
-    }
-
-    # Save the data to a JSON file
-    with open(df_export_path, 'w') as f:
-        json.dump(export_data, f, indent=4)
-def create_data_viz(index_selected: str,
-                    rx_client: RAGxplorer,
-                    chroma_client: PersistentClient,
-                    umap_params: dict = {'n_neighbors': 5, 'n_components': 2, 'random_state': 42},
-                    limit_size_qty: int = None,
-                    df_export_path: str = None,
-                    show_progress: bool = False):
-    """
-    Creates data visualization using RAGxplorer and PersistentClient.
-
-    Args:
-        index_selected (str): The name of the collection to load from chroma_client.
-        rx_client (RAGxplorer): An instance of RAGxplorer class.
-        chroma_client (PersistentClient): An instance of PersistentClient class.
-        umap_params (dict, optional): UMAP parameters for embedding. Defaults to {'n_neighbors': 5, 'n_components': 2, 'random_state': 42}.
-        limit_size_qty (int, optional): The maximum number of vectors to include in the visualization. Defaults to None.
-        df_export_path (str, optional): The file path to export the visualization data. Defaults to None.
-        show_progress (bool, optional): Whether to show progress bar. Defaults to False.
-
-    Returns:
-        tuple: A tuple containing the updated rx_client and chroma_client instances.
-    """
-    if show_progress:
-        my_bar = st.progress(0, text='Loading collection...')
-    
-    # Load collection from chroma_client
-    collection = chroma_client.get_collection(name=index_selected,
-                                              embedding_function=rx_client._chosen_embedding_model)
-    rx_client.load_chroma(collection,
-                          umap_params=umap_params,
-                          initialize_projector=True)
-    
-    if limit_size_qty:
-        if show_progress:
-            my_bar.progress(0.25, text='Reducing vector query size...')
-        
-        # Reduce vector query size
-        rx_client = reduce_vector_query_size(rx_client,
-                                             chroma_client,
-                                             vector_qty=limit_size_qty,
-                                             verbose=True)
-    
-    if show_progress:
-        my_bar.progress(0.5, text='Projecting embeddings for visualization...')
-    
-    # Run projector
-    rx_client.run_projector()
-    
-    if show_progress:
-        my_bar.progress(1, text='Projecting complete!')
-    
-    if df_export_path:
-        # Export data visualization
-        export_data_viz(rx_client, df_export_path)
-    
-    if show_progress:
-        my_bar.empty()
-    
-    return rx_client, chroma_client
-def visualize_data(index_selected: str,
-                   rx_client: RAGxplorer,
-                   chroma_client: PersistentClient,
-                   query: str,
-                   umap_params: dict = {'n_neighbors': 5, 'n_components': 2, 'random_state': 42},
-                   import_file: bool = True):
-    """
-    Visualizes data using RAGxplorer and PersistentClient.
-
-    Args:
-        index_selected (str): The name of the selected index.
-        rx_client (RAGxplorer): An instance of the RAGxplorer class.
-        chroma_client (PersistentClient): An instance of the PersistentClient class.
-        query (str): The query to visualize.
-        umap_params (dict, optional): UMAP parameters for data visualization. Defaults to {'n_neighbors': 5, 'n_components': 2, 'random_state': 42}.
-        import_file (bool, optional): Whether to import data from a file. Defaults to True.
-
-    Returns:
-        Tuple[RAGxplorer, PersistentClient]: A tuple containing the updated instances of RAGxplorer and PersistentClient.
-    """
-    if import_file:
-        with open(import_file, 'r') as f:
-            data = json.load(f)
-        viz_data = pd.read_json(data['viz_data'], orient='split')
-        collection = chroma_client.get_collection(name=index_selected, embedding_function=rx_client._chosen_embedding_model)
-        rx_client.load_chroma(collection, umap_params=umap_params, initialize_projector=True)
-        fig = rx_client.visualize_query(query, import_projection_data=viz_data)
-    else:
-        fig = rx_client.visualize_query(query)
-    st.plotly_chart(fig, use_container_width=True)
-
-    return rx_client, chroma_client
 def _sanitize_raw_page_data(page):
     """
     Sanitizes the raw page data by removing unnecessary information and checking for meaningful content.
     If pages are merged, this must happen before the merging occurs.
 
     Args:
         page (Page): The raw page data to be sanitized.
@@ -856,7 +717,202 @@
     Args:
         metadata (dict): The metadata dictionary to be hashed.
 
     Returns:
         str: The hexadecimal representation of the hashed metadata.
     """
     return hashlib.sha1(json.dumps(metadata, sort_keys=True).encode()).hexdigest()
+def _check_db_name(index_type:str,index_name:object):
+    if index_type=="Pinecone":
+        if len(index_name)>45:
+            raise ValueError(f'The Pinecone index name must be less than 45 characters. Entry: {index_name}')
+    elif index_type=="ChromaDB":
+        if len(index_name) > 63:
+            raise ValueError(f'The ChromaDB collection name must be less than 63 characters. Entry: {index_name}')
+        if not index_name[0].isalnum() or not index_name[-1].isalnum():
+            raise ValueError(f'The ChromaDB collection name must start and end with an alphanumeric character. Entry: {index_name}')
+        if not re.match(r'^[a-zA-Z0-9_-]+$', index_name):
+            raise ValueError(f'The ChromaDB collection name can only contain alphanumeric characters, underscores, or hyphens. Entry: {index_name}')
+        if '..' in index_name:
+            raise ValueError(f'The ChromaDB collection name cannot contain two consecutive periods. Entry: {index_name}')
+
+### Stuff to test out spotlight
+
+def get_or_create_spotlight_viewer(df:pd.DataFrame,host:str='0.0.0.0',port:int=9000):
+    viewers = spotlight.viewers()
+    if viewers:
+        for viewer in viewers[:-1]:
+            viewer.close()
+        existing_viewer=spotlight.viewers()[-1]
+        return existing_viewer
+    
+    new_viewer = spotlight.show(df,
+                          wait='auto',
+                          dtype={"used_by_questions": spotlight_dtypes.SequenceDType(spotlight_dtypes.str_dtype)},
+                          host=host,
+                          port=port)
+
+    return new_viewer
+def get_docs_questions_df(
+        docs_db_directory: Path,
+        docs_db_collection: str,
+        questions_db_directory: Path,
+        questions_db_collection: str,
+        query_model:object):
+    """
+    Retrieves and combines documents and questions dataframes.
+
+    Args:
+        docs_db_directory (Path): The directory of the documents database.
+        docs_db_collection (str): The name of the documents database collection.
+        questions_db_directory (Path): The directory of the questions database.
+        questions_db_collection (str): The name of the questions database collection.
+        query_model (object): The query model object.
+
+    Returns:
+        pd.DataFrame: The combined dataframe containing documents and questions data.
+    """
+    # TODO there's definitely a way to not have to pass query_model, since it should be possible to pull from the db, try to remove this in future versions
+
+    # Check if there exists a query database
+    chroma_collections = [collection.name for collection in admin.show_chroma_collections(format=False)['message']]
+    matching_collection = [collection for collection in chroma_collections if collection == questions_db_collection]
+    if len(matching_collection) > 1:
+        raise Exception('Matching collection not found or multiple matching collections found.')
+    try:
+        if not matching_collection:
+            raise Exception('Query database not found. Please create a query database using the Chatbot page and a selected index.')
+    except Exception as e:
+        st.warning(f"{e}")
+        st.stop()
+    st.markdown(f"Query database found: {questions_db_collection}")
+
+    docs_df = get_docs_df(docs_db_directory, docs_db_collection, query_model)
+    docs_df["type"] = "doc"
+    questions_df = get_questions_df(questions_db_directory, questions_db_collection, query_model)
+    questions_df["type"] = "question"
+
+    questions_df["num_sources"] = questions_df["sources"].apply(len)
+    questions_df["first_source"] = questions_df["sources"].apply(
+        lambda x: next(iter(x), None)
+    )
+
+    if len(questions_df):
+        docs_df["used_by_questions"] = docs_df["id"].apply(
+            lambda doc_id: questions_df[
+                questions_df["sources"].apply(lambda sources: doc_id in sources)
+            ]["id"].tolist()
+        )
+    else:
+        docs_df["used_by_questions"] = [[] for _ in range(len(docs_df))]
+    docs_df["used_by_num_questions"] = docs_df["used_by_questions"].apply(len)
+    docs_df["used_by_question_first"] = docs_df["used_by_questions"].apply(
+        lambda x: next(iter(x), None)
+    )
+
+    df = pd.concat([docs_df, questions_df], ignore_index=True)
+    return df
+def get_docs_df(local_db_path: Path, index_name: str, query_model: object):
+    """
+    Retrieves documents from a Chroma database and returns them as a pandas DataFrame.
+
+    Args:
+        local_db_path (Path): The local path to the Chroma database.
+        index_name (str): The name of the collection in the Chroma database.
+        query_model (object): The embedding function used for querying the database.
+
+    Returns:
+        pd.DataFrame: A DataFrame containing the retrieved documents, along with their metadata and embeddings.
+            The DataFrame has the following columns:
+            - id: The ID of the document.
+            - source: The source of the document.
+            - page: The page number of the document (default: -1 if not available).
+            - document: The content of the document.
+            - embedding: The embedding of the document.
+    """
+    persistent_client = chromadb.PersistentClient(path=os.path.join(local_db_path,'chromadb'))            
+    vectorstore = Chroma(client=persistent_client,
+                            collection_name=index_name,
+                            embedding_function=query_model) 
+
+    response = vectorstore.get(include=["metadatas", "documents", "embeddings"])
+    return pd.DataFrame(
+        {
+            "id": response["ids"],
+            "source": [metadata.get("source") for metadata in response["metadatas"]],
+            "page": [metadata.get("page", -1) for metadata in response["metadatas"]],
+            "document": response["documents"],
+            "embedding": response["embeddings"],
+        }
+    )
+def get_questions_df(local_db_path: Path, index_name: str, query_model: object):
+    """
+    Retrieves questions and related information from a Chroma database and returns them as a pandas DataFrame.
+
+    Args:
+        local_db_path (Path): The local path to the Chroma database.
+        index_name (str): The name of the collection in the Chroma database.
+        query_model (object): The embedding function used for querying the Chroma database.
+
+    Returns:
+        pd.DataFrame: A DataFrame containing the retrieved questions, answers, sources, and embeddings.
+    """
+    persistent_client = chromadb.PersistentClient(path=os.path.join(local_db_path,'chromadb'))            
+    vectorstore = Chroma(client=persistent_client,
+                            collection_name=index_name,
+                            embedding_function=query_model) 
+
+    response = vectorstore.get(include=["metadatas", "documents", "embeddings"])
+    return pd.DataFrame(
+        {
+            "id": response["ids"],
+            "question": response["documents"],
+            "answer": [metadata.get("answer") for metadata in response["metadatas"]],
+            "sources": [
+                metadata.get("sources").split(",") for metadata in response["metadatas"]
+            ],
+            "embedding": response["embeddings"],
+        }
+    )
+def add_clusters(df:pd,n_clusters:int,label_llm:object=None,doc_per_cluster:int=5):
+    """
+    Add clusters to a DataFrame based on the embeddings of its documents.
+
+    Args:
+        df (pd.DataFrame): The DataFrame containing the documents and their embeddings.
+        n_clusters (int): The number of clusters to create.
+        label_llm (object, optional): The label language model to use for generating cluster labels. Defaults to None.
+        doc_per_cluster (int, optional): The number of documents to sample per cluster for label generation. Defaults to 5.
+
+    Returns:
+        pd.DataFrame: The DataFrame with the added cluster information.
+    """
+    matrix = np.vstack(df.embedding.values)
+    kmeans = KMeans(n_clusters=n_clusters, init="k-means++", random_state=42)
+    kmeans.fit(matrix)
+    labels = kmeans.labels_
+    df["Cluster"] = labels
+
+    summary=[]
+    if label_llm is not None:
+        for i in range(n_clusters):
+            print(f"Cluster {i} Theme:")
+            chunks =  df[df.Cluster == i].document.sample(doc_per_cluster, random_state=42)
+            llm_chain = CLUSTER_LABEL | label_llm
+            summary.append(llm_chain.invoke(chunks))
+            print(summary[-1].content)
+        df["Cluster_Label"] = [summary[i].content for i in df["Cluster"]]
+    
+    return df
+def export_to_hf_dataset(df: pd.DataFrame, dataset_name: str):
+    """
+    Export a pandas DataFrame to a Hugging Face dataset and push it to the Hugging Face Hub.
+
+    Args:
+        df (pd.DataFrame): The pandas DataFrame to be exported.
+        dataset_name (str): The name of the dataset to be created in the Hugging Face Hub.
+
+    Returns:
+        None
+    """
+    hf_dataset = Dataset.from_pandas(df)
+    hf_dataset.push_to_hub(dataset_name, token=os.getenv('HUGGINGFACEHUB_API_TOKEN'))
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `aerospace_chatbot-0.0.5/src/aerospace_chatbot/prompts.py` & `aerospace_chatbot-0.0.6/src/aerospace_chatbot/prompts.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,10 +6,11 @@
 QA_PROMPT=hub.pull("dmueller/ams-chatbot-qa-retrieval")
 QA_WSOURCES_PROMPT=hub.pull("dmueller/ams-chatbot-qa-retrieval-wsources")
 QA_GENERATE_PROMPT=hub.pull("dmueller/generate_qa_prompt")
 SUMMARIZE_TEXT=hub.pull("dmueller/summarize_text")
 TEST_QUERY_PROMPT='What are examples of adhesives to use when potting motors for launch vehicle or spacecraft mechanisms?'
 GENERATE_SIMILAR_QUESTIONS=hub.pull("dmueller/generate_similar_questions")
 GENERATE_SIMILAR_QUESTIONS_W_CONTEXT=hub.pull("dmueller/generate_similar_questions_w_context")
+CLUSTER_LABEL=hub.pull("dmueller/cluster-label")
 
 # Prompts defined here only
 DEFAULT_DOCUMENT_PROMPT = PromptTemplate.from_template(template="{page_content}")
```

### Comparing `aerospace_chatbot-0.0.5/src/aerospace_chatbot/queries.py` & `aerospace_chatbot-0.0.6/src/aerospace_chatbot/queries.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 from pathlib import Path
 
 import openai
 import pinecone
 from pinecone import Pinecone as pinecone_client
 import chromadb
 
+from langchain_core.documents import Document
+
 from langchain_openai import ChatOpenAI
 
 from langchain_pinecone import Pinecone
 from langchain_community.vectorstores import Chroma
 
 from langchain.memory import ConversationBufferMemory
 
@@ -23,123 +25,139 @@
 
 from operator import itemgetter
 from langchain_core.output_parsers import StrOutputParser
 from langchain_core.runnables import RunnableLambda, RunnablePassthrough
 from langchain.schema import format_document
 from langchain_core.messages import get_buffer_string
 
+import data_processing
 from prompts import CONDENSE_QUESTION_PROMPT, QA_PROMPT, DEFAULT_DOCUMENT_PROMPT, GENERATE_SIMILAR_QUESTIONS, GENERATE_SIMILAR_QUESTIONS_W_CONTEXT
 
-# Set secrets from environment file
-OPENAI_API_KEY=os.getenv('OPENAI_API_KEY')
-VOYAGE_API_KEY=os.getenv('VOYAGE_API_KEY')
-PINECONE_API_KEY=os.getenv('PINECONE_API_KEY')
-HUGGINGFACEHUB_API_TOKEN=os.getenv('HUGGINGFACEHUB_API_TOKEN') 
-
 # Class and functions
 class QA_Model:
     """
     Represents a Question-Answering Model.
 
     Args:
-        index_type (str): The type of index.
-        index_name (str): The name of the index.
+        index_type (str): The type of document index.
+        index_name (str): The name of the document index.
         query_model (str): The query model.
         llm (ChatOpenAI): The language model for generating responses.
         rag_type (str, optional): The type of RAG model. Defaults to 'Standard'.
         k (int, optional): The number of retriever results to consider. Defaults to 6.
         search_type (str, optional): The type of search to perform. Defaults to 'similarity'.
         fetch_k (int, optional): The number of documents to fetch from the retriever. Defaults to 50.
         temperature (int, optional): The temperature for response generation. Defaults to 0.
         local_db_path (str, optional): The path to the local database. Defaults to '.'.
 
     Attributes:
-        index_type (str): The type of index.
-        index_name (str): The name of the index.
+        index_type (str): The type of document index.
+        index_name (str): The name of the document index.
         query_model (str): The query model.
         llm (ChatOpenAI): The language model for generating responses.
         rag_type (str): The type of RAG model.
         k (int): The number of retriever results to consider.
         search_type (str): The type of search to perform.
         fetch_k (int): The number of documents to fetch from the retriever.
         temperature (int): The temperature for response generation.
         local_db_path (str): The path to the local database.
-        sources (list): The list of sources for the retrieved documents.
-        vectorstore (VectorStore): The vector store for document retrieval.
-        retriever (Retriever): The retriever for document retrieval.
         memory (ConversationBufferMemory): The memory for conversation history.
+        result (dict): The result of the query.
+        sources (list): The list of sources for the retrieved documents.
+        ai_response (str): The response generated by the AI.
         conversational_qa_chain (Chain): The chain for conversational QA.
+        doc_vectorstore (VectorStore): The vector store for document retrieval.
+        query_vectorstore (VectorStore): The vector store for query retrieval. Only created with ChromaDB index_type.
+        retriever (Retriever): The retriever for document retrieval.
 
     """
     def __init__(self, 
                  index_type:str,
                  index_name:str,
                  query_model:object,
                  llm:ChatOpenAI,
                  rag_type:str='Standard',
                  k:int=6,
                  search_type:str='similarity',
                  fetch_k:int=50,
                  temperature:int=0,
-                 local_db_path:str='.'):
+                 local_db_path:str='.',
+                 reset_query_db:bool=False):
         """
         Initializes a new instance of the QA_Model class.
 
         Args:
-            index_type (str): The type of index.
-            index_name (str): The name of the index.
+            index_type (str): The type of document index.
+            index_name (str): The name of the document index.
             query_model (object): The query model.
             llm (ChatOpenAI): The language model for generating responses.
             rag_type (str, optional): The type of RAG model. Defaults to 'Standard'.
             k (int, optional): The number of retriever results to consider. Defaults to 6. 
             search_type (str, optional): The type of search to perform. Defaults to 'similarity'. Does not apply to RAGatouille.
             fetch_k (int, optional): The number of documents to fetch from the retriever. Defaults to 50. Does not apply to RAGatouille.
             temperature (int, optional): The temperature for response generation. Defaults to 0.
             local_db_path (str, optional): The path to the local database. Defaults to '.'.
+            reset_query_db (bool, optional): Whether to reset the query database. Defaults to False.
 
         """
         self.index_type=index_type
         self.index_name=index_name
         self.query_model=query_model
         self.llm=llm
         self.rag_type=rag_type
         self.k=k
         self.search_type=search_type
         self.fetch_k=fetch_k
         self.temperature=temperature
         self.local_db_path=local_db_path
+
         self.memory=None
         self.result=None
         self.sources=None
         self.ai_response=None
+        self.conversational_qa_chain=None
 
+        self.doc_vectorstore=None
+        self.query_vectorstore=None
+        self.retriever=None
 
         # Define retriever search parameters
         search_kwargs = _process_retriever_args(self.search_type,
                                                 self.k,
                                                 self.fetch_k)
 
         # Read in from the vector database
-        self.vectorstore=data_processing.initialize_database(self.index_type,
+        self.doc_vectorstore=data_processing.initialize_database(self.index_type,
                                                              self.index_name,
                                                              self.query_model,
                                                              self.rag_type,
                                                              local_db_path=self.local_db_path,
+                                                             clear=False,
                                                              init_ragatouille=False)  
+        
+        # Iniialize a database to capture queries in a temp database
+        if self.index_type=='ChromaDB':
+            self.query_vectorstore=data_processing.initialize_database(self.index_type,
+                                                                 self.index_name+'-queries',
+                                                                 self.query_model,
+                                                                 'Standard',    # Regardless of doc_vectorstore, query_vectorstore is always Standard
+                                                                 local_db_path=self.local_db_path,
+                                                                 clear=reset_query_db)
 
+        # Initialize retriever
         if self.rag_type=='Standard':  
             if self.index_type=='ChromaDB' or self.index_type=='Pinecone':
-                self.retriever=self.vectorstore.as_retriever(search_type=self.search_type,
-                                                             search_kwargs=search_kwargs)
+                self.retriever=self.doc_vectorstore.as_retriever(search_type=self.search_type,
+                                                                 search_kwargs=search_kwargs)
             elif self.index_type=='RAGatouille':
-                self.retriever=self.vectorstore.as_langchain_retriever(k=search_kwargs['k'])  
+                self.retriever=self.doc_vectorstore.as_langchain_retriever(k=search_kwargs['k'])  
         elif self.rag_type=='Parent-Child' or self.rag_type=='Summary':
             self.lfs = LocalFileStore(Path(self.local_db_path).resolve() / 'local_file_store' / self.index_name)
             self.retriever = MultiVectorRetriever(
-                                vectorstore=self.vectorstore,
+                                vectorstore=self.doc_vectorstore,
                                 byte_store=self.lfs,
                                 id_key="doc_id",
                                 search_type=self.search_type,
                                 search_kwargs=search_kwargs)
         else:
             raise NotImplementedError
 
@@ -157,24 +175,32 @@
 
         Args:
             query (str): The query string.
 
         Returns:
             None
         """       
+
+        # Retrieve memory, invoke chain
         self.memory.load_memory_variables({})
+
+        # TODO add error checking for max token length of a given model.
         self.result = self.conversational_qa_chain.invoke({'question': query})
 
+        # Add sources to response
         self.sources = '\n'.join(str(data.metadata) for data in self.result['references'])
         if self.llm.__class__.__name__=='ChatOpenAI':
             self.ai_response = self.result['answer'].content + '\n\nSources:\n' + self.sources
         else:
             raise NotImplementedError
-
         self.memory.save_context({'question': query}, {'answer': self.ai_response})
+
+        # If ChromaDB type, upsert query into query database
+        if self.index_type=='ChromaDB':
+            self.query_vectorstore.add_documents([_question_as_doc(query, self.result)])
         
     def update_model(self,
                      llm:ChatOpenAI):
         """
         Updates with a new LLM.
 
         Args:
@@ -313,8 +339,18 @@
 
     # Implement filtering and number of documents to return
     if search_type=='mmr':
         search_kwargs={'k':k,'fetch_k':fetch_k} # See as_retriever docs for parameters
     else:
         search_kwargs={'k':k} # See as_retriever docs for parameters
     
-    return search_kwargs
+    return search_kwargs
+def _question_as_doc(question: str, rag_answer: dict):    
+    sources = [data.metadata for data in rag_answer['references']]
+
+    return Document(
+        page_content=question,
+        metadata={
+            "answer": rag_answer['answer'].content,
+            "sources": ",".join(map(data_processing._stable_hash_meta, sources)),
+        },
+    )
```

### Comparing `aerospace_chatbot-0.0.5/PKG-INFO` & `aerospace_chatbot-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aerospace-chatbot
-Version: 0.0.5
+Version: 0.0.6
 Summary: Aerospace engineering chatbot and AI tools.
 Home-page: https://github.com/dan-s-mueller/aerospace_chatbot/tree/main
 License: MIT
 Author: dsmueller
 Author-email: dsm@danmueller.pro
 Requires-Python: >3.9.7,<3.12
 Classifier: License :: OSI Approved :: MIT License
@@ -28,16 +28,15 @@
 Requires-Dist: pinecone-client (>=3.2.0,<4.0.0)
 Requires-Dist: pydantic (>=2.6.0,<3.0.0)
 Requires-Dist: pypdf (>=3.17.4,<4.0.0)
 Requires-Dist: pytest (>=8.1.1,<9.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: ragas (>=0.1.6,<0.2.0)
 Requires-Dist: ragatouille (>=0.0.8.post2,<0.0.9)
-Requires-Dist: ragxplorer (>=0.1.10,<0.2.0)
-Requires-Dist: renumics-spotlight (>=1.6.8,<2.0.0)
+Requires-Dist: renumics-spotlight (==1.6.5)
 Requires-Dist: sentence-transformers (>=2.2.2,<3.0.0)
 Requires-Dist: sphinx (==7.2.6)
 Requires-Dist: sphinx-design (>=0.5.0,<0.6.0)
 Requires-Dist: sphinx-rtd-theme (==2.0.0)
 Requires-Dist: sphinxawesome-theme (>=5.1.1,<6.0.0)
 Requires-Dist: streamlit (>=1.29.0,<2.0.0)
 Requires-Dist: streamlit-authenticator (>=0.3.1,<0.4.0)
```

