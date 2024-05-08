# Comparing `tmp/tmdsclient-0.2.1.tar.gz` & `tmp/tmdsclient-0.2.2.tar.gz`

## Comparing `tmdsclient-0.2.1.tar` & `tmdsclient-0.2.2.tar`

### file list

```diff
@@ -1,53 +1,55 @@
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 tmdsclient-0.2.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     2423 2020-02-02 00:00:00.000000 tmdsclient-0.2.1/README.md
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 tmdsclient-0.2.1/domain-specific-terms.txt
--rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 tmdsclient-0.2.1/requirements.txt
--rw-r--r--   0        0        0     2753 2020-02-02 00:00:00.000000 tmdsclient-0.2.1/tox.ini
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 tmdsclient-0.2.1/.github/dependabot.yml
--rw-r--r--   0        0        0     2378 2020-02-02 00:00:00.000000 tmdsclient-0.2.1/.github/workflows/codeql-analysis.yml
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 tmdsclient-0.2.1/.github/workflows/coverage.yml
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 tmdsclient-0.2.1/.github/workflows/dependabot_automerge.yml
--rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 tmdsclient-0.2.1/.github/workflows/dev_test.yml
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 tmdsclient-0.2.1/.github/workflows/formatting.yml
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 tmdsclient-0.2.1/.github/workflows/no_byte_order_mark.yml
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 tmdsclient-0.2.1/.github/workflows/packaging_test.yml
--rw-r--r--   0        0        0     2512 2020-02-02 00:00:00.000000 tmdsclient-0.2.1/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 tmdsclient-0.2.1/.github/workflows/pythonlint.yml
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 tmdsclient-0.2.1/.github/workflows/unittests.yml
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 tmdsclient-0.2.1/dev_requirements/requirements-coverage.in
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 tmdsclient-0.2.1/dev_requirements/requirements-coverage.txt
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 tmdsclient-0.2.1/dev_requirements/requirements-formatting.in
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 tmdsclient-0.2.1/dev_requirements/requirements-formatting.txt
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 tmdsclient-0.2.1/dev_requirements/requirements-linting.in
--rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 tmdsclient-0.2.1/dev_requirements/requirements-linting.txt
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 tmdsclient-0.2.1/dev_requirements/requirements-packaging.in
--rw-r--r--   0        0        0     1458 2020-02-02 00:00:00.000000 tmdsclient-0.2.1/dev_requirements/requirements-packaging.txt
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 tmdsclient-0.2.1/dev_requirements/requirements-spell_check.in
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 tmdsclient-0.2.1/dev_requirements/requirements-spell_check.txt
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 tmdsclient-0.2.1/dev_requirements/requirements-tests.in
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 tmdsclient-0.2.1/dev_requirements/requirements-tests.txt
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 tmdsclient-0.2.1/dev_requirements/requirements-type_check.in
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 tmdsclient-0.2.1/dev_requirements/requirements-type_check.txt
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 tmdsclient-0.2.1/src/_tmdsclient_version.py
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 tmdsclient-0.2.1/src/tmdsclient/__init__.py
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 tmdsclient-0.2.1/src/tmdsclient/py.typed
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 tmdsclient-0.2.1/src/tmdsclient/client/__init__.py
--rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 tmdsclient-0.2.1/src/tmdsclient/client/config.py
--rw-r--r--   0        0        0    16026 2020-02-02 00:00:00.000000 tmdsclient-0.2.1/src/tmdsclient/client/tmdsclient.py
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 tmdsclient-0.2.1/src/tmdsclient/models/__init__.py
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 tmdsclient-0.2.1/src/tmdsclient/models/bo4e_stub.py
--rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 tmdsclient-0.2.1/src/tmdsclient/models/messlokation.py
--rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 tmdsclient-0.2.1/src/tmdsclient/models/netzvertrag.py
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 tmdsclient-0.2.1/src/tmdsclient/models/partneradresse.py
--rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 tmdsclient-0.2.1/src/tmdsclient/models/patches.py
--rw-r--r--   0        0        0     2496 2020-02-02 00:00:00.000000 tmdsclient-0.2.1/src/tmdsclient/models/utils.py
--rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 tmdsclient-0.2.1/src/tmdsclient/models/zaehler.py
--rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 tmdsclient-0.2.1/src/tmdsclient/models/zaehler_bo_model.py
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 tmdsclient-0.2.1/src/tmdsclient/models/zaehlergroesse.py
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 tmdsclient-0.2.1/src/tmdsclient/models/zaehlerhersteller.py
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 tmdsclient-0.2.1/src/tmdsclient/models/zaehlwerk.py
--rw-r--r--   0        0        0     3160 2020-02-02 00:00:00.000000 tmdsclient-0.2.1/src/tmdsclient/models/zeitscheibe.py
--rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 tmdsclient-0.2.1/.gitignore
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 tmdsclient-0.2.1/LICENSE
--rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 tmdsclient-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     3508 2020-02-02 00:00:00.000000 tmdsclient-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 tmdsclient-0.2.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     2423 2020-02-02 00:00:00.000000 tmdsclient-0.2.2/README.md
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 tmdsclient-0.2.2/domain-specific-terms.txt
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 tmdsclient-0.2.2/requirements.txt
+-rw-r--r--   0        0        0     2753 2020-02-02 00:00:00.000000 tmdsclient-0.2.2/tox.ini
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 tmdsclient-0.2.2/.github/dependabot.yml
+-rw-r--r--   0        0        0     2378 2020-02-02 00:00:00.000000 tmdsclient-0.2.2/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 tmdsclient-0.2.2/.github/workflows/coverage.yml
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 tmdsclient-0.2.2/.github/workflows/dependabot_automerge.yml
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 tmdsclient-0.2.2/.github/workflows/dev_test.yml
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 tmdsclient-0.2.2/.github/workflows/formatting.yml
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 tmdsclient-0.2.2/.github/workflows/no_byte_order_mark.yml
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 tmdsclient-0.2.2/.github/workflows/packaging_test.yml
+-rw-r--r--   0        0        0     2512 2020-02-02 00:00:00.000000 tmdsclient-0.2.2/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 tmdsclient-0.2.2/.github/workflows/pythonlint.yml
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 tmdsclient-0.2.2/.github/workflows/unittests.yml
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 tmdsclient-0.2.2/dev_requirements/requirements-coverage.in
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 tmdsclient-0.2.2/dev_requirements/requirements-coverage.txt
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 tmdsclient-0.2.2/dev_requirements/requirements-formatting.in
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 tmdsclient-0.2.2/dev_requirements/requirements-formatting.txt
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 tmdsclient-0.2.2/dev_requirements/requirements-linting.in
+-rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 tmdsclient-0.2.2/dev_requirements/requirements-linting.txt
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 tmdsclient-0.2.2/dev_requirements/requirements-packaging.in
+-rw-r--r--   0        0        0     1458 2020-02-02 00:00:00.000000 tmdsclient-0.2.2/dev_requirements/requirements-packaging.txt
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 tmdsclient-0.2.2/dev_requirements/requirements-spell_check.in
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 tmdsclient-0.2.2/dev_requirements/requirements-spell_check.txt
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 tmdsclient-0.2.2/dev_requirements/requirements-tests.in
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 tmdsclient-0.2.2/dev_requirements/requirements-tests.txt
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 tmdsclient-0.2.2/dev_requirements/requirements-type_check.in
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 tmdsclient-0.2.2/dev_requirements/requirements-type_check.txt
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 tmdsclient-0.2.2/src/_tmdsclient_version.py
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 tmdsclient-0.2.2/src/tmdsclient/__init__.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 tmdsclient-0.2.2/src/tmdsclient/py.typed
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 tmdsclient-0.2.2/src/tmdsclient/client/__init__.py
+-rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 tmdsclient-0.2.2/src/tmdsclient/client/config.py
+-rw-r--r--   0        0        0    18439 2020-02-02 00:00:00.000000 tmdsclient-0.2.2/src/tmdsclient/client/tmdsclient.py
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 tmdsclient-0.2.2/src/tmdsclient/models/__init__.py
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 tmdsclient-0.2.2/src/tmdsclient/models/adresse.py
+-rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 tmdsclient-0.2.2/src/tmdsclient/models/anschlussobjekt.py
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 tmdsclient-0.2.2/src/tmdsclient/models/bo4e_stub.py
+-rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 tmdsclient-0.2.2/src/tmdsclient/models/messlokation.py
+-rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 tmdsclient-0.2.2/src/tmdsclient/models/netzvertrag.py
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 tmdsclient-0.2.2/src/tmdsclient/models/partneradresse.py
+-rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 tmdsclient-0.2.2/src/tmdsclient/models/patches.py
+-rw-r--r--   0        0        0     2496 2020-02-02 00:00:00.000000 tmdsclient-0.2.2/src/tmdsclient/models/utils.py
+-rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 tmdsclient-0.2.2/src/tmdsclient/models/zaehler.py
+-rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 tmdsclient-0.2.2/src/tmdsclient/models/zaehler_bo_model.py
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 tmdsclient-0.2.2/src/tmdsclient/models/zaehlergroesse.py
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 tmdsclient-0.2.2/src/tmdsclient/models/zaehlerhersteller.py
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 tmdsclient-0.2.2/src/tmdsclient/models/zaehlwerk.py
+-rw-r--r--   0        0        0     3160 2020-02-02 00:00:00.000000 tmdsclient-0.2.2/src/tmdsclient/models/zeitscheibe.py
+-rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 tmdsclient-0.2.2/.gitignore
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 tmdsclient-0.2.2/LICENSE
+-rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 tmdsclient-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     3508 2020-02-02 00:00:00.000000 tmdsclient-0.2.2/PKG-INFO
```

