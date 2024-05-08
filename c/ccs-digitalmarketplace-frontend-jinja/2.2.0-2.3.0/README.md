# Comparing `tmp/ccs-digitalmarketplace-frontend-jinja-2.2.0.tar.gz` & `tmp/ccs-digitalmarketplace-frontend-jinja-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ccs-digitalmarketplace-frontend-jinja-2.2.0.tar", last modified: Fri Apr 26 09:51:05 2024, max compression
+gzip compressed data, was "ccs-digitalmarketplace-frontend-jinja-2.3.0.tar", last modified: Wed May  8 14:05:49 2024, max compression
```

## Comparing `ccs-digitalmarketplace-frontend-jinja-2.2.0.tar` & `ccs-digitalmarketplace-frontend-jinja-2.3.0.tar`

### file list

```diff
@@ -1,16 +1,123 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 09:51:05.802806 ccs-digitalmarketplace-frontend-jinja-2.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-26 09:50:57.000000 ccs-digitalmarketplace-frontend-jinja-2.2.0/LICENCE
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-26 09:51:05.802806 ccs-digitalmarketplace-frontend-jinja-2.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7264 2024-04-26 09:50:57.000000 ccs-digitalmarketplace-frontend-jinja-2.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 09:51:05.802806 ccs-digitalmarketplace-frontend-jinja-2.2.0/app/
--rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-04-26 09:50:57.000000 ccs-digitalmarketplace-frontend-jinja-2.2.0/app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 09:51:05.802806 ccs-digitalmarketplace-frontend-jinja-2.2.0/ccs_digitalmarketplace_frontend_jinja.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-26 09:51:05.000000 ccs-digitalmarketplace-frontend-jinja-2.2.0/ccs_digitalmarketplace_frontend_jinja.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-26 09:51:05.000000 ccs-digitalmarketplace-frontend-jinja-2.2.0/ccs_digitalmarketplace_frontend_jinja.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 09:51:05.000000 ccs-digitalmarketplace-frontend-jinja-2.2.0/ccs_digitalmarketplace_frontend_jinja.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-26 09:51:05.000000 ccs-digitalmarketplace-frontend-jinja-2.2.0/ccs_digitalmarketplace_frontend_jinja.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 09:51:05.000000 ccs-digitalmarketplace-frontend-jinja-2.2.0/ccs_digitalmarketplace_frontend_jinja.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 09:51:05.802806 ccs-digitalmarketplace-frontend-jinja-2.2.0/digitalmarketplace_frontend_jinja/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-26 09:50:57.000000 ccs-digitalmarketplace-frontend-jinja-2.2.0/digitalmarketplace_frontend_jinja/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 09:51:05.802806 ccs-digitalmarketplace-frontend-jinja-2.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-04-26 09:50:57.000000 ccs-digitalmarketplace-frontend-jinja-2.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:05:49.919839 ccs-digitalmarketplace-frontend-jinja-2.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-05-08 14:05:37.000000 ccs-digitalmarketplace-frontend-jinja-2.3.0/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-08 14:05:49.919839 ccs-digitalmarketplace-frontend-jinja-2.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7462 2024-05-08 14:05:37.000000 ccs-digitalmarketplace-frontend-jinja-2.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:05:49.911839 ccs-digitalmarketplace-frontend-jinja-2.3.0/app/
+-rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-05-08 14:05:37.000000 ccs-digitalmarketplace-frontend-jinja-2.3.0/app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:05:49.911839 ccs-digitalmarketplace-frontend-jinja-2.3.0/ccs_digitalmarketplace_frontend_jinja.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-08 14:05:49.000000 ccs-digitalmarketplace-frontend-jinja-2.3.0/ccs_digitalmarketplace_frontend_jinja.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4990 2024-05-08 14:05:49.000000 ccs-digitalmarketplace-frontend-jinja-2.3.0/ccs_digitalmarketplace_frontend_jinja.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 14:05:49.000000 ccs-digitalmarketplace-frontend-jinja-2.3.0/ccs_digitalmarketplace_frontend_jinja.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-08 14:05:49.000000 ccs-digitalmarketplace-frontend-jinja-2.3.0/ccs_digitalmarketplace_frontend_jinja.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 14:05:49.000000 ccs-digitalmarketplace-frontend-jinja-2.3.0/ccs_digitalmarketplace_frontend_jinja.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:05:49.911839 ccs-digitalmarketplace-frontend-jinja-2.3.0/digitalmarketplace_frontend_jinja/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-08 14:05:37.000000 ccs-digitalmarketplace-frontend-jinja-2.3.0/digitalmarketplace_frontend_jinja/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:05:49.911839 ccs-digitalmarketplace-frontend-jinja-2.3.0/digitalmarketplace_frontend_jinja/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:05:49.911839 ccs-digitalmarketplace-frontend-jinja-2.3.0/digitalmarketplace_frontend_jinja/templates/components/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:05:49.911839 ccs-digitalmarketplace-frontend-jinja-2.3.0/digitalmarketplace_frontend_jinja/templates/components/alert/
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-08 14:05:37.000000 ccs-digitalmarketplace-frontend-jinja-2.3.0/digitalmarketplace_frontend_jinja/templates/components/alert/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:05:49.911839 ccs-digitalmarketplace-frontend-jinja-2.3.0/digitalmarketplace_frontend_jinja/templates/components/attachment/
+-rw-r--r--   0 runner    (1001) docker     (127)     6452 2024-05-08 14:05:37.000000 ccs-digitalmarketplace-frontend-jinja-2.3.0/digitalmarketplace_frontend_jinja/templates/components/attachment/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:05:49.911839 ccs-digitalmarketplace-frontend-jinja-2.3.0/digitalmarketplace_frontend_jinja/templates/components/banner/
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-05-08 14:05:37.000000 ccs-digitalmarketplace-frontend-jinja-2.3.0/digitalmarketplace_frontend_jinja/templates/components/banner/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:05:49.911839 ccs-digitalmarketplace-frontend-jinja-2.3.0/digitalmarketplace_frontend_jinja/templates/components/character-count-from-form/
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-05-08 14:05:37.000000 ccs-digitalmarketplace-frontend-jinja-2.3.0/digitalmarketplace_frontend_jinja/templates/components/character-count-from-form/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:05:49.911839 ccs-digitalmarketplace-frontend-jinja-2.3.0/digitalmarketplace_frontend_jinja/templates/components/checkboxes-from-form/
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-05-08 14:05:37.000000 ccs-digitalmarketplace-frontend-jinja-2.3.0/digitalmarketplace_frontend_jinja/templates/components/checkboxes-from-form/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:05:49.911839 ccs-digitalmarketplace-frontend-jinja-2.3.0/digitalmarketplace_frontend_jinja/templates/components/compliance-communication-attachment-row/
+-rw-r--r--   0 runner    (1001) docker     (127)     2668 2024-05-08 14:05:37.000000 ccs-digitalmarketplace-frontend-jinja-2.3.0/digitalmarketplace_frontend_jinja/templates/components/compliance-communication-attachment-row/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:05:49.911839 ccs-digitalmarketplace-frontend-jinja-2.3.0/digitalmarketplace_frontend_jinja/templates/components/compliance-communication-attachments/
+-rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-05-08 14:05:37.000000 ccs-digitalmarketplace-frontend-jinja-2.3.0/digitalmarketplace_frontend_jinja/templates/components/compliance-communication-attachments/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:05:49.911839 ccs-digitalmarketplace-frontend-jinja-2.3.0/digitalmarketplace_frontend_jinja/templates/components/cookie-banner/
+-rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-05-08 14:05:37.000000 ccs-digitalmarketplace-frontend-jinja-2.3.0/digitalmarketplace_frontend_jinja/templates/components/cookie-banner/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:05:49.911839 ccs-digitalmarketplace-frontend-jinja-2.3.0/digitalmarketplace_frontend_jinja/templates/components/documents/
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-05-08 14:05:37.000000 ccs-digitalmarketplace-frontend-jinja-2.3.0/digitalmarketplace_frontend_jinja/templates/components/documents/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:05:49.915839 ccs-digitalmarketplace-frontend-jinja-2.3.0/digitalmarketplace_frontend_jinja/templates/components/file-upload-from-form/
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-08 14:05:37.000000 ccs-digitalmarketplace-frontend-jinja-2.3.0/digitalmarketplace_frontend_jinja/templates/components/file-upload-from-form/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:05:49.915839 ccs-digitalmarketplace-frontend-jinja-2.3.0/digitalmarketplace_frontend_jinja/templates/components/footer/
+-rw-r--r--   0 runner    (1001) docker     (127)     2958 2024-05-08 14:05:37.000000 ccs-digitalmarketplace-frontend-jinja-2.3.0/digitalmarketplace_frontend_jinja/templates/components/footer/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:05:49.915839 ccs-digitalmarketplace-frontend-jinja-2.3.0/digitalmarketplace_frontend_jinja/templates/components/header/
+-rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-05-08 14:05:37.000000 ccs-digitalmarketplace-frontend-jinja-2.3.0/digitalmarketplace_frontend_jinja/templates/components/header/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:05:49.915839 ccs-digitalmarketplace-frontend-jinja-2.3.0/digitalmarketplace_frontend_jinja/templates/components/input-from-form/
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-08 14:05:37.000000 ccs-digitalmarketplace-frontend-jinja-2.3.0/digitalmarketplace_frontend_jinja/templates/components/input-from-form/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:05:49.915839 ccs-digitalmarketplace-frontend-jinja-2.3.0/digitalmarketplace_frontend_jinja/templates/components/list-input/
+-rw-r--r--   0 runner    (1001) docker     (127)     5756 2024-05-08 14:05:37.000000 ccs-digitalmarketplace-frontend-jinja-2.3.0/digitalmarketplace_frontend_jinja/templates/components/list-input/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:05:49.915839 ccs-digitalmarketplace-frontend-jinja-2.3.0/digitalmarketplace_frontend_jinja/templates/components/new-framework-banner/
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-08 14:05:37.000000 ccs-digitalmarketplace-frontend-jinja-2.3.0/digitalmarketplace_frontend_jinja/templates/components/new-framework-banner/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:05:49.915839 ccs-digitalmarketplace-frontend-jinja-2.3.0/digitalmarketplace_frontend_jinja/templates/components/option-select/
+-rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-05-08 14:05:37.000000 ccs-digitalmarketplace-frontend-jinja-2.3.0/digitalmarketplace_frontend_jinja/templates/components/option-select/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:05:49.915839 ccs-digitalmarketplace-frontend-jinja-2.3.0/digitalmarketplace_frontend_jinja/templates/components/previous-next-pagination/
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-08 14:05:37.000000 ccs-digitalmarketplace-frontend-jinja-2.3.0/digitalmarketplace_frontend_jinja/templates/components/previous-next-pagination/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:05:49.915839 ccs-digitalmarketplace-frontend-jinja-2.3.0/digitalmarketplace_frontend_jinja/templates/components/question/
+-rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-05-08 14:05:37.000000 ccs-digitalmarketplace-frontend-jinja-2.3.0/digitalmarketplace_frontend_jinja/templates/components/question/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:05:49.907839 ccs-digitalmarketplace-frontend-jinja-2.3.0/digitalmarketplace_frontend_jinja/templates/components/question/macros/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:05:49.915839 ccs-digitalmarketplace-frontend-jinja-2.3.0/digitalmarketplace_frontend_jinja/templates/components/question/macros/boolean/
+-rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-05-08 14:05:37.000000 ccs-digitalmarketplace-frontend-jinja-2.3.0/digitalmarketplace_frontend_jinja/templates/components/question/macros/boolean/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:05:49.915839 ccs-digitalmarketplace-frontend-jinja-2.3.0/digitalmarketplace_frontend_jinja/templates/components/question/macros/character-count/
+-rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-05-08 14:05:37.000000 ccs-digitalmarketplace-frontend-jinja-2.3.0/digitalmarketplace_frontend_jinja/templates/components/question/macros/character-count/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:05:49.915839 ccs-digitalmarketplace-frontend-jinja-2.3.0/digitalmarketplace_frontend_jinja/templates/components/question/macros/checkbox-tree/
+-rw-r--r--   0 runner    (1001) docker     (127)     3547 2024-05-08 14:05:37.000000 ccs-digitalmarketplace-frontend-jinja-2.3.0/digitalmarketplace_frontend_jinja/templates/components/question/macros/checkbox-tree/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:05:49.915839 ccs-digitalmarketplace-frontend-jinja-2.3.0/digitalmarketplace_frontend_jinja/templates/components/question/macros/checkboxes/
+-rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-05-08 14:05:37.000000 ccs-digitalmarketplace-frontend-jinja-2.3.0/digitalmarketplace_frontend_jinja/templates/components/question/macros/checkboxes/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:05:49.915839 ccs-digitalmarketplace-frontend-jinja-2.3.0/digitalmarketplace_frontend_jinja/templates/components/question/macros/date/
+-rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-05-08 14:05:37.000000 ccs-digitalmarketplace-frontend-jinja-2.3.0/digitalmarketplace_frontend_jinja/templates/components/question/macros/date/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:05:49.915839 ccs-digitalmarketplace-frontend-jinja-2.3.0/digitalmarketplace_frontend_jinja/templates/components/question/macros/format-hint/
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-08 14:05:37.000000 ccs-digitalmarketplace-frontend-jinja-2.3.0/digitalmarketplace_frontend_jinja/templates/components/question/macros/format-hint/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:05:49.915839 ccs-digitalmarketplace-frontend-jinja-2.3.0/digitalmarketplace_frontend_jinja/templates/components/question/macros/list/
+-rw-r--r--   0 runner    (1001) docker     (127)     3512 2024-05-08 14:05:37.000000 ccs-digitalmarketplace-frontend-jinja-2.3.0/digitalmarketplace_frontend_jinja/templates/components/question/macros/list/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:05:49.915839 ccs-digitalmarketplace-frontend-jinja-2.3.0/digitalmarketplace_frontend_jinja/templates/components/question/macros/multiquestion/
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-08 14:05:37.000000 ccs-digitalmarketplace-frontend-jinja-2.3.0/digitalmarketplace_frontend_jinja/templates/components/question/macros/multiquestion/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:05:49.915839 ccs-digitalmarketplace-frontend-jinja-2.3.0/digitalmarketplace_frontend_jinja/templates/components/question/macros/number/
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-05-08 14:05:37.000000 ccs-digitalmarketplace-frontend-jinja-2.3.0/digitalmarketplace_frontend_jinja/templates/components/question/macros/number/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:05:49.915839 ccs-digitalmarketplace-frontend-jinja-2.3.0/digitalmarketplace_frontend_jinja/templates/components/question/macros/pricing/
+-rw-r--r--   0 runner    (1001) docker     (127)     6247 2024-05-08 14:05:37.000000 ccs-digitalmarketplace-frontend-jinja-2.3.0/digitalmarketplace_frontend_jinja/templates/components/question/macros/pricing/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:05:49.915839 ccs-digitalmarketplace-frontend-jinja-2.3.0/digitalmarketplace_frontend_jinja/templates/components/question/macros/radios/
+-rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-05-08 14:05:37.000000 ccs-digitalmarketplace-frontend-jinja-2.3.0/digitalmarketplace_frontend_jinja/templates/components/question/macros/radios/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:05:49.915839 ccs-digitalmarketplace-frontend-jinja-2.3.0/digitalmarketplace_frontend_jinja/templates/components/question/macros/text/
+-rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-05-08 14:05:37.000000 ccs-digitalmarketplace-frontend-jinja-2.3.0/digitalmarketplace_frontend_jinja/templates/components/question/macros/text/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:05:49.915839 ccs-digitalmarketplace-frontend-jinja-2.3.0/digitalmarketplace_frontend_jinja/templates/components/question/macros/upload/
+-rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-05-08 14:05:37.000000 ccs-digitalmarketplace-frontend-jinja-2.3.0/digitalmarketplace_frontend_jinja/templates/components/question/macros/upload/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:05:49.915839 ccs-digitalmarketplace-frontend-jinja-2.3.0/digitalmarketplace_frontend_jinja/templates/components/radios-from-form/
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-05-08 14:05:37.000000 ccs-digitalmarketplace-frontend-jinja-2.3.0/digitalmarketplace_frontend_jinja/templates/components/radios-from-form/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:05:49.915839 ccs-digitalmarketplace-frontend-jinja-2.3.0/digitalmarketplace_frontend_jinja/templates/components/search-box/
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-08 14:05:37.000000 ccs-digitalmarketplace-frontend-jinja-2.3.0/digitalmarketplace_frontend_jinja/templates/components/search-box/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:05:49.915839 ccs-digitalmarketplace-frontend-jinja-2.3.0/digitalmarketplace_frontend_jinja/templates/components/select/
+-rw-r--r--   0 runner    (1001) docker     (127)     3272 2024-05-08 14:05:37.000000 ccs-digitalmarketplace-frontend-jinja-2.3.0/digitalmarketplace_frontend_jinja/templates/components/select/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:05:49.915839 ccs-digitalmarketplace-frontend-jinja-2.3.0/digitalmarketplace_frontend_jinja/templates/components/select-country-from-form/
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-08 14:05:37.000000 ccs-digitalmarketplace-frontend-jinja-2.3.0/digitalmarketplace_frontend_jinja/templates/components/select-country-from-form/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:05:49.919839 ccs-digitalmarketplace-frontend-jinja-2.3.0/digitalmarketplace_frontend_jinja/templates/components/summary-content/
+-rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-05-08 14:05:37.000000 ccs-digitalmarketplace-frontend-jinja-2.3.0/digitalmarketplace_frontend_jinja/templates/components/summary-content/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:05:49.911839 ccs-digitalmarketplace-frontend-jinja-2.3.0/digitalmarketplace_frontend_jinja/templates/components/summary-content/macros/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:05:49.919839 ccs-digitalmarketplace-frontend-jinja-2.3.0/digitalmarketplace_frontend_jinja/templates/components/summary-content/macros/boolean/
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-08 14:05:37.000000 ccs-digitalmarketplace-frontend-jinja-2.3.0/digitalmarketplace_frontend_jinja/templates/components/summary-content/macros/boolean/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:05:49.919839 ccs-digitalmarketplace-frontend-jinja-2.3.0/digitalmarketplace_frontend_jinja/templates/components/summary-content/macros/checkbox-tree/
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-08 14:05:37.000000 ccs-digitalmarketplace-frontend-jinja-2.3.0/digitalmarketplace_frontend_jinja/templates/components/summary-content/macros/checkbox-tree/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:05:49.919839 ccs-digitalmarketplace-frontend-jinja-2.3.0/digitalmarketplace_frontend_jinja/templates/components/summary-content/macros/list/
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-08 14:05:37.000000 ccs-digitalmarketplace-frontend-jinja-2.3.0/digitalmarketplace_frontend_jinja/templates/components/summary-content/macros/list/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:05:49.919839 ccs-digitalmarketplace-frontend-jinja-2.3.0/digitalmarketplace_frontend_jinja/templates/components/summary-content/macros/list-items/
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-08 14:05:37.000000 ccs-digitalmarketplace-frontend-jinja-2.3.0/digitalmarketplace_frontend_jinja/templates/components/summary-content/macros/list-items/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:05:49.919839 ccs-digitalmarketplace-frontend-jinja-2.3.0/digitalmarketplace_frontend_jinja/templates/components/summary-content/macros/multiquestion/
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-05-08 14:05:37.000000 ccs-digitalmarketplace-frontend-jinja-2.3.0/digitalmarketplace_frontend_jinja/templates/components/summary-content/macros/multiquestion/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:05:49.919839 ccs-digitalmarketplace-frontend-jinja-2.3.0/digitalmarketplace_frontend_jinja/templates/components/summary-content/macros/number/
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-08 14:05:37.000000 ccs-digitalmarketplace-frontend-jinja-2.3.0/digitalmarketplace_frontend_jinja/templates/components/summary-content/macros/number/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:05:49.919839 ccs-digitalmarketplace-frontend-jinja-2.3.0/digitalmarketplace_frontend_jinja/templates/components/summary-content/macros/radios/
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-08 14:05:37.000000 ccs-digitalmarketplace-frontend-jinja-2.3.0/digitalmarketplace_frontend_jinja/templates/components/summary-content/macros/radios/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:05:49.919839 ccs-digitalmarketplace-frontend-jinja-2.3.0/digitalmarketplace_frontend_jinja/templates/components/summary-content/macros/service-id/
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-08 14:05:37.000000 ccs-digitalmarketplace-frontend-jinja-2.3.0/digitalmarketplace_frontend_jinja/templates/components/summary-content/macros/service-id/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:05:49.919839 ccs-digitalmarketplace-frontend-jinja-2.3.0/digitalmarketplace_frontend_jinja/templates/components/summary-content/macros/text/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-08 14:05:37.000000 ccs-digitalmarketplace-frontend-jinja-2.3.0/digitalmarketplace_frontend_jinja/templates/components/summary-content/macros/text/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:05:49.919839 ccs-digitalmarketplace-frontend-jinja-2.3.0/digitalmarketplace_frontend_jinja/templates/components/summary-content/macros/upload/
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-08 14:05:37.000000 ccs-digitalmarketplace-frontend-jinja-2.3.0/digitalmarketplace_frontend_jinja/templates/components/summary-content/macros/upload/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:05:49.919839 ccs-digitalmarketplace-frontend-jinja-2.3.0/digitalmarketplace_frontend_jinja/templates/components/temporary-message/
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-08 14:05:37.000000 ccs-digitalmarketplace-frontend-jinja-2.3.0/digitalmarketplace_frontend_jinja/templates/components/temporary-message/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:05:49.919839 ccs-digitalmarketplace-frontend-jinja-2.3.0/digitalmarketplace_frontend_jinja/templates/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-08 14:05:37.000000 ccs-digitalmarketplace-frontend-jinja-2.3.0/digitalmarketplace_frontend_jinja/templates/errors/400.html
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-08 14:05:37.000000 ccs-digitalmarketplace-frontend-jinja-2.3.0/digitalmarketplace_frontend_jinja/templates/errors/403.html
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-08 14:05:37.000000 ccs-digitalmarketplace-frontend-jinja-2.3.0/digitalmarketplace_frontend_jinja/templates/errors/404.html
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-05-08 14:05:37.000000 ccs-digitalmarketplace-frontend-jinja-2.3.0/digitalmarketplace_frontend_jinja/templates/errors/410.html
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-08 14:05:37.000000 ccs-digitalmarketplace-frontend-jinja-2.3.0/digitalmarketplace_frontend_jinja/templates/errors/500.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:05:49.919839 ccs-digitalmarketplace-frontend-jinja-2.3.0/digitalmarketplace_frontend_jinja/templates/layouts/
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-08 14:05:37.000000 ccs-digitalmarketplace-frontend-jinja-2.3.0/digitalmarketplace_frontend_jinja/templates/layouts/_custom_dimensions.html
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-08 14:05:37.000000 ccs-digitalmarketplace-frontend-jinja-2.3.0/digitalmarketplace_frontend_jinja/templates/layouts/_site_verification.html
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 14:05:49.919839 ccs-digitalmarketplace-frontend-jinja-2.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-05-08 14:05:37.000000 ccs-digitalmarketplace-frontend-jinja-2.3.0/setup.py
```

### Comparing `ccs-digitalmarketplace-frontend-jinja-2.2.0/LICENCE` & `ccs-digitalmarketplace-frontend-jinja-2.3.0/LICENCE`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-frontend-jinja-2.2.0/README.md` & `ccs-digitalmarketplace-frontend-jinja-2.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 Digital Marketplace Jinja Macros
 =========================
 
 ![Python 3.9](https://img.shields.io/badge/python-3.9-blue.svg)
+![Python 3.10](https://img.shields.io/badge/python-3.10-blue.svg)
+![Python 3.11](https://img.shields.io/badge/python-3.11-blue.svg)
+![Python 3.12](https://img.shields.io/badge/python-3.12-blue.svg)
 
 This repository provides a complete set of [Jinja](https://jinja.palletsprojects.com/) macros that are kept up-to-date and 100% compliant with [CCS Digital Marketplace GOV.UK Frontend](https://github.com/Crown-Commercial-Service/ccs-digitalmarketplace-govuk-frontend) Nunjucks macros. Porting is intentionally manual rather than automated to make updates simpler than maintaining an automated conversion routine. A comprehensive test suite ensures compliance against the latest, and every subsequent, CCS GOV.UK Frontend Frontend release.
 
 This project was inspired by the [GOV.UK Frontend Jinja Macros](https://github.com/LandRegistry/govuk-frontend-jinja) project by [HM Land Registry](https://github.com/LandRegistry) and we thank them for their work which has helped with this project.
 
 ## Compatibility
```

### Comparing `ccs-digitalmarketplace-frontend-jinja-2.2.0/app/__init__.py` & `ccs-digitalmarketplace-frontend-jinja-2.3.0/app/__init__.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-frontend-jinja-2.2.0/setup.py` & `ccs-digitalmarketplace-frontend-jinja-2.3.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,9 +30,9 @@
     package_data={'digitalmarketplace_frontend_jinja': components},
     include_package_data=True,
     install_requires=[
         'jinja2>3',
         'ccs-govuk-frontend-jinja>=1,<2',
         'ccs-digitalmarketplace-utils>=65.0.0',
     ],
-    python_requires=">=3.9,<3.12",
+    python_requires=">=3.9,<3.13",
 )
```

