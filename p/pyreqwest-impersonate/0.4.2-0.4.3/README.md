# Comparing `tmp/pyreqwest_impersonate-0.4.2.tar.gz` & `tmp/pyreqwest_impersonate-0.4.3.tar.gz`

## Comparing `pyreqwest_impersonate-0.4.2.tar` & `pyreqwest_impersonate-0.4.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      947 1970-01-01 00:00:00.000000 pyreqwest_impersonate-0.4.2/Cargo.toml
--rw-r--r--   0     1001      127     7984 2024-05-05 16:43:38.000000 pyreqwest_impersonate-0.4.2/.github/workflows/CI.yml
--rw-r--r--   0     1001      127      766 2024-05-05 16:43:38.000000 pyreqwest_impersonate-0.4.2/.gitignore
--rw-r--r--   0     1001      127     7989 2024-05-05 16:43:38.000000 pyreqwest_impersonate-0.4.2/README.md
--rw-r--r--   0     1001      127      343 2024-05-05 16:43:38.000000 pyreqwest_impersonate-0.4.2/benchmark/README.md
--rw-r--r--   0     1001      127     3484 2024-05-05 16:43:38.000000 pyreqwest_impersonate-0.4.2/benchmark/benchmark.py
--rw-r--r--   0     1001      127     3719 2024-05-05 16:43:38.000000 pyreqwest_impersonate-0.4.2/benchmark/generate_image.py
--rw-r--r--   0     1001      127      144 2024-05-05 16:43:38.000000 pyreqwest_impersonate-0.4.2/benchmark/requirements.txt
--rw-r--r--   0     1001      127      990 2024-05-05 16:43:38.000000 pyreqwest_impersonate-0.4.2/benchmark/server.py
--rw-r--r--   0     1001      127    84789 2024-05-05 16:43:38.000000 pyreqwest_impersonate-0.4.2/benchmark.jpg
--rw-r--r--   0     1001      127    26365 2024-05-05 16:43:38.000000 pyreqwest_impersonate-0.4.2/src/lib.rs
--rw-r--r--   0     1001      127     3036 2024-05-05 16:43:38.000000 pyreqwest_impersonate-0.4.2/src/response.rs
--rw-r--r--   0     1001      127     3830 2024-05-05 16:43:38.000000 pyreqwest_impersonate-0.4.2/tests/test_client.py
--rw-r--r--   0     1001      127     5370 2024-05-05 16:43:38.000000 pyreqwest_impersonate-0.4.2/tests/test_defs.py
--rw-r--r--   0     1001      127    41269 2024-05-05 16:43:38.000000 pyreqwest_impersonate-0.4.2/Cargo.lock
--rw-r--r--   0     1001      127     1151 2024-05-05 16:43:38.000000 pyreqwest_impersonate-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     9058 1970-01-01 00:00:00.000000 pyreqwest_impersonate-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1002 1970-01-01 00:00:00.000000 pyreqwest_impersonate-0.4.3/Cargo.toml
+-rw-r--r--   0     1001      127     8345 2024-05-08 00:05:27.000000 pyreqwest_impersonate-0.4.3/.github/workflows/CI.yml
+-rw-r--r--   0     1001      127      766 2024-05-08 00:05:27.000000 pyreqwest_impersonate-0.4.3/.gitignore
+-rw-r--r--   0     1001      127     8506 2024-05-08 00:05:27.000000 pyreqwest_impersonate-0.4.3/README.md
+-rw-r--r--   0     1001      127      343 2024-05-08 00:05:27.000000 pyreqwest_impersonate-0.4.3/benchmark/README.md
+-rw-r--r--   0     1001      127     3484 2024-05-08 00:05:27.000000 pyreqwest_impersonate-0.4.3/benchmark/benchmark.py
+-rw-r--r--   0     1001      127     3719 2024-05-08 00:05:27.000000 pyreqwest_impersonate-0.4.3/benchmark/generate_image.py
+-rw-r--r--   0     1001      127      144 2024-05-08 00:05:27.000000 pyreqwest_impersonate-0.4.3/benchmark/requirements.txt
+-rw-r--r--   0     1001      127      990 2024-05-08 00:05:27.000000 pyreqwest_impersonate-0.4.3/benchmark/server.py
+-rw-r--r--   0     1001      127   112338 2024-05-08 00:05:27.000000 pyreqwest_impersonate-0.4.3/benchmark.jpg
+-rw-r--r--   0     1001      127    30089 2024-05-08 00:05:27.000000 pyreqwest_impersonate-0.4.3/src/lib.rs
+-rw-r--r--   0     1001      127     3036 2024-05-08 00:05:27.000000 pyreqwest_impersonate-0.4.3/src/response.rs
+-rw-r--r--   0     1001      127     6274 2024-05-08 00:05:27.000000 pyreqwest_impersonate-0.4.3/tests/test_client.py
+-rw-r--r--   0     1001      127     8329 2024-05-08 00:05:27.000000 pyreqwest_impersonate-0.4.3/tests/test_defs.py
+-rw-r--r--   0     1001      127    41289 2024-05-08 00:05:27.000000 pyreqwest_impersonate-0.4.3/Cargo.lock
+-rw-r--r--   0     1001      127     1151 2024-05-08 00:05:27.000000 pyreqwest_impersonate-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0     9575 1970-01-01 00:00:00.000000 pyreqwest_impersonate-0.4.3/PKG-INFO
```

### Comparing `pyreqwest_impersonate-0.4.2/Cargo.toml` & `pyreqwest_impersonate-0.4.3/Cargo.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "pyreqwest_impersonate"
-version = "0.4.2"
+version = "0.4.3"
 edition = "2021"
 description = "HTTP client that can impersonate web browsers, mimicking their headers and `TLS/JA3/JA4/HTTP2` fingerprints"
 authors = ["deedy5"]
 
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
@@ -21,14 +21,15 @@
     "multipart",  # to send a multipart/form-data body
     "socks",
     "gzip",
     "brotli",
     "deflate",
 ] }
 encoding_rs = { version = "0.8" }
+form_urlencoded = "1"  # to serialize `data` parameter
 pythonize = "0.21"
 serde_json = "1"
 tokio = { version = "1", features = ["fs", "rt"] }
 
 [profile.release]
 codegen-units = 1
 lto = "fat"
