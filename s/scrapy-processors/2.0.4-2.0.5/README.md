# Comparing `tmp/scrapy_processors-2.0.4.tar.gz` & `tmp/scrapy_processors-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapy_processors-2.0.4.tar", max compression
+gzip compressed data, was "scrapy_processors-2.0.5.tar", max compression
```

## Comparing `scrapy_processors-2.0.4.tar` & `scrapy_processors-2.0.5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1072 2023-05-16 13:45:56.239068 scrapy_processors-2.0.4/LICENSE
--rw-r--r--   0        0        0    10245 2023-08-17 15:53:09.150295 scrapy_processors-2.0.4/README.md
--rw-r--r--   0        0        0      974 2024-03-21 03:18:00.762761 scrapy_processors-2.0.4/pyproject.toml
--rw-r--r--   0        0        0      955 2023-11-29 01:58:54.990661 scrapy_processors-2.0.4/scrapy_processors/__init__.py
--rw-r--r--   0        0        0    42702 2023-11-29 01:58:54.990661 scrapy_processors-2.0.4/scrapy_processors/base.py
--rw-r--r--   0        0        0     5374 2023-08-17 15:22:52.181833 scrapy_processors-2.0.4/scrapy_processors/collections.py
--rw-r--r--   0        0        0      830 2023-11-29 01:58:54.994661 scrapy_processors-2.0.4/scrapy_processors/common.py
--rw-r--r--   0        0        0     9286 2023-11-29 01:58:54.994661 scrapy_processors-2.0.4/scrapy_processors/multi_values.py
--rw-r--r--   0        0        0    43202 2023-11-29 01:58:54.994661 scrapy_processors-2.0.4/scrapy_processors/single_value.py
--rw-r--r--   0        0        0    11404 1970-01-01 00:00:00.000000 scrapy_processors-2.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-05-16 13:45:56.000000 scrapy_processors-2.0.5/LICENSE
+-rw-r--r--   0        0        0    10222 2024-03-21 03:33:39.000000 scrapy_processors-2.0.5/README.md
+-rw-r--r--   0        0        0     1008 2024-05-06 21:16:53.786128 scrapy_processors-2.0.5/pyproject.toml
+-rw-r--r--   0        0        0      969 2024-05-06 19:15:09.898927 scrapy_processors-2.0.5/scrapy_processors/__init__.py
+-rw-r--r--   0        0        0    42677 2024-05-06 22:29:23.983148 scrapy_processors-2.0.5/scrapy_processors/base.py
+-rw-r--r--   0        0        0     5414 2024-05-06 22:29:51.276907 scrapy_processors-2.0.5/scrapy_processors/collections.py
+-rw-r--r--   0        0        0      830 2023-11-29 01:58:54.000000 scrapy_processors-2.0.5/scrapy_processors/common.py
+-rw-r--r--   0        0        0     9286 2023-09-16 23:15:37.000000 scrapy_processors-2.0.5/scrapy_processors/multi_values.py
+-rw-r--r--   0        0        0    43195 2024-05-06 22:30:06.980353 scrapy_processors-2.0.5/scrapy_processors/single_value.py
+-rw-r--r--   0        0        0    11429 1970-01-01 00:00:00.000000 scrapy_processors-2.0.5/PKG-INFO
```

### Comparing `scrapy_processors-2.0.4/LICENSE` & `scrapy_processors-2.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `scrapy_processors-2.0.4/README.md` & `scrapy_processors-2.0.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 # Scrapy Processors
 
 ![License](https://img.shields.io/badge/license-MIT-blue.svg)
-[![Python Versions](https://img.shields.io/badge/Python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue)](https://www.python.org/)
+[![Python Versions](https://img.shields.io/badge/Python-3.9%20%7C%203.10%20%7C%203.11-blue)](https://www.python.org/)
 <!-- [![codecov](https://codecov.io/gh/nicholas-mischke/scrapy-processors/branch/master/graph/badge.svg)](https://codecov.io/gh/nicholas-mischke/scrapy-processors) -->
 
 Scrapy Processors is a collection of Processor classes meant to work with
 the [itemloaders](https://pypi.org/project/itemloaders/) package, commonly used with the [scrapy](https://pypi.org/project/Scrapy/) webscraping framework.
 
 These processors are meant to extend / replace the provided processors in the [itemloaders](https://pypi.org/project/itemloaders/) package.
 
@@ -161,8 +161,8 @@
 10. Once your PR is approved, it will be merged into the main codebase. Congratulations on your contribution!
 
 If you have any questions or need further assistance, feel free to open an issue or reach out to the project maintainers.
 
 Happy contributing!
 
 ## License
-This project is licensed under the MIT License. See the LICENSE file for more details.
+This project is licensed under the MIT License. See the LICENSE file for more details.
```

