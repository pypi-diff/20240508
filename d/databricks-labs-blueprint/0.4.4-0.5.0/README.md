# Comparing `tmp/databricks_labs_blueprint-0.4.4.tar.gz` & `tmp/databricks_labs_blueprint-0.5.0.tar.gz`

## Comparing `databricks_labs_blueprint-0.4.4.tar` & `databricks_labs_blueprint-0.5.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.4.4/databricks/__init__.py
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.4.4/databricks/labs/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.4.4/databricks/labs/blueprint/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.4.4/databricks/labs/blueprint/__init__.py
--rw-r--r--   0        0        0     4070 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.4.4/databricks/labs/blueprint/__main__.py
--rw-r--r--   0        0        0     3723 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.4.4/databricks/labs/blueprint/cli.py
--rw-r--r--   0        0        0     8420 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.4.4/databricks/labs/blueprint/commands.py
--rw-r--r--   0        0        0     2723 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.4.4/databricks/labs/blueprint/entrypoint.py
--rw-r--r--   0        0        0    42029 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.4.4/databricks/labs/blueprint/installation.py
--rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.4.4/databricks/labs/blueprint/installer.py
--rw-r--r--   0        0        0     2764 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.4.4/databricks/labs/blueprint/limiter.py
--rw-r--r--   0        0        0     3266 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.4.4/databricks/labs/blueprint/logger.py
--rw-r--r--   0        0        0     5626 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.4.4/databricks/labs/blueprint/parallel.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.4.4/databricks/labs/blueprint/py.typed
--rw-r--r--   0        0        0     5590 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.4.4/databricks/labs/blueprint/tui.py
--rw-r--r--   0        0        0     6176 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.4.4/databricks/labs/blueprint/upgrades.py
--rw-r--r--   0        0        0    12665 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.4.4/databricks/labs/blueprint/wheels.py
--rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.4.4/.gitignore
--rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.4.4/LICENSE
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.4.4/NOTICE
--rw-r--r--   0        0        0    43925 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.4.4/README.md
--rw-r--r--   0        0        0    26245 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.4.4/pyproject.toml
--rw-r--r--   0        0        0    44728 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.5.0/databricks/__init__.py
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.5.0/databricks/labs/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.5.0/databricks/labs/blueprint/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.5.0/databricks/labs/blueprint/__init__.py
+-rw-r--r--   0        0        0     4078 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.5.0/databricks/labs/blueprint/__main__.py
+-rw-r--r--   0        0        0     3723 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.5.0/databricks/labs/blueprint/cli.py
+-rw-r--r--   0        0        0     8420 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.5.0/databricks/labs/blueprint/commands.py
+-rw-r--r--   0        0        0     2723 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.5.0/databricks/labs/blueprint/entrypoint.py
+-rw-r--r--   0        0        0    42934 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.5.0/databricks/labs/blueprint/installation.py
+-rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.5.0/databricks/labs/blueprint/installer.py
+-rw-r--r--   0        0        0     2764 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.5.0/databricks/labs/blueprint/limiter.py
+-rw-r--r--   0        0        0     3292 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.5.0/databricks/labs/blueprint/logger.py
+-rw-r--r--   0        0        0     6424 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.5.0/databricks/labs/blueprint/parallel.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.5.0/databricks/labs/blueprint/py.typed
+-rw-r--r--   0        0        0     5590 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.5.0/databricks/labs/blueprint/tui.py
+-rw-r--r--   0        0        0     6176 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.5.0/databricks/labs/blueprint/upgrades.py
+-rw-r--r--   0        0        0    12749 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.5.0/databricks/labs/blueprint/wheels.py
+-rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.5.0/.gitignore
+-rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.5.0/LICENSE
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.5.0/NOTICE
+-rw-r--r--   0        0        0    43925 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.5.0/README.md
+-rw-r--r--   0        0        0    26290 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0    44728 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.5.0/PKG-INFO
```

### Comparing `databricks_labs_blueprint-0.4.4/databricks/labs/blueprint/__main__.py` & `databricks_labs_blueprint-0.5.0/databricks/labs/blueprint/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     relative_paths,
 )
 from databricks.labs.blueprint.tui import Prompts
 
 blueprint = App(__file__)
 logger = get_logger(__file__)
 
-main_py_file = '''from databricks.sdk import AccountClient, WorkspaceClient
+MAIN_PY_FILE = '''from databricks.sdk import AccountClient, WorkspaceClient
 from databricks.labs.blueprint.entrypoint import get_logger
 from databricks.labs.blueprint.cli import App
 
 __app__ = App(__file__)
 logger = get_logger(__file__)
 
 
