# Comparing `tmp/narwhals-0.8.0.tar.gz` & `tmp/narwhals-0.8.1.tar.gz`

## Comparing `narwhals-0.8.0.tar` & `narwhals-0.8.1.tar`

### file list

```diff
@@ -1,113 +1,116 @@
--rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 narwhals-0.8.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 narwhals-0.8.0/CONTRIBUTING.md
--rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 narwhals-0.8.0/mkdocs.yml
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 narwhals-0.8.0/requirements-dev.txt
--rw-r--r--   0        0        0     5243 2020-02-02 00:00:00.000000 narwhals-0.8.0/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     3725 2020-02-02 00:00:00.000000 narwhals-0.8.0/.github/workflows/extremes.yml
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 narwhals-0.8.0/.github/workflows/mkdocs.yml
--rw-r--r--   0        0        0     2638 2020-02-02 00:00:00.000000 narwhals-0.8.0/.github/workflows/publish_to_pypi.yml
--rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 narwhals-0.8.0/.github/workflows/pytest.yml
--rw-r--r--   0        0        0     2021 2020-02-02 00:00:00.000000 narwhals-0.8.0/docs/extending.md
--rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 narwhals-0.8.0/docs/generate_members.py
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 narwhals-0.8.0/docs/index.md
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 narwhals-0.8.0/docs/installation.md
--rw-r--r--   0        0        0     1245 2020-02-02 00:00:00.000000 narwhals-0.8.0/docs/quick_start.md
--rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 narwhals-0.8.0/docs/related.md
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 narwhals-0.8.0/docs/requirements-docs.txt
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 narwhals-0.8.0/docs/roadmap.md
--rw-r--r--   0        0        0     1281 2020-02-02 00:00:00.000000 narwhals-0.8.0/docs/why.md
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 narwhals-0.8.0/docs/api-reference/dataframe.md
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 narwhals-0.8.0/docs/api-reference/dependencies.md
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 narwhals-0.8.0/docs/api-reference/dtypes.md
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 narwhals-0.8.0/docs/api-reference/expressions.md
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 narwhals-0.8.0/docs/api-reference/expressions_dt.md
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 narwhals-0.8.0/docs/api-reference/expressions_str.md
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 narwhals-0.8.0/docs/api-reference/index.md
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 narwhals-0.8.0/docs/api-reference/lazyframe.md
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 narwhals-0.8.0/docs/api-reference/narwhals.md
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 narwhals-0.8.0/docs/api-reference/series.md
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 narwhals-0.8.0/docs/api-reference/series_dt.md
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 narwhals-0.8.0/docs/api-reference/series_str.md
--rwxr-xr-x   0        0        0   132699 2020-02-02 00:00:00.000000 narwhals-0.8.0/docs/assets/image.png
--rw-r--r--   0        0        0     4468 2020-02-02 00:00:00.000000 narwhals-0.8.0/docs/basics/column.md
--rw-r--r--   0        0        0     3572 2020-02-02 00:00:00.000000 narwhals-0.8.0/docs/basics/complete_example.md
--rw-r--r--   0        0        0     4278 2020-02-02 00:00:00.000000 narwhals-0.8.0/docs/basics/dataframe.md
--rw-r--r--   0        0        0     2523 2020-02-02 00:00:00.000000 narwhals-0.8.0/docs/other/pandas_index.md
--rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 narwhals-0.8.0/narwhals/__init__.py
--rw-r--r--   0        0        0    90926 2020-02-02 00:00:00.000000 narwhals-0.8.0/narwhals/dataframe.py
--rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 narwhals-0.8.0/narwhals/dependencies.py
--rw-r--r--   0        0        0     2791 2020-02-02 00:00:00.000000 narwhals-0.8.0/narwhals/dtypes.py
--rw-r--r--   0        0        0    25221 2020-02-02 00:00:00.000000 narwhals-0.8.0/narwhals/expression.py
--rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 narwhals-0.8.0/narwhals/functions.py
--rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 narwhals-0.8.0/narwhals/group_by.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.0/narwhals/py.typed
--rw-r--r--   0        0        0     6572 2020-02-02 00:00:00.000000 narwhals-0.8.0/narwhals/series.py
--rw-r--r--   0        0        0     7100 2020-02-02 00:00:00.000000 narwhals-0.8.0/narwhals/translate.py
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 narwhals-0.8.0/narwhals/typing.py
--rw-r--r--   0        0        0     2268 2020-02-02 00:00:00.000000 narwhals-0.8.0/narwhals/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.0/narwhals/_pandas_like/__init__.py
--rw-r--r--   0        0        0     7838 2020-02-02 00:00:00.000000 narwhals-0.8.0/narwhals/_pandas_like/dataframe.py
--rw-r--r--   0        0        0     9787 2020-02-02 00:00:00.000000 narwhals-0.8.0/narwhals/_pandas_like/expr.py
--rw-r--r--   0        0        0     5640 2020-02-02 00:00:00.000000 narwhals-0.8.0/narwhals/_pandas_like/group_by.py
--rw-r--r--   0        0        0     6324 2020-02-02 00:00:00.000000 narwhals-0.8.0/narwhals/_pandas_like/namespace.py
--rw-r--r--   0        0        0    14369 2020-02-02 00:00:00.000000 narwhals-0.8.0/narwhals/_pandas_like/series.py
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 narwhals-0.8.0/narwhals/_pandas_like/typing.py
--rw-r--r--   0        0        0    13436 2020-02-02 00:00:00.000000 narwhals-0.8.0/narwhals/_pandas_like/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.0/tests/__init__.py
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 narwhals-0.8.0/tests/conftest.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.0/tests/group_by_test.py
--rw-r--r--   0        0        0    22181 2020-02-02 00:00:00.000000 narwhals-0.8.0/tests/test_common.py
--rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 narwhals-0.8.0/tests/test_dt.py
--rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 narwhals-0.8.0/tests/test_group_by.py
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 narwhals-0.8.0/tests/test_invalid.py
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 narwhals-0.8.0/tests/test_pandas.py
--rw-r--r--   0        0        0     8935 2020-02-02 00:00:00.000000 narwhals-0.8.0/tests/test_series.py
--rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 narwhals-0.8.0/tests/test_str.py
--rw-r--r--   0        0        0     7276 2020-02-02 00:00:00.000000 narwhals-0.8.0/tests/tpch_q1_test.py
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 narwhals-0.8.0/tests/utils.py
--rw-r--r--   0        0        0    21551 2020-02-02 00:00:00.000000 narwhals-0.8.0/tests/data/customer.parquet
--rw-r--r--   0        0        0    34095 2020-02-02 00:00:00.000000 narwhals-0.8.0/tests/data/lineitem.parquet
--rw-r--r--   0        0        0     2139 2020-02-02 00:00:00.000000 narwhals-0.8.0/tests/data/nation.parquet
--rw-r--r--   0        0        0    24714 2020-02-02 00:00:00.000000 narwhals-0.8.0/tests/data/orders.parquet
--rw-r--r--   0        0        0    13276 2020-02-02 00:00:00.000000 narwhals-0.8.0/tests/data/part.parquet
--rw-r--r--   0        0        0    14921 2020-02-02 00:00:00.000000 narwhals-0.8.0/tests/data/partsupp.parquet
--rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 narwhals-0.8.0/tests/data/region.parquet
--rw-r--r--   0        0        0    19817 2020-02-02 00:00:00.000000 narwhals-0.8.0/tests/data/supplier.parquet
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.0/tests/expr/__init__.py
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 narwhals-0.8.0/tests/expr/test_to_datetime.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.0/tests/hypothesis/__init__.py
--rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 narwhals-0.8.0/tests/hypothesis/test_basic_arithmetic.py
--rw-r--r--   0        0        0     1897 2020-02-02 00:00:00.000000 narwhals-0.8.0/tests/hypothesis/test_concat.py
--rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 narwhals-0.8.0/tests/hypothesis/test_join.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.0/tpch/__init__.py
--rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 narwhals-0.8.0/tpch/q1.py
--rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 narwhals-0.8.0/tpch/q2.py
--rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 narwhals-0.8.0/tpch/q3.py
--rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 narwhals-0.8.0/tpch/q4.py
--rw-r--r--   0        0        0     2900 2020-02-02 00:00:00.000000 narwhals-0.8.0/tpch/q5.py
--rwxr-xr-x   0        0        0    47336 2020-02-02 00:00:00.000000 narwhals-0.8.0/tpch/notebooks/gpu/execute.ipynb
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 narwhals-0.8.0/tpch/notebooks/gpu/kernel-metadata.json
--rwxr-xr-x   0        0        0    17860 2020-02-02 00:00:00.000000 narwhals-0.8.0/tpch/notebooks/q1/execute.ipynb
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.8.0/tpch/notebooks/q1/kernel-metadata.json
--rwxr-xr-x   0        0        0    18811 2020-02-02 00:00:00.000000 narwhals-0.8.0/tpch/notebooks/q2/execute.ipynb
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.8.0/tpch/notebooks/q2/kernel-metadata.json
--rwxr-xr-x   0        0        0    17692 2020-02-02 00:00:00.000000 narwhals-0.8.0/tpch/notebooks/q3/execute.ipynb
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.8.0/tpch/notebooks/q3/kernel-metadata.json
--rwxr-xr-x   0        0        0    16689 2020-02-02 00:00:00.000000 narwhals-0.8.0/tpch/notebooks/q4/execute.ipynb
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.8.0/tpch/notebooks/q4/kernel-metadata.json
--rwxr-xr-x   0        0        0    18235 2020-02-02 00:00:00.000000 narwhals-0.8.0/tpch/notebooks/q5/execute.ipynb
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.8.0/tpch/notebooks/q5/kernel-metadata.json
--rwxr-xr-x   0        0        0    16156 2020-02-02 00:00:00.000000 narwhals-0.8.0/tpch/notebooks/q6/execute.ipynb
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.8.0/tpch/notebooks/q6/kernel-metadata.json
--rwxr-xr-x   0        0        0    27860 2020-02-02 00:00:00.000000 narwhals-0.8.0/tpch/notebooks/q7/execute.ipynb
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.8.0/tpch/notebooks/q7/kernel-metadata.json
--rwxr-xr-x   0        0        0    27709 2020-02-02 00:00:00.000000 narwhals-0.8.0/tpch/notebooks/q8/execute.ipynb
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.8.0/tpch/notebooks/q8/kernel-metadata.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.0/utils/__init__.py
--rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 narwhals-0.8.0/utils/bump_version.py
--rw-r--r--   0        0        0     4142 2020-02-02 00:00:00.000000 narwhals-0.8.0/utils/check_api_reference.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 narwhals-0.8.0/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 narwhals-0.8.0/LICENSE.md
--rw-r--r--   0        0        0     3229 2020-02-02 00:00:00.000000 narwhals-0.8.0/README.md
--rw-r--r--   0        0        0     1995 2020-02-02 00:00:00.000000 narwhals-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     3958 2020-02-02 00:00:00.000000 narwhals-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 narwhals-0.8.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 narwhals-0.8.1/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 narwhals-0.8.1/mkdocs.yml
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 narwhals-0.8.1/requirements-dev.txt
+-rw-r--r--   0        0        0     5243 2020-02-02 00:00:00.000000 narwhals-0.8.1/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     3725 2020-02-02 00:00:00.000000 narwhals-0.8.1/.github/workflows/extremes.yml
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 narwhals-0.8.1/.github/workflows/mkdocs.yml
+-rw-r--r--   0        0        0     2638 2020-02-02 00:00:00.000000 narwhals-0.8.1/.github/workflows/publish_to_pypi.yml
+-rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 narwhals-0.8.1/.github/workflows/pytest.yml
+-rw-r--r--   0        0        0     2021 2020-02-02 00:00:00.000000 narwhals-0.8.1/docs/extending.md
+-rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 narwhals-0.8.1/docs/generate_members.py
+-rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 narwhals-0.8.1/docs/index.md
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 narwhals-0.8.1/docs/installation.md
+-rw-r--r--   0        0        0     1245 2020-02-02 00:00:00.000000 narwhals-0.8.1/docs/quick_start.md
+-rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 narwhals-0.8.1/docs/related.md
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 narwhals-0.8.1/docs/requirements-docs.txt
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 narwhals-0.8.1/docs/roadmap.md
+-rw-r--r--   0        0        0     1281 2020-02-02 00:00:00.000000 narwhals-0.8.1/docs/why.md
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 narwhals-0.8.1/docs/api-reference/dataframe.md
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 narwhals-0.8.1/docs/api-reference/dependencies.md
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 narwhals-0.8.1/docs/api-reference/dtypes.md
+-rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 narwhals-0.8.1/docs/api-reference/expressions.md
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 narwhals-0.8.1/docs/api-reference/expressions_dt.md
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 narwhals-0.8.1/docs/api-reference/expressions_str.md
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 narwhals-0.8.1/docs/api-reference/index.md
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 narwhals-0.8.1/docs/api-reference/lazyframe.md
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 narwhals-0.8.1/docs/api-reference/narwhals.md
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 narwhals-0.8.1/docs/api-reference/series.md
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 narwhals-0.8.1/docs/api-reference/series_dt.md
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 narwhals-0.8.1/docs/api-reference/series_str.md
+-rwxr-xr-x   0        0        0   132699 2020-02-02 00:00:00.000000 narwhals-0.8.1/docs/assets/image.png
+-rw-r--r--   0        0        0     4468 2020-02-02 00:00:00.000000 narwhals-0.8.1/docs/basics/column.md
+-rw-r--r--   0        0        0     3572 2020-02-02 00:00:00.000000 narwhals-0.8.1/docs/basics/complete_example.md
+-rw-r--r--   0        0        0     4278 2020-02-02 00:00:00.000000 narwhals-0.8.1/docs/basics/dataframe.md
+-rw-r--r--   0        0        0     2523 2020-02-02 00:00:00.000000 narwhals-0.8.1/docs/other/pandas_index.md
+-rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 narwhals-0.8.1/narwhals/__init__.py
+-rw-r--r--   0        0        0    90926 2020-02-02 00:00:00.000000 narwhals-0.8.1/narwhals/dataframe.py
+-rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 narwhals-0.8.1/narwhals/dependencies.py
+-rw-r--r--   0        0        0     2791 2020-02-02 00:00:00.000000 narwhals-0.8.1/narwhals/dtypes.py
+-rw-r--r--   0        0        0    27381 2020-02-02 00:00:00.000000 narwhals-0.8.1/narwhals/expression.py
+-rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 narwhals-0.8.1/narwhals/functions.py
+-rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 narwhals-0.8.1/narwhals/group_by.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.1/narwhals/py.typed
+-rw-r--r--   0        0        0     6572 2020-02-02 00:00:00.000000 narwhals-0.8.1/narwhals/series.py
+-rw-r--r--   0        0        0     7100 2020-02-02 00:00:00.000000 narwhals-0.8.1/narwhals/translate.py
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 narwhals-0.8.1/narwhals/typing.py
+-rw-r--r--   0        0        0     2268 2020-02-02 00:00:00.000000 narwhals-0.8.1/narwhals/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.1/narwhals/_pandas_like/__init__.py
+-rw-r--r--   0        0        0     7838 2020-02-02 00:00:00.000000 narwhals-0.8.1/narwhals/_pandas_like/dataframe.py
+-rw-r--r--   0        0        0    10698 2020-02-02 00:00:00.000000 narwhals-0.8.1/narwhals/_pandas_like/expr.py
+-rw-r--r--   0        0        0     5640 2020-02-02 00:00:00.000000 narwhals-0.8.1/narwhals/_pandas_like/group_by.py
+-rw-r--r--   0        0        0     6324 2020-02-02 00:00:00.000000 narwhals-0.8.1/narwhals/_pandas_like/namespace.py
+-rw-r--r--   0        0        0    14369 2020-02-02 00:00:00.000000 narwhals-0.8.1/narwhals/_pandas_like/series.py
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 narwhals-0.8.1/narwhals/_pandas_like/typing.py
+-rw-r--r--   0        0        0    13436 2020-02-02 00:00:00.000000 narwhals-0.8.1/narwhals/_pandas_like/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.1/tests/__init__.py
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 narwhals-0.8.1/tests/conftest.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.1/tests/group_by_test.py
+-rw-r--r--   0        0        0    22181 2020-02-02 00:00:00.000000 narwhals-0.8.1/tests/test_common.py
+-rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 narwhals-0.8.1/tests/test_dt.py
+-rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 narwhals-0.8.1/tests/test_group_by.py
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 narwhals-0.8.1/tests/test_invalid.py
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 narwhals-0.8.1/tests/test_pandas.py
+-rw-r--r--   0        0        0     8935 2020-02-02 00:00:00.000000 narwhals-0.8.1/tests/test_series.py
+-rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 narwhals-0.8.1/tests/test_str.py
+-rw-r--r--   0        0        0     7276 2020-02-02 00:00:00.000000 narwhals-0.8.1/tests/tpch_q1_test.py
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 narwhals-0.8.1/tests/utils.py
+-rw-r--r--   0        0        0    21551 2020-02-02 00:00:00.000000 narwhals-0.8.1/tests/data/customer.parquet
+-rw-r--r--   0        0        0    34095 2020-02-02 00:00:00.000000 narwhals-0.8.1/tests/data/lineitem.parquet
+-rw-r--r--   0        0        0     2139 2020-02-02 00:00:00.000000 narwhals-0.8.1/tests/data/nation.parquet
+-rw-r--r--   0        0        0    24714 2020-02-02 00:00:00.000000 narwhals-0.8.1/tests/data/orders.parquet
+-rw-r--r--   0        0        0    13276 2020-02-02 00:00:00.000000 narwhals-0.8.1/tests/data/part.parquet
+-rw-r--r--   0        0        0    14921 2020-02-02 00:00:00.000000 narwhals-0.8.1/tests/data/partsupp.parquet
+-rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 narwhals-0.8.1/tests/data/region.parquet
+-rw-r--r--   0        0        0    19817 2020-02-02 00:00:00.000000 narwhals-0.8.1/tests/data/supplier.parquet
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.1/tests/expr/__init__.py
+-rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 narwhals-0.8.1/tests/expr/over_test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.1/tests/expr/test_over.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.1/tests/expr/str/__init__.py
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 narwhals-0.8.1/tests/expr/str/to_datetime_test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.1/tests/hypothesis/__init__.py
+-rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 narwhals-0.8.1/tests/hypothesis/test_basic_arithmetic.py
+-rw-r--r--   0        0        0     1897 2020-02-02 00:00:00.000000 narwhals-0.8.1/tests/hypothesis/test_concat.py
+-rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 narwhals-0.8.1/tests/hypothesis/test_join.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.1/tpch/__init__.py
+-rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 narwhals-0.8.1/tpch/q1.py
+-rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 narwhals-0.8.1/tpch/q2.py
+-rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 narwhals-0.8.1/tpch/q3.py
+-rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 narwhals-0.8.1/tpch/q4.py
+-rw-r--r--   0        0        0     2900 2020-02-02 00:00:00.000000 narwhals-0.8.1/tpch/q5.py
+-rwxr-xr-x   0        0        0    47336 2020-02-02 00:00:00.000000 narwhals-0.8.1/tpch/notebooks/gpu/execute.ipynb
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 narwhals-0.8.1/tpch/notebooks/gpu/kernel-metadata.json
+-rwxr-xr-x   0        0        0    17860 2020-02-02 00:00:00.000000 narwhals-0.8.1/tpch/notebooks/q1/execute.ipynb
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.8.1/tpch/notebooks/q1/kernel-metadata.json
+-rwxr-xr-x   0        0        0    18811 2020-02-02 00:00:00.000000 narwhals-0.8.1/tpch/notebooks/q2/execute.ipynb
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.8.1/tpch/notebooks/q2/kernel-metadata.json
+-rwxr-xr-x   0        0        0    17692 2020-02-02 00:00:00.000000 narwhals-0.8.1/tpch/notebooks/q3/execute.ipynb
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.8.1/tpch/notebooks/q3/kernel-metadata.json
+-rwxr-xr-x   0        0        0    16689 2020-02-02 00:00:00.000000 narwhals-0.8.1/tpch/notebooks/q4/execute.ipynb
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.8.1/tpch/notebooks/q4/kernel-metadata.json
+-rwxr-xr-x   0        0        0    18235 2020-02-02 00:00:00.000000 narwhals-0.8.1/tpch/notebooks/q5/execute.ipynb
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.8.1/tpch/notebooks/q5/kernel-metadata.json
+-rwxr-xr-x   0        0        0    16156 2020-02-02 00:00:00.000000 narwhals-0.8.1/tpch/notebooks/q6/execute.ipynb
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.8.1/tpch/notebooks/q6/kernel-metadata.json
+-rwxr-xr-x   0        0        0    27860 2020-02-02 00:00:00.000000 narwhals-0.8.1/tpch/notebooks/q7/execute.ipynb
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.8.1/tpch/notebooks/q7/kernel-metadata.json
+-rwxr-xr-x   0        0        0    27709 2020-02-02 00:00:00.000000 narwhals-0.8.1/tpch/notebooks/q8/execute.ipynb
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.8.1/tpch/notebooks/q8/kernel-metadata.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.1/utils/__init__.py
+-rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 narwhals-0.8.1/utils/bump_version.py
+-rw-r--r--   0        0        0     4163 2020-02-02 00:00:00.000000 narwhals-0.8.1/utils/check_api_reference.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 narwhals-0.8.1/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 narwhals-0.8.1/LICENSE.md
+-rw-r--r--   0        0        0     3229 2020-02-02 00:00:00.000000 narwhals-0.8.1/README.md
+-rw-r--r--   0        0        0     1995 2020-02-02 00:00:00.000000 narwhals-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0     3958 2020-02-02 00:00:00.000000 narwhals-0.8.1/PKG-INFO
```

