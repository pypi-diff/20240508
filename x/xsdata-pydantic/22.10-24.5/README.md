# Comparing `tmp/xsdata_pydantic-22.10.tar.gz` & `tmp/xsdata_pydantic-24.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xsdata_pydantic-22.10.tar", last modified: Sun Oct  2 07:21:44 2022, max compression
+gzip compressed data, was "xsdata_pydantic-24.5.tar", last modified: Wed May  8 17:49:35 2024, max compression
```

## Comparing `xsdata_pydantic-22.10.tar` & `xsdata_pydantic-24.5.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-02 07:21:44.094139 xsdata_pydantic-22.10/
--rw-r--r--   0 runner    (1001) docker     (121)       56 2022-10-02 07:21:35.000000 xsdata_pydantic-22.10/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1082 2022-10-02 07:21:35.000000 xsdata_pydantic-22.10/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      242 2022-10-02 07:21:35.000000 xsdata_pydantic-22.10/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     4366 2022-10-02 07:21:44.094139 xsdata_pydantic-22.10/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3016 2022-10-02 07:21:35.000000 xsdata_pydantic-22.10/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-02 07:21:44.090139 xsdata_pydantic-22.10/docs/
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-10-02 07:21:35.000000 xsdata_pydantic-22.10/docs/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      719 2022-10-02 07:21:35.000000 xsdata_pydantic-22.10/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-02 07:21:44.090139 xsdata_pydantic-22.10/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)      342 2022-10-02 07:21:35.000000 xsdata_pydantic-22.10/docs/_static/favicon.png
--rw-r--r--   0 runner    (1001) docker     (121)     6893 2022-10-02 07:21:35.000000 xsdata_pydantic-22.10/docs/_static/logo.svg
--rw-r--r--   0 runner    (1001) docker     (121)     1800 2022-10-02 07:21:35.000000 xsdata_pydantic-22.10/docs/bindings.rst
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-10-02 07:21:35.000000 xsdata_pydantic-22.10/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1242 2022-10-02 07:21:35.000000 xsdata_pydantic-22.10/docs/codegen.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2307 2022-10-02 07:21:35.000000 xsdata_pydantic-22.10/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)     1143 2022-10-02 07:21:35.000000 xsdata_pydantic-22.10/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      786 2022-10-02 07:21:35.000000 xsdata_pydantic-22.10/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (121)      795 2022-10-02 07:21:35.000000 xsdata_pydantic-22.10/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (121)     1833 2022-10-02 07:21:44.094139 xsdata_pydantic-22.10/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-02 07:21:35.000000 xsdata_pydantic-22.10/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-02 07:21:44.090139 xsdata_pydantic-22.10/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-02 07:21:35.000000 xsdata_pydantic-22.10/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-02 07:21:44.094139 xsdata_pydantic-22.10/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-02 07:21:35.000000 xsdata_pydantic-22.10/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      483 2022-10-02 07:21:35.000000 xsdata_pydantic-22.10/tests/fixtures/common.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-02 07:21:44.094139 xsdata_pydantic-22.10/tests/fixtures/po/
--rw-r--r--   0 runner    (1001) docker     (121)      228 2022-10-02 07:21:35.000000 xsdata_pydantic-22.10/tests/fixtures/po/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4085 2022-10-02 07:21:35.000000 xsdata_pydantic-22.10/tests/fixtures/po/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     1379 2022-10-02 07:21:35.000000 xsdata_pydantic-22.10/tests/fixtures/pydantic.conf.xml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-02 07:21:44.094139 xsdata_pydantic-22.10/tests/fixtures/schemas/
--rw-r--r--   0 runner    (1001) docker     (121)     2242 2022-10-02 07:21:35.000000 xsdata_pydantic-22.10/tests/fixtures/schemas/po.xsd
--rw-r--r--   0 runner    (1001) docker     (121)     3415 2022-10-02 07:21:35.000000 xsdata_pydantic-22.10/tests/test_bindings.py
--rw-r--r--   0 runner    (1001) docker     (121)      684 2022-10-02 07:21:35.000000 xsdata_pydantic-22.10/tests/test_compat.py
--rw-r--r--   0 runner    (1001) docker     (121)     3635 2022-10-02 07:21:35.000000 xsdata_pydantic-22.10/tests/test_generator.py
--rw-r--r--   0 runner    (1001) docker     (121)      891 2022-10-02 07:21:35.000000 xsdata_pydantic-22.10/tox.ini
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-02 07:21:44.094139 xsdata_pydantic-22.10/xsdata_pydantic/
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-10-02 07:21:35.000000 xsdata_pydantic-22.10/xsdata_pydantic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1203 2022-10-02 07:21:35.000000 xsdata_pydantic-22.10/xsdata_pydantic/bindings.py
--rw-r--r--   0 runner    (1001) docker     (121)     3230 2022-10-02 07:21:35.000000 xsdata_pydantic-22.10/xsdata_pydantic/compat.py
--rw-r--r--   0 runner    (1001) docker     (121)     1118 2022-10-02 07:21:35.000000 xsdata_pydantic-22.10/xsdata_pydantic/generator.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-02 07:21:44.094139 xsdata_pydantic-22.10/xsdata_pydantic/hooks/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-02 07:21:35.000000 xsdata_pydantic-22.10/xsdata_pydantic/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      147 2022-10-02 07:21:35.000000 xsdata_pydantic-22.10/xsdata_pydantic/hooks/class_type.py
--rw-r--r--   0 runner    (1001) docker     (121)      164 2022-10-02 07:21:35.000000 xsdata_pydantic-22.10/xsdata_pydantic/hooks/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-02 07:21:35.000000 xsdata_pydantic-22.10/xsdata_pydantic/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-02 07:21:44.094139 xsdata_pydantic-22.10/xsdata_pydantic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4366 2022-10-02 07:21:44.000000 xsdata_pydantic-22.10/xsdata_pydantic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      994 2022-10-02 07:21:44.000000 xsdata_pydantic-22.10/xsdata_pydantic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-02 07:21:44.000000 xsdata_pydantic-22.10/xsdata_pydantic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      146 2022-10-02 07:21:44.000000 xsdata_pydantic-22.10/xsdata_pydantic.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      175 2022-10-02 07:21:44.000000 xsdata_pydantic-22.10/xsdata_pydantic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-10-02 07:21:44.000000 xsdata_pydantic-22.10/xsdata_pydantic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:49:35.507119 xsdata_pydantic-24.5/
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-08 17:49:31.000000 xsdata_pydantic-24.5/CHANGES.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-08 17:49:31.000000 xsdata_pydantic-24.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-08 17:49:31.000000 xsdata_pydantic-24.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4854 2024-05-08 17:49:35.507119 xsdata_pydantic-24.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2534 2024-05-08 17:49:31.000000 xsdata_pydantic-24.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:49:35.503119 xsdata_pydantic-24.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-08 17:49:31.000000 xsdata_pydantic-24.5/docs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-05-08 17:49:31.000000 xsdata_pydantic-24.5/docs/bindings.md
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-08 17:49:31.000000 xsdata_pydantic-24.5/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-08 17:49:31.000000 xsdata_pydantic-24.5/docs/codegen.md
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-08 17:49:31.000000 xsdata_pydantic-24.5/docs/favicon.png
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-08 17:49:31.000000 xsdata_pydantic-24.5/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-08 17:49:31.000000 xsdata_pydantic-24.5/docs/installation.md
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-05-08 17:49:31.000000 xsdata_pydantic-24.5/docs/issues.md
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-05-08 17:49:31.000000 xsdata_pydantic-24.5/docs/logo-small.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     6893 2024-05-08 17:49:31.000000 xsdata_pydantic-24.5/docs/logo.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:49:35.503119 xsdata_pydantic-24.5/docs/overrides/
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-08 17:49:31.000000 xsdata_pydantic-24.5/docs/overrides/main.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2406 2024-05-08 17:49:31.000000 xsdata_pydantic-24.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 17:49:35.507119 xsdata_pydantic-24.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:49:35.503119 xsdata_pydantic-24.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 17:49:31.000000 xsdata_pydantic-24.5/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:49:35.503119 xsdata_pydantic-24.5/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 17:49:31.000000 xsdata_pydantic-24.5/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-08 17:49:31.000000 xsdata_pydantic-24.5/tests/fixtures/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:49:35.503119 xsdata_pydantic-24.5/tests/fixtures/po/
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-08 17:49:31.000000 xsdata_pydantic-24.5/tests/fixtures/po/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4235 2024-05-08 17:49:31.000000 xsdata_pydantic-24.5/tests/fixtures/po/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-05-08 17:49:31.000000 xsdata_pydantic-24.5/tests/fixtures/pydantic.conf.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:49:35.503119 xsdata_pydantic-24.5/tests/fixtures/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-05-08 17:49:31.000000 xsdata_pydantic-24.5/tests/fixtures/schemas/po.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-05-08 17:49:31.000000 xsdata_pydantic-24.5/tests/test_bindings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-08 17:49:31.000000 xsdata_pydantic-24.5/tests/test_compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-08 17:49:31.000000 xsdata_pydantic-24.5/tests/test_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:49:35.507119 xsdata_pydantic-24.5/xsdata_pydantic/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-08 17:49:31.000000 xsdata_pydantic-24.5/xsdata_pydantic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4176 2024-05-08 17:49:31.000000 xsdata_pydantic-24.5/xsdata_pydantic/bindings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4003 2024-05-08 17:49:31.000000 xsdata_pydantic-24.5/xsdata_pydantic/compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-08 17:49:31.000000 xsdata_pydantic-24.5/xsdata_pydantic/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-05-08 17:49:31.000000 xsdata_pydantic-24.5/xsdata_pydantic/generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:49:35.507119 xsdata_pydantic-24.5/xsdata_pydantic/hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 17:49:31.000000 xsdata_pydantic-24.5/xsdata_pydantic/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-08 17:49:31.000000 xsdata_pydantic-24.5/xsdata_pydantic/hooks/class_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-08 17:49:31.000000 xsdata_pydantic-24.5/xsdata_pydantic/hooks/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 17:49:31.000000 xsdata_pydantic-24.5/xsdata_pydantic/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:49:35.507119 xsdata_pydantic-24.5/xsdata_pydantic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4854 2024-05-08 17:49:35.000000 xsdata_pydantic-24.5/xsdata_pydantic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-05-08 17:49:35.000000 xsdata_pydantic-24.5/xsdata_pydantic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 17:49:35.000000 xsdata_pydantic-24.5/xsdata_pydantic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-08 17:49:35.000000 xsdata_pydantic-24.5/xsdata_pydantic.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-08 17:49:35.000000 xsdata_pydantic-24.5/xsdata_pydantic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-08 17:49:35.000000 xsdata_pydantic-24.5/xsdata_pydantic.egg-info/top_level.txt
```

### Comparing `xsdata_pydantic-22.10/LICENSE` & `xsdata_pydantic-24.5/LICENSE`

 * *Files identical despite different names*

### Comparing `xsdata_pydantic-22.10/docs/_static/logo.svg` & `xsdata_pydantic-24.5/docs/logo.svg`

 * *Files identical despite different names*

### Comparing `xsdata_pydantic-22.10/tests/fixtures/po/models.py` & `xsdata_pydantic-24.5/tests/fixtures/po/models.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,82 +1,23 @@
-from dataclasses import field
 from decimal import Decimal
