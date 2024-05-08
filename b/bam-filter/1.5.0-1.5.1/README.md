# Comparing `tmp/bam-filter-1.5.0.tar.gz` & `tmp/bam-filter-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bam-filter-1.5.0.tar", last modified: Tue May  7 15:03:02 2024, max compression
+gzip compressed data, was "bam-filter-1.5.1.tar", last modified: Wed May  8 07:16:53 2024, max compression
```

## Comparing `bam-filter-1.5.0.tar` & `bam-filter-1.5.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:03:02.509945 bam-filter-1.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-05-07 15:02:59.000000 bam-filter-1.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-07 15:02:59.000000 bam-filter-1.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-07 15:03:02.509945 bam-filter-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    21540 2024-05-07 15:02:59.000000 bam-filter-1.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:03:02.509945 bam-filter-1.5.0/bam_filter/
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-07 15:02:59.000000 bam-filter-1.5.0/bam_filter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-05-07 15:02:59.000000 bam-filter-1.5.0/bam_filter/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-07 15:03:02.509945 bam-filter-1.5.0/bam_filter/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     6414 2024-05-07 15:02:59.000000 bam-filter-1.5.0/bam_filter/entropy.py
--rw-r--r--   0 runner    (1001) docker     (127)    10025 2024-05-07 15:02:59.000000 bam-filter-1.5.0/bam_filter/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)    23934 2024-05-07 15:02:59.000000 bam-filter-1.5.0/bam_filter/lca.py
--rw-r--r--   0 runner    (1001) docker     (127)    36957 2024-05-07 15:02:59.000000 bam-filter-1.5.0/bam_filter/reassign.py
--rw-r--r--   0 runner    (1001) docker     (127)    51508 2024-05-07 15:02:59.000000 bam-filter-1.5.0/bam_filter/sam_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    47368 2024-05-07 15:02:59.000000 bam-filter-1.5.0/bam_filter/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:03:02.509945 bam-filter-1.5.0/bam_filter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-07 15:03:02.000000 bam-filter-1.5.0/bam_filter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-07 15:03:02.000000 bam-filter-1.5.0/bam_filter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 15:03:02.000000 bam-filter-1.5.0/bam_filter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-07 15:03:02.000000 bam-filter-1.5.0/bam_filter.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-07 15:03:02.000000 bam-filter-1.5.0/bam_filter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-07 15:03:02.000000 bam-filter-1.5.0/bam_filter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-07 15:03:02.509945 bam-filter-1.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-05-07 15:02:59.000000 bam-filter-1.5.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)    70238 2024-05-07 15:02:59.000000 bam-filter-1.5.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:16:53.669841 bam-filter-1.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-05-08 07:16:49.000000 bam-filter-1.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-08 07:16:49.000000 bam-filter-1.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-08 07:16:53.669841 bam-filter-1.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    21540 2024-05-08 07:16:49.000000 bam-filter-1.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:16:53.669841 bam-filter-1.5.1/bam_filter/
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-08 07:16:49.000000 bam-filter-1.5.1/bam_filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-05-08 07:16:49.000000 bam-filter-1.5.1/bam_filter/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-08 07:16:53.669841 bam-filter-1.5.1/bam_filter/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6414 2024-05-08 07:16:49.000000 bam-filter-1.5.1/bam_filter/entropy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10025 2024-05-08 07:16:49.000000 bam-filter-1.5.1/bam_filter/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23934 2024-05-08 07:16:49.000000 bam-filter-1.5.1/bam_filter/lca.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37663 2024-05-08 07:16:49.000000 bam-filter-1.5.1/bam_filter/reassign.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51945 2024-05-08 07:16:49.000000 bam-filter-1.5.1/bam_filter/sam_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48912 2024-05-08 07:16:49.000000 bam-filter-1.5.1/bam_filter/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:16:53.669841 bam-filter-1.5.1/bam_filter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-08 07:16:53.000000 bam-filter-1.5.1/bam_filter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-08 07:16:53.000000 bam-filter-1.5.1/bam_filter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 07:16:53.000000 bam-filter-1.5.1/bam_filter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-08 07:16:53.000000 bam-filter-1.5.1/bam_filter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-08 07:16:53.000000 bam-filter-1.5.1/bam_filter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-08 07:16:53.000000 bam-filter-1.5.1/bam_filter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-08 07:16:53.669841 bam-filter-1.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-05-08 07:16:49.000000 bam-filter-1.5.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    70238 2024-05-08 07:16:49.000000 bam-filter-1.5.1/versioneer.py
```

### Comparing `bam-filter-1.5.0/LICENSE` & `bam-filter-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bam-filter-1.5.0/README.md` & `bam-filter-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `bam-filter-1.5.0/bam_filter/__main__.py` & `bam-filter-1.5.1/bam_filter/__main__.py`

 * *Files identical despite different names*

