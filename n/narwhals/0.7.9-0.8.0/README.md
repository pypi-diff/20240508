# Comparing `tmp/narwhals-0.7.9.tar.gz` & `tmp/narwhals-0.8.0.tar.gz`

## Comparing `narwhals-0.7.9.tar` & `narwhals-0.8.0.tar`

### file list

```diff
@@ -1,101 +1,113 @@
--rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 narwhals-0.7.9/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 narwhals-0.7.9/CONTRIBUTING.md
--rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 narwhals-0.7.9/mkdocs.yml
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 narwhals-0.7.9/requirements-dev.txt
--rw-r--r--   0        0        0     5243 2020-02-02 00:00:00.000000 narwhals-0.7.9/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     2580 2020-02-02 00:00:00.000000 narwhals-0.7.9/.github/workflows/extremes.yml
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 narwhals-0.7.9/.github/workflows/mkdocs.yml
--rw-r--r--   0        0        0     2638 2020-02-02 00:00:00.000000 narwhals-0.7.9/.github/workflows/publish_to_pypi.yml
--rw-r--r--   0        0        0     2000 2020-02-02 00:00:00.000000 narwhals-0.7.9/.github/workflows/pytest.yml
--rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 narwhals-0.7.9/docs/extending.md
--rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 narwhals-0.7.9/docs/generate_members.py
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 narwhals-0.7.9/docs/index.md
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 narwhals-0.7.9/docs/installation.md
--rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 narwhals-0.7.9/docs/quick_start.md
--rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 narwhals-0.7.9/docs/related.md
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 narwhals-0.7.9/docs/requirements-docs.txt
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 narwhals-0.7.9/docs/roadmap.md
--rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 narwhals-0.7.9/docs/why.md
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 narwhals-0.7.9/docs/api-reference/dataframe.md
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 narwhals-0.7.9/docs/api-reference/dtypes.md
--rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 narwhals-0.7.9/docs/api-reference/expressions.md
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 narwhals-0.7.9/docs/api-reference/expressions_dt.md
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 narwhals-0.7.9/docs/api-reference/expressions_str.md
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 narwhals-0.7.9/docs/api-reference/index.md
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 narwhals-0.7.9/docs/api-reference/lazyframe.md
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 narwhals-0.7.9/docs/api-reference/narwhals.md
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 narwhals-0.7.9/docs/api-reference/series.md
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 narwhals-0.7.9/docs/api-reference/series_dt.md
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 narwhals-0.7.9/docs/api-reference/series_str.md
--rwxr-xr-x   0        0        0   132699 2020-02-02 00:00:00.000000 narwhals-0.7.9/docs/assets/image.png
--rw-r--r--   0        0        0     4475 2020-02-02 00:00:00.000000 narwhals-0.7.9/docs/basics/column.md
--rw-r--r--   0        0        0     3534 2020-02-02 00:00:00.000000 narwhals-0.7.9/docs/basics/complete_example.md
--rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 narwhals-0.7.9/docs/basics/dataframe.md
--rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 narwhals-0.7.9/narwhals/__init__.py
--rw-r--r--   0        0        0    46236 2020-02-02 00:00:00.000000 narwhals-0.7.9/narwhals/dataframe.py
--rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 narwhals-0.7.9/narwhals/dependencies.py
--rw-r--r--   0        0        0     2791 2020-02-02 00:00:00.000000 narwhals-0.7.9/narwhals/dtypes.py
--rw-r--r--   0        0        0     9357 2020-02-02 00:00:00.000000 narwhals-0.7.9/narwhals/expression.py
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 narwhals-0.7.9/narwhals/functions.py
--rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 narwhals-0.7.9/narwhals/group_by.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.7.9/narwhals/py.typed
--rw-r--r--   0        0        0     5381 2020-02-02 00:00:00.000000 narwhals-0.7.9/narwhals/series.py
--rw-r--r--   0        0        0     3136 2020-02-02 00:00:00.000000 narwhals-0.7.9/narwhals/translate.py
--rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 narwhals-0.7.9/narwhals/typing.py
--rw-r--r--   0        0        0     1298 2020-02-02 00:00:00.000000 narwhals-0.7.9/narwhals/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.7.9/narwhals/_pandas_like/__init__.py
--rw-r--r--   0        0        0     7914 2020-02-02 00:00:00.000000 narwhals-0.7.9/narwhals/_pandas_like/dataframe.py
--rw-r--r--   0        0        0     8871 2020-02-02 00:00:00.000000 narwhals-0.7.9/narwhals/_pandas_like/expr.py
--rw-r--r--   0        0        0     5640 2020-02-02 00:00:00.000000 narwhals-0.7.9/narwhals/_pandas_like/group_by.py
--rw-r--r--   0        0        0     6324 2020-02-02 00:00:00.000000 narwhals-0.7.9/narwhals/_pandas_like/namespace.py
--rw-r--r--   0        0        0    12038 2020-02-02 00:00:00.000000 narwhals-0.7.9/narwhals/_pandas_like/series.py
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 narwhals-0.7.9/narwhals/_pandas_like/typing.py
--rw-r--r--   0        0        0    13137 2020-02-02 00:00:00.000000 narwhals-0.7.9/narwhals/_pandas_like/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.7.9/tests/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.7.9/tests/group_by_test.py
--rw-r--r--   0        0        0    19910 2020-02-02 00:00:00.000000 narwhals-0.7.9/tests/test_common.py
--rw-r--r--   0        0        0     1393 2020-02-02 00:00:00.000000 narwhals-0.7.9/tests/test_dt.py
--rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 narwhals-0.7.9/tests/test_group_by.py
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 narwhals-0.7.9/tests/test_pandas.py
--rw-r--r--   0        0        0     7772 2020-02-02 00:00:00.000000 narwhals-0.7.9/tests/test_series.py
--rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 narwhals-0.7.9/tests/test_str.py
--rw-r--r--   0        0        0     7276 2020-02-02 00:00:00.000000 narwhals-0.7.9/tests/tpch_q1_test.py
--rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 narwhals-0.7.9/tests/utils.py
--rw-r--r--   0        0        0    21551 2020-02-02 00:00:00.000000 narwhals-0.7.9/tests/data/customer.parquet
--rw-r--r--   0        0        0    34095 2020-02-02 00:00:00.000000 narwhals-0.7.9/tests/data/lineitem.parquet
--rw-r--r--   0        0        0     2139 2020-02-02 00:00:00.000000 narwhals-0.7.9/tests/data/nation.parquet
--rw-r--r--   0        0        0    24714 2020-02-02 00:00:00.000000 narwhals-0.7.9/tests/data/orders.parquet
--rw-r--r--   0        0        0    13276 2020-02-02 00:00:00.000000 narwhals-0.7.9/tests/data/part.parquet
--rw-r--r--   0        0        0    14921 2020-02-02 00:00:00.000000 narwhals-0.7.9/tests/data/partsupp.parquet
--rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 narwhals-0.7.9/tests/data/region.parquet
--rw-r--r--   0        0        0    19817 2020-02-02 00:00:00.000000 narwhals-0.7.9/tests/data/supplier.parquet
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.7.9/tpch/__init__.py
--rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 narwhals-0.7.9/tpch/q1.py
--rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 narwhals-0.7.9/tpch/q2.py
--rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 narwhals-0.7.9/tpch/q3.py
--rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 narwhals-0.7.9/tpch/q4.py
--rw-r--r--   0        0        0     2900 2020-02-02 00:00:00.000000 narwhals-0.7.9/tpch/q5.py
--rwxr-xr-x   0        0        0    47336 2020-02-02 00:00:00.000000 narwhals-0.7.9/tpch/notebooks/gpu/execute.ipynb
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 narwhals-0.7.9/tpch/notebooks/gpu/kernel-metadata.json
--rwxr-xr-x   0        0        0    17858 2020-02-02 00:00:00.000000 narwhals-0.7.9/tpch/notebooks/q1/execute.ipynb
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.7.9/tpch/notebooks/q1/kernel-metadata.json
--rwxr-xr-x   0        0        0    21797 2020-02-02 00:00:00.000000 narwhals-0.7.9/tpch/notebooks/q2/execute.ipynb
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.7.9/tpch/notebooks/q2/kernel-metadata.json
--rwxr-xr-x   0        0        0    15420 2020-02-02 00:00:00.000000 narwhals-0.7.9/tpch/notebooks/q3/execute.ipynb
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.7.9/tpch/notebooks/q3/kernel-metadata.json
--rwxr-xr-x   0        0        0    14794 2020-02-02 00:00:00.000000 narwhals-0.7.9/tpch/notebooks/q4/execute.ipynb
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.7.9/tpch/notebooks/q4/kernel-metadata.json
--rwxr-xr-x   0        0        0    15844 2020-02-02 00:00:00.000000 narwhals-0.7.9/tpch/notebooks/q5/execute.ipynb
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.7.9/tpch/notebooks/q5/kernel-metadata.json
--rwxr-xr-x   0        0        0    14502 2020-02-02 00:00:00.000000 narwhals-0.7.9/tpch/notebooks/q6/execute.ipynb
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.7.9/tpch/notebooks/q6/kernel-metadata.json
--rwxr-xr-x   0        0        0    24376 2020-02-02 00:00:00.000000 narwhals-0.7.9/tpch/notebooks/q7/execute.ipynb
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.7.9/tpch/notebooks/q7/kernel-metadata.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.7.9/utils/__init__.py
--rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 narwhals-0.7.9/utils/bump_version.py
--rw-r--r--   0        0        0     4081 2020-02-02 00:00:00.000000 narwhals-0.7.9/utils/check_api_reference.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 narwhals-0.7.9/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 narwhals-0.7.9/LICENSE.md
--rw-r--r--   0        0        0     4550 2020-02-02 00:00:00.000000 narwhals-0.7.9/README.md
--rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 narwhals-0.7.9/pyproject.toml
--rw-r--r--   0        0        0     5136 2020-02-02 00:00:00.000000 narwhals-0.7.9/PKG-INFO
+-rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 narwhals-0.8.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 narwhals-0.8.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 narwhals-0.8.0/mkdocs.yml
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 narwhals-0.8.0/requirements-dev.txt
+-rw-r--r--   0        0        0     5243 2020-02-02 00:00:00.000000 narwhals-0.8.0/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     3725 2020-02-02 00:00:00.000000 narwhals-0.8.0/.github/workflows/extremes.yml
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 narwhals-0.8.0/.github/workflows/mkdocs.yml
+-rw-r--r--   0        0        0     2638 2020-02-02 00:00:00.000000 narwhals-0.8.0/.github/workflows/publish_to_pypi.yml
+-rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 narwhals-0.8.0/.github/workflows/pytest.yml
+-rw-r--r--   0        0        0     2021 2020-02-02 00:00:00.000000 narwhals-0.8.0/docs/extending.md
+-rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 narwhals-0.8.0/docs/generate_members.py
+-rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 narwhals-0.8.0/docs/index.md
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 narwhals-0.8.0/docs/installation.md
+-rw-r--r--   0        0        0     1245 2020-02-02 00:00:00.000000 narwhals-0.8.0/docs/quick_start.md
+-rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 narwhals-0.8.0/docs/related.md
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 narwhals-0.8.0/docs/requirements-docs.txt
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 narwhals-0.8.0/docs/roadmap.md
+-rw-r--r--   0        0        0     1281 2020-02-02 00:00:00.000000 narwhals-0.8.0/docs/why.md
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 narwhals-0.8.0/docs/api-reference/dataframe.md
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 narwhals-0.8.0/docs/api-reference/dependencies.md
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 narwhals-0.8.0/docs/api-reference/dtypes.md
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 narwhals-0.8.0/docs/api-reference/expressions.md
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 narwhals-0.8.0/docs/api-reference/expressions_dt.md
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 narwhals-0.8.0/docs/api-reference/expressions_str.md
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 narwhals-0.8.0/docs/api-reference/index.md
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 narwhals-0.8.0/docs/api-reference/lazyframe.md
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 narwhals-0.8.0/docs/api-reference/narwhals.md
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 narwhals-0.8.0/docs/api-reference/series.md
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 narwhals-0.8.0/docs/api-reference/series_dt.md
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 narwhals-0.8.0/docs/api-reference/series_str.md
+-rwxr-xr-x   0        0        0   132699 2020-02-02 00:00:00.000000 narwhals-0.8.0/docs/assets/image.png
+-rw-r--r--   0        0        0     4468 2020-02-02 00:00:00.000000 narwhals-0.8.0/docs/basics/column.md
+-rw-r--r--   0        0        0     3572 2020-02-02 00:00:00.000000 narwhals-0.8.0/docs/basics/complete_example.md
+-rw-r--r--   0        0        0     4278 2020-02-02 00:00:00.000000 narwhals-0.8.0/docs/basics/dataframe.md
+-rw-r--r--   0        0        0     2523 2020-02-02 00:00:00.000000 narwhals-0.8.0/docs/other/pandas_index.md
+-rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 narwhals-0.8.0/narwhals/__init__.py
+-rw-r--r--   0        0        0    90926 2020-02-02 00:00:00.000000 narwhals-0.8.0/narwhals/dataframe.py
+-rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 narwhals-0.8.0/narwhals/dependencies.py
+-rw-r--r--   0        0        0     2791 2020-02-02 00:00:00.000000 narwhals-0.8.0/narwhals/dtypes.py
+-rw-r--r--   0        0        0    25221 2020-02-02 00:00:00.000000 narwhals-0.8.0/narwhals/expression.py
+-rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 narwhals-0.8.0/narwhals/functions.py
+-rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 narwhals-0.8.0/narwhals/group_by.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.0/narwhals/py.typed
+-rw-r--r--   0        0        0     6572 2020-02-02 00:00:00.000000 narwhals-0.8.0/narwhals/series.py
+-rw-r--r--   0        0        0     7100 2020-02-02 00:00:00.000000 narwhals-0.8.0/narwhals/translate.py
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 narwhals-0.8.0/narwhals/typing.py
+-rw-r--r--   0        0        0     2268 2020-02-02 00:00:00.000000 narwhals-0.8.0/narwhals/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.0/narwhals/_pandas_like/__init__.py
+-rw-r--r--   0        0        0     7838 2020-02-02 00:00:00.000000 narwhals-0.8.0/narwhals/_pandas_like/dataframe.py
+-rw-r--r--   0        0        0     9787 2020-02-02 00:00:00.000000 narwhals-0.8.0/narwhals/_pandas_like/expr.py
+-rw-r--r--   0        0        0     5640 2020-02-02 00:00:00.000000 narwhals-0.8.0/narwhals/_pandas_like/group_by.py
+-rw-r--r--   0        0        0     6324 2020-02-02 00:00:00.000000 narwhals-0.8.0/narwhals/_pandas_like/namespace.py
+-rw-r--r--   0        0        0    14369 2020-02-02 00:00:00.000000 narwhals-0.8.0/narwhals/_pandas_like/series.py
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 narwhals-0.8.0/narwhals/_pandas_like/typing.py
+-rw-r--r--   0        0        0    13436 2020-02-02 00:00:00.000000 narwhals-0.8.0/narwhals/_pandas_like/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.0/tests/__init__.py
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 narwhals-0.8.0/tests/conftest.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.0/tests/group_by_test.py
+-rw-r--r--   0        0        0    22181 2020-02-02 00:00:00.000000 narwhals-0.8.0/tests/test_common.py
+-rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 narwhals-0.8.0/tests/test_dt.py
+-rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 narwhals-0.8.0/tests/test_group_by.py
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 narwhals-0.8.0/tests/test_invalid.py
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 narwhals-0.8.0/tests/test_pandas.py
+-rw-r--r--   0        0        0     8935 2020-02-02 00:00:00.000000 narwhals-0.8.0/tests/test_series.py
+-rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 narwhals-0.8.0/tests/test_str.py
+-rw-r--r--   0        0        0     7276 2020-02-02 00:00:00.000000 narwhals-0.8.0/tests/tpch_q1_test.py
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 narwhals-0.8.0/tests/utils.py
+-rw-r--r--   0        0        0    21551 2020-02-02 00:00:00.000000 narwhals-0.8.0/tests/data/customer.parquet
+-rw-r--r--   0        0        0    34095 2020-02-02 00:00:00.000000 narwhals-0.8.0/tests/data/lineitem.parquet
+-rw-r--r--   0        0        0     2139 2020-02-02 00:00:00.000000 narwhals-0.8.0/tests/data/nation.parquet
+-rw-r--r--   0        0        0    24714 2020-02-02 00:00:00.000000 narwhals-0.8.0/tests/data/orders.parquet
+-rw-r--r--   0        0        0    13276 2020-02-02 00:00:00.000000 narwhals-0.8.0/tests/data/part.parquet
+-rw-r--r--   0        0        0    14921 2020-02-02 00:00:00.000000 narwhals-0.8.0/tests/data/partsupp.parquet
+-rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 narwhals-0.8.0/tests/data/region.parquet
+-rw-r--r--   0        0        0    19817 2020-02-02 00:00:00.000000 narwhals-0.8.0/tests/data/supplier.parquet
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.0/tests/expr/__init__.py
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 narwhals-0.8.0/tests/expr/test_to_datetime.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.0/tests/hypothesis/__init__.py
+-rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 narwhals-0.8.0/tests/hypothesis/test_basic_arithmetic.py
+-rw-r--r--   0        0        0     1897 2020-02-02 00:00:00.000000 narwhals-0.8.0/tests/hypothesis/test_concat.py
+-rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 narwhals-0.8.0/tests/hypothesis/test_join.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.0/tpch/__init__.py
+-rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 narwhals-0.8.0/tpch/q1.py
+-rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 narwhals-0.8.0/tpch/q2.py
+-rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 narwhals-0.8.0/tpch/q3.py
+-rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 narwhals-0.8.0/tpch/q4.py
+-rw-r--r--   0        0        0     2900 2020-02-02 00:00:00.000000 narwhals-0.8.0/tpch/q5.py
+-rwxr-xr-x   0        0        0    47336 2020-02-02 00:00:00.000000 narwhals-0.8.0/tpch/notebooks/gpu/execute.ipynb
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 narwhals-0.8.0/tpch/notebooks/gpu/kernel-metadata.json
+-rwxr-xr-x   0        0        0    17860 2020-02-02 00:00:00.000000 narwhals-0.8.0/tpch/notebooks/q1/execute.ipynb
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.8.0/tpch/notebooks/q1/kernel-metadata.json
+-rwxr-xr-x   0        0        0    18811 2020-02-02 00:00:00.000000 narwhals-0.8.0/tpch/notebooks/q2/execute.ipynb
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.8.0/tpch/notebooks/q2/kernel-metadata.json
+-rwxr-xr-x   0        0        0    17692 2020-02-02 00:00:00.000000 narwhals-0.8.0/tpch/notebooks/q3/execute.ipynb
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.8.0/tpch/notebooks/q3/kernel-metadata.json
+-rwxr-xr-x   0        0        0    16689 2020-02-02 00:00:00.000000 narwhals-0.8.0/tpch/notebooks/q4/execute.ipynb
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.8.0/tpch/notebooks/q4/kernel-metadata.json
+-rwxr-xr-x   0        0        0    18235 2020-02-02 00:00:00.000000 narwhals-0.8.0/tpch/notebooks/q5/execute.ipynb
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.8.0/tpch/notebooks/q5/kernel-metadata.json
+-rwxr-xr-x   0        0        0    16156 2020-02-02 00:00:00.000000 narwhals-0.8.0/tpch/notebooks/q6/execute.ipynb
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.8.0/tpch/notebooks/q6/kernel-metadata.json
+-rwxr-xr-x   0        0        0    27860 2020-02-02 00:00:00.000000 narwhals-0.8.0/tpch/notebooks/q7/execute.ipynb
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.8.0/tpch/notebooks/q7/kernel-metadata.json
+-rwxr-xr-x   0        0        0    27709 2020-02-02 00:00:00.000000 narwhals-0.8.0/tpch/notebooks/q8/execute.ipynb
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.8.0/tpch/notebooks/q8/kernel-metadata.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.0/utils/__init__.py
+-rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 narwhals-0.8.0/utils/bump_version.py
+-rw-r--r--   0        0        0     4142 2020-02-02 00:00:00.000000 narwhals-0.8.0/utils/check_api_reference.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 narwhals-0.8.0/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 narwhals-0.8.0/LICENSE.md
+-rw-r--r--   0        0        0     3229 2020-02-02 00:00:00.000000 narwhals-0.8.0/README.md
+-rw-r--r--   0        0        0     1995 2020-02-02 00:00:00.000000 narwhals-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     3958 2020-02-02 00:00:00.000000 narwhals-0.8.0/PKG-INFO
```

