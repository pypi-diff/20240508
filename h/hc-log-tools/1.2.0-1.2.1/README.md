# Comparing `tmp/hc_log_tools-1.2.0.tar.gz` & `tmp/hc_log_tools-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hc_log_tools-1.2.0.tar", last modified: Mon Nov 14 06:13:09 2022, max compression
+gzip compressed data, was "hc_log_tools-1.2.1.tar", last modified: Wed May  8 09:27:21 2024, max compression
```

## Comparing `hc_log_tools-1.2.0.tar` & `hc_log_tools-1.2.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 shixukai   (501) staff       (20)        0 2022-11-14 06:13:09.739510 hc_log_tools-1.2.0/
--rw-r--r--   0 shixukai   (501) staff       (20)     1074 2022-10-10 07:50:12.000000 hc_log_tools-1.2.0/LICENSE
--rw-r--r--   0 shixukai   (501) staff       (20)       24 2022-10-10 12:18:04.000000 hc_log_tools-1.2.0/MANIFEST.in
--rw-r--r--   0 shixukai   (501) staff       (20)     1489 2022-11-14 06:13:09.739397 hc_log_tools-1.2.0/PKG-INFO
--rw-r--r--   0 shixukai   (501) staff       (20)     1272 2022-11-07 06:45:00.000000 hc_log_tools-1.2.0/README.md
-drwxr-xr-x   0 shixukai   (501) staff       (20)        0 2022-11-14 06:13:09.737055 hc_log_tools-1.2.0/hc_log_tools.egg-info/
--rw-r--r--   0 shixukai   (501) staff       (20)     1489 2022-11-14 06:13:09.000000 hc_log_tools-1.2.0/hc_log_tools.egg-info/PKG-INFO
--rw-r--r--   0 shixukai   (501) staff       (20)      550 2022-11-14 06:13:09.000000 hc_log_tools-1.2.0/hc_log_tools.egg-info/SOURCES.txt
--rw-r--r--   0 shixukai   (501) staff       (20)        1 2022-11-14 06:13:09.000000 hc_log_tools-1.2.0/hc_log_tools.egg-info/dependency_links.txt
--rw-r--r--   0 shixukai   (501) staff       (20)       49 2022-11-14 06:13:09.000000 hc_log_tools-1.2.0/hc_log_tools.egg-info/entry_points.txt
--rw-r--r--   0 shixukai   (501) staff       (20)       94 2022-11-14 06:13:09.000000 hc_log_tools-1.2.0/hc_log_tools.egg-info/requires.txt
--rw-r--r--   0 shixukai   (501) staff       (20)        9 2022-11-14 06:13:09.000000 hc_log_tools-1.2.0/hc_log_tools.egg-info/top_level.txt
--rw-r--r--   0 shixukai   (501) staff       (20)      365 2022-11-14 06:13:05.000000 hc_log_tools-1.2.0/pyproject.toml
--rw-r--r--   0 shixukai   (501) staff       (20)       94 2022-11-14 06:13:04.000000 hc_log_tools-1.2.0/requirements.txt
--rw-r--r--   0 shixukai   (501) staff       (20)       38 2022-11-14 06:13:09.739540 hc_log_tools-1.2.0/setup.cfg
--rw-r--r--   0 shixukai   (501) staff       (20)      749 2022-10-10 13:43:34.000000 hc_log_tools-1.2.0/setup.py
-drwxr-xr-x   0 shixukai   (501) staff       (20)        0 2022-11-14 06:13:09.738291 hc_log_tools-1.2.0/src/
--rw-r--r--   0 shixukai   (501) staff       (20)        0 2022-09-08 04:00:01.000000 hc_log_tools-1.2.0/src/__init__.py
--rw-r--r--   0 shixukai   (501) staff       (20)     1144 2022-10-10 09:55:42.000000 hc_log_tools-1.2.0/src/entry.py
--rw-r--r--   0 shixukai   (501) staff       (20)    16566 2022-11-14 06:01:49.000000 hc_log_tools-1.2.0/src/log_utility.py
--rw-r--r--   0 shixukai   (501) staff       (20)     4793 2022-11-11 09:42:45.000000 hc_log_tools-1.2.0/src/pack_log.py
--rw-r--r--   0 shixukai   (501) staff       (20)     3986 2022-10-12 03:57:20.000000 hc_log_tools-1.2.0/src/v_t_chart.py
-drwxr-xr-x   0 shixukai   (501) staff       (20)        0 2022-11-14 06:13:09.739221 hc_log_tools-1.2.0/test/
--rw-r--r--   0 shixukai   (501) staff       (20)        0 2022-09-08 08:42:23.000000 hc_log_tools-1.2.0/test/__init__.py
--rw-r--r--   0 shixukai   (501) staff       (20)     3537 2022-09-15 06:48:27.000000 hc_log_tools-1.2.0/test/test_log_download.py
--rw-r--r--   0 shixukai   (501) staff       (20)     1093 2022-09-09 03:40:09.000000 hc_log_tools-1.2.0/test/test_log_file_name_match.py
--rw-r--r--   0 shixukai   (501) staff       (20)     1946 2022-10-24 06:06:49.000000 hc_log_tools-1.2.0/test/test_log_utility.py
--rw-r--r--   0 shixukai   (501) staff       (20)      595 2022-09-15 06:38:26.000000 hc_log_tools-1.2.0/test/test_read_pick_data.py
--rw-r--r--   0 shixukai   (501) staff       (20)     2601 2022-09-15 06:47:28.000000 hc_log_tools-1.2.0/test/test_read_sort_data.py
--rw-r--r--   0 shixukai   (501) staff       (20)     3784 2022-10-20 03:57:29.000000 hc_log_tools-1.2.0/test/test_tiem_range.py
+drwxr-xr-x   0 shixukai   (501) staff       (20)        0 2024-05-08 09:27:21.402740 hc_log_tools-1.2.1/
+-rw-r--r--   0 shixukai   (501) staff       (20)     1074 2024-04-19 01:19:58.000000 hc_log_tools-1.2.1/LICENSE
+-rw-r--r--   0 shixukai   (501) staff       (20)       24 2024-04-19 01:19:58.000000 hc_log_tools-1.2.1/MANIFEST.in
+-rw-r--r--   0 shixukai   (501) staff       (20)     1658 2024-05-08 09:27:21.402540 hc_log_tools-1.2.1/PKG-INFO
+-rw-r--r--   0 shixukai   (501) staff       (20)     1272 2024-04-19 01:19:58.000000 hc_log_tools-1.2.1/README.md
+drwxr-xr-x   0 shixukai   (501) staff       (20)        0 2024-05-08 09:27:21.402315 hc_log_tools-1.2.1/hc_log_tools.egg-info/
+-rw-r--r--   0 shixukai   (501) staff       (20)     1658 2024-05-08 09:27:21.000000 hc_log_tools-1.2.1/hc_log_tools.egg-info/PKG-INFO
+-rw-r--r--   0 shixukai   (501) staff       (20)      525 2024-05-08 09:27:21.000000 hc_log_tools-1.2.1/hc_log_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 shixukai   (501) staff       (20)        1 2024-05-08 09:27:21.000000 hc_log_tools-1.2.1/hc_log_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 shixukai   (501) staff       (20)       94 2024-05-08 09:27:21.000000 hc_log_tools-1.2.1/hc_log_tools.egg-info/requires.txt
+-rw-r--r--   0 shixukai   (501) staff       (20)        9 2024-05-08 09:27:21.000000 hc_log_tools-1.2.1/hc_log_tools.egg-info/top_level.txt
+-rw-r--r--   0 shixukai   (501) staff       (20)      365 2024-05-08 09:27:18.000000 hc_log_tools-1.2.1/pyproject.toml
+-rw-r--r--   0 shixukai   (501) staff       (20)       94 2024-04-19 01:19:58.000000 hc_log_tools-1.2.1/requirements.txt
+-rw-r--r--   0 shixukai   (501) staff       (20)       38 2024-05-08 09:27:21.402786 hc_log_tools-1.2.1/setup.cfg
+-rw-r--r--   0 shixukai   (501) staff       (20)      719 2024-05-08 09:24:58.000000 hc_log_tools-1.2.1/setup.py
+drwxr-xr-x   0 shixukai   (501) staff       (20)        0 2024-05-08 09:27:21.401164 hc_log_tools-1.2.1/src/
+-rw-r--r--   0 shixukai   (501) staff       (20)        0 2024-04-19 01:19:58.000000 hc_log_tools-1.2.1/src/__init__.py
+-rw-r--r--   0 shixukai   (501) staff       (20)     1283 2024-05-08 09:24:58.000000 hc_log_tools-1.2.1/src/entry.py
+-rw-r--r--   0 shixukai   (501) staff       (20)    18729 2024-05-08 09:24:58.000000 hc_log_tools-1.2.1/src/log_utility.py
+-rw-r--r--   0 shixukai   (501) staff       (20)     5306 2024-05-08 09:24:58.000000 hc_log_tools-1.2.1/src/pack_log.py
+-rw-r--r--   0 shixukai   (501) staff       (20)       39 2024-05-08 09:24:58.000000 hc_log_tools-1.2.1/src/public.py
+-rw-r--r--   0 shixukai   (501) staff       (20)     3986 2024-04-19 01:19:58.000000 hc_log_tools-1.2.1/src/v_t_chart.py
+drwxr-xr-x   0 shixukai   (501) staff       (20)        0 2024-05-08 09:27:21.402135 hc_log_tools-1.2.1/test/
+-rw-r--r--   0 shixukai   (501) staff       (20)        0 2024-04-19 01:19:58.000000 hc_log_tools-1.2.1/test/__init__.py
+-rw-r--r--   0 shixukai   (501) staff       (20)     3537 2024-04-19 01:19:58.000000 hc_log_tools-1.2.1/test/test_log_download.py
+-rw-r--r--   0 shixukai   (501) staff       (20)     1093 2024-04-19 01:19:58.000000 hc_log_tools-1.2.1/test/test_log_file_name_match.py
+-rw-r--r--   0 shixukai   (501) staff       (20)     1946 2024-04-19 01:19:58.000000 hc_log_tools-1.2.1/test/test_log_utility.py
+-rw-r--r--   0 shixukai   (501) staff       (20)      595 2024-04-19 01:19:58.000000 hc_log_tools-1.2.1/test/test_read_pick_data.py
+-rw-r--r--   0 shixukai   (501) staff       (20)     2601 2024-04-19 01:19:58.000000 hc_log_tools-1.2.1/test/test_read_sort_data.py
+-rw-r--r--   0 shixukai   (501) staff       (20)     3784 2024-04-19 01:19:58.000000 hc_log_tools-1.2.1/test/test_tiem_range.py
```

### Comparing `hc_log_tools-1.2.0/LICENSE` & `hc_log_tools-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hc_log_tools-1.2.0/PKG-INFO` & `hc_log_tools-1.2.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,7 @@
-Metadata-Version: 2.1
-Name: hc_log_tools
-Version: 1.2.0
-Author-email: "xukai.sh" <shixukai@163.com>, "xukai.sh" <shixukai@163.com>
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 
 
 ## 使用说明
 https://hcrobots.feishu.cn/docx/doxcnCw5mIUCbo1CGDgt8j026Je
 
 ## generate or update requirements.txt
 ```
```

