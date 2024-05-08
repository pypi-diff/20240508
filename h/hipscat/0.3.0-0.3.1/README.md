# Comparing `tmp/hipscat-0.3.0.tar.gz` & `tmp/hipscat-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hipscat-0.3.0.tar", last modified: Mon Apr 22 15:52:16 2024, max compression
+gzip compressed data, was "hipscat-0.3.1.tar", last modified: Wed May  8 17:53:53 2024, max compression
```

## Comparing `hipscat-0.3.0.tar` & `hipscat-0.3.1.tar`

### file list

```diff
@@ -1,303 +1,304 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:52:16.493958 hipscat-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-04-22 15:52:10.000000 hipscat-0.3.0/.copier-answers.yml
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-22 15:52:10.000000 hipscat-0.3.0/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-22 15:52:10.000000 hipscat-0.3.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:52:16.441958 hipscat-0.3.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:52:16.445958 hipscat-0.3.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-22 15:52:10.000000 hipscat-0.3.0/.github/ISSUE_TEMPLATE/0-general_issue.md
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-22 15:52:10.000000 hipscat-0.3.0/.github/ISSUE_TEMPLATE/1-bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-04-22 15:52:10.000000 hipscat-0.3.0/.github/ISSUE_TEMPLATE/2-feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-22 15:52:10.000000 hipscat-0.3.0/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-04-22 15:52:10.000000 hipscat-0.3.0/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:52:16.445958 hipscat-0.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-22 15:52:10.000000 hipscat-0.3.0/.github/workflows/add-issue-to-project-tracker.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2697 2024-04-22 15:52:10.000000 hipscat-0.3.0/.github/workflows/asv-main.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-04-22 15:52:10.000000 hipscat-0.3.0/.github/workflows/asv-nightly.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3057 2024-04-22 15:52:10.000000 hipscat-0.3.0/.github/workflows/asv-pr.yml
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-22 15:52:10.000000 hipscat-0.3.0/.github/workflows/build-documentation.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-22 15:52:10.000000 hipscat-0.3.0/.github/workflows/pre-commit-ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-04-22 15:52:10.000000 hipscat-0.3.0/.github/workflows/publish-benchmarks-pr.yml
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-04-22 15:52:10.000000 hipscat-0.3.0/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-04-22 15:52:10.000000 hipscat-0.3.0/.github/workflows/smoke-test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-22 15:52:10.000000 hipscat-0.3.0/.github/workflows/testing-and-coverage.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-04-22 15:52:10.000000 hipscat-0.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     5366 2024-04-22 15:52:10.000000 hipscat-0.3.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-22 15:52:10.000000 hipscat-0.3.0/.prepare_project.sh
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-22 15:52:10.000000 hipscat-0.3.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-04-22 15:52:10.000000 hipscat-0.3.0/.setup_dev.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-04-22 15:52:10.000000 hipscat-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5917 2024-04-22 15:52:16.493958 hipscat-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2860 2024-04-22 15:52:10.000000 hipscat-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:52:16.445958 hipscat-0.3.0/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 15:52:10.000000 hipscat-0.3.0/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3597 2024-04-22 15:52:10.000000 hipscat-0.3.0/benchmarks/asv.conf.json
--rw-r--r--   0 runner    (1001) docker     (127)     5000 2024-04-22 15:52:10.000000 hipscat-0.3.0/benchmarks/benchmarks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:52:16.445958 hipscat-0.3.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-04-22 15:52:10.000000 hipscat-0.3.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:52:16.445958 hipscat-0.3.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-22 15:52:10.000000 hipscat-0.3.0/docs/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-04-22 15:52:10.000000 hipscat-0.3.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:52:16.449958 hipscat-0.3.0/docs/guide/
--rw-r--r--   0 runner    (1001) docker     (127)     4409 2024-04-22 15:52:10.000000 hipscat-0.3.0/docs/guide/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-22 15:52:10.000000 hipscat-0.3.0/docs/guide/directory_scheme.rst
--rw-r--r--   0 runner    (1001) docker     (127)    17649 2024-04-22 15:52:10.000000 hipscat-0.3.0/docs/guide/margin_cache_diagram.png
--rw-r--r--   0 runner    (1001) docker     (127)    12890 2024-04-22 15:52:10.000000 hipscat-0.3.0/docs/guide/pixel_math.md
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-22 15:52:10.000000 hipscat-0.3.0/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:52:16.449958 hipscat-0.3.0/docs/notebooks/
--rw-r--r--   0 runner    (1001) docker     (127)     4988 2024-04-22 15:52:10.000000 hipscat-0.3.0/docs/notebooks/catalog_size_inspection.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-04-22 15:52:10.000000 hipscat-0.3.0/docs/notebooks/cone_search.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-22 15:52:10.000000 hipscat-0.3.0/docs/notebooks.rst
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-22 15:52:10.000000 hipscat-0.3.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2797 2024-04-22 15:52:10.000000 hipscat-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 15:52:16.493958 hipscat-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:52:16.449958 hipscat-0.3.0/src/
--rw-r--r--   0 runner    (1001) docker     (127)    20811 2024-04-22 15:52:10.000000 hipscat-0.3.0/src/.pylintrc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:52:16.449958 hipscat-0.3.0/src/hipscat/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-22 15:52:10.000000 hipscat-0.3.0/src/hipscat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-22 15:52:16.000000 hipscat-0.3.0/src/hipscat/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:52:16.449958 hipscat-0.3.0/src/hipscat/catalog/
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-22 15:52:10.000000 hipscat-0.3.0/src/hipscat/catalog/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:52:16.453958 hipscat-0.3.0/src/hipscat/catalog/association_catalog/
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-22 15:52:10.000000 hipscat-0.3.0/src/hipscat/catalog/association_catalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3784 2024-04-22 15:52:10.000000 hipscat-0.3.0/src/hipscat/catalog/association_catalog/association_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-04-22 15:52:10.000000 hipscat-0.3.0/src/hipscat/catalog/association_catalog/association_catalog_info.py
--rw-r--r--   0 runner    (1001) docker     (127)    13211 2024-04-22 15:52:10.000000 hipscat-0.3.0/src/hipscat/catalog/association_catalog/partition_join_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     5834 2024-04-22 15:52:10.000000 hipscat-0.3.0/src/hipscat/catalog/catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-22 15:52:10.000000 hipscat-0.3.0/src/hipscat/catalog/catalog_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-22 15:52:10.000000 hipscat-0.3.0/src/hipscat/catalog/catalog_type.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:52:16.453958 hipscat-0.3.0/src/hipscat/catalog/dataset/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-22 15:52:10.000000 hipscat-0.3.0/src/hipscat/catalog/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-04-22 15:52:10.000000 hipscat-0.3.0/src/hipscat/catalog/dataset/base_catalog_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-04-22 15:52:10.000000 hipscat-0.3.0/src/hipscat/catalog/dataset/catalog_info_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     3512 2024-04-22 15:52:10.000000 hipscat-0.3.0/src/hipscat/catalog/dataset/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:52:16.453958 hipscat-0.3.0/src/hipscat/catalog/healpix_dataset/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 15:52:10.000000 hipscat-0.3.0/src/hipscat/catalog/healpix_dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4923 2024-04-22 15:52:10.000000 hipscat-0.3.0/src/hipscat/catalog/healpix_dataset/healpix_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:52:16.453958 hipscat-0.3.0/src/hipscat/catalog/index/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-22 15:52:10.000000 hipscat-0.3.0/src/hipscat/catalog/index/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-04-22 15:52:10.000000 hipscat-0.3.0/src/hipscat/catalog/index/index_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-22 15:52:10.000000 hipscat-0.3.0/src/hipscat/catalog/index/index_catalog_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:52:16.453958 hipscat-0.3.0/src/hipscat/catalog/margin_cache/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-22 15:52:10.000000 hipscat-0.3.0/src/hipscat/catalog/margin_cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-22 15:52:10.000000 hipscat-0.3.0/src/hipscat/catalog/margin_cache/margin_cache_catalog_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-04-22 15:52:10.000000 hipscat-0.3.0/src/hipscat/catalog/margin_cache/margin_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)    11819 2024-04-22 15:52:10.000000 hipscat-0.3.0/src/hipscat/catalog/partition_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:52:16.453958 hipscat-0.3.0/src/hipscat/catalog/source_catalog/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-22 15:52:10.000000 hipscat-0.3.0/src/hipscat/catalog/source_catalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      906 2024-04-22 15:52:10.000000 hipscat-0.3.0/src/hipscat/catalog/source_catalog/source_catalog_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:52:16.453958 hipscat-0.3.0/src/hipscat/inspection/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-22 15:52:10.000000 hipscat-0.3.0/src/hipscat/inspection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11751 2024-04-22 15:52:10.000000 hipscat-0.3.0/src/hipscat/inspection/almanac.py
--rw-r--r--   0 runner    (1001) docker     (127)     5457 2024-04-22 15:52:10.000000 hipscat-0.3.0/src/hipscat/inspection/almanac_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     5423 2024-04-22 15:52:10.000000 hipscat-0.3.0/src/hipscat/inspection/visualize_catalog.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:52:16.457958 hipscat-0.3.0/src/hipscat/io/
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-22 15:52:10.000000 hipscat-0.3.0/src/hipscat/io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:52:16.457958 hipscat-0.3.0/src/hipscat/io/file_io/
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-22 15:52:10.000000 hipscat-0.3.0/src/hipscat/io/file_io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12699 2024-04-22 15:52:10.000000 hipscat-0.3.0/src/hipscat/io/file_io/file_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     8211 2024-04-22 15:52:10.000000 hipscat-0.3.0/src/hipscat/io/file_io/file_pointer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7498 2024-04-22 15:52:10.000000 hipscat-0.3.0/src/hipscat/io/parquet_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     9634 2024-04-22 15:52:10.000000 hipscat-0.3.0/src/hipscat/io/paths.py
--rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-04-22 15:52:10.000000 hipscat-0.3.0/src/hipscat/io/validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5733 2024-04-22 15:52:10.000000 hipscat-0.3.0/src/hipscat/io/write_metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:52:16.457958 hipscat-0.3.0/src/hipscat/loaders/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-22 15:52:10.000000 hipscat-0.3.0/src/hipscat/loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-04-22 15:52:10.000000 hipscat-0.3.0/src/hipscat/loaders/read_from_hipscat.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:52:16.457958 hipscat-0.3.0/src/hipscat/pixel_math/
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-22 15:52:10.000000 hipscat-0.3.0/src/hipscat/pixel_math/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5614 2024-04-22 15:52:10.000000 hipscat-0.3.0/src/hipscat/pixel_math/box_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-04-22 15:52:10.000000 hipscat-0.3.0/src/hipscat/pixel_math/cone_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-04-22 15:52:10.000000 hipscat-0.3.0/src/hipscat/pixel_math/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4979 2024-04-22 15:52:10.000000 hipscat-0.3.0/src/hipscat/pixel_math/healpix_pixel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-04-22 15:52:10.000000 hipscat-0.3.0/src/hipscat/pixel_math/healpix_pixel_convertor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-04-22 15:52:10.000000 hipscat-0.3.0/src/hipscat/pixel_math/healpix_pixel_function.py
--rw-r--r--   0 runner    (1001) docker     (127)     4311 2024-04-22 15:52:10.000000 hipscat-0.3.0/src/hipscat/pixel_math/hipscat_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     5651 2024-04-22 15:52:10.000000 hipscat-0.3.0/src/hipscat/pixel_math/margin_bounding.py
--rw-r--r--   0 runner    (1001) docker     (127)    12354 2024-04-22 15:52:10.000000 hipscat-0.3.0/src/hipscat/pixel_math/partition_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     4807 2024-04-22 15:52:10.000000 hipscat-0.3.0/src/hipscat/pixel_math/pixel_margins.py
--rw-r--r--   0 runner    (1001) docker     (127)     2016 2024-04-22 15:52:10.000000 hipscat-0.3.0/src/hipscat/pixel_math/polygon_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4185 2024-04-22 15:52:10.000000 hipscat-0.3.0/src/hipscat/pixel_math/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:52:16.461958 hipscat-0.3.0/src/hipscat/pixel_tree/
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-22 15:52:10.000000 hipscat-0.3.0/src/hipscat/pixel_tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-22 15:52:10.000000 hipscat-0.3.0/src/hipscat/pixel_tree/negative_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)    16600 2024-04-22 15:52:10.000000 hipscat-0.3.0/src/hipscat/pixel_tree/pixel_alignment.py
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-22 15:52:10.000000 hipscat-0.3.0/src/hipscat/pixel_tree/pixel_alignment_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     4162 2024-04-22 15:52:10.000000 hipscat-0.3.0/src/hipscat/pixel_tree/pixel_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-22 15:52:10.000000 hipscat-0.3.0/src/hipscat/pixel_tree/pixel_tree_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 15:52:10.000000 hipscat-0.3.0/src/hipscat/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:52:16.489958 hipscat-0.3.0/src/hipscat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5917 2024-04-22 15:52:16.000000 hipscat-0.3.0/src/hipscat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10039 2024-04-22 15:52:16.000000 hipscat-0.3.0/src/hipscat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 15:52:16.000000 hipscat-0.3.0/src/hipscat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-22 15:52:16.000000 hipscat-0.3.0/src/hipscat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-22 15:52:16.000000 hipscat-0.3.0/src/hipscat.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:52:16.461958 hipscat-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    20972 2024-04-22 15:52:10.000000 hipscat-0.3.0/tests/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)     8358 2024-04-22 15:52:10.000000 hipscat-0.3.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:52:16.461958 hipscat-0.3.0/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:52:16.461958 hipscat-0.3.0/tests/data/almanac/
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-22 15:52:10.000000 hipscat-0.3.0/tests/data/almanac/deprecated.yml
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-22 15:52:10.000000 hipscat-0.3.0/tests/data/almanac/small_sky.yml
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-22 15:52:10.000000 hipscat-0.3.0/tests/data/almanac/small_sky_order1.yml
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-22 15:52:10.000000 hipscat-0.3.0/tests/data/almanac/small_sky_order1_id_index.yml
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-22 15:52:10.000000 hipscat-0.3.0/tests/data/almanac/small_sky_order1_margin.yml
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-22 15:52:10.000000 hipscat-0.3.0/tests/data/almanac/small_sky_source.yml
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-22 15:52:10.000000 hipscat-0.3.0/tests/data/almanac/small_sky_source_object_index.yml
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-22 15:52:10.000000 hipscat-0.3.0/tests/data/almanac/small_sky_to_small_sky_order1.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:52:16.465958 hipscat-0.3.0/tests/data/almanac_exception/
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-22 15:52:10.000000 hipscat-0.3.0/tests/data/almanac_exception/association_missing_join.yml
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-22 15:52:10.000000 hipscat-0.3.0/tests/data/almanac_exception/association_missing_primary.yml
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-22 15:52:10.000000 hipscat-0.3.0/tests/data/almanac_exception/bad_catalog_path.yml
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-22 15:52:10.000000 hipscat-0.3.0/tests/data/almanac_exception/bad_primary_path.yml
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-22 15:52:10.000000 hipscat-0.3.0/tests/data/almanac_exception/bad_type.yml
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-22 15:52:10.000000 hipscat-0.3.0/tests/data/almanac_exception/index_missing_primary.yml
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-22 15:52:10.000000 hipscat-0.3.0/tests/data/almanac_exception/margin_missing_primary.yml
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-22 15:52:10.000000 hipscat-0.3.0/tests/data/almanac_exception/standalone_source_catalog.yml
--rw-r--r--   0 runner    (1001) docker     (127)    10017 2024-04-22 15:52:10.000000 hipscat-0.3.0/tests/data/generate_data.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:52:16.437958 hipscat-0.3.0/tests/data/info_only/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:52:16.465958 hipscat-0.3.0/tests/data/info_only/catalog/
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-22 15:52:10.000000 hipscat-0.3.0/tests/data/info_only/catalog/catalog_info.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:52:16.465958 hipscat-0.3.0/tests/data/info_only/dataset/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-22 15:52:10.000000 hipscat-0.3.0/tests/data/info_only/dataset/catalog_info.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:52:16.465958 hipscat-0.3.0/tests/data/info_only/index_catalog/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-22 15:52:10.000000 hipscat-0.3.0/tests/data/info_only/index_catalog/catalog_info.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:52:16.465958 hipscat-0.3.0/tests/data/info_only/margin_cache/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-22 15:52:10.000000 hipscat-0.3.0/tests/data/info_only/margin_cache/catalog_info.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:52:16.469958 hipscat-0.3.0/tests/data/small_sky/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:52:16.437958 hipscat-0.3.0/tests/data/small_sky/Norder=0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:52:16.469958 hipscat-0.3.0/tests/data/small_sky/Norder=0/Dir=0/
--rw-r--r--   0 runner    (1001) docker     (127)     8880 2024-04-22 15:52:10.000000 hipscat-0.3.0/tests/data/small_sky/Norder=0/Dir=0/Npix=11.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-04-22 15:52:10.000000 hipscat-0.3.0/tests/data/small_sky/_common_metadata
--rw-r--r--   0 runner    (1001) docker     (127)     5130 2024-04-22 15:52:10.000000 hipscat-0.3.0/tests/data/small_sky/_metadata
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-22 15:52:10.000000 hipscat-0.3.0/tests/data/small_sky/catalog_info.json
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-22 15:52:10.000000 hipscat-0.3.0/tests/data/small_sky/partition_info.csv
--rw-r--r--   0 runner    (1001) docker     (127)  1581120 2024-04-22 15:52:10.000000 hipscat-0.3.0/tests/data/small_sky/point_map.fits
--rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-04-22 15:52:10.000000 hipscat-0.3.0/tests/data/small_sky/provenance_info.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:52:16.469958 hipscat-0.3.0/tests/data/small_sky_order1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:52:16.437958 hipscat-0.3.0/tests/data/small_sky_order1/Norder=1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:52:16.469958 hipscat-0.3.0/tests/data/small_sky_order1/Norder=1/Dir=0/
--rw-r--r--   0 runner    (1001) docker     (127)     7210 2024-04-22 15:52:10.000000 hipscat-0.3.0/tests/data/small_sky_order1/Norder=1/Dir=0/Npix=44.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     6973 2024-04-22 15:52:10.000000 hipscat-0.3.0/tests/data/small_sky_order1/Norder=1/Dir=0/Npix=45.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     7216 2024-04-22 15:52:10.000000 hipscat-0.3.0/tests/data/small_sky_order1/Norder=1/Dir=0/Npix=46.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     6741 2024-04-22 15:52:10.000000 hipscat-0.3.0/tests/data/small_sky_order1/Norder=1/Dir=0/Npix=47.parquet
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-04-22 15:52:10.000000 hipscat-0.3.0/tests/data/small_sky_order1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-04-22 15:52:10.000000 hipscat-0.3.0/tests/data/small_sky_order1/_common_metadata
--rw-r--r--   0 runner    (1001) docker     (127)     8423 2024-04-22 15:52:10.000000 hipscat-0.3.0/tests/data/small_sky_order1/_metadata
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-22 15:52:10.000000 hipscat-0.3.0/tests/data/small_sky_order1/catalog_info.json
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-22 15:52:10.000000 hipscat-0.3.0/tests/data/small_sky_order1/partition_info.csv
--rw-r--r--   0 runner    (1001) docker     (127)     8640 2024-04-22 15:52:10.000000 hipscat-0.3.0/tests/data/small_sky_order1/point_map.fits
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-04-22 15:52:10.000000 hipscat-0.3.0/tests/data/small_sky_order1/provenance_info.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:52:16.469958 hipscat-0.3.0/tests/data/small_sky_order1_id_index/
--rw-r--r--   0 runner    (1001) docker     (127)     2224 2024-04-22 15:52:10.000000 hipscat-0.3.0/tests/data/small_sky_order1_id_index/_common_metadata
--rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-04-22 15:52:10.000000 hipscat-0.3.0/tests/data/small_sky_order1_id_index/_metadata
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-22 15:52:10.000000 hipscat-0.3.0/tests/data/small_sky_order1_id_index/catalog_info.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:52:16.469958 hipscat-0.3.0/tests/data/small_sky_order1_id_index/index/
--rw-r--r--   0 runner    (1001) docker     (127)     3867 2024-04-22 15:52:10.000000 hipscat-0.3.0/tests/data/small_sky_order1_id_index/index/part.0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-22 15:52:10.000000 hipscat-0.3.0/tests/data/small_sky_order1_id_index/provenance_info.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:52:16.473958 hipscat-0.3.0/tests/data/small_sky_order1_margin/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:52:16.437958 hipscat-0.3.0/tests/data/small_sky_order1_margin/Norder=0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:52:16.473958 hipscat-0.3.0/tests/data/small_sky_order1_margin/Norder=0/Dir=0/
--rw-r--r--   0 runner    (1001) docker     (127)     8255 2024-04-22 15:52:10.000000 hipscat-0.3.0/tests/data/small_sky_order1_margin/Norder=0/Dir=0/Npix=4.parquet
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:52:16.437958 hipscat-0.3.0/tests/data/small_sky_order1_margin/Norder=1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:52:16.473958 hipscat-0.3.0/tests/data/small_sky_order1_margin/Norder=1/Dir=0/
--rw-r--r--   0 runner    (1001) docker     (127)     8434 2024-04-22 15:52:10.000000 hipscat-0.3.0/tests/data/small_sky_order1_margin/Norder=1/Dir=0/Npix=44.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     8476 2024-04-22 15:52:10.000000 hipscat-0.3.0/tests/data/small_sky_order1_margin/Norder=1/Dir=0/Npix=45.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     8378 2024-04-22 15:52:10.000000 hipscat-0.3.0/tests/data/small_sky_order1_margin/Norder=1/Dir=0/Npix=46.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     8344 2024-04-22 15:52:10.000000 hipscat-0.3.0/tests/data/small_sky_order1_margin/Norder=1/Dir=0/Npix=47.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-22 15:52:10.000000 hipscat-0.3.0/tests/data/small_sky_order1_margin/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     5194 2024-04-22 15:52:10.000000 hipscat-0.3.0/tests/data/small_sky_order1_margin/_common_metadata
--rw-r--r--   0 runner    (1001) docker     (127)    12384 2024-04-22 15:52:10.000000 hipscat-0.3.0/tests/data/small_sky_order1_margin/_metadata
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-22 15:52:10.000000 hipscat-0.3.0/tests/data/small_sky_order1_margin/catalog_info.json
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-22 15:52:10.000000 hipscat-0.3.0/tests/data/small_sky_order1_margin/partition_info.csv
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-04-22 15:52:10.000000 hipscat-0.3.0/tests/data/small_sky_order1_margin/provenance_info.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:52:16.477958 hipscat-0.3.0/tests/data/small_sky_source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:52:16.437958 hipscat-0.3.0/tests/data/small_sky_source/Norder=0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:52:16.477958 hipscat-0.3.0/tests/data/small_sky_source/Norder=0/Dir=0/
--rw-r--r--   0 runner    (1001) docker     (127)    11421 2024-04-22 15:52:10.000000 hipscat-0.3.0/tests/data/small_sky_source/Norder=0/Dir=0/Npix=4.parquet
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:52:16.437958 hipscat-0.3.0/tests/data/small_sky_source/Norder=1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:52:16.477958 hipscat-0.3.0/tests/data/small_sky_source/Norder=1/Dir=0/
--rw-r--r--   0 runner    (1001) docker     (127)   133671 2024-04-22 15:52:10.000000 hipscat-0.3.0/tests/data/small_sky_source/Norder=1/Dir=0/Npix=47.parquet
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:52:16.437958 hipscat-0.3.0/tests/data/small_sky_source/Norder=2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:52:16.481958 hipscat-0.3.0/tests/data/small_sky_source/Norder=2/Dir=0/
--rw-r--r--   0 runner    (1001) docker     (127)    28346 2024-04-22 15:52:10.000000 hipscat-0.3.0/tests/data/small_sky_source/Norder=2/Dir=0/Npix=176.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    86262 2024-04-22 15:52:10.000000 hipscat-0.3.0/tests/data/small_sky_source/Norder=2/Dir=0/Npix=177.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    92634 2024-04-22 15:52:10.000000 hipscat-0.3.0/tests/data/small_sky_source/Norder=2/Dir=0/Npix=178.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    99874 2024-04-22 15:52:10.000000 hipscat-0.3.0/tests/data/small_sky_source/Norder=2/Dir=0/Npix=179.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    42177 2024-04-22 15:52:10.000000 hipscat-0.3.0/tests/data/small_sky_source/Norder=2/Dir=0/Npix=180.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    54742 2024-04-22 15:52:10.000000 hipscat-0.3.0/tests/data/small_sky_source/Norder=2/Dir=0/Npix=181.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    72960 2024-04-22 15:52:10.000000 hipscat-0.3.0/tests/data/small_sky_source/Norder=2/Dir=0/Npix=182.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    67771 2024-04-22 15:52:10.000000 hipscat-0.3.0/tests/data/small_sky_source/Norder=2/Dir=0/Npix=183.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    80265 2024-04-22 15:52:10.000000 hipscat-0.3.0/tests/data/small_sky_source/Norder=2/Dir=0/Npix=184.parquet
--rw-r--r--   0 runner    (1001) docker     (127)   162064 2024-04-22 15:52:10.000000 hipscat-0.3.0/tests/data/small_sky_source/Norder=2/Dir=0/Npix=185.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    31761 2024-04-22 15:52:10.000000 hipscat-0.3.0/tests/data/small_sky_source/Norder=2/Dir=0/Npix=186.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    43705 2024-04-22 15:52:10.000000 hipscat-0.3.0/tests/data/small_sky_source/Norder=2/Dir=0/Npix=187.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     5525 2024-04-22 15:52:10.000000 hipscat-0.3.0/tests/data/small_sky_source/_common_metadata
--rw-r--r--   0 runner    (1001) docker     (127)    28968 2024-04-22 15:52:10.000000 hipscat-0.3.0/tests/data/small_sky_source/_metadata
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-22 15:52:10.000000 hipscat-0.3.0/tests/data/small_sky_source/catalog_info.json
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-22 15:52:10.000000 hipscat-0.3.0/tests/data/small_sky_source/partition_info.csv
--rw-r--r--   0 runner    (1001) docker     (127)  1581120 2024-04-22 15:52:10.000000 hipscat-0.3.0/tests/data/small_sky_source/point_map.fits
--rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-04-22 15:52:10.000000 hipscat-0.3.0/tests/data/small_sky_source/provenance_info.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:52:16.481958 hipscat-0.3.0/tests/data/small_sky_source_object_index/
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-22 15:52:10.000000 hipscat-0.3.0/tests/data/small_sky_source_object_index/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-04-22 15:52:10.000000 hipscat-0.3.0/tests/data/small_sky_source_object_index/_common_metadata
--rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-04-22 15:52:10.000000 hipscat-0.3.0/tests/data/small_sky_source_object_index/_metadata
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-22 15:52:10.000000 hipscat-0.3.0/tests/data/small_sky_source_object_index/catalog_info.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:52:16.481958 hipscat-0.3.0/tests/data/small_sky_source_object_index/index/
--rw-r--r--   0 runner    (1001) docker     (127)     4153 2024-04-22 15:52:10.000000 hipscat-0.3.0/tests/data/small_sky_source_object_index/index/part.0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-04-22 15:52:10.000000 hipscat-0.3.0/tests/data/small_sky_source_object_index/provenance_info.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:52:16.481958 hipscat-0.3.0/tests/data/small_sky_to_small_sky_order1/
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-22 15:52:10.000000 hipscat-0.3.0/tests/data/small_sky_to_small_sky_order1/_common_metadata
--rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-04-22 15:52:10.000000 hipscat-0.3.0/tests/data/small_sky_to_small_sky_order1/_metadata
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-22 15:52:10.000000 hipscat-0.3.0/tests/data/small_sky_to_small_sky_order1/catalog_info.json
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-22 15:52:10.000000 hipscat-0.3.0/tests/data/small_sky_to_small_sky_order1/partition_info.csv
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-22 15:52:10.000000 hipscat-0.3.0/tests/data/small_sky_to_small_sky_order1/partition_join_info.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:52:16.481958 hipscat-0.3.0/tests/hipscat/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:52:16.485958 hipscat-0.3.0/tests/hipscat/catalog/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:52:16.485958 hipscat-0.3.0/tests/hipscat/catalog/association_catalog/
--rw-r--r--   0 runner    (1001) docker     (127)     5552 2024-04-22 15:52:10.000000 hipscat-0.3.0/tests/hipscat/catalog/association_catalog/test_association_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     2627 2024-04-22 15:52:10.000000 hipscat-0.3.0/tests/hipscat/catalog/association_catalog/test_association_catalog_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     6156 2024-04-22 15:52:10.000000 hipscat-0.3.0/tests/hipscat/catalog/association_catalog/test_partition_join_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:52:16.485958 hipscat-0.3.0/tests/hipscat/catalog/dataset/
--rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-04-22 15:52:10.000000 hipscat-0.3.0/tests/hipscat/catalog/dataset/test_base_catalog_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     4896 2024-04-22 15:52:10.000000 hipscat-0.3.0/tests/hipscat/catalog/dataset/test_catalog_info_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-04-22 15:52:10.000000 hipscat-0.3.0/tests/hipscat/catalog/dataset/test_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:52:16.485958 hipscat-0.3.0/tests/hipscat/catalog/index/
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-22 15:52:10.000000 hipscat-0.3.0/tests/hipscat/catalog/index/test_index_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-04-22 15:52:10.000000 hipscat-0.3.0/tests/hipscat/catalog/index/test_index_catalog_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:52:16.485958 hipscat-0.3.0/tests/hipscat/catalog/loaders/
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-22 15:52:10.000000 hipscat-0.3.0/tests/hipscat/catalog/loaders/test_read_from_hipscat.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:52:16.485958 hipscat-0.3.0/tests/hipscat/catalog/margin_cache/
--rw-r--r--   0 runner    (1001) docker     (127)     2586 2024-04-22 15:52:10.000000 hipscat-0.3.0/tests/hipscat/catalog/margin_cache/test_margin_cache_catalog_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     3115 2024-04-22 15:52:10.000000 hipscat-0.3.0/tests/hipscat/catalog/margin_cache/test_margin_catalog.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:52:16.485958 hipscat-0.3.0/tests/hipscat/catalog/source_catalog/
--rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-04-22 15:52:10.000000 hipscat-0.3.0/tests/hipscat/catalog/source_catalog/test_source_catalog_info.py
--rw-r--r--   0 runner    (1001) docker     (127)    22026 2024-04-22 15:52:10.000000 hipscat-0.3.0/tests/hipscat/catalog/test_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-04-22 15:52:10.000000 hipscat-0.3.0/tests/hipscat/catalog/test_catalog_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     6742 2024-04-22 15:52:10.000000 hipscat-0.3.0/tests/hipscat/catalog/test_partition_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-04-22 15:52:10.000000 hipscat-0.3.0/tests/hipscat/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:52:16.485958 hipscat-0.3.0/tests/hipscat/inspection/
--rw-r--r--   0 runner    (1001) docker     (127)     7492 2024-04-22 15:52:10.000000 hipscat-0.3.0/tests/hipscat/inspection/test_almanac.py
--rw-r--r--   0 runner    (1001) docker     (127)     3550 2024-04-22 15:52:10.000000 hipscat-0.3.0/tests/hipscat/inspection/test_almanac_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2775 2024-04-22 15:52:10.000000 hipscat-0.3.0/tests/hipscat/inspection/test_visualize_catalog.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:52:16.489958 hipscat-0.3.0/tests/hipscat/io/
--rw-r--r--   0 runner    (1001) docker     (127)     3654 2024-04-22 15:52:10.000000 hipscat-0.3.0/tests/hipscat/io/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:52:16.489958 hipscat-0.3.0/tests/hipscat/io/file_io/
--rw-r--r--   0 runner    (1001) docker     (127)     4488 2024-04-22 15:52:10.000000 hipscat-0.3.0/tests/hipscat/io/file_io/test_file_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     5396 2024-04-22 15:52:10.000000 hipscat-0.3.0/tests/hipscat/io/file_io/test_file_pointers.py
--rw-r--r--   0 runner    (1001) docker     (127)     8508 2024-04-22 15:52:10.000000 hipscat-0.3.0/tests/hipscat/io/test_parquet_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-04-22 15:52:10.000000 hipscat-0.3.0/tests/hipscat/io/test_paths.py
--rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-04-22 15:52:10.000000 hipscat-0.3.0/tests/hipscat/io/test_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     7239 2024-04-22 15:52:10.000000 hipscat-0.3.0/tests/hipscat/io/test_write_metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:52:16.489958 hipscat-0.3.0/tests/hipscat/pixel_math/
--rw-r--r--   0 runner    (1001) docker     (127)     3203 2024-04-22 15:52:10.000000 hipscat-0.3.0/tests/hipscat/pixel_math/test_healpix_pixel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-22 15:52:10.000000 hipscat-0.3.0/tests/hipscat/pixel_math/test_healpix_pixel_convertor.py
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-22 15:52:10.000000 hipscat-0.3.0/tests/hipscat/pixel_math/test_healpix_pixel_function.py
--rw-r--r--   0 runner    (1001) docker     (127)     5361 2024-04-22 15:52:10.000000 hipscat-0.3.0/tests/hipscat/pixel_math/test_hipscat_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-04-22 15:52:10.000000 hipscat-0.3.0/tests/hipscat/pixel_math/test_margin_bounding.py
--rw-r--r--   0 runner    (1001) docker     (127)    10360 2024-04-22 15:52:10.000000 hipscat-0.3.0/tests/hipscat/pixel_math/test_partition_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     3789 2024-04-22 15:52:10.000000 hipscat-0.3.0/tests/hipscat/pixel_math/test_pixel_margins.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:52:16.489958 hipscat-0.3.0/tests/hipscat/pixel_tree/
--rw-r--r--   0 runner    (1001) docker     (127)     3418 2024-04-22 15:52:10.000000 hipscat-0.3.0/tests/hipscat/pixel_tree/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-04-22 15:52:10.000000 hipscat-0.3.0/tests/hipscat/pixel_tree/test_pixel_alignment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-04-22 15:52:10.000000 hipscat-0.3.0/tests/hipscat/pixel_tree/test_pixel_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-04-22 15:52:10.000000 hipscat-0.3.0/tests/hipscat/pixel_tree/test_pixel_tree_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.061213 hipscat-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-08 17:53:46.000000 hipscat-0.3.1/.copier-answers.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-08 17:53:46.000000 hipscat-0.3.1/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-08 17:53:46.000000 hipscat-0.3.1/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.017213 hipscat-0.3.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.017213 hipscat-0.3.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-08 17:53:46.000000 hipscat-0.3.1/.github/ISSUE_TEMPLATE/0-general_issue.md
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-08 17:53:46.000000 hipscat-0.3.1/.github/ISSUE_TEMPLATE/1-bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-05-08 17:53:46.000000 hipscat-0.3.1/.github/ISSUE_TEMPLATE/2-feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-08 17:53:46.000000 hipscat-0.3.1/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-05-08 17:53:46.000000 hipscat-0.3.1/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.021213 hipscat-0.3.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-08 17:53:46.000000 hipscat-0.3.1/.github/workflows/add-issue-to-project-tracker.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2697 2024-05-08 17:53:46.000000 hipscat-0.3.1/.github/workflows/asv-main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-05-08 17:53:46.000000 hipscat-0.3.1/.github/workflows/asv-nightly.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3057 2024-05-08 17:53:46.000000 hipscat-0.3.1/.github/workflows/asv-pr.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-05-08 17:53:46.000000 hipscat-0.3.1/.github/workflows/build-documentation.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-05-08 17:53:46.000000 hipscat-0.3.1/.github/workflows/pre-commit-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-05-08 17:53:46.000000 hipscat-0.3.1/.github/workflows/publish-benchmarks-pr.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-05-08 17:53:46.000000 hipscat-0.3.1/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-05-08 17:53:46.000000 hipscat-0.3.1/.github/workflows/smoke-test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-05-08 17:53:46.000000 hipscat-0.3.1/.github/workflows/testing-and-coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-05-08 17:53:46.000000 hipscat-0.3.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     5366 2024-05-08 17:53:46.000000 hipscat-0.3.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-08 17:53:46.000000 hipscat-0.3.1/.prepare_project.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-08 17:53:46.000000 hipscat-0.3.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-05-08 17:53:46.000000 hipscat-0.3.1/.setup_dev.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-05-08 17:53:46.000000 hipscat-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5939 2024-05-08 17:53:53.061213 hipscat-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2860 2024-05-08 17:53:46.000000 hipscat-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.021213 hipscat-0.3.1/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:46.000000 hipscat-0.3.1/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3597 2024-05-08 17:53:46.000000 hipscat-0.3.1/benchmarks/asv.conf.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4950 2024-05-08 17:53:46.000000 hipscat-0.3.1/benchmarks/benchmarks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.021213 hipscat-0.3.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-08 17:53:46.000000 hipscat-0.3.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.021213 hipscat-0.3.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-08 17:53:46.000000 hipscat-0.3.1/docs/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-05-08 17:53:46.000000 hipscat-0.3.1/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.021213 hipscat-0.3.1/docs/guide/
+-rw-r--r--   0 runner    (1001) docker     (127)     4409 2024-05-08 17:53:46.000000 hipscat-0.3.1/docs/guide/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-05-08 17:53:46.000000 hipscat-0.3.1/docs/guide/directory_scheme.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    17649 2024-05-08 17:53:46.000000 hipscat-0.3.1/docs/guide/margin_cache_diagram.png
+-rw-r--r--   0 runner    (1001) docker     (127)    12890 2024-05-08 17:53:46.000000 hipscat-0.3.1/docs/guide/pixel_math.md
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-08 17:53:46.000000 hipscat-0.3.1/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.021213 hipscat-0.3.1/docs/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)     4988 2024-05-08 17:53:46.000000 hipscat-0.3.1/docs/notebooks/catalog_size_inspection.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-05-08 17:53:46.000000 hipscat-0.3.1/docs/notebooks/cone_search.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-08 17:53:46.000000 hipscat-0.3.1/docs/notebooks.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-08 17:53:46.000000 hipscat-0.3.1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2811 2024-05-08 17:53:46.000000 hipscat-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 17:53:53.061213 hipscat-0.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.021213 hipscat-0.3.1/src/
+-rw-r--r--   0 runner    (1001) docker     (127)    20811 2024-05-08 17:53:46.000000 hipscat-0.3.1/src/.pylintrc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.021213 hipscat-0.3.1/src/hipscat/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-08 17:53:46.000000 hipscat-0.3.1/src/hipscat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-08 17:53:52.000000 hipscat-0.3.1/src/hipscat/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.025213 hipscat-0.3.1/src/hipscat/catalog/
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-08 17:53:46.000000 hipscat-0.3.1/src/hipscat/catalog/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.025213 hipscat-0.3.1/src/hipscat/catalog/association_catalog/
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-08 17:53:46.000000 hipscat-0.3.1/src/hipscat/catalog/association_catalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3883 2024-05-08 17:53:46.000000 hipscat-0.3.1/src/hipscat/catalog/association_catalog/association_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-05-08 17:53:46.000000 hipscat-0.3.1/src/hipscat/catalog/association_catalog/association_catalog_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13211 2024-05-08 17:53:46.000000 hipscat-0.3.1/src/hipscat/catalog/association_catalog/partition_join_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6029 2024-05-08 17:53:46.000000 hipscat-0.3.1/src/hipscat/catalog/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-08 17:53:46.000000 hipscat-0.3.1/src/hipscat/catalog/catalog_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-08 17:53:46.000000 hipscat-0.3.1/src/hipscat/catalog/catalog_type.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.025213 hipscat-0.3.1/src/hipscat/catalog/dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-08 17:53:46.000000 hipscat-0.3.1/src/hipscat/catalog/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-05-08 17:53:46.000000 hipscat-0.3.1/src/hipscat/catalog/dataset/base_catalog_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-05-08 17:53:46.000000 hipscat-0.3.1/src/hipscat/catalog/dataset/catalog_info_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3512 2024-05-08 17:53:46.000000 hipscat-0.3.1/src/hipscat/catalog/dataset/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.025213 hipscat-0.3.1/src/hipscat/catalog/healpix_dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:46.000000 hipscat-0.3.1/src/hipscat/catalog/healpix_dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8283 2024-05-08 17:53:46.000000 hipscat-0.3.1/src/hipscat/catalog/healpix_dataset/healpix_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.025213 hipscat-0.3.1/src/hipscat/catalog/index/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-08 17:53:46.000000 hipscat-0.3.1/src/hipscat/catalog/index/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-05-08 17:53:46.000000 hipscat-0.3.1/src/hipscat/catalog/index/index_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-08 17:53:46.000000 hipscat-0.3.1/src/hipscat/catalog/index/index_catalog_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.025213 hipscat-0.3.1/src/hipscat/catalog/margin_cache/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-08 17:53:46.000000 hipscat-0.3.1/src/hipscat/catalog/margin_cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-08 17:53:46.000000 hipscat-0.3.1/src/hipscat/catalog/margin_cache/margin_cache_catalog_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-05-08 17:53:46.000000 hipscat-0.3.1/src/hipscat/catalog/margin_cache/margin_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11819 2024-05-08 17:53:46.000000 hipscat-0.3.1/src/hipscat/catalog/partition_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.029213 hipscat-0.3.1/src/hipscat/catalog/source_catalog/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-08 17:53:46.000000 hipscat-0.3.1/src/hipscat/catalog/source_catalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      906 2024-05-08 17:53:46.000000 hipscat-0.3.1/src/hipscat/catalog/source_catalog/source_catalog_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.029213 hipscat-0.3.1/src/hipscat/inspection/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-08 17:53:46.000000 hipscat-0.3.1/src/hipscat/inspection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11751 2024-05-08 17:53:46.000000 hipscat-0.3.1/src/hipscat/inspection/almanac.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5457 2024-05-08 17:53:46.000000 hipscat-0.3.1/src/hipscat/inspection/almanac_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5462 2024-05-08 17:53:46.000000 hipscat-0.3.1/src/hipscat/inspection/visualize_catalog.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.029213 hipscat-0.3.1/src/hipscat/io/
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-05-08 17:53:46.000000 hipscat-0.3.1/src/hipscat/io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.029213 hipscat-0.3.1/src/hipscat/io/file_io/
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-08 17:53:46.000000 hipscat-0.3.1/src/hipscat/io/file_io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12699 2024-05-08 17:53:46.000000 hipscat-0.3.1/src/hipscat/io/file_io/file_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8215 2024-05-08 17:53:46.000000 hipscat-0.3.1/src/hipscat/io/file_io/file_pointer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7498 2024-05-08 17:53:46.000000 hipscat-0.3.1/src/hipscat/io/parquet_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9634 2024-05-08 17:53:46.000000 hipscat-0.3.1/src/hipscat/io/paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-05-08 17:53:46.000000 hipscat-0.3.1/src/hipscat/io/validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5733 2024-05-08 17:53:46.000000 hipscat-0.3.1/src/hipscat/io/write_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.029213 hipscat-0.3.1/src/hipscat/loaders/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-08 17:53:46.000000 hipscat-0.3.1/src/hipscat/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-05-08 17:53:46.000000 hipscat-0.3.1/src/hipscat/loaders/read_from_hipscat.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.033213 hipscat-0.3.1/src/hipscat/pixel_math/
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-05-08 17:53:46.000000 hipscat-0.3.1/src/hipscat/pixel_math/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5533 2024-05-08 17:53:46.000000 hipscat-0.3.1/src/hipscat/pixel_math/box_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-05-08 17:53:46.000000 hipscat-0.3.1/src/hipscat/pixel_math/cone_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-05-08 17:53:46.000000 hipscat-0.3.1/src/hipscat/pixel_math/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4979 2024-05-08 17:53:46.000000 hipscat-0.3.1/src/hipscat/pixel_math/healpix_pixel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-05-08 17:53:46.000000 hipscat-0.3.1/src/hipscat/pixel_math/healpix_pixel_convertor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-05-08 17:53:46.000000 hipscat-0.3.1/src/hipscat/pixel_math/healpix_pixel_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4311 2024-05-08 17:53:46.000000 hipscat-0.3.1/src/hipscat/pixel_math/hipscat_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5651 2024-05-08 17:53:46.000000 hipscat-0.3.1/src/hipscat/pixel_math/margin_bounding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12354 2024-05-08 17:53:46.000000 hipscat-0.3.1/src/hipscat/pixel_math/partition_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4807 2024-05-08 17:53:46.000000 hipscat-0.3.1/src/hipscat/pixel_math/pixel_margins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-05-08 17:53:46.000000 hipscat-0.3.1/src/hipscat/pixel_math/polygon_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4185 2024-05-08 17:53:46.000000 hipscat-0.3.1/src/hipscat/pixel_math/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.033213 hipscat-0.3.1/src/hipscat/pixel_tree/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-08 17:53:46.000000 hipscat-0.3.1/src/hipscat/pixel_tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-05-08 17:53:46.000000 hipscat-0.3.1/src/hipscat/pixel_tree/moc_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-08 17:53:46.000000 hipscat-0.3.1/src/hipscat/pixel_tree/negative_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19339 2024-05-08 17:53:46.000000 hipscat-0.3.1/src/hipscat/pixel_tree/pixel_alignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-08 17:53:46.000000 hipscat-0.3.1/src/hipscat/pixel_tree/pixel_alignment_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4367 2024-05-08 17:53:46.000000 hipscat-0.3.1/src/hipscat/pixel_tree/pixel_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:46.000000 hipscat-0.3.1/src/hipscat/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.057213 hipscat-0.3.1/src/hipscat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5939 2024-05-08 17:53:52.000000 hipscat-0.3.1/src/hipscat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10075 2024-05-08 17:53:53.000000 hipscat-0.3.1/src/hipscat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 17:53:52.000000 hipscat-0.3.1/src/hipscat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-08 17:53:52.000000 hipscat-0.3.1/src/hipscat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-08 17:53:52.000000 hipscat-0.3.1/src/hipscat.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.033213 hipscat-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    20972 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)     8358 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.033213 hipscat-0.3.1/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.033213 hipscat-0.3.1/tests/data/almanac/
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/almanac/deprecated.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/almanac/small_sky.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/almanac/small_sky_order1.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/almanac/small_sky_order1_id_index.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/almanac/small_sky_order1_margin.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/almanac/small_sky_source.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/almanac/small_sky_source_object_index.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/almanac/small_sky_to_small_sky_order1.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.037213 hipscat-0.3.1/tests/data/almanac_exception/
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/almanac_exception/association_missing_join.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/almanac_exception/association_missing_primary.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/almanac_exception/bad_catalog_path.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/almanac_exception/bad_primary_path.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/almanac_exception/bad_type.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/almanac_exception/index_missing_primary.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/almanac_exception/margin_missing_primary.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/almanac_exception/standalone_source_catalog.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    10017 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/generate_data.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.013213 hipscat-0.3.1/tests/data/info_only/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.037213 hipscat-0.3.1/tests/data/info_only/catalog/
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/info_only/catalog/catalog_info.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.037213 hipscat-0.3.1/tests/data/info_only/dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/info_only/dataset/catalog_info.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.037213 hipscat-0.3.1/tests/data/info_only/index_catalog/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/info_only/index_catalog/catalog_info.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.037213 hipscat-0.3.1/tests/data/info_only/margin_cache/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/info_only/margin_cache/catalog_info.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.041213 hipscat-0.3.1/tests/data/small_sky/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.013213 hipscat-0.3.1/tests/data/small_sky/Norder=0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.041213 hipscat-0.3.1/tests/data/small_sky/Norder=0/Dir=0/
+-rw-r--r--   0 runner    (1001) docker     (127)     8880 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky/Norder=0/Dir=0/Npix=11.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky/_common_metadata
+-rw-r--r--   0 runner    (1001) docker     (127)     5130 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky/_metadata
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky/catalog_info.json
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky/partition_info.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  1581120 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky/point_map.fits
+-rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky/provenance_info.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.041213 hipscat-0.3.1/tests/data/small_sky_order1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.013213 hipscat-0.3.1/tests/data/small_sky_order1/Norder=1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.041213 hipscat-0.3.1/tests/data/small_sky_order1/Norder=1/Dir=0/
+-rw-r--r--   0 runner    (1001) docker     (127)     7210 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky_order1/Norder=1/Dir=0/Npix=44.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     6973 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky_order1/Norder=1/Dir=0/Npix=45.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     7216 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky_order1/Norder=1/Dir=0/Npix=46.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     6741 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky_order1/Norder=1/Dir=0/Npix=47.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky_order1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky_order1/_common_metadata
+-rw-r--r--   0 runner    (1001) docker     (127)     8423 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky_order1/_metadata
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky_order1/catalog_info.json
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky_order1/partition_info.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     8640 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky_order1/point_map.fits
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky_order1/provenance_info.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.041213 hipscat-0.3.1/tests/data/small_sky_order1_id_index/
+-rw-r--r--   0 runner    (1001) docker     (127)     2224 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky_order1_id_index/_common_metadata
+-rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky_order1_id_index/_metadata
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky_order1_id_index/catalog_info.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.041213 hipscat-0.3.1/tests/data/small_sky_order1_id_index/index/
+-rw-r--r--   0 runner    (1001) docker     (127)     3867 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky_order1_id_index/index/part.0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky_order1_id_index/provenance_info.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.041213 hipscat-0.3.1/tests/data/small_sky_order1_margin/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.013213 hipscat-0.3.1/tests/data/small_sky_order1_margin/Norder=0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.045213 hipscat-0.3.1/tests/data/small_sky_order1_margin/Norder=0/Dir=0/
+-rw-r--r--   0 runner    (1001) docker     (127)     8255 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky_order1_margin/Norder=0/Dir=0/Npix=4.parquet
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.013213 hipscat-0.3.1/tests/data/small_sky_order1_margin/Norder=1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.045213 hipscat-0.3.1/tests/data/small_sky_order1_margin/Norder=1/Dir=0/
+-rw-r--r--   0 runner    (1001) docker     (127)     8434 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky_order1_margin/Norder=1/Dir=0/Npix=44.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     8476 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky_order1_margin/Norder=1/Dir=0/Npix=45.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     8378 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky_order1_margin/Norder=1/Dir=0/Npix=46.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     8344 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky_order1_margin/Norder=1/Dir=0/Npix=47.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky_order1_margin/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5194 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky_order1_margin/_common_metadata
+-rw-r--r--   0 runner    (1001) docker     (127)    12384 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky_order1_margin/_metadata
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky_order1_margin/catalog_info.json
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky_order1_margin/partition_info.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky_order1_margin/provenance_info.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.045213 hipscat-0.3.1/tests/data/small_sky_source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.013213 hipscat-0.3.1/tests/data/small_sky_source/Norder=0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.045213 hipscat-0.3.1/tests/data/small_sky_source/Norder=0/Dir=0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11421 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky_source/Norder=0/Dir=0/Npix=4.parquet
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.013213 hipscat-0.3.1/tests/data/small_sky_source/Norder=1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.045213 hipscat-0.3.1/tests/data/small_sky_source/Norder=1/Dir=0/
+-rw-r--r--   0 runner    (1001) docker     (127)   133671 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky_source/Norder=1/Dir=0/Npix=47.parquet
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.013213 hipscat-0.3.1/tests/data/small_sky_source/Norder=2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.049213 hipscat-0.3.1/tests/data/small_sky_source/Norder=2/Dir=0/
+-rw-r--r--   0 runner    (1001) docker     (127)    28346 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky_source/Norder=2/Dir=0/Npix=176.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    86262 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky_source/Norder=2/Dir=0/Npix=177.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    92634 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky_source/Norder=2/Dir=0/Npix=178.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    99874 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky_source/Norder=2/Dir=0/Npix=179.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    42177 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky_source/Norder=2/Dir=0/Npix=180.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    54742 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky_source/Norder=2/Dir=0/Npix=181.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    72960 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky_source/Norder=2/Dir=0/Npix=182.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    67771 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky_source/Norder=2/Dir=0/Npix=183.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    80265 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky_source/Norder=2/Dir=0/Npix=184.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)   162064 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky_source/Norder=2/Dir=0/Npix=185.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    31761 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky_source/Norder=2/Dir=0/Npix=186.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    43705 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky_source/Norder=2/Dir=0/Npix=187.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     5525 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky_source/_common_metadata
+-rw-r--r--   0 runner    (1001) docker     (127)    28968 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky_source/_metadata
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky_source/catalog_info.json
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky_source/partition_info.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  1581120 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky_source/point_map.fits
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky_source/provenance_info.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.049213 hipscat-0.3.1/tests/data/small_sky_source_object_index/
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky_source_object_index/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky_source_object_index/_common_metadata
+-rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky_source_object_index/_metadata
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky_source_object_index/catalog_info.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.049213 hipscat-0.3.1/tests/data/small_sky_source_object_index/index/
+-rw-r--r--   0 runner    (1001) docker     (127)     4153 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky_source_object_index/index/part.0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky_source_object_index/provenance_info.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.053213 hipscat-0.3.1/tests/data/small_sky_to_small_sky_order1/
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky_to_small_sky_order1/_common_metadata
+-rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky_to_small_sky_order1/_metadata
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky_to_small_sky_order1/catalog_info.json
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky_to_small_sky_order1/partition_info.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky_to_small_sky_order1/partition_join_info.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.053213 hipscat-0.3.1/tests/hipscat/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.053213 hipscat-0.3.1/tests/hipscat/catalog/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.053213 hipscat-0.3.1/tests/hipscat/catalog/association_catalog/
+-rw-r--r--   0 runner    (1001) docker     (127)     5552 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/hipscat/catalog/association_catalog/test_association_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2627 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/hipscat/catalog/association_catalog/test_association_catalog_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6156 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/hipscat/catalog/association_catalog/test_partition_join_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.053213 hipscat-0.3.1/tests/hipscat/catalog/dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/hipscat/catalog/dataset/test_base_catalog_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4896 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/hipscat/catalog/dataset/test_catalog_info_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/hipscat/catalog/dataset/test_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.053213 hipscat-0.3.1/tests/hipscat/catalog/index/
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/hipscat/catalog/index/test_index_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/hipscat/catalog/index/test_index_catalog_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.053213 hipscat-0.3.1/tests/hipscat/catalog/loaders/
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/hipscat/catalog/loaders/test_read_from_hipscat.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.053213 hipscat-0.3.1/tests/hipscat/catalog/margin_cache/
+-rw-r--r--   0 runner    (1001) docker     (127)     2586 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/hipscat/catalog/margin_cache/test_margin_cache_catalog_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3115 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/hipscat/catalog/margin_cache/test_margin_catalog.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.053213 hipscat-0.3.1/tests/hipscat/catalog/source_catalog/
+-rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/hipscat/catalog/source_catalog/test_source_catalog_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22579 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/hipscat/catalog/test_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/hipscat/catalog/test_catalog_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6742 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/hipscat/catalog/test_partition_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/hipscat/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.053213 hipscat-0.3.1/tests/hipscat/inspection/
+-rw-r--r--   0 runner    (1001) docker     (127)     7492 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/hipscat/inspection/test_almanac.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3550 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/hipscat/inspection/test_almanac_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2775 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/hipscat/inspection/test_visualize_catalog.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.057213 hipscat-0.3.1/tests/hipscat/io/
+-rw-r--r--   0 runner    (1001) docker     (127)     3654 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/hipscat/io/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.057213 hipscat-0.3.1/tests/hipscat/io/file_io/
+-rw-r--r--   0 runner    (1001) docker     (127)     4488 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/hipscat/io/file_io/test_file_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5396 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/hipscat/io/file_io/test_file_pointers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8508 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/hipscat/io/test_parquet_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/hipscat/io/test_paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/hipscat/io/test_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7239 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/hipscat/io/test_write_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.057213 hipscat-0.3.1/tests/hipscat/pixel_math/
+-rw-r--r--   0 runner    (1001) docker     (127)     3203 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/hipscat/pixel_math/test_healpix_pixel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/hipscat/pixel_math/test_healpix_pixel_convertor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/hipscat/pixel_math/test_healpix_pixel_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5361 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/hipscat/pixel_math/test_hipscat_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/hipscat/pixel_math/test_margin_bounding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10360 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/hipscat/pixel_math/test_partition_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3789 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/hipscat/pixel_math/test_pixel_margins.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.057213 hipscat-0.3.1/tests/hipscat/pixel_tree/
+-rw-r--r--   0 runner    (1001) docker     (127)     3395 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/hipscat/pixel_tree/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/hipscat/pixel_tree/test_moc_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11566 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/hipscat/pixel_tree/test_pixel_alignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/hipscat/pixel_tree/test_pixel_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2265 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/hipscat/pixel_tree/test_pixel_tree_builder.py
```

### Comparing `hipscat-0.3.0/.copier-answers.yml` & `hipscat-0.3.1/.copier-answers.yml`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/.gitattributes` & `hipscat-0.3.1/.gitattributes`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/.github/ISSUE_TEMPLATE/1-bug_report.md` & `hipscat-0.3.1/.github/ISSUE_TEMPLATE/1-bug_report.md`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/.github/ISSUE_TEMPLATE/2-feature_request.md` & `hipscat-0.3.1/.github/ISSUE_TEMPLATE/2-feature_request.md`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/.github/pull_request_template.md` & `hipscat-0.3.1/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/.github/workflows/asv-main.yml` & `hipscat-0.3.1/.github/workflows/asv-main.yml`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/.github/workflows/asv-nightly.yml` & `hipscat-0.3.1/.github/workflows/asv-nightly.yml`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/.github/workflows/asv-pr.yml` & `hipscat-0.3.1/.github/workflows/asv-pr.yml`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/.github/workflows/build-documentation.yml` & `hipscat-0.3.1/.github/workflows/build-documentation.yml`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/.github/workflows/pre-commit-ci.yml` & `hipscat-0.3.1/.github/workflows/pre-commit-ci.yml`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/.github/workflows/publish-benchmarks-pr.yml` & `hipscat-0.3.1/.github/workflows/publish-benchmarks-pr.yml`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/.github/workflows/publish-to-pypi.yml` & `hipscat-0.3.1/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/.github/workflows/smoke-test.yml` & `hipscat-0.3.1/.github/workflows/smoke-test.yml`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/.github/workflows/testing-and-coverage.yml` & `hipscat-0.3.1/.github/workflows/testing-and-coverage.yml`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/.gitignore` & `hipscat-0.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/.pre-commit-config.yaml` & `hipscat-0.3.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/.prepare_project.sh` & `hipscat-0.3.1/.prepare_project.sh`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/.setup_dev.sh` & `hipscat-0.3.1/.setup_dev.sh`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/LICENSE` & `hipscat-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/PKG-INFO` & `hipscat-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hipscat
-Version: 0.3.0
+Version: 0.3.1
 Summary: Hierarchical Progressive Survey Catalog
 Author-email: LINCC Frameworks <lincc-frameworks-team@lists.lsst.org>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, LINCC Frameworks
         
         Redistribution and use in source and binary forms, with or without
