# Comparing `tmp/dicom2nifti-2.4.8.tar.gz` & `tmp/dicom2nifti-2.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dicom2nifti-2.4.8.tar", last modified: Mon Mar  6 08:28:45 2023, max compression
+gzip compressed data, was "dicom2nifti-2.4.9.tar", last modified: Thu Nov  2 11:24:16 2023, max compression
```

## Comparing `dicom2nifti-2.4.8.tar` & `dicom2nifti-2.4.9.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 abrys      (501) staff       (20)        0 2023-03-06 08:28:45.493529 dicom2nifti-2.4.8/
--rw-r--r--   0 abrys      (501) staff       (20)     1078 2022-10-24 07:10:28.000000 dicom2nifti-2.4.8/LICENSE
--rw-r--r--   0 abrys      (501) staff       (20)     1147 2023-03-06 08:28:45.493607 dicom2nifti-2.4.8/PKG-INFO
--rw-r--r--   0 abrys      (501) staff       (20)     5296 2022-10-24 07:10:28.000000 dicom2nifti-2.4.8/README.rst
-drwxr-xr-x   0 abrys      (501) staff       (20)        0 2023-03-06 08:28:45.489858 dicom2nifti-2.4.8/dicom2nifti/
--rw-r--r--   0 abrys      (501) staff       (20)      730 2022-10-24 07:10:28.000000 dicom2nifti-2.4.8/dicom2nifti/__init__.py
--rw-r--r--   0 abrys      (501) staff       (20)    45352 2023-03-03 20:25:15.000000 dicom2nifti-2.4.8/dicom2nifti/common.py
--rw-r--r--   0 abrys      (501) staff       (20)     7389 2022-12-23 19:03:34.000000 dicom2nifti-2.4.8/dicom2nifti/convert_dicom.py
--rw-r--r--   0 abrys      (501) staff       (20)     6370 2022-12-23 18:54:31.000000 dicom2nifti-2.4.8/dicom2nifti/convert_dir.py
--rw-r--r--   0 abrys      (501) staff       (20)    10277 2022-12-23 20:13:56.000000 dicom2nifti-2.4.8/dicom2nifti/convert_ge.py
--rw-r--r--   0 abrys      (501) staff       (20)    13744 2023-03-03 19:57:00.000000 dicom2nifti-2.4.8/dicom2nifti/convert_generic.py
--rw-r--r--   0 abrys      (501) staff       (20)     1557 2022-10-24 07:10:28.000000 dicom2nifti-2.4.8/dicom2nifti/convert_hitachi.py
--rw-r--r--   0 abrys      (501) staff       (20)    18525 2022-10-24 11:17:14.000000 dicom2nifti-2.4.8/dicom2nifti/convert_philips.py
--rw-r--r--   0 abrys      (501) staff       (20)    22638 2022-10-24 07:10:28.000000 dicom2nifti-2.4.8/dicom2nifti/convert_siemens.py
--rw-r--r--   0 abrys      (501) staff       (20)      664 2022-10-24 07:10:28.000000 dicom2nifti-2.4.8/dicom2nifti/exceptions.py
--rw-r--r--   0 abrys      (501) staff       (20)     6865 2022-10-24 07:10:28.000000 dicom2nifti-2.4.8/dicom2nifti/image_reorientation.py
--rw-r--r--   0 abrys      (501) staff       (20)    11215 2022-10-24 07:10:28.000000 dicom2nifti-2.4.8/dicom2nifti/image_volume.py
--rw-r--r--   0 abrys      (501) staff       (20)     2219 2022-10-24 07:10:28.000000 dicom2nifti-2.4.8/dicom2nifti/patch_pydicom_encodings.py
--rw-r--r--   0 abrys      (501) staff       (20)     6465 2022-10-24 07:10:28.000000 dicom2nifti-2.4.8/dicom2nifti/resample.py
--rw-r--r--   0 abrys      (501) staff       (20)     4564 2022-10-24 07:10:28.000000 dicom2nifti-2.4.8/dicom2nifti/settings.py
-drwxr-xr-x   0 abrys      (501) staff       (20)        0 2023-03-06 08:28:45.490459 dicom2nifti-2.4.8/dicom2nifti.egg-info/
--rw-r--r--   0 abrys      (501) staff       (20)     1147 2023-03-06 08:28:45.000000 dicom2nifti-2.4.8/dicom2nifti.egg-info/PKG-INFO
--rw-r--r--   0 abrys      (501) staff       (20)      972 2023-03-06 08:28:45.000000 dicom2nifti-2.4.8/dicom2nifti.egg-info/SOURCES.txt
--rw-r--r--   0 abrys      (501) staff       (20)        1 2023-03-06 08:28:45.000000 dicom2nifti-2.4.8/dicom2nifti.egg-info/dependency_links.txt
--rw-r--r--   0 abrys      (501) staff       (20)       47 2023-03-06 08:28:45.000000 dicom2nifti-2.4.8/dicom2nifti.egg-info/requires.txt
--rw-r--r--   0 abrys      (501) staff       (20)       12 2023-03-06 08:28:45.000000 dicom2nifti-2.4.8/dicom2nifti.egg-info/top_level.txt
-drwxr-xr-x   0 abrys      (501) staff       (20)        0 2023-03-06 08:28:45.490578 dicom2nifti-2.4.8/scripts/
--rwxr-xr-x   0 abrys      (501) staff       (20)     4080 2022-10-24 07:10:28.000000 dicom2nifti-2.4.8/scripts/dicom2nifti
--rw-r--r--   0 abrys      (501) staff       (20)      274 2023-03-06 08:28:45.493867 dicom2nifti-2.4.8/setup.cfg
--rw-r--r--   0 abrys      (501) staff       (20)     1698 2023-03-06 08:28:04.000000 dicom2nifti-2.4.8/setup.py
-drwxr-xr-x   0 abrys      (501) staff       (20)        0 2023-03-06 08:28:45.493294 dicom2nifti-2.4.8/tests/
--rw-r--r--   0 abrys      (501) staff       (20)     5440 2022-10-24 07:10:28.000000 dicom2nifti-2.4.8/tests/test_common.py
--rw-r--r--   0 abrys      (501) staff       (20)     8733 2022-12-23 20:03:51.000000 dicom2nifti-2.4.8/tests/test_data.py
--rw-r--r--   0 abrys      (501) staff       (20)     8788 2022-10-24 07:10:28.000000 dicom2nifti-2.4.8/tests/test_dicom.py
--rw-r--r--   0 abrys      (501) staff       (20)     4837 2022-10-24 07:10:28.000000 dicom2nifti-2.4.8/tests/test_dicom2nifti.py
--rw-r--r--   0 abrys      (501) staff       (20)      854 2022-10-24 07:10:28.000000 dicom2nifti-2.4.8/tests/test_directory.py
--rw-r--r--   0 abrys      (501) staff       (20)     7219 2022-10-24 07:10:28.000000 dicom2nifti-2.4.8/tests/test_ge.py
--rw-r--r--   0 abrys      (501) staff       (20)     9249 2022-10-24 07:10:28.000000 dicom2nifti-2.4.8/tests/test_generic.py
--rw-r--r--   0 abrys      (501) staff       (20)     2351 2022-10-24 07:10:28.000000 dicom2nifti-2.4.8/tests/test_hitachi.py
--rw-r--r--   0 abrys      (501) staff       (20)     1287 2022-10-24 07:10:28.000000 dicom2nifti-2.4.8/tests/test_hyperfine.py
--rw-r--r--   0 abrys      (501) staff       (20)    15511 2022-10-24 09:57:46.000000 dicom2nifti-2.4.8/tests/test_philips.py
--rw-r--r--   0 abrys      (501) staff       (20)     7057 2022-10-24 07:10:28.000000 dicom2nifti-2.4.8/tests/test_script_dicom2nifti.py
--rw-r--r--   0 abrys      (501) staff       (20)    12657 2022-10-24 07:10:28.000000 dicom2nifti-2.4.8/tests/test_siemens.py
--rw-r--r--   0 abrys      (501) staff       (20)     1308 2022-12-23 20:03:51.000000 dicom2nifti-2.4.8/tests/test_sirona.py
--rw-r--r--   0 abrys      (501) staff       (20)     2861 2022-10-24 11:26:32.000000 dicom2nifti-2.4.8/tests/test_tools.py
+drwxr-xr-x   0 abrys      (501) staff       (20)        0 2023-11-02 11:24:16.509560 dicom2nifti-2.4.9/
+-rw-r--r--   0 abrys      (501) staff       (20)     1078 2022-10-24 07:10:28.000000 dicom2nifti-2.4.9/LICENSE
+-rw-r--r--   0 abrys      (501) staff       (20)     1269 2023-11-02 11:24:16.509493 dicom2nifti-2.4.9/PKG-INFO
+-rw-r--r--   0 abrys      (501) staff       (20)     5296 2022-10-24 07:10:28.000000 dicom2nifti-2.4.9/README.rst
+drwxr-xr-x   0 abrys      (501) staff       (20)        0 2023-11-02 11:24:16.504711 dicom2nifti-2.4.9/dicom2nifti/
+-rw-r--r--   0 abrys      (501) staff       (20)      730 2022-10-24 07:10:28.000000 dicom2nifti-2.4.9/dicom2nifti/__init__.py
+-rw-r--r--   0 abrys      (501) staff       (20)    45790 2023-11-02 10:41:57.000000 dicom2nifti-2.4.9/dicom2nifti/common.py
+-rw-r--r--   0 abrys      (501) staff       (20)     7389 2022-12-23 19:03:34.000000 dicom2nifti-2.4.9/dicom2nifti/convert_dicom.py
+-rw-r--r--   0 abrys      (501) staff       (20)     6370 2022-12-23 18:54:31.000000 dicom2nifti-2.4.9/dicom2nifti/convert_dir.py
+-rw-r--r--   0 abrys      (501) staff       (20)     5900 2023-11-02 10:24:05.000000 dicom2nifti-2.4.9/dicom2nifti/convert_ge.py
+-rw-r--r--   0 abrys      (501) staff       (20)    18625 2023-11-02 10:41:57.000000 dicom2nifti-2.4.9/dicom2nifti/convert_generic.py
+-rw-r--r--   0 abrys      (501) staff       (20)     1557 2022-10-24 07:10:28.000000 dicom2nifti-2.4.9/dicom2nifti/convert_hitachi.py
+-rw-r--r--   0 abrys      (501) staff       (20)    18472 2023-11-02 10:41:57.000000 dicom2nifti-2.4.9/dicom2nifti/convert_philips.py
+-rw-r--r--   0 abrys      (501) staff       (20)    22610 2023-11-02 10:41:57.000000 dicom2nifti-2.4.9/dicom2nifti/convert_siemens.py
+-rw-r--r--   0 abrys      (501) staff       (20)      664 2022-10-24 07:10:28.000000 dicom2nifti-2.4.9/dicom2nifti/exceptions.py
+-rw-r--r--   0 abrys      (501) staff       (20)     6865 2022-10-24 07:10:28.000000 dicom2nifti-2.4.9/dicom2nifti/image_reorientation.py
+-rw-r--r--   0 abrys      (501) staff       (20)    11215 2022-10-24 07:10:28.000000 dicom2nifti-2.4.9/dicom2nifti/image_volume.py
+-rw-r--r--   0 abrys      (501) staff       (20)     2219 2022-10-24 07:10:28.000000 dicom2nifti-2.4.9/dicom2nifti/patch_pydicom_encodings.py
+-rw-r--r--   0 abrys      (501) staff       (20)     6465 2022-10-24 07:10:28.000000 dicom2nifti-2.4.9/dicom2nifti/resample.py
+-rw-r--r--   0 abrys      (501) staff       (20)     4564 2022-10-24 07:10:28.000000 dicom2nifti-2.4.9/dicom2nifti/settings.py
+drwxr-xr-x   0 abrys      (501) staff       (20)        0 2023-11-02 11:24:16.505392 dicom2nifti-2.4.9/dicom2nifti.egg-info/
+-rw-r--r--   0 abrys      (501) staff       (20)     1269 2023-11-02 11:24:16.000000 dicom2nifti-2.4.9/dicom2nifti.egg-info/PKG-INFO
+-rw-r--r--   0 abrys      (501) staff       (20)      972 2023-11-02 11:24:16.000000 dicom2nifti-2.4.9/dicom2nifti.egg-info/SOURCES.txt
+-rw-r--r--   0 abrys      (501) staff       (20)        1 2023-11-02 11:24:16.000000 dicom2nifti-2.4.9/dicom2nifti.egg-info/dependency_links.txt
+-rw-r--r--   0 abrys      (501) staff       (20)       47 2023-11-02 11:24:16.000000 dicom2nifti-2.4.9/dicom2nifti.egg-info/requires.txt
+-rw-r--r--   0 abrys      (501) staff       (20)       12 2023-11-02 11:24:16.000000 dicom2nifti-2.4.9/dicom2nifti.egg-info/top_level.txt
+drwxr-xr-x   0 abrys      (501) staff       (20)        0 2023-11-02 11:24:16.505516 dicom2nifti-2.4.9/scripts/
+-rwxr-xr-x   0 abrys      (501) staff       (20)     4080 2022-10-24 07:10:28.000000 dicom2nifti-2.4.9/scripts/dicom2nifti
+-rw-r--r--   0 abrys      (501) staff       (20)      274 2023-11-02 11:24:16.509794 dicom2nifti-2.4.9/setup.cfg
+-rw-r--r--   0 abrys      (501) staff       (20)     1698 2023-11-02 11:23:15.000000 dicom2nifti-2.4.9/setup.py
+drwxr-xr-x   0 abrys      (501) staff       (20)        0 2023-11-02 11:24:16.509122 dicom2nifti-2.4.9/tests/
+-rw-r--r--   0 abrys      (501) staff       (20)     5440 2022-10-24 07:10:28.000000 dicom2nifti-2.4.9/tests/test_common.py
+-rw-r--r--   0 abrys      (501) staff       (20)     8980 2023-11-02 11:05:30.000000 dicom2nifti-2.4.9/tests/test_data.py
+-rw-r--r--   0 abrys      (501) staff       (20)     8788 2022-10-24 07:10:28.000000 dicom2nifti-2.4.9/tests/test_dicom.py
+-rw-r--r--   0 abrys      (501) staff       (20)     4837 2022-10-24 07:10:28.000000 dicom2nifti-2.4.9/tests/test_dicom2nifti.py
+-rw-r--r--   0 abrys      (501) staff       (20)      854 2022-10-24 07:10:28.000000 dicom2nifti-2.4.9/tests/test_directory.py
+-rw-r--r--   0 abrys      (501) staff       (20)     7278 2023-11-02 10:25:33.000000 dicom2nifti-2.4.9/tests/test_ge.py
+-rw-r--r--   0 abrys      (501) staff       (20)     9249 2022-10-24 07:10:28.000000 dicom2nifti-2.4.9/tests/test_generic.py
+-rw-r--r--   0 abrys      (501) staff       (20)     2351 2022-10-24 07:10:28.000000 dicom2nifti-2.4.9/tests/test_hitachi.py
+-rw-r--r--   0 abrys      (501) staff       (20)     1287 2022-10-24 07:10:28.000000 dicom2nifti-2.4.9/tests/test_hyperfine.py
+-rw-r--r--   0 abrys      (501) staff       (20)    15952 2023-11-02 11:05:30.000000 dicom2nifti-2.4.9/tests/test_philips.py
+-rw-r--r--   0 abrys      (501) staff       (20)     7057 2022-10-24 07:10:28.000000 dicom2nifti-2.4.9/tests/test_script_dicom2nifti.py
+-rw-r--r--   0 abrys      (501) staff       (20)    12657 2022-10-24 07:10:28.000000 dicom2nifti-2.4.9/tests/test_siemens.py
+-rw-r--r--   0 abrys      (501) staff       (20)     1308 2022-12-23 20:03:51.000000 dicom2nifti-2.4.9/tests/test_sirona.py
+-rw-r--r--   0 abrys      (501) staff       (20)     2861 2022-10-24 11:26:32.000000 dicom2nifti-2.4.9/tests/test_tools.py
```

### Comparing `dicom2nifti-2.4.8/LICENSE` & `dicom2nifti-2.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dicom2nifti-2.4.8/PKG-INFO` & `dicom2nifti-2.4.9/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: dicom2nifti
-Version: 2.4.8
+Version: 2.4.9
 Summary: package for converting dicom files to nifti
 Home-page: https://github.com/icometrix/dicom2nifti
