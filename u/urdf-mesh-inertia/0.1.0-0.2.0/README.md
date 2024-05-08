# Comparing `tmp/urdf_mesh_inertia-0.1.0.tar.gz` & `tmp/urdf_mesh_inertia-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "urdf_mesh_inertia-0.1.0.tar", max compression
+gzip compressed data, was "urdf_mesh_inertia-0.2.0.tar", max compression
```

## Comparing `urdf_mesh_inertia-0.1.0.tar` & `urdf_mesh_inertia-0.2.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1494 2024-05-06 21:43:12.214785 urdf_mesh_inertia-0.1.0/LICENSE
--rw-r--r--   0        0        0     2452 2024-05-07 19:59:08.507764 urdf_mesh_inertia-0.1.0/README.md
--rw-r--r--   0        0        0      930 2024-05-07 19:19:01.672600 urdf_mesh_inertia-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-06 21:42:32.066702 urdf_mesh_inertia-0.1.0/src/urdf_mesh_inertia/__init__.py
--rw-r--r--   0        0        0      900 2024-05-07 19:56:54.647004 urdf_mesh_inertia-0.1.0/src/urdf_mesh_inertia/__main__.py
--rw-r--r--   0        0        0     1776 2024-05-07 19:29:26.234228 urdf_mesh_inertia-0.1.0/src/urdf_mesh_inertia/mesh.py
--rw-r--r--   0        0        0      491 2024-05-07 17:48:21.303567 urdf_mesh_inertia-0.1.0/src/urdf_mesh_inertia/xml.py
--rw-r--r--   0        0        0     3300 1970-01-01 00:00:00.000000 urdf_mesh_inertia-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1494 2024-05-06 21:43:12.214785 urdf_mesh_inertia-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2928 2024-05-08 14:46:07.763671 urdf_mesh_inertia-0.2.0/README.md
+-rw-r--r--   0        0        0      930 2024-05-08 14:47:42.836002 urdf_mesh_inertia-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-06 21:42:32.066702 urdf_mesh_inertia-0.2.0/src/urdf_mesh_inertia/__init__.py
+-rw-r--r--   0        0        0      905 2024-05-08 14:44:55.035429 urdf_mesh_inertia-0.2.0/src/urdf_mesh_inertia/__main__.py
+-rw-r--r--   0        0        0     1776 2024-05-07 19:29:26.234228 urdf_mesh_inertia-0.2.0/src/urdf_mesh_inertia/mesh.py
+-rw-r--r--   0        0        0      491 2024-05-07 17:48:21.303567 urdf_mesh_inertia-0.2.0/src/urdf_mesh_inertia/xml.py
+-rw-r--r--   0        0        0     3776 1970-01-01 00:00:00.000000 urdf_mesh_inertia-0.2.0/PKG-INFO
```

### Comparing `urdf_mesh_inertia-0.1.0/LICENSE` & `urdf_mesh_inertia-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `urdf_mesh_inertia-0.1.0/README.md` & `urdf_mesh_inertia-0.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -37,27 +37,29 @@
    ```console
    $ pipx install dist/urdf_mesh_inertia-0.1.0-py3-none-any.whl
    ```
 
 ## Usage
 
 ```console
-Usage: urdf-mesh-inertia [OPTIONS]
+ Usage: urdf-mesh-inertia [OPTIONS] MESH_PATH MASS
 
  Compute inertial parameters for a mesh.
  Calculation is made using pymeshlab and the URDF inertial tag for links is
  returned.
 
+╭─ Arguments ──────────────────────────────────────────────────────────────────╮
+│ *    mesh_path      PATH   Path of the mesh. [default: None] [required]      │
+│ *    mass           FLOAT  Mass of the mesh in kg. [default: None]           │
+│                            [required]                                        │
+╰──────────────────────────────────────────────────────────────────────────────╯
 ╭─ Options ────────────────────────────────────────────────────────────────────╮
-│ *  --mesh-path        PATH     Path of the mesh. [default: None] [required]  │
-│ *  --mass             FLOAT    Mass of the mesh in kg. [default: None]       │
-│                                [required]                                    │
-│    --precision        INTEGER  Rounding at specified decial digit.           │
-│                                [default: None]                               │
-│    --help                      Show this message and exit.                   │
+│ --precision        INTEGER  Rounding at specified decimal digit.             │
+│                             [default: None]                                  │
+│ --help                      Show this message and exit.                      │
 ╰──────────────────────────────────────────────────────────────────────────────╯
 ```
 
 For example:
 
 ```console
 $ urdf-mesh-inertia --precision 8 ~/devel/ros/darwin_description/meshes/head_coll.stl 0.158
