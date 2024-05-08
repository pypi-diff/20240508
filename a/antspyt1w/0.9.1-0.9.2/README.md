# Comparing `tmp/antspyt1w-0.9.1.tar.gz` & `tmp/antspyt1w-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "antspyt1w-0.9.1.tar", last modified: Wed Jan 24 13:27:04 2024, max compression
+gzip compressed data, was "antspyt1w-0.9.2.tar", last modified: Wed May  8 13:23:01 2024, max compression
```

## Comparing `antspyt1w-0.9.1.tar` & `antspyt1w-0.9.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 stnava     (501) staff       (20)        0 2024-01-24 13:27:04.802931 antspyt1w-0.9.1/
-drwxr-xr-x   0 stnava     (501) staff       (20)        0 2024-01-24 13:27:04.799473 antspyt1w-0.9.1/.circleci/
--rw-r--r--   0 stnava     (501) staff       (20)      760 2021-12-05 18:20:06.000000 antspyt1w-0.9.1/.circleci/config.yml
--rw-r--r--   0 stnava     (501) staff       (20)     1924 2021-11-17 22:27:29.000000 antspyt1w-0.9.1/.gitignore
--rw-r--r--   0 stnava     (501) staff       (20)      119 2021-11-17 22:27:29.000000 antspyt1w-0.9.1/.gitmodules
--rw-r--r--   0 stnava     (501) staff       (20)      519 2021-11-17 22:27:29.000000 antspyt1w-0.9.1/Dockerfile
--rw-r--r--   0 stnava     (501) staff       (20)    11357 2021-11-17 22:27:29.000000 antspyt1w-0.9.1/LICENSE
--rw-r--r--   0 stnava     (501) staff       (20)     3409 2024-01-24 13:27:04.802809 antspyt1w-0.9.1/PKG-INFO
--rw-r--r--   0 stnava     (501) staff       (20)     3078 2023-12-14 01:09:11.000000 antspyt1w-0.9.1/README.md
-drwxr-xr-x   0 stnava     (501) staff       (20)        0 2024-01-24 13:27:04.799961 antspyt1w-0.9.1/antspyt1w/
--rw-r--r--   0 stnava     (501) staff       (20)     1573 2023-03-14 13:16:41.000000 antspyt1w-0.9.1/antspyt1w/__init__.py
--rw-r--r--   0 stnava     (501) staff       (20)   134161 2024-01-24 13:24:01.000000 antspyt1w-0.9.1/antspyt1w/get_data.py
-drwxr-xr-x   0 stnava     (501) staff       (20)        0 2024-01-24 13:27:04.800747 antspyt1w-0.9.1/antspyt1w.egg-info/
--rw-r--r--   0 stnava     (501) staff       (20)     3409 2024-01-24 13:27:04.000000 antspyt1w-0.9.1/antspyt1w.egg-info/PKG-INFO
--rw-r--r--   0 stnava     (501) staff       (20)      471 2024-01-24 13:27:04.000000 antspyt1w-0.9.1/antspyt1w.egg-info/SOURCES.txt
--rw-r--r--   0 stnava     (501) staff       (20)        1 2024-01-24 13:27:04.000000 antspyt1w-0.9.1/antspyt1w.egg-info/dependency_links.txt
--rw-r--r--   0 stnava     (501) staff       (20)        1 2022-10-05 13:41:34.000000 antspyt1w-0.9.1/antspyt1w.egg-info/not-zip-safe
--rw-r--r--   0 stnava     (501) staff       (20)       10 2024-01-24 13:27:04.000000 antspyt1w-0.9.1/antspyt1w.egg-info/top_level.txt
-drwxr-xr-x   0 stnava     (501) staff       (20)        0 2024-01-24 13:27:04.800897 antspyt1w-0.9.1/docs/
--rw-r--r--   0 stnava     (501) staff       (20)   103244 2023-05-15 15:46:35.000000 antspyt1w-0.9.1/docs/antspyt1w_data_dictionary.csv
--rw-r--r--   0 stnava     (501) staff       (20)      133 2022-01-13 15:53:02.000000 antspyt1w-0.9.1/requirements.txt
--rw-r--r--   0 stnava     (501) staff       (20)       38 2024-01-24 13:27:04.802975 antspyt1w-0.9.1/setup.cfg
--rw-r--r--   0 stnava     (501) staff       (20)      522 2024-01-24 13:26:26.000000 antspyt1w-0.9.1/setup.py
-drwxr-xr-x   0 stnava     (501) staff       (20)        0 2024-01-24 13:27:04.802600 antspyt1w-0.9.1/tests/
--rw-r--r--   0 stnava     (501) staff       (20)      987 2022-03-11 22:33:25.000000 antspyt1w-0.9.1/tests/test_deep_hipp.py
--rw-r--r--   0 stnava     (501) staff       (20)      948 2022-03-12 15:08:32.000000 antspyt1w-0.9.1/tests/test_mtl.py
--rw-r--r--   0 stnava     (501) staff       (20)      675 2022-01-11 18:52:31.000000 antspyt1w-0.9.1/tests/test_rbp.py
--rw-r--r--   0 stnava     (501) staff       (20)     1382 2022-03-18 13:56:41.000000 antspyt1w-0.9.1/tests/test_reference_run.py
--rw-r--r--   0 stnava     (501) staff       (20)      541 2022-01-09 15:31:19.000000 antspyt1w-0.9.1/tests/test_tissueseg.py
--rw-r--r--   0 stnava     (501) staff       (20)     1143 2022-01-04 12:49:35.000000 antspyt1w-0.9.1/tests/test_wmh.py
+drwxr-xr-x   0 stnava     (501) staff       (20)        0 2024-05-08 13:23:01.601569 antspyt1w-0.9.2/
+drwxr-xr-x   0 stnava     (501) staff       (20)        0 2024-05-08 13:23:01.597228 antspyt1w-0.9.2/.circleci/
+-rw-r--r--   0 stnava     (501) staff       (20)      760 2021-12-05 18:20:06.000000 antspyt1w-0.9.2/.circleci/config.yml
+-rw-r--r--   0 stnava     (501) staff       (20)     1924 2021-11-17 22:27:29.000000 antspyt1w-0.9.2/.gitignore
+-rw-r--r--   0 stnava     (501) staff       (20)      119 2021-11-17 22:27:29.000000 antspyt1w-0.9.2/.gitmodules
+-rw-r--r--   0 stnava     (501) staff       (20)      519 2021-11-17 22:27:29.000000 antspyt1w-0.9.2/Dockerfile
+-rw-r--r--   0 stnava     (501) staff       (20)    11357 2021-11-17 22:27:29.000000 antspyt1w-0.9.2/LICENSE
+-rw-r--r--   0 stnava     (501) staff       (20)     3409 2024-05-08 13:23:01.601263 antspyt1w-0.9.2/PKG-INFO
+-rw-r--r--   0 stnava     (501) staff       (20)     3078 2023-12-14 01:09:11.000000 antspyt1w-0.9.2/README.md
+drwxr-xr-x   0 stnava     (501) staff       (20)        0 2024-05-08 13:23:01.597831 antspyt1w-0.9.2/antspyt1w/
+-rw-r--r--   0 stnava     (501) staff       (20)     1573 2023-03-14 13:16:41.000000 antspyt1w-0.9.2/antspyt1w/__init__.py
+-rw-r--r--   0 stnava     (501) staff       (20)   134414 2024-05-08 13:17:46.000000 antspyt1w-0.9.2/antspyt1w/get_data.py
+drwxr-xr-x   0 stnava     (501) staff       (20)        0 2024-05-08 13:23:01.600932 antspyt1w-0.9.2/antspyt1w.egg-info/
+-rw-r--r--   0 stnava     (501) staff       (20)     3409 2024-05-08 13:23:01.000000 antspyt1w-0.9.2/antspyt1w.egg-info/PKG-INFO
+-rw-r--r--   0 stnava     (501) staff       (20)      471 2024-05-08 13:23:01.000000 antspyt1w-0.9.2/antspyt1w.egg-info/SOURCES.txt
+-rw-r--r--   0 stnava     (501) staff       (20)        1 2024-05-08 13:23:01.000000 antspyt1w-0.9.2/antspyt1w.egg-info/dependency_links.txt
+-rw-r--r--   0 stnava     (501) staff       (20)        1 2022-10-05 13:41:34.000000 antspyt1w-0.9.2/antspyt1w.egg-info/not-zip-safe
+-rw-r--r--   0 stnava     (501) staff       (20)       10 2024-05-08 13:23:01.000000 antspyt1w-0.9.2/antspyt1w.egg-info/top_level.txt
+drwxr-xr-x   0 stnava     (501) staff       (20)        0 2024-05-08 13:23:01.598967 antspyt1w-0.9.2/docs/
+-rw-r--r--   0 stnava     (501) staff       (20)   103244 2023-05-15 15:46:35.000000 antspyt1w-0.9.2/docs/antspyt1w_data_dictionary.csv
+-rw-r--r--   0 stnava     (501) staff       (20)      133 2022-01-13 15:53:02.000000 antspyt1w-0.9.2/requirements.txt
+-rw-r--r--   0 stnava     (501) staff       (20)       38 2024-05-08 13:23:01.601641 antspyt1w-0.9.2/setup.cfg
+-rw-r--r--   0 stnava     (501) staff       (20)      522 2024-05-08 13:09:59.000000 antspyt1w-0.9.2/setup.py
+drwxr-xr-x   0 stnava     (501) staff       (20)        0 2024-05-08 13:23:01.600686 antspyt1w-0.9.2/tests/
+-rw-r--r--   0 stnava     (501) staff       (20)      987 2022-03-11 22:33:25.000000 antspyt1w-0.9.2/tests/test_deep_hipp.py
+-rw-r--r--   0 stnava     (501) staff       (20)      948 2022-03-12 15:08:32.000000 antspyt1w-0.9.2/tests/test_mtl.py
+-rw-r--r--   0 stnava     (501) staff       (20)      675 2022-01-11 18:52:31.000000 antspyt1w-0.9.2/tests/test_rbp.py
+-rw-r--r--   0 stnava     (501) staff       (20)     1382 2022-03-18 13:56:41.000000 antspyt1w-0.9.2/tests/test_reference_run.py
+-rw-r--r--   0 stnava     (501) staff       (20)      541 2022-01-09 15:31:19.000000 antspyt1w-0.9.2/tests/test_tissueseg.py
+-rw-r--r--   0 stnava     (501) staff       (20)     1143 2022-01-04 12:49:35.000000 antspyt1w-0.9.2/tests/test_wmh.py
```

### Comparing `antspyt1w-0.9.1/.circleci/config.yml` & `antspyt1w-0.9.2/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `antspyt1w-0.9.1/.gitignore` & `antspyt1w-0.9.2/.gitignore`

 * *Files identical despite different names*

