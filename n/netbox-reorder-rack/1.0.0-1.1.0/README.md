# Comparing `tmp/netbox_reorder_rack-1.0.0.tar.gz` & `tmp/netbox_reorder_rack-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox_reorder_rack-1.0.0.tar", last modified: Wed Mar 13 15:09:52 2024, max compression
+gzip compressed data, was "netbox_reorder_rack-1.1.0.tar", last modified: Wed May  8 14:20:42 2024, max compression
```

## Comparing `netbox_reorder_rack-1.0.0.tar` & `netbox_reorder_rack-1.1.0.tar`

### file list

```diff
@@ -1,41 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 15:09:52.832023 netbox_reorder_rack-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-03-13 15:09:47.000000 netbox_reorder_rack-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-03-13 15:09:52.832023 netbox_reorder_rack-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-03-13 15:09:47.000000 netbox_reorder_rack-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 15:09:52.828023 netbox_reorder_rack-1.0.0/netbox_reorder_rack/
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-03-13 15:09:47.000000 netbox_reorder_rack-1.0.0/netbox_reorder_rack/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 15:09:52.832023 netbox_reorder_rack-1.0.0/netbox_reorder_rack/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 15:09:47.000000 netbox_reorder_rack-1.0.0/netbox_reorder_rack/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-03-13 15:09:47.000000 netbox_reorder_rack-1.0.0/netbox_reorder_rack/api/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-03-13 15:09:47.000000 netbox_reorder_rack-1.0.0/netbox_reorder_rack/api/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 15:09:52.828023 netbox_reorder_rack-1.0.0/netbox_reorder_rack/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 15:09:52.828023 netbox_reorder_rack-1.0.0/netbox_reorder_rack/static/netbox_reorder_rack/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 15:09:52.832023 netbox_reorder_rack-1.0.0/netbox_reorder_rack/static/netbox_reorder_rack/css/
--rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-03-13 15:09:47.000000 netbox_reorder_rack-1.0.0/netbox_reorder_rack/static/netbox_reorder_rack/css/rack.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 15:09:52.832023 netbox_reorder_rack-1.0.0/netbox_reorder_rack/static/netbox_reorder_rack/js/
--rw-r--r--   0 runner    (1001) docker     (127)   193050 2024-03-13 15:09:47.000000 netbox_reorder_rack-1.0.0/netbox_reorder_rack/static/netbox_reorder_rack/js/rack.js
--rw-r--r--   0 runner    (1001) docker     (127)    93246 2024-03-13 15:09:47.000000 netbox_reorder_rack-1.0.0/netbox_reorder_rack/static/netbox_reorder_rack/js/rack.js.map
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-03-13 15:09:47.000000 netbox_reorder_rack-1.0.0/netbox_reorder_rack/template_content.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 15:09:52.828023 netbox_reorder_rack-1.0.0/netbox_reorder_rack/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 15:09:52.832023 netbox_reorder_rack-1.0.0/netbox_reorder_rack/templates/netbox_reorder_rack/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 15:09:52.832023 netbox_reorder_rack-1.0.0/netbox_reorder_rack/templates/netbox_reorder_rack/inc/
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-03-13 15:09:47.000000 netbox_reorder_rack-1.0.0/netbox_reorder_rack/templates/netbox_reorder_rack/inc/rack_button.html
--rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-03-13 15:09:47.000000 netbox_reorder_rack-1.0.0/netbox_reorder_rack/templates/netbox_reorder_rack/inc/rack_elevation.html
--rw-r--r--   0 runner    (1001) docker     (127)     4361 2024-03-13 15:09:47.000000 netbox_reorder_rack-1.0.0/netbox_reorder_rack/templates/netbox_reorder_rack/rack.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 15:09:52.832023 netbox_reorder_rack-1.0.0/netbox_reorder_rack/templatetags/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 15:09:47.000000 netbox_reorder_rack-1.0.0/netbox_reorder_rack/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-03-13 15:09:47.000000 netbox_reorder_rack-1.0.0/netbox_reorder_rack/templatetags/rack.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 15:09:52.832023 netbox_reorder_rack-1.0.0/netbox_reorder_rack/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 15:09:47.000000 netbox_reorder_rack-1.0.0/netbox_reorder_rack/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6490 2024-03-13 15:09:47.000000 netbox_reorder_rack-1.0.0/netbox_reorder_rack/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-03-13 15:09:47.000000 netbox_reorder_rack-1.0.0/netbox_reorder_rack/tests/test_view.py
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-03-13 15:09:47.000000 netbox_reorder_rack-1.0.0/netbox_reorder_rack/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-03-13 15:09:47.000000 netbox_reorder_rack-1.0.0/netbox_reorder_rack/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 15:09:52.832023 netbox_reorder_rack-1.0.0/netbox_reorder_rack.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-03-13 15:09:52.000000 netbox_reorder_rack-1.0.0/netbox_reorder_rack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-03-13 15:09:52.000000 netbox_reorder_rack-1.0.0/netbox_reorder_rack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-13 15:09:52.000000 netbox_reorder_rack-1.0.0/netbox_reorder_rack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-13 15:09:52.000000 netbox_reorder_rack-1.0.0/netbox_reorder_rack.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-03-13 15:09:52.000000 netbox_reorder_rack-1.0.0/netbox_reorder_rack.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-13 15:09:52.832023 netbox_reorder_rack-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      873 2024-03-13 15:09:47.000000 netbox_reorder_rack-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:20:42.888701 netbox_reorder_rack-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-08 14:20:38.000000 netbox_reorder_rack-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-08 14:20:38.000000 netbox_reorder_rack-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-05-08 14:20:42.888701 netbox_reorder_rack-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-05-08 14:20:38.000000 netbox_reorder_rack-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:20:42.884701 netbox_reorder_rack-1.1.0/netbox_reorder_rack/
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-08 14:20:38.000000 netbox_reorder_rack-1.1.0/netbox_reorder_rack/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:20:42.884701 netbox_reorder_rack-1.1.0/netbox_reorder_rack/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 14:20:38.000000 netbox_reorder_rack-1.1.0/netbox_reorder_rack/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-08 14:20:38.000000 netbox_reorder_rack-1.1.0/netbox_reorder_rack/api/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-05-08 14:20:38.000000 netbox_reorder_rack-1.1.0/netbox_reorder_rack/api/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:20:42.880701 netbox_reorder_rack-1.1.0/netbox_reorder_rack/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:20:42.880701 netbox_reorder_rack-1.1.0/netbox_reorder_rack/static/netbox_reorder_rack/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:20:42.884701 netbox_reorder_rack-1.1.0/netbox_reorder_rack/static/netbox_reorder_rack/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-08 14:20:38.000000 netbox_reorder_rack-1.1.0/netbox_reorder_rack/static/netbox_reorder_rack/css/rack.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:20:42.884701 netbox_reorder_rack-1.1.0/netbox_reorder_rack/static/netbox_reorder_rack/js/
+-rw-r--r--   0 runner    (1001) docker     (127)    83425 2024-05-08 14:20:38.000000 netbox_reorder_rack-1.1.0/netbox_reorder_rack/static/netbox_reorder_rack/js/rack.js
+-rw-r--r--   0 runner    (1001) docker     (127)   102233 2024-05-08 14:20:38.000000 netbox_reorder_rack-1.1.0/netbox_reorder_rack/static/netbox_reorder_rack/js/rack.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-08 14:20:38.000000 netbox_reorder_rack-1.1.0/netbox_reorder_rack/template_content.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:20:42.884701 netbox_reorder_rack-1.1.0/netbox_reorder_rack/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:20:42.884701 netbox_reorder_rack-1.1.0/netbox_reorder_rack/templates/netbox_reorder_rack/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:20:42.888701 netbox_reorder_rack-1.1.0/netbox_reorder_rack/templates/netbox_reorder_rack/inc/
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-08 14:20:38.000000 netbox_reorder_rack-1.1.0/netbox_reorder_rack/templates/netbox_reorder_rack/inc/rack_button.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-05-08 14:20:38.000000 netbox_reorder_rack-1.1.0/netbox_reorder_rack/templates/netbox_reorder_rack/inc/rack_elevation.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4358 2024-05-08 14:20:38.000000 netbox_reorder_rack-1.1.0/netbox_reorder_rack/templates/netbox_reorder_rack/rack.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:20:42.888701 netbox_reorder_rack-1.1.0/netbox_reorder_rack/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 14:20:38.000000 netbox_reorder_rack-1.1.0/netbox_reorder_rack/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-05-08 14:20:38.000000 netbox_reorder_rack-1.1.0/netbox_reorder_rack/templatetags/rack.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:20:42.888701 netbox_reorder_rack-1.1.0/netbox_reorder_rack/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 14:20:38.000000 netbox_reorder_rack-1.1.0/netbox_reorder_rack/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6490 2024-05-08 14:20:38.000000 netbox_reorder_rack-1.1.0/netbox_reorder_rack/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-05-08 14:20:38.000000 netbox_reorder_rack-1.1.0/netbox_reorder_rack/tests/test_view.py
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-08 14:20:38.000000 netbox_reorder_rack-1.1.0/netbox_reorder_rack/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-05-08 14:20:38.000000 netbox_reorder_rack-1.1.0/netbox_reorder_rack/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:20:42.888701 netbox_reorder_rack-1.1.0/netbox_reorder_rack.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-05-08 14:20:42.000000 netbox_reorder_rack-1.1.0/netbox_reorder_rack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-08 14:20:42.000000 netbox_reorder_rack-1.1.0/netbox_reorder_rack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 14:20:42.000000 netbox_reorder_rack-1.1.0/netbox_reorder_rack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 14:20:42.000000 netbox_reorder_rack-1.1.0/netbox_reorder_rack.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-08 14:20:42.000000 netbox_reorder_rack-1.1.0/netbox_reorder_rack.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 14:20:42.888701 netbox_reorder_rack-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-05-08 14:20:38.000000 netbox_reorder_rack-1.1.0/setup.py
```

### Comparing `netbox_reorder_rack-1.0.0/PKG-INFO` & `netbox_reorder_rack-1.1.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: netbox_reorder_rack
-Version: 1.0.0
+Version: 1.1.0
 Summary: NetBox plugin to reorder rack layouts.
 Home-page: https://github.com/minitriga/netbox-reorder-rack/
 Author: Alex Gittings
 Author-email: agitting96@gmail.com
 Project-URL: Bug Tracker, https://github.com/minitriga/netbox-reorder-rack/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Framework :: Django
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # Netbox Reorder Rack Plugin
 
 ![Version](https://img.shields.io/pypi/v/netbox-reorder-rack) ![Downloads](https://img.shields.io/pypi/dm/netbox-reorder-rack)
 
 Allow the ability to reorder rack units in NetBox using a drag and drop interface.
 
@@ -53,15 +54,16 @@
 ```
 
 
 ## Compatibility Matrix
 
 | netbox version | plugin version |
 | -------------- | ----------------------------- |
-| >= 3.7.0       | >= v1.0.0                     |
+| >= 4.0.0       | >= v1.1.0                     |
+| <= 4.0.0       | = v1.0.0                     |
 
 ### Update
 
 To update the plugin, you need to update the package and restart NetBox.
 
 ```shell
 source /opt/netbox/venv/bin/activate
```

### Comparing `netbox_reorder_rack-1.0.0/README.md` & `netbox_reorder_rack-1.1.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -40,15 +40,16 @@
 ```
 
 
 ## Compatibility Matrix
 
 | netbox version | plugin version |
 | -------------- | ----------------------------- |
-| >= 3.7.0       | >= v1.0.0                     |
+| >= 4.0.0       | >= v1.1.0                     |
+| <= 4.0.0       | = v1.0.0                     |
 
 ### Update
 
 To update the plugin, you need to update the package and restart NetBox.
 
 ```shell
 source /opt/netbox/venv/bin/activate
```

### Comparing `netbox_reorder_rack-1.0.0/netbox_reorder_rack/api/views.py` & `netbox_reorder_rack-1.1.0/netbox_reorder_rack/api/views.py`

 * *Files identical despite different names*

### Comparing `netbox_reorder_rack-1.0.0/netbox_reorder_rack/templates/netbox_reorder_rack/inc/rack_elevation.html` & `netbox_reorder_rack-1.1.0/netbox_reorder_rack/templates/netbox_reorder_rack/inc/rack_elevation.html`

 * *Files 5% similar despite different names*

```diff
@@ -12,21 +12,21 @@
       </ul>
       <div class="grid-stack rack" id="grid-{{face}}" gs-column="2" gs-max-row="{{ object.u_height|mul:2 }}" gs-min-row="{{object.u_height|mul:2}}" data-grid-id="{% if front == 'front' %}0{% else %}1{% endif %}">
         {% for device in units %}
         {% if device.device %}
         {% if device.device.face == face %}
         <div class='grid-stack-item' gs-w='2' gs-h='{{ device.height|rack_unit_to_int|mul:2 }}' gs-x='0' gs-y='{{device|calculate_u_position:object}}' gs-id='{{device.device.id}}' gs-locked='false' data-item-color="{{device.device.role.color}}" data-item-text-color="{% if device.device.role.color %}{{ device.device.role.color|text_color }}{% else %}000000{% endif %}" data-full-depth="{{device.device.device_type.is_full_depth}}" data-item-face="{{ face }}">
           <div class='grid-stack-item-content' style="background-color: #{{device.device.role.color}}; color: #{% if device.device.role.color %}{{ device.device.role.color|text_color }}{% else %}000000{% endif %};">
-            {{device.device.name}}
+            {{ device.device | device_name }}
           </div>
         </div>
         {% else %}
         <div class='grid-stack-item' gs-w='2' gs-h='{{ device.height|rack_unit_to_int|mul:2 }}' gs-x='0' gs-y='{{device|calculate_u_position:object}}' gs-id='{{device.device.id}}' gs-locked='false' data-item-color="{{device.device.role.color}}" data-item-text-color="{% if device.device.role.color %}{{ device.device.role.color|text_color }}{% else %}000000{% endif %}" data-full-depth="{{device.device.device_type.is_full_depth}}" data-item-face="back">
           <div class='grid-stack-item-content device_rear' style="color: #000000">
-            {{device.device.name}}
+            {{ device.device.name }}
           </div>
         </div>
         {% endif %}
         {% endif %}
         {% endfor %}
       </div>
       <ul class="indexes"></ul>
```

### Comparing `netbox_reorder_rack-1.0.0/netbox_reorder_rack/templates/netbox_reorder_rack/rack.html` & `netbox_reorder_rack-1.1.0/netbox_reorder_rack/templates/netbox_reorder_rack/rack.html`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 {{ block.super }}
 {% endblock %}
 
 {% block title %}Reorder {{ object }}{% endblock %}
 
 {% block subtitle %}
 <div class="object-subtitle">
-  <span>Created {{ object.created|annotated_date }}</span>
+  <span>Created {{ object.created|isodatetime }}</span>
   <span class="separator">&middot;</span>
   <span>Updated <span title="{{ object.last_updated }}">{{ object.last_updated|timesince }}</span> ago</span>
 </div>
 {% endblock %}
 
 {% block tabs %}
 <ul class="nav nav-tabs px-3">
```

#### html2text {}

```diff
@@ -13,15 +13,15 @@
    8. {% endif %} {% endblock breadcrumbs %}
 {# Object identifier #}
 {% block object_identifier %} {{ object|meta:"app_label" }}.{{ object|meta:
 "model_name" }}:{{ object.pk }} {% if object.slug %}({{ object.slug }}){% endif
 %} {% endblock object_identifier %}
 {{ block.super }} {% endblock %} {% block title %}Reorder {{ object }}{%
 endblock %} {% block subtitle %}
-Created {{ object.created|annotated_date }} · Updated {
+Created {{ object.created|isodatetime }} · Updated {
 { object.last_updated|timesince }} ago
 {% endblock %} {% block tabs %}
     * {# Primary tab #}
     * _R_e_o_r_d_e_r_ _R_a_c_k
 {% endblock tabs %} {% block content-wrapper %}
 {% block content %}
 Save
```

### Comparing `netbox_reorder_rack-1.0.0/netbox_reorder_rack/templatetags/rack.py` & `netbox_reorder_rack-1.1.0/netbox_reorder_rack/templatetags/rack.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,10 @@
+from dcim.svg.racks import get_device_name
 from django import template
-from utilities.utils import foreground_color
+from utilities.html import foreground_color
 
 register = template.Library()
 
 
 @register.filter()
 def rack_unit(value):
     if value % 1 == 0:
@@ -36,7 +37,12 @@
 def mul(value, mul_value):
     return int(value) * mul_value
 
 
 @register.filter()
 def text_color(value):
     return foreground_color(value)
+
+
+@register.filter()
+def device_name(device):
+    return get_device_name(device)
```

### Comparing `netbox_reorder_rack-1.0.0/netbox_reorder_rack/tests/test_api.py` & `netbox_reorder_rack-1.1.0/netbox_reorder_rack/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `netbox_reorder_rack-1.0.0/netbox_reorder_rack/tests/test_view.py` & `netbox_reorder_rack-1.1.0/netbox_reorder_rack/tests/test_view.py`

 * *Files identical despite different names*

### Comparing `netbox_reorder_rack-1.0.0/netbox_reorder_rack/views.py` & `netbox_reorder_rack-1.1.0/netbox_reorder_rack/views.py`

 * *Files identical despite different names*

### Comparing `netbox_reorder_rack-1.0.0/netbox_reorder_rack.egg-info/PKG-INFO` & `netbox_reorder_rack-1.1.0/netbox_reorder_rack.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: netbox_reorder_rack
-Version: 1.0.0
+Version: 1.1.0
 Summary: NetBox plugin to reorder rack layouts.
 Home-page: https://github.com/minitriga/netbox-reorder-rack/
 Author: Alex Gittings
 Author-email: agitting96@gmail.com
 Project-URL: Bug Tracker, https://github.com/minitriga/netbox-reorder-rack/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Framework :: Django
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # Netbox Reorder Rack Plugin
 
 ![Version](https://img.shields.io/pypi/v/netbox-reorder-rack) ![Downloads](https://img.shields.io/pypi/dm/netbox-reorder-rack)
 
 Allow the ability to reorder rack units in NetBox using a drag and drop interface.
 
@@ -53,15 +54,16 @@
 ```
 
 
 ## Compatibility Matrix
 
 | netbox version | plugin version |
 | -------------- | ----------------------------- |
-| >= 3.7.0       | >= v1.0.0                     |
+| >= 4.0.0       | >= v1.1.0                     |
+| <= 4.0.0       | = v1.0.0                     |
 
 ### Update
 
 To update the plugin, you need to update the package and restart NetBox.
 
 ```shell
 source /opt/netbox/venv/bin/activate
```

### Comparing `netbox_reorder_rack-1.0.0/netbox_reorder_rack.egg-info/SOURCES.txt` & `netbox_reorder_rack-1.1.0/netbox_reorder_rack.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 MANIFEST.in
 README.md
 setup.py
 netbox_reorder_rack/__init__.py
 netbox_reorder_rack/template_content.py
 netbox_reorder_rack/urls.py
 netbox_reorder_rack/views.py
```

### Comparing `netbox_reorder_rack-1.0.0/setup.py` & `netbox_reorder_rack-1.1.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="netbox_reorder_rack",
-    version="1.0.0",
+    version="1.1.0",
     author="Alex Gittings",
     author_email="agitting96@gmail.com",
     description="NetBox plugin to reorder rack layouts.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=[],
     url="https://github.com/minitriga/netbox-reorder-rack/",
```

