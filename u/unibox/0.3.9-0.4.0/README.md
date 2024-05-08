# Comparing `tmp/unibox-0.3.9.tar.gz` & `tmp/unibox-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unibox-0.3.9.tar", max compression
+gzip compressed data, was "unibox-0.4.0.tar", max compression
```

## Comparing `unibox-0.3.9.tar` & `unibox-0.4.0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
--rw-r--r--   0        0        0     1061 2023-12-10 21:47:29.712946 unibox-0.3.9/LICENSE
--rw-r--r--   0        0        0     2140 2023-12-10 21:47:29.712946 unibox-0.3.9/README.md
--rw-r--r--   0        0        0      642 2023-12-10 21:47:29.712946 unibox-0.3.9/pyproject.toml
--rw-r--r--   0        0        0     3165 2023-12-10 21:47:29.712946 unibox-0.3.9/unibox/__init__.py
--rw-r--r--   0        0        0     5428 2023-12-10 21:47:29.712946 unibox-0.3.9/unibox/cli.py
--rw-r--r--   0        0        0        0 2023-12-10 21:47:29.712946 unibox-0.3.9/unibox/processing/__init__.py
--rw-r--r--   0        0        0     3051 2023-12-10 21:47:29.712946 unibox-0.3.9/unibox/processing/file_mover.py
--rw-r--r--   0        0        0     2149 2023-12-10 21:47:29.712946 unibox-0.3.9/unibox/processing/file_renamer.py
--rw-r--r--   0        0        0     7193 2023-12-10 21:47:29.712946 unibox-0.3.9/unibox/processing/image_resizer.py
--rw-r--r--   0        0        0        0 2023-12-10 21:47:29.712946 unibox-0.3.9/unibox/utils/__init__.py
--rw-r--r--   0        0        0      244 2023-12-10 21:47:29.712946 unibox-0.3.9/unibox/utils/constants.py
--rw-r--r--   0        0        0     4069 2023-12-10 21:47:29.712946 unibox-0.3.9/unibox/utils/s3_client.py
--rw-r--r--   0        0        0     5622 2023-12-10 21:47:29.712946 unibox-0.3.9/unibox/utils/uni_loader.py
--rw-r--r--   0        0        0     4279 2023-12-10 21:47:29.712946 unibox-0.3.9/unibox/utils/uni_logger.py
--rw-r--r--   0        0        0     3139 2023-12-10 21:47:29.712946 unibox-0.3.9/unibox/utils/uni_merger.py
--rw-r--r--   0        0        0     9799 2023-12-10 21:47:29.712946 unibox-0.3.9/unibox/utils/uni_resizer.py
--rw-r--r--   0        0        0     5387 2023-12-10 21:47:29.712946 unibox-0.3.9/unibox/utils/uni_saver.py
--rw-r--r--   0        0        0     5503 2023-12-10 21:47:29.712946 unibox-0.3.9/unibox/utils/uni_traverser.py
--rw-r--r--   0        0        0      580 2023-12-10 21:47:29.712946 unibox-0.3.9/unibox/utils/utils.py
--rw-r--r--   0        0        0     3245 1970-01-01 00:00:00.000000 unibox-0.3.9/PKG-INFO
+-rw-r--r--   0        0        0     1061 2024-05-08 17:50:46.629745 unibox-0.4.0/LICENSE
+-rw-r--r--   0        0        0     4088 2024-05-08 17:50:46.629745 unibox-0.4.0/README.md
+-rw-r--r--   0        0        0      629 2024-05-08 17:50:46.629745 unibox-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     4353 2024-05-08 17:50:46.629745 unibox-0.4.0/unibox/__init__.py
+-rw-r--r--   0        0        0     5428 2024-05-08 17:50:46.629745 unibox-0.4.0/unibox/cli.py
+-rw-r--r--   0        0        0        0 2024-05-08 17:50:46.629745 unibox-0.4.0/unibox/processing/__init__.py
+-rw-r--r--   0        0        0     3051 2024-05-08 17:50:46.629745 unibox-0.4.0/unibox/processing/file_mover.py
+-rw-r--r--   0        0        0     2149 2024-05-08 17:50:46.629745 unibox-0.4.0/unibox/processing/file_renamer.py
+-rw-r--r--   0        0        0     7196 2024-05-08 17:50:46.629745 unibox-0.4.0/unibox/processing/image_resizer.py
+-rw-r--r--   0        0        0        0 2024-05-08 17:50:46.629745 unibox-0.4.0/unibox/utils/__init__.py
+-rw-r--r--   0        0        0      244 2024-05-08 17:50:46.629745 unibox-0.4.0/unibox/utils/constants.py
+-rw-r--r--   0        0        0     6249 2024-05-08 17:50:46.629745 unibox-0.4.0/unibox/utils/s3_client.py
+-rw-r--r--   0        0        0     6751 2024-05-08 17:50:46.629745 unibox-0.4.0/unibox/utils/uni_loader.py
+-rw-r--r--   0        0        0     4279 2024-05-08 17:50:46.629745 unibox-0.4.0/unibox/utils/uni_logger.py
+-rw-r--r--   0        0        0     3139 2024-05-08 17:50:46.629745 unibox-0.4.0/unibox/utils/uni_merger.py
+-rw-r--r--   0        0        0     4377 2024-05-08 17:50:46.629745 unibox-0.4.0/unibox/utils/uni_peeker.py
+-rw-r--r--   0        0        0     8327 2024-05-08 17:50:46.629745 unibox-0.4.0/unibox/utils/uni_resizer.py
+-rw-r--r--   0        0        0     5387 2024-05-08 17:50:46.629745 unibox-0.4.0/unibox/utils/uni_saver.py
+-rw-r--r--   0        0        0     5885 2024-05-08 17:50:46.629745 unibox-0.4.0/unibox/utils/uni_traverser.py
+-rw-r--r--   0        0        0      580 2024-05-08 17:50:46.629745 unibox-0.4.0/unibox/utils/utils.py
+-rw-r--r--   0        0        0     5201 1970-01-01 00:00:00.000000 unibox-0.4.0/PKG-INFO
```

### Comparing `unibox-0.3.9/LICENSE` & `unibox-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `unibox-0.3.9/pyproject.toml` & `unibox-0.4.0/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "unibox"
-version = "0.3.9"
-description = "Unibox is a tool that aims to provide a unified interface for various common daily operations"
+version = "0.4.0"
+description = "Unibox provides unified interface for common file operations."
 authors = ["yada <trojblue@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/trojblue/unibox"
 
 [tool.poetry.dependencies]
 python = "^3.8"
@@ -15,14 +15,15 @@
 pillow = "^10.0.0"
 tqdm = "^4.65.0"
 colorlog = "^6.7.0"
 pandas = "*"
 pyarrow = "*"
 boto3 = "^1.28.76"
 requests = "^2.31.0"
+orjson = "^3.9.10"
 
 
 [tool.poetry.scripts]
 unibox = 'unibox.cli:cli'
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `unibox-0.3.9/unibox/cli.py` & `unibox-0.4.0/unibox/cli.py`

 * *Files identical despite different names*

### Comparing `unibox-0.3.9/unibox/processing/file_mover.py` & `unibox-0.4.0/unibox/processing/file_mover.py`

 * *Files identical despite different names*

### Comparing `unibox-0.3.9/unibox/processing/file_renamer.py` & `unibox-0.4.0/unibox/processing/file_renamer.py`

 * *Files identical despite different names*

### Comparing `unibox-0.3.9/unibox/processing/image_resizer.py` & `unibox-0.4.0/unibox/processing/image_resizer.py`

 * *Files 0% similar despite different names*

```diff
@@ -199,15 +199,15 @@
                         f"min_side={self.min_side}, format={self.format}, quality={self.quality}," \
                         f"exist_ok={self.exist_ok}"
         print(debug_string)
 
 
 if __name__ == "__main__":
     # Define the source and destination directories and the minimum side length for resizing
