# Comparing `tmp/poetry_plugin_lambda_build-0.4.1.tar.gz` & `tmp/poetry_plugin_lambda_build-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry_plugin_lambda_build-0.4.1.tar", max compression
+gzip compressed data, was "poetry_plugin_lambda_build-0.5.0.tar", max compression
```

## Comparing `poetry_plugin_lambda_build-0.4.1.tar` & `poetry_plugin_lambda_build-0.5.0.tar`

### file list

```diff
@@ -1,10 +1,14 @@
--rw-r--r--   0        0        0     1073 2024-04-25 09:58:26.300745 poetry_plugin_lambda_build-0.4.1/LICENSE
--rw-r--r--   0        0        0     5598 2024-04-25 09:58:26.300745 poetry_plugin_lambda_build-0.4.1/README.md
--rw-r--r--   0        0        0        0 2024-04-25 09:58:26.300745 poetry_plugin_lambda_build-0.4.1/poetry_plugin_lambda_build/__init__.py
--rw-r--r--   0        0        0     2134 2024-04-25 09:58:26.300745 poetry_plugin_lambda_build-0.4.1/poetry_plugin_lambda_build/docker.py
--rw-r--r--   0        0        0     6613 2024-04-25 09:58:26.300745 poetry_plugin_lambda_build-0.4.1/poetry_plugin_lambda_build/plugin.py
--rw-r--r--   0        0        0     7660 2024-04-25 09:58:26.300745 poetry_plugin_lambda_build-0.4.1/poetry_plugin_lambda_build/recipes.py
--rw-r--r--   0        0        0      257 2024-04-25 09:58:26.300745 poetry_plugin_lambda_build-0.4.1/poetry_plugin_lambda_build/utils.py
--rw-r--r--   0        0        0      652 2024-04-25 09:58:26.300745 poetry_plugin_lambda_build-0.4.1/poetry_plugin_lambda_build/zip.py
--rw-r--r--   0        0        0      707 2024-04-25 09:58:26.300745 poetry_plugin_lambda_build-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     6309 1970-01-01 00:00:00.000000 poetry_plugin_lambda_build-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-05-08 13:30:39.097909 poetry_plugin_lambda_build-0.5.0/LICENSE
+-rw-r--r--   0        0        0     5519 2024-05-08 13:30:39.097909 poetry_plugin_lambda_build-0.5.0/README.md
+-rw-r--r--   0        0        0        0 2024-05-08 13:30:39.097909 poetry_plugin_lambda_build-0.5.0/poetry_plugin_lambda_build/__init__.py
+-rw-r--r--   0        0        0      891 2024-05-08 13:30:39.097909 poetry_plugin_lambda_build-0.5.0/poetry_plugin_lambda_build/commands.py
+-rw-r--r--   0        0        0     2862 2024-05-08 13:30:39.097909 poetry_plugin_lambda_build-0.5.0/poetry_plugin_lambda_build/docker.py
+-rw-r--r--   0        0        0     3877 2024-05-08 13:30:39.097909 poetry_plugin_lambda_build-0.5.0/poetry_plugin_lambda_build/parameters.py
+-rw-r--r--   0        0        0     2041 2024-05-08 13:30:39.097909 poetry_plugin_lambda_build-0.5.0/poetry_plugin_lambda_build/plugin.py
+-rw-r--r--   0        0        0    11409 2024-05-08 13:30:39.097909 poetry_plugin_lambda_build-0.5.0/poetry_plugin_lambda_build/recipes.py
+-rw-r--r--   0        0        0     6752 2024-05-08 13:30:39.097909 poetry_plugin_lambda_build-0.5.0/poetry_plugin_lambda_build/requirements.py
+-rw-r--r--   0        0        0     2120 2024-05-08 13:30:39.097909 poetry_plugin_lambda_build-0.5.0/poetry_plugin_lambda_build/utils.py
+-rw-r--r--   0        0        0     9831 2024-05-08 13:30:39.097909 poetry_plugin_lambda_build-0.5.0/poetry_plugin_lambda_build/walker.py
+-rw-r--r--   0        0        0      767 2024-05-08 13:30:39.097909 poetry_plugin_lambda_build-0.5.0/poetry_plugin_lambda_build/zip.py
+-rw-r--r--   0        0        0     1042 2024-05-08 13:30:39.097909 poetry_plugin_lambda_build-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     6229 1970-01-01 00:00:00.000000 poetry_plugin_lambda_build-0.5.0/PKG-INFO
```

### Comparing `poetry_plugin_lambda_build-0.4.1/LICENSE` & `poetry_plugin_lambda_build-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `poetry_plugin_lambda_build-0.4.1/README.md` & `poetry_plugin_lambda_build-0.5.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 
 [![Test](https://github.com/micmurawski/poetry-plugin-lambda-build/actions/workflows/test.yml/badge.svg)](https://github.com/micmurawski/poetry-plugin-lambda-build/actions/workflows/test.yml)
 
 ## Installation
 
 ```bash
 poetry self add poetry-plugin-lambda-build
