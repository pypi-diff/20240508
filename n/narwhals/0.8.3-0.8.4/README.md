# Comparing `tmp/narwhals-0.8.3.tar.gz` & `tmp/narwhals-0.8.4.tar.gz`

## Comparing `narwhals-0.8.3.tar` & `narwhals-0.8.4.tar`

### file list

```diff
@@ -1,120 +1,122 @@
--rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 narwhals-0.8.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 narwhals-0.8.3/CONTRIBUTING.md
--rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 narwhals-0.8.3/mkdocs.yml
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 narwhals-0.8.3/requirements-dev.txt
--rw-r--r--   0        0        0     5243 2020-02-02 00:00:00.000000 narwhals-0.8.3/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     3725 2020-02-02 00:00:00.000000 narwhals-0.8.3/.github/workflows/extremes.yml
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 narwhals-0.8.3/.github/workflows/mkdocs.yml
--rw-r--r--   0        0        0     2638 2020-02-02 00:00:00.000000 narwhals-0.8.3/.github/workflows/publish_to_pypi.yml
--rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 narwhals-0.8.3/.github/workflows/pytest.yml
--rw-r--r--   0        0        0     2021 2020-02-02 00:00:00.000000 narwhals-0.8.3/docs/extending.md
--rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 narwhals-0.8.3/docs/generate_members.py
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 narwhals-0.8.3/docs/index.md
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 narwhals-0.8.3/docs/installation.md
--rw-r--r--   0        0        0     1245 2020-02-02 00:00:00.000000 narwhals-0.8.3/docs/quick_start.md
--rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 narwhals-0.8.3/docs/related.md
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 narwhals-0.8.3/docs/requirements-docs.txt
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 narwhals-0.8.3/docs/roadmap.md
--rw-r--r--   0        0        0     1281 2020-02-02 00:00:00.000000 narwhals-0.8.3/docs/why.md
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 narwhals-0.8.3/docs/api-reference/dataframe.md
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 narwhals-0.8.3/docs/api-reference/dependencies.md
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 narwhals-0.8.3/docs/api-reference/dtypes.md
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 narwhals-0.8.3/docs/api-reference/expressions.md
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 narwhals-0.8.3/docs/api-reference/expressions_dt.md
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 narwhals-0.8.3/docs/api-reference/expressions_str.md
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 narwhals-0.8.3/docs/api-reference/index.md
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 narwhals-0.8.3/docs/api-reference/lazyframe.md
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 narwhals-0.8.3/docs/api-reference/narwhals.md
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 narwhals-0.8.3/docs/api-reference/series.md
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 narwhals-0.8.3/docs/api-reference/series_dt.md
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 narwhals-0.8.3/docs/api-reference/series_str.md
--rwxr-xr-x   0        0        0   132699 2020-02-02 00:00:00.000000 narwhals-0.8.3/docs/assets/image.png
--rw-r--r--   0        0        0     4468 2020-02-02 00:00:00.000000 narwhals-0.8.3/docs/basics/column.md
--rw-r--r--   0        0        0     3572 2020-02-02 00:00:00.000000 narwhals-0.8.3/docs/basics/complete_example.md
--rw-r--r--   0        0        0     4278 2020-02-02 00:00:00.000000 narwhals-0.8.3/docs/basics/dataframe.md
--rw-r--r--   0        0        0     2523 2020-02-02 00:00:00.000000 narwhals-0.8.3/docs/other/pandas_index.md
--rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 narwhals-0.8.3/narwhals/__init__.py
--rw-r--r--   0        0        0    90926 2020-02-02 00:00:00.000000 narwhals-0.8.3/narwhals/dataframe.py
--rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 narwhals-0.8.3/narwhals/dependencies.py
--rw-r--r--   0        0        0     3087 2020-02-02 00:00:00.000000 narwhals-0.8.3/narwhals/dtypes.py
--rw-r--r--   0        0        0    34521 2020-02-02 00:00:00.000000 narwhals-0.8.3/narwhals/expression.py
--rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 narwhals-0.8.3/narwhals/functions.py
--rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 narwhals-0.8.3/narwhals/group_by.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.3/narwhals/py.typed
--rw-r--r--   0        0        0    10417 2020-02-02 00:00:00.000000 narwhals-0.8.3/narwhals/series.py
--rw-r--r--   0        0        0     7100 2020-02-02 00:00:00.000000 narwhals-0.8.3/narwhals/translate.py
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 narwhals-0.8.3/narwhals/typing.py
--rw-r--r--   0        0        0     2268 2020-02-02 00:00:00.000000 narwhals-0.8.3/narwhals/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.3/narwhals/_pandas_like/__init__.py
--rw-r--r--   0        0        0     7838 2020-02-02 00:00:00.000000 narwhals-0.8.3/narwhals/_pandas_like/dataframe.py
--rw-r--r--   0        0        0    11408 2020-02-02 00:00:00.000000 narwhals-0.8.3/narwhals/_pandas_like/expr.py
--rw-r--r--   0        0        0     5640 2020-02-02 00:00:00.000000 narwhals-0.8.3/narwhals/_pandas_like/group_by.py
--rw-r--r--   0        0        0     6324 2020-02-02 00:00:00.000000 narwhals-0.8.3/narwhals/_pandas_like/namespace.py
--rw-r--r--   0        0        0    14909 2020-02-02 00:00:00.000000 narwhals-0.8.3/narwhals/_pandas_like/series.py
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 narwhals-0.8.3/narwhals/_pandas_like/typing.py
--rw-r--r--   0        0        0    13436 2020-02-02 00:00:00.000000 narwhals-0.8.3/narwhals/_pandas_like/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.3/tests/__init__.py
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 narwhals-0.8.3/tests/conftest.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.3/tests/group_by_test.py
--rw-r--r--   0        0        0    22286 2020-02-02 00:00:00.000000 narwhals-0.8.3/tests/test_common.py
--rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 narwhals-0.8.3/tests/test_dt.py
--rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 narwhals-0.8.3/tests/test_group_by.py
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 narwhals-0.8.3/tests/test_invalid.py
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 narwhals-0.8.3/tests/test_pandas.py
--rw-r--r--   0        0        0     8935 2020-02-02 00:00:00.000000 narwhals-0.8.3/tests/test_series.py
--rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 narwhals-0.8.3/tests/test_str.py
--rw-r--r--   0        0        0     7276 2020-02-02 00:00:00.000000 narwhals-0.8.3/tests/tpch_q1_test.py
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 narwhals-0.8.3/tests/utils.py
--rw-r--r--   0        0        0    21551 2020-02-02 00:00:00.000000 narwhals-0.8.3/tests/data/customer.parquet
--rw-r--r--   0        0        0    34095 2020-02-02 00:00:00.000000 narwhals-0.8.3/tests/data/lineitem.parquet
--rw-r--r--   0        0        0     2139 2020-02-02 00:00:00.000000 narwhals-0.8.3/tests/data/nation.parquet
--rw-r--r--   0        0        0    24714 2020-02-02 00:00:00.000000 narwhals-0.8.3/tests/data/orders.parquet
--rw-r--r--   0        0        0    13276 2020-02-02 00:00:00.000000 narwhals-0.8.3/tests/data/part.parquet
--rw-r--r--   0        0        0    14921 2020-02-02 00:00:00.000000 narwhals-0.8.3/tests/data/partsupp.parquet
--rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 narwhals-0.8.3/tests/data/region.parquet
--rw-r--r--   0        0        0    19817 2020-02-02 00:00:00.000000 narwhals-0.8.3/tests/data/supplier.parquet
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.3/tests/expr/__init__.py
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 narwhals-0.8.3/tests/expr/cum_sum_test.py
--rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 narwhals-0.8.3/tests/expr/diff_test.py
--rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 narwhals-0.8.3/tests/expr/fill_null_test.py
--rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 narwhals-0.8.3/tests/expr/over_test.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.3/tests/expr/test_over.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.3/tests/expr/str/__init__.py
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 narwhals-0.8.3/tests/expr/str/head_test.py
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 narwhals-0.8.3/tests/expr/str/to_datetime_test.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.3/tests/hypothesis/__init__.py
--rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 narwhals-0.8.3/tests/hypothesis/test_basic_arithmetic.py
--rw-r--r--   0        0        0     1897 2020-02-02 00:00:00.000000 narwhals-0.8.3/tests/hypothesis/test_concat.py
--rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 narwhals-0.8.3/tests/hypothesis/test_join.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.3/tpch/__init__.py
--rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 narwhals-0.8.3/tpch/q1.py
--rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 narwhals-0.8.3/tpch/q2.py
--rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 narwhals-0.8.3/tpch/q3.py
--rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 narwhals-0.8.3/tpch/q4.py
--rw-r--r--   0        0        0     2900 2020-02-02 00:00:00.000000 narwhals-0.8.3/tpch/q5.py
--rwxr-xr-x   0        0        0    47336 2020-02-02 00:00:00.000000 narwhals-0.8.3/tpch/notebooks/gpu/execute.ipynb
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 narwhals-0.8.3/tpch/notebooks/gpu/kernel-metadata.json
--rwxr-xr-x   0        0        0    17860 2020-02-02 00:00:00.000000 narwhals-0.8.3/tpch/notebooks/q1/execute.ipynb
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.8.3/tpch/notebooks/q1/kernel-metadata.json
--rwxr-xr-x   0        0        0    18811 2020-02-02 00:00:00.000000 narwhals-0.8.3/tpch/notebooks/q2/execute.ipynb
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.8.3/tpch/notebooks/q2/kernel-metadata.json
--rwxr-xr-x   0        0        0    17692 2020-02-02 00:00:00.000000 narwhals-0.8.3/tpch/notebooks/q3/execute.ipynb
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.8.3/tpch/notebooks/q3/kernel-metadata.json
--rwxr-xr-x   0        0        0    16689 2020-02-02 00:00:00.000000 narwhals-0.8.3/tpch/notebooks/q4/execute.ipynb
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.8.3/tpch/notebooks/q4/kernel-metadata.json
--rwxr-xr-x   0        0        0    18235 2020-02-02 00:00:00.000000 narwhals-0.8.3/tpch/notebooks/q5/execute.ipynb
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.8.3/tpch/notebooks/q5/kernel-metadata.json
--rwxr-xr-x   0        0        0    16156 2020-02-02 00:00:00.000000 narwhals-0.8.3/tpch/notebooks/q6/execute.ipynb
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.8.3/tpch/notebooks/q6/kernel-metadata.json
--rwxr-xr-x   0        0        0    27860 2020-02-02 00:00:00.000000 narwhals-0.8.3/tpch/notebooks/q7/execute.ipynb
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.8.3/tpch/notebooks/q7/kernel-metadata.json
--rwxr-xr-x   0        0        0    27709 2020-02-02 00:00:00.000000 narwhals-0.8.3/tpch/notebooks/q8/execute.ipynb
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.8.3/tpch/notebooks/q8/kernel-metadata.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.3/utils/__init__.py
--rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 narwhals-0.8.3/utils/bump_version.py
--rw-r--r--   0        0        0     4163 2020-02-02 00:00:00.000000 narwhals-0.8.3/utils/check_api_reference.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 narwhals-0.8.3/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 narwhals-0.8.3/LICENSE.md
--rw-r--r--   0        0        0     3229 2020-02-02 00:00:00.000000 narwhals-0.8.3/README.md
--rw-r--r--   0        0        0     1995 2020-02-02 00:00:00.000000 narwhals-0.8.3/pyproject.toml
--rw-r--r--   0        0        0     3958 2020-02-02 00:00:00.000000 narwhals-0.8.3/PKG-INFO
+-rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 narwhals-0.8.4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 narwhals-0.8.4/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 narwhals-0.8.4/mkdocs.yml
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 narwhals-0.8.4/requirements-dev.txt
+-rw-r--r--   0        0        0     5243 2020-02-02 00:00:00.000000 narwhals-0.8.4/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     3725 2020-02-02 00:00:00.000000 narwhals-0.8.4/.github/workflows/extremes.yml
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 narwhals-0.8.4/.github/workflows/mkdocs.yml
+-rw-r--r--   0        0        0     2638 2020-02-02 00:00:00.000000 narwhals-0.8.4/.github/workflows/publish_to_pypi.yml
+-rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 narwhals-0.8.4/.github/workflows/pytest.yml
+-rw-r--r--   0        0        0     2021 2020-02-02 00:00:00.000000 narwhals-0.8.4/docs/extending.md
+-rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 narwhals-0.8.4/docs/generate_members.py
+-rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 narwhals-0.8.4/docs/index.md
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 narwhals-0.8.4/docs/installation.md
+-rw-r--r--   0        0        0     1245 2020-02-02 00:00:00.000000 narwhals-0.8.4/docs/quick_start.md
+-rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 narwhals-0.8.4/docs/related.md
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 narwhals-0.8.4/docs/requirements-docs.txt
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 narwhals-0.8.4/docs/roadmap.md
+-rw-r--r--   0        0        0     1281 2020-02-02 00:00:00.000000 narwhals-0.8.4/docs/why.md
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 narwhals-0.8.4/docs/api-reference/dataframe.md
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 narwhals-0.8.4/docs/api-reference/dependencies.md
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 narwhals-0.8.4/docs/api-reference/dtypes.md
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 narwhals-0.8.4/docs/api-reference/expressions.md
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 narwhals-0.8.4/docs/api-reference/expressions_dt.md
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 narwhals-0.8.4/docs/api-reference/expressions_str.md
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 narwhals-0.8.4/docs/api-reference/index.md
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 narwhals-0.8.4/docs/api-reference/lazyframe.md
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 narwhals-0.8.4/docs/api-reference/narwhals.md
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 narwhals-0.8.4/docs/api-reference/series.md
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 narwhals-0.8.4/docs/api-reference/series_dt.md
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 narwhals-0.8.4/docs/api-reference/series_str.md
+-rwxr-xr-x   0        0        0   132699 2020-02-02 00:00:00.000000 narwhals-0.8.4/docs/assets/image.png
+-rw-r--r--   0        0        0     4468 2020-02-02 00:00:00.000000 narwhals-0.8.4/docs/basics/column.md
+-rw-r--r--   0        0        0     3572 2020-02-02 00:00:00.000000 narwhals-0.8.4/docs/basics/complete_example.md
+-rw-r--r--   0        0        0     4278 2020-02-02 00:00:00.000000 narwhals-0.8.4/docs/basics/dataframe.md
+-rw-r--r--   0        0        0     2523 2020-02-02 00:00:00.000000 narwhals-0.8.4/docs/other/pandas_index.md
+-rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 narwhals-0.8.4/narwhals/__init__.py
+-rw-r--r--   0        0        0    93496 2020-02-02 00:00:00.000000 narwhals-0.8.4/narwhals/dataframe.py
+-rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 narwhals-0.8.4/narwhals/dependencies.py
+-rw-r--r--   0        0        0     3087 2020-02-02 00:00:00.000000 narwhals-0.8.4/narwhals/dtypes.py
+-rw-r--r--   0        0        0    35843 2020-02-02 00:00:00.000000 narwhals-0.8.4/narwhals/expression.py
+-rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 narwhals-0.8.4/narwhals/functions.py
+-rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 narwhals-0.8.4/narwhals/group_by.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.4/narwhals/py.typed
+-rw-r--r--   0        0        0    10417 2020-02-02 00:00:00.000000 narwhals-0.8.4/narwhals/series.py
+-rw-r--r--   0        0        0     7100 2020-02-02 00:00:00.000000 narwhals-0.8.4/narwhals/translate.py
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 narwhals-0.8.4/narwhals/typing.py
+-rw-r--r--   0        0        0     2268 2020-02-02 00:00:00.000000 narwhals-0.8.4/narwhals/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.4/narwhals/_pandas_like/__init__.py
+-rw-r--r--   0        0        0     7838 2020-02-02 00:00:00.000000 narwhals-0.8.4/narwhals/_pandas_like/dataframe.py
+-rw-r--r--   0        0        0    11408 2020-02-02 00:00:00.000000 narwhals-0.8.4/narwhals/_pandas_like/expr.py
+-rw-r--r--   0        0        0     5640 2020-02-02 00:00:00.000000 narwhals-0.8.4/narwhals/_pandas_like/group_by.py
+-rw-r--r--   0        0        0     6324 2020-02-02 00:00:00.000000 narwhals-0.8.4/narwhals/_pandas_like/namespace.py
+-rw-r--r--   0        0        0    14909 2020-02-02 00:00:00.000000 narwhals-0.8.4/narwhals/_pandas_like/series.py
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 narwhals-0.8.4/narwhals/_pandas_like/typing.py
+-rw-r--r--   0        0        0    13436 2020-02-02 00:00:00.000000 narwhals-0.8.4/narwhals/_pandas_like/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.4/tests/__init__.py
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 narwhals-0.8.4/tests/conftest.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.4/tests/group_by_test.py
+-rw-r--r--   0        0        0    22286 2020-02-02 00:00:00.000000 narwhals-0.8.4/tests/test_common.py
+-rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 narwhals-0.8.4/tests/test_dt.py
+-rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 narwhals-0.8.4/tests/test_group_by.py
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 narwhals-0.8.4/tests/test_invalid.py
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 narwhals-0.8.4/tests/test_pandas.py
+-rw-r--r--   0        0        0     8935 2020-02-02 00:00:00.000000 narwhals-0.8.4/tests/test_series.py
+-rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 narwhals-0.8.4/tests/test_str.py
+-rw-r--r--   0        0        0     7276 2020-02-02 00:00:00.000000 narwhals-0.8.4/tests/tpch_q1_test.py
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 narwhals-0.8.4/tests/utils.py
+-rw-r--r--   0        0        0    21551 2020-02-02 00:00:00.000000 narwhals-0.8.4/tests/data/customer.parquet
+-rw-r--r--   0        0        0    34095 2020-02-02 00:00:00.000000 narwhals-0.8.4/tests/data/lineitem.parquet
+-rw-r--r--   0        0        0     2139 2020-02-02 00:00:00.000000 narwhals-0.8.4/tests/data/nation.parquet
+-rw-r--r--   0        0        0    24714 2020-02-02 00:00:00.000000 narwhals-0.8.4/tests/data/orders.parquet
+-rw-r--r--   0        0        0    13276 2020-02-02 00:00:00.000000 narwhals-0.8.4/tests/data/part.parquet
+-rw-r--r--   0        0        0    14921 2020-02-02 00:00:00.000000 narwhals-0.8.4/tests/data/partsupp.parquet
+-rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 narwhals-0.8.4/tests/data/region.parquet
+-rw-r--r--   0        0        0    19817 2020-02-02 00:00:00.000000 narwhals-0.8.4/tests/data/supplier.parquet
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.4/tests/expr/__init__.py
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 narwhals-0.8.4/tests/expr/cum_sum_test.py
+-rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 narwhals-0.8.4/tests/expr/diff_test.py
+-rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 narwhals-0.8.4/tests/expr/fill_null_test.py
+-rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 narwhals-0.8.4/tests/expr/over_test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.4/tests/expr/test_over.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.4/tests/expr/str/__init__.py
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 narwhals-0.8.4/tests/expr/str/head_test.py
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 narwhals-0.8.4/tests/expr/str/to_datetime_test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.4/tests/frame/__init__.py
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 narwhals-0.8.4/tests/frame/pipe_test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.4/tests/hypothesis/__init__.py
+-rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 narwhals-0.8.4/tests/hypothesis/test_basic_arithmetic.py
+-rw-r--r--   0        0        0     1897 2020-02-02 00:00:00.000000 narwhals-0.8.4/tests/hypothesis/test_concat.py
+-rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 narwhals-0.8.4/tests/hypothesis/test_join.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.4/tpch/__init__.py
+-rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 narwhals-0.8.4/tpch/q1.py
+-rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 narwhals-0.8.4/tpch/q2.py
+-rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 narwhals-0.8.4/tpch/q3.py
+-rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 narwhals-0.8.4/tpch/q4.py
+-rw-r--r--   0        0        0     2900 2020-02-02 00:00:00.000000 narwhals-0.8.4/tpch/q5.py
+-rwxr-xr-x   0        0        0    47336 2020-02-02 00:00:00.000000 narwhals-0.8.4/tpch/notebooks/gpu/execute.ipynb
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 narwhals-0.8.4/tpch/notebooks/gpu/kernel-metadata.json
+-rwxr-xr-x   0        0        0    17860 2020-02-02 00:00:00.000000 narwhals-0.8.4/tpch/notebooks/q1/execute.ipynb
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.8.4/tpch/notebooks/q1/kernel-metadata.json
+-rwxr-xr-x   0        0        0    18811 2020-02-02 00:00:00.000000 narwhals-0.8.4/tpch/notebooks/q2/execute.ipynb
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.8.4/tpch/notebooks/q2/kernel-metadata.json
+-rwxr-xr-x   0        0        0    17692 2020-02-02 00:00:00.000000 narwhals-0.8.4/tpch/notebooks/q3/execute.ipynb
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.8.4/tpch/notebooks/q3/kernel-metadata.json
+-rwxr-xr-x   0        0        0    16689 2020-02-02 00:00:00.000000 narwhals-0.8.4/tpch/notebooks/q4/execute.ipynb
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.8.4/tpch/notebooks/q4/kernel-metadata.json
+-rwxr-xr-x   0        0        0    18235 2020-02-02 00:00:00.000000 narwhals-0.8.4/tpch/notebooks/q5/execute.ipynb
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.8.4/tpch/notebooks/q5/kernel-metadata.json
+-rwxr-xr-x   0        0        0    16156 2020-02-02 00:00:00.000000 narwhals-0.8.4/tpch/notebooks/q6/execute.ipynb
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.8.4/tpch/notebooks/q6/kernel-metadata.json
+-rwxr-xr-x   0        0        0    27860 2020-02-02 00:00:00.000000 narwhals-0.8.4/tpch/notebooks/q7/execute.ipynb
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.8.4/tpch/notebooks/q7/kernel-metadata.json
+-rwxr-xr-x   0        0        0    27709 2020-02-02 00:00:00.000000 narwhals-0.8.4/tpch/notebooks/q8/execute.ipynb
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.8.4/tpch/notebooks/q8/kernel-metadata.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.4/utils/__init__.py
+-rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 narwhals-0.8.4/utils/bump_version.py
+-rw-r--r--   0        0        0     4163 2020-02-02 00:00:00.000000 narwhals-0.8.4/utils/check_api_reference.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 narwhals-0.8.4/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 narwhals-0.8.4/LICENSE.md
+-rw-r--r--   0        0        0     3229 2020-02-02 00:00:00.000000 narwhals-0.8.4/README.md
+-rw-r--r--   0        0        0     1995 2020-02-02 00:00:00.000000 narwhals-0.8.4/pyproject.toml
+-rw-r--r--   0        0        0     3958 2020-02-02 00:00:00.000000 narwhals-0.8.4/PKG-INFO
```

