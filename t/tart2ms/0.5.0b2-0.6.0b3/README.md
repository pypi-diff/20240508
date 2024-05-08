# Comparing `tmp/tart2ms-0.5.0b2.tar.gz` & `tmp/tart2ms-0.6.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tart2ms-0.5.0b2.tar", last modified: Wed Feb  1 22:44:01 2023, max compression
+gzip compressed data, was "tart2ms-0.6.0b3.tar", last modified: Wed May  8 03:15:22 2024, max compression
```

## Comparing `tart2ms-0.5.0b2.tar` & `tart2ms-0.6.0b3.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 22:44:01.032901 tart2ms-0.5.0b2/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-02-01 22:43:47.000000 tart2ms-0.5.0b2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-02-01 22:43:47.000000 tart2ms-0.5.0b2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6178 2023-02-01 22:44:01.032901 tart2ms-0.5.0b2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5357 2023-02-01 22:43:47.000000 tart2ms-0.5.0b2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 22:44:01.000899 tart2ms-0.5.0b2/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)    12571 2023-02-01 22:43:47.000000 tart2ms-0.5.0b2/bin/tart2ms
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-01 22:44:01.032901 tart2ms-0.5.0b2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-02-01 22:43:47.000000 tart2ms-0.5.0b2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 22:44:01.000899 tart2ms-0.5.0b2/tart2ms/
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-02-01 22:43:47.000000 tart2ms-0.5.0b2/tart2ms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 22:44:01.032901 tart2ms-0.5.0b2/tart2ms/catalogs/
--rw-r--r--   0 runner    (1001) docker     (123)    12468 2023-02-01 22:43:47.000000 tart2ms-0.5.0b2/tart2ms/catalogs/3CRR
--rw-r--r--   0 runner    (1001) docker     (123)    14083 2023-02-01 22:43:47.000000 tart2ms-0.5.0b2/tart2ms/catalogs/MeerKAT_gaincal_list
--rwxr-xr-x   0 runner    (1001) docker     (123) 21275138 2023-02-01 22:43:47.000000 tart2ms-0.5.0b2/tart2ms/catalogs/SUMMS
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-01 22:43:47.000000 tart2ms-0.5.0b2/tart2ms/catalogs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5313 2023-02-01 22:43:47.000000 tart2ms-0.5.0b2/tart2ms/catalogs/catalog_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    13525 2023-02-01 22:43:47.000000 tart2ms-0.5.0b2/tart2ms/fixvis.py
--rw-r--r--   0 runner    (1001) docker     (123)    11213 2023-02-01 22:43:47.000000 tart2ms-0.5.0b2/tart2ms/ms_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-02-01 22:43:47.000000 tart2ms-0.5.0b2/tart2ms/named_phasings.json
--rw-r--r--   0 runner    (1001) docker     (123)    10083 2023-02-01 22:43:47.000000 tart2ms-0.5.0b2/tart2ms/read_ms.py
--rw-r--r--   0 runner    (1001) docker     (123)    67331 2023-02-01 22:43:47.000000 tart2ms-0.5.0b2/tart2ms/tart2ms.py
--rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-02-01 22:43:47.000000 tart2ms-0.5.0b2/tart2ms/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 22:44:01.004899 tart2ms-0.5.0b2/tart2ms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6178 2023-02-01 22:44:00.000000 tart2ms-0.5.0b2/tart2ms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-02-01 22:44:00.000000 tart2ms-0.5.0b2/tart2ms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-01 22:44:00.000000 tart2ms-0.5.0b2/tart2ms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-02-01 22:44:00.000000 tart2ms-0.5.0b2/tart2ms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-02-01 22:44:00.000000 tart2ms-0.5.0b2/tart2ms.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:15:22.075232 tart2ms-0.6.0b3/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-08 03:15:17.000000 tart2ms-0.6.0b3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-08 03:15:17.000000 tart2ms-0.6.0b3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6957 2024-05-08 03:15:22.075232 tart2ms-0.6.0b3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5851 2024-05-08 03:15:17.000000 tart2ms-0.6.0b3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:15:22.047232 tart2ms-0.6.0b3/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13453 2024-05-08 03:15:17.000000 tart2ms-0.6.0b3/bin/tart2ms
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 03:15:22.075232 tart2ms-0.6.0b3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-05-08 03:15:17.000000 tart2ms-0.6.0b3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:15:22.047232 tart2ms-0.6.0b3/tart2ms/
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-08 03:15:17.000000 tart2ms-0.6.0b3/tart2ms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10034 2024-05-08 03:15:17.000000 tart2ms-0.6.0b3/tart2ms/casa_read_ms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:15:22.075232 tart2ms-0.6.0b3/tart2ms/catalogs/
+-rw-r--r--   0 runner    (1001) docker     (127)    12468 2024-05-08 03:15:17.000000 tart2ms-0.6.0b3/tart2ms/catalogs/3CRR
+-rw-r--r--   0 runner    (1001) docker     (127)    14083 2024-05-08 03:15:17.000000 tart2ms-0.6.0b3/tart2ms/catalogs/MeerKAT_gaincal_list
+-rwxr-xr-x   0 runner    (1001) docker     (127) 21275138 2024-05-08 03:15:17.000000 tart2ms-0.6.0b3/tart2ms/catalogs/SUMMS
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 03:15:17.000000 tart2ms-0.6.0b3/tart2ms/catalogs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5313 2024-05-08 03:15:17.000000 tart2ms-0.6.0b3/tart2ms/catalogs/catalog_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13494 2024-05-08 03:15:17.000000 tart2ms-0.6.0b3/tart2ms/fixvis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11183 2024-05-08 03:15:17.000000 tart2ms-0.6.0b3/tart2ms/ms_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-05-08 03:15:17.000000 tart2ms-0.6.0b3/tart2ms/named_phasings.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10779 2024-05-08 03:15:17.000000 tart2ms-0.6.0b3/tart2ms/read_ms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    69511 2024-05-08 03:15:17.000000 tart2ms-0.6.0b3/tart2ms/tart2ms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4383 2024-05-08 03:15:17.000000 tart2ms-0.6.0b3/tart2ms/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:15:22.075232 tart2ms-0.6.0b3/tart2ms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6957 2024-05-08 03:15:22.000000 tart2ms-0.6.0b3/tart2ms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-05-08 03:15:22.000000 tart2ms-0.6.0b3/tart2ms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 03:15:22.000000 tart2ms-0.6.0b3/tart2ms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-08 03:15:22.000000 tart2ms-0.6.0b3/tart2ms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-08 03:15:22.000000 tart2ms-0.6.0b3/tart2ms.egg-info/top_level.txt
```

### Comparing `tart2ms-0.5.0b2/LICENSE.txt` & `tart2ms-0.6.0b3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tart2ms-0.5.0b2/PKG-INFO` & `tart2ms-0.6.0b3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,7 @@
-Metadata-Version: 2.1
-Name: tart2ms
-Version: 0.5.0b2
-Summary: Convert TART observation data to Measurement Sets
-Home-page: http://github.com/tmolteno/tart2ms
-Author: Tim Molteno
-Author-email: tim@elec.ac.nz
-License: GPLv3
-Classifier: Development Status :: 4 - Beta
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Communications :: Ham Radio
-Classifier: Operating System :: OS Independent
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Intended Audience :: Science/Research
-Description-Content-Type: text/markdown
-Provides-Extra: predict
-License-File: LICENSE.txt
-
 # tart2ms
 
 [![PyPI package](https://img.shields.io/badge/pip%20install-tart2ms-brightgreen)](https://pypi.org/project/tart2ms) [![version number](https://img.shields.io/pypi/v/tart2ms?color=green&label=version)](https://github.com/tart-telescope/tart2ms/releases) [![License](https://img.shields.io/github/license/tart-telescope/tart2ms)](https://github.com/tart-telescope/tart2ms/blob/master/LICENSE.txt)
 
 
 Convert data from a [TART radio telescope](https://tart.elec.ac.nz) to measurement set format. This module relies on the excellent dask-ms module as a helper to create the measurement sets. This packate requires python-casacore to be installed on your system
 
@@ -110,14 +88,21 @@
 
 ## TODO
 
 - 
 
 ## Changelog
 
+- 0.6.0b3 If WEIGHT_SPECTRUM is not present, then subsititude ones
+- 0.6.0b2 Clean up the logging code. Add a --debug flag.
+          Get rid of the annoying printing of casa tables
+- 0.6.0b1 New casa_read_ms function similar to read_ms, but uses casacore - blindingly fast.
+          made function signatures the same for both read_ms() and casa_read_ms().
+- 0.5.0b3 Remove noisy warnings. Add venv makefile.
+          Output the snapshot direction in 12-ball format to make rephasing easier.
 - 0.5.0b2 Make prediction an optional dependency to remove codex-africanus from requirements.
 - 0.5.0b1 Add model prediction
           Add automatic catalog download
 - 0.4.0b3 Use the new catalog url functions from tart_tools
 - 0.4.0b2 Add a helper function get_array_location
 - 0.4.0b1 Add a tart2ms.read_ms function (from disko)
           Add utilities for resolution calculations.
```

### Comparing `tart2ms-0.5.0b2/README.md` & `tart2ms-0.6.0b3/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,40 @@
+Metadata-Version: 2.1
+Name: tart2ms
+Version: 0.6.0b3
+Summary: Convert TART observation data to Measurement Sets
+Home-page: http://github.com/tmolteno/tart2ms
+Author: Tim Molteno
+Author-email: tim@elec.ac.nz
+License: GPLv3
+Classifier: Development Status :: 4 - Beta
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Communications :: Ham Radio
+Classifier: Operating System :: OS Independent
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Intended Audience :: Science/Research
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+Requires-Dist: dask-ms
+Requires-Dist: python-casacore
+Requires-Dist: tart
+Requires-Dist: tart_tools
+Requires-Dist: astropy
+Requires-Dist: numpy
+Requires-Dist: h5py
+Requires-Dist: progress
+Requires-Dist: requests
+Requires-Dist: pandas
+Provides-Extra: predict
+Requires-Dist: codex-africanus; extra == "predict"
+
 # tart2ms
 
 [![PyPI package](https://img.shields.io/badge/pip%20install-tart2ms-brightgreen)](https://pypi.org/project/tart2ms) [![version number](https://img.shields.io/pypi/v/tart2ms?color=green&label=version)](https://github.com/tart-telescope/tart2ms/releases) [![License](https://img.shields.io/github/license/tart-telescope/tart2ms)](https://github.com/tart-telescope/tart2ms/blob/master/LICENSE.txt)
 
 
 Convert data from a [TART radio telescope](https://tart.elec.ac.nz) to measurement set format. This module relies on the excellent dask-ms module as a helper to create the measurement sets. This packate requires python-casacore to be installed on your system
 
@@ -88,14 +121,21 @@
 
 ## TODO
 
 - 
 
 ## Changelog
 
+- 0.6.0b3 If WEIGHT_SPECTRUM is not present, then subsititude ones
+- 0.6.0b2 Clean up the logging code. Add a --debug flag.
+          Get rid of the annoying printing of casa tables
+- 0.6.0b1 New casa_read_ms function similar to read_ms, but uses casacore - blindingly fast.
+          made function signatures the same for both read_ms() and casa_read_ms().
+- 0.5.0b3 Remove noisy warnings. Add venv makefile.
+          Output the snapshot direction in 12-ball format to make rephasing easier.
 - 0.5.0b2 Make prediction an optional dependency to remove codex-africanus from requirements.
 - 0.5.0b1 Add model prediction
           Add automatic catalog download
 - 0.4.0b3 Use the new catalog url functions from tart_tools
 - 0.4.0b2 Add a helper function get_array_location
 - 0.4.0b1 Add a tart2ms.read_ms function (from disko)
           Add utilities for resolution calculations.
```

### Comparing `tart2ms-0.5.0b2/bin/tart2ms` & `tart2ms-0.6.0b3/bin/tart2ms`

 * *Files 8% similar despite different names*

```diff
@@ -60,16 +60,18 @@
     named_positions = util.read_known_phasings()
     specpos = list(map(lambda s: s.name, catalog_positions)) + \
               list(map(lambda s: s['name'], named_positions))
     parser.add_argument('--rephase', required=False, default=None,
                         help=f"Rephase all visibilities to a new phase center. 'obs-midpoint' rephases to the zenith at the observation "
                              f"midpoint for the provided databases. Otherwise another known position can be given or a twelve digit J2000 epoch coordinate "
                              f"(e.g. J193900-632400). Currently recognized special positions are: {','.join(specpos)}")
+    parser.add_argument('--debug', action="store_true",
+                        help="Make verbose logs and store to a log file")
     parser.add_argument('--single-field', action="store_true",
-                        help="Write out single phase center for all observations")   
+                        help="Write out single phase center for all observations")
     parser.add_argument('--telescope_name', dest="override_telescope_name", required=False, default="TART",
                         help="Override telescope name with a JPL recognized telescope name - needed for some CASA tasks")
     parser.add_argument('--uncalibrated', dest="uncalibrated", required=False, action="store_true",
                         help="Do not apply calibration solutions (store raw data)")
     parser.add_argument("--add-model", dest="addmodel", required=False, action="store_true",
                         help="DFT a model of the GNSS sources into MODEL_DATA if sources are available in the input database")
     parser.add_argument("--write-model-catalog", dest="writemodelcatalog", required=False, action="store_true",
@@ -82,32 +84,50 @@
                         help="Ignores GNSS sources already cached from a previous run")
     parser.add_argument('--timerange-start-utc', dest="timerange_start_utc", required=False, default=None,
                         help="Include only timestamps after this UTC time, e.g. 2022-03-23T21:08:12")
     parser.add_argument('--timerange-end-utc', dest="timerange_end_utc", required=False, default=None,
                         help="Include only timestamps before this UTC time, e.g. 2022-03-23T23:30:12")
     parser.add_argument('--chunks-out', dest="chunks", required=False, default=10000,
                         help="Chunk sizes to use for MAIN table writeout")
+    parser.add_argument('--override-ant-pos', required=False, default=None, dest='override_ant_pos',
+                        help="Overrides antenna positions with external json file, keyed on antenna_positions with list of ENU tripples. "
+                             "Normally will use the antenna positions stored in the provided h5 or json files.")
     
     ARGS = parser.parse_args()
     def __parsedateISO8601(x):
         return dt(*time.strptime(x, "%Y-%m-%dT%H:%M:%S")[:6])
     ARGS.timerange_start_utc = __parsedateISO8601(ARGS.timerange_start_utc) if ARGS.timerange_start_utc is not None else None
     ARGS.timerange_end_utc = __parsedateISO8601(ARGS.timerange_end_utc) if ARGS.timerange_end_utc is not None else None
-    logger = logging.getLogger("tart2ms")
-    logger.setLevel(logging.INFO)
-    ch = logging.StreamHandler()
-    ch.setLevel(logging.INFO)
-    formatter = logging.Formatter(
-        '%(asctime)s - %(name)s - %(levelname)s - %(message)s')
-    ch.setFormatter(formatter)
-    logger.addHandler(ch)
-    fileHandler = logging.FileHandler(filename=f"tart2ms.{dt.now().timestamp()}.log")
-    fileHandler.setFormatter(formatter)
-    fileHandler.setLevel(level=logging.INFO)
-    logger.addHandler(fileHandler)
+
+    if ARGS.debug:
+        level = logging.DEBUG
+    else:
+        level = logging.ERROR
+
+    logger = logging.getLogger('tart2ms')
+    logger.setLevel(level)
+
+    if ARGS.debug:
+        fh = logging.FileHandler(filename=f"tart2ms.{dt.now().timestamp()}.log")
+        fh.setLevel(level)
+
+        # create console handler and set level to debug
+        ch = logging.StreamHandler()
+        ch.setLevel(level)
+
+        # create formatter
+        formatter = logging.Formatter('%(asctime)s - %(name)s - %(levelname)s - %(message)s')
+
+        # add formatter to ch
+        ch.setFormatter(formatter)
+        fh.setFormatter(formatter)
+
+        # add ch to logger
+        logger.addHandler(ch)
+        logger.addHandler(fh)
 
     logger.info("TART2MS parameters:")
     for k in vars(ARGS).keys():
         val = getattr(ARGS, k, "Information Unavailable")
         reprk = str(k).ljust(20, " ")
         logger.info(f"\t{reprk}: {val}")
 
@@ -162,15 +182,16 @@
                      fill_model=ARGS.addmodel,
                      writemodelcatalog=ARGS.writemodelcatalog,
                      fetch_sources=not ARGS.no_fetch_sources,
                      catalog_recache=ARGS.sources_recache,
                      write_extragalactic_catalogs=not ARGS.no_celestial_sources,
                      filter_end_utc=ARGS.timerange_end_utc,
                      filter_start_utc=ARGS.timerange_start_utc,
-                     chunks_out=ARGS.chunks)
+                     chunks_out=ARGS.chunks,
+                     override_ant_pos=ARGS.override_ant_pos)
 
     elif ARGS.hdf:
         logger.info("Getting Data from file: {}".format(ARGS.hdf))
         # Load data from a HDF5 file
         logger.info("Writing measurement set '{}'...".format(ARGS.ms))
         ms_from_hdf5(ARGS.ms, ARGS.hdf, ARGS.pol2,
                      phase_center_policy, ARGS.override_telescope_name,
@@ -178,15 +199,16 @@
                      fill_model=ARGS.addmodel,
                      writemodelcatalog=ARGS.writemodelcatalog,
                      fetch_sources=not ARGS.no_fetch_sources,
                      catalog_recache=ARGS.sources_recache,
                      write_extragalactic_catalogs=not ARGS.no_celestial_sources,
                      filter_end_utc=ARGS.timerange_end_utc,
                      filter_start_utc=ARGS.timerange_start_utc,
-                     chunks_out=ARGS.chunks)
+                     chunks_out=ARGS.chunks,
+                     override_ant_pos=ARGS.override_ant_pos)
 
     else:
         logger.info("Getting Data from API: {}".format(ARGS.api))
         api = api_handler.APIhandler(ARGS.api)
         info = api.get('info')
         ant_pos = api.get('imaging/antenna_positions')
         config = settings.from_api_json(info['info'], ant_pos)
@@ -212,8 +234,9 @@
                      ARGS.override_telescope_name, json_data=json_data,
                      applycal=not ARGS.uncalibrated,
                      fill_model=ARGS.addmodel,
                      writemodelcatalog=ARGS.writemodelcatalog,
                      write_extragalactic_catalogs=not ARGS.no_celestial_sources,
                      filter_end_utc=ARGS.timerange_end_utc,
                      filter_start_utc=ARGS.timerange_start_utc,
-                     chunks_out=ARGS.chunks)
+                     chunks_out=ARGS.chunks,
+                     override_ant_pos=ARGS.override_ant_pos)
```

### Comparing `tart2ms-0.5.0b2/setup.py` & `tart2ms-0.6.0b3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 '''
 from setuptools import setup
 
 with open('README.md') as f:
     readme = f.read()
 
 setup(name='tart2ms',
-    version='0.5.0b2',
+    version='0.6.0b3',
     description='Convert TART observation data to Measurement Sets',
     long_description=readme,
     long_description_content_type="text/markdown",
     url='http://github.com/tmolteno/tart2ms',
     author='Tim Molteno',
     author_email='tim@elec.ac.nz',
     license='GPLv3',
```

### Comparing `tart2ms-0.5.0b2/tart2ms/catalogs/3CRR` & `tart2ms-0.6.0b3/tart2ms/catalogs/3CRR`

 * *Files identical despite different names*

### Comparing `tart2ms-0.5.0b2/tart2ms/catalogs/MeerKAT_gaincal_list` & `tart2ms-0.6.0b3/tart2ms/catalogs/MeerKAT_gaincal_list`

 * *Files identical despite different names*

### Comparing `tart2ms-0.5.0b2/tart2ms/catalogs/SUMMS` & `tart2ms-0.6.0b3/tart2ms/catalogs/SUMMS`

 * *Files identical despite different names*

### Comparing `tart2ms-0.5.0b2/tart2ms/catalogs/catalog_reader.py` & `tart2ms-0.6.0b3/tart2ms/catalogs/catalog_reader.py`

 * *Files identical despite different names*

### Comparing `tart2ms-0.5.0b2/tart2ms/fixvis.py` & `tart2ms-0.6.0b3/tart2ms/fixvis.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,15 @@
 from pyrap.quanta import quantity
 from pyrap import quanta
 
 import logging
 from progress.bar import FillingSquaresBar as bar
 import sys
 
-logger = logging.getLogger("tart2ms")
-logger.setLevel(logging.INFO)
+logger = logging.getLogger(__name__)
 
 
 class progress():
     def __init__(self, *args, **kwargs):
         """ Wraps a progress bar to check for TTY attachment
             otherwise does prints basic progress periodically
         """
```

### Comparing `tart2ms-0.5.0b2/tart2ms/ms_helper.py` & `tart2ms-0.6.0b3/tart2ms/ms_helper.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,23 +14,22 @@
 from astropy import units as u
 from casacore.tables import table
 from astropy.constants import c
 
 from tart2ms.catalogs.catalog_reader import catalog_factory
 from tart2ms.fixvis import progress
 
-logger = logging.getLogger("tart2ms")
-logger.setLevel(logging.INFO)
+logger = logging.getLogger(__name__)
 
 AFRICANUS_DFT_AVAIL = True
 try:
     from africanus.rime.dask import wsclean_predict
     from africanus.coordinates.dask import radec_to_lm
 except ImportError:
-    logger.warning("Cannot import Africanus API. MODEL_DATA filling capabilities disabled")
+    #logger.warning("Cannot import Africanus API. MODEL_DATA filling capabilities disabled")
     AFRICANUS_DFT_AVAIL = False
 
 def azel2radec(az, el, location, obstime, distance=None):
     """ az, el -- in degrees
         distance -- needed to convert solar system bodies back to J2000 in the barycentric frame
         location -- observer location on the ground 
         time -- astropy time for the observation
```

### Comparing `tart2ms-0.5.0b2/tart2ms/named_phasings.json` & `tart2ms-0.6.0b3/tart2ms/named_phasings.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9285714285714286%*

 * *Differences: {'delete': '[4]'}*

```diff
@@ -32,20 +32,14 @@
             "DEC": "-37d12m30s",
             "EQUINOX": "J2000",
             "FRAME": "fk5",
             "RA": "03h22m41.7s"
         }
     },
     {
-        "name": "Mars",
-        "position": {
-            "FRAME": "Special Body"
-        }
-    },
-    {
         "name": "Sun",
         "position": {
             "FRAME": "Special Body"
         }
     },
     {
         "name": "Moon",
```

### Comparing `tart2ms-0.5.0b2/tart2ms/read_ms.py` & `tart2ms-0.6.0b3/tart2ms/read_ms.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 '''
-    Get Read data from a measurement set.
+    Read data from a measurement set.
     Author: Tim Molteno, tim@elec.ac.nz
     Copyright (c) 2019-2022.
 
     License. GPLv3.
 '''
 
 import dask
@@ -15,117 +15,127 @@
 import numpy as np
 
 from daskms import xds_from_table, xds_from_ms
 
 
 from .util import resolution_min_baseline, rayleigh_criterion
 
-logger = logging.getLogger("tart2ms")
-# logger.addHandler(
-#     logging.NullHandler()
-# )  # Add other handlers if you're using this as a library
-logger.setLevel(logging.INFO)
+logger = logging.getLogger(__name__)
 
 
 class RadioObservation(object):
     def __init__(self):
         pass
 
+def dt(_t0):
+    return f"  \t\t\tElapsed {time.perf_counter() - _t0 :04f} s"
 
-def read_ms(ms, num_vis, angular_resolution, chunks=1000, channel=0,
-            field_id=0, ddid=0):
+def read_ms(ms, num_vis, angular_resolution, channel=0, field_id=0, ddid=0, snapshot=0, pol=0):
     """
     Use dask-ms to load the necessary data to create a telescope operator
     (will use uvw positions, and antenna positions)
 
     -- angular_resolution: Angular resolution (degrees) Used to calculate the maximum UVW baselines to include.
     """
 
     # local_cluster = distributed.LocalCluster(processes=False)
     # address = local_cluster.scheduler_address
     # logging.info("Using distributed scheduler "
     # "with address '{}'".format(address))
     # client = distributed.Client()
     if not os.path.exists(ms):
         raise RuntimeError(f"Measurement set {ms} not found")
-
+    chunks=10000
     try:
-        # Create a dataset representing the entire antenna table
-        ant_table = "::".join((ms, "ANTENNA"))
+        _tic = time.perf_counter()
+        logger.info(f"Reading {ms}...")
 
-        for ant_ds in xds_from_table(ant_table):
-            # print(ant_ds)
-            # print(dask.compute(ant_ds.NAME.data,
-            # ant_ds.POSITION.data,
-            # ant_ds.DISH_DIAMETER.data))
-            ant_p = np.array(ant_ds.POSITION.data)
-        logger.info("Antenna Positions {}".format(ant_p.shape))
+        # Create a dataset representing the entire antenna table
+        ant_ds, tabkw, colkw = xds_from_table(f"{ms}::ANTENNA",
+                                              table_keywords=True,
+                                              column_keywords=True)
+        logger.info(f"Table Keywords: {tabkw}")
+        logger.info(f"Column Keywords: {colkw}")
+
+        ant_p = np.array(ant_ds[0].POSITION.data)
+        # dt = 7.116458
+        logger.info(f"Antenna Positions {ant_p.shape},  {dt(_tic)}")
 
         # Create a dataset representing the field
-        field_table = "::".join((ms, "FIELD"))
-        for field_ds in xds_from_table(field_table):
+        for field_ds in xds_from_table(f"{ms}::FIELD"):
             if field_id >= field_ds.sizes['row'] or field_id < 0:
                 raise RuntimeError(f"Selected field {field_id} is not a valid field identifier. "
                                    f"Must be in [0, {field_ds.sizes['row']-1}]")
             phase_dir = np.array(field_ds.PHASE_DIR.data)[field_id].flatten()
             name = field_ds.NAME.data.compute()[field_id]
             logger.info("Field {} (index {}): Phase Dir {}".format(name,
                                                                    field_id,
                                                                    np.degrees(phase_dir)))
 
         # Create datasets representing each row of the spw table
         # we need a map to select SPW based on DDID first
         # MAIN.DDID (FK) -> DATA_DESCRIPTOR.SPECTRAL_WINDOW_ID (FK) -> SPECTRAL_WINDOW.CHAN_FREQ
+        logger.info(f"Getting Data Desciptions..,  {dt(_tic)}")
         ddid_table = "::".join((ms, "DATA_DESCRIPTION"))
         for ddid_ds in xds_from_table(ddid_table, group_cols="__row__"):
             spw_ids = ddid_ds.SPECTRAL_WINDOW_ID.data.compute()
             if ddid < 0 or ddid >= ddid_ds.sizes['row']:
                 raise RuntimeError(f"Selected DDID {ddid} is not a valid DDID identifier. "
                                    f"Must be in [0, {ddid_ds.sizes['row']-1}]")
             logger.info(f"Selecting Data Descriptor ID {int(ddid)} per user request")
             logger.info(f"DDID {int(ddid)} selects IF / SPW ID {int(spw_ids[ddid])}")
             # may be needed if we use mixed receivers in the future??
             # although I suspect GNSS receivers are all just circular
             pol_ids = ddid_ds.POLARIZATION_ID.data.compute()
 
+        logger.info(f"Getting Spectral Window..,  {dt(_tic)}")
         spw_table = "::".join((ms, "SPECTRAL_WINDOW"))
         for spw_ds in xds_from_table(spw_table, group_cols="__row__"):
-            logger.debug("CHAN_FREQ.shape: {}".format(spw_ds.CHAN_FREQ.values.shape))
+            logger.info("CHAN_FREQ.shape: {}".format(spw_ds.CHAN_FREQ.values.shape))
             frequencies = dask.compute(spw_ds.CHAN_FREQ.values)[int(spw_ids[ddid])].flatten()
             frequency = frequencies[channel]
             logger.info("Selected SPW {} Frequencies = {} MHz".format(spw_ids[ddid],
                                                                       ",".join(map(lambda nu: f"{nu:.3f}",
                                                                                frequencies * 1e-6))))
             logger.info("Selected imaging Frequency = {}".format(frequency))
             logger.debug("NUM_CHAN = %f" % np.array(spw_ds.NUM_CHAN.values)[0])
 
         # Create datasets from a partioning of the MS
+        logger.info(f"Getting datasets..,  {dt(_tic)}")
         group_cols = ["FIELD_ID", "DATA_DESC_ID"]
         datasets = list(xds_from_ms(ms, chunks={"row": chunks}, group_cols=group_cols))
         logger.debug("DataSets: N={}".format(len(datasets)))
 
         pol = 0
 
+        #
+        # Helper to read numpy arrays. This is VERY SLOW taking
+        # around 10 seconds to perform on an array of ten minutes
+        # of TART visibilities. (50000 rows)
+        #
         def read_np_array(da, title, dtype=np.float32):
             tic = time.perf_counter()
             logger.info("Reading {}...".format(title))
             ret = np.array(da, dtype=dtype)
             toc = time.perf_counter()
-            logger.info(f"Shape {ret.shape} Elapsed {toc - tic :04f} seconds")
+            logger.info(f"Shape {ret.shape} time {toc - tic :04f} s")
             return ret
+
         no_datasets_read = 0
-        for i, ds in enumerate(datasets):
+        logger.info(f"Processing datasets..,  {dt(_tic)}")
+        for ds in datasets:
             logger.debug(
                 "DATASET field_id={} shape: {}".format(ds.FIELD_ID, ds.DATA.data.shape)
             )
             logger.debug("UVW shape: {}".format(ds.UVW.data.shape))
             logger.debug("SIGMA shape: {}".format(ds.SIGMA.data.shape))
             if int(field_id) == int(ds.FIELD_ID) and \
                int(ddid) == int(ds.DATA_DESC_ID):
                 no_datasets_read += 1
+                logger.info(f"Found DATASET field_id={ds.FIELD_ID} shape: {ds.DATA.data.shape}")
                 uvw = read_np_array(ds.UVW.data, "UVW")
                 flags = read_np_array(
                     ds.FLAG.data[:, channel, pol], "FLAGS", dtype=np.int32
                 )
 
                 #
                 #
@@ -183,14 +193,17 @@
                 # ant1   = read_np_array(ds.ANTENNA1.data[indices], "ANTENNA1")
                 # ant12  = read_np_array(ds.ANTENNA1.data[indices], "ANTENNA2")
                 cv_vis = read_np_array(
                     ds.DATA.data[indices, channel, pol], "DATA", dtype=np.complex64
                 )
 
                 epoch_seconds = np.mean(np.array(ds.TIME.data))
+                break   # TODO Check this TCAM. Stop once we have our field ID.
+
+        logger.info(f"Processing complete,  {dt(_tic)}")
         if no_datasets_read == 0:
             raise RuntimeError("FIELD_ID ({}) or DDID ({}) contains no data".format(field_id, ddid))
 
         hdr = {
             "CTYPE1": ("RA---SIN", "Right ascension angle cosine"),
             "CRVAL1": np.degrees(phase_dir)[0],
             "CUNIT1": "deg     ",
```

### Comparing `tart2ms-0.5.0b2/tart2ms/tart2ms.py` & `tart2ms-0.6.0b3/tart2ms/tart2ms.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,73 +1,69 @@
 '''
     Get TART data into a measurement set.
     Author: Tim Molteno, tim@elec.ac.nz
