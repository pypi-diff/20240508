# Comparing `tmp/exchange_calendars_extensions_api-0.3.0.tar.gz` & `tmp/exchange_calendars_extensions_api-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exchange_calendars_extensions_api-0.3.0.tar", max compression
+gzip compressed data, was "exchange_calendars_extensions_api-0.4.0.tar", max compression
```

## Comparing `exchange_calendars_extensions_api-0.3.0.tar` & `exchange_calendars_extensions_api-0.4.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11357 2024-02-12 14:06:37.273908 exchange_calendars_extensions_api-0.3.0/LICENSE
--rw-r--r--   0        0        0      761 2024-02-12 14:06:37.273908 exchange_calendars_extensions_api-0.3.0/README.md
--rw-r--r--   0        0        0      530 2024-02-12 14:06:37.273908 exchange_calendars_extensions_api-0.3.0/exchange_calendars_extensions/api/__init__.py
--rw-r--r--   0        0        0    16716 2024-02-12 14:06:37.273908 exchange_calendars_extensions_api-0.3.0/exchange_calendars_extensions/api/changes.py
--rw-r--r--   0        0        0       18 2024-02-12 14:06:49.037977 exchange_calendars_extensions_api-0.3.0/exchange_calendars_extensions/api/version.py
--rw-r--r--   0        0        0     2733 2024-02-12 14:06:48.969977 exchange_calendars_extensions_api-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     2083 1970-01-01 00:00:00.000000 exchange_calendars_extensions_api-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-08 14:21:37.825068 exchange_calendars_extensions_api-0.4.0/LICENSE
+-rw-r--r--   0        0        0      761 2024-05-08 14:21:37.825068 exchange_calendars_extensions_api-0.4.0/README.md
+-rw-r--r--   0        0        0      530 2024-05-08 14:21:37.825068 exchange_calendars_extensions_api-0.4.0/exchange_calendars_extensions/api/__init__.py
+-rw-r--r--   0        0        0    17849 2024-05-08 14:21:37.825068 exchange_calendars_extensions_api-0.4.0/exchange_calendars_extensions/api/changes.py
+-rw-r--r--   0        0        0       18 2024-05-08 14:21:50.113000 exchange_calendars_extensions_api-0.4.0/exchange_calendars_extensions/api/version.py
+-rw-r--r--   0        0        0     2719 2024-05-08 14:21:50.049000 exchange_calendars_extensions_api-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     2083 1970-01-01 00:00:00.000000 exchange_calendars_extensions_api-0.4.0/PKG-INFO
```

### Comparing `exchange_calendars_extensions_api-0.3.0/LICENSE` & `exchange_calendars_extensions_api-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `exchange_calendars_extensions_api-0.3.0/README.md` & `exchange_calendars_extensions_api-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `exchange_calendars_extensions_api-0.3.0/exchange_calendars_extensions/api/__init__.py` & `exchange_calendars_extensions_api-0.4.0/exchange_calendars_extensions/api/__init__.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars_extensions_api-0.3.0/exchange_calendars_extensions/api/changes.py` & `exchange_calendars_extensions_api-0.4.0/exchange_calendars_extensions/api/changes.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,24 @@
 import datetime as dt
 import functools
 from collections import OrderedDict
 from enum import Enum, unique
-from typing import List, Set, Tuple
+from typing import Union, Annotated, Callable
 
 import pandas as pd
 from pydantic import BaseModel, Field, RootModel, model_validator, validate_call
-from pydantic.functional_validators import BeforeValidator
-from typing_extensions import Literal, Union, Annotated, Dict, Any, Self, Callable, Concatenate, ParamSpec
+from pydantic.functional_validators import BeforeValidator, AfterValidator
+from typing_extensions import (
+    Literal,
+    Any,
+    Self,
+    Concatenate,
+    ParamSpec,
+    TypeVar,
+)
 
 
 @unique
 class DayType(str, Enum):
     """
     Enum for the different types of holidays and special sessions.
 
@@ -20,19 +27,20 @@
 
     HOLIDAY: A holiday.
     SPECIAL_OPEN: A special session with a special opening time.
     SPECIAL_CLOSE: A special session with a special closing time.
     MONTHLY_EXPIRY: A monthly expiry.
     QUARTERLY_EXPIRY: A quarterly expiry.
     """