-poetry self add poetry-plugin-export
 ```
 
 ## Execution
 
 Configure `pyproject.toml` with the following configuration. This is example for [AWS Lambda configuration](#aws)
 
 ```.toml
@@ -79,15 +78,15 @@
 ```
 
 ```
 Description:
   Execute to build lambda lambda artifacts
 
 Usage:
-  build-lambda [options] [--] [<docker_image> [<docker_entrypoint> [<docker_environment> [<docker_dns> [<docker_network> [<docker_network_disabled> [<docker_network_mode> [<docker_platform> [<package_install_dir> [<layer_install_dir> [<function_install_dir> [<install_dir> [<package_artifact_path> [<layer_artifact_path> [<function_artifact_path> [<only> [<without> [<with> [<install_deps_cmd> [<install_no_deps_cmd>]]]]]]]]]]]]]]]]]]]]
+  build-lambda [options] [--] [<docker_image> [<docker_entrypoint> [<docker_environment> [<docker_dns> [<docker_network> [<docker_network_disabled> [<docker_network_mode> [<docker_platform> [<package_install_dir> [<layer_install_dir> [<function_install_dir> [<install_dir> [<package_artifact_path> [<layer_artifact_path> [<function_artifact_path> [<only> [<without> [<with> [<zip_compresslevel> [<zip_compression>]]]]]]]]]]]]]]]]]]]]
 
 Arguments:
   docker_image               The image to run
   docker_entrypoint          The entrypoint for the container (comma separated string)
   docker_environment         Environment variables to set inside the container (comma separated string) ex. VAR_1=VALUE_1,VAR_2=VALUE_2
   docker_dns                 Set custom DNS servers (comma separated string)
   docker_network             The name of the network this container will be connected to at creation time
@@ -100,16 +99,16 @@
   install_dir                Installation directory inside zip artifact for zip package (not function layer separation)
   package_artifact_path      Output package path
   layer_artifact_path        Output layer package path
   function_artifact_path     Output function package path
   only                       The only dependency groups to include
   without                    The dependency groups to ignore
   with                       The optional dependency groups to include
-  install_deps_cmd           Install dependencies command. Executed during installation of dependencies layer, by default: mkdir -p {container_cache_dir} && pip install -q --upgrade pip && pip install -q -t {container_cache_dir} --no-cache-dir -r {requirements}
-  install_no_deps_cmd        Install without dependencies command. Executed during installation of function, by default: mkdir -p {package_dir} && poetry run pip install --quiet -t {package_dir} --no-cache-dir --no-deps . --upgrade
+  zip_compresslevel          None (default for the given compression type) or an integer specifying the level to pass to the compressor. When using ZIP_STORED or ZIP_LZMA this keyword has no effect. When using ZIP_DEFLATED integers 0 through 9 are accepted. When using ZIP_BZIP2 integers 1 through 9 are accepted.
+  zip_compression            ZIP_STORED (no compression), ZIP_DEFLATED (requires zlib), ZIP_BZIP2 (requires bz2) or ZIP_LZMA (requires lzma)
 
 Options:
   -h, --help                 Display help for the given command. When no command is given display help for the list command.
   -q, --quiet                Do not output any message.
   -V, --version              Display this application version.
       --ansi                 Force ANSI output.
       --no-ansi              Disable ANSI output.
