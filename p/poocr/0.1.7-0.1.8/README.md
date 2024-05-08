# Comparing `tmp/poocr-0.1.7.tar.gz` & `tmp/poocr-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poocr-0.1.7.tar", last modified: Mon May  6 13:41:22 2024, max compression
+gzip compressed data, was "poocr-0.1.8.tar", last modified: Wed May  8 13:40:31 2024, max compression
```

## Comparing `poocr-0.1.7.tar` & `poocr-0.1.8.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 13:41:22.243298 poocr-0.1.7/
--rw-rw-rw-   0        0        0     1093 2022-09-13 01:21:27.000000 poocr-0.1.7/LICENSE
--rw-rw-rw-   0        0        0     3823 2024-05-06 13:41:22.237785 poocr-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0     3145 2024-04-30 17:27:09.000000 poocr-0.1.7/README.md
-drwxrwxrwx   0        0        0        0 2024-05-06 13:41:22.175894 poocr-0.1.7/poocr/
--rw-rw-rw-   0        0        0      810 2024-02-26 13:41:46.000000 poocr-0.1.7/poocr/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-06 13:41:22.211552 poocr-0.1.7/poocr/api/
--rw-rw-rw-   0        0        0      265 2023-03-25 11:08:27.000000 poocr-0.1.7/poocr/api/__init__.py
--rw-rw-rw-   0        0        0    25370 2024-05-06 13:35:11.000000 poocr-0.1.7/poocr/api/ocr.py
--rw-rw-rw-   0        0        0     9163 2024-05-06 13:14:21.000000 poocr-0.1.7/poocr/api/ocr2excel.py
-drwxrwxrwx   0        0        0        0 2024-05-06 13:41:22.217412 poocr-0.1.7/poocr/core/
--rw-rw-rw-   0        0        0     1815 2024-05-06 13:38:21.000000 poocr-0.1.7/poocr/core/BaiduOCR.py
--rw-rw-rw-   0        0        0     4271 2023-07-25 15:06:57.000000 poocr-0.1.7/poocr/core/OCR.py
--rw-rw-rw-   0        0        0      223 2023-01-22 06:56:13.000000 poocr-0.1.7/poocr/core/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-06 13:41:22.227708 poocr-0.1.7/poocr/lib/
--rw-rw-rw-   0        0        0     1017 2023-01-28 13:49:56.000000 poocr-0.1.7/poocr/lib/CommonUtils.py
--rw-rw-rw-   0        0        0     1132 2023-01-30 12:39:04.000000 poocr-0.1.7/poocr/lib/Config.py
--rw-rw-rw-   0        0        0      852 2023-01-30 12:39:04.000000 poocr-0.1.7/poocr/lib/Const.py
--rw-rw-rw-   0        0        0        0 2023-01-22 10:20:33.000000 poocr-0.1.7/poocr/lib/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-06 13:41:22.237785 poocr-0.1.7/poocr.egg-info/
--rw-rw-rw-   0        0        0     3823 2024-05-06 13:41:21.000000 poocr-0.1.7/poocr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      478 2024-05-06 13:41:22.000000 poocr-0.1.7/poocr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 13:41:21.000000 poocr-0.1.7/poocr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-22 14:21:59.000000 poocr-0.1.7/poocr.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       61 2024-05-06 13:41:21.000000 poocr-0.1.7/poocr.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-05-06 13:41:21.000000 poocr-0.1.7/poocr.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      759 2024-05-06 13:41:22.248565 poocr-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0      389 2022-10-23 08:47:10.000000 poocr-0.1.7/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-06 13:41:22.232731 poocr-0.1.7/tests/
--rw-rw-rw-   0        0        0      181 2023-01-30 12:39:04.000000 poocr-0.1.7/tests/__init__.py
--rw-rw-rw-   0        0        0     1150 2024-04-30 17:30:56.000000 poocr-0.1.7/tests/test_tencent.py
+drwxrwxrwx   0        0        0        0 2024-05-08 13:40:31.609313 poocr-0.1.8/
+-rw-rw-rw-   0        0        0     1093 2022-09-13 01:21:27.000000 poocr-0.1.8/LICENSE
+-rw-rw-rw-   0        0        0     3823 2024-05-08 13:40:31.608308 poocr-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0     3145 2024-04-30 17:27:09.000000 poocr-0.1.8/README.md
+drwxrwxrwx   0        0        0        0 2024-05-08 13:40:31.528763 poocr-0.1.8/poocr/
+-rw-rw-rw-   0        0        0      810 2024-02-26 13:41:46.000000 poocr-0.1.8/poocr/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 13:40:31.576783 poocr-0.1.8/poocr/api/
+-rw-rw-rw-   0        0        0      265 2023-03-25 11:08:27.000000 poocr-0.1.8/poocr/api/__init__.py
+-rw-rw-rw-   0        0        0    25370 2024-05-06 13:35:11.000000 poocr-0.1.8/poocr/api/ocr.py
+-rw-rw-rw-   0        0        0     9452 2024-05-08 13:38:46.000000 poocr-0.1.8/poocr/api/ocr2excel.py
+drwxrwxrwx   0        0        0        0 2024-05-08 13:40:31.585307 poocr-0.1.8/poocr/core/
+-rw-rw-rw-   0        0        0     1815 2024-05-06 13:38:21.000000 poocr-0.1.8/poocr/core/BaiduOCR.py
+-rw-rw-rw-   0        0        0     4271 2023-07-25 15:06:57.000000 poocr-0.1.8/poocr/core/OCR.py
+-rw-rw-rw-   0        0        0      223 2023-01-22 06:56:13.000000 poocr-0.1.8/poocr/core/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 13:40:31.598303 poocr-0.1.8/poocr/lib/
+-rw-rw-rw-   0        0        0     1017 2023-01-28 13:49:56.000000 poocr-0.1.8/poocr/lib/CommonUtils.py
+-rw-rw-rw-   0        0        0     1132 2023-01-30 12:39:04.000000 poocr-0.1.8/poocr/lib/Config.py
+-rw-rw-rw-   0        0        0      852 2023-01-30 12:39:04.000000 poocr-0.1.8/poocr/lib/Const.py
+-rw-rw-rw-   0        0        0        0 2023-01-22 10:20:33.000000 poocr-0.1.8/poocr/lib/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 13:40:31.606305 poocr-0.1.8/poocr.egg-info/
+-rw-rw-rw-   0        0        0     3823 2024-05-08 13:40:31.000000 poocr-0.1.8/poocr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      478 2024-05-08 13:40:31.000000 poocr-0.1.8/poocr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 13:40:31.000000 poocr-0.1.8/poocr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-22 14:21:59.000000 poocr-0.1.8/poocr.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       61 2024-05-08 13:40:31.000000 poocr-0.1.8/poocr.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-08 13:40:31.000000 poocr-0.1.8/poocr.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      759 2024-05-08 13:40:31.618304 poocr-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0      389 2022-10-23 08:47:10.000000 poocr-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 13:40:31.603306 poocr-0.1.8/tests/
+-rw-rw-rw-   0        0        0      181 2023-01-30 12:39:04.000000 poocr-0.1.8/tests/__init__.py
+-rw-rw-rw-   0        0        0     1150 2024-04-30 17:30:56.000000 poocr-0.1.8/tests/test_tencent.py
```

### Comparing `poocr-0.1.7/LICENSE` & `poocr-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `poocr-0.1.7/PKG-INFO` & `poocr-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poocr
-Version: 0.1.7
+Version: 0.1.8
 Summary: pip install poocr
 Home-page: https://www.python-office.com/
 Author: CoderWanFeng
 Author-email: 1957875073@qq.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/CoderWanFeng/poocr/issues
 Project-URL: Documentation, https://github.com/CoderWanFeng/poocr/blob/main/README.md
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: poocr Version: 0.1.7 Summary: pip install poocr
+Metadata-Version: 2.1 Name: poocr Version: 0.1.8 Summary: pip install poocr
 Home-page: https://www.python-office.com/ Author: CoderWanFeng Author-email:
 1957875073@qq.com License: MIT Project-URL: Bug Tracker, https://github.com/
 CoderWanFeng/poocr/issues Project-URL: Documentation, https://github.com/
 CoderWanFeng/poocr/blob/main/README.md Project-URL: Source Code, https://
 github.com/CoderWanFeng/poocr Platform: any Requires-Python: >=3.7 Description-
 Content-Type: text/markdown License-File: LICENSE Requires-Dist: toml Requires-
 Dist: tencentcloud-sdk-python Requires-Dist: poprogress Requires-Dist: pofile
```