### Comparing `tmdsclient-0.2.1/.pre-commit-config.yaml` & `tmdsclient-0.2.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `tmdsclient-0.2.1/README.md` & `tmdsclient-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `tmdsclient-0.2.1/requirements.txt` & `tmdsclient-0.2.2/requirements.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 #
 # This file is autogenerated by pip-compile with Python 3.11
 # by the following command:
 #
 #    pip-compile pyproject.toml
 #
+aiodns==3.2.0
+    # via aiohttp
 aiohttp[speedups]==3.9.5
     # via tmdsclient (pyproject.toml)
 aiosignal==1.3.1
     # via aiohttp
 annotated-types==0.6.0
     # via pydantic
 attrs==23.2.0
     # via aiohttp
 bo4e==202401.1.1
     # via tmdsclient (pyproject.toml)
 brotli==1.1.0
     # via aiohttp
+cffi==1.16.0
+    # via pycares
 frozenlist==1.4.1
     # via
     #   aiohttp
     #   aiosignal
 idna==3.7
     # via yarl
 iso3166==2.1.1
@@ -30,14 +34,18 @@
     # via jsonpatch
 more-itertools==10.2.0
     # via tmdsclient (pyproject.toml)
 multidict==6.0.5
     # via
     #   aiohttp
     #   yarl
