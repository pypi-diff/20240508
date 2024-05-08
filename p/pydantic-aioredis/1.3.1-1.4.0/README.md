# Comparing `tmp/pydantic_aioredis-1.3.1.tar.gz` & `tmp/pydantic_aioredis-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_aioredis-1.3.1.tar", max compression
+gzip compressed data, was "pydantic_aioredis-1.4.0.tar", max compression
```

## Comparing `pydantic_aioredis-1.3.1.tar` & `pydantic_aioredis-1.4.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1262 2024-05-05 21:04:05.059033 pydantic_aioredis-1.3.1/LICENSE
--rw-r--r--   0        0        0     9916 2024-05-05 21:04:05.059033 pydantic_aioredis-1.3.1/README.md
--rw-r--r--   0        0        0      338 2024-05-05 21:04:05.059033 pydantic_aioredis-1.3.1/pydantic_aioredis/__init__.py
--rw-r--r--   0        0        0     4988 2024-05-05 21:04:05.059033 pydantic_aioredis-1.3.1/pydantic_aioredis/abstract.py
--rw-r--r--   0        0        0      757 2024-05-05 21:04:05.059033 pydantic_aioredis-1.3.1/pydantic_aioredis/config.py
--rw-r--r--   0        0        0      442 2024-05-05 21:04:05.059033 pydantic_aioredis-1.3.1/pydantic_aioredis/ext/FastAPI/__init__.py
--rw-r--r--   0        0        0     4026 2024-05-05 21:04:05.059033 pydantic_aioredis-1.3.1/pydantic_aioredis/ext/FastAPI/crudrouter.py
--rw-r--r--   0        0        0      960 2024-05-05 21:04:05.059033 pydantic_aioredis-1.3.1/pydantic_aioredis/ext/FastAPI/model.py
--rw-r--r--   0        0        0        0 2024-05-05 21:04:05.059033 pydantic_aioredis-1.3.1/pydantic_aioredis/ext/__init__.py
--rw-r--r--   0        0        0     9705 2024-05-05 21:04:05.059033 pydantic_aioredis-1.3.1/pydantic_aioredis/model.py
--rw-r--r--   0        0        0     1581 2024-05-05 21:04:05.059033 pydantic_aioredis-1.3.1/pydantic_aioredis/store.py
--rw-r--r--   0        0        0     1087 2024-05-05 21:04:05.059033 pydantic_aioredis-1.3.1/pydantic_aioredis/types.py
--rw-r--r--   0        0        0      178 2024-05-05 21:04:05.059033 pydantic_aioredis-1.3.1/pydantic_aioredis/utils.py
--rw-r--r--   0        0        0     2679 2024-05-05 21:04:05.059033 pydantic_aioredis-1.3.1/pyproject.toml
--rw-r--r--   0        0        0    11428 1970-01-01 00:00:00.000000 pydantic_aioredis-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1262 2024-05-08 00:27:26.727370 pydantic_aioredis-1.4.0/LICENSE
+-rw-r--r--   0        0        0    10311 2024-05-08 00:27:26.727370 pydantic_aioredis-1.4.0/README.md
+-rw-r--r--   0        0        0      338 2024-05-08 00:27:26.727370 pydantic_aioredis-1.4.0/pydantic_aioredis/__init__.py
+-rw-r--r--   0        0        0     4988 2024-05-08 00:27:26.727370 pydantic_aioredis-1.4.0/pydantic_aioredis/abstract.py
+-rw-r--r--   0        0        0      757 2024-05-08 00:27:26.727370 pydantic_aioredis-1.4.0/pydantic_aioredis/config.py
+-rw-r--r--   0        0        0      442 2024-05-08 00:27:26.727370 pydantic_aioredis-1.4.0/pydantic_aioredis/ext/FastAPI/__init__.py
+-rw-r--r--   0        0        0     4026 2024-05-08 00:27:26.727370 pydantic_aioredis-1.4.0/pydantic_aioredis/ext/FastAPI/crudrouter.py
+-rw-r--r--   0        0        0      960 2024-05-08 00:27:26.727370 pydantic_aioredis-1.4.0/pydantic_aioredis/ext/FastAPI/model.py
+-rw-r--r--   0        0        0        0 2024-05-08 00:27:26.727370 pydantic_aioredis-1.4.0/pydantic_aioredis/ext/__init__.py
+-rw-r--r--   0        0        0     9705 2024-05-08 00:27:26.727370 pydantic_aioredis-1.4.0/pydantic_aioredis/model.py
+-rw-r--r--   0        0        0     1581 2024-05-08 00:27:26.727370 pydantic_aioredis-1.4.0/pydantic_aioredis/store.py
+-rw-r--r--   0        0        0     1087 2024-05-08 00:27:26.727370 pydantic_aioredis-1.4.0/pydantic_aioredis/types.py
+-rw-r--r--   0        0        0    11528 2024-05-08 00:27:26.727370 pydantic_aioredis-1.4.0/pydantic_aioredis/utils.py
+-rw-r--r--   0        0        0     2680 2024-05-08 00:27:26.727370 pydantic_aioredis-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0    11778 1970-01-01 00:00:00.000000 pydantic_aioredis-1.4.0/PKG-INFO
```

### Comparing `pydantic_aioredis-1.3.1/LICENSE` & `pydantic_aioredis-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_aioredis-1.3.1/README.md` & `pydantic_aioredis-1.4.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -156,14 +156,17 @@
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/Tinitto"><img src="https://avatars.githubusercontent.com/u/21363733??v=4?s=100" width="100px;" alt="Martin Ahindura"/><br /><sub><b>Martin Ahindura</b></sub></a><br /><a href="https://github.com/andrewthetechie/pydantic-aioredis/commits?author=Tinitto" title="Code">💻</a> <a href="#ideas-Tinitto" title="Ideas, Planning, & Feedback">🤔</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/david-wahlstedt"><img src="https://avatars.githubusercontent.com/u/66391333?v=4?s=100" width="100px;" alt="david-wahlstedt"/><br /><sub><b>david-wahlstedt</b></sub></a><br /><a href="https://github.com/andrewthetechie/pydantic-aioredis/commits?author=david-wahlstedt" title="Tests">⚠️</a> <a href="https://github.com/andrewthetechie/pydantic-aioredis/commits?author=david-wahlstedt" title="Documentation">📖</a> <a href="https://github.com/andrewthetechie/pydantic-aioredis/pulls?q=is%3Apr+reviewed-by%3Adavid-wahlstedt" title="Reviewed Pull Requests">👀</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://blog.gtmanfred.com"><img src="https://avatars.githubusercontent.com/u/732321?v=4?s=100" width="100px;" alt="Daniel Wallace"/><br /><sub><b>Daniel Wallace</b></sub></a><br /><a href="https://github.com/andrewthetechie/pydantic-aioredis/commits?author=gtmanfred" title="Tests">⚠️</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://derwen.ai/paco"><img src="https://avatars.githubusercontent.com/u/57973?v=4?s=100" width="100px;" alt="Paco Nathan"/><br /><sub><b>Paco Nathan</b></sub></a><br /><a href="#example-ceteri" title="Examples">💡</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://www.linkedin.com/in/andreas-brodersen-1b955b100/"><img src="https://avatars.githubusercontent.com/u/43907402?v=4?s=100" width="100px;" alt="Andreas Brodersen"/><br /><sub><b>Andreas Brodersen</b></sub></a><br /><a href="https://github.com/andrewthetechie/pydantic-aioredis/commits?author=AndreasPB" title="Documentation">📖</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/kraczak"><img src="https://avatars.githubusercontent.com/u/58468064?v=4?s=100" width="100px;" alt="kraczak"/><br /><sub><b>kraczak</b></sub></a><br /><a href="https://github.com/andrewthetechie/pydantic-aioredis/commits?author=kraczak" title="Documentation">📖</a></td>
     </tr>
