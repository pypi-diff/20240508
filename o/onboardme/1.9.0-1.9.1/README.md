# Comparing `tmp/onboardme-1.9.0.tar.gz` & `tmp/onboardme-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onboardme-1.9.0.tar", max compression
+gzip compressed data, was "onboardme-1.9.1.tar", max compression
```

## Comparing `onboardme-1.9.0.tar` & `onboardme-1.9.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0    34523 2024-05-05 12:19:45.234342 onboardme-1.9.0/LICENSE.txt
--rw-r--r--   0        0        0    13512 2024-05-05 12:19:45.234342 onboardme-1.9.0/README.md
--rwxr-xr-x   0        0        0     7598 2024-05-05 12:19:45.258343 onboardme-1.9.0/onboardme/__init__.py
--rwxr-xr-x   0        0        0     3760 2024-05-05 12:19:45.258343 onboardme-1.9.0/onboardme/config/firewall/iptables.sh
--rw-r--r--   0        0        0       98 2024-05-05 12:19:45.258343 onboardme-1.9.0/onboardme/config/firewall/ufw/discord
--rw-r--r--   0        0        0     3093 2024-05-05 12:19:45.258343 onboardme-1.9.0/onboardme/console_logging.py
--rw-r--r--   0        0        0     2086 2024-05-05 12:19:45.258343 onboardme-1.9.0/onboardme/constants.py
--rw-r--r--   0        0        0     5641 2024-05-05 12:19:45.258343 onboardme-1.9.0/onboardme/dot_files.py
--rwxr-xr-x   0        0        0     6252 2024-05-05 12:19:45.258343 onboardme-1.9.0/onboardme/env_config.py
--rw-r--r--   0        0        0     2278 2024-05-05 12:19:45.258343 onboardme-1.9.0/onboardme/firewall.py
--rwxr-xr-x   0        0        0     6276 2024-05-05 12:19:45.258343 onboardme-1.9.0/onboardme/help_text.py
--rw-r--r--   0        0        0     3296 2024-05-05 12:19:45.258343 onboardme-1.9.0/onboardme/ide_setup.py
--rw-r--r--   0        0        0      760 2024-05-05 12:19:45.262343 onboardme-1.9.0/onboardme/misc.py
--rwxr-xr-x   0        0        0     9440 2024-05-05 12:19:45.262343 onboardme-1.9.0/onboardme/pkg_management.py
--rwxr-xr-x   0        0        0      233 2024-05-05 12:19:45.262343 onboardme-1.9.0/onboardme/scripts/update_apt_sources.sh
--rw-r--r--   0        0        0     3612 2024-05-05 12:19:45.262343 onboardme-1.9.0/onboardme/subproc.py
--rw-r--r--   0        0        0     1483 2024-05-05 12:19:45.262343 onboardme-1.9.0/onboardme/sudo_setup.py
--rw-r--r--   0        0        0     1803 2024-05-05 12:19:45.262343 onboardme-1.9.0/pyproject.toml
--rw-r--r--   0        0        0    14894 1970-01-01 00:00:00.000000 onboardme-1.9.0/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-05-08 14:47:34.887620 onboardme-1.9.1/LICENSE.txt
+-rw-r--r--   0        0        0    13512 2024-05-08 14:47:34.887620 onboardme-1.9.1/README.md
+-rwxr-xr-x   0        0        0     7652 2024-05-08 14:47:34.911620 onboardme-1.9.1/onboardme/__init__.py
+-rwxr-xr-x   0        0        0     3760 2024-05-08 14:47:34.911620 onboardme-1.9.1/onboardme/config/firewall/iptables.sh
+-rw-r--r--   0        0        0       98 2024-05-08 14:47:34.911620 onboardme-1.9.1/onboardme/config/firewall/ufw/discord
+-rw-r--r--   0        0        0     3093 2024-05-08 14:47:34.911620 onboardme-1.9.1/onboardme/console_logging.py
+-rw-r--r--   0        0        0     2086 2024-05-08 14:47:34.911620 onboardme-1.9.1/onboardme/constants.py
+-rw-r--r--   0        0        0     5641 2024-05-08 14:47:34.911620 onboardme-1.9.1/onboardme/dot_files.py
+-rwxr-xr-x   0        0        0     6252 2024-05-08 14:47:34.911620 onboardme-1.9.1/onboardme/env_config.py
+-rw-r--r--   0        0        0     2278 2024-05-08 14:47:34.911620 onboardme-1.9.1/onboardme/firewall.py
+-rwxr-xr-x   0        0        0     6276 2024-05-08 14:47:34.911620 onboardme-1.9.1/onboardme/help_text.py
+-rw-r--r--   0        0        0     3296 2024-05-08 14:47:34.911620 onboardme-1.9.1/onboardme/ide_setup.py
+-rw-r--r--   0        0        0      760 2024-05-08 14:47:34.911620 onboardme-1.9.1/onboardme/misc.py
+-rwxr-xr-x   0        0        0     9440 2024-05-08 14:47:34.911620 onboardme-1.9.1/onboardme/pkg_management.py
+-rwxr-xr-x   0        0        0      233 2024-05-08 14:47:34.911620 onboardme-1.9.1/onboardme/scripts/update_apt_sources.sh
+-rw-r--r--   0        0        0     3612 2024-05-08 14:47:34.911620 onboardme-1.9.1/onboardme/subproc.py
+-rw-r--r--   0        0        0     1483 2024-05-08 14:47:34.911620 onboardme-1.9.1/onboardme/sudo_setup.py
+-rw-r--r--   0        0        0     1803 2024-05-08 14:47:34.911620 onboardme-1.9.1/pyproject.toml
+-rw-r--r--   0        0        0    14894 1970-01-01 00:00:00.000000 onboardme-1.9.1/PKG-INFO
```

### Comparing `onboardme-1.9.0/LICENSE.txt` & `onboardme-1.9.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `onboardme-1.9.0/README.md` & `onboardme-1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `onboardme-1.9.0/onboardme/__init__.py` & `onboardme-1.9.1/onboardme/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -152,19 +152,25 @@
         help=HELP['no_upgrade'],
         default=False,
         is_flag=True)
 @option('--version',
         is_flag=True,
         help=HELP['version'],
         default=False)
