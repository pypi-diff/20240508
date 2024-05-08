# Comparing `tmp/sourmash_plugin_directsketch-0.1.0.tar.gz` & `tmp/sourmash_plugin_directsketch-0.2.0.tar.gz`

## Comparing `sourmash_plugin_directsketch-0.1.0.tar` & `sourmash_plugin_directsketch-0.2.0.tar`

### file list

```diff
@@ -1,41 +1,43 @@
--rw-r--r--   0        0        0      821 1970-01-01 00:00:00.000000 sourmash_plugin_directsketch-0.1.0/Cargo.toml
--rw-r--r--   0      501       20      363 2024-04-30 22:43:20.000000 sourmash_plugin_directsketch-0.1.0/.github/dependabot.yml
--rw-r--r--   0      501       20     1474 2024-05-01 15:58:15.000000 sourmash_plugin_directsketch-0.1.0/.github/workflows/build-test.yml
--rw-r--r--   0      501       20      718 2024-04-26 03:30:23.000000 sourmash_plugin_directsketch-0.1.0/.gitignore
--rw-r--r--   0      501       20     1540 2024-04-26 00:09:24.000000 sourmash_plugin_directsketch-0.1.0/LICENSE
--rw-r--r--   0      501       20      368 2024-05-01 15:59:57.000000 sourmash_plugin_directsketch-0.1.0/Makefile
--rw-r--r--   0      501       20     2571 2024-04-27 00:56:29.000000 sourmash_plugin_directsketch-0.1.0/README.md
--rw-r--r--   0      501       20      176 2024-04-30 23:49:37.000000 sourmash_plugin_directsketch-0.1.0/environment.yml
--rw-r--r--   0      501       20   798402 2024-04-27 00:57:13.000000 sourmash_plugin_directsketch-0.1.0/out_fastas/GCA_000175555.1_genomic.fna.gz
--rw-r--r--   0      501       20   526013 2024-04-27 00:57:13.000000 sourmash_plugin_directsketch-0.1.0/out_fastas/GCA_000961135.2_genomic.fna.gz
--rw-r--r--   0      501       20   314606 2024-04-27 00:57:13.000000 sourmash_plugin_directsketch-0.1.0/out_fastas/GCA_000961135.2_protein.faa.gz
--rw-r--r--   0      501       20    15648 2024-05-01 00:34:30.000000 sourmash_plugin_directsketch-0.1.0/src/directsketch.rs
--rw-r--r--   0      501       20     1597 2024-05-01 00:29:05.000000 sourmash_plugin_directsketch-0.1.0/src/lib.rs
--rw-r--r--   0      501       20     4553 2024-05-01 01:23:38.000000 sourmash_plugin_directsketch-0.1.0/src/python/sourmash_plugin_directsketch/__init__.py
--rw-r--r--   0      501       20     5730 2024-04-26 23:49:48.000000 sourmash_plugin_directsketch-0.1.0/src/utils.rs
--rw-r--r--   0      501       20   118778 2024-04-27 00:57:14.000000 sourmash_plugin_directsketch-0.1.0/test.zip
--rw-r--r--   0      501       20      228 2024-04-27 01:38:57.000000 sourmash_plugin_directsketch-0.1.0/tests/conftest.py
--rw-r--r--   0      501       20     6849 2024-04-26 00:09:24.000000 sourmash_plugin_directsketch-0.1.0/tests/sourmash_tst_utils.py
--rw-r--r--   0      501       20        0 2024-04-26 00:09:24.000000 sourmash_plugin_directsketch-0.1.0/tests/test-data/.notempty
--rw-r--r--   0      501       20    44471 2024-04-26 18:22:33.000000 sourmash_plugin_directsketch-0.1.0/tests/test-data/GCA_000175555.1.sig.gz
--rw-r--r--   0      501       20    20407 2024-04-27 01:42:18.000000 sourmash_plugin_directsketch-0.1.0/tests/test-data/GCA_000961135.2.protein.sig.gz
--rw-r--r--   0      501       20    29259 2024-04-26 18:04:28.000000 sourmash_plugin_directsketch-0.1.0/tests/test-data/GCA_000961135.2.sig.gz
--rw-r--r--   0      501       20      497 2024-04-27 02:01:15.000000 sourmash_plugin_directsketch-0.1.0/tests/test-data/acc.csv
--rw-r--r--   0      501       20   798402 2024-04-27 00:46:04.000000 sourmash_plugin_directsketch-0.1.0/tests/test-data/out_fastas/GCA_000175555.1_genomic.fna.gz
--rw-r--r--   0      501       20   526013 2024-04-27 00:46:04.000000 sourmash_plugin_directsketch-0.1.0/tests/test-data/out_fastas/GCA_000961135.2_genomic.fna.gz
--rw-r--r--   0      501       20   314606 2024-04-27 00:46:04.000000 sourmash_plugin_directsketch-0.1.0/tests/test-data/out_fastas/GCA_000961135.2_protein.faa.gz
--rw-r--r--   0      501       20   798402 2024-04-26 18:00:37.000000 sourmash_plugin_directsketch-0.1.0/tests/test-data/outputs/GCA_000175555.1_genomic.fna.gz
--rw-r--r--   0      501       20     7793 2024-04-26 18:00:37.000000 sourmash_plugin_directsketch-0.1.0/tests/test-data/outputs/GCA_000337115.1_assembly_report.txt
--rw-r--r--   0      501       20  1118769 2024-04-26 18:00:37.000000 sourmash_plugin_directsketch-0.1.0/tests/test-data/outputs/GCA_000337115.1_genomic.fna.gz
--rw-r--r--   0      501       20     1201 2024-04-26 18:00:37.000000 sourmash_plugin_directsketch-0.1.0/tests/test-data/outputs/GCA_000337115.1_md5checksums.txt
--rw-r--r--   0      501       20   702342 2024-04-26 18:00:37.000000 sourmash_plugin_directsketch-0.1.0/tests/test-data/outputs/GCA_000337115.1_protein.faa.gz
--rw-r--r--   0      501       20    36700 2024-04-26 18:00:37.000000 sourmash_plugin_directsketch-0.1.0/tests/test-data/outputs/GCA_000961135.2_assembly_report.txt
--rw-r--r--   0      501       20   526013 2024-04-26 18:00:37.000000 sourmash_plugin_directsketch-0.1.0/tests/test-data/outputs/GCA_000961135.2_genomic.fna.gz
--rw-r--r--   0      501       20     1201 2024-04-26 18:00:37.000000 sourmash_plugin_directsketch-0.1.0/tests/test-data/outputs/GCA_000961135.2_md5checksums.txt
--rw-r--r--   0      501       20   314606 2024-04-26 18:00:37.000000 sourmash_plugin_directsketch-0.1.0/tests/test-data/outputs/GCA_000961135.2_protein.faa.gz
--rw-r--r--   0      501       20   735547 2024-04-26 18:00:37.000000 sourmash_plugin_directsketch-0.1.0/tests/test-data/outputs/GCA_001950595.1_genomic.fna.gz
--rw-r--r--   0      501       20   118778 2024-04-27 00:46:05.000000 sourmash_plugin_directsketch-0.1.0/tests/test-data/test.zip
--rw-r--r--   0      501       20    11413 2024-05-01 16:15:57.000000 sourmash_plugin_directsketch-0.1.0/tests/test_gbsketch.py
--rw-r--r--   0      501       20    61419 2024-05-01 16:18:30.000000 sourmash_plugin_directsketch-0.1.0/Cargo.lock
--rw-r--r--   0      501       20      966 2024-04-26 04:06:31.000000 sourmash_plugin_directsketch-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3241 1970-01-01 00:00:00.000000 sourmash_plugin_directsketch-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1052 1970-01-01 00:00:00.000000 sourmash_plugin_directsketch-0.2.0/Cargo.toml
+-rw-r--r--   0      501       20      405 2024-05-08 16:20:18.000000 sourmash_plugin_directsketch-0.2.0/.github/dependabot.yml
+-rw-r--r--   0      501       20     1474 2024-05-08 16:20:14.000000 sourmash_plugin_directsketch-0.2.0/.github/workflows/build-test.yml
+-rw-r--r--   0      501       20      718 2024-04-26 03:30:23.000000 sourmash_plugin_directsketch-0.2.0/.gitignore
+-rw-r--r--   0      501       20     1540 2024-04-26 00:09:24.000000 sourmash_plugin_directsketch-0.2.0/LICENSE
+-rw-r--r--   0      501       20      368 2024-05-01 15:59:57.000000 sourmash_plugin_directsketch-0.2.0/Makefile
+-rw-r--r--   0      501       20     2417 2024-05-01 22:22:17.000000 sourmash_plugin_directsketch-0.2.0/README.md
+-rw-r--r--   0      501       20      176 2024-04-30 23:49:37.000000 sourmash_plugin_directsketch-0.2.0/environment.yml
+-rw-r--r--   0      501       20    51553 2024-05-02 00:08:24.000000 sourmash_plugin_directsketch-0.2.0/out_fastas/GCA_000175555.1_assembly_report.txt
+-rw-r--r--   0      501       20   798402 2024-05-02 00:08:23.000000 sourmash_plugin_directsketch-0.2.0/out_fastas/GCA_000175555.1_genomic.fna.gz
+-rw-r--r--   0      501       20    36700 2024-05-02 00:08:22.000000 sourmash_plugin_directsketch-0.2.0/out_fastas/GCA_000961135.2_assembly_report.txt
+-rw-r--r--   0      501       20   526013 2024-05-02 00:08:22.000000 sourmash_plugin_directsketch-0.2.0/out_fastas/GCA_000961135.2_genomic.fna.gz
+-rw-r--r--   0      501       20   314606 2024-05-02 00:08:22.000000 sourmash_plugin_directsketch-0.2.0/out_fastas/GCA_000961135.2_protein.faa.gz
+-rw-r--r--   0      501       20    25113 2024-05-08 18:17:29.000000 sourmash_plugin_directsketch-0.2.0/src/directsketch.rs
+-rw-r--r--   0      501       20     2359 2024-05-08 18:17:29.000000 sourmash_plugin_directsketch-0.2.0/src/lib.rs
+-rw-r--r--   0      501       20     4597 2024-05-08 16:20:18.000000 sourmash_plugin_directsketch-0.2.0/src/python/sourmash_plugin_directsketch/__init__.py
+-rw-r--r--   0      501       20     5730 2024-05-07 17:31:28.000000 sourmash_plugin_directsketch-0.2.0/src/utils.rs
+-rw-r--r--   0      501       20    38326 2024-05-08 14:36:55.000000 sourmash_plugin_directsketch-0.2.0/test.zip
+-rw-r--r--   0      501       20      410 2024-05-08 18:17:29.000000 sourmash_plugin_directsketch-0.2.0/tests/conftest.py
+-rw-r--r--   0      501       20     6849 2024-04-26 00:09:24.000000 sourmash_plugin_directsketch-0.2.0/tests/sourmash_tst_utils.py
+-rw-r--r--   0      501       20        0 2024-04-26 00:09:24.000000 sourmash_plugin_directsketch-0.2.0/tests/test-data/.notempty
+-rw-r--r--   0      501       20    44471 2024-04-26 18:22:33.000000 sourmash_plugin_directsketch-0.2.0/tests/test-data/GCA_000175555.1.sig.gz
+-rw-r--r--   0      501       20    20407 2024-04-27 01:42:18.000000 sourmash_plugin_directsketch-0.2.0/tests/test-data/GCA_000961135.2.protein.sig.gz
+-rw-r--r--   0      501       20    29259 2024-04-26 18:04:28.000000 sourmash_plugin_directsketch-0.2.0/tests/test-data/GCA_000961135.2.sig.gz
+-rw-r--r--   0      501       20      497 2024-04-27 02:01:15.000000 sourmash_plugin_directsketch-0.2.0/tests/test-data/acc.csv
+-rw-r--r--   0      501       20   798402 2024-04-27 00:46:04.000000 sourmash_plugin_directsketch-0.2.0/tests/test-data/out_fastas/GCA_000175555.1_genomic.fna.gz
+-rw-r--r--   0      501       20   526013 2024-04-27 00:46:04.000000 sourmash_plugin_directsketch-0.2.0/tests/test-data/out_fastas/GCA_000961135.2_genomic.fna.gz
+-rw-r--r--   0      501       20   314606 2024-04-27 00:46:04.000000 sourmash_plugin_directsketch-0.2.0/tests/test-data/out_fastas/GCA_000961135.2_protein.faa.gz
+-rw-r--r--   0      501       20   798402 2024-04-26 18:00:37.000000 sourmash_plugin_directsketch-0.2.0/tests/test-data/outputs/GCA_000175555.1_genomic.fna.gz
+-rw-r--r--   0      501       20     7793 2024-04-26 18:00:37.000000 sourmash_plugin_directsketch-0.2.0/tests/test-data/outputs/GCA_000337115.1_assembly_report.txt
+-rw-r--r--   0      501       20  1118769 2024-04-26 18:00:37.000000 sourmash_plugin_directsketch-0.2.0/tests/test-data/outputs/GCA_000337115.1_genomic.fna.gz
+-rw-r--r--   0      501       20     1201 2024-04-26 18:00:37.000000 sourmash_plugin_directsketch-0.2.0/tests/test-data/outputs/GCA_000337115.1_md5checksums.txt
+-rw-r--r--   0      501       20   702342 2024-04-26 18:00:37.000000 sourmash_plugin_directsketch-0.2.0/tests/test-data/outputs/GCA_000337115.1_protein.faa.gz
+-rw-r--r--   0      501       20    36700 2024-04-26 18:00:37.000000 sourmash_plugin_directsketch-0.2.0/tests/test-data/outputs/GCA_000961135.2_assembly_report.txt
+-rw-r--r--   0      501       20   526013 2024-04-26 18:00:37.000000 sourmash_plugin_directsketch-0.2.0/tests/test-data/outputs/GCA_000961135.2_genomic.fna.gz
+-rw-r--r--   0      501       20     1201 2024-04-26 18:00:37.000000 sourmash_plugin_directsketch-0.2.0/tests/test-data/outputs/GCA_000961135.2_md5checksums.txt
+-rw-r--r--   0      501       20   314606 2024-04-26 18:00:37.000000 sourmash_plugin_directsketch-0.2.0/tests/test-data/outputs/GCA_000961135.2_protein.faa.gz
+-rw-r--r--   0      501       20   735547 2024-04-26 18:00:37.000000 sourmash_plugin_directsketch-0.2.0/tests/test-data/outputs/GCA_001950595.1_genomic.fna.gz
+-rw-r--r--   0      501       20   118778 2024-04-27 00:46:05.000000 sourmash_plugin_directsketch-0.2.0/tests/test-data/test.zip
+-rw-r--r--   0      501       20    11413 2024-05-06 22:31:50.000000 sourmash_plugin_directsketch-0.2.0/tests/test_gbsketch.py
+-rw-r--r--   0      501       20    63427 2024-05-08 18:30:02.000000 sourmash_plugin_directsketch-0.2.0/Cargo.lock
+-rw-r--r--   0      501       20     1003 2024-05-08 16:20:18.000000 sourmash_plugin_directsketch-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3087 1970-01-01 00:00:00.000000 sourmash_plugin_directsketch-0.2.0/PKG-INFO
```

