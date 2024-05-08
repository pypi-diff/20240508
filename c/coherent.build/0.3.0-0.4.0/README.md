# Comparing `tmp/coherent_build-0.3.0.tar.gz` & `tmp/coherent_build-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coherent_build-0.3.0.tar", last modified: Sun May  5 15:35:47 2024, max compression
+gzip compressed data, was "coherent_build-0.4.0.tar", last modified: Tue May  7 20:56:49 2024, max compression
```

## Comparing `coherent_build-0.3.0.tar` & `coherent_build-0.4.0.tar`

### file list

```diff
@@ -1,6 +1,8 @@
-drwxr-xr-x   0 jaraco     (501) staff       (20)        0 2024-05-05 15:22:36.523763 coherent_build-0.3.0/
--rw-r--r--   0 jaraco     (501) staff       (20)       84 2024-05-05 14:27:21.911766 coherent_build-0.3.0/README.md
--rw-r--r--   0 jaraco     (501) staff       (20)     8061 2024-05-05 15:32:14.403169 coherent_build-0.3.0/__init__.py
--rw-r--r--   0 jaraco     (501) staff       (20)      495 2024-05-02 02:13:39.559121 coherent_build-0.3.0/__main__.py
--rw-r--r--   0 jaraco     (501) staff       (20)       78 2024-05-02 15:12:07.306572 coherent_build-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      484 2024-05-05 15:35:47.105496 coherent_build-0.3.0/PKG-INFO
+drwxr-xr-x   0 jaraco     (501) staff       (20)        0 2024-05-07 20:48:20.139500 coherent_build-0.4.0/
+-rw-r--r--   0 jaraco     (501) staff       (20)       84 2024-05-05 14:27:21.911766 coherent_build-0.4.0/README.md
+-rw-r--r--   0 jaraco     (501) staff       (20)     5556 2024-05-07 20:53:13.349675 coherent_build-0.4.0/__init__.py
+-rw-r--r--   0 jaraco     (501) staff       (20)     8550 2024-05-07 20:37:24.092828 coherent_build-0.4.0/__init__.py.orig
+-rw-r--r--   0 jaraco     (501) staff       (20)      495 2024-05-02 02:13:39.559121 coherent_build-0.4.0/__main__.py
+-rw-r--r--   0 jaraco     (501) staff       (20)     3035 2024-05-07 20:55:49.864191 coherent_build-0.4.0/discovery.py
+-rw-r--r--   0 jaraco     (501) staff       (20)       78 2024-05-02 15:12:07.306572 coherent_build-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      509 2024-05-07 20:56:49.143335 coherent_build-0.4.0/PKG-INFO
```

### Comparing `coherent_build-0.3.0/__init__.py` & `coherent_build-0.4.0/__init__.py.orig`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 __requires__ = [
-    "wheel",
-    "pip-run",
-    "setuptools_scm",
-    "build",
-    "git-fame",
-    "jaraco.context",
-    "requests",
+    'wheel',
+    'pip-run',
+    'setuptools_scm',
+    'build',
+    'git-fame',
+    'jaraco.context',
+    'requests',
+    'packaging',
 ]
 
 import functools
 import importlib.metadata
 import io
 import json
 import mimetypes
@@ -22,69 +23,80 @@
 import time
 import types
 
 from collections.abc import Mapping
 from email.message import Message
 from typing import Iterable
 
+import packaging
 import requests
 import setuptools_scm
 from wheel.wheelfile import WheelFile
 from pip_run import scripts
 from jaraco.context import suppress
 
 
-mimetypes.add_type("text/plain", "", strict=True)
-mimetypes.add_type("text/markdown", ".md", strict=True)
-mimetypes.add_type("text/x-rst", ".rst", strict=True)
+mimetypes.add_type('text/plain', '', strict=True)
+mimetypes.add_type('text/markdown', '.md', strict=True)
+mimetypes.add_type('text/x-rst', '.rst', strict=True)
 
 
 def name_from_path():
-    return pathlib.Path(".").absolute().name
+    return pathlib.Path('.').absolute().name
 
 
 def version_from_vcs():
     return setuptools_scm.get_version()
 
 
-@suppress(Exception)
+@suppress(subprocess.CalledProcessError)
 def summary_from_github():
+    """
+    Load the summary from GitHub.
+
+    >>> summary_from_github()
+    'A zero-config Python project build backend'
+    """
     return (
         json.loads(
             subprocess.check_output(
-                ["gh", "repo", "view", "--json", "description"],
+                ['gh', 'repo', 'view', '--json', 'description'],
                 text=True,
-                encoding="utf-8",
+                encoding='utf-8',
             )
-        )["description"]
+        )['description']
         or None
     )
 
 
 def python_requires_supported():
-    owner = "python"
-    repo = "cpython"
-    url = f"https://api.github.com/repos/{owner}/{repo}/branches"
+    """
+    >>> python_requires_supported()
+    '>= 3...'
+    """
+    owner = 'python'
+    repo = 'cpython'
+    url = f'https://api.github.com/repos/{owner}/{repo}/branches'
     branches = requests.get(url).json()
     # cheat and grab the first branch, which is the oldest supported Python version
     return f'>= {branches[0]["name"]}'
 
 
 class Filter:
     def __init__(self, name: str):
         self.name = name
 
     def __call__(self, info):
-        if info.name == ".":
+        if info.name == '.':
             info.name = self.name
             return info
-        ignore_pattern = "|".join(self.ignored)
-        if re.match(ignore_pattern, info.name.removeprefix("./")):
+        ignore_pattern = '|'.join(self.ignored)
+        if re.match(ignore_pattern, info.name.removeprefix('./')):
             return
-        info.name = self.name + "/" + info.name.removeprefix("./")
+        info.name = self.name + '/' + info.name.removeprefix('./')
         return info
 
 
 class SDist(Filter):
     """
     >>> sf = SDist(name="foo")
 
@@ -98,100 +110,98 @@
     >>> sf(types.SimpleNamespace(name='./bar/.DS_Store'))
 
     Should not ignore nested dist dirs
     >>> sf(types.SimpleNamespace(name='./bar/dist'))
     namespace(name='foo/bar/dist')
     """
 
-    ignored = ["dist", r"(.*[/])?__pycache__$", r"(.*[/])?[.]"]
+    ignored = ['dist', r'(.*[/])?__pycache__$', r'(.*[/])?[.]']
 
 
 class Wheel(Filter):
-    ignored = ["docs", "tests", "README.*", "PKG-INFO", "(meta)"]
+    ignored = ['docs', 'tests', 'README.*', 'PKG-INFO', '(meta)']
 
 
 class ZipInfo(types.SimpleNamespace):
     def __init__(self, path):
         zip_name = path.replace(os.pathsep, posixpath.sep)
         super().__init__(path=path, name=zip_name)
 
 
-def normalize(name):
-    # todo: do proper normalization
-    return name.replace(".", "_")
+_normalize = functools.partial(
+    packaging.utils.canonicalize_version, strip_trailing_zero=False
+)
 
 
 def build_wheel(wheel_directory, config_settings=None, metadata_directory=None):
     metadata = Metadata.from_sdist() or Metadata.discover()
-    root = metadata["Name"].replace(".", "/")
-    filename = pathlib.Path(wheel_directory) / f"{metadata.id}-py3-none-any.whl"
-    with WheelFile(filename, "w") as zf:
+    root = metadata['Name'].replace('.', '/')
+    filename = pathlib.Path(wheel_directory) / f'{metadata.id}-py3-none-any.whl'
+    with WheelFile(filename, 'w') as zf:
         for info in wheel_walk(Wheel(root)):
             zf.write(info.path, arcname=info.name)
         for md_name, contents in make_wheel_metadata(metadata):
             zf.writestr(md_name, contents)
     return str(filename)
 
 
 def read_deps():
     """
     Read deps from ``__init__.py``.
     """
-    return scripts.DepsReader.search(["__init__.py"])
+    return scripts.DepsReader.search(['__init__.py'])
 
 
 def make_wheel_metadata(metadata):
-    dist_info = f"{metadata.id}.dist-info"
-    yield f"{dist_info}/METADATA", metadata.render()
-    wheel_md = Metadata(
-        {
-            "Wheel-Version": "1.0",
-            "Generator": "coherent.build",
-            "Root-Is-Purelib": "true",
-            "Tag": "py3-none-any",
-        }
-    )
-    yield f"{dist_info}/WHEEL", wheel_md.render()
+    dist_info = f'{metadata.id}.dist-info'
+    yield f'{dist_info}/METADATA', metadata.render()
+    wheel_md = Metadata({
+        'Wheel-Version': '1.0',
+        'Generator': 'coherent.build',
+        'Root-Is-Purelib': 'true',
+        'Tag': 'py3-none-any',
+    })
+    yield f'{dist_info}/WHEEL', wheel_md.render()
 
 
 def wheel_walk(filter_: Wheel):
-    for root, dirs, files in os.walk("."):
+    for root, dirs, files in os.walk('.'):
         zi = ZipInfo(path=root)
         if not filter_(zi):
             dirs[:] = []
             continue
 
         children = (ZipInfo(path=os.path.join(root, file)) for file in files)
         yield from filter(None, map(filter_, children))
 
 
 def _to_mapping(fame):
-    return (dict(zip(fame["columns"], row)) for row in fame["data"])
+    return (dict(zip(fame['columns'], row)) for row in fame['data'])
 
 
 class Contributor(types.SimpleNamespace):
     @property
     def combined_detail(self):
         return f'"{self.name}" <{self.email}>'
 
 
 @suppress(Exception)
 def author_from_vcs():
     # run git-fame twice to get both name and email
-    cmd = ["git-fame", "--format", "json"]
-    names_data = json.loads(subprocess.check_output(cmd, text=True, encoding="utf-8"))
+    cmd = ['git-fame', '--format', 'json']
+    names_data = json.loads(subprocess.check_output(cmd, text=True, encoding='utf-8'))
     emails_data = json.loads(
         subprocess.check_output(
-            cmd + ["--show-email"],
+            cmd + ['--show-email'],
             text=True,
-            encoding="utf-8",
+            encoding='utf-8',
         )
     )
-    names_data["columns"][0] = "name"
-    emails_data["columns"][0] = "email"
+    names_data['columns'][0] = 'name'
+    emails_data['columns'][0] = 'email'
     emails_contribs = _to_mapping(emails_data)
     names_contribs = _to_mapping(names_data)
 
     contribs = (
         Contributor(**val)
         for val in (
             {**name_contrib, **email_contrib}
@@ -227,36 +237,45 @@
 
     def __init__(self, values):
         super().__init__()
         for item in always_items(values):
             self.add_header(*item)
 
     def _description_in_payload(self):
-        if "Description" in self:
-            self.set_payload(self["Description"])
-            del self["Description"]
+        if 'Description' in self:
+            self.set_payload(self['Description'])
+            del self['Description']
 
     @property
     def id(self):
-        return f"{normalize(self['Name'])}-{self['Version']}"
+        """
+<<<<<<< Updated upstream
+        >>> Metadata(dict(Name='foo.bar', Version='1.0.0')).id
+        'foo_bar-1.0.0'
+=======
+        >>> Metadata(dict(Name='foo.bar', Version='1.0.dev3')).id
+        'foo.bar-1.0.dev3'
+>>>>>>> Stashed changes
+        """
+        return f"{_normalize(self['Name'])}-{self['Version']}"
 
     @classmethod
     def discover(cls):
         return cls(cls._discover_fields())
 
     @staticmethod
     def _discover_fields():
-        yield "Metadata-Version", "2.3"
-        yield "Name", name_from_path()
-        yield "Version", version_from_vcs()
-        yield "Author-Email", author_from_vcs()
-        yield "Summary", summary_from_github()
-        yield "Requires-Python", python_requires_supported()
+        yield 'Metadata-Version', '2.3'
+        yield 'Name', name_from_path()
+        yield 'Version', version_from_vcs()
+        yield 'Author-Email', author_from_vcs()
+        yield 'Summary', summary_from_github()
+        yield 'Requires-Python', python_requires_supported()
         for dep in read_deps():
-            yield "Requires-Dist", dep
+            yield 'Requires-Dist', dep
         yield from description_from_readme()
 
     @classmethod
     def from_sdist(cls):
         sdist_metadata = importlib.metadata.PathDistribution(pathlib.Path()).metadata
         return (sdist_metadata or None) and cls(sdist_metadata)
 
@@ -276,29 +295,29 @@
     """
     type, _ = mimetypes.guess_type(str(path))
     return type
 
 
 @suppress(Exception)
 def description_from_readme():
-    (readme,) = pathlib.Path().glob("README*")
+    (readme,) = pathlib.Path().glob('README*')
     ct = guess_content_type(readme)
     assert ct
-    yield "Description-Content-Type", ct
-    yield "Description", readme.read_text(encoding="utf-8")
+    yield 'Description-Content-Type', ct
+    yield 'Description', readme.read_text(encoding='utf-8')
 
 
 def make_sdist_metadata(metadata) -> tarfile.TarInfo:
-    info = tarfile.TarInfo(f"{metadata.id}/PKG-INFO")
-    file = io.BytesIO(metadata.render().encode("utf-8"))
+    info = tarfile.TarInfo(f'{metadata.id}/PKG-INFO')
+    file = io.BytesIO(metadata.render().encode('utf-8'))
     info.size = len(file.getbuffer())
     info.mtime = time.time()
     return info, file
 
 
 def build_sdist(sdist_directory, config_settings=None):
     metadata = Metadata.discover()
-    filename = pathlib.Path(sdist_directory) / f"{metadata.id}.tar.gz"
-    with tarfile.open(filename, "w:gz") as tf:
+    filename = pathlib.Path(sdist_directory) / f'{metadata.id}.tar.gz'
+    with tarfile.open(filename, 'w:gz') as tf:
         tf.add(pathlib.Path(), filter=SDist(metadata.id))
         tf.addfile(*make_sdist_metadata(metadata))
     return str(filename)
```

