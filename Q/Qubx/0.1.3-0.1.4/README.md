# Comparing `tmp/qubx-0.1.3.tar.gz` & `tmp/qubx-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qubx-0.1.3.tar", max compression
+gzip compressed data, was "qubx-0.1.4.tar", max compression
```

## Comparing `qubx-0.1.3.tar` & `qubx-0.1.4.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0      940 2024-04-25 07:51:17.473695 qubx-0.1.3/README.md
--rw-r--r--   0        0        0     9305 2024-04-21 10:35:06.164526 qubx-0.1.3/build.py
--rw-r--r--   0        0        0     1378 2024-05-07 13:17:10.565607 qubx-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     5428 2024-04-21 10:35:06.176526 qubx-0.1.3/src/qubx/__init__.py
--rw-r--r--   0        0        0     1730 2024-04-25 07:51:17.477695 qubx-0.1.3/src/qubx/_nb_magic.py
--rw-r--r--   0        0        0        0 2024-02-29 14:43:31.739720 qubx-0.1.3/src/qubx/core/__init__.py
--rw-r--r--   0        0        0     6707 2024-04-25 07:51:17.477695 qubx-0.1.3/src/qubx/core/account.py
--rw-r--r--   0        0        0    14777 2024-05-07 13:17:10.565607 qubx-0.1.3/src/qubx/core/basics.py
--rw-r--r--   0        0        0    11559 2024-05-07 13:17:10.565607 qubx-0.1.3/src/qubx/core/helpers.py
--rw-r--r--   0        0        0    11910 2024-05-07 13:17:10.565607 qubx-0.1.3/src/qubx/core/loggers.py
--rw-r--r--   0        0        0    13688 2024-04-21 10:35:06.176526 qubx-0.1.3/src/qubx/core/lookups.py
--rw-r--r--   0        0        0     2847 2024-04-21 10:35:06.176526 qubx-0.1.3/src/qubx/core/series.pxd
--rw-r--r--   0        0        0    28108 2024-04-21 10:35:06.176526 qubx-0.1.3/src/qubx/core/series.pyx
--rw-r--r--   0        0        0    30330 2024-05-07 13:17:10.565607 qubx-0.1.3/src/qubx/core/strategy.py
--rw-r--r--   0        0        0     1368 2024-02-29 14:43:31.739720 qubx-0.1.3/src/qubx/core/utils.pyx
--rw-r--r--   0        0        0    20161 2024-05-07 13:17:10.565607 qubx-0.1.3/src/qubx/data/readers.py
--rw-r--r--   0        0        0     9150 2024-05-07 13:17:10.565607 qubx-0.1.3/src/qubx/impl/ccxt_connector.py
--rw-r--r--   0        0        0     3488 2024-05-07 13:17:10.565607 qubx-0.1.3/src/qubx/impl/ccxt_customizations.py
--rw-r--r--   0        0        0     9097 2024-05-07 13:17:10.565607 qubx-0.1.3/src/qubx/impl/ccxt_trading.py
--rw-r--r--   0        0        0     3565 2024-05-07 13:17:10.565607 qubx-0.1.3/src/qubx/impl/ccxt_utils.py
--rw-r--r--   0        0        0       33 2024-02-29 14:43:31.739720 qubx-0.1.3/src/qubx/math/__init__.py
--rw-r--r--   0        0        0     1176 2024-02-29 14:43:31.739720 qubx-0.1.3/src/qubx/math/stats.py
--rw-r--r--   0        0        0        0 2024-02-29 14:43:31.739720 qubx-0.1.3/src/qubx/ta/__init__.py
--rw-r--r--   0        0        0     7708 2024-02-29 14:43:31.739720 qubx-0.1.3/src/qubx/ta/indicators.pyx
--rw-r--r--   0        0        0       60 2024-04-21 10:35:06.176526 qubx-0.1.3/src/qubx/trackers/__init__.py
--rw-r--r--   0        0        0     5522 2024-04-21 10:35:06.176526 qubx-0.1.3/src/qubx/trackers/rebalancers.py
--rw-r--r--   0        0        0      273 2024-05-07 13:17:10.569607 qubx-0.1.3/src/qubx/utils/__init__.py
--rw-r--r--   0        0        0    12076 2024-04-21 10:35:06.176526 qubx-0.1.3/src/qubx/utils/_pyxreloader.py
--rw-r--r--   0        0        0    35158 2024-05-07 13:17:10.569607 qubx-0.1.3/src/qubx/utils/charting/mpl_helpers.py
--rw-r--r--   0        0        0    10999 2024-04-21 10:35:06.176526 qubx-0.1.3/src/qubx/utils/marketdata/binance.py
--rw-r--r--   0        0        0     9837 2024-05-07 13:17:10.569607 qubx-0.1.3/src/qubx/utils/misc.py
--rw-r--r--   0        0        0    18605 2024-05-07 13:17:10.569607 qubx-0.1.3/src/qubx/utils/pandas.py
--rw-r--r--   0        0        0     9277 2024-05-07 13:17:10.569607 qubx-0.1.3/src/qubx/utils/runner.py
--rw-r--r--   0        0        0     4884 2024-05-07 13:17:10.569607 qubx-0.1.3/src/qubx/utils/time.py
--rw-r--r--   0        0        0     2144 1970-01-01 00:00:00.000000 qubx-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      940 2024-04-25 07:51:17.473695 qubx-0.1.4/README.md
+-rw-r--r--   0        0        0     9305 2024-04-21 10:35:06.164526 qubx-0.1.4/build.py
+-rw-r--r--   0        0        0     1378 2024-05-08 18:11:34.565668 qubx-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     5428 2024-04-21 10:35:06.176526 qubx-0.1.4/src/qubx/__init__.py
+-rw-r--r--   0        0        0     1730 2024-04-25 07:51:17.477695 qubx-0.1.4/src/qubx/_nb_magic.py
+-rw-r--r--   0        0        0        0 2024-02-29 14:43:31.739720 qubx-0.1.4/src/qubx/core/__init__.py
+-rw-r--r--   0        0        0     6707 2024-04-25 07:51:17.477695 qubx-0.1.4/src/qubx/core/account.py
+-rw-r--r--   0        0        0    14777 2024-05-07 13:17:10.565607 qubx-0.1.4/src/qubx/core/basics.py
+-rw-r--r--   0        0        0    11559 2024-05-07 13:17:10.565607 qubx-0.1.4/src/qubx/core/helpers.py
+-rw-r--r--   0        0        0    11910 2024-05-07 13:17:10.565607 qubx-0.1.4/src/qubx/core/loggers.py
+-rw-r--r--   0        0        0    13688 2024-04-21 10:35:06.176526 qubx-0.1.4/src/qubx/core/lookups.py
+-rw-r--r--   0        0        0     2847 2024-04-21 10:35:06.176526 qubx-0.1.4/src/qubx/core/series.pxd
+-rw-r--r--   0        0        0    28108 2024-04-21 10:35:06.176526 qubx-0.1.4/src/qubx/core/series.pyx
+-rw-r--r--   0        0        0    30330 2024-05-07 13:17:10.565607 qubx-0.1.4/src/qubx/core/strategy.py
+-rw-r--r--   0        0        0     1368 2024-02-29 14:43:31.739720 qubx-0.1.4/src/qubx/core/utils.pyx
+-rw-r--r--   0        0        0    19648 2024-05-08 18:11:34.565668 qubx-0.1.4/src/qubx/data/readers.py
+-rw-r--r--   0        0        0     9150 2024-05-07 13:17:10.565607 qubx-0.1.4/src/qubx/impl/ccxt_connector.py
+-rw-r--r--   0        0        0     3488 2024-05-07 13:17:10.565607 qubx-0.1.4/src/qubx/impl/ccxt_customizations.py
+-rw-r--r--   0        0        0     9097 2024-05-07 13:17:10.565607 qubx-0.1.4/src/qubx/impl/ccxt_trading.py
+-rw-r--r--   0        0        0     3565 2024-05-07 13:17:10.565607 qubx-0.1.4/src/qubx/impl/ccxt_utils.py
+-rw-r--r--   0        0        0       33 2024-02-29 14:43:31.739720 qubx-0.1.4/src/qubx/math/__init__.py
+-rw-r--r--   0        0        0     1176 2024-02-29 14:43:31.739720 qubx-0.1.4/src/qubx/math/stats.py
+-rw-r--r--   0        0        0        0 2024-02-29 14:43:31.739720 qubx-0.1.4/src/qubx/ta/__init__.py
+-rw-r--r--   0        0        0     7708 2024-02-29 14:43:31.739720 qubx-0.1.4/src/qubx/ta/indicators.pyx
+-rw-r--r--   0        0        0       60 2024-04-21 10:35:06.176526 qubx-0.1.4/src/qubx/trackers/__init__.py
+-rw-r--r--   0        0        0     5522 2024-04-21 10:35:06.176526 qubx-0.1.4/src/qubx/trackers/rebalancers.py
+-rw-r--r--   0        0        0      273 2024-05-07 13:17:10.569607 qubx-0.1.4/src/qubx/utils/__init__.py
+-rw-r--r--   0        0        0    12076 2024-04-21 10:35:06.176526 qubx-0.1.4/src/qubx/utils/_pyxreloader.py
+-rw-r--r--   0        0        0    35158 2024-05-07 13:17:10.569607 qubx-0.1.4/src/qubx/utils/charting/mpl_helpers.py
+-rw-r--r--   0        0        0    10999 2024-04-21 10:35:06.176526 qubx-0.1.4/src/qubx/utils/marketdata/binance.py
+-rw-r--r--   0        0        0     9837 2024-05-07 13:17:10.569607 qubx-0.1.4/src/qubx/utils/misc.py
+-rw-r--r--   0        0        0    18605 2024-05-07 13:17:10.569607 qubx-0.1.4/src/qubx/utils/pandas.py
+-rw-r--r--   0        0        0     9277 2024-05-07 13:17:10.569607 qubx-0.1.4/src/qubx/utils/runner.py
+-rw-r--r--   0        0        0     4884 2024-05-07 13:17:10.569607 qubx-0.1.4/src/qubx/utils/time.py
+-rw-r--r--   0        0        0     2144 1970-01-01 00:00:00.000000 qubx-0.1.4/PKG-INFO
```

### Comparing `qubx-0.1.3/README.md` & `qubx-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `qubx-0.1.3/build.py` & `qubx-0.1.4/build.py`

 * *Files identical despite different names*

