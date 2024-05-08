# Comparing `tmp/cjops-1.0.4.tar.gz` & `tmp/cjops-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cjops-1.0.4.tar", last modified: Wed May  8 03:15:09 2024, max compression
+gzip compressed data, was "cjops-1.0.5.tar", last modified: Wed May  8 06:11:43 2024, max compression
```

## Comparing `cjops-1.0.4.tar` & `cjops-1.0.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 caojie     (501) staff       (20)        0 2024-05-08 03:15:09.672115 cjops-1.0.4/
--rw-r--r--   0 caojie     (501) staff       (20)     1068 2024-03-15 01:36:01.000000 cjops-1.0.4/LICENSE
--rw-r--r--   0 caojie     (501) staff       (20)     2179 2024-05-08 03:15:09.671526 cjops-1.0.4/PKG-INFO
--rw-r--r--   0 caojie     (501) staff       (20)     1483 2024-04-25 10:03:23.000000 cjops-1.0.4/README.md
--rw-r--r--   0 caojie     (501) staff       (20)       38 2024-05-08 03:15:09.672238 cjops-1.0.4/setup.cfg
--rw-r--r--   0 caojie     (501) staff       (20)     2874 2024-05-07 08:48:04.000000 cjops-1.0.4/setup.py
-drwxr-xr-x   0 caojie     (501) staff       (20)        0 2024-05-08 03:15:09.656712 cjops-1.0.4/src/
-drwxr-xr-x   0 caojie     (501) staff       (20)        0 2024-05-08 03:15:09.666446 cjops-1.0.4/src/cjops/
--rw-r--r--   0 caojie     (501) staff       (20)      200 2024-05-08 00:48:52.000000 cjops-1.0.4/src/cjops/__init__.py
--rw-r--r--   0 caojie     (501) staff       (20)      333 2024-05-08 03:14:58.000000 cjops-1.0.4/src/cjops/__version__.py
--rw-r--r--   0 caojie     (501) staff       (20)     4608 2024-05-08 03:14:13.000000 cjops-1.0.4/src/cjops/aliyun.py
--rw-r--r--   0 caojie     (501) staff       (20)     2157 2024-04-15 06:29:32.000000 cjops-1.0.4/src/cjops/command.py
--rw-r--r--   0 caojie     (501) staff       (20)     4791 2024-05-07 07:49:15.000000 cjops-1.0.4/src/cjops/domain.py
--rw-r--r--   0 caojie     (501) staff       (20)     1795 2024-04-19 07:29:32.000000 cjops-1.0.4/src/cjops/email.py
--rw-r--r--   0 caojie     (501) staff       (20)     8459 2024-04-25 02:58:56.000000 cjops-1.0.4/src/cjops/excel.py
--rw-r--r--   0 caojie     (501) staff       (20)      127 2024-05-08 00:48:52.000000 cjops-1.0.4/src/cjops/info.py
--rw-r--r--   0 caojie     (501) staff       (20)      870 2024-04-12 07:35:23.000000 cjops-1.0.4/src/cjops/qw.py
--rw-r--r--   0 caojie     (501) staff       (20)     1411 2024-04-19 08:45:16.000000 cjops-1.0.4/src/cjops/sql.py
--rw-r--r--   0 caojie     (501) staff       (20)     2078 2024-05-07 09:24:16.000000 cjops-1.0.4/src/cjops/time.py
--rw-r--r--   0 caojie     (501) staff       (20)     6456 2024-05-07 07:55:52.000000 cjops-1.0.4/src/cjops/utils.py
-drwxr-xr-x   0 caojie     (501) staff       (20)        0 2024-05-08 03:15:09.670627 cjops-1.0.4/src/cjops.egg-info/
--rw-r--r--   0 caojie     (501) staff       (20)     2179 2024-05-08 03:15:09.000000 cjops-1.0.4/src/cjops.egg-info/PKG-INFO
--rw-r--r--   0 caojie     (501) staff       (20)      456 2024-05-08 03:15:09.000000 cjops-1.0.4/src/cjops.egg-info/SOURCES.txt
--rw-r--r--   0 caojie     (501) staff       (20)        1 2024-05-08 03:15:09.000000 cjops-1.0.4/src/cjops.egg-info/dependency_links.txt
--rw-r--r--   0 caojie     (501) staff       (20)        1 2024-05-07 08:48:08.000000 cjops-1.0.4/src/cjops.egg-info/not-zip-safe
--rw-r--r--   0 caojie     (501) staff       (20)      146 2024-05-08 03:15:09.000000 cjops-1.0.4/src/cjops.egg-info/requires.txt
--rw-r--r--   0 caojie     (501) staff       (20)        6 2024-05-08 03:15:09.000000 cjops-1.0.4/src/cjops.egg-info/top_level.txt
+drwxr-xr-x   0 caojie     (501) staff       (20)        0 2024-05-08 06:11:43.571551 cjops-1.0.5/
+-rw-r--r--   0 caojie     (501) staff       (20)     1068 2024-03-15 01:36:01.000000 cjops-1.0.5/LICENSE
+-rw-r--r--   0 caojie     (501) staff       (20)      383 2024-05-08 06:11:43.571152 cjops-1.0.5/PKG-INFO
+-rw-r--r--   0 caojie     (501) staff       (20)     1483 2024-04-25 10:03:23.000000 cjops-1.0.5/README.md
+-rw-r--r--   0 caojie     (501) staff       (20)       38 2024-05-08 06:11:43.571637 cjops-1.0.5/setup.cfg
+-rw-r--r--   0 caojie     (501) staff       (20)     3065 2024-05-08 06:11:18.000000 cjops-1.0.5/setup.py
+drwxr-xr-x   0 caojie     (501) staff       (20)        0 2024-05-08 06:11:43.559543 cjops-1.0.5/src/
+drwxr-xr-x   0 caojie     (501) staff       (20)        0 2024-05-08 06:11:43.568061 cjops-1.0.5/src/cjops/
+-rw-r--r--   0 caojie     (501) staff       (20)      200 2024-05-08 00:48:52.000000 cjops-1.0.5/src/cjops/__init__.py
+-rw-r--r--   0 caojie     (501) staff       (20)      333 2024-05-08 06:02:24.000000 cjops-1.0.5/src/cjops/__version__.py
+-rw-r--r--   0 caojie     (501) staff       (20)     4608 2024-05-08 03:14:13.000000 cjops-1.0.5/src/cjops/aliyun.py
+-rw-r--r--   0 caojie     (501) staff       (20)     2157 2024-04-15 06:29:32.000000 cjops-1.0.5/src/cjops/command.py
+-rw-r--r--   0 caojie     (501) staff       (20)     4791 2024-05-07 07:49:15.000000 cjops-1.0.5/src/cjops/domain.py
+-rw-r--r--   0 caojie     (501) staff       (20)     1795 2024-04-19 07:29:32.000000 cjops-1.0.5/src/cjops/email.py
+-rw-r--r--   0 caojie     (501) staff       (20)     8459 2024-04-25 02:58:56.000000 cjops-1.0.5/src/cjops/excel.py
+-rw-r--r--   0 caojie     (501) staff       (20)      127 2024-05-08 00:48:52.000000 cjops-1.0.5/src/cjops/info.py
+-rw-r--r--   0 caojie     (501) staff       (20)      870 2024-04-12 07:35:23.000000 cjops-1.0.5/src/cjops/qw.py
+-rw-r--r--   0 caojie     (501) staff       (20)     1411 2024-04-19 08:45:16.000000 cjops-1.0.5/src/cjops/sql.py
+-rw-r--r--   0 caojie     (501) staff       (20)     2078 2024-05-07 09:24:16.000000 cjops-1.0.5/src/cjops/time.py
+-rw-r--r--   0 caojie     (501) staff       (20)     6456 2024-05-07 07:55:52.000000 cjops-1.0.5/src/cjops/utils.py
+drwxr-xr-x   0 caojie     (501) staff       (20)        0 2024-05-08 06:11:43.570625 cjops-1.0.5/src/cjops.egg-info/
+-rw-r--r--   0 caojie     (501) staff       (20)      383 2024-05-08 06:11:43.000000 cjops-1.0.5/src/cjops.egg-info/PKG-INFO
+-rw-r--r--   0 caojie     (501) staff       (20)      456 2024-05-08 06:11:43.000000 cjops-1.0.5/src/cjops.egg-info/SOURCES.txt
+-rw-r--r--   0 caojie     (501) staff       (20)        1 2024-05-08 06:11:43.000000 cjops-1.0.5/src/cjops.egg-info/dependency_links.txt
+-rw-r--r--   0 caojie     (501) staff       (20)        1 2024-05-07 08:48:08.000000 cjops-1.0.5/src/cjops.egg-info/not-zip-safe
+-rw-r--r--   0 caojie     (501) staff       (20)       15 2024-05-08 06:11:43.000000 cjops-1.0.5/src/cjops.egg-info/requires.txt
+-rw-r--r--   0 caojie     (501) staff       (20)        6 2024-05-08 06:11:43.000000 cjops-1.0.5/src/cjops.egg-info/top_level.txt
```

### Comparing `cjops-1.0.4/LICENSE` & `cjops-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cjops-1.0.4/README.md` & `cjops-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `cjops-1.0.4/setup.py` & `cjops-1.0.5/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 import os, sys
 import setuptools
 from pathlib import Path
 
+package = 'cjops'
+if sys.argv[-1] in ['k8s', 'k9s','k8', 'k9']:
+    package = 'k9s'
+
 about = {}
 here = Path(__file__).absolute().parent
-with open(here /"src" / "cjops" / "__version__.py", "r", encoding="utf-8") as f:
+with open(here /"src" / f"{package}" / "__version__.py", "r", encoding="utf-8") as f:
     # exec() 函数用于执行从文件中读取的 Python 代码。具体来说，exec() 函数可以接受字符串形式的Python代码并执行,或者从文件中读取代码并执行。
     # 在你的例子中，通过打开文件 __version__.py 并读取其中的内容，然后使用 exec() 函数执行这些代码，将执行结果存储在 about 字典中。这种做法通常用于从外部文件中加载配置、定义变量或执行一些特定的操作。
     exec(f.read(), about)
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
-# 'setup.py publish' shortcut.
-if sys.argv[-1] == "publish":
-    os.system("rm -rf build cjops.egg-info dist")
+# 默认发布命令
+if sys.argv[-1] == "publish" or sys.argv[-2] == "publish":
+    os.system(f"rm -rf build {package}.egg-info dist")
     os.system("python setup.py sdist bdist_wheel")
     os.system("twine upload --skip-existing --repository-url https://upload.pypi.org/legacy/  dist/*")
-    os.system("pip uninstall cjops -y && pip install -U cjops -i https://pypi.org/simple")
+    os.system(f"pip uninstall {package} -y && pip install -U {package} -i https://pypi.org/simple")
     sys.exit()
 
-requires = [
+cjops_requires = [
         'aliyun-log-python-sdk>=0.8.15',
         'requests>=2.31.0',
         'loguru>=0.6.0',
         'dnspython',
         'pandas',
         'pendulum',
         'pymysql',
@@ -32,40 +36,45 @@
         'cryptography',
         'yagmail',
         'tqdm',
         'pyperclip',
         'emoji'
 ]
 
+k9s_requires = [
+    'loguru>=0.6.0'
+]
+
 setuptools.setup(
     # 包的分发名称，使用字母、数字、_、-
     name=about['__title__'],
      # 版本号, 版本号规范：https://www.python.org/dev/peps/pep-0440/
     version=about['__version__'],
     # 作者名
     author=about['__author__'],
      # 作者邮箱
     author_email=about['__author_email__'],
     # 包的简介描述
     description=about['__description__'],
     # 包的详细介绍(一般通过加载README.md)
-    long_description=long_description,
+    # long_description=long_description,
     # 和上条命令配合使用，声明加载的是markdown文件
     long_description_content_type="text/markdown",
     # 如果项目由多个文件组成，我们可以使用find_packages()自动发现所有包和子包，而不是手动列出每个包，在这种情况下，包列表将是example_pkg
     # packages=setuptools.find_packages(),
-    packages=["cjops"],  # 指定包名，确保只包含你需要的包
+    packages=[f"{package}"],  # 指定包名，确保只包含你需要的包
     package_dir={"": "src"},  # 指定包的根目录为src
     # 关于包的其他元数据(metadata)
     zip_safe=False,# 设置为False,提高安装效率和性能
     classifiers=[
          # 该软件包仅与Python3兼容
         "Programming Language :: Python :: 3",
         # 根据MIT许可证开源
         "License :: OSI Approved :: MIT License",
         # 与操作系统无关
         "Operating System :: OS Independent",
     ],
     # 依赖模块
-    install_requires= requires,
+    install_requires= f"{package}_requires",
     python_requires='>=3',
-)
+)
+
```

