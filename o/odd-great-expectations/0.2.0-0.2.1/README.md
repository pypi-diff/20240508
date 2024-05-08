# Comparing `tmp/odd_great_expectations-0.2.0.tar.gz` & `tmp/odd_great_expectations-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odd_great_expectations-0.2.0.tar", max compression
+gzip compressed data, was "odd_great_expectations-0.2.1.tar", max compression
```

## Comparing `odd_great_expectations-0.2.0.tar` & `odd_great_expectations-0.2.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    11357 2024-05-01 12:30:00.424308 odd_great_expectations-0.2.0/LICENSE
--rw-r--r--   0        0        0     1800 2024-05-01 12:30:00.424308 odd_great_expectations-0.2.0/README.md
--rw-r--r--   0        0        0        0 2024-05-01 12:30:00.428308 odd_great_expectations-0.2.0/odd_great_expectations/__init__.py
--rw-r--r--   0        0        0     2994 2024-05-01 12:30:00.428308 odd_great_expectations-0.2.0/odd_great_expectations/action.py
--rw-r--r--   0        0        0       80 2024-05-01 12:30:00.428308 odd_great_expectations-0.2.0/odd_great_expectations/dataset/__init__.py
--rw-r--r--   0        0        0      786 2024-05-01 12:30:00.428308 odd_great_expectations-0.2.0/odd_great_expectations/dataset/file.py
--rw-r--r--   0        0        0      721 2024-05-01 12:30:00.428308 odd_great_expectations-0.2.0/odd_great_expectations/dataset/get_dataset.py
--rw-r--r--   0        0        0     2310 2024-05-01 12:30:00.428308 odd_great_expectations-0.2.0/odd_great_expectations/dataset/sql_table.py
--rw-r--r--   0        0        0      460 2024-05-01 12:30:00.428308 odd_great_expectations-0.2.0/odd_great_expectations/logger.py
--rw-r--r--   0        0        0     4521 2024-05-01 12:30:00.428308 odd_great_expectations-0.2.0/odd_great_expectations/mapper.py
--rw-r--r--   0        0        0      777 2024-05-01 12:30:13.024219 odd_great_expectations-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2732 1970-01-01 00:00:00.000000 odd_great_expectations-0.2.0/setup.py
--rw-r--r--   0        0        0     2725 1970-01-01 00:00:00.000000 odd_great_expectations-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-08 09:23:39.497462 odd_great_expectations-0.2.1/LICENSE
+-rw-r--r--   0        0        0     1800 2024-05-08 09:23:39.497462 odd_great_expectations-0.2.1/README.md
+-rw-r--r--   0        0        0        0 2024-05-08 09:23:39.497462 odd_great_expectations-0.2.1/odd_great_expectations/__init__.py
+-rw-r--r--   0        0        0     3026 2024-05-08 09:23:39.497462 odd_great_expectations-0.2.1/odd_great_expectations/action.py
+-rw-r--r--   0        0        0       80 2024-05-08 09:23:39.497462 odd_great_expectations-0.2.1/odd_great_expectations/dataset/__init__.py
+-rw-r--r--   0        0        0      786 2024-05-08 09:23:39.497462 odd_great_expectations-0.2.1/odd_great_expectations/dataset/file.py
+-rw-r--r--   0        0        0      721 2024-05-08 09:23:39.497462 odd_great_expectations-0.2.1/odd_great_expectations/dataset/get_dataset.py
+-rw-r--r--   0        0        0     2310 2024-05-08 09:23:39.497462 odd_great_expectations-0.2.1/odd_great_expectations/dataset/sql_table.py
+-rw-r--r--   0        0        0      460 2024-05-08 09:23:39.497462 odd_great_expectations-0.2.1/odd_great_expectations/logger.py
+-rw-r--r--   0        0        0     4680 2024-05-08 09:23:39.497462 odd_great_expectations-0.2.1/odd_great_expectations/mapper.py
+-rw-r--r--   0        0        0      783 2024-05-08 09:23:53.829596 odd_great_expectations-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2738 1970-01-01 00:00:00.000000 odd_great_expectations-0.2.1/setup.py
+-rw-r--r--   0        0        0     2731 1970-01-01 00:00:00.000000 odd_great_expectations-0.2.1/PKG-INFO
```

### Comparing `odd_great_expectations-0.2.0/LICENSE` & `odd_great_expectations-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `odd_great_expectations-0.2.0/README.md` & `odd_great_expectations-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `odd_great_expectations-0.2.0/odd_great_expectations/action.py` & `odd_great_expectations-0.2.1/odd_great_expectations/action.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import traceback
 from typing import Union, Optional
 
