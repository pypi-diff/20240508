# Comparing `tmp/depthcharge_ms-0.4.5.tar.gz` & `tmp/depthcharge_ms-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "depthcharge_ms-0.4.5.tar", last modified: Tue Apr 30 18:08:33 2024, max compression
+gzip compressed data, was "depthcharge_ms-0.4.6.tar", last modified: Wed May  8 06:00:31 2024, max compression
```

## Comparing `depthcharge_ms-0.4.5.tar` & `depthcharge_ms-0.4.6.tar`

### file list

```diff
@@ -1,99 +1,99 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:08:33.714477 depthcharge_ms-0.4.5/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:08:33.694477 depthcharge_ms-0.4.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:08:33.698477 depthcharge_ms-0.4.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-04-30 18:08:21.000000 depthcharge_ms-0.4.5/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-30 18:08:21.000000 depthcharge_ms-0.4.5/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-30 18:08:21.000000 depthcharge_ms-0.4.5/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-30 18:08:21.000000 depthcharge_ms-0.4.5/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-30 18:08:21.000000 depthcharge_ms-0.4.5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5530 2024-04-30 18:08:21.000000 depthcharge_ms-0.4.5/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     4973 2024-04-30 18:08:21.000000 depthcharge_ms-0.4.5/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     3921 2024-04-30 18:08:21.000000 depthcharge_ms-0.4.5/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-30 18:08:21.000000 depthcharge_ms-0.4.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-04-30 18:08:33.714477 depthcharge_ms-0.4.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-30 18:08:21.000000 depthcharge_ms-0.4.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-30 18:08:21.000000 depthcharge_ms-0.4.5/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:08:33.702477 depthcharge_ms-0.4.5/data/
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-30 18:08:21.000000 depthcharge_ms-0.4.5/data/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    12882 2024-04-30 18:08:21.000000 depthcharge_ms-0.4.5/data/TMT10-Trial-8.mgf
--rw-r--r--   0 runner    (1001) docker     (127)   333839 2024-04-30 18:08:21.000000 depthcharge_ms-0.4.5/data/TMT10-Trial-8.mzML
--rw-r--r--   0 runner    (1001) docker     (127)    67798 2024-04-30 18:08:21.000000 depthcharge_ms-0.4.5/data/TMT10-Trial-8.mzXML
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:08:33.702477 depthcharge_ms-0.4.5/depthcharge/
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-30 18:08:21.000000 depthcharge_ms-0.4.5/depthcharge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-30 18:08:21.000000 depthcharge_ms-0.4.5/depthcharge/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:08:33.702477 depthcharge_ms-0.4.5/depthcharge/data/
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-30 18:08:21.000000 depthcharge_ms-0.4.5/depthcharge/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-04-30 18:08:21.000000 depthcharge_ms-0.4.5/depthcharge/data/analyte_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)    12035 2024-04-30 18:08:21.000000 depthcharge_ms-0.4.5/depthcharge/data/arrow.py
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-04-30 18:08:21.000000 depthcharge_ms-0.4.5/depthcharge/data/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)    18146 2024-04-30 18:08:21.000000 depthcharge_ms-0.4.5/depthcharge/data/parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-04-30 18:08:21.000000 depthcharge_ms-0.4.5/depthcharge/data/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)    18668 2024-04-30 18:08:21.000000 depthcharge_ms-0.4.5/depthcharge/data/spectrum_datasets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:08:33.702477 depthcharge_ms-0.4.5/depthcharge/encoders/
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-30 18:08:21.000000 depthcharge_ms-0.4.5/depthcharge/encoders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6969 2024-04-30 18:08:21.000000 depthcharge_ms-0.4.5/depthcharge/encoders/sinusoidal.py
--rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-04-30 18:08:21.000000 depthcharge_ms-0.4.5/depthcharge/feedforward.py
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-04-30 18:08:21.000000 depthcharge_ms-0.4.5/depthcharge/mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)    12517 2024-04-30 18:08:21.000000 depthcharge_ms-0.4.5/depthcharge/primitives.py
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-04-30 18:08:21.000000 depthcharge_ms-0.4.5/depthcharge/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:08:33.706477 depthcharge_ms-0.4.5/depthcharge/tokenizers/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-30 18:08:21.000000 depthcharge_ms-0.4.5/depthcharge/tokenizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3996 2024-04-30 18:08:21.000000 depthcharge_ms-0.4.5/depthcharge/tokenizers/molecules.py
--rw-r--r--   0 runner    (1001) docker     (127)    10042 2024-04-30 18:08:21.000000 depthcharge_ms-0.4.5/depthcharge/tokenizers/peptides.py
--rw-r--r--   0 runner    (1001) docker     (127)     4948 2024-04-30 18:08:21.000000 depthcharge_ms-0.4.5/depthcharge/tokenizers/tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:08:33.706477 depthcharge_ms-0.4.5/depthcharge/transformers/
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-30 18:08:21.000000 depthcharge_ms-0.4.5/depthcharge/transformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17251 2024-04-30 18:08:21.000000 depthcharge_ms-0.4.5/depthcharge/transformers/analytes.py
--rw-r--r--   0 runner    (1001) docker     (127)     6812 2024-04-30 18:08:21.000000 depthcharge_ms-0.4.5/depthcharge/transformers/spectra.py
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-30 18:08:21.000000 depthcharge_ms-0.4.5/depthcharge/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-30 18:08:21.000000 depthcharge_ms-0.4.5/depthcharge/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:08:33.710477 depthcharge_ms-0.4.5/depthcharge_ms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-04-30 18:08:33.000000 depthcharge_ms-0.4.5/depthcharge_ms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-04-30 18:08:33.000000 depthcharge_ms-0.4.5/depthcharge_ms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 18:08:33.000000 depthcharge_ms-0.4.5/depthcharge_ms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-30 18:08:33.000000 depthcharge_ms-0.4.5/depthcharge_ms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-30 18:08:33.000000 depthcharge_ms-0.4.5/depthcharge_ms.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:08:33.706477 depthcharge_ms-0.4.5/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     5530 2024-04-30 18:08:21.000000 depthcharge_ms-0.4.5/docs/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     4973 2024-04-30 18:08:21.000000 depthcharge_ms-0.4.5/docs/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     3921 2024-04-30 18:08:21.000000 depthcharge_ms-0.4.5/docs/CONTRIBUTING.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:08:33.706477 depthcharge_ms-0.4.5/docs/api/
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-30 18:08:21.000000 depthcharge_ms-0.4.5/docs/api/datasets.md
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-30 18:08:21.000000 depthcharge_ms-0.4.5/docs/api/encoders.md
--rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-04-30 18:08:21.000000 depthcharge_ms-0.4.5/docs/api/index.md
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-30 18:08:21.000000 depthcharge_ms-0.4.5/docs/api/primitives.md
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-30 18:08:21.000000 depthcharge_ms-0.4.5/docs/api/tokenizers.md
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-30 18:08:21.000000 depthcharge_ms-0.4.5/docs/api/transformers.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:08:33.710477 depthcharge_ms-0.4.5/docs/getting-started/
--rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-04-30 18:08:21.000000 depthcharge_ms-0.4.5/docs/getting-started/installation.md
--rw-r--r--   0 runner    (1001) docker     (127)    10048 2024-04-30 18:08:21.000000 depthcharge_ms-0.4.5/docs/getting-started/spectra.qmd
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-30 18:08:21.000000 depthcharge_ms-0.4.5/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:08:33.710477 depthcharge_ms-0.4.5/docs/stylesheets/
--rw-r--r--   0 runner    (1001) docker     (127)     3353 2024-04-30 18:08:21.000000 depthcharge_ms-0.4.5/docs/stylesheets/extra.css
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-04-30 18:08:21.000000 depthcharge_ms-0.4.5/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-04-30 18:08:21.000000 depthcharge_ms-0.4.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 18:08:33.714477 depthcharge_ms-0.4.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:08:33.710477 depthcharge_ms-0.4.5/static/
--rw-r--r--   0 runner    (1001) docker     (127)    15364 2024-04-30 18:08:21.000000 depthcharge_ms-0.4.5/static/icon.svg
--rw-r--r--   0 runner    (1001) docker     (127)    50058 2024-04-30 18:08:21.000000 depthcharge_ms-0.4.5/static/logo-dark.png
--rw-r--r--   0 runner    (1001) docker     (127)    46385 2024-04-30 18:08:21.000000 depthcharge_ms-0.4.5/static/logo-light.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:08:33.710477 depthcharge_ms-0.4.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3757 2024-04-30 18:08:21.000000 depthcharge_ms-0.4.5/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:08:33.710477 depthcharge_ms-0.4.5/tests/unit_tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:08:33.710477 depthcharge_ms-0.4.5/tests/unit_tests/test_data/
--rw-r--r--   0 runner    (1001) docker     (127)     3284 2024-04-30 18:08:21.000000 depthcharge_ms-0.4.5/tests/unit_tests/test_data/test_arrow.py
--rw-r--r--   0 runner    (1001) docker     (127)     6367 2024-04-30 18:08:21.000000 depthcharge_ms-0.4.5/tests/unit_tests/test_data/test_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-04-30 18:08:21.000000 depthcharge_ms-0.4.5/tests/unit_tests/test_data/test_loaders.py
--rw-r--r--   0 runner    (1001) docker     (127)     5886 2024-04-30 18:08:21.000000 depthcharge_ms-0.4.5/tests/unit_tests/test_data/test_parsers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:08:33.710477 depthcharge_ms-0.4.5/tests/unit_tests/test_encoders/
--rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-04-30 18:08:21.000000 depthcharge_ms-0.4.5/tests/unit_tests/test_encoders/test_sinusoidal.py
--rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-04-30 18:08:21.000000 depthcharge_ms-0.4.5/tests/unit_tests/test_feedforward.py
--rw-r--r--   0 runner    (1001) docker     (127)     3666 2024-04-30 18:08:21.000000 depthcharge_ms-0.4.5/tests/unit_tests/test_primitives.py
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-30 18:08:21.000000 depthcharge_ms-0.4.5/tests/unit_tests/test_testing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:08:33.710477 depthcharge_ms-0.4.5/tests/unit_tests/test_tokenizers/
--rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-04-30 18:08:21.000000 depthcharge_ms-0.4.5/tests/unit_tests/test_tokenizers/test_molecules.py
--rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-04-30 18:08:21.000000 depthcharge_ms-0.4.5/tests/unit_tests/test_tokenizers/test_peptides.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:08:33.710477 depthcharge_ms-0.4.5/tests/unit_tests/test_transformers/
--rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-04-30 18:08:21.000000 depthcharge_ms-0.4.5/tests/unit_tests/test_transformers/test_analyte_transformers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-04-30 18:08:21.000000 depthcharge_ms-0.4.5/tests/unit_tests/test_transformers/test_spectrum_transformers.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-30 18:08:21.000000 depthcharge_ms-0.4.5/tests/unit_tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:00:31.304104 depthcharge_ms-0.4.6/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:00:31.288104 depthcharge_ms-0.4.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:00:31.292104 depthcharge_ms-0.4.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5653 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4973 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3921 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-08 06:00:31.304104 depthcharge_ms-0.4.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:00:31.292104 depthcharge_ms-0.4.6/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/data/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    12882 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/data/TMT10-Trial-8.mgf
+-rw-r--r--   0 runner    (1001) docker     (127)   333839 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/data/TMT10-Trial-8.mzML
+-rw-r--r--   0 runner    (1001) docker     (127)    67798 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/data/TMT10-Trial-8.mzXML
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:00:31.296105 depthcharge_ms-0.4.6/depthcharge/
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/depthcharge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/depthcharge/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:00:31.296105 depthcharge_ms-0.4.6/depthcharge/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/depthcharge/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/depthcharge/data/analyte_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12035 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/depthcharge/data/arrow.py
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/depthcharge/data/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18146 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/depthcharge/data/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/depthcharge/data/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18668 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/depthcharge/data/spectrum_datasets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:00:31.296105 depthcharge_ms-0.4.6/depthcharge/encoders/
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/depthcharge/encoders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6969 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/depthcharge/encoders/sinusoidal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/depthcharge/feedforward.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/depthcharge/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12905 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/depthcharge/primitives.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/depthcharge/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:00:31.296105 depthcharge_ms-0.4.6/depthcharge/tokenizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/depthcharge/tokenizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3996 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/depthcharge/tokenizers/molecules.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10042 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/depthcharge/tokenizers/peptides.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4948 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/depthcharge/tokenizers/tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:00:31.296105 depthcharge_ms-0.4.6/depthcharge/transformers/
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/depthcharge/transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17251 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/depthcharge/transformers/analytes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6812 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/depthcharge/transformers/spectra.py
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/depthcharge/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/depthcharge/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:00:31.304104 depthcharge_ms-0.4.6/depthcharge_ms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-08 06:00:31.000000 depthcharge_ms-0.4.6/depthcharge_ms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-05-08 06:00:31.000000 depthcharge_ms-0.4.6/depthcharge_ms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 06:00:31.000000 depthcharge_ms-0.4.6/depthcharge_ms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-08 06:00:31.000000 depthcharge_ms-0.4.6/depthcharge_ms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-08 06:00:31.000000 depthcharge_ms-0.4.6/depthcharge_ms.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:00:31.300104 depthcharge_ms-0.4.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     5653 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/docs/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4973 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/docs/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3921 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/docs/CONTRIBUTING.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:00:31.300104 depthcharge_ms-0.4.6/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/docs/api/datasets.md
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/docs/api/encoders.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/docs/api/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/docs/api/primitives.md
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/docs/api/tokenizers.md
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/docs/api/transformers.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:00:31.300104 depthcharge_ms-0.4.6/docs/getting-started/
+-rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/docs/getting-started/installation.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10048 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/docs/getting-started/spectra.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:00:31.300104 depthcharge_ms-0.4.6/docs/stylesheets/
+-rw-r--r--   0 runner    (1001) docker     (127)     3353 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/docs/stylesheets/extra.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 06:00:31.304104 depthcharge_ms-0.4.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:00:31.300104 depthcharge_ms-0.4.6/static/
+-rw-r--r--   0 runner    (1001) docker     (127)    15364 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/static/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    50058 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/static/logo-dark.png
+-rw-r--r--   0 runner    (1001) docker     (127)    46385 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/static/logo-light.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:00:31.300104 depthcharge_ms-0.4.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3757 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:00:31.300104 depthcharge_ms-0.4.6/tests/unit_tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:00:31.304104 depthcharge_ms-0.4.6/tests/unit_tests/test_data/
+-rw-r--r--   0 runner    (1001) docker     (127)     3284 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/tests/unit_tests/test_data/test_arrow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6367 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/tests/unit_tests/test_data/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/tests/unit_tests/test_data/test_loaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5886 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/tests/unit_tests/test_data/test_parsers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:00:31.304104 depthcharge_ms-0.4.6/tests/unit_tests/test_encoders/
+-rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/tests/unit_tests/test_encoders/test_sinusoidal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/tests/unit_tests/test_feedforward.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/tests/unit_tests/test_primitives.py
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/tests/unit_tests/test_testing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:00:31.304104 depthcharge_ms-0.4.6/tests/unit_tests/test_tokenizers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/tests/unit_tests/test_tokenizers/test_molecules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3458 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/tests/unit_tests/test_tokenizers/test_peptides.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:00:31.304104 depthcharge_ms-0.4.6/tests/unit_tests/test_transformers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/tests/unit_tests/test_transformers/test_analyte_transformers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/tests/unit_tests/test_transformers/test_spectrum_transformers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/tests/unit_tests/test_version.py
```

### Comparing `depthcharge_ms-0.4.5/.github/workflows/docs.yml` & `depthcharge_ms-0.4.6/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.5/.github/workflows/lint.yml` & `depthcharge_ms-0.4.6/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.5/.github/workflows/publish.yml` & `depthcharge_ms-0.4.6/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.5/.github/workflows/tests.yml` & `depthcharge_ms-0.4.6/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.5/CHANGELOG.md` & `depthcharge_ms-0.4.6/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,18 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [v0.4.6]
+### Added
+- Added support for unsigned modification masses that don't quite conform to the Proforma standard.
+
 ## [v0.4.5]
 ### Changed
 - The `scan_id` column for parsed spectra is not a sting instead of an integer. This is less space efficient, but we ran into issues with Sciex indexing when trying to use only an integer.
 
 ## [v0.4.4]
 
 ### Changed
