# Comparing `tmp/llm_optimized_inference-0.1.5-py3-none-any.whl.zip` & `tmp/llm_optimized_inference-0.1.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,38 +1,38 @@
-Zip file size: 66390 bytes, number of entries: 36
--rw-rw-r--  2.0 unx      249 b- defN 24-Apr-24 00:40 llm/__init__.py
--rw-rw-r--  2.0 unx      249 b- defN 24-Apr-24 00:40 llm/optimized/__init__.py
--rw-rw-r--  2.0 unx      703 b- defN 24-Apr-24 00:40 llm/optimized/inference/__init__.py
--rw-rw-r--  2.0 unx      204 b- defN 24-Apr-24 00:40 llm/optimized/inference/_version.py
--rw-rw-r--  2.0 unx    28243 b- defN 24-Apr-24 00:40 llm/optimized/inference/api_server.py
--rw-rw-r--  2.0 unx     3203 b- defN 24-Apr-24 00:40 llm/optimized/inference/configs.py
--rw-rw-r--  2.0 unx     5548 b- defN 24-Apr-24 00:40 llm/optimized/inference/constants.py
--rw-rw-r--  2.0 unx     3255 b- defN 24-Apr-24 00:40 llm/optimized/inference/conversation.py
--rw-rw-r--  2.0 unx     5802 b- defN 24-Apr-24 00:40 llm/optimized/inference/fm_score.py
--rw-rw-r--  2.0 unx      664 b- defN 24-Apr-24 00:40 llm/optimized/inference/logging_config.py
--rw-rw-r--  2.0 unx     9028 b- defN 24-Apr-24 00:40 llm/optimized/inference/managed_inference.py
--rw-rw-r--  2.0 unx     1369 b- defN 24-Apr-24 00:40 llm/optimized/inference/model_config_factory.py
--rw-rw-r--  2.0 unx     6638 b- defN 24-Apr-24 00:40 llm/optimized/inference/model_utils.py
--rw-rw-r--  2.0 unx     1575 b- defN 24-Apr-24 00:40 llm/optimized/inference/prompt_formatter.py
--rw-rw-r--  2.0 unx    12420 b- defN 24-Apr-24 00:40 llm/optimized/inference/replica_manager.py
--rw-rw-r--  2.0 unx    18786 b- defN 24-Apr-24 00:40 llm/optimized/inference/score.py
--rw-rw-r--  2.0 unx     4731 b- defN 24-Apr-24 00:40 llm/optimized/inference/utils.py
--rw-rw-r--  2.0 unx        0 b- defN 24-Apr-24 00:40 llm/optimized/inference/api_server_setup/__init__.py
--rw-rw-r--  2.0 unx     9502 b- defN 24-Apr-24 00:40 llm/optimized/inference/api_server_setup/openapi.json
--rw-rw-r--  2.0 unx     1878 b- defN 24-Apr-24 00:40 llm/optimized/inference/api_server_setup/protocol.py
--rw-rw-r--  2.0 unx      131 b- defN 24-Apr-24 00:40 llm/optimized/inference/custom_model_configurations/__init__.py
--rw-rw-r--  2.0 unx     2725 b- defN 24-Apr-24 00:40 llm/optimized/inference/custom_model_configurations/base_configuration_builder.py
--rw-rw-r--  2.0 unx     8806 b- defN 24-Apr-24 00:40 llm/optimized/inference/custom_model_configurations/diffusion_configuration_builder.py
--rw-rw-r--  2.0 unx     1047 b- defN 24-Apr-24 00:40 llm/optimized/inference/custom_model_configurations/schema_output.py
--rw-rw-r--  2.0 unx      259 b- defN 24-Apr-24 00:40 llm/optimized/inference/engine/__init__.py
--rw-rw-r--  2.0 unx    38577 b- defN 24-Apr-24 00:40 llm/optimized/inference/engine/_hf_predictors.py
--rw-rw-r--  2.0 unx     4583 b- defN 24-Apr-24 00:40 llm/optimized/inference/engine/engine.py
--rw-rw-r--  2.0 unx     8617 b- defN 24-Apr-24 00:40 llm/optimized/inference/engine/hf_engine.py
--rw-rw-r--  2.0 unx    10797 b- defN 24-Apr-24 00:40 llm/optimized/inference/engine/mii_engine.py
--rw-rw-r--  2.0 unx     7971 b- defN 24-Apr-24 00:40 llm/optimized/inference/engine/mii_engine_v2.py
--rw-rw-r--  2.0 unx    14278 b- defN 24-Apr-24 00:40 llm/optimized/inference/engine/vllm_engine.py
--rw-rw-r--  2.0 unx        0 b- defN 24-Apr-24 00:42 llm_optimized_inference-0.1.5.dist-info/LICENSE
--rw-rw-r--  2.0 unx     3113 b- defN 24-Apr-24 00:42 llm_optimized_inference-0.1.5.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-Apr-24 00:42 llm_optimized_inference-0.1.5.dist-info/WHEEL
--rw-rw-r--  2.0 unx        4 b- defN 24-Apr-24 00:42 llm_optimized_inference-0.1.5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     3599 b- defN 24-Apr-24 00:42 llm_optimized_inference-0.1.5.dist-info/RECORD
-36 files, 218646 bytes uncompressed, 60406 bytes compressed:  72.4%
+Zip file size: 66548 bytes, number of entries: 36
+-rw-rw-r--  2.0 unx      249 b- defN 24-May-07 17:22 llm/__init__.py
+-rw-rw-r--  2.0 unx      249 b- defN 24-May-07 17:22 llm/optimized/__init__.py
+-rw-rw-r--  2.0 unx      703 b- defN 24-May-07 17:22 llm/optimized/inference/__init__.py
+-rw-rw-r--  2.0 unx      204 b- defN 24-May-07 17:22 llm/optimized/inference/_version.py
+-rw-rw-r--  2.0 unx    28243 b- defN 24-May-07 17:22 llm/optimized/inference/api_server.py
+-rw-rw-r--  2.0 unx     3203 b- defN 24-May-07 17:22 llm/optimized/inference/configs.py
+-rw-rw-r--  2.0 unx     5617 b- defN 24-May-07 17:22 llm/optimized/inference/constants.py
+-rw-rw-r--  2.0 unx     3255 b- defN 24-May-07 17:22 llm/optimized/inference/conversation.py
+-rw-rw-r--  2.0 unx     5802 b- defN 24-May-07 17:22 llm/optimized/inference/fm_score.py
+-rw-rw-r--  2.0 unx      664 b- defN 24-May-07 17:22 llm/optimized/inference/logging_config.py
+-rw-rw-r--  2.0 unx     9028 b- defN 24-May-07 17:22 llm/optimized/inference/managed_inference.py
+-rw-rw-r--  2.0 unx     1369 b- defN 24-May-07 17:22 llm/optimized/inference/model_config_factory.py
+-rw-rw-r--  2.0 unx     6638 b- defN 24-May-07 17:22 llm/optimized/inference/model_utils.py
+-rw-rw-r--  2.0 unx     1575 b- defN 24-May-07 17:22 llm/optimized/inference/prompt_formatter.py
+-rw-rw-r--  2.0 unx    12420 b- defN 24-May-07 17:22 llm/optimized/inference/replica_manager.py
+-rw-rw-r--  2.0 unx    18786 b- defN 24-May-07 17:22 llm/optimized/inference/score.py
+-rw-rw-r--  2.0 unx     4731 b- defN 24-May-07 17:22 llm/optimized/inference/utils.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-May-07 17:22 llm/optimized/inference/api_server_setup/__init__.py
+-rw-rw-r--  2.0 unx     9502 b- defN 24-May-07 17:22 llm/optimized/inference/api_server_setup/openapi.json
+-rw-rw-r--  2.0 unx     1878 b- defN 24-May-07 17:22 llm/optimized/inference/api_server_setup/protocol.py
+-rw-rw-r--  2.0 unx      131 b- defN 24-May-07 17:22 llm/optimized/inference/custom_model_configurations/__init__.py
+-rw-rw-r--  2.0 unx     2725 b- defN 24-May-07 17:22 llm/optimized/inference/custom_model_configurations/base_configuration_builder.py
+-rw-rw-r--  2.0 unx     8806 b- defN 24-May-07 17:22 llm/optimized/inference/custom_model_configurations/diffusion_configuration_builder.py
+-rw-rw-r--  2.0 unx     1047 b- defN 24-May-07 17:22 llm/optimized/inference/custom_model_configurations/schema_output.py
+-rw-rw-r--  2.0 unx      259 b- defN 24-May-07 17:22 llm/optimized/inference/engine/__init__.py
+-rw-rw-r--  2.0 unx    38577 b- defN 24-May-07 17:22 llm/optimized/inference/engine/_hf_predictors.py
+-rw-rw-r--  2.0 unx     4583 b- defN 24-May-07 17:22 llm/optimized/inference/engine/engine.py
+-rw-rw-r--  2.0 unx     8617 b- defN 24-May-07 17:22 llm/optimized/inference/engine/hf_engine.py
+-rw-rw-r--  2.0 unx    10797 b- defN 24-May-07 17:22 llm/optimized/inference/engine/mii_engine.py
+-rw-rw-r--  2.0 unx     7971 b- defN 24-May-07 17:22 llm/optimized/inference/engine/mii_engine_v2.py
+-rw-rw-r--  2.0 unx    14762 b- defN 24-May-07 17:22 llm/optimized/inference/engine/vllm_engine.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-May-07 17:25 llm_optimized_inference-0.1.6.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     3107 b- defN 24-May-07 17:25 llm_optimized_inference-0.1.6.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-May-07 17:25 llm_optimized_inference-0.1.6.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        4 b- defN 24-May-07 17:25 llm_optimized_inference-0.1.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     3599 b- defN 24-May-07 17:25 llm_optimized_inference-0.1.6.dist-info/RECORD
+36 files, 219193 bytes uncompressed, 60564 bytes compressed:  72.4%
```

## zipnote {}

```diff
@@ -87,23 +87,23 @@
 
 Filename: llm/optimized/inference/engine/mii_engine_v2.py
 Comment: 
 
 Filename: llm/optimized/inference/engine/vllm_engine.py
 Comment: 
 
