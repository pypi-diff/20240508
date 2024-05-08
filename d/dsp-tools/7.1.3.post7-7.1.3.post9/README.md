# Comparing `tmp/dsp_tools-7.1.3.post7.tar.gz` & `tmp/dsp_tools-7.1.3.post9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsp_tools-7.1.3.post7.tar", max compression
+gzip compressed data, was "dsp_tools-7.1.3.post9.tar", max compression
```

## Comparing `dsp_tools-7.1.3.post7.tar` & `dsp_tools-7.1.3.post9.tar`

### file list

```diff
@@ -1,115 +1,117 @@
--rw-r--r--   0        0        0    35149 2024-05-03 11:07:29.471428 dsp_tools-7.1.3.post7/LICENSE
--rw-r--r--   0        0        0     4941 2024-05-03 11:07:29.483428 dsp_tools-7.1.3.post7/docs/index.md
--rw-r--r--   0        0        0     8372 2024-05-03 11:08:04.283989 dsp_tools-7.1.3.post7/pyproject.toml
--rw-r--r--   0        0        0       41 2024-05-03 11:07:29.487428 dsp_tools-7.1.3.post7/src/dsp_tools/__init__.py
--rw-r--r--   0        0        0        0 2024-05-03 11:07:29.487428 dsp_tools-7.1.3.post7/src/dsp_tools/cli/__init__.py
--rw-r--r--   0        0        0     7410 2024-05-03 11:07:29.487428 dsp_tools-7.1.3.post7/src/dsp_tools/cli/call_action.py
--rw-r--r--   0        0        0    12631 2024-05-03 11:07:29.487428 dsp_tools-7.1.3.post7/src/dsp_tools/cli/create_parsers.py
--rw-r--r--   0        0        0     9909 2024-05-03 11:07:29.487428 dsp_tools-7.1.3.post7/src/dsp_tools/cli/entry_point.py
--rw-r--r--   0        0        0        0 2024-05-03 11:07:29.487428 dsp_tools-7.1.3.post7/src/dsp_tools/commands/__init__.py
--rw-r--r--   0        0        0        0 2024-05-03 11:07:29.487428 dsp_tools-7.1.3.post7/src/dsp_tools/commands/excel2json/__init__.py
--rw-r--r--   0        0        0    15987 2024-05-03 11:07:29.487428 dsp_tools-7.1.3.post7/src/dsp_tools/commands/excel2json/lists.py
--rw-r--r--   0        0        0        0 2024-05-03 11:07:29.487428 dsp_tools-7.1.3.post7/src/dsp_tools/commands/excel2json/models/__init__.py
--rw-r--r--   0        0        0     8065 2024-05-03 11:07:29.487428 dsp_tools-7.1.3.post7/src/dsp_tools/commands/excel2json/models/input_error.py
--rw-r--r--   0        0        0      501 2024-05-03 11:07:29.487428 dsp_tools-7.1.3.post7/src/dsp_tools/commands/excel2json/models/list_node_name.py
--rw-r--r--   0        0        0     6313 2024-05-03 11:07:29.487428 dsp_tools-7.1.3.post7/src/dsp_tools/commands/excel2json/project.py
--rw-r--r--   0        0        0    13717 2024-05-03 11:07:29.487428 dsp_tools-7.1.3.post7/src/dsp_tools/commands/excel2json/properties.py
--rw-r--r--   0        0        0    11887 2024-05-03 11:07:29.487428 dsp_tools-7.1.3.post7/src/dsp_tools/commands/excel2json/resources.py
--rw-r--r--   0        0        0    11866 2024-05-03 11:07:29.487428 dsp_tools-7.1.3.post7/src/dsp_tools/commands/excel2json/utils.py
--rw-r--r--   0        0        0      466 2024-05-03 11:07:29.487428 dsp_tools-7.1.3.post7/src/dsp_tools/commands/excel2xml/__init__.py
--rw-r--r--   0        0        0    21324 2024-05-03 11:07:29.487428 dsp_tools-7.1.3.post7/src/dsp_tools/commands/excel2xml/excel2xml_cli.py
--rw-r--r--   0        0        0    76416 2024-05-03 11:07:29.487428 dsp_tools-7.1.3.post7/src/dsp_tools/commands/excel2xml/excel2xml_lib.py
--rw-r--r--   0        0        0     1981 2024-05-03 11:07:29.487428 dsp_tools-7.1.3.post7/src/dsp_tools/commands/excel2xml/propertyelement.py
--rw-r--r--   0        0        0     8275 2024-05-03 11:07:29.487428 dsp_tools-7.1.3.post7/src/dsp_tools/commands/id2iri.py
--rw-r--r--   0        0        0        0 2024-05-03 11:07:29.487428 dsp_tools-7.1.3.post7/src/dsp_tools/commands/ingest_xmlupload/__init__.py
--rw-r--r--   0        0        0     2876 2024-05-03 11:07:29.487428 dsp_tools-7.1.3.post7/src/dsp_tools/commands/ingest_xmlupload/apply_ingest_id.py
--rw-r--r--   0        0        0     2351 2024-05-03 11:07:29.487428 dsp_tools-7.1.3.post7/src/dsp_tools/commands/ingest_xmlupload/upload_xml.py
--rw-r--r--   0        0        0     4891 2024-05-03 11:07:29.487428 dsp_tools-7.1.3.post7/src/dsp_tools/commands/ingest_xmlupload/user_information.py
--rw-r--r--   0        0        0        0 2024-05-03 11:07:29.487428 dsp_tools-7.1.3.post7/src/dsp_tools/commands/project/__init__.py
--rw-r--r--   0        0        0        0 2024-05-03 11:07:29.487428 dsp_tools-7.1.3.post7/src/dsp_tools/commands/project/create/__init__.py
--rw-r--r--   0        0        0    45642 2024-05-03 11:07:29.487428 dsp_tools-7.1.3.post7/src/dsp_tools/commands/project/create/project_create.py
--rw-r--r--   0        0        0     8243 2024-05-03 11:07:29.487428 dsp_tools-7.1.3.post7/src/dsp_tools/commands/project/create/project_create_lists.py
--rw-r--r--   0        0        0    21069 2024-05-03 11:07:29.487428 dsp_tools-7.1.3.post7/src/dsp_tools/commands/project/create/project_validate.py
--rw-r--r--   0        0        0     5743 2024-05-03 11:07:29.487428 dsp_tools-7.1.3.post7/src/dsp_tools/commands/project/get.py
--rw-r--r--   0        0        0        0 2024-05-03 11:07:29.487428 dsp_tools-7.1.3.post7/src/dsp_tools/commands/project/models/__init__.py
--rw-r--r--   0        0        0    12173 2024-05-03 11:07:29.487428 dsp_tools-7.1.3.post7/src/dsp_tools/commands/project/models/context.py
--rw-r--r--   0        0        0     8379 2024-05-03 11:07:29.487428 dsp_tools-7.1.3.post7/src/dsp_tools/commands/project/models/group.py
--rw-r--r--   0        0        0      850 2024-05-03 11:07:29.487428 dsp_tools-7.1.3.post7/src/dsp_tools/commands/project/models/helpers.py
--rw-r--r--   0        0        0    14910 2024-05-03 11:07:29.487428 dsp_tools-7.1.3.post7/src/dsp_tools/commands/project/models/listnode.py
--rw-r--r--   0        0        0      245 2024-05-03 11:07:29.487428 dsp_tools-7.1.3.post7/src/dsp_tools/commands/project/models/model.py
--rw-r--r--   0        0        0    12710 2024-05-03 11:07:29.487428 dsp_tools-7.1.3.post7/src/dsp_tools/commands/project/models/ontology.py
--rw-r--r--   0        0        0    11594 2024-05-03 11:07:29.487428 dsp_tools-7.1.3.post7/src/dsp_tools/commands/project/models/project.py
--rw-r--r--   0        0        0      306 2024-05-03 11:07:29.487428 dsp_tools-7.1.3.post7/src/dsp_tools/commands/project/models/project_definition.py
--rw-r--r--   0        0        0    17215 2024-05-03 11:07:29.487428 dsp_tools-7.1.3.post7/src/dsp_tools/commands/project/models/propertyclass.py
--rw-r--r--   0        0        0    28334 2024-05-03 11:07:29.491428 dsp_tools-7.1.3.post7/src/dsp_tools/commands/project/models/resourceclass.py
--rw-r--r--   0        0        0    17030 2024-05-03 11:07:29.491428 dsp_tools-7.1.3.post7/src/dsp_tools/commands/project/models/user.py
--rw-r--r--   0        0        0        0 2024-05-03 11:07:29.491428 dsp_tools-7.1.3.post7/src/dsp_tools/commands/resume_xmlupload/__init__.py
--rw-r--r--   0        0        0     4200 2024-05-03 11:07:29.491428 dsp_tools-7.1.3.post7/src/dsp_tools/commands/resume_xmlupload/resume_xmlupload.py
--rw-r--r--   0        0        0     4177 2024-05-03 11:07:29.491428 dsp_tools-7.1.3.post7/src/dsp_tools/commands/rosetta.py
--rw-r--r--   0        0        0    16102 2024-05-03 11:07:29.491428 dsp_tools-7.1.3.post7/src/dsp_tools/commands/start_stack.py
--rw-r--r--   0        0        0     1134 2024-05-03 11:07:29.491428 dsp_tools-7.1.3.post7/src/dsp_tools/commands/template.py
--rw-r--r--   0        0        0        0 2024-05-03 11:07:29.491428 dsp_tools-7.1.3.post7/src/dsp_tools/commands/xmlupload/__init__.py
--rw-r--r--   0        0        0     2350 2024-05-03 11:07:29.491428 dsp_tools-7.1.3.post7/src/dsp_tools/commands/xmlupload/ark2iri.py
--rw-r--r--   0        0        0    10356 2024-05-03 11:07:29.491428 dsp_tools-7.1.3.post7/src/dsp_tools/commands/xmlupload/check_consistency_with_ontology.py
--rw-r--r--   0        0        0      625 2024-05-03 11:07:29.491428 dsp_tools-7.1.3.post7/src/dsp_tools/commands/xmlupload/iri_resolver.py
--rw-r--r--   0        0        0     3587 2024-05-03 11:07:29.491428 dsp_tools-7.1.3.post7/src/dsp_tools/commands/xmlupload/list_client.py
--rw-r--r--   0        0        0        0 2024-05-03 11:07:29.491428 dsp_tools-7.1.3.post7/src/dsp_tools/commands/xmlupload/models/__init__.py
--rw-r--r--   0        0        0     1334 2024-05-03 11:07:29.491428 dsp_tools-7.1.3.post7/src/dsp_tools/commands/xmlupload/models/formatted_text_value.py
--rw-r--r--   0        0        0     5428 2024-05-03 11:07:29.491428 dsp_tools-7.1.3.post7/src/dsp_tools/commands/xmlupload/models/ontology_lookup_models.py
--rw-r--r--   0        0        0     6752 2024-05-03 11:07:29.491428 dsp_tools-7.1.3.post7/src/dsp_tools/commands/xmlupload/models/ontology_problem_models.py
--rw-r--r--   0        0        0     2388 2024-05-03 11:07:29.491428 dsp_tools-7.1.3.post7/src/dsp_tools/commands/xmlupload/models/permission.py
--rw-r--r--   0        0        0      812 2024-05-03 11:07:29.491428 dsp_tools-7.1.3.post7/src/dsp_tools/commands/xmlupload/models/sipi.py
--rw-r--r--   0        0        0      675 2024-05-03 11:07:29.491428 dsp_tools-7.1.3.post7/src/dsp_tools/commands/xmlupload/models/upload_state.py
--rw-r--r--   0        0        0     2236 2024-05-03 11:07:29.491428 dsp_tools-7.1.3.post7/src/dsp_tools/commands/xmlupload/models/xmlallow.py
--rw-r--r--   0        0        0      548 2024-05-03 11:07:29.491428 dsp_tools-7.1.3.post7/src/dsp_tools/commands/xmlupload/models/xmlbitstream.py
--rw-r--r--   0        0        0     1437 2024-05-03 11:07:29.491428 dsp_tools-7.1.3.post7/src/dsp_tools/commands/xmlupload/models/xmlpermission.py
--rw-r--r--   0        0        0     2026 2024-05-03 11:07:29.491428 dsp_tools-7.1.3.post7/src/dsp_tools/commands/xmlupload/models/xmlproperty.py
--rw-r--r--   0        0        0     5164 2024-05-03 11:07:29.491428 dsp_tools-7.1.3.post7/src/dsp_tools/commands/xmlupload/models/xmlresource.py
--rw-r--r--   0        0        0     4004 2024-05-03 11:07:29.491428 dsp_tools-7.1.3.post7/src/dsp_tools/commands/xmlupload/models/xmlvalue.py
--rw-r--r--   0        0        0     3466 2024-05-03 11:07:29.491428 dsp_tools-7.1.3.post7/src/dsp_tools/commands/xmlupload/ontology_client.py
--rw-r--r--   0        0        0     3063 2024-05-03 11:07:29.491428 dsp_tools-7.1.3.post7/src/dsp_tools/commands/xmlupload/project_client.py
--rw-r--r--   0        0        0     4653 2024-05-03 11:07:29.491428 dsp_tools-7.1.3.post7/src/dsp_tools/commands/xmlupload/read_validate_xml_file.py
--rw-r--r--   0        0        0    13023 2024-05-03 11:07:29.491428 dsp_tools-7.1.3.post7/src/dsp_tools/commands/xmlupload/resource_create_client.py
--rw-r--r--   0        0        0     4585 2024-05-03 11:07:29.491428 dsp_tools-7.1.3.post7/src/dsp_tools/commands/xmlupload/resource_multimedia.py
--rw-r--r--   0        0        0        0 2024-05-03 11:07:29.491428 dsp_tools-7.1.3.post7/src/dsp_tools/commands/xmlupload/stash/__init__.py
--rw-r--r--   0        0        0    12372 2024-05-03 11:07:29.491428 dsp_tools-7.1.3.post7/src/dsp_tools/commands/xmlupload/stash/construct_and_analyze_graph.py
--rw-r--r--   0        0        0     2452 2024-05-03 11:07:29.491428 dsp_tools-7.1.3.post7/src/dsp_tools/commands/xmlupload/stash/graph_models.py
--rw-r--r--   0        0        0     5724 2024-05-03 11:07:29.491428 dsp_tools-7.1.3.post7/src/dsp_tools/commands/xmlupload/stash/stash_circular_references.py
--rw-r--r--   0        0        0     3068 2024-05-03 11:07:29.491428 dsp_tools-7.1.3.post7/src/dsp_tools/commands/xmlupload/stash/stash_models.py
--rw-r--r--   0        0        0     4237 2024-05-03 11:07:29.491428 dsp_tools-7.1.3.post7/src/dsp_tools/commands/xmlupload/stash/upload_stashed_resptr_props.py
--rw-r--r--   0        0        0     7727 2024-05-03 11:07:29.491428 dsp_tools-7.1.3.post7/src/dsp_tools/commands/xmlupload/stash/upload_stashed_xml_texts.py
--rw-r--r--   0        0        0     2175 2024-05-03 11:07:29.491428 dsp_tools-7.1.3.post7/src/dsp_tools/commands/xmlupload/upload_config.py
--rw-r--r--   0        0        0      858 2024-05-03 11:07:29.491428 dsp_tools-7.1.3.post7/src/dsp_tools/commands/xmlupload/write_diagnostic_info.py
--rw-r--r--   0        0        0    22379 2024-05-03 11:07:29.491428 dsp_tools-7.1.3.post7/src/dsp_tools/commands/xmlupload/xmlupload.py
--rw-r--r--   0        0        0        0 2024-05-03 11:07:29.491428 dsp_tools-7.1.3.post7/src/dsp_tools/models/__init__.py
--rw-r--r--   0        0        0      949 2024-05-03 11:07:29.491428 dsp_tools-7.1.3.post7/src/dsp_tools/models/custom_warnings.py
--rw-r--r--   0        0        0     2876 2024-05-03 11:07:29.491428 dsp_tools-7.1.3.post7/src/dsp_tools/models/datetimestamp.py
--rw-r--r--   0        0        0     2510 2024-05-03 11:07:29.491428 dsp_tools-7.1.3.post7/src/dsp_tools/models/exceptions.py
--rw-r--r--   0        0        0     8457 2024-05-03 11:07:29.491428 dsp_tools-7.1.3.post7/src/dsp_tools/models/langstring.py
--rw-r--r--   0        0        0     1777 2024-05-03 11:07:29.491428 dsp_tools-7.1.3.post7/src/dsp_tools/models/projectContext.py
--rw-r--r--   0        0        0        0 2024-05-03 11:07:29.491428 dsp_tools-7.1.3.post7/src/dsp_tools/py.typed
--rw-r--r--   0        0        0     1488 2024-05-03 11:07:29.491428 dsp_tools-7.1.3.post7/src/dsp_tools/resources/0100-template-repo/template.json
--rw-r--r--   0        0        0     1036 2024-05-03 11:07:29.491428 dsp_tools-7.1.3.post7/src/dsp_tools/resources/0100-template-repo/template.xml
--rw-r--r--   0        0        0    24361 2024-05-03 11:07:29.491428 dsp_tools-7.1.3.post7/src/dsp_tools/resources/schema/data.xsd
--rw-r--r--   0        0        0     2770 2024-05-03 11:07:29.491428 dsp_tools-7.1.3.post7/src/dsp_tools/resources/schema/lists-only.json
--rw-r--r--   0        0        0    44347 2024-05-03 11:07:29.495428 dsp_tools-7.1.3.post7/src/dsp_tools/resources/schema/project.json
--rw-r--r--   0        0        0    33977 2024-05-03 11:07:29.495428 dsp_tools-7.1.3.post7/src/dsp_tools/resources/schema/properties-only.json
--rw-r--r--   0        0        0     4341 2024-05-03 11:07:29.495428 dsp_tools-7.1.3.post7/src/dsp_tools/resources/schema/resources-only.json
--rw-r--r--   0        0        0       61 2024-05-03 11:07:29.495428 dsp_tools-7.1.3.post7/src/dsp_tools/resources/start-stack/docker-compose.override.yml
--rw-r--r--   0        0        0     3281 2024-05-03 11:07:29.495428 dsp_tools-7.1.3.post7/src/dsp_tools/resources/start-stack/docker-compose.yml
--rw-r--r--   0        0        0      164 2024-05-03 11:07:29.495428 dsp_tools-7.1.3.post7/src/dsp_tools/resources/start-stack/start-stack-config.yml
--rw-r--r--   0        0        0        0 2024-05-03 11:07:29.495428 dsp_tools-7.1.3.post7/src/dsp_tools/utils/__init__.py
--rw-r--r--   0        0        0     1030 2024-05-03 11:07:29.495428 dsp_tools-7.1.3.post7/src/dsp_tools/utils/connection.py
--rw-r--r--   0        0        0    14126 2024-05-03 11:07:29.495428 dsp_tools-7.1.3.post7/src/dsp_tools/utils/connection_live.py
--rw-r--r--   0        0        0     4554 2024-05-03 11:07:29.495428 dsp_tools-7.1.3.post7/src/dsp_tools/utils/date_util.py
--rw-r--r--   0        0        0      457 2024-05-03 11:07:29.495428 dsp_tools-7.1.3.post7/src/dsp_tools/utils/iri_util.py
--rw-r--r--   0        0        0      893 2024-05-03 11:07:29.495428 dsp_tools-7.1.3.post7/src/dsp_tools/utils/json_ld_util.py
--rw-r--r--   0        0        0     1157 2024-05-03 11:07:29.495428 dsp_tools-7.1.3.post7/src/dsp_tools/utils/logger_config.py
--rw-r--r--   0        0        0      705 2024-05-03 11:07:29.495428 dsp_tools-7.1.3.post7/src/dsp_tools/utils/set_encoder.py
--rw-r--r--   0        0        0     5754 2024-05-03 11:07:29.495428 dsp_tools-7.1.3.post7/src/dsp_tools/utils/shared.py
--rw-r--r--   0        0        0      547 2024-05-03 11:07:29.495428 dsp_tools-7.1.3.post7/src/dsp_tools/utils/uri_util.py
--rw-r--r--   0        0        0      978 2024-05-03 11:07:29.495428 dsp_tools-7.1.3.post7/src/dsp_tools/utils/warnings_config.py
--rw-r--r--   0        0        0     4464 2024-05-03 11:07:29.495428 dsp_tools-7.1.3.post7/src/dsp_tools/utils/xml_utils.py
--rw-r--r--   0        0        0     8198 2024-05-03 11:07:29.495428 dsp_tools-7.1.3.post7/src/dsp_tools/utils/xml_validation.py
--rw-r--r--   0        0        0     2312 2024-05-03 11:07:29.495428 dsp_tools-7.1.3.post7/src/dsp_tools/utils/xml_validation_models.py
--rw-r--r--   0        0        0     6312 1970-01-01 00:00:00.000000 dsp_tools-7.1.3.post7/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-05-08 06:43:46.797018 dsp_tools-7.1.3.post9/LICENSE
+-rw-r--r--   0        0        0     4941 2024-05-08 06:43:46.813018 dsp_tools-7.1.3.post9/docs/index.md
+-rw-r--r--   0        0        0     8372 2024-05-08 06:44:15.437113 dsp_tools-7.1.3.post9/pyproject.toml
+-rw-r--r--   0        0        0       41 2024-05-08 06:43:46.813018 dsp_tools-7.1.3.post9/src/dsp_tools/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-08 06:43:46.813018 dsp_tools-7.1.3.post9/src/dsp_tools/cli/__init__.py
+-rw-r--r--   0        0        0     8102 2024-05-08 06:43:46.813018 dsp_tools-7.1.3.post9/src/dsp_tools/cli/call_action.py
+-rw-r--r--   0        0        0    13719 2024-05-08 06:43:46.813018 dsp_tools-7.1.3.post9/src/dsp_tools/cli/create_parsers.py
+-rw-r--r--   0        0        0     9909 2024-05-08 06:43:46.813018 dsp_tools-7.1.3.post9/src/dsp_tools/cli/entry_point.py
+-rw-r--r--   0        0        0        0 2024-05-08 06:43:46.813018 dsp_tools-7.1.3.post9/src/dsp_tools/commands/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-08 06:43:46.813018 dsp_tools-7.1.3.post9/src/dsp_tools/commands/excel2json/__init__.py
+-rw-r--r--   0        0        0    15987 2024-05-08 06:43:46.813018 dsp_tools-7.1.3.post9/src/dsp_tools/commands/excel2json/lists.py
+-rw-r--r--   0        0        0        0 2024-05-08 06:43:46.813018 dsp_tools-7.1.3.post9/src/dsp_tools/commands/excel2json/models/__init__.py
+-rw-r--r--   0        0        0    14898 2024-05-08 06:43:46.813018 dsp_tools-7.1.3.post9/src/dsp_tools/commands/excel2json/models/input_error.py
+-rw-r--r--   0        0        0     4018 2024-05-08 06:43:46.813018 dsp_tools-7.1.3.post9/src/dsp_tools/commands/excel2json/models/list_node.py
+-rw-r--r--   0        0        0      501 2024-05-08 06:43:46.813018 dsp_tools-7.1.3.post9/src/dsp_tools/commands/excel2json/models/list_node_name.py
+-rw-r--r--   0        0        0    29990 2024-05-08 06:43:46.813018 dsp_tools-7.1.3.post9/src/dsp_tools/commands/excel2json/new_lists.py
+-rw-r--r--   0        0        0     9829 2024-05-08 06:43:46.813018 dsp_tools-7.1.3.post9/src/dsp_tools/commands/excel2json/project.py
+-rw-r--r--   0        0        0    13717 2024-05-08 06:43:46.813018 dsp_tools-7.1.3.post9/src/dsp_tools/commands/excel2json/properties.py
+-rw-r--r--   0        0        0    11887 2024-05-08 06:43:46.813018 dsp_tools-7.1.3.post9/src/dsp_tools/commands/excel2json/resources.py
+-rw-r--r--   0        0        0    11866 2024-05-08 06:43:46.813018 dsp_tools-7.1.3.post9/src/dsp_tools/commands/excel2json/utils.py
+-rw-r--r--   0        0        0      466 2024-05-08 06:43:46.813018 dsp_tools-7.1.3.post9/src/dsp_tools/commands/excel2xml/__init__.py
+-rw-r--r--   0        0        0    21324 2024-05-08 06:43:46.813018 dsp_tools-7.1.3.post9/src/dsp_tools/commands/excel2xml/excel2xml_cli.py
+-rw-r--r--   0        0        0    76416 2024-05-08 06:43:46.817018 dsp_tools-7.1.3.post9/src/dsp_tools/commands/excel2xml/excel2xml_lib.py
+-rw-r--r--   0        0        0     1981 2024-05-08 06:43:46.817018 dsp_tools-7.1.3.post9/src/dsp_tools/commands/excel2xml/propertyelement.py
+-rw-r--r--   0        0        0     8275 2024-05-08 06:43:46.817018 dsp_tools-7.1.3.post9/src/dsp_tools/commands/id2iri.py
+-rw-r--r--   0        0        0        0 2024-05-08 06:43:46.817018 dsp_tools-7.1.3.post9/src/dsp_tools/commands/ingest_xmlupload/__init__.py
+-rw-r--r--   0        0        0     2876 2024-05-08 06:43:46.817018 dsp_tools-7.1.3.post9/src/dsp_tools/commands/ingest_xmlupload/apply_ingest_id.py
+-rw-r--r--   0        0        0     2351 2024-05-08 06:43:46.817018 dsp_tools-7.1.3.post9/src/dsp_tools/commands/ingest_xmlupload/upload_xml.py
+-rw-r--r--   0        0        0     4891 2024-05-08 06:43:46.817018 dsp_tools-7.1.3.post9/src/dsp_tools/commands/ingest_xmlupload/user_information.py
+-rw-r--r--   0        0        0        0 2024-05-08 06:43:46.817018 dsp_tools-7.1.3.post9/src/dsp_tools/commands/project/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-08 06:43:46.817018 dsp_tools-7.1.3.post9/src/dsp_tools/commands/project/create/__init__.py
+-rw-r--r--   0        0        0    45642 2024-05-08 06:43:46.817018 dsp_tools-7.1.3.post9/src/dsp_tools/commands/project/create/project_create.py
+-rw-r--r--   0        0        0     8243 2024-05-08 06:43:46.817018 dsp_tools-7.1.3.post9/src/dsp_tools/commands/project/create/project_create_lists.py
+-rw-r--r--   0        0        0    21069 2024-05-08 06:43:46.817018 dsp_tools-7.1.3.post9/src/dsp_tools/commands/project/create/project_validate.py
+-rw-r--r--   0        0        0     5743 2024-05-08 06:43:46.817018 dsp_tools-7.1.3.post9/src/dsp_tools/commands/project/get.py
+-rw-r--r--   0        0        0        0 2024-05-08 06:43:46.817018 dsp_tools-7.1.3.post9/src/dsp_tools/commands/project/models/__init__.py
+-rw-r--r--   0        0        0    12173 2024-05-08 06:43:46.817018 dsp_tools-7.1.3.post9/src/dsp_tools/commands/project/models/context.py
+-rw-r--r--   0        0        0     8379 2024-05-08 06:43:46.817018 dsp_tools-7.1.3.post9/src/dsp_tools/commands/project/models/group.py
+-rw-r--r--   0        0        0      850 2024-05-08 06:43:46.817018 dsp_tools-7.1.3.post9/src/dsp_tools/commands/project/models/helpers.py
+-rw-r--r--   0        0        0    14910 2024-05-08 06:43:46.817018 dsp_tools-7.1.3.post9/src/dsp_tools/commands/project/models/listnode.py
+-rw-r--r--   0        0        0      245 2024-05-08 06:43:46.817018 dsp_tools-7.1.3.post9/src/dsp_tools/commands/project/models/model.py
+-rw-r--r--   0        0        0    12710 2024-05-08 06:43:46.817018 dsp_tools-7.1.3.post9/src/dsp_tools/commands/project/models/ontology.py
+-rw-r--r--   0        0        0    11594 2024-05-08 06:43:46.817018 dsp_tools-7.1.3.post9/src/dsp_tools/commands/project/models/project.py
+-rw-r--r--   0        0        0      306 2024-05-08 06:43:46.817018 dsp_tools-7.1.3.post9/src/dsp_tools/commands/project/models/project_definition.py
+-rw-r--r--   0        0        0    17215 2024-05-08 06:43:46.817018 dsp_tools-7.1.3.post9/src/dsp_tools/commands/project/models/propertyclass.py
+-rw-r--r--   0        0        0    28334 2024-05-08 06:43:46.817018 dsp_tools-7.1.3.post9/src/dsp_tools/commands/project/models/resourceclass.py
+-rw-r--r--   0        0        0    17030 2024-05-08 06:43:46.817018 dsp_tools-7.1.3.post9/src/dsp_tools/commands/project/models/user.py
+-rw-r--r--   0        0        0        0 2024-05-08 06:43:46.817018 dsp_tools-7.1.3.post9/src/dsp_tools/commands/resume_xmlupload/__init__.py
+-rw-r--r--   0        0        0     4200 2024-05-08 06:43:46.817018 dsp_tools-7.1.3.post9/src/dsp_tools/commands/resume_xmlupload/resume_xmlupload.py
+-rw-r--r--   0        0        0     4177 2024-05-08 06:43:46.817018 dsp_tools-7.1.3.post9/src/dsp_tools/commands/rosetta.py
+-rw-r--r--   0        0        0    16102 2024-05-08 06:43:46.817018 dsp_tools-7.1.3.post9/src/dsp_tools/commands/start_stack.py
+-rw-r--r--   0        0        0     1134 2024-05-08 06:43:46.817018 dsp_tools-7.1.3.post9/src/dsp_tools/commands/template.py
+-rw-r--r--   0        0        0        0 2024-05-08 06:43:46.817018 dsp_tools-7.1.3.post9/src/dsp_tools/commands/xmlupload/__init__.py
+-rw-r--r--   0        0        0     2350 2024-05-08 06:43:46.817018 dsp_tools-7.1.3.post9/src/dsp_tools/commands/xmlupload/ark2iri.py
+-rw-r--r--   0        0        0    10356 2024-05-08 06:43:46.817018 dsp_tools-7.1.3.post9/src/dsp_tools/commands/xmlupload/check_consistency_with_ontology.py
+-rw-r--r--   0        0        0      625 2024-05-08 06:43:46.817018 dsp_tools-7.1.3.post9/src/dsp_tools/commands/xmlupload/iri_resolver.py
+-rw-r--r--   0        0        0     3587 2024-05-08 06:43:46.817018 dsp_tools-7.1.3.post9/src/dsp_tools/commands/xmlupload/list_client.py
+-rw-r--r--   0        0        0        0 2024-05-08 06:43:46.817018 dsp_tools-7.1.3.post9/src/dsp_tools/commands/xmlupload/models/__init__.py
+-rw-r--r--   0        0        0     1334 2024-05-08 06:43:46.817018 dsp_tools-7.1.3.post9/src/dsp_tools/commands/xmlupload/models/formatted_text_value.py
+-rw-r--r--   0        0        0     5428 2024-05-08 06:43:46.817018 dsp_tools-7.1.3.post9/src/dsp_tools/commands/xmlupload/models/ontology_lookup_models.py
+-rw-r--r--   0        0        0     6752 2024-05-08 06:43:46.817018 dsp_tools-7.1.3.post9/src/dsp_tools/commands/xmlupload/models/ontology_problem_models.py
+-rw-r--r--   0        0        0     2388 2024-05-08 06:43:46.817018 dsp_tools-7.1.3.post9/src/dsp_tools/commands/xmlupload/models/permission.py
+-rw-r--r--   0        0        0      812 2024-05-08 06:43:46.817018 dsp_tools-7.1.3.post9/src/dsp_tools/commands/xmlupload/models/sipi.py
+-rw-r--r--   0        0        0      675 2024-05-08 06:43:46.817018 dsp_tools-7.1.3.post9/src/dsp_tools/commands/xmlupload/models/upload_state.py
+-rw-r--r--   0        0        0     2236 2024-05-08 06:43:46.817018 dsp_tools-7.1.3.post9/src/dsp_tools/commands/xmlupload/models/xmlallow.py
+-rw-r--r--   0        0        0      548 2024-05-08 06:43:46.817018 dsp_tools-7.1.3.post9/src/dsp_tools/commands/xmlupload/models/xmlbitstream.py
+-rw-r--r--   0        0        0     1437 2024-05-08 06:43:46.817018 dsp_tools-7.1.3.post9/src/dsp_tools/commands/xmlupload/models/xmlpermission.py
+-rw-r--r--   0        0        0     2026 2024-05-08 06:43:46.817018 dsp_tools-7.1.3.post9/src/dsp_tools/commands/xmlupload/models/xmlproperty.py
+-rw-r--r--   0        0        0     5164 2024-05-08 06:43:46.817018 dsp_tools-7.1.3.post9/src/dsp_tools/commands/xmlupload/models/xmlresource.py
+-rw-r--r--   0        0        0     4004 2024-05-08 06:43:46.821018 dsp_tools-7.1.3.post9/src/dsp_tools/commands/xmlupload/models/xmlvalue.py
+-rw-r--r--   0        0        0     3466 2024-05-08 06:43:46.821018 dsp_tools-7.1.3.post9/src/dsp_tools/commands/xmlupload/ontology_client.py
+-rw-r--r--   0        0        0     3063 2024-05-08 06:43:46.821018 dsp_tools-7.1.3.post9/src/dsp_tools/commands/xmlupload/project_client.py
+-rw-r--r--   0        0        0     4653 2024-05-08 06:43:46.821018 dsp_tools-7.1.3.post9/src/dsp_tools/commands/xmlupload/read_validate_xml_file.py
+-rw-r--r--   0        0        0    13023 2024-05-08 06:43:46.821018 dsp_tools-7.1.3.post9/src/dsp_tools/commands/xmlupload/resource_create_client.py
+-rw-r--r--   0        0        0     4585 2024-05-08 06:43:46.821018 dsp_tools-7.1.3.post9/src/dsp_tools/commands/xmlupload/resource_multimedia.py
+-rw-r--r--   0        0        0        0 2024-05-08 06:43:46.821018 dsp_tools-7.1.3.post9/src/dsp_tools/commands/xmlupload/stash/__init__.py
+-rw-r--r--   0        0        0    12372 2024-05-08 06:43:46.821018 dsp_tools-7.1.3.post9/src/dsp_tools/commands/xmlupload/stash/construct_and_analyze_graph.py
+-rw-r--r--   0        0        0     2452 2024-05-08 06:43:46.821018 dsp_tools-7.1.3.post9/src/dsp_tools/commands/xmlupload/stash/graph_models.py
+-rw-r--r--   0        0        0     5724 2024-05-08 06:43:46.821018 dsp_tools-7.1.3.post9/src/dsp_tools/commands/xmlupload/stash/stash_circular_references.py
+-rw-r--r--   0        0        0     3068 2024-05-08 06:43:46.821018 dsp_tools-7.1.3.post9/src/dsp_tools/commands/xmlupload/stash/stash_models.py
+-rw-r--r--   0        0        0     4237 2024-05-08 06:43:46.821018 dsp_tools-7.1.3.post9/src/dsp_tools/commands/xmlupload/stash/upload_stashed_resptr_props.py
+-rw-r--r--   0        0        0     7727 2024-05-08 06:43:46.821018 dsp_tools-7.1.3.post9/src/dsp_tools/commands/xmlupload/stash/upload_stashed_xml_texts.py
+-rw-r--r--   0        0        0     2175 2024-05-08 06:43:46.821018 dsp_tools-7.1.3.post9/src/dsp_tools/commands/xmlupload/upload_config.py
+-rw-r--r--   0        0        0      858 2024-05-08 06:43:46.821018 dsp_tools-7.1.3.post9/src/dsp_tools/commands/xmlupload/write_diagnostic_info.py
+-rw-r--r--   0        0        0    22379 2024-05-08 06:43:46.821018 dsp_tools-7.1.3.post9/src/dsp_tools/commands/xmlupload/xmlupload.py
+-rw-r--r--   0        0        0        0 2024-05-08 06:43:46.821018 dsp_tools-7.1.3.post9/src/dsp_tools/models/__init__.py
+-rw-r--r--   0        0        0      949 2024-05-08 06:43:46.821018 dsp_tools-7.1.3.post9/src/dsp_tools/models/custom_warnings.py
+-rw-r--r--   0        0        0     2876 2024-05-08 06:43:46.821018 dsp_tools-7.1.3.post9/src/dsp_tools/models/datetimestamp.py
+-rw-r--r--   0        0        0     2663 2024-05-08 06:43:46.821018 dsp_tools-7.1.3.post9/src/dsp_tools/models/exceptions.py
+-rw-r--r--   0        0        0     8457 2024-05-08 06:43:46.821018 dsp_tools-7.1.3.post9/src/dsp_tools/models/langstring.py
+-rw-r--r--   0        0        0     1777 2024-05-08 06:43:46.821018 dsp_tools-7.1.3.post9/src/dsp_tools/models/projectContext.py
+-rw-r--r--   0        0        0        0 2024-05-08 06:43:46.821018 dsp_tools-7.1.3.post9/src/dsp_tools/py.typed
+-rw-r--r--   0        0        0     1488 2024-05-08 06:43:46.821018 dsp_tools-7.1.3.post9/src/dsp_tools/resources/0100-template-repo/template.json
+-rw-r--r--   0        0        0     1036 2024-05-08 06:43:46.821018 dsp_tools-7.1.3.post9/src/dsp_tools/resources/0100-template-repo/template.xml
+-rw-r--r--   0        0        0    24361 2024-05-08 06:43:46.821018 dsp_tools-7.1.3.post9/src/dsp_tools/resources/schema/data.xsd
+-rw-r--r--   0        0        0     2770 2024-05-08 06:43:46.821018 dsp_tools-7.1.3.post9/src/dsp_tools/resources/schema/lists-only.json
+-rw-r--r--   0        0        0    44347 2024-05-08 06:43:46.821018 dsp_tools-7.1.3.post9/src/dsp_tools/resources/schema/project.json
+-rw-r--r--   0        0        0    33977 2024-05-08 06:43:46.821018 dsp_tools-7.1.3.post9/src/dsp_tools/resources/schema/properties-only.json
+-rw-r--r--   0        0        0     4341 2024-05-08 06:43:46.821018 dsp_tools-7.1.3.post9/src/dsp_tools/resources/schema/resources-only.json
+-rw-r--r--   0        0        0       61 2024-05-08 06:43:46.821018 dsp_tools-7.1.3.post9/src/dsp_tools/resources/start-stack/docker-compose.override.yml
+-rw-r--r--   0        0        0     3281 2024-05-08 06:43:46.821018 dsp_tools-7.1.3.post9/src/dsp_tools/resources/start-stack/docker-compose.yml
+-rw-r--r--   0        0        0      164 2024-05-08 06:43:46.821018 dsp_tools-7.1.3.post9/src/dsp_tools/resources/start-stack/start-stack-config.yml
+-rw-r--r--   0        0        0        0 2024-05-08 06:43:46.821018 dsp_tools-7.1.3.post9/src/dsp_tools/utils/__init__.py
+-rw-r--r--   0        0        0     1030 2024-05-08 06:43:46.821018 dsp_tools-7.1.3.post9/src/dsp_tools/utils/connection.py
+-rw-r--r--   0        0        0    14126 2024-05-08 06:43:46.821018 dsp_tools-7.1.3.post9/src/dsp_tools/utils/connection_live.py
+-rw-r--r--   0        0        0     4554 2024-05-08 06:43:46.821018 dsp_tools-7.1.3.post9/src/dsp_tools/utils/date_util.py
+-rw-r--r--   0        0        0      457 2024-05-08 06:43:46.821018 dsp_tools-7.1.3.post9/src/dsp_tools/utils/iri_util.py
+-rw-r--r--   0        0        0      893 2024-05-08 06:43:46.821018 dsp_tools-7.1.3.post9/src/dsp_tools/utils/json_ld_util.py
+-rw-r--r--   0        0        0     1157 2024-05-08 06:43:46.821018 dsp_tools-7.1.3.post9/src/dsp_tools/utils/logger_config.py
+-rw-r--r--   0        0        0      705 2024-05-08 06:43:46.821018 dsp_tools-7.1.3.post9/src/dsp_tools/utils/set_encoder.py
+-rw-r--r--   0        0        0     5754 2024-05-08 06:43:46.821018 dsp_tools-7.1.3.post9/src/dsp_tools/utils/shared.py
+-rw-r--r--   0        0        0      547 2024-05-08 06:43:46.821018 dsp_tools-7.1.3.post9/src/dsp_tools/utils/uri_util.py
+-rw-r--r--   0        0        0      978 2024-05-08 06:43:46.821018 dsp_tools-7.1.3.post9/src/dsp_tools/utils/warnings_config.py
+-rw-r--r--   0        0        0     4464 2024-05-08 06:43:46.821018 dsp_tools-7.1.3.post9/src/dsp_tools/utils/xml_utils.py
+-rw-r--r--   0        0        0     8198 2024-05-08 06:43:46.821018 dsp_tools-7.1.3.post9/src/dsp_tools/utils/xml_validation.py
+-rw-r--r--   0        0        0     2312 2024-05-08 06:43:46.825018 dsp_tools-7.1.3.post9/src/dsp_tools/utils/xml_validation_models.py
+-rw-r--r--   0        0        0     6312 1970-01-01 00:00:00.000000 dsp_tools-7.1.3.post9/PKG-INFO
```

### Comparing `dsp_tools-7.1.3.post7/LICENSE` & `dsp_tools-7.1.3.post9/LICENSE`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post7/docs/index.md` & `dsp_tools-7.1.3.post9/docs/index.md`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post7/pyproject.toml` & `dsp_tools-7.1.3.post9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # See https://packaging.python.org/en/latest/guides/writing-pyproject-toml/#writing-pyproject-toml
 
 [tool.poetry]
 name = "dsp-tools"
