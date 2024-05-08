# Comparing `tmp/guan-0.1.97.tar.gz` & `tmp/guan-0.1.98.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "guan-0.1.97.tar", last modified: Tue May  7 14:22:27 2024, max compression
+gzip compressed data, was "guan-0.1.98.tar", last modified: Wed May  8 21:21:38 2024, max compression
```

## Comparing `guan-0.1.97.tar` & `guan-0.1.98.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 14:22:27.799026 guan-0.1.97/
--rw-rw-rw-   0        0        0    35821 2021-07-19 21:39:06.000000 guan-0.1.97/LICENSE
--rw-rw-rw-   0        0        0      798 2024-05-07 14:22:27.798416 guan-0.1.97/PKG-INFO
--rw-rw-rw-   0        0        0      294 2023-11-04 17:18:16.000000 guan-0.1.97/README.md
--rw-rw-rw-   0        0        0      108 2021-05-22 13:59:00.000000 guan-0.1.97/pyproject.toml
--rw-rw-rw-   0        0        0      641 2024-05-07 14:22:27.802290 guan-0.1.97/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-07 14:22:27.636207 guan-0.1.97/src/
-drwxrwxrwx   0        0        0        0 2024-05-07 14:22:27.775401 guan-0.1.97/src/guan/
--rw-rw-rw-   0        0        0     5294 2024-02-22 19:01:32.000000 guan-0.1.97/src/guan/Fourier_transform.py
--rw-rw-rw-   0        0        0     6769 2024-05-07 14:06:47.000000 guan-0.1.97/src/guan/Green_functions.py
--rw-rw-rw-   0        0        0    24114 2024-02-22 19:01:51.000000 guan-0.1.97/src/guan/Hamiltonian_of_examples.py
--rw-rw-rw-   0        0        0      811 2024-02-22 19:43:08.000000 guan-0.1.97/src/guan/__init__.py
--rw-rw-rw-   0        0        0    10438 2024-02-22 18:58:28.000000 guan-0.1.97/src/guan/band_structures_and_wave_functions.py
--rw-rw-rw-   0        0        0     2388 2024-02-22 19:00:04.000000 guan-0.1.97/src/guan/basic_functions.py
--rw-rw-rw-   0        0        0     4809 2024-05-07 14:16:28.000000 guan-0.1.97/src/guan/data_processing.py
--rw-rw-rw-   0        0        0     1398 2024-02-22 19:14:25.000000 guan-0.1.97/src/guan/decorators.py
--rw-rw-rw-   0        0        0    10300 2024-02-22 19:01:02.000000 guan-0.1.97/src/guan/density_of_states.py
--rw-rw-rw-   0        0        0    21680 2024-02-22 19:01:14.000000 guan-0.1.97/src/guan/figure_plotting.py
--rw-rw-rw-   0        0        0    12813 2024-02-28 01:45:12.000000 guan-0.1.97/src/guan/file_reading_and_writing.py
--rw-rw-rw-   0        0        0    14014 2024-04-10 14:29:46.000000 guan-0.1.97/src/guan/machine_learning.py
--rw-rw-rw-   0        0        0    41346 2024-03-12 18:43:39.000000 guan-0.1.97/src/guan/others.py
--rw-rw-rw-   0        0        0    42564 2024-05-07 14:13:45.000000 guan-0.1.97/src/guan/quantum_transport.py
--rw-rw-rw-   0        0        0    27324 2024-02-22 19:02:31.000000 guan-0.1.97/src/guan/topological_invariant.py
-drwxrwxrwx   0        0        0        0 2024-05-07 14:22:27.794395 guan-0.1.97/src/guan.egg-info/
--rw-rw-rw-   0        0        0      798 2024-05-07 14:22:27.000000 guan-0.1.97/src/guan.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      618 2024-05-07 14:22:27.000000 guan-0.1.97/src/guan.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 14:22:27.000000 guan-0.1.97/src/guan.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-05-07 14:22:27.000000 guan-0.1.97/src/guan.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-08 21:21:38.012875 guan-0.1.98/
+-rw-rw-rw-   0        0        0    35821 2021-07-19 21:39:06.000000 guan-0.1.98/LICENSE
+-rw-rw-rw-   0        0        0      798 2024-05-08 21:21:38.012875 guan-0.1.98/PKG-INFO
+-rw-rw-rw-   0        0        0      294 2023-11-04 17:18:16.000000 guan-0.1.98/README.md
+-rw-rw-rw-   0        0        0      108 2021-05-22 13:59:00.000000 guan-0.1.98/pyproject.toml
+-rw-rw-rw-   0        0        0      641 2024-05-08 21:21:38.025410 guan-0.1.98/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-08 21:21:37.848793 guan-0.1.98/src/
+drwxrwxrwx   0        0        0        0 2024-05-08 21:21:37.992855 guan-0.1.98/src/guan/
+-rw-rw-rw-   0        0        0     5294 2024-02-22 19:01:32.000000 guan-0.1.98/src/guan/Fourier_transform.py
+-rw-rw-rw-   0        0        0     6769 2024-05-07 14:06:47.000000 guan-0.1.98/src/guan/Green_functions.py
+-rw-rw-rw-   0        0        0    24114 2024-02-22 19:01:51.000000 guan-0.1.98/src/guan/Hamiltonian_of_examples.py
+-rw-rw-rw-   0        0        0      811 2024-02-22 19:43:08.000000 guan-0.1.98/src/guan/__init__.py
+-rw-rw-rw-   0        0        0    10438 2024-02-22 18:58:28.000000 guan-0.1.98/src/guan/band_structures_and_wave_functions.py
+-rw-rw-rw-   0        0        0     2388 2024-02-22 19:00:04.000000 guan-0.1.98/src/guan/basic_functions.py
+-rw-rw-rw-   0        0        0     4809 2024-05-07 14:16:28.000000 guan-0.1.98/src/guan/data_processing.py
+-rw-rw-rw-   0        0        0     1398 2024-02-22 19:14:25.000000 guan-0.1.98/src/guan/decorators.py
+-rw-rw-rw-   0        0        0    10300 2024-02-22 19:01:02.000000 guan-0.1.98/src/guan/density_of_states.py
+-rw-rw-rw-   0        0        0    21680 2024-02-22 19:01:14.000000 guan-0.1.98/src/guan/figure_plotting.py
+-rw-rw-rw-   0        0        0    12813 2024-02-28 01:45:12.000000 guan-0.1.98/src/guan/file_reading_and_writing.py
+-rw-rw-rw-   0        0        0    14014 2024-04-10 14:29:46.000000 guan-0.1.98/src/guan/machine_learning.py
+-rw-rw-rw-   0        0        0    41346 2024-03-12 18:43:39.000000 guan-0.1.98/src/guan/others.py
+-rw-rw-rw-   0        0        0    43385 2024-05-08 21:20:46.000000 guan-0.1.98/src/guan/quantum_transport.py
+-rw-rw-rw-   0        0        0    27324 2024-02-22 19:02:31.000000 guan-0.1.98/src/guan/topological_invariant.py
+drwxrwxrwx   0        0        0        0 2024-05-08 21:21:38.012875 guan-0.1.98/src/guan.egg-info/
+-rw-rw-rw-   0        0        0      798 2024-05-08 21:21:37.000000 guan-0.1.98/src/guan.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      618 2024-05-08 21:21:37.000000 guan-0.1.98/src/guan.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 21:21:37.000000 guan-0.1.98/src/guan.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-05-08 21:21:37.000000 guan-0.1.98/src/guan.egg-info/top_level.txt
```

### Comparing `guan-0.1.97/LICENSE` & `guan-0.1.98/LICENSE`

 * *Files identical despite different names*

### Comparing `guan-0.1.97/PKG-INFO` & `guan-0.1.98/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: guan
-Version: 0.1.97
+Version: 0.1.98
 Summary: An open source python package
 Home-page: https://py.guanjihuan.com
 Author: guanjihuan
 Author-email: guanjihuan@163.com
 Project-URL: Bug Tracker, https://py.guanjihuan.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `guan-0.1.97/setup.cfg` & `guan-0.1.98/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2067 7561 6e0d 0a76 6572 7369 6f6e   = guan..version
