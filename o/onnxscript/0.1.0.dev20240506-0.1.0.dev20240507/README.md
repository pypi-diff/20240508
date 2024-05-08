# Comparing `tmp/onnxscript-0.1.0.dev20240506.tar.gz` & `tmp/onnxscript-0.1.0.dev20240507.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onnxscript-0.1.0.dev20240506.tar", last modified: Mon May  6 00:01:11 2024, max compression
+gzip compressed data, was "onnxscript-0.1.0.dev20240507.tar", last modified: Tue May  7 00:01:17 2024, max compression
```

## Comparing `onnxscript-0.1.0.dev20240506.tar` & `onnxscript-0.1.0.dev20240507.tar`

### file list

```diff
@@ -1,218 +1,218 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-06 00:01:11.964910 onnxscript-0.1.0.dev20240506/
--rw-r--r--   0 vsts      (1001) docker     (127)     1073 2024-05-06 00:00:42.000000 onnxscript-0.1.0.dev20240506/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (127)      211 2024-05-06 00:00:42.000000 onnxscript-0.1.0.dev20240506/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (127)    10854 2024-05-06 00:01:11.964910 onnxscript-0.1.0.dev20240506/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     8671 2024-05-06 00:00:42.000000 onnxscript-0.1.0.dev20240506/README.md
--rw-r--r--   0 vsts      (1001) docker     (127)        6 2024-05-06 00:00:42.000000 onnxscript-0.1.0.dev20240506/VERSION
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-06 00:01:11.928910 onnxscript-0.1.0.dev20240506/onnxscript/
--rw-r--r--   0 vsts      (1001) docker     (127)     2282 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-06 00:01:11.932910 onnxscript-0.1.0.dev20240506/onnxscript/_internal/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/_internal/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9313 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/_internal/analysis.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2228 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/_internal/ast_utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9811 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/_internal/autocast.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2560 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/_internal/deprecation.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5166 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/_internal/param_manipulation.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1176 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/_internal/runtime_typing.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3523 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/_internal/utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1018 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/_internal/version_utils.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-06 00:01:11.932910 onnxscript-0.1.0.dev20240506/onnxscript/_legacy_ir/
--rw-r--r--   0 vsts      (1001) docker     (127)    11316 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/_legacy_ir/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    36198 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/_legacy_ir/visitor.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-06 00:01:11.932910 onnxscript-0.1.0.dev20240506/onnxscript/_thirdparty/
--rw-r--r--   0 vsts      (1001) docker     (127)    10608 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/_thirdparty/asciichartpy.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-06 00:01:11.932910 onnxscript-0.1.0.dev20240506/onnxscript/backend/
--rw-r--r--   0 vsts      (1001) docker     (127)      247 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/backend/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11498 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/backend/onnx_backend.py
--rw-r--r--   0 vsts      (1001) docker     (127)    30612 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/backend/onnx_export.py
--rw-r--r--   0 vsts      (1001) docker     (127)    61554 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/converter.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-06 00:01:11.920910 onnxscript-0.1.0.dev20240506/onnxscript/diagnostics/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-06 00:01:11.932910 onnxscript-0.1.0.dev20240506/onnxscript/diagnostics/infra/
--rw-r--r--   0 vsts      (1001) docker     (127)      583 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/diagnostics/infra/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11045 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/diagnostics/infra/_infra.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13086 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/diagnostics/infra/context.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5544 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/diagnostics/infra/decorator.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3364 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/diagnostics/infra/formatter.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-06 00:01:11.944910 onnxscript-0.1.0.dev20240506/onnxscript/diagnostics/infra/sarif/
--rw-r--r--   0 vsts      (1001) docker     (127)     4364 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/diagnostics/infra/sarif/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1716 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/diagnostics/infra/sarif/_address.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2980 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/diagnostics/infra/sarif/_artifact.py
--rw-r--r--   0 vsts      (1001) docker     (127)      875 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/diagnostics/infra/sarif/_artifact_change.py
--rw-r--r--   0 vsts      (1001) docker     (127)      996 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/diagnostics/infra/sarif/_artifact_content.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1029 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/diagnostics/infra/sarif/_artifact_location.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1195 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/diagnostics/infra/sarif/_attachment.py
--rw-r--r--   0 vsts      (1001) docker     (127)      900 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/diagnostics/infra/sarif/_code_flow.py
--rw-r--r--   0 vsts      (1001) docker     (127)      986 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/diagnostics/infra/sarif/_configuration_override.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1154 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/diagnostics/infra/sarif/_conversion.py
--rw-r--r--   0 vsts      (1001) docker     (127)      937 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/diagnostics/infra/sarif/_edge.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1065 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/diagnostics/infra/sarif/_edge_traversal.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1133 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/diagnostics/infra/sarif/_exception.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3794 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/diagnostics/infra/sarif/_external_properties.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1089 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/diagnostics/infra/sarif/_external_property_file_reference.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3819 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/diagnostics/infra/sarif/_external_property_file_references.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1034 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/diagnostics/infra/sarif/_fix.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1051 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/diagnostics/infra/sarif/_graph.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1388 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/diagnostics/infra/sarif/_graph_traversal.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4561 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/diagnostics/infra/sarif/_invocation.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1552 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/diagnostics/infra/sarif/_location.py
--rw-r--r--   0 vsts      (1001) docker     (127)      946 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/diagnostics/infra/sarif/_location_relationship.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1282 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/diagnostics/infra/sarif/_logical_location.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1044 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/diagnostics/infra/sarif/_message.py
--rw-r--r--   0 vsts      (1001) docker     (127)      787 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/diagnostics/infra/sarif/_multiformat_message_string.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1036 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/diagnostics/infra/sarif/_node.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1892 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/diagnostics/infra/sarif/_notification.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1305 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/diagnostics/infra/sarif/_physical_location.py
--rw-r--r--   0 vsts      (1001) docker     (127)      488 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/diagnostics/infra/sarif/_property_bag.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1141 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/diagnostics/infra/sarif/_rectangle.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2013 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/diagnostics/infra/sarif/_region.py
--rw-r--r--   0 vsts      (1001) docker     (127)      870 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/diagnostics/infra/sarif/_replacement.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1104 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/diagnostics/infra/sarif/_reporting_configuration.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2700 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/diagnostics/infra/sarif/_reporting_descriptor.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1109 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_reference.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1090 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_relationship.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5002 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/diagnostics/infra/sarif/_result.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1508 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/diagnostics/infra/sarif/_result_provenance.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5246 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/diagnostics/infra/sarif/_run.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1118 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/diagnostics/infra/sarif/_run_automation_details.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1198 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/diagnostics/infra/sarif/_sarif_log.py
--rw-r--r--   0 vsts      (1001) docker     (127)      751 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/diagnostics/infra/sarif/_special_locations.py
--rw-r--r--   0 vsts      (1001) docker     (127)      824 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/diagnostics/infra/sarif/_stack.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1070 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/diagnostics/infra/sarif/_stack_frame.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1231 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/diagnostics/infra/sarif/_suppression.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1333 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/diagnostics/infra/sarif/_thread_flow.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2473 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/diagnostics/infra/sarif/_thread_flow_location.py
--rw-r--r--   0 vsts      (1001) docker     (127)      830 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/diagnostics/infra/sarif/_tool.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4941 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/diagnostics/infra/sarif/_tool_component.py
--rw-r--r--   0 vsts      (1001) docker     (127)      915 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/diagnostics/infra/sarif/_tool_component_reference.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1452 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/diagnostics/infra/sarif/_translation_metadata.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1391 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/diagnostics/infra/sarif/_version_control_details.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1498 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/diagnostics/infra/sarif/_web_request.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1566 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/diagnostics/infra/sarif/_web_response.py
--rw-r--r--   0 vsts      (1001) docker     (127)      193 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/diagnostics/infra/sarif/version.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2515 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/diagnostics/infra/utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)    22081 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/evaluator.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-06 00:01:11.924910 onnxscript-0.1.0.dev20240506/onnxscript/function_libs/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-06 00:01:11.920910 onnxscript-0.1.0.dev20240506/onnxscript/function_libs/tools/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-06 00:01:11.944910 onnxscript-0.1.0.dev20240506/onnxscript/function_libs/tools/torch_lib/
--rw-r--r--   0 vsts      (1001) docker     (127)    16361 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/function_libs/tools/torch_lib/deduce_type_constraints.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11767 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/function_libs/tools/torch_lib/generate_aten_signatures.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11834 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/function_libs/tools/torch_lib/generate_prims_signatures.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-06 00:01:11.944910 onnxscript-0.1.0.dev20240506/onnxscript/function_libs/torch_lib/
--rw-r--r--   0 vsts      (1001) docker     (127)      149 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/function_libs/torch_lib/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)       77 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/function_libs/torch_lib/_constants.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1452 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/function_libs/torch_lib/_flags.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-06 00:01:11.944910 onnxscript-0.1.0.dev20240506/onnxscript/function_libs/torch_lib/graph_building/
--rw-r--r--   0 vsts      (1001) docker     (127)     2291 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/function_libs/torch_lib/graph_building/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    28280 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/function_libs/torch_lib/graph_building/_graph_building_ir.py
--rw-r--r--   0 vsts      (1001) docker     (127)    44452 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/function_libs/torch_lib/graph_building/_graph_building_torch.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-06 00:01:11.948910 onnxscript-0.1.0.dev20240506/onnxscript/function_libs/torch_lib/ops/
--rw-r--r--   0 vsts      (1001) docker     (127)      208 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/function_libs/torch_lib/ops/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1991 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/function_libs/torch_lib/ops/common.py
--rw-r--r--   0 vsts      (1001) docker     (127)   290367 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/function_libs/torch_lib/ops/core.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12343 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/function_libs/torch_lib/ops/fft.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13256 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/function_libs/torch_lib/ops/linalg.py
--rw-r--r--   0 vsts      (1001) docker     (127)      911 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/function_libs/torch_lib/ops/nested.py
--rw-r--r--   0 vsts      (1001) docker     (127)    86028 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/function_libs/torch_lib/ops/nn.py
--rw-r--r--   0 vsts      (1001) docker     (127)    20667 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/function_libs/torch_lib/ops/prims.py
--rw-r--r--   0 vsts      (1001) docker     (127)      920 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/function_libs/torch_lib/ops/sparse.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11262 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/function_libs/torch_lib/ops/special.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1155 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/function_libs/torch_lib/ops/vision.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5547 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/function_libs/torch_lib/registration.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2118 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/function_libs/torch_lib/tensor_typing.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-06 00:01:11.952910 onnxscript-0.1.0.dev20240506/onnxscript/ir/
--rw-r--r--   0 vsts      (1001) docker     (127)     2501 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/ir/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8474 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/ir/_convenience.py
--rw-r--r--   0 vsts      (1001) docker     (127)    82923 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/ir/_core.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1775 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/ir/_display.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4285 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/ir/_enums.py
--rw-r--r--   0 vsts      (1001) docker     (127)      900 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/ir/_graph_comparison.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1853 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/ir/_invariants.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10518 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/ir/_linked_list.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1684 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/ir/_metadata.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1064 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/ir/_name_authority.py
--rw-r--r--   0 vsts      (1001) docker     (127)    20616 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/ir/_protocols.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2863 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/ir/_type_casting.py
--rw-r--r--   0 vsts      (1001) docker     (127)    49020 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/ir/serde.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19643 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/irbuilder.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6457 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/main.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-06 00:01:11.952910 onnxscript-0.1.0.dev20240506/onnxscript/onnx_opset/
--rw-r--r--   0 vsts      (1001) docker     (127)     4852 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/onnx_opset/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-06 00:01:11.956910 onnxscript-0.1.0.dev20240506/onnxscript/onnx_opset/_impl/
--rw-r--r--   0 vsts      (1001) docker     (127)   153815 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/onnx_opset/_impl/opset1.py
--rw-r--r--   0 vsts      (1001) docker     (127)    53445 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/onnx_opset/_impl/opset10.py
--rw-r--r--   0 vsts      (1001) docker     (127)   157597 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/onnx_opset/_impl/opset11.py
--rw-r--r--   0 vsts      (1001) docker     (127)    43533 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/onnx_opset/_impl/opset12.py
--rw-r--r--   0 vsts      (1001) docker     (127)   140743 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/onnx_opset/_impl/opset13.py
--rw-r--r--   0 vsts      (1001) docker     (127)    41780 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/onnx_opset/_impl/opset14.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19290 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/onnx_opset/_impl/opset15.py
--rw-r--r--   0 vsts      (1001) docker     (127)    50662 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/onnx_opset/_impl/opset16.py
--rw-r--r--   0 vsts      (1001) docker     (127)    21513 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/onnx_opset/_impl/opset17.py
--rw-r--r--   0 vsts      (1001) docker     (127)    70208 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/onnx_opset/_impl/opset18.py
--rw-r--r--   0 vsts      (1001) docker     (127)    75098 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/onnx_opset/_impl/opset19.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7937 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/onnx_opset/_impl/opset2.py
--rw-r--r--   0 vsts      (1001) docker     (127)    28284 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/onnx_opset/_impl/opset20.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7645 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/onnx_opset/_impl/opset3.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1966 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/onnx_opset/_impl/opset4.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2572 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/onnx_opset/_impl/opset5.py
--rw-r--r--   0 vsts      (1001) docker     (127)    33248 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/onnx_opset/_impl/opset6.py
--rw-r--r--   0 vsts      (1001) docker     (127)    49053 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/onnx_opset/_impl/opset7.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19393 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/onnx_opset/_impl/opset8.py
--rw-r--r--   0 vsts      (1001) docker     (127)    58411 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/onnx_opset/_impl/opset9.py
--rw-r--r--   0 vsts      (1001) docker     (127)    39030 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml1.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4439 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml2.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13894 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml3.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5368 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml4.py
--rw-r--r--   0 vsts      (1001) docker     (127)    24713 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/onnx_opset/_impl/opset_ai_onnx_preview_training1.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5875 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/onnx_types.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-06 00:01:11.960910 onnxscript-0.1.0.dev20240506/onnxscript/optimizer/
--rw-r--r--   0 vsts      (1001) docker     (127)     4385 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/optimizer/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10232 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/optimizer/constant_folding.py
--rw-r--r--   0 vsts      (1001) docker     (127)    15603 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/optimizer/evaluator.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8554 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/optimizer/fold_constants_v0.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3994 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/optimizer/remove_unused.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2080 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/optimizer/remove_unused_function.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9978 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/optimizer/simple_function_folding.py
--rw-r--r--   0 vsts      (1001) docker     (127)       41 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/py.typed
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-06 00:01:11.960910 onnxscript-0.1.0.dev20240506/onnxscript/rewriter/
--rw-r--r--   0 vsts      (1001) docker     (127)     1508 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/rewriter/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1342 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/rewriter/_ir_utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1782 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/rewriter/_tape.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6405 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/rewriter/broadcast_to_matmul.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1419 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/rewriter/cast_constant_of_shape.py
--rw-r--r--   0 vsts      (1001) docker     (127)      709 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/rewriter/erfgelu.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8567 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/rewriter/function_rule.py
--rw-r--r--   0 vsts      (1001) docker     (127)      747 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/rewriter/gemm_to_matmul_add.py
--rw-r--r--   0 vsts      (1001) docker     (127)    29763 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/rewriter/generic_pattern.py
--rw-r--r--   0 vsts      (1001) docker     (127)      832 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/rewriter/no_op.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-06 00:01:11.960910 onnxscript-0.1.0.dev20240506/onnxscript/rewriter/onnxruntime/
--rw-r--r--   0 vsts      (1001) docker     (127)     2139 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/rewriter/onnxruntime/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1257 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/rewriter/onnxruntime/group_normalization_merge_silu.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5196 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/rewriter/onnxruntime/instance_to_group_normalization.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1824 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/rewriter/onnxruntime/softmax.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-06 00:01:11.964910 onnxscript-0.1.0.dev20240506/onnxscript/rewriter/onnxruntime/transformers/
--rw-r--r--   0 vsts      (1001) docker     (127)      602 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/rewriter/onnxruntime/transformers/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1019 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/rewriter/onnxruntime/transformers/biassplitgelu.py
--rw-r--r--   0 vsts      (1001) docker     (127)      826 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/rewriter/onnxruntime/transformers/fastgelu.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1647 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/rewriter/onnxruntime/transformers/layernorm.py
--rw-r--r--   0 vsts      (1001) docker     (127)    29345 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/rewriter/onnxruntime/transformers/multihead_attention.py
--rw-r--r--   0 vsts      (1001) docker     (127)    34531 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/rewriter/pattern.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1700 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/sourceinfo.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7658 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/tensor.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-06 00:01:11.964910 onnxscript-0.1.0.dev20240506/onnxscript/testing/
--rw-r--r--   0 vsts      (1001) docker     (127)    17350 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/testing/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11025 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/type_annotation.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-06 00:01:11.964910 onnxscript-0.1.0.dev20240506/onnxscript/utils/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/utils/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2239 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/utils/evaluation_utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)      706 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/utils/timing_utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2505 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/utils/utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)    24803 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/onnxscript/values.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-06 00:01:11.964910 onnxscript-0.1.0.dev20240506/onnxscript.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)    10854 2024-05-06 00:01:11.000000 onnxscript-0.1.0.dev20240506/onnxscript.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     8193 2024-05-06 00:01:11.000000 onnxscript-0.1.0.dev20240506/onnxscript.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-06 00:01:11.000000 onnxscript-0.1.0.dev20240506/onnxscript.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       35 2024-05-06 00:01:11.000000 onnxscript-0.1.0.dev20240506/onnxscript.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       11 2024-05-06 00:01:11.000000 onnxscript-0.1.0.dev20240506/onnxscript.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (127)     6453 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (127)       38 2024-05-06 00:01:11.964910 onnxscript-0.1.0.dev20240506/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (127)     1304 2024-05-06 00:00:43.000000 onnxscript-0.1.0.dev20240506/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-07 00:01:17.815414 onnxscript-0.1.0.dev20240507/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1073 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (127)      211 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (127)    10854 2024-05-07 00:01:17.811414 onnxscript-0.1.0.dev20240507/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     8671 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/README.md
+-rw-r--r--   0 vsts      (1001) docker     (127)        6 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/VERSION
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-07 00:01:17.775413 onnxscript-0.1.0.dev20240507/onnxscript/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2282 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-07 00:01:17.775413 onnxscript-0.1.0.dev20240507/onnxscript/_internal/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/_internal/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9313 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/_internal/analysis.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2228 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/_internal/ast_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9811 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/_internal/autocast.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2560 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/_internal/deprecation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5166 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/_internal/param_manipulation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1176 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/_internal/runtime_typing.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3523 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/_internal/utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1018 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/_internal/version_utils.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-07 00:01:17.775413 onnxscript-0.1.0.dev20240507/onnxscript/_legacy_ir/
+-rw-r--r--   0 vsts      (1001) docker     (127)    11316 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/_legacy_ir/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    36198 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/_legacy_ir/visitor.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-07 00:01:17.779414 onnxscript-0.1.0.dev20240507/onnxscript/_thirdparty/
+-rw-r--r--   0 vsts      (1001) docker     (127)    10608 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/_thirdparty/asciichartpy.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-07 00:01:17.779414 onnxscript-0.1.0.dev20240507/onnxscript/backend/
+-rw-r--r--   0 vsts      (1001) docker     (127)      247 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/backend/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11498 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/backend/onnx_backend.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    30612 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/backend/onnx_export.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    61554 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/converter.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-07 00:01:17.767413 onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-07 00:01:17.779414 onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/
+-rw-r--r--   0 vsts      (1001) docker     (127)      583 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11045 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/_infra.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13086 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/context.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5544 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/decorator.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3364 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/formatter.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-07 00:01:17.791414 onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/
+-rw-r--r--   0 vsts      (1001) docker     (127)     4364 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1716 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_address.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2980 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_artifact.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      875 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_artifact_change.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      996 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_artifact_content.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1029 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_artifact_location.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1195 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_attachment.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      900 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_code_flow.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      986 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_configuration_override.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1154 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_conversion.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      937 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_edge.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1065 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_edge_traversal.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1133 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_exception.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3794 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_external_properties.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1089 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_external_property_file_reference.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3819 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_external_property_file_references.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1034 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_fix.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1051 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_graph.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1388 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_graph_traversal.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4561 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_invocation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1552 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_location.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      946 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_location_relationship.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1282 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_logical_location.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1044 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_message.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      787 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_multiformat_message_string.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1036 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_node.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1892 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_notification.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1305 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_physical_location.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      488 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_property_bag.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1141 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_rectangle.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2013 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_region.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      870 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_replacement.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1104 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_reporting_configuration.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2700 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_reporting_descriptor.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1109 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_reference.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1090 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_relationship.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5002 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_result.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1508 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_result_provenance.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5246 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_run.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1118 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_run_automation_details.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1198 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_sarif_log.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      751 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_special_locations.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      824 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_stack.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1070 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_stack_frame.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1231 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_suppression.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1333 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_thread_flow.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2473 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_thread_flow_location.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      830 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_tool.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4941 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_tool_component.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      915 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_tool_component_reference.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1452 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_translation_metadata.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1391 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_version_control_details.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1498 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_web_request.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1566 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_web_response.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      193 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/version.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2515 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    22081 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/evaluator.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-07 00:01:17.771413 onnxscript-0.1.0.dev20240507/onnxscript/function_libs/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-07 00:01:17.767413 onnxscript-0.1.0.dev20240507/onnxscript/function_libs/tools/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-07 00:01:17.791414 onnxscript-0.1.0.dev20240507/onnxscript/function_libs/tools/torch_lib/
+-rw-r--r--   0 vsts      (1001) docker     (127)    16361 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/function_libs/tools/torch_lib/deduce_type_constraints.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11767 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/function_libs/tools/torch_lib/generate_aten_signatures.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11834 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/function_libs/tools/torch_lib/generate_prims_signatures.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-07 00:01:17.791414 onnxscript-0.1.0.dev20240507/onnxscript/function_libs/torch_lib/
+-rw-r--r--   0 vsts      (1001) docker     (127)      149 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/function_libs/torch_lib/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)       77 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/function_libs/torch_lib/_constants.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1452 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/function_libs/torch_lib/_flags.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-07 00:01:17.791414 onnxscript-0.1.0.dev20240507/onnxscript/function_libs/torch_lib/graph_building/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2291 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/function_libs/torch_lib/graph_building/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    28280 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/function_libs/torch_lib/graph_building/_graph_building_ir.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    44452 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/function_libs/torch_lib/graph_building/_graph_building_torch.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-07 00:01:17.795414 onnxscript-0.1.0.dev20240507/onnxscript/function_libs/torch_lib/ops/
+-rw-r--r--   0 vsts      (1001) docker     (127)      208 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/function_libs/torch_lib/ops/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1991 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/function_libs/torch_lib/ops/common.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   290367 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/function_libs/torch_lib/ops/core.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12343 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/function_libs/torch_lib/ops/fft.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13256 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/function_libs/torch_lib/ops/linalg.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      911 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/function_libs/torch_lib/ops/nested.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    86028 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/function_libs/torch_lib/ops/nn.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    20667 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/function_libs/torch_lib/ops/prims.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      920 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/function_libs/torch_lib/ops/sparse.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11262 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/function_libs/torch_lib/ops/special.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1155 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/function_libs/torch_lib/ops/vision.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5547 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/function_libs/torch_lib/registration.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2118 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/function_libs/torch_lib/tensor_typing.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-07 00:01:17.799414 onnxscript-0.1.0.dev20240507/onnxscript/ir/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2619 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/ir/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8474 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/ir/_convenience.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    87244 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/ir/_core.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1775 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/ir/_display.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4285 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/ir/_enums.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      900 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/ir/_graph_comparison.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1853 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/ir/_invariants.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10518 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/ir/_linked_list.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1684 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/ir/_metadata.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1064 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/ir/_name_authority.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    20616 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/ir/_protocols.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2863 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/ir/_type_casting.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    52805 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/ir/serde.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19643 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/irbuilder.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6457 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/main.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-07 00:01:17.799414 onnxscript-0.1.0.dev20240507/onnxscript/onnx_opset/
+-rw-r--r--   0 vsts      (1001) docker     (127)     4852 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/onnx_opset/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-07 00:01:17.807414 onnxscript-0.1.0.dev20240507/onnxscript/onnx_opset/_impl/
+-rw-r--r--   0 vsts      (1001) docker     (127)   153815 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/onnx_opset/_impl/opset1.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    53445 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/onnx_opset/_impl/opset10.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   157597 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/onnx_opset/_impl/opset11.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    43533 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/onnx_opset/_impl/opset12.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   140743 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/onnx_opset/_impl/opset13.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    41780 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/onnx_opset/_impl/opset14.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19290 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/onnx_opset/_impl/opset15.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    50662 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/onnx_opset/_impl/opset16.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    21513 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/onnx_opset/_impl/opset17.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    70208 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/onnx_opset/_impl/opset18.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    75098 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/onnx_opset/_impl/opset19.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7937 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/onnx_opset/_impl/opset2.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    28284 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/onnx_opset/_impl/opset20.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7645 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/onnx_opset/_impl/opset3.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1966 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/onnx_opset/_impl/opset4.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2572 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/onnx_opset/_impl/opset5.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    33248 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/onnx_opset/_impl/opset6.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    49053 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/onnx_opset/_impl/opset7.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19393 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/onnx_opset/_impl/opset8.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    58411 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/onnx_opset/_impl/opset9.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    39030 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml1.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4439 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml2.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13894 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml3.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5368 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml4.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    24713 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/onnx_opset/_impl/opset_ai_onnx_preview_training1.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5875 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/onnx_types.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-07 00:01:17.807414 onnxscript-0.1.0.dev20240507/onnxscript/optimizer/
+-rw-r--r--   0 vsts      (1001) docker     (127)     4385 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/optimizer/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10232 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/optimizer/constant_folding.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    15603 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/optimizer/evaluator.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8554 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/optimizer/fold_constants_v0.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3994 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/optimizer/remove_unused.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2080 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/optimizer/remove_unused_function.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9978 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/optimizer/simple_function_folding.py
+-rw-r--r--   0 vsts      (1001) docker     (127)       41 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/py.typed
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-07 00:01:17.811414 onnxscript-0.1.0.dev20240507/onnxscript/rewriter/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1508 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/rewriter/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1342 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/rewriter/_ir_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1782 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/rewriter/_tape.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6405 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/rewriter/broadcast_to_matmul.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1419 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/rewriter/cast_constant_of_shape.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      709 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/rewriter/erfgelu.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8567 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/rewriter/function_rule.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      747 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/rewriter/gemm_to_matmul_add.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    29763 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/rewriter/generic_pattern.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      832 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/rewriter/no_op.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-07 00:01:17.811414 onnxscript-0.1.0.dev20240507/onnxscript/rewriter/onnxruntime/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2139 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/rewriter/onnxruntime/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1257 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/rewriter/onnxruntime/group_normalization_merge_silu.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5196 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/rewriter/onnxruntime/instance_to_group_normalization.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1824 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/rewriter/onnxruntime/softmax.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-07 00:01:17.811414 onnxscript-0.1.0.dev20240507/onnxscript/rewriter/onnxruntime/transformers/
+-rw-r--r--   0 vsts      (1001) docker     (127)      602 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/rewriter/onnxruntime/transformers/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1019 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/rewriter/onnxruntime/transformers/biassplitgelu.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      826 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/rewriter/onnxruntime/transformers/fastgelu.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1647 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/rewriter/onnxruntime/transformers/layernorm.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    29345 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/rewriter/onnxruntime/transformers/multihead_attention.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    34531 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/rewriter/pattern.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1700 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/sourceinfo.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7658 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/tensor.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-07 00:01:17.811414 onnxscript-0.1.0.dev20240507/onnxscript/testing/
+-rw-r--r--   0 vsts      (1001) docker     (127)    17964 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/testing/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11025 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/type_annotation.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-07 00:01:17.811414 onnxscript-0.1.0.dev20240507/onnxscript/utils/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/utils/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2239 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/utils/evaluation_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      706 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/utils/timing_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2505 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/utils/utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    24803 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/values.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-07 00:01:17.811414 onnxscript-0.1.0.dev20240507/onnxscript.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)    10854 2024-05-07 00:01:17.000000 onnxscript-0.1.0.dev20240507/onnxscript.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     8193 2024-05-07 00:01:17.000000 onnxscript-0.1.0.dev20240507/onnxscript.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-07 00:01:17.000000 onnxscript-0.1.0.dev20240507/onnxscript.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       35 2024-05-07 00:01:17.000000 onnxscript-0.1.0.dev20240507/onnxscript.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       11 2024-05-07 00:01:17.000000 onnxscript-0.1.0.dev20240507/onnxscript.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)     6453 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (127)       38 2024-05-07 00:01:17.815414 onnxscript-0.1.0.dev20240507/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (127)     1304 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/setup.py
```

### Comparing `onnxscript-0.1.0.dev20240506/LICENSE` & `onnxscript-0.1.0.dev20240507/LICENSE`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/PKG-INFO` & `onnxscript-0.1.0.dev20240507/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onnxscript
-Version: 0.1.0.dev20240506
+Version: 0.1.0.dev20240507
 Summary: Naturally author ONNX functions and models using a subset of Python
 Author-email: Microsoft Corporation <onnx@microsoft.com>
 License: MIT License
         
         Copyright (c) Microsoft Corporation
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `onnxscript-0.1.0.dev20240506/README.md` & `onnxscript-0.1.0.dev20240507/README.md`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/__init__.py` & `onnxscript-0.1.0.dev20240507/onnxscript/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/_internal/analysis.py` & `onnxscript-0.1.0.dev20240507/onnxscript/_internal/analysis.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/_internal/ast_utils.py` & `onnxscript-0.1.0.dev20240507/onnxscript/_internal/ast_utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/_internal/autocast.py` & `onnxscript-0.1.0.dev20240507/onnxscript/_internal/autocast.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/_internal/deprecation.py` & `onnxscript-0.1.0.dev20240507/onnxscript/_internal/deprecation.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/_internal/param_manipulation.py` & `onnxscript-0.1.0.dev20240507/onnxscript/_internal/param_manipulation.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/_internal/runtime_typing.py` & `onnxscript-0.1.0.dev20240507/onnxscript/_internal/runtime_typing.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/_internal/utils.py` & `onnxscript-0.1.0.dev20240507/onnxscript/_internal/utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/_internal/version_utils.py` & `onnxscript-0.1.0.dev20240507/onnxscript/_internal/version_utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/_legacy_ir/__init__.py` & `onnxscript-0.1.0.dev20240507/onnxscript/_legacy_ir/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/_legacy_ir/visitor.py` & `onnxscript-0.1.0.dev20240507/onnxscript/_legacy_ir/visitor.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/_thirdparty/asciichartpy.py` & `onnxscript-0.1.0.dev20240507/onnxscript/_thirdparty/asciichartpy.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/backend/onnx_backend.py` & `onnxscript-0.1.0.dev20240507/onnxscript/backend/onnx_backend.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/backend/onnx_export.py` & `onnxscript-0.1.0.dev20240507/onnxscript/backend/onnx_export.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/converter.py` & `onnxscript-0.1.0.dev20240507/onnxscript/converter.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/diagnostics/infra/__init__.py` & `onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/diagnostics/infra/_infra.py` & `onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/_infra.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/diagnostics/infra/context.py` & `onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/context.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/diagnostics/infra/decorator.py` & `onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/decorator.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/diagnostics/infra/formatter.py` & `onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/formatter.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/diagnostics/infra/sarif/__init__.py` & `onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/diagnostics/infra/sarif/_address.py` & `onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_address.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/diagnostics/infra/sarif/_artifact.py` & `onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_artifact.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/diagnostics/infra/sarif/_artifact_change.py` & `onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_artifact_change.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/diagnostics/infra/sarif/_artifact_content.py` & `onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_artifact_content.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/diagnostics/infra/sarif/_artifact_location.py` & `onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_artifact_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/diagnostics/infra/sarif/_attachment.py` & `onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_attachment.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/diagnostics/infra/sarif/_code_flow.py` & `onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_code_flow.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/diagnostics/infra/sarif/_configuration_override.py` & `onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_configuration_override.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/diagnostics/infra/sarif/_conversion.py` & `onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_conversion.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/diagnostics/infra/sarif/_edge.py` & `onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_edge.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/diagnostics/infra/sarif/_edge_traversal.py` & `onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_edge_traversal.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/diagnostics/infra/sarif/_exception.py` & `onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_exception.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/diagnostics/infra/sarif/_external_properties.py` & `onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_external_properties.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/diagnostics/infra/sarif/_external_property_file_reference.py` & `onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_external_property_file_reference.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/diagnostics/infra/sarif/_external_property_file_references.py` & `onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_external_property_file_references.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/diagnostics/infra/sarif/_fix.py` & `onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_fix.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/diagnostics/infra/sarif/_graph.py` & `onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_graph.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/diagnostics/infra/sarif/_graph_traversal.py` & `onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_graph_traversal.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/diagnostics/infra/sarif/_invocation.py` & `onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_invocation.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/diagnostics/infra/sarif/_location.py` & `onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/diagnostics/infra/sarif/_location_relationship.py` & `onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_location_relationship.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/diagnostics/infra/sarif/_logical_location.py` & `onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_logical_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/diagnostics/infra/sarif/_message.py` & `onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_message.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/diagnostics/infra/sarif/_multiformat_message_string.py` & `onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_multiformat_message_string.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/diagnostics/infra/sarif/_node.py` & `onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_node.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/diagnostics/infra/sarif/_notification.py` & `onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_notification.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/diagnostics/infra/sarif/_physical_location.py` & `onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_physical_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/diagnostics/infra/sarif/_rectangle.py` & `onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_rectangle.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/diagnostics/infra/sarif/_region.py` & `onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_region.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/diagnostics/infra/sarif/_replacement.py` & `onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_replacement.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/diagnostics/infra/sarif/_reporting_configuration.py` & `onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_reporting_configuration.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/diagnostics/infra/sarif/_reporting_descriptor.py` & `onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_reporting_descriptor.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_reference.py` & `onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_reference.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_relationship.py` & `onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_relationship.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/diagnostics/infra/sarif/_result.py` & `onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_result.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/diagnostics/infra/sarif/_result_provenance.py` & `onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_result_provenance.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/diagnostics/infra/sarif/_run.py` & `onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_run.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/diagnostics/infra/sarif/_run_automation_details.py` & `onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_run_automation_details.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/diagnostics/infra/sarif/_sarif_log.py` & `onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_sarif_log.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/diagnostics/infra/sarif/_special_locations.py` & `onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_special_locations.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/diagnostics/infra/sarif/_stack.py` & `onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_stack.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/diagnostics/infra/sarif/_stack_frame.py` & `onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_stack_frame.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/diagnostics/infra/sarif/_suppression.py` & `onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_suppression.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/diagnostics/infra/sarif/_thread_flow.py` & `onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_thread_flow.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/diagnostics/infra/sarif/_thread_flow_location.py` & `onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_thread_flow_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/diagnostics/infra/sarif/_tool.py` & `onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_tool.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/diagnostics/infra/sarif/_tool_component.py` & `onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_tool_component.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/diagnostics/infra/sarif/_tool_component_reference.py` & `onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_tool_component_reference.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/diagnostics/infra/sarif/_translation_metadata.py` & `onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_translation_metadata.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/diagnostics/infra/sarif/_version_control_details.py` & `onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_version_control_details.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/diagnostics/infra/sarif/_web_request.py` & `onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_web_request.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/diagnostics/infra/sarif/_web_response.py` & `onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_web_response.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/diagnostics/infra/utils.py` & `onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/evaluator.py` & `onnxscript-0.1.0.dev20240507/onnxscript/evaluator.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/function_libs/tools/torch_lib/deduce_type_constraints.py` & `onnxscript-0.1.0.dev20240507/onnxscript/function_libs/tools/torch_lib/deduce_type_constraints.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/function_libs/tools/torch_lib/generate_aten_signatures.py` & `onnxscript-0.1.0.dev20240507/onnxscript/function_libs/tools/torch_lib/generate_aten_signatures.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/function_libs/tools/torch_lib/generate_prims_signatures.py` & `onnxscript-0.1.0.dev20240507/onnxscript/function_libs/tools/torch_lib/generate_prims_signatures.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/function_libs/torch_lib/_flags.py` & `onnxscript-0.1.0.dev20240507/onnxscript/function_libs/torch_lib/_flags.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/function_libs/torch_lib/graph_building/__init__.py` & `onnxscript-0.1.0.dev20240507/onnxscript/function_libs/torch_lib/graph_building/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/function_libs/torch_lib/graph_building/_graph_building_ir.py` & `onnxscript-0.1.0.dev20240507/onnxscript/function_libs/torch_lib/graph_building/_graph_building_ir.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/function_libs/torch_lib/graph_building/_graph_building_torch.py` & `onnxscript-0.1.0.dev20240507/onnxscript/function_libs/torch_lib/graph_building/_graph_building_torch.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/function_libs/torch_lib/ops/common.py` & `onnxscript-0.1.0.dev20240507/onnxscript/function_libs/torch_lib/ops/common.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/function_libs/torch_lib/ops/core.py` & `onnxscript-0.1.0.dev20240507/onnxscript/function_libs/torch_lib/ops/core.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/function_libs/torch_lib/ops/fft.py` & `onnxscript-0.1.0.dev20240507/onnxscript/function_libs/torch_lib/ops/fft.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/function_libs/torch_lib/ops/linalg.py` & `onnxscript-0.1.0.dev20240507/onnxscript/function_libs/torch_lib/ops/linalg.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/function_libs/torch_lib/ops/nested.py` & `onnxscript-0.1.0.dev20240507/onnxscript/function_libs/torch_lib/ops/nested.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/function_libs/torch_lib/ops/nn.py` & `onnxscript-0.1.0.dev20240507/onnxscript/function_libs/torch_lib/ops/nn.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/function_libs/torch_lib/ops/prims.py` & `onnxscript-0.1.0.dev20240507/onnxscript/function_libs/torch_lib/ops/prims.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/function_libs/torch_lib/ops/sparse.py` & `onnxscript-0.1.0.dev20240507/onnxscript/function_libs/torch_lib/ops/sparse.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/function_libs/torch_lib/ops/special.py` & `onnxscript-0.1.0.dev20240507/onnxscript/function_libs/torch_lib/ops/special.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/function_libs/torch_lib/ops/vision.py` & `onnxscript-0.1.0.dev20240507/onnxscript/function_libs/torch_lib/ops/vision.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/function_libs/torch_lib/registration.py` & `onnxscript-0.1.0.dev20240507/onnxscript/function_libs/torch_lib/registration.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/function_libs/torch_lib/tensor_typing.py` & `onnxscript-0.1.0.dev20240507/onnxscript/function_libs/torch_lib/tensor_typing.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/ir/__init__.py` & `onnxscript-0.1.0.dev20240507/onnxscript/ir/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,17 +17,20 @@
     "AttrInt64s",
     "AttrSparseTensor",
     "AttrSparseTensors",
     "AttrString",
     "AttrStrings",
     "AttrTensor",
     "AttrTensors",
+    "TypeAndShape",
     "AttrTypeProto",
+    "AttrTypeProtos",
     "SymbolicDim",
     "ExternalTensor",
+    "StringTensor",
     "Function",
     "Graph",
     "GraphView",
     "Input",
     "Model",
     "Node",
     "RefAttr",
@@ -76,29 +79,32 @@
     AttrSparseTensor,
     AttrSparseTensors,
     AttrString,
     AttrStrings,
     AttrTensor,
     AttrTensors,
     AttrTypeProto,
+    AttrTypeProtos,
     ExternalTensor,
     Function,
     Graph,
     GraphView,
     Input,
     Model,
     Node,
     OptionalType,
     RefAttr,
     SequenceType,
     Shape,
     SparseTensorType,
+    StringTensor,
     SymbolicDim,
     Tensor,
     TensorType,
+    TypeAndShape,
     Value,
 )
 from onnxscript.ir._enums import (
     AttributeType,
     DataType,
 )
 from onnxscript.ir._protocols import (
```

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/ir/_convenience.py` & `onnxscript-0.1.0.dev20240507/onnxscript/ir/_convenience.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/ir/_core.py` & `onnxscript-0.1.0.dev20240507/onnxscript/ir/_core.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 #
 # NOTE: Do not import pathlib in the IR. It is slow. Use os.path methods instead.
 
 from __future__ import annotations
 
 import abc
 import contextlib
