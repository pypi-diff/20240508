# Comparing `tmp/labnas-0.2.2.tar.gz` & `tmp/labnas-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "labnas-0.2.2.tar", max compression
+gzip compressed data, was "labnas-0.2.3.tar", max compression
```

## Comparing `labnas-0.2.2.tar` & `labnas-0.2.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0       22 2023-02-23 15:12:09.060507 labnas-0.2.2/labnas/__init__.py
--rw-r--r--   0        0        0        0 2023-10-12 08:55:37.808632 labnas-0.2.2/labnas/local/__init__.py
--rw-r--r--   0        0        0     4072 2024-03-01 13:10:56.124191 labnas-0.2.2/labnas/local/base.py
--rw-r--r--   0        0        0      503 2024-01-17 09:18:38.927107 labnas-0.2.2/labnas/local/files.py
--rw-r--r--   0        0        0     1140 2023-10-13 08:39:29.563850 labnas-0.2.2/labnas/local/storage.py
--rw-r--r--   0        0        0        0 2023-10-12 09:33:22.730159 labnas-0.2.2/labnas/remote/__init__.py
--rw-r--r--   0        0        0    11471 2024-05-08 08:18:18.103471 labnas-0.2.2/labnas/remote/base.py
--rw-r--r--   0        0        0    13803 2024-03-01 15:29:21.989436 labnas-0.2.2/labnas/remote/imaging.py
--rw-r--r--   0        0        0      396 2024-05-08 08:18:57.223203 labnas-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      499 1970-01-01 00:00:00.000000 labnas-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0       22 2023-02-23 15:12:09.060507 labnas-0.2.3/labnas/__init__.py
+-rw-r--r--   0        0        0        0 2023-10-12 08:55:37.808632 labnas-0.2.3/labnas/local/__init__.py
+-rw-r--r--   0        0        0     4072 2024-03-01 13:10:56.124191 labnas-0.2.3/labnas/local/base.py
+-rw-r--r--   0        0        0      503 2024-01-17 09:18:38.927107 labnas-0.2.3/labnas/local/files.py
+-rw-r--r--   0        0        0     1164 2024-05-08 08:44:19.047249 labnas-0.2.3/labnas/local/storage.py
+-rw-r--r--   0        0        0        0 2023-10-12 09:33:22.730159 labnas-0.2.3/labnas/remote/__init__.py
+-rw-r--r--   0        0        0    11889 2024-05-08 08:42:46.812007 labnas-0.2.3/labnas/remote/base.py
+-rw-r--r--   0        0        0    13803 2024-03-01 15:29:21.989436 labnas-0.2.3/labnas/remote/imaging.py
+-rw-r--r--   0        0        0      396 2024-05-08 08:43:12.739794 labnas-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0      499 1970-01-01 00:00:00.000000 labnas-0.2.3/PKG-INFO
```

### Comparing `labnas-0.2.2/labnas/local/base.py` & `labnas-0.2.3/labnas/local/base.py`

 * *Files identical despite different names*

### Comparing `labnas-0.2.2/labnas/local/storage.py` & `labnas-0.2.3/labnas/local/storage.py`

 * *Files 27% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import zarr
 from tqdm import tqdm
 
 from labnas.local.base import list_tif_files, sort_tif_files
 
 
 def convert_to_tif(source_folder: Path, target_file: Path) -> None:
-    """Convert a folder with multiple tifs into a single tif file."""
+    """Convert a folder with multiple single-page tifs into a single multi-page tif file."""
     if not source_folder.is_dir():
         raise FileNotFoundError(f"{source_folder} is not a directory.")
     if target_file.is_dir():
         raise FileExistsError(f"{target_file} already exists.")
     tif_files = list_tif_files(source_folder)
     tif_files = sort_tif_files(tif_files)
     n_files = tif_files.size
@@ -26,8 +26,8 @@
                 shape=shape,
                 dtype=np.uint8,
             )
             store = tifffile.imread(target_file, mode="r+", aszarr=True)
             z = zarr.open(store, mode="r+")
             print(f"Empty tif created: {shape}")
         z[i_file, :, :] = image
-    store.close()
+    store.close()
```

### Comparing `labnas-0.2.2/labnas/remote/base.py` & `labnas-0.2.3/labnas/remote/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,27 +19,41 @@
             host_name: str,
             user_name: str,
             pwd: str,
             log_file: Path | None = None,
             logger: logging.Logger | None = None
     ) -> None:
         """Create pysftp.Connection to server."""
+        # params
         self._host_name = host_name
         self._user_name = user_name
         self._pwd = pwd
         self.logger = logger
         self.log_file = log_file
+
+        # state
+        self.is_open: bool = False
+        self.connection: pysftp.Connection | None = None
+
+        # go
         if self.logger is None:
             self.logger = self.create_logger()
+        self._establish_connection()
+
+    def _establish_connection(self) -> None:
+        """Establish an SFTP connection."""
+        if self.is_open:
+            raise ValueError(f"SFTP connection is already open!")
         self.connection: pysftp.Connection = pysftp.Connection(
-            host=host_name,
-            username=user_name,
-            password=pwd,
+            host=self._host_name,
+            username=self._user_name,
+            password=self._pwd,
         )
-        self.logger.info(f"Connection established: {host_name}@{user_name}")
+        self.logger.info(f"Connection established: {self._host_name}@{self._user_name}")
+        self.is_open = True
 
     def create_logger(self) -> logging.Logger:
         """Create a logger to print output to. Optionally save output to file."""
         logger = logging.Logger("nas")
         logger.setLevel(logging.DEBUG)
         stream_handler = logging.StreamHandler(stream=sys.stdout)
         formatter = logging.Formatter("%(asctime)s - %(message)s")
@@ -49,28 +63,26 @@
             file_handler = logging.FileHandler(self.log_file)
             formatter = logging.Formatter("%(asctime)s - %(message)s")
             file_handler.setFormatter(formatter)
             logger.addHandler(file_handler)
             logger.info(f"Logging into {self.log_file}")
         return logger
 
-    def close(self) -> None:
-        """Close connection."""
+    def close_connection(self) -> None:
+        """Close SFTP connection."""
         self.connection.close()
+        self.is_open = False
+        self.logger.info(f"Connection closed: {self._host_name}@{self._user_name}")
 
     def reconnect(self) -> None:
-        try:
-            self.connection.close()
-        except Exception as e:
-            self.logger.info(f"Could not close connection: {e}")
-        self.connection: pysftp.Connection = pysftp.Connection(
-            host=self._host_name,
-            username=self._user_name,
-            password=self._pwd,
-        )
+        """Attempt to re-establish pysftp.Connection."""
+        assert self.is_open
+        self.logger.info("Reconnecting.")
+        self.close_connection()
+        self._establish_connection()
 
     def list_contents(self, remote_folder: PathLike) -> list[PathLike]:
         """List contents of a nas folder"""
         remote_folder = self._convert_to_linux(remote_folder)
         if not self.is_dir(remote_folder):
             raise FileNotFoundError(f"{remote_folder} not found.")
         contents: list[str] = self.connection.listdir(str(remote_folder))
```

### Comparing `labnas-0.2.2/labnas/remote/imaging.py` & `labnas-0.2.3/labnas/remote/imaging.py`

 * *Files identical despite different names*

