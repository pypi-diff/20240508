# Comparing `tmp/infrable-0.1.6.tar.gz` & `tmp/infrable-0.1.7.tar.gz`

## Comparing `infrable-0.1.6.tar` & `infrable-0.1.7.tar`

### file list

```diff
@@ -1,28 +1,52 @@
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 infrable-0.1.6/.envrc
--rw-r--r--   0        0        0    17796 2020-02-02 00:00:00.000000 infrable-0.1.6/.null-ls_767818_README.md
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 infrable-0.1.6/infrable/__init__.py
--rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 infrable-0.1.6/infrable/errors.py
--rw-r--r--   0        0        0     9681 2020-02-02 00:00:00.000000 infrable-0.1.6/infrable/files.py
--rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 infrable-0.1.6/infrable/host.py
--rw-r--r--   0        0        0     2983 2020-02-02 00:00:00.000000 infrable-0.1.6/infrable/infra.py
--rw-r--r--   0        0        0     5410 2020-02-02 00:00:00.000000 infrable-0.1.6/infrable/init.py
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 infrable-0.1.6/infrable/meta.py
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 infrable-0.1.6/infrable/paths.py
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 infrable-0.1.6/infrable/readfile.py
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 infrable-0.1.6/infrable/service.py
--rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 infrable-0.1.6/infrable/switch.py
--rw-r--r--   0        0        0     3329 2020-02-02 00:00:00.000000 infrable-0.1.6/infrable/template.py
--rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 infrable-0.1.6/infrable/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 infrable-0.1.6/infrable/cli/__init__.py
--rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 infrable-0.1.6/infrable/cli/files.py
--rw-r--r--   0        0        0     2155 2020-02-02 00:00:00.000000 infrable-0.1.6/infrable/cli/main.py
--rw-r--r--   0        0        0     2551 2020-02-02 00:00:00.000000 infrable-0.1.6/infrable/cli/remote.py
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 infrable-0.1.6/infrable/cli/switch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 infrable-0.1.6/infrable/distro/__init__.py
--rw-r--r--   0        0        0     3227 2020-02-02 00:00:00.000000 infrable-0.1.6/infrable/distro/linux.py
--rw-r--r--   0        0        0     1976 2020-02-02 00:00:00.000000 infrable-0.1.6/infrable/distro/ubuntu.py
--rw-r--r--   0        0        0     3142 2020-02-02 00:00:00.000000 infrable-0.1.6/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 infrable-0.1.6/LICENSE
--rw-r--r--   0        0        0    17796 2020-02-02 00:00:00.000000 infrable-0.1.6/README.md
--rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 infrable-0.1.6/pyproject.toml
--rw-r--r--   0        0        0    31622 2020-02-02 00:00:00.000000 infrable-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 infrable-0.1.7/.envrc
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 infrable-0.1.7/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 infrable-0.1.7/infrable/__init__.py
+-rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 infrable-0.1.7/infrable/errors.py
+-rw-r--r--   0        0        0     9657 2020-02-02 00:00:00.000000 infrable-0.1.7/infrable/files.py
+-rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 infrable-0.1.7/infrable/host.py
+-rw-r--r--   0        0        0     2983 2020-02-02 00:00:00.000000 infrable-0.1.7/infrable/infra.py
+-rw-r--r--   0        0        0     5423 2020-02-02 00:00:00.000000 infrable-0.1.7/infrable/init.py
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 infrable-0.1.7/infrable/meta.py
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 infrable-0.1.7/infrable/paths.py
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 infrable-0.1.7/infrable/readfile.py
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 infrable-0.1.7/infrable/service.py
+-rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 infrable-0.1.7/infrable/switch.py
+-rw-r--r--   0        0        0     3329 2020-02-02 00:00:00.000000 infrable-0.1.7/infrable/template.py
+-rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 infrable-0.1.7/infrable/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 infrable-0.1.7/infrable/cli/__init__.py
+-rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 infrable-0.1.7/infrable/cli/files.py
+-rw-r--r--   0        0        0     2155 2020-02-02 00:00:00.000000 infrable-0.1.7/infrable/cli/main.py
+-rw-r--r--   0        0        0     2551 2020-02-02 00:00:00.000000 infrable-0.1.7/infrable/cli/remote.py
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 infrable-0.1.7/infrable/cli/switch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 infrable-0.1.7/infrable/distro/__init__.py
+-rw-r--r--   0        0        0     3227 2020-02-02 00:00:00.000000 infrable-0.1.7/infrable/distro/linux.py
+-rw-r--r--   0        0        0     1976 2020-02-02 00:00:00.000000 infrable-0.1.7/infrable/distro/ubuntu.py
+-rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 infrable-0.1.7/tests/data/files_diff
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 infrable-0.1.7/tests/data/hosts
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 infrable-0.1.7/tests/data/hosts_format
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 infrable-0.1.7/tests/data/hosts_repr
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 infrable-0.1.7/tests/data/post_files_gen
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 infrable-0.1.7/tests/data/post_init
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 infrable-0.1.7/tests/data/pre_files_gen
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 infrable-0.1.7/tests/data/pre_init
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 infrable-0.1.7/tests/data/services
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 infrable-0.1.7/tests/data/services_format
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 infrable-0.1.7/tests/data/services_repr
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 infrable-0.1.7/tests/data/switches
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 infrable-0.1.7/tests/data/switches_format
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 infrable-0.1.7/tests/data/switches_repr
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 infrable-0.1.7/tests/functional/test_custom_module.py
+-rw-r--r--   0        0        0     3088 2020-02-02 00:00:00.000000 infrable-0.1.7/tests/functional/test_files.py
+-rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 infrable-0.1.7/tests/functional/test_hosts.py
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 infrable-0.1.7/tests/functional/test_init.py
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 infrable-0.1.7/tests/functional/test_remote.py
+-rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 infrable-0.1.7/tests/functional/test_services.py
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 infrable-0.1.7/tests/functional/test_switch.py
+-rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 infrable-0.1.7/tests/functional/test_switches.py
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 infrable-0.1.7/tests/functional/test_tasks.py
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 infrable-0.1.7/tests/functional/test_workflows.py
+-rw-r--r--   0        0        0     3142 2020-02-02 00:00:00.000000 infrable-0.1.7/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 infrable-0.1.7/LICENSE
+-rw-r--r--   0        0        0    17796 2020-02-02 00:00:00.000000 infrable-0.1.7/README.md
+-rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 infrable-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0    31622 2020-02-02 00:00:00.000000 infrable-0.1.7/PKG-INFO
```

