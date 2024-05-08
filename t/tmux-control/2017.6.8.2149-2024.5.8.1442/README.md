# Comparing `tmp/tmux-control-2017.6.8.2149.tar.gz` & `tmp/tmux-control-2024.5.8.1442.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tmux-control-2017.6.8.2149.tar", last modified: Thu Jun  8 21:50:16 2017, max compression
+gzip compressed data, was "tmux-control-2024.5.8.1442.tar", last modified: Wed May  8 15:09:38 2024, max compression
```

## Comparing `tmux-control-2017.6.8.2149.tar` & `tmux-control-2024.5.8.1442.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 wbm       (1000) wbm       (1000)        0 2017-06-08 21:50:16.000000 tmux-control-2017.6.8.2149/
--rw-rw-r--   0 wbm       (1000) wbm       (1000)     5086 2017-06-08 21:50:16.000000 tmux-control-2017.6.8.2149/PKG-INFO
--rw-rw-r--   0 wbm       (1000) wbm       (1000)     3080 2017-06-08 21:42:22.000000 tmux-control-2017.6.8.2149/README.md
--rw-rw-r--   0 wbm       (1000) wbm       (1000)       75 2017-06-08 11:15:12.000000 tmux-control-2017.6.8.2149/MANIFEST.in
--rw-rw-r--   0 wbm       (1000) wbm       (1000)    35142 2017-06-08 11:15:12.000000 tmux-control-2017.6.8.2149/LICENSE
--rw-rw-r--   0 wbm       (1000) wbm       (1000)       38 2017-06-08 21:50:16.000000 tmux-control-2017.6.8.2149/setup.cfg
-drwxrwxr-x   0 wbm       (1000) wbm       (1000)        0 2017-06-08 21:50:16.000000 tmux-control-2017.6.8.2149/tmux_control.egg-info/
--rw-rw-r--   0 wbm       (1000) wbm       (1000)        1 2017-06-08 21:50:16.000000 tmux-control-2017.6.8.2149/tmux_control.egg-info/top_level.txt
--rw-rw-r--   0 wbm       (1000) wbm       (1000)       16 2017-06-08 21:50:16.000000 tmux-control-2017.6.8.2149/tmux_control.egg-info/requires.txt
--rw-rw-r--   0 wbm       (1000) wbm       (1000)     5086 2017-06-08 21:50:16.000000 tmux-control-2017.6.8.2149/tmux_control.egg-info/PKG-INFO
--rw-rw-r--   0 wbm       (1000) wbm       (1000)      233 2017-06-08 21:50:16.000000 tmux-control-2017.6.8.2149/tmux_control.egg-info/SOURCES.txt
--rw-rw-r--   0 wbm       (1000) wbm       (1000)        1 2017-06-08 21:50:16.000000 tmux-control-2017.6.8.2149/tmux_control.egg-info/dependency_links.txt
--rwxrwxr-x   0 wbm       (1000) wbm       (1000)    25578 2017-06-08 21:49:20.000000 tmux-control-2017.6.8.2149/tmux-control.py
--rw-rw-r--   0 wbm       (1000) wbm       (1000)     1171 2017-06-08 21:49:16.000000 tmux-control-2017.6.8.2149/setup.py
+drwxrwxr-x   0 wbm       (1000) wbm       (1000)        0 2024-05-08 15:09:38.269868 tmux-control-2024.5.8.1442/
+-rw-rw-r--   0 wbm       (1000) wbm       (1000)    35142 2024-05-08 11:50:07.000000 tmux-control-2024.5.8.1442/LICENSE
+-rw-rw-r--   0 wbm       (1000) wbm       (1000)       75 2024-05-08 11:50:07.000000 tmux-control-2024.5.8.1442/MANIFEST.in
+-rw-rw-r--   0 wbm       (1000) wbm       (1000)     4027 2024-05-08 15:09:38.269868 tmux-control-2024.5.8.1442/PKG-INFO
+-rw-rw-r--   0 wbm       (1000) wbm       (1000)     3437 2024-05-08 14:15:50.000000 tmux-control-2024.5.8.1442/README.md
+-rw-rw-r--   0 wbm       (1000) wbm       (1000)       38 2024-05-08 15:09:38.269868 tmux-control-2024.5.8.1442/setup.cfg
+-rw-rw-r--   0 wbm       (1000) wbm       (1000)     1118 2024-05-08 14:43:26.000000 tmux-control-2024.5.8.1442/setup.py
+-rwxrwxr-x   0 wbm       (1000) wbm       (1000)    16783 2024-05-08 14:42:15.000000 tmux-control-2024.5.8.1442/tmux-control.py
+drwxrwxr-x   0 wbm       (1000) wbm       (1000)        0 2024-05-08 15:09:38.269868 tmux-control-2024.5.8.1442/tmux_control.egg-info/
+-rw-rw-r--   0 wbm       (1000) wbm       (1000)     4027 2024-05-08 15:09:37.000000 tmux-control-2024.5.8.1442/tmux_control.egg-info/PKG-INFO
+-rw-rw-r--   0 wbm       (1000) wbm       (1000)      233 2024-05-08 15:09:38.000000 tmux-control-2024.5.8.1442/tmux_control.egg-info/SOURCES.txt
+-rw-rw-r--   0 wbm       (1000) wbm       (1000)        1 2024-05-08 15:09:37.000000 tmux-control-2024.5.8.1442/tmux_control.egg-info/dependency_links.txt
+-rw-rw-r--   0 wbm       (1000) wbm       (1000)        7 2024-05-08 15:09:38.000000 tmux-control-2024.5.8.1442/tmux_control.egg-info/requires.txt
+-rw-rw-r--   0 wbm       (1000) wbm       (1000)        1 2024-05-08 15:09:38.000000 tmux-control-2024.5.8.1442/tmux_control.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `tmux-control-2017.6.8.2149/PKG-INFO` & `tmux-control-2024.5.8.1442/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,177 +1,180 @@
-Metadata-Version: 1.0
+Metadata-Version: 2.1
 Name: tmux-control
-Version: 2017.6.8.2149
+Version: 2024.5.8.1442
 Summary: configure and control tmux
 Home-page: https://github.com/wdbm/tmux-control
 Author: Will Breaden Madden
 Author-email: wbm@protonmail.ch
 License: GPLv3
-Description: tmux-control
-        ============
-        
-        configure and control tmux
-        
-        setup
-        =====
-        
-        .. code:: bash
-        
-            sudo apt-get install cmus
-            sudo apt-get install elinks
-            sudo apt-get install htop
-            sudo apt-get install ranger
-            sudo apt-get install tmux
-        
-            sudo pip install tmux_control
-        
-        configurations
-        ==============
-        
-        analysis mode
-        -------------
-        
-        This mode is designed to be ergonomic for running an analysis. The
-        bottom terminal runs the main analysis code while ranger allows for
-        quick viewing of ongoing analysis output files.
-        
-        ::
-        
-            -----------------------
-            |                     |
-            |       ranger        |
-            |                     |
-            |                     |
-            |---------------------|
-            |                     |
-            |      terminal       |
-            |                     |
-            |                     |
-            -----------------------
-        
-        badass mode
-        -----------
-        
-        This mode is designed to be useful but also to show off the size of
-        one's metaphorical terminal configuration cock. It opens arXiv so you
-        can be a physics stunna, and cmus for acid dinner jazz.
-        
-        ::
-        
-            -----------------------
-            | ranger   |          |
-            |----------|          |
-            | terminal |          |
-            |----------|          |
-            | htop     |  ranger  |
-            |----------|          |
-            | arXiv    |          |
-            |----------|          |
-            | cmus     |          |
-            -----------------------
-        
-        detail mode
-        -----------
-        
-        This mode is designed to be a less fun version of badass mode.
-        
-        ::
-        
-            -----------------------
-            |          |          |
-            | ranger   |          |
-            |----------|          |
-            | terminal |          |
-            |----------|  ranger  |
-            | htop     |          |
-            |----------|          |
-            | arXiv    |          |
-            |          |          |
-            -----------------------
-        
-        edit mode (default)
-        -------------------
-        
-        This mode is designed to be ergonomic for coding.
-        
-        ::
-        
-            -----------------------
-            |          |          |
-            |          |          |
-            |          |          |
-            |          |          |
-            | terminal |  ranger  |
-            |          |          |
-            |          |          |
-            |          |          |
-            |          |          |
-            -----------------------
-        
-        Nvidia mode
-        -----------
-        
-        This mode is designed to display system resource usage for a system
-        featuring Nvidia hardware.
-        
-        ::
-        
-            -----------------------
-            |                     |
-            |        htop         |
-            |                     |
-            |                     |
-            |---------------------|
-            |                     |
-            |     nvidia-smi      |
-            |                     |
-            |                     |
-            -----------------------
-        
-        run mode
-        --------
-        
-        This mode launches all of the scripts at a specified directory in
-        separate windows.
-        
-        ::
-        
-            -----------------------
-            |                     |
-            |                     |
-            |                     |
-            |                     |
-            |      scripts        |
-            |                     |
-            |                     |
-            |                     |
-            |                     |
-            -----------------------
-        
-        work mode
-        ---------
-        
-        This mode is designed to be a compromise between analysis, edit and
-        badass modes.
-        
-        ::
-        
-            -----------------------
-            |                     |
-            |       ranger        |
-            |---------------------|
-            |                     |
-            |      terminal       |
-            |---------------------|
-            |          |          |
-            |  ranger  |  cmus    |
-            |          |          |
-            -----------------------
-        
-        usage
-        =====
-        
-        .. code:: bash
-        
-            tmux-control.py --help
-        
-Platform: UNKNOWN
+License-File: LICENSE
+
+tmux-control
+============
+
+configure and control tmux
+
+setup
+-----
+
+.. code:: bash
+
+   sudo apt-get install \
+       cmus             \
+       elinks           \
+       htop             \
+       nvtop            \
+       ranger           \
+       tmux
+
+   sudo pip install tmux_control
+
+configurations
+--------------
+
+analysis mode
+~~~~~~~~~~~~~
+
+This mode is designed to be ergonomic for running an analysis. The
+bottom terminal runs the main analysis code while ranger allows for
+quick viewing of ongoing analysis output files.
+
+::
+
+   -----------------------
+   |                     |
+   |       ranger        |
+   |                     |
+   |                     |
+   |---------------------|
+   |                     |
+   |      terminal       |
+   |                     |
+   |                     |
+   -----------------------
+
+badass mode
+~~~~~~~~~~~
+
+::
+
+   -----------------------
+   | ranger   |          |
+   |----------|          |
+   | terminal |          |
+   |----------|          |
+   | htop     |  ranger  |
+   |----------|          |
+   | arXiv    |          |
+   |----------|          |
+   | cmus     |          |
+   -----------------------
+
+detail mode
+~~~~~~~~~~~
+
+This mode is designed to be a less fun version of badass mode.
+
+::
+
+   -----------------------
+   |          |          |
+   | ranger   |          |
+   |----------|          |
+   | terminal |          |
+   |----------|  ranger  |
+   | htop     |          |
+   |----------|          |
+   | arXiv    |          |
+   |          |          |
+   -----------------------
+
+edit mode (default)
+~~~~~~~~~~~~~~~~~~~
+
+This mode is designed to be ergonomic for coding.
+
+::
+
+   -----------------------
+   |          |          |
+   |          |          |
+   |          |          |
+   |          |          |
+   | terminal |  ranger  |
+   |          |          |
+   |          |          |
+   |          |          |
+   |          |          |
+   -----------------------
+
+Nvidia mode
+~~~~~~~~~~~
+
+This mode is designed to display system resource usage for a system
+featuring Nvidia hardware.
+
+::
+
+   -----------------------
+   |                     |
+   |        htop         |
+   |                     |
+   |                     |
+   |---------------------|
+   |                     |
+   |        nvtop        |
+   |                     |
+   |                     |
+   -----------------------
+
+run mode
+~~~~~~~~
+
+This special mode launches all of the scripts at a defined directory in
+separate windows. It is used by engaging the option ``--run``,
+optionally together with the ``--directory`` option used to set the
+directory with a full or relative path (by default, the directory
+“scripts” at the working directory) and the ``--extension`` option used
+to define the extension of the scripts (by default, “sh”, and which can
+be set to “none” for any extensions).
+
+For example, the following command should run all files, regardless of
+extensions, at the directory ``/home/user/run_scripts``:
+
+.. code:: bash
+
+   tmux-control.py --run --directory=/home/user/run_scripts --extension=none
+
+::
+
+   -----------------------
+   |                     |
+   |                     |
+   |                     |
+   |                     |
+   |      scripts        |
+   |                     |
+   |                     |
+   |                     |
+   |                     |
+   -----------------------
+
+work mode
+~~~~~~~~~
+
+This mode is designed to be a compromise between analysis, edit and
+badass modes.
+
+::
+
+   -----------------------
+   |                     |
+   |       ranger        |
+   |---------------------|
+   |                     |
+   |      terminal       |
+   |---------------------|
+   |          |          |
+   |  ranger  |  cmus    |
+   |          |          |
+   -----------------------
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `tmux-control-2017.6.8.2149/LICENSE` & `tmux-control-2024.5.8.1442/LICENSE`

 * *Files identical despite different names*

### Comparing `tmux-control-2017.6.8.2149/tmux_control.egg-info/PKG-INFO` & `tmux-control-2024.5.8.1442/tmux_control.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,177 +1,180 @@
-Metadata-Version: 1.0
+Metadata-Version: 2.1
 Name: tmux-control
