# Comparing `tmp/meltanolabs_target_postgres-0.0.8.tar.gz` & `tmp/meltanolabs_target_postgres-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meltanolabs_target_postgres-0.0.8.tar", max compression
+gzip compressed data, was "meltanolabs_target_postgres-0.0.9.tar", max compression
```

## Comparing `meltanolabs_target_postgres-0.0.8.tar` & `meltanolabs_target_postgres-0.0.9.tar`

### file list

```diff
@@ -1,55 +1,55 @@
--rw-r--r--   0        0        0     1068 2023-09-08 20:06:21.982251 meltanolabs_target_postgres-0.0.8/LICENSE
--rw-r--r--   0        0        0     9678 2023-09-08 20:06:21.982251 meltanolabs_target_postgres-0.0.8/README.md
--rw-r--r--   0        0        0     1846 2023-09-08 20:06:49.814704 meltanolabs_target_postgres-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     1911 2023-09-08 20:06:21.986251 meltanolabs_target_postgres-0.0.8/target_postgres/.gitignore
--rw-r--r--   0        0        0       21 2023-09-08 20:06:21.986251 meltanolabs_target_postgres-0.0.8/target_postgres/__init__.py
--rw-r--r--   0        0        0    26914 2023-09-08 20:06:21.986251 meltanolabs_target_postgres-0.0.8/target_postgres/connector.py
--rw-r--r--   0        0        0    14087 2023-09-08 20:06:21.986251 meltanolabs_target_postgres-0.0.8/target_postgres/sinks.py
--rw-r--r--   0        0        0    13269 2023-09-08 20:06:21.986251 meltanolabs_target_postgres-0.0.8/target_postgres/target.py
--rw-r--r--   0        0        0       38 2023-09-08 20:06:21.986251 meltanolabs_target_postgres-0.0.8/target_postgres/tests/__init__.py
--rw-r--r--   0        0        0      668 2023-09-08 20:06:21.986251 meltanolabs_target_postgres-0.0.8/target_postgres/tests/data_files/array_data.singer
--rw-r--r--   0        0        0      394 2023-09-08 20:06:21.986251 meltanolabs_target_postgres-0.0.8/target_postgres/tests/data_files/camelcase.singer
--rw-r--r--   0        0        0     1862 2023-09-08 20:06:21.986251 meltanolabs_target_postgres-0.0.8/target_postgres/tests/data_files/camelcase_complex_schema.singer
--rw-r--r--   0        0        0     6910 2023-09-08 20:06:21.986251 meltanolabs_target_postgres-0.0.8/target_postgres/tests/data_files/commits.singer
--rw-r--r--   0        0        0      722 2023-09-08 20:06:21.986251 meltanolabs_target_postgres-0.0.8/target_postgres/tests/data_files/duplicate_records.singer
--rw-r--r--   0        0        0     4275 2023-09-08 20:06:21.986251 meltanolabs_target_postgres-0.0.8/target_postgres/tests/data_files/encoded_strings.singer
--rw-r--r--   0        0        0      104 2023-09-08 20:06:21.986251 meltanolabs_target_postgres-0.0.8/target_postgres/tests/data_files/invalid_schema.singer
--rw-r--r--   0        0        0      362 2023-09-08 20:06:21.986251 meltanolabs_target_postgres-0.0.8/target_postgres/tests/data_files/large_int.singer
--rw-r--r--   0        0        0      607 2023-09-08 20:06:21.986251 meltanolabs_target_postgres-0.0.8/target_postgres/tests/data_files/missing_value.singer
--rw-r--r--   0        0        0     2129 2023-09-08 20:06:21.986251 meltanolabs_target_postgres-0.0.8/target_postgres/tests/data_files/multiple_state_messages.singer
--rw-r--r--   0        0        0      407 2023-09-08 20:06:21.986251 meltanolabs_target_postgres-0.0.8/target_postgres/tests/data_files/new_array_column.singer
--rw-r--r--   0        0        0      641 2023-09-08 20:06:21.986251 meltanolabs_target_postgres-0.0.8/target_postgres/tests/data_files/optional_attributes.singer
--rw-r--r--   0        0        0      378 2023-09-08 20:06:21.986251 meltanolabs_target_postgres-0.0.8/target_postgres/tests/data_files/record_before_schema.singer
--rw-r--r--   0        0        0      288 2023-09-08 20:06:21.986251 meltanolabs_target_postgres-0.0.8/target_postgres/tests/data_files/record_missing_key_property.singer
--rw-r--r--   0        0        0      318 2023-09-08 20:06:21.986251 meltanolabs_target_postgres-0.0.8/target_postgres/tests/data_files/record_missing_required_property.singer
--rw-r--r--   0        0        0    51890 2023-09-08 20:06:21.986251 meltanolabs_target_postgres-0.0.8/target_postgres/tests/data_files/reserved_keywords.singer
--rw-r--r--   0        0        0      892 2023-09-08 20:06:21.986251 meltanolabs_target_postgres-0.0.8/target_postgres/tests/data_files/schema_no_properties.singer
--rw-r--r--   0        0        0     2197 2023-09-08 20:06:21.986251 meltanolabs_target_postgres-0.0.8/target_postgres/tests/data_files/schema_updates.singer
--rw-r--r--   0        0        0      554 2023-09-08 20:06:21.986251 meltanolabs_target_postgres-0.0.8/target_postgres/tests/data_files/special_chars_in_attributes.singer
--rw-r--r--   0        0        0  1859439 2023-09-08 20:06:21.990251 meltanolabs_target_postgres-0.0.8/target_postgres/tests/data_files/tap_aapl.singer
--rw-r--r--   0        0        0    97655 2023-09-08 20:06:21.990251 meltanolabs_target_postgres-0.0.8/target_postgres/tests/data_files/tap_countries.singer
--rw-r--r--   0        0        0     1851 2023-09-08 20:06:21.990251 meltanolabs_target_postgres-0.0.8/target_postgres/tests/data_files/test_activate_version_deletes_data_properly.singer
--rw-r--r--   0        0        0      357 2023-09-08 20:06:21.990251 meltanolabs_target_postgres-0.0.8/target_postgres/tests/data_files/test_activate_version_deletes_data_properly_2.singer
--rw-r--r--   0        0        0     1681 2023-09-08 20:06:21.990251 meltanolabs_target_postgres-0.0.8/target_postgres/tests/data_files/test_activate_version_hard.singer
--rw-r--r--   0        0        0     1681 2023-09-08 20:06:21.990251 meltanolabs_target_postgres-0.0.8/target_postgres/tests/data_files/test_activate_version_soft.singer
--rw-r--r--   0        0        0     1491 2023-09-08 20:06:21.990251 meltanolabs_target_postgres-0.0.8/target_postgres/tests/data_files/test_activate_version_uppercase_stream_name.singer
--rw-r--r--   0        0        0      450 2023-09-08 20:06:21.990251 meltanolabs_target_postgres-0.0.8/target_postgres/tests/data_files/test_no_pk.singer
--rw-r--r--   0        0        0      611 2023-09-08 20:06:21.994251 meltanolabs_target_postgres-0.0.8/target_postgres/tests/data_files/test_no_pk_append.singer
--rw-r--r--   0        0        0     6573 2023-09-08 20:06:21.994251 meltanolabs_target_postgres-0.0.8/target_postgres/tests/data_files/test_no_type.singer
--rw-r--r--   0        0        0      915 2023-09-08 20:06:21.994251 meltanolabs_target_postgres-0.0.8/target_postgres/tests/data_files/uppercase_stream_name_with_column_alter.singer
--rw-r--r--   0        0        0     1992 2023-09-08 20:06:21.994251 meltanolabs_target_postgres-0.0.8/target_postgres/tests/data_files/user_location_data.singer
--rw-r--r--   0        0        0     2323 2023-09-08 20:06:21.994251 meltanolabs_target_postgres-0.0.8/target_postgres/tests/data_files/user_location_upsert_data.singer
--rw-r--r--   0        0        0       15 2023-09-08 20:06:21.994251 meltanolabs_target_postgres-0.0.8/target_postgres/tests/samples/.gitignore
--rw-r--r--   0        0        0      453 2023-09-08 20:06:21.994251 meltanolabs_target_postgres-0.0.8/target_postgres/tests/samples/README.md
--rw-r--r--   0        0        0       15 2023-09-08 20:06:21.994251 meltanolabs_target_postgres-0.0.8/target_postgres/tests/samples/__init__.py
--rw-r--r--   0        0        0   763998 2023-09-08 20:06:21.994251 meltanolabs_target_postgres-0.0.8/target_postgres/tests/samples/aapl/AAPL.json
--rw-r--r--   0        0        0      352 2023-09-08 20:06:21.994251 meltanolabs_target_postgres-0.0.8/target_postgres/tests/samples/aapl/README.md
--rw-r--r--   0        0        0      131 2023-09-08 20:06:21.994251 meltanolabs_target_postgres-0.0.8/target_postgres/tests/samples/aapl/__main__.py
--rw-r--r--   0        0        0      654 2023-09-08 20:06:21.994251 meltanolabs_target_postgres-0.0.8/target_postgres/tests/samples/aapl/aapl.py
--rw-r--r--   0        0        0  1492450 2023-09-08 20:06:21.998251 meltanolabs_target_postgres-0.0.8/target_postgres/tests/samples/aapl/fundamentals.json
--rw-r--r--   0        0        0       28 2023-09-08 20:06:21.998251 meltanolabs_target_postgres-0.0.8/target_postgres/tests/samples/sample_tap_countries/__init__.py
--rw-r--r--   0        0        0     2218 2023-09-08 20:06:21.998251 meltanolabs_target_postgres-0.0.8/target_postgres/tests/samples/sample_tap_countries/countries_streams.py
--rw-r--r--   0        0        0      817 2023-09-08 20:06:21.998251 meltanolabs_target_postgres-0.0.8/target_postgres/tests/samples/sample_tap_countries/countries_tap.py
--rw-r--r--   0        0        0      146 2023-09-08 20:06:21.998251 meltanolabs_target_postgres-0.0.8/target_postgres/tests/samples/sample_tap_countries/schemas/continents.json
--rw-r--r--   0        0        0    29580 2023-09-08 20:06:21.998251 meltanolabs_target_postgres-0.0.8/target_postgres/tests/test_standard_target.py
--rw-r--r--   0        0        0    10947 1970-01-01 00:00:00.000000 meltanolabs_target_postgres-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-10-20 19:12:23.273842 meltanolabs_target_postgres-0.0.9/LICENSE
+-rw-r--r--   0        0        0     9944 2023-10-20 19:12:23.273842 meltanolabs_target_postgres-0.0.9/README.md
+-rw-r--r--   0        0        0     1762 2023-10-20 19:12:45.641371 meltanolabs_target_postgres-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1911 2023-10-20 19:12:23.273842 meltanolabs_target_postgres-0.0.9/target_postgres/.gitignore
+-rw-r--r--   0        0        0       21 2023-10-20 19:12:23.273842 meltanolabs_target_postgres-0.0.9/target_postgres/__init__.py
+-rw-r--r--   0        0        0    27494 2023-10-20 19:12:23.273842 meltanolabs_target_postgres-0.0.9/target_postgres/connector.py
+-rw-r--r--   0        0        0    14251 2023-10-20 19:12:23.273842 meltanolabs_target_postgres-0.0.9/target_postgres/sinks.py
+-rw-r--r--   0        0        0    12628 2023-10-20 19:12:23.273842 meltanolabs_target_postgres-0.0.9/target_postgres/target.py
+-rw-r--r--   0        0        0       38 2023-10-20 19:12:23.273842 meltanolabs_target_postgres-0.0.9/target_postgres/tests/__init__.py
+-rw-r--r--   0        0        0      668 2023-10-20 19:12:23.273842 meltanolabs_target_postgres-0.0.9/target_postgres/tests/data_files/array_data.singer
+-rw-r--r--   0        0        0      394 2023-10-20 19:12:23.273842 meltanolabs_target_postgres-0.0.9/target_postgres/tests/data_files/camelcase.singer
+-rw-r--r--   0        0        0     1862 2023-10-20 19:12:23.273842 meltanolabs_target_postgres-0.0.9/target_postgres/tests/data_files/camelcase_complex_schema.singer
+-rw-r--r--   0        0        0     6910 2023-10-20 19:12:23.273842 meltanolabs_target_postgres-0.0.9/target_postgres/tests/data_files/commits.singer
+-rw-r--r--   0        0        0      722 2023-10-20 19:12:23.273842 meltanolabs_target_postgres-0.0.9/target_postgres/tests/data_files/duplicate_records.singer
+-rw-r--r--   0        0        0     4275 2023-10-20 19:12:23.273842 meltanolabs_target_postgres-0.0.9/target_postgres/tests/data_files/encoded_strings.singer
+-rw-r--r--   0        0        0      104 2023-10-20 19:12:23.273842 meltanolabs_target_postgres-0.0.9/target_postgres/tests/data_files/invalid_schema.singer
+-rw-r--r--   0        0        0      362 2023-10-20 19:12:23.273842 meltanolabs_target_postgres-0.0.9/target_postgres/tests/data_files/large_int.singer
+-rw-r--r--   0        0        0      607 2023-10-20 19:12:23.273842 meltanolabs_target_postgres-0.0.9/target_postgres/tests/data_files/missing_value.singer
+-rw-r--r--   0        0        0     2129 2023-10-20 19:12:23.273842 meltanolabs_target_postgres-0.0.9/target_postgres/tests/data_files/multiple_state_messages.singer
+-rw-r--r--   0        0        0      407 2023-10-20 19:12:23.273842 meltanolabs_target_postgres-0.0.9/target_postgres/tests/data_files/new_array_column.singer
+-rw-r--r--   0        0        0      641 2023-10-20 19:12:23.273842 meltanolabs_target_postgres-0.0.9/target_postgres/tests/data_files/optional_attributes.singer
+-rw-r--r--   0        0        0      378 2023-10-20 19:12:23.273842 meltanolabs_target_postgres-0.0.9/target_postgres/tests/data_files/record_before_schema.singer
+-rw-r--r--   0        0        0      288 2023-10-20 19:12:23.273842 meltanolabs_target_postgres-0.0.9/target_postgres/tests/data_files/record_missing_key_property.singer
+-rw-r--r--   0        0        0      318 2023-10-20 19:12:23.273842 meltanolabs_target_postgres-0.0.9/target_postgres/tests/data_files/record_missing_required_property.singer
+-rw-r--r--   0        0        0    51890 2023-10-20 19:12:23.273842 meltanolabs_target_postgres-0.0.9/target_postgres/tests/data_files/reserved_keywords.singer
+-rw-r--r--   0        0        0      892 2023-10-20 19:12:23.273842 meltanolabs_target_postgres-0.0.9/target_postgres/tests/data_files/schema_no_properties.singer
+-rw-r--r--   0        0        0     2197 2023-10-20 19:12:23.273842 meltanolabs_target_postgres-0.0.9/target_postgres/tests/data_files/schema_updates.singer
+-rw-r--r--   0        0        0      554 2023-10-20 19:12:23.273842 meltanolabs_target_postgres-0.0.9/target_postgres/tests/data_files/special_chars_in_attributes.singer
+-rw-r--r--   0        0        0  1859439 2023-10-20 19:12:23.281842 meltanolabs_target_postgres-0.0.9/target_postgres/tests/data_files/tap_aapl.singer
+-rw-r--r--   0        0        0    97655 2023-10-20 19:12:23.281842 meltanolabs_target_postgres-0.0.9/target_postgres/tests/data_files/tap_countries.singer
+-rw-r--r--   0        0        0     1851 2023-10-20 19:12:23.281842 meltanolabs_target_postgres-0.0.9/target_postgres/tests/data_files/test_activate_version_deletes_data_properly.singer
+-rw-r--r--   0        0        0      357 2023-10-20 19:12:23.281842 meltanolabs_target_postgres-0.0.9/target_postgres/tests/data_files/test_activate_version_deletes_data_properly_2.singer
+-rw-r--r--   0        0        0     1681 2023-10-20 19:12:23.281842 meltanolabs_target_postgres-0.0.9/target_postgres/tests/data_files/test_activate_version_hard.singer
+-rw-r--r--   0        0        0     1681 2023-10-20 19:12:23.281842 meltanolabs_target_postgres-0.0.9/target_postgres/tests/data_files/test_activate_version_soft.singer
+-rw-r--r--   0        0        0     1491 2023-10-20 19:12:23.281842 meltanolabs_target_postgres-0.0.9/target_postgres/tests/data_files/test_activate_version_uppercase_stream_name.singer
+-rw-r--r--   0        0        0      450 2023-10-20 19:12:23.281842 meltanolabs_target_postgres-0.0.9/target_postgres/tests/data_files/test_no_pk.singer
+-rw-r--r--   0        0        0      611 2023-10-20 19:12:23.281842 meltanolabs_target_postgres-0.0.9/target_postgres/tests/data_files/test_no_pk_append.singer
+-rw-r--r--   0        0        0     6573 2023-10-20 19:12:23.281842 meltanolabs_target_postgres-0.0.9/target_postgres/tests/data_files/test_no_type.singer
+-rw-r--r--   0        0        0      915 2023-10-20 19:12:23.281842 meltanolabs_target_postgres-0.0.9/target_postgres/tests/data_files/uppercase_stream_name_with_column_alter.singer
+-rw-r--r--   0        0        0     1992 2023-10-20 19:12:23.281842 meltanolabs_target_postgres-0.0.9/target_postgres/tests/data_files/user_location_data.singer
+-rw-r--r--   0        0        0     2323 2023-10-20 19:12:23.281842 meltanolabs_target_postgres-0.0.9/target_postgres/tests/data_files/user_location_upsert_data.singer
+-rw-r--r--   0        0        0       15 2023-10-20 19:12:23.281842 meltanolabs_target_postgres-0.0.9/target_postgres/tests/samples/.gitignore
+-rw-r--r--   0        0        0      453 2023-10-20 19:12:23.281842 meltanolabs_target_postgres-0.0.9/target_postgres/tests/samples/README.md
+-rw-r--r--   0        0        0       15 2023-10-20 19:12:23.281842 meltanolabs_target_postgres-0.0.9/target_postgres/tests/samples/__init__.py
+-rw-r--r--   0        0        0   763998 2023-10-20 19:12:23.285843 meltanolabs_target_postgres-0.0.9/target_postgres/tests/samples/aapl/AAPL.json
+-rw-r--r--   0        0        0      352 2023-10-20 19:12:23.285843 meltanolabs_target_postgres-0.0.9/target_postgres/tests/samples/aapl/README.md
+-rw-r--r--   0        0        0      131 2023-10-20 19:12:23.285843 meltanolabs_target_postgres-0.0.9/target_postgres/tests/samples/aapl/__main__.py
+-rw-r--r--   0        0        0      654 2023-10-20 19:12:23.285843 meltanolabs_target_postgres-0.0.9/target_postgres/tests/samples/aapl/aapl.py
+-rw-r--r--   0        0        0  1492450 2023-10-20 19:12:23.289843 meltanolabs_target_postgres-0.0.9/target_postgres/tests/samples/aapl/fundamentals.json
+-rw-r--r--   0        0        0       28 2023-10-20 19:12:23.289843 meltanolabs_target_postgres-0.0.9/target_postgres/tests/samples/sample_tap_countries/__init__.py
+-rw-r--r--   0        0        0     2218 2023-10-20 19:12:23.289843 meltanolabs_target_postgres-0.0.9/target_postgres/tests/samples/sample_tap_countries/countries_streams.py
+-rw-r--r--   0        0        0      817 2023-10-20 19:12:23.289843 meltanolabs_target_postgres-0.0.9/target_postgres/tests/samples/sample_tap_countries/countries_tap.py
+-rw-r--r--   0        0        0      146 2023-10-20 19:12:23.289843 meltanolabs_target_postgres-0.0.9/target_postgres/tests/samples/sample_tap_countries/schemas/continents.json
+-rw-r--r--   0        0        0    30627 2023-10-20 19:12:23.289843 meltanolabs_target_postgres-0.0.9/target_postgres/tests/test_standard_target.py
+-rw-r--r--   0        0        0    11221 1970-01-01 00:00:00.000000 meltanolabs_target_postgres-0.0.9/PKG-INFO
```

### Comparing `meltanolabs_target_postgres-0.0.8/LICENSE` & `meltanolabs_target_postgres-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `meltanolabs_target_postgres-0.0.8/README.md` & `meltanolabs_target_postgres-0.0.9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 # `target-postgres`
 
+![PyPI - Version](https://img.shields.io/pypi/v/meltanolabs-target-postgres)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/meltanolabs-target-postgres)
+![PyPI - License](https://img.shields.io/pypi/l/meltanolabs-target-postgres)
+![Test target-postgres](https://github.com/meltanolabs/target-postgres/actions/workflows/ci_workflow.yml/badge.svg)
+
 Target for Postgres.
 
 Built with the [Meltano SDK](https://sdk.meltano.com) for Singer Taps and Targets.
 
 ## Capabilities
 
 * `about`
@@ -42,18 +47,16 @@
 | flattening_enabled           | False    | None    | 'True' to enable schema flattening and automatically expand nested properties. |
 | flattening_max_depth         | False    | None    | The max depth to flatten schemas. |
 
 A full list of supported settings and capabilities is available by running: `target-postgres --about`
 
 ## Installation
 
-- [ ] `Developer TODO:` Come back to this re [#5](https://github.com/MeltanoLabs/target-postgres/issues/5)
-
 ```bash
