# Comparing `tmp/coop-5.2.3.tar.gz` & `tmp/coop-6.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coop-5.2.3.tar", last modified: Wed May  8 00:32:13 2024, max compression
+gzip compressed data, was "coop-6.0.0.tar", last modified: Fri Mar  8 04:25:53 2024, max compression
```

## Comparing `coop-5.2.3.tar` & `coop-6.0.0.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 00:32:13.089838 coop-5.2.3/
--rw-rw-rw-   0 root         (0) root         (0)      184 2024-05-08 00:32:01.000000 coop-5.2.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2902 2024-05-08 00:32:13.088838 coop-5.2.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1337 2024-05-08 00:32:01.000000 coop-5.2.3/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 00:32:13.071838 coop-5.2.3/coop/
--rw-rw-rw-   0 root         (0) root         (0)      123 2024-05-08 00:32:01.000000 coop-5.2.3/coop/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       68 2024-05-08 00:32:01.000000 coop-5.2.3/coop/_version.py
--rw-rw-rw-   0 root         (0) root         (0)     1893 2024-05-08 00:32:01.000000 coop-5.2.3/coop/blocks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 00:32:13.073838 coop-5.2.3/coop/factories/
--rw-rw-rw-   0 root         (0) root         (0)      470 2024-05-08 00:32:02.000000 coop-5.2.3/coop/factories/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      226 2024-05-08 00:32:02.000000 coop-5.2.3/coop/factories/attributes.py
--rw-rw-rw-   0 root         (0) root         (0)     2284 2024-05-08 00:32:02.000000 coop-5.2.3/coop/factories/blocks.py
--rw-rw-rw-   0 root         (0) root         (0)     1413 2024-05-08 00:32:02.000000 coop-5.2.3/coop/factories/fuzzy.py
--rw-rw-rw-   0 root         (0) root         (0)      164 2024-05-08 00:32:02.000000 coop-5.2.3/coop/factories/inline.py
--rw-rw-rw-   0 root         (0) root         (0)       71 2024-05-08 00:32:02.000000 coop-5.2.3/coop/factories/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 00:32:13.074838 coop-5.2.3/coop/form_builder/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-08 00:32:02.000000 coop-5.2.3/coop/form_builder/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5193 2024-05-08 00:32:01.000000 coop-5.2.3/coop/form_builder/blocks.py
--rw-rw-rw-   0 root         (0) root         (0)     2618 2024-05-08 00:32:01.000000 coop-5.2.3/coop/form_builder/factories.py
--rw-rw-rw-   0 root         (0) root         (0)      254 2024-05-08 00:32:01.000000 coop-5.2.3/coop/form_builder/forms.py
--rw-rw-rw-   0 root         (0) root         (0)     1168 2024-05-08 00:32:01.000000 coop-5.2.3/coop/form_builder/page.py
--rw-rw-rw-   0 root         (0) root         (0)     2468 2024-05-08 00:32:01.000000 coop-5.2.3/coop/form_builder/views.py
--rw-rw-rw-   0 root         (0) root         (0)      238 2024-05-08 00:32:01.000000 coop-5.2.3/coop/forms.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 00:32:13.066838 coop-5.2.3/coop/jinja2/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 00:32:13.074838 coop-5.2.3/coop/jinja2/coop/
--rw-rw-rw-   0 root         (0) root         (0)      567 2024-05-08 00:32:01.000000 coop-5.2.3/coop/jinja2/coop/analytics_warning.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 00:32:13.075838 coop-5.2.3/coop/jinja2tags/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-08 00:32:02.000000 coop-5.2.3/coop/jinja2tags/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6456 2024-05-08 00:32:01.000000 coop-5.2.3/coop/jinja2tags/core.py
--rw-rw-rw-   0 root         (0) root         (0)      385 2024-05-08 00:32:01.000000 coop-5.2.3/coop/jinja2tags/vite.py
--rw-rw-rw-   0 root         (0) root         (0)      438 2024-05-08 00:32:01.000000 coop-5.2.3/coop/jinja2tags/webpack.py
--rw-rw-rw-   0 root         (0) root         (0)      527 2024-05-08 00:32:01.000000 coop-5.2.3/coop/logging.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 00:32:13.075838 coop-5.2.3/coop/management/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-08 00:32:02.000000 coop-5.2.3/coop/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 00:32:13.076838 coop-5.2.3/coop/management/commands/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-08 00:32:02.000000 coop-5.2.3/coop/management/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1761 2024-05-08 00:32:01.000000 coop-5.2.3/coop/management/commands/phone_home.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 00:32:13.076838 coop-5.2.3/coop/migrations/
--rw-rw-rw-   0 root         (0) root         (0)      863 2024-05-08 00:32:01.000000 coop-5.2.3/coop/migrations/0001_remove_site.py
--rw-rw-rw-   0 root         (0) root         (0)      949 2024-05-08 00:32:01.000000 coop-5.2.3/coop/migrations/0002_analyticssettings.py
--rw-rw-rw-   0 root         (0) root         (0)      767 2024-05-08 00:32:01.000000 coop-5.2.3/coop/migrations/0003_tag_manager_settings.py
--rw-rw-rw-   0 root         (0) root         (0)      822 2024-05-08 00:32:01.000000 coop-5.2.3/coop/migrations/0004_increase_analytics_length.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-08 00:32:02.000000 coop-5.2.3/coop/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      508 2024-05-08 00:32:01.000000 coop-5.2.3/coop/models.py
--rw-rw-rw-   0 root         (0) root         (0)     3282 2024-05-08 00:32:01.000000 coop-5.2.3/coop/page.py
--rw-rw-rw-   0 root         (0) root         (0)     5858 2024-05-08 00:32:01.000000 coop-5.2.3/coop/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 00:32:13.077838 coop-5.2.3/coop/styleguide/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-08 00:32:02.000000 coop-5.2.3/coop/styleguide/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      206 2024-05-08 00:32:01.000000 coop-5.2.3/coop/styleguide/urls.py
--rw-rw-rw-   0 root         (0) root         (0)      188 2024-05-08 00:32:01.000000 coop-5.2.3/coop/styleguide/views.py
--rw-rw-rw-   0 root         (0) root         (0)     4689 2024-05-08 00:32:01.000000 coop-5.2.3/coop/test.py
--rw-rw-rw-   0 root         (0) root         (0)     2087 2024-05-08 00:32:01.000000 coop-5.2.3/coop/urls.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 00:32:13.077838 coop-5.2.3/coop/users/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-08 00:32:02.000000 coop-5.2.3/coop/users/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1971 2024-05-08 00:32:01.000000 coop-5.2.3/coop/users/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 00:32:13.079838 coop-5.2.3/coop/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-08 00:32:02.000000 coop-5.2.3/coop/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1591 2024-05-08 00:32:01.000000 coop-5.2.3/coop/utils/forms.py
--rw-rw-rw-   0 root         (0) root         (0)      931 2024-05-08 00:32:01.000000 coop-5.2.3/coop/utils/mailchimp.py
--rw-rw-rw-   0 root         (0) root         (0)      628 2024-05-08 00:32:01.000000 coop-5.2.3/coop/utils/migrations.py
--rw-rw-rw-   0 root         (0) root         (0)      578 2024-05-08 00:32:01.000000 coop-5.2.3/coop/utils/pagination.py
--rw-rw-rw-   0 root         (0) root         (0)      699 2024-05-08 00:32:01.000000 coop-5.2.3/coop/utils/rich_text_example.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 00:32:13.080838 coop-5.2.3/coop/utils/test_documents/
--rw-rw-rw-   0 root         (0) root         (0)   504692 2024-05-08 00:32:01.000000 coop-5.2.3/coop/utils/test_documents/magazine-article.pdf
--rw-rw-rw-   0 root         (0) root         (0)   515133 2024-05-08 00:32:01.000000 coop-5.2.3/coop/utils/test_documents/nj-logos.pdf
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 00:32:13.086838 coop-5.2.3/coop/utils/test_images/
--rw-rw-rw-   0 root         (0) root         (0)  3653229 2024-05-08 00:32:01.000000 coop-5.2.3/coop/utils/test_images/landscape-large.jpg
--rw-rw-rw-   0 root         (0) root         (0)    11487 2024-05-08 00:32:01.000000 coop-5.2.3/coop/utils/test_images/landscape-small.jpeg
--rw-rw-rw-   0 root         (0) root         (0)  2821960 2024-05-08 00:32:02.000000 coop-5.2.3/coop/utils/test_images/portrait-large.jpg
--rw-rw-rw-   0 root         (0) root         (0)     6608 2024-05-08 00:32:02.000000 coop-5.2.3/coop/utils/test_images/portrait-small.jpeg
--rw-rw-rw-   0 root         (0) root         (0)     8126 2024-05-08 00:32:02.000000 coop-5.2.3/coop/utils/testdata.py
--rw-rw-rw-   0 root         (0) root         (0)     2025 2024-05-08 00:32:02.000000 coop-5.2.3/coop/utils/views.py
--rw-rw-rw-   0 root         (0) root         (0)     1526 2024-05-08 00:32:02.000000 coop-5.2.3/coop/wagtail_hooks.py
--rw-rw-rw-   0 root         (0) root         (0)      129 2024-05-08 00:32:02.000000 coop-5.2.3/coop/wsgi.py
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-08 00:32:02.000000 coop-5.2.3/coop/wsgi_dev.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 00:32:13.087838 coop-5.2.3/coop.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2902 2024-05-08 00:32:13.000000 coop-5.2.3/coop.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1846 2024-05-08 00:32:13.000000 coop-5.2.3/coop.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-08 00:32:13.000000 coop-5.2.3/coop.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-08 00:32:13.000000 coop-5.2.3/coop.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      383 2024-05-08 00:32:13.000000 coop-5.2.3/coop.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2024-05-08 00:32:13.000000 coop-5.2.3/coop.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      237 2024-05-08 00:32:13.089838 coop-5.2.3/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1913 2024-05-08 00:32:02.000000 coop-5.2.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 00:32:13.087838 coop-5.2.3/tests/
--rw-rw-rw-   0 root         (0) root         (0)     1653 2024-05-08 00:32:02.000000 coop-5.2.3/tests/test_analytics_panel.py
--rw-rw-rw-   0 root         (0) root         (0)     2813 2024-05-08 00:32:02.000000 coop-5.2.3/tests/test_jinja2tags.py
--rw-rw-rw-   0 root         (0) root         (0)     1252 2024-05-08 00:32:02.000000 coop-5.2.3/tests/test_page.py
--rw-rw-rw-   0 root         (0) root         (0)      698 2024-05-08 00:32:02.000000 coop-5.2.3/tests/test_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 04:25:53.176389 coop-6.0.0/
+-rw-rw-rw-   0 root         (0) root         (0)      184 2024-03-08 04:25:44.000000 coop-6.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2903 2024-03-08 04:25:53.176389 coop-6.0.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1337 2024-03-08 04:25:44.000000 coop-6.0.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 04:25:53.159389 coop-6.0.0/coop/
+-rw-rw-rw-   0 root         (0) root         (0)      123 2024-03-08 04:25:44.000000 coop-6.0.0/coop/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       68 2024-03-08 04:25:44.000000 coop-6.0.0/coop/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     1893 2024-03-08 04:25:44.000000 coop-6.0.0/coop/blocks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 04:25:53.161389 coop-6.0.0/coop/factories/
+-rw-rw-rw-   0 root         (0) root         (0)      470 2024-03-08 04:25:45.000000 coop-6.0.0/coop/factories/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      226 2024-03-08 04:25:45.000000 coop-6.0.0/coop/factories/attributes.py
+-rw-rw-rw-   0 root         (0) root         (0)     2284 2024-03-08 04:25:45.000000 coop-6.0.0/coop/factories/blocks.py
+-rw-rw-rw-   0 root         (0) root         (0)     1413 2024-03-08 04:25:45.000000 coop-6.0.0/coop/factories/fuzzy.py
+-rw-rw-rw-   0 root         (0) root         (0)      164 2024-03-08 04:25:45.000000 coop-6.0.0/coop/factories/inline.py
+-rw-rw-rw-   0 root         (0) root         (0)       71 2024-03-08 04:25:45.000000 coop-6.0.0/coop/factories/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 04:25:53.162389 coop-6.0.0/coop/form_builder/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-08 04:25:44.000000 coop-6.0.0/coop/form_builder/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5193 2024-03-08 04:25:44.000000 coop-6.0.0/coop/form_builder/blocks.py
+-rw-rw-rw-   0 root         (0) root         (0)     2618 2024-03-08 04:25:44.000000 coop-6.0.0/coop/form_builder/factories.py
+-rw-rw-rw-   0 root         (0) root         (0)      254 2024-03-08 04:25:44.000000 coop-6.0.0/coop/form_builder/forms.py
+-rw-rw-rw-   0 root         (0) root         (0)     1168 2024-03-08 04:25:44.000000 coop-6.0.0/coop/form_builder/page.py
+-rw-rw-rw-   0 root         (0) root         (0)     2468 2024-03-08 04:25:44.000000 coop-6.0.0/coop/form_builder/views.py
+-rw-rw-rw-   0 root         (0) root         (0)      238 2024-03-08 04:25:44.000000 coop-6.0.0/coop/forms.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 04:25:53.154389 coop-6.0.0/coop/jinja2/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 04:25:53.162389 coop-6.0.0/coop/jinja2/coop/
+-rw-rw-rw-   0 root         (0) root         (0)      567 2024-03-08 04:25:44.000000 coop-6.0.0/coop/jinja2/coop/analytics_warning.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 04:25:53.163389 coop-6.0.0/coop/jinja2tags/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-08 04:25:44.000000 coop-6.0.0/coop/jinja2tags/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6456 2024-03-08 04:25:44.000000 coop-6.0.0/coop/jinja2tags/core.py
+-rw-rw-rw-   0 root         (0) root         (0)      385 2024-03-08 04:25:44.000000 coop-6.0.0/coop/jinja2tags/vite.py
+-rw-rw-rw-   0 root         (0) root         (0)      438 2024-03-08 04:25:44.000000 coop-6.0.0/coop/jinja2tags/webpack.py
+-rw-rw-rw-   0 root         (0) root         (0)      527 2024-03-08 04:25:44.000000 coop-6.0.0/coop/logging.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 04:25:53.163389 coop-6.0.0/coop/management/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-08 04:25:44.000000 coop-6.0.0/coop/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 04:25:53.164389 coop-6.0.0/coop/management/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-08 04:25:44.000000 coop-6.0.0/coop/management/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1761 2024-03-08 04:25:44.000000 coop-6.0.0/coop/management/commands/phone_home.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 04:25:53.165389 coop-6.0.0/coop/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)      863 2024-03-08 04:25:44.000000 coop-6.0.0/coop/migrations/0001_remove_site.py
+-rw-rw-rw-   0 root         (0) root         (0)      949 2024-03-08 04:25:44.000000 coop-6.0.0/coop/migrations/0002_analyticssettings.py
+-rw-rw-rw-   0 root         (0) root         (0)      767 2024-03-08 04:25:44.000000 coop-6.0.0/coop/migrations/0003_tag_manager_settings.py
+-rw-rw-rw-   0 root         (0) root         (0)      822 2024-03-08 04:25:44.000000 coop-6.0.0/coop/migrations/0004_increase_analytics_length.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-08 04:25:44.000000 coop-6.0.0/coop/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      508 2024-03-08 04:25:44.000000 coop-6.0.0/coop/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     3340 2024-03-08 04:25:44.000000 coop-6.0.0/coop/page.py
+-rw-rw-rw-   0 root         (0) root         (0)     5858 2024-03-08 04:25:44.000000 coop-6.0.0/coop/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 04:25:53.165389 coop-6.0.0/coop/styleguide/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-08 04:25:44.000000 coop-6.0.0/coop/styleguide/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      206 2024-03-08 04:25:44.000000 coop-6.0.0/coop/styleguide/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)      188 2024-03-08 04:25:44.000000 coop-6.0.0/coop/styleguide/views.py
+-rw-rw-rw-   0 root         (0) root         (0)     4689 2024-03-08 04:25:44.000000 coop-6.0.0/coop/test.py
+-rw-rw-rw-   0 root         (0) root         (0)     2087 2024-03-08 04:25:44.000000 coop-6.0.0/coop/urls.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 04:25:53.166389 coop-6.0.0/coop/users/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-08 04:25:44.000000 coop-6.0.0/coop/users/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1971 2024-03-08 04:25:44.000000 coop-6.0.0/coop/users/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 04:25:53.167389 coop-6.0.0/coop/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-08 04:25:44.000000 coop-6.0.0/coop/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1591 2024-03-08 04:25:44.000000 coop-6.0.0/coop/utils/forms.py
+-rw-rw-rw-   0 root         (0) root         (0)      931 2024-03-08 04:25:44.000000 coop-6.0.0/coop/utils/mailchimp.py
+-rw-rw-rw-   0 root         (0) root         (0)      628 2024-03-08 04:25:44.000000 coop-6.0.0/coop/utils/migrations.py
+-rw-rw-rw-   0 root         (0) root         (0)      578 2024-03-08 04:25:44.000000 coop-6.0.0/coop/utils/pagination.py
+-rw-rw-rw-   0 root         (0) root         (0)      699 2024-03-08 04:25:44.000000 coop-6.0.0/coop/utils/rich_text_example.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 04:25:53.168389 coop-6.0.0/coop/utils/test_documents/
+-rw-rw-rw-   0 root         (0) root         (0)   504692 2024-03-08 04:25:44.000000 coop-6.0.0/coop/utils/test_documents/magazine-article.pdf
+-rw-rw-rw-   0 root         (0) root         (0)   515133 2024-03-08 04:25:44.000000 coop-6.0.0/coop/utils/test_documents/nj-logos.pdf
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 04:25:53.174389 coop-6.0.0/coop/utils/test_images/
+-rw-rw-rw-   0 root         (0) root         (0)  3653229 2024-03-08 04:25:44.000000 coop-6.0.0/coop/utils/test_images/landscape-large.jpg
+-rw-rw-rw-   0 root         (0) root         (0)    11487 2024-03-08 04:25:44.000000 coop-6.0.0/coop/utils/test_images/landscape-small.jpeg
+-rw-rw-rw-   0 root         (0) root         (0)  2821960 2024-03-08 04:25:44.000000 coop-6.0.0/coop/utils/test_images/portrait-large.jpg
+-rw-rw-rw-   0 root         (0) root         (0)     6608 2024-03-08 04:25:44.000000 coop-6.0.0/coop/utils/test_images/portrait-small.jpeg
+-rw-rw-rw-   0 root         (0) root         (0)     8126 2024-03-08 04:25:44.000000 coop-6.0.0/coop/utils/testdata.py
+-rw-rw-rw-   0 root         (0) root         (0)     2025 2024-03-08 04:25:44.000000 coop-6.0.0/coop/utils/views.py
+-rw-rw-rw-   0 root         (0) root         (0)     1526 2024-03-08 04:25:44.000000 coop-6.0.0/coop/wagtail_hooks.py
+-rw-rw-rw-   0 root         (0) root         (0)      129 2024-03-08 04:25:44.000000 coop-6.0.0/coop/wsgi.py
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-03-08 04:25:44.000000 coop-6.0.0/coop/wsgi_dev.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 04:25:53.175389 coop-6.0.0/coop.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2903 2024-03-08 04:25:53.000000 coop-6.0.0/coop.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1846 2024-03-08 04:25:53.000000 coop-6.0.0/coop.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-03-08 04:25:53.000000 coop-6.0.0/coop.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-03-08 04:25:53.000000 coop-6.0.0/coop.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      384 2024-03-08 04:25:53.000000 coop-6.0.0/coop.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2024-03-08 04:25:53.000000 coop-6.0.0/coop.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      237 2024-03-08 04:25:53.176389 coop-6.0.0/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1914 2024-03-08 04:25:44.000000 coop-6.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 04:25:53.174389 coop-6.0.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     1653 2024-03-08 04:25:44.000000 coop-6.0.0/tests/test_analytics_panel.py
+-rw-rw-rw-   0 root         (0) root         (0)     2813 2024-03-08 04:25:44.000000 coop-6.0.0/tests/test_jinja2tags.py
+-rw-rw-rw-   0 root         (0) root         (0)     1252 2024-03-08 04:25:44.000000 coop-6.0.0/tests/test_page.py
+-rw-rw-rw-   0 root         (0) root         (0)      698 2024-03-08 04:25:44.000000 coop-6.0.0/tests/test_test.py
```

### Comparing `coop-5.2.3/PKG-INFO` & `coop-6.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coop
-Version: 5.2.3
+Version: 6.0.0
 Summary: Standard base to build Wagtail sites from
 Home-page: https://gitlab.com/neonjungle/coop
 Author: Neon Jungle
 Author-email: developers@neonjungle.studio
 License: BSD License
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
@@ -13,24 +13,24 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Framework :: Django
 Classifier: License :: OSI Approved :: BSD License
