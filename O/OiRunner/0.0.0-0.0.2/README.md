# Comparing `tmp/oirunner-0.0.0.tar.gz` & `tmp/OiRunner-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oirunner-0.0.0.tar", last modified: Wed May  8 08:39:50 2024, max compression
+gzip compressed data, was "OiRunner-0.0.2.tar", last modified: Sun Mar 31 03:55:38 2024, max compression
```

## Comparing `oirunner-0.0.0.tar` & `OiRunner-0.0.2.tar`

### file list

```diff
@@ -1,52 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:39:50.272355 oirunner-0.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:39:50.256354 oirunner-0.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:39:50.260355 oirunner-0.0.0/.github/workflows/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1882 2024-05-08 08:39:03.000000 oirunner-0.0.0/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-05-08 08:39:03.000000 oirunner-0.0.0/.github/workflows/release.yml
--rwxr-xr-x   0 runner    (1001) docker     (127)     3110 2024-05-08 08:39:03.000000 oirunner-0.0.0/.gitignore
--rwxr-xr-x   0 runner    (1001) docker     (127)     1063 2024-05-08 08:39:03.000000 oirunner-0.0.0/LICENSE
--rwxr-xr-x   0 runner    (1001) docker     (127)       33 2024-05-08 08:39:03.000000 oirunner-0.0.0/MANIFEST.in
--rwxr-xr-x   0 runner    (1001) docker     (127)      485 2024-05-08 08:39:03.000000 oirunner-0.0.0/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:39:50.260355 oirunner-0.0.0/OiRunner/
--rwxr-xr-x   0 runner    (1001) docker     (127)     9476 2024-05-08 08:39:03.000000 oirunner-0.0.0/OiRunner/BetterRunner.py
--rwxr-xr-x   0 runner    (1001) docker     (127)       24 2024-05-08 08:39:03.000000 oirunner-0.0.0/OiRunner/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:39:50.268355 oirunner-0.0.0/OiRunner.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-08 08:39:50.000000 oirunner-0.0.0/OiRunner.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-05-08 08:39:50.000000 oirunner-0.0.0/OiRunner.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 08:39:50.000000 oirunner-0.0.0/OiRunner.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-08 08:39:50.000000 oirunner-0.0.0/OiRunner.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-08 08:39:50.000000 oirunner-0.0.0/OiRunner.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-08 08:39:50.268355 oirunner-0.0.0/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)     1389 2024-05-08 08:39:03.000000 oirunner-0.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:39:50.264355 oirunner-0.0.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-05-08 08:39:03.000000 oirunner-0.0.0/docs/automation.md
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-08 08:39:03.000000 oirunner-0.0.0/docs/judge.md
--rwxr-xr-x   0 runner    (1001) docker     (127)       99 2024-05-08 08:39:03.000000 oirunner-0.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-08 08:39:03.000000 oirunner-0.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 08:39:50.272355 oirunner-0.0.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)      575 2024-05-08 08:39:03.000000 oirunner-0.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:39:50.264355 oirunner-0.0.0/tests/
--rwxr-xr-x   0 runner    (1001) docker     (127)       24 2024-05-08 08:39:03.000000 oirunner-0.0.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:39:50.268355 oirunner-0.0.0/tests/data/
--rwxr-xr-x   0 runner    (1001) docker     (127)       25 2024-05-08 08:39:03.000000 oirunner-0.0.0/tests/data/a.in
--rwxr-xr-x   0 runner    (1001) docker     (127)      203 2024-05-08 08:39:03.000000 oirunner-0.0.0/tests/data/check.cpp
--rw-r--r--   0 runner    (1001) docker     (127)  2333995 2024-05-08 08:39:03.000000 oirunner-0.0.0/tests/data/check.exe
--rwxr-xr-x   0 runner    (1001) docker     (127)    26344 2024-05-08 08:39:03.000000 oirunner-0.0.0/tests/data/check.out
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:39:50.268355 oirunner-0.0.0/tests/data/check_data/
--rwxr-xr-x   0 runner    (1001) docker     (127)        1 2024-05-08 08:39:03.000000 oirunner-0.0.0/tests/data/check_data/1.ans
--rwxr-xr-x   0 runner    (1001) docker     (127)        2 2024-05-08 08:39:03.000000 oirunner-0.0.0/tests/data/check_data/1.in
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:39:48.000000 oirunner-0.0.0/tests/data/check_data/1.out
--rwxr-xr-x   0 runner    (1001) docker     (127)       12 2024-05-08 08:39:03.000000 oirunner-0.0.0/tests/data/check_data/2.ans
--rwxr-xr-x   0 runner    (1001) docker     (127)        2 2024-05-08 08:39:03.000000 oirunner-0.0.0/tests/data/check_data/2.in
--rwxr-xr-x   0 runner    (1001) docker     (127)        1 2024-05-08 08:39:45.000000 oirunner-0.0.0/tests/data/check_data/2.out
--rwxr-xr-x   0 runner    (1001) docker     (127)        5 2024-05-08 08:39:03.000000 oirunner-0.0.0/tests/data/check_data/3.ans
--rwxr-xr-x   0 runner    (1001) docker     (127)        2 2024-05-08 08:39:03.000000 oirunner-0.0.0/tests/data/check_data/3.in
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:39:45.000000 oirunner-0.0.0/tests/data/check_data/3.out
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-05-08 08:39:03.000000 oirunner-0.0.0/tests/data/check_data/large.ans
--rw-r--r--   0 runner    (1001) docker     (127)     9600 2024-05-08 08:39:03.000000 oirunner-0.0.0/tests/data/check_data/large.in
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 08:39:45.000000 oirunner-0.0.0/tests/data/check_data/large.out
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:39:03.000000 oirunner-0.0.0/tests/data/empty1.in
--rwxr-xr-x   0 runner    (1001) docker     (127)        2 2024-05-08 08:39:03.000000 oirunner-0.0.0/tests/data/empty2.in
--rwxr-xr-x   0 runner    (1001) docker     (127)       23 2024-05-08 08:39:03.000000 oirunner-0.0.0/tests/data/fail.cpp
--rwxr-xr-x   0 runner    (1001) docker     (127)       96 2024-05-08 08:39:03.000000 oirunner-0.0.0/tests/data/success.cpp
--rwxr-xr-x   0 runner    (1001) docker     (127)    15525 2024-05-08 08:39:03.000000 oirunner-0.0.0/tests/test_basic.py
+drwxrwxr-x   0 ste1      (1000) ste1      (1000)        0 2024-03-31 03:55:38.780882 OiRunner-0.0.2/
+-rw-rw-r--   0 ste1      (1000) ste1      (1000)     3093 2024-03-31 00:03:36.000000 OiRunner-0.0.2/.gitignore
+-rw-rw-r--   0 ste1      (1000) ste1      (1000)     1063 2024-03-30 14:51:20.000000 OiRunner-0.0.2/LICENSE
+-rw-rw-r--   0 ste1      (1000) ste1      (1000)       33 2024-03-30 23:51:49.000000 OiRunner-0.0.2/MANIFEST.in
+drwxrwxr-x   0 ste1      (1000) ste1      (1000)        0 2024-03-31 03:55:38.779882 OiRunner-0.0.2/OiRunner/
+-rw-rw-r--   0 ste1      (1000) ste1      (1000)        0 2024-03-30 15:11:27.000000 OiRunner-0.0.2/OiRunner/__init__.py
+-rw-rw-r--   0 ste1      (1000) ste1      (1000)     8789 2024-03-31 03:38:04.000000 OiRunner-0.0.2/OiRunner/run.py
+drwxrwxr-x   0 ste1      (1000) ste1      (1000)        0 2024-03-31 03:55:38.779882 OiRunner-0.0.2/OiRunner.egg-info/
+-rw-r--r--   0 ste1      (1000) ste1      (1000)      270 2024-03-31 03:55:38.000000 OiRunner-0.0.2/OiRunner.egg-info/PKG-INFO
+-rw-rw-r--   0 ste1      (1000) ste1      (1000)      264 2024-03-31 03:55:38.000000 OiRunner-0.0.2/OiRunner.egg-info/SOURCES.txt
+-rw-rw-r--   0 ste1      (1000) ste1      (1000)        1 2024-03-31 03:55:38.000000 OiRunner-0.0.2/OiRunner.egg-info/dependency_links.txt
+-rw-rw-r--   0 ste1      (1000) ste1      (1000)       44 2024-03-31 03:55:38.000000 OiRunner-0.0.2/OiRunner.egg-info/entry_points.txt
+-rw-rw-r--   0 ste1      (1000) ste1      (1000)        9 2024-03-31 03:55:38.000000 OiRunner-0.0.2/OiRunner.egg-info/top_level.txt
+-rw-r--r--   0 ste1      (1000) ste1      (1000)      270 2024-03-31 03:55:38.779882 OiRunner-0.0.2/PKG-INFO
+-rw-rw-r--   0 ste1      (1000) ste1      (1000)       46 2024-03-30 14:51:20.000000 OiRunner-0.0.2/README.md
+-rw-rw-r--   0 ste1      (1000) ste1      (1000)       99 2024-03-30 15:13:42.000000 OiRunner-0.0.2/pyproject.toml
+-rw-rw-r--   0 ste1      (1000) ste1      (1000)       38 2024-03-31 03:55:38.780882 OiRunner-0.0.2/setup.cfg
+-rw-rw-r--   0 ste1      (1000) ste1      (1000)      504 2024-03-31 03:55:11.000000 OiRunner-0.0.2/setup.py
```

### Comparing `oirunner-0.0.0/.gitignore` & `OiRunner-0.0.2/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
 *$py.class
 
 # C extensions
 *.so
