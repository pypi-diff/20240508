# Comparing `tmp/git-dump-tool-0.1.0.tar.gz` & `tmp/git_dump_tool-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "git-dump-tool-0.1.0.tar", last modified: Fri Apr 12 01:10:21 2024, max compression
+gzip compressed data, was "git_dump_tool-0.1.1.tar", last modified: Wed May  8 04:25:51 2024, max compression
```

## Comparing `git-dump-tool-0.1.0.tar` & `git_dump_tool-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-12 01:10:21.137547 git-dump-tool-0.1.0/
--rw-r--r--   0 sergey    (1000) sergey    (1000)       51 2024-04-12 00:11:03.000000 git-dump-tool-0.1.0/.gitignore
--rw-r--r--   0 sergey    (1000) sergey    (1000)      165 2024-04-11 23:42:04.000000 git-dump-tool-0.1.0/LICENSE
--rw-r--r--   0 sergey    (1000) sergey    (1000)      821 2024-04-12 01:10:21.137547 git-dump-tool-0.1.0/PKG-INFO
--rw-r--r--   0 sergey    (1000) sergey    (1000)      186 2024-04-12 00:10:27.000000 git-dump-tool-0.1.0/README.md
--rw-r--r--   0 sergey    (1000) sergey    (1000)    16625 2024-04-12 00:52:28.000000 git-dump-tool-0.1.0/git_dump.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-12 01:10:21.137547 git-dump-tool-0.1.0/git_dump_tool.egg-info/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      821 2024-04-12 01:10:21.000000 git-dump-tool-0.1.0/git_dump_tool.egg-info/PKG-INFO
--rw-r--r--   0 sergey    (1000) sergey    (1000)      279 2024-04-12 01:10:21.000000 git-dump-tool-0.1.0/git_dump_tool.egg-info/SOURCES.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)        1 2024-04-12 01:10:21.000000 git-dump-tool-0.1.0/git_dump_tool.egg-info/dependency_links.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)       43 2024-04-12 01:10:21.000000 git-dump-tool-0.1.0/git_dump_tool.egg-info/entry_points.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)       44 2024-04-12 01:10:21.000000 git-dump-tool-0.1.0/git_dump_tool.egg-info/requires.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)        9 2024-04-12 01:10:21.000000 git-dump-tool-0.1.0/git_dump_tool.egg-info/top_level.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)      671 2024-04-12 01:10:14.000000 git-dump-tool-0.1.0/pyproject.toml
--rw-r--r--   0 sergey    (1000) sergey    (1000)       38 2024-04-12 01:10:21.137547 git-dump-tool-0.1.0/setup.cfg
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-05-08 04:25:51.351220 git_dump_tool-0.1.1/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       51 2024-04-12 00:11:03.000000 git_dump_tool-0.1.1/.gitignore
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      165 2024-04-11 23:42:04.000000 git_dump_tool-0.1.1/LICENSE
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      821 2024-05-08 04:25:51.347886 git_dump_tool-0.1.1/PKG-INFO
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      186 2024-04-12 00:10:27.000000 git_dump_tool-0.1.1/README.md
+-rwxr-xr-x   0 sergey    (1000) sergey    (1000)    16768 2024-05-07 04:47:39.000000 git_dump_tool-0.1.1/git_dump.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-05-08 04:25:51.347886 git_dump_tool-0.1.1/git_dump_tool.egg-info/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      821 2024-05-08 04:25:51.000000 git_dump_tool-0.1.1/git_dump_tool.egg-info/PKG-INFO
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      279 2024-05-08 04:25:51.000000 git_dump_tool-0.1.1/git_dump_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        1 2024-05-08 04:25:51.000000 git_dump_tool-0.1.1/git_dump_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       43 2024-05-08 04:25:51.000000 git_dump_tool-0.1.1/git_dump_tool.egg-info/entry_points.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       44 2024-05-08 04:25:51.000000 git_dump_tool-0.1.1/git_dump_tool.egg-info/requires.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        5 2024-05-08 04:25:51.000000 git_dump_tool-0.1.1/git_dump_tool.egg-info/top_level.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      671 2024-04-12 01:10:14.000000 git_dump_tool-0.1.1/pyproject.toml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       38 2024-05-08 04:25:51.351220 git_dump_tool-0.1.1/setup.cfg
```

### Comparing `git-dump-tool-0.1.0/PKG-INFO` & `git_dump_tool-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git-dump-tool
-Version: 0.1.0
+Version: 0.1.1
 Author: Sergey M
 License: # LICENSE
         
         Free for commercial usage. You do not have the right to use this software against residents of the Russian Federation, the Republic of Belarus and China.
         
 Project-URL: Repository, https://github.com/s3rgeym/git-dump.git
 Classifier: Topic :: Internet
