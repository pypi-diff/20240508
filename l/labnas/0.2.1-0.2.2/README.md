# Comparing `tmp/labnas-0.2.1.tar.gz` & `tmp/labnas-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "labnas-0.2.1.tar", max compression
+gzip compressed data, was "labnas-0.2.2.tar", max compression
```

## Comparing `labnas-0.2.1.tar` & `labnas-0.2.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0       22 2023-02-23 15:12:09.060507 labnas-0.2.1/labnas/__init__.py
--rw-r--r--   0        0        0        0 2023-10-12 08:55:37.808632 labnas-0.2.1/labnas/local/__init__.py
--rw-r--r--   0        0        0     2987 2023-10-31 10:35:29.391802 labnas-0.2.1/labnas/local/base.py
--rw-r--r--   0        0        0      503 2024-01-17 09:18:38.927107 labnas-0.2.1/labnas/local/files.py
--rw-r--r--   0        0        0     1140 2023-10-13 08:39:29.563850 labnas-0.2.1/labnas/local/storage.py
--rw-r--r--   0        0        0        0 2023-10-12 09:33:22.730159 labnas-0.2.1/labnas/remote/__init__.py
--rw-r--r--   0        0        0    11163 2024-01-18 09:36:08.383500 labnas-0.2.1/labnas/remote/base.py
--rw-r--r--   0        0        0    12383 2024-01-17 09:18:38.927107 labnas-0.2.1/labnas/remote/imaging.py
--rw-r--r--   0        0        0      396 2024-01-18 09:36:08.395500 labnas-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      499 1970-01-01 00:00:00.000000 labnas-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0       22 2023-02-23 15:12:09.060507 labnas-0.2.2/labnas/__init__.py
+-rw-r--r--   0        0        0        0 2023-10-12 08:55:37.808632 labnas-0.2.2/labnas/local/__init__.py
+-rw-r--r--   0        0        0     4072 2024-03-01 13:10:56.124191 labnas-0.2.2/labnas/local/base.py
+-rw-r--r--   0        0        0      503 2024-01-17 09:18:38.927107 labnas-0.2.2/labnas/local/files.py
+-rw-r--r--   0        0        0     1140 2023-10-13 08:39:29.563850 labnas-0.2.2/labnas/local/storage.py
+-rw-r--r--   0        0        0        0 2023-10-12 09:33:22.730159 labnas-0.2.2/labnas/remote/__init__.py
+-rw-r--r--   0        0        0    11471 2024-05-08 08:18:18.103471 labnas-0.2.2/labnas/remote/base.py
+-rw-r--r--   0        0        0    13803 2024-03-01 15:29:21.989436 labnas-0.2.2/labnas/remote/imaging.py
+-rw-r--r--   0        0        0      396 2024-05-08 08:18:57.223203 labnas-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      499 1970-01-01 00:00:00.000000 labnas-0.2.2/PKG-INFO
```

### Comparing `labnas-0.2.1/labnas/local/base.py` & `labnas-0.2.2/labnas/local/base.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,79 +1,108 @@
+"""Basic local functions."""
+
 import re
 from pathlib import Path
 
 import numpy as np
 
 
 def assert_single_stack(tif_files: list[Path]) -> str:
+    """Check that there is only one stack in list of tifs"""
     tif_origin = identify_tif_origin(tif_files[0])
     if tif_origin == "leica":
         stack_names = get_leica_stack_names(tif_files)
+    elif tif_origin == "basler":
+        stack_names = get_basler_stack_names(tif_files)
     else:
         raise NotImplementedError(f"{tif_origin=} not implemented.")
     assert len(stack_names) == 1, f"More than 1 stack in {tif_files[0].parent}: {stack_names}"
     print(f"Only one stack: {stack_names[0]}")
     return stack_names[0]
 
 
 def identify_tif_origin(tif: Path) -> str:
+    """
+    Identify where tif comes from.
+    Relies on file name components added by recording software.
+    """
     if "ch00" in tif.name:
         origin = "leica"
     elif "LUT" in tif.name:
         origin = "leica_metadata"
-    else:
+    elif "Basler" in tif.name:
         origin = "basler"