@@ -39,16 +39,17 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: astropy
-Requires-Dist: fsspec<=2023.9.2
+Requires-Dist: fsspec>=2023.10.0
 Requires-Dist: healpy
+Requires-Dist: mocpy
 Requires-Dist: numba>=0.58
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: pyarrow>=14.0.1
 Requires-Dist: typing-extensions>=4.3.0
 Provides-Extra: dev
 Requires-Dist: adlfs; extra == "dev"
```

### Comparing `hipscat-0.3.0/README.md` & `hipscat-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/benchmarks/asv.conf.json` & `hipscat-0.3.1/benchmarks/asv.conf.json`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/benchmarks/benchmarks.py` & `hipscat-0.3.1/benchmarks/benchmarks.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import hipscat.pixel_math as hist
 from hipscat.catalog import Catalog, PartitionInfo
 from hipscat.catalog.association_catalog.partition_join_info import PartitionJoinInfo
 from hipscat.catalog.catalog_info import CatalogInfo
 from hipscat.io.paths import pixel_catalog_files
 from hipscat.pixel_math import HealpixPixel
 from hipscat.pixel_tree import PixelAlignment, align_trees
-from hipscat.pixel_tree.pixel_tree_builder import PixelTreeBuilder
+from hipscat.pixel_tree.pixel_tree import PixelTree
 
 
 def time_test_alignment_even_sky():
     """Create alignment from an even distribution at order 7"""
     initial_histogram = np.full(hp.order2npix(7), 40)
     result = hist.generate_alignment(initial_histogram, highest_order=7, threshold=1_000)
     # everything maps to order 5, given the density
@@ -50,21 +50,21 @@
         """Just initialize things"""
         self.pixel_list = None
         self.pixel_tree_1 = None
         self.pixel_tree_2 = None
 
     def setup(self):
         self.pixel_list = [HealpixPixel(8, pixel) for pixel in np.arange(100000)]
-        self.pixel_tree_1 = PixelTreeBuilder.from_healpix(self.pixel_list)
-        self.pixel_tree_2 = PixelTreeBuilder.from_healpix(
+        self.pixel_tree_1 = PixelTree.from_healpix(self.pixel_list)
+        self.pixel_tree_2 = PixelTree.from_healpix(
             [HealpixPixel(9, pixel) for pixel in np.arange(0, 400000, 4)]
         )
 
     def time_pixel_tree_creation(self):
-        PixelTreeBuilder.from_healpix(self.pixel_list)
+        PixelTree.from_healpix(self.pixel_list)
 
     def time_inner_pixel_alignment(self):
         align_trees(self.pixel_tree_1, self.pixel_tree_2)
 
     def time_outer_pixel_alignment(self):
         align_trees(self.pixel_tree_1, self.pixel_tree_2, alignment_type="outer")
 
@@ -89,16 +89,16 @@
         pixel_list_b = [HealpixPixel(6, pixel) for pixel in np.arange(25_000)]
         catalog_path_b = os.path.join(root_dir, "catalog_b")
         os.makedirs(catalog_path_b, exist_ok=True)
         partition_info = PartitionInfo.from_healpix(pixel_list_b)
         partition_info.write_to_file(os.path.join(catalog_path_b, "partition_info.csv"))
 
         ## Fake an association table between the two
-        tree_a = PixelTreeBuilder.from_healpix(pixel_list_a)
-        tree_b = PixelTreeBuilder.from_healpix(pixel_list_b)
+        tree_a = PixelTree.from_healpix(pixel_list_a)
+        tree_b = PixelTree.from_healpix(pixel_list_b)
         alignment = align_trees(tree_a, tree_b)
         alignment_df = alignment.pixel_mapping[
             [
                 PixelAlignment.PRIMARY_ORDER_COLUMN_NAME,
                 PixelAlignment.PRIMARY_PIXEL_COLUMN_NAME,
                 PixelAlignment.JOIN_ORDER_COLUMN_NAME,
                 PixelAlignment.JOIN_PIXEL_COLUMN_NAME,
```