```

### Comparing `poetry_plugin_lambda_build-0.4.1/poetry_plugin_lambda_build/docker.py` & `poetry_plugin_lambda_build-0.5.0/poetry_plugin_lambda_build/docker.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,83 +1,103 @@
+from __future__ import annotations
+
 import os
 import tarfile
 from contextlib import contextmanager
+from tempfile import TemporaryDirectory
+from typing import Generator
 
 import docker
-from poetry.console.commands.env_command import EnvCommand
-
-LIST_ARGS = (
-    "environment",
-    "dns",
-    "entrypoint"
-)
+from docker.models.containers import Container
 
-BOOLEAN_ARGS = (
-    "docker_network_disabled"
-)
+from poetry_plugin_lambda_build.utils import cd
 
 
-def _parse_string_to_boolean(value: str):
+def _parse_str_to_bool(value: str) -> bool:
     if value.lower() in ("0", "false"):
         return False
     return True
 
 
+def _parse_str_to_list(value: str) -> list[str]:
+    return value.split(",")
+
+
+ARGS_PARSERS = {
+    "environment": _parse_str_to_list,
+    "dns": _parse_str_to_list,
+    "entrypoint": _parse_str_to_list,
+    "docker_network_disabled": _parse_str_to_bool
+}
+
+
 def get_docker_client() -> docker.DockerClient:
     return docker.from_env()
 
 
 def copy_to(src: str, dst: str):
     name, dst = dst.split(":")
     container = get_docker_client().containers.get(name)
 
-    os.chdir(os.path.dirname(src))
-    src_name = os.path.basename(src)
-    tar = tarfile.open(src + ".tar", mode="w")
-    try:
-        tar.add(src_name)
-    finally:
-        tar.close()
+    with TemporaryDirectory() as tmp_dir:
+        src_name = os.path.basename(src)
+        tar_filename = src_name + "_archive.tar"
+        tar_path = os.path.join(tmp_dir, tar_filename)
+        tar = tarfile.open(tar_path, mode="w")
+        with cd(os.path.dirname(src)):
+            try:
+                tar.add(src_name)
+            finally:
+                tar.close()
 
-    data = open(src + ".tar", "rb").read()
-    container.put_archive(os.path.dirname(dst), data)
+            data = open(tar_path, "rb").read()
+            container.put_archive(os.path.dirname(dst), data)
 
 
 def copy_from(src: str, dst: str):
     name, src = src.split(":")
     container = get_docker_client().containers.get(name)
-    tar_path = dst + ".tar"
+    tar_path = dst + "_archive.tar"
     f = open(tar_path, "wb")
     bits, _ = container.get_archive(src)
     for chunk in bits:
         f.write(chunk)
     f.close()
     tar = tarfile.open(tar_path)
     tar.extractall(dst)
+    tar.close()
     os.remove(tar_path)
 
 
 @contextmanager
-def run_container(env_cmd: EnvCommand, **kwargs):
+def run_container(logger, **kwargs) -> Generator[Container, None, None]:
     image: str = kwargs.pop("image")
     options: dict = {k: True for k in kwargs.pop("options", [])}
     kwargs: dict = {k: v for k, v in kwargs.items() if v}
 
-    for arg in LIST_ARGS:
-        if arg in kwargs:
-            kwargs[arg] = kwargs[arg].split(",")
-
-    for arg in BOOLEAN_ARGS:
+    for arg in ARGS_PARSERS:
         if arg in kwargs:
-            kwargs[arg] = _parse_string_to_boolean(kwargs[arg])
+            parser = ARGS_PARSERS[arg]
+            kwargs[arg] = parser(kwargs[arg])
 
-    docker_container = get_docker_client().containers.run(
+    docker_container: Container = get_docker_client().containers.run(
         image, **kwargs, **options, tty=True, detach=True
     )
-    env_cmd.line(f"Running docker container image: {image}", style="debug")
+    logger.debug(f"Running docker container image: {image}")
     try:
         yield docker_container
     finally:
-        env_cmd.line("Killing docker container...", style="debug")
+        logger.debug("Killing docker container...")
         docker_container.kill()
-        env_cmd.line("Removing docker container...", style="debug")
+        logger.debug("Removing docker container...")
         docker_container.remove(v=True)
+
+
+def exec_run_container(logger, container: Container, entrypoint: str, container_cmd: str):
+    _, stream = container.exec_run(
+        f'{entrypoint} -c "{container_cmd}"',
+        stdout=True,
+        stderr=True,
+        stream=True
+    )
+    for line in stream:
+        logger.info(line.strip().decode())
```

### Comparing `poetry_plugin_lambda_build-0.4.1/poetry_plugin_lambda_build/zip.py` & `poetry_plugin_lambda_build-0.5.0/poetry_plugin_lambda_build/zip.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,24 @@
+from __future__ import annotations
+
 import os
 from fnmatch import fnmatch
 from functools import reduce
 from operator import or_
 from zipfile import ZipFile
 
 
-def create_zip_package(dir, output, exclude=None):
+def create_zip_package(dir, output, exclude=None, **kwargs):
     if exclude is None:
         exclude = ["*.pyc", "*__pycache__/*"]
-    with ZipFile(output, "w") as zip_file:
+    with ZipFile(output, "w", **kwargs) as zip_file:
         for i in os.walk(dir):
             base_path, _, files = i
             for file in files:
                 file_path = os.path.join(base_path, file)
+
                 if not reduce(
-                    or_, [fnmatch(file_path, pattern) for pattern in exclude]
+                    or_, [fnmatch(file_path, pattern)
+                          for pattern in exclude], False
                 ):
-                    zip_file.write(file_path, arcname=file_path.replace(dir, ""))
+                    zip_file.write(
+                        file_path, arcname=file_path.replace(dir, ""))
```

### Comparing `poetry_plugin_lambda_build-0.4.1/pyproject.toml` & `poetry_plugin_lambda_build-0.5.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,39 @@
 [tool.poetry]
 name = "poetry-plugin-lambda-build"
-version = "0.4.1"
+version = "0.5.0"
 description = "The plugin for poetry that allows you to build zip packages suited for serverless deployment like AWS Lambda, Google App Engine, Azure App Service, and more..."
-authors = ["Michał Murawski <mmurawski777@gmail.com>"]
+authors = ["Michal Murawski <mmurawski777@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 docker = "^7.0.0"
 
 [tool.poetry.group.test.dependencies]
 pytest = "^8.0.1"
 poetry = "^1.7.1"
+pytest-cov = "^5.0.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.plugins."poetry.application.plugin"]
 build-lambda = "poetry_plugin_lambda_build.plugin:LambdaPlugin"
 
 [tool.pytest.ini_options]
 testpaths = ["tests"]
+addopts = [
+    "--cov=poetry_plugin_lambda_build",
+    "--cov-report=term-missing",
+    "--cov-report=html",
+]
+
+[tool.coverage.run]
+source = ["poetry_plugin_lambda_build"]
+command_line = "-m pytest"
+
+[tool.coverage.report]
+include = ["poetry_plugin_lambda_build/*.py"]
+omit = ["*__init__.py"]
+show_missing = true
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `poetry_plugin_lambda_build-0.4.1/PKG-INFO` & `poetry_plugin_lambda_build-0.5.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: poetry-plugin-lambda-build
-Version: 0.4.1
+Version: 0.5.0
 Summary: The plugin for poetry that allows you to build zip packages suited for serverless deployment like AWS Lambda, Google App Engine, Azure App Service, and more...
-Author: Michał Murawski
+Author: Michal Murawski
 Author-email: mmurawski777@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -22,15 +22,14 @@
 
 [![Test](https://github.com/micmurawski/poetry-plugin-lambda-build/actions/workflows/test.yml/badge.svg)](https://github.com/micmurawski/poetry-plugin-lambda-build/actions/workflows/test.yml)
 
 ## Installation
 
 ```bash
 poetry self add poetry-plugin-lambda-build
-poetry self add poetry-plugin-export
 ```
 
 ## Execution
 
 Configure `pyproject.toml` with the following configuration. This is example for [AWS Lambda configuration](#aws)
 
 ```.toml
@@ -95,15 +94,15 @@
 ```
 
 ```
 Description:
   Execute to build lambda lambda artifacts
 
 Usage:
-  build-lambda [options] [--] [<docker_image> [<docker_entrypoint> [<docker_environment> [<docker_dns> [<docker_network> [<docker_network_disabled> [<docker_network_mode> [<docker_platform> [<package_install_dir> [<layer_install_dir> [<function_install_dir> [<install_dir> [<package_artifact_path> [<layer_artifact_path> [<function_artifact_path> [<only> [<without> [<with> [<install_deps_cmd> [<install_no_deps_cmd>]]]]]]]]]]]]]]]]]]]]
+  build-lambda [options] [--] [<docker_image> [<docker_entrypoint> [<docker_environment> [<docker_dns> [<docker_network> [<docker_network_disabled> [<docker_network_mode> [<docker_platform> [<package_install_dir> [<layer_install_dir> [<function_install_dir> [<install_dir> [<package_artifact_path> [<layer_artifact_path> [<function_artifact_path> [<only> [<without> [<with> [<zip_compresslevel> [<zip_compression>]]]]]]]]]]]]]]]]]]]]
 
 Arguments:
   docker_image               The image to run
   docker_entrypoint          The entrypoint for the container (comma separated string)
   docker_environment         Environment variables to set inside the container (comma separated string) ex. VAR_1=VALUE_1,VAR_2=VALUE_2
   docker_dns                 Set custom DNS servers (comma separated string)
   docker_network             The name of the network this container will be connected to at creation time
@@ -116,16 +115,16 @@
   install_dir                Installation directory inside zip artifact for zip package (not function layer separation)
   package_artifact_path      Output package path
   layer_artifact_path        Output layer package path
   function_artifact_path     Output function package path
   only                       The only dependency groups to include
   without                    The dependency groups to ignore
   with                       The optional dependency groups to include
-  install_deps_cmd           Install dependencies command. Executed during installation of dependencies layer, by default: mkdir -p {container_cache_dir} && pip install -q --upgrade pip && pip install -q -t {container_cache_dir} --no-cache-dir -r {requirements}
-  install_no_deps_cmd        Install without dependencies command. Executed during installation of function, by default: mkdir -p {package_dir} && poetry run pip install --quiet -t {package_dir} --no-cache-dir --no-deps . --upgrade
+  zip_compresslevel          None (default for the given compression type) or an integer specifying the level to pass to the compressor. When using ZIP_STORED or ZIP_LZMA this keyword has no effect. When using ZIP_DEFLATED integers 0 through 9 are accepted. When using ZIP_BZIP2 integers 1 through 9 are accepted.
+  zip_compression            ZIP_STORED (no compression), ZIP_DEFLATED (requires zlib), ZIP_BZIP2 (requires bz2) or ZIP_LZMA (requires lzma)
 
 Options:
   -h, --help                 Display help for the given command. When no command is given display help for the list command.
   -q, --quiet                Do not output any message.
   -V, --version              Display this application version.
       --ansi                 Force ANSI output.
       --no-ansi              Disable ANSI output.
```