### Comparing `hc_log_tools-1.2.0/hc_log_tools.egg-info/PKG-INFO` & `hc_log_tools-1.2.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 Metadata-Version: 2.1
-Name: hc-log-tools
-Version: 1.2.0
+Name: hc_log_tools
+Version: 1.2.1
 Author-email: "xukai.sh" <shixukai@163.com>, "xukai.sh" <shixukai@163.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: alive_progress==2.4.1
+Requires-Dist: matplotlib==3.5.3
+Requires-Dist: pip>=20.0.2
+Requires-Dist: python_dateutil==2.8.2
+Requires-Dist: setuptools==63.4.3
 
 
 
 ## 使用说明
 https://hcrobots.feishu.cn/docx/doxcnCw5mIUCbo1CGDgt8j026Je
 
 ## generate or update requirements.txt
```

### Comparing `hc_log_tools-1.2.0/hc_log_tools.egg-info/SOURCES.txt` & `hc_log_tools-1.2.1/hc_log_tools.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 README.md
 pyproject.toml
 requirements.txt
 setup.py
 hc_log_tools.egg-info/PKG-INFO
 hc_log_tools.egg-info/SOURCES.txt
 hc_log_tools.egg-info/dependency_links.txt
-hc_log_tools.egg-info/entry_points.txt
 hc_log_tools.egg-info/requires.txt
 hc_log_tools.egg-info/top_level.txt
 src/__init__.py
 src/entry.py
 src/log_utility.py
 src/pack_log.py
