# Comparing `tmp/ptal_api-1.0.0a6.tar.gz` & `tmp/ptal_api-1.0.0a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ptal_api-1.0.0a6.tar", max compression
+gzip compressed data, was "ptal_api-1.0.0a7.tar", max compression
```

## Comparing `ptal_api-1.0.0a6.tar` & `ptal_api-1.0.0a7.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0      627 2024-03-11 14:05:21.304489 ptal_api-1.0.0a6/README.md
--rw-r--r--   0        0        0        0 2024-03-11 14:05:21.332489 ptal_api-1.0.0a6/ptal_api/__init__.py
--rw-r--r--   0        0        0   132132 2024-03-11 14:05:21.304489 ptal_api-1.0.0a6/ptal_api/adapter.py
--rw-r--r--   0        0        0      184 2024-03-11 14:05:21.304489 ptal_api-1.0.0a6/ptal_api/core/kb_sync/kb_iterator_config.py
--rw-r--r--   0        0        0      160 2024-03-11 14:05:21.304489 ptal_api-1.0.0a6/ptal_api/core/kb_sync/object_time_interval.py
--rw-r--r--   0        0        0      484 2024-03-11 14:05:21.304489 ptal_api-1.0.0a6/ptal_api/core/query_factory.py
--rw-r--r--   0        0        0      435 2024-03-11 14:05:21.304489 ptal_api-1.0.0a6/ptal_api/core/type_mapper/app_settings/logging.conf
--rw-r--r--   0        0        0      737 2024-03-11 14:05:21.304489 ptal_api-1.0.0a6/ptal_api/core/type_mapper/common/common.py
--rw-r--r--   0        0        0    14955 2024-03-11 14:05:21.304489 ptal_api-1.0.0a6/ptal_api/core/type_mapper/data_model/base_data_model.py
--rw-r--r--   0        0        0      904 2024-03-11 14:05:21.304489 ptal_api-1.0.0a6/ptal_api/core/type_mapper/data_model/config_data_model.py
--rw-r--r--   0        0        0     3255 2024-03-11 14:05:21.304489 ptal_api-1.0.0a6/ptal_api/core/type_mapper/data_model/custom_data_model.py
--rw-r--r--   0        0        0     3501 2024-03-11 14:05:21.304489 ptal_api-1.0.0a6/ptal_api/core/type_mapper/model_parameters/name_code_mapping.yml
--rw-r--r--   0        0        0     2194 2024-03-11 14:05:21.304489 ptal_api-1.0.0a6/ptal_api/core/type_mapper/modules/custom_data_handler.py
--rw-r--r--   0        0        0     1464 2024-03-11 14:05:21.304489 ptal_api-1.0.0a6/ptal_api/core/type_mapper/modules/file_generator.py
--rw-r--r--   0        0        0     4556 2024-03-11 14:05:21.304489 ptal_api-1.0.0a6/ptal_api/core/type_mapper/modules/object_name_transformer.py
--rw-r--r--   0        0        0    23314 2024-03-11 14:05:21.304489 ptal_api-1.0.0a6/ptal_api/core/type_mapper/modules/type_mapping_generator.py
--rw-r--r--   0        0        0     1800 2024-03-11 14:05:21.304489 ptal_api-1.0.0a6/ptal_api/core/type_mapper/modules/type_mapping_loader/type_mapping_loader.py
--rw-r--r--   0        0        0      418 2024-03-11 14:05:21.304489 ptal_api-1.0.0a6/ptal_api/core/type_mapper/modules/type_mapping_loader/type_mapping_loader_interface.py
--rw-r--r--   0        0        0      387 2024-03-11 14:05:21.304489 ptal_api-1.0.0a6/ptal_api/core/values/date_dataclass.py
--rw-r--r--   0        0        0     5991 2024-03-11 14:05:21.304489 ptal_api-1.0.0a6/ptal_api/core/values/value_mapping.py
--rw-r--r--   0        0        0      348 2024-03-11 14:05:21.304489 ptal_api-1.0.0a6/ptal_api/pretty_adapter/common.py
--rw-r--r--   0        0        0     1901 2024-03-11 14:05:21.304489 ptal_api-1.0.0a6/ptal_api/pretty_adapter/object_types.py
--rw-r--r--   0        0        0     2884 2024-03-11 14:05:21.304489 ptal_api-1.0.0a6/ptal_api/pretty_adapter/objects.py
--rw-r--r--   0        0        0     3766 2024-03-11 14:05:21.304489 ptal_api-1.0.0a6/ptal_api/pretty_adapter/pretty_adapter.py
--rw-r--r--   0        0        0      850 2024-03-11 14:05:21.304489 ptal_api-1.0.0a6/ptal_api/pretty_adapter/property_values.py
--rw-r--r--   0        0        0    17534 2024-03-11 14:05:21.304489 ptal_api-1.0.0a6/ptal_api/pretty_adapter/transformer.py
--rw-r--r--   0        0        0        0 2024-03-11 14:05:21.332489 ptal_api-1.0.0a6/ptal_api/providers/__init__.py
--rw-r--r--   0        0        0     7328 2024-03-11 14:05:21.304489 ptal_api-1.0.0a6/ptal_api/providers/gql_providers.py
--rw-r--r--   0        0        0     1094 2024-03-11 14:05:21.304489 ptal_api-1.0.0a6/ptal_api/schema/README.md
--rw-r--r--   0        0        0        0 2024-03-11 14:05:21.332489 ptal_api-1.0.0a6/ptal_api/schema/__init__.py
--rw-r--r--   0        0        0   312941 2024-03-11 14:05:21.308489 ptal_api-1.0.0a6/ptal_api/schema/api_schema.py
--rw-r--r--   0        0        0    93674 2024-03-11 14:05:21.308489 ptal_api-1.0.0a6/ptal_api/schema/crawlers_api_schema.py
--rw-r--r--   0        0        0    79293 2024-03-11 14:05:21.308489 ptal_api-1.0.0a6/ptal_api/schema/tcontroller_api_schema.py
--rw-r--r--   0        0        0     3732 2024-03-11 14:05:21.308489 ptal_api-1.0.0a6/ptal_api/schema/translator_api_schema.py
--rw-r--r--   0        0        0   162313 2024-03-11 14:05:21.308489 ptal_api-1.0.0a6/ptal_api/schema/utils_api_schema.py
--rw-r--r--   0        0        0     3662 2024-03-11 14:05:21.308489 ptal_api-1.0.0a6/ptal_api/scripts/type_mapper.py
--rw-r--r--   0        0        0        0 2024-03-11 14:05:21.332489 ptal_api-1.0.0a6/ptal_api/tdm_builder/__init__.py
--rw-r--r--   0        0        0     1211 2024-03-11 14:05:21.308489 ptal_api-1.0.0a6/ptal_api/tdm_builder/tdm_builder.py
--rw-r--r--   0        0        0     1913 2024-03-11 14:05:21.308489 ptal_api-1.0.0a6/pyproject.toml
--rw-r--r--   0        0        0     1616 1970-01-01 00:00:00.000000 ptal_api-1.0.0a6/PKG-INFO
+-rw-r--r--   0        0        0      627 2024-05-08 09:41:08.393047 ptal_api-1.0.0a7/README.md
+-rw-r--r--   0        0        0        0 2024-05-08 09:41:08.457047 ptal_api-1.0.0a7/ptal_api/__init__.py
+-rw-r--r--   0        0        0   132132 2024-05-08 09:41:08.397047 ptal_api-1.0.0a7/ptal_api/adapter.py
+-rw-r--r--   0        0        0      184 2024-05-08 09:41:08.397047 ptal_api-1.0.0a7/ptal_api/core/kb_sync/kb_iterator_config.py
+-rw-r--r--   0        0        0      160 2024-05-08 09:41:08.397047 ptal_api-1.0.0a7/ptal_api/core/kb_sync/object_time_interval.py
+-rw-r--r--   0        0        0      484 2024-05-08 09:41:08.397047 ptal_api-1.0.0a7/ptal_api/core/query_factory.py
+-rw-r--r--   0        0        0      435 2024-05-08 09:41:08.397047 ptal_api-1.0.0a7/ptal_api/core/type_mapper/app_settings/logging.conf
+-rw-r--r--   0        0        0      737 2024-05-08 09:41:08.397047 ptal_api-1.0.0a7/ptal_api/core/type_mapper/common/common.py
+-rw-r--r--   0        0        0    14955 2024-05-08 09:41:08.397047 ptal_api-1.0.0a7/ptal_api/core/type_mapper/data_model/base_data_model.py
+-rw-r--r--   0        0        0      904 2024-05-08 09:41:08.397047 ptal_api-1.0.0a7/ptal_api/core/type_mapper/data_model/config_data_model.py
+-rw-r--r--   0        0        0     3255 2024-05-08 09:41:08.397047 ptal_api-1.0.0a7/ptal_api/core/type_mapper/data_model/custom_data_model.py
+-rw-r--r--   0        0        0     3501 2024-05-08 09:41:08.397047 ptal_api-1.0.0a7/ptal_api/core/type_mapper/model_parameters/name_code_mapping.yml
+-rw-r--r--   0        0        0     2194 2024-05-08 09:41:08.397047 ptal_api-1.0.0a7/ptal_api/core/type_mapper/modules/custom_data_handler.py
+-rw-r--r--   0        0        0     1464 2024-05-08 09:41:08.397047 ptal_api-1.0.0a7/ptal_api/core/type_mapper/modules/file_generator.py
+-rw-r--r--   0        0        0     4556 2024-05-08 09:41:08.397047 ptal_api-1.0.0a7/ptal_api/core/type_mapper/modules/object_name_transformer.py
+-rw-r--r--   0        0        0    23314 2024-05-08 09:41:08.397047 ptal_api-1.0.0a7/ptal_api/core/type_mapper/modules/type_mapping_generator.py
+-rw-r--r--   0        0        0     1800 2024-05-08 09:41:08.397047 ptal_api-1.0.0a7/ptal_api/core/type_mapper/modules/type_mapping_loader/type_mapping_loader.py
+-rw-r--r--   0        0        0      418 2024-05-08 09:41:08.397047 ptal_api-1.0.0a7/ptal_api/core/type_mapper/modules/type_mapping_loader/type_mapping_loader_interface.py
+-rw-r--r--   0        0        0      387 2024-05-08 09:41:08.397047 ptal_api-1.0.0a7/ptal_api/core/values/date_dataclass.py
+-rw-r--r--   0        0        0     5991 2024-05-08 09:41:08.397047 ptal_api-1.0.0a7/ptal_api/core/values/value_mapping.py
+-rw-r--r--   0        0        0      348 2024-05-08 09:41:08.397047 ptal_api-1.0.0a7/ptal_api/pretty_adapter/common.py
+-rw-r--r--   0        0        0     1901 2024-05-08 09:41:08.397047 ptal_api-1.0.0a7/ptal_api/pretty_adapter/object_types.py
+-rw-r--r--   0        0        0     2884 2024-05-08 09:41:08.401047 ptal_api-1.0.0a7/ptal_api/pretty_adapter/objects.py
+-rw-r--r--   0        0        0     3766 2024-05-08 09:41:08.401047 ptal_api-1.0.0a7/ptal_api/pretty_adapter/pretty_adapter.py
+-rw-r--r--   0        0        0      850 2024-05-08 09:41:08.401047 ptal_api-1.0.0a7/ptal_api/pretty_adapter/property_values.py
+-rw-r--r--   0        0        0    17534 2024-05-08 09:41:08.401047 ptal_api-1.0.0a7/ptal_api/pretty_adapter/transformer.py
+-rw-r--r--   0        0        0        0 2024-05-08 09:41:08.461048 ptal_api-1.0.0a7/ptal_api/providers/__init__.py
+-rw-r--r--   0        0        0     7328 2024-05-08 09:41:08.401047 ptal_api-1.0.0a7/ptal_api/providers/gql_providers.py
+-rw-r--r--   0        0        0     1094 2024-05-08 09:41:08.401047 ptal_api-1.0.0a7/ptal_api/schema/README.md
+-rw-r--r--   0        0        0        0 2024-05-08 09:41:08.461048 ptal_api-1.0.0a7/ptal_api/schema/__init__.py
+-rw-r--r--   0        0        0   312895 2024-05-08 09:41:08.401047 ptal_api-1.0.0a7/ptal_api/schema/api_schema.py
+-rw-r--r--   0        0        0    94569 2024-05-08 09:41:08.405047 ptal_api-1.0.0a7/ptal_api/schema/crawlers_api_schema.py
+-rw-r--r--   0        0        0    79675 2024-05-08 09:41:08.405047 ptal_api-1.0.0a7/ptal_api/schema/tcontroller_api_schema.py
+-rw-r--r--   0        0        0     3732 2024-05-08 09:41:08.405047 ptal_api-1.0.0a7/ptal_api/schema/translator_api_schema.py
+-rw-r--r--   0        0        0   158744 2024-05-08 09:41:08.405047 ptal_api-1.0.0a7/ptal_api/schema/utils_api_schema.py
+-rw-r--r--   0        0        0     3662 2024-05-08 09:41:08.405047 ptal_api-1.0.0a7/ptal_api/scripts/type_mapper.py
+-rw-r--r--   0        0        0        0 2024-05-08 09:41:08.461048 ptal_api-1.0.0a7/ptal_api/tdm_builder/__init__.py
+-rw-r--r--   0        0        0     1211 2024-05-08 09:41:08.405047 ptal_api-1.0.0a7/ptal_api/tdm_builder/tdm_builder.py
+-rw-r--r--   0        0        0     1913 2024-05-08 09:41:08.405047 ptal_api-1.0.0a7/pyproject.toml
+-rw-r--r--   0        0        0     1616 1970-01-01 00:00:00.000000 ptal_api-1.0.0a7/PKG-INFO
```

### Comparing `ptal_api-1.0.0a6/README.md` & `ptal_api-1.0.0a7/README.md`

 * *Files identical despite different names*

### Comparing `ptal_api-1.0.0a6/ptal_api/adapter.py` & `ptal_api-1.0.0a7/ptal_api/adapter.py`

 * *Files 0% similar despite different names*

```diff
@@ -2681,15 +2681,15 @@
         )
 
         if self.tdm_builder is not None:
             self.tdm_builder.add_link_fact(relation)
 
         return relation
 
