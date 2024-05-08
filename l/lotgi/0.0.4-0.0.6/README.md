# Comparing `tmp/lotgi-0.0.4.tar.gz` & `tmp/lotgi-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lotgi-0.0.4.tar", last modified: Sun Apr 28 00:37:45 2024, max compression
+gzip compressed data, was "lotgi-0.0.6.tar", last modified: Tue May  7 04:34:17 2024, max compression
```

## Comparing `lotgi-0.0.4.tar` & `lotgi-0.0.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-28 00:37:45.233856 lotgi-0.0.4/
--rw-r--r--   0 alex       (501) staff       (20)      452 2024-04-28 00:37:45.233719 lotgi-0.0.4/PKG-INFO
--rw-r--r--   0 alex       (501) staff       (20)      660 2024-04-28 00:08:24.000000 lotgi-0.0.4/pyproject.toml
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-28 00:37:45.231787 lotgi-0.0.4/python/
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-28 00:37:45.232462 lotgi-0.0.4/python/lotgi/
--rw-r--r--   0 alex       (501) staff       (20)     4183 2024-04-28 00:11:31.000000 lotgi-0.0.4/python/lotgi/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)       61 2024-04-27 22:29:31.000000 lotgi-0.0.4/python/lotgi/__main__.py
--rw-r--r--   0 alex       (501) staff       (20)      706 2024-04-11 20:15:07.000000 lotgi-0.0.4/python/lotgi/_openai.py
--rw-r--r--   0 alex       (501) staff       (20)      383 2024-04-11 18:54:15.000000 lotgi-0.0.4/python/lotgi/logging.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-28 00:37:45.233188 lotgi-0.0.4/python/lotgi/models/
--rw-r--r--   0 alex       (501) staff       (20)     1780 2024-04-28 00:06:18.000000 lotgi-0.0.4/python/lotgi/models/rest.py
--rw-r--r--   0 alex       (501) staff       (20)     5059 2024-04-28 00:12:17.000000 lotgi-0.0.4/python/lotgi/rest_client.py
--rw-r--r--   0 alex       (501) staff       (20)     1016 2024-04-27 22:30:18.000000 lotgi-0.0.4/python/lotgi/tokens.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-28 00:37:45.233575 lotgi-0.0.4/python/lotgi.egg-info/
--rw-r--r--   0 alex       (501) staff       (20)      452 2024-04-28 00:37:45.000000 lotgi-0.0.4/python/lotgi.egg-info/PKG-INFO
--rw-r--r--   0 alex       (501) staff       (20)      436 2024-04-28 00:37:45.000000 lotgi-0.0.4/python/lotgi.egg-info/SOURCES.txt
--rw-r--r--   0 alex       (501) staff       (20)        1 2024-04-28 00:37:45.000000 lotgi-0.0.4/python/lotgi.egg-info/dependency_links.txt
--rw-r--r--   0 alex       (501) staff       (20)       36 2024-04-28 00:37:45.000000 lotgi-0.0.4/python/lotgi.egg-info/entry_points.txt
--rw-r--r--   0 alex       (501) staff       (20)       66 2024-04-28 00:37:45.000000 lotgi-0.0.4/python/lotgi.egg-info/requires.txt
--rw-r--r--   0 alex       (501) staff       (20)       12 2024-04-28 00:37:45.000000 lotgi-0.0.4/python/lotgi.egg-info/top_level.txt
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-28 00:37:45.233282 lotgi-0.0.4/python/tests/
--rw-r--r--   0 alex       (501) staff       (20)       49 2024-04-08 18:16:29.000000 lotgi-0.0.4/python/tests/test_basic.py
--rw-r--r--   0 alex       (501) staff       (20)       38 2024-04-28 00:37:45.233883 lotgi-0.0.4/setup.cfg
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-05-07 04:34:17.182882 lotgi-0.0.6/
+-rw-r--r--   0 alex       (501) staff       (20)      525 2024-05-07 04:34:17.182731 lotgi-0.0.6/PKG-INFO
+-rw-r--r--   0 alex       (501) staff       (20)      705 2024-05-07 04:30:59.000000 lotgi-0.0.6/pyproject.toml
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-05-07 04:34:17.180247 lotgi-0.0.6/python/
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-05-07 04:34:17.181399 lotgi-0.0.6/python/lotgi/
+-rw-r--r--   0 alex       (501) staff       (20)     7831 2024-05-07 04:30:28.000000 lotgi-0.0.6/python/lotgi/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)       61 2024-04-27 22:29:31.000000 lotgi-0.0.6/python/lotgi/__main__.py
+-rw-r--r--   0 alex       (501) staff       (20)      706 2024-04-11 20:15:07.000000 lotgi-0.0.6/python/lotgi/_openai.py
+-rw-r--r--   0 alex       (501) staff       (20)      383 2024-04-11 18:54:15.000000 lotgi-0.0.6/python/lotgi/logging.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-05-07 04:34:17.182145 lotgi-0.0.6/python/lotgi/models/
+-rw-r--r--   0 alex       (501) staff       (20)     2203 2024-05-07 04:23:13.000000 lotgi-0.0.6/python/lotgi/models/rest.py
+-rw-r--r--   0 alex       (501) staff       (20)     6014 2024-05-07 04:24:19.000000 lotgi-0.0.6/python/lotgi/rest_client.py
+-rw-r--r--   0 alex       (501) staff       (20)     1316 2024-05-01 23:14:33.000000 lotgi-0.0.6/python/lotgi/tokens.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-05-07 04:34:17.182558 lotgi-0.0.6/python/lotgi.egg-info/
+-rw-r--r--   0 alex       (501) staff       (20)      525 2024-05-07 04:34:17.000000 lotgi-0.0.6/python/lotgi.egg-info/PKG-INFO
+-rw-r--r--   0 alex       (501) staff       (20)      436 2024-05-07 04:34:17.000000 lotgi-0.0.6/python/lotgi.egg-info/SOURCES.txt
+-rw-r--r--   0 alex       (501) staff       (20)        1 2024-05-07 04:34:17.000000 lotgi-0.0.6/python/lotgi.egg-info/dependency_links.txt
+-rw-r--r--   0 alex       (501) staff       (20)       36 2024-05-07 04:34:17.000000 lotgi-0.0.6/python/lotgi.egg-info/entry_points.txt
+-rw-r--r--   0 alex       (501) staff       (20)       95 2024-05-07 04:34:17.000000 lotgi-0.0.6/python/lotgi.egg-info/requires.txt
+-rw-r--r--   0 alex       (501) staff       (20)       12 2024-05-07 04:34:17.000000 lotgi-0.0.6/python/lotgi.egg-info/top_level.txt
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-05-07 04:34:17.182283 lotgi-0.0.6/python/tests/
+-rw-r--r--   0 alex       (501) staff       (20)       49 2024-04-08 18:16:29.000000 lotgi-0.0.6/python/tests/test_basic.py
+-rw-r--r--   0 alex       (501) staff       (20)       38 2024-05-07 04:34:17.182910 lotgi-0.0.6/setup.cfg
```

### Comparing `lotgi-0.0.4/pyproject.toml` & `lotgi-0.0.6/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -8,31 +8,34 @@
 [project]
 name = "lotgi"
 authors = [
     {name = "Alex Wu", email = "alexanderwu@berkeley.edu"},
 ]
 description = "For the love of the game"
 readme = "README.md"