### Comparing `antspyt1w-0.9.1/Dockerfile` & `antspyt1w-0.9.2/Dockerfile`

 * *Files identical despite different names*

### Comparing `antspyt1w-0.9.1/LICENSE` & `antspyt1w-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `antspyt1w-0.9.1/PKG-INFO` & `antspyt1w-0.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antspyt1w
-Version: 0.9.1
+Version: 0.9.2
 Summary: T1w human neuroimage processing with antspyx
 Home-page: https://github.com/stnava/ANTsPyT1w
 Author: Avants, Gosselin, Tustison
 Author-email: stnava@gmail.com
 License: Apache 2.0
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 License-File: LICENSE
```

### Comparing `antspyt1w-0.9.1/README.md` & `antspyt1w-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `antspyt1w-0.9.1/antspyt1w/__init__.py` & `antspyt1w-0.9.2/antspyt1w/__init__.py`

 * *Files identical despite different names*

### Comparing `antspyt1w-0.9.1/antspyt1w/get_data.py` & `antspyt1w-0.9.2/antspyt1w/get_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -437,15 +437,15 @@
 
     if not exists( weights_filename ):
         print("resnet_grader weights do not exist: " + weights_filename )
         return None
 
     mdl = antspynet.create_resnet_model_3d( [None,None,None,1],
         lowest_resolution = 32,
-        number_of_classification_labels = 4,
+        number_of_outputs = 4,
         cardinality = 1,
         squeeze_and_excite = False )
     mdl.load_weights( weights_filename )
 
 
     t1 = ants.iMath( x - x.min(),  "Normalize" )
     bxt = ants.threshold_image( t1, 0.01, 1.0 )
