# Comparing `tmp/samples-filter-0.1.5.tar.gz` & `tmp/samples-filter-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "samples-filter-0.1.5.tar", last modified: Fri Apr 26 13:11:24 2024, max compression
+gzip compressed data, was "samples-filter-0.4.0.tar", last modified: Wed May  8 09:43:58 2024, max compression
```

## Comparing `samples-filter-0.1.5.tar` & `samples-filter-0.4.0.tar`

### file list

```diff
@@ -1,30 +1,28 @@
-drwxrwxr-x   0 r         (1000) r         (1001)        0 2024-04-26 13:11:24.917906 samples-filter-0.1.5/
--rw-r--r--   0 r         (1000) r         (1001)     1087 2024-04-26 13:06:07.000000 samples-filter-0.1.5/LICENSE.txt
--rw-rw-r--   0 r         (1000) r         (1001)    11367 2024-04-26 13:11:24.917906 samples-filter-0.1.5/PKG-INFO
--rw-r--r--   0 r         (1000) r         (1001)    10664 2024-04-26 13:06:07.000000 samples-filter-0.1.5/README.md
-drwxrwxr-x   0 r         (1000) r         (1001)        0 2024-04-26 13:11:24.889907 samples-filter-0.1.5/model/
--rw-r--r--   0 r         (1000) r         (1001)     1910 2024-04-26 13:06:07.000000 samples-filter-0.1.5/model/combine.py
--rw-r--r--   0 r         (1000) r         (1001)      128 2024-04-26 13:06:07.000000 samples-filter-0.1.5/model/inference.py
--rw-r--r--   0 r         (1000) r         (1001)     1386 2024-04-26 13:06:07.000000 samples-filter-0.1.5/model/metrics.py
--rw-r--r--   0 r         (1000) r         (1001)     1485 2024-04-26 13:06:07.000000 samples-filter-0.1.5/model/predictor.py
--rw-r--r--   0 r         (1000) r         (1001)     3155 2024-04-26 13:06:07.000000 samples-filter-0.1.5/model/train.py
-drwxrwxr-x   0 r         (1000) r         (1001)        0 2024-04-26 13:11:24.905907 samples-filter-0.1.5/objects/
--rw-r--r--   0 r         (1000) r         (1001)     1261 2024-04-26 13:06:07.000000 samples-filter-0.1.5/objects/__init__.py
--rw-r--r--   0 r         (1000) r         (1001)     1434 2024-04-26 13:06:07.000000 samples-filter-0.1.5/objects/__main__.py
--rw-r--r--   0 r         (1000) r         (1001)     2736 2024-04-26 13:06:07.000000 samples-filter-0.1.5/objects/cli.py
--rw-r--r--   0 r         (1000) r         (1001)     2757 2024-04-26 13:06:07.000000 samples-filter-0.1.5/objects/dataset.py
--rw-r--r--   0 r         (1000) r         (1001)     1479 2024-04-26 13:06:07.000000 samples-filter-0.1.5/objects/feed.py
--rw-r--r--   0 r         (1000) r         (1001)     3280 2024-04-26 13:06:07.000000 samples-filter-0.1.5/objects/filter_pipe.py
--rw-r--r--   0 r         (1000) r         (1001)     2980 2024-04-26 13:06:07.000000 samples-filter-0.1.5/objects/input.py
--rw-r--r--   0 r         (1000) r         (1001)     1433 2024-04-26 13:06:07.000000 samples-filter-0.1.5/objects/pre_filter.py
--rw-r--r--   0 r         (1000) r         (1001)     1586 2024-04-26 13:06:07.000000 samples-filter-0.1.5/objects/readme.py
--rw-r--r--   0 r         (1000) r         (1001)     1416 2024-04-26 13:06:07.000000 samples-filter-0.1.5/objects/text_prediction.py
-drwxrwxr-x   0 r         (1000) r         (1001)        0 2024-04-26 13:11:24.917906 samples-filter-0.1.5/samples_filter.egg-info/
--rw-rw-r--   0 r         (1000) r         (1001)    11367 2024-04-26 13:11:24.000000 samples-filter-0.1.5/samples_filter.egg-info/PKG-INFO
--rw-rw-r--   0 r         (1000) r         (1001)      544 2024-04-26 13:11:24.000000 samples-filter-0.1.5/samples_filter.egg-info/SOURCES.txt
--rw-rw-r--   0 r         (1000) r         (1001)        1 2024-04-26 13:11:24.000000 samples-filter-0.1.5/samples_filter.egg-info/dependency_links.txt
--rw-rw-r--   0 r         (1000) r         (1001)       58 2024-04-26 13:11:24.000000 samples-filter-0.1.5/samples_filter.egg-info/entry_points.txt
--rw-rw-r--   0 r         (1000) r         (1001)       22 2024-04-26 13:11:24.000000 samples-filter-0.1.5/samples_filter.egg-info/requires.txt
--rw-rw-r--   0 r         (1000) r         (1001)       14 2024-04-26 13:11:24.000000 samples-filter-0.1.5/samples_filter.egg-info/top_level.txt
--rw-rw-r--   0 r         (1000) r         (1001)       38 2024-04-26 13:11:24.917906 samples-filter-0.1.5/setup.cfg
--rw-r--r--   0 r         (1000) r         (1001)     2538 2024-04-26 13:06:07.000000 samples-filter-0.1.5/setup.py
+drwxrwxr-x   0 r         (1000) r         (1001)        0 2024-05-08 09:43:58.739187 samples-filter-0.4.0/
+-rw-r--r--   0 r         (1000) r         (1001)     1087 2024-05-08 09:38:45.000000 samples-filter-0.4.0/LICENSE.txt
+-rw-rw-r--   0 r         (1000) r         (1001)     4145 2024-05-08 09:43:58.739187 samples-filter-0.4.0/PKG-INFO
+-rw-r--r--   0 r         (1000) r         (1001)     3442 2024-05-08 09:38:45.000000 samples-filter-0.4.0/README.md
+drwxrwxr-x   0 r         (1000) r         (1001)        0 2024-05-08 09:43:58.723187 samples-filter-0.4.0/samples_filter.egg-info/
+-rw-rw-r--   0 r         (1000) r         (1001)     4145 2024-05-08 09:43:58.000000 samples-filter-0.4.0/samples_filter.egg-info/PKG-INFO
+-rw-rw-r--   0 r         (1000) r         (1001)      495 2024-05-08 09:43:58.000000 samples-filter-0.4.0/samples_filter.egg-info/SOURCES.txt
+-rw-rw-r--   0 r         (1000) r         (1001)        1 2024-05-08 09:43:58.000000 samples-filter-0.4.0/samples_filter.egg-info/dependency_links.txt
+-rw-rw-r--   0 r         (1000) r         (1001)       54 2024-05-08 09:43:58.000000 samples-filter-0.4.0/samples_filter.egg-info/entry_points.txt
+-rw-rw-r--   0 r         (1000) r         (1001)       22 2024-05-08 09:43:58.000000 samples-filter-0.4.0/samples_filter.egg-info/requires.txt
+-rw-rw-r--   0 r         (1000) r         (1001)        4 2024-05-08 09:43:58.000000 samples-filter-0.4.0/samples_filter.egg-info/top_level.txt
+-rw-rw-r--   0 r         (1000) r         (1001)       38 2024-05-08 09:43:58.739187 samples-filter-0.4.0/setup.cfg
+-rw-r--r--   0 r         (1000) r         (1001)     2521 2024-05-08 09:38:45.000000 samples-filter-0.4.0/setup.py
+drwxrwxr-x   0 r         (1000) r         (1001)        0 2024-05-08 09:43:58.739187 samples-filter-0.4.0/src/
+-rw-r--r--   0 r         (1000) r         (1001)     1261 2024-05-08 09:38:45.000000 samples-filter-0.4.0/src/__init__.py
+-rw-r--r--   0 r         (1000) r         (1001)     1430 2024-05-08 09:38:45.000000 samples-filter-0.4.0/src/__main__.py
+-rw-r--r--   0 r         (1000) r         (1001)     2781 2024-05-08 09:38:45.000000 samples-filter-0.4.0/src/cli.py
+-rw-r--r--   0 r         (1000) r         (1001)     2757 2024-05-08 09:38:45.000000 samples-filter-0.4.0/src/dataset.py
+-rw-r--r--   0 r         (1000) r         (1001)     2134 2024-05-08 09:38:45.000000 samples-filter-0.4.0/src/feed.py
+-rw-r--r--   0 r         (1000) r         (1001)     3452 2024-05-08 09:38:45.000000 samples-filter-0.4.0/src/filter_pipe.py
+-rw-r--r--   0 r         (1000) r         (1001)     2980 2024-05-08 09:38:45.000000 samples-filter-0.4.0/src/input.py
+-rw-r--r--   0 r         (1000) r         (1001)     1405 2024-05-08 09:38:45.000000 samples-filter-0.4.0/src/model_map.py
+-rw-r--r--   0 r         (1000) r         (1001)     1433 2024-05-08 09:38:45.000000 samples-filter-0.4.0/src/pre_filter.py
+-rw-r--r--   0 r         (1000) r         (1001)     1586 2024-05-08 09:38:45.000000 samples-filter-0.4.0/src/readme.py
+-rw-r--r--   0 r         (1000) r         (1001)     1792 2024-05-08 09:38:45.000000 samples-filter-0.4.0/src/remote_asset.py
+-rw-r--r--   0 r         (1000) r         (1001)     1561 2024-05-08 09:38:45.000000 samples-filter-0.4.0/src/rf_model.py
+-rw-r--r--   0 r         (1000) r         (1001)     1596 2024-05-08 09:38:45.000000 samples-filter-0.4.0/src/text_prediction.py
+-rw-r--r--   0 r         (1000) r         (1001)     1493 2024-05-08 09:38:45.000000 samples-filter-0.4.0/src/transformer_model.py
```

### Comparing `samples-filter-0.1.5/LICENSE.txt` & `samples-filter-0.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `samples-filter-0.1.5/model/metrics.py` & `samples-filter-0.4.0/src/text_prediction.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,33 +1,43 @@
-# MIT License
+# The MIT License (MIT)
 #
 # Copyright (c) 2024 Aliaksei Bialiauski
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
 #
-# The above copyright notice and this permission notice shall be included in all
-# copies or substantial portions of the Software.
+# The above copyright notice and this permission notice shall be included
+# in all copies or substantial portions of the Software.
 #
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# FITNESS FOR A PARTICULAR PURPOSE AND NON-INFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 """
-Evaluate metrics.
+Model prediction in simple text format.
 """
-import evaluate
-import numpy
 
-def metrics(eval):
-    predictions, labels = eval
-    predictions = numpy.argmax(predictions, axis=1)
-    accuracy = evaluate.load("accuracy")
-    return accuracy.compute(predictions=predictions, references=labels)
+
+class TextPrediction:
+    def __init__(self, pred, name):
+        self.pred = pred
+        self.model = name
+
+    def as_text(self):
+        if self.model == "rf":
+            if self.pred == [0]:
+                label = "sample"
+            else:
+                label = "real"
+        elif self.pred[0]["label"] == "POSITIVE":
+            label = "sample"
+        else:
+            label = "real"
+        return label
```