### Comparing `infrable-0.1.6/.null-ls_767818_README.md` & `infrable-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `infrable-0.1.6/infrable/__init__.py` & `infrable-0.1.7/infrable/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.1.6"
+__version__ = "0.1.7"
 
 
 from pathlib import Path
 
 INFRA_MODULE_NAME = "infra"
 IS_PROJECT_DIR = Path(f"{INFRA_MODULE_NAME}.py").exists()
```

### Comparing `infrable-0.1.6/infrable/errors.py` & `infrable-0.1.7/infrable/errors.py`

 * *Files identical despite different names*

### Comparing `infrable-0.1.6/infrable/files.py` & `infrable-0.1.7/infrable/files.py`

 * *Files 0% similar despite different names*

```diff
@@ -104,29 +104,25 @@
 
     if not paths.files.exists():
         return
 
     dirname = datetime.now().strftime("%Y-%m-%dT%H:%M:%S")
     backupdir = paths.backups / dirname
     shutil.copytree(str(paths.files), str(backupdir))
-    print()
     print(f"backup: {backupdir}")
-    print()
 
 
 def diff():
     """Diff the generated files with the pulled versions."""
 
     for new in paths.files.glob("**/*.new"):
         old = _old_path(new)
         if d := _diff(new=new, old=old):
             _print_diff(d)
             print()
