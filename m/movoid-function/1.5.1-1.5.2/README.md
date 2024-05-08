# Comparing `tmp/movoid_function-1.5.1.tar.gz` & `tmp/movoid_function-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "movoid_function-1.5.1.tar", last modified: Tue May  7 14:03:27 2024, max compression
+gzip compressed data, was "movoid_function-1.5.2.tar", last modified: Wed May  8 14:57:40 2024, max compression
```

## Comparing `movoid_function-1.5.1.tar` & `movoid_function-1.5.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 14:03:27.165840 movoid_function-1.5.1/
--rw-rw-rw-   0        0        0       10 2024-04-24 13:42:41.000000 movoid_function-1.5.1/MANIFEST.in
--rw-rw-rw-   0        0        0      213 2024-05-07 14:03:27.164842 movoid_function-1.5.1/PKG-INFO
--rw-rw-rw-   0        0        0       44 2024-01-07 14:19:32.000000 movoid_function-1.5.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-07 14:03:27.157673 movoid_function-1.5.1/movoid_function/
--rw-rw-rw-   0        0        0      562 2024-04-13 09:15:08.000000 movoid_function-1.5.1/movoid_function/__init__.py
--rw-rw-rw-   0        0        0     9812 2024-02-20 05:59:20.000000 movoid_function-1.5.1/movoid_function/check.py
--rw-rw-rw-   0        0        0    16565 2024-02-20 11:49:02.000000 movoid_function-1.5.1/movoid_function/decorator.py
--rw-rw-rw-   0        0        0     1557 2024-04-14 08:03:48.000000 movoid_function-1.5.1/movoid_function/function.py
--rw-rw-rw-   0        0        0    13000 2024-05-07 13:18:50.000000 movoid_function-1.5.1/movoid_function/type.py
-drwxrwxrwx   0        0        0        0 2024-05-07 14:03:27.163750 movoid_function-1.5.1/movoid_function.egg-info/
--rw-rw-rw-   0        0        0      213 2024-05-07 14:03:27.000000 movoid_function-1.5.1/movoid_function.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      320 2024-05-07 14:03:27.000000 movoid_function-1.5.1/movoid_function.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 14:03:27.000000 movoid_function-1.5.1/movoid_function.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-05-07 14:03:27.000000 movoid_function-1.5.1/movoid_function.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-07 14:03:27.165840 movoid_function-1.5.1/setup.cfg
--rw-rw-rw-   0        0        0      462 2024-05-07 14:02:58.000000 movoid_function-1.5.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 14:57:40.019929 movoid_function-1.5.2/
+-rw-rw-rw-   0        0        0       10 2024-04-24 13:42:41.000000 movoid_function-1.5.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      213 2024-05-08 14:57:40.017925 movoid_function-1.5.2/PKG-INFO
+-rw-rw-rw-   0        0        0       44 2024-01-07 14:19:32.000000 movoid_function-1.5.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-08 14:57:40.002968 movoid_function-1.5.2/movoid_function/
+-rw-rw-rw-   0        0        0      562 2024-04-13 09:15:08.000000 movoid_function-1.5.2/movoid_function/__init__.py
+-rw-rw-rw-   0        0        0     9920 2024-05-08 14:50:45.000000 movoid_function-1.5.2/movoid_function/check.py
+-rw-rw-rw-   0        0        0    16565 2024-02-20 11:49:02.000000 movoid_function-1.5.2/movoid_function/decorator.py
+-rw-rw-rw-   0        0        0     1557 2024-04-14 08:03:48.000000 movoid_function-1.5.2/movoid_function/function.py
+-rw-rw-rw-   0        0        0    16245 2024-05-08 14:50:45.000000 movoid_function-1.5.2/movoid_function/type.py
+drwxrwxrwx   0        0        0        0 2024-05-08 14:57:40.009339 movoid_function-1.5.2/movoid_function.egg-info/
+-rw-rw-rw-   0        0        0      213 2024-05-08 14:57:39.000000 movoid_function-1.5.2/movoid_function.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      320 2024-05-08 14:57:39.000000 movoid_function-1.5.2/movoid_function.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 14:57:39.000000 movoid_function-1.5.2/movoid_function.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-05-08 14:57:39.000000 movoid_function-1.5.2/movoid_function.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-08 14:57:40.019929 movoid_function-1.5.2/setup.cfg
+-rw-rw-rw-   0        0        0      462 2024-05-08 14:56:50.000000 movoid_function-1.5.2/setup.py
```

### Comparing `movoid_function-1.5.1/movoid_function/__init__.py` & `movoid_function-1.5.2/movoid_function/__init__.py`

 * *Files identical despite different names*

### Comparing `movoid_function-1.5.1/movoid_function/check.py` & `movoid_function-1.5.2/movoid_function/check.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,14 +119,18 @@
         self._list_formula = self._analyse_list(self._str_formula)
         self._now_formula = []
         self._result = None
 
     def __repr__(self):
         return f'CheckFormula({self._str_formula},{self._check_class.__name__})'
 
