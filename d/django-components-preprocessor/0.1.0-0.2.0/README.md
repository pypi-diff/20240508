# Comparing `tmp/django_components_preprocessor-0.1.0.tar.gz` & `tmp/django_components_preprocessor-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_components_preprocessor-0.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "django_components_preprocessor-0.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `django_components_preprocessor-0.1.0.tar` & `django_components_preprocessor-0.2.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0       40 2024-02-11 21:09:45.619261 django_components_preprocessor-0.1.0/.gitignore
--rw-r--r--   0        0        0     1078 2024-02-10 14:23:32.448117 django_components_preprocessor-0.1.0/LICENSE
--rw-r--r--   0        0        0     2540 2024-02-11 21:26:22.148717 django_components_preprocessor-0.1.0/README.md
--rw-r--r--   0        0        0      269 2024-02-11 21:08:50.363687 django_components_preprocessor-0.1.0/django_components_preprocessor/__init__.py
--rw-r--r--   0        0        0     2131 2024-02-11 18:05:00.818449 django_components_preprocessor-0.1.0/django_components_preprocessor/loader.py
--rw-r--r--   0        0        0      234 2024-02-11 09:11:14.890960 django_components_preprocessor-0.1.0/example/components/calendar/calendar.html
--rw-r--r--   0        0        0      739 2024-02-10 17:52:35.364550 django_components_preprocessor-0.1.0/example/components/calendar/calendar.py
--rw-r--r--   0        0        0      220 2024-02-10 20:33:10.955395 django_components_preprocessor-0.1.0/example/components/calendar/script.js
--rw-r--r--   0        0        0      103 2024-02-10 16:19:08.060871 django_components_preprocessor-0.1.0/example/components/calendar/style.css
--rw-r--r--   0        0        0        0 2024-02-10 14:07:33.826613 django_components_preprocessor-0.1.0/example/core/__init__.py
--rw-r--r--   0        0        0       63 2024-02-10 14:07:33.826613 django_components_preprocessor-0.1.0/example/core/admin.py
--rw-r--r--   0        0        0      140 2024-02-10 14:07:33.946612 django_components_preprocessor-0.1.0/example/core/apps.py
--rw-r--r--   0        0        0        0 2024-02-10 14:07:33.830613 django_components_preprocessor-0.1.0/example/core/migrations/__init__.py
--rw-r--r--   0        0        0       57 2024-02-10 14:07:33.826613 django_components_preprocessor-0.1.0/example/core/models.py
--rw-r--r--   0        0        0      454 2024-02-11 21:10:07.219098 django_components_preprocessor-0.1.0/example/core/templates/core/index.html
--rw-r--r--   0        0        0       60 2024-02-10 14:07:33.826613 django_components_preprocessor-0.1.0/example/core/tests.py
--rw-r--r--   0        0        0      102 2024-02-10 14:37:40.763307 django_components_preprocessor-0.1.0/example/core/views.py
--rw-r--r--   0        0        0        0 2024-02-10 14:07:12.758895 django_components_preprocessor-0.1.0/example/example/__init__.py
--rw-r--r--   0        0        0      391 2024-02-10 14:07:12.890894 django_components_preprocessor-0.1.0/example/example/asgi.py
--rw-r--r--   0        0        0     3764 2024-02-11 21:20:58.938695 django_components_preprocessor-0.1.0/example/example/settings.py
--rw-r--r--   0        0        0      168 2024-02-10 14:38:21.451500 django_components_preprocessor-0.1.0/example/example/urls.py
--rw-r--r--   0        0        0      391 2024-02-10 14:07:12.890894 django_components_preprocessor-0.1.0/example/example/wsgi.py
--rwxr-xr-x   0        0        0      663 2024-02-10 14:07:12.894894 django_components_preprocessor-0.1.0/example/manage.py
--rw-r--r--   0        0        0      518 2024-02-10 23:38:07.688278 django_components_preprocessor-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      388 1970-01-01 00:00:00.000000 django_components_preprocessor-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       40 2024-02-11 21:09:45.619261 django_components_preprocessor-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1078 2024-02-10 14:23:32.448117 django_components_preprocessor-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2540 2024-02-11 21:26:22.148717 django_components_preprocessor-0.2.0/README.md
+-rw-r--r--   0        0        0      269 2024-05-08 09:06:54.345273 django_components_preprocessor-0.2.0/django_components_preprocessor/__init__.py
+-rw-r--r--   0        0        0     2139 2024-05-08 09:06:41.005371 django_components_preprocessor-0.2.0/django_components_preprocessor/loader.py
+-rw-r--r--   0        0        0      234 2024-02-11 09:11:14.890960 django_components_preprocessor-0.2.0/example/components/calendar/calendar.html
+-rw-r--r--   0        0        0      739 2024-02-10 17:52:35.364550 django_components_preprocessor-0.2.0/example/components/calendar/calendar.py
+-rw-r--r--   0        0        0      220 2024-02-10 20:33:10.955395 django_components_preprocessor-0.2.0/example/components/calendar/script.js
+-rw-r--r--   0        0        0      103 2024-02-10 16:19:08.060871 django_components_preprocessor-0.2.0/example/components/calendar/style.css
+-rw-r--r--   0        0        0        0 2024-02-10 14:07:33.826613 django_components_preprocessor-0.2.0/example/core/__init__.py
+-rw-r--r--   0        0        0       63 2024-02-10 14:07:33.826613 django_components_preprocessor-0.2.0/example/core/admin.py
+-rw-r--r--   0        0        0      140 2024-02-10 14:07:33.946612 django_components_preprocessor-0.2.0/example/core/apps.py
+-rw-r--r--   0        0        0        0 2024-02-10 14:07:33.830613 django_components_preprocessor-0.2.0/example/core/migrations/__init__.py
+-rw-r--r--   0        0        0       57 2024-02-10 14:07:33.826613 django_components_preprocessor-0.2.0/example/core/models.py
+-rw-r--r--   0        0        0      454 2024-02-11 21:10:07.219098 django_components_preprocessor-0.2.0/example/core/templates/core/index.html
+-rw-r--r--   0        0        0       60 2024-02-10 14:07:33.826613 django_components_preprocessor-0.2.0/example/core/tests.py
+-rw-r--r--   0        0        0      102 2024-02-10 14:37:40.763307 django_components_preprocessor-0.2.0/example/core/views.py
+-rw-r--r--   0        0        0        0 2024-02-10 14:07:12.758895 django_components_preprocessor-0.2.0/example/example/__init__.py
+-rw-r--r--   0        0        0      391 2024-02-10 14:07:12.890894 django_components_preprocessor-0.2.0/example/example/asgi.py
+-rw-r--r--   0        0        0     3764 2024-02-11 21:20:58.938695 django_components_preprocessor-0.2.0/example/example/settings.py
+-rw-r--r--   0        0        0      168 2024-02-10 14:38:21.451500 django_components_preprocessor-0.2.0/example/example/urls.py
+-rw-r--r--   0        0        0      391 2024-02-10 14:07:12.890894 django_components_preprocessor-0.2.0/example/example/wsgi.py
+-rwxr-xr-x   0        0        0      663 2024-02-10 14:07:12.894894 django_components_preprocessor-0.2.0/example/manage.py
+-rw-r--r--   0        0        0      538 2024-05-08 09:06:21.917511 django_components_preprocessor-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2969 1970-01-01 00:00:00.000000 django_components_preprocessor-0.2.0/PKG-INFO
```

### Comparing `django_components_preprocessor-0.1.0/LICENSE` & `django_components_preprocessor-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_components_preprocessor-0.1.0/README.md` & `django_components_preprocessor-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `django_components_preprocessor-0.1.0/django_components_preprocessor/loader.py` & `django_components_preprocessor-0.2.0/django_components_preprocessor/loader.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,25 +22,25 @@
 
         super().__init__(engine)
 
     @staticmethod
     def replace_self_closing_tag(match):
         tag = match.group(1)
         args = match.group(2).replace("\n", " ")
-        return f'{{% component "{tag}"{args} %}}'
+        return f'{{% component "{tag}"{args} %}}{{% endcomponent %}}'
 
     @staticmethod
     def replace_opening_tag(match):
         tag = match.group(1)
         args = match.group(2).replace("\n", " ")
-        return f'{{% component_block "{tag}"{args} %}}'
+        return f'{{% component "{tag}"{args} %}}'
 
     @staticmethod
     def replace_closing_tag(match):
-        return "{% endcomponent_block %}"
+        return "{% endcomponent %}"
 
     def get_contents(self, origin):
         contents = self.loader_get_contents(origin)
 
         contents = self.self_closing_tag_re.sub(self.replace_self_closing_tag, contents)
         contents = self.opening_tag_re.sub(self.replace_opening_tag, contents)
         contents = self.closing_tag_re.sub(self.replace_closing_tag, contents)
```

### Comparing `django_components_preprocessor-0.1.0/example/components/calendar/calendar.py` & `django_components_preprocessor-0.2.0/example/components/calendar/calendar.py`

 * *Files identical despite different names*

### Comparing `django_components_preprocessor-0.1.0/example/example/settings.py` & `django_components_preprocessor-0.2.0/example/example/settings.py`

 * *Files identical despite different names*

### Comparing `django_components_preprocessor-0.1.0/example/manage.py` & `django_components_preprocessor-0.2.0/example/manage.py`

 * *Files identical despite different names*

### Comparing `django_components_preprocessor-0.1.0/pyproject.toml` & `django_components_preprocessor-0.2.0/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 [project]
 name = "django-components-preprocessor"
 authors = [{name = "Fabian Binz", email = "fabian.binz@gmail.com"}]
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: MIT License"]
 dynamic = ["version", "description"]
 dependencies = [
-  "django-components ~= 0.35",
+  "django-components >= 0.5",
 ]
+readme = "README.md"
 
 [project.urls]
 Home = "https://github.com/fbinz/django-components-preprocessor"
 
 [tool.flit.module]
 name = "django_components_preprocessor"
```