-    src_dir = input("dir path:")
+    src_dir = input("s3_uri path:")
 
     dst_dir = f"{src_dir}_768webp"
     min_side = 1024
 
     # Create an instance of the UniResizer class
     resizer = ImageResizer(src_dir, dst_dir, min_side)
```

### Comparing `unibox-0.3.9/unibox/utils/uni_loader.py` & `unibox-0.4.0/unibox/utils/uni_loader.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import json
 import timeit
 
 import os
 import mimetypes
 import tempfile
 import requests
+import orjson
 
 import tomli
 import pandas as pd
 
 from PIL import Image
 from pathlib import Path
 from omegaconf import OmegaConf
@@ -45,57 +46,67 @@
             '.png': self._load_image,
             '.jpg': self._load_image,
             '.webp': self._load_image,
             '.jpeg': self._load_image,
             '.toml': self._load_toml,
             '.yaml': self._load_yaml,
             '.parquet': self._load_parquet,
+            '.feather': self._load_feather,
         }
 
     def _load_from_s3(self, s3_uri: str):
         """Download a file from an S3 URI and load its content."""
         s3_client = S3Client()
-        with tempfile.TemporaryDirectory() as tmp_dir:
-            local_path = Path(s3_client.download(s3_uri, tmp_dir))
-            return self.loads(local_path)
+        try:
+            with tempfile.TemporaryDirectory() as tmp_dir:
+                local_path = Path(s3_client.download(s3_uri, tmp_dir))
+                return self.loads(local_path)
+        except Exception as e:
+            self.logger.error(f'Error loading from S3 at "{s3_uri}": {e}')
+            return None
 
     def _load_from_url(self, url: str):
         """Download a file from a URL and load its content."""
         response = requests.get(url)
         response.raise_for_status()  # Ensure the request was successful
 
         _, url_suffix = os.path.splitext(url)
         if url_suffix == '':
             content_type = response.headers.get('content-type')
             mime_suffix = mimetypes.guess_extension(content_type)
             suffix = mime_suffix if mime_suffix else ''
         else:
             suffix = url_suffix
 
