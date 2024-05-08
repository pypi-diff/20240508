# Comparing `tmp/pbs_builder-0.4.7.tar.gz` & `tmp/pbs_builder-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pbs_builder-0.4.7.tar", max compression
+gzip compressed data, was "pbs_builder-0.4.8.tar", max compression
```

## Comparing `pbs_builder-0.4.7.tar` & `pbs_builder-0.4.8.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1070 2023-07-19 02:02:11.000000 pbs_builder-0.4.7/LICENSE
--rw-r--r--   0        0        0     1705 2023-11-18 08:28:11.000000 pbs_builder-0.4.7/README.md
--rw-r--r--   0        0        0        0 2023-07-19 02:03:05.000000 pbs_builder-0.4.7/pbs_builder/__init__.py
--rwxr-xr-x   0        0        0    24045 2023-11-03 18:07:27.000000 pbs_builder-0.4.7/pbs_builder/bin/pestat
--rw-r--r--   0        0        0      203 2023-07-31 09:44:00.000000 pbs_builder-0.4.7/pbs_builder/pestat.py
--rw-r--r--   0        0        0     1965 2023-08-21 02:44:12.000000 pbs_builder-0.4.7/pbs_builder/pushover.py
--rw-r--r--   0        0        0    45165 2023-11-18 08:28:11.000000 pbs_builder-0.4.7/pbs_builder/qbatch.py
--rw-r--r--   0        0        0       22 2023-11-18 08:28:11.000000 pbs_builder-0.4.7/pbs_builder/version.py
--rw-r--r--   0        0        0      765 2023-11-18 08:28:11.000000 pbs_builder-0.4.7/pyproject.toml
--rw-r--r--   0        0        0     2495 1970-01-01 00:00:00.000000 pbs_builder-0.4.7/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-08-18 15:13:12.464409 pbs_builder-0.4.8/LICENSE
+-rw-r--r--   0        0        0     1705 2024-04-29 03:38:36.997436 pbs_builder-0.4.8/README.md
+-rw-r--r--   0        0        0        0 2023-08-18 15:13:12.464409 pbs_builder-0.4.8/pbs_builder/__init__.py
+-rwxr-xr-x   0        0        0    24045 2024-04-29 03:38:36.998436 pbs_builder-0.4.8/pbs_builder/bin/pestat
+-rw-r--r--   0        0        0      203 2024-04-29 03:38:36.999436 pbs_builder-0.4.8/pbs_builder/pestat.py
+-rw-r--r--   0        0        0     1965 2024-04-29 03:38:36.999436 pbs_builder-0.4.8/pbs_builder/pushover.py
+-rw-r--r--   0        0        0    45518 2024-05-08 07:24:50.372172 pbs_builder-0.4.8/pbs_builder/qbatch.py
+-rw-r--r--   0        0        0       22 2024-05-08 07:24:50.373172 pbs_builder-0.4.8/pbs_builder/version.py
+-rw-r--r--   0        0        0      765 2024-05-08 07:24:50.373172 pbs_builder-0.4.8/pyproject.toml
+-rw-r--r--   0        0        0     2495 1970-01-01 00:00:00.000000 pbs_builder-0.4.8/PKG-INFO
```

### Comparing `pbs_builder-0.4.7/LICENSE` & `pbs_builder-0.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pbs_builder-0.4.7/README.md` & `pbs_builder-0.4.8/README.md`

 * *Files identical despite different names*

### Comparing `pbs_builder-0.4.7/pbs_builder/bin/pestat` & `pbs_builder-0.4.8/pbs_builder/bin/pestat`

 * *Files identical despite different names*

### Comparing `pbs_builder-0.4.7/pbs_builder/pushover.py` & `pbs_builder-0.4.8/pbs_builder/pushover.py`

 * *Files identical despite different names*

### Comparing `pbs_builder-0.4.7/pbs_builder/qbatch.py` & `pbs_builder-0.4.8/pbs_builder/qbatch.py`

 * *Files 0% similar despite different names*

```diff
@@ -324,17 +324,20 @@
             if 'group_sheet' in job_dict:
                 groups = self.load_group_sheet(template['group_sheet'])
             else:
                 groups = {}
 
             # Iter through samples & groups
             if len(samples) > 0 and len(groups) > 0:
-                group_iterator = product(samples, groups) if is_verbose else tqdm(list(product(samples, groups)), ncols=50)
                 n_submit, n_skip = 0, 0
-                for sample, group in group_iterator:
+                for sample, group in product(samples, groups):
+                    if not is_verbose:
+                        sys.stderr.write(f"{job_name} - submitted {n_submit} and skipped {n_skip} jobs\r")
+                        sys.stderr.flush()
+
                     # Init job object & parse job
                     job = Job(job_name+'.'+sample.name+'.'+group.name, template.dict)
                     job.map_(sample, group, self.dict)
 
                     # Create PBS job script
                     pbs_file = self.script_dir / (job.name + ".sh")
                     pbs_job = PBSJob(job, self.dict, pbs_file)