+src/public.py
 src/v_t_chart.py
 test/__init__.py
 test/test_log_download.py
 test/test_log_file_name_match.py
 test/test_log_utility.py
 test/test_read_pick_data.py
 test/test_read_sort_data.py
```

### Comparing `hc_log_tools-1.2.0/src/entry.py` & `hc_log_tools-1.2.1/src/entry.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 import src.pack_log
 import src.v_t_chart
 import argparse
 import fcntl
 import sys
-
 def entry():
     # only can run one process at a time
     lock_file = open("/tmp/log-tool-lock", "w")
     try:
         fcntl.flock(lock_file, fcntl.LOCK_EX | fcntl.LOCK_NB)
     except IOError:
         print("another process is running, exit")
         sys.exit(-1)
 
-
     parser = argparse.ArgumentParser(formatter_class=argparse.ArgumentDefaultsHelpFormatter)
     parser.set_defaults(func=lambda args: parser.print_help())
 
     subparsers = parser.add_subparsers(title='subcommands', dest='command', help='sub-command help')
 
     subparsers_pack = subparsers.add_parser("pack", help='pack help')
     src.pack_log.init_input_args(subparsers_pack)
@@ -27,10 +25,16 @@
     src.v_t_chart.init_input_args(subparsers_chart)
     subparsers_chart.set_defaults(func=src.v_t_chart.generate_chart)
 
     # parse the args and call whatever function was selected
     args = parser.parse_args()
     args.func(args)
 