### Comparing `scrapy_processors-2.0.4/pyproject.toml` & `scrapy_processors-2.0.5/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 [tool.poetry]
 name = "scrapy-processors"
-version = "2.0.4"
+version = "2.0.5"
 description = "Provides processors for the itemloaders package, commonly used with scrapy."
 authors = ["Nicholas Mischke <nmischkework@proton.me>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "scrapy_processors" }]
 repository = "https://github.com/nicholas-mischke/scrapy-processors"
 keywords = ["scrapy", "itemloaders"]
 
 [tool.poetry.dependencies]
-python = ">=3.9.0"
+python = ">=3.9.0, <4.0.0"
 itemloaders = "^1.1.0"
 emoji = "^2.2.0"
 price-parser = "^0.3.4"
 beautifulsoup4 = "^4.12.2"
 pytz = "^2023.3"
 tzlocal = "^5.0.1"
 dateparser = "^1.1.8"
 phonenumbers = "^8.13.17"
-miscellaneous-utils = "^0.3.6"
+miscellaneous-utils = "^0.3.9"
+pendulum = "^3.0.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
 pytest-cov = "^4.0.0"
 tox = "^4.5.1"
 coverage = "^7.2.5"
 scrapy = "^2.9.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
-sources = [
-    { name = "pypi scrapy-processors", url = "https://pypi.org/project/scrapy-processors/" },
-]
+# sources = [
+#     { name = "pypi scrapy-processors", url = "https://pypi.org/project/scrapy-processors/" },
+# ]
```

### Comparing `scrapy_processors-2.0.4/scrapy_processors/__init__.py` & `scrapy_processors-2.0.5/scrapy_processors/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,15 @@
     PhoneNumbers,
     Socials,
     # ... Misc ...
     SelectJmes
 )
 from scrapy_processors.multi_values import (
     TakeAll,
+    Identity,
     TakeAllTruthy,
     TakeFirst,
     TakeFirstTruthy,
     Coalesce,
     Join,
     Flatten
 )
```

### Comparing `scrapy_processors-2.0.4/scrapy_processors/base.py` & `scrapy_processors-2.0.5/scrapy_processors/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,20 +14,17 @@
     Tuple,
     Type,
     TypeVar,
     Union,
 )
 
 # 3rd 🎉 Imports
+from misc_utils import arg_to_iter
 from misc_utils import ParamProbe
 
-# Local Imports
-from itemloaders.utils import arg_to_iter
-
-
 # Typing variables
 ValueType = TypeVar("ValueType")  # Single input value type
 ValueOrValues = Union[
     ValueType, Iterable[ValueType]
 ]  # Single value or iterable of values
 ContextType = Union[Mapping[str, Any], ChainMap]
```

### Comparing `scrapy_processors-2.0.4/scrapy_processors/collections.py` & `scrapy_processors-2.0.5/scrapy_processors/collections.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # Standard Library Imports
 from typing import Any, List
 
+# 3rd Party Imports
+from misc_utils import arg_to_iter
+
 # Local Imports