### Comparing `cjops-1.0.4/src/cjops/aliyun.py` & `cjops-1.0.5/src/cjops/aliyun.py`

 * *Files identical despite different names*

### Comparing `cjops-1.0.4/src/cjops/command.py` & `cjops-1.0.5/src/cjops/command.py`

 * *Files identical despite different names*

### Comparing `cjops-1.0.4/src/cjops/domain.py` & `cjops-1.0.5/src/cjops/domain.py`

 * *Files identical despite different names*

### Comparing `cjops-1.0.4/src/cjops/email.py` & `cjops-1.0.5/src/cjops/email.py`

 * *Files identical despite different names*

### Comparing `cjops-1.0.4/src/cjops/excel.py` & `cjops-1.0.5/src/cjops/excel.py`

 * *Files identical despite different names*

### Comparing `cjops-1.0.4/src/cjops/qw.py` & `cjops-1.0.5/src/cjops/qw.py`

 * *Files identical despite different names*

### Comparing `cjops-1.0.4/src/cjops/sql.py` & `cjops-1.0.5/src/cjops/sql.py`

 * *Files identical despite different names*

### Comparing `cjops-1.0.4/src/cjops/time.py` & `cjops-1.0.5/src/cjops/time.py`

 * *Files identical despite different names*

### Comparing `cjops-1.0.4/src/cjops/utils.py` & `cjops-1.0.5/src/cjops/utils.py`

 * *Files identical despite different names*