+pycares==4.4.0
+    # via aiodns
+pycparser==2.22
+    # via cffi
 pydantic==2.7.1
     # via
     #   bo4e
     #   tmdsclient (pyproject.toml)
 pydantic-core==2.18.2
     # via pydantic
 pyhumps==3.8.0
```

### Comparing `tmdsclient-0.2.1/tox.ini` & `tmdsclient-0.2.2/tox.ini`

 * *Files identical despite different names*

### Comparing `tmdsclient-0.2.1/.github/dependabot.yml` & `tmdsclient-0.2.2/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `tmdsclient-0.2.1/.github/workflows/codeql-analysis.yml` & `tmdsclient-0.2.2/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `tmdsclient-0.2.1/.github/workflows/coverage.yml` & `tmdsclient-0.2.2/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `tmdsclient-0.2.1/.github/workflows/dependabot_automerge.yml` & `tmdsclient-0.2.2/.github/workflows/dependabot_automerge.yml`

 * *Files identical despite different names*

### Comparing `tmdsclient-0.2.1/.github/workflows/dev_test.yml` & `tmdsclient-0.2.2/.github/workflows/dev_test.yml`

 * *Files identical despite different names*

### Comparing `tmdsclient-0.2.1/.github/workflows/formatting.yml` & `tmdsclient-0.2.2/.github/workflows/formatting.yml`

 * *Files identical despite different names*

### Comparing `tmdsclient-0.2.1/.github/workflows/packaging_test.yml` & `tmdsclient-0.2.2/.github/workflows/packaging_test.yml`

 * *Files identical despite different names*