### Comparing `sourmash_plugin_directsketch-0.1.0/Cargo.toml` & `sourmash_plugin_directsketch-0.2.0/Cargo.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,34 +1,42 @@
 
 [package]
 name = "sourmash_plugin_directsketch"
-version = "0.1.0"
+version = "0.2.0"
 edition = "2021"
 
 [lib]
 name = "sourmash_plugin_directsketch"
 crate-type = ["cdylib"]
 
 [dependencies]
 pyo3 = { version = "0.21.2", features = ["extension-module", "anyhow"] }
 rayon = "1.10.0"
-serde = { version = "1.0.198", features = ["derive"] }
+serde = { version = "1.0.200", features = ["derive"] }
 sourmash = { version = "0.13.1"}
 serde_json = "1.0.116"
 niffler = "2.4.0"
 needletail = "0.5.1"
 #zip = { version = "0.6", default-features = false, features = ["deflate"] }
-async_zip="0.0.6"
+async_zip={version="0.0.17", features=["full"]}
 simple-error = "0.3.0"
 anyhow = "1.0.82"
 camino = "1.1.6"
 csv = "1.3.0"
-reqwest = { version = "0.12.4", features = ["json"] }
+reqwest = { version = "0.12.4", features = ["json", "stream"] }
 tokio = { version = "1.37.0", features = ["full"] }
