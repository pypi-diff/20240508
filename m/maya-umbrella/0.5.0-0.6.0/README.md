# Comparing `tmp/maya_umbrella-0.5.0.tar.gz` & `tmp/maya_umbrella-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maya_umbrella-0.5.0.tar", max compression
+gzip compressed data, was "maya_umbrella-0.6.0.tar", max compression
```

## Comparing `maya_umbrella-0.5.0.tar` & `maya_umbrella-0.6.0.tar`

### file list

```diff
@@ -1,21 +1,28 @@
--rw-r--r--   0        0        0     1060 2024-05-06 17:49:28.275867 maya_umbrella-0.5.0/LICENSE
--rw-r--r--   0        0        0     6202 2024-05-06 17:49:28.275867 maya_umbrella-0.5.0/README.md
--rw-r--r--   0        0        0      106 2024-05-06 17:49:28.299867 maya_umbrella-0.5.0/maya_umbrella/__init__.py
--rw-r--r--   0        0        0       22 2024-05-06 17:49:28.299867 maya_umbrella-0.5.0/maya_umbrella/__version__.py
--rw-r--r--   0        0        0      408 2024-05-06 17:49:28.299867 maya_umbrella-0.5.0/maya_umbrella/constants.py
--rw-r--r--   0        0        0     4223 2024-05-06 17:49:28.299867 maya_umbrella-0.5.0/maya_umbrella/core.py
--rw-r--r--   0        0        0     5293 2024-05-06 17:49:28.299867 maya_umbrella-0.5.0/maya_umbrella/filesystem.py
--rw-r--r--   0        0        0        0 2024-05-06 17:49:28.299867 maya_umbrella-0.5.0/maya_umbrella/hooks/__init__.py
--rw-r--r--   0        0        0      761 2024-05-06 17:49:28.299867 maya_umbrella-0.5.0/maya_umbrella/hooks/delete_turtle.py
--rw-r--r--   0        0        0     1281 2024-05-06 17:49:28.299867 maya_umbrella-0.5.0/maya_umbrella/hooks/delete_unknown_plugin_node.py
--rw-r--r--   0        0        0      556 2024-05-06 17:49:28.299867 maya_umbrella-0.5.0/maya_umbrella/hooks/fix_model_panel.py
--rw-r--r--   0        0        0      484 2024-05-06 17:49:28.299867 maya_umbrella-0.5.0/maya_umbrella/hooks/fix_on_model_change_3dc.py
--rw-r--r--   0        0        0     1338 2024-05-06 17:49:28.299867 maya_umbrella-0.5.0/maya_umbrella/log.py
--rw-r--r--   0        0        0      951 2024-05-06 17:49:28.299867 maya_umbrella-0.5.0/maya_umbrella/maya_funs.py
--rw-r--r--   0        0        0     8699 2024-05-06 17:49:28.299867 maya_umbrella-0.5.0/maya_umbrella/vaccine.py
--rw-r--r--   0        0        0        0 2024-05-06 17:49:28.299867 maya_umbrella-0.5.0/maya_umbrella/vaccines/__init__.py
--rw-r--r--   0        0        0      450 2024-05-06 17:49:28.299867 maya_umbrella-0.5.0/maya_umbrella/vaccines/vaccine1.py
--rw-r--r--   0        0        0     2151 2024-05-06 17:49:28.299867 maya_umbrella-0.5.0/maya_umbrella/vaccines/vaccine2.py
--rw-r--r--   0        0        0     2869 2024-05-06 17:49:28.299867 maya_umbrella-0.5.0/maya_umbrella/vaccines/vaccine3.py
--rw-r--r--   0        0        0     5202 2024-05-06 17:49:28.299867 maya_umbrella-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     7253 1970-01-01 00:00:00.000000 maya_umbrella-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1060 2024-05-08 16:17:57.631673 maya_umbrella-0.6.0/LICENSE
+-rw-r--r--   0        0        0     8127 2024-05-08 16:17:57.631673 maya_umbrella-0.6.0/README.md
+-rw-r--r--   0        0        0      401 2024-05-08 16:17:57.655673 maya_umbrella-0.6.0/maya_umbrella/__init__.py
+-rw-r--r--   0        0        0       22 2024-05-08 16:17:57.655673 maya_umbrella-0.6.0/maya_umbrella/__version__.py
+-rw-r--r--   0        0        0     5044 2024-05-08 16:17:57.655673 maya_umbrella-0.6.0/maya_umbrella/cleaner.py
+-rw-r--r--   0        0        0    13111 2024-05-08 16:17:57.655673 maya_umbrella-0.6.0/maya_umbrella/collector.py
+-rw-r--r--   0        0        0      539 2024-05-08 16:17:57.655673 maya_umbrella-0.6.0/maya_umbrella/constants.py
+-rw-r--r--   0        0        0     5601 2024-05-08 16:17:57.655673 maya_umbrella-0.6.0/maya_umbrella/defender.py
+-rw-r--r--   0        0        0     8333 2024-05-08 16:17:57.655673 maya_umbrella-0.6.0/maya_umbrella/filesystem.py
+-rw-r--r--   0        0        0        0 2024-05-08 16:17:57.655673 maya_umbrella-0.6.0/maya_umbrella/hooks/__init__.py
+-rw-r--r--   0        0        0      761 2024-05-08 16:17:57.655673 maya_umbrella-0.6.0/maya_umbrella/hooks/delete_turtle.py
+-rw-r--r--   0        0        0     1281 2024-05-08 16:17:57.655673 maya_umbrella-0.6.0/maya_umbrella/hooks/delete_unknown_plugin_node.py
+-rw-r--r--   0        0        0      556 2024-05-08 16:17:57.655673 maya_umbrella-0.6.0/maya_umbrella/hooks/fix_model_panel.py
+-rw-r--r--   0        0        0      484 2024-05-08 16:17:57.655673 maya_umbrella-0.6.0/maya_umbrella/hooks/fix_on_model_change_3dc.py
+-rw-r--r--   0        0        0     2683 2024-05-08 16:17:57.655673 maya_umbrella-0.6.0/maya_umbrella/i18n.py
+-rw-r--r--   0        0        0      962 2024-05-08 16:17:57.655673 maya_umbrella-0.6.0/maya_umbrella/locales/en_US.json
+-rw-r--r--   0        0        0     1006 2024-05-08 16:17:57.655673 maya_umbrella-0.6.0/maya_umbrella/locales/zh_CN.json
+-rw-r--r--   0        0        0     1338 2024-05-08 16:17:57.655673 maya_umbrella-0.6.0/maya_umbrella/log.py
+-rw-r--r--   0        0        0     3394 2024-05-08 16:17:57.655673 maya_umbrella-0.6.0/maya_umbrella/maya_funs.py
+-rw-r--r--   0        0        0     3710 2024-05-08 16:17:57.655673 maya_umbrella-0.6.0/maya_umbrella/scanner.py
+-rw-r--r--   0        0        0      354 2024-05-08 16:17:57.655673 maya_umbrella-0.6.0/maya_umbrella/signatures.py
+-rw-r--r--   0        0        0     1022 2024-05-08 16:17:57.655673 maya_umbrella-0.6.0/maya_umbrella/vaccine.py
+-rw-r--r--   0        0        0        0 2024-05-08 16:17:57.655673 maya_umbrella-0.6.0/maya_umbrella/vaccines/__init__.py
+-rw-r--r--   0        0        0      489 2024-05-08 16:17:57.655673 maya_umbrella-0.6.0/maya_umbrella/vaccines/vaccine1.py
+-rw-r--r--   0        0        0     2123 2024-05-08 16:17:57.655673 maya_umbrella-0.6.0/maya_umbrella/vaccines/vaccine2.py
+-rw-r--r--   0        0        0     3493 2024-05-08 16:17:57.655673 maya_umbrella-0.6.0/maya_umbrella/vaccines/vaccine3.py
+-rw-r--r--   0        0        0     5284 2024-05-08 16:17:57.655673 maya_umbrella-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     9178 1970-01-01 00:00:00.000000 maya_umbrella-0.6.0/PKG-INFO
```

### Comparing `maya_umbrella-0.5.0/LICENSE` & `maya_umbrella-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `maya_umbrella-0.5.0/maya_umbrella/hooks/delete_turtle.py` & `maya_umbrella-0.6.0/maya_umbrella/hooks/delete_turtle.py`

 * *Files identical despite different names*

