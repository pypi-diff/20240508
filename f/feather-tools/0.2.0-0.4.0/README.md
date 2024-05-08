# Comparing `tmp/feather_tools-0.2.0.tar.gz` & `tmp/feather_tools-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feather_tools-0.2.0.tar", last modified: Wed May  8 01:54:00 2024, max compression
+gzip compressed data, was "feather_tools-0.4.0.tar", last modified: Wed May  8 17:18:17 2024, max compression
```

## Comparing `feather_tools-0.2.0.tar` & `feather_tools-0.4.0.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 paepcke    (501) staff       (20)        0 2024-05-08 01:54:00.550997 feather_tools-0.2.0/
--rw-r--r--   0 paepcke    (501) staff       (20)     3706 2024-05-08 01:54:00.550336 feather_tools-0.2.0/PKG-INFO
--rw-r--r--   0 paepcke    (501) staff       (20)     3111 2024-05-08 01:53:42.000000 feather_tools-0.2.0/README.md
--rw-r--r--   0 paepcke    (501) staff       (20)      705 2024-05-08 01:50:37.000000 feather_tools-0.2.0/pyproject.toml
--rw-r--r--   0 paepcke    (501) staff       (20)       38 2024-05-08 01:54:00.551149 feather_tools-0.2.0/setup.cfg
-drwxr-xr-x   0 paepcke    (501) staff       (20)        0 2024-05-08 01:54:00.543442 feather_tools-0.2.0/src/
-drwxr-xr-x   0 paepcke    (501) staff       (20)        0 2024-05-08 01:54:00.544470 feather_tools-0.2.0/src/feather/
--rw-r--r--   0 paepcke    (501) staff       (20)        0 2024-05-01 19:27:54.000000 feather_tools-0.2.0/src/feather/__init__.py
--rw-r--r-x   0 paepcke    (501) staff       (20)    20998 2024-05-07 17:42:50.000000 feather_tools-0.2.0/src/feather/ftools_workhorse.py
-drwxr-xr-x   0 paepcke    (501) staff       (20)        0 2024-05-08 01:54:00.547031 feather_tools-0.2.0/src/feather/test/
--rw-r--r--   0 paepcke    (501) staff       (20)        0 2024-05-01 20:55:38.000000 feather_tools-0.2.0/src/feather/test/__init__.py
--rwxr-xr--   0 paepcke    (501) staff       (20)     6441 2024-05-08 01:17:15.000000 feather_tools-0.2.0/src/feather/test/f2csv_copy.py
--rwxr-xr--   0 paepcke    (501) staff       (20)     2721 2024-05-08 00:35:07.000000 feather_tools-0.2.0/src/feather/test/fmore_copy.py
--rwxr-xr--   0 paepcke    (501) staff       (20)     2913 2024-05-08 00:35:20.000000 feather_tools-0.2.0/src/feather/test/ftail_copy.py
--rwxr-xr--   0 paepcke    (501) staff       (20)     2224 2024-05-08 00:35:30.000000 feather_tools-0.2.0/src/feather/test/fwc_copy.py
--rw-r--r--   0 paepcke    (501) staff       (20)    27512 2024-05-08 01:35:54.000000 feather_tools-0.2.0/src/feather/test/test_ftools_workhorse.py
-drwxr-xr-x   0 paepcke    (501) staff       (20)        0 2024-05-08 01:54:00.549789 feather_tools-0.2.0/src/feather_tools.egg-info/
--rw-r--r--   0 paepcke    (501) staff       (20)     3706 2024-05-08 01:54:00.000000 feather_tools-0.2.0/src/feather_tools.egg-info/PKG-INFO
--rw-r--r--   0 paepcke    (501) staff       (20)      477 2024-05-08 01:54:00.000000 feather_tools-0.2.0/src/feather_tools.egg-info/SOURCES.txt
--rw-r--r--   0 paepcke    (501) staff       (20)        1 2024-05-08 01:54:00.000000 feather_tools-0.2.0/src/feather_tools.egg-info/dependency_links.txt
--rw-r--r--   0 paepcke    (501) staff       (20)       30 2024-05-08 01:54:00.000000 feather_tools-0.2.0/src/feather_tools.egg-info/requires.txt
--rw-r--r--   0 paepcke    (501) staff       (20)        8 2024-05-08 01:54:00.000000 feather_tools-0.2.0/src/feather_tools.egg-info/top_level.txt
+drwxr-xr-x   0 paepcke    (501) staff       (20)        0 2024-05-08 17:18:17.655425 feather_tools-0.4.0/
+-rw-r--r--   0 paepcke    (501) staff       (20)      256 2024-05-08 17:15:59.000000 feather_tools-0.4.0/MANIFEST.in
+-rw-r--r--   0 paepcke    (501) staff       (20)     3610 2024-05-08 17:18:17.654557 feather_tools-0.4.0/PKG-INFO
+-rw-r--r--   0 paepcke    (501) staff       (20)     3081 2024-05-08 17:15:59.000000 feather_tools-0.4.0/README.md
+-rw-r--r--   0 paepcke    (501) staff       (20)      678 2024-05-08 17:18:03.000000 feather_tools-0.4.0/pyproject.toml
+-rw-r--r--   0 paepcke    (501) staff       (20)       38 2024-05-08 17:18:17.655558 feather_tools-0.4.0/setup.cfg
+drwxr-xr-x   0 paepcke    (501) staff       (20)        0 2024-05-08 17:18:17.646769 feather_tools-0.4.0/src/
+drwxr-xr-x   0 paepcke    (501) staff       (20)        0 2024-05-08 17:18:17.648573 feather_tools-0.4.0/src/feather_tools/
+-rw-r--r--   0 paepcke    (501) staff       (20)        0 2024-05-08 17:15:59.000000 feather_tools-0.4.0/src/feather_tools/__init__.py
+-rw-r--r--   0 paepcke    (501) staff       (20)    21004 2024-05-08 17:15:59.000000 feather_tools-0.4.0/src/feather_tools/ftools_workhorse.py
+drwxr-xr-x   0 paepcke    (501) staff       (20)        0 2024-05-08 17:18:17.653227 feather_tools-0.4.0/src/feather_tools/test/
+-rw-r--r--   0 paepcke    (501) staff       (20)        0 2024-05-08 17:15:59.000000 feather_tools-0.4.0/src/feather_tools/test/__init__.py
+-rwxr-xr-x   0 paepcke    (501) staff       (20)     6164 2024-05-08 17:15:59.000000 feather_tools-0.4.0/src/feather_tools/test/f2csv_copy.py
+-rwxr-xr-x   0 paepcke    (501) staff       (20)     2727 2024-05-08 17:15:59.000000 feather_tools-0.4.0/src/feather_tools/test/fless_copy.py
+-rwxr-xr-x   0 paepcke    (501) staff       (20)     2941 2024-05-08 17:15:59.000000 feather_tools-0.4.0/src/feather_tools/test/ftail_copy.py
+-rwxr-xr-x   0 paepcke    (501) staff       (20)     2230 2024-05-08 17:15:59.000000 feather_tools-0.4.0/src/feather_tools/test/fwc_copy.py
+-rw-r--r--   0 paepcke    (501) staff       (20)    27584 2024-05-08 17:15:59.000000 feather_tools-0.4.0/src/feather_tools/test/test_ftools_workhorse.py
+drwxr-xr-x   0 paepcke    (501) staff       (20)        0 2024-05-08 17:18:17.653917 feather_tools-0.4.0/src/feather_tools.egg-info/
+-rw-r--r--   0 paepcke    (501) staff       (20)     3610 2024-05-08 17:18:17.000000 feather_tools-0.4.0/src/feather_tools.egg-info/PKG-INFO
+-rw-r--r--   0 paepcke    (501) staff       (20)      537 2024-05-08 17:18:17.000000 feather_tools-0.4.0/src/feather_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 paepcke    (501) staff       (20)        1 2024-05-08 17:18:17.000000 feather_tools-0.4.0/src/feather_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 paepcke    (501) staff       (20)       30 2024-05-08 17:18:17.000000 feather_tools-0.4.0/src/feather_tools.egg-info/requires.txt
+-rw-r--r--   0 paepcke    (501) staff       (20)       14 2024-05-08 17:18:17.000000 feather_tools-0.4.0/src/feather_tools.egg-info/top_level.txt
```

### Comparing `feather_tools-0.2.0/PKG-INFO` & `feather_tools-0.4.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,50 +1,46 @@
 Metadata-Version: 2.1
 Name: feather_tools