### Comparing `hipscat-0.3.0/docs/Makefile` & `hipscat-0.3.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/docs/conf.py` & `hipscat-0.3.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/docs/guide/contributing.rst` & `hipscat-0.3.1/docs/guide/contributing.rst`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/docs/guide/directory_scheme.rst` & `hipscat-0.3.1/docs/guide/directory_scheme.rst`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/docs/guide/margin_cache_diagram.png` & `hipscat-0.3.1/docs/guide/margin_cache_diagram.png`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/docs/guide/pixel_math.md` & `hipscat-0.3.1/docs/guide/pixel_math.md`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/docs/index.rst` & `hipscat-0.3.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/docs/notebooks/catalog_size_inspection.ipynb` & `hipscat-0.3.1/docs/notebooks/catalog_size_inspection.ipynb`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/docs/notebooks/cone_search.ipynb` & `hipscat-0.3.1/docs/notebooks/cone_search.ipynb`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/pyproject.toml` & `hipscat-0.3.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -15,16 +15,17 @@
     "Programming Language :: Python",
 ]
 dynamic = ["version"]
 
 requires-python = ">=3.9"
 dependencies = [
     "astropy",
-    "fsspec<=2023.9.2", # Used for abstract filesystems
+    "fsspec>=2023.10.0", # Used for abstract filesystems
     "healpy",
+    "mocpy",
     "numba>=0.58",
     "numpy", 
     "pandas",
     "pyarrow>=14.0.1",
     "typing-extensions>=4.3.0",
 ]