-def main(log_level, log_file,
+def main(log_level,
+         log_file,
          steps,
-         git_url, git_branch, git_config_dir, overwrite,
-         pkg_managers, pkg_groups,
-         firewall, remote_host,
+         git_url,
+         git_branch,
+         git_config_dir,
+         overwrite,
+         pkg_managers,
+         pkg_groups,
+         firewall,
+         remote_host,
          no_upgrade,
          version) -> bool:
     """
     If run with no options on Linux, it will install brew, pip3.12, apt,
     flatpak, and snap packages. On mac, it only installs brew/pip3.12 packages.
     config loading tries to load: cli options and then defaults back to:
     $XDG_CONFIG_HOME/onboardme/config.yml
```

### Comparing `onboardme-1.9.0/onboardme/config/firewall/iptables.sh` & `onboardme-1.9.1/onboardme/config/firewall/iptables.sh`

 * *Files identical despite different names*

### Comparing `onboardme-1.9.0/onboardme/console_logging.py` & `onboardme-1.9.1/onboardme/console_logging.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.9.0/onboardme/constants.py` & `onboardme-1.9.1/onboardme/constants.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.9.0/onboardme/dot_files.py` & `onboardme-1.9.1/onboardme/dot_files.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.9.0/onboardme/env_config.py` & `onboardme-1.9.1/onboardme/env_config.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.9.0/onboardme/firewall.py` & `onboardme-1.9.1/onboardme/firewall.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.9.0/onboardme/help_text.py` & `onboardme-1.9.1/onboardme/help_text.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.9.0/onboardme/ide_setup.py` & `onboardme-1.9.1/onboardme/ide_setup.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.9.0/onboardme/misc.py` & `onboardme-1.9.1/onboardme/misc.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.9.0/onboardme/pkg_management.py` & `onboardme-1.9.1/onboardme/pkg_management.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.9.0/onboardme/subproc.py` & `onboardme-1.9.1/onboardme/subproc.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.9.0/onboardme/sudo_setup.py` & `onboardme-1.9.1/onboardme/sudo_setup.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.9.0/pyproject.toml` & `onboardme-1.9.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name          = "onboardme"
-version       = "1.9.0"
+version       = "1.9.1"
 description   = "Install dot files and packages, including a base mode with sensible defaults to run on most computers running Debian based distros or macOS."
 authors       = [
     "Jesse Hitch <jessebot@linux.com>",
     "Max Roby <emax@cloudydev.net>"
 ]
 license       = "AGPL-3.0-or-later"
 readme        = "README.md"
```

### Comparing `onboardme-1.9.0/PKG-INFO` & `onboardme-1.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onboardme
-Version: 1.9.0
+Version: 1.9.1
 Summary: Install dot files and packages, including a base mode with sensible defaults to run on most computers running Debian based distros or macOS.
 Home-page: http://github.com/jessebot/onboardme
 License: AGPL-3.0-or-later
 Keywords: onboardme,onboarding,desktop-setup,development-environment
 Author: Jesse Hitch
 Author-email: jessebot@linux.com
 Requires-Python: >=3.11,<3.13
```