+    <tr>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/CharlieJiangXXX"><img src="https://avatars.githubusercontent.com/u/45895922?v=4?s=100" width="100px;" alt="CharlieJiangXXX"/><br /><sub><b>CharlieJiangXXX</b></sub></a><br /><a href="https://github.com/andrewthetechie/pydantic-aioredis/commits?author=CharlieJiangXXX" title="Code">💻</a></td>
+    </tr>
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
 
 <!-- ALL-CONTRIBUTORS-LIST:END -->
```

### Comparing `pydantic_aioredis-1.3.1/pydantic_aioredis/abstract.py` & `pydantic_aioredis-1.4.0/pydantic_aioredis/abstract.py`

 * *Files identical despite different names*

### Comparing `pydantic_aioredis-1.3.1/pydantic_aioredis/config.py` & `pydantic_aioredis-1.4.0/pydantic_aioredis/config.py`

 * *Files identical despite different names*

### Comparing `pydantic_aioredis-1.3.1/pydantic_aioredis/ext/FastAPI/crudrouter.py` & `pydantic_aioredis-1.4.0/pydantic_aioredis/ext/FastAPI/crudrouter.py`

 * *Files identical despite different names*

### Comparing `pydantic_aioredis-1.3.1/pydantic_aioredis/ext/FastAPI/model.py` & `pydantic_aioredis-1.4.0/pydantic_aioredis/ext/FastAPI/model.py`

 * *Files identical despite different names*

### Comparing `pydantic_aioredis-1.3.1/pydantic_aioredis/model.py` & `pydantic_aioredis-1.4.0/pydantic_aioredis/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,17 +6,16 @@
 from sys import version_info
 from typing import Any
 from typing import List
 from typing import Optional
 from typing import Tuple
 from typing import Union
 