```

### Comparing `hipscat-0.3.0/src/.pylintrc` & `hipscat-0.3.1/src/.pylintrc`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/src/hipscat/catalog/association_catalog/association_catalog.py` & `hipscat-0.3.1/src/hipscat/catalog/association_catalog/association_catalog.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,13 @@
+from __future__ import annotations
+
 from typing import Any, Dict, Tuple, Union
 
 import pandas as pd
+from mocpy import MOC
 from typing_extensions import TypeAlias
 
 from hipscat.catalog.association_catalog.association_catalog_info import AssociationCatalogInfo
 from hipscat.catalog.association_catalog.partition_join_info import PartitionJoinInfo
 from hipscat.catalog.catalog_type import CatalogType
 from hipscat.catalog.healpix_dataset.healpix_dataset import HealpixDataset, PixelInputTypes
 from hipscat.io import FilePointer, file_io, paths
@@ -27,19 +30,20 @@
 
     def __init__(
         self,
         catalog_info: CatalogInfoClass,
         pixels: PixelInputTypes,
         join_pixels: JoinPixelInputTypes,
         catalog_path=None,
+        moc: MOC | None = None,
         storage_options: Union[Dict[Any, Any], None] = None,
     ) -> None:
         if not catalog_info.catalog_type == CatalogType.ASSOCIATION:
             raise ValueError("Catalog info `catalog_type` must be 'association'")
-        super().__init__(catalog_info, pixels, catalog_path, storage_options=storage_options)
+        super().__init__(catalog_info, pixels, catalog_path, moc=moc, storage_options=storage_options)
         self.join_info = self._get_partition_join_info_from_pixels(join_pixels)
 
     def get_join_pixels(self) -> pd.DataFrame:
         """Get join pixels listing all pairs of pixels from left and right catalogs that contain
         matching association rows
 
         Returns:
```

