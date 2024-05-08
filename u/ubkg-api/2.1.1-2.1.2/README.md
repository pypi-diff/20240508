# Comparing `tmp/ubkg_api-2.1.1.tar.gz` & `tmp/ubkg_api-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ubkg_api-2.1.1.tar", last modified: Fri Apr 12 19:14:51 2024, max compression
+gzip compressed data, was "ubkg_api-2.1.2.tar", last modified: Wed May  8 15:11:07 2024, max compression
```

## Comparing `ubkg_api-2.1.1.tar` & `ubkg_api-2.1.2.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2024-04-12 19:14:51.550804 ubkg_api-2.1.1/
--rw-r--r--   0 ZHY19      (503) staff       (20)     1087 2024-04-12 19:00:53.000000 ubkg_api-2.1.1/LICENSE
--rw-r--r--   0 ZHY19      (503) staff       (20)    12051 2024-04-12 19:14:51.550354 ubkg_api-2.1.1/PKG-INFO
--rw-r--r--   0 ZHY19      (503) staff       (20)    11349 2024-04-12 19:00:53.000000 ubkg_api-2.1.1/README.md
--rw-r--r--   0 ZHY19      (503) staff       (20)      762 2024-04-12 19:01:18.000000 ubkg_api-2.1.1/pyproject.toml
--rw-r--r--   0 ZHY19      (503) staff       (20)       38 2024-04-12 19:14:51.550848 ubkg_api-2.1.1/setup.cfg
-drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2024-04-12 19:14:51.432263 ubkg_api-2.1.1/src/
--rw-r--r--   0 ZHY19      (503) staff       (20)        0 2024-04-12 19:00:53.000000 ubkg_api-2.1.1/src/__init__.py
-drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2024-04-12 19:14:51.440153 ubkg_api-2.1.1/src/ubkg_api/
--rw-r--r--   0 ZHY19      (503) staff       (20)        0 2024-04-12 19:00:53.000000 ubkg_api-2.1.1/src/ubkg_api/__init__.py
--rw-r--r--   0 ZHY19      (503) staff       (20)     5556 2024-04-12 19:00:53.000000 ubkg_api-2.1.1/src/ubkg_api/app.py
-drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2024-04-12 19:14:51.452606 ubkg_api-2.1.1/src/ubkg_api/common_routes/
--rw-r--r--   0 ZHY19      (503) staff       (20)        0 2024-04-12 19:00:53.000000 ubkg_api-2.1.1/src/ubkg_api/common_routes/__init__.py
-drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2024-04-12 19:14:51.456377 ubkg_api-2.1.1/src/ubkg_api/common_routes/codes/
--rw-r--r--   0 ZHY19      (503) staff       (20)        0 2024-04-12 19:00:53.000000 ubkg_api-2.1.1/src/ubkg_api/common_routes/codes/__init__.py
--rw-r--r--   0 ZHY19      (503) staff       (20)     2280 2024-04-12 19:00:53.000000 ubkg_api-2.1.1/src/ubkg_api/common_routes/codes/codes_controller.py
--rw-r--r--   0 ZHY19      (503) staff       (20)    39519 2024-04-12 19:00:53.000000 ubkg_api-2.1.1/src/ubkg_api/common_routes/common_neo4j_logic.py
-drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2024-04-12 19:14:51.459728 ubkg_api-2.1.1/src/ubkg_api/common_routes/concepts/
--rw-r--r--   0 ZHY19      (503) staff       (20)        0 2024-04-12 19:00:53.000000 ubkg_api-2.1.1/src/ubkg_api/common_routes/concepts/__init__.py
--rw-r--r--   0 ZHY19      (503) staff       (20)    17929 2024-04-12 19:00:53.000000 ubkg_api-2.1.1/src/ubkg_api/common_routes/concepts/concepts_controller.py
-drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2024-04-12 19:14:51.462044 ubkg_api-2.1.1/src/ubkg_api/common_routes/database/
--rw-r--r--   0 ZHY19      (503) staff       (20)        0 2024-04-12 19:00:53.000000 ubkg_api-2.1.1/src/ubkg_api/common_routes/database/__init__.py
--rw-r--r--   0 ZHY19      (503) staff       (20)      479 2024-04-12 19:00:53.000000 ubkg_api-2.1.1/src/ubkg_api/common_routes/database/database_controller.py
-drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2024-04-12 19:14:51.462442 ubkg_api-2.1.1/src/ubkg_api/common_routes/deprecated/
--rw-r--r--   0 ZHY19      (503) staff       (20)        0 2024-04-12 19:00:53.000000 ubkg_api-2.1.1/src/ubkg_api/common_routes/deprecated/__init__.py
-drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2024-04-12 19:14:51.464546 ubkg_api-2.1.1/src/ubkg_api/common_routes/deprecated/tui/
--rw-r--r--   0 ZHY19      (503) staff       (20)        0 2024-04-12 19:00:53.000000 ubkg_api-2.1.1/src/ubkg_api/common_routes/deprecated/tui/__init__.py
--rw-r--r--   0 ZHY19      (503) staff       (20)      803 2024-04-12 19:00:53.000000 ubkg_api-2.1.1/src/ubkg_api/common_routes/deprecated/tui/tui_controller.py
-drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2024-04-12 19:14:51.468031 ubkg_api-2.1.1/src/ubkg_api/common_routes/node_types/
--rw-r--r--   0 ZHY19      (503) staff       (20)        0 2024-04-12 19:00:53.000000 ubkg_api-2.1.1/src/ubkg_api/common_routes/node_types/__init__.py
--rw-r--r--   0 ZHY19      (503) staff       (20)     6174 2024-04-12 19:00:53.000000 ubkg_api-2.1.1/src/ubkg_api/common_routes/node_types/node_types_controller.py
-drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2024-04-12 19:14:51.470199 ubkg_api-2.1.1/src/ubkg_api/common_routes/property_types/
--rw-r--r--   0 ZHY19      (503) staff       (20)        0 2024-04-12 19:00:53.000000 ubkg_api-2.1.1/src/ubkg_api/common_routes/property_types/__init__.py
--rw-r--r--   0 ZHY19      (503) staff       (20)     1009 2024-04-12 19:00:53.000000 ubkg_api-2.1.1/src/ubkg_api/common_routes/property_types/property_types_controller.py
-drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2024-04-12 19:14:51.472635 ubkg_api-2.1.1/src/ubkg_api/common_routes/relationship_types/
--rw-r--r--   0 ZHY19      (503) staff       (20)        0 2024-04-12 19:00:53.000000 ubkg_api-2.1.1/src/ubkg_api/common_routes/relationship_types/__init__.py
--rw-r--r--   0 ZHY19      (503) staff       (20)     1046 2024-04-12 19:00:53.000000 ubkg_api-2.1.1/src/ubkg_api/common_routes/relationship_types/relationship_types_controller.py
-drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2024-04-12 19:14:51.476111 ubkg_api-2.1.1/src/ubkg_api/common_routes/sabs/
--rw-r--r--   0 ZHY19      (503) staff       (20)        0 2024-04-12 19:00:53.000000 ubkg_api-2.1.1/src/ubkg_api/common_routes/sabs/__init__.py
--rw-r--r--   0 ZHY19      (503) staff       (20)     7433 2024-04-12 19:00:53.000000 ubkg_api-2.1.1/src/ubkg_api/common_routes/sabs/sabs_controller.py
-drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2024-04-12 19:14:51.478830 ubkg_api-2.1.1/src/ubkg_api/common_routes/semantics/
--rw-r--r--   0 ZHY19      (503) staff       (20)        0 2024-04-12 19:00:53.000000 ubkg_api-2.1.1/src/ubkg_api/common_routes/semantics/__init__.py
--rw-r--r--   0 ZHY19      (503) staff       (20)     5563 2024-04-12 19:00:53.000000 ubkg_api-2.1.1/src/ubkg_api/common_routes/semantics/semantics_controller.py
-drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2024-04-12 19:14:51.481521 ubkg_api-2.1.1/src/ubkg_api/common_routes/status/
--rw-r--r--   0 ZHY19      (503) staff       (20)        0 2024-04-12 19:00:53.000000 ubkg_api-2.1.1/src/ubkg_api/common_routes/status/__init__.py
--rw-r--r--   0 ZHY19      (503) staff       (20)      930 2024-04-12 19:00:53.000000 ubkg_api-2.1.1/src/ubkg_api/common_routes/status/status_controller.py
-drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2024-04-12 19:14:51.484007 ubkg_api-2.1.1/src/ubkg_api/common_routes/terms/
--rw-r--r--   0 ZHY19      (503) staff       (20)        0 2024-04-12 19:00:53.000000 ubkg_api-2.1.1/src/ubkg_api/common_routes/terms/__init__.py
--rw-r--r--   0 ZHY19      (503) staff       (20)     2675 2024-04-12 19:00:53.000000 ubkg_api-2.1.1/src/ubkg_api/common_routes/terms/terms_controller.py
--rw-r--r--   0 ZHY19      (503) staff       (20)      364 2024-04-12 19:00:53.000000 ubkg_api-2.1.1/src/ubkg_api/common_routes/validate.py
-drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2024-04-12 19:14:51.535126 ubkg_api-2.1.1/src/ubkg_api/models/
--rw-r--r--   0 ZHY19      (503) staff       (20)        0 2024-04-12 19:00:53.000000 ubkg_api-2.1.1/src/ubkg_api/models/__init__.py
--rw-r--r--   0 ZHY19      (503) staff       (20)     1900 2024-04-12 19:00:53.000000 ubkg_api-2.1.1/src/ubkg_api/models/base_model_.py
--rw-r--r--   0 ZHY19      (503) staff       (20)     2518 2024-04-12 19:00:53.000000 ubkg_api-2.1.1/src/ubkg_api/models/codes_codes_obj.py
--rw-r--r--   0 ZHY19      (503) staff       (20)     2037 2024-04-12 19:00:53.000000 ubkg_api-2.1.1/src/ubkg_api/models/concept_detail.py
--rw-r--r--   0 ZHY19      (503) staff       (20)     5760 2024-04-12 19:00:53.000000 ubkg_api-2.1.1/src/ubkg_api/models/concept_graph.py
--rw-r--r--   0 ZHY19      (503) staff       (20)     1512 2024-04-12 19:00:53.000000 ubkg_api-2.1.1/src/ubkg_api/models/concept_node.py
--rw-r--r--   0 ZHY19      (503) staff       (20)     4715 2024-04-12 19:00:53.000000 ubkg_api-2.1.1/src/ubkg_api/models/concept_path_hop.py
--rw-r--r--   0 ZHY19      (503) staff       (20)     2126 2024-04-12 19:00:53.000000 ubkg_api-2.1.1/src/ubkg_api/models/concept_prefterm.py
--rw-r--r--   0 ZHY19      (503) staff       (20)     2615 2024-04-12 19:00:53.000000 ubkg_api-2.1.1/src/ubkg_api/models/concept_sab_rel.py
--rw-r--r--   0 ZHY19      (503) staff       (20)     3336 2024-04-12 19:00:53.000000 ubkg_api-2.1.1/src/ubkg_api/models/concept_sab_rel_depth.py
--rw-r--r--   0 ZHY19      (503) staff       (20)     1909 2024-04-12 19:00:53.000000 ubkg_api-2.1.1/src/ubkg_api/models/concept_term.py
-drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2024-04-12 19:14:51.542315 ubkg_api-2.1.1/src/ubkg_api/models/deprecated/
--rw-r--r--   0 ZHY19      (503) staff       (20)        0 2024-04-12 19:00:53.000000 ubkg_api-2.1.1/src/ubkg_api/models/deprecated/__init__.py
--rw-r--r--   0 ZHY19      (503) staff       (20)     3438 2024-04-12 19:00:53.000000 ubkg_api-2.1.1/src/ubkg_api/models/deprecated/concept_path.py
--rw-r--r--   0 ZHY19      (503) staff       (20)     1946 2024-04-12 19:00:53.000000 ubkg_api-2.1.1/src/ubkg_api/models/deprecated/semantic_stn.py
--rw-r--r--   0 ZHY19      (503) staff       (20)     2351 2024-04-12 19:00:53.000000 ubkg_api-2.1.1/src/ubkg_api/models/deprecated/sty_tui_stn.py
--rw-r--r--   0 ZHY19      (503) staff       (20)     1418 2024-04-12 19:00:53.000000 ubkg_api-2.1.1/src/ubkg_api/models/node_type.py
--rw-r--r--   0 ZHY19      (503) staff       (20)     5645 2024-04-12 19:00:53.000000 ubkg_api-2.1.1/src/ubkg_api/models/path_item_concept_relationship_sab_prefterm.py
--rw-r--r--   0 ZHY19      (503) staff       (20)     3704 2024-04-12 19:00:53.000000 ubkg_api-2.1.1/src/ubkg_api/models/qconcept_tconcept_sab_rel.py
--rw-r--r--   0 ZHY19      (503) staff       (20)     3677 2024-04-12 19:00:53.000000 ubkg_api-2.1.1/src/ubkg_api/models/qqst.py
--rw-r--r--   0 ZHY19      (503) staff       (20)     1988 2024-04-12 19:00:53.000000 ubkg_api-2.1.1/src/ubkg_api/models/sab_definition.py
--rw-r--r--   0 ZHY19      (503) staff       (20)     3895 2024-04-12 19:00:53.000000 ubkg_api-2.1.1/src/ubkg_api/models/sab_relationship_concept_prefterm.py
--rw-r--r--   0 ZHY19      (503) staff       (20)     3537 2024-04-12 19:00:53.000000 ubkg_api-2.1.1/src/ubkg_api/models/sab_relationship_concept_term.py
--rw-r--r--   0 ZHY19      (503) staff       (20)     2198 2024-04-12 19:00:53.000000 ubkg_api-2.1.1/src/ubkg_api/models/semantictype.py
--rw-r--r--   0 ZHY19      (503) staff       (20)     1949 2024-04-12 19:00:53.000000 ubkg_api-2.1.1/src/ubkg_api/models/termtype_code.py
--rw-r--r--   0 ZHY19      (503) staff       (20)      809 2024-04-12 19:00:53.000000 ubkg_api-2.1.1/src/ubkg_api/models/typing_utils.py
--rw-r--r--   0 ZHY19      (503) staff       (20)     3507 2024-04-12 19:00:53.000000 ubkg_api-2.1.1/src/ubkg_api/models/util.py
--rw-r--r--   0 ZHY19      (503) staff       (20)     6991 2024-04-12 19:00:53.000000 ubkg_api-2.1.1/src/ubkg_api/neo4j_connection_helper.py
-drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2024-04-12 19:14:51.547371 ubkg_api-2.1.1/src/ubkg_api/utils/
--rw-r--r--   0 ZHY19      (503) staff       (20)        0 2024-04-12 19:00:53.000000 ubkg_api-2.1.1/src/ubkg_api/utils/__init__.py
-drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2024-04-12 19:14:51.549597 ubkg_api-2.1.1/src/ubkg_api/utils/deprecated/
--rw-r--r--   0 ZHY19      (503) staff       (20)        0 2024-04-12 19:00:53.000000 ubkg_api-2.1.1/src/ubkg_api/utils/deprecated/__init__.py
--rw-r--r--   0 ZHY19      (503) staff       (20)     2038 2024-04-12 19:00:53.000000 ubkg_api-2.1.1/src/ubkg_api/utils/deprecated/path_get_endpoints.py
--rw-r--r--   0 ZHY19      (503) staff       (20)     9744 2024-04-12 19:00:53.000000 ubkg_api-2.1.1/src/ubkg_api/utils/http_error_string.py
--rw-r--r--   0 ZHY19      (503) staff       (20)     1716 2024-04-12 19:00:53.000000 ubkg_api-2.1.1/src/ubkg_api/utils/http_parameter.py
--rwxr-xr-x   0 ZHY19      (503) staff       (20)      185 2024-04-12 19:00:53.000000 ubkg_api-2.1.1/src/ubkg_api/wsgi.py
-drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2024-04-12 19:14:51.550014 ubkg_api-2.1.1/src/ubkg_api.egg-info/
--rw-r--r--   0 ZHY19      (503) staff       (20)    12051 2024-04-12 19:14:51.000000 ubkg_api-2.1.1/src/ubkg_api.egg-info/PKG-INFO
--rw-r--r--   0 ZHY19      (503) staff       (20)     2979 2024-04-12 19:14:51.000000 ubkg_api-2.1.1/src/ubkg_api.egg-info/SOURCES.txt
--rw-r--r--   0 ZHY19      (503) staff       (20)        1 2024-04-12 19:14:51.000000 ubkg_api-2.1.1/src/ubkg_api.egg-info/dependency_links.txt
--rw-r--r--   0 ZHY19      (503) staff       (20)       69 2024-04-12 19:14:51.000000 ubkg_api-2.1.1/src/ubkg_api.egg-info/requires.txt
--rw-r--r--   0 ZHY19      (503) staff       (20)       18 2024-04-12 19:14:51.000000 ubkg_api-2.1.1/src/ubkg_api.egg-info/top_level.txt
+drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2024-05-08 15:11:07.085240 ubkg_api-2.1.2/
+-rw-r--r--   0 ZHY19      (503) staff       (20)     1087 2024-04-12 19:00:53.000000 ubkg_api-2.1.2/LICENSE
+-rw-r--r--   0 ZHY19      (503) staff       (20)    12051 2024-05-08 15:11:07.084258 ubkg_api-2.1.2/PKG-INFO
+-rw-r--r--   0 ZHY19      (503) staff       (20)    11349 2024-04-12 19:00:53.000000 ubkg_api-2.1.2/README.md
+-rw-r--r--   0 ZHY19      (503) staff       (20)      762 2024-05-08 15:07:19.000000 ubkg_api-2.1.2/pyproject.toml
+-rw-r--r--   0 ZHY19      (503) staff       (20)       38 2024-05-08 15:11:07.085299 ubkg_api-2.1.2/setup.cfg
+drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2024-05-08 15:11:06.956987 ubkg_api-2.1.2/src/
+-rw-r--r--   0 ZHY19      (503) staff       (20)        0 2024-04-12 19:00:53.000000 ubkg_api-2.1.2/src/__init__.py
+drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2024-05-08 15:11:06.969312 ubkg_api-2.1.2/src/ubkg_api/
+-rw-r--r--   0 ZHY19      (503) staff       (20)        0 2024-04-12 19:00:53.000000 ubkg_api-2.1.2/src/ubkg_api/__init__.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     5553 2024-05-08 15:07:19.000000 ubkg_api-2.1.2/src/ubkg_api/app.py
+drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2024-05-08 15:11:06.980352 ubkg_api-2.1.2/src/ubkg_api/common_routes/
+-rw-r--r--   0 ZHY19      (503) staff       (20)        0 2024-04-12 19:00:53.000000 ubkg_api-2.1.2/src/ubkg_api/common_routes/__init__.py
+drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2024-05-08 15:11:06.983186 ubkg_api-2.1.2/src/ubkg_api/common_routes/codes/
+-rw-r--r--   0 ZHY19      (503) staff       (20)        0 2024-04-12 19:00:53.000000 ubkg_api-2.1.2/src/ubkg_api/common_routes/codes/__init__.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     2280 2024-04-12 19:00:53.000000 ubkg_api-2.1.2/src/ubkg_api/common_routes/codes/codes_controller.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)    39844 2024-05-08 15:07:19.000000 ubkg_api-2.1.2/src/ubkg_api/common_routes/common_neo4j_logic.py
+drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2024-05-08 15:11:06.986245 ubkg_api-2.1.2/src/ubkg_api/common_routes/concepts/
+-rw-r--r--   0 ZHY19      (503) staff       (20)        0 2024-04-12 19:00:53.000000 ubkg_api-2.1.2/src/ubkg_api/common_routes/concepts/__init__.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)    18131 2024-05-08 15:07:19.000000 ubkg_api-2.1.2/src/ubkg_api/common_routes/concepts/concepts_controller.py
+drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2024-05-08 15:11:06.988178 ubkg_api-2.1.2/src/ubkg_api/common_routes/database/
+-rw-r--r--   0 ZHY19      (503) staff       (20)        0 2024-04-12 19:00:53.000000 ubkg_api-2.1.2/src/ubkg_api/common_routes/database/__init__.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)      479 2024-04-12 19:00:53.000000 ubkg_api-2.1.2/src/ubkg_api/common_routes/database/database_controller.py
+drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2024-05-08 15:11:06.988573 ubkg_api-2.1.2/src/ubkg_api/common_routes/deprecated/
+-rw-r--r--   0 ZHY19      (503) staff       (20)        0 2024-04-12 19:00:53.000000 ubkg_api-2.1.2/src/ubkg_api/common_routes/deprecated/__init__.py
+drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2024-05-08 15:11:06.991977 ubkg_api-2.1.2/src/ubkg_api/common_routes/deprecated/tui/
+-rw-r--r--   0 ZHY19      (503) staff       (20)        0 2024-04-12 19:00:53.000000 ubkg_api-2.1.2/src/ubkg_api/common_routes/deprecated/tui/__init__.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)      803 2024-04-12 19:00:53.000000 ubkg_api-2.1.2/src/ubkg_api/common_routes/deprecated/tui/tui_controller.py
+drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2024-05-08 15:11:06.997744 ubkg_api-2.1.2/src/ubkg_api/common_routes/node_types/
+-rw-r--r--   0 ZHY19      (503) staff       (20)        0 2024-04-12 19:00:53.000000 ubkg_api-2.1.2/src/ubkg_api/common_routes/node_types/__init__.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     6174 2024-04-12 19:00:53.000000 ubkg_api-2.1.2/src/ubkg_api/common_routes/node_types/node_types_controller.py
+drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2024-05-08 15:11:07.000877 ubkg_api-2.1.2/src/ubkg_api/common_routes/property_types/
+-rw-r--r--   0 ZHY19      (503) staff       (20)        0 2024-04-12 19:00:53.000000 ubkg_api-2.1.2/src/ubkg_api/common_routes/property_types/__init__.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     1009 2024-04-12 19:00:53.000000 ubkg_api-2.1.2/src/ubkg_api/common_routes/property_types/property_types_controller.py
+drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2024-05-08 15:11:07.004577 ubkg_api-2.1.2/src/ubkg_api/common_routes/relationship_types/
+-rw-r--r--   0 ZHY19      (503) staff       (20)        0 2024-04-12 19:00:53.000000 ubkg_api-2.1.2/src/ubkg_api/common_routes/relationship_types/__init__.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     1046 2024-04-12 19:00:53.000000 ubkg_api-2.1.2/src/ubkg_api/common_routes/relationship_types/relationship_types_controller.py
+drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2024-05-08 15:11:07.009912 ubkg_api-2.1.2/src/ubkg_api/common_routes/sabs/
+-rw-r--r--   0 ZHY19      (503) staff       (20)        0 2024-04-12 19:00:53.000000 ubkg_api-2.1.2/src/ubkg_api/common_routes/sabs/__init__.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     7433 2024-04-12 19:00:53.000000 ubkg_api-2.1.2/src/ubkg_api/common_routes/sabs/sabs_controller.py
+drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2024-05-08 15:11:07.013732 ubkg_api-2.1.2/src/ubkg_api/common_routes/semantics/
+-rw-r--r--   0 ZHY19      (503) staff       (20)        0 2024-04-12 19:00:53.000000 ubkg_api-2.1.2/src/ubkg_api/common_routes/semantics/__init__.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     5563 2024-04-12 19:00:53.000000 ubkg_api-2.1.2/src/ubkg_api/common_routes/semantics/semantics_controller.py
+drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2024-05-08 15:11:07.016246 ubkg_api-2.1.2/src/ubkg_api/common_routes/status/
+-rw-r--r--   0 ZHY19      (503) staff       (20)        0 2024-04-12 19:00:53.000000 ubkg_api-2.1.2/src/ubkg_api/common_routes/status/__init__.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)      930 2024-04-12 19:00:53.000000 ubkg_api-2.1.2/src/ubkg_api/common_routes/status/status_controller.py
+drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2024-05-08 15:11:07.018728 ubkg_api-2.1.2/src/ubkg_api/common_routes/terms/
+-rw-r--r--   0 ZHY19      (503) staff       (20)        0 2024-04-12 19:00:53.000000 ubkg_api-2.1.2/src/ubkg_api/common_routes/terms/__init__.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     2675 2024-04-12 19:00:53.000000 ubkg_api-2.1.2/src/ubkg_api/common_routes/terms/terms_controller.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)      364 2024-04-12 19:00:53.000000 ubkg_api-2.1.2/src/ubkg_api/common_routes/validate.py
+drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2024-05-08 15:11:07.068335 ubkg_api-2.1.2/src/ubkg_api/models/
+-rw-r--r--   0 ZHY19      (503) staff       (20)        0 2024-04-12 19:00:53.000000 ubkg_api-2.1.2/src/ubkg_api/models/__init__.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     1900 2024-04-12 19:00:53.000000 ubkg_api-2.1.2/src/ubkg_api/models/base_model_.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     2518 2024-04-12 19:00:53.000000 ubkg_api-2.1.2/src/ubkg_api/models/codes_codes_obj.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     2037 2024-04-12 19:00:53.000000 ubkg_api-2.1.2/src/ubkg_api/models/concept_detail.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     5760 2024-04-12 19:00:53.000000 ubkg_api-2.1.2/src/ubkg_api/models/concept_graph.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     1512 2024-04-12 19:00:53.000000 ubkg_api-2.1.2/src/ubkg_api/models/concept_node.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     4715 2024-04-12 19:00:53.000000 ubkg_api-2.1.2/src/ubkg_api/models/concept_path_hop.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     2126 2024-04-12 19:00:53.000000 ubkg_api-2.1.2/src/ubkg_api/models/concept_prefterm.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     2615 2024-04-12 19:00:53.000000 ubkg_api-2.1.2/src/ubkg_api/models/concept_sab_rel.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     3336 2024-04-12 19:00:53.000000 ubkg_api-2.1.2/src/ubkg_api/models/concept_sab_rel_depth.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     1909 2024-04-12 19:00:53.000000 ubkg_api-2.1.2/src/ubkg_api/models/concept_term.py
+drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2024-05-08 15:11:07.074818 ubkg_api-2.1.2/src/ubkg_api/models/deprecated/
+-rw-r--r--   0 ZHY19      (503) staff       (20)        0 2024-04-12 19:00:53.000000 ubkg_api-2.1.2/src/ubkg_api/models/deprecated/__init__.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     3438 2024-04-12 19:00:53.000000 ubkg_api-2.1.2/src/ubkg_api/models/deprecated/concept_path.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     1946 2024-04-12 19:00:53.000000 ubkg_api-2.1.2/src/ubkg_api/models/deprecated/semantic_stn.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     2351 2024-04-12 19:00:53.000000 ubkg_api-2.1.2/src/ubkg_api/models/deprecated/sty_tui_stn.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     1418 2024-04-12 19:00:53.000000 ubkg_api-2.1.2/src/ubkg_api/models/node_type.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     5645 2024-04-12 19:00:53.000000 ubkg_api-2.1.2/src/ubkg_api/models/path_item_concept_relationship_sab_prefterm.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     3704 2024-04-12 19:00:53.000000 ubkg_api-2.1.2/src/ubkg_api/models/qconcept_tconcept_sab_rel.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     3677 2024-04-12 19:00:53.000000 ubkg_api-2.1.2/src/ubkg_api/models/qqst.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     1988 2024-04-12 19:00:53.000000 ubkg_api-2.1.2/src/ubkg_api/models/sab_definition.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     3895 2024-04-12 19:00:53.000000 ubkg_api-2.1.2/src/ubkg_api/models/sab_relationship_concept_prefterm.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     3537 2024-04-12 19:00:53.000000 ubkg_api-2.1.2/src/ubkg_api/models/sab_relationship_concept_term.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     2198 2024-04-12 19:00:53.000000 ubkg_api-2.1.2/src/ubkg_api/models/semantictype.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     1949 2024-04-12 19:00:53.000000 ubkg_api-2.1.2/src/ubkg_api/models/termtype_code.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)      809 2024-04-12 19:00:53.000000 ubkg_api-2.1.2/src/ubkg_api/models/typing_utils.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     3507 2024-04-12 19:00:53.000000 ubkg_api-2.1.2/src/ubkg_api/models/util.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     6991 2024-04-12 19:00:53.000000 ubkg_api-2.1.2/src/ubkg_api/neo4j_connection_helper.py
+drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2024-05-08 15:11:07.080415 ubkg_api-2.1.2/src/ubkg_api/utils/
+-rw-r--r--   0 ZHY19      (503) staff       (20)        0 2024-04-12 19:00:53.000000 ubkg_api-2.1.2/src/ubkg_api/utils/__init__.py
+drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2024-05-08 15:11:07.082958 ubkg_api-2.1.2/src/ubkg_api/utils/deprecated/
+-rw-r--r--   0 ZHY19      (503) staff       (20)        0 2024-04-12 19:00:53.000000 ubkg_api-2.1.2/src/ubkg_api/utils/deprecated/__init__.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     2038 2024-04-12 19:00:53.000000 ubkg_api-2.1.2/src/ubkg_api/utils/deprecated/path_get_endpoints.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     9745 2024-05-08 15:07:19.000000 ubkg_api-2.1.2/src/ubkg_api/utils/http_error_string.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     1716 2024-04-12 19:00:53.000000 ubkg_api-2.1.2/src/ubkg_api/utils/http_parameter.py
+-rwxr-xr-x   0 ZHY19      (503) staff       (20)      185 2024-04-12 19:00:53.000000 ubkg_api-2.1.2/src/ubkg_api/wsgi.py
+drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2024-05-08 15:11:07.083631 ubkg_api-2.1.2/src/ubkg_api.egg-info/
+-rw-r--r--   0 ZHY19      (503) staff       (20)    12051 2024-05-08 15:11:06.000000 ubkg_api-2.1.2/src/ubkg_api.egg-info/PKG-INFO
+-rw-r--r--   0 ZHY19      (503) staff       (20)     2979 2024-05-08 15:11:06.000000 ubkg_api-2.1.2/src/ubkg_api.egg-info/SOURCES.txt
+-rw-r--r--   0 ZHY19      (503) staff       (20)        1 2024-05-08 15:11:06.000000 ubkg_api-2.1.2/src/ubkg_api.egg-info/dependency_links.txt
+-rw-r--r--   0 ZHY19      (503) staff       (20)       69 2024-05-08 15:11:06.000000 ubkg_api-2.1.2/src/ubkg_api.egg-info/requires.txt
+-rw-r--r--   0 ZHY19      (503) staff       (20)       18 2024-05-08 15:11:06.000000 ubkg_api-2.1.2/src/ubkg_api.egg-info/top_level.txt
```

### Comparing `ubkg_api-2.1.1/LICENSE` & `ubkg_api-2.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ubkg_api-2.1.1/PKG-INFO` & `ubkg_api-2.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ubkg_api
-Version: 2.1.1
+Version: 2.1.2
 Summary: A REST API in front of the Unified Biomedical Knowlegde Graph
 Author-email: HuBMAP Consortium <api-developers@hubmapconsortium.org>
 Project-URL: Homepage, https://github.com/x-atlas-consortia/ubkg-api
 Project-URL: Bug Tracker, https://github.com/x-atlas-consortia/ubkg-api/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ubkg_api-2.1.1/README.md` & `ubkg_api-2.1.2/README.md`

 * *Files identical despite different names*

