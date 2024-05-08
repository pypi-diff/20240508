# Comparing `tmp/mrchef-0.7.0.tar.gz` & `tmp/mrchef-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mrchef-0.7.0.tar", max compression
+gzip compressed data, was "mrchef-0.8.1.tar", last modified: Tue Oct  3 08:34:51 2023, max compression
```

## Comparing `mrchef-0.7.0.tar` & `mrchef-0.8.1.tar`

### file list

```diff
@@ -1,9 +1,26 @@
--rw-r--r--   0        0        0    35149 2023-07-27 10:35:56.228882 mrchef-0.7.0/LICENSE
--rw-r--r--   0        0        0     5349 2023-07-27 10:35:56.228882 mrchef-0.7.0/README.md
--rw-r--r--   0        0        0       55 2023-07-27 10:35:56.229882 mrchef-0.7.0/mrchef/__init__.py
--rw-r--r--   0        0        0      177 2023-07-27 10:35:56.229882 mrchef-0.7.0/mrchef/__main__.py
--rw-r--r--   0        0        0     4857 2023-07-27 10:35:56.229882 mrchef-0.7.0/mrchef/cli.py
--rw-r--r--   0        0        0    27881 2023-07-27 10:35:56.229882 mrchef-0.7.0/mrchef/lib.py
--rw-r--r--   0        0        0      985 2023-07-27 10:35:56.229882 mrchef-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     6409 1970-01-01 00:00:00.000000 mrchef-0.7.0/setup.py
--rw-r--r--   0        0        0     6378 1970-01-01 00:00:00.000000 mrchef-0.7.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 08:34:51.930057 mrchef-0.8.1/
+-rw-rw-rw-   0 root         (0) root         (0)    35149 2023-10-03 08:32:51.000000 mrchef-0.8.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    47085 2023-10-03 08:34:51.929057 mrchef-0.8.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5291 2023-10-03 08:32:51.000000 mrchef-0.8.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 08:34:51.926057 mrchef-0.8.1/mrchef/
+-rw-rw-rw-   0 root         (0) root         (0)       55 2023-10-03 08:32:51.000000 mrchef-0.8.1/mrchef/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      104 2023-10-03 08:32:51.000000 mrchef-0.8.1/mrchef/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5307 2023-10-03 08:32:51.000000 mrchef-0.8.1/mrchef/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)    27679 2023-10-03 08:32:51.000000 mrchef-0.8.1/mrchef/lib.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 08:34:51.927057 mrchef-0.8.1/mrchef.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    47085 2023-10-03 08:34:51.000000 mrchef-0.8.1/mrchef.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      473 2023-10-03 08:34:51.000000 mrchef-0.8.1/mrchef.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-10-03 08:34:51.000000 mrchef-0.8.1/mrchef.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       49 2023-10-03 08:34:51.000000 mrchef-0.8.1/mrchef.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      215 2023-10-03 08:34:51.000000 mrchef-0.8.1/mrchef.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-10-03 08:34:51.000000 mrchef-0.8.1/mrchef.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1587 2023-10-03 08:32:51.000000 mrchef-0.8.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-10-03 08:34:51.930057 mrchef-0.8.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 08:34:51.929057 mrchef-0.8.1/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     6112 2023-10-03 08:32:51.000000 mrchef-0.8.1/tests/test_interactive.py
+-rw-rw-rw-   0 root         (0) root         (0)     4366 2023-10-03 08:32:51.000000 mrchef-0.8.1/tests/test_multiple_meals.py
+-rw-rw-rw-   0 root         (0) root         (0)      677 2023-10-03 08:32:51.000000 mrchef-0.8.1/tests/test_nix.py
+-rw-rw-rw-   0 root         (0) root         (0)     2975 2023-10-03 08:32:51.000000 mrchef-0.8.1/tests/test_not_frozen.py
+-rw-rw-rw-   0 root         (0) root         (0)      623 2023-10-03 08:32:51.000000 mrchef-0.8.1/tests/test_prefrozen_outdated.py
+-rw-rw-rw-   0 root         (0) root         (0)     6543 2023-10-03 08:32:51.000000 mrchef-0.8.1/tests/test_prefrozen_simple.py
+-rw-rw-rw-   0 root         (0) root         (0)     2920 2023-10-03 08:32:51.000000 mrchef-0.8.1/tests/test_prefrozen_spiced.py
```

### Comparing `mrchef-0.7.0/LICENSE` & `mrchef-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mrchef-0.7.0/README.md` & `mrchef-0.8.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -106,15 +106,15 @@
 
 ```sh
 mrchef --help-all
 ```
 
 ### Using Python
 