### Comparing `bam-filter-1.5.0/bam_filter/entropy.py` & `bam-filter-1.5.1/bam_filter/entropy.py`

 * *Files identical despite different names*

### Comparing `bam-filter-1.5.0/bam_filter/filter.py` & `bam-filter-1.5.1/bam_filter/filter.py`

 * *Files identical despite different names*

### Comparing `bam-filter-1.5.0/bam_filter/lca.py` & `bam-filter-1.5.1/bam_filter/lca.py`

 * *Files identical despite different names*

### Comparing `bam-filter-1.5.0/bam_filter/reassign.py` & `bam-filter-1.5.1/bam_filter/reassign.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     create_empty_output_files,
     sort_keys_by_approx_weight,
     is_debug,
     get_arguments,
     check_tmp_dir_exists,
     handle_warning,
     create_output_files,
+    allocate_threads,
 )
 from multiprocessing import Pool, Manager
 from functools import partial
 import gc
 from collections import defaultdict
 import os
 import concurrent.futures
@@ -236,15 +237,15 @@
 def write_to_file(alns, out_bam_file, header=None):
     for aln in alns:
         out_bam_file.write(pysam.AlignedSegment.fromstring(aln, header))
 
 
 def process_references_batch(references, entries, bam, refs_idx, threads=4):
     alns = []
-    s_threads = min(4, threads)
+    s_threads = threads
     with pysam.AlignmentFile(bam, "rb", threads=s_threads) as samfile:
         for reference in references:
             r_ids = entries[reference]
             for aln in samfile.fetch(
                 reference=reference, multiple_iterators=False, until_eof=True
             ):
                 if (aln.query_name, reference) in r_ids:
@@ -267,145 +268,151 @@
     disable_sort=False,
 ):
     # if out_files["bam_reassigned"] is not None:
     #     out_bam = out_files["bam_reassigned"]
     # else:
     #     out_bam = out_files["bam_reassigned_sorted"]
     out_bam = out_files["bam_reassigned"]
-    s_threads = min(4, threads)
+    p_threads, s_threads = allocate_threads(threads, 2, 4)
+    # s_threads = min(4, threads)
     with pysam.AlignmentFile(bam, "rb", threads=s_threads) as samfile:
         references = list(entries.keys())
         refs_dict = {x: samfile.get_reference_length(x) for x in references}
         # get group reads
         header = samfile.header
 
     log.info("::: Getting reference names and lengths...")
     (ref_names, ref_lengths) = zip(*refs_dict.items())
     refs_idx = {sys.intern(str(x)): i for i, x in enumerate(ref_names)}
-    write_threads = min(4, threads)
+    write_threads = s_threads
 
     new_header = header.to_dict()
 
     log.info("::: Creating new header...")
     ref_names_set = set(ref_names)
     new_header["SQ"] = [x for x in new_header["SQ"] if x["SN"] in ref_names_set]
 
     name_index = {name: idx for idx, name in enumerate(ref_names)}
     new_header["SQ"].sort(key=lambda x: name_index[x["SN"]])
     new_header["HD"]["SO"] = "unsorted"
 