```

### Comparing `depthcharge_ms-0.4.5/CODE_OF_CONDUCT.md` & `depthcharge_ms-0.4.6/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.5/CONTRIBUTING.md` & `depthcharge_ms-0.4.6/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.5/LICENSE` & `depthcharge_ms-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.5/PKG-INFO` & `depthcharge_ms-0.4.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: depthcharge-ms
-Version: 0.4.5
+Version: 0.4.6
 Summary: A mass spectrometry toolkit for deep learning with Transformer models.
 Author-email: "William E. Fondrie" <fondriew@gmail.com>
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/wfondrie/depthcharge
 Project-URL: Documentation, https://wfondrie.github.io/depthcharge
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -13,28 +13,29 @@
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: torch>=2.0.0
 Requires-Dist: polars>=0.19.0
 Requires-Dist: pyarrow>=12.0.1
 Requires-Dist: pylance>=0.7.5
-Requires-Dist: pyteomics>=4.4.2
+Requires-Dist: pyteomics>=4.7.2
 Requires-Dist: numpy>=1.18.1
 Requires-Dist: numba>=0.48.0
 Requires-Dist: lxml>=4.9.1
 Requires-Dist: einops>=0.4.1
 Requires-Dist: tqdm>=4.65.0
 Requires-Dist: lark>=1.1.4
 Requires-Dist: selfies>=2.1.1
 Requires-Dist: sortedcontainers>=2.4.0
 Requires-Dist: dill>=0.3.6
 Requires-Dist: rdkit>=2023.03.1
 Requires-Dist: pillow>=9.4.0
 Requires-Dist: spectrum-utils>=0.4.1
 Requires-Dist: cloudpathlib>=0.18.1
