# Comparing `tmp/work-1.1.0a3.tar.gz` & `tmp/work-1.1.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "work-1.1.0a3.tar", max compression
+gzip compressed data, was "work-1.1.0a4.tar", max compression
```

## Comparing `work-1.1.0a3.tar` & `work-1.1.0a4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1033 2022-08-29 19:21:01.200221 work-1.1.0a3/README.md
--rw-r--r--   0        0        0      594 2024-04-12 15:03:30.774646 work-1.1.0a3/pyproject.toml
--rw-r--r--   0        0        0    91340 2024-04-12 15:03:12.714508 work-1.1.0a3/src/work.py
--rw-r--r--   0        0        0        0 2021-02-24 12:12:04.352563 work-1.1.0a3/src/work_components/__init__.py
--rw-r--r--   0        0        0    24511 2024-04-10 11:59:44.154278 work-1.1.0a3/src/work_components/arguments.py
--rw-r--r--   0        0        0     2190 2024-04-12 15:03:29.658638 work-1.1.0a3/src/work_components/consts.py
--rw-r--r--   0        0        0    22097 2024-04-10 16:48:42.800523 work-1.1.0a3/src/work_components/container.py
--rw-r--r--   0        0        0        0 2022-08-23 18:01:16.135701 work-1.1.0a3/src/work_components/dao/__init__.py
--rw-r--r--   0        0        0    17192 2024-04-10 16:48:42.792523 work-1.1.0a3/src/work_components/dao/core.py
--rw-r--r--   0        0        0      270 2024-04-08 19:32:29.853389 work-1.1.0a3/src/work_components/dao/env.py
--rw-r--r--   0        0        0     1643 2024-04-08 19:32:29.853389 work-1.1.0a3/src/work_components/dao/flags.py
--rw-r--r--   0        0        0    11503 2024-04-08 19:32:29.853389 work-1.1.0a3/src/work_components/dao/rc.py
--rw-r--r--   0        0        0    11011 2024-04-08 18:05:30.527145 work-1.1.0a3/src/work_components/dao/recess.py
--rw-r--r--   0        0        0     6238 2024-04-10 16:48:42.780523 work-1.1.0a3/src/work_components/dt_parse.py
--rw-r--r--   0        0        0     4470 2024-04-08 18:05:30.527145 work-1.1.0a3/src/work_components/migrate.py
--rw-r--r--   0        0        0      320 2024-04-10 12:10:12.266685 work-1.1.0a3/src/work_components/protocols.py
--rw-r--r--   0        0        0     2650 2024-04-10 16:48:42.796523 work-1.1.0a3/src/work_components/timestamps.py
--rw-r--r--   0        0        0     8067 2024-04-08 18:05:30.527145 work-1.1.0a3/src/work_components/util.py
--rw-r--r--   0        0        0     1614 1970-01-01 00:00:00.000000 work-1.1.0a3/PKG-INFO
+-rw-r--r--   0        0        0     1033 2022-08-29 19:21:01.200221 work-1.1.0a4/README.md
+-rw-r--r--   0        0        0      594 2024-05-08 18:57:26.331745 work-1.1.0a4/pyproject.toml
+-rw-r--r--   0        0        0    92536 2024-05-08 18:57:26.327746 work-1.1.0a4/src/work.py
+-rw-r--r--   0        0        0        0 2021-02-24 12:12:04.352563 work-1.1.0a4/src/work_components/__init__.py
+-rw-r--r--   0        0        0    24509 2024-05-08 18:57:26.323745 work-1.1.0a4/src/work_components/arguments.py
+-rw-r--r--   0        0        0     2188 2024-05-08 18:57:26.331745 work-1.1.0a4/src/work_components/consts.py
+-rw-r--r--   0        0        0    22107 2024-05-08 18:57:26.327746 work-1.1.0a4/src/work_components/container.py
+-rw-r--r--   0        0        0        0 2022-08-23 18:01:16.135701 work-1.1.0a4/src/work_components/dao/__init__.py
+-rw-r--r--   0        0        0    17276 2024-05-08 18:57:26.323745 work-1.1.0a4/src/work_components/dao/core.py
+-rw-r--r--   0        0        0      268 2024-05-08 18:57:26.323745 work-1.1.0a4/src/work_components/dao/env.py
+-rw-r--r--   0        0        0     1641 2024-05-08 18:57:26.323745 work-1.1.0a4/src/work_components/dao/flags.py
+-rw-r--r--   0        0        0    11501 2024-05-08 18:57:26.323745 work-1.1.0a4/src/work_components/dao/rc.py
+-rw-r--r--   0        0        0    10484 2024-05-08 18:57:26.323745 work-1.1.0a4/src/work_components/dao/recess.py
+-rw-r--r--   0        0        0     6236 2024-05-08 18:57:26.323745 work-1.1.0a4/src/work_components/dt_parse.py
+-rw-r--r--   0        0        0     4470 2024-04-08 18:05:30.527145 work-1.1.0a4/src/work_components/migrate.py
+-rw-r--r--   0        0        0      320 2024-04-10 12:10:12.266685 work-1.1.0a4/src/work_components/protocols.py
+-rw-r--r--   0        0        0     2648 2024-05-08 18:57:26.323745 work-1.1.0a4/src/work_components/timestamps.py
+-rw-r--r--   0        0        0     8065 2024-05-08 18:57:26.323745 work-1.1.0a4/src/work_components/util.py
+-rw-r--r--   0        0        0     1614 1970-01-01 00:00:00.000000 work-1.1.0a4/PKG-INFO
```

### Comparing `work-1.1.0a3/README.md` & `work-1.1.0a4/README.md`

 * *Files identical despite different names*

### Comparing `work-1.1.0a3/pyproject.toml` & `work-1.1.0a4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "work"
-version = "1.1.0a3"
+version = "1.1.0a4"
 description = "Manual time tracking via a CLI that works similarly to git."
 authors = ["vauhochzett <vauhoch@zett.cc>"]
 readme = "README.md"
 homepage = "https://vauhoch.zett.cc/work/"
 packages = [
     { include = "work.py", from = "src" },
     { include = "work_components", from = "src" },
```

### Comparing `work-1.1.0a3/src/work.py` & `work-1.1.0a4/src/work.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 
-""" The work time log app tracks working hours in an interaction model similar to git. """
+"""The work time log app tracks working hours in an interaction model similar to git."""
 
 import csv
 import datetime as dt
 import os
 import pathlib
 import sys
 from collections import defaultdict, namedtuple
@@ -18,14 +18,15 @@
     List,
     Optional,
     Set,
     Tuple,
     cast,
 )
 
