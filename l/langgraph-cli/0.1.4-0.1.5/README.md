# Comparing `tmp/langgraph_cli-0.1.4.tar.gz` & `tmp/langgraph_cli-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langgraph_cli-0.1.4.tar", max compression
+gzip compressed data, was "langgraph_cli-0.1.5.tar", max compression
```

## Comparing `langgraph_cli-0.1.4.tar` & `langgraph_cli-0.1.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       12 2024-05-02 00:35:49.772511 langgraph_cli-0.1.4/README.md
--rw-r--r--   0        0        0        0 2024-05-02 00:35:49.772849 langgraph_cli-0.1.4/langgraph_cli/__init__.py
--rw-r--r--   0        0        0     6539 2024-05-07 01:05:15.454799 langgraph_cli-0.1.4/langgraph_cli/cli.py
--rw-r--r--   0        0        0     4266 2024-05-07 00:53:49.974157 langgraph_cli-0.1.4/langgraph_cli/config.py
--rw-r--r--   0        0        0     2055 2024-05-07 01:10:15.644569 langgraph_cli-0.1.4/langgraph_cli/docker.py
--rw-r--r--   0        0        0       39 2024-05-02 00:35:49.772817 langgraph_cli-0.1.4/langgraph_cli/initdb/init.sql
--rw-r--r--   0        0        0     1024 2024-05-07 01:14:42.520096 langgraph_cli-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      443 1970-01-01 00:00:00.000000 langgraph_cli-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0       12 2024-05-02 00:35:49.772511 langgraph_cli-0.1.5/README.md
+-rw-r--r--   0        0        0        0 2024-05-02 00:35:49.772849 langgraph_cli-0.1.5/langgraph_cli/__init__.py
+-rw-r--r--   0        0        0     6539 2024-05-07 01:16:04.705160 langgraph_cli-0.1.5/langgraph_cli/cli.py
+-rw-r--r--   0        0        0     4314 2024-05-07 01:15:31.675645 langgraph_cli-0.1.5/langgraph_cli/config.py
+-rw-r--r--   0        0        0     2055 2024-05-07 01:16:04.705546 langgraph_cli-0.1.5/langgraph_cli/docker.py
+-rw-r--r--   0        0        0       39 2024-05-02 00:35:49.772817 langgraph_cli-0.1.5/langgraph_cli/initdb/init.sql
+-rw-r--r--   0        0        0     1024 2024-05-07 17:41:36.869928 langgraph_cli-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      443 1970-01-01 00:00:00.000000 langgraph_cli-0.1.5/PKG-INFO
```

### Comparing `langgraph_cli-0.1.4/langgraph_cli/cli.py` & `langgraph_cli-0.1.5/langgraph_cli/cli.py`

 * *Files identical despite different names*

### Comparing `langgraph_cli-0.1.4/langgraph_cli/config.py` & `langgraph_cli-0.1.5/langgraph_cli/config.py`

 * *Files 18% similar despite different names*

```diff
@@ -79,15 +79,18 @@
             # update the config
             config["graphs"][graph_id] = f"{module_str}:{attr_str}"
 
     faux_pkgs_str = "\n\n".join(
         f"ADD {relpath} /tmp/{fullpath.name}/{fullpath.name}\n                RUN touch /tmp/{fullpath.name}/pyproject.toml"
         for fullpath, relpath in faux_pkgs.items()
     )
-    local_pkgs_str = f"ADD {' '.join(local_pkgs.values())} /tmp/" if local_pkgs else ""
+    local_pkgs_str = "\n".join(
+        f"ADD {relpath} /tmp/{fullpath.name}"
+        for fullpath, relpath in local_pkgs.items()
+    )
     env_vars_str = (
         "\n".join(f"            {k}: {v}" for k, v in config["env"].items())
         if isinstance(config["env"], dict)
         else ""
     )
     env_file_str = (
         f"env_file: {config['env']}" if isinstance(config["env"], str) else ""
```

### Comparing `langgraph_cli-0.1.4/langgraph_cli/docker.py` & `langgraph_cli-0.1.5/langgraph_cli/docker.py`

 * *Files identical despite different names*

### Comparing `langgraph_cli-0.1.4/pyproject.toml` & `langgraph_cli-0.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "langgraph-cli"
-version = "0.1.4"
+version = "0.1.5"
 description = ""
 authors = ["Nuno Campos <nuno@langchain.dev>"]
 readme = "README.md"
 packages = [{include = "langgraph_cli"}]
 
 [tool.poetry.scripts]
 langgraph = "langgraph_cli.cli:cli"
```

