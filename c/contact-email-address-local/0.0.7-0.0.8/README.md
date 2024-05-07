# Comparing `tmp/contact_email_address_local-0.0.7.tar.gz` & `tmp/contact_email_address_local-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "contact_email_address_local-0.0.7.tar", last modified: Thu May  2 03:58:11 2024, max compression
+gzip compressed data, was "contact_email_address_local-0.0.8.tar", last modified: Tue May  7 23:38:38 2024, max compression
```

## Comparing `contact_email_address_local-0.0.7.tar` & `contact_email_address_local-0.0.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 03:58:11.047135 contact_email_address_local-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-02 03:58:11.047135 contact_email_address_local-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-02 03:57:46.000000 contact_email_address_local-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 03:58:11.043135 contact_email_address_local-0.0.7/contact_email_address_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 03:58:11.047135 contact_email_address_local-0.0.7/contact_email_address_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 03:57:46.000000 contact_email_address_local-0.0.7/contact_email_address_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      990 2024-05-02 03:57:46.000000 contact_email_address_local-0.0.7/contact_email_address_local/src/contact_email_addresses_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     5344 2024-05-02 03:57:46.000000 contact_email_address_local-0.0.7/contact_email_address_local/src/contact_email_addresses_local.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 03:58:11.047135 contact_email_address_local-0.0.7/contact_email_address_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-02 03:58:11.000000 contact_email_address_local-0.0.7/contact_email_address_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-02 03:58:11.000000 contact_email_address_local-0.0.7/contact_email_address_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 03:58:11.000000 contact_email_address_local-0.0.7/contact_email_address_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-02 03:58:11.000000 contact_email_address_local-0.0.7/contact_email_address_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-02 03:58:11.000000 contact_email_address_local-0.0.7/contact_email_address_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-02 03:57:46.000000 contact_email_address_local-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 03:58:11.047135 contact_email_address_local-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-05-02 03:57:46.000000 contact_email_address_local-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:38:38.672177 contact_email_address_local-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-05-07 23:38:38.672177 contact_email_address_local-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-07 23:38:18.000000 contact_email_address_local-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:38:38.668177 contact_email_address_local-0.0.8/contact_email_address_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:38:38.672177 contact_email_address_local-0.0.8/contact_email_address_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 23:38:18.000000 contact_email_address_local-0.0.8/contact_email_address_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-05-07 23:38:18.000000 contact_email_address_local-0.0.8/contact_email_address_local/src/contact_email_addresses_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5386 2024-05-07 23:38:18.000000 contact_email_address_local-0.0.8/contact_email_address_local/src/contact_email_addresses_local.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:38:38.672177 contact_email_address_local-0.0.8/contact_email_address_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-05-07 23:38:38.000000 contact_email_address_local-0.0.8/contact_email_address_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-07 23:38:38.000000 contact_email_address_local-0.0.8/contact_email_address_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 23:38:38.000000 contact_email_address_local-0.0.8/contact_email_address_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-07 23:38:38.000000 contact_email_address_local-0.0.8/contact_email_address_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-07 23:38:38.000000 contact_email_address_local-0.0.8/contact_email_address_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-07 23:38:18.000000 contact_email_address_local-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 23:38:38.672177 contact_email_address_local-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-07 23:38:18.000000 contact_email_address_local-0.0.8/setup.py
```

### Comparing `contact_email_address_local-0.0.7/PKG-INFO` & `contact_email_address_local-0.0.8/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 Metadata-Version: 2.1
 Name: contact-email-address-local
-Version: 0.0.7
+Version: 0.0.8
 Summary: PyPI Package for Circles contact-email-address-local Python
-Home-page: https://github.com/circles-zone/contact-email-address-local-pyhon-package
+Home-page: https://github.com/circles-zone/contact-email-address-local-python-package
 Author: Circles
 Author-email: info@circlez.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
-Requires-Dist: PyMySQL>=1.0.2
-Requires-Dist: pytest>=7.4.0
-Requires-Dist: mysql-connector>=2.2.9
-Requires-Dist: logzio-python-handler>=4.1.0
+Requires-Dist: database-mysql-local>=0.0.197
+Requires-Dist: logger-local>=0.0.100
+Requires-Dist: email-address-local>=0.0.40
 Requires-Dist: user-context-remote>=0.0.57
