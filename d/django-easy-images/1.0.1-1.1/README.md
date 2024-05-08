# Comparing `tmp/django_easy_images-1.0.1.tar.gz` & `tmp/django_easy_images-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_easy_images-1.0.1.tar", last modified: Tue Apr 23 20:53:08 2024, max compression
+gzip compressed data, was "django_easy_images-1.1.tar", last modified: Wed May  8 21:56:15 2024, max compression
```

## Comparing `django_easy_images-1.0.1.tar` & `django_easy_images-1.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     9392 2024-04-23 04:43:28.118599 django_easy_images-1.0.1/README.md
--rw-r--r--   0        0        0       36 2024-04-22 04:58:09.997777 django_easy_images-1.0.1/easy_images/__init__.py
--rw-r--r--   0        0        0      917 2024-04-22 04:58:09.984444 django_easy_images-1.0.1/easy_images/apps.py
--rw-r--r--   0        0        0    10068 2024-04-23 20:52:01.862392 django_easy_images-1.0.1/easy_images/core.py
--rw-r--r--   0        0        0     6339 2024-04-22 22:02:32.068649 django_easy_images-1.0.1/easy_images/engine.py
--rw-r--r--   0        0        0        0 2024-04-17 23:33:21.963652 django_easy_images-1.0.1/easy_images/management/__init__.py
--rw-r--r--   0        0        0        0 2024-04-17 23:33:21.963652 django_easy_images-1.0.1/easy_images/management/commands/__init__.py
--rw-r--r--   0        0        0     2342 2024-04-23 02:16:43.469563 django_easy_images-1.0.1/easy_images/management/commands/build_img_queue.py
--rw-r--r--   0        0        0      426 2024-04-23 02:00:56.360584 django_easy_images-1.0.1/easy_images/management/process_queue.py
--rw-r--r--   0        0        0     1853 2024-04-23 02:14:21.035863 django_easy_images-1.0.1/easy_images/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2024-04-17 23:33:21.963652 django_easy_images-1.0.1/easy_images/migrations/__init__.py
--rw-r--r--   0        0        0     5809 2024-04-23 20:45:20.687237 django_easy_images-1.0.1/easy_images/models.py
--rw-r--r--   0        0        0     5620 2024-04-17 23:33:21.966985 django_easy_images-1.0.1/easy_images/options.py
--rw-r--r--   0        0        0     1965 2024-04-23 20:47:23.464743 django_easy_images-1.0.1/easy_images/signals.py
--rw-r--r--   0        0        0        0 2024-04-17 23:33:21.963652 django_easy_images-1.0.1/easy_images/templatetags/__init__.py
--rw-r--r--   0        0        0     3020 2024-04-18 00:02:29.074991 django_easy_images-1.0.1/easy_images/templatetags/easy_images.py
--rw-r--r--   0        0        0     1239 2024-04-17 23:33:21.966985 django_easy_images-1.0.1/easy_images/types.py
--rw-r--r--   0        0        0     1363 2024-04-23 20:53:08.464592 django_easy_images-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      178 2024-04-23 03:16:24.712101 django_easy_images-1.0.1/tests/conftest.py
--rw-r--r--   0        0        0        0 2024-04-22 21:04:01.902198 django_easy_images-1.0.1/tests/easy_images_tests/__init__.py
--rw-r--r--   0        0        0      299 2024-04-22 21:06:20.262499 django_easy_images-1.0.1/tests/easy_images_tests/models.py
--rw-r--r--   0        0        0      410 2024-04-22 21:39:32.545263 django_easy_images-1.0.1/tests/settings.py
--rw-r--r--   0        0        0     3408 2024-04-23 02:28:25.564752 django_easy_images-1.0.1/tests/test_command.py
--rw-r--r--   0        0        0     1424 2024-04-17 23:33:25.980333 django_easy_images-1.0.1/tests/test_core.py
--rw-r--r--   0        0        0     1850 2024-04-17 23:33:25.980333 django_easy_images-1.0.1/tests/test_engine.py
--rw-r--r--   0        0        0     1036 2024-04-23 02:47:06.431022 django_easy_images-1.0.1/tests/test_models.py
--rw-r--r--   0        0        0     1257 2024-04-17 23:33:25.980333 django_easy_images-1.0.1/tests/test_options.py
--rw-r--r--   0        0        0     1333 2024-04-22 21:49:56.047786 django_easy_images-1.0.1/tests/test_signals.py
--rw-r--r--   0        0        0    10593 1970-01-01 00:00:00.000000 django_easy_images-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     9413 2024-04-23 21:48:34.323413 django_easy_images-1.1/README.md
+-rw-r--r--   0        0        0       36 2024-04-22 04:58:09.997777 django_easy_images-1.1/easy_images/__init__.py
+-rw-r--r--   0        0        0      917 2024-04-22 04:58:09.984444 django_easy_images-1.1/easy_images/apps.py
+-rw-r--r--   0        0        0    10068 2024-04-23 20:52:01.862392 django_easy_images-1.1/easy_images/core.py
+-rw-r--r--   0        0        0     6461 2024-05-08 21:53:02.355147 django_easy_images-1.1/easy_images/engine.py
+-rw-r--r--   0        0        0        0 2024-04-17 23:33:21.963652 django_easy_images-1.1/easy_images/management/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-17 23:33:21.963652 django_easy_images-1.1/easy_images/management/commands/__init__.py
+-rw-r--r--   0        0        0     5036 2024-04-23 21:46:16.614777 django_easy_images-1.1/easy_images/management/commands/build_img_queue.py
+-rw-r--r--   0        0        0     1069 2024-04-23 21:35:50.212790 django_easy_images-1.1/easy_images/management/process_queue.py
+-rw-r--r--   0        0        0     1853 2024-04-23 02:14:21.035863 django_easy_images-1.1/easy_images/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2024-04-17 23:33:21.963652 django_easy_images-1.1/easy_images/migrations/__init__.py
+-rw-r--r--   0        0        0     5809 2024-04-23 20:45:20.687237 django_easy_images-1.1/easy_images/models.py
+-rw-r--r--   0        0        0     5620 2024-04-17 23:33:21.966985 django_easy_images-1.1/easy_images/options.py
+-rw-r--r--   0        0        0     1965 2024-04-23 20:47:23.464743 django_easy_images-1.1/easy_images/signals.py
+-rw-r--r--   0        0        0        0 2024-04-17 23:33:21.963652 django_easy_images-1.1/easy_images/templatetags/__init__.py
+-rw-r--r--   0        0        0     3020 2024-04-18 00:02:29.074991 django_easy_images-1.1/easy_images/templatetags/easy_images.py
+-rw-r--r--   0        0        0     1239 2024-04-17 23:33:21.966985 django_easy_images-1.1/easy_images/types.py
+-rw-r--r--   0        0        0     1361 2024-05-08 21:56:15.425497 django_easy_images-1.1/pyproject.toml
+-rw-r--r--   0        0        0      221 2024-04-23 21:41:29.012679 django_easy_images-1.1/tests/conftest.py
+-rw-r--r--   0        0        0        0 2024-04-22 21:04:01.902198 django_easy_images-1.1/tests/easy_images_tests/__init__.py
+-rw-r--r--   0        0        0      299 2024-04-22 21:06:20.262499 django_easy_images-1.1/tests/easy_images_tests/models.py
+-rw-r--r--   0        0        0      410 2024-04-22 21:39:32.545263 django_easy_images-1.1/tests/settings.py
+-rw-r--r--   0        0        0     4470 2024-04-23 21:45:45.988357 django_easy_images-1.1/tests/test_command.py
+-rw-r--r--   0        0        0     1424 2024-04-17 23:33:25.980333 django_easy_images-1.1/tests/test_core.py
+-rw-r--r--   0        0        0     1850 2024-04-17 23:33:25.980333 django_easy_images-1.1/tests/test_engine.py
+-rw-r--r--   0        0        0     1036 2024-04-23 02:47:06.431022 django_easy_images-1.1/tests/test_models.py
+-rw-r--r--   0        0        0     1257 2024-04-17 23:33:25.980333 django_easy_images-1.1/tests/test_options.py
+-rw-r--r--   0        0        0     1333 2024-04-22 21:49:56.047786 django_easy_images-1.1/tests/test_signals.py
+-rw-r--r--   0        0        0    10612 1970-01-01 00:00:00.000000 django_easy_images-1.1/PKG-INFO
```

### Comparing `django_easy_images-1.0.1/README.md` & `django_easy_images-1.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Easy images
+# Django easy images
 
 Easily build responsive HTML `<img>` tags by thumbnailing Django images using the VIPS fast image processing library.
 
 When an `<img>` is generated, any thumbnails that don't already exist are queued for building (if aren't already queued) and left out of the HTML.
 For example, an image built from `Img(width="md")` will generate:
 
 ```html
@@ -20,18 +20,18 @@
   "
   alt="Profile photo for John Doe"
 >
 ```
 
 ## Installation & Configuration
 