```

### Comparing `pyreqwest_impersonate-0.4.2/.github/workflows/CI.yml` & `pyreqwest_impersonate-0.4.3/.github/workflows/CI.yml`

 * *Files 6% similar despite different names*

```diff
@@ -185,22 +185,22 @@
           args: --release --out dist
           sccache: 'true'
       - name: Upload wheels
         uses: actions/upload-artifact@v4
         with:
           name: wheels-macos-${{ matrix.platform.target }}
           path: dist
-      - name: pytest
-        if: ${{ !startsWith(matrix.platform.target, 'aarch64') }}
-        shell: bash
-        run: |
-          set -e
-          pip install pyreqwest_impersonate --find-links dist --force-reinstall
-          pip install pytest
-          pytest
+      #- name: pytest
+      #  if: ${{ !startsWith(matrix.platform.target, 'aarch64') }}
+      #  shell: bash
+      #  run: |
+      #    set -e
+      #    pip install pyreqwest_impersonate --find-links dist --force-reinstall
+      #    pip install pytest
+      #    pytest
 
   sdist:
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v4
       - name: Build sdist
         uses: PyO3/maturin-action@v1
@@ -254,8 +254,14 @@
       - name: Generate image and commit
         run: |
           python benchmark/generate_image.py
           git config --global user.name 'GitHub Actions'
           git config --global user.email 'actions@github.com'
           git add \*.jpg
           git commit -m "Update generated image" || echo "No changes to commit"
+          # Reattach HEAD to the branch that initiated the workflow
+          if [[ "${{ github.event_name }}" == "pull_request" ]]; then
+            git checkout "${{ github.head_ref }}"
+          elif [[ "${{ github.event_name }}" == "create" && "${{ github.event.action }}" == "tag" ]]; then
+            git checkout "${{ github.ref }}"
+          fi
           git push https://${{ secrets.PUSH_TOKEN }}@github.com/${{ github.repository }}
```

### Comparing `pyreqwest_impersonate-0.4.2/.gitignore` & `pyreqwest_impersonate-0.4.3/.gitignore`

 * *Files identical despite different names*

### Comparing `pyreqwest_impersonate-0.4.2/README.md` & `pyreqwest_impersonate-0.4.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -55,74 +55,93 @@
         params (dict, optional): Default query parameters to include in all requests. Default is None.
         headers (dict, optional): Default headers to send with requests. If `impersonate` is set, this will be ignored.
         timeout (float, optional): HTTP request timeout in seconds. Default is 30.
         cookie_store (bool, optional): Enable a persistent cookie store. Received cookies will be preserved and included 
             in additional requests. Default is True.
         referer (bool, optional): Enable or disable automatic setting of the `Referer` header. Default is True.
         proxy (str, optional): Proxy URL for HTTP requests. Example: "socks5://127.0.0.1:9150". Default is None.
-        impersonate (str, optional): Entity to impersonate. Example: "chrome_123". Default is None.
+        impersonate (str, optional): Entity to impersonate. Example: "chrome_124". Default is None.
             Chrome: "chrome_99","chrome_100","chrome_101","chrome_104","chrome_105","chrome_106","chrome_108", 
                 "chrome_107","chrome_109","chrome_114","chrome_116","chrome_117","chrome_118","chrome_119", 
-                "chrome_120","chrome_123"
-            Safari: "safari_ios_17_2","safari_12","safari_15_3","safari_15_5","safari_15_6_1","safari_16","safari_16_5",
-                "safari_17_2_1","safari17_4_1"
+                "chrome_120","chrome_123","chrome_124"
+            Safari: "safari_12","safari_15_3","safari_15_5","safari_15_6_1","safari_16","safari_16_5",
+                "safari_17_2_1"
             OkHttp: "okhttp_3_9","okhttp_3_11","okhttp_3_13","okhttp_3_14","okhttp_4_9","okhttp_4_10","okhttp_5"
-            Edge: "edge_99","edge_101","edge_122"
+            Edge: "edge_99","edge_101","edge_120"
         follow_redirects (bool, optional): Whether to follow redirects. Default is True.
         max_redirects (int, optional): Maximum redirects to follow. Default 20. Applies if `follow_redirects` is True.
-        verify (bool, optional): Verify SSL certificates. Default is False.
+        verify (bool, optional): Verify SSL certificates. Default is True.
         http1 (bool, optional): Use only HTTP/1.1. Default is None.
         http2 (bool, optional): Use only HTTP/2. Default is None.
          
     """
 ```
 
 #### Client Methods
 
 The `Client` class provides a set of methods for making HTTP requests: `get`, `head`, `options`, `delete`, `post`, `put`, `patch`, each of which internally utilizes the `request()` method for execution. The parameters for these methods closely resemble those in `httpx`.
 ```python
-def get(url, params=None, headers=None, auth=None, auth_bearer=None, timeout=None):
+def get(
+    url: str, 
+    params: Optional[Dict[str, str]] = None, 
+    headers: Optional[Dict[str, str]] = None, 
+    auth: Optional[Tuple[str, Optional[str]]] = None, 
+    auth_bearer: Optional[str] = None, 
+    timeout: Optional[float] = 30,
+):
     """Performs a GET request to the specified URL.
 
     Args:
         url (str): The URL to which the request will be made.
         params (Optional[Dict[str, str]]): A map of query parameters to append to the URL. Default is None.
         headers (Optional[Dict[str, str]]): A map of HTTP headers to send with the request. Default is None.
         auth (Optional[Tuple[str, Optional[str]]]): A tuple containing the username and an optional password 
             for basic authentication. Default is None.
         auth_bearer (Optional[str]): A string representing the bearer token for bearer token authentication. Default is None.
         timeout (Optional[float]): The timeout for the request in seconds. Default is 30.
 
     """
 ```
 ```python
-def post(url, params=None, headers=None, content=None, data=None, files=None, auth=None, auth_bearer=None, timeout=None):
+def post(
+    url: str, 
+    params: Optional[Dict[str, str]] = None, 
+    headers: Optional[Dict[str, str]] = None, 
+    content: Optional[bytes] = None, 
+    data: Optional[Dict[str, str]] = None, 
+    json: Any = None, 
+    files: Optional[Dict[str, str]] = None, 
+    auth: Optional[Tuple[str, Optional[str]]] = None, 
+    auth_bearer: Optional[str] = None, 
+    timeout: Optional[float] = 30,
+):
     """Performs a POST request to the specified URL.
 
     Args:
         url (str): The URL to which the request will be made.
         params (Optional[Dict[str, str]]): A map of query parameters to append to the URL. Default is None.
         headers (Optional[Dict[str, str]]): A map of HTTP headers to send with the request. Default is None.
         content (Optional[bytes]): The content to send in the request body as bytes. Default is None.
         data (Optional[Dict[str, str]]): The form data to send in the request body. Default is None.