-requires-python = ">=3.10"
+requires-python = ">=3.8"
 keywords = []
 license = {text = "BSD-3-Clause"}
 classifiers = [
     "Programming Language :: Python :: 3",
 ]
 dependencies = [
-  "click",
+  "click >= 7.0",
+  "openai",
+  "pandas",
   "pydantic",
   "requests",
   "tabulate",
   "transformers",
   "openai",
   "tomli",
   "pandas",
+  "shortuuid",
 ]
-version="0.0.4"
+version="0.0.6"
 
 
 [tool.setuptools.packages.find]
 where = ["python/"]
 
 [project.scripts]
 lotgi = "lotgi:cli"
```

### Comparing `lotgi-0.0.4/python/lotgi/_openai.py` & `lotgi-0.0.6/python/lotgi/_openai.py`

 * *Files identical despite different names*

### Comparing `lotgi-0.0.4/python/lotgi/models/rest.py` & `lotgi-0.0.6/python/lotgi/models/rest.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,12 @@
-from pydantic import BaseModel, Field, model_validator
+from pydantic import BaseModel, Field, model_validator, Extra
 from typing import Optional
-import uuid
+import shortuuid
+
+uuid_generator = shortuuid.ShortUUID(alphabet="abcdefghijklmnopqrstuvwxyz1234567890")
 
 class ModalCredentials(BaseModel):
     token_id : str
     token_secret : str
 
 class RunpodCredentials(BaseModel):
     api_key : str