-    out_bam_file = pysam.AlignmentFile(
+    with pysam.AlignmentFile(
         out_files["bam_reassigned_tmp"],
         "wb",
         referencenames=list(ref_names),
         referencelengths=list(ref_lengths),
         threads=write_threads,
         header=new_header,
-    )
-
-    # num_cores should be multiple of the write_threads
-    num_cores = threads // write_threads
-    # num_cores = min(threads, cpu_count())
-    # batch_size = len(references) // num_cores + 1  # Ensure non-zero batch size
-    # batch_size = calc_chunksize(n_workers=num_cores, len_iterable=len(references))
-    log.info("::: Creating reference chunks with uniform read amounts...")
+    ) as out_bam_file:
 
-    ref_chunks = sort_keys_by_approx_weight(
-        input_dict=ref_counts,
-        scale=1,
-        num_cores=num_cores,
-        verbose=False,
-        max_entries_per_chunk=1_000_000,
-    )
+        # num_cores should be multiple of the write_threads
+        num_cores = p_threads
+        # num_cores = min(threads, cpu_count())
+        # batch_size = len(references) // num_cores + 1  # Ensure non-zero batch size
+        # batch_size = calc_chunksize(n_workers=num_cores, len_iterable=len(references))
+        log.info("::: Creating reference chunks with uniform read amounts...")
+
+        ref_chunks = sort_keys_by_approx_weight(
+            input_dict=ref_counts,
+            scale=1,
+            num_cores=num_cores,
+            verbose=False,
+            max_entries_per_chunk=1_000_000,
+        )
 
-    num_cores = min(num_cores, len(ref_chunks))
-    log.info(f"::: Using {num_cores} processes to write {len(ref_chunks)} chunk(s)")
+        # num_cores = min(num_cores, len(ref_chunks))
+        log.info(f"::: Using {num_cores} processes to write {len(ref_chunks)} chunk(s)")
 