-For speed, it's highly recommended to use Python >= 3.11. Install it:
+Install it:
 
 ```sh
 pip install mrchef
 ```
 
 Use it:
```

### Comparing `mrchef-0.7.0/mrchef/cli.py` & `mrchef-0.8.1/mrchef/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,30 @@
 """Tools for command-line usage."""
 import os
-from importlib.metadata import version
+from importlib.metadata import PackageNotFoundError, version
 from pathlib import Path
 
+import rtoml
 from decorator import decorator
 from plumbum import cli
 
 from . import lib
 
 
+def _get_version():
+    """Get version from metadata or from local development environment."""
+    try:
+        return version("mrchef")
+    except PackageNotFoundError:
+        # You're developing locally using direnv
+        return rtoml.load(Path(__file__).parent.parent.joinpath("pyproject.toml"))[
+            "project"
+        ]["version"]
+
+
 @decorator
 def handle_error(function, *args, **kwargs):
     """Do not print error traces for expected errors."""
     try:
         return function(*args, **kwargs)
     except lib.MrChefError as error:
         lib.logger.log(error.trace_level, "Error trace", exc_info=True)
@@ -37,15 +49,16 @@
     - "Spices" are extra patches for the source code.
     - I am just another secondary "Chef" in the "kitchen". You are the master chef!
       I will just "freeze" or "warm up" meals for you, but you will "cook" them.
 
     Yay, I'm hungry now! 🥘
     """
 
-    VERSION = version("mrchef")
+    PROGNAME = "mrchef"  # Just in case it's being called as a module
+    VERSION = _get_version()
 
     starting_folder = cli.SwitchAttr(
         ["s", "starting-folder"],
         cli.ExistingDirectory,
         ".",
         help=f"Search for {lib.CONFIG_FILE} from this directory upwards",
     )
```

### Comparing `mrchef-0.7.0/mrchef/lib.py` & `mrchef-0.8.1/mrchef/lib.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,71 +10,32 @@
 from pathlib import Path
 from shutil import rmtree
 from textwrap import dedent
 from typing import Generator, Optional
 
 import coloredlogs
 import requests
+import rtoml
 import tomlkit
 from git_find_repos import find_repos
 from plumbum import local
 from plumbum.commands.processes import ProcessExecutionError
-from tomlkit._utils import Collection, _basic_escapes, decode, escape_string
 
 CONFIG_FILE = "mrchef.toml"
 FREEZER_FILE = ".mrchef.freezer.toml"
 
 logger = getLogger("mrchef")
 coloredlogs.install(logger=logger)
 
 # Combine with warnings
 warnings_logger = getLogger("py.warnings")
 coloredlogs.install(logger=warnings_logger)
 captureWarnings(True)
 
 
-# HACK https://github.com/sdispater/tomlkit/pull/304
-def _patched_escape_string(
-    s: str, escape_sequences: Collection[str] = _basic_escapes
-) -> str:
-    ds = decode(s)
-    found_sequences = {seq for seq in escape_sequences if seq in ds}
-    return escape_string(s, found_sequences)
-
-
-tomlkit._utils.escape_string = _patched_escape_string
-tomlkit.items.escape_string = _patched_escape_string
-
-
-def _toml_load(fd):
-    """Load TOML without any interest in preserving style.
-
-    This is a HACK because the problem it tries to solve is that tomlkit is
-    extremely slow. Just [see the report][1].
-
-    The best fix would be that tomlkit itself gets faster. But until then, this
-    works if you run Mr. Chef with Python 3.11 (which has tomllib built-in).
-
-    We only use this helper for the freezer file, because it doesn't need to
-    preserve style. Since it can contain patches, those are really slow to
-    parse and dump for tomlkit. The user config file is usually just fine with
-    it, because it's smaller.
-
-    [1]:
-    https://github.com/pwwang/toml-bench/blob/master/reports/with_python3.11.md#running-speed-with-data-provided-by-rtoml
-    """
-    try:
-        import tomllib
-
-        return tomllib.load(fd)
-    except ImportError:
-        # Not on python 3.11 yet? Well, this is gonna be slow...
-        return tomlkit.load(fd).unwrap()
-
-
 class MrChefError(Exception):
     """Core MrChef exception.
 
     It will be handled and pretty-printed when raised to CLI.
     """
 
     def __init__(self, msg: str, trace_level=DEBUG):
@@ -128,17 +89,16 @@
             self.config_user = tomlkit.load(fd)
             break
         else:
             raise MrChefError(f"No {CONFIG_FILE} file found here or in parent folders.")
         # Attempt to merge normal config with frozen one
         self.freezer_file = self.path / FREEZER_FILE
         try:
-            with self.freezer_file.open("rb") as fd:
-                # Style in the freezer isn't preserved, so we unwrap it to be faster
-                self.config_frozen = _toml_load(fd)
+            # Style in the freezer isn't preserved, so we use rtoml it to be faster
+            self.config_frozen = rtoml.load(self.freezer_file)
         except FileNotFoundError:
             warnings.warn("Freezer file not found.", stacklevel=2)
             self.config_frozen = {}
         # Setup self and do some checks
         assert self.config_user["version"] == 1
         self.kitchen = self.path / self.config_user["kitchen"]
         self.config_frozen.setdefault("meals", {})
@@ -148,21 +108,23 @@
 
     def _cache_spices(self):
         """Make sure all spices cache is updated."""
         for meal_value in self.config_user.get("meals", {}).values():
             for spice_url in meal_value.get("spices", []):
                 self._get_spice_content(spice_url)
 
-    def _get_meal_key_by_path(self, meal_path: Path, meal_menu: dict[str, Meal]) -> str:
-        """Find a meal in the menu that matches the given path."""
-        meal_abs = meal_path.absolute()
-        for key, meal in meal_menu.items():
-            if meal.path.absolute() == meal_abs:
-                return key
-        raise MrChefError(f"Couldn't find meal {meal_path}")
+    def _get_meal_key_by_path(self, meal_path: Path) -> str:
+        """Get the meal key by its path."""
+        meal_abs = meal_path.absolute().resolve()
+        kitchen_abs = self.kitchen.absolute().resolve()
+        if not meal_abs.is_relative_to(kitchen_abs):
+            raise MrChefError(
+                f"The meal {meal_path} is not inside the kitchen {self.kitchen}"
+            )
+        return str(meal_abs.relative_to(kitchen_abs))
 
     def _get_spice_content(self, spice_url: str, force_update=False) -> str:
         """Get spice content.
 
         Return the raw text of the patch.
 
         If the spice wasn't in the freezer, download it automatically and cache it.