@@ -19,40 +21,57 @@
             raise ValueError("At least one set of credentials should be specified.")
         return self
 
 EXECUTION_TRADEOFFS = {
     "Cheapest",
     "Hour",
 }
+
+DEFAULT_MAX_OUTPUT_TOKENS = 32
+DEFAULT_REGEX = r".*"
+
 class JobSpec(BaseModel):
-    job_id : str = Field(default_factory=lambda : f"job-{uuid.uuid4()}")
+    job_id : str = Field(default_factory=lambda : f"job-{uuid_generator.uuid()}")
     cloud_credentials : Optional[CloudCredentials] = None
-    input_url : str
+    input_file : str
     target_cost : float
     target_deadline : int # Specified as a unix timestamp
     model : str
     field : str
     execution_tradeoff : str
+    max_output_tokens : int = DEFAULT_MAX_OUTPUT_TOKENS
+    regex : str = DEFAULT_REGEX
     huggingface_token : Optional[str] = None
 
     # @model_validator(mode="after")
     # def valid_execution_tradeoff(self):
     #     if self.execution_tradeoff not in EXECUTION_TRADEOFFS:
     #         raise ValueError(f"execution_tradeoff must be one off {EXECUTION_TRADEOFFS}")
     #     return self
 
-class JobStatus(BaseModel):
-    job_id : str = Field(default_factory=lambda : f"job-{uuid.uuid4()}")
-    input_url : str
+class JobStatus(BaseModel, extra=Extra.allow):
+    job_id : str
+    state : str
+    model : str
+    submission_time : int
+    execution_tradeoff : str
+    input_file : str
     target_cost : float
     target_deadline : int # Specified as a unix timestamp
-    state : str
+    field : str
 
 class JobExecutionOptionsInput(BaseModel):
     input_token_count : int
-    output_token_count : int
+    num_requests : int
     model : str
+    max_output_tokens : int = 32
 
 class JobExecutionTradeoffOption(BaseModel):
     option_name : str
     expected_cost : float
     expected_duration : int # In seconds
+
+class MetricInput(BaseModel):
+    job_id: str
+    metric_name: str
+    metric_value: float
+
```

### Comparing `lotgi-0.0.4/python/lotgi/rest_client.py` & `lotgi-0.0.6/python/lotgi/rest_client.py`

 * *Files 12% similar despite different names*

```diff
@@ -54,54 +54,68 @@
         self._token = os.environ["LOTGI_TOKEN"]
 
         self.headers = {
             "lotgi-token": self._token,
             "Content-type": "application/json",
         }
 
-    def submit_job(self, *, model : str, input_url : str, field : str, target_cost : float, target_deadline : int, execution_tradeoff : str, _autodetect_cloud_credentials : bool = False) -> rest.JobStatus:
+    def submit_job(self, *,
+                   model : str,
+                   input_file : str,
+                   field : str,
+                   target_cost : float,
+                   target_deadline : int,
+                   execution_tradeoff : str,
+                   max_output_tokens : Optional[int],
+                   regex : Optional[str],
+                   _autodetect_cloud_credentials : bool = False
+                   ) -> rest.JobStatus:
         url = f"{self.endpoint}/create_job"
 
         if _autodetect_cloud_credentials:
             cloud_credentials = get_cloud_credentials()
         else:
             cloud_credentials = None
 
 
+        if max_output_tokens is None:
+            max_output_tokens = rest.DEFAULT_MAX_OUTPUT_TOKENS
+        if regex  is None:
+            regex = rest.DEFAULT_REGEX
+
         job_spec = rest.JobSpec(
             cloud_credentials=cloud_credentials,
-            input_url=input_url,
+            input_file=input_file,
             model=model,
             field=field,
             target_cost=target_cost,
             target_deadline=target_deadline,
             execution_tradeoff=execution_tradeoff,
-            huggingface_token=get_huggingface_credentials()
+            huggingface_token=get_huggingface_credentials(),
+            max_output_tokens=max_output_tokens,
+            regex=regex,
         )
 
