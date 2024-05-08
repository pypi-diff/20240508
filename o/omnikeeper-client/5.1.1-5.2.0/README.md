# Comparing `tmp/omnikeeper_client-5.1.1-py3-none-any.whl.zip` & `tmp/omnikeeper_client-5.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,18 @@
-Zip file size: 19428 bytes, number of entries: 15
--rw-r--r--  2.0 unx     1049 b- defN 24-Feb-06 12:05 omnikeeper_client/__init__.py
+Zip file size: 20869 bytes, number of entries: 16
+-rw-r--r--  2.0 unx     1265 b- defN 24-May-08 06:45 omnikeeper_client/__init__.py
 -rw-r--r--  2.0 unx     1984 b- defN 24-Mar-14 11:13 omnikeeper_client/apiclient.py
 -rw-r--r--  2.0 unx     5040 b- defN 24-Feb-06 12:05 omnikeeper_client/ci.py
--rw-r--r--  2.0 unx     3743 b- defN 24-Feb-06 12:05 omnikeeper_client/dataframes.py
+-rw-r--r--  2.0 unx     3796 b- defN 24-Apr-04 07:13 omnikeeper_client/dataframes.py
 -rw-r--r--  2.0 unx     3232 b- defN 24-Feb-06 12:05 omnikeeper_client/layer.py
--rw-r--r--  2.0 unx    10578 b- defN 24-Feb-06 12:05 omnikeeper_client/simple_traits.py
--rw-r--r--  2.0 unx     4521 b- defN 24-Feb-06 12:05 omnikeeper_client/trait.py
--rw-r--r--  2.0 unx    18432 b- defN 24-Feb-06 12:05 omnikeeper_client/traitentities.py
+-rw-r--r--  2.0 unx     2765 b- defN 24-Apr-05 10:02 omnikeeper_client/pyd.py
+-rw-r--r--  2.0 unx    10639 b- defN 24-Apr-04 07:14 omnikeeper_client/simple_traits.py
+-rw-r--r--  2.0 unx     4574 b- defN 24-Apr-04 07:13 omnikeeper_client/trait.py
+-rw-r--r--  2.0 unx    20532 b- defN 24-May-08 06:54 omnikeeper_client/traitentities.py
 -rw-r--r--  2.0 unx     5262 b- defN 24-Feb-06 12:05 omnikeeper_client/typing.py
 -rw-r--r--  2.0 unx      917 b- defN 24-Feb-06 12:05 omnikeeper_client/util.py
--rw-r--r--  2.0 unx    11357 b- defN 24-Mar-14 11:19 omnikeeper_client-5.1.1.dist-info/LICENSE
--rw-r--r--  2.0 unx      542 b- defN 24-Mar-14 11:19 omnikeeper_client-5.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Mar-14 11:19 omnikeeper_client-5.1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       18 b- defN 24-Mar-14 11:19 omnikeeper_client-5.1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1292 b- defN 24-Mar-14 11:19 omnikeeper_client-5.1.1.dist-info/RECORD
-15 files, 68059 bytes uncompressed, 17278 bytes compressed:  74.6%
+-rw-r--r--  2.0 unx    11357 b- defN 24-May-08 06:57 omnikeeper_client-5.2.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx      572 b- defN 24-May-08 06:57 omnikeeper_client-5.2.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-08 06:57 omnikeeper_client-5.2.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       18 b- defN 24-May-08 06:57 omnikeeper_client-5.2.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1373 b- defN 24-May-08 06:57 omnikeeper_client-5.2.0.dist-info/RECORD
+16 files, 73418 bytes uncompressed, 18595 bytes compressed:  74.7%
```

## zipnote {}

```diff
@@ -9,14 +9,17 @@
 
 Filename: omnikeeper_client/dataframes.py
 Comment: 
 
 Filename: omnikeeper_client/layer.py
 Comment: 
 
+Filename: omnikeeper_client/pyd.py
+Comment: 
+
 Filename: omnikeeper_client/simple_traits.py
 Comment: 
 
 Filename: omnikeeper_client/trait.py
 Comment: 
 
 Filename: omnikeeper_client/traitentities.py