### Comparing `tmdsclient-0.2.1/.github/workflows/python-publish.yml` & `tmdsclient-0.2.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `tmdsclient-0.2.1/.github/workflows/pythonlint.yml` & `tmdsclient-0.2.2/.github/workflows/pythonlint.yml`

 * *Files identical despite different names*

### Comparing `tmdsclient-0.2.1/.github/workflows/unittests.yml` & `tmdsclient-0.2.2/.github/workflows/unittests.yml`

 * *Files identical despite different names*

### Comparing `tmdsclient-0.2.1/dev_requirements/requirements-linting.txt` & `tmdsclient-0.2.2/dev_requirements/requirements-linting.txt`

 * *Files identical despite different names*

### Comparing `tmdsclient-0.2.1/dev_requirements/requirements-packaging.txt` & `tmdsclient-0.2.2/dev_requirements/requirements-packaging.txt`

 * *Files identical despite different names*

### Comparing `tmdsclient-0.2.1/dev_requirements/requirements-tests.txt` & `tmdsclient-0.2.2/dev_requirements/requirements-tests.txt`

 * *Files identical despite different names*

### Comparing `tmdsclient-0.2.1/src/tmdsclient/client/config.py` & `tmdsclient-0.2.2/src/tmdsclient/client/config.py`

 * *Files identical despite different names*

### Comparing `tmdsclient-0.2.1/src/tmdsclient/client/tmdsclient.py` & `tmdsclient-0.2.2/src/tmdsclient/client/tmdsclient.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """contains the actual client"""
 
 import asyncio
 import logging
 import uuid
+from datetime import datetime, timedelta
 from typing import AsyncGenerator, Callable, Literal, Optional, overload
 
 from aiohttp import BasicAuth, ClientResponseError, ClientSession, ClientTimeout
 from more_itertools import chunked
 from yarl import URL
 
 from tmdsclient.client.config import TmdsConfig
@@ -29,15 +30,15 @@
         chunk_idx + 1,
         total_size // chunk_size + 1,
     )
 
 
 _retry_worthy_http_status_codes = {500, 502}
 """
-if a GET request fails with one of these status codes, it might be worth retrying and the error code might simply be 
+if a GET request fails with one of these status codes, it might be worth retrying and the error code might simply be
 due to high load
 """
 
 
 class TmdsClient:
     """
     an async wrapper around the TMDS API
@@ -93,14 +94,39 @@
         """
         async with self._session_lock:
             if self._session is not None and not self._session.closed:
                 _logger.info("Closing aiohttp session")
                 await self._session.close()
                 self._session = None
 
+    async def _poll_until_has_been_handled(
+        self, tmds_event_id: uuid.UUID, timeout: timedelta = timedelta(seconds=30)
+    ) -> bool:
+        """
+        Polls the /hasBeenHandledEndpoint once per second until the event has been handled
+        Returns true if the event has been handled, false if the timeout has been reached.
+        """
+        url = self._config.server_url / "api/Event" / "hasBeenHandled" / str(tmds_event_id)
+        session = await self._get_session()
+        timeout_in_seconds: int = int(timeout.total_seconds())
+        seconds_left = timeout_in_seconds
+        while seconds_left > 0:
+            async with session.get(url, ssl=True) as response:
+                body = await response.text()
+                if body.lower() in {'"true"', "true"}:
+                    _logger.debug("Event %s has been handled", tmds_event_id)
+                    return True
+
+                _logger.log(5, "Event %s has not been handled yet. Waiting another second", tmds_event_id)
+                await asyncio.sleep(1)
+                seconds_left -= 1
+        _logger.warning("Event %s has not been handled after %s seconds", tmds_event_id, timeout_in_seconds)
+        await asyncio.sleep(60)  # slow down. slow down, at least in this thread
+        return False
+
     async def get_netzvertraege_for_melo(self, melo_id: str) -> list[Netzvertrag]:
         """
         provide a melo id, e.g. 'DE1234567890123456789012345678901' and get the corresponding netzvertrag
         """
         if not melo_id:
             raise ValueError("You must not provide an empty melo_id")
         session = await self._get_session()
@@ -129,14 +155,39 @@
                 response.raise_for_status()
             finally:
                 _logger.debug("[%s] response status: %s", str(request_uuid), response.status)
             response_json = await response.json()
             result = Netzvertrag.model_validate(response_json)
         return result
 