-    Copyright (c) 2019-2022.
+    Copyright (c) 2019-2024.
 
     Official Documentation is Here.
         https://casa.nrao.edu/Memos/229.html#SECTION00044000000000000000
 
     License. GPLv3.
 '''
-from datetime import datetime as dt
-import logging
-import json
-import h5py
-import dask
-from dask.diagnostics import ProgressBar
-#dask.config.set(scheduler='threads')  # overwrite default with threaded scheduler
-dask.config.set(scheduler='processes')  # overwrite default with threaded scheduler
-#dask.config.set(scheduler='synchronous')  # overwrite default with threaded scheduler
-import dateutil
 
-import dask.array as da
-import numpy as np
-import time
-import os
-import re
-from hashlib import sha256
+from .catalogs import catalog_reader
+from .fixvis import (fixms,
+                     synthesize_uvw,
+                     dense2sparse_uvw,
+                     progress,
+                     rephase)
+from .util import (rayleigh_criterion,
+                   read_known_phasings)
+from .ms_helper import (azel2radec,
+                        predict_model,
+                        get_catalog_sources_azel,
+                        get_solar_system_bodies)
 
+from hashlib import sha256
 from itertools import product
-
 from casacore.quanta import quantity
-
-from astropy import coordinates as ac
-
 from daskms import Dataset, xds_to_table, xds_from_ms
 
-import astropy.units as u
+from astropy import coordinates as ac
 from astropy.time import Time
 from astropy.coordinates import SkyCoord, EarthLocation, Angle
-from astropy.constants import R_earth, c as lightspeed
-
+from astropy.constants import R_earth
 
 from tart.operation import settings
 from tart.imaging.visibility import Visibility
-from tart.imaging import (calibration,
-                          elaz)
-from .catalogs import catalog_reader
+from tart.imaging import calibration
 
 from tart_tools import (api_imaging,
                         api_handler)
 
-from .fixvis import (fixms,
-                     synthesize_uvw,
-                     dense2sparse_uvw,
-                     progress,
-                     rephase)
+import logging
+import json
+import h5py
+import dask
+import dateutil
+import time
+import os
+import re
 
-from .util import (rayleigh_criterion,
-                   read_known_phasings)
-from .ms_helper import (azel2radec,
-                        predict_model,
-                        get_catalog_sources_azel,
-                        get_solar_system_bodies)
+import dask.array as da
+import numpy as np
+import astropy.units as u
 
-LOGGER = logging.getLogger("tart2ms")
-LOGGER.setLevel(logging.INFO)
+from datetime import datetime as dt
+from dask.diagnostics import ProgressBar
+# dask.config.set(scheduler='threads')  # overwrite default with threaded scheduler
+dask.config.set(scheduler='processes')  # overwrite default with threaded scheduler
+# dask.config.set(scheduler='synchronous')  # overwrite default with threaded scheduler
+
+
+LOGGER = logging.getLogger(__name__)
 
 '''
 The following from Oleg Smirnov.
 
 >
 > * We have a single circular polarization that I've labelled 1
 > (from FITS scheme I googled somewhere. Could use RR I guess).