### Comparing `narwhals-0.8.3/.pre-commit-config.yaml` & `narwhals-0.8.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.3/CONTRIBUTING.md` & `narwhals-0.8.4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.3/mkdocs.yml` & `narwhals-0.8.4/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.3/.github/CODE_OF_CONDUCT.md` & `narwhals-0.8.4/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.3/.github/workflows/extremes.yml` & `narwhals-0.8.4/.github/workflows/extremes.yml`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.3/.github/workflows/mkdocs.yml` & `narwhals-0.8.4/.github/workflows/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.3/.github/workflows/publish_to_pypi.yml` & `narwhals-0.8.4/.github/workflows/publish_to_pypi.yml`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.3/.github/workflows/pytest.yml` & `narwhals-0.8.4/.github/workflows/pytest.yml`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.3/docs/extending.md` & `narwhals-0.8.4/docs/extending.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.3/docs/generate_members.py` & `narwhals-0.8.4/docs/generate_members.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.3/docs/index.md` & `narwhals-0.8.4/docs/index.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.3/docs/quick_start.md` & `narwhals-0.8.4/docs/quick_start.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.3/docs/related.md` & `narwhals-0.8.4/docs/related.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.3/docs/roadmap.md` & `narwhals-0.8.4/docs/roadmap.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.3/docs/why.md` & `narwhals-0.8.4/docs/why.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.3/docs/api-reference/index.md` & `narwhals-0.8.4/docs/api-reference/index.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.3/docs/api-reference/series.md` & `narwhals-0.8.4/docs/api-reference/series.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.3/docs/assets/image.png` & `narwhals-0.8.4/docs/assets/image.png`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.3/docs/basics/column.md` & `narwhals-0.8.4/docs/basics/column.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.3/docs/basics/complete_example.md` & `narwhals-0.8.4/docs/basics/complete_example.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.3/docs/basics/dataframe.md` & `narwhals-0.8.4/docs/basics/dataframe.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.3/docs/other/pandas_index.md` & `narwhals-0.8.4/docs/other/pandas_index.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.3/narwhals/__init__.py` & `narwhals-0.8.4/narwhals/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from narwhals.expression import sum
 from narwhals.expression import sum_horizontal
 from narwhals.functions import concat
 from narwhals.series import Series
 from narwhals.translate import from_native
 from narwhals.translate import to_native
 
