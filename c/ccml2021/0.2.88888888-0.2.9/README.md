# Comparing `tmp/ccml2021-0.2.88888888.tar.gz` & `tmp/ccml2021-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ccml2021-0.2.88888888.tar", last modified: Wed May  8 01:24:42 2024, max compression
+gzip compressed data, was "ccml2021-0.2.9.tar", last modified: Wed May  8 01:25:05 2024, max compression
```

## Comparing `ccml2021-0.2.88888888.tar` & `ccml2021-0.2.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 mrok       (501) staff       (20)        0 2024-05-08 01:24:42.865287 ccml2021-0.2.88888888/
--rw-r--r--   0 mrok       (501) staff       (20)      227 2024-05-08 01:24:42.865127 ccml2021-0.2.88888888/PKG-INFO
--rw-r--r--   0 mrok       (501) staff       (20)       37 2024-02-04 06:11:56.000000 ccml2021-0.2.88888888/README.md
-drwxr-xr-x   0 mrok       (501) staff       (20)        0 2024-05-08 01:24:42.863751 ccml2021-0.2.88888888/ccml2021/
--rw-r--r--   0 mrok       (501) staff       (20)        0 2024-02-04 03:28:17.000000 ccml2021-0.2.88888888/ccml2021/__init__.py
--rw-r--r--   0 mrok       (501) staff       (20)     6730 2024-05-07 14:49:38.000000 ccml2021-0.2.88888888/ccml2021/checker.py
--rw-r--r--   0 mrok       (501) staff       (20)     1155 2024-02-04 03:28:17.000000 ccml2021-0.2.88888888/ccml2021/gp.py
-drwxr-xr-x   0 mrok       (501) staff       (20)        0 2024-05-08 01:24:42.864670 ccml2021-0.2.88888888/ccml2021.egg-info/
--rw-r--r--   0 mrok       (501) staff       (20)      227 2024-05-08 01:24:42.000000 ccml2021-0.2.88888888/ccml2021.egg-info/PKG-INFO
--rw-r--r--   0 mrok       (501) staff       (20)      347 2024-05-08 01:24:42.000000 ccml2021-0.2.88888888/ccml2021.egg-info/SOURCES.txt
--rw-r--r--   0 mrok       (501) staff       (20)        1 2024-05-08 01:24:42.000000 ccml2021-0.2.88888888/ccml2021.egg-info/dependency_links.txt
--rw-r--r--   0 mrok       (501) staff       (20)       84 2024-05-08 01:24:42.000000 ccml2021-0.2.88888888/ccml2021.egg-info/entry_points.txt
--rw-r--r--   0 mrok       (501) staff       (20)        1 2024-05-08 01:24:42.000000 ccml2021-0.2.88888888/ccml2021.egg-info/not-zip-safe
--rw-r--r--   0 mrok       (501) staff       (20)       12 2024-05-08 01:24:42.000000 ccml2021-0.2.88888888/ccml2021.egg-info/requires.txt
--rw-r--r--   0 mrok       (501) staff       (20)        9 2024-05-08 01:24:42.000000 ccml2021-0.2.88888888/ccml2021.egg-info/top_level.txt
--rw-r--r--   0 mrok       (501) staff       (20)       38 2024-05-08 01:24:42.865334 ccml2021-0.2.88888888/setup.cfg
--rw-r--r--   0 mrok       (501) staff       (20)     1116 2024-05-07 14:50:49.000000 ccml2021-0.2.88888888/setup.py
-drwxr-xr-x   0 mrok       (501) staff       (20)        0 2024-05-08 01:24:42.864950 ccml2021-0.2.88888888/tests/
--rw-r--r--   0 mrok       (501) staff       (20)      902 2024-02-04 03:28:17.000000 ccml2021-0.2.88888888/tests/test_gp.py
--rw-r--r--   0 mrok       (501) staff       (20)      262 2024-02-04 03:28:17.000000 ccml2021-0.2.88888888/tests/test_virtual_reaction.py
+drwxr-xr-x   0 mrok       (501) staff       (20)        0 2024-05-08 01:25:05.432330 ccml2021-0.2.9/
+-rw-r--r--   0 mrok       (501) staff       (20)      220 2024-05-08 01:25:05.432124 ccml2021-0.2.9/PKG-INFO
+-rw-r--r--   0 mrok       (501) staff       (20)       37 2024-02-04 06:11:56.000000 ccml2021-0.2.9/README.md
+drwxr-xr-x   0 mrok       (501) staff       (20)        0 2024-05-08 01:25:05.430215 ccml2021-0.2.9/ccml2021/
+-rw-r--r--   0 mrok       (501) staff       (20)        0 2024-02-04 03:28:17.000000 ccml2021-0.2.9/ccml2021/__init__.py
+-rw-r--r--   0 mrok       (501) staff       (20)     6730 2024-05-07 14:49:38.000000 ccml2021-0.2.9/ccml2021/checker.py
+-rw-r--r--   0 mrok       (501) staff       (20)     1155 2024-02-04 03:28:17.000000 ccml2021-0.2.9/ccml2021/gp.py
+drwxr-xr-x   0 mrok       (501) staff       (20)        0 2024-05-08 01:25:05.431419 ccml2021-0.2.9/ccml2021.egg-info/
+-rw-r--r--   0 mrok       (501) staff       (20)      220 2024-05-08 01:25:05.000000 ccml2021-0.2.9/ccml2021.egg-info/PKG-INFO
+-rw-r--r--   0 mrok       (501) staff       (20)      347 2024-05-08 01:25:05.000000 ccml2021-0.2.9/ccml2021.egg-info/SOURCES.txt
+-rw-r--r--   0 mrok       (501) staff       (20)        1 2024-05-08 01:25:05.000000 ccml2021-0.2.9/ccml2021.egg-info/dependency_links.txt
+-rw-r--r--   0 mrok       (501) staff       (20)       84 2024-05-08 01:25:05.000000 ccml2021-0.2.9/ccml2021.egg-info/entry_points.txt
+-rw-r--r--   0 mrok       (501) staff       (20)        1 2024-05-08 01:25:05.000000 ccml2021-0.2.9/ccml2021.egg-info/not-zip-safe
+-rw-r--r--   0 mrok       (501) staff       (20)       12 2024-05-08 01:25:05.000000 ccml2021-0.2.9/ccml2021.egg-info/requires.txt
+-rw-r--r--   0 mrok       (501) staff       (20)        9 2024-05-08 01:25:05.000000 ccml2021-0.2.9/ccml2021.egg-info/top_level.txt
+-rw-r--r--   0 mrok       (501) staff       (20)       38 2024-05-08 01:25:05.432389 ccml2021-0.2.9/setup.cfg
+-rw-r--r--   0 mrok       (501) staff       (20)     1109 2024-05-08 01:25:03.000000 ccml2021-0.2.9/setup.py
+drwxr-xr-x   0 mrok       (501) staff       (20)        0 2024-05-08 01:25:05.431865 ccml2021-0.2.9/tests/
+-rw-r--r--   0 mrok       (501) staff       (20)      902 2024-02-04 03:28:17.000000 ccml2021-0.2.9/tests/test_gp.py
+-rw-r--r--   0 mrok       (501) staff       (20)      262 2024-02-04 03:28:17.000000 ccml2021-0.2.9/tests/test_virtual_reaction.py
```

### Comparing `ccml2021-0.2.88888888/ccml2021/checker.py` & `ccml2021-0.2.9/ccml2021/checker.py`

 * *Files identical despite different names*

### Comparing `ccml2021-0.2.88888888/ccml2021/gp.py` & `ccml2021-0.2.9/ccml2021/gp.py`

 * *Files identical despite different names*

### Comparing `ccml2021-0.2.88888888/setup.py` & `ccml2021-0.2.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 for val in extras_dict.values():
     extras_list.extend(val)
 
 if __name__ == "__main__":
     setup(
         name="ccml2021",
-        version="0.2.88888888",
+        version="0.2.9",
         description="ccml2021",
         long_description=open(os.path.join(module_dir, "README.md")).read(),
         url="https://github.com/kmu/ccml2021",
         author="Koki Muraoka",
         author_email="muraok_k@chemsys.t.u-tokyo.ac.jp",
         packages=find_packages(),
         zip_safe=False,
```

### Comparing `ccml2021-0.2.88888888/tests/test_gp.py` & `ccml2021-0.2.9/tests/test_gp.py`

 * *Files identical despite different names*