-Download-URL: https://github.com/icometrix/dicom2nifti/tarball/2.4.8
+Download-URL: https://github.com/icometrix/dicom2nifti/tarball/2.4.9
 Author: icometrix NV
 Author-email: dicom2nifti@icometrix.com
 Maintainer: icometrix NV
 Maintainer-email: dicom2nifti@icometrix.com
 License: MIT
 Keywords: dicom,nifti,medical imaging
 Classifier: Development Status :: 5 - Production/Stable
@@ -17,12 +17,17 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 License-File: LICENSE
+Requires-Dist: nibabel
+Requires-Dist: numpy
+Requires-Dist: scipy
+Requires-Dist: pydicom>=2.2.0
+Requires-Dist: python-gdcm
 
 
 With this package you can convert dicom images to nifti files.
 There is support for most anatomical CT and MR data.
 For MR specifically there is support for most 4D data (like DTI and fMRI)
```

### Comparing `dicom2nifti-2.4.8/README.rst` & `dicom2nifti-2.4.9/README.rst`

 * *Files identical despite different names*

### Comparing `dicom2nifti-2.4.8/dicom2nifti/__init__.py` & `dicom2nifti-2.4.9/dicom2nifti/__init__.py`

 * *Files identical despite different names*

### Comparing `dicom2nifti-2.4.8/dicom2nifti/common.py` & `dicom2nifti-2.4.9/dicom2nifti/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -1101,14 +1101,31 @@
     """
     Set the tr and te in the nifti headers
 
     :param echo_time: echo time
     :param repetition_time: repetition time
     :param nifti_image: nifti image to set the info to
     """