+import work_components.timestamps as ts
 from work_components import consts, dt_parse, migrate, util
 from work_components.arguments import (
     ADD_NAME,
     MAINTENANCE_NAMES,
     START_NAME,
     STOP_NAME,
     SWITCH_NAME,
@@ -46,16 +47,15 @@
     ShadowProtocolDay,
     sort_and_merge,
 )
 from work_components.dao import env
 from work_components.dao.core import WorkDao
 from work_components.dao.flags import Flags
 from work_components.dao.rc import RC
-from work_components.dao.recess import RecessDao
-import work_components.timestamps as ts
+from work_components.dao.recess import Holiday, RecessDao, ReducedHourDay, Vacation
 from work_components.util import Color, PrinTable
 
 __version__: str = consts.VERSION
 
 assert sys.version_info >= (3, 8)
 
 # Formats
@@ -729,25 +729,23 @@
                 # _timedelta_str() only allows positive arguments
                 time_str: str = self._timedelta_str(abs(delta_yesterday))
                 if delta_yesterday > 0:
                     output += Color.color(time_str + " undertime", Color.ORANGE)
                 elif delta_yesterday < 0:
                     output += Color.color(time_str + " overtime", Color.GREEN)
 
-        if not (associated_recess := self.recess_dao.get_recess_for(today)).empty:
-            names: List[str] = []
-            if associated_recess.vacation is not None:
-                names.append("vacation day")
-            if associated_recess.holiday is not None:
-                names.append("holiday")
-            if associated_recess.reduced_hour_day is not None:
-                names.append("reduced hour day")
+        if (associated_recess := self.recess_dao.get_recess_for(today)) is not None:
+            recess_name: str = {  # pyright: ignore[reportArgumentType]
+                Vacation: "vacation day",
+                Holiday: "holiday",
+                ReducedHourDay: "reduced hour day",
+            }[type(associated_recess)]
             output += new_section_line()
             output += (
-                f"Note: {(' + '.join(names)).capitalize()} "
+                f"Note: {recess_name.capitalize()} "
                 + f"({self._timedelta_str(minutes_expected)} expected)"
             )
 
         print(output)
 
     # hours #
 