### Comparing `ubkg_api-2.1.1/pyproject.toml` & `ubkg_api-2.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ubkg_api"
-version = "2.1.1"
+version = "2.1.2"
 authors = [
   { name="HuBMAP Consortium", email="api-developers@hubmapconsortium.org" },
 ]
 description = "A REST API in front of the Unified Biomedical Knowlegde Graph"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `ubkg_api-2.1.1/src/ubkg_api/app.py` & `ubkg_api-2.1.2/src/ubkg_api/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,17 +84,17 @@
                     # Set self based on passed in config parameters
                     for key, value in config.items():
                         setattr(self, key, value)
                     self.app.neo4jConnectionHelper = \
                         Neo4jConnectionHelper.create(self.SERVER,
                                                      self.USERNAME,
                                                      self.PASSWORD,
-                                                     15000,
+                                                     28,
                                                      1000,
-                                                     1048576)
+                                                     9437184)
                     logger.info("Initialized Neo4jManager successfully for: {self.SERVER}")
         except Exception as e:
             logger.exception('Failed to initialize the Neo4jManager')
             raise e
 
         @self.app.route('/', methods=['GET'])
         def index():
```

### Comparing `ubkg_api-2.1.1/src/ubkg_api/common_routes/codes/codes_controller.py` & `ubkg_api-2.1.2/src/ubkg_api/common_routes/codes/codes_controller.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-2.1.1/src/ubkg_api/common_routes/common_neo4j_logic.py` & `ubkg_api-2.1.2/src/ubkg_api/common_routes/common_neo4j_logic.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,17 @@
 
 """
 import logging
 import re
 from typing import List
 import os
 
+# Apr 2024
+from pathlib import Path
+
 import neo4j
 
 from models.codes_codes_obj import CodesCodesObj
 from models.concept_detail import ConceptDetail
 from models.concept_graph import ConceptGraph
 from models.concept_sab_rel_depth import ConceptSabRelDepth
 from models.concept_term import ConceptTerm
@@ -49,20 +52,26 @@
     Keeping query strings separate from the Python code:
     1. Separates business logic from the presentation layer.
     2. Eases the transition from neo4j development to API development--in particular, by elminating the need to
          reformat a query string in Python
 
     :param filename: filename, without path.
 
-    Assumes that the file is in the cypher directory.
+    APRIL 2024
+    Assumes that the file is in the cypher subdirectory, which is at the same level as the script path.
+    When ubkg-api endpoints are called as passthrough from hs-ontology api, the script path is in hs-ontology-api.
+
+
     """
 