-Filename: llm_optimized_inference-0.1.5.dist-info/LICENSE
+Filename: llm_optimized_inference-0.1.6.dist-info/LICENSE
 Comment: 
 
-Filename: llm_optimized_inference-0.1.5.dist-info/METADATA
+Filename: llm_optimized_inference-0.1.6.dist-info/METADATA
 Comment: 
 
-Filename: llm_optimized_inference-0.1.5.dist-info/WHEEL
+Filename: llm_optimized_inference-0.1.6.dist-info/WHEEL
 Comment: 
 
-Filename: llm_optimized_inference-0.1.5.dist-info/top_level.txt
+Filename: llm_optimized_inference-0.1.6.dist-info/top_level.txt
 Comment: 
 
-Filename: llm_optimized_inference-0.1.5.dist-info/RECORD
+Filename: llm_optimized_inference-0.1.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## llm/optimized/inference/_version.py

```diff
@@ -1,5 +1,5 @@
 # ---------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # ---------------------------------------------------------
 
-VERSION = "0.1.5"
+VERSION = "0.1.6"
```

## llm/optimized/inference/constants.py

```diff
@@ -1,11 +1,12 @@
 # Copyright (c) Microsoft Corporation.
 # Licensed under the MIT License.
 """This module defines the EngineName and TaskType enums."""
 from enum import Enum
+from typing import Dict, List
 
 
 class EngineName(str, Enum):
     """Enum representing the names of the engines."""
 
     HF = "hf"
     VLLM = "vllm"
@@ -88,16 +89,17 @@
         "OPTForCausalLM",
         "OrionForCausalLM",
         "QWenLMHeadModel",
         "Qwen2ForCausalLM",
         "RWForCausalLM",
         "StableLmForCausalLM",
         "DbrxForCausalLM",
-        "Phi3MiniForCausalLM",
-        "PhiLongRoPEForCausalLM",
+        "PhiForCausalLM",
+        "Phi3ForCausalLM",
+        "Phi3SmallForCausalLM",
         "YakForCausalLM"
     }
 
 
 class MIISupportedModels:
     """MII Supported Models."""
 
@@ -126,28 +128,28 @@
 
     Models = {
         "falcon": {"kwargs": {"gpu-memory-utilization": .95}, "args": ["trust-remote-code"]},
         "RefinedWebModel": {"kwargs": {"gpu-memory-utilization": .95}, "args": ["trust-remote-code"]},
         "RefinedWeb": {"kwargs": {"gpu-memory-utilization": .95}, "args": ["trust-remote-code"]},
         "dbrx": {"args": ["trust-remote-code"]},
         "deci_lm": {"args": ["trust-remote-code"]},
-        "phi3mini": {"kwargs": {"tensor-parallel-size": 1}, "args": ["trust-remote-code"]},
-        "phi_longrope": {"kwargs": {"tensor-parallel-size": 1}, "args": ["trust-remote-code"]},
+        "phi": {"args": ["trust-remote-code"]},
+        "phi3": {"kwargs": {"tensor-parallel-size": 1}, "args": ["trust-remote-code"]},
+        "phi3small": {"args": ["trust-remote-code"]},
         "yak": {"kwargs": {"quantization": "yq"}}
-
     }
 
     @classmethod
-    def get_kwargs(cls, model_type: str):
+    def get_kwargs(cls, model_type: str) -> Dict:
         """Get the kwargs the vllm server needs for the model type."""
         params = cls.Models.get(model_type, {})
         return params.get("kwargs", {})
 
     @classmethod
-    def get_args(cls, model_type: str):
+    def get_args(cls, model_type: str) -> List:
         """Get the args the vllm server needs for the model type."""
         params = cls.Models.get(model_type, {})
         return params.get("args", [])
 
 
 ALL_TASKS = [
     SupportedTask.TEXT_TO_IMAGE,
```

