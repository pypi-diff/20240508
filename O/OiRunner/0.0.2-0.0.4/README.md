# Comparing `tmp/OiRunner-0.0.2.tar.gz` & `tmp/oirunner-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OiRunner-0.0.2.tar", last modified: Sun Mar 31 03:55:38 2024, max compression
+gzip compressed data, was "oirunner-0.0.4.tar", last modified: Wed May  8 09:02:04 2024, max compression
```

## Comparing `OiRunner-0.0.2.tar` & `oirunner-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,51 @@
-drwxrwxr-x   0 ste1      (1000) ste1      (1000)        0 2024-03-31 03:55:38.780882 OiRunner-0.0.2/
--rw-rw-r--   0 ste1      (1000) ste1      (1000)     3093 2024-03-31 00:03:36.000000 OiRunner-0.0.2/.gitignore
--rw-rw-r--   0 ste1      (1000) ste1      (1000)     1063 2024-03-30 14:51:20.000000 OiRunner-0.0.2/LICENSE
--rw-rw-r--   0 ste1      (1000) ste1      (1000)       33 2024-03-30 23:51:49.000000 OiRunner-0.0.2/MANIFEST.in
-drwxrwxr-x   0 ste1      (1000) ste1      (1000)        0 2024-03-31 03:55:38.779882 OiRunner-0.0.2/OiRunner/
--rw-rw-r--   0 ste1      (1000) ste1      (1000)        0 2024-03-30 15:11:27.000000 OiRunner-0.0.2/OiRunner/__init__.py
--rw-rw-r--   0 ste1      (1000) ste1      (1000)     8789 2024-03-31 03:38:04.000000 OiRunner-0.0.2/OiRunner/run.py
-drwxrwxr-x   0 ste1      (1000) ste1      (1000)        0 2024-03-31 03:55:38.779882 OiRunner-0.0.2/OiRunner.egg-info/
--rw-r--r--   0 ste1      (1000) ste1      (1000)      270 2024-03-31 03:55:38.000000 OiRunner-0.0.2/OiRunner.egg-info/PKG-INFO
--rw-rw-r--   0 ste1      (1000) ste1      (1000)      264 2024-03-31 03:55:38.000000 OiRunner-0.0.2/OiRunner.egg-info/SOURCES.txt
--rw-rw-r--   0 ste1      (1000) ste1      (1000)        1 2024-03-31 03:55:38.000000 OiRunner-0.0.2/OiRunner.egg-info/dependency_links.txt
--rw-rw-r--   0 ste1      (1000) ste1      (1000)       44 2024-03-31 03:55:38.000000 OiRunner-0.0.2/OiRunner.egg-info/entry_points.txt
--rw-rw-r--   0 ste1      (1000) ste1      (1000)        9 2024-03-31 03:55:38.000000 OiRunner-0.0.2/OiRunner.egg-info/top_level.txt
--rw-r--r--   0 ste1      (1000) ste1      (1000)      270 2024-03-31 03:55:38.779882 OiRunner-0.0.2/PKG-INFO
--rw-rw-r--   0 ste1      (1000) ste1      (1000)       46 2024-03-30 14:51:20.000000 OiRunner-0.0.2/README.md
--rw-rw-r--   0 ste1      (1000) ste1      (1000)       99 2024-03-30 15:13:42.000000 OiRunner-0.0.2/pyproject.toml
--rw-rw-r--   0 ste1      (1000) ste1      (1000)       38 2024-03-31 03:55:38.780882 OiRunner-0.0.2/setup.cfg
--rw-rw-r--   0 ste1      (1000) ste1      (1000)      504 2024-03-31 03:55:11.000000 OiRunner-0.0.2/setup.py
+drwxrwxr-x   0 ste1      (1000) ste1      (1000)        0 2024-05-08 09:02:04.508791 oirunner-0.0.4/
+drwxrwxr-x   0 ste1      (1000) ste1      (1000)        0 2024-05-08 09:02:04.500790 oirunner-0.0.4/.github/
+drwxrwxr-x   0 ste1      (1000) ste1      (1000)        0 2024-05-08 09:02:04.502791 oirunner-0.0.4/.github/workflows/
+-rwxrwxr-x   0 ste1      (1000) ste1      (1000)     1882 2024-05-08 08:02:13.000000 oirunner-0.0.4/.github/workflows/main.yml
+-rw-rw-r--   0 ste1      (1000) ste1      (1000)     1335 2024-05-08 08:24:04.000000 oirunner-0.0.4/.github/workflows/release.yml
+-rwxrwxr-x   0 ste1      (1000) ste1      (1000)     3110 2024-05-08 08:00:49.000000 oirunner-0.0.4/.gitignore
+-rwxrwxr-x   0 ste1      (1000) ste1      (1000)     1063 2024-03-30 14:51:20.000000 oirunner-0.0.4/LICENSE
+-rwxrwxr-x   0 ste1      (1000) ste1      (1000)       33 2024-03-30 23:51:49.000000 oirunner-0.0.4/MANIFEST.in
+-rwxrwxr-x   0 ste1      (1000) ste1      (1000)      485 2024-05-08 09:00:42.000000 oirunner-0.0.4/Makefile
+drwxrwxr-x   0 ste1      (1000) ste1      (1000)        0 2024-05-08 09:02:04.502791 oirunner-0.0.4/OiRunner/
+-rwxrwxr-x   0 ste1      (1000) ste1      (1000)     9476 2024-05-08 06:06:43.000000 oirunner-0.0.4/OiRunner/BetterRunner.py
+-rwxrwxr-x   0 ste1      (1000) ste1      (1000)       46 2024-05-08 09:01:46.000000 oirunner-0.0.4/OiRunner/__init__.py
+drwxrwxr-x   0 ste1      (1000) ste1      (1000)        0 2024-05-08 09:02:04.508791 oirunner-0.0.4/OiRunner.egg-info/
+-rw-r--r--   0 ste1      (1000) ste1      (1000)     3148 2024-05-08 09:02:04.000000 oirunner-0.0.4/OiRunner.egg-info/PKG-INFO
+-rw-rw-r--   0 ste1      (1000) ste1      (1000)      900 2024-05-08 09:02:04.000000 oirunner-0.0.4/OiRunner.egg-info/SOURCES.txt
+-rw-rw-r--   0 ste1      (1000) ste1      (1000)        1 2024-05-08 09:02:04.000000 oirunner-0.0.4/OiRunner.egg-info/dependency_links.txt
+-rw-rw-r--   0 ste1      (1000) ste1      (1000)       15 2024-05-08 09:02:04.000000 oirunner-0.0.4/OiRunner.egg-info/top_level.txt
+-rw-r--r--   0 ste1      (1000) ste1      (1000)     3148 2024-05-08 09:02:04.508791 oirunner-0.0.4/PKG-INFO
+-rwxrwxr-x   0 ste1      (1000) ste1      (1000)     1389 2024-05-08 06:06:43.000000 oirunner-0.0.4/README.md
+drwxrwxr-x   0 ste1      (1000) ste1      (1000)        0 2024-05-08 09:02:04.503790 oirunner-0.0.4/docs/
+-rw-rw-r--   0 ste1      (1000) ste1      (1000)      849 2024-05-08 06:06:43.000000 oirunner-0.0.4/docs/automation.md
+-rw-rw-r--   0 ste1      (1000) ste1      (1000)     1758 2024-05-08 06:06:43.000000 oirunner-0.0.4/docs/judge.md
+-rwxrwxr-x   0 ste1      (1000) ste1      (1000)      653 2024-05-08 08:54:59.000000 oirunner-0.0.4/pyproject.toml
+-rw-rw-r--   0 ste1      (1000) ste1      (1000)       50 2024-04-28 06:04:32.000000 oirunner-0.0.4/requirements.txt
+-rw-rw-r--   0 ste1      (1000) ste1      (1000)       38 2024-05-08 09:02:04.508791 oirunner-0.0.4/setup.cfg
+-rwxrwxr-x   0 ste1      (1000) ste1      (1000)      490 2024-05-08 08:50:27.000000 oirunner-0.0.4/setup.py
+drwxrwxr-x   0 ste1      (1000) ste1      (1000)        0 2024-05-08 09:02:04.503790 oirunner-0.0.4/tests/
+-rwxrwxr-x   0 ste1      (1000) ste1      (1000)       24 2024-04-28 06:04:32.000000 oirunner-0.0.4/tests/__init__.py
+drwxrwxr-x   0 ste1      (1000) ste1      (1000)        0 2024-05-08 09:02:04.506791 oirunner-0.0.4/tests/data/
+-rwxrwxr-x   0 ste1      (1000) ste1      (1000)       25 2024-04-07 08:13:00.000000 oirunner-0.0.4/tests/data/a.in
+-rwxrwxr-x   0 ste1      (1000) ste1      (1000)      203 2024-05-08 07:24:00.000000 oirunner-0.0.4/tests/data/check.cpp
+-rw-rw-r--   0 ste1      (1000) ste1      (1000)  2333995 2024-05-08 06:06:43.000000 oirunner-0.0.4/tests/data/check.exe
+-rwxrwxr-x   0 ste1      (1000) ste1      (1000)    26344 2024-05-08 06:06:43.000000 oirunner-0.0.4/tests/data/check.out
+drwxrwxr-x   0 ste1      (1000) ste1      (1000)        0 2024-05-08 09:02:04.507791 oirunner-0.0.4/tests/data/check_data/
+-rwxrwxr-x   0 ste1      (1000) ste1      (1000)        1 2024-04-11 05:50:21.000000 oirunner-0.0.4/tests/data/check_data/1.ans
+-rwxrwxr-x   0 ste1      (1000) ste1      (1000)        2 2024-04-11 05:50:18.000000 oirunner-0.0.4/tests/data/check_data/1.in
+-rwxrwxr-x   0 ste1      (1000) ste1      (1000)        0 2024-05-08 09:02:00.000000 oirunner-0.0.4/tests/data/check_data/1.out
+-rwxrwxr-x   0 ste1      (1000) ste1      (1000)       12 2024-04-11 05:50:40.000000 oirunner-0.0.4/tests/data/check_data/2.ans
+-rwxrwxr-x   0 ste1      (1000) ste1      (1000)        2 2024-04-11 05:50:28.000000 oirunner-0.0.4/tests/data/check_data/2.in
+-rwxrwxr-x   0 ste1      (1000) ste1      (1000)        1 2024-05-08 09:01:59.000000 oirunner-0.0.4/tests/data/check_data/2.out
+-rwxrwxr-x   0 ste1      (1000) ste1      (1000)        5 2024-04-11 05:50:54.000000 oirunner-0.0.4/tests/data/check_data/3.ans
+-rwxrwxr-x   0 ste1      (1000) ste1      (1000)        2 2024-04-11 05:50:48.000000 oirunner-0.0.4/tests/data/check_data/3.in
+-rwxrwxr-x   0 ste1      (1000) ste1      (1000)        0 2024-05-08 09:01:59.000000 oirunner-0.0.4/tests/data/check_data/3.out
+-rw-rw-r--   0 ste1      (1000) ste1      (1000)      382 2024-05-08 06:06:43.000000 oirunner-0.0.4/tests/data/check_data/large.ans
+-rw-rw-r--   0 ste1      (1000) ste1      (1000)     9600 2024-05-08 06:06:43.000000 oirunner-0.0.4/tests/data/check_data/large.in
+-rw-rw-r--   0 ste1      (1000) ste1      (1000)        0 2024-05-08 09:01:59.000000 oirunner-0.0.4/tests/data/check_data/large.out
+-rwxrwxr-x   0 ste1      (1000) ste1      (1000)        0 2024-04-07 07:56:52.000000 oirunner-0.0.4/tests/data/empty1.in
+-rwxrwxr-x   0 ste1      (1000) ste1      (1000)        2 2024-04-07 08:17:43.000000 oirunner-0.0.4/tests/data/empty2.in
+-rwxrwxr-x   0 ste1      (1000) ste1      (1000)       23 2024-03-31 16:33:50.000000 oirunner-0.0.4/tests/data/fail.cpp
+-rwxrwxr-x   0 ste1      (1000) ste1      (1000)       96 2024-03-31 13:39:27.000000 oirunner-0.0.4/tests/data/success.cpp
+-rwxrwxr-x   0 ste1      (1000) ste1      (1000)    15525 2024-05-08 08:00:49.000000 oirunner-0.0.4/tests/test_basic.py
```

### Comparing `OiRunner-0.0.2/.gitignore` & `oirunner-0.0.4/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
 *$py.class
 
 # C extensions
 *.so