@@ -567,16 +567,16 @@
         t1 = ants.rank_intensity( x * lomask, mask=lomask, get_mask=False )
         ants.plot( t1, axis=2, nslices=21, ncol=7, filename=pngfn, crop=True )
         rbp = random_basis_projection( t1, templatesmall,
             type_of_transform='Rigid',
             refbases=rbh )
         rbp.to_csv( csvfn )
         # fix up the figure
-        looper=float(rbp['loop_outlier_probability'])
-        ttl="LOOP: " + "{:0.4f}".format(looper) + " MD: " + "{:0.4f}".format(float(rbp['mhdist']))
+        looper=float(rbp['loop_outlier_probability'].iloc[0])
+        ttl="LOOP: " + "{:0.4f}".format(looper) + " MD: " + "{:0.4f}".format(float(rbp['mhdist'].iloc[0]))
         img = Image.open( pngfn ).copy()
         plt.figure(dpi=300)
         plt.imshow(img)
         plt.text(20, 0, ttl, color="red", fontsize=12 )
         plt.axis("off")
         plt.subplots_adjust(0,0,1,1)
         plt.savefig( pngfn, bbox_inches='tight',pad_inches = 0)
@@ -597,21 +597,28 @@
         templateb = ants.image_read( get_data( "S_template3_brain", target_extension='.nii.gz' ) )
         templatesmall = ants.resample_image( templateb, (2,2,2), use_voxels=False )
         rbpb = random_basis_projection( t1,
             templatesmall,
             type_of_transform='Rigid',
             refbases=rbb )
         rbpb['evratio'] = patch_eigenvalue_ratio( t1, 512, [20,20,20], evdepth = 0.9 )