-Version: 0.2.0
+Version: 0.4.0
 Summary: Scripts to use for pyarrow feather files in a Linux terminal window
 Author-email: Andreas Paepcke <paepcke@cs.stanford.edu>
 Maintainer-email: Andreas Paepcke <paepcke@cs.stanford.edu>
 License: MIT License
-Project-URL: Homepage, https://github.com/paepcke/feather_tools
-Project-URL: Documentation, https://github.com/paepcke/feather_tools
-Project-URL: Repository, https://github.com/paepcke/feather_tools
+Project-URL: Homepage, https://github.com/paepcke/feather-tools
+Project-URL: Documentation, https://github.com/paepcke/feather-tools
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Requires-Dist: pandas>=2.2.2
 Requires-Dist: pyarrow>=16.0.0
 
 ## Description
 Stand-alone Unix shell command line tools for Apache's .feather formatted files:
 
 ```
-- fmore
+- fless
 - ftail
 - fwc (-l)
 - f2csv
 ```
 
-Each tool operates in the spirit of the analogous Unix shell command. Only the most basic uses of these original Unix tools are suported in their *f* version. For example, the `fwc` command operates like `wc -l`, i.e. it displays the number of datalines. But `wc -c` is not provided.
+Each tool operates in the spirit of the analogous Unix shell command. Only the most basic uses of these original Unix tools are suported in their *f* version. For example, the `fwc` command operates like `wc -l`, i.e. it displays the number of data rows. But `wc -c` is not provided.
 
 ## Installation:
 ```
 - Create virtual environment if desired
 - pip install feather-tools
 - pip install .
 ```