### Comparing `samples-filter-0.1.5/model/predictor.py` & `samples-filter-0.4.0/src/rf_model.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,41 +1,40 @@
-# MIT License
+# The MIT License (MIT)
 #
 # Copyright (c) 2024 Aliaksei Bialiauski
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
 #
-# The above copyright notice and this permission notice shall be included in all
-# copies or substantial portions of the Software.
+# The above copyright notice and this permission notice shall be included
+# in all copies or substantial portions of the Software.
 #
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# FITNESS FOR A PARTICULAR PURPOSE AND NON-INFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
+import joblib
+
+from .remote_asset import RemoteAsset
 
 """
-Predict.
+Random Forest Model.
 """
-from transformers import pipeline
 
 
-class Predictor:
-    def __init__(self, ref="h1alexbel/github-samples-classifier"):
-        self.ref = ref
-
-    def predict(self, text):
-        classifier = pipeline(
-            "sentiment-analysis",
-            model=self.ref
-        )
-        return classifier(text)
+class RfModel:
+    def __init__(self, vec="rf-vec.joblib", ref="rf-classifier.joblib"):
+        self.vectorizer = joblib.load(RemoteAsset(vec).dump())
+        self.model = joblib.load(RemoteAsset(ref).dump())
+
+    def predict(self, input):
+        return self.model.predict(self.vectorizer.transform([input]))
 