-            print()
-            print()
 
 
 def push(yes: bool = False):
     """Diff and push the generated files to the remote server."""
 
     for new in paths.files.glob("**/*.new"):
         remote, loc = (
@@ -162,16 +158,14 @@
             addr = f"{host.admin}@{host.ip}"
             _sudo_push_file(addr, new, dest, chown=chown, chmod=chmod)
         else:
             print(f"skipping {remote_dest}")
             new.unlink()
             old.unlink()
         print()
-        print()
-        print()
 
 
 def revert(path: Path | None = None):
     """Revert files from backup."""
 
     if path is None:
         path = max(paths.backups.glob("*"))
@@ -194,29 +188,34 @@
 def deploy(
     path: Path | None = None, only: Iterable[str] | None = None, yes: bool = False
 ):
     """[WORKFLOW] generate, pull, backup, compare and push the generated files to the remote server."""
 
     if path or yes or typer.confirm("Generate fresh files?", default=True, err=True):
         gen(path, only=only)
+        print()
         pull()
+        print()
         backup()
     elif typer.confirm("Pull files from remote?", default=True, err=True):
         pull()
+        print()
         backup()
     elif typer.confirm("Backup files locally?", default=True, err=True):
         backup()
 
+    print()
     push(yes=yes)
 
 
 def recover(path: Path | None = None):
     """[WORKFLOW] revert and push files from backup."""
 
     revert(path)
+    print()
     push()
 
 
 def _pull(new):
     dest = str(new).removesuffix(".new") + ".old"
     remote, loc = str(new.relative_to(paths.files)).removesuffix(".new").split("/", 1)
     src = f"/{loc}"
```

### Comparing `infrable-0.1.6/infrable/host.py` & `infrable-0.1.7/infrable/host.py`

 * *Files identical despite different names*

### Comparing `infrable-0.1.6/infrable/infra.py` & `infrable-0.1.7/infrable/infra.py`

 * *Files identical despite different names*

### Comparing `infrable-0.1.6/infrable/init.py` & `infrable-0.1.7/infrable/init.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 
 nginx = Service(port=80, host=web.host)
 # /Services --------------------------------------------------------------------
 
 
 # Tasks/ -----------------------------------------------------------------------
 nginx.typer = typer.Typer(help="Nginx specific tasks.")
-@nginx.typer.command()
+@nginx.typer.command(name="reload")
 def reload_nginx():
     """[TASK] Reload nginx: infrable nginx reload"""
 
     assert nginx.host, "Service must have a host to reload"
     nginx.host.remote().sudo.nginx("-t")
     nginx.host.remote().sudo.systemctl.reload.nginx()
 # Tasks/ -----------------------------------------------------------------------
```

### Comparing `infrable-0.1.6/infrable/readfile.py` & `infrable-0.1.7/infrable/readfile.py`

 * *Files identical despite different names*

### Comparing `infrable-0.1.6/infrable/service.py` & `infrable-0.1.7/infrable/service.py`

 * *Files identical despite different names*

### Comparing `infrable-0.1.6/infrable/switch.py` & `infrable-0.1.7/infrable/switch.py`

 * *Files identical despite different names*

### Comparing `infrable-0.1.6/infrable/template.py` & `infrable-0.1.7/infrable/template.py`

 * *Files identical despite different names*

### Comparing `infrable-0.1.6/infrable/utils.py` & `infrable-0.1.7/infrable/utils.py`

 * *Files identical despite different names*

### Comparing `infrable-0.1.6/infrable/cli/files.py` & `infrable-0.1.7/infrable/cli/files.py`

 * *Files identical despite different names*

### Comparing `infrable-0.1.6/infrable/cli/main.py` & `infrable-0.1.7/infrable/cli/main.py`

 * *Files identical despite different names*

### Comparing `infrable-0.1.6/infrable/cli/remote.py` & `infrable-0.1.7/infrable/cli/remote.py`

 * *Files identical despite different names*

### Comparing `infrable-0.1.6/infrable/distro/linux.py` & `infrable-0.1.7/infrable/distro/linux.py`

 * *Files identical despite different names*

### Comparing `infrable-0.1.6/infrable/distro/ubuntu.py` & `infrable-0.1.7/infrable/distro/ubuntu.py`

 * *Files identical despite different names*

### Comparing `infrable-0.1.6/.gitignore` & `infrable-0.1.7/.gitignore`

 * *Files identical despite different names*

### Comparing `infrable-0.1.6/LICENSE` & `infrable-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `infrable-0.1.6/pyproject.toml` & `infrable-0.1.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `infrable-0.1.6/PKG-INFO` & `infrable-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: infrable
-Version: 0.1.6
+Version: 0.1.7
 Summary: Hanny's legendary infrastructure as code solution.
 Project-URL: Homepage, https://github.com/stckme/infrable
 Author-email: Arijit Basu <sayanarijit@gmail.com>
 Maintainer-email: Arijit Basu <sayanarijit@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

