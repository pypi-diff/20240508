# Comparing `tmp/sae_lens-1.6.0.tar.gz` & `tmp/sae_lens-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sae_lens-1.6.0.tar", max compression
+gzip compressed data, was "sae_lens-1.6.1.tar", max compression
```

## Comparing `sae_lens-1.6.0.tar` & `sae_lens-1.6.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     1069 2024-05-07 14:11:44.743109 sae_lens-1.6.0/LICENSE
--rw-r--r--   0        0        0     2553 2024-05-07 14:11:44.743109 sae_lens-1.6.0/README.md
--rw-r--r--   0        0        0     1917 2024-05-07 14:11:46.079116 sae_lens-1.6.0/pyproject.toml
--rw-r--r--   0        0        0      939 2024-05-07 14:11:46.079116 sae_lens-1.6.0/sae_lens/__init__.py
--rw-r--r--   0        0        0        0 2024-05-07 14:11:44.755109 sae_lens-1.6.0/sae_lens/analysis/__init__.py
--rw-r--r--   0        0        0    15645 2024-05-07 14:11:44.755109 sae_lens-1.6.0/sae_lens/analysis/dashboard_runner.py
--rw-r--r--   0        0        0     3535 2024-05-07 14:11:44.755109 sae_lens-1.6.0/sae_lens/analysis/feature_statistics.py
--rw-r--r--   0        0        0    17062 2024-05-07 14:11:44.755109 sae_lens-1.6.0/sae_lens/analysis/neuronpedia_integration.py
--rw-r--r--   0        0        0    20134 2024-05-07 14:11:44.755109 sae_lens-1.6.0/sae_lens/analysis/neuronpedia_runner.py
--rw-r--r--   0        0        0    18275 2024-05-07 14:11:44.755109 sae_lens-1.6.0/sae_lens/analysis/tsea.py
--rw-r--r--   0        0        0     1164 2024-05-07 14:11:44.755109 sae_lens-1.6.0/sae_lens/pretrained_saes.yaml
--rw-r--r--   0        0        0        0 2024-05-07 14:11:44.755109 sae_lens-1.6.0/sae_lens/toolkit/__init__.py
--rw-r--r--   0        0        0     2674 2024-05-07 14:11:44.755109 sae_lens-1.6.0/sae_lens/toolkit/pretrained_sae_loaders.py
--rw-r--r--   0        0        0     6643 2024-05-07 14:11:44.755109 sae_lens-1.6.0/sae_lens/toolkit/pretrained_saes.py
--rw-r--r--   0        0        0     1143 2024-05-07 14:11:44.755109 sae_lens-1.6.0/sae_lens/toolkit/pretrained_saes_directory.py
--rw-r--r--   0        0        0        0 2024-05-07 14:11:44.755109 sae_lens-1.6.0/sae_lens/training/__init__.py
--rw-r--r--   0        0        0      471 2024-05-07 14:11:44.755109 sae_lens-1.6.0/sae_lens/training/activation_functions.py
--rw-r--r--   0        0        0    20435 2024-05-07 14:11:44.755109 sae_lens-1.6.0/sae_lens/training/activations_store.py
--rw-r--r--   0        0        0     5974 2024-05-07 14:11:44.755109 sae_lens-1.6.0/sae_lens/training/cache_activations_runner.py
--rw-r--r--   0        0        0    12972 2024-05-07 14:11:44.755109 sae_lens-1.6.0/sae_lens/training/config.py
--rw-r--r--   0        0        0     7439 2024-05-07 14:11:44.755109 sae_lens-1.6.0/sae_lens/training/evals.py
--rw-r--r--   0        0        0     3747 2024-05-07 14:11:44.755109 sae_lens-1.6.0/sae_lens/training/geometric_median.py
--rw-r--r--   0        0        0     3100 2024-05-07 14:11:44.755109 sae_lens-1.6.0/sae_lens/training/lm_runner.py
--rw-r--r--   0        0        0     1020 2024-05-07 14:11:44.755109 sae_lens-1.6.0/sae_lens/training/load_model.py
--rw-r--r--   0        0        0     5065 2024-05-07 14:11:44.755109 sae_lens-1.6.0/sae_lens/training/optim.py
--rw-r--r--   0        0        0     8284 2024-05-07 14:11:44.755109 sae_lens-1.6.0/sae_lens/training/sae_group.py
--rw-r--r--   0        0        0     2319 2024-05-07 14:11:44.755109 sae_lens-1.6.0/sae_lens/training/session_loader.py
--rw-r--r--   0        0        0    20000 2024-05-07 14:11:44.755109 sae_lens-1.6.0/sae_lens/training/sparse_autoencoder.py
--rw-r--r--   0        0        0     3276 2024-05-07 14:11:44.755109 sae_lens-1.6.0/sae_lens/training/toy_model_runner.py
--rw-r--r--   0        0        0    17362 2024-05-07 14:11:44.755109 sae_lens-1.6.0/sae_lens/training/toy_models.py
--rw-r--r--   0        0        0    30305 2024-05-07 14:11:44.755109 sae_lens-1.6.0/sae_lens/training/train_sae_on_language_model.py
--rw-r--r--   0        0        0     5002 2024-05-07 14:11:44.755109 sae_lens-1.6.0/sae_lens/training/train_sae_on_toy_model.py
--rw-r--r--   0        0        0      423 2024-05-07 14:11:44.755109 sae_lens-1.6.0/sae_lens/training/utils.py
--rw-r--r--   0        0        0     4196 1970-01-01 00:00:00.000000 sae_lens-1.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-07 16:44:02.726256 sae_lens-1.6.1/LICENSE
+-rw-r--r--   0        0        0     2553 2024-05-07 16:44:02.726256 sae_lens-1.6.1/README.md
+-rw-r--r--   0        0        0     1917 2024-05-07 16:44:04.030263 sae_lens-1.6.1/pyproject.toml
+-rw-r--r--   0        0        0      939 2024-05-07 16:44:04.030263 sae_lens-1.6.1/sae_lens/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-07 16:44:02.738256 sae_lens-1.6.1/sae_lens/analysis/__init__.py
+-rw-r--r--   0        0        0    15645 2024-05-07 16:44:02.738256 sae_lens-1.6.1/sae_lens/analysis/dashboard_runner.py
+-rw-r--r--   0        0        0     3535 2024-05-07 16:44:02.738256 sae_lens-1.6.1/sae_lens/analysis/feature_statistics.py
+-rw-r--r--   0        0        0    17062 2024-05-07 16:44:02.738256 sae_lens-1.6.1/sae_lens/analysis/neuronpedia_integration.py
+-rw-r--r--   0        0        0    20134 2024-05-07 16:44:02.738256 sae_lens-1.6.1/sae_lens/analysis/neuronpedia_runner.py
+-rw-r--r--   0        0        0    18275 2024-05-07 16:44:02.738256 sae_lens-1.6.1/sae_lens/analysis/tsea.py
+-rw-r--r--   0        0        0     1164 2024-05-07 16:44:02.738256 sae_lens-1.6.1/sae_lens/pretrained_saes.yaml
+-rw-r--r--   0        0        0        0 2024-05-07 16:44:02.738256 sae_lens-1.6.1/sae_lens/toolkit/__init__.py
+-rw-r--r--   0        0        0     2674 2024-05-07 16:44:02.738256 sae_lens-1.6.1/sae_lens/toolkit/pretrained_sae_loaders.py
+-rw-r--r--   0        0        0     6643 2024-05-07 16:44:02.738256 sae_lens-1.6.1/sae_lens/toolkit/pretrained_saes.py
+-rw-r--r--   0        0        0     1143 2024-05-07 16:44:02.738256 sae_lens-1.6.1/sae_lens/toolkit/pretrained_saes_directory.py
+-rw-r--r--   0        0        0        0 2024-05-07 16:44:02.738256 sae_lens-1.6.1/sae_lens/training/__init__.py
+-rw-r--r--   0        0        0      471 2024-05-07 16:44:02.738256 sae_lens-1.6.1/sae_lens/training/activation_functions.py
+-rw-r--r--   0        0        0    20435 2024-05-07 16:44:02.738256 sae_lens-1.6.1/sae_lens/training/activations_store.py
+-rw-r--r--   0        0        0     5974 2024-05-07 16:44:02.738256 sae_lens-1.6.1/sae_lens/training/cache_activations_runner.py
+-rw-r--r--   0        0        0    12972 2024-05-07 16:44:02.738256 sae_lens-1.6.1/sae_lens/training/config.py
+-rw-r--r--   0        0        0     6544 2024-05-07 16:44:02.738256 sae_lens-1.6.1/sae_lens/training/evals.py
+-rw-r--r--   0        0        0     3747 2024-05-07 16:44:02.738256 sae_lens-1.6.1/sae_lens/training/geometric_median.py
+-rw-r--r--   0        0        0     3100 2024-05-07 16:44:02.738256 sae_lens-1.6.1/sae_lens/training/lm_runner.py
+-rw-r--r--   0        0        0     1020 2024-05-07 16:44:02.738256 sae_lens-1.6.1/sae_lens/training/load_model.py
+-rw-r--r--   0        0        0     5065 2024-05-07 16:44:02.738256 sae_lens-1.6.1/sae_lens/training/optim.py
+-rw-r--r--   0        0        0     8284 2024-05-07 16:44:02.738256 sae_lens-1.6.1/sae_lens/training/sae_group.py
+-rw-r--r--   0        0        0     2319 2024-05-07 16:44:02.738256 sae_lens-1.6.1/sae_lens/training/session_loader.py
+-rw-r--r--   0        0        0    20000 2024-05-07 16:44:02.738256 sae_lens-1.6.1/sae_lens/training/sparse_autoencoder.py
+-rw-r--r--   0        0        0     3276 2024-05-07 16:44:02.738256 sae_lens-1.6.1/sae_lens/training/toy_model_runner.py
+-rw-r--r--   0        0        0    17362 2024-05-07 16:44:02.738256 sae_lens-1.6.1/sae_lens/training/toy_models.py
+-rw-r--r--   0        0        0    30305 2024-05-07 16:44:02.738256 sae_lens-1.6.1/sae_lens/training/train_sae_on_language_model.py
+-rw-r--r--   0        0        0     5002 2024-05-07 16:44:02.738256 sae_lens-1.6.1/sae_lens/training/train_sae_on_toy_model.py
+-rw-r--r--   0        0        0      423 2024-05-07 16:44:02.738256 sae_lens-1.6.1/sae_lens/training/utils.py
+-rw-r--r--   0        0        0     4196 1970-01-01 00:00:00.000000 sae_lens-1.6.1/PKG-INFO
```

### Comparing `sae_lens-1.6.0/LICENSE` & `sae_lens-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sae_lens-1.6.0/README.md` & `sae_lens-1.6.1/README.md`

 * *Files identical despite different names*

### Comparing `sae_lens-1.6.0/pyproject.toml` & `sae_lens-1.6.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sae-lens"
-version = "1.6.0"
+version = "1.6.1"
 description = "Training and Analyzing Sparse Autoencoders (SAEs)"
 authors = ["Joseph Bloom"]
 readme = "README.md"
 packages = [{include = "sae_lens"}]
 include = ["pretrained_saes.yaml"]
 
 [tool.poetry.dependencies]
