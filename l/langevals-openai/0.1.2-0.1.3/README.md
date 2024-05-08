# Comparing `tmp/langevals_openai-0.1.2.tar.gz` & `tmp/langevals_openai-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langevals_openai-0.1.2.tar", max compression
+gzip compressed data, was "langevals_openai-0.1.3.tar", max compression
```

## Comparing `langevals_openai-0.1.2.tar` & `langevals_openai-0.1.3.tar`

### file list

```diff
@@ -1,3 +1,3 @@
--rw-r--r--   0        0        0     4293 2024-04-28 19:56:44.504808 langevals_openai-0.1.2/langevals_openai/moderation.py
--rw-r--r--   0        0        0      463 2024-04-28 19:57:28.260482 langevals_openai-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      505 1970-01-01 00:00:00.000000 langevals_openai-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     4348 2024-05-07 14:19:44.474403 langevals_openai-0.1.3/langevals_openai/moderation.py
+-rw-r--r--   0        0        0      480 2024-05-07 14:20:49.954840 langevals_openai-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      543 1970-01-01 00:00:00.000000 langevals_openai-0.1.3/PKG-INFO
```

### Comparing `langevals_openai-0.1.2/langevals_openai/moderation.py` & `langevals_openai-0.1.3/langevals_openai/moderation.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     BaseEvaluator,
     EvaluationResult,
     SingleEvaluationResult,
     BatchEvaluationResult,
     EvaluatorEntry,
     EvaluationResultSkipped,
 )
+from tqdm import tqdm
 
 
 class OpenAIModerationEntry(EvaluatorEntry):
     input: Optional[str] = None
     output: Optional[str] = None
 
 
@@ -62,26 +63,26 @@
     category = "safety"
     env_vars = ["OPENAI_API_KEY"]
     default_settings = OpenAIModerationSettings()
     docs_url = "https://platform.openai.com/docs/guides/moderation/overview"
     is_guardrail = True
 
     def evaluate_batch(
-        self, data: list[OpenAIModerationEntry]
+        self, data: list[OpenAIModerationEntry], index = 0
     ) -> BatchEvaluationResult:
         client = OpenAI(api_key=self.get_env("OPENAI_API_KEY"))
 
         results: list[SingleEvaluationResult] = []
 
         contents = [
             "\n\n".join([entry.input or "", entry.output or ""]).strip()[0:10_000]
             for entry in data
         ]
         response = client.moderations.create(input=contents)
-        for index, moderation_result in enumerate(response.results):
+        for index, moderation_result in tqdm(enumerate(response.results), position=index):
             if not contents[index]:
                 results.append(
                     EvaluationResultSkipped(details="Input and output are both empty")
                 )
                 continue
 
             detected_categories = dict(
```