+    # pack_log(args)
+
+    # if args.up_to_cloud:
+    #     pass
+    # else:
+    #     print(f'output_file_path: {Public.output_file_path}')
 
 if __name__=="__main__":
-    sys.exit(entry())
+    sys.exit(entry())
```

### Comparing `hc_log_tools-1.2.0/src/log_utility.py` & `hc_log_tools-1.2.1/src/log_utility.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 from datetime import datetime, timedelta
 from sqlite3 import Timestamp
 from dateutil.parser import parse
 import gzip
 import json
 import os
 from os import SEEK_END
@@ -83,16 +82,21 @@
             #2022-09-14T19:00:02.778000+
             log_start_timestamp_string = find_datetime_in_line(first_line)
             log_end_timestamp_string = find_datetime_in_line(last_line)
         except Exception:
             return False
 
     try:
-        log_start_timestamp = parse(log_start_timestamp_string).timestamp()
-        log_end_timestamp = parse(log_end_timestamp_string).timestamp()
+        # if log_start_timestamp_string match like 2024-04-08 17:36:40:705
+        if re.match(r"\d{4}-\d{2}-\d{2} \d{2}:\d{2}:\d{2}:\d{3}", log_start_timestamp_string) is not None:
+            log_start_timestamp = custom_parse(log_start_timestamp_string)
+            log_end_timestamp = custom_parse(log_end_timestamp_string)
+        else:
+            log_start_timestamp = parse(log_start_timestamp_string).timestamp()
+            log_end_timestamp = parse(log_end_timestamp_string).timestamp()
 
         # print(f"{log_start_timestamp} --- {log_start_timestamp}")
 
         time_range_start_timestamp = (date_selected - timedelta(minutes=delta_mins)).timestamp()
         time_range_end_timestamp = (date_selected + timedelta(minutes=delta_mins)).timestamp()
 
         if time_range_start_timestamp > log_end_timestamp:
@@ -102,28 +106,39 @@
             return False
 
         return True
     except Exception:
         return False
 
 