-        rbpb['resnetGrade'] = resnet_grader( t1 ).gradeNum[0]
+        grade0 = resnet_grader( t1 ).gradeNum[0]
+        msk=ants.threshold_image(t1,0.01,1.0)
+        t1tx=ants.n4_bias_field_correction( t1, mask=msk )
+        t1tx=ants.iMath(t1tx,'TruncateIntensity',0.001,0.98)
+        grade1 = resnet_grader( t1tx ).gradeNum[0]
+        if grade1 > grade0:
+            grade0 = grade1
+        rbpb['resnetGrade'] = grade0
         rbpb.to_csv( csvfnb )
-        looper = float( rbpb['loop_outlier_probability'] )
-        myevr = float( rbpb['evratio'] )
-        mygrd = float( rbpb['resnetGrade'] )
-        myl1 = float( rbpb['templateL1'] )
-        ttl="LOOP: " + "{:0.4f}".format(looper) + " MD: " + "{:0.4f}".format(float(rbpb['mhdist'])) + " EVR: " + "{:0.4f}".format(myevr) + " TL1: " + "{:0.4f}".format(myl1) + " grade: " + "{:0.4f}".format(mygrd)
+        looper = float(rbpb['loop_outlier_probability'].iloc[0])
+        myevr = float( rbpb['evratio'].iloc[0] )
+        mygrd = float( rbpb['resnetGrade'].iloc[0] )
+        myl1 = float( rbpb['templateL1'].iloc[0] )
+        ttl="LOOP: " + "{:0.4f}".format(looper) + " MD: " + "{:0.4f}".format(float(rbpb['mhdist'].iloc[0])) + " EVR: " + "{:0.4f}".format(myevr) + " TL1: " + "{:0.4f}".format(myl1) + " grade: " + "{:0.4f}".format(mygrd)
         img = Image.open( pngfnb ).copy()
         plt.figure(dpi=300)
         plt.imshow(img)
         plt.text(20, 0, ttl, color="red", fontsize=12 )
         plt.axis("off")
         plt.subplots_adjust(0,0,1,1)
         plt.savefig( pngfnb, bbox_inches='tight',pad_inches = 0)