-a.out
 
 # Distribution / packaging
 .Python
 build/
 develop-eggs/
 dist/
 downloads/
@@ -47,15 +46,14 @@
 nosetests.xml
 coverage.xml
 *.cover
 *.py,cover
 .hypothesis/
 .pytest_cache/
 cover/
-~*/
 
 # Translations
 *.mo
 *.pot
 
 # Django stuff:
 *.log
@@ -158,9 +156,8 @@
 # PyCharm
 #  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
 #  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
 #.idea/
 
-token
-*.html
+token
```

### Comparing `oirunner-0.0.0/LICENSE` & `OiRunner-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `oirunner-0.0.0/OiRunner/BetterRunner.py` & `OiRunner-0.0.2/OiRunner/run.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,261 +1,243 @@
-# -*- coding: utf-8 -*-
 import subprocess as sp
 import argparse
 import sys
 import os
 import shutil
 import time
-from typing import Optional
 
 
-class Functions:
-
-    def __init__(self) -> None:
+class BetterRunner:
+    def __init__(self):
         pass
 
-    def _modify_file(self, file_name: str, file_type: str) -> int:
+    def cmd_parse(self):
         '''
-        Split the file into multiple files by line, with the output file located at ~tmp/.
-
-        Args:
-            file_name -- The name of input file.
+        命令行解析
+        '''
+        pa = argparse.ArgumentParser()
+        pa.add_argument('filename', help="要编译的cpp文件(省略'.cpp')")
+        pa.add_argument('-n', '--name', default="a", help="生成的可执行文件名(省略'.exe')")
+        pa.add_argument('-j', '--judge', action='store_true', help="是否评测")
+        # pa.add_argument('-u','--use_multiple_processes',action='store_true',help="是否使用多进程评测")
+        pa.add_argument('-p', '--print', action='store_true', help="是否显示输出")
+        pa.add_argument('-if', '--inputfile', default='in.txt', help="输入文件名")
+        pa.add_argument('-of', '--outputfile', default='out.txt', help="输出文件名")
+        pa.add_argument('-af', '--answerfile', default='ans.txt', help="答案文件名")
+        pa.add_argument('-g', '--gdb', action='store_true', help="答案错误时是否使用gdb打开")
+        pa.add_argument('-gf', '--gdbfile', default=None, help="gdb调试输入文件")
+        pa.add_argument('--directgdb', action='store_true', help="直接使用gdb调试")
+        pa.add_argument('--onlyinput', action='store_true', help="使用文件输入（-j时无效）")
+        pa.add_argument('--onlyoutput', action='store_true', help="使用文件输出（-j时无效）")
+        self.args = pa.parse_args()
 
-            file_type -- The filename extension of input file.
+        self.args.use_multiple_processes = False
+        self.input_file = self.args.inputfile
+        self.output_file = self.args.outputfile
+        self.answer_file = self.args.answerfile
+        if sys.platform == "linux":
+            self.args.name = "./" + self.args.name + '.out'
+        elif sys.platform == "win32":
+            self.args.name = self.args.name + '.exe'
 
-        Returns:
-        i -- Number of output files.
+    def compile(self):
+        '''
+        编译文件
+        '''
+        try:
+            compile = sp.Popen(['g++', self.args.filename + '.cpp', '-g', '-o', self.args.name])
+            compile.wait()
+            if compile.returncode == 0:
+                print("编译成功")
+            else:
+                print("编译失败")
+                exit(0)
+        except KeyboardInterrupt:
+            print("\n手动退出，祝AC~(^v^)")
+            exit(0)
 
-        Raise:
-        SystemExit -- The file is empty.
+    def _modify_file(self, file_name, file_type):
+        '''
+        将文件按行分割
         '''
         i = 1
         a = ""
-        flag = 0
-        if not os.path.exists("~tmp"):
-            os.mkdir("~tmp")
+        if not os.path.exists('~tmp'):
+            os.mkdir('~tmp')
         with open(file_name, "r") as f:
             for line in f:
-                flag = 1
                 if line.rstrip():
                     a += f"{line}"
                 else:
                     if not a:
-                        print(f"error:{file_name} is empty.")
-                        shutil.rmtree("~tmp")
-                        sys.exit()
+                        print(f"error:{file_name}文件为空")
+                        shutil.rmtree('~tmp')
+                        exit(0)
                     with open(f"~tmp/{i}.{file_type}", "w") as _f:
                         _f.write(a)
                     i += 1
                     a = ""
-            if not flag:
-                print(f"error:{file_name} is empty.")
-                shutil.rmtree("~tmp")
-                sys.exit()
-
         if a:
             with open(f"~tmp/{i}.{file_type}", "w") as _f:
                 _f.write(a)
         return i
 
-    def _output(self, num: int, opt_file: str) -> None:
+    def _output(self, num):
         '''
-        Merge and output the split files.
-
-        Args:
-        num -- The number of files to merge.
-        opt_file -- Output file name.
+        将分割后的文件合并输出
         '''
         a = ""
         for file_num in range(1, num+1):
             a += f"#{file_num}:\n"
             with open(f"~tmp/{file_num}.out", "r") as _f:
                 for line in _f:
                     a += f"{line}"
 
-        with open(opt_file, "w") as _out:
+        with open(self.args.outputfile, "w") as _out:
             _out.write(a)
 
-
-class BetterRunner:
-    def __init__(self) -> None:
-        self.input_file = "in.txt"
-        self.output_file = "out.txt"
-        self.answer_file = "ans.txt"
-        self.func = Functions()
-
-    def cmd_parse(self) -> None:
-        '''Parse the command'''
-        pa = argparse.ArgumentParser()
-        pa.add_argument("filename", help="CPP file to be compiled (omitting '. cpp').")
-        pa.add_argument("-n", "--name", default="a", help="Generate executable file name (omit '. exe').")
-        pa.add_argument("-j", "--judge", action="store_true", help="Whether to evaluate.")
-        pa.add_argument("-p", "--print", action="store_true", help="Whether to print.")
-        pa.add_argument("-if", "--inputfile", default="in.txt", help="Input file name.")
-        pa.add_argument("-of", "--outputfile", default="out.txt", help="Output file name.")
-        pa.add_argument("-af", "--answerfile", default="ans.txt", help="Answer file name.")
-        pa.add_argument("-g", "--gdb", action="store_true", help="Whether to debug via gdb when the answer is incorrect.")
-        pa.add_argument("-d", "--directgdb", action="store_true", help="Directly using gdb for debugging.")
-        pa.add_argument("--onlyinput", action="store_true", help="Using file input (invalid for - j).")
-        pa.add_argument("--onlyoutput", action="store_true", help="Using file output (invalid when - j).")
-        self.args = pa.parse_args()
-        self.input_file = self.args.inputfile
-        self.output_file = self.args.outputfile
-        self.answer_file = self.args.answerfile
-        if sys.platform == "linux":
-            self.args.name = "./" + self.args.name + ".out"
-        elif sys.platform == "win32":
-            self.args.name = self.args.name + ".exe"
-
-    def compile(self) -> None:
-        '''
-        Compile files and generate executable files.
-
-        Raise：
-        SystemExit -- Compilation failed.
-        '''
-        try:
-            compile = sp.Popen(["g++", self.args.filename + ".cpp", "-g", "-o", self.args.name])
-            compile.wait()
-            if compile.returncode == 0:
-                print("Compilation successful.")
-            else:
-                print("Compilation failed.")
-                sys.exit()
-
-        # Can't sent Ctrl+c and get the messages.
-        except KeyboardInterrupt:  # pragma: no cover
-            print("\nManually exit, wish AC~(^ v ^)")
-            sys.exit()
-
-    def _check(self, opt_file: str, ipt_file: str, ans_file: str,
-               file_num: int = 0, run_file: Optional[str] = None, if_print: Optional[bool] = None) -> bool:
+    def _check(self, opt_file, ipt_file, ans_file, file_num=0, run_file=None):
         '''
-        Local evaluation and get results.
-
-        Args：
-        opt_file -- Output file name.
-
-        ipt_file -- Input file name.
-
-        ans_file -- Answer file name.
-
-        file_num -- File number.
-        run_file -- Executable file name (None means use the value of the command line parameter).
-        if_print -- Whether to output (None means use the value of the command line parameter).
-
-        Return：
-        if_pass -- Whether to pass the test.
+        本地评测
         '''
 
         print(f"#{file_num}:")
 
         if run_file is None:
             run_file = self.args.name
-        if if_print is None:
-            if_print = self.args.print
 
         with open(opt_file, "w") as _out, open(ipt_file, "r") as _in:
             run = sp.Popen([run_file], stdin=_in, stdout=_out)
 
-            ft = time.time()
-            run.wait()
-            now = time.time() - ft
+            if not self.args.use_multiple_processes:
+                ft = time.time()
+                run.wait()
+                now = time.time() - ft
 
             if run.returncode != 0:
-                print(f"The return value is {run.returncode}. There may be issues with the program running.")
+                print(f"返回值为{run.returncode}，程序运行可能有问题")
 
         with open(ans_file, "r") as ans, open(opt_file, "r") as my_ans:
-            ans_list = [line.rstrip() for line in ans if line.rstrip()]
-            my_ans_list = [line.rstrip() for line in my_ans if line.rstrip()]
-            if ans_list == my_ans_list:
-                if if_print:
-                    print(f"Correct answer, takes {now:.5} seconds.")
+            ans = [line.rstrip() for line in ans if line.rstrip()]
+            my_ans = [line.rstrip() for line in my_ans if line.rstrip()]
+            if ans == my_ans:
+                if self.args.print:
+                    # print(f"标准答案：{ans}\n实际答案：{my_ans}")
+                    print(f"答案正确，用时{now:.5}")
                 else:
-                    print("Correct answer.")
+                    print("答案正确")
                 return True
             else:
-                if if_print:
-                    if len(ans_list) < 10:
-                        print(f"Standard answer:{ans_list}\nYour answer:{my_ans_list}")
-                    else:
-                        print("The number of answer lines is too large.")
-                    print("Wrong answer.")
-                    print("Error data:")
+                if self.args.print:
+                    # print(f"标准答案：{ans}\n实际答案：{my_ans}")
+                    print("答案错误")
+                    print("错误数据：")
                     with open(ipt_file, "r") as _in:
-                        data_list = [line.rstrip() for line in _in if line.rstrip()]
-                        data: str = ""
-                        for data_line in data_list:
-                            data += data_line
-                            data += "\n"
-                        if len(data) < 500:
-                            print(data)
-                        else:
-                            print("The number of data words is too large.")
+                        for line in _in:
+                            if line.rstrip():
+                                print(line.rstrip())
                 else:
-                    print("Wrong answer.")
+                    print("答案错误")
 
                 return False
 
-    def run(self) -> None:
-        '''Main function.'''
+    def _copy_file(self, i):
+        '''
+        复制文件，为多进程评测准备
+        '''
+        for file_num in range(1, i + 1):
+            dst = os.path.join(r'~tmp/', f"{file_num}_{self.args.name}")
+            shutil.copy2(self.args.name, dst)
+
+    def _debug(self):
+        """
+        使用gdb调试
+        """
+        if self.args.gdbfile is None:
+            gdb = sp.Popen(['gdb', self.args.name])
+            gdb.wait()
+        else:
+            with open(self.args.gdbfile, "r") as f:
+                gdb = sp.Popen(['gdb', self.args.name], stdin=sp.PIPE, text=True)
+                for line in f:
+                    if line.rstrip():
+                        line = str(line.rstrip()) + "\n"
+                        # if line != "r":
+                        #     line = line + "\n"
+                        gdb.stdin.write(line)
+                        gdb.stdin.flush()
+                # print(gdb.stdout.read())
+                # gdb.stdin.close()
+
+                gdb.stdin = sys.stdin
+                gdb.wait()
+
+    def run(self):
+        """
+        程序主函数
+        """
         try:
             if self.args.directgdb:
-                gdb = sp.Popen(["gdb", self.args.name])
-                gdb.wait()
-                sys.exit()
+                self._debug()
+                exit(0)
 
             if self.args.judge:
                 flag = 0
 
-                if os.path.exists("~tmp"):
-                    shutil.rmtree("~tmp")
-                self.func._modify_file(self.input_file, "in")
-                i = self.func._modify_file(self.answer_file, "ans")
+                if os.path.exists('~tmp'):
+                    shutil.rmtree('~tmp')
+                self._modify_file(self.args.inputfile, "in")
+                i = self._modify_file(self.args.answerfile, "ans")
+                if self.args.use_multiple_processes:
+                    self._copy_file(i)
 
                 for file_num in range(1, i + 1):
-                    judge = self._check(f"~tmp/{file_num}.out", f"~tmp/{file_num}.in", f"~tmp/{file_num}.ans",
-                                        file_num)
+
+                    if self.args.use_multiple_processes:
+                        judge = self._check(f"~tmp/{file_num}.out", f"~tmp/{file_num}.in", f"~tmp/{file_num}.ans",
+                                            file_num, f"~tmp/{file_num}_{self.args.name}")
+                    else:
+                        judge = self._check(f"~tmp/{file_num}.out", f"~tmp/{file_num}.in", f"~tmp/{file_num}.ans",
+                                            file_num)
+
                     if not judge:
                         flag += 1
 
-                print(f"#final:Accuracy{((i - flag) / i): .2%}")
-                self.func._output(i, self.output_file)
-                shutil.rmtree("~tmp")
+                print(f"#final:正确率{((i - flag) / i) : .2%}")
+                self._output(i)
+                shutil.rmtree('~tmp')
 
                 if self.args.gdb and flag > 0:
-                    gdb = sp.Popen(["gdb", self.args.name])
-                    gdb.wait()
+                    self._debug()
 
             else:
                 if self.args.onlyinput:
                     with open(self.input_file, "r") as _in:
-                        print("The file has been executed.")
+                        print("文件已执行")
                         run = sp.Popen([self.args.name], stdin=_in)
 
                 elif self.args.onlyoutput:
                     with open(self.output_file, "w") as _out:
                         run = sp.Popen([self.args.name], stdout=_out)
 
                 else:
                     run = sp.Popen([self.args.name])
 
                 run.wait()
                 if run.returncode != 0:
-                    print(f"The return value is {run.returncode}. There may be issues with the program running.")
+                    print(f"返回值为{run.returncode}，程序运行可能有问题")
 
-        # Can't sent Ctrl+c and get the messages.
-        except KeyboardInterrupt:  # pragma: no cover
-            if os.path.exists("~tmp"):
-                shutil.rmtree("~tmp")
-            print("\nManually exit, wish AC~(^ v ^)")
+        except KeyboardInterrupt:
+            if os.path.exists('~tmp'):
+                shutil.rmtree('~tmp')
+            print("\n手动退出，祝AC~(^v^)")
 
 
 def main():
     runner = BetterRunner()
     runner.cmd_parse()
     runner.compile()
     runner.run()
 
 
 if __name__ == "__main__":
-    main()  # pragma: no cover
+    main()
```

