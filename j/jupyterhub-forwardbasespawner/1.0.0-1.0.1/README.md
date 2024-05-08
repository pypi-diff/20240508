# Comparing `tmp/jupyterhub_forwardbasespawner-1.0.0.tar.gz` & `tmp/jupyterhub_forwardbasespawner-1.0.1.tar.gz`

## Comparing `jupyterhub_forwardbasespawner-1.0.0.tar` & `jupyterhub_forwardbasespawner-1.0.1.tar`

### file list

```diff
@@ -1,27 +1,28 @@
--rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 jupyterhub_forwardbasespawner-1.0.0/.gitlab-ci.yml
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 jupyterhub_forwardbasespawner-1.0.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 jupyterhub_forwardbasespawner-1.0.0/.readthedocs.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyterhub_forwardbasespawner-1.0.0/CHANGELOG.md
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 jupyterhub_forwardbasespawner-1.0.0/release_notes.md
--rw-r--r--   0        0        0   120884 2020-02-02 00:00:00.000000 jupyterhub_forwardbasespawner-1.0.0/docs/Doxyfile
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 jupyterhub_forwardbasespawner-1.0.0/docs/Makefile
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 jupyterhub_forwardbasespawner-1.0.0/docs/apiendpoints.md
--rw-r--r--   0        0        0     3350 2020-02-02 00:00:00.000000 jupyterhub_forwardbasespawner-1.0.0/docs/conf.py
--rw-r--r--   0        0        0     2391 2020-02-02 00:00:00.000000 jupyterhub_forwardbasespawner-1.0.0/docs/index.md
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 jupyterhub_forwardbasespawner-1.0.0/docs/make.bat
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 jupyterhub_forwardbasespawner-1.0.0/docs/requirements.txt
--rw-r--r--   0        0        0    17701 2020-02-02 00:00:00.000000 jupyterhub_forwardbasespawner-1.0.0/docs/_static/rest-api.yml
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 jupyterhub_forwardbasespawner-1.0.0/docs/spawners/forwardbasespawner.md
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 jupyterhub_forwardbasespawner-1.0.0/forwardbasespawner/__init__.py
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 jupyterhub_forwardbasespawner-1.0.0/forwardbasespawner/_version.py
--rw-r--r--   0        0        0     5806 2020-02-02 00:00:00.000000 jupyterhub_forwardbasespawner-1.0.0/forwardbasespawner/api_events.py
--rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 jupyterhub_forwardbasespawner-1.0.0/forwardbasespawner/api_list_servers.py
--rw-r--r--   0        0        0     3741 2020-02-02 00:00:00.000000 jupyterhub_forwardbasespawner-1.0.0/forwardbasespawner/api_setup_tunnel.py
--rw-r--r--   0        0        0     1900 2020-02-02 00:00:00.000000 jupyterhub_forwardbasespawner-1.0.0/forwardbasespawner/api_sshnode_restarted.py
--rw-r--r--   0        0        0    64084 2020-02-02 00:00:00.000000 jupyterhub_forwardbasespawner-1.0.0/forwardbasespawner/forward.py
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 jupyterhub_forwardbasespawner-1.0.0/forwardbasespawner/utils.py
--rw-r--r--   0        0        0     2591 2020-02-02 00:00:00.000000 jupyterhub_forwardbasespawner-1.0.0/.gitignore
--rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 jupyterhub_forwardbasespawner-1.0.0/LICENSE
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 jupyterhub_forwardbasespawner-1.0.0/README.md
--rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 jupyterhub_forwardbasespawner-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     2274 2020-02-02 00:00:00.000000 jupyterhub_forwardbasespawner-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1844 2020-02-02 00:00:00.000000 jupyterhub_forwardbasespawner-1.0.1/.gitlab-ci.yml
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 jupyterhub_forwardbasespawner-1.0.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 jupyterhub_forwardbasespawner-1.0.1/.readthedocs.yaml
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 jupyterhub_forwardbasespawner-1.0.1/CHANGELOG.md
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 jupyterhub_forwardbasespawner-1.0.1/release_notes.md
+-rw-r--r--   0        0        0   120884 2020-02-02 00:00:00.000000 jupyterhub_forwardbasespawner-1.0.1/docs/Doxyfile
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 jupyterhub_forwardbasespawner-1.0.1/docs/Makefile
+-rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 jupyterhub_forwardbasespawner-1.0.1/docs/apiendpoints.md
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 jupyterhub_forwardbasespawner-1.0.1/docs/changelog.md
+-rw-r--r--   0        0        0     3350 2020-02-02 00:00:00.000000 jupyterhub_forwardbasespawner-1.0.1/docs/conf.py
+-rw-r--r--   0        0        0     2479 2020-02-02 00:00:00.000000 jupyterhub_forwardbasespawner-1.0.1/docs/index.md
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 jupyterhub_forwardbasespawner-1.0.1/docs/make.bat
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 jupyterhub_forwardbasespawner-1.0.1/docs/requirements.txt
+-rw-r--r--   0        0        0    17685 2020-02-02 00:00:00.000000 jupyterhub_forwardbasespawner-1.0.1/docs/_static/rest-api.yml
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 jupyterhub_forwardbasespawner-1.0.1/docs/spawners/forwardbasespawner.md
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 jupyterhub_forwardbasespawner-1.0.1/forwardbasespawner/__init__.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 jupyterhub_forwardbasespawner-1.0.1/forwardbasespawner/_version.py
+-rw-r--r--   0        0        0     5806 2020-02-02 00:00:00.000000 jupyterhub_forwardbasespawner-1.0.1/forwardbasespawner/api_events.py
+-rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 jupyterhub_forwardbasespawner-1.0.1/forwardbasespawner/api_list_servers.py
+-rw-r--r--   0        0        0     3741 2020-02-02 00:00:00.000000 jupyterhub_forwardbasespawner-1.0.1/forwardbasespawner/api_setup_tunnel.py
+-rw-r--r--   0        0        0     1900 2020-02-02 00:00:00.000000 jupyterhub_forwardbasespawner-1.0.1/forwardbasespawner/api_sshnode_restarted.py
+-rw-r--r--   0        0        0    64098 2020-02-02 00:00:00.000000 jupyterhub_forwardbasespawner-1.0.1/forwardbasespawner/forward.py
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 jupyterhub_forwardbasespawner-1.0.1/forwardbasespawner/utils.py
+-rw-r--r--   0        0        0     2591 2020-02-02 00:00:00.000000 jupyterhub_forwardbasespawner-1.0.1/.gitignore
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 jupyterhub_forwardbasespawner-1.0.1/LICENSE
+-rw-r--r--   0        0        0     2355 2020-02-02 00:00:00.000000 jupyterhub_forwardbasespawner-1.0.1/README.md
+-rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 jupyterhub_forwardbasespawner-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     4603 2020-02-02 00:00:00.000000 jupyterhub_forwardbasespawner-1.0.1/PKG-INFO
```