-00000020: 203d 2030 2e31 2e39 370d 0a61 7574 686f   = 0.1.97..autho
+00000020: 203d 2030 2e31 2e39 380d 0a61 7574 686f   = 0.1.98..autho
 00000030: 7220 3d20 6775 616e 6a69 6875 616e 0d0a  r = guanjihuan..
 00000040: 6175 7468 6f72 5f65 6d61 696c 203d 2067  author_email = g
 00000050: 7561 6e6a 6968 7561 6e40 3136 332e 636f  uanjihuan@163.co
 00000060: 6d0d 0a64 6573 6372 6970 7469 6f6e 203d  m..description =
 00000070: 2041 6e20 6f70 656e 2073 6f75 7263 6520   An open source 
 00000080: 7079 7468 6f6e 2070 6163 6b61 6765 0d0a  python package..
 00000090: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
```

### Comparing `guan-0.1.97/src/guan/Fourier_transform.py` & `guan-0.1.98/src/guan/Fourier_transform.py`

 * *Files identical despite different names*

### Comparing `guan-0.1.97/src/guan/Green_functions.py` & `guan-0.1.98/src/guan/Green_functions.py`

 * *Files identical despite different names*

### Comparing `guan-0.1.97/src/guan/Hamiltonian_of_examples.py` & `guan-0.1.98/src/guan/Hamiltonian_of_examples.py`

 * *Files identical despite different names*

### Comparing `guan-0.1.97/src/guan/__init__.py` & `guan-0.1.98/src/guan/__init__.py`

 * *Files identical despite different names*

### Comparing `guan-0.1.97/src/guan/band_structures_and_wave_functions.py` & `guan-0.1.98/src/guan/band_structures_and_wave_functions.py`

 * *Files identical despite different names*

### Comparing `guan-0.1.97/src/guan/basic_functions.py` & `guan-0.1.98/src/guan/basic_functions.py`

 * *Files identical despite different names*

### Comparing `guan-0.1.97/src/guan/data_processing.py` & `guan-0.1.98/src/guan/data_processing.py`

 * *Files identical despite different names*

### Comparing `guan-0.1.97/src/guan/decorators.py` & `guan-0.1.98/src/guan/decorators.py`

 * *Files identical despite different names*

### Comparing `guan-0.1.97/src/guan/density_of_states.py` & `guan-0.1.98/src/guan/density_of_states.py`

 * *Files identical despite different names*

### Comparing `guan-0.1.97/src/guan/figure_plotting.py` & `guan-0.1.98/src/guan/figure_plotting.py`

 * *Files identical despite different names*

### Comparing `guan-0.1.97/src/guan/file_reading_and_writing.py` & `guan-0.1.98/src/guan/file_reading_and_writing.py`

 * *Files identical despite different names*

### Comparing `guan-0.1.97/src/guan/machine_learning.py` & `guan-0.1.98/src/guan/machine_learning.py`

 * *Files identical despite different names*

### Comparing `guan-0.1.97/src/guan/others.py` & `guan-0.1.98/src/guan/others.py`

 * *Files identical despite different names*

### Comparing `guan-0.1.97/src/guan/quantum_transport.py` & `guan-0.1.98/src/guan/quantum_transport.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,18 @@
             green_0n_n = guan.green_function_in_n(green_0n_n, h01, green_nn_n)
         else:
             green_nn_n = guan.green_function_nn_n(fermi_energy, h00, h01, green_nn_n, broadening=0, self_energy=right_self_energy)
             green_0n_n = guan.green_function_in_n(green_0n_n, h01, green_nn_n)
     dim = np.array(h00).shape[0]
     if dim == 1:
         conductance = np.dot(np.dot(np.dot(gamma_left, green_0n_n), gamma_right), green_0n_n.transpose().conj())