-Requires-Dist: wagtail~=5.2.0
-Requires-Dist: django<4.3,>=3.2
-Requires-Dist: psycopg2-binary~=2.9.0
+Requires-Dist: wagtail~=6.0.0
+Requires-Dist: django<=5.0,>=4.2
+Requires-Dist: psycopg[binary]~=3.1.0
 Requires-Dist: pytz>=0
 Requires-Dist: Jinja2~=3.1.0
-Requires-Dist: django-htmx~=1.16.0
-Requires-Dist: django-honeypot~=1.0.0
+Requires-Dist: django-htmx~=1.17.0
+Requires-Dist: django-honeypot~=1.1.0
 Requires-Dist: wagtail-metadata~=5.0.0
 Requires-Dist: wagtail-icomoon
-Requires-Dist: wagtail-cache~=2.3.0
+Requires-Dist: wagtail-cache~=2.4.0
 Requires-Dist: wagtail-factories~=4.1.0
 Requires-Dist: sentry-sdk
 Provides-Extra: all
 Requires-Dist: mailchimp3~=3.0.0; extra == "all"
 Requires-Dist: diskcache~=5.2.0; extra == "all"
 Provides-Extra: cache
 Requires-Dist: diskcache~=5.2.0; extra == "cache"
```

### Comparing `coop-5.2.3/README.rst` & `coop-6.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `coop-5.2.3/coop/blocks.py` & `coop-6.0.0/coop/blocks.py`

 * *Files identical despite different names*