```

### Comparing `urdf_mesh_inertia-0.1.0/pyproject.toml` & `urdf_mesh_inertia-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "urdf-mesh-inertia"
-version = "0.1.0"
+version = "0.2.0"
 description = "Compute inertial parameters for a mesh using pymeshlab and return the URDF inertial tag for links."
 authors = ["Daniele Tricoli <eriol@mornie.org>"]
 readme = "README.md"
 license = "BSD-3-Clause"
 repository = "https://github.com/eriol/urdf-mesh-inertia"
 packages = [{include = "urdf_mesh_inertia", from = "src"}]
 classifiers = [
```

### Comparing `urdf_mesh_inertia-0.1.0/src/urdf_mesh_inertia/__main__.py` & `urdf_mesh_inertia-0.2.0/src/urdf_mesh_inertia/__main__.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,18 +8,18 @@
 from rich import print
 from typing_extensions import Annotated
 
 from .mesh import compute_inertial_parameters
 
 
 def main(
-    mesh_path: Annotated[Path, typer.Option(help="Path of the mesh.")],
-    mass: Annotated[float, typer.Option(help="Mass of the mesh in kg.")],
+    mesh_path: Annotated[Path, typer.Argument(help="Path of the mesh.")],
+    mass: Annotated[float, typer.Argument(help="Mass of the mesh in kg.")],
     precision: Annotated[
-        Optional[int], typer.Option(help="Rounding at specified decial digit.")
+        Optional[int], typer.Option(help="Rounding at specified decimal digit.")
     ] = None,
 ):
     """Compute inertial parameters for a mesh.
 
     Calculation is made using pymeshlab and the URDF inertial tag for links is
     returned.
     """
```

### Comparing `urdf_mesh_inertia-0.1.0/src/urdf_mesh_inertia/mesh.py` & `urdf_mesh_inertia-0.2.0/src/urdf_mesh_inertia/mesh.py`

 * *Files identical despite different names*

### Comparing `urdf_mesh_inertia-0.1.0/PKG-INFO` & `urdf_mesh_inertia-0.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: urdf-mesh-inertia
-Version: 0.1.0
+Version: 0.2.0
 Summary: Compute inertial parameters for a mesh using pymeshlab and return the URDF inertial tag for links.
 Home-page: https://github.com/eriol/urdf-mesh-inertia
 License: BSD-3-Clause
 Author: Daniele Tricoli
 Author-email: eriol@mornie.org
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -58,27 +58,29 @@
    ```console
    $ pipx install dist/urdf_mesh_inertia-0.1.0-py3-none-any.whl
    ```
 
 ## Usage
 
 ```console
-Usage: urdf-mesh-inertia [OPTIONS]
+ Usage: urdf-mesh-inertia [OPTIONS] MESH_PATH MASS
 
  Compute inertial parameters for a mesh.
  Calculation is made using pymeshlab and the URDF inertial tag for links is
  returned.
 
+╭─ Arguments ──────────────────────────────────────────────────────────────────╮
+│ *    mesh_path      PATH   Path of the mesh. [default: None] [required]      │
+│ *    mass           FLOAT  Mass of the mesh in kg. [default: None]           │
+│                            [required]                                        │
+╰──────────────────────────────────────────────────────────────────────────────╯
 ╭─ Options ────────────────────────────────────────────────────────────────────╮
-│ *  --mesh-path        PATH     Path of the mesh. [default: None] [required]  │
-│ *  --mass             FLOAT    Mass of the mesh in kg. [default: None]       │
-│                                [required]                                    │
-│    --precision        INTEGER  Rounding at specified decial digit.           │
-│                                [default: None]                               │
-│    --help                      Show this message and exit.                   │
+│ --precision        INTEGER  Rounding at specified decimal digit.             │
+│                             [default: None]                                  │
+│ --help                      Show this message and exit.                      │
 ╰──────────────────────────────────────────────────────────────────────────────╯
 ```
 
 For example:
 
 ```console
 $ urdf-mesh-inertia --precision 8 ~/devel/ros/darwin_description/meshes/head_coll.stl 0.158
```

