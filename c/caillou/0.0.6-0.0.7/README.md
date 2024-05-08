# Comparing `tmp/caillou-0.0.6-py3-none-any.whl.zip` & `tmp/caillou-0.0.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -3,13 +3,13 @@
 -rw-r--r--  2.0 unx      256 b- defN 80-Jan-01 00:00 caillou/__main__.py
 -rw-r--r--  2.0 unx       25 b- defN 80-Jan-01 00:00 caillou/apps/__init__.py
 -rw-r--r--  2.0 unx     3544 b- defN 80-Jan-01 00:00 caillou/apps/translator/__main__.py
 -rw-r--r--  2.0 unx    15743 b- defN 80-Jan-01 00:00 caillou/apps/translator/languages.json
 -rw-r--r--  2.0 unx      292 b- defN 80-Jan-01 00:00 caillou/apps/translator/styles.tcss
 -rw-r--r--  2.0 unx     1957 b- defN 80-Jan-01 00:00 caillou/config.py
 -rw-r--r--  2.0 unx     1689 b- defN 80-Jan-01 00:00 caillou/translate.py
--rw-r--r--  2.0 unx    35149 b- defN 80-Jan-01 00:00 caillou-0.0.6.dist-info/LICENSE
--rw-r--r--  2.0 unx     1685 b- defN 80-Jan-01 00:00 caillou-0.0.6.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 caillou-0.0.6.dist-info/WHEEL
--rw-r--r--  2.0 unx       49 b- defN 80-Jan-01 00:00 caillou-0.0.6.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx     1050 b- defN 16-Jan-01 00:00 caillou-0.0.6.dist-info/RECORD
+-rw-r--r--  2.0 unx    35149 b- defN 80-Jan-01 00:00 caillou-0.0.7.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1685 b- defN 80-Jan-01 00:00 caillou-0.0.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 caillou-0.0.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx       49 b- defN 80-Jan-01 00:00 caillou-0.0.7.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx     1050 b- defN 16-Jan-01 00:00 caillou-0.0.7.dist-info/RECORD
 13 files, 63598 bytes uncompressed, 21673 bytes compressed:  65.9%
```

## zipnote {}

```diff
@@ -18,23 +18,23 @@
 
 Filename: caillou/config.py
 Comment: 
 
 Filename: caillou/translate.py
 Comment: 
 
-Filename: caillou-0.0.6.dist-info/LICENSE
+Filename: caillou-0.0.7.dist-info/LICENSE
 Comment: 
 
-Filename: caillou-0.0.6.dist-info/METADATA
+Filename: caillou-0.0.7.dist-info/METADATA
 Comment: 
 
-Filename: caillou-0.0.6.dist-info/WHEEL
+Filename: caillou-0.0.7.dist-info/WHEEL
 Comment: 
 
-Filename: caillou-0.0.6.dist-info/entry_points.txt
+Filename: caillou-0.0.7.dist-info/entry_points.txt
 Comment: 
 
-Filename: caillou-0.0.6.dist-info/RECORD
+Filename: caillou-0.0.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `caillou-0.0.6.dist-info/LICENSE` & `caillou-0.0.7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `caillou-0.0.6.dist-info/METADATA` & `caillou-0.0.7.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caillou
-Version: 0.0.6
+Version: 0.0.7
 Summary: AI-powered toolbox for the terminal
 Home-page: https://github.com/sdudoit/caillou
 License: GPLv3
 Author: Sylvain
 Author-email: sdudoit@proton.me
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 3 - Alpha
```

## Comparing `caillou-0.0.6.dist-info/RECORD` & `caillou-0.0.7.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -2,12 +2,12 @@
 caillou/__main__.py,sha256=EHovA5Z4pP3JIGQLwGXor7MFr2Yi5Zj98_sKZg69ixI,256
 caillou/apps/__init__.py,sha256=XQKUn3kMmOJWNYWkKe-z_NehiXNKiAIWoKz11Ml-MUA,25
 caillou/apps/translator/__main__.py,sha256=v5tMHct08zZiGGpIcoLe5mD1IeTIt98_Lv9TATxeguE,3544
 caillou/apps/translator/languages.json,sha256=urEt0uj-zF70kedcRTANWD-2KQ_FOvB5euGj_6LlStk,15743
 caillou/apps/translator/styles.tcss,sha256=md09QGWOk3GBw44_hKCRTt2B9bTU7crpNC8zF6vMAiI,292
 caillou/config.py,sha256=uhd3wJWtdkCSvsXDtA0dVn-_w8pikcOPUOSMNCsE_wU,1957
 caillou/translate.py,sha256=rLn6y5lFHECd-TB0LQ5giOC-PifZsU4VOEK7-Z5yHAA,1689
-caillou-0.0.6.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
-caillou-0.0.6.dist-info/METADATA,sha256=uI2ILk-FrTefM_t7ZM4G4xJLg_HzqrqB7YyPwiOhoaQ,1685
-caillou-0.0.6.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
-caillou-0.0.6.dist-info/entry_points.txt,sha256=wM8bpx5q9aVcvwpMOx0WN7muwT3f8UfrS9-XnN1VgL0,49
-caillou-0.0.6.dist-info/RECORD,,
+caillou-0.0.7.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
+caillou-0.0.7.dist-info/METADATA,sha256=9uXdDDrGv_j0H0b6xMBi0Ahlddk0tHRb85_Aq5uQV-4,1685
+caillou-0.0.7.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
+caillou-0.0.7.dist-info/entry_points.txt,sha256=wM8bpx5q9aVcvwpMOx0WN7muwT3f8UfrS9-XnN1VgL0,49
+caillou-0.0.7.dist-info/RECORD,,
```

