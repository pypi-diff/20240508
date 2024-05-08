# Comparing `tmp/pygazpar-1.3.0a6.tar.gz` & `tmp/pygazpar-1.3.0a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygazpar-1.3.0a6.tar", last modified: Sat May  4 15:16:22 2024, max compression
+gzip compressed data, was "pygazpar-1.3.0a9.tar", last modified: Wed May  8 11:12:14 2024, max compression
```

## Comparing `pygazpar-1.3.0a6.tar` & `pygazpar-1.3.0a9.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 15:16:22.928136 pygazpar-1.3.0a6/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-04 15:14:22.000000 pygazpar-1.3.0a6/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-04 15:14:22.000000 pygazpar-1.3.0a6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    20961 2024-05-04 15:16:22.928136 pygazpar-1.3.0a6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4846 2024-05-04 15:14:22.000000 pygazpar-1.3.0a6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 15:16:22.928136 pygazpar-1.3.0a6/pygazpar/
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-04 15:14:22.000000 pygazpar-1.3.0a6/pygazpar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3177 2024-05-04 15:14:22.000000 pygazpar-1.3.0a6/pygazpar/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-05-04 15:14:22.000000 pygazpar-1.3.0a6/pygazpar/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    21374 2024-05-04 15:14:22.000000 pygazpar-1.3.0a6/pygazpar/datasource.py
--rw-r--r--   0 runner    (1001) docker     (127)      898 2024-05-04 15:14:22.000000 pygazpar-1.3.0a6/pygazpar/enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     5915 2024-05-04 15:14:22.000000 pygazpar-1.3.0a6/pygazpar/excelparser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-05-04 15:14:22.000000 pygazpar-1.3.0a6/pygazpar/jsonparser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 15:16:22.928136 pygazpar-1.3.0a6/pygazpar/resources/
--rw-r--r--   0 runner    (1001) docker     (127)   199583 2024-05-04 15:14:22.000000 pygazpar-1.3.0a6/pygazpar/resources/daily_data_sample.json
--rw-r--r--   0 runner    (1001) docker     (127)        3 2024-05-04 15:14:22.000000 pygazpar-1.3.0a6/pygazpar/resources/hourly_data_sample.json
--rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-05-04 15:14:22.000000 pygazpar-1.3.0a6/pygazpar/resources/monthly_data_sample.json
--rw-r--r--   0 runner    (1001) docker     (127)    15587 2024-05-04 15:14:22.000000 pygazpar-1.3.0a6/pygazpar/resources/weekly_data_sample.json
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-04 15:14:22.000000 pygazpar-1.3.0a6/pygazpar/resources/yearly_data_sample.json
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-04 15:16:21.000000 pygazpar-1.3.0a6/pygazpar/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 15:16:22.928136 pygazpar-1.3.0a6/pygazpar.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    20961 2024-05-04 15:16:22.000000 pygazpar-1.3.0a6/pygazpar.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-04 15:16:22.000000 pygazpar-1.3.0a6/pygazpar.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 15:16:22.000000 pygazpar-1.3.0a6/pygazpar.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-04 15:16:22.000000 pygazpar-1.3.0a6/pygazpar.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 15:16:22.000000 pygazpar-1.3.0a6/pygazpar.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-04 15:16:22.000000 pygazpar-1.3.0a6/pygazpar.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-04 15:16:22.000000 pygazpar-1.3.0a6/pygazpar.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 15:16:22.928136 pygazpar-1.3.0a6/samples/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 15:14:22.000000 pygazpar-1.3.0a6/samples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-04 15:14:22.000000 pygazpar-1.3.0a6/samples/excelSample.py
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-04 15:14:22.000000 pygazpar-1.3.0a6/samples/jsonSample.py
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-04 15:14:22.000000 pygazpar-1.3.0a6/samples/testSample.py
--rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-05-04 15:16:22.932136 pygazpar-1.3.0a6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 15:14:22.000000 pygazpar-1.3.0a6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 15:16:22.928136 pygazpar-1.3.0a6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 15:14:22.000000 pygazpar-1.3.0a6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5111 2024-05-04 15:14:22.000000 pygazpar-1.3.0a6/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-04 15:14:22.000000 pygazpar-1.3.0a6/tests/test_datafileparser.py
--rw-r--r--   0 runner    (1001) docker     (127)     5983 2024-05-04 15:14:22.000000 pygazpar-1.3.0a6/tests/test_datasource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:12:14.114101 pygazpar-1.3.0a9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-08 11:09:52.000000 pygazpar-1.3.0a9/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-08 11:09:52.000000 pygazpar-1.3.0a9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    21460 2024-05-08 11:12:14.114101 pygazpar-1.3.0a9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5058 2024-05-08 11:09:52.000000 pygazpar-1.3.0a9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:12:14.110101 pygazpar-1.3.0a9/pygazpar/
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-08 11:09:52.000000 pygazpar-1.3.0a9/pygazpar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3177 2024-05-08 11:09:52.000000 pygazpar-1.3.0a9/pygazpar/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-05-08 11:09:52.000000 pygazpar-1.3.0a9/pygazpar/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21470 2024-05-08 11:09:52.000000 pygazpar-1.3.0a9/pygazpar/datasource.py
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-05-08 11:09:52.000000 pygazpar-1.3.0a9/pygazpar/enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5915 2024-05-08 11:09:52.000000 pygazpar-1.3.0a9/pygazpar/excelparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-05-08 11:09:52.000000 pygazpar-1.3.0a9/pygazpar/jsonparser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:12:14.110101 pygazpar-1.3.0a9/pygazpar/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)   199583 2024-05-08 11:09:52.000000 pygazpar-1.3.0a9/pygazpar/resources/daily_data_sample.json
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2024-05-08 11:09:52.000000 pygazpar-1.3.0a9/pygazpar/resources/hourly_data_sample.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-05-08 11:09:52.000000 pygazpar-1.3.0a9/pygazpar/resources/monthly_data_sample.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15587 2024-05-08 11:09:52.000000 pygazpar-1.3.0a9/pygazpar/resources/weekly_data_sample.json
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-08 11:09:52.000000 pygazpar-1.3.0a9/pygazpar/resources/yearly_data_sample.json
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-08 11:12:13.000000 pygazpar-1.3.0a9/pygazpar/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:12:14.110101 pygazpar-1.3.0a9/pygazpar.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    21460 2024-05-08 11:12:14.000000 pygazpar-1.3.0a9/pygazpar.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-08 11:12:14.000000 pygazpar-1.3.0a9/pygazpar.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 11:12:14.000000 pygazpar-1.3.0a9/pygazpar.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-08 11:12:14.000000 pygazpar-1.3.0a9/pygazpar.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 11:12:14.000000 pygazpar-1.3.0a9/pygazpar.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-08 11:12:14.000000 pygazpar-1.3.0a9/pygazpar.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-08 11:12:14.000000 pygazpar-1.3.0a9/pygazpar.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:12:14.114101 pygazpar-1.3.0a9/samples/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 11:09:52.000000 pygazpar-1.3.0a9/samples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-08 11:09:52.000000 pygazpar-1.3.0a9/samples/excelSample.py
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-08 11:09:52.000000 pygazpar-1.3.0a9/samples/jsonSample.py
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-08 11:09:52.000000 pygazpar-1.3.0a9/samples/testSample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-05-08 11:12:14.114101 pygazpar-1.3.0a9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 11:09:52.000000 pygazpar-1.3.0a9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:12:14.114101 pygazpar-1.3.0a9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 11:09:52.000000 pygazpar-1.3.0a9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5111 2024-05-08 11:09:52.000000 pygazpar-1.3.0a9/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-08 11:09:52.000000 pygazpar-1.3.0a9/tests/test_datafileparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5983 2024-05-08 11:09:52.000000 pygazpar-1.3.0a9/tests/test_datasource.py
```

### Comparing `pygazpar-1.3.0a6/LICENSE.md` & `pygazpar-1.3.0a9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pygazpar-1.3.0a6/PKG-INFO` & `pygazpar-1.3.0a9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 Metadata-Version: 2.1
 Name: pygazpar