### Comparing `hipscat-0.3.0/src/hipscat/catalog/association_catalog/association_catalog_info.py` & `hipscat-0.3.1/src/hipscat/catalog/association_catalog/association_catalog_info.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/src/hipscat/catalog/association_catalog/partition_join_info.py` & `hipscat-0.3.1/src/hipscat/catalog/association_catalog/partition_join_info.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/src/hipscat/catalog/catalog.py` & `hipscat-0.3.1/src/hipscat/catalog/catalog.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from __future__ import annotations
 
 from typing import Any, Dict, List, Tuple, Union
 
 import healpy as hp
 import numpy as np
+from mocpy import MOC
 from typing_extensions import TypeAlias
 
 from hipscat.catalog.catalog_info import CatalogInfo
 from hipscat.catalog.catalog_type import CatalogType
 from hipscat.catalog.healpix_dataset.healpix_dataset import HealpixDataset, PixelInputTypes
 from hipscat.pixel_math import HealpixPixel
 from hipscat.pixel_math.box_filter import filter_pixels_by_box, wrap_ra_angles
@@ -44,32 +45,36 @@
     catalog_info: CatalogInfoClass
 
     def __init__(
         self,
         catalog_info: CatalogInfoClass,
         pixels: PixelInputTypes,
         catalog_path: str = None,
+        moc: MOC | None = None,
         storage_options: Union[Dict[Any, Any], None] = None,
     ) -> None:
         """Initializes a Catalog
 
         Args:
             catalog_info: CatalogInfo object with catalog metadata
             pixels: Specifies the pixels contained in the catalog. Can be either a
                 list of HealpixPixel, `PartitionInfo object`, or a `PixelTree` object
             catalog_path: If the catalog is stored on disk, specify the location of the catalog
                 Does not load the catalog from this path, only store as metadata
             storage_options: dictionary that contains abstract filesystem credentials
+            moc (mocpy.MOC): MOC object representing the coverage of the catalog
         """
         if catalog_info.catalog_type not in self.HIPS_CATALOG_TYPES:
             raise ValueError(
                 f"Catalog info `catalog_type` must be one of "
                 f"{', '.join([t.value for t in self.HIPS_CATALOG_TYPES])}"
             )
-        super().__init__(catalog_info, pixels, catalog_path, storage_options)
+        super().__init__(
+            catalog_info, pixels, catalog_path=catalog_path, moc=moc, storage_options=storage_options
+        )
 
     def filter_by_cone(self, ra: float, dec: float, radius_arcsec: float) -> Catalog:
         """Filter the pixels in the catalog to only include the pixels that overlap with a cone
 
         Args:
             ra (float): Right Ascension of the center of the cone in degrees
             dec (float): Declination of the center of the cone in degrees
```

### Comparing `hipscat-0.3.0/src/hipscat/catalog/catalog_info.py` & `hipscat-0.3.1/src/hipscat/catalog/catalog_info.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/src/hipscat/catalog/dataset/base_catalog_info.py` & `hipscat-0.3.1/src/hipscat/catalog/dataset/base_catalog_info.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/src/hipscat/catalog/dataset/catalog_info_factory.py` & `hipscat-0.3.1/src/hipscat/catalog/dataset/catalog_info_factory.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/src/hipscat/catalog/dataset/dataset.py` & `hipscat-0.3.1/src/hipscat/catalog/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/src/hipscat/catalog/index/index_catalog.py` & `hipscat-0.3.1/src/hipscat/catalog/index/index_catalog.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/src/hipscat/catalog/index/index_catalog_info.py` & `hipscat-0.3.1/src/hipscat/catalog/index/index_catalog_info.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/src/hipscat/catalog/margin_cache/margin_cache_catalog_info.py` & `hipscat-0.3.1/src/hipscat/catalog/margin_cache/margin_cache_catalog_info.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/src/hipscat/catalog/margin_cache/margin_catalog.py` & `hipscat-0.3.1/src/hipscat/catalog/margin_cache/margin_catalog.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+from mocpy import MOC
 from typing_extensions import TypeAlias
 
 from hipscat.catalog.catalog_type import CatalogType
 from hipscat.catalog.healpix_dataset.healpix_dataset import HealpixDataset, PixelInputTypes
 from hipscat.catalog.margin_cache import MarginCacheCatalogInfo
 
 
@@ -22,22 +23,26 @@
     catalog_info: CatalogInfoClass
 
     def __init__(
         self,
         catalog_info: CatalogInfoClass,
         pixels: PixelInputTypes,
         catalog_path: str = None,
+        moc: MOC | None = None,
         storage_options: dict | None = None,
     ) -> None:
         """Initializes a Margin Catalog
 
         Args:
             catalog_info: CatalogInfo object with catalog metadata
             pixels: Specifies the pixels contained in the catalog. Can be either a
                 list of HealpixPixel, `PartitionInfo object`, or a `PixelTree` object
             catalog_path: If the catalog is stored on disk, specify the location of the catalog
                 Does not load the catalog from this path, only store as metadata
             storage_options: dictionary that contains abstract filesystem credentials
+            moc (mocpy.MOC): MOC object representing the coverage of the catalog
         """
         if catalog_info.catalog_type != CatalogType.MARGIN:
             raise ValueError(f"Catalog info `catalog_type` must equal {CatalogType.MARGIN}")
-        super().__init__(catalog_info, pixels, catalog_path, storage_options)
+        super().__init__(
+            catalog_info, pixels, catalog_path=catalog_path, moc=moc, storage_options=storage_options
+        )
```

### Comparing `hipscat-0.3.0/src/hipscat/catalog/partition_info.py` & `hipscat-0.3.1/src/hipscat/catalog/partition_info.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/src/hipscat/catalog/source_catalog/source_catalog_info.py` & `hipscat-0.3.1/src/hipscat/catalog/source_catalog/source_catalog_info.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/src/hipscat/inspection/almanac.py` & `hipscat-0.3.1/src/hipscat/inspection/almanac.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/src/hipscat/inspection/almanac_info.py` & `hipscat-0.3.1/src/hipscat/inspection/almanac_info.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/src/hipscat/inspection/visualize_catalog.py` & `hipscat-0.3.1/src/hipscat/inspection/visualize_catalog.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,17 +77,18 @@
             - cart - Cartesian projection
             - orth - Orthographic projection
     """
     max_order = np.max(pixels).order
     min_order = np.min(pixels).order
 
     if max_order == min_order:
-        color = plt.cm.viridis(0.5)  # pylint: disable=no-member
-        colors = [plt.cm.viridis(0.0), color]  # pylint: disable=no-member
-        cmap = mcolors.LinearSegmentedColormap.from_list("my_colormap", colors)
+        colors = [plt.cm.viridis(0.0), plt.cm.viridis(0.1)]  # pylint: disable=no-member
+        cmap = mcolors.LinearSegmentedColormap.from_list("my_colormap", colors, 1)
+        kwargs["cbar"] = False
+        plot_title = f"Norder {max_order} {plot_title}"
     else:
         num_colors = max_order - min_order + 1
         colors = plt.cm.viridis(np.linspace(0, 1, num_colors))  # pylint: disable=no-member
         cmap = mcolors.LinearSegmentedColormap.from_list("my_colormap", colors, num_colors)
 
     order_map = np.full(hp.order2npix(max_order), hp.pixelfunc.UNSEEN)
```

### Comparing `hipscat-0.3.0/src/hipscat/io/__init__.py` & `hipscat-0.3.1/src/hipscat/io/__init__.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/src/hipscat/io/file_io/__init__.py` & `hipscat-0.3.1/src/hipscat/io/file_io/__init__.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/src/hipscat/io/file_io/file_io.py` & `hipscat-0.3.1/src/hipscat/io/file_io/file_io.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/src/hipscat/io/file_io/file_pointer.py` & `hipscat-0.3.1/src/hipscat/io/file_io/file_pointer.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
     Args:
         protocol: str filesytem protocol, file, abfs, or s3
         file_pointer: filesystem pathway
     """
     if not isinstance(file_pointer, str):
         file_pointer = str(file_pointer)
 
-    if protocol == "file":
+    if "file" in protocol:
         # return the entire filepath for local files
         if "file://" in file_pointer:
             split_pointer = file_pointer.split("file://")[1]
         else:
             split_pointer = file_pointer
     elif protocol == "https":
         # https should include the protocol in the file path
@@ -113,15 +113,15 @@
 
     Args:
         pointer: `FilePointer` object
 
     Returns:
         New file pointer with leading slash removed.
     """