@@ -392,16 +395,19 @@
                     if pbs_cmd is not None:
                         lock.write(f"{job.name}\t{pbs_id}\t{pbs_cmd}\n")
                 sys.stderr.write(f"{job_name} - submitted {n_submit} and skipped {n_skip} jobs\n")
 
             # Iter through samples only
             elif len(samples) > 0:
                 n_submit, n_skip = 0, 0
-                job_iterator = samples if is_verbose else tqdm(samples, ncols=50)
-                for sample in job_iterator:
+                for sample in samples:
+                    if not is_verbose:
+                        sys.stderr.write(f"{job_name} - submitted {n_submit} and skipped {n_skip} jobs\r")
+                        sys.stderr.flush()
+
                     # Init job object & parse job
                     job = Job(job_name+'.'+sample.name, template.dict)
                     job.map_(sample, {}, self.dict)
 
                     # Create PBS job script
                     pbs_file = self.script_dir / (job.name + ".sh")
                     pbs_job = PBSJob(job, self.dict, pbs_file)
@@ -797,14 +803,16 @@
             else:
                 pass
 
     def is_finished(self):
         # No defined output file
         if 'output' not in self.dict:
             return False
+        if 'skip' in self.dict:
+            return True
 
         # Determine if output has been generated
         flag = True
         # For multiple output files
         if isinstance(self['output'], dict):
             for k, v in self['output'].items():
                 p = Path(v)
@@ -1066,30 +1074,29 @@
     file_name = Path(args.toml).name
     time_stamp = timestamp()
     toml_content = [
         '# Parameters',
         'pipeline = "{}"'.format(file_name),
         'version = "{}"'.format(time_stamp),
         'cwd = "{}"'.format(cwd),
-        'work_dir = "{{cwd}}/qsub.{}"'.format(file_name),
-        'sample_sheet = "{cwd}/samples.csv"',
+        'work_dir = "{cwd}/qsub.{pipeline}"',
+        'sample_sheet = "{cwd}/{pipeline}.csv"',
         'pbs_scheduler = "torque"',
         'pbs_server = "mu02"',
         'pbs_queue = "batch"',
         'pbs_walltime = 1200',
         'threads = 32',
         '',
         '# Executables',
         'bwa = "/histor/public/software/bwa-0.7.17/bwa"',
         'samtools = "/histor/public/software/samtools-1.11/bin/samtools"',
         '',
         '# Reference',
         'genome = "/histor/public/database/gencode/v37/GRCh38.primary_assembly.genome.fa"',
         '',
-        '#Jobs',
         '[job.bwa]',
         'sample_sheet = "{sample_sheet}"',
         'input = "{sample.name}"',
         'output = "{cwd}/out_alignment/{sample.name}.sorted.bam"',
         'log = "{work_dir}/logs/{sample.name}.bwa.logs"',
         'shell = """',
         'mkdir -p {cwd}/out_alignment/{sample.name}',
@@ -1131,18 +1138,22 @@
             qid = content[1]
             job_ids.append(qid)
     sys.stderr.write(f"Loaded {len(job_ids)} jobs\n")
 
     # Delete job in reverse order
     # Only delete Q and R jobs, H jobs will be deleted automatically
     jobs2 = []
-    for qid in tqdm(job_ids[::-1], ncols=50):
+    n_del = 0
+    for qid in job_ids[::-1]:
+        sys.stderr.write(f"Deleted {n_del} jobs\r")
+        sys.stderr.flush()
         sleep(0.1)
-        s = validate_torque_job(qid, ret_state=True)
+        n_del += 1
 
+        s = validate_torque_job(qid, ret_state=True)
         # Completed job
         if s is False:
             continue
         
         # Hold jobs
         if s in ["H", "Q"]:
             status, ret = getstatusoutput(f"qdel {qid}")
@@ -1153,14 +1164,15 @@
             elif status == 170: # Already complete
                 continue
             else:
                 sys.stderr.write(f"Failed to delete job {qid}, {ret}:\n")
                 sys.exit(1)
         else: # Q or R jobs
             jobs2.append(qid)
+    sys.stderr.write(f"Deleted {n_del} jobs\n")
 
     # Delete Q and R jobs
     sys.stderr.write(f"{len(jobs2)} running jobs left for manual deletion\n")
 
 
 def main():
     import argparse
```

### Comparing `pbs_builder-0.4.7/pyproject.toml` & `pbs_builder-0.4.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pbs-builder"
-version = "0.4.7"
+version = "0.4.8"
 description = "The workflow management system for scalable data analyses."
 authors = ["Jinyang Zhang <zhangjinyang@biols.ac.cn>"]
 readme = "README.md"
 license = "LICENSE"
 classifiers = [
     "Development Status :: 4 - Beta",
     "License :: OSI Approved :: MIT License",
```

### Comparing `pbs_builder-0.4.7/PKG-INFO` & `pbs_builder-0.4.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pbs-builder
-Version: 0.4.7
+Version: 0.4.8
 Summary: The workflow management system for scalable data analyses.
 License: LICENSE
 Author: Jinyang Zhang
 Author-email: zhangjinyang@biols.ac.cn
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