-    def model(self):
-        return self.ref
+    def name(self):
+        return "rf"
```

### Comparing `samples-filter-0.1.5/objects/__init__.py` & `samples-filter-0.4.0/src/__init__.py`

 * *Files identical despite different names*

### Comparing `samples-filter-0.1.5/objects/__main__.py` & `samples-filter-0.4.0/src/__main__.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 """
 Command-line entry point.
 """
-from objects import cli, NAME
+from src import cli, NAME
 
 # Entry point.
 def main():
     """
     Main entry point for the command-line interface.
 
     This function initializes and runs the command-line interface application.
```

### Comparing `samples-filter-0.1.5/objects/cli.py` & `samples-filter-0.4.0/src/cli.py`

 * *Files 9% similar despite different names*

```diff
@@ -23,20 +23,17 @@
 """
 Cli runner.
 """
 from typing import Optional
 
 import typer
 
+from .model_map import ModelMap
 from .filter_pipe import FilterPipe
-from model.predictor import Predictor
-from .dataset import Dataset
-from objects import NAME, VERSION
-from .pre_filter import PreFilter
-from .input import Input
+from src import NAME, VERSION
 
 app = typer.Typer()
 
 
 def _version_callback(value: bool) -> None:
     if value:
         typer.echo(f"{VERSION}")
@@ -46,27 +43,31 @@
 @app.command()
 def filter(
         repositories: str = typer.Option(
             ..., "--repositories", help="Path to the input repositories CSV file."
         ),
         out: str = typer.Option(
             ..., "--out", help="Path to the output CSV file."
+        ),
+        model: str = typer.Option(
+            "rf", "--model", help="Which ML model to use."
         )
 ):
     """
     Filter repositories.
     """
+    models = ModelMap().build()
     # @todo #18:30min Find effective way for processing readme.
     #  For now we are not processing readme because of
     #  <a href="https://github.com/h1alexbel/samples-filter/issues/39">this</a>.
     #  We need to find actual way to process readme too since it can be crucial
     #  data as model input. Let's study papers, outlined
     #  <a href="https://github.com/yegor256/cam/issues/227#issue-2200080559">here</a>
     #  first, rethink it and try to implement here.
-    FilterPipe(repositories, out, Predictor(), typer).apply()
+    FilterPipe(repositories, out, models.get(model), typer).apply()
 
 
 # Run it.
 @app.callback()
 def main(
         # pylint: disable=unused-argument
         version: Optional[bool] = typer.Option(
```

#### html2text {}

```diff
@@ -9,23 +9,24 @@
 or substantial portions of the Software. # # THE SOFTWARE IS PROVIDED "AS IS",
 WITHOUT WARRANTY OF ANY KIND, EXPRESS OR # IMPLIED, INCLUDING BUT NOT LIMITED
 TO THE WARRANTIES OF MERCHANTABILITY, # FITNESS FOR A PARTICULAR PURPOSE AND
 NON-INFRINGEMENT. IN NO EVENT SHALL THE # AUTHORS OR COPYRIGHT HOLDERS BE
 LIABLE FOR ANY CLAIM, DAMAGES OR OTHER # LIABILITY, WHETHER IN AN ACTION OF
 CONTRACT, TORT OR OTHERWISE, ARISING FROM, # OUT OF OR IN CONNECTION WITH THE
 SOFTWARE OR THE USE OR OTHER DEALINGS IN THE # SOFTWARE. """ Cli runner. """
-from typing import Optional import typer from .filter_pipe import FilterPipe
-from model.predictor import Predictor from .dataset import Dataset from objects
-import NAME, VERSION from .pre_filter import PreFilter from .input import Input
-app = typer.Typer() def _version_callback(value: bool) -> None: if value:
-typer.echo(f"{VERSION}") raise typer.Exit() @app.command() def filter
-( repositories: str = typer.Option( ..., "--repositories", help="Path to the
-input repositories CSV file." ), out: str = typer.Option( ..., "--out",
-help="Path to the output CSV file." ) ): """ Filter repositories. """ # @todo
+from typing import Optional import typer from .model_map import ModelMap from
+.filter_pipe import FilterPipe from src import NAME, VERSION app = typer.Typer
+() def _version_callback(value: bool) -> None: if value: typer.echo(f"
+{VERSION}") raise typer.Exit() @app.command() def filter( repositories: str =
+typer.Option( ..., "--repositories", help="Path to the input repositories CSV
+file." ), out: str = typer.Option( ..., "--out", help="Path to the output CSV
+file." ), model: str = typer.Option( "rf", "--model", help="Which ML model to
+use." ) ): """ Filter repositories. """ models = ModelMap().build() # @todo
 #18:30min Find effective way for processing readme. # For now we are not
 processing readme because of # _t_h_i_s. # We need to find actual way to process
 readme too since it can be crucial # data as model input. Let's study papers,
 outlined # _h_e_r_e # first, rethink it and try to implement here. FilterPipe
-(repositories, out, Predictor(), typer).apply() # Run it. @app.callback() def
-main( # pylint: disable=unused-argument version: Optional[bool] = typer.Option
-( None, "--version", help="Show the application's version and exit.",
-callback=_version_callback, is_eager=True, ) ) -> None: f""" {NAME} """ return
+(repositories, out, models.get(model), typer).apply() # Run it. @app.callback()
+def main( # pylint: disable=unused-argument version: Optional[bool] =
+typer.Option( None, "--version", help="Show the application's version and
+exit.", callback=_version_callback, is_eager=True, ) ) -> None: f""" {NAME} """
+return
```

### Comparing `samples-filter-0.1.5/objects/dataset.py` & `samples-filter-0.4.0/src/dataset.py`

 * *Files identical despite different names*

### Comparing `samples-filter-0.1.5/objects/feed.py` & `samples-filter-0.4.0/src/pre_filter.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,26 +15,23 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NON-INFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
-import csv
 
 """