@@ -24,23 +27,23 @@
 
 Filename: omnikeeper_client/typing.py
 Comment: 
 
 Filename: omnikeeper_client/util.py
 Comment: 
 
-Filename: omnikeeper_client-5.1.1.dist-info/LICENSE
+Filename: omnikeeper_client-5.2.0.dist-info/LICENSE
 Comment: 
 
-Filename: omnikeeper_client-5.1.1.dist-info/METADATA
+Filename: omnikeeper_client-5.2.0.dist-info/METADATA
 Comment: 
 
-Filename: omnikeeper_client-5.1.1.dist-info/WHEEL
+Filename: omnikeeper_client-5.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: omnikeeper_client-5.1.1.dist-info/top_level.txt
+Filename: omnikeeper_client-5.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: omnikeeper_client-5.1.1.dist-info/RECORD
+Filename: omnikeeper_client-5.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## omnikeeper_client/__init__.py

```diff
@@ -43,14 +43,24 @@
 from .traitentities import (
     get_latest_trait_change,
     get_all_traitentities,
     get_all_traitentity_relations,
     set_traitentity_relations,
     bulk_replace_trait_entities,
     bulk_replace_trait_entities_by_filter,
+    bulk_replace_traitentity_relations,
 )
 
 from .dataframes import (
     get_all_traitentities_dataframe,
     bulk_replace_trait_entities_dataframe,
     bulk_replace_trait_entities_by_filter_dataframe,
 )
+
+from .pyd import (
+    SerializableUUID,
+    AttributeName,
+    AttributeOptional,
+    TypeHint,
+    get_all_traitentities_pydantic,
+    bulk_replace_trait_entities_pydantic
+)
```

## omnikeeper_client/dataframes.py

```diff
@@ -1,16 +1,19 @@
 import omnikeeper_client as okc
 import pandas as pd
 from .traitentities import (
     _get_all_traitentities,
     _bulk_replace_trait_entities_by_filter,
     _bulk_replace_trait_entities,
 )
+from typing import (
+    List,
+)
 
-def get_all_traitentities_dataframe(ok_api_client: okc.OkApiClient, trait_name: str, layers: [str], keep_ciid_as_column: bool = False) -> pd.DataFrame:
+def get_all_traitentities_dataframe(ok_api_client: okc.OkApiClient, trait_name: str, layers: List[str], keep_ciid_as_column: bool = False) -> pd.DataFrame:
     """
     Returns all traitentites as pandas dataframe 
 
     Parameters
     ----------
     ok_api_client : OkApiClient
         The OkApiClient instance representing omnikeeper connection
@@ -29,15 +32,15 @@
 
     data_list = _get_all_traitentities(ok_api_client, trait_id=trait_name, layers=layers)
     data_df = pd.DataFrame(data_list)
     data_df.set_index('ciid', inplace=True, drop=not keep_ciid_as_column)
 
     return data_df
 
-def bulk_replace_trait_entities_by_filter_dataframe(ok_api_client: okc.OkApiClient, trait_name: str, input: pd.DataFrame, id_attributes: [str], id_relations: [str], write_layer: str, read_layers: [str] = None, filter: object = {}) -> bool:
+def bulk_replace_trait_entities_by_filter_dataframe(ok_api_client: okc.OkApiClient, trait_name: str, input: pd.DataFrame, id_attributes: List[str], id_relations: List[str], write_layer: str, read_layers: List[str] = None, filter: object = {}) -> bool:
     """
     Replaces all traitentites in a layer input data is a dataframe, it can use a filter when updating the traitentities,
     this will also delete all old trait entities, if there are any
 
     Parameters
     ----------
     ok_api_client : OkApiClient
@@ -70,15 +73,15 @@
         True if the update is successful, False otherwise
     """
 
     input_as_dict = input.to_dict('records')
     result = _bulk_replace_trait_entities_by_filter(ok_api_client, trait_name, input_as_dict, id_attributes, id_relations, write_layer, read_layers, filter)
     return result
 
-def bulk_replace_trait_entities_dataframe(ok_api_client: okc.OkApiClient, trait_name: str, input: pd.DataFrame, write_layer: str, read_layers: [str] = None) -> bool:
+def bulk_replace_trait_entities_dataframe(ok_api_client: okc.OkApiClient, trait_name: str, input: pd.DataFrame, write_layer: str, read_layers: List[str] = None) -> bool:
     """
     Sets all traitentities, the input is a pd.DataFrame, this will also delete all old trait entities, if there are any
 
     Parameters
     ----------
     ok_api_client : OkApiClient
         The OkApiClient instance representing omnikeeper connection
```

