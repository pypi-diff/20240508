# Comparing `tmp/narwhals-0.8.1.tar.gz` & `tmp/narwhals-0.8.2.tar.gz`

## Comparing `narwhals-0.8.1.tar` & `narwhals-0.8.2.tar`

### file list

```diff
@@ -1,116 +1,120 @@
--rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 narwhals-0.8.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 narwhals-0.8.1/CONTRIBUTING.md
--rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 narwhals-0.8.1/mkdocs.yml
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 narwhals-0.8.1/requirements-dev.txt
--rw-r--r--   0        0        0     5243 2020-02-02 00:00:00.000000 narwhals-0.8.1/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     3725 2020-02-02 00:00:00.000000 narwhals-0.8.1/.github/workflows/extremes.yml
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 narwhals-0.8.1/.github/workflows/mkdocs.yml
--rw-r--r--   0        0        0     2638 2020-02-02 00:00:00.000000 narwhals-0.8.1/.github/workflows/publish_to_pypi.yml
--rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 narwhals-0.8.1/.github/workflows/pytest.yml
--rw-r--r--   0        0        0     2021 2020-02-02 00:00:00.000000 narwhals-0.8.1/docs/extending.md
--rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 narwhals-0.8.1/docs/generate_members.py
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 narwhals-0.8.1/docs/index.md
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 narwhals-0.8.1/docs/installation.md
--rw-r--r--   0        0        0     1245 2020-02-02 00:00:00.000000 narwhals-0.8.1/docs/quick_start.md
--rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 narwhals-0.8.1/docs/related.md
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 narwhals-0.8.1/docs/requirements-docs.txt
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 narwhals-0.8.1/docs/roadmap.md
--rw-r--r--   0        0        0     1281 2020-02-02 00:00:00.000000 narwhals-0.8.1/docs/why.md
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 narwhals-0.8.1/docs/api-reference/dataframe.md
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 narwhals-0.8.1/docs/api-reference/dependencies.md
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 narwhals-0.8.1/docs/api-reference/dtypes.md
--rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 narwhals-0.8.1/docs/api-reference/expressions.md
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 narwhals-0.8.1/docs/api-reference/expressions_dt.md
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 narwhals-0.8.1/docs/api-reference/expressions_str.md
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 narwhals-0.8.1/docs/api-reference/index.md
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 narwhals-0.8.1/docs/api-reference/lazyframe.md
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 narwhals-0.8.1/docs/api-reference/narwhals.md
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 narwhals-0.8.1/docs/api-reference/series.md
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 narwhals-0.8.1/docs/api-reference/series_dt.md
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 narwhals-0.8.1/docs/api-reference/series_str.md
--rwxr-xr-x   0        0        0   132699 2020-02-02 00:00:00.000000 narwhals-0.8.1/docs/assets/image.png
--rw-r--r--   0        0        0     4468 2020-02-02 00:00:00.000000 narwhals-0.8.1/docs/basics/column.md
--rw-r--r--   0        0        0     3572 2020-02-02 00:00:00.000000 narwhals-0.8.1/docs/basics/complete_example.md
--rw-r--r--   0        0        0     4278 2020-02-02 00:00:00.000000 narwhals-0.8.1/docs/basics/dataframe.md
--rw-r--r--   0        0        0     2523 2020-02-02 00:00:00.000000 narwhals-0.8.1/docs/other/pandas_index.md
--rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 narwhals-0.8.1/narwhals/__init__.py
--rw-r--r--   0        0        0    90926 2020-02-02 00:00:00.000000 narwhals-0.8.1/narwhals/dataframe.py
--rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 narwhals-0.8.1/narwhals/dependencies.py
--rw-r--r--   0        0        0     2791 2020-02-02 00:00:00.000000 narwhals-0.8.1/narwhals/dtypes.py
--rw-r--r--   0        0        0    27381 2020-02-02 00:00:00.000000 narwhals-0.8.1/narwhals/expression.py
--rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 narwhals-0.8.1/narwhals/functions.py
--rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 narwhals-0.8.1/narwhals/group_by.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.1/narwhals/py.typed
--rw-r--r--   0        0        0     6572 2020-02-02 00:00:00.000000 narwhals-0.8.1/narwhals/series.py
--rw-r--r--   0        0        0     7100 2020-02-02 00:00:00.000000 narwhals-0.8.1/narwhals/translate.py
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 narwhals-0.8.1/narwhals/typing.py
--rw-r--r--   0        0        0     2268 2020-02-02 00:00:00.000000 narwhals-0.8.1/narwhals/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.1/narwhals/_pandas_like/__init__.py
--rw-r--r--   0        0        0     7838 2020-02-02 00:00:00.000000 narwhals-0.8.1/narwhals/_pandas_like/dataframe.py
--rw-r--r--   0        0        0    10698 2020-02-02 00:00:00.000000 narwhals-0.8.1/narwhals/_pandas_like/expr.py
--rw-r--r--   0        0        0     5640 2020-02-02 00:00:00.000000 narwhals-0.8.1/narwhals/_pandas_like/group_by.py
--rw-r--r--   0        0        0     6324 2020-02-02 00:00:00.000000 narwhals-0.8.1/narwhals/_pandas_like/namespace.py
--rw-r--r--   0        0        0    14369 2020-02-02 00:00:00.000000 narwhals-0.8.1/narwhals/_pandas_like/series.py
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 narwhals-0.8.1/narwhals/_pandas_like/typing.py
--rw-r--r--   0        0        0    13436 2020-02-02 00:00:00.000000 narwhals-0.8.1/narwhals/_pandas_like/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.1/tests/__init__.py
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 narwhals-0.8.1/tests/conftest.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.1/tests/group_by_test.py
--rw-r--r--   0        0        0    22181 2020-02-02 00:00:00.000000 narwhals-0.8.1/tests/test_common.py
--rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 narwhals-0.8.1/tests/test_dt.py
--rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 narwhals-0.8.1/tests/test_group_by.py
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 narwhals-0.8.1/tests/test_invalid.py
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 narwhals-0.8.1/tests/test_pandas.py
--rw-r--r--   0        0        0     8935 2020-02-02 00:00:00.000000 narwhals-0.8.1/tests/test_series.py
--rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 narwhals-0.8.1/tests/test_str.py
--rw-r--r--   0        0        0     7276 2020-02-02 00:00:00.000000 narwhals-0.8.1/tests/tpch_q1_test.py
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 narwhals-0.8.1/tests/utils.py
--rw-r--r--   0        0        0    21551 2020-02-02 00:00:00.000000 narwhals-0.8.1/tests/data/customer.parquet
--rw-r--r--   0        0        0    34095 2020-02-02 00:00:00.000000 narwhals-0.8.1/tests/data/lineitem.parquet
--rw-r--r--   0        0        0     2139 2020-02-02 00:00:00.000000 narwhals-0.8.1/tests/data/nation.parquet
--rw-r--r--   0        0        0    24714 2020-02-02 00:00:00.000000 narwhals-0.8.1/tests/data/orders.parquet
--rw-r--r--   0        0        0    13276 2020-02-02 00:00:00.000000 narwhals-0.8.1/tests/data/part.parquet
--rw-r--r--   0        0        0    14921 2020-02-02 00:00:00.000000 narwhals-0.8.1/tests/data/partsupp.parquet
--rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 narwhals-0.8.1/tests/data/region.parquet
--rw-r--r--   0        0        0    19817 2020-02-02 00:00:00.000000 narwhals-0.8.1/tests/data/supplier.parquet
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.1/tests/expr/__init__.py
--rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 narwhals-0.8.1/tests/expr/over_test.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.1/tests/expr/test_over.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.1/tests/expr/str/__init__.py
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 narwhals-0.8.1/tests/expr/str/to_datetime_test.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.1/tests/hypothesis/__init__.py
--rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 narwhals-0.8.1/tests/hypothesis/test_basic_arithmetic.py
--rw-r--r--   0        0        0     1897 2020-02-02 00:00:00.000000 narwhals-0.8.1/tests/hypothesis/test_concat.py
--rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 narwhals-0.8.1/tests/hypothesis/test_join.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.1/tpch/__init__.py
--rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 narwhals-0.8.1/tpch/q1.py
--rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 narwhals-0.8.1/tpch/q2.py
--rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 narwhals-0.8.1/tpch/q3.py
--rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 narwhals-0.8.1/tpch/q4.py
--rw-r--r--   0        0        0     2900 2020-02-02 00:00:00.000000 narwhals-0.8.1/tpch/q5.py
--rwxr-xr-x   0        0        0    47336 2020-02-02 00:00:00.000000 narwhals-0.8.1/tpch/notebooks/gpu/execute.ipynb
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 narwhals-0.8.1/tpch/notebooks/gpu/kernel-metadata.json
--rwxr-xr-x   0        0        0    17860 2020-02-02 00:00:00.000000 narwhals-0.8.1/tpch/notebooks/q1/execute.ipynb
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.8.1/tpch/notebooks/q1/kernel-metadata.json
--rwxr-xr-x   0        0        0    18811 2020-02-02 00:00:00.000000 narwhals-0.8.1/tpch/notebooks/q2/execute.ipynb
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.8.1/tpch/notebooks/q2/kernel-metadata.json
--rwxr-xr-x   0        0        0    17692 2020-02-02 00:00:00.000000 narwhals-0.8.1/tpch/notebooks/q3/execute.ipynb
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.8.1/tpch/notebooks/q3/kernel-metadata.json
--rwxr-xr-x   0        0        0    16689 2020-02-02 00:00:00.000000 narwhals-0.8.1/tpch/notebooks/q4/execute.ipynb
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.8.1/tpch/notebooks/q4/kernel-metadata.json
--rwxr-xr-x   0        0        0    18235 2020-02-02 00:00:00.000000 narwhals-0.8.1/tpch/notebooks/q5/execute.ipynb
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.8.1/tpch/notebooks/q5/kernel-metadata.json
--rwxr-xr-x   0        0        0    16156 2020-02-02 00:00:00.000000 narwhals-0.8.1/tpch/notebooks/q6/execute.ipynb
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.8.1/tpch/notebooks/q6/kernel-metadata.json
--rwxr-xr-x   0        0        0    27860 2020-02-02 00:00:00.000000 narwhals-0.8.1/tpch/notebooks/q7/execute.ipynb
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.8.1/tpch/notebooks/q7/kernel-metadata.json
--rwxr-xr-x   0        0        0    27709 2020-02-02 00:00:00.000000 narwhals-0.8.1/tpch/notebooks/q8/execute.ipynb
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.8.1/tpch/notebooks/q8/kernel-metadata.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.1/utils/__init__.py
--rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 narwhals-0.8.1/utils/bump_version.py
--rw-r--r--   0        0        0     4163 2020-02-02 00:00:00.000000 narwhals-0.8.1/utils/check_api_reference.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 narwhals-0.8.1/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 narwhals-0.8.1/LICENSE.md
--rw-r--r--   0        0        0     3229 2020-02-02 00:00:00.000000 narwhals-0.8.1/README.md
--rw-r--r--   0        0        0     1995 2020-02-02 00:00:00.000000 narwhals-0.8.1/pyproject.toml
--rw-r--r--   0        0        0     3958 2020-02-02 00:00:00.000000 narwhals-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 narwhals-0.8.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 narwhals-0.8.2/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 narwhals-0.8.2/mkdocs.yml
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 narwhals-0.8.2/requirements-dev.txt
+-rw-r--r--   0        0        0     5243 2020-02-02 00:00:00.000000 narwhals-0.8.2/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     3725 2020-02-02 00:00:00.000000 narwhals-0.8.2/.github/workflows/extremes.yml
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 narwhals-0.8.2/.github/workflows/mkdocs.yml
+-rw-r--r--   0        0        0     2638 2020-02-02 00:00:00.000000 narwhals-0.8.2/.github/workflows/publish_to_pypi.yml
+-rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 narwhals-0.8.2/.github/workflows/pytest.yml
+-rw-r--r--   0        0        0     2021 2020-02-02 00:00:00.000000 narwhals-0.8.2/docs/extending.md
+-rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 narwhals-0.8.2/docs/generate_members.py
+-rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 narwhals-0.8.2/docs/index.md
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 narwhals-0.8.2/docs/installation.md
+-rw-r--r--   0        0        0     1245 2020-02-02 00:00:00.000000 narwhals-0.8.2/docs/quick_start.md
+-rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 narwhals-0.8.2/docs/related.md
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 narwhals-0.8.2/docs/requirements-docs.txt
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 narwhals-0.8.2/docs/roadmap.md
+-rw-r--r--   0        0        0     1281 2020-02-02 00:00:00.000000 narwhals-0.8.2/docs/why.md
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 narwhals-0.8.2/docs/api-reference/dataframe.md
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 narwhals-0.8.2/docs/api-reference/dependencies.md
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 narwhals-0.8.2/docs/api-reference/dtypes.md
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 narwhals-0.8.2/docs/api-reference/expressions.md
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 narwhals-0.8.2/docs/api-reference/expressions_dt.md
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 narwhals-0.8.2/docs/api-reference/expressions_str.md
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 narwhals-0.8.2/docs/api-reference/index.md
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 narwhals-0.8.2/docs/api-reference/lazyframe.md
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 narwhals-0.8.2/docs/api-reference/narwhals.md
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 narwhals-0.8.2/docs/api-reference/series.md
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 narwhals-0.8.2/docs/api-reference/series_dt.md
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 narwhals-0.8.2/docs/api-reference/series_str.md
+-rwxr-xr-x   0        0        0   132699 2020-02-02 00:00:00.000000 narwhals-0.8.2/docs/assets/image.png
+-rw-r--r--   0        0        0     4468 2020-02-02 00:00:00.000000 narwhals-0.8.2/docs/basics/column.md
+-rw-r--r--   0        0        0     3572 2020-02-02 00:00:00.000000 narwhals-0.8.2/docs/basics/complete_example.md
+-rw-r--r--   0        0        0     4278 2020-02-02 00:00:00.000000 narwhals-0.8.2/docs/basics/dataframe.md
+-rw-r--r--   0        0        0     2523 2020-02-02 00:00:00.000000 narwhals-0.8.2/docs/other/pandas_index.md
+-rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 narwhals-0.8.2/narwhals/__init__.py
+-rw-r--r--   0        0        0    90926 2020-02-02 00:00:00.000000 narwhals-0.8.2/narwhals/dataframe.py
+-rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 narwhals-0.8.2/narwhals/dependencies.py
+-rw-r--r--   0        0        0     3087 2020-02-02 00:00:00.000000 narwhals-0.8.2/narwhals/dtypes.py
+-rw-r--r--   0        0        0    34521 2020-02-02 00:00:00.000000 narwhals-0.8.2/narwhals/expression.py
+-rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 narwhals-0.8.2/narwhals/functions.py
+-rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 narwhals-0.8.2/narwhals/group_by.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.2/narwhals/py.typed
+-rw-r--r--   0        0        0    10417 2020-02-02 00:00:00.000000 narwhals-0.8.2/narwhals/series.py
+-rw-r--r--   0        0        0     7100 2020-02-02 00:00:00.000000 narwhals-0.8.2/narwhals/translate.py
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 narwhals-0.8.2/narwhals/typing.py
+-rw-r--r--   0        0        0     2268 2020-02-02 00:00:00.000000 narwhals-0.8.2/narwhals/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.2/narwhals/_pandas_like/__init__.py
+-rw-r--r--   0        0        0     7838 2020-02-02 00:00:00.000000 narwhals-0.8.2/narwhals/_pandas_like/dataframe.py
+-rw-r--r--   0        0        0    11408 2020-02-02 00:00:00.000000 narwhals-0.8.2/narwhals/_pandas_like/expr.py
+-rw-r--r--   0        0        0     5640 2020-02-02 00:00:00.000000 narwhals-0.8.2/narwhals/_pandas_like/group_by.py
+-rw-r--r--   0        0        0     6324 2020-02-02 00:00:00.000000 narwhals-0.8.2/narwhals/_pandas_like/namespace.py
+-rw-r--r--   0        0        0    14909 2020-02-02 00:00:00.000000 narwhals-0.8.2/narwhals/_pandas_like/series.py
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 narwhals-0.8.2/narwhals/_pandas_like/typing.py
+-rw-r--r--   0        0        0    13436 2020-02-02 00:00:00.000000 narwhals-0.8.2/narwhals/_pandas_like/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.2/tests/__init__.py
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 narwhals-0.8.2/tests/conftest.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.2/tests/group_by_test.py
+-rw-r--r--   0        0        0    22286 2020-02-02 00:00:00.000000 narwhals-0.8.2/tests/test_common.py
+-rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 narwhals-0.8.2/tests/test_dt.py
+-rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 narwhals-0.8.2/tests/test_group_by.py
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 narwhals-0.8.2/tests/test_invalid.py
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 narwhals-0.8.2/tests/test_pandas.py
+-rw-r--r--   0        0        0     8935 2020-02-02 00:00:00.000000 narwhals-0.8.2/tests/test_series.py
+-rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 narwhals-0.8.2/tests/test_str.py
+-rw-r--r--   0        0        0     7276 2020-02-02 00:00:00.000000 narwhals-0.8.2/tests/tpch_q1_test.py
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 narwhals-0.8.2/tests/utils.py
+-rw-r--r--   0        0        0    21551 2020-02-02 00:00:00.000000 narwhals-0.8.2/tests/data/customer.parquet
+-rw-r--r--   0        0        0    34095 2020-02-02 00:00:00.000000 narwhals-0.8.2/tests/data/lineitem.parquet
+-rw-r--r--   0        0        0     2139 2020-02-02 00:00:00.000000 narwhals-0.8.2/tests/data/nation.parquet
+-rw-r--r--   0        0        0    24714 2020-02-02 00:00:00.000000 narwhals-0.8.2/tests/data/orders.parquet
+-rw-r--r--   0        0        0    13276 2020-02-02 00:00:00.000000 narwhals-0.8.2/tests/data/part.parquet
+-rw-r--r--   0        0        0    14921 2020-02-02 00:00:00.000000 narwhals-0.8.2/tests/data/partsupp.parquet
+-rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 narwhals-0.8.2/tests/data/region.parquet
+-rw-r--r--   0        0        0    19817 2020-02-02 00:00:00.000000 narwhals-0.8.2/tests/data/supplier.parquet
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.2/tests/expr/__init__.py
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 narwhals-0.8.2/tests/expr/cum_sum_test.py
+-rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 narwhals-0.8.2/tests/expr/diff_test.py
+-rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 narwhals-0.8.2/tests/expr/fill_null_test.py
+-rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 narwhals-0.8.2/tests/expr/over_test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.2/tests/expr/test_over.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.2/tests/expr/str/__init__.py
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 narwhals-0.8.2/tests/expr/str/head_test.py
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 narwhals-0.8.2/tests/expr/str/to_datetime_test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.2/tests/hypothesis/__init__.py
+-rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 narwhals-0.8.2/tests/hypothesis/test_basic_arithmetic.py
+-rw-r--r--   0        0        0     1897 2020-02-02 00:00:00.000000 narwhals-0.8.2/tests/hypothesis/test_concat.py
+-rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 narwhals-0.8.2/tests/hypothesis/test_join.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.2/tpch/__init__.py
+-rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 narwhals-0.8.2/tpch/q1.py
+-rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 narwhals-0.8.2/tpch/q2.py
+-rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 narwhals-0.8.2/tpch/q3.py
+-rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 narwhals-0.8.2/tpch/q4.py
+-rw-r--r--   0        0        0     2900 2020-02-02 00:00:00.000000 narwhals-0.8.2/tpch/q5.py
+-rwxr-xr-x   0        0        0    47336 2020-02-02 00:00:00.000000 narwhals-0.8.2/tpch/notebooks/gpu/execute.ipynb
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 narwhals-0.8.2/tpch/notebooks/gpu/kernel-metadata.json
+-rwxr-xr-x   0        0        0    17860 2020-02-02 00:00:00.000000 narwhals-0.8.2/tpch/notebooks/q1/execute.ipynb
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.8.2/tpch/notebooks/q1/kernel-metadata.json
+-rwxr-xr-x   0        0        0    18811 2020-02-02 00:00:00.000000 narwhals-0.8.2/tpch/notebooks/q2/execute.ipynb
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.8.2/tpch/notebooks/q2/kernel-metadata.json
+-rwxr-xr-x   0        0        0    17692 2020-02-02 00:00:00.000000 narwhals-0.8.2/tpch/notebooks/q3/execute.ipynb
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.8.2/tpch/notebooks/q3/kernel-metadata.json
+-rwxr-xr-x   0        0        0    16689 2020-02-02 00:00:00.000000 narwhals-0.8.2/tpch/notebooks/q4/execute.ipynb
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.8.2/tpch/notebooks/q4/kernel-metadata.json
+-rwxr-xr-x   0        0        0    18235 2020-02-02 00:00:00.000000 narwhals-0.8.2/tpch/notebooks/q5/execute.ipynb
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.8.2/tpch/notebooks/q5/kernel-metadata.json
+-rwxr-xr-x   0        0        0    16156 2020-02-02 00:00:00.000000 narwhals-0.8.2/tpch/notebooks/q6/execute.ipynb
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.8.2/tpch/notebooks/q6/kernel-metadata.json
+-rwxr-xr-x   0        0        0    27860 2020-02-02 00:00:00.000000 narwhals-0.8.2/tpch/notebooks/q7/execute.ipynb
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.8.2/tpch/notebooks/q7/kernel-metadata.json
+-rwxr-xr-x   0        0        0    27709 2020-02-02 00:00:00.000000 narwhals-0.8.2/tpch/notebooks/q8/execute.ipynb
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.8.2/tpch/notebooks/q8/kernel-metadata.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.2/utils/__init__.py
+-rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 narwhals-0.8.2/utils/bump_version.py
+-rw-r--r--   0        0        0     4163 2020-02-02 00:00:00.000000 narwhals-0.8.2/utils/check_api_reference.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 narwhals-0.8.2/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 narwhals-0.8.2/LICENSE.md
+-rw-r--r--   0        0        0     3229 2020-02-02 00:00:00.000000 narwhals-0.8.2/README.md
+-rw-r--r--   0        0        0     1995 2020-02-02 00:00:00.000000 narwhals-0.8.2/pyproject.toml
+-rw-r--r--   0        0        0     3958 2020-02-02 00:00:00.000000 narwhals-0.8.2/PKG-INFO
```

