# Comparing `tmp/kube_compose-0.1.0.tar.gz` & `tmp/kube_compose-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kube_compose-0.1.0.tar", max compression
+gzip compressed data, was "kube_compose-0.2.0.tar", max compression
```

## Comparing `kube_compose-0.1.0.tar` & `kube_compose-0.2.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0    11357 2023-12-26 21:08:41.487950 kube_compose-0.1.0/LICENSE
--rw-r--r--   0        0        0     2548 2023-12-26 22:03:05.285775 kube_compose-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-12-26 21:09:16.732631 kube_compose-0.1.0/kube_compose/__init__.py
--rw-r--r--   0        0        0      286 2023-12-26 21:09:16.732631 kube_compose-0.1.0/kube_compose/__main__.py
--rw-r--r--   0        0        0      144 2023-12-26 21:09:16.732631 kube_compose-0.1.0/kube_compose/charts/kube-compose/Chart.yaml
--rw-r--r--   0        0        0     3236 2023-12-26 21:09:16.732631 kube_compose-0.1.0/kube_compose/charts/kube-compose/templates/deployment.yaml
--rw-r--r--   0        0        0       69 2023-12-26 21:09:16.732631 kube_compose-0.1.0/kube_compose/cli/__init__.py
--rw-r--r--   0        0        0      387 2023-12-26 21:09:20.839455 kube_compose-0.1.0/kube_compose/cli/config.py
--rw-r--r--   0        0        0     1006 2023-12-26 21:09:16.732631 kube_compose-0.1.0/kube_compose/cli/cp.py
--rw-r--r--   0        0        0     1042 2023-12-26 21:09:16.732631 kube_compose-0.1.0/kube_compose/cli/diff.py
--rw-r--r--   0        0        0      604 2023-12-26 21:09:16.732631 kube_compose-0.1.0/kube_compose/cli/down.py
--rw-r--r--   0        0        0      793 2023-12-26 21:09:16.732631 kube_compose-0.1.0/kube_compose/cli/exec.py
--rw-r--r--   0        0        0     1098 2023-12-26 21:09:20.839455 kube_compose-0.1.0/kube_compose/cli/init.py
--rw-r--r--   0        0        0     1157 2023-12-26 21:09:16.732631 kube_compose-0.1.0/kube_compose/cli/logs.py
--rw-r--r--   0        0        0      702 2023-12-26 21:09:16.732631 kube_compose-0.1.0/kube_compose/cli/ls.py
--rw-r--r--   0        0        0      406 2023-12-26 21:09:16.732631 kube_compose-0.1.0/kube_compose/cli/ps.py
--rw-r--r--   0        0        0      801 2023-12-26 22:01:26.475304 kube_compose-0.1.0/kube_compose/cli/restart.py
--rw-r--r--   0        0        0     2073 2023-12-26 21:09:16.732631 kube_compose-0.1.0/kube_compose/cli/run.py
--rw-r--r--   0        0        0     1168 2023-12-26 22:02:27.567657 kube_compose-0.1.0/kube_compose/cli/up.py
--rw-r--r--   0        0        0     1577 2023-12-26 21:09:16.732631 kube_compose-0.1.0/kube_compose/cli/version.py
--rw-r--r--   0        0        0      147 2023-12-26 21:09:16.732631 kube_compose-0.1.0/kube_compose/cli/volume/__init__.py
--rw-r--r--   0        0        0     1296 2023-12-26 21:09:20.832788 kube_compose-0.1.0/kube_compose/cli/volume/create.py
--rw-r--r--   0        0        0      512 2023-12-26 21:09:16.732631 kube_compose-0.1.0/kube_compose/cli/volume/inspect.py
--rw-r--r--   0        0        0      425 2023-12-26 21:09:16.732631 kube_compose-0.1.0/kube_compose/cli/volume/ls.py
--rw-r--r--   0        0        0      619 2023-12-26 21:09:20.832788 kube_compose-0.1.0/kube_compose/cli/volume/rm.py
--rw-r--r--   0        0        0     3250 2023-12-26 21:09:16.732631 kube_compose-0.1.0/kube_compose/utils.py
--rw-r--r--   0        0        0      475 2023-12-26 21:10:29.552082 kube_compose-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3070 1970-01-01 00:00:00.000000 kube_compose-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-12-26 21:08:41.487950 kube_compose-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2548 2023-12-26 22:03:05.285775 kube_compose-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-12-26 21:09:16.732631 kube_compose-0.2.0/kube_compose/__init__.py
+-rw-r--r--   0        0        0      286 2023-12-26 21:09:16.732631 kube_compose-0.2.0/kube_compose/__main__.py
+-rw-r--r--   0        0        0      144 2023-12-26 21:09:16.732631 kube_compose-0.2.0/kube_compose/charts/kube-compose/Chart.yaml
+-rw-r--r--   0        0        0     4098 2024-05-07 16:06:01.338401 kube_compose-0.2.0/kube_compose/charts/kube-compose/templates/deployment.yaml
+-rw-r--r--   0        0        0       69 2023-12-26 21:09:16.732631 kube_compose-0.2.0/kube_compose/cli/__init__.py
+-rw-r--r--   0        0        0      387 2023-12-26 21:09:20.839455 kube_compose-0.2.0/kube_compose/cli/config.py
+-rw-r--r--   0        0        0     1006 2023-12-26 21:09:16.732631 kube_compose-0.2.0/kube_compose/cli/cp.py
+-rw-r--r--   0        0        0     1042 2023-12-26 21:09:16.732631 kube_compose-0.2.0/kube_compose/cli/diff.py
+-rw-r--r--   0        0        0      604 2023-12-26 21:09:16.732631 kube_compose-0.2.0/kube_compose/cli/down.py
+-rw-r--r--   0        0        0      793 2023-12-26 21:09:16.732631 kube_compose-0.2.0/kube_compose/cli/exec.py
+-rw-r--r--   0        0        0     1098 2023-12-26 21:09:20.839455 kube_compose-0.2.0/kube_compose/cli/init.py
+-rw-r--r--   0        0        0     1157 2023-12-26 21:09:16.732631 kube_compose-0.2.0/kube_compose/cli/logs.py
+-rw-r--r--   0        0        0      702 2023-12-26 21:09:16.732631 kube_compose-0.2.0/kube_compose/cli/ls.py
+-rw-r--r--   0        0        0      406 2023-12-26 21:09:16.732631 kube_compose-0.2.0/kube_compose/cli/ps.py
+-rw-r--r--   0        0        0      801 2023-12-26 22:01:26.475304 kube_compose-0.2.0/kube_compose/cli/restart.py
+-rw-r--r--   0        0        0     2083 2024-01-23 16:48:28.990125 kube_compose-0.2.0/kube_compose/cli/run.py
+-rw-r--r--   0        0        0     1168 2023-12-26 22:02:27.567657 kube_compose-0.2.0/kube_compose/cli/up.py
+-rw-r--r--   0        0        0     1577 2023-12-26 21:09:16.732631 kube_compose-0.2.0/kube_compose/cli/version.py
+-rw-r--r--   0        0        0      147 2023-12-26 21:09:16.732631 kube_compose-0.2.0/kube_compose/cli/volume/__init__.py
+-rw-r--r--   0        0        0     1299 2024-01-23 16:48:48.390653 kube_compose-0.2.0/kube_compose/cli/volume/create.py
+-rw-r--r--   0        0        0      512 2023-12-26 21:09:16.732631 kube_compose-0.2.0/kube_compose/cli/volume/inspect.py
+-rw-r--r--   0        0        0      425 2023-12-26 21:09:16.732631 kube_compose-0.2.0/kube_compose/cli/volume/ls.py
+-rw-r--r--   0        0        0      619 2023-12-26 21:09:20.832788 kube_compose-0.2.0/kube_compose/cli/volume/rm.py
+-rw-r--r--   0        0        0     3213 2024-05-07 16:02:40.766979 kube_compose-0.2.0/kube_compose/utils.py
+-rw-r--r--   0        0        0      475 2024-05-08 12:49:01.525071 kube_compose-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3070 1970-01-01 00:00:00.000000 kube_compose-0.2.0/PKG-INFO
```

### Comparing `kube_compose-0.1.0/LICENSE` & `kube_compose-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kube_compose-0.1.0/README.md` & `kube_compose-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `kube_compose-0.1.0/kube_compose/charts/kube-compose/templates/deployment.yaml` & `kube_compose-0.2.0/kube_compose/charts/kube-compose/templates/deployment.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,31 @@
 {{- define "env" -}}
 env:
 - null
 {{- range $name, $value := .service.environment | default list }}
-{{- if ne $value nil }}
+{{- if ne ($value | toJson) "null" }}
+{{- if typeIs "int" $name }}
+{{- $value_parsed := regexSplit "=" $value 2 }}
+{{- $name := first $value_parsed }}
+{{- $value := last $value_parsed }}
 - name: {{ $name | toJson }}
   value: {{ $value | replace "$$" "$" | toJson }}
+{{- else }}
+- name: {{ $name | toJson }}
+  value: {{ $value | replace "$$" "$" | toJson }}
+{{- end }}
 {{- end }}
 {{- end }}
 {{- end -}}
 
 {{- define "ports" -}}
 ports:
 - null
 {{- range $portIndex, $port := .service.ports | default list }}
-- name: port-{{ $portIndex }}
+- name: {{ lower $port.protocol }}-{{ $port.target }}
   containerPort: {{ $port.target }}
   protocol: {{ upper $port.protocol }}
 {{- end -}}
 {{- end -}}
 
 {{- define "volumes" -}}
 volumes:
@@ -25,24 +33,65 @@
 {{- range $volume := .service.volumes | default list }}
 - name: {{ $volume.source }}
   mountPath: {{ $volume.target }}
   subPath: data
 {{- end }}
 {{- end -}}
 
+{{- define "template" -}}
+metadata:
+  labels:
+    app.kubernetes.io/name: {{ .name }}
+spec:
+  containers:
+  - name: {{ .name }}
+    image: {{ .service.image | toJson }}
+    imagePullPolicy: {{ .config.imagePullPolicy | default "Always" | toJson }}
+    {{- if .service.command }}
+    command: {{ list (index .service.command 0) | toJson }}
+    args: {{ slice .service.command 1 | toJson }}
+    {{- end }}
+    {{- if .env }}
+    env:
+{{ toYaml .env | indent 8 }}
+    {{- end }}
+    {{- if .volumes }}
+    volumeMounts:
+{{ toYaml .volumes | indent 8 }}
+    {{- end }}
+    {{- if .ports }}
+    ports:
+{{ toYaml .ports | indent 8 }}
+    {{- end }}
+  dnsPolicy: {{ .config.dnsPolicy | default "ClusterFirst" }}
+  restartPolicy: {{ .config.restartPolicy | default "Always" }}
+  {{- if .volumes }}
+  volumes:
+  {{- range $vol := .volumes }}
+  {{- $volName := index $vol "name"}}
+  - name: {{ $volName }}
+    persistentVolumeClaim:
+      claimName: {{ $volName }}
+  {{- end }}
+  {{- end }}
+{{- end -}}
+
+
 {{- range $name, $service := $.Values.services }}
 {{- with dict "name" $name "service" $service }}
 {{- $config := index .service "x-kubernetes" | default dict }}
 {{- if not ($config.exclude | default false) }}
 {{- $ports := slice (index ((include "ports" .) | fromYaml) "ports") 1 }}
 {{- $env := slice (index ((include "env" .) | fromYaml) "env") 1 }}
 {{- $volumes := slice (index ((include "volumes" .) | fromYaml) "volumes") 1 }}
+{{ with merge . (dict "config" $config "ports" $ports "env" $env "volumes" $volumes) }}
 ---
+{{- if eq ($config.cron | default "") "" }}
 apiVersion: apps/v1
-{{- if eq (.service.deploy | default dict).mode "global" }}
+{{- if eq ((.service.deploy | default dict).mode | default "") "global" }}
 kind: DaemonSet
 {{- else }}
 kind: Deployment
 {{- end }}
 metadata:
   {{- if $config.labels }}
   labels:
@@ -55,49 +104,15 @@
   name: {{ $name }}
 spec:
   replicas: {{ (.service.deploy | default dict).replicas | default 1 }}
   selector:
     matchLabels:
       app.kubernetes.io/name: {{ $name }}
   template:
-    metadata:
-      labels:
-        app.kubernetes.io/name: {{ $name }}
-    spec:
-      containers:
-      - name: {{ $name }}
-        image: {{ .service.image | toJson }}
-        imagePullPolicy: {{ $config.imagePullPolicy | default "Always" | toJson }}
-        {{- if .service.command }}
-        command: {{ list (index .service.command 0) | toJson }}
-        args: {{ slice .service.command 1 | toJson }}
-        {{- end }}
-        {{- if $env }}
-        env:
-{{ toYaml $env | indent 8 }}
-        {{- end }}
-        {{- if $volumes }}
-        volumeMounts:
-{{ toYaml $volumes | indent 8 }}
-        {{- end }}
-        {{- if $ports }}
-        ports:
-{{ toYaml $ports | indent 8 }}
-        {{- end }}
-      dnsPolicy: {{ $config.dnsPolicy | default "ClusterFirst" }}
-      restartPolicy: {{ $config.restartPolicy | default "Always" }}
-      {{- if $volumes }}
-      volumes:
-      {{- range $vol := $volumes }}
-      {{- $volName := index $vol "name"}}
-      - name: {{ $volName }}
-        persistentVolumeClaim:
-          claimName: {{ $volName }}
-      {{- end }}
-      {{- end }}
+{{ toYaml ((include "template" .) | fromYaml) | indent 4 }}
 
 {{- if $ports }}
 ---
 apiVersion: v1
 kind: Service
 metadata:
   {{- if $config.labels }}
@@ -110,16 +125,38 @@
   {{- end }}
   name: {{ $name }}
 spec:
   selector:
     app.kubernetes.io/name: {{ $name }}
   ports:
     {{- range $ports }}
-    - protocol: {{ .protocol }}
+    - name: {{ .name }}
+      protocol: {{ .protocol }}
       port: {{ .containerPort }}
       targetPort: {{ .containerPort }}
     {{- end }}
 {{- end }}
 
+{{- else }}
+apiVersion: batch/v1
+kind: CronJob
+metadata:
+  {{- if $config.labels }}
+  labels:
+{{ toYaml $config.labels | indent 4 }}
+  {{- end }}
+  {{- if $config.annotations }}
+  annotations:
+{{ toYaml $config.annotations | indent 4 }}
+  {{- end }}
+  name: {{ $name }}
+spec:
+  schedule: {{ $config.cron }}
+  jobTemplate:
+    spec:
+      template:
+{{ toYaml ((include "template" .) | fromYaml) | indent 8 }}
+{{- end }}
+{{- end }}
 {{- end }}
 {{- end }}
 {{- end }}
```