### Comparing `coop-5.2.3/coop/factories/blocks.py` & `coop-6.0.0/coop/factories/blocks.py`

 * *Files identical despite different names*

### Comparing `coop-5.2.3/coop/factories/fuzzy.py` & `coop-6.0.0/coop/factories/fuzzy.py`

 * *Files identical despite different names*

### Comparing `coop-5.2.3/coop/form_builder/blocks.py` & `coop-6.0.0/coop/form_builder/blocks.py`

 * *Files identical despite different names*

### Comparing `coop-5.2.3/coop/form_builder/factories.py` & `coop-6.0.0/coop/form_builder/factories.py`

 * *Files identical despite different names*

### Comparing `coop-5.2.3/coop/form_builder/page.py` & `coop-6.0.0/coop/form_builder/page.py`

 * *Files identical despite different names*

### Comparing `coop-5.2.3/coop/form_builder/views.py` & `coop-6.0.0/coop/form_builder/views.py`

 * *Files identical despite different names*

### Comparing `coop-5.2.3/coop/jinja2/coop/analytics_warning.html` & `coop-6.0.0/coop/jinja2/coop/analytics_warning.html`

 * *Files identical despite different names*

### Comparing `coop-5.2.3/coop/jinja2tags/core.py` & `coop-6.0.0/coop/jinja2tags/core.py`

 * *Files identical despite different names*