+    else:
+        raise ValueError(f"Cannot identify origin of tif {tif}")
     return origin
 
 
 def get_leica_stack_names(tif_files: list[Path]) -> list:
+    """Get stack names in leica tifs"""
     stack_names = []
     for file in tif_files:
         stack_name = re.findall(r".+(?=_[tz][0-9]+)", file.name)[0]
         if stack_name not in stack_names:
             stack_names.append(stack_name)
     return stack_names
 
 
+def get_basler_stack_names(tif_files: list[Path]) -> list:
+    stack_names = []
+    for file in tif_files:
+        file_name = file.name
+        stack_name = re.findall(r"(?<=__)[0-9]+_[0-9]+", file_name)[0]
+        if stack_name not in stack_names:
+            stack_names.append(stack_name)
+    return stack_names
+
+
 def list_tif_files(folder: Path) -> list:
     """List all tif files in a local folder."""
     tif_files = []
     for element in folder.iterdir():
         if element.is_file():
             if element.suffix in [".tif", ".tiff"]:
                 tif_files.append(element)
     return tif_files
 
 
 def sort_tif_files(tif_files: list[Path]) -> np.ndarray:
-    if "ch00" in tif_files[0].name:
+    """Sort tif files by frame index."""
+    tif_origin = identify_tif_origin(tif_files[0])
+    if tif_origin == "leica":
         frame_numbers = [get_leica_frame_number(x) for x in tif_files]
-    else:
+    elif tif_origin == "basler":
         frame_numbers = [get_basler_frame_number(x) for x in tif_files]
+    else:
+        raise ValueError(f"{tif_origin=} not implemented.")
     check_completeness(frame_numbers)
     sort_vector = np.argsort(frame_numbers)
     tif_files = np.asarray(tif_files)
     tif_files = tif_files[sort_vector]
     return tif_files
 
 
 def get_leica_frame_number(leica_file: Path) -> int:
+    """Extract frame number from leica file name"""
     frame_number = re.findall(r"(?<=[tz])[0-9]+", leica_file.name)[0]
     # print(leica_file.name, frame_number)
     frame_number = int(frame_number)
     return frame_number
 
 
 def get_basler_frame_number(basler_file: Path) -> int:
+    """Extract frame number from basler file name"""
     frame_number = re.findall(r"[0-9]+(?=.tif)", basler_file.name)[0]
     frame_number = int(frame_number)
     return frame_number
 
 
 def check_completeness(frame_numbers: list, verbose: bool = True) -> None:
+    """Check that all frame numbers are present."""
     lowest = np.min(frame_numbers)
     highest = np.max(frame_numbers)
     all_possible = np.arange(lowest, highest)
     if not np.all(np.isin(all_possible, frame_numbers)):
         is_missing = np.logical_not(np.isin(all_possible, frame_numbers))
         missing_numbers = all_possible[is_missing]
         n_missing = np.sum(is_missing)
```

### Comparing `labnas-0.2.1/labnas/local/storage.py` & `labnas-0.2.2/labnas/local/storage.py`

 * *Files identical despite different names*

### Comparing `labnas-0.2.1/labnas/remote/base.py` & `labnas-0.2.2/labnas/remote/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,14 +34,15 @@
             host=host_name,
             username=user_name,
             password=pwd,
         )
         self.logger.info(f"Connection established: {host_name}@{user_name}")
 
     def create_logger(self) -> logging.Logger:
+        """Create a logger to print output to. Optionally save output to file."""
         logger = logging.Logger("nas")
         logger.setLevel(logging.DEBUG)
         stream_handler = logging.StreamHandler(stream=sys.stdout)
         formatter = logging.Formatter("%(asctime)s - %(message)s")
         stream_handler.setFormatter(formatter)
         logger.addHandler(stream_handler)
         if isinstance(self.log_file, Path):
@@ -141,28 +142,38 @@
             local_file = local_folder / remote_file.name
             self.download_file(remote_file, local_file)
         if recursive:
             for remote_sub_folder in folders:
                 self.download_folder(remote_sub_folder, local_folder, recursive=recursive)
         return local_folder
 
