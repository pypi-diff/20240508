# Comparing `tmp/invenio_sip2-0.6.22.tar.gz` & `tmp/invenio_sip2-0.6.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "invenio_sip2-0.6.22.tar", max compression
+gzip compressed data, was "invenio_sip2-0.6.23.tar", max compression
```

## Comparing `invenio_sip2-0.6.22.tar` & `invenio_sip2-0.6.23.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0    34523 2020-09-01 12:22:11.361403 invenio_sip2-0.6.22/LICENSE
--rw-r--r--   0        0        0     1911 2022-12-19 14:27:54.050444 invenio_sip2-0.6.22/README.rst
--rw-r--r--   0        0        0     1089 2022-08-30 09:33:30.888790 invenio_sip2-0.6.22/invenio_sip2/__init__.py
--rw-r--r--   0        0        0     1311 2022-08-30 09:33:30.889923 invenio_sip2-0.6.22/invenio_sip2/actions/__init__.py
--rw-r--r--   0        0        0    26534 2023-03-30 07:00:48.634171 invenio_sip2-0.6.22/invenio_sip2/actions/actions.py
--rw-r--r--   0        0        0     2730 2022-08-30 09:33:30.892207 invenio_sip2-0.6.22/invenio_sip2/actions/base.py
--rw-r--r--   0        0        0    10272 2022-08-30 09:33:30.893125 invenio_sip2-0.6.22/invenio_sip2/api.py
--rw-r--r--   0        0        0     2803 2022-08-30 09:33:30.893968 invenio_sip2-0.6.22/invenio_sip2/cli.py
--rw-r--r--   0        0        0    36278 2022-12-19 14:27:54.053391 invenio_sip2-0.6.22/invenio_sip2/config.py
--rw-r--r--   0        0        0     4627 2022-08-30 09:33:30.895825 invenio_sip2-0.6.22/invenio_sip2/datastore.py
--rw-r--r--   0        0        0     2151 2022-08-30 09:33:30.896575 invenio_sip2-0.6.22/invenio_sip2/decorators.py
--rw-r--r--   0        0        0     1668 2022-12-19 14:27:54.053985 invenio_sip2-0.6.22/invenio_sip2/errors.py
--rw-r--r--   0        0        0    13453 2022-12-19 14:27:54.054864 invenio_sip2-0.6.22/invenio_sip2/ext.py
--rw-r--r--   0        0        0     1479 2022-12-19 14:27:54.056619 invenio_sip2-0.6.22/invenio_sip2/handlers/__init__.py
--rw-r--r--   0        0        0     4035 2022-12-19 14:27:54.058368 invenio_sip2-0.6.22/invenio_sip2/handlers/api_handlers.py
--rw-r--r--   0        0        0     5437 2022-12-19 14:27:54.058952 invenio_sip2-0.6.22/invenio_sip2/handlers/base.py
--rw-r--r--   0        0        0     1284 2022-08-30 09:33:30.903410 invenio_sip2-0.6.22/invenio_sip2/handlers/utils.py
--rw-r--r--   0        0        0     3473 2022-12-19 14:27:54.059471 invenio_sip2-0.6.22/invenio_sip2/helpers.py
--rw-r--r--   0        0        0    19327 2023-03-30 07:00:48.634635 invenio_sip2-0.6.22/invenio_sip2/models.py
--rw-r--r--   0        0        0     1483 2021-07-13 07:06:01.871610 invenio_sip2-0.6.22/invenio_sip2/permissions.py
--rw-r--r--   0        0        0     1164 2022-08-30 09:33:30.905373 invenio_sip2-0.6.22/invenio_sip2/proxies.py
--rw-r--r--   0        0        0      792 2022-08-30 09:33:30.906733 invenio_sip2-0.6.22/invenio_sip2/records/__init__.py
--rw-r--r--   0        0        0     8129 2022-08-30 14:05:15.469559 invenio_sip2-0.6.22/invenio_sip2/records/record.py
--rw-r--r--   0        0        0    12667 2022-08-30 09:33:30.908365 invenio_sip2-0.6.22/invenio_sip2/server.py
--rw-r--r--   0        0        0      346 2020-09-01 12:22:11.368893 invenio_sip2-0.6.22/invenio_sip2/templates/invenio_sip2/base.html
--rw-r--r--   0        0        0     1543 2021-07-13 07:06:01.873561 invenio_sip2-0.6.22/invenio_sip2/templates/invenio_sip2/monitoring.html
--rw-r--r--   0        0        0     8247 2020-09-01 12:22:11.370077 invenio_sip2-0.6.22/invenio_sip2/translations/de/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0     8248 2020-09-01 12:22:11.370445 invenio_sip2-0.6.22/invenio_sip2/translations/en/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0     8248 2020-09-01 12:22:11.371137 invenio_sip2-0.6.22/invenio_sip2/translations/es/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0     8246 2020-09-01 12:22:11.371809 invenio_sip2-0.6.22/invenio_sip2/translations/fr/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0     8248 2020-09-01 12:22:11.373259 invenio_sip2-0.6.22/invenio_sip2/translations/it/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0     8201 2020-09-01 12:22:11.373446 invenio_sip2-0.6.22/invenio_sip2/translations/messages.pot
--rw-r--r--   0        0        0     8246 2020-09-01 12:22:11.375290 invenio_sip2-0.6.22/invenio_sip2/translations/nl/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0     5545 2023-06-15 09:11:42.452769 invenio_sip2-0.6.22/invenio_sip2/utils.py
--rw-r--r--   0        0        0      748 2023-11-24 13:41:24.533698 invenio_sip2-0.6.22/invenio_sip2/version.py
--rw-r--r--   0        0        0      866 2022-08-30 09:33:30.910352 invenio_sip2-0.6.22/invenio_sip2/views/__init__.py
--rw-r--r--   0        0        0     3632 2022-11-07 13:00:55.735281 invenio_sip2-0.6.22/invenio_sip2/views/rest.py
--rw-r--r--   0        0        0     1209 2023-03-30 10:33:36.024330 invenio_sip2-0.6.22/invenio_sip2/views/views.py
--rw-r--r--   0        0        0     2191 2023-11-24 13:41:24.534947 invenio_sip2-0.6.22/pyproject.toml
--rw-r--r--   0        0        0     4001 1970-01-01 00:00:00.000000 invenio_sip2-0.6.22/setup.py
--rw-r--r--   0        0        0     3755 1970-01-01 00:00:00.000000 invenio_sip2-0.6.22/PKG-INFO
+-rw-r--r--   0        0        0    34523 2020-09-01 12:22:11.361403 invenio_sip2-0.6.23/LICENSE
+-rw-r--r--   0        0        0     1911 2022-12-19 14:27:54.050444 invenio_sip2-0.6.23/README.rst
+-rw-r--r--   0        0        0     1089 2022-08-30 09:33:30.888790 invenio_sip2-0.6.23/invenio_sip2/__init__.py
+-rw-r--r--   0        0        0     1311 2022-08-30 09:33:30.889923 invenio_sip2-0.6.23/invenio_sip2/actions/__init__.py
+-rw-r--r--   0        0        0    26534 2023-03-30 07:00:48.634171 invenio_sip2-0.6.23/invenio_sip2/actions/actions.py
+-rw-r--r--   0        0        0     2730 2022-08-30 09:33:30.892207 invenio_sip2-0.6.23/invenio_sip2/actions/base.py
+-rw-r--r--   0        0        0    10272 2022-08-30 09:33:30.893125 invenio_sip2-0.6.23/invenio_sip2/api.py
+-rw-r--r--   0        0        0     2803 2022-08-30 09:33:30.893968 invenio_sip2-0.6.23/invenio_sip2/cli.py
+-rw-r--r--   0        0        0    36278 2022-12-19 14:27:54.053391 invenio_sip2-0.6.23/invenio_sip2/config.py
+-rw-r--r--   0        0        0     4627 2022-08-30 09:33:30.895825 invenio_sip2-0.6.23/invenio_sip2/datastore.py
+-rw-r--r--   0        0        0     2151 2022-08-30 09:33:30.896575 invenio_sip2-0.6.23/invenio_sip2/decorators.py
+-rw-r--r--   0        0        0     1668 2022-12-19 14:27:54.053985 invenio_sip2-0.6.23/invenio_sip2/errors.py
+-rw-r--r--   0        0        0    13453 2022-12-19 14:27:54.054864 invenio_sip2-0.6.23/invenio_sip2/ext.py
+-rw-r--r--   0        0        0     1479 2022-12-19 14:27:54.056619 invenio_sip2-0.6.23/invenio_sip2/handlers/__init__.py
+-rw-r--r--   0        0        0     4035 2022-12-19 14:27:54.058368 invenio_sip2-0.6.23/invenio_sip2/handlers/api_handlers.py
+-rw-r--r--   0        0        0     5437 2022-12-19 14:27:54.058952 invenio_sip2-0.6.23/invenio_sip2/handlers/base.py
+-rw-r--r--   0        0        0     1284 2022-08-30 09:33:30.903410 invenio_sip2-0.6.23/invenio_sip2/handlers/utils.py
+-rw-r--r--   0        0        0     3473 2022-12-19 14:27:54.059471 invenio_sip2-0.6.23/invenio_sip2/helpers.py
+-rw-r--r--   0        0        0    19327 2023-03-30 07:00:48.634635 invenio_sip2-0.6.23/invenio_sip2/models.py
+-rw-r--r--   0        0        0     1483 2021-07-13 07:06:01.871610 invenio_sip2-0.6.23/invenio_sip2/permissions.py
+-rw-r--r--   0        0        0     1164 2022-08-30 09:33:30.905373 invenio_sip2-0.6.23/invenio_sip2/proxies.py
+-rw-r--r--   0        0        0      792 2022-08-30 09:33:30.906733 invenio_sip2-0.6.23/invenio_sip2/records/__init__.py
+-rw-r--r--   0        0        0     8129 2022-08-30 14:05:15.469559 invenio_sip2-0.6.23/invenio_sip2/records/record.py
+-rw-r--r--   0        0        0    12667 2022-08-30 09:33:30.908365 invenio_sip2-0.6.23/invenio_sip2/server.py
+-rw-r--r--   0        0        0      346 2020-09-01 12:22:11.368893 invenio_sip2-0.6.23/invenio_sip2/templates/invenio_sip2/base.html
+-rw-r--r--   0        0        0     1543 2021-07-13 07:06:01.873561 invenio_sip2-0.6.23/invenio_sip2/templates/invenio_sip2/monitoring.html
+-rw-r--r--   0        0        0     8247 2020-09-01 12:22:11.370077 invenio_sip2-0.6.23/invenio_sip2/translations/de/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     8248 2020-09-01 12:22:11.370445 invenio_sip2-0.6.23/invenio_sip2/translations/en/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     8248 2020-09-01 12:22:11.371137 invenio_sip2-0.6.23/invenio_sip2/translations/es/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     8246 2020-09-01 12:22:11.371809 invenio_sip2-0.6.23/invenio_sip2/translations/fr/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     8248 2020-09-01 12:22:11.373259 invenio_sip2-0.6.23/invenio_sip2/translations/it/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     8201 2020-09-01 12:22:11.373446 invenio_sip2-0.6.23/invenio_sip2/translations/messages.pot
+-rw-r--r--   0        0        0     8246 2020-09-01 12:22:11.375290 invenio_sip2-0.6.23/invenio_sip2/translations/nl/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     5545 2023-06-15 09:11:42.452769 invenio_sip2-0.6.23/invenio_sip2/utils.py
+-rw-r--r--   0        0        0      748 2024-05-08 09:57:37.749053 invenio_sip2-0.6.23/invenio_sip2/version.py
+-rw-r--r--   0        0        0      866 2022-08-30 09:33:30.910352 invenio_sip2-0.6.23/invenio_sip2/views/__init__.py
+-rw-r--r--   0        0        0     3632 2022-11-07 13:00:55.735281 invenio_sip2-0.6.23/invenio_sip2/views/rest.py
+-rw-r--r--   0        0        0     1209 2023-03-30 10:33:36.024330 invenio_sip2-0.6.23/invenio_sip2/views/views.py
+-rw-r--r--   0        0        0     2123 2024-05-08 10:03:22.065086 invenio_sip2-0.6.23/pyproject.toml
+-rw-r--r--   0        0        0     3864 1970-01-01 00:00:00.000000 invenio_sip2-0.6.23/setup.py
+-rw-r--r--   0        0        0     3562 1970-01-01 00:00:00.000000 invenio_sip2-0.6.23/PKG-INFO
```

### Comparing `invenio_sip2-0.6.22/LICENSE` & `invenio_sip2-0.6.23/LICENSE`

 * *Files identical despite different names*

### Comparing `invenio_sip2-0.6.22/README.rst` & `invenio_sip2-0.6.23/README.rst`

 * *Files identical despite different names*

### Comparing `invenio_sip2-0.6.22/invenio_sip2/__init__.py` & `invenio_sip2-0.6.23/invenio_sip2/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio_sip2-0.6.22/invenio_sip2/actions/__init__.py` & `invenio_sip2-0.6.23/invenio_sip2/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio_sip2-0.6.22/invenio_sip2/actions/actions.py` & `invenio_sip2-0.6.23/invenio_sip2/actions/actions.py`

 * *Files identical despite different names*

### Comparing `invenio_sip2-0.6.22/invenio_sip2/actions/base.py` & `invenio_sip2-0.6.23/invenio_sip2/actions/base.py`

 * *Files identical despite different names*

### Comparing `invenio_sip2-0.6.22/invenio_sip2/api.py` & `invenio_sip2-0.6.23/invenio_sip2/api.py`

 * *Files identical despite different names*

### Comparing `invenio_sip2-0.6.22/invenio_sip2/cli.py` & `invenio_sip2-0.6.23/invenio_sip2/cli.py`

 * *Files identical despite different names*

### Comparing `invenio_sip2-0.6.22/invenio_sip2/config.py` & `invenio_sip2-0.6.23/invenio_sip2/config.py`

 * *Files identical despite different names*

### Comparing `invenio_sip2-0.6.22/invenio_sip2/datastore.py` & `invenio_sip2-0.6.23/invenio_sip2/datastore.py`

 * *Files identical despite different names*

### Comparing `invenio_sip2-0.6.22/invenio_sip2/decorators.py` & `invenio_sip2-0.6.23/invenio_sip2/decorators.py`

 * *Files identical despite different names*

### Comparing `invenio_sip2-0.6.22/invenio_sip2/errors.py` & `invenio_sip2-0.6.23/invenio_sip2/errors.py`

 * *Files identical despite different names*

### Comparing `invenio_sip2-0.6.22/invenio_sip2/ext.py` & `invenio_sip2-0.6.23/invenio_sip2/ext.py`

 * *Files identical despite different names*

### Comparing `invenio_sip2-0.6.22/invenio_sip2/handlers/__init__.py` & `invenio_sip2-0.6.23/invenio_sip2/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio_sip2-0.6.22/invenio_sip2/handlers/api_handlers.py` & `invenio_sip2-0.6.23/invenio_sip2/handlers/api_handlers.py`

 * *Files identical despite different names*

### Comparing `invenio_sip2-0.6.22/invenio_sip2/handlers/base.py` & `invenio_sip2-0.6.23/invenio_sip2/handlers/base.py`

 * *Files identical despite different names*

### Comparing `invenio_sip2-0.6.22/invenio_sip2/handlers/utils.py` & `invenio_sip2-0.6.23/invenio_sip2/handlers/utils.py`

 * *Files identical despite different names*

### Comparing `invenio_sip2-0.6.22/invenio_sip2/helpers.py` & `invenio_sip2-0.6.23/invenio_sip2/helpers.py`

 * *Files identical despite different names*

### Comparing `invenio_sip2-0.6.22/invenio_sip2/models.py` & `invenio_sip2-0.6.23/invenio_sip2/models.py`

 * *Files identical despite different names*

### Comparing `invenio_sip2-0.6.22/invenio_sip2/permissions.py` & `invenio_sip2-0.6.23/invenio_sip2/permissions.py`

 * *Files identical despite different names*

### Comparing `invenio_sip2-0.6.22/invenio_sip2/proxies.py` & `invenio_sip2-0.6.23/invenio_sip2/proxies.py`

 * *Files identical despite different names*

### Comparing `invenio_sip2-0.6.22/invenio_sip2/records/__init__.py` & `invenio_sip2-0.6.23/invenio_sip2/records/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio_sip2-0.6.22/invenio_sip2/records/record.py` & `invenio_sip2-0.6.23/invenio_sip2/records/record.py`

 * *Files identical despite different names*

### Comparing `invenio_sip2-0.6.22/invenio_sip2/server.py` & `invenio_sip2-0.6.23/invenio_sip2/server.py`

 * *Files identical despite different names*

### Comparing `invenio_sip2-0.6.22/invenio_sip2/templates/invenio_sip2/monitoring.html` & `invenio_sip2-0.6.23/invenio_sip2/templates/invenio_sip2/monitoring.html`

 * *Files identical despite different names*

### Comparing `invenio_sip2-0.6.22/invenio_sip2/translations/de/LC_MESSAGES/messages.po` & `invenio_sip2-0.6.23/invenio_sip2/translations/de/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio_sip2-0.6.22/invenio_sip2/translations/en/LC_MESSAGES/messages.po` & `invenio_sip2-0.6.23/invenio_sip2/translations/en/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio_sip2-0.6.22/invenio_sip2/translations/es/LC_MESSAGES/messages.po` & `invenio_sip2-0.6.23/invenio_sip2/translations/es/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio_sip2-0.6.22/invenio_sip2/translations/fr/LC_MESSAGES/messages.po` & `invenio_sip2-0.6.23/invenio_sip2/translations/fr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio_sip2-0.6.22/invenio_sip2/translations/it/LC_MESSAGES/messages.po` & `invenio_sip2-0.6.23/invenio_sip2/translations/it/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio_sip2-0.6.22/invenio_sip2/translations/messages.pot` & `invenio_sip2-0.6.23/invenio_sip2/translations/messages.pot`

 * *Files identical despite different names*

### Comparing `invenio_sip2-0.6.22/invenio_sip2/translations/nl/LC_MESSAGES/messages.po` & `invenio_sip2-0.6.23/invenio_sip2/translations/nl/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio_sip2-0.6.22/invenio_sip2/utils.py` & `invenio_sip2-0.6.23/invenio_sip2/utils.py`

 * *Files identical despite different names*

### Comparing `invenio_sip2-0.6.22/invenio_sip2/version.py` & `invenio_sip2-0.6.23/invenio_sip2/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 """Version information for Invenio-SIP2."""
 
