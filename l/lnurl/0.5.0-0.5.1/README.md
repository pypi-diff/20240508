# Comparing `tmp/lnurl-0.5.0.tar.gz` & `tmp/lnurl-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lnurl-0.5.0.tar", max compression
+gzip compressed data, was "lnurl-0.5.1.tar", max compression
```

## Comparing `lnurl-0.5.0.tar` & `lnurl-0.5.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1111 2024-04-25 14:28:25.816641 lnurl-0.5.0/LICENSE
--rwxr-xr-x   0        0        0     6163 2024-04-25 14:28:25.816641 lnurl-0.5.0/README.md
--rw-r--r--   0        0        0      816 2024-04-25 14:28:25.816641 lnurl-0.5.0/lnurl/__init__.py
--rwxr-xr-x   0        0        0     1521 2024-04-25 14:28:25.816641 lnurl-0.5.0/lnurl/cli.py
--rw-r--r--   0        0        0     4863 2024-04-25 14:28:25.816641 lnurl-0.5.0/lnurl/core.py
--rw-r--r--   0        0        0      486 2024-04-25 14:28:25.816641 lnurl-0.5.0/lnurl/exceptions.py
--rw-r--r--   0        0        0     3781 2024-04-25 14:28:25.816641 lnurl-0.5.0/lnurl/helpers.py
--rw-r--r--   0        0        0     5498 2024-04-25 14:28:25.816641 lnurl-0.5.0/lnurl/models.py
--rw-r--r--   0        0        0       26 2024-04-25 14:28:25.816641 lnurl-0.5.0/lnurl/py.typed
--rw-r--r--   0        0        0     8693 2024-04-25 14:28:25.816641 lnurl-0.5.0/lnurl/types.py
--rw-r--r--   0        0        0     1796 2024-04-25 14:28:25.816641 lnurl-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     6878 1970-01-01 00:00:00.000000 lnurl-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1111 2024-05-08 05:54:28.025692 lnurl-0.5.1/LICENSE
+-rwxr-xr-x   0        0        0     6163 2024-05-08 05:54:28.025692 lnurl-0.5.1/README.md
+-rw-r--r--   0        0        0      816 2024-05-08 05:54:28.025692 lnurl-0.5.1/lnurl/__init__.py
+-rwxr-xr-x   0        0        0     1521 2024-05-08 05:54:28.025692 lnurl-0.5.1/lnurl/cli.py
+-rw-r--r--   0        0        0     6704 2024-05-08 05:54:28.025692 lnurl-0.5.1/lnurl/core.py
+-rw-r--r--   0        0        0      486 2024-05-08 05:54:28.025692 lnurl-0.5.1/lnurl/exceptions.py
+-rw-r--r--   0        0        0     3781 2024-05-08 05:54:28.025692 lnurl-0.5.1/lnurl/helpers.py
+-rw-r--r--   0        0        0     5531 2024-05-08 05:54:28.025692 lnurl-0.5.1/lnurl/models.py
+-rw-r--r--   0        0        0       26 2024-05-08 05:54:28.025692 lnurl-0.5.1/lnurl/py.typed
+-rw-r--r--   0        0        0     8693 2024-05-08 05:54:28.025692 lnurl-0.5.1/lnurl/types.py
+-rw-r--r--   0        0        0     1796 2024-05-08 05:54:28.029692 lnurl-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     6878 1970-01-01 00:00:00.000000 lnurl-0.5.1/PKG-INFO
```

### Comparing `lnurl-0.5.0/LICENSE` & `lnurl-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lnurl-0.5.0/README.md` & `lnurl-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `lnurl-0.5.0/lnurl/__init__.py` & `lnurl-0.5.1/lnurl/__init__.py`

 * *Files identical despite different names*

### Comparing `lnurl-0.5.0/lnurl/cli.py` & `lnurl-0.5.1/lnurl/cli.py`

 * *Files identical despite different names*

### Comparing `lnurl-0.5.0/lnurl/helpers.py` & `lnurl-0.5.1/lnurl/helpers.py`

 * *Files identical despite different names*

### Comparing `lnurl-0.5.0/lnurl/models.py` & `lnurl-0.5.1/lnurl/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -134,14 +134,15 @@
     )
 
 
 class LnurlPayActionResponse(LnurlResponseModel):
     pr: LightningInvoice
     success_action: Optional[Union[MessageAction, UrlAction, AesAction]] = Field(None, alias="successAction")
     routes: List[List[LnurlPayRouteHop]] = []
+    verify: Optional[str] = None
 
 
 class LnurlWithdrawResponse(LnurlResponseModel):
     tag: Literal["withdrawRequest"] = "withdrawRequest"
     callback: Union[ClearnetUrl, OnionUrl, DebugUrl]
     k1: str
     min_withdrawable: MilliSatoshi = Field(..., alias="minWithdrawable", gt=0)
```

### Comparing `lnurl-0.5.0/lnurl/types.py` & `lnurl-0.5.1/lnurl/types.py`

 * *Files identical despite different names*

### Comparing `lnurl-0.5.0/pyproject.toml` & `lnurl-0.5.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lnurl"
-version = "0.5.0"
+version = "0.5.1"
 description = "LNURL implementation for Python."
 authors = ["Alan Bits <alan@lnbits.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [
   {include = "lnurl"},
   {include = "lnurl/py.typed"},
```

### Comparing `lnurl-0.5.0/PKG-INFO` & `lnurl-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lnurl
-Version: 0.5.0
+Version: 0.5.1
 Summary: LNURL implementation for Python.
 License: MIT
 Author: Alan Bits
 Author-email: alan@lnbits.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