-    HOLIDAY = 'holiday'
-    SPECIAL_OPEN = 'special_open'
-    SPECIAL_CLOSE = 'special_close'
-    MONTHLY_EXPIRY = 'monthly_expiry'
-    QUARTERLY_EXPIRY = 'quarterly_expiry'
+
+    HOLIDAY = "holiday"
+    SPECIAL_OPEN = "special_open"
+    SPECIAL_CLOSE = "special_close"
+    MONTHLY_EXPIRY = "monthly_expiry"
+    QUARTERLY_EXPIRY = "quarterly_expiry"
 
 
 def _to_timestamp(value: Any) -> pd.Timestamp:
     """
     Convert value to Pandas timestamp.
 
     Parameters
@@ -44,52 +52,86 @@
     -------
     pd.Timestamp
         The converted value.
 
     Raises
     ------
     ValueError
-        If the value cannot be converted to pd.Timestamp.
+        If the value cannot be converted to pd.Timestamp or converts to pd.NaT.
     """
     # Check if value is a valid timestamp.
     if not isinstance(value, pd.Timestamp):
         try:
             # Convert value to timestamp.
             # noinspection PyTypeChecker
             value = pd.Timestamp(value)
         except ValueError as e:
             # Failed to convert key to timestamp.
-            raise ValueError(f'Failed to convert {value} to {pd.Timestamp}.') from e
+            raise ValueError(
+                f'Failed to convert "{value}" of type {type(value)} to {pd.Timestamp}.'
+            ) from e
+        else:
+            if value is pd.NaT:
+                # Failed to convert key to timestamp.
+                raise ValueError(
+                    f'Failed to convert "{value}" of type {type(value)} to {pd.Timestamp}.'
+                )
+
     return value
 
 
+def _to_date(value: pd.Timestamp) -> pd.Timestamp:
+    """
+    Removes timezone information from the given Timestamp and normalizes to midnight.
+
+    Parameters
+    ----------
+    value : pd.Timestamp
+        The input timestamp from which timezone information is to be removed.
+
+    Returns
+    -------
+    pd.Timestamp
+        The timestamp normalized to midnight with timezone information removed.
+
+    """
+
+    # Remove timezone information and normalize to midnight.
+    return value.tz_localize(None).normalize()
+
+
 # A type alias for pd.Timestamp that allows initialisation from suitably formatted string values.
 TimestampLike = Annotated[pd.Timestamp, BeforeValidator(_to_timestamp)]
 
+# A type alias for TimestampLike that normalizes the timestamp to a date-like value.
+#
+# Date-like means that the timestamp is timezone-naive and normalized to the date boundary, i.e. midnight of the day it
+# represents. If the input converts to a valid pd.Timestamp, any timezone information, if present, is discarded. If the
+# result is not aligned with a date boundary, it is normalized to midnight of the same day.
+DateLike = Annotated[TimestampLike, AfterValidator(_to_date)]
+
 
-class AbstractDayProps(BaseModel, arbitrary_types_allowed=True, validate_assignment=True, extra='forbid'):
+class AbstractDayProps(
+    BaseModel, arbitrary_types_allowed=True, validate_assignment=True, extra="forbid"
+):
     """
     Abstract base class for special day properties.
     """
-    name: str  # The name of the day.
 
-
-# class AbstractDaySpec(AbstractDayProperties, arbitrary_types_allowed=True, validate_assignment=True, extra='forbid'):
-#     """
-#     Abstract base class for special day specification.
-#     """
-#     date: TimestampLike  # The date of the special day.
-#     name: str  # The name of the special day.
+    name: str  # The name of the day.
 
 
 class DayProps(AbstractDayProps):
     """
     Vanilla special day specification.
     """
-    type: Literal[DayType.HOLIDAY, DayType.MONTHLY_EXPIRY, DayType.QUARTERLY_EXPIRY]  # The type of the special day.
+
+    type: Literal[
+        DayType.HOLIDAY, DayType.MONTHLY_EXPIRY, DayType.QUARTERLY_EXPIRY
+    ]  # The type of the special day.
 
     def __str__(self):
         return f'{{type={self.type.name}, name="{self.name}"}}'
 
 
 def _to_time(value: Union[dt.time, str]):
     """
@@ -107,82 +149,92 @@
 
     Raises
     ------
     ValueError
         If the value cannot be converted to dt.time.
     """
     if not isinstance(value, dt.time):