-
-For convenience, you might either include the location of the files in $PATH, or symlink the above files to where they are accessible from different directories. For example, `/usr/local/bin`.
+The files will be in .../site-packages/feather_tools. For convenience, you might add that location to $PATH.
 
 ## Usage:
 
-All Python imports are relative to `<proj-root>/src`. So ensure that your $PYTHONPATH includes that directory.
-
-### `fmore`
+### `fless`
 ```
-fmore <fpath>
+fless <fpath>
 ```
 Shows one screenful of the .feather file at a time. The number of rows displayed is determined by the terminal in which the command is issued. At the end of each displayed page, type a single character:
 
 - To show the next page: `spacebar`, or `\n`, or the character *n*
 - Back one page: *b*
 - Back to beginning (page 0): *s*
 - To the last page: *e*
@@ -55,25 +51,25 @@
 Displays the last *n* rows of the .feather file. Default is the lesser of 10, and the length of the data.
 
 **NOTE**: Starts the row display with the logical (i.e. terminal-height) page that contains the first line specified by the tail default or in the `--lines` argument. So a few more rows than requested may be displayed at the top.
 
 ### `fwc <fpath>`
 Is analogout to the Unix `wc -l`, and shows the number of data rows, not counting the column header.
 
-### `f2csv <src-fpath> <dst-fpath> `
+### `f2csv <src-fpath> [<dst-fpath>] `
 Writes a .csv file that contains the .feather data. Default separator is comma. Default output is stdout.
 
 The command line arguments are as in the [Pandas `df.to_csv()`](https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.to_csv.html) documentation. This means that the `index` keyword is True by default, while `index_label` is None. Which leads to ugly .csv like:
 ```
 ,foo,bar,fum
 Row0,1,2,3
 Row1,4,5,6
 Row2,7,8,9
 ```
-Where the `Row*n*` are the dataframe index. Note the orphan comma. To fix (same as with df.to_csv()):
+Where the `Row`*n* are the dataframe index. Note the orphan comma in the header. To fix (same as with df.to_csv()):
 ```
 f2csv --index=true --index_label=Rows file.feather
 
 Rows,foo,bar,fum
 Row0,1,2,3
 Row1,4,5,6
 Row2,7,8,9
@@ -83,10 +79,11 @@
 f2csv --index=false file.feather
 
 foo,bar,fum
 1,2,3
 4,5,6
 7,8,9
 ```
+If you clone this repo to make changes: all Python imports are relative to `<proj-root>/src`. So ensure that your $PYTHONPATH includes that directory.
 
 ## Testing
-Running nose2 in the project root runs the tests. One abnormality: in order to blend with Unix convention, the command files are without a '.py' extension. Examples: `fmore`, `fwc`. The downside is that unittest files cannot load Python files without .py extensions. Copies of the command files are therefore placed in the test subdirectory. The unittests run on those copies. If changes are made to the command files, then those copies must be updated before testing. Symlinks are not an option, because pip cannot recreate them during installation.
+Running nose2 in the project root runs the tests. One abnormality: in order to blend with Unix convention, the command files are without a '.py' extension. Examples: `fless`, `fwc`. The downside is that unittest files cannot load Python files without .py extensions. Copies of the command files are therefore placed in the test subdirectory. The unittests run on those copies. If changes are made to the command files, then those copies must be updated before testing. Symlinks are not an option, because pip cannot recreate them during installation.
```

### Comparing `feather_tools-0.2.0/README.md` & `feather_tools-0.4.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,35 +1,32 @@
 ## Description
 Stand-alone Unix shell command line tools for Apache's .feather formatted files:
 
 ```
-- fmore
+- fless
 - ftail
 - fwc (-l)
 - f2csv
 ```
 
-Each tool operates in the spirit of the analogous Unix shell command. Only the most basic uses of these original Unix tools are suported in their *f* version. For example, the `fwc` command operates like `wc -l`, i.e. it displays the number of datalines. But `wc -c` is not provided.
+Each tool operates in the spirit of the analogous Unix shell command. Only the most basic uses of these original Unix tools are suported in their *f* version. For example, the `fwc` command operates like `wc -l`, i.e. it displays the number of data rows. But `wc -c` is not provided.
 
 ## Installation:
 ```
 - Create virtual environment if desired
 - pip install feather-tools
 - pip install .
 ```
-
-For convenience, you might either include the location of the files in $PATH, or symlink the above files to where they are accessible from different directories. For example, `/usr/local/bin`.
+The files will be in .../site-packages/feather_tools. For convenience, you might add that location to $PATH.
 
 ## Usage:
 