-    with Manager() as manager:
-        # Use Manager to create a read-only proxy for the dictionary
-        entries = manager.dict(dict(entries))
-
-        with concurrent.futures.ProcessPoolExecutor(max_workers=num_cores) as executor:
-            # Use ProcessPoolExecutor to parallelize the processing of references in batches
-            futures = []
-            for batch_references in tqdm.tqdm(
-                ref_chunks,
-                total=len(ref_chunks),
-                desc="Submitted batches",
-                unit="batch",
-                leave=False,
-                ncols=80,
-                disable=is_debug(),
-            ):
-                future = executor.submit(
-                    process_references_batch, batch_references, entries, bam, refs_idx
+        with Manager() as manager:
+            # Use Manager to create a read-only proxy for the dictionary
+            entries = manager.dict(dict(entries))
+
+            with concurrent.futures.ProcessPoolExecutor(
+                max_workers=num_cores
+            ) as executor:
+                # Use ProcessPoolExecutor to parallelize the processing of references in batches
+                futures = []
+                for batch_references in tqdm.tqdm(
+                    ref_chunks,
+                    total=len(ref_chunks),
+                    desc="Submitted batches",
+                    unit="batch",
+                    leave=False,
+                    ncols=80,
+                    disable=is_debug(),
+                ):
+                    future = executor.submit(
+                        process_references_batch,
+                        batch_references,
+                        entries,
+                        bam,
+                        refs_idx,
+                        s_threads,
+                    )
+                    futures.append(future)  # Store the future
+
+                # Use a while loop to continuously check for completed futures
+                log.info("::: Collecting batches...")
+
+                completion_progress_bar = tqdm.tqdm(
+                    total=len(futures),
+                    desc="Completed",
+                    unit="batch",
+                    leave=False,
+                    ncols=80,
+                    disable=is_debug(),
                 )
-                futures.append(future)  # Store the future
-
-            # Use a while loop to continuously check for completed futures
-            log.info("::: Collecting batches...")
-
-            completion_progress_bar = tqdm.tqdm(
-                total=len(futures),
-                desc="Completed",
-                unit="batch",
-                leave=False,
-                ncols=80,
-                disable=is_debug(),
-            )
-            completed_count = 0
+                completed_count = 0
 
-            # Use as_completed to iterate over completed futures as they become available
-            for completed_future in concurrent.futures.as_completed(futures):
-                alns = completed_future.result()
-                write_to_file(alns=alns, out_bam_file=out_bam_file, header=header)
-
-                # Update the progress bar for each completed write
-                completion_progress_bar.update(1)
-                completed_count += 1
-                completed_future.cancel()  # Cancel the future to free memory
-                gc.collect()  # Force garbage collection
+                # Use as_completed to iterate over completed futures as they become available
+                for completed_future in concurrent.futures.as_completed(futures):
+                    alns = completed_future.result()
+                    write_to_file(alns=alns, out_bam_file=out_bam_file, header=header)
+
+                    # Update the progress bar for each completed write
+                    completion_progress_bar.update(1)
+                    completed_count += 1
+                    completed_future.cancel()  # Cancel the future to free memory
+                    gc.collect()  # Force garbage collection
 
-            completion_progress_bar.close()
-    out_bam_file.close()
+                completion_progress_bar.close()
     entries = None
     gc.collect()
     # prof.disable()
     # # print profiling output
     # stats = pstats.Stats(prof).strip_dirs().sort_stats("tottime")
     # stats.print_stats(5)  # top 10 rows
     if not disable_sort:
         log.info("::: ::: Sorting BAM file...")
-        s_threads = min(4, threads)
+        w_threads = max(4, s_threads)
         if sort_by_name:
             log.info("::: ::: Sorting by name...")
             pysam.sort(
                 "-n",
                 "-@",
-                str(s_threads),
+                str(w_threads),
                 "-m",
                 str(sort_memory),
                 "-o",
                 out_bam,
                 out_files["bam_reassigned_tmp"],
             )
         else:
             pysam.sort(
                 "-@",
-                str(s_threads),
+                str(w_threads),
                 "-m",
                 str(sort_memory),
                 "-o",
                 out_bam,
                 out_files["bam_reassigned_tmp"],
             )
 
         logging.info("BAM index not found. Indexing...")
 
-        s_threads = min(4, threads)
         pysam.index(
             "-c",
             "-@",
             str(threads),
             out_bam,
         )
 
@@ -462,15 +469,15 @@
     precomputed_factor = lambda_value * match_reward / math.log(2)
     precomputed_log_K = math.log(K_value) / math.log(2)
 
     bam, references = parms
     dt.options.progress.enabled = False
     dt.options.progress.clear_on_success = True
     dt.options.nthreads = max(1, threads - 1)
-    s_threads = min(4, threads)
+    s_threads = threads
 
     with pysam.AlignmentFile(bam, "rb", threads=s_threads) as samfile:
         results = []
         reads = set()
         refs = set()
         empty_df = 0
 
@@ -556,24 +563,31 @@
     min_read_ani=90,
     min_read_length=30,
     reassign_iters=25,
     reassign_scale=0.9,
     sort_memory="4G",
     disable_sort=False,
 ):
+
+    p_threads, s_threads = allocate_threads(threads, 2, 4)
     dt.options.progress.enabled = True
     dt.options.progress.clear_on_success = True
     if threads > 1:
-        dt.options.nthreads = threads - 1
+        dt.options.nthreads = p_threads
     else:
         dt.options.nthreads = 1
 
     log.info("::: Loading BAM file")
     save = pysam.set_verbosity(0)