-    def delete_documents(self, document_ids: list[str]) -> bool:
+    def delete_documents(self, document_ids: List[str]) -> bool:
         op = make_operation(Mutation, "delete_documents")
         dd = op.delete_documents(ids=document_ids)
         dd.__fields__("is_success")
         res = self._gql_client.execute(op)
         res = op + res
 
         return res.delete_documents.is_success
```

### Comparing `ptal_api-1.0.0a6/ptal_api/core/type_mapper/common/common.py` & `ptal_api-1.0.0a7/ptal_api/core/type_mapper/common/common.py`

 * *Files identical despite different names*

### Comparing `ptal_api-1.0.0a6/ptal_api/core/type_mapper/data_model/base_data_model.py` & `ptal_api-1.0.0a7/ptal_api/core/type_mapper/data_model/base_data_model.py`

 * *Files identical despite different names*

### Comparing `ptal_api-1.0.0a6/ptal_api/core/type_mapper/data_model/config_data_model.py` & `ptal_api-1.0.0a7/ptal_api/core/type_mapper/data_model/config_data_model.py`

 * *Files identical despite different names*

### Comparing `ptal_api-1.0.0a6/ptal_api/core/type_mapper/data_model/custom_data_model.py` & `ptal_api-1.0.0a7/ptal_api/core/type_mapper/data_model/custom_data_model.py`

 * *Files identical despite different names*

### Comparing `ptal_api-1.0.0a6/ptal_api/core/type_mapper/model_parameters/name_code_mapping.yml` & `ptal_api-1.0.0a7/ptal_api/core/type_mapper/model_parameters/name_code_mapping.yml`

 * *Files identical despite different names*

### Comparing `ptal_api-1.0.0a6/ptal_api/core/type_mapper/modules/custom_data_handler.py` & `ptal_api-1.0.0a7/ptal_api/core/type_mapper/modules/custom_data_handler.py`

 * *Files identical despite different names*

### Comparing `ptal_api-1.0.0a6/ptal_api/core/type_mapper/modules/file_generator.py` & `ptal_api-1.0.0a7/ptal_api/core/type_mapper/modules/file_generator.py`

 * *Files identical despite different names*

### Comparing `ptal_api-1.0.0a6/ptal_api/core/type_mapper/modules/object_name_transformer.py` & `ptal_api-1.0.0a7/ptal_api/core/type_mapper/modules/object_name_transformer.py`

 * *Files identical despite different names*

### Comparing `ptal_api-1.0.0a6/ptal_api/core/type_mapper/modules/type_mapping_generator.py` & `ptal_api-1.0.0a7/ptal_api/core/type_mapper/modules/type_mapping_generator.py`

 * *Files identical despite different names*

### Comparing `ptal_api-1.0.0a6/ptal_api/core/type_mapper/modules/type_mapping_loader/type_mapping_loader.py` & `ptal_api-1.0.0a7/ptal_api/core/type_mapper/modules/type_mapping_loader/type_mapping_loader.py`

 * *Files identical despite different names*

### Comparing `ptal_api-1.0.0a6/ptal_api/core/values/value_mapping.py` & `ptal_api-1.0.0a7/ptal_api/core/values/value_mapping.py`

 * *Files identical despite different names*

### Comparing `ptal_api-1.0.0a6/ptal_api/pretty_adapter/object_types.py` & `ptal_api-1.0.0a7/ptal_api/pretty_adapter/object_types.py`

 * *Files identical despite different names*

### Comparing `ptal_api-1.0.0a6/ptal_api/pretty_adapter/objects.py` & `ptal_api-1.0.0a7/ptal_api/pretty_adapter/objects.py`

 * *Files identical despite different names*

### Comparing `ptal_api-1.0.0a6/ptal_api/pretty_adapter/pretty_adapter.py` & `ptal_api-1.0.0a7/ptal_api/pretty_adapter/pretty_adapter.py`

 * *Files identical despite different names*

### Comparing `ptal_api-1.0.0a6/ptal_api/pretty_adapter/property_values.py` & `ptal_api-1.0.0a7/ptal_api/pretty_adapter/property_values.py`

 * *Files identical despite different names*

### Comparing `ptal_api-1.0.0a6/ptal_api/pretty_adapter/transformer.py` & `ptal_api-1.0.0a7/ptal_api/pretty_adapter/transformer.py`

 * *Files identical despite different names*

### Comparing `ptal_api-1.0.0a6/ptal_api/providers/gql_providers.py` & `ptal_api-1.0.0a7/ptal_api/providers/gql_providers.py`

 * *Files identical despite different names*

### Comparing `ptal_api-1.0.0a6/ptal_api/schema/README.md` & `ptal_api-1.0.0a7/ptal_api/schema/README.md`

 * *Files identical despite different names*

### Comparing `ptal_api-1.0.0a6/ptal_api/schema/api_schema.py` & `ptal_api-1.0.0a7/ptal_api/schema/api_schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,20 +98,20 @@
 class ConceptPropertyTypeSorting(sgqlc.types.Enum):
     __schema__ = api_schema
     __choices__ = ('name', 'registrationDate')
 
 
 class ConceptPropertyValueTypeSorting(sgqlc.types.Enum):
     __schema__ = api_schema
-    __choices__ = ('dictionary', 'id', 'name', 'regexp', 'valueType')
+    __choices__ = ('id', 'name')
 
 
 class ConceptSorting(sgqlc.types.Enum):
     __schema__ = api_schema
-    __choices__ = ('accessLevel', 'countConcepts', 'countConceptsAndDocuments', 'countDocumentFacts', 'countDocumentMentions', 'countEvents', 'countObjects', 'countPotentialDocuments', 'countProperties', 'countResearchMaps', 'countTasks', 'creator', 'id', 'lastUpdater', 'name', 'score', 'systemRegistrationDate', 'systemUpdateDate')
+    __choices__ = ('id', 'name', 'score', 'systemRegistrationDate', 'systemUpdateDate')
 
 
 class ConceptTypeLinkMetadata(sgqlc.types.Enum):
     __schema__ = api_schema
     __choices__ = ('creator', 'endDate', 'lastUpdater', 'linkType', 'registrationDate', 'startDate', 'updateDate')
 
 
@@ -163,15 +163,15 @@
 class DocumentGrouping(sgqlc.types.Enum):
     __schema__ = api_schema
     __choices__ = ('none', 'story')
 
 
 class DocumentSorting(sgqlc.types.Enum):
     __schema__ = api_schema
-    __choices__ = ('countChildDocs', 'countConcepts', 'countDisambiguatedEntities', 'countEntities', 'countEvents', 'countLinks', 'countNamedEntities', 'countObjects', 'countPropertyCandidates', 'countResearchMaps', 'countTasks', 'id', 'publicationDate', 'registrationDate', 'relevance', 'score', 'secretLevel', 'text', 'title', 'trustLevel', 'updateDate')
+    __choices__ = ('countLinks', 'countNamedEntities', 'id', 'publicationDate', 'registrationDate', 'relevance', 'score', 'title', 'updateDate')
 
 
 class DocumentSourceType(sgqlc.types.Enum):
     __schema__ = api_schema
     __choices__ = ('external', 'internal')
 
 
@@ -2604,14 +2604,21 @@
     hierarchy_level = sgqlc.types.Field(sgqlc.types.non_null(Int), graphql_name='hierarchyLevel')
     translated_text = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='translatedText')
     id = sgqlc.types.Field(sgqlc.types.non_null(ID), graphql_name='id')
     language = sgqlc.types.Field('Language', graphql_name='language')
     translation_mention = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null('MentionUnion'))), graphql_name='translationMention')
 
 
+class GeoConceptProperty(sgqlc.types.Type):
+    __schema__ = api_schema
+    __field_names__ = ('concept', 'concept_property')
+    concept = sgqlc.types.Field(sgqlc.types.non_null('Concept'), graphql_name='concept')
+    concept_property = sgqlc.types.Field(sgqlc.types.non_null('ConceptProperty'), graphql_name='conceptProperty')
+
+
 class GeoPointValue(sgqlc.types.Type):
     __schema__ = api_schema
     __field_names__ = ('point', 'name')
     point = sgqlc.types.Field(Coordinates, graphql_name='point')
     name = sgqlc.types.Field(String, graphql_name='name')
 
 
@@ -2783,27 +2790,27 @@
     __field_names__ = ('total', 'list_merged_concept')
     total = sgqlc.types.Field(sgqlc.types.non_null(Long), graphql_name='total')
     list_merged_concept = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(MergedConcept))), graphql_name='listMergedConcept')
 
 
 class Metrics(sgqlc.types.Type):
     __schema__ = api_schema