### Comparing `maya_umbrella-0.5.0/maya_umbrella/hooks/delete_unknown_plugin_node.py` & `maya_umbrella-0.6.0/maya_umbrella/hooks/delete_unknown_plugin_node.py`

 * *Files identical despite different names*

### Comparing `maya_umbrella-0.5.0/maya_umbrella/hooks/fix_model_panel.py` & `maya_umbrella-0.6.0/maya_umbrella/hooks/fix_model_panel.py`

 * *Files identical despite different names*

### Comparing `maya_umbrella-0.5.0/maya_umbrella/log.py` & `maya_umbrella-0.6.0/maya_umbrella/log.py`

 * *Files identical despite different names*

### Comparing `maya_umbrella-0.5.0/maya_umbrella/vaccines/vaccine2.py` & `maya_umbrella-0.6.0/maya_umbrella/vaccines/vaccine2.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,50 +3,50 @@
 
 # Import local modules
 from maya_umbrella.constants import JOB_SCRIPTS_VIRUS_SIGNATURES
 from maya_umbrella.filesystem import check_virus_by_signature
 from maya_umbrella.filesystem import check_virus_file_by_signature
 from maya_umbrella.maya_funs import check_reference_node_exists
 from maya_umbrella.maya_funs import cmds
+from maya_umbrella.maya_funs import get_attr_value
 from maya_umbrella.vaccine import AbstractVaccine
 
 
 class Vaccine(AbstractVaccine):
     """A class for handling the ZeiJianKang virus."""
 
     virus_name = "zei jian kang"
 
