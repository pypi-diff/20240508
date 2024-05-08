# Comparing `tmp/langgraph_cli-0.1.7.tar.gz` & `tmp/langgraph_cli-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langgraph_cli-0.1.7.tar", max compression
+gzip compressed data, was "langgraph_cli-0.1.8.tar", max compression
```

## Comparing `langgraph_cli-0.1.7.tar` & `langgraph_cli-0.1.8.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       12 2024-05-02 00:35:49.772511 langgraph_cli-0.1.7/README.md
--rw-r--r--   0        0        0        0 2024-05-02 00:35:49.772849 langgraph_cli-0.1.7/langgraph_cli/__init__.py
--rw-r--r--   0        0        0     8629 2024-05-08 01:32:41.170439 langgraph_cli-0.1.7/langgraph_cli/cli.py
--rw-r--r--   0        0        0     4425 2024-05-08 01:00:33.430647 langgraph_cli-0.1.7/langgraph_cli/config.py
--rw-r--r--   0        0        0     1828 2024-05-07 23:52:26.680396 langgraph_cli-0.1.7/langgraph_cli/docker.py
--rw-r--r--   0        0        0       39 2024-05-07 23:52:21.187318 langgraph_cli-0.1.7/langgraph_cli/initdb/init.sql
--rw-r--r--   0        0        0     1024 2024-05-08 01:32:48.975909 langgraph_cli-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      443 1970-01-01 00:00:00.000000 langgraph_cli-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0       12 2024-05-08 04:47:04.081144 langgraph_cli-0.1.8/README.md
+-rw-r--r--   0        0        0        0 2024-05-08 04:47:04.081205 langgraph_cli-0.1.8/langgraph_cli/__init__.py
+-rw-r--r--   0        0        0     8633 2024-05-08 04:47:04.081354 langgraph_cli-0.1.8/langgraph_cli/cli.py
+-rw-r--r--   0        0        0     4425 2024-05-08 04:47:04.081452 langgraph_cli-0.1.8/langgraph_cli/config.py
+-rw-r--r--   0        0        0     1828 2024-05-08 04:47:04.081513 langgraph_cli-0.1.8/langgraph_cli/docker.py
+-rw-r--r--   0        0        0       39 2024-05-08 04:47:04.081606 langgraph_cli-0.1.8/langgraph_cli/initdb/init.sql
+-rw-r--r--   0        0        0     1024 2024-05-08 04:49:17.714973 langgraph_cli-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      443 1970-01-01 00:00:00.000000 langgraph_cli-0.1.8/PKG-INFO
```

### Comparing `langgraph_cli-0.1.7/langgraph_cli/cli.py` & `langgraph_cli-0.1.8/langgraph_cli/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,15 +152,15 @@
             runner.run(exec("docker", "--version"))
             runner.run(exec("docker", "compose", "version"))
         except click.exceptions.Exit:
             click.echo("Docker not installed or not running")
             return
         # pull latest images
         if pull:
-            runner.run(exec("docker", "pull", "langchain/langserve"))
+            runner.run(exec("docker", "pull", "langchain/langgraph-api"))
         # prepare args
         stdin = langgraph_cli.docker.compose(port=port, debugger_port=debugger_port)
         args = [
             "--project-directory",
             config.parent,
             "-f",
             "-",  # stdin
```

### Comparing `langgraph_cli-0.1.7/langgraph_cli/config.py` & `langgraph_cli-0.1.8/langgraph_cli/config.py`

 * *Files identical despite different names*

### Comparing `langgraph_cli-0.1.7/langgraph_cli/docker.py` & `langgraph_cli-0.1.8/langgraph_cli/docker.py`

 * *Files identical despite different names*

### Comparing `langgraph_cli-0.1.7/pyproject.toml` & `langgraph_cli-0.1.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "langgraph-cli"
-version = "0.1.7"
+version = "0.1.8"
 description = ""
 authors = ["Nuno Campos <nuno@langchain.dev>"]
 readme = "README.md"
 packages = [{include = "langgraph_cli"}]
 
 [tool.poetry.scripts]
 langgraph = "langgraph_cli.cli:cli"
 
 [tool.poetry.dependencies]
-python = "^3.9.0,<3.12"
+python = "^3.9.0,<3.13"
 click = "^8.1.7"
 
 [tool.poetry.group.dev.dependencies]
 ruff = "^0.1.4"
 codespell = "^2.2.0"
 pytest = "^7.2.1"
 pytest-asyncio = "^0.21.1"
```