-    __field_names__ = ('count_objects', 'count_events', 'count_named_entities', 'count_disambiguated_entities', 'count_property_candidates', 'count_links', 'count_research_maps', 'count_child_docs', 'count_tasks', 'count_story_docs', 'count_concepts', 'count_entities')
-    count_objects = sgqlc.types.Field(sgqlc.types.non_null(Int), graphql_name='countObjects')
-    count_events = sgqlc.types.Field(sgqlc.types.non_null(Int), graphql_name='countEvents')
-    count_named_entities = sgqlc.types.Field(sgqlc.types.non_null(Int), graphql_name='countNamedEntities')
-    count_disambiguated_entities = sgqlc.types.Field(sgqlc.types.non_null(Int), graphql_name='countDisambiguatedEntities')
-    count_property_candidates = sgqlc.types.Field(sgqlc.types.non_null(Int), graphql_name='countPropertyCandidates')
-    count_links = sgqlc.types.Field(sgqlc.types.non_null(Int), graphql_name='countLinks')
-    count_research_maps = sgqlc.types.Field(sgqlc.types.non_null(Int), graphql_name='countResearchMaps')
-    count_child_docs = sgqlc.types.Field(sgqlc.types.non_null(Int), graphql_name='countChildDocs')
-    count_tasks = sgqlc.types.Field(sgqlc.types.non_null(Int), graphql_name='countTasks')
-    count_story_docs = sgqlc.types.Field(sgqlc.types.non_null(Int), graphql_name='countStoryDocs')
-    count_concepts = sgqlc.types.Field(sgqlc.types.non_null(Int), graphql_name='countConcepts')
-    count_entities = sgqlc.types.Field(sgqlc.types.non_null(Int), graphql_name='countEntities')
+    __field_names__ = ('count_concepts', 'count_objects', 'count_events', 'count_named_entities', 'count_disambiguated_entities', 'count_property_candidates', 'count_links', 'count_research_maps', 'count_child_docs', 'count_tasks', 'count_story_docs', 'count_entities')
+    count_concepts = sgqlc.types.Field(Int, graphql_name='countConcepts')
+    count_objects = sgqlc.types.Field(Int, graphql_name='countObjects')
+    count_events = sgqlc.types.Field(Int, graphql_name='countEvents')
+    count_named_entities = sgqlc.types.Field(Int, graphql_name='countNamedEntities')
+    count_disambiguated_entities = sgqlc.types.Field(Int, graphql_name='countDisambiguatedEntities')
+    count_property_candidates = sgqlc.types.Field(Int, graphql_name='countPropertyCandidates')
+    count_links = sgqlc.types.Field(Int, graphql_name='countLinks')
+    count_research_maps = sgqlc.types.Field(Int, graphql_name='countResearchMaps')
+    count_child_docs = sgqlc.types.Field(Int, graphql_name='countChildDocs')
+    count_tasks = sgqlc.types.Field(Int, graphql_name='countTasks')
+    count_story_docs = sgqlc.types.Field(Int, graphql_name='countStoryDocs')
+    count_entities = sgqlc.types.Field(Int, graphql_name='countEntities')
 
 
 class Mutation(sgqlc.types.Type):
     __schema__ = api_schema
     __field_names__ = ('add_concept', 'add_concept_link', 'reverse_concept_link', 'update_concept_link', 'add_concept_property', 'add_concept_link_property', 'add_concept_fact', 'delete_concept_fact', 'add_concept_link_property_fact', 'delete_concept_link_property_fact', 'add_concept_property_fact', 'delete_concept_property_fact', 'add_concept_link_fact', 'delete_concept_link_fact', 'update_concept', 'update_concept_avatar', 'update_concept_property', 'approve_kb_fact', 'delete_concept_property', 'delete_concept_link', 'delete_concept', 'delete_concept_link_property', 'merge_concepts', 'unmerge_concepts', 'delete_fact', 'normalize_value', 'update_concept_subscriptions', 'add_concept_type', 'add_composite_concept_type', 'add_composite_concept_type_template', 'add_composite_concept_type_widget_type', 'set_concept_type_default_view', 'add_concept_property_type', 'add_concept_link_property_type', 'add_concept_link_type', 'add_concept_property_value_type', 'add_concept_type_view', 'update_concept_type', 'update_composite_concept_type', 'update_composite_concept_type_template_filename', 'update_composite_concept_type_widget_type', 'update_composite_concept_type_widget_types_order', 'update_concept_property_type', 'update_concept_main_property_type_order', 'update_concept_link_property_type', 'update_concept_link_type', 'update_concept_property_value_type', 'update_concept_type_view', 'delete_concept_type_avatar', 'delete_concept_type', 'delete_composite_concept_type', 'delete_composite_concept_type_widget_type', 'delete_concept_property_type', 'delete_concept_link_property_type', 'delete_concept_link_type', 'delete_concept_property_value_type', 'delete_concept_type_view', 'delete_bulk', 'move_bulk', 'update_type_search_element', 'add_composite_property_value_template', 'update_composite_property_value_template', 'delete_composite_property_value_template', 'add_issue', 'delete_issue', 'add_concept_to_issue', 'add_document_to_issue', 'add_issue_to_issue', 'delete_document_from_issue', 'delete_concept_from_issue', 'delete_issue_from_issue', 'update_issue', 'update_issue_massive', 'add_comment_to_issue', 'update_issue_comment', 'delete_issue_comment', 'update_document', 'update_document_avatar', 'remove_candidate_fact_from_document', 'remove_all_candidate_facts_from_document', 'update_document_facts', 'remove_all_kbfacts_from_document', 'delete_documents', 'add_document_double', 'update_document_node', 'update_document_subscriptions', 'mark_document_as_read', 'mark_document_as_unread', 'delete_research_map', 'bulk_delete_research_map', 'add_research_map', 'add_research_map_from_files', 'update_research_map', 'add_content_on_research_map', 'delete_content_from_research_map', 'batch_move_nodes_on_map', 'batch_update_group_on_map', 'add_top_neighbors_on_map', 'add_concept_fact_neighbors_on_map', 'add_not_approved_neighbors_on_map', 'set_research_map_active', 'find_shortest_path_on_map', 'find_shortest_implicit_path_on_map', 'add_group', 'update_group', 'delete_group', 'create_redmine_issue', 'update_redmine_issue', 'unlink_issues', 'add_access_level', 'update_access_level', 'delete_access_level', 'add_template_docx', 'update_markers_bulk', 'update_document_bulk', 'add_platform', 'update_platform', 'delete_platform', 'add_account', 'update_account', 'delete_account', 'add_document_feed', 'update_document_feed', 'add_document_to_document_feed_favorites', 'delete_document_from_document_feed_favorites', 'delete_document_from_document_feed', 'restore_document_to_document_feed', 'delete_document_feed', 'update_concept_registry_view', 'update_document_registry_view', 'update_document_card_view', 'add_chart', 'update_chart', 'delete_chart', 'translate_tql')
     add_concept = sgqlc.types.Field(sgqlc.types.non_null('Concept'), graphql_name='addConcept', args=sgqlc.types.ArgDict((
         ('form', sgqlc.types.Arg(sgqlc.types.non_null(ConceptMutationInput), graphql_name='form', default=None)),
@@ -3417,15 +3424,15 @@
     __field_names__ = ('maximum_points', 'minimum_number')
     maximum_points = sgqlc.types.Field(Long, graphql_name='maximumPoints')
     minimum_number = sgqlc.types.Field(Long, graphql_name='minimumNumber')
 
 
 class ParagraphMetadata(sgqlc.types.Type):
     __schema__ = api_schema
-    __field_names__ = ('page_id', 'line_id', 'original_text', 'hidden', 'content_type', 'bullet', 'header', 'width', 'height', 'language', 'rowspan', 'colspan', 'name', 'size', 'md5', 'text_translations', 'paragraph_type')
+    __field_names__ = ('page_id', 'line_id', 'original_text', 'hidden', 'content_type', 'bullet', 'header', 'width', 'height', 'language', 'rowspan', 'colspan', 'name', 'size', 'md5', 'paragraph_type')
     page_id = sgqlc.types.Field(Int, graphql_name='pageId')
     line_id = sgqlc.types.Field(Int, graphql_name='lineId')
     original_text = sgqlc.types.Field(String, graphql_name='originalText')
     hidden = sgqlc.types.Field(Boolean, graphql_name='hidden')
     content_type = sgqlc.types.Field(String, graphql_name='contentType')
     bullet = sgqlc.types.Field(String, graphql_name='bullet')
     header = sgqlc.types.Field(Boolean, graphql_name='header')
@@ -3433,15 +3440,14 @@
     height = sgqlc.types.Field(Int, graphql_name='height')
     language = sgqlc.types.Field(String, graphql_name='language')
     rowspan = sgqlc.types.Field(Int, graphql_name='rowspan')
     colspan = sgqlc.types.Field(Int, graphql_name='colspan')
     name = sgqlc.types.Field(String, graphql_name='name')
     size = sgqlc.types.Field(Int, graphql_name='size')
     md5 = sgqlc.types.Field(String, graphql_name='md5')
-    text_translations = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null('Translation')), graphql_name='textTranslations')
     paragraph_type = sgqlc.types.Field(sgqlc.types.non_null(NodeType), graphql_name='paragraphType')
 
 
 class Parameter(sgqlc.types.Type):
     __schema__ = api_schema
     __field_names__ = ('key', 'value')
     key = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='key')
@@ -3474,15 +3480,15 @@
     __field_names__ = ('count_account', 'count_doc')
     count_account = sgqlc.types.Field(sgqlc.types.non_null(Int), graphql_name='countAccount')
     count_doc = sgqlc.types.Field(sgqlc.types.non_null(Int), graphql_name='countDoc')
 
 
 class Query(sgqlc.types.Type):
     __schema__ = api_schema
-    __field_names__ = ('document', 'story', 'pagination_story', 'pagination_document_markers', 'concept_type', 'composite_concept_type', 'pagination_composite_concept_type', 'concept_property_type', 'concept_link_type', 'concept_property_value_type', 'list_concept_type', 'list_user_menu_type', 'list_concept_property_type', 'list_concept_property_type_by_id', 'list_concept_link_type', 'list_concept_property_value_type', 'pagination_concept_type', 'pagination_concept_property_type', 'pagination_concept_link_property_type', 'pagination_concept_link_type', 'pagination_concept_property_value_type', 'composite_concept_property_type', 'composite_link_property_type', 'list_composite_concept_property_type', 'list_composite_link_property_type', 'pagination_composite_concept_property_type', 'pagination_composite_link_property_type', 'composite_property_value_template', 'list_composite_property_value_template', 'pagination_composite_property_value_template', 'concept_type_view', 'domain_map', 'concept', 'list_concept_by_id', 'pagination_concept', 'composite_concept', 'pagination_composite_concept', 'list_concept_link_between_fixed_concepts', 'concept_property', 'concept_link', 'pagination_concept_link', 'pagination_kbrelated_document', 'issue', 'pagination_issue', 'pagination_issue_change', 'research_map', 'pagination_research_map', 'active_research_map', 'list_top_neighbors_on_map', 'list_last_research_map', 'document_autocomplete', 'concept_autocomplete', 'get_osm_place_name', 'get_osm_coordinates', 'get_redmine_issue_creation_default_parameters', 'get_redmine_issue_update_default_description', 'search_similar_redmine_issues', 'access_level', 'pagination_access_level', 'story_fs2_query', 'concept_fs2_query', 'markers_bulk', 'platform', 'list_platform_by_id', 'pagination_platform', 'account', 'list_account_by_id', 'pagination_account', 'pagination_country', 'pagination_language', 'document_feed', 'pagination_document_feed', 'concept_registry_view', 'document_registry_view', 'document_card_view', 'chart', 'preview_chart', 'zklast_sync')
+    __field_names__ = ('document', 'story', 'pagination_story', 'pagination_document_markers', 'pagination_kbrelated_document', 'concept_type', 'composite_concept_type', 'pagination_composite_concept_type', 'concept_property_type', 'concept_link_type', 'concept_property_value_type', 'list_concept_type', 'list_user_menu_type', 'list_concept_property_type', 'list_concept_property_type_by_id', 'list_concept_link_type', 'list_concept_property_value_type', 'pagination_concept_type', 'pagination_concept_property_type', 'pagination_concept_link_property_type', 'pagination_concept_link_type', 'pagination_concept_property_value_type', 'composite_concept_property_type', 'composite_link_property_type', 'list_composite_concept_property_type', 'list_composite_link_property_type', 'pagination_composite_concept_property_type', 'pagination_composite_link_property_type', 'composite_property_value_template', 'list_composite_property_value_template', 'pagination_composite_property_value_template', 'concept_type_view', 'domain_map', 'concept', 'list_concept_by_id', 'pagination_concept', 'composite_concept', 'pagination_composite_concept', 'list_concept_link_between_fixed_concepts', 'concept_property', 'concept_link', 'pagination_concept_link', 'issue', 'pagination_issue', 'pagination_issue_change', 'research_map', 'pagination_research_map', 'active_research_map', 'list_top_neighbors_on_map', 'list_last_research_map', 'document_autocomplete', 'concept_autocomplete', 'get_osm_place_name', 'get_osm_coordinates', 'get_redmine_issue_creation_default_parameters', 'get_redmine_issue_update_default_description', 'search_similar_redmine_issues', 'access_level', 'pagination_access_level', 'story_fs2_query', 'concept_fs2_query', 'markers_bulk', 'platform', 'list_platform_by_id', 'pagination_platform', 'account', 'list_account_by_id', 'pagination_account', 'pagination_country', 'pagination_language', 'document_feed', 'pagination_document_feed', 'concept_registry_view', 'document_registry_view', 'document_card_view', 'chart', 'preview_chart', 'zklast_sync')
     document = sgqlc.types.Field('Document', graphql_name='document', args=sgqlc.types.ArgDict((
         ('id', sgqlc.types.Arg(sgqlc.types.non_null(ID), graphql_name='id', default=None)),
 ))
     )
     story = sgqlc.types.Field('Story', graphql_name='story', args=sgqlc.types.ArgDict((
         ('ids', sgqlc.types.Arg(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(ID))), graphql_name='ids', default=None)),
 ))