-        for f in ('%H:%M', '%H:%M:%S'):
+        for f in ("%H:%M", "%H:%M:%S"):
             try:
                 # noinspection PyTypeChecker
                 value = dt.datetime.strptime(value, f).time()
                 break
             except ValueError:
                 pass
 
         if not isinstance(value, dt.time):
-            raise ValueError(f'Failed to convert {value} to {dt.time}.')
+            raise ValueError(f"Failed to convert {value} to {dt.time}.")
 
     return value
 
 
 # A type alias for dt.time that allows initialisation from suitably formatted string values.
 TimeLike = Annotated[dt.time, BeforeValidator(_to_time)]
 
 
 class DayPropsWithTime(AbstractDayProps):
     """
     Special day specification that requires a (open/close) time.
     """
-    type: Literal[DayType.SPECIAL_OPEN, DayType.SPECIAL_CLOSE]  # The type of the special day.
+
+    type: Literal[
+        DayType.SPECIAL_OPEN, DayType.SPECIAL_CLOSE
+    ]  # The type of the special day.
     time: TimeLike  # The open/close time of the special day.
 
     def __str__(self):
         return f'{{type={self.type.name}, name="{self.name}", time={self.time}}}'
 
 
 # Type alias for valid day properties.
-DayPropsLike = Annotated[Union[DayProps, DayPropsWithTime], Field(discriminator='type')]
+DayPropsLike = Annotated[Union[DayProps, DayPropsWithTime], Field(discriminator="type")]
 
-Tags = Union[List[str], Union[Tuple[str], Union[Set[str], None]]]
+Tags = Union[list[str], Union[tuple[str], Union[set[str], None]]]
 
 
-class DayMeta(BaseModel, arbitrary_types_allowed=True, validate_assignment=True, extra='forbid'):
+class DayMeta(
+    BaseModel, arbitrary_types_allowed=True, validate_assignment=True, extra="forbid"
+):
     """
     Metadata for a single date.
     """
 
     # Collection of tags.
     tags: Tags = []
 
     # Free-form comment.
     comment: Union[str, None] = None
 
-    @model_validator(mode='after')
-    def _canonicalize(self) -> 'DayMeta':
+    @model_validator(mode="after")
+    def _canonicalize(self) -> "DayMeta":
         # Sort tags alphabetically and remove duplicates.
-        self.__dict__['tags'] = sorted(set(self.tags or []))
+        self.__dict__["tags"] = sorted(set(self.tags or []))
 
         # Strip comment of whitespace and set to None if empty.
         if self.comment is not None:
-            self.__dict__['comment'] = self.comment.strip() or None
+            self.__dict__["comment"] = self.comment.strip() or None
 
         return self
 
     def __len__(self):
         return len(self.tags) + (1 if self.comment is not None else 0)
 
 
-P = ParamSpec('P')
+T_Self = TypeVar("S")
+P = ParamSpec("P")
 
 
-def _with_meta(f: Callable[Concatenate[Self, DayMeta, P], DayMeta]) -> Callable[Concatenate[Self, TimestampLike, P], Self]:
+def _with_meta(
+    f: Callable[Concatenate[T_Self, DayMeta, P], DayMeta],
+) -> Callable[Concatenate[T_Self, DateLike, P], T_Self]:
     @functools.wraps(f)
-    @validate_call(config={'arbitrary_types_allowed': True})
-    def wrapper(self, date: TimestampLike, *args: P.args, **kwargs: P.kwargs) -> Self:
+    @validate_call(config={"arbitrary_types_allowed": True})
+    def wrapper(
+        self: T_Self, date: DateLike, *args: P.args, **kwargs: P.kwargs
+    ) -> T_Self:
         # Retrieve meta for given day.
         meta = self.meta.get(date, DayMeta())
 
         # Call wrapped function with meta as first positional argument.
         meta = f(self, meta, *args, **kwargs)
 
         # Update meta for date.