-__version__ = "0.8.3"
+__version__ = "0.8.4"
 
 __all__ = [
     "concat",
     "to_native",
     "from_native",
     "all",
     "col",
```

### Comparing `narwhals-0.8.3/narwhals/dataframe.py` & `narwhals-0.8.4/narwhals/dataframe.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 from typing import Any
+from typing import Callable
 from typing import Iterable
 from typing import Literal
 from typing import Sequence
 
 from narwhals._pandas_like.dataframe import PandasDataFrame
 from narwhals.dependencies import get_polars
 from narwhals.dtypes import to_narwhals_dtype
@@ -73,14 +74,17 @@
     @property
     def schema(self) -> dict[str, DType]:
         return {
             k: to_narwhals_dtype(v, is_polars=self._is_polars)
             for k, v in self._dataframe.schema.items()
         }
 
+    def pipe(self, function: Callable[[Any], Self], *args: Any, **kwargs: Any) -> Self:
+        return function(self, *args, **kwargs)
+
     @property
     def columns(self) -> list[str]:
         return self._dataframe.columns  # type: ignore[no-any-return]
 
     def lazy(self) -> LazyFrame:
         return LazyFrame(
             self._dataframe.lazy(),
@@ -429,14 +433,54 @@
                 2
                 -30
             ]}
         """
         return self._dataframe.to_dict(as_series=as_series)  # type: ignore[no-any-return]
 
     # inherited
+    def pipe(self, function: Callable[[Any], Self], *args: Any, **kwargs: Any) -> Self:
+        """
+        Pipe function call.
+
+        Examples:
+            >>> import polars as pl
+            >>> import pandas as pd
+            >>> import narwhals as nw
+            >>> data = {'a': [1,2,3], 'ba': [4,5,6]}
+            >>> df_pd = pd.DataFrame(data)
+            >>> df_pl = pl.DataFrame(data)
+
+            Let's define a dataframe-agnostic function:
+
+            >>> def func(df_any):
+            ...     df = nw.from_native(df_any)
+            ...     df = df.pipe(lambda _df: _df.select([x for x in _df.columns if len(x) == 1]))
+            ...     return nw.to_native(df)
+
+            We can then pass either pandas or Polars:
+
+            >>> func(df_pd)
+               a
+            0  1
+            1  2
+            2  3
+            >>> func(df_pl)
+            shape: (3, 1)
+            ┌─────┐
+            │ a   │
+            │ --- │
+            │ i64 │
+            ╞═════╡
+            │ 1   │
+            │ 2   │
+            │ 3   │
+            └─────┘
+        """
+        return super().pipe(function, *args, **kwargs)
+
     @property
     def schema(self) -> dict[str, DType]:
         r"""
         Get a dict[column name, DataType].
 
         Examples:
             >>> import polars as pl