-from pydantic.dataclasses import dataclass
 from typing import List, Optional
-from xsdata.models.datatype import XmlDate
 
-__NAMESPACE__ = "foo"
+from pydantic import BaseModel, ConfigDict
+from xsdata.models.datatype import XmlDate
 
+from xsdata_pydantic.fields import field
 
-@dataclass(slots=True, kw_only=True)
-class Items:
-    item: List["Items.Item"] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "foo",
-        }
-    )
-
-    @dataclass(slots=True, kw_only=True)
-    class Item:
-        product_name: str = field(
-            metadata={
-                "name": "productName",
-                "type": "Element",
-                "namespace": "foo",
-                "required": True,
-            }
-        )
-        quantity: int = field(
-            metadata={
-                "type": "Element",
-                "namespace": "foo",
-                "required": True,
-                "max_exclusive": 100,
-            }
-        )
-        usprice: Decimal = field(
-            metadata={
-                "name": "USPrice",
-                "type": "Element",
-                "namespace": "foo",
-                "required": True,
-            }
-        )
-        comment: Optional[str] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "foo",
-            }
-        )
-        ship_date: Optional[XmlDate] = field(
-            default=None,
-            metadata={
-                "name": "shipDate",
-                "type": "Element",
-                "namespace": "foo",
-            }
-        )
-        part_num: str = field(
-            metadata={
-                "name": "partNum",
-                "type": "Attribute",
-                "required": True,
-                "pattern": r"\d{3}-[A-Z]{2}",
-            }
-        )
+__NAMESPACE__ = "foo"
 
 
-@dataclass(slots=True, kw_only=True)
-class Usaddress:
+class Usaddress(BaseModel):
     class Meta:
         name = "USAddress"
 