@@ -1983,45 +1981,43 @@
 
     def recess(self, args) -> None:
         """Manage recess days, a.k.a. vacation days or holidays (add, remove, list)."""
 
         action: Optional[Callable] = None
         output: str = ""
 
-        # pylint: disable-msg=unnecessary-lambda-assignment
-
         if args.add_vacation:
             if len(args.add_vacation) not in [1, 2]:
                 raise ValueError("Expects either one or two arguments!")
             action, output = self._recess_add_vacation(args.add_vacation)
         elif args.add_holiday:
             holi_day: dt.date = dt_parse.resolve_day_argument(args.add_holiday)
-            action = lambda: self.recess_dao.add_holiday(date=holi_day)
+            action = lambda: self.recess_dao.add_holiday(date=holi_day)  # noqa: E731
             output = f"Added holiday on {holi_day.strftime(DATE_FORMAT)}"
         elif args.add_reduced_day:
             assert len(args.add_reduced_day) == 2
             redu_day: dt.date = dt_parse.resolve_day_argument(args.add_reduced_day[0])
             try:
                 hours: float = float(args.add_reduced_day[1])
             except ValueError as val_err:
                 raise ValueError(
                     f"Invalid value {args.add_reduced_day[1]} for HOURS; expects float."
                 ) from val_err
