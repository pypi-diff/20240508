# Comparing `tmp/invenio-records-rest-2.4.0.tar.gz` & `tmp/invenio-records-rest-2.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/invenio-records-rest-2.4.0.tar", last modified: Fri Dec  8 12:28:50 2023, max compression
+gzip compressed data, was "dist/invenio-records-rest-2.4.1.tar", last modified: Wed May  8 08:44:21 2024, max compression
```

## Comparing `invenio-records-rest-2.4.0.tar` & `invenio-records-rest-2.4.1.tar`

### file list

```diff
@@ -1,142 +1,142 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 12:28:50.000000 invenio-records-rest-2.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2023-12-08 12:28:39.000000 invenio-records-rest-2.4.0/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (127)      666 2023-12-08 12:28:39.000000 invenio-records-rest-2.4.0/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (127)       41 2023-12-08 12:28:39.000000 invenio-records-rest-2.4.0/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 12:28:50.000000 invenio-records-rest-2.4.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 12:28:50.000000 invenio-records-rest-2.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      824 2023-12-08 12:28:39.000000 invenio-records-rest-2.4.0/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2581 2023-12-08 12:28:39.000000 invenio-records-rest-2.4.0/.github/workflows/tests.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 12:28:50.000000 invenio-records-rest-2.4.0/.tx/
--rw-r--r--   0 runner    (1001) docker     (127)      479 2023-12-08 12:28:39.000000 invenio-records-rest-2.4.0/.tx/config
--rw-r--r--   0 runner    (1001) docker     (127)      715 2023-12-08 12:28:39.000000 invenio-records-rest-2.4.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4725 2023-12-08 12:28:39.000000 invenio-records-rest-2.4.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3785 2023-12-08 12:28:39.000000 invenio-records-rest-2.4.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)      362 2023-12-08 12:28:39.000000 invenio-records-rest-2.4.0/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2023-12-08 12:28:39.000000 invenio-records-rest-2.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      803 2023-12-08 12:28:39.000000 invenio-records-rest-2.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8032 2023-12-08 12:28:50.000000 invenio-records-rest-2.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-08 12:28:39.000000 invenio-records-rest-2.4.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      307 2023-12-08 12:28:39.000000 invenio-records-rest-2.4.0/babel.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 12:28:50.000000 invenio-records-rest-2.4.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     7465 2023-12-08 12:28:39.000000 invenio-records-rest-2.4.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     2799 2023-12-08 12:28:39.000000 invenio-records-rest-2.4.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      247 2023-12-08 12:28:39.000000 invenio-records-rest-2.4.0/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (127)      247 2023-12-08 12:28:39.000000 invenio-records-rest-2.4.0/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (127)    10851 2023-12-08 12:28:39.000000 invenio-records-rest-2.4.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      305 2023-12-08 12:28:39.000000 invenio-records-rest-2.4.0/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (127)      252 2023-12-08 12:28:39.000000 invenio-records-rest-2.4.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)      833 2023-12-08 12:28:39.000000 invenio-records-rest-2.4.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      247 2023-12-08 12:28:39.000000 invenio-records-rest-2.4.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      253 2023-12-08 12:28:39.000000 invenio-records-rest-2.4.0/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7009 2023-12-08 12:28:39.000000 invenio-records-rest-2.4.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       65 2023-12-08 12:28:39.000000 invenio-records-rest-2.4.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      269 2023-12-08 12:28:39.000000 invenio-records-rest-2.4.0/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 12:28:50.000000 invenio-records-rest-2.4.0/invenio_records_rest/
--rw-r--r--   0 runner    (1001) docker     (127)    27039 2023-12-08 12:28:39.000000 invenio-records-rest-2.4.0/invenio_records_rest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      954 2023-12-08 12:28:39.000000 invenio-records-rest-2.4.0/invenio_records_rest/_compat.py
--rw-r--r--   0 runner    (1001) docker     (127)    13499 2023-12-08 12:28:39.000000 invenio-records-rest-2.4.0/invenio_records_rest/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4926 2023-12-08 12:28:39.000000 invenio-records-rest-2.4.0/invenio_records_rest/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     3890 2023-12-08 12:28:39.000000 invenio-records-rest-2.4.0/invenio_records_rest/ext.py
--rw-r--r--   0 runner    (1001) docker     (127)     9896 2023-12-08 12:28:39.000000 invenio-records-rest-2.4.0/invenio_records_rest/facets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1546 2023-12-08 12:28:39.000000 invenio-records-rest-2.4.0/invenio_records_rest/links.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 12:28:50.000000 invenio-records-rest-2.4.0/invenio_records_rest/loaders/
--rw-r--r--   0 runner    (1001) docker     (127)      753 2023-12-08 12:28:39.000000 invenio-records-rest-2.4.0/invenio_records_rest/loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3174 2023-12-08 12:28:39.000000 invenio-records-rest-2.4.0/invenio_records_rest/loaders/marshmallow.py
--rw-r--r--   0 runner    (1001) docker     (127)      481 2023-12-08 12:28:39.000000 invenio-records-rest-2.4.0/invenio_records_rest/proxies.py
--rw-r--r--   0 runner    (1001) docker     (127)     1729 2023-12-08 12:28:39.000000 invenio-records-rest-2.4.0/invenio_records_rest/query.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 12:28:50.000000 invenio-records-rest-2.4.0/invenio_records_rest/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)      504 2023-12-08 12:28:39.000000 invenio-records-rest-2.4.0/invenio_records_rest/schemas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 12:28:50.000000 invenio-records-rest-2.4.0/invenio_records_rest/schemas/fields/
--rw-r--r--   0 runner    (1001) docker     (127)      775 2023-12-08 12:28:39.000000 invenio-records-rest-2.4.0/invenio_records_rest/schemas/fields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      871 2023-12-08 12:28:39.000000 invenio-records-rest-2.4.0/invenio_records_rest/schemas/fields/datetime.py
--rw-r--r--   0 runner    (1001) docker     (127)     2539 2023-12-08 12:28:39.000000 invenio-records-rest-2.4.0/invenio_records_rest/schemas/fields/generated.py
--rw-r--r--   0 runner    (1001) docker     (127)     4392 2023-12-08 12:28:39.000000 invenio-records-rest-2.4.0/invenio_records_rest/schemas/fields/marshmallow_contrib.py
--rw-r--r--   0 runner    (1001) docker     (127)      874 2023-12-08 12:28:39.000000 invenio-records-rest-2.4.0/invenio_records_rest/schemas/fields/persistentidentifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2023-12-08 12:28:39.000000 invenio-records-rest-2.4.0/invenio_records_rest/schemas/fields/sanitizedhtml.py
--rw-r--r--   0 runner    (1001) docker     (127)     1427 2023-12-08 12:28:39.000000 invenio-records-rest-2.4.0/invenio_records_rest/schemas/fields/sanitizedunicode.py
--rw-r--r--   0 runner    (1001) docker     (127)      597 2023-12-08 12:28:39.000000 invenio-records-rest-2.4.0/invenio_records_rest/schemas/fields/trimmedstring.py
--rw-r--r--   0 runner    (1001) docker     (127)     3916 2023-12-08 12:28:39.000000 invenio-records-rest-2.4.0/invenio_records_rest/schemas/json.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 12:28:50.000000 invenio-records-rest-2.4.0/invenio_records_rest/serializers/
--rw-r--r--   0 runner    (1001) docker     (127)      732 2023-12-08 12:28:39.000000 invenio-records-rest-2.4.0/invenio_records_rest/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6388 2023-12-08 12:28:39.000000 invenio-records-rest-2.4.0/invenio_records_rest/serializers/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4615 2023-12-08 12:28:39.000000 invenio-records-rest-2.4.0/invenio_records_rest/serializers/citeproc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5431 2023-12-08 12:28:39.000000 invenio-records-rest-2.4.0/invenio_records_rest/serializers/csv.py
--rw-r--r--   0 runner    (1001) docker     (127)     4630 2023-12-08 12:28:39.000000 invenio-records-rest-2.4.0/invenio_records_rest/serializers/datacite.py
--rw-r--r--   0 runner    (1001) docker     (127)     2193 2023-12-08 12:28:39.000000 invenio-records-rest-2.4.0/invenio_records_rest/serializers/dc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2582 2023-12-08 12:28:39.000000 invenio-records-rest-2.4.0/invenio_records_rest/serializers/json.py
--rw-r--r--   0 runner    (1001) docker     (127)     2449 2023-12-08 12:28:39.000000 invenio-records-rest-2.4.0/invenio_records_rest/serializers/jsonld.py
--rw-r--r--   0 runner    (1001) docker     (127)     1865 2023-12-08 12:28:39.000000 invenio-records-rest-2.4.0/invenio_records_rest/serializers/marshmallow.py
--rw-r--r--   0 runner    (1001) docker     (127)     2632 2023-12-08 12:28:39.000000 invenio-records-rest-2.4.0/invenio_records_rest/serializers/response.py
--rw-r--r--   0 runner    (1001) docker     (127)     4429 2023-12-08 12:28:39.000000 invenio-records-rest-2.4.0/invenio_records_rest/sorter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 12:28:50.000000 invenio-records-rest-2.4.0/invenio_records_rest/translations/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 12:28:50.000000 invenio-records-rest-2.4.0/invenio_records_rest/translations/en/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 12:28:50.000000 invenio-records-rest-2.4.0/invenio_records_rest/translations/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      482 2023-12-08 12:28:50.000000 invenio-records-rest-2.4.0/invenio_records_rest/translations/en/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)      892 2023-12-08 12:28:39.000000 invenio-records-rest-2.4.0/invenio_records_rest/translations/en/LC_MESSAGES/messages.po
--rw-r--r--   0 runner    (1001) docker     (127)     8451 2023-12-08 12:28:39.000000 invenio-records-rest-2.4.0/invenio_records_rest/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    35194 2023-12-08 12:28:39.000000 invenio-records-rest-2.4.0/invenio_records_rest/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 12:28:50.000000 invenio-records-rest-2.4.0/invenio_records_rest.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8032 2023-12-08 12:28:50.000000 invenio-records-rest-2.4.0/invenio_records_rest.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3699 2023-12-08 12:28:50.000000 invenio-records-rest-2.4.0/invenio_records_rest.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-08 12:28:50.000000 invenio-records-rest-2.4.0/invenio_records_rest.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      514 2023-12-08 12:28:50.000000 invenio-records-rest-2.4.0/invenio_records_rest.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-08 12:28:50.000000 invenio-records-rest-2.4.0/invenio_records_rest.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      798 2023-12-08 12:28:50.000000 invenio-records-rest-2.4.0/invenio_records_rest.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2023-12-08 12:28:50.000000 invenio-records-rest-2.4.0/invenio_records_rest.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      104 2023-12-08 12:28:39.000000 invenio-records-rest-2.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      857 2023-12-08 12:28:39.000000 invenio-records-rest-2.4.0/requirements-devel.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      778 2023-12-08 12:28:39.000000 invenio-records-rest-2.4.0/run-tests.sh
--rw-r--r--   0 runner    (1001) docker     (127)     2894 2023-12-08 12:28:50.000000 invenio-records-rest-2.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      389 2023-12-08 12:28:39.000000 invenio-records-rest-2.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 12:28:50.000000 invenio-records-rest-2.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     9889 2023-12-08 12:28:39.000000 invenio-records-rest-2.4.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 12:28:50.000000 invenio-records-rest-2.4.0/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)      321 2023-12-08 12:28:39.000000 invenio-records-rest-2.4.0/tests/data/testrecords.json
--rw-r--r--   0 runner    (1001) docker     (127)     2237 2023-12-08 12:28:39.000000 invenio-records-rest-2.4.0/tests/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 12:28:50.000000 invenio-records-rest-2.4.0/tests/mock_module/
--rw-r--r--   0 runner    (1001) docker     (127)      259 2023-12-08 12:28:39.000000 invenio-records-rest-2.4.0/tests/mock_module/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 12:28:50.000000 invenio-records-rest-2.4.0/tests/mock_module/mappings/
--rw-r--r--   0 runner    (1001) docker     (127)      261 2023-12-08 12:28:39.000000 invenio-records-rest-2.4.0/tests/mock_module/mappings/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 12:28:50.000000 invenio-records-rest-2.4.0/tests/mock_module/mappings/os-v1/
--rw-r--r--   0 runner    (1001) docker     (127)      272 2023-12-08 12:28:39.000000 invenio-records-rest-2.4.0/tests/mock_module/mappings/os-v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 12:28:50.000000 invenio-records-rest-2.4.0/tests/mock_module/mappings/os-v1/invenio-records-rest/
--rw-r--r--   0 runner    (1001) docker     (127)      748 2023-12-08 12:28:39.000000 invenio-records-rest-2.4.0/tests/mock_module/mappings/os-v1/invenio-records-rest/testrecord.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 12:28:50.000000 invenio-records-rest-2.4.0/tests/mock_module/mappings/os-v2/
--rw-r--r--   0 runner    (1001) docker     (127)      272 2023-12-08 12:28:39.000000 invenio-records-rest-2.4.0/tests/mock_module/mappings/os-v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 12:28:50.000000 invenio-records-rest-2.4.0/tests/mock_module/mappings/os-v2/invenio-records-rest/
--rw-r--r--   0 runner    (1001) docker     (127)      748 2023-12-08 12:28:39.000000 invenio-records-rest-2.4.0/tests/mock_module/mappings/os-v2/invenio-records-rest/testrecord.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 12:28:50.000000 invenio-records-rest-2.4.0/tests/mock_module/mappings/v7/
--rw-r--r--   0 runner    (1001) docker     (127)      275 2023-12-08 12:28:39.000000 invenio-records-rest-2.4.0/tests/mock_module/mappings/v7/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 12:28:50.000000 invenio-records-rest-2.4.0/tests/mock_module/mappings/v7/invenio-records-rest/
--rw-r--r--   0 runner    (1001) docker     (127)      748 2023-12-08 12:28:39.000000 invenio-records-rest-2.4.0/tests/mock_module/mappings/v7/invenio-records-rest/testrecord.json
--rw-r--r--   0 runner    (1001) docker     (127)     5329 2023-12-08 12:28:39.000000 invenio-records-rest-2.4.0/tests/test_custom_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (127)     5634 2023-12-08 12:28:39.000000 invenio-records-rest-2.4.0/tests/test_custom_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     2352 2023-12-08 12:28:39.000000 invenio-records-rest-2.4.0/tests/test_error_handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)      827 2023-12-08 12:28:39.000000 invenio-records-rest-2.4.0/tests/test_ext.py
--rw-r--r--   0 runner    (1001) docker     (127)     9069 2023-12-08 12:28:39.000000 invenio-records-rest-2.4.0/tests/test_facets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2505 2023-12-08 12:28:39.000000 invenio-records-rest-2.4.0/tests/test_index_prefixing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1994 2023-12-08 12:28:39.000000 invenio-records-rest-2.4.0/tests/test_links.py
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2023-12-08 12:28:39.000000 invenio-records-rest-2.4.0/tests/test_marshmallow_contrib.py
--rw-r--r--   0 runner    (1001) docker     (127)     7058 2023-12-08 12:28:39.000000 invenio-records-rest-2.4.0/tests/test_marshmallow_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2023-12-08 12:28:39.000000 invenio-records-rest-2.4.0/tests/test_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2241 2023-12-08 12:28:39.000000 invenio-records-rest-2.4.0/tests/test_pid_resolver.py
--rw-r--r--   0 runner    (1001) docker     (127)     2385 2023-12-08 12:28:39.000000 invenio-records-rest-2.4.0/tests/test_serializer_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3201 2023-12-08 12:28:39.000000 invenio-records-rest-2.4.0/tests/test_serializer_citeproc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5996 2023-12-08 12:28:39.000000 invenio-records-rest-2.4.0/tests/test_serializer_csv.py
--rw-r--r--   0 runner    (1001) docker     (127)     3034 2023-12-08 12:28:39.000000 invenio-records-rest-2.4.0/tests/test_serializer_datacite.py
--rw-r--r--   0 runner    (1001) docker     (127)     1988 2023-12-08 12:28:39.000000 invenio-records-rest-2.4.0/tests/test_serializer_dc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2929 2023-12-08 12:28:39.000000 invenio-records-rest-2.4.0/tests/test_serializer_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     3382 2023-12-08 12:28:39.000000 invenio-records-rest-2.4.0/tests/test_serializer_jsonld.py
--rw-r--r--   0 runner    (1001) docker     (127)     2066 2023-12-08 12:28:39.000000 invenio-records-rest-2.4.0/tests/test_serializer_marshmallow.py
--rw-r--r--   0 runner    (1001) docker     (127)     1920 2023-12-08 12:28:39.000000 invenio-records-rest-2.4.0/tests/test_serializer_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     5101 2023-12-08 12:28:39.000000 invenio-records-rest-2.4.0/tests/test_sorter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4018 2023-12-08 12:28:39.000000 invenio-records-rest-2.4.0/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2400 2023-12-08 12:28:39.000000 invenio-records-rest-2.4.0/tests/test_views_item_delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     2626 2023-12-08 12:28:39.000000 invenio-records-rest-2.4.0/tests/test_views_item_get.py
--rw-r--r--   0 runner    (1001) docker     (127)     5448 2023-12-08 12:28:39.000000 invenio-records-rest-2.4.0/tests/test_views_item_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     5648 2023-12-08 12:28:39.000000 invenio-records-rest-2.4.0/tests/test_views_item_put.py
--rw-r--r--   0 runner    (1001) docker     (127)     5066 2023-12-08 12:28:39.000000 invenio-records-rest-2.4.0/tests/test_views_list_post.py
--rw-r--r--   0 runner    (1001) docker     (127)     1904 2023-12-08 12:28:39.000000 invenio-records-rest-2.4.0/tests/test_views_options.py
--rw-r--r--   0 runner    (1001) docker     (127)    14801 2023-12-08 12:28:39.000000 invenio-records-rest-2.4.0/tests/test_views_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     4479 2023-12-08 12:28:39.000000 invenio-records-rest-2.4.0/tests/test_views_serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4094 2023-12-08 12:28:39.000000 invenio-records-rest-2.4.0/tests/test_views_suggesters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:44:21.000000 invenio-records-rest-2.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-08 08:44:13.000000 invenio-records-rest-2.4.1/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-05-08 08:44:13.000000 invenio-records-rest-2.4.1/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-08 08:44:13.000000 invenio-records-rest-2.4.1/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:44:21.000000 invenio-records-rest-2.4.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:44:21.000000 invenio-records-rest-2.4.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-05-08 08:44:13.000000 invenio-records-rest-2.4.1/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-05-08 08:44:13.000000 invenio-records-rest-2.4.1/.github/workflows/tests.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:44:21.000000 invenio-records-rest-2.4.1/.tx/
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-08 08:44:13.000000 invenio-records-rest-2.4.1/.tx/config
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-05-08 08:44:13.000000 invenio-records-rest-2.4.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4796 2024-05-08 08:44:13.000000 invenio-records-rest-2.4.1/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3785 2024-05-08 08:44:13.000000 invenio-records-rest-2.4.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-08 08:44:13.000000 invenio-records-rest-2.4.1/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-08 08:44:13.000000 invenio-records-rest-2.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-08 08:44:13.000000 invenio-records-rest-2.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8135 2024-05-08 08:44:21.000000 invenio-records-rest-2.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-08 08:44:13.000000 invenio-records-rest-2.4.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-08 08:44:13.000000 invenio-records-rest-2.4.1/babel.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:44:21.000000 invenio-records-rest-2.4.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     7465 2024-05-08 08:44:13.000000 invenio-records-rest-2.4.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     2799 2024-05-08 08:44:13.000000 invenio-records-rest-2.4.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-08 08:44:13.000000 invenio-records-rest-2.4.1/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-08 08:44:13.000000 invenio-records-rest-2.4.1/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10851 2024-05-08 08:44:13.000000 invenio-records-rest-2.4.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-08 08:44:13.000000 invenio-records-rest-2.4.1/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-08 08:44:13.000000 invenio-records-rest-2.4.1/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-05-08 08:44:13.000000 invenio-records-rest-2.4.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-08 08:44:13.000000 invenio-records-rest-2.4.1/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-08 08:44:13.000000 invenio-records-rest-2.4.1/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7009 2024-05-08 08:44:13.000000 invenio-records-rest-2.4.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-08 08:44:13.000000 invenio-records-rest-2.4.1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-08 08:44:13.000000 invenio-records-rest-2.4.1/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:44:21.000000 invenio-records-rest-2.4.1/invenio_records_rest/
+-rw-r--r--   0 runner    (1001) docker     (127)    27039 2024-05-08 08:44:13.000000 invenio-records-rest-2.4.1/invenio_records_rest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-05-08 08:44:13.000000 invenio-records-rest-2.4.1/invenio_records_rest/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13499 2024-05-08 08:44:13.000000 invenio-records-rest-2.4.1/invenio_records_rest/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4926 2024-05-08 08:44:13.000000 invenio-records-rest-2.4.1/invenio_records_rest/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3890 2024-05-08 08:44:13.000000 invenio-records-rest-2.4.1/invenio_records_rest/ext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9896 2024-05-08 08:44:13.000000 invenio-records-rest-2.4.1/invenio_records_rest/facets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-05-08 08:44:13.000000 invenio-records-rest-2.4.1/invenio_records_rest/links.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:44:21.000000 invenio-records-rest-2.4.1/invenio_records_rest/loaders/
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-05-08 08:44:13.000000 invenio-records-rest-2.4.1/invenio_records_rest/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3160 2024-05-08 08:44:13.000000 invenio-records-rest-2.4.1/invenio_records_rest/loaders/marshmallow.py
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-08 08:44:13.000000 invenio-records-rest-2.4.1/invenio_records_rest/proxies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-05-08 08:44:13.000000 invenio-records-rest-2.4.1/invenio_records_rest/query.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:44:21.000000 invenio-records-rest-2.4.1/invenio_records_rest/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-08 08:44:13.000000 invenio-records-rest-2.4.1/invenio_records_rest/schemas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:44:21.000000 invenio-records-rest-2.4.1/invenio_records_rest/schemas/fields/
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-08 08:44:13.000000 invenio-records-rest-2.4.1/invenio_records_rest/schemas/fields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-05-08 08:44:13.000000 invenio-records-rest-2.4.1/invenio_records_rest/schemas/fields/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-05-08 08:44:13.000000 invenio-records-rest-2.4.1/invenio_records_rest/schemas/fields/generated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4392 2024-05-08 08:44:13.000000 invenio-records-rest-2.4.1/invenio_records_rest/schemas/fields/marshmallow_contrib.py
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-05-08 08:44:13.000000 invenio-records-rest-2.4.1/invenio_records_rest/schemas/fields/persistentidentifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-08 08:44:13.000000 invenio-records-rest-2.4.1/invenio_records_rest/schemas/fields/sanitizedhtml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-05-08 08:44:13.000000 invenio-records-rest-2.4.1/invenio_records_rest/schemas/fields/sanitizedunicode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-08 08:44:13.000000 invenio-records-rest-2.4.1/invenio_records_rest/schemas/fields/trimmedstring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3879 2024-05-08 08:44:13.000000 invenio-records-rest-2.4.1/invenio_records_rest/schemas/json.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:44:21.000000 invenio-records-rest-2.4.1/invenio_records_rest/serializers/
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-08 08:44:13.000000 invenio-records-rest-2.4.1/invenio_records_rest/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6388 2024-05-08 08:44:13.000000 invenio-records-rest-2.4.1/invenio_records_rest/serializers/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4615 2024-05-08 08:44:13.000000 invenio-records-rest-2.4.1/invenio_records_rest/serializers/citeproc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5431 2024-05-08 08:44:13.000000 invenio-records-rest-2.4.1/invenio_records_rest/serializers/csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4630 2024-05-08 08:44:13.000000 invenio-records-rest-2.4.1/invenio_records_rest/serializers/datacite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-05-08 08:44:13.000000 invenio-records-rest-2.4.1/invenio_records_rest/serializers/dc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2582 2024-05-08 08:44:13.000000 invenio-records-rest-2.4.1/invenio_records_rest/serializers/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-05-08 08:44:13.000000 invenio-records-rest-2.4.1/invenio_records_rest/serializers/jsonld.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-05-08 08:44:13.000000 invenio-records-rest-2.4.1/invenio_records_rest/serializers/marshmallow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2632 2024-05-08 08:44:13.000000 invenio-records-rest-2.4.1/invenio_records_rest/serializers/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4429 2024-05-08 08:44:13.000000 invenio-records-rest-2.4.1/invenio_records_rest/sorter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:44:21.000000 invenio-records-rest-2.4.1/invenio_records_rest/translations/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:44:21.000000 invenio-records-rest-2.4.1/invenio_records_rest/translations/en/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:44:21.000000 invenio-records-rest-2.4.1/invenio_records_rest/translations/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-05-08 08:44:21.000000 invenio-records-rest-2.4.1/invenio_records_rest/translations/en/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-08 08:44:13.000000 invenio-records-rest-2.4.1/invenio_records_rest/translations/en/LC_MESSAGES/messages.po
+-rw-r--r--   0 runner    (1001) docker     (127)     8569 2024-05-08 08:44:13.000000 invenio-records-rest-2.4.1/invenio_records_rest/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35194 2024-05-08 08:44:13.000000 invenio-records-rest-2.4.1/invenio_records_rest/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:44:21.000000 invenio-records-rest-2.4.1/invenio_records_rest.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8135 2024-05-08 08:44:21.000000 invenio-records-rest-2.4.1/invenio_records_rest.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3699 2024-05-08 08:44:21.000000 invenio-records-rest-2.4.1/invenio_records_rest.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 08:44:21.000000 invenio-records-rest-2.4.1/invenio_records_rest.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-08 08:44:21.000000 invenio-records-rest-2.4.1/invenio_records_rest.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 08:44:21.000000 invenio-records-rest-2.4.1/invenio_records_rest.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-08 08:44:21.000000 invenio-records-rest-2.4.1/invenio_records_rest.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-08 08:44:21.000000 invenio-records-rest-2.4.1/invenio_records_rest.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-08 08:44:13.000000 invenio-records-rest-2.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-05-08 08:44:13.000000 invenio-records-rest-2.4.1/requirements-devel.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      778 2024-05-08 08:44:13.000000 invenio-records-rest-2.4.1/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     2894 2024-05-08 08:44:21.000000 invenio-records-rest-2.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-08 08:44:13.000000 invenio-records-rest-2.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:44:21.000000 invenio-records-rest-2.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     9889 2024-05-08 08:44:13.000000 invenio-records-rest-2.4.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:44:21.000000 invenio-records-rest-2.4.1/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-08 08:44:13.000000 invenio-records-rest-2.4.1/tests/data/testrecords.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-05-08 08:44:13.000000 invenio-records-rest-2.4.1/tests/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:44:21.000000 invenio-records-rest-2.4.1/tests/mock_module/
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-08 08:44:13.000000 invenio-records-rest-2.4.1/tests/mock_module/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:44:21.000000 invenio-records-rest-2.4.1/tests/mock_module/mappings/
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-08 08:44:13.000000 invenio-records-rest-2.4.1/tests/mock_module/mappings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:44:21.000000 invenio-records-rest-2.4.1/tests/mock_module/mappings/os-v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-08 08:44:13.000000 invenio-records-rest-2.4.1/tests/mock_module/mappings/os-v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:44:21.000000 invenio-records-rest-2.4.1/tests/mock_module/mappings/os-v1/invenio-records-rest/
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-05-08 08:44:13.000000 invenio-records-rest-2.4.1/tests/mock_module/mappings/os-v1/invenio-records-rest/testrecord.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:44:21.000000 invenio-records-rest-2.4.1/tests/mock_module/mappings/os-v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-08 08:44:13.000000 invenio-records-rest-2.4.1/tests/mock_module/mappings/os-v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:44:21.000000 invenio-records-rest-2.4.1/tests/mock_module/mappings/os-v2/invenio-records-rest/
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-05-08 08:44:13.000000 invenio-records-rest-2.4.1/tests/mock_module/mappings/os-v2/invenio-records-rest/testrecord.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:44:21.000000 invenio-records-rest-2.4.1/tests/mock_module/mappings/v7/
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-08 08:44:13.000000 invenio-records-rest-2.4.1/tests/mock_module/mappings/v7/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:44:21.000000 invenio-records-rest-2.4.1/tests/mock_module/mappings/v7/invenio-records-rest/
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-05-08 08:44:13.000000 invenio-records-rest-2.4.1/tests/mock_module/mappings/v7/invenio-records-rest/testrecord.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5329 2024-05-08 08:44:13.000000 invenio-records-rest-2.4.1/tests/test_custom_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5644 2024-05-08 08:44:13.000000 invenio-records-rest-2.4.1/tests/test_custom_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-05-08 08:44:13.000000 invenio-records-rest-2.4.1/tests/test_error_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-08 08:44:13.000000 invenio-records-rest-2.4.1/tests/test_ext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9069 2024-05-08 08:44:13.000000 invenio-records-rest-2.4.1/tests/test_facets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-05-08 08:44:13.000000 invenio-records-rest-2.4.1/tests/test_index_prefixing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-05-08 08:44:13.000000 invenio-records-rest-2.4.1/tests/test_links.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-08 08:44:13.000000 invenio-records-rest-2.4.1/tests/test_marshmallow_contrib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7039 2024-05-08 08:44:13.000000 invenio-records-rest-2.4.1/tests/test_marshmallow_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-05-08 08:44:13.000000 invenio-records-rest-2.4.1/tests/test_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2241 2024-05-08 08:44:13.000000 invenio-records-rest-2.4.1/tests/test_pid_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-05-08 08:44:13.000000 invenio-records-rest-2.4.1/tests/test_serializer_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3201 2024-05-08 08:44:13.000000 invenio-records-rest-2.4.1/tests/test_serializer_citeproc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5996 2024-05-08 08:44:13.000000 invenio-records-rest-2.4.1/tests/test_serializer_csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3034 2024-05-08 08:44:13.000000 invenio-records-rest-2.4.1/tests/test_serializer_datacite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-05-08 08:44:13.000000 invenio-records-rest-2.4.1/tests/test_serializer_dc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-05-08 08:44:13.000000 invenio-records-rest-2.4.1/tests/test_serializer_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3382 2024-05-08 08:44:13.000000 invenio-records-rest-2.4.1/tests/test_serializer_jsonld.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-05-08 08:44:13.000000 invenio-records-rest-2.4.1/tests/test_serializer_marshmallow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-05-08 08:44:13.000000 invenio-records-rest-2.4.1/tests/test_serializer_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5101 2024-05-08 08:44:13.000000 invenio-records-rest-2.4.1/tests/test_sorter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-05-08 08:44:13.000000 invenio-records-rest-2.4.1/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-05-08 08:44:13.000000 invenio-records-rest-2.4.1/tests/test_views_item_delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2626 2024-05-08 08:44:13.000000 invenio-records-rest-2.4.1/tests/test_views_item_get.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5448 2024-05-08 08:44:13.000000 invenio-records-rest-2.4.1/tests/test_views_item_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5648 2024-05-08 08:44:13.000000 invenio-records-rest-2.4.1/tests/test_views_item_put.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5066 2024-05-08 08:44:13.000000 invenio-records-rest-2.4.1/tests/test_views_list_post.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-05-08 08:44:13.000000 invenio-records-rest-2.4.1/tests/test_views_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14801 2024-05-08 08:44:13.000000 invenio-records-rest-2.4.1/tests/test_views_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4479 2024-05-08 08:44:13.000000 invenio-records-rest-2.4.1/tests/test_views_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4094 2024-05-08 08:44:13.000000 invenio-records-rest-2.4.1/tests/test_views_suggesters.py
```

### Comparing `invenio-records-rest-2.4.0/.editorconfig` & `invenio-records-rest-2.4.1/.editorconfig`

 * *Files identical despite different names*

### Comparing `invenio-records-rest-2.4.0/.github/workflows/pypi-publish.yml` & `invenio-records-rest-2.4.1/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `invenio-records-rest-2.4.0/.github/workflows/tests.yml` & `invenio-records-rest-2.4.1/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `invenio-records-rest-2.4.0/AUTHORS.rst` & `invenio-records-rest-2.4.1/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `invenio-records-rest-2.4.0/CHANGES.rst` & `invenio-records-rest-2.4.1/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,18 @@
 
     Invenio is free software; you can redistribute it and/or modify it
     under the terms of the MIT License; see LICENSE file for more details.
 
 Changes
 =======
 
+Version 2.4.1 (2024-05-08)
+
+- marhsmallow: remove deprecation warning
+
 Version 2.4.0 (2023-12-08)
 
 - facet: Allow more than one possibility on range facets
 - search: possibility to specify a different query_parser
 - facets: New parameter, RECORDS_REST_FACETS_FILTER, to filter the facets based on a category based on all the other categories
 - i18n-global: add compile-catalog fuzzy (#323)
```