-    def upload_folder(self, local_source: Path, remote_parent: PathLike, recursive: bool = True, make_tree: bool = False) -> PathLike:
+    def upload_folder(
+            self,
+            local_source: Path,
+            remote_parent: PathLike,
+            recursive: bool = True,
+            make_tree: bool = False,
+            remote_name: str | None = None,
+    ) -> PathLike:
         """Upload a folder to the NAS"""
         remote_parent = self._convert_to_linux(remote_parent)
         if not local_source.is_dir():
             raise FileNotFoundError(f"{local_source} does not exist.")
         if not self.is_dir(remote_parent):
             if make_tree:
                 self.connection.makedirs(str(remote_parent))
                 self.logger.info(f"Folder tree to {remote_parent} created.")
             else:
                 raise FileNotFoundError(f"{remote_parent} does not exist.")
 
         # create nas folder
-        remote_target = remote_parent / local_source.name
+        if isinstance(remote_name, str):
+            remote_target = remote_parent / remote_name
+        else:
+            remote_target = remote_parent / local_source.name
         if self.connection.isdir(str(remote_target)):
             raise FileExistsError(f"{remote_target} already exists.")
         self.connection.mkdir(str(remote_target))
         self.logger.info(f"Remote folder {remote_target} created.")
 
         # get contents of local folder
         files, folders = self.list_local_files_and_folders(local_source)
```

### Comparing `labnas-0.2.1/labnas/remote/imaging.py` & `labnas-0.2.2/labnas/remote/imaging.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,107 +21,46 @@
     def sort_folder(
             self,
             remote_folder: Path,
             local_temp_folder: Path,
             remote_trash_folder: Path,
             recursive: bool = True,
             level: int = 0,
+            save_one_up: bool = False,
     ) -> None:
-        """Sort a folder with imaging .tif files."""
+        """Sort a folder with imaging .tif files.
+
+        Currently only works for 2p data.
+        """
         self.logger.info(f"=> Investigating: {remote_folder} (Level: {level})")
         if "INCOMPLETE" in remote_folder.name:
             self.logger.info(f"Skipping {remote_folder} -> INCOMPLETE flag.")
         elif "multipage" in remote_folder.name:
             self.logger.info(f"Skipping {remote_folder} -> multipage flag.")
         else:
             stacks, single_tifs = self.check_folder_structure(remote_folder)
             for stack_name, stack_tifs in stacks.items():
                 self.process_stack(
                     stack_name=stack_name,
                     stack_tifs=stack_tifs,
                     remote_folder=remote_folder,
                     local_temp_folder=local_temp_folder,
                     remote_trash_folder=remote_trash_folder,
+                    save_one_up=save_one_up,
                 )
             if recursive:
                 _, folders = self.list_files_and_folders(remote_folder)
                 for folder in folders:
-                    self.sort_folder(folder, local_temp_folder, remote_trash_folder, level=level + 1)
-
-    def process_stack(self, stack_name: str, stack_tifs: list, remote_folder: Path, local_temp_folder: Path, remote_trash_folder: Path) -> None:
-        """
-        1. Download stack as multipage tif.
-        2. Upload multipage tif.
-        3. Delete local multipage tif.
-        4. Delete nas stack tifs.
-        """
-        # set paths
-        remote_tif = remote_folder / "multipage_tiff" / f"{stack_name}.tif"
-        self.logger.info(f"---{remote_tif}---")
-        if self.is_file(remote_tif):
-            raise FileExistsError(f"{remote_tif}")
-        if not self.is_dir(remote_tif.parent):
-            self.create_empty_folder(remote_tif.parent)
-            self.logger.info(f"{remote_tif.parent} created.")
-        self.logger.info(f"Downloading {stack_name} as as single tif.")
-
-        trash_name = remote_folder / stack_name
-        trash_name = str(trash_name).replace("/", "_")
-        stack_trash_folder = remote_trash_folder / trash_name
-        if self.is_file(stack_trash_folder):
-            raise FileExistsError(f"{stack_trash_folder}")
-
-        try:
-            # 1. Download stack as multipage tif
-            local_tif = self.download_files_as_single_tif(
-                tif_files=stack_tifs,
-                file_name=f"{stack_name}.tif",
-                local_folder=local_temp_folder,
-            )
-
-            # 2. Upload multipage tif
-            self.logger.info(f"Uploading {local_tif}")
-            self.upload_file(local_tif, remote_tif)
-            self.logger.info(f"Uploaded {local_tif} as {remote_tif}")
-
-            # 3. Delete local multipage tif
-            self.safely_delete(local_tif)
-
-            # 4. Move stack tifs to trash
-            self.create_empty_folder(stack_trash_folder)
-            self.logger.info(f"Moving stack tifs to {stack_trash_folder}")
-            for file in tqdm(stack_tifs):
-                trash_path = stack_trash_folder / file.name
-                self.move_file(file, trash_path)
-        except (TifFileMissingException, TiffFileError) as e:
-            self.logger.error(f"{e}")
-            self.logger.info("Moving tifs into separate folder instead of combining.")
-            incomplete_target = remote_folder / f"INCOMPLETE_{stack_name}"
-            self.create_empty_folder(incomplete_target)
-            self.logger.info(f"Moving stack tifs to {incomplete_target}")
-            for file in tqdm(stack_tifs):
-                new_path = incomplete_target / file.name
-                self.move_file(file, new_path)
-
-    def safely_delete(self, local_tif: Path, n_attempts: int = 3) -> bool:
-        count = 0
-        successful = False
-        while count < n_attempts:
-            try:
-                os.remove(local_tif)
-                self.logger.info(f"Removed {local_tif}")
-                successful = True
-                break
-            except PermissionError as pe:
-                self.logger.info(f"Could not remove {local_tif} on attempt {count + 1}: {pe}")
-                time.sleep(10)
-                count += 1
-        if not successful:
-            self.logger.warning(f"Failed to remove {local_tif} after {count} attempts.")
-        return successful
+                    self.sort_folder(
+                        remote_folder=folder,
+                        local_temp_folder=local_temp_folder,
+                        remote_trash_folder=remote_trash_folder,
+                        level=level + 1,
+                        save_one_up=save_one_up,
+                    )
 
     def check_folder_structure(self, remote_folder: Path) -> tuple[dict, list]:
         """
         Check if a folder contains .tif files belonging to more than 1 stack.
         Also return stacks and tifs because scanning large folders takes time.
         """
         tifs = self.find_tifs_in_folder(remote_folder)
@@ -130,51 +69,60 @@
             stacks = {}
             single_tifs = []
         elif len(tifs) == 1:
             self.logger.info(f"Only 1 tif: {tifs[0]}.")
             stacks = {}
             single_tifs = tifs
         else:
-            self.logger.info(f"{len(tifs)} tifs in {remote_folder} - looking for stacks.")
+            self.logger.info(f"{len(tifs)} tifs in {remote_folder}.")
             stacks, single_tifs = self.identify_stacks_in_tifs(tifs)
         return stacks, single_tifs
 
     def find_tifs_in_folder(self, remote_folder: Path) -> list[Path]:
-        """Find tif files in a nas folder."""
+        """Find tif files in a remote folder."""
         files, folders = self.list_files_and_folders(remote_folder)
         tifs = self.identify_tifs_in_files(files)
         return tifs
 
     @staticmethod
     def identify_tifs_in_files(files: list[Path]) -> list[Path]:
-        """Identify tif files in a list of files."""
+        """
+        Identify tif files in a list of files.
+        Pretty basic check for file extension.
+        """
         tifs = []
         for file in files:
             if file.suffix in [".tif", ".tiff"]:
                 tifs.append(file)
         return tifs
 
-    def identify_stacks_in_tifs(self, tifs: list[Path]) -> tuple[dict, list]:
-        """Identify if tifs come from multi-frame recordings or if they are single snapshots.."""
-        tif_origin = identify_tif_origin(tifs[0])
+    def identify_stacks_in_tifs(self, tifs: list[Path], catch_error: bool = True) -> tuple[dict, list]:
+        """Identify if tifs come from multi-frame recordings or if they are single snapshots."""
+        self.logger.info("Looking for stacks.")
+        try:
+            tif_origin = identify_tif_origin(tifs[0])
+        except ValueError as ve:
+            if not catch_error:
+                raise ve
+            tif_origin = "unknown"
+
+        self.logger.info(f"File name example: {tifs[0].name}")
+        self.logger.info(f"Tif origin: {tif_origin}")
         if tif_origin == "leica":