### Comparing `narwhals-0.8.1/.pre-commit-config.yaml` & `narwhals-0.8.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.1/CONTRIBUTING.md` & `narwhals-0.8.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.1/mkdocs.yml` & `narwhals-0.8.2/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.1/.github/CODE_OF_CONDUCT.md` & `narwhals-0.8.2/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.1/.github/workflows/extremes.yml` & `narwhals-0.8.2/.github/workflows/extremes.yml`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.1/.github/workflows/mkdocs.yml` & `narwhals-0.8.2/.github/workflows/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.1/.github/workflows/publish_to_pypi.yml` & `narwhals-0.8.2/.github/workflows/publish_to_pypi.yml`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.1/.github/workflows/pytest.yml` & `narwhals-0.8.2/.github/workflows/pytest.yml`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.1/docs/extending.md` & `narwhals-0.8.2/docs/extending.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.1/docs/generate_members.py` & `narwhals-0.8.2/docs/generate_members.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.1/docs/index.md` & `narwhals-0.8.2/docs/index.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.1/docs/quick_start.md` & `narwhals-0.8.2/docs/quick_start.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.1/docs/related.md` & `narwhals-0.8.2/docs/related.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.1/docs/roadmap.md` & `narwhals-0.8.2/docs/roadmap.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.1/docs/why.md` & `narwhals-0.8.2/docs/why.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.1/docs/api-reference/index.md` & `narwhals-0.8.2/docs/api-reference/index.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.1/docs/assets/image.png` & `narwhals-0.8.2/docs/assets/image.png`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.1/docs/basics/column.md` & `narwhals-0.8.2/docs/basics/column.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.1/docs/basics/complete_example.md` & `narwhals-0.8.2/docs/basics/complete_example.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.1/docs/basics/dataframe.md` & `narwhals-0.8.2/docs/basics/dataframe.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.1/docs/other/pandas_index.md` & `narwhals-0.8.2/docs/other/pandas_index.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.1/narwhals/__init__.py` & `narwhals-0.8.2/narwhals/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from narwhals.expression import sum
 from narwhals.expression import sum_horizontal
 from narwhals.functions import concat
 from narwhals.series import Series
 from narwhals.translate import from_native
 from narwhals.translate import to_native
 