+tokio-util = "0.7.11"
 regex = "1.10.4"
+chrono = "0.4.32"
+lazy_static = "1.4.0"
+md5 = "0.7.0"
 openssl = { version = "0.10", features = ["vendored"] }
+futures = "0.3.30"
+
+[build-dependencies]
+pyo3-build-config = { version = "0.21.2", features = ["resolve-config"] }
 
 [profile.release]
 #target-cpu=native
 lto = "thin"
 opt-level = 3
```

### Comparing `sourmash_plugin_directsketch-0.1.0/.github/workflows/build-test.yml` & `sourmash_plugin_directsketch-0.2.0/.github/workflows/build-test.yml`

 * *Files identical despite different names*

### Comparing `sourmash_plugin_directsketch-0.1.0/.gitignore` & `sourmash_plugin_directsketch-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `sourmash_plugin_directsketch-0.1.0/LICENSE` & `sourmash_plugin_directsketch-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sourmash_plugin_directsketch-0.1.0/README.md` & `sourmash_plugin_directsketch-0.2.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,15 @@
 # sourmash_plugin_directsketch
 
 ## Installation
 
-For now, git clone the repository and cd in.
 ```
-mamba env create -f environment.yml
-pip install -e .
+pip install sourmash_plugin_directsketch
 ```
 
-> When it's released, you'll be able to:
-> ```
-> pip install sourmash_plugin_directsketch
-> ```
-
 ## Usage
 First, create a file, e.g. `acc.csv` with GenBank identifiers and sketch names.
 ```
 ident,name
 GCA_000961135.2,GCA_000961135.2 Candidatus Aramenus sulfurataquae isolate AZ1-45
 GCA_000175555.1,GCA_000175555.1 ACUK01000506.1 Saccharolobus solfataricus 98/2
 ```
```

