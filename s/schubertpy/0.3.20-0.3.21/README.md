# Comparing `tmp/schubertpy-0.3.20.tar.gz` & `tmp/schubertpy-0.3.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "schubertpy-0.3.20.tar", last modified: Wed May  8 13:57:08 2024, max compression
+gzip compressed data, was "schubertpy-0.3.21.tar", last modified: Wed May  8 14:02:21 2024, max compression
```

## Comparing `schubertpy-0.3.20.tar` & `schubertpy-0.3.21.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 tranduythanh   (501) staff       (20)        0 2024-05-08 13:57:08.702054 schubertpy-0.3.20/
--rw-r--r--   0 tranduythanh   (501) staff       (20)    35147 2024-04-29 08:09:23.000000 schubertpy-0.3.20/LICENSE
--rw-r--r--   0 tranduythanh   (501) staff       (20)     7415 2024-05-08 13:57:08.701969 schubertpy-0.3.20/PKG-INFO
--rw-r--r--   0 tranduythanh   (501) staff       (20)     6874 2024-05-08 09:10:44.000000 schubertpy-0.3.20/README.md
-drwxr-xr-x   0 tranduythanh   (501) staff       (20)        0 2024-05-08 13:57:08.699995 schubertpy-0.3.20/schubertpy/
--rw-r--r--   0 tranduythanh   (501) staff       (20)      377 2024-02-13 13:37:36.000000 schubertpy-0.3.20/schubertpy/__init__.py
--rw-r--r--   0 tranduythanh   (501) staff       (20)     6220 2024-04-26 02:35:10.000000 schubertpy-0.3.20/schubertpy/abstract_grassmannian.py
--rw-r--r--   0 tranduythanh   (501) staff       (20)      175 2024-05-06 06:28:22.000000 schubertpy-0.3.20/schubertpy/const.py
--rw-r--r--   0 tranduythanh   (501) staff       (20)      942 2024-02-13 13:40:38.000000 schubertpy-0.3.20/schubertpy/csv_bijection.py
--rw-r--r--   0 tranduythanh   (501) staff       (20)     4806 2024-02-13 13:40:53.000000 schubertpy-0.3.20/schubertpy/grassmannian.py
--rw-r--r--   0 tranduythanh   (501) staff       (20)     4714 2024-02-13 13:40:49.000000 schubertpy-0.3.20/schubertpy/isotropic_grassmannian.py
--rw-r--r--   0 tranduythanh   (501) staff       (20)     9213 2024-05-06 06:50:44.000000 schubertpy-0.3.20/schubertpy/lc.py
--rw-r--r--   0 tranduythanh   (501) staff       (20)    12445 2024-02-13 13:41:11.000000 schubertpy-0.3.20/schubertpy/orthogonal_grassmannian.py
--rw-r--r--   0 tranduythanh   (501) staff       (20)     3059 2024-02-13 13:42:18.000000 schubertpy-0.3.20/schubertpy/partition.py
--rw-r--r--   0 tranduythanh   (501) staff       (20)    40455 2024-04-27 02:11:49.000000 schubertpy-0.3.20/schubertpy/qcalc.py
--rw-r--r--   0 tranduythanh   (501) staff       (20)     3239 2024-05-06 06:20:18.000000 schubertpy-0.3.20/schubertpy/schur.py
--rw-r--r--   0 tranduythanh   (501) staff       (20)      203 2024-02-13 13:41:38.000000 schubertpy-0.3.20/schubertpy/util.py
-drwxr-xr-x   0 tranduythanh   (501) staff       (20)        0 2024-05-08 13:57:08.701610 schubertpy-0.3.20/schubertpy.egg-info/
--rw-r--r--   0 tranduythanh   (501) staff       (20)     7415 2024-05-08 13:57:08.000000 schubertpy-0.3.20/schubertpy.egg-info/PKG-INFO
--rw-r--r--   0 tranduythanh   (501) staff       (20)      566 2024-05-08 13:57:08.000000 schubertpy-0.3.20/schubertpy.egg-info/SOURCES.txt
--rw-r--r--   0 tranduythanh   (501) staff       (20)        1 2024-05-08 13:57:08.000000 schubertpy-0.3.20/schubertpy.egg-info/dependency_links.txt
--rw-r--r--   0 tranduythanh   (501) staff       (20)       28 2024-05-08 13:57:08.000000 schubertpy-0.3.20/schubertpy.egg-info/requires.txt
--rw-r--r--   0 tranduythanh   (501) staff       (20)       24 2024-05-08 13:57:08.000000 schubertpy-0.3.20/schubertpy.egg-info/top_level.txt
-drwxr-xr-x   0 tranduythanh   (501) staff       (20)        0 2024-05-08 13:57:08.701305 schubertpy-0.3.20/schubertsage/
--rw-r--r--   0 tranduythanh   (501) staff       (20)      304 2024-02-14 06:03:50.000000 schubertpy-0.3.20/schubertsage/__init__.py
--rw-r--r--   0 tranduythanh   (501) staff       (20)      793 2024-02-14 06:36:52.000000 schubertpy-0.3.20/schubertsage/conversion.py
--rw-r--r--   0 tranduythanh   (501) staff       (20)      132 2024-05-08 13:57:08.702346 schubertpy-0.3.20/setup.cfg
--rw-r--r--   0 tranduythanh   (501) staff       (20)     2038 2024-05-08 13:57:08.000000 schubertpy-0.3.20/setup.py
+drwxr-xr-x   0 tranduythanh   (501) staff       (20)        0 2024-05-08 14:02:21.976234 schubertpy-0.3.21/
+-rw-r--r--   0 tranduythanh   (501) staff       (20)    35147 2024-04-29 08:09:23.000000 schubertpy-0.3.21/LICENSE
+-rw-r--r--   0 tranduythanh   (501) staff       (20)     7432 2024-05-08 14:02:21.976127 schubertpy-0.3.21/PKG-INFO
+-rw-r--r--   0 tranduythanh   (501) staff       (20)     6891 2024-05-08 13:57:52.000000 schubertpy-0.3.21/README.md
+drwxr-xr-x   0 tranduythanh   (501) staff       (20)        0 2024-05-08 14:02:21.973930 schubertpy-0.3.21/schubertpy/
+-rw-r--r--   0 tranduythanh   (501) staff       (20)      377 2024-02-13 13:37:36.000000 schubertpy-0.3.21/schubertpy/__init__.py
+-rw-r--r--   0 tranduythanh   (501) staff       (20)     6220 2024-04-26 02:35:10.000000 schubertpy-0.3.21/schubertpy/abstract_grassmannian.py
+-rw-r--r--   0 tranduythanh   (501) staff       (20)      175 2024-05-06 06:28:22.000000 schubertpy-0.3.21/schubertpy/const.py
+-rw-r--r--   0 tranduythanh   (501) staff       (20)      942 2024-02-13 13:40:38.000000 schubertpy-0.3.21/schubertpy/csv_bijection.py
+-rw-r--r--   0 tranduythanh   (501) staff       (20)     4806 2024-02-13 13:40:53.000000 schubertpy-0.3.21/schubertpy/grassmannian.py
+-rw-r--r--   0 tranduythanh   (501) staff       (20)     4714 2024-02-13 13:40:49.000000 schubertpy-0.3.21/schubertpy/isotropic_grassmannian.py
+-rw-r--r--   0 tranduythanh   (501) staff       (20)     9213 2024-05-06 06:50:44.000000 schubertpy-0.3.21/schubertpy/lc.py
+-rw-r--r--   0 tranduythanh   (501) staff       (20)    12445 2024-02-13 13:41:11.000000 schubertpy-0.3.21/schubertpy/orthogonal_grassmannian.py
+-rw-r--r--   0 tranduythanh   (501) staff       (20)     3059 2024-02-13 13:42:18.000000 schubertpy-0.3.21/schubertpy/partition.py
+-rw-r--r--   0 tranduythanh   (501) staff       (20)    40455 2024-04-27 02:11:49.000000 schubertpy-0.3.21/schubertpy/qcalc.py
+-rw-r--r--   0 tranduythanh   (501) staff       (20)     3239 2024-05-06 06:20:18.000000 schubertpy-0.3.21/schubertpy/schur.py
+-rw-r--r--   0 tranduythanh   (501) staff       (20)      203 2024-02-13 13:41:38.000000 schubertpy-0.3.21/schubertpy/util.py
+drwxr-xr-x   0 tranduythanh   (501) staff       (20)        0 2024-05-08 14:02:21.975734 schubertpy-0.3.21/schubertpy.egg-info/
+-rw-r--r--   0 tranduythanh   (501) staff       (20)     7432 2024-05-08 14:02:21.000000 schubertpy-0.3.21/schubertpy.egg-info/PKG-INFO
+-rw-r--r--   0 tranduythanh   (501) staff       (20)      566 2024-05-08 14:02:21.000000 schubertpy-0.3.21/schubertpy.egg-info/SOURCES.txt
+-rw-r--r--   0 tranduythanh   (501) staff       (20)        1 2024-05-08 14:02:21.000000 schubertpy-0.3.21/schubertpy.egg-info/dependency_links.txt
+-rw-r--r--   0 tranduythanh   (501) staff       (20)       28 2024-05-08 14:02:21.000000 schubertpy-0.3.21/schubertpy.egg-info/requires.txt
+-rw-r--r--   0 tranduythanh   (501) staff       (20)       24 2024-05-08 14:02:21.000000 schubertpy-0.3.21/schubertpy.egg-info/top_level.txt
+drwxr-xr-x   0 tranduythanh   (501) staff       (20)        0 2024-05-08 14:02:21.975394 schubertpy-0.3.21/schubertsage/
+-rw-r--r--   0 tranduythanh   (501) staff       (20)      304 2024-02-14 06:03:50.000000 schubertpy-0.3.21/schubertsage/__init__.py
+-rw-r--r--   0 tranduythanh   (501) staff       (20)      793 2024-02-14 06:36:52.000000 schubertpy-0.3.21/schubertsage/conversion.py
+-rw-r--r--   0 tranduythanh   (501) staff       (20)      132 2024-05-08 14:02:21.976608 schubertpy-0.3.21/setup.cfg
+-rw-r--r--   0 tranduythanh   (501) staff       (20)     2038 2024-05-08 14:02:21.000000 schubertpy-0.3.21/setup.py
```

### Comparing `schubertpy-0.3.20/LICENSE` & `schubertpy-0.3.21/LICENSE`

 * *Files identical despite different names*

### Comparing `schubertpy-0.3.20/PKG-INFO` & `schubertpy-0.3.21/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schubertpy
-Version: 0.3.20
+Version: 0.3.21
 Summary: This Python module facilitates operations such as quantum Pieri rules, quantum Giambelli formulae, action and multiplication of Schubert classes, and conversion between different representations of Schubert classes
 Home-page: https://github.com/tranduythanh/schubertpy
 Author: Trần Duy Thanh
 Author-email: fbtranduythanh@gmail.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -137,29 +137,29 @@
 Or directly with Python:
 
 ```bash
 python3 -m unittest schubertpy/testcases/*.py
 ```
 
 ## Authors
