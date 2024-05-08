# Comparing `tmp/MeMeST-2024.5.419269-py3-none-any.whl.zip` & `tmp/MeMeST-2024.5.591143-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 33846 bytes, number of entries: 16
--rwxrwxr-x  2.0 unx    35149 b- defN 24-Apr-10 04:45 MeMeST-2024.5.419269.data/data/LICENSE
+Zip file size: 34048 bytes, number of entries: 16
+-rwxrwxr-x  2.0 unx    35149 b- defN 24-Apr-10 04:45 MeMeST-2024.5.591143.data/data/LICENSE
 -rw-rw-r--  2.0 unx       76 b- defN 24-Apr-10 04:45 git_tools/__init__.py
 -rw-rw-r--  2.0 unx     1139 b- defN 24-Apr-18 09:30 git_tools/base_dtypes.py
 -rw-rw-r--  2.0 unx     9287 b- defN 24-May-05 13:38 git_tools/git_api.py
 -rw-rw-r--  2.0 unx      143 b- defN 24-Apr-10 04:45 git_tools/rep_task.py
 -rw-rw-r--  2.0 unx        0 b- defN 24-Apr-10 04:45 mest/__init__.py
 -rw-rw-r--  2.0 unx     4518 b- defN 24-Apr-29 10:15 mest/config.py
--rw-rw-r--  2.0 unx     3405 b- defN 24-May-05 13:37 mest/main.py
+-rw-rw-r--  2.0 unx     4135 b- defN 24-May-08 09:06 mest/main.py
 -rw-rw-r--  2.0 unx     2717 b- defN 24-Apr-29 13:50 mest/rep_mana.py
 -rw-rw-r--  2.0 unx      569 b- defN 24-Apr-10 04:45 mest/test_git.py
--rwxrwxr-x  2.0 unx    35149 b- defN 24-May-05 13:39 MeMeST-2024.5.419269.dist-info/LICENSE
--rw-rw-r--  2.0 unx     1797 b- defN 24-May-05 13:39 MeMeST-2024.5.419269.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-May-05 13:39 MeMeST-2024.5.419269.dist-info/WHEEL
--rw-rw-r--  2.0 unx       42 b- defN 24-May-05 13:39 MeMeST-2024.5.419269.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx       15 b- defN 24-May-05 13:39 MeMeST-2024.5.419269.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1286 b- defN 24-May-05 13:39 MeMeST-2024.5.419269.dist-info/RECORD
-16 files, 95384 bytes uncompressed, 31730 bytes compressed:  66.7%
+-rwxrwxr-x  2.0 unx    35149 b- defN 24-May-08 09:07 MeMeST-2024.5.591143.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     1797 b- defN 24-May-08 09:07 MeMeST-2024.5.591143.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-May-08 09:07 MeMeST-2024.5.591143.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       42 b- defN 24-May-08 09:07 MeMeST-2024.5.591143.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx       15 b- defN 24-May-08 09:07 MeMeST-2024.5.591143.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1286 b- defN 24-May-08 09:07 MeMeST-2024.5.591143.dist-info/RECORD
+16 files, 96114 bytes uncompressed, 31932 bytes compressed:  66.8%
```

## zipnote {}

```diff
@@ -1,8 +1,8 @@
-Filename: MeMeST-2024.5.419269.data/data/LICENSE
+Filename: MeMeST-2024.5.591143.data/data/LICENSE
 Comment: 
 
 Filename: git_tools/__init__.py
 Comment: 
 
 Filename: git_tools/base_dtypes.py
 Comment: 
@@ -24,26 +24,26 @@
 
 Filename: mest/rep_mana.py
 Comment: 
 
 Filename: mest/test_git.py
 Comment: 
 
-Filename: MeMeST-2024.5.419269.dist-info/LICENSE
+Filename: MeMeST-2024.5.591143.dist-info/LICENSE
 Comment: 
 
-Filename: MeMeST-2024.5.419269.dist-info/METADATA
+Filename: MeMeST-2024.5.591143.dist-info/METADATA
 Comment: 
 
-Filename: MeMeST-2024.5.419269.dist-info/WHEEL
+Filename: MeMeST-2024.5.591143.dist-info/WHEEL
 Comment: 
 
-Filename: MeMeST-2024.5.419269.dist-info/entry_points.txt
+Filename: MeMeST-2024.5.591143.dist-info/entry_points.txt
 Comment: 
 
-Filename: MeMeST-2024.5.419269.dist-info/top_level.txt
+Filename: MeMeST-2024.5.591143.dist-info/top_level.txt
 Comment: 
 
-Filename: MeMeST-2024.5.419269.dist-info/RECORD
+Filename: MeMeST-2024.5.591143.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mest/main.py