+Requires-Dist: psims>=1.3.3
 Provides-Extra: docs
 Requires-Dist: mike; extra == "docs"
 Requires-Dist: mkdocs; extra == "docs"
 Requires-Dist: mkdocs-material; extra == "docs"
 Requires-Dist: mkdocstrings[python]>=0.18; extra == "docs"
 Requires-Dist: mkquartodocs; extra == "docs"
 Provides-Extra: dev
```

### Comparing `depthcharge_ms-0.4.5/README.md` & `depthcharge_ms-0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.5/data/TMT10-Trial-8.mgf` & `depthcharge_ms-0.4.6/data/TMT10-Trial-8.mgf`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.5/data/TMT10-Trial-8.mzML` & `depthcharge_ms-0.4.6/data/TMT10-Trial-8.mzML`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.5/data/TMT10-Trial-8.mzXML` & `depthcharge_ms-0.4.6/data/TMT10-Trial-8.mzXML`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.5/depthcharge/__init__.py` & `depthcharge_ms-0.4.6/depthcharge/__init__.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.5/depthcharge/data/analyte_datasets.py` & `depthcharge_ms-0.4.6/depthcharge/data/analyte_datasets.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.5/depthcharge/data/arrow.py` & `depthcharge_ms-0.4.6/depthcharge/data/arrow.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.5/depthcharge/data/fields.py` & `depthcharge_ms-0.4.6/depthcharge/data/fields.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.5/depthcharge/data/parsers.py` & `depthcharge_ms-0.4.6/depthcharge/data/parsers.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.5/depthcharge/data/preprocessing.py` & `depthcharge_ms-0.4.6/depthcharge/data/preprocessing.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.5/depthcharge/data/spectrum_datasets.py` & `depthcharge_ms-0.4.6/depthcharge/data/spectrum_datasets.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.5/depthcharge/encoders/sinusoidal.py` & `depthcharge_ms-0.4.6/depthcharge/encoders/sinusoidal.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.5/depthcharge/feedforward.py` & `depthcharge_ms-0.4.6/depthcharge/feedforward.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.5/depthcharge/mixins.py` & `depthcharge_ms-0.4.6/depthcharge/mixins.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.5/depthcharge/primitives.py` & `depthcharge_ms-0.4.6/depthcharge/primitives.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from PIL.PngImagePlugin import PngImageFile
 from pyteomics import proforma
 from pyteomics.proforma import GenericModification, MassModification
 from rdkit import Chem
 from rdkit.Chem import Draw
 from spectrum_utils.spectrum import MsmsSpectrum
 
+from . import utils
 from .constants import PROTON
 
 MSKB_TO_UNIMOD = {
     "+42.011": "[Acetyl]-",
     "+43.006": "[Carbamyl]-",
     "-17.027": "[Ammonia-loss]-",
     "+43.006-17.027": "[+25.980265]-",  # Not in Unimod
@@ -68,25 +69,15 @@
 
         # Parse modifications into Pyteomics' format
         parsed = [None] * (len(self.sequence) + 2)
         for idx, mod in enumerate(self.modifications):
             if mod is None:
                 continue
 
-            try:
-                mod = [MassModification(mod)]
-            except ValueError:
-                try:
-                    mod = [GenericModification(mod)]
-                except (AttributeError, TypeError):
-                    pass
-            except TypeError:
-                pass
-
-            parsed[idx] = mod
+            parsed[idx] = [_resolve_mod(m) for m in utils.listify(mod)]
 
         self.modifications = parsed
         n_mod = self.modifications[0]
         c_mod = self.modifications[-1]
 
         self.proforma = proforma.to_proforma(
             sequence=list(zip(self.sequence, self.modifications[1:-1])),
@@ -112,15 +103,15 @@
 
             if len(mods) == 1:
                 try:
                     modstr = f"[{mods[0].name}]"
                 except (AttributeError, ValueError):
                     modstr = f"[{mods[0].mass:+0.6f}]"
             else:
-                modstr = f"[{sum([m.mass for m in mods]):+0.6f}]"
+                modstr = f"[{sum(m.mass for m in mods):+0.6f}]"
 
             if not idx:
                 out.append(f"{modstr}-")
             else:
                 out.append(f"{aa}{modstr}")
 
         return out
@@ -440,7 +431,34 @@
         Returns
         -------
         torch.tensor of shape (n_peaks, 2)
             The mass spectrum information.
 
         """
         return torch.tensor(np.vstack([self.mz, self.intensity]).T)
+
+
+def _resolve_mod(
+    mod: MassModification | GenericModification | str | float,
+) -> MassModification | GenericModification:
+    """Resolve the type of a modification.
+
+    Parameters
+    ----------
+    mod : MassModification, GenericModification, str, or float
+        The modification to resolve.
+
+    Returns
+    -------
+    MassModification or GenericModification
+        The best modification for the input type.
+
+    """
+    try:
+        mod = mod.value
+    except AttributeError:
+        pass
+
+    try:
+        return MassModification(float(mod))
+    except ValueError:
+        return GenericModification(str(mod))
```

