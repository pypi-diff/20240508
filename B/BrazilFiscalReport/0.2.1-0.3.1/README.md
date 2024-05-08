# Comparing `tmp/BrazilFiscalReport-0.2.1.tar.gz` & `tmp/brazilfiscalreport-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BrazilFiscalReport-0.2.1.tar", last modified: Thu Mar 14 03:31:18 2024, max compression
+gzip compressed data, was "brazilfiscalreport-0.3.1.tar", last modified: Mon May  6 23:10:10 2024, max compression
```

## Comparing `BrazilFiscalReport-0.2.1.tar` & `brazilfiscalreport-0.3.1.tar`

### file list

```diff
@@ -1,18 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 03:31:18.549757 BrazilFiscalReport-0.2.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 03:31:18.549757 BrazilFiscalReport-0.2.1/BrazilFiscalReport.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-03-14 03:31:18.000000 BrazilFiscalReport-0.2.1/BrazilFiscalReport.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-03-14 03:31:18.000000 BrazilFiscalReport-0.2.1/BrazilFiscalReport.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-14 03:31:18.000000 BrazilFiscalReport-0.2.1/BrazilFiscalReport.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-14 03:31:18.000000 BrazilFiscalReport-0.2.1/BrazilFiscalReport.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-03-14 03:31:18.000000 BrazilFiscalReport-0.2.1/BrazilFiscalReport.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-03-14 03:31:12.000000 BrazilFiscalReport-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-03-14 03:31:18.549757 BrazilFiscalReport-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-03-14 03:31:12.000000 BrazilFiscalReport-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 03:31:18.549757 BrazilFiscalReport-0.2.1/brazilfiscalreport/
--rw-r--r--   0 runner    (1001) docker     (127)    74231 2024-03-14 03:31:12.000000 BrazilFiscalReport-0.2.1/brazilfiscalreport/pdf_docs.py
--rw-r--r--   0 runner    (1001) docker     (127)     7677 2024-03-14 03:31:12.000000 BrazilFiscalReport-0.2.1/brazilfiscalreport/xfpdf.py
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-03-14 03:31:12.000000 BrazilFiscalReport-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-14 03:31:18.549757 BrazilFiscalReport-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-03-14 03:31:12.000000 BrazilFiscalReport-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 03:31:18.549757 BrazilFiscalReport-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4059 2024-03-14 03:31:12.000000 BrazilFiscalReport-0.2.1/tests/test_brazil_fiscal_report.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 23:10:10.759791 brazilfiscalreport-0.3.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 23:10:10.759791 brazilfiscalreport-0.3.1/BrazilFiscalReport.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-06 23:10:10.000000 brazilfiscalreport-0.3.1/BrazilFiscalReport.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-05-06 23:10:10.000000 brazilfiscalreport-0.3.1/BrazilFiscalReport.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 23:10:10.000000 brazilfiscalreport-0.3.1/BrazilFiscalReport.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-06 23:10:10.000000 brazilfiscalreport-0.3.1/BrazilFiscalReport.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-06 23:10:10.000000 brazilfiscalreport-0.3.1/BrazilFiscalReport.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     7635 2024-05-06 23:10:07.000000 brazilfiscalreport-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-06 23:10:10.759791 brazilfiscalreport-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6751 2024-05-06 23:10:07.000000 brazilfiscalreport-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 23:10:10.755791 brazilfiscalreport-0.3.1/brazilfiscalreport/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 23:10:07.000000 brazilfiscalreport-0.3.1/brazilfiscalreport/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 23:10:10.755791 brazilfiscalreport-0.3.1/brazilfiscalreport/dacce/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-06 23:10:07.000000 brazilfiscalreport-0.3.1/brazilfiscalreport/dacce/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5380 2024-05-06 23:10:07.000000 brazilfiscalreport-0.3.1/brazilfiscalreport/dacce/dacce.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 23:10:10.759791 brazilfiscalreport-0.3.1/brazilfiscalreport/danfe/
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-06 23:10:07.000000 brazilfiscalreport-0.3.1/brazilfiscalreport/danfe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-05-06 23:10:07.000000 brazilfiscalreport-0.3.1/brazilfiscalreport/danfe/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51511 2024-05-06 23:10:07.000000 brazilfiscalreport-0.3.1/brazilfiscalreport/danfe/danfe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-05-06 23:10:07.000000 brazilfiscalreport-0.3.1/brazilfiscalreport/danfe/danfe_basic_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4248 2024-05-06 23:10:07.000000 brazilfiscalreport-0.3.1/brazilfiscalreport/danfe/danfe_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-06 23:10:07.000000 brazilfiscalreport-0.3.1/brazilfiscalreport/danfe/danfe_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-06 23:10:07.000000 brazilfiscalreport-0.3.1/brazilfiscalreport/danfe/danfe_conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-05-06 23:10:07.000000 brazilfiscalreport-0.3.1/brazilfiscalreport/danfe/danfe_emit_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-05-06 23:10:07.000000 brazilfiscalreport-0.3.1/brazilfiscalreport/danfe/danfe_ident_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-06 23:10:07.000000 brazilfiscalreport-0.3.1/brazilfiscalreport/danfe/danfe_verification_msg.py
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-06 23:10:07.000000 brazilfiscalreport-0.3.1/brazilfiscalreport/danfe/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-06 23:10:07.000000 brazilfiscalreport-0.3.1/brazilfiscalreport/pdf_element.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-05-06 23:10:07.000000 brazilfiscalreport-0.3.1/brazilfiscalreport/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-05-06 23:10:07.000000 brazilfiscalreport-0.3.1/brazilfiscalreport/xfpdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-06 23:10:07.000000 brazilfiscalreport-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 23:10:10.759791 brazilfiscalreport-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-06 23:10:07.000000 brazilfiscalreport-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 23:10:10.759791 brazilfiscalreport-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 23:10:07.000000 brazilfiscalreport-0.3.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7578 2024-05-06 23:10:07.000000 brazilfiscalreport-0.3.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-06 23:10:07.000000 brazilfiscalreport-0.3.1/tests/test_dacce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4323 2024-05-06 23:10:07.000000 brazilfiscalreport-0.3.1/tests/test_danfe.py
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-06 23:10:07.000000 brazilfiscalreport-0.3.1/tests/test_utils.py
```