```diff
@@ -25,14 +25,29 @@
 USAGE = """ USAGE memest [cmd]
 cmd: start, status, stop, restart
 """
 
 CONFIG_FILE = os.path.expanduser("~/.config/memest/config.ini")
 
 
+def add_cron_job_if_not_exists(cron_command, schedule):
+    tmp_crontab_file = "tmp_my_crontab"
+    subprocess.run(["crontab", "-l"], stdout=open(tmp_crontab_file, "w"), check=True)
+    all_tasks = open(tmp_crontab_file, "r").read()
+    cmd = f"{schedule} {cron_command}"
+    if cmd in all_tasks:
+        subprocess.run(["rm", "-f", tmp_crontab_file], check=False)
+        return
+
+    with open(tmp_crontab_file, "a") as file:
+        file.write(f"{schedule} {cron_command}\n")
+    subprocess.run(["crontab", tmp_crontab_file], check=False)
+    subprocess.run(["rm", "-f", tmp_crontab_file], check=False)
+
+
 def get_log_error():
     error_lines = []
     for line in open(LOG_FILE, "r").read().splitlines():
         if "ERROR" in line:
             error_lines.append(line)
     content = "\n".join(error_lines[-10:])
     return content
@@ -111,14 +126,16 @@
     if len(sys.argv) < 2:
         print(USAGE)
         exit(1)
     cmd = sys.argv[1]
     os.system("mkdir -p ~/.cache/")
     init_check()
     if cmd == "start":
+        add_cron_job_if_not_exists("memest start", "@reboot")
+        add_cron_job_if_not_exists("memest start", "@daily")
         if is_memest_daemon_running():
             print("memest is running")
         else:
             print("start memest")
             os.system("nohup memest --daemon >> /dev/null 2>&1 &")
     elif cmd == "status":
         show_status()
```

## Comparing `MeMeST-2024.5.419269.data/data/LICENSE` & `MeMeST-2024.5.591143.data/data/LICENSE`

 * *Files identical despite different names*

## Comparing `MeMeST-2024.5.419269.dist-info/LICENSE` & `MeMeST-2024.5.591143.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `MeMeST-2024.5.419269.dist-info/METADATA` & `MeMeST-2024.5.591143.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MeMeST
-Version: 2024.5.419269
+Version: 2024.5.591143
 Summary: Multi-Repository Sync Tool
 Author: Xin-Xin Ma
 License: GPL
 Project-URL: Source, https://github.com/xxmawhu/memest.git
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: termcolor
```

## Comparing `MeMeST-2024.5.419269.dist-info/RECORD` & `MeMeST-2024.5.591143.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-MeMeST-2024.5.419269.data/data/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
+MeMeST-2024.5.591143.data/data/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
 git_tools/__init__.py,sha256=-M_wTgmk-Pe-gzayRUsldMI8maSAQpgrCrKbiUQFV2o,76
 git_tools/base_dtypes.py,sha256=Y7F6fUoZvETZVV4EKpPnrfS3Qfeudb-Oojh-B93mSPQ,1139
 git_tools/git_api.py,sha256=D9w3gaNY04_Nf7KBBiFgjsVlxRO2SEbTnjSAkjZBUq4,9287
 git_tools/rep_task.py,sha256=vFPW1Z8mTIF0ZGJgaGF8AZM91A4Ogf_Sdo-bKtdo8-c,143
 mest/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mest/config.py,sha256=YS4NJNE1fIAz0K3l7SreoqdtpM3nAJCe_oJc4LwREo0,4518
-mest/main.py,sha256=FKTsqOmePiQK80kg0WU95d21fJ7U4AX8M0viQW5e5a8,3405
+mest/main.py,sha256=WLrMP2GO4yyCJB0OutmquQA1_A2IrP5xZ1k07JnleBk,4135
 mest/rep_mana.py,sha256=ZEhbeopuFBYIr4Eg64GUEQQ7M9bZZn0IFhmf3HJ2Mso,2717
 mest/test_git.py,sha256=BgD4moVzqnxfnhZzoM-EgHklAVFYPbtYu5Ke6qqFHhI,569
-MeMeST-2024.5.419269.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
-MeMeST-2024.5.419269.dist-info/METADATA,sha256=S1IYpOdkYXjQMKKnlCBswrn5bT9XeT2dThPXlXqJZrM,1797
-MeMeST-2024.5.419269.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-MeMeST-2024.5.419269.dist-info/entry_points.txt,sha256=OYg2gMfzGJOXcQc_TTGdfCSPRPqlQylNW3LSReX_ta8,42
-MeMeST-2024.5.419269.dist-info/top_level.txt,sha256=iFxJRSyvq4K2f9Wl2wqP84mPUD7Ta4IoyDy9bDHkiYE,15
-MeMeST-2024.5.419269.dist-info/RECORD,,
+MeMeST-2024.5.591143.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
+MeMeST-2024.5.591143.dist-info/METADATA,sha256=OhTih6yjIkqxmfJmONZutZwN-CAylW7lkkCtOY95Elo,1797
+MeMeST-2024.5.591143.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+MeMeST-2024.5.591143.dist-info/entry_points.txt,sha256=OYg2gMfzGJOXcQc_TTGdfCSPRPqlQylNW3LSReX_ta8,42
+MeMeST-2024.5.591143.dist-info/top_level.txt,sha256=iFxJRSyvq4K2f9Wl2wqP84mPUD7Ta4IoyDy9bDHkiYE,15
+MeMeST-2024.5.591143.dist-info/RECORD,,
```