### Comparing `depthcharge_ms-0.4.5/depthcharge/testing.py` & `depthcharge_ms-0.4.6/depthcharge/testing.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.5/depthcharge/tokenizers/molecules.py` & `depthcharge_ms-0.4.6/depthcharge/tokenizers/molecules.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.5/depthcharge/tokenizers/peptides.py` & `depthcharge_ms-0.4.6/depthcharge/tokenizers/peptides.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.5/depthcharge/tokenizers/tokenizer.py` & `depthcharge_ms-0.4.6/depthcharge/tokenizers/tokenizer.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.5/depthcharge/transformers/analytes.py` & `depthcharge_ms-0.4.6/depthcharge/transformers/analytes.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.5/depthcharge/transformers/spectra.py` & `depthcharge_ms-0.4.6/depthcharge/transformers/spectra.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.5/depthcharge/utils.py` & `depthcharge_ms-0.4.6/depthcharge/utils.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.5/depthcharge_ms.egg-info/PKG-INFO` & `depthcharge_ms-0.4.6/depthcharge_ms.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: depthcharge-ms
-Version: 0.4.5
+Version: 0.4.6
 Summary: A mass spectrometry toolkit for deep learning with Transformer models.
 Author-email: "William E. Fondrie" <fondriew@gmail.com>
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/wfondrie/depthcharge
 Project-URL: Documentation, https://wfondrie.github.io/depthcharge
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -13,28 +13,29 @@
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: torch>=2.0.0
 Requires-Dist: polars>=0.19.0
 Requires-Dist: pyarrow>=12.0.1
 Requires-Dist: pylance>=0.7.5