@@ -3500,14 +3506,23 @@
     )
     pagination_document_markers = sgqlc.types.Field(sgqlc.types.non_null(CommonStringPagination), graphql_name='paginationDocumentMarkers', args=sgqlc.types.ArgDict((
         ('limit', sgqlc.types.Arg(Int, graphql_name='limit', default=20)),
         ('offset', sgqlc.types.Arg(Int, graphql_name='offset', default=0)),
         ('direction', sgqlc.types.Arg(SortDirection, graphql_name='direction', default='descending')),
 ))
     )
+    pagination_kbrelated_document = sgqlc.types.Field(DocumentPagination, graphql_name='paginationKBRelatedDocument', args=sgqlc.types.ArgDict((
+        ('id', sgqlc.types.Arg(sgqlc.types.non_null(ID), graphql_name='id', default=None)),
+        ('limit', sgqlc.types.Arg(Int, graphql_name='limit', default=20)),
+        ('offset', sgqlc.types.Arg(Int, graphql_name='offset', default=0)),
+        ('filter_settings', sgqlc.types.Arg(sgqlc.types.non_null(RelatedDocumentFilterSettings), graphql_name='filterSettings', default=None)),
+        ('direction', sgqlc.types.Arg(SortDirection, graphql_name='direction', default='descending')),
+        ('sort_field', sgqlc.types.Arg(RelatedDocumentSorting, graphql_name='sortField', default='registrationDate')),
+))
+    )
     concept_type = sgqlc.types.Field(sgqlc.types.non_null('ConceptType'), graphql_name='conceptType', args=sgqlc.types.ArgDict((
         ('id', sgqlc.types.Arg(sgqlc.types.non_null(ID), graphql_name='id', default=None)),
 ))
     )
     composite_concept_type = sgqlc.types.Field(sgqlc.types.non_null('CompositeConceptType'), graphql_name='compositeConceptType', args=sgqlc.types.ArgDict((
         ('id', sgqlc.types.Arg(sgqlc.types.non_null(ID), graphql_name='id', default=None)),
 ))
@@ -3669,23 +3684,14 @@
     )
     pagination_concept_link = sgqlc.types.Field(sgqlc.types.non_null(ConceptLinkPagination), graphql_name='paginationConceptLink', args=sgqlc.types.ArgDict((
         ('limit', sgqlc.types.Arg(Int, graphql_name='limit', default=20)),
         ('offset', sgqlc.types.Arg(Int, graphql_name='offset', default=0)),
         ('filter_settings', sgqlc.types.Arg(sgqlc.types.non_null(ConceptLinkFilterSettings), graphql_name='filterSettings', default=None)),
 ))
     )
-    pagination_kbrelated_document = sgqlc.types.Field(DocumentPagination, graphql_name='paginationKBRelatedDocument', args=sgqlc.types.ArgDict((
-        ('id', sgqlc.types.Arg(sgqlc.types.non_null(ID), graphql_name='id', default=None)),
-        ('limit', sgqlc.types.Arg(Int, graphql_name='limit', default=20)),
-        ('offset', sgqlc.types.Arg(Int, graphql_name='offset', default=0)),
-        ('filter_settings', sgqlc.types.Arg(sgqlc.types.non_null(RelatedDocumentFilterSettings), graphql_name='filterSettings', default=None)),
-        ('direction', sgqlc.types.Arg(SortDirection, graphql_name='direction', default='descending')),
-        ('sort_field', sgqlc.types.Arg(RelatedDocumentSorting, graphql_name='sortField', default='registrationDate')),
-))
-    )
     issue = sgqlc.types.Field('Issue', graphql_name='issue', args=sgqlc.types.ArgDict((
         ('id', sgqlc.types.Arg(sgqlc.types.non_null(ID), graphql_name='id', default=None)),
 ))
     )
     pagination_issue = sgqlc.types.Field(IssuePagination, graphql_name='paginationIssue', args=sgqlc.types.ArgDict((
         ('limit', sgqlc.types.Arg(Int, graphql_name='limit', default=20)),
         ('offset', sgqlc.types.Arg(Int, graphql_name='offset', default=0)),
@@ -4548,15 +4554,15 @@
         ('filter_settings', sgqlc.types.Arg(ConceptFilterSettings, graphql_name='filterSettings', default=None)),
 ))
     )
 
 
 class Document(sgqlc.types.Type, RecordInterface):
     __schema__ = api_schema
-    __field_names__ = ('id', 'title', 'external_url', 'publication_date', 'publication_author', 'notes', 'document_type', 'highlightings', 'markers', 'tables', 'metadata', 'uuid', 'trust_level', 'story', 'score', 'has_text', 'parent', 'list_child', 'pagination_child', 'internal_url', 'avatar', 'metric', 'pagination_concept_fact', 'list_concept_fact', 'pagination_concept_link_fact', 'list_concept_link_document_fact', 'preview', 'list_fact_with_mention', 'pagination_redmine_issues', 'pagination_issue', 'access_level', 'text', 'additional_text', 'list_subscription', 'pagination_similar_documents', 'is_read', 'list_mention_link', 'node', 'metadata_concept', 'list_fact', 'extra_metadata', 'list_mention', 'fact')
+    __field_names__ = ('id', 'title', 'external_url', 'publication_date', 'publication_author', 'notes', 'document_type', 'highlightings', 'markers', 'tables', 'metadata', 'uuid', 'trust_level', 'story', 'score', 'has_text', 'parent', 'list_child', 'pagination_child', 'internal_url', 'avatar', 'metric', 'pagination_concept_fact', 'list_concept_fact', 'pagination_concept_link_fact', 'list_concept_link_document_fact', 'preview', 'list_fact_with_mention', 'pagination_redmine_issues', 'pagination_issue', 'access_level', 'text', 'additional_text', 'list_subscription', 'pagination_similar_documents', 'is_read', 'list_mention_link', 'node', 'metadata_concept', 'text_translations', 'list_fact', 'extra_metadata', 'list_mention', 'fact')
     id = sgqlc.types.Field(sgqlc.types.non_null(ID), graphql_name='id')
     title = sgqlc.types.Field(String, graphql_name='title')
     external_url = sgqlc.types.Field(String, graphql_name='externalUrl')
     publication_date = sgqlc.types.Field(UnixTime, graphql_name='publicationDate')
     publication_author = sgqlc.types.Field(String, graphql_name='publicationAuthor')
     notes = sgqlc.types.Field(String, graphql_name='notes')
     document_type = sgqlc.types.Field(sgqlc.types.non_null(DocumentType), graphql_name='documentType')
@@ -4632,14 +4638,18 @@
 ))
     )
     node = sgqlc.types.Field(FlatDocumentStructure, graphql_name='node', args=sgqlc.types.ArgDict((
         ('id', sgqlc.types.Arg(sgqlc.types.non_null(ID), graphql_name='id', default=None)),
 ))
     )
     metadata_concept = sgqlc.types.Field(Concept, graphql_name='metadataConcept')
+    text_translations = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(Translation))), graphql_name='textTranslations', args=sgqlc.types.ArgDict((
+        ('node_id', sgqlc.types.Arg(sgqlc.types.non_null(ID), graphql_name='nodeId', default=None)),
+))
+    )
     list_fact = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null('Fact'))), graphql_name='listFact')
     extra_metadata = sgqlc.types.Field(JSON, graphql_name='extraMetadata')
     list_mention = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null('MentionUnion'))), graphql_name='listMention')
     fact = sgqlc.types.Field('Fact', graphql_name='fact', args=sgqlc.types.ArgDict((
         ('id', sgqlc.types.Arg(sgqlc.types.non_null(ID), graphql_name='id', default=None)),
 ))
     )
@@ -4754,15 +4764,15 @@
     __field_names__ = ('value_fact', 'mention')
     value_fact = sgqlc.types.Field(sgqlc.types.non_null(ConceptPropertyValueCandidateFact), graphql_name='valueFact')
     mention = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null('MentionUnion'))), graphql_name='mention')
 
 
 class ResearchMap(sgqlc.types.Type, RecordInterface):
     __schema__ = api_schema
-    __field_names__ = ('id', 'name', 'description', 'is_temporary', 'markers', 'list_node', 'list_edge', 'research_map_statistics', 'list_group', 'is_active', 'access_level', 'pagination_concept', 'pagination_story', 'pagination_research_map')
+    __field_names__ = ('id', 'name', 'description', 'is_temporary', 'markers', 'list_node', 'list_edge', 'research_map_statistics', 'list_group', 'is_active', 'access_level', 'pagination_concept', 'pagination_story', 'pagination_research_map', 'list_geo_concept_properties')
     id = sgqlc.types.Field(sgqlc.types.non_null(ID), graphql_name='id')
     name = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='name')
     description = sgqlc.types.Field(String, graphql_name='description')
     is_temporary = sgqlc.types.Field(sgqlc.types.non_null(Boolean), graphql_name='isTemporary')
     markers = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(String))), graphql_name='markers')
     list_node = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(MapNode))), graphql_name='listNode', args=sgqlc.types.ArgDict((
         ('filter_settings', sgqlc.types.Arg(MapNodeFilterSettings, graphql_name='filterSettings', default=None)),
@@ -4803,14 +4813,15 @@
         ('offset', sgqlc.types.Arg(Int, graphql_name='offset', default=0)),
         ('filter_settings', sgqlc.types.Arg(sgqlc.types.non_null(ResearchMapFilterSettings), graphql_name='filterSettings', default=None)),
         ('direction', sgqlc.types.Arg(SortDirection, graphql_name='direction', default='descending')),
         ('sort_field', sgqlc.types.Arg(ResearchMapSorting, graphql_name='sortField', default='conceptAndDocumentLink')),
         ('research_map_content_select_input', sgqlc.types.Arg(ResearchMapContentUpdateInput, graphql_name='ResearchMapContentSelectInput', default=None)),
 ))
     )
+    list_geo_concept_properties = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(GeoConceptProperty))), graphql_name='listGeoConceptProperties')
 
 
 class TextNodeMention(sgqlc.types.Type, MentionInterface, RecordInterface):
     __schema__ = api_schema
     __field_names__ = ('node_id', 'start', 'end')
     node_id = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='nodeId')
     start = sgqlc.types.Field(sgqlc.types.non_null(Int), graphql_name='start')
@@ -4854,15 +4865,15 @@
 class ConceptPropertyLikeFact(sgqlc.types.Union):
     __schema__ = api_schema
     __types__ = (ConceptPropertyFact, ConceptLinkPropertyFact)
 
 
 class ConceptViewValue(sgqlc.types.Union):
     __schema__ = api_schema
-    __types__ = (DateTimeValue, GeoPointValue, IntValue, DoubleValue, StringLocaleValue, StringValue, LinkValue, CompositeValue, Concept, ConceptType, ConceptLinkType, User, Image)
+    __types__ = (DateTimeValue, GeoPointValue, IntValue, DoubleValue, StringLocaleValue, StringValue, LinkValue, CompositeValue, Concept, ConceptType, ConceptLinkType, User, Image, TimestampValue)
 
 
 class Entity(sgqlc.types.Union):
     __schema__ = api_schema
     __types__ = (Concept, Document, ConceptCandidateFact, ConceptType)
```

### Comparing `ptal_api-1.0.0a6/ptal_api/schema/crawlers_api_schema.py` & `ptal_api-1.0.0a7/ptal_api/schema/crawlers_api_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -130,19 +130,14 @@
 
 
 class PeriodicJobSorting(sgqlc.types.Enum):
     __schema__ = crawlers_api_schema
     __choices__ = ('crawlerId', 'crawlerName', 'creator', 'credentialId', 'id', 'lastUpdater', 'name', 'nextScheduleTime', 'priority', 'projectId', 'projectName', 'status', 'systemRegistrationDate', 'systemUpdateDate')
 
 
-class PeriodicJobStatus(sgqlc.types.Enum):
-    __schema__ = crawlers_api_schema
-    __choices__ = ('Disabled', 'Enabled')
-
-
 class ProjectSorting(sgqlc.types.Enum):
     __schema__ = crawlers_api_schema
     __choices__ = ('creator', 'description', 'id', 'lastUpdater', 'name', 'systemRegistrationDate', 'systemUpdateDate', 'title')
 
 
 class RecoveryJobSorting(sgqlc.types.Enum):
     __schema__ = crawlers_api_schema
@@ -155,14 +150,19 @@
 
 
 class RequestSorting(sgqlc.types.Enum):
     __schema__ = crawlers_api_schema
     __choices__ = ('timestamp',)
 
 