### Comparing `sourmash_plugin_directsketch-0.1.0/out_fastas/GCA_000175555.1_genomic.fna.gz` & `sourmash_plugin_directsketch-0.2.0/out_fastas/GCA_000175555.1_genomic.fna.gz`

 * *Files identical despite different names*

### Comparing `sourmash_plugin_directsketch-0.1.0/out_fastas/GCA_000961135.2_genomic.fna.gz` & `sourmash_plugin_directsketch-0.2.0/out_fastas/GCA_000961135.2_genomic.fna.gz`

 * *Files identical despite different names*

### Comparing `sourmash_plugin_directsketch-0.1.0/out_fastas/GCA_000961135.2_protein.faa.gz` & `sourmash_plugin_directsketch-0.2.0/out_fastas/GCA_000961135.2_protein.faa.gz`

 * *Files identical despite different names*

### Comparing `sourmash_plugin_directsketch-0.1.0/src/lib.rs` & `sourmash_plugin_directsketch-0.2.0/src/lib.rs`

 * *Files 27% similar despite different names*

```diff
@@ -1,34 +1,58 @@
+use lazy_static::lazy_static;
+use pyo3::exceptions::PyRuntimeError;
 /// Python interface Rust code for sourmash_plugin_directsketch.
 use pyo3::prelude::*;
+use std::sync::Mutex;
+use tokio::runtime::{Builder, Runtime};
 
 // #[macro_use]
 extern crate simple_error;
 
 mod directsketch;
 mod utils;
 
+lazy_static! {
+    static ref GLOBAL_RUNTIME: Mutex<Option<Runtime>> = Mutex::new(None);
+}
+
 #[pyfunction]
-fn set_global_thread_pool(num_threads: usize) -> PyResult<usize> {
-    if std::panic::catch_unwind(|| {
-        rayon::ThreadPoolBuilder::new()
-            .num_threads(num_threads)
-            .build_global()
-    })
-    .is_ok()
-    {
-        Ok(rayon::current_num_threads())
-    } else {
-        Err(PyErr::new::<pyo3::exceptions::PyRuntimeError, _>(
-            "Could not set the number of threads. Global thread pool might already be initialized.",
-        ))
+fn set_tokio_thread_pool(num_threads: usize) -> PyResult<usize> {
+    let mut rt_lock = GLOBAL_RUNTIME.lock().unwrap();
+
+    // Check if pytest is running
+    let pytest_running = std::env::var("PYTEST_RUNNING").is_ok();
+
+    // Check if runtime is already initialized
+    if rt_lock.is_some() {
+        if pytest_running {
+            // If pytest is running, simply return the number of threads without error
+            return Ok(num_threads);
+        } else {
+            // If not under pytest, return an error on reinitialization attempts
+            return Err(PyErr::new::<PyRuntimeError, _>(
+                "Tokio runtime is already initialized.",
+            ));
+        }
     }
+
+    // Initialize the runtime if not already initialized
+    let runtime = Builder::new_multi_thread()
+        .worker_threads(num_threads)
+        .enable_all()
+        .build()
+        .map_err(PyErr::new::<PyRuntimeError, _>)?;
+
+    *rt_lock = Some(runtime);
+
+    Ok(num_threads)
 }
 
 #[pyfunction]
+#[allow(clippy::too_many_arguments)]
 fn do_gbsketch(
     py: Python,
     input_csv: String,
     param_str: String,
     failed_csv: String,
     output_sigs: String,
     retry_times: u32,
@@ -56,12 +80,12 @@
             eprintln!("Error: {e}");
             Ok(1)
         }
     }
 }
 
 #[pymodule]
-fn sourmash_plugin_directsketch(py: Python, m: &Bound<'_, PyModule>) -> PyResult<()> {
+fn sourmash_plugin_directsketch(_py: Python, m: &Bound<'_, PyModule>) -> PyResult<()> {
     m.add_function(wrap_pyfunction!(do_gbsketch, m)?)?;
-    m.add_function(wrap_pyfunction!(set_global_thread_pool, m)?)?;
+    m.add_function(wrap_pyfunction!(set_tokio_thread_pool, m)?)?;
     Ok(())
 }
```

### Comparing `sourmash_plugin_directsketch-0.1.0/src/python/sourmash_plugin_directsketch/__init__.py` & `sourmash_plugin_directsketch-0.2.0/src/python/sourmash_plugin_directsketch/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,20 +21,20 @@
         else:
             return os.cpu_count()
     except Exception:
         return os.cpu_count()
 
 
 def set_thread_pool(user_cores):
-    avail_threads = get_max_cores()
+    avail_threads = get_max_cores()  # Define how to get the maximum available cores
     num_threads = min(avail_threads, user_cores) if user_cores else avail_threads
     if user_cores and user_cores > avail_threads:
         notify(f"warning: only {avail_threads} threads available, using {avail_threads}")