-pipx install -e .
+pipx install meltanolabs-target-postgres
 ```
 
 ## Configuration
 
 ### An Explanation of Various SSL Configuration Options
 
 There are two distinct processes which both fall under the banner of SSL. One process occurs when the client wishes to ensure the identity of the server, and is the more common reason that SSL is used. Another is when the server wishes to ensure the identity of the client, for authentication/authorization purposes.
```

### Comparing `meltanolabs_target_postgres-0.0.8/pyproject.toml` & `meltanolabs_target_postgres-0.0.9/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "meltanolabs-target-postgres"
-version = "0.0.8"
+version = "0.0.9"
 description = "`target-postgres` is a Singer target for Postgres, built with the Meltano SDK for Singer Targets."
 authors = ["Meltano Team and Contributors <hello@meltano.com>"]
 maintainers = ["Meltano Team and Contributors <hello@meltano.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://meltano.com"
 repository = "https://github.com/meltanolabs/target-postgres"
@@ -29,27 +29,22 @@
 packages = [
     { include = "target_postgres" }
 ]
 
 [tool.poetry.dependencies]
 python = "<3.12,>=3.7.1"
 requests = "^2.25.1"
-singer-sdk = ">=0.28,<0.32"
-psycopg2-binary = "2.9.7"
-sqlalchemy = "<2"
+singer-sdk = ">=0.28,<0.34"
+psycopg2-binary = "2.9.9"
+sqlalchemy = ">=2.0,<3.0"
 sshtunnel = "0.4.0"
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.dev.dependencies]
 pytest = "^7.4.2"