### Comparing `jupyterhub_forwardbasespawner-1.0.0/.gitlab-ci.yml` & `jupyterhub_forwardbasespawner-1.0.1/.gitlab-ci.yml`

 * *Files 8% similar despite different names*

```diff
@@ -13,40 +13,40 @@
     name: python:alpine
   before_script:
     - pip install twine build
   script:
     - python -m build
     - twine upload -u __token__ -p ${PYPI_JUPYTERJSC_TOKEN} dist/*
   rules:
-    - if: '$CI_COMMIT_TAG =~ /^\d+\.\d+\.\d+$/'
+    - if: '$CI_COMMIT_TAG =~ /^\d+\.\d+\.\d+(\.post\d+)?$/'
 
 testpypi:
   stage: release
   image:
     name: python:alpine
   before_script:
     - pip install twine build
   script:
     - python -m build
     - twine upload --repository testpypi -u __token__ -p ${TESTPYPI_JUPYTERJSC_TOKEN} dist/*
   rules:
-    - if: '$CI_COMMIT_TAG =~ /^\d+\.\d+\.\d+(-.+)$/'
+    - if: '$CI_COMMIT_TAG !~ /^\d+\.\d+\.\d+(\.post\d+)?$/'
 
 
 ###
 #
 # Prepare release notes
 #
 ###
 
 prepare_job:
   stage: prepare-release
   image: alpine:latest
   rules:
-  - if: '$CI_COMMIT_TAG =~ /^\d+\.\d+\.\d+$/'
+    - if: '$CI_COMMIT_TAG =~ /^\d+\.\d+\.\d+(\.post\d+)?$/'
   script:
     - apk add curl jq
     - 'curl -H "PRIVATE-TOKEN: $CI_API_TOKEN" "$CI_API_V4_URL/projects/$CI_PROJECT_ID/repository/changelog?version=$CI_COMMIT_TAG" | jq -r .notes > release_notes.md'
     - 'curl -H "PRIVATE-TOKEN: $CI_API_TOKEN" -X POST "$CI_API_V4_URL/projects/$CI_PROJECT_ID/repository/changelog?version=$CI_COMMIT_TAG"'
   artifacts:
     paths:
     - release_notes.md
@@ -60,15 +60,15 @@
 release_job:
   stage: release
   image: registry.gitlab.com/gitlab-org/release-cli:latest
   needs:
     - job: prepare_job
       artifacts: true
   rules:
-  - if: '$CI_COMMIT_TAG =~ /^\d+\.\d+\.\d+$/'
+    - if: '$CI_COMMIT_TAG =~ /^\d+\.\d+\.\d+(\.post\d+)?$/'
   script:
     - echo "Creating release"
   release:
     name: 'Release $CI_COMMIT_TAG'
     description: release_notes.md
     tag_name: '$CI_COMMIT_TAG'
     ref: '$CI_COMMIT_SHA'
```