-        with tempfile.NamedTemporaryFile(suffix=suffix, delete=False) as tmp_file:
-            tmp_file.write(response.content)
-            tmp_file.flush()
-            tmp_file_path = tmp_file.name
-            tmp_file.close()
-            return self.loads(tmp_file_path)
+        try:
+            with tempfile.NamedTemporaryFile(suffix=suffix, delete=True) as tmp_file:
+                tmp_file.write(response.content)
+                tmp_file.flush()
+                tmp_file_path = tmp_file.name
+                tmp_file.close()
+                return self.loads(tmp_file_path)
+        except Exception as e:
+            self.logger.error(f'Error loading from URL at "{url}": {e}')
+            return None
 
     def loads(self, file_path: Path | str, encoding="utf-8"):
         """Load data from the given file path.
 
         The type of data returned depends on the file extension.
         """
         start_time = timeit.default_timer()
 
         # check if is s3 uri or url (downloads the file)
         if isinstance(file_path, str):
-            if is_url(file_path):
-                return self._load_from_url(file_path)
-            elif is_s3_uri(file_path):
+            if is_s3_uri(file_path):
                 return self._load_from_s3(file_path)
 
+            elif is_url(file_path):
+                return self._load_from_url(file_path)
+
         # is a local file
         if isinstance(file_path, str):
             file_path = Path(file_path)
 
         file_type = file_path.suffix.lower()
 
         if not file_path.exists():
@@ -112,22 +123,36 @@
             if self.debug_print:
                 self.logger.info(f'{file_type} LOADED from "{file_path}" in {timeit.default_timer() - start_time:.2f}s')
             return result
         except Exception as e:
             self.logger.error(f'{file_type} LOAD ERROR at "{file_path}": {e}')
             return None
 
-    def _load_json(self, file_path: Path, encoding):
-        with open(file_path, "r", encoding=encoding) as f:
-            return json.load(f)
+    def _load_json(self, file_path: Path, encoding='utf-8'):
+        try:
+            with open(file_path, "rb") as f:
+                file_content = f.read()
+                # Check if the file content is empty
+                if not file_content:
+                    self.logger.error(f'{file_path} is empty or zero-length.')
+                    return None  # or {} depending on how you want to handle this case
+                return orjson.loads(file_content)
+        except orjson.JSONDecodeError as e:
+            self.logger.error(f'JSON LOAD ERROR at "{file_path}": {e}')
+            return None
+        except Exception as e:
+            self.logger.error(f'Unexpected error loading JSON at "{file_path}": {e}')
+            return None
 