-Version: 1.3.0a6
+Version: 1.3.0a9
 Summary: Retrieve gas consumption from GrDF web site (French Gas Company)
 Home-page: https://github.com/ssenart/pygazpar
 Author: Stephane Senart
 Author-email: stephane.senart@gmail.com
 License: MIT
 Download-URL: https://github.com/ssenart/pygazpar/releases
 Project-URL: Home, https://github.com/ssenart/pygazpar
 Project-URL: Source, https://github.com/ssenart/pygazpar
 Project-URL: Issues, https://github.com/ssenart/PyGazpar/issues
 Project-URL: Changelog, https://github.com/ssenart/PyGazpar/blob/master/CHANGELOG.md
 Project-URL: Download, https://pypi.org/project/pygazpar
 Description: # PyGazpar
+        
+        ## <span style="color:green">!!! This library is working again. CAPTCHA has been removed !!!</span>
+        
+        ## <span style="color:red">~~!!! This library is broken since CAPTCHA is mandatory on GrDF site !!!~~</span>
+        
         PyGazpar is a Python library for getting natural gas consumption from GrDF French provider.
         
         Their natural gas meter is called Gazpar. It is wireless and transmit the gas consumption once per day.
         
         All consumption data is available on the client account at GrDF Web Site (https://monespace.grdf.fr).
         
         PyGazpar automatically goes through the Web Site and download the consumption data, and make it available in a Python structure.
@@ -193,14 +198,18 @@
         Corresponding Home Assistant integration custom component is available [here](https://github.com/ssenart/home-assistant-gazpar).
         # Changelog
         All notable changes to this project will be documented in this file.
         
         The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
         and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
         
+        ## [1.2.2](https://github.com/ssenart/PyGazpar/compare/1.2.1...1.2.2) - 2024-05-08
+        
+        ### Fixed
+        - [#65](https://github.com/ssenart/PyGazpar/issues/65): [Bug] PermissionError happens when loading data from Excel file.
         
         ## [1.2.1](https://github.com/ssenart/PyGazpar/compare/1.2.0...1.2.1) - 2024-05-04
         
         ### Fixed
         - [#64](https://github.com/ssenart/PyGazpar/issues/64): [Issue] Captcha failed issue.
         
         - [#63](https://github.com/ssenart/PyGazpar/issues/63): [Bug] If the latest received consumption is Sunday, then the last weekly period is duplicated.
```

### Comparing `pygazpar-1.3.0a6/README.md` & `pygazpar-1.3.0a9/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,13 @@
 # PyGazpar
+
+## <span style="color:green">!!! This library is working again. CAPTCHA has been removed !!!</span>
+
+## <span style="color:red">~~!!! This library is broken since CAPTCHA is mandatory on GrDF site !!!~~</span>
+
 PyGazpar is a Python library for getting natural gas consumption from GrDF French provider.
 
 Their natural gas meter is called Gazpar. It is wireless and transmit the gas consumption once per day.
 
 All consumption data is available on the client account at GrDF Web Site (https://monespace.grdf.fr).
 
 PyGazpar automatically goes through the Web Site and download the consumption data, and make it available in a Python structure.
```

### Comparing `pygazpar-1.3.0a6/pygazpar/__main__.py` & `pygazpar-1.3.0a9/pygazpar/__main__.py`

 * *Files identical despite different names*

### Comparing `pygazpar-1.3.0a6/pygazpar/client.py` & `pygazpar-1.3.0a9/pygazpar/client.py`

 * *Files identical despite different names*

### Comparing `pygazpar-1.3.0a6/pygazpar/datasource.py` & `pygazpar-1.3.0a9/pygazpar/datasource.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,15 +140,18 @@
         # XLSX is in the TMP directory
         data_file_path_pattern = self.__tmpDirectory + '/' + ExcelWebDataSource.DATA_FILENAME
 
         # We remove an eventual existing data file (from a previous run that has not deleted it).
         file_list = glob.glob(data_file_path_pattern)
         for filename in file_list:
             if os.path.isfile(filename):
-                os.remove(filename)
+                try:
+                    os.remove(filename)
+                except PermissionError:
+                    pass
 
         if frequencies is None:
             # Transform Enum in List.
             frequencyList = [frequency for frequency in Frequency]
         else:
             # Get unique values.
             frequencyList = set(frequencies)
@@ -190,15 +193,15 @@
                 Logger.warning(f"Not any data file has been found in '{self.__tmpDirectory}' directory")
 
             for filename in file_list:
                 res[frequency.value] = ExcelParser.parse(filename, frequency if frequency != Frequency.YEARLY else Frequency.DAILY)
                 try:
                     # openpyxl does not close the file properly.
                     os.remove(filename)
-                except Exception:
+                except PermissionError:
                     pass
 
             # We compute yearly from daily data.
             if frequency == Frequency.YEARLY:
                 res[frequency.value] = FrequencyConverter.computeYearly(res[frequency.value])
 
         return res
```

### Comparing `pygazpar-1.3.0a6/pygazpar/enum.py` & `pygazpar-1.3.0a9/pygazpar/enum.py`

 * *Files identical despite different names*

### Comparing `pygazpar-1.3.0a6/pygazpar/excelparser.py` & `pygazpar-1.3.0a9/pygazpar/excelparser.py`

 * *Files identical despite different names*

### Comparing `pygazpar-1.3.0a6/pygazpar/jsonparser.py` & `pygazpar-1.3.0a9/pygazpar/jsonparser.py`

 * *Files identical despite different names*

### Comparing `pygazpar-1.3.0a6/pygazpar/resources/daily_data_sample.json` & `pygazpar-1.3.0a9/pygazpar/resources/daily_data_sample.json`

 * *Files identical despite different names*

### Comparing `pygazpar-1.3.0a6/pygazpar/resources/monthly_data_sample.json` & `pygazpar-1.3.0a9/pygazpar/resources/monthly_data_sample.json`

 * *Files identical despite different names*

### Comparing `pygazpar-1.3.0a6/pygazpar/resources/weekly_data_sample.json` & `pygazpar-1.3.0a9/pygazpar/resources/weekly_data_sample.json`

 * *Files identical despite different names*

### Comparing `pygazpar-1.3.0a6/pygazpar.egg-info/PKG-INFO` & `pygazpar-1.3.0a9/pygazpar.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 Metadata-Version: 2.1
 Name: pygazpar
-Version: 1.3.0a6
+Version: 1.3.0a9
 Summary: Retrieve gas consumption from GrDF web site (French Gas Company)
 Home-page: https://github.com/ssenart/pygazpar
 Author: Stephane Senart
 Author-email: stephane.senart@gmail.com
 License: MIT
 Download-URL: https://github.com/ssenart/pygazpar/releases
 Project-URL: Home, https://github.com/ssenart/pygazpar
 Project-URL: Source, https://github.com/ssenart/pygazpar
 Project-URL: Issues, https://github.com/ssenart/PyGazpar/issues
 Project-URL: Changelog, https://github.com/ssenart/PyGazpar/blob/master/CHANGELOG.md
 Project-URL: Download, https://pypi.org/project/pygazpar
 Description: # PyGazpar
+        
+        ## <span style="color:green">!!! This library is working again. CAPTCHA has been removed !!!</span>
+        
+        ## <span style="color:red">~~!!! This library is broken since CAPTCHA is mandatory on GrDF site !!!~~</span>
+        
         PyGazpar is a Python library for getting natural gas consumption from GrDF French provider.
         
         Their natural gas meter is called Gazpar. It is wireless and transmit the gas consumption once per day.
         
         All consumption data is available on the client account at GrDF Web Site (https://monespace.grdf.fr).
         
         PyGazpar automatically goes through the Web Site and download the consumption data, and make it available in a Python structure.
@@ -193,14 +198,18 @@
         Corresponding Home Assistant integration custom component is available [here](https://github.com/ssenart/home-assistant-gazpar).
         # Changelog
         All notable changes to this project will be documented in this file.
         
         The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
         and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
         
+        ## [1.2.2](https://github.com/ssenart/PyGazpar/compare/1.2.1...1.2.2) - 2024-05-08
+        
+        ### Fixed
+        - [#65](https://github.com/ssenart/PyGazpar/issues/65): [Bug] PermissionError happens when loading data from Excel file.
         
         ## [1.2.1](https://github.com/ssenart/PyGazpar/compare/1.2.0...1.2.1) - 2024-05-04
         
         ### Fixed
         - [#64](https://github.com/ssenart/PyGazpar/issues/64): [Issue] Captcha failed issue.
         
         - [#63](https://github.com/ssenart/PyGazpar/issues/63): [Bug] If the latest received consumption is Sunday, then the last weekly period is duplicated.
```

### Comparing `pygazpar-1.3.0a6/pygazpar.egg-info/SOURCES.txt` & `pygazpar-1.3.0a9/pygazpar.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pygazpar-1.3.0a6/samples/excelSample.py` & `pygazpar-1.3.0a9/samples/excelSample.py`

 * *Files identical despite different names*

### Comparing `pygazpar-1.3.0a6/samples/jsonSample.py` & `pygazpar-1.3.0a9/samples/jsonSample.py`

 * *Files identical despite different names*

### Comparing `pygazpar-1.3.0a6/setup.cfg` & `pygazpar-1.3.0a9/setup.cfg`

 * *Files identical despite different names*

### Comparing `pygazpar-1.3.0a6/tests/test_client.py` & `pygazpar-1.3.0a9/tests/test_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,15 @@
         assert (len(data[Frequency.WEEKLY.value]) >= 51 and len(data[Frequency.WEEKLY.value]) <= 54)
 
     def test_monthly_jsonweb(self):
         client = Client(JsonWebDataSource(self.__username, self.__password))
 
         data = client.loadSince(self.__pceIdentifier, 365, [Frequency.MONTHLY])
 
-        assert (len(data[Frequency.MONTHLY.value]) >= 12 and len(data[Frequency.MONTHLY.value]) <= 13)
+        assert (len(data[Frequency.MONTHLY.value]) >= 11 and len(data[Frequency.MONTHLY.value]) <= 13)
 
     def test_yearly_jsonweb(self):
         client = Client(JsonWebDataSource(self.__username, self.__password))
 
         data = client.loadSince(self.__pceIdentifier, 365, [Frequency.YEARLY])
 
         assert (len(data[Frequency.YEARLY.value]) == 1)
```

### Comparing `pygazpar-1.3.0a6/tests/test_datafileparser.py` & `pygazpar-1.3.0a9/tests/test_datafileparser.py`

 * *Files identical despite different names*

### Comparing `pygazpar-1.3.0a6/tests/test_datasource.py` & `pygazpar-1.3.0a9/tests/test_datasource.py`

 * *Files 1% similar despite different names*

```diff
@@ -139,15 +139,15 @@
 
         data = dataSource.load(self.__pceIdentifier, startDate, endDate, [Frequency.DAILY, Frequency.WEEKLY, Frequency.MONTHLY, Frequency.YEARLY])
 
         assert (len(data[Frequency.DAILY.value]) > 0)
 
         assert (len(data[Frequency.WEEKLY.value]) >= 51 and len(data[Frequency.WEEKLY.value]) <= 54)
 
-        assert (len(data[Frequency.MONTHLY.value]) >= 12 and len(data[Frequency.MONTHLY.value]) <= 13)
+        assert (len(data[Frequency.MONTHLY.value]) >= 11 and len(data[Frequency.MONTHLY.value]) <= 13)
 
         assert (len(data[Frequency.YEARLY.value]) == 1)
 
     # ------------------------------------------------------
     def test_excelweb(self):
 
         dataSource = ExcelWebDataSource(self.__username, self.__password, self.__tmp_directory)
```

