# Comparing `tmp/pytest_httptesting-0.6.0.tar.gz` & `tmp/pytest_httptesting-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_httptesting-0.6.0.tar", max compression
+gzip compressed data, was "pytest_httptesting-0.7.0.tar", max compression
```

## Comparing `pytest_httptesting-0.6.0.tar` & `pytest_httptesting-0.7.0.tar`

### file list

```diff
@@ -1,18 +1,19 @@
--rw-r--r--   0        0        0     1064 2023-07-24 20:13:18.967621 pytest_httptesting-0.6.0/LICENSE
--rw-r--r--   0        0        0     4049 2023-07-24 20:13:18.967621 pytest_httptesting-0.6.0/README.md
--rw-r--r--   0        0        0      632 2023-07-24 20:13:18.967621 pytest_httptesting-0.6.0/http_testing/__init__.py
--rw-r--r--   0        0        0        0 2023-07-24 20:13:18.967621 pytest_httptesting-0.6.0/http_testing/_assertion_elements/__init__.py
--rw-r--r--   0        0        0      649 2023-07-24 20:13:18.967621 pytest_httptesting-0.6.0/http_testing/_assertion_elements/assert_element_checker_base.py
--rw-r--r--   0        0        0     1392 2023-07-24 20:13:18.967621 pytest_httptesting-0.6.0/http_testing/_assertion_elements/assertion_attribute_base.py
--rw-r--r--   0        0        0     1820 2023-07-24 20:13:18.967621 pytest_httptesting-0.6.0/http_testing/_assertion_elements/assertion_data.py
--rw-r--r--   0        0        0     1608 2023-07-24 20:13:18.967621 pytest_httptesting-0.6.0/http_testing/_assertion_elements/content_assertion.py
--rw-r--r--   0        0        0     2368 2023-07-24 20:13:18.967621 pytest_httptesting-0.6.0/http_testing/_assertion_elements/cookies_assertion.py
--rw-r--r--   0        0        0     1617 2023-07-24 20:13:18.967621 pytest_httptesting-0.6.0/http_testing/_assertion_elements/headers_assertion.py
--rw-r--r--   0        0        0      843 2023-07-24 20:13:18.967621 pytest_httptesting-0.6.0/http_testing/_assertion_elements/status_code_assertion.py
--rw-r--r--   0        0        0     1557 2023-07-24 20:13:18.967621 pytest_httptesting-0.6.0/http_testing/assertions.py
--rw-r--r--   0        0        0      311 2023-07-24 20:13:18.967621 pytest_httptesting-0.6.0/http_testing/cookie.py
--rw-r--r--   0        0        0     2884 2023-07-24 20:13:18.967621 pytest_httptesting-0.6.0/http_testing/page_checker.py
--rw-r--r--   0        0        0      762 2023-07-24 20:13:18.967621 pytest_httptesting-0.6.0/http_testing/plugin.py
--rw-r--r--   0        0        0      745 2023-07-24 20:13:18.967621 pytest_httptesting-0.6.0/http_testing/validators.py
--rw-r--r--   0        0        0      705 2023-07-24 20:13:18.967621 pytest_httptesting-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     4761 1970-01-01 00:00:00.000000 pytest_httptesting-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-05-08 10:41:18.875698 pytest_httptesting-0.7.0/LICENSE
+-rw-r--r--   0        0        0     4049 2024-05-08 10:41:18.875698 pytest_httptesting-0.7.0/README.md
+-rw-r--r--   0        0        0      632 2024-05-08 10:41:18.875698 pytest_httptesting-0.7.0/http_testing/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-08 10:41:18.875698 pytest_httptesting-0.7.0/http_testing/_assertion_elements/__init__.py
+-rw-r--r--   0        0        0      649 2024-05-08 10:41:18.875698 pytest_httptesting-0.7.0/http_testing/_assertion_elements/assert_element_checker_base.py
+-rw-r--r--   0        0        0     1392 2024-05-08 10:41:18.875698 pytest_httptesting-0.7.0/http_testing/_assertion_elements/assertion_attribute_base.py
+-rw-r--r--   0        0        0     1820 2024-05-08 10:41:18.875698 pytest_httptesting-0.7.0/http_testing/_assertion_elements/assertion_data.py
+-rw-r--r--   0        0        0     1715 2024-05-08 10:41:18.875698 pytest_httptesting-0.7.0/http_testing/_assertion_elements/content_assertion.py
+-rw-r--r--   0        0        0     2368 2024-05-08 10:41:18.875698 pytest_httptesting-0.7.0/http_testing/_assertion_elements/cookies_assertion.py
+-rw-r--r--   0        0        0     1617 2024-05-08 10:41:18.875698 pytest_httptesting-0.7.0/http_testing/_assertion_elements/headers_assertion.py
+-rw-r--r--   0        0        0      843 2024-05-08 10:41:18.875698 pytest_httptesting-0.7.0/http_testing/_assertion_elements/status_code_assertion.py
+-rw-r--r--   0        0        0     1647 2024-05-08 10:41:18.879698 pytest_httptesting-0.7.0/http_testing/assertions.py
+-rw-r--r--   0        0        0      311 2024-05-08 10:41:18.879698 pytest_httptesting-0.7.0/http_testing/cookie.py
+-rw-r--r--   0        0        0     2884 2024-05-08 10:41:18.879698 pytest_httptesting-0.7.0/http_testing/page_checker.py
+-rw-r--r--   0        0        0      762 2024-05-08 10:41:18.879698 pytest_httptesting-0.7.0/http_testing/plugin.py
+-rw-r--r--   0        0        0        0 2024-05-08 10:41:18.879698 pytest_httptesting-0.7.0/http_testing/py.typed
+-rw-r--r--   0        0        0      745 2024-05-08 10:41:18.879698 pytest_httptesting-0.7.0/http_testing/validators.py
+-rw-r--r--   0        0        0      843 2024-05-08 10:41:18.879698 pytest_httptesting-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     4812 1970-01-01 00:00:00.000000 pytest_httptesting-0.7.0/PKG-INFO
```

### Comparing `pytest_httptesting-0.6.0/LICENSE` & `pytest_httptesting-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_httptesting-0.6.0/README.md` & `pytest_httptesting-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `pytest_httptesting-0.6.0/http_testing/__init__.py` & `pytest_httptesting-0.7.0/http_testing/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_httptesting-0.6.0/http_testing/_assertion_elements/assert_element_checker_base.py` & `pytest_httptesting-0.7.0/http_testing/_assertion_elements/assert_element_checker_base.py`

 * *Files identical despite different names*