-            action = lambda: self.recess_dao.add_reduced_hour_day(
+            action = lambda: self.recess_dao.add_reduced_hour_day(  # noqa: E731
                 date=redu_day, hours=hours
             )
             output = (
                 f"Added reduced hour day on {redu_day.strftime(DATE_FORMAT)} "
                 f"with {hours} hours"
             )
         elif args.remove:
             remove_dates: List[dt.date] = [
                 dt_parse.resolve_day_argument(r) for r in args.remove
             ]
-            action = lambda: self.recess_dao.remove(dates=remove_dates)
+            action = lambda: self.recess_dao.remove(dates=remove_dates)  # noqa: E731
             output = (
                 f"Removed {', '.join([r.strftime(DATE_FORMAT) for r in remove_dates])}"
             )
 
         if action is None:
             # Default: List (even if no mode was selected)
             list_year = args.list or dt.date.today().year
@@ -2042,32 +2038,63 @@
 
         if first > last:
             raise InvalidOperationWarning.cant(
                 "add vacation", because="begin date lies after end date"
             )
 
         vacation_period: List[dt.date] = util.get_period(first, last)
-        free_days_in_period: List[dt.date] = [
-            day for day in vacation_period if self._is_free_day(day)
-        ]
-        if free_days_in_period:
+
+        days_to_remove: List[dt.date] = []
+        non_working_in_period: List[dt.date] = []
+        holidays_in_period: List[dt.date] = []
+
+        for day in vacation_period:
+            if self._is_non_working_day(day):
+                non_working_in_period.append(day)
+
+            its_recess = self.recess_dao.get_recess_for(day)
+            if isinstance(its_recess, ReducedHourDay):
+                return (
+                    lambda: None,
+                    "Selected period overlaps a reduced hour day. Did nothing.",
+                )
+            elif isinstance(its_recess, Holiday):
+                holidays_in_period.append(day)
+
+        if non_working_in_period:
             user_says: str = input(
                 "The vacation overlaps with configured non-working day(s): "
                 + ", ".join(
-                    [fdip.strftime("%d.%m.%Y (%A)") for fdip in free_days_in_period]
+                    [nwip.strftime("%d.%m.%Y (%A)") for nwip in non_working_in_period]
                 )
-                + "\nShould non-working days be removed from the vacation before it is added?\n"
-                + "[Y/n] "
+                + "\nShould non-working days be removed from the vacation before it "
+                + "is added?\n[Y/n] "
             )
             if user_says.lower().strip() != "n":
-                vacation_period = [
-                    day for day in vacation_period if day not in free_days_in_period
-                ]
-            if len(vacation_period) == 0:
-                return lambda: None, "No vacation days remained. Did nothing."
+                days_to_remove.extend(non_working_in_period)
+
+        if holidays_in_period:
+            user_says: str = input(
+                "The vacation overlaps with configured holiday(s): "
+                + ", ".join(
+                    [hdip.strftime("%d.%m.%Y (%A)") for hdip in holidays_in_period]
+                )
+                + "\nHolidays must be removed from the vacation before it can be "
+                + "added. Remove?\n[Y/n] "
+            )
+            # Free days cannot overlap, so we do nothing if the holidays are kept.
+            if user_says.lower().strip() == "n":
+                return lambda: None, "Selected period overlaps a holiday. Did nothing."
+
+            days_to_remove.extend(holidays_in_period)
+
+        # Remove non-working days and/or holidays if requested above
+        vacation_period = [day for day in vacation_period if day not in days_to_remove]
+        if len(vacation_period) == 0:
+            return lambda: None, "No vacation days remained. Did nothing."
 
         def action():
             self.recess_dao.add_vacation(period=vacation_period)
 
         if len(date_args) == 1:
             assert first == last
             return action, f"Added vacation on {first.strftime(DATE_FORMAT)}"
@@ -2275,15 +2302,15 @@
         """Return a list of minutes to work on a regular week.
 
         Does not consider recess days."""
         normal_hours: Collection[float] = self.configuration.expected_hours.values()
         assert len(normal_hours) == 7
         return [hour * 60.0 for hour in normal_hours]
 
-    def _is_free_day(self, day: dt.date) -> bool:
+    def _is_non_working_day(self, day: dt.date) -> bool:
         """Check if the given day is a free day, based only on the configured expected
         hours."""
         return self._expected_minutes()[day.weekday()] == 0
 
     def _minutes_per_days(self, days: List[dt.date]) -> List[Tuple[dt.date, float]]:
         """Return a list of the minutes to work on the given days. Considers recess days."""
```

### Comparing `work-1.1.0a3/src/work_components/arguments.py` & `work-1.1.0a4/src/work_components/arguments.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #!/usr/bin/env python3
-""" Argument names and the `Arguments` class. """
+"""Argument names and the `Arguments` class."""
 
 import argparse
 import datetime as dt
 import sys
 import textwrap
 from typing import Dict, List, Optional
```

### Comparing `work-1.1.0a3/src/work_components/consts.py` & `work-1.1.0a4/src/work_components/consts.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 #!/usr/bin/env python3
 
-""" Shared constants """
+"""Shared constants"""
 
 import os
 import pathlib
 from typing import List, Tuple
 
-VERSION: str = "1.1.0a3"
+VERSION: str = "1.1.0a4"
 RECORDS_VERSION: int = 3
 
 # Directories
 PARENT_DIR: pathlib.Path = pathlib.Path("~", ".local", "share").expanduser()
 DIRECTORY: pathlib.Path = PARENT_DIR.joinpath("work")
 DIRECTORY_DEBUG: pathlib.Path = PARENT_DIR.joinpath("debug", "work")
```

### Comparing `work-1.1.0a3/src/work_components/container.py` & `work-1.1.0a4/src/work_components/container.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 #!/usr/bin/env python3
 
-""" Protocol wrappers """
+"""Protocol wrappers"""
 
 import atexit
 import csv
 import datetime as dt
 import os
 import pathlib
 import re
 import shutil
 import tempfile
 from typing import Iterable, List, Optional
 
+import work_components.timestamps as ts
 from work_components import migrate, util
 from work_components.consts import (
     DATETIME_FORMAT,
     DAY_FILE_PATTERN,
     MONTH_DIR_PATTERN,
     PROTOCOL_FILE_EXTENSION,
     TIME_FORMAT,
     YEAR_DIR_PATTERN,
 )
-import work_components.timestamps as ts
 
 ### Record container classes ###
 
 
 class Record:
     """A protocol record. Invariant: start <= end"""
 
@@ -104,18 +104,17 @@
             end=max((self.end, other.end)),
             category=self.category,
             message=self.message,
         )
 
     def to_protocol_row(self) -> List[str]:
         """Create a row for a protocol file from this record."""
-        format_ = lambda d: d.strftime(DATETIME_FORMAT)
         return [
-            format_(self.start),
-            format_(self.end),
+            self.start.strftime(DATETIME_FORMAT),
+            self.end.strftime(DATETIME_FORMAT),
             self.category,
             self.message,
         ]
 
     def strftime(self, format_s: str) -> str:
         """Formatted start and end."""
         end_formatted: str = self.end.strftime(format_s)
@@ -168,17 +167,19 @@
 
         start: str
         end: str
         category: str
         message: str
         start, end, category, message = row
 
-        parse = lambda x: dt.datetime.strptime(x, DATETIME_FORMAT)
         return Record(
-            start=parse(start), end=parse(end), category=category, message=message
+            start=dt.datetime.strptime(start, DATETIME_FORMAT),
+            end=dt.datetime.strptime(end, DATETIME_FORMAT),
+            category=category,
+            message=message,
         )
 
     @staticmethod
     def one_minute_record(start: dt.datetime):
         """Create a `Record` with the given `start` and a length of one minute."""
         return Record(start, start + dt.timedelta(minutes=1))
