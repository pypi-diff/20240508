# Comparing `tmp/cron-converter-1.1.0.tar.gz` & `tmp/cron_converter-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cron-converter-1.1.0.tar", last modified: Sun Mar 24 21:48:01 2024, max compression
+gzip compressed data, was "cron_converter-1.2.0.tar", last modified: Wed May  8 21:50:26 2024, max compression
```

## Comparing `cron-converter-1.1.0.tar` & `cron_converter-1.2.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2024-03-24 21:48:01.449218 cron-converter-1.1.0/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1177 2023-04-09 20:40:39.000000 cron-converter-1.1.0/LICENSE
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     7827 2024-03-24 21:48:01.449218 cron-converter-1.1.0/PKG-INFO
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     7070 2024-03-24 21:21:40.000000 cron-converter-1.1.0/README.md
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2024-03-24 21:48:01.445218 cron-converter-1.1.0/cron_converter/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)       23 2023-04-09 20:40:39.000000 cron-converter-1.1.0/cron_converter/__init__.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     5068 2024-03-24 21:21:40.000000 cron-converter-1.1.0/cron_converter/cron.py
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2024-03-24 21:48:01.449218 cron-converter-1.1.0/cron_converter/sub_modules/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)    14926 2023-04-09 20:40:39.000000 cron-converter-1.1.0/cron_converter/sub_modules/part.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     8994 2023-04-09 21:08:32.000000 cron-converter-1.1.0/cron_converter/sub_modules/seeker.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      483 2023-04-09 20:40:39.000000 cron-converter-1.1.0/cron_converter/sub_modules/units.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      370 2024-03-24 21:21:40.000000 cron-converter-1.1.0/cron_converter/sub_modules/utils.py
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2024-03-24 21:48:01.449218 cron-converter-1.1.0/cron_converter.egg-info/
--rwxr-xr-x   0 andrea    (1000) andrea    (1000)     7827 2024-03-24 21:48:01.000000 cron-converter-1.1.0/cron_converter.egg-info/PKG-INFO
--rwxr-xr-x   0 andrea    (1000) andrea    (1000)      419 2024-03-24 21:48:01.000000 cron-converter-1.1.0/cron_converter.egg-info/SOURCES.txt
--rwxr-xr-x   0 andrea    (1000) andrea    (1000)        1 2024-03-24 21:48:01.000000 cron-converter-1.1.0/cron_converter.egg-info/dependency_links.txt
--rwxr-xr-x   0 andrea    (1000) andrea    (1000)       33 2024-03-24 21:48:01.000000 cron-converter-1.1.0/cron_converter.egg-info/requires.txt
--rwxr-xr-x   0 andrea    (1000) andrea    (1000)       42 2024-03-24 21:48:01.000000 cron-converter-1.1.0/cron_converter.egg-info/top_level.txt
--rw-rw-r--   0 andrea    (1000) andrea    (1000)       38 2024-03-24 21:48:01.449218 cron-converter-1.1.0/setup.cfg
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1074 2024-03-24 21:42:51.000000 cron-converter-1.1.0/setup.py
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2024-05-08 21:50:26.991606 cron_converter-1.2.0/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1177 2024-05-08 21:32:53.000000 cron_converter-1.2.0/LICENSE
+-rw-r--r--   0 andrea    (1000) andrea    (1000)     8116 2024-05-08 21:50:26.991606 cron_converter-1.2.0/PKG-INFO
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     7070 2024-03-24 21:21:40.000000 cron_converter-1.2.0/README.md
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2024-05-08 21:50:26.987606 cron_converter-1.2.0/cron_converter/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)       23 2023-04-09 20:40:39.000000 cron_converter-1.2.0/cron_converter/__init__.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     5016 2024-04-30 17:41:00.000000 cron_converter-1.2.0/cron_converter/cron.py
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2024-05-08 21:50:26.991606 cron_converter-1.2.0/cron_converter/sub_modules/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)    15195 2024-04-30 17:41:00.000000 cron_converter-1.2.0/cron_converter/sub_modules/part.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     8797 2024-05-08 21:31:16.000000 cron_converter-1.2.0/cron_converter/sub_modules/seeker.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      593 2024-04-30 17:41:00.000000 cron_converter-1.2.0/cron_converter/sub_modules/units.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      636 2024-04-30 17:41:00.000000 cron_converter-1.2.0/cron_converter/sub_modules/utils.py
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2024-05-08 21:50:26.991606 cron_converter-1.2.0/cron_converter.egg-info/
+-rw-r--r--   0 andrea    (1000) andrea    (1000)     8116 2024-05-08 21:50:26.000000 cron_converter-1.2.0/cron_converter.egg-info/PKG-INFO
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      415 2024-05-08 21:50:26.000000 cron_converter-1.2.0/cron_converter.egg-info/SOURCES.txt
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)        1 2024-05-08 21:50:26.000000 cron_converter-1.2.0/cron_converter.egg-info/dependency_links.txt
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)       75 2024-05-08 21:50:26.000000 cron_converter-1.2.0/cron_converter.egg-info/requires.txt
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)       15 2024-05-08 21:50:26.000000 cron_converter-1.2.0/cron_converter.egg-info/top_level.txt
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1243 2024-05-08 21:32:53.000000 cron_converter-1.2.0/pyproject.toml
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)       38 2024-05-08 21:50:26.991606 cron_converter-1.2.0/setup.cfg
```

### Comparing `cron-converter-1.1.0/LICENSE` & `cron_converter-1.2.0/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 MIT License
 
 Copyright (c) 2015-2022 Rouslan Placella (https://github.com/roccivic)
-Copyright (c) 2020-2022 Andrea Salvatori (https://github.com/Sonic0)
+Copyright (c) 2020-2024 Andrea Salvatori (https://github.com/Sonic0)
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `cron-converter-1.1.0/PKG-INFO` & `cron_converter-1.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 Metadata-Version: 2.1
 Name: cron-converter
-Version: 1.1.0
+Version: 1.2.0
 Summary: Cron string parser and scheduler for Python
-Home-page: https://github.com/Sonic0/cron-converter
-Author: Andrea Salvatori
-Author-email: andrea.salvatori92@gmail.com
-License: MIT License
-Keywords: cron
+Author-email: Andrea Salvatori <16443598+Sonic0@users.noreply.github.com>
+Project-URL: Homepage, https://github.com/Sonic0/cron-converter
+Project-URL: Issues, https://github.com/Sonic0/cron-converter/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: test
 License-File: LICENSE
+Requires-Dist: python-dateutil
+Provides-Extra: test
+Requires-Dist: python-dateutil; extra == "test"
+Provides-Extra: mypy
+Requires-Dist: mypy; extra == "mypy"
+Requires-Dist: types-python-dateutil; extra == "mypy"
 
 <p align="center">
   <img src="https://raw.githubusercontent.com/Sonic0/cron-converter/main/logo.png" title="Cron-converter">
 </p>
 
 Cron-converter provides a Cron string parser ( from string/lists to string/lists ) and iteration for the datetime object with a cron like format.<br>
 This project would be a transposition in Python of JS [cron-converter](https://github.com/roccivic/cron-converter) by [roccivic](https://github.com/roccivic).
```

### Comparing `cron-converter-1.1.0/README.md` & `cron_converter-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `cron-converter-1.1.0/cron_converter/cron.py` & `cron_converter-1.2.0/cron_converter/cron.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from datetime import datetime, date
+from datetime import date, datetime
 from functools import total_ordering
-from typing import Optional, List, Union
+from typing import List, Optional, Union
 
 from .sub_modules.part import Part
 from .sub_modules.seeker import Seeker
 from .sub_modules.units import units
 from .sub_modules.utils import to_parts
 
 
@@ -13,17 +13,17 @@
     """Creates an instance of Cron.
 
     Cron objects each represent a cron schedule.
 
     Attributes:
         options (dict): The options to use
     """
-    def __init__(self, cron_string: str = None, options=None):
+    def __init__(self, cron_string: Optional[str] = None, options=None):
         self.options = options if bool(options) else dict()
-        self.parts = None
+        self.parts: List[Part] = []
         if cron_string:
             self.from_string(cron_string)
 
     def __str__(self) -> str:
         """Print directly the Cron Object"""
         return self.to_string()
 
@@ -49,55 +49,49 @@
 
     def from_string(self, cron_string: str) -> None:
         """Parses a cron string (minutes - hours - days - months - weekday)
 
         :param cron_string: (str) The cron string to parse. It has to be made up 5 parts.
         :raises ValueError: Incorrect length of the cron string.
         """
-        if type(cron_string) != str:
+        if type(cron_string) is not str:
             raise TypeError('Invalid cron string')
-        self.parts = cron_string.strip().split()
-        if len(self.parts) != 5:
+        raw_cron_parts = cron_string.strip().split()
+        if len(raw_cron_parts) != 5:
             raise ValueError("Invalid cron string format")
-        cron_parts = []
-        for item, unit in zip(self.parts, units):
+        for item, unit in zip(raw_cron_parts, units):
             part = Part(unit, self.options)
             part.from_string(item)
-            cron_parts.append(part)
-
-        self.parts: List[Part] = cron_parts
+            self.parts.append(part)
 
     def to_string(self) -> str:
         """Return the cron schedule as a string.
 
         :return: cron string (str) -> The cron schedule as a string.
         """
         if not self.parts:
             raise LookupError('No schedule found')
         return ' '.join(str(part) for part in self.parts)
 
     def from_list(self, cron_list: List[List[Union[str, int]]]):
-        """Parses a 2-dimentional array of integers as a cron schedule.
+        """Parses a 2-dimensional array of integers as a cron schedule.
 
         :param cron_list: (list of list) The 2-dimensional list to parse.
         :raises ValueError: Incorrect length of the cron list.
         """
-        cron_parts = []
         if len(cron_list) != 5:
-            raise ValueError(f'Invalid cron list')
+            raise ValueError('Invalid cron list')
 
         for cron_part_list, unit in zip(cron_list, units):
             part = Part(unit, self.options)
             part.from_list(cron_part_list)
-            cron_parts.append(part)
-
-        self.parts = cron_parts
+            self.parts.append(part)
 
     def to_list(self) -> List[List[int]]:
-        """Returns the cron schedule as a 2-dimentional list of integers
+        """Returns the cron schedule as a 2-dimensional list of integers
 
         :return: schedule_list -> The cron schedule as a list.
         :raises LookupError: Empty Cron object.
         """
         if not self.parts:
             raise LookupError('No schedule found')
         schedule_list = []
@@ -106,15 +100,16 @@
         return schedule_list
 
     def schedule(self, start_date: Optional[datetime] = None, timezone_str: Optional[str] = None) -> Seeker:
         """Returns the time the schedule would run next.
 
         :param start_date: Optional. A datetime object. If not provided, date will be now in UTC.
                                      This param exclude 'timezone_str'.
-        :param timezone_str: Optional. A timezone str('Europe/Rome', 'America/New_York', ...). Date will be now, but localized.
+        :param timezone_str: Optional. A timezone str('Europe/Rome', 'America/New_York', ...).
+                                       Date will be now, but localized.
                                        If not provided, date will be now in UTC. This param exclude 'start_date'.
         :return: A schedule iterator.
         """
         return Seeker(self, start_date, timezone_str)
 
     def validate(self, date_time_obj: Union[datetime, date]) -> bool:
         """Returns True if the object passed is within the Cron rule.
```

### Comparing `cron-converter-1.1.0/cron_converter/sub_modules/part.py` & `cron_converter-1.2.0/cron_converter/sub_modules/part.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     Attributes:
         unit (dict): The unit of measurement of time (see units.py).
         options (dict): The options to use: output_weekday_names and output_month_names
     """
     def __init__(self, unit, options):
         self.options = options if bool(options) else dict()
         self.unit = unit
-        self.values = None
+        self.values: List[int] = []
 
     def __str__(self) -> str:
         """Print directly the Part Object"""
         return self.to_string()
 
     def __repr__(self):
         return f'{self.__class__.__name__} - (values:{self.values!r}, unit:{self.unit.get("name")!r})'
@@ -57,17 +57,17 @@
 
         if not values:
             raise ValueError('Empty interval value')
 
         sunday_fixed_values = self._fix_sunday(values)
         unique_values = list(dict.fromkeys(sunday_fixed_values))  # Remove eventual duplicates
         unique_values.sort()
-        part_value = self.out_of_range(unique_values)
-        if part_value is not None:
-            raise ValueError(f'Value {part_value!r} out of range for {self.unit.get("name")!r}')
+        out_of_range_value = self.out_of_range(unique_values)
+        if out_of_range_value is not None:
+            raise ValueError(f'Value {out_of_range_value!r} out of range for {self.unit.get("name")!r}')
 
         self.values = unique_values
 
     def from_string(self, cron_part: str) -> None:
         """Parses a string as a range of positive integers.
 
         :param cron_part: The string that represent a Part. It will be converted as a range.
@@ -77,32 +77,35 @@
         intervals_values_list = []  # Final list of list. Every sub-list will be a unit range
         # Split in the case of multiple unit ranges and replace months 'alt' with corresponding 'int' numbers
         string_parts = self._replace_alternatives(cron_part).split(',')
         for string_part in string_parts:
             # Split in the case of step parameter
             range_step_string_parts = string_part.split('/')
             if len(range_step_string_parts) > 2:
-                raise ValueError(f'Invalid value {string_part!r} in cron part {cron_part!r}')
+                raise ValueError(f"Invalid value {string_part!r} in cron part {cron_part!r}")
             range_string = range_step_string_parts[0]
             if not range_string:
-                raise ValueError(f'Invalid value {range_string}')
+                raise ValueError(f'Invalid value {string_part!r} for {self.unit.get("name")!r}')
             elif range_string == '*':
                 range_list = self.possible_values()
             else:
                 range_list = self._parse_range(range_string)
                 range_list = self._fix_sunday(range_list)
                 value = self.out_of_range(range_list)
                 if value is not None:
                     raise ValueError(f'Value {value!r} out of range for {self.unit.get("name")!r}')
             step = self._get_step(range_step_string_parts)
 
-            interval_values = self._apply_interval(range_list, step)  # filter by step
-            if not len(interval_values):
-                raise ValueError(f'Empty intervals value {cron_part}')
-            intervals_values_list.append(interval_values)
+            if step is not None:
+                interval_values = self._apply_interval(range_list, step)  # filter by step
+                if not len(interval_values):
+                    raise ValueError(f'Empty intervals value {cron_part}')
+                intervals_values_list.append(interval_values)
+            else:  # either no step value found or step value not valid
+                intervals_values_list.append(range_list)
 
         flattened_ranges_list = [item for sublist in intervals_values_list for item in sublist]
         flattened_ranges_list = list(dict.fromkeys(flattened_ranges_list))  # Remove eventual duplicates
         flattened_ranges_list.sort()
         self.values = flattened_ranges_list
 
     def _fix_sunday(self, values: List[int]) -> List[int]:
@@ -111,16 +114,15 @@
          :param values: The values to process.
          :returns: values -> The resulting array.
          """
         if self.unit.get('name') == 'weekday':
             values = [0 if value == 7 else value for value in values]
         return values
 
-    @staticmethod
-    def _parse_range(unit_range: str) -> List[int]:
+    def _parse_range(self, unit_range: str) -> List[int]:
         """Parses a range string. Example: input="15-19" output=[15, 16, 17, 18, 19]
 
         :param unit_range: The range string.
         :return: The resulting array.
         :raise ValueError: Impossible to convert the Part unit as int.
         :raise ValueError: Invalid min or max value for the Part unit.
         :raise ValueError: Not valid Range, max range is less than min range
@@ -135,35 +137,35 @@
         elif len(sub_parts) == 2:
             try:
                 min_value = int(sub_parts[0])
                 max_value = int(sub_parts[1])
             except ValueError as exc:
                 raise ValueError(f'Invalid min or max value from: {unit_range!r} --> {exc}')
             if max_value < min_value:
-                raise ValueError(f'Max range is less than min range in {unit_range}')
+                raise ValueError(f'Max range is less than min range in {unit_range!r} for {self.unit.get("name")!r}')
             return [int_value for int_value in range(min_value, max_value + 1)]
         else:
             raise ValueError(f'Invalid value {unit_range}')
 
     def _get_step(self, range_string_parts: List[str]) -> Union[None, int]:
         """Get the step part of the part string.
 
         :param range_string_parts: the part string of the current range.
         :return step: parsed step.
         :raise IndexError: The second index of the list does not exist. The step is not present.
         """
         try:
-            step = range_string_parts[1]
+            step_str = range_string_parts[1]
         except IndexError:
-            step = None
+            return None
 
-        if step or step == '':
-            step = self._parse_step(step)
+        if step_str or step_str == '':
+            return self._parse_step(step_str)
 
-        return step
+        return None
 
     def _parse_step(self, step: str) -> int:
         """Parses the step from a part string.
 
         :param step: The step string.
         :return: The step value.
         :raise ValueError: Invalid interval step value.
@@ -199,15 +201,15 @@
         if 'alt' in self.unit:
             string = string.upper()
             for idx, alt in enumerate(self.unit.get('alt')):
                 string = string.replace(alt, str(self.unit.get("min") + idx))
         return string
 
     def out_of_range(self, values: List[int]) -> Union[int, None]:
-        """Finds an element from values that is outside of the range of self.unit
+        """Finds an element from values that is outside the range of self.unit
 
         :param values: The values to test.
         :return: An integer is a value out of range was found, otherwise None.
         """
         first = values[0]
         last = values[-1]
         if first < self.unit.get('min'):
@@ -250,16 +252,15 @@
 
         :return: step between numbers in the interval whether array interval > 2.
         """
         if self.values and len(self.values) > 2:
             step = self.values[1] - self.values[0]
             if step > 1:
                 return step
-        else:
-            return None
+        return None
 
     def is_interval(self, step: int) -> bool:
         """Returns true if the range can be represented as an interval.
 
         :param step: The difference between numbers in the interval.
         """
         for idx, value in enumerate(self.values):
@@ -296,18 +297,18 @@
     def to_list(self) -> List[int]:
         """Returns the range as an array of positive integers.
 
         :return: The range as an array.
         """
         return self.values
 
-    def to_ranges(self) -> List[List[Union[str, int]]]:
+    def to_ranges(self) -> Union[List[int], List[List[Union[int]]]]:
         """Returns the range as an array of ranges defined as arrays of positive integers.
 
-        :return: multi_dim_values (list of list): The range as a multi-dimensional array.
+        :return: multi_dim_values (list of list): The range as a multidimensional array.
         """
         multi_dim_values = list()
         start_number = None
         for idx, value in enumerate(self.values):
             try:
                 next_value = self.values[idx + 1]
             except IndexError:
```

### Comparing `cron-converter-1.1.0/cron_converter/sub_modules/seeker.py` & `cron_converter-1.2.0/cron_converter/sub_modules/seeker.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,27 @@
-from datetime import datetime, timedelta, timezone
-from dateutil import tz
 import calendar
 import copy
-from typing import Optional
+from datetime import datetime, timedelta
+from typing import TYPE_CHECKING, List, Literal, Optional
+
+from dateutil import tz
 
-from typing import TYPE_CHECKING, List, Literal
+from .utils import iso_to_cron_weekday
 
 if TYPE_CHECKING:
     from cron import Cron
     from sub_modules.part import Part
 
 
-"""Converts ISO weekday numbers to cron weekday numbers.
-    ISO weekday numbers are Monday (1) to Sunday (7)
-    Cron weekday numbers are Sunday (0) to Saturday (6).
-"""
-def iso_to_cron_weekday(iso_weekday):
-    return iso_weekday % 7
-
 class Seeker:
     """Create an instance of Seeker. Seeker objects search for execution times of a cron schedule.
     Args:
         cron (object): Cron object
         start_date (datetime): The start date for the schedule iterator, with or without timezone.
-        timezone_str (str): The timezone to make an timezone aware datetime as response.
+        timezone_str (str): The timezone to make a timezone aware datetime as response.
     """
     def __init__(self, cron: 'Cron', start_date: Optional[datetime] = None, timezone_str: Optional[str] = None) -> None:
         if not cron.parts:
             raise LookupError('No schedule found')
 
         if start_date is not None and timezone_str is not None:
             raise ValueError('should have location_num or location_path, but not both')
@@ -44,55 +38,55 @@
                 self.tz_info = tz.gettz(timezone_str)
                 self.date = datetime.now(self.tz_info)
             else:
                 raise ValueError(f'Provided not a valid Timezone --> {timezone_str}')
         else:
             self.date = datetime.now(tz.tzutc())
 
-        if self.date.second > 0:
+        self.start_time = self.date
+        if self.date.second > 0 or self.date.microsecond > 0:
             # Add a minute to the date to prevent returning dates in the past
             self.date = self.date + timedelta(minutes=+1)
 
-        self.start_time = self.date
         self.cron = cron
         self.pristine = True
 
     """Resets the iterator."""
     def reset(self) -> None:
         self.pristine = True
         self.date = self.start_time
 
     """Returns the time the schedule would run next.
-    
+
      Returns:
         (datetime): The time the schedule would run next.
     """
     def next(self) -> datetime:
         if self.pristine:
             self.pristine = False
         else:
             one_minute = timedelta(minutes=+1)
             # Ensure next is never now
             self.date = self.date + one_minute
 
-        return self.find_date(getattr(self.cron, 'parts'))
+        return self.find_date(self.cron.parts)
 
     """Returns the time the schedule would have last run at.
-    
+
     Returns:
         (datetime): The time the schedule would have last run at.
     """
     def prev(self) -> datetime:
         self.pristine = False
         # Ensure prev and next cannot be same time
         self.date = self.date + timedelta(minutes=-1)
-        return self.find_date(getattr(self.cron, 'parts'), True)
+        return self.find_date(self.cron.parts, True)
 
     """Returns the time the schedule would run next. # TODO refactor description.
-    
+
     Args:
         cron_parts (List): List of all cron 'Part'.
         reverse(boolean): Whether to find the previous value instead of next.
     Returns:
         (datetime): A new datetime object. The date the schedule would have executed at.
     """
     def find_date(self, cron_parts: List['Part'], reverse: bool = False) -> datetime:
@@ -112,15 +106,15 @@
                         break
         else:
             raise Exception('Unable to find execution time for schedule')
 
         return copy.deepcopy(self.date.replace(second=0, microsecond=0))
 
     """Increments/decrements the month value of a date, until a month that matches the schedule is found.
-    
+
     Args:
         cron_month_part (Part): The month 'Part' object.
         operation (Literal['add', 'subtract']): The function to call on date: 'add' or 'subtract'.
     """
     def _shift_month(self, cron_month_part: 'Part', operation: Literal['add', 'subtract']) -> None:
         while self.date.month not in cron_month_part.to_list():
             self.date = self._calc_months(self.date, 1, operation)
@@ -129,15 +123,16 @@
 
     Args:
         cron_day_part (Part): The days 'Part' object.
         operation (Literal['add', 'subtract']): The function to call on date: 'add' or 'subtract'.
     Returns:
         (boolean): Whether the month of the date was changed.
     """
-    def _shift_day(self, cron_day_part: 'Part', cron_weekday_part: 'Part', operation: Literal['add', 'subtract']) -> bool:
+    def _shift_day(self, cron_day_part: 'Part', cron_weekday_part: 'Part', operation: Literal['add', 'subtract']) \
+            -> bool:
         current_month = self.date.month
         while self.date.day not in cron_day_part.to_list() or \
                 iso_to_cron_weekday(self.date.isoweekday()) not in cron_weekday_part.to_list():
             if operation == 'add':
                 self.date = self.date + timedelta(days=+1)
                 self.date = self.date.replace(hour=0, minute=0, second=0)
             else:
@@ -178,24 +173,24 @@
         (boolean): Whether the hour of the date was changed.
     """
     def _shift_minute(self, cron_minute_part: 'Part', operation: Literal['add', 'subtract']) -> bool:
         current_hour = self.date.hour
         while self.date.minute not in cron_minute_part.to_list():
             if operation == 'add':
                 self.date = self.date + timedelta(minutes=+1)
-                self.date = self.date.replace(second=0)
+                self.date = self.date.replace(second=0, microsecond=0)
             else:
                 self.date = self.date + timedelta(minutes=-1)
-                self.date = self.date.replace(second=59)
+                self.date = self.date.replace(second=59, microsecond=0)
             if current_hour != self.date.hour:
                 return True
         return False
 
     """Static method to increment/decrement the month value of a datetime Object.
-    
+
     Args:
         date (datetime): Date Object it increments/decrements the month value to.
         months (int): Number of months to add at the provided input date Object
         operation (Literal['add', 'subtract']): The function to call on date: 'add' or 'subtract'.
     Returns:
         (datetime): The input datetime object incremented or decremented.
     """
```

### Comparing `cron-converter-1.1.0/cron_converter.egg-info/PKG-INFO` & `cron_converter-1.2.0/cron_converter.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 Metadata-Version: 2.1
 Name: cron-converter
-Version: 1.1.0
+Version: 1.2.0
 Summary: Cron string parser and scheduler for Python
-Home-page: https://github.com/Sonic0/cron-converter
-Author: Andrea Salvatori
-Author-email: andrea.salvatori92@gmail.com
-License: MIT License
-Keywords: cron
+Author-email: Andrea Salvatori <16443598+Sonic0@users.noreply.github.com>
+Project-URL: Homepage, https://github.com/Sonic0/cron-converter
+Project-URL: Issues, https://github.com/Sonic0/cron-converter/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: test
 License-File: LICENSE
+Requires-Dist: python-dateutil
+Provides-Extra: test
+Requires-Dist: python-dateutil; extra == "test"
+Provides-Extra: mypy
+Requires-Dist: mypy; extra == "mypy"
+Requires-Dist: types-python-dateutil; extra == "mypy"
 
 <p align="center">
   <img src="https://raw.githubusercontent.com/Sonic0/cron-converter/main/logo.png" title="Cron-converter">
 </p>
 
 Cron-converter provides a Cron string parser ( from string/lists to string/lists ) and iteration for the datetime object with a cron like format.<br>
 This project would be a transposition in Python of JS [cron-converter](https://github.com/roccivic/cron-converter) by [roccivic](https://github.com/roccivic).
```

