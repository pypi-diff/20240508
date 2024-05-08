# Comparing `tmp/pennylane_kq-0.0.6.tar.gz` & `tmp/pennylane-kq-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pennylane_kq-0.0.6.tar", last modified: Tue Apr 16 06:30:57 2024, max compression
+gzip compressed data, was "pennylane-kq-0.0.7.tar", last modified: Wed May  8 01:00:03 2024, max compression
```

## Comparing `pennylane_kq-0.0.6.tar` & `pennylane-kq-0.0.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 ino        (501) staff       (20)        0 2024-04-16 06:30:57.782693 pennylane_kq-0.0.6/
--rw-r--r--   0 ino        (501) staff       (20)     1335 2023-08-22 08:26:43.000000 pennylane_kq-0.0.6/LICENSE
--rw-r--r--   0 ino        (501) staff       (20)     1668 2024-04-16 06:30:57.782483 pennylane_kq-0.0.6/PKG-INFO
--rw-r--r--   0 ino        (501) staff       (20)     1304 2023-12-21 01:57:51.000000 pennylane_kq-0.0.6/README.md
-drwxr-xr-x   0 ino        (501) staff       (20)        0 2024-04-16 06:30:57.780784 pennylane_kq-0.0.6/pennylane_kq/
--rw-r--r--   0 ino        (501) staff       (20)      293 2023-12-21 00:35:30.000000 pennylane_kq-0.0.6/pennylane_kq/__init__.py
--rw-r--r--   0 ino        (501) staff       (20)       97 2024-04-16 06:29:12.000000 pennylane_kq-0.0.6/pennylane_kq/_version.py
--rw-r--r--   0 ino        (501) staff       (20)     3439 2024-04-16 06:26:52.000000 pennylane_kq-0.0.6/pennylane_kq/kq_emulator.py
--rw-r--r--   0 ino        (501) staff       (20)     3479 2023-12-27 04:57:04.000000 pennylane_kq-0.0.6/pennylane_kq/kq_emulator_aws.py
--rw-r--r--   0 ino        (501) staff       (20)     3451 2023-12-27 04:56:48.000000 pennylane_kq-0.0.6/pennylane_kq/kq_hardware.py
--rw-r--r--   0 ino        (501) staff       (20)     2435 2024-01-15 04:53:37.000000 pennylane_kq-0.0.6/pennylane_kq/kq_local_emulator.py
-drwxr-xr-x   0 ino        (501) staff       (20)        0 2024-04-16 06:30:57.782247 pennylane_kq-0.0.6/pennylane_kq.egg-info/
--rw-r--r--   0 ino        (501) staff       (20)     1668 2024-04-16 06:30:57.000000 pennylane_kq-0.0.6/pennylane_kq.egg-info/PKG-INFO
--rw-r--r--   0 ino        (501) staff       (20)      451 2024-04-16 06:30:57.000000 pennylane_kq-0.0.6/pennylane_kq.egg-info/SOURCES.txt
--rw-r--r--   0 ino        (501) staff       (20)        1 2024-04-16 06:30:57.000000 pennylane_kq-0.0.6/pennylane_kq.egg-info/dependency_links.txt
--rw-r--r--   0 ino        (501) staff       (20)      230 2024-04-16 06:30:57.000000 pennylane_kq-0.0.6/pennylane_kq.egg-info/entry_points.txt
--rw-r--r--   0 ino        (501) staff       (20)        1 2023-11-13 13:51:28.000000 pennylane_kq-0.0.6/pennylane_kq.egg-info/not-zip-safe
--rw-r--r--   0 ino        (501) staff       (20)       22 2024-04-16 06:30:57.000000 pennylane_kq-0.0.6/pennylane_kq.egg-info/requires.txt
--rw-r--r--   0 ino        (501) staff       (20)       13 2024-04-16 06:30:57.000000 pennylane_kq-0.0.6/pennylane_kq.egg-info/top_level.txt
--rw-r--r--   0 ino        (501) staff       (20)       38 2024-04-16 06:30:57.782742 pennylane_kq-0.0.6/setup.cfg
--rw-r--r--   0 ino        (501) staff       (20)     1113 2023-12-21 01:55:43.000000 pennylane_kq-0.0.6/setup.py
+drwxr-xr-x   0 ino        (501) staff       (20)        0 2024-05-08 01:00:03.172272 pennylane-kq-0.0.7/
+-rw-r--r--   0 ino        (501) staff       (20)     1335 2023-08-22 08:26:43.000000 pennylane-kq-0.0.7/LICENSE
+-rw-r--r--   0 ino        (501) staff       (20)     1636 2024-05-08 01:00:03.172151 pennylane-kq-0.0.7/PKG-INFO
+-rw-r--r--   0 ino        (501) staff       (20)     1304 2023-12-21 01:57:51.000000 pennylane-kq-0.0.7/README.md
+drwxr-xr-x   0 ino        (501) staff       (20)        0 2024-05-08 01:00:03.170864 pennylane-kq-0.0.7/pennylane_kq/
+-rw-r--r--   0 ino        (501) staff       (20)      293 2023-12-21 00:35:30.000000 pennylane-kq-0.0.7/pennylane_kq/__init__.py
+-rw-r--r--   0 ino        (501) staff       (20)       97 2024-05-08 00:52:08.000000 pennylane-kq-0.0.7/pennylane_kq/_version.py
+-rw-r--r--   0 ino        (501) staff       (20)     4621 2024-05-07 08:59:35.000000 pennylane-kq-0.0.7/pennylane_kq/kq_emulator.py
+-rw-r--r--   0 ino        (501) staff       (20)     3479 2023-12-27 04:57:04.000000 pennylane-kq-0.0.7/pennylane_kq/kq_emulator_aws.py
+-rw-r--r--   0 ino        (501) staff       (20)     3451 2023-12-27 04:56:48.000000 pennylane-kq-0.0.7/pennylane_kq/kq_hardware.py
+-rw-r--r--   0 ino        (501) staff       (20)     3541 2024-05-07 08:44:16.000000 pennylane-kq-0.0.7/pennylane_kq/kq_local_emulator.py
+drwxr-xr-x   0 ino        (501) staff       (20)        0 2024-05-08 01:00:03.171984 pennylane-kq-0.0.7/pennylane_kq.egg-info/
+-rw-r--r--   0 ino        (501) staff       (20)     1636 2024-05-08 01:00:03.000000 pennylane-kq-0.0.7/pennylane_kq.egg-info/PKG-INFO
+-rw-r--r--   0 ino        (501) staff       (20)      451 2024-05-08 01:00:03.000000 pennylane-kq-0.0.7/pennylane_kq.egg-info/SOURCES.txt
+-rw-r--r--   0 ino        (501) staff       (20)        1 2024-05-08 01:00:03.000000 pennylane-kq-0.0.7/pennylane_kq.egg-info/dependency_links.txt
+-rw-r--r--   0 ino        (501) staff       (20)      231 2024-05-08 01:00:03.000000 pennylane-kq-0.0.7/pennylane_kq.egg-info/entry_points.txt
+-rw-r--r--   0 ino        (501) staff       (20)        1 2023-11-13 13:51:28.000000 pennylane-kq-0.0.7/pennylane_kq.egg-info/not-zip-safe
+-rw-r--r--   0 ino        (501) staff       (20)       22 2024-05-08 01:00:03.000000 pennylane-kq-0.0.7/pennylane_kq.egg-info/requires.txt
+-rw-r--r--   0 ino        (501) staff       (20)       13 2024-05-08 01:00:03.000000 pennylane-kq-0.0.7/pennylane_kq.egg-info/top_level.txt
+-rw-r--r--   0 ino        (501) staff       (20)       38 2024-05-08 01:00:03.172317 pennylane-kq-0.0.7/setup.cfg
+-rw-r--r--   0 ino        (501) staff       (20)     1113 2023-12-21 01:55:43.000000 pennylane-kq-0.0.7/setup.py
```

### Comparing `pennylane_kq-0.0.6/LICENSE` & `pennylane-kq-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pennylane_kq-0.0.6/PKG-INFO` & `pennylane-kq-0.0.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: pennylane-kq
-Version: 0.0.6
+Version: 0.0.7
 Summary: A Pennylane plugin for KQ Cloud System
 Home-page: https://www.github.com/inojeon/pennylane-kq
 Author: Inho Jeon
 Author-email: inojeon@kisti.re.kr
 License: BSD-2