-- **Đặng Tuấn Hiệp** 🇻🇳
+- **Dang Tuan Hiep** 🇻🇳
   - <img width="100" alt="Screenshot 2024-05-08 at 15 58 33" src="https://github.com/tranduythanh/schubertpy/assets/6112723/3e2bc594-e192-4450-b624-c4b18ff2be84">
-  - Email: hiepdt@dlu.edu.vn
+  - Email: hiepdt@dlu.edu.vn (Đặng Tuấn Hiệp)
   
 - **Trần Duy Thanh** 🇻🇳
-  - <img width="100" alt="Screenshot 2024-05-08 at 15 58 33" src="https://github.com/tranduythanh/schubertpy/assets/6112723/8c141d45-4c45-4545-99cd-35d5bafbeeb2">
+  - <img width="100" alt="Screenshot 2024-05-08 at 16 56 22" src="https://github.com/tranduythanh/schubertpy/assets/6112723/f3abca71-6bb5-44f6-b090-9ce206bdd5ad">
   - Email: coachtranduythanh@gmail.com
   - Email: 2015830@dlu.edu.vn
 
-- **Nguyễn Minh Đức** 🇻🇳
-  - <img width="100" alt="Screenshot 2024-05-08 at 15 58 33" src="https://github.com/tranduythanh/schubertpy/assets/6112723/c35985a6-5329-4a67-bdf3-f3a11762641e">
+- **Hoàng Minh Đức** 🇻🇳
+  - <img width="100" alt="Screenshot 2024-05-08 at 16 49 14" src="https://github.com/tranduythanh/schubertpy/assets/6112723/595e2bd1-33e0-42cd-8fc3-ee889c994664">  
   - Email: 2113423@dlu.edu.vn
 
 - **Nguyễn Trương Thiên Ân** 🇻🇳