-tox = "^3.24.4"
-flake8 = "^5.0.4"
-flake8-docstrings = "^1.7.0"
-black = "23.3.0"
 mypy = "^1.0"
-isort = "^5.11.5"
 remote-pdb="2.1.0"
 
 [tool.isort]
 profile = "black"
 multi_line_output = 3 # Vertical Hanging Indent
 src_paths = "target_postgres"
```

### Comparing `meltanolabs_target_postgres-0.0.8/target_postgres/.gitignore` & `meltanolabs_target_postgres-0.0.9/target_postgres/.gitignore`

 * *Files identical despite different names*

### Comparing `meltanolabs_target_postgres-0.0.8/target_postgres/connector.py` & `meltanolabs_target_postgres-0.0.9/target_postgres/connector.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 from sqlalchemy.engine.url import make_url
 from sqlalchemy.types import (
     BOOLEAN,
     DATE,
     DATETIME,
     DECIMAL,
     INTEGER,
+    TEXT,
     TIME,
     TIMESTAMP,
     VARCHAR,
     TypeDecorator,
 )
 from sshtunnel import SSHTunnelForwarder
 
@@ -88,32 +89,36 @@
     ) -> sqlalchemy.Table:
         """Adapt target table to provided schema if possible.
 
         Args:
             full_table_name: the target table name.
             schema: the JSON Schema for the table.
             primary_keys: list of key properties.
+            connection: the database connection.
             partition_keys: list of partition keys.
             as_temp_table: True to create a temp table.
+
+        Returns:
+            The table object.
         """
         _, schema_name, table_name = self.parse_full_table_name(full_table_name)
-        meta = sqlalchemy.MetaData(bind=connection, schema=schema_name)
+        meta = sqlalchemy.MetaData(schema=schema_name)
         table: sqlalchemy.Table = None
         if not self.table_exists(full_table_name=full_table_name):
             table = self.create_empty_table(
                 table_name=table_name,
                 meta=meta,
                 schema=schema,
                 primary_keys=primary_keys,
                 partition_keys=partition_keys,
                 as_temp_table=as_temp_table,
                 connection=connection,
             )
             return table