```

### Comparing `work-1.1.0a3/src/work_components/dao/core.py` & `work-1.1.0a4/src/work_components/dao/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 #!/usr/bin/env python3
 
-""" The DAO for the work module. """
+"""The DAO for the work module."""
 
 import datetime as dt
 import json
 import pathlib
 import zlib
 from types import SimpleNamespace
 from typing import Dict, List, Optional, Tuple
 
+import work_components.timestamps as ts
 from work_components import migrate
 from work_components.consts import (
     DATETIME_FORMAT,
     INFO_FILE_NAME,
     PROTOCOL_DIRECTORY_NAME,
     RECORDS_VERSION,
     RUN_FILE_NAME,
@@ -21,15 +22,14 @@
 from work_components.container import (
     Protocol,
     ProtocolDay,
     ProtocolMeta,
     ProtocolRange,
     Record,
 )
-import work_components.timestamps as ts
 
 
 class WorkDao:
     """DAO for the work directory and its children."""
 
     # work_directory        self.work_directory
     # |- info.winf          self.info_file
@@ -111,15 +111,15 @@
 
         self.add_protocol_entry(start_time, end_time, category, message, force)
         self.run_file.unlink()
 
     def invalid_start_and_end_error(
         self, start_time: dt.datetime, end_time: dt.datetime
     ) -> Optional[str]:
-
+        """Returns an error message if the combination of start and end is invalid."""
         if end_time <= start_time:
             return "end time must be after start time"
 
         # Ensure that start and end lie at most one calendar day apart.
         if end_time.date() not in [sd := start_time.date(), sd + dt.timedelta(days=1)]:
             return "a run end may not lie more than one calendar day after its start"
```

### Comparing `work-1.1.0a3/src/work_components/dao/flags.py` & `work-1.1.0a4/src/work_components/dao/flags.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-""" The DAO for the flags file. """
+"""The DAO for the flags file."""
 
 import json
 import pathlib
 from typing import List
 
 
 class Flags:
```

### Comparing `work-1.1.0a3/src/work_components/dao/rc.py` & `work-1.1.0a4/src/work_components/dao/rc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3
 
 # pylint: disable-msg=invalid-name
 
-""" The DAO for the runtime configuration file. """
+"""The DAO for the runtime configuration file."""
 
 import json
 from collections import ChainMap
 from typing import IO, Any, Callable, Dict, List, Mapping, MutableMapping, Optional
 
 from work_components import consts, migrate, util
 from work_components.arguments import MODES
```

### Comparing `work-1.1.0a3/src/work_components/dao/recess.py` & `work-1.1.0a4/src/work_components/dao/recess.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 
-""" The DAO for the recess files. """
+"""The DAO for the recess files."""
 
 import datetime as dt
 import json
 from collections import defaultdict
 from dataclasses import dataclass
 from itertools import chain
 from pathlib import Path
@@ -78,28 +78,14 @@
     hours: float = 0
 
     def __init__(self, date: dt.date, hours: float):
         super().__init__(date=date)
         self.hours = hours
 
 
-@dataclass
-class AssociatedRecess:
-    """Container to carry the associated recess day(s) for a date."""
-
-    holiday: Optional[Holiday] = None
-    vacation: Optional[Vacation] = None
-    reduced_hour_day: Optional[ReducedHourDay] = None
-
-    @property
-    def empty(self):
-        """Return if instance is empty, meaning no recess day is recorded."""
-        return self == AssociatedRecess()
-
-
 class ExistsError(Exception):
     """Exception that denotes that a recess day exists already."""
 
 
 class RecessFile:
     """Writes to file on update. Creates directory and file if nonexistent."""
 
@@ -140,22 +126,27 @@
             for redu_day, hours in vf_json[RecessFile.reduceds_k].items()
         ]
         self.vacations = [
             Vacation(date=dt.datetime.strptime(vaca_day, DATE_FORMAT).date())
             for vaca_day in vf_json[RecessFile.vacations_k]
         ]
 