+    model_config = ConfigDict(defer_build=True)
     name: str = field(
         metadata={
             "type": "Element",
             "namespace": "foo",
             "required": True,
         }
     )
@@ -105,38 +46,99 @@
         metadata={
             "type": "Element",
             "namespace": "foo",
             "required": True,
         }
     )
     country: str = field(
-        init=False,
+        const=True,
         default="US",
         metadata={
             "type": "Attribute",
-        }
+        },
     )
 
 
-@dataclass(slots=True, kw_only=True)
-class Comment:
+class Comment(BaseModel):
     class Meta:
         name = "comment"
         namespace = "foo"
 
+    model_config = ConfigDict(defer_build=True)
     value: str = field(
         default="",
         metadata={
             "required": True,
-        }
+        },
     )
 
 
-@dataclass(slots=True, kw_only=True)
-class PurchaseOrderType:
+class Items(BaseModel):
+    model_config = ConfigDict(defer_build=True)
+    item: List["Items.Item"] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+            "namespace": "foo",
+        },
+    )
+
+    class Item(BaseModel):
+        model_config = ConfigDict(defer_build=True)
+        product_name: str = field(
+            metadata={
+                "name": "productName",
+                "type": "Element",
+                "namespace": "foo",
+                "required": True,
+            }
+        )
+        quantity: int = field(
+            metadata={
+                "type": "Element",
+                "namespace": "foo",
+                "required": True,
+                "max_exclusive": 100,
+            }
+        )
+        usprice: Decimal = field(
+            metadata={
+                "name": "USPrice",
+                "type": "Element",
+                "namespace": "foo",
+                "required": True,
+            }
+        )
+        comment: Optional[Comment] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+                "namespace": "foo",
+            },
+        )
+        ship_date: Optional[XmlDate] = field(
+            default=None,
+            metadata={
+                "name": "shipDate",
+                "type": "Element",
+                "namespace": "foo",
+            },
+        )
+        part_num: str = field(
+            metadata={
+                "name": "partNum",
+                "type": "Attribute",
+                "required": True,
+                "pattern": r"\d{3}-[A-Z]{2}",
+            }
+        )
+
+
+class PurchaseOrderType(BaseModel):
+    model_config = ConfigDict(defer_build=True)
     ship_to: Usaddress = field(
         metadata={
             "name": "shipTo",
             "type": "Element",
             "namespace": "foo",
             "required": True,
         }
@@ -145,35 +147,36 @@
         metadata={
             "name": "billTo",
             "type": "Element",
             "namespace": "foo",
             "required": True,
         }
     )
