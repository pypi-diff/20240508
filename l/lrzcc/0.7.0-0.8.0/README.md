# Comparing `tmp/lrzcc-0.7.0.tar.gz` & `tmp/lrzcc-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lrzcc-0.7.0.tar", last modified: Wed Apr  3 14:46:10 2024, max compression
+gzip compressed data, was "lrzcc-0.8.0.tar", last modified: Wed May  8 19:51:09 2024, max compression
```

## Comparing `lrzcc-0.7.0.tar` & `lrzcc-0.8.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 sandro    (1000) alarm     (1000)        0 2024-04-03 14:46:10.347506 lrzcc-0.7.0/
--rw-r--r--   0 sandro    (1000) alarm     (1000)     1086 2024-04-03 12:55:26.000000 lrzcc-0.7.0/LICENSE
--rw-r--r--   0 sandro    (1000) alarm     (1000)     2634 2024-04-03 14:46:10.347506 lrzcc-0.7.0/PKG-INFO
--rw-r--r--   0 sandro    (1000) alarm     (1000)      142 2024-04-03 14:28:04.000000 lrzcc-0.7.0/README.md
--rw-r--r--   0 sandro    (1000) alarm     (1000)     1272 2024-04-03 14:23:01.000000 lrzcc-0.7.0/pyproject.toml
--rw-r--r--   0 sandro    (1000) alarm     (1000)       38 2024-04-03 14:46:10.347506 lrzcc-0.7.0/setup.cfg
-drwxr-xr-x   0 sandro    (1000) alarm     (1000)        0 2024-04-03 14:46:10.346506 lrzcc-0.7.0/src/
--rw-r--r--   0 sandro    (1000) alarm     (1000)        0 2024-04-03 12:47:02.000000 lrzcc-0.7.0/src/__init__.py
--rw-r--r--   0 sandro    (1000) alarm     (1000)    36436 2023-12-14 22:23:14.000000 lrzcc-0.7.0/src/accounting.py
--rw-r--r--   0 sandro    (1000) alarm     (1000)    17804 2024-02-28 16:48:41.000000 lrzcc-0.7.0/src/budgeting.py
--rw-r--r--   0 sandro    (1000) alarm     (1000)     7710 2024-04-03 11:43:42.000000 lrzcc-0.7.0/src/common.py
--rw-r--r--   0 sandro    (1000) alarm     (1000)     1577 2023-11-02 14:08:42.000000 lrzcc-0.7.0/src/hello.py
-drwxr-xr-x   0 sandro    (1000) alarm     (1000)        0 2024-04-03 14:46:10.347506 lrzcc-0.7.0/src/lrzcc.egg-info/
--rw-r--r--   0 sandro    (1000) alarm     (1000)     2634 2024-04-03 14:46:10.000000 lrzcc-0.7.0/src/lrzcc.egg-info/PKG-INFO
--rw-r--r--   0 sandro    (1000) alarm     (1000)      379 2024-04-03 14:46:10.000000 lrzcc-0.7.0/src/lrzcc.egg-info/SOURCES.txt
--rw-r--r--   0 sandro    (1000) alarm     (1000)        1 2024-04-03 14:46:10.000000 lrzcc-0.7.0/src/lrzcc.egg-info/dependency_links.txt
--rw-r--r--   0 sandro    (1000) alarm     (1000)       36 2024-04-03 14:46:10.000000 lrzcc-0.7.0/src/lrzcc.egg-info/entry_points.txt
--rw-r--r--   0 sandro    (1000) alarm     (1000)      121 2024-04-03 14:46:10.000000 lrzcc-0.7.0/src/lrzcc.egg-info/requires.txt
--rw-r--r--   0 sandro    (1000) alarm     (1000)       77 2024-04-03 14:46:10.000000 lrzcc-0.7.0/src/lrzcc.egg-info/top_level.txt
--rwxr-xr-x   0 sandro    (1000) alarm     (1000)     8982 2024-04-03 14:15:06.000000 lrzcc-0.7.0/src/main.py
--rw-r--r--   0 sandro    (1000) alarm     (1000)     6254 2024-04-03 11:43:42.000000 lrzcc-0.7.0/src/pricing.py
--rw-r--r--   0 sandro    (1000) alarm     (1000)     6278 2023-11-02 14:09:20.000000 lrzcc-0.7.0/src/quota.py
--rw-r--r--   0 sandro    (1000) alarm     (1000)    13631 2023-11-02 14:09:19.000000 lrzcc-0.7.0/src/resources.py
--rw-r--r--   0 sandro    (1000) alarm     (1000)    11717 2024-04-03 11:43:42.000000 lrzcc-0.7.0/src/user.py
+drwxr-xr-x   0 sandro    (1000) alarm     (1000)        0 2024-05-08 19:51:09.925159 lrzcc-0.8.0/
+-rw-r--r--   0 sandro    (1000) alarm     (1000)     1086 2024-04-03 12:55:26.000000 lrzcc-0.8.0/LICENSE
+-rw-r--r--   0 sandro    (1000) alarm     (1000)     5114 2024-05-08 19:51:09.925159 lrzcc-0.8.0/PKG-INFO
+-rw-r--r--   0 sandro    (1000) alarm     (1000)     2622 2024-04-19 16:46:53.000000 lrzcc-0.8.0/README.md
+-rw-r--r--   0 sandro    (1000) alarm     (1000)     1272 2024-05-08 19:46:23.000000 lrzcc-0.8.0/pyproject.toml
+-rw-r--r--   0 sandro    (1000) alarm     (1000)       38 2024-05-08 19:51:09.925159 lrzcc-0.8.0/setup.cfg
+drwxr-xr-x   0 sandro    (1000) alarm     (1000)        0 2024-05-08 19:51:09.925159 lrzcc-0.8.0/src/
+-rw-r--r--   0 sandro    (1000) alarm     (1000)        0 2024-04-03 12:47:02.000000 lrzcc-0.8.0/src/__init__.py
+-rw-r--r--   0 sandro    (1000) alarm     (1000)    36436 2023-12-14 22:23:14.000000 lrzcc-0.8.0/src/accounting.py
+-rw-r--r--   0 sandro    (1000) alarm     (1000)    17804 2024-02-28 16:48:41.000000 lrzcc-0.8.0/src/budgeting.py
+-rw-r--r--   0 sandro    (1000) alarm     (1000)     7710 2024-05-08 12:49:21.000000 lrzcc-0.8.0/src/common.py
+-rw-r--r--   0 sandro    (1000) alarm     (1000)     1577 2023-11-02 14:08:42.000000 lrzcc-0.8.0/src/hello.py
+drwxr-xr-x   0 sandro    (1000) alarm     (1000)        0 2024-05-08 19:51:09.925159 lrzcc-0.8.0/src/lrzcc.egg-info/
+-rw-r--r--   0 sandro    (1000) alarm     (1000)     5114 2024-05-08 19:51:09.000000 lrzcc-0.8.0/src/lrzcc.egg-info/PKG-INFO
+-rw-r--r--   0 sandro    (1000) alarm     (1000)      379 2024-05-08 19:51:09.000000 lrzcc-0.8.0/src/lrzcc.egg-info/SOURCES.txt
+-rw-r--r--   0 sandro    (1000) alarm     (1000)        1 2024-05-08 19:51:09.000000 lrzcc-0.8.0/src/lrzcc.egg-info/dependency_links.txt
+-rw-r--r--   0 sandro    (1000) alarm     (1000)       36 2024-05-08 19:51:09.000000 lrzcc-0.8.0/src/lrzcc.egg-info/entry_points.txt
+-rw-r--r--   0 sandro    (1000) alarm     (1000)      121 2024-05-08 19:51:09.000000 lrzcc-0.8.0/src/lrzcc.egg-info/requires.txt
+-rw-r--r--   0 sandro    (1000) alarm     (1000)       77 2024-05-08 19:51:09.000000 lrzcc-0.8.0/src/lrzcc.egg-info/top_level.txt
+-rwxr-xr-x   0 sandro    (1000) alarm     (1000)     8982 2024-05-08 12:49:21.000000 lrzcc-0.8.0/src/main.py
+-rw-r--r--   0 sandro    (1000) alarm     (1000)     6254 2024-04-03 11:43:42.000000 lrzcc-0.8.0/src/pricing.py
+-rw-r--r--   0 sandro    (1000) alarm     (1000)     6278 2023-11-02 14:09:20.000000 lrzcc-0.8.0/src/quota.py
+-rw-r--r--   0 sandro    (1000) alarm     (1000)    13998 2024-05-08 12:07:05.000000 lrzcc-0.8.0/src/resources.py
+-rw-r--r--   0 sandro    (1000) alarm     (1000)    11717 2024-05-08 12:49:21.000000 lrzcc-0.8.0/src/user.py
```

### Comparing `lrzcc-0.7.0/LICENSE` & `lrzcc-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lrzcc-0.7.0/pyproject.toml` & `lrzcc-0.8.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "lrzcc"
-version = "0.7.0"
+version = "0.8.0"
 dependencies = [
     "argcomplete==3.1.1",
     "certifi==2023.5.7",
     "charset-normalizer==3.2.0",
     "idna==3.4",
     "requests==2.31.0",
     "tabulate==0.9.0",
```

### Comparing `lrzcc-0.7.0/src/accounting.py` & `lrzcc-0.8.0/src/accounting.py`

 * *Files identical despite different names*

### Comparing `lrzcc-0.7.0/src/budgeting.py` & `lrzcc-0.8.0/src/budgeting.py`

 * *Files identical despite different names*

### Comparing `lrzcc-0.7.0/src/common.py` & `lrzcc-0.8.0/src/common.py`

 * *Files identical despite different names*

### Comparing `lrzcc-0.7.0/src/hello.py` & `lrzcc-0.8.0/src/hello.py`

 * *Files identical despite different names*

### Comparing `lrzcc-0.7.0/src/main.py` & `lrzcc-0.8.0/src/main.py`

 * *Files identical despite different names*

### Comparing `lrzcc-0.7.0/src/pricing.py` & `lrzcc-0.8.0/src/pricing.py`

 * *Files identical despite different names*

### Comparing `lrzcc-0.7.0/src/quota.py` & `lrzcc-0.8.0/src/quota.py`

 * *Files identical despite different names*

### Comparing `lrzcc-0.7.0/src/resources.py` & `lrzcc-0.8.0/src/resources.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from datetime import datetime
 import sys
 
 from common import (do_nothing, print_response, api_request, valid_datetime,
                     parse_flavor, parse_flavor_group, generate_modify_data,
                     parse_user, parse_project)
 
-cmds = ['flavor', 'flavor-group']
+cmds = ['flavor', 'flavor-group', 'usage']
 cmds_with_sub_cmds = ['flavor', 'flavor-group']
 
 
 # TODO we should probably use type annotations everywhere, here I'm just using
 # it, so that my editor can give me suggestions
 def setup_parsers(main_subparsers: _SubParsersAction):
     '''setup the quota parser'''
@@ -301,14 +301,21 @@
     flavor_group_usage_parser.add_argument(
         "-A",
         "--aggregate",
         action="store_true",
         help="Aggregate the flavor usage for all filtered users",
     )
 
+    # usage parser
+    usage_parser: ArgumentParser = main_subparsers.add_parser(
+        "usage",
+        help="Show usage of the entire cloud",
+        )
+    parsers['usage'] = usage_parser
+
     # avoid variable not used warnings
     do_nothing(flavor_group_initialize_parser)
 
     return parsers
 
 
 def parse_args(args: Namespace):
@@ -464,7 +471,13 @@
     if args.aggregate:
         params += "&aggregate=True"
     if params:
         params = '?' + params[1:]
     resp = api_request('get', f'/resources/flavorgroups/usage/{params}', None,
                        args)
     print_response(resp, args)
+
+
+def usage(args: Namespace):
+    '''show usage of the entire cloud'''
+    resp = api_request('get', '/resources/usage/', None, args)
+    print_response(resp, args)
```

### Comparing `lrzcc-0.7.0/src/user.py` & `lrzcc-0.8.0/src/user.py`

 * *Files identical despite different names*