-__version__ = '0.6.22'
+__version__ = '0.6.23'
```

### Comparing `invenio_sip2-0.6.22/invenio_sip2/views/__init__.py` & `invenio_sip2-0.6.23/invenio_sip2/views/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio_sip2-0.6.22/invenio_sip2/views/rest.py` & `invenio_sip2-0.6.23/invenio_sip2/views/rest.py`

 * *Files identical despite different names*

### Comparing `invenio_sip2-0.6.22/invenio_sip2/views/views.py` & `invenio_sip2-0.6.23/invenio_sip2/views/views.py`

 * *Files identical despite different names*

### Comparing `invenio_sip2-0.6.22/pyproject.toml` & `invenio_sip2-0.6.23/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "invenio-sip2"
-version = "0.6.22"
+version = "0.6.23"
 description = "Invenio module that add a SIP2 communication for library self-check service"
 readme = "README.rst"
 authors = ["Laurent Dubois <laurent.dubois@uclouvain.be>"]
 license = "GNU Affero General Public License v3.0"
 repository = "https://github.com/inveniosoftware-contrib/invenio-sip2"
 documentation = "https://invenio-sip2.readthedocs.io"
 classifiers = [
@@ -20,33 +20,31 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Development Status :: 3 - Alpha",
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.7,<3.10"
-invenio-base = ">=1.2.11,<1.3.0"
+invenio-base = ">=1.3.0,<2.0.0"
 invenio-access = ">=2.0.0,<3.0.0"
+invenio-i18n = ">=2.0.0,<3.0.0"
 jsonpickle = ">=1.2"
-psutil = "^5.9.0"
+psutil = ">=5.9.0"
 pycountry = ">=19.7.15"
-python-dateutil = "^2.8.2"
-mock = "^4.0.3"
-pytest-invenio = ">=2.1.0,<=3.0.0"
+python-dateutil = ">=2.8.2"
 # Pinned due to before_first_request deprecation https://flask.palletsprojects.com/en/2.2.x/api/#flask.Flask.before_first_request
 Flask = ">=2.2.0,<2.3.0"
-invenio-i18n = ">=2.0.0,<3.0.0"
-SQLAlchemy = ">=1.2.18,<1.5.0"
-SQLAlchemy-Utils = ">=0.33.1,<0.39"
 
 [tool.poetry.dev-dependencies]
-pytest-invenio = ">=2.1.0,<=3.0.0"
-pydocstyle = ">=6.1.1"
-autoflake = ">=1.3.1"
+pytest-black-ng = ">=0.4.0"
+pytest-invenio = ">=2.1.6,<3.0.0"
 Sphinx = ">=4.5.0"
+pydocstyle = ">=6.1.1,<6.2"
+autoflake = ">=1.3.1"
+mock = ">=4.0.3"
 
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.plugins."invenio_base.apps"]
 invenio_sip2 = "invenio_sip2:InvenioSIP2"