-Requires-Dist: python-sdk-local>=0.0.27
-Requires-Dist: email-address-local>=0.0.24
+Requires-Dist: language-remote
 
 PyPI Package for Circles contact-email-address-local Python
```

### Comparing `contact_email_address_local-0.0.7/contact_email_address_local/src/contact_email_addresses_constants.py` & `contact_email_address_local-0.0.8/contact_email_address_local/src/contact_email_addresses_constants.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 from logger_local.LoggerComponentEnum import LoggerComponentEnum
 
-
 CONTACT_EMAIL_ADDRESSES_LOCAL_PYTHON_COMPONENT_ID = 275
 CONTACT_EMAIL_ADDRESSES_LOCAL_PYTHON_COMPONENT_NAME = "contact-email-address-local-python-package"
 DEVELOPER_EMAIL = "tal.g@circ.zone"
 CONTACT_EMAIL_ADDRESSES_PYTHON_PACKAGE_CODE_LOGGER_OBJECT = {
     'component_id': CONTACT_EMAIL_ADDRESSES_LOCAL_PYTHON_COMPONENT_ID,
     'component_name': CONTACT_EMAIL_ADDRESSES_LOCAL_PYTHON_COMPONENT_NAME,
     'component_category': LoggerComponentEnum.ComponentCategory.Code.value,
     'developer_email': DEVELOPER_EMAIL
 }
 
-
 CONTACT_EMAIL_ADDRESSES_PYTHON_PACKAGE_TEST_LOGGER_OBJECT = {
     'component_id': CONTACT_EMAIL_ADDRESSES_LOCAL_PYTHON_COMPONENT_ID,
     'component_name': CONTACT_EMAIL_ADDRESSES_LOCAL_PYTHON_COMPONENT_NAME,
     'component_category': LoggerComponentEnum.ComponentCategory.Unit_Test.value,
     'testing_framework': LoggerComponentEnum.testingFramework.pytest.value,
     'developer_email': DEVELOPER_EMAIL
-}
+}
```

### Comparing `contact_email_address_local-0.0.7/contact_email_address_local/src/contact_email_addresses_local.py` & `contact_email_address_local-0.0.8/contact_email_address_local/src/contact_email_addresses_local.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
-from .contact_email_addresses_constants import CONTACT_EMAIL_ADDRESSES_PYTHON_PACKAGE_CODE_LOGGER_OBJECT
 from database_mysql_local.generic_mapping import GenericMapping
 from email_address_local.email_address import EmailAddressesLocal
 from language_remote.lang_code import LangCode
 from logger_local.LoggerLocal import Logger
 from user_context_remote.user_context import UserContext
 
+from .contact_email_addresses_constants import CONTACT_EMAIL_ADDRESSES_PYTHON_PACKAGE_CODE_LOGGER_OBJECT
+
 logger = Logger.create_logger(object=CONTACT_EMAIL_ADDRESSES_PYTHON_PACKAGE_CODE_LOGGER_OBJECT)
 
-user_context = UserContext.login_using_user_identification_and_password()
+user_context = UserContext()
 
 DEFAULT_SCHEMA_NAME = "contact_email_address"
 DEFAULT_ENTITY_NAME1 = "contact"
 DEFAULT_ENTITY_NAME2 = "email_address"
 DEFAULT_ID_COLUMN_NAME = "contact_email_id"
 DEFAULT_TABLE_NAME = "contact_email_address_table"
 DEFAULT_VIEW_TABLE_NAME = "contact_email_address_view"
@@ -27,37 +28,39 @@
                          default_entity_name2=default_entity_name2, default_id_column_name=default_id_column_name,
                          default_table_name=default_table_name, default_view_table_name=default_view_table_name,
                          is_test_data=is_test_data)
         self.email_address_local = EmailAddressesLocal()
         self.lang_code = lang_code or user_context.get_effective_profile_preferred_lang_code()
 
     def insert_contact_and_link_to_email_address(self, contact_dict: dict, contact_email_address: str,
-                                                 contact_id: int) -> int:
+                                                 contact_id: int) -> int or None:
         """
         Insert contact and link to existing or new email address
         :param contact_dict: contact_dict
         :param contact_email_address: contact_email_address
         :param contact_id: contact_id
         :return: contact_id
         """
         logger.start(object={"contact_dict": contact_dict, "contact_email_address": contact_email_address,
-                                  "contact_id": contact_id})
+                             "contact_id": contact_id})
         if not contact_email_address:
             # TODO: we can try to look if there's an email address in the database by phone number
             # when contact-phones-local is done
             return None