## omnikeeper_client/simple_traits.py

```diff
@@ -2,14 +2,17 @@
 import pandas as pd
 import graphql
 from graphql import GraphQLType
 from gql.dsl import DSLQuery, DSLVariableDefinitions, DSLSchema, dsl_gql
 from dateutil import parser
 import datetime
 from deprecated import deprecated
+from typing import (
+    List,
+)
 
 @deprecated(category=FutureWarning, reason="please use omnikeeper_client.* public functions instead, if really needed, use  OkApiClient()._is_relation_field()")
 def is_relation_field(type: GraphQLType) -> bool:
     # a typical relation field looks like this:
     # GraphQLList <GraphQLObjectType 'TEWrapper_tsa_cmdb__interface'>>
     # or
     # GraphQLList <GraphQLObjectType 'RelatedCIType'>
@@ -38,15 +41,15 @@
 @deprecated(category=FutureWarning, reason="please use omnikeeper_client.* public functions instead, if really needed, use  OkApiClient()._get_prefixed_trait_name()")
 def get_prefixed_trait_name(name: str) -> str:
     if name.startswith("_"):
         return f"m{name}"
     return name
 
 @deprecated(category=FutureWarning, reason="please use omnikeeper_client public function get_latest_trait_change() instead")
-def get_latest_change_for_all(client: Client, trait_name: str, layers: [str]) -> datetime.datetime:
+def get_latest_change_for_all(client: Client, trait_name: str, layers: List[str]) -> datetime.datetime:
     with client as session:
         ds = DSLSchema(client.schema)
 
         escaped_trait_name = get_escaped_trait_name(trait_name)
         prefixed_escaped_trait_name = get_prefixed_trait_name(escaped_trait_name)
 
         tetType = getattr(ds.TraitEntitiesType, prefixed_escaped_trait_name)
@@ -67,15 +70,15 @@
         result = session.execute(query, variable_values={"layers": layers})
 
         timestamp_str = result['traitEntities'][prefixed_escaped_trait_name]['latestChangeAll']['timestamp']
         timestamp = parser.parse(timestamp_str)
         return timestamp
 
 @deprecated(category=FutureWarning, reason="please use omnikeeper_client.* public functions instead, use get_all_traitentities_list() if you want to work with list, use get_all_traitentities_dataframe() if you want to work with dataframes")
-def get_all(client: Client, trait_name: str, layers: [str], keep_ciid_as_column: bool = False) -> pd.DataFrame:
+def get_all(client: Client, trait_name: str, layers: List[str], keep_ciid_as_column: bool = False) -> pd.DataFrame:
     with client as session:
         ds = DSLSchema(client.schema)
 
         escaped_trait_name = get_escaped_trait_name(trait_name)
         prefixed_escaped_trait_name = get_prefixed_trait_name(escaped_trait_name)
 
         tetType = getattr(ds.TraitEntitiesType, prefixed_escaped_trait_name)
@@ -105,15 +108,15 @@
                 .set_index('ciid', drop=not keep_ciid_as_column)
         )
         data_frame.columns = data_frame.columns.str.removeprefix('entity.')
 
         return data_frame
 
 @deprecated(category=FutureWarning, reason="please use omnikeeper_client public function get_trait_relation() instead")
-def get_relation(client: Client, trait_name: str, relation_name: str, layers: [str], keep_ciid_as_column: bool = False) -> pd.DataFrame:
+def get_relation(client: Client, trait_name: str, relation_name: str, layers: List[str], keep_ciid_as_column: bool = False) -> pd.DataFrame:
     with client as session:
         ds = DSLSchema(client.schema)
 
         escaped_trait_name = get_escaped_trait_name(trait_name)
         prefixed_escaped_trait_name = get_prefixed_trait_name(escaped_trait_name)
 
         tetType = getattr(ds.TraitEntitiesType, prefixed_escaped_trait_name)
@@ -144,15 +147,15 @@
                 .set_index('base_ciid', drop=not keep_ciid_as_column)
         )
         data_frame['related_ciids'] = data_frame['related_ciids'].apply(lambda x: list(map(lambda i: i['relatedCIID'], x)))
 
         return data_frame
     
 @deprecated(category=FutureWarning, reason="please use omnikeeper_client.* public functions instead, use bulk_replace_trait_entities_list() if you want to work with list, use bulk_replace_trait_entities_dataframe() if you want to work with dataframes")
-def set_all(client: Client, trait_name: str, input: pd.DataFrame, write_layer: str, read_layers: [str] = None) -> bool:
+def set_all(client: Client, trait_name: str, input: pd.DataFrame, write_layer: str, read_layers: List[str] = None) -> bool:
     escaped_trait_name = get_escaped_trait_name(trait_name)
     prefixed_escaped_trait_name = get_prefixed_trait_name(escaped_trait_name)
 
     with client as session:
         query = gql(f"""
             mutation($readLayers: [String]!, $writeLayer: String!, $input: [TE_CIID_And_Upsert_Attributes_Only_Input_{escaped_trait_name}]!) {{
             bulkReplace_{prefixed_escaped_trait_name}(
@@ -173,15 +176,15 @@
             writeLayer=write_layer, 
             readLayers=read_layers, 
             input=final_input
             ))
         return result[f"bulkReplace_{prefixed_escaped_trait_name}"]["success"]
 
 @deprecated(category=FutureWarning, reason="please use omnikeeper_client.* public functions instead, use bulk_replace_trait_entities_by_filter_list() if you want to work with list, use bulk_replace_trait_entities_by_filter_dataframe() if you want to work with dataframes")
-def bulk_replace(client: Client, trait_name: str, input: pd.DataFrame, id_attributes: [str], id_relations: [str], write_layer: str, read_layers: [str] = None, filter: object = {}) -> bool:
+def bulk_replace(client: Client, trait_name: str, input: pd.DataFrame, id_attributes: List[str], id_relations: List[str], write_layer: str, read_layers: List[str] = None, filter: object = {}) -> bool:
     escaped_trait_name = get_escaped_trait_name(trait_name)
     prefixed_escaped_trait_name = get_prefixed_trait_name(escaped_trait_name)
 
     with client as session:
         # example for filter object: {type: {exact: "Validator"}, context: {exact: "test"}, group: {exact: "test"} }
         query = gql(f"""
             mutation($readLayers: [String]!, $writeLayer: String!, $idAttributes: [String!]!, $idRelations: [String!]!, $filter: TE_filter_Input_{escaped_trait_name}!, $input: [TE_Upsert_Input_{escaped_trait_name}]!) {{
```

