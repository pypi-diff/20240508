# Comparing `tmp/juice_segmentation-0.6.6-py3-none-any.whl.zip` & `tmp/juice_segmentation-0.6.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 127549 bytes, number of entries: 62
--rw-r--r--  2.0 unx       18 b- defN 24-May-07 08:28 juice_segmentation/__init__.py
+Zip file size: 128194 bytes, number of entries: 62
+-rw-r--r--  2.0 unx       18 b- defN 24-May-08 09:39 juice_segmentation/__init__.py
 -rw-r--r--  2.0 unx     5029 b- defN 24-May-07 07:24 juice_segmentation/juice_segmentation_multi_cmd.py
 -rw-r--r--  2.0 unx     4820 b- defN 24-May-07 07:24 juice_segmentation/spice_segmentation_cmd.py
 -rw-r--r--  2.0 unx        0 b- defN 24-May-07 07:24 juice_segmentation/commons/__init__.py
 -rw-r--r--  2.0 unx      928 b- defN 24-May-07 07:24 juice_segmentation/commons/authentication.py
 -rw-r--r--  2.0 unx     3402 b- defN 24-May-07 07:24 juice_segmentation/commons/mission_phases.py
 -rw-r--r--  2.0 unx     4385 b- defN 24-May-07 07:24 juice_segmentation/commons/mission_timeline_event_file_handler.py
 -rw-r--r--  2.0 unx     1997 b- defN 24-May-07 07:24 juice_segmentation/commons/rest_api.py
@@ -52,13 +52,13 @@
 -rw-r--r--  2.0 unx     9714 b- defN 24-May-07 07:24 test/test_e2e_segmentation_schedule_minimum_allowed_dl.py
 -rw-r--r--  2.0 unx     7637 b- defN 24-May-07 07:24 test/test_e2e_segmentation_schedule_minor_moons.py
 -rw-r--r--  2.0 unx     3318 b- defN 24-May-07 07:24 test/test_e2e_spice_segmentation.py
 -rw-r--r--  2.0 unx     1743 b- defN 24-May-07 07:24 test/test_mission_timeline_event_file_handler.py
 -rw-r--r--  2.0 unx     1038 b- defN 24-May-07 07:24 test/test_post_new_plan.py
 -rw-r--r--  2.0 unx     1348 b- defN 24-May-07 07:24 test/test_rest_api.py
 -rw-r--r--  2.0 unx      904 b- defN 24-May-07 07:24 test/test_segment_definition_handler.py
--rw-r--r--  2.0 unx      690 b- defN 24-May-08 08:51 juice_segmentation-0.6.6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-08 08:51 juice_segmentation-0.6.6.dist-info/WHEEL
--rw-r--r--  2.0 unx      172 b- defN 24-May-08 08:51 juice_segmentation-0.6.6.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       24 b- defN 24-May-08 08:51 juice_segmentation-0.6.6.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     6300 b- defN 24-May-08 08:51 juice_segmentation-0.6.6.dist-info/RECORD
-62 files, 545766 bytes uncompressed, 117131 bytes compressed:  78.5%
+-rw-r--r--  2.0 unx     2208 b- defN 24-May-08 13:16 juice_segmentation-0.6.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-08 13:16 juice_segmentation-0.6.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx      172 b- defN 24-May-08 13:16 juice_segmentation-0.6.7.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       24 b- defN 24-May-08 13:16 juice_segmentation-0.6.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     6301 b- defN 24-May-08 13:16 juice_segmentation-0.6.7.dist-info/RECORD
+62 files, 547285 bytes uncompressed, 117776 bytes compressed:  78.5%
```

## zipnote {}

```diff
@@ -165,23 +165,23 @@
 
 Filename: test/test_rest_api.py
 Comment: 
 
 Filename: test/test_segment_definition_handler.py
 Comment: 
 
-Filename: juice_segmentation-0.6.6.dist-info/METADATA
+Filename: juice_segmentation-0.6.7.dist-info/METADATA
 Comment: 
 
-Filename: juice_segmentation-0.6.6.dist-info/WHEEL
+Filename: juice_segmentation-0.6.7.dist-info/WHEEL
 Comment: 
 
-Filename: juice_segmentation-0.6.6.dist-info/entry_points.txt
+Filename: juice_segmentation-0.6.7.dist-info/entry_points.txt
 Comment: 
 
-Filename: juice_segmentation-0.6.6.dist-info/top_level.txt
+Filename: juice_segmentation-0.6.7.dist-info/top_level.txt
 Comment: 
 