-    if protocol != "file" and str(pointer).startswith("/"):
+    if "file" not in protocol and str(pointer).startswith("/"):
         pointer = FilePointer(str(pointer).replace("/", "", 1))
     return pointer
 
 
 def append_paths_to_pointer(pointer: FilePointer, *paths: str) -> FilePointer:
     """Append directories and/or a file name to a specified file pointer.
```

### Comparing `hipscat-0.3.0/src/hipscat/io/parquet_metadata.py` & `hipscat-0.3.1/src/hipscat/io/parquet_metadata.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/src/hipscat/io/paths.py` & `hipscat-0.3.1/src/hipscat/io/paths.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/src/hipscat/io/validation.py` & `hipscat-0.3.1/src/hipscat/io/validation.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/src/hipscat/io/write_metadata.py` & `hipscat-0.3.1/src/hipscat/io/write_metadata.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/src/hipscat/loaders/read_from_hipscat.py` & `hipscat-0.3.1/src/hipscat/loaders/read_from_hipscat.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/src/hipscat/pixel_math/__init__.py` & `hipscat-0.3.1/src/hipscat/pixel_math/__init__.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/src/hipscat/pixel_math/box_filter.py` & `hipscat-0.3.1/src/hipscat/pixel_math/box_filter.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 import numpy as np
 
 from hipscat.pixel_math import HealpixPixel
 from hipscat.pixel_math.filter import get_filtered_pixel_list
 from hipscat.pixel_math.polygon_filter import SphericalCoordinates
 from hipscat.pixel_tree import PixelAlignmentType, align_trees
 from hipscat.pixel_tree.pixel_tree import PixelTree
-from hipscat.pixel_tree.pixel_tree_builder import PixelTreeBuilder
 
 
 def filter_pixels_by_box(
     pixel_tree: PixelTree, ra: Tuple[float, float] | None, dec: Tuple[float, float] | None
 ) -> List[HealpixPixel]:
     """Filter the leaf pixels in a pixel tree to return a partition_info dataframe
     with the pixels that overlap with a right ascension and/or declination region.
@@ -88,28 +87,28 @@
                 # South Pole
                 [(ra_range[0], 0), (0, -90), (ra_range[1], 0)],
             ],
             order,
         )
 
     pixel_list = [HealpixPixel(order, polygon_pixel) for polygon_pixel in pixels_in_range]
-    return PixelTreeBuilder.from_healpix(pixel_list)
+    return PixelTree.from_healpix(pixel_list)
 
 
 def _generate_dec_strip_pixel_tree(dec_range: Tuple[float, float], order: int) -> PixelTree:
     """Generates a pixel_tree filled with leaf nodes at a given order that overlap with the dec region."""
     nside = hp.order2nside(order)
     # Convert declination values to colatitudes, in radians, and revert their order
     colat_rad = np.sort(np.radians([90 - dec if dec > 0 else 90 + abs(dec) for dec in dec_range]))
     # Figure out which pixels in nested order are contained in the declination band
     pixels_in_range = hp.ring2nest(
         nside, hp.query_strip(nside, theta1=colat_rad[0], theta2=colat_rad[1], inclusive=True)
     )
     pixel_list = [HealpixPixel(order, polygon_pixel) for polygon_pixel in pixels_in_range]
-    return PixelTreeBuilder.from_healpix(pixel_list)
+    return PixelTree.from_healpix(pixel_list)
 
 
 def _get_division_ra(ra_range: Tuple[float, float]) -> float | None:
     """Gets the division angle for the right ascension region. This is crucial for the edge
     cases where we need to split up polygons wider than 180 degrees into smaller polygons."""
     division_ra = None
     if ra_range[0] > ra_range[1] and 360 - ra_range[0] + ra_range[1] >= 180:
```

### Comparing `hipscat-0.3.0/src/hipscat/pixel_math/cone_filter.py` & `hipscat-0.3.1/src/hipscat/pixel_math/cone_filter.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 import healpy as hp
 import numpy as np
 
 from hipscat.pixel_math import HealpixPixel
 from hipscat.pixel_math.filter import get_filtered_pixel_list
 from hipscat.pixel_tree.pixel_tree import PixelTree
-from hipscat.pixel_tree.pixel_tree_builder import PixelTreeBuilder
 
 
 def filter_pixels_by_cone(
     pixel_tree: PixelTree, ra: float, dec: float, radius_arcsec: float
 ) -> List[HealpixPixel]:
     """Filter the leaf pixels in a pixel tree to return a partition_info dataframe with the pixels
     that overlap with a cone.
@@ -31,8 +30,8 @@
 def _generate_cone_pixel_tree(ra: float, dec: float, radius_arcsec: float, order: int):
     """Generates a pixel_tree filled with leaf nodes at a given order that overlap with a cone"""
     n_side = hp.order2nside(order)
     center_vec = hp.ang2vec(ra, dec, lonlat=True)
     radius_radians = np.radians(radius_arcsec / 3600.0)
     cone_pixels = hp.query_disc(n_side, center_vec, radius_radians, inclusive=True, nest=True)
     pixel_list = [HealpixPixel(order, cone_pixel) for cone_pixel in cone_pixels]
-    return PixelTreeBuilder.from_healpix(pixel_list)
+    return PixelTree.from_healpix(pixel_list)
```

### Comparing `hipscat-0.3.0/src/hipscat/pixel_math/filter.py` & `hipscat-0.3.1/src/hipscat/pixel_math/filter.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/src/hipscat/pixel_math/healpix_pixel.py` & `hipscat-0.3.1/src/hipscat/pixel_math/healpix_pixel.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/src/hipscat/pixel_math/healpix_pixel_convertor.py` & `hipscat-0.3.1/src/hipscat/pixel_math/healpix_pixel_convertor.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/src/hipscat/pixel_math/healpix_pixel_function.py` & `hipscat-0.3.1/src/hipscat/pixel_math/healpix_pixel_function.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/src/hipscat/pixel_math/hipscat_id.py` & `hipscat-0.3.1/src/hipscat/pixel_math/hipscat_id.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/src/hipscat/pixel_math/margin_bounding.py` & `hipscat-0.3.1/src/hipscat/pixel_math/margin_bounding.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/src/hipscat/pixel_math/partition_stats.py` & `hipscat-0.3.1/src/hipscat/pixel_math/partition_stats.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/src/hipscat/pixel_math/pixel_margins.py` & `hipscat-0.3.1/src/hipscat/pixel_math/pixel_margins.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/src/hipscat/pixel_math/polygon_filter.py` & `hipscat-0.3.1/src/hipscat/pixel_math/polygon_filter.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import healpy as hp
 import numpy as np
 from typing_extensions import TypeAlias
 
 from hipscat.pixel_math import HealpixPixel
 from hipscat.pixel_math.filter import get_filtered_pixel_list
 from hipscat.pixel_tree.pixel_tree import PixelTree
-from hipscat.pixel_tree.pixel_tree_builder import PixelTreeBuilder
 
 # Pair of spherical sky coordinates (ra, dec)
 SphericalCoordinates: TypeAlias = Tuple[float, float]
 
 # Sky coordinates on the unit sphere, in cartesian representation (x,y,z)
 CartesianCoordinates: TypeAlias = Tuple[float, float, float]
 
@@ -40,8 +39,8 @@
 
 def _generate_polygon_pixel_tree(vertices: np.array, order: int) -> PixelTree:
     """Generates a pixel_tree filled with leaf nodes at a given order that overlap within
     a polygon. Vertices is an array of 3D coordinates, in cartesian representation (x,y,z)
     and shape (Num vertices, 3), representing the vertices of the polygon."""
     polygon_pixels = hp.query_polygon(hp.order2nside(order), vertices, inclusive=True, nest=True)
     pixel_list = [HealpixPixel(order, polygon_pixel) for polygon_pixel in polygon_pixels]
-    return PixelTreeBuilder.from_healpix(pixel_list)
+    return PixelTree.from_healpix(pixel_list)
```

### Comparing `hipscat-0.3.0/src/hipscat/pixel_math/validators.py` & `hipscat-0.3.1/src/hipscat/pixel_math/validators.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/src/hipscat/pixel_tree/negative_tree.py` & `hipscat-0.3.1/src/hipscat/pixel_tree/negative_tree.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/src/hipscat/pixel_tree/pixel_alignment.py` & `hipscat-0.3.1/src/hipscat/pixel_tree/pixel_alignment.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,17 @@
-from typing import List
+from typing import Callable, Dict, List
 
 import numba
 import numpy as np
 import pandas as pd
+from mocpy import MOC
 from numba import njit
 
 from hipscat.pixel_math.healpix_pixel_function import get_pixels_from_intervals
+from hipscat.pixel_tree.moc_filter import perform_filter_by_moc
 from hipscat.pixel_tree.pixel_alignment_types import PixelAlignmentType
 from hipscat.pixel_tree.pixel_tree import PixelTree
 
 LEFT_INCLUDE_ALIGNMENT_TYPES = [PixelAlignmentType.LEFT, PixelAlignmentType.OUTER]
 RIGHT_INCLUDE_ALIGNMENT_TYPES = [PixelAlignmentType.RIGHT, PixelAlignmentType.OUTER]
 
 
@@ -382,7 +384,62 @@
     # After loop, if either tree needs to be fully covered and loop hasn't checked all pixels from that tree
     # then cover the remaining pixels
     if include_all_right and right_index < len(right):
         _add_remaining_pixels(added_until, right, right_index, RIGHT_SIDE, mapping)
     if include_all_left and left_index < len(left):
         _add_remaining_pixels(added_until, left, left_index, LEFT_SIDE, mapping)
     return mapping
+
+
+def filter_alignment_by_moc(alignment: PixelAlignment, moc: MOC) -> PixelAlignment:
+    """Filters an alignment by a moc to only include pixels in the aligned_tree that overlap with the moc,
+    and the corresponding rows in the mapping.
+
+    Args:
+        alignment (PixelAlignment): The pixel alignment to filter
+        moc (mocpy.MOC): The moc to filter by
+
+    Returns:
+        PixelAlignment object with the filtered mapping and tree
+    """
+    moc_ranges = moc.to_depth29_ranges
+    tree_29_ranges = alignment.pixel_tree.tree << (2 * (29 - alignment.pixel_tree.tree_order))
+    tree_mask = perform_filter_by_moc(tree_29_ranges, moc_ranges)
+    new_tree = PixelTree(alignment.pixel_tree.tree[tree_mask], alignment.pixel_tree.tree_order)
+    return PixelAlignment(new_tree, alignment.pixel_mapping.iloc[tree_mask], alignment.alignment_type)
+
+
+def align_with_mocs(
+    left_tree: PixelTree,
+    right_tree: PixelTree,
+    left_moc: MOC,
+    right_moc: MOC,
+    alignment_type: PixelAlignmentType = PixelAlignmentType.INNER,
+) -> PixelAlignment:
+    """Aligns two pixel trees and mocs together, resulting in a pixel alignment with only aligned pixels that
+    have coverage in the mocs.
+
+    Args:
+        left_tree (PixelTree): The left tree to align
+        right_tree (PixelTree): The right tree to align
+        left_moc (mocpy.MOC): the moc with the coverage of the left catalog
+        right_moc (mocpy.MOC): the moc with the coverage of the right catalog
+        alignment_type (PixelAlignmentType): The type of alignment describing how to handle nodes which exist
+            in one tree but not the other. Options are:
+
+                - inner - only use pixels that appear in both catalogs
+                - left - use all pixels that appear in the left catalog and any overlapping from the right
+                - right - use all pixels that appear in the right catalog and any overlapping from the left
+                - outer - use all pixels from both catalogs
+
+    Returns:
+        The PixelAlignment object with the aligned trees filtered by the coverage in the catalogs.
+    """
+    moc_intersection_methods: Dict[PixelAlignmentType, Callable[[MOC, MOC], MOC]] = {
+        PixelAlignmentType.INNER: lambda l, r: l.intersection(r),
+        PixelAlignmentType.LEFT: lambda l, r: l,
+        PixelAlignmentType.RIGHT: lambda l, r: r,
+        PixelAlignmentType.OUTER: lambda l, r: l.union(r),
+    }
+    filter_moc = moc_intersection_methods[alignment_type](left_moc, right_moc)
+    alignment = align_trees(left_tree, right_tree, alignment_type=alignment_type)
+    return filter_alignment_by_moc(alignment, filter_moc)
```

### Comparing `hipscat-0.3.0/src/hipscat/pixel_tree/pixel_tree.py` & `hipscat-0.3.1/src/hipscat/pixel_tree/pixel_tree.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 from typing import List, Sequence
 
 import numpy as np
+from mocpy import MOC
 
 from hipscat.pixel_math import HealpixInputTypes, HealpixPixel
 from hipscat.pixel_math.healpix_pixel_convertor import get_healpix_tuple
 from hipscat.pixel_math.healpix_pixel_function import get_pixels_from_intervals
 
 
 class PixelTree:
@@ -80,15 +81,19 @@
 
     def get_healpix_pixels(self) -> List[HealpixPixel]:
         """Creates a list of HealpixPixels in the tree
 
         Returns (List[HealpixPixel]):
             A list of the HEALPix pixels in the tree
         """
-        return np.vectorize(HealpixPixel)(self.pixels.T[0], self.pixels.T[1])
+        return [HealpixPixel(p[0], p[1]) for p in self.pixels]
+
+    def to_moc(self) -> MOC:
+        """Returns the MOC object that covers the same pixels as the tree"""
+        return MOC.from_healpix_cells(self.pixels.T[1], self.pixels.T[0], self.tree_order)
 
     @classmethod
     def from_healpix(cls, healpix_pixels: Sequence[HealpixInputTypes], tree_order=None) -> PixelTree:
         """Build a tree from a list of constituent healpix pixels
 
         Args:
             healpix_pixels: list of healpix pixels
```

### Comparing `hipscat-0.3.0/src/hipscat.egg-info/PKG-INFO` & `hipscat-0.3.1/src/hipscat.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hipscat
-Version: 0.3.0
+Version: 0.3.1
 Summary: Hierarchical Progressive Survey Catalog
 Author-email: LINCC Frameworks <lincc-frameworks-team@lists.lsst.org>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, LINCC Frameworks
         
         Redistribution and use in source and binary forms, with or without
@@ -39,16 +39,17 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: astropy
-Requires-Dist: fsspec<=2023.9.2
+Requires-Dist: fsspec>=2023.10.0
 Requires-Dist: healpy
+Requires-Dist: mocpy
 Requires-Dist: numba>=0.58
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: pyarrow>=14.0.1
 Requires-Dist: typing-extensions>=4.3.0
 Provides-Extra: dev
 Requires-Dist: adlfs; extra == "dev"
```

### Comparing `hipscat-0.3.0/src/hipscat.egg-info/SOURCES.txt` & `hipscat-0.3.1/src/hipscat.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -95,19 +95,19 @@
 src/hipscat/pixel_math/hipscat_id.py
 src/hipscat/pixel_math/margin_bounding.py
 src/hipscat/pixel_math/partition_stats.py
 src/hipscat/pixel_math/pixel_margins.py
 src/hipscat/pixel_math/polygon_filter.py
 src/hipscat/pixel_math/validators.py
 src/hipscat/pixel_tree/__init__.py
