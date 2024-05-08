# Comparing `tmp/optrabot-0.9.2a0.tar.gz` & `tmp/optrabot-0.9.2a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optrabot-0.9.2a0.tar", max compression
+gzip compressed data, was "optrabot-0.9.2a1.tar", max compression
```

## Comparing `optrabot-0.9.2a0.tar` & `optrabot-0.9.2a1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0      742 2023-12-14 21:15:50.230643 optrabot-0.9.2a0/README.md
--rw-r--r--   0        0        0        0 2023-12-12 13:10:12.039398 optrabot-0.9.2a0/optrabot/__init__.py
--rw-r--r--   0        0        0       38 2024-02-22 12:22:44.563187 optrabot-0.9.2a0/optrabot/alembic/README
--rw-r--r--   0        0        0     2717 2024-02-29 07:20:04.745375 optrabot-0.9.2a0/optrabot/alembic/env.py
--rw-r--r--   0        0        0      635 2024-02-22 12:22:44.563872 optrabot-0.9.2a0/optrabot/alembic/script.py.mako
--rw-r--r--   0        0        0     1996 2024-02-22 12:22:44.564106 optrabot-0.9.2a0/optrabot/alembic/versions/cc3c6f4d83dc_initial_database.py
--rw-r--r--   0        0        0     3633 2024-02-22 12:22:44.562937 optrabot-0.9.2a0/optrabot/alembic.ini
--rw-r--r--   0        0        0    11856 2024-04-15 10:20:52.308184 optrabot-0.9.2a0/optrabot/config.py
--rw-r--r--   0        0        0     3133 2024-04-15 10:20:52.308983 optrabot-0.9.2a0/optrabot/crud.py
--rw-r--r--   0        0        0     1106 2024-02-22 12:22:44.565150 optrabot-0.9.2a0/optrabot/database.py
--rw-r--r--   0        0        0     2323 2024-05-07 18:46:58.969402 optrabot-0.9.2a0/optrabot/main.py
--rw-r--r--   0        0        0      936 2023-12-21 19:35:29.667749 optrabot-0.9.2a0/optrabot/marketdatatype.py
--rw-r--r--   0        0        0     1613 2024-02-22 12:22:44.565732 optrabot-0.9.2a0/optrabot/models.py
--rw-r--r--   0        0        0      966 2024-02-22 12:22:44.566114 optrabot-0.9.2a0/optrabot/optionhelper.py
--rw-r--r--   0        0        0    10733 2024-05-08 11:10:23.701664 optrabot-0.9.2a0/optrabot/optrabot.py
--rw-r--r--   0        0        0      855 2024-02-22 12:22:44.566593 optrabot-0.9.2a0/optrabot/schemas.py
--rw-r--r--   0        0        0     2859 2024-02-29 07:20:04.746827 optrabot-0.9.2a0/optrabot/stoplossadjuster.py
--rw-r--r--   0        0        0     2936 2024-02-22 12:22:44.567158 optrabot-0.9.2a0/optrabot/tradehelper.py
--rw-r--r--   0        0        0        0 2024-02-22 12:22:44.567199 optrabot-0.9.2a0/optrabot/tradetemplate/__init__.py
--rw-r--r--   0        0        0      177 2024-05-08 06:34:31.950408 optrabot-0.9.2a0/optrabot/tradetemplate/ironfly.py
--rw-r--r--   0        0        0      181 2024-02-22 12:22:44.568125 optrabot-0.9.2a0/optrabot/tradetemplate/putspread.py
--rw-r--r--   0        0        0     3405 2024-03-19 15:36:19.404722 optrabot-0.9.2a0/optrabot/tradetemplate/template.py
--rw-r--r--   0        0        0     2273 2024-04-22 05:51:40.165667 optrabot-0.9.2a0/optrabot/tradetemplate/templatefactory.py
--rw-r--r--   0        0        0      564 2024-02-22 12:22:44.568968 optrabot-0.9.2a0/optrabot/tradetemplate/templatetrigger.py
--rw-r--r--   0        0        0    49985 2024-05-08 11:10:23.702123 optrabot-0.9.2a0/optrabot/tradinghubclient.py
--rw-r--r--   0        0        0      821 2024-05-08 11:15:41.630244 optrabot-0.9.2a0/pyproject.toml
--rw-r--r--   0        0        0     1842 1970-01-01 00:00:00.000000 optrabot-0.9.2a0/PKG-INFO
+-rw-r--r--   0        0        0      742 2023-12-14 21:15:50.230643 optrabot-0.9.2a1/README.md
+-rw-r--r--   0        0        0        0 2023-12-12 13:10:12.039398 optrabot-0.9.2a1/optrabot/__init__.py
+-rw-r--r--   0        0        0       38 2024-02-22 12:22:44.563187 optrabot-0.9.2a1/optrabot/alembic/README
+-rw-r--r--   0        0        0     2717 2024-02-29 07:20:04.745375 optrabot-0.9.2a1/optrabot/alembic/env.py
+-rw-r--r--   0        0        0      635 2024-02-22 12:22:44.563872 optrabot-0.9.2a1/optrabot/alembic/script.py.mako
+-rw-r--r--   0        0        0     1996 2024-02-22 12:22:44.564106 optrabot-0.9.2a1/optrabot/alembic/versions/cc3c6f4d83dc_initial_database.py
+-rw-r--r--   0        0        0     3633 2024-02-22 12:22:44.562937 optrabot-0.9.2a1/optrabot/alembic.ini
+-rw-r--r--   0        0        0    11856 2024-04-15 10:20:52.308184 optrabot-0.9.2a1/optrabot/config.py
+-rw-r--r--   0        0        0     3133 2024-04-15 10:20:52.308983 optrabot-0.9.2a1/optrabot/crud.py
+-rw-r--r--   0        0        0     1106 2024-02-22 12:22:44.565150 optrabot-0.9.2a1/optrabot/database.py
+-rw-r--r--   0        0        0     2323 2024-05-07 18:46:58.969402 optrabot-0.9.2a1/optrabot/main.py
+-rw-r--r--   0        0        0      936 2023-12-21 19:35:29.667749 optrabot-0.9.2a1/optrabot/marketdatatype.py
+-rw-r--r--   0        0        0     1613 2024-02-22 12:22:44.565732 optrabot-0.9.2a1/optrabot/models.py
+-rw-r--r--   0        0        0      966 2024-02-22 12:22:44.566114 optrabot-0.9.2a1/optrabot/optionhelper.py
+-rw-r--r--   0        0        0    10733 2024-05-08 11:10:23.701664 optrabot-0.9.2a1/optrabot/optrabot.py
+-rw-r--r--   0        0        0      855 2024-02-22 12:22:44.566593 optrabot-0.9.2a1/optrabot/schemas.py
+-rw-r--r--   0        0        0     2859 2024-02-29 07:20:04.746827 optrabot-0.9.2a1/optrabot/stoplossadjuster.py
+-rw-r--r--   0        0        0     2936 2024-02-22 12:22:44.567158 optrabot-0.9.2a1/optrabot/tradehelper.py
+-rw-r--r--   0        0        0        0 2024-02-22 12:22:44.567199 optrabot-0.9.2a1/optrabot/tradetemplate/__init__.py
+-rw-r--r--   0        0        0      177 2024-05-08 06:34:31.950408 optrabot-0.9.2a1/optrabot/tradetemplate/ironfly.py
+-rw-r--r--   0        0        0      181 2024-02-22 12:22:44.568125 optrabot-0.9.2a1/optrabot/tradetemplate/putspread.py
+-rw-r--r--   0        0        0     3405 2024-03-19 15:36:19.404722 optrabot-0.9.2a1/optrabot/tradetemplate/template.py
+-rw-r--r--   0        0        0     2273 2024-04-22 05:51:40.165667 optrabot-0.9.2a1/optrabot/tradetemplate/templatefactory.py
+-rw-r--r--   0        0        0      564 2024-02-22 12:22:44.568968 optrabot-0.9.2a1/optrabot/tradetemplate/templatetrigger.py
+-rw-r--r--   0        0        0    49985 2024-05-08 11:10:23.702123 optrabot-0.9.2a1/optrabot/tradinghubclient.py
+-rw-r--r--   0        0        0      845 2024-05-08 11:21:42.865668 optrabot-0.9.2a1/pyproject.toml
+-rw-r--r--   0        0        0     1887 1970-01-01 00:00:00.000000 optrabot-0.9.2a1/PKG-INFO
```

### Comparing `optrabot-0.9.2a0/README.md` & `optrabot-0.9.2a1/README.md`

 * *Files identical despite different names*

### Comparing `optrabot-0.9.2a0/optrabot/alembic/env.py` & `optrabot-0.9.2a1/optrabot/alembic/env.py`

 * *Files identical despite different names*

### Comparing `optrabot-0.9.2a0/optrabot/alembic/script.py.mako` & `optrabot-0.9.2a1/optrabot/alembic/script.py.mako`

 * *Files identical despite different names*

### Comparing `optrabot-0.9.2a0/optrabot/alembic/versions/cc3c6f4d83dc_initial_database.py` & `optrabot-0.9.2a1/optrabot/alembic/versions/cc3c6f4d83dc_initial_database.py`

 * *Files identical despite different names*

### Comparing `optrabot-0.9.2a0/optrabot/alembic.ini` & `optrabot-0.9.2a1/optrabot/alembic.ini`

 * *Files identical despite different names*

### Comparing `optrabot-0.9.2a0/optrabot/config.py` & `optrabot-0.9.2a1/optrabot/config.py`

 * *Files identical despite different names*

### Comparing `optrabot-0.9.2a0/optrabot/crud.py` & `optrabot-0.9.2a1/optrabot/crud.py`

 * *Files identical despite different names*

### Comparing `optrabot-0.9.2a0/optrabot/database.py` & `optrabot-0.9.2a1/optrabot/database.py`

 * *Files identical despite different names*

### Comparing `optrabot-0.9.2a0/optrabot/main.py` & `optrabot-0.9.2a1/optrabot/main.py`

 * *Files identical despite different names*

### Comparing `optrabot-0.9.2a0/optrabot/marketdatatype.py` & `optrabot-0.9.2a1/optrabot/marketdatatype.py`

 * *Files identical despite different names*

### Comparing `optrabot-0.9.2a0/optrabot/models.py` & `optrabot-0.9.2a1/optrabot/models.py`

 * *Files identical despite different names*

### Comparing `optrabot-0.9.2a0/optrabot/optionhelper.py` & `optrabot-0.9.2a1/optrabot/optionhelper.py`

 * *Files identical despite different names*

### Comparing `optrabot-0.9.2a0/optrabot/optrabot.py` & `optrabot-0.9.2a1/optrabot/optrabot.py`

 * *Files identical despite different names*

### Comparing `optrabot-0.9.2a0/optrabot/schemas.py` & `optrabot-0.9.2a1/optrabot/schemas.py`

 * *Files identical despite different names*

### Comparing `optrabot-0.9.2a0/optrabot/stoplossadjuster.py` & `optrabot-0.9.2a1/optrabot/stoplossadjuster.py`

 * *Files identical despite different names*

### Comparing `optrabot-0.9.2a0/optrabot/tradehelper.py` & `optrabot-0.9.2a1/optrabot/tradehelper.py`

 * *Files identical despite different names*

### Comparing `optrabot-0.9.2a0/optrabot/tradetemplate/template.py` & `optrabot-0.9.2a1/optrabot/tradetemplate/template.py`

 * *Files identical despite different names*

### Comparing `optrabot-0.9.2a0/optrabot/tradetemplate/templatefactory.py` & `optrabot-0.9.2a1/optrabot/tradetemplate/templatefactory.py`

 * *Files identical despite different names*

### Comparing `optrabot-0.9.2a0/optrabot/tradetemplate/templatetrigger.py` & `optrabot-0.9.2a1/optrabot/tradetemplate/templatetrigger.py`

 * *Files identical despite different names*

### Comparing `optrabot-0.9.2a0/optrabot/tradinghubclient.py` & `optrabot-0.9.2a1/optrabot/tradinghubclient.py`

 * *Files identical despite different names*

### Comparing `optrabot-0.9.2a0/pyproject.toml` & `optrabot-0.9.2a1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "optrabot"
-version = "0.9.2a0"
+version = "0.9.2a1"
 description = "QuantX OptraBot is a Options Trading Bot for automatically trading options strategies with an Interactive Brokers account."
 authors = ["QuantX GmbH"]
 readme = "README.md"
 license = "MIT"
 homepage = "http://www.optrabot.com"
 keywords = ["tws"]
 packages =  [{include = "optrabot"}]