+def custom_parse(time_str):
+    # match like 2024-04-08 17:36:40:705
+    if re.match(r"\d{4}-\d{2}-\d{2} \d{2}:\d{2}:\d{2}:\d{3}", time_str) is  None:
+        raise Exception
+
+    last_colon = time_str.rfind(':')
+    time_str = time_str[:last_colon] + '.' + time_str[last_colon+1:]
+    return parse(time_str).timestamp()
+
+
 def find_datetime_in_line(line):
     """匹配log文件一行中的时间戳
 
     Args:
         line (string): log文件中的一行
 
     Returns:
         string: 时间戳的字符串格式
     """
     # datetime like: 2022-11-07T08:48:24.269000+0800, 2022-11-14 11:27:34.772000+0800
 
     datetime_patterns = [
         re.compile(r"(\d{4}-\d{2}-\d{2}T\d{2}:\d{2}:\d{2}\.\d{6})"),
         re.compile(r"(\d{4}-\d{2}-\d{2}\s\d{2}:\d{2}:\d{2}\.\d{6})"),
+        re.compile(r"(\d{4}-\d{2}-\d{2} \d{2}:\d{2}:\d{2}:\d{3})"),
     ]
 
     for timestamp_pattern in datetime_patterns:
         try:
             m = re.search(timestamp_pattern, line)
             return m[0]
         except Exception:
@@ -213,15 +228,15 @@
 def get_file_in_time_range(input_args, **kwargs):
     """_summary_
 
     Args:
         input_args (_type_): _description_
 
     Raises:
-        RuntimeError:  输入错误的参数，kwargs['download_log']不为True的情况下，input_args的值不为"sort"或"pick"
+        RuntimeError:  输入错误的参数，kwargs['download_log']不为True的情况下，input_args的值不为"sort"或"pick"或"embedded"
 
     Returns:
         _type_: _description_
     """
 
     # if input_args.log_root_dir is None or empty, raise error
     if not input_args.log_root_dir:
@@ -236,15 +251,17 @@
 
     if input_args.prd_type == "sort":
         return get_file_in_time_range_sort(input_args.robot_id, input_args.log_root_dir, input_args.time_range, parse(input_args.timestamp))
 
     if input_args.prd_type == "pick":
         return get_file_in_time_range_pick(input_args.robot_id, input_args.log_root_dir, input_args.time_range, parse(input_args.timestamp))
 
-    raise RuntimeError("prd_type 参数错误， 不是sort或pick")
+    if input_args.prd_type == "embedded":
+        return get_file_in_time_range_embedded(input_args.robot_id, input_args.log_root_dir, input_args.time_range, parse(input_args.timestamp))
+    raise RuntimeError("prd_type 参数错误， 不是sort或pick或embedded")
 
 
 def get_file_in_time_range_sort(robot_id,  log_root_folder, time_range_in_mins=10, date_selected=datetime.now()):
     """ 遍历所有文件并保存所有日志文件
 
     Args:
         robot_id (string): 机器人编号
@@ -293,38 +310,47 @@
         for file_name in files:
             res = pick_load_file_match_res(file_name)
             log_file_full_path = os.path.abspath(os.path.join(root, file_name))
 
             if bool(res) and bool(re.search(rf"{robot_id}$", root)) and is_file_in_time_range(log_file_full_path, time_range_in_mins, date_selected):
                 yield log_file_full_path
 
+def get_file_in_time_range_embedded(robot_id, log_root_folder, time_range_in_mins, date_selected, custom_log_dir):
+    # 遍历用户指定的目录并保存所有符合时间范围的日志文件
+    for root, dirs, files in os.walk(custom_log_dir):
+        for file_name in files:
+            log_file_full_path = os.path.abspath(os.path.join(root, file_name))
+            if is_file_in_time_range(log_file_full_path, time_range_in_mins, date_selected):
+                yield log_file_full_path
+
+
 
 def get_file_in_time_range_for_download(log_root_folder, time_range_in_mins=10, date_selected=datetime.now(), **kwargs):
     """ 遍历所有文件并保存所有日志文件名,日志下载用
 
     Args:
         log_root_folder (string): 日志文件根目录
         time_range_in_mins (int, optional): 基于选取日志的时间，确定选取日志范围的时间窗口
         date_selected (datetime, optional): 选取日志的时间
 
     Yields:
         generator(string): 目标文件路径的生成器
     """
     if 'recursive' in kwargs and not kwargs['recursive']:
-        for file in os.listdir(log_root_folder):
+        for file in os.listdir(log_root_folder,followlinks=True):
             log_file_full_path = os.path.abspath(os.path.join(log_root_folder, file))
 
             if os.path.isdir(log_file_full_path):
                 continue
 
             if is_file_in_time_range(log_file_full_path, time_range_in_mins, date_selected):
                 yield log_file_full_path
 
     if 'recursive' not in kwargs or ('recursive' in kwargs and kwargs['recursive']):
-        for root, dirs, files in os.walk(log_root_folder):
+        for root, dirs, files in os.walk(log_root_folder,followlinks=True):
             for file_name in files:
                 log_file_full_path = os.path.abspath(os.path.join(root, file_name))
 
                 if is_file_in_time_range(log_file_full_path, time_range_in_mins, date_selected):
                     yield log_file_full_path
 
 
@@ -454,38 +480,54 @@
 
 
 
     except Exception as error:
         print(error)
 
 
-def upload_to_obs(upload_file):
-    # check if {User}/obsutil/push.sh exists
-    try:
-        # ask if want to upload to obs
-        # print beautiful box around the tip in terminal
+# def upload_to_obs(upload_file):
+#     # check if {User}/obsutil/push.sh exists
+#     try:
+#         # ask if want to upload to obs
+#         # print beautiful box around the tip in terminal
+
+#         # the box length should auto adjust to the length of the tip
+
+
+#         print("""
+#         \033[1;31m
+#         +-------------------------------------------------+
+#             是否要将打包的日志文件上传到云盘？ (y/n) .
+#         +-------------------------------------------------+
+#         \033[0m
+#         """.format(upload_file=upload_file))
+
+#         print(f"是否要将 {upload_file} 上传到云盘? (y/n)")
+#         if input() == 'y':
+#             obsutil_push_script_path = os.path.join(os.path.expanduser('~'), 'obsutil', 'push.sh')
+
+#             if not os.path.exists(obsutil_push_script_path):
+#                 print(f"{obsutil_push_script_path} 不存在, 请联系管理员安装")
+#                 return
+#             # run {User}/obsutil/push.sh upload_file
+#             os.system(f"{obsutil_push_script_path} {upload_file}")
+#         else:
+#             print(f"已选择跳过上传 {upload_file} 到云盘")
 