### Comparing `narwhals-0.8.0/.pre-commit-config.yaml` & `narwhals-0.8.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.0/CONTRIBUTING.md` & `narwhals-0.8.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.0/mkdocs.yml` & `narwhals-0.8.1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.0/.github/CODE_OF_CONDUCT.md` & `narwhals-0.8.1/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.0/.github/workflows/extremes.yml` & `narwhals-0.8.1/.github/workflows/extremes.yml`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.0/.github/workflows/mkdocs.yml` & `narwhals-0.8.1/.github/workflows/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.0/.github/workflows/publish_to_pypi.yml` & `narwhals-0.8.1/.github/workflows/publish_to_pypi.yml`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.0/.github/workflows/pytest.yml` & `narwhals-0.8.1/.github/workflows/pytest.yml`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.0/docs/extending.md` & `narwhals-0.8.1/docs/extending.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.0/docs/generate_members.py` & `narwhals-0.8.1/docs/generate_members.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.0/docs/index.md` & `narwhals-0.8.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.0/docs/quick_start.md` & `narwhals-0.8.1/docs/quick_start.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.0/docs/related.md` & `narwhals-0.8.1/docs/related.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.0/docs/roadmap.md` & `narwhals-0.8.1/docs/roadmap.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.0/docs/why.md` & `narwhals-0.8.1/docs/why.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.0/docs/api-reference/index.md` & `narwhals-0.8.1/docs/api-reference/index.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.0/docs/api-reference/series.md` & `narwhals-0.8.1/docs/api-reference/series.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.0/docs/assets/image.png` & `narwhals-0.8.1/docs/assets/image.png`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.0/docs/basics/column.md` & `narwhals-0.8.1/docs/basics/column.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.0/docs/basics/complete_example.md` & `narwhals-0.8.1/docs/basics/complete_example.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.0/docs/basics/dataframe.md` & `narwhals-0.8.1/docs/basics/dataframe.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.0/docs/other/pandas_index.md` & `narwhals-0.8.1/docs/other/pandas_index.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.0/narwhals/__init__.py` & `narwhals-0.8.1/narwhals/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from narwhals.expression import sum
 from narwhals.expression import sum_horizontal
 from narwhals.functions import concat
 from narwhals.series import Series
 from narwhals.translate import from_native
 from narwhals.translate import to_native
 