+from great_expectations.core import ExpectationSuiteValidationResult
+
 from great_expectations.checkpoint.actions import (
-    ExpectationSuiteValidationResult,
     GXCloudIdentifier,
     ValidationAction,
     ValidationResultIdentifier,
 )
 from great_expectations.validator.validator import Validator
 from oddrn_generator.generators import GreatExpectationsGenerator
```

### Comparing `odd_great_expectations-0.2.0/odd_great_expectations/dataset/file.py` & `odd_great_expectations-0.2.1/odd_great_expectations/dataset/file.py`

 * *Files identical despite different names*

### Comparing `odd_great_expectations-0.2.0/odd_great_expectations/dataset/get_dataset.py` & `odd_great_expectations-0.2.1/odd_great_expectations/dataset/get_dataset.py`

 * *Files identical despite different names*

### Comparing `odd_great_expectations-0.2.0/odd_great_expectations/dataset/sql_table.py` & `odd_great_expectations-0.2.1/odd_great_expectations/dataset/sql_table.py`

 * *Files identical despite different names*

### Comparing `odd_great_expectations-0.2.0/odd_great_expectations/mapper.py` & `odd_great_expectations-0.2.1/odd_great_expectations/mapper.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 import datetime
 from typing import Any, Optional, Tuple
 
+from great_expectations.core import ExpectationSuiteValidationResult
+
 from funcy import lmapcat
 from great_expectations.checkpoint.actions import (
-    ExpectationSuiteValidationResult,
     ValidationResultIdentifier,
 )
 from great_expectations.core import ExpectationConfiguration
 from great_expectations.expectations.registry import get_expectation_impl
 from great_expectations.validator.validator import ExpectationValidationResult
 from odd_models.models import (
     DataEntity,
     DataEntityList,
     DataEntityType,
     DataQualityTest,
     DataQualityTestExpectation,
+    DataQualityTestExpectationCategory,
     DataQualityTestRun,
     LinkedUrl,
     QualityRunStatus,
 )
 from oddrn_generator.generators import GreatExpectationsGenerator
 
 