-    fpath = os.path.dirname(os.getcwd())
-    fpath = os.path.join(fpath, 'ubkg_api/cypher', filename)
+    #fpath = os.path.dirname(os.getcwd())
+    #fpath = os.path.join(fpath, 'ubkg_api/cypher', filename)
 
+    fpath = Path(__file__).resolve().parent.parent
+    fpath = os.path.join(fpath,'cypher',filename)
     f = open(fpath, "r")
     query = f.read()
     f.close()
     return query
 
 
 def timebox_query(query: str, timeout: int = 10000) -> str:
@@ -307,17 +316,17 @@
     querytxt = querytxt.replace('$maxdepth', str(maxdepth))
     querytxt = querytxt.replace('$skip', str(skip))
     querytxt = querytxt.replace('$limit', str(limit))
 
     # Set timeout for query based on value in app.cfg.
     query = neo4j.Query(text=querytxt, timeout=neo4j_instance.timeout)
 
+    # MAY 2024 - bug fix - changed argument from querytxt to query
     return get_graph(neo4j_instance, query=query)
 
-
 def concepts_shortestpath_get_logic(neo4j_instance, origin_concept_id=None, terminus_concept_id=None,
                                     sab=None, rel=None) \
         -> List[PathItemConceptRelationshipSabPrefterm]:
 
     # Load query string and associate parameter values to variables.
     querytxt = loadquerystring(filename='concepts_shortestpath.cypher')
     querytxt = querytxt.replace('$origin_concept_id', f'"{origin_concept_id}"')