+
         body = job_spec.dict()
 
         result = requests.post(url, headers=self.headers, json=body)
 
         if result.status_code == 401:
             raise PermissionError(f"Request authentication failed. Is your `LOTGI_TOKEN` environment variable set correctly? {result.status_code} : {result.json()['detail']}")
 
         if not result.ok:
             raise RuntimeError(f"Request was not successfully submitted. {result.status_code}: {result.text}")
 
         return rest.JobStatus.validate(result.json())
 
     def job_exection_options(self, *, job_execution_options_input : rest.JobExecutionOptionsInput) -> List[rest.JobExecutionTradeoffOption]:
         url = f"{self.endpoint}/job_execution_options"
-        headers = {
-            "user-id": self._user_id,
-            "Content-type": "application/json",
-        }
 
-        result = requests.get(url, headers=headers, json=job_execution_options_input.dict())
+        result = requests.get(url, headers=self.headers, json=job_execution_options_input.dict())
 
         if not result.ok:
             raise RuntimeError(f"Request was not successfully submitted. {result.status_code}: {result.text}")
 
         return [
             rest.JobExecutionTradeoffOption.parse_obj(result.json()[i])
             for i in range(len(result.json()))
@@ -133,8 +147,17 @@
         if result.status_code == 404:
             raise KeyError(f"Job doesn't exist! {result.text}")
 
         if not result.ok:
             raise RuntimeError(f"Request was not successfully submitted. {result.status_code}: {result.text}")
         return result.json()
 
+    def get_upload_url(self, filename : str) -> str:
+        url = f"{self.endpoint}/get_upload_url"
+        result = requests.get(url, headers=self.headers, params={"filename": filename})
+
+        if result.status_code == 401:
+            raise PermissionError(f"Request authentication failed. Is your `LOTGI_TOKEN` environment variable set correctly? {result.status_code} : {result.json()['detail']}")
 
+        if not result.ok:
+            raise RuntimeError(f"Request was not successfully submitted. {result.status_code}: {result.text}")
+        return result.json()
```

### Comparing `lotgi-0.0.4/python/lotgi/tokens.py` & `lotgi-0.0.6/python/lotgi/tokens.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,40 @@
 from transformers import AutoTokenizer
+from tqdm import tqdm
 import pandas as pd
 from dataclasses import dataclass
 
 from lotgi.models.rest import JobExecutionOptionsInput
 
-@dataclass
-class TokenUsageEstimate:
-    input_tokens : str # We should be pretty confident this number is correct.
-    output_tokens : str # This is an estimate
+tqdm.pandas()
 
+TEMPLATE = (
+    "We have provided context information below. \n"
+    "---------------------\n"
+    "{context_str}"
+    "\n---------------------\n"
+    "Given this information, please answer the question: {query_str}\n"
+)
 
 def estimate_token_usage(input_url : str, prompt : str, model : str, field : str) -> JobExecutionOptionsInput:
     tokenizer = AutoTokenizer.from_pretrained(model)
 
     inputs = pd.read_json(input_url, lines=True)
 
+    print("Inserting prompt into dataset...")
+    inputs[field] = inputs[field].progress_apply(lambda text: TEMPLATE.format(context_str=text, query_str=prompt))
+
     num_prompt_tokens = len(tokenizer.encode(prompt))
     num_completions = len(inputs)
 
     def token_count(row) -> int:
         return len(tokenizer.encode(row))
 
-    num_dataset_tokens = inputs[field].map(token_count).sum()
+    print("Calculating number of tokens...")
+    num_dataset_tokens = inputs[field].progress_map(token_count).sum()
 
     return JobExecutionOptionsInput(
         model=model,
         input_token_count=(num_prompt_tokens * num_completions) + num_dataset_tokens,
         # TODO: This is an incredibly not-robust estimate.
-        output_token_count=250 * num_completions,
+        num_requests=num_completions,
     )
```