+class RunningStatus(sgqlc.types.Enum):
+    __schema__ = crawlers_api_schema
+    __choices__ = ('Disabled', 'Enabled')
+
+
 class SettingsType(sgqlc.types.Enum):
     __schema__ = crawlers_api_schema
     __choices__ = ('array', 'boolean', 'float', 'int', 'object', 'string')
 
 
 class SortDirection(sgqlc.types.Enum):
     __schema__ = crawlers_api_schema
@@ -309,19 +309,20 @@
     updaters = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null(String)), graphql_name='updaters')
     system_registration_date = sgqlc.types.Field('TimestampInterval', graphql_name='systemRegistrationDate')
     system_update_date = sgqlc.types.Field('TimestampInterval', graphql_name='systemUpdateDate')
 
 
 class InformationSourceLoaderInput(sgqlc.types.Input):
     __schema__ = crawlers_api_schema
-    __field_names__ = ('file_settings', 'urls', 'is_retrospective', 'retrospective_interval', 'actual_status')
+    __field_names__ = ('file_settings', 'urls', 'is_retrospective', 'retrospective_interval', 'running_status', 'actual_status')
     file_settings = sgqlc.types.Field('S3FileSettings', graphql_name='fileSettings')
     urls = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null('KeyOptionValueInput')), graphql_name='urls')
     is_retrospective = sgqlc.types.Field(Boolean, graphql_name='isRetrospective')
     retrospective_interval = sgqlc.types.Field('TimestampInterval', graphql_name='retrospectiveInterval')
+    running_status = sgqlc.types.Field(RunningStatus, graphql_name='runningStatus')
     actual_status = sgqlc.types.Field(InformationSourceLoaderActualStatus, graphql_name='actualStatus')
 
 
 class JobInput(sgqlc.types.Input):
     __schema__ = crawlers_api_schema
     __field_names__ = ('crawler_id', 'version_id', 'credential_id', 'priority', 'message_priority', 'is_noise', 'research_map_id', 'settings', 'args')
     crawler_id = sgqlc.types.Field(sgqlc.types.non_null(ID), graphql_name='crawlerId')
@@ -385,15 +386,15 @@
 class PeriodicJobFilterSettings(sgqlc.types.Input):
     __schema__ = crawlers_api_schema
     __field_names__ = ('input_value', 'projects', 'crawlers', 'priorities', 'running_statuses', 'creators', 'updaters', 'system_registration_date', 'system_update_date', 'next_schedule_time')
     input_value = sgqlc.types.Field(String, graphql_name='inputValue')
     projects = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null(ID)), graphql_name='projects')
     crawlers = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null(ID)), graphql_name='crawlers')
     priorities = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null(JobPriorityType)), graphql_name='priorities')
-    running_statuses = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null(PeriodicJobStatus)), graphql_name='runningStatuses')
+    running_statuses = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null(RunningStatus)), graphql_name='runningStatuses')
     creators = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null(String)), graphql_name='creators')
     updaters = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null(String)), graphql_name='updaters')
     system_registration_date = sgqlc.types.Field('TimestampInterval', graphql_name='systemRegistrationDate')
     system_update_date = sgqlc.types.Field('TimestampInterval', graphql_name='systemUpdateDate')
     next_schedule_time = sgqlc.types.Field('TimestampInterval', graphql_name='nextScheduleTime')
 
 
@@ -401,15 +402,15 @@
     __schema__ = crawlers_api_schema
     __field_names__ = ('title', 'description', 'crawler_id', 'version_id', 'credential_id', 'status', 'priority', 'message_priority', 'cron_expression', 'cron_utcoffset_minutes', 'disable_time', 'settings', 'args', 'update_on_reload')
     title = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='title')
     description = sgqlc.types.Field(String, graphql_name='description')
     crawler_id = sgqlc.types.Field(sgqlc.types.non_null(ID), graphql_name='crawlerId')
     version_id = sgqlc.types.Field(sgqlc.types.non_null(ID), graphql_name='versionId')
     credential_id = sgqlc.types.Field(ID, graphql_name='credentialId')
-    status = sgqlc.types.Field(PeriodicJobStatus, graphql_name='status')
+    status = sgqlc.types.Field(RunningStatus, graphql_name='status')
     priority = sgqlc.types.Field(JobPriorityType, graphql_name='priority')
     message_priority = sgqlc.types.Field(MessagePriority, graphql_name='messagePriority')
     cron_expression = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='cronExpression')
     cron_utcoffset_minutes = sgqlc.types.Field(Int, graphql_name='cronUTCOffsetMinutes')
     disable_time = sgqlc.types.Field(UnixTime, graphql_name='disableTime')
     settings = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(KeyValueInputType))), graphql_name='settings')
     args = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(KeyValueInputType))), graphql_name='args')
@@ -699,15 +700,15 @@
     __field_names__ = ('total', 'list_metric')
     total = sgqlc.types.Field(sgqlc.types.non_null(Long), graphql_name='total')
     list_metric = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(Metric))), graphql_name='listMetric')
 
 
 class Mutation(sgqlc.types.Type):
     __schema__ = crawlers_api_schema
-    __field_names__ = ('update_crawler', 'update_crawler_settings_arguments', 'delete_crawler_versions', 'delete_crawlers', 'update_site_map_crawler_body', 'add_crawl_state', 'update_crawl_state', 'delete_crawl_state', 'add_credential', 'update_credential', 'delete_credential', 'add_job', 'delete_job', 'cancel_job', 'suspend_job', 'resume_job', 'download_pending_jobs', 'schedule_uploaded_jobs', 'restart_job', 'add_periodic_job', 'run_periodic_jobs', 'update_enable_jobs_scheduling', 'update_disable_jobs_scheduling', 'delete_periodic_job', 'update_periodic_job', 'update_periodic_job_settings_and_arguments', 'import_periodic_jobs', 'delete_project', 'delete_project_versions', 'add_project', 'update_project', 'update_project_settings_and_arguments', 'add_information_source_loader', 'delete_information_source_loader', 'add_recovery_job', 'cancel_recovery_job')
+    __field_names__ = ('update_crawler', 'update_crawler_settings_arguments', 'delete_crawler_versions', 'delete_crawlers', 'update_site_map_crawler_body', 'add_crawl_state', 'update_crawl_state', 'delete_crawl_state', 'add_credential', 'update_credential', 'delete_credential', 'add_job', 'delete_job', 'cancel_job', 'suspend_job', 'resume_job', 'download_pending_jobs', 'schedule_uploaded_jobs', 'restart_job', 'add_periodic_job', 'run_periodic_jobs', 'update_enable_jobs_scheduling', 'update_disable_jobs_scheduling', 'delete_periodic_job', 'update_periodic_job', 'update_periodic_job_settings_and_arguments', 'import_periodic_jobs', 'delete_project', 'delete_project_versions', 'add_project', 'update_project', 'update_project_settings_and_arguments', 'add_information_source_loader', 'delete_information_source_loader', 'update_enable_information_source_loader', 'update_disable_information_source_loader', 'add_recovery_job', 'cancel_recovery_job')
     update_crawler = sgqlc.types.Field(sgqlc.types.non_null('Crawler'), graphql_name='updateCrawler', args=sgqlc.types.ArgDict((
         ('crawler_update_input', sgqlc.types.Arg(sgqlc.types.non_null(CrawlerUpdateInput), graphql_name='crawlerUpdateInput', default=None)),
         ('crawler_id', sgqlc.types.Arg(sgqlc.types.non_null(ID), graphql_name='crawlerId', default=None)),
         ('project_id', sgqlc.types.Arg(sgqlc.types.non_null(ID), graphql_name='projectId', default=None)),
 ))
     )
     update_crawler_settings_arguments = sgqlc.types.Field(sgqlc.types.non_null('Crawler'), graphql_name='updateCrawlerSettingsArguments', args=sgqlc.types.ArgDict((
@@ -850,14 +851,22 @@
         ('information_source_loader_input', sgqlc.types.Arg(sgqlc.types.non_null(InformationSourceLoaderInput), graphql_name='informationSourceLoaderInput', default=None)),
 ))
     )
     delete_information_source_loader = sgqlc.types.Field(sgqlc.types.non_null('State'), graphql_name='deleteInformationSourceLoader', args=sgqlc.types.ArgDict((
         ('ids', sgqlc.types.Arg(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(ID))), graphql_name='ids', default=None)),
 ))
     )
+    update_enable_information_source_loader = sgqlc.types.Field(sgqlc.types.non_null('State'), graphql_name='updateEnableInformationSourceLoader', args=sgqlc.types.ArgDict((
+        ('ids', sgqlc.types.Arg(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(ID))), graphql_name='ids', default=None)),
+))
+    )
+    update_disable_information_source_loader = sgqlc.types.Field(sgqlc.types.non_null('State'), graphql_name='updateDisableInformationSourceLoader', args=sgqlc.types.ArgDict((
+        ('ids', sgqlc.types.Arg(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(ID))), graphql_name='ids', default=None)),
+))
+    )
     add_recovery_job = sgqlc.types.Field(sgqlc.types.non_null('RecoveryJob'), graphql_name='addRecoveryJob', args=sgqlc.types.ArgDict((
         ('add_recovery_job_input', sgqlc.types.Arg(sgqlc.types.non_null(AddRecoveryJobInput), graphql_name='addRecoveryJobInput', default=None)),
 ))
     )
     cancel_recovery_job = sgqlc.types.Field(sgqlc.types.non_null('RecoveryJob'), graphql_name='cancelRecoveryJob', args=sgqlc.types.ArgDict((
         ('id', sgqlc.types.Arg(sgqlc.types.non_null(ID), graphql_name='id', default=None)),
 ))
@@ -1326,19 +1335,20 @@
     domain = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='domain')
     status = sgqlc.types.Field(sgqlc.types.non_null(CredentialStatus), graphql_name='status')
     projects = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null('Project'))), graphql_name='projects')
 
 
 class InformationSourceLoader(sgqlc.types.Type, RecordInterface):
     __schema__ = crawlers_api_schema
-    __field_names__ = ('id', 'is_retrospective', 'retrospective_start', 'retrospective_end', 'actual_status', 'status', 'metrics', 'title')
+    __field_names__ = ('id', 'is_retrospective', 'retrospective_start', 'retrospective_end', 'running_status', 'actual_status', 'status', 'metrics', 'title')
     id = sgqlc.types.Field(sgqlc.types.non_null(ID), graphql_name='id')
     is_retrospective = sgqlc.types.Field(sgqlc.types.non_null(Boolean), graphql_name='isRetrospective')
     retrospective_start = sgqlc.types.Field(UnixTime, graphql_name='retrospectiveStart')
     retrospective_end = sgqlc.types.Field(UnixTime, graphql_name='retrospectiveEnd')
+    running_status = sgqlc.types.Field(sgqlc.types.non_null(RunningStatus), graphql_name='runningStatus')
     actual_status = sgqlc.types.Field(sgqlc.types.non_null(InformationSourceLoaderActualStatus), graphql_name='actualStatus')
     status = sgqlc.types.Field(sgqlc.types.non_null(CollectionStatus), graphql_name='status')
     metrics = sgqlc.types.Field(sgqlc.types.non_null(InformationSourceLoaderStats), graphql_name='metrics')
     title = sgqlc.types.Field(sgqlc.types.non_null('InformationSourceLoaderTitle'), graphql_name='title')
 
 
 class Job(sgqlc.types.Type, RecordInterface):
@@ -1356,15 +1366,15 @@
     crawler = sgqlc.types.Field(sgqlc.types.non_null(Crawler), graphql_name='crawler')
     project = sgqlc.types.Field(sgqlc.types.non_null('Project'), graphql_name='project')
     version = sgqlc.types.Field(sgqlc.types.non_null('Version'), graphql_name='version')
     credential = sgqlc.types.Field(Credential, graphql_name='credential')
     periodic_job = sgqlc.types.Field('PeriodicJob', graphql_name='periodicJob')
     settings = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(KeyValue))), graphql_name='settings')
     args = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(KeyValue))), graphql_name='args')
-    metrics = sgqlc.types.Field(sgqlc.types.non_null(JobMetrics), graphql_name='metrics')
+    metrics = sgqlc.types.Field(JobMetrics, graphql_name='metrics')
     job_stats = sgqlc.types.Field(JobStats, graphql_name='jobStats')
     platforms = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(Platform))), graphql_name='platforms')
     histogram_requests = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(DateHistogramBucket))), graphql_name='histogramRequests')
     histogram_items = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(DateHistogramBucket))), graphql_name='histogramItems')
     schema = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(KeyValue))), graphql_name='schema')
 
 
