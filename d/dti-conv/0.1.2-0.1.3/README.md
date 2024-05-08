# Comparing `tmp/dti_conv-0.1.2.tar.gz` & `tmp/dti_conv-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dti_conv-0.1.2.tar", max compression
+gzip compressed data, was "dti_conv-0.1.3.tar", max compression
```

## Comparing `dti_conv-0.1.2.tar` & `dti_conv-0.1.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     6148 2024-05-02 13:13:10.300400 dti_conv-0.1.2/dti_conv/.DS_Store
--rw-r--r--   0        0        0       47 2024-02-19 13:57:04.801804 dti_conv-0.1.2/dti_conv/.idea/.gitignore
--rw-r--r--   0        0        0      284 2024-02-19 13:57:04.696015 dti_conv-0.1.2/dti_conv/.idea/dti_conv.iml
--rw-r--r--   0        0        0      174 2024-02-19 13:57:04.706177 dti_conv-0.1.2/dti_conv/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0      276 2024-02-19 14:02:55.694187 dti_conv-0.1.2/dti_conv/.idea/misc.xml
--rw-r--r--   0        0        0      268 2024-02-19 13:57:04.699516 dti_conv-0.1.2/dti_conv/.idea/modules.xml
--rw-r--r--   0        0        0     1761 2024-02-19 14:07:48.875843 dti_conv-0.1.2/dti_conv/.idea/workspace.xml
--rw-r--r--   0        0        0        0 2023-12-01 01:24:28.364797 dti_conv-0.1.2/dti_conv/__init__.py
--rw-r--r--   0        0        0    26829 2024-04-30 01:28:26.240713 dti_conv-0.1.2/dti_conv/main.py
--rw-r--r--   0        0        0      635 2024-05-02 13:00:13.493247 dti_conv-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      912 1970-01-01 00:00:00.000000 dti_conv-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     6148 2024-05-07 23:16:36.231414 dti_conv-0.1.3/dti_conv/.DS_Store
+-rw-r--r--   0        0        0       47 2024-02-19 13:57:04.801804 dti_conv-0.1.3/dti_conv/.idea/.gitignore
+-rw-r--r--   0        0        0      284 2024-02-19 13:57:04.696015 dti_conv-0.1.3/dti_conv/.idea/dti_conv.iml
+-rw-r--r--   0        0        0      174 2024-02-19 13:57:04.706177 dti_conv-0.1.3/dti_conv/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0      276 2024-02-19 14:02:55.694187 dti_conv-0.1.3/dti_conv/.idea/misc.xml
+-rw-r--r--   0        0        0      268 2024-02-19 13:57:04.699516 dti_conv-0.1.3/dti_conv/.idea/modules.xml
+-rw-r--r--   0        0        0     1761 2024-02-19 14:07:48.875843 dti_conv-0.1.3/dti_conv/.idea/workspace.xml
+-rw-r--r--   0        0        0        0 2023-12-01 01:24:28.364797 dti_conv-0.1.3/dti_conv/__init__.py
+-rw-r--r--   0        0        0    28364 2024-05-08 21:12:43.999725 dti_conv-0.1.3/dti_conv/main.py
+-rw-r--r--   0        0        0      635 2024-05-08 21:19:05.217892 dti_conv-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      912 1970-01-01 00:00:00.000000 dti_conv-0.1.3/PKG-INFO
```

### Comparing `dti_conv-0.1.2/dti_conv/.idea/workspace.xml` & `dti_conv-0.1.3/dti_conv/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `dti_conv-0.1.2/dti_conv/main.py` & `dti_conv-0.1.3/dti_conv/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -101,38 +101,41 @@
 		print("Done")
 		plt.close()
 		print(self.SEPERATOR + "\n")
 
 	def getParameters(self):
 		questions = [iq.Checkbox('Saves',
 							message="What files do you want to save?",
-							choices=['Anatomy', 'FA', 'ADC', 'b0', "RD"],
+							choices=['Anatomy', 'FA', 'ADC', 'b0', "RD", "Lambda"],
 							),]
 		answers = iq.prompt(questions)
 		return answers["Saves"]
 
 	def parse_parameters(self):
 		parameters = self.getParameters()
 
 		self.bool_anatomy = False
 		self.bool_fa = False
 		self.bool_adc = False
 		self.bool_b0 = False
 		self.bool_rd = False
+		self.bool_lambda = False
 
 		if "Anatomy" in parameters:
 			self.bool_anatomy = True
 		if "FA" in parameters:
 			self.bool_fa = True
 		if "ADC" in parameters:
 			self.bool_adc = True
 		if "b0" in parameters:
 			self.bool_b0 = True
 		if "RD" in parameters:
 			self.bool_rd = True
+		if "Lambda" in parameters:
+			self.bool_lambda = True
 
 	def save_files(self):
 		for scan, numb in self.dti_instance.dti_scans.items():
 			OUTPUT_DIR = os.path.join(self.output_folder, os.path.basename(scan))
 			if numb:
 				if self.bool_fa or self.bool_adc or self.bool_b0:
 					for number in numb:
@@ -164,22 +167,55 @@
 							rd.header["pixdim"][2] = dim[1]
 							rd.header["pixdim"][3] = dim[2]
 							rd.header["pixdim"][4] = dim[3]
 							rd.set_data_dtype("<f4")
 							nib.save(rd, os.path.join(OUTPUT_DIR, os.path.basename(scan) + "_"+str(os.path.basename(number))+"_rd.nii"))
 							print("Saved " + os.path.join(OUTPUT_DIR, os.path.basename(scan) + "_"+str(os.path.basename(number))+"_rd.nii"))
 						if self.bool_adc:
-							md = nib.Nifti1Image(tenfit.md, None)
+							md = nib.Nifti1Image(tenfit.md*1000, None)
 							md.header["pixdim"][1] = dim[0]
 							md.header["pixdim"][2] = dim[1]
 							md.header["pixdim"][3] = dim[2]
 							md.header["pixdim"][4] = dim[3]
 							md.set_data_dtype("<f4")
 							nib.save(md, os.path.join(OUTPUT_DIR, os.path.basename(scan) + "_"+str(os.path.basename(number))+"_adc.nii"))
 							print("Saved " + os.path.join(OUTPUT_DIR, os.path.basename(scan) + "_"+str(os.path.basename(number))+"_adc.nii"))
+						if self.bool_lambda:
+							l1, l2, l3 = dti._roll_evals(tenfit.evals, -1)
+							l1 = l1*1000
+							l2 = l2*1000
+							l3 = l3*1000
+
+							l1 = nib.Nifti1Image(l1, None)
+							l2 = nib.Nifti1Image(l2, None)
+							l3 = nib.Nifti1Image(l3, None)
+
+							l1.header["pixdim"][1] = dim[0]
+							l1.header["pixdim"][2] = dim[1]
+							l1.header["pixdim"][3] = dim[2]
+							l2.header["pixdim"][1] = dim[0]
+							l2.header["pixdim"][2] = dim[1]
+							l2.header["pixdim"][3] = dim[2]
+							l3.header["pixdim"][1] = dim[0]
+							l3.header["pixdim"][2] = dim[1]
+							l3.header["pixdim"][3] = dim[2]
+
+							l1.set_data_dtype("<f4")
+							l2.set_data_dtype("<f4")
+							l3.set_data_dtype("<f4")
+
+							nib.save(l1, os.path.join(OUTPUT_DIR, os.path.basename(scan) + "_"+str(os.path.basename(number))+"_l1.nii"))
+							nib.save(l2, os.path.join(OUTPUT_DIR, os.path.basename(scan) + "_" + str(os.path.basename(number)) + "_l2.nii"))
+							nib.save(l3, os.path.join(OUTPUT_DIR, os.path.basename(scan) + "_" + str(os.path.basename(number)) + "_l3.nii"))
+
+							print("Saved " + os.path.join(OUTPUT_DIR, os.path.basename(scan) + "_" + str(os.path.basename(number)) + "_l1.nii"))
+							print("Saved " + os.path.join(OUTPUT_DIR, os.path.basename(scan) + "_" + str(os.path.basename(number)) + "_l2.nii"))
+							print("Saved " + os.path.join(OUTPUT_DIR, os.path.basename(scan) + "_" + str(os.path.basename(number)) + "_l3.nii"))
+
+
 				if self.bool_anatomy:
 					number = self.dti_instance.rare_scans[scan]
 					dim = self.dti_instance.getVoxelSize(number)
 					img_anat = self.dti_instance.rare_imgs[scan]
 					#nib.load(os.path.join(OUTPUT_DIR, os.path.basename(scan) + "_"+str(os.path.basename(number))+".nii"))
 					img_anat.header["pixdim"][1] = dim[0]
 					img_anat.header["pixdim"][2] = dim[1]
```

### Comparing `dti_conv-0.1.2/pyproject.toml` & `dti_conv-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dti-conv"
-version = "0.1.2"
+version = "0.1.3"
 description = "A command line utility that allows easy modifications on DWI volumes and Datasets."
 authors = ["AtulPhadke <atulphadke8@gmail.com>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 
 python = ">=3.9"
```

### Comparing `dti_conv-0.1.2/PKG-INFO` & `dti_conv-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dti-conv
-Version: 0.1.2
+Version: 0.1.3
 Summary: A command line utility that allows easy modifications on DWI volumes and Datasets.
 License: MIT
 Author: AtulPhadke
 Author-email: atulphadke8@gmail.com
 Requires-Python: >=3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