-Requires-Dist: pyteomics>=4.4.2
+Requires-Dist: pyteomics>=4.7.2
 Requires-Dist: numpy>=1.18.1
 Requires-Dist: numba>=0.48.0
 Requires-Dist: lxml>=4.9.1
 Requires-Dist: einops>=0.4.1
 Requires-Dist: tqdm>=4.65.0
 Requires-Dist: lark>=1.1.4
 Requires-Dist: selfies>=2.1.1
 Requires-Dist: sortedcontainers>=2.4.0
 Requires-Dist: dill>=0.3.6
 Requires-Dist: rdkit>=2023.03.1
 Requires-Dist: pillow>=9.4.0
 Requires-Dist: spectrum-utils>=0.4.1
 Requires-Dist: cloudpathlib>=0.18.1
+Requires-Dist: psims>=1.3.3
 Provides-Extra: docs
 Requires-Dist: mike; extra == "docs"
 Requires-Dist: mkdocs; extra == "docs"
 Requires-Dist: mkdocs-material; extra == "docs"
 Requires-Dist: mkdocstrings[python]>=0.18; extra == "docs"
 Requires-Dist: mkquartodocs; extra == "docs"
 Provides-Extra: dev
```

### Comparing `depthcharge_ms-0.4.5/depthcharge_ms.egg-info/SOURCES.txt` & `depthcharge_ms-0.4.6/depthcharge_ms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.5/docs/CHANGELOG.md` & `depthcharge_ms-0.4.6/docs/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,18 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [v0.4.6]
+### Added
+- Added support for unsigned modification masses that don't quite conform to the Proforma standard.
+
 ## [v0.4.5]
 ### Changed
 - The `scan_id` column for parsed spectra is not a sting instead of an integer. This is less space efficient, but we ran into issues with Sciex indexing when trying to use only an integer.
 
 ## [v0.4.4]
 
 ### Changed