-    def _load_jsonl(self, file_path: Path, encoding):
+
+    def _load_jsonl(self, file_path: Path, encoding='utf-8'):
         """Load data from a .jsonl file and return it as a list of dictionaries."""
-        with open(file_path, "r", encoding=encoding) as f:
-            return [json.loads(line) for line in f]
+        with open(file_path, "rb") as f:
+            # Decode each line if necessary after parsing
+            return [orjson.loads(line) for line in f]
 
     def _load_txt(self, file_path: Path, encoding):
         with open(file_path, "r", encoding=encoding) as f:
             raw_lines = f.readlines()
             return [line.strip() for line in raw_lines]
 
     def _load_csv(self, file_path: Path, encoding):
@@ -143,14 +168,16 @@
     def _load_yaml(self, file_path: Path, encoding):
         with open(file_path, "r", encoding=encoding) as f:
             return OmegaConf.load(f)
 
     def _load_parquet(self, file_path: Path, encoding):
         return pd.read_parquet(file_path)
 
+    def _load_feather(self, file_path: Path, encoding):
+        return pd.read_feather(file_path)
 
 if __name__ == "__main__":
     # Usage example
     logger = UniLogger("logs", file_suffix="data_loader")
     data_loader = UniLoader(logger)
     json_data = data_loader.loads("example.json")  # string
     txt_data = data_loader.loads(Path("example.txt"))  # path
```

### Comparing `unibox-0.3.9/unibox/utils/uni_logger.py` & `unibox-0.4.0/unibox/utils/uni_logger.py`

 * *Files identical despite different names*

### Comparing `unibox-0.3.9/unibox/utils/uni_merger.py` & `unibox-0.4.0/unibox/utils/uni_merger.py`

 * *Files identical despite different names*

### Comparing `unibox-0.3.9/unibox/utils/uni_resizer.py` & `unibox-0.4.0/unibox/utils/uni_resizer.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,236 +1,172 @@
 import os
 import math
-import shutil
 from PIL import Image
 from pathlib import Path
 from tqdm.auto import tqdm
-
-import unibox
-from unibox import UniLoader, UniLogger
-
 from concurrent.futures import ProcessPoolExecutor, as_completed
 from typing import List, Tuple
+import unibox
+from unibox import UniLogger
 
 
-class UniResizer:
-    """
-    Resizes images in a directory to a specified size.
+def chunk_list(lst, chunk_size):
+    """Yield successive chunks of size `chunk_size` from list `lst`."""
+    for i in range(0, len(lst), chunk_size):
+        yield lst[i:i + chunk_size]
 
-    Resolution:
-        - by min_dim: resize the shorter side to a specified size
-        - by max_dim: resize the longer side to a specified size
-        - by target_pixels: resize the shorter side to a specified number of pixels
-
-    Methods:
-        - by directory: resize all images in a directory
-        - by list: resize a list of images given
-
-    Usage:
-    >>> resizer = UniResizer(root_dir, dst_dir, min_dim=min_dim, max_dim=max_dim, target_pixels=target_pixels,
-    >>>                   keep_hierarchy=False, exist_ok=True)
-    >>> resizer.execute_resize_jobs(resizer.get_resize_jobs())
-    """
 
+class UniResizer:
     TRUNCATE_MULTIPLIER = 32  # the shorter side will be a multiple of 32 after scaling
     WEBP_QUALITY = 98  # quality of the output image (max:100)
     EXTENSION = ".webp"  # file extension (.webp)
 