### Comparing `jupyterhub_forwardbasespawner-1.0.0/docs/Doxyfile` & `jupyterhub_forwardbasespawner-1.0.1/docs/Doxyfile`

 * *Files identical despite different names*

### Comparing `jupyterhub_forwardbasespawner-1.0.0/docs/Makefile` & `jupyterhub_forwardbasespawner-1.0.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `jupyterhub_forwardbasespawner-1.0.0/docs/apiendpoints.md` & `jupyterhub_forwardbasespawner-1.0.1/docs/apiendpoints.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # API Endpoints
 
-Below is an interactive view of the OutpostSpawner REST API specification.
+Below is an interactive view of the ForwardBaseSpawner REST API specification.
 
 <!-- client-rendered openapi UI copied from FastAPI -->
 
 <link type="text/css" rel="stylesheet" href="https://cdn.jsdelivr.net/npm/swagger-ui-dist@3/swagger-ui.css">
 <script src="https://cdn.jsdelivr.net/npm/swagger-ui-dist@4.1/swagger-ui-bundle.js"></script>
 <!-- `SwaggerUIBundle` is now available on the page -->
```

#### html2text {}

```diff
@@ -1,2 +1,2 @@
-# API Endpoints Below is an interactive view of the OutpostSpawner REST API
+# API Endpoints Below is an interactive view of the ForwardBaseSpawner REST API
 specification.
```

### Comparing `jupyterhub_forwardbasespawner-1.0.0/docs/conf.py` & `jupyterhub_forwardbasespawner-1.0.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `jupyterhub_forwardbasespawner-1.0.0/docs/index.md` & `jupyterhub_forwardbasespawner-1.0.1/docs/index.md`

 * *Files 4% similar despite different names*

```diff
@@ -39,7 +39,15 @@
 .. toctree::
     :maxdepth: 2
     :caption: Classes
 
     spawners/forwardbasespawner
     apiendpoints
 ```