### Comparing `narwhals-0.7.9/.pre-commit-config.yaml` & `narwhals-0.8.0/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 repos:
 - repo: https://github.com/astral-sh/ruff-pre-commit
   # Ruff version.
-  rev: 'v0.3.5'
+  rev: 'v0.4.3'
   hooks:
     # Run the formatter.
     - id: ruff-format
     # Run the linter.
     - id: ruff
       args: [--fix]
 - repo: https://github.com/pre-commit/mirrors-mypy
-  rev: 'v1.9.0'
+  rev: 'v1.10.0'
   hooks:
     - id: mypy
       additional_dependencies: ['polars==0.20.10', 'pytest==8.0.1']
       exclude: utils|tpch
 - repo: https://github.com/codespell-project/codespell
   rev: 'v2.2.6'
   hooks:
```

### Comparing `narwhals-0.7.9/CONTRIBUTING.md` & `narwhals-0.8.0/CONTRIBUTING.md`

 * *Files 18% similar despite different names*

```diff
@@ -9,14 +9,21 @@
 1. Make sure you have Python3.9+ installed
 2. Create a new virtual environment with `python3.11 -m venv .venv` (or whichever version of Python3.9+ you prefer)
 3. Activate it: `. .venv/bin/activate`
 4. Install Narwhals: `pip install -e .`
 5. Install test requirements: `pip install -r requirements-dev.txt`
 6. Install docs requirements: `pip install -r docs/requirements-docs.txt`
 
+You should also install pre-commit:
+```
+pip install pre-commit
+pre-commit install
+```
+This will automatically format and lint your code before each commit, and it will block the commit if any issues are found.
+
 ## Running tests
 
 To run tests, run `pytest`. To check coverage: `pytest --cov=narwhals`.
 
 ## Building docs
 
 To build the docs, run `mkdocs serve`, and then open the link provided in a browser.
```

### Comparing `narwhals-0.7.9/mkdocs.yml` & `narwhals-0.8.0/mkdocs.yml`

 * *Files 6% similar despite different names*

```diff
@@ -5,29 +5,32 @@
   - Why: why.md
   - Installation: installation.md
   - Quick start: quick_start.md
   - Tutorial:
     - basics/dataframe.md
     - basics/column.md
     - basics/complete_example.md
-  - Extending: extending.md
+  - Other concepts:
+    - other/pandas_index.md
+  - extending.md
   - Roadmap: roadmap.md
   - Related projects: related.md
   - API Reference:
     - api-reference/index.md
     - api-reference/narwhals.md
     - api-reference/dataframe.md
     - api-reference/lazyframe.md
     - api-reference/series.md
     - api-reference/series_dt.md
     - api-reference/series_str.md
     - api-reference/expressions.md
     - api-reference/expressions_dt.md
     - api-reference/expressions_str.md
     - api-reference/dtypes.md
+    - api-reference/dependencies.md
 theme:
   name: material
   font: false
   features:
     - content.code.copy
     - content.code.annotate
     - navigation.footer