+    @property
+    def formula(self):
+        return self._str_formula
+
     def _analyse_list(self, str_formula) -> list:
         re_list = []
         child = False
         bracket = 0
         now_str = ''
         for i, v in enumerate(str_formula):
             if child:
@@ -251,19 +255,19 @@
             i += 1
         if len(list_formula) == 1 and isinstance(list_formula[0], bool):
             return list_formula[0]
         else:
             raise ValueError(f'{list_formula} can not be calculate anymore')
 
     def show_all_step(self):
-        print(self._str_formula)
-        print(self._list_formula)
+        re_str = self._str_formula + '\n' + str(self._list_formula)
         for i, v in enumerate(self._calculate_step):
-            print(f'={v}')
+            re_str += f'\n={v}'
         if self._result is not None:
-            print(f'={self._result}')
+            re_str += f'\n={self._result}'
+        return re_str
 
     def _record_one_step(self, replace=False):
         if replace:
             self._calculate_step[-1] = deepcopy(self._now_formula)
         else:
             self._calculate_step.append(deepcopy(self._now_formula))
```

### Comparing `movoid_function-1.5.1/movoid_function/decorator.py` & `movoid_function-1.5.2/movoid_function/decorator.py`

 * *Files identical despite different names*

### Comparing `movoid_function-1.5.1/movoid_function/function.py` & `movoid_function-1.5.2/movoid_function/function.py`

 * *Files identical despite different names*

### Comparing `movoid_function-1.5.1/movoid_function/type.py` & `movoid_function-1.5.2/movoid_function/type.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,323 +3,361 @@
 """
 # File          : type
 # Author        : Sun YiFan-Movoid
 # Time          : 2024/1/30 22:45
 # Description   : 
 """
 
-import json
 import pathlib
 import re
+import traceback
+import typing
 from abc import ABC, abstractmethod
-from typing import Union, Any
 
 from .check import NumberCheck, CheckFormula
 from .decorator import recover_signature_from_function_func
 
 
 class Type(ABC):
     def __init__(self, convert=False, **kwargs):
         self._convert = bool(convert)
 
     @abstractmethod
     def __repr__(self):
         pass
 
     @abstractmethod
-    def check(self, check_target, convert=None) -> bool:
+    def convert_function(self, check_target) -> object:
         pass
 
     @abstractmethod
-    def _convert_function(self, check_target):
+    def check_function(self, check_target) -> typing.List[str]:
         pass
 
+    def check(self, check_target, convert=None):
+        try:
+            check_value = self.convert(check_target, convert)
+        except:
+            re_bool = False
+            re_value = f'convert failed:\n{traceback.format_exc()}'
+        else:
+            fail_str = self.check_function(check_value)
+            re_bool = len(fail_str) == 0
+            re_value = check_value if re_bool else fail_str
+        return re_bool, re_value
+
     def convert(self, convert_target, convert=None):
         should_convert = self._convert if convert is None else bool(convert)
         if should_convert:
-            re_value = self._convert_function(convert_target)
+            re_value = self.convert_function(convert_target)
         else:
             re_value = convert_target
         return re_value
 
     @property
     def annotation(self):
-        return Any
+        return typing.Any
 
 
 class Bool(Type):
     def __init__(self, convert=False, **kwargs):
         super().__init__(convert=convert, **kwargs)
 
     def __repr__(self):
         return f'Bool(convert={self._convert})'
 