@@ -1693,15 +1700,15 @@
     pp = wmhunet.predict( myfeatures )
 
     limg = ants.from_numpy( tf.squeeze( pp[0] ).numpy( ) )
     limg = ants.copy_image_info( templatesmall, limg )
     lesresam = ants.apply_transforms( x, limg, afftx, whichtoinvert=[False] )
     # lesresam = lesresam * cerebrum
     rnmdl = antspynet.create_resnet_model_3d( inshape,
-      number_of_classification_labels = 1,
+      number_of_outputs = 1,
       layers = (1,2,3),
       residual_block_schedule = (3,4,6,3), squeeze_and_excite = True,
       lowest_resolution = 32, cardinality = 1, mode = "regression" )
     rnmdl.load_weights( get_data("simwmdisc", target_extension='.h5' ) )
     qq = rnmdl.predict( myfeatures )
 
     lesresamb = ants.threshold_image( lesresam, wmh_thresh, 1.0 )
@@ -1833,15 +1840,15 @@
             "segc": special_crop( imgseg, com, crop_size ),
             "reg" : reg,
             "mask": masker
             }
 
 
     nLabels = len( group_labels )
-    number_of_classification_labels = len(group_labels)
+    number_of_outputs = len(group_labels)
     number_of_channels = 1
     ################################################
     unet0 = antspynet.create_unet_model_3d(
          [ None, None, None, number_of_channels ],
          number_of_outputs = 1, # number of landmarks must be known
          number_of_layers = 4, # should optimize this wrt criterion
          number_of_filters_at_base_layer = 32, # should optimize this wrt criterion
@@ -1852,15 +1859,15 @@
          dropout_rate = 0.0,
          weight_decay = 0,
          additional_options = "nnUnetActivationStyle",
          mode =  "sigmoid" )
 
     unet1 = antspynet.create_unet_model_3d(
         [None,None,None,2],
-        number_of_outputs=number_of_classification_labels,
+        number_of_outputs=number_of_outputs,
         mode="classification",
         number_of_filters=(32, 64, 96, 128, 256),
         convolution_kernel_size=(3, 3, 3),
         deconvolution_kernel_size=(2, 2, 2),
         dropout_rate=0.0,
         weight_decay=0,
         additional_options = "nnUnetActivationStyle")
@@ -1902,15 +1909,15 @@
     segpred = snpred[0]
     sigmoidpred = snpred[1]
     snpred1_image = ants.from_numpy( sigmoidpred[0,:,:,:,0] )
     snpred1_image = ants.copy_image_info( physspaceBF, snpred1_image )
     snpred1_image = map_back( snpred1_image, t1, imgprepro, 'linear', deform )
     bint = ants.threshold_image( snpred1_image, 0.5, 1.0 )
     probability_images = []
-    for jj in range(number_of_classification_labels-1):
+    for jj in range(number_of_outputs-1):
                 temp = ants.from_numpy( segpred[0,:,:,:,jj+1] )
                 temp = ants.copy_image_info( physspaceBF, temp )
                 temp = map_back( temp, t1, imgprepro, 'linear', deform )
                 probability_images.append( temp )
     image_matrix = ants.image_list_to_matrix(probability_images, bint)
     segmentation_matrix = (np.argmax(image_matrix, axis=0) + 1)
     segmentation_image = ants.matrix_to_images(np.expand_dims(segmentation_matrix, axis=0), bint)[0]
