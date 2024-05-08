# Comparing `tmp/basewhat-1.0.4.tar.gz` & `tmp/basewhat-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "basewhat-1.0.4.tar", max compression
+gzip compressed data, was "basewhat-1.1.tar", max compression
```

## Comparing `basewhat-1.0.4.tar` & `basewhat-1.1.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0      602 2022-07-30 20:23:53.794758 basewhat-1.0.4/README.md
--rw-r--r--   0        0        0       31 2022-07-30 20:33:24.703995 basewhat-1.0.4/basewhat/__init__.py
--rwxr-xr-x   0        0        0     2363 2022-07-30 20:23:53.795805 basewhat-1.0.4/basewhat/basewhat.py
--rw-r--r--   0        0        0        0 2022-07-30 20:23:53.796279 basewhat-1.0.4/basewhat/py.typed
--rw-r--r--   0        0        0      679 2022-07-30 20:38:06.855709 basewhat-1.0.4/pyproject.toml
--rw-r--r--   0        0        0     1224 2022-07-30 20:38:41.086420 basewhat-1.0.4/setup.py
--rw-r--r--   0        0        0     1491 2022-07-30 20:38:41.086790 basewhat-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0      629 2024-05-07 01:42:15.261384 basewhat-1.1/README.md
+-rw-r--r--   0        0        0       43 2024-05-08 02:24:33.353011 basewhat-1.1/basewhat/__init__.py
+-rwxr-xr-x   0        0        0     3425 2024-05-08 02:21:36.147598 basewhat-1.1/basewhat/basewhat.py
+-rw-r--r--   0        0        0        0 2022-07-30 20:23:53.796279 basewhat-1.1/basewhat/py.typed
+-rw-r--r--   0        0        0      759 2024-05-07 01:39:38.959438 basewhat-1.1/pyproject.toml
+-rw-r--r--   0        0        0     1700 1970-01-01 00:00:00.000000 basewhat-1.1/PKG-INFO
```

### Comparing `basewhat-1.0.4/basewhat/basewhat.py` & `basewhat-1.1/basewhat/basewhat.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,22 @@
-﻿"""
+"""
 Convert integers to and from strings in other bases.
 """
 
 
 class BaseWhat(object):
     """
     Encode/decode arbitrary-base numbers (as strings).
 
     >>> b16 = BaseWhat(base=16)
     >>> b16.from_int(65535)
     'FFFF'
     >>> b16.to_int('DECAFBAD')
     3737844653
+
     >>> b32 = BaseWhat(digits="23456789ABCDEFGHJKLMNPQRSTUVWXYZ")
     >>> b32.from_int(32767)
     'ZZZ'
     >>> b32.from_int(9223372036854775808)
     'A222222222222'
     >>> b32.to_int('1900MIXALOT')
     Traceback (most recent call last):
@@ -25,35 +26,62 @@
     'CV9'
     >>> b32.from_int(-11111)
     '-CV9'
     >>> b32.from_int(0)
     '0'
     >>> b32.to_int('DECAFBAD')
     391186392331
+
+    Converters are case-sensitive by default
+    >>> b2 = BaseWhat(digits='aA')
+    >>> b2.to_int('AaaAaaA')
+    73
+
+    ...but can be made case-insensitive
+    >>> b5 = BaseWhat(base=16, case_sensitive=False)
+    >>> b5.to_int('a') == b5.to_int('A')
+    True
     """
-    def __init__(self, base=None, digits=None) -> None:
+
+    def __init__(self, base=None, digits=None, case_sensitive=True) -> None:
         """
         Construct an instance given either the base or an explicit set of symbols to use for digits.
 