```

### Comparing `sae_lens-1.6.0/sae_lens/__init__.py` & `sae_lens-1.6.1/sae_lens/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "1.6.0"
+__version__ = "1.6.1"
 
 from .training.activations_store import ActivationsStore
 from .training.cache_activations_runner import CacheActivationsRunner
 from .training.config import CacheActivationsRunnerConfig, LanguageModelSAERunnerConfig
 from .training.evals import run_evals
 from .training.lm_runner import language_model_sae_runner
 from .training.sae_group import SparseAutoencoderDictionary
```

### Comparing `sae_lens-1.6.0/sae_lens/analysis/dashboard_runner.py` & `sae_lens-1.6.1/sae_lens/analysis/dashboard_runner.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.6.0/sae_lens/analysis/feature_statistics.py` & `sae_lens-1.6.1/sae_lens/analysis/feature_statistics.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.6.0/sae_lens/analysis/neuronpedia_integration.py` & `sae_lens-1.6.1/sae_lens/analysis/neuronpedia_integration.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.6.0/sae_lens/analysis/neuronpedia_runner.py` & `sae_lens-1.6.1/sae_lens/analysis/neuronpedia_runner.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.6.0/sae_lens/analysis/tsea.py` & `sae_lens-1.6.1/sae_lens/analysis/tsea.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.6.0/sae_lens/pretrained_saes.yaml` & `sae_lens-1.6.1/sae_lens/pretrained_saes.yaml`

 * *Files identical despite different names*

### Comparing `sae_lens-1.6.0/sae_lens/toolkit/pretrained_sae_loaders.py` & `sae_lens-1.6.1/sae_lens/toolkit/pretrained_sae_loaders.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.6.0/sae_lens/toolkit/pretrained_saes.py` & `sae_lens-1.6.1/sae_lens/toolkit/pretrained_saes.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.6.0/sae_lens/toolkit/pretrained_saes_directory.py` & `sae_lens-1.6.1/sae_lens/toolkit/pretrained_saes_directory.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.6.0/sae_lens/training/activations_store.py` & `sae_lens-1.6.1/sae_lens/training/activations_store.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.6.0/sae_lens/training/cache_activations_runner.py` & `sae_lens-1.6.1/sae_lens/training/cache_activations_runner.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.6.0/sae_lens/training/config.py` & `sae_lens-1.6.1/sae_lens/training/config.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.6.0/sae_lens/training/evals.py` & `sae_lens-1.6.1/sae_lens/training/evals.py`

 * *Files 11% similar despite different names*

```diff
@@ -35,15 +35,14 @@
         n_batches=10,
     )
 
     recons_score = losses_df["score"].mean()
     ntp_loss = losses_df["loss"].mean()
     recons_loss = losses_df["recons_loss"].mean()
     zero_abl_loss = losses_df["zero_abl_loss"].mean()