+
+    def is_float(number):
+        """
+        Helper to check if something is a float
+        """
+        try:
+            float(number)
+            return True
+        except ValueError:
+            return False
+
+    # only set if it is an actual float, can also be empty/none
+    if not is_float(repetition_time) or not is_float(echo_time):
+        return
+    repetition_time = float(repetition_time)
+    echo_time = float(echo_time)
+
     # set the repetition time in pixdim
     nifti_image.header.structarr['pixdim'][4] = repetition_time / 1000.0
 
     # set tr and te in db_name field
     nifti_image.header.structarr['db_name'] = '?TR:%.3f TE:%d' % (repetition_time, echo_time)
 
     return nifti_image
```

### Comparing `dicom2nifti-2.4.8/dicom2nifti/convert_dicom.py` & `dicom2nifti-2.4.9/dicom2nifti/convert_dicom.py`

 * *Files identical despite different names*

### Comparing `dicom2nifti-2.4.8/dicom2nifti/convert_dir.py` & `dicom2nifti-2.4.9/dicom2nifti/convert_dir.py`

 * *Files identical despite different names*

### Comparing `dicom2nifti-2.4.8/dicom2nifti/convert_generic.py` & `dicom2nifti-2.4.9/dicom2nifti/convert_generic.py`

 * *Files 25% similar despite different names*

```diff
@@ -13,14 +13,132 @@
 import dicom2nifti.common as common
 import dicom2nifti.settings as settings
 import dicom2nifti.resample as resample
 from dicom2nifti.exceptions import ConversionError, ConversionValidationError
 
 logger = logging.getLogger(__name__)
 
