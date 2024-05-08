# Comparing `tmp/cjops-1.0.5.tar.gz` & `tmp/cjops-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cjops-1.0.5.tar", last modified: Wed May  8 06:11:43 2024, max compression
+gzip compressed data, was "cjops-1.0.6.tar", last modified: Wed May  8 06:13:06 2024, max compression
```

## Comparing `cjops-1.0.5.tar` & `cjops-1.0.6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 caojie     (501) staff       (20)        0 2024-05-08 06:11:43.571551 cjops-1.0.5/
--rw-r--r--   0 caojie     (501) staff       (20)     1068 2024-03-15 01:36:01.000000 cjops-1.0.5/LICENSE
--rw-r--r--   0 caojie     (501) staff       (20)      383 2024-05-08 06:11:43.571152 cjops-1.0.5/PKG-INFO
--rw-r--r--   0 caojie     (501) staff       (20)     1483 2024-04-25 10:03:23.000000 cjops-1.0.5/README.md
--rw-r--r--   0 caojie     (501) staff       (20)       38 2024-05-08 06:11:43.571637 cjops-1.0.5/setup.cfg
--rw-r--r--   0 caojie     (501) staff       (20)     3065 2024-05-08 06:11:18.000000 cjops-1.0.5/setup.py
-drwxr-xr-x   0 caojie     (501) staff       (20)        0 2024-05-08 06:11:43.559543 cjops-1.0.5/src/
-drwxr-xr-x   0 caojie     (501) staff       (20)        0 2024-05-08 06:11:43.568061 cjops-1.0.5/src/cjops/
--rw-r--r--   0 caojie     (501) staff       (20)      200 2024-05-08 00:48:52.000000 cjops-1.0.5/src/cjops/__init__.py
--rw-r--r--   0 caojie     (501) staff       (20)      333 2024-05-08 06:02:24.000000 cjops-1.0.5/src/cjops/__version__.py
--rw-r--r--   0 caojie     (501) staff       (20)     4608 2024-05-08 03:14:13.000000 cjops-1.0.5/src/cjops/aliyun.py
--rw-r--r--   0 caojie     (501) staff       (20)     2157 2024-04-15 06:29:32.000000 cjops-1.0.5/src/cjops/command.py
--rw-r--r--   0 caojie     (501) staff       (20)     4791 2024-05-07 07:49:15.000000 cjops-1.0.5/src/cjops/domain.py
--rw-r--r--   0 caojie     (501) staff       (20)     1795 2024-04-19 07:29:32.000000 cjops-1.0.5/src/cjops/email.py
--rw-r--r--   0 caojie     (501) staff       (20)     8459 2024-04-25 02:58:56.000000 cjops-1.0.5/src/cjops/excel.py
--rw-r--r--   0 caojie     (501) staff       (20)      127 2024-05-08 00:48:52.000000 cjops-1.0.5/src/cjops/info.py
--rw-r--r--   0 caojie     (501) staff       (20)      870 2024-04-12 07:35:23.000000 cjops-1.0.5/src/cjops/qw.py
--rw-r--r--   0 caojie     (501) staff       (20)     1411 2024-04-19 08:45:16.000000 cjops-1.0.5/src/cjops/sql.py
--rw-r--r--   0 caojie     (501) staff       (20)     2078 2024-05-07 09:24:16.000000 cjops-1.0.5/src/cjops/time.py
--rw-r--r--   0 caojie     (501) staff       (20)     6456 2024-05-07 07:55:52.000000 cjops-1.0.5/src/cjops/utils.py
-drwxr-xr-x   0 caojie     (501) staff       (20)        0 2024-05-08 06:11:43.570625 cjops-1.0.5/src/cjops.egg-info/
--rw-r--r--   0 caojie     (501) staff       (20)      383 2024-05-08 06:11:43.000000 cjops-1.0.5/src/cjops.egg-info/PKG-INFO
--rw-r--r--   0 caojie     (501) staff       (20)      456 2024-05-08 06:11:43.000000 cjops-1.0.5/src/cjops.egg-info/SOURCES.txt
--rw-r--r--   0 caojie     (501) staff       (20)        1 2024-05-08 06:11:43.000000 cjops-1.0.5/src/cjops.egg-info/dependency_links.txt
--rw-r--r--   0 caojie     (501) staff       (20)        1 2024-05-07 08:48:08.000000 cjops-1.0.5/src/cjops.egg-info/not-zip-safe
--rw-r--r--   0 caojie     (501) staff       (20)       15 2024-05-08 06:11:43.000000 cjops-1.0.5/src/cjops.egg-info/requires.txt
--rw-r--r--   0 caojie     (501) staff       (20)        6 2024-05-08 06:11:43.000000 cjops-1.0.5/src/cjops.egg-info/top_level.txt
+drwxr-xr-x   0 caojie     (501) staff       (20)        0 2024-05-08 06:13:06.513515 cjops-1.0.6/
+-rw-r--r--   0 caojie     (501) staff       (20)     1068 2024-03-15 01:36:01.000000 cjops-1.0.6/LICENSE
+-rw-r--r--   0 caojie     (501) staff       (20)      383 2024-05-08 06:13:06.513002 cjops-1.0.6/PKG-INFO
+-rw-r--r--   0 caojie     (501) staff       (20)     1483 2024-04-25 10:03:23.000000 cjops-1.0.6/README.md
+-rw-r--r--   0 caojie     (501) staff       (20)       38 2024-05-08 06:13:06.513611 cjops-1.0.6/setup.cfg
+-rw-r--r--   0 caojie     (501) staff       (20)     3090 2024-05-08 06:12:31.000000 cjops-1.0.6/setup.py
+drwxr-xr-x   0 caojie     (501) staff       (20)        0 2024-05-08 06:13:06.499918 cjops-1.0.6/src/
+drwxr-xr-x   0 caojie     (501) staff       (20)        0 2024-05-08 06:13:06.508970 cjops-1.0.6/src/cjops/
+-rw-r--r--   0 caojie     (501) staff       (20)      200 2024-05-08 00:48:52.000000 cjops-1.0.6/src/cjops/__init__.py
+-rw-r--r--   0 caojie     (501) staff       (20)      333 2024-05-08 06:12:40.000000 cjops-1.0.6/src/cjops/__version__.py
+-rw-r--r--   0 caojie     (501) staff       (20)     4608 2024-05-08 03:14:13.000000 cjops-1.0.6/src/cjops/aliyun.py
+-rw-r--r--   0 caojie     (501) staff       (20)     2157 2024-04-15 06:29:32.000000 cjops-1.0.6/src/cjops/command.py
+-rw-r--r--   0 caojie     (501) staff       (20)     4791 2024-05-07 07:49:15.000000 cjops-1.0.6/src/cjops/domain.py
+-rw-r--r--   0 caojie     (501) staff       (20)     1795 2024-04-19 07:29:32.000000 cjops-1.0.6/src/cjops/email.py
+-rw-r--r--   0 caojie     (501) staff       (20)     8459 2024-04-25 02:58:56.000000 cjops-1.0.6/src/cjops/excel.py
+-rw-r--r--   0 caojie     (501) staff       (20)      127 2024-05-08 00:48:52.000000 cjops-1.0.6/src/cjops/info.py
+-rw-r--r--   0 caojie     (501) staff       (20)      870 2024-04-12 07:35:23.000000 cjops-1.0.6/src/cjops/qw.py
+-rw-r--r--   0 caojie     (501) staff       (20)     1411 2024-04-19 08:45:16.000000 cjops-1.0.6/src/cjops/sql.py
+-rw-r--r--   0 caojie     (501) staff       (20)     2078 2024-05-07 09:24:16.000000 cjops-1.0.6/src/cjops/time.py
+-rw-r--r--   0 caojie     (501) staff       (20)     6456 2024-05-07 07:55:52.000000 cjops-1.0.6/src/cjops/utils.py
+drwxr-xr-x   0 caojie     (501) staff       (20)        0 2024-05-08 06:13:06.512299 cjops-1.0.6/src/cjops.egg-info/
+-rw-r--r--   0 caojie     (501) staff       (20)      383 2024-05-08 06:13:06.000000 cjops-1.0.6/src/cjops.egg-info/PKG-INFO
+-rw-r--r--   0 caojie     (501) staff       (20)      456 2024-05-08 06:13:06.000000 cjops-1.0.6/src/cjops.egg-info/SOURCES.txt
+-rw-r--r--   0 caojie     (501) staff       (20)        1 2024-05-08 06:13:06.000000 cjops-1.0.6/src/cjops.egg-info/dependency_links.txt
+-rw-r--r--   0 caojie     (501) staff       (20)        1 2024-05-07 08:48:08.000000 cjops-1.0.6/src/cjops.egg-info/not-zip-safe
+-rw-r--r--   0 caojie     (501) staff       (20)       15 2024-05-08 06:13:06.000000 cjops-1.0.6/src/cjops.egg-info/requires.txt
+-rw-r--r--   0 caojie     (501) staff       (20)        6 2024-05-08 06:13:06.000000 cjops-1.0.6/src/cjops.egg-info/top_level.txt
```

### Comparing `cjops-1.0.5/LICENSE` & `cjops-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `cjops-1.0.5/README.md` & `cjops-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `cjops-1.0.5/setup.py` & `cjops-1.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     long_description = fh.read()
 
 # 默认发布命令
 if sys.argv[-1] == "publish" or sys.argv[-2] == "publish":
     os.system(f"rm -rf build {package}.egg-info dist")
     os.system("python setup.py sdist bdist_wheel")
     os.system("twine upload --skip-existing --repository-url https://upload.pypi.org/legacy/  dist/*")