```

### Comparing `depthcharge_ms-0.4.5/docs/CODE_OF_CONDUCT.md` & `depthcharge_ms-0.4.6/docs/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.5/docs/CONTRIBUTING.md` & `depthcharge_ms-0.4.6/docs/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.5/docs/api/index.md` & `depthcharge_ms-0.4.6/docs/api/index.md`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.5/docs/getting-started/installation.md` & `depthcharge_ms-0.4.6/docs/getting-started/installation.md`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.5/docs/getting-started/spectra.qmd` & `depthcharge_ms-0.4.6/docs/getting-started/spectra.qmd`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.5/docs/index.md` & `depthcharge_ms-0.4.6/docs/index.md`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.5/docs/stylesheets/extra.css` & `depthcharge_ms-0.4.6/docs/stylesheets/extra.css`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.5/mkdocs.yml` & `depthcharge_ms-0.4.6/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.5/pyproject.toml` & `depthcharge_ms-0.4.6/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -15,28 +15,29 @@
 ]
 requires-python = ">=3.10"
 dependencies = [
     "torch>=2.0.0",
     "polars>=0.19.0",
     "pyarrow>=12.0.1",
     "pylance>=0.7.5",
-    "pyteomics>=4.4.2",
+    "pyteomics>=4.7.2",
     "numpy>=1.18.1",
     "numba>=0.48.0",
     "lxml>=4.9.1",
     "einops>=0.4.1",
     "tqdm>=4.65.0",
     "lark>=1.1.4",
     "selfies>=2.1.1",
     "sortedcontainers>=2.4.0",
     "dill>=0.3.6",
     "rdkit>=2023.03.1",
     "pillow>=9.4.0",
     "spectrum-utils>=0.4.1",
     "cloudpathlib>=0.18.1",
+    "psims>=1.3.3"
 ]
 dynamic = ["version"]
 
 [project.readme]
 file = "REAMDE.md"
 content-type = "text/markdown"
```

