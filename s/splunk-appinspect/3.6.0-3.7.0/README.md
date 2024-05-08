# Comparing `tmp/splunk-appinspect-3.6.0.tar.gz` & `tmp/splunk-appinspect-3.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/splunk-appinspect-3.6.0.tar", last modified: Tue Apr  9 11:29:31 2024, max compression
+gzip compressed data, was "dist/splunk-appinspect-3.7.0.tar", last modified: Wed May  8 08:47:46 2024, max compression
```

## Comparing `splunk-appinspect-3.6.0.tar` & `splunk-appinspect-3.7.0.tar`

### file list

```diff
@@ -1,448 +1,448 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.346859 splunk-appinspect-3.6.0/
--rw-rw-rw-   0 root         (0) root         (0)      270 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1332 2024-04-09 11:29:31.346859 splunk-appinspect-3.6.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5702 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)      518 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1247 2024-04-09 11:29:31.346859 splunk-appinspect-3.6.0/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     4172 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.294859 splunk-appinspect-3.6.0/splunk_appinspect/
--rw-rw-rw-   0 root         (0) root         (0)     1077 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11155 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/alert_actions.py
--rw-rw-rw-   0 root         (0) root         (0)      354 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/alert_actions_configuration_file.py
--rw-rw-rw-   0 root         (0) root         (0)    57040 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/app.py
--rw-rw-rw-   0 root         (0) root         (0)     1287 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/app_configuration_file.py
--rw-rw-rw-   0 root         (0) root         (0)    42976 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/app_package_handler.py
--rw-rw-rw-   0 root         (0) root         (0)     2931 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/app_util.py
--rw-rw-rw-   0 root         (0) root         (0)      349 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/authentication_configuration_file.py
--rw-rw-rw-   0 root         (0) root         (0)      334 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/authorize_configuration_file.py
--rw-rw-rw-   0 root         (0) root         (0)      427 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/banned_wordlist.txt
--rw-rw-rw-   0 root         (0) root         (0)     1778 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/bias.py
--rw-rw-rw-   0 root         (0) root         (0)       32 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/bias_wordlist.txt
--rw-rw-rw-   0 root         (0) root         (0)     1275 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/canary_modules.py
--rw-rw-rw-   0 root         (0) root         (0)     3031 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/check_messages.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.298859 splunk-appinspect-3.6.0/splunk_appinspect/check_routine/
--rw-rw-rw-   0 root         (0) root         (0)     6301 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/check_routine/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1917 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/check_routine/find_endpoint_usage.py
--rw-rw-rw-   0 root         (0) root         (0)     3090 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/check_routine/find_spl_command_usage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.298859 splunk-appinspect-3.6.0/splunk_appinspect/check_routine/python_ast_searcher/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-09 11:28:58.000000 splunk-appinspect-3.6.0/splunk_appinspect/check_routine/python_ast_searcher/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4944 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/check_routine/python_ast_searcher/ast_searcher.py
--rw-rw-rw-   0 root         (0) root         (0)      444 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/check_routine/python_ast_searcher/node_filters.py
--rw-rw-rw-   0 root         (0) root         (0)    14985 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/check_routine/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.306859 splunk-appinspect-3.6.0/splunk_appinspect/checks/
--rw-rw-rw-   0 root         (0) root         (0)     5019 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/checks/check_addon_builder_config.py
--rw-rw-rw-   0 root         (0) root         (0)    10554 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/checks/check_alert_actions_config.py
--rw-rw-rw-   0 root         (0) root         (0)    38520 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/checks/check_app_configuration_file.py
--rw-rw-rw-   0 root         (0) root         (0)     8106 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/checks/check_application_content.py
--rw-rw-rw-   0 root         (0) root         (0)     5120 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/checks/check_application_structure.py
--rw-rw-rw-   0 root         (0) root         (0)     9133 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/checks/check_authentication_configuration_file.py
--rw-rw-rw-   0 root         (0) root         (0)     2458 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/checks/check_authorize_configuration_file.py
--rw-rw-rw-   0 root         (0) root         (0)     1635 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/checks/check_bias_language.py
--rw-rw-rw-   0 root         (0) root         (0)    11922 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/checks/check_binary_files.py
--rw-rw-rw-   0 root         (0) root         (0)    93219 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/checks/check_cloud_simple_app.py
--rw-rw-rw-   0 root         (0) root         (0)    10168 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/checks/check_configuration_files.py
--rw-rw-rw-   0 root         (0) root         (0)    15005 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/checks/check_custom_commands.py
--rw-rw-rw-   0 root         (0) root         (0)    35763 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/checks/check_custom_visualizations.py
--rw-rw-rw-   0 root         (0) root         (0)     6090 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/checks/check_data_models_config.py
--rw-rw-rw-   0 root         (0) root         (0)     4013 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/checks/check_documentation_for_sensitive_functionality.py
--rw-rw-rw-   0 root         (0) root         (0)     7509 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/checks/check_documentation_standards.py
--rw-rw-rw-   0 root         (0) root         (0)     5130 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/checks/check_for_indexer_synced_locals.py
--rw-rw-rw-   0 root         (0) root         (0)     7410 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/checks/check_frontend_libraries.py
--rw-rw-rw-   0 root         (0) root         (0)     1505 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/checks/check_git_conflict_file.py
--rw-rw-rw-   0 root         (0) root         (0)    11555 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/checks/check_indexes_configuration_file.py
--rw-rw-rw-   0 root         (0) root         (0)     1793 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/checks/check_itsi_module.py
--rw-rw-rw-   0 root         (0) root         (0)    11941 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/checks/check_javascript_files.py
--rw-rw-rw-   0 root         (0) root         (0)     6013 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/checks/check_jquery_standards.py
--rw-rw-rw-   0 root         (0) root         (0)     1351 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/checks/check_json_files.py
--rw-rw-rw-   0 root         (0) root         (0)     2046 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/checks/check_limits_configuration_file.py
--rw-rw-rw-   0 root         (0) root         (0)     5294 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/checks/check_lookup_files.py
--rw-rw-rw-   0 root         (0) root         (0)     4717 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/checks/check_malware.py
--rw-rw-rw-   0 root         (0) root         (0)     4995 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/checks/check_meta_files.py
--rw-rw-rw-   0 root         (0) root         (0)    15802 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/checks/check_modular_inputs.py
--rw-rw-rw-   0 root         (0) root         (0)     2838 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/checks/check_outputs_configuration_file.py
--rw-rw-rw-   0 root         (0) root         (0)    26539 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/checks/check_packaging_standards.py
--rw-rw-rw-   0 root         (0) root         (0)     5423 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/checks/check_potentially_harmful_operations.py
--rw-rw-rw-   0 root         (0) root         (0)    25269 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/checks/check_props_configuration_file.py
--rw-rw-rw-   0 root         (0) root         (0)    42923 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/checks/check_python_files.py
--rw-rw-rw-   0 root         (0) root         (0)     1922 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/checks/check_readme_spec_files.py
--rw-rw-rw-   0 root         (0) root         (0)     7519 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/checks/check_rest_endpoints.py
--rw-rw-rw-   0 root         (0) root         (0)    21103 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/checks/check_saved_searches.py
--rwxrwxrwx   0 root         (0) root         (0)    32660 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/checks/check_security.py
--rw-rw-rw-   0 root         (0) root         (0)     3894 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/checks/check_server_configuration_file.py
--rwxrwxrwx   0 root         (0) root         (0)     8583 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/checks/check_source_and_binaries.py
--rw-rw-rw-   0 root         (0) root         (0)     4241 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/checks/check_splunk_5_0_deprecated_features.py
--rw-rw-rw-   0 root         (0) root         (0)     2983 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/checks/check_splunk_6_0_deprecated_features.py
--rw-rw-rw-   0 root         (0) root         (0)     1521 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/checks/check_splunk_6_1_deprecated_features.py
--rw-rw-rw-   0 root         (0) root         (0)     7075 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/checks/check_splunk_6_2_deprecated_features.py
--rw-rw-rw-   0 root         (0) root         (0)    10039 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/checks/check_splunk_6_3_deprecated_features.py
--rw-rw-rw-   0 root         (0) root         (0)    12198 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/checks/check_splunk_6_4_deprecated_features.py
--rw-rw-rw-   0 root         (0) root         (0)     3502 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/checks/check_splunk_6_5_deprecated_features.py
--rw-rw-rw-   0 root         (0) root         (0)     5140 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/checks/check_splunk_6_6_deprecated_features.py
--rw-rw-rw-   0 root         (0) root         (0)     2910 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/checks/check_splunk_7_1_deprecated_features.py
--rw-rw-rw-   0 root         (0) root         (0)     1918 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/checks/check_splunk_7_2_deprecated_features.py
--rw-rw-rw-   0 root         (0) root         (0)     3087 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/checks/check_splunk_7_3_deprecated_features.py
--rw-rw-rw-   0 root         (0) root         (0)    12727 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/checks/check_splunk_8_0_deprecated_features.py
--rw-rw-rw-   0 root         (0) root         (0)     1944 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/checks/check_splunk_9_0_deprecated_features.py
--rw-rw-rw-   0 root         (0) root         (0)     1147 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/checks/check_support_requirements.py
--rw-rw-rw-   0 root         (0) root         (0)     4861 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/checks/check_transforms_configuration_file.py
--rw-rw-rw-   0 root         (0) root         (0)     9134 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/checks/check_web_configuration_file.py
--rw-rw-rw-   0 root         (0) root         (0)     4190 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/checks/check_workflow_actions.py
--rw-rw-rw-   0 root         (0) root         (0)     5073 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/checks/check_xml_files.py
--rw-rw-rw-   0 root         (0) root         (0)    28306 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/checks/class_based_checks_guide.md
--rw-rw-rw-   0 root         (0) root         (0)     1248 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/checks/disabled_check_splunk_future_deprecated_features.py
--rw-rw-rw-   0 root         (0) root         (0)    82204 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/checks.py
--rw-rw-rw-   0 root         (0) root         (0)      427 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/collections_configuration_file.py
--rw-rw-rw-   0 root         (0) root         (0)     5689 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/command_line_helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.306859 splunk-appinspect-3.6.0/splunk_appinspect/common/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-09 11:28:58.000000 splunk-appinspect-3.6.0/splunk_appinspect/common/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      374 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/common/file_hash.py
--rw-rw-rw-   0 root         (0) root         (0)     8663 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/common/string_utils.py
--rw-rw-rw-   0 root         (0) root         (0)    17928 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/configuration_file.py
--rw-rw-rw-   0 root         (0) root         (0)     5963 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/configuration_parser.py
--rw-rw-rw-   0 root         (0) root         (0)     1763 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     2990 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/cron_expression.py
--rw-rw-rw-   0 root         (0) root         (0)    12526 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/custom_commands.py
--rw-rw-rw-   0 root         (0) root         (0)     1636 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/custom_types.py
--rw-rw-rw-   0 root         (0) root         (0)     5288 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/custom_visualizations.py
--rw-rw-rw-   0 root         (0) root         (0)     1052 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/decorators.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.306859 splunk-appinspect-3.6.0/splunk_appinspect/documentation/
--rw-rw-rw-   0 root         (0) root         (0)      196 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/documentation/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3785 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/documentation/cli_docs.py
--rw-rw-rw-   0 root         (0) root         (0)     2991 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/documentation/criteria_generator.py
--rw-rw-rw-   0 root         (0) root         (0)      635 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/documentation/splunk_docs.py
--rw-rw-rw-   0 root         (0) root         (0)     2894 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/documentation/tag_reference_generator.py
--rw-rw-rw-   0 root         (0) root         (0)      447 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/environment_validator.py
--rw-rw-rw-   0 root         (0) root         (0)     3869 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/feedback_file_generator.py
--rw-rw-rw-   0 root         (0) root         (0)     1447 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/file_resource.py
--rw-rw-rw-   0 root         (0) root         (0)    10797 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/file_view.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.306859 splunk-appinspect-3.6.0/splunk_appinspect/formatters/
--rw-rw-rw-   0 root         (0) root         (0)      357 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/formatters/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      429 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/formatters/date_time_encoder.py
--rw-rw-rw-   0 root         (0) root         (0)      543 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/formatters/validation_report_formatter.py
--rw-rw-rw-   0 root         (0) root         (0)     6288 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/formatters/validation_report_json_formatter.py
--rw-rw-rw-   0 root         (0) root         (0)     8384 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/formatters/validation_report_junitxml_formatter.py
--rw-rw-rw-   0 root         (0) root         (0)      830 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/image_resource.py
--rw-rw-rw-   0 root         (0) root         (0)      421 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/indexes_configuration_file.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.306859 splunk-appinspect-3.6.0/splunk_appinspect/infra/
--rw-rw-rw-   0 root         (0) root         (0)     1006 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/infra/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      981 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/infra/log_utils.py
--rw-rw-rw-   0 root         (0) root         (0)      380 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/inputs_configuration_file.py
--rw-rw-rw-   0 root         (0) root         (0)      375 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/inputs_specification_file.py
--rw-rw-rw-   0 root         (0) root         (0)     8403 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/inspected_file.py
--rw-rw-rw-   0 root         (0) root         (0)      586 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/iter_ext.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.306859 splunk-appinspect-3.6.0/splunk_appinspect/listeners/
--rw-rw-rw-   0 root         (0) root         (0)      226 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/listeners/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3991 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/listeners/cert_status_listener.py
--rw-rw-rw-   0 root         (0) root         (0)     3778 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/listeners/dot_status_listener.py
--rw-rw-rw-   0 root         (0) root         (0)      507 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/listeners/listener.py
--rw-rw-rw-   0 root         (0) root         (0)     5841 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/lookup.py
--rwxrwxrwx   0 root         (0) root         (0)    26203 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/main.py
--rw-rw-rw-   0 root         (0) root         (0)    15254 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/modular_inputs.py
--rw-rw-rw-   0 root         (0) root         (0)     1597 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/mutually_exclusive_option.py
--rw-rw-rw-   0 root         (0) root         (0)     1956 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/offense.py
--rw-rw-rw-   0 root         (0) root         (0)      370 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/outputs_configuration_file.py
--rw-rw-rw-   0 root         (0) root         (0)      393 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/props_configuration_file.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.310859 splunk-appinspect-3.6.0/splunk_appinspect/python_analyzer/
--rw-rw-rw-   0 root         (0) root         (0)      176 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_analyzer/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)   109167 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_analyzer/ast_analyzer.py
--rw-rw-rw-   0 root         (0) root         (0)    12307 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_analyzer/ast_info_query.py
--rw-rw-rw-   0 root         (0) root         (0)     2827 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_analyzer/ast_info_store.py
--rw-rw-rw-   0 root         (0) root         (0)    27144 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_analyzer/ast_types.py
--rw-rw-rw-   0 root         (0) root         (0)    12126 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_analyzer/client.py
--rw-rw-rw-   0 root         (0) root         (0)    18666 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_analyzer/file_dep_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.310859 splunk-appinspect-3.6.0/splunk_appinspect/python_analyzer/trustedlibs/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-09 11:28:58.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_analyzer/trustedlibs/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.326859 splunk-appinspect-3.6.0/splunk_appinspect/python_analyzer/trustedlibs/lib_files/
--rw-r--r--   0 root         (0) root         (0)     1404 2024-04-09 11:29:31.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_analyzer/trustedlibs/lib_files/checks_used_for_libs.csv
--rw-r--r--   0 root         (0) root         (0) 17023502 2024-04-09 11:29:31.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_analyzer/trustedlibs/lib_files/trusted_file_hashes.csv
--rw-r--r--   0 root         (0) root         (0)  1252134 2024-04-09 11:29:31.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_analyzer/trustedlibs/lib_files/trusted_libs_record.csv
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 11:29:31.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_analyzer/trustedlibs/lib_files/untrusted_file_hashes.csv
--rw-r--r--   0 root         (0) root         (0)       23 2024-04-09 11:29:31.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_analyzer/trustedlibs/lib_files/untrusted_libs_record.csv
--rw-rw-rw-   0 root         (0) root         (0)     2313 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_analyzer/trustedlibs/trusted_data_collector.py
--rw-rw-rw-   0 root         (0) root         (0)     1244 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_analyzer/trustedlibs/trusted_libs_manager.py
--rw-rw-rw-   0 root         (0) root         (0)      279 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_analyzer/trustedlibs/utilities.py
--rw-rw-rw-   0 root         (0) root         (0)    14673 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_analyzer/utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.326859 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-09 11:28:58.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.326859 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.326859 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/BaseHTTPServer/
--rw-rw-rw-   0 root         (0) root         (0)      486 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/BaseHTTPServer/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.326859 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/ConfigParser/
--rw-rw-rw-   0 root         (0) root         (0)      960 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/ConfigParser/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.330859 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/DocXMLRPCServer/
--rw-rw-rw-   0 root         (0) root         (0)      550 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/DocXMLRPCServer/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.330859 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/MimeWriter/
--rw-rw-rw-   0 root         (0) root         (0)      633 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/MimeWriter/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.330859 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/SimpleXMLRPCServer/
--rw-rw-rw-   0 root         (0) root         (0)      539 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/SimpleXMLRPCServer/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.330859 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/SocketServer/
--rw-rw-rw-   0 root         (0) root         (0)      658 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/SocketServer/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.330859 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/___configparser/
--rw-rw-rw-   0 root         (0) root         (0)      960 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/___configparser/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.330859 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/___socketserver/
--rw-rw-rw-   0 root         (0) root         (0)      698 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/___socketserver/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      247 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.330859 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/_thread/
--rw-rw-rw-   0 root         (0) root         (0)      387 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/_thread/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.330859 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/aifc/
--rw-rw-rw-   0 root         (0) root         (0)      474 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/aifc/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.330859 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/anydbm/
--rw-rw-rw-   0 root         (0) root         (0)      425 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/anydbm/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.330859 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/argparse/
--rw-rw-rw-   0 root         (0) root         (0)      507 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/argparse/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.330859 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/asynchat/
--rw-rw-rw-   0 root         (0) root         (0)      560 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/asynchat/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.330859 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/asyncore/
--rw-rw-rw-   0 root         (0) root         (0)     1126 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/asyncore/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.330859 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/base64/
--rw-rw-rw-   0 root         (0) root         (0)      739 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/base64/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.330859 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/binhex/
--rw-rw-rw-   0 root         (0) root         (0)      619 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/binhex/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.330859 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/bz2/
--rw-rw-rw-   0 root         (0) root         (0)      375 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/bz2/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.330859 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/cPickle/
--rw-rw-rw-   0 root         (0) root         (0)      767 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/cPickle/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.330859 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/chunk/
--rw-rw-rw-   0 root         (0) root         (0)      496 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/chunk/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.330859 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/cmd/
--rw-rw-rw-   0 root         (0) root         (0)      425 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/cmd/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.330859 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/code/
--rw-rw-rw-   0 root         (0) root         (0)      954 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/code/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.330859 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/commands/
--rw-rw-rw-   0 root         (0) root         (0)      783 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/commands/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.330859 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/crypt/
--rw-rw-rw-   0 root         (0) root         (0)      410 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/crypt/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.330859 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/csv/
--rw-rw-rw-   0 root         (0) root         (0)      684 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/csv/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.330859 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/dbm/
--rw-rw-rw-   0 root         (0) root         (0)      431 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/dbm/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.330859 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/dbm/dumb/
--rw-rw-rw-   0 root         (0) root         (0)      440 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/dbm/dumb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.330859 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/dbm/gnu/
--rw-rw-rw-   0 root         (0) root         (0)      394 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/dbm/gnu/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.330859 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/dbm/ndbm/
--rw-rw-rw-   0 root         (0) root         (0)      400 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/dbm/ndbm/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.330859 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/dircache/
--rw-rw-rw-   0 root         (0) root         (0)       43 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/dircache/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.330859 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/dl/
--rw-rw-rw-   0 root         (0) root         (0)      539 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/dl/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.330859 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/dumbdbm/
--rw-rw-rw-   0 root         (0) root         (0)      433 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/dumbdbm/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.330859 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/email/
--rw-rw-rw-   0 root         (0) root         (0)      545 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/email/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.334859 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/ftplib/
--rw-rw-rw-   0 root         (0) root         (0)      544 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/ftplib/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.334859 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/gc/
--rw-rw-rw-   0 root         (0) root         (0)      446 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/gc/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.334859 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/gdbm/
--rw-rw-rw-   0 root         (0) root         (0)      435 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/gdbm/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.334859 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/getpass/
--rw-rw-rw-   0 root         (0) root         (0)      366 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/getpass/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.334859 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/gzip/
--rw-rw-rw-   0 root         (0) root         (0)      571 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/gzip/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.334859 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/http/
--rw-rw-rw-   0 root         (0) root         (0)      114 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/http/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.334859 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/http/client/
--rw-rw-rw-   0 root         (0) root         (0)      467 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/http/client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.334859 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/http/server/
--rw-rw-rw-   0 root         (0) root         (0)      688 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/http/server/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.334859 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/httplib/
--rw-rw-rw-   0 root         (0) root         (0)      332 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/httplib/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.334859 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/httplib2/
--rw-rw-rw-   0 root         (0) root         (0)      356 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/httplib2/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.334859 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/imaplib/
--rw-rw-rw-   0 root         (0) root         (0)      767 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/imaplib/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.334859 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/imp/
--rw-rw-rw-   0 root         (0) root         (0)      524 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/imp/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.334859 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/importlib/
--rw-rw-rw-   0 root         (0) root         (0)      555 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/importlib/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.334859 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/imputil/
--rw-rw-rw-   0 root         (0) root         (0)      918 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/imputil/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.334859 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/inspect/
--rw-rw-rw-   0 root         (0) root         (0)      915 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/inspect/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.334859 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/io/
--rw-rw-rw-   0 root         (0) root         (0)     3620 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/io/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.334859 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/json/
--rw-rw-rw-   0 root         (0) root         (0)      568 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/json/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.334859 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/linecache/
--rw-rw-rw-   0 root         (0) root         (0)      835 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/linecache/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.334859 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/logging/
--rw-rw-rw-   0 root         (0) root         (0)      590 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/logging/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.334859 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/logging/config/
--rw-rw-rw-   0 root         (0) root         (0)      594 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/logging/config/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.334859 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/logging/handlers/
--rw-rw-rw-   0 root         (0) root         (0)     2068 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/logging/handlers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.334859 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/marshal/
--rw-rw-rw-   0 root         (0) root         (0)      524 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/marshal/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.334859 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/mimetools/
--rw-rw-rw-   0 root         (0) root         (0)      845 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/mimetools/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.334859 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/mimetypes/
--rw-rw-rw-   0 root         (0) root         (0)     1040 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/mimetypes/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.334859 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/mimify/
--rw-rw-rw-   0 root         (0) root         (0)      684 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/mimify/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.334859 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/mmap/
--rw-rw-rw-   0 root         (0) root         (0)      445 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/mmap/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.334859 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/modulefinder/
--rw-rw-rw-   0 root         (0) root         (0)      814 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/modulefinder/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.334859 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/multifile/
--rw-rw-rw-   0 root         (0) root         (0)     1181 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/multifile/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.334859 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/multiprocessing/
--rw-rw-rw-   0 root         (0) root         (0)      605 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/multiprocessing/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.334859 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/nntplib/
--rw-rw-rw-   0 root         (0) root         (0)      388 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/nntplib/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.338859 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/os/
--rw-rw-rw-   0 root         (0) root         (0)     4886 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/os/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.338859 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/os/path/
--rw-rw-rw-   0 root         (0) root         (0)      931 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/os/path/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.338859 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/pickle/
--rw-rw-rw-   0 root         (0) root         (0)      693 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/pickle/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.338859 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/pipes/
--rw-rw-rw-   0 root         (0) root         (0)      548 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/pipes/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.338859 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/pkgutil/
--rw-rw-rw-   0 root         (0) root         (0)      807 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/pkgutil/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.338859 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/plistlib/
--rw-rw-rw-   0 root         (0) root         (0)      733 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/plistlib/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.338859 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/poplib/
--rw-rw-rw-   0 root         (0) root         (0)      361 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/poplib/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.338859 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/posix/
--rw-rw-rw-   0 root         (0) root         (0)     2273 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/posix/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.338859 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/posixfile/
--rw-rw-rw-   0 root         (0) root         (0)      535 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/posixfile/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.338859 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/pty/
--rw-rw-rw-   0 root         (0) root         (0)      668 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/pty/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.338859 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/quopri/
--rw-rw-rw-   0 root         (0) root         (0)      769 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/quopri/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.338859 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/requests/
--rw-rw-rw-   0 root         (0) root         (0)     1991 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/requests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.338859 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/runpy/
--rw-rw-rw-   0 root         (0) root         (0)      725 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/runpy/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.338859 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/shelve/
--rw-rw-rw-   0 root         (0) root         (0)      354 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/shelve/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.338859 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/shutil/
--rw-rw-rw-   0 root         (0) root         (0)     1542 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/shutil/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.338859 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/smtplib/
--rw-rw-rw-   0 root         (0) root         (0)      851 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/smtplib/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.338859 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/socket/
--rw-rw-rw-   0 root         (0) root         (0)      743 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/socket/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.338859 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/sqlite3/
--rw-rw-rw-   0 root         (0) root         (0)      541 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/sqlite3/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.338859 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/subprocess/
--rw-rw-rw-   0 root         (0) root         (0)     1719 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/subprocess/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.338859 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/sunau/
--rw-rw-rw-   0 root         (0) root         (0)      679 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/sunau/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.338859 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/syslog/
--rw-rw-rw-   0 root         (0) root         (0)      550 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/syslog/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.338859 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/tarfile/
--rw-rw-rw-   0 root         (0) root         (0)      616 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/tarfile/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.338859 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/telnetlib/
--rw-rw-rw-   0 root         (0) root         (0)      597 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/telnetlib/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.338859 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/tempfile/
--rw-rw-rw-   0 root         (0) root         (0)     1059 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/tempfile/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.338859 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/termios/
--rw-rw-rw-   0 root         (0) root         (0)      459 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/termios/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.338859 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/thread/
--rw-rw-rw-   0 root         (0) root         (0)      326 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/thread/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.338859 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/threading/
--rw-rw-rw-   0 root         (0) root         (0)      543 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/threading/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.338859 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/trace/
--rw-rw-rw-   0 root         (0) root         (0)     1135 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/trace/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.338859 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/tty/
--rw-rw-rw-   0 root         (0) root         (0)      575 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/tty/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.338859 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/urllib/
--rw-rw-rw-   0 root         (0) root         (0)     1698 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/urllib/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.342859 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/urllib/request/
--rw-rw-rw-   0 root         (0) root         (0)     1467 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/urllib/request/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.342859 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/urllib2/
--rw-rw-rw-   0 root         (0) root         (0)      427 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/urllib2/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.342859 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/uu/
--rw-rw-rw-   0 root         (0) root         (0)      730 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/uu/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.342859 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/wave/
--rw-rw-rw-   0 root         (0) root         (0)      685 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/wave/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.342859 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/wsgiref/
--rw-rw-rw-   0 root         (0) root         (0)      182 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/wsgiref/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.342859 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/wsgiref/simple_server/
--rw-rw-rw-   0 root         (0) root         (0)      613 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/wsgiref/simple_server/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.342859 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/xml/
--rw-rw-rw-   0 root         (0) root         (0)       73 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/xml/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.342859 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/xml/dom/
--rw-rw-rw-   0 root         (0) root         (0)       78 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/xml/dom/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      582 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/xml/dom/minidom.py
--rw-rw-rw-   0 root         (0) root         (0)      397 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/xml/dom/pulldom.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.342859 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/xml/etree/
--rw-rw-rw-   0 root         (0) root         (0)     1077 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/xml/etree/ElementTree.py
--rw-rw-rw-   0 root         (0) root         (0)       74 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/xml/etree/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.342859 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/xml/sax/
--rw-rw-rw-   0 root         (0) root         (0)      368 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/xml/sax/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      459 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/xml/sax/xmlreader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.342859 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/xmlrpc/
--rw-rw-rw-   0 root         (0) root         (0)      126 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/xmlrpc/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.342859 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/xmlrpc/client/
--rw-rw-rw-   0 root         (0) root         (0)      434 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/xmlrpc/client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.342859 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/xmlrpc/server/
--rw-rw-rw-   0 root         (0) root         (0)      651 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/xmlrpc/server/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.342859 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/xmlrpclib/
--rw-rw-rw-   0 root         (0) root         (0)      406 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/xmlrpclib/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.342859 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/zipfile/
--rw-rw-rw-   0 root         (0) root         (0)      453 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/zipfile/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.342859 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/zipimport/
--rw-rw-rw-   0 root         (0) root         (0)      635 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/zipimport/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.342859 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata_common/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-09 11:28:58.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata_common/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3841 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata_common/metadata_consts.py
--rw-rw-rw-   0 root         (0) root         (0)      416 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata_common/metadata_decorator.py
--rw-rw-rw-   0 root         (0) root         (0)       96 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata_common/metadata_exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     6831 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata_common/metadata_types.py
--rw-rw-rw-   0 root         (0) root         (0)      843 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata_importer.py
--rw-rw-rw-   0 root         (0) root         (0)    16123 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/python_modules_metadata_store.py
--rw-rw-rw-   0 root         (0) root         (0)    23619 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/reflected_xss_detector.py
--rw-rw-rw-   0 root         (0) root         (0)    15016 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/regex_matcher.py
--rw-rw-rw-   0 root         (0) root         (0)    12564 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/reporter.py
--rw-rw-rw-   0 root         (0) root         (0)     2238 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/resource_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.342859 splunk-appinspect-3.6.0/splunk_appinspect/resources/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-09 11:28:58.000000 splunk-appinspect-3.6.0/splunk_appinspect/resources/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1536 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/resources/semgrep_recognized_extensions.json
--rw-rw-rw-   0 root         (0) root         (0)     9582 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/rest_map.py
--rw-rw-rw-   0 root         (0) root         (0)      401 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/rest_map_configuration_file.py
--rw-rw-rw-   0 root         (0) root         (0)     4784 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/saved_searches.py
--rw-rw-rw-   0 root         (0) root         (0)      442 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/saved_searches_configuration_file.py
--rw-rw-rw-   0 root         (0) root         (0)     1367 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/sideview_utils_modules.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.346859 splunk-appinspect-3.6.0/splunk_appinspect/splunk/
--rw-rw-rw-   0 root         (0) root         (0)      127 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/splunk/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.346859 splunk-appinspect-3.6.0/splunk_appinspect/splunk/jquery_checks_data/
--rw-rw-rw-   0 root         (0) root         (0)   194102 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/splunk/jquery_checks_data/disallowed_imports.json
--rw-rw-rw-   0 root         (0) root         (0)     2080 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/splunk/jquery_checks_data/risky_imports.json
--rw-rw-rw-   0 root         (0) root         (0)     7992 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/splunk/splunk_default_source_type_list.py
--rw-rw-rw-   0 root         (0) root         (0)     1802 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/splunk/splunk_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.346859 splunk-appinspect-3.6.0/splunk_appinspect/splunk/telemetry/
--rw-rw-rw-   0 root         (0) root         (0)       39 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/splunk/telemetry/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      526 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/splunk/telemetry/core.py
--rw-rw-rw-   0 root         (0) root         (0)     1408 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/splunk/telemetry/list.csv
--rw-rw-rw-   0 root         (0) root         (0)     1975 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/splunk/util.py
--rw-rw-rw-   0 root         (0) root         (0)     7992 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/splunk_default_source_type_list.py
--rw-rw-rw-   0 root         (0) root         (0)     5132 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/splunk_defined_authorize_capability_list.py
--rw-rw-rw-   0 root         (0) root         (0)     3402 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/splunk_defined_conf_file_list.py
--rw-rw-rw-   0 root         (0) root         (0)     3021 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/splunk_pretrained_sourcetypes_list.py
--rw-rw-rw-   0 root         (0) root         (0)      767 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/telemetry_configuration_file.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.346859 splunk-appinspect-3.6.0/splunk_appinspect/templates/
--rw-rw-rw-   0 root         (0) root         (0)     2782 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/templates/html_criteria.html
--rw-rw-rw-   0 root         (0) root         (0)     1727 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/templates/tag_reference.html
--rw-rw-rw-   0 root         (0) root         (0)    10003 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/validation_report.py
--rw-rw-rw-   0 root         (0) root         (0)    16793 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/validator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.346859 splunk-appinspect-3.6.0/splunk_appinspect/version/
--rw-rw-rw-   0 root         (0) root         (0)        6 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/version/VERSION.txt
--rw-rw-rw-   0 root         (0) root         (0)      106 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/version/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      596 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/version/version.py
--rw-rw-rw-   0 root         (0) root         (0)      356 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/visualizations_configuration_file.py
--rw-rw-rw-   0 root         (0) root         (0)      392 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/web_configuration_file.py
--rw-rw-rw-   0 root         (0) root         (0)      454 2024-04-09 11:28:56.000000 splunk-appinspect-3.6.0/splunk_appinspect/workflow_actions_configuration_file.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.298859 splunk-appinspect-3.6.0/splunk_appinspect.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1332 2024-04-09 11:29:31.000000 splunk-appinspect-3.6.0/splunk_appinspect.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    17979 2024-04-09 11:29:31.000000 splunk-appinspect-3.6.0/splunk_appinspect.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-09 11:29:31.000000 splunk-appinspect-3.6.0/splunk_appinspect.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       70 2024-04-09 11:29:31.000000 splunk-appinspect-3.6.0/splunk_appinspect.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      478 2024-04-09 11:29:31.000000 splunk-appinspect-3.6.0/splunk_appinspect.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       30 2024-04-09 11:29:31.000000 splunk-appinspect-3.6.0/splunk_appinspect.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.286859 splunk-appinspect-3.6.0/tarsec/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:29:31.346859 splunk-appinspect-3.6.0/tarsec/tarsec/
--rw-rw-rw-   0 root         (0) root         (0)      193 2024-04-09 11:29:01.000000 splunk-appinspect-3.6.0/tarsec/tarsec/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6069 2024-04-09 11:29:01.000000 splunk-appinspect-3.6.0/tarsec/tarsec/check_tar.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.623249 splunk-appinspect-3.7.0/
+-rw-rw-rw-   0 root         (0) root         (0)      270 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1332 2024-05-08 08:47:46.623249 splunk-appinspect-3.7.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5702 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      518 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1247 2024-05-08 08:47:46.623249 splunk-appinspect-3.7.0/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     4172 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.571249 splunk-appinspect-3.7.0/splunk_appinspect/
+-rw-rw-rw-   0 root         (0) root         (0)     1077 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11155 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/alert_actions.py
+-rw-rw-rw-   0 root         (0) root         (0)      354 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/alert_actions_configuration_file.py
+-rw-rw-rw-   0 root         (0) root         (0)    57040 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/app.py
+-rw-rw-rw-   0 root         (0) root         (0)     1287 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/app_configuration_file.py
+-rw-rw-rw-   0 root         (0) root         (0)    42976 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/app_package_handler.py
+-rw-rw-rw-   0 root         (0) root         (0)     2931 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/app_util.py
+-rw-rw-rw-   0 root         (0) root         (0)      349 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/authentication_configuration_file.py
+-rw-rw-rw-   0 root         (0) root         (0)      334 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/authorize_configuration_file.py
+-rw-rw-rw-   0 root         (0) root         (0)      427 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/banned_wordlist.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1778 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/bias.py
+-rw-rw-rw-   0 root         (0) root         (0)       32 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/bias_wordlist.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1275 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/canary_modules.py
+-rw-rw-rw-   0 root         (0) root         (0)     3031 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/check_messages.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.575249 splunk-appinspect-3.7.0/splunk_appinspect/check_routine/
+-rw-rw-rw-   0 root         (0) root         (0)     6301 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/check_routine/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1917 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/check_routine/find_endpoint_usage.py
+-rw-rw-rw-   0 root         (0) root         (0)     3090 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/check_routine/find_spl_command_usage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.575249 splunk-appinspect-3.7.0/splunk_appinspect/check_routine/python_ast_searcher/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-08 08:47:12.000000 splunk-appinspect-3.7.0/splunk_appinspect/check_routine/python_ast_searcher/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4944 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/check_routine/python_ast_searcher/ast_searcher.py
+-rw-rw-rw-   0 root         (0) root         (0)      444 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/check_routine/python_ast_searcher/node_filters.py
+-rw-rw-rw-   0 root         (0) root         (0)    14985 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/check_routine/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.583249 splunk-appinspect-3.7.0/splunk_appinspect/checks/
+-rw-rw-rw-   0 root         (0) root         (0)     4986 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/checks/check_addon_builder_config.py
+-rw-rw-rw-   0 root         (0) root         (0)    10554 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/checks/check_alert_actions_config.py
+-rw-rw-rw-   0 root         (0) root         (0)    38520 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/checks/check_app_configuration_file.py
+-rw-rw-rw-   0 root         (0) root         (0)     8106 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/checks/check_application_content.py
+-rw-rw-rw-   0 root         (0) root         (0)     5120 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/checks/check_application_structure.py
+-rw-rw-rw-   0 root         (0) root         (0)     9133 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/checks/check_authentication_configuration_file.py
+-rw-rw-rw-   0 root         (0) root         (0)     2458 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/checks/check_authorize_configuration_file.py
+-rw-rw-rw-   0 root         (0) root         (0)     1635 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/checks/check_bias_language.py
+-rw-rw-rw-   0 root         (0) root         (0)    11922 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/checks/check_binary_files.py
+-rw-rw-rw-   0 root         (0) root         (0)    93177 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/checks/check_cloud_simple_app.py
+-rw-rw-rw-   0 root         (0) root         (0)    10168 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/checks/check_configuration_files.py
+-rw-rw-rw-   0 root         (0) root         (0)    15005 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/checks/check_custom_commands.py
+-rw-rw-rw-   0 root         (0) root         (0)    35763 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/checks/check_custom_visualizations.py
+-rw-rw-rw-   0 root         (0) root         (0)     6090 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/checks/check_data_models_config.py
+-rw-rw-rw-   0 root         (0) root         (0)     4013 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/checks/check_documentation_for_sensitive_functionality.py
+-rw-rw-rw-   0 root         (0) root         (0)     7509 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/checks/check_documentation_standards.py
+-rw-rw-rw-   0 root         (0) root         (0)     5130 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/checks/check_for_indexer_synced_locals.py
+-rw-rw-rw-   0 root         (0) root         (0)     7410 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/checks/check_frontend_libraries.py
+-rw-rw-rw-   0 root         (0) root         (0)     1505 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/checks/check_git_conflict_file.py
+-rw-rw-rw-   0 root         (0) root         (0)    11555 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/checks/check_indexes_configuration_file.py
+-rw-rw-rw-   0 root         (0) root         (0)     1793 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/checks/check_itsi_module.py
+-rw-rw-rw-   0 root         (0) root         (0)    11941 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/checks/check_javascript_files.py
+-rw-rw-rw-   0 root         (0) root         (0)     6013 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/checks/check_jquery_standards.py
+-rw-rw-rw-   0 root         (0) root         (0)     1351 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/checks/check_json_files.py
+-rw-rw-rw-   0 root         (0) root         (0)     2046 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/checks/check_limits_configuration_file.py
+-rw-rw-rw-   0 root         (0) root         (0)     5294 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/checks/check_lookup_files.py
+-rw-rw-rw-   0 root         (0) root         (0)     4717 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/checks/check_malware.py
+-rw-rw-rw-   0 root         (0) root         (0)     4995 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/checks/check_meta_files.py
+-rw-rw-rw-   0 root         (0) root         (0)    15802 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/checks/check_modular_inputs.py
+-rw-rw-rw-   0 root         (0) root         (0)     2838 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/checks/check_outputs_configuration_file.py
+-rw-rw-rw-   0 root         (0) root         (0)    26539 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/checks/check_packaging_standards.py
+-rw-rw-rw-   0 root         (0) root         (0)     5423 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/checks/check_potentially_harmful_operations.py
+-rw-rw-rw-   0 root         (0) root         (0)    25269 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/checks/check_props_configuration_file.py
+-rw-rw-rw-   0 root         (0) root         (0)    42923 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/checks/check_python_files.py
+-rw-rw-rw-   0 root         (0) root         (0)     1922 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/checks/check_readme_spec_files.py
+-rw-rw-rw-   0 root         (0) root         (0)     7519 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/checks/check_rest_endpoints.py
+-rw-rw-rw-   0 root         (0) root         (0)    21103 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/checks/check_saved_searches.py
+-rwxrwxrwx   0 root         (0) root         (0)    32660 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/checks/check_security.py
+-rw-rw-rw-   0 root         (0) root         (0)     3894 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/checks/check_server_configuration_file.py
+-rwxrwxrwx   0 root         (0) root         (0)     8583 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/checks/check_source_and_binaries.py
+-rw-rw-rw-   0 root         (0) root         (0)     4241 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/checks/check_splunk_5_0_deprecated_features.py
+-rw-rw-rw-   0 root         (0) root         (0)     2983 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/checks/check_splunk_6_0_deprecated_features.py
+-rw-rw-rw-   0 root         (0) root         (0)     1521 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/checks/check_splunk_6_1_deprecated_features.py
+-rw-rw-rw-   0 root         (0) root         (0)     7075 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/checks/check_splunk_6_2_deprecated_features.py
+-rw-rw-rw-   0 root         (0) root         (0)    10039 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/checks/check_splunk_6_3_deprecated_features.py
+-rw-rw-rw-   0 root         (0) root         (0)    12198 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/checks/check_splunk_6_4_deprecated_features.py
+-rw-rw-rw-   0 root         (0) root         (0)     3502 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/checks/check_splunk_6_5_deprecated_features.py
+-rw-rw-rw-   0 root         (0) root         (0)     5140 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/checks/check_splunk_6_6_deprecated_features.py
+-rw-rw-rw-   0 root         (0) root         (0)     2910 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/checks/check_splunk_7_1_deprecated_features.py
+-rw-rw-rw-   0 root         (0) root         (0)     1918 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/checks/check_splunk_7_2_deprecated_features.py
+-rw-rw-rw-   0 root         (0) root         (0)     3087 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/checks/check_splunk_7_3_deprecated_features.py
+-rw-rw-rw-   0 root         (0) root         (0)    12727 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/checks/check_splunk_8_0_deprecated_features.py
+-rw-rw-rw-   0 root         (0) root         (0)     1944 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/checks/check_splunk_9_0_deprecated_features.py
+-rw-rw-rw-   0 root         (0) root         (0)     1147 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/checks/check_support_requirements.py
+-rw-rw-rw-   0 root         (0) root         (0)     4861 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/checks/check_transforms_configuration_file.py
+-rw-rw-rw-   0 root         (0) root         (0)     9134 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/checks/check_web_configuration_file.py
+-rw-rw-rw-   0 root         (0) root         (0)     4190 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/checks/check_workflow_actions.py
+-rw-rw-rw-   0 root         (0) root         (0)     5073 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/checks/check_xml_files.py
+-rw-rw-rw-   0 root         (0) root         (0)    28306 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/checks/class_based_checks_guide.md
+-rw-rw-rw-   0 root         (0) root         (0)     1248 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/checks/disabled_check_splunk_future_deprecated_features.py
+-rw-rw-rw-   0 root         (0) root         (0)    82204 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/checks.py
+-rw-rw-rw-   0 root         (0) root         (0)      427 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/collections_configuration_file.py
+-rw-rw-rw-   0 root         (0) root         (0)     5689 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/command_line_helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.583249 splunk-appinspect-3.7.0/splunk_appinspect/common/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-08 08:47:12.000000 splunk-appinspect-3.7.0/splunk_appinspect/common/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      374 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/common/file_hash.py
+-rw-rw-rw-   0 root         (0) root         (0)     8663 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/common/string_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    17928 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/configuration_file.py
+-rw-rw-rw-   0 root         (0) root         (0)     5963 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/configuration_parser.py
+-rw-rw-rw-   0 root         (0) root         (0)     1763 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     2990 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/cron_expression.py
+-rw-rw-rw-   0 root         (0) root         (0)    12526 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/custom_commands.py
+-rw-rw-rw-   0 root         (0) root         (0)     1636 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/custom_types.py
+-rw-rw-rw-   0 root         (0) root         (0)     5288 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/custom_visualizations.py
+-rw-rw-rw-   0 root         (0) root         (0)     1052 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/decorators.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.583249 splunk-appinspect-3.7.0/splunk_appinspect/documentation/
+-rw-rw-rw-   0 root         (0) root         (0)      196 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/documentation/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3785 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/documentation/cli_docs.py
+-rw-rw-rw-   0 root         (0) root         (0)     2991 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/documentation/criteria_generator.py
+-rw-rw-rw-   0 root         (0) root         (0)      635 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/documentation/splunk_docs.py
+-rw-rw-rw-   0 root         (0) root         (0)     2894 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/documentation/tag_reference_generator.py
+-rw-rw-rw-   0 root         (0) root         (0)      447 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/environment_validator.py
+-rw-rw-rw-   0 root         (0) root         (0)     3869 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/feedback_file_generator.py
+-rw-rw-rw-   0 root         (0) root         (0)     1447 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/file_resource.py
+-rw-rw-rw-   0 root         (0) root         (0)    10797 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/file_view.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.583249 splunk-appinspect-3.7.0/splunk_appinspect/formatters/
+-rw-rw-rw-   0 root         (0) root         (0)      357 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/formatters/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      429 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/formatters/date_time_encoder.py
+-rw-rw-rw-   0 root         (0) root         (0)      543 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/formatters/validation_report_formatter.py
+-rw-rw-rw-   0 root         (0) root         (0)     6288 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/formatters/validation_report_json_formatter.py
+-rw-rw-rw-   0 root         (0) root         (0)     8384 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/formatters/validation_report_junitxml_formatter.py
+-rw-rw-rw-   0 root         (0) root         (0)      830 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/image_resource.py
+-rw-rw-rw-   0 root         (0) root         (0)      421 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/indexes_configuration_file.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.583249 splunk-appinspect-3.7.0/splunk_appinspect/infra/
+-rw-rw-rw-   0 root         (0) root         (0)     1006 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/infra/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      981 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/infra/log_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      380 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/inputs_configuration_file.py
+-rw-rw-rw-   0 root         (0) root         (0)      375 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/inputs_specification_file.py
+-rw-rw-rw-   0 root         (0) root         (0)     8403 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/inspected_file.py
+-rw-rw-rw-   0 root         (0) root         (0)      586 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/iter_ext.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.583249 splunk-appinspect-3.7.0/splunk_appinspect/listeners/
+-rw-rw-rw-   0 root         (0) root         (0)      226 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/listeners/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3991 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/listeners/cert_status_listener.py
+-rw-rw-rw-   0 root         (0) root         (0)     3778 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/listeners/dot_status_listener.py
+-rw-rw-rw-   0 root         (0) root         (0)      507 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/listeners/listener.py
+-rw-rw-rw-   0 root         (0) root         (0)     5841 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/lookup.py
+-rwxrwxrwx   0 root         (0) root         (0)    26203 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/main.py
+-rw-rw-rw-   0 root         (0) root         (0)    15254 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/modular_inputs.py
+-rw-rw-rw-   0 root         (0) root         (0)     1597 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/mutually_exclusive_option.py
+-rw-rw-rw-   0 root         (0) root         (0)     1956 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/offense.py
+-rw-rw-rw-   0 root         (0) root         (0)      370 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/outputs_configuration_file.py
+-rw-rw-rw-   0 root         (0) root         (0)      393 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/props_configuration_file.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.587249 splunk-appinspect-3.7.0/splunk_appinspect/python_analyzer/
+-rw-rw-rw-   0 root         (0) root         (0)      176 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_analyzer/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)   109167 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_analyzer/ast_analyzer.py
+-rw-rw-rw-   0 root         (0) root         (0)    12307 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_analyzer/ast_info_query.py
+-rw-rw-rw-   0 root         (0) root         (0)     2827 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_analyzer/ast_info_store.py
+-rw-rw-rw-   0 root         (0) root         (0)    27144 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_analyzer/ast_types.py
+-rw-rw-rw-   0 root         (0) root         (0)    12126 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_analyzer/client.py
+-rw-rw-rw-   0 root         (0) root         (0)    18666 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_analyzer/file_dep_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.587249 splunk-appinspect-3.7.0/splunk_appinspect/python_analyzer/trustedlibs/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-08 08:47:12.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_analyzer/trustedlibs/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.603249 splunk-appinspect-3.7.0/splunk_appinspect/python_analyzer/trustedlibs/lib_files/
+-rw-r--r--   0 root         (0) root         (0)     1404 2024-05-08 08:47:46.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_analyzer/trustedlibs/lib_files/checks_used_for_libs.csv
+-rw-r--r--   0 root         (0) root         (0) 17023502 2024-05-08 08:47:46.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_analyzer/trustedlibs/lib_files/trusted_file_hashes.csv
+-rw-r--r--   0 root         (0) root         (0)  1252134 2024-05-08 08:47:46.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_analyzer/trustedlibs/lib_files/trusted_libs_record.csv
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-08 08:47:46.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_analyzer/trustedlibs/lib_files/untrusted_file_hashes.csv
+-rw-r--r--   0 root         (0) root         (0)       23 2024-05-08 08:47:46.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_analyzer/trustedlibs/lib_files/untrusted_libs_record.csv
+-rw-rw-rw-   0 root         (0) root         (0)     2313 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_analyzer/trustedlibs/trusted_data_collector.py
+-rw-rw-rw-   0 root         (0) root         (0)     1244 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_analyzer/trustedlibs/trusted_libs_manager.py
+-rw-rw-rw-   0 root         (0) root         (0)      279 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_analyzer/trustedlibs/utilities.py
+-rw-rw-rw-   0 root         (0) root         (0)    14673 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_analyzer/utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.603249 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-08 08:47:12.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.603249 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.603249 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/BaseHTTPServer/
+-rw-rw-rw-   0 root         (0) root         (0)      486 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/BaseHTTPServer/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.603249 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/ConfigParser/
+-rw-rw-rw-   0 root         (0) root         (0)      960 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/ConfigParser/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.603249 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/DocXMLRPCServer/
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/DocXMLRPCServer/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.603249 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/MimeWriter/
+-rw-rw-rw-   0 root         (0) root         (0)      633 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/MimeWriter/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.603249 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/SimpleXMLRPCServer/
+-rw-rw-rw-   0 root         (0) root         (0)      539 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/SimpleXMLRPCServer/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.603249 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/SocketServer/
+-rw-rw-rw-   0 root         (0) root         (0)      658 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/SocketServer/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.607249 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/___configparser/
+-rw-rw-rw-   0 root         (0) root         (0)      960 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/___configparser/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.607249 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/___socketserver/
+-rw-rw-rw-   0 root         (0) root         (0)      698 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/___socketserver/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      247 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.607249 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/_thread/
+-rw-rw-rw-   0 root         (0) root         (0)      387 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/_thread/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.607249 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/aifc/
+-rw-rw-rw-   0 root         (0) root         (0)      474 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/aifc/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.607249 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/anydbm/
+-rw-rw-rw-   0 root         (0) root         (0)      425 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/anydbm/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.607249 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/argparse/
+-rw-rw-rw-   0 root         (0) root         (0)      507 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/argparse/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.607249 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/asynchat/
+-rw-rw-rw-   0 root         (0) root         (0)      560 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/asynchat/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.607249 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/asyncore/
+-rw-rw-rw-   0 root         (0) root         (0)     1126 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/asyncore/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.607249 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/base64/
+-rw-rw-rw-   0 root         (0) root         (0)      739 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/base64/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.607249 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/binhex/
+-rw-rw-rw-   0 root         (0) root         (0)      619 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/binhex/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.607249 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/bz2/
+-rw-rw-rw-   0 root         (0) root         (0)      375 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/bz2/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.607249 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/cPickle/
+-rw-rw-rw-   0 root         (0) root         (0)      767 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/cPickle/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.607249 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/chunk/
+-rw-rw-rw-   0 root         (0) root         (0)      496 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/chunk/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.607249 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/cmd/
+-rw-rw-rw-   0 root         (0) root         (0)      425 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/cmd/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.607249 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/code/
+-rw-rw-rw-   0 root         (0) root         (0)      954 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/code/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.607249 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/commands/
+-rw-rw-rw-   0 root         (0) root         (0)      783 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/commands/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.607249 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/crypt/
+-rw-rw-rw-   0 root         (0) root         (0)      410 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/crypt/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.607249 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/csv/
+-rw-rw-rw-   0 root         (0) root         (0)      684 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/csv/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.607249 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/dbm/
+-rw-rw-rw-   0 root         (0) root         (0)      431 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/dbm/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.607249 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/dbm/dumb/
+-rw-rw-rw-   0 root         (0) root         (0)      440 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/dbm/dumb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.607249 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/dbm/gnu/
+-rw-rw-rw-   0 root         (0) root         (0)      394 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/dbm/gnu/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.607249 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/dbm/ndbm/
+-rw-rw-rw-   0 root         (0) root         (0)      400 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/dbm/ndbm/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.607249 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/dircache/
+-rw-rw-rw-   0 root         (0) root         (0)       43 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/dircache/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.607249 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/dl/
+-rw-rw-rw-   0 root         (0) root         (0)      539 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/dl/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.607249 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/dumbdbm/
+-rw-rw-rw-   0 root         (0) root         (0)      433 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/dumbdbm/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.607249 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/email/
+-rw-rw-rw-   0 root         (0) root         (0)      545 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/email/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.607249 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/ftplib/
+-rw-rw-rw-   0 root         (0) root         (0)      544 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/ftplib/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.607249 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/gc/
+-rw-rw-rw-   0 root         (0) root         (0)      446 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/gc/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.607249 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/gdbm/
+-rw-rw-rw-   0 root         (0) root         (0)      435 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/gdbm/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.611249 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/getpass/
+-rw-rw-rw-   0 root         (0) root         (0)      366 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/getpass/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.611249 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/gzip/
+-rw-rw-rw-   0 root         (0) root         (0)      571 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/gzip/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.611249 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/http/
+-rw-rw-rw-   0 root         (0) root         (0)      114 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/http/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.611249 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/http/client/
+-rw-rw-rw-   0 root         (0) root         (0)      467 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/http/client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.611249 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/http/server/
+-rw-rw-rw-   0 root         (0) root         (0)      688 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/http/server/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.611249 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/httplib/
+-rw-rw-rw-   0 root         (0) root         (0)      332 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/httplib/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.611249 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/httplib2/
+-rw-rw-rw-   0 root         (0) root         (0)      356 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/httplib2/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.611249 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/imaplib/
+-rw-rw-rw-   0 root         (0) root         (0)      767 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/imaplib/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.611249 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/imp/
+-rw-rw-rw-   0 root         (0) root         (0)      524 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/imp/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.611249 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/importlib/
+-rw-rw-rw-   0 root         (0) root         (0)      555 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/importlib/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.611249 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/imputil/
+-rw-rw-rw-   0 root         (0) root         (0)      918 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/imputil/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.611249 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/inspect/
+-rw-rw-rw-   0 root         (0) root         (0)      915 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/inspect/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.611249 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/io/
+-rw-rw-rw-   0 root         (0) root         (0)     3620 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/io/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.611249 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/json/
+-rw-rw-rw-   0 root         (0) root         (0)      568 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/json/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.611249 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/linecache/
+-rw-rw-rw-   0 root         (0) root         (0)      835 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/linecache/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.611249 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/logging/
+-rw-rw-rw-   0 root         (0) root         (0)      590 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/logging/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.611249 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/logging/config/
+-rw-rw-rw-   0 root         (0) root         (0)      594 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/logging/config/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.611249 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/logging/handlers/
+-rw-rw-rw-   0 root         (0) root         (0)     2068 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/logging/handlers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.611249 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/marshal/
+-rw-rw-rw-   0 root         (0) root         (0)      524 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/marshal/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.611249 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/mimetools/
+-rw-rw-rw-   0 root         (0) root         (0)      845 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/mimetools/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.611249 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/mimetypes/
+-rw-rw-rw-   0 root         (0) root         (0)     1040 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/mimetypes/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.611249 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/mimify/
+-rw-rw-rw-   0 root         (0) root         (0)      684 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/mimify/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.611249 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/mmap/
+-rw-rw-rw-   0 root         (0) root         (0)      445 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/mmap/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.611249 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/modulefinder/
+-rw-rw-rw-   0 root         (0) root         (0)      814 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/modulefinder/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.611249 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/multifile/
+-rw-rw-rw-   0 root         (0) root         (0)     1181 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/multifile/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.611249 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/multiprocessing/
+-rw-rw-rw-   0 root         (0) root         (0)      605 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/multiprocessing/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.611249 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/nntplib/
+-rw-rw-rw-   0 root         (0) root         (0)      388 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/nntplib/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.611249 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/os/
+-rw-rw-rw-   0 root         (0) root         (0)     4886 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/os/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.611249 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/os/path/
+-rw-rw-rw-   0 root         (0) root         (0)      931 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/os/path/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.611249 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/pickle/
+-rw-rw-rw-   0 root         (0) root         (0)      693 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/pickle/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.615249 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/pipes/
+-rw-rw-rw-   0 root         (0) root         (0)      548 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/pipes/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.615249 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/pkgutil/
+-rw-rw-rw-   0 root         (0) root         (0)      807 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/pkgutil/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.615249 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/plistlib/
+-rw-rw-rw-   0 root         (0) root         (0)      733 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/plistlib/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.615249 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/poplib/
+-rw-rw-rw-   0 root         (0) root         (0)      361 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/poplib/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.615249 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/posix/
+-rw-rw-rw-   0 root         (0) root         (0)     2273 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/posix/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.615249 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/posixfile/
+-rw-rw-rw-   0 root         (0) root         (0)      535 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/posixfile/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.615249 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/pty/
+-rw-rw-rw-   0 root         (0) root         (0)      668 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/pty/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.615249 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/quopri/
+-rw-rw-rw-   0 root         (0) root         (0)      769 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/quopri/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.615249 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/requests/
+-rw-rw-rw-   0 root         (0) root         (0)     1991 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/requests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.615249 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/runpy/
+-rw-rw-rw-   0 root         (0) root         (0)      725 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/runpy/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.615249 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/shelve/
+-rw-rw-rw-   0 root         (0) root         (0)      354 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/shelve/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.615249 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/shutil/
+-rw-rw-rw-   0 root         (0) root         (0)     1542 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/shutil/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.615249 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/smtplib/
+-rw-rw-rw-   0 root         (0) root         (0)      851 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/smtplib/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.615249 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/socket/
+-rw-rw-rw-   0 root         (0) root         (0)      743 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/socket/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.615249 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/sqlite3/
+-rw-rw-rw-   0 root         (0) root         (0)      541 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/sqlite3/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.615249 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/subprocess/
+-rw-rw-rw-   0 root         (0) root         (0)     1719 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/subprocess/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.615249 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/sunau/
+-rw-rw-rw-   0 root         (0) root         (0)      679 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/sunau/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.615249 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/syslog/
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/syslog/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.615249 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/tarfile/
+-rw-rw-rw-   0 root         (0) root         (0)      616 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/tarfile/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.615249 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/telnetlib/
+-rw-rw-rw-   0 root         (0) root         (0)      597 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/telnetlib/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.615249 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/tempfile/
+-rw-rw-rw-   0 root         (0) root         (0)     1059 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/tempfile/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.615249 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/termios/
+-rw-rw-rw-   0 root         (0) root         (0)      459 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/termios/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.615249 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/thread/
+-rw-rw-rw-   0 root         (0) root         (0)      326 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/thread/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.615249 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/threading/
+-rw-rw-rw-   0 root         (0) root         (0)      543 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/threading/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.615249 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/trace/
+-rw-rw-rw-   0 root         (0) root         (0)     1135 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/trace/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.615249 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/tty/
+-rw-rw-rw-   0 root         (0) root         (0)      575 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/tty/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.615249 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/urllib/
+-rw-rw-rw-   0 root         (0) root         (0)     1698 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/urllib/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.615249 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/urllib/request/
+-rw-rw-rw-   0 root         (0) root         (0)     1467 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/urllib/request/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.615249 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/urllib2/
+-rw-rw-rw-   0 root         (0) root         (0)      427 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/urllib2/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.619249 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/uu/
+-rw-rw-rw-   0 root         (0) root         (0)      730 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/uu/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.619249 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/wave/
+-rw-rw-rw-   0 root         (0) root         (0)      685 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/wave/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.619249 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/wsgiref/
+-rw-rw-rw-   0 root         (0) root         (0)      182 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/wsgiref/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.619249 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/wsgiref/simple_server/
+-rw-rw-rw-   0 root         (0) root         (0)      613 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/wsgiref/simple_server/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.619249 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/xml/
+-rw-rw-rw-   0 root         (0) root         (0)       73 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/xml/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.619249 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/xml/dom/
+-rw-rw-rw-   0 root         (0) root         (0)       78 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/xml/dom/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      582 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/xml/dom/minidom.py
+-rw-rw-rw-   0 root         (0) root         (0)      397 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/xml/dom/pulldom.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.619249 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/xml/etree/
+-rw-rw-rw-   0 root         (0) root         (0)     1077 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/xml/etree/ElementTree.py
+-rw-rw-rw-   0 root         (0) root         (0)       74 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/xml/etree/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.619249 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/xml/sax/
+-rw-rw-rw-   0 root         (0) root         (0)      368 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/xml/sax/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      459 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/xml/sax/xmlreader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.619249 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/xmlrpc/
+-rw-rw-rw-   0 root         (0) root         (0)      126 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/xmlrpc/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.619249 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/xmlrpc/client/
+-rw-rw-rw-   0 root         (0) root         (0)      434 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/xmlrpc/client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.619249 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/xmlrpc/server/
+-rw-rw-rw-   0 root         (0) root         (0)      651 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/xmlrpc/server/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.619249 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/xmlrpclib/
+-rw-rw-rw-   0 root         (0) root         (0)      406 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/xmlrpclib/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.619249 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/zipfile/
+-rw-rw-rw-   0 root         (0) root         (0)      453 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/zipfile/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.619249 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/zipimport/
+-rw-rw-rw-   0 root         (0) root         (0)      635 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/zipimport/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.619249 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata_common/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-08 08:47:12.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata_common/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3841 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata_common/metadata_consts.py
+-rw-rw-rw-   0 root         (0) root         (0)      416 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata_common/metadata_decorator.py
+-rw-rw-rw-   0 root         (0) root         (0)       96 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata_common/metadata_exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     6831 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata_common/metadata_types.py
+-rw-rw-rw-   0 root         (0) root         (0)      843 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata_importer.py
+-rw-rw-rw-   0 root         (0) root         (0)    16123 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/python_modules_metadata_store.py
+-rw-rw-rw-   0 root         (0) root         (0)    23619 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/reflected_xss_detector.py
+-rw-rw-rw-   0 root         (0) root         (0)    15016 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/regex_matcher.py
+-rw-rw-rw-   0 root         (0) root         (0)    12564 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/reporter.py
+-rw-rw-rw-   0 root         (0) root         (0)     2238 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/resource_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.619249 splunk-appinspect-3.7.0/splunk_appinspect/resources/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-08 08:47:12.000000 splunk-appinspect-3.7.0/splunk_appinspect/resources/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1536 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/resources/semgrep_recognized_extensions.json
+-rw-rw-rw-   0 root         (0) root         (0)     9582 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/rest_map.py
+-rw-rw-rw-   0 root         (0) root         (0)      401 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/rest_map_configuration_file.py
+-rw-rw-rw-   0 root         (0) root         (0)     4784 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/saved_searches.py
+-rw-rw-rw-   0 root         (0) root         (0)      442 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/saved_searches_configuration_file.py
+-rw-rw-rw-   0 root         (0) root         (0)     1367 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/sideview_utils_modules.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.619249 splunk-appinspect-3.7.0/splunk_appinspect/splunk/
+-rw-rw-rw-   0 root         (0) root         (0)      127 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/splunk/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.623249 splunk-appinspect-3.7.0/splunk_appinspect/splunk/jquery_checks_data/
+-rw-rw-rw-   0 root         (0) root         (0)   194102 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/splunk/jquery_checks_data/disallowed_imports.json
+-rw-rw-rw-   0 root         (0) root         (0)     2080 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/splunk/jquery_checks_data/risky_imports.json
+-rw-rw-rw-   0 root         (0) root         (0)     7992 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/splunk/splunk_default_source_type_list.py
+-rw-rw-rw-   0 root         (0) root         (0)     1802 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/splunk/splunk_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.623249 splunk-appinspect-3.7.0/splunk_appinspect/splunk/telemetry/
+-rw-rw-rw-   0 root         (0) root         (0)       39 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/splunk/telemetry/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      526 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/splunk/telemetry/core.py
+-rw-rw-rw-   0 root         (0) root         (0)     1408 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/splunk/telemetry/list.csv
+-rw-rw-rw-   0 root         (0) root         (0)     1975 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/splunk/util.py
+-rw-rw-rw-   0 root         (0) root         (0)     7992 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/splunk_default_source_type_list.py
+-rw-rw-rw-   0 root         (0) root         (0)     5132 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/splunk_defined_authorize_capability_list.py
+-rw-rw-rw-   0 root         (0) root         (0)     3402 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/splunk_defined_conf_file_list.py
+-rw-rw-rw-   0 root         (0) root         (0)     3021 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/splunk_pretrained_sourcetypes_list.py
+-rw-rw-rw-   0 root         (0) root         (0)      767 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/telemetry_configuration_file.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.623249 splunk-appinspect-3.7.0/splunk_appinspect/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     2782 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/templates/html_criteria.html
+-rw-rw-rw-   0 root         (0) root         (0)     1727 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/templates/tag_reference.html
+-rw-rw-rw-   0 root         (0) root         (0)    10003 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/validation_report.py
+-rw-rw-rw-   0 root         (0) root         (0)    16793 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/validator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.623249 splunk-appinspect-3.7.0/splunk_appinspect/version/
+-rw-rw-rw-   0 root         (0) root         (0)        6 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/version/VERSION.txt
+-rw-rw-rw-   0 root         (0) root         (0)      106 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/version/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      596 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/version/version.py
+-rw-rw-rw-   0 root         (0) root         (0)      356 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/visualizations_configuration_file.py
+-rw-rw-rw-   0 root         (0) root         (0)      392 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/web_configuration_file.py
+-rw-rw-rw-   0 root         (0) root         (0)      454 2024-05-08 08:47:10.000000 splunk-appinspect-3.7.0/splunk_appinspect/workflow_actions_configuration_file.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.575249 splunk-appinspect-3.7.0/splunk_appinspect.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1332 2024-05-08 08:47:46.000000 splunk-appinspect-3.7.0/splunk_appinspect.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    17979 2024-05-08 08:47:46.000000 splunk-appinspect-3.7.0/splunk_appinspect.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-08 08:47:46.000000 splunk-appinspect-3.7.0/splunk_appinspect.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       70 2024-05-08 08:47:46.000000 splunk-appinspect-3.7.0/splunk_appinspect.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      478 2024-05-08 08:47:46.000000 splunk-appinspect-3.7.0/splunk_appinspect.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       30 2024-05-08 08:47:46.000000 splunk-appinspect-3.7.0/splunk_appinspect.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.563249 splunk-appinspect-3.7.0/tarsec/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:47:46.623249 splunk-appinspect-3.7.0/tarsec/tarsec/
+-rw-rw-rw-   0 root         (0) root         (0)      193 2024-05-08 08:47:15.000000 splunk-appinspect-3.7.0/tarsec/tarsec/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6069 2024-05-08 08:47:15.000000 splunk-appinspect-3.7.0/tarsec/tarsec/check_tar.py
```

### Comparing `splunk-appinspect-3.6.0/PKG-INFO` & `splunk-appinspect-3.7.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: splunk-appinspect
-Version: 3.6.0
+Version: 3.7.0
 Summary: Automatic validation checks for Splunk Apps
 Home-page: https://splunk.com
 Author: Splunk
 Author-email: appinspect@splunk.com
 License: Other/Proprietary License
 Download-URL: http://dev.splunk.com/goto/appinspectdownload
 Description: AppInspect is a tool for assessing a Splunk App's compliance with Splunk recommended development practices, by using static analysis. AppInspect is open for extension, allowing other teams to compose checks that meet their domain specific needs for semi- or fully-automated analysis and validation of Splunk Apps.
