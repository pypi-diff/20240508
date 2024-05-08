# Comparing `tmp/r_shepard-0.1.6.tar.gz` & `tmp/r_shepard-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "r_shepard-0.1.6.tar", max compression
+gzip compressed data, was "r_shepard-0.1.7.tar", max compression
```

## Comparing `r_shepard-0.1.6.tar` & `r_shepard-0.1.7.tar`

### file list

```diff
@@ -1,58 +1,60 @@
--rw-r--r--   0        0        0     3517 2024-05-07 13:27:13.812834 r_shepard-0.1.6/README.md
--rwxr-xr-x   0        0        0      666 2024-05-01 08:42:22.525077 r_shepard-0.1.6/manage.py
--rw-r--r--   0        0        0      783 2024-05-07 13:47:17.674811 r_shepard-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      174 2024-05-06 20:18:43.831721 r_shepard-0.1.6/r_shepard/__init__.py
--rw-r--r--   0        0        0       52 2024-05-06 21:14:06.784472 r_shepard-0.1.6/r_shepard/api/__init__.py
--rw-r--r--   0        0        0     3231 2024-05-07 10:03:25.055844 r_shepard-0.1.6/r_shepard/api/admin.py
--rw-r--r--   0        0        0      457 2024-05-07 10:02:03.501832 r_shepard-0.1.6/r_shepard/api/apps.py
--rw-r--r--   0        0        0      179 2024-05-06 21:14:06.784472 r_shepard-0.1.6/r_shepard/api/appy.py
--rw-r--r--   0        0        0     1137 2024-05-07 10:01:34.041125 r_shepard-0.1.6/r_shepard/api/migrations/0001_initial.py
--rw-r--r--   0        0        0      442 2024-05-07 10:01:34.041125 r_shepard-0.1.6/r_shepard/api/migrations/0002_project_is_active.py
--rw-r--r--   0        0        0      505 2024-05-07 10:01:34.041125 r_shepard-0.1.6/r_shepard/api/migrations/0003_project_url.py
--rw-r--r--   0        0        0      460 2024-05-07 10:01:34.041125 r_shepard-0.1.6/r_shepard/api/migrations/0004_project_rstudio_version.py
--rw-r--r--   0        0        0     1103 2024-05-07 10:01:34.042125 r_shepard-0.1.6/r_shepard/api/migrations/0005_remove_project_url_project_local_url_and_more.py
--rw-r--r--   0        0        0     3210 2024-05-07 10:01:34.042125 r_shepard-0.1.6/r_shepard/api/migrations/0006_remove_project_cpus_remove_project_is_active_and_more.py
--rw-r--r--   0        0        0      491 2024-05-07 10:01:34.043125 r_shepard-0.1.6/r_shepard/api/migrations/0007_alter_container_container_id.py
--rw-r--r--   0        0        0     1688 2024-04-22 08:54:16.989356 r_shepard-0.1.6/r_shepard/api/migrations/0008_container_port_alter_container_container_id_and_more.py
--rw-r--r--   0        0        0      506 2024-05-07 10:01:34.043125 r_shepard-0.1.6/r_shepard/api/migrations/0009_alter_container_port.py
--rw-r--r--   0        0        0      479 2024-05-07 10:01:34.043125 r_shepard-0.1.6/r_shepard/api/migrations/0010_alter_container_port.py
--rw-r--r--   0        0        0      518 2024-05-07 10:01:34.043125 r_shepard-0.1.6/r_shepard/api/migrations/0011_alter_container_tailscale_serve_url.py
--rw-r--r--   0        0        0      586 2024-04-23 09:28:07.929488 r_shepard-0.1.6/r_shepard/api/migrations/0012_project_slug.py
--rw-r--r--   0        0        0      656 2024-04-23 11:30:47.550693 r_shepard-0.1.6/r_shepard/api/migrations/0013_remove_project_password_container_password.py
--rw-r--r--   0        0        0      541 2024-04-24 10:26:22.152733 r_shepard-0.1.6/r_shepard/api/migrations/0014_project_max_containers.py
--rw-r--r--   0        0        0      918 2024-04-24 13:21:19.864083 r_shepard-0.1.6/r_shepard/api/migrations/0015_project_auto_commit_enabled_project_git_repo_url.py
--rw-r--r--   0        0        0     1381 2024-04-24 13:32:06.450029 r_shepard-0.1.6/r_shepard/api/migrations/0016_project_commit_interval_project_last_commit_time_and_more.py
--rw-r--r--   0        0        0        0 2024-04-20 15:09:46.014593 r_shepard-0.1.6/r_shepard/api/migrations/__init__.py
--rw-r--r--   0        0        0     5512 2024-05-07 10:02:03.501832 r_shepard-0.1.6/r_shepard/api/models.py
--rw-r--r--   0        0        0     4346 2024-05-07 10:04:34.289600 r_shepard-0.1.6/r_shepard/api/podman.py
--rw-r--r--   0        0        0     3104 2024-05-07 09:58:12.404696 r_shepard-0.1.6/r_shepard/api/static/custom.css
--rw-r--r--   0        0        0    48101 2024-04-22 17:57:33.717054 r_shepard-0.1.6/r_shepard/api/static/htmx.min.js
--rw-r--r--   0        0        0    82210 2024-04-22 16:54:30.950446 r_shepard-0.1.6/r_shepard/api/static/pico.blue.min.css
--rw-r--r--   0        0        0    74999 2024-04-23 06:39:38.438525 r_shepard-0.1.6/r_shepard/api/static/pico.colors.min.css
--rw-r--r--   0        0        0     2982 2024-04-23 09:15:45.253107 r_shepard-0.1.6/r_shepard/api/tailscale.py
--rw-r--r--   0        0        0     1397 2024-04-25 07:52:49.580151 r_shepard-0.1.6/r_shepard/api/tasks.py
--rw-r--r--   0        0        0     5807 2024-05-07 10:02:03.502833 r_shepard-0.1.6/r_shepard/api/views.py
--rw-r--r--   0        0        0      395 2024-04-26 07:51:03.905968 r_shepard-0.1.6/r_shepard/asgi.py
--rw-r--r--   0        0        0      226 2024-04-26 08:04:10.741465 r_shepard-0.1.6/r_shepard/celery.py
--rw-r--r--   0        0        0     4324 2024-05-07 13:36:39.120077 r_shepard-0.1.6/r_shepard/settings.py
--rw-r--r--   0        0        0     1983 2024-04-26 08:33:25.063331 r_shepard-0.1.6/r_shepard/tests/test_models.py
--rw-r--r--   0        0        0     1549 2024-04-30 14:46:22.169959 r_shepard-0.1.6/r_shepard/tests/test_views.py
--rw-r--r--   0        0        0     2275 2024-04-30 14:28:56.240315 r_shepard-0.1.6/r_shepard/tests/utils.py
--rw-r--r--   0        0        0     2527 2024-04-23 09:40:06.216686 r_shepard-0.1.6/r_shepard/urls.py
--rw-r--r--   0        0        0      395 2024-04-22 08:53:11.183304 r_shepard-0.1.6/r_shepard/wsgi.py
--rw-r--r--   0        0        0      356 2024-04-23 06:43:01.074990 r_shepard-0.1.6/templates/admin/base.html
--rw-r--r--   0        0        0      739 2024-04-23 16:45:21.318848 r_shepard-0.1.6/templates/base.html
--rw-r--r--   0        0        0     4087 2024-05-07 10:02:03.210825 r_shepard-0.1.6/templates/container_list.html
--rw-r--r--   0        0        0     2535 2024-05-07 10:00:50.352098 r_shepard-0.1.6/templates/project_detail.html
--rw-r--r--   0        0        0      795 2024-05-06 20:56:17.747817 r_shepard-0.1.6/templates/project_list.html
--rw-r--r--   0        0        0      234 2024-04-22 17:10:53.021583 r_shepard-0.1.6/templates/two_factor/_base_focus.html
--rw-r--r--   0        0        0      500 2024-04-22 16:49:01.953028 r_shepard-0.1.6/templates/two_factor/_wizard_actions.html
--rw-r--r--   0        0        0       90 2024-04-22 16:29:08.847147 r_shepard-0.1.6/templates/two_factor/_wizard_forms.html
--rw-r--r--   0        0        0     1145 2024-04-22 16:29:08.812144 r_shepard-0.1.6/templates/two_factor/core/backup_tokens.html
--rw-r--r--   0        0        0     2008 2024-04-22 16:48:40.642014 r_shepard-0.1.6/templates/two_factor/core/login.html
--rw-r--r--   0        0        0      833 2024-04-22 16:29:08.813144 r_shepard-0.1.6/templates/two_factor/core/otp_required.html
--rw-r--r--   0        0        0     3149 2024-04-22 16:29:08.813144 r_shepard-0.1.6/templates/two_factor/core/setup.html
--rw-r--r--   0        0        0      963 2024-04-22 16:29:08.814144 r_shepard-0.1.6/templates/two_factor/core/setup_complete.html
--rw-r--r--   0        0        0      529 2024-04-22 16:29:08.801143 r_shepard-0.1.6/templates/two_factor/profile/disable.html
--rw-r--r--   0        0        0     2527 2024-04-23 08:51:59.180319 r_shepard-0.1.6/templates/two_factor/profile/profile.html
--rw-r--r--   0        0        0     4343 1970-01-01 00:00:00.000000 r_shepard-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     3517 2024-05-07 13:27:13.812834 r_shepard-0.1.7/README.md
+-rwxr-xr-x   0        0        0      666 2024-05-01 08:42:22.525077 r_shepard-0.1.7/manage.py
+-rw-r--r--   0        0        0      807 2024-05-08 13:57:17.540269 r_shepard-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      174 2024-05-06 20:18:43.831721 r_shepard-0.1.7/r_shepard/__init__.py
+-rw-r--r--   0        0        0       52 2024-05-06 21:14:06.784472 r_shepard-0.1.7/r_shepard/api/__init__.py
+-rw-r--r--   0        0        0     3793 2024-05-08 13:45:19.864296 r_shepard-0.1.7/r_shepard/api/admin.py
+-rw-r--r--   0        0        0      457 2024-05-07 10:02:03.501832 r_shepard-0.1.7/r_shepard/api/apps.py
+-rw-r--r--   0        0        0      179 2024-05-06 21:14:06.784472 r_shepard-0.1.7/r_shepard/api/appy.py
+-rw-r--r--   0        0        0     1137 2024-05-07 10:01:34.041125 r_shepard-0.1.7/r_shepard/api/migrations/0001_initial.py
+-rw-r--r--   0        0        0      442 2024-05-07 10:01:34.041125 r_shepard-0.1.7/r_shepard/api/migrations/0002_project_is_active.py
+-rw-r--r--   0        0        0      505 2024-05-07 10:01:34.041125 r_shepard-0.1.7/r_shepard/api/migrations/0003_project_url.py
+-rw-r--r--   0        0        0      460 2024-05-07 10:01:34.041125 r_shepard-0.1.7/r_shepard/api/migrations/0004_project_rstudio_version.py
+-rw-r--r--   0        0        0     1103 2024-05-07 10:01:34.042125 r_shepard-0.1.7/r_shepard/api/migrations/0005_remove_project_url_project_local_url_and_more.py
+-rw-r--r--   0        0        0     3210 2024-05-07 10:01:34.042125 r_shepard-0.1.7/r_shepard/api/migrations/0006_remove_project_cpus_remove_project_is_active_and_more.py
+-rw-r--r--   0        0        0      491 2024-05-07 10:01:34.043125 r_shepard-0.1.7/r_shepard/api/migrations/0007_alter_container_container_id.py
+-rw-r--r--   0        0        0     1688 2024-04-22 08:54:16.989356 r_shepard-0.1.7/r_shepard/api/migrations/0008_container_port_alter_container_container_id_and_more.py
+-rw-r--r--   0        0        0      506 2024-05-07 10:01:34.043125 r_shepard-0.1.7/r_shepard/api/migrations/0009_alter_container_port.py
+-rw-r--r--   0        0        0      479 2024-05-07 10:01:34.043125 r_shepard-0.1.7/r_shepard/api/migrations/0010_alter_container_port.py
+-rw-r--r--   0        0        0      518 2024-05-07 10:01:34.043125 r_shepard-0.1.7/r_shepard/api/migrations/0011_alter_container_tailscale_serve_url.py
+-rw-r--r--   0        0        0      586 2024-04-23 09:28:07.929488 r_shepard-0.1.7/r_shepard/api/migrations/0012_project_slug.py
+-rw-r--r--   0        0        0      656 2024-04-23 11:30:47.550693 r_shepard-0.1.7/r_shepard/api/migrations/0013_remove_project_password_container_password.py
+-rw-r--r--   0        0        0      541 2024-04-24 10:26:22.152733 r_shepard-0.1.7/r_shepard/api/migrations/0014_project_max_containers.py
+-rw-r--r--   0        0        0      918 2024-04-24 13:21:19.864083 r_shepard-0.1.7/r_shepard/api/migrations/0015_project_auto_commit_enabled_project_git_repo_url.py
+-rw-r--r--   0        0        0     1381 2024-04-24 13:32:06.450029 r_shepard-0.1.7/r_shepard/api/migrations/0016_project_commit_interval_project_last_commit_time_and_more.py
+-rw-r--r--   0        0        0     3177 2024-05-08 12:34:05.383598 r_shepard-0.1.7/r_shepard/api/migrations/0017_alter_container_container_id_alter_container_cpus_and_more.py
+-rw-r--r--   0        0        0      512 2024-05-08 13:12:31.128211 r_shepard-0.1.7/r_shepard/api/migrations/0018_project_description.py
+-rw-r--r--   0        0        0        0 2024-04-20 15:09:46.014593 r_shepard-0.1.7/r_shepard/api/migrations/__init__.py
+-rw-r--r--   0        0        0     5679 2024-05-08 13:12:27.806227 r_shepard-0.1.7/r_shepard/api/models.py
+-rw-r--r--   0        0        0     4346 2024-05-07 10:04:34.289600 r_shepard-0.1.7/r_shepard/api/podman.py
+-rw-r--r--   0        0        0     3104 2024-05-08 13:55:02.555158 r_shepard-0.1.7/r_shepard/api/static/custom.css
+-rw-r--r--   0        0        0    48101 2024-04-22 17:57:33.717054 r_shepard-0.1.7/r_shepard/api/static/htmx.min.js
+-rw-r--r--   0        0        0    82210 2024-04-22 16:54:30.950446 r_shepard-0.1.7/r_shepard/api/static/pico.blue.min.css
+-rw-r--r--   0        0        0    74999 2024-04-23 06:39:38.438525 r_shepard-0.1.7/r_shepard/api/static/pico.colors.min.css
+-rw-r--r--   0        0        0     2982 2024-04-23 09:15:45.253107 r_shepard-0.1.7/r_shepard/api/tailscale.py
+-rw-r--r--   0        0        0     1397 2024-04-25 07:52:49.580151 r_shepard-0.1.7/r_shepard/api/tasks.py
+-rw-r--r--   0        0        0     5807 2024-05-07 10:02:03.502833 r_shepard-0.1.7/r_shepard/api/views.py
+-rw-r--r--   0        0        0      395 2024-04-26 07:51:03.905968 r_shepard-0.1.7/r_shepard/asgi.py
+-rw-r--r--   0        0        0      226 2024-04-26 08:04:10.741465 r_shepard-0.1.7/r_shepard/celery.py
+-rw-r--r--   0        0        0     4390 2024-05-08 12:35:02.019115 r_shepard-0.1.7/r_shepard/settings.py
+-rw-r--r--   0        0        0     1983 2024-04-26 08:33:25.063331 r_shepard-0.1.7/r_shepard/tests/test_models.py
+-rw-r--r--   0        0        0     1549 2024-04-30 14:46:22.169959 r_shepard-0.1.7/r_shepard/tests/test_views.py
+-rw-r--r--   0        0        0     2275 2024-04-30 14:28:56.240315 r_shepard-0.1.7/r_shepard/tests/utils.py
+-rw-r--r--   0        0        0     2527 2024-04-23 09:40:06.216686 r_shepard-0.1.7/r_shepard/urls.py
+-rw-r--r--   0        0        0      395 2024-04-22 08:53:11.183304 r_shepard-0.1.7/r_shepard/wsgi.py
+-rw-r--r--   0        0        0      356 2024-04-23 06:43:01.074990 r_shepard-0.1.7/templates/admin/base.html
+-rw-r--r--   0        0        0      739 2024-04-23 16:45:21.318848 r_shepard-0.1.7/templates/base.html
+-rw-r--r--   0        0        0     4152 2024-05-08 13:25:20.796846 r_shepard-0.1.7/templates/container_list.html
+-rw-r--r--   0        0        0     2590 2024-05-08 13:56:15.535676 r_shepard-0.1.7/templates/project_detail.html
+-rw-r--r--   0        0        0     1150 2024-05-08 13:20:01.025476 r_shepard-0.1.7/templates/project_list.html
+-rw-r--r--   0        0        0      234 2024-04-22 17:10:53.021583 r_shepard-0.1.7/templates/two_factor/_base_focus.html
+-rw-r--r--   0        0        0      500 2024-04-22 16:49:01.953028 r_shepard-0.1.7/templates/two_factor/_wizard_actions.html
+-rw-r--r--   0        0        0       90 2024-04-22 16:29:08.847147 r_shepard-0.1.7/templates/two_factor/_wizard_forms.html
+-rw-r--r--   0        0        0     1145 2024-04-22 16:29:08.812144 r_shepard-0.1.7/templates/two_factor/core/backup_tokens.html
+-rw-r--r--   0        0        0     2008 2024-04-22 16:48:40.642014 r_shepard-0.1.7/templates/two_factor/core/login.html
+-rw-r--r--   0        0        0      833 2024-04-22 16:29:08.813144 r_shepard-0.1.7/templates/two_factor/core/otp_required.html
+-rw-r--r--   0        0        0     3149 2024-04-22 16:29:08.813144 r_shepard-0.1.7/templates/two_factor/core/setup.html
+-rw-r--r--   0        0        0      963 2024-04-22 16:29:08.814144 r_shepard-0.1.7/templates/two_factor/core/setup_complete.html
+-rw-r--r--   0        0        0      529 2024-04-22 16:29:08.801143 r_shepard-0.1.7/templates/two_factor/profile/disable.html
+-rw-r--r--   0        0        0     2527 2024-04-23 08:51:59.180319 r_shepard-0.1.7/templates/two_factor/profile/profile.html
+-rw-r--r--   0        0        0     4400 1970-01-01 00:00:00.000000 r_shepard-0.1.7/PKG-INFO
```

### Comparing `r_shepard-0.1.6/README.md` & `r_shepard-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `r_shepard-0.1.6/manage.py` & `r_shepard-0.1.7/manage.py`

 * *Files identical despite different names*

