# Comparing `tmp/databricks_labs_remorph-0.1.6.tar.gz` & `tmp/databricks_labs_remorph-0.1.7.tar.gz`

## Comparing `databricks_labs_remorph-0.1.6.tar` & `databricks_labs_remorph-0.1.7.tar`

### file list

```diff
@@ -1,49 +1,97 @@
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.6/databricks/__init__.py
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.6/databricks/labs/__init__.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.6/databricks/labs/remorph/__about__.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.6/databricks/labs/remorph/__init__.py
--rw-r--r--   0        0        0     3222 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.6/databricks/labs/remorph/cli.py
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.6/databricks/labs/remorph/config.py
--rw-r--r--   0        0        0     8586 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.6/databricks/labs/remorph/install.py
--rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.6/databricks/labs/remorph/uninstall.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.6/databricks/labs/remorph/coverage/__init__.py
--rw-r--r--   0        0        0     5749 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.6/databricks/labs/remorph/coverage/commons.py
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.6/databricks/labs/remorph/coverage/remorph_snow_transpilation_coverage.py
--rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.6/databricks/labs/remorph/coverage/sqlglot_snow_transpilation_coverage.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.6/databricks/labs/remorph/helpers/__init__.py
--rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.6/databricks/labs/remorph/helpers/db_sql.py
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.6/databricks/labs/remorph/helpers/execution_time.py
--rw-r--r--   0        0        0     3361 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.6/databricks/labs/remorph/helpers/file_utils.py
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.6/databricks/labs/remorph/helpers/morph_status.py
--rw-r--r--   0        0        0     4062 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.6/databricks/labs/remorph/helpers/validation.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.6/databricks/labs/remorph/intermediate/__init__.py
--rw-r--r--   0        0        0     3112 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.6/databricks/labs/remorph/intermediate/dag.py
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.6/databricks/labs/remorph/intermediate/engine_adapter.py
--rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.6/databricks/labs/remorph/intermediate/root_tables.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.6/databricks/labs/remorph/reconcile/__init__.py
--rw-r--r--   0        0        0     2343 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.6/databricks/labs/remorph/reconcile/constants.py
--rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.6/databricks/labs/remorph/reconcile/execute.py
--rw-r--r--   0        0        0     3011 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.6/databricks/labs/remorph/reconcile/recon_config.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.6/databricks/labs/remorph/reconcile/connectors/__init__.py
--rw-r--r--   0        0        0     2060 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.6/databricks/labs/remorph/reconcile/connectors/data_source.py
--rw-r--r--   0        0        0     2396 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.6/databricks/labs/remorph/reconcile/connectors/databricks.py
--rw-r--r--   0        0        0     3806 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.6/databricks/labs/remorph/reconcile/connectors/oracle.py
--rw-r--r--   0        0        0     3657 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.6/databricks/labs/remorph/reconcile/connectors/snowflake.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.6/databricks/labs/remorph/reconcile/query_builder/__init__.py
--rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.6/databricks/labs/remorph/reconcile/query_builder/base.py
--rw-r--r--   0        0        0     2449 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.6/databricks/labs/remorph/reconcile/query_builder/hash_query.py
--rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.6/databricks/labs/remorph/reconcile/query_builder/threshold_query.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.6/databricks/labs/remorph/snow/__init__.py
--rw-r--r--   0        0        0    25157 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.6/databricks/labs/remorph/snow/databricks.py
--rw-r--r--   0        0        0     3445 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.6/databricks/labs/remorph/snow/dialect_utils.py
--rw-r--r--   0        0        0     3231 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.6/databricks/labs/remorph/snow/local_expression.py
--rw-r--r--   0        0        0    22324 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.6/databricks/labs/remorph/snow/snowflake.py
--rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.6/databricks/labs/remorph/snow/sql_transpiler.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.6/databricks/labs/remorph/transpiler/__init__.py
--rw-r--r--   0        0        0     6816 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.6/databricks/labs/remorph/transpiler/execute.py
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.6/.gitignore
--rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.6/LICENSE
--rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.6/NOTICE
--rw-r--r--   0        0        0     6443 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.6/README.md
--rw-r--r--   0        0        0    26918 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     7366 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/core/src/main/antlr4/com/databricks/labs/remorph/parsers/snowflake/.gitignore
+-rw-r--r--   0        0        0    54055 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/core/src/main/antlr4/com/databricks/labs/remorph/parsers/snowflake/SnowflakeLexer.g4
+-rw-r--r--   0        0        0   112460 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/core/src/main/antlr4/com/databricks/labs/remorph/parsers/snowflake/SnowflakeParser.g4
+-rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/core/src/main/antlr4/com/databricks/labs/remorph/parsers/tsql/.gitignore
+-rw-r--r--   0        0        0    71070 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/core/src/main/antlr4/com/databricks/labs/remorph/parsers/tsql/TSqlLexer.g4
+-rw-r--r--   0        0        0   207140 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/core/src/main/antlr4/com/databricks/labs/remorph/parsers/tsql/TSqlParser.g4
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/core/src/main/scala/com/databricks/labs/remorph/Main.scala
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/core/src/main/scala/com/databricks/labs/remorph/parsers/IncompleteParser.scala
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/core/src/main/scala/com/databricks/labs/remorph/parsers/ParserCommon.scala
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/core/src/main/scala/com/databricks/labs/remorph/parsers/intermediate/Plan.scala
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/core/src/main/scala/com/databricks/labs/remorph/parsers/intermediate/TreeNode.scala
+-rw-r--r--   0        0        0     2253 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/core/src/main/scala/com/databricks/labs/remorph/parsers/intermediate/catalog.scala
+-rw-r--r--   0        0        0     2758 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/core/src/main/scala/com/databricks/labs/remorph/parsers/intermediate/commands.scala
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/core/src/main/scala/com/databricks/labs/remorph/parsers/intermediate/common.scala
+-rw-r--r--   0        0        0     4545 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/core/src/main/scala/com/databricks/labs/remorph/parsers/intermediate/expressions.scala
+-rw-r--r--   0        0        0     5893 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/core/src/main/scala/com/databricks/labs/remorph/parsers/intermediate/extensions.scala
+-rw-r--r--   0        0        0     8466 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/core/src/main/scala/com/databricks/labs/remorph/parsers/intermediate/relations.scala
+-rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/core/src/main/scala/com/databricks/labs/remorph/parsers/intermediate/types.scala
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/core/src/main/scala/com/databricks/labs/remorph/parsers/intermediate/unresolved.scala
+-rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/core/src/main/scala/com/databricks/labs/remorph/parsers/snowflake/DataTypeBuilder.scala
+-rw-r--r--   0        0        0     2024 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/core/src/main/scala/com/databricks/labs/remorph/parsers/snowflake/SnowflakeAstBuilder.scala
+-rw-r--r--   0        0        0     6830 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/core/src/main/scala/com/databricks/labs/remorph/parsers/snowflake/SnowflakeDDLBuilder.scala
+-rw-r--r--   0        0        0    10725 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/core/src/main/scala/com/databricks/labs/remorph/parsers/snowflake/SnowflakeExpressionBuilder.scala
+-rw-r--r--   0        0        0     8581 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/core/src/main/scala/com/databricks/labs/remorph/parsers/snowflake/SnowflakeRelationBuilder.scala
+-rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/core/src/main/scala/com/databricks/labs/remorph/parsers/snowflake/package.scala
+-rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/core/src/main/scala/com/databricks/labs/remorph/parsers/tsql/TSqlAstBuilder.scala
+-rw-r--r--   0        0        0     5777 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/core/src/main/scala/com/databricks/labs/remorph/parsers/tsql/TSqlExpressionBuilder.scala
+-rw-r--r--   0        0        0     2008 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/core/src/main/scala/com/databricks/labs/remorph/parsers/tsql/TSqlRelationBuilder.scala
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/core/src/test/scala/com/databricks/labs/remorph/MainTest.scala
+-rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/core/src/test/scala/com/databricks/labs/remorph/parsers/ParserTestCommon.scala
+-rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/core/src/test/scala/com/databricks/labs/remorph/parsers/snowflake/DataTypeBuilderSpec.scala
+-rw-r--r--   0        0        0    15017 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/core/src/test/scala/com/databricks/labs/remorph/parsers/snowflake/SnowflakeAstBuilderSpec.scala
+-rw-r--r--   0        0        0     9428 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/core/src/test/scala/com/databricks/labs/remorph/parsers/snowflake/SnowflakeDDLBuilderSpec.scala
+-rw-r--r--   0        0        0    12839 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/core/src/test/scala/com/databricks/labs/remorph/parsers/snowflake/SnowflakeExpressionBuilderSpec.scala
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/core/src/test/scala/com/databricks/labs/remorph/parsers/snowflake/SnowflakeParserTestCommon.scala
+-rw-r--r--   0        0        0     5919 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/core/src/test/scala/com/databricks/labs/remorph/parsers/snowflake/SnowflakeRelationBuilderSpec.scala
+-rw-r--r--   0        0        0     4720 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/core/src/test/scala/com/databricks/labs/remorph/parsers/tsql/TSqlAstBuilderSpec.scala
+-rw-r--r--   0        0        0     7189 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/core/src/test/scala/com/databricks/labs/remorph/parsers/tsql/TSqlExpressionBuilderSpec.scala
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/core/src/test/scala/com/databricks/labs/remorph/parsers/tsql/TSqlParserTestCommon.scala
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/databricks/__init__.py
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/databricks/labs/__init__.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/databricks/labs/remorph/__about__.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/databricks/labs/remorph/__init__.py
+-rw-r--r--   0        0        0     5082 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/databricks/labs/remorph/cli.py
+-rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/databricks/labs/remorph/config.py
+-rw-r--r--   0        0        0     8693 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/databricks/labs/remorph/install.py
+-rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/databricks/labs/remorph/lineage.py
+-rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/databricks/labs/remorph/uninstall.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/databricks/labs/remorph/coverage/__init__.py
+-rw-r--r--   0        0        0     5749 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/databricks/labs/remorph/coverage/commons.py
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/databricks/labs/remorph/coverage/remorph_snow_transpilation_coverage.py
+-rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/databricks/labs/remorph/coverage/sqlglot_snow_transpilation_coverage.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/databricks/labs/remorph/helpers/__init__.py
+-rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/databricks/labs/remorph/helpers/db_sql.py
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/databricks/labs/remorph/helpers/execution_time.py
+-rw-r--r--   0        0        0     3913 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/databricks/labs/remorph/helpers/file_utils.py
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/databricks/labs/remorph/helpers/morph_status.py
+-rw-r--r--   0        0        0     7412 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/databricks/labs/remorph/helpers/recon_config_utils.py
+-rw-r--r--   0        0        0     4242 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/databricks/labs/remorph/helpers/validation.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/databricks/labs/remorph/intermediate/__init__.py
+-rw-r--r--   0        0        0     3112 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/databricks/labs/remorph/intermediate/dag.py
+-rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/databricks/labs/remorph/intermediate/engine_adapter.py
+-rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/databricks/labs/remorph/intermediate/root_tables.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/databricks/labs/remorph/reconcile/__init__.py
+-rw-r--r--   0        0        0     4696 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/databricks/labs/remorph/reconcile/compare.py
+-rw-r--r--   0        0        0     2495 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/databricks/labs/remorph/reconcile/constants.py
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/databricks/labs/remorph/reconcile/exception.py
+-rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/databricks/labs/remorph/reconcile/execute.py
+-rw-r--r--   0        0        0     5635 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/databricks/labs/remorph/reconcile/recon_config.py
+-rw-r--r--   0        0        0     5049 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/databricks/labs/remorph/reconcile/schema_compare.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/databricks/labs/remorph/reconcile/connectors/__init__.py
+-rw-r--r--   0        0        0     1967 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/databricks/labs/remorph/reconcile/connectors/data_source.py
+-rw-r--r--   0        0        0     2396 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/databricks/labs/remorph/reconcile/connectors/databricks.py
+-rw-r--r--   0        0        0     3806 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/databricks/labs/remorph/reconcile/connectors/oracle.py
+-rw-r--r--   0        0        0     3657 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/databricks/labs/remorph/reconcile/connectors/snowflake.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/databricks/labs/remorph/reconcile/query_builder/__init__.py
+-rw-r--r--   0        0        0     4246 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/databricks/labs/remorph/reconcile/query_builder/base.py
+-rw-r--r--   0        0        0     8512 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/databricks/labs/remorph/reconcile/query_builder/expression_generator.py
+-rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/databricks/labs/remorph/reconcile/query_builder/hash_query.py
+-rw-r--r--   0        0        0     2333 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/databricks/labs/remorph/reconcile/query_builder/sampling_query.py
+-rw-r--r--   0        0        0     7481 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/databricks/labs/remorph/reconcile/query_builder/threshold_query.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/databricks/labs/remorph/snow/__init__.py
+-rw-r--r--   0        0        0    26739 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/databricks/labs/remorph/snow/databricks.py
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/databricks/labs/remorph/snow/experimental.py
+-rw-r--r--   0        0        0     4805 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/databricks/labs/remorph/snow/lca_utils.py
+-rw-r--r--   0        0        0     3408 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/databricks/labs/remorph/snow/local_expression.py
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/databricks/labs/remorph/snow/oracle.py
+-rw-r--r--   0        0        0    22385 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/databricks/labs/remorph/snow/snowflake.py
+-rw-r--r--   0        0        0     2103 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/databricks/labs/remorph/snow/sql_transpiler.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/databricks/labs/remorph/transpiler/__init__.py
+-rw-r--r--   0        0        0     7048 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/databricks/labs/remorph/transpiler/execute.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/.gitignore
+-rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/LICENSE
+-rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/NOTICE
+-rw-r--r--   0        0        0     6443 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/README.md
+-rw-r--r--   0        0        0    26966 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     7367 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/PKG-INFO
```