-    actual_rayon_cores = sourmash_plugin_directsketch.set_global_thread_pool(num_threads)
-    return actual_rayon_cores
+    actual_tokio_cores = sourmash_plugin_directsketch.set_tokio_thread_pool(num_threads)
+    return actual_tokio_cores
 
 class Download_and_Sketch_Assemblies(CommandLinePlugin):
     command = 'gbsketch'
     description = 'download and sketch GenBank assembly datasets'
 
     def __init__(self, p):
         super().__init__(p)
@@ -72,15 +72,15 @@
         # convert to a single string for easier rust handling
         args.param_string = "_".join(args.param_string)
         # lowercase the param string
         args.param_string = args.param_string.lower()
 
         num_threads = set_thread_pool(args.cores)
 
-        notify(f"downloading and sketching all accessions in '{args.input_csv}'") #using {num_threads} threads")
+        notify(f"downloading and sketching all accessions in '{args.input_csv} using {num_threads} threads")
 
         super().main(args)
         status = sourmash_plugin_directsketch.do_gbsketch(args.input_csv,
                                                            args.param_string,
                                                            args.failed,
                                                            args.output,
                                                            args.retry_times,
```

### Comparing `sourmash_plugin_directsketch-0.1.0/src/utils.rs` & `sourmash_plugin_directsketch-0.2.0/src/utils.rs`

 * *Files identical despite different names*

### Comparing `sourmash_plugin_directsketch-0.1.0/test.zip` & `sourmash_plugin_directsketch-0.2.0/tests/test-data/test.zip`

 * *Files 1% similar despite different names*

#### zipinfo {}

```diff
@@ -1,8 +1,8 @@
 Zip file size: 118778 bytes, number of entries: 6
--rw----     0.0 fat    15210 b- stor 24-Apr-27 00:57 signatures/febc807030a90b6e6823b7942a5e4988.sig.gz
--rw----     0.0 fat    15047 b- stor 24-Apr-27 00:57 signatures/d900308fb443444ff6127b7bfbd463c1.sig.gz
--rw----     0.0 fat    40761 b- stor 24-Apr-27 00:57 signatures/7b72fb5f81ec4e5dceb61ff330253511.sig.gz
--rw----     0.0 fat    23316 b- stor 24-Apr-27 00:57 signatures/f54c012657c20304f8455dca3b268196.sig.gz
--rw----     0.0 fat    22245 b- stor 24-Apr-27 00:57 signatures/8196cc69b814cab9fc3c7e9eed861bf6.sig.gz
--rw----     0.0 fat     1179 b- stor 24-Apr-27 00:57 SOURMASH-MANIFEST.csv
+-rw----     0.0 fat    15210 b- stor 24-Apr-27 00:46 signatures/febc807030a90b6e6823b7942a5e4988.sig.gz
+-rw----     0.0 fat    15047 b- stor 24-Apr-27 00:46 signatures/d900308fb443444ff6127b7bfbd463c1.sig.gz
+-rw----     0.0 fat    40761 b- stor 24-Apr-27 00:46 signatures/7b72fb5f81ec4e5dceb61ff330253511.sig.gz
+-rw----     0.0 fat    23316 b- stor 24-Apr-27 00:46 signatures/f54c012657c20304f8455dca3b268196.sig.gz
+-rw----     0.0 fat    22245 b- stor 24-Apr-27 00:46 signatures/8196cc69b814cab9fc3c7e9eed861bf6.sig.gz
+-rw----     0.0 fat     1179 b- stor 24-Apr-27 00:46 SOURMASH-MANIFEST.csv
 6 files, 117758 bytes uncompressed, 117758 bytes compressed:  0.0%
```

### Comparing `sourmash_plugin_directsketch-0.1.0/tests/sourmash_tst_utils.py` & `sourmash_plugin_directsketch-0.2.0/tests/sourmash_tst_utils.py`

 * *Files identical despite different names*

### Comparing `sourmash_plugin_directsketch-0.1.0/tests/test-data/GCA_000175555.1.sig.gz` & `sourmash_plugin_directsketch-0.2.0/tests/test-data/GCA_000175555.1.sig.gz`

 * *Files identical despite different names*

### Comparing `sourmash_plugin_directsketch-0.1.0/tests/test-data/GCA_000961135.2.protein.sig.gz` & `sourmash_plugin_directsketch-0.2.0/tests/test-data/GCA_000961135.2.protein.sig.gz`

 * *Files identical despite different names*

### Comparing `sourmash_plugin_directsketch-0.1.0/tests/test-data/GCA_000961135.2.sig.gz` & `sourmash_plugin_directsketch-0.2.0/tests/test-data/GCA_000961135.2.sig.gz`

 * *Files identical despite different names*

### Comparing `sourmash_plugin_directsketch-0.1.0/tests/test-data/out_fastas/GCA_000175555.1_genomic.fna.gz` & `sourmash_plugin_directsketch-0.2.0/tests/test-data/out_fastas/GCA_000175555.1_genomic.fna.gz`

 * *Files identical despite different names*

### Comparing `sourmash_plugin_directsketch-0.1.0/tests/test-data/out_fastas/GCA_000961135.2_genomic.fna.gz` & `sourmash_plugin_directsketch-0.2.0/tests/test-data/out_fastas/GCA_000961135.2_genomic.fna.gz`

 * *Files identical despite different names*

### Comparing `sourmash_plugin_directsketch-0.1.0/tests/test-data/out_fastas/GCA_000961135.2_protein.faa.gz` & `sourmash_plugin_directsketch-0.2.0/tests/test-data/out_fastas/GCA_000961135.2_protein.faa.gz`

 * *Files identical despite different names*

### Comparing `sourmash_plugin_directsketch-0.1.0/tests/test-data/outputs/GCA_000175555.1_genomic.fna.gz` & `sourmash_plugin_directsketch-0.2.0/tests/test-data/outputs/GCA_000175555.1_genomic.fna.gz`

 * *Files identical despite different names*

### Comparing `sourmash_plugin_directsketch-0.1.0/tests/test-data/outputs/GCA_000337115.1_assembly_report.txt` & `sourmash_plugin_directsketch-0.2.0/tests/test-data/outputs/GCA_000337115.1_assembly_report.txt`

 * *Files identical despite different names*

### Comparing `sourmash_plugin_directsketch-0.1.0/tests/test-data/outputs/GCA_000337115.1_genomic.fna.gz` & `sourmash_plugin_directsketch-0.2.0/tests/test-data/outputs/GCA_000337115.1_genomic.fna.gz`

 * *Files identical despite different names*

### Comparing `sourmash_plugin_directsketch-0.1.0/tests/test-data/outputs/GCA_000337115.1_md5checksums.txt` & `sourmash_plugin_directsketch-0.2.0/tests/test-data/outputs/GCA_000337115.1_md5checksums.txt`

 * *Files identical despite different names*

### Comparing `sourmash_plugin_directsketch-0.1.0/tests/test-data/outputs/GCA_000337115.1_protein.faa.gz` & `sourmash_plugin_directsketch-0.2.0/tests/test-data/outputs/GCA_000337115.1_protein.faa.gz`

 * *Files identical despite different names*

### Comparing `sourmash_plugin_directsketch-0.1.0/tests/test-data/outputs/GCA_000961135.2_assembly_report.txt` & `sourmash_plugin_directsketch-0.2.0/out_fastas/GCA_000961135.2_assembly_report.txt`

 * *Files identical despite different names*

### Comparing `sourmash_plugin_directsketch-0.1.0/tests/test-data/outputs/GCA_000961135.2_genomic.fna.gz` & `sourmash_plugin_directsketch-0.2.0/tests/test-data/outputs/GCA_000961135.2_genomic.fna.gz`

 * *Files identical despite different names*

### Comparing `sourmash_plugin_directsketch-0.1.0/tests/test-data/outputs/GCA_000961135.2_md5checksums.txt` & `sourmash_plugin_directsketch-0.2.0/tests/test-data/outputs/GCA_000961135.2_md5checksums.txt`

 * *Files identical despite different names*

### Comparing `sourmash_plugin_directsketch-0.1.0/tests/test-data/outputs/GCA_000961135.2_protein.faa.gz` & `sourmash_plugin_directsketch-0.2.0/tests/test-data/outputs/GCA_000961135.2_protein.faa.gz`

 * *Files identical despite different names*

### Comparing `sourmash_plugin_directsketch-0.1.0/tests/test-data/outputs/GCA_001950595.1_genomic.fna.gz` & `sourmash_plugin_directsketch-0.2.0/tests/test-data/outputs/GCA_001950595.1_genomic.fna.gz`

 * *Files identical despite different names*

### Comparing `sourmash_plugin_directsketch-0.1.0/tests/test_gbsketch.py` & `sourmash_plugin_directsketch-0.2.0/tests/test_gbsketch.py`

 * *Files identical despite different names*

### Comparing `sourmash_plugin_directsketch-0.1.0/Cargo.lock` & `sourmash_plugin_directsketch-0.2.0/Cargo.lock`

 * *Files 3% similar despite different names*

```diff
@@ -60,50 +60,44 @@
 checksum = "cab112f0a86d568ea0e627cc1d6be74a1e9cd55214684db5561995f6dad897c6"
 dependencies = [
  "num-traits",
 ]
 
 [[package]]
 name = "async-compression"
-version = "0.3.15"
+version = "0.4.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "942c7cd7ae39e91bde4820d74132e9862e62c2f386c3aa90ccf55949f5bad63a"
+checksum = "4e9eabd7a98fe442131a17c316bd9349c43695e49e730c3c8e12cfb5f4da2693"
 dependencies = [
  "bzip2",
+ "deflate64",
  "flate2",
  "futures-core",
+ "futures-io",
  "memchr",
  "pin-project-lite",
- "tokio",
  "xz2",
- "zstd 0.11.2+zstd.1.5.2",
- "zstd-safe 5.0.2+zstd.1.5.2",
-]
-
-[[package]]
-name = "async_io_utilities"
-version = "0.1.4"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9b20cffc5590f4bf33f05f97a3ea587feba9c50d20325b401daa096b92ff7da0"
-dependencies = [
- "tokio",
+ "zstd 0.13.1",
+ "zstd-safe 7.1.0",
 ]
 
 [[package]]
 name = "async_zip"
-version = "0.0.6"
+version = "0.0.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "998dba685506ca6f05f5a54ece5938eb50ce047c7badd9d0e65327f33426b3aa"
+checksum = "00b9f7252833d5ed4b00aa9604b563529dd5e11de9c23615de2dcdf91eb87b52"
 dependencies = [
  "async-compression",
- "async_io_utilities",
  "chrono",
  "crc32fast",
+ "futures-lite",
+ "pin-project",
  "thiserror",
  "tokio",
+ "tokio-util",
 ]
 
 [[package]]
 name = "autocfg"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f1fdabc7756949593fe60f30ec81974b613357de856987752631dea1e3394c80"
@@ -349,14 +343,20 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5efa2b3d7902f4b634a20cae3c9c4e6209dc4779feb6863329607560143efa70"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
+name = "deflate64"
+version = "0.1.8"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "83ace6c86376be0b6cdcf3fb41882e81d94b31587573d1cfa9d01cd06bba210d"
+
+[[package]]
 name = "either"
 version = "1.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a47c1c47d2f5964e29c61246e81db715514cd532db6b5116a25ea3c03d6780a2"
 
 [[package]]
 name = "encoding_rs"
@@ -444,29 +444,86 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e13624c2627564efccf4934284bdd98cbaa14e79b0b5a141218e507b3a823456"
 dependencies = [
  "percent-encoding",
 ]
 
 [[package]]
+name = "futures"
+version = "0.3.30"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "645c6916888f6cb6350d2550b80fb63e734897a8498abe35cfb732b6487804b0"
+dependencies = [
+ "futures-channel",
+ "futures-core",
+ "futures-executor",
+ "futures-io",
+ "futures-sink",
+ "futures-task",
+ "futures-util",
+]
+
+[[package]]
 name = "futures-channel"
 version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "eac8f7d7865dcb88bd4373ab671c8cf4508703796caa2b1985a9ca867b3fcb78"
 dependencies = [
  "futures-core",
+ "futures-sink",
 ]
 
 [[package]]
 name = "futures-core"
 version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dfc6580bb841c5a68e9ef15c77ccc837b40a7504914d52e47b8b0e9bbda25a1d"
 
 [[package]]
+name = "futures-executor"
+version = "0.3.30"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a576fc72ae164fca6b9db127eaa9a9dda0d61316034f33a0a0d4eda41f02b01d"
+dependencies = [
+ "futures-core",
+ "futures-task",
+ "futures-util",
+]
+
+[[package]]
+name = "futures-io"
+version = "0.3.30"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a44623e20b9681a318efdd71c299b6b222ed6f231972bfe2f224ebad6311f0c1"
+
+[[package]]
+name = "futures-lite"
+version = "2.3.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "52527eb5074e35e9339c6b4e8d12600c7128b68fb25dcb9fa9dec18f7c25f3a5"
+dependencies = [
+ "fastrand",
+ "futures-core",
+ "futures-io",
+ "parking",
+ "pin-project-lite",
+]
+
+[[package]]
+name = "futures-macro"
+version = "0.3.30"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "87750cf4b7a4c0625b1529e4c543c2182106e4dedc60a2a6455e00d212c489ac"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn 2.0.60",
+]
+
+[[package]]
 name = "futures-sink"
 version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9fb8e00e87438d937621c1c6269e53f536c14d3fbd6a042bb24879e57d474fb5"
 
 [[package]]
 name = "futures-task"