-version = "7.1.3.post7"
+version = "7.1.3.post9"
 description = "DSP-TOOLS is a Python package with a command line interface that helps you interact with a DaSCH service platform (DSP) server."
 authors = ["DaSCH - Swiss National Data and Service Center for the Humanities <info@dasch.swiss>"]
 readme = "docs/index.md"
 license = "GPL-3.0-only"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
```

### Comparing `dsp_tools-7.1.3.post7/src/dsp_tools/cli/call_action.py` & `dsp_tools-7.1.3.post9/src/dsp_tools/cli/call_action.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import argparse
 from pathlib import Path
 
 from loguru import logger
 
 from dsp_tools.commands.excel2json.lists import excel2lists
 from dsp_tools.commands.excel2json.lists import validate_lists_section_with_schema
+from dsp_tools.commands.excel2json.new_lists import new_excel2lists
 from dsp_tools.commands.excel2json.project import excel2json
+from dsp_tools.commands.excel2json.project import new_excel2json
 from dsp_tools.commands.excel2json.properties import excel2properties
 from dsp_tools.commands.excel2json.resources import excel2resources
 from dsp_tools.commands.excel2xml.excel2xml_cli import excel2xml
 from dsp_tools.commands.id2iri import id2iri
 from dsp_tools.commands.ingest_xmlupload.upload_xml import ingest_xmlupload
 from dsp_tools.commands.project.create.project_create import create_project
 from dsp_tools.commands.project.create.project_create_lists import create_lists
