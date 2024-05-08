# Comparing `tmp/bia_explorer-0.1.3.tar.gz` & `tmp/bia_explorer-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bia_explorer-0.1.3.tar", max compression
+gzip compressed data, was "bia_explorer-0.1.4.tar", max compression
```

## Comparing `bia_explorer-0.1.3.tar` & `bia_explorer-0.1.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       22 2024-04-03 15:51:29.515817 bia_explorer-0.1.3/bia_explorer/__init__.py
--rw-r--r--   0        0        0    13527 2024-04-22 11:17:46.539466 bia_explorer-0.1.3/bia_explorer/api.py
--rw-r--r--   0        0        0     5155 2024-04-05 08:40:37.342221 bia_explorer-0.1.3/bia_explorer/biostudies.py
--rw-r--r--   0        0        0     1874 2024-04-10 10:13:37.573253 bia_explorer-0.1.3/bia_explorer/io.py
--rw-r--r--   0        0        0     1212 2024-04-03 15:51:29.515817 bia_explorer-0.1.3/bia_explorer/models.py
--rw-r--r--   0        0        0      293 2024-04-03 15:51:29.519816 bia_explorer-0.1.3/bia_explorer/utils.py
--rw-r--r--   0        0        0      732 2024-04-19 15:26:04.318164 bia_explorer-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      891 1970-01-01 00:00:00.000000 bia_explorer-0.1.3/setup.py
--rw-r--r--   0        0        0      882 1970-01-01 00:00:00.000000 bia_explorer-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0       22 2024-04-03 15:51:29.515817 bia_explorer-0.1.4/bia_explorer/__init__.py
+-rw-r--r--   0        0        0    15177 2024-05-03 13:46:07.052056 bia_explorer-0.1.4/bia_explorer/api.py
+-rw-r--r--   0        0        0     5155 2024-04-05 08:40:37.342221 bia_explorer-0.1.4/bia_explorer/biostudies.py
+-rw-r--r--   0        0        0     1874 2024-04-10 10:13:37.573253 bia_explorer-0.1.4/bia_explorer/io.py
+-rw-r--r--   0        0        0     1212 2024-04-03 15:51:29.515817 bia_explorer-0.1.4/bia_explorer/models.py
+-rw-r--r--   0        0        0      293 2024-04-03 15:51:29.519816 bia_explorer-0.1.4/bia_explorer/utils.py
+-rw-r--r--   0        0        0      710 2024-05-08 12:45:27.763694 bia_explorer-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      862 1970-01-01 00:00:00.000000 bia_explorer-0.1.4/setup.py
+-rw-r--r--   0        0        0      839 1970-01-01 00:00:00.000000 bia_explorer-0.1.4/PKG-INFO
```

### Comparing `bia_explorer-0.1.3/bia_explorer/api.py` & `bia_explorer-0.1.4/bia_explorer/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,23 +9,43 @@
 from bia_integrator_api.util import get_client
 import bia_integrator_api.models as api_models
 
 from collections.abc import Iterator
 from typing import Optional, List
 from pydantic import BaseModel
 
-import matplotlib.pyplot as plt
-
 import dask.array as da
 import zarr
 import numpy as np
 from ome_zarr.io import parse_url
 from ome_zarr.reader import Reader
 
 class ReprHtmlMixin(BaseModel):
+    _include_fields: List[str] = [
+        "context",
+        "uuid",
+        "title",
+        "description",
+        "authors",
+        "name",
+        "organism",
+        "release_date",
+        "accession_id",
+        "imaging_type",
+        "file_references_count",
+        "images_count",
+        "study_uuid",
+        "original_relpath",
+        "dimensions",
+        "representations",
+        "uri",
+        "size",
+        "type"
+    ]
+
     def repr_html_embed_image(self) -> Optional[str]:
         """
         Override by children that support sample images (e.g. representative image, or thumbnail) 
         """
         return 
 
     def _repr_html_(self) -> str:
@@ -46,14 +66,17 @@
             list_html += "</table>"
             return list_html
 
         def dict_to_html_table(obj_comp):
             dict_html = "<table>"
             
             for k, v in obj_comp.items():
+                if k not in self._include_fields:
+                    continue
+
                 dict_html += "<tr>"
                 dict_html += f"<td>{k}</td>"
                 dict_html += f"<td>{primitive_to_html(v)}</td>"
                 dict_html += "</tr>"
 
             dict_html += "</table>"
             return dict_html
@@ -163,15 +186,19 @@
     c: Optional[int] = None
     x: Optional[int] = None
     y: Optional[int] = None
     z: Optional[int] = None
     t: Optional[int] = None
 
     def as_tuple(self):
-        # ?!
+        """
+        For numpy array slices from ImageSlice instances.
+        Keep in mind that this *doesn't include any notion of data dimensions*,
+            it just maps a human-friendly way of expressing slices into a fixed-order tuple, independent of the dimension order in the actual data
+        """
         return (self.c, self.z, self.t)
         
 class BIAImageRepresentation(api_models.BIAImageRepresentation, ReprHtmlMixin):
     """
     ! No representation-image link
     """
     def ome_ngff_to_dask_array(self):
@@ -195,38 +222,53 @@
         if max_size_bytes and file_size > max_size_bytes:
             raise Exception(f"File size {file_size} over the maximum limit of {max_size_bytes}. Pass a higher max_size_bytes (or None to disable) if your machine has enough memory")
 
         data_request = requests.get(self.uri[0])
         assert data_request.status_code == 200
 
         img = BytesIO(data_request.content)
-        return Image.open(img)
+        return img
 
     def to_dask_array(self):
         if self.type == ImageRepresentationType.OME_NGFF.value:
             return self.ome_ngff_to_dask_array()
         elif self.type == ImageRepresentationType.OME_ZARR_ZIPPED.value:
             return self.zipped_zarr_to_dask_array()
         else:
             raise Exception(f"No automatic display supported for representation of type {self.type} at '{self.uri[0]}'")
 
-    def pyplot_display_slice(self, image_slice: Optional[ImageSlice] = None):
+    def get_slice_image(self, image_slice: Optional[ImageSlice] = None, img_h = 512, img_w = None) -> Image:
         if image_slice is None:
             # @TODO: Make "default slice" some function of the actual darray 
             image_slice = ImageSlice(c=0,t=0,z=0)
 
         slice_tuple = image_slice.as_tuple()
         img_as_darray = self.to_dask_array()
         slice_to_display = img_as_darray[slice_tuple].compute()
         if len(np.shape(slice_to_display)) != 2:
+            # This also guarantees all images are greyscale (they probably aren't in practice)
             raise Exception(f"Unable to display slice of shape {np.shape(slice_to_display)}. xy plane required")
 
-        plt.imshow(slice_to_display, cmap='gray')
-        plt.axis('off')
-        plt.show()
+        max_dimension_size = 5000
+        if np.shape(slice_to_display)[0] > max_dimension_size or np.shape(slice_to_display)[1] > max_dimension_size:
+            raise Exception(f"Trying to display a {np.shape(slice_to_display)} plane. Consider manual data manipulation and rendering for planes larger than ({max_dimension_size}, {max_dimension_size})")
+
+        # len(np.shape(slice_to_display)) == 2 -> greyscale
+        img = Image.fromarray(slice_to_display, 'L')
+        if not img_h and not img_w:
+            # no resizing
+            return img
+        else:
+            # if any target dimension is None, keep aspect ratio
+            if not img_w:
+                img_w = img.height*img_h // img.width
+            if not img_h:
+                img_h = img.width*img_w // img.height
+
+            return img.resize((img_h, img_w))
 
 class FileReference(api_models.FileReference, ReprHtmlMixin):
     def get_study(self) -> BIAStudy:
         return ApiClient.get_study_by_uuid(self.study_uuid)
 
 class ImageAcquisition(api_models.ImageAcquisition, ReprHtmlMixin):
     pass