-    comment: Optional[str] = field(
+    comment: Optional[Comment] = field(
         default=None,
         metadata={
             "type": "Element",
             "namespace": "foo",
-        }
+        },
     )
     items: Items = field(
         metadata={
             "type": "Element",
             "namespace": "foo",
             "required": True,
         }
     )
     order_date: Optional[XmlDate] = field(
         default=None,
         metadata={
             "name": "orderDate",
             "type": "Attribute",
-        }
+        },
     )
 
 
-@dataclass(slots=True, kw_only=True)
 class PurchaseOrder(PurchaseOrderType):
     class Meta:
         name = "purchaseOrder"
         namespace = "foo"
+
+    model_config = ConfigDict(defer_build=True)
```

### Comparing `xsdata_pydantic-22.10/tests/fixtures/pydantic.conf.xml` & `xsdata_pydantic-24.5/tests/fixtures/pydantic.conf.xml`

 * *Files identical despite different names*

### Comparing `xsdata_pydantic-22.10/tests/fixtures/schemas/po.xsd` & `xsdata_pydantic-24.5/tests/fixtures/schemas/po.xsd`

 * *Files identical despite different names*

### Comparing `xsdata_pydantic-22.10/tests/test_bindings.py` & `xsdata_pydantic-24.5/tests/test_bindings.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 from datetime import datetime
 from unittest import TestCase
 
-from xsdata.formats.dataclass.serializers.config import SerializerConfig
-
 from tests.fixtures.common import TypeC
-from xsdata_pydantic.bindings import JsonParser
-from xsdata_pydantic.bindings import JsonSerializer
+
 from xsdata_pydantic.bindings import XmlParser
 from xsdata_pydantic.bindings import XmlSerializer
 from xsdata_pydantic.compat import AnyElement
 from xsdata_pydantic.compat import DerivedElement
 
 
 class BindingsTests(TestCase):