@@ -45,16 +47,20 @@
             result = _call_create(args)
         case "xmlupload":
             result = _call_xmlupload(args)
         case "resume-xmlupload":
             result = _call_resume_xmlupload(args)
         case "excel2json":
             result = _call_excel2json(args)
+        case "new-excel2json":
+            result = _call_new_excel2json(args)
         case "excel2lists":
             result = _call_excel2lists(args)
+        case "new-excel2lists":
+            result = _call_new_excel2lists(args)
         case "excel2resources":
             result = _call_excel2resources(args)
         case "excel2properties":
             result = _call_excel2properties(args)
         case "id2iri":
             result = _call_id2iri(args)
         case "excel2xml":
@@ -125,14 +131,22 @@
     _, success = excel2resources(
         excelfile=args.excelfile,
         path_to_output_file=args.resources_section,
     )
     return success
 
 
+def _call_new_excel2lists(args: argparse.Namespace) -> bool:
+    _, success = new_excel2lists(
+        excelfolder=args.excelfolder,
+        path_to_output_file=args.lists_section,
+    )
+    return success
+
+
 def _call_excel2lists(args: argparse.Namespace) -> bool:
     _, success = excel2lists(
         excelfolder=args.excelfolder,
         path_to_output_file=args.lists_section,
         verbose=args.verbose,
     )
     return success