+        if conductance.shape == ():
+            pass
+        else:
+            conductance = conductance[0][0]
     else:
         conductance = np.trace(np.dot(np.dot(np.dot(gamma_left, green_0n_n), gamma_right), green_0n_n.transpose().conj()))
     return conductance
 
 # 计算不同费米能下的电导
 def calculate_conductance_with_fermi_energy_array(fermi_energy_array, h00, h01, length=100, print_show=0):
     import numpy as np
@@ -55,14 +59,18 @@
             green_nn_n = guan.green_function_nn_n(fermi_energy, h00, h01, green_nn_n, broadening=0)
             green_0n_n = guan.green_function_in_n(green_0n_n, h01, green_nn_n)
         else:
             green_nn_n = guan.green_function_nn_n(fermi_energy, h00, h01, green_nn_n, broadening=0, self_energy=right_self_energy)
             green_0n_n = guan.green_function_in_n(green_0n_n, h01, green_nn_n)
     if dim == 1:
         conductance = np.dot(np.dot(np.dot(gamma_left, green_0n_n), gamma_right), green_0n_n.transpose().conj())
+        if conductance.shape == ():
+            pass
+        else:
+            conductance = conductance[0][0]
     else:
         conductance = np.trace(np.dot(np.dot(np.dot(gamma_left, green_0n_n), gamma_right), green_0n_n.transpose().conj()))
     return conductance
 
 # 计算在无序散射下的电导
 def calculate_conductance_with_disorder(fermi_energy, h00, h01, disorder_intensity=2.0, disorder_concentration=1.0, length=100, calculation_times=1):
     import numpy as np