@@ -1372,28 +1382,28 @@
     __schema__ = crawlers_api_schema
     __field_names__ = ('id', 'name', 'description', 'priority', 'message_priority', 'status', 'monitoring_status', 'cron', 'cron_utcoffset_minutes', 'next_schedule_time', 'disable_time', 'update_on_reload', 'crawler', 'project', 'version', 'credential', 'settings', 'args', 'metrics', 'histogram_requests', 'histogram_items', 'job_stats', 'platforms', 'job_failed_monitoring_statuses')
     id = sgqlc.types.Field(sgqlc.types.non_null(ID), graphql_name='id')
     name = sgqlc.types.Field(String, graphql_name='name')
     description = sgqlc.types.Field(String, graphql_name='description')
     priority = sgqlc.types.Field(sgqlc.types.non_null(JobPriorityType), graphql_name='priority')
     message_priority = sgqlc.types.Field(sgqlc.types.non_null(MessagePriority), graphql_name='messagePriority')
-    status = sgqlc.types.Field(sgqlc.types.non_null(PeriodicJobStatus), graphql_name='status')
+    status = sgqlc.types.Field(sgqlc.types.non_null(RunningStatus), graphql_name='status')
     monitoring_status = sgqlc.types.Field(sgqlc.types.non_null(MonitoringStatus), graphql_name='monitoringStatus')
     cron = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='cron')
     cron_utcoffset_minutes = sgqlc.types.Field(sgqlc.types.non_null(Int), graphql_name='cronUTCOffsetMinutes')
     next_schedule_time = sgqlc.types.Field(UnixTime, graphql_name='nextScheduleTime')
     disable_time = sgqlc.types.Field(UnixTime, graphql_name='disableTime')
     update_on_reload = sgqlc.types.Field(sgqlc.types.non_null(Boolean), graphql_name='updateOnReload')
     crawler = sgqlc.types.Field(sgqlc.types.non_null(Crawler), graphql_name='crawler')
     project = sgqlc.types.Field(sgqlc.types.non_null('Project'), graphql_name='project')
     version = sgqlc.types.Field(sgqlc.types.non_null('Version'), graphql_name='version')
     credential = sgqlc.types.Field(Credential, graphql_name='credential')
     settings = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(KeyValue))), graphql_name='settings')
     args = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(KeyValue))), graphql_name='args')
-    metrics = sgqlc.types.Field(sgqlc.types.non_null(PeriodicJobMetrics), graphql_name='metrics')
+    metrics = sgqlc.types.Field(PeriodicJobMetrics, graphql_name='metrics')
     histogram_requests = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(DateHistogramBucket))), graphql_name='histogramRequests', args=sgqlc.types.ArgDict((
         ('interval', sgqlc.types.Arg(TimestampInterval, graphql_name='interval', default=None)),
 ))
     )
     histogram_items = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(DateHistogramBucket))), graphql_name='histogramItems', args=sgqlc.types.ArgDict((
         ('interval', sgqlc.types.Arg(TimestampInterval, graphql_name='interval', default=None)),
 ))
```

### Comparing `ptal_api-1.0.0a6/ptal_api/schema/tcontroller_api_schema.py` & `ptal_api-1.0.0a7/ptal_api/schema/tcontroller_api_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -106,18 +106,14 @@
 
 String = sgqlc.types.String
 
 class UnixTime(sgqlc.types.Scalar):
     __schema__ = tcontroller_api_schema
 
 
-class Upload(sgqlc.types.Scalar):
-    __schema__ = tcontroller_api_schema
-
-
 class UserPipelineTransformSort(sgqlc.types.Enum):
     __schema__ = tcontroller_api_schema
     __choices__ = ('description', 'id', 'state', 'systemRegistrationDate', 'systemUpdateDate')
 
 
 class UserServiceState(sgqlc.types.Enum):
     __schema__ = tcontroller_api_schema
@@ -306,14 +302,21 @@
 class PipelineTransformSetupInput(sgqlc.types.Input):
     __schema__ = tcontroller_api_schema
     __field_names__ = ('id', 'params')
     id = sgqlc.types.Field(sgqlc.types.non_null(ID), graphql_name='id')
     params = sgqlc.types.Field(sgqlc.types.non_null(JSON), graphql_name='params')
 
 
+class S3FileInput(sgqlc.types.Input):
+    __schema__ = tcontroller_api_schema
+    __field_names__ = ('bucket_name', 'object_name')
+    bucket_name = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='bucketName')
+    object_name = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='objectName')
+
+
 class TimestampInterval(sgqlc.types.Input):
     __schema__ = tcontroller_api_schema
     __field_names__ = ('start', 'end')
     start = sgqlc.types.Field(UnixTime, graphql_name='start')
     end = sgqlc.types.Field(UnixTime, graphql_name='end')
 
 
@@ -643,15 +646,15 @@
     )
     copy_pipeline_config = sgqlc.types.Field(sgqlc.types.non_null('PipelineConfig'), graphql_name='copyPipelineConfig', args=sgqlc.types.ArgDict((
         ('source_id', sgqlc.types.Arg(sgqlc.types.non_null(ID), graphql_name='sourceId', default=None)),
         ('description', sgqlc.types.Arg(String, graphql_name='description', default=None)),
 ))
     )
     import_pipeline_config = sgqlc.types.Field(sgqlc.types.non_null('PipelineConfig'), graphql_name='importPipelineConfig', args=sgqlc.types.ArgDict((
-        ('export', sgqlc.types.Arg(sgqlc.types.non_null(Upload), graphql_name='export', default=None)),
+        ('export', sgqlc.types.Arg(sgqlc.types.non_null(S3FileInput), graphql_name='export', default=None)),
 ))
     )
     update_pipeline_config = sgqlc.types.Field(sgqlc.types.non_null('PipelineConfig'), graphql_name='updatePipelineConfig', args=sgqlc.types.ArgDict((
         ('pipeline_config', sgqlc.types.Arg(sgqlc.types.non_null(PipelineConfigInput), graphql_name='pipelineConfig', default=None)),
 ))
     )
     delete_pipeline_config = sgqlc.types.Field(sgqlc.types.non_null('PipelineConfig'), graphql_name='deletePipelineConfig', args=sgqlc.types.ArgDict((
@@ -671,14 +674,15 @@
     update_kafka_topics = sgqlc.types.Field(sgqlc.types.non_null(Int), graphql_name='updateKafkaTopics', args=sgqlc.types.ArgDict((
         ('topics', sgqlc.types.Arg(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(ID))), graphql_name='topics', default=None)),
         ('update', sgqlc.types.Arg(sgqlc.types.non_null(KafkaTopicUpdate), graphql_name='update', default=None)),
 ))
     )
     delete_kafka_topic = sgqlc.types.Field(sgqlc.types.non_null('KafkaTopic'), graphql_name='deleteKafkaTopic', args=sgqlc.types.ArgDict((
         ('topic', sgqlc.types.Arg(sgqlc.types.non_null(ID), graphql_name='topic', default=None)),
+        ('continue_after_timeout', sgqlc.types.Arg(Boolean, graphql_name='continueAfterTimeout', default=False)),
 ))
     )
     retry_failed_in_topic = sgqlc.types.Field(sgqlc.types.non_null(Int), graphql_name='retryFailedInTopic', args=sgqlc.types.ArgDict((
         ('topic', sgqlc.types.Arg(sgqlc.types.non_null(ID), graphql_name='topic', default=None)),
 ))
     )
     retry_failed_message = sgqlc.types.Field(sgqlc.types.non_null(Int), graphql_name='retryFailedMessage', args=sgqlc.types.ArgDict((
@@ -701,22 +705,22 @@
         ('topic', sgqlc.types.Arg(ID, graphql_name='topic', default=None)),
         ('use_kb', sgqlc.types.Arg(Boolean, graphql_name='useKb', default=False)),
         ('priority', sgqlc.types.Arg(MessagePriority, graphql_name='priority', default='Normal')),
 ))
     )
     add_exporter = sgqlc.types.Field(sgqlc.types.non_null('Exporter'), graphql_name='addExporter', args=sgqlc.types.ArgDict((
         ('data', sgqlc.types.Arg(ExporterInput, graphql_name='data', default=None)),
-        ('service_image', sgqlc.types.Arg(sgqlc.types.non_null(Upload), graphql_name='serviceImage', default=None)),
+        ('service_image', sgqlc.types.Arg(sgqlc.types.non_null(S3FileInput), graphql_name='serviceImage', default=None)),
         ('service', sgqlc.types.Arg(UserServiceInput, graphql_name='service', default=None)),
 ))
     )
     update_exporter = sgqlc.types.Field(sgqlc.types.non_null('Exporter'), graphql_name='updateExporter', args=sgqlc.types.ArgDict((
         ('id', sgqlc.types.Arg(sgqlc.types.non_null(ID), graphql_name='id', default=None)),
         ('data', sgqlc.types.Arg(ExporterInput, graphql_name='data', default=None)),
-        ('service_image', sgqlc.types.Arg(Upload, graphql_name='serviceImage', default=None)),
+        ('service_image', sgqlc.types.Arg(S3FileInput, graphql_name='serviceImage', default=None)),
         ('service', sgqlc.types.Arg(UserServiceInput, graphql_name='service', default=None)),
 ))
     )
     delete_exporter = sgqlc.types.Field(sgqlc.types.non_null('Exporter'), graphql_name='deleteExporter', args=sgqlc.types.ArgDict((
         ('id', sgqlc.types.Arg(sgqlc.types.non_null(ID), graphql_name='id', default=None)),
 ))
     )
@@ -758,22 +762,22 @@
     )
     cancel_concept_transform_task = sgqlc.types.Field(sgqlc.types.non_null('ConceptTransformTask'), graphql_name='cancelConceptTransformTask', args=sgqlc.types.ArgDict((
         ('id', sgqlc.types.Arg(sgqlc.types.non_null(ID), graphql_name='id', default=None)),
 ))
     )
     add_user_pipeline_transform = sgqlc.types.Field(sgqlc.types.non_null('UserPipelineTransform'), graphql_name='addUserPipelineTransform', args=sgqlc.types.ArgDict((
         ('description', sgqlc.types.Arg(String, graphql_name='description', default=None)),
-        ('service_image', sgqlc.types.Arg(Upload, graphql_name='serviceImage', default=None)),
+        ('service_image', sgqlc.types.Arg(S3FileInput, graphql_name='serviceImage', default=None)),
         ('service', sgqlc.types.Arg(UserServiceInput, graphql_name='service', default=None)),
 ))
     )
     update_user_pipeline_transform = sgqlc.types.Field(sgqlc.types.non_null('UserPipelineTransform'), graphql_name='updateUserPipelineTransform', args=sgqlc.types.ArgDict((
         ('id', sgqlc.types.Arg(sgqlc.types.non_null(ID), graphql_name='id', default=None)),
         ('description', sgqlc.types.Arg(String, graphql_name='description', default=None)),
-        ('service_image', sgqlc.types.Arg(Upload, graphql_name='serviceImage', default=None)),
+        ('service_image', sgqlc.types.Arg(S3FileInput, graphql_name='serviceImage', default=None)),
         ('service', sgqlc.types.Arg(UserServiceInput, graphql_name='service', default=None)),
 ))
     )
     delete_user_pipeline_transform = sgqlc.types.Field(sgqlc.types.non_null('UserPipelineTransform'), graphql_name='deleteUserPipelineTransform', args=sgqlc.types.ArgDict((
         ('id', sgqlc.types.Arg(sgqlc.types.non_null(ID), graphql_name='id', default=None)),
 ))
     )
```

### Comparing `ptal_api-1.0.0a6/ptal_api/schema/translator_api_schema.py` & `ptal_api-1.0.0a7/ptal_api/schema/translator_api_schema.py`

 * *Files identical despite different names*

### Comparing `ptal_api-1.0.0a6/ptal_api/schema/utils_api_schema.py` & `ptal_api-1.0.0a7/ptal_api/schema/utils_api_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 class ConceptPropertyTypeSorting(sgqlc.types.Enum):
     __schema__ = utils_api_schema
     __choices__ = ('name', 'registrationDate')
 
 
 class ConceptSorting(sgqlc.types.Enum):
     __schema__ = utils_api_schema
