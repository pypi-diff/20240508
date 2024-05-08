# Comparing `tmp/imumaster-0.0.1.tar.gz` & `tmp/imumaster-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imumaster-0.0.1.tar", last modified: Fri Mar 29 01:20:00 2024, max compression
+gzip compressed data, was "imumaster-0.0.2.tar", last modified: Wed May  8 08:59:44 2024, max compression
```

## Comparing `imumaster-0.0.1.tar` & `imumaster-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-03-29 01:20:00.967101 imumaster-0.0.1/
--rw-rw-rw-   0        0        0     1091 2024-03-06 01:34:34.000000 imumaster-0.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0     2481 2024-03-29 01:20:00.964093 imumaster-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2006 2024-03-29 01:18:27.000000 imumaster-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-03-29 01:20:00.935043 imumaster-0.0.1/imumaster/
--rw-rw-rw-   0        0        0       64 2024-03-27 03:49:05.000000 imumaster-0.0.1/imumaster/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-29 01:20:00.952118 imumaster-0.0.1/imumaster/filters/
--rw-rw-rw-   0        0        0    12462 2024-03-29 01:09:51.000000 imumaster-0.0.1/imumaster/filters/EKF.py
--rw-rw-rw-   0        0        0     4321 2024-03-29 00:18:21.000000 imumaster-0.0.1/imumaster/filters/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-29 01:20:00.958346 imumaster-0.0.1/imumaster/math/
--rw-rw-rw-   0        0        0    10831 2024-03-29 00:40:05.000000 imumaster-0.0.1/imumaster/math/Quaternion.py
--rw-rw-rw-   0        0        0       36 2024-03-08 06:21:33.000000 imumaster-0.0.1/imumaster/math/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-29 01:20:00.962586 imumaster-0.0.1/imumaster.egg-info/
--rw-rw-rw-   0        0        0     2481 2024-03-29 01:20:00.000000 imumaster-0.0.1/imumaster.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      301 2024-03-29 01:20:00.000000 imumaster-0.0.1/imumaster.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-29 01:20:00.000000 imumaster-0.0.1/imumaster.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-03-29 01:20:00.000000 imumaster-0.0.1/imumaster.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      555 2024-03-29 01:19:50.000000 imumaster-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-29 01:20:00.967101 imumaster-0.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-08 08:59:44.456352 imumaster-0.0.2/
+-rw-rw-rw-   0        0        0     1091 2024-03-06 01:34:34.000000 imumaster-0.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0     2481 2024-05-08 08:59:44.454892 imumaster-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2006 2024-03-29 01:18:27.000000 imumaster-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-08 08:59:44.375384 imumaster-0.0.2/imumaster/
+-rw-rw-rw-   0        0        0       64 2024-03-27 03:49:05.000000 imumaster-0.0.2/imumaster/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 08:59:44.426691 imumaster-0.0.2/imumaster/filters/
+-rw-rw-rw-   0        0        0    12293 2024-05-07 07:34:11.000000 imumaster-0.0.2/imumaster/filters/EKF.py
+-rw-rw-rw-   0        0        0     4321 2024-03-29 00:18:21.000000 imumaster-0.0.2/imumaster/filters/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 08:59:44.449474 imumaster-0.0.2/imumaster/math/
+-rw-rw-rw-   0        0        0    10790 2024-05-07 07:34:11.000000 imumaster-0.0.2/imumaster/math/Quaternion.py
+-rw-rw-rw-   0        0        0       36 2024-03-08 06:21:33.000000 imumaster-0.0.2/imumaster/math/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 08:59:44.453431 imumaster-0.0.2/imumaster.egg-info/
+-rw-rw-rw-   0        0        0     2481 2024-05-08 08:59:44.000000 imumaster-0.0.2/imumaster.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      301 2024-05-08 08:59:44.000000 imumaster-0.0.2/imumaster.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 08:59:44.000000 imumaster-0.0.2/imumaster.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-05-08 08:59:44.000000 imumaster-0.0.2/imumaster.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      555 2024-05-07 07:34:11.000000 imumaster-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-08 08:59:44.457356 imumaster-0.0.2/setup.cfg
```

### Comparing `imumaster-0.0.1/LICENSE.txt` & `imumaster-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `imumaster-0.0.1/PKG-INFO` & `imumaster-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imumaster
-Version: 0.0.1
+Version: 0.0.2
 Summary: This package provides different sensor fusion algorithms like Extended Kalman Filter (EKF) to estimate orientation.
 Author-email: imumaster <xujunkai@imumaster.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `imumaster-0.0.1/README.md` & `imumaster-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `imumaster-0.0.1/imumaster/filters/EKF.py` & `imumaster-0.0.2/imumaster/filters/EKF.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,33 +85,32 @@
 
     """
 
     def __init__(self,
                  sample_rate: float = 200.0,
                  frame: str = 'NED',
                  **kwargs):
-        # 地面坐标系的定义：x轴指向北，y轴指向西，z轴指向天；
         self.sample_rate = sample_rate
         self.frame = frame  # Local tangent plane coordinate frame
         self.dt = kwargs.get('sample_dt', 1.0 / self.sample_rate)
 
         # Initial values of state variables
         self.x_k_minus_1 = np.array(kwargs.get('q0', [1, 0, 0, 0])).reshape(-1, 1)
         self.P_k_minus_1 = kwargs.get('P', 0.001 * np.identity(4))  # Initial state covariance
-        # Prior Estimate 先验估计
+        # Prior Estimate
         self.P_k_prior = np.identity(4)
         self.x_k_prior = np.array([1, 0, 0, 0])
-        # Posterior Estimate 后验估计
+        # Posterior Estimate
         self.x_k_posterior = np.array([1, 0, 0, 0])
         self.P_k_posterior = np.identity(4)
 
-        # Process Noise Covariance Matrix 过程噪声协方差矩阵
+        # Process Noise Covariance Matrix
         self.Q_noise = kwargs.get('Q_noise', 0.1 * np.eye(4))
 
-        # Observation Noise Covariance Matrix 观测噪声协方差矩阵
+        # Observation Noise Covariance Matrix
         self.accel_noise = kwargs.get('accel_noise', 3.8 * np.eye(3))
         self.mag_noise = kwargs.get('mag_noise', 0.5 * np.eye(3))
 
         if frame.upper() == 'NED':
             self.a_ref = np.array([0.0, 0.0, -1.0]).reshape(-1, 1)
         elif frame.upper() == 'ENU' or frame.upper() == 'NWU':
             self.a_ref = np.array([0.0, 0.0, 1.0]).reshape(-1, 1)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `imumaster-0.0.1/imumaster/filters/__init__.py` & `imumaster-0.0.2/imumaster/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `imumaster-0.0.1/imumaster/math/Quaternion.py` & `imumaster-0.0.2/imumaster/math/Quaternion.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,27 +118,27 @@
             numpy.ndarray: The inverse quaternion.
         """
         Quat = np.array([self.w, self.x, self.y, self.z])
         conjugate = np.array([self.w, -self.x, -self.y, -self.z])
         norm = np.linalg.norm(Quat)
 
         if self.scalar_first:
-            return conjugate / norm
+            return conjugate / (norm*norm)
         else:
-            return conjugate[::-1] / norm
+            return conjugate[::-1] / (norm*norm)
 
     # @property
     # def norm(self):
     #     return np.linalg.norm(np.array([self.w, self.x, self.y, self.z]))
 
     # @property
     # def normalize(self):
     #     return np.array([self.w, self.x, self.y, self.z])/np.linalg.norm(np.array([self.w, self.x, self.y, self.z]))
 
-    # 四元数乘法-Quaternion Multiplication
+    # Quaternion Multiplication
     @staticmethod
     def multiply(Q1, Q2, scalar_first=True):
         if scalar_first:
             w1, x1, y1, z1 = Q1
             w2, x2, y2, z2 = Q2
             w = w1 * w2 - x1 * x2 - y1 * y2 - z1 * z2
             x = x1 * w2 + w1 * x2 - z1 * y2 + y1 * z2
@@ -165,15 +165,15 @@
         b = b1 + b2
         c = c1 + c2
         d = d1 + d2
         add_result = np.array([a, b, c, d])
 
         return add_result
 
-    # -Quaternion Subtraction
+    # Quaternion Subtraction
     @staticmethod
     def substract(Q1, Q2):
         a1, b1, c1, d1 = Q1
         a2, b2, c2, d2 = Q2
         a = a1 - a2
         b = b1 - b2
         c = c1 - c2
@@ -195,40 +195,40 @@
         normalize_result = Quat / norm
         return normalize_result
 
     # Quaternion Conjugate
     @staticmethod
     def conjugate(Quat, scalar_first=True):
         if scalar_first:
-            # Quat[w,x,y,z] 实部在前
+            # Quat[w,x,y,z]
             w, x, y, z = np.array(Quat)
             conjugate_result = np.array([w, -x, -y, -z])
 
         else:
-            # Quat[x,y,z,w] 实部在后
+            # Quat[x,y,z,w]
             x, y, z, w = np.array(Quat)
             conjugate_result = np.array([-x, -y, -z, w])
 
         return conjugate_result
 
     # 四元数的逆-Quaternion Inverse
     @staticmethod
     def inverse(Quat, scalar_first=True):
         if scalar_first:
-            # Quat[w,x,y,z] 实部在前
+            # Quat[w,x,y,z]
             w, x, y, z = np.array(Quat)
             conjugate = np.array([w, -x, -y, -z])
             norm = np.linalg.norm(Quat)
-            inverse_result = conjugate / norm
+            inverse_result = conjugate / (norm*norm)
         else:
-            # Quat[x,y,z,w] 实部在后
+            # Quat[x,y,z,w]
             x, y, z, w = np.array(Quat)
             conjugate = np.array([-x, -y, -z, w])
             norm = np.linalg.norm(Quat)
-            inverse_result = conjugate / norm
+            inverse_result = conjugate / (norm*norm)
 
         return inverse_result
 
     @staticmethod
     def ground_to_sensor(ground_vector, Quat, scalar_first=True):
         if scalar_first:
             # Quat[w,x,y,z]
```

### Comparing `imumaster-0.0.1/imumaster.egg-info/PKG-INFO` & `imumaster-0.0.2/imumaster.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imumaster
-Version: 0.0.1
+Version: 0.0.2
 Summary: This package provides different sensor fusion algorithms like Extended Kalman Filter (EKF) to estimate orientation.
 Author-email: imumaster <xujunkai@imumaster.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `imumaster-0.0.1/pyproject.toml` & `imumaster-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "imumaster"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="imumaster", email="xujunkai@imumaster.com" },
 ]
 description = "This package provides different sensor fusion algorithms like Extended Kalman Filter (EKF) to estimate orientation."
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