### Comparing `depthcharge_ms-0.4.5/static/icon.svg` & `depthcharge_ms-0.4.6/static/icon.svg`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.5/static/logo-dark.png` & `depthcharge_ms-0.4.6/static/logo-dark.png`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.5/static/logo-light.png` & `depthcharge_ms-0.4.6/static/logo-light.png`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.5/tests/conftest.py` & `depthcharge_ms-0.4.6/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.5/tests/unit_tests/test_data/test_arrow.py` & `depthcharge_ms-0.4.6/tests/unit_tests/test_data/test_arrow.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.5/tests/unit_tests/test_data/test_datasets.py` & `depthcharge_ms-0.4.6/tests/unit_tests/test_data/test_datasets.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.5/tests/unit_tests/test_data/test_loaders.py` & `depthcharge_ms-0.4.6/tests/unit_tests/test_data/test_loaders.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.5/tests/unit_tests/test_data/test_parsers.py` & `depthcharge_ms-0.4.6/tests/unit_tests/test_data/test_parsers.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.5/tests/unit_tests/test_encoders/test_sinusoidal.py` & `depthcharge_ms-0.4.6/tests/unit_tests/test_encoders/test_sinusoidal.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.5/tests/unit_tests/test_feedforward.py` & `depthcharge_ms-0.4.6/tests/unit_tests/test_feedforward.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.5/tests/unit_tests/test_primitives.py` & `depthcharge_ms-0.4.6/tests/unit_tests/test_primitives.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,14 +46,20 @@
         "E[Phospho]",
         "K",
     ]
     parsed = Peptide(peptide, mods)
     assert parsed.split() == expected
 
 