-Feed.
+Prepares outputs before running filters.
 """
+import os.path
 
 
-class Feed:
-    def __init__(self, file):
-        self.file = file
+class PreFilter:
+    def __init__(self, out):
+        self.out = out
 
-    def read(self):
-        with open(self.file, "r") as input:
-            reader = csv.DictReader(input)
-            feed = []
-            for row in reader:
-                name = row["full_name"]
-                feed.append(name)
-            return feed
+    def prepare(self):
+        if not os.path.exists("pipeline"):
+            os.makedirs("pipeline")
+        with open(self.out, "w") as file:
+            file.write("")
```

### Comparing `samples-filter-0.1.5/objects/filter_pipe.py` & `samples-filter-0.4.0/src/filter_pipe.py`

 * *Files 14% similar despite different names*

```diff
@@ -26,49 +26,53 @@
 
 """
 Filter pipe.
 """
 
 
 class FilterPipe:
-    def __init__(self, repos, output, predictor, typer):
+    def __init__(self, repos, output, mdl, typer):
         self.repos = repos
         self.output = output
-        self.predictor = predictor
+        self.model = mdl
         self.typer = typer
 
     # @todo #18:60min Create integration test case for filter_pipe.py.
     #  We should create some sort of integration test that checks filtering
     #  together with model prediction, files creation and other things happening
     #  in #apply(). Don't forget to remove this puzzle.
     def apply(self):
-        self.typer.echo(f"Filtering {self.repos}...")
+        instance = self.model()
+        self.typer.echo(f"Filtering {self.repos} with {instance.name()}...")
         feed = Feed(self.repos).read()
         with open("predictions.csv", "w") as predictions:
             writer = csv.DictWriter(
                 predictions,
-                fieldnames=["candidate", "prediction", "model"]
+                fieldnames=["candidate", "input", "prediction", "model"]
             )
             writer.writeheader()
             samples = []
             self.typer.echo(
                 f"Predicting... (all predictions will be saved into {predictions.name})"
             )
             for candidate in feed:
-                prediction = self.predictor.predict(candidate)
+                identifier = candidate["id"]
+                text = candidate["input"]
+                prediction = instance.predict(text)
                 log = {
-                    "candidate": candidate,
+                    "candidate": identifier,
+                    "input": text,
                     "prediction": prediction,
-                    "model": self.predictor.model()
+                    "model": instance.name()
                 }
                 writer.writerow(log)
-                answer = TextPrediction(prediction).as_text()
-                self.typer.echo(f"{candidate} classified as {answer}")
+                answer = TextPrediction(prediction, instance.name()).as_text()
+                self.typer.echo(f"{identifier} classified as {answer}")
                 if answer == "sample":
-                    samples.append(candidate)
+                    samples.append(identifier)
         self.typer.echo(f"found {len(samples)} samples")
         with open(self.repos, "r") as source, open(self.output, "w") as target:
             reader = csv.DictReader(source)
             writer = csv.DictWriter(target, fieldnames=reader.fieldnames)
             writer.writeheader()
             for row in reader:
                 identifier = row["full_name"]
```

### Comparing `samples-filter-0.1.5/objects/input.py` & `samples-filter-0.4.0/src/input.py`

 * *Files identical despite different names*

### Comparing `samples-filter-0.1.5/objects/pre_filter.py` & `samples-filter-0.4.0/src/transformer_model.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,23 +15,24 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NON-INFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
+from transformers import pipeline
 
 """
