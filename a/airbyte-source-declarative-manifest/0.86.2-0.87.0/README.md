# Comparing `tmp/airbyte_source_declarative_manifest-0.86.2.tar.gz` & `tmp/airbyte_source_declarative_manifest-0.87.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_declarative_manifest-0.86.2.tar", max compression
+gzip compressed data, was "airbyte_source_declarative_manifest-0.87.0.tar", max compression
```

## Comparing `airbyte_source_declarative_manifest-0.86.2.tar` & `airbyte_source_declarative_manifest-0.87.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     3992 2024-05-02 14:55:17.701976 airbyte_source_declarative_manifest-0.86.2/README.md
--rw-r--r--   0        0        0      817 2024-05-02 14:59:14.045201 airbyte_source_declarative_manifest-0.86.2/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-02 14:55:17.701976 airbyte_source_declarative_manifest-0.86.2/source_declarative_manifest/__init__.py
--rw-r--r--   0        0        0     2180 2024-05-02 14:55:17.701976 airbyte_source_declarative_manifest-0.86.2/source_declarative_manifest/run.py
--rw-r--r--   0        0        0      554 2024-05-02 14:55:17.701976 airbyte_source_declarative_manifest-0.86.2/source_declarative_manifest/spec.json
--rw-r--r--   0        0        0     4728 1970-01-01 00:00:00.000000 airbyte_source_declarative_manifest-0.86.2/PKG-INFO
+-rw-r--r--   0        0        0     4003 2024-05-07 15:44:57.771301 airbyte_source_declarative_manifest-0.87.0/README.md
+-rw-r--r--   0        0        0      817 2024-05-07 15:48:55.866973 airbyte_source_declarative_manifest-0.87.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-07 15:44:57.771301 airbyte_source_declarative_manifest-0.87.0/source_declarative_manifest/__init__.py
+-rw-r--r--   0        0        0     2180 2024-05-07 15:44:57.771301 airbyte_source_declarative_manifest-0.87.0/source_declarative_manifest/run.py
+-rw-r--r--   0        0        0      554 2024-05-07 15:44:57.771301 airbyte_source_declarative_manifest-0.87.0/source_declarative_manifest/spec.json
+-rw-r--r--   0        0        0     4739 1970-01-01 00:00:00.000000 airbyte_source_declarative_manifest-0.87.0/PKG-INFO
```

### Comparing `airbyte_source_declarative_manifest-0.86.2/README.md` & `airbyte_source_declarative_manifest-0.87.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -7,78 +7,88 @@
 **Note**: This connector is managed by the Airbyte Python CDK release process. It can be run as a standalone connector
 in Docker and PyAirbyte, but is not yet meant to be run in the platform as a standalone connector. This source is
 an interface to the low-code CDK and as such, should not be modified without a corresponding CDK change.
 
 ## Local development
 
 ### Prerequisites