@@ -84,14 +92,18 @@
                 green_nn_n = guan.green_function_nn_n(fermi_energy, h00+disorder, h01, green_nn_n, broadening=0)
                 green_0n_n = guan.green_function_in_n(green_0n_n, h01, green_nn_n)
             else:
                 green_nn_n = guan.green_function_nn_n(fermi_energy, h00, h01, green_nn_n, broadening=0, self_energy=right_self_energy)
                 green_0n_n = guan.green_function_in_n(green_0n_n, h01, green_nn_n)
         if dim == 1:
             conductance = np.dot(np.dot(np.dot(gamma_left, green_0n_n), gamma_right), green_0n_n.transpose().conj())
+            if conductance.shape == ():
+                pass
+            else:
+                conductance = conductance[0][0]
         else:
             conductance = np.trace(np.dot(np.dot(np.dot(gamma_left, green_0n_n), gamma_right), green_0n_n.transpose().conj()))
         conductance_averaged += conductance
     conductance_averaged = conductance_averaged/calculation_times
     return conductance_averaged
 
 # 计算在无序散射下的电导（需要输入无序数组）
@@ -112,14 +124,18 @@
             green_nn_n = guan.green_function_nn_n(fermi_energy, h00+disorder, h01, green_nn_n, broadening=0)
             green_0n_n = guan.green_function_in_n(green_0n_n, h01, green_nn_n)
         else:
             green_nn_n = guan.green_function_nn_n(fermi_energy, h00, h01, green_nn_n, broadening=0, self_energy=right_self_energy)
             green_0n_n = guan.green_function_in_n(green_0n_n, h01, green_nn_n)
     if dim == 1:
         conductance = np.dot(np.dot(np.dot(gamma_left, green_0n_n), gamma_right), green_0n_n.transpose().conj())
+        if conductance.shape == ():
+            pass
+        else:
+            conductance = conductance[0][0]
     else:
         conductance = np.trace(np.dot(np.dot(np.dot(gamma_left, green_0n_n), gamma_right), green_0n_n.transpose().conj()))
     return conductance
 
 # 计算在无序垂直切片的散射下的电导
 def calculate_conductance_with_slice_disorder(fermi_energy, h00, h01, disorder_intensity=2.0, disorder_concentration=1.0, length=100):
     import numpy as np
