# Comparing `tmp/cell-annotation-schema-0.2b0.tar.gz` & `tmp/cell-annotation-schema-0.3b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cell-annotation-schema-0.2b0.tar", last modified: Thu Jan  4 13:38:30 2024, max compression
+gzip compressed data, was "cell-annotation-schema-0.3b0.tar", last modified: Tue May  7 22:16:06 2024, max compression
```

## Comparing `cell-annotation-schema-0.2b0.tar` & `cell-annotation-schema-0.3b0.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxr-xr-x   0 hk9        (503) staff       (20)        0 2024-01-04 13:38:30.960177 cell-annotation-schema-0.2b0/
--rw-r--r--   0 hk9        (503) staff       (20)     1862 2024-01-02 15:18:39.000000 cell-annotation-schema-0.2b0/BICAN_extension.json
--rw-r--r--   0 hk9        (503) staff       (20)    12782 2024-01-04 13:36:56.000000 cell-annotation-schema-0.2b0/BICAN_schema.json
--rw-r--r--   0 hk9        (503) staff       (20)     1755 2024-01-02 15:18:39.000000 cell-annotation-schema-0.2b0/CAP_extension.json
--rw-r--r--   0 hk9        (503) staff       (20)    12701 2024-01-04 13:36:56.000000 cell-annotation-schema-0.2b0/CAP_schema.json
--rw-r--r--   0 hk9        (503) staff       (20)      123 2024-01-02 15:18:39.000000 cell-annotation-schema-0.2b0/MANIFEST.in
--rw-r--r--   0 hk9        (503) staff       (20)     3906 2024-01-04 13:38:30.959949 cell-annotation-schema-0.2b0/PKG-INFO
--rw-r--r--   0 hk9        (503) staff       (20)     3490 2024-01-02 15:18:39.000000 cell-annotation-schema-0.2b0/README.md
--rw-r--r--   0 hk9        (503) staff       (20)    11110 2024-01-02 15:18:39.000000 cell-annotation-schema-0.2b0/general_schema.json
--rw-r--r--   0 hk9        (503) staff       (20)       38 2024-01-04 13:38:30.960237 cell-annotation-schema-0.2b0/setup.cfg
--rw-r--r--   0 hk9        (503) staff       (20)     1005 2024-01-04 13:36:25.000000 cell-annotation-schema-0.2b0/setup.py
-drwxr-xr-x   0 hk9        (503) staff       (20)        0 2024-01-04 13:38:30.952647 cell-annotation-schema-0.2b0/src/
-drwxr-xr-x   0 hk9        (503) staff       (20)        0 2024-01-04 13:38:30.956492 cell-annotation-schema-0.2b0/src/cas_schema/
--rw-r--r--   0 hk9        (503) staff       (20)        0 2024-01-02 15:18:39.000000 cell-annotation-schema-0.2b0/src/cas_schema/__init__.py
--rw-r--r--   0 hk9        (503) staff       (20)      123 2024-01-02 15:18:39.000000 cell-annotation-schema-0.2b0/src/cas_schema/catalog.yaml
--rw-r--r--   0 hk9        (503) staff       (20)     4163 2024-01-02 15:18:39.000000 cell-annotation-schema-0.2b0/src/cas_schema/json_utils.py
--rw-r--r--   0 hk9        (503) staff       (20)     2611 2024-01-02 15:18:39.000000 cell-annotation-schema-0.2b0/src/cas_schema/schema_manager.py
--rw-r--r--   0 hk9        (503) staff       (20)     1789 2024-01-02 15:18:39.000000 cell-annotation-schema-0.2b0/src/cas_schema/schema_merger.py
--rw-r--r--   0 hk9        (503) staff       (20)     5199 2024-01-02 15:18:39.000000 cell-annotation-schema-0.2b0/src/cas_schema/schema_validator.py
-drwxr-xr-x   0 hk9        (503) staff       (20)        0 2024-01-04 13:38:30.957365 cell-annotation-schema-0.2b0/src/cas_schema/schemas/
--rw-r--r--   0 hk9        (503) staff       (20)    12782 2024-01-04 13:37:08.000000 cell-annotation-schema-0.2b0/src/cas_schema/schemas/BICAN_schema.json
--rw-r--r--   0 hk9        (503) staff       (20)    12701 2024-01-04 13:37:08.000000 cell-annotation-schema-0.2b0/src/cas_schema/schemas/CAP_schema.json
--rw-r--r--   0 hk9        (503) staff       (20)        0 2024-01-04 13:37:08.000000 cell-annotation-schema-0.2b0/src/cas_schema/schemas/__init__.py
--rw-r--r--   0 hk9        (503) staff       (20)    11110 2024-01-04 13:37:08.000000 cell-annotation-schema-0.2b0/src/cas_schema/schemas/general_schema.json
-drwxr-xr-x   0 hk9        (503) staff       (20)        0 2024-01-04 13:38:30.959591 cell-annotation-schema-0.2b0/src/cell_annotation_schema.egg-info/
--rw-r--r--   0 hk9        (503) staff       (20)     3906 2024-01-04 13:38:30.000000 cell-annotation-schema-0.2b0/src/cell_annotation_schema.egg-info/PKG-INFO
--rw-r--r--   0 hk9        (503) staff       (20)      715 2024-01-04 13:38:30.000000 cell-annotation-schema-0.2b0/src/cell_annotation_schema.egg-info/SOURCES.txt
--rw-r--r--   0 hk9        (503) staff       (20)        1 2024-01-04 13:38:30.000000 cell-annotation-schema-0.2b0/src/cell_annotation_schema.egg-info/dependency_links.txt
--rw-r--r--   0 hk9        (503) staff       (20)       66 2024-01-04 13:38:30.000000 cell-annotation-schema-0.2b0/src/cell_annotation_schema.egg-info/requires.txt
--rw-r--r--   0 hk9        (503) staff       (20)       11 2024-01-04 13:38:30.000000 cell-annotation-schema-0.2b0/src/cell_annotation_schema.egg-info/top_level.txt
+drwxr-xr-x   0 hk9        (503) staff       (20)        0 2024-05-07 22:16:06.573437 cell-annotation-schema-0.3b0/
+-rw-r--r--   0 hk9        (503) staff       (20)     1833 2024-05-07 22:04:32.000000 cell-annotation-schema-0.3b0/BICAN_extension.json
+-rw-r--r--   0 hk9        (503) staff       (20)    13645 2024-05-07 22:13:35.000000 cell-annotation-schema-0.3b0/BICAN_schema.json
+-rw-r--r--   0 hk9        (503) staff       (20)     2346 2024-05-07 22:04:32.000000 cell-annotation-schema-0.3b0/CAP_extension.json
+-rw-r--r--   0 hk9        (503) staff       (20)    14163 2024-05-07 22:13:35.000000 cell-annotation-schema-0.3b0/CAP_schema.json
+-rw-r--r--   0 hk9        (503) staff       (20)      123 2024-05-07 22:04:32.000000 cell-annotation-schema-0.3b0/MANIFEST.in
+-rw-r--r--   0 hk9        (503) staff       (20)     4946 2024-05-07 22:16:06.573175 cell-annotation-schema-0.3b0/PKG-INFO
+-rw-r--r--   0 hk9        (503) staff       (20)     4404 2024-05-07 22:04:32.000000 cell-annotation-schema-0.3b0/README.md
+-rw-r--r--   0 hk9        (503) staff       (20)    12002 2024-05-07 22:04:32.000000 cell-annotation-schema-0.3b0/general_schema.json
+-rw-r--r--   0 hk9        (503) staff       (20)       38 2024-05-07 22:16:06.573484 cell-annotation-schema-0.3b0/setup.cfg
+-rw-r--r--   0 hk9        (503) staff       (20)     1005 2024-05-07 22:15:06.000000 cell-annotation-schema-0.3b0/setup.py
+drwxr-xr-x   0 hk9        (503) staff       (20)        0 2024-05-07 22:16:06.567081 cell-annotation-schema-0.3b0/src/
+drwxr-xr-x   0 hk9        (503) staff       (20)        0 2024-05-07 22:16:06.570841 cell-annotation-schema-0.3b0/src/cas_schema/
+-rw-r--r--   0 hk9        (503) staff       (20)        0 2024-05-07 22:04:32.000000 cell-annotation-schema-0.3b0/src/cas_schema/__init__.py
+-rw-r--r--   0 hk9        (503) staff       (20)      123 2024-05-07 22:04:32.000000 cell-annotation-schema-0.3b0/src/cas_schema/catalog.yaml
+-rw-r--r--   0 hk9        (503) staff       (20)     4163 2024-05-07 22:04:32.000000 cell-annotation-schema-0.3b0/src/cas_schema/json_utils.py
+-rw-r--r--   0 hk9        (503) staff       (20)    13274 2024-05-07 22:04:32.000000 cell-annotation-schema-0.3b0/src/cas_schema/schema_docs.py
+-rw-r--r--   0 hk9        (503) staff       (20)     2611 2024-05-07 22:04:32.000000 cell-annotation-schema-0.3b0/src/cas_schema/schema_manager.py
+-rw-r--r--   0 hk9        (503) staff       (20)     1789 2024-05-07 22:04:32.000000 cell-annotation-schema-0.3b0/src/cas_schema/schema_merger.py
+-rw-r--r--   0 hk9        (503) staff       (20)     5199 2024-05-07 22:04:32.000000 cell-annotation-schema-0.3b0/src/cas_schema/schema_validator.py
+drwxr-xr-x   0 hk9        (503) staff       (20)        0 2024-05-07 22:16:06.571785 cell-annotation-schema-0.3b0/src/cas_schema/schemas/
+-rw-r--r--   0 hk9        (503) staff       (20)    13645 2024-05-07 22:14:37.000000 cell-annotation-schema-0.3b0/src/cas_schema/schemas/BICAN_schema.json
+-rw-r--r--   0 hk9        (503) staff       (20)    14163 2024-05-07 22:14:37.000000 cell-annotation-schema-0.3b0/src/cas_schema/schemas/CAP_schema.json
+-rw-r--r--   0 hk9        (503) staff       (20)        0 2024-05-07 22:14:00.000000 cell-annotation-schema-0.3b0/src/cas_schema/schemas/__init__.py
+-rw-r--r--   0 hk9        (503) staff       (20)    12002 2024-05-07 22:14:37.000000 cell-annotation-schema-0.3b0/src/cas_schema/schemas/general_schema.json
+drwxr-xr-x   0 hk9        (503) staff       (20)        0 2024-05-07 22:16:06.572871 cell-annotation-schema-0.3b0/src/cell_annotation_schema.egg-info/
+-rw-r--r--   0 hk9        (503) staff       (20)     4946 2024-05-07 22:16:06.000000 cell-annotation-schema-0.3b0/src/cell_annotation_schema.egg-info/PKG-INFO
+-rw-r--r--   0 hk9        (503) staff       (20)      745 2024-05-07 22:16:06.000000 cell-annotation-schema-0.3b0/src/cell_annotation_schema.egg-info/SOURCES.txt
+-rw-r--r--   0 hk9        (503) staff       (20)        1 2024-05-07 22:16:06.000000 cell-annotation-schema-0.3b0/src/cell_annotation_schema.egg-info/dependency_links.txt
+-rw-r--r--   0 hk9        (503) staff       (20)       66 2024-05-07 22:16:06.000000 cell-annotation-schema-0.3b0/src/cell_annotation_schema.egg-info/requires.txt
+-rw-r--r--   0 hk9        (503) staff       (20)       11 2024-05-07 22:16:06.000000 cell-annotation-schema-0.3b0/src/cell_annotation_schema.egg-info/top_level.txt
```

### Comparing `cell-annotation-schema-0.2b0/BICAN_extension.json` & `cell-annotation-schema-0.3b0/BICAN_extension.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9895833333333334%*

 * *Differences: {"'definitions'": "{'Annotation': {'properties': {'parent_cell_set_accession': "*

 * *                  "OrderedDict([('type', 'string'), ('description', 'A list of accessions of cell "*

 * *                  'sets that subsume this cell set. This can be used to compose hierarchies of '*

 * *                  "annotated cell sets, built from a fixed set of clusters.')]), delete: "*

 * *                  "['parent_cell_set_accessions']}}}"}*