-* Python (~=3.9)
-* Poetry (~=1.7) - installation instructions [here](https://python-poetry.org/docs/#installation)
 
+- Python (~=3.9)
+- Poetry (~=1.7) - installation instructions [here](https://python-poetry.org/docs/#installation)
 
 ### Installing the connector
+
 From this connector directory, run:
+
 ```bash
 poetry install
 ```
 
-
 ### Create credentials
+
 The credentials for source-declarative-manifest are a little different. Your `config` will need to contain the
 injected declarative manifest, as indicated in the `spec`. It will also need to contain the fields that the spec
 coming out of the manifest requires. An example is available in `integration_tests/pokeapi_config.json`. To use
 this example in the following instructions, copy this file to `secrets/config.json`.
 
-
 ### Locally running the connector
+
 ```
 poetry run source-declarative-manifest spec
 poetry run source-declarative-manifest check --config secrets/config.json
 poetry run source-declarative-manifest discover --config secrets/config.json
 poetry run source-declarative-manifest read --config secrets/config.json --catalog sample_files/configured_catalog.json
 ```
 
 ### Running unit tests
+
 To run unit tests locally, from the connector directory run:
+
 ```
 poetry run pytest unit_tests
 ```
 
 ### Building the docker image
+
 1. Install [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md)
 2. Run the following command to build the docker image:
+
 ```bash
 airbyte-ci connectors --name=source-declarative-manifest build
 ```
 
 An image will be available on your host with the tag `airbyte/source-declarative-manifest:dev`.
 
-
 ### Running as a docker container
+
 Then run any of the connector commands as follows:
+
 ```
 docker run --rm airbyte/source-declarative-manifest:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-declarative-manifest:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-declarative-manifest:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-declarative-manifest:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
 ### Running our CI test suite
+
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
+
 ```bash
 airbyte-ci connectors --name=source-declarative-manifest test
 ```
-This source does not currently pass the full test suite.
 
+This source does not currently pass the full test suite.
 
 ### Dependency Management
+
 The manifest declarative source is built to be an interface to the low-code CDK source. This means that
 this source should not have any production dependencies other than the Airbyte Python CDK. If for some reason
 you feel that a new dependency is needed, you likely want to add it to the CDK instead. It is expected
 that a given version of the source-declarative-manifest connector corresponds to the same version in
 its CDK dependency.
 
-
 ## Publishing a new version of the connector
+
 New versions of this connector should only be published (automatically) via the manual Airbyte CDK release process.
 If you want to make a change to this connector that is not a result of a CDK change and a corresponding
-CDK dependency bump, please reach out to the Connector Extensibility team for guidance.
+CDK dependency bump, please reach out to the Connector Extensibility team for guidance.
```

### Comparing `airbyte_source_declarative_manifest-0.86.2/pyproject.toml` & `airbyte_source_declarative_manifest-0.87.0/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "0.86.2"
+version = "0.87.0"
 name = "airbyte-source-declarative-manifest"
 description = "Base source implementation for low-code sources."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "MIT"
 readme = "README.md"
@@ -18,15 +18,15 @@
 repository = "https://github.com/airbytehq/airbyte"
 packages = [
     { include = "source_declarative_manifest" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9,<3.12"
-airbyte-cdk = "0.86.3"
+airbyte-cdk = "0.87.0"
 
 [tool.poetry.scripts]
 source-declarative-manifest = "source_declarative_manifest.run:run"
 
 [tool.poetry.group.dev.dependencies]
 pytest-mock = "^3.6.1"
 pytest = "^6.2"
```

### Comparing `airbyte_source_declarative_manifest-0.86.2/source_declarative_manifest/run.py` & `airbyte_source_declarative_manifest-0.87.0/source_declarative_manifest/run.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_declarative_manifest-0.86.2/source_declarative_manifest/spec.json` & `airbyte_source_declarative_manifest-0.87.0/source_declarative_manifest/spec.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_declarative_manifest-0.86.2/PKG-INFO` & `airbyte_source_declarative_manifest-0.87.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: airbyte-source-declarative-manifest
-Version: 0.86.2
+Version: 0.87.0
 Summary: Base source implementation for low-code sources.
 Home-page: https://airbyte.com
 License: MIT
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: airbyte-cdk (==0.86.3)
+Requires-Dist: airbyte-cdk (==0.87.0)
 Project-URL: Documentation, https://docs.airbyte.com/integrations/sources/low-code
 Project-URL: Repository, https://github.com/airbytehq/airbyte
 Description-Content-Type: text/markdown
 
 # Declarative-Manifest source connector
 
 This is the repository for the Declarative-Manifest source connector, written in Python.
@@ -26,78 +26,89 @@
 **Note**: This connector is managed by the Airbyte Python CDK release process. It can be run as a standalone connector
 in Docker and PyAirbyte, but is not yet meant to be run in the platform as a standalone connector. This source is
 an interface to the low-code CDK and as such, should not be modified without a corresponding CDK change.
 
 ## Local development
 
 ### Prerequisites
-* Python (~=3.9)
-* Poetry (~=1.7) - installation instructions [here](https://python-poetry.org/docs/#installation)
 
+- Python (~=3.9)
+- Poetry (~=1.7) - installation instructions [here](https://python-poetry.org/docs/#installation)
 
 ### Installing the connector
+
 From this connector directory, run:
+
 ```bash
 poetry install
 ```
 
-
 ### Create credentials
+
 The credentials for source-declarative-manifest are a little different. Your `config` will need to contain the
 injected declarative manifest, as indicated in the `spec`. It will also need to contain the fields that the spec
 coming out of the manifest requires. An example is available in `integration_tests/pokeapi_config.json`. To use
 this example in the following instructions, copy this file to `secrets/config.json`.
 
-
 ### Locally running the connector
+
 ```
 poetry run source-declarative-manifest spec
 poetry run source-declarative-manifest check --config secrets/config.json
 poetry run source-declarative-manifest discover --config secrets/config.json
 poetry run source-declarative-manifest read --config secrets/config.json --catalog sample_files/configured_catalog.json
 ```
 
 ### Running unit tests
+
 To run unit tests locally, from the connector directory run:
+
 ```
 poetry run pytest unit_tests
 ```
 
 ### Building the docker image
+
 1. Install [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md)
 2. Run the following command to build the docker image:
+
 ```bash
 airbyte-ci connectors --name=source-declarative-manifest build
 ```
 
 An image will be available on your host with the tag `airbyte/source-declarative-manifest:dev`.
 
-
 ### Running as a docker container
+
 Then run any of the connector commands as follows:
+
 ```
 docker run --rm airbyte/source-declarative-manifest:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-declarative-manifest:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-declarative-manifest:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-declarative-manifest:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
 ### Running our CI test suite
+
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
+
 ```bash
 airbyte-ci connectors --name=source-declarative-manifest test
 ```
-This source does not currently pass the full test suite.
 
+This source does not currently pass the full test suite.
 
 ### Dependency Management
+
 The manifest declarative source is built to be an interface to the low-code CDK source. This means that
 this source should not have any production dependencies other than the Airbyte Python CDK. If for some reason
 you feel that a new dependency is needed, you likely want to add it to the CDK instead. It is expected
 that a given version of the source-declarative-manifest connector corresponds to the same version in
 its CDK dependency.
 
-
 ## Publishing a new version of the connector
+
 New versions of this connector should only be published (automatically) via the manual Airbyte CDK release process.
 If you want to make a change to this connector that is not a result of a CDK change and a corresponding
 CDK dependency bump, please reach out to the Connector Extensibility team for guidance.
+
```