-__version__ = "0.8.1"
+__version__ = "0.8.2"
 
 __all__ = [
     "concat",
     "to_native",
     "from_native",
     "all",
     "col",
```

### Comparing `narwhals-0.8.1/narwhals/dataframe.py` & `narwhals-0.8.2/narwhals/dataframe.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.1/narwhals/dependencies.py` & `narwhals-0.8.2/narwhals/dependencies.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.1/narwhals/dtypes.py` & `narwhals-0.8.2/narwhals/dtypes.py`

 * *Files 8% similar despite different names*

```diff
@@ -66,14 +66,22 @@
 class Datetime(TemporalType): ...
 
 
 class Date(TemporalType): ...
 
 
 def translate_dtype(plx: Any, dtype: DType) -> Any:
+    if "polars" in str(type(dtype)):
+        msg = (
+            f"Expected Narwhals object, got: {type(dtype)}.\n\n"
+            "Perhaps you:\n"
+            "- Forgot a `nw.from_native` somewhere?\n"
+            "- Used `pl.Int64` instead of `nw.Int64`?"
+        )
+        raise TypeError(msg)
     if dtype == Float64:
         return plx.Float64
     if dtype == Float32:
         return plx.Float32
     if dtype == Int64:
         return plx.Int64
     if dtype == Int32:
```

### Comparing `narwhals-0.8.1/narwhals/expression.py` & `narwhals-0.8.2/narwhals/expression.py`

 * *Files 14% similar despite different names*

```diff
@@ -486,15 +486,15 @@
             │ 5   ┆ 3   │
             └─────┴─────┘
         """
         return self.__class__(lambda plx: self._call(plx).n_unique())
 
     def unique(self) -> Expr:
         """
-         Returns unique values
+        Return unique values
 
         Examples:
             >>> import polars as pl
             >>> import pandas as pd
             >>> import narwhals as nw
             >>> df_pd = pd.DataFrame({'a': [1, 1, 3, 5, 5], 'b': [2, 4, 4, 6, 6]})
             >>> df_pl = pl.DataFrame({'a': [1, 1, 3, 5, 5], 'b': [2, 4, 4, 6, 6]})
@@ -523,14 +523,111 @@
             │ 1   ┆ 2   │
             │ 3   ┆ 4   │
             │ 5   ┆ 6   │
             └─────┴─────┘
         """
         return self.__class__(lambda plx: self._call(plx).unique())
 
+    def cum_sum(self) -> Expr:
+        """
+        Return cumulative sum.
+
+        Examples:
+            >>> import polars as pl
+            >>> import pandas as pd
+            >>> import narwhals as nw
+            >>> df_pd = pd.DataFrame({'a': [1, 1, 3, 5, 5], 'b': [2, 4, 4, 6, 6]})
+            >>> df_pl = pl.DataFrame({'a': [1, 1, 3, 5, 5], 'b': [2, 4, 4, 6, 6]})
+
+            Let's define a dataframe-agnostic function:
+
+            >>> def func(df_any):
+            ...    df = nw.from_native(df_any)
+            ...    df = df.select(nw.col('a', 'b').cum_sum())
+            ...    return nw.to_native(df)
+
+            We can then pass either pandas or Polars to `func`:
+
+            >>> func(df_pd)
+                a   b
+            0   1   2
+            1   2   6
+            2   5  10
+            3  10  16
+            4  15  22
+            >>> func(df_pl)
+            shape: (5, 2)
+            ┌─────┬─────┐
+            │ a   ┆ b   │
+            │ --- ┆ --- │
+            │ i64 ┆ i64 │
+            ╞═════╪═════╡
+            │ 1   ┆ 2   │
+            │ 2   ┆ 6   │
+            │ 5   ┆ 10  │
+            │ 10  ┆ 16  │
+            │ 15  ┆ 22  │
+            └─────┴─────┘
+        """
+        return self.__class__(lambda plx: self._call(plx).cum_sum())
+
+    def diff(self) -> Expr:
+        """
+        Returns the difference between each element and the previous one.
+
+        Notes:
+            pandas may change the dtype here, for example when introducing missing
+            values in an integer column. To ensure, that the dtype doesn't change,
+            you may want to use `fill_null` and `cast`. For example, to calculate
+            the diff and fill missing values with `0` in a Int64 column, you could
+            do:
+
+            ```python
+            nw.col('a').diff().fill_null(0).cast(nw.Int64)
+            ```
+
+        Examples:
+            >>> import polars as pl
+            >>> import pandas as pd
+            >>> import narwhals as nw
+            >>> df_pd = pd.DataFrame({'a': [1, 1, 3, 5, 5]})
+            >>> df_pl = pl.DataFrame({'a': [1, 1, 3, 5, 5]})
+
+            Let's define a dataframe-agnostic function:
+
+            >>> def func(df_any):
+            ...    df = nw.from_native(df_any)
+            ...    df = df.select(a_diff=nw.col('a').diff())
+            ...    return nw.to_native(df)
+
+            We can then pass either pandas or Polars to `func`:
+
+            >>> func(df_pd)
+               a_diff
+            0     NaN
+            1     0.0
+            2     2.0
+            3     2.0
+            4     0.0
+            >>> func(df_pl)
+            shape: (5, 1)
+            ┌────────┐
+            │ a_diff │
+            │ ---    │
+            │ i64    │
+            ╞════════╡
+            │ null   │
+            │ 0      │
+            │ 2      │
+            │ 2      │
+            │ 0      │
+            └────────┘
+        """
+        return self.__class__(lambda plx: self._call(plx).diff())
+
     def sort(self, *, descending: bool = False) -> Expr:
         return self.__class__(lambda plx: self._call(plx).sort(descending=descending))
 
     # --- transform ---
     def is_between(
         self, lower_bound: Any, upper_bound: Any, closed: str = "both"
     ) -> Expr:
@@ -546,14 +643,18 @@
             lambda plx: self._call(plx).filter(extract_native(plx, other))
         )
 
     def is_null(self) -> Expr:
         """
         Returns a boolean Series indicating which values are null.
 
+        Notes:
+            pandas and Polars handle null values differently. Polars distinguishes
+            between NaN and Null, whereas pandas doesn't.
+
         Examples:
             >>> import pandas as pd
             >>> import polars as pl
             >>> import narwhals as nw
             >>> df_pd = pd.DataFrame(
             ...         {
             ...             'a': [2, 4, None, 3, 5],
@@ -599,14 +700,72 @@
             │ null ┆ NaN ┆ true      ┆ false     │
             │ 3    ┆ 3.0 ┆ false     ┆ false     │
             │ 5    ┆ 5.0 ┆ false     ┆ false     │
             └──────┴─────┴───────────┴───────────┘
         """
         return self.__class__(lambda plx: self._call(plx).is_null())
 
+    def fill_null(self, value: Any) -> Expr:
+        """
+        Fill null values with given value.
+
+        Notes:
+            pandas and Polars handle null values differently. Polars distinguishes
+            between NaN and Null, whereas pandas doesn't.
+
+        Examples:
+            >>> import pandas as pd
+            >>> import polars as pl
+            >>> import narwhals as nw
+            >>> df_pd = pd.DataFrame(
+            ...         {
+            ...             'a': [2, 4, None, 3, 5],
+            ...             'b': [2.0, 4.0, float("nan"), 3.0, 5.0]
+            ...         }
+            ... )
+            >>> df_pl = pl.DataFrame(
+            ...         {
+            ...             'a': [2, 4, None, 3, 5],
+            ...             'b': [2.0, 4.0, float("nan"), 3.0, 5.0]
+            ...         }
+            ... )
+
+            Let's define a dataframe-agnostic function:
+
+            >>> def func(df_any):
+            ...     df = nw.from_native(df_any)
+            ...     df = df.with_columns(nw.col('a', 'b').fill_null(0))
+            ...     return nw.to_native(df)
+
+            We can then pass either pandas or Polars to `func`:
+
+            >>> func(df_pd)
+                 a    b
+            0  2.0  2.0
+            1  4.0  4.0
+            2  0.0  0.0
+            3  3.0  3.0
+            4  5.0  5.0
+
+            >>> func(df_pl)  # nan != null for polars
+            shape: (5, 2)
+            ┌─────┬─────┐
+            │ a   ┆ b   │
+            │ --- ┆ --- │
+            │ i64 ┆ f64 │
+            ╞═════╪═════╡
+            │ 2   ┆ 2.0 │
+            │ 4   ┆ 4.0 │
+            │ 0   ┆ NaN │
+            │ 3   ┆ 3.0 │
+            │ 5   ┆ 5.0 │
+            └─────┴─────┘
+        """
+        return self.__class__(lambda plx: self._call(plx).fill_null(value))
+
     # --- partial reduction ---
     def drop_nulls(self) -> Expr:
         return self.__class__(lambda plx: self._call(plx).drop_nulls())
 
     def sample(
         self,
         n: int | None = None,
@@ -681,14 +840,65 @@
         self._expr = expr
 
     def ends_with(self, suffix: str) -> Expr:
         return self._expr.__class__(
             lambda plx: self._expr._call(plx).str.ends_with(suffix)
         )
 
+    def head(self, n: int = 5) -> Expr:
+        """
+        Take the first n elements of each string.
+
+        Arguments:
+            n: Number of elements to take.
+
+        Examples:
+            >>> import pandas as pd
+            >>> import polars as pl
+            >>> import narwhals as nw
+            >>> data = {'lyrics': ['Atatata', 'taata', 'taatatata', 'zukkyun']}
+            >>> df_pd = pd.DataFrame(data)
+            >>> df_pl = pl.DataFrame(data)
+
+            We define a data-frame agnostic function:
+
+            >>> def func(df_any):
+            ...     df = nw.from_native(df_any)
+            ...     df = df.with_columns(lyrics_head = nw.col('lyrics').str.head())
+            ...     return nw.to_native(df)
+
+            We can then pass either pandas or Polars to `func`:
+
+            >>> func(df_pd)
+                  lyrics lyrics_head
+            0    Atatata       Atata
+            1      taata       taata
+            2  taatatata       taata
+            3    zukkyun       zukky
+            >>> func(df_pl)
+            shape: (4, 2)
+            ┌───────────┬─────────────┐
+            │ lyrics    ┆ lyrics_head │
+            │ ---       ┆ ---         │
+            │ str       ┆ str         │
+            ╞═══════════╪═════════════╡
+            │ Atatata   ┆ Atata       │
+            │ taata     ┆ taata       │
+            │ taatatata ┆ taata       │
+            │ zukkyun   ┆ zukky       │
+            └───────────┴─────────────┘
+        """
+
+        def func(plx: Any) -> Any:
+            if plx is get_polars():
+                return self._expr._call(plx).str.slice(0, n)
+            return self._expr._call(plx).str.head(n)
+
+        return self._expr.__class__(func)
+
     def to_datetime(self, format: str) -> Expr:  # noqa: A002
         """
         Convert to Datetime dtype.
 
         Notes:
             pandas defaults to nanosecond time unit, Polars to microsecond.
             Prior to pandas 2.0, nanoseconds were the only time unit supported
```

### Comparing `narwhals-0.8.1/narwhals/functions.py` & `narwhals-0.8.2/narwhals/functions.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.1/narwhals/group_by.py` & `narwhals-0.8.2/narwhals/group_by.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.1/narwhals/translate.py` & `narwhals-0.8.2/narwhals/translate.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.1/narwhals/typing.py` & `narwhals-0.8.2/narwhals/typing.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.1/narwhals/utils.py` & `narwhals-0.8.2/narwhals/utils.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.1/narwhals/_pandas_like/dataframe.py` & `narwhals-0.8.2/narwhals/_pandas_like/dataframe.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.1/narwhals/_pandas_like/expr.py` & `narwhals-0.8.2/narwhals/_pandas_like/expr.py`

 * *Files 2% similar despite different names*

```diff
@@ -174,14 +174,17 @@
         return register_expression_call(
             self, "is_between", lower_bound, upper_bound, closed
         )
 
     def is_null(self) -> Self:
         return register_expression_call(self, "is_null")
 
+    def fill_null(self, value: Any) -> Self:
+        return register_expression_call(self, "fill_null", value)
+
     def is_in(self, other: Any) -> Self:
         return register_expression_call(self, "is_in", other)
 
     def filter(self, other: Any) -> Self:
         return register_expression_call(self, "filter", other)
 
     def drop_nulls(self) -> Self:
@@ -189,17 +192,23 @@
 
     def sort(self, *, descending: bool = False) -> Self:
         return register_expression_call(self, "sort", descending=descending)
 
     def n_unique(self) -> Self:
         return register_expression_call(self, "n_unique")
 
+    def cum_sum(self) -> Self:
+        return register_expression_call(self, "cum_sum")
+
     def unique(self) -> Self:
         return register_expression_call(self, "unique")
 
+    def diff(self) -> Self:
+        return register_expression_call(self, "diff")
+
     def sample(
         self,
         n: int | None = None,
         fraction: float | None = None,
         *,
         with_replacement: bool = False,
     ) -> Self:
@@ -268,14 +277,24 @@
             depth=self._expr._depth + 1,
             function_name=f"{self._expr._function_name}->str.ends_with",
             root_names=self._expr._root_names,
             output_names=self._expr._output_names,
             implementation=self._expr._implementation,
         )
 
+    def head(self, n: int = 5) -> PandasExpr:
+        return PandasExpr(
+            lambda df: [series.str.head(n) for series in self._expr._call(df)],
+            depth=self._expr._depth + 1,
+            function_name=f"{self._expr._function_name}->str.head",
+            root_names=self._expr._root_names,
+            output_names=self._expr._output_names,
+            implementation=self._expr._implementation,
+        )
+
     def to_datetime(self, format: str | None = None) -> PandasExpr:  # noqa: A002
         # TODO make a register_expression_call for namespaces
         return PandasExpr(
             lambda df: [
                 PandasSeries(
                     to_datetime(df._implementation)(series._series, format=format),
                     implementation=df._implementation,
```

### Comparing `narwhals-0.8.1/narwhals/_pandas_like/group_by.py` & `narwhals-0.8.2/narwhals/_pandas_like/group_by.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.1/narwhals/_pandas_like/namespace.py` & `narwhals-0.8.2/narwhals/_pandas_like/namespace.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.1/narwhals/_pandas_like/series.py` & `narwhals-0.8.2/narwhals/_pandas_like/series.py`

 * *Files 11% similar despite different names*

```diff
@@ -331,14 +331,18 @@
 
     # Transformations
 
     def is_null(self) -> PandasSeries:
         ser = self._series
         return self._from_series(ser.isna())
 
+    def fill_null(self, value: Any) -> PandasSeries:
+        ser = self._series
+        return self._from_series(ser.fillna(value))
+
     def drop_nulls(self) -> PandasSeries:
         ser = self._series
         return self._from_series(ser.dropna())
 
     def n_unique(self) -> int:
         ser = self._series
         return ser.nunique()  # type: ignore[no-any-return]
@@ -349,21 +353,31 @@
         fraction: float | None = None,
         *,
         with_replacement: bool = False,
     ) -> PandasSeries:
         ser = self._series
         return self._from_series(ser.sample(n=n, frac=fraction, replace=with_replacement))
 
-    def unique(self) -> PandasSeries:
+    def cum_sum(self) -> PandasSeries:
         return self._from_series(
             self._series.__class__(
-                self._series.unique(), dtype=self._series.dtype, name=self._series.name
+                self._series.cumsum(), dtype=self._series.dtype, name=self._series.name
             )
         )
 
+    def unique(self) -> PandasSeries:
+        return self._from_series(
+            self._series.__class__(self._series.unique(), name=self._series.name)
+        )
+
+    def diff(self) -> PandasSeries:
+        return self._from_series(
+            self._series.__class__(self._series.diff(), name=self._series.name)
+        )
+
     def sort(
         self,
         *,
         descending: bool | Sequence[bool] = False,
     ) -> PandasSeries:
         ser = self._series
         return self._from_series(
@@ -410,20 +424,23 @@
 
 
 class PandasSeriesStringNamespace:
     def __init__(self, series: PandasSeries) -> None:
         self._series = series
 
     def ends_with(self, suffix: str) -> PandasSeries:
-        # TODO make a register_expression_call for namespaces
-
         return self._series._from_series(
             self._series._series.str.endswith(suffix),
         )
 
+    def head(self, n: int = 5) -> PandasSeries:
+        return self._series._from_series(
+            self._series._series.str[:n],
+        )
+
 
 class PandasSeriesDateTimeNamespace:
     def __init__(self, series: PandasSeries) -> None:
         self._series = series
 
     def year(self) -> PandasSeries:
         return self._series._from_series(
```

### Comparing `narwhals-0.8.1/narwhals/_pandas_like/typing.py` & `narwhals-0.8.2/narwhals/_pandas_like/typing.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.1/narwhals/_pandas_like/utils.py` & `narwhals-0.8.2/narwhals/_pandas_like/utils.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.1/tests/conftest.py` & `narwhals-0.8.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.1/tests/test_common.py` & `narwhals-0.8.2/tests/test_common.py`

 * *Files 0% similar despite different names*

```diff
@@ -600,14 +600,16 @@
 
 def test_invalid() -> None:
     df = nw.LazyFrame(df_pandas)
     with pytest.raises(ValueError, match="Multi-output"):
         df.select(nw.all() + nw.all())
     with pytest.raises(TypeError, match="Perhaps you:"):
         df.select([pl.col("a")])  # type: ignore[list-item]
+    with pytest.raises(TypeError, match="Perhaps you:"):
+        df.select([nw.col("a").cast(pl.Int64)])
 
 
 @pytest.mark.parametrize("df_raw", [df_pandas])
 def test_reindex(df_raw: Any) -> None:
     df = nw.DataFrame(df_raw)
     result = df.select("b", df["a"].sort(descending=True))
     expected = {"b": [4, 4, 6], "a": [3, 2, 1]}
```

### Comparing `narwhals-0.8.1/tests/test_dt.py` & `narwhals-0.8.2/tests/test_dt.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.1/tests/test_group_by.py` & `narwhals-0.8.2/tests/test_group_by.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.1/tests/test_series.py` & `narwhals-0.8.2/tests/test_series.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.1/tests/test_str.py` & `narwhals-0.8.2/tests/test_str.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.1/tests/tpch_q1_test.py` & `narwhals-0.8.2/tests/tpch_q1_test.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.1/tests/utils.py` & `narwhals-0.8.2/tests/utils.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.1/tests/data/customer.parquet` & `narwhals-0.8.2/tests/data/customer.parquet`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.1/tests/data/lineitem.parquet` & `narwhals-0.8.2/tests/data/lineitem.parquet`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.1/tests/data/nation.parquet` & `narwhals-0.8.2/tests/data/nation.parquet`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.1/tests/data/orders.parquet` & `narwhals-0.8.2/tests/data/orders.parquet`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.1/tests/data/part.parquet` & `narwhals-0.8.2/tests/data/part.parquet`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.1/tests/data/partsupp.parquet` & `narwhals-0.8.2/tests/data/partsupp.parquet`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.1/tests/data/region.parquet` & `narwhals-0.8.2/tests/data/region.parquet`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.1/tests/data/supplier.parquet` & `narwhals-0.8.2/tests/data/supplier.parquet`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.1/tests/expr/over_test.py` & `narwhals-0.8.2/tests/expr/over_test.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.1/tests/expr/str/to_datetime_test.py` & `narwhals-0.8.2/tests/expr/str/to_datetime_test.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.1/tests/hypothesis/test_basic_arithmetic.py` & `narwhals-0.8.2/tests/hypothesis/test_basic_arithmetic.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.1/tests/hypothesis/test_concat.py` & `narwhals-0.8.2/tests/hypothesis/test_concat.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.1/tests/hypothesis/test_join.py` & `narwhals-0.8.2/tests/hypothesis/test_join.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.1/tpch/q1.py` & `narwhals-0.8.2/tpch/q1.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.1/tpch/q2.py` & `narwhals-0.8.2/tpch/q2.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.1/tpch/q3.py` & `narwhals-0.8.2/tpch/q3.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.1/tpch/q4.py` & `narwhals-0.8.2/tpch/q4.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.1/tpch/q5.py` & `narwhals-0.8.2/tpch/q5.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.1/tpch/notebooks/gpu/execute.ipynb` & `narwhals-0.8.2/tpch/notebooks/gpu/execute.ipynb`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.1/tpch/notebooks/q1/execute.ipynb` & `narwhals-0.8.2/tpch/notebooks/q1/execute.ipynb`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.1/tpch/notebooks/q2/execute.ipynb` & `narwhals-0.8.2/tpch/notebooks/q2/execute.ipynb`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.1/tpch/notebooks/q3/execute.ipynb` & `narwhals-0.8.2/tpch/notebooks/q3/execute.ipynb`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.1/tpch/notebooks/q4/execute.ipynb` & `narwhals-0.8.2/tpch/notebooks/q4/execute.ipynb`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.1/tpch/notebooks/q5/execute.ipynb` & `narwhals-0.8.2/tpch/notebooks/q5/execute.ipynb`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.1/tpch/notebooks/q6/execute.ipynb` & `narwhals-0.8.2/tpch/notebooks/q6/execute.ipynb`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.1/tpch/notebooks/q7/execute.ipynb` & `narwhals-0.8.2/tpch/notebooks/q7/execute.ipynb`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.1/tpch/notebooks/q8/execute.ipynb` & `narwhals-0.8.2/tpch/notebooks/q8/execute.ipynb`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.1/utils/bump_version.py` & `narwhals-0.8.2/utils/bump_version.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.1/utils/check_api_reference.py` & `narwhals-0.8.2/utils/check_api_reference.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.1/LICENSE.md` & `narwhals-0.8.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.1/README.md` & `narwhals-0.8.2/README.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.1/pyproject.toml` & `narwhals-0.8.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "narwhals"
-version = "0.8.1"
+version = "0.8.2"
 authors = [
   { name="Marco Gorelli", email="33491632+MarcoGorelli@users.noreply.github.com" },
 ]
 description = "Extremely lightweight compatibility layer between pandas, Polars, cuDF, and Modin"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `narwhals-0.8.1/PKG-INFO` & `narwhals-0.8.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: narwhals
-Version: 0.8.1
+Version: 0.8.2
 Summary: Extremely lightweight compatibility layer between pandas, Polars, cuDF, and Modin
 Project-URL: Homepage, https://github.com/MarcoGorelli/narwhals
 Project-URL: Bug Tracker, https://github.com/MarcoGorelli/narwhals
 Author-email: Marco Gorelli <33491632+MarcoGorelli@users.noreply.github.com>
 License-File: LICENSE.md
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