@@ -476,18 +533,24 @@
 
 [[package]]
 name = "futures-util"
 version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3d6401deb83407ab3da39eba7e33987a73c3df0c82b4bb5813ee871c19c41d48"
 dependencies = [
+ "futures-channel",
  "futures-core",
+ "futures-io",
+ "futures-macro",
+ "futures-sink",
  "futures-task",
+ "memchr",
  "pin-project-lite",
  "pin-utils",
+ "slab",
 ]
 
 [[package]]
 name = "getrandom"
 version = "0.2.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "94b22e06ecb0110981051723910cbf0b5f5e09a2062dd7663334ee79a9d1286c"
@@ -1112,14 +1175,20 @@
  "proc-macro2",
  "proc-macro2-diagnostics",
  "quote",
  "syn 2.0.60",
 ]
 
 [[package]]
+name = "parking"
+version = "2.2.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "bb813b8af86854136c6922af0598d719255ecb2179515e6e7730d468f05c9cae"
+
+[[package]]
 name = "parking_lot"
 version = "0.12.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7e4af0ca4f6caed20e900d564c242b8e5d4903fdacf31d3daf527b66fe6f42fb"
 dependencies = [
  "lock_api",
  "parking_lot_core",
@@ -1478,18 +1547,20 @@
  "serde",
  "serde_json",
  "serde_urlencoded",
  "sync_wrapper",
  "system-configuration",
  "tokio",
  "tokio-native-tls",
+ "tokio-util",
  "tower-service",
  "url",
  "wasm-bindgen",
  "wasm-bindgen-futures",
+ "wasm-streams",
  "web-sys",
  "winreg",
 ]
 
 [[package]]
 name = "roaring"
 version = "0.10.3"