@@ -138,14 +154,18 @@
             green_nn_n = guan.green_function_nn_n(fermi_energy, h00+disorder, h01, green_nn_n, broadening=0)
             green_0n_n = guan.green_function_in_n(green_0n_n, h01, green_nn_n)
         else:
             green_nn_n = guan.green_function_nn_n(fermi_energy, h00, h01, green_nn_n, broadening=0, self_energy=right_self_energy)
             green_0n_n = guan.green_function_in_n(green_0n_n, h01, green_nn_n)
     if dim == 1:
         conductance = np.dot(np.dot(np.dot(gamma_left, green_0n_n), gamma_right), green_0n_n.transpose().conj())
+        if conductance.shape == ():
+            pass
+        else:
+            conductance = conductance[0][0]
     else:
         conductance = np.trace(np.dot(np.dot(np.dot(gamma_left, green_0n_n), gamma_right), green_0n_n.transpose().conj()))
     return conductance
 
 # 计算在无序水平切片的散射下的电导
 def calculate_conductance_with_disorder_inside_unit_cell_which_keeps_translational_symmetry(fermi_energy, h00, h01, disorder_intensity=2.0, disorder_concentration=1.0, length=100):
     import numpy as np
@@ -165,14 +185,18 @@
             green_nn_n = guan.green_function_nn_n(fermi_energy, h00+disorder, h01, green_nn_n, broadening=0)
             green_0n_n = guan.green_function_in_n(green_0n_n, h01, green_nn_n)
         else:
             green_nn_n = guan.green_function_nn_n(fermi_energy, h00, h01, green_nn_n, broadening=0, self_energy=right_self_energy)
             green_0n_n = guan.green_function_in_n(green_0n_n, h01, green_nn_n)
     if dim == 1:
         conductance = np.dot(np.dot(np.dot(gamma_left, green_0n_n), gamma_right), green_0n_n.transpose().conj())
+        if conductance.shape == ():
+            pass
+        else:
+            conductance = conductance[0][0]
     else:
         conductance = np.trace(np.dot(np.dot(np.dot(gamma_left, green_0n_n), gamma_right), green_0n_n.transpose().conj()))
     return conductance
 
 # 计算在随机空位的散射下的电导
 def calculate_conductance_with_random_vacancy(fermi_energy, h00, h01, vacancy_concentration=0.5, vacancy_potential=1e9, length=100):
     import numpy as np
@@ -192,14 +216,18 @@
             green_nn_n = guan.green_function_nn_n(fermi_energy, h00+random_vacancy, h01, green_nn_n, broadening=0)
             green_0n_n = guan.green_function_in_n(green_0n_n, h01, green_nn_n)
         else:
             green_nn_n = guan.green_function_nn_n(fermi_energy, h00, h01, green_nn_n, broadening=0, self_energy=right_self_energy)
             green_0n_n = guan.green_function_in_n(green_0n_n, h01, green_nn_n)
     if dim == 1:
         conductance = np.dot(np.dot(np.dot(gamma_left, green_0n_n), gamma_right), green_0n_n.transpose().conj())
+        if conductance.shape == ():
+            pass
+        else:
+            conductance = conductance[0][0]
     else:
         conductance = np.trace(np.dot(np.dot(np.dot(gamma_left, green_0n_n), gamma_right), green_0n_n.transpose().conj()))
     return conductance
 
 # 计算在不同无序散射强度下的电导
 def calculate_conductance_with_disorder_intensity_array(fermi_energy, h00, h01, disorder_intensity_array, disorder_concentration=1.0, length=100, calculation_times=1, print_show=0):
     import numpy as np
```

### Comparing `guan-0.1.97/src/guan/topological_invariant.py` & `guan-0.1.98/src/guan/topological_invariant.py`

 * *Files identical despite different names*

### Comparing `guan-0.1.97/src/guan.egg-info/PKG-INFO` & `guan-0.1.98/src/guan.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: guan
-Version: 0.1.97
+Version: 0.1.98
 Summary: An open source python package
 Home-page: https://py.guanjihuan.com
 Author: guanjihuan
 Author-email: guanjihuan@163.com
 Project-URL: Bug Tracker, https://py.guanjihuan.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `guan-0.1.97/src/guan.egg-info/SOURCES.txt` & `guan-0.1.98/src/guan.egg-info/SOURCES.txt`

 * *Files identical despite different names*