### Comparing `invenio-records-rest-2.4.0/CONTRIBUTING.rst` & `invenio-records-rest-2.4.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `invenio-records-rest-2.4.0/LICENSE` & `invenio-records-rest-2.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `invenio-records-rest-2.4.0/MANIFEST.in` & `invenio-records-rest-2.4.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `invenio-records-rest-2.4.0/PKG-INFO` & `invenio-records-rest-2.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-records-rest
-Version: 2.4.0
+Version: 2.4.1
 Summary: "REST API for invenio-records."
 Home-page: https://github.com/inveniosoftware/invenio-records-rest
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             This file is part of Invenio.
@@ -41,14 +41,18 @@
         
             Invenio is free software; you can redistribute it and/or modify it
             under the terms of the MIT License; see LICENSE file for more details.
         
         Changes
         =======
         
+        Version 2.4.1 (2024-05-08)
+        
+        - marhsmallow: remove deprecation warning
+        
         Version 2.4.0 (2023-12-08)
         
         - facet: Allow more than one possibility on range facets
         - search: possibility to specify a different query_parser
         - facets: New parameter, RECORDS_REST_FACETS_FILTER, to filter the facets based on a category based on all the other categories
         - i18n-global: add compile-catalog fuzzy (#323)
```

### Comparing `invenio-records-rest-2.4.0/README.rst` & `invenio-records-rest-2.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `invenio-records-rest-2.4.0/docs/Makefile` & `invenio-records-rest-2.4.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `invenio-records-rest-2.4.0/docs/api.rst` & `invenio-records-rest-2.4.1/docs/api.rst`

 * *Files identical despite different names*

### Comparing `invenio-records-rest-2.4.0/docs/conf.py` & `invenio-records-rest-2.4.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `invenio-records-rest-2.4.0/docs/index.rst` & `invenio-records-rest-2.4.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `invenio-records-rest-2.4.0/docs/make.bat` & `invenio-records-rest-2.4.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `invenio-records-rest-2.4.0/invenio_records_rest/__init__.py` & `invenio-records-rest-2.4.1/invenio_records_rest/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -707,10 +707,10 @@
 To fectch the corresponding object a fetcher is used, typically provided
 by Invenio-PIDStore.
 """
 
 from .ext import InvenioRecordsREST
 from .proxies import current_records_rest
 
-__version__ = "2.4.0"
+__version__ = "2.4.1"
 
 __all__ = ("__version__", "current_records_rest", "InvenioRecordsREST")
```

### Comparing `invenio-records-rest-2.4.0/invenio_records_rest/_compat.py` & `invenio-records-rest-2.4.1/invenio_records_rest/_compat.py`

 * *Files identical despite different names*

### Comparing `invenio-records-rest-2.4.0/invenio_records_rest/config.py` & `invenio-records-rest-2.4.1/invenio_records_rest/config.py`

 * *Files identical despite different names*

### Comparing `invenio-records-rest-2.4.0/invenio_records_rest/errors.py` & `invenio-records-rest-2.4.1/invenio_records_rest/errors.py`

 * *Files identical despite different names*

### Comparing `invenio-records-rest-2.4.0/invenio_records_rest/ext.py` & `invenio-records-rest-2.4.1/invenio_records_rest/ext.py`

 * *Files identical despite different names*

### Comparing `invenio-records-rest-2.4.0/invenio_records_rest/facets.py` & `invenio-records-rest-2.4.1/invenio_records_rest/facets.py`

 * *Files identical despite different names*

### Comparing `invenio-records-rest-2.4.0/invenio_records_rest/links.py` & `invenio-records-rest-2.4.1/invenio_records_rest/links.py`

 * *Files identical despite different names*

### Comparing `invenio-records-rest-2.4.0/invenio_records_rest/loaders/__init__.py` & `invenio-records-rest-2.4.1/invenio_records_rest/loaders/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-records-rest-2.4.0/invenio_records_rest/loaders/marshmallow.py` & `invenio-records-rest-2.4.1/invenio_records_rest/loaders/marshmallow.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,16 @@
 """
 
 import json
 
 from flask import request
 from invenio_rest.errors import RESTValidationError
 from marshmallow import ValidationError
-from marshmallow import __version_info__ as marshmallow_version
+
+from ..utils import marshmallow_major_version
 
 
 def _flatten_marshmallow_errors(errors, parents=()):
     """Flatten marshmallow errors."""
     res = []
     for field, error in errors.items():
         if isinstance(error, list):
@@ -77,15 +78,15 @@
 
         context = {}
         pid_data = request.view_args.get("pid_value")
         if pid_data:
             pid, record = pid_data.data
             context["pid"] = pid
             context["record"] = record
-        if marshmallow_version[0] < 3:
+        if marshmallow_major_version < 3:
             result = schema_class(context=context).load(request_json)
             if result.errors:
                 raise MarshmallowErrors(result.errors)
         else:
             # From Marshmallow 3 the errors on .load() are being raised rather
             # than returned. To adjust this change to our flow we catch these
             # errors and reraise them instead.
```

### Comparing `invenio-records-rest-2.4.0/invenio_records_rest/query.py` & `invenio-records-rest-2.4.1/invenio_records_rest/query.py`

 * *Files identical despite different names*

### Comparing `invenio-records-rest-2.4.0/invenio_records_rest/schemas/fields/__init__.py` & `invenio-records-rest-2.4.1/invenio_records_rest/schemas/fields/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-records-rest-2.4.0/invenio_records_rest/schemas/fields/datetime.py` & `invenio-records-rest-2.4.1/invenio_records_rest/schemas/fields/datetime.py`

 * *Files identical despite different names*

### Comparing `invenio-records-rest-2.4.0/invenio_records_rest/schemas/fields/generated.py` & `invenio-records-rest-2.4.1/invenio_records_rest/schemas/fields/generated.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,30 +6,31 @@
 # Invenio is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 
 """Generated field."""
 
 import warnings
 
-from marshmallow import __version_info__ as marshmallow_version
 from marshmallow import missing as missing_
 
+from invenio_records_rest.utils import marshmallow_major_version
+
 from .marshmallow_contrib import Function, Method
 
 
 class GeneratedValue(object):
     """Sentinel value class forcing marshmallow missing field generation."""
 
     pass
 
 
 class ForcedFieldDeserializeMixin(object):
     """Mixin that forces deserialization of marshmallow fields."""
 
-    if marshmallow_version[0] < 3:
+    if marshmallow_major_version < 3:
 
         def __init__(self, *args, **kwargs):
             """Override the "missing" parameter."""
             if "missing" in kwargs:
                 obj_name = "{self.__module__}.{self.__class__.__name__}".format(
                     self=self
                 )
```

### Comparing `invenio-records-rest-2.4.0/invenio_records_rest/schemas/fields/marshmallow_contrib.py` & `invenio-records-rest-2.4.1/invenio_records_rest/schemas/fields/marshmallow_contrib.py`

 * *Files identical despite different names*

### Comparing `invenio-records-rest-2.4.0/invenio_records_rest/schemas/fields/persistentidentifier.py` & `invenio-records-rest-2.4.1/invenio_records_rest/schemas/fields/persistentidentifier.py`

 * *Files identical despite different names*

### Comparing `invenio-records-rest-2.4.0/invenio_records_rest/schemas/fields/sanitizedhtml.py` & `invenio-records-rest-2.4.1/invenio_records_rest/schemas/fields/sanitizedhtml.py`

 * *Files identical despite different names*

### Comparing `invenio-records-rest-2.4.0/invenio_records_rest/schemas/fields/sanitizedunicode.py` & `invenio-records-rest-2.4.1/invenio_records_rest/schemas/fields/sanitizedunicode.py`

 * *Files identical despite different names*

### Comparing `invenio-records-rest-2.4.0/invenio_records_rest/schemas/fields/trimmedstring.py` & `invenio-records-rest-2.4.1/invenio_records_rest/schemas/fields/trimmedstring.py`

 * *Files identical despite different names*

### Comparing `invenio-records-rest-2.4.0/invenio_records_rest/schemas/json.py` & `invenio-records-rest-2.4.1/invenio_records_rest/schemas/json.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,20 +6,20 @@
 # Invenio is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 
 """Marshmallow JSON schema."""
 
 from flask import current_app
 from invenio_rest.serializer import BaseSchema as Schema
-from marshmallow import ValidationError
-from marshmallow import __version_info__ as marshmallow_version
-from marshmallow import fields, missing, post_load, validates_schema
+from marshmallow import ValidationError, fields, missing, post_load, validates_schema
 
 from invenio_records_rest.schemas.fields import PersistentIdentifier
 
+from ..utils import marshmallow_major_version
+
 
 class StrictKeysMixin(Schema):
     """Ensure only valid keys exists."""
 
     @validates_schema(pass_original=True)
     def check_unknown_fields(self, data, original_data, **kwargs):
         """Check for unknown keys."""
@@ -70,15 +70,15 @@
         else:
             for key, value in original_data.items():
                 if key not in data:
                     data[key] = value
         return data
 
 
-if marshmallow_version[0] < 3:
+if marshmallow_major_version < 3:
 
     class RecordMetadataSchemaJSONV1(OriginalKeysMixin):
         """Schema for records metadata v1 in JSON with injected PID value."""
 
         pid = PersistentIdentifier()
 
         def get_pid_field(self):
```

### Comparing `invenio-records-rest-2.4.0/invenio_records_rest/serializers/__init__.py` & `invenio-records-rest-2.4.1/invenio_records_rest/serializers/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-records-rest-2.4.0/invenio_records_rest/serializers/base.py` & `invenio-records-rest-2.4.1/invenio_records_rest/serializers/base.py`

 * *Files identical despite different names*

### Comparing `invenio-records-rest-2.4.0/invenio_records_rest/serializers/citeproc.py` & `invenio-records-rest-2.4.1/invenio_records_rest/serializers/citeproc.py`

 * *Files identical despite different names*

### Comparing `invenio-records-rest-2.4.0/invenio_records_rest/serializers/csv.py` & `invenio-records-rest-2.4.1/invenio_records_rest/serializers/csv.py`

 * *Files identical despite different names*

### Comparing `invenio-records-rest-2.4.0/invenio_records_rest/serializers/datacite.py` & `invenio-records-rest-2.4.1/invenio_records_rest/serializers/datacite.py`

 * *Files identical despite different names*

### Comparing `invenio-records-rest-2.4.0/invenio_records_rest/serializers/dc.py` & `invenio-records-rest-2.4.1/invenio_records_rest/serializers/dc.py`

 * *Files identical despite different names*

### Comparing `invenio-records-rest-2.4.0/invenio_records_rest/serializers/json.py` & `invenio-records-rest-2.4.1/invenio_records_rest/serializers/json.py`

 * *Files identical despite different names*

### Comparing `invenio-records-rest-2.4.0/invenio_records_rest/serializers/jsonld.py` & `invenio-records-rest-2.4.1/invenio_records_rest/serializers/jsonld.py`

 * *Files identical despite different names*

### Comparing `invenio-records-rest-2.4.0/invenio_records_rest/serializers/marshmallow.py` & `invenio-records-rest-2.4.1/invenio_records_rest/serializers/marshmallow.py`

 * *Files identical despite different names*

### Comparing `invenio-records-rest-2.4.0/invenio_records_rest/serializers/response.py` & `invenio-records-rest-2.4.1/invenio_records_rest/serializers/response.py`

 * *Files identical despite different names*

### Comparing `invenio-records-rest-2.4.0/invenio_records_rest/sorter.py` & `invenio-records-rest-2.4.1/invenio_records_rest/sorter.py`

 * *Files identical despite different names*

### Comparing `invenio-records-rest-2.4.0/invenio_records_rest/translations/en/LC_MESSAGES/messages.po` & `invenio-records-rest-2.4.1/invenio_records_rest/translations/en/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-records-rest-2.4.0/invenio_records_rest/utils.py` & `invenio-records-rest-2.4.1/invenio_records_rest/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 # Invenio is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 
 """General utility functions module."""
 
 from functools import partial
 
+import pkg_resources
 import six
 from flask import abort, current_app, jsonify, make_response, request, url_for
 from invenio_pidstore.errors import (
     PIDDeletedError,
     PIDDoesNotExistError,
     PIDMissingObjectError,
     PIDRedirectedError,
@@ -29,14 +30,18 @@
     PIDDoesNotExistRESTError,
     PIDMissingObjectRESTError,
     PIDRedirectedRESTError,
     PIDUnregisteredRESTError,
 )
 from .proxies import current_records_rest
 
+marshmallow_major_version = int(
+    pkg_resources.get_distribution("marshmallow").version[0]
+)
+
 
 def build_default_endpoint_prefixes(records_rest_endpoints):
     """Build the default_endpoint_prefixes map."""
     pid_types = set()
     guessed = set()
     endpoint_prefixes = {}
```

### Comparing `invenio-records-rest-2.4.0/invenio_records_rest/views.py` & `invenio-records-rest-2.4.1/invenio_records_rest/views.py`

 * *Files identical despite different names*

### Comparing `invenio-records-rest-2.4.0/invenio_records_rest.egg-info/PKG-INFO` & `invenio-records-rest-2.4.1/invenio_records_rest.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-records-rest
-Version: 2.4.0
+Version: 2.4.1
 Summary: "REST API for invenio-records."
 Home-page: https://github.com/inveniosoftware/invenio-records-rest
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             This file is part of Invenio.
@@ -41,14 +41,18 @@
         
             Invenio is free software; you can redistribute it and/or modify it
             under the terms of the MIT License; see LICENSE file for more details.
         
         Changes
         =======
         
+        Version 2.4.1 (2024-05-08)
+        
+        - marhsmallow: remove deprecation warning
+        
         Version 2.4.0 (2023-12-08)
         
         - facet: Allow more than one possibility on range facets
         - search: possibility to specify a different query_parser
         - facets: New parameter, RECORDS_REST_FACETS_FILTER, to filter the facets based on a category based on all the other categories
         - i18n-global: add compile-catalog fuzzy (#323)
```

### Comparing `invenio-records-rest-2.4.0/invenio_records_rest.egg-info/SOURCES.txt` & `invenio-records-rest-2.4.1/invenio_records_rest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `invenio-records-rest-2.4.0/invenio_records_rest.egg-info/entry_points.txt` & `invenio-records-rest-2.4.1/invenio_records_rest.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `invenio-records-rest-2.4.0/invenio_records_rest.egg-info/requires.txt` & `invenio-records-rest-2.4.1/invenio_records_rest.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `invenio-records-rest-2.4.0/requirements-devel.txt` & `invenio-records-rest-2.4.1/requirements-devel.txt`

 * *Files identical despite different names*

### Comparing `invenio-records-rest-2.4.0/run-tests.sh` & `invenio-records-rest-2.4.1/run-tests.sh`

 * *Files identical despite different names*

### Comparing `invenio-records-rest-2.4.0/setup.cfg` & `invenio-records-rest-2.4.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `invenio-records-rest-2.4.0/tests/conftest.py` & `invenio-records-rest-2.4.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-records-rest-2.4.0/tests/helpers.py` & `invenio-records-rest-2.4.1/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `invenio-records-rest-2.4.0/tests/mock_module/mappings/os-v1/invenio-records-rest/testrecord.json` & `invenio-records-rest-2.4.1/tests/mock_module/mappings/os-v1/invenio-records-rest/testrecord.json`

 * *Files identical despite different names*

### Comparing `invenio-records-rest-2.4.0/tests/mock_module/mappings/os-v2/invenio-records-rest/testrecord.json` & `invenio-records-rest-2.4.1/tests/mock_module/mappings/os-v2/invenio-records-rest/testrecord.json`

 * *Files identical despite different names*

### Comparing `invenio-records-rest-2.4.0/tests/mock_module/mappings/v7/invenio-records-rest/testrecord.json` & `invenio-records-rest-2.4.1/tests/mock_module/mappings/v7/invenio-records-rest/testrecord.json`

 * *Files identical despite different names*

### Comparing `invenio-records-rest-2.4.0/tests/test_custom_endpoints.py` & `invenio-records-rest-2.4.1/tests/test_custom_endpoints.py`

 * *Files identical despite different names*

### Comparing `invenio-records-rest-2.4.0/tests/test_custom_fields.py` & `invenio-records-rest-2.4.1/tests/test_custom_fields.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,39 +8,39 @@
 
 """Invenio custom schema fields tests."""
 
 import pytest
 from invenio_pidstore.models import PersistentIdentifier as PIDModel
 from invenio_records import Record
 from invenio_rest.serializer import BaseSchema as Schema
-from marshmallow import __version_info__ as marshmallow_version
 from marshmallow import missing
 
 from invenio_records_rest.schemas import StrictKeysMixin
 from invenio_records_rest.schemas.fields import (
     DateString,
     GenFunction,
     GenMethod,
     PersistentIdentifier,
     SanitizedHTML,
     SanitizedUnicode,
     TrimmedString,
 )
+from invenio_records_rest.utils import marshmallow_major_version
 
-if marshmallow_version[0] >= 3:
+if marshmallow_major_version >= 3:
     schema_to_use = Schema
     from marshmallow import EXCLUDE
 else:
     schema_to_use = StrictKeysMixin
 
 
 class CustomFieldSchema(schema_to_use):
     """Test schema."""
 
-    if marshmallow_version[0] >= 3:
+    if marshmallow_major_version >= 3:
 
         class Meta:
             """."""
 
             unknown = EXCLUDE
 
     date_string_field = DateString(attribute="date_string_field")
@@ -103,15 +103,15 @@
 
     def deserialize_func(value, ctx, data):
         return ctx.get("func-foo", data.get("func-bar", missing))
 
     class GeneratedFieldsSchema(schema_to_use):
         """Test schema."""
 
-        if marshmallow_version[0] >= 3:
+        if marshmallow_major_version >= 3:
 
             class Meta:
                 """Meta attributes for the schema."""
 
                 unknown = EXCLUDE
 
         gen_function = GenFunction(
```

### Comparing `invenio-records-rest-2.4.0/tests/test_error_handlers.py` & `invenio-records-rest-2.4.1/tests/test_error_handlers.py`

 * *Files identical despite different names*

### Comparing `invenio-records-rest-2.4.0/tests/test_ext.py` & `invenio-records-rest-2.4.1/tests/test_ext.py`

 * *Files identical despite different names*

### Comparing `invenio-records-rest-2.4.0/tests/test_facets.py` & `invenio-records-rest-2.4.1/tests/test_facets.py`

 * *Files identical despite different names*

### Comparing `invenio-records-rest-2.4.0/tests/test_index_prefixing.py` & `invenio-records-rest-2.4.1/tests/test_index_prefixing.py`

 * *Files identical despite different names*

### Comparing `invenio-records-rest-2.4.0/tests/test_links.py` & `invenio-records-rest-2.4.1/tests/test_links.py`

 * *Files identical despite different names*

### Comparing `invenio-records-rest-2.4.0/tests/test_marshmallow_contrib.py` & `invenio-records-rest-2.4.1/tests/test_marshmallow_contrib.py`

 * *Files identical despite different names*

### Comparing `invenio-records-rest-2.4.0/tests/test_marshmallow_loader.py` & `invenio-records-rest-2.4.1/tests/test_marshmallow_loader.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,25 +10,24 @@
 
 import json
 from copy import deepcopy
 
 from helpers import get_json
 from invenio_records.models import RecordMetadata
 from invenio_rest.serializer import BaseSchema as Schema
-from marshmallow import ValidationError
-from marshmallow import __version_info__ as marshmallow_version
-from marshmallow import fields
+from marshmallow import ValidationError, fields
 
 from invenio_records_rest.loaders import json_pid_checker
 from invenio_records_rest.loaders.marshmallow import (
     MarshmallowErrors,
     marshmallow_loader,
 )
 from invenio_records_rest.schemas import Nested
 from invenio_records_rest.schemas.fields import PersistentIdentifier
+from invenio_records_rest.utils import marshmallow_major_version
 
 
 class _TestSchema(Schema):
     """Test schema."""
 
     title = fields.Str(required=True, attribute="metadata.mytitle")
     random = fields.Str(required=True, attribute="metadata.nonexistant")
@@ -162,15 +161,15 @@
         assert has_error(field="title", parents=["non_list"])
         assert has_error(field="sample", parents=["nested_field", 0])
 
 
 def test_marshmallow_errors(test_data):
     """Test MarshmallowErrors class."""
     incomplete_data = dict(test_data[0])
-    if marshmallow_version[0] >= 3:
+    if marshmallow_major_version >= 3:
         try:
             res = _TestSchema(context={}).load(json.dumps(incomplete_data))
         except ValidationError as error:
             errors = error.messages
     else:
         res = _TestSchema(context={}).load(json.dumps(incomplete_data))
         errors = res.errors
```

### Comparing `invenio-records-rest-2.4.0/tests/test_permissions.py` & `invenio-records-rest-2.4.1/tests/test_permissions.py`

 * *Files identical despite different names*

### Comparing `invenio-records-rest-2.4.0/tests/test_pid_resolver.py` & `invenio-records-rest-2.4.1/tests/test_pid_resolver.py`

 * *Files identical despite different names*

### Comparing `invenio-records-rest-2.4.0/tests/test_serializer_base.py` & `invenio-records-rest-2.4.1/tests/test_serializer_base.py`

 * *Files identical despite different names*

### Comparing `invenio-records-rest-2.4.0/tests/test_serializer_citeproc.py` & `invenio-records-rest-2.4.1/tests/test_serializer_citeproc.py`

 * *Files identical despite different names*

### Comparing `invenio-records-rest-2.4.0/tests/test_serializer_csv.py` & `invenio-records-rest-2.4.1/tests/test_serializer_csv.py`

 * *Files identical despite different names*

### Comparing `invenio-records-rest-2.4.0/tests/test_serializer_datacite.py` & `invenio-records-rest-2.4.1/tests/test_serializer_datacite.py`

 * *Files identical despite different names*

### Comparing `invenio-records-rest-2.4.0/tests/test_serializer_dc.py` & `invenio-records-rest-2.4.1/tests/test_serializer_dc.py`

 * *Files identical despite different names*

### Comparing `invenio-records-rest-2.4.0/tests/test_serializer_json.py` & `invenio-records-rest-2.4.1/tests/test_serializer_json.py`

 * *Files identical despite different names*

### Comparing `invenio-records-rest-2.4.0/tests/test_serializer_jsonld.py` & `invenio-records-rest-2.4.1/tests/test_serializer_jsonld.py`

 * *Files identical despite different names*

### Comparing `invenio-records-rest-2.4.0/tests/test_serializer_marshmallow.py` & `invenio-records-rest-2.4.1/tests/test_serializer_marshmallow.py`

 * *Files identical despite different names*

### Comparing `invenio-records-rest-2.4.0/tests/test_serializer_response.py` & `invenio-records-rest-2.4.1/tests/test_serializer_response.py`

 * *Files identical despite different names*

### Comparing `invenio-records-rest-2.4.0/tests/test_sorter.py` & `invenio-records-rest-2.4.1/tests/test_sorter.py`

 * *Files identical despite different names*

### Comparing `invenio-records-rest-2.4.0/tests/test_utils.py` & `invenio-records-rest-2.4.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `invenio-records-rest-2.4.0/tests/test_views_item_delete.py` & `invenio-records-rest-2.4.1/tests/test_views_item_delete.py`

 * *Files identical despite different names*

### Comparing `invenio-records-rest-2.4.0/tests/test_views_item_get.py` & `invenio-records-rest-2.4.1/tests/test_views_item_get.py`

 * *Files identical despite different names*

### Comparing `invenio-records-rest-2.4.0/tests/test_views_item_patch.py` & `invenio-records-rest-2.4.1/tests/test_views_item_patch.py`

 * *Files identical despite different names*

### Comparing `invenio-records-rest-2.4.0/tests/test_views_item_put.py` & `invenio-records-rest-2.4.1/tests/test_views_item_put.py`

 * *Files identical despite different names*

### Comparing `invenio-records-rest-2.4.0/tests/test_views_list_post.py` & `invenio-records-rest-2.4.1/tests/test_views_list_post.py`

 * *Files identical despite different names*

### Comparing `invenio-records-rest-2.4.0/tests/test_views_options.py` & `invenio-records-rest-2.4.1/tests/test_views_options.py`

 * *Files identical despite different names*

### Comparing `invenio-records-rest-2.4.0/tests/test_views_search.py` & `invenio-records-rest-2.4.1/tests/test_views_search.py`

 * *Files identical despite different names*

### Comparing `invenio-records-rest-2.4.0/tests/test_views_serializers.py` & `invenio-records-rest-2.4.1/tests/test_views_serializers.py`

 * *Files identical despite different names*

### Comparing `invenio-records-rest-2.4.0/tests/test_views_suggesters.py` & `invenio-records-rest-2.4.1/tests/test_views_suggesters.py`

 * *Files identical despite different names*