### Comparing `qubx-0.1.3/pyproject.toml` & `qubx-0.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "Qubx"
-version = "0.1.3"
+version = "0.1.4"
 description = "Qubx - quantitative trading framework"
 authors = ["Dmitry Marienko <dmitry@gmail.com>"]
 readme = "README.md"
 packages = [
     { include = "qubx", from = "src" },
 ]
 repository = "https://github.com/dmarienko/Qubx"
```

### Comparing `qubx-0.1.3/src/qubx/__init__.py` & `qubx-0.1.4/src/qubx/__init__.py`

 * *Files identical despite different names*

### Comparing `qubx-0.1.3/src/qubx/_nb_magic.py` & `qubx-0.1.4/src/qubx/_nb_magic.py`

 * *Files identical despite different names*

### Comparing `qubx-0.1.3/src/qubx/core/account.py` & `qubx-0.1.4/src/qubx/core/account.py`

 * *Files identical despite different names*

### Comparing `qubx-0.1.3/src/qubx/core/basics.py` & `qubx-0.1.4/src/qubx/core/basics.py`

 * *Files identical despite different names*

### Comparing `qubx-0.1.3/src/qubx/core/helpers.py` & `qubx-0.1.4/src/qubx/core/helpers.py`

 * *Files identical despite different names*

### Comparing `qubx-0.1.3/src/qubx/core/loggers.py` & `qubx-0.1.4/src/qubx/core/loggers.py`

 * *Files identical despite different names*

### Comparing `qubx-0.1.3/src/qubx/core/lookups.py` & `qubx-0.1.4/src/qubx/core/lookups.py`

 * *Files identical despite different names*

### Comparing `qubx-0.1.3/src/qubx/core/series.pxd` & `qubx-0.1.4/src/qubx/core/series.pxd`

 * *Files identical despite different names*

### Comparing `qubx-0.1.3/src/qubx/core/series.pyx` & `qubx-0.1.4/src/qubx/core/series.pyx`

 * *Files identical despite different names*

### Comparing `qubx-0.1.3/src/qubx/core/strategy.py` & `qubx-0.1.4/src/qubx/core/strategy.py`

 * *Files identical despite different names*

### Comparing `qubx-0.1.3/src/qubx/core/utils.pyx` & `qubx-0.1.4/src/qubx/core/utils.pyx`

 * *Files identical despite different names*

### Comparing `qubx-0.1.3/src/qubx/data/readers.py` & `qubx-0.1.4/src/qubx/data/readers.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-import re
-from typing import List, Union, Optional, Iterable, Any
-from os.path import exists
+import re, os
+from typing import Callable, List, Union, Optional, Iterable, Any
+from os.path import exists, join
 import numpy as np
 import pandas as pd
 import pyarrow as pa
 from pyarrow import csv
 import psycopg as pg
 from functools import wraps
 