### Comparing `coop-5.2.3/coop/logging.py` & `coop-6.0.0/coop/logging.py`

 * *Files identical despite different names*

### Comparing `coop-5.2.3/coop/management/commands/phone_home.py` & `coop-6.0.0/coop/management/commands/phone_home.py`

 * *Files identical despite different names*

### Comparing `coop-5.2.3/coop/migrations/0001_remove_site.py` & `coop-6.0.0/coop/migrations/0001_remove_site.py`

 * *Files identical despite different names*

### Comparing `coop-5.2.3/coop/migrations/0002_analyticssettings.py` & `coop-6.0.0/coop/migrations/0002_analyticssettings.py`

 * *Files identical despite different names*

### Comparing `coop-5.2.3/coop/migrations/0003_tag_manager_settings.py` & `coop-6.0.0/coop/migrations/0003_tag_manager_settings.py`

 * *Files identical despite different names*

### Comparing `coop-5.2.3/coop/migrations/0004_increase_analytics_length.py` & `coop-6.0.0/coop/migrations/0004_increase_analytics_length.py`

 * *Files identical despite different names*

### Comparing `coop-5.2.3/coop/page.py` & `coop-6.0.0/coop/page.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,17 @@
         label = self._meta.label.split(".")
         app = label[0]
         model_name = "_".join(re.findall("^[a-z]+|[A-Z][^A-Z]*", label[1])).lower()
         return "layouts/{}/{}.html".format(app, model_name)
 
     def get_object_title(self):
         site = self.get_site()