+    @property
+    def recess(self) -> Iterable[Recess]:
+        """Iterate over stored recess containers of any type."""
+        yield from chain(self.holidays, self.reduced_hour_days, self.vacations)
+
     def add_any(self, container: List, add_us: List):
         """Add any type of recess day."""
         if container and add_us:
             assert isinstance(add_us[0], type(container[0]))
 
         if exist := [
             rec.date
-            for rec in chain(self.holidays, self.reduced_hour_days, self.vacations)
+            for rec in self.recess
             if rec.date in list(map(lambda obj: obj.date, add_us))
         ]:
             raise ExistsError(
                 "Free day(s) already stored: "
                 f"{', '.join([e_date.strftime('%d.%m.%Y') for e_date in exist])}"
             )
         container.extend(add_us)
@@ -271,42 +262,36 @@
             r_file.add_any(r_file.vacations, vacations_by_year[year])
 
     def remove(self, dates: List[dt.date]) -> None:
         """Remove recess day(s). If any date is present in more than one list, raises."""
         for date in dates:
             self._get(year=date.year).remove(date=date)
 
-    def get_recess_for(self, date: dt.date) -> AssociatedRecess:
-        """Return all associated recess objects for the given date."""
-        associated_recess = AssociatedRecess()
+    def get_recess_for(self, date: dt.date) -> Optional[Recess]:
+        """Return the associated recess for the given date if it exists."""
         r_file: RecessFile = self._get(year=date.year)
 
-        its_rhds = list(filter(lambda d: d.date == date, r_file.reduced_hour_days))
-        if len(its_rhds) > 1:
-            raise ExistsError(f"Multiple reduced days found for {date}")
-
-        if len(its_rhds) == 1:
-            associated_recess.reduced_hour_day = its_rhds[0]
-
-        if (holiday := Holiday(date=date)) in r_file.holidays:
-            associated_recess.holiday = holiday
-        if (vacation := Vacation(date=date)) in r_file.vacations:
-            associated_recess.vacation = vacation
-        return associated_recess
+        its_recess: List[Recess] = [day for day in r_file.recess if day.date == date]
+
+        # We assume that each day can have at most one associated recess.
+        if len(its_recess) > 1:
+            raise ExistsError(f"Multiple free days found for {date}")
+
+        return its_recess[0] if its_recess else None
 
     def reduced_hours(self, date: dt.date) -> Optional[float]:
         """
         Get the reduced hours for a given date. The lowest value is returned, that
         means if a date is added as reduced_hour_day with 2 hours and as a vacation,
         0 is returned.
 
         Returns None if hours are not reduced on the given day.
         """
-        associated_recess: AssociatedRecess = self.get_recess_for(date)
-        if associated_recess.empty:
+        associated_recess: Optional[Recess] = self.get_recess_for(date)
+        if associated_recess is None:
             return None
 
-        if associated_recess.reduced_hour_day is not None:
-            return associated_recess.reduced_hour_day.hours
+        if isinstance(associated_recess, ReducedHourDay):
+            return associated_recess.hours
 
         # Has holiday or vacation
         return 0
```

### Comparing `work-1.1.0a3/src/work_components/dt_parse.py` & `work-1.1.0a4/src/work_components/dt_parse.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #!/usr/bin/env python3
-""" Smart date/time parsing """
+"""Smart date/time parsing"""
 
 import datetime as dt
 import re
 from enum import Enum
 from typing import List, Optional, Tuple
 
 from work_components import util
```

### Comparing `work-1.1.0a3/src/work_components/migrate.py` & `work-1.1.0a4/src/work_components/migrate.py`

 * *Files identical despite different names*

### Comparing `work-1.1.0a3/src/work_components/timestamps.py` & `work-1.1.0a4/src/work_components/timestamps.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-""" API wrapper and extension for datetime """
+"""API wrapper and extension for datetime"""
 
 from dataclasses import dataclass
 import datetime as dt
 from typing import Set
 
 
 def date_equals(left: dt.date, right: dt.date) -> bool:
```

### Comparing `work-1.1.0a3/src/work_components/util.py` & `work-1.1.0a4/src/work_components/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 
-""" Utils for the work module. """
+"""Utils for the work module."""
 
 import datetime as dt
 import re
 import textwrap
 from collections import Counter
 from fnmatch import fnmatch
 from typing import Dict, List, Optional
```

### Comparing `work-1.1.0a3/PKG-INFO` & `work-1.1.0a4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: work
-Version: 1.1.0a3
+Version: 1.1.0a4
 Summary: Manual time tracking via a CLI that works similarly to git.
 Home-page: https://vauhoch.zett.cc/work/
 Author: vauhochzett
 Author-email: vauhoch@zett.cc
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