+        json (Any): A JSON serializable object to send in the request body. Default is None.
         files (Optional[Dict[str, str]]): A map of file fields to file paths to be sent as multipart/form-data. Default is None.
         auth (Optional[Tuple[str, Optional[str]]]): A tuple containing the username and an optional password 
             for basic authentication. Default is None.
         auth_bearer (Optional[str]): A string representing the bearer token for bearer token authentication. Default is None.
         timeout (Optional[float]): The timeout for the request in seconds. Default is 30.
 
     """
 ```
 
 #### Example
 
 ```python
 import pyreqwest_impersonate as pri
 
-client = pri.Client(impersonate="chrome_123")
+client = pri.Client(impersonate="chrome_124")
 
 # get request
 resp = client.get("https://tls.peet.ws/api/all")
 print(resp.json())
 
 # post request
 data = {"key1": "value1", "key2": "value2"}
@@ -135,13 +154,13 @@
 print(resp.status_code)
 print(resp.text)
 print(resp.url)
 
 # You can also use convenience functions that use a default Client instance under the hood:
 # pri.get() | pri.head() | pri.options() | pri.delete() | pri.post | pri.patch | pri.put
 # These functions can accept the `impersonate` parameter:
-resp = pri.get("https://httpbin.org/anything", impersonate="chrome_123")  
+resp = pri.get("https://httpbin.org/anything", impersonate="chrome_124")  
 ```
 ### II. AsyncClient
 
 TODO
```

### Comparing `pyreqwest_impersonate-0.4.2/benchmark/benchmark.py` & `pyreqwest_impersonate-0.4.3/benchmark/benchmark.py`

 * *Files identical despite different names*

### Comparing `pyreqwest_impersonate-0.4.2/benchmark/generate_image.py` & `pyreqwest_impersonate-0.4.3/benchmark/generate_image.py`

 * *Files identical despite different names*

### Comparing `pyreqwest_impersonate-0.4.2/benchmark/server.py` & `pyreqwest_impersonate-0.4.3/benchmark/server.py`

 * *Files identical despite different names*

### Comparing `pyreqwest_impersonate-0.4.2/src/lib.rs` & `pyreqwest_impersonate-0.4.3/src/lib.rs`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 use std::collections::HashMap;
 use std::str::FromStr;
 use std::sync::{Arc, OnceLock};
 use std::time::Duration;
 
+use form_urlencoded::Serializer;
 use pyo3::exceptions;
 use pyo3::prelude::*;
-use pyo3::types::{PyBytes, PyDict, PyString};
+use pyo3::types::{PyBytes, PyDict, PyList, PyString};
 use reqwest_impersonate::header::{HeaderMap, HeaderName, HeaderValue};
 use reqwest_impersonate::impersonate::Impersonate;
 use reqwest_impersonate::multipart;
 use reqwest_impersonate::redirect::Policy;
 use reqwest_impersonate::Method;
 use tokio::runtime::{self, Runtime};
 
@@ -23,14 +24,34 @@
         runtime::Builder::new_current_thread()
             .enable_all()
             .build()
             .unwrap()
     })
 }
 
+/// Converts a Python dictionary to a Rust HashMap.
+fn py_dict_to_hashmap(_py: Python, py_dict: &PyDict) -> PyResult<HashMap<String, Vec<String>>> {
+    let mut map = HashMap::new();
+    for (key, value) in py_dict.iter() {
+        let key: String = key.extract()?;
+        let values: Vec<String> = if let Ok(py_list) = value.downcast::<PyList>() {
+            // If the value is a list, extract each item as a String
+            py_list
+                .iter()
+                .map(|item| item.extract::<String>())
+                .collect::<PyResult<_>>()?
+        } else {
+            // If the value is not a list, treat it as a single-item list
+            vec![value.extract::<String>()?]
+        };
+        map.insert(key, values);
+    }
+    Ok(map)
+}
+
 #[pyclass]
 /// HTTP client that can impersonate web browsers.
 pub struct Client {
     client: Arc<reqwest_impersonate::Client>,
     auth: Option<(String, Option<String>)>,
     auth_bearer: Option<String>,
     params: Option<HashMap<String, String>>,
@@ -55,15 +76,15 @@
     ///         in additional requests. Default is `true`.
     /// * `referer` - Enable or disable automatic setting of the `Referer` header. Default is `true`.
     /// * `proxy` - An optional proxy URL for HTTP requests.
     /// * `timeout` - An optional timeout for HTTP requests in seconds.
     /// * `impersonate` - An optional entity to impersonate. Supported browsers and versions include Chrome, Safari, OkHttp, and Edge.
     /// * `follow_redirects` - A boolean to enable or disable following redirects. Default is `true`.
     /// * `max_redirects` - The maximum number of redirects to follow. Default is 20. Applies if `follow_redirects` is `true`.
-    /// * `verify` - An optional boolean indicating whether to verify SSL certificates. Default is `false`.
+    /// * `verify` - An optional boolean indicating whether to verify SSL certificates. Default is `true`.
     /// * `http1` - An optional boolean indicating whether to use only HTTP/1.1. Default is `false`.
     /// * `http2` - An optional boolean indicating whether to use only HTTP/2. Default is `false`.
     ///
     /// # Example
     ///
     /// ```
     /// from reqwest_impersonate import Client
@@ -162,15 +183,15 @@
         if follow_redirects.unwrap_or(true) {
             client_builder = client_builder.redirect(Policy::limited(max_redirects));
         } else {
             client_builder = client_builder.redirect(Policy::none());
         }
 
         // Verify
-        let verify = verify.unwrap_or(false);
+        let verify = verify.unwrap_or(true);
         if !verify {
             client_builder = client_builder.danger_accept_invalid_certs(true);
         }
 
         // Http version: http1 || http2
         match (http1, http2) {
             (Some(true), Some(true)) => {
@@ -203,14 +224,15 @@
     ///
     /// * `method` - The HTTP method to use (e.g., "GET", "POST").
     /// * `url` - The URL to which the request will be made.
     /// * `params` - A map of query parameters to append to the URL. Default is None.
     /// * `headers` - A map of HTTP headers to send with the request. Default is None.
     /// * `content` - The content to send in the request body as bytes. Default is None.
     /// * `data` - The form data to send in the request body. Default is None.
+    /// * `json` -  A JSON serializable object to send in the request body. Default is None.
     /// * `files` - A map of file fields to file paths to be sent as multipart/form-data. Default is None.
     /// * `auth` - A tuple containing the username and an optional password for basic authentication. Default is None.
     /// * `auth_bearer` - A string representing the bearer token for bearer token authentication. Default is None.
     /// * `timeout` - The timeout for the request in seconds. Default is 30.
     ///
     /// # Returns
     ///
@@ -223,24 +245,37 @@
         &self,
         py: Python,
         method: &str,
         url: &str,
         params: Option<HashMap<String, String>>,
         headers: Option<HashMap<String, String>>,
         content: Option<Vec<u8>>,
-        data: Option<HashMap<String, String>>,
+        data: Option<&Bound<'_, PyDict>>,
+        json: Option<&Bound<'_, PyDict>>,
         files: Option<HashMap<String, String>>,
         auth: Option<(String, Option<String>)>,
         auth_bearer: Option<String>,
         timeout: Option<f64>,
     ) -> PyResult<Response> {
         let client = Arc::clone(&self.client);
         let auth = auth.or(self.auth.clone());
         let auth_bearer = auth_bearer.or(self.auth_bearer.clone());
         let params = params.or(self.params.clone());
+        // Converts 'data' (if any) into a URL-encoded string for sending the data as `application/x-www-form-urlencoded` content type.
+        let data_str: Option<String> = data.map(|data_pydict| {
+            let data_map = py_dict_to_hashmap(py, data_pydict.as_gil_ref()).unwrap();
+            let mut serializer = Serializer::new(String::new());
+            let flattened_pairs = data_map.into_iter().flat_map(|(key, values)| {
+                values.into_iter().map(move |value| (key.to_owned(), value))
+            });
+            serializer.extend_pairs(flattened_pairs);
+            serializer.finish()
+        });
+        // Converts 'json' (if any) into a string for sending the data as `application/json` content type.
+        let json_str: Option<String> = json.map(|json_data| json_data.to_string());
 
         let future = async move {
             // Check if method is POST || PUT || PATCH
             let is_post_put_patch = method == "POST" || method == "PUT" || method == "PATCH";
 
             // Method
             let method = match method {
@@ -283,16 +318,24 @@
             // Only if method POST || PUT || PATCH
             if is_post_put_patch {
                 // Content
                 if let Some(content) = content {
                     request_builder = request_builder.body(content);
                 }
                 // Data
-                if let Some(data) = data {
-                    request_builder = request_builder.form(&data);
+                if let Some(url_encoded_data) = data_str {
+                    request_builder = request_builder
+                        .header("Content-Type", "application/x-www-form-urlencoded")
+                        .body(url_encoded_data);
+                }
+                // Json
+                if let Some(json_str) = json_str {
+                    request_builder = request_builder
+                        .header("Content-Type", "application/json")
+                        .body(json_str);
                 }
                 // Files
                 if let Some(files) = files {
                     let mut form = multipart::Form::new();
                     for (field, path) in files {
                         let file_content = tokio::fs::read(&path).await.map_err(|e| {
                             PyErr::new::<exceptions::PyException, _>(format!(
@@ -421,14 +464,15 @@
             "GET",
             url,
             params,
             headers,
             None,
             None,
             None,
+            None,
             auth,
             auth_bearer,
             timeout,
         )
     }
     fn head(
         &self,
@@ -445,14 +489,15 @@
             "HEAD",
             url,
             params,
             headers,
             None,
             None,
             None,
+            None,
             auth,
             auth_bearer,
             timeout,
         )
     }
     fn options(
         &self,
@@ -469,14 +514,15 @@
             "OPTIONS",
             url,
             params,
             headers,
             None,
             None,
             None,
+            None,
             auth,
             auth_bearer,
             timeout,
         )
     }
     fn delete(
         &self,
@@ -493,158 +539,216 @@
             "DELETE",
             url,
             params,
             headers,
             None,
             None,
             None,
+            None,
             auth,
             auth_bearer,
             timeout,
         )
     }
 
     fn post(
         &self,
         py: Python,
         url: &str,
         params: Option<HashMap<String, String>>,
         headers: Option<HashMap<String, String>>,
         content: Option<Vec<u8>>,
-        data: Option<HashMap<String, String>>,
+        data: Option<&Bound<'_, PyDict>>,
+        json: Option<&Bound<'_, PyDict>>,
         files: Option<HashMap<String, String>>,
         auth: Option<(String, Option<String>)>,
         auth_bearer: Option<String>,
         timeout: Option<f64>,
     ) -> PyResult<Response> {
         self.request(
             py,
             "POST",
             url,
             params,
             headers,
             content,
             data,
+            json,
             files,
             auth,
             auth_bearer,
             timeout,
         )
     }
     fn put(
         &self,
         py: Python,
         url: &str,
         params: Option<HashMap<String, String>>,
         headers: Option<HashMap<String, String>>,
         content: Option<Vec<u8>>,
-        data: Option<HashMap<String, String>>,
+        data: Option<&Bound<'_, PyDict>>,
+        json: Option<&Bound<'_, PyDict>>,
         files: Option<HashMap<String, String>>,
         auth: Option<(String, Option<String>)>,
         auth_bearer: Option<String>,
         timeout: Option<f64>,
     ) -> PyResult<Response> {
         self.request(
             py,
             "PUT",
             url,
             params,
             headers,
             content,
             data,
+            json,
             files,
             auth,
             auth_bearer,
             timeout,
         )
     }
     fn patch(
         &self,
         py: Python,
         url: &str,
         params: Option<HashMap<String, String>>,
         headers: Option<HashMap<String, String>>,
         content: Option<Vec<u8>>,
-        data: Option<HashMap<String, String>>,
+        data: Option<&Bound<'_, PyDict>>,
+        json: Option<&Bound<'_, PyDict>>,
         files: Option<HashMap<String, String>>,
         auth: Option<(String, Option<String>)>,
         auth_bearer: Option<String>,
         timeout: Option<f64>,
     ) -> PyResult<Response> {
         self.request(
             py,
             "PATCH",
             url,
             params,
             headers,
             content,
             data,
+            json,
             files,
             auth,
             auth_bearer,
             timeout,
         )
     }
 }
 
 /// Convenience functions that use a default Client instance under the hood
 #[pyfunction]
-fn get(
+fn request(
     py: Python,
+    method: &str,
     url: &str,
     params: Option<HashMap<String, String>>,
     headers: Option<HashMap<String, String>>,
+    content: Option<Vec<u8>>,
+    data: Option<&Bound<'_, PyDict>>,
+    json: Option<&Bound<'_, PyDict>>,
+    files: Option<HashMap<String, String>>,
     auth: Option<(String, Option<String>)>,
     auth_bearer: Option<String>,
     timeout: Option<f64>,
     impersonate: Option<&str>,
+    verify: Option<bool>,
 ) -> PyResult<Response> {
     let client = Client::new(
         None,
         None,
         None,
         None,
         None,
         None,
         None,
         None,
         impersonate,
         None,
         None,
+        verify,
+        None,
+        None,
+    )?;
+    client.request(
+        py,
+        method,
+        url,
+        params,
+        headers,
+        content,
+        data,
+        json,
+        files,
+        auth,
+        auth_bearer,
+        timeout,
+    )
+}
+
+#[pyfunction]
+fn get(
+    py: Python,
+    url: &str,
+    params: Option<HashMap<String, String>>,
+    headers: Option<HashMap<String, String>>,
+    auth: Option<(String, Option<String>)>,
+    auth_bearer: Option<String>,
+    timeout: Option<f64>,
+    impersonate: Option<&str>,
+    verify: Option<bool>,
+) -> PyResult<Response> {
+    let client = Client::new(
+        None,
+        None,
         None,
         None,
         None,
+        None,
+        None,
+        None,
+        impersonate,
+        None,
+        None,
+        verify,
+        None,
+        None,
     )?;
     client.get(py, url, params, headers, auth, auth_bearer, timeout)
 }
 
 #[pyfunction]
 fn head(
     py: Python,
     url: &str,
     params: Option<HashMap<String, String>>,
     headers: Option<HashMap<String, String>>,
     auth: Option<(String, Option<String>)>,
     auth_bearer: Option<String>,
     timeout: Option<f64>,
     impersonate: Option<&str>,
+    verify: Option<bool>,
 ) -> PyResult<Response> {
     let client = Client::new(
         None,
         None,
         None,
         None,
         None,
         None,
         None,
         None,
         impersonate,
         None,
         None,
-        None,
+        verify,
         None,
         None,
     )?;
     client.head(py, url, params, headers, auth, auth_bearer, timeout)
 }
 
 #[pyfunction]
@@ -653,28 +757,29 @@
     url: &str,
     params: Option<HashMap<String, String>>,
     headers: Option<HashMap<String, String>>,
     auth: Option<(String, Option<String>)>,
     auth_bearer: Option<String>,
     timeout: Option<f64>,
     impersonate: Option<&str>,
+    verify: Option<bool>,
 ) -> PyResult<Response> {
     let client = Client::new(
         None,
         None,
         None,
         None,
         None,
         None,
         None,
         None,
         impersonate,
         None,
         None,
-        None,
+        verify,
         None,
         None,
     )?;
     client.options(py, url, params, headers, auth, auth_bearer, timeout)
 }
 
 #[pyfunction]
@@ -683,169 +788,180 @@
     url: &str,
     params: Option<HashMap<String, String>>,
     headers: Option<HashMap<String, String>>,
     auth: Option<(String, Option<String>)>,
     auth_bearer: Option<String>,
     timeout: Option<f64>,
     impersonate: Option<&str>,
+    verify: Option<bool>,
 ) -> PyResult<Response> {
     let client = Client::new(
         None,
         None,
         None,
         None,
         None,
         None,
         None,
         None,
         impersonate,
         None,
         None,
-        None,
+        verify,
         None,
         None,
     )?;
     client.delete(py, url, params, headers, auth, auth_bearer, timeout)
 }
 
 #[pyfunction]
 fn post(
     py: Python,
     url: &str,
     params: Option<HashMap<String, String>>,
     headers: Option<HashMap<String, String>>,
     content: Option<Vec<u8>>,
-    data: Option<HashMap<String, String>>,
+    data: Option<&Bound<'_, PyDict>>,
+    json: Option<&Bound<'_, PyDict>>,
     files: Option<HashMap<String, String>>,
     auth: Option<(String, Option<String>)>,
     auth_bearer: Option<String>,
     timeout: Option<f64>,
     impersonate: Option<&str>,
+    verify: Option<bool>,
 ) -> PyResult<Response> {
     let client = Client::new(
         None,
         None,
         None,
         None,
         None,
         None,
         None,
         None,
         impersonate,
         None,
         None,
-        None,
+        verify,
         None,
         None,
     )?;
     client.post(
         py,
         url,
         params,
         headers,
         content,
         data,
+        json,
         files,
         auth,
         auth_bearer,
         timeout,
     )
 }
 
 #[pyfunction]
 fn put(
     py: Python,
     url: &str,
     params: Option<HashMap<String, String>>,
     headers: Option<HashMap<String, String>>,
     content: Option<Vec<u8>>,
-    data: Option<HashMap<String, String>>,
+    data: Option<&Bound<'_, PyDict>>,
+    json: Option<&Bound<'_, PyDict>>,
     files: Option<HashMap<String, String>>,
     auth: Option<(String, Option<String>)>,
     auth_bearer: Option<String>,
     timeout: Option<f64>,
     impersonate: Option<&str>,
+    verify: Option<bool>,
 ) -> PyResult<Response> {
     let client = Client::new(
         None,
         None,
         None,
         None,
         None,
         None,
         None,
         None,
         impersonate,
         None,
         None,
-        None,
+        verify,
         None,
         None,
     )?;
     client.put(
         py,
         url,
         params,
         headers,
         content,
         data,
+        json,
         files,
         auth,
         auth_bearer,
         timeout,
     )
 }
 
 #[pyfunction]
 fn patch(
     py: Python,
     url: &str,
     params: Option<HashMap<String, String>>,
     headers: Option<HashMap<String, String>>,
     content: Option<Vec<u8>>,
-    data: Option<HashMap<String, String>>,
+    data: Option<&Bound<'_, PyDict>>,
+    json: Option<&Bound<'_, PyDict>>,
     files: Option<HashMap<String, String>>,
     auth: Option<(String, Option<String>)>,
     auth_bearer: Option<String>,
     timeout: Option<f64>,
     impersonate: Option<&str>,
+    verify: Option<bool>,
 ) -> PyResult<Response> {
     let client = Client::new(
         None,
         None,
         None,
         None,
         None,
         None,
         None,
         None,
         impersonate,
         None,
         None,
-        None,
+        verify,
         None,
         None,
     )?;
     client.patch(
         py,
         url,
         params,
         headers,
         content,
         data,
+        json,
         files,
         auth,
         auth_bearer,
         timeout,
     )
 }
 
 #[pymodule]
 fn pyreqwest_impersonate(_py: Python, m: &Bound<'_, PyModule>) -> PyResult<()> {
     m.add_class::<Client>()?;
+    m.add_function(wrap_pyfunction!(request, m)?)?;
     m.add_function(wrap_pyfunction!(get, m)?)?;
     m.add_function(wrap_pyfunction!(head, m)?)?;
     m.add_function(wrap_pyfunction!(options, m)?)?;
     m.add_function(wrap_pyfunction!(delete, m)?)?;
     m.add_function(wrap_pyfunction!(post, m)?)?;
     m.add_function(wrap_pyfunction!(patch, m)?)?;
     m.add_function(wrap_pyfunction!(put, m)?)?;
```

### Comparing `pyreqwest_impersonate-0.4.2/src/response.rs` & `pyreqwest_impersonate-0.4.3/src/response.rs`

 * *Files identical despite different names*

### Comparing `pyreqwest_impersonate-0.4.2/tests/test_client.py` & `pyreqwest_impersonate-0.4.3/tests/test_client.py`

 * *Files 26% similar despite different names*

```diff
@@ -31,14 +31,37 @@
     json_data = response.json()
     assert json_data["headers"]["X-Test"] == "test"
     assert json_data["headers"]["Authorization"] == "Basic dXNlcjpwYXNzd29yZA=="
     assert json_data["args"] == {"x": "aaa", "y": "bbb"}
 
 
 @retry()
+def test_client_request_get():
+    client = Client(verify=False)
+    auth_bearer = "bearerXXXXXXXXXXXXXXXXXXXX"
+    headers = {"X-Test": "test"}
+    params = {"x": "aaa", "y": "bbb"}
+    response = client.request(
+        "GET",
+        "https://httpbin.org/anything",
+        auth_bearer=auth_bearer,
+        headers=headers,
+        params=params,
+    )
+    assert response.status_code == 200
+    json_data = response.json()
+    assert json_data["method"] == "GET"
+    assert json_data["headers"]["X-Test"] == "test"
+    assert json_data["headers"]["Authorization"] == "Bearer bearerXXXXXXXXXXXXXXXXXXXX"
+    assert json_data["args"] == {"x": "aaa", "y": "bbb"}
+    assert "Bearer bearerXXXXXXXXXXXXXXXXXXXX" in response.text
+    assert b"Bearer bearerXXXXXXXXXXXXXXXXXXXX" in response.content
+
+
+@retry()
 def test_client_get():
     client = Client(verify=False)
     auth_bearer = "bearerXXXXXXXXXXXXXXXXXXXX"
     headers = {"X-Test": "test"}
     params = {"x": "aaa", "y": "bbb"}
     response = client.get(
         "https://httpbin.org/anything",
@@ -99,16 +122,62 @@
     assert json_data["headers"]["X-Test"] == "test"
     assert json_data["headers"]["Authorization"] == "Bearer bearerXXXXXXXXXXXXXXXXXXXX"
     assert json_data["args"] == {"x": "aaa", "y": "bbb"}
     assert json_data["form"] == {"key1": "value1", "key2": "value2"}
 
 
 @retry()
-def test_client_impersonate():
-    client = Client(impersonate="chrome_123", verify=False)
+def test_client_post_data2():
+    client = Client(verify=False)
+    auth_bearer = "bearerXXXXXXXXXXXXXXXXXXXX"
+    headers = {"X-Test": "test"}
+    params = {"x": "aaa", "y": "bbb"}
+    data = {"key1": "value1", "key2": ["value2_1", "value2_2"]}
+    response = client.post(
+        "https://httpbin.org/anything",
+        auth_bearer=auth_bearer,
+        headers=headers,
+        params=params,
+        data=data,
+    )
+    assert response.status_code == 200
+    json_data = response.json()
+    assert json_data["method"] == "POST"
+    assert json_data["headers"]["X-Test"] == "test"
+    assert json_data["headers"]["Authorization"] == "Bearer bearerXXXXXXXXXXXXXXXXXXXX"
+    assert json_data["args"] == {"x": "aaa", "y": "bbb"}
+    assert json_data["form"] == {"key1": "value1", "key2": ["value2_1", "value2_2"]}
+
+
+@retry()
+def test_client_post_json():
+    client = Client(verify=False)
+    auth_bearer = "bearerXXXXXXXXXXXXXXXXXXXX"
+    headers = {"X-Test": "test"}
+    params = {"x": "aaa", "y": "bbb"}
+    data = {"key1": "value1", "key2": "value2"}
+    response = client.post(
+        "https://httpbin.org/anything",
+        auth_bearer=auth_bearer,
+        headers=headers,
+        params=params,
+        json=data,
+    )
+    assert response.status_code == 200
+    json_data = response.json()
+    assert json_data["method"] == "POST"
+    assert json_data["headers"]["X-Test"] == "test"
+    assert json_data["headers"]["Authorization"] == "Bearer bearerXXXXXXXXXXXXXXXXXXXX"
+    assert json_data["args"] == {"x": "aaa", "y": "bbb"}
+    assert json_data["data"] == "{\'key1\': \'value1\', \'key2\': \'value2\'}"
+
+
+@retry()
+def test_client_impersonate_chrome124():
+    client = Client(impersonate="chrome_124", verify=False)
     response = client.get("https://tls.peet.ws/api/all")
     assert response.status_code == 200
     json_data = response.json()
     assert json_data["http_version"] == "h2"
     assert json_data["tls"]["ja4"].startswith("t13d")
     assert (
         json_data["http2"]["akamai_fingerprint_hash"]
```

### Comparing `pyreqwest_impersonate-0.4.2/Cargo.lock` & `pyreqwest_impersonate-0.4.3/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -118,17 +118,17 @@
 name = "bitflags"
 version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "cf4b9d6a944f767f8e5e0db018570623c85f3d925ac718db4e06d0187adb21c1"
 
 [[package]]
 name = "boring-imp"
-version = "2.1.0"
+version = "2.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ee11ff36b69529f0749e81e9236f2f605402bdc506a86fa7aefed0cfcc777b68"
+checksum = "09cf17120028694687f563bdc3a2cf38ed520aefa07f1f5587efdf3235a58c4b"
 dependencies = [
  "bitflags 1.3.2",
  "boring-sys-imp",
  "brotli 3.5.0",
  "flate2",
  "foreign-types",
  "lazy_static",
@@ -197,17 +197,17 @@
 name = "bytes"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "514de17de45fdb8dc022b1a7975556c53c86f9f0aa5f534b98977b171857c2c9"
 
 [[package]]
 name = "cc"
-version = "1.0.96"
+version = "1.0.97"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "065a29261d53ba54260972629f9ca6bffa69bac13cd1fed61420f7fa68b9f8bd"
+checksum = "099a5357d84c4c61eb35fc8eafa9a79a902c2f76911e5747ced4e032edd8d9b4"
 
 [[package]]
 name = "cexpr"
 version = "0.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6fac387a98bb7c37292057cffc56d62ecb629900026402633ae9160df93a8766"
 dependencies = [
@@ -796,17 +796,17 @@
 name = "powerfmt"
 version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "439ee305def115ba05938db6eb1644ff94165c5ab5e9420d1c1bcedbba909391"
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.81"
+version = "1.0.82"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3d1597b0c024618f09a9c3b8655b7e430397a36d23fdafec26d6965e9eec3eba"
+checksum = "8ad3d49ab951a01fbaafe34f2ec74122942fe18a3f9814c3268f1bb72042131b"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "psl-types"
 version = "2.0.11"
@@ -884,17 +884,18 @@
  "pyo3-build-config",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "pyreqwest_impersonate"
-version = "0.4.2"
+version = "0.4.3"
 dependencies = [
  "encoding_rs",
+ "form_urlencoded",
  "pyo3",
  "pythonize",
  "reqwest-impersonate",
  "serde_json",
  "tokio",
 ]
 
@@ -953,17 +954,17 @@
 name = "regex-syntax"
 version = "0.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "adad44e29e4c806119491a7f06f03de4d1af22c3a680dd47f1e6e179439d1f56"
 
 [[package]]
 name = "reqwest-impersonate"
-version = "0.11.76"
+version = "0.11.77"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "72f5de030049c9f3a4a6ba4abe11c451ec3464eae3fa1e55020514891f3f5953"
+checksum = "7be6af65af12d9582d7fe87c3c0ba91e1312097d0b381223b5a1c186370dac27"
 dependencies = [
  "async-compression",
  "base64",
  "boring-imp",
  "boring-sys-imp",
  "bytes",
  "cookie",
@@ -999,29 +1000,29 @@
  "wasm-bindgen-futures",
  "web-sys",
  "winreg",
 ]
 
 [[package]]
 name = "rustc-demangle"
-version = "0.1.23"
+version = "0.1.24"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d626bb9dae77e28219937af045c257c28bfd3f69333c512553507f5f9798cb76"
+checksum = "719b953e2095829ee67db738b3bfa9fa368c94900df327b3f07fe6e794d2fe1f"
 
 [[package]]
 name = "rustc-hash"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "08d43f7aa6b08d49f382cde6a7982047c3426db949b1424bc4b7ec9ae12c6ce2"
 
 [[package]]
 name = "ryu"
-version = "1.0.17"
+version = "1.0.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e86697c916019a8588c99b5fac3cead74ec0b4b819707a682fd4d23fa0ce1ba1"
+checksum = "f3cb5ba0dc43242ce17de99c180e96db90b235b8a9fdc9543c96d2209116bd9f"
 
 [[package]]
 name = "scopeguard"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "94143f37725109f92c262ed2cf5e59bce7498c01bcc1502d7b9afe439a4e9f49"
 
@@ -1097,17 +1098,17 @@
 dependencies = [
  "libc",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.60"
+version = "2.0.61"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "909518bc7b1c9b779f1bbf07f2929d35af9f0f37e47c6e9ef7f9dddc1e1821f3"
+checksum = "c993ed8ccba56ae856363b1845da7266a7cb78e1d146c8a32d54b45a8b831fc9"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
@@ -1135,26 +1136,26 @@
 name = "target-lexicon"
 version = "0.12.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1fc403891a21bcfb7c37834ba66a547a8f402146eba7265b5a6d88059c9ff2f"
 
 [[package]]
 name = "thiserror"
-version = "1.0.59"
+version = "1.0.60"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f0126ad08bff79f29fc3ae6a55cc72352056dfff61e3ff8bb7129476d44b23aa"
+checksum = "579e9083ca58dd9dcf91a9923bb9054071b9ebbd800b342194c9feb0ee89fc18"
 dependencies = [
  "thiserror-impl",
 ]
 
 [[package]]
 name = "thiserror-impl"
-version = "1.0.59"
+version = "1.0.60"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d1cd413b5d558b4c5bf3680e324a6fa5014e7b7c067a51e69dbdf47eb7148b66"
+checksum = "e2470041c06ec3ac1ab38d0356a6119054dedaea53e12fbefc0de730a1c08524"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
```

### Comparing `pyreqwest_impersonate-0.4.2/pyproject.toml` & `pyreqwest_impersonate-0.4.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyreqwest_impersonate-0.4.2/PKG-INFO` & `pyreqwest_impersonate-0.4.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pyreqwest_impersonate
-Version: 0.4.2
+Version: 0.4.3
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -79,74 +79,93 @@
         params (dict, optional): Default query parameters to include in all requests. Default is None.
         headers (dict, optional): Default headers to send with requests. If `impersonate` is set, this will be ignored.
         timeout (float, optional): HTTP request timeout in seconds. Default is 30.
         cookie_store (bool, optional): Enable a persistent cookie store. Received cookies will be preserved and included 
             in additional requests. Default is True.
         referer (bool, optional): Enable or disable automatic setting of the `Referer` header. Default is True.
         proxy (str, optional): Proxy URL for HTTP requests. Example: "socks5://127.0.0.1:9150". Default is None.
-        impersonate (str, optional): Entity to impersonate. Example: "chrome_123". Default is None.
+        impersonate (str, optional): Entity to impersonate. Example: "chrome_124". Default is None.
             Chrome: "chrome_99","chrome_100","chrome_101","chrome_104","chrome_105","chrome_106","chrome_108", 
                 "chrome_107","chrome_109","chrome_114","chrome_116","chrome_117","chrome_118","chrome_119", 
-                "chrome_120","chrome_123"
-            Safari: "safari_ios_17_2","safari_12","safari_15_3","safari_15_5","safari_15_6_1","safari_16","safari_16_5",
-                "safari_17_2_1","safari17_4_1"
+                "chrome_120","chrome_123","chrome_124"
+            Safari: "safari_12","safari_15_3","safari_15_5","safari_15_6_1","safari_16","safari_16_5",
+                "safari_17_2_1"
             OkHttp: "okhttp_3_9","okhttp_3_11","okhttp_3_13","okhttp_3_14","okhttp_4_9","okhttp_4_10","okhttp_5"
-            Edge: "edge_99","edge_101","edge_122"
+            Edge: "edge_99","edge_101","edge_120"
         follow_redirects (bool, optional): Whether to follow redirects. Default is True.
         max_redirects (int, optional): Maximum redirects to follow. Default 20. Applies if `follow_redirects` is True.
-        verify (bool, optional): Verify SSL certificates. Default is False.
+        verify (bool, optional): Verify SSL certificates. Default is True.
         http1 (bool, optional): Use only HTTP/1.1. Default is None.
         http2 (bool, optional): Use only HTTP/2. Default is None.
          
     """
 ```
 
 #### Client Methods
 
 The `Client` class provides a set of methods for making HTTP requests: `get`, `head`, `options`, `delete`, `post`, `put`, `patch`, each of which internally utilizes the `request()` method for execution. The parameters for these methods closely resemble those in `httpx`.
 ```python