-__version__ = "0.8.0"
+__version__ = "0.8.1"
 
 __all__ = [
     "concat",
     "to_native",
     "from_native",
     "all",
     "col",
```

### Comparing `narwhals-0.8.0/narwhals/dataframe.py` & `narwhals-0.8.1/narwhals/dataframe.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.0/narwhals/dependencies.py` & `narwhals-0.8.1/narwhals/dependencies.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.0/narwhals/dtypes.py` & `narwhals-0.8.1/narwhals/dtypes.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.0/narwhals/expression.py` & `narwhals-0.8.1/narwhals/expression.py`

 * *Files 1% similar despite different names*

```diff
@@ -616,14 +616,61 @@
     ) -> Expr:
         return self.__class__(
             lambda plx: self._call(plx).sample(
                 n, fraction=fraction, with_replacement=with_replacement
             )
         )
 
+    def over(self, *keys: str | Iterable[str]) -> Expr:
+        """
+        Compute expressions over the given groups.
+
+        Arguments:
+            keys: Names of columns to compute window expression over.
+                  Must be names of columns, as opposed to expressions -
+                  so, this is a bit less flexible than Polars' `Expr.over`.
+
+        Examples:
+            >>> import narwhals as nw
+            >>> import pandas as pd
+            >>> import polars as pl
+            >>> data = {'a': [1, 2, 3], 'b': [1, 1, 2]}
+            >>> df_pd = pd.DataFrame(data)
+            >>> df_pl = pl.DataFrame(data)
+
+            Let's define a dataframe-agnostic function:
+
+            >>> def func(df_any):
+            ...     df = nw.from_native(df_any)
+            ...     df = df.with_columns(
+            ...         a_min_per_group = nw.col('a').min().over('b')
+            ...     )
+            ...     return nw.to_native(df)
+
+            We can then pass either pandas or Polars:
+
+            >>> func(df_pd)
+               a  b  a_min_per_group
+            0  1  1                1
+            1  2  1                1
+            2  3  2                3
+            >>> func(df_pl)
+            shape: (3, 3)
+            ┌─────┬─────┬─────────────────┐
+            │ a   ┆ b   ┆ a_min_per_group │
+            │ --- ┆ --- ┆ ---             │
+            │ i64 ┆ i64 ┆ i64             │
+            ╞═════╪═════╪═════════════════╡
+            │ 1   ┆ 1   ┆ 1               │
+            │ 2   ┆ 1   ┆ 1               │
+            │ 3   ┆ 2   ┆ 3               │
+            └─────┴─────┴─────────────────┘
+        """
+        return self.__class__(lambda plx: self._call(plx).over(flatten(keys)))
+
     @property
     def str(self) -> ExprStringNamespace:
         return ExprStringNamespace(self)
 
     @property
     def dt(self) -> ExprDateTimeNamespace:
         return ExprDateTimeNamespace(self)