### Comparing `poocr-0.1.7/README.md` & `poocr-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `poocr-0.1.7/poocr/__init__.py` & `poocr-0.1.8/poocr/__init__.py`

 * *Files identical despite different names*

### Comparing `poocr-0.1.7/poocr/api/ocr.py` & `poocr-0.1.8/poocr/api/ocr.py`

 * *Files identical despite different names*

### Comparing `poocr-0.1.7/poocr/api/ocr2excel.py` & `poocr-0.1.8/poocr/api/ocr2excel.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,19 +47,25 @@
     for vat_img in simple_progress(vat_img_files):
         try:
             api_res = VatInvoiceOCR(img_path=str(vat_img), img_url=img_url, configPath=configPath, id=id, key=key)
             api_res_json = json.loads(str(api_res))
             VatInvoiceInfos = api_res_json['VatInvoiceInfos']
             dict_pandas = {}  # 存放一行数据
             # 读返回值的第一个key
+            beizhu_value = ''
             for VatInvoiceInfo in VatInvoiceInfos:
                 if file_name:
                     dict_pandas['文件名'] = Path(vat_img).name  # 增加文件名作为一列
+                row_name = VatInvoiceInfo['Name']
+                if row_name == "备注":
+                    beizhu_value += VatInvoiceInfo['Value']
+                else:
+                    dict_pandas[row_name] = VatInvoiceInfo['Value']
+            dict_pandas['备注'] = beizhu_value  # TODO：备注内容跟的合并方式
 