+Platform: UNKNOWN
 Provides: pennylane_kq
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: pennylane>=0.31
-Requires-Dist: numpy
 
 # PennyLane Korea Quantum Plugin
 
 The PennyLane-KQ plugin integrates the KQ quantum computing library.
 
 [PennyLane](https://pennylane.readthedocs.io) is a cross-platform Python library for quantum machine learning, automatic differentiation, and optimization of hybrid quantum-classical computations.
 
@@ -44,7 +43,9 @@
 
 -[**Source Code:**](https://github.com/inojeon/pennylane-kq)
 
 -[**Issue Tracker:**](https://github.com/inojeon/pennylane-kq/issues)
 
 If you are having issues, please let us know by posting the issue on our Github issue tracker, or
 by asking a question in the forum.
+
+
```

### Comparing `pennylane_kq-0.0.6/README.md` & `pennylane-kq-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `pennylane_kq-0.0.6/pennylane_kq/kq_emulator.py` & `pennylane-kq-0.0.7/pennylane_kq/kq_hardware.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,42 +2,42 @@
 A device that allows us to implement operation on a single qudit. The backend is a remote simulator.
 """
 
 import requests, json, time
 from pennylane import DeviceError, QubitDevice
 
 
-class KoreaQuantumEmulator(QubitDevice):
+class KoreaQuantumHardware(QubitDevice):
     """
     The base class for all devices that call to an external server.
     """
 
-    name = "Korea Quantum Emulator"
-    short_name = "kq.emulator"
+    name = "Korea Quantum Hardware"
+    short_name = "kq.hardware"
     pennylane_requires = ">=0.16.0"
     version = "0.0.1"
     author = "Inho Jeon"
     accessToken = None
-    resourceId = "f8284e6e-d97e-4afc-a015-39d382273a99"
+    resourceId = "18208724-e51f-4bab-b635-298ea07070b2"
 
-    operations = {"PauliX", "RX", "CNOT", "RY", "RZ", "Hadamard"}
+    operations = {"PauliX", "RX", "CNOT", "RY", "RZ"}
     observables = {"PauliZ", "PauliX", "PauliY"}
 
     def __init__(self, wires=4, shots=1024, accessKeyId=None, secretAccessKey=None):
         super().__init__(wires=wires, shots=shots)
         self.accessKeyId = accessKeyId
         self.secretAccessKey = secretAccessKey
-        # self.hardware_options = hardware_options or "kqEmulator"
+        # self.hardware_options = hardware_options or "kqHardware"
 
     def apply(self, operations, **kwargs):
         self.run(self._circuit)
 
     def _get_token(self):
         print("get KQ Cloud Token")
-        api_url = f"http://150.183.154.20/oauth/token"
+        api_url = f"http://150.183.154.20:31001/oauth/token"
         headers = {"Content-Type": "application/x-www-form-urlencoded"}
         data = {
             "grant_type": "apikey",
             "accessKeyId": self.accessKeyId,
             "secretAccessKey": self.secretAccessKey,
         }
         requestData = requests.post(api_url, data=data, headers=headers)
@@ -48,22 +48,22 @@
         else:
             raise DeviceError(
                 f"/oauth/token error. req code : {requestData.status_code}"
             )
 
     def _job_submit(self, circuits):
         print("job submit")
-        URL = "http://150.183.154.20/v2/jobs"
+        URL = "http://150.183.154.20:31001/v2/jobs"
         headers = {
             "Content-Type": "application/json",
             "Authorization": f"Bearer {self.accessToken}",
         }
         data = {
             "resource": {"id": self.resourceId},
-            "code": circuits[0].to_openqasm(wires=sorted(circuits[0].wires)),
+            "input_file": circuits[0].to_openqasm(wires=sorted(circuits[0].wires)),
             "shot": self.shots,
             "name": "test job",
             "type": "QASM",
         }
         res = requests.post(URL, data=json.dumps(data), headers=headers)
 
         if res.status_code == 201:
@@ -72,15 +72,15 @@
             raise DeviceError(f"Job sumbit error. req code : {res.status_code}")
 
     def _check_job_status(self, jobId):
         timeout = 6000
         timeout_start = time.time()
 
         while time.time() < timeout_start + timeout:
-            URL = f"http://150.183.154.20/v2/jobs/{jobId}"
+            URL = f"http://150.183.154.20:31001/v2/jobs/{jobId}"
             headers = {"Authorization": f"Bearer {self.accessToken}"}
             res = requests.get(URL, headers=headers)
             status = res.json().get("status")
             print(f"job status check: {status}")
 
             if status == "COMPLETED":
                 return res.json().get("result")
```

### Comparing `pennylane_kq-0.0.6/pennylane_kq/kq_emulator_aws.py` & `pennylane-kq-0.0.7/pennylane_kq/kq_emulator_aws.py`

 * *Files identical despite different names*

### Comparing `pennylane_kq-0.0.6/pennylane_kq/kq_hardware.py` & `pennylane-kq-0.0.7/pennylane_kq/kq_local_emulator.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,100 +1,103 @@
 """
 A device that allows us to implement operation on a single qudit. The backend is a remote simulator.
 """
 
+# import numpy as np
+
 import requests, json, time
 from pennylane import DeviceError, QubitDevice
 
 
-class KoreaQuantumHardware(QubitDevice):
+class KoreaQuantumLocalEmulator(QubitDevice):
     """
     The base class for all devices that call to an external server.
     """
 
-    name = "Korea Quantum Hardware"
-    short_name = "kq.hardware"
+    name = "Korea Quantum Local Emulator"
+    short_name = "kq.local_emulator"
     pennylane_requires = ">=0.16.0"
     version = "0.0.1"
     author = "Inho Jeon"
-    accessToken = None
-    resourceId = "18208724-e51f-4bab-b635-298ea07070b2"
 
-    operations = {"PauliX", "RX", "CNOT", "RY", "RZ"}
+    operations = {"PauliX", "RX", "CNOT", "RY", "RZ", "Hadamard"}
     observables = {"PauliZ", "PauliX", "PauliY"}
 
-    def __init__(self, wires=4, shots=1024, accessKeyId=None, secretAccessKey=None):
+    def __init__(self, wires=4, shots=1024):
         super().__init__(wires=wires, shots=shots)
-        self.accessKeyId = accessKeyId
-        self.secretAccessKey = secretAccessKey
-        # self.hardware_options = hardware_options or "kqHardware"
 
     def apply(self, operations, **kwargs):
-        self.run(self._circuit)
-
-    def _get_token(self):
-        print("get KQ Cloud Token")
-        api_url = f"http://150.183.154.20:31001/oauth/token"
-        headers = {"Content-Type": "application/x-www-form-urlencoded"}
-        data = {
-            "grant_type": "apikey",
-            "accessKeyId": self.accessKeyId,
-            "secretAccessKey": self.secretAccessKey,
-        }
-        requestData = requests.post(api_url, data=data, headers=headers)
-        if requestData.status_code == 200:
-            jsondata = requestData.json()
-            self.accessToken = jsondata.get("accessToken")
-            return True
-        else:
-            raise DeviceError(
-                f"/oauth/token error. req code : {requestData.status_code}"
-            )
+        print("apply")
+        # self.run(self._circuit)
 
     def _job_submit(self, circuits):
-        print("job submit")
-        URL = "http://150.183.154.20:31001/v2/jobs"
-        headers = {
-            "Content-Type": "application/json",
-            "Authorization": f"Bearer {self.accessToken}",
-        }
+        # print(circuits[0].wires)
+        # print(circuits[0].to_openqasm(wires=sorted(circuits[0].wires)))
+        URL = "http://localhost:8000/job"
+        headers = {"Content-Type": "application/json"}
         data = {
-            "resource": {"id": self.resourceId},
             "input_file": circuits[0].to_openqasm(wires=sorted(circuits[0].wires)),
             "shot": self.shots,
-            "name": "test job",
-            "type": "QASM",
+            "type": "qasm",
         }
         res = requests.post(URL, data=json.dumps(data), headers=headers)
 
         if res.status_code == 201:
-            return res.json().get("id")
+            return res.json().get("jobUUID")
         else:
-            raise DeviceError(f"Job sumbit error. req code : {res.status_code}")
+            raise DeviceError(
+                f"Job sumbit error. post /job/ req code : {res.status_code}"
+            )
 
-    def _check_job_status(self, jobId):
+    def _check_job_status(self, jobUUID):
         timeout = 6000
         timeout_start = time.time()
 
         while time.time() < timeout_start + timeout:
-            URL = f"http://150.183.154.20:31001/v2/jobs/{jobId}"
-            headers = {"Authorization": f"Bearer {self.accessToken}"}
-            res = requests.get(URL, headers=headers)
-            status = res.json().get("status")
-            print(f"job status check: {status}")
-
-            if status == "COMPLETED":
-                return res.json().get("result")
+            URL = f"http://localhost:8000/job/{jobUUID}/status"
+            res = requests.get(URL)
             time.sleep(1)
-        raise DeviceError("Job timeout")
+            if res.json().get("status") == "SUCCESS":
+                URL = f"http://localhost:8000/job/{jobUUID}/result"
+                res = requests.get(URL)
+                return res.json()
+
+    def _convert_counts_to_samples(self, count_datas, wires):
+        import numpy as np
+
+        first = True
+        result = None
+
+        for hex_value, count in count_datas.items():
+            # 16진수 값을 10진수로 변환
+            decimal_value = int(hex_value, 16)
+
+            if decimal_value >= 2**wires:
+                decimal_value = 2**wires - 1
+            # 10진수 값을 지정된 자릿수의 이진수 배열로 변환
+            binary_array = np.array([int(x) for x in f"{decimal_value:0{wires}b}"])
+            # 지정된 횟수만큼 배열을 반복하여 결과 리스트에 추가
+            expanded_array = np.tile(binary_array, (count, 1))
+            # 첫 번째 배열인 경우 result를 초기화
+            if first:
+                result = expanded_array
+                first = False
+            else:
+                result = np.vstack((result, expanded_array))
+        return result
+
+    def batch_execute(self, circuits):
+        jobUUID = self._job_submit(circuits)
+        res_results = self._check_job_status(jobUUID)
+
+        results = []
+        for circuit, res_result in zip(circuits, res_results["results"]):
+            self._samples = self._convert_counts_to_samples(
+                res_result["data"]["counts"], circuit.num_wires
+            )
+
+            res = self.statistics(circuit)
+            single_measurement = len(circuit.measurements) == 1
+            res = res[0] if single_measurement else tuple(res)
+            results.append(res)
 
-    def batch_execute(
-        self, circuits
-    ):  # pragma: no cover, pylint:disable=arguments-differ
-        # print(self.accessKeyId, self.secretAccessKey)
-        if not self.accessToken:
-            self._get_token()
-
-        jobId = self._job_submit(circuits)
-        result = self._check_job_status(jobId)
-        # print(jobId)
-        return [result]
+        return results
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pennylane_kq-0.0.6/pennylane_kq.egg-info/PKG-INFO` & `pennylane-kq-0.0.7/pennylane_kq.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: pennylane-kq
-Version: 0.0.6
+Version: 0.0.7
 Summary: A Pennylane plugin for KQ Cloud System
 Home-page: https://www.github.com/inojeon/pennylane-kq
 Author: Inho Jeon
 Author-email: inojeon@kisti.re.kr
 License: BSD-2
+Platform: UNKNOWN
 Provides: pennylane_kq
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: pennylane>=0.31
-Requires-Dist: numpy
 
 # PennyLane Korea Quantum Plugin
 
 The PennyLane-KQ plugin integrates the KQ quantum computing library.
 
 [PennyLane](https://pennylane.readthedocs.io) is a cross-platform Python library for quantum machine learning, automatic differentiation, and optimization of hybrid quantum-classical computations.
 
@@ -44,7 +43,9 @@
 
 -[**Source Code:**](https://github.com/inojeon/pennylane-kq)
 
 -[**Issue Tracker:**](https://github.com/inojeon/pennylane-kq/issues)
 
 If you are having issues, please let us know by posting the issue on our Github issue tracker, or
 by asking a question in the forum.
+
+
```

### Comparing `pennylane_kq-0.0.6/setup.py` & `pennylane-kq-0.0.7/setup.py`

 * *Files identical despite different names*