-from itemloaders.utils import arg_to_iter
 from scrapy_processors.base import ProcessorCollection
 
 
 class Compose(ProcessorCollection):
     """
     Compose applies a collection of processors to the entire list of values,
     one after the other. If a processor returns a list, or another object type
@@ -134,12 +136,12 @@
             processed_values = []
             for value in values:
                 try:
                     processed_values += arg_to_iter(processor(value))
                 except Exception as e:
                     raise ValueError(
                         "Error in MapCompose with "
-                        f"{str(processor)} values={values} "
+                        f"processor={str(processor)} values={values} & value={value} "
                         f"error='{type(e).__name__}: {str(e)}'"
                     ) from e
             values = processed_values
         return values
```

### Comparing `scrapy_processors-2.0.4/scrapy_processors/common.py` & `scrapy_processors-2.0.5/scrapy_processors/common.py`

 * *Files identical despite different names*

### Comparing `scrapy_processors-2.0.4/scrapy_processors/multi_values.py` & `scrapy_processors-2.0.5/scrapy_processors/multi_values.py`

 * *Files identical despite different names*

### Comparing `scrapy_processors-2.0.4/scrapy_processors/single_value.py` & `scrapy_processors-2.0.5/scrapy_processors/single_value.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,17 +29,17 @@
 import emoji
 import jmespath
 import pytz
 from bs4 import BeautifulSoup
 from phonenumbers import PhoneNumberMatcher, PhoneNumberFormat, format_number
 from price_parser import Price
 from tzlocal import get_localzone
+from misc_utils import arg_to_iter
 
 # Local Imports
-from itemloaders.utils import arg_to_iter
 from scrapy.http import Response
 from scrapy_processors.base import Processor
 
 
 # ... String ...
 def regex_chars(chars: Union[str, Iterable[str]], escape: bool = True) -> str:
     """
```

### Comparing `scrapy_processors-2.0.4/PKG-INFO` & `scrapy_processors-2.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,41 @@
 Metadata-Version: 2.1
 Name: scrapy-processors
-Version: 2.0.4
+Version: 2.0.5
 Summary: Provides processors for the itemloaders package, commonly used with scrapy.
 Home-page: https://github.com/nicholas-mischke/scrapy-processors
 License: MIT
 Keywords: scrapy,itemloaders
 Author: Nicholas Mischke
 Author-email: nmischkework@proton.me
-Requires-Python: >=3.9.0
+Requires-Python: >=3.9.0,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0)
 Requires-Dist: dateparser (>=1.1.8,<2.0.0)
 Requires-Dist: emoji (>=2.2.0,<3.0.0)
 Requires-Dist: itemloaders (>=1.1.0,<2.0.0)
-Requires-Dist: miscellaneous-utils (>=0.3.6,<0.4.0)
+Requires-Dist: miscellaneous-utils (>=0.3.9,<0.4.0)
+Requires-Dist: pendulum (>=3.0.0,<4.0.0)
 Requires-Dist: phonenumbers (>=8.13.17,<9.0.0)
 Requires-Dist: price-parser (>=0.3.4,<0.4.0)
 Requires-Dist: pytz (>=2023.3,<2024.0)
 Requires-Dist: tzlocal (>=5.0.1,<6.0.0)
 Project-URL: Repository, https://github.com/nicholas-mischke/scrapy-processors
 Description-Content-Type: text/markdown
 
 
 # Scrapy Processors
 
 ![License](https://img.shields.io/badge/license-MIT-blue.svg)
-[![Python Versions](https://img.shields.io/badge/Python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue)](https://www.python.org/)
+[![Python Versions](https://img.shields.io/badge/Python-3.9%20%7C%203.10%20%7C%203.11-blue)](https://www.python.org/)
 <!-- [![codecov](https://codecov.io/gh/nicholas-mischke/scrapy-processors/branch/master/graph/badge.svg)](https://codecov.io/gh/nicholas-mischke/scrapy-processors) -->
 
 Scrapy Processors is a collection of Processor classes meant to work with
 the [itemloaders](https://pypi.org/project/itemloaders/) package, commonly used with the [scrapy](https://pypi.org/project/Scrapy/) webscraping framework.
 
 These processors are meant to extend / replace the provided processors in the [itemloaders](https://pypi.org/project/itemloaders/) package.
 
@@ -190,7 +191,8 @@
 
 If you have any questions or need further assistance, feel free to open an issue or reach out to the project maintainers.
 
 Happy contributing!
 
 ## License
 This project is licensed under the MIT License. See the LICENSE file for more details.
+
```