@@ -1592,26 +1663,26 @@
 dependencies = [
  "core-foundation-sys",
  "libc",
 ]
 
 [[package]]
 name = "serde"
-version = "1.0.198"
+version = "1.0.200"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9846a40c979031340571da2545a4e5b7c4163bdae79b301d5f86d03979451fcc"
+checksum = "ddc6f9cc94d67c0e21aaf7eda3a010fd3af78ebf6e096aa6e2e13c79749cce4f"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.198"
+version = "1.0.200"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e88edab869b01783ba905e7d0153f9fc1a6505a96e4ad3018011eedb838566d9"
+checksum = "856f046b9400cee3c8c94ed572ecdb752444c24528c035cd35882aad6f492bcb"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 2.0.60",
 ]
 
 [[package]]
@@ -1740,32 +1811,38 @@
  "vec-collections",
  "wasm-bindgen",
  "web-sys",
 ]
 
 [[package]]
 name = "sourmash_plugin_directsketch"
-version = "0.1.0"
+version = "0.2.0"
 dependencies = [
  "anyhow",
  "async_zip",
  "camino",
+ "chrono",
  "csv",
+ "futures",
+ "lazy_static",
+ "md5",
  "needletail",
  "niffler",
  "openssl",
  "pyo3",
+ "pyo3-build-config",
  "rayon",
  "regex",
  "reqwest",
  "serde",
  "serde_json",
  "simple-error",
  "sourmash",
  "tokio",
+ "tokio-util",
 ]
 
 [[package]]
 name = "static_assertions"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a2eb9349b6444b326872e140eb1cf5e7c522154d69e7a0ffb0fb81c06b37543f"
@@ -1932,24 +2009,24 @@
 dependencies = [
  "native-tls",
  "tokio",
 ]
 
 [[package]]
 name = "tokio-util"