```

### Comparing `bia_explorer-0.1.3/bia_explorer/biostudies.py` & `bia_explorer-0.1.4/bia_explorer/biostudies.py`

 * *Files identical despite different names*

### Comparing `bia_explorer-0.1.3/bia_explorer/io.py` & `bia_explorer-0.1.4/bia_explorer/io.py`

 * *Files identical despite different names*

### Comparing `bia_explorer-0.1.3/bia_explorer/models.py` & `bia_explorer-0.1.4/bia_explorer/models.py`

 * *Files identical despite different names*

### Comparing `bia_explorer-0.1.3/pyproject.toml` & `bia_explorer-0.1.4/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 [tool.poetry]
 name = "bia-explorer"
 # managed by poetry-version-plugin
-version = "000"
+version = "0.1"
 description = ""
 authors = ["Matthew Hartley <matthewh@ebi.ac.uk>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 requests = "^2.28.1"
 pydantic = "^1.10.2"
 Pillow = "^9.3.0"
-bia-integrator-api = "^0.2.0"
+bia-integrator-api = "^0.3.0"
 dask = "^2024.4.1"
 zarr = "^2.17.2"
-matplotlib = "^3.8.4"
 jupyter = "^1.0.0"
+ome-zarr = "^0.8.3"
 # Transitive dependeices from upstream projects,
 #   useful to bound to make poetry install faster
 aiobotocore = "^2.0.0"
 s3fs = "^2024.0.0"
-ome-zarr = "^0.8.3"
 
 [tool.poetry.dev-dependencies]
 pytest = "^5.2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `bia_explorer-0.1.3/setup.py` & `bia_explorer-0.1.4/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,27 +6,26 @@
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['Pillow>=9.3.0,<10.0.0',
  'aiobotocore>=2.0.0,<3.0.0',
- 'bia-integrator-api>=0.2.0,<0.3.0',
+ 'bia-integrator-api>=0.3.0,<0.4.0',
  'dask>=2024.4.1,<2025.0.0',
  'jupyter>=1.0.0,<2.0.0',
- 'matplotlib>=3.8.4,<4.0.0',
  'ome-zarr>=0.8.3,<0.9.0',
  'pydantic>=1.10.2,<2.0.0',
  'requests>=2.28.1,<3.0.0',
  's3fs>=2024.0.0,<2025.0.0',
  'zarr>=2.17.2,<3.0.0']
 
 setup_kwargs = {
     'name': 'bia-explorer',
-    'version': '0.1.3',
+    'version': '0.1.4',
     'description': '',
     'long_description': 'None',
     'author': 'Matthew Hartley',
     'author_email': 'matthewh@ebi.ac.uk',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `bia_explorer-0.1.3/PKG-INFO` & `bia_explorer-0.1.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: bia-explorer
-Version: 0.1.3
+Version: 0.1.4
 Summary: 
 License: MIT
 Author: Matthew Hartley
 Author-email: matthewh@ebi.ac.uk
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Pillow (>=9.3.0,<10.0.0)
 Requires-Dist: aiobotocore (>=2.0.0,<3.0.0)
-Requires-Dist: bia-integrator-api (>=0.2.0,<0.3.0)
+Requires-Dist: bia-integrator-api (>=0.3.0,<0.4.0)
 Requires-Dist: dask (>=2024.4.1,<2025.0.0)
 Requires-Dist: jupyter (>=1.0.0,<2.0.0)
-Requires-Dist: matplotlib (>=3.8.4,<4.0.0)
 Requires-Dist: ome-zarr (>=0.8.3,<0.9.0)
 Requires-Dist: pydantic (>=1.10.2,<2.0.0)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
 Requires-Dist: s3fs (>=2024.0.0,<2025.0.0)
 Requires-Dist: zarr (>=2.17.2,<3.0.0)
```