@@ -193,15 +245,17 @@
 
         # Return self.
         return self
 
     return wrapper
 
 
-class ChangeSet(BaseModel, arbitrary_types_allowed=True, validate_assignment=True, extra='forbid'):
+class ChangeSet(
+    BaseModel, arbitrary_types_allowed=True, validate_assignment=True, extra="forbid"
+):
     """
     Represents a modification to an existing exchange calendar.
 
     A changeset consists of a set of dates to add and a set of dates to remove, respectively, for each of the following
     types of days:
     - holidays
     - special open
@@ -237,56 +291,59 @@
     To resolve this issue, the date 2020-01-01 could be added to the changeset, respectively, for all day types (except
     special opens) as a day to remove. Now, if the changeset is applied to the original calendar, 2020-01-01 will no
     longer be a holiday and therefore no longer conflict with the new special open day. This form of sanitization
     ensures that a consistent changeset can be applied safely to any exchange calendar. Effectively, normalization
     ensures that adding a new day for a given day type becomes an upsert operation, i.e. the day is added if it does not
     already exist in any day type category, and updated/moved to the new day type if it does.
     """
-    add: Dict[TimestampLike, DayPropsLike] = Field(default_factory=dict)
-    remove: List[TimestampLike] = Field(default_factory=list)
-    meta: Dict[TimestampLike, DayMeta] = Field(default_factory=dict)
 
-    @model_validator(mode='after')
-    def _canonicalize(self) -> 'ChangeSet':
+    add: dict[DateLike, DayPropsLike] = Field(default_factory=dict)
+    remove: list[DateLike] = Field(default_factory=list)
+    meta: dict[DateLike, DayMeta] = Field(default_factory=dict)
+
+    @model_validator(mode="after")
+    def _canonicalize(self) -> "ChangeSet":
         # Sort days to add by date.
         add = OrderedDict(sorted(self.add.items(), key=lambda i: i[0]))
 
         # Sort days to remove by date and remove duplicates.
         remove = sorted(set(self.remove))
 
         # Sort meta by date. Sort tag values and remove duplicates.
-        meta = OrderedDict([(k, v) for k, v in sorted(self.meta.items(), key=lambda i: i[0])])
-
-        self.__dict__['add'] = add
-        self.__dict__['remove'] = remove
-        self.__dict__['meta'] = meta
+        meta = OrderedDict(
+            [(k, v) for k, v in sorted(self.meta.items(), key=lambda i: i[0])]
+        )
+
+        self.__dict__["add"] = add
+        self.__dict__["remove"] = remove
+        self.__dict__["meta"] = meta
 
         return self
 
-    @validate_call(config={'arbitrary_types_allowed': True})
-    def add_day(self, date: TimestampLike, props: DayPropsLike) -> Self:
+    @validate_call(config={"arbitrary_types_allowed": True})
+    def add_day(self, date: DateLike, props: DayPropsLike) -> Self:
         """
         Add a day to the change set.
 
         Parameters
         ----------
-        date : TimestampLike
+        date : DateLike
             The day to add.
         props : Annotated[Union[DayProps, DayPropsWithTime], Field(discriminator='type')]
             The properties of the day to add.
 
         Returns
         -------
         ExchangeCalendarChangeSet : self
         """
 
         # Checks if day is already in the dictionary of days to add.
         if date in self.add:
             # Throw an exception.
-            raise ValueError(f'Day {date} already in days to add.')
+            raise ValueError(f"Day {date} already in days to add.")
 
         # Previous value.
         prev = self.add.get(date, None)
 
         # Add the day to the dictionary of days to add.
         self.add[date] = props
 
@@ -301,22 +358,22 @@
                 del self.add[date]
 
             # Let exception bubble up.
             raise e
 
         return self
 