-            self.logger.info(f"Tifs (e.g. {tifs[0].name}) identified as leica tifs")
             stacks, single_tifs = self.identify_leica_stacks_in_tifs(tifs)
         elif tif_origin == "basler":
-            self.logger.info(f"Tifs (e.g. {tifs[0].name}) identified as basler tifs")
             stacks, single_tifs = self.identify_basler_stacks_in_tifs(tifs)
         elif tif_origin == "leica_metadata":
-            self.logger.info(f"{tifs[0].parent} identified as leica metadata tifs.")
             single_tifs = tifs
             stacks = {}
         else:
-            self.logger.info(f"Could not identify stacks: neither leica nor basler.")
+            self.logger.info(f"Could not identify tif origin: neither leica nor basler.")
             single_tifs = tifs
             stacks = {}
-        self.logger.info(f"{len(stacks)} tif stacks and {len(single_tifs)} single tifs found.")
+        self.logger.info(f"{len(stacks)} tif stack(s) and {len(single_tifs)} single tif(s) found.")
         return stacks, single_tifs
 
     def identify_leica_stacks_in_tifs(self, tifs: list[Path]) -> tuple[dict, list]:
         """Sort tif files into stacks belonging to a single recording."""
         stacks = {}
         single_tifs = []
         for file in tifs:
@@ -186,51 +134,144 @@
                 stack_name = parts[0]
                 if stack_name not in stacks.keys():
                     self.logger.info(f"Stack in {tifs[0].parent}: {stack_name}")
                     stacks[stack_name] = []
                 stacks[stack_name].append(file)
             else:
                 single_tifs.append(file)
+        stacks, single_tifs = self.check_for_false_stacks(stacks, single_tifs)
+        return stacks, single_tifs
+
+    def check_for_false_stacks(self, stacks: dict, single_tifs: list) -> tuple:
+        """Check for stacks that only contain 1 tif (so they aren't really stacks after all)."""
         keys_to_delete = []
         for stack_name, stack_list in stacks.items():
             if len(stack_list) == 1:
                 single_tifs.append(stack_list[0])
                 keys_to_delete.append(stack_name)
                 self.logger.info(f"Only 1 tif in stack {stack_name} -> Appending to single tifs.")
         for key in keys_to_delete:
             del stacks[key]
         return stacks, single_tifs
 
-    @staticmethod
-    def identify_basler_stacks_in_tifs(tifs: list[Path]) -> tuple[dict, list]:
+    def identify_basler_stacks_in_tifs(self, tifs: list[Path]) -> tuple[dict, list]:
         """Sort tif files into stacks belonging to a single recording."""
         stacks = {}
         single_tifs = []
         for file in tifs:
             parts = file.name.split("_")
             index_part = parts[-1]
             stack_name = "_".join(parts[:-1])
             if stack_name not in stacks.keys():
                 stacks[stack_name] = []
             stacks[stack_name].append(file)
+        stacks, single_tifs = self.check_for_false_stacks(stacks, single_tifs)
         return stacks, single_tifs
 