-        meta.reflect(only=[table_name])
+        meta.reflect(connection, only=[table_name])
         table = meta.tables[
             full_table_name
         ]  # So we don't mess up the casing of the Table reference
         for property_name, property_def in schema["properties"].items():
             self.prepare_column(
                 schema_name=schema_name,
                 table=table,
@@ -131,19 +136,23 @@
         connection: sqlalchemy.engine.Connection,
         as_temp_table: bool = False,
     ) -> sqlalchemy.Table:
         """Copy table structure.
 
         Args:
             full_table_name: the target table name potentially including schema
-            fromtable: the  source table
+            from_table: the  source table
+            connection: the database connection.
             as_temp_table: True to create a temp table.
+
+        Returns:
+            The new table object.
         """
         _, schema_name, table_name = self.parse_full_table_name(full_table_name)
-        meta = sqlalchemy.MetaData(bind=connection, schema=schema_name)
+        meta = sqlalchemy.MetaData(schema=schema_name)
         new_table: sqlalchemy.Table = None
         columns = []
         if self.table_exists(full_table_name=full_table_name):
             raise RuntimeError("Table already exists")
         for column in from_table.columns:
             columns.append(column._copy())
         if as_temp_table:
@@ -182,16 +191,15 @@
             )
         if temp_table is True:
             new_table = sqlalchemy.Table(
                 new_table_name, metadata, *new_columns, prefixes=["TEMPORARY"]
             )
         else:
             new_table = sqlalchemy.Table(new_table_name, metadata, *new_columns)
-        with self._connect() as connection:
-            new_table.create(bind=connection)
+        new_table.create(bind=connection)
         return new_table
 
     @staticmethod
     def to_sql_type(jsonschema_type: dict) -> sqlalchemy.types.TypeEngine:
         """Return a JSON Schema representation of the provided type.
 
         By default will call `typing.to_sql_type()`.
@@ -257,30 +265,33 @@
             return BIGINT()
         if "object" in jsonschema_type["type"]:
             return JSONB()
         if "array" in jsonschema_type["type"]:
             return ARRAY(JSONB())
         if jsonschema_type.get("format") == "date-time":
             return TIMESTAMP()
-        return th.to_sql_type(jsonschema_type)
+        individual_type = th.to_sql_type(jsonschema_type)
+        if isinstance(individual_type, VARCHAR):
+            return TEXT()
+        return individual_type
 
     @staticmethod
     def pick_best_sql_type(sql_type_array: list):
         """Select the best SQL type from an array of instances of SQL type classes.
 
         Args:
             sql_type_array: The array of instances of SQL type classes.
 
         Returns:
             An instance of the best SQL type class based on defined precedence order.
         """
         precedence_order = [
             ARRAY,
             JSONB,
-            VARCHAR,
+            TEXT,
             TIMESTAMP,
             DATETIME,
             DATE,
             TIME,
             DECIMAL,
             BIGINT,
             INTEGER,
@@ -288,15 +299,15 @@
             NOTYPE,
         ]
 
         for sql_type in precedence_order:
             for obj in sql_type_array:
                 if isinstance(obj, sql_type):
                     return obj
-        return VARCHAR()
+        return TEXT()
 
     def create_empty_table(
         self,
         table_name: str,
         meta: sqlalchemy.MetaData,
         schema: dict,
         connection: sqlalchemy.engine.Connection,
@@ -354,20 +365,21 @@
         column_name: str,
         sql_type: sqlalchemy.types.TypeEngine,
         connection: sqlalchemy.engine.Connection,
     ) -> None:
         """Adapt target table to provided schema if possible.
 
         Args:
-            full_table_name: the target table name.
+            schema_name: the schema name.
+            table: the target table.
             column_name: the target column name.
             sql_type: the SQLAlchemy type.
-            schema_name: the schema name.
+            connection: the database connection.
         """
-        if not self.column_exists(table.fullname, column_name):
+        if not self.column_exists(table.fullname, column_name, connection=connection):
             self._create_empty_column(
                 # We should migrate every function to use sqlalchemy.Table
                 # instead of having to know what the function wants
                 table_name=table.name,
                 column_name=column_name,
                 sql_type=sql_type,
                 schema_name=schema_name,
@@ -464,14 +476,15 @@
         Raises:
             NotImplementedError: if altering columns is not supported.
         """
         current_type: sqlalchemy.types.TypeEngine = self._get_column_type(
             schema_name=schema_name,
             table_name=table_name,
             column_name=column_name,
+            connection=connection,
         )
 
         # remove collation if present and save it
         current_type_collation = self.remove_collation(current_type)
 
         # Check if the existing column type and the sql type are the same
         if str(sql_type) == str(current_type):
@@ -674,14 +687,15 @@
         exit(1)  # Calling this to be sure atexit is called, so clean_up gets called
 
     def _get_column_type(
         self,
         schema_name: str,
         table_name: str,
         column_name: str,
+        connection: sqlalchemy.engine.Connection,
     ) -> sqlalchemy.types.TypeEngine:
         """Get the SQL type of the declared column.
 
         Args:
             full_table_name: The name of the table.
             column_name: The name of the column.
 
@@ -691,78 +705,85 @@
         Raises:
             KeyError: If the provided column name does not exist.
         """
         try:
             column = self.get_table_columns(
                 schema_name=schema_name,
                 table_name=table_name,
+                connection=connection,
             )[column_name]
         except KeyError as ex:
             msg = (
                 f"Column `{column_name}` does not exist in table"
                 "`{schema_name}.{table_name}`."
             )
             raise KeyError(msg) from ex
 
         return t.cast(sqlalchemy.types.TypeEngine, column.type)
 
     def get_table_columns(
         self,
         schema_name: str,
         table_name: str,
+        connection: sqlalchemy.engine.Connection,
         column_names: list[str] | None = None,
     ) -> dict[str, sqlalchemy.Column]:
         """Return a list of table columns.
 
         Overrode to support schema_name
 
         Args:
             schema_name: schema name.
             table_name: table name to get columns for.
             column_names: A list of column names to filter to.
 
         Returns:
             An ordered list of column objects.
         """
-        inspector = sqlalchemy.inspect(self._engine)
+        inspector = sqlalchemy.inspect(connection)
         columns = inspector.get_columns(table_name, schema_name)
 
         return {
             col_meta["name"]: sqlalchemy.Column(
                 col_meta["name"],
                 col_meta["type"],
                 nullable=col_meta.get("nullable", False),
             )
             for col_meta in columns
             if not column_names
             or col_meta["name"].casefold() in {col.casefold() for col in column_names}
         }
 
-    def column_exists(self, full_table_name: str, column_name: str) -> bool:
+    def column_exists(
+        self,
+        full_table_name: str,
+        column_name: str,
+        connection: sqlalchemy.engine.Connection,
+    ) -> bool:
         """Determine if the target column already exists.
 
         Args:
             full_table_name: the target table name.
             column_name: the target column name.
 
         Returns:
             True if table exists, False if not.
         """
         _, schema_name, table_name = self.parse_full_table_name(full_table_name)
         assert schema_name is not None
         assert table_name is not None
         return column_name in self.get_table_columns(
-            schema_name=schema_name, table_name=table_name
+            schema_name=schema_name, table_name=table_name, connection=connection
         )
 
 
 class NOTYPE(TypeDecorator):
     """Type to use when none is provided in the schema."""
 
-    impl = VARCHAR
+    impl = TEXT
     cache_ok = True
 
     def process_bind_param(self, value, dialect):
         """Return value as is unless it is dict or list.
 
         Used internally by SQL Alchemy. Should not be used directly.
         """
```

### Comparing `meltanolabs_target_postgres-0.0.8/target_postgres/sinks.py` & `meltanolabs_target_postgres-0.0.9/target_postgres/sinks.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,15 +41,15 @@
         """
         if self.key_properties is None or self.key_properties == []:
             self.append_only = True
         else:
             self.append_only = False
         if self.schema_name:
             self.connector.prepare_schema(self.schema_name)
-        with self.connector._connect() as connection:
+        with self.connector._connect() as connection, connection.begin():
             self.connector.prepare_table(
                 full_table_name=self.full_table_name,
                 schema=self.schema,
                 primary_keys=self.key_properties,
                 connection=connection,
                 as_temp_table=False,
             )
@@ -60,15 +60,15 @@
         Writes a batch to the SQL target. Developers may override this method
         in order to provide a more efficient upload/upsert process.
 
         Args:
             context: Stream partition or context dictionary.
         """
         # Use one connection so we do this all in a single transaction