```

### Comparing `invenio_sip2-0.6.22/setup.py` & `invenio_sip2-0.6.23/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,38 +17,34 @@
                   'translations/es/LC_MESSAGES/*',
                   'translations/fr/LC_MESSAGES/*',
                   'translations/it/LC_MESSAGES/*',
                   'translations/nl/LC_MESSAGES/*']}
 
 install_requires = \
 ['Flask>=2.2.0,<2.3.0',
- 'SQLAlchemy-Utils>=0.33.1,<0.39',
- 'SQLAlchemy>=1.2.18,<1.5.0',
  'invenio-access>=2.0.0,<3.0.0',
- 'invenio-base>=1.2.11,<1.3.0',
+ 'invenio-base>=1.3.0,<2.0.0',
  'invenio-i18n>=2.0.0,<3.0.0',
  'jsonpickle>=1.2',
- 'mock>=4.0.3,<5.0.0',
- 'psutil>=5.9.0,<6.0.0',
+ 'psutil>=5.9.0',
  'pycountry>=19.7.15',
- 'pytest-invenio>=2.1.0,<=3.0.0',
- 'python-dateutil>=2.8.2,<3.0.0']
+ 'python-dateutil>=2.8.2']
 
 entry_points = \
 {'flask.commands': ['selfcheck = invenio_sip2.cli:selfcheck'],
  'invenio_base.api_apps': ['invenio_sip2 = invenio_sip2:InvenioSIP2'],
  'invenio_base.api_blueprints': ['invenio_sip2 = '
                                  'invenio_sip2.views.rest:api_blueprint'],
  'invenio_base.apps': ['invenio_sip2 = invenio_sip2:InvenioSIP2'],
  'invenio_base.blueprints': ['invenio_sip2 = '
                              'invenio_sip2.views.views:blueprint']}
 
 setup_kwargs = {
     'name': 'invenio-sip2',
-    'version': '0.6.22',
+    'version': '0.6.23',
     'description': 'Invenio module that add a SIP2 communication for library self-check service',
     'long_description': '..\n    INVENIO-SIP2\n    Copyright (C) 2020 UCLouvain\n\n    This program is free software: you can redistribute it and/or modify\n    it under the terms of the GNU Affero General Public License as published by\n    the Free Software Foundation, version 3 of the License.\n\n    This program is distributed in the hope that it will be useful,\n    but WITHOUT ANY WARRANTY; without even the implied warranty of\n    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the\n    GNU Affero General Public License for more details.\n\n    You should have received a copy of the GNU Affero General Public License\n    along with this program. If not, see <http://www.gnu.org/licenses/>.\n\n==============\n Invenio-SIP2\n==============\n\n.. image:: https://img.shields.io/travis/inveniosoftware-contrib/invenio-sip2.svg\n        :target: https://travis-ci.org/inveniosoftware-contrib/invenio-sip2\n\n.. image:: https://img.shields.io/coveralls/inveniosoftware-contrib/invenio-sip2.svg\n        :target: https://coveralls.io/github/inveniosoftware-contrib/invenio-sip2\n\n.. image:: https://img.shields.io/github/tag/inveniosoftware-contrib/invenio-sip2.svg\n        :target: https://github.com/inveniosoftware-contrib/invenio-sip2/releases\n\n.. image:: https://img.shields.io/github/license/inveniosoftware-contrib/invenio-sip2.svg\n        :target: https://github.com/inveniosoftware-contrib/invenio-sip2/blob/master/LICENSE\n\nInvenio module that add a SIP2 interface between a library’s Automated\nCirculation System and library automation devices.\n\nThis project is in work in progress. Some features may not yet be implemented.\n\nFurther documentation is available on\nhttps://invenio-sip2.readthedocs.io/\n\nImplemented SIP2 Features\n=========================\n- Login\n- Selfcheck Status\n- Request Resend\n- Patron Status\n- Patron Enable\n- End Patron Session\n- Patron Information\n- Item Information\n- Checkout\n- Checkin\n- Renew\n- Fee Paid\n',
     'author': 'Laurent Dubois',
     'author_email': 'laurent.dubois@uclouvain.be',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/inveniosoftware-contrib/invenio-sip2',
```

### Comparing `invenio_sip2-0.6.22/PKG-INFO` & `invenio_sip2-0.6.23/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-sip2
-Version: 0.6.22
+Version: 0.6.23
 Summary: Invenio module that add a SIP2 communication for library self-check service
 Home-page: https://github.com/inveniosoftware-contrib/invenio-sip2
 License: AGPL-3.0
 Author: Laurent Dubois
 Author-email: laurent.dubois@uclouvain.be
 Requires-Python: >=3.7,<3.10
 Classifier: Development Status :: 3 - Alpha
@@ -20,25 +20,21 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: Flask (>=2.2.0,<2.3.0)
-Requires-Dist: SQLAlchemy (>=1.2.18,<1.5.0)
-Requires-Dist: SQLAlchemy-Utils (>=0.33.1,<0.39)
 Requires-Dist: invenio-access (>=2.0.0,<3.0.0)
-Requires-Dist: invenio-base (>=1.2.11,<1.3.0)
+Requires-Dist: invenio-base (>=1.3.0,<2.0.0)
 Requires-Dist: invenio-i18n (>=2.0.0,<3.0.0)
 Requires-Dist: jsonpickle (>=1.2)
-Requires-Dist: mock (>=4.0.3,<5.0.0)
-Requires-Dist: psutil (>=5.9.0,<6.0.0)
+Requires-Dist: psutil (>=5.9.0)
 Requires-Dist: pycountry (>=19.7.15)
-Requires-Dist: pytest-invenio (>=2.1.0,<=3.0.0)
-Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
+Requires-Dist: python-dateutil (>=2.8.2)
 Project-URL: Documentation, https://invenio-sip2.readthedocs.io
 Project-URL: Repository, https://github.com/inveniosoftware-contrib/invenio-sip2
 Description-Content-Type: text/x-rst
 
 ..
     INVENIO-SIP2
     Copyright (C) 2020 UCLouvain
```

