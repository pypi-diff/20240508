# Comparing `tmp/langgraph_cli-0.1.6.tar.gz` & `tmp/langgraph_cli-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langgraph_cli-0.1.6.tar", max compression
+gzip compressed data, was "langgraph_cli-0.1.7.tar", max compression
```

## Comparing `langgraph_cli-0.1.6.tar` & `langgraph_cli-0.1.7.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       12 2024-05-02 00:35:49.772511 langgraph_cli-0.1.6/README.md
--rw-r--r--   0        0        0        0 2024-05-02 00:35:49.772849 langgraph_cli-0.1.6/langgraph_cli/__init__.py
--rw-r--r--   0        0        0     8471 2024-05-08 00:03:21.317946 langgraph_cli-0.1.6/langgraph_cli/cli.py
--rw-r--r--   0        0        0     4425 2024-05-08 01:00:33.430647 langgraph_cli-0.1.6/langgraph_cli/config.py
--rw-r--r--   0        0        0     1828 2024-05-07 23:52:26.680396 langgraph_cli-0.1.6/langgraph_cli/docker.py
--rw-r--r--   0        0        0       39 2024-05-07 23:52:21.187318 langgraph_cli-0.1.6/langgraph_cli/initdb/init.sql
--rw-r--r--   0        0        0     1024 2024-05-08 01:08:03.834308 langgraph_cli-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      443 1970-01-01 00:00:00.000000 langgraph_cli-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0       12 2024-05-02 00:35:49.772511 langgraph_cli-0.1.7/README.md
+-rw-r--r--   0        0        0        0 2024-05-02 00:35:49.772849 langgraph_cli-0.1.7/langgraph_cli/__init__.py
+-rw-r--r--   0        0        0     8629 2024-05-08 01:32:41.170439 langgraph_cli-0.1.7/langgraph_cli/cli.py
+-rw-r--r--   0        0        0     4425 2024-05-08 01:00:33.430647 langgraph_cli-0.1.7/langgraph_cli/config.py
+-rw-r--r--   0        0        0     1828 2024-05-07 23:52:26.680396 langgraph_cli-0.1.7/langgraph_cli/docker.py
+-rw-r--r--   0        0        0       39 2024-05-07 23:52:21.187318 langgraph_cli-0.1.7/langgraph_cli/initdb/init.sql
+-rw-r--r--   0        0        0     1024 2024-05-08 01:32:48.975909 langgraph_cli-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      443 1970-01-01 00:00:00.000000 langgraph_cli-0.1.7/PKG-INFO
```

### Comparing `langgraph_cli-0.1.6/langgraph_cli/cli.py` & `langgraph_cli-0.1.7/langgraph_cli/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -177,17 +177,19 @@
             shutil.rmtree(".langserve-data", ignore_errors=True)
         # run docker compose
         runner.run(exec("docker", "compose", *args, input=stdin))
 
 
 @OPT_C
 @click.option("--tag", "-t", help="Tag for the image", required=True)
+@click.option("--platform", help="Platform to build for")
 @cli.command(help="Build langgraph API server image")
 def build(
     config: pathlib.Path,
+    platform: Optional[str],
     tag: str,
 ):
     with asyncio.Runner() as runner:
         # check docker available
         try:
             runner.run(exec("docker", "--version"))
             runner.run(exec("docker", "compose", "version"))
@@ -197,14 +199,16 @@
         # apply options
         args = [
             "-f",
             "-",  # stdin
             "-t",
             tag,
         ]
+        if platform:
+            args.extend(["--platform", platform])
         with open(config) as f:
             stdin = langgraph_cli.config.config_to_docker(config, json.load(f))
         # run docker build
         runner.run(exec("docker", "build", *args, config.parent, input=stdin))
 
 
 @OPT_DEBUGGER_PORT
```

### Comparing `langgraph_cli-0.1.6/langgraph_cli/config.py` & `langgraph_cli-0.1.7/langgraph_cli/config.py`

 * *Files identical despite different names*

### Comparing `langgraph_cli-0.1.6/langgraph_cli/docker.py` & `langgraph_cli-0.1.7/langgraph_cli/docker.py`

 * *Files identical despite different names*

### Comparing `langgraph_cli-0.1.6/pyproject.toml` & `langgraph_cli-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "langgraph-cli"
-version = "0.1.6"
+version = "0.1.7"
 description = ""
 authors = ["Nuno Campos <nuno@langchain.dev>"]
 readme = "README.md"
 packages = [{include = "langgraph_cli"}]
 
 [tool.poetry.scripts]
 langgraph = "langgraph_cli.cli:cli"
```