-        with self.connector._connect() as connection:
+        with self.connector._connect() as connection, connection.begin():
             # Check structure of table
             table: sqlalchemy.Table = self.connector.prepare_table(
                 full_table_name=self.full_table_name,
                 schema=self.schema,
                 primary_keys=self.key_properties,
                 as_temp_table=False,
                 connection=connection,
@@ -138,30 +138,22 @@
         )
         self.logger.info("Inserting with SQL: %s", insert)
         # Only one record per PK, we want to take the last one
         data_to_insert: List[Dict[str, Any]] = []
 
         if self.append_only is False:
             insert_records: Dict[str, Dict] = {}  # pk : record
-            try:
-                for record in records:
-                    insert_record = {}
-                    for column in columns:
-                        insert_record[column.name] = record.get(column.name)
-                    primary_key_value = "".join(
-                        [str(record[key]) for key in primary_keys]
-                    )
-                    insert_records[primary_key_value] = insert_record
-            except KeyError:
-                raise RuntimeError(
-                    "Primary key not found in record. "
-                    f"full_table_name: {table.name}. "
-                    f"schema: {table.schema}.  "
-                    f"primary_keys: {primary_keys}."
-                )
+            for record in records:
+                insert_record = {}
+                for column in columns:
+                    insert_record[column.name] = record.get(column.name)
+                # No need to check for a KeyError here because the SDK already
+                # guaruntees that all key properties exist in the record.
+                primary_key_value = "".join([str(record[key]) for key in primary_keys])
+                insert_records[primary_key_value] = insert_record
             data_to_insert = list(insert_records.values())
         else:
             for record in records:
                 insert_record = {}
                 for column in columns:
                     insert_record[column.name] = record.get(column.name)
                 data_to_insert.append(insert_record)
@@ -175,18 +167,19 @@
         schema: dict,
         join_keys: List[Column],
         connection: sqlalchemy.engine.Connection,
     ) -> Optional[int]:
         """Merge upsert data from one table to another.
 
         Args:
-            from_table_name: The source table name.
-            to_table_name: The destination table name.
-            join_keys: The merge upsert keys, or `None` to append.
+            from_table: The source table.
+            to_table: The destination table.
             schema: Singer Schema message.
+            join_keys: The merge upsert keys, or `None` to append.
+            connection: The database connection.
 
         Return:
             The number of records copied, if detectable, or `None` if the API does not
             report number of records affected/inserted.
 
         """
         if self.append_only is True:
@@ -320,50 +313,55 @@
             {"type": "string", "format": "date-time"}
         )
 
         # Different from SingerSDK as we need to handle types the
         # same as SCHEMA messsages
         integer_type = self.connector.to_sql_type({"type": "integer"})
 
-        if not self.connector.column_exists(
-            full_table_name=self.full_table_name,
-            column_name=self.version_column_name,
-        ):
-            self.connector.prepare_column(
-                self.full_table_name,
-                self.version_column_name,
-                sql_type=integer_type,
-            )
+        with self.connector._connect() as connection, connection.begin():
+            if not self.connector.column_exists(
+                full_table_name=self.full_table_name,
+                column_name=self.version_column_name,
+                connection=connection,
+            ):
+                self.connector.prepare_column(
+                    self.full_table_name,
+                    self.version_column_name,
+                    sql_type=integer_type,
+                    connection=connection,
+                )
 
-        self.logger.info("Hard delete: %s", self.config.get("hard_delete"))
-        if self.config["hard_delete"] is True:
-            with self.connector._connect() as connection:
+            self.logger.info("Hard delete: %s", self.config.get("hard_delete"))
+            if self.config["hard_delete"] is True:
                 connection.execute(
-                    f'DELETE FROM "{self.schema_name}"."{self.table_name}" '
-                    f"WHERE {self.version_column_name} <= {new_version} "
-                    f"OR {self.version_column_name} IS NULL"
+                    sqlalchemy.text(
+                        f'DELETE FROM "{self.schema_name}"."{self.table_name}" '
+                        f"WHERE {self.version_column_name} <= {new_version} "
+                        f"OR {self.version_column_name} IS NULL"
+                    )
                 )
                 return
 
-        if not self.connector.column_exists(
-            full_table_name=self.full_table_name,
-            column_name=self.soft_delete_column_name,
-        ):
-            self.connector.prepare_column(
-                self.full_table_name,
-                self.soft_delete_column_name,
-                sql_type=datetime_type,
-            )
-        # Need to deal with the case where data doesn't exist for the version column
-        query = sqlalchemy.text(
-            f'UPDATE "{self.schema_name}"."{self.table_name}"\n'
-            f"SET {self.soft_delete_column_name} = :deletedate \n"
-            f"WHERE {self.version_column_name} < :version "
-            f"OR {self.version_column_name} IS NULL \n"
-            f"  AND {self.soft_delete_column_name} IS NULL\n"
-        )
-        query = query.bindparams(
-            bindparam("deletedate", value=deleted_at, type_=datetime_type),
-            bindparam("version", value=new_version, type_=integer_type),
-        )
-        with self.connector._connect() as connection:
+            if not self.connector.column_exists(
+                full_table_name=self.full_table_name,
+                column_name=self.soft_delete_column_name,
+                connection=connection,
+            ):
+                self.connector.prepare_column(
+                    self.full_table_name,
+                    self.soft_delete_column_name,
+                    sql_type=datetime_type,
+                    connection=connection,
+                )
+            # Need to deal with the case where data doesn't exist for the version column
+            query = sqlalchemy.text(
+                f'UPDATE "{self.schema_name}"."{self.table_name}"\n'
+                f"SET {self.soft_delete_column_name} = :deletedate \n"
+                f"WHERE {self.version_column_name} < :version "
+                f"OR {self.version_column_name} IS NULL \n"
+                f"  AND {self.soft_delete_column_name} IS NULL\n"
+            )
+            query = query.bindparams(
+                bindparam("deletedate", value=deleted_at, type_=datetime_type),
+                bindparam("version", value=new_version, type_=integer_type),
+            )
             connection.execute(query)
```

### Comparing `meltanolabs_target_postgres-0.0.8/target_postgres/target.py` & `meltanolabs_target_postgres-0.0.9/target_postgres/target.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """Postgres target class."""
 from __future__ import annotations
 
 from pathlib import PurePath
 
-import jsonschema
 from singer_sdk import typing as th
 from singer_sdk.target_base import SQLTarget
 
 from target_postgres.sinks import PostgresSink
 
 
 class TargetPostgres(SQLTarget):