-Prepares outputs before running filters.
+Transformer model for predictions.
 """
-import os.path
 
 
-class PreFilter:
-    def __init__(self, out):
-        self.out = out
-
-    def prepare(self):
-        if not os.path.exists("pipeline"):
-            os.makedirs("pipeline")
-        with open(self.out, "w") as file:
-            file.write("")
+class TransformerModel:
+
+    def __init__(self, ref="h1alexbel/github-samples-tclassifier"):
+        self.classifier = pipeline("sentiment-analysis", model=ref)
+
+    def predict(self, input):
+        return self.classifier.predict(input)
+
+    def name(self):
+        return "transformer"
```

### Comparing `samples-filter-0.1.5/objects/readme.py` & `samples-filter-0.4.0/src/readme.py`

 * *Files identical despite different names*

### Comparing `samples-filter-0.1.5/setup.py` & `samples-filter-0.4.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,22 +42,22 @@
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='samples-filter',
     version=actual,
-    packages=['objects', 'model'],
+    packages=['src'],
     install_requires=[
         'typer',
         'pyarrow==16.0.0'
     ],
     entry_points={
         'console_scripts': [
-            'samples-filter=objects.__main__:main',
+            'samples-filter=src.__main__:main',
         ],
     },
     author='Aliaksei Bialiauski',
     author_email='aliaksei.bialiauski@hey.com',
     description=
     'Command-line filter for GitHub repositories that contain "samples",'
     ' instead of real project or framework or library',
```