-Version: 2017.6.8.2149
+Version: 2024.5.8.1442
 Summary: configure and control tmux
 Home-page: https://github.com/wdbm/tmux-control
 Author: Will Breaden Madden
 Author-email: wbm@protonmail.ch
 License: GPLv3
-Description: tmux-control
-        ============
-        
-        configure and control tmux
-        
-        setup
-        =====
-        
-        .. code:: bash
-        
-            sudo apt-get install cmus
-            sudo apt-get install elinks
-            sudo apt-get install htop
-            sudo apt-get install ranger
-            sudo apt-get install tmux
-        
-            sudo pip install tmux_control
-        
-        configurations
-        ==============
-        
-        analysis mode
-        -------------
-        
-        This mode is designed to be ergonomic for running an analysis. The
-        bottom terminal runs the main analysis code while ranger allows for
-        quick viewing of ongoing analysis output files.
-        
-        ::
-        
-            -----------------------
-            |                     |
-            |       ranger        |
-            |                     |
-            |                     |
-            |---------------------|
-            |                     |
-            |      terminal       |
-            |                     |
-            |                     |
-            -----------------------
-        
-        badass mode
-        -----------
-        
-        This mode is designed to be useful but also to show off the size of
-        one's metaphorical terminal configuration cock. It opens arXiv so you
-        can be a physics stunna, and cmus for acid dinner jazz.
-        
-        ::
-        
-            -----------------------
-            | ranger   |          |
-            |----------|          |
-            | terminal |          |
-            |----------|          |
-            | htop     |  ranger  |
-            |----------|          |
-            | arXiv    |          |
-            |----------|          |
-            | cmus     |          |
-            -----------------------
-        
-        detail mode
-        -----------
-        
-        This mode is designed to be a less fun version of badass mode.
-        
-        ::
-        
-            -----------------------
-            |          |          |
-            | ranger   |          |
-            |----------|          |
-            | terminal |          |
-            |----------|  ranger  |
-            | htop     |          |
-            |----------|          |
-            | arXiv    |          |
-            |          |          |
-            -----------------------
-        
-        edit mode (default)
-        -------------------
-        
-        This mode is designed to be ergonomic for coding.
-        
-        ::
-        
-            -----------------------
-            |          |          |
-            |          |          |
-            |          |          |
-            |          |          |
-            | terminal |  ranger  |
-            |          |          |
-            |          |          |
-            |          |          |
-            |          |          |
-            -----------------------
-        
-        Nvidia mode
-        -----------
-        
-        This mode is designed to display system resource usage for a system
-        featuring Nvidia hardware.
-        
-        ::
-        
-            -----------------------
-            |                     |
-            |        htop         |
-            |                     |
-            |                     |
-            |---------------------|
-            |                     |
-            |     nvidia-smi      |
-            |                     |
-            |                     |
-            -----------------------
-        
-        run mode
-        --------
-        
-        This mode launches all of the scripts at a specified directory in
-        separate windows.
-        
-        ::
-        
-            -----------------------
-            |                     |
-            |                     |
-            |                     |
-            |                     |
-            |      scripts        |
-            |                     |
-            |                     |
-            |                     |
-            |                     |
-            -----------------------
-        
-        work mode
-        ---------
-        
-        This mode is designed to be a compromise between analysis, edit and
-        badass modes.
-        
-        ::
-        
-            -----------------------
-            |                     |
-            |       ranger        |
-            |---------------------|
-            |                     |
-            |      terminal       |
-            |---------------------|
-            |          |          |
-            |  ranger  |  cmus    |
-            |          |          |
-            -----------------------
-        
-        usage
-        =====
-        
-        .. code:: bash
-        
-            tmux-control.py --help
-        
-Platform: UNKNOWN
+License-File: LICENSE
+
+tmux-control
+============
+
+configure and control tmux
+
+setup
+-----
+
+.. code:: bash
+
+   sudo apt-get install \
+       cmus             \
+       elinks           \
+       htop             \
+       nvtop            \
+       ranger           \
+       tmux
+
+   sudo pip install tmux_control
+
+configurations
+--------------
+
+analysis mode
+~~~~~~~~~~~~~
+
+This mode is designed to be ergonomic for running an analysis. The
+bottom terminal runs the main analysis code while ranger allows for
+quick viewing of ongoing analysis output files.
+
+::
+
+   -----------------------
+   |                     |
+   |       ranger        |
+   |                     |
+   |                     |
+   |---------------------|
+   |                     |
+   |      terminal       |
+   |                     |
+   |                     |
+   -----------------------
+
+badass mode
+~~~~~~~~~~~
+
+::
+
+   -----------------------
+   | ranger   |          |
+   |----------|          |
+   | terminal |          |
+   |----------|          |
+   | htop     |  ranger  |
+   |----------|          |
+   | arXiv    |          |
+   |----------|          |
+   | cmus     |          |
+   -----------------------
+
+detail mode
+~~~~~~~~~~~
+
+This mode is designed to be a less fun version of badass mode.
+
+::
+
+   -----------------------
+   |          |          |
+   | ranger   |          |
+   |----------|          |
+   | terminal |          |
+   |----------|  ranger  |
+   | htop     |          |
+   |----------|          |
+   | arXiv    |          |
+   |          |          |
+   -----------------------
+
+edit mode (default)
+~~~~~~~~~~~~~~~~~~~
+
+This mode is designed to be ergonomic for coding.
+
+::
+
+   -----------------------
+   |          |          |
+   |          |          |
+   |          |          |
+   |          |          |
+   | terminal |  ranger  |
+   |          |          |
+   |          |          |
+   |          |          |
+   |          |          |
+   -----------------------
+
+Nvidia mode
+~~~~~~~~~~~
+
+This mode is designed to display system resource usage for a system
+featuring Nvidia hardware.
+
+::
+
+   -----------------------
+   |                     |
+   |        htop         |
+   |                     |
+   |                     |
+   |---------------------|
+   |                     |
+   |        nvtop        |
+   |                     |
+   |                     |
+   -----------------------
+
+run mode
+~~~~~~~~
+
+This special mode launches all of the scripts at a defined directory in
+separate windows. It is used by engaging the option ``--run``,
+optionally together with the ``--directory`` option used to set the
+directory with a full or relative path (by default, the directory
+“scripts” at the working directory) and the ``--extension`` option used
+to define the extension of the scripts (by default, “sh”, and which can
+be set to “none” for any extensions).
+
+For example, the following command should run all files, regardless of
+extensions, at the directory ``/home/user/run_scripts``:
+
+.. code:: bash
+
+   tmux-control.py --run --directory=/home/user/run_scripts --extension=none
+
+::
+
+   -----------------------
+   |                     |
+   |                     |
+   |                     |
+   |                     |
+   |      scripts        |
+   |                     |
+   |                     |
+   |                     |
+   |                     |
+   -----------------------
+
+work mode
+~~~~~~~~~
+
+This mode is designed to be a compromise between analysis, edit and
+badass modes.
+
+::
+
+   -----------------------
+   |                     |
+   |       ranger        |
+   |---------------------|
+   |                     |
+   |      terminal       |
+   |---------------------|
+   |          |          |
+   |  ranger  |  cmus    |
+   |          |          |
+   -----------------------
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `tmux-control-2017.6.8.2149/setup.py` & `tmux-control-2024.5.8.1442/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,37 +3,32 @@
 
 import os
 
 import setuptools
 import pypandoc
 
 def main():
-
     setuptools.setup(
         name             = "tmux-control",
-        version          = "2017.06.08.2149",
+        version          = "2024.05.08.1442",
         description      = "configure and control tmux",
         long_description = long_description(),
         url              = "https://github.com/wdbm/tmux-control",
         author           = "Will Breaden Madden",
         author_email     = "wbm@protonmail.ch",
         license          = "GPLv3",
         install_requires = [
-                           "propyte",
-                           "shijian"
+                           "docopt"
                            ],
         scripts          = [
                            "tmux-control.py"
                            ]
     )
 
-def long_description(
-    filename = "README.md"
-    ):
-
+def long_description(filename="README.md"):
     if os.path.isfile(os.path.expandvars(filename)):
         try:
             import pypandoc
             long_description = pypandoc.convert_file(filename, "rst")
         except ImportError:
             long_description = open(filename).read()
     else:
```