+    async def set_plattformfaehigkeit(
+        self, external_ao_id: str, change_date: datetime, is_plattformfaehig: bool = True
+    ) -> bool:
+        """
+        set the plattformfaehigkeit of an Anschlussobjekt; return true on success, false or raises exception on failure
+        """
+        if change_date.tzinfo is None:
+            raise ValueError("change_date must be timezone aware")
+        url = (
+            self._config.server_url
+            / "api"
+            / "Anschlussobjekt"
+            / external_ao_id
+            / "setPlattform"
+            % {"aenderungsdatum": change_date.isoformat(), "plattformfaehig": str(is_plattformfaehig).lower()}
+        )
+        session = await self._get_session()
+        async with session.post(url, ssl=True) as response:
+            # the beloved tmds api does not consistently return an event id
+            id_string = response.headers.get("x-event-id")
+        if id_string is None:
+            return True
+        tmds_event_id = uuid.UUID(id_string)
+        return await self._poll_until_has_been_handled(tmds_event_id)
+
     async def get_all_netzvertrag_ids(self) -> list[uuid.UUID]:
         """
         get all IDs of netzverträge that exist on server side
         """
         session = await self._get_session()
         request_url = self._config.server_url / "api" / "Netzvertrag" / "allIds"
         request_uuid = uuid.uuid4()
```

### Comparing `tmdsclient-0.2.1/src/tmdsclient/models/bo4e_stub.py` & `tmdsclient-0.2.2/src/tmdsclient/models/bo4e_stub.py`

 * *Files identical despite different names*

### Comparing `tmdsclient-0.2.1/src/tmdsclient/models/messlokation.py` & `tmdsclient-0.2.2/src/tmdsclient/models/messlokation.py`

 * *Files identical despite different names*

### Comparing `tmdsclient-0.2.1/src/tmdsclient/models/netzvertrag.py` & `tmdsclient-0.2.2/src/tmdsclient/models/netzvertrag.py`

 * *Files identical despite different names*

### Comparing `tmdsclient-0.2.1/src/tmdsclient/models/patches.py` & `tmdsclient-0.2.2/src/tmdsclient/models/patches.py`

 * *Files identical despite different names*

### Comparing `tmdsclient-0.2.1/src/tmdsclient/models/utils.py` & `tmdsclient-0.2.2/src/tmdsclient/models/utils.py`

 * *Files identical despite different names*

### Comparing `tmdsclient-0.2.1/src/tmdsclient/models/zaehler.py` & `tmdsclient-0.2.2/src/tmdsclient/models/zaehler.py`

 * *Files identical despite different names*

### Comparing `tmdsclient-0.2.1/src/tmdsclient/models/zaehler_bo_model.py` & `tmdsclient-0.2.2/src/tmdsclient/models/zaehler_bo_model.py`

 * *Files identical despite different names*

### Comparing `tmdsclient-0.2.1/src/tmdsclient/models/zaehlwerk.py` & `tmdsclient-0.2.2/src/tmdsclient/models/zaehlwerk.py`

 * *Files identical despite different names*

### Comparing `tmdsclient-0.2.1/src/tmdsclient/models/zeitscheibe.py` & `tmdsclient-0.2.2/src/tmdsclient/models/zeitscheibe.py`

 * *Files identical despite different names*

### Comparing `tmdsclient-0.2.1/.gitignore` & `tmdsclient-0.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `tmdsclient-0.2.1/LICENSE` & `tmdsclient-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tmdsclient-0.2.1/pyproject.toml` & `tmdsclient-0.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tmdsclient-0.2.1/PKG-INFO` & `tmdsclient-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: tmdsclient
-Version: 0.2.1
+Version: 0.2.2
 Summary: Fully typed, async client library for Technical Master Data Service (TMDS)
 Project-URL: Changelog, https://github.com/Hochfrequenz/tmdsclient.py/releases
 Project-URL: Homepage, https://github.com/Hochfrequenz/tmdsclient.py
 Author-email: Hochfreuqenz Unternehmensberatung GmbH <info+github@hochfrequenz.de>
 License: MIT
 License-File: LICENSE
 Keywords: technical master data,tmds
```