-                dict_pandas[VatInvoiceInfo['Name']] = VatInvoiceInfo['Value']
             # 读返回值的第二个key
             key_trans_history = {}
             new_item_json = []
             Items = api_res_json['Items']
             if trans:
                 import wftools
```

### Comparing `poocr-0.1.7/poocr/core/BaiduOCR.py` & `poocr-0.1.8/poocr/core/BaiduOCR.py`

 * *Files identical despite different names*

### Comparing `poocr-0.1.7/poocr/core/OCR.py` & `poocr-0.1.8/poocr/core/OCR.py`

 * *Files identical despite different names*

### Comparing `poocr-0.1.7/poocr/lib/CommonUtils.py` & `poocr-0.1.8/poocr/lib/CommonUtils.py`

 * *Files identical despite different names*

### Comparing `poocr-0.1.7/poocr/lib/Config.py` & `poocr-0.1.8/poocr/lib/Config.py`

 * *Files identical despite different names*

### Comparing `poocr-0.1.7/poocr/lib/Const.py` & `poocr-0.1.8/poocr/lib/Const.py`

 * *Files identical despite different names*

### Comparing `poocr-0.1.7/poocr.egg-info/PKG-INFO` & `poocr-0.1.8/poocr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poocr
-Version: 0.1.7
+Version: 0.1.8
 Summary: pip install poocr
 Home-page: https://www.python-office.com/
 Author: CoderWanFeng
 Author-email: 1957875073@qq.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/CoderWanFeng/poocr/issues
 Project-URL: Documentation, https://github.com/CoderWanFeng/poocr/blob/main/README.md
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: poocr Version: 0.1.7 Summary: pip install poocr
+Metadata-Version: 2.1 Name: poocr Version: 0.1.8 Summary: pip install poocr
 Home-page: https://www.python-office.com/ Author: CoderWanFeng Author-email:
 1957875073@qq.com License: MIT Project-URL: Bug Tracker, https://github.com/
 CoderWanFeng/poocr/issues Project-URL: Documentation, https://github.com/
 CoderWanFeng/poocr/blob/main/README.md Project-URL: Source Code, https://
 github.com/CoderWanFeng/poocr Platform: any Requires-Python: >=3.7 Description-
 Content-Type: text/markdown License-File: LICENSE Requires-Dist: toml Requires-
 Dist: tencentcloud-sdk-python Requires-Dist: poprogress Requires-Dist: pofile
```

### Comparing `poocr-0.1.7/setup.cfg` & `poocr-0.1.8/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 6f6f 6372 0d0a 7665 7273 696f   = poocr..versio
-00000020: 6e20 3d20 302e 312e 370d 0a64 6573 6372  n = 0.1.7..descr
+00000020: 6e20 3d20 302e 312e 380d 0a64 6573 6372  n = 0.1.8..descr
 00000030: 6970 7469 6f6e 203d 2070 6970 2069 6e73  iption = pip ins
 00000040: 7461 6c6c 2070 6f6f 6372 0d0a 6c6f 6e67  tall poocr..long
 00000050: 5f64 6573 6372 6970 7469 6f6e 203d 2066  _description = f
 00000060: 696c 653a 2052 4541 444d 452e 6d64 0d0a  ile: README.md..
 00000070: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
 00000080: 5f63 6f6e 7465 6e74 5f74 7970 6520 3d20  _content_type = 
 00000090: 7465 7874 2f6d 6172 6b64 6f77 6e0d 0a75  text/markdown..u
```

### Comparing `poocr-0.1.7/tests/test_tencent.py` & `poocr-0.1.8/tests/test_tencent.py`

 * *Files identical despite different names*