-    @validate_call(config={'arbitrary_types_allowed': True})
-    def remove_day(self, date: TimestampLike) -> Self:
+    @validate_call(config={"arbitrary_types_allowed": True})
+    def remove_day(self, date: DateLike) -> Self:
         """
         Remove a day from the change set.
 
         Parameters
         ----------
-        date : TimestampLike
+        date : DateLike
             The date to remove.
 
         Returns
         -------
         ExchangeCalendarChangeSet : self
 
         Raises
@@ -335,15 +392,15 @@
 
             # Let exception bubble up.
             raise e
 
         return self
 
     @_with_meta
-    @validate_call(config={'arbitrary_types_allowed': True})
+    @validate_call(config={"arbitrary_types_allowed": True})
     def set_tags(self, meta: DayMeta, tags: Tags) -> DayMeta:
         """
         Set the tags of a given day.
 
         Parameters
         ----------
         meta : DayMeta
@@ -358,15 +415,15 @@
 
         # Set the tags.
         meta.tags = tags or []
 
         return meta
 
     @_with_meta
-    @validate_call(config={'arbitrary_types_allowed': True})
+    @validate_call(config={"arbitrary_types_allowed": True})
     def set_comment(self, meta: DayMeta, comment: Union[str, None]) -> DayMeta:
         """
         Set the comment for a given day.
 
         Parameters
         ----------
         meta : DayMeta
@@ -381,15 +438,15 @@
 
         # Set the tags.
         meta.comment = comment or None
 
         return meta
 
     @_with_meta
-    @validate_call(config={'arbitrary_types_allowed': True})
+    @validate_call(config={"arbitrary_types_allowed": True})
     def set_meta(self, meta: DayMeta, meta0: Union[DayMeta, None]) -> DayMeta:
         """
         Set the metadata for a given day.
 
         Parameters
         ----------
         meta : DayMeta
@@ -402,37 +459,37 @@
         ExchangeCalendarChangeSet : self
         """
 
         # Set the tags.
 
         return meta0
 
-    @validate_call(config={'arbitrary_types_allowed': True})
-    def clear_day(self, date: TimestampLike, include_meta: bool = False) -> Self:
+    @validate_call(config={"arbitrary_types_allowed": True})
+    def clear_day(self, date: DateLike, include_meta: bool = False) -> Self:
         """
         Clear a day from the change set.
 
         Parameters
         ----------
-        date : TimestampLike
-            The date to clear. Must be convertible to pandas.Timestamp.
+        date : DateLike
+            The date to clear.
         include_meta : bool
             Whether to also remove any metadata associated with the given date.
 
         Returns
         -------
         ExchangeCalendarChangeSet : self
         """
 
         # Avoid re-validation since this change cannot make the changeset inconsistent.
-        self.__dict__['add'].pop(date, None)
-        self.__dict__['remove'] = [x for x in self.remove if x != date]
+        self.__dict__["add"].pop(date, None)
+        self.__dict__["remove"] = [x for x in self.remove if x != date]
 
         if include_meta:
-            self.__dict__['meta'].pop(date, None)
+            self.__dict__["meta"].pop(date, None)
 
         return self
 
     def clear(self, include_meta: bool = False) -> Self:
         """
         Clear all changes.
 
@@ -456,17 +513,21 @@
     def __len__(self):
         return len(self.add) + len(self.remove) + len(self.meta)
 
     def __eq__(self, other):
         if not isinstance(other, ChangeSet):
             return False
 
-        return self.add == other.add and self.remove == other.remove and self.meta == other.meta
+        return (
+            self.add == other.add
+            and self.remove == other.remove
+            and self.meta == other.meta
+        )
 