### Comparing `pytest_httptesting-0.6.0/http_testing/_assertion_elements/assertion_attribute_base.py` & `pytest_httptesting-0.7.0/http_testing/_assertion_elements/assertion_attribute_base.py`

 * *Files identical despite different names*

### Comparing `pytest_httptesting-0.6.0/http_testing/_assertion_elements/assertion_data.py` & `pytest_httptesting-0.7.0/http_testing/_assertion_elements/assertion_data.py`

 * *Files identical despite different names*

### Comparing `pytest_httptesting-0.6.0/http_testing/_assertion_elements/content_assertion.py` & `pytest_httptesting-0.7.0/http_testing/_assertion_elements/content_assertion.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,25 +4,26 @@
 from http_testing.validators import Regex, Text, Validator
 
 from .assert_element_checker_base import AssertElementCheckerBase
 from .assertion_attribute_base import AssertionAttributeBase
 from .assertion_data import AssertionData
 
 
-class _ContentChecker(AssertElementCheckerBase[Sequence[Union[str, Validator]]]):
+class _ContentChecker(AssertElementCheckerBase[Union[str, Validator, Sequence[Union[str, Validator]]]]):
     """
     Check the response's content.
     If the given expected value is `str`, first convert it to `validators.Text` validator.
     If the given expected value is a `Regex` validator and its flag is 0, override the flag to `re.MULTILINE`
     """
 
     def check(self, assertion_data: AssertionData, negative: bool) -> None:
         if self.value is None:
             return
-        for expected in self.value:
+        rules = [self.value] if isinstance(self.value, (str, Validator)) else self.value
+        for expected in rules:
             validator: Validator
             if isinstance(expected, str):
                 validator = Text(value=expected)
             elif isinstance(expected, Regex):
                 validator = expected
                 if validator.flags == 0:
                     # prefer multiline mode when search in http content