-All Python imports are relative to `<proj-root>/src`. So ensure that your $PYTHONPATH includes that directory.
-
-### `fmore`
+### `fless`
 ```
-fmore <fpath>
+fless <fpath>
 ```
 Shows one screenful of the .feather file at a time. The number of rows displayed is determined by the terminal in which the command is issued. At the end of each displayed page, type a single character:
 
 - To show the next page: `spacebar`, or `\n`, or the character *n*
 - Back one page: *b*
 - Back to beginning (page 0): *s*
 - To the last page: *e*
@@ -40,25 +37,25 @@
 Displays the last *n* rows of the .feather file. Default is the lesser of 10, and the length of the data.
 
 **NOTE**: Starts the row display with the logical (i.e. terminal-height) page that contains the first line specified by the tail default or in the `--lines` argument. So a few more rows than requested may be displayed at the top.
 
 ### `fwc <fpath>`
 Is analogout to the Unix `wc -l`, and shows the number of data rows, not counting the column header.
 
-### `f2csv <src-fpath> <dst-fpath> `
+### `f2csv <src-fpath> [<dst-fpath>] `
 Writes a .csv file that contains the .feather data. Default separator is comma. Default output is stdout.
 
 The command line arguments are as in the [Pandas `df.to_csv()`](https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.to_csv.html) documentation. This means that the `index` keyword is True by default, while `index_label` is None. Which leads to ugly .csv like:
 ```
 ,foo,bar,fum
 Row0,1,2,3
 Row1,4,5,6
 Row2,7,8,9
 ```
-Where the `Row*n*` are the dataframe index. Note the orphan comma. To fix (same as with df.to_csv()):
+Where the `Row`*n* are the dataframe index. Note the orphan comma in the header. To fix (same as with df.to_csv()):
 ```
 f2csv --index=true --index_label=Rows file.feather
 
 Rows,foo,bar,fum
 Row0,1,2,3
 Row1,4,5,6
 Row2,7,8,9
@@ -68,10 +65,11 @@
 f2csv --index=false file.feather
 
 foo,bar,fum
 1,2,3
 4,5,6
 7,8,9
 ```
+If you clone this repo to make changes: all Python imports are relative to `<proj-root>/src`. So ensure that your $PYTHONPATH includes that directory.
 
 ## Testing
-Running nose2 in the project root runs the tests. One abnormality: in order to blend with Unix convention, the command files are without a '.py' extension. Examples: `fmore`, `fwc`. The downside is that unittest files cannot load Python files without .py extensions. Copies of the command files are therefore placed in the test subdirectory. The unittests run on those copies. If changes are made to the command files, then those copies must be updated before testing. Symlinks are not an option, because pip cannot recreate them during installation.
+Running nose2 in the project root runs the tests. One abnormality: in order to blend with Unix convention, the command files are without a '.py' extension. Examples: `fless`, `fwc`. The downside is that unittest files cannot load Python files without .py extensions. Copies of the command files are therefore placed in the test subdirectory. The unittests run on those copies. If changes are made to the command files, then those copies must be updated before testing. Symlinks are not an option, because pip cannot recreate them during installation.
```

### Comparing `feather_tools-0.2.0/pyproject.toml` & `feather_tools-0.4.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 [build-system]
 
-requires = ["setuptools >= 64", "cython", "wheel"]
+requires = ["setuptools >= 64", "wheel"]
+build-backend = "setuptools.build_meta"
 
 [project]
 
 name = "feather_tools"
 description = "Scripts to use for pyarrow feather files in a Linux terminal window"
-version = "0.2.0"
+version = "0.4.0"
 readme  = "README.md"
 authors = [
   {name = "Andreas Paepcke", email = "paepcke@cs.stanford.edu"}
   ]
 maintainers = [
   {name = "Andreas Paepcke", email = "paepcke@cs.stanford.edu"}
   ]
@@ -19,12 +20,10 @@
 dependencies = [
     "pandas>=2.2.2",
     "pyarrow>=16.0.0"
     ]
 requires-python = ">= 3.11"
 
 [project.urls]
-
-Homepage = "https://github.com/paepcke/feather_tools"
-Documentation = "https://github.com/paepcke/feather_tools"
-Repository = "https://github.com/paepcke/feather_tools"
+Homepage = "https://github.com/paepcke/feather-tools"
+Documentation = "https://github.com/paepcke/feather-tools"
```

### Comparing `feather_tools-0.2.0/src/feather/ftools_workhorse.py` & `feather_tools-0.4.0/src/feather_tools/ftools_workhorse.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     classdocs
     '''
 
     def __init__(self, path, lines=None, cols=None, out_stream=sys.stdout, unittesting=False):
         '''
         
         
-        :param path: location of dataframe .feather file. Maybe
+        :param path: location of dataframe .feather_tools file. Maybe
             absolute, or relative to current directory
         :type path: str
         :param lines: number of lines per page. If None, 
             use terminal height
         :type lines: union[None | int]
         :param cols: number character columns for each line.
             If None, use terminal width
