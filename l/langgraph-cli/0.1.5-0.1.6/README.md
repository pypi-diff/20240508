# Comparing `tmp/langgraph_cli-0.1.5.tar.gz` & `tmp/langgraph_cli-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langgraph_cli-0.1.5.tar", max compression
+gzip compressed data, was "langgraph_cli-0.1.6.tar", max compression
```

## Comparing `langgraph_cli-0.1.5.tar` & `langgraph_cli-0.1.6.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       12 2024-05-02 00:35:49.772511 langgraph_cli-0.1.5/README.md
--rw-r--r--   0        0        0        0 2024-05-02 00:35:49.772849 langgraph_cli-0.1.5/langgraph_cli/__init__.py
--rw-r--r--   0        0        0     6539 2024-05-07 01:16:04.705160 langgraph_cli-0.1.5/langgraph_cli/cli.py
--rw-r--r--   0        0        0     4314 2024-05-07 01:15:31.675645 langgraph_cli-0.1.5/langgraph_cli/config.py
--rw-r--r--   0        0        0     2055 2024-05-07 01:16:04.705546 langgraph_cli-0.1.5/langgraph_cli/docker.py
--rw-r--r--   0        0        0       39 2024-05-02 00:35:49.772817 langgraph_cli-0.1.5/langgraph_cli/initdb/init.sql
--rw-r--r--   0        0        0     1024 2024-05-07 17:41:36.869928 langgraph_cli-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      443 1970-01-01 00:00:00.000000 langgraph_cli-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0       12 2024-05-02 00:35:49.772511 langgraph_cli-0.1.6/README.md
+-rw-r--r--   0        0        0        0 2024-05-02 00:35:49.772849 langgraph_cli-0.1.6/langgraph_cli/__init__.py
+-rw-r--r--   0        0        0     8471 2024-05-08 00:03:21.317946 langgraph_cli-0.1.6/langgraph_cli/cli.py
+-rw-r--r--   0        0        0     4425 2024-05-08 01:00:33.430647 langgraph_cli-0.1.6/langgraph_cli/config.py
+-rw-r--r--   0        0        0     1828 2024-05-07 23:52:26.680396 langgraph_cli-0.1.6/langgraph_cli/docker.py
+-rw-r--r--   0        0        0       39 2024-05-07 23:52:21.187318 langgraph_cli-0.1.6/langgraph_cli/initdb/init.sql
+-rw-r--r--   0        0        0     1024 2024-05-08 01:08:03.834308 langgraph_cli-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      443 1970-01-01 00:00:00.000000 langgraph_cli-0.1.6/PKG-INFO
```

### Comparing `langgraph_cli-0.1.5/langgraph_cli/cli.py` & `langgraph_cli-0.1.6/langgraph_cli/cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -175,14 +175,78 @@
         if recreate:
             args.extend(["--force-recreate", "--remove-orphans"])
             shutil.rmtree(".langserve-data", ignore_errors=True)
         # run docker compose
         runner.run(exec("docker", "compose", *args, input=stdin))
 
 