@@ -34,147 +34,366 @@
     for a in args:
         ai = a.lower()
         if ai in xs:
             return xs.index(ai)
     raise IndexError(f"Can't find any from {args} in list: {xs}")
 
 
-class DataProcessor:
-    """
-    Common interface for data processor with default aggregating into list implementation
-    """
+class DataTransformer:
+
     def __init__(self) -> None:
-        self.buffer = {}
+        self.buffer = []
         self._column_names = []
 
-    def start_processing(self, column_names: List[str], name: str | None = None):
+    def start_transform(self, name: str, column_names: List[str]):
         self._column_names = column_names
-        self.buffer = {c: [] for c in column_names}
-
-    def process_data_columns(self, columns_data: list) -> Optional[Iterable]:
-        for i, c in enumerate(columns_data):
-            self.buffer[self._column_names[i]].append(c)
-        return None
-
-    def process_data_rows(self, rows_data: list) -> Optional[Iterable]:
-        for r in rows_data:
-            c = []
-            for j, d in enumerate(r):
-                self.buffer[self._column_names[j]].append(d)
-        return None
+        self.buffer = []
+    
+    def process_data(self, rows_data: Iterable) -> Any:
+        if rows_data is not None: 
+            self.buffer.extend(rows_data)
 
-    def get_result(self) -> Any:
+    def collect(self) -> Any:
         return self.buffer
 
 
 class DataReader:
+
+    def get_names(self) -> List[str] :
+        raise NotImplemented()
+
+    def read(self, data_id: str, start: str | None=None, stop: str | None=None, 
+             transform: DataTransformer = DataTransformer(), 
+             chunksize=0, 
+             **kwargs
+            ) -> Iterable | List:
+        raise NotImplemented()
+
+
+class CsvStorageDataReader(DataReader):
     """
-    Common interface for data reader
+    Data reader for timeseries data stored as csv files in the specified directory
     """
-    _processor: DataProcessor
 
-    def __init__(self, processor=None) -> None:
-        self._processor = DataProcessor() if processor is None else processor
+    def __init__(self, path: str) -> None:
+        if not exists(path):
+            raise ValueError(f"Folder is not found at {path}")
+        self.path = path
 
-    def read(self, start: Optional[str]=None, stop: Optional[str]=None) -> Any:
-        pass
+    def __find_time_idx(self, arr: pa.ChunkedArray, v) -> int:
+        ix = arr.index(v).as_py()
+        if ix < 0:
+            for c in arr.iterchunks():
+                a = c.to_numpy()
+                ix = np.searchsorted(a, v, side='right')
+                if ix > 0 and ix < len(c):
+                    ix = arr.index(a[ix]).as_py() - 1
+                    break
+        return ix
 