```

### Comparing `splunk-appinspect-3.6.0/README.md` & `splunk-appinspect-3.7.0/README.md`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/pyproject.toml` & `splunk-appinspect-3.7.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/setup.cfg` & `splunk-appinspect-3.7.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/setup.py` & `splunk-appinspect-3.7.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     "langdetect==1.*,>=1.0.7",
     "lxml==4.*,>=4.6.0",
     "mako==1.*,>=1.0.12",
     "markdown==3.*,>=3.1.1",
     "packaging==23.0",
     "packaging-legacy==23.0",
     "painter==0.*,>=0.3.1",
-    "pillow>=9.5.0,<=10.0.0",
+    "pillow>=9.5.0,<=10.3.0",
     "pyyaml==6.*,>=6.0.1",
     "regex==2022.1.18",  # Python re module does not support PCRE, so use another one
     "six==1.*,>=1.12.0",
     "semver>=2.13.0",
 ]
 
 platform_specific_install_requirements = []
```

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/__init__.py` & `splunk-appinspect-3.7.0/splunk_appinspect/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/alert_actions.py` & `splunk-appinspect-3.7.0/splunk_appinspect/alert_actions.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/app.py` & `splunk-appinspect-3.7.0/splunk_appinspect/app.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/app_configuration_file.py` & `splunk-appinspect-3.7.0/splunk_appinspect/app_configuration_file.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/app_package_handler.py` & `splunk-appinspect-3.7.0/splunk_appinspect/app_package_handler.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/app_util.py` & `splunk-appinspect-3.7.0/splunk_appinspect/app_util.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/bias.py` & `splunk-appinspect-3.7.0/splunk_appinspect/bias.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/canary_modules.py` & `splunk-appinspect-3.7.0/splunk_appinspect/canary_modules.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/check_messages.py` & `splunk-appinspect-3.7.0/splunk_appinspect/check_messages.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/check_routine/__init__.py` & `splunk-appinspect-3.7.0/splunk_appinspect/check_routine/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/check_routine/find_endpoint_usage.py` & `splunk-appinspect-3.7.0/splunk_appinspect/check_routine/find_endpoint_usage.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/check_routine/find_spl_command_usage.py` & `splunk-appinspect-3.7.0/splunk_appinspect/check_routine/find_spl_command_usage.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/check_routine/python_ast_searcher/ast_searcher.py` & `splunk-appinspect-3.7.0/splunk_appinspect/check_routine/python_ast_searcher/ast_searcher.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/check_routine/util.py` & `splunk-appinspect-3.7.0/splunk_appinspect/check_routine/util.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/checks/check_addon_builder_config.py` & `splunk-appinspect-3.7.0/splunk_appinspect/checks/check_addon_builder_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,20 +45,19 @@
                 tags=(
                     Tags.SPLUNK_APPINSPECT,
                     Tags.CLOUD,
                     Tags.PRIVATE_APP,
                     Tags.PRIVATE_CLASSIC,
                     Tags.PRIVATE_VICTORIA,
                     Tags.MIGRATION_VICTORIA,
-                    Tags.FUTURE,
                 ),
             )
         )
 
