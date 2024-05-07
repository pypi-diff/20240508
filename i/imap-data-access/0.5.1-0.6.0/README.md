# Comparing `tmp/imap_data_access-0.5.1.tar.gz` & `tmp/imap_data_access-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imap_data_access-0.5.1.tar", last modified: Fri Apr 19 14:35:36 2024, max compression
+gzip compressed data, was "imap_data_access-0.6.0.tar", last modified: Tue May  7 22:00:59 2024, max compression
```

## Comparing `imap_data_access-0.5.1.tar` & `imap_data_access-0.6.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:35:36.261167 imap_data_access-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-19 14:35:28.000000 imap_data_access-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7267 2024-04-19 14:35:36.261167 imap_data_access-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6024 2024-04-19 14:35:28.000000 imap_data_access-0.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:35:36.257167 imap_data_access-0.5.1/imap_data_access/
--rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-04-19 14:35:28.000000 imap_data_access-0.5.1/imap_data_access/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9036 2024-04-19 14:35:28.000000 imap_data_access-0.5.1/imap_data_access/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     9903 2024-04-19 14:35:28.000000 imap_data_access-0.5.1/imap_data_access/file_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     7266 2024-04-19 14:35:28.000000 imap_data_access-0.5.1/imap_data_access/io.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:35:36.257167 imap_data_access-0.5.1/imap_data_access.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7267 2024-04-19 14:35:36.000000 imap_data_access-0.5.1/imap_data_access.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-19 14:35:36.000000 imap_data_access-0.5.1/imap_data_access.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 14:35:36.000000 imap_data_access-0.5.1/imap_data_access.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-19 14:35:36.000000 imap_data_access-0.5.1/imap_data_access.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 14:35:36.000000 imap_data_access-0.5.1/imap_data_access.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-19 14:35:36.000000 imap_data_access-0.5.1/imap_data_access.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-04-19 14:35:28.000000 imap_data_access-0.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 14:35:36.261167 imap_data_access-0.5.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:35:36.257167 imap_data_access-0.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-04-19 14:35:28.000000 imap_data_access-0.5.1/tests/test_config_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     5823 2024-04-19 14:35:28.000000 imap_data_access-0.5.1/tests/test_file_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)    10273 2024-04-19 14:35:28.000000 imap_data_access-0.5.1/tests/test_io.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:00:59.089087 imap_data_access-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-07 22:00:51.000000 imap_data_access-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7267 2024-05-07 22:00:59.089087 imap_data_access-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6024 2024-05-07 22:00:51.000000 imap_data_access-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:00:59.085087 imap_data_access-0.6.0/imap_data_access/
+-rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-05-07 22:00:51.000000 imap_data_access-0.6.0/imap_data_access/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9467 2024-05-07 22:00:51.000000 imap_data_access-0.6.0/imap_data_access/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12241 2024-05-07 22:00:51.000000 imap_data_access-0.6.0/imap_data_access/file_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7735 2024-05-07 22:00:51.000000 imap_data_access-0.6.0/imap_data_access/io.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:00:59.089087 imap_data_access-0.6.0/imap_data_access.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7267 2024-05-07 22:00:59.000000 imap_data_access-0.6.0/imap_data_access.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-07 22:00:59.000000 imap_data_access-0.6.0/imap_data_access.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 22:00:59.000000 imap_data_access-0.6.0/imap_data_access.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-07 22:00:59.000000 imap_data_access-0.6.0/imap_data_access.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 22:00:59.000000 imap_data_access-0.6.0/imap_data_access.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-07 22:00:59.000000 imap_data_access-0.6.0/imap_data_access.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-05-07 22:00:51.000000 imap_data_access-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 22:00:59.089087 imap_data_access-0.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:00:59.089087 imap_data_access-0.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-05-07 22:00:51.000000 imap_data_access-0.6.0/tests/test_config_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6209 2024-05-07 22:00:51.000000 imap_data_access-0.6.0/tests/test_file_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10457 2024-05-07 22:00:51.000000 imap_data_access-0.6.0/tests/test_io.py
```

### Comparing `imap_data_access-0.5.1/LICENSE` & `imap_data_access-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `imap_data_access-0.5.1/PKG-INFO` & `imap_data_access-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imap-data-access
-Version: 0.5.1
+Version: 0.6.0
 Summary: IMAP SDC Data Access
 Author-email: IMAP SDC Developers <imap-sdc@lists.lasp.colorado.edu>
 License: MIT
 Project-URL: homepage, https://github.com/IMAP-Science-Operations-Center
 Project-URL: repository, https://github.com/IMAP-Science-Operations-Center/imap-data-access
 Keywords: IMAP,SDC,SOC,SDS,Science Operations
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `imap_data_access-0.5.1/README.md` & `imap_data_access-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `imap_data_access-0.5.1/imap_data_access/__init__.py` & `imap_data_access-0.6.0/imap_data_access/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,42 +4,47 @@
 heliosphere. This package contains the data access tools for the IMAP mission. It
 provides a convenient way to query the IMAP data archive and download data files.
 """
 
 import os
 from pathlib import Path
 
-from imap_data_access.file_validation import ScienceFilePath
+from imap_data_access.file_validation import ScienceFilePath, SPICEFilePath
 from imap_data_access.io import download, query, upload
 
 __all__ = [
     "query",
     "download",
     "upload",
     "ScienceFilePath",
+    "SPICEFilePath",
     "VALID_INSTRUMENTS",
     "VALID_DATALEVELS",
     "VALID_FILE_EXTENSION",
     "FILENAME_CONVENTION",
 ]
-__version__ = "0.5.1"
+__version__ = "0.6.0"
 
 
 config = {
     "DATA_ACCESS_URL": os.getenv("IMAP_DATA_ACCESS_URL")
     or "https://api.dev.imap-mission.com",
     "DATA_DIR": Path(os.getenv("IMAP_DATA_DIR") or Path.cwd() / "data"),
+    "API_KEY": os.getenv("IMAP_API_KEY"),
 }
 """Settings configuration dictionary.
 
 DATA_ACCESS_URL : This is the URL of the data access API.
 DATA_DIR : This is where the file data is stored and organized by instrument and level.
     The default location is a 'data/' folder in the current working directory,
     "but this can be set on the command line using the --data-dir option, or through
     the environment variable IMAP_DATA_DIR.
+API_KEY : This is the API key used to authenticate with the data access API.
+    It can be set on the command line using the --api-key option, or through the
+    environment variable IMAP_API_KEY. It is only necessary for uploading files.
 """
 
 
 VALID_INSTRUMENTS = {
     "codice",
     "glows",
     "hit",
```