@@ -272,25 +234,24 @@
                     "rev", self.config_frozen["meals"].get(key, {}).get("rev")
                 ),
                 spices=value.get("spices", []),
             )
             for key, value in self.config_user.get("meals", {}).items()
         }
 
-    def hot_meals(self) -> dict[str, Meal]:
+    def hot_meals(self, *meal_keys: str) -> dict[str, Meal]:
         """Get info from the hot meals found in the kitchen."""
         result = {}
         if not self.kitchen.is_dir():
             return result
         self._cache_spices()
         for meal_path in map(Path, find_repos(self.kitchen)):
-            meal_path = meal_path.resolve()
-            if not git_is_repo(meal_path):
+            key = self._get_meal_key_by_path(meal_path)
+            if meal_keys and key not in meal_keys:
                 continue
-            key = str(meal_path.relative_to(self.kitchen))
             branch = git_branch(meal_path)
             url = self.config_user.get(key, {}).get("url") or git_origin(meal_path)
             remote_head = git_remote_head(meal_path, url, branch)
             meal = Meal(
                 path=meal_path,
                 url=url,
                 branch=branch,
@@ -305,32 +266,34 @@
                     # Get patch URL from freezer
                     hot_spice_url = self.config_frozen["patch2spice"][hot_patch_id]
                 except KeyError:
                     # The patch is local; store it locally
                     local_path = self._new_patch()
                     local_contents = git_get_commit_patch(meal_path, hot_commit)
                     hot_spice_url = str(local_path.relative_to(self.path))
-                    local_path.write_text(local_contents)
                     # Cache patch contents in the freezer
                     self.config_frozen["spices"][hot_spice_url] = local_contents
                     self.config_frozen["patch2spice"][hot_patch_id] = hot_spice_url
                     # Store patch in user configuration
                     self.config_user["meals"][key].setdefault("spices", [])
                     self.config_user["meals"][key]["spices"].append(hot_spice_url)
                 # A spice can contain various commits, so it could exist already
                 if hot_spice_url not in meal.spices:
                     meal.spices.append(hot_spice_url)
             result[key] = meal
         return result
 
-    def all_meals(self) -> dict[str, dict[str, Optional[Meal]]]:
+    def all_meals(self, *meal_paths: Path) -> dict[str, dict[str, Optional[Meal]]]:
         """Obtain all meals, both warmed up and frozen.
 
         Useful to compare meals in both states.
 
+        Args:
+            meal_paths: Filter only meals related to these paths.
+
         Returns:
             Dict with all meals and their states.
 
             The dict key will be the meal name (relative path to kitchen root).
 
             The dict value will be another dict with keys "hot" and "cold".
             Each of those keys will contain `None` if the meal is not found in
@@ -347,16 +310,26 @@
                     "pizza/pepperoni": {
                         "hot": Meal(...),
                         "cold": Meal(...),
                     },
                 }
                 ```
         """
-        cold, hot = self.cold_meals(), self.hot_meals()
-        all_keys = sorted(set(cold) | set(hot))
+        cold = self.cold_meals()
+        meal_keys = {self._get_meal_key_by_path(meal_path) for meal_path in meal_paths}
+        invented_meals = meal_keys - set(cold)
+        if invented_meals:
+            raise MrChefError(
+                f"Couldn't find meal(s) in freezer: {', '.join(sorted(invented_meals))}"
+            )
+        hot = self.hot_meals(*meal_keys)
+        all_keys = set(cold) | set(hot)
+        if meal_paths:
+            all_keys &= set(meal_keys)
+        all_keys = sorted(all_keys)
         return {key: {"cold": cold.get(key), "hot": hot.get(key)} for key in all_keys}
 
     def update_user_config(self):
         """Update user config."""
         tomlkit.dump(self.config_user, self.config_file.open("w"))
 
     def check(self):
@@ -379,38 +352,30 @@
                     f"Meal {key} is frozen with rev {cold.rev}, but hot with rev {hot.rev}"
                 )
             if hot.spices != cold.spices:
                 errors.append(
                     f"Meal {key} spices are different. frozen={cold.spices} warm={hot.spices}"
                 )
         try:
-            if self.config_frozen != tomlkit.load(self.freezer_file.open()):
+            if self.config_frozen != rtoml.load(self.freezer_file):
                 errors.append("Freezer is outdated.")
         except FileNotFoundError:
             errors.append("Freezer not found.")
         if errors:
             raise MrChefError("🔪 Found errors:\n" + "\n".join(errors))
         logger.info("All frozen and hot meals are ready! 👨‍🍳")
 
     def warmup(self, *meal_paths: Path, force: bool = False):
         """Get meals out from freezer, warm them up in the kitchen.
 
         Args:
             *meal_paths: Meals to warm up. Skip to select all.
             force: Continue warming up meal if it is dirty.
         """
-        cold_meals = self.cold_meals()
-        meal_keys = {
-            self._get_meal_key_by_path(meal_path, cold_meals)
-            for meal_path in meal_paths
-        }
-        for key, value in self.all_meals().items():
-            # Skip unselected meals
-            if meal_paths and key not in meal_keys:
-                continue
+        for key, value in self.all_meals(*meal_paths).items():
             hot, cold = value["hot"], value["cold"]
             # Nothing to do if something is not in the freezer
             if not cold:
                 continue
             if hot == cold:
                 logger.info("Matches frozen status, skipping meal: %s", key)
                 continue
@@ -442,39 +407,46 @@
             logger.info(
                 "Updating %s: remote=%s branch=%s rev=%s",
                 key,
                 cold.url,
                 cold.branch,
                 cold.rev,
             )
-            remote_head = git_remote_head(cold.path, cold.url, cold.rev or cold.branch)
+            remote_head = git_remote_head(
+                cold.path, cold.url, cold.rev or cold.branch, not cold.rev
+            )
             _git("switch", "--force-create", cold.branch, cold.rev or remote_head)
             for spice in cold.spices:
                 logger.info("Applying spice to %s: %s", key, spice)
                 content = self._get_spice_content(spice)
                 self.spice_apply(cold.path, content)