@@ -133,23 +129,24 @@
 
 
 class MSTable:
     '''
         Little Helper to simplify writing a table.
     '''
     __write_futures = []
+
     def __init__(self, ms_name, table_name):
         self.table_name = "::".join((ms_name, table_name))
         self.datasets = []
 
     def append(self, dataset):
         self.datasets.append(dataset)
 
     def write(self):
-        """ Creates a future to be computed 
+        """ Creates a future to be computed
             ensure to call dask.compute with get_futures
             to finalize graph construction
         """
         writes = xds_to_table(self.datasets, self.table_name, columns="ALL")
         self.__write_futures.append(writes)
 
     @classmethod
@@ -186,15 +183,16 @@
               phase_center_policy,
               override_telescope_name,
               uvw_generator='casacore',
               fill_model=True,
               writemodelcatalog=True,
               sources_timestamps=None,
               write_extragalactic_catalogs=True,
-              chunks_out=10000):
+              chunks_out=10000,
+              skip_sources_keywordtbl=False):
     ''' Create a Measurement Set from some TART observations
 
     Parameters
     ----------
 
     ms_table_name : string
         The name of the MS top level directory. I think this only workds in
@@ -225,14 +223,17 @@
     '''
     start_time = time.time()
     try:
         loc = info['location']
     except Exception:
         loc = info
 
+    print(f"Creating Measurement Set: frames={len(timestamps)}")
+    print(f"Fields: 0..{len(timestamps)-1}")
+
     lat, lon, height = loc["lat"], loc["lon"], loc["alt"]
     LOGGER.info("Telescope position (WGS84):")
     LOGGER.info(f"\tLat {lat}")
     LOGGER.info(f"\tLon {lon}")
     LOGGER.info(f"\tAlt {height}")
     # by default SOURCES (usually GNSS) come from the same json database
     # but we could forseeably load them in (or augment) separately in the future
@@ -372,35 +373,35 @@
         sc_dir_repr = f"J{sc_dir.ra.hms[0]:02.0f}{sc_dir.ra.hms[1]:02.0f}{sc_dir.ra.hms[2]:02.0f}"\
                       f"{sign}"\
                       f"{abs(sc_dir.dec.dms[0]):02.0f}{abs(sc_dir.dec.dms[1]):02.0f}{abs(sc_dir.dec.dms[2]):02.0f}"
         return sc_dir_repr
 
     directions = direction.T
     for d in directions:
-        LOGGER.info(f"    shapshot direction {d[0]}, {d[1]} {SkyCoord(d[0]*u.rad, d[1]*u.rad, frame='icrs').to_string('dms')}")
+        LOGGER.info(f"    shapshot direction {d[0]}, {d[1]} {__twelveball(d.flatten())}")
 
     use_special_fn = None
     if phase_center_policy == "instantaneous-zenith":
         pass
     elif isinstance(phase_center_policy, SkyCoord):
-        direction = np.deg2rad(np.array([[phase_center_policy.icrs.ra.value, 
+        direction = np.deg2rad(np.array([[phase_center_policy.icrs.ra.value,
                                           phase_center_policy.icrs.dec.value]]).reshape(1, 2, 1))
     elif (phase_center_policy == "no-rephase-obs-midpoint") or \
          (phase_center_policy == "rephase-obs-midpoint"):
         direction = direction[:, :, direction.shape[2]//2].reshape(1, 2, 1)  # observation midpoint
     elif phase_center_policy.find("rephase-") == 0:
-        fn = phase_center_policy.replace("rephase-","")
+        fn = phase_center_policy.replace("rephase-", "")
         use_special_fn = fn
         # 3CRR currently only catalog with special names
         catalog_positions = catalog_reader.catalog_factory.from_3CRR(fluxlim15=0.0)
         named_positions = read_known_phasings()
         fsrc = list(filter(lambda x: x.name == fn, catalog_positions))
         if len(fsrc) > 0:
             direction = np.array([[fsrc[0].rarad, fsrc[0].decrad]]).reshape(1, 2, 1)
-        else: # otherwise it is in the named positions list
+        else:  # otherwise it is in the named positions list
             fsrc = list(filter(lambda x: x['name'].upper() == fn, named_positions))
             if len(fsrc) == 0:
                 raise RuntimeError(f"Unknown named source {fn}")
             if fsrc[0]['position']['FRAME'] == "Special Body":
                 body = ac.get_body(fn, obstime[0], location=location)
                 LOGGER.critical(f"User caution: enabling non-sidereal tracking of '{fn}'. Indicated field centre will be "
                                 f"that of the first timestamp in your synthesized map, but W-coordinate will be actively "
@@ -446,29 +447,30 @@
         'TELESCOPE_NAME': (("row",), da.asarray(np.asarray([override_telescope_name], dtype=object), chunks=1)),
         'OBSERVER': (("row",), da.asarray(np.asarray(['Tim'], dtype=object), chunks=1)),
         "TIME_RANGE": (("row", "obs-exts"), da.asarray(np.array([[epoch_s[0], epoch_s[-1]]]), chunks=1))
     })
     obs_table.append(dataset)
 
     # ----------------------------- SOURCE datasets -------------------------- #
-    if sources:
+    if sources and not skip_sources_keywordtbl:
         all_numlines = []
         all_name = []
         all_time = []
         all_direction = []
         if len(epoch_s_sources) != len(sources):
             raise RuntimeError(
                 "If sources are specified then we expected epochs to be of same size as sources list")
         for database_i, (epoch_s_i, sources_i) in enumerate(zip(epoch_s_sources, sources)):
-            if sources_i is None: continue
+            if sources_i is None:
+                continue
             for src in sources_i:
                 name = src['name']
                 # Convert to J2000
                 direction_src = azel2radec(az=src['az'],
-                                           el=src['el'], 
+                                           el=src['el'],
                                            location=location,
                                            obstime=sources_obstime[database_i])
                 LOGGER.debug(
                     f"SOURCE: {name}, timestamp: {timestamps}, dir: {direction_src}")
                 # , 1, dtype=np.int32)
                 dask_num_lines = da.asarray(np.asarray([1], dtype=np.int32))
                 dask_direction = da.asarray(np.asarray(
@@ -598,20 +600,20 @@
         LOGGER.debug(f"Data size {row} {chan} {corr}")
         LOGGER.info(
             f"Data column size {row * chan * corr * 8 / 1024.0**2:.2f} MiB")
 
         np_data = np.zeros((row, chan, corr), dtype=np.complex128)
         for i in range(corr):
             np_data[:, :, i] = vis_array.reshape((row, chan))
-        
+
         data_chunks = tuple((chunks['row'], chan, corr))
         dask_data = da.from_array(np_data, chunks=data_chunks)
         flag_categories = da.from_array(0.05*np.ones((row, 1, chan, corr)), chunks=(chunks['row'], 1, chan, corr))
         flag_data = np.zeros((row, chan, corr), dtype=np.bool_)
-        
+
         # Create dask ddid column
         dask_ddid = da.full(row, ddid, chunks=chunks['row'], dtype=np.int32)
         if np_data.shape[0] % len(epoch_s) != 0:
             raise RuntimeError(
                 "Expected nrow to be integral multiple of number of time slots")
         if np_data.shape[0] != len(epoch_s) * nbl:
             raise RuntimeError(
@@ -645,42 +647,41 @@
               'rephase-' in phase_center_policy):
             # user is just going to get a single zenith position at the observation centoid
             scan = np.ones(len(epoch_s), dtype=int).repeat(
                 nbl)  # start at 1, per convention
             field_no = np.zeros_like(scan)
         else:
             raise ValueError(f"phase_center_policy must be one of "
-                         f"['instantaneous-zenith','rephase-obs-midpoint','no-rephase-obs-midpoint',"
-                         f"'rephase-<named position>' or Astropy.SkyCoord] got {phase_center_policy}")
-        
+                             f"['instantaneous-zenith','rephase-obs-midpoint','no-rephase-obs-midpoint',"
+                             f"'rephase-<named position>' or Astropy.SkyCoord] got {phase_center_policy}")
 
         # apply rephasor if needed
         mean_sidereal_day = 23 + 56 / 60. + 4.0905 / 3600.  # hrs
         # degrees per second at equator
         sidereal_rate = 360. / (mean_sidereal_day * 3600)
         # if we move more than say 5% of the instrument resolution during the observation
         # then warnings must be raised if we're snapping the field centre without phasing
         obs_length = np.max(epoch_s) - np.min(epoch_s)
         snapshot_length_cutoff = rayleigh_crit / sidereal_rate * 0.05
-        
+
         if np.array(timestamps).size > 1 and uvw_generator != 'casacore':
             LOGGER.warning(f"You should not use '{uvw_generator}' mode to generate UVW coordinates"
                            f"for multi-timestamp databases. Your UVW coordinates will be wrong")
         assert direction.ndim == 3
         assert direction.shape[0] == 1
         assert direction.shape[1] == 2
         zenith_directions = np.array(
             [[phase_j2000.ra.radian, phase_j2000.dec.radian]])
         zenith_directions = zenith_directions.reshape(zenith_directions.shape[1],
                                                       zenith_directions.shape[2]).T.copy()
         map_row_to_zendir = da.from_array(np.arange(len(epoch_s), dtype=int).repeat(nbl), chunks=chunks['row'])
         if uvw_generator == 'telescope_snapshot':
             if isinstance(phase_center_policy, SkyCoord) or \
-               phase_center_policy.find('rephase-') >= 0: # rephase or non-rephase single field database
-               raise RuntimeError("Telescope snapshot UVW mode may only be used for zenethal snapshotting mode")
+                phase_center_policy.find('rephase-') >= 0:  # rephase or non-rephase single field database
+                raise RuntimeError("Telescope snapshot UVW mode may only be used for zenethal snapshotting mode")
             bl_pos = np.array(ant_pos)[baselines]
             uu_a, vv_a, ww_a = -(bl_pos[:, 1] - bl_pos[:, 0]).T
             # Use the - sign to get the same orientation as our tart projections.
             uvw_array = np.array([uu_a, vv_a, ww_a]).T
         elif uvw_generator == 'casacore':
             # need to generate UVW coordinates for zenith positions for the model prediction step
             # if enabled otherwise we can wait till the end (unless we rephase)
@@ -688,25 +689,25 @@
                phase_center_policy.find('rephase-') == 0 or \
                fill_model:
                 # we must first have accurate uvw coordinates in each different zenith direction
                 if phase_center_policy == 'rephase-obs-midpoint' or phase_center_policy == 'no-rephase-obs-midpoint':
                     centroid_direction = zenith_directions[zenith_directions.shape[0]//2, :].reshape(
                         1, 2)
                 elif isinstance(phase_center_policy, SkyCoord):
-                    centroid_direction = np.deg2rad(np.array([[phase_center_policy.icrs.ra.value, 
+                    centroid_direction = np.deg2rad(np.array([[phase_center_policy.icrs.ra.value,
                                                                phase_center_policy.icrs.dec.value]]).reshape(1, 2))
                 elif phase_center_policy.find("rephase-") == 0:
-                    fn = phase_center_policy.replace("rephase-","")
+                    fn = phase_center_policy.replace("rephase-", "")
                     # 3CRR currently only catalog with special names
                     catalog_positions = catalog_reader.catalog_factory.from_3CRR(fluxlim15=0.0)
                     named_positions = read_known_phasings()
                     fsrc = list(filter(lambda x: x.name == fn, catalog_positions))
                     if len(fsrc) > 0:
                         centroid_direction = np.array([[fsrc[0].rarad, fsrc[0].decrad]]).reshape(1, 2)
-                    else: # otherwise it is in the named positions list
+                    else:  # otherwise it is in the named positions list
                         fsrc = list(filter(lambda x: x['name'].upper() == fn, named_positions))
                         if len(fsrc) == 0:
                             raise RuntimeError(f"Unknown named source {fn}")
                         if fsrc[0]['position']['FRAME'] == "Special Body":
                             centroid_direction = np.empty((len(obstime), 2), dtype=float)
                             for ti, tt in enumerate(obstime):
                                 body = ac.get_body(fn, tt, location=location)
@@ -720,15 +721,15 @@
                             crd = SkyCoord(f"{ra} {dec}", equinox=equinox, frame=frame)
                             centroid_direction = np.deg2rad(np.array([[crd.icrs.ra.value,
                                                                        crd.icrs.dec.value]]).reshape(1, 2))
                 elif phase_center_policy == "instantaneous-zenith":
                     centroid_direction = zenith_directions
                 else:
                     raise RuntimeError("Invalid rephase option")
-                
+
                 subfields = da.unique(map_row_to_zendir).compute()
                 assert zenith_directions.shape[0] == subfields.size
                 p = progress(
                     "Computing UVW towards original zenith points", max=subfields.size)
                 uvw_array = np.zeros((vis_array.shape[0], 3), dtype=np.float64)
                 for sfi in subfields:
                     selrow = map_row_to_zendir.compute() == sfi
@@ -766,92 +767,95 @@
                             f"is short enough for sources not to move more than a fraction of the instrumental "
                             f"resolution! You are predicted to move about "
                             f"{np.ceil(obs_length / (rayleigh_crit / sidereal_rate) * 100):.0f}% "
                             f"of the instrument resolution during the course of this observation")
 
         if fill_model:
             LOGGER.info(f"Predicting GNSS positions for {len(epoch_s)} timestamps")
-            model_data = predict_model(dask_data.shape, dask_data.chunks, dask_data.dtype, 
+            model_data = predict_model(dask_data.shape, dask_data.chunks, dask_data.dtype,
                                        uvw_data,
                                        epoch_s, spw_chan_freqs, spw_i,
                                        zenith_directions,
                                        map_row_to_zendir,
                                        location,
                                        sources, epoch_s_sources, sources_obstime,
                                        writemodelcatalog)
             if model_data is None:
                 model_data = da.zeros_like(dask_data)
             cat_sources = get_catalog_sources_azel(obstime, location)
             if write_extragalactic_catalogs:
                 LOGGER.info(f"Predicting celestial catalog positions for {len(epoch_s)} timestamps")
-                celestial_model = predict_model(dask_data.shape, dask_data.chunks, dask_data.dtype, 
-                                            uvw_data,
-                                            epoch_s, spw_chan_freqs, spw_i,
-                                            zenith_directions,
-                                            map_row_to_zendir,
-                                            location,
-                                            cat_sources, epoch_s, obstime,
-                                            writemodelcatalog,
-                                            filter_elevation=20.0,
-                                            append_catalog=True)
+                celestial_model = predict_model(dask_data.shape, dask_data.chunks,
+                                                dask_data.dtype,
+                                                uvw_data,
+                                                epoch_s, spw_chan_freqs, spw_i,
+                                                zenith_directions,
+                                                map_row_to_zendir,
+                                                location,
+                                                cat_sources, epoch_s, obstime,
+                                                writemodelcatalog,
+                                                filter_elevation=20.0,
+                                                append_catalog=True)
                 if celestial_model is None:
                     celestial_model = da.zeros_like(dask_data)
                 model_data += celestial_model
             LOGGER.info(f"Predicting Sun and Moon positions for {len(epoch_s)} timestamps")
             cat_sources = get_solar_system_bodies(obstime, location)
-            solar_model = predict_model(dask_data.shape, dask_data.chunks, dask_data.dtype, 
+            solar_model = predict_model(dask_data.shape, dask_data.chunks, dask_data.dtype,
                                         uvw_data,
                                         epoch_s, spw_chan_freqs, spw_i,
                                         zenith_directions,
                                         map_row_to_zendir,
                                         location,
                                         cat_sources, epoch_s, obstime,
                                         writemodelcatalog,
                                         filter_elevation=20.0,
                                         append_catalog=True)
 
             if solar_model is None:
                 solar_model = da.zeros_like(dask_data)
             model_data += solar_model
             model_data.rechunk(dask_data.chunks)
+
         def __rephase_dask_wrapper(vis, uvw, field_ids, sel, freq, pos, refdir, phasesign=-1):
             vis = np.array(vis[0]) if isinstance(vis, list) else vis
             uvw = np.array(uvw[0]) if isinstance(uvw, list) else uvw
             field_ids = np.array(field_ids[0]) if isinstance(field_ids, list) else field_ids
             sel = np.array(sel[0]) if isinstance(sel, list) else sel
             return rephase(vis, uvw, field_ids, sel, freq, pos, refdir, phasesign=phasesign)
 
         if isinstance(phase_center_policy, SkyCoord) or \
-           phase_center_policy.find('rephase-') == 0:
-            if centroid_direction.shape[0] == 1: 
-                new_phase_dir = SkyCoord(centroid_direction[0, 0]*u.rad, centroid_direction[0, 1]*u.rad,
-                                        frame='icrs')
+            phase_center_policy.find('rephase-') == 0:
+            if centroid_direction.shape[0] == 1:
+                new_phase_dir = SkyCoord(centroid_direction[0, 0]*u.rad,
+                                         centroid_direction[0, 1]*u.rad,
+                                         frame='icrs')
                 new_phase_dir_repr = f"{new_phase_dir.ra.hms[0]:02.0f}h{new_phase_dir.ra.hms[1]:02.0f}m{new_phase_dir.ra.hms[2]:05.2f}s "\
                                     f"{new_phase_dir.dec.dms[0]:02.0f}d{abs(new_phase_dir.dec.dms[1]):02.0f}m{abs(new_phase_dir.dec.dms[2]):05.2f}s"
                 LOGGER.info(
                     f"Per user request: Rephase all data to {new_phase_dir_repr}")
                 rephased_data = da.empty_like(dask_data)
                 sel = da.ones(dask_data.shape[0], chunks=dask_data.chunks[0], dtype=bool)
                 rephased_data = \
-                    da.blockwise(__rephase_dask_wrapper, ('row','chan','corr'),
-                                 dask_data, ('row','chan','corr'),
+                    da.blockwise(__rephase_dask_wrapper, ('row', 'chan', 'corr'),
+                                 dask_data, ('row', 'chan', 'corr'),
                                  uvw_data, ('row', 'uvw'),
                                  map_row_to_zendir, ('row',),
                                  sel, ('row',),
                                  dtype=dask_data.dtype,
                                  freq=spw_chan_freqs[spw_id],
                                  pos=np.rad2deg(centroid_direction[0, :]),
                                  refdir=np.rad2deg(zenith_directions))
                 dask_data = rephased_data
                 rephased_data = da.empty_like(dask_data)
                 if fill_model:
                     sel = da.ones(model_data.shape[0], chunks=model_data.chunks[0], dtype=bool)
                     rephased_data = \
-                        da.blockwise(__rephase_dask_wrapper, ('row','chan','corr'),
-                                     model_data, ('row','chan','corr'),
+                        da.blockwise(__rephase_dask_wrapper, ('row', 'chan', 'corr'),
+                                     model_data, ('row', 'chan', 'corr'),
                                      uvw_data, ('row', 'uvw'),
                                      map_row_to_zendir, ('row',),
                                      sel, ('row',),
                                      dtype=dask_data.dtype,
                                      freq=spw_chan_freqs[spw_id],
                                      pos=np.rad2deg(centroid_direction[0, :]),
                                      refdir=np.rad2deg(zenith_directions))
@@ -859,32 +863,32 @@
             elif centroid_direction.shape[0] == len(obstime):
                 LOGGER.info(f"Per user request: Rephase data to special field {phase_center_policy.replace('rephase-','')} per timestamp")
                 rephased_data = da.zeros_like(dask_data)
                 subfields = np.unique(map_row_to_zendir)
                 for sfi in subfields.compute():
                     sel = map_row_to_zendir == sfi
                     rephased_data += \
-                        da.blockwise(__rephase_dask_wrapper, ('row','chan','corr'),
-                                     dask_data, ('row','chan','corr'),
+                        da.blockwise(__rephase_dask_wrapper, ('row', 'chan', 'corr'),
+                                     dask_data, ('row', 'chan', 'corr'),
                                      uvw_data, ('row', 'uvw'),
                                      map_row_to_zendir, ('row',),
                                      sel, ('row',),
                                      # kwargs for rephase
                                      freq=spw_chan_freqs[spw_id],
                                      pos=np.rad2deg(centroid_direction[sfi, :]),
                                      refdir=np.rad2deg(zenith_directions),
                                      dtype=dask_data.dtype)
                 dask_data = rephased_data
                 if fill_model:
                     rephased_data = da.zeros_like(dask_data)
                     for sfi in subfields.compute():
                         sel = map_row_to_zendir == sfi
                         rephased_data += \
-                            da.blockwise(__rephase_dask_wrapper, ('row','chan','corr'),
-                                         model_data, ('row','chan','corr'),
+                            da.blockwise(__rephase_dask_wrapper, ('row', 'chan', 'corr'),
+                                         model_data, ('row', 'chan', 'corr'),
                                          uvw_data, ('row', 'uvw'),
                                          map_row_to_zendir, ('row',),
                                          sel, ('row',),
                                          # kwargs for rephase
                                          freq=spw_chan_freqs[spw_id],
                                          pos=np.rad2deg(centroid_direction[sfi, :]),
                                          refdir=np.rad2deg(zenith_directions),
@@ -911,15 +915,15 @@
                                                              np.ones(selrow.size)*ddid)[selrow],
                                                          padded_uvw=padded_uvw["UVW"],
                                                          ack=False)
                     p.next()
                 uvw_data = da.from_array(np_uvw, chunks=(chunks['row'], 3))
                 LOGGER.info("<Done>")
             else:
-                raise RuntimeError("Rephaseing centroids must be 1 or a centre per original zenith position") 
+                raise RuntimeError("Rephaseing centroids must be 1 or a centre per original zenith position")
         else:
             LOGGER.info("No rephasing requested - field centers left as is")
 
         main_table = {
             'DATA': (dims, dask_data),
             'FLAG': (dims, da.from_array(flag_data, chunks=(chunks['row'], chan, corr))),
             'TIME': (("row",), da.from_array(timems, chunks=chunks['row'])),
@@ -1053,32 +1057,66 @@
         else:
             LOGGER.critical(f"Failed to retrieve GNSS TLS from '{cat_url}'. "
                             f"Source information will be unavailable and prediction will not return a useful model")
             return None, downsampletimes
     LOGGER.info(f"GNSS source catalogs retrieved for {len(downsampletimes)} timestamps, {ncache_objs} from local cache")
     return sources, downsampletimes
 
+def __load_ext_ant_pos(fn, ack=True):
+    """ Loads external antenna local ENU positions from json format 
+        The database must be keyed on 'antenna_positions' and have the following format
+        {
+            "antenna_positions": [
+                [E, 
+                 N, 
+                 U],
+                 ...
+            ]
+        }
+    """
+    if not os.path.exists(fn) and not os.path.isfile(fn):
+        raise RuntimeError(f"External antenna position file '{fn}' is not a valid file or does not exist")
+    with open(fn) as ffn:
+        ant_pos_dict = json.loads(ffn.read())
+        if "antenna_positions" not in ant_pos_dict.keys():
+            raise RuntimeError("Expected a dictionary keyed on 'antenna_positions'. Key does not exist")
+        ant_pos = ant_pos_dict['antenna_positions']
+        if not isinstance(ant_pos, list):
+            raise RuntimeError("Expected a list of ENU coordinates in external antenna positions file")
+        if not all(map(lambda x: isinstance(x, list) and len(x) == 3 and all(map(lambda xn: isinstance(xn, float), x)),
+                       ant_pos)):
+            raise RuntimeError("Expected a list of tripplets for antenna ENU positions")
+        ant_pos = np.array(ant_pos)
+        assert ant_pos.ndim == 2 and ant_pos.shape[1] == 3
+    if ack:
+        LOGGER.warning(f"Per user request will override antenna positions from externally provided database {fn}")
+    return ant_pos
+
 def ms_from_hdf5(ms_name, h5file, pol2, phase_center_policy, override_telescope_name, uvw_generator="casacore",
                  applycal=True, fill_model=False, writemodelcatalog=True, fetch_sources=True, catalog_recache=False,
-                 write_extragalactic_catalogs=True, filter_start_utc=None, filter_end_utc=None, chunks_out=10000):
+                 write_extragalactic_catalogs=True, filter_start_utc=None, filter_end_utc=None, chunks_out=10000,
+                 override_ant_pos=None):
     if pol2:
         pol_feeds = ['RR', 'LL']
     else:
         pol_feeds = ['RR']
     if isinstance(h5file, str):
         h5file = [h5file]
     all_times = []
     all_vis = []
     all_baselines = []
     ant_pos_orig = None
     orig_dico_info = None
     LOGGER.info("Will process HDF5 file: ")
     for h5 in h5file:
         LOGGER.info(f"\t '{h5}'")
-
+    if override_ant_pos:
+        ext_ant_pos = __load_ext_ant_pos(override_ant_pos)
+    else:
+        ext_ant_pos = None
     p = progress("Processing HDF database", max=len(h5file))
     all_sources = []
     all_sources_timestamps = []
     tscount = 0
     for ih5, h5 in enumerate(h5file):
         with h5py.File(h5, "r") as h5f:
             config_string = np.string_(h5f['config'][0]).decode('UTF-8')
@@ -1093,18 +1131,21 @@
                 __print_infodict_keys(config_json,
                                       ["L0_frequency", "bandwidth", "baseband_frequency",
                                        "operating_frequency", "name", "num_antenna",
                                        "sampling_frequency"])
             config = settings.from_json(config_string)
             hdf_baselines = h5f['baselines'][:]
             hdf_phase_elaz = h5f['phase_elaz'][:]
+            if ext_ant_pos is None:
+                ant_pos = h5f['antenna_positions'][:]
+                if ant_pos_orig is None:
+                    ant_pos_orig = ant_pos.copy()
+            else:
+                ant_pos = ant_pos_orig = ext_ant_pos
 
-            ant_pos = h5f['antenna_positions'][:]
-            if ant_pos_orig is None:
-                ant_pos_orig = ant_pos.copy()
             if not np.isclose(ant_pos_orig, ant_pos, atol=1.0e-1, rtol=1.0).all():
                 raise RuntimeError("The databases you are trying to concatenate have different antenna layouts. "
                                    "This is not yet supported. You could try running CASA virtualconcat to "
                                    "concatenate such heterogeneous databases")
             if orig_dico_info is None:
                 orig_dico_info = config_json
             config_same = True
@@ -1174,15 +1215,15 @@
                 online_sources, online_sources_timestamps = __fetch_sources(timestamps=timestamps, 
                                                  observer_lat=lat,
                                                  observer_lon=lon,
                                                  force_recache=catalog_recache) 
                 all_sources += online_sources if online_sources is not None else [None] * len(online_sources_timestamps)
                 all_sources_timestamps += online_sources_timestamps
         p.next()
-    LOGGER.info("<Done>")
+    print("<Done>")
     if tscount == 0:
         raise RuntimeError("Time filtering criteria resulted in an empty database. Goodbye!")
 
     # finally create concat ms
     all_vis = np.array(all_vis).flatten()
     all_baselines = np.array(all_baselines)
     ms_create(ms_table_name=ms_name,
@@ -1202,15 +1243,16 @@
               write_extragalactic_catalogs=write_extragalactic_catalogs,
               chunks_out=chunks_out)
 
 
 def ms_from_json(ms_name, json_filename, pol2, phase_center_policy, override_telescope_name,
                  uvw_generator="casacore", json_data=None, applycal=True, fill_model=False,
                  writemodelcatalog=True, fetch_sources=True, catalog_recache=False,
-                 write_extragalactic_catalogs=True, filter_start_utc=None, filter_end_utc=None, chunks_out=10000):
+                 write_extragalactic_catalogs=True, filter_start_utc=None, filter_end_utc=None, chunks_out=10000,
+                 override_ant_pos=None):
     # Load data from a JSON file
     if json_filename is not None and json_data is None:
         if isinstance(json_filename, str):
             json_filename = [json_filename]
         json_data = []
         LOGGER.info("Will process JSON file: ")
         for jfi in json_filename:
@@ -1219,15 +1261,19 @@
                 json_data.append(json.load(json_file))
     elif json_filename is None and json_data is not None:
         if not isinstance(json_data, list):
             json_data = [json_data]
     else:
         raise ValueError(
             "Either json_filename or json_data arguments should be given")
-
+    if override_ant_pos:
+        ext_ant_pos = __load_ext_ant_pos(override_ant_pos)
+    else:
+        ext_ant_pos = None
+        
     all_times = []
     all_vis = []
     all_sources = []
     all_sources_timestamps = []
     all_baselines = []
     ant_pos_orig = None
     orig_dico_info = None
@@ -1238,16 +1284,20 @@
         ant_pos = jdi['ant_pos']
         config = settings.from_api_json(info['info'], ant_pos)
         gains = np.array(jdi['gains']['gain'])
         phases = np.array(jdi['gains']['phase_offset'])
         if not applycal:
             gains[...] = 1.0
             phases[...] = 0.0
-        if ant_pos_orig is None:
-            ant_pos_orig = ant_pos.copy()
+        if ext_ant_pos is None:
+            if ant_pos_orig is None:
+                ant_pos_orig = ant_pos.copy()
+        else:
+            ant_pos = ant_pos_orig = ext_ant_pos
+        
         if not np.isclose(ant_pos_orig, ant_pos, atol=1.0e-1, rtol=1.0).all():
             raise RuntimeError("The databases you are trying to concatenate have different antenna layouts. "
                                "This is not yet supported. You could try running CASA virtualconcat to "
                                "concatenate such heterogeneous databases")
         if orig_dico_info is None:
             orig_dico_info = info["info"]
```

### Comparing `tart2ms-0.5.0b2/tart2ms/util.py` & `tart2ms-0.6.0b3/tart2ms/util.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,35 +10,45 @@
 
 import numpy as np
 import os
 import json
 import re
 from astropy import constants
 from astropy.coordinates import SkyCoord
-from astropy import units as u
+# from astropy import units as u
 
-LOGGER = logging.getLogger("tart2ms")
-LOGGER.setLevel(logging.INFO)
+LOGGER = logging.getLogger(__name__)
+
+
+def get_wavelength(frequency):
+    return constants.c.value / frequency
+
+
+def get_wavelengths(distance, frequency):
+    '''
+        Used to convert from meters to uvw coordinates
+    '''
+    return distance * frequency / constants.c.value
 
 
 def rayleigh_criterion(max_freq, baseline_lengths):
     '''
         The accepted criterion for determining the diffraction limit to resolution
         developed by Lord Rayleigh in the 19th century.
 
         approx resolution given by first order Bessel functions
         assuming array is a flat disk of length max_baseline
     '''
     min_wl = constants.c.value / max_freq
     max_baseline = np.max(baseline_lengths)
     min_baseline = np.min(baseline_lengths)
 
-    LOGGER.info("Baseline lengths:")
-    LOGGER.info(f"\tMinimum: {min_baseline:.4f} m")
-    LOGGER.info(
+    LOGGER.debug("Baseline lengths:")
+    LOGGER.debug(f"\tMinimum: {min_baseline:.4f} m")
+    LOGGER.debug(
         f"\tMaximum: {max_baseline:.4f} m --- {max_baseline/min_wl:.4f} wavelengths")
     return np.degrees(1.220 * min_wl / max_baseline)
 
 
 def resolution_min_baseline(max_freq, resolution_deg):
     '''
         Return the minimum baseline to achieve an angular resolution
@@ -48,54 +58,56 @@
         max_baseline = 1.220 * min_wl / res_rad
     '''
     min_wl = constants.c.value / max_freq
     res_rad = np.radians(resolution_deg)
 
     return 1.220 * min_wl / res_rad
 
-def read_known_phasings(fn=os.path.join(os.path.split(os.path.abspath(__file__))[0], 
+
+def read_known_phasings(fn=os.path.join(os.path.split(os.path.abspath(__file__))[0],
                                         "named_phasings.json")):
     def __try_construct_skycoord(x):
         try:
             SkyCoord(f"{x['RA']} {x['DEC']}", equinox=x["EQUINOX"], frame=x["FRAME"])
         except:
             return False
         return True
 
-    with open(fn, 'r') as f: 
+    with open(fn, 'r') as f:
         vals = json.load(f)
     if not isinstance(vals, list):
         raise RuntimeError("named_phasings.json should contain only a list of dictionaries")
     if not all(map(lambda x: hasattr(x, 'keys'), vals)):
         raise RuntimeError("named_phasings.json should contain only a list of dictionaries")
     for req_key in ['name', 'position']:
         if not all(map(lambda x: req_key in x.keys(), vals)):
             raise RuntimeError(f"named_phasings should contain attribute '{req_key}'")
     if not all(map(lambda x: "FRAME" in x['position'], vals)):
-        raise RuntimeError(f"named_phasings should contain attribute 'FRAME'")
+        raise RuntimeError("named_phasings should contain attribute 'FRAME'")
     for req_key in ["RA", "DEC", "EQUINOX"]:
-        if not all(map(lambda x: req_key in x['position'], 
+        if not all(map(lambda x: req_key in x['position'],
                    filter(lambda x: x['position']["FRAME"] != "Special Body", vals))):
             raise RuntimeError(f"Non special body named_phasings position should contain attribute {req_key}")
     if not all(map(lambda x: __try_construct_skycoord(x['position']),
                    filter(lambda x: x['position']["FRAME"] != "Special Body", vals))):
-        raise RuntimeError(f"One or more positions in the named_phasings.json is not convertable to astropy SkyCoord")
+        raise RuntimeError("One or more positions in the named_phasings.json is not convertable to astropy SkyCoord")
     return vals
 
+
 def read_coordinate_twelveball(coordstring):
     """
         Reads a standard twelve digit coordinate of the form JRARARA+/-DECDEC
         Acccepts J as J2000 or B as B1950 equinox
         yields ICRS Astropy SkyCoord if valid coord string is specified
         otherwise None
     """
-    m = re.match(r'^(?P<equinox>J|B)(?P<ra>[0-9]{6})(?P<sign>[+-]{1})(?P<dec>[0-9]{6})$', 
+    m = re.match(r'^(?P<equinox>J|B)(?P<ra>[0-9]{6})(?P<sign>[+-]{1})(?P<dec>[0-9]{6})$',
                  coordstring)
     if m is None:
-        return None # no match
+        return None  # no match
     rah = m['ra'][0:2]
     ram = m['ra'][2:4]
     ras = m['ra'][4:6]
     sign = m['sign']
     decd = m['dec'][0:2]
     decm = m['dec'][2:4]
     decs = m['dec'][4:6]
@@ -103,8 +115,8 @@
     # BH: use FK5 as Astropy ICRS implementation seemingly
     # discards equinox information and then convert to icrs
     # coordinate afterwards
     # for the purposes of TART (and most radio telescopes)
     # this does not make any difference ICRS ~= FK5 to few 10s mas level
     return SkyCoord(f"{rah}h{ram}m{ras}s {sign}{decd}d{decm}m{decs}s",
                     equinox=equinox,
-                    frame="fk5").icrs
+                    frame="fk5").icrs
```

### Comparing `tart2ms-0.5.0b2/tart2ms.egg-info/PKG-INFO` & `tart2ms-0.6.0b3/tart2ms.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tart2ms
-Version: 0.5.0b2
+Version: 0.6.0b3
 Summary: Convert TART observation data to Measurement Sets
 Home-page: http://github.com/tmolteno/tart2ms
 Author: Tim Molteno
 Author-email: tim@elec.ac.nz
 License: GPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Scientific/Engineering
@@ -13,16 +13,27 @@
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Intended Audience :: Science/Research
 Description-Content-Type: text/markdown
-Provides-Extra: predict
 License-File: LICENSE.txt
+Requires-Dist: dask-ms
+Requires-Dist: python-casacore
+Requires-Dist: tart
+Requires-Dist: tart_tools
+Requires-Dist: astropy
+Requires-Dist: numpy
+Requires-Dist: h5py
+Requires-Dist: progress
+Requires-Dist: requests
+Requires-Dist: pandas
+Provides-Extra: predict
+Requires-Dist: codex-africanus; extra == "predict"
 
 # tart2ms
 
 [![PyPI package](https://img.shields.io/badge/pip%20install-tart2ms-brightgreen)](https://pypi.org/project/tart2ms) [![version number](https://img.shields.io/pypi/v/tart2ms?color=green&label=version)](https://github.com/tart-telescope/tart2ms/releases) [![License](https://img.shields.io/github/license/tart-telescope/tart2ms)](https://github.com/tart-telescope/tart2ms/blob/master/LICENSE.txt)
 
 
 Convert data from a [TART radio telescope](https://tart.elec.ac.nz) to measurement set format. This module relies on the excellent dask-ms module as a helper to create the measurement sets. This packate requires python-casacore to be installed on your system
@@ -110,14 +121,21 @@
 
 ## TODO
 
 - 
 
 ## Changelog
 
+- 0.6.0b3 If WEIGHT_SPECTRUM is not present, then subsititude ones
+- 0.6.0b2 Clean up the logging code. Add a --debug flag.
+          Get rid of the annoying printing of casa tables
+- 0.6.0b1 New casa_read_ms function similar to read_ms, but uses casacore - blindingly fast.
+          made function signatures the same for both read_ms() and casa_read_ms().
+- 0.5.0b3 Remove noisy warnings. Add venv makefile.
+          Output the snapshot direction in 12-ball format to make rephasing easier.
 - 0.5.0b2 Make prediction an optional dependency to remove codex-africanus from requirements.
 - 0.5.0b1 Add model prediction
           Add automatic catalog download
 - 0.4.0b3 Use the new catalog url functions from tart_tools
 - 0.4.0b2 Add a helper function get_array_location
 - 0.4.0b1 Add a tart2ms.read_ms function (from disko)
           Add utilities for resolution calculations.
```