### Comparing `imap_data_access-0.5.1/imap_data_access/cli.py` & `imap_data_access-0.6.0/imap_data_access/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     """
     num_files = len(query_results)
     print(f"Found [{num_files}] matching files")
     if num_files == 0:
         return
     format_string = "{:<10}|{:<10}|{:<10}|{:<10}|{:<10}|{:<7}|{:<50}|"
     # Add hyphens for a separator between header and data
-    hyphens = "-" * 111 + "|"
+    hyphens = "-" * 113 + "|"
     print(hyphens)
     header = [
         "Instrument",
         "Data Level",
         "Descriptor",
         "Start Date",
         "Repointing",
@@ -135,14 +135,19 @@
 
 
 def main():
     """Parse the command line arguments.
 
     Run the command line interface to the IMAP Data Access API.
     """
+    api_key_help = (
+        "API key to authenticate with the IMAP SDC. "
+        "This can also be set using the IMAP_API_KEY environment variable. "
+        "It is only necessary for uploading files."
+    )
     data_dir_help = (
         "Directory to use for reading and writing IMAP data. "
         "The default is a 'data/' folder in the "
         "current working directory. This can also be "
         "set using the IMAP_DATA_DIR environment variable."
     )
     description = (
@@ -172,14 +177,15 @@
 
     parser = argparse.ArgumentParser(prog="imap-data-access", description=description)
     parser.add_argument(
         "--version",
         action="version",
         version=f"%(prog)s {imap_data_access.__version__}",
     )
+    parser.add_argument("--api-key", type=str, required=False, help=api_key_help)
     parser.add_argument("--data-dir", type=Path, required=False, help=data_dir_help)
     parser.add_argument("--url", type=str, required=False, help=url_help)
     # Logging level
     parser.add_argument(
         "--debug",
         help="Print lots of debugging statements",
         action="store_const",
@@ -285,14 +291,18 @@
         # Set the data directory to the user-supplied value
         imap_data_access.config["DATA_DIR"] = data_path
 
     if args.url:
         # We got an explicit url from the command line
         imap_data_access.config["DATA_ACCESS_URL"] = args.url
 
+    if args.api_key:
+        # We got an explicit api key from the command line
+        imap_data_access.config["API_KEY"] = args.api_key
+
     # Now process through the respective function for the invoked command
     # (set with set_defaults on the subparsers above)
     try:
         args.func(args)
     except Exception as e:
         parser.error(e)
```

### Comparing `imap_data_access-0.5.1/imap_data_access/file_validation.py` & `imap_data_access-0.6.0/imap_data_access/file_validation.py`

 * *Files 21% similar despite different names*

```diff
@@ -272,7 +272,87 @@
             )
 
         components = match.groupdict()
         if components["repointing"]:
             # We want the repointing number as an integer
             components["repointing"] = int(components["repointing"])
         return components
+
+
+# Transform the suffix to the directory structure we are using
+# Commented out mappings are not being used on IMAP
+_SPICE_DIR_MAPPING = {
+    ".bc": "ck",
+    # ".bds": "dsk",
+    # ".bes": "ek",
+    ".bpc": "pck",
+    ".bsp": "spk",
+    ".tf": "fk",
+    # "ti": "ik",
+    ".tls": "lsk",
+    ".tm": "mk",
+    ".tpc": "pck",
+    ".tsc": "sclk",
+}
+"""These are the valid extensions for SPICE files according to NAIF
+https://naif.jpl.nasa.gov/pub/naif/toolkit_docs/C/req/kernel.html
+
+.bc    binary CK
+.bds   binary DSK
+.bes   binary Sequence Component EK
+.bpc   binary PCK
+.bsp   binary SPK
+.tf    text FK
+.ti    text IK
+.tls   text LSK
+.tm    text meta-kernel (FURNSH kernel)
+.tpc   text PCK
+.tsc   text SCLK
+"""
+
+
+class SPICEFilePath:
+    """Class for building and validating filepaths for SPICE files."""
+
+    class InvalidSPICEFileError(Exception):
+        """Indicates a bad file type."""
+
+        pass
+
+    def __init__(self, filename: str | Path):
+        """Class to store filepath and file management methods for SPICE files.
+
+        If you have an instance of this class, you can be confident you have a valid
+        SPICE file and generate paths in the correct format. The parent of the file
+        path is set by the "IMAP_DATA_DIR" environment variable, or defaults to "data/"
+
+        IMAP_DATA_DIR/spice/<subdir>/filename"
+
+        Parameters
+        ----------
+        filename : str | Path
+            SPICE data filename or file path.
+        """
+        self.filename = Path(filename)
+
+        if self.filename.suffix not in _SPICE_DIR_MAPPING:
+            raise self.InvalidSPICEFileError(
+                f"Invalid SPICE file. Expected file to have one of the following "
+                f"extensions {list(_SPICE_DIR_MAPPING.keys())}"
+            )
+
+    def construct_path(self) -> Path:
+        """Construct valid path from the class variables and data_dir.
+
+        expected return:
+        <data_dir>/imap/spice/<subdir>/filename
+
+        Returns
+        -------
+        Path
+            Upload path
+        """
+        spice_dir = imap_data_access.config["DATA_DIR"] / "imap/spice"
+        subdir = _SPICE_DIR_MAPPING[self.filename.suffix]
+        # Use the file suffix to determine the directory structure
+        # IMAP_DATA_DIR/imap/spice/<subdir>/filename
+        return spice_dir / subdir / self.filename
```

### Comparing `imap_data_access-0.5.1/imap_data_access/io.py` & `imap_data_access-0.6.0/imap_data_access/io.py`

 * *Files 7% similar despite different names*

```diff
@@ -57,24 +57,27 @@
 
     Returns
     -------
     pathlib.Path
         Path to the downloaded file
     """
     destination = imap_data_access.config["DATA_DIR"]
-    if isinstance(file_path, str) and "/" not in file_path:
-        # Construct the directory structure from the filename
-        # This is for science files that contain the directory structure in the filename
-        # Otherwise, we assume the full path to the file was given
+    # Create the proper file path object based on the extension and filename
+    file_path = Path(file_path)
+    if file_path.suffix in imap_data_access.file_validation._SPICE_DIR_MAPPING:
+        # SPICE
+        path_obj = imap_data_access.SPICEFilePath(file_path.name)
+    else:
+        # Science
+        path_obj = imap_data_access.ScienceFilePath(file_path.name)
 
-        science_file_path = imap_data_access.ScienceFilePath(file_path)
+    destination = path_obj.construct_path()
 
-        destination = science_file_path.construct_path()
-    else:
-        destination /= file_path
+    # Update the file_path with the full path for the download below
+    file_path = destination.relative_to(imap_data_access.config["DATA_DIR"]).as_posix()
 
     # Only download if the file doesn't already exist
     # TODO: Do we want to verify any hashes to make sure we have the right file?
     if destination.exists():
         logger.info("The file %s already exists, skipping download", destination)
         return destination
 
@@ -151,22 +154,25 @@
         logger.debug("Received response: %s", items)
         # Decode the JSON string into a list
         items = json.loads(items)
         logger.debug("Decoded JSON: %s", items)
     return items
 
 
-def upload(file_path: Union[Path, str]) -> None:
+def upload(file_path: Union[Path, str], *, api_key: Optional[str] = None) -> None:
     """Upload a file to the data archive.
 
     Parameters
     ----------
     file_path : pathlib.Path or str
         Path to the file to upload. It must be located within
         the ``imap_data_access.config["DATA_DIR"]`` directory.
+    api_key : str, optional
+        API key to authenticate with the data access API. If not provided,
+        the value from the IMAP_API_KEY environment variable will be used.
     """
     file_path = Path(file_path).resolve()
     if not file_path.exists():
         raise FileNotFoundError(file_path)
 
     if not file_path.is_relative_to(imap_data_access.config["DATA_DIR"]):
         raise ValueError(
@@ -181,18 +187,20 @@
     )
 
     url = f"{imap_data_access.config['DATA_ACCESS_URL']}"
     # The upload name needs to be given as a path parameter
     url += f"/upload/{upload_name}"
     logger.info("Uploading file %s to %s", file_path, url)
 
+    # Create a request header with the API key
+    api_key = api_key or imap_data_access.config["API_KEY"]
     # We send a GET request with the filename and the server
     # will respond with an s3 presigned URL that we can use
     # to upload the file to the data archive
-    request = urllib.request.Request(url, method="GET")
+    request = urllib.request.Request(url, method="GET", headers={"X-api-key": api_key})
 
     with _get_url_response(request) as response:
         # Retrieve the key for the upload
         s3_url = response.read().decode("utf-8")
         logger.debug("Received s3 presigned URL: %s", s3_url)
         s3_url = json.loads(s3_url)
```

### Comparing `imap_data_access-0.5.1/imap_data_access.egg-info/PKG-INFO` & `imap_data_access-0.6.0/imap_data_access.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imap-data-access
-Version: 0.5.1
+Version: 0.6.0
 Summary: IMAP SDC Data Access
 Author-email: IMAP SDC Developers <imap-sdc@lists.lasp.colorado.edu>
 License: MIT
 Project-URL: homepage, https://github.com/IMAP-Science-Operations-Center
 Project-URL: repository, https://github.com/IMAP-Science-Operations-Center/imap-data-access
 Keywords: IMAP,SDC,SOC,SDS,Science Operations
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `imap_data_access-0.5.1/pyproject.toml` & `imap_data_access-0.6.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "imap-data-access"
-version = "0.5.1"
+version = "0.6.0"
 description = "IMAP SDC Data Access"
 authors = [{name = "IMAP SDC Developers", email = "imap-sdc@lists.lasp.colorado.edu"}]
 readme = "README.md"
 license = {text = "MIT"}
 keywords = ["IMAP", "SDC", "SOC", "SDS", "Science Operations"]
 classifiers = [
     "Development Status :: 3 - Alpha",
```

### Comparing `imap_data_access-0.5.1/tests/test_file_validation.py` & `imap_data_access-0.6.0/tests/test_file_validation.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Tests for the ``file_validataion`` module."""
 
 from pathlib import Path
 
 import pytest
 
 import imap_data_access
-from imap_data_access.file_validation import ScienceFilePath
+from imap_data_access.file_validation import ScienceFilePath, SPICEFilePath
 
 
 def test_extract_filename_components():
     """Tests the ``extract_filename_components`` function."""
     valid_filename = "imap_mag_l1a_burst_20210101_v001.pkts"
 
     expected_output = {
@@ -165,7 +165,19 @@
         "v001",
         repointing=1,
     )
     expected_output = imap_data_access.config["DATA_DIR"] / Path(
         "imap/mag/l0/2021/01/imap_mag_l0_raw_20210101-repoint00001_v001.pkts"
     )
     assert sfm.construct_path() == expected_output
+
+
+def test_spice_file_path():
+    """Tests the ``SPICEFilePath`` class."""
+    file_path = SPICEFilePath("test.bc")
+    assert file_path.construct_path() == imap_data_access.config["DATA_DIR"] / Path(
+        "imap/spice/ck/test.bc"
+    )
+
+    # Test a bad file extension too
+    with pytest.raises(SPICEFilePath.InvalidSPICEFileError):
+        SPICEFilePath("test.txt")
```

### Comparing `imap_data_access-0.5.1/tests/test_io.py` & `imap_data_access-0.6.0/tests/test_io.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,14 +12,17 @@
 from urllib.parse import urlencode
 from urllib.request import Request
 
 import pytest
 
 import imap_data_access
 
+test_science_filename = "imap_swe_l1_test-description_20100101_v000.cdf"
+test_science_path = "imap/swe/l1/2010/01/" + test_science_filename
+
 
 @pytest.fixture()
 def mock_urlopen():
     """Mock urlopen to return a file-like object.
 
     Yields
     ------
@@ -56,34 +59,36 @@
         Mock object for ``urlopen``
     """
     # Set up the mock to raise an HTTPError
     mock_urlopen.side_effect = HTTPError(
         url="http://example.com", code=404, msg="Not Found", hdrs={}, fp=BytesIO()
     )
     with pytest.raises(imap_data_access.io.IMAPDataAccessError, match="HTTP Error"):
-        imap_data_access.download("test/test.txt")
+        imap_data_access.download(test_science_path)
 
     # Set up the mock to raise a URLError
     mock_urlopen.side_effect = URLError(reason="Not Found")
     with pytest.raises(imap_data_access.io.IMAPDataAccessError, match="URL Error"):
-        imap_data_access.download("test/test.txt")
+        imap_data_access.download(test_science_path)
 
 
 @pytest.mark.parametrize(
     ("file_path", "destination"),
     [
         # Directory structure inferred
         (
-            "imap_swe_l1_test-description_20100101_v000.cdf",
-            "imap/swe/l1/2010/01/imap_swe_l1_test-description_20100101_v000.cdf",
+            test_science_filename,
+            test_science_path,
         ),
         # Directory structure provided in the request
-        ("imap/test/config/file.txt", "imap/test/config/file.txt"),
+        (test_science_path, test_science_path),
         # Pathlib.Path object
-        (Path("imap/test/config/file.txt"), "imap/test/config/file.txt"),
+        (Path(test_science_path), test_science_path),
+        # SPICE file
+        ("test.bc", "imap/spice/ck/test.bc"),
     ],
 )
 def test_download(
     mock_urlopen: unittest.mock.MagicMock, file_path: str | Path, destination: str
 ):
     """Test that the download API works as expected.
 
@@ -115,35 +120,33 @@
     # Assert that the correct URL was used for the download
     urlopen_calls = mock_urlopen.mock_calls
     # Check the arguments passed to urlopen
     # We pass a Request object, so need to get that with args[0]
     request_sent = urlopen_calls[0].args[0]
     called_url = request_sent.full_url
     # url should be provided as path parameters
-    expected_url_encoded = f"https://api.test.com/download/{file_path}"
+    expected_url_encoded = f"https://api.test.com/download/{destination}"
     assert called_url == expected_url_encoded
     assert request_sent.method == "GET"
 
 
 def test_download_already_exists(mock_urlopen: unittest.mock.MagicMock):
     """Test that downloading a file that already exists does result in any requests.
 
     Parameters
     ----------
     mock_urlopen : unittest.mock.MagicMock
         Mock object for ``urlopen``
     """
     # Call the download function
-    file_path = "a/b.txt"
     # set up the destination and create a file
-    destination = Path(imap_data_access.config["DATA_DIR"])
-    destination /= f"{file_path}"
+    destination = imap_data_access.config["DATA_DIR"] / test_science_path
     destination.parent.mkdir(parents=True, exist_ok=True)
     destination.touch(exist_ok=True)
-    result = imap_data_access.download(file_path)
+    result = imap_data_access.download(test_science_path)
     assert result == destination
     # Make sure we didn't make any requests
     assert mock_urlopen.call_count == 0
 
 
 @pytest.mark.parametrize(
     "query_params",
@@ -290,14 +293,16 @@
     # First urlopen call should be to get the s3 upload url
     urlopen_call = mock_calls[0]
     request_sent = urlopen_call.args[0]
     called_url = request_sent.full_url
     expected_url_encoded = "https://api.test.com/upload/a/b/test-file.txt"
     assert called_url == expected_url_encoded
     assert request_sent.method == "GET"
+    # An API key needs to be added to the header for uploads
+    assert request_sent.headers == {"X-api-key": "test-api-key"}
 
     # Verify that we put that response into our second request
     urlopen_call = mock_calls[1]
     request_sent = urlopen_call.args[0]
     called_url = request_sent.full_url
     expected_url_encoded = "https://s3-test-bucket.com"
     assert called_url == expected_url_encoded
```