### Comparing `r_shepard-0.1.6/pyproject.toml` & `r_shepard-0.1.7/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 [tool.poetry]
-packages = [
-    { include = "r_shepard", from = "." },
-    { include = "manage.py" },
-]
+packages = [{ include = "r_shepard", from = "." }, { include = "manage.py" }]
 name = "r-shepard"
-version = "0.1.6"
+version = "0.1.7"
 description = ""
 authors = ["linozen <linus@sehn.dev>"]
 license = "GPL-3.0"
 readme = "README.md"
 include = ["templates/*"]
 
 [tool.poetry.dependencies]
@@ -17,14 +14,15 @@
 podman = "^5.0.0"
 django-two-factor-auth = "^1.16.0"
 django-otp-yubikey = "^1.1.0"
 phonenumberslite = "^8.13.35"
 celery = "^5.4.0"
 redis = "^5.0.4"
 daphne = "^4.1.2"
+django-admin-interface = "^0.28.6"
 
 [tool.poetry.scripts]
 r-shepard = "manage:main"
 
 [tool.poetry.group.dev.dependencies]
 djlint = "^1.34.1"
 bumpversion = "^0.6.0"
```

### Comparing `r_shepard-0.1.6/r_shepard/api/admin.py` & `r_shepard-0.1.7/r_shepard/api/admin.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 from typing import Any
 
 from django import forms
 from django.contrib import admin, messages