-    def __init__(self, root_dir: str, dst_dir: str,
-                 min_dim: int = None, max_dim: int = None, target_pixels: int = None,
-                 keep_hierarchy: bool = True, exist_ok: bool = True, logger: UniLogger = None):
-        """
-        Initialize an instance of UniResizer.
-
-        :param root_dir: root directory containing the images to be resized
-        :param dst_dir: destination directory to saves the resized images
-        :param min_dim: minimum dimension of the shorter side
-        :param max_dim: maximum dimension of the longer side (higher priority than min_dim)
-        :param target_pixels: target number of pixels (higher priority than max_dim), will be truncated
-        :param keep_hierarchy: if True, keep the original directory hierarchy; otherwise, flatten the directory
-        """
+    def __init__(self, root_dir: str, dst_dir: str, min_dim: int = None, max_dim: int = None, target_pixels: int = None,
+                 keep_hierarchy: bool = True, exist_ok: bool = True, logger: UniLogger = None, max_workers: int = None,
+                 chunk_size: int = 10_000, ):
+        """
+        Resizes images in a directory to a specified size.
+
+        Resolution:
+            - by min_dim: resize the shorter side to a specified size
+            - by max_dim: resize the longer side to a specified size
+            - by target_pixels: resize the shorter side to a specified number of pixels
+
+        Methods:
+            - by directory: resize all images in a directory
+            - by list: resize a list of images given
+
+        Configs:
+            - keep_hierarchy: keep the same directory structure as the source directory
+            - exist_ok: skip resizing if the destination file already exists
+            - max_workers: number of workers for parallel processing
+            - chunk_size: number of images to process in each chunk (to be dispatched to ProcessPoolExecutor each time)
+        
+        Usage:
+        >>> resizer = UniResizer(root_dir, dst_dir, min_dim=min_dim, max_dim=max_dim, target_pixels=target_pixels,
+        >>>                   keep_hierarchy=False, exist_ok=True)
+        >>> resizer.execute_resize_jobs(resizer.get_resize_jobs())
+        """ 
+        
         self.root_dir = root_dir
         self.dst_dir = dst_dir
-
         self.min_dim = min_dim
         self.max_dim = max_dim
         self.target_pixels = target_pixels
-
         self.keep_hierarchy = keep_hierarchy
         self.exist_ok = exist_ok
-
         self.logger = logger if logger is not None else UniLogger()
-
-    @staticmethod
-    def _get_new_dimensions(width: int, height: int, target_side: int, resize_by_longer_side: bool = False) -> tuple:
-        """
-        Calculates new dimensions based on the target,
-        for either the shorter or longer side while maintaining aspect ratio.
-
-        :param width: original width of the image
-        :param height: original height of the image
-        :param target_side: target dimension for the side specified
-        :param resize_by_longer_side: if True, resize by longer side; otherwise, by shorter side
-        :return: tuple containing new dimensions (new_width, new_height)
-        """
-        if target_side == -1:
-            return int(width), int(height)
-
-        if any(x <= 0 or type(x) != int for x in [width, height, target_side]):
-            raise ValueError("width, height and target_side must be positive integers")
-
-        # Determine shorter and longer side
-        shorter_side, longer_side = min(width, height), max(width, height)
-
-        if resize_by_longer_side:
-            target_longer_side = target_side
-            new_longer_side = target_longer_side
-            new_shorter_side = round(new_longer_side * (shorter_side / longer_side))
-        else:
-            target_shorter_side = target_side
-            new_shorter_side = target_shorter_side
-            new_longer_side = round(new_shorter_side * (longer_side / shorter_side))
-
-        # Assign new dimensions based on original orientation (portrait or landscape)
-        if width > height:
-            return new_longer_side, new_shorter_side
-        else:
-            return new_shorter_side, new_longer_side
+        self.max_workers = int(os.cpu_count() - 1) if max_workers is None else max_workers
+        self.chunk_size = chunk_size
 
     def _get_dst_path(self, og_rel_image_path: str) -> str:
-        """
-        :param og_rel_image_path: original relative image path
-        """
-        assert self.EXTENSION.startswith(".") and self.EXTENSION != ".", "extension must start with a dot"
-
         og_rel_path = Path(og_rel_image_path)
         rel_resized_path = og_rel_path.with_name(f"{og_rel_path.stem}_resized{self.EXTENSION}")
-
         if self.keep_hierarchy:
             dst_file_path = Path(self.dst_dir) / rel_resized_path