+def test_almost_proforma():
+    """Test a peptide lacking an explicit sign."""
+    parsed = Peptide.from_proforma("LES[79.0]LIEK")
+    assert parsed.split() == ["L", "E", "S[+79.000000]", "L", "I", "E", "K"]
+
+
 def test_peptide_from_proforma():
     """Test proforma parsing."""
     parsed = Peptide.from_proforma("LESLIEK/2")
     assert parsed.split() == list("LESLIEK")
     assert parsed.charge == 2
 
     parsed = Peptide.from_proforma("<[Phospho]@C,T>CAT")
```

### Comparing `depthcharge_ms-0.4.5/tests/unit_tests/test_testing.py` & `depthcharge_ms-0.4.6/tests/unit_tests/test_testing.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.5/tests/unit_tests/test_tokenizers/test_molecules.py` & `depthcharge_ms-0.4.6/tests/unit_tests/test_tokenizers/test_molecules.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.5/tests/unit_tests/test_tokenizers/test_peptides.py` & `depthcharge_ms-0.4.6/tests/unit_tests/test_tokenizers/test_peptides.py`

 * *Files 4% similar despite different names*

```diff
@@ -105,7 +105,13 @@
     tokenizer = PeptideTokenizer.from_proforma("[+10]-EDITHR")
     out = tokenizer.tokenize("LESLIEK")
     assert out.shape == (1, 7)
 
     ion = tokenizer.calculate_precursor_ions("LESLIEK", 2)
     expected = mass.fast_mass("LESLIEK", charge=2, ion_type="M")
     torch.testing.assert_close(ion, torch.tensor([expected]))
+
+
+def test_almost_compliant_proform():
+    """Test initializing with a peptide without an expicit mass sign."""
+    tokenizer = PeptideTokenizer.from_proforma("[10]-EDITHR")
+    assert "[+10.000000]-" in tokenizer.residues
```

### Comparing `depthcharge_ms-0.4.5/tests/unit_tests/test_transformers/test_analyte_transformers.py` & `depthcharge_ms-0.4.6/tests/unit_tests/test_transformers/test_analyte_transformers.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.5/tests/unit_tests/test_transformers/test_spectrum_transformers.py` & `depthcharge_ms-0.4.6/tests/unit_tests/test_transformers/test_spectrum_transformers.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.5/tests/unit_tests/test_version.py` & `depthcharge_ms-0.4.6/tests/unit_tests/test_version.py`

 * *Files identical despite different names*