-        return f"{self.get_meta_title()} | {site.site_name}"
+        if site:
+            return f"{self.get_meta_title()} | {site.site_name}"
+        return self.get_meta_title()
 
     class Meta:
         abstract = True
 
 
 class ContactPageMixin(models.Model):
     contact_form_class = ContactForm
```

### Comparing `coop-5.2.3/coop/settings.py` & `coop-6.0.0/coop/settings.py`

 * *Files identical despite different names*

### Comparing `coop-5.2.3/coop/test.py` & `coop-6.0.0/coop/test.py`

 * *Files identical despite different names*

### Comparing `coop-5.2.3/coop/urls.py` & `coop-6.0.0/coop/urls.py`

 * *Files identical despite different names*

### Comparing `coop-5.2.3/coop/users/models.py` & `coop-6.0.0/coop/users/models.py`

 * *Files identical despite different names*

### Comparing `coop-5.2.3/coop/utils/forms.py` & `coop-6.0.0/coop/utils/forms.py`

 * *Files identical despite different names*

### Comparing `coop-5.2.3/coop/utils/mailchimp.py` & `coop-6.0.0/coop/utils/mailchimp.py`

 * *Files identical despite different names*

### Comparing `coop-5.2.3/coop/utils/migrations.py` & `coop-6.0.0/coop/utils/migrations.py`

 * *Files identical despite different names*

### Comparing `coop-5.2.3/coop/utils/pagination.py` & `coop-6.0.0/coop/utils/pagination.py`

 * *Files identical despite different names*

### Comparing `coop-5.2.3/coop/utils/rich_text_example.html` & `coop-6.0.0/coop/utils/rich_text_example.html`

 * *Files identical despite different names*

### Comparing `coop-5.2.3/coop/utils/test_documents/magazine-article.pdf` & `coop-6.0.0/coop/utils/test_documents/magazine-article.pdf`

 * *Files identical despite different names*

### Comparing `coop-5.2.3/coop/utils/test_documents/nj-logos.pdf` & `coop-6.0.0/coop/utils/test_documents/nj-logos.pdf`

 * *Files identical despite different names*

### Comparing `coop-5.2.3/coop/utils/test_images/landscape-large.jpg` & `coop-6.0.0/coop/utils/test_images/landscape-large.jpg`

 * *Files identical despite different names*

### Comparing `coop-5.2.3/coop/utils/test_images/landscape-small.jpeg` & `coop-6.0.0/coop/utils/test_images/landscape-small.jpeg`

 * *Files identical despite different names*

### Comparing `coop-5.2.3/coop/utils/test_images/portrait-large.jpg` & `coop-6.0.0/coop/utils/test_images/portrait-large.jpg`

 * *Files identical despite different names*

### Comparing `coop-5.2.3/coop/utils/test_images/portrait-small.jpeg` & `coop-6.0.0/coop/utils/test_images/portrait-small.jpeg`

 * *Files identical despite different names*

### Comparing `coop-5.2.3/coop/utils/testdata.py` & `coop-6.0.0/coop/utils/testdata.py`

 * *Files identical despite different names*

### Comparing `coop-5.2.3/coop/utils/views.py` & `coop-6.0.0/coop/utils/views.py`

 * *Files identical despite different names*

### Comparing `coop-5.2.3/coop/wagtail_hooks.py` & `coop-6.0.0/coop/wagtail_hooks.py`

 * *Files identical despite different names*

### Comparing `coop-5.2.3/coop.egg-info/PKG-INFO` & `coop-6.0.0/coop.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coop
-Version: 5.2.3
+Version: 6.0.0
 Summary: Standard base to build Wagtail sites from
 Home-page: https://gitlab.com/neonjungle/coop
 Author: Neon Jungle
 Author-email: developers@neonjungle.studio
 License: BSD License
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
@@ -13,24 +13,24 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Framework :: Django
 Classifier: License :: OSI Approved :: BSD License