+        # Some hot meals may have been modified
+        git_remote_head.cache_clear()
 
     def freeze(self):
         """Get meals from the kitchen and put them in the freezer."""
+        logger.info("Freezing...")
         new_freezer = {"version": 1, "meals": {}, "spices": {}, "patch2spice": {}}
         for name, meal in sorted(self.hot_meals().items()):
             assert meal.rev
             new_freezer["meals"][name] = {
                 "rev": meal.rev,
             }
-            for spice_url in meal.spices:
+            # Force cast to str for compatibility with rtoml.dump
+            for spice_url in map(str, meal.spices):
                 spice_content = self._get_spice_content(spice_url)
-                new_freezer["spices"][spice_url] = tomlkit.api.string(
-                    spice_content, multiline=True
-                )
+                new_freezer["spices"][spice_url] = spice_content
                 for patch_id in git_get_patch_ids_map(meal.path, spice_content):
                     new_freezer["patch2spice"][patch_id] = spice_url
+                local_patch = self.path / spice_url
+                if self._is_auto_patch(local_patch) and not local_patch.exists():
+                    local_patch.write_text(spice_content)
         with self.freezer_file.open("w") as fd:
             fd.write("# MrChef's freezer. MANUAL CHANGES WILL BE OVERRIDDEN.\n")
-            tomlkit.dump(new_freezer, fd)
+            rtoml.dump(new_freezer, fd, pretty=True)
         # Because maybe we detected hot patches in the mean time
         self.update_user_config()
 
     def meal_add(
         self, meal_path: Path, url: str, branch: str, rev: Optional[str] = None
     ):
         """Add a new meal to the kitchen and the freezer."""
@@ -492,73 +464,67 @@
             url,
             branch,
             rev,
         )
         self.config_user["meals"][key] = {"url": url, "branch": branch}
         if rev:
             self.config_user["meals"][key]["rev"] = rev
-        self.update_user_config()
         self.warmup(meal_path)
         self.freeze()
 
     def meal_rm(self, meal_path: Path):
         """Remove a meal from the kitchen."""
         meals = self.cold_meals()
-        key = self._get_meal_key_by_path(meal_path, meals)
+        key = self._get_meal_key_by_path(meal_path)
         del self.config_user["meals"][key]
         logger.info("Removing meal %s", key)
         with suppress(FileNotFoundError):
             rmtree(meals[key].path)
-        self.update_user_config()
         self.freeze()
 
     def spice_add(self, meal_path: Path, url: str, freeze: bool = True):
         """Download a patch and spice up meal with it."""
         if git_is_dirty(meal_path):
             raise MrChefError("Cannot add spice to dirty meal {meal_path}")
-        menu = self.hot_meals()
-        key = self._get_meal_key_by_path(meal_path, menu)
-        meal = menu[key]
+        key = self._get_meal_key_by_path(meal_path)
+        meal = self.hot_meals(key)[key]
         content = self._get_spice_content(url, True)
         if self.spice_is_applied(meal, content):
             raise MrChefError(f"Spice already exists: {url}")
         self.spice_apply(meal_path, content)
         self.config_user["meals"][key].setdefault("spices", [])
         self.config_user["meals"][key]["spices"].append(url)
-        self.update_user_config()
         self.freeze()
 
     def spice_rm(self, meal_path: Path, url: str):
         """Remove a patch from a meal.
 
         After successfully removing it, the meal will be re-warmed up and the
         config and freezer files will be updated.
 
         Args:
             meal_path: Where to find the meal.
             url: Spice URL to remove.
         """
         if git_is_dirty(meal_path):
             raise MrChefError("Cannot remove spice from dirty meal {meal_path}")
-        menu = self.hot_meals()
-        key = self._get_meal_key_by_path(meal_path, menu)
+        key = self._get_meal_key_by_path(meal_path)
         logger.info("Removing spice from %s: %s", key, url)
         try:
             self.config_user["meals"][key]["spices"].remove(url)
         except ValueError as error:
             raise MrChefError(
                 f"Cannot remove spice, not found in meal {key}: {url}"
             ) from error
         # If it was an autogenerated patch file, remove it
         patch_file = self.path / url
         if self._is_auto_patch(patch_file):
             patch_file.unlink(missing_ok=True)
         # Clean the kitchen
         self.warmup(meal_path)
