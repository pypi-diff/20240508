# Comparing `tmp/snap_saas_base-0.9.0.tar.gz` & `tmp/snap_saas_base-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snap_saas_base-0.9.0.tar", max compression
+gzip compressed data, was "snap_saas_base-0.9.1.tar", max compression
```

## Comparing `snap_saas_base-0.9.0.tar` & `snap_saas_base-0.9.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     6775 2024-02-19 20:13:18.774029 snap_saas_base-0.9.0/README.md
--rw-r--r--   0        0        0     4267 2024-02-19 20:13:18.782029 snap_saas_base-0.9.0/pyproject.toml
--rw-r--r--   0        0        0       31 2024-02-19 20:13:18.782029 snap_saas_base-0.9.0/src/snap_saas_base/__init__.py
--rw-r--r--   0        0        0       31 2024-02-19 20:13:18.782029 snap_saas_base-0.9.0/src/snap_saas_base/models/__init__.py
--rw-r--r--   0        0        0     2214 2024-02-19 20:13:18.782029 snap_saas_base-0.9.0/src/snap_saas_base/models/base_model.py
--rw-r--r--   0        0        0     5767 2024-02-19 20:13:18.782029 snap_saas_base-0.9.0/src/snap_saas_base/models/organization.py
--rw-r--r--   0        0        0     3335 2024-02-19 20:13:18.782029 snap_saas_base-0.9.0/src/snap_saas_base/models/user.py
--rw-r--r--   0        0        0    14168 2024-02-19 20:13:18.782029 snap_saas_base-0.9.0/src/snap_saas_base/models/workspace.py
--rw-r--r--   0        0        0        0 2024-02-19 20:13:18.782029 snap_saas_base-0.9.0/src/snap_saas_base/py.typed
--rw-r--r--   0        0        0       39 2024-02-19 20:13:18.782029 snap_saas_base-0.9.0/src/snap_saas_base/schemas/__init__.py
--rw-r--r--   0        0        0     3773 2024-02-19 20:13:18.782029 snap_saas_base-0.9.0/src/snap_saas_base/schemas/user.py
--rw-r--r--   0        0        0     7310 1970-01-01 00:00:00.000000 snap_saas_base-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     6775 2024-02-21 15:12:25.523268 snap_saas_base-0.9.1/README.md
+-rw-r--r--   0        0        0     4267 2024-02-21 15:12:25.527268 snap_saas_base-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0       31 2024-02-21 15:12:25.527268 snap_saas_base-0.9.1/src/snap_saas_base/__init__.py
+-rw-r--r--   0        0        0       31 2024-02-21 15:12:25.527268 snap_saas_base-0.9.1/src/snap_saas_base/models/__init__.py
+-rw-r--r--   0        0        0     2214 2024-02-21 15:12:25.527268 snap_saas_base-0.9.1/src/snap_saas_base/models/base_model.py
+-rw-r--r--   0        0        0     5767 2024-02-21 15:12:25.527268 snap_saas_base-0.9.1/src/snap_saas_base/models/organization.py
+-rw-r--r--   0        0        0     3335 2024-02-21 15:12:25.527268 snap_saas_base-0.9.1/src/snap_saas_base/models/user.py
+-rw-r--r--   0        0        0    14494 2024-02-21 15:12:25.527268 snap_saas_base-0.9.1/src/snap_saas_base/models/workspace.py
+-rw-r--r--   0        0        0        0 2024-02-21 15:12:25.527268 snap_saas_base-0.9.1/src/snap_saas_base/py.typed
+-rw-r--r--   0        0        0       39 2024-02-21 15:12:25.527268 snap_saas_base-0.9.1/src/snap_saas_base/schemas/__init__.py
+-rw-r--r--   0        0        0     3773 2024-02-21 15:12:25.527268 snap_saas_base-0.9.1/src/snap_saas_base/schemas/user.py
+-rw-r--r--   0        0        0     7310 1970-01-01 00:00:00.000000 snap_saas_base-0.9.1/PKG-INFO
```

### Comparing `snap_saas_base-0.9.0/README.md` & `snap_saas_base-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `snap_saas_base-0.9.0/pyproject.toml` & `snap_saas_base-0.9.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [build-system]  # https://python-poetry.org/docs/pyproject/#poetry-and-pep-517
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]  # https://python-poetry.org/docs/pyproject/
 name = "snap-saas-base"
-version = "0.9.0"
+version = "0.9.1"
 description = "Snap Env (https://snapenv.com) Python base module."
 authors = ["Abner G Jacobsen <abner@apoana.com.br>"]
 readme = "README.md"
 repository = "https://github.com/orgs/snapenv/snap-saas-base"
 
 [tool.commitizen]  # https://commitizen-tools.github.io/commitizen/config/
 bump_message = "bump(release): v$current_version → v$new_version"
 tag_format = "v$version"
 update_changelog_on_bump = true
-version = "0.9.0"
+version = "0.9.1"
 version_files = ["pyproject.toml:version"]
 
 [tool.poetry.dependencies]  # https://python-poetry.org/docs/dependency-specification/
 python = ">=3.11,<4.0"
 sqlalchemy = {extras = ["asyncio"], version = "^2.0.18"}
 uuid6 = "^2023.5.2"
 pydantic = {extras = ["email"], version = "^2.3.0"}
```