@@ -1338,14 +1382,54 @@
             └─────┴─────┴─────┘
         """
         return DataFrame(
             self._dataframe.collect(),
         )
 
     # inherited
+    def pipe(self, function: Callable[[Any], Self], *args: Any, **kwargs: Any) -> Self:
+        """
+        Pipe function call.
+
+        Examples:
+            >>> import polars as pl
+            >>> import pandas as pd
+            >>> import narwhals as nw
+            >>> data = {'a': [1,2,3], 'ba': [4,5,6]}
+            >>> df_pd = pd.DataFrame(data)
+            >>> df_pl = pl.LazyFrame(data)
+
+            Let's define a dataframe-agnostic function:
+
+            >>> def func(df_any):
+            ...     df = nw.from_native(df_any)
+            ...     df = df.pipe(lambda _df: _df.select([x for x in _df.columns if len(x) == 1]))
+            ...     return nw.to_native(df)
+
+            We can then pass either pandas or Polars:
+
+            >>> func(df_pd)
+               a
+            0  1
+            1  2
+            2  3
+            >>> func(df_pl).collect()
+            shape: (3, 1)
+            ┌─────┐
+            │ a   │
+            │ --- │
+            │ i64 │
+            ╞═════╡
+            │ 1   │
+            │ 2   │
+            │ 3   │
+            └─────┘
+        """
+        return super().pipe(function, *args, **kwargs)
+
     @property
     def schema(self) -> dict[str, DType]:
         r"""
         Get a dict[column name, DType].
 
         Examples:
             >>> import polars as pl