### Comparing `kube_compose-0.1.0/kube_compose/cli/cp.py` & `kube_compose-0.2.0/kube_compose/cli/cp.py`

 * *Files identical despite different names*

### Comparing `kube_compose-0.1.0/kube_compose/cli/diff.py` & `kube_compose-0.2.0/kube_compose/cli/diff.py`

 * *Files identical despite different names*

### Comparing `kube_compose-0.1.0/kube_compose/cli/down.py` & `kube_compose-0.2.0/kube_compose/cli/down.py`

 * *Files identical despite different names*

### Comparing `kube_compose-0.1.0/kube_compose/cli/exec.py` & `kube_compose-0.2.0/kube_compose/cli/exec.py`

 * *Files identical despite different names*

### Comparing `kube_compose-0.1.0/kube_compose/cli/init.py` & `kube_compose-0.2.0/kube_compose/cli/init.py`

 * *Files identical despite different names*

### Comparing `kube_compose-0.1.0/kube_compose/cli/logs.py` & `kube_compose-0.2.0/kube_compose/cli/logs.py`

 * *Files identical despite different names*

### Comparing `kube_compose-0.1.0/kube_compose/cli/ls.py` & `kube_compose-0.2.0/kube_compose/cli/ls.py`

 * *Files identical despite different names*