-Requires-Dist: wagtail~=5.2.0
-Requires-Dist: django<4.3,>=3.2
-Requires-Dist: psycopg2-binary~=2.9.0
+Requires-Dist: wagtail~=6.0.0
+Requires-Dist: django<=5.0,>=4.2
+Requires-Dist: psycopg[binary]~=3.1.0
 Requires-Dist: pytz>=0
 Requires-Dist: Jinja2~=3.1.0
-Requires-Dist: django-htmx~=1.16.0
-Requires-Dist: django-honeypot~=1.0.0
+Requires-Dist: django-htmx~=1.17.0
+Requires-Dist: django-honeypot~=1.1.0
 Requires-Dist: wagtail-metadata~=5.0.0
 Requires-Dist: wagtail-icomoon
-Requires-Dist: wagtail-cache~=2.3.0
+Requires-Dist: wagtail-cache~=2.4.0
 Requires-Dist: wagtail-factories~=4.1.0
 Requires-Dist: sentry-sdk
 Provides-Extra: all
 Requires-Dist: mailchimp3~=3.0.0; extra == "all"
 Requires-Dist: diskcache~=5.2.0; extra == "all"
 Provides-Extra: cache
 Requires-Dist: diskcache~=5.2.0; extra == "cache"
```

### Comparing `coop-5.2.3/coop.egg-info/SOURCES.txt` & `coop-6.0.0/coop.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `coop-5.2.3/setup.py` & `coop-6.0.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,24 +18,24 @@
     version=version,
     description="Standard base to build Wagtail sites from",
     long_description=readme,
     author="Neon Jungle",
     author_email="developers@neonjungle.studio",
     url="https://gitlab.com/neonjungle/coop",
     install_requires=[
-        "wagtail~=5.2.0",
-        "django>=3.2,<4.3",
-        "psycopg2-binary~=2.9.0",
+        "wagtail~=6.0.0",
+        "django>=4.2,<=5.0",
+        "psycopg[binary]~=3.1.0",
         "pytz>=0",
         "Jinja2~=3.1.0",
-        "django-htmx~=1.16.0",
-        "django-honeypot~=1.0.0",
+        "django-htmx~=1.17.0",
+        "django-honeypot~=1.1.0",
         "wagtail-metadata~=5.0.0",
         "wagtail-icomoon",
-        "wagtail-cache~=2.3.0",
+        "wagtail-cache~=2.4.0",
         "wagtail-factories~=4.1.0",
         "sentry-sdk",
     ],
     extras_require={
         "all": [
             "mailchimp3~=3.0.0",
             "diskcache~=5.2.0",
```

### Comparing `coop-5.2.3/tests/test_analytics_panel.py` & `coop-6.0.0/tests/test_analytics_panel.py`

 * *Files identical despite different names*

### Comparing `coop-5.2.3/tests/test_jinja2tags.py` & `coop-6.0.0/tests/test_jinja2tags.py`

 * *Files identical despite different names*

### Comparing `coop-5.2.3/tests/test_page.py` & `coop-6.0.0/tests/test_page.py`

 * *Files identical despite different names*

### Comparing `coop-5.2.3/tests/test_test.py` & `coop-6.0.0/tests/test_test.py`

 * *Files identical despite different names*