+a.out
 
 # Distribution / packaging
 .Python
 build/
 develop-eggs/
 dist/
 downloads/
@@ -46,14 +47,15 @@
 nosetests.xml
 coverage.xml
 *.cover
 *.py,cover
 .hypothesis/
 .pytest_cache/
 cover/
+~*/
 
 # Translations
 *.mo
 *.pot
 
 # Django stuff:
 *.log
@@ -156,8 +158,9 @@
 # PyCharm
 #  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
 #  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
 #.idea/
 
-token
+token
+*.html
```

### Comparing `OiRunner-0.0.2/LICENSE` & `oirunner-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `OiRunner-0.0.2/OiRunner/run.py` & `oirunner-0.0.4/OiRunner/BetterRunner.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,243 +1,261 @@
+# -*- coding: utf-8 -*-
 import subprocess as sp
 import argparse
 import sys
 import os
 import shutil
 import time
+from typing import Optional
 
 
-class BetterRunner:
-    def __init__(self):
+class Functions:
+
+    def __init__(self) -> None:
         pass
 
-    def cmd_parse(self):
+    def _modify_file(self, file_name: str, file_type: str) -> int:
         '''
-        命令行解析
-        '''
-        pa = argparse.ArgumentParser()
-        pa.add_argument('filename', help="要编译的cpp文件(省略'.cpp')")
-        pa.add_argument('-n', '--name', default="a", help="生成的可执行文件名(省略'.exe')")
-        pa.add_argument('-j', '--judge', action='store_true', help="是否评测")
-        # pa.add_argument('-u','--use_multiple_processes',action='store_true',help="是否使用多进程评测")
-        pa.add_argument('-p', '--print', action='store_true', help="是否显示输出")
-        pa.add_argument('-if', '--inputfile', default='in.txt', help="输入文件名")
-        pa.add_argument('-of', '--outputfile', default='out.txt', help="输出文件名")
-        pa.add_argument('-af', '--answerfile', default='ans.txt', help="答案文件名")
-        pa.add_argument('-g', '--gdb', action='store_true', help="答案错误时是否使用gdb打开")
-        pa.add_argument('-gf', '--gdbfile', default=None, help="gdb调试输入文件")
-        pa.add_argument('--directgdb', action='store_true', help="直接使用gdb调试")
-        pa.add_argument('--onlyinput', action='store_true', help="使用文件输入（-j时无效）")
-        pa.add_argument('--onlyoutput', action='store_true', help="使用文件输出（-j时无效）")
-        self.args = pa.parse_args()
+        Split the file into multiple files by line, with the output file located at ~tmp/.
 
-        self.args.use_multiple_processes = False
-        self.input_file = self.args.inputfile
-        self.output_file = self.args.outputfile
-        self.answer_file = self.args.answerfile
-        if sys.platform == "linux":
-            self.args.name = "./" + self.args.name + '.out'
-        elif sys.platform == "win32":
-            self.args.name = self.args.name + '.exe'
+        Args:
+            file_name -- The name of input file.
 
-    def compile(self):
-        '''
-        编译文件
-        '''
-        try:
-            compile = sp.Popen(['g++', self.args.filename + '.cpp', '-g', '-o', self.args.name])
-            compile.wait()
-            if compile.returncode == 0:
-                print("编译成功")
-            else:
-                print("编译失败")
-                exit(0)
-        except KeyboardInterrupt:
-            print("\n手动退出，祝AC~(^v^)")
-            exit(0)
+            file_type -- The filename extension of input file.
 
-    def _modify_file(self, file_name, file_type):
-        '''
-        将文件按行分割
+        Returns:
+        i -- Number of output files.
+
+        Raise:
+        SystemExit -- The file is empty.
         '''
         i = 1
         a = ""
-        if not os.path.exists('~tmp'):
-            os.mkdir('~tmp')
+        flag = 0
+        if not os.path.exists("~tmp"):
+            os.mkdir("~tmp")
         with open(file_name, "r") as f:
             for line in f:
+                flag = 1
                 if line.rstrip():
                     a += f"{line}"
                 else:
                     if not a:
-                        print(f"error:{file_name}文件为空")
-                        shutil.rmtree('~tmp')
-                        exit(0)
+                        print(f"error:{file_name} is empty.")
+                        shutil.rmtree("~tmp")
+                        sys.exit()
                     with open(f"~tmp/{i}.{file_type}", "w") as _f:
                         _f.write(a)
                     i += 1
                     a = ""
+            if not flag:
+                print(f"error:{file_name} is empty.")
+                shutil.rmtree("~tmp")
+                sys.exit()
+
         if a:
             with open(f"~tmp/{i}.{file_type}", "w") as _f:
                 _f.write(a)
         return i
 
-    def _output(self, num):
+    def _output(self, num: int, opt_file: str) -> None:
         '''
-        将分割后的文件合并输出
+        Merge and output the split files.
+
+        Args:
+        num -- The number of files to merge.
+        opt_file -- Output file name.
         '''
         a = ""
         for file_num in range(1, num+1):
             a += f"#{file_num}:\n"
             with open(f"~tmp/{file_num}.out", "r") as _f:
                 for line in _f:
                     a += f"{line}"
 
-        with open(self.args.outputfile, "w") as _out:
+        with open(opt_file, "w") as _out:
             _out.write(a)
 
-    def _check(self, opt_file, ipt_file, ans_file, file_num=0, run_file=None):
+
+class BetterRunner:
+    def __init__(self) -> None:
+        self.input_file = "in.txt"
+        self.output_file = "out.txt"
+        self.answer_file = "ans.txt"
+        self.func = Functions()
+
+    def cmd_parse(self) -> None:
+        '''Parse the command'''
+        pa = argparse.ArgumentParser()
+        pa.add_argument("filename", help="CPP file to be compiled (omitting '. cpp').")
+        pa.add_argument("-n", "--name", default="a", help="Generate executable file name (omit '. exe').")
+        pa.add_argument("-j", "--judge", action="store_true", help="Whether to evaluate.")
+        pa.add_argument("-p", "--print", action="store_true", help="Whether to print.")
+        pa.add_argument("-if", "--inputfile", default="in.txt", help="Input file name.")
+        pa.add_argument("-of", "--outputfile", default="out.txt", help="Output file name.")
+        pa.add_argument("-af", "--answerfile", default="ans.txt", help="Answer file name.")
+        pa.add_argument("-g", "--gdb", action="store_true", help="Whether to debug via gdb when the answer is incorrect.")
+        pa.add_argument("-d", "--directgdb", action="store_true", help="Directly using gdb for debugging.")
+        pa.add_argument("--onlyinput", action="store_true", help="Using file input (invalid for - j).")
+        pa.add_argument("--onlyoutput", action="store_true", help="Using file output (invalid when - j).")
+        self.args = pa.parse_args()
+        self.input_file = self.args.inputfile
+        self.output_file = self.args.outputfile
+        self.answer_file = self.args.answerfile
+        if sys.platform == "linux":
+            self.args.name = "./" + self.args.name + ".out"
+        elif sys.platform == "win32":
+            self.args.name = self.args.name + ".exe"
+
+    def compile(self) -> None:
+        '''
+        Compile files and generate executable files.
+
+        Raise：
+        SystemExit -- Compilation failed.
+        '''
+        try:
+            compile = sp.Popen(["g++", self.args.filename + ".cpp", "-g", "-o", self.args.name])
+            compile.wait()
+            if compile.returncode == 0:
+                print("Compilation successful.")
+            else:
+                print("Compilation failed.")
+                sys.exit()
+
+        # Can't sent Ctrl+c and get the messages.
+        except KeyboardInterrupt:  # pragma: no cover
+            print("\nManually exit, wish AC~(^ v ^)")
+            sys.exit()
+
+    def _check(self, opt_file: str, ipt_file: str, ans_file: str,
+               file_num: int = 0, run_file: Optional[str] = None, if_print: Optional[bool] = None) -> bool:
         '''
-        本地评测
+        Local evaluation and get results.
+
+        Args：
+        opt_file -- Output file name.
+
+        ipt_file -- Input file name.
+
+        ans_file -- Answer file name.
+
+        file_num -- File number.
+        run_file -- Executable file name (None means use the value of the command line parameter).
+        if_print -- Whether to output (None means use the value of the command line parameter).
+
+        Return：
+        if_pass -- Whether to pass the test.
         '''
 
         print(f"#{file_num}:")
 
         if run_file is None:
             run_file = self.args.name
+        if if_print is None:
+            if_print = self.args.print
 
         with open(opt_file, "w") as _out, open(ipt_file, "r") as _in:
             run = sp.Popen([run_file], stdin=_in, stdout=_out)
 
-            if not self.args.use_multiple_processes:
-                ft = time.time()
-                run.wait()
-                now = time.time() - ft
+            ft = time.time()
+            run.wait()
+            now = time.time() - ft
 
             if run.returncode != 0:
-                print(f"返回值为{run.returncode}，程序运行可能有问题")
+                print(f"The return value is {run.returncode}. There may be issues with the program running.")
 
         with open(ans_file, "r") as ans, open(opt_file, "r") as my_ans:
-            ans = [line.rstrip() for line in ans if line.rstrip()]
-            my_ans = [line.rstrip() for line in my_ans if line.rstrip()]
-            if ans == my_ans:
-                if self.args.print:
-                    # print(f"标准答案：{ans}\n实际答案：{my_ans}")
-                    print(f"答案正确，用时{now:.5}")
+            ans_list = [line.rstrip() for line in ans if line.rstrip()]
+            my_ans_list = [line.rstrip() for line in my_ans if line.rstrip()]
+            if ans_list == my_ans_list:
+                if if_print:
+                    print(f"Correct answer, takes {now:.5} seconds.")
                 else:
-                    print("答案正确")
+                    print("Correct answer.")
                 return True
             else:
-                if self.args.print:
-                    # print(f"标准答案：{ans}\n实际答案：{my_ans}")
-                    print("答案错误")
-                    print("错误数据：")
+                if if_print:
+                    if len(ans_list) < 10:
+                        print(f"Standard answer:{ans_list}\nYour answer:{my_ans_list}")
+                    else:
+                        print("The number of answer lines is too large.")
+                    print("Wrong answer.")
+                    print("Error data:")
                     with open(ipt_file, "r") as _in:
-                        for line in _in:
-                            if line.rstrip():
-                                print(line.rstrip())
+                        data_list = [line.rstrip() for line in _in if line.rstrip()]
+                        data: str = ""
+                        for data_line in data_list:
+                            data += data_line
+                            data += "\n"
+                        if len(data) < 500:
+                            print(data)
+                        else:
+                            print("The number of data words is too large.")
                 else:
-                    print("答案错误")
+                    print("Wrong answer.")
 
                 return False
 
-    def _copy_file(self, i):
-        '''
-        复制文件，为多进程评测准备
-        '''
-        for file_num in range(1, i + 1):
-            dst = os.path.join(r'~tmp/', f"{file_num}_{self.args.name}")
-            shutil.copy2(self.args.name, dst)
-
-    def _debug(self):
-        """
-        使用gdb调试
-        """
-        if self.args.gdbfile is None:
-            gdb = sp.Popen(['gdb', self.args.name])
-            gdb.wait()
-        else:
-            with open(self.args.gdbfile, "r") as f:
-                gdb = sp.Popen(['gdb', self.args.name], stdin=sp.PIPE, text=True)
-                for line in f:
-                    if line.rstrip():
-                        line = str(line.rstrip()) + "\n"
-                        # if line != "r":
-                        #     line = line + "\n"
-                        gdb.stdin.write(line)
-                        gdb.stdin.flush()
-                # print(gdb.stdout.read())
-                # gdb.stdin.close()
-
-                gdb.stdin = sys.stdin
-                gdb.wait()
-
-    def run(self):
-        """
-        程序主函数
-        """
+    def run(self) -> None:
+        '''Main function.'''
         try:
             if self.args.directgdb:
-                self._debug()
-                exit(0)
+                gdb = sp.Popen(["gdb", self.args.name])
+                gdb.wait()
+                sys.exit()
 
             if self.args.judge:
                 flag = 0
 
-                if os.path.exists('~tmp'):
-                    shutil.rmtree('~tmp')
-                self._modify_file(self.args.inputfile, "in")
-                i = self._modify_file(self.args.answerfile, "ans")
-                if self.args.use_multiple_processes:
-                    self._copy_file(i)
+                if os.path.exists("~tmp"):
+                    shutil.rmtree("~tmp")
+                self.func._modify_file(self.input_file, "in")
+                i = self.func._modify_file(self.answer_file, "ans")
 
                 for file_num in range(1, i + 1):
-
-                    if self.args.use_multiple_processes:
-                        judge = self._check(f"~tmp/{file_num}.out", f"~tmp/{file_num}.in", f"~tmp/{file_num}.ans",
-                                            file_num, f"~tmp/{file_num}_{self.args.name}")
-                    else:
-                        judge = self._check(f"~tmp/{file_num}.out", f"~tmp/{file_num}.in", f"~tmp/{file_num}.ans",
-                                            file_num)
-
+                    judge = self._check(f"~tmp/{file_num}.out", f"~tmp/{file_num}.in", f"~tmp/{file_num}.ans",
+                                        file_num)
                     if not judge:
                         flag += 1
 
-                print(f"#final:正确率{((i - flag) / i) : .2%}")
-                self._output(i)
-                shutil.rmtree('~tmp')
+                print(f"#final:Accuracy{((i - flag) / i): .2%}")
+                self.func._output(i, self.output_file)
+                shutil.rmtree("~tmp")
 
                 if self.args.gdb and flag > 0:
-                    self._debug()
+                    gdb = sp.Popen(["gdb", self.args.name])
+                    gdb.wait()
 
             else:
                 if self.args.onlyinput:
                     with open(self.input_file, "r") as _in:
-                        print("文件已执行")
+                        print("The file has been executed.")
                         run = sp.Popen([self.args.name], stdin=_in)
 
                 elif self.args.onlyoutput:
                     with open(self.output_file, "w") as _out:
                         run = sp.Popen([self.args.name], stdout=_out)
 
                 else:
                     run = sp.Popen([self.args.name])
 
                 run.wait()
                 if run.returncode != 0:
-                    print(f"返回值为{run.returncode}，程序运行可能有问题")
+                    print(f"The return value is {run.returncode}. There may be issues with the program running.")
 
-        except KeyboardInterrupt:
-            if os.path.exists('~tmp'):
-                shutil.rmtree('~tmp')
-            print("\n手动退出，祝AC~(^v^)")
+        # Can't sent Ctrl+c and get the messages.
+        except KeyboardInterrupt:  # pragma: no cover
+            if os.path.exists("~tmp"):
+                shutil.rmtree("~tmp")
+            print("\nManually exit, wish AC~(^ v ^)")
 
 
 def main():
     runner = BetterRunner()
     runner.cmd_parse()
     runner.compile()
     runner.run()
 
 
 if __name__ == "__main__":
-    main()
+    main()  # pragma: no cover
```