+
+```{eval-rst}
+.. toctree::
+    :maxdepth: 2
+    :caption: Reference
+
+    changelog
+```
```

### Comparing `jupyterhub_forwardbasespawner-1.0.0/docs/make.bat` & `jupyterhub_forwardbasespawner-1.0.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `jupyterhub_forwardbasespawner-1.0.0/docs/_static/rest-api.yml` & `jupyterhub_forwardbasespawner-1.0.1/docs/_static/rest-api.yml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 openapi: 3.0.3
 info:
-  title: JupyterHub OutpostSpawner
-  description: The REST API for JupyterHub OutpostSpawner
+  title: JupyterHub ForwardBaseSpawner
+  description: The REST API for JupyterHub ForwardBaseSpawner
   license:
     name: BSD-3-Clause
 servers:
   - url: /hub/api
 security:
   - token: []
 paths:
@@ -274,15 +274,15 @@
           application/json:
             schema:
               type: object
               properties:
                 service:
                   type: string
                   description: |
-                    Where the JupyterHub Outpost will be able to reach
+                    Where JupyterHub will be able to reach
                     the JupyterLab.
                   required: true
                 ssh_port:
                   type: int
                   description: |
                     Port used to create connection to the <ssh_node>
                   required: false
@@ -362,15 +362,15 @@
           application/json:
             schema:
               type: object
               properties:
                 service:
                   type: string
                   description: |
-                    Where the JupyterHub Outpost will be able to reach
+                    Where JupyterHub will be able to reach
                     the JupyterLab.
                   required: true
                 ssh_port:
                   type: int
                   description: |
                     Port used to create connection to the <ssh_node>
                   required: false
```

### Comparing `jupyterhub_forwardbasespawner-1.0.0/docs/spawners/forwardbasespawner.md` & `jupyterhub_forwardbasespawner-1.0.1/docs/spawners/forwardbasespawner.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# OutpostSpawner
+# ForwardBaseSpawner
 
 ```{eval-rst}
 .. automodule:: forwardbasespawner
 ```
 
 ```{eval-rst}
 .. autoconfigurable:: ForwardBaseSpawner
```

### Comparing `jupyterhub_forwardbasespawner-1.0.0/forwardbasespawner/api_events.py` & `jupyterhub_forwardbasespawner-1.0.1/forwardbasespawner/api_events.py`

 * *Files identical despite different names*

### Comparing `jupyterhub_forwardbasespawner-1.0.0/forwardbasespawner/api_list_servers.py` & `jupyterhub_forwardbasespawner-1.0.1/forwardbasespawner/api_list_servers.py`

 * *Files identical despite different names*

### Comparing `jupyterhub_forwardbasespawner-1.0.0/forwardbasespawner/api_setup_tunnel.py` & `jupyterhub_forwardbasespawner-1.0.1/forwardbasespawner/api_setup_tunnel.py`

 * *Files identical despite different names*

### Comparing `jupyterhub_forwardbasespawner-1.0.0/forwardbasespawner/api_sshnode_restarted.py` & `jupyterhub_forwardbasespawner-1.0.1/forwardbasespawner/api_sshnode_restarted.py`

 * *Files identical despite different names*

### Comparing `jupyterhub_forwardbasespawner-1.0.0/forwardbasespawner/forward.py` & `jupyterhub_forwardbasespawner-1.0.1/forwardbasespawner/forward.py`

 * *Files 0% similar despite different names*