@@ -21,14 +21,15 @@
 ruyaml = "^0.91.0"
 ib-insync = "^0.9.86"
 httpx = "^0.25.2"
 inquirerpy = "^0.3.4"
 tzdata = "^2023.3"
 sqlalchemy = "^2.0.25"
 alembic = "^1.13.1"
+apscheduler = "^3.10.4"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 optrabot = "optrabot.main:run"
```

### Comparing `optrabot-0.9.2a0/PKG-INFO` & `optrabot-0.9.2a1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: optrabot
-Version: 0.9.2a0
+Version: 0.9.2a1
 Summary: QuantX OptraBot is a Options Trading Bot for automatically trading options strategies with an Interactive Brokers account.
 Home-page: http://www.optrabot.com
 License: MIT
 Keywords: tws
 Author: QuantX GmbH
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: alembic (>=1.13.1,<2.0.0)
+Requires-Dist: apscheduler (>=3.10.4,<4.0.0)
 Requires-Dist: fastapi (>=0.105.0,<0.106.0)
 Requires-Dist: httpx (>=0.25.2,<0.26.0)
 Requires-Dist: ib-insync (>=0.9.86,<0.10.0)
 Requires-Dist: inquirerpy (>=0.3.4,<0.4.0)
 Requires-Dist: loguru (>=0.7.2,<0.8.0)
 Requires-Dist: ruyaml (>=0.91.0,<0.92.0)
 Requires-Dist: sqlalchemy (>=2.0.25,<3.0.0)
```