### Comparing `snap_saas_base-0.9.0/src/snap_saas_base/models/base_model.py` & `snap_saas_base-0.9.1/src/snap_saas_base/models/base_model.py`

 * *Files identical despite different names*

### Comparing `snap_saas_base-0.9.0/src/snap_saas_base/models/organization.py` & `snap_saas_base-0.9.1/src/snap_saas_base/models/organization.py`

 * *Files identical despite different names*

### Comparing `snap_saas_base-0.9.0/src/snap_saas_base/models/user.py` & `snap_saas_base-0.9.1/src/snap_saas_base/models/user.py`

 * *Files identical despite different names*

### Comparing `snap_saas_base-0.9.0/src/snap_saas_base/models/workspace.py` & `snap_saas_base-0.9.1/src/snap_saas_base/models/workspace.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,14 +27,16 @@
         The name of the workspace. This field is not nullable.
     slug : so.Mapped[str]
         The slug of the workspace. This field is not nullable.
     bucket : so.Mapped[str]
         The bucket of the workspace. This field is nullable.
     org_id : so.Mapped[str]
         The organization id of the workspace. This field is not nullable and is a foreign key referencing the id of the organization.
+    org : so.Mapped["Organization"]
+        an object representing the organization the workspace belongs to.
     __table_args__ : tuple
         A tuple containing a unique constraint for the combination of org_id and slug.
 
     Methods
     -------
     as_dict:
         Returns the workspace as a dictionary.
@@ -151,14 +153,16 @@
 
     Attributes
     ----------
     __tablename__ : str
         The name of the table in the database that this class maps to.
     workspace_id : so.Mapped[str]
         The ID of the workspace that this key-value pair belongs to.
+    workspace : so.Mapped["Workspace"]
+        an object representing the workspace the key-value pair belongs to.
     key : so.Mapped[str]
         The key in the key-value pair.
     value : so.Mapped[dict[str, str]]
         The value in the key-value pair.
 
     Methods
     -------
@@ -168,14 +172,15 @@
         Initializes the workspace. If no id is provided, a unique id is generated.
     """
 
     __tablename__ = "workspaces_kv"
     workspace_id: so.Mapped[str] = so.mapped_column(
         sa.ForeignKey("workspaces.id", ondelete="CASCADE"), nullable=False
     )
+    workspace: so.Mapped[Workspace] = so.relationship("Workspace", uselist=False, lazy="raise")
     key: so.Mapped[str] = so.mapped_column(nullable=False)
     value: so.Mapped[dict[str, str]] = so.mapped_column(JSONB, nullable=False)
 
     @property
     def as_dict(self):
         """Returns a dictionary representation of the WorkspaceKv object.
```

### Comparing `snap_saas_base-0.9.0/src/snap_saas_base/schemas/user.py` & `snap_saas_base-0.9.1/src/snap_saas_base/schemas/user.py`

 * *Files identical despite different names*

### Comparing `snap_saas_base-0.9.0/PKG-INFO` & `snap_saas_base-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snap-saas-base
-Version: 0.9.0
+Version: 0.9.1
 Summary: Snap Env (https://snapenv.com) Python base module.
 Home-page: https://github.com/orgs/snapenv/snap-saas-base
 Author: Abner G Jacobsen
 Author-email: abner@apoana.com.br
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