-    def check(self, check_target, convert=None) -> bool:
-        check_target = self.convert(check_target, convert)
-        return isinstance(check_target, bool)
+    def convert_function(self, check_target) -> bool:
+        if isinstance(check_target, str):
+            if check_target.lower() in ('true', 'yes'):
+                re_value = True
+            elif check_target.lower() in ('false', 'no'):
+                re_value = False
+            else:
+                raise ValueError(f'we do not know what is <{check_target}> for bool.')
+        else:
+            re_value = bool(check_target)
+        return re_value
 
-    def _convert_function(self, check_target) -> bool:
-        return bool(check_target)
+    def check_function(self, check_target) -> typing.List[str]:
+        fail_str: typing.List[str] = []
+        if not isinstance(check_target, bool):
+            fail_str.append(f'{check_target} is {type(check_target).__name__} not bool')
+        return fail_str
 
     @property
     def annotation(self):
         if self._convert:
-            return Any
+            return typing.Any
         else:
             return bool
 
 
 class Int(Type):
     def __init__(self, limit='', convert=False, **kwargs):
         super().__init__(convert=convert, **kwargs)
         self._limit = CheckFormula(limit, NumberCheck)
 
     def __repr__(self):
-        limit_text = f'limit={self._limit}, ' if self._limit._str_formula else ''
+        limit_text = f'limit={self._limit}, ' if self._limit.formula else ''
         return f'Int({limit_text}convert={self._convert})'
 
-    def check(self, check_target, convert=None) -> bool:
-        check_target = self.convert(check_target, convert)
+    def convert_function(self, check_target) -> int:
+        return int(check_target)
+
+    def check_function(self, check_target) -> typing.List[str]:
+        fail_str: typing.List[str] = []
         if isinstance(check_target, int):
-            re_bool = self._limit.check(check_target)
+            if not self._limit.check(check_target):
+                fail_str.append(f'{check_target} did not match: {self._limit.show_all_step()}')
         else:
-            re_bool = False
-        return re_bool
-
-    def _convert_function(self, check_target) -> int:
-        return int(check_target)
+            fail_str.append(f'{check_target} is {type(check_target).__name__} not int')
+        return fail_str
 
     @property
     def annotation(self):
         if self._convert:
-            return Union[int, str]
+            return typing.Union[int, str]
         else:
             return int
 
 
 class Float(Type):
     def __init__(self, limit='', convert=False, **kwargs):
         super().__init__(convert=convert, **kwargs)
         self._limit = CheckFormula(limit, NumberCheck)
 
     def __repr__(self):
-        limit_text = f'limit={self._limit}, ' if self._limit._str_formula else ''
+        limit_text = f'limit={self._limit}, ' if self._limit.formula else ''
         return f'Float({limit_text}convert={self._convert})'
 
-    def check(self, check_target, convert=None) -> bool:
-        check_target = self.convert(check_target, convert)
+    def convert_function(self, check_target) -> float:
+        return float(check_target)
+
+    def check_function(self, check_target) -> typing.List[str]:
+        fail_str: typing.List[str] = []
         if isinstance(check_target, float):
-            re_bool = self._limit.check(check_target)
+            if not self._limit.check(check_target):
+                fail_str.append(f'{check_target} did not match: {self._limit.show_all_step()}')
         else:
-            re_bool = False
-        return re_bool
-
-    def _convert_function(self, check_target) -> float:
-        return float(check_target)
+            fail_str.append(f'{check_target} is {type(check_target).__name__} not float')
+        return fail_str
 
     @property
     def annotation(self):
         if self._convert:
-            return Union[float, str]
+            return typing.Union[float, str]
         else:
             return float
 
 
 class Number(Type):
     def __init__(self, limit='', convert=False, **kwargs):
         super().__init__(convert=convert, **kwargs)
         self._limit = CheckFormula(limit, NumberCheck)
 
     def __repr__(self):
-        limit_text = f'limit={self._limit}, ' if self._limit._str_formula else ''
+        limit_text = f'limit={self._limit}, ' if self._limit.formula else ''
         return f'Number({limit_text}convert={self._convert})'
 
-    def check(self, check_target, convert=None) -> bool:
-        check_target = self.convert(check_target, convert)
-        if isinstance(check_target, float) or isinstance(check_target, int):
-            re_bool = self._limit.check(check_target)
-        else:
-            re_bool = False
-        return re_bool
-
-    def _convert_function(self, check_target) -> Union[int, float]:
+    def convert_function(self, check_target) -> typing.Union[int, float]:
         temp = float(check_target)
         if float(int(temp)) == temp:
             return int(temp)
         else:
             return temp
 