@@ -316,24 +315,7 @@
         The default is 8 if not overridden.
 
         Returns:
             Max number of sinks that can be drained in parallel.
         """
         # https://github.com/MeltanoLabs/target-postgres/issues/3
         return 1
-
-    def _process_record_message(self, message_dict: dict) -> None:
-        """Process a RECORD message.
-
-        Args:
-            message_dict: TODO
-        """
-        stream_name = message_dict["stream"]
-        if self.mapper.stream_maps.get(stream_name) is None:
-            raise Exception(f"Schema message has not been sent for {stream_name}")
-        try:
-            super()._process_record_message(message_dict)
-        except jsonschema.exceptions.ValidationError as e:
-            self.logger.error(
-                f"Exception is being thrown for stream_name: {stream_name}"
-            )
-            raise e
```

### Comparing `meltanolabs_target_postgres-0.0.8/target_postgres/tests/data_files/array_data.singer` & `meltanolabs_target_postgres-0.0.9/target_postgres/tests/data_files/array_data.singer`

 * *Files identical despite different names*

### Comparing `meltanolabs_target_postgres-0.0.8/target_postgres/tests/data_files/camelcase_complex_schema.singer` & `meltanolabs_target_postgres-0.0.9/target_postgres/tests/data_files/camelcase_complex_schema.singer`

 * *Files identical despite different names*

### Comparing `meltanolabs_target_postgres-0.0.8/target_postgres/tests/data_files/commits.singer` & `meltanolabs_target_postgres-0.0.9/target_postgres/tests/data_files/commits.singer`

 * *Files identical despite different names*

### Comparing `meltanolabs_target_postgres-0.0.8/target_postgres/tests/data_files/duplicate_records.singer` & `meltanolabs_target_postgres-0.0.9/target_postgres/tests/data_files/duplicate_records.singer`

 * *Files identical despite different names*

### Comparing `meltanolabs_target_postgres-0.0.8/target_postgres/tests/data_files/encoded_strings.singer` & `meltanolabs_target_postgres-0.0.9/target_postgres/tests/data_files/encoded_strings.singer`

 * *Files identical despite different names*

### Comparing `meltanolabs_target_postgres-0.0.8/target_postgres/tests/data_files/missing_value.singer` & `meltanolabs_target_postgres-0.0.9/target_postgres/tests/data_files/missing_value.singer`

 * *Files identical despite different names*

### Comparing `meltanolabs_target_postgres-0.0.8/target_postgres/tests/data_files/multiple_state_messages.singer` & `meltanolabs_target_postgres-0.0.9/target_postgres/tests/data_files/multiple_state_messages.singer`

 * *Files identical despite different names*

### Comparing `meltanolabs_target_postgres-0.0.8/target_postgres/tests/data_files/optional_attributes.singer` & `meltanolabs_target_postgres-0.0.9/target_postgres/tests/data_files/optional_attributes.singer`

 * *Files identical despite different names*

### Comparing `meltanolabs_target_postgres-0.0.8/target_postgres/tests/data_files/reserved_keywords.singer` & `meltanolabs_target_postgres-0.0.9/target_postgres/tests/data_files/reserved_keywords.singer`

 * *Files identical despite different names*

### Comparing `meltanolabs_target_postgres-0.0.8/target_postgres/tests/data_files/schema_no_properties.singer` & `meltanolabs_target_postgres-0.0.9/target_postgres/tests/data_files/schema_no_properties.singer`

 * *Files identical despite different names*

### Comparing `meltanolabs_target_postgres-0.0.8/target_postgres/tests/data_files/schema_updates.singer` & `meltanolabs_target_postgres-0.0.9/target_postgres/tests/data_files/schema_updates.singer`

 * *Files identical despite different names*

### Comparing `meltanolabs_target_postgres-0.0.8/target_postgres/tests/data_files/special_chars_in_attributes.singer` & `meltanolabs_target_postgres-0.0.9/target_postgres/tests/data_files/special_chars_in_attributes.singer`

 * *Files identical despite different names*

### Comparing `meltanolabs_target_postgres-0.0.8/target_postgres/tests/data_files/tap_aapl.singer` & `meltanolabs_target_postgres-0.0.9/target_postgres/tests/data_files/tap_aapl.singer`

 * *Files identical despite different names*

### Comparing `meltanolabs_target_postgres-0.0.8/target_postgres/tests/data_files/tap_countries.singer` & `meltanolabs_target_postgres-0.0.9/target_postgres/tests/data_files/tap_countries.singer`

 * *Files identical despite different names*

### Comparing `meltanolabs_target_postgres-0.0.8/target_postgres/tests/data_files/test_activate_version_deletes_data_properly.singer` & `meltanolabs_target_postgres-0.0.9/target_postgres/tests/data_files/test_activate_version_deletes_data_properly.singer`

 * *Files identical despite different names*

### Comparing `meltanolabs_target_postgres-0.0.8/target_postgres/tests/data_files/test_activate_version_hard.singer` & `meltanolabs_target_postgres-0.0.9/target_postgres/tests/data_files/test_activate_version_hard.singer`

 * *Files identical despite different names*

### Comparing `meltanolabs_target_postgres-0.0.8/target_postgres/tests/data_files/test_activate_version_soft.singer` & `meltanolabs_target_postgres-0.0.9/target_postgres/tests/data_files/test_activate_version_soft.singer`

 * *Files identical despite different names*

### Comparing `meltanolabs_target_postgres-0.0.8/target_postgres/tests/data_files/test_activate_version_uppercase_stream_name.singer` & `meltanolabs_target_postgres-0.0.9/target_postgres/tests/data_files/test_activate_version_uppercase_stream_name.singer`

 * *Files identical despite different names*

### Comparing `meltanolabs_target_postgres-0.0.8/target_postgres/tests/data_files/test_no_pk_append.singer` & `meltanolabs_target_postgres-0.0.9/target_postgres/tests/data_files/test_no_pk_append.singer`

 * *Files identical despite different names*

### Comparing `meltanolabs_target_postgres-0.0.8/target_postgres/tests/data_files/test_no_type.singer` & `meltanolabs_target_postgres-0.0.9/target_postgres/tests/data_files/test_no_type.singer`

 * *Files identical despite different names*

### Comparing `meltanolabs_target_postgres-0.0.8/target_postgres/tests/data_files/uppercase_stream_name_with_column_alter.singer` & `meltanolabs_target_postgres-0.0.9/target_postgres/tests/data_files/uppercase_stream_name_with_column_alter.singer`

 * *Files identical despite different names*

### Comparing `meltanolabs_target_postgres-0.0.8/target_postgres/tests/data_files/user_location_data.singer` & `meltanolabs_target_postgres-0.0.9/target_postgres/tests/data_files/user_location_data.singer`

 * *Files identical despite different names*

### Comparing `meltanolabs_target_postgres-0.0.8/target_postgres/tests/data_files/user_location_upsert_data.singer` & `meltanolabs_target_postgres-0.0.9/target_postgres/tests/data_files/user_location_upsert_data.singer`

 * *Files identical despite different names*

### Comparing `meltanolabs_target_postgres-0.0.8/target_postgres/tests/samples/aapl/AAPL.json` & `meltanolabs_target_postgres-0.0.9/target_postgres/tests/samples/aapl/AAPL.json`

 * *Files identical despite different names*

### Comparing `meltanolabs_target_postgres-0.0.8/target_postgres/tests/samples/aapl/aapl.py` & `meltanolabs_target_postgres-0.0.9/target_postgres/tests/samples/aapl/aapl.py`

 * *Files identical despite different names*

### Comparing `meltanolabs_target_postgres-0.0.8/target_postgres/tests/samples/aapl/fundamentals.json` & `meltanolabs_target_postgres-0.0.9/target_postgres/tests/samples/aapl/fundamentals.json`

 * *Files identical despite different names*

### Comparing `meltanolabs_target_postgres-0.0.8/target_postgres/tests/samples/sample_tap_countries/countries_streams.py` & `meltanolabs_target_postgres-0.0.9/target_postgres/tests/samples/sample_tap_countries/countries_streams.py`

 * *Files identical despite different names*

### Comparing `meltanolabs_target_postgres-0.0.8/target_postgres/tests/samples/sample_tap_countries/countries_tap.py` & `meltanolabs_target_postgres-0.0.9/target_postgres/tests/samples/sample_tap_countries/countries_tap.py`

 * *Files identical despite different names*

### Comparing `meltanolabs_target_postgres-0.0.8/target_postgres/tests/test_standard_target.py` & `meltanolabs_target_postgres-0.0.9/target_postgres/tests/test_standard_target.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,17 +5,18 @@
 import uuid
 from contextlib import redirect_stdout
 from pathlib import Path
 
 import jsonschema
 import pytest
 import sqlalchemy
+from singer_sdk.exceptions import MissingKeyPropertiesError
 from singer_sdk.testing import sync_end_to_end
 from sqlalchemy.dialects.postgresql import ARRAY
-from sqlalchemy.types import TIMESTAMP, VARCHAR
+from sqlalchemy.types import TEXT, TIMESTAMP
 
 from target_postgres.connector import PostgresConnector
 from target_postgres.target import TargetPostgres
 from target_postgres.tests.samples.aapl.aapl import Fundamentals
 from target_postgres.tests.samples.sample_tap_countries.countries_tap import (
     SampleTapCountries,
 )
@@ -150,15 +151,15 @@
     password = config["password"]
     database = config["database"]
     target_config = TargetPostgres(config=config).config
     connector = PostgresConnector(target_config)
 
     engine: sqlalchemy.engine.Engine = connector._engine
     assert (
-        str(engine.url)
+        engine.url.render_as_string(hide_password=False)
         == f"{dialect_driver}://{user}:{password}@{host}:5432/{database}"
     )
 
 
 def test_port_config():
     """Test that the port config works"""
     config = {
@@ -175,15 +176,15 @@
     password = config["password"]
     database = config["database"]
     target_config = TargetPostgres(config=config).config
     connector = PostgresConnector(target_config)
 
     engine: sqlalchemy.engine.Engine = connector._engine
     assert (
-        str(engine.url)
+        engine.url.render_as_string(hide_password=False)
         == f"{dialect_driver}://{user}:{password}@{host}:5433/{database}"
     )
 
 
 # Test name would work well
 def test_countries_to_postgres(postgres_config):
     tap = SampleTapCountries(config={}, state=None)
@@ -193,35 +194,25 @@
 
 def test_aapl_to_postgres(postgres_config):
     tap = Fundamentals(config={}, state=None)
     target = TargetPostgres(config=postgres_config)
     sync_end_to_end(tap, target)
 
 
-def test_record_before_schema(postgres_target):
-    with pytest.raises(Exception) as e:
-        file_name = "record_before_schema.singer"
-        singer_file_to_target(file_name, postgres_target)
-
-    assert (
-        str(e.value) == "Schema message has not been sent for test_record_before_schema"
-    )
-
-
 def test_invalid_schema(postgres_target):
     with pytest.raises(Exception) as e:
         file_name = "invalid_schema.singer"
         singer_file_to_target(file_name, postgres_target)
     assert (
         str(e.value) == "Line is missing required properties key(s): {'type': 'object'}"
     )
 
 
 def test_record_missing_key_property(postgres_target):
-    with pytest.raises(Exception) as e:
+    with pytest.raises(MissingKeyPropertiesError) as e:
         file_name = "record_missing_key_property.singer"
         singer_file_to_target(file_name, postgres_target)
     assert "Record is missing one or more key_properties." in str(e.value)
 
 
 def test_record_missing_required_property(postgres_target):
     with pytest.raises(jsonschema.exceptions.ValidationError):
@@ -282,28 +273,32 @@
             {"id": 5, "name": "Jim"},
             {"id": 8, "name": "Thomas"},
             {"id": 12, "name": "Paul"},
             {"id": 13, "name": "Mary"},
         ]
 
         full_table_name = f"{schema_name}.test_users"
-        result = connection.execute(f"SELECT * FROM {full_table_name} ORDER BY id")
+        result = connection.execute(
+            sqlalchemy.text(f"SELECT * FROM {full_table_name} ORDER BY id")
+        )
         result_dict = [remove_metadata_columns(row._asdict()) for row in result.all()]
         assert result_dict == expected_test_users
 
         expected_test_locations = [
             {"id": 1, "name": "Philly"},
             {"id": 2, "name": "NY"},
             {"id": 3, "name": "San Francisco"},
             {"id": 6, "name": "Colorado"},
             {"id": 8, "name": "Boston"},
         ]
 
         full_table_name = f"{schema_name}.test_locations"
-        result = connection.execute(f"SELECT * FROM {full_table_name} ORDER BY id")
+        result = connection.execute(
+            sqlalchemy.text(f"SELECT * FROM {full_table_name} ORDER BY id")
+        )
         result_dict = [remove_metadata_columns(row._asdict()) for row in result.all()]
         assert result_dict == expected_test_locations
 
         expected_test_user_in_location = [
             {
                 "id": 1,
                 "user_id": 1,
@@ -333,41 +328,45 @@
                 "user_id": 4,
                 "location_id": 1,
                 "info": {"weather": "cloudy", "mood": "ok"},
             },
         ]
 
         full_table_name = f"{schema_name}.test_user_in_location"
-        result = connection.execute(f"SELECT * FROM {full_table_name} ORDER BY id")
+        result = connection.execute(
+            sqlalchemy.text(f"SELECT * FROM {full_table_name} ORDER BY id")
+        )
         result_dict = [remove_metadata_columns(row._asdict()) for row in result.all()]
         assert result_dict == expected_test_user_in_location
 
 
 def test_no_primary_keys(postgres_target):
     """We run both of these tests twice just to ensure that no records are removed and append only works properly"""
     engine = create_engine(postgres_target)
     table_name = "test_no_pk"
     full_table_name = postgres_target.config["default_target_schema"] + "." + table_name
-    with engine.connect() as connection:
-        result = connection.execute(f"DROP TABLE IF EXISTS {full_table_name}")
+    with engine.connect() as connection, connection.begin():
+        result = connection.execute(
+            sqlalchemy.text(f"DROP TABLE IF EXISTS {full_table_name}")
+        )
     file_name = f"{table_name}.singer"
     singer_file_to_target(file_name, postgres_target)
 
     file_name = f"{table_name}_append.singer"
     singer_file_to_target(file_name, postgres_target)
 
     file_name = f"{table_name}.singer"
     singer_file_to_target(file_name, postgres_target)
 
     file_name = f"{table_name}_append.singer"
     singer_file_to_target(file_name, postgres_target)
 
     # Will populate us with 22 records, we run this twice
     with engine.connect() as connection:
-        result = connection.execute(f"SELECT * FROM {full_table_name}")
+        result = connection.execute(sqlalchemy.text(f"SELECT * FROM {full_table_name}"))
         assert result.rowcount == 16
 
 
 def test_no_type(postgres_target):
     file_name = "test_no_type.singer"
     singer_file_to_target(file_name, postgres_target)
 
@@ -424,20 +423,22 @@
     """Test that anyOf is handled correctly"""
     engine = create_engine(postgres_target)
     table_name = "commits"
     file_name = f"{table_name}.singer"
     schema = postgres_target.config["default_target_schema"]
     singer_file_to_target(file_name, postgres_target)
     with engine.connect() as connection:
-        meta = sqlalchemy.MetaData(bind=connection)
-        table = sqlalchemy.Table("commits", meta, schema=schema, autoload=True)
+        meta = sqlalchemy.MetaData()
+        table = sqlalchemy.Table(
+            "commits", meta, schema=schema, autoload_with=connection
+        )
         for column in table.c:
             # {"type":"string"}
             if column.name == "id":
-                assert isinstance(column.type, VARCHAR)
+                assert isinstance(column.type, TEXT)
 
             # Any of nullable date-time.
             # Note that postgres timestamp is equivalent to jsonschema date-time.
             # {"anyOf":[{"type":"string","format":"date-time"},{"type":"null"}]}
             if column.name in {"authored_date", "committed_date"}:
                 assert isinstance(column.type, TIMESTAMP)
 
@@ -445,20 +446,20 @@
             # {"anyOf":[{"type":"array","items":{"type":["null","string"]}},{"type":"string"},{"type":"null"}]}
             if column.name == "parent_ids":
                 assert isinstance(column.type, ARRAY)
 
             # Any of nullable string.
             # {"anyOf":[{"type":"string"},{"type":"null"}]}
             if column.name == "commit_message":
-                assert isinstance(column.type, VARCHAR)
+                assert isinstance(column.type, TEXT)
 
             # Any of nullable string or integer.
             # {"anyOf":[{"type":"string"},{"type":"integer"},{"type":"null"}]}
             if column.name == "legacy_id":
-                assert isinstance(column.type, VARCHAR)
+                assert isinstance(column.type, TEXT)
 
 
 def test_new_array_column(postgres_target):
     """Create a new Array column with an existing table"""
     file_name = "new_array_column.singer"
     singer_file_to_target(file_name, postgres_target)
 
@@ -470,102 +471,127 @@
     full_table_name = postgres_config_no_ssl["default_target_schema"] + "." + table_name
     postgres_config_hard_delete_true = copy.deepcopy(postgres_config_no_ssl)
     postgres_config_hard_delete_true["hard_delete"] = True
     pg_hard_delete_true = TargetPostgres(config=postgres_config_hard_delete_true)
     engine = create_engine(pg_hard_delete_true)
     singer_file_to_target(file_name, pg_hard_delete_true)
     with engine.connect() as connection:
-        result = connection.execute(f"SELECT * FROM {full_table_name}")
+        result = connection.execute(sqlalchemy.text(f"SELECT * FROM {full_table_name}"))
         assert result.rowcount == 7
+    with engine.connect() as connection, connection.begin():
         # Add a record like someone would if they weren't using the tap target combo
         result = connection.execute(
-            f"INSERT INTO {full_table_name}(code, \"name\") VALUES('Manual1', 'Meltano')"
+            sqlalchemy.text(
+                f"INSERT INTO {full_table_name}(code, \"name\") VALUES('Manual1', 'Meltano')"
+            )
         )
         result = connection.execute(
-            f"INSERT INTO {full_table_name}(code, \"name\") VALUES('Manual2', 'Meltano')"
+            sqlalchemy.text(
+                f"INSERT INTO {full_table_name}(code, \"name\") VALUES('Manual2', 'Meltano')"
+            )
         )
-        result = connection.execute(f"SELECT * FROM {full_table_name}")
+    with engine.connect() as connection:
+        result = connection.execute(sqlalchemy.text(f"SELECT * FROM {full_table_name}"))
         assert result.rowcount == 9
 
     singer_file_to_target(file_name, pg_hard_delete_true)
 
     # Should remove the 2 records we added manually
     with engine.connect() as connection:
-        result = connection.execute(f"SELECT * FROM {full_table_name}")
+        result = connection.execute(sqlalchemy.text(f"SELECT * FROM {full_table_name}"))
         assert result.rowcount == 7
 
 
 def test_activate_version_soft_delete(postgres_target):
     """Activate Version Soft Delete Test"""
     engine = create_engine(postgres_target)
     table_name = "test_activate_version_soft"
     file_name = f"{table_name}.singer"
     full_table_name = postgres_target.config["default_target_schema"] + "." + table_name
-    with engine.connect() as connection:
-        result = connection.execute(f"DROP TABLE IF EXISTS {full_table_name}")
+    with engine.connect() as connection, connection.begin():
+        result = connection.execute(
+            sqlalchemy.text(f"DROP TABLE IF EXISTS {full_table_name}")
+        )
     postgres_config_soft_delete = copy.deepcopy(postgres_target._config)
     postgres_config_soft_delete["hard_delete"] = False
     pg_soft_delete = TargetPostgres(config=postgres_config_soft_delete)
     singer_file_to_target(file_name, pg_soft_delete)
 
     with engine.connect() as connection:
-        result = connection.execute(f"SELECT * FROM {full_table_name}")
+        result = connection.execute(sqlalchemy.text(f"SELECT * FROM {full_table_name}"))
         assert result.rowcount == 7
+    with engine.connect() as connection, connection.begin():
         # Add a record like someone would if they weren't using the tap target combo
         result = connection.execute(
-            f"INSERT INTO {full_table_name}(code, \"name\") VALUES('Manual1', 'Meltano')"
+            sqlalchemy.text(
+                f"INSERT INTO {full_table_name}(code, \"name\") VALUES('Manual1', 'Meltano')"
+            )
         )
         result = connection.execute(
-            f"INSERT INTO {full_table_name}(code, \"name\") VALUES('Manual2', 'Meltano')"
+            sqlalchemy.text(
+                f"INSERT INTO {full_table_name}(code, \"name\") VALUES('Manual2', 'Meltano')"
+            )
         )
-        result = connection.execute(f"SELECT * FROM {full_table_name}")
+    with engine.connect() as connection:
+        result = connection.execute(sqlalchemy.text(f"SELECT * FROM {full_table_name}"))
         assert result.rowcount == 9
 
     singer_file_to_target(file_name, pg_soft_delete)
 
     # Should have all records including the 2 we added manually
     with engine.connect() as connection:
-        result = connection.execute(f"SELECT * FROM {full_table_name}")
+        result = connection.execute(sqlalchemy.text(f"SELECT * FROM {full_table_name}"))
         assert result.rowcount == 9
 
         result = connection.execute(
-            f"SELECT * FROM {full_table_name} where _sdc_deleted_at is NOT NULL"
+            sqlalchemy.text(
+                f"SELECT * FROM {full_table_name} where _sdc_deleted_at is NOT NULL"
+            )
         )
         assert result.rowcount == 2
 
 
 def test_activate_version_deletes_data_properly(postgres_target):
     """Activate Version should"""
     engine = create_engine(postgres_target)
     table_name = "test_activate_version_deletes_data_properly"
     file_name = f"{table_name}.singer"
     full_table_name = postgres_target.config["default_target_schema"] + "." + table_name
-    with engine.connect() as connection:
-        result = connection.execute(f"DROP TABLE IF EXISTS {full_table_name}")
+    with engine.connect() as connection, connection.begin():
+        result = connection.execute(
+            sqlalchemy.text(f"DROP TABLE IF EXISTS {full_table_name}")
+        )
 
     postgres_config_soft_delete = copy.deepcopy(postgres_target._config)
     postgres_config_soft_delete["hard_delete"] = True
     pg_hard_delete = TargetPostgres(config=postgres_config_soft_delete)
     singer_file_to_target(file_name, pg_hard_delete)
     # Will populate us with 7 records
     with engine.connect() as connection:
+        result = connection.execute(sqlalchemy.text(f"SELECT * FROM {full_table_name}"))
+        assert result.rowcount == 7
+    with engine.connect() as connection, connection.begin():
         result = connection.execute(
-            f"INSERT INTO {full_table_name} (code, \"name\") VALUES('Manual1', 'Meltano')"
+            sqlalchemy.text(
+                f"INSERT INTO {full_table_name} (code, \"name\") VALUES('Manual1', 'Meltano')"
+            )
         )
         result = connection.execute(
-            f"INSERT INTO {full_table_name} (code, \"name\") VALUES('Manual2', 'Meltano')"
+            sqlalchemy.text(
+                f"INSERT INTO {full_table_name} (code, \"name\") VALUES('Manual2', 'Meltano')"
+            )
         )
-        result = connection.execute(f"SELECT * FROM {full_table_name}")
+    with engine.connect() as connection:
+        result = connection.execute(sqlalchemy.text(f"SELECT * FROM {full_table_name}"))
         assert result.rowcount == 9
-
     # Only has a schema and one activate_version message, should delete all records as it's a higher version than what's currently in the table
     file_name = f"{table_name}_2.singer"
     singer_file_to_target(file_name, pg_hard_delete)
     with engine.connect() as connection:
-        result = connection.execute(f"SELECT * FROM {full_table_name}")
+        result = connection.execute(sqlalchemy.text(f"SELECT * FROM {full_table_name}"))
         assert result.rowcount == 0
 
 
 def test_reserved_keywords(postgres_target):
     """Target should work regardless of column names
 
     Postgres has a number of resereved keywords listed here https://www.postgresql.org/docs/current/sql-keywords-appendix.html.