-        email_address_id = self.email_address_local.get_email_address_id_by_email_address(email_address=contact_email_address)
+        email_address_id = self.email_address_local.get_email_address_id_by_email_address(
+            email_address=contact_email_address)
         if not email_address_id:
             # Create a new  email address and add it to email_address_table and email_address_ml_table
             logger.info(log_message="email_address_id is None, creating a new email address and adding it to"
-                             " email_address_table and email_address_ml_table")
+                                    " email_address_table and email_address_ml_table")
             first_name = contact_dict.get("first_name")
             last_name = contact_dict.get("last_name")
             name = f"{first_name} {last_name}"
-            email_address_id = self.email_address_local.insert(email_address=contact_email_address, lang_code=self.lang_code,
+            email_address_id = self.email_address_local.insert(email_address=contact_email_address,
+                                                               lang_code=self.lang_code,
                                                                name=name, is_test_data=self.is_test_data)
             if not email_address_id:
                 logger.error(log_message="email_address_id is None")
                 return None
             # Link contact to email address
             logger.info(log_message="Linking contact to email address")
             contact_email_address_id = self.insert_mapping(entity_name1=self.default_entity_name1,
```

### Comparing `contact_email_address_local-0.0.7/contact_email_address_local.egg-info/PKG-INFO` & `contact_email_address_local-0.0.8/contact_email_address_local.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 Metadata-Version: 2.1
 Name: contact-email-address-local
-Version: 0.0.7
+Version: 0.0.8
 Summary: PyPI Package for Circles contact-email-address-local Python
-Home-page: https://github.com/circles-zone/contact-email-address-local-pyhon-package
+Home-page: https://github.com/circles-zone/contact-email-address-local-python-package
 Author: Circles
 Author-email: info@circlez.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
-Requires-Dist: PyMySQL>=1.0.2
-Requires-Dist: pytest>=7.4.0
-Requires-Dist: mysql-connector>=2.2.9
-Requires-Dist: logzio-python-handler>=4.1.0
+Requires-Dist: database-mysql-local>=0.0.197
+Requires-Dist: logger-local>=0.0.100
+Requires-Dist: email-address-local>=0.0.40
 Requires-Dist: user-context-remote>=0.0.57
-Requires-Dist: python-sdk-local>=0.0.27
-Requires-Dist: email-address-local>=0.0.24
+Requires-Dist: language-remote
 
 PyPI Package for Circles contact-email-address-local Python
```

### Comparing `contact_email_address_local-0.0.7/setup.py` & `contact_email_address_local-0.0.8/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,32 +1,30 @@
 import setuptools
 
 PACKAGE_NAME = "contact-email-address-local"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name=PACKAGE_NAME,
-    version='0.0.7',  # update only the minor version each time # https://pypi.org/project/contact-email-address-local/
+    version='0.0.8',  # https://pypi.org/project/contact-email-address-local/
     author="Circles",
     author_email="info@circlez.ai",
     description="PyPI Package for Circles contact-email-address-local Python",
     long_description="PyPI Package for Circles contact-email-address-local Python",
     long_description_content_type='text/markdown',
-    url="https://github.com/circles-zone/contact-email-address-local-pyhon-package",  # https://pypi.org/project/contact-email-address-local/       # noqa: E501
+    url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir],
     package_dir={package_dir: f'{package_dir}/src'},
     package_data={package_dir: ['*.py']},
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: Other/Proprietary License",
         "Operating System :: OS Independent",
     ],
     install_requires=[
-        'PyMySQL>=1.0.2',
-        'pytest>=7.4.0',
-        'mysql-connector>=2.2.9',
-        'logzio-python-handler>= 4.1.0',
-        'user-context-remote>=0.0.57',
-        'python-sdk-local>=0.0.27',
-        'email-address-local>=0.0.24',
+        "database-mysql-local>=0.0.197",
+        "logger-local>=0.0.100",
+        "email-address-local>=0.0.40",
+        "user-context-remote>=0.0.57",
+        "language-remote"
     ],
 )
```