@@ -2257,15 +2264,15 @@
         if sn:
             group_labels = [0,7,8,9,23,24,25,33,34]
             newfn=get_data( "deepCIT168_sn", target_extension=".h5" )
         else:
             group_labels = [0,1,2,5,6,17,18,21,22]
             newfn=get_data( "deepCIT168", target_extension=".h5" )
 
-        number_of_classification_labels = len(group_labels)
+        number_of_outputs = len(group_labels)
         number_of_channels = len(group_labels)
 
         unet0 = antspynet.create_unet_model_3d(
                  [ None, None, None, number_of_channels ],
                  number_of_outputs = 1, # number of landmarks must be known
                  number_of_layers = 4, # should optimize this wrt criterion
                  number_of_filters_at_base_layer = 32, # should optimize this wrt criterion
@@ -2276,15 +2283,15 @@
                  dropout_rate = 0.0,
                  weight_decay = 0,
                  additional_options = "nnUnetActivationStyle",
                  mode =  "sigmoid" )
 
         unet1 = antspynet.create_unet_model_3d(
             [None,None,None,2],
-            number_of_outputs=number_of_classification_labels,
+            number_of_outputs=number_of_outputs,
             mode="classification",
             number_of_filters=(32, 64, 96, 128, 256),
             convolution_kernel_size=(3, 3, 3),
             deconvolution_kernel_size=(2, 2, 2),
             dropout_rate=0.0,
             weight_decay=0,
             additional_options = "nnUnetActivationStyle")
```

### Comparing `antspyt1w-0.9.1/antspyt1w.egg-info/PKG-INFO` & `antspyt1w-0.9.2/antspyt1w.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antspyt1w
-Version: 0.9.1
+Version: 0.9.2
 Summary: T1w human neuroimage processing with antspyx
 Home-page: https://github.com/stnava/ANTsPyT1w
 Author: Avants, Gosselin, Tustison
 Author-email: stnava@gmail.com
 License: Apache 2.0
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 License-File: LICENSE
```

### Comparing `antspyt1w-0.9.1/docs/antspyt1w_data_dictionary.csv` & `antspyt1w-0.9.2/docs/antspyt1w_data_dictionary.csv`

 * *Files identical despite different names*

### Comparing `antspyt1w-0.9.1/setup.py` & `antspyt1w-0.9.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 from setuptools import setup
 
 long_description = open("README.md").read()
 
 setup(name='antspyt1w',
-      version='0.9.1',
+      version='0.9.2',
       description='T1w human neuroimage processing with antspyx',
       long_description=long_description,
       long_description_content_type="text/markdown; charset=UTF-8; variant=GFM",
       url='https://github.com/stnava/ANTsPyT1w',
       author='Avants, Gosselin, Tustison',
       author_email='stnava@gmail.com',
       license='Apache 2.0',
```

### Comparing `antspyt1w-0.9.1/tests/test_deep_hipp.py` & `antspyt1w-0.9.2/tests/test_deep_hipp.py`

 * *Files identical despite different names*

### Comparing `antspyt1w-0.9.1/tests/test_mtl.py` & `antspyt1w-0.9.2/tests/test_mtl.py`

 * *Files identical despite different names*

### Comparing `antspyt1w-0.9.1/tests/test_rbp.py` & `antspyt1w-0.9.2/tests/test_rbp.py`

 * *Files identical despite different names*

### Comparing `antspyt1w-0.9.1/tests/test_reference_run.py` & `antspyt1w-0.9.2/tests/test_reference_run.py`

 * *Files identical despite different names*

### Comparing `antspyt1w-0.9.1/tests/test_tissueseg.py` & `antspyt1w-0.9.2/tests/test_tissueseg.py`

 * *Files identical despite different names*

### Comparing `antspyt1w-0.9.1/tests/test_wmh.py` & `antspyt1w-0.9.2/tests/test_wmh.py`

 * *Files identical despite different names*

