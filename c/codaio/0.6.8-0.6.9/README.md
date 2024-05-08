# Comparing `tmp/codaio-0.6.8.tar.gz` & `tmp/codaio-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codaio-0.6.8.tar", max compression
+gzip compressed data, was "codaio-0.6.9.tar", max compression
```

## Comparing `codaio-0.6.8.tar` & `codaio-0.6.9.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     5843 2021-06-16 15:47:45.647935 codaio-0.6.8/README.md
--rw-r--r--   0        0        0       67 2021-06-16 15:47:45.647935 codaio-0.6.8/codaio/__init__.py
--rw-r--r--   0        0        0    40221 2021-06-16 15:47:45.647935 codaio-0.6.8/codaio/coda.py
--rw-r--r--   0        0        0      411 2021-06-16 15:47:45.647935 codaio-0.6.8/codaio/err.py
--rw-r--r--   0        0        0      990 2021-06-16 15:47:45.647935 codaio-0.6.8/pyproject.toml
--rw-r--r--   0        0        0     6900 2021-06-16 15:47:53.235333 codaio-0.6.8/setup.py
--rw-r--r--   0        0        0     6670 2021-06-16 15:47:53.235918 codaio-0.6.8/PKG-INFO
+-rw-r--r--   0        0        0     5968 2021-12-05 20:14:33.538631 codaio-0.6.9/README.md
+-rw-r--r--   0        0        0       67 2021-12-05 20:14:33.538631 codaio-0.6.9/codaio/__init__.py
+-rw-r--r--   0        0        0    40221 2021-12-05 20:14:33.538631 codaio-0.6.9/codaio/coda.py
+-rw-r--r--   0        0        0      411 2021-12-05 20:14:33.538631 codaio-0.6.9/codaio/err.py
+-rw-r--r--   0        0        0      990 2021-12-05 20:14:33.542631 codaio-0.6.9/pyproject.toml
+-rw-r--r--   0        0        0     7033 2021-12-05 20:14:46.249206 codaio-0.6.9/setup.py
+-rw-r--r--   0        0        0     6846 2021-12-05 20:14:46.250043 codaio-0.6.9/PKG-INFO
```

### Comparing `codaio-0.6.8/README.md` & `codaio-0.6.9/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -8,23 +8,31 @@
 ![PyPI - Downloads](https://img.shields.io/pypi/dw/codaio)
 [![](https://img.shields.io/badge/Support-Buy_coffee!-Orange)](https://www.buymeacoffee.com/licht1stein)
 
 `codaio` is in active development stage. Issues and PRs very welcome! 
 
 
 ### Installation
+Install with [poetry](https://python-poetry.org/) (always recommended):
+
+```shell script
+poetry add codaio
+```
+
+or with `pip`
+
 ```shell script
 pip install codaio
 ```
 
 ### Config via environment variables
 The following variables will be called from environment where applicable:
 
 * `CODA_API_ENDPOINT` (default value `https://coda.io/apis/v1`)
-* `CODA_API_KEY` - your API key to use when initializing document from environment
+* `CODA_API_KEY` - your API key to use when initializing client from environment
 
 ### Quickstart using raw API
 Coda class provides a wrapper for all API methods. If API response included a JSON it will be returned as a dictionary from all methods. If it didn't a dictionary `{"status": response.status_code}` will be returned.
 If request wasn't successful a `CodaError` will be raised with details of the API error.
 
 ```python
 from codaio import Coda
```

### Comparing `codaio-0.6.8/codaio/coda.py` & `codaio-0.6.9/codaio/coda.py`

 * *Files identical despite different names*

### Comparing `codaio-0.6.8/pyproject.toml` & `codaio-0.6.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "codaio"
-version = "0.6.8"
+version = "0.6.9"
 description = "Python wrapper for Coda.io API"
 authors = ["MB <mb@blaster.ai>"]
 license = "MIT"
 readme='README.md'
 homepage='https://github.com/Blasterai/codaio'
 documentation='https://codaio.readthedocs.io/en/latest/index.html'
```

### Comparing `codaio-0.6.8/setup.py` & `codaio-0.6.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,17 +13,17 @@
  'envparse>=0.2.0,<0.3.0',
  'inflection>=0.3.1,<0.4.0',
  'python-dateutil>=2.8,<3.0',
  'requests>=2.22,<3.0']
 
 setup_kwargs = {
     'name': 'codaio',
-    'version': '0.6.8',
+    'version': '0.6.9',
     'description': 'Python wrapper for Coda.io API',
-    'long_description': '## Python wrapper for [Coda.io](https://coda.io) API\n\n[![CodaAPI](https://img.shields.io/badge/Coda_API_-V1-green)](https://coda.io/developers/apis/v1beta1)\n![PyPI - Python Version](https://img.shields.io/pypi/pyversions/codaio)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n[![Documentation Status](https://readthedocs.org/projects/codaio/badge/?version=latest)](https://codaio.readthedocs.io/en/latest/?badge=latest)\n[![PyPI](https://img.shields.io/pypi/v/codaio)](https://pypi.org/project/codaio/)\n![PyPI - Downloads](https://img.shields.io/pypi/dw/codaio)\n[![](https://img.shields.io/badge/Support-Buy_coffee!-Orange)](https://www.buymeacoffee.com/licht1stein)\n\n`codaio` is in active development stage. Issues and PRs very welcome! \n\n\n### Installation\n```shell script\npip install codaio\n```\n\n### Config via environment variables\nThe following variables will be called from environment where applicable:\n\n* `CODA_API_ENDPOINT` (default value `https://coda.io/apis/v1`)\n* `CODA_API_KEY` - your API key to use when initializing document from environment\n\n### Quickstart using raw API\nCoda class provides a wrapper for all API methods. If API response included a JSON it will be returned as a dictionary from all methods. If it didn\'t a dictionary `{"status": response.status_code}` will be returned.\nIf request wasn\'t successful a `CodaError` will be raised with details of the API error.\n\n```python\nfrom codaio import Coda\n\ncoda = Coda(\'YOUR_API_KEY\')\n\n>>> coda.create_doc(\'My Document\')\n{\'id\': \'NEW_DOC_ID\', \'type\': \'doc\', \'href\': \'https://coda.io/apis/v1/docs/NEW_DOC_ID\', \'browserLink\': \'https://coda.io/d/_dNEW_DOC_ID\', \'name\': \'My Document\', \'owner\': \'your@email\', \'ownerName\': \'Your Name\', \'createdAt\': \'2020-09-28T19:32:20.866Z\', \'updatedAt\': \'2020-09-28T19:32:20.924Z\'}\n```\nFor full API reference for Coda class see [documentation](https://codaio.readthedocs.io/en/latest/index.html#codaio.Coda)\n\n### Quickstart using codaio objects\n\n`codaio` implements convenient classes to work with Coda documents: `Document`, `Table`, `Row`, `Column` and `Cell`.\n\n```python\nfrom codaio import Coda, Document\n\n# Initialize by providing a coda object directly\ncoda = Coda(\'YOUR_API_KEY\')\n\ndoc = Document(\'YOUR_DOC_ID\', coda=coda)\n\n# Or initialiaze from environment by storing your API key in environment variable `CODA_API_KEY`\ndoc = Document.from_environment(\'YOUR_DOC_ID\')\n\ndoc.list_tables()\n\ntable = doc.get_table(\'TABLE_ID\')\n```\n#### Fetching a Row\n```python\n# You can fetch a row by ID\nrow  = table[\'ROW_ID\']\n```\n\n#### Using with Pandas\nIf you want to load a codaio Table or Row into pandas, you can use the `Table.to_dict()` or `Row.to_dict()` methods:\n```python\nimport pandas as pd\n\ndf = pd.DataFrame(table.to_dict())\n```\n\n#### Fetching a Cell\n```python\n# Or fetch a cell by ROW_ID and COLUMN_ID\ncell = table[\'ROW_ID\'][\'COLUMN_ID\']  \n\n# This is equivalent to getting item from a row\ncell = row[\'COLUMN_ID\']\n# or \ncell = row[\'COLUMN_NAME\']  # This should work fine if COLUMN_NAME is unique, otherwise it will raise AmbiguousColumn error\n# or use a Column instance\ncell = row[column]\n```\n\n#### Changing Cell value\n\n```python\nrow[\'COLUMN_ID\'] = \'foo\'\n# or\nrow[\'Column Name\'] = \'foo\'\n```\n\n#### Iterating over rows\n```python\n# Iterate over rows using IDs -> delete rows that match a condition\nfor row in table.rows():\n    if row[\'COLUMN_ID\'] == \'foo\':\n        row.delete()\n\n# Iterate over rows using names -> edit cells in rows that match a condition\nfor row in table.rows():\n    if row[\'Name\'] == \'bar\':\n        row[\'Value\'] = \'spam\'\n```\n\n#### Upserting new row\nTo upsert a new row you can pass a list of cells to `table.upsert_row()`\n```python\nname_cell = Cell(column=\'COLUMN_ID\', value_storage=\'new_name\')\nvalue_cell = Cell(column=\'COLUMN_ID\', value_storage=\'new_value\')\n\ntable.upsert_row([name_cell, value_cell])\n```\n\n#### Upserting multiple new rows\nWorks like upserting one row, except you pass a list of lists to `table.upsert_rows()` (rows, not row)\n```python\nname_cell_a = Cell(column=\'COLUMN_ID\', value_storage=\'new_name\')\nvalue_cell_a = Cell(column=\'COLUMN_ID\', value_storage=\'new_value\')\n\nname_cell_b = Cell(column=\'COLUMN_ID\', value_storage=\'new_name\')\nvalue_cell_b = Cell(column=\'COLUMN_ID\', value_storage=\'new_value\')\n\ntable.upsert_rows([[name_cell_a, value_cell_a], [name_cell_b, value_cell_b]])\n```\n\n#### Updating a row\nTo update a row use `table.update_row(row, cells)`\n```python\nrow = table[\'ROW_ID\']\n\nname_cell_a = Cell(column=\'COLUMN_ID\', value_storage=\'new_name\')\nvalue_cell_a = Cell(column=\'COLUMN_ID\', value_storage=\'new_value\')\n\ntable.update_row(row, [name_cell_a, value_cell_a])\n```\n\n### Documentation\n\n`codaio` documentation lives at [readthedocs.io](https://codaio.readthedocs.io/en/latest/index.html)\n\n### Running the tests\n\nThe recommended way of running the test suite is to use [nox](https://nox.thea.codes/en/stable/tutorial.html).\n\nOnce `nox`: is installed, just run the following command:\n```shell script\nnox\n```\n\nThe nox session will run the test suite against python 3.8 and 3.7. It will also look for linting errors with `flake8`.\n\nYou can still invoke `pytest` directly with:\n```shell script\npoetry run pytest --cov\n```\n\nCheck out the fixtures if you want to improve the testing process.\n\n\n#### Contributing\n\nIf you are willing to contribute please go ahead, we can use some help!\n\n##### Using CI to deploy to PyPi\n\nWhen a PR is merged to master the CI will try to deploy to pypi.org using poetry. It will succeed only if the \nversion number changed in pyproject.toml. \n\nTo do so use poetry\'s [version command](https://python-poetry.org/docs/cli/#version). For example:\n\nBump 0.4.11 to 0.4.12:\n```bash\npoetry version patch\n```\n\nBump 0.4.11 to 0.5.0:\n```bash\npoetry version minor\n```\n\nBump 0.4.11 to 1.0.0:\n```bash\npoetry version major\n```\n',
+    'long_description': '## Python wrapper for [Coda.io](https://coda.io) API\n\n[![CodaAPI](https://img.shields.io/badge/Coda_API_-V1-green)](https://coda.io/developers/apis/v1beta1)\n![PyPI - Python Version](https://img.shields.io/pypi/pyversions/codaio)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n[![Documentation Status](https://readthedocs.org/projects/codaio/badge/?version=latest)](https://codaio.readthedocs.io/en/latest/?badge=latest)\n[![PyPI](https://img.shields.io/pypi/v/codaio)](https://pypi.org/project/codaio/)\n![PyPI - Downloads](https://img.shields.io/pypi/dw/codaio)\n[![](https://img.shields.io/badge/Support-Buy_coffee!-Orange)](https://www.buymeacoffee.com/licht1stein)\n\n`codaio` is in active development stage. Issues and PRs very welcome! \n\n\n### Installation\nInstall with [poetry](https://python-poetry.org/) (always recommended):\n\n```shell script\npoetry add codaio\n```\n\nor with `pip`\n\n```shell script\npip install codaio\n```\n\n### Config via environment variables\nThe following variables will be called from environment where applicable:\n\n* `CODA_API_ENDPOINT` (default value `https://coda.io/apis/v1`)\n* `CODA_API_KEY` - your API key to use when initializing client from environment\n\n### Quickstart using raw API\nCoda class provides a wrapper for all API methods. If API response included a JSON it will be returned as a dictionary from all methods. If it didn\'t a dictionary `{"status": response.status_code}` will be returned.\nIf request wasn\'t successful a `CodaError` will be raised with details of the API error.\n\n```python\nfrom codaio import Coda\n\ncoda = Coda(\'YOUR_API_KEY\')\n\n>>> coda.create_doc(\'My Document\')\n{\'id\': \'NEW_DOC_ID\', \'type\': \'doc\', \'href\': \'https://coda.io/apis/v1/docs/NEW_DOC_ID\', \'browserLink\': \'https://coda.io/d/_dNEW_DOC_ID\', \'name\': \'My Document\', \'owner\': \'your@email\', \'ownerName\': \'Your Name\', \'createdAt\': \'2020-09-28T19:32:20.866Z\', \'updatedAt\': \'2020-09-28T19:32:20.924Z\'}\n```\nFor full API reference for Coda class see [documentation](https://codaio.readthedocs.io/en/latest/index.html#codaio.Coda)\n\n### Quickstart using codaio objects\n\n`codaio` implements convenient classes to work with Coda documents: `Document`, `Table`, `Row`, `Column` and `Cell`.\n\n```python\nfrom codaio import Coda, Document\n\n# Initialize by providing a coda object directly\ncoda = Coda(\'YOUR_API_KEY\')\n\ndoc = Document(\'YOUR_DOC_ID\', coda=coda)\n\n# Or initialiaze from environment by storing your API key in environment variable `CODA_API_KEY`\ndoc = Document.from_environment(\'YOUR_DOC_ID\')\n\ndoc.list_tables()\n\ntable = doc.get_table(\'TABLE_ID\')\n```\n#### Fetching a Row\n```python\n# You can fetch a row by ID\nrow  = table[\'ROW_ID\']\n```\n\n#### Using with Pandas\nIf you want to load a codaio Table or Row into pandas, you can use the `Table.to_dict()` or `Row.to_dict()` methods:\n```python\nimport pandas as pd\n\ndf = pd.DataFrame(table.to_dict())\n```\n\n#### Fetching a Cell\n```python\n# Or fetch a cell by ROW_ID and COLUMN_ID\ncell = table[\'ROW_ID\'][\'COLUMN_ID\']  \n\n# This is equivalent to getting item from a row\ncell = row[\'COLUMN_ID\']\n# or \ncell = row[\'COLUMN_NAME\']  # This should work fine if COLUMN_NAME is unique, otherwise it will raise AmbiguousColumn error\n# or use a Column instance\ncell = row[column]\n```\n\n#### Changing Cell value\n\n```python\nrow[\'COLUMN_ID\'] = \'foo\'\n# or\nrow[\'Column Name\'] = \'foo\'\n```\n\n#### Iterating over rows\n```python\n# Iterate over rows using IDs -> delete rows that match a condition\nfor row in table.rows():\n    if row[\'COLUMN_ID\'] == \'foo\':\n        row.delete()\n\n# Iterate over rows using names -> edit cells in rows that match a condition\nfor row in table.rows():\n    if row[\'Name\'] == \'bar\':\n        row[\'Value\'] = \'spam\'\n```\n\n#### Upserting new row\nTo upsert a new row you can pass a list of cells to `table.upsert_row()`\n```python\nname_cell = Cell(column=\'COLUMN_ID\', value_storage=\'new_name\')\nvalue_cell = Cell(column=\'COLUMN_ID\', value_storage=\'new_value\')\n\ntable.upsert_row([name_cell, value_cell])\n```\n\n#### Upserting multiple new rows\nWorks like upserting one row, except you pass a list of lists to `table.upsert_rows()` (rows, not row)\n```python\nname_cell_a = Cell(column=\'COLUMN_ID\', value_storage=\'new_name\')\nvalue_cell_a = Cell(column=\'COLUMN_ID\', value_storage=\'new_value\')\n\nname_cell_b = Cell(column=\'COLUMN_ID\', value_storage=\'new_name\')\nvalue_cell_b = Cell(column=\'COLUMN_ID\', value_storage=\'new_value\')\n\ntable.upsert_rows([[name_cell_a, value_cell_a], [name_cell_b, value_cell_b]])\n```\n\n#### Updating a row\nTo update a row use `table.update_row(row, cells)`\n```python\nrow = table[\'ROW_ID\']\n\nname_cell_a = Cell(column=\'COLUMN_ID\', value_storage=\'new_name\')\nvalue_cell_a = Cell(column=\'COLUMN_ID\', value_storage=\'new_value\')\n\ntable.update_row(row, [name_cell_a, value_cell_a])\n```\n\n### Documentation\n\n`codaio` documentation lives at [readthedocs.io](https://codaio.readthedocs.io/en/latest/index.html)\n\n### Running the tests\n\nThe recommended way of running the test suite is to use [nox](https://nox.thea.codes/en/stable/tutorial.html).\n\nOnce `nox`: is installed, just run the following command:\n```shell script\nnox\n```\n\nThe nox session will run the test suite against python 3.8 and 3.7. It will also look for linting errors with `flake8`.\n\nYou can still invoke `pytest` directly with:\n```shell script\npoetry run pytest --cov\n```\n\nCheck out the fixtures if you want to improve the testing process.\n\n\n#### Contributing\n\nIf you are willing to contribute please go ahead, we can use some help!\n\n##### Using CI to deploy to PyPi\n\nWhen a PR is merged to master the CI will try to deploy to pypi.org using poetry. It will succeed only if the \nversion number changed in pyproject.toml. \n\nTo do so use poetry\'s [version command](https://python-poetry.org/docs/cli/#version). For example:\n\nBump 0.4.11 to 0.4.12:\n```bash\npoetry version patch\n```\n\nBump 0.4.11 to 0.5.0:\n```bash\npoetry version minor\n```\n\nBump 0.4.11 to 1.0.0:\n```bash\npoetry version major\n```\n',
     'author': 'MB',
     'author_email': 'mb@blaster.ai',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/Blasterai/codaio',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `codaio-0.6.8/PKG-INFO` & `codaio-0.6.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: codaio
-Version: 0.6.8
+Version: 0.6.9
 Summary: Python wrapper for Coda.io API
 Home-page: https://github.com/Blasterai/codaio
 License: MIT
 Author: MB
 Author-email: mb@blaster.ai
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: attrs (>=19.1,<20.0)
 Requires-Dist: decorator (>=4.4,<5.0)
 Requires-Dist: envparse (>=0.2.0,<0.3.0)
 Requires-Dist: inflection (>=0.3.1,<0.4.0)
@@ -31,23 +32,31 @@
 ![PyPI - Downloads](https://img.shields.io/pypi/dw/codaio)
 [![](https://img.shields.io/badge/Support-Buy_coffee!-Orange)](https://www.buymeacoffee.com/licht1stein)
 
 `codaio` is in active development stage. Issues and PRs very welcome! 
 
 
 ### Installation
+Install with [poetry](https://python-poetry.org/) (always recommended):
+
+```shell script
+poetry add codaio
+```
+
+or with `pip`
+
 ```shell script
 pip install codaio
 ```
 
 ### Config via environment variables
 The following variables will be called from environment where applicable:
 
 * `CODA_API_ENDPOINT` (default value `https://coda.io/apis/v1`)
-* `CODA_API_KEY` - your API key to use when initializing document from environment
+* `CODA_API_KEY` - your API key to use when initializing client from environment
 
 ### Quickstart using raw API
 Coda class provides a wrapper for all API methods. If API response included a JSON it will be returned as a dictionary from all methods. If it didn't a dictionary `{"status": response.status_code}` will be returned.
 If request wasn't successful a `CodaError` will be raised with details of the API error.
 
 ```python
 from codaio import Coda
```