-  - <img width="100" alt="Screenshot 2024-05-08 at 15 58 33" src="https://github.com/tranduythanh/schubertpy/assets/6112723/827e6a24-22e5-4ffd-b6cc-b841f8c685c4">
+  - <img width="100" alt="Screenshot 2024-05-08 at 16 50 21" src="https://github.com/tranduythanh/schubertpy/assets/6112723/a8b695fa-48fd-42d5-831d-fc58bb26dd45">
   - Email: 2113421@dlu.edu.vn
 
 ## Contributing
 
 We highly encourage contributions to `schubertpy`. Whether you are looking to expand functionality, enhance performance, or fix bugs, your input is valuable. To get started:
 
 - **Report Issues**: If you encounter issues or have suggestions, please report them by creating an issue on our GitHub page.
```

### Comparing `schubertpy-0.3.20/README.md` & `schubertpy-0.3.21/schubertpy.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: schubertpy
+Version: 0.3.21
+Summary: This Python module facilitates operations such as quantum Pieri rules, quantum Giambelli formulae, action and multiplication of Schubert classes, and conversion between different representations of Schubert classes
+Home-page: https://github.com/tranduythanh/schubertpy
+Author: Trần Duy Thanh
+Author-email: fbtranduythanh@gmail.com
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: numpy>=1.24.3
+Requires-Dist: sympy>=1.11.1
+
 # schubertpy
 
 ## Overview
 
 `schubertpy` is a powerful Python package designed for performing advanced mathematical operations on the Grassmannian, a key concept in algebraic geometry and representation theory. This module facilitates operations such as quantum Pieri rules, quantum Giambelli formulae, and the manipulation of Schubert classes. It is a Python implementation based on the comprehensive maple library available at [https://sites.math.rutgers.edu/~asbuch/qcalc/](https://sites.math.rutgers.edu/~asbuch/qcalc/).
 
 References:
@@ -124,29 +137,29 @@
 Or directly with Python:
 
 ```bash
 python3 -m unittest schubertpy/testcases/*.py
 ```
 
 ## Authors
-- **Đặng Tuấn Hiệp** 🇻🇳
+- **Dang Tuan Hiep** 🇻🇳
   - <img width="100" alt="Screenshot 2024-05-08 at 15 58 33" src="https://github.com/tranduythanh/schubertpy/assets/6112723/3e2bc594-e192-4450-b624-c4b18ff2be84">
-  - Email: hiepdt@dlu.edu.vn
+  - Email: hiepdt@dlu.edu.vn (Đặng Tuấn Hiệp)
   
 - **Trần Duy Thanh** 🇻🇳
-  - <img width="100" alt="Screenshot 2024-05-08 at 15 58 33" src="https://github.com/tranduythanh/schubertpy/assets/6112723/8c141d45-4c45-4545-99cd-35d5bafbeeb2">
+  - <img width="100" alt="Screenshot 2024-05-08 at 16 56 22" src="https://github.com/tranduythanh/schubertpy/assets/6112723/f3abca71-6bb5-44f6-b090-9ce206bdd5ad">
   - Email: coachtranduythanh@gmail.com
   - Email: 2015830@dlu.edu.vn
 
-- **Nguyễn Minh Đức** 🇻🇳
-  - <img width="100" alt="Screenshot 2024-05-08 at 15 58 33" src="https://github.com/tranduythanh/schubertpy/assets/6112723/c35985a6-5329-4a67-bdf3-f3a11762641e">
+- **Hoàng Minh Đức** 🇻🇳
+  - <img width="100" alt="Screenshot 2024-05-08 at 16 49 14" src="https://github.com/tranduythanh/schubertpy/assets/6112723/595e2bd1-33e0-42cd-8fc3-ee889c994664">  
   - Email: 2113423@dlu.edu.vn
 
 - **Nguyễn Trương Thiên Ân** 🇻🇳
-  - <img width="100" alt="Screenshot 2024-05-08 at 15 58 33" src="https://github.com/tranduythanh/schubertpy/assets/6112723/827e6a24-22e5-4ffd-b6cc-b841f8c685c4">
+  - <img width="100" alt="Screenshot 2024-05-08 at 16 50 21" src="https://github.com/tranduythanh/schubertpy/assets/6112723/a8b695fa-48fd-42d5-831d-fc58bb26dd45">
   - Email: 2113421@dlu.edu.vn
 
 ## Contributing
 
 We highly encourage contributions to `schubertpy`. Whether you are looking to expand functionality, enhance performance, or fix bugs, your input is valuable. To get started:
 
 - **Report Issues**: If you encounter issues or have suggestions, please report them by creating an issue on our GitHub page.
```

### Comparing `schubertpy-0.3.20/schubertpy/abstract_grassmannian.py` & `schubertpy-0.3.21/schubertpy/abstract_grassmannian.py`

 * *Files identical despite different names*

### Comparing `schubertpy-0.3.20/schubertpy/csv_bijection.py` & `schubertpy-0.3.21/schubertpy/csv_bijection.py`

 * *Files identical despite different names*

### Comparing `schubertpy-0.3.20/schubertpy/grassmannian.py` & `schubertpy-0.3.21/schubertpy/grassmannian.py`

 * *Files identical despite different names*

### Comparing `schubertpy-0.3.20/schubertpy/isotropic_grassmannian.py` & `schubertpy-0.3.21/schubertpy/isotropic_grassmannian.py`

 * *Files identical despite different names*

### Comparing `schubertpy-0.3.20/schubertpy/lc.py` & `schubertpy-0.3.21/schubertpy/lc.py`

 * *Files identical despite different names*

### Comparing `schubertpy-0.3.20/schubertpy/orthogonal_grassmannian.py` & `schubertpy-0.3.21/schubertpy/orthogonal_grassmannian.py`

 * *Files identical despite different names*

### Comparing `schubertpy-0.3.20/schubertpy/partition.py` & `schubertpy-0.3.21/schubertpy/partition.py`

 * *Files identical despite different names*

### Comparing `schubertpy-0.3.20/schubertpy/qcalc.py` & `schubertpy-0.3.21/schubertpy/qcalc.py`

 * *Files identical despite different names*

### Comparing `schubertpy-0.3.20/schubertpy/schur.py` & `schubertpy-0.3.21/schubertpy/schur.py`

 * *Files identical despite different names*

### Comparing `schubertpy-0.3.20/schubertpy.egg-info/PKG-INFO` & `schubertpy-0.3.21/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: schubertpy
-Version: 0.3.20
-Summary: This Python module facilitates operations such as quantum Pieri rules, quantum Giambelli formulae, action and multiplication of Schubert classes, and conversion between different representations of Schubert classes
-Home-page: https://github.com/tranduythanh/schubertpy
-Author: Trần Duy Thanh
-Author-email: fbtranduythanh@gmail.com
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: numpy>=1.24.3
-Requires-Dist: sympy>=1.11.1
-
 # schubertpy
 
 ## Overview
 
 `schubertpy` is a powerful Python package designed for performing advanced mathematical operations on the Grassmannian, a key concept in algebraic geometry and representation theory. This module facilitates operations such as quantum Pieri rules, quantum Giambelli formulae, and the manipulation of Schubert classes. It is a Python implementation based on the comprehensive maple library available at [https://sites.math.rutgers.edu/~asbuch/qcalc/](https://sites.math.rutgers.edu/~asbuch/qcalc/).
 
 References:
@@ -137,29 +124,29 @@
 Or directly with Python:
 
 ```bash
 python3 -m unittest schubertpy/testcases/*.py
 ```
 
 ## Authors
-- **Đặng Tuấn Hiệp** 🇻🇳
+- **Dang Tuan Hiep** 🇻🇳
   - <img width="100" alt="Screenshot 2024-05-08 at 15 58 33" src="https://github.com/tranduythanh/schubertpy/assets/6112723/3e2bc594-e192-4450-b624-c4b18ff2be84">
-  - Email: hiepdt@dlu.edu.vn
+  - Email: hiepdt@dlu.edu.vn (Đặng Tuấn Hiệp)
   
 - **Trần Duy Thanh** 🇻🇳
-  - <img width="100" alt="Screenshot 2024-05-08 at 15 58 33" src="https://github.com/tranduythanh/schubertpy/assets/6112723/8c141d45-4c45-4545-99cd-35d5bafbeeb2">
+  - <img width="100" alt="Screenshot 2024-05-08 at 16 56 22" src="https://github.com/tranduythanh/schubertpy/assets/6112723/f3abca71-6bb5-44f6-b090-9ce206bdd5ad">
   - Email: coachtranduythanh@gmail.com
   - Email: 2015830@dlu.edu.vn
 
-- **Nguyễn Minh Đức** 🇻🇳
-  - <img width="100" alt="Screenshot 2024-05-08 at 15 58 33" src="https://github.com/tranduythanh/schubertpy/assets/6112723/c35985a6-5329-4a67-bdf3-f3a11762641e">
+- **Hoàng Minh Đức** 🇻🇳
+  - <img width="100" alt="Screenshot 2024-05-08 at 16 49 14" src="https://github.com/tranduythanh/schubertpy/assets/6112723/595e2bd1-33e0-42cd-8fc3-ee889c994664">  
   - Email: 2113423@dlu.edu.vn
 
 - **Nguyễn Trương Thiên Ân** 🇻🇳
-  - <img width="100" alt="Screenshot 2024-05-08 at 15 58 33" src="https://github.com/tranduythanh/schubertpy/assets/6112723/827e6a24-22e5-4ffd-b6cc-b841f8c685c4">
+  - <img width="100" alt="Screenshot 2024-05-08 at 16 50 21" src="https://github.com/tranduythanh/schubertpy/assets/6112723/a8b695fa-48fd-42d5-831d-fc58bb26dd45">
   - Email: 2113421@dlu.edu.vn
 
 ## Contributing
 
 We highly encourage contributions to `schubertpy`. Whether you are looking to expand functionality, enhance performance, or fix bugs, your input is valuable. To get started:
 
 - **Report Issues**: If you encounter issues or have suggestions, please report them by creating an issue on our GitHub page.
```

### Comparing `schubertpy-0.3.20/schubertpy.egg-info/SOURCES.txt` & `schubertpy-0.3.21/schubertpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `schubertpy-0.3.20/schubertsage/conversion.py` & `schubertpy-0.3.21/schubertsage/conversion.py`

 * *Files identical despite different names*

### Comparing `schubertpy-0.3.20/setup.py` & `schubertpy-0.3.21/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 # Read the contents of your README file
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 # Define package metadata
 package_name = 'schubertpy'
-package_version = '0.3.20'
+package_version = '0.3.21'
 package_author = 'Trần Duy Thanh'
 package_author_email = 'fbtranduythanh@gmail.com'
 package_url = 'https://github.com/tranduythanh/schubertpy'
 package_description = 'This Python module facilitates operations such as quantum Pieri rules, quantum Giambelli formulae, action and multiplication of Schubert classes, and conversion between different representations of Schubert classes'
 package_license = 'GNU General Public License'
 
 # Generate CITATION.cff content
```