## llm/optimized/inference/engine/vllm_engine.py

```diff
@@ -103,16 +103,27 @@
             )
         if "model" not in self._vllm_args:
             self._vllm_args["model"] = self.engine_config.model_id
 
         if "tokenizer" not in self._vllm_args:
             self._vllm_args["tokenizer"] = self.engine_config.tokenizer
 
-        self._vllm_args.update(VLLMSpecialModels.get_kwargs(self._model_type))
-        self._vllm_additional_args.extend(VLLMSpecialModels.get_args(self._model_type))
+
+        kwargs = VLLMSpecialModels.get_kwargs(self._model_type)
+        args = VLLMSpecialModels.get_args(self._model_type)
+        if self._model_type == "phi3":
+            full_model_name = self.engine_config.ml_model_info.get("model_id", None)
+
+            # Phi-3 models share the same model type names but phi-3-medium-128k requires a different
+            # tensor parallel size than the other Phi-3 models
+            if full_model_name == "microsoft/phi-3-medium-128k-instruct":
+                kwargs.update({"tensor-parallel-size": 2})
+    
+        self._vllm_args.update(kwargs)
+        self._vllm_additional_args.extend(args)
         self._vllm_additional_args.append("disable-log-requests")
 
     def _verify_and_convert_float_type(self):
         """Check to see whether the model's float type is compatible with the compute type selected.
 
         Bfloat16 is only supported on GPUs such as A100s. V100s do not support bfloat16, only float16.
         Converting from bfloat16 to float16 is ok in this case.
```