```

### Comparing `narwhals-0.8.3/narwhals/dependencies.py` & `narwhals-0.8.4/narwhals/dependencies.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.3/narwhals/dtypes.py` & `narwhals-0.8.4/narwhals/dtypes.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.3/narwhals/expression.py` & `narwhals-0.8.4/narwhals/expression.py`

 * *Files 1% similar despite different names*

```diff
@@ -760,14 +760,58 @@
             │ 5   ┆ 5.0 │
             └─────┴─────┘
         """
         return self.__class__(lambda plx: self._call(plx).fill_null(value))
 
     # --- partial reduction ---
     def drop_nulls(self) -> Expr:
+        """
+        Remove missing values.
+
+        Notes:
+            pandas and Polars handle null values differently. Polars distinguishes
+            between NaN and Null, whereas pandas doesn't.
+
+        Examples:
+            >>> import narwhals as nw
+            >>> import pandas as pd
+            >>> import polars as pl
+
+            >>> df_pd = pd.DataFrame({"a": [2.0, 4.0, float("nan"), 3.0, None, 5.0]})
+            >>> df_pl = pl.DataFrame({"a": [2.0, 4.0, float("nan"), 3.0, None, 5.0]})
+
+            Let's define a dataframe-agnostic function:
+
+            >>> def func(df_any):
+            ...     df = nw.from_native(df_any)
+            ...     df = df.select(nw.col("a").drop_nulls())
+            ...     return nw.to_native(df)
+
+            We can then pass either pandas or Polars to `func`:
+
+            >>> func(df_pd)
+                 a
+            0  2.0
+            1  4.0
+            3  3.0
+            5  5.0
+            >>> func(df_pl)  # nan != null for polars
+            shape: (5, 1)
+            ┌─────┐
+            │ a   │
+            │ --- │
+            │ f64 │
+            ╞═════╡
+            │ 2.0 │
+            │ 4.0 │
+            │ NaN │
+            │ 3.0 │
+            │ 5.0 │
+            └─────┘
+        """
         return self.__class__(lambda plx: self._call(plx).drop_nulls())
 
     def sample(
         self,
         n: int | None = None,
         fraction: float | None = None,
         *,
```

### Comparing `narwhals-0.8.3/narwhals/functions.py` & `narwhals-0.8.4/narwhals/functions.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.3/narwhals/group_by.py` & `narwhals-0.8.4/narwhals/group_by.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.3/narwhals/series.py` & `narwhals-0.8.4/narwhals/series.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.3/narwhals/translate.py` & `narwhals-0.8.4/narwhals/translate.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.3/narwhals/typing.py` & `narwhals-0.8.4/narwhals/typing.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.3/narwhals/utils.py` & `narwhals-0.8.4/narwhals/utils.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.3/narwhals/_pandas_like/dataframe.py` & `narwhals-0.8.4/narwhals/_pandas_like/dataframe.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.3/narwhals/_pandas_like/expr.py` & `narwhals-0.8.4/narwhals/_pandas_like/expr.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.3/narwhals/_pandas_like/group_by.py` & `narwhals-0.8.4/narwhals/_pandas_like/group_by.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.3/narwhals/_pandas_like/namespace.py` & `narwhals-0.8.4/narwhals/_pandas_like/namespace.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.3/narwhals/_pandas_like/series.py` & `narwhals-0.8.4/narwhals/_pandas_like/series.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.3/narwhals/_pandas_like/typing.py` & `narwhals-0.8.4/narwhals/_pandas_like/typing.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.3/narwhals/_pandas_like/utils.py` & `narwhals-0.8.4/narwhals/_pandas_like/utils.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.3/tests/conftest.py` & `narwhals-0.8.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.3/tests/test_common.py` & `narwhals-0.8.4/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.3/tests/test_dt.py` & `narwhals-0.8.4/tests/test_dt.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.3/tests/test_group_by.py` & `narwhals-0.8.4/tests/test_group_by.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.3/tests/test_series.py` & `narwhals-0.8.4/tests/test_series.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.3/tests/test_str.py` & `narwhals-0.8.4/tests/test_str.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.3/tests/tpch_q1_test.py` & `narwhals-0.8.4/tests/tpch_q1_test.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.3/tests/utils.py` & `narwhals-0.8.4/tests/utils.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.3/tests/data/customer.parquet` & `narwhals-0.8.4/tests/data/customer.parquet`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.3/tests/data/lineitem.parquet` & `narwhals-0.8.4/tests/data/lineitem.parquet`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.3/tests/data/nation.parquet` & `narwhals-0.8.4/tests/data/nation.parquet`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.3/tests/data/orders.parquet` & `narwhals-0.8.4/tests/data/orders.parquet`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.3/tests/data/part.parquet` & `narwhals-0.8.4/tests/data/part.parquet`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.3/tests/data/partsupp.parquet` & `narwhals-0.8.4/tests/data/partsupp.parquet`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.3/tests/data/region.parquet` & `narwhals-0.8.4/tests/data/region.parquet`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.3/tests/data/supplier.parquet` & `narwhals-0.8.4/tests/data/supplier.parquet`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.3/tests/expr/cum_sum_test.py` & `narwhals-0.8.4/tests/expr/cum_sum_test.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.3/tests/expr/diff_test.py` & `narwhals-0.8.4/tests/expr/diff_test.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.3/tests/expr/fill_null_test.py` & `narwhals-0.8.4/tests/expr/fill_null_test.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.3/tests/expr/over_test.py` & `narwhals-0.8.4/tests/expr/over_test.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.3/tests/expr/str/head_test.py` & `narwhals-0.8.4/tests/expr/str/head_test.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.3/tests/expr/str/to_datetime_test.py` & `narwhals-0.8.4/tests/expr/str/to_datetime_test.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.3/tests/hypothesis/test_basic_arithmetic.py` & `narwhals-0.8.4/tests/hypothesis/test_basic_arithmetic.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.3/tests/hypothesis/test_concat.py` & `narwhals-0.8.4/tests/hypothesis/test_concat.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.3/tests/hypothesis/test_join.py` & `narwhals-0.8.4/tests/hypothesis/test_join.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.3/tpch/q1.py` & `narwhals-0.8.4/tpch/q1.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.3/tpch/q2.py` & `narwhals-0.8.4/tpch/q2.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.3/tpch/q3.py` & `narwhals-0.8.4/tpch/q3.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.3/tpch/q4.py` & `narwhals-0.8.4/tpch/q4.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.3/tpch/q5.py` & `narwhals-0.8.4/tpch/q5.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.3/tpch/notebooks/gpu/execute.ipynb` & `narwhals-0.8.4/tpch/notebooks/gpu/execute.ipynb`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.3/tpch/notebooks/q1/execute.ipynb` & `narwhals-0.8.4/tpch/notebooks/q1/execute.ipynb`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.3/tpch/notebooks/q2/execute.ipynb` & `narwhals-0.8.4/tpch/notebooks/q2/execute.ipynb`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.3/tpch/notebooks/q3/execute.ipynb` & `narwhals-0.8.4/tpch/notebooks/q3/execute.ipynb`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.3/tpch/notebooks/q4/execute.ipynb` & `narwhals-0.8.4/tpch/notebooks/q4/execute.ipynb`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.3/tpch/notebooks/q5/execute.ipynb` & `narwhals-0.8.4/tpch/notebooks/q5/execute.ipynb`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.3/tpch/notebooks/q6/execute.ipynb` & `narwhals-0.8.4/tpch/notebooks/q6/execute.ipynb`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.3/tpch/notebooks/q7/execute.ipynb` & `narwhals-0.8.4/tpch/notebooks/q7/execute.ipynb`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.3/tpch/notebooks/q8/execute.ipynb` & `narwhals-0.8.4/tpch/notebooks/q8/execute.ipynb`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.3/utils/bump_version.py` & `narwhals-0.8.4/utils/bump_version.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.3/utils/check_api_reference.py` & `narwhals-0.8.4/utils/check_api_reference.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.3/LICENSE.md` & `narwhals-0.8.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.3/README.md` & `narwhals-0.8.4/README.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.3/pyproject.toml` & `narwhals-0.8.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "narwhals"
-version = "0.8.3"
+version = "0.8.4"
 authors = [
   { name="Marco Gorelli", email="33491632+MarcoGorelli@users.noreply.github.com" },
 ]
 description = "Extremely lightweight compatibility layer between pandas, Polars, cuDF, and Modin"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `narwhals-0.8.3/PKG-INFO` & `narwhals-0.8.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: narwhals
-Version: 0.8.3
+Version: 0.8.4
 Summary: Extremely lightweight compatibility layer between pandas, Polars, cuDF, and Modin
 Project-URL: Homepage, https://github.com/MarcoGorelli/narwhals
 Project-URL: Bug Tracker, https://github.com/MarcoGorelli/narwhals
 Author-email: Marco Gorelli <33491632+MarcoGorelli@users.noreply.github.com>
 License-File: LICENSE.md
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