```

### Comparing `feather_tools-0.2.0/src/feather/test/f2csv_copy.py` & `feather_tools-0.4.0/src/feather_tools/test/f2csv_copy.py`

 * *Files 19% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 '''
 
 import argparse
 import os
 import sys
 
-from feather.ftools_workhorse import FToolsWorkhorse
+from feather_tools.ftools_workhorse import FToolsWorkhorse
 from numpy.lib._iotools import str2bool
 
 #------------------------------------
 # main 
 #-------------------
 
 def main(**kwargs):
@@ -49,21 +49,15 @@
 
     out_stream = kwargs['path_or_buf']
     if out_stream is None:
         out_stream = sys.stdout 
         kwargs['path_or_buf'] = sys.stdout
         
     workhorse = FToolsWorkhorse(src_file, out_stream=out_stream)
-    # If the index is to be included in the .csv,
-    # and no column name is given for that column,
-    # add one:
-    
-    # if kwargs['index']:
-    #     if kwargs['index_label'] is None:
-    #         kwargs['index_label'] = 'Row Label'
+    
     workhorse.df.to_csv(**kwargs)
 
 #------------------------------------
 # str2bool
 #-------------------
 
 def str2bool(bool_str):
@@ -99,17 +93,19 @@
     parser.add_argument('--float_format',
                         default=None,
                         help='format string for floating point numbers')
     parser.add_argument('--columns',
                         default=None,
                         help='columns to include')
     parser.add_argument('--header',
+                        type=str2bool,
                         default=True,
                         help='include the column names')
     parser.add_argument('--index',
+                        type=str2bool,
                         default=True,
                         help='write row names')
     parser.add_argument('--index_label',
                         default=None,
                         help='column header for the row names')
     parser.add_argument('--mode',
                         default='w',
@@ -135,14 +131,15 @@
     parser.add_argument('--chunksize',
                         default=None,
                         help='rows to write at a time')
     parser.add_argument('--date_format',
                         default=None,
                         help='format string for datetime objects')
     parser.add_argument('--doublequote',
+                        type=str2bool,
                         default=True,
                         help='control quoting of quotechar inside fields')
     parser.add_argument('--escapechar',
                         default=None,
                         help='string of length 1. Used to escape sep and quotechar')
     parser.add_argument('--decimal',
                         default='.',
@@ -159,14 +156,10 @@
 
     if not os.path.exists(args.src_file):
         print(f"File {args.src_file} not found")
         sys.exit()
         
     args_dict = args.__dict__
     
-    # Turn boolean option values into true booleans:
-    for option in ['header', 'index', 'doublequote']:
-        args_dict[option] = str2bool(args_dict[option])
-
     
     main(**args_dict)
```

### Comparing `feather_tools-0.2.0/src/feather/test/fmore_copy.py` & `feather_tools-0.4.0/src/feather_tools/test/fless_copy.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 	
 
 '''
 import argparse
 import os
 import sys
 
-from feather.ftools_workhorse import FToolsWorkhorse
+from feather_tools.ftools_workhorse import FToolsWorkhorse
 
 def main(args, term_lines=None, term_cols=None, out_stream=sys.stdout):
     '''
     Create a feather-tools workhorse instance, and have it
     page through the feather file.
     
     Arguments term_lines, term_cols, and out_stream are only
```

### Comparing `feather_tools-0.2.0/src/feather/test/ftail_copy.py` & `feather_tools-0.4.0/src/feather_tools/test/ftail_copy.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+#!/usr/bin/env python
 '''
 Created on May 6, 2024
 
 @author: paepcke
 
 Emulates the Unix shell command 'tail' for .feather files.
 
@@ -13,15 +14,15 @@
 
 '''
 
 import argparse
 import os
 import sys
 
-from feather.ftools_workhorse import FToolsWorkhorse
+from feather_tools.ftools_workhorse import FToolsWorkhorse
 
 def main(args, term_lines=None, term_cols=None, out_stream=sys.stdout):
     '''
     Create a feather-tools workhorse instance, and have it
     load the feather file into a dataframe.
     
     Arguments term_lines, term_cols, and out_stream are only
```

### Comparing `feather_tools-0.2.0/src/feather/test/fwc_copy.py` & `feather_tools-0.4.0/src/feather_tools/test/fwc_copy.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 '''
 
 import argparse
 import os
 import sys
 