-        # the box length should auto adjust to the length of the tip
+#     except Exception as error:
+#         print(f"Error: {error}")
 
 
-        print("""
-        \033[1;31m
-        +-------------------------------------------------+
-            是否要将打包的日志文件上传到云盘？ (y/n) .
-        +-------------------------------------------------+
-        \033[0m
-        """.format(upload_file=upload_file))
-
-        print(f"是否要将 {upload_file} 上传到云盘? (y/n)")
-        if input() == 'y':
-            obsutil_push_script_path = os.path.join(os.path.expanduser('~'), 'obsutil', 'push.sh')
-
-            if not os.path.exists(obsutil_push_script_path):
-                print(f"{obsutil_push_script_path} 不存在, 请联系管理员安装")
-                return
-            # run {User}/obsutil/push.sh upload_file
+def upload_to_obs(upload_file):
+    try:
+        # 检查上传脚本是否存在
+        obsutil_push_script_path = os.path.join(os.path.expanduser('~'), 'obsutil', 'push.sh')
+        if os.path.exists(obsutil_push_script_path):
+            print(f"正在上传 {upload_file} 到云盘...")
+            # 执行上传脚本
             os.system(f"{obsutil_push_script_path} {upload_file}")
+            print("上传完成。")
         else:
-            print(f"已选择跳过上传 {upload_file} 到云盘")
+            print(f"错误：上传脚本 {obsutil_push_script_path} 不存在，请联系管理员安装。")
 
     except Exception as error:
-        print(f"Error: {error}")
+        print(f"发生错误：{error}")
```

### Comparing `hc_log_tools-1.2.0/src/pack_log.py` & `hc_log_tools-1.2.1/src/pack_log.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """This is the description.
 
   example: src/pack_log.py --prd_type=sort --time_range=100  --timestamp="2022-09-13 17:55:00" --log_root_dir=/tmp/66log
 """
 from src.log_utility import *
+from src.public import Public
 import argparse
 import tarfile
 import os
 from datetime import datetime
 from alive_progress import alive_bar
 
 
@@ -35,15 +36,21 @@
 
     sub_parser.add_argument(
         "--output_directory",
         help="输出文件的目录, 默认路径：/tmp/log_trans/",
         default="/tmp/log_trans/",
         required=False
     )