+import dataclasses
 import math
 import mmap
 import os
 import sys
 import textwrap
 import typing
 from typing import (
@@ -43,14 +44,15 @@
     _metadata,
     _name_authority,
     _protocols,
     _type_casting,
 )
 
 if typing.TYPE_CHECKING:
+    import numpy.typing as npt
     from typing_extensions import TypeGuard
 
 TArrayCompatible = typing.TypeVar(
     "TArrayCompatible",
     bound=Union[_protocols.ArrayCompatible, _protocols.DLPackCompatible],
 )
 
@@ -572,14 +574,124 @@
         to the ONNX proto.
         """
         if self._metadata is None:
             self._metadata = _metadata.MetadataStore()
         return self._metadata
 
 
+class StringTensor(TensorBase, _protocols.TensorProtocol):
+    """Multidimensional array of strings (as binary data to match the string_data field in TensorProto)."""
+
+    __slots__ = (
+        "_raw",
+        "_shape",
+        "name",
+        "doc_string",
+        "_metadata_props",
+        "_metadata",
+    )
+
+    def __init__(
+        self,
+        value: Sequence[bytes] | npt.NDArray[np.bytes_],
+        *,
+        shape: Shape | None = None,
+        name: str = "",
+        doc_string: str | None = None,
+        metadata_props: dict[str, str] | None = None,
+    ) -> None:
+        """Initialize a tensor.
+
+        Args:
+            value: The backing data of the tensor. It can be a numpy array or a Sequence of bytes.
+            shape: The shape of the tensor. If None, the shape is obtained from the value.
+            name: The name of the tensor.
+            doc_string: The documentation string.
+            metadata_props: The metadata properties.
+        """
+        if shape is None:
+            if not hasattr(value, "shape"):
+                raise ValueError(
+                    f"Expected an object with a shape attribute, but {type(value)} does not have shape. "
+                    "Please specify the shape explicitly."
+                )
+            self._shape = Shape(getattr(value, "shape"), frozen=True)  # noqa: B009
+        else:
+            self._shape = shape
+            self._shape._frozen = True
+        self._raw = value
+        self.name = name
+        self.doc_string = doc_string
+        self._metadata: _metadata.MetadataStore | None = None
+        self._metadata_props = metadata_props
+
+    def __array__(self, dtype: Any = None) -> np.ndarray:
+        if isinstance(self._raw, np.ndarray):
+            return self._raw
+        assert isinstance(
+            self._raw, Sequence
+        ), f"Bug: Expected a sequence, got {type(self._raw)}"
+        return np.array(self._raw, dtype=dtype).reshape(self.shape.numpy())
+
+    def __dlpack__(self, *, stream: Any = None) -> Any:
+        del stream  # unused
+        raise TypeError("StringTensor does not support DLPack")
+
+    def __dlpack_device__(self) -> tuple[int, int]:
+        raise TypeError("StringTensor does not support DLPack")
+
+    def __repr__(self) -> str:
+        return f"{self._repr_base()}({self._raw!r}, name={self.name!r})"
+
+    @property
+    def dtype(self) -> _enums.DataType:
+        """The data type of the tensor. Immutable."""
+        return _enums.DataType.STRING
+
+    @property
+    def shape(self) -> Shape:
+        """The shape of the tensor. Immutable."""
+        return self._shape
+
+    @property
+    def raw(self) -> Sequence[bytes] | npt.NDArray[np.bytes_]:
+        """Backing data of the tensor. Immutable."""
+        return self._raw  # type: ignore[return-value]
+
+    def numpy(self) -> npt.NDArray[np.bytes_]:
+        """Return the tensor as a numpy array."""
+        return self.__array__()
+
+    def tobytes(self) -> bytes:
+        raise ValueError("StringTensor does not support tobytes. Use 'string_data' instead.")
+
+    def string_data(self) -> Sequence[bytes]:
+        """Return the string data of the tensor."""
+        if isinstance(self._raw, np.ndarray):
+            return self._raw.flatten().tolist()
+        return self._raw
+
+    @property
+    def metadata_props(self) -> dict[str, str]:
+        if self._metadata_props is None:
+            self._metadata_props = {}
+        return self._metadata_props
+
+    @property
+    def meta(self) -> _metadata.MetadataStore:
+        """The metadata store for intermediate analysis.
+
+        Write to the :attribute:`metadata_props` if you would like the metadata to be serialized
+        to the ONNX proto.
+        """
+        if self._metadata is None:
+            self._metadata = _metadata.MetadataStore()
+        return self._metadata
+
+
 class SymbolicDim(_protocols.SymbolicDimProtocol, _display.PrettyPrintable):
     __slots__ = ("_value",)
 
     def __init__(self, value: str | None) -> None:
         """Initialize a symbolic dimension.
 
         Args:
@@ -2404,21 +2516,46 @@
             name,
             _enums.AttributeType.SPARSE_TENSORS,
             value,
             doc_string=doc_string,
         )
 
 
+@dataclasses.dataclass
+class TypeAndShape:
+    """Type and shape.
+
+    Useful for constructing a type proto.
+    """
+
+    type: _protocols.TypeProtocol | None
+    shape: Shape | None
+
+
 class AttrTypeProto(_SpecializedAttr):
     def __init__(
         self,
         name: str,
-        value: _protocols.TypeProtocol,
+        value: TypeAndShape,
         doc_string: str | None = None,
     ):
-        # TODO(justinchuby): Include shape as well
         super().__init__(
             name,
             _enums.AttributeType.TYPE_PROTO,
             value,
             doc_string=doc_string,
         )
+
+
+class AttrTypeProtos(_SpecializedAttr):
+    def __init__(
+        self,
+        name: str,
+        value: Sequence[TypeAndShape],
+        doc_string: str | None = None,
+    ):
+        super().__init__(
+            name,
+            _enums.AttributeType.TYPE_PROTOS,
+            value,
+            doc_string=doc_string,
+        )
```

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/ir/_display.py` & `onnxscript-0.1.0.dev20240507/onnxscript/ir/_display.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/ir/_enums.py` & `onnxscript-0.1.0.dev20240507/onnxscript/ir/_enums.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/ir/_graph_comparison.py` & `onnxscript-0.1.0.dev20240507/onnxscript/ir/_graph_comparison.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/ir/_invariants.py` & `onnxscript-0.1.0.dev20240507/onnxscript/ir/_invariants.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/ir/_linked_list.py` & `onnxscript-0.1.0.dev20240507/onnxscript/ir/_linked_list.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/ir/_metadata.py` & `onnxscript-0.1.0.dev20240507/onnxscript/ir/_metadata.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/ir/_name_authority.py` & `onnxscript-0.1.0.dev20240507/onnxscript/ir/_name_authority.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/ir/_protocols.py` & `onnxscript-0.1.0.dev20240507/onnxscript/ir/_protocols.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/ir/_type_casting.py` & `onnxscript-0.1.0.dev20240507/onnxscript/ir/_type_casting.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/ir/serde.py` & `onnxscript-0.1.0.dev20240507/onnxscript/ir/serde.py`

 * *Files 6% similar despite different names*