+@OPT_C
+@click.option("--tag", "-t", help="Tag for the image", required=True)
+@cli.command(help="Build langgraph API server image")
+def build(
+    config: pathlib.Path,
+    tag: str,
+):
+    with asyncio.Runner() as runner:
+        # check docker available
+        try:
+            runner.run(exec("docker", "--version"))
+            runner.run(exec("docker", "compose", "version"))
+        except click.exceptions.Exit:
+            click.echo("Docker not installed or not running")
+            return
+        # apply options
+        args = [
+            "-f",
+            "-",  # stdin
+            "-t",
+            tag,
+        ]
+        with open(config) as f:
+            stdin = langgraph_cli.config.config_to_docker(config, json.load(f))
+        # run docker build
+        runner.run(exec("docker", "build", *args, config.parent, input=stdin))
+
+
+@OPT_DEBUGGER_PORT
+@OPT_PORT
+@OPT_O
+@OPT_C
+@cli.command(help="Write k8s files", hidden=True)
+def k8s(
+    config: pathlib.Path,
+    docker_compose: Optional[pathlib.Path],
+    port: int,
+    debugger_port: Optional[int],
+):
+    with asyncio.Runner() as runner:
+        # check docker available
+        try:
+            runner.run(exec("docker", "--version"))
+            runner.run(exec("docker", "compose", "version"))
+        except click.exceptions.Exit:
+            click.echo("Docker not installed or not running")
+            return
+        # prepare args
+        stdin = langgraph_cli.docker.compose(port=port, debugger_port=debugger_port)
+        args = [
+            "-f",
+            "-",  # stdin
+        ]
+        # apply options
+        if docker_compose:
+            args.extend(["-f", str(docker_compose)])
+        args.append("convert")
+        if config:
+            with open(config) as f:
+                stdin += langgraph_cli.config.config_to_compose(config, json.load(f))
+        # run kompose convert
+        runner.run(exec("kompose", *args, input=stdin))
+
+
 @OPT_O
 @OPT_PORT
 @cli.command()
 def watch(override: pathlib.Path, port: int):
     compose = langgraph_cli.docker.compose(port=port)
 
     with asyncio.Runner() as runner:
```

### Comparing `langgraph_cli-0.1.5/langgraph_cli/config.py` & `langgraph_cli-0.1.6/langgraph_cli/config.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import json
 import os
 import pathlib
+import textwrap
 from typing import TypedDict, Union
 
 
 class Config(TypedDict):
     dependencies: list[str]
     graphs: dict[str, str]
     env: Union[dict[str, str], str]
 
 
-def config_to_compose(config_path: pathlib.Path, config: Config):
+def config_to_docker(config_path: pathlib.Path, config: Config):
     pypi_deps = [dep for dep in config["dependencies"] if not dep.startswith(".")]
     local_pkgs: dict[pathlib.Path, str] = {}
     faux_pkgs: dict[pathlib.Path, str] = {}
     pkg_names = set()
 
     for local_dep in config["dependencies"]:
         if local_dep.startswith("."):
@@ -83,31 +84,37 @@
         f"ADD {relpath} /tmp/{fullpath.name}/{fullpath.name}\n                RUN touch /tmp/{fullpath.name}/pyproject.toml"
         for fullpath, relpath in faux_pkgs.items()
     )
     local_pkgs_str = "\n".join(
         f"ADD {relpath} /tmp/{fullpath.name}"
         for fullpath, relpath in local_pkgs.items()
     )
+
+    return f"""FROM langchain/langgraph-api
+
+ENV LANGSERVE_GRAPHS='{json.dumps(config["graphs"])}'
+
+{local_pkgs_str}
+
+{faux_pkgs_str}
+
+RUN pip install {' '.join(pypi_deps)} /tmp/*"""
+
+
+def config_to_compose(config_path: pathlib.Path, config: Config):
     env_vars_str = (
         "\n".join(f"            {k}: {v}" for k, v in config["env"].items())
         if isinstance(config["env"], dict)
         else ""
     )
     env_file_str = (
         f"env_file: {config['env']}" if isinstance(config["env"], str) else ""
     )
 
     return f"""
-            LANGSERVE_GRAPHS: '{json.dumps(config["graphs"])}'
             {env_vars_str}
         {env_file_str}
         pull_policy: build
         build:
             dockerfile_inline: |
-                FROM langchain/langserve
-
-                {local_pkgs_str}
-
-                {faux_pkgs_str}
-
-                RUN pip install {' '.join(pypi_deps)} /tmp/*
+{textwrap.indent(config_to_docker(config_path, config), "                ")}
 """
```

### Comparing `langgraph_cli-0.1.5/pyproject.toml` & `langgraph_cli-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "langgraph-cli"
-version = "0.1.5"
+version = "0.1.6"
 description = ""
 authors = ["Nuno Campos <nuno@langchain.dev>"]
 readme = "README.md"
 packages = [{include = "langgraph_cli"}]
 
 [tool.poetry.scripts]
 langgraph = "langgraph_cli.cli:cli"
```