+    sub_parser.add_argument(
+        "--not-up-to-cloud", 
+        action='store_true', 
+        help="Automatically upload the compressed log files to the cloud.",
+        required=False
 
+    )
     # DON'T want to allow --feature and --no-feature at the same time
     feature_recursive_parser = sub_parser.add_mutually_exclusive_group(required=False)
     feature_recursive_parser.add_argument('--recursive', dest='recursive', action='store_true', help='递归处理log文件目录的子目录, 默认激活该选项')
     feature_recursive_parser.add_argument('--no-recursive', dest='recursive', action='store_false', help='不处理log文件目录的子目录')
     sub_parser.set_defaults(recursive=True)
 
     feature_compress_parser = sub_parser.add_mutually_exclusive_group(required=False)
@@ -60,15 +67,14 @@
 
 
 def pack_log(input_args):
     """找到指定的log，并打包
     Args:
         input_args: shell 传入的参数
     """
-
     preprocessing_output_directory(input_args.output_directory)
 
     print(f"input_args.recursive: {input_args.recursive}")
     log_files = set(
         get_file_in_time_range(
             input_args, download_log=True, recursive=input_args.recursive
         )
@@ -85,14 +91,15 @@
     # get current datetime like 20210913175500
     cur_datetime = datetime.now().strftime("%Y%m%d%H%M%S")
     # get system hostname
     hostname = os.popen("hostname").read().strip()
     output_file_name = f"{hostname}-{cur_datetime}.log.tar.gz"
     # join args.output_directory and OUTPUT_FILE_NAME
     output_file_path = os.path.join(input_args.output_directory, output_file_name)
+    Public.output_file_path = output_file_path
 
 
     # if input_args.compress, tar with gzip
     if input_args.compress:
         with alive_bar(len(log_files),  title='pack with compress') as bar:
             with tarfile.open(output_file_path, "w:gz") as tar:
                 for log_file in log_files:
@@ -112,16 +119,22 @@
                         bar()
                     except FileNotFoundError:
                         print(f"file {log_file} is not exist")
 
     # terminal process bar for compress with alive-progress
     # show the output file size with MB, precision=2
     print(f"compress finished, output file: {output_file_path}, size: {os.path.getsize(output_file_path) / 1024 / 1024:.2f} MB")
+    if input_args.not_up_to_cloud:  # 判断是否设置了 --up-to-cloud 参数
+        print(f'output_file_path: {Public.output_file_path}') #判断选项是否包含--up-to-cloud，没有则抛出错误及打印压缩文件路径和文件名称
+
+    else:
+        upload_to_obs(output_file_path)
+
+
 
-    upload_to_obs(output_file_path)
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser(
         description=__doc__, formatter_class=argparse.RawDescriptionHelpFormatter
     )
     input_args = init_input_args_warp(parser)
-    pack_log(input_args)
+
```

### Comparing `hc_log_tools-1.2.0/src/v_t_chart.py` & `hc_log_tools-1.2.1/src/v_t_chart.py`

 * *Files identical despite different names*

### Comparing `hc_log_tools-1.2.0/test/test_log_download.py` & `hc_log_tools-1.2.1/test/test_log_download.py`

 * *Files identical despite different names*

### Comparing `hc_log_tools-1.2.0/test/test_log_file_name_match.py` & `hc_log_tools-1.2.1/test/test_log_file_name_match.py`

 * *Files identical despite different names*

### Comparing `hc_log_tools-1.2.0/test/test_log_utility.py` & `hc_log_tools-1.2.1/test/test_log_utility.py`

 * *Files identical despite different names*

### Comparing `hc_log_tools-1.2.0/test/test_read_pick_data.py` & `hc_log_tools-1.2.1/test/test_read_pick_data.py`

 * *Files identical despite different names*

### Comparing `hc_log_tools-1.2.0/test/test_read_sort_data.py` & `hc_log_tools-1.2.1/test/test_read_sort_data.py`

 * *Files identical despite different names*

### Comparing `hc_log_tools-1.2.0/test/test_tiem_range.py` & `hc_log_tools-1.2.1/test/test_tiem_range.py`

 * *Files identical despite different names*