### Comparing `kube_compose-0.1.0/kube_compose/cli/restart.py` & `kube_compose-0.2.0/kube_compose/cli/restart.py`

 * *Files identical despite different names*

### Comparing `kube_compose-0.1.0/kube_compose/cli/run.py` & `kube_compose-0.2.0/kube_compose/cli/run.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     ]
   #
   if service_config.get('volumes'):
     overrides['spec']['containers'][0]['volumeMounts'] = []
     overrides['spec']['volumes'] = []
     for volume in service_config['volumes']:
       from kube_compose.cli.volume.create import create
-      create(volume=volume)
+      create(volume=volume['source'])
       overrides['spec']['containers'][0]['volumeMounts'].append(
         {
           'mountPath': volume['target'],
           'name': volume['source'],
         }
       )
       overrides['spec']['volumes'].append(
```

### Comparing `kube_compose-0.1.0/kube_compose/cli/up.py` & `kube_compose-0.2.0/kube_compose/cli/up.py`

 * *Files identical despite different names*

### Comparing `kube_compose-0.1.0/kube_compose/cli/version.py` & `kube_compose-0.2.0/kube_compose/cli/version.py`

 * *Files identical despite different names*

### Comparing `kube_compose-0.1.0/kube_compose/cli/volume/create.py` & `kube_compose-0.2.0/kube_compose/cli/volume/create.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
   ''' Ensure a kubernetes persistent volume is created
   '''
   create(**kwargs)
 
 @utils.require_binaries(kubectl='kubectl')
 @utils.require_kube_compose_release
 def create(*, volume, docker_compose_config, namespace, kubectl, **_):
-  for volume, volume_config in ([volume, docker_compose_config['volumes'][volume]] if volume is not None else docker_compose_config.get('volumes', {}).items()):
+  for volume, volume_config in ([(volume, docker_compose_config['volumes'][volume],)] if volume is not None else docker_compose_config.get('volumes', {}).items()):
     volume_ext_config = volume_config.get('x-kubernetes', {})
     utils.run([
       kubectl, 'apply',
       *(('-n', namespace) if namespace else tuple()),
       '-f', '-',
     ], input=json.dumps({
       'apiVersion': 'v1',
```

### Comparing `kube_compose-0.1.0/kube_compose/cli/volume/inspect.py` & `kube_compose-0.2.0/kube_compose/cli/volume/inspect.py`

 * *Files identical despite different names*

### Comparing `kube_compose-0.1.0/kube_compose/cli/volume/rm.py` & `kube_compose-0.2.0/kube_compose/cli/volume/rm.py`

 * *Files identical despite different names*

### Comparing `kube_compose-0.1.0/kube_compose/utils.py` & `kube_compose-0.2.0/kube_compose/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -79,26 +79,26 @@
   click.echo_via_pager([
     ' '.join(('{:^%d}' % (colSize[i])).format(cell) for i, cell in enumerate(record)) + '\n'
     for record in records
   ])
 
 def require_kube_compose_release(fn):
   @functools.wraps(fn)
-  @require_binaries(docker_compose='docker-compose')
-  def wrapper(*, docker_compose, **kwargs):
+  @require_binaries(docker='docker')
+  def wrapper(*, docker, **kwargs):
     import yaml
-    docker_compose_config_raw = check_output([docker_compose, 'config'])
+    docker_compose_config_raw = check_output([docker, 'compose', 'config'])
     docker_compose_config = yaml.safe_load(docker_compose_config_raw)
     if 'x-kubernetes' not in docker_compose_config:
       raise click.ClickException('top-level `x-kubernetes` map with release `name` and `namespace` is required')
     release_config = docker_compose_config['x-kubernetes']
     name = release_config['name']
     namespace = release_config.get('namespace')
     return fn(**dict(kwargs,
-      docker_compose=docker_compose,
+      docker=docker,
       docker_compose_config_raw=docker_compose_config_raw,
       docker_compose_config=docker_compose_config,
       release_config=release_config,
       name=name,
       namespace=namespace,
     ))
   return wrapper
```

### Comparing `kube_compose-0.1.0/PKG-INFO` & `kube_compose-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kube-compose
-Version: 0.1.0
+Version: 0.2.0
 Summary: An opinionated way of deploying docker-compose to kubernetes clusters by managing them with a helm chart.
 Author: Daniel Clarke
 Author-email: u8sand@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