-def get(url, params=None, headers=None, auth=None, auth_bearer=None, timeout=None):
+def get(
+    url: str, 
+    params: Optional[Dict[str, str]] = None, 
+    headers: Optional[Dict[str, str]] = None, 
+    auth: Optional[Tuple[str, Optional[str]]] = None, 
+    auth_bearer: Optional[str] = None, 
+    timeout: Optional[float] = 30,
+):
     """Performs a GET request to the specified URL.
 
     Args:
         url (str): The URL to which the request will be made.
         params (Optional[Dict[str, str]]): A map of query parameters to append to the URL. Default is None.
         headers (Optional[Dict[str, str]]): A map of HTTP headers to send with the request. Default is None.
         auth (Optional[Tuple[str, Optional[str]]]): A tuple containing the username and an optional password 
             for basic authentication. Default is None.
         auth_bearer (Optional[str]): A string representing the bearer token for bearer token authentication. Default is None.
         timeout (Optional[float]): The timeout for the request in seconds. Default is 30.
 
     """
 ```
 ```python
-def post(url, params=None, headers=None, content=None, data=None, files=None, auth=None, auth_bearer=None, timeout=None):
+def post(
+    url: str, 
+    params: Optional[Dict[str, str]] = None, 
+    headers: Optional[Dict[str, str]] = None, 
+    content: Optional[bytes] = None, 
+    data: Optional[Dict[str, str]] = None, 
+    json: Any = None, 
+    files: Optional[Dict[str, str]] = None, 
+    auth: Optional[Tuple[str, Optional[str]]] = None, 
+    auth_bearer: Optional[str] = None, 
+    timeout: Optional[float] = 30,
+):
     """Performs a POST request to the specified URL.
 
     Args:
         url (str): The URL to which the request will be made.
         params (Optional[Dict[str, str]]): A map of query parameters to append to the URL. Default is None.
         headers (Optional[Dict[str, str]]): A map of HTTP headers to send with the request. Default is None.
         content (Optional[bytes]): The content to send in the request body as bytes. Default is None.
         data (Optional[Dict[str, str]]): The form data to send in the request body. Default is None.
+        json (Any): A JSON serializable object to send in the request body. Default is None.
         files (Optional[Dict[str, str]]): A map of file fields to file paths to be sent as multipart/form-data. Default is None.
         auth (Optional[Tuple[str, Optional[str]]]): A tuple containing the username and an optional password 
             for basic authentication. Default is None.
         auth_bearer (Optional[str]): A string representing the bearer token for bearer token authentication. Default is None.
         timeout (Optional[float]): The timeout for the request in seconds. Default is 30.
 
     """
 ```
 
 #### Example
 
 ```python
 import pyreqwest_impersonate as pri
 
-client = pri.Client(impersonate="chrome_123")
+client = pri.Client(impersonate="chrome_124")
 
 # get request
 resp = client.get("https://tls.peet.ws/api/all")
 print(resp.json())
 
 # post request
 data = {"key1": "value1", "key2": "value2"}
@@ -159,14 +178,14 @@
 print(resp.status_code)
 print(resp.text)
 print(resp.url)
 
 # You can also use convenience functions that use a default Client instance under the hood:
 # pri.get() | pri.head() | pri.options() | pri.delete() | pri.post | pri.patch | pri.put
 # These functions can accept the `impersonate` parameter:
-resp = pri.get("https://httpbin.org/anything", impersonate="chrome_123")  
+resp = pri.get("https://httpbin.org/anything", impersonate="chrome_124")  
 ```
 ### II. AsyncClient
 
 TODO
```