## Comparing `llm_optimized_inference-0.1.5.dist-info/METADATA` & `llm_optimized_inference-0.1.6.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 Metadata-Version: 2.1
 Name: llm-optimized-inference
-Version: 0.1.5
+Version: 0.1.6
 Home-page: 
 Author: Microsoft
 Author-email: 
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: deepspeed ==0.13.2
 Requires-Dist: deepspeed-mii ==0.2.2
-Requires-Dist: vllm ==0.4.0.post1
+Requires-Dist: vllm ==0.4.2
 Requires-Dist: deepspeed-kernels ==0.0.1.dev1698255861
 Requires-Dist: diffusers ==0.26.2
 Requires-Dist: pandas ~=2.1.4
 Requires-Dist: transformers ~=4.40.0
 Requires-Dist: aiolimiter ~=1.1.0
 Requires-Dist: azure-ai-contentsafety ==1.0.0b1
 Requires-Dist: azure-ai-ml ==1.12.1
 Requires-Dist: azure-identity ==1.15.0
 Requires-Dist: azureml-ai-monitoring ==0.1.0b4
 Requires-Dist: azureml-inference-server-http
 Requires-Dist: azureml-mlflow
 Requires-Dist: requests ~=2.31.0
 Requires-Dist: aiohttp ~=3.9.1
-Requires-Dist: torch ~=2.1.2
+Requires-Dist: torch ~=2.3.0
 Requires-Dist: scipy
 Requires-Dist: accelerate >=0.20.3
 Provides-Extra: dev
 Requires-Dist: pytest ; extra == 'dev'
 
 # Foundation Model Inferencing