@@ -644,14 +691,19 @@
 
         Notes:
             pandas defaults to nanosecond time unit, Polars to microsecond.
             Prior to pandas 2.0, nanoseconds were the only time unit supported
             in pandas, with no ability to set any other one. The ability to
             set the time unit in pandas, if the version permits, will arrive.
 
+        Arguments:
+            format: Format to parse strings with. Must be passed, as different
+                    dataframe libraries have different ways of auto-inferring
+                    formats.
+
         Examples:
             >>> import pandas as pd
             >>> import polars as pl
             >>> import narwhals as nw
             >>> df_pd = pd.DataFrame({'a': ['2020-01-01', '2020-01-02']})
             >>> df_pl = pl.DataFrame({'a': ['2020-01-01', '2020-01-02']})
```

### Comparing `narwhals-0.8.0/narwhals/functions.py` & `narwhals-0.8.1/narwhals/functions.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.0/narwhals/group_by.py` & `narwhals-0.8.1/narwhals/group_by.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.0/narwhals/series.py` & `narwhals-0.8.1/narwhals/series.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.0/narwhals/translate.py` & `narwhals-0.8.1/narwhals/translate.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.0/narwhals/typing.py` & `narwhals-0.8.1/narwhals/typing.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.0/narwhals/utils.py` & `narwhals-0.8.1/narwhals/utils.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.0/narwhals/_pandas_like/dataframe.py` & `narwhals-0.8.1/narwhals/_pandas_like/dataframe.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.0/narwhals/_pandas_like/expr.py` & `narwhals-0.8.1/narwhals/_pandas_like/expr.py`

 * *Files 3% similar despite different names*

```diff
@@ -215,14 +215,36 @@
             depth=self._depth,
             function_name=self._function_name,
             root_names=self._root_names,
             output_names=[name],
             implementation=self._implementation,
         )
 