```diff
@@ -7,18 +7,17 @@
     "definitions": {
         "Annotation": {
             "properties": {
                 "cell_set_accession": {
                     "description": "An identifier that can be used to consistently refer to the set of cells being annotated, even if the cell_label changes.",
                     "type": "string"
                 },
-                "parent_cell_set_accessions": {
+                "parent_cell_set_accession": {
                     "description": "A list of accessions of cell sets that subsume this cell set. This can be used to compose hierarchies of annotated cell sets, built from a fixed set of clusters.",
-                    "type": "array",
-                    "value": "string"
+                    "type": "string"
                 },
                 "transferred_annotations": {
                     "items": {
                         "$ref": "#/definitions/Annotation_transfer"
                     },
                     "type": "array"
                 }
```

### Comparing `cell-annotation-schema-0.2b0/BICAN_schema.json` & `cell-annotation-schema-0.3b0/BICAN_schema.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9889480744949495%*

 * *Differences: {"'definitions'": "{'Annotation': {'properties': {'marker_gene_evidence': {'description': 'List of "*

 * *                  'names of genes whose expression in the cells being annotated is explicitly used '*

 * *                  'as evidence for this cell annotation. Each gene MUST be included in the matrix '*

 * *                  "of the AnnData/Seurat file.'}, 'negative_marker_gene_evidence': "*

 * *                  "OrderedDict([('description', 'List of names of genes, the absence of expression "*

 * *                  'of wh […]*

```diff
@@ -33,25 +33,32 @@
                     "type": "string"
                 },
                 "labelset": {
                     "description": "The unique name of the set of cell annotations. \nEach cell within the AnnData/Seurat file MUST be associated with a 'cell_label' value in order for this to be a valid 'cellannotation_setname'.",
                     "type": "string"
                 },
                 "marker_gene_evidence": {
-                    "description": "List of gene names explicitly used as evidence for this cell annotation. Each gene MUST be included in the matrix of the AnnData/Seurat file.",
+                    "description": "List of names of genes whose expression in the cells being annotated is explicitly used as evidence for this cell annotation. Each gene MUST be included in the matrix of the AnnData/Seurat file.",
                     "items": {
                         "description": "Gene names explicitly used as evidence, which MUST be in the matrix of the AnnData/Seurat file",
                         "type": "string"
                     },
                     "type": "array"
                 },
-                "parent_cell_set_accessions": {
+                "negative_marker_gene_evidence": {
+                    "description": "List of names of genes, the absence of expression of which is explicitly used as evidence for this cell annotation. Each gene MUST be included in the matrix of the AnnData/Seurat file.",
+                    "items": {
+                        "description": "Gene names explicitly used as evidence, which MUST be in the matrix of the AnnData/Seurat file",
+                        "type": "string"
+                    },
+                    "type": "array"
+                },
+                "parent_cell_set_accession": {
                     "description": "A list of accessions of cell sets that subsume this cell set. This can be used to compose hierarchies of annotated cell sets, built from a fixed set of clusters.",
-                    "type": "array",
-                    "value": "string"
+                    "type": "string"
                 },
                 "rationale": {
                     "description": "The free-text rationale which users provide as justification/evidence for their cell annotations. \nResearchers are encouraged to use this field to cite relevant publications in-line using standard academic citations of the form `(Zheng et al., 2020)` This human-readable free-text MUST be encoded as a single string.\nAll references cited SHOULD be listed using DOIs under rationale_dois. There MUST be a 2000-character limit.",
                     "maxLength": 2000,
                     "type": "string"
                 },
                 "rationale_dois": {
@@ -172,20 +179,24 @@
         "annotations": {
             "items": {
                 "$ref": "#/definitions/Annotation"
             },
             "type": "array"
         },
         "author_contact": {
-            "description": "This MUST be a valid email address of the author",
+            "description": "Primary author's contact. This MUST be a valid email address of the author",
             "format": "email",
             "type": "string"
         },
+        "author_list": {
+            "description": "This field stores a list of users who are included in the project as collaborators, regardless of their specific role. An example list; '['John Smith', 'Cody Miller', 'Sarah Jones']'",
+            "type": "string"
+        },
         "author_name": {
-            "description": "This MUST be a string in the format `[FIRST NAME] [LAST NAME]`",
+            "description": "Primary author's name. This MUST be a string in the format `[FIRST NAME] [LAST NAME]`",
             "type": "string"
         },
         "cellannotation_schema_version": {
             "description": "The schema version, the cell annotation open standard. Current version MUST follow 0.1.0\nThis versioning MUST follow the format `'[MAJOR].[MINOR].[PATCH]'` as defined by Semantic Versioning 2.0.0, https://semver.org/",
             "type": "string"
         },
         "cellannotation_timestamp": {
@@ -198,23 +209,25 @@
             "type": "string"
         },
         "cellannotation_version": {
             "description": "The version for all cell annotations published (per dataset). This MUST be a string. The recommended versioning format is `'[MAJOR].[MINOR].[PATCH]'` as defined by Semantic Versioning 2.0.0, https://semver.org/",
             "type": "string"
         },
         "labelsets": {
-            "$ref": "#/definitions/Labelset",
+            "items": {
+                "$ref": "#/definitions/Labelset"
+            },
             "type": "array"
         },
         "matrix_file_id": {
             "description": "A resolvable ID for a cell by gene matrix file in the form namespace:accession, e.g. CellXGene_dataset:8e10f1c4-8e98-41e5-b65f-8cd89a887122.  Please see https://github.com/cellannotation/cell-annotation-schema/registry/registry.json for supported namespaces.",
             "type": "string"
         },
         "orcid": {
-            "description": "This MUST be a valid ORCID for the author",
+            "description": "Primary author's orcid. This MUST be a valid ORCID for the author",
             "type": "string"
         }
     },
     "required": [
         "author_name",
         "annotations",
         "labelsets"
```

### Comparing `cell-annotation-schema-0.2b0/CAP_schema.json` & `cell-annotation-schema-0.3b0/general_schema.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.947856863705078%*

 * *Differences: {"'definitions'": "{'Annotation': {'properties': {'marker_gene_evidence': {'description': 'List of "*

 * *                  'names of genes whose expression in the cells being annotated is explicitly used '*

 * *                  'as evidence for this cell annotation. Each gene MUST be included in the matrix '*

 * *                  "of the AnnData/Seurat file.'}, 'negative_marker_gene_evidence': "*

 * *                  "OrderedDict([('description', 'List of names of genes, the absence of expression "*

 * *                  'of wh […]*

```diff
@@ -1,29 +1,13 @@
 {
     "$schema": "http://json-schema.org/draft-07/schema#",
     "definitions": {
         "Annotation": {
             "description": "A collection of fields recording a cell type/class/state annotation on some set os cells, supporting evidence and provenance. As this is intended as a general schema, compulsory fields are kept to a minimum. However, tools using this schema are encouarged to specify a larger set of compulsory fields for publication. \n\nNote: This schema deliberately allows for additional fields in order to support ad hoc user fields, new formal schema extensions and project/tool specific metadata.",
             "properties": {
-                "category_cell_ontology_exists": {
-                    "description": "Decision by user whether this biological entity exists in the current Cell Ontology or not (at the given time of publication). If True, then the user MUST specify this Cell Ontology entry in the fields category_cell_ontology_term_id and category_cell_ontology_term.",
-                    "type": "boolean"
-                },
-                "category_cell_ontology_term": {
-                    "description": "This MUST be the human-readable name assigned to the value of 'category_cell_ontology_term_id'",
-                    "type": "string"
-                },
-                "category_cell_ontology_term_id": {
-                    "description": "This MUST be a term from either the Cell Ontology (https://www.ebi.ac.uk/ols/ontologies/cl) or from some ontology that extends it by classifying cell types under terms from the Cell Ontology e.g. the Provisional Cell Ontology (https://www.ebi.ac.uk/ols/ontologies/pcl) or the Drosophila Anatomy Ontology (DAO) (https://www.ebi.ac.uk/ols4/ontologies/fbbt).  This field MUST be filled if `category_cell_ontology_exists` is True.",
-                    "type": "string"
-                },
-                "category_fullname": {
-                    "description": "Any term denoting a biological entity which the author associates as the nearest \"class\" or 'broader term' (or \"parent term\") for the value/term in the field. This field MAY be 'NA' if the author cannot associate any term to the value.",
-                    "type": "string"
-                },
                 "cell_fullname": {
                     "description": "This MUST be the full-length name for the biological entity listed in `cell_label` by the author. (If the value in `cell_label` is the full-length term, this field will contain the same value.) \nNOTE: any reserved word used in the field 'cell_label' MUST match the value of this field. \n\nEXAMPLE 1: Given the matching terms 'LC' and 'luminal cell' used to annotate the same cell(s), then users could use either terms as values in the field 'cell_label'. However, the abbreviation 'LC' CANNOT be provided in the field 'cell_fullname'. \n\nEXAMPLE 2: Either the abbreviation 'AC' or the full-length term intended by the author 'GABAergic amacrine cell' MAY be placed in the field 'cell_label', but as full-length term naming this biological entity, 'GABAergic amacrine cell' MUST be placed in the field 'cell_fullname'.",
                     "type": "string"
                 },
                 "cell_ids": {
                     "description": "List of cell barcode sequences/UUIDs used to uniquely identify the cells within the AnnData/Seurat matrix. Any and all cell barcode sequences/UUIDs MUST be included in the AnnData/Seurat matrix.",
                     "items": {
@@ -45,15 +29,23 @@
                     "type": "string"
                 },
                 "labelset": {
                     "description": "The unique name of the set of cell annotations. \nEach cell within the AnnData/Seurat file MUST be associated with a 'cell_label' value in order for this to be a valid 'cellannotation_setname'.",
                     "type": "string"
                 },
                 "marker_gene_evidence": {
-                    "description": "List of gene names explicitly used as evidence for this cell annotation. Each gene MUST be included in the matrix of the AnnData/Seurat file.",
+                    "description": "List of names of genes whose expression in the cells being annotated is explicitly used as evidence for this cell annotation. Each gene MUST be included in the matrix of the AnnData/Seurat file.",
+                    "items": {
+                        "description": "Gene names explicitly used as evidence, which MUST be in the matrix of the AnnData/Seurat file",
+                        "type": "string"
+                    },
+                    "type": "array"
+                },
+                "negative_marker_gene_evidence": {
+                    "description": "List of names of genes, the absence of expression of which is explicitly used as evidence for this cell annotation. Each gene MUST be included in the matrix of the AnnData/Seurat file.",
                     "items": {
                         "description": "Gene names explicitly used as evidence, which MUST be in the matrix of the AnnData/Seurat file",
                         "type": "string"
                     },
                     "type": "array"
                 },
                 "rationale": {
@@ -145,20 +137,24 @@
         "annotations": {
             "items": {
                 "$ref": "#/definitions/Annotation"
             },
             "type": "array"
         },
         "author_contact": {
-            "description": "This MUST be a valid email address of the author",
+            "description": "Primary author's contact. This MUST be a valid email address of the author",
             "format": "email",
             "type": "string"
         },
+        "author_list": {
+            "description": "This field stores a list of users who are included in the project as collaborators, regardless of their specific role. An example list; '['John Smith', 'Cody Miller', 'Sarah Jones']'",
+            "type": "string"
+        },
         "author_name": {
-            "description": "This MUST be a string in the format `[FIRST NAME] [LAST NAME]`",
+            "description": "Primary author's name. This MUST be a string in the format `[FIRST NAME] [LAST NAME]`",
             "type": "string"
         },
         "cellannotation_schema_version": {
             "description": "The schema version, the cell annotation open standard. Current version MUST follow 0.1.0\nThis versioning MUST follow the format `'[MAJOR].[MINOR].[PATCH]'` as defined by Semantic Versioning 2.0.0, https://semver.org/",
             "type": "string"
         },
         "cellannotation_timestamp": {
@@ -171,31 +167,29 @@
             "type": "string"
         },
         "cellannotation_version": {
             "description": "The version for all cell annotations published (per dataset). This MUST be a string. The recommended versioning format is `'[MAJOR].[MINOR].[PATCH]'` as defined by Semantic Versioning 2.0.0, https://semver.org/",
             "type": "string"
         },
         "labelsets": {
-            "$ref": "#/definitions/Labelset",
+            "items": {
+                "$ref": "#/definitions/Labelset"
+            },
             "type": "array"
         },
         "matrix_file_id": {
             "description": "A resolvable ID for a cell by gene matrix file in the form namespace:accession, e.g. CellXGene_dataset:8e10f1c4-8e98-41e5-b65f-8cd89a887122.  Please see https://github.com/cellannotation/cell-annotation-schema/registry/registry.json for supported namespaces.",
             "type": "string"
         },
         "orcid": {
-            "description": "This MUST be a valid ORCID for the author",
+            "description": "Primary author's orcid. This MUST be a valid ORCID for the author",
             "type": "string"
         }
     },
     "required": [
         "author_name",
         "annotations",
-        "labelsets",
-        "cellannotation_schema_version",
-        "cellannotation_timestamp",
-        "cellannotation_version",
-        "cellannotation_url"
+        "labelsets"
     ],
     "title": "General Cell Annotation Open Standard",
     "type": "object"
 }
```

### Comparing `cell-annotation-schema-0.2b0/PKG-INFO` & `cell-annotation-schema-0.3b0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,63 +1,61 @@
-Metadata-Version: 2.1
-Name: cell-annotation-schema
-Version: 0.2b0
-Summary: Cell Annotation Schema
-Home-page: https://github.com/cellannotation/cell-annotation-schema
-Author: 
-License: Apache-2.0 license
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-
 ![Schema Validation](https://github.com/cellannotation/cell-annotation-schema/actions/workflows/schema_validator.yaml/badge.svg?branch=main)
 # cell-annotation-schema
 
-General, open-standard schema for cell annotations
+A general, open-standard schema for cell annotations and related metadata.
+
+This effort is part of [scFAIR](https://sc-fair.org/), an initiative to standardize single-cell genomics metadata.
 
 ## Motivation
 
-Annotation of single cell transcriptomics data with cell types/classes is inherently variable. The reasons that authors choose to annotate a set of cells with a particular label are not typically represented in annotated data and there is no established standard for doing so.  For relatively simple datasets it may be possible to reconstruct this information by reading an associated publication, but as single cell transcriptomics datasets and accompanying publications become increasingly complex, doing so is becoming increasingly difficult and in many cases publications lack the necessary detail.
+Annotation of single cell transcriptomics data with cell types/classes is inherently variable. The reasons authors choose to annotate a set of cells with a particular label are not typically represented in annotated data and there is no established standard for doing so.  For relatively simple datasets it may be possible to reconstruct this information by reading an associated publication, but as single cell transcriptomics datasets and accompanying publications become increasingly complex, doing so is becoming increasingly difficult and in many cases publications lack the necessary detail.
 
 CAS provides a programmatically accessible standard designed to solve this problem by allowing users to record additional metadata about individual cell type annotations, including marker genes used as evidence and details of automated annotation transfer.  The standard is represented as JSON schema as this allows all metadata to be gathered in a single, compact validatable file - which includes a link to a cell by gene matrix file of annotated data. However, the schema is designed so that it can be decomposed into individual tables suitable for use in dataframes/TSVs and flattened onto obs in AnnData format.
 
 ## User stories: 
 
-https://github.com/cellannotation/cell-annotation-schema/blob/main/user_stories.md
+https://github.com/cellannotation/cell-annotation-schema/blob/main/docs/user_stories.md
 
 ## Examples
 
 Examples used in testing can be browsed under: https://github.com/cellannotation/cell-annotation-schema/tree/main/examples
 
+brain-bican contains a growing set of working taxonomies including: 
+
+- https://github.com/brain-bican/human-brain-cell-atlas_v1_neurons
 
 ## Overview
 
-The top level of the JSON is used to store metadata about the annotations it contains: Author details; links to the annotated matrix file, version information etc.  This can be thought of as a table the links to a set of subtables.
+The top level of the JSON is used to store metadata about the annotations: Author details; links to the annotated matrix file, version information etc.  This can be thought of as a table that links to a set of subtables.
 
 The top level wraps other JSON objects (sub-tables):
 
 1. A list of annotation objects (a table of annotations). Each annotation belongs to a named `labelset`
 2. A table of labelsets - recording names, and additional metadata including a description and provenance (manual vs automated) and if automated, details of automated annotation algorithms etc.
 
 ## Core schema vs extensions
 
 We define a core schema with a very limited set of compulsory fields.  The core schema avoids specifying that additional fields are forbidden, allowing extensions to be built and for any users to add their own customs fields as long as they don't stomp on existing fields in the specification. 
 
+Documentation for the core and extension schemas is available at:
+
+- [general_schema.md](https://github.com/cellannotation/cell-annotation-schema/blob/main/build/general_schema.md); Derived from [general_schema.json](https://github.com/cellannotation/cell-annotation-schema/blob/main/general_schema.json)
+- [BICAN_schema.md](https://github.com/cellannotation/cell-annotation-schema/blob/main/build/BICAN_schema.md); Derived from [BICAN_schema.json](https://github.com/cellannotation/cell-annotation-schema/blob/main/build/BICAN_schema.json)
+- [CAP_schema.md](https://github.com/cellannotation/cell-annotation-schema/blob/main/build/CAP_schema.md); Derived from [CAP_schema.json](https://github.com/cellannotation/cell-annotation-schema/blob/main/build/CAP_schema.json)
+
+This repo also contains the [CAP AnnData Specification](https://github.com/cellannotation/cell-annotation-schema/blob/main/docs/cap_anndata_schema.md). Warning - PROVISIONAL - We are working to fully align this with the CAP extension.
+
+
 ## Releases
 
 We publish both versioned releases and a nightly snapshot at https://github.com/cellannotation/cell-annotation-schema/releases
 
 Release assets include a core schema file and extensions (currently for BICAN and the Cell Annotation Platform).
 
 PyPI release is at https://pypi.org/project/cell-annotation-schema/
 
-You can discover instructions on utilizing the PyPI package by visiting the following link https://github.com/cellannotation/cell-annotation-schema/blob/main/docs/pypi_package.md
+You can discover instructions on utilizing the PyPI package by visiting the following link https://github.com/cellannotation/cell-annotation-schema/blob/main/docs/pypi_package.md.
+
 
-## Contents
-- General standard for annotating cell sets (JSON Schema)
-- General standard - JSON Schema rendered in Markdown  - WARNING - MAY BE OUT OF DATE - DERIVATION NOT CURRENTLY AUTOMATED
-- Specification of flattening to AnnData. -  WARNING - MAY BE OUT OF DATE - DERIVATION NOT CURRENTLY AUTOMATED
-- Extensions for BICAN and the Cell Annotation Platform.
```

### Comparing `cell-annotation-schema-0.2b0/README.md` & `cell-annotation-schema-0.3b0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,51 +1,77 @@
+Metadata-Version: 2.1
+Name: cell-annotation-schema
+Version: 0.3b0
+Summary: Cell Annotation Schema
+Home-page: https://github.com/cellannotation/cell-annotation-schema
+Author: 
+License: Apache-2.0 license
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+Requires-Dist: jsonschema==4.4.0
+Requires-Dist: ordered-set==4.1.0
+Requires-Dist: deepmerge==1.1.0
+Requires-Dist: ruamel.yaml
+
 ![Schema Validation](https://github.com/cellannotation/cell-annotation-schema/actions/workflows/schema_validator.yaml/badge.svg?branch=main)
 # cell-annotation-schema
 
-General, open-standard schema for cell annotations
+A general, open-standard schema for cell annotations and related metadata.
+
+This effort is part of [scFAIR](https://sc-fair.org/), an initiative to standardize single-cell genomics metadata.
 
 ## Motivation
 
-Annotation of single cell transcriptomics data with cell types/classes is inherently variable. The reasons that authors choose to annotate a set of cells with a particular label are not typically represented in annotated data and there is no established standard for doing so.  For relatively simple datasets it may be possible to reconstruct this information by reading an associated publication, but as single cell transcriptomics datasets and accompanying publications become increasingly complex, doing so is becoming increasingly difficult and in many cases publications lack the necessary detail.
+Annotation of single cell transcriptomics data with cell types/classes is inherently variable. The reasons authors choose to annotate a set of cells with a particular label are not typically represented in annotated data and there is no established standard for doing so.  For relatively simple datasets it may be possible to reconstruct this information by reading an associated publication, but as single cell transcriptomics datasets and accompanying publications become increasingly complex, doing so is becoming increasingly difficult and in many cases publications lack the necessary detail.
 
 CAS provides a programmatically accessible standard designed to solve this problem by allowing users to record additional metadata about individual cell type annotations, including marker genes used as evidence and details of automated annotation transfer.  The standard is represented as JSON schema as this allows all metadata to be gathered in a single, compact validatable file - which includes a link to a cell by gene matrix file of annotated data. However, the schema is designed so that it can be decomposed into individual tables suitable for use in dataframes/TSVs and flattened onto obs in AnnData format.
 
 ## User stories: 
 
-https://github.com/cellannotation/cell-annotation-schema/blob/main/user_stories.md
+https://github.com/cellannotation/cell-annotation-schema/blob/main/docs/user_stories.md
 
 ## Examples
 
 Examples used in testing can be browsed under: https://github.com/cellannotation/cell-annotation-schema/tree/main/examples
 
+brain-bican contains a growing set of working taxonomies including: 
+
+- https://github.com/brain-bican/human-brain-cell-atlas_v1_neurons
 
 ## Overview
 
-The top level of the JSON is used to store metadata about the annotations it contains: Author details; links to the annotated matrix file, version information etc.  This can be thought of as a table the links to a set of subtables.
+The top level of the JSON is used to store metadata about the annotations: Author details; links to the annotated matrix file, version information etc.  This can be thought of as a table that links to a set of subtables.
 
 The top level wraps other JSON objects (sub-tables):
 
 1. A list of annotation objects (a table of annotations). Each annotation belongs to a named `labelset`
 2. A table of labelsets - recording names, and additional metadata including a description and provenance (manual vs automated) and if automated, details of automated annotation algorithms etc.
 
 ## Core schema vs extensions
 
 We define a core schema with a very limited set of compulsory fields.  The core schema avoids specifying that additional fields are forbidden, allowing extensions to be built and for any users to add their own customs fields as long as they don't stomp on existing fields in the specification. 
 
+Documentation for the core and extension schemas is available at:
+
+- [general_schema.md](https://github.com/cellannotation/cell-annotation-schema/blob/main/build/general_schema.md); Derived from [general_schema.json](https://github.com/cellannotation/cell-annotation-schema/blob/main/general_schema.json)
+- [BICAN_schema.md](https://github.com/cellannotation/cell-annotation-schema/blob/main/build/BICAN_schema.md); Derived from [BICAN_schema.json](https://github.com/cellannotation/cell-annotation-schema/blob/main/build/BICAN_schema.json)
+- [CAP_schema.md](https://github.com/cellannotation/cell-annotation-schema/blob/main/build/CAP_schema.md); Derived from [CAP_schema.json](https://github.com/cellannotation/cell-annotation-schema/blob/main/build/CAP_schema.json)
+
+This repo also contains the [CAP AnnData Specification](https://github.com/cellannotation/cell-annotation-schema/blob/main/docs/cap_anndata_schema.md). Warning - PROVISIONAL - We are working to fully align this with the CAP extension.
+
+
 ## Releases
 
 We publish both versioned releases and a nightly snapshot at https://github.com/cellannotation/cell-annotation-schema/releases
 
 Release assets include a core schema file and extensions (currently for BICAN and the Cell Annotation Platform).
 
 PyPI release is at https://pypi.org/project/cell-annotation-schema/
 
-You can discover instructions on utilizing the PyPI package by visiting the following link https://github.com/cellannotation/cell-annotation-schema/blob/main/docs/pypi_package.md
+You can discover instructions on utilizing the PyPI package by visiting the following link https://github.com/cellannotation/cell-annotation-schema/blob/main/docs/pypi_package.md.
+
 
-## Contents
-- General standard for annotating cell sets (JSON Schema)
-- General standard - JSON Schema rendered in Markdown  - WARNING - MAY BE OUT OF DATE - DERIVATION NOT CURRENTLY AUTOMATED
-- Specification of flattening to AnnData. -  WARNING - MAY BE OUT OF DATE - DERIVATION NOT CURRENTLY AUTOMATED
-- Extensions for BICAN and the Cell Annotation Platform.
```

### Comparing `cell-annotation-schema-0.2b0/general_schema.json` & `cell-annotation-schema-0.3b0/src/cas_schema/schemas/general_schema.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9890309343434343%*

 * *Differences: {"'definitions'": "{'Annotation': {'properties': {'marker_gene_evidence': {'description': 'List of "*

 * *                  'names of genes whose expression in the cells being annotated is explicitly used '*

 * *                  'as evidence for this cell annotation. Each gene MUST be included in the matrix '*

 * *                  "of the AnnData/Seurat file.'}, 'negative_marker_gene_evidence': "*

 * *                  "OrderedDict([('description', 'List of names of genes, the absence of expression "*

 * *                  'of wh […]*

```diff
@@ -29,15 +29,23 @@
                     "type": "string"
                 },
                 "labelset": {
                     "description": "The unique name of the set of cell annotations. \nEach cell within the AnnData/Seurat file MUST be associated with a 'cell_label' value in order for this to be a valid 'cellannotation_setname'.",
                     "type": "string"
                 },
                 "marker_gene_evidence": {
-                    "description": "List of gene names explicitly used as evidence for this cell annotation. Each gene MUST be included in the matrix of the AnnData/Seurat file.",
+                    "description": "List of names of genes whose expression in the cells being annotated is explicitly used as evidence for this cell annotation. Each gene MUST be included in the matrix of the AnnData/Seurat file.",
+                    "items": {
+                        "description": "Gene names explicitly used as evidence, which MUST be in the matrix of the AnnData/Seurat file",
+                        "type": "string"
+                    },
+                    "type": "array"
+                },
+                "negative_marker_gene_evidence": {
+                    "description": "List of names of genes, the absence of expression of which is explicitly used as evidence for this cell annotation. Each gene MUST be included in the matrix of the AnnData/Seurat file.",
                     "items": {
                         "description": "Gene names explicitly used as evidence, which MUST be in the matrix of the AnnData/Seurat file",
                         "type": "string"
                     },
                     "type": "array"
                 },
                 "rationale": {
@@ -129,20 +137,24 @@
         "annotations": {
             "items": {
                 "$ref": "#/definitions/Annotation"
             },
             "type": "array"
         },
         "author_contact": {
-            "description": "This MUST be a valid email address of the author",
+            "description": "Primary author's contact. This MUST be a valid email address of the author",
             "format": "email",
             "type": "string"
         },
+        "author_list": {
+            "description": "This field stores a list of users who are included in the project as collaborators, regardless of their specific role. An example list; '['John Smith', 'Cody Miller', 'Sarah Jones']'",
+            "type": "string"
+        },
         "author_name": {
-            "description": "This MUST be a string in the format `[FIRST NAME] [LAST NAME]`",
+            "description": "Primary author's name. This MUST be a string in the format `[FIRST NAME] [LAST NAME]`",
             "type": "string"
         },
         "cellannotation_schema_version": {
             "description": "The schema version, the cell annotation open standard. Current version MUST follow 0.1.0\nThis versioning MUST follow the format `'[MAJOR].[MINOR].[PATCH]'` as defined by Semantic Versioning 2.0.0, https://semver.org/",
             "type": "string"
         },
         "cellannotation_timestamp": {
@@ -155,23 +167,25 @@
             "type": "string"
         },
         "cellannotation_version": {
             "description": "The version for all cell annotations published (per dataset). This MUST be a string. The recommended versioning format is `'[MAJOR].[MINOR].[PATCH]'` as defined by Semantic Versioning 2.0.0, https://semver.org/",
             "type": "string"
         },
         "labelsets": {
-            "$ref": "#/definitions/Labelset",
+            "items": {
+                "$ref": "#/definitions/Labelset"
+            },
             "type": "array"
         },
         "matrix_file_id": {
             "description": "A resolvable ID for a cell by gene matrix file in the form namespace:accession, e.g. CellXGene_dataset:8e10f1c4-8e98-41e5-b65f-8cd89a887122.  Please see https://github.com/cellannotation/cell-annotation-schema/registry/registry.json for supported namespaces.",
             "type": "string"
         },
         "orcid": {
-            "description": "This MUST be a valid ORCID for the author",
+            "description": "Primary author's orcid. This MUST be a valid ORCID for the author",
             "type": "string"
         }
     },
     "required": [
         "author_name",
         "annotations",
         "labelsets"
```

### Comparing `cell-annotation-schema-0.2b0/setup.py` & `cell-annotation-schema-0.3b0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # The directory containing this file
 HERE = pathlib.Path(__file__).parent
 README = (HERE / "README.md").read_text()
 
 setup(
     name="cell-annotation-schema",
     # version="__version__",
-    version=" v0.2beta",
+    version="v0.3-beta",
     description="Cell Annotation Schema",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/cellannotation/cell-annotation-schema",
     author="",
     license="Apache-2.0 license",
     classifiers=[
```

### Comparing `cell-annotation-schema-0.2b0/src/cas_schema/json_utils.py` & `cell-annotation-schema-0.3b0/src/cas_schema/json_utils.py`

 * *Files identical despite different names*

### Comparing `cell-annotation-schema-0.2b0/src/cas_schema/schema_manager.py` & `cell-annotation-schema-0.3b0/src/cas_schema/schema_manager.py`

 * *Files identical despite different names*

### Comparing `cell-annotation-schema-0.2b0/src/cas_schema/schema_merger.py` & `cell-annotation-schema-0.3b0/src/cas_schema/schema_merger.py`

 * *Files identical despite different names*

### Comparing `cell-annotation-schema-0.2b0/src/cas_schema/schema_validator.py` & `cell-annotation-schema-0.3b0/src/cas_schema/schema_validator.py`

 * *Files identical despite different names*

### Comparing `cell-annotation-schema-0.2b0/src/cas_schema/schemas/BICAN_schema.json` & `cell-annotation-schema-0.3b0/src/cas_schema/schemas/BICAN_schema.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9889480744949495%*

 * *Differences: {"'definitions'": "{'Annotation': {'properties': {'marker_gene_evidence': {'description': 'List of "*

 * *                  'names of genes whose expression in the cells being annotated is explicitly used '*

 * *                  'as evidence for this cell annotation. Each gene MUST be included in the matrix '*

 * *                  "of the AnnData/Seurat file.'}, 'negative_marker_gene_evidence': "*

 * *                  "OrderedDict([('description', 'List of names of genes, the absence of expression "*

 * *                  'of wh […]*

```diff
@@ -33,25 +33,32 @@
                     "type": "string"
                 },
                 "labelset": {
                     "description": "The unique name of the set of cell annotations. \nEach cell within the AnnData/Seurat file MUST be associated with a 'cell_label' value in order for this to be a valid 'cellannotation_setname'.",
                     "type": "string"
                 },
                 "marker_gene_evidence": {
-                    "description": "List of gene names explicitly used as evidence for this cell annotation. Each gene MUST be included in the matrix of the AnnData/Seurat file.",
+                    "description": "List of names of genes whose expression in the cells being annotated is explicitly used as evidence for this cell annotation. Each gene MUST be included in the matrix of the AnnData/Seurat file.",
                     "items": {
                         "description": "Gene names explicitly used as evidence, which MUST be in the matrix of the AnnData/Seurat file",
                         "type": "string"
                     },
                     "type": "array"
                 },
-                "parent_cell_set_accessions": {
+                "negative_marker_gene_evidence": {
+                    "description": "List of names of genes, the absence of expression of which is explicitly used as evidence for this cell annotation. Each gene MUST be included in the matrix of the AnnData/Seurat file.",
+                    "items": {
+                        "description": "Gene names explicitly used as evidence, which MUST be in the matrix of the AnnData/Seurat file",
+                        "type": "string"
+                    },
+                    "type": "array"
+                },
+                "parent_cell_set_accession": {
                     "description": "A list of accessions of cell sets that subsume this cell set. This can be used to compose hierarchies of annotated cell sets, built from a fixed set of clusters.",
-                    "type": "array",
-                    "value": "string"
+                    "type": "string"
                 },
                 "rationale": {
                     "description": "The free-text rationale which users provide as justification/evidence for their cell annotations. \nResearchers are encouraged to use this field to cite relevant publications in-line using standard academic citations of the form `(Zheng et al., 2020)` This human-readable free-text MUST be encoded as a single string.\nAll references cited SHOULD be listed using DOIs under rationale_dois. There MUST be a 2000-character limit.",
                     "maxLength": 2000,
                     "type": "string"
                 },
                 "rationale_dois": {
@@ -172,20 +179,24 @@
         "annotations": {
             "items": {
                 "$ref": "#/definitions/Annotation"
             },
             "type": "array"
         },
         "author_contact": {
-            "description": "This MUST be a valid email address of the author",
+            "description": "Primary author's contact. This MUST be a valid email address of the author",
             "format": "email",
             "type": "string"
         },
+        "author_list": {
+            "description": "This field stores a list of users who are included in the project as collaborators, regardless of their specific role. An example list; '['John Smith', 'Cody Miller', 'Sarah Jones']'",
+            "type": "string"
+        },
         "author_name": {
-            "description": "This MUST be a string in the format `[FIRST NAME] [LAST NAME]`",
+            "description": "Primary author's name. This MUST be a string in the format `[FIRST NAME] [LAST NAME]`",
             "type": "string"
         },
         "cellannotation_schema_version": {
             "description": "The schema version, the cell annotation open standard. Current version MUST follow 0.1.0\nThis versioning MUST follow the format `'[MAJOR].[MINOR].[PATCH]'` as defined by Semantic Versioning 2.0.0, https://semver.org/",
             "type": "string"
         },
         "cellannotation_timestamp": {
@@ -198,23 +209,25 @@
             "type": "string"
         },
         "cellannotation_version": {
             "description": "The version for all cell annotations published (per dataset). This MUST be a string. The recommended versioning format is `'[MAJOR].[MINOR].[PATCH]'` as defined by Semantic Versioning 2.0.0, https://semver.org/",
             "type": "string"
         },
         "labelsets": {
-            "$ref": "#/definitions/Labelset",
+            "items": {
+                "$ref": "#/definitions/Labelset"
+            },
             "type": "array"
         },
         "matrix_file_id": {
             "description": "A resolvable ID for a cell by gene matrix file in the form namespace:accession, e.g. CellXGene_dataset:8e10f1c4-8e98-41e5-b65f-8cd89a887122.  Please see https://github.com/cellannotation/cell-annotation-schema/registry/registry.json for supported namespaces.",
             "type": "string"
         },
         "orcid": {
-            "description": "This MUST be a valid ORCID for the author",
+            "description": "Primary author's orcid. This MUST be a valid ORCID for the author",
             "type": "string"
         }
     },
     "required": [
         "author_name",
         "annotations",
         "labelsets"
```

### Comparing `cell-annotation-schema-0.2b0/src/cas_schema/schemas/CAP_schema.json` & `cell-annotation-schema-0.3b0/CAP_schema.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9696723090277778%*

 * *Differences: {"'definitions'": "{'Annotation': {'properties': {'marker_gene_evidence': {'description': 'List of "*

 * *                  'names of genes whose expression in the cells being annotated is explicitly used '*

 * *                  'as evidence for this cell annotation. Each gene MUST be included in the matrix '*

 * *                  "of the AnnData/Seurat file.'}, 'negative_marker_gene_evidence': "*

 * *                  "OrderedDict([('description', 'List of names of genes, the absence of expression "*

 * *                  'of wh […]*

```diff
@@ -1,28 +1,20 @@
 {
     "$schema": "http://json-schema.org/draft-07/schema#",
     "definitions": {
         "Annotation": {
             "description": "A collection of fields recording a cell type/class/state annotation on some set os cells, supporting evidence and provenance. As this is intended as a general schema, compulsory fields are kept to a minimum. However, tools using this schema are encouarged to specify a larger set of compulsory fields for publication. \n\nNote: This schema deliberately allows for additional fields in order to support ad hoc user fields, new formal schema extensions and project/tool specific metadata.",
             "properties": {
-                "category_cell_ontology_exists": {
-                    "description": "Decision by user whether this biological entity exists in the current Cell Ontology or not (at the given time of publication). If True, then the user MUST specify this Cell Ontology entry in the fields category_cell_ontology_term_id and category_cell_ontology_term.",
-                    "type": "boolean"
-                },
-                "category_cell_ontology_term": {
-                    "description": "This MUST be the human-readable name assigned to the value of 'category_cell_ontology_term_id'",
-                    "type": "string"
-                },
-                "category_cell_ontology_term_id": {
-                    "description": "This MUST be a term from either the Cell Ontology (https://www.ebi.ac.uk/ols/ontologies/cl) or from some ontology that extends it by classifying cell types under terms from the Cell Ontology e.g. the Provisional Cell Ontology (https://www.ebi.ac.uk/ols/ontologies/pcl) or the Drosophila Anatomy Ontology (DAO) (https://www.ebi.ac.uk/ols4/ontologies/fbbt).  This field MUST be filled if `category_cell_ontology_exists` is True.",
-                    "type": "string"
-                },
-                "category_fullname": {
-                    "description": "Any term denoting a biological entity which the author associates as the nearest \"class\" or 'broader term' (or \"parent term\") for the value/term in the field. This field MAY be 'NA' if the author cannot associate any term to the value.",
-                    "type": "string"
+                "canonical_marker_genes": {
+                    "description": "A list of gene names considered to be canonical markers for the biological entity used in the cell annotation.",
+                    "items": {
+                        "description": "A gene name recognized as a key marker for the entity's classification.",
+                        "type": "string"
+                    },
+                    "type": "array"
                 },
                 "cell_fullname": {
                     "description": "This MUST be the full-length name for the biological entity listed in `cell_label` by the author. (If the value in `cell_label` is the full-length term, this field will contain the same value.) \nNOTE: any reserved word used in the field 'cell_label' MUST match the value of this field. \n\nEXAMPLE 1: Given the matching terms 'LC' and 'luminal cell' used to annotate the same cell(s), then users could use either terms as values in the field 'cell_label'. However, the abbreviation 'LC' CANNOT be provided in the field 'cell_fullname'. \n\nEXAMPLE 2: Either the abbreviation 'AC' or the full-length term intended by the author 'GABAergic amacrine cell' MAY be placed in the field 'cell_label', but as full-length term naming this biological entity, 'GABAergic amacrine cell' MUST be placed in the field 'cell_fullname'.",
                     "type": "string"
                 },
                 "cell_ids": {
                     "description": "List of cell barcode sequences/UUIDs used to uniquely identify the cells within the AnnData/Seurat matrix. Any and all cell barcode sequences/UUIDs MUST be included in the AnnData/Seurat matrix.",
@@ -45,15 +37,23 @@
                     "type": "string"
                 },
                 "labelset": {
                     "description": "The unique name of the set of cell annotations. \nEach cell within the AnnData/Seurat file MUST be associated with a 'cell_label' value in order for this to be a valid 'cellannotation_setname'.",
                     "type": "string"
                 },
                 "marker_gene_evidence": {
-                    "description": "List of gene names explicitly used as evidence for this cell annotation. Each gene MUST be included in the matrix of the AnnData/Seurat file.",
+                    "description": "List of names of genes whose expression in the cells being annotated is explicitly used as evidence for this cell annotation. Each gene MUST be included in the matrix of the AnnData/Seurat file.",
+                    "items": {
+                        "description": "Gene names explicitly used as evidence, which MUST be in the matrix of the AnnData/Seurat file",
+                        "type": "string"
+                    },
+                    "type": "array"
+                },
+                "negative_marker_gene_evidence": {
+                    "description": "List of names of genes, the absence of expression of which is explicitly used as evidence for this cell annotation. Each gene MUST be included in the matrix of the AnnData/Seurat file.",
                     "items": {
                         "description": "Gene names explicitly used as evidence, which MUST be in the matrix of the AnnData/Seurat file",
                         "type": "string"
                     },
                     "type": "array"
                 },
                 "rationale": {
@@ -145,20 +145,36 @@
         "annotations": {
             "items": {
                 "$ref": "#/definitions/Annotation"
             },
             "type": "array"
         },
         "author_contact": {
-            "description": "This MUST be a valid email address of the author",
+            "description": "Primary author's contact. This MUST be a valid email address of the author",
             "format": "email",
             "type": "string"
         },
+        "author_list": {
+            "description": "This field stores a list of users who are included in the project as collaborators, regardless of their specific role. An example list; '['John Smith', 'Cody Miller', 'Sarah Jones']'",
+            "type": "string"
+        },
         "author_name": {
-            "description": "This MUST be a string in the format `[FIRST NAME] [LAST NAME]`",
+            "description": "Primary author's name. This MUST be a string in the format `[FIRST NAME] [LAST NAME]`",
+            "type": "string"
+        },
+        "cap_publication_description": {
+            "description": "The description of the publication on CAP. The description of the publication on CAP. (NOTE: the term \"publication\" refers to the workspace published on CAP with a version and timestamp.) This MUST be less than or equal to N characters, and this MUST be encoded as a single string.",
+            "type": "string"
+        },
+        "cap_publication_title": {
+            "description": "The title of the publication on CAP (i.e. a published collection of datasets, the \"CAP Workspace\".). The title of the publication on CAP. (NOTE: the term \"publication\" refers to the workspace published on CAP with a version and timestamp.) This MUST be less than or equal to N characters, and this MUST be encoded as a single string.",
+            "type": "string"
+        },
+        "cap_publication_url": {
+            "description": "A persistent URL of the publication on CAP. (NOTE: the term \"publication\" refers to the workspace published on CAP with a version and timestamp.)",
             "type": "string"
         },
         "cellannotation_schema_version": {
             "description": "The schema version, the cell annotation open standard. Current version MUST follow 0.1.0\nThis versioning MUST follow the format `'[MAJOR].[MINOR].[PATCH]'` as defined by Semantic Versioning 2.0.0, https://semver.org/",
             "type": "string"
         },
         "cellannotation_timestamp": {
@@ -171,23 +187,33 @@
             "type": "string"
         },
         "cellannotation_version": {
             "description": "The version for all cell annotations published (per dataset). This MUST be a string. The recommended versioning format is `'[MAJOR].[MINOR].[PATCH]'` as defined by Semantic Versioning 2.0.0, https://semver.org/",
             "type": "string"
         },
         "labelsets": {
-            "$ref": "#/definitions/Labelset",
+            "items": {
+                "$ref": "#/definitions/Labelset"
+            },
             "type": "array"
         },
         "matrix_file_id": {
             "description": "A resolvable ID for a cell by gene matrix file in the form namespace:accession, e.g. CellXGene_dataset:8e10f1c4-8e98-41e5-b65f-8cd89a887122.  Please see https://github.com/cellannotation/cell-annotation-schema/registry/registry.json for supported namespaces.",
             "type": "string"
         },
         "orcid": {
-            "description": "This MUST be a valid ORCID for the author",
+            "description": "Primary author's orcid. This MUST be a valid ORCID for the author",
+            "type": "string"
+        },
+        "publication_timestamp": {
+            "description": "The timestamp of the CAP publication. This MUST be a string in the format %yyyy-%MM-%dd'T'%hh:%mm:%ss. This value will be overwritten by the newest timestamp upon a new publication.",
+            "type": "string"
+        },
+        "publication_version": {
+            "description": "The (latest) version of the CAP publication. This value will be overwritten by the newest version upon a new publication (and automatically incremented). This versioning MUST follow the format 'v' + '[integer]', whereby newer versions must be naturally incremented.",
             "type": "string"
         }
     },
     "required": [
         "author_name",
         "annotations",
         "labelsets",
```

### Comparing `cell-annotation-schema-0.2b0/src/cas_schema/schemas/general_schema.json` & `cell-annotation-schema-0.3b0/src/cas_schema/schemas/CAP_schema.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9291634188397582%*

 * *Differences: {"'definitions'": "{'Annotation': {'properties': {'marker_gene_evidence': {'description': 'List of "*

 * *                  'names of genes whose expression in the cells being annotated is explicitly used '*

 * *                  'as evidence for this cell annotation. Each gene MUST be included in the matrix '*

 * *                  "of the AnnData/Seurat file.'}, 'negative_marker_gene_evidence': "*

 * *                  "OrderedDict([('description', 'List of names of genes, the absence of expression "*

 * *                  'of wh […]*

```diff
@@ -1,13 +1,21 @@
 {
     "$schema": "http://json-schema.org/draft-07/schema#",
     "definitions": {
         "Annotation": {
             "description": "A collection of fields recording a cell type/class/state annotation on some set os cells, supporting evidence and provenance. As this is intended as a general schema, compulsory fields are kept to a minimum. However, tools using this schema are encouarged to specify a larger set of compulsory fields for publication. \n\nNote: This schema deliberately allows for additional fields in order to support ad hoc user fields, new formal schema extensions and project/tool specific metadata.",
             "properties": {
+                "canonical_marker_genes": {
+                    "description": "A list of gene names considered to be canonical markers for the biological entity used in the cell annotation.",
+                    "items": {
+                        "description": "A gene name recognized as a key marker for the entity's classification.",
+                        "type": "string"
+                    },
+                    "type": "array"
+                },
                 "cell_fullname": {
                     "description": "This MUST be the full-length name for the biological entity listed in `cell_label` by the author. (If the value in `cell_label` is the full-length term, this field will contain the same value.) \nNOTE: any reserved word used in the field 'cell_label' MUST match the value of this field. \n\nEXAMPLE 1: Given the matching terms 'LC' and 'luminal cell' used to annotate the same cell(s), then users could use either terms as values in the field 'cell_label'. However, the abbreviation 'LC' CANNOT be provided in the field 'cell_fullname'. \n\nEXAMPLE 2: Either the abbreviation 'AC' or the full-length term intended by the author 'GABAergic amacrine cell' MAY be placed in the field 'cell_label', but as full-length term naming this biological entity, 'GABAergic amacrine cell' MUST be placed in the field 'cell_fullname'.",
                     "type": "string"
                 },
                 "cell_ids": {
                     "description": "List of cell barcode sequences/UUIDs used to uniquely identify the cells within the AnnData/Seurat matrix. Any and all cell barcode sequences/UUIDs MUST be included in the AnnData/Seurat matrix.",
                     "items": {
@@ -29,15 +37,23 @@
                     "type": "string"
                 },
                 "labelset": {
                     "description": "The unique name of the set of cell annotations. \nEach cell within the AnnData/Seurat file MUST be associated with a 'cell_label' value in order for this to be a valid 'cellannotation_setname'.",
                     "type": "string"
                 },
                 "marker_gene_evidence": {
-                    "description": "List of gene names explicitly used as evidence for this cell annotation. Each gene MUST be included in the matrix of the AnnData/Seurat file.",
+                    "description": "List of names of genes whose expression in the cells being annotated is explicitly used as evidence for this cell annotation. Each gene MUST be included in the matrix of the AnnData/Seurat file.",
+                    "items": {
+                        "description": "Gene names explicitly used as evidence, which MUST be in the matrix of the AnnData/Seurat file",
+                        "type": "string"
+                    },
+                    "type": "array"
+                },
+                "negative_marker_gene_evidence": {
+                    "description": "List of names of genes, the absence of expression of which is explicitly used as evidence for this cell annotation. Each gene MUST be included in the matrix of the AnnData/Seurat file.",
                     "items": {
                         "description": "Gene names explicitly used as evidence, which MUST be in the matrix of the AnnData/Seurat file",
                         "type": "string"
                     },
                     "type": "array"
                 },
                 "rationale": {
@@ -129,20 +145,36 @@
         "annotations": {
             "items": {
                 "$ref": "#/definitions/Annotation"
             },
             "type": "array"
         },
         "author_contact": {
-            "description": "This MUST be a valid email address of the author",
+            "description": "Primary author's contact. This MUST be a valid email address of the author",
             "format": "email",
             "type": "string"
         },
+        "author_list": {
+            "description": "This field stores a list of users who are included in the project as collaborators, regardless of their specific role. An example list; '['John Smith', 'Cody Miller', 'Sarah Jones']'",
+            "type": "string"
+        },
         "author_name": {
-            "description": "This MUST be a string in the format `[FIRST NAME] [LAST NAME]`",
+            "description": "Primary author's name. This MUST be a string in the format `[FIRST NAME] [LAST NAME]`",
+            "type": "string"
+        },
+        "cap_publication_description": {
+            "description": "The description of the publication on CAP. The description of the publication on CAP. (NOTE: the term \"publication\" refers to the workspace published on CAP with a version and timestamp.) This MUST be less than or equal to N characters, and this MUST be encoded as a single string.",
+            "type": "string"
+        },
+        "cap_publication_title": {
+            "description": "The title of the publication on CAP (i.e. a published collection of datasets, the \"CAP Workspace\".). The title of the publication on CAP. (NOTE: the term \"publication\" refers to the workspace published on CAP with a version and timestamp.) This MUST be less than or equal to N characters, and this MUST be encoded as a single string.",
+            "type": "string"
+        },
+        "cap_publication_url": {
+            "description": "A persistent URL of the publication on CAP. (NOTE: the term \"publication\" refers to the workspace published on CAP with a version and timestamp.)",
             "type": "string"
         },
         "cellannotation_schema_version": {
             "description": "The schema version, the cell annotation open standard. Current version MUST follow 0.1.0\nThis versioning MUST follow the format `'[MAJOR].[MINOR].[PATCH]'` as defined by Semantic Versioning 2.0.0, https://semver.org/",
             "type": "string"
         },
         "cellannotation_timestamp": {
@@ -155,27 +187,41 @@
             "type": "string"
         },
         "cellannotation_version": {
             "description": "The version for all cell annotations published (per dataset). This MUST be a string. The recommended versioning format is `'[MAJOR].[MINOR].[PATCH]'` as defined by Semantic Versioning 2.0.0, https://semver.org/",
             "type": "string"
         },
         "labelsets": {
-            "$ref": "#/definitions/Labelset",
+            "items": {
+                "$ref": "#/definitions/Labelset"
+            },
             "type": "array"
         },
         "matrix_file_id": {
             "description": "A resolvable ID for a cell by gene matrix file in the form namespace:accession, e.g. CellXGene_dataset:8e10f1c4-8e98-41e5-b65f-8cd89a887122.  Please see https://github.com/cellannotation/cell-annotation-schema/registry/registry.json for supported namespaces.",
             "type": "string"
         },
         "orcid": {
-            "description": "This MUST be a valid ORCID for the author",
+            "description": "Primary author's orcid. This MUST be a valid ORCID for the author",
+            "type": "string"
+        },
+        "publication_timestamp": {
+            "description": "The timestamp of the CAP publication. This MUST be a string in the format %yyyy-%MM-%dd'T'%hh:%mm:%ss. This value will be overwritten by the newest timestamp upon a new publication.",
+            "type": "string"
+        },
+        "publication_version": {
+            "description": "The (latest) version of the CAP publication. This value will be overwritten by the newest version upon a new publication (and automatically incremented). This versioning MUST follow the format 'v' + '[integer]', whereby newer versions must be naturally incremented.",
             "type": "string"
         }
     },
     "required": [
         "author_name",
         "annotations",
-        "labelsets"
+        "labelsets",
+        "cellannotation_schema_version",
+        "cellannotation_timestamp",
+        "cellannotation_version",
+        "cellannotation_url"
     ],
     "title": "General Cell Annotation Open Standard",
     "type": "object"
 }
```

### Comparing `cell-annotation-schema-0.2b0/src/cell_annotation_schema.egg-info/PKG-INFO` & `cell-annotation-schema-0.3b0/src/cell_annotation_schema.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,63 +1,77 @@
 Metadata-Version: 2.1
 Name: cell-annotation-schema
-Version: 0.2b0
+Version: 0.3b0
 Summary: Cell Annotation Schema
 Home-page: https://github.com/cellannotation/cell-annotation-schema
 Author: 
 License: Apache-2.0 license
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+Requires-Dist: jsonschema==4.4.0
+Requires-Dist: ordered-set==4.1.0
+Requires-Dist: deepmerge==1.1.0
+Requires-Dist: ruamel.yaml
 
 ![Schema Validation](https://github.com/cellannotation/cell-annotation-schema/actions/workflows/schema_validator.yaml/badge.svg?branch=main)
 # cell-annotation-schema
 
-General, open-standard schema for cell annotations
+A general, open-standard schema for cell annotations and related metadata.
+
+This effort is part of [scFAIR](https://sc-fair.org/), an initiative to standardize single-cell genomics metadata.
 
 ## Motivation
 
-Annotation of single cell transcriptomics data with cell types/classes is inherently variable. The reasons that authors choose to annotate a set of cells with a particular label are not typically represented in annotated data and there is no established standard for doing so.  For relatively simple datasets it may be possible to reconstruct this information by reading an associated publication, but as single cell transcriptomics datasets and accompanying publications become increasingly complex, doing so is becoming increasingly difficult and in many cases publications lack the necessary detail.
+Annotation of single cell transcriptomics data with cell types/classes is inherently variable. The reasons authors choose to annotate a set of cells with a particular label are not typically represented in annotated data and there is no established standard for doing so.  For relatively simple datasets it may be possible to reconstruct this information by reading an associated publication, but as single cell transcriptomics datasets and accompanying publications become increasingly complex, doing so is becoming increasingly difficult and in many cases publications lack the necessary detail.
 
 CAS provides a programmatically accessible standard designed to solve this problem by allowing users to record additional metadata about individual cell type annotations, including marker genes used as evidence and details of automated annotation transfer.  The standard is represented as JSON schema as this allows all metadata to be gathered in a single, compact validatable file - which includes a link to a cell by gene matrix file of annotated data. However, the schema is designed so that it can be decomposed into individual tables suitable for use in dataframes/TSVs and flattened onto obs in AnnData format.
 
 ## User stories: 
 
-https://github.com/cellannotation/cell-annotation-schema/blob/main/user_stories.md
+https://github.com/cellannotation/cell-annotation-schema/blob/main/docs/user_stories.md
 
 ## Examples
 
 Examples used in testing can be browsed under: https://github.com/cellannotation/cell-annotation-schema/tree/main/examples
 
+brain-bican contains a growing set of working taxonomies including: 
+
+- https://github.com/brain-bican/human-brain-cell-atlas_v1_neurons
 
 ## Overview
 
-The top level of the JSON is used to store metadata about the annotations it contains: Author details; links to the annotated matrix file, version information etc.  This can be thought of as a table the links to a set of subtables.
+The top level of the JSON is used to store metadata about the annotations: Author details; links to the annotated matrix file, version information etc.  This can be thought of as a table that links to a set of subtables.
 
 The top level wraps other JSON objects (sub-tables):
 
 1. A list of annotation objects (a table of annotations). Each annotation belongs to a named `labelset`
 2. A table of labelsets - recording names, and additional metadata including a description and provenance (manual vs automated) and if automated, details of automated annotation algorithms etc.
 
 ## Core schema vs extensions
 
 We define a core schema with a very limited set of compulsory fields.  The core schema avoids specifying that additional fields are forbidden, allowing extensions to be built and for any users to add their own customs fields as long as they don't stomp on existing fields in the specification. 
 
+Documentation for the core and extension schemas is available at:
+
+- [general_schema.md](https://github.com/cellannotation/cell-annotation-schema/blob/main/build/general_schema.md); Derived from [general_schema.json](https://github.com/cellannotation/cell-annotation-schema/blob/main/general_schema.json)
+- [BICAN_schema.md](https://github.com/cellannotation/cell-annotation-schema/blob/main/build/BICAN_schema.md); Derived from [BICAN_schema.json](https://github.com/cellannotation/cell-annotation-schema/blob/main/build/BICAN_schema.json)
+- [CAP_schema.md](https://github.com/cellannotation/cell-annotation-schema/blob/main/build/CAP_schema.md); Derived from [CAP_schema.json](https://github.com/cellannotation/cell-annotation-schema/blob/main/build/CAP_schema.json)
+
+This repo also contains the [CAP AnnData Specification](https://github.com/cellannotation/cell-annotation-schema/blob/main/docs/cap_anndata_schema.md). Warning - PROVISIONAL - We are working to fully align this with the CAP extension.
+
+
 ## Releases
 
 We publish both versioned releases and a nightly snapshot at https://github.com/cellannotation/cell-annotation-schema/releases
 
 Release assets include a core schema file and extensions (currently for BICAN and the Cell Annotation Platform).
 
 PyPI release is at https://pypi.org/project/cell-annotation-schema/
 
-You can discover instructions on utilizing the PyPI package by visiting the following link https://github.com/cellannotation/cell-annotation-schema/blob/main/docs/pypi_package.md
+You can discover instructions on utilizing the PyPI package by visiting the following link https://github.com/cellannotation/cell-annotation-schema/blob/main/docs/pypi_package.md.
+
 
-## Contents
-- General standard for annotating cell sets (JSON Schema)
-- General standard - JSON Schema rendered in Markdown  - WARNING - MAY BE OUT OF DATE - DERIVATION NOT CURRENTLY AUTOMATED
-- Specification of flattening to AnnData. -  WARNING - MAY BE OUT OF DATE - DERIVATION NOT CURRENTLY AUTOMATED
-- Extensions for BICAN and the Cell Annotation Platform.
```

### Comparing `cell-annotation-schema-0.2b0/src/cell_annotation_schema.egg-info/SOURCES.txt` & `cell-annotation-schema-0.3b0/src/cell_annotation_schema.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 MANIFEST.in
 README.md
 general_schema.json
 setup.py
 src/cas_schema/__init__.py
 src/cas_schema/catalog.yaml
 src/cas_schema/json_utils.py
+src/cas_schema/schema_docs.py
 src/cas_schema/schema_manager.py
 src/cas_schema/schema_merger.py
 src/cas_schema/schema_validator.py
 src/cas_schema/schemas/BICAN_schema.json
 src/cas_schema/schemas/CAP_schema.json
 src/cas_schema/schemas/__init__.py
 src/cas_schema/schemas/general_schema.json
```