```diff
@@ -462,14 +462,15 @@
     # Fill in values for graph outputs
     outputs = [deserialize_value_info_proto(info, values[info.name]) for info in proto.output]
     scoped_values.pop()
     return _core.Graph(
         inputs,
         outputs,
         nodes=nodes,
+        # TODO(justinchuby): Attach the values associated with the initializers
         initializers=initializers,
         doc_string=_get_field(proto, "doc_string"),
         name=_get_field(proto, "name"),
         metadata_props=deserialize_metadata_props(proto.metadata_props),
     )
 
 
@@ -629,14 +630,25 @@
             length=external_info.length,
             dtype=_enums.DataType(proto.data_type),
             name=proto.name,
             shape=_core.Shape(proto.dims),
             doc_string=proto.doc_string,
             metadata_props=deserialize_metadata_props(proto.metadata_props),
         )
+    if proto.data_type == _enums.DataType.STRING:
+        name = _get_field(proto, "name")
+        doc_string = _get_field(proto, "doc_string")
+        metadata_props = deserialize_metadata_props(proto.metadata_props)
+        return _core.StringTensor(
+            proto.string_data,
+            shape=_core.Shape(proto.dims),
+            name=name,
+            doc_string=doc_string,
+            metadata_props=metadata_props,
+        )
     return TensorProtoTensor(proto)
 
 
 def deserialize_metadata_props(
     proto: Sequence[onnx.StringStringEntryProto],
 ) -> dict[str, str] | None:
     if len(proto) == 0:
@@ -687,15 +699,33 @@
         )
     if type_ == _enums.AttributeType.GRAPHS:
         return _core.AttrGraphs(
             name,
             [_deserialize_graph(g, scoped_values) for g in proto.graphs],
             doc_string=doc_string,
         )
-    # TODO: Handle type protos etc.
+    if type_ == _enums.AttributeType.SPARSE_TENSOR:
+        raise NotImplementedError("Sparse tensors are not supported yet")
+    if type_ == _enums.AttributeType.SPARSE_TENSORS:
+        raise NotImplementedError("Sparse tensors are not supported yet")
+    if type_ == _enums.AttributeType.TYPE_PROTO:
+        ir_type = deserialize_type_proto_for_type(proto.tp)
+        shape = deserialize_type_proto_for_shape(proto.tp)
+        return _core.AttrTypeProto(
+            name, _core.TypeAndShape(ir_type, shape), doc_string=doc_string
+        )
+    if type_ == _enums.AttributeType.TYPE_PROTOS:
+        type_and_shapes = []
+        for type_proto in proto.type_protos:
+            ir_type = deserialize_type_proto_for_type(type_proto)
+            shape = deserialize_type_proto_for_shape(type_proto)
+            type_and_shapes.append(_core.TypeAndShape(ir_type, shape))
+        return _core.AttrTypeProtos(name, type_and_shapes, doc_string=doc_string)
+    if type_ == _enums.AttributeType.UNDEFINED:
+        return _core.Attr(name, type_, None, doc_string=doc_string)
     raise ValueError(f"Unsupported attribute type: '{type_}'")
 
 
 def deserialize_node(proto: onnx.NodeProto) -> _core.Node:
     return _deserialize_node(proto, scoped_values=[], value_info={})
 
 
@@ -1074,14 +1104,16 @@
             "offset": from_.offset,
             "length": from_.length,
         }.items():
             if v is not None:
                 entry = tensor_proto.external_data.add()
                 entry.key = k
                 entry.value = str(v)
+    elif isinstance(from_, _core.StringTensor):
+        tensor_proto.string_data.extend(from_.string_data())
     else:
         tensor_proto.raw_data = from_.tobytes()
     _serialize_metadata_props_into(tensor_proto.metadata_props, from_.metadata_props)
 
 
 def serialize_attribute(attribute: _protocols.AttributeProtocol) -> onnx.AttributeProto:
     attribute_proto = onnx.AttributeProto()
@@ -1098,45 +1130,77 @@
     _fill_in_value_for_attribute(attribute_proto, from_.type, from_.value)
 
 
 def _fill_in_value_for_attribute(
     attribute_proto: onnx.AttributeProto, type_: _enums.AttributeType, value: Any
 ) -> None:
     if type_ == _enums.AttributeType.INT:
+        # value: int
         attribute_proto.i = value
         attribute_proto.type = onnx.AttributeProto.INT
     elif type_ == _enums.AttributeType.FLOAT:
+        # value: float
         attribute_proto.f = value
         attribute_proto.type = onnx.AttributeProto.FLOAT
     elif type_ == _enums.AttributeType.STRING:
+        # value: str
         attribute_proto.s = value.encode("utf-8")
         attribute_proto.type = onnx.AttributeProto.STRING
     elif type_ == _enums.AttributeType.INTS:
+        # value: Sequence[int]
         attribute_proto.ints.extend(value)
         attribute_proto.type = onnx.AttributeProto.INTS
     elif type_ == _enums.AttributeType.FLOATS:
+        # value: Sequence[float]
         attribute_proto.floats.extend(value)
         attribute_proto.type = onnx.AttributeProto.FLOATS
     elif type_ == _enums.AttributeType.STRINGS:
+        # value: Sequence[str]
         attribute_proto.strings.extend([s.encode("utf-8") for s in value])
         attribute_proto.type = onnx.AttributeProto.STRINGS
     elif type_ == _enums.AttributeType.TENSOR:
+        # value: _protocols.TensorProtocol
         serialize_tensor_into(attribute_proto.t, value)
         attribute_proto.type = onnx.AttributeProto.TENSOR
     elif type_ == _enums.AttributeType.GRAPH:
+        # value: _protocols.GraphProtocol
         serialize_graph_into(attribute_proto.g, value)
         attribute_proto.type = onnx.AttributeProto.GRAPH
     elif type_ == _enums.AttributeType.TENSORS:
+        # value: Sequence[_protocols.TensorProtocol]
         for tensor in value:
             serialize_tensor_into(attribute_proto.tensors.add(), tensor)
         attribute_proto.type = onnx.AttributeProto.TENSORS
     elif type_ == _enums.AttributeType.GRAPHS:
+        # value: Sequence[_protocols.GraphProtocol]
         for graph in value:
             serialize_graph_into(attribute_proto.graphs.add(), graph)
         attribute_proto.type = onnx.AttributeProto.GRAPHS
+    elif type_ == _enums.AttributeType.SPARSE_TENSOR:
+        raise NotImplementedError("Sparse tensors are not supported yet")
+    elif type_ == _enums.AttributeType.SPARSE_TENSORS:
+        raise NotImplementedError("Sparse tensors are not supported yet")
+    elif type_ == _enums.AttributeType.TYPE_PROTO:
+        # value: _core.TypeAndShape
+        if value.type is not None:
+            serialize_type_into(attribute_proto.tp, value.type)
+        # Need to create the type _before_ writing the shape
+        if value.shape is not None:
+            serialize_shape_into(attribute_proto.tp, value.shape)
+        attribute_proto.type = onnx.AttributeProto.TYPE_PROTO
+    elif type_ == _enums.AttributeType.TYPE_PROTOS:
+        for ir_type in value:
+            # ir_type: _core.TypeAndShape
+            type_proto = attribute_proto.type_protos.add()
+            if ir_type.type is not None:
+                serialize_type_into(type_proto, ir_type.type)
+            # Need to create the type _before_ writing the shape so that the shape can be written to the leaf type proto
+            if ir_type.shape is not None:
+                serialize_shape_into(type_proto, ir_type.shape)
+        attribute_proto.type = onnx.AttributeProto.TYPE_PROTOS
     else:
         raise TypeError(f"Unsupported attribute type: {type_}")
 
 
 def serialize_reference_attribute_into(
     attribute_proto: onnx.AttributeProto, from_: _protocols.ReferenceAttributeProtocol
 ) -> None:
@@ -1175,18 +1239,19 @@
     """
     if name:
         value_info_proto.name = name
     else:
         value_info_proto.name = from_.name
     if from_.metadata_props:
         _serialize_metadata_props_into(value_info_proto.metadata_props, from_.metadata_props)
-    if from_.shape is not None:
-        serialize_shape_into(value_info_proto.type, from_.shape)
     if from_.type is not None:
         serialize_type_into(value_info_proto.type, from_.type)
+    # Need to create the type _before_ writing the shape so that the shape can be written to the leaf type proto
+    if from_.shape is not None:
+        serialize_shape_into(value_info_proto.type, from_.shape)
 
 
 def serialize_type_into(type_proto: onnx.TypeProto, from_: _protocols.TypeProtocol) -> None:
     if from_.denotation:
         type_proto.denotation = from_.denotation
     if isinstance(from_, _core.TensorType):
         tensor_type_proto = type_proto.tensor_type
@@ -1201,26 +1266,34 @@
         optional_type_proto = type_proto.optional_type
         serialize_type_into(optional_type_proto.elem_type, from_.elem_type)
     else:
         raise TypeError(f"Unsupported type: {from_}")
 
 
 def serialize_shape_into(type_proto: onnx.TypeProto, from_: _protocols.ShapeProtocol) -> None:
-    tensor_type_proto = type_proto.tensor_type
+    value_field = type_proto.WhichOneof("value")
+    tensor_type = getattr(type_proto, value_field)
+    while not isinstance(tensor_type.elem_type, int):
+        # Find the leaf type that has the shape field
+        type_proto = tensor_type.elem_type
+        value_field = type_proto.WhichOneof("value")
+        tensor_type = getattr(type_proto, value_field)
     # When from is empty, we still need to set the shape field to an empty list by touching it
-    tensor_type_proto.shape.ClearField("dim")
+    tensor_type.shape.ClearField("dim")
     for i, dim in enumerate(from_):
         denotation = from_.get_denotation(i)
-        serialize_dimension_into(tensor_type_proto.shape.dim.add(), dim, denotation)
+        serialize_dimension_into(tensor_type.shape.dim.add(), dim, denotation)
 
 
 def serialize_dimension_into(
     dim_proto: onnx.TensorShapeProto.Dimension,
     dim: int | _protocols.SymbolicDimProtocol,
     denotation: str | None = None,
 ) -> None:
     if denotation:
         dim_proto.denotation = denotation
     if isinstance(dim, int):
         dim_proto.dim_value = dim
     elif isinstance(dim, (_core.SymbolicDim, _protocols.SymbolicDimProtocol)):
-        dim_proto.dim_param = str(dim.value)
+        if dim.value is not None:
+            # TODO(justinchuby): None is probably not a valid value for dim_param
+            dim_proto.dim_param = str(dim.value)
```

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/irbuilder.py` & `onnxscript-0.1.0.dev20240507/onnxscript/irbuilder.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/main.py` & `onnxscript-0.1.0.dev20240507/onnxscript/main.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/onnx_opset/__init__.py` & `onnxscript-0.1.0.dev20240507/onnxscript/onnx_opset/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/onnx_opset/_impl/opset1.py` & `onnxscript-0.1.0.dev20240507/onnxscript/onnx_opset/_impl/opset1.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/onnx_opset/_impl/opset10.py` & `onnxscript-0.1.0.dev20240507/onnxscript/onnx_opset/_impl/opset10.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/onnx_opset/_impl/opset11.py` & `onnxscript-0.1.0.dev20240507/onnxscript/onnx_opset/_impl/opset11.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/onnx_opset/_impl/opset12.py` & `onnxscript-0.1.0.dev20240507/onnxscript/onnx_opset/_impl/opset12.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/onnx_opset/_impl/opset13.py` & `onnxscript-0.1.0.dev20240507/onnxscript/onnx_opset/_impl/opset13.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/onnx_opset/_impl/opset14.py` & `onnxscript-0.1.0.dev20240507/onnxscript/onnx_opset/_impl/opset14.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/onnx_opset/_impl/opset15.py` & `onnxscript-0.1.0.dev20240507/onnxscript/onnx_opset/_impl/opset15.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/onnx_opset/_impl/opset16.py` & `onnxscript-0.1.0.dev20240507/onnxscript/onnx_opset/_impl/opset16.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/onnx_opset/_impl/opset17.py` & `onnxscript-0.1.0.dev20240507/onnxscript/onnx_opset/_impl/opset17.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/onnx_opset/_impl/opset18.py` & `onnxscript-0.1.0.dev20240507/onnxscript/onnx_opset/_impl/opset18.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/onnx_opset/_impl/opset19.py` & `onnxscript-0.1.0.dev20240507/onnxscript/onnx_opset/_impl/opset19.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/onnx_opset/_impl/opset2.py` & `onnxscript-0.1.0.dev20240507/onnxscript/onnx_opset/_impl/opset2.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/onnx_opset/_impl/opset20.py` & `onnxscript-0.1.0.dev20240507/onnxscript/onnx_opset/_impl/opset20.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/onnx_opset/_impl/opset3.py` & `onnxscript-0.1.0.dev20240507/onnxscript/onnx_opset/_impl/opset3.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/onnx_opset/_impl/opset4.py` & `onnxscript-0.1.0.dev20240507/onnxscript/onnx_opset/_impl/opset4.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/onnx_opset/_impl/opset5.py` & `onnxscript-0.1.0.dev20240507/onnxscript/onnx_opset/_impl/opset5.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/onnx_opset/_impl/opset6.py` & `onnxscript-0.1.0.dev20240507/onnxscript/onnx_opset/_impl/opset6.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/onnx_opset/_impl/opset7.py` & `onnxscript-0.1.0.dev20240507/onnxscript/onnx_opset/_impl/opset7.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/onnx_opset/_impl/opset8.py` & `onnxscript-0.1.0.dev20240507/onnxscript/onnx_opset/_impl/opset8.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/onnx_opset/_impl/opset9.py` & `onnxscript-0.1.0.dev20240507/onnxscript/onnx_opset/_impl/opset9.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml1.py` & `onnxscript-0.1.0.dev20240507/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml1.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml2.py` & `onnxscript-0.1.0.dev20240507/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml2.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml3.py` & `onnxscript-0.1.0.dev20240507/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml3.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml4.py` & `onnxscript-0.1.0.dev20240507/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml4.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/onnx_opset/_impl/opset_ai_onnx_preview_training1.py` & `onnxscript-0.1.0.dev20240507/onnxscript/onnx_opset/_impl/opset_ai_onnx_preview_training1.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/onnx_types.py` & `onnxscript-0.1.0.dev20240507/onnxscript/onnx_types.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/optimizer/__init__.py` & `onnxscript-0.1.0.dev20240507/onnxscript/optimizer/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/optimizer/constant_folding.py` & `onnxscript-0.1.0.dev20240507/onnxscript/optimizer/constant_folding.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/optimizer/evaluator.py` & `onnxscript-0.1.0.dev20240507/onnxscript/optimizer/evaluator.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/optimizer/fold_constants_v0.py` & `onnxscript-0.1.0.dev20240507/onnxscript/optimizer/fold_constants_v0.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/optimizer/remove_unused.py` & `onnxscript-0.1.0.dev20240507/onnxscript/optimizer/remove_unused.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/optimizer/remove_unused_function.py` & `onnxscript-0.1.0.dev20240507/onnxscript/optimizer/remove_unused_function.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/optimizer/simple_function_folding.py` & `onnxscript-0.1.0.dev20240507/onnxscript/optimizer/simple_function_folding.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/rewriter/__init__.py` & `onnxscript-0.1.0.dev20240507/onnxscript/rewriter/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/rewriter/_ir_utils.py` & `onnxscript-0.1.0.dev20240507/onnxscript/rewriter/_ir_utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/rewriter/_tape.py` & `onnxscript-0.1.0.dev20240507/onnxscript/rewriter/_tape.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/rewriter/broadcast_to_matmul.py` & `onnxscript-0.1.0.dev20240507/onnxscript/rewriter/broadcast_to_matmul.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/rewriter/cast_constant_of_shape.py` & `onnxscript-0.1.0.dev20240507/onnxscript/rewriter/cast_constant_of_shape.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/rewriter/erfgelu.py` & `onnxscript-0.1.0.dev20240507/onnxscript/rewriter/erfgelu.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/rewriter/function_rule.py` & `onnxscript-0.1.0.dev20240507/onnxscript/rewriter/function_rule.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/rewriter/gemm_to_matmul_add.py` & `onnxscript-0.1.0.dev20240507/onnxscript/rewriter/gemm_to_matmul_add.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/rewriter/generic_pattern.py` & `onnxscript-0.1.0.dev20240507/onnxscript/rewriter/generic_pattern.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/rewriter/no_op.py` & `onnxscript-0.1.0.dev20240507/onnxscript/rewriter/no_op.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/rewriter/onnxruntime/__init__.py` & `onnxscript-0.1.0.dev20240507/onnxscript/rewriter/onnxruntime/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/rewriter/onnxruntime/group_normalization_merge_silu.py` & `onnxscript-0.1.0.dev20240507/onnxscript/rewriter/onnxruntime/group_normalization_merge_silu.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/rewriter/onnxruntime/instance_to_group_normalization.py` & `onnxscript-0.1.0.dev20240507/onnxscript/rewriter/onnxruntime/instance_to_group_normalization.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/rewriter/onnxruntime/softmax.py` & `onnxscript-0.1.0.dev20240507/onnxscript/rewriter/onnxruntime/softmax.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/rewriter/onnxruntime/transformers/__init__.py` & `onnxscript-0.1.0.dev20240507/onnxscript/rewriter/onnxruntime/transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/rewriter/onnxruntime/transformers/biassplitgelu.py` & `onnxscript-0.1.0.dev20240507/onnxscript/rewriter/onnxruntime/transformers/biassplitgelu.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/rewriter/onnxruntime/transformers/fastgelu.py` & `onnxscript-0.1.0.dev20240507/onnxscript/rewriter/onnxruntime/transformers/fastgelu.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/rewriter/onnxruntime/transformers/layernorm.py` & `onnxscript-0.1.0.dev20240507/onnxscript/rewriter/onnxruntime/transformers/layernorm.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/rewriter/onnxruntime/transformers/multihead_attention.py` & `onnxscript-0.1.0.dev20240507/onnxscript/rewriter/onnxruntime/transformers/multihead_attention.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/rewriter/pattern.py` & `onnxscript-0.1.0.dev20240507/onnxscript/rewriter/pattern.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/sourceinfo.py` & `onnxscript-0.1.0.dev20240507/onnxscript/sourceinfo.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/tensor.py` & `onnxscript-0.1.0.dev20240507/onnxscript/tensor.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/testing/__init__.py` & `onnxscript-0.1.0.dev20240507/onnxscript/testing/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
     "assert_isomorphic",
     "assert_isomorphic_graph",
     "assert_isomorphic_function",
     "assert_onnx_proto_equal",
 ]
 
 import difflib