## omnikeeper_client/trait.py

```diff
@@ -1,38 +1,41 @@
 import omnikeeper_client as okc
 import omnikeeper_client.typing as okc_typing
 import omnikeeper_client.util as okc_util
 from gql import gql
 from gql.transport.exceptions import (
     TransportQueryError,
 )
+from typing import (
+    List,
+)
 
 # NOTE: these classes use camelCase members, so they can be easily encoded for GraphQL using okc_util.to_dict()
 class TraitAttributeDefinition:
     def __init__(self, identifier: str, name: str, attribute_type: str = okc_typing.ATTRIBUTETYPE_TEXT, is_array: bool = False):
         self.identifier = identifier
         self.template = dict(
             name = name,
             type = attribute_type,
             isArray = is_array,
             isID = False, # NOTE: isID is deprecated anyway, so we don't support this
             valueConstraints = [] # TODO: support value constraints properly
         )
 
 class TraitRelationDefinition:
-    def __init__(self, identifier: str, predicate_id: str, direction_forward: bool, trait_hints: [str] = []):
+    def __init__(self, identifier: str, predicate_id: str, direction_forward: bool, trait_hints: List[str] = []):
         self.identifier = identifier
         self.template = dict(
             predicateID = predicate_id,
             directionForward = direction_forward,
             traitHints = trait_hints
         )
 
 class TraitDefinition:
-    def __init__(self, trait_id: str, required_attributes: [TraitAttributeDefinition], optional_attributes: [TraitAttributeDefinition] = [], optional_relations: [TraitRelationDefinition] = [], required_traits: [str] = []):
+    def __init__(self, trait_id: str, required_attributes: List[TraitAttributeDefinition], optional_attributes: List[TraitAttributeDefinition] = [], optional_relations: List[TraitRelationDefinition] = [], required_traits: List[str] = []):
         self.id = trait_id
         self.requiredAttributes = required_attributes
         self.optionalAttributes = optional_attributes
         self.optionalRelations = optional_relations
         self.requiredTraits = required_traits
 
 def upsert_trait(ok_api_client: okc.OkApiClient, trait_definition: TraitDefinition):
```