-import nest_asyncio
 from pydantic_aioredis.abstract import _AbstractModel
-from pydantic_aioredis.utils import bytes_to_string
+from pydantic_aioredis.utils import bytes_to_string, NestedAsyncIO
 
 
 class Model(_AbstractModel):
     """
     The section in the store that saves rows of the same kind
 
     Model has some custom fields you can set in your models that alter the behavior of how this is stored in redis
@@ -65,16 +64,16 @@
             # equal or greater than 3.10.0
             try:
                 io_loop = asyncio.get_running_loop()
                 # https://github.com/erdewit/nest_asyncio
                 # Use nest_asyncio so we can call the async save
             except RuntimeError:
                 io_loop = asyncio.new_event_loop()
-        nest_asyncio.apply()
-        io_loop.run_until_complete(self.save())
+        with NestedAsyncIO():
+            io_loop.run_until_complete(self.save())
 
     @asynccontextmanager
     async def update(self):
         """
         Async Context manager to allow for updating multiple fields without syncing to redis until the end
         """
         auto_sync = self.auto_sync
```

### Comparing `pydantic_aioredis-1.3.1/pydantic_aioredis/store.py` & `pydantic_aioredis-1.4.0/pydantic_aioredis/store.py`

 * *Files identical despite different names*

### Comparing `pydantic_aioredis-1.3.1/pydantic_aioredis/types.py` & `pydantic_aioredis-1.4.0/pydantic_aioredis/types.py`

 * *Files identical despite different names*

### Comparing `pydantic_aioredis-1.3.1/pyproject.toml` & `pydantic_aioredis-1.4.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydantic-aioredis"
-version = "1.3.1"
+version = "1.4.0"
 description = "Use your pydantic models as an ORM, storing data in Redis."
 authors = ["Andrew Herrington <andrew.the.techie@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/andrewthetechie/pydantic-aioredis"
 repository = "https://github.com/andrewthetechie/pydantic-aioredis"
 documentation = "https://pydantic-aioredis.readthedocs.io/en/latest/"
@@ -23,32 +23,31 @@
 
 [tool.poetry.urls]
 Changelog = "https://github.com/andrewthetechie/pydantic-aioredis/releases"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 pydantic = "^1.10.2"
-redis = "^4.4.4"
-anyio = "^3.6.2"
-nest-asyncio = "^1.5.6"
+redis = ">=4.4.4,<6.0.0"
+anyio = ">=3.6.2,<5.0.0"
 fastapi = {version = ">=0.110", optional = true}
 fastapi-crudrouter = {version = "^0.8.6", optional = true}
 
 [tool.poetry.extras]
 FastAPI= ['fastapi']
 fastapi-crudrouter=['fastapi-crudrouter']
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.0"
 coverage = {extras = ["toml"], version = ">=6.5,<8.0"}
 safety = ">=2.3.1,<4.0.0"
-mypy = ">=0.991,<1.5"
+mypy = ">=0.991,<1.11"
 xdoctest = {extras = ["colors"], version = "^1.1.0"}
-sphinx = ">=4.3.2,<6.0.0"
+sphinx = ">=4.3.2,<8.0.0"
 sphinx-autobuild = ">=2021.3.14"
 pre-commit = ">=2.12.1"
 pep8-naming = "^0.13.2"
 reorder-python-imports = "^3.9.0"
 pre-commit-hooks = "^4.2.0"
 Pygments = "^2.13.0"
 pyupgrade = "^3.3.1"
@@ -58,18 +57,18 @@
 pytest_async = "^0.1.1"
 pytest-asyncio = ">=0.20.1,<0.22.0"
 pytest-mock = "^3.10.0"
 pytest-lazy-fixture = "^0.6.3"
 fastapi = ">=0.6.3"
 fastapi-crudrouter = ">=0.8.4"
 httpx = ">=0.23,<0.28"
-pytest-env = "^0.8.1"
+pytest-env = ">=0.8.1,<1.2.0"
 pytest-xdist = "^3.1.0"
 bandit = "^1.7.8"
-fakeredis = {extras = ["json"], version = "2.22.0"}
+fakeredis = {extras = ["json"], version = "2.23.0"}
 hypothesis = "^6.61.0"
 pytest-rerunfailures = ">=11.1,<15.0"
 ruff = "^0.4.2"
 
 [tool.mypy]
 strict = true
 warn_unreachable = true
@@ -82,12 +81,12 @@
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.bandit]
 exclude_dirs = ["test", "noxfile.py", ".github/scripts", "dist", "examples/*"]
 
 [tool.pytest.ini_options]
-addopts = "-n 4 --ignore examples --cov=pydantic_aioredis --cov-report xml:.coverage.xml --cov-report=term-missing --cov-fail-under 91"
+addopts = "-n 4 --ignore examples --cov=pydantic_aioredis --cov-report xml:.coverage.xml --cov-report=term-missing --cov-fail-under 85"
 
 [tool.ruff]
 line-length = 120
-target-version = "py37"
+target-version = "py38"
```

### Comparing `pydantic_aioredis-1.3.1/PKG-INFO` & `pydantic_aioredis-1.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-aioredis
-Version: 1.3.1
+Version: 1.4.0
 Summary: Use your pydantic models as an ORM, storing data in Redis.
 Home-page: https://github.com/andrewthetechie/pydantic-aioredis
 License: MIT
 Author: Andrew Herrington
 Author-email: andrew.the.techie@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -17,20 +17,19 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.7
 Provides-Extra: fastapi
 Provides-Extra: fastapi-crudrouter
-Requires-Dist: anyio (>=3.6.2,<4.0.0)
+Requires-Dist: anyio (>=3.6.2,<5.0.0)
 Requires-Dist: fastapi (>=0.110) ; extra == "fastapi"
 Requires-Dist: fastapi-crudrouter (>=0.8.6,<0.9.0) ; extra == "fastapi-crudrouter"
-Requires-Dist: nest-asyncio (>=1.5.6,<2.0.0)
 Requires-Dist: pydantic (>=1.10.2,<2.0.0)
-Requires-Dist: redis (>=4.4.4,<5.0.0)
+Requires-Dist: redis (>=4.4.4,<6.0.0)
 Project-URL: Changelog, https://github.com/andrewthetechie/pydantic-aioredis/releases
 Project-URL: Documentation, https://pydantic-aioredis.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/andrewthetechie/pydantic-aioredis
 Description-Content-Type: text/markdown
 
 # pydantic-aioredis
 
@@ -190,14 +189,17 @@
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/Tinitto"><img src="https://avatars.githubusercontent.com/u/21363733??v=4?s=100" width="100px;" alt="Martin Ahindura"/><br /><sub><b>Martin Ahindura</b></sub></a><br /><a href="https://github.com/andrewthetechie/pydantic-aioredis/commits?author=Tinitto" title="Code">💻</a> <a href="#ideas-Tinitto" title="Ideas, Planning, & Feedback">🤔</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/david-wahlstedt"><img src="https://avatars.githubusercontent.com/u/66391333?v=4?s=100" width="100px;" alt="david-wahlstedt"/><br /><sub><b>david-wahlstedt</b></sub></a><br /><a href="https://github.com/andrewthetechie/pydantic-aioredis/commits?author=david-wahlstedt" title="Tests">⚠️</a> <a href="https://github.com/andrewthetechie/pydantic-aioredis/commits?author=david-wahlstedt" title="Documentation">📖</a> <a href="https://github.com/andrewthetechie/pydantic-aioredis/pulls?q=is%3Apr+reviewed-by%3Adavid-wahlstedt" title="Reviewed Pull Requests">👀</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://blog.gtmanfred.com"><img src="https://avatars.githubusercontent.com/u/732321?v=4?s=100" width="100px;" alt="Daniel Wallace"/><br /><sub><b>Daniel Wallace</b></sub></a><br /><a href="https://github.com/andrewthetechie/pydantic-aioredis/commits?author=gtmanfred" title="Tests">⚠️</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://derwen.ai/paco"><img src="https://avatars.githubusercontent.com/u/57973?v=4?s=100" width="100px;" alt="Paco Nathan"/><br /><sub><b>Paco Nathan</b></sub></a><br /><a href="#example-ceteri" title="Examples">💡</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://www.linkedin.com/in/andreas-brodersen-1b955b100/"><img src="https://avatars.githubusercontent.com/u/43907402?v=4?s=100" width="100px;" alt="Andreas Brodersen"/><br /><sub><b>Andreas Brodersen</b></sub></a><br /><a href="https://github.com/andrewthetechie/pydantic-aioredis/commits?author=AndreasPB" title="Documentation">📖</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/kraczak"><img src="https://avatars.githubusercontent.com/u/58468064?v=4?s=100" width="100px;" alt="kraczak"/><br /><sub><b>kraczak</b></sub></a><br /><a href="https://github.com/andrewthetechie/pydantic-aioredis/commits?author=kraczak" title="Documentation">📖</a></td>
     </tr>
+    <tr>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/CharlieJiangXXX"><img src="https://avatars.githubusercontent.com/u/45895922?v=4?s=100" width="100px;" alt="CharlieJiangXXX"/><br /><sub><b>CharlieJiangXXX</b></sub></a><br /><a href="https://github.com/andrewthetechie/pydantic-aioredis/commits?author=CharlieJiangXXX" title="Code">💻</a></td>
+    </tr>
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
 
 <!-- ALL-CONTRIBUTORS-LIST:END -->
```