-        self.update_user_config()
         self.freeze()
 
     def spice_export(self, url: str) -> str:
         """Export spice contents from the freezer.
 
         Args:
             url: The url that was frozen.
@@ -589,22 +555,20 @@
     def update(self, *meal_paths: Path, force: bool = False):
         """Update hot meals, store changes in the freezer.
 
         Args:
             *meal_paths: Meals to update. Skip to select all.
             force: Continue warming up meal if it is dirty.
         """
-        hot_meals = self.hot_meals()
-        meal_keys = {
-            self._get_meal_key_by_path(meal_path, hot_meals) for meal_path in meal_paths
-        }
-        for key in hot_meals:
-            # Skip unselected meals
-            if meal_paths and key not in meal_keys:
-                continue
+        meal_keys = (
+            {self._get_meal_key_by_path(meal_path) for meal_path in meal_paths}
+            if meal_paths
+            else list(self.config_frozen.get("meals", {}).keys())
+        )
+        for key in meal_keys:
             # Clear meal cache
             with suppress(KeyError):
                 del self.config_frozen["meals"][key]
             for spice in self.config_user["meals"].get(key, {}).get("spices", []):
                 with suppress(KeyError):
                     del self.config_frozen["spices"][spice]
         # Warm up again without cache
@@ -678,23 +642,14 @@
         patch_id: commit_id
         for patch_id, commit_id in (
             line.split() for line in patch_id_map().splitlines()
         )
     }
 
 
-def git_is_repo(folder: Path) -> bool:
-    """Know if the folder is a git repository."""
-    try:
-        git(folder)("status", "--porcelain")
-        return True
-    except ProcessExecutionError:
-        return False
-
-
 def git_is_dirty(folder: Path) -> bool:
     """Know if the folder is a dirty git repository."""
     return bool(git(folder)("status", "--porcelain"))
 
 
 def git_origin(folder: Path) -> str:
     """Know the git origin URL for Mr. Chef's default origin."""
@@ -713,27 +668,60 @@
         rev1: First commit to compare.
         rev2: Second commit to compare.
     """
     return git(folder)("merge-base", rev1, rev2).strip()
 
 
 @lru_cache
-def git_remote_head(folder: Path, remote_url: str, remote_ref: str) -> str:
+def git_remote_head(
+    folder: Path, remote_url: str, remote_ref: str, force_fetch: bool = False
+) -> str:
     """Get latest commit sha from remote url and ref combination.
 
     Args:
         folder: Path to git repo.
         remote_url: Absolute URL to remote.
-        remote_ref: Branch or revision to fetch from remote.
+        remote_ref: Branch or revision to query from remote.
+        force_fetch: Do not use a locally cached remote head.
     """
     _git = git(folder)
-    _git("fetch", "--write-fetch-head", remote_url, remote_ref)
+    remote_alias = git_remote_alias(folder, remote_url)
+    if not force_fetch and remote_alias:
+        try:
+            return _git(
+                "rev-parse", f"refs/remotes/{remote_alias}/{remote_ref}"
+            ).strip()
+        except ProcessExecutionError:
+            # Remote ref not found locally, fetch it
+            pass
+    # By attempting to fetch using the alias instead of the URL, we force Git
+    # to cache the result, so next calls with force_fetch=False will be faster
+    _git("fetch", "--write-fetch-head", remote_alias or remote_url, remote_ref)
     return _git("rev-parse", "FETCH_HEAD").strip()
 
 
+def git_remote_alias(folder: Path, remote_url: str) -> Optional[str]:
+    """Get local alias of a remote URL.
+
+    Args:
+        folder: Path to git repo.
+        remote_url: Absolute URL to remote.
+
+    Returns:
+        Local alias of the remote, or None if not found.
+    """
+    _git = git(folder)
+    # Output is like:
+    #   origin  https://gitlab.com/moduon/mrchef (fetch) [blob:none]
+    for remote in _git("remote", "-v").splitlines():
+        alias, url, mode = remote.split()[:3]
+        if url == remote_url and mode == "(fetch)":
+            return alias
+
+
 def git_rev(folder: Path) -> str:
     """Know the commit where a git repository is currently checked out."""
     return git(folder)("rev-parse", "--verify", "HEAD").strip()
 
 
 def git_root(folder: Path) -> Path:
     """Know the root of the git repository that owns a folder."""
```