-To install easy-images, simply run the following command:
+To install django-easy-images, simply run the following command:
 
 ```bash
-pip install easy-images
+pip install django-easy-images
 ```
 
 Once installed, add the `easy_images` app in your Django settings file:
 
 ```python
 INSTALLED_APPS = [
     "easy_images",
```

### Comparing `django_easy_images-1.0.1/easy_images/apps.py` & `django_easy_images-1.1/easy_images/apps.py`

 * *Files identical despite different names*

### Comparing `django_easy_images-1.0.1/easy_images/core.py` & `django_easy_images-1.1/easy_images/core.py`

 * *Files identical despite different names*

### Comparing `django_easy_images-1.0.1/easy_images/engine.py` & `django_easy_images-1.1/easy_images/engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,24 @@
+from __future__ import annotations
+
 import io
 import math
 import os
 from mimetypes import guess_type
 from pathlib import Path
+from typing import TYPE_CHECKING
 
 from django.core.files import File
 from django.core.files.uploadedfile import InMemoryUploadedFile, TemporaryUploadedFile
 from django.db.models.fields.files import FieldFile
 
 from easy_images.core import ParsedOptions
-from pyvips import Image
+
+if TYPE_CHECKING:
+    from pyvips import Image
 
 
 def scale_image(
     img,
     target: tuple[int, int],
     /,
     crop: tuple[float, float] | bool | None = None,
@@ -114,14 +119,16 @@
     if min_scale < 2:
         return img
     shrink = min(2 ** (math.floor(math.log(min_scale, 2))), 8)
     return _new_image(file, shrink=shrink, access=access)
 
 
 def _new_image(file: str | Path | File, access, **kwargs):
+    from pyvips import Image
+
     path = None
     if isinstance(file, File):
         if isinstance(file, FieldFile):
             try:
                 path = file.path
             except Exception:
                 pass
```

### Comparing `django_easy_images-1.0.1/easy_images/migrations/0001_initial.py` & `django_easy_images-1.1/easy_images/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_easy_images-1.0.1/easy_images/models.py` & `django_easy_images-1.1/easy_images/models.py`

 * *Files identical despite different names*

### Comparing `django_easy_images-1.0.1/easy_images/options.py` & `django_easy_images-1.1/easy_images/options.py`

 * *Files identical despite different names*

### Comparing `django_easy_images-1.0.1/easy_images/signals.py` & `django_easy_images-1.1/easy_images/signals.py`

 * *Files identical despite different names*

### Comparing `django_easy_images-1.0.1/easy_images/templatetags/easy_images.py` & `django_easy_images-1.1/easy_images/templatetags/easy_images.py`

 * *Files identical despite different names*

### Comparing `django_easy_images-1.0.1/easy_images/types.py` & `django_easy_images-1.1/easy_images/types.py`

 * *Files identical despite different names*

### Comparing `django_easy_images-1.0.1/pyproject.toml` & `django_easy_images-1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "django-easy-images"
-version = "1.0.1"
+version = "1.1"
 description = "Easily build responsive HTML `<img>` tags from Django images"
 authors = [
     { name = "Chris Beaven", email = "smileychris@gmail.com" },
 ]
 dependencies = [
     "django>=4.2",
     "typing-extensions>=4.11.0",
```

### Comparing `django_easy_images-1.0.1/tests/test_command.py` & `django_easy_images-1.1/tests/test_command.py`

 * *Files 14% similar despite different names*

```diff
@@ -49,14 +49,46 @@
 Skipping 1 with build errors...
 Successfully built 2 <img> thumbnails
 """
     )
 
 
 @pytest.mark.django_db
+def test_retry():
+    EasyImage.objects.create(args={}, name="1")
+    EasyImage.objects.create(status=ImageStatus.BUILDING, args={}, name="2")
+    EasyImage.objects.create(
+        status=ImageStatus.BUILD_ERROR, args={}, name="3", error_count=1
+    )
+    EasyImage.objects.create(
+        status=ImageStatus.SOURCE_ERROR, args={}, name="4", error_count=2
+    )
+    for name in "567":
+        EasyImage.objects.create(
+            image="test",
+            status=ImageStatus.BUILT,
+            width=800,
+            height=600,
+            args={},
+            name=name,
+        )
+    test_output = StringIO()
+    with mock.patch("easy_images.models.EasyImage.build", return_value=True):
+        call_command("build_img_queue", stdout=test_output, retry=1)
+    assert test_output.getvalue() == (
+        """Building queued <img> thumbnails...
+Skipping 1 marked as already building...
+Retrying 0 with source errors (1 with more than 1 retries skipped)...
+Retrying 1 with build errors...
+Successfully built 2 <img> thumbnails
+"""
+    )
+
+
+@pytest.mark.django_db
 def test_force():
     EasyImage.objects.create(args={}, name="1")
     EasyImage.objects.create(status=ImageStatus.BUILDING, args={}, name="2")
     EasyImage.objects.create(status=ImageStatus.BUILD_ERROR, args={}, name="3")
     EasyImage.objects.create(status=ImageStatus.SOURCE_ERROR, args={}, name="4")
     for name in "567":
         EasyImage.objects.create(
```

### Comparing `django_easy_images-1.0.1/tests/test_core.py` & `django_easy_images-1.1/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `django_easy_images-1.0.1/tests/test_engine.py` & `django_easy_images-1.1/tests/test_engine.py`

 * *Files identical despite different names*

### Comparing `django_easy_images-1.0.1/tests/test_models.py` & `django_easy_images-1.1/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `django_easy_images-1.0.1/tests/test_options.py` & `django_easy_images-1.1/tests/test_options.py`

 * *Files identical despite different names*

### Comparing `django_easy_images-1.0.1/tests/test_signals.py` & `django_easy_images-1.1/tests/test_signals.py`

 * *Files identical despite different names*

### Comparing `django_easy_images-1.0.1/PKG-INFO` & `django_easy_images-1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-easy-images
-Version: 1.0.1
+Version: 1.1
 Summary: Easily build responsive HTML `<img>` tags from Django images
 Author-Email: Chris Beaven <smileychris@gmail.com>
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -25,15 +25,15 @@
 Requires-Dist: tqdm>=4.66.2
 Requires-Dist: pillow
 Requires-Dist: pytest; extra == "tests"
 Requires-Dist: pytest-django>=4.8.0; extra == "tests"
 Provides-Extra: tests
 Description-Content-Type: text/markdown
 
-# Easy images
+# Django easy images
 
 Easily build responsive HTML `<img>` tags by thumbnailing Django images using the VIPS fast image processing library.
 
 When an `<img>` is generated, any thumbnails that don't already exist are queued for building (if aren't already queued) and left out of the HTML.
 For example, an image built from `Img(width="md")` will generate:
 
 ```html
@@ -51,18 +51,18 @@
   "
   alt="Profile photo for John Doe"
 >
 ```
 
 ## Installation & Configuration
 
-To install easy-images, simply run the following command:
+To install django-easy-images, simply run the following command:
 
 ```bash
-pip install easy-images
+pip install django-easy-images
 ```
 
 Once installed, add the `easy_images` app in your Django settings file:
 
 ```python
 INSTALLED_APPS = [
     "easy_images",
```