### Comparing `databricks_labs_remorph-0.1.6/databricks/labs/remorph/install.py` & `databricks_labs_remorph-0.1.7/databricks/labs/remorph/install.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,26 +6,25 @@
 from pathlib import Path
 
 from databricks.labs.blueprint.entrypoint import get_logger
 from databricks.labs.blueprint.installation import Installation
 from databricks.labs.blueprint.installer import InstallState
 from databricks.labs.blueprint.tui import Prompts
 from databricks.labs.blueprint.wheels import ProductInfo
+from databricks.labs.remorph.__about__ import __version__
+from databricks.labs.remorph.config import SQLGLOT_DIALECTS, MorphConfig
 from databricks.sdk import WorkspaceClient
 from databricks.sdk.errors import NotFound
 from databricks.sdk.retries import retried
 from databricks.sdk.service.sql import (
     CreateWarehouseRequestWarehouseType,
     EndpointInfoWarehouseType,
     SpotInstancePolicy,
 )
 
-from databricks.labs.remorph.__about__ import __version__
-from databricks.labs.remorph.config import MorphConfig
-
 logger = logging.getLogger(__name__)
 
 PRODUCT_INFO = ProductInfo(__file__)
 WAREHOUSE_PREFIX = "Remorph Transpiler Validation"
 
 
 class WorkspaceInstaller:
@@ -58,15 +57,15 @@
         logger.info("Please answer a couple of questions to configure Remorph")
 
         # default params
         catalog_name = "transpiler_test"
         schema_name = "convertor_test"
         ws_config = None
 
-        source_prompt = self._prompts.choice("Select the source", ["snowflake", "tsql"])
+        source_prompt = self._prompts.choice("Select the source", SQLGLOT_DIALECTS.keys())
         source = source_prompt.lower()
 
         skip_validation = self._prompts.confirm("Do you want to Skip Validation")
 
         if not skip_validation:
             ws_config = self._configure_runtime()
             catalog_name = self._prompts.question("Enter catalog_name")
@@ -84,32 +83,33 @@
 
         config = MorphConfig(
             source=source,
             skip_validation=skip_validation,
             catalog_name=catalog_name,
             schema_name=schema_name,
             sdk_config=ws_config,
+            mode="current",  # mode will not have a prompt as this is hidden flag
         )
 
         ws_file_url = self._installation.save(config)
         if self._prompts.confirm("Open config file in the browser and continue installing?"):
             webbrowser.open(ws_file_url)
         return config
 
     def _configure_runtime(self) -> dict[str, str]:
         if self._prompts.confirm("Do you want to use SQL Warehouse for validation?"):
             warehouse_id = self._configure_warehouse()
             return {"warehouse_id": warehouse_id}
 
         if self._ws.config.cluster_id:
             logger.info(f"Using cluster {self._ws.config.cluster_id} for validation")
-            return {"cluster": self._ws.config.cluster_id}
+            return {"cluster_id": self._ws.config.cluster_id}
 
         cluster_id = self._prompts.question("Enter a valid cluster_id to proceed")