-    
-class QuotesDataProcessor(DataProcessor):
+    def __check_file_name(self, name: str) -> str | None:
+        _f = join(self.path, name)
+        for sfx in ['.csv', '.csv.gz', '']:
+            if exists(p:=(_f + sfx)):
+                return p 
+        return None
+
+    def read(self, data_id: str, start: str | None=None, stop: str | None=None, 
+             transform: DataTransformer = DataTransformer(),
+             chunksize=0,
+             timestamp_formatters = None
+            ) -> Iterable | Any:
+
+        f_path = self.__check_file_name(data_id)
+        if not f_path:
+            ValueError(f"Can't find any csv data for {data_id} in {self.path} !")
+
+        convert_options = None
+        if timestamp_formatters is not None:
+            convert_options=csv.ConvertOptions(timestamp_parsers=timestamp_formatters)
+
+        table = csv.read_csv(
+            f_path, 
+            parse_options=csv.ParseOptions(ignore_empty_lines=True),
+            convert_options=convert_options
+        )
+        fieldnames =  table.column_names  
+
+        # - try to find range to load  
+        start_idx, stop_idx = 0, table.num_rows
+        try:
+            _time_field_idx = _find_column_index_in_list(fieldnames, 'time', 'timestamp', 'datetime', 'date')
+            _time_type = table.field(_time_field_idx).type
+            _time_unit = _time_type.unit if hasattr(_time_type, 'unit') else 's'
+            _time_data = table[_time_field_idx]
+
+            # - check if need convert time to primitive types (i.e. Date32 -> timestamp[x])
+            _time_cast_function = lambda xs: xs
+            if _time_type != pa.timestamp(_time_unit):
+                _time_cast_function = lambda xs: xs.cast(pa.timestamp(_time_unit)) 
+                _time_data = _time_cast_function(_time_data)
+
+            # - preprocessing start and stop
+            t_0, t_1 = handle_start_stop(start, stop, convert=lambda x: _recognize_t(x, None, _time_unit))
+
+            # - check requested range
+            if t_0:
+                start_idx = self.__find_time_idx(_time_data, t_0)
+                if start_idx >= table.num_rows:
+                    # no data for requested start date
+                    return None
+
+            if t_1:
+                stop_idx = self.__find_time_idx(_time_data, t_1)
+                if stop_idx < 0 or stop_idx < start_idx:
+                    stop_idx = table.num_rows
+
+        except Exception as exc:
+            logger.warning(exc)
+            logger.info('loading whole file')
+
+        length = (stop_idx - start_idx + 1)
+        selected_table = table.slice(start_idx, length)
+
+        # - in this case we want to return iterable chunks of data
+        if chunksize > 0:
+            def _iter_chunks():
+                for n in range(0, length // chunksize + 1):
+                    transform.start_transform(data_id, fieldnames)
+                    raw_data = selected_table[n*chunksize : min((n+1)*chunksize, length)].to_pandas().to_numpy()
+                    transform.process_data(raw_data)
+                    yield transform.collect()
+            return _iter_chunks()
+
+        transform.start_transform(data_id, fieldnames)
+        raw_data = selected_table.to_pandas().to_numpy()
+        transform.process_data(raw_data)
+        return transform.collect()
+
+    def get_names(self) -> List[str] :
+        _n = []
+        for s in os.listdir(self.path):
+            if (m:=re.match(r'(.*)\.csv(.gz)?$', s)):
+                _n.append(m.group(1))
+        return _n
+
+
+class AsPandasFrame(DataTransformer):
     """
-    Process quotes data and collect them as list
+    List of records to pandas dataframe transformer
     """
-    def start_processing(self, fieldnames: List[str], name: str | None = None):
-        self.buffer = list()
-        self._time_idx = _find_column_index_in_list(fieldnames, 'time', 'timestamp', 'datetime')
-        self._bid_idx = _find_column_index_in_list(fieldnames, 'bid')
-        self._ask_idx = _find_column_index_in_list(fieldnames, 'ask')
-        self._bidvol_idx = _find_column_index_in_list(fieldnames, 'bidvol', 'bid_vol', 'bidsize', 'bid_size')
-        self._askvol_idx = _find_column_index_in_list(fieldnames, 'askvol', 'ask_vol', 'asksize', 'ask_size')
-
-    def process_data_columns(self, columns_data: list) -> Optional[Iterable]:
-        tms = columns_data[self._time_idx] 
-        bids = columns_data[self._bid_idx]
-        asks = columns_data[self._ask_idx]
-        bidvol = columns_data[self._bidvol_idx]
-        askvol = columns_data[self._askvol_idx]
-        for i in range(len(tms)):
-            self.buffer.append(Quote(tms[i], bids[i], asks[i], bidvol[i], askvol[i]))
+
+    def start_transform(self, name: str, column_names: List[str]):
+        self._time_idx = _find_column_index_in_list(column_names, 'time', 'timestamp', 'datetime', 'date')
+        self._column_names = column_names
+        self._frame = pd.DataFrame()
+    
+    def process_data(self, rows_data: Iterable) -> Any:
+        self._frame
+        p = pd.DataFrame.from_records(rows_data, columns=self._column_names)
+        p.set_index(self._column_names[self._time_idx], drop=True, inplace=True)
+        p.sort_index(inplace=True)
+        self._frame = pd.concat((self._frame, p), axis=0, sort=True)
+        return p
+
+    def collect(self) -> Any:
+        return self._frame 
+
+
+class AsOhlcvSeries(DataTransformer):
+
+    def __init__(self, timeframe: str | None = None, timestamp_units='ns') -> None:
+        super().__init__()
+        self.timeframe = timeframe 
+        self._series = None
+        self._data_type = None
+        self.timestamp_units = timestamp_units
+
+    def start_transform(self, name: str, column_names: List[str]):
+        self._time_idx = _find_column_index_in_list(column_names, 'time', 'timestamp', 'datetime', 'date')
+        self._volume_idx = None
+        self._b_volume_idx = None
+        try:
+            self._close_idx = _find_column_index_in_list(column_names, 'close')
+            self._open_idx = _find_column_index_in_list(column_names, 'open')
+            self._high_idx = _find_column_index_in_list(column_names, 'high')
+            self._low_idx = _find_column_index_in_list(column_names, 'low')
+
+            try:
+                self._volume_idx = _find_column_index_in_list(column_names, 'quote_volume', 'volume', 'vol')
+            except: pass
+
+            try:
+                self._b_volume_idx = _find_column_index_in_list(column_names, 'taker_buy_volume', 'taker_buy_quote_volume', 'buy_volume')
+            except: pass
+
+            self._data_type = 'ohlc'
+        except: 
+            try:
+                self._ask_idx = _find_column_index_in_list(column_names, 'ask')
+                self._bid_idx = _find_column_index_in_list(column_names, 'bid')
+                self._data_type = 'quotes'
+            except: 
+
+                try:
+                    self._price_idx = _find_column_index_in_list(column_names, 'price')
+                    self._size_idx = _find_column_index_in_list(column_names, 'quote_qty', 'qty', 'size', 'amount', 'volume')
+                    self._taker_idx = None
+                    try:
+                        self._taker_idx = _find_column_index_in_list(column_names, 'is_buyer_maker', 'side', 'aggressive', 'taker', 'is_taker')
+                    except: pass
+
+                    self._data_type = 'trades'
+                except: 
+                    raise ValueError(f"Can't recognize data for update from header: {column_names}")
+
+        self._column_names = column_names
+        self._name = name
+        if self.timeframe:
+            self._series = OHLCV(self._name, self.timeframe)
+
+    def _time(self, t) -> int:
+        if self.timestamp_units == 'ns':
+            return np.datetime64(t, 'ns').item() 
+        return np.datetime64(t, self.timestamp_units).astype('datetime64[ns]').item()
+
+    def _proc_ohlc(self, rows_data: List[List]):
+        for d in rows_data:
+            self._series.update_by_bar(
+                self._time(d[self._time_idx]),
+                d[self._open_idx], d[self._high_idx], d[self._low_idx], d[self._close_idx], 
+                d[self._volume_idx] if self._volume_idx else 0,
+                d[self._b_volume_idx] if self._b_volume_idx else 0
+            )
+
+    def _proc_quotes(self, rows_data: List[List]):
+        for d in rows_data:
+            self._series.update(
+                self._time(d[self._time_idx]),
+                (d[self._ask_idx] + d[self._bid_idx])/2
+            )
+
+    def _proc_trades(self, rows_data: List[List]):
+        for d in rows_data:
+            a = d[self._taker_idx] if self._taker_idx else 0
+            s = d[self._size_idx]
+            b = s if a else 0 
+            self._series.update(self._time(d[self._time_idx]), d[self._price_idx], s, b)
+
+    def process_data(self, rows_data: List[List]) -> Any:
+        if self._series is None:
+            ts = [t[self._time_idx] for t in rows_data[:100]]
+            self.timeframe = pd.Timedelta(infer_series_frequency(ts)).asm8.item()
+
+            # - create instance after first data received if 
+            self._series = OHLCV(self._name, self.timeframe)
+
+        match self._data_type:
+            case 'ohlc':
+                self._proc_ohlc(rows_data)
+            case 'quotes':
+                self._proc_quotes(rows_data)
+            case 'trades':
+                self._proc_trades(rows_data)
+
         return None
 
+    def collect(self) -> Any:
+        return self._series
+
+
+class AsQuotes(DataTransformer):
 
-class QuotesFromOHLCVDataProcessor(DataProcessor):
+    def start_transform(self, name: str, column_names: List[str]):
+        self.buffer = list()
+        self._time_idx = _find_column_index_in_list(column_names, 'time', 'timestamp', 'datetime')
+        self._bid_idx = _find_column_index_in_list(column_names, 'bid')
+        self._ask_idx = _find_column_index_in_list(column_names, 'ask')
+        self._bidvol_idx = _find_column_index_in_list(column_names, 'bidvol', 'bid_vol', 'bidsize', 'bid_size')
+        self._askvol_idx = _find_column_index_in_list(column_names, 'askvol', 'ask_vol', 'asksize', 'ask_size')
+
+    def process_data(self, rows_data: Iterable) -> Any:
+        if rows_data is not None: 
+            for d in rows_data:
+                t = d[self._time_idx] 
+                b = d[self._bid_idx]
+                a = d[self._ask_idx]
+                bv = d[self._bidvol_idx]
+                av = d[self._askvol_idx]
+                self.buffer.append(Quote(t.as_unit('ns').asm8.item(), b, a, bv, av))
+
+
+class RestoreTicksFromOHLC(DataTransformer):
     """
-    Process OHLC and generate Quotes (+ Trades) from it
+    Emulates quotes (and trades) from OHLC bars
     """
-    def __init__(self, trades: bool=False, 
+
+    def __init__(self, 
+                 trades: bool=False,    # if we also wants 'trades'
                  default_bid_size=1e9,  # default bid/ask is big
                  default_ask_size=1e9,  # default bid/ask is big
                  daily_session_start_end=DEFAULT_DAILY_SESSION,
-                 spread=0.0,
-                ) -> None:
+                 spread=0.0):
         super().__init__()
         self._trades = trades
         self._bid_size = default_bid_size
         self._ask_size = default_ask_size
         self._s2 = spread / 2.0
         self._d_session_start = daily_session_start_end[0]
         self._d_session_end = daily_session_start_end[1]
 
-    def start_processing(self, fieldnames: List[str], name: str | None = None):
-        self._time_idx = _find_column_index_in_list(fieldnames, 'time', 'timestamp', 'datetime', 'date')
-        self._open_idx = _find_column_index_in_list(fieldnames, 'open')
-        self._high_idx = _find_column_index_in_list(fieldnames, 'high')
-        self._low_idx = _find_column_index_in_list(fieldnames, 'low')
-        self._close_idx = _find_column_index_in_list(fieldnames, 'close')
+    def start_transform(self, name: str, column_names: List[str]):
+        self.buffer = []
+        # - it will fail if receive data doesn't look as ohlcv 
+        self._time_idx = _find_column_index_in_list(column_names, 'time', 'timestamp', 'datetime', 'date')
+        self._open_idx = _find_column_index_in_list(column_names, 'open')
+        self._high_idx = _find_column_index_in_list(column_names, 'high')
+        self._low_idx = _find_column_index_in_list(column_names, 'low')
+        self._close_idx = _find_column_index_in_list(column_names, 'close')
         self._volume_idx = None
-        self._timeframe = None
-
+        self._freq = None
         try:
-            self._volume_idx = _find_column_index_in_list(fieldnames, 'volume', 'vol')
-        except:
-            pass
+            self._volume_idx = _find_column_index_in_list(column_names, 'volume', 'vol')
+        except: pass
 
-        self.buffer = []
+        if self._volume_idx is None and self._trades:
+            logger.warning("Input OHLC data doesn't contain volume information so trades can't be emulated !")
+            self._trades = False
+
+    def process_data(self, rows_data:List[List]) -> Any:
+        if rows_data is None: 
+            return
 
-    def process_data_columns(self, data: list) -> Optional[Iterable]:
         s2 = self._s2
-        if self._timeframe is None:
-            _freq = infer_series_frequency(data[self._time_idx])
-            self._timeframe = _freq.astype('timedelta64[s]')
+
+        if self._freq is None:
+            ts = [t[self._time_idx] for t in rows_data[:100]]
+            self._freq = infer_series_frequency(ts)
 
             # - timestamps when we emit simulated quotes
-            dt = _freq.astype('timedelta64[ns]').item()
+            dt = self._freq.astype('timedelta64[ns]').item()
             if dt < D1:
                 self._t_start = dt // 10
                 self._t_mid1 = dt // 2 - dt // 10
                 self._t_mid2 = dt // 2 + dt // 10
                 self._t_end = dt - dt // 10
             else:
                 self._t_start = self._d_session_start
                 self._t_mid1 = dt // 2 - H1
                 self._t_mid2 = dt // 2 + H1
                 self._t_end = self._d_session_end
 
         # - input data
-        times = data[self._time_idx]
-        opens = data[self._open_idx]
-        highs = data[self._high_idx]
-        lows = data[self._low_idx]
-        closes = data[self._close_idx]
-        volumes = data[self._volume_idx] if self._volume_idx else None
-        if volumes is None and self._trades:
-            logger.warning("Input OHLC data doesn't contain volume information so trades can't be emulated !")
-            self._trades = False
-
-        for i in range(len(times)):
-            ti, o, h, l, c = times[i].astype('datetime64[ns]'), opens[i], highs[i], lows[i], closes[i]
-
-            if self._trades:
-                rv = volumes[i] / (h - l) 
+        for data in rows_data:
+            ti = pd.Timestamp(data[self._time_idx]).as_unit('ns').asm8.item()
+            o = data[self._open_idx]
+            h=  data[self._high_idx]
+            l = data[self._low_idx]
+            c = data[self._close_idx]
+            rv = data[self._volume_idx] if self._volume_idx else 0
 
             # - opening quote
             self.buffer.append(Quote(ti + self._t_start, o - s2, o + s2, self._bid_size, self._ask_size))
 
             if c >= o:
                 if self._trades:
                     self.buffer.append(Trade(ti + self._t_start, o - s2, rv * (o - l))) # sell 1
@@ -197,246 +416,14 @@
 
                 if self._trades:
                     self.buffer.append(Trade(ti + self._t_mid2, l + s2, rv * (c - l))) # buy 2
 
             # - closing quote
             self.buffer.append(Quote(ti + self._t_end, c - s2, c + s2, self._bid_size, self._ask_size))
 
-        return None
-
-    def get_result(self) -> Any:
-        return self.buffer
-
-
-class OhlcvDataProcessor(DataProcessor):
-    """
-    Process data and convert it to Qube OHLCV timeseries 
-    """
-    def __init__(self, name: str | None = None) -> None:
-        super().__init__()
-        self._name = name
-
-    def start_processing(self, fieldnames: List[str], name: str | None = None):
-        self._time_idx = _find_column_index_in_list(fieldnames, 'time', 'timestamp', 'datetime', 'date')
-        self._open_idx = _find_column_index_in_list(fieldnames, 'open')
-        self._high_idx = _find_column_index_in_list(fieldnames, 'high')
-        self._low_idx = _find_column_index_in_list(fieldnames, 'low')
-        self._close_idx = _find_column_index_in_list(fieldnames, 'close')
-        self._volume_idx = None
-        self._b_volume_idx = None
-        self._timeframe = None
-        self._name = name if name else self._name
-
-        try:
-            self._volume_idx = _find_column_index_in_list(fieldnames, 'quote_volume', 'volume', 'vol')
-        except: pass
-
-        try:
-            self._b_volume_idx = _find_column_index_in_list(fieldnames, 'taker_buy_volume', 'taker_buy_quote_volume', 'buy_volume')
-        except: pass
-
-        self.ohlc = None
-
-    def process_data_columns(self, data: list) -> Optional[Iterable]:
-        if self._timeframe is None:
-            self._timeframe = infer_series_frequency(data[self._time_idx]).astype('timedelta64[s]')
-
-            # - create instance after first data received
-            self.ohlc = OHLCV(self._name, self._timeframe)
-
-        self.ohlc.append_data(
-            data[self._time_idx],
-            data[self._open_idx], data[self._high_idx], data[self._low_idx], data[self._close_idx], 
-            data[self._volume_idx] if self._volume_idx else np.empty(0),
-            data[self._b_volume_idx] if self._b_volume_idx else np.empty(0)
-        )
-        return None
-
-    def process_data_rows(self, data: List[list]) -> Iterable | None:
-        if self._timeframe is None:
-            ts = [t[self._time_idx] for t in data[:100]]
-            self._timeframe = pd.Timedelta(infer_series_frequency(ts)).asm8.item()
-
-            # - create instance after first data received
-            self.ohlc = OHLCV(self._name, self._timeframe)
-
-        for d in data:
-            self.ohlc.update_by_bar(
-                np.datetime64(d[self._time_idx], 'ns').item(),
-                d[self._open_idx], d[self._high_idx], d[self._low_idx], d[self._close_idx], 
-                d[self._volume_idx] if self._volume_idx else 0,
-                d[self._b_volume_idx] if self._b_volume_idx else 0
-            )
-        return None
-
-    def get_result(self) -> Any:
-        return self.ohlc
-
-
-class OhlcvPandasDataProcessor(DataProcessor):
-    """
-    Process data and convert it to pandas OHLCV dataframes 
-    """
-    def __init__(self) -> None:
-        super().__init__()
-        self._fieldnames: List = []
-
-    def start_processing(self, fieldnames: List[str], name: str | None = None):
-        self._time_idx = _find_column_index_in_list(fieldnames, 'time', 'timestamp', 'datetime', 'date')
-        self._open_idx = _find_column_index_in_list(fieldnames, 'open')
-        self._high_idx = _find_column_index_in_list(fieldnames, 'high')
-        self._low_idx = _find_column_index_in_list(fieldnames, 'low')
-        self._close_idx = _find_column_index_in_list(fieldnames, 'close')
-        self._volume_idx = None
-        self._b_volume_idx = None
-        self._timeframe = None
-
-        try:
-            self._volume_idx = _find_column_index_in_list(fieldnames, 'quote_volume', 'volume', 'vol')
-        except: pass
-
-        try:
-            self._b_volume_idx = _find_column_index_in_list(fieldnames, 'taker_buy_volume', 'taker_buy_quote_volume', 'buy_volume')
-        except: pass
-
-        self._time = np.array([], dtype=np.datetime64)
-        self._open = np.array([])
-        self._high = np.array([])
-        self._low = np.array([])
-        self._close = np.array([])
-        self._volume = np.array([])
-        self._bvolume = np.array([])
-        self._fieldnames = fieldnames
-        self._ohlc = pd.DataFrame()
-
-    def process_data_rows(self, data: List[list]) -> Optional[Iterable]:
-        p = pd.DataFrame.from_records(data, columns=self._fieldnames)
-        p.set_index(self._fieldnames[self._time_idx], drop=True, inplace=True)
-        self._ohlc = pd.concat((self._ohlc, p), axis=0, sort=True, copy=True)
-        return None
-
-    def process_data_columns(self, data: list) -> Optional[Iterable]:
-        # p = pd.DataFrame({
-        #     'open': data[self._open_idx], 
-        #     'high': data[self._high_idx], 
-        #     'low': data[self._low_idx], 
-        #     'close': data[self._close_idx], 
-        #     'volume': data[self._volume_idx] if self._volume_idx else []},
-        #     index = data[self._time_idx]
-        # )
-        # self.ohlc = pd.concat((self.ohlc, p), axis=0, sort=True, copy=True)
-        self._time = np.concatenate((self._time, data[self._time_idx]))
-        self._open = np.concatenate((self._open, data[self._open_idx]))
-        self._high = np.concatenate((self._high, data[self._high_idx]))
-        self._low = np.concatenate((self._low, data[self._low_idx]))
-        self._close = np.concatenate((self._close, data[self._close_idx]))
-        if self._volume_idx:
-            self._volume = np.concatenate((self._volume, data[self._volume_idx]))
-        if self._b_volume_idx:
-            self._bvolume = np.concatenate((self._bvolume, data[self._b_volume_idx]))
-
-        return None
-
-    def get_result(self) -> Any:
-        if not self._ohlc.empty:
-            return self._ohlc
-
-        rd = {
-            'open': self._open, 'high': self._high, 'low': self._low, 'close': self._close, 
-        }
-
-        if self._volume_idx:
-            rd['volume'] = self._volume
-
-        if self._b_volume_idx:
-            rd['taker_buy_quote_volume'] = self._bvolume
-
-        return pd.DataFrame(rd, index = self._time).sort_index()
- 
-
-class CsvDataReader(DataReader):
-    """
-    CSV data file reader
-    """
-
-    def __init__(self, path: str, processor: DataProcessor|None=None, timestamp_parsers=None) -> None:
-        if not exists(path):
-            raise ValueError(f"CSV file not found at {path}")
-        super().__init__(processor)
-        self.time_parsers = timestamp_parsers
-        self.path = path
-
-    def __find_time_idx(self, arr: pa.ChunkedArray, v) -> int:
-        ix = arr.index(v).as_py()
-        if ix < 0:
-            for c in arr.iterchunks():
-                a = c.to_numpy()
-                ix = np.searchsorted(a, v, side='right')
-                if ix > 0 and ix < len(c):
-                    ix = arr.index(a[ix]).as_py() - 1
-                    break
-        return ix
-
-    def read(self, start: Optional[str]=None, stop: Optional[str]=None) -> Any:
-        convert_options = None
-        if self.time_parsers:
-            convert_options=csv.ConvertOptions(timestamp_parsers=self.time_parsers)
-
-        table = csv.read_csv(
-            self.path, 
-            parse_options=csv.ParseOptions(ignore_empty_lines=True),
-            convert_options=convert_options
-        )
-        fieldnames =  table.column_names  
-
-        # - try to find range to load  
-        start_idx, stop_idx = 0, table.num_rows
-        try:
-            _time_field_idx = _find_column_index_in_list(fieldnames, 'time', 'timestamp', 'datetime', 'date')
-            _time_type = table.field(_time_field_idx).type
-            _time_unit = _time_type.unit if hasattr(_time_type, 'unit') else 's'
-            _time_data = table[_time_field_idx]
-
-            # - check if need convert time to primitive types (i.e. Date32 -> timestamp[x])
-            _time_cast_function = lambda xs: xs
-            if _time_type != pa.timestamp(_time_unit):
-                _time_cast_function = lambda xs: xs.cast(pa.timestamp(_time_unit)) 
-                _time_data = _time_cast_function(_time_data)
-
-            # - preprocessing start and stop
-            t_0, t_1 = handle_start_stop(start, stop, convert=lambda x: _recognize_t(x, None, _time_unit))
-
-            # - check requested range
-            if t_0:
-                start_idx = self.__find_time_idx(_time_data, t_0)
-                if start_idx >= table.num_rows:
-                    # no data for requested start date
-                    return None
-
-            if t_1:
-                stop_idx = self.__find_time_idx(_time_data, t_1)
-                if stop_idx < 0 or stop_idx < start_idx:
-                    stop_idx = table.num_rows
-
-        except Exception as exc:
-            logger.warning(exc)
-            logger.info('loading whole file')
-
-        length = (stop_idx - start_idx + 1)
-        self._processor.start_processing(fieldnames)
-        selected_table = table.slice(start_idx, length)
-        n_chunks = selected_table[table.column_names[0]].num_chunks
-        for n in range(n_chunks):
-            data = [
-                # - in some cases we need to convert time index to primitive type
-                _time_cast_function(selected_table[k].chunk(n)).to_numpy() if k == _time_field_idx else selected_table[k].chunk(n).to_numpy()
-                for k in range(selected_table.num_columns)]
-            self._processor.process_data_columns(data)
-        return self._processor.get_result()
-
 
 def _retry(fn):
     @wraps(fn)
     def wrapper(*args, **kw):
         cls = args[0]
         for x in range(cls._reconnect_tries):
             # print(x, cls._reconnect_tries)
@@ -452,38 +439,43 @@
 
 class QuestDBConnector(DataReader):
     """
     Very first version of QuestDB connector
 
     # Connect to an existing QuestDB instance
     >>> db = QuestDBConnector('user=admin password=quest host=localhost port=8812', OhlcvPandasDataProcessor())
-    >>> db.read('BINANCEF.ETHUSDT', '5m', '2024-01-01')
+    >>> db.read('BINANCEF.ETHUSDT', '2024-01-01')
     """
     _reconnect_tries = 5
     _reconnect_idle = 0.1  # wait seconds before retying
 
-    def __init__(self, connection_url: str, processor: DataProcessor | None=None) -> None:
-        super().__init__(processor)
+    def __init__(self, connection_url: str) -> None:
         self._connection = None
         self._cursor = None
         self.connection_url = connection_url
         self._connect()
 
     def _connect(self):
         logger.info("Connecting to QuestDB ...")
         self._connection = pg.connect(self.connection_url, autocommit=True)
         self._cursor = self._connection.cursor()
 
     @_retry
-    def read(self, symbol: str, timeframe: str, start: str|None=None, stop: str|None=None) -> Any:
+    def read(self, data_id: str, start: str|None=None, stop: str|None=None, 
+             transform: DataTransformer = DataTransformer(),
+             chunksize=0,  # TODO: use self._cursor.fetchmany in this case !!!!
+             timeframe: str='1m') -> Any:
         start, end = handle_start_stop(start, stop)
         w0 = f"timestamp >= '{start}'" if start else ''
         w1 = f"timestamp <= '{end}'" if end else ''
         where = f'where {w0} and {w1}' if (w0 and w1) else f"where {(w0 or w1)}"
 
+        # just a temp hack - actually we need to discuss symbology etc
+        symbol = data_id#.split('.')[-1]
+
         self._cursor.execute(
             f"""
                 select timestamp, 
                 first(open) as open, 
                 max(high) as high,
                 min(low) as low,
                 last(close) as close,
@@ -492,22 +484,28 @@
                 sum(count) as count,
                 sum(taker_buy_volume) as taker_buy_volume,
                 sum(taker_buy_quote_volume) as taker_buy_quote_volume
                 from "{symbol.upper()}" {where}
                 SAMPLE by {timeframe};
             """ # type: ignore
         )
-        records = self._cursor.fetchall()
+        records = self._cursor.fetchall() # TODO: for chunksize > 0 use fetchmany etc
         names = [d.name for d in self._cursor.description]
 
-        self._processor.start_processing(names, re.split(r'[.:]', symbol)[-1])
+        transform.start_transform(data_id, names)
         
         # d = np.array(records)
-        self._processor.process_data_rows(records)
-        return self._processor.get_result()
+        transform.process_data(records)
+        return transform.collect()
+
+    @_retry
+    def get_names(self) -> List[str] :
+        self._cursor.execute("select table_name from tables()")
+        records = self._cursor.fetchall()
+        return [r[0] for r in records]
 
     def __del__(self):
         for c in (self._cursor, self._connection):
             try:
                 logger.info("Closing connection")
                 c.close()
             except:
```

### Comparing `qubx-0.1.3/src/qubx/impl/ccxt_connector.py` & `qubx-0.1.4/src/qubx/impl/ccxt_connector.py`

 * *Files identical despite different names*

### Comparing `qubx-0.1.3/src/qubx/impl/ccxt_customizations.py` & `qubx-0.1.4/src/qubx/impl/ccxt_customizations.py`

 * *Files identical despite different names*

### Comparing `qubx-0.1.3/src/qubx/impl/ccxt_trading.py` & `qubx-0.1.4/src/qubx/impl/ccxt_trading.py`

 * *Files identical despite different names*

### Comparing `qubx-0.1.3/src/qubx/impl/ccxt_utils.py` & `qubx-0.1.4/src/qubx/impl/ccxt_utils.py`

 * *Files identical despite different names*

### Comparing `qubx-0.1.3/src/qubx/math/stats.py` & `qubx-0.1.4/src/qubx/math/stats.py`

 * *Files identical despite different names*

### Comparing `qubx-0.1.3/src/qubx/ta/indicators.pyx` & `qubx-0.1.4/src/qubx/ta/indicators.pyx`

 * *Files identical despite different names*

### Comparing `qubx-0.1.3/src/qubx/trackers/rebalancers.py` & `qubx-0.1.4/src/qubx/trackers/rebalancers.py`

 * *Files identical despite different names*

### Comparing `qubx-0.1.3/src/qubx/utils/_pyxreloader.py` & `qubx-0.1.4/src/qubx/utils/_pyxreloader.py`

 * *Files identical despite different names*

### Comparing `qubx-0.1.3/src/qubx/utils/charting/mpl_helpers.py` & `qubx-0.1.4/src/qubx/utils/charting/mpl_helpers.py`

 * *Files identical despite different names*

### Comparing `qubx-0.1.3/src/qubx/utils/marketdata/binance.py` & `qubx-0.1.4/src/qubx/utils/marketdata/binance.py`

 * *Files identical despite different names*

### Comparing `qubx-0.1.3/src/qubx/utils/misc.py` & `qubx-0.1.4/src/qubx/utils/misc.py`

 * *Files identical despite different names*

### Comparing `qubx-0.1.3/src/qubx/utils/pandas.py` & `qubx-0.1.4/src/qubx/utils/pandas.py`

 * *Files identical despite different names*

### Comparing `qubx-0.1.3/src/qubx/utils/runner.py` & `qubx-0.1.4/src/qubx/utils/runner.py`

 * *Files identical despite different names*

### Comparing `qubx-0.1.3/src/qubx/utils/time.py` & `qubx-0.1.4/src/qubx/utils/time.py`

 * *Files identical despite different names*

### Comparing `qubx-0.1.3/PKG-INFO` & `qubx-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Qubx
-Version: 0.1.3
+Version: 0.1.4
 Summary: Qubx - quantitative trading framework
 Home-page: https://github.com/dmarienko/Qubx
 Author: Dmitry Marienko
 Author-email: dmitry@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