```

### Comparing `meltanolabs_target_postgres-0.0.8/PKG-INFO` & `meltanolabs_target_postgres-0.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meltanolabs-target-postgres
-Version: 0.0.8
+Version: 0.0.9
 Summary: `target-postgres` is a Singer target for Postgres, built with the Meltano SDK for Singer Targets.
 Home-page: https://meltano.com
 License: MIT
 Keywords: Postgres,Singer,ELT,Meltano,Meltano SDK
 Author: Meltano Team and Contributors
 Author-email: hello@meltano.com
 Maintainer: Meltano Team and Contributors
@@ -16,24 +16,29 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Requires-Dist: psycopg2-binary (==2.9.7)
+Requires-Dist: psycopg2-binary (==2.9.9)
 Requires-Dist: requests (>=2.25.1,<3.0.0)
-Requires-Dist: singer-sdk (>=0.28,<0.32)
-Requires-Dist: sqlalchemy (<2)
+Requires-Dist: singer-sdk (>=0.28,<0.34)
+Requires-Dist: sqlalchemy (>=2.0,<3.0)
 Requires-Dist: sshtunnel (==0.4.0)
 Project-URL: Repository, https://github.com/meltanolabs/target-postgres
 Description-Content-Type: text/markdown
 
 # `target-postgres`
 