+    os.system("sleep 5")
     os.system(f"pip uninstall {package} -y && pip install -U {package} -i https://pypi.org/simple")
     sys.exit()
 
 cjops_requires = [
         'aliyun-log-python-sdk>=0.8.15',
         'requests>=2.31.0',
         'loguru>=0.6.0',
```

### Comparing `cjops-1.0.5/src/cjops/aliyun.py` & `cjops-1.0.6/src/cjops/aliyun.py`

 * *Files identical despite different names*

### Comparing `cjops-1.0.5/src/cjops/command.py` & `cjops-1.0.6/src/cjops/command.py`

 * *Files identical despite different names*

### Comparing `cjops-1.0.5/src/cjops/domain.py` & `cjops-1.0.6/src/cjops/domain.py`

 * *Files identical despite different names*

### Comparing `cjops-1.0.5/src/cjops/email.py` & `cjops-1.0.6/src/cjops/email.py`

 * *Files identical despite different names*

### Comparing `cjops-1.0.5/src/cjops/excel.py` & `cjops-1.0.6/src/cjops/excel.py`

 * *Files identical despite different names*

### Comparing `cjops-1.0.5/src/cjops/qw.py` & `cjops-1.0.6/src/cjops/qw.py`

 * *Files identical despite different names*

### Comparing `cjops-1.0.5/src/cjops/sql.py` & `cjops-1.0.6/src/cjops/sql.py`

 * *Files identical despite different names*

### Comparing `cjops-1.0.5/src/cjops/time.py` & `cjops-1.0.6/src/cjops/time.py`

 * *Files identical despite different names*

### Comparing `cjops-1.0.5/src/cjops/utils.py` & `cjops-1.0.6/src/cjops/utils.py`

 * *Files identical despite different names*

