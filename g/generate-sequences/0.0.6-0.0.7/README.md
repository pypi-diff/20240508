# Comparing `tmp/generate_sequences-0.0.6.tar.gz` & `tmp/generate_sequences-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "generate_sequences-0.0.6.tar", last modified: Fri May  3 17:10:41 2024, max compression
+gzip compressed data, was "generate_sequences-0.0.7.tar", last modified: Wed May  8 16:16:28 2024, max compression
```

## Comparing `generate_sequences-0.0.6.tar` & `generate_sequences-0.0.7.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:10:41.018571 generate_sequences-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)    11359 2024-05-03 17:08:30.000000 generate_sequences-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14973 2024-05-03 17:10:41.018571 generate_sequences-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-03 17:08:30.000000 generate_sequences-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:10:41.014571 generate_sequences-0.0.6/generate_sequences/
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-03 17:08:30.000000 generate_sequences-0.0.6/generate_sequences/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9926 2024-05-03 17:08:30.000000 generate_sequences-0.0.6/generate_sequences/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 17:08:30.000000 generate_sequences-0.0.6/generate_sequences/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-03 17:08:30.000000 generate_sequences-0.0.6/generate_sequences/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:10:41.014571 generate_sequences-0.0.6/generate_sequences.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14973 2024-05-03 17:10:41.000000 generate_sequences-0.0.6/generate_sequences.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-03 17:10:41.000000 generate_sequences-0.0.6/generate_sequences.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 17:10:41.000000 generate_sequences-0.0.6/generate_sequences.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-03 17:10:41.000000 generate_sequences-0.0.6/generate_sequences.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-03 17:10:41.000000 generate_sequences-0.0.6/generate_sequences.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-05-03 17:08:30.000000 generate_sequences-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 17:10:41.018571 generate_sequences-0.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:16:28.860396 generate_sequences-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)    11359 2024-05-08 16:13:58.000000 generate_sequences-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14973 2024-05-08 16:16:28.860396 generate_sequences-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-08 16:13:58.000000 generate_sequences-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:16:28.856396 generate_sequences-0.0.7/generate_sequences/
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-08 16:13:58.000000 generate_sequences-0.0.7/generate_sequences/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10801 2024-05-08 16:13:58.000000 generate_sequences-0.0.7/generate_sequences/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 16:13:58.000000 generate_sequences-0.0.7/generate_sequences/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-08 16:13:58.000000 generate_sequences-0.0.7/generate_sequences/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-08 16:13:58.000000 generate_sequences-0.0.7/generate_sequences/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:16:28.856396 generate_sequences-0.0.7/generate_sequences.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14973 2024-05-08 16:16:28.000000 generate_sequences-0.0.7/generate_sequences.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-08 16:16:28.000000 generate_sequences-0.0.7/generate_sequences.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 16:16:28.000000 generate_sequences-0.0.7/generate_sequences.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-08 16:16:28.000000 generate_sequences-0.0.7/generate_sequences.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-08 16:16:28.000000 generate_sequences-0.0.7/generate_sequences.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-05-08 16:13:58.000000 generate_sequences-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 16:16:28.860396 generate_sequences-0.0.7/setup.cfg
```

### Comparing `generate_sequences-0.0.6/LICENSE` & `generate_sequences-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `generate_sequences-0.0.6/PKG-INFO` & `generate_sequences-0.0.7/PKG-INFO`

 * *Files identical despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: generate-sequences
-Version: 0.0.6
+Version: 0.0.7
 Author-email: "Maged S. Al-Shaibani" <mageedsaeed1@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 https://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
@@ -216,15 +216,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: tqdm==4.66.*
 Requires-Dist: numpy>=1.24.0
 Requires-Dist: torch<2.4,>=2.2
 Provides-Extra: dev
 Requires-Dist: ruff; extra == "dev"
-Requires-Dist: mypy<1.10,>=1.0; extra == "dev"
+Requires-Dist: mypy<1.11,>=1.0; extra == "dev"
 Requires-Dist: black<25.0,>=23.0; extra == "dev"
 Requires-Dist: isort<5.14,>=5.12; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-sphinx; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: twine>=1.11.0; extra == "dev"
 Requires-Dist: build; extra == "dev"
```

### Comparing `generate_sequences-0.0.6/generate_sequences/generate.py` & `generate_sequences-0.0.7/generate_sequences/generate.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,49 +3,67 @@
 from typing import Callable, Iterator, List, Union
 
 import torch
 import torch.nn.functional as F
 import torch.utils
 from tqdm.auto import tqdm
 
+from generate_sequences.utils import sort_list_with_positions
+
 
 class BaseGenerator:
     def __init__(
         self,
         decoder_start_token_id: int,
         eos_token_id: int,
         generation_forward: Callable[
             [Union[List[torch.Tensor], List[str]], torch.Tensor],
             torch.Tensor,
         ],
         max_length: int = 1_024,
         batch_size: int = 1,
-        device: str = "cuda",
+        device: str = "cuda" if torch.cuda.is_available() else "cpu",
         temperature: float = 1.0,
         use_tqdm: bool = True,
         multinomial_sampling: bool = False,
+        sort_samples: bool = False,
     ) -> None:
         self.device = device
         self.use_tqdm = use_tqdm
         self.max_length = max_length
         self.batch_size = batch_size
         self.generation_forward = generation_forward
         self.eos_token_id = eos_token_id
         self.decoder_start_token_id = decoder_start_token_id
         self.temperature = temperature
         self.multinomial_sampling = multinomial_sampling
+        self.sort_samples = sort_samples
 
     def get_batches(self, inputs: Union[List[torch.Tensor], List[str]]) -> Iterator[List[str]]:
+        batched_inputs = inputs
+        if self.sort_samples:
+            sorted_inputs, inputs_positions = sort_list_with_positions(inputs)
+            self.inputs_original_positions = inputs_positions
+            batched_inputs = sorted_inputs
+
         for i in tqdm(
-            range(0, len(inputs), self.batch_size),
+            range(0, len(batched_inputs), self.batch_size),
             disable=not self.use_tqdm,
             desc="Generating Sequences",
-            total=len(inputs) // self.batch_size,
+            total=len(batched_inputs) // self.batch_size,
         ):
-            yield inputs[i : i + self.batch_size]
+            yield batched_inputs[i : i + self.batch_size]
+
+    def restore_outputs_order(self, outputs):
+        if not self.sort_samples:
+            return outputs
+        ordered_outputs = []
+        for position in self.inputs_original_positions:
+            ordered_outputs.append(outputs[position])
+        return ordered_outputs
 
 
 class GreedyGenerator(BaseGenerator):
     @torch.no_grad()
     def generate(self, inputs: Union[List[torch.Tensor], List[str]]) -> List[torch.Tensor]:
         outputs = []
         # add user warning if temperature is not 1.0 that greedy search is not appropriate
@@ -80,15 +98,15 @@
                     ).squeeze()
                 else:
                     next_tokens = torch.argmax(next_tokens, dim=-1)
                 not_finished = ~finished_mask
                 decoder_inputs[not_finished, step] = next_tokens[not_finished]
                 finished_mask |= next_tokens == self.eos_token_id  # Update finished sequences
             outputs += decoder_inputs
-        return outputs
+        return self.restore_outputs_order(outputs)
 
 
 class BeamNode:
     """Represents a node in a beam search. Stores token sequences and their associated score."""
 
     def __init__(self, tokens: List[int], score: float) -> None:
         self.tokens = tokens
@@ -116,18 +134,19 @@
         eos_token_id: int,
         generation_forward: Callable[
             [Union[List[torch.Tensor], List[str]], torch.Tensor],
             torch.Tensor,
         ],
         max_length: int = 1_024,
         batch_size: int = 1,
-        device: str = "cuda",
+        device: str = "cuda" if torch.cuda.is_available() else "cpu",
         temperature: float = 1.0,
         use_tqdm: bool = True,
         multinomial_sampling: bool = False,
+        sort_samples: bool = False,
         beam_width: int = 4,
         length_penalty: float = 1.0,
         beam_nodes_ordering_function: Callable[
             [BeamNode, int, float], float
         ] = default_beam_nodes_ordering_fn,
     ) -> None:
         super().__init__(
@@ -136,14 +155,15 @@
             generation_forward,
             max_length,
             batch_size,
             device,
             temperature,
             use_tqdm,
             multinomial_sampling,
+            sort_samples,
         )
         self.beam_width = beam_width
         self.length_penalty = length_penalty
         self.beam_nodes_ordering_function = beam_nodes_ordering_function
 
     def get_top_nodes(self, nodes) -> List[BeamNode]:
         """Returns the top k nodes in the beam according to the ordering function."""
@@ -155,15 +175,15 @@
                 self.eos_token_id,
                 self.length_penalty,
             ),
         )
 
     @torch.no_grad
     def generate(self, inputs: Union[List[torch.Tensor], List[str]]) -> List[torch.Tensor]:
-        predictions = []
+        outputs = []
         for batch in self.get_batches(inputs):
             batch_nodes = [
                 [
                     BeamNode(
                         tokens=[self.decoder_start_token_id],
                         score=0.0,
                     )
@@ -232,9 +252,9 @@
                     key=lambda node: self.beam_nodes_ordering_function(
                         node,
                         self.eos_token_id,
                         self.length_penalty,
                     ),
                 )
                 batch_predictions.append(best_node.tokens)
-            predictions += batch_predictions
-        return predictions
+            outputs += batch_predictions
+        return self.restore_outputs_order(outputs)
```

### Comparing `generate_sequences-0.0.6/generate_sequences.egg-info/PKG-INFO` & `generate_sequences-0.0.7/generate_sequences.egg-info/PKG-INFO`

 * *Files identical despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: generate-sequences
-Version: 0.0.6
+Version: 0.0.7
 Author-email: "Maged S. Al-Shaibani" <mageedsaeed1@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 https://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
@@ -216,15 +216,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: tqdm==4.66.*
 Requires-Dist: numpy>=1.24.0
 Requires-Dist: torch<2.4,>=2.2
 Provides-Extra: dev
 Requires-Dist: ruff; extra == "dev"
-Requires-Dist: mypy<1.10,>=1.0; extra == "dev"
+Requires-Dist: mypy<1.11,>=1.0; extra == "dev"
 Requires-Dist: black<25.0,>=23.0; extra == "dev"
 Requires-Dist: isort<5.14,>=5.12; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-sphinx; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: twine>=1.11.0; extra == "dev"
 Requires-Dist: build; extra == "dev"
```

### Comparing `generate_sequences-0.0.6/pyproject.toml` & `generate_sequences-0.0.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 Repository = "https://github.com/MagedSaeed/generate-sequences"
 Changelog = "https://github.com/MagedSaeed/generate-sequences/blob/main/CHANGELOG.md"
 # Documentation = "https://generate-sequences.readthedocs.io/"
 
 [project.optional-dependencies]
 dev = [
   "ruff",
-  "mypy>=1.0,<1.10",
+  "mypy>=1.0,<1.11",
   "black>=23.0,<25.0",
   "isort>=5.12,<5.14",
   "pytest",
   "pytest-sphinx",
   "pytest-cov",
   "twine>=1.11.0",
   "build",
```