+    def process_stack(
+            self,
+            stack_name: str,
+            stack_tifs: list,
+            remote_folder: Path,
+            local_temp_folder: Path,
+            remote_trash_folder: Path,
+            save_one_up: bool,
+    ) -> None:
+        """
+        TODO: split this
+        1. Download stack as multipage tif.
+        2. Upload multipage tif.
+        3. Delete local multipage tif.
+        4. Delete nas stack tifs.
+        """
+        # set paths
+        if save_one_up:
+            file_name = f"{remote_folder.name}_{stack_name}.tif"
+            self.logger.info(f"Using parent folder and stack name as file name: {file_name}.")
+            remote_tif = remote_folder.parent / "multipage_tiff" / file_name
+            self.logger.info(f"Saving multipage-tiff one level up: {remote_tif}")
+        else:
+            remote_tif = remote_folder / "multipage_tiff" / f"{stack_name}.tif"
+        self.logger.info(f"---{remote_tif}---")
+        if self.is_file(remote_tif):
+            raise FileExistsError(f"{remote_tif}")
+        if not self.is_dir(remote_tif.parent):
+            self.create_empty_folder(remote_tif.parent)
+            self.logger.info(f"{remote_tif.parent} created.")
+        self.logger.info(f"Downloading {stack_name} as as single tif.")
+
+        trash_name = remote_folder / stack_name
+        trash_name = str(trash_name).replace("/", "_")
+        stack_trash_folder = remote_trash_folder / trash_name
+        if self.is_file(stack_trash_folder):
+            raise FileExistsError(f"{stack_trash_folder}")
+
+        try:
+            # 1. Download stack as multipage tif
+            local_tif = self.download_files_as_single_tif(
+                tif_files=stack_tifs,
+                file_name=f"{stack_name}.tif",
+                local_folder=local_temp_folder,
+            )
+
+            # 2. Upload multipage tif
+            self.logger.info(f"Uploading {local_tif}")
+            self.upload_file(local_tif, remote_tif)
+            self.logger.info(f"Uploaded {local_tif} as {remote_tif}")
+
+            # 3. Delete local multipage tif
+            self.safely_delete(local_tif)
+
+            # 4. Move stack tifs to trash
+            self.create_empty_folder(stack_trash_folder)
+            self.logger.info(f"Moving stack tifs to {stack_trash_folder}")
+            for file in tqdm(stack_tifs):
+                trash_path = stack_trash_folder / file.name
+                self.move_file(file, trash_path)
+        except (TifFileMissingException, TiffFileError) as e:
+            self.logger.error(f"{e}")
+            self.logger.info("Moving tifs into separate folder instead of combining.")
+            incomplete_target = remote_folder / f"INCOMPLETE_{stack_name}"
+            self.create_empty_folder(incomplete_target)
+            self.logger.info(f"Moving stack tifs to {incomplete_target}")
+            for file in tqdm(stack_tifs):
+                new_path = incomplete_target / file.name
+                self.move_file(file, new_path)
+
+    def safely_delete(self, local_tif: Path, n_attempts: int = 3) -> bool:
+        count = 0
+        successful = False
+        while count < n_attempts:
+            try:
+                os.remove(local_tif)
+                self.logger.info(f"Removed {local_tif}")
+                successful = True
+                break
+            except PermissionError as pe:
+                self.logger.info(f"Could not remove {local_tif} on attempt {count + 1}: {pe}")
+                time.sleep(10)
+                count += 1
+        if not successful:
+            self.logger.warning(f"Failed to remove {local_tif} after {count} attempts.")
+        return successful
+
     def create_folder_for_stack(self, stack_name: str, remote_folder: Path, stack_files: list[Path]) -> None:
         """Move .tif files belonging to a single stack into a dedicated folder."""
         self.logger.info(f"{len(stack_files)} tifs in stack {stack_name}.")
         parent_directory = remote_folder / stack_name
         if parent_directory.is_dir():
             raise FileExistsError(f"{parent_directory}")
         self.connection.mkdir(str(parent_directory))
         for file in tqdm(stack_files):
             new_path = parent_directory / file.name
             self.move_file(file, new_path)
         self.logger.info(f"Moved {len(stack_files)} tifs into {parent_directory}.")
 
     def download_files_as_single_tif(self, tif_files: list, file_name: str, local_folder: Path) -> Path:
+        """Download multiple 2D tif files and combine to single 3D tif."""
         temp_local = local_folder / "temp.tif"
         multipage_local = local_folder / file_name
         assert multipage_local.suffix == ".tif"
 
         n_files = len(tif_files)
         self.logger.info(f"{len(tif_files)} tif files")
         assert n_files > 1, f"Not enough files: {n_files=} < 1"
@@ -277,7 +318,9 @@
                 )
                 store = tifffile.imread(multipage_local, mode="r+", aszarr=True)
                 z = zarr.open(store, mode="r+")
                 self.logger.info(f"Empty tif created: {shape}")
             z[i_file, :, :] = image
         os.remove(local_folder / "temp.tif")
         return multipage_local
+
+
```