-    __choices__ = ('accessLevel', 'countConcepts', 'countConceptsAndDocuments', 'countDocumentFacts', 'countDocumentMentions', 'countEvents', 'countObjects', 'countPotentialDocuments', 'countProperties', 'countResearchMaps', 'countTasks', 'creator', 'id', 'lastUpdater', 'name', 'score', 'systemRegistrationDate', 'systemUpdateDate')
+    __choices__ = ('id', 'name', 'score', 'systemRegistrationDate', 'systemUpdateDate')
 
 
 class ConceptTypeLinkMetadata(sgqlc.types.Enum):
     __schema__ = utils_api_schema
     __choices__ = ('creator', 'endDate', 'lastUpdater', 'linkType', 'registrationDate', 'startDate', 'updateDate')
 
 
@@ -83,15 +83,15 @@
 class DocumentGrouping(sgqlc.types.Enum):
     __schema__ = utils_api_schema
     __choices__ = ('none', 'story')
 
 
 class DocumentSorting(sgqlc.types.Enum):
     __schema__ = utils_api_schema
-    __choices__ = ('countChildDocs', 'countConcepts', 'countDisambiguatedEntities', 'countEntities', 'countEvents', 'countLinks', 'countNamedEntities', 'countObjects', 'countPropertyCandidates', 'countResearchMaps', 'countTasks', 'id', 'publicationDate', 'registrationDate', 'relevance', 'score', 'secretLevel', 'text', 'title', 'trustLevel', 'updateDate')
+    __choices__ = ('countLinks', 'countNamedEntities', 'id', 'publicationDate', 'registrationDate', 'relevance', 'score', 'title', 'updateDate')
 
 
 class DocumentSourceType(sgqlc.types.Enum):
     __schema__ = utils_api_schema
     __choices__ = ('external', 'internal')
 
 
@@ -341,64 +341,28 @@
     creation_date = sgqlc.types.Field('TimestampInterval', graphql_name='creationDate')
     update_date = sgqlc.types.Field('TimestampInterval', graphql_name='updateDate')
     markers = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null(String)), graphql_name='markers')
     has_linked_issues = sgqlc.types.Field(Boolean, graphql_name='hasLinkedIssues')
     status = sgqlc.types.Field(KbFactStatusFilter, graphql_name='status')
 
 
-class ConceptLinkFactInput(sgqlc.types.Input):
-    __schema__ = utils_api_schema
-    __field_names__ = ('id', 'link_type_id', 'concept_from_fact_id', 'concept_to_fact_id', 'reject', 'approved')
-    id = sgqlc.types.Field(sgqlc.types.non_null(ID), graphql_name='id')
-    link_type_id = sgqlc.types.Field(ID, graphql_name='linkTypeId')
-    concept_from_fact_id = sgqlc.types.Field(ID, graphql_name='conceptFromFactId')
-    concept_to_fact_id = sgqlc.types.Field(ID, graphql_name='conceptToFactId')
-    reject = sgqlc.types.Field(Boolean, graphql_name='reject')
-    approved = sgqlc.types.Field(Boolean, graphql_name='approved')
-
-
-class ConceptLinkFactsCreationInput(sgqlc.types.Input):
-    __schema__ = utils_api_schema
-    __field_names__ = ('document_id', 'access_level_id', 'concept_link_fact', 'concept_link_property_fact', 'property_value_fact', 'composite_property_value_component_fact', 'composite_property_value_fact', 'property_value_mention_fact', 'mention')
-    document_id = sgqlc.types.Field(sgqlc.types.non_null(ID), graphql_name='documentId')
-    access_level_id = sgqlc.types.Field(sgqlc.types.non_null(ID), graphql_name='accessLevelId')
-    concept_link_fact = sgqlc.types.Field(sgqlc.types.non_null(ConceptLinkFactInput), graphql_name='conceptLinkFact')
-    concept_link_property_fact = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null('ConceptLinkPropertyFactInput')), graphql_name='conceptLinkPropertyFact')
-    property_value_fact = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null('PropertyValueFactInput')), graphql_name='propertyValueFact')
-    composite_property_value_component_fact = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null(CompositePropertyValueComponentFactInput)), graphql_name='compositePropertyValueComponentFact')
-    composite_property_value_fact = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null(CompositePropertyValueFactInput)), graphql_name='compositePropertyValueFact')
-    property_value_mention_fact = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null('PropertyValueMentionFactInput')), graphql_name='propertyValueMentionFact')
-    mention = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null('MentionInput')), graphql_name='mention')
-
-
 class ConceptLinkFilterSettings(sgqlc.types.Input):
     __schema__ = utils_api_schema
     __field_names__ = ('is_event', 'concept_link_type', 'document_id', 'creation_date', 'update_date', 'other_concept_name', 'value_type', 'value', 'status')
     is_event = sgqlc.types.Field(Boolean, graphql_name='isEvent')
     concept_link_type = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null(ID)), graphql_name='conceptLinkType')
     document_id = sgqlc.types.Field(ID, graphql_name='documentId')
     creation_date = sgqlc.types.Field('TimestampInterval', graphql_name='creationDate')
     update_date = sgqlc.types.Field('TimestampInterval', graphql_name='updateDate')
     other_concept_name = sgqlc.types.Field(String, graphql_name='otherConceptName')
     value_type = sgqlc.types.Field(ValueType, graphql_name='valueType')
     value = sgqlc.types.Field('ValueFilter', graphql_name='value')
     status = sgqlc.types.Field(KbFactStatusFilter, graphql_name='status')
 
 
-class ConceptLinkPropertyFactInput(sgqlc.types.Input):
-    __schema__ = utils_api_schema
-    __field_names__ = ('id', 'link_property_type_id', 'concept_link_fact_id', 'value_fact_id', 'reject', 'approved')
-    id = sgqlc.types.Field(sgqlc.types.non_null(ID), graphql_name='id')
-    link_property_type_id = sgqlc.types.Field(ID, graphql_name='linkPropertyTypeId')
-    concept_link_fact_id = sgqlc.types.Field(ID, graphql_name='conceptLinkFactId')
-    value_fact_id = sgqlc.types.Field(ID, graphql_name='valueFactId')
-    reject = sgqlc.types.Field(Boolean, graphql_name='reject')
-    approved = sgqlc.types.Field(Boolean, graphql_name='approved')
-
-
 class ConceptLinkTypeFilterSettings(sgqlc.types.Input):
     __schema__ = utils_api_schema
     __field_names__ = ('name', 'concept_from_type_id', 'concept_to_type_id', 'concept_type_and_event_filter', 'is_directed', 'is_hierarchical', 'creator', 'last_updater', 'registration_date', 'update_date', 'has_rel_ext_models')
     name = sgqlc.types.Field(String, graphql_name='name')
     concept_from_type_id = sgqlc.types.Field(ID, graphql_name='conceptFromTypeId')
     concept_to_type_id = sgqlc.types.Field(ID, graphql_name='conceptToTypeId')
     concept_type_and_event_filter = sgqlc.types.Field('conceptTypeAndEventFilter', graphql_name='conceptTypeAndEventFilter')
@@ -1291,14 +1255,21 @@
     hierarchy_level = sgqlc.types.Field(sgqlc.types.non_null(Int), graphql_name='hierarchyLevel')
     translated_text = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='translatedText')
     id = sgqlc.types.Field(sgqlc.types.non_null(ID), graphql_name='id')
     language = sgqlc.types.Field('Language', graphql_name='language')
     translation_mention = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null('MentionUnion'))), graphql_name='translationMention')
 
 
+class GeoConceptProperty(sgqlc.types.Type):
+    __schema__ = utils_api_schema
+    __field_names__ = ('concept', 'concept_property')
+    concept = sgqlc.types.Field(sgqlc.types.non_null('Concept'), graphql_name='concept')
+    concept_property = sgqlc.types.Field(sgqlc.types.non_null('ConceptProperty'), graphql_name='conceptProperty')
+
+
 class GeoPointValue(sgqlc.types.Type):
     __schema__ = utils_api_schema
     __field_names__ = ('point', 'name')
     point = sgqlc.types.Field(Coordinates, graphql_name='point')
     name = sgqlc.types.Field(String, graphql_name='name')
 
 
@@ -1458,32 +1429,32 @@
     __field_names__ = ('total', 'list_merged_concept')
     total = sgqlc.types.Field(sgqlc.types.non_null(Long), graphql_name='total')
     list_merged_concept = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(MergedConcept))), graphql_name='listMergedConcept')
 
 
 class Metrics(sgqlc.types.Type):
     __schema__ = utils_api_schema
-    __field_names__ = ('count_objects', 'count_events', 'count_named_entities', 'count_disambiguated_entities', 'count_property_candidates', 'count_links', 'count_research_maps', 'count_child_docs', 'count_tasks', 'count_story_docs', 'count_concepts', 'count_entities')
-    count_objects = sgqlc.types.Field(sgqlc.types.non_null(Int), graphql_name='countObjects')
-    count_events = sgqlc.types.Field(sgqlc.types.non_null(Int), graphql_name='countEvents')
-    count_named_entities = sgqlc.types.Field(sgqlc.types.non_null(Int), graphql_name='countNamedEntities')
-    count_disambiguated_entities = sgqlc.types.Field(sgqlc.types.non_null(Int), graphql_name='countDisambiguatedEntities')
-    count_property_candidates = sgqlc.types.Field(sgqlc.types.non_null(Int), graphql_name='countPropertyCandidates')
-    count_links = sgqlc.types.Field(sgqlc.types.non_null(Int), graphql_name='countLinks')
-    count_research_maps = sgqlc.types.Field(sgqlc.types.non_null(Int), graphql_name='countResearchMaps')
-    count_child_docs = sgqlc.types.Field(sgqlc.types.non_null(Int), graphql_name='countChildDocs')
-    count_tasks = sgqlc.types.Field(sgqlc.types.non_null(Int), graphql_name='countTasks')
-    count_story_docs = sgqlc.types.Field(sgqlc.types.non_null(Int), graphql_name='countStoryDocs')
-    count_concepts = sgqlc.types.Field(sgqlc.types.non_null(Int), graphql_name='countConcepts')
-    count_entities = sgqlc.types.Field(sgqlc.types.non_null(Int), graphql_name='countEntities')
+    __field_names__ = ('count_concepts', 'count_objects', 'count_events', 'count_named_entities', 'count_disambiguated_entities', 'count_property_candidates', 'count_links', 'count_research_maps', 'count_child_docs', 'count_tasks', 'count_story_docs', 'count_entities')
+    count_concepts = sgqlc.types.Field(Int, graphql_name='countConcepts')
+    count_objects = sgqlc.types.Field(Int, graphql_name='countObjects')
+    count_events = sgqlc.types.Field(Int, graphql_name='countEvents')
+    count_named_entities = sgqlc.types.Field(Int, graphql_name='countNamedEntities')
+    count_disambiguated_entities = sgqlc.types.Field(Int, graphql_name='countDisambiguatedEntities')
+    count_property_candidates = sgqlc.types.Field(Int, graphql_name='countPropertyCandidates')
+    count_links = sgqlc.types.Field(Int, graphql_name='countLinks')
+    count_research_maps = sgqlc.types.Field(Int, graphql_name='countResearchMaps')
+    count_child_docs = sgqlc.types.Field(Int, graphql_name='countChildDocs')
+    count_tasks = sgqlc.types.Field(Int, graphql_name='countTasks')
+    count_story_docs = sgqlc.types.Field(Int, graphql_name='countStoryDocs')
+    count_entities = sgqlc.types.Field(Int, graphql_name='countEntities')
 
 
 class Mutation(sgqlc.types.Type):
     __schema__ = utils_api_schema
-    __field_names__ = ('add_alias_to_concept', 'get_or_add_account', 'get_or_add_platform', 'get_or_add_concept', 'get_or_add_concept_new', 'get_or_add_concept_link')
+    __field_names__ = ('add_alias_to_concept', 'get_or_add_account', 'get_or_add_platform', 'get_or_add_concept', 'get_or_add_concept_new')
     add_alias_to_concept = sgqlc.types.Field(sgqlc.types.non_null('State'), graphql_name='addAliasToConcept', args=sgqlc.types.ArgDict((
         ('form', sgqlc.types.Arg(sgqlc.types.non_null(AliasCreateInput), graphql_name='form', default=None)),
 ))
     )
     get_or_add_account = sgqlc.types.Field(sgqlc.types.non_null(ID), graphql_name='getOrAddAccount', args=sgqlc.types.ArgDict((
         ('form', sgqlc.types.Arg(sgqlc.types.non_null(AccountGetOrCreateInput), graphql_name='form', default=None)),
 ))
@@ -1501,21 +1472,14 @@
     )
     get_or_add_concept_new = sgqlc.types.Field(sgqlc.types.non_null('Concept'), graphql_name='getOrAddConceptNew', args=sgqlc.types.ArgDict((
         ('filter_settings', sgqlc.types.Arg(sgqlc.types.non_null(ConceptFilterSettings), graphql_name='filterSettings', default=None)),
         ('form', sgqlc.types.Arg(sgqlc.types.non_null(ConceptFactsCreationInput), graphql_name='form', default=None)),
         ('take_first_result', sgqlc.types.Arg(Boolean, graphql_name='takeFirstResult', default=False)),
 ))
     )