+    def over(self, keys: list[str]) -> Self:
+        def func(df: PandasDataFrame) -> list[PandasSeries]:
+            if self._output_names is None:
+                msg = (
+                    "Anonymous expressions are not supported in over.\n"
+                    "Instead of `nw.all()`, try using a named expression, such as "
+                    "`nw.col('a', 'b')`\n"
+                )
+                raise ValueError(msg)
+            tmp = df.group_by(keys).agg(self)
+            tmp = df.select(keys).join(tmp, how="left", left_on=keys, right_on=keys)
+            return [tmp[name] for name in self._output_names]
+
+        return self.__class__(
+            func,
+            depth=self._depth + 1,
+            function_name=self._function_name + "->over",
+            root_names=self._root_names,
+            output_names=self._output_names,
+            implementation=self._implementation,
+        )
+
     @property
     def str(self) -> PandasExprStringNamespace:
         return PandasExprStringNamespace(self)
 
     @property
     def dt(self) -> PandasExprDateTimeNamespace:
         return PandasExprDateTimeNamespace(self)
```

### Comparing `narwhals-0.8.0/narwhals/_pandas_like/group_by.py` & `narwhals-0.8.1/narwhals/_pandas_like/group_by.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.0/narwhals/_pandas_like/namespace.py` & `narwhals-0.8.1/narwhals/_pandas_like/namespace.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.0/narwhals/_pandas_like/series.py` & `narwhals-0.8.1/narwhals/_pandas_like/series.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.0/narwhals/_pandas_like/typing.py` & `narwhals-0.8.1/narwhals/_pandas_like/typing.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.0/narwhals/_pandas_like/utils.py` & `narwhals-0.8.1/narwhals/_pandas_like/utils.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.0/tests/conftest.py` & `narwhals-0.8.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.0/tests/test_common.py` & `narwhals-0.8.1/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.0/tests/test_dt.py` & `narwhals-0.8.1/tests/test_dt.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.0/tests/test_group_by.py` & `narwhals-0.8.1/tests/test_group_by.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.0/tests/test_series.py` & `narwhals-0.8.1/tests/test_series.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.0/tests/test_str.py` & `narwhals-0.8.1/tests/test_str.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.0/tests/tpch_q1_test.py` & `narwhals-0.8.1/tests/tpch_q1_test.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.0/tests/utils.py` & `narwhals-0.8.1/tests/utils.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.0/tests/data/customer.parquet` & `narwhals-0.8.1/tests/data/customer.parquet`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.0/tests/data/lineitem.parquet` & `narwhals-0.8.1/tests/data/lineitem.parquet`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.0/tests/data/nation.parquet` & `narwhals-0.8.1/tests/data/nation.parquet`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.0/tests/data/orders.parquet` & `narwhals-0.8.1/tests/data/orders.parquet`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.0/tests/data/part.parquet` & `narwhals-0.8.1/tests/data/part.parquet`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.0/tests/data/partsupp.parquet` & `narwhals-0.8.1/tests/data/partsupp.parquet`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.0/tests/data/region.parquet` & `narwhals-0.8.1/tests/data/region.parquet`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.0/tests/data/supplier.parquet` & `narwhals-0.8.1/tests/data/supplier.parquet`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.0/tests/expr/test_to_datetime.py` & `narwhals-0.8.1/tests/expr/str/to_datetime_test.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.0/tests/hypothesis/test_basic_arithmetic.py` & `narwhals-0.8.1/tests/hypothesis/test_basic_arithmetic.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.0/tests/hypothesis/test_concat.py` & `narwhals-0.8.1/tests/hypothesis/test_concat.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.0/tests/hypothesis/test_join.py` & `narwhals-0.8.1/tests/hypothesis/test_join.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.0/tpch/q1.py` & `narwhals-0.8.1/tpch/q1.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.0/tpch/q2.py` & `narwhals-0.8.1/tpch/q2.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.0/tpch/q3.py` & `narwhals-0.8.1/tpch/q3.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.0/tpch/q4.py` & `narwhals-0.8.1/tpch/q4.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.0/tpch/q5.py` & `narwhals-0.8.1/tpch/q5.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.0/tpch/notebooks/gpu/execute.ipynb` & `narwhals-0.8.1/tpch/notebooks/gpu/execute.ipynb`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.0/tpch/notebooks/q1/execute.ipynb` & `narwhals-0.8.1/tpch/notebooks/q1/execute.ipynb`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.0/tpch/notebooks/q2/execute.ipynb` & `narwhals-0.8.1/tpch/notebooks/q2/execute.ipynb`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.0/tpch/notebooks/q3/execute.ipynb` & `narwhals-0.8.1/tpch/notebooks/q3/execute.ipynb`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.0/tpch/notebooks/q4/execute.ipynb` & `narwhals-0.8.1/tpch/notebooks/q4/execute.ipynb`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.0/tpch/notebooks/q5/execute.ipynb` & `narwhals-0.8.1/tpch/notebooks/q5/execute.ipynb`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.0/tpch/notebooks/q6/execute.ipynb` & `narwhals-0.8.1/tpch/notebooks/q6/execute.ipynb`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.0/tpch/notebooks/q7/execute.ipynb` & `narwhals-0.8.1/tpch/notebooks/q7/execute.ipynb`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.0/tpch/notebooks/q8/execute.ipynb` & `narwhals-0.8.1/tpch/notebooks/q8/execute.ipynb`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.0/utils/bump_version.py` & `narwhals-0.8.1/utils/bump_version.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.0/utils/check_api_reference.py` & `narwhals-0.8.1/utils/check_api_reference.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,15 +122,15 @@
 # str
 
 # Check Expr vs Series
 expr = [i for i in nw.Expr(lambda: 0).__dir__() if not i[0].isupper() and i[0] != "_"]
 series = [
     i for i in nw.Series(pl.Series()).__dir__() if not i[0].isupper() and i[0] != "_"
 ]
-if missing := set(expr).difference(series):
+if missing := set(expr).difference(series).difference({"over"}):
     print("In expr but not in series")  # noqa: T201
     print(missing)  # noqa: T201
     ret = 1
 if (
     extra := set(series)
     .difference(expr)
     .difference({"to_pandas", "to_numpy", "dtype", "name", "shape"})
```

### Comparing `narwhals-0.8.0/LICENSE.md` & `narwhals-0.8.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.0/README.md` & `narwhals-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.0/pyproject.toml` & `narwhals-0.8.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "narwhals"
-version = "0.8.0"
+version = "0.8.1"
 authors = [
   { name="Marco Gorelli", email="33491632+MarcoGorelli@users.noreply.github.com" },
 ]
 description = "Extremely lightweight compatibility layer between pandas, Polars, cuDF, and Modin"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `narwhals-0.8.0/PKG-INFO` & `narwhals-0.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: narwhals
-Version: 0.8.0
+Version: 0.8.1
 Summary: Extremely lightweight compatibility layer between pandas, Polars, cuDF, and Modin
 Project-URL: Homepage, https://github.com/MarcoGorelli/narwhals
 Project-URL: Bug Tracker, https://github.com/MarcoGorelli/narwhals
 Author-email: Marco Gorelli <33491632+MarcoGorelli@users.noreply.github.com>
 License-File: LICENSE.md
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