+![PyPI - Version](https://img.shields.io/pypi/v/meltanolabs-target-postgres)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/meltanolabs-target-postgres)
+![PyPI - License](https://img.shields.io/pypi/l/meltanolabs-target-postgres)
+![Test target-postgres](https://github.com/meltanolabs/target-postgres/actions/workflows/ci_workflow.yml/badge.svg)
+
 Target for Postgres.
 
 Built with the [Meltano SDK](https://sdk.meltano.com) for Singer Taps and Targets.
 
 ## Capabilities
 
 * `about`
@@ -72,18 +77,16 @@
 | flattening_enabled           | False    | None    | 'True' to enable schema flattening and automatically expand nested properties. |
 | flattening_max_depth         | False    | None    | The max depth to flatten schemas. |
 
 A full list of supported settings and capabilities is available by running: `target-postgres --about`
 
 ## Installation
 
-- [ ] `Developer TODO:` Come back to this re [#5](https://github.com/MeltanoLabs/target-postgres/issues/5)
-
 ```bash
-pipx install -e .
+pipx install meltanolabs-target-postgres
 ```
 
 ## Configuration
 
 ### An Explanation of Various SSL Configuration Options
 
 There are two distinct processes which both fall under the banner of SSL. One process occurs when the client wishes to ensure the identity of the server, and is the more common reason that SSL is used. Another is when the server wishes to ensure the identity of the client, for authentication/authorization purposes.
```