-    s_threads = min(4, threads)
+    # we need to separate the threads for reading the BAM and process in parallel.
+    # At least 2 threads are needed for reading the BAM file and the rest for multiprocessing
+
+    # s_threads = min(4, threads)
+
+    log.info(f"::: IO Threads: {s_threads} | Processing Threads: {p_threads}")
 
     with pysam.AlignmentFile(bam, "rb", threads=s_threads) as samfile:
         references = samfile.references
         pysam.set_verbosity(save)
 
         total_refs = samfile.nreferences
         log.info(f"::: Found {total_refs:,} reference sequences")
@@ -668,15 +682,15 @@
                 leave=False,
                 ncols=80,
                 desc="Chunks processed",
             )
         )
     else:
         p = Pool(
-            threads,
+            p_threads,
         )
         data = list(
             tqdm.tqdm(
                 p.imap_unordered(
                     partial(
                         get_bam_data,
                         ref_lengths=ref_len_dict,
@@ -684,15 +698,15 @@
                         min_read_length=min_read_length,
                         match_reward=match_reward,
                         mismatch_penalty=mismatch_penalty,
                         gap_open_penalty=gap_open_penalty,
                         gap_extension_penalty=gap_extension_penalty,
                         lambda_value=lambda_value,
                         K_value=K_value,
-                        threads=4,
+                        threads=s_threads,
                     ),
                     parms,
                     chunksize=1,
                 ),
                 total=len(parms),
                 leave=False,
                 ncols=80,
```

### Comparing `bam-filter-1.5.0/bam_filter/sam_utils.py` & `bam-filter-1.5.1/bam_filter/sam_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import pysam
 import numpy as np
 import os
 import sys
 import pandas as pd
-from multiprocessing import Pool, cpu_count
+from multiprocessing import Pool
 import functools
 from scipy import stats
 import tqdm
 import logging
 import warnings
 from bam_filter.utils import (
     is_debug,
     create_empty_output_files,
     create_empty_bam,
     sort_keys_by_approx_weight,
+    allocate_threads,
 )
 from bam_filter.entropy import entropy, norm_entropy, gini_coeff, norm_gini_coeff
 from collections import defaultdict
 import pyranges as pr
 from pathlib import Path
 import concurrent.futures
 import gc
@@ -45,19 +46,20 @@
 #     ):
 #         alns.append(aln.to_string())
 #     return alns
 
 
 def write_bam(bam, references, output_files, threads=1, sort_memory="1G"):
     logging.info("::: Writing temporary filtered BAM file... (be patient)")
-    s_threads = min(threads, 4)
+    p_threads, s_threads = allocate_threads(threads, 2, 4)
+    # s_threads = min(threads, 4)
     samfile = pysam.AlignmentFile(bam, "rb", threads=s_threads)
     header = samfile.header
 
-    threads = min(threads, 4)
+    # threads = min(threads, 4)
 
     # convert the dictionary to an array
     refs_dict = dict(zip(samfile.references, samfile.lengths))
     my_array = np.array(list(refs_dict.items()))
 
     # get the indices of the keys to keep
     keep_indices = np.isin(my_array[:, 0], references)
@@ -71,15 +73,15 @@
     (ref_names, ref_lengths) = zip(*refs_dict.items())
     ref_lengths = list(ref_lengths)
     # convert reference lengths to integers
     ref_lengths = [int(x) for x in ref_lengths]
 
     refs_idx = {sys.intern(str(x)): i for i, x in enumerate(ref_names)}
 
-    write_threads = min(threads, 4)
+    write_threads = min(s_threads, 4)
 
     new_header = header.to_dict()
     new_header["SQ"] = [x for x in new_header["SQ"] if x["SN"] in list(ref_names)]
     new_header["SQ"].sort(key=lambda x: list(ref_names).index(x["SN"]))
     # change it to unsorted
     new_header["HD"]["SO"] = "unsorted"
 
@@ -112,15 +114,15 @@
             out_bam_file.write(aln)
     out_bam_file.close()
     samfile.close()
     # prof.disable()
     # # print profiling output
     # stats = pstats.Stats(prof).strip_dirs().sort_stats("tottime")
     # stats.print_stats(5)  # top 10 rows
-    s_threads = min(threads, 4)
+    # s_threads = min(threads, 4)
 
     logging.info("::: ::: Sorting BAM file...")
     pysam.sort(
         "-@",
         str(s_threads),
         "-m",
         str(sort_memory),
@@ -128,15 +130,15 @@
         output_files["bam_tmp_sorted"],
         output_files["bam_tmp"],
     )
 
     logging.info("::: ::: BAM index not found. Indexing...")
     save = pysam.set_verbosity(0)
 
-    s_threads = min(threads, 4)
+    # s_threads = min(threads, 4)
 
     samfile = pysam.AlignmentFile(
         output_files["bam_tmp_sorted"], "rb", threads=s_threads
     )
     # chr_lengths = []
     # for chrom in samfile.references:
     #     chr_lengths.append(samfile.get_reference_length(chrom))
@@ -281,15 +283,15 @@
     two definitions of the edit distances to the reference genome scaled by aligned read length
     """
     # prof = profile.Profile()
     # prof.enable()
     bam, references = params
     results = []
 
-    threads = min(threads, 4)
+    # threads = min(threads, 4)
 
     with pysam.AlignmentFile(bam, "rb", threads=threads) as samfile:
         bam_reference_lengths = {
             reference: np.int64(samfile.get_reference_length(reference))
             for reference in references
         }
         read_hits = defaultdict(int)
@@ -788,16 +790,16 @@
     sort_memory="1G",
 ):
     logging.info("Checking BAM file status")
     save = pysam.set_verbosity(0)
 
     # Use a with statement to ensure proper closing of the samfile
     try:
+        # p_threads, s_threads = allocate_threads(threads, 2, 4)
         s_threads = min(threads, 4)
-
         with pysam.AlignmentFile(bam, "rb", threads=s_threads) as samfile:
             references = samfile.references
             log.info(f"::: Found {samfile.nreferences:,} reference sequences")
             references = samfile.references
             pysam.set_verbosity(save)
             ref_lengths = None
 
@@ -867,15 +869,17 @@
     Processing function: calls pool of worker functions
     to extract from a bam file two definitions of the edit distances to the reference genome scaled by read length
     Returned in a pandas DataFrame
     """
     logging.info("Loading BAM file")
     save = pysam.set_verbosity(0)
 
-    s_threads = min(threads, 4)
+    # s_threads = min(threads, 4)
+    p_threads, s_threads = allocate_threads(threads, 2, 4)
+    log.info(f"::: IO Threads: {s_threads} | Processing Threads: {p_threads}")
 
     with pysam.AlignmentFile(bam, "rb", threads=s_threads) as samfile:
 
         references = samfile.references
 
         # chr_lengths = []
         # for chrom in samfile.references:
@@ -940,25 +944,25 @@
             bam = write_bam(
                 bam=bam,
                 references=references,
                 output_files=output_files,
                 sort_memory=sort_memory,
                 threads=threads,
             )
-            s_threads = min(threads, 4)
+            # s_threads = min(threads, 4)
 
             # samfile = pysam.AlignmentFile(bam, "rb", threads=s_threads)
 
     log.info("::: Creating reference chunks with uniform read amounts...")
 
     # ify the number of chunks
     ref_chunks = sort_keys_by_approx_weight(
         input_dict=references_m,
         scale=1,
-        num_cores=threads,
+        num_cores=p_threads,
         verbose=False,
         max_entries_per_chunk=100_000,
     )
     log.info(f"::: Created {len(ref_chunks):,} chunks")
     # ref_chunks = random.sample(ref_chunks, len(ref_chunks))
     params = zip([bam] * len(ref_chunks), ref_chunks)
     try:
@@ -973,15 +977,15 @@
                         trim_ends=0,
                         trim_min=trim_min,
                         trim_max=trim_max,
                         scale=scale,
                         plot=plot,
                         plots_dir=plots_dir,
                         read_length_freqs=read_length_freqs,
-                        threads=threads,
+                        threads=s_threads,
                     ),
                     params,
                 )
             )
         else:
             p = Pool(
                 threads,
@@ -1028,18 +1032,16 @@
 def write_to_file(alns, out_bam_file, header=None):
     for aln in alns:
         out_bam_file.write(pysam.AlignedSegment.fromstring(aln, header))
 
 
 def process_references_batch(references, bam, refs_idx, min_read_ani, threads=1):
     alns = []
-    if threads > 4:
-        s_threads = 4
-    else:
-        s_threads = threads
+    p_threads, s_threads = allocate_threads(threads, 2, 4)
+
     with pysam.AlignmentFile(bam, "rb", threads=s_threads) as samfile:
         for reference in references:
             for aln in samfile.fetch(
                 reference=reference, multiple_iterators=False, until_eof=True
             ):
                 ani_read = (1 - ((aln.get_tag("NM") / aln.infer_query_length()))) * 100
                 if ani_read >= min_read_ani:
@@ -1153,18 +1155,19 @@
         )
         if out_files["bam_filtered"] is not None:
             logging.info("Writing filtered BAM file... (be patient)")
             # refs_dict = dict(
             #     zip(df_filtered["reference"], df_filtered["bam_reference_length"])
             # )
             references = df_filtered["reference"].tolist()