-    def all_days(self, include_meta: bool = False) -> Tuple[pd.Timestamp, ...]:
+    def all_days(self, include_meta: bool = False) -> tuple[pd.Timestamp, ...]:
         """
         All unique dates contained in the changeset.
 
         This is the union of the dates to add and the dates to remove, with any duplicates removed.
 
         Parameters
         ----------
@@ -487,15 +548,15 @@
 
         # Return as sorted tuple.
         return tuple(sorted(dates))
 
 
 # A type alias for a dictionary of changesets, mapping exchange key to a corresponding change set.
 class ChangeSetDict(RootModel):
-    root: Dict[str, ChangeSet]
+    root: dict[str, ChangeSet]
 
     # Delegate all dictionary-typical methods to the root dictionary.
     def __getitem__(self, key):
         return self.root[key]
 
     def __setitem__(self, key, value):
         self.root[key] = value
```

### Comparing `exchange_calendars_extensions_api-0.3.0/pyproject.toml` & `exchange_calendars_extensions_api-0.4.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "exchange-calendars-extensions-api"
-version = "0.3.0"
+version = "0.4.0"
 description = "A package that defines parts of the API of the exchange-calendars-extensions package."
 license = "Apache-2.0"
 authors = ["Jens Keiner <jens.keiner@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/jenskeiner/exchange_calendars_extensions_api/"
 repository = "https://github.com/jenskeiner/exchange_calendars_extensions_api/"
 documentation = "https://github.com/jenskeiner/exchange_calendars_extensions_api/tree/main/docs/"
@@ -32,30 +32,22 @@
 [tool.poetry.dependencies]
 python = "~=3.9"
 typing-extensions = ">=4.0,<5"
 pydantic = ">=2,<3"
 pandas = "^2"
 
 [tool.poetry.group.dev.dependencies]
-pytest = ">=7.3.1,<8.1.0"
-pytest-cov = "~=4.1.0"
-pre-commit = ">=3.3.3,<3.7.0"
+pytest = ">=7.3.1,<8.3.0"
+pytest-cov = ">=4.1,<5.1"
+pre-commit = ">=3.3.3,<3.8.0"
 
 [tool.pytest.ini_options]
 addopts = "--cov=exchange_calendars_extensions.api --cov-report=term-missing"
 
 [tool.ruff]
-# Enable pycodestyle (`E`) and Pyflakes (`F`) codes by default.
-select = ["E", "F"]
-ignore = ["E501"]
-
-# Allow autofix for all enabled rules (when `--fix`) is provided.
-fixable = ["A", "B", "C", "D", "E", "F", "G", "I", "N", "Q", "S", "T", "W", "ANN", "ARG", "BLE", "COM", "DJ", "DTZ", "EM", "ERA", "EXE", "FBT", "ICN", "INP", "ISC", "NPY", "PD", "PGH", "PIE", "PL", "PT", "PTH", "PYI", "RET", "RSE", "RUF", "SIM", "SLF", "TCH", "TID", "TRY", "UP", "YTT"]
-unfixable = []
-
 # Exclude a variety of commonly ignored directories.
 exclude = [
     ".bzr",
     ".direnv",
     ".eggs",
     ".git",
     ".git-rewrite",
@@ -76,16 +68,27 @@
     "node_modules",
     "venv",
 ]
 
 # Same as Black.
 line-length = 88
 
+# Assume Python 3.9.
+target-version = "py39"
+
+
+[lint]
 # Allow unused variables when underscore-prefixed.
 dummy-variable-rgx = "^(_+|(_+[a-zA-Z0-9_]*[a-zA-Z0-9]+?))$"
 
-# Assume Python 3.9.
-target-version = "py39"
+fixable = ["A", "B", "C", "D", "E", "F", "G", "I", "N", "Q", "S", "T", "W", "ANN", "ARG", "BLE", "COM", "DJ", "DTZ", "EM", "ERA", "EXE", "FBT", "ICN", "INP", "ISC", "NPY", "PD", "PGH", "PIE", "PL", "PT", "PTH", "PYI", "RET", "RSE", "RUF", "SIM", "SLF", "TCH", "TID", "TRY", "UP", "YTT"]
+
+ignore = ["E501"]
+
+# Enable pycodestyle (`E`) and Pyflakes (`F`) codes by default.
+select = ["E", "F"]
+
+# Allow autofix for all enabled rules (when `--fix`) is provided.
+unfixable = []
 
-[tool.ruff.mccabe]
 # Unlike Flake8, default to a complexity level of 10.
-max-complexity = 10
+mccabe = 10
```

### Comparing `exchange_calendars_extensions_api-0.3.0/PKG-INFO` & `exchange_calendars_extensions_api-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exchange-calendars-extensions-api
-Version: 0.3.0
+Version: 0.4.0
 Summary: A package that defines parts of the API of the exchange-calendars-extensions package.
 Home-page: https://github.com/jenskeiner/exchange_calendars_extensions_api/
 License: Apache-2.0
 Keywords: keywords...
 Author: Jens Keiner
 Author-email: jens.keiner@gmail.com
 Requires-Python: >=3.9,<4.0
```