@@ -504,60 +513,60 @@
 
     termtypecodes: [TermtypeCode] = []
 
     """
     Returns information on Codes with terms that exactly match the specified term_id string.
     """
 
-    query: str = \
+    querytxt: str = \
         'WITH [$term_id] AS query' \
         ' MATCH (a:Term)<-[b]-(c:Code)' \
         ' WHERE a.name IN query' \
         ' RETURN DISTINCT a.name AS Term, Type(b) AS TermType, c.CodeID AS Code' \
         ' ORDER BY Term, TermType, Code'
 
-    # JAS February 2024
-    # To prevent timeout errors, limit the query execution time to a value specified in the app.cfg.
-    query = query.replace('$term_id', f'"{term_id}"')
-    query = timebox_query(query=query, timeout=neo4j_instance.timeout)
+    # JAS February 2024/May 2024
+    # To prevent timeout errors, limit the query execution time to a value specified in the app.cfg
+    querytxt = querytxt.replace('$term_id', f'"{term_id}"')
+
+    # Set timeout for query based on value in app.cfg.
+    query = neo4j.Query(text=querytxt, timeout=neo4j_instance.timeout)
     with neo4j_instance.driver.session() as session:
         recds: neo4j.Result = session.run(query)
         for record in recds:
-            # The timeboxed query returns query results as values of a dict instead of as a dict.
-            val = record.get('value')
             try:
-                termtypecode: TermtypeCode = TermtypeCode(val.get('TermType'), val.get('Code')).serialize()
+                termtypecode: TermtypeCode = TermtypeCode(record.get('TermType'), record.get('Code')).serialize()
                 termtypecodes.append(termtypecode)
             except KeyError:
                 pass
     return termtypecodes
 
 
 def terms_term_id_concepts_get_logic(neo4j_instance, term_id: str) -> List[str]:
     concepts: [str] = []
-    query: str = \
+    querytxt: str = \
         'WITH [$term_id] AS query' \
         ' MATCH (a:Term)<-[b]-(c:Code)<-[:CODE]-(d:Concept)' \
         ' WHERE a.name IN query AND b.CUI = d.CUI' \
         ' OPTIONAL MATCH (a:Term)<--(d:Concept) WHERE a.name IN query' \
         ' RETURN DISTINCT a.name AS Term, d.CUI AS Concept' \
         ' ORDER BY Concept ASC'
 
-    # JAS February 2024
+    # JAS February 2024/May 2024
     # To prevent timeout errors, limit the query execution time to a value specified in the app.cfg.
-    query = query.replace('$term_id', f'"{term_id}"')
-    query = timebox_query(query, timeout=neo4j_instance.timeout)
+    querytxt = querytxt.replace('$term_id', f'"{term_id}"')
+
+    # Set timeout for query based on value in app.cfg.
+    query = neo4j.Query(text=querytxt, timeout=neo4j_instance.timeout)
+
     with neo4j_instance.driver.session() as session:
         recds: neo4j.Result = session.run(query)
         for record in recds:
-            # The timeboxed query returns query results as values of a dict instead of as a dict.
-            val = record.get('value')
             try:
-                concept: str = val.get('Concept')
-                concepts.append(concept)
+                concepts.append(record)
             except KeyError:
                 pass
 
     return concepts
 
 
 def remove_null_placeholder_objects(listdict: list[dict]) -> list[dict]:
@@ -600,31 +609,31 @@
 
 
 def concepts_identfier_node_get_logic(neo4j_instance, search: str) -> List[ConceptNode]:
     """
     Obtains information on the set of Concept subgraphs with identifiers that match the search parameter string.
 
     """
+    # MAY 2024 - Replaced timeboxing method.
+
     conceptnodes: [ConceptNode] = []
-    query = loadquerystring(filename='concepts_nodes.cypher')
+    querytxt = loadquerystring(filename='concepts_nodes.cypher')
 
     # Format the search parameter for the Cypher query.
     list_identifier = [search]
     list_identifier_join = format_list_for_query(listquery=list_identifier, doublequote=True)
-    query = query.replace('$search', list_identifier_join)
+    querytxt = querytxt.replace('$search', list_identifier_join)
 
-    # Timebox the query.
-    query = timebox_query(query, timeout=neo4j_instance.timeout)
+    # Set timeout for query based on value in app.cfg.
+    query = neo4j.Query(text=querytxt, timeout=neo4j_instance.timeout)
 
     with neo4j_instance.driver.session() as session:
         recds: neo4j.Result = session.run(query)
         for record in recds:
-            # The timeboxed query returns query results as values of a dict instead of as a dict.
-            val = record.get('value')
-            concept = val.get('nodeobject')
+            concept = record.get('nodeobject')
             # Remove null placeholder dictionaries from nested list objects.
             concept['semantic_types'] = remove_null_placeholder_objects(concept.get('semantic_types'))
             concept['definitions'] = remove_null_placeholder_objects(concept.get('definitions'))
             try:
                 conceptnode: ConceptNode = ConceptNode(concept).serialize()
                 conceptnodes.append(conceptnode)
             except KeyError:
@@ -699,40 +708,43 @@
     Obtains information on node types, grouped by SAB.
 
     :param node_type: an optional filter for node type (label)
     :param neo4j_instance: neo4j connection
     :param sab: optional list of sabs
 
     """
+
+    # MAY 2024 - Replaced timeboxing method.
+
     nodetypes: [NodeType] = []
     # Load and parameterize base query.
-    query = loadquerystring('node_types_by_sab.cypher')
+    querytxt = loadquerystring('node_types_by_sab.cypher')
 
     if node_type is None:
         node_type = ''
     else:
         node_type = [node_type]
     typesjoin = format_list_for_query(listquery=node_type, doublequote=True)
-    query = query.replace('$node_type', typesjoin)
+    querytxt = querytxt.replace('$node_type', typesjoin)
+
     if sab is None:
         sab = ''
     else:
         sabjoin = format_list_for_query(listquery=sab, doublequote=True)
-    query = query.replace('$sab', sabjoin)
+    querytxt = querytxt.replace('$sab', sabjoin)
 
-    # Limit query execution time to duration specified in app.cfg.
-    query = timebox_query(query, timeout=neo4j_instance.timeout)
+    # Set timeout for query based on value in app.cfg.
+    query = neo4j.Query(text=querytxt, timeout=neo4j_instance.timeout)
 
     with neo4j_instance.driver.session() as session:
         recds: neo4j.Result = session.run(query)
         total_count = 0
         for record in recds:
             # Each row from the query includes a dict that contains the actual response content.
-            val = record.get('value')
-            output = val.get('output')
+            output = record.get('output')
             node_types = output.get('node_types')
             for node_type in node_types:
                 count_by_label = node_type.get('count')
                 total_count = total_count + count_by_label
             try:
                 nodetype: NodeType = NodeType(node_type).serialize()
                 nodetypes.append(nodetype)
@@ -749,34 +761,35 @@
 
     :param node_type: an optional filter for node type (label)
     :param neo4j_instance: neo4j connection
 
     """
     nodetypes: [NodeType] = []
     # Load and parameterize base query.
-    query = loadquerystring('node_types.cypher')
+    querytxt = loadquerystring('node_types.cypher')
 
     if node_type is None:
         node_type = ''
     else:
         node_type = [node_type]
     typesjoin = format_list_for_query(listquery=node_type, doublequote=True)
-    query = query.replace('$node_type', typesjoin)
+    querytxt = querytxt.replace('$node_type', typesjoin)
 
-    # Limit query execution time to duration specified in app.cfg.
-    query = timebox_query(query, timeout=neo4j_instance.timeout)
+    # MAY 2024 replaced timebox method.
+    # Set timeout for query based on value in app.cfg.
+    query = neo4j.Query(text=querytxt, timeout=neo4j_instance.timeout)
 
     with neo4j_instance.driver.session() as session:
         recds: neo4j.Result = session.run(query)
         total_count = 0
         for record in recds:
             # Each row from the query includes a dict that contains the actual response content.
-            val = record.get('value')
-            output = val.get('output')
+            output = record.get('output')
             node_types = output.get('node_types')
+            print(node_types)
             for node_type in node_types:
                 count_by_label = node_type.get('count')
                 total_count = total_count + count_by_label
                 try:
                     nodetype: NodeType = NodeType(node_type).serialize()
                     nodetypes.append(nodetype)
                 except KeyError:
@@ -954,34 +967,35 @@
     :param limit: LIMIT value for the query
     :param sab: source (SAB)
 
     """
     codes: [dict] = []
 
     # Load and parameterize query.
-    query = loadquerystring('sabs_codes_details.cypher')
+    querytxt = loadquerystring('sabs_codes_details.cypher')
     if sab is None:
         sabjoin = ''
     else:
         sabjoin = format_list_for_query(listquery=[sab], doublequote=True)
-    query = query.replace('$sab', sabjoin)
+    querytxt = querytxt.replace('$sab', sabjoin)
 
-    query = query.replace('$skip', str(skip))
-    query = query.replace('$limit', str(limit))
+    querytxt = querytxt.replace('$skip', str(skip))
+    querytxt = querytxt.replace('$limit', str(limit))
 
-    query = timebox_query(query=query, timeout=neo4j_instance.timeout)
+    # MAY 2024 Replacing timebox method.
+    # Set timeout for query based on value in app.cfg.
+    query = neo4j.Query(text=querytxt, timeout=neo4j_instance.timeout)
 
     with neo4j_instance.driver.session() as session:
         recds: neo4j.Result = session.run(query)
         # Track the position of the codes in the list, based on the value of skip.
         position = int(skip) + 1
         res_codes = {}
         for record in recds:
-            val = record.get('value')
-            output = val.get('output')
+            output = record.get('output')
             try:
                 res_codes = output.get('codes')
                 for c in res_codes:
                     c['position'] = position
                     position = position + 1
                 codes.append(res_codes)
```

### Comparing `ubkg_api-2.1.1/src/ubkg_api/common_routes/concepts/concepts_controller.py` & `ubkg_api-2.1.2/src/ubkg_api/common_routes/concepts/concepts_controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,25 +132,28 @@
 
     # Check that the minimum path depth is non-negative.
     mindepth = request.args.get('mindepth')
     err = validate_parameter_is_nonnegative(param_name='mindepth', param_value=mindepth)
     if err != 'ok':
         return make_response(err, 400)
 
+    # APR 2024 - Check range after setting defaults.
+    # Set default mininum.
+    mindepth = set_default_minimum(param_value=mindepth, default=1)
+
+    # MAY 2024 - moved mindepth !> maxdepth check up.
     # Validate that mindepth is not greater than maxdepth.
     err = validate_parameter_range_order(min_name='mindepth', min_value=mindepth, max_name='maxdepth',
                                          max_value=maxdepth)
-    if err != 'ok':
-        return make_response(err, 400)
-
-    # Set default mininum.
-    mindepth = set_default_minimum(param_value=mindepth, default=1)
     # Set default maximum.
     maxdepth = str(int(mindepth) + 2)
 
+    if err != 'ok':
+        return make_response(err, 400)
+
     # Check that the non-default skip is non-negative.
     skip = request.args.get('skip')
     err = validate_parameter_is_nonnegative(param_name='skip', param_value=skip)
     if err != 'ok':
         return make_response(err, 400)
 
     # Set default mininum.
@@ -272,24 +275,24 @@
 
     # Limit the minimum to 0 or 1.
     if int(mindepth) > 1:
         err = f"Invalid value for 'mindepth' {mindepth}. The 'mindepth' parameter value for a spanning tree " \
               f"can be either 0 or 1."
         return make_response(err, 400)
 
-
-    # Set default maximum.
-    maxdepth = str(int(mindepth) + 2)
-
+    # MAY 2024 - moved the mindepth !> maxdepth check before setting the default maxdepth.
     # Validate that mindepth is not greater than maxdepth.
     err = validate_parameter_range_order(min_name='mindepth', min_value=mindepth, max_name='maxdepth',
-                                         max_value=maxdepth)
+                                             max_value=maxdepth)
     if err != 'ok':
         return make_response(err, 400)
 
+    # Set default maximum.
+    maxdepth = str(int(mindepth) + 2)
+
     # Check that the non-default skip is non-negative.
     skip = request.args.get('skip')
     err = validate_parameter_is_nonnegative(param_name='skip', param_value=skip)
     if err != 'ok':
         return make_response(err, 400)
 
     # Set default mininum for the skip.
```

### Comparing `ubkg_api-2.1.1/src/ubkg_api/common_routes/deprecated/tui/tui_controller.py` & `ubkg_api-2.1.2/src/ubkg_api/common_routes/deprecated/tui/tui_controller.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-2.1.1/src/ubkg_api/common_routes/node_types/node_types_controller.py` & `ubkg_api-2.1.2/src/ubkg_api/common_routes/node_types/node_types_controller.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-2.1.1/src/ubkg_api/common_routes/property_types/property_types_controller.py` & `ubkg_api-2.1.2/src/ubkg_api/common_routes/property_types/property_types_controller.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-2.1.1/src/ubkg_api/common_routes/relationship_types/relationship_types_controller.py` & `ubkg_api-2.1.2/src/ubkg_api/common_routes/relationship_types/relationship_types_controller.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-2.1.1/src/ubkg_api/common_routes/sabs/sabs_controller.py` & `ubkg_api-2.1.2/src/ubkg_api/common_routes/sabs/sabs_controller.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-2.1.1/src/ubkg_api/common_routes/semantics/semantics_controller.py` & `ubkg_api-2.1.2/src/ubkg_api/common_routes/semantics/semantics_controller.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-2.1.1/src/ubkg_api/common_routes/status/status_controller.py` & `ubkg_api-2.1.2/src/ubkg_api/common_routes/status/status_controller.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-2.1.1/src/ubkg_api/common_routes/terms/terms_controller.py` & `ubkg_api-2.1.2/src/ubkg_api/common_routes/terms/terms_controller.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-2.1.1/src/ubkg_api/models/base_model_.py` & `ubkg_api-2.1.2/src/ubkg_api/models/base_model_.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-2.1.1/src/ubkg_api/models/codes_codes_obj.py` & `ubkg_api-2.1.2/src/ubkg_api/models/codes_codes_obj.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-2.1.1/src/ubkg_api/models/concept_detail.py` & `ubkg_api-2.1.2/src/ubkg_api/models/concept_detail.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-2.1.1/src/ubkg_api/models/concept_graph.py` & `ubkg_api-2.1.2/src/ubkg_api/models/concept_graph.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-2.1.1/src/ubkg_api/models/concept_node.py` & `ubkg_api-2.1.2/src/ubkg_api/models/concept_node.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-2.1.1/src/ubkg_api/models/concept_path_hop.py` & `ubkg_api-2.1.2/src/ubkg_api/models/concept_path_hop.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-2.1.1/src/ubkg_api/models/concept_prefterm.py` & `ubkg_api-2.1.2/src/ubkg_api/models/concept_prefterm.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-2.1.1/src/ubkg_api/models/concept_sab_rel.py` & `ubkg_api-2.1.2/src/ubkg_api/models/concept_sab_rel.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-2.1.1/src/ubkg_api/models/concept_sab_rel_depth.py` & `ubkg_api-2.1.2/src/ubkg_api/models/concept_sab_rel_depth.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-2.1.1/src/ubkg_api/models/concept_term.py` & `ubkg_api-2.1.2/src/ubkg_api/models/concept_term.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-2.1.1/src/ubkg_api/models/deprecated/concept_path.py` & `ubkg_api-2.1.2/src/ubkg_api/models/deprecated/concept_path.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-2.1.1/src/ubkg_api/models/deprecated/semantic_stn.py` & `ubkg_api-2.1.2/src/ubkg_api/models/deprecated/semantic_stn.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-2.1.1/src/ubkg_api/models/deprecated/sty_tui_stn.py` & `ubkg_api-2.1.2/src/ubkg_api/models/deprecated/sty_tui_stn.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-2.1.1/src/ubkg_api/models/node_type.py` & `ubkg_api-2.1.2/src/ubkg_api/models/node_type.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-2.1.1/src/ubkg_api/models/path_item_concept_relationship_sab_prefterm.py` & `ubkg_api-2.1.2/src/ubkg_api/models/path_item_concept_relationship_sab_prefterm.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-2.1.1/src/ubkg_api/models/qconcept_tconcept_sab_rel.py` & `ubkg_api-2.1.2/src/ubkg_api/models/qconcept_tconcept_sab_rel.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-2.1.1/src/ubkg_api/models/qqst.py` & `ubkg_api-2.1.2/src/ubkg_api/models/qqst.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-2.1.1/src/ubkg_api/models/sab_definition.py` & `ubkg_api-2.1.2/src/ubkg_api/models/sab_definition.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-2.1.1/src/ubkg_api/models/sab_relationship_concept_prefterm.py` & `ubkg_api-2.1.2/src/ubkg_api/models/sab_relationship_concept_prefterm.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-2.1.1/src/ubkg_api/models/sab_relationship_concept_term.py` & `ubkg_api-2.1.2/src/ubkg_api/models/sab_relationship_concept_term.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-2.1.1/src/ubkg_api/models/semantictype.py` & `ubkg_api-2.1.2/src/ubkg_api/models/semantictype.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-2.1.1/src/ubkg_api/models/termtype_code.py` & `ubkg_api-2.1.2/src/ubkg_api/models/termtype_code.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-2.1.1/src/ubkg_api/models/typing_utils.py` & `ubkg_api-2.1.2/src/ubkg_api/models/typing_utils.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-2.1.1/src/ubkg_api/models/util.py` & `ubkg_api-2.1.2/src/ubkg_api/models/util.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-2.1.1/src/ubkg_api/neo4j_connection_helper.py` & `ubkg_api-2.1.2/src/ubkg_api/neo4j_connection_helper.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-2.1.1/src/ubkg_api/utils/deprecated/path_get_endpoints.py` & `ubkg_api-2.1.2/src/ubkg_api/utils/deprecated/path_get_endpoints.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-2.1.1/src/ubkg_api/utils/http_error_string.py` & `ubkg_api-2.1.2/src/ubkg_api/utils/http_error_string.py`

 * *Files 0% similar despite different names*

```diff
@@ -227,14 +227,15 @@
         :param min_value: value for minimum parameter
         :param max_name: name of maximum parameter
         :param max_value: value for maximum parameter
        :return:
        --"ok"
        --error string suitable for a 400 message
        """
+
     if int(min_value) > int(max_value):
         return f"Invalid parameter values: '{min_name}' ({min_value}) greater than '{max_name}' ({max_value}). "
 
     return "ok"
 
 
 def check_payload_size(payload: str, max_payload_size: int) -> str:
```

### Comparing `ubkg_api-2.1.1/src/ubkg_api/utils/http_parameter.py` & `ubkg_api-2.1.2/src/ubkg_api/utils/http_parameter.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-2.1.1/src/ubkg_api.egg-info/PKG-INFO` & `ubkg_api-2.1.2/src/ubkg_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ubkg_api
-Version: 2.1.1
+Version: 2.1.2
 Summary: A REST API in front of the Unified Biomedical Knowlegde Graph
 Author-email: HuBMAP Consortium <api-developers@hubmapconsortium.org>
 Project-URL: Homepage, https://github.com/x-atlas-consortia/ubkg-api
 Project-URL: Bug Tracker, https://github.com/x-atlas-consortia/ubkg-api/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ubkg_api-2.1.1/src/ubkg_api.egg-info/SOURCES.txt` & `ubkg_api-2.1.2/src/ubkg_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