+src/hipscat/pixel_tree/moc_filter.py
 src/hipscat/pixel_tree/negative_tree.py
 src/hipscat/pixel_tree/pixel_alignment.py
 src/hipscat/pixel_tree/pixel_alignment_types.py
 src/hipscat/pixel_tree/pixel_tree.py
-src/hipscat/pixel_tree/pixel_tree_builder.py
 tests/.pylintrc
 tests/conftest.py
 tests/data/generate_data.ipynb
 tests/data/almanac/deprecated.yml
 tests/data/almanac/small_sky.yml
 tests/data/almanac/small_sky_order1.yml
 tests/data/almanac/small_sky_order1_id_index.yml
@@ -222,10 +222,11 @@
 tests/hipscat/pixel_math/test_healpix_pixel_convertor.py
 tests/hipscat/pixel_math/test_healpix_pixel_function.py
 tests/hipscat/pixel_math/test_hipscat_id.py
 tests/hipscat/pixel_math/test_margin_bounding.py
 tests/hipscat/pixel_math/test_partition_stats.py
 tests/hipscat/pixel_math/test_pixel_margins.py
 tests/hipscat/pixel_tree/conftest.py
+tests/hipscat/pixel_tree/test_moc_filter.py
 tests/hipscat/pixel_tree/test_pixel_alignment.py
 tests/hipscat/pixel_tree/test_pixel_tree.py
 tests/hipscat/pixel_tree/test_pixel_tree_builder.py
```

### Comparing `hipscat-0.3.0/tests/.pylintrc` & `hipscat-0.3.1/tests/.pylintrc`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/tests/conftest.py` & `hipscat-0.3.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/tests/data/generate_data.ipynb` & `hipscat-0.3.1/tests/data/generate_data.ipynb`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/tests/data/small_sky/Norder=0/Dir=0/Npix=11.parquet` & `hipscat-0.3.1/tests/data/small_sky/Norder=0/Dir=0/Npix=11.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/tests/data/small_sky/_common_metadata` & `hipscat-0.3.1/tests/data/small_sky/_common_metadata`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/tests/data/small_sky/_metadata` & `hipscat-0.3.1/tests/data/small_sky/_metadata`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/tests/data/small_sky/point_map.fits` & `hipscat-0.3.1/tests/data/small_sky/point_map.fits`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/tests/data/small_sky/provenance_info.json` & `hipscat-0.3.1/tests/data/small_sky/provenance_info.json`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/tests/data/small_sky_order1/Norder=1/Dir=0/Npix=44.parquet` & `hipscat-0.3.1/tests/data/small_sky_order1/Norder=1/Dir=0/Npix=44.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/tests/data/small_sky_order1/Norder=1/Dir=0/Npix=45.parquet` & `hipscat-0.3.1/tests/data/small_sky_order1/Norder=1/Dir=0/Npix=45.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/tests/data/small_sky_order1/Norder=1/Dir=0/Npix=46.parquet` & `hipscat-0.3.1/tests/data/small_sky_order1/Norder=1/Dir=0/Npix=46.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/tests/data/small_sky_order1/Norder=1/Dir=0/Npix=47.parquet` & `hipscat-0.3.1/tests/data/small_sky_order1/Norder=1/Dir=0/Npix=47.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/tests/data/small_sky_order1/README.md` & `hipscat-0.3.1/tests/data/small_sky_order1/README.md`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/tests/data/small_sky_order1/_common_metadata` & `hipscat-0.3.1/tests/data/small_sky_order1/_common_metadata`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/tests/data/small_sky_order1/_metadata` & `hipscat-0.3.1/tests/data/small_sky_order1/_metadata`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/tests/data/small_sky_order1/point_map.fits` & `hipscat-0.3.1/tests/data/small_sky_order1/point_map.fits`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/tests/data/small_sky_order1/provenance_info.json` & `hipscat-0.3.1/tests/data/small_sky_order1/provenance_info.json`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/tests/data/small_sky_order1_id_index/_common_metadata` & `hipscat-0.3.1/tests/data/small_sky_order1_id_index/_common_metadata`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/tests/data/small_sky_order1_id_index/_metadata` & `hipscat-0.3.1/tests/data/small_sky_order1_id_index/_metadata`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/tests/data/small_sky_order1_id_index/index/part.0.parquet` & `hipscat-0.3.1/tests/data/small_sky_order1_id_index/index/part.0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/tests/data/small_sky_order1_id_index/provenance_info.json` & `hipscat-0.3.1/tests/data/small_sky_order1_id_index/provenance_info.json`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/tests/data/small_sky_order1_margin/Norder=0/Dir=0/Npix=4.parquet` & `hipscat-0.3.1/tests/data/small_sky_order1_margin/Norder=0/Dir=0/Npix=4.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/tests/data/small_sky_order1_margin/Norder=1/Dir=0/Npix=44.parquet` & `hipscat-0.3.1/tests/data/small_sky_order1_margin/Norder=1/Dir=0/Npix=44.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/tests/data/small_sky_order1_margin/Norder=1/Dir=0/Npix=45.parquet` & `hipscat-0.3.1/tests/data/small_sky_order1_margin/Norder=1/Dir=0/Npix=45.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/tests/data/small_sky_order1_margin/Norder=1/Dir=0/Npix=46.parquet` & `hipscat-0.3.1/tests/data/small_sky_order1_margin/Norder=1/Dir=0/Npix=46.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/tests/data/small_sky_order1_margin/Norder=1/Dir=0/Npix=47.parquet` & `hipscat-0.3.1/tests/data/small_sky_order1_margin/Norder=1/Dir=0/Npix=47.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/tests/data/small_sky_order1_margin/README.md` & `hipscat-0.3.1/tests/data/small_sky_order1_margin/README.md`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/tests/data/small_sky_order1_margin/_common_metadata` & `hipscat-0.3.1/tests/data/small_sky_order1_margin/_common_metadata`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/tests/data/small_sky_order1_margin/_metadata` & `hipscat-0.3.1/tests/data/small_sky_order1_margin/_metadata`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/tests/data/small_sky_order1_margin/provenance_info.json` & `hipscat-0.3.1/tests/data/small_sky_order1_margin/provenance_info.json`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/tests/data/small_sky_source/Norder=0/Dir=0/Npix=4.parquet` & `hipscat-0.3.1/tests/data/small_sky_source/Norder=0/Dir=0/Npix=4.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/tests/data/small_sky_source/Norder=1/Dir=0/Npix=47.parquet` & `hipscat-0.3.1/tests/data/small_sky_source/Norder=1/Dir=0/Npix=47.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/tests/data/small_sky_source/Norder=2/Dir=0/Npix=176.parquet` & `hipscat-0.3.1/tests/data/small_sky_source/Norder=2/Dir=0/Npix=176.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/tests/data/small_sky_source/Norder=2/Dir=0/Npix=177.parquet` & `hipscat-0.3.1/tests/data/small_sky_source/Norder=2/Dir=0/Npix=177.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/tests/data/small_sky_source/Norder=2/Dir=0/Npix=178.parquet` & `hipscat-0.3.1/tests/data/small_sky_source/Norder=2/Dir=0/Npix=178.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/tests/data/small_sky_source/Norder=2/Dir=0/Npix=179.parquet` & `hipscat-0.3.1/tests/data/small_sky_source/Norder=2/Dir=0/Npix=179.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/tests/data/small_sky_source/Norder=2/Dir=0/Npix=180.parquet` & `hipscat-0.3.1/tests/data/small_sky_source/Norder=2/Dir=0/Npix=180.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/tests/data/small_sky_source/Norder=2/Dir=0/Npix=181.parquet` & `hipscat-0.3.1/tests/data/small_sky_source/Norder=2/Dir=0/Npix=181.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/tests/data/small_sky_source/Norder=2/Dir=0/Npix=182.parquet` & `hipscat-0.3.1/tests/data/small_sky_source/Norder=2/Dir=0/Npix=182.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/tests/data/small_sky_source/Norder=2/Dir=0/Npix=183.parquet` & `hipscat-0.3.1/tests/data/small_sky_source/Norder=2/Dir=0/Npix=183.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/tests/data/small_sky_source/Norder=2/Dir=0/Npix=184.parquet` & `hipscat-0.3.1/tests/data/small_sky_source/Norder=2/Dir=0/Npix=184.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/tests/data/small_sky_source/Norder=2/Dir=0/Npix=185.parquet` & `hipscat-0.3.1/tests/data/small_sky_source/Norder=2/Dir=0/Npix=185.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/tests/data/small_sky_source/Norder=2/Dir=0/Npix=186.parquet` & `hipscat-0.3.1/tests/data/small_sky_source/Norder=2/Dir=0/Npix=186.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/tests/data/small_sky_source/Norder=2/Dir=0/Npix=187.parquet` & `hipscat-0.3.1/tests/data/small_sky_source/Norder=2/Dir=0/Npix=187.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/tests/data/small_sky_source/_common_metadata` & `hipscat-0.3.1/tests/data/small_sky_source/_common_metadata`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/tests/data/small_sky_source/_metadata` & `hipscat-0.3.1/tests/data/small_sky_source/_metadata`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/tests/data/small_sky_source/point_map.fits` & `hipscat-0.3.1/tests/data/small_sky_source/point_map.fits`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/tests/data/small_sky_source/provenance_info.json` & `hipscat-0.3.1/tests/data/small_sky_source/provenance_info.json`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/tests/data/small_sky_source_object_index/README.md` & `hipscat-0.3.1/tests/data/small_sky_source_object_index/README.md`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/tests/data/small_sky_source_object_index/_common_metadata` & `hipscat-0.3.1/tests/data/small_sky_source_object_index/_common_metadata`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/tests/data/small_sky_source_object_index/_metadata` & `hipscat-0.3.1/tests/data/small_sky_source_object_index/_metadata`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/tests/data/small_sky_source_object_index/index/part.0.parquet` & `hipscat-0.3.1/tests/data/small_sky_source_object_index/index/part.0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/tests/data/small_sky_source_object_index/provenance_info.json` & `hipscat-0.3.1/tests/data/small_sky_source_object_index/provenance_info.json`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/tests/data/small_sky_to_small_sky_order1/_common_metadata` & `hipscat-0.3.1/tests/data/small_sky_to_small_sky_order1/_common_metadata`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/tests/data/small_sky_to_small_sky_order1/_metadata` & `hipscat-0.3.1/tests/data/small_sky_to_small_sky_order1/_metadata`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/tests/hipscat/catalog/association_catalog/test_association_catalog.py` & `hipscat-0.3.1/tests/hipscat/catalog/association_catalog/test_association_catalog.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/tests/hipscat/catalog/association_catalog/test_association_catalog_info.py` & `hipscat-0.3.1/tests/hipscat/catalog/association_catalog/test_association_catalog_info.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/tests/hipscat/catalog/association_catalog/test_partition_join_info.py` & `hipscat-0.3.1/tests/hipscat/catalog/association_catalog/test_partition_join_info.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/tests/hipscat/catalog/dataset/test_base_catalog_info.py` & `hipscat-0.3.1/tests/hipscat/catalog/dataset/test_base_catalog_info.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/tests/hipscat/catalog/dataset/test_catalog_info_factory.py` & `hipscat-0.3.1/tests/hipscat/catalog/dataset/test_catalog_info_factory.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/tests/hipscat/catalog/dataset/test_dataset.py` & `hipscat-0.3.1/tests/hipscat/catalog/dataset/test_dataset.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/tests/hipscat/catalog/index/test_index_catalog.py` & `hipscat-0.3.1/tests/hipscat/catalog/index/test_index_catalog.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/tests/hipscat/catalog/index/test_index_catalog_info.py` & `hipscat-0.3.1/tests/hipscat/catalog/index/test_index_catalog_info.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/tests/hipscat/catalog/margin_cache/test_margin_cache_catalog_info.py` & `hipscat-0.3.1/tests/hipscat/catalog/margin_cache/test_margin_cache_catalog_info.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/tests/hipscat/catalog/margin_cache/test_margin_catalog.py` & `hipscat-0.3.1/tests/hipscat/catalog/margin_cache/test_margin_catalog.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/tests/hipscat/catalog/source_catalog/test_source_catalog_info.py` & `hipscat-0.3.1/tests/hipscat/catalog/source_catalog/test_source_catalog_info.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/tests/hipscat/catalog/test_catalog.py` & `hipscat-0.3.1/tests/hipscat/catalog/test_catalog.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,19 +3,21 @@
 import os
 
 import healpy as hp
 import numpy as np
 import pytest
 
 from hipscat.catalog import Catalog, CatalogType, PartitionInfo
+from hipscat.io import paths
+from hipscat.io.file_io import read_fits_image
 from hipscat.loaders import read_from_hipscat
 from hipscat.pixel_math import HealpixPixel
 from hipscat.pixel_math.box_filter import _generate_ra_strip_pixel_tree
 from hipscat.pixel_math.validators import ValidatorsErrors
-from hipscat.pixel_tree.pixel_tree_builder import PixelTreeBuilder
+from hipscat.pixel_tree.pixel_tree import PixelTree
 
 
 def test_catalog_load(catalog_info, catalog_pixels):
     catalog = Catalog(catalog_info, catalog_pixels)
     assert catalog.get_healpix_pixels() == catalog_pixels
     assert catalog.catalog_name == catalog_info.catalog_name
 
@@ -40,15 +42,15 @@
     assert len(catalog.get_healpix_pixels()) == len(catalog_pixels)
     assert len(catalog.pixel_tree.get_healpix_pixels()) == len(catalog_pixels)
     for hp_pixel in catalog_pixels:
         assert hp_pixel in catalog.pixel_tree
 
 
 def test_tree_pixel_input(catalog_info, catalog_pixels):
-    tree = PixelTreeBuilder.from_healpix(catalog_pixels)
+    tree = PixelTree.from_healpix(catalog_pixels)
     catalog = Catalog(catalog_info, tree)
     assert len(catalog.get_healpix_pixels()) == len(catalog_pixels)
     assert len(catalog.pixel_tree.get_healpix_pixels()) == len(catalog_pixels)
     for pixel in catalog_pixels:
         assert pixel in catalog.pixel_tree
 
 
@@ -89,14 +91,26 @@
     cat = read_from_hipscat(small_sky_order1_dir)
 
     assert isinstance(cat, Catalog)
     assert cat.catalog_name == "small_sky_order1"
     assert len(cat.get_healpix_pixels()) == 4
 
 
+def test_load_catalog_small_sky_order1_moc(small_sky_order1_dir):
+    """Instantiate a catalog with 4 pixels"""
+    cat = read_from_hipscat(small_sky_order1_dir)
+
+    assert isinstance(cat, Catalog)
+    assert cat.moc is not None
+    counts_skymap = read_fits_image(paths.get_point_map_file_pointer(small_sky_order1_dir))
+    skymap_order = hp.nside2order(hp.npix2nside(len(counts_skymap)))
+    assert cat.moc.max_order == skymap_order
+    assert np.all(cat.moc.flatten() == np.where(counts_skymap > 0))
+
+
 def test_load_catalog_small_sky_source(small_sky_source_dir):
     """Instantiate a source catalog with 14 pixels"""
     cat = read_from_hipscat(small_sky_source_dir)
 
     assert isinstance(cat, Catalog)
     assert cat.catalog_name == "small_sky_source"
     assert len(cat.get_healpix_pixels()) == 14