+    def check_function(self, check_target) -> typing.List[str]:
+        fail_str: typing.List[str] = []
+        if isinstance(check_target, (int, float)):
+            if not self._limit.check(check_target):
+                fail_str.append(f'{check_target} did not match: {self._limit.show_all_step()}')
+        else:
+            fail_str.append(f'{check_target} is {type(check_target).__name__} not number')
+        return fail_str
+
     @property
     def annotation(self):
         if self._convert:
-            return Union[int, float, str]
+            return typing.Union[int, float, str]
         else:
-            return Union[int, float]
+            return typing.Union[int, float]
 
 
 class Str(Type):
     def __init__(self, char=None, length='', regex=None, convert=False, **kwargs):
         super().__init__(convert=convert, **kwargs)
         self._char = char
         self._length = CheckFormula(length, NumberCheck)
         self._regex = regex
 
     def __repr__(self):
         char_text = f'char={self._char}, ' if self._char else ''
-        limit_text = f'length={self._length}, ' if self._length._str_formula else ''
+        limit_text = f'length={self._length}, ' if self._length.formula else ''
         regex_text = f'regex={self._regex}, ' if self._regex else ''
         return f'Str({char_text}{limit_text}{regex_text}convert={self._convert})'
 
-    def check(self, check_target, convert=None) -> bool:
-        check_target = self.convert(check_target, convert)
+    def convert_function(self, check_target) -> str:
+        return str(check_target)
+
+    def check_function(self, check_target) -> typing.List[str]:
+        fail_str: typing.List[str] = []
         if isinstance(check_target, str):
-            re_bool = True
             if self._char:
-                re_bool = re_bool and all([_ in self._char for _ in check_target])
-            re_bool = re_bool and self._length.check(len(check_target))
+                char_error = [[_i, _v] for _i, _v in enumerate(check_target) if _v not in self._char]
+                if char_error:
+                    fail_str.append(f'{check_target} contain char more than <{self._char}>:{char_error}')
+            if not self._length.check(len(check_target)):
+                fail_str.append(f'{len(check_target)} length of {check_target} did not match: {self._length.show_all_step()}')
             if self._regex:
-                re_bool = re_bool and bool(re.search(self._regex, check_target))
+                if not bool(re.search(self._regex, check_target)):
+                    fail_str.append(f'{check_target} does not meet rule {self._regex}')
         else:
-            re_bool = False
-        return re_bool
-
-    def _convert_function(self, check_target) -> str:
-        return str(check_target)
+            fail_str.append(f'{check_target} is {type(check_target).__name__} not number')
+        return fail_str
 
     @property
     def annotation(self):
         return str
 
 
 class List(Type):
     def __init__(self, length='', convert=False, **kwargs):
         super().__init__(convert=convert, **kwargs)
         self._length = CheckFormula(length, NumberCheck)
 
     def __repr__(self):
-        length_text = f'length={self._length}, ' if self._length._str_formula else ''
+        length_text = f'length={self._length}, ' if self._length.formula else ''
         return f'List({length_text}convert={self._convert})'
 
+    def convert_function(self, check_target) -> list:
+        if isinstance(check_target, str):
+            check_target = eval(check_target)
+        return list(check_target)
+
+    def check_function(self, check_target) -> typing.List[str]:
+        fail_str: typing.List[str] = []
+        if isinstance(check_target, str):
+            if not self._length.check(len(check_target)):
+                fail_str.append(f'{len(check_target)} length of {check_target} did not match: {self._length.show_all_step()}')
+        else:
+            fail_str.append(f'{check_target} is {type(check_target).__name__} not number')
+        return fail_str
+
     def check(self, check_target, convert=None) -> bool:
         check_target = self.convert(check_target, convert)
         if isinstance(check_target, list):
             re_bool = True
             re_bool = re_bool and self._length.check(len(check_target))
         else:
             re_bool = False
         return re_bool
 
-    def _convert_function(self, check_target) -> list:
-        if isinstance(check_target, str):
-            check_target = json.loads(check_target)
-        return list(check_target)
-
     @property
     def annotation(self):
         if self._convert:
-            return Union[list, str]
+            return typing.Union[list, str]
         else:
             return list
 
 
 class Tuple(Type):
     def __init__(self, length='', convert=False, **kwargs):
         super().__init__(convert=convert, **kwargs)
         self._length = CheckFormula(length, NumberCheck)
 
     def __repr__(self):
-        length_text = f'length={self._length}, ' if self._length._str_formula else ''
+        length_text = f'length={self._length}, ' if self._length.formula else ''
         return f'Tuple({length_text}convert={self._convert})'
 
-    def check(self, check_target, convert=None) -> bool:
-        check_target = self.convert(check_target, convert)
-        if isinstance(check_target, tuple):
-            re_bool = True
-            re_bool = re_bool and self._length.check(len(check_target))
-        else:
-            re_bool = False
-        return re_bool
-
-    def _convert_function(self, check_target) -> tuple:
+    def convert_function(self, check_target) -> tuple:
         if isinstance(check_target, str):
-            check_target = json.loads(check_target)
+            check_target = eval(check_target)
         return tuple(check_target)
 
+    def check_function(self, check_target) -> typing.List[str]:
+        fail_str: typing.List[str] = []
+        if isinstance(check_target, str):
+            if not self._length.check(len(check_target)):
+                fail_str.append(f'{len(check_target)} length of {check_target} did not match: {self._length.show_all_step()}')
+        else:
+            fail_str.append(f'{check_target} is {type(check_target).__name__} not number')
+        return fail_str
+
     @property
     def annotation(self):
         if self._convert:
-            return Union[tuple, str]
+            return typing.Union[tuple, str]
         else:
             return tuple
 
 
 class Set(Type):
     def __init__(self, length='', convert=False, **kwargs):
         super().__init__(convert=convert, **kwargs)
         self._length = CheckFormula(length, NumberCheck)
 
     def __repr__(self):
-        length_text = f'length={self._length}, ' if self._length._str_formula else ''
+        length_text = f'length={self._length}, ' if self._length.formula else ''
         return f'Set({length_text}convert={self._convert})'
 
-    def check(self, check_target, convert=None) -> bool:
-        check_target = self.convert(check_target, convert)
-        if isinstance(check_target, set):
-            re_bool = True
-            re_bool = re_bool and self._length.check(len(check_target))
-        else:
-            re_bool = False
-        return re_bool
-
-    def _convert_function(self, check_target) -> set:
+    def convert_function(self, check_target) -> set:
         if isinstance(check_target, str):
-            check_target = json.loads(check_target)
+            check_target = eval(check_target)
         return set(check_target)
 
+    def check_function(self, check_target) -> typing.List[str]:
+        fail_str: typing.List[str] = []
+        if isinstance(check_target, str):
+            if not self._length.check(len(check_target)):
+                fail_str.append(f'{len(check_target)} length of {check_target} did not match: {self._length.show_all_step()}')
+        else:
+            fail_str.append(f'{check_target} is {type(check_target).__name__} not number')
+        return fail_str
+
     @property
     def annotation(self):
         if self._convert:
-            return Union[set, str]
+            return typing.Union[set, str]
         else:
             return set
 
 
 class Dict(Type):
     def __init__(self, length='', convert=False, **kwargs):
         super().__init__(convert=convert, **kwargs)
         self._length = CheckFormula(length, NumberCheck)
 
     def __repr__(self):
-        length_text = f'length={self._length}, ' if self._length._str_formula else ''
+        length_text = f'length={self._length}, ' if self._length.formula else ''
         return f'Dict({length_text}convert={self._convert})'
 
-    def check(self, check_target, convert=None) -> bool:
-        check_target = self.convert(check_target, convert)
-        if isinstance(check_target, dict):
-            re_bool = True
-            re_bool = re_bool and self._length.check(len(check_target))
-        else:
-            re_bool = False
-        return re_bool
-
-    def _convert_function(self, check_target) -> dict:
+    def convert_function(self, check_target) -> dict:
         if isinstance(check_target, str):
-            check_target = json.loads(check_target)
+            check_target = eval(check_target)
         return dict(check_target)
 