@@ -82,15 +84,17 @@
         if self._docs_link and not self._docs_link.startswith("file://"):
             linked_url_list = [LinkedUrl(name="docs", url=self._docs_link)]
 
         dqt = DataQualityTest(
             suite_name=suite_name,
             dataset_list=self._datasets,
             expectation=DataQualityTestExpectation(
-                type=original_type, **flat_kwargs(config.kwargs)
+                type=original_type,
+                category=DataQualityTestExpectationCategory.ASSERTION,
+                **flat_kwargs(config.kwargs)
             ),
             linked_url_list=linked_url_list,
         )
 
         return DataEntity(
             oddrn=oddrn,
             name=f"{suite_name}:{original_type}",
```

### Comparing `odd_great_expectations-0.2.0/pyproject.toml` & `odd_great_expectations-0.2.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [tool.poetry]
 name = "odd-great-expectations"
-version = "0.2.0"
+version = "0.2.1"
 description = "OpenDataDiscovery Action for Great Expectations"
 authors = ["Pavel Makarichev <vixtir90@gmail.com>"]
 readme = "README.md"
 license = "Apache-2.0"
 keywords = ['Open Data Discovery', 'Great Expectations', "Metadata", "Data Discovery", "Data Observability"]
 packages = [{include = "odd_great_expectations"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-odd-models = "2.0.17"
+odd-models = "2.0.47"
 oddrn-generator = "^0.1.68"
-great-expectations = "^0.15.44"
-funcy = "^1.17"
+great-expectations = "^0.18.12"
+funcy = "^2.0"
 sqlalchemy = "^1.4.46"
-psycopg2 = "^2.9.5"
-loguru = "^0.6.0"
+psycopg2-binary = "^2.9.5"
+loguru = "^0.7.2"
 
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.12.0"
 isort = "^5.11.4"
 
 [build-system]
```

### Comparing `odd_great_expectations-0.2.0/setup.py` & `odd_great_expectations-0.2.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 packages = \
 ['odd_great_expectations', 'odd_great_expectations.dataset']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['funcy>=1.17,<2.0',
- 'great-expectations>=0.15.44,<0.16.0',
- 'loguru>=0.6.0,<0.7.0',
- 'odd-models==2.0.17',
+['funcy>=2.0,<3.0',
+ 'great-expectations>=0.18.12,<0.19.0',
+ 'loguru>=0.7.2,<0.8.0',
+ 'odd-models==2.0.47',
  'oddrn-generator>=0.1.68,<0.2.0',
- 'psycopg2>=2.9.5,<3.0.0',
+ 'psycopg2-binary>=2.9.5,<3.0.0',
  'sqlalchemy>=1.4.46,<2.0.0']
 
 setup_kwargs = {
     'name': 'odd-great-expectations',
-    'version': '0.2.0',
+    'version': '0.2.1',
     'description': 'OpenDataDiscovery Action for Great Expectations',
     'long_description': "## OpenDataDiscovery Action for handling Great Expectations tests results.\n\n[![PyPI version](https://badge.fury.io/py/odd-great-expectations.svg)](https://badge.fury.io/py/odd-great-expectations)\n\n![image](assets/screenshot.png)\n\n# What is it?\n`odd_great_expectation.action.ODDAction`\nIs a class derived from GX `ValidationAction` which will be run by GreatExpectations at runtime with `ValidationResult`s for checkpoint.\n\n\n# How to use it?:\nInstall `odd-great-expectations` package\n```bash\npip install odd-great-expectations\n```\nAdd `ODDAction` action to some checkpoint's action list:\n```yaml\nname: <CHECKPOINT_NAME>\nconfig_version: 1.0\n...\naction_list:\n  # other actions\n  - name: store_metadata_to_odd\n    action:\n      module_name: odd_great_expectations.action\n      class_name: ODDAction\n      platform_host: <PLATFORM_HOST>\n      data_source_name: <DATA_SOURCE_NAME>\n```\n\nParameters:\n\n`platform_host` - Location of OpenDataDiscovery platform, i.e. http://localhost:8080\n\n`platform_token` - OpenDataDiscovery token, how to get it - https://docs.opendatadiscovery.org/configuration-and-deployment/trylocally#create-collector-entity\n\n`data_source_name` - Unique name for data source, i.e. local_qa_test\n\nBoth `platform_host` and `platform_token`  can be set using `ODD_PLATFORM_HOST` and `ODD_PLATFORM_PLATFORM` env variables accordingly.\n\nRun checkpoint\n```bash\ngreat_expectations checkpoint run <CHECKPOINT_NAME>\n```\nCheck results on `PLATFORM_HOST` UI.\n\n## Supporting features\n| Feature                     | Supporting |\n| --------------------------- | ---------- |\n| V3 API +                    | +          |\n| SqlAlchemyEngine            | +          |\n| PandasEngine                | +          |\n| Great Expectations V2 API - | -          |\n| Cloud Solution              | -          |\n",
     'author': 'Pavel Makarichev',
     'author_email': 'vixtir90@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `odd_great_expectations-0.2.0/PKG-INFO` & `odd_great_expectations-0.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: odd-great-expectations
-Version: 0.2.0
+Version: 0.2.1
 Summary: OpenDataDiscovery Action for Great Expectations
 License: Apache-2.0
 Keywords: Open Data Discovery,Great Expectations,Metadata,Data Discovery,Data Observability
 Author: Pavel Makarichev
 Author-email: vixtir90@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: funcy (>=1.17,<2.0)
-Requires-Dist: great-expectations (>=0.15.44,<0.16.0)
-Requires-Dist: loguru (>=0.6.0,<0.7.0)
-Requires-Dist: odd-models (==2.0.17)
+Requires-Dist: funcy (>=2.0,<3.0)
+Requires-Dist: great-expectations (>=0.18.12,<0.19.0)
+Requires-Dist: loguru (>=0.7.2,<0.8.0)
+Requires-Dist: odd-models (==2.0.47)
 Requires-Dist: oddrn-generator (>=0.1.68,<0.2.0)
-Requires-Dist: psycopg2 (>=2.9.5,<3.0.0)
+Requires-Dist: psycopg2-binary (>=2.9.5,<3.0.0)
 Requires-Dist: sqlalchemy (>=1.4.46,<2.0.0)
 Description-Content-Type: text/markdown
 
 ## OpenDataDiscovery Action for handling Great Expectations tests results.
 
 [![PyPI version](https://badge.fury.io/py/odd-great-expectations.svg)](https://badge.fury.io/py/odd-great-expectations)
```