-version = "0.7.10"
+version = "0.7.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5419f34732d9eb6ee4c3578b7989078579b7f039cbbb9ca2c4da015749371e15"
+checksum = "9cf6b47b3771c49ac75ad09a6162f53ad4b8088b76ac60e8ec1455b31a189fe1"
 dependencies = [
  "bytes",
  "futures-core",
+ "futures-io",
  "futures-sink",
  "pin-project-lite",
  "tokio",
- "tracing",
 ]
 
 [[package]]
 name = "tower"
 version = "0.4.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b8fa9be0de6cf49e536ce1851f987bd21a43b771b09473c3549a6c853db37c1c"
@@ -2184,14 +2261,27 @@
 [[package]]
 name = "wasm-bindgen-shared"
 version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "af190c94f2773fdb3729c55b007a722abb5384da03bc0986df4c289bf5567e96"
 
 [[package]]
+name = "wasm-streams"
+version = "0.4.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b65dc4c90b63b118468cf747d8bf3566c1913ef60be765b5730ead9e0a3ba129"
+dependencies = [
+ "futures-util",
+ "js-sys",
+ "wasm-bindgen",
+ "wasm-bindgen-futures",
+ "web-sys",
+]
+
+[[package]]
 name = "web-sys"
 version = "0.3.69"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "77afa9a11836342370f4817622a2f0f418b134426d91a82dfb48f532d2ec13ef"
 dependencies = [
  "js-sys",
  "wasm-bindgen",
@@ -2378,47 +2468,46 @@
 name = "yansi"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "cfe53a6657fd280eaa890a3bc59152892ffa3e30101319d168b781ed6529b049"
 
 [[package]]
 name = "zstd"
-version = "0.11.2+zstd.1.5.2"
+version = "0.12.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "20cc960326ece64f010d2d2107537f26dc589a6573a316bd5b1dba685fa5fde4"
+checksum = "1a27595e173641171fc74a1232b7b1c7a7cb6e18222c11e9dfb9888fa424c53c"
 dependencies = [
- "zstd-safe 5.0.2+zstd.1.5.2",
+ "zstd-safe 6.0.6",
 ]
 
 [[package]]
 name = "zstd"
-version = "0.12.4"
+version = "0.13.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1a27595e173641171fc74a1232b7b1c7a7cb6e18222c11e9dfb9888fa424c53c"
+checksum = "2d789b1514203a1120ad2429eae43a7bd32b90976a7bb8a05f7ec02fa88cc23a"
 dependencies = [
- "zstd-safe 6.0.6",
+ "zstd-safe 7.1.0",
 ]
 
 [[package]]
 name = "zstd-safe"
-version = "5.0.2+zstd.1.5.2"
+version = "6.0.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1d2a5585e04f9eea4b2a3d1eca508c4dee9592a89ef6f450c11719da0726f4db"
+checksum = "ee98ffd0b48ee95e6c5168188e44a54550b1564d9d530ee21d5f0eaed1069581"
 dependencies = [
  "libc",
  "zstd-sys",
 ]
 
 [[package]]
 name = "zstd-safe"
-version = "6.0.6"
+version = "7.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ee98ffd0b48ee95e6c5168188e44a54550b1564d9d530ee21d5f0eaed1069581"
+checksum = "1cd99b45c6bc03a018c8b8a86025678c87e55526064e38f9df301989dce7ec0a"
 dependencies = [
- "libc",
  "zstd-sys",
 ]
 
 [[package]]
 name = "zstd-sys"
 version = "2.0.10+zstd.1.5.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
```

### Comparing `sourmash_plugin_directsketch-0.1.0/pyproject.toml` & `sourmash_plugin_directsketch-0.2.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -19,20 +19,21 @@
 build-backend = "maturin"
 
 [project.entry-points."sourmash.cli_script"]
 gbsketch = "sourmash_plugin_directsketch:Download_and_Sketch_Assemblies"
 
 [project.optional-dependencies]
 test = [
-  "pytest>=6.2.4,<8.2.0",
+  "pytest>=6.2.4,<8.3.0",
   "pytest-cov>=2.12,<6.0",
   "pytest-xdist",
 ]
 
 [tool.maturin]
 python-source = "src/python"
+features = ["pyo3/extension-module"]
 
 [tool.maturin.target.x86_64-apple-darwin]
 macos-deployment-target = "10.14"
 
 [metadata]
 license = { text = "GNU Affero General Public License v3" }
```

### Comparing `sourmash_plugin_directsketch-0.1.0/PKG-INFO` & `sourmash_plugin_directsketch-0.2.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,32 @@
 Metadata-Version: 2.3
 Name: sourmash_plugin_directsketch
-Version: 0.1.0
+Version: 0.2.0
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: sourmash >=4.8.5, <5
-Requires-Dist: pytest >=6.2.4, <8.2.0 ; extra == 'test'
+Requires-Dist: pytest >=6.2.4, <8.3.0 ; extra == 'test'
 Requires-Dist: pytest-cov >=2.12, <6.0 ; extra == 'test'
 Requires-Dist: pytest-xdist ; extra == 'test'
 Provides-Extra: test
 License-File: LICENSE
 Summary: Download and Sketch GenBank Assembly Datasets
 Author: N. Tessa Pierce-Ward
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
 # sourmash_plugin_directsketch
 
 ## Installation
 
-For now, git clone the repository and cd in.
 ```
-mamba env create -f environment.yml
-pip install -e .
+pip install sourmash_plugin_directsketch
 ```
 
-> When it's released, you'll be able to:
-> ```
-> pip install sourmash_plugin_directsketch
-> ```
-
 ## Usage
 First, create a file, e.g. `acc.csv` with GenBank identifiers and sketch names.
 ```
 ident,name
 GCA_000961135.2,GCA_000961135.2 Candidatus Aramenus sulfurataquae isolate AZ1-45
 GCA_000175555.1,GCA_000175555.1 ACUK01000506.1 Saccharolobus solfataricus 98/2
 ```
```

