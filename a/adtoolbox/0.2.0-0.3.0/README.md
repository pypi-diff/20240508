# Comparing `tmp/adtoolbox-0.2.0.tar.gz` & `tmp/adtoolbox-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adtoolbox-0.2.0.tar", max compression
+gzip compressed data, was "adtoolbox-0.3.0.tar", max compression
```

## Comparing `adtoolbox-0.2.0.tar` & `adtoolbox-0.3.0.tar`

### file list

```diff
@@ -1,26 +1,25 @@
--rw-r--r--   0        0        0      602 2024-05-07 21:44:54.922798 adtoolbox-0.2.0/README.md
--rw-r--r--   0        0        0    10244 2024-04-30 20:19:14.071995 adtoolbox-0.2.0/adtoolbox/.DS_Store
--rw-r--r--   0        0        0     1157 2024-05-03 20:27:38.209459 adtoolbox-0.2.0/adtoolbox/__init__.py
--rw-r--r--   0        0        0      105 2024-05-08 17:23:25.597504 adtoolbox-0.2.0/adtoolbox/__main__.py
--rw-r--r--   0        0        0   128057 2024-05-08 17:13:08.818845 adtoolbox-0.2.0/adtoolbox/adm.py
--rw-r--r--   0        0        0     2205 2022-08-16 19:59:36.800896 adtoolbox-0.2.0/adtoolbox/bio_struct.py
--rwxr-xr-x   0        0        0    29972 2024-05-08 17:23:18.629590 adtoolbox-0.2.0/adtoolbox/cli.py
--rw-r--r--   0        0        0    16774 2024-05-07 04:58:30.708719 adtoolbox-0.2.0/adtoolbox/configs.py
--rw-r--r--   0        0        0   108577 2024-05-02 21:59:44.885729 adtoolbox-0.2.0/adtoolbox/core.py
--rw-r--r--   0        0        0    22543 2023-08-02 19:32:18.486966 adtoolbox-0.2.0/adtoolbox/metagenomics_report.py
--rw-r--r--   0        0        0    22395 2024-05-03 15:32:20.794835 adtoolbox-0.2.0/adtoolbox/optimize.py
--rw-r--r--   0        0        0     1416 2024-02-02 20:59:40.864054 adtoolbox-0.2.0/adtoolbox/pipeline.py
--rw-r--r--   0        0        0     6148 2024-04-30 20:21:01.993885 adtoolbox-0.2.0/adtoolbox/pkg_data/.DS_Store
--rw-r--r--   0        0        0       16 2024-05-08 17:26:06.999520 adtoolbox-0.2.0/adtoolbox/pkg_data/ADToolbox_Configs.json
--rw-r--r--   0        0        0    68830 2024-04-30 20:16:40.698305 adtoolbox-0.2.0/adtoolbox/pkg_data/Modified_ADM_Map.json
--rw-r--r--   0        0        0    12494 2024-04-30 20:13:51.051065 adtoolbox-0.2.0/adtoolbox/pkg_data/Modified_ADM_Model.json
--rw-r--r--   0        0        0     7558 2022-08-16 19:59:36.805098 adtoolbox-0.2.0/adtoolbox/pkg_data/README.md
--rw-r--r--   0        0        0     1123 2024-05-01 22:24:41.310110 adtoolbox-0.2.0/adtoolbox/pkg_data/qiime_template_paired.txt
--rw-r--r--   0        0        0     1090 2023-01-24 23:43:30.618643 adtoolbox-0.2.0/adtoolbox/pkg_data/qiime_template_single.txt
--rw-r--r--   0        0        0      235 2023-01-24 22:36:35.570064 adtoolbox-0.2.0/adtoolbox/pkg_data/slurm_template.txt
--rw-r--r--   0        0        0     2851 2023-12-18 19:46:22.537162 adtoolbox-0.2.0/adtoolbox/stats.py
--rw-r--r--   0        0        0    10949 2024-01-31 20:24:29.307481 adtoolbox-0.2.0/adtoolbox/tables.py
--rw-r--r--   0        0        0    15931 2024-02-01 18:57:40.645825 adtoolbox-0.2.0/adtoolbox/utils.py
--rw-r--r--   0        0        0      748 2024-05-08 17:28:38.270406 adtoolbox-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1773 2024-05-08 17:28:45.063110 adtoolbox-0.2.0/setup.py
--rw-r--r--   0        0        0     1575 2024-05-08 17:28:45.063294 adtoolbox-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      815 2024-05-08 17:32:14.704061 adtoolbox-0.3.0/README.md
+-rw-r--r--   0        0        0    10244 2024-05-08 17:37:32.568953 adtoolbox-0.3.0/adtoolbox/.DS_Store
+-rw-r--r--   0        0        0     1340 2024-05-08 17:40:07.800723 adtoolbox-0.3.0/adtoolbox/__init__.py
+-rw-r--r--   0        0        0      105 2024-05-08 17:23:25.597504 adtoolbox-0.3.0/adtoolbox/__main__.py
+-rw-r--r--   0        0        0   128039 2024-05-08 17:32:14.705216 adtoolbox-0.3.0/adtoolbox/adm.py
+-rw-r--r--   0        0        0     2205 2022-08-16 19:59:36.800896 adtoolbox-0.3.0/adtoolbox/bio_struct.py
+-rwxr-xr-x   0        0        0    29972 2024-05-08 17:23:18.629590 adtoolbox-0.3.0/adtoolbox/cli.py
+-rw-r--r--   0        0        0    16774 2024-05-07 04:58:30.708719 adtoolbox-0.3.0/adtoolbox/configs.py
+-rw-r--r--   0        0        0   108577 2024-05-02 21:59:44.885729 adtoolbox-0.3.0/adtoolbox/core.py
+-rw-r--r--   0        0        0    22543 2023-08-02 19:32:18.486966 adtoolbox-0.3.0/adtoolbox/metagenomics_report.py
+-rw-r--r--   0        0        0    22395 2024-05-03 15:32:20.794835 adtoolbox-0.3.0/adtoolbox/optimize.py
+-rw-r--r--   0        0        0     1416 2024-02-02 20:59:40.864054 adtoolbox-0.3.0/adtoolbox/pipeline.py
+-rw-r--r--   0        0        0     6148 2024-05-08 17:37:41.165336 adtoolbox-0.3.0/adtoolbox/pkg_data/.DS_Store
+-rw-r--r--   0        0        0    68830 2024-04-30 20:16:40.698305 adtoolbox-0.3.0/adtoolbox/pkg_data/Modified_ADM_Map.json
+-rw-r--r--   0        0        0    12494 2024-04-30 20:13:51.051065 adtoolbox-0.3.0/adtoolbox/pkg_data/Modified_ADM_Model.json
+-rw-r--r--   0        0        0     7558 2022-08-16 19:59:36.805098 adtoolbox-0.3.0/adtoolbox/pkg_data/README.md
+-rw-r--r--   0        0        0     1123 2024-05-01 22:24:41.310110 adtoolbox-0.3.0/adtoolbox/pkg_data/qiime_template_paired.txt
+-rw-r--r--   0        0        0     1090 2023-01-24 23:43:30.618643 adtoolbox-0.3.0/adtoolbox/pkg_data/qiime_template_single.txt
+-rw-r--r--   0        0        0      235 2023-01-24 22:36:35.570064 adtoolbox-0.3.0/adtoolbox/pkg_data/slurm_template.txt
+-rw-r--r--   0        0        0     2851 2023-12-18 19:46:22.537162 adtoolbox-0.3.0/adtoolbox/stats.py
+-rw-r--r--   0        0        0    10949 2024-01-31 20:24:29.307481 adtoolbox-0.3.0/adtoolbox/tables.py
+-rw-r--r--   0        0        0    15931 2024-02-01 18:57:40.645825 adtoolbox-0.3.0/adtoolbox/utils.py
+-rw-r--r--   0        0        0      748 2024-05-08 17:41:27.076133 adtoolbox-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1989 2024-05-08 17:41:47.971249 adtoolbox-0.3.0/setup.py
+-rw-r--r--   0        0        0     1788 2024-05-08 17:41:47.971426 adtoolbox-0.3.0/PKG-INFO
```

### Comparing `adtoolbox-0.2.0/adtoolbox/.DS_Store` & `adtoolbox-0.3.0/adtoolbox/.DS_Store`

 * *Files 0% similar despite different names*

```diff
@@ -417,15 +417,15 @@
 00001a00: 6270 6c69 7374 3030 d601 0203 0405 0607  bplist00........
 00001a10: 0709 070b 075d 5368 6f77 5374 6174 7573  .....]ShowStatus
 00001a20: 4261 725b 5368 6f77 546f 6f6c 6261 725b  Bar[ShowToolbar[
 00001a30: 5368 6f77 5461 6256 6965 775f 1014 436f  ShowTabView_..Co
 00001a40: 6e74 6169 6e65 7253 686f 7753 6964 6562  ntainerShowSideb
 00001a50: 6172 5c57 696e 646f 7742 6f75 6e64 735b  ar\WindowBounds[
 00001a60: 5368 6f77 5369 6465 6261 7209 0908 095f  ShowSidebar...._
-00001a70: 1018 7b7b 3133 332c 2033 3831 7d2c 207b  ..{{133, 381}, {
+00001a70: 1018 7b7b 3139 312c 2033 3233 7d2c 207b  ..{{191, 323}, {
 00001a80: 3932 302c 2034 3336 7d7d 0908 1523 2f3b  920, 436}}...#/;
 00001a90: 525f 6b6c 6d6e 6f8a 0000 0000 0000 0101  R_klmno.........
 00001aa0: 0000 0000 0000 000d 0000 0000 0000 0000  ................
 00001ab0: 0000 0000 0000 008b 0000 0008 0070 006b  .............p.k
 00001ac0: 0067 005f 0064 0061 0074 0061 6c67 3153  .g._.d.a.t.alg1S
 00001ad0: 636f 6d70 0000 0000 0001 7730 0000 0008  comp......w0....
 00001ae0: 0070 006b 0067 005f 0064 0061 0074 0061  .p.k.g._.d.a.t.a
```

### Comparing `adtoolbox-0.2.0/adtoolbox/__init__.py` & `adtoolbox-0.3.0/adtoolbox/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,14 +9,18 @@
 
 __version__ = "1.0.0"
 
 sys.path.append(os.path.join(os.path.dirname(__file__)))
 
 PKG_DATA=os.path.join(os.path.dirname(os.path.realpath(__file__)),"pkg_data")
 
+if not os.path.exists(os.path.join(PKG_DATA,"ADToolbox_Configs.json")):
+    with open(os.path.join(PKG_DATA,"ADToolbox_Configs.json"),"w") as f:
+        json.dump({"Base_Dir":""},f)
+
 with open(os.path.join(PKG_DATA,"ADToolbox_Configs.json"),"r") as f:
     conf = json.load(f)
     Main_Dir=conf["Base_Dir"]
 if Main_Dir and os.path.exists(Main_Dir):
     pass
 elif Main_Dir and not os.path.exists(Main_Dir):
     Main_Dir=input(f"Base directory is not configured properly.\nPlease input the correct path for the base directory:")
```

### Comparing `adtoolbox-0.2.0/adtoolbox/adm.py` & `adtoolbox-0.3.0/adtoolbox/adm.py`

 * *Files 0% similar despite different names*

```diff
@@ -575,15 +575,15 @@
             
                 )
             fig.update_traces(line=dict(width=3))
             return fig
             
 
 
-        app.run_server(port=8000, host='127.0.0.1')
+        app.run_server(**kwargs)
 
     def csv_report(self,sol: scipy.integrate._ivp.ivp.OdeResult ,address: str)->None:
         """Converts the results to a pandas data frame then to a csv"""
         df = pd.DataFrame(sol.y, columns=sol.t, index=self.species)
         df.to_csv(os.path.join(address,self.name+"_Report.csv"), header=True,
                   index=True)
         
@@ -2165,8 +2165,8 @@
                             metagenome_report=None)
     mod_adm1.control_state['S_H_ion']=0.000001
     mod_adm1.time_limit=100000
     
     mod_adm1.dash_app(mod_adm1.solve_model(t_eval=np.linspace(0, 30, 1000)))
     
     
-    
+
```

### Comparing `adtoolbox-0.2.0/adtoolbox/bio_struct.py` & `adtoolbox-0.3.0/adtoolbox/bio_struct.py`

 * *Files identical despite different names*

### Comparing `adtoolbox-0.2.0/adtoolbox/cli.py` & `adtoolbox-0.3.0/adtoolbox/cli.py`

 * *Files identical despite different names*

### Comparing `adtoolbox-0.2.0/adtoolbox/configs.py` & `adtoolbox-0.3.0/adtoolbox/configs.py`

 * *Files identical despite different names*

### Comparing `adtoolbox-0.2.0/adtoolbox/core.py` & `adtoolbox-0.3.0/adtoolbox/core.py`

 * *Files identical despite different names*

### Comparing `adtoolbox-0.2.0/adtoolbox/metagenomics_report.py` & `adtoolbox-0.3.0/adtoolbox/metagenomics_report.py`

 * *Files identical despite different names*

### Comparing `adtoolbox-0.2.0/adtoolbox/optimize.py` & `adtoolbox-0.3.0/adtoolbox/optimize.py`

 * *Files identical despite different names*

### Comparing `adtoolbox-0.2.0/adtoolbox/pipeline.py` & `adtoolbox-0.3.0/adtoolbox/pipeline.py`

 * *Files identical despite different names*

### Comparing `adtoolbox-0.2.0/adtoolbox/pkg_data/.DS_Store` & `adtoolbox-0.3.0/adtoolbox/pkg_data/.DS_Store`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 00000000: 0000 0001 4275 6431 0000 1000 0000 0800  ....Bud1........
-00000010: 0000 1000 0000 040a 0000 0000 0000 0000  ................
+00000010: 0000 1000 0000 0209 0000 0000 0000 0000  ................
 00000020: 0000 0000 0000 0000 0000 0000 0000 0800  ................
 00000030: 0000 0800 0000 0000 0000 0000 0000 0000  ................
-00000040: 0000 0000 0000 0002 0000 0000 0000 0007  ................
-00000050: 0000 0001 0000 1000 006f 006c 0062 006f  .........o.l.b.o
-00000060: 0078 005f 0000 0000 0000 0000 0000 0000  .x._............
+00000040: 0000 0000 0000 0002 0000 0000 0000 0006  ................
+00000050: 0000 0001 0000 1000 0066 0069 0065 0064  .........f.i.e.d
+00000060: 005f 0041 0000 0000 0000 0000 0000 0000  ._.A............
 00000070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000090: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -26,79 +26,79 @@
 00000190: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000200: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000210: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000220: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000230: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000240: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000250: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000260: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000270: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000280: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000290: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000002a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000002b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000002c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000002d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000002e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000002f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000300: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000310: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000320: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000330: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000340: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000350: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000360: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000370: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000380: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000390: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000003a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000003b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000200: 0000 0000 0000 0000 0000 0006 0000 0015  ................
+00000210: 004d 006f 0064 0069 0066 0069 0065 0064  .M.o.d.i.f.i.e.d
+00000220: 005f 0041 0044 004d 005f 004d 0061 0070  ._.A.D.M._.M.a.p
+00000230: 002e 006a 0073 006f 006e 496c 6f63 626c  ...j.s.o.nIlocbl
+00000240: 6f62 0000 0010 0000 0116 0000 002e ffff  ob..............
+00000250: ffff ffff 0000 0000 0017 004d 006f 0064  ...........M.o.d
+00000260: 0069 0066 0069 0065 0064 005f 0041 0044  .i.f.i.e.d._.A.D
+00000270: 004d 005f 004d 006f 0064 0065 006c 002e  .M._.M.o.d.e.l..
+00000280: 006a 0073 006f 006e 496c 6f63 626c 6f62  .j.s.o.nIlocblob
+00000290: 0000 0010 0000 018b 0000 002e ffff ffff  ................
+000002a0: ffff 0000 0000 0019 0071 0069 0069 006d  .........q.i.i.m
+000002b0: 0065 005f 0074 0065 006d 0070 006c 0061  .e._.t.e.m.p.l.a
+000002c0: 0074 0065 005f 0070 0061 0069 0072 0065  .t.e._.p.a.i.r.e
+000002d0: 0064 002e 0074 0078 0074 496c 6f63 626c  .d...t.x.tIlocbl
+000002e0: 6f62 0000 0010 0000 01f9 0000 002e ffff  ob..............
+000002f0: ffff ffff 0000 0000 0019 0071 0069 0069  ...........q.i.i
+00000300: 006d 0065 005f 0074 0065 006d 0070 006c  .m.e._.t.e.m.p.l
+00000310: 0061 0074 0065 005f 0073 0069 006e 0067  .a.t.e._.s.i.n.g
+00000320: 006c 0065 002e 0074 0078 0074 496c 6f63  .l.e...t.x.tIloc
+00000330: 626c 6f62 0000 0010 0000 0267 0000 002e  blob.......g....
+00000340: ffff ffff ffff 0000 0000 0009 0052 0045  .............R.E
+00000350: 0041 0044 004d 0045 002e 006d 0064 496c  .A.D.M.E...m.dIl
+00000360: 6f63 626c 6f62 0000 0010 0000 0041 0000  ocblob.......A..
+00000370: 002e ffff ffff ffff 0000 0000 0012 0073  ...............s
+00000380: 006c 0075 0072 006d 005f 0074 0065 006d  .l.u.r.m._.t.e.m
+00000390: 0070 006c 0061 0074 0065 002e 0074 0078  .p.l.a.t.e...t.x
+000003a0: 0074 496c 6f63 626c 6f62 0000 0010 0000  .tIlocblob......
+000003b0: 0041 0000 009e ffff ffff ffff 0000 0000  .A..............
 000003c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000400: 0000 0000 0000 0000 0000 0007 0000 0016  ................
-00000410: 0041 0044 0054 006f 006f 006c 0062 006f  .A.D.T.o.o.l.b.o
-00000420: 0078 005f 0043 006f 006e 0066 0069 0067  .x._.C.o.n.f.i.g
-00000430: 0073 002e 006a 0073 006f 006e 496c 6f63  .s...j.s.o.nIloc
-00000440: 626c 6f62 0000 0010 0000 00af 0000 002e  blob............
-00000450: ffff ffff ffff 0000 0000 0015 004d 006f  .............M.o
-00000460: 0064 0069 0066 0069 0065 0064 005f 0041  .d.i.f.i.e.d._.A
-00000470: 0044 004d 005f 004d 0061 0070 002e 006a  .D.M._.M.a.p...j
-00000480: 0073 006f 006e 496c 6f63 626c 6f62 0000  .s.o.nIlocblob..
-00000490: 0010 0000 0113 0000 003c ffff ffff ffff  .........<......
-000004a0: 0000 0000 0017 004d 006f 0064 0069 0066  .......M.o.d.i.f
-000004b0: 0069 0065 0064 005f 0041 0044 004d 005f  .i.e.d._.A.D.M._
-000004c0: 004d 006f 0064 0065 006c 002e 006a 0073  .M.o.d.e.l...j.s
-000004d0: 006f 006e 496c 6f63 626c 6f62 0000 0010  .o.nIlocblob....
-000004e0: 0000 018b 0000 002e ffff ffff ffff 0000  ................
-000004f0: 0000 0019 0071 0069 0069 006d 0065 005f  .....q.i.i.m.e._
-00000500: 0074 0065 006d 0070 006c 0061 0074 0065  .t.e.m.p.l.a.t.e
-00000510: 005f 0070 0061 0069 0072 0065 0064 002e  ._.p.a.i.r.e.d..
-00000520: 0074 0078 0074 496c 6f63 626c 6f62 0000  .t.x.tIlocblob..
-00000530: 0010 0000 01f9 0000 002e ffff ffff ffff  ................
-00000540: 0000 0000 0019 0071 0069 0069 006d 0065  .......q.i.i.m.e
-00000550: 005f 0074 0065 006d 0070 006c 0061 0074  ._.t.e.m.p.l.a.t
-00000560: 0065 005f 0073 0069 006e 0067 006c 0065  .e._.s.i.n.g.l.e
-00000570: 002e 0074 0078 0074 496c 6f63 626c 6f62  ...t.x.tIlocblob
-00000580: 0000 0010 0000 0267 0000 002e ffff ffff  .......g........
-00000590: ffff 0000 0000 0009 0052 0045 0041 0044  .........R.E.A.D
-000005a0: 004d 0045 002e 006d 0064 496c 6f63 626c  .M.E...m.dIlocbl
-000005b0: 6f62 0000 0010 0000 0041 0000 002e ffff  ob.......A......
-000005c0: ffff ffff 0000 0000 0012 0073 006c 0075  ...........s.l.u
-000005d0: 0072 006d 005f 0074 0065 006d 0070 006c  .r.m._.t.e.m.p.l
-000005e0: 0061 0074 0065 002e 0074 0078 0074 496c  .a.t.e...t.x.tIl
-000005f0: 6f63 626c 6f62 0000 0010 0000 0041 0000  ocblob.......A..
-00000600: 009e ffff ffff ffff 0000 0000 0000 0000  ................
+00000400: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000410: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000420: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000430: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000440: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000450: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000460: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000470: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000480: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000490: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000004a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000004b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000004c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000004d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000004e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000004f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000500: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000510: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000520: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000530: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000540: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000550: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000560: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000570: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000580: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000590: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000005a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000005b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000005c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000005d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000005e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000005f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000600: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000610: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000620: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000630: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000640: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000650: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000660: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000670: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -251,15 +251,15 @@
 00000fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001000: 0000 0000 0000 0003 0000 0000 0000 100b  ................
-00001010: 0000 0045 0000 040a 0000 0000 0000 0000  ...E............
+00001010: 0000 0045 0000 0209 0000 0000 0000 0000  ...E............
 00001020: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001030: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001040: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001050: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001060: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -319,15 +319,15 @@
 000013e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000013f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001400: 0000 0000 0000 0000 0000 0000 0000 0001  ................
 00001410: 0444 5344 4200 0000 0100 0000 0000 0000  .DSDB...........
 00001420: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001430: 0200 0000 2000 0000 6000 0000 0000 0000  .... ...`.......
 00001440: 0100 0000 8000 0000 0100 0001 0000 0000  ................
-00001450: 0100 0002 0000 0000 0000 0000 0200 0008  ................
+00001450: 0000 0000 0100 0004 0000 0000 0200 0008  ................
 00001460: 0000 0018 0000 0000 0000 0000 0100 0020  ............... 
 00001470: 0000 0000 0100 0040 0000 0000 0100 0080  .......@........
 00001480: 0000 0000 0100 0100 0000 0000 0100 0200  ................
 00001490: 0000 0000 0100 0400 0000 0000 0100 0800  ................
 000014a0: 0000 0000 0100 1000 0000 0000 0100 2000  .............. .
 000014b0: 0000 0000 0100 4000 0000 0000 0100 8000  ......@.........
 000014c0: 0000 0000 0101 0000 0000 0000 0102 0000  ................
```

### Comparing `adtoolbox-0.2.0/adtoolbox/pkg_data/Modified_ADM_Map.json` & `adtoolbox-0.3.0/adtoolbox/pkg_data/Modified_ADM_Map.json`

 * *Files identical despite different names*

### Comparing `adtoolbox-0.2.0/adtoolbox/pkg_data/Modified_ADM_Model.json` & `adtoolbox-0.3.0/adtoolbox/pkg_data/Modified_ADM_Model.json`

 * *Files identical despite different names*

### Comparing `adtoolbox-0.2.0/adtoolbox/pkg_data/README.md` & `adtoolbox-0.3.0/adtoolbox/pkg_data/README.md`

 * *Files identical despite different names*

### Comparing `adtoolbox-0.2.0/adtoolbox/pkg_data/qiime_template_paired.txt` & `adtoolbox-0.3.0/adtoolbox/pkg_data/qiime_template_paired.txt`

 * *Files identical despite different names*

### Comparing `adtoolbox-0.2.0/adtoolbox/pkg_data/qiime_template_single.txt` & `adtoolbox-0.3.0/adtoolbox/pkg_data/qiime_template_single.txt`

 * *Files identical despite different names*

### Comparing `adtoolbox-0.2.0/adtoolbox/stats.py` & `adtoolbox-0.3.0/adtoolbox/stats.py`

 * *Files identical despite different names*

### Comparing `adtoolbox-0.2.0/adtoolbox/tables.py` & `adtoolbox-0.3.0/adtoolbox/tables.py`

 * *Files identical despite different names*

### Comparing `adtoolbox-0.2.0/adtoolbox/utils.py` & `adtoolbox-0.3.0/adtoolbox/utils.py`

 * *Files identical despite different names*

### Comparing `adtoolbox-0.2.0/pyproject.toml` & `adtoolbox-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "adtoolbox"
-version = "0.2.0"
+version = "0.3.0"
 description = "A tool for modeling and optimization of anaerobic digestion process."
 authors = ["ParsaGhadermazi <54489047+ParsaGhadermazi@users.noreply.github.com>"]
 readme= "README.md"
 [tool.poetry.dependencies]
 python = ">=3.9,<3.12"
 bs4 = "^0.0.1"
 dash = "^2.4.1"
```

### Comparing `adtoolbox-0.2.0/setup.py` & `adtoolbox-0.3.0/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -23,17 +23,17 @@
  'sympy>=1.10.1,<2.0.0']
 
 entry_points = \
 {'console_scripts': ['ADToolbox = adtoolbox.__main__:main']}
 
 setup_kwargs = {
     'name': 'adtoolbox',
-    'version': '0.2.0',
+    'version': '0.3.0',
     'description': 'A tool for modeling and optimization of anaerobic digestion process.',
-    'long_description': '# Toolbox Overview\nParsa Ghadermazi \nparsa96@colostate.edu\n\nAD Toolbox is developed in Chan Lab at Colorado State University. The main goal of this toolbox is to provide the tools that are useful for modeling and optimization of anaerobic digestion process.\n\nInterested in trying ADToolbox? Run the notebooks on Binder:\n\n[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/chan-csu/ADToolbox/HEAD)\n\nADToolbox comes with a detailed documentation website. You can access this website using the link below:\n\n** [Full Documentation Here](https://chan-csu.github.io/ADToolbox/) **\n\n\n',
+    'long_description': '# Toolbox Overview\nParsa Ghadermazi \nparsa96@colostate.edu\n\nAD Toolbox is developed in Chan Lab at Colorado State University. The main goal of this toolbox is to provide the tools that are useful for modeling and optimization of anaerobic digestion process.\n\nInterested in trying ADToolbox? Run the notebooks on Binder or Colab:\n\n[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/chan-csu/ADToolbox/HEAD)\n<a target="_blank" href="https://colab.research.google.com/github/chan-csu/ADToolbox/blob/main/README.md">\n  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>\n</a>\n\nADToolbox comes with a detailed documentation website. You can access this website using the link below:\n\n** [Full Documentation Here](https://chan-csu.github.io/ADToolbox/) **\n\n\n',
     'author': 'ParsaGhadermazi',
     'author_email': '54489047+ParsaGhadermazi@users.noreply.github.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
     'packages': packages,
     'package_data': package_data,
```

### Comparing `adtoolbox-0.2.0/PKG-INFO` & `adtoolbox-0.3.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adtoolbox
-Version: 0.2.0
+Version: 0.3.0
 Summary: A tool for modeling and optimization of anaerobic digestion process.
 Author: ParsaGhadermazi
 Author-email: 54489047+ParsaGhadermazi@users.noreply.github.com
 Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
@@ -25,17 +25,20 @@
 
 # Toolbox Overview
 Parsa Ghadermazi 
 parsa96@colostate.edu
 
 AD Toolbox is developed in Chan Lab at Colorado State University. The main goal of this toolbox is to provide the tools that are useful for modeling and optimization of anaerobic digestion process.
 
-Interested in trying ADToolbox? Run the notebooks on Binder:
+Interested in trying ADToolbox? Run the notebooks on Binder or Colab:
 
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/chan-csu/ADToolbox/HEAD)
+<a target="_blank" href="https://colab.research.google.com/github/chan-csu/ADToolbox/blob/main/README.md">
+  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
+</a>
 
 ADToolbox comes with a detailed documentation website. You can access this website using the link below:
 
 ** [Full Documentation Here](https://chan-csu.github.io/ADToolbox/) **
```