-        :param: base: The number base
-        :param: digits: A string containing this base's digits, in order
+        :param int base: The number base (optional, if `digits` is specified)
+        :param str digits: A string containing this base's digits, in order (optional, if `base` is specified and is 36 or less)
+        :param bool case_sensitive: For digit sets with alphabetic characters, make lowercase/uppercase significant (default: True)
         """
         RAW_DIGITS = "0123456789ABCDEFGHIJKLMNOPQRSTUVWXYZ"
         if not (base or digits):
             raise ValueError("Either base or digits required")
         if base and digits and base != len(digits):
             raise ValueError("Base and digits are mismatched")
+        if base and base > len(RAW_DIGITS) and not digits:
+            raise ValueError("Must specify digits for bases over 36")
         if base and not digits:
             self.base = base
             self.digits = RAW_DIGITS[:base]
         if digits:
             self.digits = digits
             self.base = len(digits)
+        self.case_sensitive = case_sensitive
 
-    def from_int(self, num:int) -> str:
+    def valid_digit(self, d: str) -> bool:
+        if self.case_sensitive:
+            return d in self.digits
+        else:
+            return d.upper() in self.digits.upper()
+
+    def digit_value(self, digit: str) -> int:
+        if self.case_sensitive:
+            return self.digits.index(digit)
+        else:
+            return self.digits.upper().index(digit.upper())
+
+    def from_int(self, num: int) -> str:
         result = ""
         negative = False
         if num == 0:
             result = "0"
         elif num < 0:
             num = abs(num)
             negative = True
@@ -61,21 +89,21 @@
             digitval = num % self.base
             result = self.digits[digitval] + result
             num //= self.base
         if negative:
             result = "-" + result
         return result
 
-    def to_int(self, encoded:str) -> int:
-        if any((d not in self.digits for d in encoded)):
+    def to_int(self, encoded: str) -> int:
+        if any((not self.valid_digit(d) for d in encoded)):
             raise ValueError("Not a valid base {0} number".format(self.base))
         result = 0
         for pos, digit in enumerate(encoded):
-            result += self.digits.index(digit) * pow(self.base, len(encoded) - pos - 1)
+            result += self.digit_value(digit) * pow(self.base, len(encoded) - pos - 1)
         return result
 
 
 if __name__ == "__main__":
     import doctest
+
     doctest.testmod()
     print("Tests complete.")
-
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `basewhat-1.0.4/PKG-INFO` & `basewhat-1.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,35 +1,41 @@
 Metadata-Version: 2.1
 Name: basewhat
-Version: 1.0.4
+Version: 1.1
 Summary: A Python utility for encoding/decoding arbitrary-base numbers.
-Home-page: https://sr.ht/~paulbissex/Basewhat/
+Home-page: https://helixteamhub.cloud/paulbissex/projects/basewhat/activity
 License: MIT
 Author: Paul Bissex
 Author-email: paul@bissex.net
 Requires-Python: >=3.6,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Project-URL: Repository, https://hg.sr.ht/~paulbissex/basewhat
+Project-URL: Repository, https://helixteamhub.cloud/paulbissex/projects/basewhat/repositories/basewhat/tree/default
 Description-Content-Type: text/markdown
 
 ﻿basewhat
 ========
 
 A Python utility for encoding/decoding arbitrary-base numbers.
 
-**Usage:**
+**Project home page**: <https://helixteamhub.cloud/paulbissex/projects/basewhat/>
+
+**Author**: Paul Bissex <paul@bissex.net>
+
+## Usage
 
     >>> b16 = BaseWhat(base=16)
     >>> b16.from_int(65535)
     'FFFF'
     >>> b16.to_int('DECAFBAD')
     3737844653
     >>> b32 = BaseWhat(digits="23456789ABCDEFGHJKLMNPQRSTUVWXYZ")
@@ -38,11 +44,7 @@
     >>> b32.from_int(9223372036854775808)
     'A222222222222'
     >>> b32.to_int('1900MIXALOT')
     Traceback (most recent call last):
     ...
     ValueError: Not a valid base 32 number
 
-Project home page: <https://sr.ht/~paulbissex/Basewhat/>
-
-Author: Paul Bissex <paul@bissex.net>
-
```