-Filename: juice_segmentation-0.6.6.dist-info/RECORD
+Filename: juice_segmentation-0.6.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## juice_segmentation/__init__.py

```diff
@@ -1 +1 @@
-version = "0.6.6"
+version = "0.6.7"
```

## Comparing `juice_segmentation-0.6.6.dist-info/RECORD` & `juice_segmentation-0.6.7.dist-info/RECORD`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-juice_segmentation/__init__.py,sha256=1rCEct6O4bN-9NvsTgwjU_6L8F42w6J4Vl0NJ-4nIcY,18
+juice_segmentation/__init__.py,sha256=2VRvyMb7pcj_Edl5NT9wbRJSFEq1UBe6Fkn_Ebw0L6Y,18
 juice_segmentation/juice_segmentation_multi_cmd.py,sha256=GA8F3jdMAOWCpDmEjOi-hVv1Dojvon_AvilVA2ugjMA,5029
 juice_segmentation/spice_segmentation_cmd.py,sha256=K48nej6Zv6aOHrEfU28REwj00NwpFzhrh0lJhm0gcUA,4820
 juice_segmentation/commons/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 juice_segmentation/commons/authentication.py,sha256=9QVw53iUF9aI5k9EZnieoTCJuIdtD6uxT4s5wO9Q4yE,928
 juice_segmentation/commons/mission_phases.py,sha256=Kbmt1oMmT5Iv9H0Y3ySE5WimpHLVaBotzcC58BZXDeo,3402
 juice_segmentation/commons/mission_timeline_event_file_handler.py,sha256=Y8ym6usL0v55x8waeK9PpRuUTDVrYoJsukIXY_j9q6g,4385
 juice_segmentation/commons/rest_api.py,sha256=ClC7rmDDzWGqN3KVLf9klSqA6-E2TOYQ7LC2UHpmsFY,1997
@@ -51,12 +51,12 @@
 test/test_e2e_segmentation_schedule_minimum_allowed_dl.py,sha256=9SC2hKlnwYYq6AxKPmaFLaWHNcqebZIOPxoXK29uQxU,9714
 test/test_e2e_segmentation_schedule_minor_moons.py,sha256=NwGGLJINzFNTVR_tAvCtVEiJcOigWQ3mGJaJTN7oR9A,7637
 test/test_e2e_spice_segmentation.py,sha256=wEdJkFdpi48tHfPBpeXAIGzqJ1S3yWsqIvHUfCGnTRg,3318
 test/test_mission_timeline_event_file_handler.py,sha256=bxVl95Iex5VzY18OyxcB0wGZggAYUTXv3zPeUNAznCs,1743
 test/test_post_new_plan.py,sha256=7WigtrbNcBUQ26niWJ9ONHbqniF3TTux9vmGBK0I1QY,1038
 test/test_rest_api.py,sha256=BawNLdCMDqPLFCt_eaPOKYboEaUB1J8bH4zlN-KC0BQ,1348
 test/test_segment_definition_handler.py,sha256=JOW3yRn_N4u2DjyaFBL970G8bi4x6iLO5T36UEimVjU,904
-juice_segmentation-0.6.6.dist-info/METADATA,sha256=dk5s7QdCXSrG0ILmCXbiseZioU-wa3O5eU4_vf1fNEs,690
-juice_segmentation-0.6.6.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-juice_segmentation-0.6.6.dist-info/entry_points.txt,sha256=29RrjGYfU2579fQovQ3e3cgbofPJqDODRvgNzhBpT4Q,172
-juice_segmentation-0.6.6.dist-info/top_level.txt,sha256=6QQJSxdaHumYJS3_cnNtLjj4QSRfKRlYY6da_G8ouAI,24
-juice_segmentation-0.6.6.dist-info/RECORD,,
+juice_segmentation-0.6.7.dist-info/METADATA,sha256=b6abhH2MSmq163WD1oOovOEeBVNKeNcXdeXcfG_59gU,2208
+juice_segmentation-0.6.7.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+juice_segmentation-0.6.7.dist-info/entry_points.txt,sha256=29RrjGYfU2579fQovQ3e3cgbofPJqDODRvgNzhBpT4Q,172
+juice_segmentation-0.6.7.dist-info/top_level.txt,sha256=6QQJSxdaHumYJS3_cnNtLjj4QSRfKRlYY6da_G8ouAI,24
+juice_segmentation-0.6.7.dist-info/RECORD,,
```