@@ -28,15 +25,15 @@
                     DerivedElement(qname="bar", value=2),
                 ]
             ),
         )
 
     def test_xml_bindings(self):
         serializer = XmlSerializer()
-        serializer.config.pretty_print = True
+        serializer.config.indent = "  "
         serializer.config.xml_declaration = False
         parser = XmlParser()
         ns_map = {
             "xs": "http://www.w3.org/2001/XMLSchema",
             "xsi": "http://www.w3.org/2001/XMLSchema-instance",
         }
 
@@ -51,50 +48,7 @@
             "  <foo>bar</foo>\n"
             '  <bar xsi:type="xs:string">1</bar>\n'
             '  <bar xsi:type="xs:short">2</bar>\n'
             "</TypeC>\n"
         )
         self.assertEqual(expected, serializer.render(self.obj, ns_map))
         self.assertEqual(self.obj, parser.from_string(expected))
-
-    def test_serialize_json(self):
-        serializer = JsonSerializer(config=SerializerConfig(pretty_print=True))
-        parser = JsonParser()
-
-        expected = (
-            "{\n"
-            '  "one": "first",\n'
-            '  "two": 1.1,\n'
-            '  "three": true,\n'
-            '  "four": [\n'
-            '    "01 January 2002 12:01",\n'
-            '    "05 February 2003 13:05"\n'
-            "  ],\n"
-            '  "any": {\n'
-            '    "qname": null,\n'
-            '    "text": null,\n'
-            '    "tail": null,\n'
-            '    "children": [\n'
-            "      {\n"
-            '        "qname": "foo",\n'
-            '        "text": "bar",\n'
-            '        "tail": null,\n'
-            '        "children": [],\n'
-            '        "attributes": {}\n'
-            "      },\n"
-            "      {\n"
-            '        "qname": "bar",\n'
-            '        "value": "1",\n'
-            '        "type": null\n'
-            "      },\n"
-            "      {\n"
-            '        "qname": "bar",\n'
-            '        "value": 2,\n'
-            '        "type": null\n'
-            "      }\n"
-            "    ],\n"
-            '    "attributes": {}\n'
-            "  }\n"
-            "}"
-        )
-        self.assertEqual(expected, serializer.render(self.obj))
-        self.assertEqual(self.obj, parser.from_string(expected, TypeC))
```

### Comparing `xsdata_pydantic-22.10/tests/test_compat.py` & `xsdata_pydantic-24.5/tests/test_compat.py`

 * *Files identical despite different names*

### Comparing `xsdata_pydantic-22.10/xsdata_pydantic.egg-info/SOURCES.txt` & `xsdata_pydantic-24.5/xsdata_pydantic.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -1,38 +1,37 @@
-CHANGES.rst
+CHANGES.md
 LICENSE
 MANIFEST.in
-README.rst
-setup.cfg
-setup.py
-tox.ini
+README.md
+pyproject.toml
 docs/.gitignore
-docs/Makefile
-docs/bindings.rst
-docs/changelog.rst
-docs/codegen.rst
-docs/conf.py
-docs/index.rst
-docs/installation.rst
-docs/make.bat
-docs/_static/favicon.png
-docs/_static/logo.svg
+docs/bindings.md
+docs/changelog.md
+docs/codegen.md
+docs/favicon.png
+docs/index.md
+docs/installation.md
+docs/issues.md
+docs/logo-small.svg
+docs/logo.svg
+docs/overrides/main.html
 tests/__init__.py
 tests/test_bindings.py
 tests/test_compat.py
 tests/test_generator.py
 tests/fixtures/__init__.py
 tests/fixtures/common.py
 tests/fixtures/pydantic.conf.xml
 tests/fixtures/po/__init__.py
 tests/fixtures/po/models.py
 tests/fixtures/schemas/po.xsd
 xsdata_pydantic/__init__.py
 xsdata_pydantic/bindings.py
 xsdata_pydantic/compat.py
+xsdata_pydantic/fields.py
 xsdata_pydantic/generator.py
 xsdata_pydantic/py.typed
 xsdata_pydantic.egg-info/PKG-INFO
 xsdata_pydantic.egg-info/SOURCES.txt
 xsdata_pydantic.egg-info/dependency_links.txt
 xsdata_pydantic.egg-info/entry_points.txt
 xsdata_pydantic.egg-info/requires.txt
```