-        return {"cluster": cluster_id}
+        return {"cluster_id": cluster_id}
 
     def _configure_warehouse(self):
         def warehouse_type(_):
             return _.warehouse_type.value if not _.enable_serverless_compute else "SERVERLESS"
 
         pro_warehouses = {"[Create new PRO SQL warehouse]": "create_new"} | {
             f"{_.name} ({_.id}, {warehouse_type(_)}, {_.state.value})": _.id
```

### Comparing `databricks_labs_remorph-0.1.6/databricks/labs/remorph/uninstall.py` & `databricks_labs_remorph-0.1.7/databricks/labs/remorph/uninstall.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 import logging
 from datetime import timedelta
 
 from databricks.labs.blueprint.installation import Installation
 from databricks.labs.blueprint.tui import Prompts
 from databricks.labs.blueprint.wheels import ProductInfo
-from databricks.sdk import WorkspaceClient
-from databricks.sdk.errors import NotFound
-
 from databricks.labs.remorph.__about__ import __version__
 from databricks.labs.remorph.config import MorphConfig
+from databricks.sdk import WorkspaceClient
+from databricks.sdk.errors import NotFound
 
 logger = logging.getLogger("databricks.labs.remorph.install")
 
 PRODUCT_INFO = ProductInfo(__file__)
 
 
 class WorkspaceUnInstallation:
```

### Comparing `databricks_labs_remorph-0.1.6/databricks/labs/remorph/coverage/commons.py` & `databricks_labs_remorph-0.1.7/databricks/labs/remorph/coverage/commons.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_remorph-0.1.6/databricks/labs/remorph/coverage/remorph_snow_transpilation_coverage.py` & `databricks_labs_remorph-0.1.7/databricks/labs/remorph/coverage/remorph_snow_transpilation_coverage.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from pathlib import Path
 
 from databricks.labs.blueprint.wheels import ProductInfo
-
 from databricks.labs.remorph.coverage import commons
 from databricks.labs.remorph.snow.databricks import Databricks
 from databricks.labs.remorph.snow.snowflake import Snow
 
 if __name__ == "__main__":
     input_dir = commons.get_env_var("INPUT_DIR", required=True)
     output_dir = commons.get_env_var("OUTPUT_DIR", required=True)
```

### Comparing `databricks_labs_remorph-0.1.6/databricks/labs/remorph/coverage/sqlglot_snow_transpilation_coverage.py` & `databricks_labs_remorph-0.1.7/databricks/labs/remorph/coverage/sqlglot_snow_transpilation_coverage.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_remorph-0.1.6/databricks/labs/remorph/helpers/db_sql.py` & `databricks_labs_remorph-0.1.7/databricks/labs/remorph/helpers/db_sql.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,19 +3,18 @@
 
 from databricks.labs.lsql.backends import (
     DatabricksConnectBackend,
     RuntimeBackend,
     SqlBackend,
     StatementExecutionBackend,
 )
+from databricks.labs.remorph.config import MorphConfig
 from databricks.sdk import WorkspaceClient
 from databricks.sdk.errors.base import DatabricksError
 
-from databricks.labs.remorph.config import MorphConfig
-
 logger = logging.getLogger(__name__)
 
 
 def get_sql_backend(ws: WorkspaceClient, config: MorphConfig) -> SqlBackend:
     sdk_config = config.sdk_config
     warehouse_id = sdk_config.get("warehouse_id", None) if sdk_config else None
     cluster_id = sdk_config.get("cluster_id", None) if sdk_config else None
```

### Comparing `databricks_labs_remorph-0.1.6/databricks/labs/remorph/helpers/execution_time.py` & `databricks_labs_remorph-0.1.7/databricks/labs/remorph/helpers/execution_time.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_remorph-0.1.6/databricks/labs/remorph/helpers/file_utils.py` & `databricks_labs_remorph-0.1.7/databricks/labs/remorph/helpers/file_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -84,7 +84,20 @@
     Reads the contents of the given file and returns it as a string.
     :param filename: Input File Path
     :return: File Contents as String
     """
     # pylint: disable=unspecified-encoding
     with Path(filename).open() as file:
         return file.read()
+
+
+def refactor_hexadecimal_chars(input_string: str) -> str:
+    """
+    Updates the HexaDecimal characters ( \x1b[\\d+m ) in the given string as below.
+    :param input_string: String with HexaDecimal characters. ex: ( \x1b[4mWHERE\x1b[0m )
+    :return: String with HexaDecimal characters refactored to arrows. ex: ( --> WHERE <--)
+    """
+    output_string = input_string
+    highlight = {"\x1b[4m": "--> ", "\x1b[0m": " <--"}
+    for key, value in highlight.items():
+        output_string = output_string.replace(key, value)
+    return output_string
```

### Comparing `databricks_labs_remorph-0.1.6/databricks/labs/remorph/helpers/validation.py` & `databricks_labs_remorph-0.1.7/databricks/labs/remorph/helpers/validation.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import logging
 from io import StringIO
 
 from databricks.labs.lsql.backends import SqlBackend
-from databricks.sdk.errors.base import DatabricksError
-
 from databricks.labs.remorph.config import MorphConfig
+from databricks.sdk.errors.base import DatabricksError
 
 logger = logging.getLogger(__name__)
 
 
 class Validator:
     """
     The Validator class is used to validate SQL queries.
@@ -28,18 +27,19 @@
         - config (MorphConfig): The configuration for the validation.
         - input_sql (str): The SQL query to be validated.
 
         Returns:
         - tuple: A tuple containing the result of the validation and the exception message (if any).
         """
         logger.debug(f"Validating query with catalog {config.catalog_name} and schema {config.schema_name}")
-        (is_valid, exception_msg) = self._query(self._sql_backend, input_sql)
+        (is_valid, exception_type, exception_msg) = self._query(self._sql_backend, input_sql)
         if is_valid:
             result = input_sql + "\n;\n"
-            exception_msg = None
+            if exception_type is not None:
+                exception_msg = f"[{exception_type.upper()}]: {exception_msg}"
         else:
             query = ""
             if "[UNRESOLVED_ROUTINE]" in exception_msg:
                 query = input_sql
             buffer = StringIO()
             buffer.write("-------------- Exception Start-------------------\n")
             buffer.write("/* \n")
@@ -48,15 +48,15 @@
             buffer.write(query)
             buffer.write("\n ---------------Exception End --------------------\n")
 
             result = buffer.getvalue()
 
         return result, exception_msg
 
-    def _query(self, sql_backend: SqlBackend, query: str) -> tuple[bool, str | None]:
+    def _query(self, sql_backend: SqlBackend, query: str) -> tuple[bool, str | None, str | None]:
         """
         Validate a given SQL query using the provided SQL backend
 
         Parameters:
         - query (str): The SQL query to be validated.
         - sql_backend (SqlBackend): The SQL backend to be used for validation.
 
@@ -65,30 +65,30 @@
         and a string containing a success message or an exception message.
         """
         # When variables is mentioned Explain fails we need way to replace them before explain is executed.
         explain_query = f'EXPLAIN {query.replace("${", "`{").replace("}", "}`").replace("``", "`")}'
         try:
             rows = list(sql_backend.fetch(explain_query))
             if not rows:
-                return False, "No results returned from explain query."
+                return False, "error", "No results returned from explain query."
 
             if "Error occurred during query planning" in rows[0].as_dict().get("plan", ""):
                 error_details = rows[1].as_dict().get("plan", "Unknown error.") if len(rows) > 1 else "Unknown error."
                 raise DatabricksError(error_details)
-            return True, None
+            return True, None, None
         except DatabricksError as dbe:
             err_msg = str(dbe)
             if "[PARSE_SYNTAX_ERROR]" in err_msg:
                 logger.debug(f"Syntax Exception : NOT IGNORED. Flag as syntax error: {err_msg}")
-                return False, err_msg
+                return False, "error", err_msg
             if "[UNRESOLVED_ROUTINE]" in err_msg:
                 logger.debug(f"Analysis Exception : NOT IGNORED: Flag as Function Missing error {err_msg}")
-                return False, err_msg
+                return False, "error", err_msg
             if "[TABLE_OR_VIEW_NOT_FOUND]" in err_msg or "[TABLE_OR_VIEW_ALREADY_EXISTS]" in err_msg:
                 logger.debug(f"Analysis Exception : IGNORED: {err_msg}")
-                return True, err_msg
+                return True, "warning", err_msg
             if "Hive support is required to CREATE Hive TABLE (AS SELECT).;" in err_msg:
                 logger.debug(f"Analysis Exception : IGNORED: {err_msg}")
-                return True, err_msg
+                return True, "warning", err_msg
 
             logger.debug(f"Unknown Exception: {err_msg}")
-            return False, err_msg
+            return False, "error", err_msg
```

### Comparing `databricks_labs_remorph-0.1.6/databricks/labs/remorph/intermediate/dag.py` & `databricks_labs_remorph-0.1.7/databricks/labs/remorph/intermediate/dag.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_remorph-0.1.6/databricks/labs/remorph/intermediate/root_tables.py` & `databricks_labs_remorph-0.1.7/databricks/labs/remorph/intermediate/root_tables.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import logging
 from pathlib import Path
 
+from databricks.labs.remorph.config import SQLGLOT_DIALECTS
 from databricks.labs.remorph.helpers.file_utils import (
     get_sql_file,
     is_sql_file,
     read_file,
 )
 from databricks.labs.remorph.intermediate.dag import DAG
 from databricks.labs.remorph.intermediate.engine_adapter import EngineAdapter
@@ -12,15 +13,15 @@
 logger = logging.getLogger(__name__)
 
 
 class RootTableIdentifier:
     def __init__(self, source: str, input_path: str | Path):
         self.source = source
         self.input_path = input_path
-        self.engine_adapter = EngineAdapter(source)
+        self.engine_adapter = EngineAdapter(SQLGLOT_DIALECTS.get(source))
 
     def generate_lineage(self, engine="sqlglot") -> DAG:
         dag = DAG()
 
         # when input is sql file then parse the file
         if is_sql_file(self.input_path):
             filename = self.input_path
```

### Comparing `databricks_labs_remorph-0.1.6/databricks/labs/remorph/reconcile/constants.py` & `databricks_labs_remorph-0.1.7/databricks/labs/remorph/reconcile/constants.py`

 * *Files 5% similar despite different names*

```diff
@@ -54,32 +54,39 @@
     DATA = "data"
     SCHEMA = "schema"
     HASH = "hash"
     ALL = "all"
 
 
 class ThresholdMode(AutoName):
-    PERCENTILE = "percentile"
+    PERCENTAGE = "percentage"
     ABSOLUTE = "absolute"
+    NUMBER_ABSOLUTE = "number_absolute"
+    NUMBER_PERCENTAGE = "number_percentage"
+    DATETIME = "datetime"
 
 
 class ThresholdMatchType(AutoName):
     INTEGER = "integer"
     TIMESTAMP = "timestamp"
 
 
 class Constants:
-    hash_column_name = "hash_value__recon"
+    hash_column_name = "hash_value_recon"
     hash_algorithm_mapping = {  # noqa RUF012
         SourceType.SNOWFLAKE.value: {
             "source": HashAlgorithm.SNOWFLAKE_SHA_256.value,
             "target": HashAlgorithm.DATABRICKS_SHA_256.value,
         },
         SourceType.ORACLE.value: {
             "source": HashAlgorithm.ORACLE_SHA_256.value,
             "target": HashAlgorithm.DATABRICKS_SHA_256.value,
         },
         SourceType.DATABRICKS.value: {
             "source": HashAlgorithm.DATABRICKS_SHA_256.value,
             "target": HashAlgorithm.DATABRICKS_SHA_256.value,
         },
     }
+
+
+class SampleConfig:
+    SAMPLE_ROWS = 50
```

### Comparing `databricks_labs_remorph-0.1.6/databricks/labs/remorph/reconcile/execute.py` & `databricks_labs_remorph-0.1.7/databricks/labs/remorph/reconcile/execute.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 from pathlib import Path
 
 from databricks.labs.blueprint.installation import Installation
-
+from databricks.labs.remorph.config import TableRecon
 from databricks.labs.remorph.reconcile.connectors.data_source import DataSource
-from databricks.labs.remorph.reconcile.recon_config import Table, TableRecon
+from databricks.labs.remorph.reconcile.recon_config import Table
 
 logger = logging.getLogger(__name__)
 
 
 def recon(recon_conf, conn_profile, source, report):
     logger.info(conn_profile)
     logger.info(source)
```

### Comparing `databricks_labs_remorph-0.1.6/databricks/labs/remorph/reconcile/connectors/data_source.py` & `databricks_labs_remorph-0.1.7/databricks/labs/remorph/reconcile/connectors/data_source.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 import re
 from abc import ABC, abstractmethod
 
-from databricks.sdk import WorkspaceClient  # pylint: disable-next=wrong-import-order
 from pyspark.sql import DataFrame, SparkSession
 
-from databricks.labs.remorph.reconcile.recon_config import (  # pylint: disable=ungrouped-imports
-    JdbcReaderOptions,
-    Schema,
-)
+from databricks.labs.remorph.reconcile.recon_config import JdbcReaderOptions, Schema
+from databricks.sdk import WorkspaceClient
 
 
 class DataSource(ABC):
     # TODO need to remove connection_params
     def __init__(
         self,
         engine: str,
```

### Comparing `databricks_labs_remorph-0.1.6/databricks/labs/remorph/reconcile/connectors/databricks.py` & `databricks_labs_remorph-0.1.7/databricks/labs/remorph/reconcile/connectors/databricks.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_remorph-0.1.6/databricks/labs/remorph/reconcile/connectors/oracle.py` & `databricks_labs_remorph-0.1.7/databricks/labs/remorph/reconcile/connectors/oracle.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_remorph-0.1.6/databricks/labs/remorph/reconcile/connectors/snowflake.py` & `databricks_labs_remorph-0.1.7/databricks/labs/remorph/reconcile/connectors/snowflake.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_remorph-0.1.6/databricks/labs/remorph/reconcile/query_builder/hash_query.py` & `databricks_labs_remorph-0.1.7/databricks/labs/remorph/reconcile/query_builder/hash_query.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,58 +1,49 @@
-from io import StringIO
+import sqlglot.expressions as exp
 
-from databricks.labs.remorph.reconcile.constants import Constants, SourceType
+from databricks.labs.remorph.reconcile.constants import Constants
 from databricks.labs.remorph.reconcile.query_builder.base import QueryBuilder
-from databricks.labs.remorph.reconcile.recon_config import TransformRuleMapping
+from databricks.labs.remorph.reconcile.query_builder.expression_generator import (
+    build_column,
+    concat,
+    get_hash_transform,
+    lower,
+    transform_expression,
+)
 
 
 class HashQueryBuilder(QueryBuilder):
-
     def build_query(self) -> str:
-        hash_cols = sorted(
-            (self.table_conf.get_join_columns | self.select_columns)
-            - self.table_conf.get_threshold_columns
-            - self.table_conf.get_drop_columns
-        )
-        key_cols = sorted(self.table_conf.get_join_columns | self.table_conf.get_partition_column(self.layer))
+        hash_cols = sorted((self.join_columns | self.select_columns) - self.threshold_columns - self.drop_columns)
+        key_cols = sorted(self.join_columns | self.partition_column)
 
-        # get transformation for columns considered for hashing
-        col_transform = self._generate_transform_rule_mapping(hash_cols)
-        hash_cols_expr = sorted(
-            self._get_column_expr(TransformRuleMapping.get_column_expr_without_alias, col_transform)
+        cols_with_alias = [
+            build_column(this=col, alias=self.table_conf.get_tgt_to_src_col_mapping(col, self.layer))
+            for col in key_cols
+        ]
+
+        key_cols_with_transform = self.add_transformations(cols_with_alias, self.source)
+        hash_col_with_transform = [self._generate_hash_algorithm(hash_cols)]
+
+        res = (
+            exp.select(*hash_col_with_transform + key_cols_with_transform)
+            .from_(":tbl")
+            .where(self.filter)
+            .sql(dialect=self.source)
         )
-        hash_expr = self._generate_hash_algorithm(self.source, hash_cols_expr)
 
-        # get transformation for columns considered for joining and partition key
-        key_col_transform = self._generate_transform_rule_mapping(key_cols)
-        key_col_expr = sorted(self._get_column_expr(TransformRuleMapping.get_column_expr_with_alias, key_col_transform))
-
-        # construct select hash query
-        select_query = self._construct_hash_query(
-            self.table_name, self.table_conf.get_filter(self.layer), hash_expr, key_col_expr
-        )
+        return res
 
-        return select_query
+    def _generate_hash_algorithm(self, cols: list[str]) -> exp.Expression:
+        cols_with_alias = [build_column(this=col, alias=None) for col in cols]
+        cols_with_transform = self.add_transformations(cols_with_alias, self.source)
+        col_exprs = exp.select(*cols_with_transform).iter_expressions()
+        concat_expr = concat(list(col_exprs))
 
-    @staticmethod
-    def _generate_hash_algorithm(source: str, col_expr: list[str]) -> str:
-        if source in {SourceType.DATABRICKS.value, SourceType.SNOWFLAKE.value}:
-            hash_expr = "concat(" + ", ".join(col_expr) + ")"
-        else:
-            hash_expr = " || ".join(col_expr)
+        hash_expr = concat_expr.transform(self._hash_transform, self.source).transform(lower, is_expr=True)
 
-        return (Constants.hash_algorithm_mapping.get(source).get("source")).format(hash_expr)
+        return build_column(hash_expr, alias=Constants.hash_column_name)
 
     @staticmethod
-    def _construct_hash_query(table: str, query_filter: str, hash_expr: str, key_col_expr: list[str]) -> str:
-        sql_query = StringIO()
-        # construct hash expr
-        sql_query.write(f"select {hash_expr} as {Constants.hash_column_name}")
-
-        # add join column
-        if key_col_expr:
-            sql_query.write(", " + ",".join(key_col_expr))
-        sql_query.write(f" from {table} where {query_filter}")
-
-        select_query = sql_query.getvalue()
-        sql_query.close()
-        return select_query
+    def _hash_transform(node: exp.Expression, source: str):
+        transform = get_hash_transform(source)
+        return transform_expression(node, transform)
```

### Comparing `databricks_labs_remorph-0.1.6/databricks/labs/remorph/snow/databricks.py` & `databricks_labs_remorph-0.1.7/databricks/labs/remorph/snow/databricks.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from sqlglot import expressions as exp
 from sqlglot.dialects import hive
 from sqlglot.dialects.databricks import Databricks
 from sqlglot.dialects.dialect import rename_func
 from sqlglot.errors import ParseError, UnsupportedError
 from sqlglot.helper import apply_index_offset, csv
 
-from databricks.labs.remorph.snow import local_expression
+from databricks.labs.remorph.snow import lca_utils, local_expression
 
 logger = logging.getLogger(__name__)
 
 VALID_DATABRICKS_TYPES = {
     "BIGINT",
     "BINARY",
     "BOOLEAN",
@@ -75,53 +75,64 @@
     return self.create_sql(expression)
 
 
 def _curr_time():
     return "date_format(current_timestamp(), 'HH:mm:ss')"
 
 
-def _lateral_view(self, expression: exp.Lateral) -> str:
-    str_lateral_view = "LATERAL VIEW"
-    str_outer = "OUTER"
-    str_explode = "EXPLODE("
-    str_pfx = f"{str_lateral_view} {str_explode}"
-    str_alias = ")"
+def _select_contains_index(expression: exp.Select) -> bool:
+    for expr in expression.expressions:
+        column = expr.unalias() if isinstance(expr, exp.Alias) else expr
+        if column.name == "index":
+            return True
+    return False
 
+
+def _lateral_view(self: Databricks.Generator, expression: exp.Lateral) -> str:
     this = expression.args['this']
     alias = expression.args['alias']
-    # [TODO]: Implement for options: RECURSIVE and MODE
-    # view = expression.args['view']
-    # outer = expression.args['outer']
-    # cross_apply = expression.args['cross_apply']
+    alias_str = f" AS {alias.name}" if isinstance(alias, exp.TableAlias) else ""
+    generator_function_str = self.sql(this)
+    is_outer = False
+
     if isinstance(this, exp.Explode):
         explode_expr = this
+        parent_select = explode_expr.parent_select
+        select_contains_index = _select_contains_index(parent_select) if parent_select else False
+        generator_expr = ""
         if isinstance(explode_expr.this, exp.Kwarg):
-            str_pfx = str_pfx + self.sql(explode_expr.this, 'expression')
+            generator_expr = self.sql(explode_expr.this, 'expression')
             if not isinstance(explode_expr.this.expression, exp.ParseJSON):
-                str_pfx = str_pfx.replace("{", "").replace("}", "")
-
+                generator_expr = generator_expr.replace("{", "").replace("}", "")
         for expr in explode_expr.expressions:
             node = str(expr.this).upper()
             if node == "PATH":
-                str_pfx = str_pfx + "." + self.sql(expr, 'expression').replace("'", "")
+                generator_expr += "." + self.sql(expr, 'expression').replace("'", "")
             if node == "OUTER":
-                str_pfx = str_pfx.replace(str_lateral_view, f"{str_lateral_view} {str_outer}")
+                is_outer = True
 
-        if isinstance(alias, exp.TableAlias):
-            str_alias = str_alias + f" AS {alias.name}"
+        if select_contains_index:
+            generator_function_str = f"POSEXPLODE({generator_expr})"
+            alias_str = f"{' ' + alias.name if isinstance(alias, exp.TableAlias) else ''} AS index, value"
+        else:
+            generator_function_str = f"EXPLODE({generator_expr})"
 
-    return self.sql(str_pfx + str_alias)
+    return self.sql(f"LATERAL VIEW {'OUTER ' if is_outer else ''}{generator_function_str}{alias_str}")
 
 
 # [TODO] Add more datatype coverage https://docs.databricks.com/sql/language-manual/sql-ref-datatypes.html
 def _datatype_map(self, expression) -> str:
     if expression.this in [exp.DataType.Type.VARCHAR, exp.DataType.Type.NVARCHAR, exp.DataType.Type.CHAR]:
         return "STRING"
     if expression.this in [exp.DataType.Type.TIMESTAMP, exp.DataType.Type.TIMESTAMPLTZ]:
         return "TIMESTAMP"
+    if expression.this == exp.DataType.Type.BINARY:
+        return "BINARY"
+    if expression.this == exp.DataType.Type.NCHAR:
+        return "STRING"
     return self.datatype_sql(expression)
 
 
 def try_to_date(self, expression: local_expression.TryToDate):
     func = "TRY_TO_TIMESTAMP"
     time_format = self.sql(expression, "format")
     if not time_format:
@@ -331,14 +342,16 @@
             exp.DataType.Type.SMALLINT: "SMALLINT",
             exp.DataType.Type.INT: "INT",
             exp.DataType.Type.BIGINT: "BIGINT",
             exp.DataType.Type.DATETIME: "TIMESTAMP",
             exp.DataType.Type.VARCHAR: "STRING",
             exp.DataType.Type.VARIANT: "STRING",
             exp.DataType.Type.FLOAT: "DOUBLE",
+            exp.DataType.Type.OBJECT: "STRING",
+            exp.DataType.Type.GEOGRAPHY: "STRING",
         }
 
         TRANSFORMS: ClassVar[dict] = {
             **Databricks.Generator.TRANSFORMS,
             exp.Create: _format_create_sql,
             exp.DataType: _datatype_map,
             exp.CurrentTime: _curr_time(),
@@ -366,16 +379,21 @@
             exp.ToBase64: rename_func("BASE64"),
             local_expression.ToNumber: _to_number,
             local_expression.UUID: _uuid,
             local_expression.DateTrunc: _parse_date_trunc,
             exp.ApproxQuantile: rename_func("APPROX_PERCENTILE"),
             exp.TimestampTrunc: timestamptrunc_sql,
             exp.Mod: rename_func("MOD"),
+            exp.NullSafeEQ: lambda self, e: self.binary(e, "<=>"),
         }
 
+        def preprocess(self, expression: exp.Expression) -> exp.Expression:
+            fixed_ast = expression.transform(lca_utils.unalias_lca_in_select, copy=False)
+            return super().preprocess(fixed_ast)
+
         def join_sql(self, expression: exp.Join) -> str:
             """Overwrites `join_sql()` in `sqlglot/generator.py`
             Added logic to handle Lateral View
             """
             op_list = [
                 expression.method,
                 "GLOBAL" if expression.args.get("global") else None,
@@ -617,7 +635,24 @@
 
             if from_sql:
                 sql = f"MERGE INTO {this}{expression_sql} WHEN MATCHED THEN UPDATE SET {set_sql}{order}{limit}"
             else:
                 sql = f"UPDATE {this} SET {set_sql}{expression_sql}{order}{limit}"
 
             return self.prepend_ctes(expression, sql)
+
+        def struct_sql(self, expression: exp.Struct) -> str:
+            expression.set(
+                "expressions",
+                [
+                    (
+                        exp.alias_(
+                            e.expression, e.name if hasattr(e.this, "is_string") and e.this.is_string else e.this
+                        )
+                        if isinstance(e, exp.PropertyEQ)
+                        else e
+                    )
+                    for e in expression.expressions
+                ],
+            )
+
+            return self.function_fallback_sql(expression)
```

### Comparing `databricks_labs_remorph-0.1.6/databricks/labs/remorph/snow/dialect_utils.py` & `databricks_labs_remorph-0.1.7/databricks/labs/remorph/snow/lca_utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import logging
 
 from sqlglot import ErrorLevel, exp, parse
 from sqlglot.errors import ParseError, TokenError, UnsupportedError
 from sqlglot.expressions import Expression, Select
+from sqlglot.optimizer.scope import build_scope
 
 from databricks.labs.remorph.helpers.morph_status import ValidationError
+from databricks.labs.remorph.snow.local_expression import AliasInfo
 from databricks.labs.remorph.snow.snowflake import Snow
 
 logger = logging.getLogger(__name__)
 
 
 def check_for_unsupported_lca(
     dialect: str,
@@ -30,71 +32,100 @@
 
     aliases_in_where = set()
     aliases_in_window = set()
 
     for expr in parsed_expr:
         if expr:
             for select in expr.find_all(exp.Select, bfs=False):
-                alias_names = _find_aliases_in_select(select)
-                aliases_in_where.update(_find_invalid_lca_in_where(select, alias_names))
-                aliases_in_window.update(_find_invalid_lca_in_window(select, alias_names))
+                alias_info = _find_aliases_in_select(select)
+                aliases_in_where.update(_find_invalid_lca_in_where(select, alias_info))
+                aliases_in_window.update(_find_invalid_lca_in_window(select, alias_info))
 
     if not (aliases_in_where or aliases_in_window):
         return None
 
     err_messages = [f"Unsupported operation found in file {filename}. Needs manual review of transpiled query."]
     if aliases_in_where:
         err_messages.append(f"Lateral column aliases `{', '.join(aliases_in_where)}` found in where clause.")
 
     if aliases_in_window:
         err_messages.append(f"Lateral column aliases `{', '.join(aliases_in_window)}` found in window expressions.")
 
     return ValidationError(filename, " ".join(err_messages))
 
 
+def unalias_lca_in_select(expr: exp.Expression) -> exp.Expression:
+    if not isinstance(expr, exp.Select):
+        return expr
+    root_select = build_scope(expr)
+    # We won't search inside nested selects, they will be visited separately
+    nested_selects = {*root_select.derived_tables, *root_select.subqueries}
+    alias_info = _find_aliases_in_select(expr)
+    where_ast: Expression = expr.args.get("where")
+    if where_ast:
+        for column in where_ast.walk(prune=lambda n: n in nested_selects):
+            if (
+                isinstance(column, exp.Column)
+                and column.name in alias_info
+                and not alias_info[column.name].is_same_name_as_column
+            ):
+                column.replace(alias_info[column.name].expression)
+    for window in _find_windows_in_select(expr):
+        for column in window.walk():
+            if (
+                isinstance(column, exp.Column)
+                and column.name in alias_info
+                and not alias_info[column.name].is_same_name_as_column
+            ):
+                column.replace(alias_info[column.name].expression)
+    return expr
+
+
 def _find_windows_in_select(select: Select) -> list[exp.Window]:
     window_expressions = []
     for expr in select.expressions:
         window_expr = expr.find(exp.Window)
         if window_expr:
             window_expressions.append(window_expr)
     return window_expressions
 
 
-def _find_aliases_in_select(select_expr: Select) -> dict[str, bool]:
-    aliases = {}  # Alias name and if it is same as a column name used in the alias expression
+def _find_aliases_in_select(select_expr: Select) -> dict[str, AliasInfo]:
+    aliases = {}
     for expr in select_expr.expressions:
         if isinstance(expr, exp.Alias):
-            aliases[expr.output_name] = False
+            alias_name = expr.output_name
+            is_same_name_as_column = False
             for column in expr.find_all(exp.Column):
-                if column.name == expr.output_name:
-                    aliases[expr.output_name] = True
+                if column.name == alias_name:
+                    is_same_name_as_column = True
                     break
+            aliases[alias_name] = AliasInfo(alias_name, expr.unalias(), is_same_name_as_column)
     return aliases
 
 
 def _find_invalid_lca_in_where(
     select_expr: Select,
-    aliases: dict[str, bool],
+    aliases: dict[str, AliasInfo],
 ) -> set[str]:
     aliases_in_where = set()
     where_ast: Expression = select_expr.args.get("where")
     if where_ast:
         for column in where_ast.find_all(exp.Column):
-            if column.name in aliases and not aliases[column.name]:
+            if column.name in aliases and not aliases[column.name].is_same_name_as_column:
                 aliases_in_where.add(column.name)
 
     return aliases_in_where
 
 
 def _find_invalid_lca_in_window(
     select_expr: Select,
-    aliases: dict[str, bool],
+    aliases: dict[str, AliasInfo],
 ) -> set[str]:
     aliases_in_window = set()
     windows = _find_windows_in_select(select_expr)
     for window in windows:
         for column in window.find_all(exp.Column):
-            if column.name in aliases and not aliases[column.name]:
+            if column.name in aliases and not aliases[column.name].is_same_name_as_column:
                 aliases_in_window.add(column.name)
 
     return aliases_in_window
```

### Comparing `databricks_labs_remorph-0.1.6/databricks/labs/remorph/snow/local_expression.py` & `databricks_labs_remorph-0.1.7/databricks/labs/remorph/snow/local_expression.py`

 * *Files 13% similar despite different names*

```diff
@@ -126,12 +126,23 @@
     arg_types: ClassVar[dict] = {"this": False, "name": False}
 
 
 class DateTrunc(Func):
     arg_types: ClassVar[dict] = {"unit": False, "this": True, "zone": False}
 
 
+class Median(Func):
+    arg_types: ClassVar[dict] = {"this": True}
+
+
 @dataclass
 class WithinGroupParams:
     agg_col: exp.Column
     order_col: exp.Column
     is_order_asc: bool
+
+
+@dataclass
+class AliasInfo:
+    name: str
+    expression: exp.Expression
+    is_same_name_as_column: bool
```

### Comparing `databricks_labs_remorph-0.1.6/databricks/labs/remorph/snow/snowflake.py` & `databricks_labs_remorph-0.1.7/databricks/labs/remorph/snow/snowflake.py`

 * *Files 1% similar despite different names*

```diff
@@ -362,14 +362,15 @@
             "TO_VARIANT": local_expression.ToVariant.from_arg_list,
             "TRY_TO_BOOLEAN": lambda args: _parse_to_boolean(args, error=False),
             "UUID_STRING": local_expression.UUID.from_arg_list,
             "SYSDATE": exp.CurrentTimestamp.from_arg_list,
             "TRUNC": lambda args: local_expression.DateTrunc(unit=seq_get(args, 1), this=seq_get(args, 0)),
             "APPROX_PERCENTILE": exp.ApproxQuantile.from_arg_list,
             "NTH_VALUE": local_expression.NthValue.from_arg_list,
+            "MEDIAN": local_expression.Median.from_arg_list,
         }
 
         FUNCTION_PARSERS: ClassVar[dict] = {
             **Snowflake.Parser.FUNCTION_PARSERS,
             "LISTAGG": lambda self: self._parse_list_agg(),
         }
```

### Comparing `databricks_labs_remorph-0.1.6/databricks/labs/remorph/transpiler/execute.py` & `databricks_labs_remorph-0.1.7/databricks/labs/remorph/transpiler/execute.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,49 +1,56 @@
 import logging
 import os
 from pathlib import Path
 
-from databricks.sdk import WorkspaceClient
-
 from databricks.labs.remorph.config import MorphConfig
 from databricks.labs.remorph.helpers import db_sql
 from databricks.labs.remorph.helpers.execution_time import timeit
 from databricks.labs.remorph.helpers.file_utils import (
     dir_walk,
     is_sql_file,
     make_dir,
     remove_bom,
 )
 from databricks.labs.remorph.helpers.morph_status import MorphStatus, ValidationError
 from databricks.labs.remorph.helpers.validation import Validator
-from databricks.labs.remorph.snow import dialect_utils
-from databricks.labs.remorph.snow.sql_transpiler import SQLTranspiler
+from databricks.labs.remorph.snow import lca_utils
+from databricks.labs.remorph.snow.sql_transpiler import SqlglotEngine
+from databricks.sdk import WorkspaceClient
 
 # pylint: disable=unspecified-encoding
 
 logger = logging.getLogger(__name__)
 
 
-def process_file(config: MorphConfig, validator: Validator, input_file: str | Path, output_file: str | Path):
-    source = config.source
-    parse_error_list = []
+def process_file(
+    config: MorphConfig,
+    validator: Validator,
+    transpiler: SqlglotEngine,
+    input_file: str | Path,
+    output_file: str | Path,
+):
+    logger.info(f"started processing for the file ${input_file}")
     validate_error_list = []
     no_of_sqls = 0
 
     input_file = Path(input_file)
     output_file = Path(output_file)
 
     with input_file.open("r") as f:
         sql = remove_bom(f.read())
 
-    lca_error = dialect_utils.check_for_unsupported_lca(source, sql, str(input_file))
+    lca_error = lca_utils.check_for_unsupported_lca(config.source, sql, str(input_file))
+
     if lca_error:
         validate_error_list.append(lca_error)
-    transpiler = SQLTranspiler(source, parse_error_list)  # [TODO] move the object creation outside the loop
-    transpiled_sql = transpiler.transpile(sql, str(input_file))
+
+    write_dialect = config.get_write_dialect()
+
+    transpiled_sql, parse_error_list = transpiler.transpile(write_dialect, sql, str(input_file), [])
 
     with output_file.open("w") as w:
         for output in transpiled_sql:
             if output:
                 no_of_sqls = no_of_sqls + 1
                 if config.skip_validation:
                     w.write(output)
@@ -59,58 +66,69 @@
                     f"Check for unsupported operations related to STREAM, TASK, SESSION etc."
                 )
                 logger.warning(warning_message)
 
     return no_of_sqls, parse_error_list, validate_error_list
 
 
-def process_directory(config: MorphConfig, validator: Validator, root: str | Path, base_root: str, files: list[str]):
+def process_directory(
+    config: MorphConfig,
+    validator: Validator,
+    transpiler: SqlglotEngine,
+    root: str | Path,
+    base_root: str,
+    files: list[str],
+):
     output_folder = config.output_folder
     parse_error_list = []
     validate_error_list = []
     counter = 0
 
     root = Path(root)
 
     for file in files:
-        logger.debug(f"Processing file :{file}")
+        logger.info(f"Processing file :{file}")
         if is_sql_file(file):
             if output_folder in {None, "None"}:
                 output_folder_base = root / "transpiled"
             else:
                 output_folder_base = f'{output_folder.rstrip("/")}/{base_root}'
 
             output_file_name = Path(output_folder_base) / Path(file).name
             make_dir(output_folder_base)
 
-            no_of_sqls, parse_error, validation_error = process_file(config, validator, file, output_file_name)
+            no_of_sqls, parse_error, validation_error = process_file(
+                config, validator, transpiler, file, output_file_name
+            )
             counter = counter + no_of_sqls
             parse_error_list.extend(parse_error)
             validate_error_list.extend(validation_error)
         else:
             # Only SQL files are processed with extension .sql or .ddl
             pass
 
     return counter, parse_error_list, validate_error_list
 
 
-def process_recursive_dirs(config: MorphConfig, validator: Validator):
+def process_recursive_dirs(config: MorphConfig, validator: Validator, transpiler: SqlglotEngine):
     input_sql = Path(config.input_sql)
     parse_error_list = []
     validate_error_list = []
 
     file_list = []
     counter = 0
     for root, _, files in dir_walk(input_sql):
         base_root = str(root).replace(str(input_sql), "")
         folder = str(input_sql.resolve().joinpath(base_root))
         msg = f"Processing for sqls under this folder: {folder}"
         logger.info(msg)
         file_list.extend(files)
-        no_of_sqls, parse_error, validation_error = process_directory(config, validator, root, base_root, files)
+        no_of_sqls, parse_error, validation_error = process_directory(
+            config, validator, transpiler, root, base_root, files
+        )
         counter = counter + no_of_sqls
         parse_error_list.extend(parse_error)
         validate_error_list.extend(validation_error)
 
     error_log = parse_error_list + validate_error_list
 
     return MorphStatus(file_list, counter, len(parse_error_list), len(validate_error_list), error_log)
@@ -121,17 +139,19 @@
     """
     Transpiles the SQL queries from one dialect to another.
 
     :param config: The configuration for the morph operation.
     :param workspace_client: The WorkspaceClient object.
     """
     input_sql = Path(config.input_sql)
-    skip_validation = config.skip_validation
     status = []
     result = MorphStatus([], 0, 0, 0, [])
+
+    read_dialect = config.get_read_dialect()
+    transpiler = SqlglotEngine(read_dialect)
     validator = None
     if not config.skip_validation:
         validator = Validator(db_sql.get_sql_backend(workspace_client, config))
 
     if input_sql.is_file():
         if is_sql_file(input_sql):
             msg = f"Processing for sqls under this file: {input_sql}"
@@ -139,43 +159,42 @@
             if config.output_folder in {None, "None"}:
                 output_folder = input_sql.parent / "transpiled"
             else:
                 output_folder = Path(config.output_folder.rstrip("/"))
 
             make_dir(output_folder)
             output_file = output_folder / input_sql.name
-            no_of_sqls, parse_error, validation_error = process_file(config, validator, input_sql, output_file)
+            no_of_sqls, parse_error, validation_error = process_file(
+                config, validator, transpiler, input_sql, output_file
+            )
             error_log = parse_error + validation_error
             result = MorphStatus([str(input_sql)], no_of_sqls, len(parse_error), len(validation_error), error_log)
         else:
             msg = f"{input_sql} is not a SQL file."
             logger.warning(msg)
     elif input_sql.is_dir():
-        result = process_recursive_dirs(config, validator)
+        result = process_recursive_dirs(config, validator, transpiler)
     else:
         msg = f"{input_sql} does not exist."
         logger.error(msg)
         raise FileNotFoundError(msg)
 
-    parse_error_count = result.parse_error_count
-    validate_error_count = result.validate_error_count
-
-    error_list_count = parse_error_count + validate_error_count
-    if not skip_validation:
-        logger.info(f"No of Sql Failed while Validating: {validate_error_count}")
+    error_list_count = result.parse_error_count + result.validate_error_count
+    if not config.skip_validation:
+        logger.info(f"No of Sql Failed while Validating: {result.validate_error_count}")
 
     error_log_file = "None"
     if error_list_count > 0:
         error_log_file = Path.cwd() / f"err_{os.getpid()}.lst"
         with error_log_file.open("a") as e:
             e.writelines(f"{err}\n" for err in result.error_log_list)
 
     status.append(
         {
             "total_files_processed": len(result.file_list),
             "total_queries_processed": result.no_of_queries,
-            "no_of_sql_failed_while_parsing": parse_error_count,
-            "no_of_sql_failed_while_validating": validate_error_count,
+            "no_of_sql_failed_while_parsing": result.parse_error_count,
+            "no_of_sql_failed_while_validating": result.validate_error_count,
             "error_log_file": str(error_log_file),
         }
     )
     return status
```

### Comparing `databricks_labs_remorph-0.1.6/LICENSE` & `databricks_labs_remorph-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `databricks_labs_remorph-0.1.6/README.md` & `databricks_labs_remorph-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `databricks_labs_remorph-0.1.6/pyproject.toml` & `databricks_labs_remorph-0.1.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
   "Development Status :: 3 - Alpha",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
 ]
 dependencies = [
   "databricks-sdk>=0.18.0",
-  "sqlglot==23.0.1",
+  "sqlglot==23.13.7",
   "databricks-labs-blueprint[yaml]>=0.2.3",
   "databricks-labs-lsql>=0.2.3",
 ]
 
 [project.urls]
 Documentation = "https://github.com/databrickslabs/remorph"
 Issues = "https://github.com/databrickslabs/remorph/issues"
@@ -55,31 +55,32 @@
 
 [tool.hatch.envs.default.scripts]
 test        = "pytest --cov src --cov-report=xml tests/unit"
 coverage    = "pytest --cov src tests/unit --cov-report=html"
 integration = "pytest --cov src tests/integration --durations 20"
 fmt         = ["isort .",
                "black .",
-               "ruff  . --fix",
+               "ruff  check . --fix",
                "pylint --output-format=colorized -j 0 src tests"]
 verify      = ["black --check .",
                "isort . --check-only",
-               "ruff .",
+               "ruff check .",
                "pylint --output-format=colorized -j 0 src tests"]
 
 [tool.hatch.envs.sqlglot-latest]
 detached = true
 python="3.10"
 dependencies = [
   "sqlglot",
 ]
 
 [tool.isort]
 skip_glob = ["notebooks/*.py"]
 profile = "black"
+known_first_party = ["databricks"]
 
 [tool.pytest.ini_options]
 addopts = "-s -p no:warnings -vv --cache-clear"
 cache_dir = ".venv/pytest-cache"
 
 [tool.black]
 target-version = ["py310"]
```

### Comparing `databricks_labs_remorph-0.1.6/PKG-INFO` & `databricks_labs_remorph-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: databricks-labs-remorph
-Version: 0.1.6
+Version: 0.1.7
 Summary: SQL code converter and data reconcilation tool for accelerating data onboarding to Databricks from EDW, CDW and other ETL sources.
 Project-URL: Documentation, https://github.com/databrickslabs/remorph
 Project-URL: Issues, https://github.com/databrickslabs/remorph/issues
 Project-URL: Source, https://github.com/databrickslabs/remorph
 License-File: LICENSE
 License-File: NOTICE
 Keywords: Databricks
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.10
 Requires-Dist: databricks-labs-blueprint[yaml]>=0.2.3
 Requires-Dist: databricks-labs-lsql>=0.2.3
 Requires-Dist: databricks-sdk>=0.18.0
-Requires-Dist: sqlglot==23.0.1
+Requires-Dist: sqlglot==23.13.7
 Description-Content-Type: text/markdown
 
 Databricks Labs Remorph
 ---
 ![Databricks Labs Remorph](docs/remorph-logo.svg)
 
 [![lines of code](https://tokei.rs/b1/github/databrickslabs/remorph)]([https://codecov.io/github/databrickslabs/remorph](https://github.com/databrickslabs/remorph))
```