-    def collect_bad_nodes(self):
+    def collect_infected_nodes(self):
         """Collect all bad nodes related to the virus."""
         for script_node in cmds.ls(type="script"):
             if check_reference_node_exists(script_node):
                 continue
-            script_before_string = cmds.getAttr("{}.before".format(script_node))
-            script_after_string = cmds.getAttr("{}.after".format(script_node))
-            for script_string in [script_before_string, script_after_string]:
+            for attr_name in ("before", "after"):
+                script_string = get_attr_value(script_node, attr_name)
                 if not script_string:
                     continue
                 if check_virus_by_signature(script_string, JOB_SCRIPTS_VIRUS_SIGNATURES):
                     self.report_issue(script_node)
-                    self.api.add_bad_node(script_node)
+                    self.api.add_infected_node(script_node)
 
     def collect_issues(self):
         """Collect all issues related to the virus."""
-        self.api.add_bad_files(
+        self.api.add_malicious_files(
             [
                 os.path.join(self.api.local_script_path, "vaccine.py"),
                 os.path.join(self.api.local_script_path, "vaccine.pyc"),
             ],
         )
-        self.collect_bad_usersetup_py()
-        self.collect_bad_nodes()
+        self.collect_infected_user_setup_py()
+        self.collect_infected_nodes()
 
-    def collect_bad_usersetup_py(self):
+    def collect_infected_user_setup_py(self):
         """Collect all bad userSetup.py files related to the virus."""
-        for usersetup_py in [
+        for user_setup_py in [
             os.path.join(self.api.local_script_path, "userSetup.py"),
             os.path.join(self.api.user_script_path, "userSetup.py"),
         ]:
-            if os.path.exists(usersetup_py):
-                if check_virus_file_by_signature(usersetup_py):
-                    self.report_issue(usersetup_py)
-                    self.api.add_infected_file(usersetup_py)
+            if os.path.exists(user_setup_py):
+                if check_virus_file_by_signature(user_setup_py):
+                    self.report_issue(user_setup_py)
+                    self.api.add_infected_file(user_setup_py)
```

### Comparing `maya_umbrella-0.5.0/pyproject.toml` & `maya_umbrella-0.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "maya_umbrella"
-version = "0.5.0"
+version = "0.6.0"
 description = "Check and fix maya virus."
 homepage = "https://github.com/loonghao/maya_umbrella"
 repository = "https://github.com/loonghao/maya_umbrella"
 documentation = "https://github.com/loonghao/maya_umbrella"
 keywords = ["notifiers", "python", "Maya", "dcc"]
 authors = ["longhao <hal.long@outlook.com>"]
 license = "MIT"
@@ -15,30 +15,32 @@
     "Programming Language :: Python :: 2.7",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
 ]
-
+include = [
+    { path = "maya_umbrella/locales", format = ["sdist", "wheel"] },
+]
 packages = [
     { include = "maya_umbrella" },
 ]
 [tool.poetry.build]
 generate-setup-file = false
 
 [tool.poetry.dependencies]
 python = ">=2.7,<2.8 || >=3.6.0"
 
 [tool.poetry.dev-dependencies]
 nox = { version = "^2024.3.2", python = ">=3.8.1,<3.11" }
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.5.0"
+version = "0.6.0"
 tag_format = "v$version"
 version_files = [
     "pyproject.toml:version",
     "maya_umbrella/__version__.py"
 ]
 
 [build-system]
```

### Comparing `maya_umbrella-0.5.0/PKG-INFO` & `maya_umbrella-0.6.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,32 +1,7 @@
-Metadata-Version: 2.1
-Name: maya_umbrella
-Version: 0.5.0
-Summary: Check and fix maya virus.
-Home-page: https://github.com/loonghao/maya_umbrella
-License: MIT
-Keywords: notifiers,python,Maya,dcc
-Author: longhao
-Author-email: hal.long@outlook.com
-Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Project-URL: Documentation, https://github.com/loonghao/maya_umbrella
-Project-URL: Repository, https://github.com/loonghao/maya_umbrella
-Description-Content-Type: text/markdown
-
 # maya-umbrella
 
 [![Python Version](https://img.shields.io/pypi/pyversions/maya-umbrella)](https://img.shields.io/pypi/pyversions/maya-umbrella)
 [![Nox](https://img.shields.io/badge/%F0%9F%A6%8A-Nox-D85E00.svg)](https://github.com/wntrblm/nox)
 [![PyPI Version](https://img.shields.io/pypi/v/maya-umbrella?color=green)](https://pypi.org/project/maya-umbrella/)
 [![Downloads](https://static.pepy.tech/badge/maya-umbrella)](https://pepy.tech/project/maya-umbrella)
 [![Downloads](https://static.pepy.tech/badge/maya-umbrella/month)](https://pepy.tech/project/maya-umbrella)
@@ -39,26 +14,40 @@
 [![maya-2022](https://img.shields.io/badge/maya-2022-green)](https://img.shields.io/badge/maya-2022-green)
 [![maya-2021](https://img.shields.io/badge/maya-2021-green)](https://img.shields.io/badge/maya-2021-green)
 [![maya-2020](https://img.shields.io/badge/maya-2020-green)](https://img.shields.io/badge/maya-2020-green)
 [![maya-2019](https://img.shields.io/badge/maya-2019-green)](https://img.shields.io/badge/maya-2019-green)
 [![maya-2018](https://img.shields.io/badge/maya-2018-green)](https://img.shields.io/badge/maya-2018-green)
 
 <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
-[![All Contributors](https://img.shields.io/badge/all_contributors-4-orange.svg?style=flat-square)](#contributors-)
+[![All Contributors](https://img.shields.io/badge/all_contributors-5-orange.svg?style=flat-square)](#contributors-)
 <!-- ALL-CONTRIBUTORS-BADGE:END -->
 
-This tool is designed to provide a robust solution for identifying and resolving any potential viruses within Autodesk Maya. 
+This tool is designed to provide a robust solution for identifying and resolving any potential viruses within Autodesk
+Maya.
 It ensures a secure and seamless user experience by proactively scanning for threats and effectively neutralizing them.
 
 It can be provided as an API for seamless integration into your existing pipeline.
 
+# 安装
+maya_umbrella是以标准pipy包去发布的，所以我们可以通过pip install去安装
+```shell
+your/maya-root/mayapy -m pip install maya-umbrella
+```
+更新版本
+```shell
+your/maya-root/mayapy -m pip install maya-umbrella --upgrade
+```
+卸载
+```shell
+your/maya-root/mayapy -m pip uninstall  maya-umbrella
+```
 
 # 开发环境设置
 
-Set up the development environment using a virtual environment, 
+Set up the development environment using a virtual environment,
 and it is recommended to use Python 3.8 or higher versions.
 
 通过虚拟环境去设置开发环境, 推荐python-3.8以上的版本
 
 ```shell
 pip install nox poetry
 ```
@@ -91,14 +80,22 @@
 
 我们可以利用封装好的`nox`命令去执行进行代码检查
 
 ```shell
 nox -s ruff_check
 ```
 
+# 生成安装包
+
+执行下面的命令可以在<repo>/.zip下面创建zip，参数 `--version` 当前工具的版本号
+
+```shell
+nox -s make-zip -- --version 0.5.0
+```
+
 # 环境变量
 
 我们可以通过下列环境变量去修改maya_umbrella的一些设置，方便有pipeline的公司可以更好的集成
 
 修改maya umbrella的日志保存目录，默认是windows temp目录
 
 ```shell
@@ -112,14 +109,53 @@
 ```
 
 设置日志级别，默认是info, 可以是debug可以看到更多的日志信息
 
 ```shell
 MAYA_UMBRELLA_LOG_LEVEL
 ```
+修改杀毒后文件的备份文件夹名称， 默认是`_virus`
+比如:
+你文件路径是  `c:/your/path/file.ma`
+那么备份文件路径是 `c:/your/path/_maya_umbrella/file.ma`
+```shell
+MAYA_UMBRELLA_BACKUP_FOLDER_NAME
+```
+默认的显示语言，包含日志打印输出等，默认是根据你当前maya的界面语言来设置的，当然我们也可以通过下面的环境变量去设置
+```shell
+MAYA_UMBRELLA_LANG
+```
+
+忽略保存到备份文件夹，*请注意，如果你不清楚这个会导致的后果请不要轻易修改*，默认批量杀毒后会把源文件自动备份到当前文件的备份文件夹.
+```shell
+MAYA_UMBRELLA_IGNORE_BACKUP
+```
+如果忽略请设置为
+```shell
+SET MAYA_UMBRELLA_IGNORE_BACKUP=true
+```
+
+# API
+获取当前场景没有被修复的病毒文件
+
+```python
+from maya_umbrella import MayaVirusDefender
+
+api = MayaVirusDefender()
+print(api.get_unfixed_references())
+```
+
+批量修复文件
+```python
+from maya_umbrella import MayaVirusScanner
+
+api = MayaVirusScanner()
+print(api.scan_files_from_pattern("your/path/*.m[ab]"))
+
+```
 
 ## Contributors ✨
 
 Thanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):
 
 <!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
 <!-- prettier-ignore-start -->
@@ -127,19 +163,19 @@
 <table>
   <tbody>
     <tr>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/loonghao"><img src="https://avatars1.githubusercontent.com/u/13111745?v=4?s=100" width="100px;" alt="Hal"/><br /><sub><b>Hal</b></sub></a><br /><a href="https://github.com/loonghao/maya_umbrella/commits?author=loonghao" title="Code">💻</a> <a href="#infra-loonghao" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a> <a href="https://github.com/loonghao/maya_umbrella/commits?author=loonghao" title="Tests">⚠️</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/hotwinter0"><img src="https://avatars.githubusercontent.com/u/106237305?v=4?s=100" width="100px;" alt="hotwinter0"/><br /><sub><b>hotwinter0</b></sub></a><br /><a href="https://github.com/loonghao/maya_umbrella/commits?author=hotwinter0" title="Tests">⚠️</a> <a href="https://github.com/loonghao/maya_umbrella/commits?author=hotwinter0" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/lingyunfx"><img src="https://avatars.githubusercontent.com/u/73666629?v=4?s=100" width="100px;" alt="lingyunfx"/><br /><sub><b>lingyunfx</b></sub></a><br /><a href="https://github.com/loonghao/maya_umbrella/commits?author=lingyunfx" title="Tests">⚠️</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/yjjjj"><img src="https://avatars.githubusercontent.com/u/12741735?v=4?s=100" width="100px;" alt="yjjjj"/><br /><sub><b>yjjjj</b></sub></a><br /><a href="https://github.com/loonghao/maya_umbrella/commits?author=yjjjj" title="Tests">⚠️</a> <a href="https://github.com/loonghao/maya_umbrella/commits?author=yjjjj" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/uncleschen"><img src="https://avatars.githubusercontent.com/u/37014389?v=4?s=100" width="100px;" alt="Unclechen"/><br /><sub><b>Unclechen</b></sub></a><br /><a href="https://github.com/loonghao/maya_umbrella/commits?author=uncleschen" title="Tests">⚠️</a></td>
     </tr>
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
 
 <!-- ALL-CONTRIBUTORS-LIST:END -->
 
 This project follows the [all-contributors](https://allcontributors.org) specification.
 Contributions of any kind are welcome!
-
```