-    get_or_add_concept_link = sgqlc.types.Field(sgqlc.types.non_null('ConceptLink'), graphql_name='getOrAddConceptLink', args=sgqlc.types.ArgDict((
-        ('concept_from_id', sgqlc.types.Arg(sgqlc.types.non_null(ID), graphql_name='conceptFromId', default=None)),
-        ('concept_to_id', sgqlc.types.Arg(sgqlc.types.non_null(ID), graphql_name='conceptToId', default=None)),
-        ('filter_settings', sgqlc.types.Arg(sgqlc.types.non_null(ConceptLinkFilterSettings), graphql_name='filterSettings', default=None)),
-        ('form', sgqlc.types.Arg(sgqlc.types.non_null(ConceptLinkFactsCreationInput), graphql_name='form', default=None)),
-))
-    )
 
 
 class NERCRegexp(sgqlc.types.Type):
     __schema__ = utils_api_schema
     __field_names__ = ('regexp', 'context_regexp', 'auto_create')
     regexp = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='regexp')
     context_regexp = sgqlc.types.Field(String, graphql_name='contextRegexp')
@@ -1528,15 +1492,15 @@
     id = sgqlc.types.Field(sgqlc.types.non_null(ID), graphql_name='id')
     property_value_type = sgqlc.types.Field(sgqlc.types.non_null(CompositePropertyValueType), graphql_name='propertyValueType')
     value = sgqlc.types.Field(sgqlc.types.non_null('Value'), graphql_name='value')
 
 
 class ParagraphMetadata(sgqlc.types.Type):
     __schema__ = utils_api_schema
-    __field_names__ = ('page_id', 'line_id', 'original_text', 'hidden', 'content_type', 'bullet', 'header', 'width', 'height', 'language', 'rowspan', 'colspan', 'name', 'size', 'md5', 'text_translations', 'paragraph_type')
+    __field_names__ = ('page_id', 'line_id', 'original_text', 'hidden', 'content_type', 'bullet', 'header', 'width', 'height', 'language', 'rowspan', 'colspan', 'name', 'size', 'md5', 'paragraph_type')
     page_id = sgqlc.types.Field(Int, graphql_name='pageId')
     line_id = sgqlc.types.Field(Int, graphql_name='lineId')
     original_text = sgqlc.types.Field(String, graphql_name='originalText')
     hidden = sgqlc.types.Field(Boolean, graphql_name='hidden')
     content_type = sgqlc.types.Field(String, graphql_name='contentType')
     bullet = sgqlc.types.Field(String, graphql_name='bullet')
     header = sgqlc.types.Field(Boolean, graphql_name='header')
@@ -1544,15 +1508,14 @@
     height = sgqlc.types.Field(Int, graphql_name='height')
     language = sgqlc.types.Field(String, graphql_name='language')
     rowspan = sgqlc.types.Field(Int, graphql_name='rowspan')
     colspan = sgqlc.types.Field(Int, graphql_name='colspan')
     name = sgqlc.types.Field(String, graphql_name='name')
     size = sgqlc.types.Field(Int, graphql_name='size')
     md5 = sgqlc.types.Field(String, graphql_name='md5')
-    text_translations = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null('Translation')), graphql_name='textTranslations')
     paragraph_type = sgqlc.types.Field(sgqlc.types.non_null(NodeType), graphql_name='paragraphType')
 
 
 class Parameter(sgqlc.types.Type):
     __schema__ = utils_api_schema
     __field_names__ = ('key', 'value')
     key = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='key')
@@ -2261,15 +2224,15 @@
         ('filter_settings', sgqlc.types.Arg(ConceptFilterSettings, graphql_name='filterSettings', default=None)),
 ))
     )
 
 
 class Document(sgqlc.types.Type, RecordInterface):
     __schema__ = utils_api_schema
-    __field_names__ = ('id', 'title', 'external_url', 'publication_date', 'publication_author', 'notes', 'document_type', 'highlightings', 'markers', 'tables', 'metadata', 'uuid', 'trust_level', 'story', 'score', 'has_text', 'parent', 'list_child', 'pagination_child', 'internal_url', 'avatar', 'metric', 'pagination_concept_fact', 'list_concept_fact', 'pagination_concept_link_fact', 'list_concept_link_document_fact', 'preview', 'list_fact_with_mention', 'pagination_redmine_issues', 'pagination_issue', 'access_level', 'text', 'additional_text', 'list_subscription', 'pagination_similar_documents', 'is_read', 'list_mention_link', 'node', 'metadata_concept', 'list_fact', 'extra_metadata', 'list_mention', 'fact')
+    __field_names__ = ('id', 'title', 'external_url', 'publication_date', 'publication_author', 'notes', 'document_type', 'highlightings', 'markers', 'tables', 'metadata', 'uuid', 'trust_level', 'story', 'score', 'has_text', 'parent', 'list_child', 'pagination_child', 'internal_url', 'avatar', 'metric', 'pagination_concept_fact', 'list_concept_fact', 'pagination_concept_link_fact', 'list_concept_link_document_fact', 'preview', 'list_fact_with_mention', 'pagination_redmine_issues', 'pagination_issue', 'access_level', 'text', 'additional_text', 'list_subscription', 'pagination_similar_documents', 'is_read', 'list_mention_link', 'node', 'metadata_concept', 'text_translations', 'list_fact', 'extra_metadata', 'list_mention', 'fact')
     id = sgqlc.types.Field(sgqlc.types.non_null(ID), graphql_name='id')
     title = sgqlc.types.Field(String, graphql_name='title')
     external_url = sgqlc.types.Field(String, graphql_name='externalUrl')
     publication_date = sgqlc.types.Field(UnixTime, graphql_name='publicationDate')
     publication_author = sgqlc.types.Field(String, graphql_name='publicationAuthor')
     notes = sgqlc.types.Field(String, graphql_name='notes')
     document_type = sgqlc.types.Field(sgqlc.types.non_null(DocumentType), graphql_name='documentType')
@@ -2345,14 +2308,18 @@
 ))
     )
     node = sgqlc.types.Field(FlatDocumentStructure, graphql_name='node', args=sgqlc.types.ArgDict((
         ('id', sgqlc.types.Arg(sgqlc.types.non_null(ID), graphql_name='id', default=None)),
 ))
     )
     metadata_concept = sgqlc.types.Field(Concept, graphql_name='metadataConcept')
+    text_translations = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(Translation))), graphql_name='textTranslations', args=sgqlc.types.ArgDict((
+        ('node_id', sgqlc.types.Arg(sgqlc.types.non_null(ID), graphql_name='nodeId', default=None)),
+))
+    )
     list_fact = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null('Fact'))), graphql_name='listFact')
     extra_metadata = sgqlc.types.Field(JSON, graphql_name='extraMetadata')
     list_mention = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null('MentionUnion'))), graphql_name='listMention')
     fact = sgqlc.types.Field('Fact', graphql_name='fact', args=sgqlc.types.ArgDict((
         ('id', sgqlc.types.Arg(sgqlc.types.non_null(ID), graphql_name='id', default=None)),
 ))
     )
@@ -2449,15 +2416,15 @@
     __field_names__ = ('value_fact', 'mention')
     value_fact = sgqlc.types.Field(sgqlc.types.non_null(ConceptPropertyValueCandidateFact), graphql_name='valueFact')
     mention = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null('MentionUnion'))), graphql_name='mention')
 
 
 class ResearchMap(sgqlc.types.Type, RecordInterface):
     __schema__ = utils_api_schema
-    __field_names__ = ('id', 'name', 'description', 'is_temporary', 'markers', 'list_node', 'list_edge', 'research_map_statistics', 'list_group', 'is_active', 'access_level', 'pagination_concept', 'pagination_story', 'pagination_research_map')
+    __field_names__ = ('id', 'name', 'description', 'is_temporary', 'markers', 'list_node', 'list_edge', 'research_map_statistics', 'list_group', 'is_active', 'access_level', 'pagination_concept', 'pagination_story', 'pagination_research_map', 'list_geo_concept_properties')
     id = sgqlc.types.Field(sgqlc.types.non_null(ID), graphql_name='id')
     name = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='name')
     description = sgqlc.types.Field(String, graphql_name='description')
     is_temporary = sgqlc.types.Field(sgqlc.types.non_null(Boolean), graphql_name='isTemporary')
     markers = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(String))), graphql_name='markers')
     list_node = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(MapNode))), graphql_name='listNode', args=sgqlc.types.ArgDict((
         ('filter_settings', sgqlc.types.Arg(MapNodeFilterSettings, graphql_name='filterSettings', default=None)),
@@ -2498,14 +2465,15 @@
         ('offset', sgqlc.types.Arg(Int, graphql_name='offset', default=0)),
         ('filter_settings', sgqlc.types.Arg(sgqlc.types.non_null(ResearchMapFilterSettings), graphql_name='filterSettings', default=None)),
         ('direction', sgqlc.types.Arg(SortDirection, graphql_name='direction', default='descending')),
         ('sort_field', sgqlc.types.Arg(ResearchMapSorting, graphql_name='sortField', default='conceptAndDocumentLink')),
         ('research_map_content_select_input', sgqlc.types.Arg(ResearchMapContentUpdateInput, graphql_name='ResearchMapContentSelectInput', default=None)),
 ))
     )
+    list_geo_concept_properties = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(GeoConceptProperty))), graphql_name='listGeoConceptProperties')
 
 
 class TextNodeMention(sgqlc.types.Type, MentionInterface, RecordInterface):
     __schema__ = utils_api_schema
     __field_names__ = ('node_id', 'start', 'end')
     node_id = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='nodeId')
     start = sgqlc.types.Field(sgqlc.types.non_null(Int), graphql_name='start')
@@ -2549,15 +2517,15 @@
 class ConceptPropertyLikeFact(sgqlc.types.Union):
     __schema__ = utils_api_schema
     __types__ = (ConceptPropertyFact, ConceptLinkPropertyFact)
 
 
 class ConceptViewValue(sgqlc.types.Union):
     __schema__ = utils_api_schema
-    __types__ = (DateTimeValue, GeoPointValue, IntValue, DoubleValue, StringLocaleValue, StringValue, LinkValue, CompositeValue, Concept, ConceptType, ConceptLinkType, User, Image)
+    __types__ = (DateTimeValue, GeoPointValue, IntValue, DoubleValue, StringLocaleValue, StringValue, LinkValue, CompositeValue, Concept, ConceptType, ConceptLinkType, User, Image, TimestampValue)
 
 
 class Entity(sgqlc.types.Union):
     __schema__ = utils_api_schema
     __types__ = (Concept, Document, ConceptCandidateFact, ConceptType)
```

### Comparing `ptal_api-1.0.0a6/ptal_api/scripts/type_mapper.py` & `ptal_api-1.0.0a7/ptal_api/scripts/type_mapper.py`

 * *Files identical despite different names*

### Comparing `ptal_api-1.0.0a6/ptal_api/tdm_builder/tdm_builder.py` & `ptal_api-1.0.0a7/ptal_api/tdm_builder/tdm_builder.py`

 * *Files identical despite different names*

### Comparing `ptal_api-1.0.0a6/pyproject.toml` & `ptal_api-1.0.0a7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ptal-api"
-version = "1.0.0a6"
+version = "1.0.0a7"
 description = "TALISMAN API adapter"
 authors = ["Evgeny Bechkalo <bechkalo@ispras.ru>", "Ivan Medvedev <medvedev.iv@ispras.ru>", "Alexey Isakov <isakov@ispras.ru>"]
 readme = "README.md"
 packages = [{include = "ptal_api"}]
 classifiers = [
     'Development Status :: 3 - Alpha',
     'Programming Language :: Python :: 3',
```

### Comparing `ptal_api-1.0.0a6/PKG-INFO` & `ptal_api-1.0.0a7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ptal-api
-Version: 1.0.0a6
+Version: 1.0.0a7
 Summary: TALISMAN API adapter
 Author: Evgeny Bechkalo
 Author-email: bechkalo@ispras.ru
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