-from django.http import HttpResponseRedirect
+from django.http import HttpRequest, HttpResponseRedirect
+from django.http.response import HttpResponse
 from django.urls import reverse
 
 from .models import Container, Project
 from .podman import PodmanError, start_container
 
 admin.site.site_header = "R-Shepard"
 admin.site.site_title = "R-Shepard"
 admin.site.index_title = "Admin Area"
 
 
-admin.site.register(Project)
-
-
 class EditContainerForm(forms.ModelForm):
     class Meta:
         model = Container
         fields = "__all__"
         # These fields cannot be edited and are excluded from the edit form
         exclude = [
             "project",
@@ -94,9 +92,21 @@
             return
         super().save_model(request, obj, form, change)
 
     # Redirect to project detail page after adding a container
     def response_add(self, request, obj, post_url_continue=None):
         return HttpResponseRedirect(reverse("project_detail", args=[obj.project.pk]))
 
+    def response_change(self, request: HttpRequest, obj: Any) -> HttpResponse:
+        return HttpResponseRedirect(reverse("project_detail", args=[obj.project.pk]))
+
+
+class ProjectAdmin(admin.ModelAdmin):
+    def response_add(self, request, obj, post_url_continue=None):
+        return HttpResponseRedirect(reverse("project_list"))
+
+    def response_change(self, request: HttpRequest, obj: Any) -> HttpResponse:
+        return HttpResponseRedirect(reverse("project_detail", args=[obj.pk]))
+
 
 admin.site.register(Container, ContainerAdmin)
+admin.site.register(Project, ProjectAdmin)
```

### Comparing `r_shepard-0.1.6/r_shepard/api/migrations/0001_initial.py` & `r_shepard-0.1.7/r_shepard/api/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `r_shepard-0.1.6/r_shepard/api/migrations/0005_remove_project_url_project_local_url_and_more.py` & `r_shepard-0.1.7/r_shepard/api/migrations/0005_remove_project_url_project_local_url_and_more.py`

 * *Files identical despite different names*

### Comparing `r_shepard-0.1.6/r_shepard/api/migrations/0006_remove_project_cpus_remove_project_is_active_and_more.py` & `r_shepard-0.1.7/r_shepard/api/migrations/0006_remove_project_cpus_remove_project_is_active_and_more.py`

 * *Files identical despite different names*

### Comparing `r_shepard-0.1.6/r_shepard/api/migrations/0008_container_port_alter_container_container_id_and_more.py` & `r_shepard-0.1.7/r_shepard/api/migrations/0008_container_port_alter_container_container_id_and_more.py`

 * *Files identical despite different names*

### Comparing `r_shepard-0.1.6/r_shepard/api/migrations/0011_alter_container_tailscale_serve_url.py` & `r_shepard-0.1.7/r_shepard/api/migrations/0011_alter_container_tailscale_serve_url.py`

 * *Files identical despite different names*

### Comparing `r_shepard-0.1.6/r_shepard/api/migrations/0012_project_slug.py` & `r_shepard-0.1.7/r_shepard/api/migrations/0012_project_slug.py`

 * *Files identical despite different names*

### Comparing `r_shepard-0.1.6/r_shepard/api/migrations/0013_remove_project_password_container_password.py` & `r_shepard-0.1.7/r_shepard/api/migrations/0013_remove_project_password_container_password.py`

 * *Files identical despite different names*

### Comparing `r_shepard-0.1.6/r_shepard/api/migrations/0014_project_max_containers.py` & `r_shepard-0.1.7/r_shepard/api/migrations/0014_project_max_containers.py`

 * *Files identical despite different names*

### Comparing `r_shepard-0.1.6/r_shepard/api/migrations/0015_project_auto_commit_enabled_project_git_repo_url.py` & `r_shepard-0.1.7/r_shepard/api/migrations/0015_project_auto_commit_enabled_project_git_repo_url.py`

 * *Files identical despite different names*

### Comparing `r_shepard-0.1.6/r_shepard/api/migrations/0016_project_commit_interval_project_last_commit_time_and_more.py` & `r_shepard-0.1.7/r_shepard/api/migrations/0016_project_commit_interval_project_last_commit_time_and_more.py`

 * *Files identical despite different names*

### Comparing `r_shepard-0.1.6/r_shepard/api/models.py` & `r_shepard-0.1.7/r_shepard/api/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,19 @@
 
 class Project(models.Model):
     name = models.CharField(
         max_length=255,
         unique=True,
         help_text="The name of the project.",
     )
+    description = models.CharField(
+        default="",
+        max_length=1024,
+        help_text="A short description of your project (max. 1025 characters)",
+    )
     slug = models.SlugField(
         max_length=255,
         unique=True,
         help_text="A URL-safe slug for the project.",
     )
     data_path = models.CharField(
         max_length=1024,
```

### Comparing `r_shepard-0.1.6/r_shepard/api/podman.py` & `r_shepard-0.1.7/r_shepard/api/podman.py`

 * *Files identical despite different names*

### Comparing `r_shepard-0.1.6/r_shepard/api/static/custom.css` & `r_shepard-0.1.7/r_shepard/api/static/custom.css`

 * *Files 6% similar despite different names*

```diff
@@ -11,18 +11,24 @@
 
 .header-line {
   display: inline-block;
   margin-bottom: 20px;
 }
 
 .header-line h1,
-h2 {
+h2,
+h3,
+h4 {
   display: inline;
 }
 
+.header-line h4 {
+  line-height: 1.7;
+}
+
 .header-line a {
   float: right;
   margin-left: 10px;
 }
 
 button {
   --pico-font-weight: 700;
@@ -49,46 +55,46 @@
   background-color: #f44336; /* Red */
   border: none;
   border-radius: 4px;
   margin: 10px 0;
   padding: 10px;
 }
 
-.project-info {
-  margin-right: 5px;
-}
-
 .action-button {
   display: flex;
   justify-content: center;
   align-items: center;
 }
 
-.container-list {
+.container-list,
+.project-list {
   display: flex;
   flex-wrap: wrap;
   justify-content: start;
+  gap: 10px;
 }
 
-.container-card {
+.container-card,
+.project-card {
   width: 100%;
 }
 
 @media (min-width: 600px) {
-  .container-card {
-    width: calc(50% - 20px); /* Adjust for desired gap */
-    margin: 10px; /* Half of the gap */
+  .container-card,
+  .project-card {
+    width: calc(50% - 10px); /* Adjust for desired gap */
+    /* margin: 10px; */
     box-sizing: border-box;
   }
 }
 
 @media (min-width: 900px) {
-  .container-card {
-    width: calc(33.33% - 20px); /* Adjust for desired gap */
-    margin: 10px; /* Half of the gap */
+  .container-card,
+  .project-card {
+    width: calc(33.5% - 10px);
     box-sizing: border-box;
   }
 }
 
 .container-title {
   font-size: 20px;
   margin-top: 4px;
```

### Comparing `r_shepard-0.1.6/r_shepard/api/static/htmx.min.js` & `r_shepard-0.1.7/r_shepard/api/static/htmx.min.js`

 * *Files identical despite different names*

### Comparing `r_shepard-0.1.6/r_shepard/api/static/pico.blue.min.css` & `r_shepard-0.1.7/r_shepard/api/static/pico.blue.min.css`

 * *Files identical despite different names*

### Comparing `r_shepard-0.1.6/r_shepard/api/static/pico.colors.min.css` & `r_shepard-0.1.7/r_shepard/api/static/pico.colors.min.css`

 * *Files identical despite different names*

### Comparing `r_shepard-0.1.6/r_shepard/api/tailscale.py` & `r_shepard-0.1.7/r_shepard/api/tailscale.py`

 * *Files identical despite different names*

### Comparing `r_shepard-0.1.6/r_shepard/api/tasks.py` & `r_shepard-0.1.7/r_shepard/api/tasks.py`

 * *Files identical despite different names*

### Comparing `r_shepard-0.1.6/r_shepard/api/views.py` & `r_shepard-0.1.7/r_shepard/api/views.py`

 * *Files identical despite different names*

### Comparing `r_shepard-0.1.6/r_shepard/settings.py` & `r_shepard-0.1.7/r_shepard/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,25 +22,27 @@
 
 # SECURITY WARNING: keep the secret key used in production secret!
 SECRET_KEY = "django-insecure-yc+#%@i2_hyrl1ut+c-9#ejwrv6(cv2de=-2+dv375a+oal*n7"
 
 # SECURITY WARNING: don't run with debug turned on in production!
 DEBUG = True
 
-ALLOWED_HOSTS = os.getenv("ALLOWED_HOSTS", "").split(",")
-CSRF_TRUSTED_ORIGINS = os.getenv("CSRF_TRUSTED_ORIGINS", "").split(",")
+ALLOWED_HOSTS = os.getenv("ALLOWED_HOSTS", "127.0.0.1").split(",")
+CSRF_TRUSTED_ORIGINS = os.getenv("CSRF_TRUSTED_ORIGINS", "http://127.0.0.1").split(",")
 
 LOGIN_URL = "two_factor:login"
 
 # this one is optional
 LOGIN_REDIRECT_URL = "two_factor:profile"
 
 # Application definition
 INSTALLED_APPS = [
     "r_shepard.api",
+    "admin_interface",
+    "colorfield",
     "django.contrib.admin",
     "django.contrib.auth",
     "django.contrib.contenttypes",
     "django.contrib.sessions",
     "django.contrib.messages",
     "django.contrib.staticfiles",
     "django_otp",
```

### Comparing `r_shepard-0.1.6/r_shepard/tests/test_models.py` & `r_shepard-0.1.7/r_shepard/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `r_shepard-0.1.6/r_shepard/tests/test_views.py` & `r_shepard-0.1.7/r_shepard/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `r_shepard-0.1.6/r_shepard/tests/utils.py` & `r_shepard-0.1.7/r_shepard/tests/utils.py`

 * *Files identical despite different names*

### Comparing `r_shepard-0.1.6/r_shepard/urls.py` & `r_shepard-0.1.7/r_shepard/urls.py`

 * *Files identical despite different names*

### Comparing `r_shepard-0.1.6/templates/base.html` & `r_shepard-0.1.7/templates/base.html`

 * *Files identical despite different names*

### Comparing `r_shepard-0.1.6/templates/container_list.html` & `r_shepard-0.1.7/templates/container_list.html`

 * *Files 4% similar despite different names*

```diff
@@ -88,9 +88,11 @@
               class="action-button delete-button"
               type="submit">
         <span class="button-content">Delete</span>
         <span id="loading-delete-{{ container.pk }}"
               class="htmx-indicator lds-dual-ring"></span>
       </button>
     </article>
+  {% empty %}
+    <p>No containers have been created yet...</p>
   {% endfor %}
-</div>
+</div>
```

### Comparing `r_shepard-0.1.6/templates/two_factor/core/backup_tokens.html` & `r_shepard-0.1.7/templates/two_factor/core/backup_tokens.html`

 * *Files identical despite different names*

### Comparing `r_shepard-0.1.6/templates/two_factor/core/login.html` & `r_shepard-0.1.7/templates/two_factor/core/login.html`

 * *Files identical despite different names*

### Comparing `r_shepard-0.1.6/templates/two_factor/core/otp_required.html` & `r_shepard-0.1.7/templates/two_factor/core/otp_required.html`

 * *Files identical despite different names*

### Comparing `r_shepard-0.1.6/templates/two_factor/core/setup.html` & `r_shepard-0.1.7/templates/two_factor/core/setup.html`

 * *Files identical despite different names*

### Comparing `r_shepard-0.1.6/templates/two_factor/core/setup_complete.html` & `r_shepard-0.1.7/templates/two_factor/core/setup_complete.html`

 * *Files identical despite different names*

### Comparing `r_shepard-0.1.6/templates/two_factor/profile/disable.html` & `r_shepard-0.1.7/templates/two_factor/profile/disable.html`

 * *Files identical despite different names*

### Comparing `r_shepard-0.1.6/templates/two_factor/profile/profile.html` & `r_shepard-0.1.7/templates/two_factor/profile/profile.html`

 * *Files identical despite different names*

### Comparing `r_shepard-0.1.6/PKG-INFO` & `r_shepard-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: r-shepard
-Version: 0.1.6
+Version: 0.1.7
 Summary: 
 License: GPL-3.0
 Author: linozen
 Author-email: linus@sehn.dev
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: celery (>=5.4.0,<6.0.0)
 Requires-Dist: daphne (>=4.1.2,<5.0.0)
 Requires-Dist: django (>=5.0.4,<6.0.0)
+Requires-Dist: django-admin-interface (>=0.28.6,<0.29.0)
 Requires-Dist: django-otp-yubikey (>=1.1.0,<2.0.0)
 Requires-Dist: django-two-factor-auth (>=1.16.0,<2.0.0)
 Requires-Dist: phonenumberslite (>=8.13.35,<9.0.0)
 Requires-Dist: podman (>=5.0.0,<6.0.0)
 Requires-Dist: redis (>=5.0.4,<6.0.0)
 Description-Content-Type: text/markdown
```