@@ -141,14 +155,21 @@
 def _call_excel2json(args: argparse.Namespace) -> bool:
     return excel2json(
         data_model_files=args.excelfolder,
         path_to_output_file=args.project_definition,
     )
 
 
+def _call_new_excel2json(args: argparse.Namespace) -> bool:
+    return new_excel2json(
+        data_model_files=args.excelfolder,
+        path_to_output_file=args.project_definition,
+    )
+
+
 def _call_ingest_xmlupload(args: argparse.Namespace) -> bool:
     interrupt_after = args.interrupt_after if args.interrupt_after > 0 else None
     ingest_xmlupload(
         xml_file=Path(args.xml_file),
         user=args.user,
         password=args.password,
         dsp_url=args.server,
```

### Comparing `dsp_tools-7.1.3.post7/src/dsp_tools/cli/create_parsers.py` & `dsp_tools-7.1.3.post9/src/dsp_tools/cli/create_parsers.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,16 +46,18 @@
 
     _add_xmlupload(subparsers, default_dsp_api_url, root_user_email, root_user_pw)
 
     _add_resume_xmlupload(subparsers, default_dsp_api_url, root_user_email, root_user_pw)
 
     _add_ingest_xmlupload(subparsers, default_dsp_api_url, root_user_email, root_user_pw)
 
+    _add_new_excel2json(subparsers)
     _add_excel2json(subparsers)
 
+    _add_new_excel2lists(subparsers)
     _add_excel2lists(subparsers)
 
     _add_excel2resources(subparsers)
 
     _add_excel2properties(subparsers)
 
     _add_excel2xml(subparsers)
@@ -157,14 +159,24 @@
         help="Create the 'resources' section of a JSON project file from one or multiple Excel files",
     )
     subparser.set_defaults(action="excel2resources")
     subparser.add_argument("excelfile", help="path to the Excel file containing the resources")
     subparser.add_argument("resources_section", help="path to the output JSON file containing the 'resources' section")
 
 