@@ -482,15 +496,15 @@
 
 def test_generate_negative_tree_pixels_multi_order(small_sky_order1_catalog):
     """Test generate_negative_tree_pixels on a catalog with
     missing pixels on multiple order.
     """
     # remove one of the order 1 pixels from the catalog.
     nodes = small_sky_order1_catalog.pixel_tree.get_healpix_pixels()
-    small_sky_order1_catalog.pixel_tree = PixelTreeBuilder.from_healpix(nodes[1:])
+    small_sky_order1_catalog.pixel_tree = PixelTree.from_healpix(nodes[1:])
 
     expected_pixels = [
         HealpixPixel(0, 0),
         HealpixPixel(0, 1),
         HealpixPixel(0, 2),
         HealpixPixel(0, 3),
         HealpixPixel(0, 4),
```

### Comparing `hipscat-0.3.0/tests/hipscat/catalog/test_catalog_info.py` & `hipscat-0.3.1/tests/hipscat/catalog/test_catalog_info.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/tests/hipscat/catalog/test_partition_info.py` & `hipscat-0.3.1/tests/hipscat/catalog/test_partition_info.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/tests/hipscat/conftest.py` & `hipscat-0.3.1/tests/hipscat/conftest.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/tests/hipscat/inspection/test_almanac.py` & `hipscat-0.3.1/tests/hipscat/inspection/test_almanac.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/tests/hipscat/inspection/test_almanac_info.py` & `hipscat-0.3.1/tests/hipscat/inspection/test_almanac_info.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/tests/hipscat/inspection/test_visualize_catalog.py` & `hipscat-0.3.1/tests/hipscat/inspection/test_visualize_catalog.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/tests/hipscat/io/conftest.py` & `hipscat-0.3.1/tests/hipscat/io/conftest.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/tests/hipscat/io/file_io/test_file_io.py` & `hipscat-0.3.1/tests/hipscat/io/file_io/test_file_io.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/tests/hipscat/io/file_io/test_file_pointers.py` & `hipscat-0.3.1/tests/hipscat/io/file_io/test_file_pointers.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,15 +108,15 @@
     assert small_sky_contents == expected
 
     assert len(get_directory_contents(tmp_path)) == 0
 
 
 def test_get_fs():
     filesystem, _ = get_fs("file://")
-    assert filesystem.protocol == "file"
+    assert "file" in filesystem.protocol
 
     # this will fail if the environment installs lakefs to import
     with pytest.raises(ImportError):
         get_fs("lakefs://")
 
     with pytest.raises(ValueError):
         get_fs("invalid://")
```

### Comparing `hipscat-0.3.0/tests/hipscat/io/test_parquet_metadata.py` & `hipscat-0.3.1/tests/hipscat/io/test_parquet_metadata.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/tests/hipscat/io/test_paths.py` & `hipscat-0.3.1/tests/hipscat/io/test_paths.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/tests/hipscat/io/test_validation.py` & `hipscat-0.3.1/tests/hipscat/io/test_validation.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/tests/hipscat/io/test_write_metadata.py` & `hipscat-0.3.1/tests/hipscat/io/test_write_metadata.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/tests/hipscat/pixel_math/test_healpix_pixel.py` & `hipscat-0.3.1/tests/hipscat/pixel_math/test_healpix_pixel.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/tests/hipscat/pixel_math/test_healpix_pixel_convertor.py` & `hipscat-0.3.1/tests/hipscat/pixel_math/test_healpix_pixel_convertor.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/tests/hipscat/pixel_math/test_healpix_pixel_function.py` & `hipscat-0.3.1/tests/hipscat/pixel_math/test_healpix_pixel_function.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/tests/hipscat/pixel_math/test_hipscat_id.py` & `hipscat-0.3.1/tests/hipscat/pixel_math/test_hipscat_id.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/tests/hipscat/pixel_math/test_margin_bounding.py` & `hipscat-0.3.1/tests/hipscat/pixel_math/test_margin_bounding.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/tests/hipscat/pixel_math/test_partition_stats.py` & `hipscat-0.3.1/tests/hipscat/pixel_math/test_partition_stats.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/tests/hipscat/pixel_math/test_pixel_margins.py` & `hipscat-0.3.1/tests/hipscat/pixel_math/test_pixel_margins.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.0/tests/hipscat/pixel_tree/conftest.py` & `hipscat-0.3.1/tests/hipscat/pixel_tree/conftest.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,45 +1,48 @@
 import os
 
 import pytest
 
 from hipscat.pixel_math import HealpixPixel
-from hipscat.pixel_tree.pixel_tree_builder import PixelTreeBuilder
+from hipscat.pixel_tree.pixel_tree import PixelTree
 
 
 @pytest.fixture
 def pixel_trees_dir(test_data_dir):
     return os.path.join(test_data_dir, "pixel_trees")
 
 
 @pytest.fixture
 def pixel_tree_1():
-    return PixelTreeBuilder.from_healpix([HealpixPixel(0, 11)])
+    return PixelTree.from_healpix([HealpixPixel(0, 11)])
 
 
 @pytest.fixture
-def pixel_tree_2():
-    return PixelTreeBuilder.from_healpix(
-        [
-            HealpixPixel(0, 10),
-            HealpixPixel(1, 33),
-            HealpixPixel(1, 35),
-            HealpixPixel(1, 44),
-            HealpixPixel(1, 45),
-            HealpixPixel(1, 46),
-            HealpixPixel(2, 128),
-            HealpixPixel(2, 130),
-            HealpixPixel(2, 131),
-        ]
-    )
+def pixel_tree_2_pixels():
+    return [
+        HealpixPixel(2, 128),
+        HealpixPixel(2, 130),
+        HealpixPixel(2, 131),
+        HealpixPixel(1, 33),
+        HealpixPixel(1, 35),
+        HealpixPixel(0, 10),
+        HealpixPixel(1, 44),
+        HealpixPixel(1, 45),
+        HealpixPixel(1, 46),
+    ]
+
+
+@pytest.fixture
+def pixel_tree_2(pixel_tree_2_pixels):
+    return PixelTree.from_healpix(pixel_tree_2_pixels)
 
 
 @pytest.fixture
 def pixel_tree_3():
-    return PixelTreeBuilder.from_healpix(
+    return PixelTree.from_healpix(
         [
             HealpixPixel(0, 8),
             HealpixPixel(1, 36),
             HealpixPixel(1, 37),
             HealpixPixel(1, 40),
             HealpixPixel(1, 42),
             HealpixPixel(1, 43),
@@ -48,15 +51,15 @@
             HealpixPixel(1, 47),
         ]
     )
 
 
 @pytest.fixture
 def aligned_trees_2_3_inner():
-    return PixelTreeBuilder.from_healpix(
+    return PixelTree.from_healpix(
         [
             HealpixPixel(1, 33),
             HealpixPixel(1, 35),
             HealpixPixel(1, 40),
             HealpixPixel(1, 42),
             HealpixPixel(1, 43),
             HealpixPixel(1, 44),
@@ -66,15 +69,15 @@
             HealpixPixel(2, 131),
         ]
     )
 
 
 @pytest.fixture
 def aligned_trees_2_3_left():
-    return PixelTreeBuilder.from_healpix(
+    return PixelTree.from_healpix(
         [
             HealpixPixel(1, 33),
             HealpixPixel(1, 35),
             HealpixPixel(1, 40),
             HealpixPixel(1, 41),
             HealpixPixel(1, 42),
             HealpixPixel(1, 43),
@@ -86,15 +89,15 @@
             HealpixPixel(2, 131),
         ]
     )
 
 
 @pytest.fixture
 def aligned_trees_2_3_right():
-    return PixelTreeBuilder.from_healpix(
+    return PixelTree.from_healpix(
         [
             HealpixPixel(1, 33),
             HealpixPixel(1, 34),
             HealpixPixel(1, 35),
             HealpixPixel(1, 36),
             HealpixPixel(1, 37),
             HealpixPixel(1, 40),
@@ -109,15 +112,15 @@
             HealpixPixel(2, 131),
         ]
     )
 
 
 @pytest.fixture
 def aligned_trees_2_3_outer():
-    return PixelTreeBuilder.from_healpix(
+    return PixelTree.from_healpix(
         [
             HealpixPixel(1, 33),
             HealpixPixel(1, 34),
             HealpixPixel(1, 35),
             HealpixPixel(1, 36),
             HealpixPixel(1, 37),
             HealpixPixel(1, 40),
```

### Comparing `hipscat-0.3.0/tests/hipscat/pixel_tree/test_pixel_tree.py` & `hipscat-0.3.1/tests/hipscat/pixel_tree/test_pixel_tree.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,37 +1,54 @@
+import numpy as np
+
 from hipscat.pixel_math import HealpixPixel
+from hipscat.pixel_math.healpix_pixel import get_higher_order_pixels
 from hipscat.pixel_tree.pixel_tree import PixelTree
-from hipscat.pixel_tree.pixel_tree_builder import PixelTreeBuilder
 
 
 def test_pixel_tree_length():
     lengths = [1, 3, 6]
     orders = [1, 2, 7]
     for order in orders:
         for length in lengths:
             hp_pixels = [(order, i) for i in range(length)]
-            tree = PixelTreeBuilder.from_healpix(hp_pixels)
+            tree = PixelTree.from_healpix(hp_pixels)
             assert len(tree) == length
 
 
+def test_get_healpix_pixels(pixel_tree_2, pixel_tree_2_pixels):
+    assert pixel_tree_2.get_healpix_pixels() == pixel_tree_2_pixels
+
+
 def test_pixel_tree_max_depth(pixel_tree_1, pixel_tree_2, pixel_tree_3):
     assert pixel_tree_1.get_max_depth() == 0
     assert pixel_tree_2.get_max_depth() == 2
     assert pixel_tree_3.get_max_depth() == 1
 
 
 def test_pixel_tree_different_tree_order(pixel_tree_2):
     pixel_tree_2_order_5 = PixelTree.from_healpix(pixel_tree_2.get_healpix_pixels(), tree_order=5)
     assert pixel_tree_2_order_5.get_max_depth() == 2
     assert pixel_tree_2_order_5.tree_order == 5
-    assert all(pixel_tree_2_order_5.get_healpix_pixels() == pixel_tree_2.get_healpix_pixels())
+    assert pixel_tree_2_order_5.get_healpix_pixels() == pixel_tree_2.get_healpix_pixels()
+
+
+def test_pixel_tree_to_moc(pixel_tree_2):
+    moc = pixel_tree_2.to_moc()
+    moc_order_pixels = np.concatenate(
+        [
+            get_higher_order_pixels(pixel.order, pixel.pixel, moc.max_order - pixel.order)
+            for pixel in pixel_tree_2.get_healpix_pixels()
+        ]
+    )
+    assert np.all(moc.flatten() == moc_order_pixels)
 
 
 def test_pixel_tree_contains():
-    tree = PixelTreeBuilder.from_healpix([(0, 0)])
+    tree = PixelTree.from_healpix([(0, 0)])
     assert tree.contains((0, 0))
     assert tree.contains(HealpixPixel(0, 0))
     assert (0, 0) in tree
     assert HealpixPixel(0, 0) in tree
     assert not tree.contains((1, 1))
     assert not tree.contains(HealpixPixel(1, 1))
     assert (1, 1) not in tree
```

### Comparing `hipscat-0.3.0/tests/hipscat/pixel_tree/test_pixel_tree_builder.py` & `hipscat-0.3.1/tests/hipscat/pixel_tree/test_pixel_tree_builder.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,60 +1,60 @@
 import pytest
 
 from hipscat.pixel_math import HealpixPixel
-from hipscat.pixel_tree.pixel_tree_builder import PixelTreeBuilder
+from hipscat.pixel_tree.pixel_tree import PixelTree
 
 
 def assert_pixel_tree_has_nodes_in_catalog(tree, catalog):
     """assert tree contains the same nodes as the catalog"""
     for pixel in catalog.get_healpix_pixels():
         assert tree.contains((pixel.order, pixel.pixel))
 
 
 def test_pixel_tree_small_sky(small_sky_catalog):
     """test pixel tree on small sky"""
-    pixel_tree = PixelTreeBuilder.from_healpix(small_sky_catalog.get_healpix_pixels())
+    pixel_tree = PixelTree.from_healpix(small_sky_catalog.get_healpix_pixels())
     assert len(pixel_tree) == len(small_sky_catalog.get_healpix_pixels())
     assert_pixel_tree_has_nodes_in_catalog(pixel_tree, small_sky_catalog)
 
 
 def test_pixel_tree_small_sky_order1(small_sky_order1_catalog):
     """test pixel tree on small sky order1"""
-    pixel_tree = PixelTreeBuilder.from_healpix(small_sky_order1_catalog.get_healpix_pixels())
+    pixel_tree = PixelTree.from_healpix(small_sky_order1_catalog.get_healpix_pixels())
     assert_pixel_tree_has_nodes_in_catalog(pixel_tree, small_sky_order1_catalog)
 
 
 def test_pixel_tree_small_sky_from_list(small_sky_catalog, small_sky_pixels):
     """test pixel tree on small sky"""
-    pixel_tree = PixelTreeBuilder.from_healpix(small_sky_pixels)
+    pixel_tree = PixelTree.from_healpix(small_sky_pixels)
     assert len(pixel_tree) == len(small_sky_pixels)
     assert_pixel_tree_has_nodes_in_catalog(pixel_tree, small_sky_catalog)
 
 
 def test_pixel_tree_small_sky_order1_from_list(small_sky_order1_catalog, small_sky_order1_pixels):
     """test pixel tree on small sky order1"""
-    pixel_tree = PixelTreeBuilder.from_healpix(small_sky_order1_pixels)
+    pixel_tree = PixelTree.from_healpix(small_sky_order1_pixels)
     assert_pixel_tree_has_nodes_in_catalog(pixel_tree, small_sky_order1_catalog)
 
 
 def test_duplicate_pixel_raises_error():
     """test pixel tree raises error with duplicate pixels"""
     partition_info = [
         HealpixPixel(0, 11),
     ]
-    PixelTreeBuilder.from_healpix(partition_info)
+    PixelTree.from_healpix(partition_info)
     info_with_duplicate = [
         HealpixPixel(0, 11),
         HealpixPixel(0, 11),
     ]
     with pytest.raises(ValueError):
-        PixelTreeBuilder.from_healpix(info_with_duplicate)
+        PixelTree.from_healpix(info_with_duplicate)
 
 
 def test_pixel_duplicated_at_different_order_raises_error():
     """test pixel tree raises error with duplicate pixels at different orders"""
     info_with_duplicate = [
         HealpixPixel(0, 11),
         HealpixPixel(1, 44),  # overlaps with (0,11)
     ]
     with pytest.raises(ValueError):
-        PixelTreeBuilder.from_healpix(info_with_duplicate)
+        PixelTree.from_healpix(info_with_duplicate)
```