## omnikeeper_client/traitentities.py

```diff
@@ -3,14 +3,17 @@
 from graphql import GraphQLType
 from gql.dsl import DSLQuery, DSLVariableDefinitions, DSLSchema, dsl_gql
 from dateutil import parser
 import datetime
 import omnikeeper_client as okc
 from typing import List, Dict, Any
 import uuid
+from typing import (
+    List,
+)
 
 
 def _is_relation_field(type: GraphQLType) -> bool:
     """
     Checks if field is a relation. A typical relation field looks like this:
     GraphQLList <GraphQLObjectType 'TEWrapper_tsa_cmdb__interface'>> or
     GraphQLList <GraphQLObjectType 'RelatedCIType'>
@@ -77,15 +80,15 @@
     str
         the prefixed trait name with m prefix
     """
     if name.startswith("_"):
         return f"m{name}"
     return name
 
-def get_latest_trait_change(ok_api_client: okc.OkApiClient, trait_id: str, layers: [str]) -> datetime.datetime:
+def get_latest_trait_change(ok_api_client: okc.OkApiClient, trait_id: str, layers: List[str]) -> datetime.datetime:
     """
     Returns the timestamp of the latest change for the provided trait
 
     Parameters
     ----------
     ok_api_client : OkApiClient
         The OkApiClient instance representing omnikeeper connection
@@ -125,15 +128,15 @@
 
         result = session.execute(query, variable_values={"layers": layers})
 
         timestamp_str = result['traitEntities'][prefixed_escaped_trait_id]['latestChangeAll']['timestamp']
         timestamp = parser.parse(timestamp_str)
         return timestamp
  
-def _get_all_traitentities(ok_api_client: okc.OkApiClient, trait_id: str, layers: [str]) -> List[Dict[str,Any]]:
+def _get_all_traitentities(ok_api_client: okc.OkApiClient, trait_id: str, layers: List[str]) -> List[Dict[str,Any]]:
     """
     Internal method used to fetch all traitentites
 
     Parameters
     ----------
     ok_api_client : OkApiClient
         The OkApiClient instance representing omnikeeper connection
@@ -182,15 +185,15 @@
         data_list = result['traitEntities'][prefixed_escaped_trait_id]['all']
         for data in data_list:
             data.update(data.pop('entity'))
 
         return data_list
     
   
-def get_all_traitentities(ok_api_client: okc.OkApiClient, trait_id: str, layers: [str]) -> List[Dict[str,Any]]:
+def get_all_traitentities(ok_api_client: okc.OkApiClient, trait_id: str, layers: List[str]) -> List[Dict[str,Any]]:
     """
     Returns all traitentites
 
     Parameters
     ----------
     ok_api_client : OkApiClient
         The OkApiClient instance representing omnikeeper connection
@@ -206,15 +209,15 @@
     List[Dict[str,Any]]
         result containing all traitentites
     """
     
     trait_entities = _get_all_traitentities(ok_api_client, trait_id, layers)
     return trait_entities
 
-def get_all_traitentity_relations(ok_api_client: okc.OkApiClient, trait_id: str, traitrelation_id: str, layers: [str]) -> List[Dict[str,Any]]:
+def get_all_traitentity_relations(ok_api_client: okc.OkApiClient, trait_id: str, traitrelation_id: str, layers: List[str]) -> List[Dict[str,Any]]:
     """
     Returns the trait relations for all trait entities of a particular trait
 
     Parameters
     ----------
     ok_api_client : OkApiClient
         The OkApiClient instance representing omnikeeper connection
@@ -268,15 +271,15 @@
                 "base_ciid": entity['ciid'],
                 "related_ciids": related_ciids,
             }
             result_list.append(result_dict)
 
         return result_list
     
-def set_traitentity_relations(ok_api_client: okc.OkApiClient, trait_id: str, traitrelation_id: str, base_ciid: uuid.UUID | str, related_ciids: List[uuid.UUID | str], write_layer: str, read_layers: [str] = None) -> bool:
+def set_traitentity_relations(ok_api_client: okc.OkApiClient, trait_id: str, traitrelation_id: str, base_ciid: uuid.UUID | str, related_ciids: List[uuid.UUID | str], write_layer: str, read_layers: List[str] = None) -> bool:
     """
     Sets a particular trait relation of a particular trait for a single CI
     Adds new traitrelations and deletes all traitrelations not in the provided list
 
     Parameters
     ----------
     ok_api_client : OkApiClient
@@ -328,16 +331,72 @@
         writeLayer=write_layer, 
         readLayers=read_layers, 
         baseCIID=base_ciid,
         relatedCIIDs=related_ciids
         ))
 
     return True
+
+def bulk_replace_traitentity_relations(ok_api_client: okc.OkApiClient, trait_id: str, traitrelation_id: str, input: List[Dict[str, Any]], write_layer: str, read_layers: List[str] = None) -> bool:
+    """
+    Bulk replaces a particular trait relation of a particular trait for ALL trait entities of that trait
+    Adds new traitrelations and deletes all relevant traitrelations not in the provided list
+
+    Parameters
+    ----------
+    ok_api_client : OkApiClient
+        The OkApiClient instance representing omnikeeper connection
+
+    trait_id : str
+        the id of the trait
+
+    traitrelation_id: str
+        the id of the trait's traitrelation
+        
+    input: List[Dict[str, Any]]
+        a list of dicts, the dicts in the following form: { "baseCIID" = <ciid>, "relatedCIIDs" = [<ciid>, <ciid>, ...] }
+
+    write_layer : str
+        the id of the layer in which the data should be added
+
+    read_layers : [str]
+        A list with ids of the layers in which the omnikeeper will look if trait entities already exist
+
+    Returns
+    -------
+    bool 
+        True if the update is successful, False otherwise
+    """
+
+    prefixed_escaped_trait_id = _get_prefixed_trait_id(_get_escaped_trait_id(trait_id))
+    escaped_traitrelation_id = _get_escaped_trait_id(traitrelation_id)
+    query = gql(f"""
+        mutation($readLayers: [String]!, $writeLayer: String!, $input: [TE_Upsert_Relations_Only_Input]!) {{
+        bulkReplaceRelations_{prefixed_escaped_trait_id}_{escaped_traitrelation_id}(
+            layers: $readLayers
+            writeLayer: $writeLayer
+            input: $input
+        ) {{
+            success
+        }}
+        }}
+        """)
+        
+    if read_layers is None:
+        read_layers = [write_layer]
+
+    result = ok_api_client.execute_graphql(query, variables=dict(
+        writeLayer=write_layer, 
+        readLayers=read_layers, 
+        input=input
+        ))
+
+    return result[f"bulkReplaceRelations_{prefixed_escaped_trait_id}_{escaped_traitrelation_id}"]["success"]
   
-def _bulk_replace_trait_entities_by_filter(ok_api_client: okc.OkApiClient, trait_id: str, input: List[Dict[str,Any]], id_attributes: [str], id_relations: [str], write_layer: str, read_layers: [str] = None, filter: object = {}) -> bool:
+def _bulk_replace_trait_entities_by_filter(ok_api_client: okc.OkApiClient, trait_id: str, input: List[Dict[str,Any]], id_attributes: List[str], id_relations: List[str], write_layer: str, read_layers: List[str] = None, filter: object = {}) -> bool:
     """
     Internal method used to replace all traitentites in a layer, it can use a filter when updating the trait entities,
     this will also delete all old trait entities, if there are any
 
     Parameters
     ----------
     ok_api_client : OkApiClient
@@ -397,15 +456,15 @@
         idRelations=id_relations,
         filter=filter,
         input=input
         ))
 
     return result[f"bulkReplaceByFilter_{prefixed_escaped_trait_id}"]["success"]
 
-def _bulk_replace_trait_entities(ok_api_client: okc.OkApiClient, trait_id: str, input: List[Dict[str,Any]], write_layer: str, read_layers: [str] = None) -> bool:
+def _bulk_replace_trait_entities(ok_api_client: okc.OkApiClient, trait_id: str, input: List[Dict[str,Any]], write_layer: str, read_layers: List[str] = None) -> bool:
     """
     Internal method that sets all trait entities, this will also delete all old trait entities, if there are any
 
     Parameters
     ----------
     ok_api_client : OkApiClient
         The OkApiClient instance representing omnikeeper connection
@@ -453,15 +512,15 @@
         readLayers=read_layers, 
         input=final_input
         ))
 
     return result[f"bulkReplace_{prefixed_escaped_trait_id}"]["success"]
 
 # TODO: support use of uuid.UUID for ciids
-def bulk_replace_trait_entities_by_filter(ok_api_client: okc.OkApiClient, trait_id: str, input: List[Dict[str,Any]], id_attributes: [str], id_relations: [str], write_layer: str, read_layers: [str] = None, filter: object = {}) -> bool:
+def bulk_replace_trait_entities_by_filter(ok_api_client: okc.OkApiClient, trait_id: str, input: List[Dict[str,Any]], id_attributes: List[str], id_relations: List[str], write_layer: str, read_layers: List[str] = None, filter: object = {}) -> bool:
     """
     Replaces all traitentites in a layer, it can use a filter when updating the trait entities,
     this will also delete all old trait entities, if there are any
 
     Parameters
     ----------
     ok_api_client : OkApiClient
@@ -495,15 +554,15 @@
     bool 
         True if the update is successful, False otherwise
     """
     result = _bulk_replace_trait_entities_by_filter(ok_api_client, trait_id, input, id_attributes, id_relations, write_layer, read_layers, filter)
     return result
 
 # TODO: support use of uuid.UUID for ciids
-def bulk_replace_trait_entities(ok_api_client: okc.OkApiClient, trait_id: str, input: List[Dict[str,Any]], write_layer: str, read_layers: [str] = None) -> bool:
+def bulk_replace_trait_entities(ok_api_client: okc.OkApiClient, trait_id: str, input: List[Dict[str,Any]], write_layer: str, read_layers: List[str] = None) -> bool:
     """
     Sets all trait entities, this will also delete all old trait entities, if there are any
 
     Parameters
     ----------
     ok_api_client : OkApiClient
         The OkApiClient instance representing omnikeeper connection
```

## Comparing `omnikeeper_client-5.1.1.dist-info/LICENSE` & `omnikeeper_client-5.2.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `omnikeeper_client-5.1.1.dist-info/METADATA` & `omnikeeper_client-5.2.0.dist-info/METADATA`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: omnikeeper-client
-Version: 5.1.1
+Version: 5.2.0
 Summary: Python library containing helper functions for implementing omnikeeper clients
 Home-page: UNKNOWN
 Author: Maximilian Csuk
 License: Apache 2.0
 Platform: UNKNOWN
 License-File: LICENSE
 Requires-Dist: appengine-python-standard ~=1.1
 Requires-Dist: gql ~=3.4
 Requires-Dist: oauthlib ~=3.2
 Requires-Dist: pandas >=2.0
+Requires-Dist: pydantic ~=2.6
 Requires-Dist: python-json-logger ~=2.0
 Requires-Dist: requests-oauthlib ~=1.3
 Requires-Dist: requests-toolbelt ~=0.10
 Requires-Dist: webcolors ~=1.3
 
 UNKNOWN
```