-
         else:
             dst_file_path = Path(self.dst_dir) / rel_resized_path.name
-
         return str(dst_file_path)
 
     def _create_dst_dir(self, dst_file_path: str) -> None:
         Path(dst_file_path).parent.mkdir(parents=True, exist_ok=True)
 
     def resize_single_image(self, image: Image.Image) -> Image.Image:
         width, height = image.size
         new_width, new_height = width, height
 
-        # Define the need_resize variable
         need_resize = (self.min_dim is not None and min(width, height) < self.min_dim) or \
                       (self.max_dim is not None and max(width, height) > self.max_dim)
 
-        # Priority 1: Resize based on target_pixels
         if self.target_pixels is not None:
-            if width * height > self.target_pixels:  # Add this check
+            if width * height > self.target_pixels:
                 scale_factor = math.sqrt(self.target_pixels / (width * height))
-                target_shorter_side = round(
-                    (min(width, height) * scale_factor) // self.TRUNCATE_MULTIPLIER) * self.TRUNCATE_MULTIPLIER
+                target_shorter_side = round((min(width, height) * scale_factor) // self.TRUNCATE_MULTIPLIER) * self.TRUNCATE_MULTIPLIER
                 new_width, new_height = self._get_new_dimensions(width, height, target_shorter_side)
 
-        # Priority 2: Resize based on max_dim
         elif self.max_dim is not None and need_resize:
             new_width, new_height = self._get_new_dimensions(width, height, self.max_dim, resize_by_longer_side=True)
 
-        # Priority 3: Resize based on min_dim
         elif self.min_dim is not None and need_resize:
-            if min(width, height) > self.min_dim:  # Add this check
-                new_width, new_height = self._get_new_dimensions(width, height, self.min_dim)
+            new_width, new_height = self._get_new_dimensions(width, height, self.min_dim)
 
-        # If resizing is not needed, return the original image
         elif not need_resize:
             return image
 
-        # Perform the resize operation
         return image.resize((new_width, new_height), Image.LANCZOS)
 
-    def _resize_single_image_task(self, og_rel_image_path: str) -> None:
-        """
-        Resize a single image and saves the result.
-
-        :param og_rel_image_path: original image path relative to self.root_dir
-        """
-        loader = UniLoader(debug_print=False)
-        image = loader.loads(os.path.join(self.root_dir, og_rel_image_path))
-        image = self.resize_single_image(image)
+    @staticmethod
+    def _get_new_dimensions(width: int, height: int, target_side: int, resize_by_longer_side: bool = False) -> tuple:
+        if target_side == -1:
+            return int(width), int(height)
+        if any(x <= 0 or type(x) != int for x in [width, height, target_side]):
+            raise ValueError("width, height and target_side must be positive integers")
+        shorter_side, longer_side = min(width, height), max(width, height)
+        if resize_by_longer_side:
+            new_longer_side = target_side
+            new_shorter_side = round(new_longer_side * (shorter_side / longer_side))
+        else:
+            new_shorter_side = target_side
+            new_longer_side = round(new_shorter_side * (longer_side / shorter_side))
+        if width > height:
+            return new_longer_side, new_shorter_side
+        else:
+            return new_shorter_side, new_longer_side
 
-        # Handle saves path
+    def _resize_single_image_task(self, og_rel_image_path: str) -> None:
+        src_file_path = os.path.join(self.root_dir, og_rel_image_path)
         dst_file_path = self._get_dst_path(og_rel_image_path)
-
-        # Create destination directory
         if self.keep_hierarchy:
             self._create_dst_dir(dst_file_path)
-
-        # Save
         try:
-            with open(dst_file_path, "wb") as f:
-                image.save(f, "webp", quality=self.WEBP_QUALITY)
-        except OSError:
-            self.logger.error(f"Error saving image {dst_file_path}. Skipping...")
+            with Image.open(src_file_path) as image:
+                resized_image = self.resize_single_image(image)
+                with open(dst_file_path, "wb") as f:
+                    resized_image.save(f, "webp", quality=self.WEBP_QUALITY)
+        except OSError as e:
+            self.logger.error(f"Error processing image {og_rel_image_path}: {e}. Skipping...")
 
     @staticmethod
-    def _execute_resize_tasks(tasks: List[Tuple]):
-        """
-        Execute tasks using ProcessPoolExecutor
-        """
-        with ProcessPoolExecutor() as executor:
-            futures = [executor.submit(task, *args) for task, *args in tasks]
-            list(tqdm(as_completed(futures), total=len(tasks), desc="Resizing images"))
+    def _execute_resize_tasks(tasks: List[Tuple], max_workers: int, total_progress: tqdm) -> None:
+        with ProcessPoolExecutor(max_workers=max_workers) as executor:
+            future_to_task = {executor.submit(task, *args): i for i, (task, *args) in enumerate(tasks)}
+            for future in as_completed(future_to_task):
+                total_progress.update(1)
 
     def get_resize_jobs(self) -> List[str]:
-        """
-        Get the list of image files that need to be resized.
-
-        :return: List of image paths relative to self.root_dir to be resized
-        """
         self.logger.info("Getting image paths...")
-        todo_image_files = unibox.traverses(self.root_dir, include_extensions=unibox.constants.IMG_FILES,
-                                            relative_unix=True)
-
+        todo_image_files = unibox.traverses(self.root_dir, include_extensions=unibox.constants.IMG_FILES, relative_unix=True)
         if self.exist_ok:
             self.logger.info("Checking existing files...")
-            existing_files = unibox.traverses(self.dst_dir, include_extensions=unibox.constants.IMG_FILES,
-                                              relative_unix=False)
-
+            existing_files = unibox.traverses(self.dst_dir, include_extensions=unibox.constants.IMG_FILES, relative_unix=False)
             expected_file_set = {self._get_dst_path(rel_path) for rel_path in todo_image_files}
             existing_file_set = set(existing_files)
-
-            # Find the difference between the two sets
             needed_files_set = expected_file_set - existing_file_set
-
-            # Map back to original relative paths
             reverse_mapping = {self._get_dst_path(rel_path): rel_path for rel_path in todo_image_files}
             todo_image_files = [reverse_mapping[dst_path] for dst_path in needed_files_set]
-
         return todo_image_files
 
-    def execute_resize_jobs(self, image_files: List[str]) -> None:
-        """
-        Execute resizing tasks for the given list of image files.
-
-        :param image_files: List of relative image paths to be resized
-            e.g. "root_dir/some_dir/image.jpg" -> entry should be "some_dir/image_resized.jpg"
-        """
+    def execute_resize_jobs(self, image_files: List[str], report_interval:float=5) -> None:
         tasks = [(self._resize_single_image_task, og_rel_image_path) for og_rel_image_path in image_files]
+        self.logger.info(f"Resizing {len(tasks)} images from {self.root_dir} to {self.dst_dir} | chunk size: {self.chunk_size} | report interval: {report_interval}s")
+        
+        # creating shared progress bar
+        pbar = tqdm(total=len(tasks), 
+                    desc=f"[interval={report_interval}] resizing [{self.root_dir}]", 
+                    mininterval=report_interval
+                    )
+        # Process each chunk
+        for chunk in chunk_list(tasks, self.chunk_size):
+            self._execute_resize_tasks(chunk, self.max_workers, pbar)
+        
+        pbar.close()
 
-        self.logger.info(f"Resizing {len(tasks)} images...")
-        self._execute_resize_tasks(tasks)
-
-
+# Example Usage
 if __name__ == '__main__':
     root_dir = r"E:\_benchmark\1k"
     dst_dir = r"E:\_benchmark\1k_resized"
-
-    min_dim = 512  # lower priority
-    max_dim = int(1024 * 3)  # higher priority
-    target_pixels = int(1024 * 1024 * 1.25)  # highest priority
-
-    resizer = UniResizer(root_dir, dst_dir, min_dim=min_dim, max_dim=max_dim, target_pixels=target_pixels,
-                         keep_hierarchy=False, exist_ok=True)
-
+    min_dim = 512
+    max_dim = int(1024 * 3)
+    target_pixels = int(1024 * 1024 * 1.25)
+    resizer = UniResizer(root_dir, dst_dir, min_dim=min_dim, max_dim=max_dim, target_pixels=target_pixels, keep_hierarchy=False, exist_ok=True)
     images_to_resize = resizer.get_resize_jobs()
     resizer.execute_resize_jobs(images_to_resize)
```

### Comparing `unibox-0.3.9/unibox/utils/uni_saver.py` & `unibox-0.4.0/unibox/utils/uni_saver.py`

 * *Files identical despite different names*

### Comparing `unibox-0.3.9/unibox/utils/uni_traverser.py` & `unibox-0.4.0/unibox/utils/uni_traverser.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,42 +37,50 @@
         for root, _, files in os.walk(self.root_dir):
             for file_name in files:
                 extension = os.path.splitext(file_name)[1].lower()
                 if (self.include_extensions is None or extension in self.include_extensions) and \
                         (self.exclude_extensions is None or extension not in self.exclude_extensions):
                     yield os.path.join(root, file_name)
 
-    def traverse(self, file_handler: Callable[[str], None] = None) -> None:
+    def traverse(self, file_handler: Callable[[str], None] = None, debug_print: bool = True) -> None:
         """
         Traverses the directory tree and applies the given file handler to each file.
 
         Args:
             file_handler: A function that takes a file path and performs the desired action.
+            debug_print: Whether to print debug messages such as tqdm. (turn off if traversing many files)
         """
         if not file_handler:
             file_handler = lambda x: x  # do nothing; only get the file paths
 
         if self.pre_process:
             self.pre_process()
 
-        with tqdm(desc="Traversing files", leave=False, unit="files", total=None) as pbar:
-            for file_path in self._files_to_traverse():
-                try:
-                    file_handler(file_path)
-                except Exception as e:
-                    if self.error_handler:
-                        self.error_handler(e)
-                    else:
-                        raise e
+        # Conditionally initialize tqdm based on debug_print
+        pbar = tqdm(desc="Traversing files", leave=False, unit="files", total=None, disable=not debug_print) if debug_print else None
+
+        for file_path in self._files_to_traverse():
+            try:
+                file_handler(file_path)
+            except Exception as e:
+                if self.error_handler:
+                    self.error_handler(e)
+                else:
+                    raise e
+            if debug_print:
                 pbar.update(1)
-                self.traversed_files.append(file_path)
+            self.traversed_files.append(file_path)
+
+        if pbar is not None:  # Ensure the progress bar is closed if it was used
+            pbar.close()
 
         if self.post_process:
             self.post_process()
 
+
     def to_relative_unix_path(self, absolute_path: str, convert_slash: bool = True) -> str:
         """
         Converts the absolute Windows path to a relative path with respect to the root directory.
         Optionally, converts the backslashes to forward slashes for cross-platform compatibility.
 
         Args:
             absolute_path: The absolute Windows path to convert.
@@ -93,28 +101,28 @@
         if relative_unix:
             return [self.to_relative_unix_path(file_path) for file_path in self.traversed_files]
         else:
             return self.traversed_files
 
 
 def traverses(root_dir: str, include_extensions: List[str] = None,
-              exclude_extensions: List[str] = None, relative_unix=False):
+              exclude_extensions: List[str] = None, relative_unix=False, debug_print=True):
     """
 
     Args:
-        root_dir: the root dir to traverse
+        root_dir: the root s3_uri to traverse
         include_extensions: list of extensions that will be included in the traversal (.txt .jpg .webp)
         exclude_extensions: list of extensions that will be excluded in the traversal (.txt .jpg .webp)
         relative_unix: whether to give a relative path or not (default False gives absolute path)
 
     Returns:
         list of files that were traversed
     """
     traverser = UniTraverser(root_dir, include_extensions, exclude_extensions)
-    traverser.traverse()
+    traverser.traverse(debug_print=debug_print)
     files = traverser.get_traversed_files(relative_unix=relative_unix)
     return files
 
 
 # example code
 def pre_process():
     print("Starting traversal...")
```

### Comparing `unibox-0.3.9/unibox/utils/utils.py` & `unibox-0.4.0/unibox/utils/utils.py`

 * *Files identical despite different names*