+def get_grouped_dicoms(dicom_input):
+    """
+    Search all dicoms in the dicom directory, sort and validate them
+
+    fast_read = True will only read the headers not the data
+    """
+
+    # Order all dicom files by InstanceNumber
+    dicoms = sorted(dicom_input, key=lambda x: x.InstanceNumber)
+
+    # now group per stack
+    grouped_dicoms = [[]]  # list with first element a list
+    stack_index = 0
+
+    # loop over all sorted dicoms and sort them by stack
+    # for this we use the position and direction of the slices so we can detect a new stack easily
+    previous_position = None
+    previous_direction = None
+    for dicom_ in dicoms:
+        current_direction = None
+        # if the stack number decreases we moved to the next stack
+        if previous_position is not None:
+            current_direction = numpy.array(dicom_.ImagePositionPatient) - previous_position
+            current_direction = current_direction / numpy.linalg.norm(current_direction)
+        if current_direction is not None and \
+                previous_direction is not None and \
+                not numpy.allclose(current_direction, previous_direction, rtol=0.05, atol=0.05):
+            previous_position = numpy.array(dicom_.ImagePositionPatient)
+            previous_direction = None
+            stack_index += 1
+        else:
+            previous_position = numpy.array(dicom_.ImagePositionPatient)
+            previous_direction = current_direction
+
+        if stack_index >= len(grouped_dicoms):
+            grouped_dicoms.append([])
+        grouped_dicoms[stack_index].append(dicom_)
+
+    return grouped_dicoms
+
+def is_4d(grouped_dicoms):
+    """
+    Use this function to detect if a dicom series is a ge 4d dataset
+    NOTE: Only the first slice will be checked so you can only provide an already sorted dicom directory
+    (containing one series)
+    """
+    # read dicom header
+    header = grouped_dicoms[0][0]
+
+    # check if contains multiple stacks
+    if len(grouped_dicoms) > 1:
+        return True
+
+    return False
+
+def four_d_to_nifti(grouped_dicoms, output_file):
+    """
+    This function will convert ge 4d series to a nifti
+    """
+
+    # Create mosaic block
+    logger.info('Creating data block')
+    full_block = _get_full_block(grouped_dicoms)
+
+    logger.info('Creating affine')
+    # Create the nifti header info
+    affine, slice_increment = common.create_affine(grouped_dicoms[0])
+
+    logger.info('Creating nifti')
+    # Convert to nifti
+    nii_image = nibabel.Nifti1Image(full_block, affine)
+    common.set_tr_te(nii_image, grouped_dicoms[0][0].RepetitionTime, grouped_dicoms[0][0].EchoTime)
+    logger.info('Saving nifti to disk %s' % output_file)
+
+    # Save to disk
+    if output_file is not None:
+        nii_image.header.set_slope_inter(1, 0)
+        nii_image.header.set_xyzt_units(2)  # set units for xyz (leave t as unknown)
+        nii_image.to_filename(output_file)
+
+    return {'NII_FILE': output_file,
+            'NII': nii_image,
+            'MAX_SLICE_INCREMENT': slice_increment}
+
+def _get_full_block(grouped_dicoms):
+    """
+    Generate a full datablock containing all timepoints
+    """
+    # For each slice / mosaic create a data volume block
+    data_blocks = []
+    for index in range(0, len(grouped_dicoms)):
+        logger.info('Creating block %s of %s' % (index + 1, len(grouped_dicoms)))
+        data_blocks.append(_timepoint_to_block(grouped_dicoms[index]))
+
+    # Add the data_blocks together to one 4d block
+    size_x = numpy.shape(data_blocks[0])[0]
+    size_y = numpy.shape(data_blocks[0])[1]
+    size_z = numpy.shape(data_blocks[0])[2]
+    size_t = len(data_blocks)
+    full_block = numpy.zeros((size_x, size_y, size_z, size_t), dtype=data_blocks[0].dtype)
+    for index in range(0, size_t):
+        if full_block[:, :, :, index].shape != data_blocks[index].shape:
+            logger.warning('Missing slices (slice count mismatch between timepoint %s and %s)' % (index - 1, index))
+            logger.warning('---------------------------------------------------------')
+            logger.warning(full_block[:, :, :, index].shape)
+            logger.warning(data_blocks[index].shape)
+            logger.warning('---------------------------------------------------------')
+            raise ConversionError("MISSING_DICOM_FILES")
+        full_block[:, :, :, index] = data_blocks[index]
+
+    return full_block
+
+def _timepoint_to_block(timepoint_dicoms):
+    """
+    Convert slices to a block of data by reading the headers and appending
+    """
+    # similar way of getting the block to anatomical however here we are creating the dicom series our selves
+    return common.get_volume_pixeldata(timepoint_dicoms)
 
 def multiframe_to_nifti(dicom_input, output_file):
     """
     This function will convert an anatomical dicom series to a nifti
 
     Examples: See unit test
 
@@ -64,15 +182,15 @@
         if dicom_input[0].PhotometricInterpretation == 'RGB':
             nii_image = create_rgba_nifti(data, affine)
         else:
             nii_image = nibabel.Nifti1Image(data, affine)
 
     # Set TR and TE if available
     if Tag(0x0018, 0x0080) in dicom_input[0] and Tag(0x0018, 0x0081) in dicom_input[0]:
-        common.set_tr_te(nii_image, float(dicom_input[0].RepetitionTime), float(dicom_input[0].EchoTime))
+        common.set_tr_te(nii_image, dicom_input[0].RepetitionTime, dicom_input[0].EchoTime)
 
     # Save to disk
     if output_file is not None:
         logger.info('Saving nifti to disk %s' % output_file)
         nii_image.header.set_slope_inter(1, 0)
         nii_image.header.set_xyzt_units(2)  # set units for xyz (leave t as unknown)
         nii_image.to_filename(output_file)
@@ -118,14 +236,21 @@
     if settings.validate_orientation:
         # validate that all slices have the same orientation
         common.validate_orientation(dicom_input)
     if settings.validate_orthogonal:
         # validate that we have an orthogonal image (to detect gantry tilting etc)
         common.validate_orthogonal(dicom_input)
 
+    logger.info('Reading and sorting dicom files')
+    grouped_dicoms = get_grouped_dicoms(dicom_input)
+
+    if is_4d(grouped_dicoms):
+        logger.info('Found sequence type: 4D')
+        return four_d_to_nifti(grouped_dicoms, output_file)
+
     # sort the dicoms
     dicom_input = common.sort_dicoms(dicom_input)
 
     # validate slice increment inconsistent
     slice_increment_inconsistent = False
     if settings.validate_slice_increment:
         # validate that all slices have a consistent slice increment
@@ -153,15 +278,15 @@
         if dicom_input[0].PhotometricInterpretation == 'RGB':
             nii_image = create_rgba_nifti(data, affine)
         else:
             nii_image = nibabel.Nifti1Image(data, affine)
 
     # Set TR and TE if available
     if Tag(0x0018, 0x0080) in dicom_input[0] and Tag(0x0018, 0x0081) in dicom_input[0]:
-        common.set_tr_te(nii_image, float(dicom_input[0].RepetitionTime), float(dicom_input[0].EchoTime))
+        common.set_tr_te(nii_image, dicom_input[0].RepetitionTime, dicom_input[0].EchoTime)
 
     # Save to disk
     if output_file is not None:
         logger.info('Saving nifti to disk %s' % output_file)
         nii_image.header.set_slope_inter(1, 0)
         nii_image.header.set_xyzt_units(2)  # set units for xyz (leave t as unknown)
         nii_image.to_filename(output_file)
```

### Comparing `dicom2nifti-2.4.8/dicom2nifti/convert_hitachi.py` & `dicom2nifti-2.4.9/dicom2nifti/convert_hitachi.py`

 * *Files identical despite different names*

### Comparing `dicom2nifti-2.4.8/dicom2nifti/convert_philips.py` & `dicom2nifti-2.4.9/dicom2nifti/convert_philips.py`

 * *Files 0% similar despite different names*

```diff
@@ -234,16 +234,15 @@
     # Convert to nifti
     if full_block.ndim > 3:  # do not squeeze single slice data
         full_block = full_block.squeeze()
     nii_image = nibabel.Nifti1Image(full_block, affine)
     try:
         timing_parameters = multiframe_dicom.SharedFunctionalGroupsSequence[0].MRTimingAndRelatedParametersSequence[0]
         first_frame = multiframe_dicom[Tag(0x5200, 0x9230)][0]
-        common.set_tr_te(nii_image, float(timing_parameters.RepetitionTime),
-                         float(first_frame.MREchoSequence[0].EchoTime))
+        common.set_tr_te(nii_image, timing_parameters.RepetitionTime, first_frame.MREchoSequence[0].EchoTime)
     except:
         logger.info('Unable to set timing info')
 
     # Save to disk
     if output_file is not None:
         logger.info('Saving nifti to disk %s' % output_file)
         nii_image.header.set_slope_inter(1, 0)
@@ -289,15 +288,15 @@
     affine, slice_increment = common.create_affine(grouped_dicoms[0])
 
     logger.info('Creating nifti')
     # Convert to nifti
     if full_block.ndim > 3:  # do not squeeze single slice data
         full_block = full_block.squeeze()
     nii_image = nibabel.Nifti1Image(full_block, affine)
-    common.set_tr_te(nii_image, float(grouped_dicoms[0][0].RepetitionTime), float(grouped_dicoms[0][0].EchoTime))
+    common.set_tr_te(nii_image, grouped_dicoms[0][0].RepetitionTime, grouped_dicoms[0][0].EchoTime)
 
     if output_file is not None:
         # Save to disk
         logger.info('Saving nifti to disk %s' % output_file)
         nii_image.header.set_slope_inter(1, 0)
         nii_image.header.set_xyzt_units(2)  # set units for xyz (leave t as unknown)
         nii_image.to_filename(output_file)
```

### Comparing `dicom2nifti-2.4.8/dicom2nifti/convert_siemens.py` & `dicom2nifti-2.4.9/dicom2nifti/convert_siemens.py`

 * *Files 1% similar despite different names*

```diff
@@ -162,15 +162,15 @@
     # Create the nifti header info
     affine = _create_affine_siemens_mosaic(dicom_input)
     logger.info('Creating nifti')
     # Convert to nifti
     if full_block.ndim > 3:
         full_block = full_block.squeeze()
     nii_image = nibabel.Nifti1Image(full_block, affine)
-    common.set_tr_te(nii_image, float(sorted_mosaics[0].RepetitionTime), float(sorted_mosaics[0].EchoTime))
+    common.set_tr_te(nii_image, sorted_mosaics[0].RepetitionTime, sorted_mosaics[0].EchoTime)
     logger.info('Saving nifti to disk')
     # Save to disk
     if output_file is not None:
         nii_image.header.set_slope_inter(1, 0)
         nii_image.header.set_xyzt_units(2)  # set units for xyz (leave t as unknown)
         nii_image.to_filename(output_file)
 
@@ -218,15 +218,15 @@
     affine, slice_increment = common.create_affine(grouped_dicoms[0])
 
     logger.info('Creating nifti')
     # Convert to nifti
     if full_block.ndim > 3:  # do not squeeze single slice data
         full_block = full_block.squeeze()
     nii_image = nibabel.Nifti1Image(full_block, affine)
-    common.set_tr_te(nii_image, float(grouped_dicoms[0][0].RepetitionTime), float(grouped_dicoms[0][0].EchoTime))
+    common.set_tr_te(nii_image, grouped_dicoms[0][0].RepetitionTime, grouped_dicoms[0][0].EchoTime)
     logger.info('Saving nifti to disk')
     # Save to disk
     if output_file is not None:
         nii_image.header.set_slope_inter(1, 0)
         nii_image.header.set_xyzt_units(2)  # set units for xyz (leave t as unknown)
         nii_image.to_filename(output_file)
```

### Comparing `dicom2nifti-2.4.8/dicom2nifti/exceptions.py` & `dicom2nifti-2.4.9/dicom2nifti/exceptions.py`

 * *Files identical despite different names*

### Comparing `dicom2nifti-2.4.8/dicom2nifti/image_reorientation.py` & `dicom2nifti-2.4.9/dicom2nifti/image_reorientation.py`

 * *Files identical despite different names*

### Comparing `dicom2nifti-2.4.8/dicom2nifti/image_volume.py` & `dicom2nifti-2.4.9/dicom2nifti/image_volume.py`

 * *Files identical despite different names*

### Comparing `dicom2nifti-2.4.8/dicom2nifti/patch_pydicom_encodings.py` & `dicom2nifti-2.4.9/dicom2nifti/patch_pydicom_encodings.py`

 * *Files identical despite different names*

### Comparing `dicom2nifti-2.4.8/dicom2nifti/resample.py` & `dicom2nifti-2.4.9/dicom2nifti/resample.py`

 * *Files identical despite different names*

### Comparing `dicom2nifti-2.4.8/dicom2nifti/settings.py` & `dicom2nifti-2.4.9/dicom2nifti/settings.py`

 * *Files identical despite different names*

### Comparing `dicom2nifti-2.4.8/dicom2nifti.egg-info/PKG-INFO` & `dicom2nifti-2.4.9/dicom2nifti.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: dicom2nifti
-Version: 2.4.8
+Version: 2.4.9
 Summary: package for converting dicom files to nifti
 Home-page: https://github.com/icometrix/dicom2nifti
-Download-URL: https://github.com/icometrix/dicom2nifti/tarball/2.4.8
+Download-URL: https://github.com/icometrix/dicom2nifti/tarball/2.4.9
 Author: icometrix NV
 Author-email: dicom2nifti@icometrix.com
 Maintainer: icometrix NV
 Maintainer-email: dicom2nifti@icometrix.com
 License: MIT
 Keywords: dicom,nifti,medical imaging
 Classifier: Development Status :: 5 - Production/Stable
@@ -17,12 +17,17 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 License-File: LICENSE
+Requires-Dist: nibabel
+Requires-Dist: numpy
+Requires-Dist: scipy
+Requires-Dist: pydicom>=2.2.0
+Requires-Dist: python-gdcm
 
 
 With this package you can convert dicom images to nifti files.
 There is support for most anatomical CT and MR data.
 For MR specifically there is support for most 4D data (like DTI and fMRI)
```

### Comparing `dicom2nifti-2.4.8/dicom2nifti.egg-info/SOURCES.txt` & `dicom2nifti-2.4.9/dicom2nifti.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dicom2nifti-2.4.8/scripts/dicom2nifti` & `dicom2nifti-2.4.9/scripts/dicom2nifti`

 * *Files identical despite different names*

### Comparing `dicom2nifti-2.4.8/setup.py` & `dicom2nifti-2.4.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 from setuptools import find_packages
 
 
-version = "2.4.8"
+version = "2.4.9"
 print('Starting pypi release version %s' % version)
 long_description = """
 With this package you can convert dicom images to nifti files.
 There is support for most anatomical CT and MR data.
 For MR specifically there is support for most 4D data (like DTI and fMRI)
 """
```

### Comparing `dicom2nifti-2.4.8/tests/test_common.py` & `dicom2nifti-2.4.9/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `dicom2nifti-2.4.8/tests/test_data.py` & `dicom2nifti-2.4.9/tests/test_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,14 +56,17 @@
 
 # PHILIPS DATASETS
 PHILIPS_ANATOMICAL = os.path.join(os.path.dirname(os.path.abspath(__file__)),
                                   'data', 'philips', 'anatomical', '001')
 
 PHILIPS_ANATOMICAL_IMPLICIT = os.path.join(os.path.dirname(os.path.abspath(__file__)),
                                            'data', 'philips', 'anatomical', '001_implicit')
+# icometrix/dicom2nifti#136 dataset containing both magnitude and phase encoded images
+PHILIPS_ANATOMICAL_SWI = os.path.join(os.path.dirname(os.path.abspath(__file__)),
+                                      'data', 'philips', 'anatomical', '002')
 
 PHILIPS_DTI = os.path.join(os.path.dirname(os.path.abspath(__file__)),
                            'data', 'philips', 'dti', '001')
 
 PHILIPS_DTI_IMPLICIT = os.path.join(os.path.dirname(os.path.abspath(__file__)),
                                     'data', 'philips', 'dti', '001_implicit')
```

### Comparing `dicom2nifti-2.4.8/tests/test_dicom.py` & `dicom2nifti-2.4.9/tests/test_dicom.py`

 * *Files identical despite different names*

### Comparing `dicom2nifti-2.4.8/tests/test_dicom2nifti.py` & `dicom2nifti-2.4.9/tests/test_dicom2nifti.py`

 * *Files identical despite different names*

### Comparing `dicom2nifti-2.4.8/tests/test_directory.py` & `dicom2nifti-2.4.9/tests/test_directory.py`

 * *Files identical despite different names*

### Comparing `dicom2nifti-2.4.8/tests/test_ge.py` & `dicom2nifti-2.4.9/tests/test_ge.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import shutil
 import tempfile
 import unittest
 
 import nibabel
 import numpy
 
+import convert_generic
 import tests.test_data as test_data
 
 import dicom2nifti.convert_ge as convert_ge
 import dicom2nifti.common as common
 from dicom2nifti.common import read_dicom_directory
 from tests.test_tools import assert_compare_nifti, assert_compare_bval, assert_compare_bvec, ground_thruth_filenames
 
@@ -113,25 +114,25 @@
         assert not common.is_ge(read_dicom_directory(test_data.SIEMENS_ANATOMICAL))
         assert common.is_ge(read_dicom_directory(test_data.GE_ANATOMICAL))
         assert not common.is_ge(read_dicom_directory(test_data.PHILIPS_ANATOMICAL))
         assert not common.is_ge(read_dicom_directory(test_data.GENERIC_ANATOMICAL))
         assert not common.is_ge(read_dicom_directory(test_data.HITACHI_ANATOMICAL))
 
     def test_is_4d(self):
-        diffusion_group = convert_ge._get_grouped_dicoms(read_dicom_directory(test_data.GE_DTI))
-        _4d_group = convert_ge._get_grouped_dicoms(read_dicom_directory(test_data.GE_FMRI))
-        anatomical_group = convert_ge._get_grouped_dicoms(read_dicom_directory(test_data.GE_ANATOMICAL))
-        self.assertTrue(convert_ge._is_4d(diffusion_group))
-        self.assertTrue(convert_ge._is_4d(_4d_group))
-        self.assertFalse(convert_ge._is_4d(anatomical_group))
+        diffusion_group = convert_generic.get_grouped_dicoms(read_dicom_directory(test_data.GE_DTI))
+        _4d_group = convert_generic.get_grouped_dicoms(read_dicom_directory(test_data.GE_FMRI))
+        anatomical_group = convert_generic.get_grouped_dicoms(read_dicom_directory(test_data.GE_ANATOMICAL))
+        self.assertTrue(convert_generic.is_4d(diffusion_group))
+        self.assertTrue(convert_generic.is_4d(_4d_group))
+        self.assertFalse(convert_generic.is_4d(anatomical_group))
 
     def test_is_diffusion_imaging(self):
-        diffusion_group = convert_ge._get_grouped_dicoms(read_dicom_directory(test_data.GE_DTI))
-        _4d_group = convert_ge._get_grouped_dicoms(read_dicom_directory(test_data.GE_FMRI))
-        anatomical_group = convert_ge._get_grouped_dicoms(read_dicom_directory(test_data.GE_ANATOMICAL))
+        diffusion_group = convert_generic.get_grouped_dicoms(read_dicom_directory(test_data.GE_DTI))
+        _4d_group = convert_generic.get_grouped_dicoms(read_dicom_directory(test_data.GE_FMRI))
+        anatomical_group = convert_generic.get_grouped_dicoms(read_dicom_directory(test_data.GE_ANATOMICAL))
         assert convert_ge._is_diffusion_imaging(diffusion_group)
         assert not convert_ge._is_diffusion_imaging(_4d_group)
         assert not convert_ge._is_diffusion_imaging(anatomical_group)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `dicom2nifti-2.4.8/tests/test_generic.py` & `dicom2nifti-2.4.9/tests/test_generic.py`

 * *Files identical despite different names*

### Comparing `dicom2nifti-2.4.8/tests/test_hitachi.py` & `dicom2nifti-2.4.9/tests/test_hitachi.py`

 * *Files identical despite different names*

### Comparing `dicom2nifti-2.4.8/tests/test_hyperfine.py` & `dicom2nifti-2.4.9/tests/test_hyperfine.py`

 * *Files identical despite different names*

### Comparing `dicom2nifti-2.4.8/tests/test_philips.py` & `dicom2nifti-2.4.9/tests/test_philips.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,14 +154,20 @@
 
             results = convert_philips.dicom_to_nifti(read_dicom_directory(test_data.PHILIPS_ANATOMICAL),
                                                      os.path.join(tmp_output_dir, 'test.nii.gz'))
             assert_compare_nifti(results['NII_FILE'],
                                  ground_thruth_filenames(test_data.PHILIPS_ANATOMICAL)[0])
             self.assertTrue(isinstance(results['NII'], nibabel.nifti1.Nifti1Image))
 
+            results = convert_philips.dicom_to_nifti(read_dicom_directory(test_data.PHILIPS_ANATOMICAL_SWI),
+                                                     os.path.join(tmp_output_dir, 'test.nii.gz'))
+            assert_compare_nifti(results['NII_FILE'],
+                                 ground_thruth_filenames(test_data.PHILIPS_ANATOMICAL_SWI)[0])
+            self.assertTrue(isinstance(results['NII'], nibabel.nifti1.Nifti1Image))
+
             results = convert_philips.dicom_to_nifti(read_dicom_directory(test_data.PHILIPS_ANATOMICAL_IMPLICIT),
                                                      os.path.join(tmp_output_dir, 'test.nii.gz'))
             assert_compare_nifti(results['NII_FILE'],
                                  ground_thruth_filenames(test_data.PHILIPS_ANATOMICAL_IMPLICIT)[0])
             self.assertTrue(isinstance(results['NII'], nibabel.nifti1.Nifti1Image))
 
             results = convert_philips.dicom_to_nifti(read_dicom_directory(test_data.PHILIPS_ENHANCED_ANATOMICAL),
```

### Comparing `dicom2nifti-2.4.8/tests/test_script_dicom2nifti.py` & `dicom2nifti-2.4.9/tests/test_script_dicom2nifti.py`

 * *Files identical despite different names*

### Comparing `dicom2nifti-2.4.8/tests/test_siemens.py` & `dicom2nifti-2.4.9/tests/test_siemens.py`

 * *Files identical despite different names*

### Comparing `dicom2nifti-2.4.8/tests/test_sirona.py` & `dicom2nifti-2.4.9/tests/test_sirona.py`

 * *Files identical despite different names*

### Comparing `dicom2nifti-2.4.8/tests/test_tools.py` & `dicom2nifti-2.4.9/tests/test_tools.py`

 * *Files identical despite different names*