-    MINIMUM_BUILDER_VERSION = parse_version("4.1.3")
+    MINIMUM_BUILDER_VERSION = parse_version("4.1.4")
     MAXIMUM_BUILDER_VERSION = parse_version("4.2.0")
 
     def check_config(self, app: "App", config: "ConfigurationProxy") -> Generator[CheckMessage, Any, None]:
         if not config["addon_builder"].has_section("base"):
             yield FailMessage(
                 "No base section found in addon_builder.conf.",
                 file_name=config["addon_builder"].get_relative_path(),
```

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/checks/check_alert_actions_config.py` & `splunk-appinspect-3.7.0/splunk_appinspect/checks/check_alert_actions_config.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/checks/check_app_configuration_file.py` & `splunk-appinspect-3.7.0/splunk_appinspect/checks/check_app_configuration_file.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/checks/check_application_content.py` & `splunk-appinspect-3.7.0/splunk_appinspect/checks/check_application_content.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/checks/check_application_structure.py` & `splunk-appinspect-3.7.0/splunk_appinspect/checks/check_application_structure.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/checks/check_authentication_configuration_file.py` & `splunk-appinspect-3.7.0/splunk_appinspect/checks/check_authentication_configuration_file.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/checks/check_authorize_configuration_file.py` & `splunk-appinspect-3.7.0/splunk_appinspect/checks/check_authorize_configuration_file.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/checks/check_bias_language.py` & `splunk-appinspect-3.7.0/splunk_appinspect/checks/check_bias_language.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/checks/check_binary_files.py` & `splunk-appinspect-3.7.0/splunk_appinspect/checks/check_binary_files.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/checks/check_cloud_simple_app.py` & `splunk-appinspect-3.7.0/splunk_appinspect/checks/check_cloud_simple_app.py`

 * *Files 0% similar despite different names*

```diff
@@ -232,15 +232,15 @@
         """Check that the `metadata/` or `users/<username>/metadata/` directory only contains .meta files
         and does not contain any subdirectories
         """
         parts = path_in_app.parts
         is_user = len(parts) == 4 and parts[0] == "users"
         is_local = len(path_in_app.parts) == 2
         if not (is_user or is_local) or path_in_app.parts[-2] != "metadata":
-            yield WarningMessage(
+            yield FailMessage(
                 "A Subdirectory found under metadata directory",
                 file_name=path_in_app.parent,
                 remediation="Please remove this directory from the metadata directory.",
             )
         elif not str(path_in_app).endswith(".meta"):
             yield FailMessage(
                 "A file within the `metadata` directory was found"
@@ -385,38 +385,37 @@
                 tags=(
                     Tags.SPLUNK_APPINSPECT,
                     Tags.CLOUD,
                     Tags.PRIVATE_APP,
                     Tags.PRIVATE_VICTORIA,
                     Tags.MIGRATION_VICTORIA,
                     Tags.PRIVATE_CLASSIC,
-                    Tags.FUTURE,
                 ),
                 depends_on_config=("authorize",),
             )
         )
 
     def check_config(self, app: "App", config: "ConfigurationProxy") -> Generator[CheckMessage, Any, None]:
         for section in config["authorize"].sections_with_setting_key_pattern("role_*"):
             # find `importRoles` and `grantableRoles` settings
             prohibited_options = (opt for opt in section.options.values() if opt.name in self.TARGET_OPTIONS)
             if section.name in self.ADMIN_STANZAS:
                 for option in prohibited_options:
-                    yield WarningMessage(
+                    yield FailMessage(
                         message=f"Stanza [{section.name}] should not contain `{option.name}` settings.",
                         remediation=f"Remove `{option.name}` settings from [{section.name}] stanza.",
                         file_name=option.relative_path,
                         line_number=option.lineno,
                     )
             else:
                 for option in prohibited_options:
                     # find `admin` and `splunk-system-role` in the option value (semicolon-separated list)
                     roles = (role for role in option.value.split(";") if role.strip() in self.PROHIBITED_ROLES)
                     for role in roles:
-                        yield WarningMessage(
+                        yield FailMessage(
                             message=f"Stanza [{section.name}] should not contain `{role}` role in `{option.name}` settings.",
                             remediation=f"Remove `{role}` role from `{option.name}` settings in [{section.name}] stanza.",
                             file_name=option.relative_path,
                             line_number=option.lineno,
                         )
```

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/checks/check_configuration_files.py` & `splunk-appinspect-3.7.0/splunk_appinspect/checks/check_configuration_files.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/checks/check_custom_commands.py` & `splunk-appinspect-3.7.0/splunk_appinspect/checks/check_custom_commands.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/checks/check_custom_visualizations.py` & `splunk-appinspect-3.7.0/splunk_appinspect/checks/check_custom_visualizations.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/checks/check_data_models_config.py` & `splunk-appinspect-3.7.0/splunk_appinspect/checks/check_data_models_config.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/checks/check_documentation_for_sensitive_functionality.py` & `splunk-appinspect-3.7.0/splunk_appinspect/checks/check_documentation_for_sensitive_functionality.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/checks/check_documentation_standards.py` & `splunk-appinspect-3.7.0/splunk_appinspect/checks/check_documentation_standards.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/checks/check_for_indexer_synced_locals.py` & `splunk-appinspect-3.7.0/splunk_appinspect/checks/check_for_indexer_synced_locals.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/checks/check_frontend_libraries.py` & `splunk-appinspect-3.7.0/splunk_appinspect/checks/check_frontend_libraries.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/checks/check_git_conflict_file.py` & `splunk-appinspect-3.7.0/splunk_appinspect/checks/check_git_conflict_file.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/checks/check_indexes_configuration_file.py` & `splunk-appinspect-3.7.0/splunk_appinspect/checks/check_indexes_configuration_file.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/checks/check_itsi_module.py` & `splunk-appinspect-3.7.0/splunk_appinspect/checks/check_itsi_module.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/checks/check_javascript_files.py` & `splunk-appinspect-3.7.0/splunk_appinspect/checks/check_javascript_files.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/checks/check_jquery_standards.py` & `splunk-appinspect-3.7.0/splunk_appinspect/checks/check_jquery_standards.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/checks/check_json_files.py` & `splunk-appinspect-3.7.0/splunk_appinspect/checks/check_json_files.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/checks/check_limits_configuration_file.py` & `splunk-appinspect-3.7.0/splunk_appinspect/checks/check_limits_configuration_file.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/checks/check_lookup_files.py` & `splunk-appinspect-3.7.0/splunk_appinspect/checks/check_lookup_files.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/checks/check_malware.py` & `splunk-appinspect-3.7.0/splunk_appinspect/checks/check_malware.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/checks/check_meta_files.py` & `splunk-appinspect-3.7.0/splunk_appinspect/checks/check_meta_files.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/checks/check_modular_inputs.py` & `splunk-appinspect-3.7.0/splunk_appinspect/checks/check_modular_inputs.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/checks/check_outputs_configuration_file.py` & `splunk-appinspect-3.7.0/splunk_appinspect/checks/check_outputs_configuration_file.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/checks/check_packaging_standards.py` & `splunk-appinspect-3.7.0/splunk_appinspect/checks/check_packaging_standards.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/checks/check_potentially_harmful_operations.py` & `splunk-appinspect-3.7.0/splunk_appinspect/checks/check_potentially_harmful_operations.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/checks/check_props_configuration_file.py` & `splunk-appinspect-3.7.0/splunk_appinspect/checks/check_props_configuration_file.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/checks/check_python_files.py` & `splunk-appinspect-3.7.0/splunk_appinspect/checks/check_python_files.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/checks/check_readme_spec_files.py` & `splunk-appinspect-3.7.0/splunk_appinspect/checks/check_readme_spec_files.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/checks/check_rest_endpoints.py` & `splunk-appinspect-3.7.0/splunk_appinspect/checks/check_rest_endpoints.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/checks/check_saved_searches.py` & `splunk-appinspect-3.7.0/splunk_appinspect/checks/check_saved_searches.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/checks/check_security.py` & `splunk-appinspect-3.7.0/splunk_appinspect/checks/check_security.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/checks/check_server_configuration_file.py` & `splunk-appinspect-3.7.0/splunk_appinspect/checks/check_server_configuration_file.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/checks/check_source_and_binaries.py` & `splunk-appinspect-3.7.0/splunk_appinspect/checks/check_source_and_binaries.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/checks/check_splunk_5_0_deprecated_features.py` & `splunk-appinspect-3.7.0/splunk_appinspect/checks/check_splunk_5_0_deprecated_features.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/checks/check_splunk_6_0_deprecated_features.py` & `splunk-appinspect-3.7.0/splunk_appinspect/checks/check_splunk_6_0_deprecated_features.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/checks/check_splunk_6_1_deprecated_features.py` & `splunk-appinspect-3.7.0/splunk_appinspect/checks/check_splunk_6_1_deprecated_features.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/checks/check_splunk_6_2_deprecated_features.py` & `splunk-appinspect-3.7.0/splunk_appinspect/checks/check_splunk_6_2_deprecated_features.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/checks/check_splunk_6_3_deprecated_features.py` & `splunk-appinspect-3.7.0/splunk_appinspect/checks/check_splunk_6_3_deprecated_features.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/checks/check_splunk_6_4_deprecated_features.py` & `splunk-appinspect-3.7.0/splunk_appinspect/checks/check_splunk_6_4_deprecated_features.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/checks/check_splunk_6_5_deprecated_features.py` & `splunk-appinspect-3.7.0/splunk_appinspect/checks/check_splunk_6_5_deprecated_features.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/checks/check_splunk_6_6_deprecated_features.py` & `splunk-appinspect-3.7.0/splunk_appinspect/checks/check_splunk_6_6_deprecated_features.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/checks/check_splunk_7_1_deprecated_features.py` & `splunk-appinspect-3.7.0/splunk_appinspect/checks/check_splunk_7_1_deprecated_features.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/checks/check_splunk_7_2_deprecated_features.py` & `splunk-appinspect-3.7.0/splunk_appinspect/checks/check_splunk_7_2_deprecated_features.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/checks/check_splunk_7_3_deprecated_features.py` & `splunk-appinspect-3.7.0/splunk_appinspect/checks/check_splunk_7_3_deprecated_features.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/checks/check_splunk_8_0_deprecated_features.py` & `splunk-appinspect-3.7.0/splunk_appinspect/checks/check_splunk_8_0_deprecated_features.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/checks/check_splunk_9_0_deprecated_features.py` & `splunk-appinspect-3.7.0/splunk_appinspect/checks/check_splunk_9_0_deprecated_features.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/checks/check_support_requirements.py` & `splunk-appinspect-3.7.0/splunk_appinspect/checks/check_support_requirements.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/checks/check_transforms_configuration_file.py` & `splunk-appinspect-3.7.0/splunk_appinspect/checks/check_transforms_configuration_file.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/checks/check_web_configuration_file.py` & `splunk-appinspect-3.7.0/splunk_appinspect/checks/check_web_configuration_file.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/checks/check_workflow_actions.py` & `splunk-appinspect-3.7.0/splunk_appinspect/checks/check_workflow_actions.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/checks/check_xml_files.py` & `splunk-appinspect-3.7.0/splunk_appinspect/checks/check_xml_files.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/checks/class_based_checks_guide.md` & `splunk-appinspect-3.7.0/splunk_appinspect/checks/class_based_checks_guide.md`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/checks/disabled_check_splunk_future_deprecated_features.py` & `splunk-appinspect-3.7.0/splunk_appinspect/checks/disabled_check_splunk_future_deprecated_features.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/checks.py` & `splunk-appinspect-3.7.0/splunk_appinspect/checks.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/command_line_helpers.py` & `splunk-appinspect-3.7.0/splunk_appinspect/command_line_helpers.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/common/string_utils.py` & `splunk-appinspect-3.7.0/splunk_appinspect/common/string_utils.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/configuration_file.py` & `splunk-appinspect-3.7.0/splunk_appinspect/configuration_file.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/configuration_parser.py` & `splunk-appinspect-3.7.0/splunk_appinspect/configuration_parser.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/constants.py` & `splunk-appinspect-3.7.0/splunk_appinspect/constants.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/cron_expression.py` & `splunk-appinspect-3.7.0/splunk_appinspect/cron_expression.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/custom_commands.py` & `splunk-appinspect-3.7.0/splunk_appinspect/custom_commands.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/custom_types.py` & `splunk-appinspect-3.7.0/splunk_appinspect/custom_types.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/custom_visualizations.py` & `splunk-appinspect-3.7.0/splunk_appinspect/custom_visualizations.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/decorators.py` & `splunk-appinspect-3.7.0/splunk_appinspect/decorators.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/documentation/cli_docs.py` & `splunk-appinspect-3.7.0/splunk_appinspect/documentation/cli_docs.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/documentation/criteria_generator.py` & `splunk-appinspect-3.7.0/splunk_appinspect/documentation/criteria_generator.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/documentation/splunk_docs.py` & `splunk-appinspect-3.7.0/splunk_appinspect/documentation/splunk_docs.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/documentation/tag_reference_generator.py` & `splunk-appinspect-3.7.0/splunk_appinspect/documentation/tag_reference_generator.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/feedback_file_generator.py` & `splunk-appinspect-3.7.0/splunk_appinspect/feedback_file_generator.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/file_resource.py` & `splunk-appinspect-3.7.0/splunk_appinspect/file_resource.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/file_view.py` & `splunk-appinspect-3.7.0/splunk_appinspect/file_view.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/formatters/validation_report_formatter.py` & `splunk-appinspect-3.7.0/splunk_appinspect/formatters/validation_report_formatter.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/formatters/validation_report_json_formatter.py` & `splunk-appinspect-3.7.0/splunk_appinspect/formatters/validation_report_json_formatter.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/formatters/validation_report_junitxml_formatter.py` & `splunk-appinspect-3.7.0/splunk_appinspect/formatters/validation_report_junitxml_formatter.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/image_resource.py` & `splunk-appinspect-3.7.0/splunk_appinspect/image_resource.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/infra/__init__.py` & `splunk-appinspect-3.7.0/splunk_appinspect/infra/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/infra/log_utils.py` & `splunk-appinspect-3.7.0/splunk_appinspect/infra/log_utils.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/inspected_file.py` & `splunk-appinspect-3.7.0/splunk_appinspect/inspected_file.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/iter_ext.py` & `splunk-appinspect-3.7.0/splunk_appinspect/iter_ext.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/listeners/cert_status_listener.py` & `splunk-appinspect-3.7.0/splunk_appinspect/listeners/cert_status_listener.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/listeners/dot_status_listener.py` & `splunk-appinspect-3.7.0/splunk_appinspect/listeners/dot_status_listener.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/lookup.py` & `splunk-appinspect-3.7.0/splunk_appinspect/lookup.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/main.py` & `splunk-appinspect-3.7.0/splunk_appinspect/main.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/modular_inputs.py` & `splunk-appinspect-3.7.0/splunk_appinspect/modular_inputs.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/mutually_exclusive_option.py` & `splunk-appinspect-3.7.0/splunk_appinspect/mutually_exclusive_option.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/offense.py` & `splunk-appinspect-3.7.0/splunk_appinspect/offense.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/python_analyzer/ast_analyzer.py` & `splunk-appinspect-3.7.0/splunk_appinspect/python_analyzer/ast_analyzer.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/python_analyzer/ast_info_query.py` & `splunk-appinspect-3.7.0/splunk_appinspect/python_analyzer/ast_info_query.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/python_analyzer/ast_info_store.py` & `splunk-appinspect-3.7.0/splunk_appinspect/python_analyzer/ast_info_store.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/python_analyzer/ast_types.py` & `splunk-appinspect-3.7.0/splunk_appinspect/python_analyzer/ast_types.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/python_analyzer/client.py` & `splunk-appinspect-3.7.0/splunk_appinspect/python_analyzer/client.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/python_analyzer/file_dep_manager.py` & `splunk-appinspect-3.7.0/splunk_appinspect/python_analyzer/file_dep_manager.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/python_analyzer/trustedlibs/lib_files/checks_used_for_libs.csv` & `splunk-appinspect-3.7.0/splunk_appinspect/python_analyzer/trustedlibs/lib_files/checks_used_for_libs.csv`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/python_analyzer/trustedlibs/lib_files/trusted_file_hashes.csv` & `splunk-appinspect-3.7.0/splunk_appinspect/python_analyzer/trustedlibs/lib_files/trusted_file_hashes.csv`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/python_analyzer/trustedlibs/lib_files/trusted_libs_record.csv` & `splunk-appinspect-3.7.0/splunk_appinspect/python_analyzer/trustedlibs/lib_files/trusted_libs_record.csv`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/python_analyzer/trustedlibs/trusted_data_collector.py` & `splunk-appinspect-3.7.0/splunk_appinspect/python_analyzer/trustedlibs/trusted_data_collector.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/python_analyzer/trustedlibs/trusted_libs_manager.py` & `splunk-appinspect-3.7.0/splunk_appinspect/python_analyzer/trustedlibs/trusted_libs_manager.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/python_analyzer/utilities.py` & `splunk-appinspect-3.7.0/splunk_appinspect/python_analyzer/utilities.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/ConfigParser/__init__.py` & `splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/ConfigParser/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/DocXMLRPCServer/__init__.py` & `splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/DocXMLRPCServer/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/MimeWriter/__init__.py` & `splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/MimeWriter/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/SimpleXMLRPCServer/__init__.py` & `splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/SimpleXMLRPCServer/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/SocketServer/__init__.py` & `splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/SocketServer/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/___configparser/__init__.py` & `splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/___configparser/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/___socketserver/__init__.py` & `splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/___socketserver/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/asynchat/__init__.py` & `splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/asynchat/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/asyncore/__init__.py` & `splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/asyncore/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/base64/__init__.py` & `splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/base64/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/binhex/__init__.py` & `splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/binhex/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/cPickle/__init__.py` & `splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/cPickle/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/code/__init__.py` & `splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/code/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/commands/__init__.py` & `splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/csv/__init__.py` & `splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/csv/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/dl/__init__.py` & `splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/dl/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/email/__init__.py` & `splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/email/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/ftplib/__init__.py` & `splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/ftplib/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/gzip/__init__.py` & `splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/gzip/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/http/server/__init__.py` & `splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/http/server/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/imaplib/__init__.py` & `splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/imaplib/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/imp/__init__.py` & `splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/imp/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/importlib/__init__.py` & `splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/importlib/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/imputil/__init__.py` & `splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/imputil/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/inspect/__init__.py` & `splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/inspect/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/io/__init__.py` & `splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/io/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/json/__init__.py` & `splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/json/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/linecache/__init__.py` & `splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/linecache/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/logging/__init__.py` & `splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/logging/config/__init__.py` & `splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/logging/config/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/logging/handlers/__init__.py` & `splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/logging/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/marshal/__init__.py` & `splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/marshal/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/mimetools/__init__.py` & `splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/mimetools/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/mimetypes/__init__.py` & `splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/mimetypes/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/mimify/__init__.py` & `splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/mimify/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/modulefinder/__init__.py` & `splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/modulefinder/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/multifile/__init__.py` & `splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/multifile/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/multiprocessing/__init__.py` & `splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/multiprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/os/__init__.py` & `splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/os/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/os/path/__init__.py` & `splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/os/path/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/pickle/__init__.py` & `splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/pickle/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/pipes/__init__.py` & `splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/pipes/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/pkgutil/__init__.py` & `splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/pkgutil/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/plistlib/__init__.py` & `splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/plistlib/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/posix/__init__.py` & `splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/posix/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/posixfile/__init__.py` & `splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/posixfile/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/pty/__init__.py` & `splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/pty/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/quopri/__init__.py` & `splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/quopri/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/requests/__init__.py` & `splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/runpy/__init__.py` & `splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/runpy/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/shutil/__init__.py` & `splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/shutil/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/smtplib/__init__.py` & `splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/smtplib/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/socket/__init__.py` & `splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/socket/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/sqlite3/__init__.py` & `splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/sqlite3/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/subprocess/__init__.py` & `splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/subprocess/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/sunau/__init__.py` & `splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/sunau/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/syslog/__init__.py` & `splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/syslog/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/tarfile/__init__.py` & `splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/tarfile/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/telnetlib/__init__.py` & `splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/telnetlib/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/tempfile/__init__.py` & `splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/tempfile/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/threading/__init__.py` & `splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/threading/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/trace/__init__.py` & `splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/trace/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/tty/__init__.py` & `splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/tty/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/urllib/__init__.py` & `splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/urllib/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/urllib/request/__init__.py` & `splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/urllib/request/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/uu/__init__.py` & `splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/uu/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/wave/__init__.py` & `splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/wave/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/wsgiref/simple_server/__init__.py` & `splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/wsgiref/simple_server/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/xml/dom/minidom.py` & `splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/xml/dom/minidom.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/xml/etree/ElementTree.py` & `splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/xml/etree/ElementTree.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/xmlrpc/server/__init__.py` & `splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/xmlrpc/server/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata/zipimport/__init__.py` & `splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata/zipimport/__init__.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata_common/metadata_consts.py` & `splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata_common/metadata_consts.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata_common/metadata_types.py` & `splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata_common/metadata_types.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/metadata_importer.py` & `splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/metadata_importer.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/python_modules_metadata/python_modules_metadata_store.py` & `splunk-appinspect-3.7.0/splunk_appinspect/python_modules_metadata/python_modules_metadata_store.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/reflected_xss_detector.py` & `splunk-appinspect-3.7.0/splunk_appinspect/reflected_xss_detector.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/regex_matcher.py` & `splunk-appinspect-3.7.0/splunk_appinspect/regex_matcher.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/reporter.py` & `splunk-appinspect-3.7.0/splunk_appinspect/reporter.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/resource_manager.py` & `splunk-appinspect-3.7.0/splunk_appinspect/resource_manager.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/resources/semgrep_recognized_extensions.json` & `splunk-appinspect-3.7.0/splunk_appinspect/resources/semgrep_recognized_extensions.json`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/rest_map.py` & `splunk-appinspect-3.7.0/splunk_appinspect/rest_map.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/saved_searches.py` & `splunk-appinspect-3.7.0/splunk_appinspect/saved_searches.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/sideview_utils_modules.py` & `splunk-appinspect-3.7.0/splunk_appinspect/sideview_utils_modules.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/splunk/jquery_checks_data/disallowed_imports.json` & `splunk-appinspect-3.7.0/splunk_appinspect/splunk/jquery_checks_data/disallowed_imports.json`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/splunk/jquery_checks_data/risky_imports.json` & `splunk-appinspect-3.7.0/splunk_appinspect/splunk/jquery_checks_data/risky_imports.json`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/splunk/splunk_default_source_type_list.py` & `splunk-appinspect-3.7.0/splunk_appinspect/splunk/splunk_default_source_type_list.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/splunk/splunk_version.py` & `splunk-appinspect-3.7.0/splunk_appinspect/splunk/splunk_version.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/splunk/telemetry/core.py` & `splunk-appinspect-3.7.0/splunk_appinspect/splunk/telemetry/core.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/splunk/telemetry/list.csv` & `splunk-appinspect-3.7.0/splunk_appinspect/splunk/telemetry/list.csv`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/splunk/util.py` & `splunk-appinspect-3.7.0/splunk_appinspect/splunk/util.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/splunk_default_source_type_list.py` & `splunk-appinspect-3.7.0/splunk_appinspect/splunk_default_source_type_list.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/splunk_defined_authorize_capability_list.py` & `splunk-appinspect-3.7.0/splunk_appinspect/splunk_defined_authorize_capability_list.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/splunk_defined_conf_file_list.py` & `splunk-appinspect-3.7.0/splunk_appinspect/splunk_defined_conf_file_list.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/splunk_pretrained_sourcetypes_list.py` & `splunk-appinspect-3.7.0/splunk_appinspect/splunk_pretrained_sourcetypes_list.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/telemetry_configuration_file.py` & `splunk-appinspect-3.7.0/splunk_appinspect/telemetry_configuration_file.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/templates/html_criteria.html` & `splunk-appinspect-3.7.0/splunk_appinspect/templates/html_criteria.html`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/templates/tag_reference.html` & `splunk-appinspect-3.7.0/splunk_appinspect/templates/tag_reference.html`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/validation_report.py` & `splunk-appinspect-3.7.0/splunk_appinspect/validation_report.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/validator.py` & `splunk-appinspect-3.7.0/splunk_appinspect/validator.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect/version/version.py` & `splunk-appinspect-3.7.0/splunk_appinspect/version/version.py`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect.egg-info/PKG-INFO` & `splunk-appinspect-3.7.0/splunk_appinspect.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: splunk-appinspect
-Version: 3.6.0
+Version: 3.7.0
 Summary: Automatic validation checks for Splunk Apps
 Home-page: https://splunk.com
 Author: Splunk
 Author-email: appinspect@splunk.com
 License: Other/Proprietary License
 Download-URL: http://dev.splunk.com/goto/appinspectdownload
 Description: AppInspect is a tool for assessing a Splunk App's compliance with Splunk recommended development practices, by using static analysis. AppInspect is open for extension, allowing other teams to compose checks that meet their domain specific needs for semi- or fully-automated analysis and validation of Splunk Apps.
```

### Comparing `splunk-appinspect-3.6.0/splunk_appinspect.egg-info/SOURCES.txt` & `splunk-appinspect-3.7.0/splunk_appinspect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `splunk-appinspect-3.6.0/tarsec/tarsec/check_tar.py` & `splunk-appinspect-3.7.0/tarsec/tarsec/check_tar.py`

 * *Files identical despite different names*

