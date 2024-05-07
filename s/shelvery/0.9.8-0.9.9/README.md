# Comparing `tmp/shelvery-0.9.8.tar.gz` & `tmp/shelvery-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shelvery-0.9.8.tar", last modified: Thu Apr 27 02:51:51 2023, max compression
+gzip compressed data, was "shelvery-0.9.9.tar", last modified: Tue May  7 23:42:52 2024, max compression
```

## Comparing `shelvery-0.9.8.tar` & `shelvery-0.9.9.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 02:51:51.363486 shelvery-0.9.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-04-27 02:51:35.000000 shelvery-0.9.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-27 02:51:51.363486 shelvery-0.9.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    21023 2023-04-27 02:51:35.000000 shelvery-0.9.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 02:51:51.363486 shelvery-0.9.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-04-27 02:51:35.000000 shelvery-0.9.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 02:51:51.363486 shelvery-0.9.8/shelvery/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-27 02:51:35.000000 shelvery-0.9.8/shelvery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-04-27 02:51:35.000000 shelvery-0.9.8/shelvery/aws_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     8888 2023-04-27 02:51:35.000000 shelvery-0.9.8/shelvery/backup_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    15628 2023-04-27 02:51:35.000000 shelvery-0.9.8/shelvery/documentdb_backup.py
--rw-r--r--   0 runner    (1001) docker     (123)     8222 2023-04-27 02:51:35.000000 shelvery-0.9.8/shelvery/ebs_backup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-04-27 02:51:35.000000 shelvery-0.9.8/shelvery/ec2_backup.py
--rw-r--r--   0 runner    (1001) docker     (123)    10747 2023-04-27 02:51:35.000000 shelvery-0.9.8/shelvery/ec2ami_backup.py
--rw-r--r--   0 runner    (1001) docker     (123)    40843 2023-04-27 02:51:35.000000 shelvery-0.9.8/shelvery/engine.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-27 02:51:35.000000 shelvery-0.9.8/shelvery/entity_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-04-27 02:51:35.000000 shelvery-0.9.8/shelvery/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-04-27 02:51:35.000000 shelvery-0.9.8/shelvery/notifications.py
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-04-27 02:51:35.000000 shelvery-0.9.8/shelvery/queue.py
--rw-r--r--   0 runner    (1001) docker     (123)    17185 2023-04-27 02:51:35.000000 shelvery-0.9.8/shelvery/rds_backup.py
--rw-r--r--   0 runner    (1001) docker     (123)    17594 2023-04-27 02:51:35.000000 shelvery-0.9.8/shelvery/rds_cluster_backup.py
--rw-r--r--   0 runner    (1001) docker     (123)    11496 2023-04-27 02:51:35.000000 shelvery-0.9.8/shelvery/redshift_backup.py
--rw-r--r--   0 runner    (1001) docker     (123)    14825 2023-04-27 02:51:35.000000 shelvery-0.9.8/shelvery/runtime_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-04-27 02:51:35.000000 shelvery-0.9.8/shelvery/shelvery_invoker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 02:51:51.363486 shelvery-0.9.8/shelvery.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-27 02:51:51.000000 shelvery-0.9.8/shelvery.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-04-27 02:51:51.000000 shelvery-0.9.8/shelvery.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 02:51:51.000000 shelvery-0.9.8/shelvery.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-27 02:51:51.000000 shelvery-0.9.8/shelvery.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-27 02:51:51.000000 shelvery-0.9.8/shelvery.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 02:51:51.000000 shelvery-0.9.8/shelvery.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 02:51:51.363486 shelvery-0.9.8/shelvery_cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 02:51:35.000000 shelvery-0.9.8/shelvery_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-04-27 02:51:35.000000 shelvery-0.9.8/shelvery_cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-04-27 02:51:35.000000 shelvery-0.9.8/shelvery_cli/shelver_cli_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 02:51:51.363486 shelvery-0.9.8/shelvery_lambda/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 02:51:35.000000 shelvery-0.9.8/shelvery_lambda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-04-27 02:51:35.000000 shelvery-0.9.8/shelvery_lambda/lambda_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:42:52.764177 shelvery-0.9.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-07 23:42:41.000000 shelvery-0.9.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-07 23:42:52.764177 shelvery-0.9.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    21023 2024-05-07 23:42:41.000000 shelvery-0.9.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 23:42:52.764177 shelvery-0.9.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-05-07 23:42:41.000000 shelvery-0.9.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:42:52.764177 shelvery-0.9.9/shelvery/
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-07 23:42:41.000000 shelvery-0.9.9/shelvery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4209 2024-05-07 23:42:41.000000 shelvery-0.9.9/shelvery/aws_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8888 2024-05-07 23:42:41.000000 shelvery-0.9.9/shelvery/backup_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15628 2024-05-07 23:42:41.000000 shelvery-0.9.9/shelvery/documentdb_backup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8222 2024-05-07 23:42:41.000000 shelvery-0.9.9/shelvery/ebs_backup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-05-07 23:42:41.000000 shelvery-0.9.9/shelvery/ec2_backup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10747 2024-05-07 23:42:41.000000 shelvery-0.9.9/shelvery/ec2ami_backup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40843 2024-05-07 23:42:41.000000 shelvery-0.9.9/shelvery/engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-05-07 23:42:41.000000 shelvery-0.9.9/shelvery/entity_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-07 23:42:41.000000 shelvery-0.9.9/shelvery/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      941 2024-05-07 23:42:41.000000 shelvery-0.9.9/shelvery/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-05-07 23:42:41.000000 shelvery-0.9.9/shelvery/queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17185 2024-05-07 23:42:41.000000 shelvery-0.9.9/shelvery/rds_backup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17594 2024-05-07 23:42:41.000000 shelvery-0.9.9/shelvery/rds_cluster_backup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11496 2024-05-07 23:42:41.000000 shelvery-0.9.9/shelvery/redshift_backup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14825 2024-05-07 23:42:41.000000 shelvery-0.9.9/shelvery/runtime_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2542 2024-05-07 23:42:41.000000 shelvery-0.9.9/shelvery/shelvery_invoker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:42:52.764177 shelvery-0.9.9/shelvery.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-07 23:42:52.000000 shelvery-0.9.9/shelvery.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-05-07 23:42:52.000000 shelvery-0.9.9/shelvery.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 23:42:52.000000 shelvery-0.9.9/shelvery.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-07 23:42:52.000000 shelvery-0.9.9/shelvery.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-07 23:42:52.000000 shelvery-0.9.9/shelvery.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 23:42:52.000000 shelvery-0.9.9/shelvery.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:42:52.764177 shelvery-0.9.9/shelvery_cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 23:42:41.000000 shelvery-0.9.9/shelvery_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-05-07 23:42:41.000000 shelvery-0.9.9/shelvery_cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-07 23:42:41.000000 shelvery-0.9.9/shelvery_cli/shelver_cli_main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:42:52.764177 shelvery-0.9.9/shelvery_lambda/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 23:42:41.000000 shelvery-0.9.9/shelvery_lambda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-05-07 23:42:41.000000 shelvery-0.9.9/shelvery_lambda/lambda_handler.py
```

### Comparing `shelvery-0.9.8/LICENSE.txt` & `shelvery-0.9.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `shelvery-0.9.8/README.md` & `shelvery-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `shelvery-0.9.8/setup.py` & `shelvery-0.9.9/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-setup(name='shelvery', version='0.9.8', author='Base2Services R&D',
+setup(name='shelvery', version='0.9.9', author='Base2Services R&D',
       author_email='itsupport@base2services.com',
       url='http://github.com/base2Services/shelvery-aws-backups',
       classifiers=[
           'Development Status :: 3 - Alpha',
           'Programming Language :: Python :: 3.6',
           'Intended Audience :: System Administrators',
           'Intended Audience :: Information Technology',
```

### Comparing `shelvery-0.9.8/shelvery/aws_helper.py` & `shelvery-0.9.9/shelvery/aws_helper.py`

 * *Files identical despite different names*

### Comparing `shelvery-0.9.8/shelvery/backup_resource.py` & `shelvery-0.9.9/shelvery/backup_resource.py`

 * *Files identical despite different names*

### Comparing `shelvery-0.9.8/shelvery/documentdb_backup.py` & `shelvery-0.9.9/shelvery/documentdb_backup.py`

 * *Files identical despite different names*

### Comparing `shelvery-0.9.8/shelvery/ebs_backup.py` & `shelvery-0.9.9/shelvery/ebs_backup.py`

 * *Files identical despite different names*

### Comparing `shelvery-0.9.8/shelvery/ec2_backup.py` & `shelvery-0.9.9/shelvery/ec2_backup.py`

 * *Files identical despite different names*

### Comparing `shelvery-0.9.8/shelvery/ec2ami_backup.py` & `shelvery-0.9.9/shelvery/ec2ami_backup.py`

 * *Files identical despite different names*

### Comparing `shelvery-0.9.8/shelvery/engine.py` & `shelvery-0.9.9/shelvery/engine.py`

 * *Files identical despite different names*

### Comparing `shelvery-0.9.8/shelvery/entity_resource.py` & `shelvery-0.9.9/shelvery/entity_resource.py`

 * *Files identical despite different names*

### Comparing `shelvery-0.9.8/shelvery/factory.py` & `shelvery-0.9.9/shelvery/factory.py`

 * *Files identical despite different names*

### Comparing `shelvery-0.9.8/shelvery/notifications.py` & `shelvery-0.9.9/shelvery/notifications.py`

 * *Files identical despite different names*

### Comparing `shelvery-0.9.8/shelvery/queue.py` & `shelvery-0.9.9/shelvery/queue.py`

 * *Files identical despite different names*

### Comparing `shelvery-0.9.8/shelvery/rds_backup.py` & `shelvery-0.9.9/shelvery/rds_backup.py`

 * *Files identical despite different names*

### Comparing `shelvery-0.9.8/shelvery/rds_cluster_backup.py` & `shelvery-0.9.9/shelvery/rds_cluster_backup.py`

 * *Files identical despite different names*

### Comparing `shelvery-0.9.8/shelvery/redshift_backup.py` & `shelvery-0.9.9/shelvery/redshift_backup.py`

 * *Files identical despite different names*

### Comparing `shelvery-0.9.8/shelvery/runtime_config.py` & `shelvery-0.9.9/shelvery/runtime_config.py`

 * *Files identical despite different names*

### Comparing `shelvery-0.9.8/shelvery/shelvery_invoker.py` & `shelvery-0.9.9/shelvery/shelvery_invoker.py`

 * *Files identical despite different names*

### Comparing `shelvery-0.9.8/shelvery.egg-info/SOURCES.txt` & `shelvery-0.9.9/shelvery.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `shelvery-0.9.8/shelvery_cli/__main__.py` & `shelvery-0.9.9/shelvery_cli/__main__.py`

 * *Files identical despite different names*

### Comparing `shelvery-0.9.8/shelvery_lambda/lambda_handler.py` & `shelvery-0.9.9/shelvery_lambda/lambda_handler.py`

 * *Files identical despite different names*