@@ -34,15 +34,15 @@
 
 
 if "__main__" == __name__:
     __app__()
 
 '''
 
-labs_yml_file = """---
+LABS_YML_FILE = """---
 name: __app__
 description: Common libraries for Databricks Labs
 install:
   script: src/databricks/labs/__app__/__init__.py
 entrypoint: src/databricks/labs/__app__/__main__.py
 min_python: 3.10
   - name: me
@@ -88,36 +88,36 @@
         current = queue.pop(0)
         if current.name in ignore_names:
             continue
         if current.is_file():
             relative_file_name = current.as_posix().replace("blueprint", project_name)
             dst_file = dst_dir / relative_file_name
             dst_file.parent.mkdir(exist_ok=True, parents=True)
-            with current.open("r", encoding=sys.getdefaultencoding()) as r, dst_file.open("w") as w:
-                content = r.read().replace("blueprint", project_name)
+            with current.open("r", encoding=sys.getdefaultencoding()) as src, dst_file.open("w") as dst:
+                content = src.read().replace("blueprint", project_name)
                 content = content.replace("databricks-sdk", "databricks-labs-blueprint")
-                w.write(content)
+                dst.write(content)
             continue
         virtual_env_marker = current / "pyvenv.cfg"
         if virtual_env_marker.exists():
             continue
         for file in current.iterdir():
             if file.as_posix() == "src/databricks/labs/blueprint":
                 continue
             queue.append(file)
     inner_package_dir = dst_dir / "src" / "databricks" / "labs" / project_name
     inner_package_dir.mkdir(parents=True, exist_ok=True)
     with (inner_package_dir / "__main__.py").open("w") as f:
-        f.write(main_py_file.replace("__app__", project_name))
+        f.write(MAIN_PY_FILE.replace("__app__", project_name))
     with (inner_package_dir / "__init__.py").open("w") as f:
         f.write(f"from databricks.labs.{project_name}.__about__ import __version__")
     with (inner_package_dir / "__about__.py").open("w") as f:
         f.write('__version__ = "0.0.0"\n')
     with (dst_dir / "labs.yml").open("w") as f:
-        f.write(labs_yml_file.replace("__app__", project_name))
+        f.write(LABS_YML_FILE.replace("__app__", project_name))
     with (dst_dir / "CODEOWNERS").open("w") as f:
         f.write(f"* @nfx\n/src @databrickslabs/{project_name}-write\n/tests @databrickslabs/{project_name}-write\n")
     with (dst_dir / "CHANGELOG.md").open("w") as f:
         f.write(f"# Version changelog\n\n## 0.0.0\n\nInitial {project_name} commit\n")
 
 
 if __name__ == "__main__":
```

### Comparing `databricks_labs_blueprint-0.4.4/databricks/labs/blueprint/cli.py` & `databricks_labs_blueprint-0.5.0/databricks/labs/blueprint/cli.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_blueprint-0.4.4/databricks/labs/blueprint/commands.py` & `databricks_labs_blueprint-0.5.0/databricks/labs/blueprint/commands.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_blueprint-0.4.4/databricks/labs/blueprint/entrypoint.py` & `databricks_labs_blueprint-0.5.0/databricks/labs/blueprint/entrypoint.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_blueprint-0.4.4/databricks/labs/blueprint/installation.py` & `databricks_labs_blueprint-0.5.0/databricks/labs/blueprint/installation.py`

 * *Files 1% similar despite different names*

```diff
@@ -402,18 +402,18 @@
             return converters[extension](raw)
         except JSONDecodeError:
             return {}
 
     def __repr__(self):
         return self.install_folder()
 
-    def __eq__(self, o):
-        if not isinstance(o, Installation):
+    def __eq__(self, other):
+        if not isinstance(other, Installation):
             return False
-        return self.install_folder() == o.install_folder()
+        return self.install_folder() == other.install_folder()
 
     def __hash__(self):
         """The `__hash__` method is used to hash the `Installation` object.
         This method is called by the `hash` function."""
         return hash(self.install_folder())
 
     @staticmethod
@@ -469,43 +469,46 @@
         item_type = type(from_list[0])  # type: ignore[misc]
         return list[item_type]  # type: ignore[valid-type]
 
     @classmethod
     def _marshal(cls, type_ref: type, path: list[str], inst: Any) -> tuple[Any, bool]:
         """The `_marshal` method is a private method that is used to serialize an object of type `type_ref` to
         a dictionary. This method is called by the `save` method."""
-        # pylint: disable-next=import-outside-toplevel
-        from typing import (  # type: ignore[attr-defined]
-            _GenericAlias,
-            _UnionGenericAlias,
-        )
-
         if hasattr(inst, "as_dict"):
             return inst.as_dict(), True
         if dataclasses.is_dataclass(type_ref):
             return cls._marshal_dataclass(type_ref, path, inst)
-        if isinstance(type_ref, (types.UnionType, _UnionGenericAlias)):  # type: ignore[attr-defined]
-            return cls._marshal_union(type_ref, path, inst)
-        if isinstance(type_ref, (_GenericAlias, types.GenericAlias)):  # type: ignore[attr-defined]
-            if type_ref.__origin__ in (dict, list) or isinstance(type_ref, types.GenericAlias):
-                return cls._marshal_generic(type_ref, path, inst)
-            return cls._marshal_generic_alias(type_ref, inst)
         if isinstance(inst, databricks.sdk.core.Config):
             return inst.as_dict(), True
         if type_ref == list:
             return cls._marshal_list(type_ref, path, inst)
         if isinstance(type_ref, enum.EnumMeta):
             return cls._marshal_enum(inst)
         if type_ref == types.NoneType:
             return inst, inst is None
         if type_ref == databricks.sdk.core.Config:
             return cls._marshal_databricks_config(inst)
         if type_ref in cls._PRIMITIVES:
             return inst, True
+        return cls._marshal_generic_types(type_ref, path, inst)
 
+    @classmethod
+    def _marshal_generic_types(cls, type_ref: type, path: list[str], inst: Any) -> tuple[Any, bool]:
+        # pylint: disable-next=import-outside-toplevel,import-private-name
+        from typing import (  # type: ignore[attr-defined]
+            _GenericAlias,
+            _UnionGenericAlias,
+        )
+
+        if isinstance(type_ref, (types.UnionType, _UnionGenericAlias)):  # type: ignore[attr-defined]
+            return cls._marshal_union(type_ref, path, inst)
+        if isinstance(type_ref, (_GenericAlias, types.GenericAlias)):  # type: ignore[attr-defined]
+            if type_ref.__origin__ in (dict, list) or isinstance(type_ref, types.GenericAlias):
+                return cls._marshal_generic(type_ref, path, inst)
+            return cls._marshal_generic_alias(type_ref, inst)
         raise SerdeError(f'{".".join(path)}: unknown: {inst}')
 
     @classmethod
     def _marshal_union(cls, type_ref: type, path: list[str], inst: Any) -> tuple[Any, bool]:
         """The `_marshal_union` method is a private method that is used to serialize an object of type `type_ref` to
         a dictionary. This method is called by the `save` method."""
         combo = []
@@ -608,40 +611,44 @@
         def from_dict(cls, raw: dict):
             pass
 
     @classmethod
     def _unmarshal(cls, inst: Any, path: list[str], type_ref: type[T]) -> T | None:
         """The `_unmarshal` method is a private method that is used to deserialize a dictionary to an object of type
         `type_ref`. This method is called by the `load` method."""
-        # pylint: disable-next=import-outside-toplevel
-        from typing import (  # type: ignore[attr-defined]
-            _GenericAlias,
-            _UnionGenericAlias,
-        )
-
         if dataclasses.is_dataclass(type_ref):
             return cls._unmarshal_dataclass(inst, path, type_ref)
-        if isinstance(type_ref, (types.UnionType, _UnionGenericAlias)):
-            return cls._unmarshal_union(inst, path, type_ref)
-        if isinstance(type_ref, (_GenericAlias, types.GenericAlias)):
-            return cls._unmarshal_generic(inst, path, type_ref)
         if isinstance(type_ref, enum.EnumMeta):
             if not inst:
                 return None
             return type_ref(inst)
         if type_ref in cls._PRIMITIVES:
             return cls._unmarshal_primitive(inst, type_ref)
         if type_ref == databricks.sdk.core.Config:
             if not inst:
                 inst = {}
             return databricks.sdk.core.Config(**inst)  # type: ignore[return-value]
         if type_ref == types.NoneType:
             return None
         if isinstance(type_ref, cls._FromDict):
             return type_ref.from_dict(inst)
+        return cls._unmarshal_generic_types(type_ref, path, inst)
+
+    @classmethod
+    def _unmarshal_generic_types(cls, type_ref, path, inst):
+        # pylint: disable-next=import-outside-toplevel,import-private-name
+        from typing import (  # type: ignore[attr-defined]
+            _GenericAlias,
+            _UnionGenericAlias,
+        )
+
+        if isinstance(type_ref, (types.UnionType, _UnionGenericAlias)):
+            return cls._unmarshal_union(inst, path, type_ref)
+        if isinstance(type_ref, (_GenericAlias, types.GenericAlias)):
+            return cls._unmarshal_generic(inst, path, type_ref)
         raise SerdeError(f'{".".join(path)}: unknown: {type_ref}: {inst}')
 
     @classmethod
     def _unmarshal_dataclass(cls, inst, path, type_ref):
         """The `_unmarshal_dataclass` method is a private method that is used to deserialize a dictionary to an object
         of type `type_ref`. This method is called by the `load` method."""
         if inst is None:
@@ -679,15 +686,15 @@
                 return value
         return None
 
     @classmethod
     def _unmarshal_generic(cls, inst, path, type_ref):
         """The `_unmarshal_generic` method is a private method that is used to deserialize a dictionary to an object
         of type `type_ref`. This method is called by the `load` method."""
-        # pylint: disable-next=import-outside-toplevel
+        # pylint: disable-next=import-outside-toplevel,import-private-name
         from typing import _GenericAlias  # type: ignore[attr-defined]
 
         type_args = get_args(type_ref)
         if not type_args:
             raise SerdeError(f"Missing type arguments: {type_args}")
         if type_ref.__origin__ not in (dict, list) and isinstance(type_ref, _GenericAlias):
             return cls._unmarshal(inst, path, type_ref.__origin__)
@@ -892,24 +899,31 @@
         if isinstance(expected, dict):
             for k, v in expected.items():
                 if v == ...:
                     self._overwrites[filename][k] = ...
         actual = self._overwrites[filename]
         assert expected == actual, f"{filename} content missmatch"
 
-    def assert_file_uploaded(self, filename):
-        self._assert_upload(filename, self._uploads)
-
-    def assert_file_dbfs_uploaded(self, filename):
-        self._assert_upload(filename, self._dbfs)
+    def assert_file_uploaded(self, filename, expected: bytes | None = None):
+        """Asserts that a file was uploaded with the expected content"""
+        self._assert_upload(filename, self._uploads, expected)
+
+    def assert_file_dbfs_uploaded(self, filename, expected: bytes | None = None):
+        """Asserts that a file was uploaded to DBFS with the expected content"""
+        self._assert_upload(filename, self._dbfs, expected)
 
     def assert_removed(self):
         assert self._removed
 
     @staticmethod
-    def _assert_upload(filename: Any, loc: dict[str, bytes]):
+    def _assert_upload(filename: Any, loc: dict[str, bytes], expected: bytes | None = None):
         if isinstance(filename, re.Pattern):
             for name in loc.keys():
-                if filename.match(name):
-                    return
+                if not filename.match(name):
+                    continue
+                if expected:
+                    assert loc[name] == expected, f"{filename} content missmatch"
+                return
             raise AssertionError(f'Cannot find {filename.pattern} among {", ".join(loc.keys())}')
         assert filename in loc, f"{filename} had no writes"
+        if expected:
+            assert loc[filename] == expected, f"{filename} content missmatch"
```

### Comparing `databricks_labs_blueprint-0.4.4/databricks/labs/blueprint/installer.py` & `databricks_labs_blueprint-0.5.0/databricks/labs/blueprint/installer.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_blueprint-0.4.4/databricks/labs/blueprint/limiter.py` & `databricks_labs_blueprint-0.5.0/databricks/labs/blueprint/limiter.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_blueprint-0.4.4/databricks/labs/blueprint/logger.py` & `databricks_labs_blueprint-0.5.0/databricks/labs/blueprint/logger.py`

 * *Files 15% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         """Return text in bold."""
         return f"{self.BOLD}{text}{self.RESET}"
 
     def format(self, record: logging.LogRecord):  # noqa: A003
         """Format the log record. If colors are enabled, use them."""
         if not self.colors:
             return super().format(record)
-        ts = self.formatTime(record, datefmt="%H:%M:%S")
+        timestamp = self.formatTime(record, datefmt="%H:%M:%S")
         level = self._levels[record.levelno]
         # databricks.labs.ucx.foo.bar -> d.l.u.foo.bar
         module_split = record.name.split(".")
         last_two_modules = len(module_split) - 2
         name = ".".join(part if i >= last_two_modules else part[0] for i, part in enumerate(module_split))
         msg = record.msg
         if record.exc_info and not record.exc_text:
@@ -61,19 +61,19 @@
         if record.levelno in (logging.INFO, logging.WARNING):
             color_marker = self.BOLD
         elif record.levelno in (logging.ERROR, logging.FATAL):
             color_marker = self.RED + self.BOLD
         thread_name = ""
         if record.threadName != "MainThread":
             thread_name = f"[{record.threadName}]"
-        return f"{self.GRAY}{ts}{self.RESET} {level} {color_marker}[{name}]{thread_name} {msg}{self.RESET}"
+        return f"{self.GRAY}{timestamp}{self.RESET} {level} {color_marker}[{name}]{thread_name} {msg}{self.RESET}"
 
 
 def install_logger(level="DEBUG"):
     """Install a console logger with a nice formatter."""
-    for h in logging.root.handlers:
-        logging.root.removeHandler(h)
+    for handler in logging.root.handlers:
+        logging.root.removeHandler(handler)
     console_handler = logging.StreamHandler(sys.stderr)
     console_handler.setFormatter(NiceFormatter())
     console_handler.setLevel(level)
     logging.root.addHandler(console_handler)
     return console_handler
```

### Comparing `databricks_labs_blueprint-0.4.4/databricks/labs/blueprint/parallel.py` & `databricks_labs_blueprint-0.5.0/databricks/labs/blueprint/parallel.py`

 * *Files 8% similar despite different names*

```diff
@@ -127,19 +127,38 @@
             since = dt.datetime.now() - self._started
             rps = self._completed_cnt / since.total_seconds()
             if self._completed_cnt % log_every == 0 or self._completed_cnt == total_cnt:
                 msg = f"{self._name} {self._completed_cnt}/{total_cnt}, rps: {rps:.3f}/sec"
                 logger.info(msg)
 
     @staticmethod
-    def _wrap_result(func, name):
+    def _get_result_function_signature(func, name):
+        if not isinstance(func, functools.partial):
+            return name
+
+        # try to build up signature, this should never fail
+        try:
+            args = []
+            args.extend(repr(x) for x in func.args)
+            args.extend(f"{k}={v!r}" for (k, v) in func.keywords.items())
+            args_str = ", ".join(args)
+            if args_str:
+                return f"{name}({args_str})"
+            return name
+        # but if it would ever fail, better return generic serialized name, than messing up traceback even more...
+        except Exception:  # pylint: disable=broad-exception-caught
+            return str(func)
+
+    @classmethod
+    def _wrap_result(cls, func, name):
         """This method emulates GoLang's error return style"""
 
         @functools.wraps(func)
         def inner(*args, **kwargs):
             try:
                 return func(*args, **kwargs), None
             except Exception as err:  # pylint: disable=broad-exception-caught
-                logger.error(f"{name} task failed: {err!s}", exc_info=err)
+                signature = cls._get_result_function_signature(func, name)
+                logger.error(f"{signature} task failed: {err!s}", exc_info=err)
                 return None, err
 
         return inner
```

### Comparing `databricks_labs_blueprint-0.4.4/databricks/labs/blueprint/tui.py` & `databricks_labs_blueprint-0.5.0/databricks/labs/blueprint/tui.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_blueprint-0.4.4/databricks/labs/blueprint/upgrades.py` & `databricks_labs_blueprint-0.5.0/databricks/labs/blueprint/upgrades.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_blueprint-0.4.4/databricks/labs/blueprint/wheels.py` & `databricks_labs_blueprint-0.5.0/databricks/labs/blueprint/wheels.py`

 * *Files 2% similar despite different names*

```diff
@@ -145,22 +145,22 @@
                 return f"{first}-{second}"
         charset = string.ascii_uppercase + string.ascii_lowercase + string.digits
         return "".join(random.choices(charset, k=int(k)))
 
     @staticmethod
     def _semver_and_pep440(git_detached_version: str) -> str:
         """Create a version that is both SemVer and PEP440 compliant."""
-        dv = SemVer.parse(git_detached_version)
+        detached_version = SemVer.parse(git_detached_version)
         datestamp = datetime.now().strftime("%Y%m%d%H%M%S")
         # new commits on main branch since the last tag
-        new_commits = dv.pre_release.split("-")[0] if dv.pre_release else None
+        new_commits = detached_version.pre_release.split("-")[0] if detached_version.pre_release else None
         # show that it's a version different from the released one in stats
-        bump_patch = dv.patch + 1
+        bump_patch = detached_version.patch + 1
         # create something that is both https://semver.org and https://peps.python.org/pep-0440/
-        semver_and_pep0440 = f"{dv.major}.{dv.minor}.{bump_patch}+{new_commits}{datestamp}"
+        semver_and_pep0440 = f"{detached_version.major}.{detached_version.minor}.{bump_patch}+{new_commits}{datestamp}"
         # validate the semver
         SemVer.parse(semver_and_pep0440)
         return semver_and_pep0440
 
     @classmethod
     def _infer_version_file(cls, start: Path, version_file_names: list[str]) -> Path:
         # be aware, that WheelsV2 overwrites this wheel file with unreleased version identifier,
```

### Comparing `databricks_labs_blueprint-0.4.4/.gitignore` & `databricks_labs_blueprint-0.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `databricks_labs_blueprint-0.4.4/LICENSE` & `databricks_labs_blueprint-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `databricks_labs_blueprint-0.4.4/README.md` & `databricks_labs_blueprint-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `databricks_labs_blueprint-0.4.4/pyproject.toml` & `databricks_labs_blueprint-0.5.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -33,40 +33,41 @@
 
 [tool.hatch.version]
 path = "src/databricks/labs/blueprint/__about__.py"
 
 [tool.hatch.envs.default]
 dependencies = [
     "databricks-labs-blueprint[yaml]",
-    "coverage[toml]>=6.5",
-    "pytest",
-    "pylint",
-    "pytest-xdist",
-    "pytest-cov>=4.0.0,<5.0.0",
-    "pytest-mock>=3.0.0,<4.0.0",
-    "pytest-timeout",
-    "ruff>=0.0.243",
-    "isort>=2.5.0",
-    "mypy",
-    "types-PyYAML",
-    "types-requests",
+    "coverage[toml]~=7.4.4",
+    "mypy~=1.9.0",
+    "pylint~=3.1.0",
+    "pylint-pytest==2.0.0a0",
+    "databricks-labs-pylint~=0.3.0",
+    "pytest~=8.1.0",
+    "pytest-cov~=4.1.0",
+    "pytest-mock~=3.14.0",
+    "pytest-timeout~=2.3.1",
+    "pytest-xdist~=3.5.0",
+    "ruff~=0.3.4",
+    "types-PyYAML~=6.0.12",
+    "types-requests~=2.31.0",
 ]
 
 python="3.10"
 
 # store virtual env as the child of this folder. Helps VSCode (and PyCharm) to run better
 path = ".venv"
 
 [tool.hatch.envs.default.scripts]
 test        = "pytest -n 2 --cov src --cov-report=xml --timeout 30 tests/unit --durations 20"
 coverage    = "pytest -n 2 --cov src tests/unit --timeout 30 --cov-report=html --durations 20"
 integration = "pytest -n 10 --cov src tests/integration --durations 20"
 fmt         = ["isort .",
                "ruff format",
-               "ruff  . --fix",
+               "ruff check . --fix",
                "mypy .",
                "pylint --output-format=colorized -j 0 src"]
 verify      = ["black --check .",
                "isort . --check-only",
                "ruff .",
                "mypy .",
                "pylint --output-format=colorized -j 0 src"]
@@ -84,15 +85,15 @@
 skip-string-normalization = true
 
 [tool.ruff]
 cache-dir = ".venv/ruff-cache"
 target-version = "py310"
 line-length = 120
 
-[tool.ruff.isort]
+[tool.ruff.lint.isort]
 known-first-party = ["databricks.labs.blueprint"]
 
 [tool.coverage.run]
 branch = true
 parallel = true
 
 [tool.coverage.report]
@@ -104,19 +105,14 @@
 ]
 
 [tool.pylint.main]
 # PyLint configuration is adapted from Google Python Style Guide with modifications.
 # Sources https://google.github.io/styleguide/pylintrc
 # License: https://github.com/google/styleguide/blob/gh-pages/LICENSE
 
-# Analyse import fallback blocks. This can be used to support both Python 2 and 3
-# compatible code, which means that the block might have code that exists only in
-# one or another interpreter, leading to false positives when analysed.
-# analyse-fallback-blocks =
-
 # Clear in-memory caches upon conclusion of linting. Useful if running pylint in
 # a server-like mode.
 # clear-cache-post-run =
 
 # Always return a 0 (non-error) status code, even if lint errors are found. This
 # is primarily useful in continuous integration scripts.
 # exit-zero =
@@ -128,19 +124,14 @@
 
 # A comma-separated list of package or module names from where C extensions may
 # be loaded. Extensions are loading into the active Python interpreter and may
 # run arbitrary code. (This is an alternative name to extension-pkg-allow-list
 # for backward compatibility.)
 # extension-pkg-whitelist =
 
-# Return non-zero exit code if any of these messages/categories are detected,
-# even if score is above --fail-under value. Syntax same as enable. Messages
-# specified are enabled, while categories only check already-enabled messages.
-# fail-on =
-
 # Specify a score threshold under which the program will exit with error.
 fail-under = 10.0
 
 # Interpret the stdin as a python script, whose filename needs to be passed as
 # the module_or_package argument.
 # from-stdin =
 
@@ -164,24 +155,44 @@
 # Python code to execute, usually for sys.path manipulation such as
 # pygtk.require().
 # init-hook =
 
 # Use multiple processes to speed up Pylint. Specifying 0 will auto-detect the
 # number of processors available to use, and will cap the count on Windows to
 # avoid hangs.
-# jobs =
+jobs = 0
 
 # Control the amount of potential inferred values when inferring a single object.
 # This can help the performance when dealing with large functions or complex,
 # nested conditions.
 limit-inference-results = 100
 
 # List of plugins (as comma separated values of python module names) to load,
 # usually to register additional checkers.
-load-plugins = ["pylint.extensions.check_elif", "pylint.extensions.bad_builtin", "pylint.extensions.docparams", "pylint.extensions.for_any_all", "pylint.extensions.set_membership", "pylint.extensions.code_style", "pylint.extensions.overlapping_exceptions", "pylint.extensions.typing", "pylint.extensions.redefined_variable_type", "pylint.extensions.comparison_placement", "pylint.extensions.broad_try_clause", "pylint.extensions.dict_init_mutate", "pylint.extensions.consider_refactoring_into_while_condition"]
+load-plugins = [
+    "databricks.labs.pylint.all",
+    "pylint_pytest",
+    "pylint.extensions.bad_builtin",
+    "pylint.extensions.broad_try_clause",
+    "pylint.extensions.check_elif",
+    "pylint.extensions.code_style",
+    "pylint.extensions.confusing_elif",
+    "pylint.extensions.comparison_placement",
+    "pylint.extensions.consider_refactoring_into_while_condition",
+    "pylint.extensions.dict_init_mutate",
+    "pylint.extensions.docparams",
+    "pylint.extensions.dunder",
+    "pylint.extensions.for_any_all",
+    "pylint.extensions.mccabe",
+    "pylint.extensions.overlapping_exceptions",
+    "pylint.extensions.private_import",
+    "pylint.extensions.redefined_variable_type",
+    "pylint.extensions.set_membership",
+    "pylint.extensions.typing",
+]
 
 # Pickle collected data for later comparisons.
 persistent = true
 
 # Minimum Python version to use for version dependent checks. Will default to the
 # version used to run pylint.
 py-version = "3.10"
@@ -213,30 +224,30 @@
 
 # Naming style matching correct attribute names.
 attr-naming-style = "snake_case"
 
 # Regular expression matching correct attribute names. Overrides attr-naming-
 # style. If left empty, attribute names will be checked with the set naming
 # style.
-attr-rgx = "[a-z_][a-z0-9_]{2,}$"
+attr-rgx = "[a-z_][a-z0-9_]{1,}$"
 
 # Bad variable names which should always be refused, separated by a comma.
 bad-names = ["foo", "bar", "baz", "toto", "tutu", "tata"]
 
 # Bad variable names regexes, separated by a comma. If names match any regex,
 # they will always be refused
 # bad-names-rgxs =
 
 # Naming style matching correct class attribute names.
 class-attribute-naming-style = "any"
 
 # Regular expression matching correct class attribute names. Overrides class-
 # attribute-naming-style. If left empty, class attribute names will be checked
 # with the set naming style.
-class-attribute-rgx = "([A-Za-z_][A-Za-z0-9_]{2,30}|(__.*__))$"
+class-attribute-rgx = "([A-Za-z_][A-Za-z0-9_]{1,30}|(__.*__))$"
 
 # Naming style matching correct class constant names.
 class-const-naming-style = "UPPER_CASE"
 
 # Regular expression matching correct class constant names. Overrides class-
 # const-naming-style. If left empty, class constant names will be checked with
 # the set naming style.
@@ -261,18 +272,29 @@
 docstring-min-length = -1
 
 # Naming style matching correct function names.
 function-naming-style = "snake_case"
 
 # Regular expression matching correct function names. Overrides function-naming-
 # style. If left empty, function names will be checked with the set naming style.
-function-rgx = "[a-z_][a-z0-9_]{2,30}$"
+function-rgx = "[a-z_][a-z0-9_]{2,}$"
 
 # Good variable names which should always be accepted, separated by a comma.
-good-names = ["i", "j", "k", "ex", "Run", "_"]
+good-names = [
+    "i", "j", "k", "v",  # use for loops
+    "f",            # use for file handles
+    "df",           # use for pyspark.sql.DataFrame
+    "ex", "e",      # use for exceptions
+    "fn", "cb",     # use for callbacks
+    "_", "ok",      # use for ignores
+    "a",            # use for databricks.sdk.AccountClient
+    "w", "ws",      # use for databricks.sdk.WorkspaceClient
+    "me",           # use for current user
+    "T"             # use for type variables
+]
 
 # Good variable names regexes, separated by a comma. If names match any regex,
 # they will always be accepted
 # good-names-rgxs =
 
 # Include a hint for the correct naming format with invalid-name.
 # include-naming-hint =
@@ -286,15 +308,16 @@
 inlinevar-rgx = "[A-Za-z_][A-Za-z0-9_]*$"
 
 # Naming style matching correct method names.
 method-naming-style = "snake_case"
 
 # Regular expression matching correct method names. Overrides method-naming-
 # style. If left empty, method names will be checked with the set naming style.
-method-rgx = "[a-z_][a-z0-9_]{2,}$"
+# Special exception is for `visit_` methods related to AST visitors.
+method-rgx = "(([a-z_][a-z0-9_]{2,})|(visit_.*))$"
 
 # Naming style matching correct module names.
 module-naming-style = "snake_case"
 
 # Regular expression matching correct module names. Overrides module-naming-
 # style. If left empty, module names will be checked with the set naming style.
 module-rgx = "(([a-z_][a-z0-9_]*)|([A-Z][a-zA-Z0-9]+))$"
@@ -455,15 +478,15 @@
 
 # Couples of modules and preferred modules, separated by a comma.
 # preferred-modules =
 
 [tool.pylint.logging]
 # The type of string formatting that logging methods do. `old` means using %
 # formatting, `new` is for `{}` formatting.
-logging-format-style = "old"
+logging-format-style = "new"
 
 # Logging modules to check that the string format arguments are in logging
 # function parameter format.
 logging-modules = ["logging"]
 
 [tool.pylint."messages control"]
 # Only show warnings with the listed confidence levels. Leave empty to show all.
@@ -475,15 +498,33 @@
 # multiple times (only on the command line, not in the configuration file where
 # it should appear only once). You can also use "--disable=all" to disable
 # everything first and then re-enable specific checks. For example, if you want
 # to run only the similarities checker, you can use "--disable=all
 # --enable=similarities". If you want to run only the classes checker, but have
 # no Warning level messages displayed, use "--disable=all --enable=classes
 # --disable=W".
-disable = ["raw-checker-failed", "bad-inline-option", "locally-disabled", "file-ignored", "suppressed-message", "deprecated-pragma", "use-implicit-booleaness-not-comparison-to-string", "use-implicit-booleaness-not-comparison-to-zero", "consider-using-augmented-assign", "prefer-typing-namedtuple", "attribute-defined-outside-init", "invalid-name", "missing-module-docstring", "missing-class-docstring", "missing-function-docstring", "protected-access", "too-few-public-methods", "line-too-long", "too-many-lines", "trailing-whitespace", "missing-final-newline", "trailing-newlines", "bad-indentation", "unnecessary-semicolon", "multiple-statements", "superfluous-parens", "mixed-line-endings", "unexpected-line-ending-format", "fixme", "consider-using-assignment-expr", "logging-fstring-interpolation", "consider-using-any-or-all"]
+disable = [
+    "prefer-typing-namedtuple",
+    "attribute-defined-outside-init",
+    "missing-module-docstring",
+    "missing-class-docstring",
+    "missing-function-docstring",
+    "too-few-public-methods",
+    "line-too-long",
+    "trailing-whitespace",
+    "missing-final-newline",
+    "trailing-newlines",
+    "unnecessary-semicolon",
+    "mixed-line-endings",
+    "unexpected-line-ending-format",
+    "fixme",
+    "consider-using-assignment-expr",
+    "logging-fstring-interpolation",
+    "consider-using-any-or-all"
+]
 
 # Enable the message, report, category or checker with the given id(s). You can
 # either give multiple identifier separated by comma (,) or put this option
 # multiple time (only on the command line, not in the configuration file where it
 # should appear only once). See also the "--disable" option for examples.
 enable = ["useless-suppression", "use-symbolic-message-instead"]
 
@@ -518,15 +559,15 @@
 
 # If the docstring type cannot be guessed the specified docstring type will be
 # used.
 default-docstring-type = "default"
 
 [tool.pylint.refactoring]
 # Maximum number of nested blocks for function / method body
-max-nested-blocks = 5
+max-nested-blocks = 3
 
 # Complete name of functions that never returns. When checking for inconsistent-
 # return-statements if a never returning function is called then it will be
 # considered as an explicit return statement and no message will be printed.
 never-returning-functions = ["sys.exit", "argparse.parse_error"]
 
 [tool.pylint.reports]
```

### Comparing `databricks_labs_blueprint-0.4.4/PKG-INFO` & `databricks_labs_blueprint-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: databricks-labs-blueprint
-Version: 0.4.4
+Version: 0.5.0
 Summary: Common libraries for Databricks Labs
 Project-URL: Issues, https://github.com/databrickslabs/blueprint/issues
 Project-URL: Source, https://github.com/databrickslabs/blueprint
 License-File: LICENSE
 License-File: NOTICE
 Keywords: Databricks
 Classifier: Development Status :: 3 - Alpha
```