-            if threads > 4:
-                s_threads = 4
-            else:
-                s_threads = threads
+            # if threads > 4:
+            #     s_threads = 4
+            # else:
+            #     s_threads = threads
+            p_threads, s_threads = allocate_threads(threads, 2, 4)
             samfile = pysam.AlignmentFile(bam, "rb", threads=s_threads)
             refs_dict = {x: samfile.get_reference_length(x) for x in references}
             header = samfile.header
             (ref_names, ref_lengths) = zip(*refs_dict.items())
             ref_dict_m = {
                 chrom.contig: chrom.mapped
                 for chrom in samfile.get_index_statistics()
@@ -1208,25 +1211,25 @@
             #     ):
             #         ani_read = (
             #             1 - ((aln.get_tag("NM") / aln.infer_query_length()))
             #         ) * 100
             #         if ani_read >= min_read_ani:
             #             aln.reference_id = refs_idx[aln.reference_name]
             #             out_bam_file.write(aln)
-            num_cores = min(threads, cpu_count())
+            num_cores = p_threads
             # batch_size = len(references) // num_cores + 1  # Ensure non-zero batch size
             log.info("::: Creating reference chunks with uniform read amounts...")
             ref_chunks = sort_keys_by_approx_weight(
                 input_dict=ref_dict_m,
                 scale=1,
                 num_cores=threads,
                 verbose=False,
                 max_entries_per_chunk=1_000_000,
             )
-            num_cores = min(num_cores, len(ref_chunks))
+            # num_cores = min(num_cores, len(ref_chunks))
             log.info(f"::: Using {num_cores} cores to write {len(ref_chunks)} chunk(s)")
 
             # with Manager() as manager:
             #     # Use Manager to create a read-only proxy for the dictionary
             #     #refs_idx = manager.dict(refs_idx)
 
             with concurrent.futures.ProcessPoolExecutor(
@@ -1245,14 +1248,15 @@
                 ):
                     future = executor.submit(
                         process_references_batch,
                         batch_references,
                         bam,
                         refs_idx,
                         min_read_ani=min_read_ani,
+                        threads=s_threads,
                     )
                     futures.append(future)  # Store the future
 
                 # Use a while loop to continuously check for completed futures
                 log.info("::: Collecting batches...")
 
                 completion_progress_bar = tqdm.tqdm(
@@ -1276,21 +1280,23 @@
                     gc.collect()  # Force garbage collection
                 completion_progress_bar.close()
             out_bam_file.close()
             # prof.disable()
             # # print profiling output
             # stats = pstats.Stats(prof).strip_dirs().sort_stats("tottime")
             # stats.print_stats(5)  # top 10 rows
+
             if not disable_sort:
+                s_threads = min(threads, 4)
                 if sort_by_name:
                     logging.info("Sorting BAM file by read name...")
-                    if threads > 4:
-                        s_threads = 4
-                    else:
-                        s_threads = threads
+                    # if threads > 4:
+                    #     s_threads = 4
+                    # else:
+                    #     s_threads = threads
                     pysam.sort(
                         "-n",
                         "-@",
                         str(s_threads),
                         "-m",
                         str(sort_memory),
                         "-o",
@@ -1307,18 +1313,18 @@
                         "-o",
                         out_files["bam_filtered"],
                         out_files["bam_filtered_tmp"],
                     )
 
                     logging.info("BAM index not found. Indexing...")
                     save = pysam.set_verbosity(0)
-                    if threads > 4:
-                        s_threads = 4
-                    else:
-                        s_threads = threads
+                    # if threads > 4:
+                    #     s_threads = 4
+                    # else:
+                    #     s_threads = threads
                     samfile = pysam.AlignmentFile(
                         out_files["bam_filtered"], "rb", threads=s_threads
                     )
                     # chr_lengths = []
                     # for chrom in samfile.references:
                     #     chr_lengths.append(samfile.get_reference_length(chrom))
                     # max_chr_length = np.max(chr_lengths)
```

### Comparing `bam-filter-1.5.0/bam_filter/utils.py` & `bam-filter-1.5.1/bam_filter/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import time
 from itertools import chain
 import numpy as np
 from pathlib import Path
 import pysam
 import tempfile
 
-
 log = logging.getLogger("my_logger")
 log.setLevel(logging.INFO)
 timestr = time.strftime("%Y%m%d-%H%M%S")
 
 
 def handle_warning(message, category, filename, lineno, file=None, line=None):
     print("A warning occurred:")
@@ -1466,7 +1465,47 @@
     #     "bam_reassigned": bam_reassigned,
     #     "read_length_freqs": read_length_freqs,
     #     "read_hits_count": read_hits_count,
     #     "knee_plot": knee_plot,
     #     "coverage_plot_dir": coverage_plots,
     #     "lca_summary": lca_summary,
     # }
+
+
+def allocate_threads(total_threads, min_io_processes, max_io_processes):
+    """
+    Allocates threads between CPU-bound workers and I/O-bound processes based on total threads and
+    desired range of I/O processes. Selects the best compromise to maximize CPU-bound workers.
+
+    Parameters:
+        total_threads (int): Total number of available threads.
+        min_io_processes (int): Minimum desired I/O-bound processes.
+        max_io_processes (int): Maximum desired I/O-bound processes.
+
+    Returns:
+        tuple: (Number of workers, Number of I/O processes)
+    """
+    if min_io_processes > max_io_processes:
+        raise ValueError(
+            "Minimum I/O processes cannot be greater than maximum I/O processes."
+        )
+    if min_io_processes <= 0 or max_io_processes <= 0:
+        raise ValueError("I/O processes must be positive integers.")
+
+    best_allocation = (
+        1,
+        total_threads,
+    )  # Start with all threads assigned to 1 worker if no better found
+    max_workers = 0
+
+    for io_processes in range(min_io_processes, max_io_processes + 1):
+        if (
+            total_threads >= io_processes
+        ):  # Ensure there are enough threads to allocate at least these many I/O processes
+            workers = total_threads // io_processes
+            if (
+                workers > max_workers
+            ):  # Find the configuration with the maximum number of CPU workers
+                max_workers = workers
+                best_allocation = (workers, io_processes)
+
+    return best_allocation
```

### Comparing `bam-filter-1.5.0/setup.cfg` & `bam-filter-1.5.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `bam-filter-1.5.0/setup.py` & `bam-filter-1.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `bam-filter-1.5.0/versioneer.py` & `bam-filter-1.5.1/versioneer.py`

 * *Files identical despite different names*