```

### Comparing `git-dump-tool-0.1.0/git_dump.py` & `git_dump_tool-0.1.1/git_dump.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #!/usr/bin/env python3
 # pylint: disable=C,R,W
 """\
 null-dependency git dumper
 """
+
 import argparse
 import codecs
 import functools
 import io
 import math
 import multiprocessing
 import os
@@ -23,15 +24,15 @@
 import zlib
 from collections import namedtuple
 from multiprocessing import JoinableQueue, Manager, Process
 from urllib.error import HTTPError
 from urllib.parse import unquote, urljoin, urlsplit
 from urllib.request import HTTPHandler, HTTPSHandler, Request, build_opener
 
-__version__ = "0.1.0"
+__version__ = "0.1.1"
 __author__ = "Sergey M"
 
 GIT_DIR = "/.git/"
 GIT_COMMIT_TYPE = "commit"
 GIT_TREE_TYPE = "tree"
 
 GIT_COMMON_FILES = [
@@ -86,44 +87,51 @@
 REFERER = "https://www.google.com/"
 
 SHA1_RE = re.compile(r"\b[a-f\d]{40}\b")
 PACK_RE = re.compile(r"\bpack-" + SHA1_RE.pattern[2:-2] + r"\b")
 
 MAX_PARSE_SIZE = 1 << 27  # 128 MiB
 
-print = functools.partial(print, file=sys.stderr)
+print_stderr = functools.partial(print, file=sys.stderr)
 
 ASSET_EXTS = (
+    ".ai",
+    ".apk",
+    ".bmp",
     ".css",
-    ".html",
-    ".htm",
-    ".min.js",
     ".css",
-    ".map",
+    ".doc",
+    ".docx",
+    ".eot",
+    ".gif",
+    ".htm",
+    ".html",
+    ".ico",
     ".jpeg",
     ".jpg",
+    ".less",
+    ".map",
+    ".min.js",
+    ".mo",
+    ".mov",
+    ".mp3",
+    ".mp4",
+    ".otf",
+    ".pdf",
     ".png",
-    ".gif",
-    ".bmp",
-    ".ico",
-    ".eot",
+    ".po",
+    ".psd",
+    ".scss",
+    ".svg",
+    ".swf",
     ".ttf",
     ".ttf2",
-    ".otf",
-    ".psd",
-    ".doc",
-    ".docx",
-    ".pdf",
-    ".mp3",
-    ".mp4",
-    ".mov",
     ".webm",
-    ".ai",
-    ".swf",
-    ".apk",
+    ".woff",
+    ".woff2",
 )
 
 
 class ArgumentFormatter(
     argparse.ArgumentDefaultsHelpFormatter,
     argparse.RawDescriptionHelpFormatter,
 ):
@@ -158,17 +166,15 @@
     parser.add_argument(
         "-t",
         "--timeout",
         help="fetch timeout",
         type=float,
         default=15.0,
     )
-    parser.add_argument(
-        "-A", "--user-agent", help="user-agent", default=USER_AGENT
-    )
+    parser.add_argument("-A", "--user-agent", help="user-agent", default=USER_AGENT)
     parser.add_argument(
         "-w",
         "--workers",
         dest="num_workers",
         help="number of workers",
         type=int,
         default=max(4, multiprocessing.cpu_count() * 2 - 1),
@@ -263,17 +269,17 @@
     '1.44 M'
     >>> humansize(1234567890)
     '1.15 G'
     """
     if n == 0:
         return "0"
     exp = min(math.floor(math.log(n) / math.log(base)), len(units) - 1)
-    return "{:.2f} {}".format(
-        math.ceil(n / base**exp * 100) / 100, units[exp]
-    ).replace(".00", "")
+    return "{:.2f} {}".format(math.ceil(n / base**exp * 100) / 100, units[exp]).replace(
+        ".00", ""
+    )
 
 
 class DecodeError(Exception):
     pass
 
 
 class GitDumper(Process):
@@ -338,29 +344,25 @@
         try:
             decompressed = zlib.decompress(fp.read())
         except zlib.error as e:
             raise DecodeError() from e
         pos = decompressed.find(b"\x00")
         obj_type = decompressed[:pos].decode()
         if obj_type in [GIT_COMMIT_TYPE, GIT_TREE_TYPE]:
-            self.extract_hashes(
-                decompressed.decode(errors="ignore"), git_base_url
-            )
+            self.extract_hashes(decompressed.decode(errors="ignore"), git_base_url)
 
     def parse_git(self, temp_file, url):
         pos = url.find(GIT_DIR) + len(GIT_DIR)
         git_base_url, path = url[:pos], url[pos:]
         if path == "index":
             for entry in GitIndex(temp_file).get_entries():
                 object_url = self.get_object_url(git_base_url, entry.sha1)
 
-                print(
-                    "\033[36mFound {} => {}\033[0m".format(
-                        object_url, entry.filename
-                    )
+                print_stderr(
+                    "\033[36mFound {} => {}\033[0m".format(object_url, entry.filename)
                 )
 
                 self.queue.put(object_url)
 
                 lower_filename = entry.filename.lower()
 
                 # объектный файл может отдаваться как text/html в UTF-8, поэтому из него не получится восстановить данные
@@ -409,84 +411,78 @@
         while 42:
             try:
                 url = self.queue.get()
                 if url is None:
                     break
                 # assert GIT_DIR in url
                 if url in self.seen:
-                    # print("\033[31mSeen: {}\033[0m".format(url))
+                    # print_stderr("\033[31mSeen: {}\033[0m".format(url))
                     continue
                 # файл может долго скачиваться, поэтому все же произойдет
                 # обработка одного и того же файла разными процессами
                 self.seen[url] = 1
                 # Сохраняем все во временный файл, который будет удален в случае ошибки
                 with tempfile.NamedTemporaryFile(delete=False) as temp_file:
                     try:
                         size = self.http_download(url, temp_file)
                         if GIT_DIR in url:
                             if size <= MAX_PARSE_SIZE:
                                 try:
                                     self.parse_git(temp_file, url)
                                 except DecodeError:
-                                    print(
+                                    print_stderr(
                                         "\033[31mNon zlib-deflated data: {}\033[0m".format(
                                             url
                                         )
                                     )
                                     continue
                             else:
-                                print(
+                                print_stderr(
                                     "\033[31mWARN: Too Large to Parse ({} > {}) - {}\033[0m".format(
                                         humansize(size),
                                         humansize(MAX_PARSE_SIZE),
                                         url,
                                     )
                                 )
                         sp = urlsplit(url)
 
                         # hostname = sp.netloc.split(":")[0].strip("[]")
 
                         dest = (
-                            self.output_path
-                            / sp.netloc
-                            / unquote(sp.path.lstrip("/"))
+                            self.output_path / sp.netloc / unquote(sp.path.lstrip("/"))
                         )
 
                         try:
                             dest.parent.mkdir(parents=True)
                         except FileExistsError:
                             pass
 
                         temp_file.close()
                         # Эта функция работает только в пределах одной файловой системы, те из tmpfs
                         # файл нельзя переместить куда-то в /home
                         # os.replace(temp_file.name, str(dest))
                         shutil.move(temp_file.name, str(dest))
-                        print("\033[32mSaved: {}\033[0m".format(dest))
+                        print_stderr("\033[32mSaved: {}\033[0m".format(dest))
                     except HTTPError as ex:
-                        print(
+                        print_stderr(
                             "\033[31mError {}: {}\033[0m".format(
                                 ex.status,
                                 url,
                             )
                         )
                     except socket.timeout:
-                        print("\033[31mTimeout: {}\033[0m".format(url))
+                        print_stderr("\033[31mTimeout: {}\033[0m".format(url))
                     finally:
                         if os.path.exists(temp_file.name):
                             os.unlink(temp_file.name)
             except Exception as ex:
-                print(
+                print_stderr(
                     "\033[31mAn Unexpected Error has occurred:",
                     "",
-                    "".join(
-                        traceback.format_exception(
-                            type(ex), ex, ex.__traceback__
-                        )
-                    ),
+                    "".join(traceback.format_exception(type(ex), ex, ex.__traceback__)),
                     "\033[0m",
                     sep=os.linesep,
                 )
             finally:
                 self.queue.task_done()
 
 
@@ -494,18 +490,20 @@
     cwd = os.path.curdir
     for host in hosts:
         try:
             repo_path = output_dir / host
             if not repo_path.exists():
                 continue
             os.chdir(str(repo_path))
-            subprocess.check_call(["git", "checkout", "--", "."])
-            print("\033[32mRestored: {}\033[0m".format(repo_path))
+            # Исправил ошибку при которой удалялись выкаченные файлы
+            # shell=True полный аналон ['sh', '-c', '...']
+            subprocess.check_call("git checkout $(git ls-files -d)", shell=True)
+            print_stderr("\033[32mRestored: {}\033[0m".format(repo_path))
         except subprocess.CalledProcessError:
-            print("\033[31mCan't restore: {}\033[0m".format(repo_path))
+            print_stderr("\033[31mCan't restore: {}\033[0m".format(repo_path))
         finally:
             os.chdir(cwd)
 
 
 def main(argv=None):
     args = parse_args(argv)
 
@@ -540,17 +538,17 @@
 
     for _ in range(len(workers)):
         queue.put(None)
 
     for w in workers:
         w.join()
 
-    print("\033[33mDump tasks completed!\033[0m")
+    print_stderr("\033[33mDump tasks completed!\033[0m")
 
-    print("\033[33mGit checkout files\033[0m")
+    print_stderr("\033[33mGit checkout files\033[0m")
     hosts = set(urlsplit(u).netloc for u in seen.keys())
     git_checkout_files(hosts, args.output_dir)
-    print("\033[33mFinished!\033[0m")
+    print_stderr("\033[33mFinished!\033[0m")
 
 
 if __name__ == "__main__":
     sys.exit(main())
```

### Comparing `git-dump-tool-0.1.0/git_dump_tool.egg-info/PKG-INFO` & `git_dump_tool-0.1.1/git_dump_tool.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git-dump-tool
-Version: 0.1.0
+Version: 0.1.1
 Author: Sergey M
 License: # LICENSE
         
         Free for commercial usage. You do not have the right to use this software against residents of the Russian Federation, the Republic of Belarus and China.
         
 Project-URL: Repository, https://github.com/s3rgeym/git-dump.git
 Classifier: Topic :: Internet
```

### Comparing `git-dump-tool-0.1.0/pyproject.toml` & `git_dump_tool-0.1.1/pyproject.toml`

 * *Files identical despite different names*