```

### Comparing `narwhals-0.7.9/.github/CODE_OF_CONDUCT.md` & `narwhals-0.8.0/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.9/.github/workflows/extremes.yml` & `narwhals-0.8.0/.github/workflows/extremes.yml`

 * *Files 16% similar despite different names*

```diff
@@ -25,21 +25,21 @@
             ~/.cache/pip
             $RUNNER_TOOL_CACHE/Python/*
             ~\AppData\Local\pip\Cache
           key: ${{ runner.os }}-build-${{ matrix.python-version }}
       - name: install-reqs
         run: python -m pip install --upgrade tox virtualenv setuptools pip -r requirements-dev.txt
       - name: install-modin
-        run: python -m pip install pandas==2.0.0 polars==0.20.5 modin[dask]
+        run: python -m pip install pandas==1.1.5 polars==0.20.3
       - name: Run pytest
-        run: pytest tests --cov=narwhals --cov=tests --cov-fail-under=50
+        run: pytest tests --cov=narwhals --cov=tests --cov-fail-under=50 --runslow
       - name: Run doctests
         run: pytest narwhals --doctest-modules
 
-  nightlies:
+  pandas-nightly:
     strategy:
       matrix:
         python-version: ["3.12"]
         os: [ubuntu-latest]
 
     runs-on: ${{ matrix.os }}
     steps:
@@ -51,28 +51,60 @@
         uses: actions/cache@v3
         with:
           path: |
             ~/.cache/pip
             $RUNNER_TOOL_CACHE/Python/*
             ~\AppData\Local\pip\Cache
           key: ${{ runner.os }}-build-${{ matrix.python-version }}
-      - name: install-kaggle
-        run: python -m pip install kaggle
-      - name: Download Kaggle notebook artifact
-        env:
-          KAGGLE_USERNAME: ${{ secrets.KAGGLE_USERNAME }}
-          KAGGLE_KEY: ${{ secrets.KAGGLE_KEY }}
-        run: kaggle kernels output marcogorelli/polars-nightly
+      - name: uninstall pandas
+        run: python -m pip uninstall pandas -y
+      - name: install-modin-polars
+        run: pip install modin[dask] polars
       - name: install-reqs
         run: python -m pip install --upgrade tox virtualenv setuptools pip -r requirements-dev.txt
-      - name: uninstall pandas/polars
-        run: python -m pip uninstall pandas polars -y
-      - name: install-modin
-        run: pip install modin[dask]
       - name: install-pandas-nightly
         run: python -m pip install --pre --extra-index https://pypi.anaconda.org/scientific-python-nightly-wheels/simple pandas
-      - name: install-polars-nightly
-        run: python -m pip install *.whl
       - name: Run pytest
-        run: pytest tests --cov=narwhals --cov=tests --cov-fail-under=50
+        run: pytest tests --cov=narwhals --cov=tests --cov-fail-under=50 --runslow
       - name: Run doctests
         run: pytest narwhals --doctest-modules
+
+  # polars-nightly:
+  #   if: github.ref == 'refs/heads/main'
+  #   strategy:
+  #     matrix:
+  #       python-version: ["3.12"]
+  #       os: [ubuntu-latest]
+
+  #   runs-on: ${{ matrix.os }}
+  #   steps:
+  #     - uses: actions/checkout@v3
+  #     - uses: actions/setup-python@v4
+  #       with:
+  #         python-version: ${{ matrix.python-version }}
+  #     - name: Cache multiple paths
+  #       uses: actions/cache@v3
+  #       with:
+  #         path: |
+  #           ~/.cache/pip
+  #           $RUNNER_TOOL_CACHE/Python/*
+  #           ~\AppData\Local\pip\Cache
+  #         key: ${{ runner.os }}-build-${{ matrix.python-version }}
+  #     - name: install-kaggle
+  #       run: python -m pip install kaggle
+  #     - name: Download Kaggle notebook artifact
+  #       env:
+  #         KAGGLE_USERNAME: ${{ secrets.KAGGLE_USERNAME }}
+  #         KAGGLE_KEY: ${{ secrets.KAGGLE_KEY }}
+  #       run: kaggle kernels output marcogorelli/polars-nightly
+  #     - name: install-reqs
+  #       run: python -m pip install --upgrade tox virtualenv setuptools pip -r requirements-dev.txt
+  #     - name: uninstall polars
+  #       run: python -m pip uninstall polars -y
+  #     - name: install-modin-pandas
+  #       run: pip install modin[dask] pandas
+  #     - name: install-polars-nightly
+  #       run: python -m pip install *.whl
+  #     - name: Run pytest
+  #       run: pytest tests --cov=narwhals --cov=tests --cov-fail-under=50
+  #     - name: Run doctests
+  #       run: pytest narwhals --doctest-modules
```

### Comparing `narwhals-0.7.9/.github/workflows/mkdocs.yml` & `narwhals-0.8.0/.github/workflows/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.9/.github/workflows/publish_to_pypi.yml` & `narwhals-0.8.0/.github/workflows/publish_to_pypi.yml`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.9/.github/workflows/pytest.yml` & `narwhals-0.8.0/.github/workflows/pytest.yml`

 * *Files 1% similar despite different names*

```diff
@@ -56,10 +56,10 @@
             ~\AppData\Local\pip\Cache
           key: ${{ runner.os }}-build-${{ matrix.python-version }}
       - name: install-reqs
         run: python -m pip install --upgrade tox virtualenv setuptools pip -r requirements-dev.txt
       - name: install-modin
         run: python -m pip install --upgrade modin[dask]
       - name: Run pytest
-        run: pytest tests --cov=narwhals --cov=tests --cov-fail-under=100
+        run: pytest tests --cov=narwhals --cov=tests --cov-fail-under=100 --runslow
       - name: Run doctests
         run: pytest narwhals --doctest-modules
```

### Comparing `narwhals-0.7.9/docs/extending.md` & `narwhals-0.8.0/docs/extending.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,26 @@
-# How Narwhals can support your dataframe as well!
+# List of supported libraries (and how to add yours!)
 
-Currently, Narwhals recognises the following libraries as inputs:
+Currently, Narwhals supports the following libraries as inputs:
 
 - pandas
 - Polars
 - cuDF
 - Modin
 
-If you want your own library to be recognised too, you can either open a PR (with tests) or
-you can make sure that, in addition to the public Narwhals API, you also define:
+If you want your own library to be recognised too, you're welcome open a PR (with tests)!
+Alternatively, if you can't do that (for example, if you library is closed-source), see
+the next section for what else you can do.
+
+## Extending Narwhals
+
+We love open source, but we're not "open source absolutists". If you're unable to open
+source you library, then this is how you can make your library compatible with Narwhals.
+
+Make sure that, in addition to the public Narwhals API, you also define:
 
   - `DataFrame.__narwhals_dataframe__`: return an object which implements public methods
     from `Narwhals.DataFrame`
   - `DataFrame.__narwhals_namespace__`: return an object which implements public top-level
     functions from `narwhals` (e.g. `narwhals.col`, `narwhals.concat`, ...)
   - `LazyFrame.__narwhals_lazyframe__`: return an object which implements public methods
     from `Narwhals.LazyFrame`
@@ -21,8 +29,12 @@
   - `Series.__narwhals_series__`: return an object which implements public methods
     from `Narwhals.Series`
   - `Series.__narwhals_namespace__`: return an object which implements public top-level
     functions from `narwhals` (e.g. `narwhals.col`, `narwhals.concat`, ...)
 
   If your library doesn't distinguish between lazy and eager, then it's OK for your dataframe
   object to implement both `__narwhals_dataframe__` and `__narwhals_lazyframe__`. In fact,
-  that's currently what `narwhals._pandas_like.dataframe.PandasDataFrame` does!
+  that's currently what `narwhals._pandas_like.dataframe.PandasDataFrame` does. So, if you're stuck,
+  take a look at the source code to see how it's done!
+
+Note that the "extension" mechanism is still experimental. If anything is not clear, or
+doesn't work, please do raise an issue or contact us on Discord (see the link on the README).
```

### Comparing `narwhals-0.7.9/docs/generate_members.py` & `narwhals-0.8.0/docs/generate_members.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.9/docs/index.md` & `narwhals-0.8.0/docs/index.md`

 * *Files 23% similar despite different names*

```diff
@@ -5,16 +5,17 @@
 Extremely lightweight compatibility layer between Polars, pandas, and more.
 
 Seamlessly support both, without depending on either!
 
 - ✅ **Just use** a subset of **the Polars API**, no need to learn anything new
 - ✅ **No dependencies** (not even Polars), keep your library lightweight
 - ✅ Support both **lazy** and eager execution
-- ✅ Use Polars **Expressions**
+- ✅ Use **Expressions**
 - ✅ Tested against pandas and Polars nightly builds!
+- ✅ Preserve your Index (if present) without it getting in the way!
 
 ## Who's this for?
 
 Anyone wishing to write a library/application/service which consumes dataframes, and wishing to make it
 completely dataframe-agnostic.
 
 Let's get started!
```

### Comparing `narwhals-0.7.9/docs/quick_start.md` & `narwhals-0.8.0/docs/quick_start.md`

 * *Files 5% similar despite different names*

```diff
@@ -33,7 +33,9 @@
 print('Polars output')
 print(my_function(df_polars))
 ```
 
 If you run `python t.py` then your output should look like the above. This is the simplest possible example of a dataframe-agnostic
 function - as we'll soon see, we can do much more advanced things.
 Let's learn about what you just did, and what Narwhals can do for you!
+
+Note: these examples are only using pandas and Polars. Please see the following to find the [supported libriaries](extending.md).
```

### Comparing `narwhals-0.7.9/docs/related.md` & `narwhals-0.8.0/docs/related.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.9/docs/roadmap.md` & `narwhals-0.8.0/docs/roadmap.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.9/docs/why.md` & `narwhals-0.8.0/docs/why.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Why?
 
-You may think that pandas and Polars are quite similar. But are they really?
+You may think that pandas, Polars, and all dataframe libraries are quite similar. But are they really?
 
 For example, do the following produce the same output?
 
 ```python
 import pandas as pd
 import polars as pl
```

### Comparing `narwhals-0.7.9/docs/api-reference/index.md` & `narwhals-0.8.0/docs/api-reference/index.md`

 * *Files 6% similar despite different names*

```diff
@@ -3,29 +3,27 @@
 Anything documented in the API reference is intended to work consistently among
 supported backends.
 
 For example:
 ```python
 import narwhals as nw
 
-nw: DataFrame
-nw.with_columns(
+df.with_columns(
     a_mean = nw.col('a').mean(),
     a_std = nw.col('a').std(),
 )
 ```
 is supported, as `DataFrame.with_columns`, `narwhals.col`, `Expr.mean`, and `Expr.std` are
 all documented in the API reference.
 
 However,
 ```python
 import narwhals as nw
 
-nw: DataFrame
-nw.with_columns(
+df.with_columns(
     a_ewm_mean = nw.col('a').ewm_mean(alpha=.7),
 )
 ```
 is not - `Expr.ewm_mean` only appears in the Polars API reference, but not in the Narwhals
 one.
 
 In general, you should expect any fundamental dataframe operation to be supported - if
```

### Comparing `narwhals-0.7.9/docs/api-reference/series.md` & `narwhals-0.8.0/docs/api-reference/series.md`

 * *Files 22% similar despite different names*

```diff
@@ -5,27 +5,27 @@
     options:
       members:
         - alias
         - all
         - any
         - cast
         - drop_nulls
-        - dt
         - dtype
+        - filter
         - is_between
         - is_in
         - is_null
         - max
         - mean
         - min
         - name
         - n_unique
         - sample
+        - shape
         - sort
         - std
-        - str
         - sum
         - to_numpy
         - to_pandas
         - unique
       show_source: false
       show_bases: false
```

### Comparing `narwhals-0.7.9/docs/assets/image.png` & `narwhals-0.8.0/docs/assets/image.png`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.9/docs/basics/column.md` & `narwhals-0.8.0/docs/basics/column.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # Series
 
-In [dataframe.md](dataframe.md), you learned how to write a dataframe-agnostic function.
+In [dataframe](dataframe.md), you learned how to write a dataframe-agnostic function.
 
 We only used DataFrame methods there - but what if we need to operate on its columns?
 
 Note that Polars does not have lazy columns. If you need to operate on columns as part of
 a dataframe operation, you should use expressions - but if you need to extract a single
-column, you need to ensure that you start with an eager `DataFrame`. To do that, we'll
-use the `nw.DataFrame` constructor, as opposed to `nw.from_native`.
+column, you need to ensure that you start with an eager `DataFrame`. To do that, you need
+to pass `eager_only=True` to `nw.from_native`.
 
 ## Example 1: filter based on a column's values
 
 This can stay lazy, so we just use `nw.from_native` and expressions:
 
 ```python exec="1" source="above" session="ex1"
 import narwhals as nw
@@ -120,22 +120,22 @@
     print(my_func(df).collect())
     ```
 
 ## Example 3: finding the mean of a column as a scalar
 
 Now, we want to find the mean of column `'a'`, and we need it as a Python scalar.
 This means that computation cannot stay lazy - it must execute!
-Therefore, instead of `nw.from_native`, we'll use `nw.DataFrame`, and then, instead
+Therefore, we'll pass `eager_only=True` to `nw.from_native`, and then, instead
 of using expressions, we'll extract a `Series`.
 
 ```python exec="1" source="above" session="ex2"
 import narwhals as nw
 
 def my_func(df):
-    df_s = nw.DataFrame(df)
+    df_s = nw.from_native(df, eager_only=True)
     return df_s['a'].mean()
 ```
 
 === "pandas"
     ```python exec="true" source="material-block" result="python" session="ex2"
     import pandas as pd
```

### Comparing `narwhals-0.7.9/docs/basics/complete_example.md` & `narwhals-0.8.0/docs/basics/complete_example.md`

 * *Files 7% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 
 ## Transform method
 
 The general strategy will be:
 
 1. Initialise a Narwhals DataFrame or LazyFrame by passing your dataframe to `nw.from_native`.
    
-    Note: if you need eager execution, use `nw.DataFrame` instead.
+    Note: if you need eager execution, make sure to pass `eager_only=True` to `nw.from_native`.
 
 2. Express your logic using the subset of the Polars API supported by Narwhals.
-3. If you need to return a dataframe to the user in its original library, call `narwhals.to_native`.
+3. If you need to return a dataframe to the user in its original library, call `nw.to_native`.
 
 ```python
 import narwhals as nw
 
 class StandardScalar:
     def transform(self, df):
         df = nw.from_native(df)
@@ -41,37 +41,37 @@
 Note that all the calculations here can stay lazy if the underlying library permits it.
 
 ## Fit method
 
 Unlike the `transform` method, `fit` cannot stay lazy, as we need to compute concrete values
 for the means and standard deviations.
 
-To be able to get `Series` out of our `DataFrame`, we'll need to use `narwhals.DataFrame` (as opposed to
-`narwhals.from_native`). This is because Polars doesn't have a concept of lazy `Series`, and so Narwhals
+To be able to get `Series` out of our `DataFrame`, we'll pass `eager_only=True` to `narwhals.from_native`.
+This is because Polars doesn't have a concept of lazy `Series`, and so Narwhals
 doesn't either.
 
 ```python
 import narwhals as nw
 
 class StandardScalar:
     def fit(self, df):
-        df = nw.DataFrame(df)
+        df = nw.from_native(df, eager_only=True)
         self._means = {col: df[col].mean() for col in df.columns}
         self._std_devs = {col: df[col].std() for col in df.columns}
 ```
 
 ## Putting it all together
 
 Here is our dataframe-agnostic standard scaler:
 ```python exec="1" source="above" session="tute-ex1"
 import narwhals as nw
 
 class StandardScaler:
     def fit(self, df):
-        df = nw.DataFrame(df)
+        df = nw.from_native(df, eager_only=True)
         self._means = {col: df[col].mean() for col in df.columns}
         self._std_devs = {col: df[col].std() for col in df.columns}
 
     def transform(self, df):
         df = nw.from_native(df)
         df = df.with_columns(
             (nw.col(col) - self._means[col]) / self._std_devs[col]
```

### Comparing `narwhals-0.7.9/narwhals/__init__.py` & `narwhals-0.8.0/narwhals/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from narwhals.expression import sum
 from narwhals.expression import sum_horizontal
 from narwhals.functions import concat
 from narwhals.series import Series
 from narwhals.translate import from_native
 from narwhals.translate import to_native
 
-__version__ = "0.7.9"
+__version__ = "0.8.0"
 
 __all__ = [
     "concat",
     "to_native",
     "from_native",
     "all",
     "col",
```

### Comparing `narwhals-0.7.9/narwhals/dtypes.py` & `narwhals-0.8.0/narwhals/dtypes.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.9/narwhals/functions.py` & `narwhals-0.8.0/narwhals/functions.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 from typing import Iterable
 from typing import Literal
 
+from narwhals.utils import validate_same_library
+
 if TYPE_CHECKING:
     from narwhals.dataframe import DataFrame
     from narwhals.dataframe import LazyFrame
 
 
 def concat(
     items: Iterable[DataFrame | LazyFrame],
@@ -17,13 +19,14 @@
     if how not in ("horizontal", "vertical"):
         raise NotImplementedError(
             "Only horizontal and vertical concatenations are supported"
         )
     if not items:
         raise ValueError("No items to concatenate")
     items = list(items)
+    validate_same_library(items)
     first_item = items[0]
     plx = first_item.__narwhals_namespace__()
     return first_item.__class__(
         plx.concat([df._dataframe for df in items], how=how),
         is_polars=first_item._is_polars,
     )
```

### Comparing `narwhals-0.7.9/narwhals/group_by.py` & `narwhals-0.8.0/narwhals/group_by.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.9/narwhals/series.py` & `narwhals-0.8.0/narwhals/series.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 from narwhals.dtypes import to_narwhals_dtype
 from narwhals.dtypes import translate_dtype
 from narwhals.translate import get_pandas
 from narwhals.translate import get_polars
 
 if TYPE_CHECKING:
+    import numpy as np
     from typing_extensions import Self
 
 
 class Series:
     def __init__(
         self,
         series: Any,
@@ -33,24 +34,31 @@
             return
         if (pd := get_pandas()) is not None and isinstance(series, pd.Series):
             self._series = PandasSeries(series, implementation="pandas")
             return
         msg = f"Expected pandas or Polars Series, got: {type(series)}"  # pragma: no cover
         raise TypeError(msg)  # pragma: no cover
 
+    def __array__(self, *args: Any, **kwargs: Any) -> np.ndarray:
+        return self._series.to_numpy(*args, **kwargs)
+
     def __getitem__(self, idx: int) -> Any:
         return self._series[idx]
 
     def __narwhals_namespace__(self) -> Any:
         if self._is_polars:
             import polars as pl
 
             return pl
         return self._series.__narwhals_namespace__()
 
+    @property
+    def shape(self) -> tuple[int]:
+        return self._series.shape  # type: ignore[no-any-return]
+
     def _extract_native(self, arg: Any) -> Any:
         from narwhals.series import Series
 
         if isinstance(arg, Series):
             return arg._series
         return arg
 
@@ -104,16 +112,16 @@
 
     def max(self) -> Any:
         return self._series.max()
 
     def sum(self) -> Any:
         return self._series.sum()
 
-    def std(self) -> Any:
-        return self._series.std()
+    def std(self, *, ddof: int = 1) -> Any:
+        return self._series.std(ddof=ddof)
 
     def is_in(self, other: Any) -> Self:
         return self._from_series(self._series.is_in(self._extract_native(other)))
 
     def drop_nulls(self) -> Self:
         return self._from_series(self._series.drop_nulls())
 
@@ -155,18 +163,36 @@
 
     def to_pandas(self) -> Any:
         return self._series.to_pandas()
 
     def __gt__(self, other: Any) -> Series:
         return self._from_series(self._series.__gt__(self._extract_native(other)))
 
+    def __ge__(self, other: Any) -> Series:  # pragma: no cover (todo)
+        return self._from_series(self._series.__ge__(self._extract_native(other)))
+
+    def __lt__(self, other: Any) -> Series:  # pragma: no cover (todo)
+        return self._from_series(self._series.__lt__(self._extract_native(other)))
+
+    def __le__(self, other: Any) -> Series:  # pragma: no cover (todo)
+        return self._from_series(self._series.__le__(self._extract_native(other)))
+
+    def __and__(self, other: Any) -> Series:  # pragma: no cover (todo)
+        return self._from_series(self._series.__and__(self._extract_native(other)))
+
+    def __or__(self, other: Any) -> Series:  # pragma: no cover (todo)
+        return self._from_series(self._series.__or__(self._extract_native(other)))
+
     # unary
     def __invert__(self) -> Series:
         return self._from_series(self._series.__invert__())
 
+    def filter(self, other: Any) -> Series:
+        return self._from_series(self._series.filter(self._extract_native(other)))
+
     @property
     def str(self) -> SeriesStringNamespace:
         return SeriesStringNamespace(self)
 
     @property
     def dt(self) -> SeriesDateTimeNamespace:
         return SeriesDateTimeNamespace(self)
```

### Comparing `narwhals-0.7.9/narwhals/_pandas_like/dataframe.py` & `narwhals-0.8.0/narwhals/_pandas_like/dataframe.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 from typing import Literal
 
 from narwhals._pandas_like.utils import evaluate_into_exprs
 from narwhals._pandas_like.utils import horizontal_concat
 from narwhals._pandas_like.utils import translate_dtype
 from narwhals._pandas_like.utils import validate_dataframe_comparand
 from narwhals._pandas_like.utils import validate_indices
-from narwhals.dependencies import get_pyarrow
 from narwhals.utils import flatten
 
 if TYPE_CHECKING:
     from collections.abc import Sequence
 
     from typing_extensions import Self
 
@@ -31,42 +30,28 @@
     def __init__(
         self,
         dataframe: Any,
         *,
         implementation: str,
     ) -> None:
         self._validate_columns(dataframe.columns)
-        self._dataframe = self._convert_object_dtypes(dataframe)
+        self._dataframe = dataframe
         self._implementation = implementation
 
     def __narwhals_dataframe__(self) -> Self:
         return self
 
     def __narwhals_lazyframe__(self) -> Self:
         return self
 
     def __narwhals_namespace__(self) -> PandasNamespace:
         from narwhals._pandas_like.namespace import PandasNamespace
 
         return PandasNamespace(self._implementation)
 
-    def _convert_object_dtypes(self, dataframe: Any) -> Any:
-        schema = dataframe.dtypes
-        if (schema != object).all():
-            return dataframe
-        replacements = {}
-        for col in dataframe.columns:
-            if schema[col] != object:
-                continue
-            if get_pyarrow() is not None:
-                replacements[col] = dataframe[col].astype("string[pyarrow]")
-            else:  # pragma: no cover
-                replacements[col] = dataframe[col].astype("string[python]")
-        return dataframe.assign(**replacements)
-
     def _validate_columns(self, columns: Sequence[str]) -> None:
         if len(columns) != len(set(columns)):
             counter = collections.Counter(columns)
             for col, count in counter.items():
                 if count > 1:
                     msg = f"Expected unique column names, got {col!r} {count} time(s)"
                     raise ValueError(
@@ -104,15 +89,15 @@
         self,
         *exprs: IntoPandasExpr | Iterable[IntoPandasExpr],
         **named_exprs: IntoPandasExpr,
     ) -> Self:
         new_series = evaluate_into_exprs(self, *exprs, **named_exprs)
         new_series = validate_indices(new_series)
         df = horizontal_concat(
-            [series._series for series in new_series],
+            new_series,
             implementation=self._implementation,
         )
         return self._from_dataframe(df)
 
     def filter(
         self,
         *predicates: IntoPandasExpr | Iterable[IntoPandasExpr],
@@ -223,14 +208,25 @@
     def to_dict(self, *, as_series: bool = False) -> dict[str, Any]:
         if as_series:
             # todo: should this return narwhals series?
             return {col: self._dataframe.loc[:, col] for col in self.columns}
         return self._dataframe.to_dict(orient="list")  # type: ignore[no-any-return]
 
     def to_numpy(self) -> Any:
+        from narwhals._pandas_like.series import PANDAS_TO_NUMPY_DTYPE_MISSING
+
+        # pandas return `object` dtype for nullable dtypes, so we cast each
+        # Series to numpy and let numpy find a common dtype.
+        # If there aren't any dtypes where `to_numpy()` is "broken" (i.e. it
+        # returns Object) then we just call `to_numpy()` on the DataFrame.
+        for dtype in self._dataframe.dtypes:
+            if str(dtype) in PANDAS_TO_NUMPY_DTYPE_MISSING:
+                import numpy as np
+
+                return np.hstack([self[col].to_numpy()[:, None] for col in self.columns])
         return self._dataframe.to_numpy()
 
     def to_pandas(self) -> Any:
         if self._implementation == "pandas":
             return self._dataframe
         if self._implementation == "modin":  # pragma: no cover
             return self._dataframe._to_pandas()
```

### Comparing `narwhals-0.7.9/narwhals/_pandas_like/expr.py` & `narwhals-0.8.0/narwhals/_pandas_like/expr.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from typing import TYPE_CHECKING
 from typing import Any
 from typing import Callable
 
 from narwhals._pandas_like.series import PandasSeries
 from narwhals._pandas_like.utils import register_expression_call
+from narwhals._pandas_like.utils import to_datetime
 
 if TYPE_CHECKING:
     from typing_extensions import Self
 
     from narwhals._pandas_like.dataframe import PandasDataFrame
 
 
@@ -147,16 +148,16 @@
 
     def sum(self) -> Self:
         return register_expression_call(self, "sum")
 
     def mean(self) -> Self:
         return register_expression_call(self, "mean")
 
-    def std(self) -> Self:
-        return register_expression_call(self, "std")
+    def std(self, *, ddof: int = 1) -> Self:
+        return register_expression_call(self, "std", ddof=ddof)
 
     def any(self) -> Self:
         return register_expression_call(self, "any")
 
     def all(self) -> Self:
         return register_expression_call(self, "all")
 
@@ -176,14 +177,17 @@
 
     def is_null(self) -> Self:
         return register_expression_call(self, "is_null")
 
     def is_in(self, other: Any) -> Self:
         return register_expression_call(self, "is_in", other)
 
+    def filter(self, other: Any) -> Self:
+        return register_expression_call(self, "filter", other)
+
     def drop_nulls(self) -> Self:
         return register_expression_call(self, "drop_nulls")
 
     def sort(self, *, descending: bool = False) -> Self:
         return register_expression_call(self, "sort", descending=descending)
 
     def n_unique(self) -> Self:
@@ -242,14 +246,31 @@
             depth=self._expr._depth + 1,
             function_name=f"{self._expr._function_name}->str.ends_with",
             root_names=self._expr._root_names,
             output_names=self._expr._output_names,
             implementation=self._expr._implementation,
         )
 
+    def to_datetime(self, format: str | None = None) -> PandasExpr:  # noqa: A002
+        # TODO make a register_expression_call for namespaces
+        return PandasExpr(
+            lambda df: [
+                PandasSeries(
+                    to_datetime(df._implementation)(series._series, format=format),
+                    implementation=df._implementation,
+                )
+                for series in self._expr._call(df)
+            ],
+            depth=self._expr._depth + 1,
+            function_name=f"{self._expr._function_name}->str.to_datetime",
+            root_names=self._expr._root_names,
+            output_names=self._expr._output_names,
+            implementation=self._expr._implementation,
+        )
+
 
 class PandasExprDateTimeNamespace:
     def __init__(self, expr: PandasExpr) -> None:
         self._expr = expr
 
     def year(self) -> PandasExpr:
         # TODO make a register_expression_call for namespaces
```

### Comparing `narwhals-0.7.9/narwhals/_pandas_like/group_by.py` & `narwhals-0.8.0/narwhals/_pandas_like/group_by.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.9/narwhals/_pandas_like/namespace.py` & `narwhals-0.8.0/narwhals/_pandas_like/namespace.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.9/narwhals/_pandas_like/series.py` & `narwhals-0.8.0/narwhals/_pandas_like/series.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+import warnings
 from typing import TYPE_CHECKING
 from typing import Any
 from typing import Sequence
 
 from narwhals._pandas_like.utils import item
 from narwhals._pandas_like.utils import reverse_translate_dtype
 from narwhals._pandas_like.utils import translate_dtype
@@ -12,14 +13,59 @@
 
 if TYPE_CHECKING:
     from typing_extensions import Self
 
     from narwhals._pandas_like.namespace import PandasNamespace
     from narwhals.dtypes import DType
 
+PANDAS_TO_NUMPY_DTYPE_NO_MISSING = {
+    "Int64": "int64",
+    "int64[pyarrow]": "int64",
+    "Int32": "int32",
+    "int32[pyarrow]": "int32",
+    "Int16": "int16",
+    "int16[pyarrow]": "int16",
+    "Int8": "int8",
+    "int8[pyarrow]": "int8",
+    "UInt64": "uint64",
+    "uint64[pyarrow]": "uint64",
+    "UInt32": "uint32",
+    "uint32[pyarrow]": "uint32",
+    "UInt16": "uint16",
+    "uint16[pyarrow]": "uint16",
+    "UInt8": "uint8",
+    "uint8[pyarrow]": "uint8",
+    "Float64": "float64",
+    "float64[pyarrow]": "float64",
+    "Float32": "float32",
+    "float32[pyarrow]": "float32",
+}
+PANDAS_TO_NUMPY_DTYPE_MISSING = {
+    "Int64": "float64",
+    "int64[pyarrow]": "float64",
+    "Int32": "float64",
+    "int32[pyarrow]": "float64",
+    "Int16": "float64",
+    "int16[pyarrow]": "float64",
+    "Int8": "float64",
+    "int8[pyarrow]": "float64",
+    "UInt64": "float64",
+    "uint64[pyarrow]": "float64",
+    "UInt32": "float64",
+    "uint32[pyarrow]": "float64",
+    "UInt16": "float64",
+    "uint16[pyarrow]": "float64",
+    "UInt8": "float64",
+    "uint8[pyarrow]": "float64",
+    "Float64": "float64",
+    "float64[pyarrow]": "float64",
+    "Float32": "float32",
+    "float32[pyarrow]": "float32",
+}
+
 
 class PandasSeries:
     def __init__(
         self,
         series: Any,
         *,
         implementation: str,
@@ -98,20 +144,32 @@
         ser = self._series
         return self._from_series(ser.between(lower_bound, upper_bound, inclusive=closed))
 
     def is_in(self, other: Any) -> PandasSeries:
         import pandas as pd
 
         ser = self._series
-        res = ser.isin(other).convert_dtypes()
+        with warnings.catch_warnings():
+            # np.find_common_type is deprecated.  Please use `np.result_type` or `np.promote_types`
+            warnings.filterwarnings(
+                "ignore",
+                message="np.find_common_type is deprecated.*",
+                category=DeprecationWarning,
+            )
+            res = ser.isin(other).convert_dtypes()
         res[ser.isna()] = pd.NA
         return self._from_series(res)
 
     # Binary comparisons
 
+    def filter(self, other: Any) -> PandasSeries:
+        ser = self._series
+        other = validate_column_comparand(self._series.index, other)
+        return self._from_series(self._rename(ser.loc[other], ser.name))
+
     def __eq__(self, other: object) -> PandasSeries:  # type: ignore[override]
         ser = self._series
         other = validate_column_comparand(self._series.index, other)
         return self._from_series(self._rename(ser.__eq__(other), ser.name))
 
     def __ne__(self, other: object) -> PandasSeries:  # type: ignore[override]
         ser = self._series
@@ -259,18 +317,18 @@
     def mean(self) -> Any:
         ser = self._series
         return ser.mean()
 
     def std(
         self,
         *,
-        correction: float = 1.0,
+        ddof: int = 1,
     ) -> Any:
         ser = self._series
-        return ser.std(ddof=correction)
+        return ser.std(ddof=ddof)
 
     def len(self) -> Any:
         return len(self._series)
 
     # Transformations
 
     def is_null(self) -> PandasSeries:
@@ -313,14 +371,27 @@
         )
 
     def alias(self, name: str) -> Self:
         ser = self._series
         return self._from_series(self._rename(ser, name))
 
     def to_numpy(self) -> Any:
+        has_missing = self._series.isna().any()
+        if has_missing and str(self._series.dtype) in PANDAS_TO_NUMPY_DTYPE_MISSING:
+            return self._series.to_numpy(
+                dtype=PANDAS_TO_NUMPY_DTYPE_MISSING[str(self._series.dtype)],
+                na_value=float("nan"),
+            )
+        if (
+            not has_missing
+            and str(self._series.dtype) in PANDAS_TO_NUMPY_DTYPE_NO_MISSING
+        ):
+            return self._series.to_numpy(
+                dtype=PANDAS_TO_NUMPY_DTYPE_NO_MISSING[str(self._series.dtype)]
+            )
         return self._series.to_numpy()
 
     def to_pandas(self) -> Any:
         if self._implementation == "pandas":
             return self._series
         elif self._implementation == "cudf":  # pragma: no cover
             return self._series.to_pandas()
```

### Comparing `narwhals-0.7.9/narwhals/_pandas_like/utils.py` & `narwhals-0.8.0/narwhals/_pandas_like/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,17 @@
 
 from copy import copy
 from typing import TYPE_CHECKING
 from typing import Any
 from typing import Iterable
 from typing import TypeVar
 
+from narwhals.dependencies import get_cudf
+from narwhals.dependencies import get_modin
+from narwhals.dependencies import get_pandas
 from narwhals.dependencies import get_pyarrow
 from narwhals.utils import flatten
 from narwhals.utils import isinstance_or_issubclass
 from narwhals.utils import parse_version
 
 T = TypeVar("T")
 
@@ -45,19 +48,15 @@
     if isinstance(other, PandasDataFrame):
         return NotImplemented
     if isinstance(other, PandasSeries):
         if other.len() == 1:
             # broadcast
             return other.item()
         if other._series.index is not index and not (other._series.index == index).all():
-            msg = (
-                "Narwhals does not support automated index alignment. "
-                "You may need to do a join before this operation."
-            )
-            raise ValueError(msg)
+            return other._series.set_axis(index, axis=0)
         return other._series
     return other
 
 
 def validate_dataframe_comparand(index: Any, other: Any) -> Any:
     """Validate RHS of binary operation.
 
@@ -70,19 +69,15 @@
     if isinstance(other, PandasDataFrame):
         return NotImplemented
     if isinstance(other, PandasSeries):
         if other.len() == 1:
             # broadcast
             return item(other._series)
         if other._series.index is not index and not (other._series.index == index).all():
-            msg = (
-                "Narwhals does not support automated index alignment. "
-                "You may need to do a join before this operation."
-            )
-            raise ValueError(msg)
+            return other._series.set_axis(index, axis=0)
         return other._series
     raise AssertionError("Please report a bug")
 
 
 def maybe_evaluate_expr(df: PandasDataFrame, arg: Any) -> Any:
     """Evaluate expression if it's an expression, otherwise return it as is."""
     from narwhals._pandas_like.expr import PandasExpr
@@ -316,14 +311,16 @@
     if dtype in ("string", "string[python]", "string[pyarrow]"):
         return dtypes.String()
     if dtype in ("bool", "boolean", "boolean[pyarrow]"):
         return dtypes.Boolean()
     if str(dtype).startswith("datetime64"):
         # todo: different time units and time zones
         return dtypes.Datetime()
+    if dtype == "object":
+        return dtypes.String()
     msg = f"Unknown dtype: {dtype}"  # pragma: no cover
     raise AssertionError(msg)
 
 
 def reverse_translate_dtype(dtype: DType | type[DType]) -> Any:
     # Use the default pandas dtype here
     # TODO: maybe this could be configurable?
@@ -346,29 +343,42 @@
     if isinstance_or_issubclass(dtype, dtypes.UInt32):
         return "uint32"
     if isinstance_or_issubclass(dtype, dtypes.UInt16):
         return "uint16"
     if isinstance_or_issubclass(dtype, dtypes.UInt8):
         return "uint8"
     if isinstance_or_issubclass(dtype, dtypes.String):
-        if get_pyarrow() is not None:
-            return "string[pyarrow]"
-        return "string[python]"  # pragma: no cover
+        import pandas as pd
+
+        if parse_version(pd.__version__) >= parse_version("2.0.0"):
+            if get_pyarrow() is not None:
+                return "string[pyarrow]"
+            return "string[python]"  # pragma: no cover
+        return "object"  # pragma: no cover
     if isinstance_or_issubclass(dtype, dtypes.Boolean):
         return "bool"
     if isinstance_or_issubclass(dtype, dtypes.Datetime):
         # todo: different time units and time zones
         return "datetime64[us]"
     msg = f"Unknown dtype: {dtype}"  # pragma: no cover
     raise AssertionError(msg)
 
 
-def validate_indices(series: list[PandasSeries]) -> list[PandasSeries]:
+def validate_indices(series: list[PandasSeries]) -> list[Any]:
     idx = series[0]._series.index
+    reindexed = [series[0]._series]
     for s in series[1:]:
         if s._series.index is not idx and not (s._series.index == idx).all():
-            msg = (
-                "Narwhals does not support automated index alignment. "
-                "You may need to do a join before this operation."
-            )
-            raise RuntimeError(msg)
-    return series
+            reindexed.append(s._series.set_axis(idx.rename(s._series.index.name), axis=0))
+        else:
+            reindexed.append(s._series)
+    return reindexed
+
+
+def to_datetime(implementation: str) -> Any:
+    if implementation == "pandas":
+        return get_pandas().to_datetime
+    if implementation == "modin":
+        return get_modin().to_datetime
+    if implementation == "cudf":
+        return get_cudf().to_datetime
+    raise AssertionError
```

### Comparing `narwhals-0.7.9/tests/test_common.py` & `narwhals-0.8.0/tests/test_common.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,50 +8,58 @@
 import pandas as pd
 import polars as pl
 import pytest
 from pandas.testing import assert_series_equal as pd_assert_series_equal
 from polars.testing import assert_series_equal as pl_assert_series_equal
 
 import narwhals as nw
+from narwhals.utils import parse_version
 from tests.utils import compare_dicts
 
 df_pandas = pd.DataFrame({"a": [1, 3, 2], "b": [4, 4, 6], "z": [7.0, 8, 9]})
-df_pandas_nullable = pd.DataFrame(
-    {"a": [1, 3, 2], "b": [4, 4, 6], "z": [7.0, 8, 9]}
-).astype(
-    {
-        "a": "Int64",
-        "b": "Int64",
-        "z": "Float64",
-    }
-)
-df_pandas_pyarrow = pd.DataFrame(
-    {"a": [1, 3, 2], "b": [4, 4, 6], "z": [7.0, 8, 9]}
-).astype(
-    {
-        "a": "Int64[pyarrow]",
-        "b": "Int64[pyarrow]",
-        "z": "Float64[pyarrow]",
-    }
-)
+if parse_version(pd.__version__) >= parse_version("1.5.0"):
+    df_pandas_pyarrow = pd.DataFrame(
+        {"a": [1, 3, 2], "b": [4, 4, 6], "z": [7.0, 8, 9]}
+    ).astype(
+        {
+            "a": "Int64[pyarrow]",
+            "b": "Int64[pyarrow]",
+            "z": "Float64[pyarrow]",
+        }
+    )
+    df_pandas_nullable = pd.DataFrame(
+        {"a": [1, 3, 2], "b": [4, 4, 6], "z": [7.0, 8, 9]}
+    ).astype(
+        {
+            "a": "Int64",
+            "b": "Int64",
+            "z": "Float64",
+        }
+    )
+else:  # pragma: no cover
+    df_pandas_pyarrow = df_pandas
+    df_pandas_nullable = df_pandas
 df_polars = pl.DataFrame({"a": [1, 3, 2], "b": [4, 4, 6], "z": [7.0, 8, 9]})
 df_lazy = pl.LazyFrame({"a": [1, 3, 2], "b": [4, 4, 6], "z": [7.0, 8, 9]})
 df_pandas_na = pd.DataFrame({"a": [None, 3, 2], "b": [4, 4, 6], "z": [7.0, None, 9]})
 df_lazy_na = pl.LazyFrame({"a": [None, 3, 2], "b": [4, 4, 6], "z": [7.0, None, 9]})
 df_right_pandas = pd.DataFrame({"c": [6, 12, -1], "d": [0, -4, 2]})
 df_right_lazy = pl.LazyFrame({"c": [6, 12, -1], "d": [0, -4, 2]})
 
 if os.environ.get("CI", None):
-    import modin.pandas as mpd
-
-    with warnings.catch_warnings():
-        warnings.filterwarnings("ignore", category=UserWarning)
-        df_mpd = mpd.DataFrame(
-            pd.DataFrame({"a": [1, 3, 2], "b": [4, 4, 6], "z": [7.0, 8, 9]})
-        )
+    try:
+        import modin.pandas as mpd
+    except ImportError:  # pragma: no cover
+        df_mpd = df_pandas.copy()
+    else:
+        with warnings.catch_warnings():
+            warnings.filterwarnings("ignore", category=UserWarning)
+            df_mpd = mpd.DataFrame(
+                pd.DataFrame({"a": [1, 3, 2], "b": [4, 4, 6], "z": [7.0, 8, 9]})
+            )
 else:  # pragma: no cover
     df_mpd = df_pandas.copy()
 
 
 @pytest.mark.parametrize(
     "df_raw",
     [df_pandas, df_polars, df_lazy, df_pandas_nullable, df_pandas_pyarrow],
@@ -123,14 +131,38 @@
     compare_dicts(result_native, expected)
 
 
 @pytest.mark.parametrize(
     "df_raw",
     [df_pandas, df_lazy, df_pandas_nullable, df_pandas_pyarrow],
 )
+def test_std(df_raw: Any) -> None:
+    df = nw.LazyFrame(df_raw)
+    result = df.select(
+        nw.col("a").std().alias("a_ddof_default"),
+        nw.col("a").std(ddof=1).alias("a_ddof_1"),
+        nw.col("a").std(ddof=0).alias("a_ddof_0"),
+        nw.col("b").std(ddof=2).alias("b_ddof_2"),
+        nw.col("z").std(ddof=0).alias("z_ddof_0"),
+    )
+    result_native = nw.to_native(result)
+    expected = {
+        "a_ddof_default": [1.0],
+        "a_ddof_1": [1.0],
+        "a_ddof_0": [0.816497],
+        "b_ddof_2": [1.632993],
+        "z_ddof_0": [0.816497],
+    }
+    compare_dicts(result_native, expected)
+
+
+@pytest.mark.parametrize(
+    "df_raw",
+    [df_pandas, df_lazy, df_pandas_nullable, df_pandas_pyarrow],
+)
 def test_double(df_raw: Any) -> None:
     df = nw.LazyFrame(df_raw)
     result = df.with_columns(nw.all() * 2)
     result_native = nw.to_native(result)
     expected = {"a": [2, 6, 4], "b": [8, 8, 12], "z": [14.0, 16.0, 18.0]}
     compare_dicts(result_native, expected)
     result = df.with_columns(nw.col("a").alias("o"), nw.all() * 2)
@@ -318,22 +350,28 @@
 @pytest.mark.filterwarnings("ignore:.*Passing a BlockManager.*:DeprecationWarning")
 def test_convert_pandas(df_raw: Any) -> None:
     result = nw.from_native(df_raw).to_pandas()  # type: ignore[union-attr]
     expected = pd.DataFrame({"a": [1, 3, 2], "b": [4, 4, 6], "z": [7.0, 8, 9]})
     pd.testing.assert_frame_equal(result, expected)
 
 
-@pytest.mark.parametrize("df_raw", [df_polars, df_pandas, df_mpd])
+@pytest.mark.parametrize(
+    "df_raw", [df_polars, df_pandas, df_mpd, df_pandas_nullable, df_pandas_pyarrow]
+)
 @pytest.mark.filterwarnings(
     r"ignore:np\.find_common_type is deprecated\.:DeprecationWarning"
 )
 def test_convert_numpy(df_raw: Any) -> None:
     result = nw.DataFrame(df_raw).to_numpy()
     expected = np.array([[1, 3, 2], [4, 4, 6], [7.0, 8, 9]]).T
     np.testing.assert_array_equal(result, expected)
+    assert result.dtype == "float64"
+    result = nw.DataFrame(df_raw).__array__()
+    np.testing.assert_array_equal(result, expected)
+    assert result.dtype == "float64"
 
 
 @pytest.mark.parametrize("df_raw", [df_polars, df_pandas, df_mpd])
 def test_shape(df_raw: Any) -> None:
     result = nw.DataFrame(df_raw).shape
     expected = (3, 3)
     assert result == expected
@@ -560,24 +598,51 @@
     compare_dicts(result, expected)
 
 
 def test_invalid() -> None:
     df = nw.LazyFrame(df_pandas)
     with pytest.raises(ValueError, match="Multi-output"):
         df.select(nw.all() + nw.all())
+    with pytest.raises(TypeError, match="Perhaps you:"):
+        df.select([pl.col("a")])  # type: ignore[list-item]
 
 
 @pytest.mark.parametrize("df_raw", [df_pandas])
 def test_reindex(df_raw: Any) -> None:
     df = nw.DataFrame(df_raw)
-    with pytest.raises(RuntimeError, match="automated index alignment"):
-        df.select("a", df["b"].sort(descending=True))
-    with pytest.raises(RuntimeError, match="automated index alignment"):
-        df.select("a", nw.col("b").sort(descending=True))
+    result = df.select("b", df["a"].sort(descending=True))
+    expected = {"b": [4, 4, 6], "a": [3, 2, 1]}
+    compare_dicts(result, expected)
+    result = df.select("b", nw.col("a").sort(descending=True))
+    compare_dicts(result, expected)
 
     s = df["a"]
-    with pytest.raises(ValueError, match="index alignment"):
-        nw.to_native(s > s.sort())
-    with pytest.raises(ValueError, match="index alignment"):
-        nw.to_native(df.with_columns(s.sort()))
+    result_s = s > s.sort()
+    assert not result_s[0]
+    assert result_s[1]
+    assert not result_s[2]
+    result = df.with_columns(s.sort())
+    expected = {"a": [1, 2, 3], "b": [4, 4, 6], "z": [7.0, 8.0, 9.0]}  # type: ignore[list-item]
+    compare_dicts(result, expected)
     with pytest.raises(ValueError, match="Multi-output expressions are not supported"):
         nw.to_native(df.with_columns(nw.all() + nw.all()))
+
+
+@pytest.mark.parametrize(
+    ("df_raw", "df_raw_right"),
+    [(df_pandas, df_polars), (df_polars, df_pandas)],
+)
+def test_library(df_raw: Any, df_raw_right: Any) -> None:
+    df_left = nw.LazyFrame(df_raw)
+    df_right = nw.LazyFrame(df_raw_right)
+    with pytest.raises(
+        NotImplementedError, match="Cross-library comparisons aren't supported"
+    ):
+        nw.concat([df_left, df_right], how="horizontal")
+    with pytest.raises(
+        NotImplementedError, match="Cross-library comparisons aren't supported"
+    ):
+        nw.concat([df_left, df_right], how="vertical")
+    with pytest.raises(
+        NotImplementedError, match="Cross-library comparisons aren't supported"
+    ):
+        df_left.join(df_right, left_on=["a"], right_on=["a"], how="inner")
```

### Comparing `narwhals-0.7.9/tests/test_group_by.py` & `narwhals-0.8.0/tests/test_group_by.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.9/tests/test_series.py` & `narwhals-0.8.0/tests/test_series.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,64 +6,82 @@
 import pandas as pd
 import polars as pl
 import pytest
 from numpy.testing import assert_array_equal
 from pandas.testing import assert_series_equal
 
 import narwhals as nw
+from narwhals.utils import parse_version
 
 df_pandas = pd.DataFrame({"a": [1, 3, 2], "b": [4, 4, 6], "z": [7.0, 8, 9]})
-df_pandas_nullable = pd.DataFrame(
-    {"a": [1, 3, 2], "b": [4, 4, 6], "z": [7.0, 8, 9]}
-).astype(
-    {
-        "a": "Int64",
-        "b": "Int64",
-        "z": "Float64",
-    }
-)
-df_pandas_pyarrow = pd.DataFrame(
-    {"a": [1, 3, 2], "b": [4, 4, 6], "z": [7.0, 8, 9]}
-).astype(
-    {
-        "a": "Int64[pyarrow]",
-        "b": "Int64[pyarrow]",
-        "z": "Float64[pyarrow]",
-    }
-)
+if parse_version(pd.__version__) >= parse_version("1.5.0"):
+    df_pandas_pyarrow = pd.DataFrame(
+        {"a": [1, 3, 2], "b": [4, 4, 6], "z": [7.0, 8, 9]}
+    ).astype(
+        {
+            "a": "Int64[pyarrow]",
+            "b": "Int64[pyarrow]",
+            "z": "Float64[pyarrow]",
+        }
+    )
+    df_pandas_nullable = pd.DataFrame(
+        {"a": [1, 3, 2], "b": [4, 4, 6], "z": [7.0, 8, 9]}
+    ).astype(
+        {
+            "a": "Int64",
+            "b": "Int64",
+            "z": "Float64",
+        }
+    )
+else:  # pragma: no cover
+    # pyarrow/nullable dtypes not supported so far back
+    df_pandas_pyarrow = df_pandas
+    df_pandas_nullable = df_pandas
 df_polars = pl.DataFrame({"a": [1, 3, 2], "b": [4, 4, 6], "z": [7.0, 8, 9]})
 df_lazy = pl.LazyFrame({"a": [1, 3, 2], "b": [4, 4, 6], "z": [7.0, 8, 9]})
 
 
 @pytest.mark.parametrize(
     "df_raw", [df_pandas, df_polars, df_pandas_nullable, df_pandas_pyarrow]
 )
 def test_len(df_raw: Any) -> None:
     result = len(nw.Series(df_raw["a"]))
     assert result == 3
-    result = len(nw.to_native(nw.LazyFrame(df_raw).collect()["a"]))
+    result = len(nw.LazyFrame(df_raw).collect()["a"])
     assert result == 3
 
 
 @pytest.mark.parametrize("df_raw", [df_pandas, df_polars])
+@pytest.mark.filterwarnings("ignore:np.find_common_type is deprecated:DeprecationWarning")
 def test_is_in(df_raw: Any) -> None:
-    result = nw.to_native(nw.Series(df_raw["a"]).is_in([1, 2]))
+    result = nw.from_native(df_raw["a"], series_only=True).is_in([1, 2])
     assert result[0]
     assert not result[1]
     assert result[2]
 
 
 @pytest.mark.parametrize("df_raw", [df_pandas, df_polars])
+@pytest.mark.filterwarnings("ignore:np.find_common_type is deprecated:DeprecationWarning")
+def test_filter(df_raw: Any) -> None:
+    result = nw.from_native(df_raw["a"], series_only=True).filter(df_raw["a"] > 1)
+    expected = np.array([3, 2])
+    assert (result.to_numpy() == expected).all()
+    result = nw.DataFrame(df_raw).select(nw.col("a").filter(nw.col("a") > 1))["a"]
+    expected = np.array([3, 2])
+    assert (result.to_numpy() == expected).all()
+
+
+@pytest.mark.parametrize("df_raw", [df_pandas, df_polars])
 def test_gt(df_raw: Any) -> None:
     s = nw.Series(df_raw["a"])
-    result = nw.to_native(s > s)  # noqa: PLR0124
+    result = s > s  # noqa: PLR0124
     assert not result[0]
     assert not result[1]
     assert not result[2]
-    result = nw.to_native(s > 1)
+    result = s > 1
     assert not result[0]
     assert result[1]
     assert result[2]
 
 
 @pytest.mark.parametrize(
     "df_raw", [df_pandas, df_lazy, df_pandas_nullable, df_pandas_pyarrow]
@@ -229,15 +247,15 @@
         "j": nw.Float64,
         "k": nw.String,
         "l": nw.Datetime,
         "m": nw.Int8,
         "n": nw.Boolean,
     }
     assert result == expected
-    result_pd = nw.from_native(df.to_pandas()).schema
+    result_pd = nw.DataFrame(df.to_pandas()).schema
     assert result_pd == expected
     result = df.select(
         df["a"].cast(nw.Int32),
         df["b"].cast(nw.Int16),
         df["c"].cast(nw.Int8),
         df["d"].cast(nw.Int64),
         df["e"].cast(nw.UInt32),
@@ -281,7 +299,16 @@
         df["j"].cast(nw.Float64),
         df["k"].cast(nw.String),
         df["l"].cast(nw.Datetime),
         df["m"].cast(nw.Int8),
         n=df["m"].cast(nw.Boolean),
     ).schema
     assert result == expected
+
+
+def test_to_numpy() -> None:
+    s = pd.Series([1, 2, None], dtype="Int64")
+    result = nw.Series(s).to_numpy()
+    assert result.dtype == "float64"
+    result = nw.Series(s).__array__()
+    assert result.dtype == "float64"
+    assert nw.Series(s).shape == (3,)
```

### Comparing `narwhals-0.7.9/tests/test_str.py` & `narwhals-0.8.0/tests/test_str.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,19 +11,22 @@
 import narwhals as nw
 from tests.utils import compare_dicts
 
 df_pandas = pd.DataFrame({"a": ["fdas", "edfas"]})
 df_polars = pl.LazyFrame({"a": ["fdas", "edfas"]})
 
 if os.environ.get("CI", None):
-    import modin.pandas as mpd
-
-    with warnings.catch_warnings():
-        warnings.filterwarnings("ignore", category=UserWarning)
-        df_mpd = mpd.DataFrame({"a": ["fdas", "edfas"]})
+    try:
+        import modin.pandas as mpd
+    except ImportError:  # pragma: no cover
+        df_mpd = df_pandas.copy()
+    else:
+        with warnings.catch_warnings():
+            warnings.filterwarnings("ignore", category=UserWarning)
+            df_mpd = mpd.DataFrame({"a": ["fdas", "edfas"]})
 else:  # pragma: no cover
     df_mpd = df_pandas.copy()
 
 
 @pytest.mark.parametrize(
     "df_raw",
     [df_pandas, df_polars, df_mpd],
```

### Comparing `narwhals-0.7.9/tests/tpch_q1_test.py` & `narwhals-0.8.0/tests/tpch_q1_test.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.9/tests/utils.py` & `narwhals-0.8.0/tests/utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+import math
 from typing import Any
 from typing import Iterator
 from typing import Sequence
 
 
 def zip_longest(left: Sequence[Any], right: Sequence[Any]) -> Iterator[Any]:
     if len(left) != len(right):
@@ -17,11 +18,13 @@
     if hasattr(result, "collect"):
         result = result.collect()
     if hasattr(result, "columns"):
         for key in result.columns:
             assert key in expected
     for key in expected:
         for lhs, rhs in zip_longest(result[key], expected[key]):
-            if isinstance(lhs, float):
-                assert abs(lhs - rhs) < 1e-6, (lhs, rhs)
+            if isinstance(lhs, float) and not math.isnan(lhs):
+                assert math.isclose(lhs, rhs, rel_tol=0, abs_tol=1e-6), (lhs, rhs)
+            elif isinstance(lhs, float) and math.isnan(lhs):
+                assert math.isnan(rhs), (lhs, rhs)  # pragma: no cover
             else:
                 assert lhs == rhs, (lhs, rhs)
```

### Comparing `narwhals-0.7.9/tests/data/customer.parquet` & `narwhals-0.8.0/tests/data/customer.parquet`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.9/tests/data/lineitem.parquet` & `narwhals-0.8.0/tests/data/lineitem.parquet`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.9/tests/data/nation.parquet` & `narwhals-0.8.0/tests/data/nation.parquet`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.9/tests/data/orders.parquet` & `narwhals-0.8.0/tests/data/orders.parquet`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.9/tests/data/part.parquet` & `narwhals-0.8.0/tests/data/part.parquet`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.9/tests/data/partsupp.parquet` & `narwhals-0.8.0/tests/data/partsupp.parquet`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.9/tests/data/region.parquet` & `narwhals-0.8.0/tests/data/region.parquet`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.9/tests/data/supplier.parquet` & `narwhals-0.8.0/tests/data/supplier.parquet`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.9/tpch/q1.py` & `narwhals-0.8.0/tpch/q1.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.9/tpch/q2.py` & `narwhals-0.8.0/tpch/q2.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.9/tpch/q3.py` & `narwhals-0.8.0/tpch/q3.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.9/tpch/q4.py` & `narwhals-0.8.0/tpch/q4.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.9/tpch/q5.py` & `narwhals-0.8.0/tpch/q5.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.9/tpch/notebooks/gpu/execute.ipynb` & `narwhals-0.8.0/tpch/notebooks/gpu/execute.ipynb`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.9/tpch/notebooks/q1/execute.ipynb` & `narwhals-0.8.0/tpch/notebooks/q1/execute.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999780701754386%*

 * *Differences: {"'cells'": '{8: {\'source\': {insert: [(3, "results[tool+\'[native]\'] = timings.best")], delete: '*

 * *            '[3]}}}'}*

```diff
@@ -284,15 +284,15 @@
                     "output_type": "display_data"
                 }
             ],
             "source": [
                 "tool = 'pandas[pyarrow]'\n",
                 "fn = IO_FUNCS[tool]\n",
                 "timings = %timeit -o q1_pandas_native(fn(lineitem))\n",
-                "results[tool+'native'] = timings.best"
+                "results[tool+'[native]'] = timings.best"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "09249944",
             "metadata": {
                 "papermill": {
```

### Comparing `narwhals-0.7.9/tpch/notebooks/q2/execute.ipynb` & `narwhals-0.8.0/tpch/notebooks/q2/execute.ipynb`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9993298418744229%*

 * *Differences: {"'cells'": "{2: {'source': {insert: [(12, '\\n'), (13, '    jn = (\\n'), (14, '        "*

 * *            'part_ds.merge(part_supp_ds, left_on="p_partkey", right_on="ps_partkey")\\n\'), (15, '*

 * *            '\'        .merge(supplier_ds, left_on="ps_suppkey", right_on="s_suppkey")\\n\'), (16, '*

 * *            '\'        .merge(nation_ds, left_on="s_nationkey", right_on="n_nationkey")\\n\'), '*

 * *            '(17, \'        .merge(region_ds, left_on="n_regionkey", '*

 * *            'right_on="r_regionkey")\\n\'), (19, \'\\n […]*

```diff
@@ -94,130 +94,49 @@
                 "    supplier_ds: Any,\n",
                 "    part_ds: Any,\n",
                 "    part_supp_ds: Any,\n",
                 "):\n",
                 "    var1 = 15\n",
                 "    var2 = \"BRASS\"\n",
                 "    var3 = \"EUROPE\"\n",
-                "    nation_filtered = nation_ds.loc[:, [\"n_nationkey\", \"n_name\", \"n_regionkey\"]]\n",
-                "    region_filtered = region_ds[(region_ds[\"r_name\"] == var3)]\n",
-                "    region_filtered = region_filtered.loc[:, [\"r_regionkey\"]]\n",
-                "    r_n_merged = nation_ds.merge(\n",
-                "        region_ds, left_on=\"n_regionkey\", right_on=\"r_regionkey\", how=\"inner\"\n",
-                "    )\n",
-                "    # r_n_merged = r_n_merged.loc[:, [\"n_nationkey\", \"n_name\"]]\n",
-                "    # supplier_filtered = supplier_ds.loc[\n",
-                "    #     :,\n",
-                "    #     [\n",
-                "    #         \"s_suppkey\",\n",
-                "    #         \"s_name\",\n",
-                "    #         \"s_address\",\n",
-                "    #         \"s_nationkey\",\n",
-                "    #         \"s_phone\",\n",
-                "    #         \"s_acctbal\",\n",
-                "    #         \"s_comment\",\n",
-                "    #     ],\n",
-                "    # ]\n",
-                "    s_r_n_merged = r_n_merged.merge(\n",
-                "        supplier_ds,\n",
-                "        left_on=\"n_nationkey\",\n",
-                "        right_on=\"s_nationkey\",\n",
-                "        how=\"inner\",\n",
-                "    )\n",
-                "    s_r_n_merged = s_r_n_merged.loc[\n",
-                "        :,\n",
-                "        [\n",
-                "            \"n_name\",\n",
-                "            \"s_suppkey\",\n",
-                "            \"s_name\",\n",
-                "            \"s_address\",\n",
-                "            \"s_phone\",\n",
-                "            \"s_acctbal\",\n",
-                "            \"s_comment\",\n",
-                "        ],\n",
-                "    ]\n",
-                "    partsupp_filtered = part_supp_ds.loc[\n",
-                "        :, [\"ps_partkey\", \"ps_suppkey\", \"ps_supplycost\"]\n",
-                "    ]\n",
-                "    ps_s_r_n_merged = s_r_n_merged.merge(\n",
-                "        partsupp_filtered, left_on=\"s_suppkey\", right_on=\"ps_suppkey\", how=\"inner\"\n",
-                "    )\n",
-                "    ps_s_r_n_merged = ps_s_r_n_merged.loc[\n",
-                "        :,\n",
-                "        [\n",
-                "            \"n_name\",\n",
-                "            \"s_name\",\n",
-                "            \"s_address\",\n",
-                "            \"s_phone\",\n",
-                "            \"s_acctbal\",\n",
-                "            \"s_comment\",\n",
-                "            \"ps_partkey\",\n",
-                "            \"ps_supplycost\",\n",
-                "        ],\n",
-                "    ]\n",
-                "    part_filtered = part_ds.loc[:, [\"p_partkey\", \"p_mfgr\", \"p_size\", \"p_type\"]]\n",
-                "    part_filtered = part_filtered[\n",
-                "        (part_filtered[\"p_size\"] == var1)\n",
-                "        & (part_filtered[\"p_type\"].str.endswith(var2))\n",
-                "    ]\n",
-                "    part_filtered = part_filtered.loc[:, [\"p_partkey\", \"p_mfgr\"]]\n",
-                "    merged_df = part_filtered.merge(\n",
-                "        ps_s_r_n_merged, left_on=\"p_partkey\", right_on=\"ps_partkey\", how=\"inner\"\n",
-                "    )\n",
-                "    merged_df = merged_df.loc[\n",
-                "        :,\n",
-                "        [\n",
-                "            \"n_name\",\n",
-                "            \"s_name\",\n",
-                "            \"s_address\",\n",
-                "            \"s_phone\",\n",
-                "            \"s_acctbal\",\n",
-                "            \"s_comment\",\n",
-                "            \"ps_supplycost\",\n",
-                "            \"p_partkey\",\n",
-                "            \"p_mfgr\",\n",
-                "        ],\n",
-                "    ]\n",
-                "    min_values = merged_df.groupby(\"p_partkey\", as_index=False)[\n",
-                "        \"ps_supplycost\"\n",
-                "    ].min()\n",
-                "    min_values.columns = [\"P_PARTKEY_CPY\", \"MIN_SUPPLYCOST\"]\n",
-                "    merged_df = merged_df.merge(\n",
-                "        min_values,\n",
-                "        left_on=[\"p_partkey\", \"ps_supplycost\"],\n",
-                "        right_on=[\"P_PARTKEY_CPY\", \"MIN_SUPPLYCOST\"],\n",
-                "        how=\"inner\",\n",
-                "    )\n",
-                "    result_df = merged_df.loc[\n",
+                "\n",
+                "    jn = (\n",
+                "        part_ds.merge(part_supp_ds, left_on=\"p_partkey\", right_on=\"ps_partkey\")\n",
+                "        .merge(supplier_ds, left_on=\"ps_suppkey\", right_on=\"s_suppkey\")\n",
+                "        .merge(nation_ds, left_on=\"s_nationkey\", right_on=\"n_nationkey\")\n",
+                "        .merge(region_ds, left_on=\"n_regionkey\", right_on=\"r_regionkey\")\n",
+                "    )\n",
+                "\n",
+                "    jn = jn[jn[\"p_size\"] == var1]\n",
+                "    jn = jn[jn[\"p_type\"].str.endswith(var2)]\n",
+                "    jn = jn[jn[\"r_name\"] == var3]\n",
+                "\n",
+                "    gb = jn.groupby(\"p_partkey\", as_index=False)\n",
+                "    agg = gb[\"ps_supplycost\"].min()\n",
+                "    jn2 = agg.merge(jn, on=[\"p_partkey\", \"ps_supplycost\"])\n",
+                "\n",
+                "    sel = jn2.loc[\n",
                 "        :,\n",
                 "        [\n",
                 "            \"s_acctbal\",\n",
                 "            \"s_name\",\n",
                 "            \"n_name\",\n",
                 "            \"p_partkey\",\n",
                 "            \"p_mfgr\",\n",
                 "            \"s_address\",\n",
                 "            \"s_phone\",\n",
                 "            \"s_comment\",\n",
                 "        ],\n",
                 "    ]\n",
-                "    result_df = result_df.sort_values(\n",
-                "        by=[\n",
-                "            \"s_acctbal\",\n",
-                "            \"n_name\",\n",
-                "            \"s_name\",\n",
-                "            \"p_partkey\",\n",
-                "        ],\n",
-                "        ascending=[\n",
-                "            False,\n",
-                "            True,\n",
-                "            True,\n",
-                "            True,\n",
-                "        ],\n",
-                "    ).head(100)\n",
+                "\n",
+                "    sort = sel.sort_values(\n",
+                "        by=[\"s_acctbal\", \"n_name\", \"s_name\", \"p_partkey\"],\n",
+                "        ascending=[False, True, True, True],\n",
+                "    )\n",
+                "    result_df = sort.head(100)\n",
                 "\n",
                 "    return result_df  # type: ignore[no-any-return]"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 4,
@@ -407,15 +326,15 @@
                     "output_type": "display_data"
                 }
             ],
             "source": [
                 "tool = 'pandas[pyarrow]'\n",
                 "fn = IO_FUNCS[tool]\n",
                 "timings = %timeit -o q2_pandas_native(fn(region), fn(nation), fn(supplier), fn(part), fn(partsupp))\n",
-                "results[tool+'native'] = timings.best"
+                "results[tool+'[native]'] = timings.best"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "09249944",
             "metadata": {
                 "papermill": {
```

### Comparing `narwhals-0.7.9/tpch/notebooks/q3/execute.ipynb` & `narwhals-0.8.0/tpch/notebooks/q6/execute.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9786549707602339%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(3, 'pd.options.mode.copy_on_write = True')], delete: [4, "*

 * *            "3]}}, 3: {'source': {insert: [(4, 'def q6(line_item_raw) -> None:\\n'), (5, '    "*

 * *            "var_1 = datetime(1994, 1, 1)\\n'), (6, '    var_2 = datetime(1995, 1, 1)\\n'), (7, "*

 * *            "'    var_3 = 24\\n'), (9, '    line_item_ds = nw.from_native(line_item_raw)\\n'), "*

 * *            "(11, '    result = (\\n'), (12, '        line_item_ds.filter(\\n'), (13, '            "*

 * *            'nw.col("l […]*

```diff
@@ -71,16 +71,45 @@
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "import pandas as pd\n",
                 "import polars as pl\n",
                 "\n",
-                "pd.options.mode.copy_on_write = True\n",
-                "pd.options.future.infer_string = True"
+                "pd.options.mode.copy_on_write = True"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "3b4dcf55",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "from datetime import date\n",
+                "\n",
+                "def q6_pandas_native(line_item_ds):\n",
+                "    var1 = date(1994, 1, 1)\n",
+                "    var2 = date(1995, 1, 1)\n",
+                "    var3 = 0.05\n",
+                "    var4 = 0.07\n",
+                "    var5 = 24\n",
+                "\n",
+                "    flineitem = line_item_ds[\n",
+                "        (line_item_ds[\"l_shipdate\"] >= var1)\n",
+                "        & (line_item_ds[\"l_shipdate\"] < var2)\n",
+                "        & (line_item_ds[\"l_discount\"] >= var3)\n",
+                "        & (line_item_ds[\"l_discount\"] <= var4)\n",
+                "        & (line_item_ds[\"l_quantity\"] < var5)\n",
+                "    ]\n",
+                "\n",
+                "    result_value = (flineitem[\"l_extendedprice\"] * flineitem[\"l_discount\"]).sum()\n",
+                "    result_df = pd.DataFrame({\"revenue\": [result_value]})\n",
+                "\n",
+                "    return result_df"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 4,
             "id": "42e7f0e2",
             "metadata": {
@@ -101,51 +130,32 @@
             },
             "outputs": [],
             "source": [
                 "from typing import Any\n",
                 "from datetime import datetime\n",
                 "import narwhals as nw\n",
                 "\n",
-                "def q3(\n",
-                "    customer_ds_raw: Any,\n",
-                "    line_item_ds_raw: Any,\n",
-                "    orders_ds_raw: Any,\n",
-                ") -> Any:\n",
-                "    var_1 = var_2 = datetime(1995, 3, 15)\n",
-                "    var_3 = \"BUILDING\"\n",
+                "def q6(line_item_raw) -> None:\n",
+                "    var_1 = datetime(1994, 1, 1)\n",
+                "    var_2 = datetime(1995, 1, 1)\n",
+                "    var_3 = 24\n",
                 "\n",
-                "    customer_ds = nw.from_native(customer_ds_raw)\n",
-                "    line_item_ds = nw.from_native(line_item_ds_raw)\n",
-                "    orders_ds = nw.from_native(orders_ds_raw)\n",
+                "    line_item_ds = nw.from_native(line_item_raw)\n",
                 "\n",
-                "    q_final = (\n",
-                "        customer_ds.filter(nw.col(\"c_mktsegment\") == var_3)\n",
-                "        .join(orders_ds, left_on=\"c_custkey\", right_on=\"o_custkey\")\n",
-                "        .join(line_item_ds, left_on=\"o_orderkey\", right_on=\"l_orderkey\")\n",
-                "        .filter(\n",
-                "            nw.col(\"o_orderdate\") < var_2,\n",
-                "            nw.col(\"l_shipdate\") > var_1,\n",
+                "    result = (\n",
+                "        line_item_ds.filter(\n",
+                "            nw.col(\"l_shipdate\").is_between(var_1, var_2, closed=\"left\"),\n",
+                "            nw.col(\"l_discount\").is_between(0.05, 0.07),\n",
+                "            nw.col(\"l_quantity\") < var_3,\n",
                 "        ).with_columns(\n",
-                "            (nw.col(\"l_extendedprice\") * (1 - nw.col(\"l_discount\"))).alias(\"revenue\")\n",
+                "            (nw.col(\"l_extendedprice\") * nw.col(\"l_discount\")).alias(\"revenue\")\n",
                 "        )\n",
-                "        .group_by([\"o_orderkey\", \"o_orderdate\", \"o_shippriority\"])\n",
-                "        .agg([nw.sum(\"revenue\")])\n",
-                "        .select(\n",
-                "            [\n",
-                "                nw.col(\"o_orderkey\").alias(\"l_orderkey\"),\n",
-                "                \"revenue\",\n",
-                "                \"o_orderdate\",\n",
-                "                \"o_shippriority\",\n",
-                "            ]\n",
-                "        )\n",
-                "        .sort(by=[\"revenue\", \"o_orderdate\"], descending=[True, False])\n",
-                "        .head(10)\n",
+                "        .select(nw.sum(\"revenue\"))\n",
                 "    )\n",
-                "\n",
-                "    return nw.to_native(q_final)"
+                "    return nw.to_native(result)\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 5,
             "id": "8d540303",
             "metadata": {
@@ -215,14 +225,52 @@
             "outputs": [],
             "source": [
                 "results = {}"
             ]
         },
         {
             "cell_type": "markdown",
+            "id": "56b73231",
+            "metadata": {},
+            "source": [
+                "## pandas, pyarrow dtypes, native"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "bbea3aa9",
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "24 s \u00b1 142 ms per loop (mean \u00b1 std. dev. of 7 runs, 1 loop each)\n"
+                    ]
+                },
+                {
+                    "data": {
+                        "text/plain": [
+                            "23.841894793999984"
+                        ]
+                    },
+                    "metadata": {},
+                    "output_type": "display_data"
+                }
+            ],
+            "source": [
+                "tool = 'pandas[pyarrow]'\n",
+                "fn = IO_FUNCS[tool]\n",
+                "timings = %timeit -o q6_pandas_native(fn(lineitem))\n",
+                "results[tool+'[native]'] = timings.best"
+            ]
+        },
+        {
+            "cell_type": "markdown",
             "id": "09249944",
             "metadata": {
                 "papermill": {
                     "duration": 0.005113,
                     "end_time": "2024-03-22T17:24:39.130472",
                     "exception": false,
                     "start_time": "2024-03-22T17:24:39.125359",
@@ -272,15 +320,15 @@
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "tool = 'pandas'\n",
                 "fn = IO_FUNCS[tool]\n",
-                "timings = %timeit -o q3(fn(customer), fn(lineitem), fn(orders))\n",
+                "timings = %timeit -o q6(fn(lineitem))\n",
                 "results[tool] = timings.best"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "0b561017",
             "metadata": {
@@ -335,15 +383,15 @@
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "tool = 'pandas[pyarrow]'\n",
                 "fn = IO_FUNCS[tool]\n",
-                "timings = %timeit -o q3(fn(customer), fn(lineitem), fn(orders))\n",
+                "timings = %timeit -o q6(fn(lineitem))\n",
                 "results[tool] = timings.best"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "a8005d7d",
             "metadata": {
@@ -398,15 +446,15 @@
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "tool = 'polars[eager]'\n",
                 "fn = IO_FUNCS[tool]\n",
-                "timings = %timeit -o q3(fn(customer), fn(lineitem), fn(orders))\n",
+                "timings = %timeit -o q6(fn(lineitem))\n",
                 "results[tool] = timings.best"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "c77a701f",
             "metadata": {
@@ -461,15 +509,15 @@
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "tool = 'polars[lazy]'\n",
                 "fn = IO_FUNCS[tool]\n",
-                "timings = %timeit -o q3(fn(customer), fn(lineitem), fn(orders)).collect()\n",
+                "timings = %timeit -o q6(fn(lineitem)).collect()\n",
                 "results[tool] = timings.best"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "37ce6bf3",
             "metadata": {},
```

### Comparing `narwhals-0.7.9/tpch/notebooks/q4/execute.ipynb` & `narwhals-0.8.0/tpch/notebooks/q5/execute.ipynb`

 * *Files 13% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9789916128039396%*

 * *Differences: {"'cells'": "{3: {'source': {insert: [(4, 'def q5(\\n'), (5, '    region_ds_raw: Any,\\n'), (6, "*

 * *            "'    nation_ds_raw: Any,\\n'), (7, '    customer_ds_raw: Any,\\n'), (10, '    "*

 * *            'supplier_ds_raw: Any,\\n\'), (12, \'    var_1 = "ASIA"\\n\'), (13, \'    var_2 = '*

 * *            "datetime(1994, 1, 1)\\n'), (14, '    var_3 = datetime(1995, 1, 1)\\n'), (16, '    "*

 * *            "region_ds = nw.from_native(region_ds_raw)\\n'), (17, '    nation_ds = "*

 * *            "nw.from_native(nation_ds_raw)\ […]*

```diff
@@ -77,14 +77,56 @@
                 "\n",
                 "pd.options.mode.copy_on_write = True\n",
                 "pd.options.future.infer_string = True"
             ]
         },
         {
             "cell_type": "code",
+            "execution_count": null,
+            "id": "690c74b3",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "from typing import Any\n",
+                "from datetime import date\n",
+                "\n",
+                "def q5_pandas_native(\n",
+                "    region_ds: Any,\n",
+                "    nation_ds: Any,\n",
+                "    customer_ds: Any,\n",
+                "    line_item_ds: Any,\n",
+                "    orders_ds: Any,\n",
+                "    supplier_ds: Any,\n",
+                "):\n",
+                "    var1 = \"ASIA\"\n",
+                "    var2 = date(1994, 1, 1)\n",
+                "    var3 = date(1995, 1, 1)\n",
+                "\n",
+                "    jn1 = region_ds.merge(nation_ds, left_on=\"r_regionkey\", right_on=\"n_regionkey\")\n",
+                "    jn2 = jn1.merge(customer_ds, left_on=\"n_nationkey\", right_on=\"c_nationkey\")\n",
+                "    jn3 = jn2.merge(orders_ds, left_on=\"c_custkey\", right_on=\"o_custkey\")\n",
+                "    jn4 = jn3.merge(line_item_ds, left_on=\"o_orderkey\", right_on=\"l_orderkey\")\n",
+                "    jn5 = jn4.merge(\n",
+                "        supplier_ds,\n",
+                "        left_on=[\"l_suppkey\", \"n_nationkey\"],\n",
+                "        right_on=[\"s_suppkey\", \"s_nationkey\"],\n",
+                "    )\n",
+                "\n",
+                "    jn5 = jn5[jn5[\"r_name\"] == var1]\n",
+                "    jn5 = jn5[(jn5[\"o_orderdate\"] >= var2) & (jn5[\"o_orderdate\"] < var3)]\n",
+                "    jn5[\"revenue\"] = jn5.l_extendedprice * (1.0 - jn5.l_discount)\n",
+                "\n",
+                "    gb = jn5.groupby(\"n_name\", as_index=False)[\"revenue\"].sum()\n",
+                "    result_df = gb.sort_values(\"revenue\", ascending=False)\n",
+                "\n",
+                "    return result_df  # type: ignore[no-any-return]"
+            ]
+        },
+        {
+            "cell_type": "code",
             "execution_count": 4,
             "id": "42e7f0e2",
             "metadata": {
                 "execution": {
                     "iopub.execute_input": "2024-03-22T17:24:39.066341Z",
                     "iopub.status.busy": "2024-03-22T17:24:39.065881Z",
                     "iopub.status.idle": "2024-03-22T17:24:39.078875Z",
@@ -101,34 +143,53 @@
             },
             "outputs": [],
             "source": [
                 "from typing import Any\n",
                 "from datetime import datetime\n",
                 "import narwhals as nw\n",
                 "\n",
-                "def q4(\n",
+                "def q5(\n",
+                "    region_ds_raw: Any,\n",
+                "    nation_ds_raw: Any,\n",
+                "    customer_ds_raw: Any,\n",
                 "    lineitem_ds_raw: Any,\n",
                 "    orders_ds_raw: Any,\n",
+                "    supplier_ds_raw: Any,\n",
                 ") -> Any:\n",
-                "    var_1 = datetime(1993, 7, 1)\n",
-                "    var_2 = datetime(1993, 10, 1)\n",
+                "    var_1 = \"ASIA\"\n",
+                "    var_2 = datetime(1994, 1, 1)\n",
+                "    var_3 = datetime(1995, 1, 1)\n",
                 "\n",
+                "    region_ds = nw.from_native(region_ds_raw)\n",
+                "    nation_ds = nw.from_native(nation_ds_raw)\n",
+                "    customer_ds = nw.from_native(customer_ds_raw)\n",
                 "    line_item_ds = nw.from_native(lineitem_ds_raw)\n",
                 "    orders_ds = nw.from_native(orders_ds_raw)\n",
+                "    supplier_ds = nw.from_native(supplier_ds_raw)\n",
                 "\n",
                 "    result = (\n",
-                "        line_item_ds.join(orders_ds, left_on=\"l_orderkey\", right_on=\"o_orderkey\")\n",
+                "        region_ds.join(nation_ds, left_on=\"r_regionkey\", right_on=\"n_regionkey\")\n",
+                "        .join(customer_ds, left_on=\"n_nationkey\", right_on=\"c_nationkey\")\n",
+                "        .join(orders_ds, left_on=\"c_custkey\", right_on=\"o_custkey\")\n",
+                "        .join(line_item_ds, left_on=\"o_orderkey\", right_on=\"l_orderkey\")\n",
+                "        .join(\n",
+                "            supplier_ds,\n",
+                "            left_on=[\"l_suppkey\", \"n_nationkey\"],\n",
+                "            right_on=[\"s_suppkey\", \"s_nationkey\"],\n",
+                "        )\n",
                 "        .filter(\n",
-                "            nw.col(\"o_orderdate\").is_between(var_1, var_2, closed=\"left\"),\n",
-                "            nw.col(\"l_commitdate\") < nw.col(\"l_receiptdate\"),\n",
-                "        ).unique(subset=[\"o_orderpriority\", \"l_orderkey\"])\n",
-                "        .group_by(\"o_orderpriority\")\n",
-                "        .agg(nw.len().alias(\"order_count\"))\n",
-                "        .sort(by=\"o_orderpriority\")\n",
-                "        .with_columns(nw.col(\"order_count\").cast(nw.Int64))\n",
+                "            nw.col(\"r_name\") == var_1,\n",
+                "            nw.col(\"o_orderdate\").is_between(var_2, var_3, closed=\"left\")\n",
+                "        )\n",
+                "        .with_columns(\n",
+                "            (nw.col(\"l_extendedprice\") * (1 - nw.col(\"l_discount\"))).alias(\"revenue\")\n",
+                "        )\n",
+                "        .group_by(\"n_name\")\n",
+                "        .agg([nw.sum(\"revenue\")])\n",
+                "        .sort(by=\"revenue\", descending=True)\n",
                 "    )\n",
                 "\n",
                 "    return nw.to_native(result)"
             ]
         },
         {
             "cell_type": "code",
@@ -201,14 +262,52 @@
             "outputs": [],
             "source": [
                 "results = {}"
             ]
         },
         {
             "cell_type": "markdown",
+            "id": "3d76284a",
+            "metadata": {},
+            "source": [
+                "## pandas, pyarrow dtypes, native"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "0fd7e705",
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "24 s \u00b1 142 ms per loop (mean \u00b1 std. dev. of 7 runs, 1 loop each)\n"
+                    ]
+                },
+                {
+                    "data": {
+                        "text/plain": [
+                            "23.841894793999984"
+                        ]
+                    },
+                    "metadata": {},
+                    "output_type": "display_data"
+                }
+            ],
+            "source": [
+                "tool = 'pandas[pyarrow]'\n",
+                "fn = IO_FUNCS[tool]\n",
+                "timings = %timeit -o q5_pandas_native(fn(region), fn(nation), fn(customer), fn(lineitem), fn(orders), fn(supplier))\n",
+                "results[tool+'[native]'] = timings.best"
+            ]
+        },
+        {
+            "cell_type": "markdown",
             "id": "09249944",
             "metadata": {
                 "papermill": {
                     "duration": 0.005113,
                     "end_time": "2024-03-22T17:24:39.130472",
                     "exception": false,
                     "start_time": "2024-03-22T17:24:39.125359",
@@ -258,15 +357,15 @@
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "tool = 'pandas'\n",
                 "fn = IO_FUNCS[tool]\n",
-                "timings = %timeit -o q4(fn(lineitem), fn(orders))\n",
+                "timings = %timeit -o q5(fn(region), fn(nation), fn(customer), fn(lineitem), fn(orders), fn(supplier))\n",
                 "results[tool] = timings.best"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "0b561017",
             "metadata": {
@@ -321,15 +420,15 @@
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "tool = 'pandas[pyarrow]'\n",
                 "fn = IO_FUNCS[tool]\n",
-                "timings = %timeit -o q4(fn(lineitem), fn(orders))\n",
+                "timings = %timeit -o q5(fn(region), fn(nation), fn(customer), fn(lineitem), fn(orders), fn(supplier))\n",
                 "results[tool] = timings.best"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "a8005d7d",
             "metadata": {
@@ -384,15 +483,15 @@
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "tool = 'polars[eager]'\n",
                 "fn = IO_FUNCS[tool]\n",
-                "timings = %timeit -o q4(fn(lineitem), fn(orders))\n",
+                "timings = %timeit -o q5(fn(region), fn(nation), fn(customer), fn(lineitem), fn(orders), fn(supplier))\n",
                 "results[tool] = timings.best"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "c77a701f",
             "metadata": {
@@ -447,15 +546,15 @@
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "tool = 'polars[lazy]'\n",
                 "fn = IO_FUNCS[tool]\n",
-                "timings = %timeit -o q4(fn(lineitem), fn(orders)).collect()\n",
+                "timings = %timeit -o q5(fn(region), fn(nation), fn(customer), fn(lineitem), fn(orders), fn(supplier)).collect()\n",
                 "results[tool] = timings.best"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "37ce6bf3",
             "metadata": {},
```

### Comparing `narwhals-0.7.9/tpch/notebooks/q5/execute.ipynb` & `narwhals-0.8.0/tpch/notebooks/q4/execute.ipynb`

 * *Files 17% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9789916128039396%*

 * *Differences: {"'cells'": "{3: {'source': {insert: [(4, 'def q4(\\n'), (8, '    var_1 = datetime(1993, 7, "*

 * *            "1)\\n'), (9, '    var_2 = datetime(1993, 10, 1)\\n'), (15, '        "*

 * *            'line_item_ds.join(orders_ds, left_on="l_orderkey", right_on="o_orderkey")\\n\'), (17, '*

 * *            '\'            nw.col("o_orderdate").is_between(var_1, var_2, closed="left"),\\n\'), '*

 * *            '(18, \'            nw.col("l_commitdate") < nw.col("l_receiptdate"),\\n\'), (19, '*

 * *            '\'        ).unique(subset= […]*

```diff
@@ -77,14 +77,49 @@
                 "\n",
                 "pd.options.mode.copy_on_write = True\n",
                 "pd.options.future.infer_string = True"
             ]
         },
         {
             "cell_type": "code",
+            "execution_count": null,
+            "id": "580ac2a5",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "from datetime import date\n",
+                "from typing import Any\n",
+                "\n",
+                "def q4_pandas_native(\n",
+                "    line_item_ds: Any,\n",
+                "    orders_ds: Any,\n",
+                "):\n",
+                "    var1 = date(1993, 7, 1)\n",
+                "    var2 = date(1993, 10, 1)\n",
+                "\n",
+                "    jn = line_item_ds.merge(orders_ds, left_on=\"l_orderkey\", right_on=\"o_orderkey\")\n",
+                "\n",
+                "    jn = jn[\n",
+                "        (jn[\"o_orderdate\"] < var2)\n",
+                "        & (jn[\"o_orderdate\"] >= var1)\n",
+                "        & (jn[\"l_commitdate\"] < jn[\"l_receiptdate\"])\n",
+                "    ]\n",
+                "\n",
+                "    jn = jn.drop_duplicates(subset=[\"o_orderpriority\", \"l_orderkey\"])\n",
+                "\n",
+                "    gb = jn.groupby(\"o_orderpriority\", as_index=False)\n",
+                "    agg = gb.agg(order_count=pd.NamedAgg(column=\"o_orderkey\", aggfunc=\"count\"))\n",
+                "\n",
+                "    result_df = agg.sort_values([\"o_orderpriority\"])\n",
+                "\n",
+                "    return result_df  # type: ignore[no-any-return]"
+            ]
+        },
+        {
+            "cell_type": "code",
             "execution_count": 4,
             "id": "42e7f0e2",
             "metadata": {
                 "execution": {
                     "iopub.execute_input": "2024-03-22T17:24:39.066341Z",
                     "iopub.status.busy": "2024-03-22T17:24:39.065881Z",
                     "iopub.status.idle": "2024-03-22T17:24:39.078875Z",
@@ -101,53 +136,34 @@
             },
             "outputs": [],
             "source": [
                 "from typing import Any\n",
                 "from datetime import datetime\n",
                 "import narwhals as nw\n",
                 "\n",
-                "def q5(\n",
-                "    region_ds_raw: Any,\n",
-                "    nation_ds_raw: Any,\n",
-                "    customer_ds_raw: Any,\n",
+                "def q4(\n",
                 "    lineitem_ds_raw: Any,\n",
                 "    orders_ds_raw: Any,\n",
-                "    supplier_ds_raw: Any,\n",
                 ") -> Any:\n",
-                "    var_1 = \"ASIA\"\n",
-                "    var_2 = datetime(1994, 1, 1)\n",
-                "    var_3 = datetime(1995, 1, 1)\n",
-                "\n",
-                "    region_ds = nw.from_native(region_ds_raw)\n",
-                "    nation_ds = nw.from_native(nation_ds_raw)\n",
-                "    customer_ds = nw.from_native(customer_ds_raw)\n",
+                "    var_1 = datetime(1993, 7, 1)\n",
+                "    var_2 = datetime(1993, 10, 1)\n",
+                "\n",
                 "    line_item_ds = nw.from_native(lineitem_ds_raw)\n",
                 "    orders_ds = nw.from_native(orders_ds_raw)\n",
-                "    supplier_ds = nw.from_native(supplier_ds_raw)\n",
                 "\n",
                 "    result = (\n",
-                "        region_ds.join(nation_ds, left_on=\"r_regionkey\", right_on=\"n_regionkey\")\n",
-                "        .join(customer_ds, left_on=\"n_nationkey\", right_on=\"c_nationkey\")\n",
-                "        .join(orders_ds, left_on=\"c_custkey\", right_on=\"o_custkey\")\n",
-                "        .join(line_item_ds, left_on=\"o_orderkey\", right_on=\"l_orderkey\")\n",
-                "        .join(\n",
-                "            supplier_ds,\n",
-                "            left_on=[\"l_suppkey\", \"n_nationkey\"],\n",
-                "            right_on=[\"s_suppkey\", \"s_nationkey\"],\n",
-                "        )\n",
+                "        line_item_ds.join(orders_ds, left_on=\"l_orderkey\", right_on=\"o_orderkey\")\n",
                 "        .filter(\n",
-                "            nw.col(\"r_name\") == var_1,\n",
-                "            nw.col(\"o_orderdate\").is_between(var_2, var_3, closed=\"left\")\n",
-                "        )\n",
-                "        .with_columns(\n",
-                "            (nw.col(\"l_extendedprice\") * (1 - nw.col(\"l_discount\"))).alias(\"revenue\")\n",
-                "        )\n",
-                "        .group_by(\"n_name\")\n",
-                "        .agg([nw.sum(\"revenue\")])\n",
-                "        .sort(by=\"revenue\", descending=True)\n",
+                "            nw.col(\"o_orderdate\").is_between(var_1, var_2, closed=\"left\"),\n",
+                "            nw.col(\"l_commitdate\") < nw.col(\"l_receiptdate\"),\n",
+                "        ).unique(subset=[\"o_orderpriority\", \"l_orderkey\"])\n",
+                "        .group_by(\"o_orderpriority\")\n",
+                "        .agg(nw.len().alias(\"order_count\"))\n",
+                "        .sort(by=\"o_orderpriority\")\n",
+                "        .with_columns(nw.col(\"order_count\").cast(nw.Int64))\n",
                 "    )\n",
                 "\n",
                 "    return nw.to_native(result)"
             ]
         },
         {
             "cell_type": "code",
@@ -220,14 +236,52 @@
             "outputs": [],
             "source": [
                 "results = {}"
             ]
         },
         {
             "cell_type": "markdown",
+            "id": "956e9675",
+            "metadata": {},
+            "source": [
+                "## pandas, pyarrow dtype, via Narwhals"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "ca578422",
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "24 s \u00b1 142 ms per loop (mean \u00b1 std. dev. of 7 runs, 1 loop each)\n"
+                    ]
+                },
+                {
+                    "data": {
+                        "text/plain": [
+                            "23.841894793999984"
+                        ]
+                    },
+                    "metadata": {},
+                    "output_type": "display_data"
+                }
+            ],
+            "source": [
+                "tool = 'pandas[pyarrow]'\n",
+                "fn = IO_FUNCS[tool]\n",
+                "timings = %timeit -o q4_pandas_native(fn(lineitem), fn(orders))\n",
+                "results[tool+'[native]'] = timings.best"
+            ]
+        },
+        {
+            "cell_type": "markdown",
             "id": "09249944",
             "metadata": {
                 "papermill": {
                     "duration": 0.005113,
                     "end_time": "2024-03-22T17:24:39.130472",
                     "exception": false,
                     "start_time": "2024-03-22T17:24:39.125359",
@@ -277,15 +331,15 @@
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "tool = 'pandas'\n",
                 "fn = IO_FUNCS[tool]\n",
-                "timings = %timeit -o q5(fn(region), fn(nation), fn(customer), fn(lineitem), fn(orders), fn(supplier))\n",
+                "timings = %timeit -o q4(fn(lineitem), fn(orders))\n",
                 "results[tool] = timings.best"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "0b561017",
             "metadata": {
@@ -340,15 +394,15 @@
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "tool = 'pandas[pyarrow]'\n",
                 "fn = IO_FUNCS[tool]\n",
-                "timings = %timeit -o q5(fn(region), fn(nation), fn(customer), fn(lineitem), fn(orders), fn(supplier))\n",
+                "timings = %timeit -o q4(fn(lineitem), fn(orders))\n",
                 "results[tool] = timings.best"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "a8005d7d",
             "metadata": {
@@ -403,15 +457,15 @@
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "tool = 'polars[eager]'\n",
                 "fn = IO_FUNCS[tool]\n",
-                "timings = %timeit -o q5(fn(region), fn(nation), fn(customer), fn(lineitem), fn(orders), fn(supplier))\n",
+                "timings = %timeit -o q4(fn(lineitem), fn(orders))\n",
                 "results[tool] = timings.best"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "c77a701f",
             "metadata": {
@@ -466,15 +520,15 @@
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "tool = 'polars[lazy]'\n",
                 "fn = IO_FUNCS[tool]\n",
-                "timings = %timeit -o q5(fn(region), fn(nation), fn(customer), fn(lineitem), fn(orders), fn(supplier)).collect()\n",
+                "timings = %timeit -o q4(fn(lineitem), fn(orders)).collect()\n",
                 "results[tool] = timings.best"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "37ce6bf3",
             "metadata": {},
```

### Comparing `narwhals-0.7.9/tpch/notebooks/q7/execute.ipynb` & `narwhals-0.8.0/tpch/notebooks/q8/execute.ipynb`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9802796052631579%*

 * *Differences: {"'cells'": "{1: {'source': ['!pip install -U narwhals']}, 4: {'source': {insert: [(4, 'def "*

 * *            "q8(\\n'), (5, '    nation_ds_raw: Any,\\n'), (6, '    customer_ds_raw: Any,\\n'), (7, "*

 * *            "'    line_item_ds_raw: Any,\\n'), (8, '    orders_ds_raw: Any,\\n'), (9, '    "*

 * *            "supplier_ds_raw: Any,\\n'), (10, '    part_ds_raw: Any,\\n'), (12, '    nation_ds = "*

 * *            "nw.from_native(nation_ds_raw)\\n'), (13, '    customer_ds = "*

 * *            "nw.from_native(customer_ds_raw)\\n'), […]*

```diff
@@ -53,15 +53,15 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "92c1bf9f",
             "metadata": {},
             "outputs": [],
             "source": [
-                "!pip install git+https://github.com/MarcoGorelli/narwhals@3fb34c59fbe41374fb05ea9ee31c65ac271efe8e"
+                "!pip install -U narwhals"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 1,
             "id": "b969208d",
             "metadata": {
@@ -87,14 +87,73 @@
                 "\n",
                 "pd.options.mode.copy_on_write = True\n",
                 "pd.options.future.infer_string = True"
             ]
         },
         {
             "cell_type": "code",
+            "execution_count": null,
+            "id": "3c83ec1b",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "from typing import Any\n",
+                "from datetime import datetime, date\n",
+                "import narwhals as nw\n",
+                "\n",
+                "def q8_pandas_native(\n",
+                "    nation_ds,\n",
+                "    customer_ds,\n",
+                "    line_item_ds,\n",
+                "    orders_ds,\n",
+                "    supplier_ds,\n",
+                ") -> None:\n",
+                "    var1 = \"FRANCE\"\n",
+                "    var2 = \"GERMANY\"\n",
+                "    var3 = date(1995, 1, 1)\n",
+                "    var4 = date(1996, 12, 31)\n",
+                "\n",
+                "    n1 = nation_ds[(nation_ds[\"n_name\"] == var1)]\n",
+                "    n2 = nation_ds[(nation_ds[\"n_name\"] == var2)]\n",
+                "\n",
+                "    # Part 1\n",
+                "    jn1 = customer_ds.merge(n1, left_on=\"c_nationkey\", right_on=\"n_nationkey\")\n",
+                "    jn2 = jn1.merge(orders_ds, left_on=\"c_custkey\", right_on=\"o_custkey\")\n",
+                "    jn2 = jn2.rename({\"n_name\": \"cust_nation\"}, axis=\"columns\")\n",
+                "    jn3 = jn2.merge(line_item_ds, left_on=\"o_orderkey\", right_on=\"l_orderkey\")\n",
+                "    jn4 = jn3.merge(supplier_ds, left_on=\"l_suppkey\", right_on=\"s_suppkey\")\n",
+                "    jn5 = jn4.merge(n2, left_on=\"s_nationkey\", right_on=\"n_nationkey\")\n",
+                "    df1 = jn5.rename({\"n_name\": \"supp_nation\"}, axis=\"columns\")\n",
+                "\n",
+                "    # Part 2\n",
+                "    jn1 = customer_ds.merge(n2, left_on=\"c_nationkey\", right_on=\"n_nationkey\")\n",
+                "    jn2 = jn1.merge(orders_ds, left_on=\"c_custkey\", right_on=\"o_custkey\")\n",
+                "    jn2 = jn2.rename({\"n_name\": \"cust_nation\"}, axis=\"columns\")\n",
+                "    jn3 = jn2.merge(line_item_ds, left_on=\"o_orderkey\", right_on=\"l_orderkey\")\n",
+                "    jn4 = jn3.merge(supplier_ds, left_on=\"l_suppkey\", right_on=\"s_suppkey\")\n",
+                "    jn5 = jn4.merge(n1, left_on=\"s_nationkey\", right_on=\"n_nationkey\")\n",
+                "    df2 = jn5.rename({\"n_name\": \"supp_nation\"}, axis=\"columns\")\n",
+                "\n",
+                "    # Combine\n",
+                "    total = pd.concat([df1, df2])\n",
+                "\n",
+                "    total = total[(total[\"l_shipdate\"] >= var3) & (total[\"l_shipdate\"] <= var4)]\n",
+                "    total[\"volume\"] = total[\"l_extendedprice\"] * (1.0 - total[\"l_discount\"])\n",
+                "    total[\"l_year\"] = total[\"l_shipdate\"].dt.year\n",
+                "\n",
+                "    gb = total.groupby([\"supp_nation\", \"cust_nation\", \"l_year\"], as_index=False)\n",
+                "    agg = gb.agg(revenue=pd.NamedAgg(column=\"volume\", aggfunc=\"sum\"))\n",
+                "\n",
+                "    result_df = agg.sort_values(by=[\"supp_nation\", \"cust_nation\", \"l_year\"])\n",
+                "\n",
+                "    return result_df  # type: ignore[no-any-return]"
+            ]
+        },
+        {
+            "cell_type": "code",
             "execution_count": 2,
             "id": "42e7f0e2",
             "metadata": {
                 "execution": {
                     "iopub.execute_input": "2024-03-22T17:24:39.066341Z",
                     "iopub.status.busy": "2024-03-22T17:24:39.065881Z",
                     "iopub.status.idle": "2024-03-22T17:24:39.078875Z",
@@ -111,64 +170,62 @@
             },
             "outputs": [],
             "source": [
                 "from typing import Any\n",
                 "from datetime import datetime\n",
                 "import narwhals as nw\n",
                 "\n",
-                "def q7(\n",
-                "    nation_ds,\n",
-                "    customer_ds,\n",
-                "    line_item_ds,\n",
-                "    orders_ds,\n",
-                "    supplier_ds,\n",
+                "def q8(\n",
+                "    nation_ds_raw: Any,\n",
+                "    customer_ds_raw: Any,\n",
+                "    line_item_ds_raw: Any,\n",
+                "    orders_ds_raw: Any,\n",
+                "    supplier_ds_raw: Any,\n",
+                "    part_ds_raw: Any,\n",
                 ") -> None:\n",
-                "    nation_ds = nw.from_native(nation_ds)\n",
-                "    customer_ds = nw.from_native(customer_ds)\n",
-                "    line_item_ds = nw.from_native(line_item_ds)\n",
-                "    orders_ds = nw.from_native(orders_ds)\n",
-                "    supplier_ds = nw.from_native(supplier_ds)\n",
-                "\n",
-                "    n1 = nation_ds.filter(nw.col(\"n_name\") == \"FRANCE\")\n",
-                "    n2 = nation_ds.filter(nw.col(\"n_name\") == \"GERMANY\")\n",
-                "\n",
-                "    var_1 = datetime(1995, 1, 1)\n",
-                "    var_2 = datetime(1996, 12, 31)\n",
-                "\n",
-                "    df1 = (\n",
-                "        customer_ds.join(n1, left_on=\"c_nationkey\", right_on=\"n_nationkey\")\n",
-                "        .join(orders_ds, left_on=\"c_custkey\", right_on=\"o_custkey\")\n",
-                "        .rename({\"n_name\": \"cust_nation\"})\n",
-                "        .join(line_item_ds, left_on=\"o_orderkey\", right_on=\"l_orderkey\")\n",
-                "        .join(supplier_ds, left_on=\"l_suppkey\", right_on=\"s_suppkey\")\n",
-                "        .join(n2, left_on=\"s_nationkey\", right_on=\"n_nationkey\")\n",
-                "        .rename({\"n_name\": \"supp_nation\"})\n",
-                "    )\n",
+                "    nation_ds = nw.from_native(nation_ds_raw)\n",
+                "    customer_ds = nw.from_native(customer_ds_raw)\n",
+                "    line_item_ds = nw.from_native(line_item_ds_raw)\n",
+                "    orders_ds = nw.from_native(orders_ds_raw)\n",
+                "    supplier_ds = nw.from_native(supplier_ds_raw)\n",
+                "    part_ds = nw.from_native(part_ds_raw)\n",
                 "\n",
-                "    df2 = (\n",
-                "        customer_ds.join(n2, left_on=\"c_nationkey\", right_on=\"n_nationkey\")\n",
-                "        .join(orders_ds, left_on=\"c_custkey\", right_on=\"o_custkey\")\n",
-                "        .rename({\"n_name\": \"cust_nation\"})\n",
-                "        .join(line_item_ds, left_on=\"o_orderkey\", right_on=\"l_orderkey\")\n",
-                "        .join(supplier_ds, left_on=\"l_suppkey\", right_on=\"s_suppkey\")\n",
-                "        .join(n1, left_on=\"s_nationkey\", right_on=\"n_nationkey\")\n",
-                "        .rename({\"n_name\": \"supp_nation\"})\n",
-                "    )\n",
+                "    n1 = nation_ds.select(\"n_nationkey\", \"n_regionkey\")\n",
+                "    n2 = nation_ds.select(\"n_nationkey\", \"n_name\")\n",
                 "\n",
                 "    result = (\n",
-                "        nw.concat([df1, df2])\n",
-                "        .filter(nw.col(\"l_shipdate\").is_between(var_1, var_2))\n",
+                "        part_ds.join(line_item_ds, left_on=\"p_partkey\", right_on=\"l_partkey\")\n",
+                "        .join(supplier_ds, left_on=\"l_suppkey\", right_on=\"s_suppkey\")\n",
+                "        .join(orders_ds, left_on=\"l_orderkey\", right_on=\"o_orderkey\")\n",
+                "        .join(customer_ds, left_on=\"o_custkey\", right_on=\"c_custkey\")\n",
+                "        .join(n1, left_on=\"c_nationkey\", right_on=\"n_nationkey\")\n",
+                "        .join(region_ds, left_on=\"n_regionkey\", right_on=\"r_regionkey\")\n",
+                "        .filter(nw.col(\"r_name\") == \"AMERICA\")\n",
+                "        .join(n2, left_on=\"s_nationkey\", right_on=\"n_nationkey\")\n",
+                "        .filter(\n",
+                "            nw.col(\"o_orderdate\")>= date(1995, 1, 1),\n",
+                "            nw.col('o_orderdate')<=date(1996, 12, 31)\n",
+                "        )\n",
+                "        .filter(nw.col(\"p_type\") == \"ECONOMY ANODIZED STEEL\")\n",
+                "        .select(\n",
+                "            nw.col(\"o_orderdate\").dt.year().alias(\"o_year\"),\n",
+                "            (nw.col(\"l_extendedprice\") * (1 - nw.col(\"l_discount\"))).alias(\"volume\"),\n",
+                "            nw.col(\"n_name\").alias(\"nation\"),\n",
+                "        )\n",
                 "        .with_columns(\n",
-                "            (nw.col(\"l_extendedprice\") * (1 - nw.col(\"l_discount\"))).alias(\"volume\")\n",
+                "            nw.when(nw.col(\"nation\") == \"BRAZIL\")\n",
+                "            .then(nw.col(\"volume\"))\n",
+                "            .otherwise(0)\n",
+                "            .alias(\"_tmp\")\n",
                 "        )\n",
-                "        .with_columns(nw.col(\"l_shipdate\").dt.year().alias(\"l_year\"))\n",
-                "        .group_by(\"supp_nation\", \"cust_nation\", \"l_year\")\n",
-                "        .agg(nw.sum(\"volume\").alias(\"revenue\"))\n",
-                "        .sort(by=[\"supp_nation\", \"cust_nation\", \"l_year\"])\n",
+                "        .group_by(\"o_year\")\n",
+                "        .agg((nw.sum(\"_tmp\") / nw.sum(\"volume\")).round(2).alias(\"mkt_share\"))\n",
+                "        .sort(\"o_year\")\n",
                 "    )\n",
+                "    \n",
                 "    return nw.to_native(result)\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 3,
             "id": "8d540303",
@@ -239,14 +296,52 @@
             "outputs": [],
             "source": [
                 "results = {}"
             ]
         },
         {
             "cell_type": "markdown",
+            "id": "12824d5d",
+            "metadata": {},
+            "source": [
+                "## pandas, pyarrow dtypes, native"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "ce229598",
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "20.2 s \u00b1 5.8 s per loop (mean \u00b1 std. dev. of 7 runs, 1 loop each)\n"
+                    ]
+                },
+                {
+                    "data": {
+                        "text/plain": [
+                            "16.42582530300001"
+                        ]
+                    },
+                    "metadata": {},
+                    "output_type": "display_data"
+                }
+            ],
+            "source": [
+                "tool = 'pandas[pyarrow]'\n",
+                "fn = IO_FUNCS[tool]\n",
+                "timings = %timeit -o q7_pandas_native(fn(nation), fn(customer), fn(lineitem), fn(orders), fn(supplier))\n",
+                "results[tool+'[native]'] = timings.best"
+            ]
+        },
+        {
+            "cell_type": "markdown",
             "id": "09249944",
             "metadata": {
                 "papermill": {
                     "duration": 0.005113,
                     "end_time": "2024-03-22T17:24:39.130472",
                     "exception": false,
                     "start_time": "2024-03-22T17:24:39.125359",
```

### Comparing `narwhals-0.7.9/utils/bump_version.py` & `narwhals-0.8.0/utils/bump_version.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.9/utils/check_api_reference.py` & `narwhals-0.8.0/utils/check_api_reference.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,15 @@
 with open("docs/api-reference/series.md") as fd:
     content = fd.read()
 documented = [
     remove_prefix(i, "        - ")
     for i in content.splitlines()
     if i.startswith("        - ")
 ]
-if missing := set(top_level_functions).difference(documented):
+if missing := set(top_level_functions).difference(documented).difference({"dt", "str"}):
     print("Series: not documented")  # noqa: T201
     print(missing)  # noqa: T201
     ret = 1
 if extra := set(documented).difference(top_level_functions):
     print("Series: outdated")  # noqa: T201
     print(extra)  # noqa: T201
     ret = 1
@@ -102,15 +102,15 @@
 with open("docs/api-reference/expressions.md") as fd:
     content = fd.read()
 documented = [
     remove_prefix(i, "        - ")
     for i in content.splitlines()
     if i.startswith("        - ")
 ]
-if missing := set(top_level_functions).difference(documented):
+if missing := set(top_level_functions).difference(documented).difference({"str", "dt"}):
     print("Expr: not documented")  # noqa: T201
     print(missing)  # noqa: T201
     ret = 1
 if extra := set(documented).difference(top_level_functions):
     print("Expr: outdated")  # noqa: T201
     print(extra)  # noqa: T201
     ret = 1
@@ -129,14 +129,14 @@
 if missing := set(expr).difference(series):
     print("In expr but not in series")  # noqa: T201
     print(missing)  # noqa: T201
     ret = 1
 if (
     extra := set(series)
     .difference(expr)
-    .difference({"to_pandas", "to_numpy", "dtype", "name"})
+    .difference({"to_pandas", "to_numpy", "dtype", "name", "shape"})
 ):
     print("in series but not in expr")  # noqa: T201
     print(extra)  # noqa: T201
     ret = 1
 
 sys.exit(ret)
```

### Comparing `narwhals-0.7.9/LICENSE.md` & `narwhals-0.8.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.9/pyproject.toml` & `narwhals-0.8.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "narwhals"
-version = "0.7.9"
+version = "0.8.0"
 authors = [
   { name="Marco Gorelli", email="33491632+MarcoGorelli@users.noreply.github.com" },
 ]
 description = "Extremely lightweight compatibility layer between pandas, Polars, cuDF, and Modin"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
+[project.optional-dependencies]
+pandas = ["pandas>=1.1.5"]
+polars = ["polars>=0.20.3"]
+
 [project.urls]
 "Homepage" = "https://github.com/MarcoGorelli/narwhals"
 "Bug Tracker" = "https://github.com/MarcoGorelli/narwhals"
 
 [tool.ruff]
 line-length = 90
 fix = true
@@ -79,14 +83,16 @@
 [tool.coverage.run]
 plugins = ["covdefaults"]
 
 [tool.coverage.report]
 exclude_also = [
   "> POLARS_VERSION",
   "if sys.version_info() <",
+  "if implementation == \"modin\"",
+  "if implementation == \"cudf\"",
 ]
 
 [tool.mypy]
 strict = true
 
 [[tool.mypy.overrides]]
 # the pandas API is just too inconsistent for type hinting to be useful.
```