+def _add_new_excel2lists(subparsers: _SubParsersAction[ArgumentParser]) -> None:
+    subparser = subparsers.add_parser(
+        name="new-excel2lists",
+        help="Create the 'lists' section of a JSON project file from one or multiple Excel files",
+    )
+    subparser.set_defaults(action="new-excel2lists")
+    subparser.add_argument("excelfolder", help="path to the folder containing the Excel file(s)")
+    subparser.add_argument("lists_section", help="path to the output JSON file containing the 'lists' section")
+
+
 def _add_excel2lists(subparsers: _SubParsersAction[ArgumentParser]) -> None:
     subparser = subparsers.add_parser(
         name="excel2lists",
         help="Create the 'lists' section of a JSON project file from one or multiple Excel files",
     )
     subparser.set_defaults(action="excel2lists")
     subparser.add_argument("-v", "--verbose", action="store_true", help=verbose_text)
@@ -178,14 +190,24 @@
         help="Create an entire JSON project file from a folder containing the required Excel files",
     )
     subparser.set_defaults(action="excel2json")
     subparser.add_argument("excelfolder", help="path to the folder containing the Excel files")
     subparser.add_argument("project_definition", help="path to the output JSON file")
 
 
+def _add_new_excel2json(subparsers: _SubParsersAction[ArgumentParser]) -> None:
+    subparser = subparsers.add_parser(
+        name="new-excel2json",
+        help="Create an entire JSON project file from a folder containing the required Excel files",
+    )
+    subparser.set_defaults(action="new-excel2json")
+    subparser.add_argument("excelfolder", help="path to the folder containing the Excel files")
+    subparser.add_argument("project_definition", help="path to the output JSON file")
+
+
 def _add_ingest_xmlupload(
     subparsers: _SubParsersAction[ArgumentParser],
     default_dsp_api_url: str,
     root_user_email: str,
     root_user_pw: str,
 ) -> None:
     subparser = subparsers.add_parser(
```

### Comparing `dsp_tools-7.1.3.post7/src/dsp_tools/cli/entry_point.py` & `dsp_tools-7.1.3.post9/src/dsp_tools/cli/entry_point.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post7/src/dsp_tools/commands/excel2json/lists.py` & `dsp_tools-7.1.3.post9/src/dsp_tools/commands/excel2json/lists.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post7/src/dsp_tools/commands/excel2json/project.py` & `dsp_tools-7.1.3.post9/src/dsp_tools/commands/excel2json/project.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import json
 from pathlib import Path
 from typing import Any
 
 import regex
 
 from dsp_tools.commands.excel2json.lists import excel2lists
+from dsp_tools.commands.excel2json.new_lists import new_excel2lists
 from dsp_tools.commands.excel2json.properties import excel2properties
 from dsp_tools.commands.excel2json.resources import excel2resources
 from dsp_tools.models.exceptions import UserError
 
 
 def excel2json(
     data_model_files: str,
@@ -55,15 +56,15 @@
 
 
 def _validate_folder_structure_get_filenames(data_model_files: str) -> tuple[list[Path], list[Path]]:
     if not Path(data_model_files).is_dir():
         raise UserError(f"ERROR: {data_model_files} is not a directory.")
     folder = [x for x in Path(data_model_files).glob("*") if _non_hidden(x)]
     processed_files = []
-    onto_folders, processed_onto = _get_validate_onto_folder(data_model_files, folder)
+    onto_folders, processed_onto = _get_and_validate_onto_folder(Path(data_model_files), folder)
     processed_files.extend(processed_onto)
     listfolder, processed_lists = _get_validate_list_folder(data_model_files, folder)
     processed_files.extend(processed_lists)
     if len(onto_folders) + len(listfolder) != len(folder):
         raise UserError(
             f"The only allowed subfolders in '{data_model_files}' are 'lists' "
             "and folders that match the pattern 'onto_name (onto_label)'"
@@ -82,15 +83,72 @@
             raise UserError(
                 f"The only files allowed in '{data_model_files}/lists' are en.xlsx, de.xlsx, fr.xlsx, it.xlsx, rm.xlsx"
             )
         processed_files = [f"{data_model_files}/lists/{file.name}" for file in listfolder_contents]
     return listfolder, processed_files
 
 
-def _get_validate_onto_folder(data_model_files: str, folder: list[Path]) -> tuple[list[Path], list[str]]:
+def new_excel2json(
+    data_model_files: str,
+    path_to_output_file: str,
+) -> bool:
+    """
+    Converts a folder containing Excel files into a JSON data model file. The folder must be structured like this:
+
+    ::
+
+        data_model_files
+        |-- lists
+        |   |-- list.xlsx
+        |   `-- list_2.xlsx
+        `-- onto_name (onto_label)
+            |-- properties.xlsx
+            `-- resources.xlsx
+
+    The names of the files must be exactly like in the example. The folder "lists" can be missing, because it is
+    optional to have lists in a DSP project. Only XLSX files are allowed.
+
+    Args:
+        data_model_files: path to the folder (called "data_model_files" in the example)
+        path_to_output_file: path to the file where the output JSON file will be saved
+
+    Raises:
+        InputError: if something went wrong
+
+    Returns:
+        True if everything went well
+    """
+
+    listfolder, onto_folders = _new_validate_folder_structure_and_get_filenames(Path(data_model_files))
+
+    overall_success, project = _new_create_project_json(data_model_files, onto_folders, listfolder)
+
+    with open(path_to_output_file, "w", encoding="utf-8") as f:
+        json.dump(project, f, indent=4, ensure_ascii=False)
+
+    print(f"JSON project file successfully saved at {path_to_output_file}")
+
+    return overall_success
+
+
+def _new_validate_folder_structure_and_get_filenames(data_model_files: Path) -> tuple[Path | None, list[Path]]:
+    if not data_model_files.is_dir():
+        raise UserError(f"ERROR: {data_model_files} is not a directory.")
+    folder = [x for x in data_model_files.glob("*") if _non_hidden(x)]
+    processed_files = []
+    onto_folders, processed_onto = _get_and_validate_onto_folder(data_model_files, folder)
+    processed_files.extend(processed_onto)
+    listfolder, processed_lists = _new_get_and_validate_list_folder(data_model_files)
+    processed_files.extend(processed_lists)
+    print("The following files will be processed:")
+    print(*(f" - {file}" for file in processed_files), sep="\n")
+    return listfolder, onto_folders
+
+
+def _get_and_validate_onto_folder(data_model_files: Path, folder: list[Path]) -> tuple[list[Path], list[str]]:
     processed_files = []
     onto_folders = [x for x in folder if x.is_dir() and regex.search(r"([\w.-]+) \(([\w.\- ]+)\)", x.name)]
     if not onto_folders:
         raise UserError(
             f"'{data_model_files}' must contain at least one subfolder named after the pattern 'onto_name (onto_label)'"
         )
     for onto_folder in onto_folders:
@@ -100,14 +158,23 @@
                 f"ERROR: '{data_model_files}/{onto_folder.name}' must contain one file 'properties.xlsx' "
                 "and one file 'resources.xlsx', but nothing else."
             )
         processed_files.extend([f"{data_model_files}/{onto_folder.name}/{file}" for file in contents])
     return onto_folders, processed_files
 
 
+def _new_get_and_validate_list_folder(
+    data_model_files: Path,
+) -> tuple[Path | None, list[str]]:
+    if not (list_dir := (data_model_files / "lists")).is_dir():
+        return None, []
+    processed_files = [str(file) for file in list_dir.glob("*list*.xlsx") if _non_hidden(file)]
+    return list_dir, processed_files
+
+
 def _non_hidden(path: Path) -> bool:
     return not regex.search(r"^(\.|~\$).+", path.name)
 
 
 def _create_project_json(
     data_model_files: str, listfolder: list[Path], onto_folders: list[Path]
 ) -> tuple[bool, dict[str, Any]]:
@@ -118,14 +185,44 @@
     ontologies, success = _get_ontologies(data_model_files, onto_folders)
     if not success:
         overall_success = False
     schema = "https://raw.githubusercontent.com/dasch-swiss/dsp-tools/main/src/dsp_tools/resources/schema/project.json"
     project = {
         "prefixes": {"": ""},
         "$schema": schema,
+        "project": {
+            "shortcode": "",
+            "shortname": "",
+            "longname": "",
+            "descriptions": {"en": ""},
+            "keywords": [""],
+        },
+    }
+    if lists:
+        project["project"]["lists"] = lists  # type: ignore[index]
+    project["project"]["ontologies"] = ontologies  # type: ignore[index]
+    return overall_success, project
+
+
+def _new_create_project_json(
+    data_model_files: str, onto_folders: list[Path], list_folder: Path | None
+) -> tuple[bool, dict[str, Any]]:
+    overall_success = True
+    lists = None
+    if list_folder:
+        lists, success = new_excel2lists(list_folder)
+        if not success:
+            overall_success = False
+    ontologies, success = _get_ontologies(data_model_files, onto_folders)
+    if not success:
+        overall_success = False
+    schema = "https://raw.githubusercontent.com/dasch-swiss/dsp-tools/main/src/dsp_tools/resources/schema/project.json"
+    project = {
+        "prefixes": {"": ""},
+        "$schema": schema,
         "project": {
             "shortcode": "",
             "shortname": "",
             "longname": "",
             "descriptions": {"en": ""},
             "keywords": [""],
         },
```

### Comparing `dsp_tools-7.1.3.post7/src/dsp_tools/commands/excel2json/properties.py` & `dsp_tools-7.1.3.post9/src/dsp_tools/commands/excel2json/properties.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post7/src/dsp_tools/commands/excel2json/resources.py` & `dsp_tools-7.1.3.post9/src/dsp_tools/commands/excel2json/resources.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post7/src/dsp_tools/commands/excel2json/utils.py` & `dsp_tools-7.1.3.post9/src/dsp_tools/commands/excel2json/utils.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post7/src/dsp_tools/commands/excel2xml/excel2xml_cli.py` & `dsp_tools-7.1.3.post9/src/dsp_tools/commands/excel2xml/excel2xml_cli.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post7/src/dsp_tools/commands/excel2xml/excel2xml_lib.py` & `dsp_tools-7.1.3.post9/src/dsp_tools/commands/excel2xml/excel2xml_lib.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post7/src/dsp_tools/commands/excel2xml/propertyelement.py` & `dsp_tools-7.1.3.post9/src/dsp_tools/commands/excel2xml/propertyelement.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post7/src/dsp_tools/commands/id2iri.py` & `dsp_tools-7.1.3.post9/src/dsp_tools/commands/id2iri.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post7/src/dsp_tools/commands/ingest_xmlupload/apply_ingest_id.py` & `dsp_tools-7.1.3.post9/src/dsp_tools/commands/ingest_xmlupload/apply_ingest_id.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post7/src/dsp_tools/commands/ingest_xmlupload/upload_xml.py` & `dsp_tools-7.1.3.post9/src/dsp_tools/commands/ingest_xmlupload/upload_xml.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post7/src/dsp_tools/commands/ingest_xmlupload/user_information.py` & `dsp_tools-7.1.3.post9/src/dsp_tools/commands/ingest_xmlupload/user_information.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post7/src/dsp_tools/commands/project/create/project_create.py` & `dsp_tools-7.1.3.post9/src/dsp_tools/commands/project/create/project_create.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post7/src/dsp_tools/commands/project/create/project_create_lists.py` & `dsp_tools-7.1.3.post9/src/dsp_tools/commands/project/create/project_create_lists.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post7/src/dsp_tools/commands/project/create/project_validate.py` & `dsp_tools-7.1.3.post9/src/dsp_tools/commands/project/create/project_validate.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post7/src/dsp_tools/commands/project/get.py` & `dsp_tools-7.1.3.post9/src/dsp_tools/commands/project/get.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post7/src/dsp_tools/commands/project/models/context.py` & `dsp_tools-7.1.3.post9/src/dsp_tools/commands/project/models/context.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post7/src/dsp_tools/commands/project/models/group.py` & `dsp_tools-7.1.3.post9/src/dsp_tools/commands/project/models/group.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post7/src/dsp_tools/commands/project/models/helpers.py` & `dsp_tools-7.1.3.post9/src/dsp_tools/commands/project/models/helpers.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post7/src/dsp_tools/commands/project/models/listnode.py` & `dsp_tools-7.1.3.post9/src/dsp_tools/commands/project/models/listnode.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post7/src/dsp_tools/commands/project/models/ontology.py` & `dsp_tools-7.1.3.post9/src/dsp_tools/commands/project/models/ontology.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post7/src/dsp_tools/commands/project/models/project.py` & `dsp_tools-7.1.3.post9/src/dsp_tools/commands/project/models/project.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post7/src/dsp_tools/commands/project/models/propertyclass.py` & `dsp_tools-7.1.3.post9/src/dsp_tools/commands/project/models/propertyclass.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post7/src/dsp_tools/commands/project/models/resourceclass.py` & `dsp_tools-7.1.3.post9/src/dsp_tools/commands/project/models/resourceclass.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post7/src/dsp_tools/commands/project/models/user.py` & `dsp_tools-7.1.3.post9/src/dsp_tools/commands/project/models/user.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post7/src/dsp_tools/commands/resume_xmlupload/resume_xmlupload.py` & `dsp_tools-7.1.3.post9/src/dsp_tools/commands/resume_xmlupload/resume_xmlupload.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post7/src/dsp_tools/commands/rosetta.py` & `dsp_tools-7.1.3.post9/src/dsp_tools/commands/rosetta.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post7/src/dsp_tools/commands/start_stack.py` & `dsp_tools-7.1.3.post9/src/dsp_tools/commands/start_stack.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post7/src/dsp_tools/commands/template.py` & `dsp_tools-7.1.3.post9/src/dsp_tools/commands/template.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post7/src/dsp_tools/commands/xmlupload/ark2iri.py` & `dsp_tools-7.1.3.post9/src/dsp_tools/commands/xmlupload/ark2iri.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post7/src/dsp_tools/commands/xmlupload/check_consistency_with_ontology.py` & `dsp_tools-7.1.3.post9/src/dsp_tools/commands/xmlupload/check_consistency_with_ontology.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post7/src/dsp_tools/commands/xmlupload/iri_resolver.py` & `dsp_tools-7.1.3.post9/src/dsp_tools/commands/xmlupload/iri_resolver.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post7/src/dsp_tools/commands/xmlupload/list_client.py` & `dsp_tools-7.1.3.post9/src/dsp_tools/commands/xmlupload/list_client.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post7/src/dsp_tools/commands/xmlupload/models/formatted_text_value.py` & `dsp_tools-7.1.3.post9/src/dsp_tools/commands/xmlupload/models/formatted_text_value.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post7/src/dsp_tools/commands/xmlupload/models/ontology_lookup_models.py` & `dsp_tools-7.1.3.post9/src/dsp_tools/commands/xmlupload/models/ontology_lookup_models.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post7/src/dsp_tools/commands/xmlupload/models/ontology_problem_models.py` & `dsp_tools-7.1.3.post9/src/dsp_tools/commands/xmlupload/models/ontology_problem_models.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post7/src/dsp_tools/commands/xmlupload/models/permission.py` & `dsp_tools-7.1.3.post9/src/dsp_tools/commands/xmlupload/models/permission.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post7/src/dsp_tools/commands/xmlupload/models/sipi.py` & `dsp_tools-7.1.3.post9/src/dsp_tools/commands/xmlupload/models/sipi.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post7/src/dsp_tools/commands/xmlupload/models/upload_state.py` & `dsp_tools-7.1.3.post9/src/dsp_tools/commands/xmlupload/models/upload_state.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post7/src/dsp_tools/commands/xmlupload/models/xmlallow.py` & `dsp_tools-7.1.3.post9/src/dsp_tools/commands/xmlupload/models/xmlallow.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post7/src/dsp_tools/commands/xmlupload/models/xmlbitstream.py` & `dsp_tools-7.1.3.post9/src/dsp_tools/commands/xmlupload/models/xmlbitstream.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post7/src/dsp_tools/commands/xmlupload/models/xmlpermission.py` & `dsp_tools-7.1.3.post9/src/dsp_tools/commands/xmlupload/models/xmlpermission.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post7/src/dsp_tools/commands/xmlupload/models/xmlproperty.py` & `dsp_tools-7.1.3.post9/src/dsp_tools/commands/xmlupload/models/xmlproperty.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post7/src/dsp_tools/commands/xmlupload/models/xmlresource.py` & `dsp_tools-7.1.3.post9/src/dsp_tools/commands/xmlupload/models/xmlresource.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post7/src/dsp_tools/commands/xmlupload/models/xmlvalue.py` & `dsp_tools-7.1.3.post9/src/dsp_tools/commands/xmlupload/models/xmlvalue.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post7/src/dsp_tools/commands/xmlupload/ontology_client.py` & `dsp_tools-7.1.3.post9/src/dsp_tools/commands/xmlupload/ontology_client.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post7/src/dsp_tools/commands/xmlupload/project_client.py` & `dsp_tools-7.1.3.post9/src/dsp_tools/commands/xmlupload/project_client.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post7/src/dsp_tools/commands/xmlupload/read_validate_xml_file.py` & `dsp_tools-7.1.3.post9/src/dsp_tools/commands/xmlupload/read_validate_xml_file.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post7/src/dsp_tools/commands/xmlupload/resource_create_client.py` & `dsp_tools-7.1.3.post9/src/dsp_tools/commands/xmlupload/resource_create_client.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post7/src/dsp_tools/commands/xmlupload/resource_multimedia.py` & `dsp_tools-7.1.3.post9/src/dsp_tools/commands/xmlupload/resource_multimedia.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post7/src/dsp_tools/commands/xmlupload/stash/construct_and_analyze_graph.py` & `dsp_tools-7.1.3.post9/src/dsp_tools/commands/xmlupload/stash/construct_and_analyze_graph.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post7/src/dsp_tools/commands/xmlupload/stash/graph_models.py` & `dsp_tools-7.1.3.post9/src/dsp_tools/commands/xmlupload/stash/graph_models.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post7/src/dsp_tools/commands/xmlupload/stash/stash_circular_references.py` & `dsp_tools-7.1.3.post9/src/dsp_tools/commands/xmlupload/stash/stash_circular_references.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post7/src/dsp_tools/commands/xmlupload/stash/stash_models.py` & `dsp_tools-7.1.3.post9/src/dsp_tools/commands/xmlupload/stash/stash_models.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post7/src/dsp_tools/commands/xmlupload/stash/upload_stashed_resptr_props.py` & `dsp_tools-7.1.3.post9/src/dsp_tools/commands/xmlupload/stash/upload_stashed_resptr_props.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post7/src/dsp_tools/commands/xmlupload/stash/upload_stashed_xml_texts.py` & `dsp_tools-7.1.3.post9/src/dsp_tools/commands/xmlupload/stash/upload_stashed_xml_texts.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post7/src/dsp_tools/commands/xmlupload/upload_config.py` & `dsp_tools-7.1.3.post9/src/dsp_tools/commands/xmlupload/upload_config.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post7/src/dsp_tools/commands/xmlupload/write_diagnostic_info.py` & `dsp_tools-7.1.3.post9/src/dsp_tools/commands/xmlupload/write_diagnostic_info.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post7/src/dsp_tools/commands/xmlupload/xmlupload.py` & `dsp_tools-7.1.3.post9/src/dsp_tools/commands/xmlupload/xmlupload.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post7/src/dsp_tools/models/custom_warnings.py` & `dsp_tools-7.1.3.post9/src/dsp_tools/models/custom_warnings.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post7/src/dsp_tools/models/datetimestamp.py` & `dsp_tools-7.1.3.post9/src/dsp_tools/models/datetimestamp.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post7/src/dsp_tools/models/exceptions.py` & `dsp_tools-7.1.3.post9/src/dsp_tools/models/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,21 @@
 
     message: str
 
     def __str__(self) -> str:
         return self.message
 
 
+@dataclass
+class Excel2JsonListError(BaseError):
+    """
+    Class for errors that are raised in the context of the excel2json ListNode class.
+    """
+
+
 class InternalError(BaseError):
     """
     Class for errors that are raised if the user cannot solve the problem themselves.
     """
 
     def __init__(self, custom_msg: str | None = None, keep_default_msg: bool = True) -> None:
         default_msg = (
```

### Comparing `dsp_tools-7.1.3.post7/src/dsp_tools/models/langstring.py` & `dsp_tools-7.1.3.post9/src/dsp_tools/models/langstring.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post7/src/dsp_tools/models/projectContext.py` & `dsp_tools-7.1.3.post9/src/dsp_tools/models/projectContext.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post7/src/dsp_tools/resources/0100-template-repo/template.json` & `dsp_tools-7.1.3.post9/src/dsp_tools/resources/0100-template-repo/template.json`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post7/src/dsp_tools/resources/0100-template-repo/template.xml` & `dsp_tools-7.1.3.post9/src/dsp_tools/resources/0100-template-repo/template.xml`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post7/src/dsp_tools/resources/schema/data.xsd` & `dsp_tools-7.1.3.post9/src/dsp_tools/resources/schema/data.xsd`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post7/src/dsp_tools/resources/schema/lists-only.json` & `dsp_tools-7.1.3.post9/src/dsp_tools/resources/schema/lists-only.json`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post7/src/dsp_tools/resources/schema/project.json` & `dsp_tools-7.1.3.post9/src/dsp_tools/resources/schema/project.json`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post7/src/dsp_tools/resources/schema/properties-only.json` & `dsp_tools-7.1.3.post9/src/dsp_tools/resources/schema/properties-only.json`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post7/src/dsp_tools/resources/schema/resources-only.json` & `dsp_tools-7.1.3.post9/src/dsp_tools/resources/schema/resources-only.json`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post7/src/dsp_tools/resources/start-stack/docker-compose.yml` & `dsp_tools-7.1.3.post9/src/dsp_tools/resources/start-stack/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post7/src/dsp_tools/utils/connection.py` & `dsp_tools-7.1.3.post9/src/dsp_tools/utils/connection.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post7/src/dsp_tools/utils/connection_live.py` & `dsp_tools-7.1.3.post9/src/dsp_tools/utils/connection_live.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post7/src/dsp_tools/utils/date_util.py` & `dsp_tools-7.1.3.post9/src/dsp_tools/utils/date_util.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post7/src/dsp_tools/utils/json_ld_util.py` & `dsp_tools-7.1.3.post9/src/dsp_tools/utils/json_ld_util.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post7/src/dsp_tools/utils/logger_config.py` & `dsp_tools-7.1.3.post9/src/dsp_tools/utils/logger_config.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post7/src/dsp_tools/utils/set_encoder.py` & `dsp_tools-7.1.3.post9/src/dsp_tools/utils/set_encoder.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post7/src/dsp_tools/utils/shared.py` & `dsp_tools-7.1.3.post9/src/dsp_tools/utils/shared.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post7/src/dsp_tools/utils/uri_util.py` & `dsp_tools-7.1.3.post9/src/dsp_tools/utils/uri_util.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post7/src/dsp_tools/utils/warnings_config.py` & `dsp_tools-7.1.3.post9/src/dsp_tools/utils/warnings_config.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post7/src/dsp_tools/utils/xml_utils.py` & `dsp_tools-7.1.3.post9/src/dsp_tools/utils/xml_utils.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post7/src/dsp_tools/utils/xml_validation.py` & `dsp_tools-7.1.3.post9/src/dsp_tools/utils/xml_validation.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post7/src/dsp_tools/utils/xml_validation_models.py` & `dsp_tools-7.1.3.post9/src/dsp_tools/utils/xml_validation_models.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post7/PKG-INFO` & `dsp_tools-7.1.3.post9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsp-tools
-Version: 7.1.3.post7
+Version: 7.1.3.post9
 Summary: DSP-TOOLS is a Python package with a command line interface that helps you interact with a DaSCH service platform (DSP) server.
 Home-page: https://www.dasch.swiss/
 License: GPL-3.0-only
 Author: DaSCH - Swiss National Data and Service Center for the Humanities
 Author-email: info@dasch.swiss
 Requires-Python: >=3.12,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