+import math
 from typing import Any, Collection, Sequence
 
 import google.protobuf.message
 import onnx
 from onnx import parser
 
 import onnxscript
@@ -444,20 +445,36 @@
                 ):
                     try:
                         assert_onnx_proto_equal(a_value_i, b_value_i)
                     except AssertionError as e:
                         error_message = f"Field {field} index {i} in sequence not equal. type(a_value_i): {type(a_value_i)}, type(b_value_i): {type(b_value_i)}, a_value_i: {a_value_i}, b_value_i: {b_value_i}"
                         raise AssertionError(error_message) from e
                 elif a_value_i != b_value_i:
+                    if (
+                        isinstance(a_value_i, float)
+                        and isinstance(b_value_i, float)
+                        and math.isnan(a_value_i)
+                        and math.isnan(b_value_i)
+                    ):
+                        # Consider NaNs equal
+                        continue
                     error_message = f"Field {field} index {i} in sequence not equal. type(a_value_i): {type(a_value_i)}, type(b_value_i): {type(b_value_i)}"
                     for line in difflib.ndiff(
                         str(a_value_i).splitlines(), str(b_value_i).splitlines()
                     ):
                         error_message += "\n" + line
                     raise AssertionError(error_message)
         elif isinstance(a_value, google.protobuf.message.Message) and isinstance(
             b_value, google.protobuf.message.Message
         ):
             assert_onnx_proto_equal(a_value, b_value)
         elif a_value != b_value:
+            if (
+                isinstance(a_value, float)
+                and isinstance(b_value, float)
+                and math.isnan(a_value)
+                and math.isnan(b_value)
+            ):
+                # Consider NaNs equal
+                continue
             error_message = f"Field {field} not equal. field_a: {a_value}, field_b: {b_value}"
             raise AssertionError(error_message)
```

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/type_annotation.py` & `onnxscript-0.1.0.dev20240507/onnxscript/type_annotation.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/utils/evaluation_utils.py` & `onnxscript-0.1.0.dev20240507/onnxscript/utils/evaluation_utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/utils/timing_utils.py` & `onnxscript-0.1.0.dev20240507/onnxscript/utils/timing_utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/utils/utils.py` & `onnxscript-0.1.0.dev20240507/onnxscript/utils/utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript/values.py` & `onnxscript-0.1.0.dev20240507/onnxscript/values.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript.egg-info/PKG-INFO` & `onnxscript-0.1.0.dev20240507/onnxscript.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onnxscript
-Version: 0.1.0.dev20240506
+Version: 0.1.0.dev20240507
 Summary: Naturally author ONNX functions and models using a subset of Python
 Author-email: Microsoft Corporation <onnx@microsoft.com>
 License: MIT License
         
         Copyright (c) Microsoft Corporation
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `onnxscript-0.1.0.dev20240506/onnxscript.egg-info/SOURCES.txt` & `onnxscript-0.1.0.dev20240507/onnxscript.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/pyproject.toml` & `onnxscript-0.1.0.dev20240507/pyproject.toml`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240506/setup.py` & `onnxscript-0.1.0.dev20240507/setup.py`

 * *Files identical despite different names*

