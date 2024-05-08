# Comparing `tmp/django_import_export-4.0.0rc3.tar.gz` & `tmp/django_import_export-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_import_export-4.0.0rc3.tar", last modified: Sat Apr 13 13:35:48 2024, max compression
+gzip compressed data, was "django_import_export-4.0.1.tar", last modified: Wed May  8 08:57:18 2024, max compression
```

## Comparing `django_import_export-4.0.0rc3.tar` & `django_import_export-4.0.1.tar`

### file list

```diff
@@ -1,333 +1,335 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.528308 django_import_export-4.0.0rc3/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/.flake8
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.488308 django_import_export-4.0.0rc3/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.492308 django_import_export-4.0.0rc3/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/.github/ISSUE_TEMPLATE/question.md
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/.github/pull_request_template.md
--rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/.github/stale.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.492308 django_import_export-4.0.0rc3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/.github/workflows/pre-commit.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3756 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)     5547 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     5508 2024-04-13 13:35:48.528308 django_import_export-4.0.0rc3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/RELEASE.md
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.524308 django_import_export-4.0.0rc3/django_import_export.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5508 2024-04-13 13:35:48.000000 django_import_export-4.0.0rc3/django_import_export.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9941 2024-04-13 13:35:48.000000 django_import_export-4.0.0rc3/django_import_export.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 13:35:48.000000 django_import_export-4.0.0rc3/django_import_export.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-13 13:35:48.000000 django_import_export-4.0.0rc3/django_import_export.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-13 13:35:48.000000 django_import_export-4.0.0rc3/django_import_export.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.496308 django_import_export-4.0.0rc3/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     5621 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.476308 django_import_export-4.0.0rc3/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.500308 django_import_export-4.0.0rc3/docs/_static/images/
--rw-r--r--   0 runner    (1001) docker     (127)    21509 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/docs/_static/images/change-form-export.png
--rw-r--r--   0 runner    (1001) docker     (127)    28966 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/docs/_static/images/custom-export-form.png
--rw-r--r--   0 runner    (1001) docker     (127)    90059 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/docs/_static/images/custom-import-form.png
--rw-r--r--   0 runner    (1001) docker     (127)    33092 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/docs/_static/images/date-widget-validation-error.png
--rw-r--r--   0 runner    (1001) docker     (127)    30818 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/docs/_static/images/django-import-export-change.png
--rw-r--r--   0 runner    (1001) docker     (127)    29191 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/docs/_static/images/django-import-export-export-confirm.png
--rw-r--r--   0 runner    (1001) docker     (127)    35696 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/docs/_static/images/django-import-export-import-confirm.png
--rw-r--r--   0 runner    (1001) docker     (127)    32366 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/docs/_static/images/django-import-export-import.png
--rw-r--r--   0 runner    (1001) docker     (127)     6097 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/docs/_static/images/export-button.png
--rw-r--r--   0 runner    (1001) docker     (127)    33286 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/docs/_static/images/export_workflow.svg
--rw-r--r--   0 runner    (1001) docker     (127)     6047 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/docs/_static/images/import-button.png
--rw-r--r--   0 runner    (1001) docker     (127)    56726 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/docs/_static/images/import_workflow.svg
--rw-r--r--   0 runner    (1001) docker     (127)    29758 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/docs/_static/images/non-field-specific-validation-error.png
--rw-r--r--   0 runner    (1001) docker     (127)    17197 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/docs/_static/images/select-for-export.png
--rw-r--r--   0 runner    (1001) docker     (127)    21868 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/docs/admin_integration.rst
--rw-r--r--   0 runner    (1001) docker     (127)    30548 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/docs/advanced_usage.rst
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/docs/api_admin.rst
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/docs/api_exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/docs/api_fields.rst
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/docs/api_forms.rst
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/docs/api_instance_loaders.rst
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/docs/api_mixins.rst
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/docs/api_resources.rst
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/docs/api_results.rst
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/docs/api_tmp_storages.rst
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/docs/api_widgets.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3421 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/docs/bulk_import.rst
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/docs/celery.rst
--rw-r--r--   0 runner    (1001) docker     (127)    30340 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     6284 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/docs/export_workflow.rst
--rwxr-xr-x   0 runner    (1001) docker     (127)    10047 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/docs/faq.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4748 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/docs/getting_started.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.500308 django_import_export-4.0.0rc3/docs/image_src/
--rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/docs/image_src/export_workflow.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3002 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/docs/image_src/import_workflow.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5713 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/docs/import_workflow.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7857 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5126 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)    14757 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/docs/release_notes.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2662 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/docs/testing.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.500308 django_import_export-4.0.0rc3/import_export/
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-13 13:35:48.000000 django_import_export-4.0.0rc3/import_export/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    35262 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)     6292 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/declarative.py
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5653 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/fields.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.500308 django_import_export-4.0.0rc3/import_export/formats/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/formats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6018 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/formats/base_formats.py
--rw-r--r--   0 runner    (1001) docker     (127)     9611 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/forms.py
--rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/instance_loaders.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.480308 django_import_export-4.0.0rc3/import_export/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.476308 django_import_export-4.0.0rc3/import_export/locale/ar/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.500308 django_import_export-4.0.0rc3/import_export/locale/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/locale/ar/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5394 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/locale/ar/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.476308 django_import_export-4.0.0rc3/import_export/locale/bg/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.500308 django_import_export-4.0.0rc3/import_export/locale/bg/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/locale/bg/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5626 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/locale/bg/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.476308 django_import_export-4.0.0rc3/import_export/locale/ca/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.504308 django_import_export-4.0.0rc3/import_export/locale/ca/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/locale/ca/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5117 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/locale/ca/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.476308 django_import_export-4.0.0rc3/import_export/locale/cs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.504308 django_import_export-4.0.0rc3/import_export/locale/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/locale/cs/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5187 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/locale/cs/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.476308 django_import_export-4.0.0rc3/import_export/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.504308 django_import_export-4.0.0rc3/import_export/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     2269 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5619 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.476308 django_import_export-4.0.0rc3/import_export/locale/es/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.504308 django_import_export-4.0.0rc3/import_export/locale/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5708 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.476308 django_import_export-4.0.0rc3/import_export/locale/es_AR/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.504308 django_import_export-4.0.0rc3/import_export/locale/es_AR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/locale/es_AR/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5712 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/locale/es_AR/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.476308 django_import_export-4.0.0rc3/import_export/locale/fa/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.504308 django_import_export-4.0.0rc3/import_export/locale/fa/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/locale/fa/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5726 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/locale/fa/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.476308 django_import_export-4.0.0rc3/import_export/locale/fi/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.504308 django_import_export-4.0.0rc3/import_export/locale/fi/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/locale/fi/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5140 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/locale/fi/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.476308 django_import_export-4.0.0rc3/import_export/locale/fr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.504308 django_import_export-4.0.0rc3/import_export/locale/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5108 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.476308 django_import_export-4.0.0rc3/import_export/locale/it/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.504308 django_import_export-4.0.0rc3/import_export/locale/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/locale/it/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5067 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/locale/it/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.480308 django_import_export-4.0.0rc3/import_export/locale/ja/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.504308 django_import_export-4.0.0rc3/import_export/locale/ja/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/locale/ja/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5194 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/locale/ja/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.480308 django_import_export-4.0.0rc3/import_export/locale/ko/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.504308 django_import_export-4.0.0rc3/import_export/locale/ko/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/locale/ko/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5371 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/locale/ko/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.480308 django_import_export-4.0.0rc3/import_export/locale/kz/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.504308 django_import_export-4.0.0rc3/import_export/locale/kz/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/locale/kz/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5913 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/locale/kz/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.480308 django_import_export-4.0.0rc3/import_export/locale/nl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.504308 django_import_export-4.0.0rc3/import_export/locale/nl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/locale/nl/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5456 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/locale/nl/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.480308 django_import_export-4.0.0rc3/import_export/locale/pl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.508308 django_import_export-4.0.0rc3/import_export/locale/pl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/locale/pl/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5280 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/locale/pl/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.480308 django_import_export-4.0.0rc3/import_export/locale/pt_BR/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.508308 django_import_export-4.0.0rc3/import_export/locale/pt_BR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/locale/pt_BR/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5405 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/locale/pt_BR/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.480308 django_import_export-4.0.0rc3/import_export/locale/ru/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.508308 django_import_export-4.0.0rc3/import_export/locale/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5961 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.480308 django_import_export-4.0.0rc3/import_export/locale/sk/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.508308 django_import_export-4.0.0rc3/import_export/locale/sk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/locale/sk/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5113 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/locale/sk/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.480308 django_import_export-4.0.0rc3/import_export/locale/tr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.508308 django_import_export-4.0.0rc3/import_export/locale/tr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/locale/tr/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5465 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/locale/tr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.480308 django_import_export-4.0.0rc3/import_export/locale/zh_Hans/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.508308 django_import_export-4.0.0rc3/import_export/locale/zh_Hans/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/locale/zh_Hans/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5238 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/locale/zh_Hans/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (127)     8064 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)     6543 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/options.py
--rw-r--r--   0 runner    (1001) docker     (127)    48286 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     8079 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/results.py
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.480308 django_import_export-4.0.0rc3/import_export/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.508308 django_import_export-4.0.0rc3/import_export/static/import_export/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/static/import_export/export.css
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/static/import_export/export_selectable_fields.js
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/static/import_export/guess_format.js
--rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/static/import_export/import.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.480308 django_import_export-4.0.0rc3/import_export/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.480308 django_import_export-4.0.0rc3/import_export/templates/admin/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.508308 django_import_export-4.0.0rc3/import_export/templates/admin/import_export/
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/templates/admin/import_export/base.html
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/templates/admin/import_export/change_form.html
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/templates/admin/import_export/change_list.html
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/templates/admin/import_export/change_list_export.html
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/templates/admin/import_export/change_list_export_item.html
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/templates/admin/import_export/change_list_import.html
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/templates/admin/import_export/change_list_import_export.html
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/templates/admin/import_export/change_list_import_item.html
--rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/templates/admin/import_export/export.html
--rw-r--r--   0 runner    (1001) docker     (127)     6686 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/templates/admin/import_export/import.html
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/templates/admin/import_export/resource_fields_list.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.512308 django_import_export-4.0.0rc3/import_export/templatetags/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/templatetags/import_export_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/tmp_storages.py
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    21360 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/import_export/widgets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.512308 django_import_export-4.0.0rc3/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/runtests.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      884 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/runtests.sh
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 13:35:48.528308 django_import_export-4.0.0rc3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.512308 django_import_export-4.0.0rc3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/books-sample.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.512308 django_import_export-4.0.0rc3/tests/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3233 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.516308 django_import_export-4.0.0rc3/tests/core/exports/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/exports/authors.csv
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/exports/books-ISO-8859-1.csv
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/exports/books-dos.csv
--rw-r--r--   0 runner    (1001) docker     (127)     9650 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/exports/books-empty-author-email.xlsx
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/exports/books-for-delete.csv
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/exports/books-invalid-date.csv
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/exports/books-mac.csv
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/exports/books-mac.tsv
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/exports/books-no-headers.csv
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/exports/books-unicode.csv
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/exports/books-unicode.tsv
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/exports/books.csv
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/exports/books.json
--rw-r--r--   0 runner    (1001) docker     (127)     5632 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/exports/books.xls
--rw-r--r--   0 runner    (1001) docker     (127)     4886 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/exports/books.xlsx
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/exports/child.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.516308 django_import_export-4.0.0rc3/tests/core/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/fixtures/author.json
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/fixtures/book.json
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/fixtures/category.json
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.516308 django_import_export-4.0.0rc3/tests/core/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     5662 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/migrations/0002_book_published_time.py
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/migrations/0003_withfloatfield.py
--rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/migrations/0004_bookwithchapters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/migrations/0005_addparentchild.py
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/migrations/0006_auto_20171130_0147.py
--rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/migrations/0007_auto_20180628_0411.py
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/migrations/0008_auto_20190409_0846.py
--rw-r--r--   0 runner    (1001) docker     (127)     3131 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/migrations/0009_auto_20211111_0807.py
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/migrations/0010_uuidbook.py
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/migrations/0011_uuidcategory_legacybook_alter_uuidbook_id_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/migrations/0012_delete_legacybook.py
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/migrations/0013_alter_author_birthday.py
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/migrations/0014_bookwithchapternumbers.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4820 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.484308 django_import_export-4.0.0rc3/tests/core/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.516308 django_import_export-4.0.0rc3/tests/core/templates/core/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.516308 django_import_export-4.0.0rc3/tests/core/templates/core/admin/
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/templates/core/admin/change_list.html
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/templates/core/category_list.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.520308 django_import_export-4.0.0rc3/tests/core/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.520308 django_import_export-4.0.0rc3/tests/core/tests/admin_integration/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/tests/admin_integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/tests/admin_integration/mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)     7219 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/tests/admin_integration/test_action.py
--rw-r--r--   0 runner    (1001) docker     (127)    17602 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/tests/admin_integration/test_export.py
--rw-r--r--   0 runner    (1001) docker     (127)    41866 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/tests/admin_integration/test_import.py
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/tests/admin_integration/test_views.py
--rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/tests/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     8043 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/tests/test_base_formats.py
--rw-r--r--   0 runner    (1001) docker     (127)     3706 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/tests/test_declarative.py
--rw-r--r--   0 runner    (1001) docker     (127)     5318 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/tests/test_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     7211 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/tests/test_forms.py
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/tests/test_import_export_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/tests/test_instance_loaders.py
--rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/tests/test_invalidrow.py
--rw-r--r--   0 runner    (1001) docker     (127)    11274 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/tests/test_mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)     4715 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/tests/test_permissions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.520308 django_import_export-4.0.0rc3/tests/core/tests/test_resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/tests/test_resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23519 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/tests/test_resources/test_bulk_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     4295 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/tests/test_resources/test_diffs.py
--rw-r--r--   0 runner    (1001) docker     (127)    14488 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/tests/test_resources/test_import_export.py
--rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/tests/test_resources/test_misc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.524308 django_import_export-4.0.0rc3/tests/core/tests/test_resources/test_modelresource/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/tests/test_resources/test_modelresource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6519 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/tests/test_resources/test_modelresource/test_data_deletion.py
--rw-r--r--   0 runner    (1001) docker     (127)     4806 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/tests/test_resources/test_modelresource/test_data_handling.py
--rw-r--r--   0 runner    (1001) docker     (127)     6034 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/tests/test_resources/test_modelresource/test_data_import.py
--rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/tests/test_resources/test_modelresource/test_deprecated_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)    13861 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/tests/test_resources/test_modelresource/test_dynamic_customization.py
--rw-r--r--   0 runner    (1001) docker     (127)     6948 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/tests/test_resources/test_modelresource/test_error_handling.py
--rw-r--r--   0 runner    (1001) docker     (127)     3068 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/tests/test_resources/test_modelresource/test_export.py
--rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/tests/test_resources/test_modelresource/test_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     5971 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/tests/test_resources/test_modelresource/test_m2m.py
--rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/tests/test_resources/test_modelresource/test_queryset.py
--rw-r--r--   0 runner    (1001) docker     (127)     4061 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/tests/test_resources/test_modelresource/test_relationship.py
--rw-r--r--   0 runner    (1001) docker     (127)     3661 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/tests/test_resources/test_modelresource/test_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/tests/test_resources/test_modelresource/test_resource_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     6536 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/tests/test_resources/test_modelresource/test_resource_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     7663 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/tests/test_resources/test_modelresource/test_resource_postgres.py
--rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/tests/test_resources/test_modelresource/test_resource_setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     4778 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/tests/test_resources/test_modelresource/test_resource_transactions.py
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/tests/test_resources/test_modelresource/test_string_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/tests/test_resources/test_modelresource/test_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)    10093 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/tests/test_resources/test_relationships.py
--rw-r--r--   0 runner    (1001) docker     (127)     4651 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/tests/test_results.py
--rw-r--r--   0 runner    (1001) docker     (127)     5877 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/tests/test_tmp_storages.py
--rw-r--r--   0 runner    (1001) docker     (127)    28373 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/tests/test_widgets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/tests/widget.py
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/core/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.484308 django_import_export-4.0.0rc3/tests/docker/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.524308 django_import_export-4.0.0rc3/tests/docker/db/
--rwxr-xr-x   0 runner    (1001) docker     (127)      146 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/docker/db/init-mysql-db.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      401 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/docker/db/init-postgres-db.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/docker-compose.yml
--rwxr-xr-x   0 runner    (1001) docker     (127)      320 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/manage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:48.524308 django_import_export-4.0.0rc3/tests/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5341 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/scripts/bulk_import.py
--rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tests/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-04-13 13:35:44.000000 django_import_export-4.0.0rc3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.552449 django_import_export-4.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-08 08:57:10.000000 django_import_export-4.0.1/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-08 08:57:10.000000 django_import_export-4.0.1/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-08 08:57:10.000000 django_import_export-4.0.1/.flake8
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-08 08:57:10.000000 django_import_export-4.0.1/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.508449 django_import_export-4.0.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-08 08:57:10.000000 django_import_export-4.0.1/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.508449 django_import_export-4.0.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-08 08:57:10.000000 django_import_export-4.0.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-08 08:57:10.000000 django_import_export-4.0.1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-08 08:57:10.000000 django_import_export-4.0.1/.github/ISSUE_TEMPLATE/question.md
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-08 08:57:10.000000 django_import_export-4.0.1/.github/pull_request_template.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-05-08 08:57:10.000000 django_import_export-4.0.1/.github/stale.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.508449 django_import_export-4.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-08 08:57:10.000000 django_import_export-4.0.1/.github/workflows/pre-commit.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-05-08 08:57:10.000000 django_import_export-4.0.1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-05-08 08:57:10.000000 django_import_export-4.0.1/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-08 08:57:10.000000 django_import_export-4.0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-08 08:57:10.000000 django_import_export-4.0.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-05-08 08:57:10.000000 django_import_export-4.0.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3784 2024-05-08 08:57:10.000000 django_import_export-4.0.1/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)     5547 2024-05-08 08:57:10.000000 django_import_export-4.0.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-08 08:57:10.000000 django_import_export-4.0.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-08 08:57:10.000000 django_import_export-4.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-05-08 08:57:10.000000 django_import_export-4.0.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     5434 2024-05-08 08:57:18.552449 django_import_export-4.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-05-08 08:57:10.000000 django_import_export-4.0.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-05-08 08:57:10.000000 django_import_export-4.0.1/RELEASE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-08 08:57:10.000000 django_import_export-4.0.1/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.552449 django_import_export-4.0.1/django_import_export.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5434 2024-05-08 08:57:18.000000 django_import_export-4.0.1/django_import_export.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10068 2024-05-08 08:57:18.000000 django_import_export-4.0.1/django_import_export.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 08:57:18.000000 django_import_export-4.0.1/django_import_export.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-08 08:57:18.000000 django_import_export-4.0.1/django_import_export.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-08 08:57:18.000000 django_import_export-4.0.1/django_import_export.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.512449 django_import_export-4.0.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     5621 2024-05-08 08:57:10.000000 django_import_export-4.0.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.496449 django_import_export-4.0.1/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.516449 django_import_export-4.0.1/docs/_static/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    21509 2024-05-08 08:57:10.000000 django_import_export-4.0.1/docs/_static/images/change-form-export.png
+-rw-r--r--   0 runner    (1001) docker     (127)    28966 2024-05-08 08:57:10.000000 django_import_export-4.0.1/docs/_static/images/custom-export-form.png
+-rw-r--r--   0 runner    (1001) docker     (127)    90059 2024-05-08 08:57:10.000000 django_import_export-4.0.1/docs/_static/images/custom-import-form.png
+-rw-r--r--   0 runner    (1001) docker     (127)    33092 2024-05-08 08:57:10.000000 django_import_export-4.0.1/docs/_static/images/date-widget-validation-error.png
+-rw-r--r--   0 runner    (1001) docker     (127)    30818 2024-05-08 08:57:10.000000 django_import_export-4.0.1/docs/_static/images/django-import-export-change.png
+-rw-r--r--   0 runner    (1001) docker     (127)    29191 2024-05-08 08:57:10.000000 django_import_export-4.0.1/docs/_static/images/django-import-export-export-confirm.png
+-rw-r--r--   0 runner    (1001) docker     (127)    35696 2024-05-08 08:57:10.000000 django_import_export-4.0.1/docs/_static/images/django-import-export-import-confirm.png
+-rw-r--r--   0 runner    (1001) docker     (127)    32366 2024-05-08 08:57:10.000000 django_import_export-4.0.1/docs/_static/images/django-import-export-import.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6097 2024-05-08 08:57:10.000000 django_import_export-4.0.1/docs/_static/images/export-button.png
+-rw-r--r--   0 runner    (1001) docker     (127)    33710 2024-05-08 08:57:10.000000 django_import_export-4.0.1/docs/_static/images/export_workflow.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     6047 2024-05-08 08:57:10.000000 django_import_export-4.0.1/docs/_static/images/import-button.png
+-rw-r--r--   0 runner    (1001) docker     (127)    56726 2024-05-08 08:57:10.000000 django_import_export-4.0.1/docs/_static/images/import_workflow.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    29758 2024-05-08 08:57:10.000000 django_import_export-4.0.1/docs/_static/images/non-field-specific-validation-error.png
+-rw-r--r--   0 runner    (1001) docker     (127)    17197 2024-05-08 08:57:10.000000 django_import_export-4.0.1/docs/_static/images/select-for-export.png
+-rw-r--r--   0 runner    (1001) docker     (127)    21868 2024-05-08 08:57:10.000000 django_import_export-4.0.1/docs/admin_integration.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    30548 2024-05-08 08:57:10.000000 django_import_export-4.0.1/docs/advanced_usage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-08 08:57:10.000000 django_import_export-4.0.1/docs/api_admin.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-08 08:57:10.000000 django_import_export-4.0.1/docs/api_exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-08 08:57:10.000000 django_import_export-4.0.1/docs/api_fields.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-08 08:57:10.000000 django_import_export-4.0.1/docs/api_forms.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-08 08:57:10.000000 django_import_export-4.0.1/docs/api_instance_loaders.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-05-08 08:57:10.000000 django_import_export-4.0.1/docs/api_mixins.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-08 08:57:10.000000 django_import_export-4.0.1/docs/api_resources.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-08 08:57:10.000000 django_import_export-4.0.1/docs/api_results.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-08 08:57:10.000000 django_import_export-4.0.1/docs/api_tmp_storages.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-08 08:57:10.000000 django_import_export-4.0.1/docs/api_widgets.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3421 2024-05-08 08:57:10.000000 django_import_export-4.0.1/docs/bulk_import.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-08 08:57:10.000000 django_import_export-4.0.1/docs/celery.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    57619 2024-05-08 08:57:10.000000 django_import_export-4.0.1/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-05-08 08:57:10.000000 django_import_export-4.0.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6284 2024-05-08 08:57:10.000000 django_import_export-4.0.1/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-05-08 08:57:10.000000 django_import_export-4.0.1/docs/export_workflow.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10047 2024-05-08 08:57:10.000000 django_import_export-4.0.1/docs/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4748 2024-05-08 08:57:10.000000 django_import_export-4.0.1/docs/getting_started.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.516449 django_import_export-4.0.1/docs/image_src/
+-rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-05-08 08:57:10.000000 django_import_export-4.0.1/docs/image_src/export_workflow.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3002 2024-05-08 08:57:10.000000 django_import_export-4.0.1/docs/image_src/import_workflow.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5713 2024-05-08 08:57:10.000000 django_import_export-4.0.1/docs/import_workflow.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-05-08 08:57:10.000000 django_import_export-4.0.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7889 2024-05-08 08:57:10.000000 django_import_export-4.0.1/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5126 2024-05-08 08:57:10.000000 django_import_export-4.0.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)    14882 2024-05-08 08:57:10.000000 django_import_export-4.0.1/docs/release_notes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2662 2024-05-08 08:57:10.000000 django_import_export-4.0.1/docs/testing.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.520449 django_import_export-4.0.1/import_export/
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-08 08:57:18.000000 django_import_export-4.0.1/import_export/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35221 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6292 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/declarative.py
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5643 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/fields.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.520449 django_import_export-4.0.1/import_export/formats/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/formats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6018 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/formats/base_formats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9611 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/instance_loaders.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.500449 django_import_export-4.0.1/import_export/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.496449 django_import_export-4.0.1/import_export/locale/ar/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.520449 django_import_export-4.0.1/import_export/locale/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/locale/ar/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5394 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/locale/ar/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.496449 django_import_export-4.0.1/import_export/locale/bg/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.520449 django_import_export-4.0.1/import_export/locale/bg/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/locale/bg/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5626 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/locale/bg/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.496449 django_import_export-4.0.1/import_export/locale/ca/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.520449 django_import_export-4.0.1/import_export/locale/ca/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/locale/ca/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5117 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/locale/ca/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.496449 django_import_export-4.0.1/import_export/locale/cs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.524449 django_import_export-4.0.1/import_export/locale/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/locale/cs/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5187 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/locale/cs/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.496449 django_import_export-4.0.1/import_export/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.524449 django_import_export-4.0.1/import_export/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2269 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5619 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.496449 django_import_export-4.0.1/import_export/locale/es/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.524449 django_import_export-4.0.1/import_export/locale/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5708 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.496449 django_import_export-4.0.1/import_export/locale/es_AR/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.524449 django_import_export-4.0.1/import_export/locale/es_AR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/locale/es_AR/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5712 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/locale/es_AR/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.496449 django_import_export-4.0.1/import_export/locale/fa/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.524449 django_import_export-4.0.1/import_export/locale/fa/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/locale/fa/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5726 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/locale/fa/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.496449 django_import_export-4.0.1/import_export/locale/fi/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.524449 django_import_export-4.0.1/import_export/locale/fi/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/locale/fi/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5140 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/locale/fi/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.496449 django_import_export-4.0.1/import_export/locale/fr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.524449 django_import_export-4.0.1/import_export/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5108 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.496449 django_import_export-4.0.1/import_export/locale/it/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.524449 django_import_export-4.0.1/import_export/locale/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/locale/it/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5067 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/locale/it/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.500449 django_import_export-4.0.1/import_export/locale/ja/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.524449 django_import_export-4.0.1/import_export/locale/ja/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/locale/ja/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5194 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/locale/ja/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.500449 django_import_export-4.0.1/import_export/locale/ko/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.524449 django_import_export-4.0.1/import_export/locale/ko/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/locale/ko/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5371 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/locale/ko/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.500449 django_import_export-4.0.1/import_export/locale/kz/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.524449 django_import_export-4.0.1/import_export/locale/kz/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/locale/kz/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5913 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/locale/kz/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.500449 django_import_export-4.0.1/import_export/locale/nl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.524449 django_import_export-4.0.1/import_export/locale/nl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/locale/nl/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5456 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/locale/nl/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.500449 django_import_export-4.0.1/import_export/locale/pl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.528449 django_import_export-4.0.1/import_export/locale/pl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/locale/pl/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5280 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/locale/pl/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.500449 django_import_export-4.0.1/import_export/locale/pt_BR/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.528449 django_import_export-4.0.1/import_export/locale/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/locale/pt_BR/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5405 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/locale/pt_BR/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.500449 django_import_export-4.0.1/import_export/locale/ru/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.528449 django_import_export-4.0.1/import_export/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     5198 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     7399 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.500449 django_import_export-4.0.1/import_export/locale/sk/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.528449 django_import_export-4.0.1/import_export/locale/sk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/locale/sk/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5113 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/locale/sk/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.500449 django_import_export-4.0.1/import_export/locale/tr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.528449 django_import_export-4.0.1/import_export/locale/tr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/locale/tr/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5465 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/locale/tr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.500449 django_import_export-4.0.1/import_export/locale/zh_Hans/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.528449 django_import_export-4.0.1/import_export/locale/zh_Hans/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/locale/zh_Hans/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5238 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/locale/zh_Hans/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (127)     8064 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6543 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49322 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8079 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/results.py
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.500449 django_import_export-4.0.1/import_export/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.528449 django_import_export-4.0.1/import_export/static/import_export/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/static/import_export/export.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/static/import_export/export_selectable_fields.js
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/static/import_export/guess_format.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/static/import_export/import.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.500449 django_import_export-4.0.1/import_export/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.500449 django_import_export-4.0.1/import_export/templates/admin/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.532449 django_import_export-4.0.1/import_export/templates/admin/import_export/
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/templates/admin/import_export/base.html
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/templates/admin/import_export/change_form.html
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/templates/admin/import_export/change_list.html
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/templates/admin/import_export/change_list_export.html
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/templates/admin/import_export/change_list_export_item.html
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/templates/admin/import_export/change_list_import.html
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/templates/admin/import_export/change_list_import_export.html
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/templates/admin/import_export/change_list_import_item.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/templates/admin/import_export/export.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6686 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/templates/admin/import_export/import.html
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/templates/admin/import_export/resource_fields_list.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.532449 django_import_export-4.0.1/import_export/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/templatetags/import_export_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/tmp_storages.py
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21360 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/widgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-05-08 08:57:10.000000 django_import_export-4.0.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.532449 django_import_export-4.0.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-08 08:57:10.000000 django_import_export-4.0.1/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-08 08:57:10.000000 django_import_export-4.0.1/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-08 08:57:10.000000 django_import_export-4.0.1/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-05-08 08:57:10.000000 django_import_export-4.0.1/runtests.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      884 2024-05-08 08:57:10.000000 django_import_export-4.0.1/runtests.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 08:57:18.552449 django_import_export-4.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 08:57:10.000000 django_import_export-4.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.532449 django_import_export-4.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/books-sample.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.532449 django_import_export-4.0.1/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3360 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.536449 django_import_export-4.0.1/tests/core/exports/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/exports/authors.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/exports/books-ISO-8859-1.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/exports/books-dos.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     9650 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/exports/books-empty-author-email.xlsx
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/exports/books-for-delete.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/exports/books-invalid-date.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/exports/books-mac.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/exports/books-mac.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/exports/books-no-headers.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/exports/books-unicode.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/exports/books-unicode.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/exports/books.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/exports/books.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5632 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/exports/books.xls
+-rw-r--r--   0 runner    (1001) docker     (127)     4886 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/exports/books.xlsx
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/exports/child.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.536449 django_import_export-4.0.1/tests/core/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/fixtures/author.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/fixtures/book.json
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/fixtures/category.json
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.540449 django_import_export-4.0.1/tests/core/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     5662 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/migrations/0002_book_published_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/migrations/0003_withfloatfield.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/migrations/0004_bookwithchapters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/migrations/0005_addparentchild.py
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/migrations/0006_auto_20171130_0147.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/migrations/0007_auto_20180628_0411.py
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/migrations/0008_auto_20190409_0846.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3131 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/migrations/0009_auto_20211111_0807.py
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/migrations/0010_uuidbook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/migrations/0011_uuidcategory_legacybook_alter_uuidbook_id_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/migrations/0012_delete_legacybook.py
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/migrations/0013_alter_author_birthday.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/migrations/0014_bookwithchapternumbers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/migrations/0015_withpositiveintegerfields.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5102 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.500449 django_import_export-4.0.1/tests/core/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.540449 django_import_export-4.0.1/tests/core/templates/core/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.540449 django_import_export-4.0.1/tests/core/templates/core/admin/
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/templates/core/admin/change_list.html
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/templates/core/category_list.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.544449 django_import_export-4.0.1/tests/core/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.544449 django_import_export-4.0.1/tests/core/tests/admin_integration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/tests/admin_integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/tests/admin_integration/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7657 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/tests/admin_integration/test_action_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17599 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/tests/admin_integration/test_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39062 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/tests/admin_integration/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/tests/admin_integration/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/tests/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8043 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/tests/test_base_formats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3706 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/tests/test_declarative.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5318 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/tests/test_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7211 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/tests/test_forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/tests/test_import_export_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/tests/test_instance_loaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/tests/test_invalidrow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11181 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/tests/test_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7385 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/tests/test_model_resource_fields_generate_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4622 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/tests/test_permissions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.544449 django_import_export-4.0.1/tests/core/tests/test_resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/tests/test_resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22130 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/tests/test_resources/test_bulk_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4295 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/tests/test_resources/test_diffs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14330 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/tests/test_resources/test_import_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/tests/test_resources/test_misc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.548449 django_import_export-4.0.1/tests/core/tests/test_resources/test_modelresource/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/tests/test_resources/test_modelresource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6300 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/tests/test_resources/test_modelresource/test_data_deletion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4626 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/tests/test_resources/test_modelresource/test_data_handling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5698 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/tests/test_resources/test_modelresource/test_data_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/tests/test_resources/test_modelresource/test_deprecated_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13486 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/tests/test_resources/test_modelresource/test_dynamic_customization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6718 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/tests/test_resources/test_modelresource/test_error_handling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2810 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/tests/test_resources/test_modelresource/test_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/tests/test_resources/test_modelresource/test_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5596 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/tests/test_resources/test_modelresource/test_m2m.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/tests/test_resources/test_modelresource/test_queryset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/tests/test_resources/test_modelresource/test_relationship.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3661 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/tests/test_resources/test_modelresource/test_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/tests/test_resources/test_modelresource/test_resource_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6083 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/tests/test_resources/test_modelresource/test_resource_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7346 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/tests/test_resources/test_modelresource/test_resource_postgres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/tests/test_resources/test_modelresource/test_resource_setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4598 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/tests/test_resources/test_modelresource/test_resource_transactions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/tests/test_resources/test_modelresource/test_string_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/tests/test_resources/test_modelresource/test_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9679 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/tests/test_resources/test_relationships.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4651 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/tests/test_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5877 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/tests/test_tmp_storages.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26269 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/tests/test_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/tests/widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.504449 django_import_export-4.0.1/tests/docker/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.548449 django_import_export-4.0.1/tests/docker/db/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      146 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/docker/db/init-mysql-db.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      401 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/docker/db/init-postgres-db.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/docker-compose.yml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      320 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/manage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.548449 django_import_export-4.0.1/tests/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5341 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/scripts/bulk_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tox.ini
```

### Comparing `django_import_export-4.0.0rc3/.github/ISSUE_TEMPLATE/bug_report.md` & `django_import_export-4.0.1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/.github/ISSUE_TEMPLATE/question.md` & `django_import_export-4.0.1/.github/ISSUE_TEMPLATE/question.md`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/.github/stale.yml` & `django_import_export-4.0.1/.github/stale.yml`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/.github/workflows/release.yml` & `django_import_export-4.0.1/.github/workflows/release.yml`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     runs-on: ubuntu-latest
 
     steps:
       - uses: actions/checkout@v4
         with:
           fetch-depth: 0
       - name: Set up Python
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: "3.x"
       - name: Install pypa/build
         run: >-
           SETUPTOOLS_SCM_DEBUG=1
           python -m
           pip install
```

### Comparing `django_import_export-4.0.0rc3/.github/workflows/test.yml` & `django_import_export-4.0.1/.github/workflows/test.yml`

 * *Files 0% similar despite different names*

```diff
@@ -48,17 +48,17 @@
       run: >
         sudo /etc/init.d/mysql start
 
         mysql -e 'CREATE DATABASE ${{ env.DB_NAME }};'
         -u${{ env.IMPORT_EXPORT_MYSQL_USER }}
         -p${{ env.IMPORT_EXPORT_MYSQL_PASSWORD }}
     - name: Check out repository code
-      uses: actions/checkout@v3
+      uses: actions/checkout@v4
     - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v4
+      uses: actions/setup-python@v5
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install Dependencies
       run: |
         python -m pip install --upgrade pip
         pip install tox coverage coveralls
     - name: Run tox targets for ${{ matrix.python-version }} (sqlite)
```

### Comparing `django_import_export-4.0.0rc3/AUTHORS` & `django_import_export-4.0.1/AUTHORS`

 * *Files 2% similar despite different names*

```diff
@@ -146,7 +146,8 @@
 * EricOuma (Eric Ouma)
 * ZibingZhang (Zibing Zhang)
 * Glay00 (Gleb Gorelov)
 * PrashansaChaudhary (Prashansa Chaudhary)
 * Vedang Barhate (bvedang)
 * RobTilton (Robert Tilton)
 * ulliholtgrave
+* mishka251 (Mikhail Belov)
```

### Comparing `django_import_export-4.0.0rc3/CODE_OF_CONDUCT.md` & `django_import_export-4.0.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/LICENSE` & `django_import_export-4.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/Makefile` & `django_import_export-4.0.1/Makefile`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/PKG-INFO` & `django_import_export-4.0.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-import-export
-Version: 4.0.0rc3
+Version: 4.0.1
 Summary: Django application and library for importing and exporting data with included admin integration.
 Author-email: Bojan Mihelač <djangoimportexport@gmail.com>
 Maintainer-email: Matthew Hegarty <djangoimportexport@gmail.com>
 License: Copyright (c) Bojan Mihelac and individual contributors.
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without modification,
@@ -30,15 +30,14 @@
         
 Project-URL: Documentation, https://django-import-export.readthedocs.io/en/stable/
 Project-URL: Repository, https://github.com/django-import-export/django-import-export
 Project-URL: Changelog, https://github.com/django-import-export/django-import-export/blob/main/docs/changelog.rst
 Keywords: django,import,export
 Platform: OS Independent
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.2
 Classifier: Framework :: Django :: 5.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -71,16 +70,16 @@
 Provides-Extra: yaml
 Requires-Dist: tablib[yaml]==3.5.0; extra == "yaml"
 
 ====================
 django-import-export
 ====================
 
-.. image:: https://github.com/django-import-export/django-import-export/actions/workflows/django-import-export-ci.yml/badge.svg
-    :target: https://github.com/django-import-export/django-import-export/actions/workflows/django-import-export-ci.yml
+.. image:: https://github.com/django-import-export/django-import-export/actions/workflows/release.yml/badge.svg
+    :target: https://github.com/django-import-export/django-import-export/actions/workflows/release.yml
     :alt: Build status on Github
 
 .. image:: https://coveralls.io/repos/github/django-import-export/django-import-export/badge.svg?branch=main
     :target: https://coveralls.io/github/django-import-export/django-import-export?branch=main
 
 .. image:: https://img.shields.io/pypi/v/django-import-export.svg
     :target: https://pypi.org/project/django-import-export/
```

### Comparing `django_import_export-4.0.0rc3/README.rst` & `django_import_export-4.0.1/README.rst`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 ====================
 django-import-export
 ====================
 
-.. image:: https://github.com/django-import-export/django-import-export/actions/workflows/django-import-export-ci.yml/badge.svg
-    :target: https://github.com/django-import-export/django-import-export/actions/workflows/django-import-export-ci.yml
+.. image:: https://github.com/django-import-export/django-import-export/actions/workflows/release.yml/badge.svg
+    :target: https://github.com/django-import-export/django-import-export/actions/workflows/release.yml
     :alt: Build status on Github
 
 .. image:: https://coveralls.io/repos/github/django-import-export/django-import-export/badge.svg?branch=main
     :target: https://coveralls.io/github/django-import-export/django-import-export?branch=main
 
 .. image:: https://img.shields.io/pypi/v/django-import-export.svg
     :target: https://pypi.org/project/django-import-export/
```

### Comparing `django_import_export-4.0.0rc3/RELEASE.md` & `django_import_export-4.0.1/RELEASE.md`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/django_import_export.egg-info/PKG-INFO` & `django_import_export-4.0.1/django_import_export.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-import-export
-Version: 4.0.0rc3
+Version: 4.0.1
 Summary: Django application and library for importing and exporting data with included admin integration.
 Author-email: Bojan Mihelač <djangoimportexport@gmail.com>
 Maintainer-email: Matthew Hegarty <djangoimportexport@gmail.com>
 License: Copyright (c) Bojan Mihelac and individual contributors.
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without modification,
@@ -30,15 +30,14 @@
         
 Project-URL: Documentation, https://django-import-export.readthedocs.io/en/stable/
 Project-URL: Repository, https://github.com/django-import-export/django-import-export
 Project-URL: Changelog, https://github.com/django-import-export/django-import-export/blob/main/docs/changelog.rst
 Keywords: django,import,export
 Platform: OS Independent
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.2
 Classifier: Framework :: Django :: 5.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -71,16 +70,16 @@
 Provides-Extra: yaml
 Requires-Dist: tablib[yaml]==3.5.0; extra == "yaml"
 
 ====================
 django-import-export
 ====================
 
-.. image:: https://github.com/django-import-export/django-import-export/actions/workflows/django-import-export-ci.yml/badge.svg
-    :target: https://github.com/django-import-export/django-import-export/actions/workflows/django-import-export-ci.yml
+.. image:: https://github.com/django-import-export/django-import-export/actions/workflows/release.yml/badge.svg
+    :target: https://github.com/django-import-export/django-import-export/actions/workflows/release.yml
     :alt: Build status on Github
 
 .. image:: https://coveralls.io/repos/github/django-import-export/django-import-export/badge.svg?branch=main
     :target: https://coveralls.io/github/django-import-export/django-import-export?branch=main
 
 .. image:: https://img.shields.io/pypi/v/django-import-export.svg
     :target: https://pypi.org/project/django-import-export/
```

### Comparing `django_import_export-4.0.0rc3/django_import_export.egg-info/SOURCES.txt` & `django_import_export-4.0.1/django_import_export.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -194,36 +194,38 @@
 tests/core/migrations/0008_auto_20190409_0846.py
 tests/core/migrations/0009_auto_20211111_0807.py
 tests/core/migrations/0010_uuidbook.py
 tests/core/migrations/0011_uuidcategory_legacybook_alter_uuidbook_id_and_more.py
 tests/core/migrations/0012_delete_legacybook.py
 tests/core/migrations/0013_alter_author_birthday.py
 tests/core/migrations/0014_bookwithchapternumbers.py
+tests/core/migrations/0015_withpositiveintegerfields.py
 tests/core/migrations/__init__.py
 tests/core/templates/core/category_list.html
 tests/core/templates/core/admin/change_list.html
 tests/core/tests/__init__.py
 tests/core/tests/resources.py
 tests/core/tests/test_base_formats.py
 tests/core/tests/test_declarative.py
 tests/core/tests/test_fields.py
 tests/core/tests/test_forms.py
 tests/core/tests/test_import_export_tags.py
 tests/core/tests/test_instance_loaders.py
 tests/core/tests/test_invalidrow.py
 tests/core/tests/test_mixins.py
+tests/core/tests/test_model_resource_fields_generate_widgets.py
 tests/core/tests/test_permissions.py
 tests/core/tests/test_results.py
 tests/core/tests/test_tmp_storages.py
 tests/core/tests/test_widgets.py
 tests/core/tests/utils.py
 tests/core/tests/widget.py
 tests/core/tests/admin_integration/__init__.py
 tests/core/tests/admin_integration/mixins.py
-tests/core/tests/admin_integration/test_action.py
+tests/core/tests/admin_integration/test_action_export.py
 tests/core/tests/admin_integration/test_export.py
 tests/core/tests/admin_integration/test_import.py
 tests/core/tests/admin_integration/test_views.py
 tests/core/tests/test_resources/__init__.py
 tests/core/tests/test_resources/test_bulk_operations.py
 tests/core/tests/test_resources/test_diffs.py
 tests/core/tests/test_resources/test_import_export.py
```

### Comparing `django_import_export-4.0.0rc3/docs/Makefile` & `django_import_export-4.0.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/docs/_static/images/change-form-export.png` & `django_import_export-4.0.1/docs/_static/images/change-form-export.png`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/docs/_static/images/custom-export-form.png` & `django_import_export-4.0.1/docs/_static/images/custom-export-form.png`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/docs/_static/images/custom-import-form.png` & `django_import_export-4.0.1/docs/_static/images/custom-import-form.png`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/docs/_static/images/date-widget-validation-error.png` & `django_import_export-4.0.1/docs/_static/images/date-widget-validation-error.png`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/docs/_static/images/django-import-export-change.png` & `django_import_export-4.0.1/docs/_static/images/django-import-export-change.png`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/docs/_static/images/django-import-export-export-confirm.png` & `django_import_export-4.0.1/docs/_static/images/django-import-export-export-confirm.png`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/docs/_static/images/django-import-export-import-confirm.png` & `django_import_export-4.0.1/docs/_static/images/django-import-export-import-confirm.png`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/docs/_static/images/django-import-export-import.png` & `django_import_export-4.0.1/docs/_static/images/django-import-export-import.png`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/docs/_static/images/export-button.png` & `django_import_export-4.0.1/docs/_static/images/export-button.png`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/docs/_static/images/export_workflow.svg` & `django_import_export-4.0.1/docs/_static/images/export_workflow.svg`

 * *Files 7% similar despite different names*

```diff
@@ -1,2081 +1,2107 @@
 00000000: 3c73 7667 2076 6572 7369 6f6e 3d22 312e  <svg version="1.
 00000010: 3122 2078 6d6c 6e73 3d22 6874 7470 3a2f  1" xmlns="http:/
 00000020: 2f77 7777 2e77 332e 6f72 672f 3230 3030  /www.w3.org/2000
 00000030: 2f73 7667 2220 786d 6c6e 733a 786c 696e  /svg" xmlns:xlin
 00000040: 6b3d 2268 7474 703a 2f2f 7777 772e 7733  k="http://www.w3
 00000050: 2e6f 7267 2f31 3939 392f 786c 696e 6b22  .org/1999/xlink"
-00000060: 2077 6964 7468 3d22 3131 3036 2220 6865   width="1106" he
+00000060: 2077 6964 7468 3d22 3130 3638 2220 6865   width="1068" he
 00000070: 6967 6874 3d22 3136 3337 223e 3c64 6573  ight="1637"><des
-00000080: 633e 7061 7274 6963 6970 616e 7425 3230  c>participant%20
-00000090: 5265 736f 7572 6365 2530 4170 6172 7469  Resource%0Aparti
-000000a0: 6369 7061 6e74 2532 3046 6965 6c64 2530  cipant%20Field%0
-000000b0: 4170 6172 7469 6369 7061 6e74 2532 3057  Aparticipant%20W
-000000c0: 6964 6765 7425 3041 7061 7274 6963 6970  idget%0Aparticip
-000000d0: 616e 7425 3230 7461 626c 6962 2e44 6174  ant%20tablib.Dat
-000000e0: 6173 6574 2530 4125 3041 5265 736f 7572  aset%0A%0AResour
-000000f0: 6365 2d25 3345 5265 736f 7572 6365 2533  ce-%3EResource%3
-00000100: 4125 3232 2532 3265 7870 6f72 7428 7175  A%22%22export(qu
-00000110: 6572 7973 6574 2533 444e 6f6e 6525 3243  eryset%3DNone%2C
-00000120: 2532 3025 3543 2a25 3543 2a6b 7761 7267  %20%5C*%5C*kwarg
-00000130: 7329 2532 3225 3232 2530 4161 6374 6976  s)%22%22%0Aactiv
-00000140: 6174 6525 3230 5265 736f 7572 6365 2530  ate%20Resource%0
-00000150: 4125 3041 5265 736f 7572 6365 2d25 3345  A%0AResource-%3E
-00000160: 5265 736f 7572 6365 2533 4125 3343 6261  Resource%3A%3Cba
-00000170: 636b 6772 6f75 6e64 2533 4125 3233 7965  ckground%3A%23ye
-00000180: 6c6c 6f77 2533 4525 3232 2532 3262 6566  llow%3E%22%22bef
-00000190: 6f72 655f 6578 706f 7274 2871 7565 7279  ore_export(query
-000001a0: 7365 7425 3344 4e6f 6e65 2532 4325 3230  set%3DNone%2C%20
-000001b0: 2535 432a 2535 432a 6b77 6172 6773 2925  %5C*%5C*kwargs)%
-000001c0: 3232 2532 3225 3041 2530 416e 6f74 6525  22%22%0A%0Anote%
-000001d0: 3230 6f76 6572 2532 3052 6573 6f75 7263  20over%20Resourc
-000001e0: 6525 3341 2532 3041 2532 3051 7565 7279  e%3A%20A%20Query
-000001f0: 7365 7425 3230 696e 7374 616e 6365 2532  set%20instance%2
-00000200: 3063 616e 2532 3062 6525 3230 7061 7373  0can%20be%20pass
-00000210: 6564 2532 3069 6e74 6f25 3230 6578 706f  ed%20into%20expo
-00000220: 7274 2829 2e25 3543 6e49 6625 3230 6e6f  rt().%5CnIf%20no
-00000230: 2532 3051 7565 7279 7365 7425 3230 6973  %20Queryset%20is
-00000240: 2532 3070 6173 7365 6425 3243 2532 3067  %20passed%2C%20g
-00000250: 6574 5f71 7565 7279 7365 7428 2925 3230  et_queryset()%20
-00000260: 6973 2532 3063 616c 6c65 642e 2530 4125  is%20called.%0A%
-00000270: 3041 5265 736f 7572 6365 2d25 3345 5265  0AResource-%3ERe
-00000280: 736f 7572 6365 2533 4125 3343 6261 636b  source%3A%3Cback
-00000290: 6772 6f75 6e64 2533 4125 3233 7965 6c6c  ground%3A%23yell
-000002a0: 6f77 2533 4525 3232 2532 3267 6574 5f71  ow%3E%22%22get_q
-000002b0: 7565 7279 7365 7428 2925 3232 2532 3225  ueryset()%22%22%
-000002c0: 3041 6163 7469 7661 7465 2532 3052 6573  0Aactivate%20Res
-000002d0: 6f75 7263 6525 3230 2532 336c 6967 6874  ource%20%23light
-000002e0: 626c 7565 2530 4152 6573 6f75 7263 6525  blue%0AResource%
-000002f0: 3343 2d2d 5265 736f 7572 6365 2533 4125  3C--Resource%3A%
-00000300: 3232 2532 3251 7565 7279 7365 7425 3232  22%22Queryset%22
-00000310: 2532 3225 3041 6465 6163 7469 7661 7465  %22%0Adeactivate
-00000320: 2532 3052 6573 6f75 7263 6525 3041 2530  %20Resource%0A%0
-00000330: 4152 6573 6f75 7263 652d 2533 4552 6573  AResource-%3ERes
-00000340: 6f75 7263 6525 3341 2533 4362 6163 6b67  ource%3A%3Cbackg
-00000350: 726f 756e 6425 3341 2532 3379 656c 6c6f  round%3A%23yello
-00000360: 7725 3345 2532 3225 3232 6669 6c74 6572  w%3E%22%22filter
-00000370: 5f65 7870 6f72 7428 7175 6572 7973 6574  _export(queryset
-00000380: 2532 4325 3230 2535 432a 2535 432a 6b77  %2C%20%5C*%5C*kw
-00000390: 6172 6773 2925 3232 2532 3225 3041 6163  args)%22%22%0Aac
-000003a0: 7469 7661 7465 2532 3052 6573 6f75 7263  tivate%20Resourc
-000003b0: 6525 3230 2532 336c 6967 6874 626c 7565  e%20%23lightblue
-000003c0: 2530 4152 6573 6f75 7263 6525 3343 2d2d  %0AResource%3C--
-000003d0: 5265 736f 7572 6365 2533 4125 3232 2532  Resource%3A%22%2
-000003e0: 3251 7565 7279 7365 7425 3232 2532 3225  2Queryset%22%22%
-000003f0: 3041 6465 6163 7469 7661 7465 2532 3052  0Adeactivate%20R
-00000400: 6573 6f75 7263 6525 3041 2530 416c 6f6f  esource%0A%0Aloo
-00000410: 7025 3230 2532 3370 696e 6b25 3230 6561  p%20%23pink%20ea
-00000420: 6368 2532 3072 6f77 2532 3069 6e25 3230  ch%20row%20in%20
-00000430: 5175 6572 7973 6574 2530 4125 3041 5265  Queryset%0A%0ARe
-00000440: 736f 7572 6365 2d25 3345 5265 736f 7572  source-%3EResour
-00000450: 6365 2533 4125 3343 6261 636b 6772 6f75  ce%3A%3Cbackgrou
-00000460: 6e64 2533 4125 3233 7965 6c6c 6f77 2533  nd%3A%23yellow%3
-00000470: 4525 3232 2532 3265 7870 6f72 745f 7265  E%22%22export_re
-00000480: 736f 7572 6365 2869 6e73 7461 6e63 6529  source(instance)
-00000490: 2532 3225 3232 2530 4161 6374 6976 6174  %22%22%0Aactivat
-000004a0: 6525 3230 5265 736f 7572 6365 2532 3025  e%20Resource%20%
-000004b0: 3233 6c69 6768 7462 6c75 6525 3041 2530  23lightblue%0A%0
-000004c0: 416c 6f6f 7025 3230 2532 3367 7265 656e  Aloop%20%23green
-000004d0: 2532 3065 6163 6825 3230 6669 656c 6425  %20each%20field%
-000004e0: 3230 696e 2532 3065 7870 6f72 7425 3230  20in%20export%20
-000004f0: 6669 656c 6425 3230 6c69 7374 2530 4152  field%20list%0AR
-00000500: 6573 6f75 7263 652d 2533 4552 6573 6f75  esource-%3EResou
-00000510: 7263 6525 3341 2532 3225 3232 6578 706f  rce%3A%22%22expo
-00000520: 7274 5f66 6965 6c64 2866 6965 6c64 2532  rt_field(field%2
-00000530: 4325 3230 696e 7374 616e 6365 2925 3232  C%20instance)%22
-00000540: 2532 3225 3041 6163 7469 7661 7465 2532  %22%0Aactivate%2
-00000550: 3052 6573 6f75 7263 6525 3230 2532 336c  0Resource%20%23l
-00000560: 6967 6874 7069 6e6b 2530 4152 6573 6f75  ightpink%0AResou
-00000570: 7263 652d 2533 4546 6965 6c64 2533 4125  rce-%3EField%3A%
-00000580: 3232 2532 3265 7870 6f72 7428 696e 7374  22%22export(inst
-00000590: 616e 6365 2925 3232 2532 3225 3041 6163  ance)%22%22%0Aac
-000005a0: 7469 7661 7465 2532 3046 6965 6c64 2532  tivate%20Field%2
-000005b0: 3025 3233 6c69 6768 7462 6c75 6525 3041  0%23lightblue%0A
-000005c0: 6e6f 7465 2532 306f 7665 7225 3230 4669  note%20over%20Fi
-000005d0: 656c 6425 3341 2532 3041 6e25 3230 6f70  eld%3A%20An%20op
-000005e0: 7469 6f6e 616c 2532 3063 616c 6c61 626c  tional%20callabl
-000005f0: 6525 3230 6361 6e25 3230 6265 2532 3064  e%20can%20be%20d
-00000600: 6566 696e 6564 2532 3069 6e73 7465 6164  efined%20instead
-00000610: 2532 306f 6625 3230 6578 706f 7274 2829  %20of%20export()
-00000620: 2e25 3543 6e25 3230 5365 6525 3230 2764  .%5Cn%20See%20'd
-00000630: 6568 7964 7261 7465 2725 3230 6d65 7468  ehydrate'%20meth
-00000640: 6f64 7325 3230 696e 2532 3064 6f63 732e  ods%20in%20docs.
-00000650: 2530 4146 6965 6c64 2d25 3345 4669 656c  %0AField-%3EFiel
-00000660: 6425 3341 2532 3225 3232 6765 745f 7661  d%3A%22%22get_va
-00000670: 6c75 6528 696e 7374 616e 6365 2925 3232  lue(instance)%22
-00000680: 2532 3225 3041 6163 7469 7661 7465 2532  %22%0Aactivate%2
-00000690: 3046 6965 6c64 2532 3025 3233 6c69 6768  0Field%20%23ligh
-000006a0: 7470 696e 6b25 3041 6e6f 7465 2532 306f  tpink%0Anote%20o
-000006b0: 7665 7225 3230 4669 656c 6425 3341 2532  ver%20Field%3A%2
-000006c0: 3047 6574 2532 3074 6865 2532 3066 6965  0Get%20the%20fie
-000006d0: 6c64 2773 2532 3076 616c 7565 2532 3066  ld's%20value%20f
-000006e0: 726f 6d25 3230 7468 6525 3230 696e 7374  rom%20the%20inst
-000006f0: 616e 6365 2e25 3041 4669 656c 6425 3343  ance.%0AField%3C
-00000700: 2d2d 4669 656c 6425 3341 2532 3225 3232  --Field%3A%22%22
-00000710: 2533 4325 3343 7661 6c75 6525 3345 2533  %3C%3Cvalue%3E%3
-00000720: 4525 3232 2532 3225 3041 4669 656c 642d  E%22%22%0AField-
-00000730: 2533 4557 6964 6765 7425 3341 2532 3225  %3EWidget%3A%22%
-00000740: 3232 7265 6e64 6572 2876 616c 7565 2532  22render(value%2
-00000750: 4325 3230 696e 7374 616e 6365 2925 3232  C%20instance)%22
-00000760: 2532 3225 3041 6163 7469 7661 7465 2532  %22%0Aactivate%2
-00000770: 3057 6964 6765 7425 3041 6e6f 7465 2532  0Widget%0Anote%2
-00000780: 306f 7665 7225 3230 5769 6467 6574 2533  0over%20Widget%3
-00000790: 4125 3230 466f 726d 6174 2532 3066 6965  A%20Format%20fie
-000007a0: 6c64 2532 3076 616c 7565 2532 3069 6e74  ld%20value%20int
-000007b0: 6f25 3230 6125 3543 6e73 7472 696e 6725  o%20a%5Cnstring%
-000007c0: 3230 6f72 2532 3076 616c 7565 2532 3061  20or%20value%20a
-000007d0: 7325 3230 7265 7175 6972 6564 2e25 3041  s%20required.%0A
-000007e0: 4669 656c 6425 3343 2d2d 5769 6467 6574  Field%3C--Widget
-000007f0: 2533 4125 3232 2532 3225 3343 2533 4376  %3A%22%22%3C%3Cv
-00000800: 616c 7565 2533 4525 3345 2530 4164 6561  alue%3E%3E%0Adea
-00000810: 6374 6976 6174 6525 3230 5769 6467 6574  ctivate%20Widget
-00000820: 2530 4164 6561 6374 6976 6174 6525 3230  %0Adeactivate%20
-00000830: 4669 656c 6425 3041 5265 736f 7572 6365  Field%0AResource
-00000840: 2533 432d 2d46 6965 6c64 2533 4125 3232  %3C--Field%3A%22
-00000850: 2532 3225 3343 2533 4376 616c 7565 2533  %22%3C%3Cvalue%3
-00000860: 4525 3345 2532 3225 3232 2530 4164 6561  E%3E%22%22%0Adea
-00000870: 6374 6976 6174 6525 3230 4669 656c 6425  ctivate%20Field%
-00000880: 3041 6465 6163 7469 7661 7465 2532 3052  0Adeactivate%20R
-00000890: 6573 6f75 7263 6525 3041 656e 6425 3041  esource%0Aend%0A
-000008a0: 6465 6163 7469 7661 7465 2532 3052 6573  deactivate%20Res
-000008b0: 6f75 7263 6525 3041 2530 4152 6573 6f75  ource%0A%0AResou
-000008c0: 7263 652d 2533 4574 6162 6c69 622e 4461  rce-%3Etablib.Da
-000008d0: 7461 7365 7425 3341 2532 3225 3232 6170  taset%3A%22%22ap
-000008e0: 7065 6e64 2829 2532 3225 3232 2530 4165  pend()%22%22%0Ae
-000008f0: 6e64 2530 4125 3041 5265 736f 7572 6365  nd%0A%0AResource
-00000900: 2533 432d 2d52 6573 6f75 7263 6525 3341  %3C--Resource%3A
-00000910: 2532 3225 3232 2533 4325 3343 4461 7461  %22%22%3C%3CData
-00000920: 7365 7425 3345 2533 4525 3232 2532 3225  set%3E%3E%22%22%
-00000930: 3041 6465 6163 7469 7661 7465 2532 3052  0Adeactivate%20R
-00000940: 6573 6f75 7263 6525 3041 2530 4125 3041  esource%0A%0A%0A
-00000950: 3c2f 6465 7363 3e3c 6465 6673 2f3e 3c67  </desc><defs/><g
-00000960: 3e3c 672f 3e3c 672f 3e3c 672f 3e3c 672f  ><g/><g/><g/><g/
-00000970: 3e3c 672f 3e3c 672f 3e3c 672f 3e3c 672f  ><g/><g/><g/><g/
-00000980: 3e3c 672f 3e3c 672f 3e3c 672f 3e3c 672f  ><g/><g/><g/><g/
-00000990: 3e3c 672f 3e3c 672f 3e3c 672f 3e3c 672f  ><g/><g/><g/><g/
-000009a0: 3e3c 672f 3e3c 672f 3e3c 672f 3e3c 672f  ><g/><g/><g/><g/
-000009b0: 3e3c 672f 3e3c 672f 3e3c 672f 3e3c 673e  ><g/><g/><g/><g>
-000009c0: 3c72 6563 7420 6669 6c6c 3d22 7768 6974  <rect fill="whit
-000009d0: 6522 2073 7472 6f6b 653d 226e 6f6e 6522  e" stroke="none"
-000009e0: 2078 3d22 3022 2079 3d22 3022 2077 6964   x="0" y="0" wid
-000009f0: 7468 3d22 3131 3036 2220 6865 6967 6874  th="1106" height
-00000a00: 3d22 3136 3337 222f 3e3c 2f67 3e3c 673e  ="1637"/></g><g>
-00000a10: 3c72 6563 7420 6669 6c6c 3d22 7267 6228  <rect fill="rgb(
-00000a20: 3235 352c 3234 322c 3234 3529 2220 7374  255,242,245)" st
-00000a30: 726f 6b65 3d22 6e6f 6e65 2220 783d 2239  roke="none" x="9
-00000a40: 372e 3630 3031 3639 3537 3538 3230 3332  7.60016957582032
-00000a50: 2220 793d 2236 3131 2e36 3635 3430 3437  " y="611.6654047
-00000a60: 3937 3939 3939 2220 7769 6474 683d 2239  979999" width="9
-00000a70: 3931 2e30 3932 3935 3339 3634 3139 3932  91.0929539641992
-00000a80: 2220 6865 6967 6874 3d22 3839 312e 3930  " height="891.90
-00000a90: 3231 3030 3137 3939 3939 3622 2f3e 3c72  21001799996"/><r
-00000aa0: 6563 7420 6669 6c6c 3d22 7267 6228 3230  ect fill="rgb(20
-00000ab0: 342c 3233 302c 3230 3429 2220 7374 726f  4,230,204)" stro
-00000ac0: 6b65 3d22 6e6f 6e65 2220 783d 2231 3135  ke="none" x="115
-00000ad0: 2e31 3931 3932 3639 3735 3832 3033 3222  .19192697582032"
-00000ae0: 2079 3d22 3733 312e 3238 3933 3535 3131   y="731.28935511
-00000af0: 3739 3939 3922 2077 6964 7468 3d22 3838  79999" width="88
-00000b00: 352e 3534 3234 3039 3536 3431 3939 3122  5.5424095641991"
-00000b10: 2068 6569 6768 743d 2236 3936 2e36 3333   height="696.633
-00000b20: 3539 3330 3339 3939 3937 222f 3e3c 2f67  5930399997"/></g
-00000b30: 3e3c 673e 3c70 6174 6820 6669 6c6c 3d22  ><g><path fill="
-00000b40: 6e6f 6e65 2220 7374 726f 6b65 3d22 626c  none" stroke="bl
-00000b50: 6163 6b22 2070 6169 6e74 2d6f 7264 6572  ack" paint-order
-00000b60: 3d22 6669 6c6c 2073 7472 6f6b 6520 6d61  ="fill stroke ma
-00000b70: 726b 6572 7322 2064 3d22 204d 2032 3033  rkers" d=" M 203
-00000b80: 2e31 3530 3731 3339 3735 3832 3033 2035  .1507139758203 5
-00000b90: 392e 3238 3432 3232 3433 3739 3939 3938  9.28422243799998
-00000ba0: 3620 4c20 3230 332e 3135 3037 3133 3937  6 L 203.15071397
-00000bb0: 3538 3230 3320 3136 3337 2e32 3634 3836  58203 1637.26486
-00000bc0: 3132 3137 3939 3936 2220 7374 726f 6b65  12179996" stroke
-00000bd0: 2d6d 6974 6572 6c69 6d69 743d 2231 3022  -miterlimit="10"
-00000be0: 2073 7472 6f6b 652d 7769 6474 683d 2231   stroke-width="1
-00000bf0: 2e34 3635 3937 3937 3833 3333 3333 3333  .465979783333333
-00000c00: 3222 2073 7472 6f6b 652d 6461 7368 6172  2" stroke-dashar
-00000c10: 7261 793d 2231 332e 3533 3231 3231 3037  ray="13.53212107
-00000c20: 3639 3233 3037 362c 352e 3836 3339 3139  6923076,5.863919
-00000c30: 3133 3333 3333 3333 3322 2f3e 3c70 6174  133333333"/><pat
-00000c40: 6820 6669 6c6c 3d22 6e6f 6e65 2220 7374  h fill="none" st
-00000c50: 726f 6b65 3d22 626c 6163 6b22 2070 6169  roke="black" pai
-00000c60: 6e74 2d6f 7264 6572 3d22 6669 6c6c 2073  nt-order="fill s
-00000c70: 7472 6f6b 6520 6d61 726b 6572 7322 2064  troke markers" d
-00000c80: 3d22 204d 2036 3034 2e38 3837 3930 3830  =" M 604.8879080
-00000c90: 3332 3539 3132 2035 392e 3238 3432 3232  325912 59.284222
-00000ca0: 3433 3739 3939 3938 3620 4c20 3630 342e  437999986 L 604.
-00000cb0: 3838 3739 3038 3033 3235 3931 3220 3136  8879080325912 16
-00000cc0: 3337 2e32 3634 3836 3132 3137 3939 3936  37.2648612179996
-00000cd0: 2220 7374 726f 6b65 2d6d 6974 6572 6c69  " stroke-miterli
-00000ce0: 6d69 743d 2231 3022 2073 7472 6f6b 652d  mit="10" stroke-
-00000cf0: 7769 6474 683d 2231 2e34 3635 3937 3937  width="1.4659797
-00000d00: 3833 3333 3333 3333 3222 2073 7472 6f6b  833333332" strok
-00000d10: 652d 6461 7368 6172 7261 793d 2231 332e  e-dasharray="13.
-00000d20: 3533 3231 3231 3037 3639 3233 3037 362c  532121076923076,
-00000d30: 352e 3836 3339 3139 3133 3333 3333 3333  5.86391913333333
-00000d40: 3322 2f3e 3c70 6174 6820 6669 6c6c 3d22  3"/><path fill="
-00000d50: 6e6f 6e65 2220 7374 726f 6b65 3d22 626c  none" stroke="bl
-00000d60: 6163 6b22 2070 6169 6e74 2d6f 7264 6572  ack" paint-order
-00000d70: 3d22 6669 6c6c 2073 7472 6f6b 6520 6d61  ="fill stroke ma
-00000d80: 726b 6572 7322 2064 3d22 204d 2038 3830  rkers" d=" M 880
-00000d90: 2e35 3237 3635 3634 3736 3630 3136 2035  .5276564766016 5
-00000da0: 392e 3238 3432 3232 3433 3739 3939 3938  9.28422243799998
-00000db0: 3620 4c20 3838 302e 3532 3736 3536 3437  6 L 880.52765647
-00000dc0: 3636 3031 3620 3136 3337 2e32 3634 3836  66016 1637.26486
-00000dd0: 3132 3137 3939 3936 2220 7374 726f 6b65  12179996" stroke
-00000de0: 2d6d 6974 6572 6c69 6d69 743d 2231 3022  -miterlimit="10"
-00000df0: 2073 7472 6f6b 652d 7769 6474 683d 2231   stroke-width="1
-00000e00: 2e34 3635 3937 3937 3833 3333 3333 3333  .465979783333333
-00000e10: 3222 2073 7472 6f6b 652d 6461 7368 6172  2" stroke-dashar
-00000e20: 7261 793d 2231 332e 3533 3231 3231 3037  ray="13.53212107
-00000e30: 3639 3233 3037 362c 352e 3836 3339 3139  6923076,5.863919
-00000e40: 3133 3333 3333 3333 3322 2f3e 3c70 6174  133333333"/><pat
-00000e50: 6820 6669 6c6c 3d22 6e6f 6e65 2220 7374  h fill="none" st
-00000e60: 726f 6b65 3d22 626c 6163 6b22 2070 6169  roke="black" pai
-00000e70: 6e74 2d6f 7264 6572 3d22 6669 6c6c 2073  nt-order="fill s
-00000e80: 7472 6f6b 6520 6d61 726b 6572 7322 2064  troke markers" d
-00000e90: 3d22 204d 2031 3032 372e 3132 3139 3732  =" M 1027.121972
-00000ea0: 3634 3030 3139 3520 3539 2e32 3834 3232  6400195 59.28422
-00000eb0: 3234 3337 3939 3939 3836 204c 2031 3032  2437999986 L 102
-00000ec0: 372e 3132 3139 3732 3634 3030 3139 3520  7.1219726400195 
-00000ed0: 3136 3337 2e32 3634 3836 3132 3137 3939  1637.26486121799
-00000ee0: 3936 2220 7374 726f 6b65 2d6d 6974 6572  96" stroke-miter
-00000ef0: 6c69 6d69 743d 2231 3022 2073 7472 6f6b  limit="10" strok
-00000f00: 652d 7769 6474 683d 2231 2e34 3635 3937  e-width="1.46597
-00000f10: 3937 3833 3333 3333 3333 3222 2073 7472  97833333332" str
-00000f20: 6f6b 652d 6461 7368 6172 7261 793d 2231  oke-dasharray="1
-00000f30: 332e 3533 3231 3231 3037 3639 3233 3037  3.53212107692307
-00000f40: 362c 352e 3836 3339 3139 3133 3333 3333  6,5.863919133333
-00000f50: 3333 3322 2f3e 3c2f 673e 3c67 3e3c 7061  333"/></g><g><pa
-00000f60: 7468 2066 696c 6c3d 226e 6f6e 6522 2073  th fill="none" s
-00000f70: 7472 6f6b 653d 226e 6f6e 6522 2f3e 3c67  troke="none"/><g
-00000f80: 3e3c 7061 7468 2066 696c 6c3d 2277 6869  ><path fill="whi
-00000f90: 7465 2220 7374 726f 6b65 3d22 626c 6163  te" stroke="blac
-00000fa0: 6b22 2070 6169 6e74 2d6f 7264 6572 3d22  k" paint-order="
-00000fb0: 6669 6c6c 2073 7472 6f6b 6520 6d61 726b  fill stroke mark
-00000fc0: 6572 7322 2064 3d22 204d 2031 3532 2e36  ers" d=" M 152.6
-00000fd0: 3932 3837 3632 3531 3939 3631 2031 312e  928762519961 11.
-00000fe0: 3738 3634 3737 3435 3739 3939 3939 3720  786477457999997 
-00000ff0: 4c20 3235 332e 3630 3835 3531 3639 3936  L 253.6085516996
-00001000: 3434 3532 2031 312e 3738 3634 3737 3435  4452 11.78647745
-00001010: 3739 3939 3939 3720 4c20 3235 332e 3630  7999997 L 253.60
-00001020: 3835 3531 3639 3936 3434 3532 2035 392e  855169964452 59.
-00001030: 3238 3432 3232 3433 3739 3939 3938 3620  284222437999986 
-00001040: 4c20 3135 322e 3639 3238 3736 3235 3139  L 152.6928762519
-00001050: 3936 3120 3539 2e32 3834 3232 3234 3337  961 59.284222437
-00001060: 3939 3939 3836 204c 2031 3532 2e36 3932  999986 L 152.692
-00001070: 3837 3632 3531 3939 3631 2031 312e 3738  8762519961 11.78
-00001080: 3634 3737 3435 3739 3939 3939 3720 5a22  6477457999997 Z"
-00001090: 2073 7472 6f6b 652d 6d69 7465 726c 696d   stroke-miterlim
-000010a0: 6974 3d22 3130 2220 7374 726f 6b65 2d77  it="10" stroke-w
-000010b0: 6964 7468 3d22 322e 3831 3436 3831 3138  idth="2.81468118
-000010c0: 3422 2073 7472 6f6b 652d 6461 7368 6172  4" stroke-dashar
-000010d0: 7261 793d 2222 2f3e 3c2f 673e 3c67 3e3c  ray=""/></g><g><
-000010e0: 672f 3e3c 7465 7874 2066 696c 6c3d 2262  g/><text fill="b
-000010f0: 6c61 636b 2220 7374 726f 6b65 3d22 6e6f  lack" stroke="no
-00001100: 6e65 2220 666f 6e74 2d66 616d 696c 793d  ne" font-family=
-00001110: 2273 616e 732d 7365 7269 6622 2066 6f6e  "sans-serif" fon
-00001120: 742d 7369 7a65 3d22 3131 7074 2220 666f  t-size="11pt" fo
-00001130: 6e74 2d73 7479 6c65 3d22 6e6f 726d 616c  nt-style="normal
-00001140: 2220 666f 6e74 2d77 6569 6768 743d 226e  " font-weight="n
-00001150: 6f72 6d61 6c22 2074 6578 742d 6465 636f  ormal" text-deco
-00001160: 7261 7469 6f6e 3d22 6e6f 726d 616c 2220  ration="normal" 
-00001170: 783d 2231 3731 2e37 3739 3933 3330 3330  x="171.779933030
-00001180: 3939 3631 2220 793d 2234 312e 3639 3234  9961" y="41.6924
-00001190: 3635 3033 3739 3939 3939 3522 2074 6578  65037999995" tex
-000011a0: 742d 616e 6368 6f72 3d22 7374 6172 7422  t-anchor="start"
-000011b0: 2064 6f6d 696e 616e 742d 6261 7365 6c69   dominant-baseli
-000011c0: 6e65 3d22 616c 7068 6162 6574 6963 2220  ne="alphabetic" 
-000011d0: 786d 6c3a 7370 6163 653d 2270 7265 7365  xml:space="prese
-000011e0: 7276 6522 3e52 6573 6f75 7263 653c 2f74  rve">Resource</t
-000011f0: 6578 743e 3c2f 673e 3c70 6174 6820 6669  ext></g><path fi
-00001200: 6c6c 3d22 6e6f 6e65 2220 7374 726f 6b65  ll="none" stroke
-00001210: 3d22 6e6f 6e65 222f 3e3c 673e 3c70 6174  ="none"/><g><pat
-00001220: 6820 6669 6c6c 3d22 7768 6974 6522 2073  h fill="white" s
-00001230: 7472 6f6b 653d 2262 6c61 636b 2220 7061  troke="black" pa
-00001240: 696e 742d 6f72 6465 723d 2266 696c 6c20  int-order="fill 
-00001250: 7374 726f 6b65 206d 6172 6b65 7273 2220  stroke markers" 
-00001260: 643d 2220 4d20 3536 392e 3931 3332 3339  d=" M 569.913239
-00001270: 3836 3434 3331 2031 312e 3738 3634 3737  864431 11.786477
-00001280: 3435 3739 3939 3939 3720 4c20 3633 392e  457999997 L 639.
-00001290: 3836 3235 3736 3230 3037 3531 3420 3131  8625762007514 11
-000012a0: 2e37 3836 3437 3734 3537 3939 3939 3937  .786477457999997
-000012b0: 204c 2036 3339 2e38 3632 3537 3632 3030   L 639.862576200
-000012c0: 3735 3134 2035 392e 3238 3432 3232 3433  7514 59.28422243
-000012d0: 3739 3939 3938 3620 4c20 3536 392e 3931  7999986 L 569.91
-000012e0: 3332 3339 3836 3434 3331 2035 392e 3238  3239864431 59.28
-000012f0: 3432 3232 3433 3739 3939 3938 3620 4c20  4222437999986 L 
-00001300: 3536 392e 3931 3332 3339 3836 3434 3331  569.913239864431
-00001310: 2031 312e 3738 3634 3737 3435 3739 3939   11.786477457999
-00001320: 3939 3720 5a22 2073 7472 6f6b 652d 6d69  997 Z" stroke-mi
-00001330: 7465 726c 696d 6974 3d22 3130 2220 7374  terlimit="10" st
-00001340: 726f 6b65 2d77 6964 7468 3d22 322e 3831  roke-width="2.81
-00001350: 3436 3831 3138 3422 2073 7472 6f6b 652d  4681184" stroke-
-00001360: 6461 7368 6172 7261 793d 2222 2f3e 3c2f  dasharray=""/></
-00001370: 673e 3c67 3e3c 672f 3e3c 7465 7874 2066  g><g><g/><text f
-00001380: 696c 6c3d 2262 6c61 636b 2220 7374 726f  ill="black" stro
-00001390: 6b65 3d22 6e6f 6e65 2220 666f 6e74 2d66  ke="none" font-f
-000013a0: 616d 696c 793d 2273 616e 732d 7365 7269  amily="sans-seri
-000013b0: 6622 2066 6f6e 742d 7369 7a65 3d22 3131  f" font-size="11
-000013c0: 7074 2220 666f 6e74 2d73 7479 6c65 3d22  pt" font-style="
-000013d0: 6e6f 726d 616c 2220 666f 6e74 2d77 6569  normal" font-wei
-000013e0: 6768 743d 226e 6f72 6d61 6c22 2074 6578  ght="normal" tex
-000013f0: 742d 6465 636f 7261 7469 6f6e 3d22 6e6f  t-decoration="no
-00001400: 726d 616c 2220 783d 2235 3839 2e30 3030  rmal" x="589.000
-00001410: 3239 3636 3433 3433 3122 2079 3d22 3431  296643431" y="41
-00001420: 2e36 3932 3436 3530 3337 3939 3939 3935  .692465037999995
-00001430: 2220 7465 7874 2d61 6e63 686f 723d 2273  " text-anchor="s
-00001440: 7461 7274 2220 646f 6d69 6e61 6e74 2d62  tart" dominant-b
-00001450: 6173 656c 696e 653d 2261 6c70 6861 6265  aseline="alphabe
-00001460: 7469 6322 2078 6d6c 3a73 7061 6365 3d22  tic" xml:space="
-00001470: 7072 6573 6572 7665 223e 4669 656c 643c  preserve">Field<
-00001480: 2f74 6578 743e 3c2f 673e 3c70 6174 6820  /text></g><path 
-00001490: 6669 6c6c 3d22 6e6f 6e65 2220 7374 726f  fill="none" stro
-000014a0: 6b65 3d22 6e6f 6e65 222f 3e3c 673e 3c70  ke="none"/><g><p
-000014b0: 6174 6820 6669 6c6c 3d22 7768 6974 6522  ath fill="white"
-000014c0: 2073 7472 6f6b 653d 2262 6c61 636b 2220   stroke="black" 
-000014d0: 7061 696e 742d 6f72 6465 723d 2266 696c  paint-order="fil
-000014e0: 6c20 7374 726f 6b65 206d 6172 6b65 7273  l stroke markers
-000014f0: 2220 643d 2220 4d20 3833 382e 3632 3734  " d=" M 838.6274
-00001500: 3335 3934 3032 3737 3320 3131 2e37 3836  359402773 11.786
-00001510: 3437 3734 3537 3939 3939 3937 204c 2039  477457999997 L 9
-00001520: 3232 2e34 3237 3837 3730 3132 3932 3538  22.4278770129258
-00001530: 2031 312e 3738 3634 3737 3435 3739 3939   11.786477457999
-00001540: 3939 3720 4c20 3932 322e 3432 3738 3737  997 L 922.427877
-00001550: 3031 3239 3235 3820 3539 2e32 3834 3232  0129258 59.28422
-00001560: 3234 3337 3939 3939 3836 204c 2038 3338  2437999986 L 838
-00001570: 2e36 3237 3433 3539 3430 3237 3733 2035  .6274359402773 5
-00001580: 392e 3238 3432 3232 3433 3739 3939 3938  9.28422243799998
-00001590: 3620 4c20 3833 382e 3632 3734 3335 3934  6 L 838.62743594
-000015a0: 3032 3737 3320 3131 2e37 3836 3437 3734  02773 11.7864774
-000015b0: 3537 3939 3939 3937 205a 2220 7374 726f  57999997 Z" stro
-000015c0: 6b65 2d6d 6974 6572 6c69 6d69 743d 2231  ke-miterlimit="1
-000015d0: 3022 2073 7472 6f6b 652d 7769 6474 683d  0" stroke-width=
-000015e0: 2232 2e38 3134 3638 3131 3834 2220 7374  "2.814681184" st
-000015f0: 726f 6b65 2d64 6173 6861 7272 6179 3d22  roke-dasharray="
-00001600: 222f 3e3c 2f67 3e3c 673e 3c67 2f3e 3c74  "/></g><g><g/><t
-00001610: 6578 7420 6669 6c6c 3d22 626c 6163 6b22  ext fill="black"
-00001620: 2073 7472 6f6b 653d 226e 6f6e 6522 2066   stroke="none" f
-00001630: 6f6e 742d 6661 6d69 6c79 3d22 7361 6e73  ont-family="sans
-00001640: 2d73 6572 6966 2220 666f 6e74 2d73 697a  -serif" font-siz
-00001650: 653d 2231 3170 7422 2066 6f6e 742d 7374  e="11pt" font-st
-00001660: 796c 653d 226e 6f72 6d61 6c22 2066 6f6e  yle="normal" fon
-00001670: 742d 7765 6967 6874 3d22 6e6f 726d 616c  t-weight="normal
-00001680: 2220 7465 7874 2d64 6563 6f72 6174 696f  " text-decoratio
-00001690: 6e3d 226e 6f72 6d61 6c22 2078 3d22 3835  n="normal" x="85
-000016a0: 372e 3731 3434 3932 3731 3932 3737 3422  7.7144927192774"
-000016b0: 2079 3d22 3431 2e36 3932 3436 3530 3337   y="41.692465037
-000016c0: 3939 3939 3935 2220 7465 7874 2d61 6e63  999995" text-anc
-000016d0: 686f 723d 2273 7461 7274 2220 646f 6d69  hor="start" domi
-000016e0: 6e61 6e74 2d62 6173 656c 696e 653d 2261  nant-baseline="a
-000016f0: 6c70 6861 6265 7469 6322 2078 6d6c 3a73  lphabetic" xml:s
-00001700: 7061 6365 3d22 7072 6573 6572 7665 223e  pace="preserve">
-00001710: 5769 6467 6574 3c2f 7465 7874 3e3c 2f67  Widget</text></g
-00001720: 3e3c 7061 7468 2066 696c 6c3d 226e 6f6e  ><path fill="non
-00001730: 6522 2073 7472 6f6b 653d 226e 6f6e 6522  e" stroke="none"
-00001740: 2f3e 3c67 3e3c 7061 7468 2066 696c 6c3d  /><g><path fill=
-00001750: 2277 6869 7465 2220 7374 726f 6b65 3d22  "white" stroke="
-00001760: 626c 6163 6b22 2070 6169 6e74 2d6f 7264  black" paint-ord
-00001770: 6572 3d22 6669 6c6c 2073 7472 6f6b 6520  er="fill stroke 
-00001780: 6d61 726b 6572 7322 2064 3d22 204d 2039  markers" d=" M 9
-00001790: 3633 2e32 3133 3838 3631 3937 3933 3336  63.2138861979336
-000017a0: 2031 312e 3738 3634 3737 3435 3739 3939   11.786477457999
-000017b0: 3939 3720 4c20 3130 3931 2e30 3330 3035  997 L 1091.03005
-000017c0: 3930 3832 3130 3535 2031 312e 3738 3634  90821055 11.7864
-000017d0: 3737 3435 3739 3939 3939 3720 4c20 3130  77457999997 L 10
-000017e0: 3931 2e30 3330 3035 3930 3832 3130 3535  91.0300590821055
-000017f0: 2035 392e 3238 3432 3232 3433 3739 3939   59.284222437999
-00001800: 3938 3620 4c20 3936 332e 3231 3338 3836  986 L 963.213886
-00001810: 3139 3739 3333 3620 3539 2e32 3834 3232  1979336 59.28422
-00001820: 3234 3337 3939 3939 3836 204c 2039 3633  2437999986 L 963
-00001830: 2e32 3133 3838 3631 3937 3933 3336 2031  .2138861979336 1
-00001840: 312e 3738 3634 3737 3435 3739 3939 3939  1.78647745799999
-00001850: 3720 5a22 2073 7472 6f6b 652d 6d69 7465  7 Z" stroke-mite
-00001860: 726c 696d 6974 3d22 3130 2220 7374 726f  rlimit="10" stro
-00001870: 6b65 2d77 6964 7468 3d22 322e 3831 3436  ke-width="2.8146
-00001880: 3831 3138 3422 2073 7472 6f6b 652d 6461  81184" stroke-da
-00001890: 7368 6172 7261 793d 2222 2f3e 3c2f 673e  sharray=""/></g>
-000018a0: 3c67 3e3c 672f 3e3c 7465 7874 2066 696c  <g><g/><text fil
-000018b0: 6c3d 2262 6c61 636b 2220 7374 726f 6b65  l="black" stroke
-000018c0: 3d22 6e6f 6e65 2220 666f 6e74 2d66 616d  ="none" font-fam
-000018d0: 696c 793d 2273 616e 732d 7365 7269 6622  ily="sans-serif"
-000018e0: 2066 6f6e 742d 7369 7a65 3d22 3131 7074   font-size="11pt
-000018f0: 2220 666f 6e74 2d73 7479 6c65 3d22 6e6f  " font-style="no
-00001900: 726d 616c 2220 666f 6e74 2d77 6569 6768  rmal" font-weigh
-00001910: 743d 226e 6f72 6d61 6c22 2074 6578 742d  t="normal" text-
-00001920: 6465 636f 7261 7469 6f6e 3d22 6e6f 726d  decoration="norm
-00001930: 616c 2220 783d 2239 3832 2e33 3030 3934  al" x="982.30094
-00001940: 3239 3736 3933 3336 2220 793d 2234 312e  29769336" y="41.
-00001950: 3639 3234 3635 3033 3739 3939 3939 3522  692465037999995"
-00001960: 2074 6578 742d 616e 6368 6f72 3d22 7374   text-anchor="st
-00001970: 6172 7422 2064 6f6d 696e 616e 742d 6261  art" dominant-ba
-00001980: 7365 6c69 6e65 3d22 616c 7068 6162 6574  seline="alphabet
-00001990: 6963 2220 786d 6c3a 7370 6163 653d 2270  ic" xml:space="p
-000019a0: 7265 7365 7276 6522 3e74 6162 6c69 622e  reserve">tablib.
-000019b0: 4461 7461 7365 743c 2f74 6578 743e 3c2f  Dataset</text></
-000019c0: 673e 3c2f 673e 3c67 3e3c 7061 7468 2066  g></g><g><path f
-000019d0: 696c 6c3d 2277 6869 7465 2220 7374 726f  ill="white" stro
-000019e0: 6b65 3d22 626c 6163 6b22 2070 6169 6e74  ke="black" paint
-000019f0: 2d6f 7264 6572 3d22 6669 6c6c 2073 7472  -order="fill str
-00001a00: 6f6b 6520 6d61 726b 6572 7322 2064 3d22  oke markers" d="
-00001a10: 204d 2031 3934 2e33 3534 3833 3532 3735   M 194.354835275
-00001a20: 3832 3033 2031 3430 2e32 3036 3330 3634  8203 140.2063064
-00001a30: 3738 204c 2032 3131 2e39 3436 3539 3236  78 L 211.9465926
-00001a40: 3735 3832 3033 2031 3430 2e32 3036 3330  758203 140.20630
-00001a50: 3634 3738 204c 2032 3131 2e39 3436 3539  6478 L 211.94659
-00001a60: 3236 3735 3832 3033 2031 3535 322e 3832  26758203 1552.82
-00001a70: 3434 3235 3639 3739 3939 3720 4c20 3139  44256979997 L 19
-00001a80: 342e 3335 3438 3335 3237 3538 3230 3320  4.3548352758203 
-00001a90: 3135 3532 2e38 3234 3432 3536 3937 3939  1552.82442569799
-00001aa0: 3937 204c 2031 3934 2e33 3534 3833 3532  97 L 194.3548352
-00001ab0: 3735 3832 3033 2031 3430 2e32 3036 3330  758203 140.20630
-00001ac0: 3634 3738 2220 7374 726f 6b65 2d6d 6974  6478" stroke-mit
-00001ad0: 6572 6c69 6d69 743d 2231 3022 2073 7472  erlimit="10" str
-00001ae0: 6f6b 652d 7769 6474 683d 2231 2e34 3635  oke-width="1.465
-00001af0: 3937 3937 3833 3333 3333 3333 3222 2073  9797833333332" s
-00001b00: 7472 6f6b 652d 6461 7368 6172 7261 793d  troke-dasharray=
-00001b10: 2222 2f3e 3c70 6174 6820 6669 6c6c 3d22  ""/><path fill="
-00001b20: 6c69 6768 7462 6c75 6522 2073 7472 6f6b  lightblue" strok
-00001b30: 653d 2262 6c61 636b 2220 7061 696e 742d  e="black" paint-
-00001b40: 6f72 6465 723d 2266 696c 6c20 7374 726f  order="fill stro
-00001b50: 6b65 206d 6172 6b65 7273 2220 643d 2220  ke markers" d=" 
-00001b60: 4d20 3230 332e 3135 3037 3133 3937 3538  M 203.1507139758
-00001b70: 3230 3320 3336 382e 3839 3931 3532 3637  203 368.89915267
-00001b80: 3820 4c20 3232 302e 3734 3234 3731 3337  8 L 220.74247137
-00001b90: 3538 3230 3332 2033 3638 2e38 3939 3135  582032 368.89915
-00001ba0: 3236 3738 204c 2032 3230 2e37 3432 3437  2678 L 220.74247
-00001bb0: 3133 3735 3832 3033 3220 3431 382e 3135  137582032 418.15
-00001bc0: 3630 3733 3339 3830 3030 3035 204c 2032  607339800005 L 2
-00001bd0: 3033 2e31 3530 3731 3339 3735 3832 3033  03.1507139758203
-00001be0: 2034 3138 2e31 3536 3037 3333 3938 3030   418.15607339800
-00001bf0: 3030 3520 4c20 3230 332e 3135 3037 3133  005 L 203.150713
-00001c00: 3937 3538 3230 3320 3336 382e 3839 3931  9758203 368.8991
-00001c10: 3532 3637 3822 2073 7472 6f6b 652d 6d69  52678" stroke-mi
-00001c20: 7465 726c 696d 6974 3d22 3130 2220 7374  terlimit="10" st
-00001c30: 726f 6b65 2d77 6964 7468 3d22 312e 3436  roke-width="1.46
-00001c40: 3539 3739 3738 3333 3333 3333 3332 2220  59797833333332" 
-00001c50: 7374 726f 6b65 2d64 6173 6861 7272 6179  stroke-dasharray
-00001c60: 3d22 222f 3e3c 7061 7468 2066 696c 6c3d  =""/><path fill=
-00001c70: 226c 6967 6874 626c 7565 2220 7374 726f  "lightblue" stro
-00001c80: 6b65 3d22 626c 6163 6b22 2070 6169 6e74  ke="black" paint
-00001c90: 2d6f 7264 6572 3d22 6669 6c6c 2073 7472  -order="fill str
-00001ca0: 6f6b 6520 6d61 726b 6572 7322 2064 3d22  oke markers" d="
-00001cb0: 204d 2032 3033 2e31 3530 3731 3339 3735   M 203.150713975
-00001cc0: 3832 3033 2035 3133 2e31 3531 3536 3333  8203 513.1515633
-00001cd0: 3538 204c 2032 3230 2e37 3432 3437 3133  58 L 220.7424713
-00001ce0: 3735 3832 3033 3220 3531 332e 3135 3135  7582032 513.1515
-00001cf0: 3633 3335 3820 4c20 3232 302e 3734 3234  63358 L 220.7424
-00001d00: 3731 3337 3538 3230 3332 2035 3632 2e34  7137582032 562.4
-00001d10: 3038 3438 3430 3737 3939 3939 204c 2032  084840779999 L 2
-00001d20: 3033 2e31 3530 3731 3339 3735 3832 3033  03.1507139758203
-00001d30: 2035 3632 2e34 3038 3438 3430 3737 3939   562.40848407799
-00001d40: 3939 204c 2032 3033 2e31 3530 3731 3339  99 L 203.1507139
-00001d50: 3735 3832 3033 2035 3133 2e31 3531 3536  758203 513.15156
-00001d60: 3333 3538 2220 7374 726f 6b65 2d6d 6974  3358" stroke-mit
-00001d70: 6572 6c69 6d69 743d 2231 3022 2073 7472  erlimit="10" str
-00001d80: 6f6b 652d 7769 6474 683d 2231 2e34 3635  oke-width="1.465
-00001d90: 3937 3937 3833 3333 3333 3333 3222 2073  9797833333332" s
-00001da0: 7472 6f6b 652d 6461 7368 6172 7261 793d  troke-dasharray=
-00001db0: 2222 2f3e 3c70 6174 6820 6669 6c6c 3d22  ""/><path fill="
-00001dc0: 6c69 6768 7462 6c75 6522 2073 7472 6f6b  lightblue" strok
-00001dd0: 653d 2262 6c61 636b 2220 7061 696e 742d  e="black" paint-
-00001de0: 6f72 6465 723d 2266 696c 6c20 7374 726f  order="fill stro
-00001df0: 6b65 206d 6172 6b65 7273 2220 643d 2220  ke markers" d=" 
-00001e00: 4d20 3230 332e 3135 3037 3133 3937 3538  M 203.1507139758
-00001e10: 3230 3320 3730 342e 3930 3137 3139 3031  203 704.90171901
-00001e20: 3739 3939 3920 4c20 3232 302e 3734 3234  79999 L 220.7424
-00001e30: 3731 3337 3538 3230 3332 2037 3034 2e39  7137582032 704.9
-00001e40: 3031 3731 3930 3137 3939 3939 204c 2032  017190179999 L 2
-00001e50: 3230 2e37 3432 3437 3133 3735 3832 3033  20.7424713758203
-00001e60: 3220 3134 3237 2e39 3232 3934 3831 3537  2 1427.922948157
-00001e70: 3939 3936 204c 2032 3033 2e31 3530 3731  9996 L 203.15071
-00001e80: 3339 3735 3832 3033 2031 3432 372e 3932  39758203 1427.92
-00001e90: 3239 3438 3135 3739 3939 3620 4c20 3230  29481579996 L 20
-00001ea0: 332e 3135 3037 3133 3937 3538 3230 3320  3.1507139758203 
-00001eb0: 3730 342e 3930 3137 3139 3031 3739 3939  704.901719017999
-00001ec0: 3922 2073 7472 6f6b 652d 6d69 7465 726c  9" stroke-miterl
-00001ed0: 696d 6974 3d22 3130 2220 7374 726f 6b65  imit="10" stroke
-00001ee0: 2d77 6964 7468 3d22 312e 3436 3539 3739  -width="1.465979
-00001ef0: 3738 3333 3333 3333 3332 2220 7374 726f  7833333332" stro
-00001f00: 6b65 2d64 6173 6861 7272 6179 3d22 222f  ke-dasharray=""/
-00001f10: 3e3c 7061 7468 2066 696c 6c3d 226c 6967  ><path fill="lig
-00001f20: 6874 7069 6e6b 2220 7374 726f 6b65 3d22  htpink" stroke="
-00001f30: 626c 6163 6b22 2070 6169 6e74 2d6f 7264  black" paint-ord
-00001f40: 6572 3d22 6669 6c6c 2073 7472 6f6b 6520  er="fill stroke 
-00001f50: 6d61 726b 6572 7322 2064 3d22 204d 2032  markers" d=" M 2
-00001f60: 3131 2e39 3436 3539 3236 3735 3832 3033  11.9465926758203
-00001f70: 2038 3234 2e35 3235 3636 3933 3337 3939   824.52566933799
-00001f80: 3938 204c 2032 3239 2e35 3338 3335 3030  98 L 229.5383500
-00001f90: 3735 3832 3033 3220 3832 342e 3532 3536  7582032 824.5256
-00001fa0: 3639 3333 3739 3939 3820 4c20 3232 392e  693379998 L 229.
-00001fb0: 3533 3833 3530 3037 3538 3230 3332 2031  53835007582032 1
-00001fc0: 3430 312e 3533 3533 3132 3035 3739 3939  401.535312057999
-00001fd0: 3620 4c20 3231 312e 3934 3635 3932 3637  6 L 211.94659267
-00001fe0: 3538 3230 3320 3134 3031 2e35 3335 3331  58203 1401.53531
-00001ff0: 3230 3537 3939 3936 204c 2032 3131 2e39  20579996 L 211.9
-00002000: 3436 3539 3236 3735 3832 3033 2038 3234  465926758203 824
-00002010: 2e35 3235 3636 3933 3337 3939 3938 2220  .5256693379998" 
-00002020: 7374 726f 6b65 2d6d 6974 6572 6c69 6d69  stroke-miterlimi
-00002030: 743d 2231 3022 2073 7472 6f6b 652d 7769  t="10" stroke-wi
-00002040: 6474 683d 2231 2e34 3635 3937 3937 3833  dth="1.465979783
-00002050: 3333 3333 3333 3222 2073 7472 6f6b 652d  3333332" stroke-
-00002060: 6461 7368 6172 7261 793d 2222 2f3e 3c70  dasharray=""/><p
-00002070: 6174 6820 6669 6c6c 3d22 6c69 6768 7462  ath fill="lightb
-00002080: 6c75 6522 2073 7472 6f6b 653d 2262 6c61  lue" stroke="bla
-00002090: 636b 2220 7061 696e 742d 6f72 6465 723d  ck" paint-order=
-000020a0: 2266 696c 6c20 7374 726f 6b65 206d 6172  "fill stroke mar
-000020b0: 6b65 7273 2220 643d 2220 4d20 3539 362e  kers" d=" M 596.
-000020c0: 3039 3230 3239 3333 3235 3931 3220 3837  0920293325912 87
-000020d0: 332e 3738 3235 3930 3035 3739 3939 3920  3.7825900579999 
-000020e0: 4c20 3631 332e 3638 3337 3836 3733 3235  L 613.6837867325
-000020f0: 3931 3220 3837 332e 3738 3235 3930 3035  912 873.78259005
-00002100: 3739 3939 3920 4c20 3631 332e 3638 3337  79999 L 613.6837
-00002110: 3836 3733 3235 3931 3220 3134 3031 2e35  867325912 1401.5
-00002120: 3335 3331 3230 3537 3939 3936 204c 2035  353120579996 L 5
-00002130: 3936 2e30 3932 3032 3933 3332 3539 3132  96.0920293325912
-00002140: 2031 3430 312e 3533 3533 3132 3035 3739   1401.5353120579
-00002150: 3939 3620 4c20 3539 362e 3039 3230 3239  996 L 596.092029
-00002160: 3333 3235 3931 3220 3837 332e 3738 3235  3325912 873.7825
-00002170: 3930 3035 3739 3939 3922 2073 7472 6f6b  900579999" strok
-00002180: 652d 6d69 7465 726c 696d 6974 3d22 3130  e-miterlimit="10
-00002190: 2220 7374 726f 6b65 2d77 6964 7468 3d22  " stroke-width="
-000021a0: 312e 3436 3539 3739 3738 3333 3333 3333  1.46597978333333
-000021b0: 3332 2220 7374 726f 6b65 2d64 6173 6861  32" stroke-dasha
-000021c0: 7272 6179 3d22 222f 3e3c 7061 7468 2066  rray=""/><path f
-000021d0: 696c 6c3d 226c 6967 6874 7069 6e6b 2220  ill="lightpink" 
-000021e0: 7374 726f 6b65 3d22 626c 6163 6b22 2070  stroke="black" p
-000021f0: 6169 6e74 2d6f 7264 6572 3d22 6669 6c6c  aint-order="fill
-00002200: 2073 7472 6f6b 6520 6d61 726b 6572 7322   stroke markers"
-00002210: 2064 3d22 204d 2036 3034 2e38 3837 3930   d=" M 604.88790
-00002220: 3830 3332 3539 3132 2031 3033 302e 3334  80325912 1030.34
-00002230: 3932 3330 3931 3739 3939 3920 4c20 3632  92309179999 L 62
-00002240: 322e 3437 3936 3635 3433 3235 3931 3220  2.4796654325912 
-00002250: 3130 3330 2e33 3439 3233 3039 3137 3939  1030.34923091799
-00002260: 3939 204c 2036 3232 2e34 3739 3636 3534  99 L 622.4796654
-00002270: 3332 3539 3132 2031 3335 322e 3237 3833  325912 1352.2783
-00002280: 3931 3333 3739 3939 3720 4c20 3630 342e  913379997 L 604.
-00002290: 3838 3739 3038 3033 3235 3931 3220 3133  8879080325912 13
-000022a0: 3532 2e32 3738 3339 3133 3337 3939 3937  52.2783913379997
-000022b0: 204c 2036 3034 2e38 3837 3930 3830 3332   L 604.887908032
-000022c0: 3539 3132 2031 3033 302e 3334 3932 3330  5912 1030.349230
-000022d0: 3931 3739 3939 3922 2073 7472 6f6b 652d  9179999" stroke-
-000022e0: 6d69 7465 726c 696d 6974 3d22 3130 2220  miterlimit="10" 
-000022f0: 7374 726f 6b65 2d77 6964 7468 3d22 312e  stroke-width="1.
-00002300: 3436 3539 3739 3738 3333 3333 3333 3332  4659797833333332
-00002310: 2220 7374 726f 6b65 2d64 6173 6861 7272  " stroke-dasharr
-00002320: 6179 3d22 222f 3e3c 7061 7468 2066 696c  ay=""/><path fil
-00002330: 6c3d 2277 6869 7465 2220 7374 726f 6b65  l="white" stroke
-00002340: 3d22 626c 6163 6b22 2070 6169 6e74 2d6f  ="black" paint-o
-00002350: 7264 6572 3d22 6669 6c6c 2073 7472 6f6b  rder="fill strok
-00002360: 6520 6d61 726b 6572 7322 2064 3d22 204d  e markers" d=" M
-00002370: 2038 3731 2e37 3331 3737 3737 3736 3630   871.73177777660
-00002380: 3136 2031 3231 382e 3538 3130 3335 3039  16 1218.58103509
-00002390: 3739 3939 3820 4c20 3838 392e 3332 3335  79998 L 889.3235
-000023a0: 3335 3137 3636 3031 3620 3132 3138 2e35  351766016 1218.5
-000023b0: 3831 3033 3530 3937 3939 3938 204c 2038  810350979998 L 8
-000023c0: 3839 2e33 3233 3533 3531 3736 3630 3136  89.3235351766016
-000023d0: 2031 3335 322e 3237 3833 3931 3333 3739   1352.2783913379
-000023e0: 3939 3720 4c20 3837 312e 3733 3137 3737  997 L 871.731777
-000023f0: 3737 3636 3031 3620 3133 3532 2e32 3738  7766016 1352.278
-00002400: 3339 3133 3337 3939 3937 204c 2038 3731  3913379997 L 871
-00002410: 2e37 3331 3737 3737 3736 3630 3136 2031  .7317777766016 1
-00002420: 3231 382e 3538 3130 3335 3039 3739 3939  218.581035097999
-00002430: 3822 2073 7472 6f6b 652d 6d69 7465 726c  8" stroke-miterl
-00002440: 696d 6974 3d22 3130 2220 7374 726f 6b65  imit="10" stroke
-00002450: 2d77 6964 7468 3d22 312e 3436 3539 3739  -width="1.465979
-00002460: 3738 3333 3333 3333 3332 2220 7374 726f  7833333332" stro
-00002470: 6b65 2d64 6173 6861 7272 6179 3d22 222f  ke-dasharray=""/
-00002480: 3e3c 673e 3c67 3e3c 7265 6374 2066 696c  ><g><g><rect fil
-00002490: 6c3d 2277 6869 7465 2220 7374 726f 6b65  l="white" stroke
-000024a0: 3d22 6e6f 6e65 2220 783d 2232 3332 2e37  ="none" x="232.7
-000024b0: 3633 3530 3535 3939 3135 3336 3322 2079  6350559915363" y
-000024c0: 3d22 3934 2e34 3637 3733 3732 3337 3939  ="94.46773723799
-000024d0: 3939 3822 2077 6964 7468 3d22 3237 372e  998" width="277.
-000024e0: 3939 3736 3831 3032 3835 3933 3822 2068  9976810285938" h
-000024f0: 6569 6768 743d 2232 322e 3836 3932 3834  eight="22.869284
-00002500: 3632 222f 3e3c 2f67 3e3c 7465 7874 2066  62"/></g><text f
-00002510: 696c 6c3d 2262 6c61 636b 2220 7374 726f  ill="black" stro
-00002520: 6b65 3d22 6e6f 6e65 2220 666f 6e74 2d66  ke="none" font-f
-00002530: 616d 696c 793d 226d 6f6e 6f73 7061 6365  amily="monospace
-00002540: 2220 666f 6e74 2d73 697a 653d 2231 3170  " font-size="11p
-00002550: 7422 2066 6f6e 742d 7374 796c 653d 226e  t" font-style="n
-00002560: 6f72 6d61 6c22 2066 6f6e 742d 7765 6967  ormal" font-weig
-00002570: 6874 3d22 6e6f 726d 616c 2220 7465 7874  ht="normal" text
-00002580: 2d64 6563 6f72 6174 696f 6e3d 226e 6f72  -decoration="nor
-00002590: 6d61 6c22 2078 3d22 3233 352e 3430 3232  mal" x="235.4022
-000025a0: 3639 3230 3931 3533 3634 2220 793d 2231  6920915364" y="1
-000025b0: 3130 2e33 3030 3331 3838 3937 3939 3939  10.3003188979999
-000025c0: 3722 2074 6578 742d 616e 6368 6f72 3d22  7" text-anchor="
-000025d0: 7374 6172 7422 2064 6f6d 696e 616e 742d  start" dominant-
-000025e0: 6261 7365 6c69 6e65 3d22 616c 7068 6162  baseline="alphab
-000025f0: 6574 6963 2220 786d 6c3a 7370 6163 653d  etic" xml:space=
-00002600: 2270 7265 7365 7276 6522 3e65 7870 6f72  "preserve">expor
-00002610: 7428 7175 6572 7973 6574 3d4e 6f6e 652c  t(queryset=None,
-00002620: c2a0 2a2a 6b77 6172 6773 293c 2f74 6578  ..**kwargs)</tex
-00002630: 743e 3c2f 673e 3c67 3e3c 7061 7468 2066  t></g><g><path f
-00002640: 696c 6c3d 226e 6f6e 6522 2073 7472 6f6b  ill="none" strok
-00002650: 653d 2262 6c61 636b 2220 7061 696e 742d  e="black" paint-
-00002660: 6f72 6465 723d 2266 696c 6c20 7374 726f  order="fill stro
-00002670: 6b65 206d 6172 6b65 7273 2220 643d 2220  ke markers" d=" 
-00002680: 4d20 3230 332e 3135 3037 3133 3937 3538  M 203.1507139758
-00002690: 3230 3320 3131 372e 3333 3730 3231 3835  203 117.33702185
-000026a0: 3739 3939 3939 204c 2032 3832 2e33 3133  799999 L 282.313
-000026b0: 3632 3232 3735 3832 3033 2031 3137 2e33  6222758203 117.3
-000026c0: 3337 3032 3138 3537 3939 3939 3920 4c20  3702185799999 L 
-000026d0: 3238 322e 3331 3336 3232 3237 3538 3230  282.313622275820
-000026e0: 3320 3134 302e 3230 3633 3036 3437 3820  3 140.206306478 
-000026f0: 4c20 3232 362e 3433 3034 3732 3933 3531  L 226.4304729351
-00002700: 3533 3636 2031 3430 2e32 3036 3330 3634  5366 140.2063064
-00002710: 3738 2220 7374 726f 6b65 2d6d 6974 6572  78" stroke-miter
-00002720: 6c69 6d69 743d 2231 3022 2073 7472 6f6b  limit="10" strok
-00002730: 652d 7769 6474 683d 2231 2e34 3635 3937  e-width="1.46597
-00002740: 3937 3833 3333 3333 3333 3222 2073 7472  97833333332" str
-00002750: 6f6b 652d 6461 7368 6172 7261 793d 2222  oke-dasharray=""
-00002760: 2f3e 3c67 2074 7261 6e73 666f 726d 3d22  /><g transform="
-00002770: 7472 616e 736c 6174 6528 3231 312e 3934  translate(211.94
-00002780: 3635 3932 3637 3538 3230 332c 3134 302e  65926758203,140.
-00002790: 3230 3633 3036 3437 3829 2074 7261 6e73  206306478) trans
-000027a0: 6c61 7465 282d 3231 312e 3934 3635 3932  late(-211.946592
-000027b0: 3637 3538 3230 332c 2d31 3430 2e32 3036  6758203,-140.206
-000027c0: 3330 3634 3738 2922 3e3c 7061 7468 2066  306478)"><path f
-000027d0: 696c 6c3d 2262 6c61 636b 2220 7374 726f  ill="black" stro
-000027e0: 6b65 3d22 6e6f 6e65 2220 7061 696e 742d  ke="none" paint-
-000027f0: 6f72 6465 723d 2273 7472 6f6b 6520 6669  order="stroke fi
-00002800: 6c6c 206d 6172 6b65 7273 2220 643d 2220  ll markers" d=" 
-00002810: 4d20 3232 362e 3630 3633 3930 3530 3931  M 226.6063905091
-00002820: 3533 3634 2031 3332 2e38 3736 3430 3735  5364 132.8764075
-00002830: 3631 3333 3333 204c 2032 3131 2e39 3436  613333 L 211.946
-00002840: 3539 3236 3735 3832 3033 2031 3430 2e32  5926758203 140.2
-00002850: 3036 3330 3634 3738 204c 2032 3236 2e36  06306478 L 226.6
-00002860: 3036 3339 3035 3039 3135 3336 3420 3134  0639050915364 14
-00002870: 372e 3533 3632 3035 3339 3436 3636 3637  7.53620539466667
-00002880: 205a 222f 3e3c 2f67 3e3c 2f67 3e3c 673e   Z"/></g></g><g>
-00002890: 3c67 3e3c 7265 6374 2066 696c 6c3d 2277  <g><rect fill="w
-000028a0: 6869 7465 2220 7374 726f 6b65 3d22 6e6f  hite" stroke="no
-000028b0: 6e65 2220 783d 2232 3332 2e37 3633 3530  ne" x="232.76350
-000028c0: 3535 3939 3135 3336 3322 2079 3d22 3136  559915363" y="16
-000028d0: 362e 3539 3339 3432 3537 3822 2077 6964  6.593942578" wid
-000028e0: 7468 3d22 3333 392e 3537 3936 3531 3234  th="339.57965124
-000028f0: 3334 3337 3522 2068 6569 6768 743d 2232  34375" height="2
-00002900: 322e 3836 3932 3834 3632 222f 3e3c 2f67  2.86928462"/></g
-00002910: 3e3c 673e 3c72 6563 7420 6669 6c6c 3d22  ><g><rect fill="
-00002920: 7965 6c6c 6f77 2220 7374 726f 6b65 3d22  yellow" stroke="
-00002930: 6e6f 6e65 2220 783d 2232 3335 2e34 3032  none" x="235.402
-00002940: 3236 3932 3039 3135 3336 3422 2079 3d22  26920915364" y="
-00002950: 3136 392e 3430 3836 3233 3736 3230 3030  169.408623762000
-00002960: 3032 2220 7769 6474 683d 2233 3334 2e33  02" width="334.3
-00002970: 3032 3132 3430 3233 3433 3735 2220 6865  021240234375" he
-00002980: 6967 6874 3d22 3137 2e37 3637 3637 3439  ight="17.7676749
-00002990: 3734 222f 3e3c 7465 7874 2066 696c 6c3d  74"/><text fill=
-000029a0: 2262 6c61 636b 2220 7374 726f 6b65 3d22  "black" stroke="
-000029b0: 6e6f 6e65 2220 666f 6e74 2d66 616d 696c  none" font-famil
-000029c0: 793d 226d 6f6e 6f73 7061 6365 2220 666f  y="monospace" fo
-000029d0: 6e74 2d73 697a 653d 2231 3170 7422 2066  nt-size="11pt" f
-000029e0: 6f6e 742d 7374 796c 653d 226e 6f72 6d61  ont-style="norma
-000029f0: 6c22 2066 6f6e 742d 7765 6967 6874 3d22  l" font-weight="
-00002a00: 6e6f 726d 616c 2220 7465 7874 2d64 6563  normal" text-dec
-00002a10: 6f72 6174 696f 6e3d 226e 6f72 6d61 6c22  oration="normal"
-00002a20: 2078 3d22 3233 352e 3430 3232 3639 3230   x="235.40226920
-00002a30: 3931 3533 3634 2220 793d 2231 3832 2e34  915364" y="182.4
-00002a40: 3236 3532 3432 3338 2220 7465 7874 2d61  26524238" text-a
-00002a50: 6e63 686f 723d 2273 7461 7274 2220 646f  nchor="start" do
-00002a60: 6d69 6e61 6e74 2d62 6173 656c 696e 653d  minant-baseline=
-00002a70: 2261 6c70 6861 6265 7469 6322 2078 6d6c  "alphabetic" xml
-00002a80: 3a73 7061 6365 3d22 7072 6573 6572 7665  :space="preserve
-00002a90: 223e 6265 666f 7265 5f65 7870 6f72 7428  ">before_export(
-00002aa0: 7175 6572 7973 6574 3d4e 6f6e 652c c2a0  queryset=None,..
-00002ab0: 2a2a 6b77 6172 6773 293c 2f74 6578 743e  **kwargs)</text>
-00002ac0: 3c2f 673e 3c67 3e3c 7061 7468 2066 696c  </g><g><path fil
-00002ad0: 6c3d 226e 6f6e 6522 2073 7472 6f6b 653d  l="none" stroke=
-00002ae0: 2262 6c61 636b 2220 7061 696e 742d 6f72  "black" paint-or
-00002af0: 6465 723d 2266 696c 6c20 7374 726f 6b65  der="fill stroke
-00002b00: 206d 6172 6b65 7273 2220 643d 2220 4d20   markers" d=" M 
-00002b10: 3231 312e 3934 3635 3932 3637 3538 3230  211.946592675820
-00002b20: 3320 3138 392e 3436 3332 3237 3139 3820  3 189.463227198 
-00002b30: 4c20 3238 322e 3331 3336 3232 3237 3538  L 282.3136222758
-00002b40: 3230 3320 3138 392e 3436 3332 3237 3139  203 189.46322719
-00002b50: 3820 4c20 3238 322e 3331 3336 3232 3237  8 L 282.31362227
-00002b60: 3538 3230 3320 3231 322e 3333 3235 3131  58203 212.332511
-00002b70: 3831 3820 4c20 3232 362e 3433 3034 3732  818 L 226.430472
-00002b80: 3933 3531 3533 3636 2032 3132 2e33 3332  93515366 212.332
-00002b90: 3531 3138 3138 2220 7374 726f 6b65 2d6d  511818" stroke-m
-00002ba0: 6974 6572 6c69 6d69 743d 2231 3022 2073  iterlimit="10" s
-00002bb0: 7472 6f6b 652d 7769 6474 683d 2231 2e34  troke-width="1.4
-00002bc0: 3635 3937 3937 3833 3333 3333 3333 3222  659797833333332"
-00002bd0: 2073 7472 6f6b 652d 6461 7368 6172 7261   stroke-dasharra
-00002be0: 793d 2222 2f3e 3c67 2074 7261 6e73 666f  y=""/><g transfo
-00002bf0: 726d 3d22 7472 616e 736c 6174 6528 3231  rm="translate(21
-00002c00: 312e 3934 3635 3932 3637 3538 3230 332c  1.9465926758203,
-00002c10: 3231 322e 3333 3235 3131 3831 3829 2074  212.332511818) t
-00002c20: 7261 6e73 6c61 7465 282d 3231 312e 3934  ranslate(-211.94
-00002c30: 3635 3932 3637 3538 3230 332c 2d32 3132  65926758203,-212
-00002c40: 2e33 3332 3531 3138 3138 2922 3e3c 7061  .332511818)"><pa
-00002c50: 7468 2066 696c 6c3d 2262 6c61 636b 2220  th fill="black" 
-00002c60: 7374 726f 6b65 3d22 6e6f 6e65 2220 7061  stroke="none" pa
-00002c70: 696e 742d 6f72 6465 723d 2273 7472 6f6b  int-order="strok
-00002c80: 6520 6669 6c6c 206d 6172 6b65 7273 2220  e fill markers" 
-00002c90: 643d 2220 4d20 3232 362e 3630 3633 3930  d=" M 226.606390
-00002ca0: 3530 3931 3533 3634 2032 3035 2e30 3032  50915364 205.002
-00002cb0: 3631 3239 3031 3333 3333 3220 4c20 3231  61290133332 L 21
-00002cc0: 312e 3934 3635 3932 3637 3538 3230 3320  1.9465926758203 
-00002cd0: 3231 322e 3333 3235 3131 3831 3820 4c20  212.332511818 L 
-00002ce0: 3232 362e 3630 3633 3930 3530 3931 3533  226.606390509153
-00002cf0: 3634 2032 3139 2e36 3632 3431 3037 3334  64 219.662410734
-00002d00: 3636 3636 3820 5a22 2f3e 3c2f 673e 3c2f  66668 Z"/></g></
-00002d10: 673e 3c70 6174 6820 6669 6c6c 3d22 7768  g><path fill="wh
-00002d20: 6974 6522 2073 7472 6f6b 653d 2262 6c61  ite" stroke="bla
-00002d30: 636b 2220 7061 696e 742d 6f72 6465 723d  ck" paint-order=
-00002d40: 2266 696c 6c20 7374 726f 6b65 206d 6172  "fill stroke mar
-00002d50: 6b65 7273 2220 643d 2220 4d20 3137 2e35  kers" d=" M 17.5
-00002d60: 3931 3735 3734 3030 3030 3030 3032 2032  91757400000002 2
-00002d70: 3338 2e37 3230 3134 3739 3138 204c 2033  38.720147918 L 3
-00002d80: 3732 2e38 3737 3038 3838 3931 3634 3036  72.8770888916406
-00002d90: 2032 3338 2e37 3230 3134 3739 3138 204c   238.720147918 L
-00002da0: 2033 3838 2e37 3039 3637 3035 3531 3634   388.70967055164
-00002db0: 3036 2032 3534 2e35 3532 3732 3935 3738  06 254.552729578
-00002dc0: 204c 2033 3838 2e37 3039 3637 3035 3531   L 388.709670551
-00002dd0: 3634 3036 2032 3936 2e37 3732 3934 3733  6406 296.7729473
-00002de0: 3338 204c 2031 372e 3539 3137 3537 3430  38 L 17.59175740
-00002df0: 3030 3030 3030 3220 3239 362e 3737 3239  0000002 296.7729
-00002e00: 3437 3333 3820 4c20 3137 2e35 3931 3735  47338 L 17.59175
-00002e10: 3734 3030 3030 3030 3032 2032 3338 2e37  7400000002 238.7
-00002e20: 3230 3134 3739 3138 204d 2033 3732 2e38  20147918 M 372.8
-00002e30: 3737 3038 3838 3931 3634 3036 2032 3338  770888916406 238
-00002e40: 2e37 3230 3134 3739 3138 204c 2033 3732  .720147918 L 372
-00002e50: 2e38 3737 3038 3838 3931 3634 3036 2032  .8770888916406 2
-00002e60: 3534 2e35 3532 3732 3935 3738 204c 2033  54.552729578 L 3
-00002e70: 3838 2e37 3039 3637 3035 3531 3634 3036  88.7096705516406
-00002e80: 2032 3534 2e35 3532 3732 3935 3738 2220   254.552729578" 
-00002e90: 7374 726f 6b65 2d6d 6974 6572 6c69 6d69  stroke-miterlimi
-00002ea0: 743d 2231 3022 2073 7472 6f6b 652d 7769  t="10" stroke-wi
-00002eb0: 6474 683d 2231 2e34 3635 3937 3937 3833  dth="1.465979783
-00002ec0: 3333 3333 3333 3222 2073 7472 6f6b 652d  3333332" stroke-
-00002ed0: 6461 7368 6172 7261 793d 2222 2f3e 3c67  dasharray=""/><g
-00002ee0: 3e3c 7465 7874 2066 696c 6c3d 2262 6c61  ><text fill="bla
-00002ef0: 636b 2220 7374 726f 6b65 3d22 6e6f 6e65  ck" stroke="none
-00002f00: 2220 666f 6e74 2d66 616d 696c 793d 2273  " font-family="s
-00002f10: 616e 732d 7365 7269 6622 2066 6f6e 742d  ans-serif" font-
-00002f20: 7369 7a65 3d22 3131 7074 2220 666f 6e74  size="11pt" font
-00002f30: 2d73 7479 6c65 3d22 6e6f 726d 616c 2220  -style="normal" 
-00002f40: 666f 6e74 2d77 6569 6768 743d 226e 6f72  font-weight="nor
-00002f50: 6d61 6c22 2074 6578 742d 6465 636f 7261  mal" text-decora
-00002f60: 7469 6f6e 3d22 6e6f 726d 616c 2220 783d  tion="normal" x=
-00002f70: 2234 322e 3232 3032 3137 3736 2220 793d  "42.22021776" y=
-00002f80: 2232 3633 2e33 3438 3630 3832 3738 2220  "263.348608278" 
-00002f90: 7465 7874 2d61 6e63 686f 723d 2273 7461  text-anchor="sta
-00002fa0: 7274 2220 646f 6d69 6e61 6e74 2d62 6173  rt" dominant-bas
-00002fb0: 656c 696e 653d 2261 6c70 6861 6265 7469  eline="alphabeti
-00002fc0: 6322 2078 6d6c 3a73 7061 6365 3d22 7072  c" xml:space="pr
-00002fd0: 6573 6572 7665 223e 41c2 a051 7565 7279  eserve">A..Query
-00002fe0: 7365 74c2 a069 6e73 7461 6e63 65c2 a063  set..instance..c
-00002ff0: 616e c2a0 6265 c2a0 7061 7373 6564 c2a0  an..be..passed..
-00003000: 696e 746f c2a0 6578 706f 7274 2829 2e3c  into..export().<
-00003010: 2f74 6578 743e 3c74 6578 7420 6669 6c6c  /text><text fill
-00003020: 3d22 626c 6163 6b22 2073 7472 6f6b 653d  ="black" stroke=
-00003030: 226e 6f6e 6522 2066 6f6e 742d 6661 6d69  "none" font-fami
-00003040: 6c79 3d22 7361 6e73 2d73 6572 6966 2220  ly="sans-serif" 
-00003050: 666f 6e74 2d73 697a 653d 2231 3170 7422  font-size="11pt"
-00003060: 2066 6f6e 742d 7374 796c 653d 226e 6f72   font-style="nor
-00003070: 6d61 6c22 2066 6f6e 742d 7765 6967 6874  mal" font-weight
-00003080: 3d22 6e6f 726d 616c 2220 7465 7874 2d64  ="normal" text-d
-00003090: 6563 6f72 6174 696f 6e3d 226e 6f72 6d61  ecoration="norma
-000030a0: 6c22 2078 3d22 3432 2e32 3230 3231 3737  l" x="42.2202177
-000030b0: 3622 2079 3d22 3238 302e 3934 3033 3635  6" y="280.940365
-000030c0: 3637 3822 2074 6578 742d 616e 6368 6f72  678" text-anchor
-000030d0: 3d22 7374 6172 7422 2064 6f6d 696e 616e  ="start" dominan
-000030e0: 742d 6261 7365 6c69 6e65 3d22 616c 7068  t-baseline="alph
-000030f0: 6162 6574 6963 2220 786d 6c3a 7370 6163  abetic" xml:spac
-00003100: 653d 2270 7265 7365 7276 6522 3e49 66c2  e="preserve">If.
-00003110: a06e 6fc2 a051 7565 7279 7365 74c2 a069  .no..Queryset..i
-00003120: 73c2 a070 6173 7365 642c c2a0 6765 745f  s..passed,..get_
-00003130: 7175 6572 7973 6574 2829 c2a0 6973 c2a0  queryset()..is..
-00003140: 6361 6c6c 6564 2e3c 2f74 6578 743e 3c2f  called.</text></
-00003150: 673e 3c67 3e3c 673e 3c72 6563 7420 6669  g><g><g><rect fi
-00003160: 6c6c 3d22 7768 6974 6522 2073 7472 6f6b  ll="white" strok
-00003170: 653d 226e 6f6e 6522 2078 3d22 3234 312e  e="none" x="241.
-00003180: 3535 3933 3834 3239 3931 3533 3633 2220  55938429915363" 
-00003190: 793d 2233 3233 2e31 3630 3538 3334 3338  y="323.160583438
-000031a0: 2220 7769 6474 683d 2231 3238 2e34 3431  " width="128.441
-000031b0: 3436 3736 3439 3638 3735 2220 6865 6967  4676496875" heig
-000031c0: 6874 3d22 3232 2e38 3639 3238 3436 3222  ht="22.86928462"
-000031d0: 2f3e 3c2f 673e 3c67 3e3c 7265 6374 2066  /></g><g><rect f
-000031e0: 696c 6c3d 2279 656c 6c6f 7722 2073 7472  ill="yellow" str
-000031f0: 6f6b 653d 226e 6f6e 6522 2078 3d22 3234  oke="none" x="24
-00003200: 342e 3139 3831 3437 3930 3931 3533 3635  4.19814790915365
-00003210: 2220 793d 2233 3235 2e39 3735 3236 3436  " y="325.9752646
-00003220: 3232 2220 7769 6474 683d 2231 3233 2e31  22" width="123.1
-00003230: 3633 3934 3034 3239 3638 3735 2220 6865  639404296875" he
-00003240: 6967 6874 3d22 3137 2e37 3637 3637 3439  ight="17.7676749
-00003250: 3734 222f 3e3c 7465 7874 2066 696c 6c3d  74"/><text fill=
-00003260: 2262 6c61 636b 2220 7374 726f 6b65 3d22  "black" stroke="
-00003270: 6e6f 6e65 2220 666f 6e74 2d66 616d 696c  none" font-famil
-00003280: 793d 226d 6f6e 6f73 7061 6365 2220 666f  y="monospace" fo
-00003290: 6e74 2d73 697a 653d 2231 3170 7422 2066  nt-size="11pt" f
-000032a0: 6f6e 742d 7374 796c 653d 226e 6f72 6d61  ont-style="norma
-000032b0: 6c22 2066 6f6e 742d 7765 6967 6874 3d22  l" font-weight="
-000032c0: 6e6f 726d 616c 2220 7465 7874 2d64 6563  normal" text-dec
-000032d0: 6f72 6174 696f 6e3d 226e 6f72 6d61 6c22  oration="normal"
-000032e0: 2078 3d22 3234 342e 3139 3831 3437 3930   x="244.19814790
-000032f0: 3931 3533 3635 2220 793d 2233 3338 2e39  915365" y="338.9
-00003300: 3933 3136 3530 3938 2220 7465 7874 2d61  93165098" text-a
-00003310: 6e63 686f 723d 2273 7461 7274 2220 646f  nchor="start" do
-00003320: 6d69 6e61 6e74 2d62 6173 656c 696e 653d  minant-baseline=
-00003330: 2261 6c70 6861 6265 7469 6322 2078 6d6c  "alphabetic" xml
-00003340: 3a73 7061 6365 3d22 7072 6573 6572 7665  :space="preserve
-00003350: 223e 6765 745f 7175 6572 7973 6574 2829  ">get_queryset()
-00003360: 3c2f 7465 7874 3e3c 2f67 3e3c 673e 3c70  </text></g><g><p
-00003370: 6174 6820 6669 6c6c 3d22 6e6f 6e65 2220  ath fill="none" 
-00003380: 7374 726f 6b65 3d22 626c 6163 6b22 2070  stroke="black" p
-00003390: 6169 6e74 2d6f 7264 6572 3d22 6669 6c6c  aint-order="fill
-000033a0: 2073 7472 6f6b 6520 6d61 726b 6572 7322   stroke markers"
-000033b0: 2064 3d22 204d 2032 3131 2e39 3436 3539   d=" M 211.94659
-000033c0: 3236 3735 3832 3033 2033 3436 2e30 3239  26758203 346.029
-000033d0: 3836 3830 3538 3030 3030 3320 4c20 3239  86805800003 L 29
-000033e0: 312e 3130 3935 3030 3937 3538 3230 3320  1.1095009758203 
-000033f0: 3334 362e 3032 3938 3638 3035 3830 3030  346.029868058000
-00003400: 3033 204c 2032 3931 2e31 3039 3530 3039  03 L 291.1095009
-00003410: 3735 3832 3033 2033 3638 2e38 3939 3135  758203 368.89915
-00003420: 3236 3738 204c 2032 3335 2e32 3236 3335  2678 L 235.22635
-00003430: 3136 3335 3135 3336 3620 3336 382e 3839  163515366 368.89
-00003440: 3931 3532 3637 3822 2073 7472 6f6b 652d  9152678" stroke-
-00003450: 6d69 7465 726c 696d 6974 3d22 3130 2220  miterlimit="10" 
-00003460: 7374 726f 6b65 2d77 6964 7468 3d22 312e  stroke-width="1.
-00003470: 3436 3539 3739 3738 3333 3333 3333 3332  4659797833333332
-00003480: 2220 7374 726f 6b65 2d64 6173 6861 7272  " stroke-dasharr
-00003490: 6179 3d22 222f 3e3c 6720 7472 616e 7366  ay=""/><g transf
-000034a0: 6f72 6d3d 2274 7261 6e73 6c61 7465 2832  orm="translate(2
-000034b0: 3230 2e37 3432 3437 3133 3735 3832 3033  20.7424713758203
-000034c0: 322c 3336 382e 3839 3931 3532 3637 3829  2,368.899152678)
-000034d0: 2074 7261 6e73 6c61 7465 282d 3232 302e   translate(-220.
-000034e0: 3734 3234 3731 3337 3538 3230 3332 2c2d  74247137582032,-
-000034f0: 3336 382e 3839 3931 3532 3637 3829 223e  368.899152678)">
-00003500: 3c70 6174 6820 6669 6c6c 3d22 626c 6163  <path fill="blac
-00003510: 6b22 2073 7472 6f6b 653d 226e 6f6e 6522  k" stroke="none"
-00003520: 2070 6169 6e74 2d6f 7264 6572 3d22 7374   paint-order="st
-00003530: 726f 6b65 2066 696c 6c20 6d61 726b 6572  roke fill marker
-00003540: 7322 2064 3d22 204d 2032 3335 2e34 3032  s" d=" M 235.402
-00003550: 3236 3932 3039 3135 3336 3420 3336 312e  26920915364 361.
-00003560: 3536 3932 3533 3736 3133 3333 3336 204c  56925376133336 L
-00003570: 2032 3230 2e37 3432 3437 3133 3735 3832   220.74247137582
-00003580: 3033 3220 3336 382e 3839 3931 3532 3637  032 368.89915267
-00003590: 3820 4c20 3233 352e 3430 3232 3639 3230  8 L 235.40226920
-000035a0: 3931 3533 3634 2033 3736 2e32 3239 3035  915364 376.22905
-000035b0: 3135 3934 3636 3636 3620 5a22 2f3e 3c2f  159466666 Z"/></
-000035c0: 673e 3c2f 673e 3c67 3e3c 673e 3c72 6563  g></g><g><g><rec
-000035d0: 7420 6669 6c6c 3d22 7768 6974 6522 2073  t fill="white" s
-000035e0: 7472 6f6b 653d 226e 6f6e 6522 2078 3d22  troke="none" x="
-000035f0: 3234 312e 3535 3933 3834 3239 3931 3533  241.559384299153
-00003600: 3633 2220 793d 2233 3935 2e32 3836 3738  63" y="395.28678
-00003610: 3837 3738 2220 7769 6474 683d 2237 352e  8778" width="75.
-00003620: 3635 3639 3231 3735 3132 3522 2068 6569  65692175125" hei
-00003630: 6768 743d 2232 322e 3836 3932 3834 3632  ght="22.86928462
-00003640: 222f 3e3c 2f67 3e3c 7465 7874 2066 696c  "/></g><text fil
-00003650: 6c3d 2262 6c61 636b 2220 7374 726f 6b65  l="black" stroke
-00003660: 3d22 6e6f 6e65 2220 666f 6e74 2d66 616d  ="none" font-fam
-00003670: 696c 793d 226d 6f6e 6f73 7061 6365 2220  ily="monospace" 
-00003680: 666f 6e74 2d73 697a 653d 2231 3170 7422  font-size="11pt"
-00003690: 2066 6f6e 742d 7374 796c 653d 226e 6f72   font-style="nor
-000036a0: 6d61 6c22 2066 6f6e 742d 7765 6967 6874  mal" font-weight
-000036b0: 3d22 6e6f 726d 616c 2220 7465 7874 2d64  ="normal" text-d
-000036c0: 6563 6f72 6174 696f 6e3d 226e 6f72 6d61  ecoration="norma
-000036d0: 6c22 2078 3d22 3234 342e 3139 3831 3437  l" x="244.198147
-000036e0: 3930 3931 3533 3635 2220 793d 2234 3131  90915365" y="411
-000036f0: 2e31 3139 3337 3034 3338 3030 3030 3322  .11937043800003"
-00003700: 2074 6578 742d 616e 6368 6f72 3d22 7374   text-anchor="st
-00003710: 6172 7422 2064 6f6d 696e 616e 742d 6261  art" dominant-ba
-00003720: 7365 6c69 6e65 3d22 616c 7068 6162 6574  seline="alphabet
-00003730: 6963 2220 786d 6c3a 7370 6163 653d 2270  ic" xml:space="p
-00003740: 7265 7365 7276 6522 3e51 7565 7279 7365  reserve">Queryse
-00003750: 743c 2f74 6578 743e 3c2f 673e 3c67 3e3c  t</text></g><g><
-00003760: 7061 7468 2066 696c 6c3d 226e 6f6e 6522  path fill="none"
-00003770: 2073 7472 6f6b 653d 2262 6c61 636b 2220   stroke="black" 
-00003780: 7061 696e 742d 6f72 6465 723d 2266 696c  paint-order="fil
-00003790: 6c20 7374 726f 6b65 206d 6172 6b65 7273  l stroke markers
-000037a0: 2220 643d 2220 4d20 3232 302e 3734 3234  " d=" M 220.7424
-000037b0: 3731 3337 3538 3230 3332 2034 3138 2e31  7137582032 418.1
-000037c0: 3536 3037 3333 3938 3030 3030 3520 4c20  5607339800005 L 
-000037d0: 3239 312e 3130 3935 3030 3937 3538 3230  291.109500975820
-000037e0: 3320 3431 382e 3135 3630 3733 3339 3830  3 418.1560733980
-000037f0: 3030 3035 204c 2032 3931 2e31 3039 3530  0005 L 291.10950
-00003800: 3039 3735 3832 3033 2034 3431 2e30 3235  09758203 441.025
-00003810: 3335 3830 3138 204c 2032 3236 2e34 3330  358018 L 226.430
-00003820: 3437 3239 3335 3135 3336 3620 3434 312e  47293515366 441.
-00003830: 3032 3533 3538 3031 3822 2073 7472 6f6b  025358018" strok
-00003840: 652d 6d69 7465 726c 696d 6974 3d22 3130  e-miterlimit="10
-00003850: 2220 7374 726f 6b65 2d77 6964 7468 3d22  " stroke-width="
-00003860: 312e 3436 3539 3739 3738 3333 3333 3333  1.46597978333333
-00003870: 3332 2220 7374 726f 6b65 2d64 6173 6861  32" stroke-dasha
-00003880: 7272 6179 3d22 372e 3033 3637 3032 3935  rray="7.03670295
-00003890: 3939 3939 3939 3935 222f 3e3c 6720 7472  99999995"/><g tr
-000038a0: 616e 7366 6f72 6d3d 2274 7261 6e73 6c61  ansform="transla
-000038b0: 7465 2832 3131 2e39 3436 3539 3236 3735  te(211.946592675
-000038c0: 3832 3033 2c34 3431 2e30 3235 3335 3830  8203,441.0253580
-000038d0: 3138 2920 7472 616e 736c 6174 6528 2d32  18) translate(-2
-000038e0: 3131 2e39 3436 3539 3236 3735 3832 3033  11.9465926758203
-000038f0: 2c2d 3434 312e 3032 3533 3538 3031 3829  ,-441.025358018)
-00003900: 223e 3c70 6174 6820 6669 6c6c 3d22 626c  "><path fill="bl
-00003910: 6163 6b22 2073 7472 6f6b 653d 226e 6f6e  ack" stroke="non
-00003920: 6522 2070 6169 6e74 2d6f 7264 6572 3d22  e" paint-order="
-00003930: 7374 726f 6b65 2066 696c 6c20 6d61 726b  stroke fill mark
-00003940: 6572 7322 2064 3d22 204d 2032 3236 2e36  ers" d=" M 226.6
-00003950: 3036 3339 3035 3039 3135 3336 3420 3433  0639050915364 43
-00003960: 332e 3639 3534 3539 3130 3133 3333 3337  3.69545910133337
-00003970: 204c 2032 3131 2e39 3436 3539 3236 3735   L 211.946592675
-00003980: 3832 3033 2034 3431 2e30 3235 3335 3830  8203 441.0253580
-00003990: 3138 204c 2032 3236 2e36 3036 3339 3035  18 L 226.6063905
-000039a0: 3039 3135 3336 3420 3434 382e 3335 3532  0915364 448.3552
-000039b0: 3536 3933 3436 3636 3637 205a 222f 3e3c  5693466667 Z"/><
-000039c0: 2f67 3e3c 2f67 3e3c 673e 3c67 3e3c 7265  /g></g><g><g><re
-000039d0: 6374 2066 696c 6c3d 2277 6869 7465 2220  ct fill="white" 
-000039e0: 7374 726f 6b65 3d22 6e6f 6e65 2220 783d  stroke="none" x=
-000039f0: 2232 3431 2e35 3539 3338 3432 3939 3135  "241.55938429915
-00003a00: 3336 3322 2079 3d22 3436 372e 3431 3239  363" y="467.4129
-00003a10: 3934 3131 3822 2077 6964 7468 3d22 3239  94118" width="29
-00003a20: 352e 3539 3235 3239 3636 3134 3036 3322  5.5925296614063"
-00003a30: 2068 6569 6768 743d 2232 322e 3836 3932   height="22.8692
-00003a40: 3834 3632 222f 3e3c 2f67 3e3c 673e 3c72  8462"/></g><g><r
-00003a50: 6563 7420 6669 6c6c 3d22 7965 6c6c 6f77  ect fill="yellow
-00003a60: 2220 7374 726f 6b65 3d22 6e6f 6e65 2220  " stroke="none" 
-00003a70: 783d 2232 3434 2e31 3938 3134 3739 3039  x="244.198147909
-00003a80: 3135 3336 3522 2079 3d22 3437 302e 3232  15365" y="470.22
-00003a90: 3736 3735 3330 3139 3939 3937 2220 7769  767530199997" wi
-00003aa0: 6474 683d 2232 3930 2e33 3135 3030 3234  dth="290.3150024
-00003ab0: 3431 3430 3632 3522 2068 6569 6768 743d  4140625" height=
-00003ac0: 2231 372e 3736 3736 3734 3937 3422 2f3e  "17.767674974"/>
-00003ad0: 3c74 6578 7420 6669 6c6c 3d22 626c 6163  <text fill="blac
-00003ae0: 6b22 2073 7472 6f6b 653d 226e 6f6e 6522  k" stroke="none"
-00003af0: 2066 6f6e 742d 6661 6d69 6c79 3d22 6d6f   font-family="mo
-00003b00: 6e6f 7370 6163 6522 2066 6f6e 742d 7369  nospace" font-si
-00003b10: 7a65 3d22 3131 7074 2220 666f 6e74 2d73  ze="11pt" font-s
-00003b20: 7479 6c65 3d22 6e6f 726d 616c 2220 666f  tyle="normal" fo
-00003b30: 6e74 2d77 6569 6768 743d 226e 6f72 6d61  nt-weight="norma
-00003b40: 6c22 2074 6578 742d 6465 636f 7261 7469  l" text-decorati
-00003b50: 6f6e 3d22 6e6f 726d 616c 2220 783d 2232  on="normal" x="2
-00003b60: 3434 2e31 3938 3134 3739 3039 3135 3336  44.1981479091536
-00003b70: 3522 2079 3d22 3438 332e 3234 3535 3735  5" y="483.245575
-00003b80: 3737 3822 2074 6578 742d 616e 6368 6f72  778" text-anchor
-00003b90: 3d22 7374 6172 7422 2064 6f6d 696e 616e  ="start" dominan
-00003ba0: 742d 6261 7365 6c69 6e65 3d22 616c 7068  t-baseline="alph
-00003bb0: 6162 6574 6963 2220 786d 6c3a 7370 6163  abetic" xml:spac
-00003bc0: 653d 2270 7265 7365 7276 6522 3e66 696c  e="preserve">fil
-00003bd0: 7465 725f 6578 706f 7274 2871 7565 7279  ter_export(query
-00003be0: 7365 742c c2a0 2a2a 6b77 6172 6773 293c  set,..**kwargs)<
-00003bf0: 2f74 6578 743e 3c2f 673e 3c67 3e3c 7061  /text></g><g><pa
-00003c00: 7468 2066 696c 6c3d 226e 6f6e 6522 2073  th fill="none" s
-00003c10: 7472 6f6b 653d 2262 6c61 636b 2220 7061  troke="black" pa
-00003c20: 696e 742d 6f72 6465 723d 2266 696c 6c20  int-order="fill 
-00003c30: 7374 726f 6b65 206d 6172 6b65 7273 2220  stroke markers" 
-00003c40: 643d 2220 4d20 3231 312e 3934 3635 3932  d=" M 211.946592
-00003c50: 3637 3538 3230 3320 3439 302e 3238 3232  6758203 490.2822
-00003c60: 3738 3733 3820 4c20 3239 312e 3130 3935  78738 L 291.1095
-00003c70: 3030 3937 3538 3230 3320 3439 302e 3238  009758203 490.28
-00003c80: 3232 3738 3733 3820 4c20 3239 312e 3130  2278738 L 291.10
-00003c90: 3935 3030 3937 3538 3230 3320 3531 332e  95009758203 513.
-00003ca0: 3135 3135 3633 3335 3820 4c20 3233 352e  151563358 L 235.
-00003cb0: 3232 3633 3531 3633 3531 3533 3636 2035  22635163515366 5
-00003cc0: 3133 2e31 3531 3536 3333 3538 2220 7374  13.151563358" st
-00003cd0: 726f 6b65 2d6d 6974 6572 6c69 6d69 743d  roke-miterlimit=
-00003ce0: 2231 3022 2073 7472 6f6b 652d 7769 6474  "10" stroke-widt
-00003cf0: 683d 2231 2e34 3635 3937 3937 3833 3333  h="1.46597978333
-00003d00: 3333 3333 3222 2073 7472 6f6b 652d 6461  33332" stroke-da
-00003d10: 7368 6172 7261 793d 2222 2f3e 3c67 2074  sharray=""/><g t
-00003d20: 7261 6e73 666f 726d 3d22 7472 616e 736c  ransform="transl
-00003d30: 6174 6528 3232 302e 3734 3234 3731 3337  ate(220.74247137
-00003d40: 3538 3230 3332 2c35 3133 2e31 3531 3536  582032,513.15156
-00003d50: 3333 3538 2920 7472 616e 736c 6174 6528  3358) translate(
-00003d60: 2d32 3230 2e37 3432 3437 3133 3735 3832  -220.74247137582
-00003d70: 3033 322c 2d35 3133 2e31 3531 3536 3333  032,-513.1515633
-00003d80: 3538 2922 3e3c 7061 7468 2066 696c 6c3d  58)"><path fill=
-00003d90: 2262 6c61 636b 2220 7374 726f 6b65 3d22  "black" stroke="
-00003da0: 6e6f 6e65 2220 7061 696e 742d 6f72 6465  none" paint-orde
-00003db0: 723d 2273 7472 6f6b 6520 6669 6c6c 206d  r="stroke fill m
-00003dc0: 6172 6b65 7273 2220 643d 2220 4d20 3233  arkers" d=" M 23
-00003dd0: 352e 3430 3232 3639 3230 3931 3533 3634  5.40226920915364
-00003de0: 2035 3035 2e38 3231 3636 3434 3431 3333   505.82166444133
-00003df0: 3333 204c 2032 3230 2e37 3432 3437 3133  33 L 220.7424713
-00003e00: 3735 3832 3033 3220 3531 332e 3135 3135  7582032 513.1515
-00003e10: 3633 3335 3820 4c20 3233 352e 3430 3232  63358 L 235.4022
-00003e20: 3639 3230 3931 3533 3634 2035 3230 2e34  6920915364 520.4
-00003e30: 3831 3436 3232 3734 3636 3637 205a 222f  814622746667 Z"/
-00003e40: 3e3c 2f67 3e3c 2f67 3e3c 673e 3c67 3e3c  ></g></g><g><g><
-00003e50: 7265 6374 2066 696c 6c3d 2277 6869 7465  rect fill="white
-00003e60: 2220 7374 726f 6b65 3d22 6e6f 6e65 2220  " stroke="none" 
-00003e70: 783d 2232 3431 2e35 3539 3338 3432 3939  x="241.559384299
-00003e80: 3135 3336 3322 2079 3d22 3533 392e 3533  15363" y="539.53
-00003e90: 3931 3939 3435 3822 2077 6964 7468 3d22  9199458" width="
-00003ea0: 3735 2e36 3536 3932 3137 3531 3235 2220  75.65692175125" 
-00003eb0: 6865 6967 6874 3d22 3232 2e38 3639 3238  height="22.86928
-00003ec0: 3436 3222 2f3e 3c2f 673e 3c74 6578 7420  462"/></g><text 
-00003ed0: 6669 6c6c 3d22 626c 6163 6b22 2073 7472  fill="black" str
-00003ee0: 6f6b 653d 226e 6f6e 6522 2066 6f6e 742d  oke="none" font-
-00003ef0: 6661 6d69 6c79 3d22 6d6f 6e6f 7370 6163  family="monospac
-00003f00: 6522 2066 6f6e 742d 7369 7a65 3d22 3131  e" font-size="11
-00003f10: 7074 2220 666f 6e74 2d73 7479 6c65 3d22  pt" font-style="
-00003f20: 6e6f 726d 616c 2220 666f 6e74 2d77 6569  normal" font-wei
-00003f30: 6768 743d 226e 6f72 6d61 6c22 2074 6578  ght="normal" tex
-00003f40: 742d 6465 636f 7261 7469 6f6e 3d22 6e6f  t-decoration="no
-00003f50: 726d 616c 2220 783d 2232 3434 2e31 3938  rmal" x="244.198
-00003f60: 3134 3739 3039 3135 3336 3522 2079 3d22  14790915365" y="
-00003f70: 3535 352e 3337 3137 3831 3131 3822 2074  555.371781118" t
-00003f80: 6578 742d 616e 6368 6f72 3d22 7374 6172  ext-anchor="star
-00003f90: 7422 2064 6f6d 696e 616e 742d 6261 7365  t" dominant-base
-00003fa0: 6c69 6e65 3d22 616c 7068 6162 6574 6963  line="alphabetic
-00003fb0: 2220 786d 6c3a 7370 6163 653d 2270 7265  " xml:space="pre
-00003fc0: 7365 7276 6522 3e51 7565 7279 7365 743c  serve">Queryset<
-00003fd0: 2f74 6578 743e 3c2f 673e 3c67 3e3c 7061  /text></g><g><pa
-00003fe0: 7468 2066 696c 6c3d 226e 6f6e 6522 2073  th fill="none" s
-00003ff0: 7472 6f6b 653d 2262 6c61 636b 2220 7061  troke="black" pa
-00004000: 696e 742d 6f72 6465 723d 2266 696c 6c20  int-order="fill 
-00004010: 7374 726f 6b65 206d 6172 6b65 7273 2220  stroke markers" 
-00004020: 643d 2220 4d20 3232 302e 3734 3234 3731  d=" M 220.742471
-00004030: 3337 3538 3230 3332 2035 3632 2e34 3038  37582032 562.408
-00004040: 3438 3430 3737 3939 3939 204c 2032 3931  4840779999 L 291
-00004050: 2e31 3039 3530 3039 3735 3832 3033 2035  .1095009758203 5
-00004060: 3632 2e34 3038 3438 3430 3737 3939 3939  62.4084840779999
-00004070: 204c 2032 3931 2e31 3039 3530 3039 3735   L 291.109500975
-00004080: 3832 3033 2035 3835 2e32 3737 3736 3836  8203 585.2777686
-00004090: 3937 3939 3939 204c 2032 3236 2e34 3330  979999 L 226.430
-000040a0: 3437 3239 3335 3135 3336 3620 3538 352e  47293515366 585.
-000040b0: 3237 3737 3638 3639 3739 3939 3922 2073  2777686979999" s
-000040c0: 7472 6f6b 652d 6d69 7465 726c 696d 6974  troke-miterlimit
-000040d0: 3d22 3130 2220 7374 726f 6b65 2d77 6964  ="10" stroke-wid
-000040e0: 7468 3d22 312e 3436 3539 3739 3738 3333  th="1.4659797833
-000040f0: 3333 3333 3332 2220 7374 726f 6b65 2d64  333332" stroke-d
-00004100: 6173 6861 7272 6179 3d22 372e 3033 3637  asharray="7.0367
-00004110: 3032 3935 3939 3939 3939 3935 222f 3e3c  029599999995"/><
-00004120: 6720 7472 616e 7366 6f72 6d3d 2274 7261  g transform="tra
-00004130: 6e73 6c61 7465 2832 3131 2e39 3436 3539  nslate(211.94659
-00004140: 3236 3735 3832 3033 2c35 3835 2e32 3737  26758203,585.277
-00004150: 3736 3836 3937 3939 3939 2920 7472 616e  7686979999) tran
-00004160: 736c 6174 6528 2d32 3131 2e39 3436 3539  slate(-211.94659
-00004170: 3236 3735 3832 3033 2c2d 3538 352e 3237  26758203,-585.27
-00004180: 3737 3638 3639 3739 3939 3929 223e 3c70  77686979999)"><p
-00004190: 6174 6820 6669 6c6c 3d22 626c 6163 6b22  ath fill="black"
-000041a0: 2073 7472 6f6b 653d 226e 6f6e 6522 2070   stroke="none" p
-000041b0: 6169 6e74 2d6f 7264 6572 3d22 7374 726f  aint-order="stro
-000041c0: 6b65 2066 696c 6c20 6d61 726b 6572 7322  ke fill markers"
-000041d0: 2064 3d22 204d 2032 3236 2e36 3036 3339   d=" M 226.60639
-000041e0: 3035 3039 3135 3336 3420 3537 372e 3934  050915364 577.94
-000041f0: 3738 3639 3738 3133 3333 3220 4c20 3231  78697813332 L 21
-00004200: 312e 3934 3635 3932 3637 3538 3230 3320  1.9465926758203 
-00004210: 3538 352e 3237 3737 3638 3639 3739 3939  585.277768697999
-00004220: 3920 4c20 3232 362e 3630 3633 3930 3530  9 L 226.60639050
-00004230: 3931 3533 3634 2035 3932 2e36 3037 3636  915364 592.60766
-00004240: 3736 3134 3636 3636 205a 222f 3e3c 2f67  76146666 Z"/></g
-00004250: 3e3c 2f67 3e3c 673e 3c67 3e3c 7265 6374  ></g><g><g><rect
-00004260: 2066 696c 6c3d 2272 6762 2832 3535 2c32   fill="rgb(255,2
-00004270: 3432 2c32 3435 2922 2073 7472 6f6b 653d  42,245)" stroke=
-00004280: 226e 6f6e 6522 2078 3d22 3234 312e 3535  "none" x="241.55
-00004290: 3933 3834 3239 3931 3533 3633 2220 793d  938429915363" y=
-000042a0: 2236 3539 2e31 3633 3134 3937 3737 3939  "659.16314977799
-000042b0: 3939 2220 7769 6474 683d 2232 3235 2e32  99" width="225.2
-000042c0: 3133 3133 3531 3330 3135 3632 3522 2068  1313513015625" h
-000042d0: 6569 6768 743d 2232 322e 3836 3932 3834  eight="22.869284
-000042e0: 3632 222f 3e3c 2f67 3e3c 673e 3c72 6563  62"/></g><g><rec
-000042f0: 7420 6669 6c6c 3d22 7965 6c6c 6f77 2220  t fill="yellow" 
-00004300: 7374 726f 6b65 3d22 6e6f 6e65 2220 783d  stroke="none" x=
-00004310: 2232 3434 2e31 3938 3134 3739 3039 3135  "244.19814790915
-00004320: 3336 3522 2079 3d22 3636 312e 3937 3738  365" y="661.9778
-00004330: 3330 3936 3139 3939 3922 2077 6964 7468  309619999" width
-00004340: 3d22 3231 392e 3933 3536 3037 3931 3031  ="219.9356079101
-00004350: 3536 3235 2220 6865 6967 6874 3d22 3137  5625" height="17
-00004360: 2e37 3637 3637 3439 3734 222f 3e3c 7465  .767674974"/><te
-00004370: 7874 2066 696c 6c3d 2262 6c61 636b 2220  xt fill="black" 
-00004380: 7374 726f 6b65 3d22 6e6f 6e65 2220 666f  stroke="none" fo
-00004390: 6e74 2d66 616d 696c 793d 226d 6f6e 6f73  nt-family="monos
-000043a0: 7061 6365 2220 666f 6e74 2d73 697a 653d  pace" font-size=
-000043b0: 2231 3170 7422 2066 6f6e 742d 7374 796c  "11pt" font-styl
-000043c0: 653d 226e 6f72 6d61 6c22 2066 6f6e 742d  e="normal" font-
-000043d0: 7765 6967 6874 3d22 6e6f 726d 616c 2220  weight="normal" 
-000043e0: 7465 7874 2d64 6563 6f72 6174 696f 6e3d  text-decoration=
-000043f0: 226e 6f72 6d61 6c22 2078 3d22 3234 342e  "normal" x="244.
-00004400: 3139 3831 3437 3930 3931 3533 3635 2220  19814790915365" 
-00004410: 793d 2236 3734 2e39 3935 3733 3134 3337  y="674.995731437
-00004420: 3939 3939 2220 7465 7874 2d61 6e63 686f  9999" text-ancho
-00004430: 723d 2273 7461 7274 2220 646f 6d69 6e61  r="start" domina
-00004440: 6e74 2d62 6173 656c 696e 653d 2261 6c70  nt-baseline="alp
-00004450: 6861 6265 7469 6322 2078 6d6c 3a73 7061  habetic" xml:spa
-00004460: 6365 3d22 7072 6573 6572 7665 223e 6578  ce="preserve">ex
-00004470: 706f 7274 5f72 6573 6f75 7263 6528 696e  port_resource(in
-00004480: 7374 616e 6365 293c 2f74 6578 743e 3c2f  stance)</text></
-00004490: 673e 3c67 3e3c 7061 7468 2066 696c 6c3d  g><g><path fill=
-000044a0: 226e 6f6e 6522 2073 7472 6f6b 653d 2262  "none" stroke="b
-000044b0: 6c61 636b 2220 7061 696e 742d 6f72 6465  lack" paint-orde
-000044c0: 723d 2266 696c 6c20 7374 726f 6b65 206d  r="fill stroke m
-000044d0: 6172 6b65 7273 2220 643d 2220 4d20 3231  arkers" d=" M 21
-000044e0: 312e 3934 3635 3932 3637 3538 3230 3320  1.9465926758203 
-000044f0: 3638 322e 3033 3234 3334 3339 3739 3939  682.032434397999
-00004500: 3920 4c20 3239 312e 3130 3935 3030 3937  9 L 291.10950097
-00004510: 3538 3230 3320 3638 322e 3033 3234 3334  58203 682.032434
-00004520: 3339 3739 3939 3920 4c20 3239 312e 3130  3979999 L 291.10
-00004530: 3935 3030 3937 3538 3230 3320 3730 342e  95009758203 704.
-00004540: 3930 3137 3139 3031 3739 3939 3920 4c20  9017190179999 L 
-00004550: 3233 352e 3232 3633 3531 3633 3531 3533  235.226351635153
-00004560: 3636 2037 3034 2e39 3031 3731 3930 3137  66 704.901719017
-00004570: 3939 3939 2220 7374 726f 6b65 2d6d 6974  9999" stroke-mit
-00004580: 6572 6c69 6d69 743d 2231 3022 2073 7472  erlimit="10" str
-00004590: 6f6b 652d 7769 6474 683d 2231 2e34 3635  oke-width="1.465
-000045a0: 3937 3937 3833 3333 3333 3333 3222 2073  9797833333332" s
-000045b0: 7472 6f6b 652d 6461 7368 6172 7261 793d  troke-dasharray=
-000045c0: 2222 2f3e 3c67 2074 7261 6e73 666f 726d  ""/><g transform
-000045d0: 3d22 7472 616e 736c 6174 6528 3232 302e  ="translate(220.
-000045e0: 3734 3234 3731 3337 3538 3230 3332 2c37  74247137582032,7
-000045f0: 3034 2e39 3031 3731 3930 3137 3939 3939  04.9017190179999
-00004600: 2920 7472 616e 736c 6174 6528 2d32 3230  ) translate(-220
-00004610: 2e37 3432 3437 3133 3735 3832 3033 322c  .74247137582032,
-00004620: 2d37 3034 2e39 3031 3731 3930 3137 3939  -704.90171901799
-00004630: 3939 2922 3e3c 7061 7468 2066 696c 6c3d  99)"><path fill=
-00004640: 2262 6c61 636b 2220 7374 726f 6b65 3d22  "black" stroke="
-00004650: 6e6f 6e65 2220 7061 696e 742d 6f72 6465  none" paint-orde
-00004660: 723d 2273 7472 6f6b 6520 6669 6c6c 206d  r="stroke fill m
-00004670: 6172 6b65 7273 2220 643d 2220 4d20 3233  arkers" d=" M 23
-00004680: 352e 3430 3232 3639 3230 3931 3533 3634  5.40226920915364
-00004690: 2036 3937 2e35 3731 3832 3031 3031 3333   697.57182010133
-000046a0: 3332 204c 2032 3230 2e37 3432 3437 3133  32 L 220.7424713
-000046b0: 3735 3832 3033 3220 3730 342e 3930 3137  7582032 704.9017
-000046c0: 3139 3031 3739 3939 3920 4c20 3233 352e  190179999 L 235.
-000046d0: 3430 3232 3639 3230 3931 3533 3634 2037  40226920915364 7
-000046e0: 3132 2e32 3331 3631 3739 3334 3636 3636  12.2316179346666
-000046f0: 205a 222f 3e3c 2f67 3e3c 2f67 3e3c 673e   Z"/></g></g><g>
-00004700: 3c67 3e3c 7265 6374 2066 696c 6c3d 2272  <g><rect fill="r
-00004710: 6762 2832 3034 2c32 3330 2c32 3034 2922  gb(204,230,204)"
-00004720: 2073 7472 6f6b 653d 226e 6f6e 6522 2078   stroke="none" x
-00004730: 3d22 3235 302e 3335 3532 3632 3939 3931  ="250.3552629991
-00004740: 3533 3634 2220 793d 2237 3738 2e37 3837  5364" y="778.787
-00004750: 3130 3030 3937 3939 3939 2220 7769 6474  1000979999" widt
-00004760: 683d 2232 3630 2e34 3032 3833 3233 3935  h="260.402832395
-00004770: 3738 3133 2220 6865 6967 6874 3d22 3232  7813" height="22
-00004780: 2e38 3639 3238 3436 3222 2f3e 3c2f 673e  .86928462"/></g>
-00004790: 3c74 6578 7420 6669 6c6c 3d22 626c 6163  <text fill="blac
-000047a0: 6b22 2073 7472 6f6b 653d 226e 6f6e 6522  k" stroke="none"
-000047b0: 2066 6f6e 742d 6661 6d69 6c79 3d22 6d6f   font-family="mo
-000047c0: 6e6f 7370 6163 6522 2066 6f6e 742d 7369  nospace" font-si
-000047d0: 7a65 3d22 3131 7074 2220 666f 6e74 2d73  ze="11pt" font-s
-000047e0: 7479 6c65 3d22 6e6f 726d 616c 2220 666f  tyle="normal" fo
-000047f0: 6e74 2d77 6569 6768 743d 226e 6f72 6d61  nt-weight="norma
-00004800: 6c22 2074 6578 742d 6465 636f 7261 7469  l" text-decorati
-00004810: 6f6e 3d22 6e6f 726d 616c 2220 783d 2232  on="normal" x="2
-00004820: 3532 2e39 3934 3032 3636 3039 3135 3336  52.9940266091536
-00004830: 3522 2079 3d22 3739 342e 3631 3936 3831  5" y="794.619681
-00004840: 3735 3739 3939 3822 2074 6578 742d 616e  7579998" text-an
-00004850: 6368 6f72 3d22 7374 6172 7422 2064 6f6d  chor="start" dom
-00004860: 696e 616e 742d 6261 7365 6c69 6e65 3d22  inant-baseline="
-00004870: 616c 7068 6162 6574 6963 2220 786d 6c3a  alphabetic" xml:
-00004880: 7370 6163 653d 2270 7265 7365 7276 6522  space="preserve"
-00004890: 3e65 7870 6f72 745f 6669 656c 6428 6669  >export_field(fi
-000048a0: 656c 642c c2a0 696e 7374 616e 6365 293c  eld,..instance)<
-000048b0: 2f74 6578 743e 3c2f 673e 3c67 3e3c 7061  /text></g><g><pa
-000048c0: 7468 2066 696c 6c3d 226e 6f6e 6522 2073  th fill="none" s
-000048d0: 7472 6f6b 653d 2262 6c61 636b 2220 7061  troke="black" pa
-000048e0: 696e 742d 6f72 6465 723d 2266 696c 6c20  int-order="fill 
-000048f0: 7374 726f 6b65 206d 6172 6b65 7273 2220  stroke markers" 
-00004900: 643d 2220 4d20 3232 302e 3734 3234 3731  d=" M 220.742471
-00004910: 3337 3538 3230 3332 2038 3031 2e36 3536  37582032 801.656
-00004920: 3338 3437 3137 3939 3938 204c 2032 3939  3847179998 L 299
-00004930: 2e39 3035 3337 3936 3735 3832 3033 2038  .9053796758203 8
-00004940: 3031 2e36 3536 3338 3437 3137 3939 3938  01.6563847179998
-00004950: 204c 2032 3939 2e39 3035 3337 3936 3735   L 299.905379675
-00004960: 3832 3033 2038 3234 2e35 3235 3636 3933  8203 824.5256693
-00004970: 3337 3939 3938 204c 2032 3434 2e30 3232  379998 L 244.022
-00004980: 3233 3033 3335 3135 3336 3720 3832 342e  23033515367 824.
-00004990: 3532 3536 3639 3333 3739 3939 3822 2073  5256693379998" s
-000049a0: 7472 6f6b 652d 6d69 7465 726c 696d 6974  troke-miterlimit
-000049b0: 3d22 3130 2220 7374 726f 6b65 2d77 6964  ="10" stroke-wid
-000049c0: 7468 3d22 312e 3436 3539 3739 3738 3333  th="1.4659797833
-000049d0: 3333 3333 3332 2220 7374 726f 6b65 2d64  333332" stroke-d
-000049e0: 6173 6861 7272 6179 3d22 222f 3e3c 6720  asharray=""/><g 
-000049f0: 7472 616e 7366 6f72 6d3d 2274 7261 6e73  transform="trans
-00004a00: 6c61 7465 2832 3239 2e35 3338 3335 3030  late(229.5383500
-00004a10: 3735 3832 3033 322c 3832 342e 3532 3536  7582032,824.5256
-00004a20: 3639 3333 3739 3939 3829 2074 7261 6e73  693379998) trans
-00004a30: 6c61 7465 282d 3232 392e 3533 3833 3530  late(-229.538350
-00004a40: 3037 3538 3230 3332 2c2d 3832 342e 3532  07582032,-824.52
-00004a50: 3536 3639 3333 3739 3939 3829 223e 3c70  56693379998)"><p
-00004a60: 6174 6820 6669 6c6c 3d22 626c 6163 6b22  ath fill="black"
-00004a70: 2073 7472 6f6b 653d 226e 6f6e 6522 2070   stroke="none" p
-00004a80: 6169 6e74 2d6f 7264 6572 3d22 7374 726f  aint-order="stro
-00004a90: 6b65 2066 696c 6c20 6d61 726b 6572 7322  ke fill markers"
-00004aa0: 2064 3d22 204d 2032 3434 2e31 3938 3134   d=" M 244.19814
-00004ab0: 3739 3039 3135 3336 3520 3831 372e 3139  790915365 817.19
-00004ac0: 3537 3730 3432 3133 3333 3120 4c20 3232  57704213331 L 22
-00004ad0: 392e 3533 3833 3530 3037 3538 3230 3332  9.53835007582032
-00004ae0: 2038 3234 2e35 3235 3636 3933 3337 3939   824.52566933799
-00004af0: 3938 204c 2032 3434 2e31 3938 3134 3739  98 L 244.1981479
-00004b00: 3039 3135 3336 3520 3833 312e 3835 3535  0915365 831.8555
-00004b10: 3638 3235 3436 3636 3520 5a22 2f3e 3c2f  682546665 Z"/></
-00004b20: 673e 3c2f 673e 3c67 3e3c 673e 3c72 6563  g></g><g><g><rec
-00004b30: 7420 6669 6c6c 3d22 7267 6228 3230 342c  t fill="rgb(204,
-00004b40: 3233 302c 3230 3429 2220 7374 726f 6b65  230,204)" stroke
-00004b50: 3d22 6e6f 6e65 2220 783d 2233 3339 2e37  ="none" x="339.7
-00004b60: 3937 3033 3135 3632 3935 3537 3422 2079  9703156295574" y
-00004b70: 3d22 3835 302e 3931 3333 3035 3433 3739  ="850.9133054379
-00004b80: 3939 3822 2077 6964 7468 3d22 3134 362e  998" width="146.
-00004b90: 3033 3633 3136 3238 3235 2220 6865 6967  0363162825" heig
-00004ba0: 6874 3d22 3232 2e38 3639 3238 3436 3222  ht="22.86928462"
-00004bb0: 2f3e 3c2f 673e 3c74 6578 7420 6669 6c6c  /></g><text fill
-00004bc0: 3d22 626c 6163 6b22 2073 7472 6f6b 653d  ="black" stroke=
-00004bd0: 226e 6f6e 6522 2066 6f6e 742d 6661 6d69  "none" font-fami
-00004be0: 6c79 3d22 6d6f 6e6f 7370 6163 6522 2066  ly="monospace" f
-00004bf0: 6f6e 742d 7369 7a65 3d22 3131 7074 2220  ont-size="11pt" 
-00004c00: 666f 6e74 2d73 7479 6c65 3d22 6e6f 726d  font-style="norm
-00004c10: 616c 2220 666f 6e74 2d77 6569 6768 743d  al" font-weight=
-00004c20: 226e 6f72 6d61 6c22 2074 6578 742d 6465  "normal" text-de
-00004c30: 636f 7261 7469 6f6e 3d22 6e6f 726d 616c  coration="normal
-00004c40: 2220 783d 2233 3432 2e34 3335 3739 3531  " x="342.4357951
-00004c50: 3732 3935 3537 3522 2079 3d22 3836 362e  7295575" y="866.
-00004c60: 3734 3538 3837 3039 3739 3939 3822 2074  7458870979998" t
-00004c70: 6578 742d 616e 6368 6f72 3d22 7374 6172  ext-anchor="star
-00004c80: 7422 2064 6f6d 696e 616e 742d 6261 7365  t" dominant-base
-00004c90: 6c69 6e65 3d22 616c 7068 6162 6574 6963  line="alphabetic
-00004ca0: 2220 786d 6c3a 7370 6163 653d 2270 7265  " xml:space="pre
-00004cb0: 7365 7276 6522 3e65 7870 6f72 7428 696e  serve">export(in
-00004cc0: 7374 616e 6365 293c 2f74 6578 743e 3c2f  stance)</text></
-00004cd0: 673e 3c67 3e3c 7061 7468 2066 696c 6c3d  g><g><path fill=
-00004ce0: 226e 6f6e 6522 2073 7472 6f6b 653d 2262  "none" stroke="b
-00004cf0: 6c61 636b 2220 7061 696e 742d 6f72 6465  lack" paint-orde
-00004d00: 723d 2266 696c 6c20 7374 726f 6b65 206d  r="fill stroke m
-00004d10: 6172 6b65 7273 2220 643d 2220 4d20 3232  arkers" d=" M 22
-00004d20: 392e 3533 3833 3530 3037 3538 3230 3332  9.53835007582032
-00004d30: 2038 3733 2e37 3832 3539 3030 3537 3939   873.78259005799
-00004d40: 3939 204c 2035 3831 2e36 3038 3134 3930  99 L 581.6081490
-00004d50: 3733 3235 3739 2038 3733 2e37 3832 3539  732579 873.78259
-00004d60: 3030 3537 3939 3939 2220 7374 726f 6b65  00579999" stroke
-00004d70: 2d6d 6974 6572 6c69 6d69 743d 2231 3022  -miterlimit="10"
-00004d80: 2073 7472 6f6b 652d 7769 6474 683d 2231   stroke-width="1
-00004d90: 2e34 3635 3937 3937 3833 3333 3333 3333  .465979783333333
-00004da0: 3222 2073 7472 6f6b 652d 6461 7368 6172  2" stroke-dashar
-00004db0: 7261 793d 2222 2f3e 3c67 2074 7261 6e73  ray=""/><g trans
-00004dc0: 666f 726d 3d22 7472 616e 736c 6174 6528  form="translate(
-00004dd0: 3539 362e 3039 3230 3239 3333 3235 3931  596.092029332591
-00004de0: 322c 3837 332e 3738 3235 3930 3035 3739  2,873.7825900579
-00004df0: 3939 3929 2074 7261 6e73 6c61 7465 282d  999) translate(-
-00004e00: 3539 362e 3039 3230 3239 3333 3235 3931  596.092029332591
-00004e10: 322c 2d38 3733 2e37 3832 3539 3030 3537  2,-873.782590057
-00004e20: 3939 3939 2922 3e3c 7061 7468 2066 696c  9999)"><path fil
-00004e30: 6c3d 2262 6c61 636b 2220 7374 726f 6b65  l="black" stroke
-00004e40: 3d22 6e6f 6e65 2220 7061 696e 742d 6f72  ="none" paint-or
-00004e50: 6465 723d 2273 7472 6f6b 6520 6669 6c6c  der="stroke fill
-00004e60: 206d 6172 6b65 7273 2220 643d 2220 4d20   markers" d=" M 
-00004e70: 3538 312e 3433 3232 3331 3439 3932 3537  581.432231499257
-00004e80: 3920 3836 362e 3435 3236 3931 3134 3133  9 866.4526911413
-00004e90: 3333 3220 4c20 3539 362e 3039 3230 3239  332 L 596.092029
-00004ea0: 3333 3235 3931 3220 3837 332e 3738 3235  3325912 873.7825
-00004eb0: 3930 3035 3739 3939 3920 4c20 3538 312e  900579999 L 581.
-00004ec0: 3433 3232 3331 3439 3932 3537 3920 3838  4322314992579 88
-00004ed0: 312e 3131 3234 3838 3937 3436 3636 3620  1.1124889746666 
-00004ee0: 5a22 2f3e 3c2f 673e 3c2f 673e 3c70 6174  Z"/></g></g><pat
-00004ef0: 6820 6669 6c6c 3d22 7768 6974 6522 2073  h fill="white" s
-00004f00: 7472 6f6b 653d 2262 6c61 636b 2220 7061  troke="black" pa
-00004f10: 696e 742d 6f72 6465 723d 2266 696c 6c20  int-order="fill 
-00004f20: 7374 726f 6b65 206d 6172 6b65 7273 2220  stroke markers" 
-00004f30: 643d 2220 4d20 3430 332e 3430 3931 3531  d=" M 403.409151
-00004f40: 3635 3230 3833 3434 2039 3030 2e31 3730  65208344 900.170
-00004f50: 3232 3631 3537 3939 3938 204c 2037 3930  2261579998 L 790
-00004f60: 2e35 3334 3038 3237 3533 3039 3920 3930  .534082753099 90
-00004f70: 302e 3137 3032 3236 3135 3739 3939 3820  0.1702261579998 
-00004f80: 4c20 3830 362e 3336 3636 3634 3431 3330  L 806.3666644130
-00004f90: 3939 2039 3136 2e30 3032 3830 3738 3137  99 916.002807817
-00004fa0: 3939 3937 204c 2038 3036 2e33 3636 3636  9997 L 806.36666
-00004fb0: 3434 3133 3039 3920 3935 382e 3232 3330  4413099 958.2230
-00004fc0: 3235 3537 3739 3939 3820 4c20 3430 332e  255779998 L 403.
-00004fd0: 3430 3931 3531 3635 3230 3833 3434 2039  40915165208344 9
-00004fe0: 3538 2e32 3233 3032 3535 3737 3939 3938  58.2230255779998
-00004ff0: 204c 2034 3033 2e34 3039 3135 3136 3532   L 403.409151652
-00005000: 3038 3334 3420 3930 302e 3137 3032 3236  08344 900.170226
-00005010: 3135 3739 3939 3820 4d20 3739 302e 3533  1579998 M 790.53
-00005020: 3430 3832 3735 3330 3939 2039 3030 2e31  4082753099 900.1
-00005030: 3730 3232 3631 3537 3939 3938 204c 2037  702261579998 L 7
-00005040: 3930 2e35 3334 3038 3237 3533 3039 3920  90.534082753099 
-00005050: 3931 362e 3030 3238 3037 3831 3739 3939  916.002807817999
-00005060: 3720 4c20 3830 362e 3336 3636 3634 3431  7 L 806.36666441
-00005070: 3330 3939 2039 3136 2e30 3032 3830 3738  3099 916.0028078
-00005080: 3137 3939 3937 2220 7374 726f 6b65 2d6d  179997" stroke-m
-00005090: 6974 6572 6c69 6d69 743d 2231 3022 2073  iterlimit="10" s
-000050a0: 7472 6f6b 652d 7769 6474 683d 2231 2e34  troke-width="1.4
-000050b0: 3635 3937 3937 3833 3333 3333 3333 3222  659797833333332"
-000050c0: 2073 7472 6f6b 652d 6461 7368 6172 7261   stroke-dasharra
-000050d0: 793d 2222 2f3e 3c67 3e3c 7465 7874 2066  y=""/><g><text f
-000050e0: 696c 6c3d 2262 6c61 636b 2220 7374 726f  ill="black" stro
-000050f0: 6b65 3d22 6e6f 6e65 2220 666f 6e74 2d66  ke="none" font-f
-00005100: 616d 696c 793d 2273 616e 732d 7365 7269  amily="sans-seri
-00005110: 6622 2066 6f6e 742d 7369 7a65 3d22 3131  f" font-size="11
-00005120: 7074 2220 666f 6e74 2d73 7479 6c65 3d22  pt" font-style="
-00005130: 6e6f 726d 616c 2220 666f 6e74 2d77 6569  normal" font-wei
-00005140: 6768 743d 226e 6f72 6d61 6c22 2074 6578  ght="normal" tex
-00005150: 742d 6465 636f 7261 7469 6f6e 3d22 6e6f  t-decoration="no
-00005160: 726d 616c 2220 783d 2234 3238 2e30 3337  rmal" x="428.037
-00005170: 3631 3230 3132 3038 3334 2220 793d 2239  6120120834" y="9
-00005180: 3234 2e37 3938 3638 3635 3137 3939 3938  24.7986865179998
-00005190: 2220 7465 7874 2d61 6e63 686f 723d 2273  " text-anchor="s
-000051a0: 7461 7274 2220 646f 6d69 6e61 6e74 2d62  tart" dominant-b
-000051b0: 6173 656c 696e 653d 2261 6c70 6861 6265  aseline="alphabe
-000051c0: 7469 6322 2078 6d6c 3a73 7061 6365 3d22  tic" xml:space="
-000051d0: 7072 6573 6572 7665 223e 416e c2a0 6f70  preserve">An..op
-000051e0: 7469 6f6e 616c c2a0 6361 6c6c 6162 6c65  tional..callable
-000051f0: c2a0 6361 6ec2 a062 65c2 a064 6566 696e  ..can..be..defin
-00005200: 6564 c2a0 696e 7374 6561 64c2 a06f 66c2  ed..instead..of.
-00005210: a065 7870 6f72 7428 292e 3c2f 7465 7874  .export().</text
-00005220: 3e3c 7465 7874 2066 696c 6c3d 2262 6c61  ><text fill="bla
-00005230: 636b 2220 7374 726f 6b65 3d22 6e6f 6e65  ck" stroke="none
-00005240: 2220 666f 6e74 2d66 616d 696c 793d 2273  " font-family="s
-00005250: 616e 732d 7365 7269 6622 2066 6f6e 742d  ans-serif" font-
-00005260: 7369 7a65 3d22 3131 7074 2220 666f 6e74  size="11pt" font
-00005270: 2d73 7479 6c65 3d22 6e6f 726d 616c 2220  -style="normal" 
-00005280: 666f 6e74 2d77 6569 6768 743d 226e 6f72  font-weight="nor
-00005290: 6d61 6c22 2074 6578 742d 6465 636f 7261  mal" text-decora
-000052a0: 7469 6f6e 3d22 6e6f 726d 616c 2220 783d  tion="normal" x=
-000052b0: 2234 3238 2e30 3337 3631 3230 3132 3038  "428.03761201208
-000052c0: 3334 2220 793d 2239 3432 2e33 3930 3434  34" y="942.39044
-000052d0: 3339 3137 3939 3938 2220 7465 7874 2d61  39179998" text-a
-000052e0: 6e63 686f 723d 2273 7461 7274 2220 646f  nchor="start" do
-000052f0: 6d69 6e61 6e74 2d62 6173 656c 696e 653d  minant-baseline=
-00005300: 2261 6c70 6861 6265 7469 6322 2078 6d6c  "alphabetic" xml
-00005310: 3a73 7061 6365 3d22 7072 6573 6572 7665  :space="preserve
-00005320: 223e c2a0 5365 65c2 a027 6465 6879 6472  ">..See..'dehydr
-00005330: 6174 6527 c2a0 6d65 7468 6f64 73c2 a069  ate'..methods..i
-00005340: 6ec2 a064 6f63 732e 3c2f 7465 7874 3e3c  n..docs.</text><
-00005350: 2f67 3e3c 673e 3c67 3e3c 7265 6374 2066  /g><g><g><rect f
-00005360: 696c 6c3d 2272 6762 2832 3034 2c32 3330  ill="rgb(204,230
-00005370: 2c32 3034 2922 2073 7472 6f6b 653d 226e  ,204)" stroke="n
-00005380: 6f6e 6522 2078 3d22 3634 332e 3239 3635  one" x="643.2965
-00005390: 3738 3335 3539 3234 3622 2079 3d22 3938  783559246" y="98
-000053a0: 342e 3631 3036 3631 3637 3739 3939 3922  4.6106616779999"
-000053b0: 2077 6964 7468 3d22 3137 322e 3432 3835   width="172.4285
-000053c0: 3839 3233 3137 3138 3735 2220 6865 6967  8923171875" heig
-000053d0: 6874 3d22 3232 2e38 3639 3238 3436 3222  ht="22.86928462"
-000053e0: 2f3e 3c2f 673e 3c74 6578 7420 6669 6c6c  /></g><text fill
-000053f0: 3d22 626c 6163 6b22 2073 7472 6f6b 653d  ="black" stroke=
-00005400: 226e 6f6e 6522 2066 6f6e 742d 6661 6d69  "none" font-fami
-00005410: 6c79 3d22 6d6f 6e6f 7370 6163 6522 2066  ly="monospace" f
-00005420: 6f6e 742d 7369 7a65 3d22 3131 7074 2220  ont-size="11pt" 
-00005430: 666f 6e74 2d73 7479 6c65 3d22 6e6f 726d  font-style="norm
-00005440: 616c 2220 666f 6e74 2d77 6569 6768 743d  al" font-weight=
-00005450: 226e 6f72 6d61 6c22 2074 6578 742d 6465  "normal" text-de
-00005460: 636f 7261 7469 6f6e 3d22 6e6f 726d 616c  coration="normal
-00005470: 2220 783d 2236 3435 2e39 3335 3334 3139  " x="645.9353419
-00005480: 3635 3932 3435 2220 793d 2231 3030 302e  659245" y="1000.
-00005490: 3434 3332 3433 3333 3739 3939 3922 2074  4432433379999" t
-000054a0: 6578 742d 616e 6368 6f72 3d22 7374 6172  ext-anchor="star
-000054b0: 7422 2064 6f6d 696e 616e 742d 6261 7365  t" dominant-base
-000054c0: 6c69 6e65 3d22 616c 7068 6162 6574 6963  line="alphabetic
-000054d0: 2220 786d 6c3a 7370 6163 653d 2270 7265  " xml:space="pre
-000054e0: 7365 7276 6522 3e67 6574 5f76 616c 7565  serve">get_value
-000054f0: 2869 6e73 7461 6e63 6529 3c2f 7465 7874  (instance)</text
-00005500: 3e3c 2f67 3e3c 673e 3c70 6174 6820 6669  ></g><g><path fi
-00005510: 6c6c 3d22 6e6f 6e65 2220 7374 726f 6b65  ll="none" stroke
-00005520: 3d22 626c 6163 6b22 2070 6169 6e74 2d6f  ="black" paint-o
-00005530: 7264 6572 3d22 6669 6c6c 2073 7472 6f6b  rder="fill strok
-00005540: 6520 6d61 726b 6572 7322 2064 3d22 204d  e markers" d=" M
-00005550: 2036 3133 2e36 3833 3738 3637 3332 3539   613.68378673259
-00005560: 3132 2031 3030 372e 3437 3939 3436 3239  12 1007.47994629
-00005570: 3739 3939 3820 4c20 3639 322e 3834 3636  79998 L 692.8466
-00005580: 3935 3033 3235 3931 3220 3130 3037 2e34  950325912 1007.4
-00005590: 3739 3934 3632 3937 3939 3938 204c 2036  799462979998 L 6
-000055a0: 3932 2e38 3436 3639 3530 3332 3539 3132  92.8466950325912
-000055b0: 2031 3033 302e 3334 3932 3330 3931 3739   1030.3492309179
-000055c0: 3939 3920 4c20 3633 362e 3936 3335 3435  999 L 636.963545
-000055d0: 3639 3139 3234 3520 3130 3330 2e33 3439  6919245 1030.349
-000055e0: 3233 3039 3137 3939 3939 2220 7374 726f  2309179999" stro
-000055f0: 6b65 2d6d 6974 6572 6c69 6d69 743d 2231  ke-miterlimit="1
-00005600: 3022 2073 7472 6f6b 652d 7769 6474 683d  0" stroke-width=
-00005610: 2231 2e34 3635 3937 3937 3833 3333 3333  "1.4659797833333
-00005620: 3333 3222 2073 7472 6f6b 652d 6461 7368  332" stroke-dash
-00005630: 6172 7261 793d 2222 2f3e 3c67 2074 7261  array=""/><g tra
-00005640: 6e73 666f 726d 3d22 7472 616e 736c 6174  nsform="translat
-00005650: 6528 3632 322e 3437 3936 3635 3433 3235  e(622.4796654325
-00005660: 3931 322c 3130 3330 2e33 3439 3233 3039  912,1030.3492309
-00005670: 3137 3939 3939 2920 7472 616e 736c 6174  179999) translat
-00005680: 6528 2d36 3232 2e34 3739 3636 3534 3332  e(-622.479665432
-00005690: 3539 3132 2c2d 3130 3330 2e33 3439 3233  5912,-1030.34923
-000056a0: 3039 3137 3939 3939 2922 3e3c 7061 7468  09179999)"><path
-000056b0: 2066 696c 6c3d 2262 6c61 636b 2220 7374   fill="black" st
-000056c0: 726f 6b65 3d22 6e6f 6e65 2220 7061 696e  roke="none" pain
-000056d0: 742d 6f72 6465 723d 2273 7472 6f6b 6520  t-order="stroke 
-000056e0: 6669 6c6c 206d 6172 6b65 7273 2220 643d  fill markers" d=
-000056f0: 2220 4d20 3633 372e 3133 3934 3633 3236  " M 637.13946326
-00005700: 3539 3234 3520 3130 3233 2e30 3139 3333  59245 1023.01933
-00005710: 3230 3031 3333 3332 204c 2036 3232 2e34  20013332 L 622.4
-00005720: 3739 3636 3534 3332 3539 3132 2031 3033  796654325912 103
-00005730: 302e 3334 3932 3330 3931 3739 3939 3920  0.3492309179999 
-00005740: 4c20 3633 372e 3133 3934 3633 3236 3539  L 637.1394632659
-00005750: 3234 3520 3130 3337 2e36 3739 3132 3938  245 1037.6791298
-00005760: 3334 3636 3636 205a 222f 3e3c 2f67 3e3c  346666 Z"/></g><
-00005770: 2f67 3e3c 7061 7468 2066 696c 6c3d 2277  /g><path fill="w
-00005780: 6869 7465 2220 7374 726f 6b65 3d22 626c  hite" stroke="bl
-00005790: 6163 6b22 2070 6169 6e74 2d6f 7264 6572  ack" paint-order
-000057a0: 3d22 6669 6c6c 2073 7472 6f6b 6520 6d61  ="fill stroke ma
-000057b0: 726b 6572 7322 2064 3d22 204d 2034 3535  rkers" d=" M 455
-000057c0: 2e38 3134 3235 3732 3432 3930 3337 3520  .81425724290375 
-000057d0: 3130 3536 2e37 3336 3836 3730 3137 3939  1056.73686701799
-000057e0: 3939 204c 2037 3338 2e31 3238 3937 3731  99 L 738.1289771
-000057f0: 3632 3237 3837 2031 3035 362e 3733 3638  622787 1056.7368
-00005800: 3637 3031 3739 3939 3920 4c20 3735 332e  670179999 L 753.
-00005810: 3936 3135 3538 3832 3232 3738 3720 3130  9615588222787 10
-00005820: 3732 2e35 3639 3434 3836 3737 3939 3938  72.5694486779998
-00005830: 204c 2037 3533 2e39 3631 3535 3838 3232   L 753.961558822
-00005840: 3237 3837 2031 3039 372e 3139 3739 3039  2787 1097.197909
-00005850: 3033 3739 3939 3820 4c20 3435 352e 3831  0379998 L 455.81
-00005860: 3432 3537 3234 3239 3033 3735 2031 3039  425724290375 109
-00005870: 372e 3139 3739 3039 3033 3739 3939 3820  7.1979090379998 
-00005880: 4c20 3435 352e 3831 3432 3537 3234 3239  L 455.8142572429
-00005890: 3033 3735 2031 3035 362e 3733 3638 3637  0375 1056.736867
-000058a0: 3031 3739 3939 3920 4d20 3733 382e 3132  0179999 M 738.12
-000058b0: 3839 3737 3136 3232 3738 3720 3130 3536  89771622787 1056
-000058c0: 2e37 3336 3836 3730 3137 3939 3939 204c  .7368670179999 L
-000058d0: 2037 3338 2e31 3238 3937 3731 3632 3237   738.12897716227
-000058e0: 3837 2031 3037 322e 3536 3934 3438 3637  87 1072.56944867
-000058f0: 3739 3939 3820 4c20 3735 332e 3936 3135  79998 L 753.9615
-00005900: 3538 3832 3232 3738 3720 3130 3732 2e35  588222787 1072.5
-00005910: 3639 3434 3836 3737 3939 3938 2220 7374  694486779998" st
-00005920: 726f 6b65 2d6d 6974 6572 6c69 6d69 743d  roke-miterlimit=
-00005930: 2231 3022 2073 7472 6f6b 652d 7769 6474  "10" stroke-widt
-00005940: 683d 2231 2e34 3635 3937 3937 3833 3333  h="1.46597978333
-00005950: 3333 3333 3222 2073 7472 6f6b 652d 6461  33332" stroke-da
-00005960: 7368 6172 7261 793d 2222 2f3e 3c67 3e3c  sharray=""/><g><
-00005970: 7465 7874 2066 696c 6c3d 2262 6c61 636b  text fill="black
-00005980: 2220 7374 726f 6b65 3d22 6e6f 6e65 2220  " stroke="none" 
-00005990: 666f 6e74 2d66 616d 696c 793d 2273 616e  font-family="san
-000059a0: 732d 7365 7269 6622 2066 6f6e 742d 7369  s-serif" font-si
-000059b0: 7a65 3d22 3131 7074 2220 666f 6e74 2d73  ze="11pt" font-s
-000059c0: 7479 6c65 3d22 6e6f 726d 616c 2220 666f  tyle="normal" fo
-000059d0: 6e74 2d77 6569 6768 743d 226e 6f72 6d61  nt-weight="norma
-000059e0: 6c22 2074 6578 742d 6465 636f 7261 7469  l" text-decorati
-000059f0: 6f6e 3d22 6e6f 726d 616c 2220 783d 2234  on="normal" x="4
-00005a00: 3830 2e34 3432 3731 3736 3032 3930 3337  80.4427176029037
-00005a10: 2220 793d 2231 3038 312e 3336 3533 3237  " y="1081.365327
-00005a20: 3337 3739 3939 3622 2074 6578 742d 616e  3779996" text-an
-00005a30: 6368 6f72 3d22 7374 6172 7422 2064 6f6d  chor="start" dom
-00005a40: 696e 616e 742d 6261 7365 6c69 6e65 3d22  inant-baseline="
-00005a50: 616c 7068 6162 6574 6963 2220 786d 6c3a  alphabetic" xml:
-00005a60: 7370 6163 653d 2270 7265 7365 7276 6522  space="preserve"
-00005a70: 3e47 6574 c2a0 7468 65c2 a066 6965 6c64  >Get..the..field
-00005a80: 2773 c2a0 7661 6c75 65c2 a066 726f 6dc2  's..value..from.
-00005a90: a074 6865 c2a0 696e 7374 616e 6365 2e3c  .the..instance.<
-00005aa0: 2f74 6578 743e 3c2f 673e 3c67 3e3c 673e  /text></g><g><g>
-00005ab0: 3c72 6563 7420 6669 6c6c 3d22 7267 6228  <rect fill="rgb(
-00005ac0: 3230 342c 3233 302c 3230 3429 2220 7374  204,230,204)" st
-00005ad0: 726f 6b65 3d22 6e6f 6e65 2220 783d 2236  roke="none" x="6
-00005ae0: 3433 2e32 3936 3537 3833 3535 3932 3436  43.2965783559246
-00005af0: 2220 793d 2231 3132 332e 3538 3535 3435  " y="1123.585545
-00005b00: 3133 3739 3939 3822 2077 6964 7468 3d22  1379998" width="
-00005b10: 3834 2e34 3534 3334 3630 3637 3635 3632  84.4543460676562
-00005b20: 3522 2068 6569 6768 743d 2232 322e 3836  5" height="22.86
-00005b30: 3932 3834 3632 222f 3e3c 2f67 3e3c 7465  928462"/></g><te
-00005b40: 7874 2066 696c 6c3d 2262 6c61 636b 2220  xt fill="black" 
-00005b50: 7374 726f 6b65 3d22 6e6f 6e65 2220 666f  stroke="none" fo
-00005b60: 6e74 2d66 616d 696c 793d 226d 6f6e 6f73  nt-family="monos
-00005b70: 7061 6365 2220 666f 6e74 2d73 697a 653d  pace" font-size=
-00005b80: 2231 3170 7422 2066 6f6e 742d 7374 796c  "11pt" font-styl
-00005b90: 653d 226e 6f72 6d61 6c22 2066 6f6e 742d  e="normal" font-
-00005ba0: 7765 6967 6874 3d22 6e6f 726d 616c 2220  weight="normal" 
-00005bb0: 7465 7874 2d64 6563 6f72 6174 696f 6e3d  text-decoration=
-00005bc0: 226e 6f72 6d61 6c22 2078 3d22 3634 352e  "normal" x="645.
-00005bd0: 3933 3533 3431 3936 3539 3234 3522 2079  9353419659245" y
-00005be0: 3d22 3131 3339 2e34 3138 3132 3637 3937  ="1139.418126797
-00005bf0: 3939 3938 2220 7465 7874 2d61 6e63 686f  9998" text-ancho
-00005c00: 723d 2273 7461 7274 2220 646f 6d69 6e61  r="start" domina
-00005c10: 6e74 2d62 6173 656c 696e 653d 2261 6c70  nt-baseline="alp
-00005c20: 6861 6265 7469 6322 2078 6d6c 3a73 7061  habetic" xml:spa
-00005c30: 6365 3d22 7072 6573 6572 7665 223e 266c  ce="preserve">&l
-00005c40: 743b 266c 743b 7661 6c75 6526 6774 3b26  t;&lt;value&gt;&
-00005c50: 6774 3b3c 2f74 6578 743e 3c2f 673e 3c67  gt;</text></g><g
-00005c60: 3e3c 7061 7468 2066 696c 6c3d 226e 6f6e  ><path fill="non
-00005c70: 6522 2073 7472 6f6b 653d 2262 6c61 636b  e" stroke="black
-00005c80: 2220 7061 696e 742d 6f72 6465 723d 2266  " paint-order="f
-00005c90: 696c 6c20 7374 726f 6b65 206d 6172 6b65  ill stroke marke
-00005ca0: 7273 2220 643d 2220 4d20 3632 322e 3437  rs" d=" M 622.47
-00005cb0: 3936 3635 3433 3235 3931 3220 3131 3436  96654325912 1146
-00005cc0: 2e34 3534 3832 3937 3538 204c 2036 3932  .454829758 L 692
-00005cd0: 2e38 3436 3639 3530 3332 3539 3132 2031  .8466950325912 1
-00005ce0: 3134 362e 3435 3438 3239 3735 3820 4c20  146.454829758 L 
-00005cf0: 3639 322e 3834 3636 3935 3033 3235 3931  692.846695032591
-00005d00: 3220 3131 3639 2e33 3234 3131 3433 3737  2 1169.324114377
-00005d10: 3939 3939 204c 2036 3336 2e39 3633 3534  9999 L 636.96354
-00005d20: 3536 3931 3932 3435 2031 3136 392e 3332  56919245 1169.32
-00005d30: 3431 3134 3337 3739 3939 3922 2073 7472  41143779999" str
-00005d40: 6f6b 652d 6d69 7465 726c 696d 6974 3d22  oke-miterlimit="
-00005d50: 3130 2220 7374 726f 6b65 2d77 6964 7468  10" stroke-width
-00005d60: 3d22 312e 3436 3539 3739 3738 3333 3333  ="1.465979783333
-00005d70: 3333 3332 2220 7374 726f 6b65 2d64 6173  3332" stroke-das
-00005d80: 6861 7272 6179 3d22 372e 3033 3637 3032  harray="7.036702
-00005d90: 3935 3939 3939 3939 3935 222f 3e3c 6720  9599999995"/><g 
-00005da0: 7472 616e 7366 6f72 6d3d 2274 7261 6e73  transform="trans
-00005db0: 6c61 7465 2836 3232 2e34 3739 3636 3534  late(622.4796654
-00005dc0: 3332 3539 3132 2c31 3136 392e 3332 3431  325912,1169.3241
-00005dd0: 3134 3337 3739 3939 3929 2074 7261 6e73  143779999) trans
-00005de0: 6c61 7465 282d 3632 322e 3437 3936 3635  late(-622.479665
-00005df0: 3433 3235 3931 322c 2d31 3136 392e 3332  4325912,-1169.32
-00005e00: 3431 3134 3337 3739 3939 3929 223e 3c70  41143779999)"><p
-00005e10: 6174 6820 6669 6c6c 3d22 626c 6163 6b22  ath fill="black"
-00005e20: 2073 7472 6f6b 653d 226e 6f6e 6522 2070   stroke="none" p
-00005e30: 6169 6e74 2d6f 7264 6572 3d22 7374 726f  aint-order="stro
-00005e40: 6b65 2066 696c 6c20 6d61 726b 6572 7322  ke fill markers"
-00005e50: 2064 3d22 204d 2036 3337 2e31 3339 3436   d=" M 637.13946
-00005e60: 3332 3635 3932 3435 2031 3136 312e 3939  32659245 1161.99
-00005e70: 3432 3135 3436 3133 3333 3220 4c20 3632  42154613332 L 62
-00005e80: 322e 3437 3936 3635 3433 3235 3931 3220  2.4796654325912 
-00005e90: 3131 3639 2e33 3234 3131 3433 3737 3939  1169.32411437799
-00005ea0: 3939 204c 2036 3337 2e31 3339 3436 3332  99 L 637.1394632
-00005eb0: 3635 3932 3435 2031 3137 362e 3635 3430  659245 1176.6540
-00005ec0: 3133 3239 3436 3636 3620 5a22 2f3e 3c2f  132946666 Z"/></
-00005ed0: 673e 3c2f 673e 3c67 3e3c 673e 3c72 6563  g></g><g><g><rec
-00005ee0: 7420 6669 6c6c 3d22 7267 6228 3230 342c  t fill="rgb(204,
-00005ef0: 3233 302c 3230 3429 2220 7374 726f 6b65  230,204)" stroke
-00005f00: 3d22 6e6f 6e65 2220 783d 2236 3433 2e32  ="none" x="643.2
-00005f10: 3936 3537 3833 3535 3932 3436 2220 793d  965783559246" y=
-00005f20: 2231 3139 352e 3731 3137 3530 3437 3739  "1195.7117504779
-00005f30: 3939 3922 2077 6964 7468 3d22 3230 372e  999" width="207.
-00005f40: 3631 3832 3836 3439 3733 3433 3735 2220  61828649734375" 
-00005f50: 6865 6967 6874 3d22 3232 2e38 3639 3238  height="22.86928
-00005f60: 3436 3222 2f3e 3c2f 673e 3c74 6578 7420  462"/></g><text 
-00005f70: 6669 6c6c 3d22 626c 6163 6b22 2073 7472  fill="black" str
-00005f80: 6f6b 653d 226e 6f6e 6522 2066 6f6e 742d  oke="none" font-
-00005f90: 6661 6d69 6c79 3d22 6d6f 6e6f 7370 6163  family="monospac
-00005fa0: 6522 2066 6f6e 742d 7369 7a65 3d22 3131  e" font-size="11
-00005fb0: 7074 2220 666f 6e74 2d73 7479 6c65 3d22  pt" font-style="
-00005fc0: 6e6f 726d 616c 2220 666f 6e74 2d77 6569  normal" font-wei
-00005fd0: 6768 743d 226e 6f72 6d61 6c22 2074 6578  ght="normal" tex
-00005fe0: 742d 6465 636f 7261 7469 6f6e 3d22 6e6f  t-decoration="no
-00005ff0: 726d 616c 2220 783d 2236 3435 2e39 3335  rmal" x="645.935
-00006000: 3334 3139 3635 3932 3435 2220 793d 2231  3419659245" y="1
-00006010: 3231 312e 3534 3433 3332 3133 3739 3939  211.544332137999
-00006020: 3822 2074 6578 742d 616e 6368 6f72 3d22  8" text-anchor="
-00006030: 7374 6172 7422 2064 6f6d 696e 616e 742d  start" dominant-
-00006040: 6261 7365 6c69 6e65 3d22 616c 7068 6162  baseline="alphab
-00006050: 6574 6963 2220 786d 6c3a 7370 6163 653d  etic" xml:space=
-00006060: 2270 7265 7365 7276 6522 3e72 656e 6465  "preserve">rende
-00006070: 7228 7661 6c75 652c c2a0 696e 7374 616e  r(value,..instan
-00006080: 6365 293c 2f74 6578 743e 3c2f 673e 3c67  ce)</text></g><g
-00006090: 3e3c 7061 7468 2066 696c 6c3d 226e 6f6e  ><path fill="non
-000060a0: 6522 2073 7472 6f6b 653d 2262 6c61 636b  e" stroke="black
-000060b0: 2220 7061 696e 742d 6f72 6465 723d 2266  " paint-order="f
-000060c0: 696c 6c20 7374 726f 6b65 206d 6172 6b65  ill stroke marke
-000060d0: 7273 2220 643d 2220 4d20 3632 322e 3437  rs" d=" M 622.47
-000060e0: 3936 3635 3433 3235 3931 3220 3132 3138  96654325912 1218
-000060f0: 2e35 3831 3033 3530 3937 3939 3938 204c  .5810350979998 L
-00006100: 2038 3537 2e32 3437 3839 3735 3137 3236   857.24789751726
-00006110: 3833 2031 3231 382e 3538 3130 3335 3039  83 1218.58103509
-00006120: 3739 3939 3822 2073 7472 6f6b 652d 6d69  79998" stroke-mi
-00006130: 7465 726c 696d 6974 3d22 3130 2220 7374  terlimit="10" st
-00006140: 726f 6b65 2d77 6964 7468 3d22 312e 3436  roke-width="1.46
-00006150: 3539 3739 3738 3333 3333 3333 3332 2220  59797833333332" 
-00006160: 7374 726f 6b65 2d64 6173 6861 7272 6179  stroke-dasharray
-00006170: 3d22 222f 3e3c 6720 7472 616e 7366 6f72  =""/><g transfor
-00006180: 6d3d 2274 7261 6e73 6c61 7465 2838 3731  m="translate(871
-00006190: 2e37 3331 3737 3737 3736 3630 3136 2c31  .7317777766016,1
-000061a0: 3231 382e 3538 3130 3335 3039 3739 3939  218.581035097999
-000061b0: 3829 2074 7261 6e73 6c61 7465 282d 3837  8) translate(-87
-000061c0: 312e 3733 3137 3737 3737 3636 3031 362c  1.7317777766016,
-000061d0: 2d31 3231 382e 3538 3130 3335 3039 3739  -1218.5810350979
-000061e0: 3939 3829 223e 3c70 6174 6820 6669 6c6c  998)"><path fill
-000061f0: 3d22 626c 6163 6b22 2073 7472 6f6b 653d  ="black" stroke=
-00006200: 226e 6f6e 6522 2070 6169 6e74 2d6f 7264  "none" paint-ord
-00006210: 6572 3d22 7374 726f 6b65 2066 696c 6c20  er="stroke fill 
-00006220: 6d61 726b 6572 7322 2064 3d22 204d 2038  markers" d=" M 8
-00006230: 3537 2e30 3731 3937 3939 3433 3236 3833  57.0719799432683
-00006240: 2031 3231 312e 3235 3131 3336 3138 3133   1211.2511361813
-00006250: 3333 204c 2038 3731 2e37 3331 3737 3737  33 L 871.7317777
-00006260: 3736 3630 3136 2031 3231 382e 3538 3130  766016 1218.5810
-00006270: 3335 3039 3739 3939 3820 4c20 3835 372e  350979998 L 857.
-00006280: 3037 3139 3739 3934 3332 3638 3320 3132  0719799432683 12
-00006290: 3235 2e39 3130 3933 3430 3134 3636 3635  25.9109340146665
-000062a0: 205a 222f 3e3c 2f67 3e3c 2f67 3e3c 7061   Z"/></g></g><pa
-000062b0: 7468 2066 696c 6c3d 2277 6869 7465 2220  th fill="white" 
-000062c0: 7374 726f 6b65 3d22 626c 6163 6b22 2070  stroke="black" p
-000062d0: 6169 6e74 2d6f 7264 6572 3d22 6669 6c6c  aint-order="fill
-000062e0: 2073 7472 6f6b 6520 6d61 726b 6572 7322   stroke markers"
-000062f0: 2064 3d22 204d 2037 3639 2e31 3136 3835   d=" M 769.11685
-00006300: 3531 3133 3138 3336 2031 3234 342e 3936  51131836 1244.96
-00006310: 3836 3731 3139 3739 3939 3820 4c20 3937  86711979998 L 97
-00006320: 362e 3130 3538 3736 3138 3030 3139 3720  6.1058761800197 
-00006330: 3132 3434 2e39 3638 3637 3131 3937 3939  1244.96867119799
-00006340: 3938 204c 2039 3931 2e39 3338 3435 3738  98 L 991.9384578
-00006350: 3430 3031 3936 2031 3236 302e 3830 3132  400196 1260.8012
-00006360: 3532 3835 3739 3939 3820 4c20 3939 312e  528579998 L 991.
-00006370: 3933 3834 3537 3834 3030 3139 3620 3133  9384578400196 13
-00006380: 3033 2e30 3231 3437 3036 3137 3939 3937  03.0214706179997
-00006390: 204c 2037 3639 2e31 3136 3835 3531 3133   L 769.116855113
-000063a0: 3138 3336 2031 3330 332e 3032 3134 3730  1836 1303.021470
-000063b0: 3631 3739 3939 3720 4c20 3736 392e 3131  6179997 L 769.11
-000063c0: 3638 3535 3131 3331 3833 3620 3132 3434  68551131836 1244
-000063d0: 2e39 3638 3637 3131 3937 3939 3938 204d  .9686711979998 M
-000063e0: 2039 3736 2e31 3035 3837 3631 3830 3031   976.10587618001
-000063f0: 3937 2031 3234 342e 3936 3836 3731 3139  97 1244.96867119
-00006400: 3739 3939 3820 4c20 3937 362e 3130 3538  79998 L 976.1058
-00006410: 3736 3138 3030 3139 3720 3132 3630 2e38  761800197 1260.8
-00006420: 3031 3235 3238 3537 3939 3938 204c 2039  012528579998 L 9
-00006430: 3931 2e39 3338 3435 3738 3430 3031 3936  91.9384578400196
-00006440: 2031 3236 302e 3830 3132 3532 3835 3739   1260.8012528579
-00006450: 3939 3822 2073 7472 6f6b 652d 6d69 7465  998" stroke-mite
-00006460: 726c 696d 6974 3d22 3130 2220 7374 726f  rlimit="10" stro
-00006470: 6b65 2d77 6964 7468 3d22 312e 3436 3539  ke-width="1.4659
-00006480: 3739 3738 3333 3333 3333 3332 2220 7374  797833333332" st
-00006490: 726f 6b65 2d64 6173 6861 7272 6179 3d22  roke-dasharray="
-000064a0: 222f 3e3c 673e 3c74 6578 7420 6669 6c6c  "/><g><text fill
-000064b0: 3d22 626c 6163 6b22 2073 7472 6f6b 653d  ="black" stroke=
-000064c0: 226e 6f6e 6522 2066 6f6e 742d 6661 6d69  "none" font-fami
-000064d0: 6c79 3d22 7361 6e73 2d73 6572 6966 2220  ly="sans-serif" 
-000064e0: 666f 6e74 2d73 697a 653d 2231 3170 7422  font-size="11pt"
-000064f0: 2066 6f6e 742d 7374 796c 653d 226e 6f72   font-style="nor
-00006500: 6d61 6c22 2066 6f6e 742d 7765 6967 6874  mal" font-weight
-00006510: 3d22 6e6f 726d 616c 2220 7465 7874 2d64  ="normal" text-d
-00006520: 6563 6f72 6174 696f 6e3d 226e 6f72 6d61  ecoration="norma
-00006530: 6c22 2078 3d22 3739 332e 3734 3533 3135  l" x="793.745315
-00006540: 3437 3331 3833 3622 2079 3d22 3132 3639  4731836" y="1269
-00006550: 2e35 3937 3133 3135 3537 3939 3935 2220  .5971315579995" 
-00006560: 7465 7874 2d61 6e63 686f 723d 2273 7461  text-anchor="sta
-00006570: 7274 2220 646f 6d69 6e61 6e74 2d62 6173  rt" dominant-bas
-00006580: 656c 696e 653d 2261 6c70 6861 6265 7469  eline="alphabeti
-00006590: 6322 2078 6d6c 3a73 7061 6365 3d22 7072  c" xml:space="pr
-000065a0: 6573 6572 7665 223e 466f 726d 6174 c2a0  eserve">Format..
-000065b0: 6669 656c 64c2 a076 616c 7565 c2a0 696e  field..value..in
-000065c0: 746f c2a0 613c 2f74 6578 743e 3c74 6578  to..a</text><tex
-000065d0: 7420 6669 6c6c 3d22 626c 6163 6b22 2073  t fill="black" s
-000065e0: 7472 6f6b 653d 226e 6f6e 6522 2066 6f6e  troke="none" fon
-000065f0: 742d 6661 6d69 6c79 3d22 7361 6e73 2d73  t-family="sans-s
-00006600: 6572 6966 2220 666f 6e74 2d73 697a 653d  erif" font-size=
-00006610: 2231 3170 7422 2066 6f6e 742d 7374 796c  "11pt" font-styl
-00006620: 653d 226e 6f72 6d61 6c22 2066 6f6e 742d  e="normal" font-
-00006630: 7765 6967 6874 3d22 6e6f 726d 616c 2220  weight="normal" 
-00006640: 7465 7874 2d64 6563 6f72 6174 696f 6e3d  text-decoration=
-00006650: 226e 6f72 6d61 6c22 2078 3d22 3739 332e  "normal" x="793.
-00006660: 3734 3533 3135 3437 3331 3833 3622 2079  7453154731836" y
-00006670: 3d22 3132 3837 2e31 3838 3838 3839 3537  ="1287.188888957
-00006680: 3939 3936 2220 7465 7874 2d61 6e63 686f  9996" text-ancho
-00006690: 723d 2273 7461 7274 2220 646f 6d69 6e61  r="start" domina
-000066a0: 6e74 2d62 6173 656c 696e 653d 2261 6c70  nt-baseline="alp
-000066b0: 6861 6265 7469 6322 2078 6d6c 3a73 7061  habetic" xml:spa
-000066c0: 6365 3d22 7072 6573 6572 7665 223e 7374  ce="preserve">st
-000066d0: 7269 6e67 c2a0 6f72 c2a0 7661 6c75 65c2  ring..or..value.
-000066e0: a061 73c2 a072 6571 7569 7265 642e 3c2f  .as..required.</
-000066f0: 7465 7874 3e3c 2f67 3e3c 673e 3c67 3e3c  text></g><g><g><
-00006700: 7265 6374 2066 696c 6c3d 2272 6762 2832  rect fill="rgb(2
-00006710: 3034 2c32 3330 2c32 3034 2922 2073 7472  04,230,204)" str
-00006720: 6f6b 653d 226e 6f6e 6522 2078 3d22 3730  oke="none" x="70
-00006730: 342e 3837 3835 3438 3537 3037 3638 3322  4.8785485707683"
-00006740: 2079 3d22 3133 3239 2e34 3039 3130 3637   y="1329.4091067
-00006750: 3137 3939 3937 2220 7769 6474 683d 2238  179997" width="8
-00006760: 342e 3435 3433 3436 3036 3736 3536 3235  4.45434606765625
-00006770: 2220 6865 6967 6874 3d22 3232 2e38 3639  " height="22.869
-00006780: 3238 3436 3222 2f3e 3c2f 673e 3c74 6578  28462"/></g><tex
-00006790: 7420 6669 6c6c 3d22 626c 6163 6b22 2073  t fill="black" s
-000067a0: 7472 6f6b 653d 226e 6f6e 6522 2066 6f6e  troke="none" fon
-000067b0: 742d 6661 6d69 6c79 3d22 6d6f 6e6f 7370  t-family="monosp
-000067c0: 6163 6522 2066 6f6e 742d 7369 7a65 3d22  ace" font-size="
-000067d0: 3131 7074 2220 666f 6e74 2d73 7479 6c65  11pt" font-style
-000067e0: 3d22 6e6f 726d 616c 2220 666f 6e74 2d77  ="normal" font-w
-000067f0: 6569 6768 743d 226e 6f72 6d61 6c22 2074  eight="normal" t
-00006800: 6578 742d 6465 636f 7261 7469 6f6e 3d22  ext-decoration="
-00006810: 6e6f 726d 616c 2220 783d 2237 3037 2e35  normal" x="707.5
-00006820: 3137 3331 3231 3830 3736 3833 2220 793d  173121807683" y=
-00006830: 2231 3334 352e 3234 3136 3838 3337 3739  "1345.2416883779
-00006840: 3939 3722 2074 6578 742d 616e 6368 6f72  997" text-anchor
-00006850: 3d22 7374 6172 7422 2064 6f6d 696e 616e  ="start" dominan
-00006860: 742d 6261 7365 6c69 6e65 3d22 616c 7068  t-baseline="alph
-00006870: 6162 6574 6963 2220 786d 6c3a 7370 6163  abetic" xml:spac
-00006880: 653d 2270 7265 7365 7276 6522 3e26 6c74  e="preserve">&lt
-00006890: 3b26 6c74 3b76 616c 7565 2667 743b 2667  ;&lt;value&gt;&g
-000068a0: 743b 3c2f 7465 7874 3e3c 2f67 3e3c 673e  t;</text></g><g>
-000068b0: 3c70 6174 6820 6669 6c6c 3d22 6e6f 6e65  <path fill="none
-000068c0: 2220 7374 726f 6b65 3d22 626c 6163 6b22  " stroke="black"
-000068d0: 2070 6169 6e74 2d6f 7264 6572 3d22 6669   paint-order="fi
-000068e0: 6c6c 2073 7472 6f6b 6520 6d61 726b 6572  ll stroke marker
-000068f0: 7322 2064 3d22 204d 2038 3731 2e37 3331  s" d=" M 871.731
-00006900: 3737 3737 3736 3630 3136 2031 3335 322e  7777766016 1352.
-00006910: 3237 3833 3931 3333 3739 3939 3720 4c20  2783913379997 L 
-00006920: 3633 362e 3936 3335 3435 3639 3139 3234  636.963545691924
-00006930: 3520 3133 3532 2e32 3738 3339 3133 3337  5 1352.278391337
-00006940: 3939 3937 2220 7374 726f 6b65 2d6d 6974  9997" stroke-mit
-00006950: 6572 6c69 6d69 743d 2231 3022 2073 7472  erlimit="10" str
-00006960: 6f6b 652d 7769 6474 683d 2231 2e34 3635  oke-width="1.465
-00006970: 3937 3937 3833 3333 3333 3333 3222 2073  9797833333332" s
-00006980: 7472 6f6b 652d 6461 7368 6172 7261 793d  troke-dasharray=
-00006990: 2237 2e30 3336 3730 3239 3539 3939 3939  "7.0367029599999
-000069a0: 3939 3522 2f3e 3c67 2074 7261 6e73 666f  995"/><g transfo
-000069b0: 726d 3d22 7472 616e 736c 6174 6528 3632  rm="translate(62
-000069c0: 322e 3437 3936 3635 3433 3235 3931 322c  2.4796654325912,
-000069d0: 3133 3532 2e32 3738 3339 3133 3337 3939  1352.27839133799
-000069e0: 3937 2920 7472 616e 736c 6174 6528 2d36  97) translate(-6
-000069f0: 3232 2e34 3739 3636 3534 3332 3539 3132  22.4796654325912
-00006a00: 2c2d 3133 3532 2e32 3738 3339 3133 3337  ,-1352.278391337
-00006a10: 3939 3937 2922 3e3c 7061 7468 2066 696c  9997)"><path fil
-00006a20: 6c3d 2262 6c61 636b 2220 7374 726f 6b65  l="black" stroke
-00006a30: 3d22 6e6f 6e65 2220 7061 696e 742d 6f72  ="none" paint-or
-00006a40: 6465 723d 2273 7472 6f6b 6520 6669 6c6c  der="stroke fill
-00006a50: 206d 6172 6b65 7273 2220 643d 2220 4d20   markers" d=" M 
-00006a60: 3633 372e 3133 3934 3633 3236 3539 3234  637.139463265924
-00006a70: 3520 3133 3434 2e39 3438 3439 3234 3231  5 1344.948492421
-00006a80: 3333 3320 4c20 3632 322e 3437 3936 3635  333 L 622.479665
-00006a90: 3433 3235 3931 3220 3133 3532 2e32 3738  4325912 1352.278
-00006aa0: 3339 3133 3337 3939 3937 204c 2036 3337  3913379997 L 637
-00006ab0: 2e31 3339 3436 3332 3635 3932 3435 2031  .1394632659245 1
-00006ac0: 3335 392e 3630 3832 3930 3235 3436 3636  359.608290254666
-00006ad0: 3420 5a22 2f3e 3c2f 673e 3c2f 673e 3c67  4 Z"/></g></g><g
-00006ae0: 3e3c 673e 3c72 6563 7420 6669 6c6c 3d22  ><g><rect fill="
-00006af0: 7267 6228 3230 342c 3233 302c 3230 3429  rgb(204,230,204)
-00006b00: 2220 7374 726f 6b65 3d22 6e6f 6e65 2220  " stroke="none" 
-00006b10: 783d 2233 3730 2e35 3838 3031 3636 3730  x="370.588016670
-00006b20: 3337 3736 2220 793d 2231 3337 382e 3636  3776" y="1378.66
-00006b30: 3630 3237 3433 3739 3939 3722 2077 6964  60274379997" wid
-00006b40: 7468 3d22 3834 2e34 3534 3334 3630 3637  th="84.454346067
-00006b50: 3635 3632 3522 2068 6569 6768 743d 2232  65625" height="2
-00006b60: 322e 3836 3932 3834 3632 222f 3e3c 2f67  2.86928462"/></g
-00006b70: 3e3c 7465 7874 2066 696c 6c3d 2262 6c61  ><text fill="bla
-00006b80: 636b 2220 7374 726f 6b65 3d22 6e6f 6e65  ck" stroke="none
-00006b90: 2220 666f 6e74 2d66 616d 696c 793d 226d  " font-family="m
-00006ba0: 6f6e 6f73 7061 6365 2220 666f 6e74 2d73  onospace" font-s
-00006bb0: 697a 653d 2231 3170 7422 2066 6f6e 742d  ize="11pt" font-
-00006bc0: 7374 796c 653d 226e 6f72 6d61 6c22 2066  style="normal" f
-00006bd0: 6f6e 742d 7765 6967 6874 3d22 6e6f 726d  ont-weight="norm
-00006be0: 616c 2220 7465 7874 2d64 6563 6f72 6174  al" text-decorat
-00006bf0: 696f 6e3d 226e 6f72 6d61 6c22 2078 3d22  ion="normal" x="
-00006c00: 3337 332e 3232 3637 3830 3238 3033 3737  373.226780280377
-00006c10: 3622 2079 3d22 3133 3934 2e34 3938 3630  6" y="1394.49860
-00006c20: 3930 3937 3939 3936 2220 7465 7874 2d61  90979996" text-a
-00006c30: 6e63 686f 723d 2273 7461 7274 2220 646f  nchor="start" do
-00006c40: 6d69 6e61 6e74 2d62 6173 656c 696e 653d  minant-baseline=
-00006c50: 2261 6c70 6861 6265 7469 6322 2078 6d6c  "alphabetic" xml
-00006c60: 3a73 7061 6365 3d22 7072 6573 6572 7665  :space="preserve
-00006c70: 223e 266c 743b 266c 743b 7661 6c75 6526  ">&lt;&lt;value&
-00006c80: 6774 3b26 6774 3b3c 2f74 6578 743e 3c2f  gt;&gt;</text></
-00006c90: 673e 3c67 3e3c 7061 7468 2066 696c 6c3d  g><g><path fill=
-00006ca0: 226e 6f6e 6522 2073 7472 6f6b 653d 2262  "none" stroke="b
-00006cb0: 6c61 636b 2220 7061 696e 742d 6f72 6465  lack" paint-orde
-00006cc0: 723d 2266 696c 6c20 7374 726f 6b65 206d  r="fill stroke m
-00006cd0: 6172 6b65 7273 2220 643d 2220 4d20 3539  arkers" d=" M 59
-00006ce0: 362e 3039 3230 3239 3333 3235 3931 3220  6.0920293325912 
-00006cf0: 3134 3031 2e35 3335 3331 3230 3537 3939  1401.53531205799
-00006d00: 3936 204c 2032 3434 2e30 3232 3233 3033  96 L 244.0222303
-00006d10: 3335 3135 3336 3720 3134 3031 2e35 3335  3515367 1401.535
-00006d20: 3331 3230 3537 3939 3936 2220 7374 726f  3120579996" stro
-00006d30: 6b65 2d6d 6974 6572 6c69 6d69 743d 2231  ke-miterlimit="1
-00006d40: 3022 2073 7472 6f6b 652d 7769 6474 683d  0" stroke-width=
-00006d50: 2231 2e34 3635 3937 3937 3833 3333 3333  "1.4659797833333
-00006d60: 3333 3222 2073 7472 6f6b 652d 6461 7368  332" stroke-dash
-00006d70: 6172 7261 793d 2237 2e30 3336 3730 3239  array="7.0367029
-00006d80: 3539 3939 3939 3939 3522 2f3e 3c67 2074  599999995"/><g t
-00006d90: 7261 6e73 666f 726d 3d22 7472 616e 736c  ransform="transl
-00006da0: 6174 6528 3232 392e 3533 3833 3530 3037  ate(229.53835007
-00006db0: 3538 3230 3332 2c31 3430 312e 3533 3533  582032,1401.5353
-00006dc0: 3132 3035 3739 3939 3629 2074 7261 6e73  120579996) trans
-00006dd0: 6c61 7465 282d 3232 392e 3533 3833 3530  late(-229.538350
-00006de0: 3037 3538 3230 3332 2c2d 3134 3031 2e35  07582032,-1401.5
-00006df0: 3335 3331 3230 3537 3939 3936 2922 3e3c  353120579996)"><
-00006e00: 7061 7468 2066 696c 6c3d 2262 6c61 636b  path fill="black
-00006e10: 2220 7374 726f 6b65 3d22 6e6f 6e65 2220  " stroke="none" 
-00006e20: 7061 696e 742d 6f72 6465 723d 2273 7472  paint-order="str
-00006e30: 6f6b 6520 6669 6c6c 206d 6172 6b65 7273  oke fill markers
-00006e40: 2220 643d 2220 4d20 3234 342e 3139 3831  " d=" M 244.1981
-00006e50: 3437 3930 3931 3533 3635 2031 3339 342e  4790915365 1394.
-00006e60: 3230 3534 3133 3134 3133 3332 3920 4c20  2054131413329 L 
-00006e70: 3232 392e 3533 3833 3530 3037 3538 3230  229.538350075820
-00006e80: 3332 2031 3430 312e 3533 3533 3132 3035  32 1401.53531205
-00006e90: 3739 3939 3620 4c20 3234 342e 3139 3831  79996 L 244.1981
-00006ea0: 3437 3930 3931 3533 3635 2031 3430 382e  4790915365 1408.
-00006eb0: 3836 3532 3130 3937 3436 3636 3320 5a22  8652109746663 Z"
-00006ec0: 2f3e 3c2f 673e 3c2f 673e 3c67 3e3c 673e  /></g></g><g><g>
-00006ed0: 3c72 6563 7420 6669 6c6c 3d22 7267 6228  <rect fill="rgb(
-00006ee0: 3235 352c 3234 322c 3234 3529 2220 7374  255,242,245)" st
-00006ef0: 726f 6b65 3d22 6e6f 6e65 2220 783d 2235  roke="none" x="5
-00006f00: 3831 2e37 3035 3832 3137 3832 3239 3522  81.705821782295"
-00006f10: 2079 3d22 3134 3534 2e33 3130 3538 3432   y="1454.3105842
-00006f20: 3537 3939 3936 2220 7769 6474 683d 2237  579996" width="7
-00006f30: 352e 3635 3639 3231 3735 3132 3522 2068  5.65692175125" h
-00006f40: 6569 6768 743d 2232 322e 3836 3932 3834  eight="22.869284
-00006f50: 3632 222f 3e3c 2f67 3e3c 7465 7874 2066  62"/></g><text f
-00006f60: 696c 6c3d 2262 6c61 636b 2220 7374 726f  ill="black" stro
-00006f70: 6b65 3d22 6e6f 6e65 2220 666f 6e74 2d66  ke="none" font-f
-00006f80: 616d 696c 793d 226d 6f6e 6f73 7061 6365  amily="monospace
-00006f90: 2220 666f 6e74 2d73 697a 653d 2231 3170  " font-size="11p
-00006fa0: 7422 2066 6f6e 742d 7374 796c 653d 226e  t" font-style="n
-00006fb0: 6f72 6d61 6c22 2066 6f6e 742d 7765 6967  ormal" font-weig
-00006fc0: 6874 3d22 6e6f 726d 616c 2220 7465 7874  ht="normal" text
-00006fd0: 2d64 6563 6f72 6174 696f 6e3d 226e 6f72  -decoration="nor
-00006fe0: 6d61 6c22 2078 3d22 3538 342e 3334 3435  mal" x="584.3445
-00006ff0: 3835 3339 3232 3934 3922 2079 3d22 3134  853922949" y="14
-00007000: 3730 2e31 3433 3136 3539 3137 3939 3936  70.1431659179996
-00007010: 2220 7465 7874 2d61 6e63 686f 723d 2273  " text-anchor="s
-00007020: 7461 7274 2220 646f 6d69 6e61 6e74 2d62  tart" dominant-b
-00007030: 6173 656c 696e 653d 2261 6c70 6861 6265  aseline="alphabe
-00007040: 7469 6322 2078 6d6c 3a73 7061 6365 3d22  tic" xml:space="
-00007050: 7072 6573 6572 7665 223e 6170 7065 6e64  preserve">append
-00007060: 2829 3c2f 7465 7874 3e3c 2f67 3e3c 673e  ()</text></g><g>
-00007070: 3c70 6174 6820 6669 6c6c 3d22 6e6f 6e65  <path fill="none
-00007080: 2220 7374 726f 6b65 3d22 626c 6163 6b22  " stroke="black"
-00007090: 2070 6169 6e74 2d6f 7264 6572 3d22 6669   paint-order="fi
-000070a0: 6c6c 2073 7472 6f6b 6520 6d61 726b 6572  ll stroke marker
-000070b0: 7322 2064 3d22 204d 2032 3131 2e39 3436  s" d=" M 211.946
-000070c0: 3539 3236 3735 3832 3033 2031 3437 372e  5926758203 1477.
-000070d0: 3137 3938 3638 3837 3739 3939 3520 4c20  1798688779995 L 
-000070e0: 3130 3132 2e36 3338 3039 3233 3830 3638  1012.63809238068
-000070f0: 3632 2031 3437 372e 3137 3938 3638 3837  62 1477.17986887
-00007100: 3739 3939 3522 2073 7472 6f6b 652d 6d69  79995" stroke-mi
-00007110: 7465 726c 696d 6974 3d22 3130 2220 7374  terlimit="10" st
-00007120: 726f 6b65 2d77 6964 7468 3d22 312e 3436  roke-width="1.46
-00007130: 3539 3739 3738 3333 3333 3333 3332 2220  59797833333332" 
-00007140: 7374 726f 6b65 2d64 6173 6861 7272 6179  stroke-dasharray
-00007150: 3d22 222f 3e3c 6720 7472 616e 7366 6f72  =""/><g transfor
-00007160: 6d3d 2274 7261 6e73 6c61 7465 2831 3032  m="translate(102
-00007170: 372e 3132 3139 3732 3634 3030 3139 352c  7.1219726400195,
-00007180: 3134 3737 2e31 3739 3836 3838 3737 3939  1477.17986887799
-00007190: 3935 2920 7472 616e 736c 6174 6528 2d31  95) translate(-1
-000071a0: 3032 372e 3132 3139 3732 3634 3030 3139  027.121972640019
-000071b0: 352c 2d31 3437 372e 3137 3938 3638 3837  5,-1477.17986887
-000071c0: 3739 3939 3529 223e 3c70 6174 6820 6669  79995)"><path fi
-000071d0: 6c6c 3d22 626c 6163 6b22 2073 7472 6f6b  ll="black" strok
-000071e0: 653d 226e 6f6e 6522 2070 6169 6e74 2d6f  e="none" paint-o
-000071f0: 7264 6572 3d22 7374 726f 6b65 2066 696c  rder="stroke fil
-00007200: 6c20 6d61 726b 6572 7322 2064 3d22 204d  l markers" d=" M
-00007210: 2031 3031 322e 3436 3231 3734 3830 3636   1012.4621748066
-00007220: 3836 3220 3134 3639 2e38 3439 3936 3939  862 1469.8499699
-00007230: 3631 3333 3238 204c 2031 3032 372e 3132  613328 L 1027.12
-00007240: 3139 3732 3634 3030 3139 3520 3134 3737  19726400195 1477
-00007250: 2e31 3739 3836 3838 3737 3939 3935 204c  .1798688779995 L
-00007260: 2031 3031 322e 3436 3231 3734 3830 3636   1012.4621748066
-00007270: 3836 3220 3134 3834 2e35 3039 3736 3737  862 1484.5097677
-00007280: 3934 3636 3632 205a 222f 3e3c 2f67 3e3c  946662 Z"/></g><
-00007290: 2f67 3e3c 673e 3c67 3e3c 7265 6374 2066  /g><g><g><rect f
-000072a0: 696c 6c3d 2277 6869 7465 2220 7374 726f  ill="white" stro
-000072b0: 6b65 3d22 6e6f 6e65 2220 783d 2232 3332  ke="none" x="232
-000072c0: 2e37 3633 3530 3535 3939 3135 3336 3322  .76350559915363"
-000072d0: 2079 3d22 3135 3239 2e39 3535 3134 3130   y="1529.9551410
-000072e0: 3737 3939 3935 2220 7769 6474 683d 2231  779995" width="1
-000072f0: 3032 2e30 3439 3139 3437 3030 3436 3837  02.0491947004687
-00007300: 3522 2068 6569 6768 743d 2232 322e 3836  5" height="22.86
-00007310: 3932 3834 3632 222f 3e3c 2f67 3e3c 7465  928462"/></g><te
-00007320: 7874 2066 696c 6c3d 2262 6c61 636b 2220  xt fill="black" 
-00007330: 7374 726f 6b65 3d22 6e6f 6e65 2220 666f  stroke="none" fo
-00007340: 6e74 2d66 616d 696c 793d 226d 6f6e 6f73  nt-family="monos
-00007350: 7061 6365 2220 666f 6e74 2d73 697a 653d  pace" font-size=
-00007360: 2231 3170 7422 2066 6f6e 742d 7374 796c  "11pt" font-styl
-00007370: 653d 226e 6f72 6d61 6c22 2066 6f6e 742d  e="normal" font-
-00007380: 7765 6967 6874 3d22 6e6f 726d 616c 2220  weight="normal" 
-00007390: 7465 7874 2d64 6563 6f72 6174 696f 6e3d  text-decoration=
-000073a0: 226e 6f72 6d61 6c22 2078 3d22 3233 352e  "normal" x="235.
-000073b0: 3430 3232 3639 3230 3931 3533 3634 2220  40226920915364" 
-000073c0: 793d 2231 3534 352e 3738 3737 3232 3733  y="1545.78772273
-000073d0: 3739 3939 3522 2074 6578 742d 616e 6368  79995" text-anch
-000073e0: 6f72 3d22 7374 6172 7422 2064 6f6d 696e  or="start" domin
-000073f0: 616e 742d 6261 7365 6c69 6e65 3d22 616c  ant-baseline="al
-00007400: 7068 6162 6574 6963 2220 786d 6c3a 7370  phabetic" xml:sp
-00007410: 6163 653d 2270 7265 7365 7276 6522 3e26  ace="preserve">&
-00007420: 6c74 3b26 6c74 3b44 6174 6173 6574 2667  lt;&lt;Dataset&g
-00007430: 743b 2667 743b 3c2f 7465 7874 3e3c 2f67  t;&gt;</text></g
-00007440: 3e3c 673e 3c70 6174 6820 6669 6c6c 3d22  ><g><path fill="
-00007450: 6e6f 6e65 2220 7374 726f 6b65 3d22 626c  none" stroke="bl
-00007460: 6163 6b22 2070 6169 6e74 2d6f 7264 6572  ack" paint-order
-00007470: 3d22 6669 6c6c 2073 7472 6f6b 6520 6d61  ="fill stroke ma
-00007480: 726b 6572 7322 2064 3d22 204d 2032 3131  rkers" d=" M 211
-00007490: 2e39 3436 3539 3236 3735 3832 3033 2031  .9465926758203 1
-000074a0: 3535 322e 3832 3434 3235 3639 3739 3939  552.824425697999
-000074b0: 3720 4c20 3238 322e 3331 3336 3232 3237  7 L 282.31362227
-000074c0: 3538 3230 3320 3135 3532 2e38 3234 3432  58203 1552.82442
-000074d0: 3536 3937 3939 3937 204c 2032 3832 2e33  56979997 L 282.3
-000074e0: 3133 3632 3232 3735 3832 3033 2031 3537  136222758203 157
-000074f0: 352e 3639 3337 3130 3331 3739 3939 3620  5.6937103179996 
-00007500: 4c20 3231 372e 3633 3435 3934 3233 3531  L 217.6345942351
-00007510: 3533 3636 2031 3537 352e 3639 3337 3130  5366 1575.693710
-00007520: 3331 3739 3939 3622 2073 7472 6f6b 652d  3179996" stroke-
-00007530: 6d69 7465 726c 696d 6974 3d22 3130 2220  miterlimit="10" 
-00007540: 7374 726f 6b65 2d77 6964 7468 3d22 312e  stroke-width="1.
-00007550: 3436 3539 3739 3738 3333 3333 3333 3332  4659797833333332
-00007560: 2220 7374 726f 6b65 2d64 6173 6861 7272  " stroke-dasharr
-00007570: 6179 3d22 372e 3033 3637 3032 3935 3939  ay="7.0367029599
-00007580: 3939 3939 3935 222f 3e3c 6720 7472 616e  999995"/><g tran
-00007590: 7366 6f72 6d3d 2274 7261 6e73 6c61 7465  sform="translate
-000075a0: 2832 3033 2e31 3530 3731 3339 3735 3832  (203.15071397582
-000075b0: 3033 2c31 3537 352e 3639 3337 3130 3331  03,1575.69371031
-000075c0: 3739 3939 3629 2074 7261 6e73 6c61 7465  79996) translate
-000075d0: 282d 3230 332e 3135 3037 3133 3937 3538  (-203.1507139758
-000075e0: 3230 332c 2d31 3537 352e 3639 3337 3130  203,-1575.693710
-000075f0: 3331 3739 3939 3629 223e 3c70 6174 6820  3179996)"><path 
-00007600: 6669 6c6c 3d22 626c 6163 6b22 2073 7472  fill="black" str
-00007610: 6f6b 653d 226e 6f6e 6522 2070 6169 6e74  oke="none" paint
-00007620: 2d6f 7264 6572 3d22 7374 726f 6b65 2066  -order="stroke f
-00007630: 696c 6c20 6d61 726b 6572 7322 2064 3d22  ill markers" d="
-00007640: 204d 2032 3137 2e38 3130 3531 3138 3039   M 217.810511809
-00007650: 3135 3336 3420 3135 3638 2e33 3633 3831  15364 1568.36381
-00007660: 3134 3031 3333 3320 4c20 3230 332e 3135  1401333 L 203.15
-00007670: 3037 3133 3937 3538 3230 3320 3135 3735  07139758203 1575
-00007680: 2e36 3933 3731 3033 3137 3939 3936 204c  .6937103179996 L
-00007690: 2032 3137 2e38 3130 3531 3138 3039 3135   217.81051180915
-000076a0: 3336 3420 3135 3833 2e30 3233 3630 3932  364 1583.0236092
-000076b0: 3334 3636 3633 205a 222f 3e3c 2f67 3e3c  346663 Z"/></g><
-000076c0: 2f67 3e3c 673e 3c67 2f3e 3c70 6174 6820  /g><g><g/><path 
-000076d0: 6669 6c6c 3d22 6e6f 6e65 2220 7374 726f  fill="none" stro
-000076e0: 6b65 3d22 626c 6163 6b22 2070 6169 6e74  ke="black" paint
-000076f0: 2d6f 7264 6572 3d22 6669 6c6c 2073 7472  -order="fill str
-00007700: 6f6b 6520 6d61 726b 6572 7322 2064 3d22  oke markers" d="
-00007710: 204d 2039 372e 3630 3031 3639 3537 3538   M 97.6001695758
-00007720: 3230 3332 2036 3131 2e36 3635 3430 3437  2032 611.6654047
-00007730: 3937 3939 3939 204c 2031 3038 382e 3639  979999 L 1088.69
-00007740: 3331 3233 3534 3030 3139 3520 3631 312e  31235400195 611.
-00007750: 3636 3534 3034 3739 3739 3939 3920 4c20  6654047979999 L 
-00007760: 3130 3838 2e36 3933 3132 3335 3430 3031  1088.69312354001
-00007770: 3935 2031 3530 332e 3536 3735 3034 3937  95 1503.56750497
-00007780: 3739 3939 3520 4c20 3937 2e36 3030 3136  79995 L 97.60016
-00007790: 3935 3735 3832 3033 3220 3135 3033 2e35  957582032 1503.5
-000077a0: 3637 3530 3439 3737 3939 3935 204c 2039  675049779995 L 9
-000077b0: 372e 3630 3031 3639 3537 3538 3230 3332  7.60016957582032
-000077c0: 2036 3131 2e36 3635 3430 3437 3937 3939   611.66540479799
-000077d0: 3939 205a 2220 7374 726f 6b65 2d6d 6974  99 Z" stroke-mit
-000077e0: 6572 6c69 6d69 743d 2231 3022 2073 7472  erlimit="10" str
-000077f0: 6f6b 652d 7769 6474 683d 2232 2e35 3133  oke-width="2.513
-00007800: 3130 3832 2220 7374 726f 6b65 2d64 6173  1082" stroke-das
-00007810: 6861 7272 6179 3d22 222f 3e3c 7061 7468  harray=""/><path
-00007820: 2066 696c 6c3d 2270 696e 6b22 2073 7472   fill="pink" str
-00007830: 6f6b 653d 2262 6c61 636b 2220 7061 696e  oke="black" pain
-00007840: 742d 6f72 6465 723d 2266 696c 6c20 7374  t-order="fill st
-00007850: 726f 6b65 206d 6172 6b65 7273 2220 643d  roke markers" d=
-00007860: 2220 4d20 3937 2e36 3030 3136 3935 3735  " M 97.600169575
-00007870: 3832 3033 3220 3631 312e 3636 3534 3034  82032 611.665404
-00007880: 3739 3739 3939 3920 4c20 3937 2e36 3030  7979999 L 97.600
-00007890: 3136 3935 3735 3832 3033 3220 3633 322e  16957582032 632.
-000078a0: 3737 3535 3133 3637 3739 3939 3920 4c20  7755136779999 L 
-000078b0: 3135 372e 3533 3830 3738 3930 3730 3730  157.538078907070
-000078c0: 3331 2036 3332 2e37 3735 3531 3336 3737  31 632.775513677
-000078d0: 3939 3939 204c 2031 3638 2e30 3933 3133  9999 L 168.09313
-000078e0: 3333 3437 3037 3033 2036 3232 2e32 3230  33470703 622.220
-000078f0: 3435 3932 3338 204c 2031 3638 2e30 3933  459238 L 168.093
-00007900: 3133 3333 3437 3037 3033 2036 3131 2e36  1333470703 611.6
-00007910: 3635 3430 3437 3937 3939 3939 204c 2039  654047979999 L 9
-00007920: 372e 3630 3031 3639 3537 3538 3230 3332  7.60016957582032
-00007930: 2036 3131 2e36 3635 3430 3437 3937 3939   611.66540479799
-00007940: 3939 2220 7374 726f 6b65 2d6d 6974 6572  99" stroke-miter
-00007950: 6c69 6d69 743d 2231 3022 2073 7472 6f6b  limit="10" strok
-00007960: 652d 7769 6474 683d 2232 2e35 3133 3130  e-width="2.51310
-00007970: 3832 2220 7374 726f 6b65 2d64 6173 6861  82" stroke-dasha
-00007980: 7272 6179 3d22 222f 3e3c 7465 7874 2066  rray=""/><text f
-00007990: 696c 6c3d 2262 6c61 636b 2220 7374 726f  ill="black" stro
-000079a0: 6b65 3d22 6e6f 6e65 2220 666f 6e74 2d66  ke="none" font-f
-000079b0: 616d 696c 793d 2273 616e 732d 7365 7269  amily="sans-seri
-000079c0: 6622 2066 6f6e 742d 7369 7a65 3d22 382e  f" font-size="8.
-000079d0: 3870 7422 2066 6f6e 742d 7374 796c 653d  8pt" font-style=
-000079e0: 226e 6f72 6d61 6c22 2066 6f6e 742d 7765  "normal" font-we
-000079f0: 6967 6874 3d22 626f 6c64 2220 7465 7874  ight="bold" text
-00007a00: 2d64 6563 6f72 6174 696f 6e3d 226e 6f72  -decoration="nor
-00007a10: 6d61 6c22 2078 3d22 3131 352e 3139 3139  mal" x="115.1919
-00007a20: 3236 3937 3538 3230 3331 2220 793d 2236  2697582031" y="6
-00007a30: 3235 2e37 3338 3831 3037 3138 2220 7465  25.738810718" te
-00007a40: 7874 2d61 6e63 686f 723d 2273 7461 7274  xt-anchor="start
-00007a50: 2220 646f 6d69 6e61 6e74 2d62 6173 656c  " dominant-basel
-00007a60: 696e 653d 2261 6c70 6861 6265 7469 6322  ine="alphabetic"
-00007a70: 2078 6d6c 3a73 7061 6365 3d22 7072 6573   xml:space="pres
-00007a80: 6572 7665 223e 6c6f 6f70 3c2f 7465 7874  erve">loop</text
-00007a90: 3e3c 673e 3c72 6563 7420 6669 6c6c 3d22  ><g><rect fill="
-00007aa0: 7267 6228 3235 352c 3234 322c 3234 3529  rgb(255,242,245)
-00007ab0: 2220 7374 726f 6b65 3d22 6e6f 6e65 2220  " stroke="none" 
-00007ac0: 783d 2231 3833 2e30 3436 3132 3731 3337  x="183.046127137
-00007ad0: 3037 3033 2220 793d 2236 3133 2e30 3732  0703" y="613.072
-00007ae0: 3734 3533 3922 2077 6964 7468 3d22 3133  74539" width="13
-00007af0: 312e 3733 3537 3138 3133 3739 3638 3735  1.73571813796875
-00007b00: 2220 6865 6967 6874 3d22 3138 2e32 3935  " height="18.295
-00007b10: 3432 3736 3936 222f 3e3c 2f67 3e3c 7465  427696"/></g><te
-00007b20: 7874 2066 696c 6c3d 2262 6c61 636b 2220  xt fill="black" 
-00007b30: 7374 726f 6b65 3d22 6e6f 6e65 2220 666f  stroke="none" fo
-00007b40: 6e74 2d66 616d 696c 793d 2273 616e 732d  nt-family="sans-
-00007b50: 7365 7269 6622 2066 6f6e 742d 7369 7a65  serif" font-size
-00007b60: 3d22 382e 3870 7422 2066 6f6e 742d 7374  ="8.8pt" font-st
-00007b70: 796c 653d 226e 6f72 6d61 6c22 2066 6f6e  yle="normal" fon
-00007b80: 742d 7765 6967 6874 3d22 626f 6c64 2220  t-weight="bold" 
-00007b90: 7465 7874 2d64 6563 6f72 6174 696f 6e3d  text-decoration=
-00007ba0: 226e 6f72 6d61 6c22 2078 3d22 3138 352e  "normal" x="185.
-00007bb0: 3638 3438 3930 3734 3730 3730 3322 2079  6848907470703" y
-00007bc0: 3d22 3632 352e 3733 3838 3130 3731 3822  ="625.738810718"
-00007bd0: 2074 6578 742d 616e 6368 6f72 3d22 7374   text-anchor="st
-00007be0: 6172 7422 2064 6f6d 696e 616e 742d 6261  art" dominant-ba
-00007bf0: 7365 6c69 6e65 3d22 616c 7068 6162 6574  seline="alphabet
-00007c00: 6963 2220 786d 6c3a 7370 6163 653d 2270  ic" xml:space="p
-00007c10: 7265 7365 7276 6522 3e5b 6561 6368 c2a0  reserve">[each..
-00007c20: 726f 77c2 a069 6ec2 a051 7565 7279 7365  row..in..Queryse
-00007c30: 745d 3c2f 7465 7874 3e3c 2f67 3e3c 673e  t]</text></g><g>
-00007c40: 3c67 2f3e 3c70 6174 6820 6669 6c6c 3d22  <g/><path fill="
-00007c50: 6e6f 6e65 2220 7374 726f 6b65 3d22 626c  none" stroke="bl
-00007c60: 6163 6b22 2070 6169 6e74 2d6f 7264 6572  ack" paint-order
-00007c70: 3d22 6669 6c6c 2073 7472 6f6b 6520 6d61  ="fill stroke ma
-00007c80: 726b 6572 7322 2064 3d22 204d 2031 3135  rkers" d=" M 115
-00007c90: 2e31 3931 3932 3639 3735 3832 3033 3220  .19192697582032 
-00007ca0: 3733 312e 3238 3933 3535 3131 3739 3939  731.289355117999
-00007cb0: 3920 4c20 3130 3030 2e37 3334 3333 3635  9 L 1000.7343365
-00007cc0: 3430 3031 3935 2037 3331 2e32 3839 3335  400195 731.28935
-00007cd0: 3531 3137 3939 3939 204c 2031 3030 302e  51179999 L 1000.
-00007ce0: 3733 3433 3336 3534 3030 3139 3520 3134  7343365400195 14
-00007cf0: 3237 2e39 3232 3934 3831 3537 3939 3936  27.9229481579996
-00007d00: 204c 2031 3135 2e31 3931 3932 3639 3735   L 115.191926975
-00007d10: 3832 3033 3220 3134 3237 2e39 3232 3934  82032 1427.92294
-00007d20: 3831 3537 3939 3936 204c 2031 3135 2e31  81579996 L 115.1
-00007d30: 3931 3932 3639 3735 3832 3033 3220 3733  9192697582032 73
-00007d40: 312e 3238 3933 3535 3131 3739 3939 3920  1.2893551179999 
-00007d50: 5a22 2073 7472 6f6b 652d 6d69 7465 726c  Z" stroke-miterl
-00007d60: 696d 6974 3d22 3130 2220 7374 726f 6b65  imit="10" stroke
-00007d70: 2d77 6964 7468 3d22 322e 3531 3331 3038  -width="2.513108
-00007d80: 3222 2073 7472 6f6b 652d 6461 7368 6172  2" stroke-dashar
-00007d90: 7261 793d 2222 2f3e 3c70 6174 6820 6669  ray=""/><path fi
-00007da0: 6c6c 3d22 6772 6565 6e22 2073 7472 6f6b  ll="green" strok
-00007db0: 653d 2262 6c61 636b 2220 7061 696e 742d  e="black" paint-
-00007dc0: 6f72 6465 723d 2266 696c 6c20 7374 726f  order="fill stro
-00007dd0: 6b65 206d 6172 6b65 7273 2220 643d 2220  ke markers" d=" 
-00007de0: 4d20 3131 352e 3139 3139 3236 3937 3538  M 115.1919269758
-00007df0: 3230 3332 2037 3331 2e32 3839 3335 3531  2032 731.2893551
-00007e00: 3137 3939 3939 204c 2031 3135 2e31 3931  179999 L 115.191
-00007e10: 3932 3639 3735 3832 3033 3220 3735 322e  92697582032 752.
-00007e20: 3339 3934 3633 3939 3739 3939 3920 4c20  3994639979999 L 
-00007e30: 3137 352e 3132 3938 3336 3330 3730 3730  175.129836307070
-00007e40: 3332 2037 3532 2e33 3939 3436 3339 3937  32 752.399463997
-00007e50: 3939 3939 204c 2031 3835 2e36 3834 3839  9999 L 185.68489
-00007e60: 3037 3437 3037 3033 2037 3431 2e38 3434  07470703 741.844
-00007e70: 3430 3935 3537 3939 3939 204c 2031 3835  4095579999 L 185
-00007e80: 2e36 3834 3839 3037 3437 3037 3033 2037  .6848907470703 7
-00007e90: 3331 2e32 3839 3335 3531 3137 3939 3939  31.2893551179999
-00007ea0: 204c 2031 3135 2e31 3931 3932 3639 3735   L 115.191926975
-00007eb0: 3832 3033 3220 3733 312e 3238 3933 3535  82032 731.289355
-00007ec0: 3131 3739 3939 3922 2073 7472 6f6b 652d  1179999" stroke-
-00007ed0: 6d69 7465 726c 696d 6974 3d22 3130 2220  miterlimit="10" 
-00007ee0: 7374 726f 6b65 2d77 6964 7468 3d22 322e  stroke-width="2.
-00007ef0: 3531 3331 3038 3222 2073 7472 6f6b 652d  5131082" stroke-
-00007f00: 6461 7368 6172 7261 793d 2222 2f3e 3c74  dasharray=""/><t
-00007f10: 6578 7420 6669 6c6c 3d22 626c 6163 6b22  ext fill="black"
-00007f20: 2073 7472 6f6b 653d 226e 6f6e 6522 2066   stroke="none" f
-00007f30: 6f6e 742d 6661 6d69 6c79 3d22 7361 6e73  ont-family="sans
-00007f40: 2d73 6572 6966 2220 666f 6e74 2d73 697a  -serif" font-siz
-00007f50: 653d 2238 2e38 7074 2220 666f 6e74 2d73  e="8.8pt" font-s
-00007f60: 7479 6c65 3d22 6e6f 726d 616c 2220 666f  tyle="normal" fo
-00007f70: 6e74 2d77 6569 6768 743d 2262 6f6c 6422  nt-weight="bold"
-00007f80: 2074 6578 742d 6465 636f 7261 7469 6f6e   text-decoration
-00007f90: 3d22 6e6f 726d 616c 2220 783d 2231 3332  ="normal" x="132
-00007fa0: 2e37 3833 3638 3433 3735 3832 3033 3122  .78368437582031"
-00007fb0: 2079 3d22 3734 352e 3336 3237 3631 3033   y="745.36276103
-00007fc0: 3739 3939 3922 2074 6578 742d 616e 6368  79999" text-anch
-00007fd0: 6f72 3d22 7374 6172 7422 2064 6f6d 696e  or="start" domin
-00007fe0: 616e 742d 6261 7365 6c69 6e65 3d22 616c  ant-baseline="al
-00007ff0: 7068 6162 6574 6963 2220 786d 6c3a 7370  phabetic" xml:sp
-00008000: 6163 653d 2270 7265 7365 7276 6522 3e6c  ace="preserve">l
-00008010: 6f6f 703c 2f74 6578 743e 3c67 3e3c 7265  oop</text><g><re
-00008020: 6374 2066 696c 6c3d 2272 6762 2832 3034  ct fill="rgb(204
-00008030: 2c32 3330 2c32 3034 2922 2073 7472 6f6b  ,230,204)" strok
-00008040: 653d 226e 6f6e 6522 2078 3d22 3230 302e  e="none" x="200.
-00008050: 3633 3738 3834 3533 3730 3730 3322 2079  6378845370703" y
-00008060: 3d22 3733 322e 3639 3636 3935 3731 2220  ="732.69669571" 
-00008070: 7769 6474 683d 2231 3637 2e35 3637 3132  width="167.56712
-00008080: 3337 3737 3631 3731 3822 2068 6569 6768  377761718" heigh
-00008090: 743d 2231 382e 3239 3534 3237 3639 3622  t="18.295427696"
-000080a0: 2f3e 3c2f 673e 3c74 6578 7420 6669 6c6c  /></g><text fill
-000080b0: 3d22 626c 6163 6b22 2073 7472 6f6b 653d  ="black" stroke=
-000080c0: 226e 6f6e 6522 2066 6f6e 742d 6661 6d69  "none" font-fami
-000080d0: 6c79 3d22 7361 6e73 2d73 6572 6966 2220  ly="sans-serif" 
-000080e0: 666f 6e74 2d73 697a 653d 2238 2e38 7074  font-size="8.8pt
-000080f0: 2220 666f 6e74 2d73 7479 6c65 3d22 6e6f  " font-style="no
-00008100: 726d 616c 2220 666f 6e74 2d77 6569 6768  rmal" font-weigh
-00008110: 743d 2262 6f6c 6422 2074 6578 742d 6465  t="bold" text-de
-00008120: 636f 7261 7469 6f6e 3d22 6e6f 726d 616c  coration="normal
-00008130: 2220 783d 2232 3033 2e32 3736 3634 3831  " x="203.2766481
-00008140: 3437 3037 3033 3222 2079 3d22 3734 352e  4707032" y="745.
-00008150: 3336 3237 3631 3033 3739 3939 3922 2074  3627610379999" t
-00008160: 6578 742d 616e 6368 6f72 3d22 7374 6172  ext-anchor="star
-00008170: 7422 2064 6f6d 696e 616e 742d 6261 7365  t" dominant-base
-00008180: 6c69 6e65 3d22 616c 7068 6162 6574 6963  line="alphabetic
-00008190: 2220 786d 6c3a 7370 6163 653d 2270 7265  " xml:space="pre
-000081a0: 7365 7276 6522 3e5b 6561 6368 c2a0 6669  serve">[each..fi
-000081b0: 656c 64c2 a069 6ec2 a065 7870 6f72 74c2  eld..in..export.
-000081c0: a066 6965 6c64 c2a0 6c69 7374 5d3c 2f74  .field..list]</t
-000081d0: 6578 743e 3c2f 673e 3c2f 673e 3c67 2f3e  ext></g></g><g/>
-000081e0: 3c67 2f3e 3c67 2f3e 3c67 2f3e 3c2f 673e  <g/><g/><g/></g>
-000081f0: 3c2f 673e 3c2f 673e 3c2f 673e 3c2f 673e  </g></g></g></g>
-00008200: 3c2f 7376 673e                           </svg>
+00000080: 633e 2532 3325 3230 7365 6525 3230 696d  c>%23%20see%20im
+00000090: 706f 7274 5f77 6f72 6b66 6c6f 772e 7478  port_workflow.tx
+000000a0: 7425 3041 2530 4170 6172 7469 6369 7061  t%0A%0Aparticipa
+000000b0: 6e74 2532 3052 6573 6f75 7263 6525 3041  nt%20Resource%0A
+000000c0: 7061 7274 6963 6970 616e 7425 3230 4669  participant%20Fi
+000000d0: 656c 6425 3041 7061 7274 6963 6970 616e  eld%0Aparticipan
+000000e0: 7425 3230 5769 6467 6574 2530 4170 6172  t%20Widget%0Apar
+000000f0: 7469 6369 7061 6e74 2532 3074 6162 6c69  ticipant%20tabli
+00000100: 622e 4461 7461 7365 7425 3041 2530 4152  b.Dataset%0A%0AR
+00000110: 6573 6f75 7263 652d 2533 4552 6573 6f75  esource-%3EResou
+00000120: 7263 6525 3341 2532 3225 3232 6578 706f  rce%3A%22%22expo
+00000130: 7274 2871 7565 7279 7365 7425 3344 4e6f  rt(queryset%3DNo
+00000140: 6e65 2532 4325 3230 2535 432a 2535 432a  ne%2C%20%5C*%5C*
+00000150: 6b77 6172 6773 2925 3232 2532 3225 3041  kwargs)%22%22%0A
+00000160: 6163 7469 7661 7465 2532 3052 6573 6f75  activate%20Resou
+00000170: 7263 6525 3041 2530 4152 6573 6f75 7263  rce%0A%0AResourc
+00000180: 652d 2533 4552 6573 6f75 7263 6525 3341  e-%3EResource%3A
+00000190: 2533 4362 6163 6b67 726f 756e 6425 3341  %3Cbackground%3A
+000001a0: 2532 3379 656c 6c6f 7725 3345 2532 3225  %23yellow%3E%22%
+000001b0: 3232 6265 666f 7265 5f65 7870 6f72 7428  22before_export(
+000001c0: 7175 6572 7973 6574 2533 444e 6f6e 6525  queryset%3DNone%
+000001d0: 3243 2532 3025 3543 2a25 3543 2a6b 7761  2C%20%5C*%5C*kwa
+000001e0: 7267 7329 2532 3225 3232 2530 4125 3041  rgs)%22%22%0A%0A
+000001f0: 6e6f 7465 2532 306f 7665 7225 3230 5265  note%20over%20Re
+00000200: 736f 7572 6365 2533 4125 3230 4125 3230  source%3A%20A%20
+00000210: 5175 6572 7973 6574 2532 3069 6e73 7461  Queryset%20insta
+00000220: 6e63 6525 3230 6361 6e25 3230 6265 2532  nce%20can%20be%2
+00000230: 3070 6173 7365 6425 3230 696e 746f 2532  0passed%20into%2
+00000240: 3065 7870 6f72 7428 292e 2535 436e 4966  0export().%5CnIf
+00000250: 2532 306e 6f25 3230 5175 6572 7973 6574  %20no%20Queryset
+00000260: 2532 3069 7325 3230 7061 7373 6564 2532  %20is%20passed%2
+00000270: 4325 3230 6765 745f 7175 6572 7973 6574  C%20get_queryset
+00000280: 2829 2532 3069 7325 3230 6361 6c6c 6564  ()%20is%20called
+00000290: 2e25 3041 2530 4152 6573 6f75 7263 652d  .%0A%0AResource-
+000002a0: 2533 4552 6573 6f75 7263 6525 3341 2533  %3EResource%3A%3
+000002b0: 4362 6163 6b67 726f 756e 6425 3341 2532  Cbackground%3A%2
+000002c0: 3379 656c 6c6f 7725 3345 2532 3225 3232  3yellow%3E%22%22
+000002d0: 6765 745f 7175 6572 7973 6574 2829 2532  get_queryset()%2
+000002e0: 3225 3232 2530 4161 6374 6976 6174 6525  2%22%0Aactivate%
+000002f0: 3230 5265 736f 7572 6365 2532 3025 3233  20Resource%20%23
+00000300: 6c69 6768 7462 6c75 6525 3041 5265 736f  lightblue%0AReso
+00000310: 7572 6365 2533 432d 2d52 6573 6f75 7263  urce%3C--Resourc
+00000320: 6525 3341 2532 3225 3232 5175 6572 7973  e%3A%22%22Querys
+00000330: 6574 2532 3225 3232 2530 4164 6561 6374  et%22%22%0Adeact
+00000340: 6976 6174 6525 3230 5265 736f 7572 6365  ivate%20Resource
+00000350: 2530 4125 3041 5265 736f 7572 6365 2d25  %0A%0AResource-%
+00000360: 3345 5265 736f 7572 6365 2533 4125 3343  3EResource%3A%3C
+00000370: 6261 636b 6772 6f75 6e64 2533 4125 3233  background%3A%23
+00000380: 7965 6c6c 6f77 2533 4525 3232 2532 3266  yellow%3E%22%22f
+00000390: 696c 7465 725f 6578 706f 7274 2871 7565  ilter_export(que
+000003a0: 7279 7365 7425 3243 2532 3025 3543 2a25  ryset%2C%20%5C*%
+000003b0: 3543 2a6b 7761 7267 7329 2532 3225 3232  5C*kwargs)%22%22
+000003c0: 2530 4161 6374 6976 6174 6525 3230 5265  %0Aactivate%20Re
+000003d0: 736f 7572 6365 2532 3025 3233 6c69 6768  source%20%23ligh
+000003e0: 7462 6c75 6525 3041 5265 736f 7572 6365  tblue%0AResource
+000003f0: 2533 432d 2d52 6573 6f75 7263 6525 3341  %3C--Resource%3A
+00000400: 2532 3225 3232 5175 6572 7973 6574 2532  %22%22Queryset%2
+00000410: 3225 3232 2530 4164 6561 6374 6976 6174  2%22%0Adeactivat
+00000420: 6525 3230 5265 736f 7572 6365 2530 4125  e%20Resource%0A%
+00000430: 3041 6c6f 6f70 2532 3025 3233 7069 6e6b  0Aloop%20%23pink
+00000440: 2532 3065 6163 6825 3230 726f 7725 3230  %20each%20row%20
+00000450: 696e 2532 3051 7565 7279 7365 7425 3041  in%20Queryset%0A
+00000460: 2530 4152 6573 6f75 7263 652d 2533 4552  %0AResource-%3ER
+00000470: 6573 6f75 7263 6525 3341 2533 4362 6163  esource%3A%3Cbac
+00000480: 6b67 726f 756e 6425 3341 2532 3379 656c  kground%3A%23yel
+00000490: 6c6f 7725 3345 2532 3225 3232 6578 706f  low%3E%22%22expo
+000004a0: 7274 5f72 6573 6f75 7263 6528 696e 7374  rt_resource(inst
+000004b0: 616e 6365 2925 3232 2532 3225 3041 6163  ance)%22%22%0Aac
+000004c0: 7469 7661 7465 2532 3052 6573 6f75 7263  tivate%20Resourc
+000004d0: 6525 3230 2532 336c 6967 6874 626c 7565  e%20%23lightblue
+000004e0: 2530 4125 3041 6c6f 6f70 2532 3025 3233  %0A%0Aloop%20%23
+000004f0: 6772 6565 6e25 3230 6561 6368 2532 3066  green%20each%20f
+00000500: 6965 6c64 2532 3069 6e25 3230 6578 706f  ield%20in%20expo
+00000510: 7274 2532 3066 6965 6c64 2532 306c 6973  rt%20field%20lis
+00000520: 7425 3041 5265 736f 7572 6365 2d25 3345  t%0AResource-%3E
+00000530: 5265 736f 7572 6365 2533 4125 3232 2532  Resource%3A%22%2
+00000540: 3265 7870 6f72 745f 6669 656c 6428 6669  2export_field(fi
+00000550: 656c 6425 3243 2532 3069 6e73 7461 6e63  eld%2C%20instanc
+00000560: 6529 2532 3225 3232 2530 4161 6374 6976  e)%22%22%0Aactiv
+00000570: 6174 6525 3230 5265 736f 7572 6365 2532  ate%20Resource%2
+00000580: 3025 3233 6c69 6768 7470 696e 6b25 3041  0%23lightpink%0A
+00000590: 5265 736f 7572 6365 2d25 3345 4669 656c  Resource-%3EFiel
+000005a0: 6425 3341 2532 3225 3232 6578 706f 7274  d%3A%22%22export
+000005b0: 2869 6e73 7461 6e63 6529 2532 3225 3232  (instance)%22%22
+000005c0: 2530 4161 6374 6976 6174 6525 3230 4669  %0Aactivate%20Fi
+000005d0: 656c 6425 3230 2532 336c 6967 6874 626c  eld%20%23lightbl
+000005e0: 7565 2530 416e 6f74 6525 3230 6f76 6572  ue%0Anote%20over
+000005f0: 2532 3046 6965 6c64 2533 4125 3230 416e  %20Field%3A%20An
+00000600: 2532 306f 7074 696f 6e61 6c25 3230 6361  %20optional%20ca
+00000610: 6c6c 6162 6c65 2532 3063 616e 2532 3062  llable%20can%20b
+00000620: 6525 3230 6465 6669 6e65 6425 3230 696e  e%20defined%20in
+00000630: 7374 6561 6425 3230 6f66 2532 3065 7870  stead%20of%20exp
+00000640: 6f72 7428 292e 2535 436e 2532 3053 6565  ort().%5Cn%20See
+00000650: 2532 3027 6465 6879 6472 6174 6527 2532  %20'dehydrate'%2
+00000660: 306d 6574 686f 6473 2532 3069 6e25 3230  0methods%20in%20
+00000670: 646f 6373 2e25 3041 4669 656c 642d 2533  docs.%0AField-%3
+00000680: 4546 6965 6c64 2533 4125 3232 2532 3267  EField%3A%22%22g
+00000690: 6574 5f76 616c 7565 2869 6e73 7461 6e63  et_value(instanc
+000006a0: 6529 2532 3225 3232 2530 4161 6374 6976  e)%22%22%0Aactiv
+000006b0: 6174 6525 3230 4669 656c 6425 3230 2532  ate%20Field%20%2
+000006c0: 336c 6967 6874 7069 6e6b 2530 416e 6f74  3lightpink%0Anot
+000006d0: 6525 3230 6f76 6572 2532 3046 6965 6c64  e%20over%20Field
+000006e0: 2533 4125 3230 4765 7425 3230 7468 6525  %3A%20Get%20the%
+000006f0: 3230 6669 656c 6427 7325 3230 7661 6c75  20field's%20valu
+00000700: 6525 3230 6672 6f6d 2532 3074 6865 2532  e%20from%20the%2
+00000710: 3069 6e73 7461 6e63 652e 2530 4146 6965  0instance.%0AFie
+00000720: 6c64 2533 432d 2d46 6965 6c64 2533 4125  ld%3C--Field%3A%
+00000730: 3232 2532 3225 3343 2533 4376 616c 7565  22%22%3C%3Cvalue
+00000740: 2533 4525 3345 2532 3225 3232 2530 4146  %3E%3E%22%22%0AF
+00000750: 6965 6c64 2d25 3345 5769 6467 6574 2533  ield-%3EWidget%3
+00000760: 4125 3232 2532 3272 656e 6465 7228 7661  A%22%22render(va
+00000770: 6c75 6529 2532 3225 3232 2530 4161 6374  lue)%22%22%0Aact
+00000780: 6976 6174 6525 3230 5769 6467 6574 2530  ivate%20Widget%0
+00000790: 416e 6f74 6525 3230 6f76 6572 2532 3057  Anote%20over%20W
+000007a0: 6964 6765 7425 3341 2532 3046 6f72 6d61  idget%3A%20Forma
+000007b0: 7425 3230 6669 656c 6425 3230 7661 6c75  t%20field%20valu
+000007c0: 6525 3230 696e 746f 2532 3061 2535 436e  e%20into%20a%5Cn
+000007d0: 7374 7269 6e67 2532 306f 7225 3230 7661  string%20or%20va
+000007e0: 6c75 6525 3230 6173 2532 3072 6571 7569  lue%20as%20requi
+000007f0: 7265 642e 2530 4146 6965 6c64 2533 432d  red.%0AField%3C-
+00000800: 2d57 6964 6765 7425 3341 2532 3225 3232  -Widget%3A%22%22
+00000810: 2533 4325 3343 7661 6c75 6525 3345 2533  %3C%3Cvalue%3E%3
+00000820: 4525 3041 6465 6163 7469 7661 7465 2532  E%0Adeactivate%2
+00000830: 3057 6964 6765 7425 3041 6465 6163 7469  0Widget%0Adeacti
+00000840: 7661 7465 2532 3046 6965 6c64 2530 4152  vate%20Field%0AR
+00000850: 6573 6f75 7263 6525 3343 2d2d 4669 656c  esource%3C--Fiel
+00000860: 6425 3341 2532 3225 3232 2533 4325 3343  d%3A%22%22%3C%3C
+00000870: 7661 6c75 6525 3345 2533 4525 3232 2532  value%3E%3E%22%2
+00000880: 3225 3041 6465 6163 7469 7661 7465 2532  2%0Adeactivate%2
+00000890: 3046 6965 6c64 2530 4164 6561 6374 6976  0Field%0Adeactiv
+000008a0: 6174 6525 3230 5265 736f 7572 6365 2530  ate%20Resource%0
+000008b0: 4165 6e64 2530 4164 6561 6374 6976 6174  Aend%0Adeactivat
+000008c0: 6525 3230 5265 736f 7572 6365 2530 4125  e%20Resource%0A%
+000008d0: 3041 5265 736f 7572 6365 2d25 3345 7461  0AResource-%3Eta
+000008e0: 626c 6962 2e44 6174 6173 6574 2533 4125  blib.Dataset%3A%
+000008f0: 3232 2532 3261 7070 656e 6428 2925 3232  22%22append()%22
+00000900: 2532 3225 3041 656e 6425 3041 2530 4152  %22%0Aend%0A%0AR
+00000910: 6573 6f75 7263 6525 3343 2d2d 5265 736f  esource%3C--Reso
+00000920: 7572 6365 2533 4125 3232 2532 3225 3343  urce%3A%22%22%3C
+00000930: 2533 4344 6174 6173 6574 2533 4525 3345  %3CDataset%3E%3E
+00000940: 2532 3225 3232 2530 4164 6561 6374 6976  %22%22%0Adeactiv
+00000950: 6174 6525 3230 5265 736f 7572 6365 2530  ate%20Resource%0
+00000960: 4125 3041 2530 413c 2f64 6573 633e 3c64  A%0A%0A</desc><d
+00000970: 6566 732f 3e3c 673e 3c67 2f3e 3c67 2f3e  efs/><g><g/><g/>
+00000980: 3c67 2f3e 3c67 2f3e 3c67 2f3e 3c67 2f3e  <g/><g/><g/><g/>
+00000990: 3c67 2f3e 3c67 2f3e 3c67 2f3e 3c67 2f3e  <g/><g/><g/><g/>
+000009a0: 3c67 2f3e 3c67 2f3e 3c67 2f3e 3c67 2f3e  <g/><g/><g/><g/>
+000009b0: 3c67 2f3e 3c67 2f3e 3c67 2f3e 3c67 2f3e  <g/><g/><g/><g/>
+000009c0: 3c67 2f3e 3c67 2f3e 3c67 2f3e 3c67 2f3e  <g/><g/><g/><g/>
+000009d0: 3c67 2f3e 3c67 2f3e 3c67 2f3e 3c67 2f3e  <g/><g/><g/><g/>
+000009e0: 3c67 2f3e 3c67 2f3e 3c67 2f3e 3c67 2f3e  <g/><g/><g/><g/>
+000009f0: 3c67 2f3e 3c67 2f3e 3c67 2f3e 3c67 2f3e  <g/><g/><g/><g/>
+00000a00: 3c67 2f3e 3c67 2f3e 3c67 2f3e 3c67 2f3e  <g/><g/><g/><g/>
+00000a10: 3c67 2f3e 3c67 2f3e 3c67 2f3e 3c67 2f3e  <g/><g/><g/><g/>
+00000a20: 3c67 2f3e 3c67 2f3e 3c67 2f3e 3c67 2f3e  <g/><g/><g/><g/>
+00000a30: 3c67 2f3e 3c67 2f3e 3c67 2f3e 3c67 2f3e  <g/><g/><g/><g/>
+00000a40: 3c67 2f3e 3c67 2f3e 3c67 2f3e 3c67 2f3e  <g/><g/><g/><g/>
+00000a50: 3c67 2f3e 3c67 2f3e 3c67 2f3e 3c67 2f3e  <g/><g/><g/><g/>
+00000a60: 3c67 2f3e 3c67 2f3e 3c67 2f3e 3c67 2f3e  <g/><g/><g/><g/>
+00000a70: 3c67 2f3e 3c67 2f3e 3c67 2f3e 3c67 2f3e  <g/><g/><g/><g/>
+00000a80: 3c67 2f3e 3c67 2f3e 3c67 2f3e 3c67 2f3e  <g/><g/><g/><g/>
+00000a90: 3c67 2f3e 3c67 2f3e 3c67 2f3e 3c67 2f3e  <g/><g/><g/><g/>
+00000aa0: 3c67 2f3e 3c67 2f3e 3c67 2f3e 3c67 2f3e  <g/><g/><g/><g/>
+00000ab0: 3c67 2f3e 3c67 2f3e 3c67 2f3e 3c67 2f3e  <g/><g/><g/><g/>
+00000ac0: 3c67 2f3e 3c67 2f3e 3c67 2f3e 3c67 2f3e  <g/><g/><g/><g/>
+00000ad0: 3c67 2f3e 3c67 2f3e 3c67 2f3e 3c67 2f3e  <g/><g/><g/><g/>
+00000ae0: 3c67 2f3e 3c67 2f3e 3c67 2f3e 3c67 2f3e  <g/><g/><g/><g/>
+00000af0: 3c67 2f3e 3c67 2f3e 3c67 2f3e 3c67 2f3e  <g/><g/><g/><g/>
+00000b00: 3c67 2f3e 3c67 2f3e 3c67 2f3e 3c67 2f3e  <g/><g/><g/><g/>
+00000b10: 3c67 2f3e 3c67 2f3e 3c67 2f3e 3c67 2f3e  <g/><g/><g/><g/>
+00000b20: 3c67 2f3e 3c67 2f3e 3c67 2f3e 3c67 2f3e  <g/><g/><g/><g/>
+00000b30: 3c67 2f3e 3c67 2f3e 3c67 2f3e 3c67 2f3e  <g/><g/><g/><g/>
+00000b40: 3c67 2f3e 3c67 2f3e 3c67 2f3e 3c67 2f3e  <g/><g/><g/><g/>
+00000b50: 3c67 2f3e 3c67 2f3e 3c67 2f3e 3c67 2f3e  <g/><g/><g/><g/>
+00000b60: 3c67 2f3e 3c67 2f3e 3c67 2f3e 3c67 2f3e  <g/><g/><g/><g/>
+00000b70: 3c67 2f3e 3c67 2f3e 3c67 2f3e 3c67 2f3e  <g/><g/><g/><g/>
+00000b80: 3c67 2f3e 3c67 2f3e 3c67 2f3e 3c67 2f3e  <g/><g/><g/><g/>
+00000b90: 3c67 2f3e 3c67 2f3e 3c67 3e3c 7265 6374  <g/><g/><g><rect
+00000ba0: 2066 696c 6c3d 2277 6869 7465 2220 7374   fill="white" st
+00000bb0: 726f 6b65 3d22 6e6f 6e65 2220 783d 2230  roke="none" x="0
+00000bc0: 2220 793d 2230 2220 7769 6474 683d 2231  " y="0" width="1
+00000bd0: 3036 3822 2068 6569 6768 743d 2231 3633  068" height="163
+00000be0: 3722 2f3e 3c2f 673e 3c67 3e3c 7265 6374  7"/></g><g><rect
+00000bf0: 2066 696c 6c3d 2272 6762 2832 3535 2c32   fill="rgb(255,2
+00000c00: 3432 2c32 3435 2922 2073 7472 6f6b 653d  42,245)" stroke=
+00000c10: 226e 6f6e 6522 2078 3d22 3937 2e36 3030  "none" x="97.600
+00000c20: 3136 3139 3436 3432 3537 3922 2079 3d22  16194642579" y="
+00000c30: 3631 312e 3636 3534 3034 3739 3739 3939  611.665404797999
+00000c40: 3922 2077 6964 7468 3d22 3935 332e 3230  9" width="953.20
+00000c50: 3332 3630 3531 3431 3733 3222 2068 6569  32605141732" hei
+00000c60: 6768 743d 2238 3931 2e39 3032 3130 3031  ght="891.9021001
+00000c70: 3739 3939 3936 222f 3e3c 7265 6374 2066  799996"/><rect f
+00000c80: 696c 6c3d 2272 6762 2832 3034 2c32 3330  ill="rgb(204,230
+00000c90: 2c32 3034 2922 2073 7472 6f6b 653d 226e  ,204)" stroke="n
+00000ca0: 6f6e 6522 2078 3d22 3131 352e 3139 3139  one" x="115.1919
+00000cb0: 3139 3334 3634 3235 3739 2220 793d 2237  1934642579" y="7
+00000cc0: 3331 2e32 3839 3335 3531 3137 3939 3939  31.2893551179999
+00000cd0: 2220 7769 6474 683d 2238 3437 2e36 3532  " width="847.652
+00000ce0: 3731 3631 3134 3137 3331 2220 6865 6967  7161141731" heig
+00000cf0: 6874 3d22 3639 362e 3633 3335 3933 3033  ht="696.63359303
+00000d00: 3939 3939 3722 2f3e 3c2f 673e 3c67 3e3c  99997"/></g><g><
+00000d10: 7061 7468 2066 696c 6c3d 226e 6f6e 6522  path fill="none"
+00000d20: 2073 7472 6f6b 653d 2262 6c61 636b 2220   stroke="black" 
+00000d30: 7061 696e 742d 6f72 6465 723d 2266 696c  paint-order="fil
+00000d40: 6c20 7374 726f 6b65 206d 6172 6b65 7273  l stroke markers
+00000d50: 2220 643d 2220 4d20 3230 332e 3135 3037  " d=" M 203.1507
+00000d60: 3036 3334 3634 3235 3738 2035 392e 3238  0634642578 59.28
+00000d70: 3432 3232 3433 3739 3939 3938 3620 4c20  4222437999986 L 
+00000d80: 3230 332e 3135 3037 3036 3334 3634 3235  203.150706346425
+00000d90: 3738 2031 3633 372e 3236 3438 3631 3231  78 1637.26486121
+00000da0: 3739 3939 3622 2073 7472 6f6b 652d 6d69  79996" stroke-mi
+00000db0: 7465 726c 696d 6974 3d22 3130 2220 7374  terlimit="10" st
+00000dc0: 726f 6b65 2d77 6964 7468 3d22 312e 3436  roke-width="1.46
+00000dd0: 3539 3739 3738 3333 3333 3333 3332 2220  59797833333332" 
+00000de0: 7374 726f 6b65 2d64 6173 6861 7272 6179  stroke-dasharray
+00000df0: 3d22 3133 2e35 3332 3132 3130 3736 3932  ="13.53212107692
+00000e00: 3330 3736 2c35 2e38 3633 3931 3931 3333  3076,5.863919133
+00000e10: 3333 3333 3333 222f 3e3c 7061 7468 2066  333333"/><path f
+00000e20: 696c 6c3d 226e 6f6e 6522 2073 7472 6f6b  ill="none" strok
+00000e30: 653d 2262 6c61 636b 2220 7061 696e 742d  e="black" paint-
+00000e40: 6f72 6465 723d 2266 696c 6c20 7374 726f  order="fill stro
+00000e50: 6b65 206d 6172 6b65 7273 2220 643d 2220  ke markers" d=" 
+00000e60: 4d20 3630 352e 3937 3536 3638 3935 3738  M 605.9756689578
+00000e70: 3834 3220 3539 2e32 3834 3232 3234 3337  842 59.284222437
+00000e80: 3939 3939 3836 204c 2036 3035 2e39 3735  999986 L 605.975
+00000e90: 3636 3839 3537 3838 3432 2031 3633 372e  6689578842 1637.
+00000ea0: 3236 3438 3631 3231 3739 3939 3622 2073  2648612179996" s
+00000eb0: 7472 6f6b 652d 6d69 7465 726c 696d 6974  troke-miterlimit
+00000ec0: 3d22 3130 2220 7374 726f 6b65 2d77 6964  ="10" stroke-wid
+00000ed0: 7468 3d22 312e 3436 3539 3739 3738 3333  th="1.4659797833
+00000ee0: 3333 3333 3332 2220 7374 726f 6b65 2d64  333332" stroke-d
+00000ef0: 6173 6861 7272 6179 3d22 3133 2e35 3332  asharray="13.532
+00000f00: 3132 3130 3736 3932 3330 3736 2c35 2e38  121076923076,5.8
+00000f10: 3633 3931 3931 3333 3333 3333 3333 222f  63919133333333"/
+00000f20: 3e3c 7061 7468 2066 696c 6c3d 226e 6f6e  ><path fill="non
+00000f30: 6522 2073 7472 6f6b 653d 2262 6c61 636b  e" stroke="black
+00000f40: 2220 7061 696e 742d 6f72 6465 723d 2266  " paint-order="f
+00000f50: 696c 6c20 7374 726f 6b65 206d 6172 6b65  ill stroke marke
+00000f60: 7273 2220 643d 2220 4d20 3834 322e 3633  rs" d=" M 842.63
+00000f70: 3739 3535 3339 3731 3831 2035 392e 3238  7955397181 59.28
+00000f80: 3432 3232 3433 3739 3939 3938 3620 4c20  4222437999986 L 
+00000f90: 3834 322e 3633 3739 3535 3339 3731 3831  842.637955397181
+00000fa0: 2031 3633 372e 3236 3438 3631 3231 3739   1637.2648612179
+00000fb0: 3939 3622 2073 7472 6f6b 652d 6d69 7465  996" stroke-mite
+00000fc0: 726c 696d 6974 3d22 3130 2220 7374 726f  rlimit="10" stro
+00000fd0: 6b65 2d77 6964 7468 3d22 312e 3436 3539  ke-width="1.4659
+00000fe0: 3739 3738 3333 3333 3333 3332 2220 7374  797833333332" st
+00000ff0: 726f 6b65 2d64 6173 6861 7272 6179 3d22  roke-dasharray="
+00001000: 3133 2e35 3332 3132 3130 3736 3932 3330  13.5321210769230
+00001010: 3736 2c35 2e38 3633 3931 3931 3333 3333  76,5.86391913333
+00001020: 3333 3333 222f 3e3c 7061 7468 2066 696c  3333"/><path fil
+00001030: 6c3d 226e 6f6e 6522 2073 7472 6f6b 653d  l="none" stroke=
+00001040: 2262 6c61 636b 2220 7061 696e 742d 6f72  "black" paint-or
+00001050: 6465 723d 2266 696c 6c20 7374 726f 6b65  der="fill stroke
+00001060: 206d 6172 6b65 7273 2220 643d 2220 4d20   markers" d=" M 
+00001070: 3938 392e 3233 3232 3731 3536 3035 3939  989.232271560599
+00001080: 2035 392e 3238 3432 3232 3433 3739 3939   59.284222437999
+00001090: 3938 3620 4c20 3938 392e 3233 3232 3731  986 L 989.232271
+000010a0: 3536 3035 3939 2031 3633 372e 3236 3438  560599 1637.2648
+000010b0: 3631 3231 3739 3939 3622 2073 7472 6f6b  612179996" strok
+000010c0: 652d 6d69 7465 726c 696d 6974 3d22 3130  e-miterlimit="10
+000010d0: 2220 7374 726f 6b65 2d77 6964 7468 3d22  " stroke-width="
+000010e0: 312e 3436 3539 3739 3738 3333 3333 3333  1.46597978333333
+000010f0: 3332 2220 7374 726f 6b65 2d64 6173 6861  32" stroke-dasha
+00001100: 7272 6179 3d22 3133 2e35 3332 3132 3130  rray="13.5321210
+00001110: 3736 3932 3330 3736 2c35 2e38 3633 3931  76923076,5.86391
+00001120: 3931 3333 3333 3333 3333 222f 3e3c 2f67  9133333333"/></g
+00001130: 3e3c 673e 3c70 6174 6820 6669 6c6c 3d22  ><g><path fill="
+00001140: 6e6f 6e65 2220 7374 726f 6b65 3d22 6e6f  none" stroke="no
+00001150: 6e65 222f 3e3c 673e 3c70 6174 6820 6669  ne"/><g><path fi
+00001160: 6c6c 3d22 7768 6974 6522 2073 7472 6f6b  ll="white" strok
+00001170: 653d 2262 6c61 636b 2220 7061 696e 742d  e="black" paint-
+00001180: 6f72 6465 723d 2266 696c 6c20 7374 726f  order="fill stro
+00001190: 6b65 206d 6172 6b65 7273 2220 643d 2220  ke markers" d=" 
+000011a0: 4d20 3135 322e 3639 3238 3638 3632 3236  M 152.6928686226
+000011b0: 3031 3537 2031 312e 3738 3634 3737 3435  0157 11.78647745
+000011c0: 3739 3939 3939 3720 4c20 3235 332e 3630  7999997 L 253.60
+000011d0: 3835 3434 3037 3032 3520 3131 2e37 3836  854407025 11.786
+000011e0: 3437 3734 3537 3939 3939 3937 204c 2032  477457999997 L 2
+000011f0: 3533 2e36 3038 3534 3430 3730 3235 2035  53.60854407025 5
+00001200: 392e 3238 3432 3232 3433 3739 3939 3938  9.28422243799998
+00001210: 3620 4c20 3135 322e 3639 3238 3638 3632  6 L 152.69286862
+00001220: 3236 3031 3537 2035 392e 3238 3432 3232  260157 59.284222
+00001230: 3433 3739 3939 3938 3620 4c20 3135 322e  437999986 L 152.
+00001240: 3639 3238 3638 3632 3236 3031 3537 2031  69286862260157 1
+00001250: 312e 3738 3634 3737 3435 3739 3939 3939  1.78647745799999
+00001260: 3720 5a22 2073 7472 6f6b 652d 6d69 7465  7 Z" stroke-mite
+00001270: 726c 696d 6974 3d22 3130 2220 7374 726f  rlimit="10" stro
+00001280: 6b65 2d77 6964 7468 3d22 322e 3831 3436  ke-width="2.8146
+00001290: 3831 3138 3422 2073 7472 6f6b 652d 6461  81184" stroke-da
+000012a0: 7368 6172 7261 793d 2222 2f3e 3c2f 673e  sharray=""/></g>
+000012b0: 3c67 3e3c 672f 3e3c 7465 7874 2066 696c  <g><g/><text fil
+000012c0: 6c3d 2262 6c61 636b 2220 7374 726f 6b65  l="black" stroke
+000012d0: 3d22 6e6f 6e65 2220 666f 6e74 2d66 616d  ="none" font-fam
+000012e0: 696c 793d 2273 616e 732d 7365 7269 6622  ily="sans-serif"
+000012f0: 2066 6f6e 742d 7369 7a65 3d22 3131 7074   font-size="11pt
+00001300: 2220 666f 6e74 2d73 7479 6c65 3d22 6e6f  " font-style="no
+00001310: 726d 616c 2220 666f 6e74 2d77 6569 6768  rmal" font-weigh
+00001320: 743d 226e 6f72 6d61 6c22 2074 6578 742d  t="normal" text-
+00001330: 6465 636f 7261 7469 6f6e 3d22 6e6f 726d  decoration="norm
+00001340: 616c 2220 783d 2231 3731 2e37 3739 3932  al" x="171.77992
+00001350: 3534 3031 3630 3135 3622 2079 3d22 3431  540160156" y="41
+00001360: 2e36 3932 3436 3530 3337 3939 3939 3935  .692465037999995
+00001370: 2220 7465 7874 2d61 6e63 686f 723d 2273  " text-anchor="s
+00001380: 7461 7274 2220 646f 6d69 6e61 6e74 2d62  tart" dominant-b
+00001390: 6173 656c 696e 653d 2261 6c70 6861 6265  aseline="alphabe
+000013a0: 7469 6322 2078 6d6c 3a73 7061 6365 3d22  tic" xml:space="
+000013b0: 7072 6573 6572 7665 223e 5265 736f 7572  preserve">Resour
+000013c0: 6365 3c2f 7465 7874 3e3c 2f67 3e3c 7061  ce</text></g><pa
+000013d0: 7468 2066 696c 6c3d 226e 6f6e 6522 2073  th fill="none" s
+000013e0: 7472 6f6b 653d 226e 6f6e 6522 2f3e 3c67  troke="none"/><g
+000013f0: 3e3c 7061 7468 2066 696c 6c3d 2277 6869  ><path fill="whi
+00001400: 7465 2220 7374 726f 6b65 3d22 626c 6163  te" stroke="blac
+00001410: 6b22 2070 6169 6e74 2d6f 7264 6572 3d22  k" paint-order="
+00001420: 6669 6c6c 2073 7472 6f6b 6520 6d61 726b  fill stroke mark
+00001430: 6572 7322 2064 3d22 204d 2035 3731 2e30  ers" d=" M 571.0
+00001440: 3031 3030 3037 3839 3732 3420 3131 2e37  01000789724 11.7
+00001450: 3836 3437 3734 3537 3939 3939 3937 204c  86477457999997 L
+00001460: 2036 3430 2e39 3530 3333 3731 3236 3034   640.95033712604
+00001470: 3434 2031 312e 3738 3634 3737 3435 3739  44 11.7864774579
+00001480: 3939 3939 3720 4c20 3634 302e 3935 3033  99997 L 640.9503
+00001490: 3337 3132 3630 3434 3420 3539 2e32 3834  371260444 59.284
+000014a0: 3232 3234 3337 3939 3939 3836 204c 2035  222437999986 L 5
+000014b0: 3731 2e30 3031 3030 3037 3839 3732 3420  71.001000789724 
+000014c0: 3539 2e32 3834 3232 3234 3337 3939 3939  59.2842224379999
+000014d0: 3836 204c 2035 3731 2e30 3031 3030 3037  86 L 571.0010007
+000014e0: 3839 3732 3420 3131 2e37 3836 3437 3734  89724 11.7864774
+000014f0: 3537 3939 3939 3937 205a 2220 7374 726f  57999997 Z" stro
+00001500: 6b65 2d6d 6974 6572 6c69 6d69 743d 2231  ke-miterlimit="1
+00001510: 3022 2073 7472 6f6b 652d 7769 6474 683d  0" stroke-width=
+00001520: 2232 2e38 3134 3638 3131 3834 2220 7374  "2.814681184" st
+00001530: 726f 6b65 2d64 6173 6861 7272 6179 3d22  roke-dasharray="
+00001540: 222f 3e3c 2f67 3e3c 673e 3c67 2f3e 3c74  "/></g><g><g/><t
+00001550: 6578 7420 6669 6c6c 3d22 626c 6163 6b22  ext fill="black"
+00001560: 2073 7472 6f6b 653d 226e 6f6e 6522 2066   stroke="none" f
+00001570: 6f6e 742d 6661 6d69 6c79 3d22 7361 6e73  ont-family="sans
+00001580: 2d73 6572 6966 2220 666f 6e74 2d73 697a  -serif" font-siz
+00001590: 653d 2231 3170 7422 2066 6f6e 742d 7374  e="11pt" font-st
+000015a0: 796c 653d 226e 6f72 6d61 6c22 2066 6f6e  yle="normal" fon
+000015b0: 742d 7765 6967 6874 3d22 6e6f 726d 616c  t-weight="normal
+000015c0: 2220 7465 7874 2d64 6563 6f72 6174 696f  " text-decoratio
+000015d0: 6e3d 226e 6f72 6d61 6c22 2078 3d22 3539  n="normal" x="59
+000015e0: 302e 3038 3830 3537 3536 3837 3234 2220  0.088057568724" 
+000015f0: 793d 2234 312e 3639 3234 3635 3033 3739  y="41.6924650379
+00001600: 3939 3939 3522 2074 6578 742d 616e 6368  99995" text-anch
+00001610: 6f72 3d22 7374 6172 7422 2064 6f6d 696e  or="start" domin
+00001620: 616e 742d 6261 7365 6c69 6e65 3d22 616c  ant-baseline="al
+00001630: 7068 6162 6574 6963 2220 786d 6c3a 7370  phabetic" xml:sp
+00001640: 6163 653d 2270 7265 7365 7276 6522 3e46  ace="preserve">F
+00001650: 6965 6c64 3c2f 7465 7874 3e3c 2f67 3e3c  ield</text></g><
+00001660: 7061 7468 2066 696c 6c3d 226e 6f6e 6522  path fill="none"
+00001670: 2073 7472 6f6b 653d 226e 6f6e 6522 2f3e   stroke="none"/>
+00001680: 3c67 3e3c 7061 7468 2066 696c 6c3d 2277  <g><path fill="w
+00001690: 6869 7465 2220 7374 726f 6b65 3d22 626c  hite" stroke="bl
+000016a0: 6163 6b22 2070 6169 6e74 2d6f 7264 6572  ack" paint-order
+000016b0: 3d22 6669 6c6c 2073 7472 6f6b 6520 6d61  ="fill stroke ma
+000016c0: 726b 6572 7322 2064 3d22 204d 2038 3030  rkers" d=" M 800
+000016d0: 2e37 3337 3733 3438 3630 3835 3638 2031  .7377348608568 1
+000016e0: 312e 3738 3634 3737 3435 3739 3939 3939  1.78647745799999
+000016f0: 3720 4c20 3838 342e 3533 3831 3735 3933  7 L 884.53817593
+00001700: 3335 3035 3320 3131 2e37 3836 3437 3734  35053 11.7864774
+00001710: 3537 3939 3939 3937 204c 2038 3834 2e35  57999997 L 884.5
+00001720: 3338 3137 3539 3333 3530 3533 2035 392e  381759335053 59.
+00001730: 3238 3432 3232 3433 3739 3939 3938 3620  284222437999986 
+00001740: 4c20 3830 302e 3733 3737 3334 3836 3038  L 800.7377348608
+00001750: 3536 3820 3539 2e32 3834 3232 3234 3337  568 59.284222437
+00001760: 3939 3939 3836 204c 2038 3030 2e37 3337  999986 L 800.737
+00001770: 3733 3438 3630 3835 3638 2031 312e 3738  7348608568 11.78
+00001780: 3634 3737 3435 3739 3939 3939 3720 5a22  6477457999997 Z"
+00001790: 2073 7472 6f6b 652d 6d69 7465 726c 696d   stroke-miterlim
+000017a0: 6974 3d22 3130 2220 7374 726f 6b65 2d77  it="10" stroke-w
+000017b0: 6964 7468 3d22 322e 3831 3436 3831 3138  idth="2.81468118
+000017c0: 3422 2073 7472 6f6b 652d 6461 7368 6172  4" stroke-dashar
+000017d0: 7261 793d 2222 2f3e 3c2f 673e 3c67 3e3c  ray=""/></g><g><
+000017e0: 672f 3e3c 7465 7874 2066 696c 6c3d 2262  g/><text fill="b
+000017f0: 6c61 636b 2220 7374 726f 6b65 3d22 6e6f  lack" stroke="no
+00001800: 6e65 2220 666f 6e74 2d66 616d 696c 793d  ne" font-family=
+00001810: 2273 616e 732d 7365 7269 6622 2066 6f6e  "sans-serif" fon
+00001820: 742d 7369 7a65 3d22 3131 7074 2220 666f  t-size="11pt" fo
+00001830: 6e74 2d73 7479 6c65 3d22 6e6f 726d 616c  nt-style="normal
+00001840: 2220 666f 6e74 2d77 6569 6768 743d 226e  " font-weight="n
+00001850: 6f72 6d61 6c22 2074 6578 742d 6465 636f  ormal" text-deco
+00001860: 7261 7469 6f6e 3d22 6e6f 726d 616c 2220  ration="normal" 
+00001870: 783d 2238 3139 2e38 3234 3739 3136 3339  x="819.824791639
+00001880: 3835 3638 2220 793d 2234 312e 3639 3234  8568" y="41.6924
+00001890: 3635 3033 3739 3939 3939 3522 2074 6578  65037999995" tex
+000018a0: 742d 616e 6368 6f72 3d22 7374 6172 7422  t-anchor="start"
+000018b0: 2064 6f6d 696e 616e 742d 6261 7365 6c69   dominant-baseli
+000018c0: 6e65 3d22 616c 7068 6162 6574 6963 2220  ne="alphabetic" 
+000018d0: 786d 6c3a 7370 6163 653d 2270 7265 7365  xml:space="prese
+000018e0: 7276 6522 3e57 6964 6765 743c 2f74 6578  rve">Widget</tex
+000018f0: 743e 3c2f 673e 3c70 6174 6820 6669 6c6c  t></g><path fill
+00001900: 3d22 6e6f 6e65 2220 7374 726f 6b65 3d22  ="none" stroke="
+00001910: 6e6f 6e65 222f 3e3c 673e 3c70 6174 6820  none"/><g><path 
+00001920: 6669 6c6c 3d22 7768 6974 6522 2073 7472  fill="white" str
+00001930: 6f6b 653d 2262 6c61 636b 2220 7061 696e  oke="black" pain
+00001940: 742d 6f72 6465 723d 2266 696c 6c20 7374  t-order="fill st
+00001950: 726f 6b65 206d 6172 6b65 7273 2220 643d  roke markers" d=
+00001960: 2220 4d20 3932 352e 3332 3431 3835 3131  " M 925.32418511
+00001970: 3835 3133 2031 312e 3738 3634 3737 3435  8513 11.78647745
+00001980: 3739 3939 3939 3720 4c20 3130 3533 2e31  7999997 L 1053.1
+00001990: 3430 3335 3830 3032 3638 3520 3131 2e37  40358002685 11.7
+000019a0: 3836 3437 3734 3537 3939 3939 3937 204c  86477457999997 L
+000019b0: 2031 3035 332e 3134 3033 3538 3030 3236   1053.1403580026
+000019c0: 3835 2035 392e 3238 3432 3232 3433 3739  85 59.2842224379
+000019d0: 3939 3938 3620 4c20 3932 352e 3332 3431  99986 L 925.3241
+000019e0: 3835 3131 3835 3133 2035 392e 3238 3432  85118513 59.2842
+000019f0: 3232 3433 3739 3939 3938 3620 4c20 3932  22437999986 L 92
+00001a00: 352e 3332 3431 3835 3131 3835 3133 2031  5.324185118513 1
+00001a10: 312e 3738 3634 3737 3435 3739 3939 3939  1.78647745799999
+00001a20: 3720 5a22 2073 7472 6f6b 652d 6d69 7465  7 Z" stroke-mite
+00001a30: 726c 696d 6974 3d22 3130 2220 7374 726f  rlimit="10" stro
+00001a40: 6b65 2d77 6964 7468 3d22 322e 3831 3436  ke-width="2.8146
+00001a50: 3831 3138 3422 2073 7472 6f6b 652d 6461  81184" stroke-da
+00001a60: 7368 6172 7261 793d 2222 2f3e 3c2f 673e  sharray=""/></g>
+00001a70: 3c67 3e3c 672f 3e3c 7465 7874 2066 696c  <g><g/><text fil
+00001a80: 6c3d 2262 6c61 636b 2220 7374 726f 6b65  l="black" stroke
+00001a90: 3d22 6e6f 6e65 2220 666f 6e74 2d66 616d  ="none" font-fam
+00001aa0: 696c 793d 2273 616e 732d 7365 7269 6622  ily="sans-serif"
+00001ab0: 2066 6f6e 742d 7369 7a65 3d22 3131 7074   font-size="11pt
+00001ac0: 2220 666f 6e74 2d73 7479 6c65 3d22 6e6f  " font-style="no
+00001ad0: 726d 616c 2220 666f 6e74 2d77 6569 6768  rmal" font-weigh
+00001ae0: 743d 226e 6f72 6d61 6c22 2074 6578 742d  t="normal" text-
+00001af0: 6465 636f 7261 7469 6f6e 3d22 6e6f 726d  decoration="norm
+00001b00: 616c 2220 783d 2239 3434 2e34 3131 3234  al" x="944.41124
+00001b10: 3138 3937 3531 3322 2079 3d22 3431 2e36  1897513" y="41.6
+00001b20: 3932 3436 3530 3337 3939 3939 3935 2220  92465037999995" 
+00001b30: 7465 7874 2d61 6e63 686f 723d 2273 7461  text-anchor="sta
+00001b40: 7274 2220 646f 6d69 6e61 6e74 2d62 6173  rt" dominant-bas
+00001b50: 656c 696e 653d 2261 6c70 6861 6265 7469  eline="alphabeti
+00001b60: 6322 2078 6d6c 3a73 7061 6365 3d22 7072  c" xml:space="pr
+00001b70: 6573 6572 7665 223e 7461 626c 6962 2e44  eserve">tablib.D
+00001b80: 6174 6173 6574 3c2f 7465 7874 3e3c 2f67  ataset</text></g
+00001b90: 3e3c 2f67 3e3c 673e 3c70 6174 6820 6669  ></g><g><path fi
+00001ba0: 6c6c 3d22 7768 6974 6522 2073 7472 6f6b  ll="white" strok
+00001bb0: 653d 2262 6c61 636b 2220 7061 696e 742d  e="black" paint-
+00001bc0: 6f72 6465 723d 2266 696c 6c20 7374 726f  order="fill stro
+00001bd0: 6b65 206d 6172 6b65 7273 2220 643d 2220  ke markers" d=" 
+00001be0: 4d20 3139 342e 3335 3438 3237 3634 3634  M 194.3548276464
+00001bf0: 3235 3738 2031 3430 2e32 3036 3330 3634  2578 140.2063064
+00001c00: 3738 204c 2032 3131 2e39 3436 3538 3530  78 L 211.9465850
+00001c10: 3436 3432 3537 3820 3134 302e 3230 3633  4642578 140.2063
+00001c20: 3036 3437 3820 4c20 3231 312e 3934 3635  06478 L 211.9465
+00001c30: 3835 3034 3634 3235 3738 2031 3535 322e  8504642578 1552.
+00001c40: 3832 3434 3235 3639 3739 3939 3720 4c20  8244256979997 L 
+00001c50: 3139 342e 3335 3438 3237 3634 3634 3235  194.354827646425
+00001c60: 3738 2031 3535 322e 3832 3434 3235 3639  78 1552.82442569
+00001c70: 3739 3939 3720 4c20 3139 342e 3335 3438  79997 L 194.3548
+00001c80: 3237 3634 3634 3235 3738 2031 3430 2e32  2764642578 140.2
+00001c90: 3036 3330 3634 3738 2220 7374 726f 6b65  06306478" stroke
+00001ca0: 2d6d 6974 6572 6c69 6d69 743d 2231 3022  -miterlimit="10"
+00001cb0: 2073 7472 6f6b 652d 7769 6474 683d 2231   stroke-width="1
+00001cc0: 2e34 3635 3937 3937 3833 3333 3333 3333  .465979783333333
+00001cd0: 3222 2073 7472 6f6b 652d 6461 7368 6172  2" stroke-dashar
+00001ce0: 7261 793d 2222 2f3e 3c70 6174 6820 6669  ray=""/><path fi
+00001cf0: 6c6c 3d22 6c69 6768 7462 6c75 6522 2073  ll="lightblue" s
+00001d00: 7472 6f6b 653d 2262 6c61 636b 2220 7061  troke="black" pa
+00001d10: 696e 742d 6f72 6465 723d 2266 696c 6c20  int-order="fill 
+00001d20: 7374 726f 6b65 206d 6172 6b65 7273 2220  stroke markers" 
+00001d30: 643d 2220 4d20 3230 332e 3135 3037 3036  d=" M 203.150706
+00001d40: 3334 3634 3235 3738 2033 3638 2e38 3939  34642578 368.899
+00001d50: 3135 3236 3738 204c 2032 3230 2e37 3432  152678 L 220.742
+00001d60: 3436 3337 3436 3432 3537 3820 3336 382e  46374642578 368.
+00001d70: 3839 3931 3532 3637 3820 4c20 3232 302e  899152678 L 220.
+00001d80: 3734 3234 3633 3734 3634 3235 3738 2034  74246374642578 4
+00001d90: 3138 2e31 3536 3037 3333 3938 3030 3030  18.1560733980000
+00001da0: 3520 4c20 3230 332e 3135 3037 3036 3334  5 L 203.15070634
+00001db0: 3634 3235 3738 2034 3138 2e31 3536 3037  642578 418.15607
+00001dc0: 3333 3938 3030 3030 3520 4c20 3230 332e  339800005 L 203.
+00001dd0: 3135 3037 3036 3334 3634 3235 3738 2033  15070634642578 3
+00001de0: 3638 2e38 3939 3135 3236 3738 2220 7374  68.899152678" st
+00001df0: 726f 6b65 2d6d 6974 6572 6c69 6d69 743d  roke-miterlimit=
+00001e00: 2231 3022 2073 7472 6f6b 652d 7769 6474  "10" stroke-widt
+00001e10: 683d 2231 2e34 3635 3937 3937 3833 3333  h="1.46597978333
+00001e20: 3333 3333 3222 2073 7472 6f6b 652d 6461  33332" stroke-da
+00001e30: 7368 6172 7261 793d 2222 2f3e 3c70 6174  sharray=""/><pat
+00001e40: 6820 6669 6c6c 3d22 6c69 6768 7462 6c75  h fill="lightblu
+00001e50: 6522 2073 7472 6f6b 653d 2262 6c61 636b  e" stroke="black
+00001e60: 2220 7061 696e 742d 6f72 6465 723d 2266  " paint-order="f
+00001e70: 696c 6c20 7374 726f 6b65 206d 6172 6b65  ill stroke marke
+00001e80: 7273 2220 643d 2220 4d20 3230 332e 3135  rs" d=" M 203.15
+00001e90: 3037 3036 3334 3634 3235 3738 2035 3133  070634642578 513
+00001ea0: 2e31 3531 3536 3333 3538 204c 2032 3230  .151563358 L 220
+00001eb0: 2e37 3432 3436 3337 3436 3432 3537 3820  .74246374642578 
+00001ec0: 3531 332e 3135 3135 3633 3335 3820 4c20  513.151563358 L 
+00001ed0: 3232 302e 3734 3234 3633 3734 3634 3235  220.742463746425
+00001ee0: 3738 2035 3632 2e34 3038 3438 3430 3737  78 562.408484077
+00001ef0: 3939 3939 204c 2032 3033 2e31 3530 3730  9999 L 203.15070
+00001f00: 3633 3436 3432 3537 3820 3536 322e 3430  634642578 562.40
+00001f10: 3834 3834 3037 3739 3939 3920 4c20 3230  84840779999 L 20
+00001f20: 332e 3135 3037 3036 3334 3634 3235 3738  3.15070634642578
+00001f30: 2035 3133 2e31 3531 3536 3333 3538 2220   513.151563358" 
+00001f40: 7374 726f 6b65 2d6d 6974 6572 6c69 6d69  stroke-miterlimi
+00001f50: 743d 2231 3022 2073 7472 6f6b 652d 7769  t="10" stroke-wi
+00001f60: 6474 683d 2231 2e34 3635 3937 3937 3833  dth="1.465979783
+00001f70: 3333 3333 3333 3222 2073 7472 6f6b 652d  3333332" stroke-
+00001f80: 6461 7368 6172 7261 793d 2222 2f3e 3c70  dasharray=""/><p
+00001f90: 6174 6820 6669 6c6c 3d22 6c69 6768 7462  ath fill="lightb
+00001fa0: 6c75 6522 2073 7472 6f6b 653d 2262 6c61  lue" stroke="bla
+00001fb0: 636b 2220 7061 696e 742d 6f72 6465 723d  ck" paint-order=
+00001fc0: 2266 696c 6c20 7374 726f 6b65 206d 6172  "fill stroke mar
+00001fd0: 6b65 7273 2220 643d 2220 4d20 3230 332e  kers" d=" M 203.
+00001fe0: 3135 3037 3036 3334 3634 3235 3738 2037  15070634642578 7
+00001ff0: 3034 2e39 3031 3731 3930 3137 3939 3939  04.9017190179999
+00002000: 204c 2032 3230 2e37 3432 3436 3337 3436   L 220.742463746
+00002010: 3432 3537 3820 3730 342e 3930 3137 3139  42578 704.901719
+00002020: 3031 3739 3939 3920 4c20 3232 302e 3734  0179999 L 220.74
+00002030: 3234 3633 3734 3634 3235 3738 2031 3432  246374642578 142
+00002040: 372e 3932 3239 3438 3135 3739 3939 3620  7.9229481579996 
+00002050: 4c20 3230 332e 3135 3037 3036 3334 3634  L 203.1507063464
+00002060: 3235 3738 2031 3432 372e 3932 3239 3438  2578 1427.922948
+00002070: 3135 3739 3939 3620 4c20 3230 332e 3135  1579996 L 203.15
+00002080: 3037 3036 3334 3634 3235 3738 2037 3034  070634642578 704
+00002090: 2e39 3031 3731 3930 3137 3939 3939 2220  .9017190179999" 
+000020a0: 7374 726f 6b65 2d6d 6974 6572 6c69 6d69  stroke-miterlimi
+000020b0: 743d 2231 3022 2073 7472 6f6b 652d 7769  t="10" stroke-wi
+000020c0: 6474 683d 2231 2e34 3635 3937 3937 3833  dth="1.465979783
+000020d0: 3333 3333 3333 3222 2073 7472 6f6b 652d  3333332" stroke-
+000020e0: 6461 7368 6172 7261 793d 2222 2f3e 3c70  dasharray=""/><p
+000020f0: 6174 6820 6669 6c6c 3d22 6c69 6768 7470  ath fill="lightp
+00002100: 696e 6b22 2073 7472 6f6b 653d 2262 6c61  ink" stroke="bla
+00002110: 636b 2220 7061 696e 742d 6f72 6465 723d  ck" paint-order=
+00002120: 2266 696c 6c20 7374 726f 6b65 206d 6172  "fill stroke mar
+00002130: 6b65 7273 2220 643d 2220 4d20 3231 312e  kers" d=" M 211.
+00002140: 3934 3635 3835 3034 3634 3235 3738 2038  94658504642578 8
+00002150: 3234 2e35 3235 3636 3933 3337 3939 3938  24.5256693379998
+00002160: 204c 2032 3239 2e35 3338 3334 3234 3436   L 229.538342446
+00002170: 3432 3538 2038 3234 2e35 3235 3636 3933  4258 824.5256693
+00002180: 3337 3939 3938 204c 2032 3239 2e35 3338  379998 L 229.538
+00002190: 3334 3234 3436 3432 3538 2031 3430 312e  3424464258 1401.
+000021a0: 3533 3533 3132 3035 3739 3939 3620 4c20  5353120579996 L 
+000021b0: 3231 312e 3934 3635 3835 3034 3634 3235  211.946585046425
+000021c0: 3738 2031 3430 312e 3533 3533 3132 3035  78 1401.53531205
+000021d0: 3739 3939 3620 4c20 3231 312e 3934 3635  79996 L 211.9465
+000021e0: 3835 3034 3634 3235 3738 2038 3234 2e35  8504642578 824.5
+000021f0: 3235 3636 3933 3337 3939 3938 2220 7374  256693379998" st
+00002200: 726f 6b65 2d6d 6974 6572 6c69 6d69 743d  roke-miterlimit=
+00002210: 2231 3022 2073 7472 6f6b 652d 7769 6474  "10" stroke-widt
+00002220: 683d 2231 2e34 3635 3937 3937 3833 3333  h="1.46597978333
+00002230: 3333 3333 3222 2073 7472 6f6b 652d 6461  33332" stroke-da
+00002240: 7368 6172 7261 793d 2222 2f3e 3c70 6174  sharray=""/><pat
+00002250: 6820 6669 6c6c 3d22 6c69 6768 7462 6c75  h fill="lightblu
+00002260: 6522 2073 7472 6f6b 653d 2262 6c61 636b  e" stroke="black
+00002270: 2220 7061 696e 742d 6f72 6465 723d 2266  " paint-order="f
+00002280: 696c 6c20 7374 726f 6b65 206d 6172 6b65  ill stroke marke
+00002290: 7273 2220 643d 2220 4d20 3539 372e 3137  rs" d=" M 597.17
+000022a0: 3937 3930 3235 3738 3834 3220 3837 332e  97902578842 873.
+000022b0: 3738 3235 3930 3035 3739 3939 3920 4c20  7825900579999 L 
+000022c0: 3631 342e 3737 3135 3437 3635 3738 3834  614.771547657884
+000022d0: 3220 3837 332e 3738 3235 3930 3035 3739  2 873.7825900579
+000022e0: 3939 3920 4c20 3631 342e 3737 3135 3437  999 L 614.771547
+000022f0: 3635 3738 3834 3220 3134 3031 2e35 3335  6578842 1401.535
+00002300: 3331 3230 3537 3939 3936 204c 2035 3937  3120579996 L 597
+00002310: 2e31 3739 3739 3032 3537 3838 3432 2031  .1797902578842 1
+00002320: 3430 312e 3533 3533 3132 3035 3739 3939  401.535312057999
+00002330: 3620 4c20 3539 372e 3137 3937 3930 3235  6 L 597.17979025
+00002340: 3738 3834 3220 3837 332e 3738 3235 3930  78842 873.782590
+00002350: 3035 3739 3939 3922 2073 7472 6f6b 652d  0579999" stroke-
+00002360: 6d69 7465 726c 696d 6974 3d22 3130 2220  miterlimit="10" 
+00002370: 7374 726f 6b65 2d77 6964 7468 3d22 312e  stroke-width="1.
+00002380: 3436 3539 3739 3738 3333 3333 3333 3332  4659797833333332
+00002390: 2220 7374 726f 6b65 2d64 6173 6861 7272  " stroke-dasharr
+000023a0: 6179 3d22 222f 3e3c 7061 7468 2066 696c  ay=""/><path fil
+000023b0: 6c3d 226c 6967 6874 7069 6e6b 2220 7374  l="lightpink" st
+000023c0: 726f 6b65 3d22 626c 6163 6b22 2070 6169  roke="black" pai
+000023d0: 6e74 2d6f 7264 6572 3d22 6669 6c6c 2073  nt-order="fill s
+000023e0: 7472 6f6b 6520 6d61 726b 6572 7322 2064  troke markers" d
+000023f0: 3d22 204d 2036 3035 2e39 3735 3636 3839  =" M 605.9756689
+00002400: 3537 3838 3432 2031 3033 302e 3334 3932  578842 1030.3492
+00002410: 3330 3931 3739 3939 3920 4c20 3632 332e  309179999 L 623.
+00002420: 3536 3734 3236 3335 3738 3834 3220 3130  5674263578842 10
+00002430: 3330 2e33 3439 3233 3039 3137 3939 3939  30.3492309179999
+00002440: 204c 2036 3233 2e35 3637 3432 3633 3537   L 623.567426357
+00002450: 3838 3432 2031 3335 322e 3237 3833 3931  8842 1352.278391
+00002460: 3333 3739 3939 3720 4c20 3630 352e 3937  3379997 L 605.97
+00002470: 3536 3638 3935 3738 3834 3220 3133 3532  56689578842 1352
+00002480: 2e32 3738 3339 3133 3337 3939 3937 204c  .2783913379997 L
+00002490: 2036 3035 2e39 3735 3636 3839 3537 3838   605.97566895788
+000024a0: 3432 2031 3033 302e 3334 3932 3330 3931  42 1030.34923091
+000024b0: 3739 3939 3922 2073 7472 6f6b 652d 6d69  79999" stroke-mi
+000024c0: 7465 726c 696d 6974 3d22 3130 2220 7374  terlimit="10" st
+000024d0: 726f 6b65 2d77 6964 7468 3d22 312e 3436  roke-width="1.46
+000024e0: 3539 3739 3738 3333 3333 3333 3332 2220  59797833333332" 
+000024f0: 7374 726f 6b65 2d64 6173 6861 7272 6179  stroke-dasharray
+00002500: 3d22 222f 3e3c 7061 7468 2066 696c 6c3d  =""/><path fill=
+00002510: 2277 6869 7465 2220 7374 726f 6b65 3d22  "white" stroke="
+00002520: 626c 6163 6b22 2070 6169 6e74 2d6f 7264  black" paint-ord
+00002530: 6572 3d22 6669 6c6c 2073 7472 6f6b 6520  er="fill stroke 
+00002540: 6d61 726b 6572 7322 2064 3d22 204d 2038  markers" d=" M 8
+00002550: 3333 2e38 3432 3037 3636 3937 3138 3120  33.842076697181 
+00002560: 3132 3138 2e35 3831 3033 3530 3937 3939  1218.58103509799
+00002570: 3938 204c 2038 3531 2e34 3333 3833 3430  98 L 851.4338340
+00002580: 3937 3138 3120 3132 3138 2e35 3831 3033  97181 1218.58103
+00002590: 3530 3937 3939 3938 204c 2038 3531 2e34  50979998 L 851.4
+000025a0: 3333 3833 3430 3937 3138 3120 3133 3532  33834097181 1352
+000025b0: 2e32 3738 3339 3133 3337 3939 3937 204c  .2783913379997 L
+000025c0: 2038 3333 2e38 3432 3037 3636 3937 3138   833.84207669718
+000025d0: 3120 3133 3532 2e32 3738 3339 3133 3337  1 1352.278391337
+000025e0: 3939 3937 204c 2038 3333 2e38 3432 3037  9997 L 833.84207
+000025f0: 3636 3937 3138 3120 3132 3138 2e35 3831  6697181 1218.581
+00002600: 3033 3530 3937 3939 3938 2220 7374 726f  0350979998" stro
+00002610: 6b65 2d6d 6974 6572 6c69 6d69 743d 2231  ke-miterlimit="1
+00002620: 3022 2073 7472 6f6b 652d 7769 6474 683d  0" stroke-width=
+00002630: 2231 2e34 3635 3937 3937 3833 3333 3333  "1.4659797833333
+00002640: 3333 3222 2073 7472 6f6b 652d 6461 7368  332" stroke-dash
+00002650: 6172 7261 793d 2222 2f3e 3c67 3e3c 673e  array=""/><g><g>
+00002660: 3c72 6563 7420 6669 6c6c 3d22 7768 6974  <rect fill="whit
+00002670: 6522 2073 7472 6f6b 653d 226e 6f6e 6522  e" stroke="none"
+00002680: 2078 3d22 3233 322e 3736 3334 3937 3936   x="232.76349796
+00002690: 3937 3539 3122 2079 3d22 3934 2e34 3637  97591" y="94.467
+000026a0: 3733 3732 3337 3939 3939 3822 2077 6964  73723799998" wid
+000026b0: 7468 3d22 3237 382e 3838 3530 3731 3136  th="278.88507116
+000026c0: 3533 3132 3522 2068 6569 6768 743d 2232  53125" height="2
+000026d0: 322e 3836 3932 3834 3632 222f 3e3c 2f67  2.86928462"/></g
+000026e0: 3e3c 7465 7874 2066 696c 6c3d 2262 6c61  ><text fill="bla
+000026f0: 636b 2220 7374 726f 6b65 3d22 6e6f 6e65  ck" stroke="none
+00002700: 2220 666f 6e74 2d66 616d 696c 793d 226d  " font-family="m
+00002710: 6f6e 6f73 7061 6365 2220 666f 6e74 2d73  onospace" font-s
+00002720: 697a 653d 2231 3170 7422 2066 6f6e 742d  ize="11pt" font-
+00002730: 7374 796c 653d 226e 6f72 6d61 6c22 2066  style="normal" f
+00002740: 6f6e 742d 7765 6967 6874 3d22 6e6f 726d  ont-weight="norm
+00002750: 616c 2220 7465 7874 2d64 6563 6f72 6174  al" text-decorat
+00002760: 696f 6e3d 226e 6f72 6d61 6c22 2078 3d22  ion="normal" x="
+00002770: 3233 352e 3430 3232 3631 3537 3937 3539  235.402261579759
+00002780: 3122 2079 3d22 3131 302e 3330 3033 3138  1" y="110.300318
+00002790: 3839 3739 3939 3937 2220 7465 7874 2d61  89799997" text-a
+000027a0: 6e63 686f 723d 2273 7461 7274 2220 646f  nchor="start" do
+000027b0: 6d69 6e61 6e74 2d62 6173 656c 696e 653d  minant-baseline=
+000027c0: 2261 6c70 6861 6265 7469 6322 2078 6d6c  "alphabetic" xml
+000027d0: 3a73 7061 6365 3d22 7072 6573 6572 7665  :space="preserve
+000027e0: 223e 6578 706f 7274 2871 7565 7279 7365  ">export(queryse
+000027f0: 743d 4e6f 6e65 2cc2 a02a 2a6b 7761 7267  t=None,..**kwarg
+00002800: 7329 3c2f 7465 7874 3e3c 2f67 3e3c 673e  s)</text></g><g>
+00002810: 3c70 6174 6820 6669 6c6c 3d22 6e6f 6e65  <path fill="none
+00002820: 2220 7374 726f 6b65 3d22 626c 6163 6b22  " stroke="black"
+00002830: 2070 6169 6e74 2d6f 7264 6572 3d22 6669   paint-order="fi
+00002840: 6c6c 2073 7472 6f6b 6520 6d61 726b 6572  ll stroke marker
+00002850: 7322 2064 3d22 204d 2032 3033 2e31 3530  s" d=" M 203.150
+00002860: 3730 3633 3436 3432 3537 3820 3131 372e  70634642578 117.
+00002870: 3333 3730 3231 3835 3739 3939 3939 204c  33702185799999 L
+00002880: 2032 3832 2e33 3133 3631 3436 3436 3432   282.31361464642
+00002890: 3538 2031 3137 2e33 3337 3032 3138 3537  58 117.337021857
+000028a0: 3939 3939 3920 4c20 3238 322e 3331 3336  99999 L 282.3136
+000028b0: 3134 3634 3634 3235 3820 3134 302e 3230  146464258 140.20
+000028c0: 3633 3036 3437 3820 4c20 3232 362e 3433  6306478 L 226.43
+000028d0: 3034 3635 3330 3537 3539 3133 2031 3430  046530575913 140
+000028e0: 2e32 3036 3330 3634 3738 2220 7374 726f  .206306478" stro
+000028f0: 6b65 2d6d 6974 6572 6c69 6d69 743d 2231  ke-miterlimit="1
+00002900: 3022 2073 7472 6f6b 652d 7769 6474 683d  0" stroke-width=
+00002910: 2231 2e34 3635 3937 3937 3833 3333 3333  "1.4659797833333
+00002920: 3333 3222 2073 7472 6f6b 652d 6461 7368  332" stroke-dash
+00002930: 6172 7261 793d 2222 2f3e 3c67 2074 7261  array=""/><g tra
+00002940: 6e73 666f 726d 3d22 7472 616e 736c 6174  nsform="translat
+00002950: 6528 3231 312e 3934 3635 3835 3034 3634  e(211.9465850464
+00002960: 3235 3738 2c31 3430 2e32 3036 3330 3634  2578,140.2063064
+00002970: 3738 2920 7472 616e 736c 6174 6528 2d32  78) translate(-2
+00002980: 3131 2e39 3436 3538 3530 3436 3432 3537  11.9465850464257
+00002990: 382c 2d31 3430 2e32 3036 3330 3634 3738  8,-140.206306478
+000029a0: 2922 3e3c 7061 7468 2066 696c 6c3d 2262  )"><path fill="b
+000029b0: 6c61 636b 2220 7374 726f 6b65 3d22 6e6f  lack" stroke="no
+000029c0: 6e65 2220 7061 696e 742d 6f72 6465 723d  ne" paint-order=
+000029d0: 2273 7472 6f6b 6520 6669 6c6c 206d 6172  "stroke fill mar
+000029e0: 6b65 7273 2220 643d 2220 4d20 3232 362e  kers" d=" M 226.
+000029f0: 3630 3633 3832 3837 3937 3539 3120 3133  6063828797591 13
+00002a00: 322e 3837 3634 3037 3536 3133 3333 3320  2.8764075613333 
+00002a10: 4c20 3231 312e 3934 3635 3835 3034 3634  L 211.9465850464
+00002a20: 3235 3738 2031 3430 2e32 3036 3330 3634  2578 140.2063064
+00002a30: 3738 204c 2032 3236 2e36 3036 3338 3238  78 L 226.6063828
+00002a40: 3739 3735 3931 2031 3437 2e35 3336 3230  797591 147.53620
+00002a50: 3533 3934 3636 3636 3720 5a22 2f3e 3c2f  539466667 Z"/></
+00002a60: 673e 3c2f 673e 3c67 3e3c 673e 3c72 6563  g></g><g><g><rec
+00002a70: 7420 6669 6c6c 3d22 7768 6974 6522 2073  t fill="white" s
+00002a80: 7472 6f6b 653d 226e 6f6e 6522 2078 3d22  troke="none" x="
+00002a90: 3233 322e 3736 3334 3937 3936 3937 3539  232.763497969759
+00002aa0: 3122 2079 3d22 3136 362e 3539 3339 3432  1" y="166.593942
+00002ab0: 3537 3822 2077 6964 7468 3d22 3334 302e  578" width="340.
+00002ac0: 3636 3734 3139 3739 3831 3235 2220 6865  667419798125" he
+00002ad0: 6967 6874 3d22 3232 2e38 3639 3238 3436  ight="22.8692846
+00002ae0: 3222 2f3e 3c2f 673e 3c67 3e3c 7265 6374  2"/></g><g><rect
+00002af0: 2066 696c 6c3d 2279 656c 6c6f 7722 2073   fill="yellow" s
+00002b00: 7472 6f6b 653d 226e 6f6e 6522 2078 3d22  troke="none" x="
+00002b10: 3233 352e 3430 3232 3631 3537 3937 3539  235.402261579759
+00002b20: 3122 2079 3d22 3136 392e 3430 3836 3233  1" y="169.408623
+00002b30: 3736 3230 3030 3032 2220 7769 6474 683d  76200002" width=
+00002b40: 2233 3335 2e33 3839 3839 3235 3738 3132  "335.38989257812
+00002b50: 3522 2068 6569 6768 743d 2231 372e 3736  5" height="17.76
+00002b60: 3736 3734 3937 3422 2f3e 3c74 6578 7420  7674974"/><text 
+00002b70: 6669 6c6c 3d22 626c 6163 6b22 2073 7472  fill="black" str
+00002b80: 6f6b 653d 226e 6f6e 6522 2066 6f6e 742d  oke="none" font-
+00002b90: 6661 6d69 6c79 3d22 6d6f 6e6f 7370 6163  family="monospac
+00002ba0: 6522 2066 6f6e 742d 7369 7a65 3d22 3131  e" font-size="11
+00002bb0: 7074 2220 666f 6e74 2d73 7479 6c65 3d22  pt" font-style="
+00002bc0: 6e6f 726d 616c 2220 666f 6e74 2d77 6569  normal" font-wei
+00002bd0: 6768 743d 226e 6f72 6d61 6c22 2074 6578  ght="normal" tex
+00002be0: 742d 6465 636f 7261 7469 6f6e 3d22 6e6f  t-decoration="no
+00002bf0: 726d 616c 2220 783d 2232 3335 2e34 3032  rmal" x="235.402
+00002c00: 3236 3135 3739 3735 3931 2220 793d 2231  2615797591" y="1
+00002c10: 3832 2e34 3236 3532 3432 3338 2220 7465  82.426524238" te
+00002c20: 7874 2d61 6e63 686f 723d 2273 7461 7274  xt-anchor="start
+00002c30: 2220 646f 6d69 6e61 6e74 2d62 6173 656c  " dominant-basel
+00002c40: 696e 653d 2261 6c70 6861 6265 7469 6322  ine="alphabetic"
+00002c50: 2078 6d6c 3a73 7061 6365 3d22 7072 6573   xml:space="pres
+00002c60: 6572 7665 223e 6265 666f 7265 5f65 7870  erve">before_exp
+00002c70: 6f72 7428 7175 6572 7973 6574 3d4e 6f6e  ort(queryset=Non
+00002c80: 652c c2a0 2a2a 6b77 6172 6773 293c 2f74  e,..**kwargs)</t
+00002c90: 6578 743e 3c2f 673e 3c67 3e3c 7061 7468  ext></g><g><path
+00002ca0: 2066 696c 6c3d 226e 6f6e 6522 2073 7472   fill="none" str
+00002cb0: 6f6b 653d 2262 6c61 636b 2220 7061 696e  oke="black" pain
+00002cc0: 742d 6f72 6465 723d 2266 696c 6c20 7374  t-order="fill st
+00002cd0: 726f 6b65 206d 6172 6b65 7273 2220 643d  roke markers" d=
+00002ce0: 2220 4d20 3231 312e 3934 3635 3835 3034  " M 211.94658504
+00002cf0: 3634 3235 3738 2031 3839 2e34 3633 3232  642578 189.46322
+00002d00: 3731 3938 204c 2032 3832 2e33 3133 3631  7198 L 282.31361
+00002d10: 3436 3436 3432 3538 2031 3839 2e34 3633  46464258 189.463
+00002d20: 3232 3731 3938 204c 2032 3832 2e33 3133  227198 L 282.313
+00002d30: 3631 3436 3436 3432 3538 2032 3132 2e33  6146464258 212.3
+00002d40: 3332 3531 3138 3138 204c 2032 3236 2e34  32511818 L 226.4
+00002d50: 3330 3436 3533 3035 3735 3931 3320 3231  3046530575913 21
+00002d60: 322e 3333 3235 3131 3831 3822 2073 7472  2.332511818" str
+00002d70: 6f6b 652d 6d69 7465 726c 696d 6974 3d22  oke-miterlimit="
+00002d80: 3130 2220 7374 726f 6b65 2d77 6964 7468  10" stroke-width
+00002d90: 3d22 312e 3436 3539 3739 3738 3333 3333  ="1.465979783333
+00002da0: 3333 3332 2220 7374 726f 6b65 2d64 6173  3332" stroke-das
+00002db0: 6861 7272 6179 3d22 222f 3e3c 6720 7472  harray=""/><g tr
+00002dc0: 616e 7366 6f72 6d3d 2274 7261 6e73 6c61  ansform="transla
+00002dd0: 7465 2832 3131 2e39 3436 3538 3530 3436  te(211.946585046
+00002de0: 3432 3537 382c 3231 322e 3333 3235 3131  42578,212.332511
+00002df0: 3831 3829 2074 7261 6e73 6c61 7465 282d  818) translate(-
+00002e00: 3231 312e 3934 3635 3835 3034 3634 3235  211.946585046425
+00002e10: 3738 2c2d 3231 322e 3333 3235 3131 3831  78,-212.33251181
+00002e20: 3829 223e 3c70 6174 6820 6669 6c6c 3d22  8)"><path fill="
+00002e30: 626c 6163 6b22 2073 7472 6f6b 653d 226e  black" stroke="n
+00002e40: 6f6e 6522 2070 6169 6e74 2d6f 7264 6572  one" paint-order
+00002e50: 3d22 7374 726f 6b65 2066 696c 6c20 6d61  ="stroke fill ma
+00002e60: 726b 6572 7322 2064 3d22 204d 2032 3236  rkers" d=" M 226
+00002e70: 2e36 3036 3338 3238 3739 3735 3931 2032  .6063828797591 2
+00002e80: 3035 2e30 3032 3631 3239 3031 3333 3333  05.0026129013333
+00002e90: 3220 4c20 3231 312e 3934 3635 3835 3034  2 L 211.94658504
+00002ea0: 3634 3235 3738 2032 3132 2e33 3332 3531  642578 212.33251
+00002eb0: 3138 3138 204c 2032 3236 2e36 3036 3338  1818 L 226.60638
+00002ec0: 3238 3739 3735 3931 2032 3139 2e36 3632  28797591 219.662
+00002ed0: 3431 3037 3334 3636 3636 3820 5a22 2f3e  41073466668 Z"/>
+00002ee0: 3c2f 673e 3c2f 673e 3c70 6174 6820 6669  </g></g><path fi
+00002ef0: 6c6c 3d22 7768 6974 6522 2073 7472 6f6b  ll="white" strok
+00002f00: 653d 2262 6c61 636b 2220 7061 696e 742d  e="black" paint-
+00002f10: 6f72 6465 723d 2266 696c 6c20 7374 726f  order="fill stro
+00002f20: 6b65 206d 6172 6b65 7273 2220 643d 2220  ke markers" d=" 
+00002f30: 4d20 3137 2e35 3931 3735 3734 3030 3030  M 17.59175740000
+00002f40: 3030 3032 2032 3338 2e37 3230 3134 3739  0002 238.7201479
+00002f50: 3138 204c 2033 3732 2e38 3737 3037 3336  18 L 372.8770736
+00002f60: 3332 3835 3135 3320 3233 382e 3732 3031  3285153 238.7201
+00002f70: 3437 3931 3820 4c20 3338 382e 3730 3936  47918 L 388.7096
+00002f80: 3535 3239 3238 3531 3535 2032 3534 2e35  5529285155 254.5
+00002f90: 3532 3732 3935 3738 204c 2033 3838 2e37  52729578 L 388.7
+00002fa0: 3039 3635 3532 3932 3835 3135 3520 3239  0965529285155 29
+00002fb0: 362e 3737 3239 3437 3333 3820 4c20 3137  6.772947338 L 17
+00002fc0: 2e35 3931 3735 3734 3030 3030 3030 3032  .591757400000002
+00002fd0: 2032 3936 2e37 3732 3934 3733 3338 204c   296.772947338 L
+00002fe0: 2031 372e 3539 3137 3537 3430 3030 3030   17.591757400000
+00002ff0: 3030 3220 3233 382e 3732 3031 3437 3931  002 238.72014791
+00003000: 3820 4d20 3337 322e 3837 3730 3733 3633  8 M 372.87707363
+00003010: 3238 3531 3533 2032 3338 2e37 3230 3134  285153 238.72014
+00003020: 3739 3138 204c 2033 3732 2e38 3737 3037  7918 L 372.87707
+00003030: 3336 3332 3835 3135 3320 3235 342e 3535  363285153 254.55
+00003040: 3237 3239 3537 3820 4c20 3338 382e 3730  2729578 L 388.70
+00003050: 3936 3535 3239 3238 3531 3535 2032 3534  965529285155 254
+00003060: 2e35 3532 3732 3935 3738 2220 7374 726f  .552729578" stro
+00003070: 6b65 2d6d 6974 6572 6c69 6d69 743d 2231  ke-miterlimit="1
+00003080: 3022 2073 7472 6f6b 652d 7769 6474 683d  0" stroke-width=
+00003090: 2231 2e34 3635 3937 3937 3833 3333 3333  "1.4659797833333
+000030a0: 3333 3222 2073 7472 6f6b 652d 6461 7368  332" stroke-dash
+000030b0: 6172 7261 793d 2222 2f3e 3c67 3e3c 7465  array=""/><g><te
+000030c0: 7874 2066 696c 6c3d 2262 6c61 636b 2220  xt fill="black" 
+000030d0: 7374 726f 6b65 3d22 6e6f 6e65 2220 666f  stroke="none" fo
+000030e0: 6e74 2d66 616d 696c 793d 2273 616e 732d  nt-family="sans-
+000030f0: 7365 7269 6622 2066 6f6e 742d 7369 7a65  serif" font-size
+00003100: 3d22 3131 7074 2220 666f 6e74 2d73 7479  ="11pt" font-sty
+00003110: 6c65 3d22 6e6f 726d 616c 2220 666f 6e74  le="normal" font
+00003120: 2d77 6569 6768 743d 226e 6f72 6d61 6c22  -weight="normal"
+00003130: 2074 6578 742d 6465 636f 7261 7469 6f6e   text-decoration
+00003140: 3d22 6e6f 726d 616c 2220 783d 2234 322e  ="normal" x="42.
+00003150: 3232 3032 3137 3736 2220 793d 2232 3633  22021776" y="263
+00003160: 2e33 3438 3630 3832 3738 2220 7465 7874  .348608278" text
+00003170: 2d61 6e63 686f 723d 2273 7461 7274 2220  -anchor="start" 
+00003180: 646f 6d69 6e61 6e74 2d62 6173 656c 696e  dominant-baselin
+00003190: 653d 2261 6c70 6861 6265 7469 6322 2078  e="alphabetic" x
+000031a0: 6d6c 3a73 7061 6365 3d22 7072 6573 6572  ml:space="preser
+000031b0: 7665 223e 41c2 a051 7565 7279 7365 74c2  ve">A..Queryset.
+000031c0: a069 6e73 7461 6e63 65c2 a063 616e c2a0  .instance..can..
+000031d0: 6265 c2a0 7061 7373 6564 c2a0 696e 746f  be..passed..into
+000031e0: c2a0 6578 706f 7274 2829 2e3c 2f74 6578  ..export().</tex
+000031f0: 743e 3c74 6578 7420 6669 6c6c 3d22 626c  t><text fill="bl
+00003200: 6163 6b22 2073 7472 6f6b 653d 226e 6f6e  ack" stroke="non
+00003210: 6522 2066 6f6e 742d 6661 6d69 6c79 3d22  e" font-family="
+00003220: 7361 6e73 2d73 6572 6966 2220 666f 6e74  sans-serif" font
+00003230: 2d73 697a 653d 2231 3170 7422 2066 6f6e  -size="11pt" fon
+00003240: 742d 7374 796c 653d 226e 6f72 6d61 6c22  t-style="normal"
+00003250: 2066 6f6e 742d 7765 6967 6874 3d22 6e6f   font-weight="no
+00003260: 726d 616c 2220 7465 7874 2d64 6563 6f72  rmal" text-decor
+00003270: 6174 696f 6e3d 226e 6f72 6d61 6c22 2078  ation="normal" x
+00003280: 3d22 3432 2e32 3230 3231 3737 3622 2079  ="42.22021776" y
+00003290: 3d22 3238 302e 3934 3033 3635 3637 3822  ="280.940365678"
+000032a0: 2074 6578 742d 616e 6368 6f72 3d22 7374   text-anchor="st
+000032b0: 6172 7422 2064 6f6d 696e 616e 742d 6261  art" dominant-ba
+000032c0: 7365 6c69 6e65 3d22 616c 7068 6162 6574  seline="alphabet
+000032d0: 6963 2220 786d 6c3a 7370 6163 653d 2270  ic" xml:space="p
+000032e0: 7265 7365 7276 6522 3e49 66c2 a06e 6fc2  reserve">If..no.
+000032f0: a051 7565 7279 7365 74c2 a069 73c2 a070  .Queryset..is..p
+00003300: 6173 7365 642c c2a0 6765 745f 7175 6572  assed,..get_quer
+00003310: 7973 6574 2829 c2a0 6973 c2a0 6361 6c6c  yset()..is..call
+00003320: 6564 2e3c 2f74 6578 743e 3c2f 673e 3c67  ed.</text></g><g
+00003330: 3e3c 673e 3c72 6563 7420 6669 6c6c 3d22  ><g><rect fill="
+00003340: 7768 6974 6522 2073 7472 6f6b 653d 226e  white" stroke="n
+00003350: 6f6e 6522 2078 3d22 3234 312e 3535 3933  one" x="241.5593
+00003360: 3736 3636 3937 3539 3122 2079 3d22 3332  766697591" y="32
+00003370: 332e 3136 3035 3833 3433 3822 2077 6964  3.160583438" wid
+00003380: 7468 3d22 3132 382e 3834 3232 3234 3438  th="128.84222448
+00003390: 3536 3235 2220 6865 6967 6874 3d22 3232  5625" height="22
+000033a0: 2e38 3639 3238 3436 3222 2f3e 3c2f 673e  .86928462"/></g>
+000033b0: 3c67 3e3c 7265 6374 2066 696c 6c3d 2279  <g><rect fill="y
+000033c0: 656c 6c6f 7722 2073 7472 6f6b 653d 226e  ellow" stroke="n
+000033d0: 6f6e 6522 2078 3d22 3234 342e 3139 3831  one" x="244.1981
+000033e0: 3430 3237 3937 3539 3132 2220 793d 2233  4027975912" y="3
+000033f0: 3235 2e39 3735 3236 3436 3232 2220 7769  25.975264622" wi
+00003400: 6474 683d 2231 3233 2e35 3634 3639 3732  dth="123.5646972
+00003410: 3635 3632 3522 2068 6569 6768 743d 2231  65625" height="1
+00003420: 372e 3736 3736 3734 3937 3422 2f3e 3c74  7.767674974"/><t
+00003430: 6578 7420 6669 6c6c 3d22 626c 6163 6b22  ext fill="black"
+00003440: 2073 7472 6f6b 653d 226e 6f6e 6522 2066   stroke="none" f
+00003450: 6f6e 742d 6661 6d69 6c79 3d22 6d6f 6e6f  ont-family="mono
+00003460: 7370 6163 6522 2066 6f6e 742d 7369 7a65  space" font-size
+00003470: 3d22 3131 7074 2220 666f 6e74 2d73 7479  ="11pt" font-sty
+00003480: 6c65 3d22 6e6f 726d 616c 2220 666f 6e74  le="normal" font
+00003490: 2d77 6569 6768 743d 226e 6f72 6d61 6c22  -weight="normal"
+000034a0: 2074 6578 742d 6465 636f 7261 7469 6f6e   text-decoration
+000034b0: 3d22 6e6f 726d 616c 2220 783d 2232 3434  ="normal" x="244
+000034c0: 2e31 3938 3134 3032 3739 3735 3931 3222  .19814027975912"
+000034d0: 2079 3d22 3333 382e 3939 3331 3635 3039   y="338.99316509
+000034e0: 3822 2074 6578 742d 616e 6368 6f72 3d22  8" text-anchor="
+000034f0: 7374 6172 7422 2064 6f6d 696e 616e 742d  start" dominant-
+00003500: 6261 7365 6c69 6e65 3d22 616c 7068 6162  baseline="alphab
+00003510: 6574 6963 2220 786d 6c3a 7370 6163 653d  etic" xml:space=
+00003520: 2270 7265 7365 7276 6522 3e67 6574 5f71  "preserve">get_q
+00003530: 7565 7279 7365 7428 293c 2f74 6578 743e  ueryset()</text>
+00003540: 3c2f 673e 3c67 3e3c 7061 7468 2066 696c  </g><g><path fil
+00003550: 6c3d 226e 6f6e 6522 2073 7472 6f6b 653d  l="none" stroke=
+00003560: 2262 6c61 636b 2220 7061 696e 742d 6f72  "black" paint-or
+00003570: 6465 723d 2266 696c 6c20 7374 726f 6b65  der="fill stroke
+00003580: 206d 6172 6b65 7273 2220 643d 2220 4d20   markers" d=" M 
+00003590: 3231 312e 3934 3635 3835 3034 3634 3235  211.946585046425
+000035a0: 3738 2033 3436 2e30 3239 3836 3830 3538  78 346.029868058
+000035b0: 3030 3030 3320 4c20 3239 312e 3130 3934  00003 L 291.1094
+000035c0: 3933 3334 3634 3235 3820 3334 362e 3032  933464258 346.02
+000035d0: 3938 3638 3035 3830 3030 3033 204c 2032  986805800003 L 2
+000035e0: 3931 2e31 3039 3439 3333 3436 3432 3538  91.1094933464258
+000035f0: 2033 3638 2e38 3939 3135 3236 3738 204c   368.899152678 L
+00003600: 2032 3335 2e32 3236 3334 3430 3035 3735   235.22634400575
+00003610: 3931 3320 3336 382e 3839 3931 3532 3637  913 368.89915267
+00003620: 3822 2073 7472 6f6b 652d 6d69 7465 726c  8" stroke-miterl
+00003630: 696d 6974 3d22 3130 2220 7374 726f 6b65  imit="10" stroke
+00003640: 2d77 6964 7468 3d22 312e 3436 3539 3739  -width="1.465979
+00003650: 3738 3333 3333 3333 3332 2220 7374 726f  7833333332" stro
+00003660: 6b65 2d64 6173 6861 7272 6179 3d22 222f  ke-dasharray=""/
+00003670: 3e3c 6720 7472 616e 7366 6f72 6d3d 2274  ><g transform="t
+00003680: 7261 6e73 6c61 7465 2832 3230 2e37 3432  ranslate(220.742
+00003690: 3436 3337 3436 3432 3537 382c 3336 382e  46374642578,368.
+000036a0: 3839 3931 3532 3637 3829 2074 7261 6e73  899152678) trans
+000036b0: 6c61 7465 282d 3232 302e 3734 3234 3633  late(-220.742463
+000036c0: 3734 3634 3235 3738 2c2d 3336 382e 3839  74642578,-368.89
+000036d0: 3931 3532 3637 3829 223e 3c70 6174 6820  9152678)"><path 
+000036e0: 6669 6c6c 3d22 626c 6163 6b22 2073 7472  fill="black" str
+000036f0: 6f6b 653d 226e 6f6e 6522 2070 6169 6e74  oke="none" paint
+00003700: 2d6f 7264 6572 3d22 7374 726f 6b65 2066  -order="stroke f
+00003710: 696c 6c20 6d61 726b 6572 7322 2064 3d22  ill markers" d="
+00003720: 204d 2032 3335 2e34 3032 3236 3135 3739   M 235.402261579
+00003730: 3735 3931 2033 3631 2e35 3639 3235 3337  7591 361.5692537
+00003740: 3631 3333 3333 3620 4c20 3232 302e 3734  6133336 L 220.74
+00003750: 3234 3633 3734 3634 3235 3738 2033 3638  246374642578 368
+00003760: 2e38 3939 3135 3236 3738 204c 2032 3335  .899152678 L 235
+00003770: 2e34 3032 3236 3135 3739 3735 3931 2033  .4022615797591 3
+00003780: 3736 2e32 3239 3035 3135 3934 3636 3636  76.2290515946666
+00003790: 3620 5a22 2f3e 3c2f 673e 3c2f 673e 3c67  6 Z"/></g></g><g
+000037a0: 3e3c 673e 3c72 6563 7420 6669 6c6c 3d22  ><g><rect fill="
+000037b0: 7768 6974 6522 2073 7472 6f6b 653d 226e  white" stroke="n
+000037c0: 6f6e 6522 2078 3d22 3234 312e 3535 3933  one" x="241.5593
+000037d0: 3736 3636 3937 3539 3122 2079 3d22 3339  766697591" y="39
+000037e0: 352e 3238 3637 3838 3737 3822 2077 6964  5.286788778" wid
+000037f0: 7468 3d22 3735 2e38 3835 3932 3536 3537  th="75.885925657
+00003800: 3522 2068 6569 6768 743d 2232 322e 3836  5" height="22.86
+00003810: 3932 3834 3632 222f 3e3c 2f67 3e3c 7465  928462"/></g><te
+00003820: 7874 2066 696c 6c3d 2262 6c61 636b 2220  xt fill="black" 
+00003830: 7374 726f 6b65 3d22 6e6f 6e65 2220 666f  stroke="none" fo
+00003840: 6e74 2d66 616d 696c 793d 226d 6f6e 6f73  nt-family="monos
+00003850: 7061 6365 2220 666f 6e74 2d73 697a 653d  pace" font-size=
+00003860: 2231 3170 7422 2066 6f6e 742d 7374 796c  "11pt" font-styl
+00003870: 653d 226e 6f72 6d61 6c22 2066 6f6e 742d  e="normal" font-
+00003880: 7765 6967 6874 3d22 6e6f 726d 616c 2220  weight="normal" 
+00003890: 7465 7874 2d64 6563 6f72 6174 696f 6e3d  text-decoration=
+000038a0: 226e 6f72 6d61 6c22 2078 3d22 3234 342e  "normal" x="244.
+000038b0: 3139 3831 3430 3237 3937 3539 3132 2220  19814027975912" 
+000038c0: 793d 2234 3131 2e31 3139 3337 3034 3338  y="411.119370438
+000038d0: 3030 3030 3322 2074 6578 742d 616e 6368  00003" text-anch
+000038e0: 6f72 3d22 7374 6172 7422 2064 6f6d 696e  or="start" domin
+000038f0: 616e 742d 6261 7365 6c69 6e65 3d22 616c  ant-baseline="al
+00003900: 7068 6162 6574 6963 2220 786d 6c3a 7370  phabetic" xml:sp
+00003910: 6163 653d 2270 7265 7365 7276 6522 3e51  ace="preserve">Q
+00003920: 7565 7279 7365 743c 2f74 6578 743e 3c2f  ueryset</text></
+00003930: 673e 3c67 3e3c 7061 7468 2066 696c 6c3d  g><g><path fill=
+00003940: 226e 6f6e 6522 2073 7472 6f6b 653d 2262  "none" stroke="b
+00003950: 6c61 636b 2220 7061 696e 742d 6f72 6465  lack" paint-orde
+00003960: 723d 2266 696c 6c20 7374 726f 6b65 206d  r="fill stroke m
+00003970: 6172 6b65 7273 2220 643d 2220 4d20 3232  arkers" d=" M 22
+00003980: 302e 3734 3234 3633 3734 3634 3235 3738  0.74246374642578
+00003990: 2034 3138 2e31 3536 3037 3333 3938 3030   418.15607339800
+000039a0: 3030 3520 4c20 3239 312e 3130 3934 3933  005 L 291.109493
+000039b0: 3334 3634 3235 3820 3431 382e 3135 3630  3464258 418.1560
+000039c0: 3733 3339 3830 3030 3035 204c 2032 3931  7339800005 L 291
+000039d0: 2e31 3039 3439 3333 3436 3432 3538 2034  .1094933464258 4
+000039e0: 3431 2e30 3235 3335 3830 3138 204c 2032  41.025358018 L 2
+000039f0: 3236 2e34 3330 3436 3533 3035 3735 3931  26.4304653057591
+00003a00: 3320 3434 312e 3032 3533 3538 3031 3822  3 441.025358018"
+00003a10: 2073 7472 6f6b 652d 6d69 7465 726c 696d   stroke-miterlim
+00003a20: 6974 3d22 3130 2220 7374 726f 6b65 2d77  it="10" stroke-w
+00003a30: 6964 7468 3d22 312e 3436 3539 3739 3738  idth="1.46597978
+00003a40: 3333 3333 3333 3332 2220 7374 726f 6b65  33333332" stroke
+00003a50: 2d64 6173 6861 7272 6179 3d22 372e 3033  -dasharray="7.03
+00003a60: 3637 3032 3935 3939 3939 3939 3935 222f  67029599999995"/
+00003a70: 3e3c 6720 7472 616e 7366 6f72 6d3d 2274  ><g transform="t
+00003a80: 7261 6e73 6c61 7465 2832 3131 2e39 3436  ranslate(211.946
+00003a90: 3538 3530 3436 3432 3537 382c 3434 312e  58504642578,441.
+00003aa0: 3032 3533 3538 3031 3829 2074 7261 6e73  025358018) trans
+00003ab0: 6c61 7465 282d 3231 312e 3934 3635 3835  late(-211.946585
+00003ac0: 3034 3634 3235 3738 2c2d 3434 312e 3032  04642578,-441.02
+00003ad0: 3533 3538 3031 3829 223e 3c70 6174 6820  5358018)"><path 
+00003ae0: 6669 6c6c 3d22 626c 6163 6b22 2073 7472  fill="black" str
+00003af0: 6f6b 653d 226e 6f6e 6522 2070 6169 6e74  oke="none" paint
+00003b00: 2d6f 7264 6572 3d22 7374 726f 6b65 2066  -order="stroke f
+00003b10: 696c 6c20 6d61 726b 6572 7322 2064 3d22  ill markers" d="
+00003b20: 204d 2032 3236 2e36 3036 3338 3238 3739   M 226.606382879
+00003b30: 3735 3931 2034 3333 2e36 3935 3435 3931  7591 433.6954591
+00003b40: 3031 3333 3333 3720 4c20 3231 312e 3934  0133337 L 211.94
+00003b50: 3635 3835 3034 3634 3235 3738 2034 3431  658504642578 441
+00003b60: 2e30 3235 3335 3830 3138 204c 2032 3236  .025358018 L 226
+00003b70: 2e36 3036 3338 3238 3739 3735 3931 2034  .6063828797591 4
+00003b80: 3438 2e33 3535 3235 3639 3334 3636 3636  48.3552569346666
+00003b90: 3720 5a22 2f3e 3c2f 673e 3c2f 673e 3c67  7 Z"/></g></g><g
+00003ba0: 3e3c 673e 3c72 6563 7420 6669 6c6c 3d22  ><g><rect fill="
+00003bb0: 7768 6974 6522 2073 7472 6f6b 653d 226e  white" stroke="n
+00003bc0: 6f6e 6522 2078 3d22 3234 312e 3535 3933  one" x="241.5593
+00003bd0: 3736 3636 3937 3539 3122 2079 3d22 3436  766697591" y="46
+00003be0: 372e 3431 3239 3934 3131 3822 2077 6964  7.412994118" wid
+00003bf0: 7468 3d22 3239 362e 3533 3731 3730 3737  th="296.53717077
+00003c00: 3436 3837 3522 2068 6569 6768 743d 2232  46875" height="2
+00003c10: 322e 3836 3932 3834 3632 222f 3e3c 2f67  2.86928462"/></g
+00003c20: 3e3c 673e 3c72 6563 7420 6669 6c6c 3d22  ><g><rect fill="
+00003c30: 7965 6c6c 6f77 2220 7374 726f 6b65 3d22  yellow" stroke="
+00003c40: 6e6f 6e65 2220 783d 2232 3434 2e31 3938  none" x="244.198
+00003c50: 3134 3032 3739 3735 3931 3222 2079 3d22  14027975912" y="
+00003c60: 3437 302e 3232 3736 3735 3330 3139 3939  470.227675301999
+00003c70: 3937 2220 7769 6474 683d 2232 3931 2e32  97" width="291.2
+00003c80: 3539 3634 3335 3534 3638 3735 2220 6865  596435546875" he
+00003c90: 6967 6874 3d22 3137 2e37 3637 3637 3439  ight="17.7676749
+00003ca0: 3734 222f 3e3c 7465 7874 2066 696c 6c3d  74"/><text fill=
+00003cb0: 2262 6c61 636b 2220 7374 726f 6b65 3d22  "black" stroke="
+00003cc0: 6e6f 6e65 2220 666f 6e74 2d66 616d 696c  none" font-famil
+00003cd0: 793d 226d 6f6e 6f73 7061 6365 2220 666f  y="monospace" fo
+00003ce0: 6e74 2d73 697a 653d 2231 3170 7422 2066  nt-size="11pt" f
+00003cf0: 6f6e 742d 7374 796c 653d 226e 6f72 6d61  ont-style="norma
+00003d00: 6c22 2066 6f6e 742d 7765 6967 6874 3d22  l" font-weight="
+00003d10: 6e6f 726d 616c 2220 7465 7874 2d64 6563  normal" text-dec
+00003d20: 6f72 6174 696f 6e3d 226e 6f72 6d61 6c22  oration="normal"
+00003d30: 2078 3d22 3234 342e 3139 3831 3430 3237   x="244.19814027
+00003d40: 3937 3539 3132 2220 793d 2234 3833 2e32  975912" y="483.2
+00003d50: 3435 3537 3537 3738 2220 7465 7874 2d61  45575778" text-a
+00003d60: 6e63 686f 723d 2273 7461 7274 2220 646f  nchor="start" do
+00003d70: 6d69 6e61 6e74 2d62 6173 656c 696e 653d  minant-baseline=
+00003d80: 2261 6c70 6861 6265 7469 6322 2078 6d6c  "alphabetic" xml
+00003d90: 3a73 7061 6365 3d22 7072 6573 6572 7665  :space="preserve
+00003da0: 223e 6669 6c74 6572 5f65 7870 6f72 7428  ">filter_export(
+00003db0: 7175 6572 7973 6574 2cc2 a02a 2a6b 7761  queryset,..**kwa
+00003dc0: 7267 7329 3c2f 7465 7874 3e3c 2f67 3e3c  rgs)</text></g><
+00003dd0: 673e 3c70 6174 6820 6669 6c6c 3d22 6e6f  g><path fill="no
+00003de0: 6e65 2220 7374 726f 6b65 3d22 626c 6163  ne" stroke="blac
+00003df0: 6b22 2070 6169 6e74 2d6f 7264 6572 3d22  k" paint-order="
+00003e00: 6669 6c6c 2073 7472 6f6b 6520 6d61 726b  fill stroke mark
+00003e10: 6572 7322 2064 3d22 204d 2032 3131 2e39  ers" d=" M 211.9
+00003e20: 3436 3538 3530 3436 3432 3537 3820 3439  4658504642578 49
+00003e30: 302e 3238 3232 3738 3733 3820 4c20 3239  0.282278738 L 29
+00003e40: 312e 3130 3934 3933 3334 3634 3235 3820  1.1094933464258 
+00003e50: 3439 302e 3238 3232 3738 3733 3820 4c20  490.282278738 L 
+00003e60: 3239 312e 3130 3934 3933 3334 3634 3235  291.109493346425
+00003e70: 3820 3531 332e 3135 3135 3633 3335 3820  8 513.151563358 
+00003e80: 4c20 3233 352e 3232 3633 3434 3030 3537  L 235.2263440057
+00003e90: 3539 3133 2035 3133 2e31 3531 3536 3333  5913 513.1515633
+00003ea0: 3538 2220 7374 726f 6b65 2d6d 6974 6572  58" stroke-miter
+00003eb0: 6c69 6d69 743d 2231 3022 2073 7472 6f6b  limit="10" strok
+00003ec0: 652d 7769 6474 683d 2231 2e34 3635 3937  e-width="1.46597
+00003ed0: 3937 3833 3333 3333 3333 3222 2073 7472  97833333332" str
+00003ee0: 6f6b 652d 6461 7368 6172 7261 793d 2222  oke-dasharray=""
+00003ef0: 2f3e 3c67 2074 7261 6e73 666f 726d 3d22  /><g transform="
+00003f00: 7472 616e 736c 6174 6528 3232 302e 3734  translate(220.74
+00003f10: 3234 3633 3734 3634 3235 3738 2c35 3133  246374642578,513
+00003f20: 2e31 3531 3536 3333 3538 2920 7472 616e  .151563358) tran
+00003f30: 736c 6174 6528 2d32 3230 2e37 3432 3436  slate(-220.74246
+00003f40: 3337 3436 3432 3537 382c 2d35 3133 2e31  374642578,-513.1
+00003f50: 3531 3536 3333 3538 2922 3e3c 7061 7468  51563358)"><path
+00003f60: 2066 696c 6c3d 2262 6c61 636b 2220 7374   fill="black" st
+00003f70: 726f 6b65 3d22 6e6f 6e65 2220 7061 696e  roke="none" pain
+00003f80: 742d 6f72 6465 723d 2273 7472 6f6b 6520  t-order="stroke 
+00003f90: 6669 6c6c 206d 6172 6b65 7273 2220 643d  fill markers" d=
+00003fa0: 2220 4d20 3233 352e 3430 3232 3631 3537  " M 235.40226157
+00003fb0: 3937 3539 3120 3530 352e 3832 3136 3634  97591 505.821664
+00003fc0: 3434 3133 3333 3320 4c20 3232 302e 3734  4413333 L 220.74
+00003fd0: 3234 3633 3734 3634 3235 3738 2035 3133  246374642578 513
+00003fe0: 2e31 3531 3536 3333 3538 204c 2032 3335  .151563358 L 235
+00003ff0: 2e34 3032 3236 3135 3739 3735 3931 2035  .4022615797591 5
+00004000: 3230 2e34 3831 3436 3232 3734 3636 3637  20.4814622746667
+00004010: 205a 222f 3e3c 2f67 3e3c 2f67 3e3c 673e   Z"/></g></g><g>
+00004020: 3c67 3e3c 7265 6374 2066 696c 6c3d 2277  <g><rect fill="w
+00004030: 6869 7465 2220 7374 726f 6b65 3d22 6e6f  hite" stroke="no
+00004040: 6e65 2220 783d 2232 3431 2e35 3539 3337  ne" x="241.55937
+00004050: 3636 3639 3735 3931 2220 793d 2235 3339  66697591" y="539
+00004060: 2e35 3339 3139 3934 3538 2220 7769 6474  .539199458" widt
+00004070: 683d 2237 352e 3838 3539 3235 3635 3735  h="75.8859256575
+00004080: 2220 6865 6967 6874 3d22 3232 2e38 3639  " height="22.869
+00004090: 3238 3436 3222 2f3e 3c2f 673e 3c74 6578  28462"/></g><tex
+000040a0: 7420 6669 6c6c 3d22 626c 6163 6b22 2073  t fill="black" s
+000040b0: 7472 6f6b 653d 226e 6f6e 6522 2066 6f6e  troke="none" fon
+000040c0: 742d 6661 6d69 6c79 3d22 6d6f 6e6f 7370  t-family="monosp
+000040d0: 6163 6522 2066 6f6e 742d 7369 7a65 3d22  ace" font-size="
+000040e0: 3131 7074 2220 666f 6e74 2d73 7479 6c65  11pt" font-style
+000040f0: 3d22 6e6f 726d 616c 2220 666f 6e74 2d77  ="normal" font-w
+00004100: 6569 6768 743d 226e 6f72 6d61 6c22 2074  eight="normal" t
+00004110: 6578 742d 6465 636f 7261 7469 6f6e 3d22  ext-decoration="
+00004120: 6e6f 726d 616c 2220 783d 2232 3434 2e31  normal" x="244.1
+00004130: 3938 3134 3032 3739 3735 3931 3222 2079  9814027975912" y
+00004140: 3d22 3535 352e 3337 3137 3831 3131 3822  ="555.371781118"
+00004150: 2074 6578 742d 616e 6368 6f72 3d22 7374   text-anchor="st
+00004160: 6172 7422 2064 6f6d 696e 616e 742d 6261  art" dominant-ba
+00004170: 7365 6c69 6e65 3d22 616c 7068 6162 6574  seline="alphabet
+00004180: 6963 2220 786d 6c3a 7370 6163 653d 2270  ic" xml:space="p
+00004190: 7265 7365 7276 6522 3e51 7565 7279 7365  reserve">Queryse
+000041a0: 743c 2f74 6578 743e 3c2f 673e 3c67 3e3c  t</text></g><g><
+000041b0: 7061 7468 2066 696c 6c3d 226e 6f6e 6522  path fill="none"
+000041c0: 2073 7472 6f6b 653d 2262 6c61 636b 2220   stroke="black" 
+000041d0: 7061 696e 742d 6f72 6465 723d 2266 696c  paint-order="fil
+000041e0: 6c20 7374 726f 6b65 206d 6172 6b65 7273  l stroke markers
+000041f0: 2220 643d 2220 4d20 3232 302e 3734 3234  " d=" M 220.7424
+00004200: 3633 3734 3634 3235 3738 2035 3632 2e34  6374642578 562.4
+00004210: 3038 3438 3430 3737 3939 3939 204c 2032  084840779999 L 2
+00004220: 3931 2e31 3039 3439 3333 3436 3432 3538  91.1094933464258
+00004230: 2035 3632 2e34 3038 3438 3430 3737 3939   562.40848407799
+00004240: 3939 204c 2032 3931 2e31 3039 3439 3333  99 L 291.1094933
+00004250: 3436 3432 3538 2035 3835 2e32 3737 3736  464258 585.27776
+00004260: 3836 3937 3939 3939 204c 2032 3236 2e34  86979999 L 226.4
+00004270: 3330 3436 3533 3035 3735 3931 3320 3538  3046530575913 58
+00004280: 352e 3237 3737 3638 3639 3739 3939 3922  5.2777686979999"
+00004290: 2073 7472 6f6b 652d 6d69 7465 726c 696d   stroke-miterlim
+000042a0: 6974 3d22 3130 2220 7374 726f 6b65 2d77  it="10" stroke-w
+000042b0: 6964 7468 3d22 312e 3436 3539 3739 3738  idth="1.46597978
+000042c0: 3333 3333 3333 3332 2220 7374 726f 6b65  33333332" stroke
+000042d0: 2d64 6173 6861 7272 6179 3d22 372e 3033  -dasharray="7.03
+000042e0: 3637 3032 3935 3939 3939 3939 3935 222f  67029599999995"/
+000042f0: 3e3c 6720 7472 616e 7366 6f72 6d3d 2274  ><g transform="t
+00004300: 7261 6e73 6c61 7465 2832 3131 2e39 3436  ranslate(211.946
+00004310: 3538 3530 3436 3432 3537 382c 3538 352e  58504642578,585.
+00004320: 3237 3737 3638 3639 3739 3939 3929 2074  2777686979999) t
+00004330: 7261 6e73 6c61 7465 282d 3231 312e 3934  ranslate(-211.94
+00004340: 3635 3835 3034 3634 3235 3738 2c2d 3538  658504642578,-58
+00004350: 352e 3237 3737 3638 3639 3739 3939 3929  5.2777686979999)
+00004360: 223e 3c70 6174 6820 6669 6c6c 3d22 626c  "><path fill="bl
+00004370: 6163 6b22 2073 7472 6f6b 653d 226e 6f6e  ack" stroke="non
+00004380: 6522 2070 6169 6e74 2d6f 7264 6572 3d22  e" paint-order="
+00004390: 7374 726f 6b65 2066 696c 6c20 6d61 726b  stroke fill mark
+000043a0: 6572 7322 2064 3d22 204d 2032 3236 2e36  ers" d=" M 226.6
+000043b0: 3036 3338 3238 3739 3735 3931 2035 3737  063828797591 577
+000043c0: 2e39 3437 3836 3937 3831 3333 3332 204c  .9478697813332 L
+000043d0: 2032 3131 2e39 3436 3538 3530 3436 3432   211.94658504642
+000043e0: 3537 3820 3538 352e 3237 3737 3638 3639  578 585.27776869
+000043f0: 3739 3939 3920 4c20 3232 362e 3630 3633  79999 L 226.6063
+00004400: 3832 3837 3937 3539 3120 3539 322e 3630  828797591 592.60
+00004410: 3736 3637 3631 3436 3636 3620 5a22 2f3e  76676146666 Z"/>
+00004420: 3c2f 673e 3c2f 673e 3c67 3e3c 673e 3c72  </g></g><g><g><r
+00004430: 6563 7420 6669 6c6c 3d22 7267 6228 3235  ect fill="rgb(25
+00004440: 352c 3234 322c 3234 3529 2220 7374 726f  5,242,245)" stro
+00004450: 6b65 3d22 6e6f 6e65 2220 783d 2232 3431  ke="none" x="241
+00004460: 2e35 3539 3337 3636 3639 3735 3931 2220  .5593766697591" 
+00004470: 793d 2236 3539 2e31 3633 3134 3937 3737  y="659.163149777
+00004480: 3939 3939 2220 7769 6474 683d 2232 3235  9999" width="225
+00004490: 2e39 3238 3737 3233 3337 3138 3735 2220  .9287723371875" 
+000044a0: 6865 6967 6874 3d22 3232 2e38 3639 3238  height="22.86928
+000044b0: 3436 3222 2f3e 3c2f 673e 3c67 3e3c 7265  462"/></g><g><re
+000044c0: 6374 2066 696c 6c3d 2279 656c 6c6f 7722  ct fill="yellow"
+000044d0: 2073 7472 6f6b 653d 226e 6f6e 6522 2078   stroke="none" x
+000044e0: 3d22 3234 342e 3139 3831 3430 3237 3937  ="244.1981402797
+000044f0: 3539 3132 2220 793d 2236 3631 2e39 3737  5912" y="661.977
+00004500: 3833 3039 3631 3939 3939 2220 7769 6474  8309619999" widt
+00004510: 683d 2232 3230 2e36 3531 3234 3531 3137  h="220.651245117
+00004520: 3138 3735 2220 6865 6967 6874 3d22 3137  1875" height="17
+00004530: 2e37 3637 3637 3439 3734 222f 3e3c 7465  .767674974"/><te
+00004540: 7874 2066 696c 6c3d 2262 6c61 636b 2220  xt fill="black" 
+00004550: 7374 726f 6b65 3d22 6e6f 6e65 2220 666f  stroke="none" fo
+00004560: 6e74 2d66 616d 696c 793d 226d 6f6e 6f73  nt-family="monos
+00004570: 7061 6365 2220 666f 6e74 2d73 697a 653d  pace" font-size=
+00004580: 2231 3170 7422 2066 6f6e 742d 7374 796c  "11pt" font-styl
+00004590: 653d 226e 6f72 6d61 6c22 2066 6f6e 742d  e="normal" font-
+000045a0: 7765 6967 6874 3d22 6e6f 726d 616c 2220  weight="normal" 
+000045b0: 7465 7874 2d64 6563 6f72 6174 696f 6e3d  text-decoration=
+000045c0: 226e 6f72 6d61 6c22 2078 3d22 3234 342e  "normal" x="244.
+000045d0: 3139 3831 3430 3237 3937 3539 3132 2220  19814027975912" 
+000045e0: 793d 2236 3734 2e39 3935 3733 3134 3337  y="674.995731437
+000045f0: 3939 3939 2220 7465 7874 2d61 6e63 686f  9999" text-ancho
+00004600: 723d 2273 7461 7274 2220 646f 6d69 6e61  r="start" domina
+00004610: 6e74 2d62 6173 656c 696e 653d 2261 6c70  nt-baseline="alp
+00004620: 6861 6265 7469 6322 2078 6d6c 3a73 7061  habetic" xml:spa
+00004630: 6365 3d22 7072 6573 6572 7665 223e 6578  ce="preserve">ex
+00004640: 706f 7274 5f72 6573 6f75 7263 6528 696e  port_resource(in
+00004650: 7374 616e 6365 293c 2f74 6578 743e 3c2f  stance)</text></
+00004660: 673e 3c67 3e3c 7061 7468 2066 696c 6c3d  g><g><path fill=
+00004670: 226e 6f6e 6522 2073 7472 6f6b 653d 2262  "none" stroke="b
+00004680: 6c61 636b 2220 7061 696e 742d 6f72 6465  lack" paint-orde
+00004690: 723d 2266 696c 6c20 7374 726f 6b65 206d  r="fill stroke m
+000046a0: 6172 6b65 7273 2220 643d 2220 4d20 3231  arkers" d=" M 21
+000046b0: 312e 3934 3635 3835 3034 3634 3235 3738  1.94658504642578
+000046c0: 2036 3832 2e30 3332 3433 3433 3937 3939   682.03243439799
+000046d0: 3939 204c 2032 3931 2e31 3039 3439 3333  99 L 291.1094933
+000046e0: 3436 3432 3538 2036 3832 2e30 3332 3433  464258 682.03243
+000046f0: 3433 3937 3939 3939 204c 2032 3931 2e31  43979999 L 291.1
+00004700: 3039 3439 3333 3436 3432 3538 2037 3034  094933464258 704
+00004710: 2e39 3031 3731 3930 3137 3939 3939 204c  .9017190179999 L
+00004720: 2032 3335 2e32 3236 3334 3430 3035 3735   235.22634400575
+00004730: 3931 3320 3730 342e 3930 3137 3139 3031  913 704.90171901
+00004740: 3739 3939 3922 2073 7472 6f6b 652d 6d69  79999" stroke-mi
+00004750: 7465 726c 696d 6974 3d22 3130 2220 7374  terlimit="10" st
+00004760: 726f 6b65 2d77 6964 7468 3d22 312e 3436  roke-width="1.46
+00004770: 3539 3739 3738 3333 3333 3333 3332 2220  59797833333332" 
+00004780: 7374 726f 6b65 2d64 6173 6861 7272 6179  stroke-dasharray
+00004790: 3d22 222f 3e3c 6720 7472 616e 7366 6f72  =""/><g transfor
+000047a0: 6d3d 2274 7261 6e73 6c61 7465 2832 3230  m="translate(220
+000047b0: 2e37 3432 3436 3337 3436 3432 3537 382c  .74246374642578,
+000047c0: 3730 342e 3930 3137 3139 3031 3739 3939  704.901719017999
+000047d0: 3929 2074 7261 6e73 6c61 7465 282d 3232  9) translate(-22
+000047e0: 302e 3734 3234 3633 3734 3634 3235 3738  0.74246374642578
+000047f0: 2c2d 3730 342e 3930 3137 3139 3031 3739  ,-704.9017190179
+00004800: 3939 3929 223e 3c70 6174 6820 6669 6c6c  999)"><path fill
+00004810: 3d22 626c 6163 6b22 2073 7472 6f6b 653d  ="black" stroke=
+00004820: 226e 6f6e 6522 2070 6169 6e74 2d6f 7264  "none" paint-ord
+00004830: 6572 3d22 7374 726f 6b65 2066 696c 6c20  er="stroke fill 
+00004840: 6d61 726b 6572 7322 2064 3d22 204d 2032  markers" d=" M 2
+00004850: 3335 2e34 3032 3236 3135 3739 3735 3931  35.4022615797591
+00004860: 2036 3937 2e35 3731 3832 3031 3031 3333   697.57182010133
+00004870: 3332 204c 2032 3230 2e37 3432 3436 3337  32 L 220.7424637
+00004880: 3436 3432 3537 3820 3730 342e 3930 3137  4642578 704.9017
+00004890: 3139 3031 3739 3939 3920 4c20 3233 352e  190179999 L 235.
+000048a0: 3430 3232 3631 3537 3937 3539 3120 3731  4022615797591 71
+000048b0: 322e 3233 3136 3137 3933 3436 3636 3620  2.2316179346666 
+000048c0: 5a22 2f3e 3c2f 673e 3c2f 673e 3c67 3e3c  Z"/></g></g><g><
+000048d0: 673e 3c72 6563 7420 6669 6c6c 3d22 7267  g><rect fill="rg
+000048e0: 6228 3230 342c 3233 302c 3230 3429 2220  b(204,230,204)" 
+000048f0: 7374 726f 6b65 3d22 6e6f 6e65 2220 783d  stroke="none" x=
+00004900: 2232 3530 2e33 3535 3235 3533 3639 3735  "250.35525536975
+00004910: 3931 2220 793d 2237 3738 2e37 3837 3130  91" y="778.78710
+00004920: 3030 3937 3939 3939 2220 7769 6474 683d  00979999" width=
+00004930: 2232 3631 2e32 3332 3937 3135 3535 3933  "261.23297155593
+00004940: 3735 2220 6865 6967 6874 3d22 3232 2e38  75" height="22.8
+00004950: 3639 3238 3436 3222 2f3e 3c2f 673e 3c74  6928462"/></g><t
+00004960: 6578 7420 6669 6c6c 3d22 626c 6163 6b22  ext fill="black"
+00004970: 2073 7472 6f6b 653d 226e 6f6e 6522 2066   stroke="none" f
+00004980: 6f6e 742d 6661 6d69 6c79 3d22 6d6f 6e6f  ont-family="mono
+00004990: 7370 6163 6522 2066 6f6e 742d 7369 7a65  space" font-size
+000049a0: 3d22 3131 7074 2220 666f 6e74 2d73 7479  ="11pt" font-sty
+000049b0: 6c65 3d22 6e6f 726d 616c 2220 666f 6e74  le="normal" font
+000049c0: 2d77 6569 6768 743d 226e 6f72 6d61 6c22  -weight="normal"
+000049d0: 2074 6578 742d 6465 636f 7261 7469 6f6e   text-decoration
+000049e0: 3d22 6e6f 726d 616c 2220 783d 2232 3532  ="normal" x="252
+000049f0: 2e39 3934 3031 3839 3739 3735 3931 3222  .99401897975912"
+00004a00: 2079 3d22 3739 342e 3631 3936 3831 3735   y="794.61968175
+00004a10: 3739 3939 3822 2074 6578 742d 616e 6368  79998" text-anch
+00004a20: 6f72 3d22 7374 6172 7422 2064 6f6d 696e  or="start" domin
+00004a30: 616e 742d 6261 7365 6c69 6e65 3d22 616c  ant-baseline="al
+00004a40: 7068 6162 6574 6963 2220 786d 6c3a 7370  phabetic" xml:sp
+00004a50: 6163 653d 2270 7265 7365 7276 6522 3e65  ace="preserve">e
+00004a60: 7870 6f72 745f 6669 656c 6428 6669 656c  xport_field(fiel
+00004a70: 642c c2a0 696e 7374 616e 6365 293c 2f74  d,..instance)</t
+00004a80: 6578 743e 3c2f 673e 3c67 3e3c 7061 7468  ext></g><g><path
+00004a90: 2066 696c 6c3d 226e 6f6e 6522 2073 7472   fill="none" str
+00004aa0: 6f6b 653d 2262 6c61 636b 2220 7061 696e  oke="black" pain
+00004ab0: 742d 6f72 6465 723d 2266 696c 6c20 7374  t-order="fill st
+00004ac0: 726f 6b65 206d 6172 6b65 7273 2220 643d  roke markers" d=
+00004ad0: 2220 4d20 3232 302e 3734 3234 3633 3734  " M 220.74246374
+00004ae0: 3634 3235 3738 2038 3031 2e36 3536 3338  642578 801.65638
+00004af0: 3437 3137 3939 3938 204c 2032 3939 2e39  47179998 L 299.9
+00004b00: 3035 3337 3230 3436 3432 3538 2038 3031  053720464258 801
+00004b10: 2e36 3536 3338 3437 3137 3939 3938 204c  .6563847179998 L
+00004b20: 2032 3939 2e39 3035 3337 3230 3436 3432   299.90537204642
+00004b30: 3538 2038 3234 2e35 3235 3636 3933 3337  58 824.525669337
+00004b40: 3939 3938 204c 2032 3434 2e30 3232 3232  9998 L 244.02222
+00004b50: 3237 3035 3735 3931 3320 3832 342e 3532  270575913 824.52
+00004b60: 3536 3639 3333 3739 3939 3822 2073 7472  56693379998" str
+00004b70: 6f6b 652d 6d69 7465 726c 696d 6974 3d22  oke-miterlimit="
+00004b80: 3130 2220 7374 726f 6b65 2d77 6964 7468  10" stroke-width
+00004b90: 3d22 312e 3436 3539 3739 3738 3333 3333  ="1.465979783333
+00004ba0: 3333 3332 2220 7374 726f 6b65 2d64 6173  3332" stroke-das
+00004bb0: 6861 7272 6179 3d22 222f 3e3c 6720 7472  harray=""/><g tr
+00004bc0: 616e 7366 6f72 6d3d 2274 7261 6e73 6c61  ansform="transla
+00004bd0: 7465 2832 3239 2e35 3338 3334 3234 3436  te(229.538342446
+00004be0: 3432 3538 2c38 3234 2e35 3235 3636 3933  4258,824.5256693
+00004bf0: 3337 3939 3938 2920 7472 616e 736c 6174  379998) translat
+00004c00: 6528 2d32 3239 2e35 3338 3334 3234 3436  e(-229.538342446
+00004c10: 3432 3538 2c2d 3832 342e 3532 3536 3639  4258,-824.525669
+00004c20: 3333 3739 3939 3829 223e 3c70 6174 6820  3379998)"><path 
+00004c30: 6669 6c6c 3d22 626c 6163 6b22 2073 7472  fill="black" str
+00004c40: 6f6b 653d 226e 6f6e 6522 2070 6169 6e74  oke="none" paint
+00004c50: 2d6f 7264 6572 3d22 7374 726f 6b65 2066  -order="stroke f
+00004c60: 696c 6c20 6d61 726b 6572 7322 2064 3d22  ill markers" d="
+00004c70: 204d 2032 3434 2e31 3938 3134 3032 3739   M 244.198140279
+00004c80: 3735 3931 3220 3831 372e 3139 3537 3730  75912 817.195770
+00004c90: 3432 3133 3333 3120 4c20 3232 392e 3533  4213331 L 229.53
+00004ca0: 3833 3432 3434 3634 3235 3820 3832 342e  83424464258 824.
+00004cb0: 3532 3536 3639 3333 3739 3939 3820 4c20  5256693379998 L 
+00004cc0: 3234 342e 3139 3831 3430 3237 3937 3539  244.198140279759
+00004cd0: 3132 2038 3331 2e38 3535 3536 3832 3534  12 831.855568254
+00004ce0: 3636 3635 205a 222f 3e3c 2f67 3e3c 2f67  6665 Z"/></g></g
+00004cf0: 3e3c 673e 3c67 3e3c 7265 6374 2066 696c  ><g><g><rect fil
+00004d00: 6c3d 2272 6762 2832 3034 2c32 3330 2c32  l="rgb(204,230,2
+00004d10: 3034 2922 2073 7472 6f6b 653d 226e 6f6e  04)" stroke="non
+00004d20: 6522 2078 3d22 3334 302e 3131 3139 3034  e" x="340.111904
+00004d30: 3330 3436 3534 3936 2220 793d 2238 3530  30465496" y="850
+00004d40: 2e39 3133 3330 3534 3337 3939 3938 2220  .9133054379998" 
+00004d50: 7769 6474 683d 2231 3436 2e34 3934 3332  width="146.49432
+00004d60: 3430 3935 2220 6865 6967 6874 3d22 3232  4095" height="22
+00004d70: 2e38 3639 3238 3436 3222 2f3e 3c2f 673e  .86928462"/></g>
+00004d80: 3c74 6578 7420 6669 6c6c 3d22 626c 6163  <text fill="blac
+00004d90: 6b22 2073 7472 6f6b 653d 226e 6f6e 6522  k" stroke="none"
+00004da0: 2066 6f6e 742d 6661 6d69 6c79 3d22 6d6f   font-family="mo
+00004db0: 6e6f 7370 6163 6522 2066 6f6e 742d 7369  nospace" font-si
+00004dc0: 7a65 3d22 3131 7074 2220 666f 6e74 2d73  ze="11pt" font-s
+00004dd0: 7479 6c65 3d22 6e6f 726d 616c 2220 666f  tyle="normal" fo
+00004de0: 6e74 2d77 6569 6768 743d 226e 6f72 6d61  nt-weight="norma
+00004df0: 6c22 2074 6578 742d 6465 636f 7261 7469  l" text-decorati
+00004e00: 6f6e 3d22 6e6f 726d 616c 2220 783d 2233  on="normal" x="3
+00004e10: 3432 2e37 3530 3636 3739 3134 3635 3439  42.7506679146549
+00004e20: 3722 2079 3d22 3836 362e 3734 3538 3837  7" y="866.745887
+00004e30: 3039 3739 3939 3822 2074 6578 742d 616e  0979998" text-an
+00004e40: 6368 6f72 3d22 7374 6172 7422 2064 6f6d  chor="start" dom
+00004e50: 696e 616e 742d 6261 7365 6c69 6e65 3d22  inant-baseline="
+00004e60: 616c 7068 6162 6574 6963 2220 786d 6c3a  alphabetic" xml:
+00004e70: 7370 6163 653d 2270 7265 7365 7276 6522  space="preserve"
+00004e80: 3e65 7870 6f72 7428 696e 7374 616e 6365  >export(instance
+00004e90: 293c 2f74 6578 743e 3c2f 673e 3c67 3e3c  )</text></g><g><
+00004ea0: 7061 7468 2066 696c 6c3d 226e 6f6e 6522  path fill="none"
+00004eb0: 2073 7472 6f6b 653d 2262 6c61 636b 2220   stroke="black" 
+00004ec0: 7061 696e 742d 6f72 6465 723d 2266 696c  paint-order="fil
+00004ed0: 6c20 7374 726f 6b65 206d 6172 6b65 7273  l stroke markers
+00004ee0: 2220 643d 2220 4d20 3232 392e 3533 3833  " d=" M 229.5383
+00004ef0: 3432 3434 3634 3235 3820 3837 332e 3738  424464258 873.78
+00004f00: 3235 3930 3035 3739 3939 3920 4c20 3538  25900579999 L 58
+00004f10: 322e 3639 3539 3039 3939 3835 3530 3920  2.6959099985509 
+00004f20: 3837 332e 3738 3235 3930 3035 3739 3939  873.782590057999
+00004f30: 3922 2073 7472 6f6b 652d 6d69 7465 726c  9" stroke-miterl
+00004f40: 696d 6974 3d22 3130 2220 7374 726f 6b65  imit="10" stroke
+00004f50: 2d77 6964 7468 3d22 312e 3436 3539 3739  -width="1.465979
+00004f60: 3738 3333 3333 3333 3332 2220 7374 726f  7833333332" stro
+00004f70: 6b65 2d64 6173 6861 7272 6179 3d22 222f  ke-dasharray=""/
+00004f80: 3e3c 6720 7472 616e 7366 6f72 6d3d 2274  ><g transform="t
+00004f90: 7261 6e73 6c61 7465 2835 3937 2e31 3739  ranslate(597.179
+00004fa0: 3739 3032 3537 3838 3432 2c38 3733 2e37  7902578842,873.7
+00004fb0: 3832 3539 3030 3537 3939 3939 2920 7472  825900579999) tr
+00004fc0: 616e 736c 6174 6528 2d35 3937 2e31 3739  anslate(-597.179
+00004fd0: 3739 3032 3537 3838 3432 2c2d 3837 332e  7902578842,-873.
+00004fe0: 3738 3235 3930 3035 3739 3939 3929 223e  7825900579999)">
+00004ff0: 3c70 6174 6820 6669 6c6c 3d22 626c 6163  <path fill="blac
+00005000: 6b22 2073 7472 6f6b 653d 226e 6f6e 6522  k" stroke="none"
+00005010: 2070 6169 6e74 2d6f 7264 6572 3d22 7374   paint-order="st
+00005020: 726f 6b65 2066 696c 6c20 6d61 726b 6572  roke fill marker
+00005030: 7322 2064 3d22 204d 2035 3832 2e35 3139  s" d=" M 582.519
+00005040: 3939 3234 3234 3535 3039 2038 3636 2e34  9924245509 866.4
+00005050: 3532 3639 3131 3431 3333 3332 204c 2035  526911413332 L 5
+00005060: 3937 2e31 3739 3739 3032 3537 3838 3432  97.1797902578842
+00005070: 2038 3733 2e37 3832 3539 3030 3537 3939   873.78259005799
+00005080: 3939 204c 2035 3832 2e35 3139 3939 3234  99 L 582.5199924
+00005090: 3234 3535 3039 2038 3831 2e31 3132 3438  245509 881.11248
+000050a0: 3839 3734 3636 3636 205a 222f 3e3c 2f67  89746666 Z"/></g
+000050b0: 3e3c 2f67 3e3c 7061 7468 2066 696c 6c3d  ></g><path fill=
+000050c0: 2277 6869 7465 2220 7374 726f 6b65 3d22  "white" stroke="
+000050d0: 626c 6163 6b22 2070 6169 6e74 2d6f 7264  black" paint-ord
+000050e0: 6572 3d22 6669 6c6c 2073 7472 6f6b 6520  er="fill stroke 
+000050f0: 6d61 726b 6572 7322 2064 3d22 204d 2034  markers" d=" M 4
+00005100: 3034 2e34 3936 3839 3733 3138 3538 3733  04.4968973185873
+00005110: 3420 3930 302e 3137 3032 3236 3135 3739  4 900.1702261579
+00005120: 3939 3820 4c20 3739 312e 3632 3138 3538  998 L 791.621858
+00005130: 3933 3731 3831 3120 3930 302e 3137 3032  9371811 900.1702
+00005140: 3236 3135 3739 3939 3820 4c20 3830 372e  261579998 L 807.
+00005150: 3435 3434 3430 3539 3731 3831 2039 3136  454440597181 916
+00005160: 2e30 3032 3830 3738 3137 3939 3937 204c  .0028078179997 L
+00005170: 2038 3037 2e34 3534 3434 3035 3937 3138   807.45444059718
+00005180: 3120 3935 382e 3232 3330 3235 3537 3739  1 958.2230255779
+00005190: 3939 3820 4c20 3430 342e 3439 3638 3937  998 L 404.496897
+000051a0: 3331 3835 3837 3334 2039 3538 2e32 3233  31858734 958.223
+000051b0: 3032 3535 3737 3939 3938 204c 2034 3034  0255779998 L 404
+000051c0: 2e34 3936 3839 3733 3138 3538 3733 3420  .49689731858734 
+000051d0: 3930 302e 3137 3032 3236 3135 3739 3939  900.170226157999
+000051e0: 3820 4d20 3739 312e 3632 3138 3538 3933  8 M 791.62185893
+000051f0: 3731 3831 3120 3930 302e 3137 3032 3236  71811 900.170226
+00005200: 3135 3739 3939 3820 4c20 3739 312e 3632  1579998 L 791.62
+00005210: 3138 3538 3933 3731 3831 3120 3931 362e  18589371811 916.
+00005220: 3030 3238 3037 3831 3739 3939 3720 4c20  0028078179997 L 
+00005230: 3830 372e 3435 3434 3430 3539 3731 3831  807.454440597181
+00005240: 2039 3136 2e30 3032 3830 3738 3137 3939   916.00280781799
+00005250: 3937 2220 7374 726f 6b65 2d6d 6974 6572  97" stroke-miter
+00005260: 6c69 6d69 743d 2231 3022 2073 7472 6f6b  limit="10" strok
+00005270: 652d 7769 6474 683d 2231 2e34 3635 3937  e-width="1.46597
+00005280: 3937 3833 3333 3333 3333 3222 2073 7472  97833333332" str
+00005290: 6f6b 652d 6461 7368 6172 7261 793d 2222  oke-dasharray=""
+000052a0: 2f3e 3c67 3e3c 7465 7874 2066 696c 6c3d  /><g><text fill=
+000052b0: 2262 6c61 636b 2220 7374 726f 6b65 3d22  "black" stroke="
+000052c0: 6e6f 6e65 2220 666f 6e74 2d66 616d 696c  none" font-famil
+000052d0: 793d 2273 616e 732d 7365 7269 6622 2066  y="sans-serif" f
+000052e0: 6f6e 742d 7369 7a65 3d22 3131 7074 2220  ont-size="11pt" 
+000052f0: 666f 6e74 2d73 7479 6c65 3d22 6e6f 726d  font-style="norm
+00005300: 616c 2220 666f 6e74 2d77 6569 6768 743d  al" font-weight=
+00005310: 226e 6f72 6d61 6c22 2074 6578 742d 6465  "normal" text-de
+00005320: 636f 7261 7469 6f6e 3d22 6e6f 726d 616c  coration="normal
+00005330: 2220 783d 2234 3239 2e31 3235 3335 3736  " x="429.1253576
+00005340: 3738 3538 3733 2220 793d 2239 3234 2e37  785873" y="924.7
+00005350: 3938 3638 3635 3137 3939 3938 2220 7465  986865179998" te
+00005360: 7874 2d61 6e63 686f 723d 2273 7461 7274  xt-anchor="start
+00005370: 2220 646f 6d69 6e61 6e74 2d62 6173 656c  " dominant-basel
+00005380: 696e 653d 2261 6c70 6861 6265 7469 6322  ine="alphabetic"
+00005390: 2078 6d6c 3a73 7061 6365 3d22 7072 6573   xml:space="pres
+000053a0: 6572 7665 223e 416e c2a0 6f70 7469 6f6e  erve">An..option
+000053b0: 616c c2a0 6361 6c6c 6162 6c65 c2a0 6361  al..callable..ca
+000053c0: 6ec2 a062 65c2 a064 6566 696e 6564 c2a0  n..be..defined..
+000053d0: 696e 7374 6561 64c2 a06f 66c2 a065 7870  instead..of..exp
+000053e0: 6f72 7428 292e 3c2f 7465 7874 3e3c 7465  ort().</text><te
+000053f0: 7874 2066 696c 6c3d 2262 6c61 636b 2220  xt fill="black" 
+00005400: 7374 726f 6b65 3d22 6e6f 6e65 2220 666f  stroke="none" fo
+00005410: 6e74 2d66 616d 696c 793d 2273 616e 732d  nt-family="sans-
+00005420: 7365 7269 6622 2066 6f6e 742d 7369 7a65  serif" font-size
+00005430: 3d22 3131 7074 2220 666f 6e74 2d73 7479  ="11pt" font-sty
+00005440: 6c65 3d22 6e6f 726d 616c 2220 666f 6e74  le="normal" font
+00005450: 2d77 6569 6768 743d 226e 6f72 6d61 6c22  -weight="normal"
+00005460: 2074 6578 742d 6465 636f 7261 7469 6f6e   text-decoration
+00005470: 3d22 6e6f 726d 616c 2220 783d 2234 3239  ="normal" x="429
+00005480: 2e31 3235 3335 3736 3738 3538 3733 2220  .1253576785873" 
+00005490: 793d 2239 3432 2e33 3930 3434 3339 3137  y="942.390443917
+000054a0: 3939 3938 2220 7465 7874 2d61 6e63 686f  9998" text-ancho
+000054b0: 723d 2273 7461 7274 2220 646f 6d69 6e61  r="start" domina
+000054c0: 6e74 2d62 6173 656c 696e 653d 2261 6c70  nt-baseline="alp
+000054d0: 6861 6265 7469 6322 2078 6d6c 3a73 7061  habetic" xml:spa
+000054e0: 6365 3d22 7072 6573 6572 7665 223e c2a0  ce="preserve">..
+000054f0: 5365 65c2 a027 6465 6879 6472 6174 6527  See..'dehydrate'
+00005500: c2a0 6d65 7468 6f64 73c2 a069 6ec2 a064  ..methods..in..d
+00005510: 6f63 732e 3c2f 7465 7874 3e3c 2f67 3e3c  ocs.</text></g><
+00005520: 673e 3c67 3e3c 7265 6374 2066 696c 6c3d  g><g><rect fill=
+00005530: 2272 6762 2832 3034 2c32 3330 2c32 3034  "rgb(204,230,204
+00005540: 2922 2073 7472 6f6b 653d 226e 6f6e 6522  )" stroke="none"
+00005550: 2078 3d22 3634 342e 3338 3433 3339 3238   x="644.38433928
+00005560: 3132 3137 3522 2079 3d22 3938 342e 3631  12175" y="984.61
+00005570: 3036 3631 3637 3739 3939 3922 2077 6964  06616779999" wid
+00005580: 7468 3d22 3137 322e 3937 3234 3733 3530  th="172.97247350
+00005590: 3930 3632 3522 2068 6569 6768 743d 2232  90625" height="2
+000055a0: 322e 3836 3932 3834 3632 222f 3e3c 2f67  2.86928462"/></g
+000055b0: 3e3c 7465 7874 2066 696c 6c3d 2262 6c61  ><text fill="bla
+000055c0: 636b 2220 7374 726f 6b65 3d22 6e6f 6e65  ck" stroke="none
+000055d0: 2220 666f 6e74 2d66 616d 696c 793d 226d  " font-family="m
+000055e0: 6f6e 6f73 7061 6365 2220 666f 6e74 2d73  onospace" font-s
+000055f0: 697a 653d 2231 3170 7422 2066 6f6e 742d  ize="11pt" font-
+00005600: 7374 796c 653d 226e 6f72 6d61 6c22 2066  style="normal" f
+00005610: 6f6e 742d 7765 6967 6874 3d22 6e6f 726d  ont-weight="norm
+00005620: 616c 2220 7465 7874 2d64 6563 6f72 6174  al" text-decorat
+00005630: 696f 6e3d 226e 6f72 6d61 6c22 2078 3d22  ion="normal" x="
+00005640: 3634 372e 3032 3331 3032 3839 3132 3137  647.023102891217
+00005650: 3522 2079 3d22 3130 3030 2e34 3433 3234  5" y="1000.44324
+00005660: 3333 3337 3939 3939 2220 7465 7874 2d61  33379999" text-a
+00005670: 6e63 686f 723d 2273 7461 7274 2220 646f  nchor="start" do
+00005680: 6d69 6e61 6e74 2d62 6173 656c 696e 653d  minant-baseline=
+00005690: 2261 6c70 6861 6265 7469 6322 2078 6d6c  "alphabetic" xml
+000056a0: 3a73 7061 6365 3d22 7072 6573 6572 7665  :space="preserve
+000056b0: 223e 6765 745f 7661 6c75 6528 696e 7374  ">get_value(inst
+000056c0: 616e 6365 293c 2f74 6578 743e 3c2f 673e  ance)</text></g>
+000056d0: 3c67 3e3c 7061 7468 2066 696c 6c3d 226e  <g><path fill="n
+000056e0: 6f6e 6522 2073 7472 6f6b 653d 2262 6c61  one" stroke="bla
+000056f0: 636b 2220 7061 696e 742d 6f72 6465 723d  ck" paint-order=
+00005700: 2266 696c 6c20 7374 726f 6b65 206d 6172  "fill stroke mar
+00005710: 6b65 7273 2220 643d 2220 4d20 3631 342e  kers" d=" M 614.
+00005720: 3737 3135 3437 3635 3738 3834 3220 3130  7715476578842 10
+00005730: 3037 2e34 3739 3934 3632 3937 3939 3938  07.4799462979998
+00005740: 204c 2036 3933 2e39 3334 3435 3539 3537   L 693.934455957
+00005750: 3838 3432 2031 3030 372e 3437 3939 3436  8842 1007.479946
+00005760: 3239 3739 3939 3820 4c20 3639 332e 3933  2979998 L 693.93
+00005770: 3434 3535 3935 3738 3834 3220 3130 3330  44559578842 1030
+00005780: 2e33 3439 3233 3039 3137 3939 3939 204c  .3492309179999 L
+00005790: 2036 3338 2e30 3531 3330 3636 3137 3231   638.05130661721
+000057a0: 3735 2031 3033 302e 3334 3932 3330 3931  75 1030.34923091
+000057b0: 3739 3939 3922 2073 7472 6f6b 652d 6d69  79999" stroke-mi
+000057c0: 7465 726c 696d 6974 3d22 3130 2220 7374  terlimit="10" st
+000057d0: 726f 6b65 2d77 6964 7468 3d22 312e 3436  roke-width="1.46
+000057e0: 3539 3739 3738 3333 3333 3333 3332 2220  59797833333332" 
+000057f0: 7374 726f 6b65 2d64 6173 6861 7272 6179  stroke-dasharray
+00005800: 3d22 222f 3e3c 6720 7472 616e 7366 6f72  =""/><g transfor
+00005810: 6d3d 2274 7261 6e73 6c61 7465 2836 3233  m="translate(623
+00005820: 2e35 3637 3432 3633 3537 3838 3432 2c31  .5674263578842,1
+00005830: 3033 302e 3334 3932 3330 3931 3739 3939  030.349230917999
+00005840: 3929 2074 7261 6e73 6c61 7465 282d 3632  9) translate(-62
+00005850: 332e 3536 3734 3236 3335 3738 3834 322c  3.5674263578842,
+00005860: 2d31 3033 302e 3334 3932 3330 3931 3739  -1030.3492309179
+00005870: 3939 3929 223e 3c70 6174 6820 6669 6c6c  999)"><path fill
+00005880: 3d22 626c 6163 6b22 2073 7472 6f6b 653d  ="black" stroke=
+00005890: 226e 6f6e 6522 2070 6169 6e74 2d6f 7264  "none" paint-ord
+000058a0: 6572 3d22 7374 726f 6b65 2066 696c 6c20  er="stroke fill 
+000058b0: 6d61 726b 6572 7322 2064 3d22 204d 2036  markers" d=" M 6
+000058c0: 3338 2e32 3237 3232 3431 3931 3231 3735  38.2272241912175
+000058d0: 2031 3032 332e 3031 3933 3332 3030 3133   1023.0193320013
+000058e0: 3333 3220 4c20 3632 332e 3536 3734 3236  332 L 623.567426
+000058f0: 3335 3738 3834 3220 3130 3330 2e33 3439  3578842 1030.349
+00005900: 3233 3039 3137 3939 3939 204c 2036 3338  2309179999 L 638
+00005910: 2e32 3237 3232 3431 3931 3231 3735 2031  .2272241912175 1
+00005920: 3033 372e 3637 3931 3239 3833 3436 3636  037.679129834666
+00005930: 3620 5a22 2f3e 3c2f 673e 3c2f 673e 3c70  6 Z"/></g></g><p
+00005940: 6174 6820 6669 6c6c 3d22 7768 6974 6522  ath fill="white"
+00005950: 2073 7472 6f6b 653d 2262 6c61 636b 2220   stroke="black" 
+00005960: 7061 696e 742d 6f72 6465 723d 2266 696c  paint-order="fil
+00005970: 6c20 7374 726f 6b65 206d 6172 6b65 7273  l stroke markers
+00005980: 2220 643d 2220 4d20 3435 362e 3930 3230  " d=" M 456.9020
+00005990: 3138 3136 3831 3936 3720 3130 3536 2e37  181681967 1056.7
+000059a0: 3336 3836 3730 3137 3939 3939 204c 2037  368670179999 L 7
+000059b0: 3339 2e32 3136 3733 3830 3837 3537 3137  39.2167380875717
+000059c0: 2031 3035 362e 3733 3638 3637 3031 3739   1056.7368670179
+000059d0: 3939 3920 4c20 3735 352e 3034 3933 3139  999 L 755.049319
+000059e0: 3734 3735 3731 3620 3130 3732 2e35 3639  7475716 1072.569
+000059f0: 3434 3836 3737 3939 3938 204c 2037 3535  4486779998 L 755
+00005a00: 2e30 3439 3331 3937 3437 3537 3136 2031  .0493197475716 1
+00005a10: 3039 372e 3139 3739 3039 3033 3739 3939  097.197909037999
+00005a20: 3820 4c20 3435 362e 3930 3230 3138 3136  8 L 456.90201816
+00005a30: 3831 3936 3720 3130 3937 2e31 3937 3930  81967 1097.19790
+00005a40: 3930 3337 3939 3938 204c 2034 3536 2e39  90379998 L 456.9
+00005a50: 3032 3031 3831 3638 3139 3637 2031 3035  020181681967 105
+00005a60: 362e 3733 3638 3637 3031 3739 3939 3920  6.7368670179999 
+00005a70: 4d20 3733 392e 3231 3637 3338 3038 3735  M 739.2167380875
+00005a80: 3731 3720 3130 3536 2e37 3336 3836 3730  717 1056.7368670
+00005a90: 3137 3939 3939 204c 2037 3339 2e32 3136  179999 L 739.216
+00005aa0: 3733 3830 3837 3537 3137 2031 3037 322e  7380875717 1072.
+00005ab0: 3536 3934 3438 3637 3739 3939 3820 4c20  5694486779998 L 
+00005ac0: 3735 352e 3034 3933 3139 3734 3735 3731  755.049319747571
+00005ad0: 3620 3130 3732 2e35 3639 3434 3836 3737  6 1072.569448677
+00005ae0: 3939 3938 2220 7374 726f 6b65 2d6d 6974  9998" stroke-mit
+00005af0: 6572 6c69 6d69 743d 2231 3022 2073 7472  erlimit="10" str
+00005b00: 6f6b 652d 7769 6474 683d 2231 2e34 3635  oke-width="1.465
+00005b10: 3937 3937 3833 3333 3333 3333 3222 2073  9797833333332" s
+00005b20: 7472 6f6b 652d 6461 7368 6172 7261 793d  troke-dasharray=
+00005b30: 2222 2f3e 3c67 3e3c 7465 7874 2066 696c  ""/><g><text fil
+00005b40: 6c3d 2262 6c61 636b 2220 7374 726f 6b65  l="black" stroke
+00005b50: 3d22 6e6f 6e65 2220 666f 6e74 2d66 616d  ="none" font-fam
+00005b60: 696c 793d 2273 616e 732d 7365 7269 6622  ily="sans-serif"
+00005b70: 2066 6f6e 742d 7369 7a65 3d22 3131 7074   font-size="11pt
+00005b80: 2220 666f 6e74 2d73 7479 6c65 3d22 6e6f  " font-style="no
+00005b90: 726d 616c 2220 666f 6e74 2d77 6569 6768  rmal" font-weigh
+00005ba0: 743d 226e 6f72 6d61 6c22 2074 6578 742d  t="normal" text-
+00005bb0: 6465 636f 7261 7469 6f6e 3d22 6e6f 726d  decoration="norm
+00005bc0: 616c 2220 783d 2234 3831 2e35 3330 3437  al" x="481.53047
+00005bd0: 3835 3238 3139 3637 2220 793d 2231 3038  85281967" y="108
+00005be0: 312e 3336 3533 3237 3337 3739 3939 3622  1.3653273779996"
+00005bf0: 2074 6578 742d 616e 6368 6f72 3d22 7374   text-anchor="st
+00005c00: 6172 7422 2064 6f6d 696e 616e 742d 6261  art" dominant-ba
+00005c10: 7365 6c69 6e65 3d22 616c 7068 6162 6574  seline="alphabet
+00005c20: 6963 2220 786d 6c3a 7370 6163 653d 2270  ic" xml:space="p
+00005c30: 7265 7365 7276 6522 3e47 6574 c2a0 7468  reserve">Get..th
+00005c40: 65c2 a066 6965 6c64 2773 c2a0 7661 6c75  e..field's..valu
+00005c50: 65c2 a066 726f 6dc2 a074 6865 c2a0 696e  e..from..the..in
+00005c60: 7374 616e 6365 2e3c 2f74 6578 743e 3c2f  stance.</text></
+00005c70: 673e 3c67 3e3c 673e 3c72 6563 7420 6669  g><g><g><rect fi
+00005c80: 6c6c 3d22 7267 6228 3230 342c 3233 302c  ll="rgb(204,230,
+00005c90: 3230 3429 2220 7374 726f 6b65 3d22 6e6f  204)" stroke="no
+00005ca0: 6e65 2220 783d 2236 3434 2e33 3834 3333  ne" x="644.38433
+00005cb0: 3932 3831 3231 3735 2220 793d 2231 3132  92812175" y="112
+00005cc0: 332e 3538 3535 3435 3133 3739 3939 3822  3.5855451379998"
+00005cd0: 2077 6964 7468 3d22 3834 2e37 3131 3937   width="84.71197
+00005ce0: 3534 3632 3138 3735 2220 6865 6967 6874  54621875" height
+00005cf0: 3d22 3232 2e38 3639 3238 3436 3222 2f3e  ="22.86928462"/>
+00005d00: 3c2f 673e 3c74 6578 7420 6669 6c6c 3d22  </g><text fill="
+00005d10: 626c 6163 6b22 2073 7472 6f6b 653d 226e  black" stroke="n
+00005d20: 6f6e 6522 2066 6f6e 742d 6661 6d69 6c79  one" font-family
+00005d30: 3d22 6d6f 6e6f 7370 6163 6522 2066 6f6e  ="monospace" fon
+00005d40: 742d 7369 7a65 3d22 3131 7074 2220 666f  t-size="11pt" fo
+00005d50: 6e74 2d73 7479 6c65 3d22 6e6f 726d 616c  nt-style="normal
+00005d60: 2220 666f 6e74 2d77 6569 6768 743d 226e  " font-weight="n
+00005d70: 6f72 6d61 6c22 2074 6578 742d 6465 636f  ormal" text-deco
+00005d80: 7261 7469 6f6e 3d22 6e6f 726d 616c 2220  ration="normal" 
+00005d90: 783d 2236 3437 2e30 3233 3130 3238 3931  x="647.023102891
+00005da0: 3231 3735 2220 793d 2231 3133 392e 3431  2175" y="1139.41
+00005db0: 3831 3236 3739 3739 3939 3822 2074 6578  81267979998" tex
+00005dc0: 742d 616e 6368 6f72 3d22 7374 6172 7422  t-anchor="start"
+00005dd0: 2064 6f6d 696e 616e 742d 6261 7365 6c69   dominant-baseli
+00005de0: 6e65 3d22 616c 7068 6162 6574 6963 2220  ne="alphabetic" 
+00005df0: 786d 6c3a 7370 6163 653d 2270 7265 7365  xml:space="prese
+00005e00: 7276 6522 3e26 6c74 3b26 6c74 3b76 616c  rve">&lt;&lt;val
+00005e10: 7565 2667 743b 2667 743b 3c2f 7465 7874  ue&gt;&gt;</text
+00005e20: 3e3c 2f67 3e3c 673e 3c70 6174 6820 6669  ></g><g><path fi
+00005e30: 6c6c 3d22 6e6f 6e65 2220 7374 726f 6b65  ll="none" stroke
+00005e40: 3d22 626c 6163 6b22 2070 6169 6e74 2d6f  ="black" paint-o
+00005e50: 7264 6572 3d22 6669 6c6c 2073 7472 6f6b  rder="fill strok
+00005e60: 6520 6d61 726b 6572 7322 2064 3d22 204d  e markers" d=" M
+00005e70: 2036 3233 2e35 3637 3432 3633 3537 3838   623.56742635788
+00005e80: 3432 2031 3134 362e 3435 3438 3239 3735  42 1146.45482975
+00005e90: 3820 4c20 3639 332e 3933 3434 3535 3935  8 L 693.93445595
+00005ea0: 3738 3834 3220 3131 3436 2e34 3534 3832  78842 1146.45482
+00005eb0: 3937 3538 204c 2036 3933 2e39 3334 3435  9758 L 693.93445
+00005ec0: 3539 3537 3838 3432 2031 3136 392e 3332  59578842 1169.32
+00005ed0: 3431 3134 3337 3739 3939 3920 4c20 3633  41143779999 L 63
+00005ee0: 382e 3035 3133 3036 3631 3732 3137 3520  8.0513066172175 
+00005ef0: 3131 3639 2e33 3234 3131 3433 3737 3939  1169.32411437799
+00005f00: 3939 2220 7374 726f 6b65 2d6d 6974 6572  99" stroke-miter
+00005f10: 6c69 6d69 743d 2231 3022 2073 7472 6f6b  limit="10" strok
+00005f20: 652d 7769 6474 683d 2231 2e34 3635 3937  e-width="1.46597
+00005f30: 3937 3833 3333 3333 3333 3222 2073 7472  97833333332" str
+00005f40: 6f6b 652d 6461 7368 6172 7261 793d 2237  oke-dasharray="7
+00005f50: 2e30 3336 3730 3239 3539 3939 3939 3939  .036702959999999
+00005f60: 3522 2f3e 3c67 2074 7261 6e73 666f 726d  5"/><g transform
+00005f70: 3d22 7472 616e 736c 6174 6528 3632 332e  ="translate(623.
+00005f80: 3536 3734 3236 3335 3738 3834 322c 3131  5674263578842,11
+00005f90: 3639 2e33 3234 3131 3433 3737 3939 3939  69.3241143779999
+00005fa0: 2920 7472 616e 736c 6174 6528 2d36 3233  ) translate(-623
+00005fb0: 2e35 3637 3432 3633 3537 3838 3432 2c2d  .5674263578842,-
+00005fc0: 3131 3639 2e33 3234 3131 3433 3737 3939  1169.32411437799
+00005fd0: 3939 2922 3e3c 7061 7468 2066 696c 6c3d  99)"><path fill=
+00005fe0: 2262 6c61 636b 2220 7374 726f 6b65 3d22  "black" stroke="
+00005ff0: 6e6f 6e65 2220 7061 696e 742d 6f72 6465  none" paint-orde
+00006000: 723d 2273 7472 6f6b 6520 6669 6c6c 206d  r="stroke fill m
+00006010: 6172 6b65 7273 2220 643d 2220 4d20 3633  arkers" d=" M 63
+00006020: 382e 3232 3732 3234 3139 3132 3137 3520  8.2272241912175 
+00006030: 3131 3631 2e39 3934 3231 3534 3631 3333  1161.99421546133
+00006040: 3332 204c 2036 3233 2e35 3637 3432 3633  32 L 623.5674263
+00006050: 3537 3838 3432 2031 3136 392e 3332 3431  578842 1169.3241
+00006060: 3134 3337 3739 3939 3920 4c20 3633 382e  143779999 L 638.
+00006070: 3232 3732 3234 3139 3132 3137 3520 3131  2272241912175 11
+00006080: 3736 2e36 3534 3031 3332 3934 3636 3636  76.6540132946666
+00006090: 205a 222f 3e3c 2f67 3e3c 2f67 3e3c 673e   Z"/></g></g><g>
+000060a0: 3c67 3e3c 7265 6374 2066 696c 6c3d 2272  <g><rect fill="r
+000060b0: 6762 2832 3034 2c32 3330 2c32 3034 2922  gb(204,230,204)"
+000060c0: 2073 7472 6f6b 653d 226e 6f6e 6522 2078   stroke="none" x
+000060d0: 3d22 3636 382e 3639 3636 3634 3138 3730  ="668.6966641870
+000060e0: 3633 3922 2079 3d22 3131 3935 2e37 3131  639" y="1195.711
+000060f0: 3735 3034 3737 3939 3939 2220 7769 6474  7504779999" widt
+00006100: 683d 2231 3230 2e30 3136 3137 3436 3830  h="120.016174680
+00006110: 3933 3735 2220 6865 6967 6874 3d22 3232  9375" height="22
+00006120: 2e38 3639 3238 3436 3222 2f3e 3c2f 673e  .86928462"/></g>
+00006130: 3c74 6578 7420 6669 6c6c 3d22 626c 6163  <text fill="blac
+00006140: 6b22 2073 7472 6f6b 653d 226e 6f6e 6522  k" stroke="none"
+00006150: 2066 6f6e 742d 6661 6d69 6c79 3d22 6d6f   font-family="mo
+00006160: 6e6f 7370 6163 6522 2066 6f6e 742d 7369  nospace" font-si
+00006170: 7a65 3d22 3131 7074 2220 666f 6e74 2d73  ze="11pt" font-s
+00006180: 7479 6c65 3d22 6e6f 726d 616c 2220 666f  tyle="normal" fo
+00006190: 6e74 2d77 6569 6768 743d 226e 6f72 6d61  nt-weight="norma
+000061a0: 6c22 2074 6578 742d 6465 636f 7261 7469  l" text-decorati
+000061b0: 6f6e 3d22 6e6f 726d 616c 2220 783d 2236  on="normal" x="6
+000061c0: 3731 2e33 3335 3432 3737 3937 3036 3339  71.3354277970639
+000061d0: 2220 793d 2231 3231 312e 3534 3433 3332  " y="1211.544332
+000061e0: 3133 3739 3939 3822 2074 6578 742d 616e  1379998" text-an
+000061f0: 6368 6f72 3d22 7374 6172 7422 2064 6f6d  chor="start" dom
+00006200: 696e 616e 742d 6261 7365 6c69 6e65 3d22  inant-baseline="
+00006210: 616c 7068 6162 6574 6963 2220 786d 6c3a  alphabetic" xml:
+00006220: 7370 6163 653d 2270 7265 7365 7276 6522  space="preserve"
+00006230: 3e72 656e 6465 7228 7661 6c75 6529 3c2f  >render(value)</
+00006240: 7465 7874 3e3c 2f67 3e3c 673e 3c70 6174  text></g><g><pat
+00006250: 6820 6669 6c6c 3d22 6e6f 6e65 2220 7374  h fill="none" st
+00006260: 726f 6b65 3d22 626c 6163 6b22 2070 6169  roke="black" pai
+00006270: 6e74 2d6f 7264 6572 3d22 6669 6c6c 2073  nt-order="fill s
+00006280: 7472 6f6b 6520 6d61 726b 6572 7322 2064  troke markers" d
+00006290: 3d22 204d 2036 3233 2e35 3637 3432 3633  =" M 623.5674263
+000062a0: 3537 3838 3432 2031 3231 382e 3538 3130  578842 1218.5810
+000062b0: 3335 3039 3739 3939 3820 4c20 3831 392e  350979998 L 819.
+000062c0: 3335 3831 3936 3433 3738 3437 3720 3132  3581964378477 12
+000062d0: 3138 2e35 3831 3033 3530 3937 3939 3938  18.5810350979998
+000062e0: 2220 7374 726f 6b65 2d6d 6974 6572 6c69  " stroke-miterli
+000062f0: 6d69 743d 2231 3022 2073 7472 6f6b 652d  mit="10" stroke-
+00006300: 7769 6474 683d 2231 2e34 3635 3937 3937  width="1.4659797
+00006310: 3833 3333 3333 3333 3222 2073 7472 6f6b  833333332" strok
+00006320: 652d 6461 7368 6172 7261 793d 2222 2f3e  e-dasharray=""/>
+00006330: 3c67 2074 7261 6e73 666f 726d 3d22 7472  <g transform="tr
+00006340: 616e 736c 6174 6528 3833 332e 3834 3230  anslate(833.8420
+00006350: 3736 3639 3731 3831 2c31 3231 382e 3538  76697181,1218.58
+00006360: 3130 3335 3039 3739 3939 3829 2074 7261  10350979998) tra
+00006370: 6e73 6c61 7465 282d 3833 332e 3834 3230  nslate(-833.8420
+00006380: 3736 3639 3731 3831 2c2d 3132 3138 2e35  76697181,-1218.5
+00006390: 3831 3033 3530 3937 3939 3938 2922 3e3c  810350979998)"><
+000063a0: 7061 7468 2066 696c 6c3d 2262 6c61 636b  path fill="black
+000063b0: 2220 7374 726f 6b65 3d22 6e6f 6e65 2220  " stroke="none" 
+000063c0: 7061 696e 742d 6f72 6465 723d 2273 7472  paint-order="str
+000063d0: 6f6b 6520 6669 6c6c 206d 6172 6b65 7273  oke fill markers
+000063e0: 2220 643d 2220 4d20 3831 392e 3138 3232  " d=" M 819.1822
+000063f0: 3738 3836 3338 3437 3720 3132 3131 2e32  788638477 1211.2
+00006400: 3531 3133 3631 3831 3333 3320 4c20 3833  51136181333 L 83
+00006410: 332e 3834 3230 3736 3639 3731 3831 2031  3.842076697181 1
+00006420: 3231 382e 3538 3130 3335 3039 3739 3939  218.581035097999
+00006430: 3820 4c20 3831 392e 3138 3232 3738 3836  8 L 819.18227886
+00006440: 3338 3437 3720 3132 3235 2e39 3130 3933  38477 1225.91093
+00006450: 3430 3134 3636 3635 205a 222f 3e3c 2f67  40146665 Z"/></g
+00006460: 3e3c 2f67 3e3c 7061 7468 2066 696c 6c3d  ></g><path fill=
+00006470: 2277 6869 7465 2220 7374 726f 6b65 3d22  "white" stroke="
+00006480: 626c 6163 6b22 2070 6169 6e74 2d6f 7264  black" paint-ord
+00006490: 6572 3d22 6669 6c6c 2073 7472 6f6b 6520  er="fill stroke 
+000064a0: 6d61 726b 6572 7322 2064 3d22 204d 2037  markers" d=" M 7
+000064b0: 3331 2e32 3237 3135 3430 3333 3736 3331  31.2271540337631
+000064c0: 2031 3234 342e 3936 3836 3731 3139 3739   1244.9686711979
+000064d0: 3939 3820 4c20 3933 382e 3231 3631 3735  998 L 938.216175
+000064e0: 3130 3035 3939 3120 3132 3434 2e39 3638  1005991 1244.968
+000064f0: 3637 3131 3937 3939 3938 204c 2039 3534  6711979998 L 954
+00006500: 2e30 3438 3735 3637 3630 3539 3931 2031  .0487567605991 1
+00006510: 3236 302e 3830 3132 3532 3835 3739 3939  260.801252857999
+00006520: 3820 4c20 3935 342e 3034 3837 3536 3736  8 L 954.04875676
+00006530: 3035 3939 3120 3133 3033 2e30 3231 3437  05991 1303.02147
+00006540: 3036 3137 3939 3937 204c 2037 3331 2e32  06179997 L 731.2
+00006550: 3237 3135 3430 3333 3736 3331 2031 3330  271540337631 130
+00006560: 332e 3032 3134 3730 3631 3739 3939 3720  3.0214706179997 
+00006570: 4c20 3733 312e 3232 3731 3534 3033 3337  L 731.2271540337
+00006580: 3633 3120 3132 3434 2e39 3638 3637 3131  631 1244.9686711
+00006590: 3937 3939 3938 204d 2039 3338 2e32 3136  979998 M 938.216
+000065a0: 3137 3531 3030 3539 3931 2031 3234 342e  1751005991 1244.
+000065b0: 3936 3836 3731 3139 3739 3939 3820 4c20  9686711979998 L 
+000065c0: 3933 382e 3231 3631 3735 3130 3035 3939  938.216175100599
+000065d0: 3120 3132 3630 2e38 3031 3235 3238 3537  1 1260.801252857
+000065e0: 3939 3938 204c 2039 3534 2e30 3438 3735  9998 L 954.04875
+000065f0: 3637 3630 3539 3931 2031 3236 302e 3830  67605991 1260.80
+00006600: 3132 3532 3835 3739 3939 3822 2073 7472  12528579998" str
+00006610: 6f6b 652d 6d69 7465 726c 696d 6974 3d22  oke-miterlimit="
+00006620: 3130 2220 7374 726f 6b65 2d77 6964 7468  10" stroke-width
+00006630: 3d22 312e 3436 3539 3739 3738 3333 3333  ="1.465979783333
+00006640: 3333 3332 2220 7374 726f 6b65 2d64 6173  3332" stroke-das
+00006650: 6861 7272 6179 3d22 222f 3e3c 673e 3c74  harray=""/><g><t
+00006660: 6578 7420 6669 6c6c 3d22 626c 6163 6b22  ext fill="black"
+00006670: 2073 7472 6f6b 653d 226e 6f6e 6522 2066   stroke="none" f
+00006680: 6f6e 742d 6661 6d69 6c79 3d22 7361 6e73  ont-family="sans
+00006690: 2d73 6572 6966 2220 666f 6e74 2d73 697a  -serif" font-siz
+000066a0: 653d 2231 3170 7422 2066 6f6e 742d 7374  e="11pt" font-st
+000066b0: 796c 653d 226e 6f72 6d61 6c22 2066 6f6e  yle="normal" fon
+000066c0: 742d 7765 6967 6874 3d22 6e6f 726d 616c  t-weight="normal
+000066d0: 2220 7465 7874 2d64 6563 6f72 6174 696f  " text-decoratio
+000066e0: 6e3d 226e 6f72 6d61 6c22 2078 3d22 3735  n="normal" x="75
+000066f0: 352e 3835 3536 3134 3339 3337 3633 3122  5.8556143937631"
+00006700: 2079 3d22 3132 3639 2e35 3937 3133 3135   y="1269.5971315
+00006710: 3537 3939 3935 2220 7465 7874 2d61 6e63  579995" text-anc
+00006720: 686f 723d 2273 7461 7274 2220 646f 6d69  hor="start" domi
+00006730: 6e61 6e74 2d62 6173 656c 696e 653d 2261  nant-baseline="a
+00006740: 6c70 6861 6265 7469 6322 2078 6d6c 3a73  lphabetic" xml:s
+00006750: 7061 6365 3d22 7072 6573 6572 7665 223e  pace="preserve">
+00006760: 466f 726d 6174 c2a0 6669 656c 64c2 a076  Format..field..v
+00006770: 616c 7565 c2a0 696e 746f c2a0 613c 2f74  alue..into..a</t
+00006780: 6578 743e 3c74 6578 7420 6669 6c6c 3d22  ext><text fill="
+00006790: 626c 6163 6b22 2073 7472 6f6b 653d 226e  black" stroke="n
+000067a0: 6f6e 6522 2066 6f6e 742d 6661 6d69 6c79  one" font-family
+000067b0: 3d22 7361 6e73 2d73 6572 6966 2220 666f  ="sans-serif" fo
+000067c0: 6e74 2d73 697a 653d 2231 3170 7422 2066  nt-size="11pt" f
+000067d0: 6f6e 742d 7374 796c 653d 226e 6f72 6d61  ont-style="norma
+000067e0: 6c22 2066 6f6e 742d 7765 6967 6874 3d22  l" font-weight="
+000067f0: 6e6f 726d 616c 2220 7465 7874 2d64 6563  normal" text-dec
+00006800: 6f72 6174 696f 6e3d 226e 6f72 6d61 6c22  oration="normal"
+00006810: 2078 3d22 3735 352e 3835 3536 3134 3339   x="755.85561439
+00006820: 3337 3633 3122 2079 3d22 3132 3837 2e31  37631" y="1287.1
+00006830: 3838 3838 3839 3537 3939 3936 2220 7465  888889579996" te
+00006840: 7874 2d61 6e63 686f 723d 2273 7461 7274  xt-anchor="start
+00006850: 2220 646f 6d69 6e61 6e74 2d62 6173 656c  " dominant-basel
+00006860: 696e 653d 2261 6c70 6861 6265 7469 6322  ine="alphabetic"
+00006870: 2078 6d6c 3a73 7061 6365 3d22 7072 6573   xml:space="pres
+00006880: 6572 7665 223e 7374 7269 6e67 c2a0 6f72  erve">string..or
+00006890: c2a0 7661 6c75 65c2 a061 73c2 a072 6571  ..value..as..req
+000068a0: 7569 7265 642e 3c2f 7465 7874 3e3c 2f67  uired.</text></g
+000068b0: 3e3c 673e 3c67 3e3c 7265 6374 2066 696c  ><g><g><rect fil
+000068c0: 6c3d 2272 6762 2832 3034 2c32 3330 2c32  l="rgb(204,230,2
+000068d0: 3034 2922 2073 7472 6f6b 653d 226e 6f6e  04)" stroke="non
+000068e0: 6522 2078 3d22 3638 362e 3334 3837 3633  e" x="686.348763
+000068f0: 3739 3634 3338 3922 2079 3d22 3133 3239  7964389" y="1329
+00006900: 2e34 3039 3130 3637 3137 3939 3937 2220  .4091067179997" 
+00006910: 7769 6474 683d 2238 342e 3731 3139 3735  width="84.711975
+00006920: 3436 3231 3837 3522 2068 6569 6768 743d  4621875" height=
+00006930: 2232 322e 3836 3932 3834 3632 222f 3e3c  "22.86928462"/><
+00006940: 2f67 3e3c 7465 7874 2066 696c 6c3d 2262  /g><text fill="b
+00006950: 6c61 636b 2220 7374 726f 6b65 3d22 6e6f  lack" stroke="no
+00006960: 6e65 2220 666f 6e74 2d66 616d 696c 793d  ne" font-family=
+00006970: 226d 6f6e 6f73 7061 6365 2220 666f 6e74  "monospace" font
+00006980: 2d73 697a 653d 2231 3170 7422 2066 6f6e  -size="11pt" fon
+00006990: 742d 7374 796c 653d 226e 6f72 6d61 6c22  t-style="normal"
+000069a0: 2066 6f6e 742d 7765 6967 6874 3d22 6e6f   font-weight="no
+000069b0: 726d 616c 2220 7465 7874 2d64 6563 6f72  rmal" text-decor
+000069c0: 6174 696f 6e3d 226e 6f72 6d61 6c22 2078  ation="normal" x
+000069d0: 3d22 3638 382e 3938 3735 3237 3430 3634  ="688.9875274064
+000069e0: 3338 3922 2079 3d22 3133 3435 2e32 3431  389" y="1345.241
+000069f0: 3638 3833 3737 3939 3937 2220 7465 7874  6883779997" text
+00006a00: 2d61 6e63 686f 723d 2273 7461 7274 2220  -anchor="start" 
+00006a10: 646f 6d69 6e61 6e74 2d62 6173 656c 696e  dominant-baselin
+00006a20: 653d 2261 6c70 6861 6265 7469 6322 2078  e="alphabetic" x
+00006a30: 6d6c 3a73 7061 6365 3d22 7072 6573 6572  ml:space="preser
+00006a40: 7665 223e 266c 743b 266c 743b 7661 6c75  ve">&lt;&lt;valu
+00006a50: 6526 6774 3b26 6774 3b3c 2f74 6578 743e  e&gt;&gt;</text>
+00006a60: 3c2f 673e 3c67 3e3c 7061 7468 2066 696c  </g><g><path fil
+00006a70: 6c3d 226e 6f6e 6522 2073 7472 6f6b 653d  l="none" stroke=
+00006a80: 2262 6c61 636b 2220 7061 696e 742d 6f72  "black" paint-or
+00006a90: 6465 723d 2266 696c 6c20 7374 726f 6b65  der="fill stroke
+00006aa0: 206d 6172 6b65 7273 2220 643d 2220 4d20   markers" d=" M 
+00006ab0: 3833 332e 3834 3230 3736 3639 3731 3831  833.842076697181
+00006ac0: 2031 3335 322e 3237 3833 3931 3333 3739   1352.2783913379
+00006ad0: 3939 3720 4c20 3633 382e 3035 3133 3036  997 L 638.051306
+00006ae0: 3631 3732 3137 3520 3133 3532 2e32 3738  6172175 1352.278
+00006af0: 3339 3133 3337 3939 3937 2220 7374 726f  3913379997" stro
+00006b00: 6b65 2d6d 6974 6572 6c69 6d69 743d 2231  ke-miterlimit="1
+00006b10: 3022 2073 7472 6f6b 652d 7769 6474 683d  0" stroke-width=
+00006b20: 2231 2e34 3635 3937 3937 3833 3333 3333  "1.4659797833333
+00006b30: 3333 3222 2073 7472 6f6b 652d 6461 7368  332" stroke-dash
+00006b40: 6172 7261 793d 2237 2e30 3336 3730 3239  array="7.0367029
+00006b50: 3539 3939 3939 3939 3522 2f3e 3c67 2074  599999995"/><g t
+00006b60: 7261 6e73 666f 726d 3d22 7472 616e 736c  ransform="transl
+00006b70: 6174 6528 3632 332e 3536 3734 3236 3335  ate(623.56742635
+00006b80: 3738 3834 322c 3133 3532 2e32 3738 3339  78842,1352.27839
+00006b90: 3133 3337 3939 3937 2920 7472 616e 736c  13379997) transl
+00006ba0: 6174 6528 2d36 3233 2e35 3637 3432 3633  ate(-623.5674263
+00006bb0: 3537 3838 3432 2c2d 3133 3532 2e32 3738  578842,-1352.278
+00006bc0: 3339 3133 3337 3939 3937 2922 3e3c 7061  3913379997)"><pa
+00006bd0: 7468 2066 696c 6c3d 2262 6c61 636b 2220  th fill="black" 
+00006be0: 7374 726f 6b65 3d22 6e6f 6e65 2220 7061  stroke="none" pa
+00006bf0: 696e 742d 6f72 6465 723d 2273 7472 6f6b  int-order="strok
+00006c00: 6520 6669 6c6c 206d 6172 6b65 7273 2220  e fill markers" 
+00006c10: 643d 2220 4d20 3633 382e 3232 3732 3234  d=" M 638.227224
+00006c20: 3139 3132 3137 3520 3133 3434 2e39 3438  1912175 1344.948
+00006c30: 3439 3234 3231 3333 3320 4c20 3632 332e  492421333 L 623.
+00006c40: 3536 3734 3236 3335 3738 3834 3220 3133  5674263578842 13
+00006c50: 3532 2e32 3738 3339 3133 3337 3939 3937  52.2783913379997
+00006c60: 204c 2036 3338 2e32 3237 3232 3431 3931   L 638.227224191
+00006c70: 3231 3735 2031 3335 392e 3630 3832 3930  2175 1359.608290
+00006c80: 3235 3436 3636 3420 5a22 2f3e 3c2f 673e  2546664 Z"/></g>
+00006c90: 3c2f 673e 3c67 3e3c 673e 3c72 6563 7420  </g><g><g><rect 
+00006ca0: 6669 6c6c 3d22 7267 6228 3230 342c 3233  fill="rgb(204,23
+00006cb0: 302c 3230 3429 2220 7374 726f 6b65 3d22  0,204)" stroke="
+00006cc0: 6e6f 6e65 2220 783d 2233 3731 2e30 3033  none" x="371.003
+00006cd0: 3037 3836 3231 3036 3132 2220 793d 2231  0786210612" y="1
+00006ce0: 3337 382e 3636 3630 3237 3433 3739 3939  378.666027437999
+00006cf0: 3722 2077 6964 7468 3d22 3834 2e37 3131  7" width="84.711
+00006d00: 3937 3534 3632 3138 3735 2220 6865 6967  9754621875" heig
+00006d10: 6874 3d22 3232 2e38 3639 3238 3436 3222  ht="22.86928462"
+00006d20: 2f3e 3c2f 673e 3c74 6578 7420 6669 6c6c  /></g><text fill
+00006d30: 3d22 626c 6163 6b22 2073 7472 6f6b 653d  ="black" stroke=
+00006d40: 226e 6f6e 6522 2066 6f6e 742d 6661 6d69  "none" font-fami
+00006d50: 6c79 3d22 6d6f 6e6f 7370 6163 6522 2066  ly="monospace" f
+00006d60: 6f6e 742d 7369 7a65 3d22 3131 7074 2220  ont-size="11pt" 
+00006d70: 666f 6e74 2d73 7479 6c65 3d22 6e6f 726d  font-style="norm
+00006d80: 616c 2220 666f 6e74 2d77 6569 6768 743d  al" font-weight=
+00006d90: 226e 6f72 6d61 6c22 2074 6578 742d 6465  "normal" text-de
+00006da0: 636f 7261 7469 6f6e 3d22 6e6f 726d 616c  coration="normal
+00006db0: 2220 783d 2233 3733 2e36 3431 3834 3232  " x="373.6418422
+00006dc0: 3331 3036 3132 2220 793d 2231 3339 342e  310612" y="1394.
+00006dd0: 3439 3836 3039 3039 3739 3939 3622 2074  4986090979996" t
+00006de0: 6578 742d 616e 6368 6f72 3d22 7374 6172  ext-anchor="star
+00006df0: 7422 2064 6f6d 696e 616e 742d 6261 7365  t" dominant-base
+00006e00: 6c69 6e65 3d22 616c 7068 6162 6574 6963  line="alphabetic
+00006e10: 2220 786d 6c3a 7370 6163 653d 2270 7265  " xml:space="pre
+00006e20: 7365 7276 6522 3e26 6c74 3b26 6c74 3b76  serve">&lt;&lt;v
+00006e30: 616c 7565 2667 743b 2667 743b 3c2f 7465  alue&gt;&gt;</te
+00006e40: 7874 3e3c 2f67 3e3c 673e 3c70 6174 6820  xt></g><g><path 
+00006e50: 6669 6c6c 3d22 6e6f 6e65 2220 7374 726f  fill="none" stro
+00006e60: 6b65 3d22 626c 6163 6b22 2070 6169 6e74  ke="black" paint
+00006e70: 2d6f 7264 6572 3d22 6669 6c6c 2073 7472  -order="fill str
+00006e80: 6f6b 6520 6d61 726b 6572 7322 2064 3d22  oke markers" d="
+00006e90: 204d 2035 3937 2e31 3739 3739 3032 3537   M 597.179790257
+00006ea0: 3838 3432 2031 3430 312e 3533 3533 3132  8842 1401.535312
+00006eb0: 3035 3739 3939 3620 4c20 3234 342e 3032  0579996 L 244.02
+00006ec0: 3232 3232 3730 3537 3539 3133 2031 3430  222270575913 140
+00006ed0: 312e 3533 3533 3132 3035 3739 3939 3622  1.5353120579996"
+00006ee0: 2073 7472 6f6b 652d 6d69 7465 726c 696d   stroke-miterlim
+00006ef0: 6974 3d22 3130 2220 7374 726f 6b65 2d77  it="10" stroke-w
+00006f00: 6964 7468 3d22 312e 3436 3539 3739 3738  idth="1.46597978
+00006f10: 3333 3333 3333 3332 2220 7374 726f 6b65  33333332" stroke
+00006f20: 2d64 6173 6861 7272 6179 3d22 372e 3033  -dasharray="7.03
+00006f30: 3637 3032 3935 3939 3939 3939 3935 222f  67029599999995"/
+00006f40: 3e3c 6720 7472 616e 7366 6f72 6d3d 2274  ><g transform="t
+00006f50: 7261 6e73 6c61 7465 2832 3239 2e35 3338  ranslate(229.538
+00006f60: 3334 3234 3436 3432 3538 2c31 3430 312e  3424464258,1401.
+00006f70: 3533 3533 3132 3035 3739 3939 3629 2074  5353120579996) t
+00006f80: 7261 6e73 6c61 7465 282d 3232 392e 3533  ranslate(-229.53
+00006f90: 3833 3432 3434 3634 3235 382c 2d31 3430  83424464258,-140
+00006fa0: 312e 3533 3533 3132 3035 3739 3939 3629  1.5353120579996)
+00006fb0: 223e 3c70 6174 6820 6669 6c6c 3d22 626c  "><path fill="bl
+00006fc0: 6163 6b22 2073 7472 6f6b 653d 226e 6f6e  ack" stroke="non
+00006fd0: 6522 2070 6169 6e74 2d6f 7264 6572 3d22  e" paint-order="
+00006fe0: 7374 726f 6b65 2066 696c 6c20 6d61 726b  stroke fill mark
+00006ff0: 6572 7322 2064 3d22 204d 2032 3434 2e31  ers" d=" M 244.1
+00007000: 3938 3134 3032 3739 3735 3931 3220 3133  9814027975912 13
+00007010: 3934 2e32 3035 3431 3331 3431 3333 3239  94.2054131413329
+00007020: 204c 2032 3239 2e35 3338 3334 3234 3436   L 229.538342446
+00007030: 3432 3538 2031 3430 312e 3533 3533 3132  4258 1401.535312
+00007040: 3035 3739 3939 3620 4c20 3234 342e 3139  0579996 L 244.19
+00007050: 3831 3430 3237 3937 3539 3132 2031 3430  814027975912 140
+00007060: 382e 3836 3532 3130 3937 3436 3636 3320  8.8652109746663 
+00007070: 5a22 2f3e 3c2f 673e 3c2f 673e 3c67 3e3c  Z"/></g></g><g><
+00007080: 673e 3c72 6563 7420 6669 6c6c 3d22 7267  g><rect fill="rg
+00007090: 6228 3235 352c 3234 322c 3234 3529 2220  b(255,242,245)" 
+000070a0: 7374 726f 6b65 3d22 6e6f 6e65 2220 783d  stroke="none" x=
+000070b0: 2235 3632 2e36 3436 3436 3534 3734 3736  "562.64646547476
+000070c0: 3234 2220 793d 2231 3435 342e 3331 3035  24" y="1454.3105
+000070d0: 3834 3235 3739 3939 3622 2077 6964 7468  842579996" width
+000070e0: 3d22 3735 2e38 3835 3932 3536 3537 3522  ="75.8859256575"
+000070f0: 2068 6569 6768 743d 2232 322e 3836 3932   height="22.8692
+00007100: 3834 3632 222f 3e3c 2f67 3e3c 7465 7874  8462"/></g><text
+00007110: 2066 696c 6c3d 2262 6c61 636b 2220 7374   fill="black" st
+00007120: 726f 6b65 3d22 6e6f 6e65 2220 666f 6e74  roke="none" font
+00007130: 2d66 616d 696c 793d 226d 6f6e 6f73 7061  -family="monospa
+00007140: 6365 2220 666f 6e74 2d73 697a 653d 2231  ce" font-size="1
+00007150: 3170 7422 2066 6f6e 742d 7374 796c 653d  1pt" font-style=
+00007160: 226e 6f72 6d61 6c22 2066 6f6e 742d 7765  "normal" font-we
+00007170: 6967 6874 3d22 6e6f 726d 616c 2220 7465  ight="normal" te
+00007180: 7874 2d64 6563 6f72 6174 696f 6e3d 226e  xt-decoration="n
+00007190: 6f72 6d61 6c22 2078 3d22 3536 352e 3238  ormal" x="565.28
+000071a0: 3532 3239 3038 3437 3632 3422 2079 3d22  52290847624" y="
+000071b0: 3134 3730 2e31 3433 3136 3539 3137 3939  1470.14316591799
+000071c0: 3936 2220 7465 7874 2d61 6e63 686f 723d  96" text-anchor=
+000071d0: 2273 7461 7274 2220 646f 6d69 6e61 6e74  "start" dominant
+000071e0: 2d62 6173 656c 696e 653d 2261 6c70 6861  -baseline="alpha
+000071f0: 6265 7469 6322 2078 6d6c 3a73 7061 6365  betic" xml:space
+00007200: 3d22 7072 6573 6572 7665 223e 6170 7065  ="preserve">appe
+00007210: 6e64 2829 3c2f 7465 7874 3e3c 2f67 3e3c  nd()</text></g><
+00007220: 673e 3c70 6174 6820 6669 6c6c 3d22 6e6f  g><path fill="no
+00007230: 6e65 2220 7374 726f 6b65 3d22 626c 6163  ne" stroke="blac
+00007240: 6b22 2070 6169 6e74 2d6f 7264 6572 3d22  k" paint-order="
+00007250: 6669 6c6c 2073 7472 6f6b 6520 6d61 726b  fill stroke mark
+00007260: 6572 7322 2064 3d22 204d 2032 3131 2e39  ers" d=" M 211.9
+00007270: 3436 3538 3530 3436 3432 3537 3820 3134  4658504642578 14
+00007280: 3737 2e31 3739 3836 3838 3737 3939 3935  77.1798688779995
+00007290: 204c 2039 3734 2e37 3438 3339 3133 3031   L 974.748391301
+000072a0: 3236 3537 2031 3437 372e 3137 3938 3638  2657 1477.179868
+000072b0: 3837 3739 3939 3522 2073 7472 6f6b 652d  8779995" stroke-
+000072c0: 6d69 7465 726c 696d 6974 3d22 3130 2220  miterlimit="10" 
+000072d0: 7374 726f 6b65 2d77 6964 7468 3d22 312e  stroke-width="1.
+000072e0: 3436 3539 3739 3738 3333 3333 3333 3332  4659797833333332
+000072f0: 2220 7374 726f 6b65 2d64 6173 6861 7272  " stroke-dasharr
+00007300: 6179 3d22 222f 3e3c 6720 7472 616e 7366  ay=""/><g transf
+00007310: 6f72 6d3d 2274 7261 6e73 6c61 7465 2839  orm="translate(9
+00007320: 3839 2e32 3332 3237 3135 3630 3539 392c  89.232271560599,
+00007330: 3134 3737 2e31 3739 3836 3838 3737 3939  1477.17986887799
+00007340: 3935 2920 7472 616e 736c 6174 6528 2d39  95) translate(-9
+00007350: 3839 2e32 3332 3237 3135 3630 3539 392c  89.232271560599,
+00007360: 2d31 3437 372e 3137 3938 3638 3837 3739  -1477.1798688779
+00007370: 3939 3529 223e 3c70 6174 6820 6669 6c6c  995)"><path fill
+00007380: 3d22 626c 6163 6b22 2073 7472 6f6b 653d  ="black" stroke=
+00007390: 226e 6f6e 6522 2070 6169 6e74 2d6f 7264  "none" paint-ord
+000073a0: 6572 3d22 7374 726f 6b65 2066 696c 6c20  er="stroke fill 
+000073b0: 6d61 726b 6572 7322 2064 3d22 204d 2039  markers" d=" M 9
+000073c0: 3734 2e35 3732 3437 3337 3237 3236 3537  74.5724737272657
+000073d0: 2031 3436 392e 3834 3939 3639 3936 3133   1469.8499699613
+000073e0: 3332 3820 4c20 3938 392e 3233 3232 3731  328 L 989.232271
+000073f0: 3536 3035 3939 2031 3437 372e 3137 3938  560599 1477.1798
+00007400: 3638 3837 3739 3939 3520 4c20 3937 342e  688779995 L 974.
+00007410: 3537 3234 3733 3732 3732 3635 3720 3134  5724737272657 14
+00007420: 3834 2e35 3039 3736 3737 3934 3636 3632  84.5097677946662
+00007430: 205a 222f 3e3c 2f67 3e3c 2f67 3e3c 673e   Z"/></g></g><g>
+00007440: 3c67 3e3c 7265 6374 2066 696c 6c3d 2277  <g><rect fill="w
+00007450: 6869 7465 2220 7374 726f 6b65 3d22 6e6f  hite" stroke="no
+00007460: 6e65 2220 783d 2232 3332 2e37 3633 3439  ne" x="232.76349
+00007470: 3739 3639 3735 3931 2220 793d 2231 3532  79697591" y="152
+00007480: 392e 3935 3531 3431 3037 3739 3939 3522  9.9551410779995"
+00007490: 2077 6964 7468 3d22 3130 322e 3336 3430   width="102.3640
+000074a0: 3735 3037 3135 3632 3522 2068 6569 6768  750715625" heigh
+000074b0: 743d 2232 322e 3836 3932 3834 3632 222f  t="22.86928462"/
+000074c0: 3e3c 2f67 3e3c 7465 7874 2066 696c 6c3d  ></g><text fill=
+000074d0: 2262 6c61 636b 2220 7374 726f 6b65 3d22  "black" stroke="
+000074e0: 6e6f 6e65 2220 666f 6e74 2d66 616d 696c  none" font-famil
+000074f0: 793d 226d 6f6e 6f73 7061 6365 2220 666f  y="monospace" fo
+00007500: 6e74 2d73 697a 653d 2231 3170 7422 2066  nt-size="11pt" f
+00007510: 6f6e 742d 7374 796c 653d 226e 6f72 6d61  ont-style="norma
+00007520: 6c22 2066 6f6e 742d 7765 6967 6874 3d22  l" font-weight="
+00007530: 6e6f 726d 616c 2220 7465 7874 2d64 6563  normal" text-dec
+00007540: 6f72 6174 696f 6e3d 226e 6f72 6d61 6c22  oration="normal"
+00007550: 2078 3d22 3233 352e 3430 3232 3631 3537   x="235.40226157
+00007560: 3937 3539 3122 2079 3d22 3135 3435 2e37  97591" y="1545.7
+00007570: 3837 3732 3237 3337 3939 3935 2220 7465  877227379995" te
+00007580: 7874 2d61 6e63 686f 723d 2273 7461 7274  xt-anchor="start
+00007590: 2220 646f 6d69 6e61 6e74 2d62 6173 656c  " dominant-basel
+000075a0: 696e 653d 2261 6c70 6861 6265 7469 6322  ine="alphabetic"
+000075b0: 2078 6d6c 3a73 7061 6365 3d22 7072 6573   xml:space="pres
+000075c0: 6572 7665 223e 266c 743b 266c 743b 4461  erve">&lt;&lt;Da
+000075d0: 7461 7365 7426 6774 3b26 6774 3b3c 2f74  taset&gt;&gt;</t
+000075e0: 6578 743e 3c2f 673e 3c67 3e3c 7061 7468  ext></g><g><path
+000075f0: 2066 696c 6c3d 226e 6f6e 6522 2073 7472   fill="none" str
+00007600: 6f6b 653d 2262 6c61 636b 2220 7061 696e  oke="black" pain
+00007610: 742d 6f72 6465 723d 2266 696c 6c20 7374  t-order="fill st
+00007620: 726f 6b65 206d 6172 6b65 7273 2220 643d  roke markers" d=
+00007630: 2220 4d20 3231 312e 3934 3635 3835 3034  " M 211.94658504
+00007640: 3634 3235 3738 2031 3535 322e 3832 3434  642578 1552.8244
+00007650: 3235 3639 3739 3939 3720 4c20 3238 322e  256979997 L 282.
+00007660: 3331 3336 3134 3634 3634 3235 3820 3135  3136146464258 15
+00007670: 3532 2e38 3234 3432 3536 3937 3939 3937  52.8244256979997
+00007680: 204c 2032 3832 2e33 3133 3631 3436 3436   L 282.313614646
+00007690: 3432 3538 2031 3537 352e 3639 3337 3130  4258 1575.693710
+000076a0: 3331 3739 3939 3620 4c20 3231 372e 3633  3179996 L 217.63
+000076b0: 3435 3836 3630 3537 3539 3133 2031 3537  458660575913 157
+000076c0: 352e 3639 3337 3130 3331 3739 3939 3622  5.6937103179996"
+000076d0: 2073 7472 6f6b 652d 6d69 7465 726c 696d   stroke-miterlim
+000076e0: 6974 3d22 3130 2220 7374 726f 6b65 2d77  it="10" stroke-w
+000076f0: 6964 7468 3d22 312e 3436 3539 3739 3738  idth="1.46597978
+00007700: 3333 3333 3333 3332 2220 7374 726f 6b65  33333332" stroke
+00007710: 2d64 6173 6861 7272 6179 3d22 372e 3033  -dasharray="7.03
+00007720: 3637 3032 3935 3939 3939 3939 3935 222f  67029599999995"/
+00007730: 3e3c 6720 7472 616e 7366 6f72 6d3d 2274  ><g transform="t
+00007740: 7261 6e73 6c61 7465 2832 3033 2e31 3530  ranslate(203.150
+00007750: 3730 3633 3436 3432 3537 382c 3135 3735  70634642578,1575
+00007760: 2e36 3933 3731 3033 3137 3939 3936 2920  .6937103179996) 
+00007770: 7472 616e 736c 6174 6528 2d32 3033 2e31  translate(-203.1
+00007780: 3530 3730 3633 3436 3432 3537 382c 2d31  5070634642578,-1
+00007790: 3537 352e 3639 3337 3130 3331 3739 3939  575.693710317999
+000077a0: 3629 223e 3c70 6174 6820 6669 6c6c 3d22  6)"><path fill="
+000077b0: 626c 6163 6b22 2073 7472 6f6b 653d 226e  black" stroke="n
+000077c0: 6f6e 6522 2070 6169 6e74 2d6f 7264 6572  one" paint-order
+000077d0: 3d22 7374 726f 6b65 2066 696c 6c20 6d61  ="stroke fill ma
+000077e0: 726b 6572 7322 2064 3d22 204d 2032 3137  rkers" d=" M 217
+000077f0: 2e38 3130 3530 3431 3739 3735 3931 2031  .8105041797591 1
+00007800: 3536 382e 3336 3338 3131 3430 3133 3333  568.363811401333
+00007810: 204c 2032 3033 2e31 3530 3730 3633 3436   L 203.150706346
+00007820: 3432 3537 3820 3135 3735 2e36 3933 3731  42578 1575.69371
+00007830: 3033 3137 3939 3936 204c 2032 3137 2e38  03179996 L 217.8
+00007840: 3130 3530 3431 3739 3735 3931 2031 3538  105041797591 158
+00007850: 332e 3032 3336 3039 3233 3436 3636 3320  3.0236092346663 
+00007860: 5a22 2f3e 3c2f 673e 3c2f 673e 3c67 3e3c  Z"/></g></g><g><
+00007870: 672f 3e3c 7061 7468 2066 696c 6c3d 226e  g/><path fill="n
+00007880: 6f6e 6522 2073 7472 6f6b 653d 2262 6c61  one" stroke="bla
+00007890: 636b 2220 7061 696e 742d 6f72 6465 723d  ck" paint-order=
+000078a0: 2266 696c 6c20 7374 726f 6b65 206d 6172  "fill stroke mar
+000078b0: 6b65 7273 2220 643d 2220 4d20 3937 2e36  kers" d=" M 97.6
+000078c0: 3030 3136 3139 3436 3432 3537 3920 3631  0016194642579 61
+000078d0: 312e 3636 3534 3034 3739 3739 3939 3920  1.6654047979999 
+000078e0: 4c20 3130 3530 2e38 3033 3432 3234 3630  L 1050.803422460
+000078f0: 3539 3920 3631 312e 3636 3534 3034 3739  599 611.66540479
+00007900: 3739 3939 3920 4c20 3130 3530 2e38 3033  79999 L 1050.803
+00007910: 3432 3234 3630 3539 3920 3135 3033 2e35  422460599 1503.5
+00007920: 3637 3530 3439 3737 3939 3935 204c 2039  675049779995 L 9
+00007930: 372e 3630 3031 3631 3934 3634 3235 3739  7.60016194642579
+00007940: 2031 3530 332e 3536 3735 3034 3937 3739   1503.5675049779
+00007950: 3939 3520 4c20 3937 2e36 3030 3136 3139  995 L 97.6001619
+00007960: 3436 3432 3537 3920 3631 312e 3636 3534  4642579 611.6654
+00007970: 3034 3739 3739 3939 3920 5a22 2073 7472  047979999 Z" str
+00007980: 6f6b 652d 6d69 7465 726c 696d 6974 3d22  oke-miterlimit="
+00007990: 3130 2220 7374 726f 6b65 2d77 6964 7468  10" stroke-width
+000079a0: 3d22 322e 3531 3331 3038 3222 2073 7472  ="2.5131082" str
+000079b0: 6f6b 652d 6461 7368 6172 7261 793d 2222  oke-dasharray=""
+000079c0: 2f3e 3c70 6174 6820 6669 6c6c 3d22 7069  /><path fill="pi
+000079d0: 6e6b 2220 7374 726f 6b65 3d22 626c 6163  nk" stroke="blac
+000079e0: 6b22 2070 6169 6e74 2d6f 7264 6572 3d22  k" paint-order="
+000079f0: 6669 6c6c 2073 7472 6f6b 6520 6d61 726b  fill stroke mark
+00007a00: 6572 7322 2064 3d22 204d 2039 372e 3630  ers" d=" M 97.60
+00007a10: 3031 3631 3934 3634 3235 3739 2036 3131  016194642579 611
+00007a20: 2e36 3635 3430 3437 3937 3939 3939 204c  .6654047979999 L
+00007a30: 2039 372e 3630 3031 3631 3934 3634 3235   97.600161946425
+00007a40: 3739 2036 3332 2e37 3735 3531 3336 3737  79 632.775513677
+00007a50: 3939 3939 204c 2031 3537 2e35 3338 3037  9999 L 157.53807
+00007a60: 3132 3737 3637 3537 3820 3633 322e 3737  127767578 632.77
+00007a70: 3535 3133 3637 3739 3939 3920 4c20 3136  55136779999 L 16
+00007a80: 382e 3039 3331 3235 3731 3736 3735 3738  8.09312571767578
+00007a90: 2036 3232 2e32 3230 3435 3932 3338 204c   622.220459238 L
+00007aa0: 2031 3638 2e30 3933 3132 3537 3137 3637   168.09312571767
+00007ab0: 3537 3820 3631 312e 3636 3534 3034 3739  578 611.66540479
+00007ac0: 3739 3939 3920 4c20 3937 2e36 3030 3136  79999 L 97.60016
+00007ad0: 3139 3436 3432 3537 3920 3631 312e 3636  194642579 611.66
+00007ae0: 3534 3034 3739 3739 3939 3922 2073 7472  54047979999" str
+00007af0: 6f6b 652d 6d69 7465 726c 696d 6974 3d22  oke-miterlimit="
+00007b00: 3130 2220 7374 726f 6b65 2d77 6964 7468  10" stroke-width
+00007b10: 3d22 322e 3531 3331 3038 3222 2073 7472  ="2.5131082" str
+00007b20: 6f6b 652d 6461 7368 6172 7261 793d 2222  oke-dasharray=""
+00007b30: 2f3e 3c74 6578 7420 6669 6c6c 3d22 626c  /><text fill="bl
+00007b40: 6163 6b22 2073 7472 6f6b 653d 226e 6f6e  ack" stroke="non
+00007b50: 6522 2066 6f6e 742d 6661 6d69 6c79 3d22  e" font-family="
+00007b60: 7361 6e73 2d73 6572 6966 2220 666f 6e74  sans-serif" font
+00007b70: 2d73 697a 653d 2238 2e38 7074 2220 666f  -size="8.8pt" fo
+00007b80: 6e74 2d73 7479 6c65 3d22 6e6f 726d 616c  nt-style="normal
+00007b90: 2220 666f 6e74 2d77 6569 6768 743d 2262  " font-weight="b
+00007ba0: 6f6c 6422 2074 6578 742d 6465 636f 7261  old" text-decora
+00007bb0: 7469 6f6e 3d22 6e6f 726d 616c 2220 783d  tion="normal" x=
+00007bc0: 2231 3135 2e31 3931 3931 3933 3436 3432  "115.19191934642
+00007bd0: 3537 3822 2079 3d22 3632 352e 3733 3838  578" y="625.7388
+00007be0: 3130 3731 3822 2074 6578 742d 616e 6368  10718" text-anch
+00007bf0: 6f72 3d22 7374 6172 7422 2064 6f6d 696e  or="start" domin
+00007c00: 616e 742d 6261 7365 6c69 6e65 3d22 616c  ant-baseline="al
+00007c10: 7068 6162 6574 6963 2220 786d 6c3a 7370  phabetic" xml:sp
+00007c20: 6163 653d 2270 7265 7365 7276 6522 3e6c  ace="preserve">l
+00007c30: 6f6f 703c 2f74 6578 743e 3c67 3e3c 7265  oop</text><g><re
+00007c40: 6374 2066 696c 6c3d 2272 6762 2832 3535  ct fill="rgb(255
+00007c50: 2c32 3432 2c32 3435 2922 2073 7472 6f6b  ,242,245)" strok
+00007c60: 653d 226e 6f6e 6522 2078 3d22 3138 332e  e="none" x="183.
+00007c70: 3034 3631 3139 3530 3736 3735 3737 2220  04611950767577" 
+00007c80: 793d 2236 3133 2e30 3732 3734 3533 3922  y="613.07274539"
+00007c90: 2077 6964 7468 3d22 3133 312e 3733 3537   width="131.7357
+00007ca0: 3138 3133 3739 3638 3735 2220 6865 6967  1813796875" heig
+00007cb0: 6874 3d22 3138 2e32 3935 3432 3736 3936  ht="18.295427696
+00007cc0: 222f 3e3c 2f67 3e3c 7465 7874 2066 696c  "/></g><text fil
+00007cd0: 6c3d 2262 6c61 636b 2220 7374 726f 6b65  l="black" stroke
+00007ce0: 3d22 6e6f 6e65 2220 666f 6e74 2d66 616d  ="none" font-fam
+00007cf0: 696c 793d 2273 616e 732d 7365 7269 6622  ily="sans-serif"
+00007d00: 2066 6f6e 742d 7369 7a65 3d22 382e 3870   font-size="8.8p
+00007d10: 7422 2066 6f6e 742d 7374 796c 653d 226e  t" font-style="n
+00007d20: 6f72 6d61 6c22 2066 6f6e 742d 7765 6967  ormal" font-weig
+00007d30: 6874 3d22 626f 6c64 2220 7465 7874 2d64  ht="bold" text-d
+00007d40: 6563 6f72 6174 696f 6e3d 226e 6f72 6d61  ecoration="norma
+00007d50: 6c22 2078 3d22 3138 352e 3638 3438 3833  l" x="185.684883
+00007d60: 3131 3736 3735 3738 2220 793d 2236 3235  11767578" y="625
+00007d70: 2e37 3338 3831 3037 3138 2220 7465 7874  .738810718" text
+00007d80: 2d61 6e63 686f 723d 2273 7461 7274 2220  -anchor="start" 
+00007d90: 646f 6d69 6e61 6e74 2d62 6173 656c 696e  dominant-baselin
+00007da0: 653d 2261 6c70 6861 6265 7469 6322 2078  e="alphabetic" x
+00007db0: 6d6c 3a73 7061 6365 3d22 7072 6573 6572  ml:space="preser
+00007dc0: 7665 223e 5b65 6163 68c2 a072 6f77 c2a0  ve">[each..row..
+00007dd0: 696e c2a0 5175 6572 7973 6574 5d3c 2f74  in..Queryset]</t
+00007de0: 6578 743e 3c2f 673e 3c67 3e3c 672f 3e3c  ext></g><g><g/><
+00007df0: 7061 7468 2066 696c 6c3d 226e 6f6e 6522  path fill="none"
+00007e00: 2073 7472 6f6b 653d 2262 6c61 636b 2220   stroke="black" 
+00007e10: 7061 696e 742d 6f72 6465 723d 2266 696c  paint-order="fil
+00007e20: 6c20 7374 726f 6b65 206d 6172 6b65 7273  l stroke markers
+00007e30: 2220 643d 2220 4d20 3131 352e 3139 3139  " d=" M 115.1919
+00007e40: 3139 3334 3634 3235 3739 2037 3331 2e32  1934642579 731.2
+00007e50: 3839 3335 3531 3137 3939 3939 204c 2039  893551179999 L 9
+00007e60: 3632 2e38 3434 3633 3534 3630 3539 3920  62.844635460599 
+00007e70: 3733 312e 3238 3933 3535 3131 3739 3939  731.289355117999
+00007e80: 3920 4c20 3936 322e 3834 3436 3335 3436  9 L 962.84463546
+00007e90: 3035 3939 2031 3432 372e 3932 3239 3438  0599 1427.922948
+00007ea0: 3135 3739 3939 3620 4c20 3131 352e 3139  1579996 L 115.19
+00007eb0: 3139 3139 3334 3634 3235 3739 2031 3432  191934642579 142
+00007ec0: 372e 3932 3239 3438 3135 3739 3939 3620  7.9229481579996 
+00007ed0: 4c20 3131 352e 3139 3139 3139 3334 3634  L 115.1919193464
+00007ee0: 3235 3739 2037 3331 2e32 3839 3335 3531  2579 731.2893551
+00007ef0: 3137 3939 3939 205a 2220 7374 726f 6b65  179999 Z" stroke
+00007f00: 2d6d 6974 6572 6c69 6d69 743d 2231 3022  -miterlimit="10"
+00007f10: 2073 7472 6f6b 652d 7769 6474 683d 2232   stroke-width="2
+00007f20: 2e35 3133 3130 3832 2220 7374 726f 6b65  .5131082" stroke
+00007f30: 2d64 6173 6861 7272 6179 3d22 222f 3e3c  -dasharray=""/><
+00007f40: 7061 7468 2066 696c 6c3d 2267 7265 656e  path fill="green
+00007f50: 2220 7374 726f 6b65 3d22 626c 6163 6b22  " stroke="black"
+00007f60: 2070 6169 6e74 2d6f 7264 6572 3d22 6669   paint-order="fi
+00007f70: 6c6c 2073 7472 6f6b 6520 6d61 726b 6572  ll stroke marker
+00007f80: 7322 2064 3d22 204d 2031 3135 2e31 3931  s" d=" M 115.191
+00007f90: 3931 3933 3436 3432 3537 3920 3733 312e  91934642579 731.
+00007fa0: 3238 3933 3535 3131 3739 3939 3920 4c20  2893551179999 L 
+00007fb0: 3131 352e 3139 3139 3139 3334 3634 3235  115.191919346425
+00007fc0: 3739 2037 3532 2e33 3939 3436 3339 3937  79 752.399463997
+00007fd0: 3939 3939 204c 2031 3735 2e31 3239 3832  9999 L 175.12982
+00007fe0: 3836 3737 3637 3538 2037 3532 2e33 3939  86776758 752.399
+00007ff0: 3436 3339 3937 3939 3939 204c 2031 3835  4639979999 L 185
+00008000: 2e36 3834 3838 3331 3137 3637 3537 3820  .68488311767578 
+00008010: 3734 312e 3834 3434 3039 3535 3739 3939  741.844409557999
+00008020: 3920 4c20 3138 352e 3638 3438 3833 3131  9 L 185.68488311
+00008030: 3736 3735 3738 2037 3331 2e32 3839 3335  767578 731.28935
+00008040: 3531 3137 3939 3939 204c 2031 3135 2e31  51179999 L 115.1
+00008050: 3931 3931 3933 3436 3432 3537 3920 3733  9191934642579 73
+00008060: 312e 3238 3933 3535 3131 3739 3939 3922  1.2893551179999"
+00008070: 2073 7472 6f6b 652d 6d69 7465 726c 696d   stroke-miterlim
+00008080: 6974 3d22 3130 2220 7374 726f 6b65 2d77  it="10" stroke-w
+00008090: 6964 7468 3d22 322e 3531 3331 3038 3222  idth="2.5131082"
+000080a0: 2073 7472 6f6b 652d 6461 7368 6172 7261   stroke-dasharra
+000080b0: 793d 2222 2f3e 3c74 6578 7420 6669 6c6c  y=""/><text fill
+000080c0: 3d22 626c 6163 6b22 2073 7472 6f6b 653d  ="black" stroke=
+000080d0: 226e 6f6e 6522 2066 6f6e 742d 6661 6d69  "none" font-fami
+000080e0: 6c79 3d22 7361 6e73 2d73 6572 6966 2220  ly="sans-serif" 
+000080f0: 666f 6e74 2d73 697a 653d 2238 2e38 7074  font-size="8.8pt
+00008100: 2220 666f 6e74 2d73 7479 6c65 3d22 6e6f  " font-style="no
+00008110: 726d 616c 2220 666f 6e74 2d77 6569 6768  rmal" font-weigh
+00008120: 743d 2262 6f6c 6422 2074 6578 742d 6465  t="bold" text-de
+00008130: 636f 7261 7469 6f6e 3d22 6e6f 726d 616c  coration="normal
+00008140: 2220 783d 2231 3332 2e37 3833 3637 3637  " x="132.7836767
+00008150: 3436 3432 3537 3822 2079 3d22 3734 352e  4642578" y="745.
+00008160: 3336 3237 3631 3033 3739 3939 3922 2074  3627610379999" t
+00008170: 6578 742d 616e 6368 6f72 3d22 7374 6172  ext-anchor="star
+00008180: 7422 2064 6f6d 696e 616e 742d 6261 7365  t" dominant-base
+00008190: 6c69 6e65 3d22 616c 7068 6162 6574 6963  line="alphabetic
+000081a0: 2220 786d 6c3a 7370 6163 653d 2270 7265  " xml:space="pre
+000081b0: 7365 7276 6522 3e6c 6f6f 703c 2f74 6578  serve">loop</tex
+000081c0: 743e 3c67 3e3c 7265 6374 2066 696c 6c3d  t><g><rect fill=
+000081d0: 2272 6762 2832 3034 2c32 3330 2c32 3034  "rgb(204,230,204
+000081e0: 2922 2073 7472 6f6b 653d 226e 6f6e 6522  )" stroke="none"
+000081f0: 2078 3d22 3230 302e 3633 3738 3736 3930   x="200.63787690
+00008200: 3736 3735 3737 2220 793d 2237 3332 2e36  767577" y="732.6
+00008210: 3936 3639 3537 3122 2077 6964 7468 3d22  9669571" width="
+00008220: 3136 372e 3536 3731 3233 3737 3736 3137  167.567123777617
+00008230: 3138 2220 6865 6967 6874 3d22 3138 2e32  18" height="18.2
+00008240: 3935 3432 3736 3936 222f 3e3c 2f67 3e3c  95427696"/></g><
+00008250: 7465 7874 2066 696c 6c3d 2262 6c61 636b  text fill="black
+00008260: 2220 7374 726f 6b65 3d22 6e6f 6e65 2220  " stroke="none" 
+00008270: 666f 6e74 2d66 616d 696c 793d 2273 616e  font-family="san
+00008280: 732d 7365 7269 6622 2066 6f6e 742d 7369  s-serif" font-si
+00008290: 7a65 3d22 382e 3870 7422 2066 6f6e 742d  ze="8.8pt" font-
+000082a0: 7374 796c 653d 226e 6f72 6d61 6c22 2066  style="normal" f
+000082b0: 6f6e 742d 7765 6967 6874 3d22 626f 6c64  ont-weight="bold
+000082c0: 2220 7465 7874 2d64 6563 6f72 6174 696f  " text-decoratio
+000082d0: 6e3d 226e 6f72 6d61 6c22 2078 3d22 3230  n="normal" x="20
+000082e0: 332e 3237 3636 3430 3531 3736 3735 3822  3.2766405176758"
+000082f0: 2079 3d22 3734 352e 3336 3237 3631 3033   y="745.36276103
+00008300: 3739 3939 3922 2074 6578 742d 616e 6368  79999" text-anch
+00008310: 6f72 3d22 7374 6172 7422 2064 6f6d 696e  or="start" domin
+00008320: 616e 742d 6261 7365 6c69 6e65 3d22 616c  ant-baseline="al
+00008330: 7068 6162 6574 6963 2220 786d 6c3a 7370  phabetic" xml:sp
+00008340: 6163 653d 2270 7265 7365 7276 6522 3e5b  ace="preserve">[
+00008350: 6561 6368 c2a0 6669 656c 64c2 a069 6ec2  each..field..in.
+00008360: a065 7870 6f72 74c2 a066 6965 6c64 c2a0  .export..field..
+00008370: 6c69 7374 5d3c 2f74 6578 743e 3c2f 673e  list]</text></g>
+00008380: 3c2f 673e 3c67 2f3e 3c67 2f3e 3c67 2f3e  </g><g/><g/><g/>
+00008390: 3c67 2f3e 3c2f 673e 3c2f 673e 3c2f 673e  <g/></g></g></g>
+000083a0: 3c2f 673e 3c2f 673e 3c2f 7376 673e       </g></g></svg>
```

### Comparing `django_import_export-4.0.0rc3/docs/_static/images/import-button.png` & `django_import_export-4.0.1/docs/_static/images/import-button.png`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/docs/_static/images/import_workflow.svg` & `django_import_export-4.0.1/docs/_static/images/import_workflow.svg`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/docs/_static/images/non-field-specific-validation-error.png` & `django_import_export-4.0.1/docs/_static/images/non-field-specific-validation-error.png`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/docs/_static/images/select-for-export.png` & `django_import_export-4.0.1/docs/_static/images/select-for-export.png`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/docs/admin_integration.rst` & `django_import_export-4.0.1/docs/admin_integration.rst`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/docs/advanced_usage.rst` & `django_import_export-4.0.1/docs/advanced_usage.rst`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/docs/api_mixins.rst` & `django_import_export-4.0.1/docs/api_mixins.rst`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/docs/api_widgets.rst` & `django_import_export-4.0.1/docs/api_widgets.rst`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/docs/bulk_import.rst` & `django_import_export-4.0.1/docs/bulk_import.rst`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/docs/conf.py` & `django_import_export-4.0.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/docs/contributing.rst` & `django_import_export-4.0.1/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/docs/export_workflow.rst` & `django_import_export-4.0.1/docs/export_workflow.rst`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/docs/faq.rst` & `django_import_export-4.0.1/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/docs/getting_started.rst` & `django_import_export-4.0.1/docs/getting_started.rst`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/docs/image_src/export_workflow.txt` & `django_import_export-4.0.1/docs/image_src/export_workflow.txt`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/docs/image_src/import_workflow.txt` & `django_import_export-4.0.1/docs/image_src/import_workflow.txt`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/docs/import_workflow.rst` & `django_import_export-4.0.1/docs/import_workflow.rst`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/docs/index.rst` & `django_import_export-4.0.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/docs/installation.rst` & `django_import_export-4.0.1/docs/installation.rst`

 * *Files 1% similar despite different names*

```diff
@@ -157,15 +157,15 @@
 
 .. _import_export_skip_admin_action_export_ui:
 
 ``IMPORT_EXPORT_SKIP_ADMIN_ACTION_EXPORT_UI``
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 A boolean value which will skip the 'file format' and 'resource' select page in the Admin UI
-when the export is requested from an Admin UI action.
+when the export is requested from an :ref:`Admin UI action<export_via_admin_action>`.
 If ``TRUE`` then the first element in the 'file format' and 'resource' lists will be used.
 By default this is ``FALSE``.
 
 .. _import_export_escape_formulae_on_export:
 
 ``IMPORT_EXPORT_ESCAPE_FORMULAE_ON_EXPORT``
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
```

### Comparing `django_import_export-4.0.0rc3/docs/make.bat` & `django_import_export-4.0.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/docs/release_notes.rst` & `django_import_export-4.0.1/docs/release_notes.rst`

 * *Files 2% similar despite different names*

```diff
@@ -71,14 +71,15 @@
 
 Deprecations
 ============
 
 * The ``obj`` param passed to :meth:`~import_export.widgets.Widget.render` is deprecated.
   The :meth:`~import_export.widgets.Widget.render` method should not need to have a reference to
   model instance.
+  The call to :meth:`~import_export.widgets.Widget.render` from :meth:`~import_export.fields.Field.export` has been removed.
 
 * Use of ``ExportViewFormMixin`` is deprecated.  See `this issue <https://github.com/django-import-export/django-import-export/issues/1666>`_.
 
 * See :ref:`renamed_methods`.
 
 Admin UI
 ========
```

### Comparing `django_import_export-4.0.0rc3/docs/testing.rst` & `django_import_export-4.0.1/docs/testing.rst`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/import_export/admin.py` & `django_import_export-4.0.1/import_export/admin.py`

 * *Files 1% similar despite different names*

```diff
@@ -663,16 +663,15 @@
             "list_select_related": list_select_related,
             "list_per_page": self.list_per_page,
             "list_max_show_all": self.list_max_show_all,
             "list_editable": self.list_editable,
             "model_admin": self,
             "sortable_by": self.sortable_by,
         }
-        if django.VERSION >= (4, 0):
-            changelist_kwargs["search_help_text"] = self.search_help_text
+        changelist_kwargs["search_help_text"] = self.search_help_text
 
         class ExportChangeList(ChangeList):
             def get_results(self, request):
                 """
                 Overrides ChangeList.get_results() to bypass default operations like
                 pagination and result counting, which are not needed for export. This
                 prevents executing unnecessary COUNT queries during ChangeList
@@ -730,15 +729,15 @@
             formats,
             self.get_export_resource_classes(request),
             data=request.POST or None,
         )
         form.fields["export_items"] = MultipleChoiceField(
             widget=MultipleHiddenInput,
             required=False,
-            choices=[(o.id, o.id) for o in self.model.objects.all()],
+            choices=[(o.pk, o.pk) for o in self.model.objects.all()],
         )
         if form.is_valid():
             file_format = formats[int(form.cleaned_data["format"])]()
 
             if "export_items" in form.changed_data:
                 # this request has arisen from an Admin UI action
                 # export item pks are stored in form data
@@ -873,15 +872,15 @@
             return response
 
         form_type = self.get_export_form_class()
         formats = self.get_export_formats()
         form = form_type(
             formats=formats,
             resources=self.get_export_resource_classes(request),
-            initial={"export_items": list(queryset.values_list("id", flat=True))},
+            initial={"export_items": list(queryset.values_list("pk", flat=True))},
         )
         # selected items are to be stored as a hidden input on the form
         form.fields["export_items"] = MultipleChoiceField(
             widget=MultipleHiddenInput,
             required=False,
             choices=[(str(o), str(o)) for o in queryset.all()],
         )
```

### Comparing `django_import_export-4.0.0rc3/import_export/declarative.py` & `django_import_export-4.0.1/import_export/declarative.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/import_export/exceptions.py` & `django_import_export-4.0.1/import_export/exceptions.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/import_export/fields.py` & `django_import_export-4.0.1/import_export/fields.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,15 +142,15 @@
 
     def export(self, instance):
         """
         Returns value from the provided instance converted to export
         representation.
         """
         value = self.get_value(instance)
-        return self.widget.render(value, instance)
+        return self.widget.render(value)
 
     def get_dehydrate_method(self, field_name=None):
         """
         Returns method name to be used for dehydration of the field.
         Defaults to `dehydrate_{field_name}`
         """
         DEFAULT_DEHYDRATE_METHOD_PREFIX = "dehydrate_"
```

### Comparing `django_import_export-4.0.0rc3/import_export/formats/base_formats.py` & `django_import_export-4.0.1/import_export/formats/base_formats.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/import_export/forms.py` & `django_import_export-4.0.1/import_export/forms.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/import_export/instance_loaders.py` & `django_import_export-4.0.1/import_export/instance_loaders.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/import_export/locale/ar/LC_MESSAGES/django.mo` & `django_import_export-4.0.1/import_export/locale/ar/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/import_export/locale/ar/LC_MESSAGES/django.po` & `django_import_export-4.0.1/import_export/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/import_export/locale/bg/LC_MESSAGES/django.mo` & `django_import_export-4.0.1/import_export/locale/bg/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/import_export/locale/bg/LC_MESSAGES/django.po` & `django_import_export-4.0.1/import_export/locale/bg/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/import_export/locale/ca/LC_MESSAGES/django.mo` & `django_import_export-4.0.1/import_export/locale/ca/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/import_export/locale/ca/LC_MESSAGES/django.po` & `django_import_export-4.0.1/import_export/locale/ca/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/import_export/locale/cs/LC_MESSAGES/django.mo` & `django_import_export-4.0.1/import_export/locale/cs/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/import_export/locale/cs/LC_MESSAGES/django.po` & `django_import_export-4.0.1/import_export/locale/cs/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/import_export/locale/de/LC_MESSAGES/django.mo` & `django_import_export-4.0.1/import_export/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/import_export/locale/de/LC_MESSAGES/django.po` & `django_import_export-4.0.1/import_export/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/import_export/locale/es/LC_MESSAGES/django.mo` & `django_import_export-4.0.1/import_export/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/import_export/locale/es/LC_MESSAGES/django.po` & `django_import_export-4.0.1/import_export/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/import_export/locale/es_AR/LC_MESSAGES/django.mo` & `django_import_export-4.0.1/import_export/locale/es_AR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/import_export/locale/es_AR/LC_MESSAGES/django.po` & `django_import_export-4.0.1/import_export/locale/es_AR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/import_export/locale/fa/LC_MESSAGES/django.mo` & `django_import_export-4.0.1/import_export/locale/fa/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/import_export/locale/fa/LC_MESSAGES/django.po` & `django_import_export-4.0.1/import_export/locale/fa/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/import_export/locale/fi/LC_MESSAGES/django.mo` & `django_import_export-4.0.1/import_export/locale/fi/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/import_export/locale/fi/LC_MESSAGES/django.po` & `django_import_export-4.0.1/import_export/locale/fi/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/import_export/locale/fr/LC_MESSAGES/django.mo` & `django_import_export-4.0.1/import_export/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/import_export/locale/fr/LC_MESSAGES/django.po` & `django_import_export-4.0.1/import_export/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/import_export/locale/it/LC_MESSAGES/django.mo` & `django_import_export-4.0.1/import_export/locale/it/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/import_export/locale/it/LC_MESSAGES/django.po` & `django_import_export-4.0.1/import_export/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/import_export/locale/ja/LC_MESSAGES/django.mo` & `django_import_export-4.0.1/import_export/locale/ja/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/import_export/locale/ja/LC_MESSAGES/django.po` & `django_import_export-4.0.1/import_export/locale/ja/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/import_export/locale/ko/LC_MESSAGES/django.mo` & `django_import_export-4.0.1/import_export/locale/ko/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/import_export/locale/ko/LC_MESSAGES/django.po` & `django_import_export-4.0.1/import_export/locale/ko/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/import_export/locale/kz/LC_MESSAGES/django.mo` & `django_import_export-4.0.1/import_export/locale/kz/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/import_export/locale/kz/LC_MESSAGES/django.po` & `django_import_export-4.0.1/import_export/locale/kz/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/import_export/locale/nl/LC_MESSAGES/django.mo` & `django_import_export-4.0.1/import_export/locale/nl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/import_export/locale/nl/LC_MESSAGES/django.po` & `django_import_export-4.0.1/import_export/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/import_export/locale/pl/LC_MESSAGES/django.mo` & `django_import_export-4.0.1/import_export/locale/pl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/import_export/locale/pl/LC_MESSAGES/django.po` & `django_import_export-4.0.1/import_export/locale/pl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/import_export/locale/pt_BR/LC_MESSAGES/django.mo` & `django_import_export-4.0.1/import_export/locale/pt_BR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/import_export/locale/pt_BR/LC_MESSAGES/django.po` & `django_import_export-4.0.1/import_export/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/import_export/locale/sk/LC_MESSAGES/django.mo` & `django_import_export-4.0.1/import_export/locale/sk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/import_export/locale/sk/LC_MESSAGES/django.po` & `django_import_export-4.0.1/import_export/locale/sk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/import_export/locale/tr/LC_MESSAGES/django.mo` & `django_import_export-4.0.1/import_export/locale/tr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/import_export/locale/tr/LC_MESSAGES/django.po` & `django_import_export-4.0.1/import_export/locale/tr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/import_export/locale/zh_Hans/LC_MESSAGES/django.mo` & `django_import_export-4.0.1/import_export/locale/zh_Hans/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/import_export/locale/zh_Hans/LC_MESSAGES/django.po` & `django_import_export-4.0.1/import_export/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/import_export/mixins.py` & `django_import_export-4.0.1/import_export/mixins.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/import_export/options.py` & `django_import_export-4.0.1/import_export/options.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/import_export/resources.py` & `django_import_export-4.0.1/import_export/resources.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import functools
+import inspect
 import logging
 import traceback
 from collections import OrderedDict
 from copy import deepcopy
 from html import escape
 from warnings import warn
 
@@ -163,14 +164,21 @@
         """
         raise NotImplementedError()
 
     def get_instance(self, instance_loader, row):
         """
         Calls the :doc:`InstanceLoader <api_instance_loaders>`.
         """
+        import_id_fields = [self.fields[f] for f in self.get_import_id_fields()]
+        for field in import_id_fields:
+            if field.column_name not in row:
+                # if there is an 'import id field' which is not defined in the
+                # row, then it is not possible to return an existing instance,
+                # so no need to proceed any further
+                return
         return instance_loader.get_instance(row)
 
     def get_or_init_instance(self, instance_loader, row):
         """
         Either fetches an already existing instance or initializes a new one.
         """
         if not self._meta.force_init_instance:
@@ -1115,14 +1123,18 @@
         return kwargs.get("dry_run", False)
 
     def _check_import_id_fields(self, headers):
         import_id_fields = list()
         missing_fields = list()
         missing_headers = list()
 
+        if self.get_import_id_fields() == ["id"]:
+            # this is the default case, so ok if not present
+            return
+
         for field_name in self.get_import_id_fields():
             if field_name not in self.fields:
                 missing_fields.append(field_name)
             else:
                 import_id_fields.append(self.fields[field_name])
 
         if missing_fields:
@@ -1167,14 +1179,15 @@
         "DateField": widgets.DateWidget,
         "TimeField": widgets.TimeWidget,
         "DurationField": widgets.DurationWidget,
         "FloatField": widgets.FloatWidget,
         "IntegerField": widgets.IntegerWidget,
         "PositiveIntegerField": widgets.IntegerWidget,
         "BigIntegerField": widgets.IntegerWidget,
+        "PositiveBigIntegerField": widgets.IntegerWidget,
         "PositiveSmallIntegerField": widgets.IntegerWidget,
         "SmallIntegerField": widgets.IntegerWidget,
         "SmallAutoField": widgets.IntegerWidget,
         "AutoField": widgets.IntegerWidget,
         "BigAutoField": widgets.IntegerWidget,
         "NullBooleanField": widgets.BooleanWidget,
         "BooleanField": widgets.BooleanWidget,
@@ -1224,14 +1237,23 @@
             internal_type = f.get_internal_type()
 
         if internal_type in cls.WIDGETS_MAP:
             result = cls.WIDGETS_MAP[internal_type]
             if isinstance(result, str):
                 result = getattr(cls, result)(f)
         else:
+            # issue 1804
+            # The field class may be in a third party library as a subclass
+            # of a standard field class.
+            # iterate base classes to determine the correct widget class to use.
+            for base_class in inspect.getmro(f.__class__):
+                if base_class.__name__ in cls.WIDGETS_MAP:
+                    result = cls.WIDGETS_MAP[base_class.__name__]
+                    break
+
             try:
                 from django.contrib.postgres.fields import ArrayField
             except ImportError:
                 # ImportError: No module named psycopg2.extras
                 class ArrayField:
                     pass
```

### Comparing `django_import_export-4.0.0rc3/import_export/results.py` & `django_import_export-4.0.1/import_export/results.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/import_export/static/import_export/export_selectable_fields.js` & `django_import_export-4.0.1/import_export/static/import_export/export_selectable_fields.js`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/import_export/static/import_export/guess_format.js` & `django_import_export-4.0.1/import_export/static/import_export/guess_format.js`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/import_export/static/import_export/import.css` & `django_import_export-4.0.1/import_export/static/import_export/import.css`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/import_export/templates/admin/import_export/base.html` & `django_import_export-4.0.1/import_export/templates/admin/import_export/base.html`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/import_export/templates/admin/import_export/export.html` & `django_import_export-4.0.1/import_export/templates/admin/import_export/export.html`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/import_export/templates/admin/import_export/import.html` & `django_import_export-4.0.1/import_export/templates/admin/import_export/import.html`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/import_export/templates/admin/import_export/resource_fields_list.html` & `django_import_export-4.0.1/import_export/templates/admin/import_export/resource_fields_list.html`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/import_export/tmp_storages.py` & `django_import_export-4.0.1/import_export/tmp_storages.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/import_export/utils.py` & `django_import_export-4.0.1/import_export/utils.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/import_export/widgets.py` & `django_import_export-4.0.1/import_export/widgets.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/pyproject.toml` & `django_import_export-4.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 description = "Django application and library for importing and exporting data with included admin integration."
 keywords = ["django", "import", "export"]
 license = {file = "LICENSE"}
 requires-python = ">=3.8"
 dynamic = ["version", "readme"]
 classifiers = [
     "Framework :: Django",
-    "Framework :: Django :: 3.2",
     "Framework :: Django :: 4.2",
     "Framework :: Django :: 5.0",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: BSD License",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
```

### Comparing `django_import_export-4.0.0rc3/runtests.py` & `django_import_export-4.0.1/runtests.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/runtests.sh` & `django_import_export-4.0.1/runtests.sh`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/tests/core/admin.py` & `django_import_export-4.0.1/tests/core/admin.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     ExportActionModelAdmin,
     ImportExportModelAdmin,
     ImportMixin,
 )
 from import_export.resources import ModelResource
 
 from .forms import CustomConfirmImportForm, CustomExportForm, CustomImportForm
-from .models import Author, Book, Category, Child, EBook
+from .models import Author, Book, Category, Child, EBook, UUIDCategory
 
 
 class ChildAdmin(ImportMixin, admin.ModelAdmin):
     pass
 
 
 class BookResource(ModelResource):
@@ -37,14 +37,18 @@
     change_list_template = "core/admin/change_list.html"
 
 
 class CategoryAdmin(ExportActionModelAdmin):
     pass
 
 
+class UUIDCategoryAdmin(ExportActionModelAdmin):
+    pass
+
+
 class AuthorAdmin(ImportMixin, admin.ModelAdmin):
     pass
 
 
 class EBookResource(ModelResource):
     def __init__(self, **kwargs):
         super().__init__()
@@ -100,7 +104,8 @@
 
 
 admin.site.register(Book, BookAdmin)
 admin.site.register(Category, CategoryAdmin)
 admin.site.register(Author, AuthorAdmin)
 admin.site.register(Child, ChildAdmin)
 admin.site.register(EBook, CustomBookAdmin)
+admin.site.register(UUIDCategory, UUIDCategoryAdmin)
```

### Comparing `django_import_export-4.0.0rc3/tests/core/exports/books-empty-author-email.xlsx` & `django_import_export-4.0.1/tests/core/exports/books-empty-author-email.xlsx`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/tests/core/exports/books.json` & `django_import_export-4.0.1/tests/core/exports/books.json`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/tests/core/exports/books.xls` & `django_import_export-4.0.1/tests/core/exports/books.xls`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/tests/core/exports/books.xlsx` & `django_import_export-4.0.1/tests/core/exports/books.xlsx`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/tests/core/fixtures/book.json` & `django_import_export-4.0.1/tests/core/fixtures/book.json`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/tests/core/forms.py` & `django_import_export-4.0.1/tests/core/forms.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/tests/core/migrations/0001_initial.py` & `django_import_export-4.0.1/tests/core/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/tests/core/migrations/0003_withfloatfield.py` & `django_import_export-4.0.1/tests/core/migrations/0003_withfloatfield.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/tests/core/migrations/0004_bookwithchapters.py` & `django_import_export-4.0.1/tests/core/migrations/0004_bookwithchapters.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/tests/core/migrations/0005_addparentchild.py` & `django_import_export-4.0.1/tests/core/migrations/0005_addparentchild.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/tests/core/migrations/0007_auto_20180628_0411.py` & `django_import_export-4.0.1/tests/core/migrations/0007_auto_20180628_0411.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/tests/core/migrations/0008_auto_20190409_0846.py` & `django_import_export-4.0.1/tests/core/migrations/0008_auto_20190409_0846.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/tests/core/migrations/0009_auto_20211111_0807.py` & `django_import_export-4.0.1/tests/core/migrations/0009_auto_20211111_0807.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/tests/core/migrations/0010_uuidbook.py` & `django_import_export-4.0.1/tests/core/migrations/0010_uuidbook.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/tests/core/migrations/0011_uuidcategory_legacybook_alter_uuidbook_id_and_more.py` & `django_import_export-4.0.1/tests/core/migrations/0011_uuidcategory_legacybook_alter_uuidbook_id_and_more.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/tests/core/migrations/0014_bookwithchapternumbers.py` & `django_import_export-4.0.1/tests/core/migrations/0014_bookwithchapternumbers.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/tests/core/models.py` & `django_import_export-4.0.1/tests/core/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,14 +52,17 @@
         max_length=100,
         unique=True,
     )
 
     def __str__(self):
         return self.name
 
+    class Meta:
+        verbose_name_plural = "categories"
+
 
 class BookManager(models.Manager):
     """
     Added to enable get_by_natural_key method
     NOTE: Manager classes are only required to enable
     using the natural key functionality of ForeignKeyWidget
     """
@@ -154,14 +157,22 @@
         proxy = True
 
 
 class UUIDCategory(models.Model):
     catid = models.UUIDField(primary_key=True, default=uuid.uuid4, editable=False)
     name = models.CharField(max_length=32)
 
+    class Meta:
+        verbose_name_plural = "UUID categories"
+
 
 class UUIDBook(models.Model):
     """A model which uses a UUID pk (issue 1274)"""
 
     id = models.UUIDField(primary_key=True, default=uuid.uuid4, editable=False)
     name = models.CharField("Book name", max_length=100)
     categories = models.ManyToManyField(UUIDCategory, blank=True)
+
+
+class WithPositiveIntegerFields(models.Model):
+    big = models.PositiveBigIntegerField(null=True)
+    small = models.PositiveSmallIntegerField(null=True)
```

### Comparing `django_import_export-4.0.0rc3/tests/core/tests/admin_integration/mixins.py` & `django_import_export-4.0.1/tests/core/tests/admin_integration/mixins.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,16 +4,21 @@
 from django.contrib.auth.models import User
 
 from import_export.formats.base_formats import DEFAULT_FORMATS
 
 
 class AdminTestMixin(object):
     category_change_url = "/admin/core/category/"
+    uuid_category_change_url = "/admin/core/uuidcategory/"
+    category_export_url = "/admin/core/category/export/"
+    uuid_category_export_url = "/admin/core/uuidcategory/export/"
     book_import_url = "/admin/core/book/import/"
+    book_export_url = "/admin/core/book/export/"
     ebook_import_url = "/admin/core/ebook/import/"
+    ebook_export_url = "/admin/core/ebook/export/"
     book_process_import_url = "/admin/core/book/process_import/"
     legacybook_import_url = "/admin/core/legacybook/import/"
     legacybook_process_import_url = "/admin/core/legacybook/process_import/"
     child_import_url = "/admin/core/child/import/"
     child_process_import_url = "/admin/core/child/process_import/"
 
     def setUp(self):
```

### Comparing `django_import_export-4.0.0rc3/tests/core/tests/admin_integration/test_action.py` & `django_import_export-4.0.1/tests/core/tests/admin_integration/test_action_export.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from datetime import datetime
 from unittest import mock
 from unittest.mock import MagicMock
 
 from core.admin import CategoryAdmin
-from core.models import Book, Category
+from core.models import Book, Category, UUIDCategory
 from core.tests.admin_integration.mixins import AdminTestMixin
-from core.tests.utils import ignore_widget_deprecation_warning
 from django.contrib import admin
 from django.core.exceptions import PermissionDenied
 from django.http import HttpRequest
 from django.test import RequestFactory
 from django.test.testcases import TestCase
 from django.test.utils import override_settings
 from django.urls import reverse
@@ -36,65 +35,77 @@
         date_str = datetime.now().strftime("%Y-%m-%d")
         self.assertEqual(
             response["Content-Disposition"],
             'attachment; filename="Category-{}.csv"'.format(date_str),
         )
 
     @override_settings(IMPORT_EXPORT_SKIP_ADMIN_ACTION_EXPORT_UI=True)
-    @ignore_widget_deprecation_warning
     def test_export_skips_export_ui_page(self):
         data = {
             "action": ["export_admin_action"],
             "_selected_action": [str(self.cat1.id)],
         }
-        response = self.client.post("/admin/core/category/", data)
+        response = self.client.post(self.category_change_url, data)
         self._check_export_response(response)
 
-    @ignore_widget_deprecation_warning
     def test_export_displays_ui_select_page(self):
         data = {
             "action": ["export_admin_action"],
             "_selected_action": [str(self.cat1.id)],
         }
-        response = self.client.post("/admin/core/category/", data)
+        response = self.client.post(self.category_change_url, data)
 
         self.assertEqual(response.status_code, 200)
         self.assertIn("form", response.context)
         export_form = response.context["form"]
         data = export_form.initial
         self.assertEqual([self.cat1.id], data["export_items"])
         self.assertIn("Export 1 selected item.", str(response.content))
 
-    @ignore_widget_deprecation_warning
     def test_export_displays_ui_select_page_multiple_items(self):
         data = {
             "action": ["export_admin_action"],
             "_selected_action": [str(self.cat1.id), str(self.cat2.id)],
         }
-        response = self.client.post("/admin/core/category/", data)
+        response = self.client.post(self.category_change_url, data)
 
         self.assertEqual(response.status_code, 200)
         self.assertIn("form", response.context)
         export_form = response.context["form"]
         data = export_form.initial
         self.assertEqual(
             sorted([self.cat1.id, self.cat2.id]), sorted(data["export_items"])
         )
         self.assertIn("Export 2 selected items.", str(response.content))
 
-    @ignore_widget_deprecation_warning
+    def test_action_export_model_with_custom_PK(self):
+        # issue 1800
+        cat = UUIDCategory.objects.create(name="UUIDCategory")
+        data = {
+            "action": ["export_admin_action"],
+            "_selected_action": [str(cat.pk)],
+        }
+        response = self.client.post(self.uuid_category_change_url, data)
+
+        self.assertEqual(response.status_code, 200)
+        self.assertIn("form", response.context)
+        export_form = response.context["form"]
+        data = export_form.initial
+        self.assertEqual([cat.pk], data["export_items"])
+        self.assertIn("Export 1 selected item.", str(response.content))
+
     def test_export_post(self):
         # create a POST request with data selected from the 'action' export
         data = {
             "format": "0",
             "export_items": [str(self.cat1.id)],
             **self.resource_fields_payload,
         }
         date_str = datetime.now().strftime("%Y-%m-%d")
-        response = self.client.post("/admin/core/category/export/", data)
+        response = self.client.post(self.category_export_url, data)
         self.assertEqual(response.status_code, 200)
         self.assertTrue(response.has_header("Content-Disposition"))
         self.assertEqual(response["Content-Type"], "text/csv")
         self.assertEqual(
             response["Content-Disposition"],
             'attachment; filename="Category-{}.csv"'.format(date_str),
         )
```

### Comparing `django_import_export-4.0.0rc3/tests/core/tests/admin_integration/test_export.py` & `django_import_export-4.0.1/tests/core/tests/admin_integration/test_export.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,20 +2,17 @@
 from io import BytesIO
 from unittest import mock
 from unittest.mock import MagicMock, patch
 
 import chardet
 import tablib
 from core.admin import BookAdmin, BookResource
-from core.models import Author, Book
+from core.models import Author, Book, UUIDCategory
 from core.tests.admin_integration.mixins import AdminTestMixin
-from core.tests.utils import (
-    ignore_utcnow_deprecation_warning,
-    ignore_widget_deprecation_warning,
-)
+from core.tests.utils import ignore_utcnow_deprecation_warning
 from django.contrib.admin.sites import AdminSite
 from django.contrib.admin.views.main import ChangeList
 from django.contrib.auth.models import User
 from django.core.exceptions import FieldError
 from django.http import HttpRequest
 from django.test import RequestFactory
 from django.test.testcases import TestCase
@@ -35,25 +32,25 @@
             "bookresource_id": True,
             "bookresource_name": True,
             "bookresource_author_email": True,
             "bookresource_categories": True,
         }
 
     def test_export(self):
-        response = self.client.get("/admin/core/book/export/")
+        response = self.client.get(self.book_export_url)
         self.assertEqual(response.status_code, 200)
         self.assertNotIn("Export 0 selected items.", str(response.content))
         form = response.context["form"]
         self.assertEqual(2, len(form.fields["resource"].choices))
 
         data = {"format": "0", **self.bookresource_export_fields_payload}
         date_str = datetime.now().strftime("%Y-%m-%d")
         # Should not contain COUNT queries from ModelAdmin.get_results()
         with self.assertNumQueries(6):
-            response = self.client.post("/admin/core/book/export/", data)
+            response = self.client.post(self.book_export_url, data)
         self.assertEqual(response.status_code, 200)
         self.assertTrue(response.has_header("Content-Disposition"))
         self.assertEqual(response["Content-Type"], "text/csv")
         self.assertEqual(
             response["Content-Disposition"],
             'attachment; filename="Book-{}.csv"'.format(date_str),
         )
@@ -64,35 +61,35 @@
 
     @mock.patch("core.admin.BookAdmin.get_export_resource_kwargs")
     def test_export_passes_export_resource_kwargs(
         self, mock_get_export_resource_kwargs
     ):
         # issue 1738
         mock_get_export_resource_kwargs.return_value = {"a": 1}
-        response = self.client.get("/admin/core/book/export/")
+        response = self.client.get(self.book_export_url)
         self.assertEqual(response.status_code, 200)
         self.assertEqual(2, mock_get_export_resource_kwargs.call_count)
 
     def book_resource_init(self, **kwargs):
         # stub call to the resource constructor
         pass
 
     @mock.patch.object(BookResource, "__init__", book_resource_init)
     def test_export_passes_no_resource_constructor_params(self):
         # issue 1716
         # assert that the export call with a no-arg constructor
         # does not crash
-        response = self.client.get("/admin/core/book/export/")
+        response = self.client.get(self.book_export_url)
         self.assertEqual(response.status_code, 200)
 
     def test_get_export_queryset(self):
         model_admin = BookAdmin(Book, AdminSite())
 
         factory = RequestFactory()
-        request = factory.get("/admin/core/book/export/")
+        request = factory.get(self.book_export_url)
         request.user = User.objects.create_user("admin1")
 
         call_number = 0
 
         class MyChangeList(ChangeList):
             def get_queryset(self, request):
                 nonlocal call_number
@@ -111,15 +108,15 @@
         self.assertEqual(queryset.count(), Book.objects.count())
 
     def test_get_export_queryset_no_queryset_init(self):
         """Test if user has own ChangeList which doesn't store queryset during init"""
         model_admin = BookAdmin(Book, AdminSite())
 
         factory = RequestFactory()
-        request = factory.get("/admin/core/book/export/")
+        request = factory.get(self.book_export_url)
         request.user = User.objects.create_user("admin1")
 
         call_number = 0
 
         class MyChangeList(ChangeList):
             def __init__(self, *args, **kwargs):
                 self.filter_params = {}
@@ -166,44 +163,44 @@
             mock_export.side_effect = FieldError("some unknown error")
             data = {
                 "format": "0",
                 "resource": 1,
                 "booknameresource_id": True,
                 "booknameresource_name": True,
             }
-            response = self.client.post("/admin/core/book/export/", data)
+            response = self.client.post(self.book_export_url, data)
         self.assertEqual(response.status_code, 200)
         target_msg = "Some unknown error"
         self.assertIn(target_msg, str(response.content))
 
     def test_export_second_resource(self):
-        response = self.client.get("/admin/core/book/export/")
+        response = self.client.get(self.book_export_url)
         self.assertEqual(response.status_code, 200)
         self.assertContains(response, "Export/Import only book names")
 
         data = {
             "format": "0",
             "resource": 1,
             # Second resource is `BookNameResource`
             "booknameresource_id": True,
             "booknameresource_name": True,
         }
         date_str = datetime.now().strftime("%Y-%m-%d")
-        response = self.client.post("/admin/core/book/export/", data)
+        response = self.client.post(self.book_export_url, data)
         self.assertEqual(response.status_code, 200)
         self.assertTrue(response.has_header("Content-Disposition"))
         self.assertEqual(response["Content-Type"], "text/csv")
         self.assertEqual(
             response["Content-Disposition"],
             'attachment; filename="Book-{}.csv"'.format(date_str),
         )
         self.assertEqual(b"id,name\r\n", response.content)
 
     def test_export_displays_resources_fields(self):
-        response = self.client.get("/admin/core/book/export/")
+        response = self.client.get(self.book_export_url)
         self.assertEqual(response.status_code, 200)
         self.assertEqual(
             response.context["fields_list"],
             [
                 (
                     "BookResource",
                     [
@@ -234,95 +231,98 @@
 
     @override_settings(EXPORT_FORMATS=[])
     def test_export_empty_export_formats(self):
         with self.assertRaisesRegex(ValueError, "invalid formats list"):
             self.client.get("/admin/core/category/export/")
 
     def test_returns_xlsx_export(self):
-        response = self.client.get("/admin/core/book/export/")
+        response = self.client.get(self.book_export_url)
         self.assertEqual(response.status_code, 200)
 
         xlsx_index = self._get_input_format_index("xlsx")
         data = {"format": str(xlsx_index), **self.bookresource_export_fields_payload}
-        response = self.client.post("/admin/core/book/export/", data)
+        response = self.client.post(self.book_export_url, data)
         self.assertEqual(response.status_code, 200)
         self.assertTrue(response.has_header("Content-Disposition"))
         self.assertEqual(
             response["Content-Type"],
             "application/vnd.openxmlformats-officedocument.spreadsheetml.sheet",
         )
 
     @ignore_utcnow_deprecation_warning
     @override_settings(IMPORT_EXPORT_ESCAPE_FORMULAE_ON_EXPORT=True)
-    @ignore_widget_deprecation_warning
     def test_export_escape_formulae(self):
         Book.objects.create(id=1, name="=SUM(1+1)")
         Book.objects.create(id=2, name="<script>alert(1)</script>")
-        response = self.client.get("/admin/core/book/export/")
+        response = self.client.get(self.book_export_url)
         self.assertEqual(response.status_code, 200)
 
         xlsx_index = self._get_input_format_index("xlsx")
         data = {"format": str(xlsx_index), **self.bookresource_export_fields_payload}
-        response = self.client.post("/admin/core/book/export/", data)
+        response = self.client.post(self.book_export_url, data)
         self.assertEqual(response.status_code, 200)
         content = response.content
         wb = load_workbook(filename=BytesIO(content))
         self.assertEqual("<script>alert(1)</script>", wb.active["B2"].value)
         self.assertEqual("SUM(1+1)", wb.active["B3"].value)
 
     @override_settings(IMPORT_EXPORT_ESCAPE_FORMULAE_ON_EXPORT=True)
-    @ignore_widget_deprecation_warning
     def test_export_escape_formulae_csv(self):
         b1 = Book.objects.create(id=1, name="=SUM(1+1)")
-        response = self.client.get("/admin/core/book/export/")
+        response = self.client.get(self.book_export_url)
         self.assertEqual(response.status_code, 200)
 
         index = self._get_input_format_index("csv")
         data = {
             "format": str(index),
             "bookresource_id": True,
             "bookresource_name": True,
         }
-        response = self.client.post("/admin/core/book/export/", data)
+        response = self.client.post(self.book_export_url, data)
         self.assertIn(
             f"{b1.id},SUM(1+1)\r\n".encode(),
             response.content,
         )
 
     @override_settings(IMPORT_EXPORT_ESCAPE_FORMULAE_ON_EXPORT=False)
-    @ignore_widget_deprecation_warning
     def test_export_escape_formulae_csv_false(self):
         b1 = Book.objects.create(id=1, name="=SUM(1+1)")
-        response = self.client.get("/admin/core/book/export/")
+        response = self.client.get(self.book_export_url)
         self.assertEqual(response.status_code, 200)
 
         index = self._get_input_format_index("csv")
         data = {
             "format": str(index),
             "bookresource_id": True,
             "bookresource_name": True,
         }
-        response = self.client.post("/admin/core/book/export/", data)
+        response = self.client.post(self.book_export_url, data)
         self.assertIn(
             f"{b1.id},=SUM(1+1)\r\n".encode(),
             response.content,
         )
 
+    def test_export_model_with_custom_PK(self):
+        # issue 1800
+        UUIDCategory.objects.create(name="UUIDCategory")
+        response = self.client.get(self.uuid_category_export_url)
+        self.assertEqual(response.status_code, 200)
+        self.assertContains(response, "UUIDCategoryResource")
+
 
 class FilteredExportAdminIntegrationTest(AdminTestMixin, TestCase):
     fixtures = ["category", "book", "author"]
 
-    @ignore_widget_deprecation_warning
     def test_export_filters_by_form_param(self):
         # issue 1578
         author = Author.objects.get(name="Ian Fleming")
 
         data = {"format": "0", "author": str(author.id)}
         date_str = datetime.now().strftime("%Y-%m-%d")
-        response = self.client.post("/admin/core/ebook/export/", data)
+        response = self.client.post(self.ebook_export_url, data)
         self.assertEqual(response.status_code, 200)
         self.assertTrue(response.has_header("Content-Disposition"))
         self.assertEqual(response["Content-Type"], "text/csv")
         self.assertEqual(
             response["Content-Disposition"],
             'attachment; filename="EBook-{}.csv"'.format(date_str),
         )
@@ -419,15 +419,15 @@
             self.export_mixin.export_admin_action(self.mock_request, list())
             encoding_kwarg = mock_get_export_data.call_args_list[0][1]["encoding"]
             self.assertEqual("utf-8", encoding_kwarg)
 
 
 class TestSelectableFieldsExportPage(AdminTestMixin, TestCase):
     def test_selectable_fields_rendered_with_resource_index_attribute(self) -> None:
-        response = self.client.get("/admin/core/book/export/")
+        response = self.client.get(self.book_export_url)
 
         self.assertEqual(response.status_code, 200)
         form_resources = response.context["form"].resources
         response_content = str(response.content)
 
         for index, resource in enumerate(form_resources):
             resource_fields = resource().get_export_order()
```

### Comparing `django_import_export-4.0.0rc3/tests/core/tests/admin_integration/test_import.py` & `django_import_export-4.0.1/tests/core/tests/admin_integration/test_import.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 import os
 import warnings
 from io import StringIO
 from unittest import mock
 from unittest.mock import patch
 
-import django
 from core.admin import AuthorAdmin, BookAdmin, CustomBookAdmin, ImportMixin
 from core.models import Author, Book, EBook, Parent
 from core.tests.admin_integration.mixins import AdminTestMixin
-from core.tests.utils import ignore_widget_deprecation_warning
 from django.contrib.admin.models import DELETION, LogEntry
 from django.contrib.admin.sites import AdminSite
 from django.contrib.auth.models import User
 from django.test import RequestFactory
 from django.test.testcases import TestCase, TransactionTestCase
 from django.test.utils import override_settings
 from django.utils.translation import gettext_lazy as _
@@ -34,15 +32,14 @@
         self.assertTemplateUsed(response, "admin/change_list.html")
         self.assertTemplateUsed(response, "core/admin/change_list.html")
         self.assertContains(response, _("Import"))
         self.assertContains(response, _("Export"))
         self.assertContains(response, "Custom change list item")
 
     @override_settings(TEMPLATE_STRING_IF_INVALID="INVALID_VARIABLE")
-    @ignore_widget_deprecation_warning
     def test_import(self):
         # GET the import form
         response = self.client.get(self.book_import_url)
         self.assertEqual(response.status_code, 200)
         self.assertTemplateUsed(response, "admin/import_export/import.html")
         self.assertContains(response, 'form action=""')
 
@@ -113,15 +110,14 @@
             response,
             '<script src="/static/import_export/guess_format.js">',
             count=1,
             html=True,
         )
 
     @override_settings(TEMPLATE_STRING_IF_INVALID="INVALID_VARIABLE")
-    @ignore_widget_deprecation_warning
     def test_import_second_resource(self):
         Book.objects.create(id=1)
 
         # GET the import form
         response = self.client.get(self.book_import_url)
         self.assertContains(response, "Export/Import only book names")
         self.assertEqual(response.status_code, 200)
@@ -158,53 +154,43 @@
             )
             response = self._do_import_post(self.book_import_url, "books.csv")
         self.assertEqual(response.status_code, 200)
         target_msg = (
             "'UnicodeDecodeError' encountered while trying to read file. "
             "Ensure you have chosen the correct format for the file."
         )
-        # required for testing via tox
-        # remove after django 5.0 released
-        if django.VERSION >= (4, 0):
-            with warnings.catch_warnings():
-                warnings.filterwarnings("ignore", category=DeprecationWarning)
-                try:
-                    self.assertFormError(
-                        response.context["form"], "import_file", target_msg
-                    )
-                except TypeError:
-                    self.assertFormError(response, "form", "import_file", target_msg)
-        else:
-            self.assertFormError(response, "form", "import_file", target_msg)
+        with warnings.catch_warnings():
+            warnings.filterwarnings("ignore", category=DeprecationWarning)
+            try:
+                self.assertFormError(
+                    response.context["form"], "import_file", target_msg
+                )
+            except TypeError:
+                self.assertFormError(response, "form", "import_file", target_msg)
 
     def test_import_action_handles_ValueError_as_form_error(self):
         with mock.patch(
             "import_export.admin.TempFolderStorage.read"
         ) as mock_tmp_folder_storage:
             mock_tmp_folder_storage.side_effect = ValueError("some unknown error")
             response = self._do_import_post(self.book_import_url, "books.csv")
         self.assertEqual(response.status_code, 200)
         target_msg = (
             "'ValueError' encountered while trying to read file. "
             "Ensure you have chosen the correct format for the file."
         )
 
-        # required for testing via tox
-        # remove after django 5.0 released
-        if django.VERSION >= (4, 0):
-            with warnings.catch_warnings():
-                warnings.filterwarnings("ignore", category=DeprecationWarning)
-                try:
-                    self.assertFormError(
-                        response.context["form"], "import_file", target_msg
-                    )
-                except TypeError:
-                    self.assertFormError(response, "form", "import_file", target_msg)
-        else:
-            self.assertFormError(response, "form", "import_file", target_msg)
+        with warnings.catch_warnings():
+            warnings.filterwarnings("ignore", category=DeprecationWarning)
+            try:
+                self.assertFormError(
+                    response.context["form"], "import_file", target_msg
+                )
+            except TypeError:
+                self.assertFormError(response, "form", "import_file", target_msg)
 
     def test_import_action_handles_FieldError(self):
         # issue 1722
         with mock.patch(
             "import_export.resources.Resource._check_import_id_fields"
         ) as mock_check_import_id_fields:
             mock_check_import_id_fields.side_effect = FieldError("some unknown error")
@@ -222,27 +208,22 @@
             response = self._do_import_post(self.book_import_url, "books.csv")
         self.assertEqual(response.status_code, 200)
         target_msg = (
             "Se encontró 'ValueError' mientras se intentaba leer el archivo. "
             "Asegúrese que seleccionó el formato correcto para el archivo."
         )
 
-        # required for testing via tox
-        # remove after django 5.0 released
-        if django.VERSION >= (4, 0):
-            with warnings.catch_warnings():
-                warnings.filterwarnings("ignore", category=DeprecationWarning)
-                try:
-                    self.assertFormError(
-                        response.context["form"], "import_file", target_msg
-                    )
-                except TypeError:
-                    self.assertFormError(response, "form", "import_file", target_msg)
-        else:
-            self.assertFormError(response, "form", "import_file", target_msg)
+        with warnings.catch_warnings():
+            warnings.filterwarnings("ignore", category=DeprecationWarning)
+            try:
+                self.assertFormError(
+                    response.context["form"], "import_file", target_msg
+                )
+            except TypeError:
+                self.assertFormError(response, "form", "import_file", target_msg)
 
     def test_import_action_invalidates_data_sheet_with_no_headers_or_data(self):
         # GET the import form
         response = self.client.get(self.book_import_url)
         self.assertEqual(response.status_code, 200)
         self.assertTemplateUsed(response, "admin/import_export/import.html")
         self.assertContains(response, 'form action=""')
@@ -252,29 +233,23 @@
         )
         self.assertEqual(response.status_code, 200)
         target_msg = (
             "No valid data to import. Ensure your file "
             "has the correct headers or data for import."
         )
 
-        # required for testing via tox
-        # remove after django 5.0 released
-        if django.VERSION >= (4, 0):
-            with warnings.catch_warnings():
-                warnings.filterwarnings("ignore", category=DeprecationWarning)
-                try:
-                    self.assertFormError(
-                        response.context["form"], "import_file", target_msg
-                    )
-                except TypeError:
-                    self.assertFormError(response, "form", "import_file", target_msg)
-        else:
-            self.assertFormError(response, "form", "import_file", target_msg)
+        with warnings.catch_warnings():
+            warnings.filterwarnings("ignore", category=DeprecationWarning)
+            try:
+                self.assertFormError(
+                    response.context["form"], "import_file", target_msg
+                )
+            except TypeError:
+                self.assertFormError(response, "form", "import_file", target_msg)
 
-    @ignore_widget_deprecation_warning
     def test_delete_from_admin(self):
         # test delete from admin site (see #432)
 
         # create a book which can be deleted
         b = Book.objects.create(id=1)
 
         response = self._do_import_post(self.book_import_url, "books-for-delete.csv")
@@ -288,15 +263,14 @@
         deleted_entry = LogEntry.objects.latest("id")
         self.assertEqual("delete through import_export", deleted_entry.change_message)
         self.assertEqual(DELETION, deleted_entry.action_flag)
         self.assertEqual(b.id, int(deleted_entry.object_id))
         self.assertEqual("", deleted_entry.object_repr)
 
     @override_settings(TEMPLATE_STRING_IF_INVALID="INVALID_VARIABLE")
-    @ignore_widget_deprecation_warning
     def test_import_mac(self):
         # GET the import form
         response = self.client.get(self.book_import_url)
         self.assertEqual(response.status_code, 200)
         self.assertTemplateUsed(response, "admin/import_export/import.html")
         self.assertContains(response, 'form action=""')
 
@@ -353,43 +327,40 @@
         with self.assertRaises(FileNotFoundError):
             self.client.post(self.book_process_import_url, data)
 
     def test_csrf(self):
         response = self.client.get(self.book_process_import_url)
         self.assertEqual(response.status_code, 405)
 
-    @ignore_widget_deprecation_warning
     def test_import_log_entry(self):
         response = self._do_import_post(self.book_import_url, "books.csv")
 
         self.assertEqual(response.status_code, 200)
         confirm_form = response.context["confirm_form"]
         data = confirm_form.initial
         response = self.client.post(self.book_process_import_url, data, follow=True)
         self.assertEqual(response.status_code, 200)
         book = LogEntry.objects.latest("id")
         self.assertEqual(book.object_repr, "Some book")
         self.assertEqual(book.object_id, str(1))
 
-    @ignore_widget_deprecation_warning
     def test_import_log_entry_with_fk(self):
         Parent.objects.create(id=1234, name="Some Parent")
         response = self._do_import_post(self.child_import_url, "child.csv")
         self.assertEqual(response.status_code, 200)
         confirm_form = response.context["confirm_form"]
         data = confirm_form.initial
         response = self.client.post(
             "/admin/core/child/process_import/", data, follow=True
         )
         self.assertEqual(response.status_code, 200)
         child = LogEntry.objects.latest("id")
         self.assertEqual(child.object_repr, "Some - child of Some Parent")
         self.assertEqual(child.object_id, str(1))
 
-    @ignore_widget_deprecation_warning
     def test_import_with_customized_forms(self):
         """Test if admin import works if forms are customized"""
         # We reuse import scheme from `test_import` to import books.csv.
         # We use customized BookAdmin (CustomBookAdmin) with modified import
         # form, which requires Author to be selected (from available authors).
         # Note that url is /admin/core/ebook/import (and not: ...book/import)!
 
@@ -558,55 +529,51 @@
         self.data = {"format": "0", "import_file": self.filedata}
         self.model_admin = BookAdmin(Book, AdminSite())
 
         factory = RequestFactory()
         self.request = factory.post(self.book_import_url, self.data, follow=True)
         self.request.user = User.objects.create_user("admin1")
 
-    @ignore_widget_deprecation_warning
     def test_result_error_display_default(self):
         response = self.model_admin.import_action(self.request)
         response.render()
         self.assertIn("import-error-display-message", str(response.content))
         self.assertIn(
             "Line number: 1 - Author matching query does not exist.",
             str(response.content),
         )
         self.assertNotIn("import-error-display-row", str(response.content))
         self.assertNotIn("import-error-display-traceback", str(response.content))
 
-    @ignore_widget_deprecation_warning
     def test_result_error_display_message_only(self):
         self.model_admin.import_error_display = ("message",)
 
         response = self.model_admin.import_action(self.request)
         response.render()
         self.assertIn(
             "Line number: 1 - Author matching query does not exist.",
             str(response.content),
         )
         self.assertIn("import-error-display-message", str(response.content))
         self.assertNotIn("import-error-display-row", str(response.content))
         self.assertNotIn("import-error-display-traceback", str(response.content))
 
-    @ignore_widget_deprecation_warning
     def test_result_error_display_row_only(self):
         self.model_admin.import_error_display = ("row",)
 
         response = self.model_admin.import_action(self.request)
         response.render()
         self.assertNotIn(
             "Line number: 1 - Author matching query does not exist.",
             str(response.content),
         )
         self.assertNotIn("import-error-display-message", str(response.content))
         self.assertIn("import-error-display-row", str(response.content))
         self.assertNotIn("import-error-display-traceback", str(response.content))
 
-    @ignore_widget_deprecation_warning
     def test_result_error_display_traceback_only(self):
         self.model_admin.import_error_display = ("traceback",)
 
         response = self.model_admin.import_action(self.request)
         response.render()
         self.assertNotIn(
             "Line number: 1 - Author matching query does not exist.",
@@ -630,92 +597,80 @@
             encoding=encoding,
             str_in_response="test@example.com",
         )
 
     @override_settings(
         IMPORT_EXPORT_TMP_STORAGE_CLASS="import_export.tmp_storages.TempFolderStorage"
     )
-    @ignore_widget_deprecation_warning
     def test_import_action_handles_TempFolderStorage_read(self):
         self._is_str_in_response("books.csv", "0")
 
     @override_settings(
         IMPORT_EXPORT_TMP_STORAGE_CLASS="import_export.tmp_storages.TempFolderStorage"
     )
-    @ignore_widget_deprecation_warning
     def test_import_action_handles_TempFolderStorage_read_mac(self):
         self._is_str_in_response("books-mac.csv", "0")
 
     @override_settings(
         IMPORT_EXPORT_TMP_STORAGE_CLASS="import_export.tmp_storages.TempFolderStorage"
     )
-    @ignore_widget_deprecation_warning
     def test_import_action_handles_TempFolderStorage_read_iso_8859_1(self):
         self._is_str_in_response("books-ISO-8859-1.csv", "0", "ISO-8859-1")
 
     @override_settings(
         IMPORT_EXPORT_TMP_STORAGE_CLASS="import_export.tmp_storages.TempFolderStorage"
     )
-    @ignore_widget_deprecation_warning
     def test_import_action_handles_TempFolderStorage_read_binary(self):
         self._is_str_in_response("books.xls", "1")
 
     @override_settings(
         IMPORT_EXPORT_TMP_STORAGE_CLASS="import_export.tmp_storages.CacheStorage"
     )
-    @ignore_widget_deprecation_warning
     def test_import_action_handles_CacheStorage_read(self):
         self._is_str_in_response("books.csv", "0")
 
     @override_settings(
         IMPORT_EXPORT_TMP_STORAGE_CLASS="import_export.tmp_storages.CacheStorage"
     )
-    @ignore_widget_deprecation_warning
     def test_import_action_handles_CacheStorage_read_mac(self):
         self._is_str_in_response("books-mac.csv", "0")
 
     @override_settings(
         IMPORT_EXPORT_TMP_STORAGE_CLASS="import_export.tmp_storages.CacheStorage"
     )
-    @ignore_widget_deprecation_warning
     def test_import_action_handles_CacheStorage_read_iso_8859_1(self):
         self._is_str_in_response("books-ISO-8859-1.csv", "0", "ISO-8859-1")
 
     @override_settings(
         IMPORT_EXPORT_TMP_STORAGE_CLASS="import_export.tmp_storages.CacheStorage"
     )
-    @ignore_widget_deprecation_warning
     def test_import_action_handles_CacheStorage_read_binary(self):
         self._is_str_in_response("books.xls", "1")
 
     @override_settings(
         IMPORT_EXPORT_TMP_STORAGE_CLASS="import_export.tmp_storages.MediaStorage"
     )
-    @ignore_widget_deprecation_warning
     def test_import_action_handles_MediaStorage_read(self):
         self._is_str_in_response("books.csv", "0")
 
     @override_settings(
         IMPORT_EXPORT_TMP_STORAGE_CLASS="import_export.tmp_storages.MediaStorage"
     )
-    @ignore_widget_deprecation_warning
     def test_import_action_handles_MediaStorage_read_mac(self):
         self._is_str_in_response("books-mac.csv", "0")
 
     @override_settings(
         IMPORT_EXPORT_TMP_STORAGE_CLASS="import_export.tmp_storages.MediaStorage"
     )
-    @ignore_widget_deprecation_warning
     def test_import_action_handles_MediaStorage_read_iso_8859_1(self):
         self._is_str_in_response("books-ISO-8859-1.csv", "0", "ISO-8859-1")
 
     @override_settings(
         IMPORT_EXPORT_TMP_STORAGE_CLASS="import_export.tmp_storages.MediaStorage"
     )
-    @ignore_widget_deprecation_warning
     def test_import_action_handles_MediaStorage_read_binary(self):
         self._is_str_in_response("books.xls", "1")
 
 
 class CompleteImportEncodingTest(AdminTestMixin, TestCase):
     """Test handling 'complete import' step using different file encodings
     and storage types.
@@ -734,92 +689,80 @@
             response,
             "Import finished: 1 new, 0 updated, 0 deleted and 0 skipped books.",
         )
 
     @override_settings(
         IMPORT_EXPORT_TMP_STORAGE_CLASS="import_export.tmp_storages.TempFolderStorage"
     )
-    @ignore_widget_deprecation_warning
     def test_import_action_handles_TempFolderStorage_read(self):
         self._is_str_in_response("books.csv", "0")
 
     @override_settings(
         IMPORT_EXPORT_TMP_STORAGE_CLASS="import_export.tmp_storages.TempFolderStorage"
     )
-    @ignore_widget_deprecation_warning
     def test_import_action_handles_TempFolderStorage_read_mac(self):
         self._is_str_in_response("books-mac.csv", "0")
 
     @override_settings(
         IMPORT_EXPORT_TMP_STORAGE_CLASS="import_export.tmp_storages.TempFolderStorage"
     )
-    @ignore_widget_deprecation_warning
     def test_import_action_handles_TempFolderStorage_read_iso_8859_1(self):
         self._is_str_in_response("books-ISO-8859-1.csv", "0", "ISO-8859-1")
 
     @override_settings(
         IMPORT_EXPORT_TMP_STORAGE_CLASS="import_export.tmp_storages.TempFolderStorage"
     )
-    @ignore_widget_deprecation_warning
     def test_import_action_handles_TempFolderStorage_read_binary(self):
         self._is_str_in_response("books.xls", "1")
 
     @override_settings(
         IMPORT_EXPORT_TMP_STORAGE_CLASS="import_export.tmp_storages.CacheStorage"
     )
-    @ignore_widget_deprecation_warning
     def test_import_action_handles_CacheStorage_read(self):
         self._is_str_in_response("books.csv", "0")
 
     @override_settings(
         IMPORT_EXPORT_TMP_STORAGE_CLASS="import_export.tmp_storages.CacheStorage"
     )
-    @ignore_widget_deprecation_warning
     def test_import_action_handles_CacheStorage_read_mac(self):
         self._is_str_in_response("books-mac.csv", "0")
 
     @override_settings(
         IMPORT_EXPORT_TMP_STORAGE_CLASS="import_export.tmp_storages.CacheStorage"
     )
-    @ignore_widget_deprecation_warning
     def test_import_action_handles_CacheStorage_read_iso_8859_1(self):
         self._is_str_in_response("books-ISO-8859-1.csv", "0", "ISO-8859-1")
 
     @override_settings(
         IMPORT_EXPORT_TMP_STORAGE_CLASS="import_export.tmp_storages.CacheStorage"
     )
-    @ignore_widget_deprecation_warning
     def test_import_action_handles_CacheStorage_read_binary(self):
         self._is_str_in_response("books.xls", "1")
 
     @override_settings(
         IMPORT_EXPORT_TMP_STORAGE_CLASS="import_export.tmp_storages.MediaStorage"
     )
-    @ignore_widget_deprecation_warning
     def test_import_action_handles_MediaStorage_read(self):
         self._is_str_in_response("books.csv", "0")
 
     @override_settings(
         IMPORT_EXPORT_TMP_STORAGE_CLASS="import_export.tmp_storages.MediaStorage"
     )
-    @ignore_widget_deprecation_warning
     def test_import_action_handles_MediaStorage_read_mac(self):
         self._is_str_in_response("books-mac.csv", "0")
 
     @override_settings(
         IMPORT_EXPORT_TMP_STORAGE_CLASS="import_export.tmp_storages.MediaStorage"
     )
-    @ignore_widget_deprecation_warning
     def test_import_action_handles_MediaStorage_read_iso_8859_1(self):
         self._is_str_in_response("books-ISO-8859-1.csv", "0", "ISO-8859-1")
 
     @override_settings(
         IMPORT_EXPORT_TMP_STORAGE_CLASS="import_export.tmp_storages.MediaStorage"
     )
-    @ignore_widget_deprecation_warning
     def test_import_action_handles_MediaStorage_read_binary(self):
         self._is_str_in_response("books.xls", "1")
 
 
 @override_settings(IMPORT_EXPORT_SKIP_ADMIN_CONFIRM=True)
 class TestImportSkipConfirm(AdminTestMixin, TransactionTestCase):
     fixtures = ["author"]
@@ -860,26 +803,24 @@
             encoding=encoding,
             follow=follow,
         )
         self.assertEqual(response.status_code, status_code)
         if regex_in_response is not None:
             self.assertRegex(str(response.content), regex_in_response)
 
-    @ignore_widget_deprecation_warning
     def test_import_action_create(self):
         self._is_str_in_response(
             "books.csv",
             "0",
             follow=True,
             str_in_response="Import finished: 1 new, 0 updated, "
             + "0 deleted and 0 skipped books.",
         )
         self.assertEqual(1, Book.objects.count())
 
-    @ignore_widget_deprecation_warning
     def test_import_action_invalid_date(self):
         # test that a row with an invalid date redirects to errors page
         index = self._get_input_format_index("csv")
         response = self._do_import_post(
             self.book_import_url, "books-invalid-date.csv", index
         )
         result = response.context["result"]
@@ -888,72 +829,66 @@
         self.assertEqual(
             "Value could not be parsed using defined date formats.",
             result.invalid_rows[0].error.messages[0],
         )
         # no rows should be imported because we rollback on validation errors
         self.assertEqual(0, Book.objects.count())
 
-    @ignore_widget_deprecation_warning
     def test_import_action_error_on_save(self):
         with mock.patch("core.models.Book.save") as mock_save:
             mock_save.side_effect = ValueError("some unknown error")
             response = self._do_import_post(self.book_import_url, "books.csv")
         self.assertIn("some unknown error", str(response.content))
 
     @override_settings(IMPORT_EXPORT_USE_TRANSACTIONS=True)
     def test_import_transaction_enabled_validation_error(self):
         # with transactions enabled, a validation error should cause the entire
         # import to be rolled back
         self._do_import_post(self.book_import_url, "books-invalid-date.csv")
         self.assertEqual(0, Book.objects.count())
 
     @override_settings(IMPORT_EXPORT_USE_TRANSACTIONS=False)
-    @ignore_widget_deprecation_warning
     def test_import_transaction_disabled_validation_error(self):
         # with transactions disabled, a validation error should not cause the entire
         # import to fail
         self._do_import_post(self.book_import_url, "books-invalid-date.csv")
         self.assertEqual(1, Book.objects.count())
 
     @override_settings(IMPORT_EXPORT_USE_TRANSACTIONS=True)
-    @ignore_widget_deprecation_warning
     def test_import_transaction_enabled_core_error(self):
         # test that if we send a file with multiple rows,
         # and transactions is enabled, a core error means that
         # no instances are persisted
         index = self._get_input_format_index("json")
         with mock.patch("core.admin.BookResource.skip_row") as mock_skip:
             mock_skip.side_effect = [None, ValueError("some unknown error"), None]
             response = self._do_import_post(self.book_import_url, "books.json", index)
         self.assertIn("some unknown error", str(response.content))
         self.assertEqual(0, Book.objects.count())
 
     @override_settings(IMPORT_EXPORT_USE_TRANSACTIONS=False)
-    @ignore_widget_deprecation_warning
     def test_import_transaction_disabled_core_error(self):
         # with transactions disabled, a core (db constraint) error should not cause the
         # entire import to fail
         index = self._get_input_format_index("json")
         with mock.patch("core.admin.BookResource.skip_row") as mock_skip:
             mock_skip.side_effect = [None, ValueError("some unknown error"), None]
             response = self._do_import_post(self.book_import_url, "books.json", index)
         self.assertIn("some unknown error", str(response.content))
         self.assertEqual(2, Book.objects.count())
 
-    @ignore_widget_deprecation_warning
     def test_import_action_mac(self):
         self._is_str_in_response(
             "books-mac.csv",
             "0",
             follow=True,
             str_in_response="Import finished: 1 new, 0 updated, "
             + "0 deleted and 0 skipped books.",
         )
 
-    @ignore_widget_deprecation_warning
     def test_import_action_iso_8859_1(self):
         self._is_str_in_response(
             "books-ISO-8859-1.csv",
             "0",
             "ISO-8859-1",
             follow=True,
             str_in_response="Import finished: 1 new, 0 updated, "
@@ -968,15 +903,14 @@
             follow=True,
             encoding="utf-8-sig",
             regex_in_response=(
                 ".*UnicodeDecodeError.* encountered " "while trying to read file"
             ),
         )
 
-    @ignore_widget_deprecation_warning
     def test_import_action_binary(self):
         self._is_str_in_response(
             "books.xls",
             "1",
             follow=True,
             str_in_response="Import finished: 1 new, 0 updated, "
             + "0 deleted and 0 skipped books.",
@@ -984,15 +918,14 @@
 
 
 class ConfirmImportPreviewOrderTest(AdminTestMixin, TestCase):
     """Test preview order displayed correctly (issue 1784)."""
 
     fixtures = ["author"]
 
-    @ignore_widget_deprecation_warning
     def test_import_preview_order(self):
         author_id = Author.objects.first().id
         response = self._do_import_post(
             self.ebook_import_url,
             "books.csv",
             input_format="0",
             data={"author": author_id},
```

### Comparing `django_import_export-4.0.0rc3/tests/core/tests/admin_integration/test_views.py` & `django_import_export-4.0.1/tests/core/tests/admin_integration/test_views.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/tests/core/tests/resources.py` & `django_import_export-4.0.1/tests/core/tests/resources.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/tests/core/tests/test_base_formats.py` & `django_import_export-4.0.1/tests/core/tests/test_base_formats.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/tests/core/tests/test_declarative.py` & `django_import_export-4.0.1/tests/core/tests/test_declarative.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/tests/core/tests/test_fields.py` & `django_import_export-4.0.1/tests/core/tests/test_fields.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/tests/core/tests/test_forms.py` & `django_import_export-4.0.1/tests/core/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/tests/core/tests/test_instance_loaders.py` & `django_import_export-4.0.1/tests/core/tests/test_instance_loaders.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/tests/core/tests/test_invalidrow.py` & `django_import_export-4.0.1/tests/core/tests/test_invalidrow.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/tests/core/tests/test_mixins.py` & `django_import_export-4.0.1/tests/core/tests/test_mixins.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,14 @@
 from django.http import HttpRequest
 from django.test.testcases import TestCase
 from django.urls import reverse
 
 from import_export import admin, formats, forms, mixins, resources
 from import_export.resources import modelresource_factory
 
-from .utils import ignore_widget_deprecation_warning
-
 
 class ExportViewMixinTest(TestCase):
     class TestExportForm(forms.ExportForm):
         cleaned_data = dict()
 
     def setUp(self):
         self.url = reverse("export-category")
@@ -29,15 +27,14 @@
         self.form.cleaned_data["format"] = "0"
 
     def test_get(self):
         response = self.client.get(self.url)
         self.assertContains(response, self.cat1.name, status_code=200)
         self.assertEqual(response["Content-Type"], "text/html; charset=utf-8")
 
-    @ignore_widget_deprecation_warning
     def test_post(self):
         data = {"format": "0", "categoryresource_id": True}
         with warnings.catch_warnings():
             warnings.filterwarnings("ignore", category=DeprecationWarning)
             response = self.client.post(self.url, data)
         self.assertContains(response, self.cat1.name, status_code=200)
         self.assertTrue(response.has_header("Content-Disposition"))
```

### Comparing `django_import_export-4.0.0rc3/tests/core/tests/test_permissions.py` & `django_import_export-4.0.1/tests/core/tests/test_permissions.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 import os.path
 
 from core.models import Category
 from django.contrib.auth.models import Permission, User
 from django.test.testcases import TestCase
 from django.test.utils import override_settings
 
-from .utils import ignore_widget_deprecation_warning
-
 
 class ImportExportPermissionTest(TestCase):
     def setUp(self):
         user = User.objects.create_user("admin", "admin@example.com", "password")
         user.is_staff = True
         user.is_superuser = False
         user.save()
@@ -19,15 +17,14 @@
         self.client.login(username="admin", password="password")
 
     def set_user_model_permission(self, action, model_name):
         permission = Permission.objects.get(codename="%s_%s" % (action, model_name))
         self.user.user_permissions.add(permission)
 
     @override_settings(IMPORT_EXPORT_IMPORT_PERMISSION_CODE="change")
-    @ignore_widget_deprecation_warning
     def test_import(self):
         # user has no permission to import
         response = self.client.get("/admin/core/book/import/")
         self.assertEqual(response.status_code, 403)
 
         # POST the import form
         input_format = "0"
```

### Comparing `django_import_export-4.0.0rc3/tests/core/tests/test_resources/test_bulk_operations.py` & `django_import_export-4.0.1/tests/core/tests/test_resources/test_bulk_operations.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from unittest import mock
 
 import tablib
 from core.models import Book, UUIDBook
-from core.tests.utils import ignore_widget_deprecation_warning
 from django.core.exceptions import ValidationError
 from django.test import TestCase
 
 from import_export import exceptions, fields, resources, widgets
 from import_export.instance_loaders import ModelInstanceLoader
 
 
@@ -27,38 +26,35 @@
         rows = model.objects.all().values_list("id", "name")
         updated_rows = [(r[0], "UPDATED") for r in rows]
         self.dataset = tablib.Dataset(*updated_rows, headers=["id", "name"])
 
 
 class BulkCreateTest(BulkTest):
     @mock.patch("core.models.Book.objects.bulk_create")
-    @ignore_widget_deprecation_warning
     def test_bulk_create_does_not_call_object_save(self, mock_bulk_create):
         with mock.patch("core.models.Book.save") as mock_obj_save:
             self.resource.import_data(self.dataset)
             mock_obj_save.assert_not_called()
         mock_bulk_create.assert_called_with(mock.ANY, batch_size=None)
 
     @mock.patch("core.models.Book.objects.bulk_create")
-    @ignore_widget_deprecation_warning
     def test_bulk_create_batch_size_of_5(self, mock_bulk_create):
         class _BookResource(resources.ModelResource):
             class Meta:
                 model = Book
                 use_bulk = True
                 batch_size = 5
 
         resource = _BookResource()
         result = resource.import_data(self.dataset)
         self.assertEqual(2, mock_bulk_create.call_count)
         mock_bulk_create.assert_called_with(mock.ANY, batch_size=5)
         self.assertEqual(10, result.total_rows)
 
     @mock.patch("core.models.UUIDBook.objects.bulk_create")
-    @ignore_widget_deprecation_warning
     def test_bulk_create_uuid_model(self, mock_bulk_create):
         """Test create of a Model which defines uuid not pk (issue #1274)"""
 
         class _UUIDBookResource(resources.ModelResource):
             class Meta:
                 model = UUIDBook
                 use_bulk = True
@@ -71,15 +67,14 @@
         resource = _UUIDBookResource()
         result = resource.import_data(self.dataset)
         self.assertEqual(2, mock_bulk_create.call_count)
         mock_bulk_create.assert_called_with(mock.ANY, batch_size=5)
         self.assertEqual(10, result.total_rows)
 
     @mock.patch("core.models.Book.objects.bulk_create")
-    @ignore_widget_deprecation_warning
     def test_bulk_create_no_batch_size(self, mock_bulk_create):
         class _BookResource(resources.ModelResource):
             class Meta:
                 model = Book
                 use_bulk = True
                 batch_size = None
 
@@ -87,30 +82,28 @@
         result = resource.import_data(self.dataset)
         self.assertEqual(1, mock_bulk_create.call_count)
         mock_bulk_create.assert_called_with(mock.ANY, batch_size=None)
         self.assertEqual(10, result.total_rows)
         self.assertEqual(10, result.totals["new"])
 
     @mock.patch("core.models.Book.objects.bulk_create")
-    @ignore_widget_deprecation_warning
     def test_bulk_create_called_dry_run(self, mock_bulk_create):
         class _BookResource(resources.ModelResource):
             class Meta:
                 model = Book
                 use_bulk = True
                 batch_size = None
 
         resource = _BookResource()
         result = resource.import_data(self.dataset, dry_run=True)
         self.assertEqual(1, mock_bulk_create.call_count)
         self.assertEqual(10, result.total_rows)
         self.assertEqual(10, result.totals["new"])
 
     @mock.patch("core.models.Book.objects.bulk_create")
-    @ignore_widget_deprecation_warning
     def test_bulk_create_not_called_when_not_using_transactions(self, mock_bulk_create):
         class _BookResource(resources.ModelResource):
             def import_data(
                 self,
                 dataset,
                 dry_run=False,
                 raise_errors=False,
@@ -134,52 +127,48 @@
                 use_bulk = True
 
         resource = _BookResource()
         resource.import_data(self.dataset, dry_run=True)
         mock_bulk_create.assert_not_called()
 
     @mock.patch("core.models.Book.objects.bulk_create")
-    @ignore_widget_deprecation_warning
     def test_bulk_create_batch_size_of_4(self, mock_bulk_create):
         class _BookResource(resources.ModelResource):
             class Meta:
                 model = Book
                 use_bulk = True
                 batch_size = 4
 
         resource = _BookResource()
         result = resource.import_data(self.dataset)
         self.assertEqual(3, mock_bulk_create.call_count)
         self.assertEqual(10, result.total_rows)
         self.assertEqual(10, result.totals["new"])
 
-    @ignore_widget_deprecation_warning
     def test_no_changes_for_errors_if_use_transactions_enabled(self):
         with mock.patch("import_export.results.Result.has_errors") as mock_has_errors:
             mock_has_errors.return_val = True
             self.resource.import_data(self.dataset)
         self.assertEqual(0, Book.objects.count())
 
     @mock.patch("core.models.Book.objects.bulk_create")
-    @ignore_widget_deprecation_warning
     def test_bulk_create_use_bulk_disabled(self, mock_bulk_create):
         class _BookResource(resources.ModelResource):
             class Meta:
                 model = Book
                 use_bulk = False
 
         resource = _BookResource()
         result = resource.import_data(self.dataset)
         mock_bulk_create.assert_not_called()
         self.assertEqual(10, Book.objects.count())
         self.assertEqual(10, result.total_rows)
         self.assertEqual(10, result.totals["new"])
 
     @mock.patch("core.models.Book.objects.bulk_create")
-    @ignore_widget_deprecation_warning
     def test_bulk_create_bad_batch_size_value(self, mock_bulk_create):
         class _BookResource(resources.ModelResource):
             class Meta:
                 model = Book
                 use_bulk = True
                 batch_size = "a"
 
@@ -198,15 +187,14 @@
 
         resource = _BookResource()
         with self.assertRaises(ValueError):
             resource.import_data(self.dataset)
         mock_bulk_create.assert_not_called()
 
     @mock.patch("core.models.Book.objects.bulk_create")
-    @ignore_widget_deprecation_warning
     def test_bulk_create_oversized_batch_size_value(self, mock_bulk_create):
         class _BookResource(resources.ModelResource):
             class Meta:
                 model = Book
                 use_bulk = True
                 batch_size = 100
 
@@ -214,15 +202,14 @@
         result = resource.import_data(self.dataset)
         self.assertEqual(1, mock_bulk_create.call_count)
         mock_bulk_create.assert_called_with(mock.ANY, batch_size=None)
         self.assertEqual(10, result.total_rows)
         self.assertEqual(10, result.totals["new"])
 
     @mock.patch("core.models.Book.objects.bulk_create")
-    @ignore_widget_deprecation_warning
     def test_bulk_create_logs_exception(self, mock_bulk_create):
         e = ValidationError("invalid field")
         mock_bulk_create.side_effect = e
 
         class _BookResource(resources.ModelResource):
             class Meta:
                 model = Book
@@ -231,44 +218,41 @@
 
         resource = _BookResource()
         with mock.patch("logging.Logger.debug") as mock_exception:
             resource.import_data(self.dataset)
             mock_exception.assert_called_with(e, exc_info=e)
 
     @mock.patch("core.models.Book.objects.bulk_create")
-    @ignore_widget_deprecation_warning
     def test_bulk_create_raises_exception(self, mock_bulk_create):
         mock_bulk_create.side_effect = ValidationError("invalid field")
 
         class _BookResource(resources.ModelResource):
             class Meta:
                 model = Book
                 use_bulk = True
                 batch_size = 100
 
         resource = _BookResource()
         with self.assertRaises(exceptions.ImportError):
             resource.import_data(self.dataset, raise_errors=True)
 
     @mock.patch("core.models.Book.objects.bulk_create")
-    @ignore_widget_deprecation_warning
     def test_bulk_create_exception_gathered_on_dry_run(self, mock_bulk_create):
         mock_bulk_create.side_effect = ValidationError("invalid field")
 
         class _BookResource(resources.ModelResource):
             class Meta:
                 model = Book
                 use_bulk = True
                 batch_size = 100
 
         resource = _BookResource()
         result = resource.import_data(self.dataset, dry_run=True, raise_errors=False)
         self.assertTrue(result.has_errors())
 
-    @ignore_widget_deprecation_warning
     def test_m2m_not_called_for_bulk(self):
         mock_m2m_widget = mock.Mock(spec=widgets.ManyToManyWidget)
 
         class BookM2MResource(resources.ModelResource):
             categories = fields.Field(attribute="categories", widget=mock_m2m_widget)
 
             class Meta:
@@ -319,53 +303,49 @@
             import_id_fields = ("id",)
 
     def setUp(self):
         super().setUp()
         self.init_update_test_data()
         self.resource = self._BookResource()
 
-    @ignore_widget_deprecation_warning
     def test_bulk_update(self):
         result = self.resource.import_data(self.dataset)
         [self.assertEqual("UPDATED", b.name) for b in Book.objects.all()]
         self.assertEqual(10, result.total_rows)
         self.assertEqual(10, result.totals["update"])
 
     @mock.patch("core.models.Book.objects.bulk_update")
-    @ignore_widget_deprecation_warning
     def test_bulk_update_batch_size_of_4(self, mock_bulk_update):
         class _BookResource(resources.ModelResource):
             class Meta:
                 model = Book
                 use_bulk = True
                 batch_size = 4
 
         resource = _BookResource()
         result = resource.import_data(self.dataset)
         self.assertEqual(3, mock_bulk_update.call_count)
         self.assertEqual(10, result.total_rows)
         self.assertEqual(10, result.totals["update"])
 
     @mock.patch("core.models.Book.objects.bulk_update")
-    @ignore_widget_deprecation_warning
     def test_bulk_update_batch_size_of_5(self, mock_bulk_update):
         class _BookResource(resources.ModelResource):
             class Meta:
                 model = Book
                 use_bulk = True
                 batch_size = 5
 
         resource = _BookResource()
         result = resource.import_data(self.dataset)
         self.assertEqual(2, mock_bulk_update.call_count)
         self.assertEqual(10, result.total_rows)
         self.assertEqual(10, result.totals["update"])
 
     @mock.patch("core.models.Book.objects.bulk_update")
-    @ignore_widget_deprecation_warning
     def test_bulk_update_no_batch_size(self, mock_bulk_update):
         class _BookResource(resources.ModelResource):
             class Meta:
                 model = Book
                 use_bulk = True
                 batch_size = None
 
@@ -373,15 +353,14 @@
         result = resource.import_data(self.dataset)
         self.assertEqual(1, mock_bulk_update.call_count)
         mock_bulk_update.assert_called_with(mock.ANY, mock.ANY, batch_size=None)
         self.assertEqual(10, result.total_rows)
         self.assertEqual(10, result.totals["update"])
 
     @mock.patch("core.models.Book.objects.bulk_update")
-    @ignore_widget_deprecation_warning
     def test_bulk_update_not_called_when_not_using_transactions(self, mock_bulk_update):
         class _BookResource(resources.ModelResource):
             def import_data(
                 self,
                 dataset,
                 dry_run=False,
                 raise_errors=False,
@@ -405,36 +384,33 @@
                 use_bulk = True
 
         resource = _BookResource()
         resource.import_data(self.dataset, dry_run=True)
         mock_bulk_update.assert_not_called()
 
     @mock.patch("core.models.Book.objects.bulk_update")
-    @ignore_widget_deprecation_warning
     def test_bulk_update_called_for_dry_run(self, mock_bulk_update):
         self.resource.import_data(self.dataset, dry_run=True)
         self.assertEqual(1, mock_bulk_update.call_count)
 
     @mock.patch("core.models.Book.objects.bulk_update")
-    @ignore_widget_deprecation_warning
     def test_bulk_not_called_when_use_bulk_disabled(self, mock_bulk_update):
         class _BookResource(resources.ModelResource):
             class Meta:
                 model = Book
                 use_bulk = False
 
         resource = _BookResource()
         result = resource.import_data(self.dataset)
         self.assertEqual(10, Book.objects.count())
         self.assertEqual(10, result.total_rows)
         self.assertEqual(10, result.totals["update"])
         mock_bulk_update.assert_not_called()
 
     @mock.patch("core.models.Book.objects.bulk_update")
-    @ignore_widget_deprecation_warning
     def test_bulk_update_logs_exception(self, mock_bulk_update):
         e = ValidationError("invalid field")
         mock_bulk_update.side_effect = e
 
         class _BookResource(resources.ModelResource):
             class Meta:
                 model = Book
@@ -442,15 +418,14 @@
 
         resource = _BookResource()
         with mock.patch("logging.Logger.debug") as mock_exception:
             resource.import_data(self.dataset)
             mock_exception.assert_called_with(e, exc_info=e)
 
     @mock.patch("core.models.Book.objects.bulk_update")
-    @ignore_widget_deprecation_warning
     def test_bulk_update_raises_exception(self, mock_bulk_update):
         e = ValidationError("invalid field")
         mock_bulk_update.side_effect = e
 
         class _BookResource(resources.ModelResource):
             class Meta:
                 model = Book
@@ -464,15 +439,14 @@
 
 class BulkUUIDBookUpdateTest(BulkTest):
     def setUp(self):
         super().setUp()
         self.init_update_test_data(model=UUIDBook)
 
     @mock.patch("core.models.UUIDBook.objects.bulk_update")
-    @ignore_widget_deprecation_warning
     def test_bulk_update_uuid_model(self, mock_bulk_update):
         """Test update of a Model which defines uuid not pk (issue #1274)"""
 
         class _UUIDBookResource(resources.ModelResource):
             class Meta:
                 model = UUIDBook
                 use_bulk = True
@@ -505,49 +479,44 @@
         super().setUp()
         self.resource = self.DeleteBookResource()
         self.resource._meta.batch_size = 1000
         self.resource._meta.use_bulk = True
         self.init_update_test_data()
 
     @mock.patch("core.models.Book.delete")
-    @ignore_widget_deprecation_warning
     def test_bulk_delete_use_bulk_is_false(self, mock_obj_delete):
         self.resource._meta.use_bulk = False
         self.resource.import_data(self.dataset)
         self.assertEqual(10, mock_obj_delete.call_count)
 
     @mock.patch("core.models.Book.objects")
-    @ignore_widget_deprecation_warning
     def test_bulk_delete_batch_size_of_4(self, mock_obj_manager):
         self.resource._meta.batch_size = 4
         result = self.resource.import_data(self.dataset)
         self.assertEqual(3, mock_obj_manager.filter.return_value.delete.call_count)
         self.assertEqual(10, result.total_rows)
         self.assertEqual(10, result.totals["delete"])
 
     @mock.patch("core.models.Book.objects")
-    @ignore_widget_deprecation_warning
     def test_bulk_delete_batch_size_of_5(self, mock_obj_manager):
         self.resource._meta.batch_size = 5
         result = self.resource.import_data(self.dataset)
         self.assertEqual(2, mock_obj_manager.filter.return_value.delete.call_count)
         self.assertEqual(10, result.total_rows)
         self.assertEqual(10, result.totals["delete"])
 
     @mock.patch("core.models.Book.objects")
-    @ignore_widget_deprecation_warning
     def test_bulk_delete_batch_size_is_none(self, mock_obj_manager):
         self.resource._meta.batch_size = None
         result = self.resource.import_data(self.dataset)
         self.assertEqual(1, mock_obj_manager.filter.return_value.delete.call_count)
         self.assertEqual(10, result.total_rows)
         self.assertEqual(10, result.totals["delete"])
 
     @mock.patch("core.models.Book.objects")
-    @ignore_widget_deprecation_warning
     def test_bulk_delete_not_called_when_not_using_transactions(self, mock_obj_manager):
         class _BookResource(self.DeleteBookResource):
             def import_data(
                 self,
                 dataset,
                 dry_run=False,
                 raise_errors=False,
@@ -567,32 +536,29 @@
                 )
 
         resource = _BookResource()
         resource.import_data(self.dataset, dry_run=True)
         self.assertEqual(0, mock_obj_manager.filter.return_value.delete.call_count)
 
     @mock.patch("core.models.Book.objects")
-    @ignore_widget_deprecation_warning
     def test_bulk_delete_called_for_dry_run(self, mock_obj_manager):
         self.resource.import_data(self.dataset, dry_run=True)
         self.assertEqual(1, mock_obj_manager.filter.return_value.delete.call_count)
 
     @mock.patch("core.models.Book.objects")
-    @ignore_widget_deprecation_warning
     def test_bulk_delete_logs_exception(self, mock_obj_manager):
         e = Exception("invalid")
         mock_obj_manager.filter.return_value.delete.side_effect = e
 
         with mock.patch("logging.Logger.debug") as mock_exception:
             self.resource.import_data(self.dataset)
             mock_exception.assert_called_with(e, exc_info=mock.ANY)
             self.assertEqual(1, mock_exception.call_count)
 
     @mock.patch("core.models.Book.objects")
-    @ignore_widget_deprecation_warning
     def test_bulk_delete_raises_exception(self, mock_obj_manager):
         e = Exception("invalid")
         mock_obj_manager.filter.return_value.delete.side_effect = e
 
         with self.assertRaises(Exception) as raised_exc:
             self.resource.import_data(self.dataset, raise_errors=True)
             self.assertEqual(e, raised_exc)
@@ -609,12 +575,11 @@
             batch_size = 5
 
     def setUp(self):
         super().setUp()
         self.resource = self.DeleteBookResource()
         self.init_update_test_data(model=UUIDBook)
 
-    @ignore_widget_deprecation_warning
     def test_bulk_delete_batch_size_of_5(self):
         self.assertEqual(10, UUIDBook.objects.count())
         self.resource.import_data(self.dataset)
         self.assertEqual(0, UUIDBook.objects.count())
```

### Comparing `django_import_export-4.0.0rc3/tests/core/tests/test_resources/test_diffs.py` & `django_import_export-4.0.1/tests/core/tests/test_resources/test_diffs.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/tests/core/tests/test_resources/test_import_export.py` & `django_import_export-4.0.1/tests/core/tests/test_resources/test_import_export.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from datetime import date
 from unittest.mock import patch
 
 import tablib
 from core.models import Author, Book, Category
-from core.tests.resources import BookResource
-from core.tests.utils import ignore_widget_deprecation_warning
+from core.tests.resources import AuthorResource, BookResource
 from django.test import TestCase
 
 from import_export import exceptions, fields, resources, widgets
 
 
 class AfterImportComparisonTest(TestCase):
     class BookResource(resources.ModelResource):
@@ -29,15 +28,14 @@
         super().setUp()
         self.resource = AfterImportComparisonTest.BookResource()
         self.book = Book.objects.create(name="Some book")
         self.dataset = tablib.Dataset(headers=["id", "name", "published"])
         row = [self.book.pk, "Some book", "2023-05-09"]
         self.dataset.append(row)
 
-    @ignore_widget_deprecation_warning
     def test_after_import_row_check_for_change(self):
         # issue 1583 - assert that `original` object is available to after_import_row()
         self.resource.import_data(self.dataset, raise_errors=True)
         self.assertTrue(self.resource.is_published)
 
 
 class ImportExportFieldOrderTest(TestCase):
@@ -114,77 +112,67 @@
     def setUp(self):
         super().setUp()
         self.pk = Book.objects.create(name="Ulysses", price="1.99").pk
         self.dataset = tablib.Dataset(headers=["id", "name", "price"])
         row = [self.pk, "Some book", "19.99"]
         self.dataset.append(row)
 
-    @ignore_widget_deprecation_warning
     def test_defined_import_order(self):
         self.resource = ImportExportFieldOrderTest.OrderedBookResource()
         self.resource.import_data(self.dataset)
         self.assertEqual(["price", "name", "id"], self.resource.field_names)
 
-    @ignore_widget_deprecation_warning
     def test_undefined_import_order(self):
         self.resource = ImportExportFieldOrderTest.UnorderedBookResource()
         self.resource.import_data(self.dataset)
         self.assertEqual(["price", "id", "name"], self.resource.field_names)
 
-    @ignore_widget_deprecation_warning
     def test_defined_export_order(self):
         self.resource = ImportExportFieldOrderTest.OrderedBookResource()
         data = self.resource.export()
         target = f"price,name,id\r\n1.99,Ulysses,{self.pk}\r\n"
         self.assertEqual(target, data.csv)
 
-    @ignore_widget_deprecation_warning
     def test_undefined_export_order(self):
         # When export order is not defined,
         # exported order should correspond with 'fields' definition
         self.resource = ImportExportFieldOrderTest.UnorderedBookResource()
         data = self.resource.export()
         target = f"price,id,name\r\n1.99,{self.pk},Ulysses\r\n"
         self.assertEqual(target, data.csv)
 
-    @ignore_widget_deprecation_warning
     def test_subset_import_order(self):
         self.resource = ImportExportFieldOrderTest.SubsetOrderedBookResource()
         self.resource.import_data(self.dataset)
         self.assertEqual(
             ["name", "price", "id", "published"], self.resource.field_names
         )
 
-    @ignore_widget_deprecation_warning
     def test_subset_export_order(self):
         self.resource = ImportExportFieldOrderTest.SubsetOrderedBookResource()
         data = self.resource.export()
         target = f"published,price,id,name\r\n,1.99,{self.pk},Ulysses\r\n"
         self.assertEqual(target, data.csv)
 
-    @ignore_widget_deprecation_warning
     def test_duplicate_import_order(self):
         self.resource = ImportExportFieldOrderTest.DuplicateFieldsBookResource()
         self.resource.import_data(self.dataset)
         self.assertEqual(["id", "price", "name"], self.resource.field_names)
 
-    @ignore_widget_deprecation_warning
     def test_duplicate_export_order(self):
         self.resource = ImportExportFieldOrderTest.DuplicateFieldsBookResource()
         data = self.resource.export()
         target = f"id,price,name\r\n{self.pk},1.99,Ulysses\r\n"
         self.assertEqual(target, data.csv)
 
-    @ignore_widget_deprecation_warning
     def test_fields_as_list_import_order(self):
         self.resource = ImportExportFieldOrderTest.FieldsAsListBookResource()
         self.resource.import_data(self.dataset)
         self.assertEqual(["id", "price", "name"], self.resource.field_names)
 
-    @ignore_widget_deprecation_warning
     def test_fields_as_list_export_order(self):
         self.resource = ImportExportFieldOrderTest.FieldsAsListBookResource()
         data = self.resource.export()
         target = f"id,price,name\r\n{self.pk},1.99,Ulysses\r\n"
         self.assertEqual(target, data.csv)
 
     def test_declared_model_fields_not_alter_export_order(self):
@@ -342,15 +330,14 @@
 
 
 class ImportWithMissingFields(TestCase):
     # issue 1517
 
     @patch("import_export.resources.logger")
     @patch("import_export.fields.Field.save")
-    @ignore_widget_deprecation_warning
     def test_import_with_missing_instance_attribute(self, mock_field_save, mock_logger):
         class _BookResource(resources.ModelResource):
             name = fields.Field(column_name="name")
 
             class Meta:
                 model = Book
 
@@ -363,18 +350,25 @@
             "- field attribute is not defined"
         )
         mock_logger.debug.assert_any_call(target)
         self.assertEqual(1, mock_field_save.call_count)
 
     @patch("import_export.resources.logger")
     @patch("import_export.fields.Field.save")
-    @ignore_widget_deprecation_warning
     def test_import_with_missing_field_in_row(self, mock_field_save, mock_logger):
         dataset = tablib.Dataset(*[(1, "Some book")], headers=["id", "name"])
         self.resource = BookResource()
         result = self.resource.import_data(dataset)
         self.assertFalse(result.has_errors())
         mock_logger.debug.assert_any_call(
             "skipping field '<import_export.fields.Field: author_email>' "
             "- column name 'author_email' is not present in row"
         )
         self.assertEqual(2, mock_field_save.call_count)
+
+    def test_import_row_with_no_defined_id_field(self):
+        """Ensure a row with no id field can be imported (issue 1812)."""
+        self.assertEqual(0, Author.objects.count())
+        dataset = tablib.Dataset(*[("J. R. R. Tolkien",)], headers=["name"])
+        self.resource = AuthorResource()
+        self.resource.import_data(dataset)
+        self.assertEqual(1, Author.objects.count())
```

### Comparing `django_import_export-4.0.0rc3/tests/core/tests/test_resources/test_misc.py` & `django_import_export-4.0.1/tests/core/tests/test_resources/test_misc.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import tablib
 from core.models import Author, Book, Category
-from core.tests.utils import ignore_widget_deprecation_warning
 from django.test import TestCase
 
 from import_export import resources, results
 
 
 class RawValueTest(TestCase):
     def setUp(self):
@@ -16,15 +15,14 @@
         self.resource = _BookResource()
 
         self.book = Book.objects.create(name="Some book")
         self.dataset = tablib.Dataset(headers=["id", "name", "author_email", "price"])
         row = [self.book.pk, "Some book", "test@example.com", "10.25"]
         self.dataset.append(row)
 
-    @ignore_widget_deprecation_warning
     def test_import_data(self):
         result = self.resource.import_data(self.dataset, raise_errors=True)
 
         self.assertFalse(result.has_errors())
         self.assertEqual(len(result.rows), 1)
         self.assertTrue(result.rows[0].diff)
         self.assertEqual(
```

### Comparing `django_import_export-4.0.0rc3/tests/core/tests/test_resources/test_modelresource/test_data_deletion.py` & `django_import_export-4.0.1/tests/core/tests/test_resources/test_modelresource/test_data_deletion.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 from unittest import mock
 
 import tablib
 from core.models import Book
 from core.tests.resources import BookResource
-from core.tests.utils import ignore_widget_deprecation_warning
 from django.test import TestCase
 
 from import_export import fields, results, widgets
 
 
 class DataDeletionDryRunTest(TestCase):
     def setUp(self):
         self.resource = BookResource()
         self.book = Book.objects.create(name="Some book")
         self.dataset = tablib.Dataset(headers=["id", "name", "author_email", "price"])
         row = [self.book.pk, "Some book", "test@example.com", "10.25"]
         self.dataset.append(row)
 
-    @ignore_widget_deprecation_warning
     def test_import_data_delete(self):
         class B(BookResource):
             delete = fields.Field(widget=widgets.BooleanWidget())
 
             def for_delete(self, row, instance):
                 return self.fields["delete"].clean(row)
 
@@ -32,15 +30,14 @@
         self.assertEqual(
             result.rows[0].import_type, results.RowResult.IMPORT_TYPE_DELETE
         )
         self.assertFalse(Book.objects.filter(pk=self.book.pk))
         self.assertIsNone(result.rows[0].instance)
         self.assertIsNone(result.rows[0].original)
 
-    @ignore_widget_deprecation_warning
     def test_import_data_delete_store_instance(self):
         class B(BookResource):
             delete = fields.Field(widget=widgets.BooleanWidget())
 
             def for_delete(self, row, instance):
                 return self.fields["delete"].clean(row)
 
@@ -51,15 +48,14 @@
         dataset = tablib.Dataset(*[row], headers=["id", "name", "delete"])
         result = B().import_data(dataset, raise_errors=True)
         self.assertEqual(
             result.rows[0].import_type, results.RowResult.IMPORT_TYPE_DELETE
         )
         self.assertIsNotNone(result.rows[0].instance)
 
-    @ignore_widget_deprecation_warning
     def test_save_instance_with_dry_run_flag(self):
         class B(BookResource):
             def before_save_instance(self, instance, row, **kwargs):
                 super().before_save_instance(instance, row, **kwargs)
                 dry_run = kwargs.get("dry_run", False)
                 if dry_run:
                     self.before_save_instance_dry_run = True
@@ -105,15 +101,14 @@
     def test_delete_instance_noop(self, mock_book):
         book = Book.objects.first()
         self.resource.delete_instance(
             book, None, using_transactions=False, dry_run=True
         )
         self.assertEqual(0, mock_book.call_count)
 
-    @ignore_widget_deprecation_warning
     def test_delete_instance_with_dry_run_flag(self):
         class B(BookResource):
             delete = fields.Field(widget=widgets.BooleanWidget())
 
             def for_delete(self, row, instance):
                 return self.fields["delete"].clean(row)
```

### Comparing `django_import_export-4.0.0rc3/tests/core/tests/test_resources/test_modelresource/test_data_handling.py` & `django_import_export-4.0.1/tests/core/tests/test_resources/test_modelresource/test_data_handling.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 from decimal import InvalidOperation
 
 import tablib
 from core.models import Author, Book
 from core.tests.resources import AuthorResourceWithCustomWidget, BookResource
-from core.tests.utils import ignore_widget_deprecation_warning
 from django.test import TestCase
 
 from import_export import resources, results
 
 
 class DataHandlingTest(TestCase):
     def setUp(self):
         self.resource = BookResource()
         self.book = Book.objects.create(name="Some book")
         self.dataset = tablib.Dataset(headers=["id", "name", "author_email", "price"])
         row = [self.book.pk, "Some book", "test@example.com", "10.25"]
         self.dataset.append(row)
 
-    @ignore_widget_deprecation_warning
     def test_import_data_handles_widget_valueerrors_with_unicode_messages(self):
         resource = AuthorResourceWithCustomWidget()
         dataset = tablib.Dataset(headers=["id", "name", "birthday"])
         dataset.append(["", "A.A.Milne", "1882-01-18"])
 
         result = resource.import_data(dataset, raise_errors=False)
 
@@ -44,15 +42,14 @@
         dataset = tablib.Dataset(headers=["id", "name"])
         dataset.append(["", "123"])
 
         result = resource.import_data(dataset, raise_errors=False)
         self.assertFalse(result.has_validation_errors())
         self.assertEqual(len(result.invalid_rows), 0)
 
-    @ignore_widget_deprecation_warning
     def test_model_validation_errors_raised_when_clean_model_instances_is_true(self):
         class TestResource(resources.ModelResource):
             class Meta:
                 model = Author
                 clean_model_instances = True
                 export_order = ["id", "name", "birthday"]
 
@@ -74,15 +71,14 @@
         self.assertEqual(
             invalid_row.field_specific_errors, {"name": ["'123' is not a valid value"]}
         )
         # diff_header and invalid_row.values should match too
         self.assertEqual(result.diff_headers, ["id", "name", "birthday"])
         self.assertEqual(invalid_row.values, ("1", "123", "---"))
 
-    @ignore_widget_deprecation_warning
     def test_known_invalid_fields_are_excluded_from_model_instance_cleaning(self):
         # The custom widget on the parent class should complain about
         # 'name' first, preventing Author.full_clean() from raising the
         # error as it does in the previous test
 
         class TestResource(AuthorResourceWithCustomWidget):
             class Meta:
```

### Comparing `django_import_export-4.0.0rc3/tests/core/tests/test_resources/test_modelresource/test_data_import.py` & `django_import_export-4.0.1/tests/core/tests/test_resources/test_modelresource/test_data_import.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,43 +1,40 @@
 from decimal import Decimal
 from unittest import mock
 
 import tablib
 from core.models import Book
 from core.tests.resources import BookResource, BookResourceWithStoreInstance
-from core.tests.utils import ignore_widget_deprecation_warning
 from django.test import TestCase, skipUnlessDBFeature
 
 from import_export import results
 from import_export.resources import Diff
 
 
 class DataImportTests(TestCase):
     def setUp(self):
         self.resource = BookResource()
         self.book = Book.objects.create(name="Some book")
         self.dataset = tablib.Dataset(headers=["id", "name", "author_email", "price"])
         row = [self.book.pk, "Some book", "test@example.com", "10.25"]
         self.dataset.append(row)
 
-    @ignore_widget_deprecation_warning
     def test_get_diff(self):
         diff = Diff(self.resource, self.book, False)
         book2 = Book(name="Some other book")
         diff.compare_with(self.resource, book2)
         html = diff.as_html()
         headers = self.resource.get_export_headers()
         self.assertEqual(
             html[headers.index("name")],
             '<span>Some </span><ins style="background:#e6ffe6;">'
             "other </ins><span>book</span>",
         )
         self.assertFalse(html[headers.index("author_email")])
 
-    @ignore_widget_deprecation_warning
     def test_import_data_update(self):
         result = self.resource.import_data(self.dataset, raise_errors=True)
 
         self.assertFalse(result.has_errors())
         self.assertEqual(len(result.rows), 1)
         self.assertTrue(result.rows[0].diff)
         self.assertEqual(
@@ -49,15 +46,14 @@
         self.assertIsNone(result.rows[0].instance)
         self.assertIsNotNone(result.rows[0].original)
 
         instance = Book.objects.get(pk=self.book.pk)
         self.assertEqual(instance.author_email, "test@example.com")
         self.assertEqual(instance.price, Decimal("10.25"))
 
-    @ignore_widget_deprecation_warning
     def test_import_data_new(self):
         Book.objects.all().delete()
         self.assertEqual(0, Book.objects.count())
         result = self.resource.import_data(self.dataset, raise_errors=True)
 
         self.assertFalse(result.has_errors())
         self.assertEqual(len(result.rows), 1)
@@ -70,44 +66,41 @@
         self.assertIsNone(result.rows[0].original)
 
         self.assertEqual(1, Book.objects.count())
         instance = Book.objects.first()
         self.assertEqual(instance.author_email, "test@example.com")
         self.assertEqual(instance.price, Decimal("10.25"))
 
-    @ignore_widget_deprecation_warning
     def test_import_data_new_store_instance(self):
         self.resource = BookResourceWithStoreInstance()
         Book.objects.all().delete()
         self.assertEqual(0, Book.objects.count())
         result = self.resource.import_data(self.dataset, raise_errors=True)
 
         self.assertEqual(result.rows[0].import_type, results.RowResult.IMPORT_TYPE_NEW)
         self.assertIsNotNone(result.rows[0].instance)
         self.assertIsNone(result.rows[0].original)
         self.assertEqual(1, Book.objects.count())
         book = Book.objects.first()
         self.assertEqual(book.pk, result.rows[0].instance.pk)
 
-    @ignore_widget_deprecation_warning
     def test_import_data_update_store_instance(self):
         self.resource = BookResourceWithStoreInstance()
         result = self.resource.import_data(self.dataset, raise_errors=True)
         self.assertEqual(
             result.rows[0].import_type, results.RowResult.IMPORT_TYPE_UPDATE
         )
         self.assertIsNotNone(result.rows[0].instance)
         self.assertIsNotNone(result.rows[0].original)
         self.assertEqual(1, Book.objects.count())
         book = Book.objects.first()
         self.assertEqual(book.pk, result.rows[0].instance.pk)
 
     @skipUnlessDBFeature("supports_transactions")
     @mock.patch("import_export.resources.connections")
-    @ignore_widget_deprecation_warning
     def test_import_data_no_transaction(self, mock_db_connections):
         class Features:
             supports_transactions = False
 
         class DummyConnection:
             features = Features()
 
@@ -122,15 +115,14 @@
         self.assertTrue(result.rows[0].diff)
         self.assertEqual(
             result.rows[0].import_type, results.RowResult.IMPORT_TYPE_UPDATE
         )
         self.assertEqual(result.rows[0].row_values.get("name"), None)
         self.assertEqual(result.rows[0].row_values.get("author_email"), None)
 
-    @ignore_widget_deprecation_warning
     def test_import_data_new_override_do_instance_save(self):
         class CustomDoInstanceSave(BookResource):
             is_create = False
 
             def do_instance_save(self, instance, is_create):
                 self.is_create = is_create
                 super().do_instance_save(instance, is_create)
```

### Comparing `django_import_export-4.0.0rc3/tests/core/tests/test_resources/test_modelresource/test_deprecated_fields.py` & `django_import_export-4.0.1/tests/core/tests/test_resources/test_modelresource/test_deprecated_fields.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/tests/core/tests/test_resources/test_modelresource/test_dynamic_customization.py` & `django_import_export-4.0.1/tests/core/tests/test_resources/test_modelresource/test_dynamic_customization.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,14 @@
     Category,
     Entry,
     Profile,
     WithDynamicDefault,
     WithFloatField,
 )
 from core.tests.resources import BookResource, CategoryResource
-from core.tests.utils import ignore_widget_deprecation_warning
 from django.contrib.auth.models import User
 from django.core.exceptions import FieldDoesNotExist
 from django.db.models import Count
 from django.db.utils import ConnectionDoesNotExist
 from django.test import TestCase
 
 from import_export import exceptions, fields, resources, results
@@ -22,15 +21,14 @@
     def setUp(self):
         self.resource = BookResource()
         self.book = Book.objects.create(name="Some book")
         self.dataset = tablib.Dataset(headers=["id", "name", "author_email", "price"])
         row = [self.book.pk, "Some book", "test@example.com", "10.25"]
         self.dataset.append(row)
 
-    @ignore_widget_deprecation_warning
     def test_related_one_to_one(self):
         # issue #17 - Exception when attempting access something on the
         # related_name
 
         user = User.objects.create(username="foo")
         profile = Profile.objects.create(user=user)
         Entry.objects.create(user=user)
@@ -50,15 +48,14 @@
 
     def test_empty_get_queryset(self):
         # issue #25 - Overriding queryset on export() fails when passed
         # queryset has zero elements
         dataset = self.resource.export(queryset=Book.objects.none())
         self.assertEqual(len(dataset), 0)
 
-    @ignore_widget_deprecation_warning
     def test_import_data_skip_unchanged(self):
         class MyBookResource(resources.ModelResource):
             save_count = 0
 
             def save_instance(self, instance, is_create, row, **kwargs):
                 self.save_count += 1
 
@@ -87,15 +84,14 @@
 
         # Test that we can suppress reporting of skipped rows
         resource._meta.report_skipped = False
         result = resource.import_data(dataset, raise_errors=True)
         self.assertFalse(result.has_errors())
         self.assertEqual(len(result.rows), 0)
 
-    @ignore_widget_deprecation_warning
     def test_before_import_access_to_kwargs(self):
         class B(BookResource):
             def before_import(self, dataset, **kwargs):
                 if "extra_arg" in kwargs:
                     dataset.headers[dataset.headers.index("author_email")] = "old_email"
                     dataset.insert_col(
                         0, lambda row: kwargs["extra_arg"], header="author_email"
@@ -116,15 +112,14 @@
                 raise Exception("This is an invalid dataset")
 
         resource = B()
         with self.assertRaises(exceptions.ImportError) as cm:
             resource.import_data(self.dataset, raise_errors=True)
         self.assertEqual("This is an invalid dataset", cm.exception.error.args[0])
 
-    @ignore_widget_deprecation_warning
     def test_after_import_raises_error(self):
         class B(BookResource):
             def after_import(
                 self, dataset, result, using_transactions, dry_run, **kwargs
             ):
                 raise Exception("This is an invalid dataset")
 
@@ -187,15 +182,14 @@
             def field_from_django_field(self, field_name, django_field, readonly):
                 if field_name == "published":
                     return {"sound": "quack"}
 
         B()
         self.assertEqual({"sound": "quack"}, B.fields["published"])
 
-    @ignore_widget_deprecation_warning
     def test_readonly_annotated_field_import_and_export(self):
         class B(BookResource):
             total_categories = fields.Field("total_categories", readonly=True)
 
             class Meta:
                 model = Book
                 skip_unchanged = True
@@ -214,15 +208,14 @@
         # Verify that importing the annotated field raises no errors and that
         # the rows are skipped
         result = resource.import_data(dataset, raise_errors=True)
         self.assertFalse(result.has_errors())
         self.assertEqual(len(result.rows), len(dataset))
         self.assertEqual(result.rows[0].import_type, results.RowResult.IMPORT_TYPE_SKIP)
 
-    @ignore_widget_deprecation_warning
     def test_follow_relationship_for_modelresource(self):
         class EntryResource(resources.ModelResource):
             username = fields.Field(attribute="user__username", readonly=False)
 
             class Meta:
                 model = Entry
                 fields = ("id", "username")
@@ -246,15 +239,14 @@
         self.dataset.append(row)
         result = EntryResource().import_data(
             self.dataset, raise_errors=True, dry_run=False
         )
         self.assertFalse(result.has_errors())
         self.assertEqual(User.objects.get(pk=user.pk).username, "bar")
 
-    @ignore_widget_deprecation_warning
     def test_import_data_dynamic_default_callable(self):
         class DynamicDefaultResource(resources.ModelResource):
             class Meta:
                 model = WithDynamicDefault
                 fields = (
                     "id",
                     "name",
@@ -271,15 +263,14 @@
         )
         dataset.append([1, None])
         dataset.append([2, None])
         resource.import_data(dataset, raise_errors=False)
         objs = WithDynamicDefault.objects.all()
         self.assertNotEqual(objs[0].name, objs[1].name)
 
-    @ignore_widget_deprecation_warning
     def test_float_field(self):
         # 433
         class R(resources.ModelResource):
             class Meta:
                 model = WithFloatField
 
         resource = R()
```

### Comparing `django_import_export-4.0.0rc3/tests/core/tests/test_resources/test_modelresource/test_error_handling.py` & `django_import_export-4.0.1/tests/core/tests/test_resources/test_modelresource/test_error_handling.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,19 +4,18 @@
 from core.models import Author, Book
 from core.tests.resources import (
     AuthorResource,
     BookResource,
     BookResourceWithLineNumberLogger,
     ProfileResource,
 )
-from core.tests.utils import ignore_widget_deprecation_warning
 from django.core.exceptions import ImproperlyConfigured, ValidationError
 from django.test import TestCase
 
-from import_export import exceptions, results
+from import_export import exceptions, resources, results
 
 
 class ErrorHandlingTest(TestCase):
     def setUp(self):
         self.resource = BookResource()
         self.book = Book.objects.create(name="Some book")
         self.dataset = tablib.Dataset(headers=["id", "name", "author_email", "price"])
@@ -37,64 +36,63 @@
         mock_db_connections.__getitem__.return_value = dummy_connection
         with self.assertRaises(ImproperlyConfigured):
             self.resource.import_data(
                 self.dataset,
                 use_transactions=True,
             )
 
-    @ignore_widget_deprecation_warning
     def test_importing_with_line_number_logging(self):
         resource = BookResourceWithLineNumberLogger()
         resource.import_data(self.dataset, raise_errors=True)
         self.assertEqual(resource.before_lines, [1])
         self.assertEqual(resource.after_lines, [1])
 
-    @ignore_widget_deprecation_warning
     def test_import_data_raises_field_specific_validation_errors(self):
         resource = AuthorResource()
-        dataset = tablib.Dataset(headers=["id", "name", "birthday"])
-        dataset.append(["", "A.A.Milne", "1882test-01-18"])
+        dataset = tablib.Dataset(headers=["name", "birthday"])
+        dataset.append(["A.A.Milne", "1882test-01-18"])
 
         result = resource.import_data(dataset, raise_errors=False)
 
         self.assertTrue(result.has_validation_errors())
         self.assertIs(result.rows[0].import_type, results.RowResult.IMPORT_TYPE_INVALID)
         self.assertIn("birthday", result.invalid_rows[0].field_specific_errors)
 
-    @ignore_widget_deprecation_warning
     def test_import_data_raises_field_specific_validation_errors_with_skip_unchanged(
         self,
     ):
         resource = AuthorResource()
-        resource._meta.skip_unchanged = True
-
         author = Author.objects.create(name="Some author")
 
         dataset = tablib.Dataset(headers=["id", "birthday"])
         dataset.append([author.id, "1882test-01-18"])
 
         result = resource.import_data(dataset, raise_errors=False)
 
         self.assertTrue(result.has_validation_errors())
         self.assertIs(result.rows[0].import_type, results.RowResult.IMPORT_TYPE_INVALID)
         self.assertIn("birthday", result.invalid_rows[0].field_specific_errors)
 
     def test_import_data_empty_dataset_with_collect_failed_rows(self):
-        resource = AuthorResource()
+        class _AuthorResource(resources.ModelResource):
+            class Meta:
+                model = Author
+                import_id_fields = ["non_existent_field"]
+
+        resource = _AuthorResource()
         with self.assertRaises(exceptions.ImportError) as e:
             resource.import_data(
                 tablib.Dataset(), collect_failed_rows=True, raise_errors=True
             )
         self.assertEqual(
             "The following fields are declared in 'import_id_fields' "
-            "but are not present in the file headers: id",
+            "but are not present in the resource fields: non_existent_field",
             str(e.exception),
         )
 
-    @ignore_widget_deprecation_warning
     def test_collect_failed_rows(self):
         resource = ProfileResource()
         headers = ["id", "user"]
         # 'user' is a required field, the database will raise an error.
         row = [None, None]
         dataset = tablib.Dataset(row, headers=headers)
         result = resource.import_data(
@@ -103,15 +101,14 @@
             use_transactions=True,
             collect_failed_rows=True,
         )
         self.assertEqual(result.failed_dataset.headers, ["id", "user", "Error"])
         self.assertEqual(len(result.failed_dataset), 1)
         # We can't check the error message because it's package- and version-dependent
 
-    @ignore_widget_deprecation_warning
     def test_row_result_raise_errors(self):
         resource = ProfileResource()
         headers = ["id", "user"]
         # 'user' is a required field, the database will raise an error.
         row = [None, None]
         dataset = tablib.Dataset(row, headers=headers)
         with self.assertRaises(exceptions.ImportError) as exc:
@@ -121,15 +118,14 @@
                 use_transactions=True,
                 raise_errors=True,
             )
         row_error = exc.exception
         self.assertEqual(1, row_error.number)
         self.assertEqual({"id": None, "user": None}, row_error.row)
 
-    @ignore_widget_deprecation_warning
     def test_collect_failed_rows_validation_error(self):
         resource = ProfileResource()
         row = ["1"]
         dataset = tablib.Dataset(row, headers=["id"])
         with mock.patch(
             "import_export.resources.Field.save", side_effect=Exception("fail!")
         ):
@@ -143,15 +139,14 @@
         self.assertEqual(
             1,
             len(result.failed_dataset),
         )
         self.assertEqual("1", result.failed_dataset.dict[0]["id"])
         self.assertEqual("fail!", result.failed_dataset.dict[0]["Error"])
 
-    @ignore_widget_deprecation_warning
     def test_row_result_raise_ValidationError(self):
         resource = ProfileResource()
         row = ["1"]
         dataset = tablib.Dataset(row, headers=["id"])
         with mock.patch(
             "import_export.resources.Field.save", side_effect=ValidationError("fail!")
         ):
@@ -161,15 +156,14 @@
                 resource.import_data(
                     dataset,
                     dry_run=True,
                     use_transactions=True,
                     raise_errors=True,
                 )
 
-    @ignore_widget_deprecation_warning
     def test_row_result_raise_ValidationError_collect_failed_rows(self):
         # 1752
         resource = ProfileResource()
         row = ["1"]
         dataset = tablib.Dataset(row, headers=["id"])
         with mock.patch(
             "import_export.resources.Field.save", side_effect=ValidationError("fail!")
```

### Comparing `django_import_export-4.0.0rc3/tests/core/tests/test_resources/test_modelresource/test_export.py` & `django_import_export-4.0.1/tests/core/tests/test_resources/test_modelresource/test_export.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import tablib
 from core.models import Author, Book
-from core.tests.utils import ignore_widget_deprecation_warning
 from django.test import TestCase
 
 from tests.core.tests.resources import BookResource
 
 
 class ExportFunctionalityTest(TestCase):
     def setUp(self):
@@ -27,21 +26,19 @@
                 "published_time",
                 "price",
                 "added",
                 "categories",
             ],
         )
 
-    @ignore_widget_deprecation_warning
     def test_export(self):
         with self.assertNumQueries(2):
             dataset = self.resource.export(queryset=Book.objects.all())
             self.assertEqual(len(dataset), 1)
 
-    @ignore_widget_deprecation_warning
     def test_export_with_foreign_keys(self):
         """
         Test that export() containing foreign keys doesn't generate
         extra query for every row.
         Fixes #974
         """
         author = Author.objects.create()
@@ -51,29 +48,26 @@
         Book.objects.create(name="Third book", author=Author.objects.create())
 
         with self.assertNumQueries(3):
             dataset = self.resource.export(Book.objects.prefetch_related("categories"))
             self.assertEqual(dataset.dict[0]["author"], author.pk)
             self.assertEqual(len(dataset), 3)
 
-    @ignore_widget_deprecation_warning
     def test_export_iterable(self):
         with self.assertNumQueries(2):
             dataset = self.resource.export(queryset=list(Book.objects.all()))
             self.assertEqual(len(dataset), 1)
 
-    @ignore_widget_deprecation_warning
     def test_export_prefetch_related(self):
         with self.assertNumQueries(3):
             dataset = self.resource.export(
                 queryset=Book.objects.prefetch_related("categories").all()
             )
             self.assertEqual(len(dataset), 1)
 
-    @ignore_widget_deprecation_warning
     def test_export_handles_named_queryset_parameter(self):
         class _BookResource(BookResource):
             def before_export(self, queryset, **kwargs):
                 self.qs = queryset
                 self.kwargs_ = kwargs
 
         self.resource = _BookResource()
```

### Comparing `django_import_export-4.0.0rc3/tests/core/tests/test_resources/test_modelresource/test_fields.py` & `django_import_export-4.0.1/tests/core/tests/test_resources/test_modelresource/test_fields.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/tests/core/tests/test_resources/test_modelresource/test_m2m.py` & `django_import_export-4.0.1/tests/core/tests/test_resources/test_modelresource/test_m2m.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,66 +1,60 @@
 import tablib
 from core.models import Author, Book, Category
 from core.tests.resources import BookResource
-from core.tests.utils import ignore_widget_deprecation_warning
 from django.test import TestCase
 
 from import_export import fields, resources, widgets
 
 
 class ForeignKeyM2MTest(TestCase):
     def setUp(self):
         self.resource = BookResource()
         self.book = Book.objects.create(name="Some book")
         self.dataset = tablib.Dataset(headers=["id", "name", "author_email", "price"])
         row = [self.book.pk, "Some book", "test@example.com", "10.25"]
         self.dataset.append(row)
 
-    @ignore_widget_deprecation_warning
     def test_foreign_keys_export(self):
         author1 = Author.objects.create(name="Foo")
         self.book.author = author1
         self.book.save()
 
         dataset = self.resource.export(Book.objects.all())
         self.assertEqual(dataset.dict[0]["author"], author1.pk)
 
-    @ignore_widget_deprecation_warning
     def test_foreign_keys_import(self):
         author2 = Author.objects.create(name="Bar")
         headers = ["id", "name", "author"]
         row = [None, "FooBook", author2.pk]
         dataset = tablib.Dataset(row, headers=headers)
         self.resource.import_data(dataset, raise_errors=True)
 
         book = Book.objects.get(name="FooBook")
         self.assertEqual(book.author, author2)
 
-    @ignore_widget_deprecation_warning
     def test_m2m_export(self):
         cat1 = Category.objects.create(name="Cat 1")
         cat2 = Category.objects.create(name="Cat 2")
         self.book.categories.add(cat1)
         self.book.categories.add(cat2)
 
         dataset = self.resource.export(Book.objects.all())
         self.assertEqual(dataset.dict[0]["categories"], "%d,%d" % (cat1.pk, cat2.pk))
 
-    @ignore_widget_deprecation_warning
     def test_m2m_import(self):
         cat1 = Category.objects.create(name="Cat 1")
         headers = ["id", "name", "categories"]
         row = [None, "FooBook", str(cat1.pk)]
         dataset = tablib.Dataset(row, headers=headers)
         self.resource.import_data(dataset, raise_errors=True)
 
         book = Book.objects.get(name="FooBook")
         self.assertIn(cat1, book.categories.all())
 
-    @ignore_widget_deprecation_warning
     def test_m2m_options_import(self):
         cat1 = Category.objects.create(name="Cat 1")
         cat2 = Category.objects.create(name="Cat 2")
         headers = ["id", "name", "categories"]
         row = [None, "FooBook", "Cat 1|Cat 2"]
         dataset = tablib.Dataset(row, headers=headers)
 
@@ -75,40 +69,37 @@
 
         resource = BookM2MResource()
         resource.import_data(dataset, raise_errors=True)
         book = Book.objects.get(name="FooBook")
         self.assertIn(cat1, book.categories.all())
         self.assertIn(cat2, book.categories.all())
 
-    @ignore_widget_deprecation_warning
     def test_import_null_django_CharField_saved_as_empty_string(self):
         # issue 1485
         resource = BookResource()
         self.assertTrue(resource._meta.model.author_email.field.blank)
         self.assertFalse(resource._meta.model.author_email.field.null)
         headers = ["id", "author_email"]
         row = [1, None]
         dataset = tablib.Dataset(row, headers=headers)
         resource.import_data(dataset, raise_errors=True)
         book = Book.objects.get(id=1)
         self.assertEqual("", book.author_email)
 
-    @ignore_widget_deprecation_warning
     def test_import_empty_django_CharField_saved_as_empty_string(self):
         resource = BookResource()
         self.assertTrue(resource._meta.model.author_email.field.blank)
         self.assertFalse(resource._meta.model.author_email.field.null)
         headers = ["id", "author_email"]
         row = [1, ""]
         dataset = tablib.Dataset(row, headers=headers)
         resource.import_data(dataset, raise_errors=True)
         book = Book.objects.get(id=1)
         self.assertEqual("", book.author_email)
 
-    @ignore_widget_deprecation_warning
     def test_m2m_add(self):
         cat1 = Category.objects.create(name="Cat 1")
         cat2 = Category.objects.create(name="Cat 2")
         cat3 = Category.objects.create(name="Cat 3")
         cat4 = Category.objects.create(name="Cat 4")
         headers = ["id", "name", "categories"]
         row = [None, "FooBook", "Cat 1|Cat 2"]
```

### Comparing `django_import_export-4.0.0rc3/tests/core/tests/test_resources/test_modelresource/test_queryset.py` & `django_import_export-4.0.1/tests/core/tests/test_resources/test_modelresource/test_queryset.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/tests/core/tests/test_resources/test_modelresource/test_relationship.py` & `django_import_export-4.0.1/tests/core/tests/test_resources/test_modelresource/test_relationship.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 from datetime import date
 
 import tablib
 from core.models import Author, Book
 from core.tests.resources import BookResource
-from core.tests.utils import ignore_widget_deprecation_warning
 from django.test import TestCase
 
 from import_export import fields, resources
 
 
 class RelationshipFieldTest(TestCase):
     def setUp(self):
         self.resource = BookResource()
         self.book = Book.objects.create(name="Some book")
         self.dataset = tablib.Dataset(headers=["id", "name", "author_email", "price"])
         row = [self.book.pk, "Some book", "test@example.com", "10.25"]
         self.dataset.append(row)
 
-    @ignore_widget_deprecation_warning
     def test_relationships_fields(self):
         class B(resources.ModelResource):
             class Meta:
                 model = Book
                 fields = ("author__name",)
 
         author = Author.objects.create(name="Author")
@@ -79,15 +77,14 @@
                 # so should be ignored
                 fields = ("author_name", "full_title")
 
         resource = B()
         self.assertEqual(1, len(resource.fields))
         self.assertEqual("full_title", list(resource.fields.keys())[0])
 
-    @ignore_widget_deprecation_warning
     def test_widget_format_in_fk_field(self):
         class B(resources.ModelResource):
             class Meta:
                 model = Book
                 fields = ("author__birthday",)
                 widgets = {
                     "author__birthday": {"format": "%Y-%m-%d"},
@@ -95,15 +92,14 @@
 
         author = Author.objects.create(name="Author")
         self.book.author = author
         resource = B()
         result = resource.fields["author__birthday"].export(self.book)
         self.assertEqual(result, str(date.today()))
 
-    @ignore_widget_deprecation_warning
     def test_widget_kwargs_for_field(self):
         class B(resources.ModelResource):
             class Meta:
                 model = Book
                 fields = ("published",)
                 widgets = {
                     "published": {"format": "%d.%m.%Y"},
```

### Comparing `django_import_export-4.0.0rc3/tests/core/tests/test_resources/test_modelresource/test_resource.py` & `django_import_export-4.0.1/tests/core/tests/test_resources/test_modelresource/test_resource.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/tests/core/tests/test_resources/test_modelresource/test_resource_fields.py` & `django_import_export-4.0.1/tests/core/tests/test_resources/test_modelresource/test_resource_fields.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import tablib
 from core.models import Book
-from core.tests.utils import ignore_widget_deprecation_warning
 from django.test import TestCase
 
 from import_export import fields, resources
 
 
 class ModelResourceFieldDeclarations(TestCase):
     class MyBookResource(resources.ModelResource):
@@ -16,27 +15,25 @@
             model = Book
             fields = ("id", "price")
 
     def setUp(self):
         self.book = Book.objects.create(name="Moonraker", price=".99")
         self.resource = ModelResourceFieldDeclarations.MyBookResource()
 
-    @ignore_widget_deprecation_warning
     def test_declared_field_not_imported(self):
         self.assertEqual("", self.book.author_email)
         rows = [
             (self.book.id, "12.99", "jj@example.com"),
         ]
         dataset = tablib.Dataset(*rows, headers=["id", "price", "author_email"])
         self.resource.import_data(dataset, raise_errors=True)
         self.book.refresh_from_db()
         # email should not be updated
         self.assertEqual("", self.book.author_email)
 
-    @ignore_widget_deprecation_warning
     def test_declared_field_not_exported(self):
         self.assertEqual("", self.book.author_email)
         data = self.resource.export()
         self.assertFalse("author_email" in data.dict[0])
 
 
 class ModelResourceNoFieldDeclarations(TestCase):
@@ -49,27 +46,25 @@
         class Meta:
             model = Book
 
     def setUp(self):
         self.book = Book.objects.create(name="Moonraker", price=".99")
         self.resource = ModelResourceNoFieldDeclarations.MyBookResource()
 
-    @ignore_widget_deprecation_warning
     def test_declared_field_imported(self):
         self.assertEqual("", self.book.author_email)
         rows = [
             (self.book.id, "12.99", "jj@example.com"),
         ]
         dataset = tablib.Dataset(*rows, headers=["id", "price", "author_email"])
         self.resource.import_data(dataset, raise_errors=True)
         self.book.refresh_from_db()
         # email should be updated
         self.assertEqual("jj@example.com", self.book.author_email)
 
-    @ignore_widget_deprecation_warning
     def test_declared_field_not_exported(self):
         self.assertEqual("", self.book.author_email)
         data = self.resource.export()
         self.assertTrue("author_email" in data.dict[0])
 
 
 class ModelResourceExcludeDeclarations(TestCase):
@@ -83,27 +78,25 @@
             fields = ("id", "price")
             exclude = ("author_email",)
 
     def setUp(self):
         self.book = Book.objects.create(name="Moonraker", price=".99")
         self.resource = ModelResourceExcludeDeclarations.MyBookResource()
 
-    @ignore_widget_deprecation_warning
     def test_excluded_field_not_imported(self):
         self.assertEqual("", self.book.author_email)
         rows = [
             (self.book.id, "12.99", "jj@example.com"),
         ]
         dataset = tablib.Dataset(*rows, headers=["id", "price", "author_email"])
         self.resource.import_data(dataset, raise_errors=True)
         self.book.refresh_from_db()
         # email should not be updated
         self.assertEqual("", self.book.author_email)
 
-    @ignore_widget_deprecation_warning
     def test_declared_field_not_exported(self):
         self.assertEqual("", self.book.author_email)
         data = self.resource.export()
         self.assertFalse("author_email" in data.dict[0])
 
 
 class ModelResourceFieldsAndExcludeDeclarations(TestCase):
@@ -119,27 +112,25 @@
             fields = ("id", "price", "author_email")
             exclude = ("author_email",)
 
     def setUp(self):
         self.book = Book.objects.create(name="Moonraker", price=".99")
         self.resource = ModelResourceFieldsAndExcludeDeclarations.MyBookResource()
 
-    @ignore_widget_deprecation_warning
     def test_excluded_field_not_imported(self):
         self.assertEqual("", self.book.author_email)
         rows = [
             (self.book.id, "12.99", "jj@example.com"),
         ]
         dataset = tablib.Dataset(*rows, headers=["id", "price", "author_email"])
         self.resource.import_data(dataset, raise_errors=True)
         self.book.refresh_from_db()
         # email should be updated
         self.assertEqual("jj@example.com", self.book.author_email)
 
-    @ignore_widget_deprecation_warning
     def test_declared_field_not_exported(self):
         self.assertEqual("", self.book.author_email)
         data = self.resource.export()
         self.assertTrue("author_email" in data.dict[0])
 
 
 class ModelResourceDeclarationsNotInImportTest(TestCase):
@@ -157,24 +148,22 @@
                 "id",
                 "price",
             )
 
     def setUp(self):
         self.resource = ModelResourceDeclarationsNotInImportTest.MyBookResource()
 
-    @ignore_widget_deprecation_warning
     def test_excluded_field_not_imported(self):
         rows = [
             ("1", "12.99"),
         ]
         dataset = tablib.Dataset(*rows, headers=["id", "price"])
         result = self.resource.import_data(dataset, raise_errors=True)
         book = Book.objects.first()
         self.assertEqual("", book.author_email)
         self.assertEqual(1, result.totals["new"])
 
-    @ignore_widget_deprecation_warning
     def test_excluded_field_not_exported(self):
         self.book = Book.objects.create(name="Moonraker", price=".99")
         self.assertEqual("", self.book.author_email)
         data = self.resource.export()
         self.assertFalse("author_email" in data.dict[0])
```

### Comparing `django_import_export-4.0.0rc3/tests/core/tests/test_resources/test_modelresource/test_resource_postgres.py` & `django_import_export-4.0.1/tests/core/tests/test_resources/test_modelresource/test_resource_postgres.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import json
 import sys
 from unittest import skipUnless
 
 import tablib
 from core.models import Book
 from core.tests.resources import BookResource
-from core.tests.utils import ignore_widget_deprecation_warning
 from django.conf import settings
 from django.db import IntegrityError
 from django.db.models import CharField
 from django.test import TestCase, TransactionTestCase
 
 from import_export import fields, resources, widgets
 
@@ -47,15 +46,14 @@
 @skipUnless(
     "postgresql" in settings.DATABASES["default"]["ENGINE"], "Run only against Postgres"
 )
 class PostgresTests(TransactionTestCase):
     # Make sure to start the sequences back at 1
     reset_sequences = True
 
-    @ignore_widget_deprecation_warning
     def test_create_object_after_importing_dataset_with_id(self):
         dataset = tablib.Dataset(headers=["id", "name"])
         dataset.append([1, "Some book"])
         resource = BookResource()
         result = resource.import_data(dataset)
         self.assertFalse(result.has_errors())
         try:
@@ -99,15 +97,14 @@
             fields = (
                 "id",
                 "name",
                 "chapter_numbers",
             )
 
     class TestExportArrayField(TestCase):
-        @ignore_widget_deprecation_warning
         def test_exports_array_field(self):
             dataset_headers = ["id", "name", "chapters"]
             chapters = ["Introduction", "Middle Chapter", "Ending"]
             dataset_row = ["1", "Book With Chapters", ",".join(chapters)]
             dataset = tablib.Dataset(headers=dataset_headers)
             dataset.append(dataset_row)
             book_with_chapters_resource = resources.modelresource_factory(
@@ -124,15 +121,14 @@
             self.resource = BookWithChaptersResource()
             self.chapters = ["Introduction", "Middle Chapter", "Ending"]
             self.book = BookWithChapters.objects.create(name="foo")
             self.dataset = tablib.Dataset(headers=["id", "name", "chapters"])
             row = [self.book.id, "Some book", ",".join(self.chapters)]
             self.dataset.append(row)
 
-        @ignore_widget_deprecation_warning
         def test_import_of_data_with_array(self):
             self.assertListEqual(self.book.chapters, [])
             result = self.resource.import_data(self.dataset, raise_errors=True)
 
             self.assertFalse(result.has_errors())
             self.assertEqual(len(result.rows), 1)
 
@@ -146,15 +142,14 @@
             self.book = BookWithChapterNumbers.objects.create(
                 name="foo", chapter_numbers=[]
             )
             self.dataset = tablib.Dataset(
                 *[(1, "some book", "1,2,3")], headers=["id", "name", "chapter_numbers"]
             )
 
-        @ignore_widget_deprecation_warning
         def test_import_of_data_with_int_array(self):
             # issue #1495
             self.assertListEqual(self.book.chapter_numbers, [])
             result = self.resource.import_data(self.dataset, raise_errors=True)
 
             self.assertFalse(result.has_errors())
             self.assertEqual(len(result.rows), 1)
@@ -163,15 +158,14 @@
             self.assertEqual(self.book.chapter_numbers, self.chapter_numbers)
 
     class TestExportJsonField(TestCase):
         def setUp(self):
             self.json_data = {"some_key": "some_value"}
             self.book = BookWithChapters.objects.create(name="foo", data=self.json_data)
 
-        @ignore_widget_deprecation_warning
         def test_export_field_with_appropriate_format(self):
             resource = resources.modelresource_factory(model=BookWithChapters)()
             result = resource.export(BookWithChapters.objects.all())
             self.assertEqual(result[0][3], json.dumps(self.json_data))
 
     class TestImportJsonField(TestCase):
         def setUp(self):
@@ -179,15 +173,14 @@
             self.data = {"some_key": "some_value"}
             self.json_data = json.dumps(self.data)
             self.book = BookWithChapters.objects.create(name="foo")
             self.dataset = tablib.Dataset(headers=["id", "name", "data"])
             row = [self.book.id, "Some book", self.json_data]
             self.dataset.append(row)
 
-        @ignore_widget_deprecation_warning
         def test_sets_json_data_when_model_field_is_empty(self):
             self.assertIsNone(self.book.data)
             result = self.resource.import_data(self.dataset, raise_errors=True)
 
             self.assertFalse(result.has_errors())
             self.assertEqual(len(result.rows), 1)
```

### Comparing `django_import_export-4.0.0rc3/tests/core/tests/test_resources/test_modelresource/test_resource_setup.py` & `django_import_export-4.0.1/tests/core/tests/test_resources/test_modelresource/test_resource_setup.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/tests/core/tests/test_resources/test_modelresource/test_resource_transactions.py` & `django_import_export-4.0.1/tests/core/tests/test_resources/test_modelresource/test_resource_transactions.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,23 +2,21 @@
 from core.models import Author, Book, Category, Profile
 from core.tests.resources import (
     AuthorResource,
     BookResource,
     CategoryResource,
     ProfileResource,
 )
-from core.tests.utils import ignore_widget_deprecation_warning
 from django.test import TransactionTestCase, skipUnlessDBFeature
 from django.utils.encoding import force_str
 from django.utils.html import strip_tags
 
 
 class ModelResourceTransactionTest(TransactionTestCase):
     @skipUnlessDBFeature("supports_transactions")
-    @ignore_widget_deprecation_warning
     def test_m2m_import_with_transactions(self):
         resource = BookResource()
         cat1 = Category.objects.create(name="Cat 1")
         headers = ["id", "name", "categories"]
         row = [None, "FooBook", str(cat1.pk)]
         dataset = tablib.Dataset(row, headers=headers)
 
@@ -73,15 +71,14 @@
         dataset = tablib.Dataset(*rows, headers=headers)
         result = resource.import_data(
             dataset,
             use_transactions=True,
         )
         self.assertTrue(result.has_errors())
 
-    @ignore_widget_deprecation_warning
     def test_rollback_on_validation_errors_false(self):
         """Should create only one instance as the second one
         raises a ``ValidationError``"""
         resource = AuthorResource()
         headers = ["id", "name", "birthday"]
         rows = [
             ["", "A.A.Milne", ""],
@@ -96,15 +93,14 @@
 
         # Ensure the validation error raised by the database has been saved.
         self.assertTrue(result.has_validation_errors())
 
         # Ensure that valid row resulted in an instance created.
         self.assertEqual(Author.objects.count(), 1)
 
-    @ignore_widget_deprecation_warning
     def test_rollback_on_validation_errors_true(self):
         """
         Should not create any instances as the second one raises a ``ValidationError``
         and ``rollback_on_validation_errors`` flag is set
         """
         resource = AuthorResource()
         headers = ["id", "name", "birthday"]
```

### Comparing `django_import_export-4.0.0rc3/tests/core/tests/test_resources/test_relationships.py` & `django_import_export-4.0.1/tests/core/tests/test_resources/test_relationships.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 import tablib
 from core.models import Book, Category, Person, Role, UUIDBook, UUIDCategory
 from core.tests.resources import BookResource
-from core.tests.utils import ignore_widget_deprecation_warning
 from django.contrib.auth.models import User
 from django.test import TestCase
 
 from import_export import fields, resources, results, widgets
 
 
 class ForeignKeyWidgetFollowRelationship(TestCase):
     def setUp(self):
         self.user = User.objects.create(username="foo")
         self.role = Role.objects.create(user=self.user)
         self.person = Person.objects.create(role=self.role)
 
-    @ignore_widget_deprecation_warning
     def test_export(self):
         class MyPersonResource(resources.ModelResource):
             role = fields.Field(
                 column_name="role",
                 attribute="role",
                 widget=widgets.ForeignKeyWidget(Role, field="user__username"),
             )
@@ -45,15 +43,14 @@
 
 class ManyRelatedManagerDiffTest(TestCase):
     fixtures = ["category", "book", "author"]
 
     def setUp(self):
         pass
 
-    @ignore_widget_deprecation_warning
     def test_related_manager_diff(self):
         dataset_headers = ["id", "name", "categories"]
         dataset_row = ["1", "Test Book", "1"]
         original_dataset = tablib.Dataset(headers=dataset_headers)
         original_dataset.append(dataset_row)
         dataset_row[2] = "2"
         changed_dataset = tablib.Dataset(headers=dataset_headers)
@@ -82,15 +79,14 @@
     # issue #1270 - ensure ManyToMany fields are correctly checked for
     # changes when skip_unchanged=True
     fixtures = ["category", "book", "author"]
 
     def setUp(self):
         pass
 
-    @ignore_widget_deprecation_warning
     def test_many_to_many_widget_create(self):
         # the book is associated with 0 categories
         # when we import a book with category 1, the book
         # should be updated, not skipped
         book = Book.objects.first()
         book.categories.clear()
         dataset_headers = ["id", "name", "categories"]
@@ -107,15 +103,14 @@
         book.refresh_from_db()
         self.assertEqual(1, book.categories.count())
         self.assertEqual(
             result.rows[0].import_type, results.RowResult.IMPORT_TYPE_UPDATE
         )
         self.assertEqual(Category.objects.first(), book.categories.first())
 
-    @ignore_widget_deprecation_warning
     def test_many_to_many_widget_create_with_m2m_being_compared(self):
         # issue 1558 - when the object is a new instance and m2m is
         # evaluated for differences
         dataset_headers = ["id", "categories"]
         dataset_row = ["1", "1"]
         dataset = tablib.Dataset(headers=dataset_headers)
         dataset.append(dataset_row)
@@ -124,15 +119,14 @@
 
         result = book_resource.import_data(dataset, dry_run=False)
 
         self.assertFalse(result.has_errors())
         self.assertEqual(len(result.rows), 1)
         self.assertEqual(result.rows[0].import_type, results.RowResult.IMPORT_TYPE_NEW)
 
-    @ignore_widget_deprecation_warning
     def test_many_to_many_widget_update(self):
         # the book is associated with 1 category ('Category 2')
         # when we import a book with category 1, the book
         # should be updated, not skipped, so that Category 2 is replaced by Category 1
         book = Book.objects.first()
         dataset_headers = ["id", "name", "categories"]
         dataset_row = [book.id, book.name, "1"]
@@ -146,15 +140,14 @@
         result = book_resource.import_data(dataset, dry_run=False)
         self.assertEqual(
             result.rows[0].import_type, results.RowResult.IMPORT_TYPE_UPDATE
         )
         self.assertEqual(1, book.categories.count())
         self.assertEqual(Category.objects.first(), book.categories.first())
 
-    @ignore_widget_deprecation_warning
     def test_many_to_many_widget_no_changes(self):
         # the book is associated with 1 category ('Category 2')
         # when we import a row with a book with category 1, the book
         # should be skipped, because there is no change
         book = Book.objects.first()
         dataset_headers = ["id", "name", "categories"]
         dataset_row = [book.id, book.name, book.categories.first().id]
@@ -165,15 +158,14 @@
         book_resource._meta.skip_unchanged = True
 
         self.assertEqual(1, book.categories.count())
         result = book_resource.import_data(dataset, dry_run=False)
         self.assertEqual(result.rows[0].import_type, results.RowResult.IMPORT_TYPE_SKIP)
         self.assertEqual(1, book.categories.count())
 
-    @ignore_widget_deprecation_warning
     def test_many_to_many_widget_handles_ordering(self):
         # the book is associated with 2 categories ('Category 1', 'Category 2')
         # when we import a row with a book with both categories (in any order), the book
         # should be skipped, because there is no change
         book = Book.objects.first()
         self.assertEqual(1, book.categories.count())
         cat1 = Category.objects.get(name="Category 1")
@@ -200,15 +192,14 @@
         dataset.append(dataset_row)
 
         result = book_resource.import_data(dataset, dry_run=False)
         self.assertEqual(result.rows[0].import_type, results.RowResult.IMPORT_TYPE_SKIP)
 
         self.assertEqual(2, book.categories.count())
 
-    @ignore_widget_deprecation_warning
     def test_many_to_many_widget_handles_uuid(self):
         # Test for #1435 - skip_row() handles M2M field when UUID pk used
         class _UUIDBookResource(resources.ModelResource):
             class Meta:
                 model = UUIDBook
 
         uuid_resource = _UUIDBookResource()
@@ -222,15 +213,14 @@
         dataset_headers = ["id", "name", "categories"]
         dataset_row = [uuid_book.id, uuid_book.name, f"{cat1.catid},{cat2.catid}"]
         dataset = tablib.Dataset(headers=dataset_headers)
         dataset.append(dataset_row)
         result = uuid_resource.import_data(dataset, dry_run=False)
         self.assertEqual(result.rows[0].import_type, results.RowResult.IMPORT_TYPE_SKIP)
 
-    @ignore_widget_deprecation_warning
     def test_skip_row_no_m2m_data_supplied(self):
         # issue #1437
         # test skip_row() when the model defines a m2m field
         # but it is not present in the dataset
         book = Book.objects.first()
         dataset_headers = ["id", "name"]
         dataset_row = [book.id, book.name]
```

### Comparing `django_import_export-4.0.0rc3/tests/core/tests/test_results.py` & `django_import_export-4.0.1/tests/core/tests/test_results.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/tests/core/tests/test_tmp_storages.py` & `django_import_export-4.0.1/tests/core/tests/test_tmp_storages.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/tests/core/tests/test_widgets.py` & `django_import_export-4.0.1/tests/core/tests/test_widgets.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import json
 from datetime import date, datetime, time, timedelta
 from decimal import Decimal
-from unittest import mock, skipUnless
+from unittest import mock
 from unittest.mock import patch
 
 import django
 from core.models import Author, Book, Category
 from core.tests.utils import ignore_utcnow_deprecation_warning
 from django.test import TestCase
 from django.test.utils import override_settings
@@ -98,25 +98,14 @@
 
 
 class FormatDatetimeTest(TestCase):
     date = date(10, 8, 2)
     target_dt = "02.08.0010"
     format = "%d.%m.%Y"
 
-    @skipUnless(
-        django.VERSION[0] < 4, f"skipping django {django.VERSION} version specific test"
-    )
-    def test_format_datetime_lt_django4(self):
-        self.assertEqual(
-            self.target_dt, widgets.format_datetime(self.date, self.format)
-        )
-
-    @skipUnless(
-        django.VERSION[0] >= 4, f"running django {django.VERSION} version specific test"
-    )
     def test_format_datetime_gte_django4(self):
         self.assertEqual(
             self.target_dt, widgets.format_datetime(self.date, self.format)
         )
 
 
 class DateWidgetTest(TestCase, RowDeprecationTestMixin):
@@ -379,25 +368,14 @@
 
     def test_render_None_coerce_to_string_False(self):
         self.assertEqual("", self.widget.render(None))
 
     def test_render_invalid_type(self):
         self.assertEqual(self.widget.render("a"), "")
 
-    @skipUnless(
-        django.VERSION[0] < 4, f"skipping django {django.VERSION} version specific test"
-    )
-    @override_settings(LANGUAGE_CODE="fr-fr", USE_L10N=True)
-    def test_locale_render_coerce_to_string_lt4(self):
-        self.assertEqual("11,111", self.widget_coerce_to_string.render(self.value))
-
-    @skipUnless(
-        django.VERSION[0] >= 4,
-        f"skipping django {django.VERSION} version specific test",
-    )
     @override_settings(LANGUAGE_CODE="fr-fr")
     def test_locale_render_coerce_to_string_gte4(self):
         self.assertEqual("11,111", self.widget_coerce_to_string.render(self.value))
 
     def test_coerce_to_string_value_is_None(self):
         self.assertEqual("", self.widget_coerce_to_string.render(None))
 
@@ -422,25 +400,14 @@
         self.assertEqual(self.widget.clean("0.0"), 0.0)
 
     def test_clean_empty_string(self):
         self.assertEqual(self.widget.clean(""), None)
         self.assertEqual(self.widget.clean(" "), None)
         self.assertEqual(self.widget.clean("\r\n\t"), None)
 
-    @skipUnless(
-        django.VERSION[0] < 4, f"skipping django {django.VERSION} version specific test"
-    )
-    @override_settings(LANGUAGE_CODE="fr-fr", USE_L10N=True)
-    def test_locale_render_coerce_to_string_lt4(self):
-        self.assertEqual(self.widget_coerce_to_string.render(self.value), "11,111")
-
-    @skipUnless(
-        django.VERSION[0] >= 4,
-        f"skipping django {django.VERSION} version specific test",
-    )
     @override_settings(LANGUAGE_CODE="fr-fr")
     def test_locale_render_coerce_to_string_gte4(self):
         self.assertEqual(self.widget_coerce_to_string.render(self.value), "11,111")
 
 
 class DecimalWidgetTest(TestCase, RowDeprecationTestMixin):
     def setUp(self):
@@ -466,25 +433,14 @@
         self.assertEqual(self.widget.clean("0.0"), Decimal("0"))
 
     def test_clean_empty_string(self):
         self.assertEqual(self.widget.clean(""), None)
         self.assertEqual(self.widget.clean(" "), None)
         self.assertEqual(self.widget.clean("\r\n\t"), None)
 
-    @skipUnless(
-        django.VERSION[0] < 4, f"skipping django {django.VERSION} version specific test"
-    )
-    @override_settings(LANGUAGE_CODE="fr-fr", USE_L10N=True)
-    def test_locale_render_coerce_to_string_lt4(self):
-        self.assertEqual(self.widget.render(self.value), "11,111")
-
-    @skipUnless(
-        django.VERSION[0] >= 4,
-        f"skipping django {django.VERSION} version specific test",
-    )
     @override_settings(LANGUAGE_CODE="fr-fr")
     def test_locale_render_coerce_to_string_gte4(self):
         self.assertEqual(self.widget.render(self.value), "11,111")
 
 
 class IntegerWidgetTest(TestCase, RowDeprecationTestMixin):
     def setUp(self):
@@ -507,25 +463,14 @@
         self.assertEqual(self.widget.clean(""), None)
         self.assertEqual(self.widget.clean(" "), None)
         self.assertEqual(self.widget.clean("\n\t\r"), None)
 
     def test_render_invalid_type(self):
         self.assertEqual(self.widget.render("a"), "")
 
-    @skipUnless(
-        django.VERSION[0] < 4, f"skipping django {django.VERSION} version specific test"
-    )
-    @override_settings(LANGUAGE_CODE="fr-fr", USE_L10N=True)
-    def test_locale_render_lt_django4(self):
-        self.assertEqual(self.widget_coerce_to_string.render(self.value), "0")
-
-    @skipUnless(
-        django.VERSION[0] >= 4,
-        f"skipping django {django.VERSION} version specific test",
-    )
     @override_settings(LANGUAGE_CODE="fr-fr")
     def test_locale_render_gte_django4(self):
         self.assertEqual(self.widget_coerce_to_string.render(self.value), "0")
 
 
 class ForeignKeyWidgetTest(TestCase, RowDeprecationTestMixin):
     def setUp(self):
```

### Comparing `django_import_export-4.0.0rc3/tests/docker-compose.yml` & `django_import_export-4.0.1/tests/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/tests/scripts/bulk_import.py` & `django_import_export-4.0.1/tests/scripts/bulk_import.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/tests/settings.py` & `django_import_export-4.0.1/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.0rc3/tox.ini` & `django_import_export-4.0.1/tox.ini`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tox]
 min_version = 4.0
 envlist =
-       {py38,py39,py310}-{django32}
+       {py38,py39}-{django42}
        {py310,py311,py312}-{django42,django50,djangomain}
        # tablib dev temporarily removed - see issue #1602
        # py311-djangomain-tablibdev
 
 [gh-actions]
 python =
     3.8: py38
@@ -15,16 +15,15 @@
     3.12: py312
 
 [testenv]
 setenv = PYTHONPATH = {toxinidir}/tests
 commands = python ./runtests.py
 deps =
     tablibdev: -egit+https://github.com/jazzband/tablib.git@master\#egg=tablib
-    django32: Django>=3.2,<4.0
-    django42: Django>=4.2,<4.3
+    django42: Django>=4.2,<5.0
     django50: Django>=5.0,<6.0
     djangomain: https://github.com/django/django/archive/main.tar.gz
     -rrequirements/test.txt
 
 # if postgres / mysql environment variables exist, we can go ahead and run db specific tests
 passenv =
     COVERAGE
```