```

### Comparing `pytest_httptesting-0.6.0/http_testing/_assertion_elements/cookies_assertion.py` & `pytest_httptesting-0.7.0/http_testing/_assertion_elements/cookies_assertion.py`

 * *Files identical despite different names*

### Comparing `pytest_httptesting-0.6.0/http_testing/_assertion_elements/headers_assertion.py` & `pytest_httptesting-0.7.0/http_testing/_assertion_elements/headers_assertion.py`

 * *Files identical despite different names*

### Comparing `pytest_httptesting-0.6.0/http_testing/_assertion_elements/status_code_assertion.py` & `pytest_httptesting-0.7.0/http_testing/_assertion_elements/status_code_assertion.py`

 * *Files identical despite different names*

### Comparing `pytest_httptesting-0.6.0/http_testing/assertions.py` & `pytest_httptesting-0.7.0/http_testing/assertions.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 from abc import ABC
-from typing import Mapping, Optional, Sequence
+from typing import Mapping, Optional, Sequence, Union
 
 from httpx import Client, Response
 
 from http_testing._assertion_elements.assertion_attribute_base import check_all
 from http_testing._assertion_elements.assertion_data import AssertionData
 from http_testing._assertion_elements.content_assertion import ContentAssertion
 from http_testing._assertion_elements.cookies_assertion import Cookie, CookiesAssertion
 from http_testing._assertion_elements.headers_assertion import HeadersAssertion
 from http_testing._assertion_elements.status_code_assertion import StatusCodeAssertion
+from http_testing.validators import Validator
 
 
 class _AssertionsBase(ABC):
     _negative: bool = False
     status_code = StatusCodeAssertion()
     content = ContentAssertion()
     headers = HeadersAssertion()
     cookies = CookiesAssertion()
 
     def __init__(
         self,
         status_code: Optional[int] = None,
-        content: Optional[Sequence[str]] = None,
+        content: Union[None, str, Validator, Sequence[Union[str, Validator]]] = None,
         headers: Optional[Mapping[str, str]] = None,
         cookies: Optional[Sequence[Cookie]] = None,
     ):
         self.status_code = status_code
         self.content = content
         self.headers = headers
         self.cookies = cookies
```

### Comparing `pytest_httptesting-0.6.0/http_testing/page_checker.py` & `pytest_httptesting-0.7.0/http_testing/page_checker.py`

 * *Files identical despite different names*

### Comparing `pytest_httptesting-0.6.0/http_testing/plugin.py` & `pytest_httptesting-0.7.0/http_testing/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest_httptesting-0.6.0/http_testing/validators.py` & `pytest_httptesting-0.7.0/http_testing/validators.py`

 * *Files identical despite different names*

### Comparing `pytest_httptesting-0.6.0/pyproject.toml` & `pytest_httptesting-0.7.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,41 @@
 [tool.poetry]
 name = "pytest-httptesting"
-version = "0.6.0"
+version = "0.7.0"
 description = "http_testing framework on top of pytest"
 authors = ["HE Qile <mr.qile@gmail.com>"]
 readme = "README.md"
-packages = [{include = "http_testing"}]
+packages = [
+    {include = "http_testing"},
+    {include = "http_testing/py.typed"},
+]
 
 homepage = "https://github.com/heqile/http_testing"
 repository = "https://github.com/heqile/http_testing"
 
 include = ["LICENSE"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-pytest = "^7.2.0"
-httpx = "^0.24.0"
+pytest = "^8.2.0"
+httpx = "^0.27.0"
 attrs = "^23.1.0"
 
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^3.1.1"
 mypy = "^1.1.1"
-black = "^23.1.0"
+black = "^24.4.2"
+ruff = "^0.4.3"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.plugins."pytest11"]
 "http_page_checker" = "http_testing.plugin"
+
+[tool.ruff]
+line-length = 120
+
+[tool.mypy]
+ignore_missing_imports = true
```

### Comparing `pytest_httptesting-0.6.0/PKG-INFO` & `pytest_httptesting-0.7.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: pytest-httptesting
-Version: 0.6.0
+Version: 0.7.0
 Summary: http_testing framework on top of pytest
 Home-page: https://github.com/heqile/http_testing
 Author: HE Qile
 Author-email: mr.qile@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: attrs (>=23.1.0,<24.0.0)
-Requires-Dist: httpx (>=0.24.0,<0.25.0)
-Requires-Dist: pytest (>=7.2.0,<8.0.0)
+Requires-Dist: httpx (>=0.27.0,<0.28.0)
+Requires-Dist: pytest (>=8.2.0,<9.0.0)
 Project-URL: Repository, https://github.com/heqile/http_testing
 Description-Content-Type: text/markdown
 
 # HTTP_TESTING
 
 <a href="https://github.com/heqile/http_testing/actions?query=branch%3Amain+event%3Apush+" target="_blank">
     <img src="https://github.com/heqile/http_testing/workflows/Test/badge.svg?event=push&branch=main" alt="Test">
```