-    d_kl = losses_df["d_kl"].mean()
 
     # get cache
     _, cache = model.run_with_cache(
         eval_tokens,
         prepend_bos=False,
         names_filter=[hook_point_eval, hook_point],
         **sparse_autoencoder.cfg.model_kwargs,
@@ -81,16 +80,14 @@
         f"weights/W_dec_norms{suffix}": wandb.Histogram(W_dec_norm_dist),
         f"weights/b_e{suffix}": wandb.Histogram(b_e_dist),
         # CE Loss
         f"metrics/CE_loss_score{suffix}": recons_score,
         f"metrics/ce_loss_without_sae{suffix}": ntp_loss,
         f"metrics/ce_loss_with_sae{suffix}": recons_loss,
         f"metrics/ce_loss_with_ablation{suffix}": zero_abl_loss,
-        # KL divergence against intact model
-        f"metrics/kl_div{suffix}": d_kl,
     }
 
     if wandb.run is not None:
         wandb.log(
             metrics,
             step=n_training_steps,
         )
@@ -103,47 +100,44 @@
     model: HookedRootModule,
     activation_store: ActivationsStore,
     n_batches: int = 100,
 ):
     losses = []
     for _ in range(n_batches):
         batch_tokens = activation_store.get_batch_tokens()
-        score, loss, recons_loss, zero_abl_loss, d_kl = get_recons_loss(
+        score, loss, recons_loss, zero_abl_loss = get_recons_loss(
             sparse_autoencoder, model, batch_tokens
         )
         losses.append(
             (
                 score.mean().item(),
                 loss.mean().item(),
                 recons_loss.mean().item(),
                 zero_abl_loss.mean().item(),
-                d_kl.mean().item(),
             )
         )
 
     losses = pd.DataFrame(
-        losses,
-        columns=cast(Any, ["score", "loss", "recons_loss", "zero_abl_loss", "d_kl"]),
+        losses, columns=cast(Any, ["score", "loss", "recons_loss", "zero_abl_loss"])
     )
 
     return losses
 
 
 @torch.no_grad()
 def get_recons_loss(
     sparse_autoencoder: SparseAutoencoder,
     model: HookedRootModule,
     batch_tokens: torch.Tensor,
 ):
     hook_point = sparse_autoencoder.cfg.hook_point
-    model_outs = model(
-        batch_tokens, return_type="both", **sparse_autoencoder.cfg.model_kwargs
+    loss = model(
+        batch_tokens, return_type="loss", **sparse_autoencoder.cfg.model_kwargs
     )
     head_index = sparse_autoencoder.cfg.hook_point_head_index
-    loss = model_outs.loss
 
     def standard_replacement_hook(activations: torch.Tensor, hook: Any):
         activations = sparse_autoencoder.forward(activations).sae_out.to(
             activations.dtype
         )
         return activations
 
@@ -168,50 +162,34 @@
         if head_index is None:
             replacement_hook = all_head_replacement_hook
         else:
             replacement_hook = single_head_replacement_hook
     else:
         replacement_hook = standard_replacement_hook
 
-    recons_outs = model.run_with_hooks(
+    recons_loss = model.run_with_hooks(
         batch_tokens,
-        return_type="both",
+        return_type="loss",
         fwd_hooks=[(hook_point, partial(replacement_hook))],
         **sparse_autoencoder.cfg.model_kwargs,
     )
-    recons_loss = recons_outs.loss
 
     zero_abl_loss = model.run_with_hooks(
         batch_tokens,
         return_type="loss",
         fwd_hooks=[(hook_point, zero_ablate_hook)],
         **sparse_autoencoder.cfg.model_kwargs,
     )
 
     div_val = zero_abl_loss - loss
     div_val[torch.abs(div_val) < 0.0001] = 1.0
 
     score = (zero_abl_loss - recons_loss) / div_val
 
-    # KL divergence
-    model_logits = model_outs.logits  # [batch, pos, d_vocab]
-    model_logprobs = torch.nn.functional.log_softmax(model_logits, dim=-1)
-    recons_logits = recons_outs.logits
-    recons_logprobs = torch.nn.functional.log_softmax(recons_logits, dim=-1)
-    # Note: PyTorch KL is backwards compared to the mathematical definition
-    # target distribution comes second, see
-    # https://pytorch.org/docs/stable/generated/torch.nn.functional.kl_div.html
-    d_kl = torch.nn.functional.kl_div(
-        recons_logprobs,
-        model_logprobs,
-        reduction="batchmean",
-        log_target=True,  # for numerics
-    )
-
-    return score, loss, recons_loss, zero_abl_loss, d_kl
+    return score, loss, recons_loss, zero_abl_loss
 
 
 def zero_ablate_hook(activations: torch.Tensor, hook: Any):
     activations = torch.zeros_like(activations)
     return activations
```

### Comparing `sae_lens-1.6.0/sae_lens/training/geometric_median.py` & `sae_lens-1.6.1/sae_lens/training/geometric_median.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.6.0/sae_lens/training/lm_runner.py` & `sae_lens-1.6.1/sae_lens/training/lm_runner.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.6.0/sae_lens/training/load_model.py` & `sae_lens-1.6.1/sae_lens/training/load_model.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.6.0/sae_lens/training/optim.py` & `sae_lens-1.6.1/sae_lens/training/optim.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.6.0/sae_lens/training/sae_group.py` & `sae_lens-1.6.1/sae_lens/training/sae_group.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.6.0/sae_lens/training/session_loader.py` & `sae_lens-1.6.1/sae_lens/training/session_loader.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.6.0/sae_lens/training/sparse_autoencoder.py` & `sae_lens-1.6.1/sae_lens/training/sparse_autoencoder.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.6.0/sae_lens/training/toy_model_runner.py` & `sae_lens-1.6.1/sae_lens/training/toy_model_runner.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.6.0/sae_lens/training/toy_models.py` & `sae_lens-1.6.1/sae_lens/training/toy_models.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.6.0/sae_lens/training/train_sae_on_language_model.py` & `sae_lens-1.6.1/sae_lens/training/train_sae_on_language_model.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.6.0/sae_lens/training/train_sae_on_toy_model.py` & `sae_lens-1.6.1/sae_lens/training/train_sae_on_toy_model.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.6.0/PKG-INFO` & `sae_lens-1.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sae-lens
-Version: 1.6.0
+Version: 1.6.1
 Summary: Training and Analyzing Sparse Autoencoders (SAEs)
 Author: Joseph Bloom
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