```diff
@@ -222,47 +222,47 @@
             c.ForwardBaseSpawner.ssh_remote_key = ssh_remote_key
 
         """,
     ).tag(config=True)
 
     ssh_username = Union(
         [Callable(), Unicode()],
-        default_value="jupyterhuboutpost",
+        default_value="jhuboutpost",
         help="""
         An optional hook function, or string, you can implement to
         set the ssh username used for ssh port forwarding.
 
         This may be a coroutine.
 
         Example::
 
             def ssh_username(spawner):
                 if spawner.user_options.get("system", "") == "A":
-                    return "jupyterhuboutpost"
+                    return "jhuboutpost"
                 return "ubuntu"
 
             c.ForwardBaseSpawner.ssh_username = ssh_username
 
         """,
     ).tag(config=True)
 
     ssh_remote_username = Union(
         [Callable(), Unicode()],
-        default_value="jupyterhuboutpost",
+        default_value="jhuboutpost",
         help="""
         An optional hook function, or string, you can implement to
         set the ssh username used for ssh port forwarding remote.
 
         This may be a coroutine.
 
         Example::
 
             def ssh_username(spawner):
                 if spawner.user_options.get("system", "") == "A":
-                    return "jupyterhuboutpost"
+                    return "jhuboutpost"
                 return "ubuntu"
 
             c.ForwardBaseSpawner.ssh_remote_username = ssh_username
 
         """,
     ).tag(config=True)
 
@@ -949,29 +949,29 @@
             )
         return ssh_remote_port
 
     async def get_ssh_username(self):
         """Get ssh username
 
         Returns:
-          ssh_user (string): Used in ssh forward command. Default ist "jupyterhuboutpost"
+          ssh_user (string): Used in ssh forward command. Default is "jhuboutpost"
         """
         if callable(self.ssh_username):
             ssh_user = await maybe_future(
                 self.ssh_username(self, self.port_forward_info)
             )
         else:
             ssh_user = self.port_forward_info.get("ssh_username", self.ssh_username)
         return ssh_user
 
     async def get_ssh_remote_username(self):
         """Get ssh username
 
         Returns:
-          ssh_remote_username (string): Used in ssh forward command. Default ist "None"
+          ssh_remote_username (string): Used in ssh forward command. Default is "None"
         """
         if callable(self.ssh_remote_username):
             ssh_remote_username = await maybe_future(
                 self.ssh_remote_username(self, self.port_forward_info.get("remote", {}))
             )
         else:
             ssh_remote_username = self.port_forward_info.get("remote", {}).get(
@@ -1038,14 +1038,16 @@
 
         Returns:
           ssh_node_mapping (string): Used in ssh port forwading command
         """
 
         if callable(self.ssh_node_mapping):
             ssh_node_mapping = await maybe_future(self.ssh_node_mapping(self, ssh_node))
+        else:
+            ssh_node_mapping = ssh_node
         return ssh_node_mapping
 
     async def get_ssh_remote_node(self):
         """Get ssh node
 
         Returns:
           ssh_remote_node (string): Used in ssh port forwading remote command
@@ -1061,15 +1063,15 @@
             )
         return ssh_remote_node
 
     async def get_svc_create(self):
         """Get ssh username
 
         Returns:
-          ssh_user (string): Used in ssh forward command. Default ist "jupyterhuboutpost"
+          svc_create (bool): Whether a service should be created. Default is True
         """
         if callable(self.svc_create):
             svc_create = await maybe_future(self.svc_create(self))
         else:
             svc_create = self.svc_create
         return svc_create
```

### Comparing `jupyterhub_forwardbasespawner-1.0.0/.gitignore` & `jupyterhub_forwardbasespawner-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyterhub_forwardbasespawner-1.0.0/LICENSE` & `jupyterhub_forwardbasespawner-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterhub_forwardbasespawner-1.0.0/pyproject.toml` & `jupyterhub_forwardbasespawner-1.0.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -45,23 +45,24 @@
 profile = "black"
 
 [tool.tbump]
 # Uncomment this if your project is hosted on GitHub:
 github_url = "https://github.com/kreuzert/jupyterhub-forwardbasespawner"
 
 [tool.tbump.version]
-current = "1.0.0"
+current = "1.0.1"
 regex = '''
   (?P<major>\d+)
   \.
   (?P<minor>\d+)
   \.
   (?P<patch>\d+)
   (?P<pre>((a|b|rc)\d+)|)
   \.?
+  (?P<post>((post)\d+)|)
   (?P<dev>(?<=\.)dev\d*|)
 '''
 
 [tool.tbump.git]
 message_template = "Bump to {new_version}"
 tag_template = "{new_version}"
```