```

## Comparing `llm_optimized_inference-0.1.5.dist-info/RECORD` & `llm_optimized_inference-0.1.6.dist-info/RECORD`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 llm/__init__.py,sha256=ybCtCrXNS3six25SvldGKjcl-9eR9CzOMgoUjbRBdBQ,249
 llm/optimized/__init__.py,sha256=ybCtCrXNS3six25SvldGKjcl-9eR9CzOMgoUjbRBdBQ,249
 llm/optimized/inference/__init__.py,sha256=rGZODP-qE2NOlUgdbmxhfuS3svmx9gM-kU97d9-jb50,703
-llm/optimized/inference/_version.py,sha256=aMIajadgoqRXx51Q5q1FRPYUqvpLEK0ugL8CtTU-DrA,204
+llm/optimized/inference/_version.py,sha256=E33LCXtRMMIS-GExLNxF_yCpQ1D-zJrxuCDiZv6aGI4,204
 llm/optimized/inference/api_server.py,sha256=kyUIykJuk9jPajQyUqqMl4FEQKLZV57LykfGY0Z99Ak,28243
 llm/optimized/inference/configs.py,sha256=d5NKbQlfYVkUQ4SL03KVBQekdOG4VrcD0xGxVeHESeQ,3203
-llm/optimized/inference/constants.py,sha256=FqDNm7XiTHbFbdUKxgFwYEeH7pOomJngU4PB3mOwgoI,5548
+llm/optimized/inference/constants.py,sha256=8hpMpT0RwWeqqKoAa4TTD0MXQNdq5bpcwBXF0JdaCcc,5617
 llm/optimized/inference/conversation.py,sha256=cBrHv1sI1hrOQB57sSZKAarplKRgqQWqmYxT-wkZHLM,3255
 llm/optimized/inference/fm_score.py,sha256=7z7ZbLMXUXH6gp1-G_l3rOus9r9vSpIm5-wOj5X17aQ,5802
 llm/optimized/inference/logging_config.py,sha256=egtAiGCNVNoU8E_JPhp2aGJVIJ_QkTwLhkNjpVKjICI,664
 llm/optimized/inference/managed_inference.py,sha256=O_HlOPNl24Uoy68gFKrSM_gOG-rg4P_lishBQFAXyC8,9028
 llm/optimized/inference/model_config_factory.py,sha256=EpHH8QyUaE5DC6A5O5nKbie_kMEpfeqmufbOn0U6jFI,1369
 llm/optimized/inference/model_utils.py,sha256=W9nLxInrhuPnmhvZldBpS2POB7-u_SST7ostxatAYrA,6638
 llm/optimized/inference/prompt_formatter.py,sha256=xxM4MbvvPL6jQcLB37uKA9-wCHXTZUL9l5GiUu3r964,1575
@@ -24,13 +24,13 @@
 llm/optimized/inference/custom_model_configurations/schema_output.py,sha256=JIpThLkAPoO7MlhaJVSxP2RYVwYzIpw3R3k-nraLq9k,1047
 llm/optimized/inference/engine/__init__.py,sha256=8GqGW53dbRlGShwO11h5HQH4KjnUzoW0t0cChUUFDPY,259
 llm/optimized/inference/engine/_hf_predictors.py,sha256=AwQTIpmOHb7h31H2DF2Jx-9b03lcB5DOrgSbXGpamIk,38577
 llm/optimized/inference/engine/engine.py,sha256=xbpEVJBjovFyACw6WF8uqnmyodRWqb52oaR3s3pr8Sc,4583
 llm/optimized/inference/engine/hf_engine.py,sha256=4rRldNod-pMDJ_-3q0RDWEkigCTr6I62HyJspb01lAs,8617
 llm/optimized/inference/engine/mii_engine.py,sha256=TBfc_wt4-NKTzkjHCie5YpqRGS6pvBNigyYpTHt_jII,10797
 llm/optimized/inference/engine/mii_engine_v2.py,sha256=rI4tjRyj-dCZBDAiN0YNPKMBtkD3MXxcbucuSlHg6lI,7971
-llm/optimized/inference/engine/vllm_engine.py,sha256=IZDkMxOTMhsn7qCmsSAfIE8DFll4dfDRIWd5FU6_a3c,14278
-llm_optimized_inference-0.1.5.dist-info/LICENSE,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-llm_optimized_inference-0.1.5.dist-info/METADATA,sha256=rry2yZ8rLf2ozc1k-3qP6kJ9fD6UkTYXpqsslblJgN0,3113
-llm_optimized_inference-0.1.5.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
-llm_optimized_inference-0.1.5.dist-info/top_level.txt,sha256=TwpEQXP3b1MS9Y2XuGgRuo9-Kny507xt2HFZgJ5TSIY,4
-llm_optimized_inference-0.1.5.dist-info/RECORD,,
+llm/optimized/inference/engine/vllm_engine.py,sha256=_-q0S8ewaLJR7dN0I2nTY19hbuqwD4SOxVGibJc4Y4k,14762
+llm_optimized_inference-0.1.6.dist-info/LICENSE,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+llm_optimized_inference-0.1.6.dist-info/METADATA,sha256=H9_Ix9Km_7FfmJFeTbnQO40MYTtDj_a64zb-F-0Yg8I,3107
+llm_optimized_inference-0.1.6.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+llm_optimized_inference-0.1.6.dist-info/top_level.txt,sha256=TwpEQXP3b1MS9Y2XuGgRuo9-Kny507xt2HFZgJ5TSIY,4
+llm_optimized_inference-0.1.6.dist-info/RECORD,,
```