-from feather.ftools_workhorse import FToolsWorkhorse
+from feather_tools.ftools_workhorse import FToolsWorkhorse
 
 def main(args, term_lines=None, term_cols=None, out_stream=sys.stdout):
     '''
     Create a feather-tools workhorse instance, and have it
     load the feather file into a dataframe.
     
     Arguments term_lines, term_cols, and out_stream are only
```

### Comparing `feather_tools-0.2.0/src/feather/test/test_ftools_workhorse.py` & `feather_tools-0.4.0/src/feather_tools/test/test_ftools_workhorse.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 '''
 Created on May 1, 2024
 
 @author: paepcke
 '''
 from collections import namedtuple
-from feather.test.f2csv_copy import main as f2csv_main
-from feather.test.fmore_copy import main as fmore_main
-from feather.test.ftail_copy import main as ftail_main
-from feather.test.fwc_copy import main as fwc_main
+from feather_tools.test.f2csv_copy import main as f2csv_main
+from feather_tools.test.fless_copy import main as fless_main
+from feather_tools.test.ftail_copy import main as ftail_main
+from feather_tools.test.fwc_copy import main as fwc_main
 
-from feather.ftools_workhorse import Pager, FToolsWorkhorse
+from feather_tools.ftools_workhorse import Pager, FToolsWorkhorse
 from tempfile import NamedTemporaryFile
 from unittest.mock import patch
 import io
 import numpy as np
 import pandas as pd
 import sys
 import tempfile
 import unittest
 
 TEST_ALL = True
 #TEST_ALL = False
 
-class FMoreTester(unittest.TestCase):
+class FlessTester(unittest.TestCase):
 
 
     def setUp(self):
         self.create_test_files()
 
 
     def tearDown(self):
@@ -125,18 +125,18 @@
     #------------------------------------
     # test_paging
     #-------------------
     
     # @unittest.skipIf(TEST_ALL != True, 'skipping temporarily')
     # def test_paging(self):
     #
-    #     #_fmore = FMore(self.path_narrow_and_short.name)
-    #     _fmore = FMore(self.path_wide_and_long.name, lines=38, cols=111)
-    #     #_fmore = FMore(self.path_narrow_and_short.name)
-    #     #_fmore = FMore(self.path_wide_and_short.name)
+    #     #_fless = Fless(self.path_narrow_and_short.name)
+    #     _fless = Fless(self.path_wide_and_long.name, lines=38, cols=111)
+    #     #_fless = Fless(self.path_narrow_and_short.name)
+    #     #_fless = Fless(self.path_wide_and_short.name)
 
 
     #------------------------------------
     # test__num_broken_lines
     #-------------------
     
     @unittest.skipIf(TEST_ALL != True, 'skipping temporarily')
@@ -247,16 +247,16 @@
 
     #------------------------------------
     # test_logical_page_by_row
     #-------------------
     
     @unittest.skipIf(TEST_ALL != True, 'skipping temporarily')
     def test_logical_page_by_row(self):
-        fmore = FToolsWorkhorse(self.path_wide_and_long.name, lines=38, cols=111)
-        pager = fmore.pager
+        fless = FToolsWorkhorse(self.path_wide_and_long.name, lines=38, cols=111)
+        pager = fless.pager
         key_list = list(pager.pindex.keys())
         
         row_num = 0
         logical_pnum = pager.logical_page_by_row(row_num)
         row_low, row_hi   = pager.pindex[logical_pnum] 
         row_range    = range(row_low, row_hi) 
         self.assertTrue(row_num in row_range)
@@ -378,68 +378,68 @@
             self.assertEqual(output, expected)
             buf.close()
             
         finally:
             sys.stdout = sys.__stdout__
 
     #------------------------------------
-    # test_fmore
+    # test_fless
     #-------------------
     
     @unittest.skipIf(TEST_ALL != True, 'skipping temporarily')
-    def test_fmore(self):
+    def test_fless(self):
         
-        FmoreArgs = namedtuple('FmoreArgs', ['src_file'])
+        FlessArgs = namedtuple('FlessArgs', ['src_file'])
         test_term_lines = 24
         test_term_cols  = 80
         
         try:
             buf = io.StringIO()
-            args = FmoreArgs(self.path_narrow_and_short.name)
+            args = FlessArgs(self.path_narrow_and_short.name)
             
             # Ask for more tail lines than the df is long (the default 10):
-            with patch('feather.ftools_workhorse.Pager.getchr') as mock_input:
+            with patch('feather_tools.ftools_workhorse.Pager.getchr') as mock_input:
                 # Pretend user hit 'q' after first page:
                 mock_input.side_effect = ['q']
-                fmore_main(args, test_term_lines, test_term_cols, buf)
+                fless_main(args, test_term_lines, test_term_cols, buf)
             output = buf.getvalue()
             expected = ('foo    bar    fum\n'
                         '0: 10    100    1000\n'
                         '1: 20    200    2000\n'
                         '2: 30    300    3000\n'
                         '3: 40    400    4000\n'
                         '4: 50    500    5000\n'
                         '5: 60    600    6000\n')
 
             self.assertEqual(output, expected)
             buf.close()
             
             buf = io.StringIO()
-            with patch('feather.ftools_workhorse.Pager.getchr') as mock_input:
+            with patch('feather_tools.ftools_workhorse.Pager.getchr') as mock_input:
                 # Pretend user hits first 'n', then 'q':
                 mock_input.side_effect = ['n', 'q']
-                fmore_main(args, test_term_lines, test_term_cols, buf)
+                fless_main(args, test_term_lines, test_term_cols, buf)
             output = buf.getvalue()
             expected = ('foo    bar    fum\n'
                         '0: 10    100    1000\n'
                         '1: 20    200    2000\n'
                         '2: 30    300    3000\n'
                         '3: 40    400    4000\n'
                         '4: 50    500    5000\n'
                         '5: 60    600    6000\n')
             self.assertEqual(output, expected)
             
             # Larger df, where 'next' does show a second page:
 
-            args = FmoreArgs(self.path_wide_and_long.name)
+            args = FlessArgs(self.path_wide_and_long.name)
             buf = io.StringIO()
-            with patch('feather.ftools_workhorse.Pager.getchr') as mock_input:
+            with patch('feather_tools.ftools_workhorse.Pager.getchr') as mock_input:
                 # Pretend user hits first 'n', then 'q':
                 mock_input.side_effect = ['n', 'q']
-                fmore_main(args, test_term_lines, test_term_cols, buf)
+                fless_main(args, test_term_lines, test_term_cols, buf)
             output = buf.getvalue()
             expected = (
                 'Col0    Col1    Col2    Col3    Col4    Col5    Col6    Col7    Col8    Col9   \n'
                 'Col10    Col11    Col12    Col13    Col14    Col15    Col16    Col17    Col18   \n'
                 'Col19    Col20    Col21    Col22    Col23    Col24    Col25    Col26    Col27   \n'
                 'Col28    Col29    Col30    Col31    Col32    Col33    Col34    Col35    Col36   \n'
                 'Col37    Col38    Col39    Col40    Col41    Col42    Col43    Col44    Col45   \n'
@@ -478,22 +478,22 @@
                 '   288    289    290    291    292    293    294    295    296    297    298   \n'
                 '   299\n'
                 )
             self.assertEqual(output, expected)
             
             # Larger df, press 'n', then 'b', then 'q':
 
-            args = FmoreArgs(self.path_wide_and_long.name)
+            args = FlessArgs(self.path_wide_and_long.name)
             buf = io.StringIO()
-            with patch('feather.ftools_workhorse.Pager.getchr') as mock_input:
+            with patch('feather_tools.ftools_workhorse.Pager.getchr') as mock_input:
                 # Pretend user hits first 'n', then 'b' for 'back 1 page', then 'q'.
                 # That should yield the same displayed paged as hitting 'q' after
                 # the first page:
                 mock_input.side_effect = ['n', 'b', 'q']
-                fmore_main(args, test_term_lines, test_term_cols, buf)
+                fless_main(args, test_term_lines, test_term_cols, buf)
             output = buf.getvalue()
             
             # This test fails. No time to figure this out.
             # But works on command line:
             #*****self.assertEqual(output.strip(), expected.strip())
             
         finally:
@@ -579,15 +579,15 @@
             sys.stdout = sys.__stdout__
             
         
     # ----------------------- Utilities --------------
     
     def create_test_files(self):
         
-        self.tmpdir = tempfile.TemporaryDirectory(dir='/tmp', prefix='fmore_')
+        self.tmpdir = tempfile.TemporaryDirectory(dir='/tmp', prefix='fless_')
         
         self.df_narrow_and_short = pd.DataFrame(
             {'foo' : [10,20,30,40,50,60],
              'bar' : [100,200,300,400,500,600],
              'fum' : [1000,2000,3000,4000,5000,6000]
             })
 
@@ -605,26 +605,26 @@
         arr_wide_and_long = self.df_wide_and_short.values 
         for _ in list(range(10)):
             arr_wide_and_long = np.vstack((arr_wide_and_long, arr_wide_and_long))
         
         self.df_wide_and_long = pd.DataFrame(arr_wide_and_long, columns=self.df_wide_and_short.columns)
         
         self.path_narrow_and_short = tempfile.NamedTemporaryFile( 
-                                                                 suffix='.feather', 
-                                                                 prefix="fmore_", 
+                                                                 suffix='.feather_tools', 
+                                                                 prefix="fless_", 
                                                                  dir=self.tmpdir.name, 
                                                                  delete=False)
         self.path_wide_and_short = tempfile.NamedTemporaryFile(
-                                                               suffix='.feather', 
-                                                               prefix="fmore_", 
+                                                               suffix='.feather_tools', 
+                                                               prefix="fless_", 
                                                                dir=self.tmpdir.name, 
                                                                delete=False)
         self.path_wide_and_long = tempfile.NamedTemporaryFile(
-                                                              suffix='.feather', 
-                                                              prefix="fmore_", 
+                                                              suffix='.feather_tools', 
+                                                              prefix="fless_", 
                                                               dir=self.tmpdir.name, 
                                                               delete=False)
 
         
         self.df_narrow_and_short.to_feather(self.path_narrow_and_short)
         self.df_wide_and_short.to_feather(self.path_wide_and_short)
         self.df_wide_and_long.to_feather(self.path_wide_and_long)
```

### Comparing `feather_tools-0.2.0/src/feather_tools.egg-info/PKG-INFO` & `feather_tools-0.4.0/src/feather_tools.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,50 +1,46 @@
 Metadata-Version: 2.1
 Name: feather_tools
-Version: 0.2.0
+Version: 0.4.0
 Summary: Scripts to use for pyarrow feather files in a Linux terminal window
 Author-email: Andreas Paepcke <paepcke@cs.stanford.edu>
 Maintainer-email: Andreas Paepcke <paepcke@cs.stanford.edu>
 License: MIT License
-Project-URL: Homepage, https://github.com/paepcke/feather_tools
-Project-URL: Documentation, https://github.com/paepcke/feather_tools
-Project-URL: Repository, https://github.com/paepcke/feather_tools
+Project-URL: Homepage, https://github.com/paepcke/feather-tools
+Project-URL: Documentation, https://github.com/paepcke/feather-tools
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Requires-Dist: pandas>=2.2.2
 Requires-Dist: pyarrow>=16.0.0
 
 ## Description
 Stand-alone Unix shell command line tools for Apache's .feather formatted files:
 
 ```
-- fmore
+- fless
 - ftail
 - fwc (-l)
 - f2csv
 ```
 
-Each tool operates in the spirit of the analogous Unix shell command. Only the most basic uses of these original Unix tools are suported in their *f* version. For example, the `fwc` command operates like `wc -l`, i.e. it displays the number of datalines. But `wc -c` is not provided.
+Each tool operates in the spirit of the analogous Unix shell command. Only the most basic uses of these original Unix tools are suported in their *f* version. For example, the `fwc` command operates like `wc -l`, i.e. it displays the number of data rows. But `wc -c` is not provided.
 
 ## Installation:
 ```
 - Create virtual environment if desired
 - pip install feather-tools
 - pip install .
 ```
-
-For convenience, you might either include the location of the files in $PATH, or symlink the above files to where they are accessible from different directories. For example, `/usr/local/bin`.
+The files will be in .../site-packages/feather_tools. For convenience, you might add that location to $PATH.
 
 ## Usage:
 
-All Python imports are relative to `<proj-root>/src`. So ensure that your $PYTHONPATH includes that directory.
-
-### `fmore`
+### `fless`
 ```
-fmore <fpath>
+fless <fpath>
 ```
 Shows one screenful of the .feather file at a time. The number of rows displayed is determined by the terminal in which the command is issued. At the end of each displayed page, type a single character:
 
 - To show the next page: `spacebar`, or `\n`, or the character *n*
 - Back one page: *b*
 - Back to beginning (page 0): *s*
 - To the last page: *e*
@@ -55,25 +51,25 @@
 Displays the last *n* rows of the .feather file. Default is the lesser of 10, and the length of the data.
 
 **NOTE**: Starts the row display with the logical (i.e. terminal-height) page that contains the first line specified by the tail default or in the `--lines` argument. So a few more rows than requested may be displayed at the top.
 
 ### `fwc <fpath>`
 Is analogout to the Unix `wc -l`, and shows the number of data rows, not counting the column header.
 
-### `f2csv <src-fpath> <dst-fpath> `
+### `f2csv <src-fpath> [<dst-fpath>] `
 Writes a .csv file that contains the .feather data. Default separator is comma. Default output is stdout.
 
 The command line arguments are as in the [Pandas `df.to_csv()`](https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.to_csv.html) documentation. This means that the `index` keyword is True by default, while `index_label` is None. Which leads to ugly .csv like:
 ```
 ,foo,bar,fum
 Row0,1,2,3
 Row1,4,5,6
 Row2,7,8,9
 ```
-Where the `Row*n*` are the dataframe index. Note the orphan comma. To fix (same as with df.to_csv()):
+Where the `Row`*n* are the dataframe index. Note the orphan comma in the header. To fix (same as with df.to_csv()):
 ```
 f2csv --index=true --index_label=Rows file.feather
 
 Rows,foo,bar,fum
 Row0,1,2,3
 Row1,4,5,6
 Row2,7,8,9
@@ -83,10 +79,11 @@
 f2csv --index=false file.feather
 
 foo,bar,fum
 1,2,3
 4,5,6
 7,8,9
 ```
+If you clone this repo to make changes: all Python imports are relative to `<proj-root>/src`. So ensure that your $PYTHONPATH includes that directory.
 
 ## Testing
-Running nose2 in the project root runs the tests. One abnormality: in order to blend with Unix convention, the command files are without a '.py' extension. Examples: `fmore`, `fwc`. The downside is that unittest files cannot load Python files without .py extensions. Copies of the command files are therefore placed in the test subdirectory. The unittests run on those copies. If changes are made to the command files, then those copies must be updated before testing. Symlinks are not an option, because pip cannot recreate them during installation.
+Running nose2 in the project root runs the tests. One abnormality: in order to blend with Unix convention, the command files are without a '.py' extension. Examples: `fless`, `fwc`. The downside is that unittest files cannot load Python files without .py extensions. Copies of the command files are therefore placed in the test subdirectory. The unittests run on those copies. If changes are made to the command files, then those copies must be updated before testing. Symlinks are not an option, because pip cannot recreate them during installation.
```