+    def check_function(self, check_target) -> typing.List[str]:
+        fail_str: typing.List[str] = []
+        if isinstance(check_target, str):
+            if not self._length.check(len(check_target)):
+                fail_str.append(f'{len(check_target)} length of {check_target} did not match: {self._length.show_all_step()}')
+        else:
+            fail_str.append(f'{check_target} is {type(check_target).__name__} not number')
+        return fail_str
+
     @property
     def annotation(self):
         if self._convert:
-            return Union[dict, str]
+            return typing.Union[dict, str]
         else:
             return dict
 
 
 class Path(Type):
-    def __init__(self, should_exist=True, convert=False, **kwargs):
+    def __init__(self, should_exist=False, convert=False, **kwargs):
         super().__init__(convert=convert, **kwargs)
         self._should_exist = should_exist
 
     def __repr__(self):
         return f'Path(convert={self._convert})'
 
     def check(self, check_target, convert=None) -> bool:
@@ -333,71 +371,92 @@
                     re_bool = True
             except:
                 re_bool = False
         else:
             re_bool = False
         return re_bool
 
-    def _convert_function(self, check_target):
+    def convert_function(self, check_target):
         return str(check_target)
 
+    def check_function(self, check_target) -> typing.List[str]:
+        fail_str: typing.List[str] = []
+        if isinstance(check_target, str):
+            try:
+                tar_path = pathlib.Path(check_target)
+                if self._should_exist and not tar_path.exists():
+                    fail_str.append(f'{check_target} does not exists.')
+            except:
+                fail_str.append(f'{check_target} is not a valid path.')
+        else:
+            fail_str.append(f'{check_target} is {type(check_target).__name__} not number')
+        return fail_str
+
     @property
     def annotation(self):
         return str
 
 
 default_type = {
-    bool: Bool,
-    str: Str,
-    int: Int,
-    float: Float,
-    list: List,
-    set: Set,
-    tuple: Tuple,
-    dict: Dict,
+    "builtin": {
+        bool: Bool,
+        str: Str,
+        int: Int,
+        float: Float,
+        list: List,
+        set: Set,
+        tuple: Tuple,
+        dict: Dict,
+    }
 }
 
 
+def convert_type(target_type, **kwargs):
+    if isinstance(target_type, Type):
+        return target_type
+    elif target_type in default_type['builtin']:
+        return default_type['builtin'][target_type](**kwargs)
+    else:
+        return None
+
+
 def check_parameters_type(convert=False, check_arguments=True, check_return=True):
     def dec(func):
         argument_annotation = {}
         return_annotation = {}
         change_annotation = {}
         for _i, _v in func.__annotations__.items():
-            if _v in default_type:
-                real_annotation = default_type[_v](convert=convert)
-                change_annotation[_i] = _v
-            elif isinstance(_v, Type):
-                real_annotation = _v
-                change_annotation[_i] = _v.annotation
-            else:
-                change_annotation[_i] = _v
+            _v_convert = convert_type(_v)
+            if _v is None:
                 continue
+            else:
+                real_annotation = _v_convert
+                change_annotation[_i] = _v.annotation
             if _i == 'return':
                 if check_return:
                     return_annotation[_i] = real_annotation
             else:
                 if check_arguments:
                     argument_annotation[_i] = real_annotation
         func.__annotations__ = change_annotation
 
         @recover_signature_from_function_func(func)
         def wrapper(**kwargs):
             for _i2, _v2 in kwargs.items():
                 if _i2 in argument_annotation:
                     _v3 = argument_annotation[_i2]
-                    check_result = _v3.check(_v2)
-                    if not check_result:
-                        raise TypeError(f'{_i2} is {_v2}({type(_v2).__name__}),but it should be a {_v3}')
-                    kwargs[_i2] = _v3.convert(_v2)
+                    _bool, _value = _v3.check(_v2, convert=convert)
+                    if not _bool:
+                        raise TypeError('\n'.join(_value))
+                    kwargs[_i2] = _value
             re_value = func(**kwargs)
             if 'return' in return_annotation:
                 _v3 = return_annotation['return']
-                check_result = _v3.check(re_value)
-                if not check_result:
-                    raise TypeError(f'return value is {re_value}({type(re_value).__name__}),but it should be a {_v3}')
-                re_value = _v3.convert(re_value)
+                _bool, _value = _v3.check(re_value, convert=convert)
+                if not _bool:
+                    raise TypeError('\n'.join(_value))
+                re_value = _value
             return re_value
 
         return wrapper
 
     return dec
```

