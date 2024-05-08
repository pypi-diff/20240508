# Comparing `tmp/wagtail_fedit-1.5.4rc9.tar.gz` & `tmp/wagtail_fedit-1.5.5rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail_fedit-1.5.4rc9.tar", last modified: Tue Apr 23 20:50:48 2024, max compression
+gzip compressed data, was "wagtail_fedit-1.5.5rc1.tar", last modified: Wed May  8 11:33:58 2024, max compression
```

## Comparing `wagtail_fedit-1.5.4rc9.tar` & `wagtail_fedit-1.5.5rc1.tar`

### file list

```diff
@@ -1,137 +1,136 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 20:50:48.263680 wagtail_fedit-1.5.4rc9/
--rw-rw-rw-   0        0        0    18429 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.4rc9/LICENSE
--rw-rw-rw-   0        0        0      257 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.4rc9/MANIFEST.in
--rw-rw-rw-   0        0        0    21651 2024-04-23 20:50:48.263680 wagtail_fedit-1.5.4rc9/PKG-INFO
--rw-rw-rw-   0        0        0    20450 2024-04-23 11:23:03.000000 wagtail_fedit-1.5.4rc9/README.md
--rw-rw-rw-   0        0        0       90 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.4rc9/pyproject.toml
--rw-rw-rw-   0        0        0     1189 2024-04-23 20:50:48.274174 wagtail_fedit-1.5.4rc9/setup.cfg
--rw-rw-rw-   0        0        0       39 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.4rc9/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-23 20:50:48.075351 wagtail_fedit-1.5.4rc9/wagtail_fedit/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-23 20:50:48.126731 wagtail_fedit-1.5.4rc9/wagtail_fedit/adapters/
--rw-rw-rw-   0        0        0      532 2024-04-22 21:01:35.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/adapters/__init__.py
--rw-rw-rw-   0        0        0    14330 2024-04-23 15:34:38.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/adapters/base.py
--rw-rw-rw-   0        0        0     6524 2024-04-23 20:05:52.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/adapters/block.py
--rw-rw-rw-   0        0        0     8652 2024-04-23 18:12:26.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/adapters/field.py
--rw-rw-rw-   0        0        0     2671 2024-04-22 20:52:19.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/adapters/funcs.py
--rw-rw-rw-   0        0        0     2739 2024-04-23 14:30:53.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/adapters/misc.py
--rw-rw-rw-   0        0        0     4632 2024-04-23 15:46:14.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/adapters/models.py
--rw-rw-rw-   0        0        0     1595 2024-04-18 20:22:37.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/adapters/registry.py
--rw-rw-rw-   0        0        0      163 2024-03-29 20:13:25.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/apps.py
-drwxrwxrwx   0        0        0        0 2024-04-23 20:50:48.132731 wagtail_fedit-1.5.4rc9/wagtail_fedit/forms/
--rw-rw-rw-   0        0        0      215 2024-04-23 13:02:23.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/forms/__init__.py
--rw-rw-rw-   0        0        0     2881 2024-04-18 20:27:35.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/forms/blocks.py
--rw-rw-rw-   0        0        0     3269 2024-04-23 13:28:56.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/forms/fields.py
--rw-rw-rw-   0        0        0     4617 2024-04-21 02:08:33.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/hooks.py
-drwxrwxrwx   0        0        0        0 2024-04-23 20:50:48.034404 wagtail_fedit-1.5.4rc9/wagtail_fedit/locale/
-drwxrwxrwx   0        0        0        0 2024-04-23 20:50:48.034404 wagtail_fedit-1.5.4rc9/wagtail_fedit/locale/nl/
-drwxrwxrwx   0        0        0        0 2024-04-23 20:50:48.135730 wagtail_fedit-1.5.4rc9/wagtail_fedit/locale/nl/LC_MESSAGES/
--rw-rw-rw-   0        0        0     7262 2024-04-23 15:50:58.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/locale/nl/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0    13018 2024-04-23 15:50:49.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/locale/nl/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2024-04-23 20:50:48.138732 wagtail_fedit-1.5.4rc9/wagtail_fedit/migrations/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/migrations/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-23 20:50:48.139731 wagtail_fedit-1.5.4rc9/wagtail_fedit/migrations/__pycache__/
--rw-rw-rw-   0        0        0      215 2024-03-29 21:05:00.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/migrations/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0     3170 2024-04-05 20:30:10.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/models.py
--rw-rw-rw-   0        0        0     1585 2024-04-23 15:56:07.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/settings.py
-drwxrwxrwx   0        0        0        0 2024-04-23 20:50:48.037413 wagtail_fedit-1.5.4rc9/wagtail_fedit/static/
-drwxrwxrwx   0        0        0        0 2024-04-23 20:50:48.039407 wagtail_fedit-1.5.4rc9/wagtail_fedit/static/wagtail_fedit/
-drwxrwxrwx   0        0        0        0 2024-04-23 20:50:48.144728 wagtail_fedit-1.5.4rc9/wagtail_fedit/static/wagtail_fedit/css/
--rw-rw-rw-   0        0        0     5791 2024-04-23 18:28:37.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/static/wagtail_fedit/css/frontend.css
--rw-rw-rw-   0        0        0     5098 2024-04-17 20:40:49.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/static/wagtail_fedit/css/furniture.css
--rw-rw-rw-   0        0        0     1266 2024-04-05 19:37:44.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css
-drwxrwxrwx   0        0        0        0 2024-04-23 20:50:48.146728 wagtail_fedit-1.5.4rc9/wagtail_fedit/static/wagtail_fedit/js/
--rw-rw-rw-   0        0        0    22454 2024-04-23 18:08:58.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/static/wagtail_fedit/js/frontend.js
-drwxrwxrwx   0        0        0        0 2024-04-23 20:50:48.039407 wagtail_fedit-1.5.4rc9/wagtail_fedit/static/wagtail_fedit/vendor/
-drwxrwxrwx   0        0        0        0 2024-04-23 20:50:48.151729 wagtail_fedit-1.5.4rc9/wagtail_fedit/static/wagtail_fedit/vendor/tippy/
--rw-rw-rw-   0        0        0     1091 2024-04-23 15:39:19.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/static/wagtail_fedit/vendor/tippy/LICENSE
--rw-rw-rw-   0        0        0    20122 2024-04-23 14:51:23.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/static/wagtail_fedit/vendor/tippy/popper.min.js
--rw-rw-rw-   0        0        0    25717 2024-04-23 14:51:31.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/static/wagtail_fedit/vendor/tippy/tippy-bundle.min.js
-drwxrwxrwx   0        0        0        0 2024-04-23 20:50:48.040651 wagtail_fedit-1.5.4rc9/wagtail_fedit/templates/
-drwxrwxrwx   0        0        0        0 2024-04-23 20:50:48.154733 wagtail_fedit-1.5.4rc9/wagtail_fedit/templates/wagtail_fedit/
--rw-rw-rw-   0        0        0       56 2024-04-16 18:37:39.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/templates/wagtail_fedit/_hook_output.html
-drwxrwxrwx   0        0        0        0 2024-04-23 20:50:48.155728 wagtail_fedit-1.5.4rc9/wagtail_fedit/templates/wagtail_fedit/content/
-drwxrwxrwx   0        0        0        0 2024-04-23 20:50:48.158728 wagtail_fedit-1.5.4rc9/wagtail_fedit/templates/wagtail_fedit/content/buttons/
--rw-rw-rw-   0        0        0      929 2024-04-23 15:23:24.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/templates/wagtail_fedit/content/buttons/admin_link.html
--rw-rw-rw-   0        0        0      991 2024-04-23 15:27:54.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_adapter.html
--rw-rw-rw-   0        0        0      571 2024-04-23 17:34:21.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/templates/wagtail_fedit/content/editable_adapter.html
-drwxrwxrwx   0        0        0        0 2024-04-23 20:50:48.170738 wagtail_fedit-1.5.4rc9/wagtail_fedit/templates/wagtail_fedit/editor/
--rw-rw-rw-   0        0        0     2259 2024-04-11 08:02:26.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html
--rw-rw-rw-   0        0        0     3699 2024-04-20 21:55:10.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/templates/wagtail_fedit/editor/action_publish_confirm.html
--rw-rw-rw-   0        0        0      266 2024-04-21 21:15:09.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/templates/wagtail_fedit/editor/adapter_edit_handler.html
--rw-rw-rw-   0        0        0      265 2024-04-21 21:23:24.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/templates/wagtail_fedit/editor/adapter_edit_handler_form.html
--rw-rw-rw-   0        0        0      555 2024-04-21 21:13:45.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/templates/wagtail_fedit/editor/adapter_form.html
--rw-rw-rw-   0        0        0      455 2024-04-21 00:11:35.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/templates/wagtail_fedit/editor/adapter_form_errors.html
--rw-rw-rw-   0        0        0      330 2024-04-21 00:12:14.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/templates/wagtail_fedit/editor/adapter_iframe.html
--rw-rw-rw-   0        0        0     5271 2024-04-21 00:11:24.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html
--rw-rw-rw-   0        0        0      496 2024-04-02 17:46:59.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/templates/wagtail_fedit/editor/field.html
-drwxrwxrwx   0        0        0        0 2024-04-23 20:50:48.177728 wagtail_fedit-1.5.4rc9/wagtail_fedit/templates/wagtail_fedit/icons/
--rw-rw-rw-   0        0        0      797 2024-04-11 08:36:19.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/templates/wagtail_fedit/icons/fedit-check-list.svg
--rw-rw-rw-   0        0        0      584 2024-04-11 08:36:55.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-closed.svg
--rw-rw-rw-   0        0        0      377 2024-04-11 08:23:07.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-open.svg
--rw-rw-rw-   0        0        0      725 2024-04-11 09:02:58.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/templates/wagtail_fedit/icons/fedit-save.svg
--rw-rw-rw-   0        0        0     1323 2024-04-11 08:36:52.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/templates/wagtail_fedit/icons/fedit-stop-sign.svg
-drwxrwxrwx   0        0        0        0 2024-04-23 20:50:48.179728 wagtail_fedit-1.5.4rc9/wagtail_fedit/templates/wagtail_fedit/userbar/
--rw-rw-rw-   0        0        0      867 2024-04-03 17:05:21.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html
--rw-rw-rw-   0        0        0      876 2024-04-03 16:59:31.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html
-drwxrwxrwx   0        0        0        0 2024-04-23 20:50:48.182729 wagtail_fedit-1.5.4rc9/wagtail_fedit/templates/wagtail_fedit/userbar/publish/
--rw-rw-rw-   0        0        0      263 2024-04-11 08:24:35.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/templates/wagtail_fedit/userbar/publish/action_button.html
--rw-rw-rw-   0        0        0      967 2024-04-11 09:03:51.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html
-drwxrwxrwx   0        0        0        0 2024-04-23 20:50:48.200749 wagtail_fedit-1.5.4rc9/wagtail_fedit/templatetags/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:42.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/templatetags/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-23 20:50:48.203736 wagtail_fedit-1.5.4rc9/wagtail_fedit/templatetags/__pycache__/
--rw-rw-rw-   0        0        0      217 2024-03-29 21:05:00.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/templatetags/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0    12928 2024-04-23 20:05:43.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc
--rw-rw-rw-   0        0        0    10181 2024-04-23 20:50:38.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/templatetags/fedit.py
-drwxrwxrwx   0        0        0        0 2024-04-23 20:50:48.207729 wagtail_fedit-1.5.4rc9/wagtail_fedit/test/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/test/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-23 20:50:48.213728 wagtail_fedit-1.5.4rc9/wagtail_fedit/test/core/
--rw-rw-rw-   0        0        0      151 2024-04-05 07:59:49.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/test/core/__init__.py
--rw-rw-rw-   0        0        0      165 2024-04-05 08:41:40.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/test/core/apps.py
--rw-rw-rw-   0        0        0      130 2024-04-15 20:12:38.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/test/core/context_processors.py
-drwxrwxrwx   0        0        0        0 2024-04-23 20:50:48.217728 wagtail_fedit-1.5.4rc9/wagtail_fedit/test/core/migrations/
--rw-rw-rw-   0        0        0    12115 2024-04-20 22:33:35.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/test/core/migrations/0001_initial.py
--rw-rw-rw-   0        0        0      509 2024-04-21 18:41:55.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/test/core/migrations/0002_basicmodel_related_field.py
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/test/core/migrations/__init__.py
--rw-rw-rw-   0        0        0     6047 2024-04-23 13:09:46.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/test/core/models.py
-drwxrwxrwx   0        0        0        0 2024-04-23 20:50:48.231724 wagtail_fedit-1.5.4rc9/wagtail_fedit/test/core/tests/
--rw-rw-rw-   0        0        0        0 2024-04-05 07:59:29.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/test/core/tests/__init__.py
--rw-rw-rw-   0        0        0     8475 2024-04-23 13:35:29.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/test/core/tests/base.py
--rw-rw-rw-   0        0        0    22637 2024-04-23 12:36:52.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/test/core/tests/test_adapters.py
--rw-rw-rw-   0        0        0     4320 2024-04-06 22:44:26.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/test/core/tests/test_block_edit.py
--rw-rw-rw-   0        0        0     5664 2024-04-05 10:31:29.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/test/core/tests/test_blocks.py
--rw-rw-rw-   0        0        0     3642 2024-04-05 18:00:23.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/test/core/tests/test_field_edit.py
--rw-rw-rw-   0        0        0     3709 2024-04-10 13:03:30.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/test/core/tests/test_generic.py
--rw-rw-rw-   0        0        0     4865 2024-04-23 14:23:09.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/test/core/tests/test_model_edit.py
--rw-rw-rw-   0        0        0     1574 2024-04-20 20:49:12.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/test/core/tests/test_revision.py
--rw-rw-rw-   0        0        0     9545 2024-04-20 21:54:40.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/test/core/tests/test_submit.py
--rw-rw-rw-   0        0        0      704 2024-04-05 17:55:36.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/test/manage.py
-drwxrwxrwx   0        0        0        0 2024-04-23 20:50:48.240090 wagtail_fedit-1.5.4rc9/wagtail_fedit/test/testapp/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/test/testapp/__init__.py
--rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/test/testapp/asgi.py
--rw-rw-rw-   0        0        0     3625 2024-04-15 20:14:41.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/test/testapp/settings.py
--rw-rw-rw-   0        0        0      897 2024-04-05 08:04:53.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/test/testapp/urls.py
--rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/test/testapp/wsgi.py
--rw-rw-rw-   0        0        0     2220 2024-04-23 14:21:34.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/toolbar.py
--rw-rw-rw-   0        0        0     1196 2024-04-23 17:25:08.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/urls.py
--rw-rw-rw-   0        0        0    17176 2024-04-23 20:17:01.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-23 20:50:48.246416 wagtail_fedit-1.5.4rc9/wagtail_fedit/views/
--rw-rw-rw-   0        0        0      215 2024-04-23 17:24:50.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/views/__init__.py
--rw-rw-rw-   0        0        0     7388 2024-04-23 20:03:50.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/views/adapters.py
--rw-rw-rw-   0        0        0    17563 2024-04-21 20:25:17.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/views/editable.py
--rw-rw-rw-   0        0        0     1923 2024-04-21 20:29:01.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/views/mixins.py
-drwxrwxrwx   0        0        0        0 2024-04-23 20:50:48.262678 wagtail_fedit-1.5.4rc9/wagtail_fedit/wagtail_hooks/
--rw-rw-rw-   0        0        0      184 2024-04-16 10:03:02.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/wagtail_hooks/__init__.py
--rw-rw-rw-   0        0        0     1748 2024-04-06 18:37:13.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/wagtail_hooks/action_menu.py
--rw-rw-rw-   0        0        0     2857 2024-04-23 15:56:51.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/wagtail_hooks/adapter_hooks.py
--rw-rw-rw-   0        0        0      328 2024-04-21 16:44:33.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/wagtail_hooks/adapter_registry.py
--rw-rw-rw-   0        0        0      398 2024-04-11 09:03:10.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/wagtail_hooks/icons.py
--rw-rw-rw-   0        0        0     2573 2024-04-11 07:39:50.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/wagtail_hooks/log_actions.py
--rw-rw-rw-   0        0        0      340 2024-03-30 17:10:05.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/wagtail_hooks/urls.py
--rw-rw-rw-   0        0        0     7637 2024-04-23 20:17:24.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit/wagtail_hooks/userbar.py
-drwxrwxrwx   0        0        0        0 2024-04-23 20:50:48.110357 wagtail_fedit-1.5.4rc9/wagtail_fedit.egg-info/
--rw-rw-rw-   0        0        0    21651 2024-04-23 20:50:47.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4521 2024-04-23 20:50:48.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 20:50:47.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2024-04-23 20:50:47.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-23 20:50:47.000000 wagtail_fedit-1.5.4rc9/wagtail_fedit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-08 11:33:58.877143 wagtail_fedit-1.5.5rc1/
+-rw-rw-rw-   0        0        0    18429 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.5rc1/LICENSE
+-rw-rw-rw-   0        0        0      257 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.5rc1/MANIFEST.in
+-rw-rw-rw-   0        0        0     3013 2024-05-08 11:33:58.877457 wagtail_fedit-1.5.5rc1/PKG-INFO
+-rw-rw-rw-   0        0        0     1812 2024-04-28 14:18:11.000000 wagtail_fedit-1.5.5rc1/README.md
+-rw-rw-rw-   0        0        0       90 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.5rc1/pyproject.toml
+-rw-rw-rw-   0        0        0     1189 2024-05-08 11:33:58.878496 wagtail_fedit-1.5.5rc1/setup.cfg
+-rw-rw-rw-   0        0        0       39 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.5rc1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 11:33:58.757114 wagtail_fedit-1.5.5rc1/wagtail_fedit/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.5.5rc1/wagtail_fedit/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 11:33:58.775308 wagtail_fedit-1.5.5rc1/wagtail_fedit/adapters/
+-rw-rw-rw-   0        0        0      532 2024-04-22 21:01:35.000000 wagtail_fedit-1.5.5rc1/wagtail_fedit/adapters/__init__.py
+-rw-rw-rw-   0        0        0    14469 2024-04-25 18:57:33.000000 wagtail_fedit-1.5.5rc1/wagtail_fedit/adapters/base.py
+-rw-rw-rw-   0        0        0     6545 2024-04-25 18:29:05.000000 wagtail_fedit-1.5.5rc1/wagtail_fedit/adapters/block.py
+-rw-rw-rw-   0        0        0     8652 2024-04-23 18:12:26.000000 wagtail_fedit-1.5.5rc1/wagtail_fedit/adapters/field.py
+-rw-rw-rw-   0        0        0     2305 2024-04-25 18:28:58.000000 wagtail_fedit-1.5.5rc1/wagtail_fedit/adapters/funcs.py
+-rw-rw-rw-   0        0        0     2755 2024-04-25 18:28:49.000000 wagtail_fedit-1.5.5rc1/wagtail_fedit/adapters/misc.py
+-rw-rw-rw-   0        0        0     5607 2024-05-07 18:13:59.000000 wagtail_fedit-1.5.5rc1/wagtail_fedit/adapters/models.py
+-rw-rw-rw-   0        0        0     1595 2024-04-18 20:22:37.000000 wagtail_fedit-1.5.5rc1/wagtail_fedit/adapters/registry.py
+-rw-rw-rw-   0        0        0      163 2024-03-29 20:13:25.000000 wagtail_fedit-1.5.5rc1/wagtail_fedit/apps.py
+-rw-rw-rw-   0        0        0     1354 2024-04-25 09:55:56.000000 wagtail_fedit-1.5.5rc1/wagtail_fedit/errors.py
+drwxrwxrwx   0        0        0        0 2024-05-08 11:33:58.779125 wagtail_fedit-1.5.5rc1/wagtail_fedit/forms/
+-rw-rw-rw-   0        0        0      215 2024-04-23 13:02:23.000000 wagtail_fedit-1.5.5rc1/wagtail_fedit/forms/__init__.py
+-rw-rw-rw-   0        0        0     2881 2024-04-18 20:27:35.000000 wagtail_fedit-1.5.5rc1/wagtail_fedit/forms/blocks.py
+-rw-rw-rw-   0        0        0     3269 2024-04-23 13:28:56.000000 wagtail_fedit-1.5.5rc1/wagtail_fedit/forms/fields.py
+-rw-rw-rw-   0        0        0     4617 2024-04-21 02:08:33.000000 wagtail_fedit-1.5.5rc1/wagtail_fedit/hooks.py
+drwxrwxrwx   0        0        0        0 2024-05-08 11:33:58.724283 wagtail_fedit-1.5.5rc1/wagtail_fedit/locale/
+drwxrwxrwx   0        0        0        0 2024-05-08 11:33:58.724283 wagtail_fedit-1.5.5rc1/wagtail_fedit/locale/nl/
+drwxrwxrwx   0        0        0        0 2024-05-08 11:33:58.781203 wagtail_fedit-1.5.5rc1/wagtail_fedit/locale/nl/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     7262 2024-04-23 15:50:58.000000 wagtail_fedit-1.5.5rc1/wagtail_fedit/locale/nl/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0    15296 2024-04-25 14:19:13.000000 wagtail_fedit-1.5.5rc1/wagtail_fedit/locale/nl/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2024-05-08 11:33:58.781203 wagtail_fedit-1.5.5rc1/wagtail_fedit/migrations/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.5.5rc1/wagtail_fedit/migrations/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 11:33:58.781203 wagtail_fedit-1.5.5rc1/wagtail_fedit/migrations/__pycache__/
+-rw-rw-rw-   0        0        0      215 2024-03-29 21:05:00.000000 wagtail_fedit-1.5.5rc1/wagtail_fedit/migrations/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0     3170 2024-04-05 20:30:10.000000 wagtail_fedit-1.5.5rc1/wagtail_fedit/models.py
+-rw-rw-rw-   0        0        0     1626 2024-04-25 13:40:59.000000 wagtail_fedit-1.5.5rc1/wagtail_fedit/settings.py
+drwxrwxrwx   0        0        0        0 2024-05-08 11:33:58.726729 wagtail_fedit-1.5.5rc1/wagtail_fedit/static/
+drwxrwxrwx   0        0        0        0 2024-05-08 11:33:58.727975 wagtail_fedit-1.5.5rc1/wagtail_fedit/static/wagtail_fedit/
+drwxrwxrwx   0        0        0        0 2024-05-08 11:33:58.787360 wagtail_fedit-1.5.5rc1/wagtail_fedit/static/wagtail_fedit/css/
+-rw-rw-rw-   0        0        0     5745 2024-05-08 11:26:45.000000 wagtail_fedit-1.5.5rc1/wagtail_fedit/static/wagtail_fedit/css/frontend.css
+-rw-rw-rw-   0        0        0     5098 2024-04-17 20:40:49.000000 wagtail_fedit-1.5.5rc1/wagtail_fedit/static/wagtail_fedit/css/furniture.css
+-rw-rw-rw-   0        0        0     1266 2024-04-05 19:37:44.000000 wagtail_fedit-1.5.5rc1/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css
+drwxrwxrwx   0        0        0        0 2024-05-08 11:33:58.790356 wagtail_fedit-1.5.5rc1/wagtail_fedit/static/wagtail_fedit/js/
+-rw-rw-rw-   0        0        0    50935 2024-05-08 11:33:40.000000 wagtail_fedit-1.5.5rc1/wagtail_fedit/static/wagtail_fedit/js/edit.js
+-rw-rw-rw-   0        0        0    26914 2024-05-07 17:43:52.000000 wagtail_fedit-1.5.5rc1/wagtail_fedit/static/wagtail_fedit/js/frontend.js
+drwxrwxrwx   0        0        0        0 2024-05-08 11:33:58.792862 wagtail_fedit-1.5.5rc1/wagtail_fedit/static/wagtail_fedit/js/licenses/
+-rw-rw-rw-   0        0        0     1091 2024-04-23 15:39:19.000000 wagtail_fedit-1.5.5rc1/wagtail_fedit/static/wagtail_fedit/js/licenses/TIPPY.LICENSE
+drwxrwxrwx   0        0        0        0 2024-05-08 11:33:58.728982 wagtail_fedit-1.5.5rc1/wagtail_fedit/templates/
+drwxrwxrwx   0        0        0        0 2024-05-08 11:33:58.794519 wagtail_fedit-1.5.5rc1/wagtail_fedit/templates/wagtail_fedit/
+-rw-rw-rw-   0        0        0       56 2024-04-16 18:37:39.000000 wagtail_fedit-1.5.5rc1/wagtail_fedit/templates/wagtail_fedit/_hook_output.html
+drwxrwxrwx   0        0        0        0 2024-05-08 11:33:58.796831 wagtail_fedit-1.5.5rc1/wagtail_fedit/templates/wagtail_fedit/content/
+drwxrwxrwx   0        0        0        0 2024-05-08 11:33:58.796926 wagtail_fedit-1.5.5rc1/wagtail_fedit/templates/wagtail_fedit/content/buttons/
+-rw-rw-rw-   0        0        0      929 2024-04-23 15:23:24.000000 wagtail_fedit-1.5.5rc1/wagtail_fedit/templates/wagtail_fedit/content/buttons/admin_link.html
+-rw-rw-rw-   0        0        0      991 2024-04-23 15:27:54.000000 wagtail_fedit-1.5.5rc1/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_adapter.html
+-rw-rw-rw-   0        0        0      571 2024-05-08 11:29:32.000000 wagtail_fedit-1.5.5rc1/wagtail_fedit/templates/wagtail_fedit/content/editable_adapter.html
+drwxrwxrwx   0        0        0        0 2024-05-08 11:33:58.809767 wagtail_fedit-1.5.5rc1/wagtail_fedit/templates/wagtail_fedit/editor/
+-rw-rw-rw-   0        0        0     2259 2024-04-11 08:02:26.000000 wagtail_fedit-1.5.5rc1/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html
+-rw-rw-rw-   0        0        0     3699 2024-04-20 21:55:10.000000 wagtail_fedit-1.5.5rc1/wagtail_fedit/templates/wagtail_fedit/editor/action_publish_confirm.html
+-rw-rw-rw-   0        0        0      266 2024-04-21 21:15:09.000000 wagtail_fedit-1.5.5rc1/wagtail_fedit/templates/wagtail_fedit/editor/adapter_edit_handler.html
+-rw-rw-rw-   0        0        0      265 2024-04-21 21:23:24.000000 wagtail_fedit-1.5.5rc1/wagtail_fedit/templates/wagtail_fedit/editor/adapter_edit_handler_form.html
+-rw-rw-rw-   0        0        0      555 2024-04-21 21:13:45.000000 wagtail_fedit-1.5.5rc1/wagtail_fedit/templates/wagtail_fedit/editor/adapter_form.html
+-rw-rw-rw-   0        0        0      455 2024-04-21 00:11:35.000000 wagtail_fedit-1.5.5rc1/wagtail_fedit/templates/wagtail_fedit/editor/adapter_form_errors.html
+-rw-rw-rw-   0        0        0      330 2024-04-21 00:12:14.000000 wagtail_fedit-1.5.5rc1/wagtail_fedit/templates/wagtail_fedit/editor/adapter_iframe.html
+-rw-rw-rw-   0        0        0     5271 2024-04-21 00:11:24.000000 wagtail_fedit-1.5.5rc1/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html
+-rw-rw-rw-   0        0        0      496 2024-04-02 17:46:59.000000 wagtail_fedit-1.5.5rc1/wagtail_fedit/templates/wagtail_fedit/editor/field.html
+drwxrwxrwx   0        0        0        0 2024-05-08 11:33:58.816040 wagtail_fedit-1.5.5rc1/wagtail_fedit/templates/wagtail_fedit/icons/
+-rw-rw-rw-   0        0        0      797 2024-04-11 08:36:19.000000 wagtail_fedit-1.5.5rc1/wagtail_fedit/templates/wagtail_fedit/icons/fedit-check-list.svg
+-rw-rw-rw-   0        0        0      584 2024-04-11 08:36:55.000000 wagtail_fedit-1.5.5rc1/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-closed.svg
+-rw-rw-rw-   0        0        0      377 2024-04-11 08:23:07.000000 wagtail_fedit-1.5.5rc1/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-open.svg
+-rw-rw-rw-   0        0        0      725 2024-04-11 09:02:58.000000 wagtail_fedit-1.5.5rc1/wagtail_fedit/templates/wagtail_fedit/icons/fedit-save.svg
+-rw-rw-rw-   0        0        0     1323 2024-04-11 08:36:52.000000 wagtail_fedit-1.5.5rc1/wagtail_fedit/templates/wagtail_fedit/icons/fedit-stop-sign.svg
+drwxrwxrwx   0        0        0        0 2024-05-08 11:33:58.821915 wagtail_fedit-1.5.5rc1/wagtail_fedit/templates/wagtail_fedit/userbar/
+-rw-rw-rw-   0        0        0      867 2024-04-03 17:05:21.000000 wagtail_fedit-1.5.5rc1/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html
+-rw-rw-rw-   0        0        0      876 2024-04-03 16:59:31.000000 wagtail_fedit-1.5.5rc1/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html
+drwxrwxrwx   0        0        0        0 2024-05-08 11:33:58.824916 wagtail_fedit-1.5.5rc1/wagtail_fedit/templates/wagtail_fedit/userbar/publish/
+-rw-rw-rw-   0        0        0      263 2024-04-11 08:24:35.000000 wagtail_fedit-1.5.5rc1/wagtail_fedit/templates/wagtail_fedit/userbar/publish/action_button.html
+-rw-rw-rw-   0        0        0      967 2024-04-11 09:03:51.000000 wagtail_fedit-1.5.5rc1/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html
+drwxrwxrwx   0        0        0        0 2024-05-08 11:33:58.827918 wagtail_fedit-1.5.5rc1/wagtail_fedit/templatetags/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:42.000000 wagtail_fedit-1.5.5rc1/wagtail_fedit/templatetags/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 11:33:58.830917 wagtail_fedit-1.5.5rc1/wagtail_fedit/templatetags/__pycache__/
+-rw-rw-rw-   0        0        0      217 2024-03-29 21:05:00.000000 wagtail_fedit-1.5.5rc1/wagtail_fedit/templatetags/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0    13140 2024-05-08 09:22:37.000000 wagtail_fedit-1.5.5rc1/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc
+-rw-rw-rw-   0        0        0    10310 2024-05-07 21:59:17.000000 wagtail_fedit-1.5.5rc1/wagtail_fedit/templatetags/fedit.py
+drwxrwxrwx   0        0        0        0 2024-05-08 11:33:58.833916 wagtail_fedit-1.5.5rc1/wagtail_fedit/test/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.5rc1/wagtail_fedit/test/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 11:33:58.839414 wagtail_fedit-1.5.5rc1/wagtail_fedit/test/core/
+-rw-rw-rw-   0        0        0      151 2024-04-05 07:59:49.000000 wagtail_fedit-1.5.5rc1/wagtail_fedit/test/core/__init__.py
+-rw-rw-rw-   0        0        0      165 2024-04-05 08:41:40.000000 wagtail_fedit-1.5.5rc1/wagtail_fedit/test/core/apps.py
+-rw-rw-rw-   0        0        0      130 2024-04-15 20:12:38.000000 wagtail_fedit-1.5.5rc1/wagtail_fedit/test/core/context_processors.py
+drwxrwxrwx   0        0        0        0 2024-05-08 11:33:58.843403 wagtail_fedit-1.5.5rc1/wagtail_fedit/test/core/migrations/
+-rw-rw-rw-   0        0        0    12115 2024-04-20 22:33:35.000000 wagtail_fedit-1.5.5rc1/wagtail_fedit/test/core/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      509 2024-04-21 18:41:55.000000 wagtail_fedit-1.5.5rc1/wagtail_fedit/test/core/migrations/0002_basicmodel_related_field.py
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.5rc1/wagtail_fedit/test/core/migrations/__init__.py
+-rw-rw-rw-   0        0        0     6047 2024-04-23 13:09:46.000000 wagtail_fedit-1.5.5rc1/wagtail_fedit/test/core/models.py
+drwxrwxrwx   0        0        0        0 2024-05-08 11:33:58.855245 wagtail_fedit-1.5.5rc1/wagtail_fedit/test/core/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-05 07:59:29.000000 wagtail_fedit-1.5.5rc1/wagtail_fedit/test/core/tests/__init__.py
+-rw-rw-rw-   0        0        0     8962 2024-04-25 13:24:28.000000 wagtail_fedit-1.5.5rc1/wagtail_fedit/test/core/tests/base.py
+-rw-rw-rw-   0        0        0    28117 2024-04-25 18:07:06.000000 wagtail_fedit-1.5.5rc1/wagtail_fedit/test/core/tests/test_adapters.py
+-rw-rw-rw-   0        0        0     4320 2024-04-06 22:44:26.000000 wagtail_fedit-1.5.5rc1/wagtail_fedit/test/core/tests/test_block_edit.py
+-rw-rw-rw-   0        0        0     5664 2024-04-05 10:31:29.000000 wagtail_fedit-1.5.5rc1/wagtail_fedit/test/core/tests/test_blocks.py
+-rw-rw-rw-   0        0        0     3642 2024-04-05 18:00:23.000000 wagtail_fedit-1.5.5rc1/wagtail_fedit/test/core/tests/test_field_edit.py
+-rw-rw-rw-   0        0        0     3709 2024-04-10 13:03:30.000000 wagtail_fedit-1.5.5rc1/wagtail_fedit/test/core/tests/test_generic.py
+-rw-rw-rw-   0        0        0     4865 2024-04-23 14:23:09.000000 wagtail_fedit-1.5.5rc1/wagtail_fedit/test/core/tests/test_model_edit.py
+-rw-rw-rw-   0        0        0     1574 2024-04-20 20:49:12.000000 wagtail_fedit-1.5.5rc1/wagtail_fedit/test/core/tests/test_revision.py
+-rw-rw-rw-   0        0        0     9545 2024-04-20 21:54:40.000000 wagtail_fedit-1.5.5rc1/wagtail_fedit/test/core/tests/test_submit.py
+-rw-rw-rw-   0        0        0      704 2024-04-05 17:55:36.000000 wagtail_fedit-1.5.5rc1/wagtail_fedit/test/manage.py
+drwxrwxrwx   0        0        0        0 2024-05-08 11:33:58.860242 wagtail_fedit-1.5.5rc1/wagtail_fedit/test/testapp/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.5rc1/wagtail_fedit/test/testapp/__init__.py
+-rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.5rc1/wagtail_fedit/test/testapp/asgi.py
+-rw-rw-rw-   0        0        0     3625 2024-04-15 20:14:41.000000 wagtail_fedit-1.5.5rc1/wagtail_fedit/test/testapp/settings.py
+-rw-rw-rw-   0        0        0      897 2024-04-05 08:04:53.000000 wagtail_fedit-1.5.5rc1/wagtail_fedit/test/testapp/urls.py
+-rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.5rc1/wagtail_fedit/test/testapp/wsgi.py
+-rw-rw-rw-   0        0        0     2220 2024-04-23 14:21:34.000000 wagtail_fedit-1.5.5rc1/wagtail_fedit/toolbar.py
+-rw-rw-rw-   0        0        0     1196 2024-04-23 17:25:08.000000 wagtail_fedit-1.5.5rc1/wagtail_fedit/urls.py
+-rw-rw-rw-   0        0        0    18101 2024-04-25 13:15:30.000000 wagtail_fedit-1.5.5rc1/wagtail_fedit/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-08 11:33:58.865609 wagtail_fedit-1.5.5rc1/wagtail_fedit/views/
+-rw-rw-rw-   0        0        0      215 2024-04-23 17:24:50.000000 wagtail_fedit-1.5.5rc1/wagtail_fedit/views/__init__.py
+-rw-rw-rw-   0        0        0     8490 2024-04-25 13:06:47.000000 wagtail_fedit-1.5.5rc1/wagtail_fedit/views/adapters.py
+-rw-rw-rw-   0        0        0    17778 2024-04-25 09:19:32.000000 wagtail_fedit-1.5.5rc1/wagtail_fedit/views/editable.py
+-rw-rw-rw-   0        0        0     2239 2024-04-25 09:52:47.000000 wagtail_fedit-1.5.5rc1/wagtail_fedit/views/mixins.py
+drwxrwxrwx   0        0        0        0 2024-05-08 11:33:58.874859 wagtail_fedit-1.5.5rc1/wagtail_fedit/wagtail_hooks/
+-rw-rw-rw-   0        0        0      184 2024-04-16 10:03:02.000000 wagtail_fedit-1.5.5rc1/wagtail_fedit/wagtail_hooks/__init__.py
+-rw-rw-rw-   0        0        0     1748 2024-04-06 18:37:13.000000 wagtail_fedit-1.5.5rc1/wagtail_fedit/wagtail_hooks/action_menu.py
+-rw-rw-rw-   0        0        0     2446 2024-05-07 21:59:49.000000 wagtail_fedit-1.5.5rc1/wagtail_fedit/wagtail_hooks/adapter_hooks.py
+-rw-rw-rw-   0        0        0      328 2024-04-21 16:44:33.000000 wagtail_fedit-1.5.5rc1/wagtail_fedit/wagtail_hooks/adapter_registry.py
+-rw-rw-rw-   0        0        0      398 2024-04-11 09:03:10.000000 wagtail_fedit-1.5.5rc1/wagtail_fedit/wagtail_hooks/icons.py
+-rw-rw-rw-   0        0        0     3100 2024-05-07 18:11:10.000000 wagtail_fedit-1.5.5rc1/wagtail_fedit/wagtail_hooks/log_actions.py
+-rw-rw-rw-   0        0        0      340 2024-03-30 17:10:05.000000 wagtail_fedit-1.5.5rc1/wagtail_fedit/wagtail_hooks/urls.py
+-rw-rw-rw-   0        0        0     7637 2024-04-23 20:17:24.000000 wagtail_fedit-1.5.5rc1/wagtail_fedit/wagtail_hooks/userbar.py
+drwxrwxrwx   0        0        0        0 2024-05-08 11:33:58.764384 wagtail_fedit-1.5.5rc1/wagtail_fedit.egg-info/
+-rw-rw-rw-   0        0        0     3013 2024-05-08 11:33:58.000000 wagtail_fedit-1.5.5rc1/wagtail_fedit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4466 2024-05-08 11:33:58.000000 wagtail_fedit-1.5.5rc1/wagtail_fedit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 11:33:58.000000 wagtail_fedit-1.5.5rc1/wagtail_fedit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2024-05-08 11:33:58.000000 wagtail_fedit-1.5.5rc1/wagtail_fedit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-08 11:33:58.000000 wagtail_fedit-1.5.5rc1/wagtail_fedit.egg-info/top_level.txt
```

### Comparing `wagtail_fedit-1.5.4rc9/LICENSE` & `wagtail_fedit-1.5.5rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc9/setup.cfg` & `wagtail_fedit-1.5.5rc1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2077 6167 7461 696c 5f66 6564 6974   = wagtail_fedit
 00000020: 0d0a 7665 7273 696f 6e20 3d20 312e 352e  ..version = 1.5.
-00000030: 3472 6339 0d0a 6465 7363 7269 7074 696f  4rc9..descriptio
+00000030: 3572 6331 0d0a 6465 7363 7269 7074 696f  5rc1..descriptio
 00000040: 6e20 3d20 4672 6f6e 7465 6e64 2065 6469  n = Frontend edi
 00000050: 7469 6e67 2066 6f72 2079 6f75 7220 5761  ting for your Wa
 00000060: 6774 6169 6c20 7369 7465 0d0a 6c6f 6e67  gtail site..long
 00000070: 5f64 6573 6372 6970 7469 6f6e 203d 2066  _description = f
 00000080: 696c 653a 2052 4541 444d 452e 6d64 0d0a  ile: README.md..
 00000090: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
 000000a0: 5f63 6f6e 7465 6e74 5f74 7970 6520 3d20  _content_type =
```

### Comparing `wagtail_fedit-1.5.4rc9/wagtail_fedit/adapters/__init__.py` & `wagtail_fedit-1.5.5rc1/wagtail_fedit/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc9/wagtail_fedit/adapters/base.py` & `wagtail_fedit-1.5.5rc1/wagtail_fedit/adapters/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,57 +22,59 @@
     TRACK_LOCALES,
 )
 from ..utils import (
     FeditIFrameMixin,
     wrap_adapter,
 )
 
-import uuid
-
 if TYPE_CHECKING:
     from ..toolbar import (
         FeditToolbarComponent,
     )
 
+import json, base64, uuid
+
+
 class AdapterError(Exception):
     pass
 
 
 def content_id_from_parts(*parts: Any) -> str:
     return "-".join(map(slugify, map(str, parts)))
 
+def Base85_json_dumps(obj):
+    return base64.b85encode(json.dumps(obj).encode("utf-8")).decode("utf-8")
 
-import pickle, json, base64
+def Base85_json_loads(data):
+    return json.loads(base64.b85decode(data).decode("utf-8"))
+
+def _get_keywords(bases, attrs):
+    if "keywords" in attrs:
+        return list(attrs["keywords"])
+    
+    for base in bases:
+        if hasattr(base, "keywords"):
+            return list(base.keywords)
+        
+    return list()
+
+def _sort_keywords(keywords):
+    _s = sorted(
+        list(set(keywords)),
+        key=lambda x: (not x.absolute, x.optional, x.default is not None, x.name)
+    )
+    return _s
 
 
 
 class VARIABLES:
     PY_SIZE_VAR = "editor_size"
     FORM_SIZE_VAR = "data-editor-size"
 
 
-class PickleBlockSerializer:
-    """
-    Simple wrapper around pickle to be used in signing.dumps and
-    signing.loads.
-    """
-
-    def dumps(self, obj):
-        return pickle.dumps(obj, protocol=pickle.HIGHEST_PROTOCOL)
-
-    def loads(self, data):
-        return pickle.loads(data)
-
-def Base85_json_dumps(obj):
-    return base64.b85encode(json.dumps(obj).encode("utf-8")).decode("utf-8")
-
-def Base85_json_loads(data):
-    return json.loads(base64.b85decode(data).decode("utf-8"))
-
-
 
 class Keyword:
     def __init__(self, name: str, optional: bool = False, absolute: bool = False, default=None, help_text: str = None, type_hint: Type[Any] = None):
 
         if (default and absolute) or (default and not optional):
             raise AdapterError("Keywords cannot be absolute or required and have a default value")
 
@@ -85,14 +87,24 @@
         self.name = name
         self.optional = optional
         self.absolute = absolute
         self.default = default
         self.help_text = help_text
         self.type_hint = type_hint
 
+    def __hash__(self):
+        return hash(self.name)
+    
+    def __eq__(self, other):
+        if isinstance(other, Keyword):
+            return self.name == other.name
+        elif isinstance(other, str):
+            return self.name == other
+        return False
+
     def __str__(self):
         k = []
 
         if self.optional:
             k.append("?")
         if self.absolute:
             k.append("!")
@@ -126,59 +138,49 @@
         if self.help_text:
             s.append(f"help_text='{self.help_text}'")
         if self.type_hint:
             s.append(f"type: {self.type_hint}")
         s = " ".join(s)
         return f"<{s}>"
 
-def _get_keywords(bases, attrs):
-    if "keywords" in attrs:
-        return list(attrs["keywords"])
-    
-    for base in bases:
-        if hasattr(base, "keywords"):
-            return list(base.keywords)
-        
-    return list()
-
-def _sort_keywords(keywords):
-    _s = sorted(keywords, key=lambda x: (not x.absolute, x.optional))
-    return _s
-
 class AdapterMeta(type):
     def __new__(cls, name, bases, attrs):
         keywords: list[Keyword] = _get_keywords(bases, attrs)
+        
         required_kwargs = []
         absolute_tokens = []
-        optional_kwargs = {}
+        _defaults       = {}
 
         for keyword in keywords:
             if keyword.absolute:
                 absolute_tokens.append(keyword.name)
+                _defaults[keyword.name] = False
             elif keyword.optional:
-                if keyword.default is not None:
-                    optional_kwargs[keyword.name] = keyword.default
-                else:
-                    optional_kwargs[keyword.name] = None
+                _defaults[keyword.name] = keyword.default
             else:
                 required_kwargs.append(keyword.name)
 
         cls = super().__new__(cls, name, bases, attrs)
 
         cls.required_kwargs: tuple[str]     = tuple(required_kwargs)
         cls.absolute_tokens: tuple[str]     = tuple(absolute_tokens)
-        cls.optional_kwargs: dict[str, Any] = optional_kwargs
+        cls._defaults:       dict[str, Any] = _defaults
         cls.keywords:        tuple[Keyword] = tuple(
             _sort_keywords(keywords)
         )
 
         return cls
 
 
 class BaseAdapter(FeditIFrameMixin, metaclass=AdapterMeta):
+    # Type hints for keyword arguments set by metaclass.
+    required_kwargs: tuple[str]
+    absolute_tokens: tuple[str]
+    _defaults:       dict[str, Any]
+
     # How the adapter is identified on inside of the templatetag.
     identifier              = None
 
     # If the templatetag required the first argument to be model.field or just model
     field_required          = True
 
     # The template used to render the form.
@@ -201,19 +203,15 @@
     # The JS constructor for the adapter.
     # This will receive the data after a successful form submission.
     js_constructor          = None
 
     def __init__(self, object: models.Model, field_name: str, request: HttpRequest, **kwargs):
         self.object           = object
         self.request          = request
-        self.kwargs           = kwargs
-
-        for k, v in self.optional_kwargs.items():
-            if k not in self.kwargs and v is not None:
-                self.kwargs[k] = v
+        self.kwargs           = self._defaults.copy() | kwargs
 
         if hasattr(request, "LANGUAGE_CODE") and TRACK_LOCALES:
             if "LANGUAGE_CODE" not in self.kwargs:
                 self.kwargs["LANGUAGE_CODE"] = request.LANGUAGE_CODE
 
             if self.kwargs["LANGUAGE_CODE"] != request.LANGUAGE_CODE:
                 translation.activate(self.kwargs["LANGUAGE_CODE"])
@@ -421,15 +419,21 @@
                 )
                 
             self.request.session[id] = self.kwargs
             self.request.session.modified = True
             return id
         
         if SIGN_SHARED_CONTEXT:
-            return self.signer.sign_object(self.kwargs, compress=True)
+            return self.signer.sign_object(
+                self.kwargs,
+                compress=True,
+                # serializer=SharedContextSerializer(
+                #     self,
+                # ),
+            )
         
         return Base85_json_dumps(self.kwargs)
 
 
     @classmethod
     def decode_shared_context(cls, request: HttpRequest, object: models.Model, field: str, context: str) -> dict:
         """
```

### Comparing `wagtail_fedit-1.5.4rc9/wagtail_fedit/adapters/block.py` & `wagtail_fedit-1.5.5rc1/wagtail_fedit/adapters/block.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,43 +36,43 @@
     """
     An adapter for editing Wagtail blocks.
     This will render the block and replace it on the frontend
     on successful form submission.
     """
     identifier = "block"
     usage_description = "This adapter is used to edit a block of a streamfield."
-    keywords = (
+    keywords = BlockFieldReplacementAdapter.keywords + (
         Keyword("block",
             help_text="the block instance to edit. This can be a regular block instance or a BoundBlock.",
             type_hint="blocks.Block"
         ),
         Keyword("block_id",
             optional=True,
             help_text="the ID of the block to edit, required if block is not a BoundBlock.",
-            type_hint="int"
+            type_hint="str"
         ),
         Keyword("admin",
             absolute=True,
-            help_text="if passed; the adapter will a quick- link to the Wagtail Admin for this block."
+            help_text="if passed; the adapter will add a quick- link to the Wagtail Admin for this block."
         ),
     )
 
     def __init__(self, object: models.Model, field_name: str, request: HttpRequest, **kwargs):
         super().__init__(object, field_name, request, **kwargs)
 
         self.block = self.kwargs.pop("block", None)
         if self.block:
-            if not hasattr(self.block, "id") and not "block_id" in self.kwargs:
+            if not hasattr(self.block, "id") and not self.kwargs["block_id"]:
                 raise AdapterError("Invalid block type, block must have an `id` attribute or provide a `block_id`")
             
             if hasattr(self.block, "id"):
                 self.kwargs["block_id"] = self.block.id
 
         else:
-            block_id = self.kwargs.get("block_id", None)
+            block_id = self.kwargs["block_id"]
             if block_id is None:
                 raise AdapterError("Block ID is required")
             
             self.streamfield: StreamValue = getattr(self.object, self.field_name)
             result = utils.find_block(block_id, self.streamfield)
             if not result:
                 raise AdapterError("Block not found; did you provide the correct block ID?")
@@ -87,15 +87,15 @@
         finder = AdminURLFinder(self.request.user)
         url = finder.get_edit_url(self.object)
         hash = f"#block-{self.kwargs['block_id']}-section"
         return f"{url}{hash}"
 
     def get_toolbar_buttons(self) -> list[FeditAdapterComponent]:
         buttons = super().get_toolbar_buttons()
-        if not self.kwargs.get("admin", False):
+        if not self.kwargs["admin"]:
             return buttons
         
         buttons.append(FeditAdapterAdminLinkButton(
             self.request, self,
         ))
         return buttons
```

### Comparing `wagtail_fedit-1.5.4rc9/wagtail_fedit/adapters/field.py` & `wagtail_fedit-1.5.5rc1/wagtail_fedit/adapters/field.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc9/wagtail_fedit/adapters/funcs.py` & `wagtail_fedit-1.5.5rc1/wagtail_fedit/adapters/funcs.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,25 +1,14 @@
 from django.utils.functional import classproperty
 from .base import Keyword
 from .block import BlockAdapter
 from .field import FieldAdapter
 from itertools import chain
 
 
-# https://stackoverflow.com/a/29088221/18020941
-def dj_model_to_dict(instance):
-    opts = instance._meta
-    data = {}
-    for f in chain(opts.concrete_fields, opts.private_fields):
-        data[f.name] = f.value_from_object(instance)
-    for f in opts.many_to_many:
-        data[f.name] = [i.id for i in f.value_from_object(instance)]
-    return data
-
-
 class FuncAdapterMixin:
     base_identifier = None
     base_keywords = ()
     js_constructor = "wagtail_fedit.editors.BaseFuncEditor"
     js_function = None
 
     @classproperty
```

### Comparing `wagtail_fedit-1.5.4rc9/wagtail_fedit/adapters/misc.py` & `wagtail_fedit-1.5.5rc1/wagtail_fedit/adapters/misc.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,28 +29,28 @@
             "target",
             help_text="The target element to apply the background-image to - this should be a css selector.",
             type_hint="str",
         ),
         Keyword(
             "css_variable_name",
             optional=True,
+            default="background-image",
             help_text="The CSS variable name to apply the background-image to. element.style.setProperty(css_variable_name, url);",
             type_hint="str",
         ),
         Keyword(
             "filter_spec",
             optional=True,
             default="original",
             help_text="The filter spec to apply to the image.",
         ),
         Keyword(
             "preserve_svg",
-            optional=True,
-            default=False,
-            help_text="Preserve SVG images by converting them to a safe format.",
+            absolute=True,
+            help_text="Remove any directives that would require an SVG to be rasterised", # From wagtail.images.utils.to_svg_safe_spec
         ),
     )
     js_constructor = "wagtail_fedit.editors.WagtailFeditFuncEditor"
     js_function = "wagtail_fedit.funcs.backgroundImageFunc"
 
     def render_content(self, parent_context=None):
         return ""
@@ -73,10 +73,9 @@
         rendition = get_rendition_or_not_found(
             image,
             filter,
         )
 
         return data | {
             "url": rendition.url,
-            "css_variable_name":\
-                self.kwargs.get("css_variable_name", None) or "background-image",
+            "css_variable_name": self.kwargs["css_variable_name"],
         }
```

### Comparing `wagtail_fedit-1.5.4rc9/wagtail_fedit/adapters/models.py` & `wagtail_fedit-1.5.5rc1/wagtail_fedit/adapters/models.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 from django.utils.translation import gettext_lazy as _
 from django.http import HttpRequest
+from django.utils import translation
 
-from wagtail.models import Page
+from wagtail.log_actions import log
+from wagtail.models import (
+    Page, RevisionMixin
+)
 from wagtail.admin.panels import (
     page_utils,
     model_utils,
     TabbedInterface,
 )
 
 from .base import (
@@ -37,35 +41,44 @@
     """
     template_name = "wagtail_fedit/editor/adapter_edit_handler.html"
     identifier = "model"
     field_required = False
     usage_description = _("This adapter is used for directly editing a model instance.")
     keywords = BlockFieldReplacementAdapter.keywords + (
         Keyword(
+            "admin",
+            absolute=True,
+            help_text="If passed; the adapter will add a quick-link to the Wagtail Admin for this model.",
+        ),
+        Keyword(
             "render_method",
             optional=True,
             default="render_as_content",
             help_text="The method to call on the object to render it as content. Default is 'render_as_content'.",
         ),
     )
 
     def __init__(self, object, field_name: str, request: HttpRequest, **kwargs):
         super().__init__(object, field_name, request, **kwargs)
         if isinstance(self.object, Page):
-            self.edit_handler = page_utils._get_page_edit_handler(self.object.__class__)
+            self.edit_handler = page_utils._get_page_edit_handler(
+                self.object.__class__,
+            )
         else:
-            self.edit_handler = model_utils.get_edit_handler(self.object.__class__)
+            self.edit_handler = model_utils.get_edit_handler(
+                self.object.__class__,
+            )
 
     def get_admin_url(self) -> str:
         finder = AdminURLFinder(self.request.user)
         return finder.get_edit_url(self.object)
 
     def get_toolbar_buttons(self) -> list[FeditAdapterComponent]:
         buttons = super().get_toolbar_buttons()
-        if not self.kwargs.get("admin", False):
+        if not self.kwargs["admin"]:
             return buttons
         
         buttons.append(FeditAdapterAdminLinkButton(
             self.request, self,
         ))
         return buttons
 
@@ -92,24 +105,41 @@
         class RevisionModelForm(PossibleRevisionFormMixin, cls):
             pass
         return RevisionModelForm
 
     def form_valid(self, form):
         self.object = form.save()
 
+        extra_log_kwargs = {}
+        if isinstance(self.object, RevisionMixin):
+            extra_log_kwargs["revision"] = self.object.latest_revision
+
+        with translation.override(None):
+            log(
+                instance=self.object,
+                action="wagtail_fedit.edit_model",
+                user=self.request.user,
+                data={
+                    "model_verbose": self.object._meta.verbose_name,
+                },
+                content_changed=form.has_changed(),
+                **extra_log_kwargs,
+            )
+
     def get_form(self):
         if self.request.method == "POST":
             form = self.form_class(self.request.POST, for_user=self.request.user, instance=self.object, request=self.request)
         else:
             form = self.form_class(for_user=self.request.user, instance=self.object, request=self.request)
         return form
 
     def get_header_title(self):
         instance_string = get_model_string(self.object)
-        return _("Edit model '%(instance_string)s'") % {
+        return _("Edit model %(type)s '%(instance_string)s'") % {
+            "type": self.object._meta.verbose_name,
             "instance_string": instance_string,
         }
     
     def get_help_text(self):
         return None
           
     def get_element_id(self) -> str:
```

### Comparing `wagtail_fedit-1.5.4rc9/wagtail_fedit/adapters/registry.py` & `wagtail_fedit-1.5.5rc1/wagtail_fedit/adapters/registry.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc9/wagtail_fedit/forms/blocks.py` & `wagtail_fedit-1.5.5rc1/wagtail_fedit/forms/blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc9/wagtail_fedit/forms/fields.py` & `wagtail_fedit-1.5.5rc1/wagtail_fedit/forms/fields.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc9/wagtail_fedit/hooks.py` & `wagtail_fedit-1.5.5rc1/wagtail_fedit/hooks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc9/wagtail_fedit/locale/nl/LC_MESSAGES/django.mo` & `wagtail_fedit-1.5.5rc1/wagtail_fedit/locale/nl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc9/wagtail_fedit/locale/nl/LC_MESSAGES/django.po` & `wagtail_fedit-1.5.5rc1/wagtail_fedit/locale/nl/LC_MESSAGES/django.po`

 * *Files 10% similar despite different names*

```diff
@@ -4,71 +4,127 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-04-23 17:49+0200\n"
+"POT-Creation-Date: 2024-04-25 12:49+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #: .\tester\wagtail_fedit\adapters\block.py:110
+#, python-format
 msgid "Edit block %(block_label)s for %(model_name)s '%(model_string)s'"
 msgstr "Bewerk blok %(block_label)s voor %(model_name)s '%(model_string)s'"
 
-#: .\tester\wagtail_fedit\adapters\field.py:71
+#: .\tester\wagtail_fedit\adapters\field.py:72
+#, python-format
 msgid "Edit model '%(instance_string)s' for %(model_name)s '%(model_string)s'"
-msgstr "Bewerk model %(instance_string)s voor %(model_name)s '%(model_string)s'"
+msgstr ""
+"Bewerk model %(instance_string)s voor %(model_name)s '%(model_string)s'"
 
-#: .\tester\wagtail_fedit\adapters\field.py:77
+#: .\tester\wagtail_fedit\adapters\field.py:78
+#, python-format
 msgid "Edit field '%(field_name)s' for %(model_name)s '%(model_string)s'"
 msgstr "Bewerk veld %(field_name)s voor %(model_name)s' %(model_string)s'"
 
-#: .\tester\wagtail_fedit\adapters\field.py:91
+#: .\tester\wagtail_fedit\adapters\field.py:92
 #, python-format
 msgid ""
 "You must publish %(model)s and the related object of type "
 "%(related_verbose_name)s (%(related_model)s) to make any changes visible."
 msgstr ""
 "U moet %(model)s en het gerelateerde object van het type "
 "%(related_verbose_name)s (%(related_model)s) publiceren om wijzigingen "
 "zichtbaar te maken."
 
-#: .\tester\wagtail_fedit\adapters\field.py:115
+#: .\tester\wagtail_fedit\adapters\field.py:116
 msgid "Publishing related object required."
 msgstr "Publicatie van gerelateerd object vereist."
 
-#: .\tester\wagtail_fedit\adapters\field.py:116
+#: .\tester\wagtail_fedit\adapters\field.py:117
 #: .\tester\wagtail_fedit\utils.py:71
 msgid "The object you are editing supports drafts."
 msgstr "Het object dat u bewerkt ondersteunt concepten."
 
-#: .\tester\wagtail_fedit\adapters\field.py:117
+#: .\tester\wagtail_fedit\adapters\field.py:118
 #, python-format
 msgid ""
 "You must publish the related object of type %(type)s (%(model)s) to make any "
 "changes visible."
 msgstr ""
 "U moet het gerelateerde object van het type %(type)s (%(model)s) publiceren "
 "om wijzigingen zichtbaar te maken."
 
 #: .\tester\wagtail_fedit\adapters\models.py:41
 msgid "This adapter is used for directly editing a model instance."
-msgstr ""
+msgstr "Deze adapter wordt gebruikt voor het direct bewerken van een model."
 
 #: .\tester\wagtail_fedit\adapters\models.py:108
-msgid "Edit model '%(instance_string)s'"
-msgstr "Bewerk model '%(instance_string)s'"
+msgid "Edit model %(type)s '%(instance_string)s'"
+msgstr "Bewerk model %(type)s '%(instance_string)s'"
+
+#: .\tester\wagtail_fedit\errors.py:22
+msgid "You do not have permission to view this page."
+msgstr "U heeft geen toestemming om deze pagina te bekijken."
+
+#: .\tester\wagtail_fedit\errors.py:23
+msgid "User does not have permission to {}"
+msgstr "Gebruiker heeft geen toestemming om {}"
+
+#: .\tester\wagtail_fedit\errors.py:24
+msgid "No workflow state found"
+msgstr "Geen workflowstatus gevonden"
+
+#: .\tester\wagtail_fedit\errors.py:25
+msgid "This object is locked - it cannot be acted upon."
+msgstr "Dit object is vergrendeld - het kan niet worden bewerkt."
+
+#: .\tester\wagtail_fedit\errors.py:26
+msgid "This object is not live"
+msgstr "Dit object is niet live"
+
+#: .\tester\wagtail_fedit\errors.py:27
+msgid "No action specified"
+msgstr "Geen actie opgegeven"
+
+#: .\tester\wagtail_fedit\errors.py:28
+msgid "Invalid action specified: {}"
+msgstr "Ongeldige actie opgegeven: {}"
+
+#: .\tester\wagtail_fedit\errors.py:29
+msgid "Model {} does not inherit from {}"
+msgstr "Model {} erft niet van {}"
+
+#: .\tester\wagtail_fedit\errors.py:30
+msgid "Object has no unpublished changes"
+msgstr "Object heeft geen ongepubliceerde wijzigingen"
+
+#: .\tester\wagtail_fedit\errors.py:31
+msgid "Model not found"
+msgstr "Model niet gevonden"
+
+#: .\tester\wagtail_fedit\errors.py:33
+msgid "Invalid {}"
+msgstr "Ongeldige {}"
+
+#: .\tester\wagtail_fedit\errors.py:34 .\tester\wagtail_fedit\errors.py:38
+msgid "for object {}"
+msgstr "voor object {}"
+
+#: .\tester\wagtail_fedit\errors.py:37
+msgid "{} is required"
+msgstr "{} is vereist"
 
 #: .\tester\wagtail_fedit\templates\wagtail_fedit\content\buttons\admin_link.html:1
 msgid "View in Wagtail admin"
 msgstr "Bekijk in Wagtail admin"
 
 #: .\tester\wagtail_fedit\templates\wagtail_fedit\editor\action_confirm.html:32
 msgid "Are you sure you want to continue?"
@@ -150,15 +206,15 @@
 msgstr "Bekijk live pagina"
 
 #: .\tester\wagtail_fedit\templates\wagtail_fedit\userbar\publish\item_fedit_publishing.html:17
 msgid "Revision Management"
 msgstr "Revisiebeheer"
 
 #: .\tester\wagtail_fedit\utils.py:68
-#: .\tester\wagtail_fedit\views\adapters.py:40
+#: .\tester\wagtail_fedit\views\adapters.py:49
 msgid "Validation Errors"
 msgstr "Validatiefouten"
 
 #: .\tester\wagtail_fedit\utils.py:70
 msgid "Publishing Required"
 msgstr "Publicatie vereist"
 
@@ -182,134 +238,162 @@
 "U hoeft dit object niet te publiceren om deze wijziging zichtbaar te maken."
 
 #: .\tester\wagtail_fedit\utils.py:90
 #, python-format
 msgid "Edit %(type)s '%(model)s'"
 msgstr "Bewerk %(type)s '%(model)s'"
 
-#: .\tester\wagtail_fedit\views\editable.py:222
-msgid "This object is locked. It cannot be acted upon."
-msgstr "Dit object is vergrendeld. Er kan niet op worden gereageerd."
-
-#: .\tester\wagtail_fedit\views\editable.py:226
-msgid "No action specified"
-msgstr "Geen actie opgegeven"
-
-#: .\tester\wagtail_fedit\views\editable.py:230
-msgid "Invalid action specified: {}"
-msgstr "Ongeldige actie opgegeven: {}"
+#: .\tester\wagtail_fedit\views\adapters.py:66
+msgid "Adapter ID"
+msgstr "Adapter-ID"
+
+#: .\tester\wagtail_fedit\views\adapters.py:76
+msgid "Model"
+msgstr "Model"
+
+#: .\tester\wagtail_fedit\views\adapters.py:83
+msgid "view this page"
+msgstr "Bekijk deze pagina"
+
+#: .\tester\wagtail_fedit\views\adapters.py:101
+msgid "Field name"
+msgstr "Veldnaam"
+
+#: .\tester\wagtail_fedit\views\adapters.py:109
+msgid "field name"
+msgstr "veldnaam"
+
+#: .\tester\wagtail_fedit\views\adapters.py:135
+msgid "edit this field"
+msgstr "bewerken van dit veld"
 
-#: .\tester\wagtail_fedit\views\editable.py:239
+#: .\tester\wagtail_fedit\views\editable.py:251
 #: .\tester\wagtail_fedit\wagtail_hooks\userbar.py:53
 msgid "Publish"
 msgstr "Publiceren"
 
-#: .\tester\wagtail_fedit\views\editable.py:243
+#: .\tester\wagtail_fedit\views\editable.py:255
 msgid "Publishing {} \"{}\""
 msgstr "Publiceren van {} \"{}\""
 
-#: .\tester\wagtail_fedit\views\editable.py:246
+#: .\tester\wagtail_fedit\views\editable.py:258
 msgid "About publishing"
 msgstr "Over publiceren"
 
-#: .\tester\wagtail_fedit\views\editable.py:250
+#: .\tester\wagtail_fedit\views\editable.py:262
 msgid "Publishing this object will make it visible to users on the site."
 msgstr ""
 "Publicatie van dit object maakt het zichtbaar voor gebruikers op de site."
 
-#: .\tester\wagtail_fedit\views\editable.py:251
+#: .\tester\wagtail_fedit\views\editable.py:263
 msgid ""
 "That means that any changes you make will be immediately visible to everyone."
 msgstr ""
 "Dit betekent dat alle wijzigingen die u aanbrengt, onmiddellijk zichtbaar "
 "zijnvoor iedereen."
 
-#: .\tester\wagtail_fedit\views\editable.py:255
+#: .\tester\wagtail_fedit\views\editable.py:267
 msgid "You can always choose to unpublish it."
 msgstr "U kunt er altijd voor kiezen om het te depubliceren."
 
-#: .\tester\wagtail_fedit\views\editable.py:356
+#: .\tester\wagtail_fedit\views\editable.py:337
+msgid "publish"
+msgstr "publiceren"
+
+#: .\tester\wagtail_fedit\views\editable.py:370
 #: .\tester\wagtail_fedit\wagtail_hooks\userbar.py:65
 msgid "Unpublish"
 msgstr "Depubliceren"
 
-#: .\tester\wagtail_fedit\views\editable.py:357
+#: .\tester\wagtail_fedit\views\editable.py:371
 msgid "About unpublishing"
 msgstr "Over depubliceren"
 
-#: .\tester\wagtail_fedit\views\editable.py:359
+#: .\tester\wagtail_fedit\views\editable.py:373
 msgid "Unpublishing this object will make it invisible to users on the site."
 msgstr ""
 "Depublicatie van dit object maakt het onzichtbaar voor gebruikers op de site."
 
-#: .\tester\wagtail_fedit\views\editable.py:360
-#: .\tester\wagtail_fedit\views\editable.py:399
-#: .\tester\wagtail_fedit\views\editable.py:442
+#: .\tester\wagtail_fedit\views\editable.py:374
+#: .\tester\wagtail_fedit\views\editable.py:415
+#: .\tester\wagtail_fedit\views\editable.py:460
 msgid "That means that it will no longer be visible to anyone."
 msgstr "Dat betekent dat het niet langer zichtbaar is voor iedereen."
 
-#: .\tester\wagtail_fedit\views\editable.py:361
-#: .\tester\wagtail_fedit\views\editable.py:400
+#: .\tester\wagtail_fedit\views\editable.py:375
+#: .\tester\wagtail_fedit\views\editable.py:416
 msgid "You can always choose to publish it again."
 msgstr "U kunt er altijd voor kiezen om het opnieuw te publiceren."
 
-#: .\tester\wagtail_fedit\views\editable.py:365
+#: .\tester\wagtail_fedit\views\editable.py:379
 msgid "Unpublishing {} \"{}\""
 msgstr "Depubliceren van {} \"{}\""
 
-#: .\tester\wagtail_fedit\views\editable.py:379
-msgid "This object is not live"
-msgstr "Dit object is niet live"
+#: .\tester\wagtail_fedit\views\editable.py:384
+msgid "unpublish"
+msgstr "depubliceren"
 
-#: .\tester\wagtail_fedit\views\editable.py:395
+#: .\tester\wagtail_fedit\views\editable.py:411
 #: .\tester\wagtail_fedit\wagtail_hooks\userbar.py:76
 msgid "Submit for moderation"
 msgstr "Indienen voor moderatie"
 
-#: .\tester\wagtail_fedit\views\editable.py:396
+#: .\tester\wagtail_fedit\views\editable.py:412
 msgid "About submitting for moderation"
 msgstr "Over indienen voor moderatie"
 
-#: .\tester\wagtail_fedit\views\editable.py:398
+#: .\tester\wagtail_fedit\views\editable.py:414
 msgid ""
 "Submitting this object for moderation will make it invisible to users on the "
 "site."
 msgstr ""
 "Het indienen van dit object voor moderatie maakt het onzichtbaar voor "
 "gebruikers op de site."
 
-#: .\tester\wagtail_fedit\views\editable.py:404
+#: .\tester\wagtail_fedit\views\editable.py:420
 msgid "Submitting {} \"{}\" for moderation"
 msgstr "Indienen van {} \"{}\" voor moderatie"
 
-#: .\tester\wagtail_fedit\views\editable.py:438
+#: .\tester\wagtail_fedit\views\editable.py:425
+msgid "submit for moderation"
+msgstr "indienen voor moderatie"
+
+#: .\tester\wagtail_fedit\views\editable.py:456
 #: .\tester\wagtail_fedit\wagtail_hooks\userbar.py:88
 msgid "Cancel Workflow"
 msgstr "Workflow annuleren"
 
-#: .\tester\wagtail_fedit\views\editable.py:439
+#: .\tester\wagtail_fedit\views\editable.py:457
 msgid "About cancelling workflows"
 msgstr "Over het annuleren van workflows"
 
-#: .\tester\wagtail_fedit\views\editable.py:441
+#: .\tester\wagtail_fedit\views\editable.py:459
 msgid ""
 "Cancelling the workflow for this object will remove it from the moderation "
 "process."
 msgstr ""
 "Het annuleren van de workflow voor dit object verwijdert het uit het "
 "moderatieproces."
 
-#: .\tester\wagtail_fedit\views\editable.py:443
+#: .\tester\wagtail_fedit\views\editable.py:461
 msgid "You can always choose to submit it for moderation again."
 msgstr ""
 "Je kunt er altijd voor kiezen om het opnieuw in te dienen voor moderatie."
 
-#: .\tester\wagtail_fedit\views\editable.py:447
+#: .\tester\wagtail_fedit\views\editable.py:465
 msgid "Cancelling workflow for {} \"{}\""
-msgstr ""
+msgstr "Workflow annuleren voor {} \"{}\""
+
+#: .\tester\wagtail_fedit\views\editable.py:473
+msgid "cancel the workflow"
+msgstr "workflow te annuleren"
+
+#: .\tester\wagtail_fedit\views\mixins.py:29
+msgid "model provided"
+msgstr "model verstrekt"
 
 #: .\tester\wagtail_fedit\wagtail_hooks\action_menu.py:14
 msgid "Frontend Edit"
 msgstr "Bewerk op frontend"
 
 #: .\tester\wagtail_fedit\wagtail_hooks\log_actions.py:10
 msgid "Edit Related"
```

### Comparing `wagtail_fedit-1.5.4rc9/wagtail_fedit/models.py` & `wagtail_fedit-1.5.5rc1/wagtail_fedit/models.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc9/wagtail_fedit/settings.py` & `wagtail_fedit-1.5.5rc1/wagtail_fedit/settings.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 TRACK_LOCALES = getattr(settings, "WAGTAIL_FEDIT_TRACK_LOCALES", False)
 """
 Track the locales of the users across the views.
 **This sets the initial request.LANGUAGE_CODE (if available) in the shared context.**
 If this is false, there is no guarantee that the language of a saved field/model
 will be the same as it initially was, generally it will be - however this might mess up with Wagtail's `Page.locale` and
-the page not being available in the context afterwards.
+the page not being available in the context afterwards. If that is the case, set this to `True`.
 """
 
 TIPPY_ENABLED = getattr(settings, "WAGTAIL_FEDIT_TIPPY_ENABLED", True)
 """
 Enable Tippy.js tooltips for toolbar buttons.
 """
```

### Comparing `wagtail_fedit-1.5.4rc9/wagtail_fedit/static/wagtail_fedit/css/frontend.css` & `wagtail_fedit-1.5.5rc1/wagtail_fedit/static/wagtail_fedit/css/frontend.css`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 html, body {
     margin: 0;
     padding: 0;
 }
-
+.wagtail-fedit-adapter-wrapper {
+    position: relative;
+}
 .wagtail-fedit-buttons {
     display: flex;
 }
 
 .wagtail-fedit-adapter-wrapper:has(> .wagtail-fedit-buttons:only-child) {
-    position: relative;
     min-height: 24px;
 }
 .wagtail-fedit-field_bg_image {
     display: inline-flex;
 }
-.wagtail-fedit-adapter-wrapper:has(> .wagtail-fedit-buttons a:hover)::after,
-.wagtail-fedit-adapter-wrapper:has(> .wagtail-fedit-buttons button:hover)::after {
+.wagtail-fedit-adapter-wrapper:has(> .wagtail-fedit-buttons > *:hover)::after {
     content: '';
     display: block;
     position: absolute;
     top: 0;
     left: 0;
     width: 100%;
     height: 100%;
```

### Comparing `wagtail_fedit-1.5.4rc9/wagtail_fedit/static/wagtail_fedit/css/furniture.css` & `wagtail_fedit-1.5.5rc1/wagtail_fedit/static/wagtail_fedit/css/furniture.css`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc9/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css` & `wagtail_fedit-1.5.5rc1/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc9/wagtail_fedit/static/wagtail_fedit/js/frontend.js` & `wagtail_fedit-1.5.5rc1/wagtail_fedit/static/wagtail_fedit/js/frontend.js`

 * *Files 24% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,48 @@
+/**
+ * @callback EditorAPIFunc
+ * @param {WagtailFeditorAPI} api
+ * @returns {void}
+ * 
+ * @callback StringFunc
+ * @param {string} html
+ * @returns {HTMLElement}
+ * 
+ * @callback UpdateFunc
+ * @param {StringFunc} html
+ * 
+ * @typedef {Object} ResponseObject
+ * @property {boolean} success
+ * @property {string|null} html
+ * 
+ * @typedef {Object} FuncResponseObject
+ * @property {boolean} success
+ * @property {string|null} html
+ * @property {Object} func
+ * @property {string} func.name
+ * @property {string} func.target
+ * 
+ * @typedef {Function} EditorCallback
+ * @param {HTMLElement} element
+ * @param {ResponseObject} response
+ * @returns {Promise<any>|void}
+ */
+
+
 class iFrame {
+    /**
+     * @param {Object} options
+     * @param {string} options.id
+     * @param {string} options.className
+     * @param {string} [options.srcdoc=null]
+     * @param {string} [options.url=null]
+     * @param {Function} [options.onLoad=() => {}]
+     * @param {Function} [options.onError=() => {}]
+     * @param {Function} [options.onCancel=() => {}]
+     */
     constructor(options) {
         const {
             id,
             className,
             srcdoc = null,
             url = null,
             onLoad = () => {},
@@ -18,14 +58,17 @@
         this.className = className;
         this.onLoad = onLoad;
         this.onError = onError;
         this.onCancel = onCancel;
         this.render();
     }
 
+    /**
+     * @returns {HTMLIFrameElement}
+     */
     get element() {
         if (!this.iframe) {
             this.iframe = this._renderFrame(this.url, this.srcdoc, this.onLoad);
         }
         return this.iframe;
     }
 
@@ -94,14 +137,17 @@
         };
         return iframe;
     }
 }
 
 
 class Tooltip {
+    /**
+     * @param {HTMLElement} element
+     **/
     constructor(element) {
         this.element = element;
         this.tooltipConfig = this.makeConfig();
         this.init();
     }
 
     init() {
@@ -143,109 +189,195 @@
         this.#editor.makeModal();
     }
 
     closeModal() {
         this.#editor.closeModal();
     }
 
+    dispatchEvent(name, detail = null) {
+        this.#editor.dispatchEvent(name, detail);
+    }
+
+    addEventListener(name, callback) {
+        this.#editor.addEventListener(name, callback);
+    }
+
+    removeEventListener(name, callback, options = null) {
+        this.#editor.removeEventListener(name, callback, options);
+    }
+
+    /**
+     * @param {string|UpdateFunc} html
+     * @returns {Promise<HTMLElement>}
+     **/
     updateHtml(html) {
+        return new Promise((resolve, reject) => {
+            const update = (innerHtml) => {
+                const blockWrapper = this.#editor.wrapperElement;
+                const element = document.createElement("div");
+                element.innerHTML = innerHtml;
+                const newBlockWrapper = element.firstElementChild;
+                newBlockWrapper.classList.add("wagtail-fedit-initialized");
+                blockWrapper.parentNode.insertBefore(newBlockWrapper, blockWrapper);
+                blockWrapper.parentNode.removeChild(blockWrapper);
+                this.#editor.wrapperElement = newBlockWrapper;
+                this.#editor.initNewEditors();
+                this.#editor.init();
 
-        const update = (innerHtml) => {
-            const blockWrapper = this.#editor.wrapperElement;
-            const element = document.createElement("div");
-            element.innerHTML = innerHtml;
-            const newBlockWrapper = element.firstElementChild;
-            newBlockWrapper.classList.add("wagtail-fedit-initialized");
-            blockWrapper.parentNode.insertBefore(newBlockWrapper, blockWrapper);
-            blockWrapper.parentNode.removeChild(blockWrapper);
-            this.#editor.wrapperElement = newBlockWrapper;
-            this.#editor.initNewEditors();
-            this.#editor.init();
+                resolve(newBlockWrapper);
 
-            return blockWrapper;
-        }
+                return blockWrapper;
+            }
 
-        if (typeof html === "string") {
-            update(html);
-            return;
-        }
+            if (typeof html === "string") {
+                update(html);
+                return;
+            }
 
-        if (typeof html === "function") {
-            this.#editor.wrapperElement.editorAPI = this;
-            html(update);
-            return;
-        }
+            if (typeof html === "function") {
+                this.#editor.wrapperElement.editorAPI = this;
+                html(update);
+                return;
+            }
+        });
     }
 
+    /**
+     * @returns {Promise<any>}
+     **/
     refetch() {
-        this.#editor.refetch();
+        return this.#editor.refetch();
     }
 
+    /**
+     * @param {EditorAPIFunc} func
+     * @returns {void}
+     **/
     execRelated(func) {
         for (const wrapper of this.#editor.relatedWrappers) {
             func(wrapper.editorAPI);
         }
     }
 }
 
 
-class BaseWagtailFeditEditor {
-    constructor(options) {
-        const {
-            element = null,
-        } = options;
+class BaseWagtailFeditEditor extends EventTarget {
+    /**
+     * @param {HTMLElement} element
+     */
+    constructor(element) {
+        super();
 
+        /**@type {string} */
         this.initialTitle = document.title;
 
         /**@type {HTMLElement} */
         this.wrapperElement = element;
+
+        /**@type {WagtailFeditorAPI} */
         this.api = new WagtailFeditorAPI(this);
+
+        /**@type {string} */
         this.sharedContext = null;
+
+        /**@type {string} */
         this.modalHtml = null;
+
+        /**@type {HTMLElement} */
         this.editBtn = null;
         this.init();
+
+        /**@type {iFrame} */
         this.iframe = null;
 
 
         if (window.location.hash === `#${this.wrapperElement.id}`) {
             this.makeModal();
             this.focus();
         }
     }
 
+    get editUrl() {
+        return this.wrapperElement.dataset.editUrl;
+    }
+
+    get refetchUrl() {
+        return this.wrapperElement.dataset.refetchUrl;
+    }
+
     get relatedWrappers() {
         const wrapperId = this.wrapperElement.dataset.wrapperId;
         const filterFn = (el) => el !== this.wrapperElement
         const elements = document.querySelectorAll(`[data-wrapper-id="${wrapperId}"]`)
         return Array.from(elements).filter(filterFn);
     }
 
-    focus() {
-        this.wrapperElement.focus();
+    get modalWrapper() {
+        const modalWrapper = document.querySelector("#wagtail-fedit-modal-wrapper");
+        if (modalWrapper) {
+            return modalWrapper;
+        }
+        const wrapper = document.createElement("div");
+        wrapper.id = "wagtail-fedit-modal-wrapper";
+        wrapper.classList.add("wagtail-fedit-modal-wrapper");
+        wrapper.editorAPI = this.api;
+        document.body.appendChild(wrapper);
+        return wrapper;
     }
 
-    get editUrl() {
-        return this.wrapperElement.dataset.editUrl;
+    init() {
+        this.sharedContext = this.wrapperElement.dataset.sharedContext;
+        this.modalHtml = modalHtml.replace("__ID__", this.wrapperElement.dataset.id);
+        this.editBtn = this.wrapperElement.querySelector(".wagtail-fedit-edit-button");
+
+        this.wrapperElement.editorAPI = this.api;
+
+        this.editBtn.addEventListener("click", async (e) => {
+            e.preventDefault();
+            e.stopPropagation();
+            await this.makeModal();
+        });
     }
 
-    get refetchUrl() {
-        return this.wrapperElement.dataset.refetchUrl;
+    initNewEditors() {
+        initNewEditors(this.wrapperElement);
     }
 
+    focus() {
+        this.wrapperElement.focus();
+    }
+
+    /**
+     * @returns {Promise<ResponseObject>}
+     */
     refetch() {
-        fetch(this.getRefetchUrl()).then((response) => {
-            response = response.json();
-            return response;
-        }).then((response) => {
-            if (!response.success) {
-                console.error("Errors rendering response", response);
-                return;
-            }
-            this.onResponse(response);
-        });
+        return new Promise((resolve, reject) => {
+            fetch(this.getRefetchUrl()).then((response) => {
+                response = response.json();
+                return response;
+            }).then((response) => {
+                if (!response.success) {
+                    console.error("Errors rendering response, failed to refetch", response);
+                    return;
+                }
+                this.onResponse(response);
+                resolve(response);
+            }).catch((e) => {
+                console.error("Failed to refetch", e);
+                reject(e);
+            });
+        })
+    }
+
+    /**
+     * @param {ResponseObject} response
+     * @returns {Promise<any>|void}
+     */
+    onResponse(response) {
+
     }
 
     getEditUrl() {
         // build the edit url from relative edit url
         const url = new URL(window.location.href);
         url.pathname = this.editUrl;
         if (this.sharedContext) {
@@ -272,14 +404,20 @@
             url: this.getEditUrl(),
             id: "wagtail-fedit-iframe",
             className: null,
             onLoad: () => {
                 const onSubmit = (e) => {
                     e.preventDefault();
                     const formData = new FormData(this.iframe.formElement);
+
+                    this.dispatchEvent(window.wagtailFedit.EVENTS.SUBMIT, {
+                        element: this.wrapperElement,
+                        formData: formData,
+                    });
+
                     fetch(this.getEditUrl(), {
                         method: "POST",
                         body: formData,
                     }).then((response) => {
                         response = response.json();
                         return response;
                     }).then((response) => {
@@ -293,58 +431,60 @@
                             const uninitializedBlock = this.iframe.mainElement.querySelector("#value[data-block]");
                             if (uninitializedBlock) {
                                 this.iframe.window.initBlockWidget(uninitializedBlock.id);
                             }
 
                             const cancelButton = this.iframe.document.querySelector(".wagtail-fedit-cancel-button");
                             cancelButton.addEventListener("click", this.closeModal.bind(this));
+                            this.iframe.onCancel = this.closeModal.bind(this);
+                            this.dispatchEvent(window.wagtailFedit.EVENTS.SUBMIT_ERROR, {
+                                element: this.wrapperElement,
+                                response: response,
+                            });
                             return;
                         }
-                        this.onResponse(response);
-                        this.closeModal();
-
-                        const event = new CustomEvent("wagtail-fedit:change", {
-                            detail: {
+                        const ret = this.onResponse(response);
+                        const success = () => {
+                            this.closeModal();
+                            this.dispatchEvent(window.wagtailFedit.EVENTS.CHANGE, {
                                 element: this.wrapperElement,
-                            }
-                        });
-                        document.dispatchEvent(event);
+                            });
+                        }
+                        if (ret instanceof Promise) {
+                            ret.then(success);
+                        } else {
+                            success();
+                        }
                     });
                 };
                 this.iframe.formElement.onsubmit = onSubmit;
                 this.iframe.onCancel = this.closeModal.bind(this);
 
                 // Check if we need to apply the fedit-full class to the modal
-                const formHeight = this.iframe.formElement.getBoundingClientRect().height;
                 const formWrapper = this.iframe.formWrapper;
                 const options = ["large", "full"]
 
                 for (const option of options) {
                     if (formWrapper && (
                             formWrapper.classList.contains(`fedit-${option}`) ||
                             (this.iframe.formElement.dataset.editorSize || "").toLowerCase() === option
                         )) {
                         this.modal.classList.add(`fedit-${option}`);
                         break;
                     }
                 }
 
-                if (
-                    (formWrapper && (
-                        formWrapper.classList.contains("fedit-large") ||
-                        (this.iframe.formElement.dataset.fullEditor || "").toLowerCase() === "true"
-                    )) ||
-                    (formHeight > window.innerHeight)
-                ) {
-                    this.modal.classList.add("fedit-large");
-                }
-
                 const url = window.location.href.split("#")[0];
                 window.history.pushState(null, this.iframe.document.title, url + `#${this.wrapperElement.id}`);
                 document.title = this.iframe.document.title;
+
+                this.dispatchEvent(window.wagtailFedit.EVENTS.MODAL_LOAD, {
+                    iframe: this.iframe,
+                    modal: this.modal,
+                });
             },
             onError: () => {
                 this.closeModal();
             },
             onCancel: () => {
                 this.closeModal();
             },
@@ -353,85 +493,91 @@
         this.modal.appendChild(this.iframe.element);
 
         const closeBtn = document.createElement("button");
         closeBtn.innerHTML = "&times;";
         closeBtn.classList.add("wagtail-fedit-close-button");
         closeBtn.addEventListener("click", this.closeModal.bind(this));
         this.modal.appendChild(closeBtn);
+        this.dispatchEvent(window.wagtailFedit.EVENTS.MODAL_OPEN, {
+            iframe: this.iframe,
+            modal: this.modal,
+        });
     }
 
     closeModal() {
         this.modalWrapper.remove();
         window.history.pushState(null, this.initialTitle, window.location.href.split("#")[0]);
         document.title = this.initialTitle;
-        if ("onModalClose" in this) {
-            this.onModalClose();
-        }
+        this.dispatchEvent(window.wagtailFedit.EVENTS.MODAL_CLOSE);
     }
 
-    get modalWrapper() {
-        const modalWrapper = document.querySelector("#wagtail-fedit-modal-wrapper");
-        if (modalWrapper) {
-            return modalWrapper;
+    dispatchEvent(name, detail = null) {
+        if (!detail) {
+            detail = {
+                element: this.wrapperElement,
+            };
         }
-        const wrapper = document.createElement("div");
-        wrapper.id = "wagtail-fedit-modal-wrapper";
-        wrapper.classList.add("wagtail-fedit-modal-wrapper");
-        document.body.appendChild(wrapper);
-        return wrapper;
-    }
-
-    init() {
-        this.sharedContext = this.wrapperElement.dataset.sharedContext;
-        this.modalHtml = modalHtml.replace("__ID__", this.wrapperElement.dataset.id);
-        this.editBtn = this.wrapperElement.querySelector(".wagtail-fedit-edit-button");
 
-        this.wrapperElement.editorAPI = this.api;
-
-        this.editBtn.addEventListener("click", async (e) => {
-            e.preventDefault();
-            e.stopPropagation();
-            await this.makeModal();
+        detail.editor = this;
+        detail.api = this.api;
+        let eventStr = name.toLowerCase();
+        if (!name.startsWith(`${window.wagtailFedit.NAMESPACE}:`)) {
+            eventStr = `${window.wagtailFedit.NAMESPACE}:${name}`;
+        }
+        const event = new CustomEvent(eventStr, {
+            detail: detail,
         });
-    }
-
-    initNewEditors() {
-        initNewEditors(this.wrapperElement);
+        super.dispatchEvent(event);
+        this.wrapperElement.dispatchEvent(event);
+        document.dispatchEvent(event);
     }
 }
 
 function initNewEditors(wrapper = document) {
-    const wagtailFeditBlockEditors = wrapper.querySelectorAll(".wagtail-fedit-adapter-wrapper");
+    let wagtailFeditBlockEditors;
+    if (
+        wrapper != document &&
+        wrapper.classList.contains("wagtail-fedit-adapter-wrapper") &&
+        !wrapper.classList.contains("wagtail-fedit-initialized")
+    ) {
+        wagtailFeditBlockEditors = [wrapper];
+    } else {
+        wagtailFeditBlockEditors = wrapper.querySelectorAll(".wagtail-fedit-adapter-wrapper");
+    }
     for (const editor of wagtailFeditBlockEditors) {
         if (!editor.classList.contains("wagtail-fedit-initialized")) {
             editor.classList.add("wagtail-fedit-initialized");
             const editorClass = getEditorClass(editor);
             if (editorClass) {
-                new editorClass({
-                    element: editor
-                });
+                new editorClass(editor);
             } else {
                 console.error("No editor class found for element", editor);
             }
         }
-    }
-    const editButtons = wrapper.querySelectorAll("[data-tooltip='true']");
-    for (const button of editButtons) {
-        if (button.dataset.tooltip == "true") {
-            new Tooltip(button);
-            delete button.dataset.tooltip;
+
+        const editButtons = wrapper.querySelectorAll("[data-tooltip='true']");
+        for (const button of editButtons) {
+            if (button.dataset.tooltip == "true") {
+                new Tooltip(button);
+                delete button.dataset.tooltip;
+            }
         }
     }
 }
 
 class BaseFuncEditor extends BaseWagtailFeditEditor {
     static get funcMap() {
         return window
     }
 
+    /**
+     * @param {FuncResponseObject} response
+     * @returns {Promise<any>|void}
+     * @override
+     **/
     onResponse(response) {
         const name = response.func.name;
         const targetElementSelector = response.func.target;
         if (!name || !targetElementSelector) {
             console.error("Invalid response", response);
             return;
         }
@@ -444,29 +590,34 @@
 
         const func = this.constructor.funcMap[name];
         if (!func) {
             console.error("Function not found", name);
             return;
         }
 
-        func(targetElement, response);
+        return func(targetElement, response);
     }
 }
 
 
 class WagtailFeditFuncEditor extends BaseFuncEditor {
     static get funcMap() {
         return window.wagtailFedit.funcs;
     }
 }
 
 
 class BlockFieldEditor extends BaseWagtailFeditEditor {
+    /**
+     * @param {ResponseObject} response
+     * @returns {Promise<any>|void}
+     * @override
+     **/
     onResponse(response) {
-        this.api.updateHtml((update) => {
+        return this.api.updateHtml((update) => {
             // Fade out the old block
             const anim = this.wrapperElement.animate([{
                 opacity: 1
             }, {
                 opacity: 0
             }, ], {
                 duration: 350,
@@ -474,17 +625,17 @@
             });
 
             anim.onfinish = () => {
 
                 const blockWrapper = update(response.html);
 
                 if (!response.refetch) {
-                    for (const wrapper of this.relatedWrappers) {
-                        wrapper.editorAPI.refetch();
-                    }
+                    this.api.execRelated((relatedAPI) => {
+                        relatedAPI.refetch();
+                    });
                 }
 
                 // Fade in the new block
                 const anim = blockWrapper.animate([{
                     opacity: 0
                 }, {
                     opacity: 1
@@ -499,27 +650,30 @@
         });
     }
 }
 
 
 class WagtailFeditPublishMenu {
     constructor(publishButton) {
+        /**@type {HTMLElement} */
         this.publishButton = publishButton;
+        /**@type {HTMLElement} */
         this.publishButtonsWrapper = publishButton.parentElement.querySelector(".wagtail-fedit-form-buttons");
+        /**@type {NodeList} */
         const buttons = this.publishButtonsWrapper.querySelectorAll(".wagtail-fedit-userbar-button");
         let initialIsHidden = false;
         for (const button of buttons) {
             if (button.classList.contains("initially-hidden")) {
                 initialIsHidden = true;
                 break;
             }
         }
 
         if (initialIsHidden) {
-            document.addEventListener("wagtail-fedit:change", (e) => {
+            document.addEventListener(window.wagtailFedit.EVENTS.CHANGE, () => {
                 for (const button of buttons) {
                     if (button.classList.contains("initially-hidden")) {
                         button.classList.remove("initially-hidden");
                     }
                 }
             })
         }
@@ -576,32 +730,15 @@
 
 function initFEditors() {
     initNewEditors()
     const observer = new MutationObserver((mutations) => {
         for (const mutation of mutations) {
             for (const node of mutation.addedNodes) {
                 if (node.nodeType === 1) {
-                    if (node.classList.contains("wagtail-fedit-adapter-wrapper") && !node.classList.contains("wagtail-fedit-initialized")) {
-                        node.classList.add("wagtail-fedit-initialized");
-                        const editorClass = getEditorClass(node);
-                        if (editorClass) {
-                            new editorClass({
-                                element: node
-                            });
-                        } else {
-                            console.error("No editor class found for element", node);
-                        }
-                    }
-                    const editButtons = node.querySelectorAll("[data-tooltip='true']");
-                    for (const button of editButtons) {
-                        if (button.dataset.tooltip == "true") {
-                            new Tooltip(button);
-                            delete button.dataset.tooltip;
-                        }
-                    }
+                    initNewEditors(node);
                 }
             }
         }
     });
     observer.observe(document.body, {
         childList: true,
         subtree: true
@@ -651,20 +788,25 @@
                     window.history.replaceState(null, "", windowURL.toString());
                 }, 50);
             });
         }
 
 
         if (publishMenu) {
-            const publisher = new WagtailFeditPublishMenu(publishMenu);
+            new WagtailFeditPublishMenu(publishMenu);
         }
     }
 }
 
-
+/**
+ * @satisfies {EditorCallback}
+ * @param {HTMLElement} element
+ * @param {ResponseObject} response
+ * @returns {void}
+ */
 function wagtailFeditBackgroundImageAdapter(element, response) {
     const url = response.url;
     const cssVar = response.css_variable_name;
     if (cssVar) {
         if (cssVar.startsWith("--")) {
             element.style.setProperty(cssVar, `url(${url})`);
         } else {
@@ -674,31 +816,57 @@
         element.style.backgroundImage = `url(${url})`;
     }
 }
 
 
 document.addEventListener("DOMContentLoaded", initFEditors);
 
-
 window.wagtailFedit = {
-    initFEditors,
-    BaseWagtailFeditEditor,
-    BaseFuncEditor,
-    BlockFieldEditor,
-    WagtailFeditPublishMenu,
-    WagtailFeditorAPI,
-    iFrame,
+    NAMESPACE: "wagtail-fedit",
+    EVENTS: {
+        SUBMIT: "wagtail-fedit:submit",
+        CHANGE: "wagtail-fedit:change",
+        MODAL_OPEN: "wagtail-fedit:modalOpen",
+        MODAL_LOAD: "wagtail-fedit:modalLoad",
+        MODAL_CLOSE: "wagtail-fedit:modalClose",
+        SUBMIT_ERROR: "wagtail-fedit:submitError",
+    },
+    exports: {
+        initFEditors,
+        BaseWagtailFeditEditor,
+        BaseFuncEditor,
+        BlockFieldEditor,
+        WagtailFeditPublishMenu,
+        WagtailFeditorAPI,
+        iFrame,
+        Tooltip,
+    },
+    /**
+     * @type {Object<string, BaseWagtailFeditEditor>}
+     **/
     editors: {
         "wagtail_fedit.editors.BaseFuncEditor": BaseFuncEditor,
         "wagtail_fedit.editors.BlockFieldEditor": BlockFieldEditor,
         "wagtail_fedit.editors.WagtailFeditFuncEditor": WagtailFeditFuncEditor,
     },
+    /**
+     * @type {Object<string, EditorCallback>}
+     */
     funcs: {
         "wagtail_fedit.funcs.backgroundImageFunc": wagtailFeditBackgroundImageAdapter,
     },
+    /**
+     * @param {string} name
+     * @param {BaseWagtailFeditEditor} editor
+     */
     register: function(name, editor) {
         this.editors[name] = editor;
     },
+
+    /**
+     * @param {string} name
+     * @param {EditorCallback} func
+     */
     registerFunc: function(name, func) {
         this.funcs[name] = func;
     },
 };
```

### Comparing `wagtail_fedit-1.5.4rc9/wagtail_fedit/static/wagtail_fedit/vendor/tippy/LICENSE` & `wagtail_fedit-1.5.5rc1/wagtail_fedit/static/wagtail_fedit/js/licenses/TIPPY.LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc9/wagtail_fedit/templates/wagtail_fedit/content/buttons/admin_link.html` & `wagtail_fedit-1.5.5rc1/wagtail_fedit/templates/wagtail_fedit/content/buttons/admin_link.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc9/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_adapter.html` & `wagtail_fedit-1.5.5rc1/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_adapter.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc9/wagtail_fedit/templates/wagtail_fedit/content/editable_adapter.html` & `wagtail_fedit-1.5.5rc1/wagtail_fedit/templates/wagtail_fedit/content/editable_adapter.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc9/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html` & `wagtail_fedit-1.5.5rc1/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc9/wagtail_fedit/templates/wagtail_fedit/editor/action_publish_confirm.html` & `wagtail_fedit-1.5.5rc1/wagtail_fedit/templates/wagtail_fedit/editor/action_publish_confirm.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc9/wagtail_fedit/templates/wagtail_fedit/editor/adapter_form.html` & `wagtail_fedit-1.5.5rc1/wagtail_fedit/templates/wagtail_fedit/editor/adapter_form.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc9/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html` & `wagtail_fedit-1.5.5rc1/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc9/wagtail_fedit/templates/wagtail_fedit/icons/fedit-check-list.svg` & `wagtail_fedit-1.5.5rc1/wagtail_fedit/templates/wagtail_fedit/icons/fedit-check-list.svg`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc9/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-closed.svg` & `wagtail_fedit-1.5.5rc1/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-closed.svg`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc9/wagtail_fedit/templates/wagtail_fedit/icons/fedit-save.svg` & `wagtail_fedit-1.5.5rc1/wagtail_fedit/templates/wagtail_fedit/icons/fedit-save.svg`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc9/wagtail_fedit/templates/wagtail_fedit/icons/fedit-stop-sign.svg` & `wagtail_fedit-1.5.5rc1/wagtail_fedit/templates/wagtail_fedit/icons/fedit-stop-sign.svg`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc9/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html` & `wagtail_fedit-1.5.5rc1/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc9/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html` & `wagtail_fedit-1.5.5rc1/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc9/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html` & `wagtail_fedit-1.5.5rc1/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc9/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc` & `wagtail_fedit-1.5.5rc1/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc`

 * *Files 16% similar despite different names*

#### Python bytecode

```diff
@@ -1,40 +1,42 @@
 magic:    0xa70d0d0a
-moddate:  0x83142866 (Tue Apr 23 20:05:23 2024 UTC)
-files sz: 9810
+moddate:  0x35a43a66 (Tue May  7 21:59:17 2024 UTC)
+files sz: 10310
 code
    argcount  : 0
    nlocals   : 0
-   stacksize : 13
+   stacksize : 11
    flags     : 0
    code
       0x9700640064016c006d015a016d025a020100640064026c036d045a046d
       055a056d065a060100640064036c076d085a080100640064046c096d0a5a
       0a6d0b5a0b6d0c5a0c0100640064056c0d6d0e5a0e0100640064066c0f6d
       105a100100640064076c116d125a120100640064086c136d145a14010064
-      0064096c156d165a1601006400640a6c176d185a1801006400640b6c196d
-      1a5a1a6d1b5a1b01006400640c6c1c5a1c640d640e6c1d6d1e5a1e6d1f5a
-      1f6d205a206d215a210100640d640f6c226d235a236d245a246d255a256d
-      265a260100640d64106c186d275a276d285a280100020065046a29000000
-      0000000000a6000000ab0000000000000000005a2a64115a2b64125a2c64
-      13652d641465086415652d6416652d6608641784045a2e02004700641884
-      0064196505a6030000ab0300000000000000005a2f652aa0300000000000
-      0000000000000000000000000000006526ac1aa6010000ab010000000000
-      000000641b650a641c650b6604641d8404a6000000ab0000000000000000
-      005a31652aa0320000000000000000000000000000000000000000641eac
-      1fa6010000ab01000000000000000064146508642065206416652d660664
-      218404a6000000ab0000000000000000005a33652aa03400000000000000
-      0000000000000000000000000064226423641eac24a6030000ab03000000
-      000000000064166535660264258404a6000000ab0000000000000000005a
-      36652aa032000000000000000000000000000000000000000064266427ac
-      28a6020000ab02000000000000000064306429652d6416652d6604642a84
-      05a6000000ab0000000000000000005a376431641b650a642b6538652d19
-      000000000000000000642c6538652d19000000000000000000642d653865
-      2d19000000000000000000642e6535652d65026602190000000000000000
-      0064166535660c642f84055a39640c5300
+      0064096c156d165a166d175a1701006400640a6c185a18640b640c6c196d
+      1a5a1a0100640b640d6c1b6d1c5a1c6d1d5a1d6d1e5a1e6d1f5a1f010064
+      0b640e6c206d215a216d225a226d235a236d245a246d255a256d265a266d
+      275a276d285a286d295a290100640b640f6c146d2a5a2a6d2b5a2b010002
+      0065046a2c0000000000000000a6000000ab0000000000000000005a2d64
+      105a2e64115a2f641265306413650864146530641565306608641684045a
+      31020047006417840064186505a6030000ab0300000000000000005a3265
+      2da03300000000000000000000000000000000000000006527ac19a60100
+      00ab010000000000000000641a650a641b650b6604641c8404a6000000ab
+      0000000000000000005a34652da035000000000000000000000000000000
+      0000000000641dac1ea6010000ab01000000000000000064136508641f65
+      1e64156530660664208404a6000000ab0000000000000000005a36652da0
+      37000000000000000000000000000000000000000064216422641dac23a6
+      030000ab03000000000000000064156538660264248404a6000000ab0000
+      000000000000005a39652da0350000000000000000000000000000000000
+      00000064256426ac27a6020000ab02000000000000000064316428653064
+      156530660464298405a6000000ab0000000000000000005a3a652da03500
+      00000000000000000000000000000000000000641d642aac27a6020000ab
+      020000000000000000642b6502641565306604642c8404a6000000ab0000
+      000000000000005a3b6432641a650a642d653c6530190000000000000000
+      00642e653c653019000000000000000000642f653c653019000000000000
+      00000064156538660a643084055a3d640a5300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (('Type', 'Any'))
                  6 IMPORT_NAME              0 (typing)
                  8 IMPORT_FROM              1 (Type)
                 10 STORE_NAME               1 (Type)
@@ -68,355 +70,372 @@
                 60 IMPORT_FROM             11 (Token)
                 62 STORE_NAME              11 (Token)
                 64 IMPORT_FROM             12 (FilterExpression)
                 66 STORE_NAME              12 (FilterExpression)
                 68 POP_TOP
    
     12          70 LOAD_CONST               0 (0)
-                72 LOAD_CONST               5 (('HttpRequest',))
-                74 IMPORT_NAME             13 (django.http)
-                76 IMPORT_FROM             14 (HttpRequest)
-                78 STORE_NAME              14 (HttpRequest)
+                72 LOAD_CONST               5 (('escape',))
+                74 IMPORT_NAME             13 (django.utils.html)
+                76 IMPORT_FROM             14 (escape)
+                78 STORE_NAME              14 (escape)
                 80 POP_TOP
    
     13          82 LOAD_CONST               0 (0)
-                84 LOAD_CONST               6 (('escape',))
-                86 IMPORT_NAME             15 (django.utils.html)
-                88 IMPORT_FROM             16 (escape)
-                90 STORE_NAME              16 (escape)
+                84 LOAD_CONST               6 (('mark_safe',))
+                86 IMPORT_NAME             15 (django.utils.safestring)
+                88 IMPORT_FROM             16 (mark_safe)
+                90 STORE_NAME              16 (mark_safe)
                 92 POP_TOP
    
     14          94 LOAD_CONST               0 (0)
-                96 LOAD_CONST               7 (('mark_safe',))
-                98 IMPORT_NAME             17 (django.utils.safestring)
-               100 IMPORT_FROM             18 (mark_safe)
-               102 STORE_NAME              18 (mark_safe)
+                96 LOAD_CONST               7 (('signing',))
+                98 IMPORT_NAME             17 (django.core)
+               100 IMPORT_FROM             18 (signing)
+               102 STORE_NAME              18 (signing)
                104 POP_TOP
    
-    15         106 LOAD_CONST               0 (0)
-               108 LOAD_CONST               8 (('reverse',))
-               110 IMPORT_NAME             19 (django.urls)
-               112 IMPORT_FROM             20 (reverse)
-               114 STORE_NAME              20 (reverse)
+    16         106 LOAD_CONST               0 (0)
+               108 LOAD_CONST               8 (('hooks',))
+               110 IMPORT_NAME             19 (wagtail)
+               112 IMPORT_FROM             20 (hooks)
+               114 STORE_NAME              20 (hooks)
                116 POP_TOP
    
-    16         118 LOAD_CONST               0 (0)
-               120 LOAD_CONST               9 (('signing',))
-               122 IMPORT_NAME             21 (django.core)
-               124 IMPORT_FROM             22 (signing)
-               126 STORE_NAME              22 (signing)
-               128 POP_TOP
-   
-    18         130 LOAD_CONST               0 (0)
-               132 LOAD_CONST              10 (('hooks',))
-               134 IMPORT_NAME             23 (wagtail)
-               136 IMPORT_FROM             24 (hooks)
-               138 STORE_NAME              24 (hooks)
-               140 POP_TOP
-   
-    19         142 LOAD_CONST               0 (0)
-               144 LOAD_CONST              11 (('Page', 'PAGE_TEMPLATE_VAR'))
-               146 IMPORT_NAME             25 (wagtail.models)
-               148 IMPORT_FROM             26 (Page)
-               150 STORE_NAME              26 (Page)
-               152 IMPORT_FROM             27 (PAGE_TEMPLATE_VAR)
-               154 STORE_NAME              27 (PAGE_TEMPLATE_VAR)
-               156 POP_TOP
-   
-    24         158 LOAD_CONST               0 (0)
-               160 LOAD_CONST              12 (None)
-               162 IMPORT_NAME             28 (warnings)
-               164 STORE_NAME              28 (warnings)
-   
-    26         166 LOAD_CONST              13 (2)
-               168 LOAD_CONST              14 (('adapter_registry', 'RegistryLookUpError', 'BaseAdapter', 'AdapterError'))
-               170 IMPORT_NAME             29 (adapters)
-               172 IMPORT_FROM             30 (adapter_registry)
-               174 STORE_NAME              30 (adapter_registry)
-               176 IMPORT_FROM             31 (RegistryLookUpError)
-               178 STORE_NAME              31 (RegistryLookUpError)
-               180 IMPORT_FROM             32 (BaseAdapter)
-               182 STORE_NAME              32 (BaseAdapter)
-               184 IMPORT_FROM             33 (AdapterError)
-               186 STORE_NAME              33 (AdapterError)
-               188 POP_TOP
-   
-    32         190 LOAD_CONST              13 (2)
-               192 LOAD_CONST              15 (('wrap_adapter', '_can_edit', 'FEDIT_PREVIEW_VAR', 'TEMPLATE_TAG_NAME'))
-               194 IMPORT_NAME             34 (utils)
-               196 IMPORT_FROM             35 (wrap_adapter)
-               198 STORE_NAME              35 (wrap_adapter)
-               200 IMPORT_FROM             36 (_can_edit)
-               202 STORE_NAME              36 (_can_edit)
-               204 IMPORT_FROM             37 (FEDIT_PREVIEW_VAR)
-               206 STORE_NAME              37 (FEDIT_PREVIEW_VAR)
-               208 IMPORT_FROM             38 (TEMPLATE_TAG_NAME)
-               210 STORE_NAME              38 (TEMPLATE_TAG_NAME)
-               212 POP_TOP
-   
-    38         214 LOAD_CONST              13 (2)
-               216 LOAD_CONST              16 (('REGISTER_CSS', 'REGISTER_JS'))
-               218 IMPORT_NAME             24 (hooks)
-               220 IMPORT_FROM             39 (REGISTER_CSS)
-               222 STORE_NAME              39 (REGISTER_CSS)
-               224 IMPORT_FROM             40 (REGISTER_JS)
-               226 STORE_NAME              40 (REGISTER_JS)
-               228 POP_TOP
-   
-    44         230 PUSH_NULL
-               232 LOAD_NAME                4 (library)
-               234 LOAD_ATTR               41 (Library)
-               244 PRECALL                  0
-               248 CALL                     0
-               258 STORE_NAME              42 (register)
-   
-    47         260 LOAD_CONST              17 ('Field name is not available in the context for %(object)s.')
-               262 STORE_NAME              43 (WARNING_FIELD_NAME_NOT_AVAILABLE)
-   
-    48         264 LOAD_CONST              18 ('Model instance is not available in the context for %(object)s.')
-               266 STORE_NAME              44 (WARNING_MODEL_INSTANCE_NOT_AVAILABLE)
-   
-    51         268 LOAD_CONST              19 ('var')
-               270 LOAD_NAME               45 (str)
-               272 LOAD_CONST              20 ('context')
-               274 LOAD_NAME                8 (Context)
-               276 LOAD_CONST              21 ('value')
-               278 LOAD_NAME               45 (str)
-               280 LOAD_CONST              22 ('return')
-               282 LOAD_NAME               45 (str)
-               284 BUILD_TUPLE              8
-               286 LOAD_CONST              23 (<code object as_var, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 51>)
-               288 MAKE_FUNCTION            4 (annotations)
-               290 STORE_NAME              46 (as_var)
-   
-    58         292 PUSH_NULL
-               294 LOAD_BUILD_CLASS
-               296 LOAD_CONST              24 (<code object AdapterNode, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 58>)
-               298 MAKE_FUNCTION            0
-               300 LOAD_CONST              25 ('AdapterNode')
-               302 LOAD_NAME                5 (Node)
-               304 PRECALL                  3
-               308 CALL                     3
-               318 STORE_NAME              47 (AdapterNode)
-   
-   149         320 LOAD_NAME               42 (register)
-               322 LOAD_METHOD             48 (tag)
-               344 LOAD_NAME               38 (TEMPLATE_TAG_NAME)
-               346 KW_NAMES                26
-               348 PRECALL                  1
-               352 CALL                     1
-   
-   150         362 LOAD_CONST              27 ('parser')
-               364 LOAD_NAME               10 (Parser)
-               366 LOAD_CONST              28 ('token')
-               368 LOAD_NAME               11 (Token)
-               370 BUILD_TUPLE              4
-               372 LOAD_CONST              29 (<code object do_render_fedit, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 149>)
-               374 MAKE_FUNCTION            4 (annotations)
-   
-   149         376 PRECALL                  0
-               380 CALL                     0
-   
-   150         390 STORE_NAME              49 (do_render_fedit)
-   
-   207         392 LOAD_NAME               42 (register)
-               394 LOAD_METHOD             50 (simple_tag)
-               416 LOAD_CONST              30 (True)
-               418 KW_NAMES                31
-               420 PRECALL                  1
-               424 CALL                     1
-   
-   208         434 LOAD_CONST              20 ('context')
-               436 LOAD_NAME                8 (Context)
-               438 LOAD_CONST              32 ('adapter')
-               440 LOAD_NAME               32 (BaseAdapter)
-               442 LOAD_CONST              22 ('return')
-               444 LOAD_NAME               45 (str)
-               446 BUILD_TUPLE              6
-               448 LOAD_CONST              33 (<code object render_adapter, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 207>)
-               450 MAKE_FUNCTION            4 (annotations)
-   
-   207         452 PRECALL                  0
-               456 CALL                     0
-   
-   208         466 STORE_NAME              51 (render_adapter)
-   
-   229         468 LOAD_NAME               42 (register)
-               470 LOAD_METHOD             52 (inclusion_tag)
-               492 LOAD_CONST              34 ('wagtail_fedit/_hook_output.html')
-               494 LOAD_CONST              35 ('fedit_scripts')
-               496 LOAD_CONST              30 (True)
-               498 KW_NAMES                36
-               500 PRECALL                  3
-               504 CALL                     3
-   
-   230         514 LOAD_CONST              22 ('return')
-               516 LOAD_NAME               53 (dict)
-               518 BUILD_TUPLE              2
-               520 LOAD_CONST              37 (<code object static_hook_output, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 229>)
-               522 MAKE_FUNCTION            4 (annotations)
-   
-   229         524 PRECALL                  0
-               528 CALL                     0
-   
-   230         538 STORE_NAME              54 (static_hook_output)
-   
-   259         540 LOAD_NAME               42 (register)
-               542 LOAD_METHOD             50 (simple_tag)
-               564 LOAD_CONST              38 (False)
-               566 LOAD_CONST              39 ('tooltip')
-               568 KW_NAMES                40
-               570 PRECALL                  2
-               574 CALL                     2
-   
-   260         584 LOAD_CONST              48 ((None,))
-               586 LOAD_CONST              41 ('wrapping')
-               588 LOAD_NAME               45 (str)
-               590 LOAD_CONST              22 ('return')
-               592 LOAD_NAME               45 (str)
-               594 BUILD_TUPLE              4
-               596 LOAD_CONST              42 (<code object tooltip, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 259>)
-               598 MAKE_FUNCTION            5 (defaults, annotations)
-   
-   259         600 PRECALL                  0
-               604 CALL                     0
-   
-   260         614 STORE_NAME              55 (tooltip)
-   
-   275         616 LOAD_CONST              49 ((None, None, None))
-               618 LOAD_CONST              27 ('parser')
-               620 LOAD_NAME               10 (Parser)
-               622 LOAD_CONST              43 ('tokens')
-               624 LOAD_NAME               56 (list)
-               626 LOAD_NAME               45 (str)
-               628 BINARY_SUBSCR
-               638 LOAD_CONST              44 ('kwarg_list')
-               640 LOAD_NAME               56 (list)
-               642 LOAD_NAME               45 (str)
-               644 BINARY_SUBSCR
-               654 LOAD_CONST              45 ('absolute_tokens')
-               656 LOAD_NAME               56 (list)
-               658 LOAD_NAME               45 (str)
-               660 BINARY_SUBSCR
-               670 LOAD_CONST              46 ('optional_tokens')
-               672 LOAD_NAME               53 (dict)
-               674 LOAD_NAME               45 (str)
-               676 LOAD_NAME                2 (Any)
-               678 BUILD_TUPLE              2
-               680 BINARY_SUBSCR
-               690 LOAD_CONST              22 ('return')
-               692 LOAD_NAME               53 (dict)
-               694 BUILD_TUPLE             12
-               696 LOAD_CONST              47 (<code object get_kwargs, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 275>)
-               698 MAKE_FUNCTION            5 (defaults, annotations)
-               700 STORE_NAME              57 (get_kwargs)
-               702 LOAD_CONST              12 (None)
-               704 RETURN_VALUE
+    17         118 LOAD_CONST               0 (0)
+               120 LOAD_CONST               9 (('Page', 'PAGE_TEMPLATE_VAR'))
+               122 IMPORT_NAME             21 (wagtail.models)
+               124 IMPORT_FROM             22 (Page)
+               126 STORE_NAME              22 (Page)
+               128 IMPORT_FROM             23 (PAGE_TEMPLATE_VAR)
+               130 STORE_NAME              23 (PAGE_TEMPLATE_VAR)
+               132 POP_TOP
+   
+    22         134 LOAD_CONST               0 (0)
+               136 LOAD_CONST              10 (None)
+               138 IMPORT_NAME             24 (warnings)
+               140 STORE_NAME              24 (warnings)
+   
+    24         142 LOAD_CONST              11 (2)
+               144 LOAD_CONST              12 (('TIPPY_ENABLED',))
+               146 IMPORT_NAME             25 (settings)
+               148 IMPORT_FROM             26 (TIPPY_ENABLED)
+               150 STORE_NAME              26 (TIPPY_ENABLED)
+               152 POP_TOP
+   
+    27         154 LOAD_CONST              11 (2)
+               156 LOAD_CONST              13 (('adapter_registry', 'RegistryLookUpError', 'BaseAdapter', 'AdapterError'))
+               158 IMPORT_NAME             27 (adapters)
+               160 IMPORT_FROM             28 (adapter_registry)
+               162 STORE_NAME              28 (adapter_registry)
+               164 IMPORT_FROM             29 (RegistryLookUpError)
+               166 STORE_NAME              29 (RegistryLookUpError)
+               168 IMPORT_FROM             30 (BaseAdapter)
+               170 STORE_NAME              30 (BaseAdapter)
+               172 IMPORT_FROM             31 (AdapterError)
+               174 STORE_NAME              31 (AdapterError)
+               176 POP_TOP
+   
+    33         178 LOAD_CONST              11 (2)
+               180 LOAD_CONST              14 (('wrap_adapter', 'with_userbar_model', 'base_adapter_context', '_flatten_context', '_can_edit', 'FEDIT_PREVIEW_VAR', 'TEMPLATE_TAG_NAME', 'FIELD_TEMPLATE_VAR', 'INSTANCE_TEMPLATE_VAR'))
+               182 IMPORT_NAME             32 (utils)
+               184 IMPORT_FROM             33 (wrap_adapter)
+               186 STORE_NAME              33 (wrap_adapter)
+               188 IMPORT_FROM             34 (with_userbar_model)
+               190 STORE_NAME              34 (with_userbar_model)
+               192 IMPORT_FROM             35 (base_adapter_context)
+               194 STORE_NAME              35 (base_adapter_context)
+               196 IMPORT_FROM             36 (_flatten_context)
+               198 STORE_NAME              36 (_flatten_context)
+               200 IMPORT_FROM             37 (_can_edit)
+               202 STORE_NAME              37 (_can_edit)
+               204 IMPORT_FROM             38 (FEDIT_PREVIEW_VAR)
+               206 STORE_NAME              38 (FEDIT_PREVIEW_VAR)
+               208 IMPORT_FROM             39 (TEMPLATE_TAG_NAME)
+               210 STORE_NAME              39 (TEMPLATE_TAG_NAME)
+               212 IMPORT_FROM             40 (FIELD_TEMPLATE_VAR)
+               214 STORE_NAME              40 (FIELD_TEMPLATE_VAR)
+               216 IMPORT_FROM             41 (INSTANCE_TEMPLATE_VAR)
+               218 STORE_NAME              41 (INSTANCE_TEMPLATE_VAR)
+               220 POP_TOP
+   
+    45         222 LOAD_CONST              11 (2)
+               224 LOAD_CONST              15 (('REGISTER_CSS', 'REGISTER_JS'))
+               226 IMPORT_NAME             20 (hooks)
+               228 IMPORT_FROM             42 (REGISTER_CSS)
+               230 STORE_NAME              42 (REGISTER_CSS)
+               232 IMPORT_FROM             43 (REGISTER_JS)
+               234 STORE_NAME              43 (REGISTER_JS)
+               236 POP_TOP
+   
+    51         238 PUSH_NULL
+               240 LOAD_NAME                4 (library)
+               242 LOAD_ATTR               44 (Library)
+               252 PRECALL                  0
+               256 CALL                     0
+               266 STORE_NAME              45 (register)
+   
+    54         268 LOAD_CONST              16 ('Field name is not available in the context for %(object)s.')
+               270 STORE_NAME              46 (WARNING_FIELD_NAME_NOT_AVAILABLE)
+   
+    55         272 LOAD_CONST              17 ('Model instance is not available in the context for %(object)s.')
+               274 STORE_NAME              47 (WARNING_MODEL_INSTANCE_NOT_AVAILABLE)
+   
+    58         276 LOAD_CONST              18 ('var')
+               278 LOAD_NAME               48 (str)
+               280 LOAD_CONST              19 ('context')
+               282 LOAD_NAME                8 (Context)
+               284 LOAD_CONST              20 ('value')
+               286 LOAD_NAME               48 (str)
+               288 LOAD_CONST              21 ('return')
+               290 LOAD_NAME               48 (str)
+               292 BUILD_TUPLE              8
+               294 LOAD_CONST              22 (<code object as_var, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 58>)
+               296 MAKE_FUNCTION            4 (annotations)
+               298 STORE_NAME              49 (as_var)
+   
+    65         300 PUSH_NULL
+               302 LOAD_BUILD_CLASS
+               304 LOAD_CONST              23 (<code object AdapterNode, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 65>)
+               306 MAKE_FUNCTION            0
+               308 LOAD_CONST              24 ('AdapterNode')
+               310 LOAD_NAME                5 (Node)
+               312 PRECALL                  3
+               316 CALL                     3
+               326 STORE_NAME              50 (AdapterNode)
+   
+   174         328 LOAD_NAME               45 (register)
+               330 LOAD_METHOD             51 (tag)
+               352 LOAD_NAME               39 (TEMPLATE_TAG_NAME)
+               354 KW_NAMES                25
+               356 PRECALL                  1
+               360 CALL                     1
+   
+   175         370 LOAD_CONST              26 ('parser')
+               372 LOAD_NAME               10 (Parser)
+               374 LOAD_CONST              27 ('token')
+               376 LOAD_NAME               11 (Token)
+               378 BUILD_TUPLE              4
+               380 LOAD_CONST              28 (<code object do_render_fedit, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 174>)
+               382 MAKE_FUNCTION            4 (annotations)
+   
+   174         384 PRECALL                  0
+               388 CALL                     0
+   
+   175         398 STORE_NAME              52 (do_render_fedit)
+   
+   230         400 LOAD_NAME               45 (register)
+               402 LOAD_METHOD             53 (simple_tag)
+               424 LOAD_CONST              29 (True)
+               426 KW_NAMES                30
+               428 PRECALL                  1
+               432 CALL                     1
+   
+   231         442 LOAD_CONST              19 ('context')
+               444 LOAD_NAME                8 (Context)
+               446 LOAD_CONST              31 ('adapter')
+               448 LOAD_NAME               30 (BaseAdapter)
+               450 LOAD_CONST              21 ('return')
+               452 LOAD_NAME               48 (str)
+               454 BUILD_TUPLE              6
+               456 LOAD_CONST              32 (<code object render_adapter, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 230>)
+               458 MAKE_FUNCTION            4 (annotations)
+   
+   230         460 PRECALL                  0
+               464 CALL                     0
+   
+   231         474 STORE_NAME              54 (render_adapter)
+   
+   252         476 LOAD_NAME               45 (register)
+               478 LOAD_METHOD             55 (inclusion_tag)
+               500 LOAD_CONST              33 ('wagtail_fedit/_hook_output.html')
+               502 LOAD_CONST              34 ('fedit_scripts')
+               504 LOAD_CONST              29 (True)
+               506 KW_NAMES                35
+               508 PRECALL                  3
+               512 CALL                     3
+   
+   253         522 LOAD_CONST              21 ('return')
+               524 LOAD_NAME               56 (dict)
+               526 BUILD_TUPLE              2
+               528 LOAD_CONST              36 (<code object static_hook_output, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 252>)
+               530 MAKE_FUNCTION            4 (annotations)
+   
+   252         532 PRECALL                  0
+               536 CALL                     0
+   
+   253         546 STORE_NAME              57 (static_hook_output)
+   
+   282         548 LOAD_NAME               45 (register)
+               550 LOAD_METHOD             53 (simple_tag)
+               572 LOAD_CONST              37 (False)
+               574 LOAD_CONST              38 ('tooltip')
+               576 KW_NAMES                39
+               578 PRECALL                  2
+               582 CALL                     2
+   
+   283         592 LOAD_CONST              49 ((None,))
+               594 LOAD_CONST              40 ('wrapping')
+               596 LOAD_NAME               48 (str)
+               598 LOAD_CONST              21 ('return')
+               600 LOAD_NAME               48 (str)
+               602 BUILD_TUPLE              4
+               604 LOAD_CONST              41 (<code object tooltip, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 282>)
+               606 MAKE_FUNCTION            5 (defaults, annotations)
+   
+   282         608 PRECALL                  0
+               612 CALL                     0
+   
+   283         622 STORE_NAME              58 (tooltip)
+   
+   301         624 LOAD_NAME               45 (register)
+               626 LOAD_METHOD             53 (simple_tag)
+               648 LOAD_CONST              29 (True)
+               650 LOAD_CONST              42 ('fedit_userbar')
+               652 KW_NAMES                39
+               654 PRECALL                  2
+               658 CALL                     2
+   
+   302         668 LOAD_CONST              43 ('model')
+               670 LOAD_NAME                2 (Any)
+               672 LOAD_CONST              21 ('return')
+               674 LOAD_NAME               48 (str)
+               676 BUILD_TUPLE              4
+               678 LOAD_CONST              44 (<code object do_with_userbar_model, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 301>)
+               680 MAKE_FUNCTION            4 (annotations)
+   
+   301         682 PRECALL                  0
+               686 CALL                     0
+   
+   302         696 STORE_NAME              59 (do_with_userbar_model)
+   
+   309         698 LOAD_CONST              50 ((None, None))
+               700 LOAD_CONST              26 ('parser')
+               702 LOAD_NAME               10 (Parser)
+               704 LOAD_CONST              45 ('tokens')
+               706 LOAD_NAME               60 (list)
+               708 LOAD_NAME               48 (str)
+               710 BINARY_SUBSCR
+               720 LOAD_CONST              46 ('kwarg_list')
+               722 LOAD_NAME               60 (list)
+               724 LOAD_NAME               48 (str)
+               726 BINARY_SUBSCR
+               736 LOAD_CONST              47 ('absolute_tokens')
+               738 LOAD_NAME               60 (list)
+               740 LOAD_NAME               48 (str)
+               742 BINARY_SUBSCR
+               752 LOAD_CONST              21 ('return')
+               754 LOAD_NAME               56 (dict)
+               756 BUILD_TUPLE             10
+               758 LOAD_CONST              48 (<code object get_kwargs, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 309>)
+               760 MAKE_FUNCTION            5 (defaults, annotations)
+               762 STORE_NAME              61 (get_kwargs)
+               764 LOAD_CONST              10 (None)
+               766 RETURN_VALUE
    consts
       0
       ('Type', 'Any')
       ('library', 'Node', 'TemplateSyntaxError')
       ('Context',)
       ('Parser', 'Token', 'FilterExpression')
-      ('HttpRequest',)
       ('escape',)
       ('mark_safe',)
-      ('reverse',)
       ('signing',)
       ('hooks',)
       ('Page', 'PAGE_TEMPLATE_VAR')
       None
       2
+      ('TIPPY_ENABLED',)
       ('adapter_registry', 'RegistryLookUpError', 'BaseAdapter', 'AdapterError')
-      ('wrap_adapter', '_can_edit', 'FEDIT_PREVIEW_VAR', 'TEMPLATE_TAG_NAME')
+      ('wrap_adapter', 'with_userbar_model', 'base_adapter_context', '_flatten_context', '_can_edit', 'FEDIT_PREVIEW_VAR', 'TEMPLATE_TAG_NAME', 'FIELD_TEMPLATE_VAR', 'INSTANCE_TEMPLATE_VAR')
       ('REGISTER_CSS', 'REGISTER_JS')
       'Field name is not available in the context for %(object)s.'
       'Model instance is not available in the context for %(object)s.'
       'var'
       'context'
       'value'
       'return'
       code
          argcount  : 3
          nlocals   : 3
          stacksize : 3
          flags     : 3
          code 0x97007c0073027c0253007c027c017c003c00000064015300
-          51           0 RESUME                   0
+          58           0 RESUME                   0
          
-          52           2 LOAD_FAST                0 (var)
+          59           2 LOAD_FAST                0 (var)
                        4 POP_JUMP_FORWARD_IF_TRUE     2 (to 10)
          
-          53           6 LOAD_FAST                2 (value)
+          60           6 LOAD_FAST                2 (value)
                        8 RETURN_VALUE
          
-          55     >>   10 LOAD_FAST                2 (value)
+          62     >>   10 LOAD_FAST                2 (value)
                       12 LOAD_FAST                1 (context)
                       14 LOAD_FAST                0 (var)
                       16 STORE_SUBSCR
          
-          56          20 LOAD_CONST               1 ('')
+          63          20 LOAD_CONST               1 ('')
                       22 RETURN_VALUE
          consts
             None
             ''
          names      ()
          varnames   ('var', 'context', 'value')
          freevars   ()
          cellvars   ()
-         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
+         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
          name       'as_var'
-         firstlineno 51
+         firstlineno 58
          lnotab 0x0201040104020a01
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 9
          flags     : 0
          code
             0x970065005a0164005a02020065036a040000000000000000a6000000ab
             0000000000000000005a0564096402650665071900000000000000000064
             03650864046509650a190000000000000000006405650a6608640684055a
             0b640784005a0c640884005a0d64015300
-          58           0 RESUME                   0
+          65           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('AdapterNode')
                        8 STORE_NAME               2 (__qualname__)
          
-          59          10 PUSH_NULL
+          66          10 PUSH_NULL
                       12 LOAD_NAME                3 (signing)
                       14 LOAD_ATTR                4 (TimestampSigner)
                       24 PRECALL                  0
                       28 CALL                     0
                       38 STORE_NAME               5 (signer)
          
-          61          40 LOAD_CONST               9 ((None,))
+          68          40 LOAD_CONST               9 ((None,))
                       42 LOAD_CONST               2 ('adapter')
                       44 LOAD_NAME                6 (Type)
                       46 LOAD_NAME                7 (BaseAdapter)
                       48 BINARY_SUBSCR
                       58 LOAD_CONST               3 ('model')
                       60 LOAD_NAME                8 (FilterExpression)
                       62 LOAD_CONST               4 ('getters')
                       64 LOAD_NAME                9 (list)
                       66 LOAD_NAME               10 (str)
                       68 BINARY_SUBSCR
                       78 LOAD_CONST               5 ('as_var')
                       80 LOAD_NAME               10 (str)
                       82 BUILD_TUPLE              8
-                      84 LOAD_CONST               6 (<code object __init__, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 61>)
+                      84 LOAD_CONST               6 (<code object __init__, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 68>)
                       86 MAKE_FUNCTION            5 (defaults, annotations)
                       88 STORE_NAME              11 (__init__)
          
-          68          90 LOAD_CONST               7 (<code object _resolve_expressions, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 68>)
+          75          90 LOAD_CONST               7 (<code object _resolve_expressions, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 75>)
                       92 MAKE_FUNCTION            0
                       94 STORE_NAME              12 (_resolve_expressions)
          
-          78          96 LOAD_CONST               8 (<code object render, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 78>)
+          85          96 LOAD_CONST               8 (<code object render, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 85>)
                       98 MAKE_FUNCTION            0
                      100 STORE_NAME              13 (render)
                      102 LOAD_CONST               1 (None)
                      104 RETURN_VALUE
          consts
             'AdapterNode'
             None
@@ -429,46 +448,46 @@
                nlocals   : 6
                stacksize : 2
                flags     : 11
                code
                   0x97007c017c005f0000000000000000007c027c005f0100000000000000
                   007c037c005f0200000000000000007c057c005f0300000000000000007c
                   047c005f04000000000000000064005300
-                61           0 RESUME                   0
+                68           0 RESUME                   0
                
-                62           2 LOAD_FAST                1 (adapter)
+                69           2 LOAD_FAST                1 (adapter)
                              4 LOAD_FAST                0 (self)
                              6 STORE_ATTR               0 (adapter)
                
-                63          16 LOAD_FAST                2 (model)
+                70          16 LOAD_FAST                2 (model)
                             18 LOAD_FAST                0 (self)
                             20 STORE_ATTR               1 (model)
                
-                64          30 LOAD_FAST                3 (getters)
+                71          30 LOAD_FAST                3 (getters)
                             32 LOAD_FAST                0 (self)
                             34 STORE_ATTR               2 (getters)
                
-                65          44 LOAD_FAST                5 (kwargs)
+                72          44 LOAD_FAST                5 (kwargs)
                             46 LOAD_FAST                0 (self)
                             48 STORE_ATTR               3 (kwargs)
                
-                66          58 LOAD_FAST                4 (as_var)
+                73          58 LOAD_FAST                4 (as_var)
                             60 LOAD_FAST                0 (self)
                             62 STORE_ATTR               4 (as_var)
                             72 LOAD_CONST               0 (None)
                             74 RETURN_VALUE
                consts
                   None
                names      ('adapter', 'model', 'getters', 'kwargs', 'as_var')
                varnames   ('self', 'adapter', 'model', 'getters', 'as_var', 'kwargs')
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
+               filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
                name       '__init__'
-               firstlineno 61
+               firstlineno 68
                lnotab 0x02010e010e010e010e01
             code
                argcount  : 3
                nlocals   : 6
                stacksize : 5
                flags     : 11
                code
@@ -476,474 +495,487 @@
                   00ab00000000000000000044005d325c0200007d047d0574030000000000
                   00000000007c05740400000000000000000000a6020000ab020000000000
                   00000072187c05a00300000000000000000000000000000000000000007c
                   01a6010000ab0100000000000000007c037c043c0000008c337403000000
                   000000000000007c02740400000000000000000000a6020000ab02000000
                   000000000072157c02a00300000000000000000000000000000000000000
                   007c01a6010000ab0100000000000000007d027c027c0366025300
-                68           0 RESUME                   0
+                75           0 RESUME                   0
                
-                69           2 LOAD_FAST                3 (kwargs)
+                76           2 LOAD_FAST                3 (kwargs)
                              4 LOAD_METHOD              0 (items)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 GET_ITER
                        >>   42 FOR_ITER                50 (to 144)
                             44 UNPACK_SEQUENCE          2
                             48 STORE_FAST               4 (k)
                             50 STORE_FAST               5 (v)
                
-                70          52 LOAD_GLOBAL              3 (NULL + isinstance)
+                77          52 LOAD_GLOBAL              3 (NULL + isinstance)
                             64 LOAD_FAST                5 (v)
                             66 LOAD_GLOBAL              4 (FilterExpression)
                             78 PRECALL                  2
                             82 CALL                     2
                             92 POP_JUMP_FORWARD_IF_FALSE    24 (to 142)
                
-                71          94 LOAD_FAST                5 (v)
+                78          94 LOAD_FAST                5 (v)
                             96 LOAD_METHOD              3 (resolve)
                            118 LOAD_FAST                1 (context)
                            120 PRECALL                  1
                            124 CALL                     1
                            134 LOAD_FAST                3 (kwargs)
                            136 LOAD_FAST                4 (k)
                            138 STORE_SUBSCR
                        >>  142 JUMP_BACKWARD           51 (to 42)
                
-                73     >>  144 LOAD_GLOBAL              3 (NULL + isinstance)
+                80     >>  144 LOAD_GLOBAL              3 (NULL + isinstance)
                            156 LOAD_FAST                2 (model)
                            158 LOAD_GLOBAL              4 (FilterExpression)
                            170 PRECALL                  2
                            174 CALL                     2
                            184 POP_JUMP_FORWARD_IF_FALSE    21 (to 228)
                
-                74         186 LOAD_FAST                2 (model)
+                81         186 LOAD_FAST                2 (model)
                            188 LOAD_METHOD              3 (resolve)
                            210 LOAD_FAST                1 (context)
                            212 PRECALL                  1
                            216 CALL                     1
                            226 STORE_FAST               2 (model)
                
-                76     >>  228 LOAD_FAST                2 (model)
+                83     >>  228 LOAD_FAST                2 (model)
                            230 LOAD_FAST                3 (kwargs)
                            232 BUILD_TUPLE              2
                            234 RETURN_VALUE
                consts
                   None
                names      ('items', 'isinstance', 'FilterExpression', 'resolve')
                varnames   ('self', 'context', 'model', 'kwargs', 'k', 'v')
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
+               filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
                name       '_resolve_expressions'
-               firstlineno 68
+               firstlineno 75
                lnotab 0x020132012a0132022a012a02
             code
                argcount  : 2
-               nlocals   : 12
+               nlocals   : 13
                stacksize : 9
                flags     : 3
                code
                   0x97007c006a0000000000000000007d027c006a0100000000000000007d
                   0302007c006a0200000000000000007c017c02660269007c006a03000000
-                  0000000000a4018e015c0200007d027d0464017c017600722464027c0176
-                  0072207c02731e7c006a0400000000000000006a05000000000000000072
-                  127c016401190000000000000000007d057c016402190000000000000000
-                  007d0690016e3e7c02731c64027c01760072187c006a0400000000000000
-                  006a050000000000000000730c7c016402190000000000000000007d0664
-                  007d0590016e207c027398740d000000000000000000006a070000000000
-                  00000074100000000000000000000064037c006a0400000000000000006a
-                  09000000000000000069017a060000741400000000000000000000a60200
-                  00ab02000000000000000001007c01a00b00000000000000000000000000
-                  00000000000000a6000000ab0000000000000000007d0109007419000000
-                  000000000000007c006a0c00000000000000007c0102007c006a04000000
-                  00000000006a0d00000000000000007c01660169007c04a4018e01a60300
-                  00ab03000000000000000053002300741c00000000000000000000240072
-                  217d07741f000000000000000000007421000000000000000000007c07a6
+                  0000000000a4018e015c0200007d027d047408000000000000000000007c
+                  0176007233740a000000000000000000007c017600722a7c0273287c006a
+                  0600000000000000006a070000000000000000721c7c0174080000000000
+                  0000000000190000000000000000007d057c01740a000000000000000000
+                  00190000000000000000007d0690016e487c027326740a00000000000000
+                  0000007c017600721d7c006a0600000000000000006a0700000000000000
+                  0073117c01740a00000000000000000000190000000000000000007d0664
+                  007d0590016e207c0273987411000000000000000000006a090000000000
+                  00000074140000000000000000000064017c006a0600000000000000006a
+                  0b000000000000000069017a060000741800000000000000000000a60200
+                  00ab02000000000000000001007c01a00d00000000000000000000000000
+                  00000000000000a6000000ab0000000000000000007d010900741d000000
+                  000000000000007c006a0e00000000000000007c0102007c006a06000000
+                  00000000006a0f00000000000000007c01660169007c04a4018e01a60300
+                  00ab03000000000000000053002300742000000000000000000000240072
+                  217d077423000000000000000000007425000000000000000000007c07a6
                   010000ab010000000000000000a6010000ab010000000000000000820164
                   007d077e077701770078035900770164007d057c027d067c0372807c0374
-                  23000000000000000000007c03a6010000ab01000000000000000064047a
-                  0a0000190000000000000000007d05742500000000000000000000742300
-                  0000000000000000007c03a6010000ab01000000000000000064047a0a00
+                  27000000000000000000007c03a6010000ab01000000000000000064027a
+                  0a0000190000000000000000007d05742900000000000000000000742700
+                  0000000000000000007c03a6010000ab01000000000000000064027a0a00
                   00a6010000ab01000000000000000044005d487d087c037c081900000000
-                  00000000007d0909007427000000000000000000007c067c09a6020000ab
-                  0200000000000000007d068c1c2300742800000000000000000000240072
-                  20010074290000000000000000000064057c026a1500000000000000006a
-                  0900000000000000009b0064067c099b009d04a6010000ab010000000000
-                  000000820177007803590077017c01a01600000000000000000000000000
-                  000000000000006407a6010000ab0100000000000000007d0a02007c006a
-                  04000000000000000064097c067c057c0a64089c037c04a4018e017d0b7c
-                  0ba0170000000000000000000000000000000000000000a6000000ab0000
-                  0000000000000072107431000000000000000000007c0a7c06a6020000ab
-                  02000000000000000073627c01a019000000000000000000000000000000
-                  00000000007c0b6a030000000000000000a6010000ab0100000000000000
-                  0001007435000000000000000000007c06743600000000000000000000a6
-                  020000ab020000000000000000720a7c067c017438000000000000000000
-                  003c0000007419000000000000000000007c006a0c00000000000000007c
-                  017c0ba01d00000000000000000000000000000000000000007c01a60100
-                  00ab010000000000000000a6030000ab0300000000000000005300741900
-                  0000000000000000007c006a0c00000000000000007c01743d0000000000
-                  00000000007c0a7c0b7c01a6030000ab030000000000000000a6030000ab
-                  0300000000000000005300
-                78           0 RESUME                   0
+                  00000000007d090900742b000000000000000000007c067c09a6020000ab
+                  0200000000000000007d068c1c2300742c00000000000000000000240072
+                  20010074230000000000000000000064037c026a1700000000000000006a
+                  0b00000000000000009b0064047c099b009d04a6010000ab010000000000
+                  000000820177007803590077017c01a01800000000000000000000000000
+                  000000000000006405a6010000ab0100000000000000007d0a02007c006a
+                  06000000000000000064097c067c057c0a64069c037c04a4018e017d0b74
+                  33000000000000000000007c0b7c01a6020000ab0200000000000000007d
+                  0164007d0c7c0ba01a0000000000000000000000000000000000000000a6
+                  000000ab00000000000000000072247437000000000000000000007c0a7c
+                  06a6020000ab02000000000000000072147439000000000000000000007c
+                  0a7c0b7c016407ac08a6040000ab0400000000000000007d0c6e24743b00
+                  0000000000000000007c01a6010000ab01000000000000000001007c0ba0
+                  1e00000000000000000000000000000000000000007c01a6010000ab0100
+                  000000000000007d0c741d000000000000000000007c006a0e0000000000
+                  0000007c017c0ca6030000ab0300000000000000005300
+                85           0 RESUME                   0
                
-                79           2 LOAD_FAST                0 (self)
+                86           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (model)
                             14 STORE_FAST               2 (model)
                
-                80          16 LOAD_FAST                0 (self)
+                87          16 LOAD_FAST                0 (self)
                             18 LOAD_ATTR                1 (getters)
                             28 STORE_FAST               3 (getters)
                
-                82          30 PUSH_NULL
+                89          30 PUSH_NULL
                             32 LOAD_FAST                0 (self)
                             34 LOAD_ATTR                2 (_resolve_expressions)
                
-                83          44 LOAD_FAST                1 (context)
+                90          44 LOAD_FAST                1 (context)
                             46 LOAD_FAST                2 (model)
                
-                82          48 BUILD_TUPLE              2
+                89          48 BUILD_TUPLE              2
                             50 BUILD_MAP                0
                
-                83          52 LOAD_FAST                0 (self)
+                90          52 LOAD_FAST                0 (self)
                             54 LOAD_ATTR                3 (kwargs)
                
-                82          64 DICT_MERGE               1
+                89          64 DICT_MERGE               1
                             66 CALL_FUNCTION_EX         1
                             68 UNPACK_SEQUENCE          2
                             72 STORE_FAST               2 (model)
                             74 STORE_FAST               4 (kwargs)
                
-                86          76 LOAD_CONST               1 ('wagtail_fedit_field')
-                            78 LOAD_FAST                1 (context)
-                            80 CONTAINS_OP              0
-                            82 POP_JUMP_FORWARD_IF_FALSE    36 (to 156)
-               
-                87          84 LOAD_CONST               2 ('wagtail_fedit_instance')
-                            86 LOAD_FAST                1 (context)
-                            88 CONTAINS_OP              0
-                            90 POP_JUMP_FORWARD_IF_FALSE    32 (to 156)
-               
-                88          92 LOAD_FAST                2 (model)
-               
-                87          94 POP_JUMP_FORWARD_IF_TRUE    30 (to 156)
-               
-                88          96 LOAD_FAST                0 (self)
-                            98 LOAD_ATTR                4 (adapter)
-                           108 LOAD_ATTR                5 (field_required)
-               
-                87         118 POP_JUMP_FORWARD_IF_FALSE    18 (to 156)
-               
-                90         120 LOAD_FAST                1 (context)
-                           122 LOAD_CONST               1 ('wagtail_fedit_field')
-                           124 BINARY_SUBSCR
-                           134 STORE_FAST               5 (field_name)
-               
-                91         136 LOAD_FAST                1 (context)
-                           138 LOAD_CONST               2 ('wagtail_fedit_instance')
-                           140 BINARY_SUBSCR
-                           150 STORE_FAST               6 (obj)
-                           152 EXTENDED_ARG             1
-                           154 JUMP_FORWARD           318 (to 792)
-               
-                93     >>  156 LOAD_FAST                2 (model)
-                           158 POP_JUMP_FORWARD_IF_TRUE    28 (to 216)
-                           160 LOAD_CONST               2 ('wagtail_fedit_instance')
-                           162 LOAD_FAST                1 (context)
-                           164 CONTAINS_OP              0
-                           166 POP_JUMP_FORWARD_IF_FALSE    24 (to 216)
-                           168 LOAD_FAST                0 (self)
-                           170 LOAD_ATTR                4 (adapter)
-                           180 LOAD_ATTR                5 (field_required)
-                           190 POP_JUMP_FORWARD_IF_TRUE    12 (to 216)
-               
-                94         192 LOAD_FAST                1 (context)
-                           194 LOAD_CONST               2 ('wagtail_fedit_instance')
-                           196 BINARY_SUBSCR
-                           206 STORE_FAST               6 (obj)
-               
-                95         208 LOAD_CONST               0 (None)
-                           210 STORE_FAST               5 (field_name)
-                           212 EXTENDED_ARG             1
-                           214 JUMP_FORWARD           288 (to 792)
-               
-                99     >>  216 LOAD_FAST                2 (model)
-                           218 POP_JUMP_FORWARD_IF_TRUE   152 (to 524)
-               
-               100         220 LOAD_GLOBAL             13 (NULL + warnings)
-                           232 LOAD_ATTR                7 (warn)
-               
-               101         242 LOAD_GLOBAL             16 (WARNING_MODEL_INSTANCE_NOT_AVAILABLE)
-               
-               102         254 LOAD_CONST               3 ('object')
-                           256 LOAD_FAST                0 (self)
-                           258 LOAD_ATTR                4 (adapter)
-                           268 LOAD_ATTR                9 (__name__)
-               
-               101         278 BUILD_MAP                1
-                           280 BINARY_OP                6 (%)
-               
-               104         284 LOAD_GLOBAL             20 (RuntimeWarning)
-               
-               100         296 PRECALL                  2
-                           300 CALL                     2
-                           310 POP_TOP
-               
-               107         312 LOAD_FAST                1 (context)
-                           314 LOAD_METHOD             11 (flatten)
-                           336 PRECALL                  0
-                           340 CALL                     0
-                           350 STORE_FAST               1 (context)
-               
-               109         352 NOP
-               
-               110         354 LOAD_GLOBAL             25 (NULL + as_var)
-                           366 LOAD_FAST                0 (self)
-                           368 LOAD_ATTR               12 (as_var)
-                           378 LOAD_FAST                1 (context)
-                           380 PUSH_NULL
-                           382 LOAD_FAST                0 (self)
-                           384 LOAD_ATTR                4 (adapter)
-                           394 LOAD_ATTR               13 (render_from_kwargs)
-               
-               111         404 LOAD_FAST                1 (context)
-               
-               110         406 BUILD_TUPLE              1
-                           408 BUILD_MAP                0
-               
-               111         410 LOAD_FAST                4 (kwargs)
-               
-               110         412 DICT_MERGE               1
-                           414 CALL_FUNCTION_EX         1
-                           416 PRECALL                  3
-                           420 CALL                     3
-                           430 RETURN_VALUE
-                       >>  432 PUSH_EXC_INFO
-               
-               113         434 LOAD_GLOBAL             28 (AdapterError)
-                           446 CHECK_EXC_MATCH
-                           448 POP_JUMP_FORWARD_IF_FALSE    33 (to 516)
-                           450 STORE_FAST               7 (e)
-               
-               114         452 LOAD_GLOBAL             31 (NULL + TemplateSyntaxError)
-                           464 LOAD_GLOBAL             33 (NULL + str)
-                           476 LOAD_FAST                7 (e)
-                           478 PRECALL                  1
-                           482 CALL                     1
-                           492 PRECALL                  1
-                           496 CALL                     1
-                           506 RAISE_VARARGS            1
-                       >>  508 LOAD_CONST               0 (None)
+                93          76 LOAD_GLOBAL              8 (FIELD_TEMPLATE_VAR)
+                            88 LOAD_FAST                1 (context)
+                            90 CONTAINS_OP              0
+                            92 POP_JUMP_FORWARD_IF_FALSE    51 (to 196)
+               
+                94          94 LOAD_GLOBAL             10 (INSTANCE_TEMPLATE_VAR)
+                           106 LOAD_FAST                1 (context)
+                           108 CONTAINS_OP              0
+                           110 POP_JUMP_FORWARD_IF_FALSE    42 (to 196)
+               
+                95         112 LOAD_FAST                2 (model)
+               
+                94         114 POP_JUMP_FORWARD_IF_TRUE    40 (to 196)
+               
+                95         116 LOAD_FAST                0 (self)
+                           118 LOAD_ATTR                6 (adapter)
+                           128 LOAD_ATTR                7 (field_required)
+               
+                94         138 POP_JUMP_FORWARD_IF_FALSE    28 (to 196)
+               
+                97         140 LOAD_FAST                1 (context)
+                           142 LOAD_GLOBAL              8 (FIELD_TEMPLATE_VAR)
+                           154 BINARY_SUBSCR
+                           164 STORE_FAST               5 (field_name)
+               
+                98         166 LOAD_FAST                1 (context)
+                           168 LOAD_GLOBAL             10 (INSTANCE_TEMPLATE_VAR)
+                           180 BINARY_SUBSCR
+                           190 STORE_FAST               6 (obj)
+                           192 EXTENDED_ARG             1
+                           194 JUMP_FORWARD           328 (to 852)
+               
+               100     >>  196 LOAD_FAST                2 (model)
+                           198 POP_JUMP_FORWARD_IF_TRUE    38 (to 276)
+               
+               101         200 LOAD_GLOBAL             10 (INSTANCE_TEMPLATE_VAR)
+                           212 LOAD_FAST                1 (context)
+                           214 CONTAINS_OP              0
+                           216 POP_JUMP_FORWARD_IF_FALSE    29 (to 276)
+               
+               102         218 LOAD_FAST                0 (self)
+                           220 LOAD_ATTR                6 (adapter)
+                           230 LOAD_ATTR                7 (field_required)
+               
+               101         240 POP_JUMP_FORWARD_IF_TRUE    17 (to 276)
+               
+               103         242 LOAD_FAST                1 (context)
+                           244 LOAD_GLOBAL             10 (INSTANCE_TEMPLATE_VAR)
+                           256 BINARY_SUBSCR
+                           266 STORE_FAST               6 (obj)
+               
+               104         268 LOAD_CONST               0 (None)
+                           270 STORE_FAST               5 (field_name)
+                           272 EXTENDED_ARG             1
+                           274 JUMP_FORWARD           288 (to 852)
+               
+               108     >>  276 LOAD_FAST                2 (model)
+                           278 POP_JUMP_FORWARD_IF_TRUE   152 (to 584)
+               
+               109         280 LOAD_GLOBAL             17 (NULL + warnings)
+                           292 LOAD_ATTR                9 (warn)
+               
+               110         302 LOAD_GLOBAL             20 (WARNING_MODEL_INSTANCE_NOT_AVAILABLE)
+               
+               111         314 LOAD_CONST               1 ('object')
+                           316 LOAD_FAST                0 (self)
+                           318 LOAD_ATTR                6 (adapter)
+                           328 LOAD_ATTR               11 (__name__)
+               
+               110         338 BUILD_MAP                1
+                           340 BINARY_OP                6 (%)
+               
+               113         344 LOAD_GLOBAL             24 (RuntimeWarning)
+               
+               109         356 PRECALL                  2
+                           360 CALL                     2
+                           370 POP_TOP
+               
+               116         372 LOAD_FAST                1 (context)
+                           374 LOAD_METHOD             13 (flatten)
+                           396 PRECALL                  0
+                           400 CALL                     0
+                           410 STORE_FAST               1 (context)
+               
+               118         412 NOP
+               
+               119         414 LOAD_GLOBAL             29 (NULL + as_var)
+                           426 LOAD_FAST                0 (self)
+                           428 LOAD_ATTR               14 (as_var)
+                           438 LOAD_FAST                1 (context)
+                           440 PUSH_NULL
+                           442 LOAD_FAST                0 (self)
+                           444 LOAD_ATTR                6 (adapter)
+                           454 LOAD_ATTR               15 (render_from_kwargs)
+               
+               120         464 LOAD_FAST                1 (context)
+               
+               119         466 BUILD_TUPLE              1
+                           468 BUILD_MAP                0
+               
+               120         470 LOAD_FAST                4 (kwargs)
+               
+               119         472 DICT_MERGE               1
+                           474 CALL_FUNCTION_EX         1
+                           476 PRECALL                  3
+                           480 CALL                     3
+                           490 RETURN_VALUE
+                       >>  492 PUSH_EXC_INFO
+               
+               122         494 LOAD_GLOBAL             32 (AdapterError)
+                           506 CHECK_EXC_MATCH
+                           508 POP_JUMP_FORWARD_IF_FALSE    33 (to 576)
                            510 STORE_FAST               7 (e)
-                           512 DELETE_FAST              7 (e)
-                           514 RERAISE                  1
                
-               113     >>  516 RERAISE                  0
-                       >>  518 COPY                     3
-                           520 POP_EXCEPT
-                           522 RERAISE                  1
-               
-               116     >>  524 LOAD_CONST               0 (None)
-                           526 STORE_FAST               5 (field_name)
-               
-               117         528 LOAD_FAST                2 (model)
-                           530 STORE_FAST               6 (obj)
-               
-               118         532 LOAD_FAST                3 (getters)
-                           534 POP_JUMP_FORWARD_IF_FALSE   128 (to 792)
-               
-               119         536 LOAD_FAST                3 (getters)
-                           538 LOAD_GLOBAL             35 (NULL + len)
-                           550 LOAD_FAST                3 (getters)
+               123         512 LOAD_GLOBAL             35 (NULL + TemplateSyntaxError)
+                           524 LOAD_GLOBAL             37 (NULL + str)
+                           536 LOAD_FAST                7 (e)
+                           538 PRECALL                  1
+                           542 CALL                     1
                            552 PRECALL                  1
                            556 CALL                     1
-                           566 LOAD_CONST               4 (1)
-                           568 BINARY_OP               10 (-)
-                           572 BINARY_SUBSCR
-                           582 STORE_FAST               5 (field_name)
-               
-               121         584 LOAD_GLOBAL             37 (NULL + range)
-                           596 LOAD_GLOBAL             35 (NULL + len)
-                           608 LOAD_FAST                3 (getters)
-                           610 PRECALL                  1
-                           614 CALL                     1
-                           624 LOAD_CONST               4 (1)
-                           626 BINARY_OP               10 (-)
-                           630 PRECALL                  1
-                           634 CALL                     1
-                           644 GET_ITER
-                       >>  646 FOR_ITER                72 (to 792)
-                           648 STORE_FAST               8 (i)
-               
-               122         650 LOAD_FAST                3 (getters)
-                           652 LOAD_FAST                8 (i)
-                           654 BINARY_SUBSCR
-                           664 STORE_FAST               9 (getter)
-               
-               123         666 NOP
-               
-               124         668 LOAD_GLOBAL             39 (NULL + getattr)
-                           680 LOAD_FAST                6 (obj)
-                           682 LOAD_FAST                9 (getter)
-                           684 PRECALL                  2
-                           688 CALL                     2
-                           698 STORE_FAST               6 (obj)
-                           700 JUMP_BACKWARD           28 (to 646)
-                       >>  702 PUSH_EXC_INFO
-               
-               125         704 LOAD_GLOBAL             40 (AttributeError)
-                           716 CHECK_EXC_MATCH
-                           718 POP_JUMP_FORWARD_IF_FALSE    32 (to 784)
-                           720 POP_TOP
-               
-               126         722 LOAD_GLOBAL             41 (NULL + AttributeError)
-                           734 LOAD_CONST               5 ('Object ')
-                           736 LOAD_FAST                2 (model)
-                           738 LOAD_ATTR               21 (__class__)
-                           748 LOAD_ATTR                9 (__name__)
-                           758 FORMAT_VALUE             0
-                           760 LOAD_CONST               6 (' does not have attribute ')
-                           762 LOAD_FAST                9 (getter)
-                           764 FORMAT_VALUE             0
-                           766 BUILD_STRING             4
-                           768 PRECALL                  1
-                           772 CALL                     1
-                           782 RAISE_VARARGS            1
-               
-               125     >>  784 RERAISE                  0
-                       >>  786 COPY                     3
-                           788 POP_EXCEPT
-                           790 RERAISE                  1
-               
-               129     >>  792 LOAD_FAST                1 (context)
-                           794 LOAD_METHOD             22 (get)
-                           816 LOAD_CONST               7 ('request')
-                           818 PRECALL                  1
-                           822 CALL                     1
-                           832 STORE_FAST              10 (request)
-               
-               130         834 PUSH_NULL
-                           836 LOAD_FAST                0 (self)
-                           838 LOAD_ATTR                4 (adapter)
-                           848 LOAD_CONST               9 (())
-               
-               131         850 LOAD_FAST                6 (obj)
-               
-               132         852 LOAD_FAST                5 (field_name)
-               
-               133         854 LOAD_FAST               10 (request)
-               
-               130         856 LOAD_CONST               8 (('object', 'field_name', 'request'))
-                           858 BUILD_CONST_KEY_MAP      3
-               
-               134         860 LOAD_FAST                4 (kwargs)
-               
-               130         862 DICT_MERGE               1
-                           864 CALL_FUNCTION_EX         1
-                           866 STORE_FAST              11 (adapter)
-               
-               137         868 LOAD_FAST               11 (adapter)
-                           870 LOAD_METHOD             23 (check_permissions)
-                           892 PRECALL                  0
-                           896 CALL                     0
-                           906 POP_JUMP_FORWARD_IF_FALSE    16 (to 940)
-               
-               138         908 LOAD_GLOBAL             49 (NULL + _can_edit)
-                           920 LOAD_FAST               10 (request)
-                           922 LOAD_FAST                6 (obj)
-                           924 PRECALL                  2
-                           928 CALL                     2
-               
-               137         938 POP_JUMP_FORWARD_IF_TRUE    98 (to 1136)
-               
-               139     >>  940 LOAD_FAST                1 (context)
-                           942 LOAD_METHOD             25 (update)
-                           964 LOAD_FAST               11 (adapter)
-                           966 LOAD_ATTR                3 (kwargs)
-                           976 PRECALL                  1
-                           980 CALL                     1
-                           990 POP_TOP
-               
-               141         992 LOAD_GLOBAL             53 (NULL + isinstance)
-                          1004 LOAD_FAST                6 (obj)
-                          1006 LOAD_GLOBAL             54 (Page)
-                          1018 PRECALL                  2
-                          1022 CALL                     2
-                          1032 POP_JUMP_FORWARD_IF_FALSE    10 (to 1054)
-               
-               142        1034 LOAD_FAST                6 (obj)
-                          1036 LOAD_FAST                1 (context)
-                          1038 LOAD_GLOBAL             56 (PAGE_TEMPLATE_VAR)
-                          1050 STORE_SUBSCR
-               
-               144     >> 1054 LOAD_GLOBAL             25 (NULL + as_var)
-                          1066 LOAD_FAST                0 (self)
-                          1068 LOAD_ATTR               12 (as_var)
-                          1078 LOAD_FAST                1 (context)
-                          1080 LOAD_FAST               11 (adapter)
-                          1082 LOAD_METHOD             29 (render_content)
-                          1104 LOAD_FAST                1 (context)
-                          1106 PRECALL                  1
-                          1110 CALL                     1
-                          1120 PRECALL                  3
-                          1124 CALL                     3
-                          1134 RETURN_VALUE
-               
-               146     >> 1136 LOAD_GLOBAL             25 (NULL + as_var)
-                          1148 LOAD_FAST                0 (self)
-                          1150 LOAD_ATTR               12 (as_var)
-                          1160 LOAD_FAST                1 (context)
-                          1162 LOAD_GLOBAL             61 (NULL + wrap_adapter)
-                          1174 LOAD_FAST               10 (request)
-                          1176 LOAD_FAST               11 (adapter)
-                          1178 LOAD_FAST                1 (context)
-                          1180 PRECALL                  3
-                          1184 CALL                     3
-                          1194 PRECALL                  3
-                          1198 CALL                     3
-                          1208 RETURN_VALUE
+                           566 RAISE_VARARGS            1
+                       >>  568 LOAD_CONST               0 (None)
+                           570 STORE_FAST               7 (e)
+                           572 DELETE_FAST              7 (e)
+                           574 RERAISE                  1
+               
+               122     >>  576 RERAISE                  0
+                       >>  578 COPY                     3
+                           580 POP_EXCEPT
+                           582 RERAISE                  1
+               
+               125     >>  584 LOAD_CONST               0 (None)
+                           586 STORE_FAST               5 (field_name)
+               
+               126         588 LOAD_FAST                2 (model)
+                           590 STORE_FAST               6 (obj)
+               
+               127         592 LOAD_FAST                3 (getters)
+                           594 POP_JUMP_FORWARD_IF_FALSE   128 (to 852)
+               
+               128         596 LOAD_FAST                3 (getters)
+                           598 LOAD_GLOBAL             39 (NULL + len)
+                           610 LOAD_FAST                3 (getters)
+                           612 PRECALL                  1
+                           616 CALL                     1
+                           626 LOAD_CONST               2 (1)
+                           628 BINARY_OP               10 (-)
+                           632 BINARY_SUBSCR
+                           642 STORE_FAST               5 (field_name)
+               
+               130         644 LOAD_GLOBAL             41 (NULL + range)
+                           656 LOAD_GLOBAL             39 (NULL + len)
+                           668 LOAD_FAST                3 (getters)
+                           670 PRECALL                  1
+                           674 CALL                     1
+                           684 LOAD_CONST               2 (1)
+                           686 BINARY_OP               10 (-)
+                           690 PRECALL                  1
+                           694 CALL                     1
+                           704 GET_ITER
+                       >>  706 FOR_ITER                72 (to 852)
+                           708 STORE_FAST               8 (i)
+               
+               131         710 LOAD_FAST                3 (getters)
+                           712 LOAD_FAST                8 (i)
+                           714 BINARY_SUBSCR
+                           724 STORE_FAST               9 (getter)
+               
+               132         726 NOP
+               
+               133         728 LOAD_GLOBAL             43 (NULL + getattr)
+                           740 LOAD_FAST                6 (obj)
+                           742 LOAD_FAST                9 (getter)
+                           744 PRECALL                  2
+                           748 CALL                     2
+                           758 STORE_FAST               6 (obj)
+                           760 JUMP_BACKWARD           28 (to 706)
+                       >>  762 PUSH_EXC_INFO
+               
+               134         764 LOAD_GLOBAL             44 (AttributeError)
+                           776 CHECK_EXC_MATCH
+                           778 POP_JUMP_FORWARD_IF_FALSE    32 (to 844)
+                           780 POP_TOP
+               
+               135         782 LOAD_GLOBAL             35 (NULL + TemplateSyntaxError)
+                           794 LOAD_CONST               3 ('Object ')
+                           796 LOAD_FAST                2 (model)
+                           798 LOAD_ATTR               23 (__class__)
+                           808 LOAD_ATTR               11 (__name__)
+                           818 FORMAT_VALUE             0
+                           820 LOAD_CONST               4 (' does not have attribute ')
+                           822 LOAD_FAST                9 (getter)
+                           824 FORMAT_VALUE             0
+                           826 BUILD_STRING             4
+                           828 PRECALL                  1
+                           832 CALL                     1
+                           842 RAISE_VARARGS            1
+               
+               134     >>  844 RERAISE                  0
+                       >>  846 COPY                     3
+                           848 POP_EXCEPT
+                           850 RERAISE                  1
+               
+               138     >>  852 LOAD_FAST                1 (context)
+                           854 LOAD_METHOD             24 (get)
+                           876 LOAD_CONST               5 ('request')
+                           878 PRECALL                  1
+                           882 CALL                     1
+                           892 STORE_FAST              10 (request)
+               
+               139         894 PUSH_NULL
+                           896 LOAD_FAST                0 (self)
+                           898 LOAD_ATTR                6 (adapter)
+                           908 LOAD_CONST               9 (())
+               
+               140         910 LOAD_FAST                6 (obj)
+               
+               141         912 LOAD_FAST                5 (field_name)
+               
+               142         914 LOAD_FAST               10 (request)
+               
+               139         916 LOAD_CONST               6 (('object', 'field_name', 'request'))
+                           918 BUILD_CONST_KEY_MAP      3
+               
+               143         920 LOAD_FAST                4 (kwargs)
+               
+               139         922 DICT_MERGE               1
+                           924 CALL_FUNCTION_EX         1
+                           926 STORE_FAST              11 (adapter)
+               
+               146         928 LOAD_GLOBAL             51 (NULL + base_adapter_context)
+               
+               147         940 LOAD_FAST               11 (adapter)
+               
+               148         942 LOAD_FAST                1 (context)
+               
+               146         944 PRECALL                  2
+                           948 CALL                     2
+                           958 STORE_FAST               1 (context)
+               
+               151         960 LOAD_CONST               0 (None)
+                           962 STORE_FAST              12 (content)
+               
+               152         964 LOAD_FAST               11 (adapter)
+                           966 LOAD_METHOD             26 (check_permissions)
+                           988 PRECALL                  0
+                           992 CALL                     0
+                          1002 POP_JUMP_FORWARD_IF_FALSE    36 (to 1076)
+               
+               153        1004 LOAD_GLOBAL             55 (NULL + _can_edit)
+                          1016 LOAD_FAST               10 (request)
+                          1018 LOAD_FAST                6 (obj)
+                          1020 PRECALL                  2
+                          1024 CALL                     2
+               
+               152        1034 POP_JUMP_FORWARD_IF_FALSE    20 (to 1076)
+               
+               154        1036 LOAD_GLOBAL             57 (NULL + wrap_adapter)
+               
+               155        1048 LOAD_FAST               10 (request)
+               
+               156        1050 LOAD_FAST               11 (adapter)
+               
+               157        1052 LOAD_FAST                1 (context)
+               
+               158        1054 LOAD_CONST               7 (False)
+               
+               154        1056 KW_NAMES                 8
+                          1058 PRECALL                  4
+                          1062 CALL                     4
+                          1072 STORE_FAST              12 (content)
+                          1074 JUMP_FORWARD            36 (to 1148)
+               
+               162     >> 1076 LOAD_GLOBAL             59 (NULL + _flatten_context)
+                          1088 LOAD_FAST                1 (context)
+                          1090 PRECALL                  1
+                          1094 CALL                     1
+                          1104 POP_TOP
+               
+               163        1106 LOAD_FAST               11 (adapter)
+                          1108 LOAD_METHOD             30 (render_content)
+               
+               164        1130 LOAD_FAST                1 (context)
+               
+               163        1132 PRECALL                  1
+                          1136 CALL                     1
+                          1146 STORE_FAST              12 (content)
+               
+               167     >> 1148 LOAD_GLOBAL             29 (NULL + as_var)
+               
+               168        1160 LOAD_FAST                0 (self)
+                          1162 LOAD_ATTR               14 (as_var)
+               
+               169        1172 LOAD_FAST                1 (context)
+               
+               170        1174 LOAD_FAST               12 (content)
+               
+               167        1176 PRECALL                  3
+                          1180 CALL                     3
+                          1190 RETURN_VALUE
                ExceptionTable:
-                 354 to 428 -> 432 [0]
-                 432 to 450 -> 518 [1] lasti
-                 452 to 506 -> 508 [1] lasti
-                 508 to 516 -> 518 [1] lasti
-                 668 to 698 -> 702 [1]
-                 702 to 784 -> 786 [2] lasti
+                 414 to 488 -> 492 [0]
+                 492 to 510 -> 578 [1] lasti
+                 512 to 566 -> 568 [1] lasti
+                 568 to 576 -> 578 [1] lasti
+                 728 to 758 -> 762 [1]
+                 762 to 844 -> 846 [2] lasti
                consts
                   None
-                  'wagtail_fedit_field'
-                  'wagtail_fedit_instance'
                   'object'
                   1
                   'Object '
                   ' does not have attribute '
                   'request'
                   ('object', 'field_name', 'request')
+                  False
+                  ('request', 'adapter', 'context', 'run_context_processors')
                   ()
-               names      ('model', 'getters', '_resolve_expressions', 'kwargs', 'adapter', 'field_required', 'warnings', 'warn', 'WARNING_MODEL_INSTANCE_NOT_AVAILABLE', '__name__', 'RuntimeWarning', 'flatten', 'as_var', 'render_from_kwargs', 'AdapterError', 'TemplateSyntaxError', 'str', 'len', 'range', 'getattr', 'AttributeError', '__class__', 'get', 'check_permissions', '_can_edit', 'update', 'isinstance', 'Page', 'PAGE_TEMPLATE_VAR', 'render_content', 'wrap_adapter')
-               varnames   ('self', 'context', 'model', 'getters', 'kwargs', 'field_name', 'obj', 'e', 'i', 'getter', 'request', 'adapter')
+               names      ('model', 'getters', '_resolve_expressions', 'kwargs', 'FIELD_TEMPLATE_VAR', 'INSTANCE_TEMPLATE_VAR', 'adapter', 'field_required', 'warnings', 'warn', 'WARNING_MODEL_INSTANCE_NOT_AVAILABLE', '__name__', 'RuntimeWarning', 'flatten', 'as_var', 'render_from_kwargs', 'AdapterError', 'TemplateSyntaxError', 'str', 'len', 'range', 'getattr', 'AttributeError', '__class__', 'get', 'base_adapter_context', 'check_permissions', '_can_edit', 'wrap_adapter', '_flatten_context', 'render_content')
+               varnames   ('self', 'context', 'model', 'getters', 'kwargs', 'field_name', 'obj', 'e', 'i', 'getter', 'request', 'adapter', 'content')
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
+               filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
                name       'render'
-               firstlineno 78
+               firstlineno 85
                lnotab
-                  0x02010e010e020e0104ff04010cff0c040801080102ff020116ff020310
-                  011402240110010804040116010c0118ff06030cfc100728020201320102
-                  ff040102ff1603120140ff08030401040104013002420110010201240112
-                  013eff08042a0110010201020102fd040402fc060728011eff020234022a
-                  0114025202
+                  0x02010e010e020e0104ff04010cff0c041201120102ff020116ff02031a
+                  011e020401120116ff02021a010804040116010c0118ff06030cfc100728
+                  020201320102ff040102ff1603120140ff08030401040104013002420110
+                  010201240112013eff08042a0110010201020102fd040402fc06070c0102
+                  0102fe1005040128011eff02020c0102010201020102fc14081e01180102
+                  ff10040c010c01020102fd
             (None,)
          names      ('__name__', '__module__', '__qualname__', 'signing', 'TimestampSigner', 'signer', 'Type', 'BaseAdapter', 'FilterExpression', 'list', 'str', '__init__', '_resolve_expressions', 'render')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
+         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
          name       'AdapterNode'
-         firstlineno 58
+         firstlineno 65
          lnotab 0x0a011e023207060a
       'AdapterNode'
       ('name',)
       'parser'
       'token'
       code
          argcount  : 2
@@ -974,224 +1006,221 @@
             00000000007c02a6010000ab01000000000000000064067a0a0000190000
             00000000000000640a6b0200000000724a7c02a001000000000000000000
             0000000000000000000000740d000000000000000000007c02a6010000ab
             01000000000000000064097a0a0000a6010000ab0100000000000000007d
             097c02a0010000000000000000000000000000000000000000740d000000
             000000000000007c02a6010000ab01000000000000000064097a0a0000a6
             010000ab01000000000000000001007413000000000000000000007c007c
-            027c056a0a00000000000000007c056a0b00000000000000007c056a0c00
-            00000000000000a6050000ab0500000000000000007d0a741b0000000000
-            0000000000640c7c057c067c077c09640b9c047c0aa4018e015300
-         149           0 RESUME                   0
+            027c056a0a00000000000000007c056a0b0000000000000000a6040000ab
+            0400000000000000007d0a741900000000000000000000640c7c057c067c
+            077c09640b9c047c0aa4018e015300
+         174           0 RESUME                   0
          
-         152           2 LOAD_FAST                1 (token)
+         177           2 LOAD_FAST                1 (token)
                        4 LOAD_METHOD              0 (split_contents)
                       26 PRECALL                  0
                       30 CALL                     0
                       40 STORE_FAST               2 (tokens)
          
-         154          42 LOAD_FAST                2 (tokens)
+         179          42 LOAD_FAST                2 (tokens)
                       44 LOAD_METHOD              1 (pop)
                       66 LOAD_CONST               1 (0)
                       68 PRECALL                  1
                       72 CALL                     1
                       82 STORE_FAST               3 (_)
          
-         155          84 LOAD_FAST                2 (tokens)
+         180          84 LOAD_FAST                2 (tokens)
                       86 LOAD_METHOD              1 (pop)
                      108 LOAD_CONST               1 (0)
                      110 PRECALL                  1
                      114 CALL                     1
                      124 STORE_FAST               4 (adapter_id)
          
-         157         126 NOP
+         182         126 NOP
          
-         158         128 LOAD_GLOBAL              4 (adapter_registry)
+         183         128 LOAD_GLOBAL              4 (adapter_registry)
                      140 LOAD_FAST                4 (adapter_id)
                      142 BINARY_SUBSCR
                      152 STORE_FAST               5 (adapter)
                      154 JUMP_FORWARD            33 (to 222)
                  >>  156 PUSH_EXC_INFO
          
-         159         158 LOAD_GLOBAL              6 (RegistryLookUpError)
+         184         158 LOAD_GLOBAL              6 (RegistryLookUpError)
                      170 CHECK_EXC_MATCH
                      172 POP_JUMP_FORWARD_IF_FALSE    20 (to 214)
                      174 POP_TOP
          
-         160         176 LOAD_GLOBAL              9 (NULL + TemplateSyntaxError)
+         185         176 LOAD_GLOBAL              9 (NULL + TemplateSyntaxError)
                      188 LOAD_CONST               2 ("No adapter found with identifier '")
                      190 LOAD_FAST                4 (adapter_id)
                      192 FORMAT_VALUE             0
                      194 LOAD_CONST               3 ("'")
                      196 BUILD_STRING             3
                      198 PRECALL                  1
                      202 CALL                     1
                      212 RAISE_VARARGS            1
          
-         159     >>  214 RERAISE                  0
+         184     >>  214 RERAISE                  0
                  >>  216 COPY                     3
                      218 POP_EXCEPT
                      220 RERAISE                  1
          
-         162     >>  222 LOAD_CONST               4 ((None, None))
+         187     >>  222 LOAD_CONST               4 ((None, None))
                      224 UNPACK_SEQUENCE          2
                      228 STORE_FAST               6 (model)
                      230 STORE_FAST               7 (model_tokens)
          
-         163         232 LOAD_FAST                2 (tokens)
+         188         232 LOAD_FAST                2 (tokens)
                      234 POP_JUMP_FORWARD_IF_FALSE   173 (to 582)
          
-         164         236 LOAD_FAST                2 (tokens)
+         189         236 LOAD_FAST                2 (tokens)
                      238 LOAD_METHOD              1 (pop)
                      260 LOAD_CONST               1 (0)
                      262 PRECALL                  1
                      266 CALL                     1
                      276 STORE_FAST               8 (model__field)
          
-         165         278 LOAD_FAST                8 (model__field)
+         190         278 LOAD_FAST                8 (model__field)
                      280 LOAD_METHOD              5 (split)
                      302 LOAD_CONST               5 ('.')
                      304 PRECALL                  1
                      308 CALL                     1
                      318 STORE_FAST               7 (model_tokens)
          
-         169         320 LOAD_GLOBAL             13 (NULL + len)
+         194         320 LOAD_GLOBAL             13 (NULL + len)
                      332 LOAD_FAST                7 (model_tokens)
                      334 PRECALL                  1
                      338 CALL                     1
                      348 LOAD_CONST               6 (2)
                      350 COMPARE_OP               0 (<)
                      356 POP_JUMP_FORWARD_IF_FALSE    34 (to 426)
          
-         170         358 LOAD_FAST                7 (model_tokens)
+         195         358 LOAD_FAST                7 (model_tokens)
                      360 LOAD_CONST               1 (0)
                      362 BINARY_SUBSCR
                      372 LOAD_CONST               7 ('from_context')
                      374 COMPARE_OP               3 (!=)
                      380 POP_JUMP_FORWARD_IF_FALSE    22 (to 426)
                      382 LOAD_FAST                5 (adapter)
                      384 LOAD_ATTR                7 (field_required)
                      394 POP_JUMP_FORWARD_IF_FALSE    15 (to 426)
          
-         171         396 LOAD_GLOBAL              9 (NULL + TemplateSyntaxError)
+         196         396 LOAD_GLOBAL              9 (NULL + TemplateSyntaxError)
          
-         172         408 LOAD_CONST               8 ("Model and field name are required: 'mymodel.myfield' or 'from_context'")
+         197         408 LOAD_CONST               8 ("Model and field name are required: 'mymodel.myfield' or 'from_context'")
          
-         171         410 PRECALL                  1
+         196         410 PRECALL                  1
                      414 CALL                     1
                      424 RAISE_VARARGS            1
          
-         176     >>  426 LOAD_GLOBAL             13 (NULL + len)
+         201     >>  426 LOAD_GLOBAL             13 (NULL + len)
                      438 LOAD_FAST                7 (model_tokens)
                      440 PRECALL                  1
                      444 CALL                     1
                      454 LOAD_CONST               9 (1)
                      456 COMPARE_OP               4 (>)
                      462 POP_JUMP_FORWARD_IF_TRUE    19 (to 502)
          
-         177         464 LOAD_FAST                7 (model_tokens)
+         202         464 LOAD_FAST                7 (model_tokens)
                      466 LOAD_CONST               1 (0)
                      468 BINARY_SUBSCR
                      478 LOAD_CONST               7 ('from_context')
                      480 COMPARE_OP               3 (!=)
                      486 POP_JUMP_FORWARD_IF_FALSE    47 (to 582)
                      488 LOAD_FAST                5 (adapter)
                      490 LOAD_ATTR                7 (field_required)
                      500 POP_JUMP_FORWARD_IF_TRUE    40 (to 582)
          
-         182     >>  502 LOAD_FAST                0 (parser)
+         207     >>  502 LOAD_FAST                0 (parser)
                      504 LOAD_METHOD              8 (compile_filter)
                      526 LOAD_FAST                7 (model_tokens)
                      528 LOAD_METHOD              1 (pop)
                      550 LOAD_CONST               1 (0)
                      552 PRECALL                  1
                      556 CALL                     1
                      566 PRECALL                  1
                      570 CALL                     1
                      580 STORE_FAST               6 (model)
          
-         184     >>  582 LOAD_CONST               0 (None)
+         209     >>  582 LOAD_CONST               0 (None)
                      584 STORE_FAST               9 (as_var)
          
-         185         586 LOAD_FAST                2 (tokens)
+         210         586 LOAD_FAST                2 (tokens)
                      588 POP_JUMP_FORWARD_IF_FALSE   102 (to 794)
                      590 LOAD_FAST                2 (tokens)
                      592 LOAD_GLOBAL             13 (NULL + len)
                      604 LOAD_FAST                2 (tokens)
                      606 PRECALL                  1
                      610 CALL                     1
                      620 LOAD_CONST               6 (2)
                      622 BINARY_OP               10 (-)
                      626 BINARY_SUBSCR
                      636 LOAD_CONST              10 ('as')
                      638 COMPARE_OP               2 (==)
                      644 POP_JUMP_FORWARD_IF_FALSE    74 (to 794)
          
-         186         646 LOAD_FAST                2 (tokens)
+         211         646 LOAD_FAST                2 (tokens)
                      648 LOAD_METHOD              1 (pop)
                      670 LOAD_GLOBAL             13 (NULL + len)
                      682 LOAD_FAST                2 (tokens)
                      684 PRECALL                  1
                      688 CALL                     1
                      698 LOAD_CONST               9 (1)
                      700 BINARY_OP               10 (-)
                      704 PRECALL                  1
                      708 CALL                     1
                      718 STORE_FAST               9 (as_var)
          
-         187         720 LOAD_FAST                2 (tokens)
+         212         720 LOAD_FAST                2 (tokens)
                      722 LOAD_METHOD              1 (pop)
                      744 LOAD_GLOBAL             13 (NULL + len)
                      756 LOAD_FAST                2 (tokens)
                      758 PRECALL                  1
                      762 CALL                     1
                      772 LOAD_CONST               9 (1)
                      774 BINARY_OP               10 (-)
                      778 PRECALL                  1
                      782 CALL                     1
                      792 POP_TOP
          
-         189     >>  794 LOAD_GLOBAL             19 (NULL + get_kwargs)
+         214     >>  794 LOAD_GLOBAL             19 (NULL + get_kwargs)
          
-         190         806 LOAD_FAST                0 (parser)
+         215         806 LOAD_FAST                0 (parser)
          
-         191         808 LOAD_FAST                2 (tokens)
+         216         808 LOAD_FAST                2 (tokens)
          
-         192         810 LOAD_FAST                5 (adapter)
+         217         810 LOAD_FAST                5 (adapter)
                      812 LOAD_ATTR               10 (required_kwargs)
          
-         193         822 LOAD_FAST                5 (adapter)
+         218         822 LOAD_FAST                5 (adapter)
                      824 LOAD_ATTR               11 (absolute_tokens)
          
-         194         834 LOAD_FAST                5 (adapter)
-                     836 LOAD_ATTR               12 (optional_kwargs)
-         
-         189         846 PRECALL                  5
-                     850 CALL                     5
-                     860 STORE_FAST              10 (kwargs)
+         214         834 PRECALL                  4
+                     838 CALL                     4
+                     848 STORE_FAST              10 (kwargs)
          
-         197         862 LOAD_GLOBAL             27 (NULL + AdapterNode)
-                     874 LOAD_CONST              12 (())
+         221         850 LOAD_GLOBAL             25 (NULL + AdapterNode)
+                     862 LOAD_CONST              12 (())
          
-         198         876 LOAD_FAST                5 (adapter)
+         222         864 LOAD_FAST                5 (adapter)
          
-         199         878 LOAD_FAST                6 (model)
+         223         866 LOAD_FAST                6 (model)
          
-         200         880 LOAD_FAST                7 (model_tokens)
+         224         868 LOAD_FAST                7 (model_tokens)
          
-         201         882 LOAD_FAST                9 (as_var)
+         225         870 LOAD_FAST                9 (as_var)
          
-         197         884 LOAD_CONST              11 (('adapter', 'model', 'getters', 'as_var'))
-                     886 BUILD_CONST_KEY_MAP      4
+         221         872 LOAD_CONST              11 (('adapter', 'model', 'getters', 'as_var'))
+                     874 BUILD_CONST_KEY_MAP      4
          
-         202         888 LOAD_FAST               10 (kwargs)
+         226         876 LOAD_FAST               10 (kwargs)
          
-         197         890 DICT_MERGE               1
-                     892 CALL_FUNCTION_EX         1
-                     894 RETURN_VALUE
+         221         878 DICT_MERGE               1
+                     880 CALL_FUNCTION_EX         1
+                     882 RETURN_VALUE
          ExceptionTable:
            128 to 152 -> 156 [0]
            156 to 214 -> 216 [1] lasti
          consts
             None
             0
             "No adapter found with identifier '"
@@ -1201,131 +1230,102 @@
             2
             'from_context'
             "Model and field name are required: 'mymodel.myfield' or 'from_context'"
             1
             'as'
             ('adapter', 'model', 'getters', 'as_var')
             ()
-         names      ('split_contents', 'pop', 'adapter_registry', 'RegistryLookUpError', 'TemplateSyntaxError', 'split', 'len', 'field_required', 'compile_filter', 'get_kwargs', 'required_kwargs', 'absolute_tokens', 'optional_kwargs', 'AdapterNode')
+         names      ('split_contents', 'pop', 'adapter_registry', 'RegistryLookUpError', 'TemplateSyntaxError', 'split', 'len', 'field_required', 'compile_filter', 'get_kwargs', 'required_kwargs', 'absolute_tokens', 'AdapterNode')
          varnames   ('parser', 'token', 'tokens', '_', 'adapter_id', 'adapter', 'model', 'model_tokens', 'model__field', 'as_var', 'kwargs')
          freevars   ()
          cellvars   ()
-         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
+         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
          name       'do_render_fedit'
-         firstlineno 149
+         firstlineno 174
          lnotab
             0x020328022a012a0202011e01120126ff08030a0104012a012a04260126
             010c0102ff100526012605500204013c014a014a020c01020102010c010c
-            010cfb10080e0102010201020102fc040502fb
+            fc10070e0102010201020102fc040502fb
       True
       ('takes_context',)
       'adapter'
       code
          argcount  : 2
          nlocals   : 3
-         stacksize : 4
+         stacksize : 3
          flags     : 3
          code
             0x970069007d0264017c007600720b7c006401190000000000000000007d
-            027c0064013d007c00a00000000000000000000000000000000000000000
-            007c02a6010000ab01000000000000000001007c016a0100000000000000
-            007c0064023c0000007c016a0200000000000000007c0064033c0000007c
-            016a0300000000000000007c0064043c0000007c00a00000000000000000
-            000000000000000000000000007c016a040000000000000000a6010000ab
-            0100000000000000000100740b000000000000000000007c016a02000000
-            0000000000740c00000000000000000000a6020000ab0200000000000000
-            00720f7c016a0200000000000000007c00740e000000000000000000003c
-            0000007c01a00800000000000000000000000000000000000000007c00a6
-            010000ab0100000000000000005300
-         207           0 RESUME                   0
+            027c0064013d007401000000000000000000007c00a6010000ab01000000
+            00000000007d007401000000000000000000007c02a6010000ab01000000
+            00000000007d027c00a00100000000000000000000000000000000000000
+            007c02a6010000ab01000000000000000001007c01a00200000000000000
+            000000000000000000000000007c00a6010000ab01000000000000000053
+            00
+         230           0 RESUME                   0
          
-         209           2 BUILD_MAP                0
-                       4 STORE_FAST               2 (parent_context)
+         232           2 BUILD_MAP                0
+                       4 STORE_FAST               2 (adapter_context)
          
-         211           6 LOAD_CONST               1 ('parent_context')
+         234           6 LOAD_CONST               1 ('adapter_context')
                        8 LOAD_FAST                0 (context)
                       10 CONTAINS_OP              0
                       12 POP_JUMP_FORWARD_IF_FALSE    11 (to 36)
          
-         212          14 LOAD_FAST                0 (context)
-                      16 LOAD_CONST               1 ('parent_context')
+         235          14 LOAD_FAST                0 (context)
+                      16 LOAD_CONST               1 ('adapter_context')
                       18 BINARY_SUBSCR
-                      28 STORE_FAST               2 (parent_context)
+                      28 STORE_FAST               2 (adapter_context)
          
-         213          30 LOAD_FAST                0 (context)
-                      32 LOAD_CONST               1 ('parent_context')
+         236          30 LOAD_FAST                0 (context)
+                      32 LOAD_CONST               1 ('adapter_context')
                       34 DELETE_SUBSCR
          
-         215     >>   36 LOAD_FAST                0 (context)
-                      38 LOAD_METHOD              0 (update)
-                      60 LOAD_FAST                2 (parent_context)
-                      62 PRECALL                  1
-                      66 CALL                     1
-                      76 POP_TOP
-         
-         217          78 LOAD_FAST                1 (adapter)
-                      80 LOAD_ATTR                1 (field_name)
-                      90 LOAD_FAST                0 (context)
-                      92 LOAD_CONST               2 ('wagtail_fedit_field')
-                      94 STORE_SUBSCR
-         
-         218          98 LOAD_FAST                1 (adapter)
-                     100 LOAD_ATTR                2 (object)
-                     110 LOAD_FAST                0 (context)
-                     112 LOAD_CONST               3 ('wagtail_fedit_instance')
-                     114 STORE_SUBSCR
-         
-         219         118 LOAD_FAST                1 (adapter)
-                     120 LOAD_ATTR                3 (request)
-                     130 LOAD_FAST                0 (context)
-                     132 LOAD_CONST               4 ('request')
-                     134 STORE_SUBSCR
-         
-         221         138 LOAD_FAST                0 (context)
-                     140 LOAD_METHOD              0 (update)
-                     162 LOAD_FAST                1 (adapter)
-                     164 LOAD_ATTR                4 (kwargs)
-                     174 PRECALL                  1
-                     178 CALL                     1
-                     188 POP_TOP
-         
-         223         190 LOAD_GLOBAL             11 (NULL + isinstance)
-                     202 LOAD_FAST                1 (adapter)
-                     204 LOAD_ATTR                2 (object)
-                     214 LOAD_GLOBAL             12 (Page)
-                     226 PRECALL                  2
-                     230 CALL                     2
-                     240 POP_JUMP_FORWARD_IF_FALSE    15 (to 272)
-         
-         224         242 LOAD_FAST                1 (adapter)
-                     244 LOAD_ATTR                2 (object)
-                     254 LOAD_FAST                0 (context)
-                     256 LOAD_GLOBAL             14 (PAGE_TEMPLATE_VAR)
-                     268 STORE_SUBSCR
-         
-         226     >>  272 LOAD_FAST                1 (adapter)
-                     274 LOAD_METHOD              8 (render_content)
-                     296 LOAD_FAST                0 (context)
-                     298 PRECALL                  1
-                     302 CALL                     1
-                     312 RETURN_VALUE
+         238     >>   36 LOAD_GLOBAL              1 (NULL + _flatten_context)
+         
+         239          48 LOAD_FAST                0 (context)
+         
+         238          50 PRECALL                  1
+                      54 CALL                     1
+                      64 STORE_FAST               0 (context)
+         
+         241          66 LOAD_GLOBAL              1 (NULL + _flatten_context)
+         
+         242          78 LOAD_FAST                2 (adapter_context)
+         
+         241          80 PRECALL                  1
+                      84 CALL                     1
+                      94 STORE_FAST               2 (adapter_context)
+         
+         245          96 LOAD_FAST                0 (context)
+                      98 LOAD_METHOD              1 (update)
+                     120 LOAD_FAST                2 (adapter_context)
+                     122 PRECALL                  1
+                     126 CALL                     1
+                     136 POP_TOP
+         
+         247         138 LOAD_FAST                1 (adapter)
+                     140 LOAD_METHOD              2 (render_content)
+         
+         248         162 LOAD_FAST                0 (context)
+         
+         247         164 PRECALL                  1
+                     168 CALL                     1
+                     178 RETURN_VALUE
          consts
             None
-            'parent_context'
-            'wagtail_fedit_field'
-            'wagtail_fedit_instance'
-            'request'
-         names      ('update', 'field_name', 'object', 'request', 'kwargs', 'isinstance', 'Page', 'PAGE_TEMPLATE_VAR', 'render_content')
-         varnames   ('context', 'adapter', 'parent_context')
+            'adapter_context'
+         names      ('_flatten_context', 'update', 'render_content')
+         varnames   ('context', 'adapter', 'adapter_context')
          freevars   ()
          cellvars   ()
-         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
+         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
          name       'render_adapter'
-         firstlineno 207
-         lnotab 0x020204020801100106022a02140114011402340234011e02
+         firstlineno 230
+         lnotab 0x020204020801100106020c0102ff10030c0102ff10042a02180102ff
       'wagtail_fedit/_hook_output.html'
       'fedit_scripts'
       ('name', 'takes_context')
       code
          argcount  : 2
          nlocals   : 7
          stacksize : 6
@@ -1341,520 +1341,561 @@
             00530067007d04740f000000000000000000006a0800000000000000007c
             03a6010000ab01000000000000000044005d417d0502007c057c02a60100
             00ab0100000000000000007d067413000000000000000000007c06741400
             0000000000000000007416000000000000000000006602a6020000ab0200
             0000000000000073037c0667017d067c04a00c0000000000000000000000
             0000000000000000007c06a6010000ab01000000000000000001008c4264
             067c0469015300
-         229           0 RESUME                   0
+         252           0 RESUME                   0
          
-         231           2 LOAD_FAST                1 (css_or_js)
+         254           2 LOAD_FAST                1 (css_or_js)
                        4 LOAD_METHOD              0 (lower)
                       26 PRECALL                  0
                       30 CALL                     0
                       40 STORE_FAST               1 (css_or_js)
          
-         233          42 LOAD_FAST                1 (css_or_js)
+         256          42 LOAD_FAST                1 (css_or_js)
                       44 LOAD_CONST               1 (('css', 'js'))
                       46 CONTAINS_OP              1
                       48 POP_JUMP_FORWARD_IF_FALSE    15 (to 80)
          
-         234          50 LOAD_GLOBAL              3 (NULL + ValueError)
+         257          50 LOAD_GLOBAL              3 (NULL + ValueError)
                       62 LOAD_CONST               2 ("Invalid argument, must be 'css' or 'js'")
                       64 PRECALL                  1
                       68 CALL                     1
                       78 RAISE_VARARGS            1
          
-         236     >>   80 LOAD_FAST                0 (context)
+         259     >>   80 LOAD_FAST                0 (context)
                       82 LOAD_METHOD              2 (get)
                      104 LOAD_CONST               3 ('request')
                      106 PRECALL                  1
                      110 CALL                     1
                      120 STORE_FAST               2 (request)
          
-         238         122 LOAD_FAST                1 (css_or_js)
+         261         122 LOAD_FAST                1 (css_or_js)
                      124 LOAD_CONST               4 ('css')
                      126 COMPARE_OP               2 (==)
                      132 POP_JUMP_FORWARD_IF_FALSE     8 (to 150)
          
-         239         134 LOAD_GLOBAL              6 (REGISTER_CSS)
+         262         134 LOAD_GLOBAL              6 (REGISTER_CSS)
                      146 STORE_FAST               3 (hook_name)
                      148 JUMP_FORWARD             7 (to 164)
          
-         241     >>  150 LOAD_GLOBAL              8 (REGISTER_JS)
+         264     >>  150 LOAD_GLOBAL              8 (REGISTER_JS)
                      162 STORE_FAST               3 (hook_name)
          
-         243     >>  164 LOAD_GLOBAL             11 (NULL + getattr)
+         266     >>  164 LOAD_GLOBAL             11 (NULL + getattr)
                      176 LOAD_FAST                2 (request)
                      178 LOAD_GLOBAL             12 (FEDIT_PREVIEW_VAR)
                      190 LOAD_CONST               5 (False)
                      192 PRECALL                  3
                      196 CALL                     3
                      206 POP_JUMP_FORWARD_IF_TRUE     2 (to 212)
          
-         244         208 BUILD_MAP                0
+         267         208 BUILD_MAP                0
                      210 RETURN_VALUE
          
-         246     >>  212 BUILD_LIST               0
+         269     >>  212 BUILD_LIST               0
                      214 STORE_FAST               4 (files)
          
-         247         216 LOAD_GLOBAL             15 (NULL + hooks)
+         270         216 LOAD_GLOBAL             15 (NULL + hooks)
                      228 LOAD_ATTR                8 (get_hooks)
                      238 LOAD_FAST                3 (hook_name)
                      240 PRECALL                  1
                      244 CALL                     1
                      254 GET_ITER
                  >>  256 FOR_ITER                65 (to 388)
                      258 STORE_FAST               5 (hook)
          
-         248         260 PUSH_NULL
+         271         260 PUSH_NULL
                      262 LOAD_FAST                5 (hook)
                      264 LOAD_FAST                2 (request)
                      266 PRECALL                  1
                      270 CALL                     1
                      280 STORE_FAST               6 (ret)
          
-         250         282 LOAD_GLOBAL             19 (NULL + isinstance)
+         273         282 LOAD_GLOBAL             19 (NULL + isinstance)
                      294 LOAD_FAST                6 (ret)
                      296 LOAD_GLOBAL             20 (list)
                      308 LOAD_GLOBAL             22 (tuple)
                      320 BUILD_TUPLE              2
                      322 PRECALL                  2
                      326 CALL                     2
                      336 POP_JUMP_FORWARD_IF_TRUE     3 (to 344)
          
-         251         338 LOAD_FAST                6 (ret)
+         274         338 LOAD_FAST                6 (ret)
                      340 BUILD_LIST               1
                      342 STORE_FAST               6 (ret)
          
-         253     >>  344 LOAD_FAST                4 (files)
+         276     >>  344 LOAD_FAST                4 (files)
                      346 LOAD_METHOD             12 (extend)
                      368 LOAD_FAST                6 (ret)
                      370 PRECALL                  1
                      374 CALL                     1
                      384 POP_TOP
                      386 JUMP_BACKWARD           66 (to 256)
          
-         256     >>  388 LOAD_CONST               6 ('hook_output')
+         279     >>  388 LOAD_CONST               6 ('hook_output')
                      390 LOAD_FAST                4 (files)
          
-         255         392 BUILD_MAP                1
+         278         392 BUILD_MAP                1
                      394 RETURN_VALUE
          consts
             None
             ('css', 'js')
             "Invalid argument, must be 'css' or 'js'"
             'request'
             'css'
             False
             'hook_output'
          names      ('lower', 'ValueError', 'get', 'REGISTER_CSS', 'REGISTER_JS', 'getattr', 'FEDIT_PREVIEW_VAR', 'hooks', 'get_hooks', 'isinstance', 'list', 'tuple', 'extend')
          varnames   ('context', 'css_or_js', 'request', 'hook_name', 'files', 'hook', 'ret')
          freevars   ()
          cellvars   ()
-         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
+         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
          name       'static_hook_output'
-         firstlineno 229
+         firstlineno 252
          lnotab
             0x0202280208011e022a020c0110020e022c01040204012c011602380106
             022c0304ff
       False
       'tooltip'
       ('takes_context', 'name')
       'wrapping'
       code
          argcount  : 2
          nlocals   : 7
          stacksize : 9
          flags     : 11
          code
-            0x97007c007c0264013c000000640267017d037c02a00000000000000000
-            00000000000000000000000000a6000000ab00000000000000000044005d
-            2e5c0200007d047d057c03a0010000000000000000000000000000000000
-            00000064037c049b0064047405000000000000000000007c05a6010000ab
-            0100000000000000009b0064059d05a6010000ab01000000000000000001
-            008c2f6406a00300000000000000000000000000000000000000007c03a6
-            010000ab0100000000000000007d067c01730f7409000000000000000000
-            007c06a6010000ab01000000000000000053007409000000000000000000
-            0064077c069b0064087c019b0064099d05a6010000ab0100000000000000
-            005300
-         259           0 RESUME                   0
-         
-         261           2 LOAD_FAST                0 (content)
-                       4 LOAD_FAST                2 (kwargs)
-                       6 LOAD_CONST               1 ('content')
-                       8 STORE_SUBSCR
-         
-         263          12 LOAD_CONST               2 ("data-tooltip='true'")
-         
-         262          14 BUILD_LIST               1
-                      16 STORE_FAST               3 (s)
-         
-         265          18 LOAD_FAST                2 (kwargs)
-                      20 LOAD_METHOD              0 (items)
-                      42 PRECALL                  0
-                      46 CALL                     0
-                      56 GET_ITER
-                 >>   58 FOR_ITER                46 (to 152)
-                      60 UNPACK_SEQUENCE          2
-                      64 STORE_FAST               4 (key)
-                      66 STORE_FAST               5 (value)
-         
-         266          68 LOAD_FAST                3 (s)
-                      70 LOAD_METHOD              1 (append)
-                      92 LOAD_CONST               3 ('data-tooltip-')
-                      94 LOAD_FAST                4 (key)
-                      96 FORMAT_VALUE             0
-                      98 LOAD_CONST               4 ("='")
-                     100 LOAD_GLOBAL              5 (NULL + escape)
-                     112 LOAD_FAST                5 (value)
-                     114 PRECALL                  1
-                     118 CALL                     1
-                     128 FORMAT_VALUE             0
-                     130 LOAD_CONST               5 ("'")
-                     132 BUILD_STRING             5
-                     134 PRECALL                  1
-                     138 CALL                     1
-                     148 POP_TOP
-                     150 JUMP_BACKWARD           47 (to 58)
-         
-         267     >>  152 LOAD_CONST               6 (' ')
-                     154 LOAD_METHOD              3 (join)
-                     176 LOAD_FAST                3 (s)
-                     178 PRECALL                  1
-                     182 CALL                     1
-                     192 STORE_FAST               6 (attrs)
-         
-         269         194 LOAD_FAST                1 (wrapping)
-                     196 POP_JUMP_FORWARD_IF_TRUE    15 (to 228)
-         
-         270         198 LOAD_GLOBAL              9 (NULL + mark_safe)
-                     210 LOAD_FAST                6 (attrs)
-                     212 PRECALL                  1
-                     216 CALL                     1
-                     226 RETURN_VALUE
-         
-         272     >>  228 LOAD_GLOBAL              9 (NULL + mark_safe)
-                     240 LOAD_CONST               7 ('<span ')
-                     242 LOAD_FAST                6 (attrs)
-                     244 FORMAT_VALUE             0
-                     246 LOAD_CONST               8 ('>')
-                     248 LOAD_FAST                1 (wrapping)
-                     250 FORMAT_VALUE             0
-                     252 LOAD_CONST               9 ('</span>')
-                     254 BUILD_STRING             5
-                     256 PRECALL                  1
-                     260 CALL                     1
-                     270 RETURN_VALUE
+            0x97007400000000000000000000007302640153007c007c0264023c0000
+            00640367017d037c02a00100000000000000000000000000000000000000
+            00a6000000ab00000000000000000044005d2e5c0200007d047d057c03a0
+            02000000000000000000000000000000000000000064047c049b00640574
+            07000000000000000000007c05a6010000ab0100000000000000009b0064
+            069d05a6010000ab01000000000000000001008c2f6407a0040000000000
+            0000000000000000000000000000007c03a6010000ab0100000000000000
+            007d067c01730f740b000000000000000000007c06a6010000ab01000000
+            00000000005300740b0000000000000000000064087c069b0064097c019b
+            00640a9d05a6010000ab0100000000000000005300
+         282           0 RESUME                   0
+         
+         285           2 LOAD_GLOBAL              0 (TIPPY_ENABLED)
+                      14 POP_JUMP_FORWARD_IF_TRUE     2 (to 20)
+         
+         286          16 LOAD_CONST               1 ('')
+                      18 RETURN_VALUE
+         
+         288     >>   20 LOAD_FAST                0 (content)
+                      22 LOAD_FAST                2 (kwargs)
+                      24 LOAD_CONST               2 ('content')
+                      26 STORE_SUBSCR
+         
+         290          30 LOAD_CONST               3 ("data-tooltip='true'")
+         
+         289          32 BUILD_LIST               1
+                      34 STORE_FAST               3 (s)
+         
+         292          36 LOAD_FAST                2 (kwargs)
+                      38 LOAD_METHOD              1 (items)
+                      60 PRECALL                  0
+                      64 CALL                     0
+                      74 GET_ITER
+                 >>   76 FOR_ITER                46 (to 170)
+                      78 UNPACK_SEQUENCE          2
+                      82 STORE_FAST               4 (key)
+                      84 STORE_FAST               5 (value)
+         
+         293          86 LOAD_FAST                3 (s)
+                      88 LOAD_METHOD              2 (append)
+                     110 LOAD_CONST               4 ('data-tooltip-')
+                     112 LOAD_FAST                4 (key)
+                     114 FORMAT_VALUE             0
+                     116 LOAD_CONST               5 ("='")
+                     118 LOAD_GLOBAL              7 (NULL + escape)
+                     130 LOAD_FAST                5 (value)
+                     132 PRECALL                  1
+                     136 CALL                     1
+                     146 FORMAT_VALUE             0
+                     148 LOAD_CONST               6 ("'")
+                     150 BUILD_STRING             5
+                     152 PRECALL                  1
+                     156 CALL                     1
+                     166 POP_TOP
+                     168 JUMP_BACKWARD           47 (to 76)
+         
+         294     >>  170 LOAD_CONST               7 (' ')
+                     172 LOAD_METHOD              4 (join)
+                     194 LOAD_FAST                3 (s)
+                     196 PRECALL                  1
+                     200 CALL                     1
+                     210 STORE_FAST               6 (attrs)
+         
+         296         212 LOAD_FAST                1 (wrapping)
+                     214 POP_JUMP_FORWARD_IF_TRUE    15 (to 246)
+         
+         297         216 LOAD_GLOBAL             11 (NULL + mark_safe)
+                     228 LOAD_FAST                6 (attrs)
+                     230 PRECALL                  1
+                     234 CALL                     1
+                     244 RETURN_VALUE
+         
+         299     >>  246 LOAD_GLOBAL             11 (NULL + mark_safe)
+                     258 LOAD_CONST               8 ('<span ')
+                     260 LOAD_FAST                6 (attrs)
+                     262 FORMAT_VALUE             0
+                     264 LOAD_CONST               9 ('>')
+                     266 LOAD_FAST                1 (wrapping)
+                     268 FORMAT_VALUE             0
+                     270 LOAD_CONST              10 ('</span>')
+                     272 BUILD_STRING             5
+                     274 PRECALL                  1
+                     278 CALL                     1
+                     288 RETURN_VALUE
          consts
             None
+            ''
             'content'
             "data-tooltip='true'"
             'data-tooltip-'
             "='"
             "'"
             ' '
             '<span '
             '>'
             '</span>'
-         names      ('items', 'append', 'escape', 'join', 'mark_safe')
+         names      ('TIPPY_ENABLED', 'items', 'append', 'escape', 'join', 'mark_safe')
          varnames   ('content', 'wrapping', 'kwargs', 's', 'key', 'value', 'attrs')
          freevars   ()
          cellvars   ()
-         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
+         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
          name       'tooltip'
-         firstlineno 259
-         lnotab 0x02020a0202ff0403320154012a0204011e02
+         firstlineno 282
+         lnotab 0x02030e0104020a0202ff0403320154012a0204011e02
+      'fedit_userbar'
+      'model'
+      code
+         argcount  : 2
+         nlocals   : 2
+         stacksize : 4
+         flags     : 3
+         code
+            0x970064017c00760072197401000000000000000000007c006401190000
+            000000000000007c01a6020000ab0200000000000000007c0064013c0000
+            007402000000000000000000007c007600721b7c00740200000000000000
+            000000190000000000000000007c016b0300000000720a7c017c00740200
+            0000000000000000003c00000064025300
+         301           0 RESUME                   0
+         
+         303           2 LOAD_CONST               1 ('request')
+                       4 LOAD_FAST                0 (context)
+                       6 CONTAINS_OP              0
+                       8 POP_JUMP_FORWARD_IF_FALSE    25 (to 60)
+         
+         304          10 LOAD_GLOBAL              1 (NULL + with_userbar_model)
+                      22 LOAD_FAST                0 (context)
+                      24 LOAD_CONST               1 ('request')
+                      26 BINARY_SUBSCR
+                      36 LOAD_FAST                1 (model)
+                      38 PRECALL                  2
+                      42 CALL                     2
+                      52 LOAD_FAST                0 (context)
+                      54 LOAD_CONST               1 ('request')
+                      56 STORE_SUBSCR
+         
+         305     >>   60 LOAD_GLOBAL              2 (PAGE_TEMPLATE_VAR)
+                      72 LOAD_FAST                0 (context)
+                      74 CONTAINS_OP              0
+                      76 POP_JUMP_FORWARD_IF_FALSE    27 (to 132)
+                      78 LOAD_FAST                0 (context)
+                      80 LOAD_GLOBAL              2 (PAGE_TEMPLATE_VAR)
+                      92 BINARY_SUBSCR
+                     102 LOAD_FAST                1 (model)
+                     104 COMPARE_OP               3 (!=)
+                     110 POP_JUMP_FORWARD_IF_FALSE    10 (to 132)
+         
+         306         112 LOAD_FAST                1 (model)
+                     114 LOAD_FAST                0 (context)
+                     116 LOAD_GLOBAL              2 (PAGE_TEMPLATE_VAR)
+                     128 STORE_SUBSCR
+         
+         307     >>  132 LOAD_CONST               2 ('')
+                     134 RETURN_VALUE
+         consts
+            None
+            'request'
+            ''
+         names      ('with_userbar_model', 'PAGE_TEMPLATE_VAR')
+         varnames   ('context', 'model')
+         freevars   ()
+         cellvars   ()
+         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
+         name       'do_with_userbar_model'
+         firstlineno 301
+         lnotab 0x02020801320134011401
       'tokens'
       'kwarg_list'
       'absolute_tokens'
-      'optional_tokens'
       code
-         argcount  : 5
-         nlocals   : 13
+         argcount  : 4
+         nlocals   : 11
          stacksize : 6
          flags     : 3
          code
-            0x970064017d0569007d067c02730e740100000000000000000000a60000
+            0x970064017d0469007d057c02730e740100000000000000000000a60000
             00ab0000000000000000007d027c03730e740100000000000000000000a6
-            000000ab0000000000000000007d037c04730269007d0474030000000000
-            00000000007c01a6010000ab010000000000000000440090015d125c0200
-            007d077d087c08a002000000000000000000000000000000000000000064
-            02a6010000ab0100000000000000007d097407000000000000000000007c
-            09a6010000ab01000000000000000064036b020000000072597407000000
-            000000000000007c02a6010000ab0100000000000000007c076b04000000
-            0072467c096404190000000000000000007c037600720c64057c067c0964
-            04190000000000000000003c0000008c577c05720f740900000000000000
-            0000006406a6010000ab01000000000000000082017c00a0050000000000
-            0000000000000000000000000000007c08a6010000ab0100000000000000
-            007c067c027c07190000000000000000003c0000008c8774070000000000
-            00000000007c09a6010000ab01000000000000000064036b020000000072
-            397c096404190000000000000000007c037600720c64057c067c09640419
-            0000000000000000003c0000008cb07c096404190000000000000000007d
-            0a7c00a00500000000000000000000000000000000000000007c0aa60100
-            00ab0100000000000000007d0b7c0b7c067c0a3c0000008cd37c09640419
-            0000000000000000007d0a7c0a7c03760072137409000000000000000000
-            0064077c0a9b0064089d03a6010000ab01000000000000000082017c00a0
-            0500000000000000000000000000000000000000007c0964031900000000
-            0000000000a6010000ab0100000000000000007c067c0a3c00000064057d
-            0590018c147c0244005d187d0c7c0c7c0676017212740d00000000000000
-            00000064097c0c9b009d02a6010000ab01000000000000000082018c197c
-            04a0070000000000000000000000000000000000000000a6000000ab0000
-            0000000000000044005d0e5c0200007d0a7d0b7c0a7c06760172057c0b7c
-            067c0a3c0000008c0f7c065300
-         275           0 RESUME                   0
+            000000ab0000000000000000007d037403000000000000000000007c01a6
+            010000ab010000000000000000440090015d125c0200007d067d077c07a0
+            0200000000000000000000000000000000000000006402a6010000ab0100
+            000000000000007d087407000000000000000000007c08a6010000ab0100
+            0000000000000064036b020000000072597407000000000000000000007c
+            02a6010000ab0100000000000000007c066b040000000072467c08640419
+            0000000000000000007c037600720c64057c057c08640419000000000000
+            0000003c0000008c577c04720f7409000000000000000000006406a60100
+            00ab01000000000000000082017c00a00500000000000000000000000000
+            000000000000007c07a6010000ab0100000000000000007c057c027c0619
+            0000000000000000003c0000008c877407000000000000000000007c08a6
+            010000ab01000000000000000064036b020000000072397c086404190000
+            000000000000007c037600720c64057c057c086404190000000000000000
+            003c0000008cb07c086404190000000000000000007d097c00a005000000
+            00000000000000000000000000000000007c09a6010000ab010000000000
+            0000007d0a7c0a7c057c093c0000008cd37c086404190000000000000000
+            007d097c097c0376007213740d0000000000000000000064077c099b0064
+            089d03a6010000ab01000000000000000082017c00a00500000000000000
+            000000000000000000000000007c08640319000000000000000000a60100
+            00ab0100000000000000007c057c093c00000064057d0490018c147c0244
+            005d187d097c097c0576017212740d0000000000000000000064097c099b
+            009d02a6010000ab01000000000000000082018c197c055300
+         309           0 RESUME                   0
          
-         276           2 LOAD_CONST               1 (False)
-                       4 STORE_FAST               5 (had_kwargs)
+         310           2 LOAD_CONST               1 (False)
+                       4 STORE_FAST               4 (had_kwargs)
          
-         277           6 BUILD_MAP                0
-                       8 STORE_FAST               6 (kwargs)
+         311           6 BUILD_MAP                0
+                       8 STORE_FAST               5 (kwargs)
          
-         279          10 LOAD_FAST                2 (kwarg_list)
+         313          10 LOAD_FAST                2 (kwarg_list)
                       12 POP_JUMP_FORWARD_IF_TRUE    14 (to 42)
          
-         280          14 LOAD_GLOBAL              1 (NULL + tuple)
+         314          14 LOAD_GLOBAL              1 (NULL + tuple)
                       26 PRECALL                  0
                       30 CALL                     0
                       40 STORE_FAST               2 (kwarg_list)
          
-         282     >>   42 LOAD_FAST                3 (absolute_tokens)
+         316     >>   42 LOAD_FAST                3 (absolute_tokens)
                       44 POP_JUMP_FORWARD_IF_TRUE    14 (to 74)
          
-         283          46 LOAD_GLOBAL              1 (NULL + tuple)
+         317          46 LOAD_GLOBAL              1 (NULL + tuple)
                       58 PRECALL                  0
                       62 CALL                     0
                       72 STORE_FAST               3 (absolute_tokens)
          
-         285     >>   74 LOAD_FAST                4 (optional_tokens)
-                      76 POP_JUMP_FORWARD_IF_TRUE     2 (to 82)
-         
-         286          78 BUILD_MAP                0
-                      80 STORE_FAST               4 (optional_tokens)
-         
-         288     >>   82 LOAD_GLOBAL              3 (NULL + enumerate)
-                      94 LOAD_FAST                1 (tokens)
-                      96 PRECALL                  1
-                     100 CALL                     1
-                     110 GET_ITER
-                 >>  112 EXTENDED_ARG             1
-                     114 FOR_ITER               274 (to 664)
-                     116 UNPACK_SEQUENCE          2
-                     120 STORE_FAST               7 (i)
-                     122 STORE_FAST               8 (token)
-         
-         289         124 LOAD_FAST                8 (token)
-                     126 LOAD_METHOD              2 (split)
-                     148 LOAD_CONST               2 ('=')
-                     150 PRECALL                  1
-                     154 CALL                     1
-                     164 STORE_FAST               9 (split)
-         
-         290         166 LOAD_GLOBAL              7 (NULL + len)
-                     178 LOAD_FAST                9 (split)
-                     180 PRECALL                  1
-                     184 CALL                     1
-                     194 LOAD_CONST               3 (1)
-                     196 COMPARE_OP               2 (==)
-                     202 POP_JUMP_FORWARD_IF_FALSE    89 (to 382)
-                     204 LOAD_GLOBAL              7 (NULL + len)
-                     216 LOAD_FAST                2 (kwarg_list)
-                     218 PRECALL                  1
-                     222 CALL                     1
-                     232 LOAD_FAST                7 (i)
-                     234 COMPARE_OP               4 (>)
-                     240 POP_JUMP_FORWARD_IF_FALSE    70 (to 382)
-         
-         291         242 LOAD_FAST                9 (split)
-                     244 LOAD_CONST               4 (0)
-                     246 BINARY_SUBSCR
-                     256 LOAD_FAST                3 (absolute_tokens)
-                     258 CONTAINS_OP              0
-                     260 POP_JUMP_FORWARD_IF_FALSE    12 (to 286)
-         
-         292         262 LOAD_CONST               5 (True)
-                     264 LOAD_FAST                6 (kwargs)
-                     266 LOAD_FAST                9 (split)
-                     268 LOAD_CONST               4 (0)
-                     270 BINARY_SUBSCR
-                     280 STORE_SUBSCR
-         
-         293         284 JUMP_BACKWARD           87 (to 112)
-         
-         295     >>  286 LOAD_FAST                5 (had_kwargs)
-                     288 POP_JUMP_FORWARD_IF_FALSE    15 (to 320)
-         
-         296         290 LOAD_GLOBAL              9 (NULL + ValueError)
-                     302 LOAD_CONST               6 ('Unexpected positional argument after keyword argument')
-                     304 PRECALL                  1
-                     308 CALL                     1
-                     318 RAISE_VARARGS            1
-         
-         298     >>  320 LOAD_FAST                0 (parser)
-                     322 LOAD_METHOD              5 (compile_filter)
-                     344 LOAD_FAST                8 (token)
-                     346 PRECALL                  1
-                     350 CALL                     1
-                     360 LOAD_FAST                6 (kwargs)
-                     362 LOAD_FAST                2 (kwarg_list)
-                     364 LOAD_FAST                7 (i)
-                     366 BINARY_SUBSCR
-                     376 STORE_SUBSCR
-                     380 JUMP_BACKWARD          135 (to 112)
-         
-         299     >>  382 LOAD_GLOBAL              7 (NULL + len)
-                     394 LOAD_FAST                9 (split)
-                     396 PRECALL                  1
-                     400 CALL                     1
-                     410 LOAD_CONST               3 (1)
-                     412 COMPARE_OP               2 (==)
-                     418 POP_JUMP_FORWARD_IF_FALSE    57 (to 534)
-         
-         300         420 LOAD_FAST                9 (split)
-                     422 LOAD_CONST               4 (0)
-                     424 BINARY_SUBSCR
-                     434 LOAD_FAST                3 (absolute_tokens)
-                     436 CONTAINS_OP              0
-                     438 POP_JUMP_FORWARD_IF_FALSE    12 (to 464)
-         
-         301         440 LOAD_CONST               5 (True)
-                     442 LOAD_FAST                6 (kwargs)
-                     444 LOAD_FAST                9 (split)
-                     446 LOAD_CONST               4 (0)
-                     448 BINARY_SUBSCR
-                     458 STORE_SUBSCR
-         
-         302         462 JUMP_BACKWARD          176 (to 112)
-         
-         304     >>  464 LOAD_FAST                9 (split)
-                     466 LOAD_CONST               4 (0)
-                     468 BINARY_SUBSCR
-                     478 STORE_FAST              10 (key)
+         319     >>   74 LOAD_GLOBAL              3 (NULL + enumerate)
+                      86 LOAD_FAST                1 (tokens)
+                      88 PRECALL                  1
+                      92 CALL                     1
+                     102 GET_ITER
+                 >>  104 EXTENDED_ARG             1
+                     106 FOR_ITER               274 (to 656)
+                     108 UNPACK_SEQUENCE          2
+                     112 STORE_FAST               6 (i)
+                     114 STORE_FAST               7 (token)
+         
+         320         116 LOAD_FAST                7 (token)
+                     118 LOAD_METHOD              2 (split)
+                     140 LOAD_CONST               2 ('=')
+                     142 PRECALL                  1
+                     146 CALL                     1
+                     156 STORE_FAST               8 (split)
+         
+         321         158 LOAD_GLOBAL              7 (NULL + len)
+                     170 LOAD_FAST                8 (split)
+                     172 PRECALL                  1
+                     176 CALL                     1
+                     186 LOAD_CONST               3 (1)
+                     188 COMPARE_OP               2 (==)
+                     194 POP_JUMP_FORWARD_IF_FALSE    89 (to 374)
+                     196 LOAD_GLOBAL              7 (NULL + len)
+                     208 LOAD_FAST                2 (kwarg_list)
+                     210 PRECALL                  1
+                     214 CALL                     1
+                     224 LOAD_FAST                6 (i)
+                     226 COMPARE_OP               4 (>)
+                     232 POP_JUMP_FORWARD_IF_FALSE    70 (to 374)
+         
+         322         234 LOAD_FAST                8 (split)
+                     236 LOAD_CONST               4 (0)
+                     238 BINARY_SUBSCR
+                     248 LOAD_FAST                3 (absolute_tokens)
+                     250 CONTAINS_OP              0
+                     252 POP_JUMP_FORWARD_IF_FALSE    12 (to 278)
+         
+         323         254 LOAD_CONST               5 (True)
+                     256 LOAD_FAST                5 (kwargs)
+                     258 LOAD_FAST                8 (split)
+                     260 LOAD_CONST               4 (0)
+                     262 BINARY_SUBSCR
+                     272 STORE_SUBSCR
+         
+         324         276 JUMP_BACKWARD           87 (to 104)
+         
+         326     >>  278 LOAD_FAST                4 (had_kwargs)
+                     280 POP_JUMP_FORWARD_IF_FALSE    15 (to 312)
+         
+         327         282 LOAD_GLOBAL              9 (NULL + ValueError)
+                     294 LOAD_CONST               6 ('Unexpected positional argument after keyword argument')
+                     296 PRECALL                  1
+                     300 CALL                     1
+                     310 RAISE_VARARGS            1
+         
+         329     >>  312 LOAD_FAST                0 (parser)
+                     314 LOAD_METHOD              5 (compile_filter)
+                     336 LOAD_FAST                7 (token)
+                     338 PRECALL                  1
+                     342 CALL                     1
+                     352 LOAD_FAST                5 (kwargs)
+                     354 LOAD_FAST                2 (kwarg_list)
+                     356 LOAD_FAST                6 (i)
+                     358 BINARY_SUBSCR
+                     368 STORE_SUBSCR
+                     372 JUMP_BACKWARD          135 (to 104)
+         
+         330     >>  374 LOAD_GLOBAL              7 (NULL + len)
+                     386 LOAD_FAST                8 (split)
+                     388 PRECALL                  1
+                     392 CALL                     1
+                     402 LOAD_CONST               3 (1)
+                     404 COMPARE_OP               2 (==)
+                     410 POP_JUMP_FORWARD_IF_FALSE    57 (to 526)
+         
+         331         412 LOAD_FAST                8 (split)
+                     414 LOAD_CONST               4 (0)
+                     416 BINARY_SUBSCR
+                     426 LOAD_FAST                3 (absolute_tokens)
+                     428 CONTAINS_OP              0
+                     430 POP_JUMP_FORWARD_IF_FALSE    12 (to 456)
+         
+         332         432 LOAD_CONST               5 (True)
+                     434 LOAD_FAST                5 (kwargs)
+                     436 LOAD_FAST                8 (split)
+                     438 LOAD_CONST               4 (0)
+                     440 BINARY_SUBSCR
+                     450 STORE_SUBSCR
+         
+         333         454 JUMP_BACKWARD          176 (to 104)
+         
+         335     >>  456 LOAD_FAST                8 (split)
+                     458 LOAD_CONST               4 (0)
+                     460 BINARY_SUBSCR
+                     470 STORE_FAST               9 (key)
+         
+         336         472 LOAD_FAST                0 (parser)
+                     474 LOAD_METHOD              5 (compile_filter)
+                     496 LOAD_FAST                9 (key)
+                     498 PRECALL                  1
+                     502 CALL                     1
+                     512 STORE_FAST              10 (value)
+         
+         337         514 LOAD_FAST               10 (value)
+                     516 LOAD_FAST                5 (kwargs)
+                     518 LOAD_FAST                9 (key)
+                     520 STORE_SUBSCR
+                     524 JUMP_BACKWARD          211 (to 104)
+         
+         339     >>  526 LOAD_FAST                8 (split)
+                     528 LOAD_CONST               4 (0)
+                     530 BINARY_SUBSCR
+                     540 STORE_FAST               9 (key)
+         
+         342         542 LOAD_FAST                9 (key)
+                     544 LOAD_FAST                3 (absolute_tokens)
+                     546 CONTAINS_OP              0
+                     548 POP_JUMP_FORWARD_IF_FALSE    19 (to 588)
+         
+         343         550 LOAD_GLOBAL             13 (NULL + TemplateSyntaxError)
+         
+         344         562 LOAD_CONST               7 ('Keyword argument ')
+                     564 LOAD_FAST                9 (key)
+                     566 FORMAT_VALUE             0
+                     568 LOAD_CONST               8 (' cannot be resolved; it can only be used as an absolute argument.')
+                     570 BUILD_STRING             3
+         
+         343         572 PRECALL                  1
+                     576 CALL                     1
+                     586 RAISE_VARARGS            1
+         
+         348     >>  588 LOAD_FAST                0 (parser)
+                     590 LOAD_METHOD              5 (compile_filter)
+                     612 LOAD_FAST                8 (split)
+                     614 LOAD_CONST               3 (1)
+                     616 BINARY_SUBSCR
+                     626 PRECALL                  1
+                     630 CALL                     1
+                     640 LOAD_FAST                5 (kwargs)
+                     642 LOAD_FAST                9 (key)
+                     644 STORE_SUBSCR
+         
+         349         648 LOAD_CONST               5 (True)
+                     650 STORE_FAST               4 (had_kwargs)
+                     652 EXTENDED_ARG             1
+                     654 JUMP_BACKWARD          276 (to 104)
+         
+         351     >>  656 LOAD_FAST                2 (kwarg_list)
+                     658 GET_ITER
+                 >>  660 FOR_ITER                24 (to 710)
+                     662 STORE_FAST               9 (key)
+         
+         352         664 LOAD_FAST                9 (key)
+                     666 LOAD_FAST                5 (kwargs)
+                     668 CONTAINS_OP              1
+                     670 POP_JUMP_FORWARD_IF_FALSE    18 (to 708)
+         
+         353         672 LOAD_GLOBAL             13 (NULL + TemplateSyntaxError)
+         
+         354         684 LOAD_CONST               9 ('Missing required keyword argument ')
+                     686 LOAD_FAST                9 (key)
+                     688 FORMAT_VALUE             0
+                     690 BUILD_STRING             2
+         
+         353         692 PRECALL                  1
+                     696 CALL                     1
+                     706 RAISE_VARARGS            1
          
-         305         480 LOAD_FAST                0 (parser)
-                     482 LOAD_METHOD              5 (compile_filter)
-                     504 LOAD_FAST               10 (key)
-                     506 PRECALL                  1
-                     510 CALL                     1
-                     520 STORE_FAST              11 (value)
-         
-         306         522 LOAD_FAST               11 (value)
-                     524 LOAD_FAST                6 (kwargs)
-                     526 LOAD_FAST               10 (key)
-                     528 STORE_SUBSCR
-                     532 JUMP_BACKWARD          211 (to 112)
-         
-         308     >>  534 LOAD_FAST                9 (split)
-                     536 LOAD_CONST               4 (0)
-                     538 BINARY_SUBSCR
-                     548 STORE_FAST              10 (key)
-         
-         311         550 LOAD_FAST               10 (key)
-                     552 LOAD_FAST                3 (absolute_tokens)
-                     554 CONTAINS_OP              0
-                     556 POP_JUMP_FORWARD_IF_FALSE    19 (to 596)
-         
-         312         558 LOAD_GLOBAL              9 (NULL + ValueError)
-                     570 LOAD_CONST               7 ('Keyword argument ')
-                     572 LOAD_FAST               10 (key)
-                     574 FORMAT_VALUE             0
-                     576 LOAD_CONST               8 (' cannot be resolved; it will not be parsed as a variable.')
-                     578 BUILD_STRING             3
-                     580 PRECALL                  1
-                     584 CALL                     1
-                     594 RAISE_VARARGS            1
-         
-         314     >>  596 LOAD_FAST                0 (parser)
-                     598 LOAD_METHOD              5 (compile_filter)
-                     620 LOAD_FAST                9 (split)
-                     622 LOAD_CONST               3 (1)
-                     624 BINARY_SUBSCR
-                     634 PRECALL                  1
-                     638 CALL                     1
-                     648 LOAD_FAST                6 (kwargs)
-                     650 LOAD_FAST               10 (key)
-                     652 STORE_SUBSCR
-         
-         315         656 LOAD_CONST               5 (True)
-                     658 STORE_FAST               5 (had_kwargs)
-                     660 EXTENDED_ARG             1
-                     662 JUMP_BACKWARD          276 (to 112)
-         
-         317     >>  664 LOAD_FAST                2 (kwarg_list)
-                     666 GET_ITER
-                 >>  668 FOR_ITER                24 (to 718)
-                     670 STORE_FAST              12 (kwarg)
-         
-         318         672 LOAD_FAST               12 (kwarg)
-                     674 LOAD_FAST                6 (kwargs)
-                     676 CONTAINS_OP              1
-                     678 POP_JUMP_FORWARD_IF_FALSE    18 (to 716)
-         
-         319         680 LOAD_GLOBAL             13 (NULL + TemplateSyntaxError)
-                     692 LOAD_CONST               9 ('Missing required keyword argument ')
-                     694 LOAD_FAST               12 (kwarg)
-                     696 FORMAT_VALUE             0
-                     698 BUILD_STRING             2
-                     700 PRECALL                  1
-                     704 CALL                     1
-                     714 RAISE_VARARGS            1
-         
-         318     >>  716 JUMP_BACKWARD           25 (to 668)
-         
-         321     >>  718 LOAD_FAST                4 (optional_tokens)
-                     720 LOAD_METHOD              7 (items)
-                     742 PRECALL                  0
-                     746 CALL                     0
-                     756 GET_ITER
-                 >>  758 FOR_ITER                14 (to 788)
-                     760 UNPACK_SEQUENCE          2
-                     764 STORE_FAST              10 (key)
-                     766 STORE_FAST              11 (value)
-         
-         322         768 LOAD_FAST               10 (key)
-                     770 LOAD_FAST                6 (kwargs)
-                     772 CONTAINS_OP              1
-                     774 POP_JUMP_FORWARD_IF_FALSE     5 (to 786)
-         
-         323         776 LOAD_FAST               11 (value)
-                     778 LOAD_FAST                6 (kwargs)
-                     780 LOAD_FAST               10 (key)
-                     782 STORE_SUBSCR
-                 >>  786 JUMP_BACKWARD           15 (to 758)
+         352     >>  708 JUMP_BACKWARD           25 (to 660)
          
-         325     >>  788 LOAD_FAST                6 (kwargs)
-                     790 RETURN_VALUE
+         357     >>  710 LOAD_FAST                5 (kwargs)
+                     712 RETURN_VALUE
          consts
             None
             False
             '='
             1
             0
             True
             'Unexpected positional argument after keyword argument'
             'Keyword argument '
-            ' cannot be resolved; it will not be parsed as a variable.'
+            ' cannot be resolved; it can only be used as an absolute argument.'
             'Missing required keyword argument '
-         names      ('tuple', 'enumerate', 'split', 'len', 'ValueError', 'compile_filter', 'TemplateSyntaxError', 'items')
-         varnames   ('parser', 'tokens', 'kwarg_list', 'absolute_tokens', 'optional_tokens', 'had_kwargs', 'kwargs', 'i', 'token', 'split', 'key', 'value', 'kwarg')
+         names      ('tuple', 'enumerate', 'split', 'len', 'ValueError', 'compile_filter', 'TemplateSyntaxError')
+         varnames   ('parser', 'tokens', 'kwarg_list', 'absolute_tokens', 'had_kwargs', 'kwargs', 'i', 'token', 'split', 'key', 'value')
          freevars   ()
          cellvars   ()
-         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
+         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
          name       'get_kwargs'
-         firstlineno 275
+         firstlineno 309
          lnotab
-            0x02010401040204011c0204011c02040104022a012a014c011401160102
-            0204011e023e01260114011601020210012a010c021003080126023c0108
-            020801080124ff0203320108010c02
+            0x02010401040204011c0204011c022a012a014c0114011601020204011e
+            023e01260114011601020210012a010c02100308010c010aff10053c0108
+            02080108010c0108ff10ff0205
       (None,)
-      (None, None, None)
-   names      ('typing', 'Type', 'Any', 'django.template', 'library', 'Node', 'TemplateSyntaxError', 'django.template.context', 'Context', 'django.template.base', 'Parser', 'Token', 'FilterExpression', 'django.http', 'HttpRequest', 'django.utils.html', 'escape', 'django.utils.safestring', 'mark_safe', 'django.urls', 'reverse', 'django.core', 'signing', 'wagtail', 'hooks', 'wagtail.models', 'Page', 'PAGE_TEMPLATE_VAR', 'warnings', 'adapters', 'adapter_registry', 'RegistryLookUpError', 'BaseAdapter', 'AdapterError', 'utils', 'wrap_adapter', '_can_edit', 'FEDIT_PREVIEW_VAR', 'TEMPLATE_TAG_NAME', 'REGISTER_CSS', 'REGISTER_JS', 'Library', 'register', 'WARNING_FIELD_NAME_NOT_AVAILABLE', 'WARNING_MODEL_INSTANCE_NOT_AVAILABLE', 'str', 'as_var', 'AdapterNode', 'tag', 'do_render_fedit', 'simple_tag', 'render_adapter', 'inclusion_tag', 'dict', 'static_hook_output', 'tooltip', 'list', 'get_kwargs')
+      (None, None)
+   names      ('typing', 'Type', 'Any', 'django.template', 'library', 'Node', 'TemplateSyntaxError', 'django.template.context', 'Context', 'django.template.base', 'Parser', 'Token', 'FilterExpression', 'django.utils.html', 'escape', 'django.utils.safestring', 'mark_safe', 'django.core', 'signing', 'wagtail', 'hooks', 'wagtail.models', 'Page', 'PAGE_TEMPLATE_VAR', 'warnings', 'settings', 'TIPPY_ENABLED', 'adapters', 'adapter_registry', 'RegistryLookUpError', 'BaseAdapter', 'AdapterError', 'utils', 'wrap_adapter', 'with_userbar_model', 'base_adapter_context', '_flatten_context', '_can_edit', 'FEDIT_PREVIEW_VAR', 'TEMPLATE_TAG_NAME', 'FIELD_TEMPLATE_VAR', 'INSTANCE_TEMPLATE_VAR', 'REGISTER_CSS', 'REGISTER_JS', 'Library', 'register', 'WARNING_FIELD_NAME_NOT_AVAILABLE', 'WARNING_MODEL_INSTANCE_NOT_AVAILABLE', 'str', 'as_var', 'AdapterNode', 'tag', 'do_render_fedit', 'simple_tag', 'render_adapter', 'inclusion_tag', 'dict', 'static_hook_output', 'tooltip', 'do_with_userbar_model', 'list', 'get_kwargs')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
+   filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff0201100114030c0314040c010c010c010c010c020c011005080218
-      06180610061e030401040318071c5b2a010eff0e0102392a0112ff0e0102
-      152e010aff0e01021d2c0110ff0e01020f
+      0x00ff0201100114030c0314040c010c010c020c01100508020c0318062c
+      0c10061e030401040318071c6d2a010eff0e0102372a0112ff0e0102152e
+      010aff0e01021d2c0110ff0e0102122c010eff0e010207
```

### Comparing `wagtail_fedit-1.5.4rc9/wagtail_fedit/templatetags/fedit.py` & `wagtail_fedit-1.5.5rc1/wagtail_fedit/templatetags/fedit.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,40 +5,46 @@
 from django.template.context import (
     Context,
 )
 from django.template.base import (
     Parser, Token,
     FilterExpression,
 )
-from django.http import HttpRequest
 from django.utils.html import escape
 from django.utils.safestring import mark_safe
-from django.urls import reverse
 from django.core import signing
 
 from wagtail import hooks
 from wagtail.models import (
     Page,
     PAGE_TEMPLATE_VAR,
 )
 
 import warnings
 
+from ..settings import (
+    TIPPY_ENABLED,
+)
 from ..adapters import (
     adapter_registry,
     RegistryLookUpError,
     BaseAdapter,
     AdapterError,
 )
 from ..utils import (
     wrap_adapter,
     with_userbar_model,
+    base_adapter_context,
+    _flatten_context,
     _can_edit,
     FEDIT_PREVIEW_VAR,
     TEMPLATE_TAG_NAME,
+
+    FIELD_TEMPLATE_VAR,
+    INSTANCE_TEMPLATE_VAR,
 )
 from ..hooks import (
     REGISTER_CSS,
     REGISTER_JS,
 )
 
 
@@ -80,23 +86,25 @@
         model = self.model
         getters = self.getters
 
         model, kwargs = self._resolve_expressions(
             context, model, **self.kwargs,
         )
 
-        if "wagtail_fedit_field" in context\
-            and "wagtail_fedit_instance" in context\
+        if FIELD_TEMPLATE_VAR in context\
+            and INSTANCE_TEMPLATE_VAR in context\
             and not model and self.adapter.field_required:
 
-            field_name = context["wagtail_fedit_field"]
-            obj = context["wagtail_fedit_instance"]
+            field_name = context[FIELD_TEMPLATE_VAR]
+            obj = context[INSTANCE_TEMPLATE_VAR]
 
-        elif not model and "wagtail_fedit_instance" in context and not self.adapter.field_required:
-            obj = context["wagtail_fedit_instance"]
+        elif not model\
+                and INSTANCE_TEMPLATE_VAR in context\
+                and not self.adapter.field_required:
+            obj = context[INSTANCE_TEMPLATE_VAR]
             field_name = None
             
         else:
 
             if not model:
                 warnings.warn(
                     WARNING_MODEL_INSTANCE_NOT_AVAILABLE % {
@@ -120,31 +128,51 @@
                 field_name = getters[len(getters) - 1]
 
                 for i in range(len(getters) - 1):
                     getter = getters[i]
                     try:
                         obj = getattr(obj, getter)
                     except AttributeError:
-                        raise AttributeError(f"Object {model.__class__.__name__} does not have attribute {getter}")
+                        raise TemplateSyntaxError(f"Object {model.__class__.__name__} does not have attribute {getter}")
                     
 
         request = context.get("request")
         adapter = self.adapter(
             object=obj,
             field_name=field_name,
             request=request,
             **kwargs,
         )
 
-        if not adapter.check_permissions()\
-          or not _can_edit(request, obj):
-            context.update(adapter.kwargs)
-            return as_var(self.as_var, context, adapter.render_content(context))
+        context = base_adapter_context(
+            adapter,
+            context,
+        )
 
-        return as_var(self.as_var, context, wrap_adapter(request, adapter, context))
+        content = None
+        if adapter.check_permissions()\
+          and _can_edit(request, obj):
+            content = wrap_adapter(
+                request=request,
+                adapter=adapter,
+                context=context,
+                run_context_processors=False,
+            )
+
+        else:
+            _flatten_context(context)
+            content = adapter.render_content(
+                context,
+            )
+
+        return as_var(
+            self.as_var,
+            context,
+            content,
+        )
 
 
 @register.tag(name=TEMPLATE_TAG_NAME)
 def do_render_fedit(parser: Parser, token: Token):
 
     tokens = token.split_contents()
 
@@ -184,50 +212,45 @@
         tokens.pop(len(tokens)-1)
 
     kwargs = get_kwargs(
         parser,
         tokens,
         adapter.required_kwargs,
         adapter.absolute_tokens,
-        adapter.optional_kwargs,
     )
 
     return AdapterNode(
         adapter=adapter,
         model=model,
         getters=model_tokens,
         as_var=as_var,
         **kwargs,
     )
 
 
-
 @register.simple_tag(takes_context=True)
 def render_adapter(context: Context, adapter: BaseAdapter) -> str:
-    parent_context = {}
+    adapter_context = {}
     
-    if "parent_context" in context:
-        parent_context = context["parent_context"]
-        del context["parent_context"]
-
-    if hasattr(context, "flatten"):
-        context = context.flatten()
-
-    if hasattr(parent_context, "flatten"):
-        parent_context = parent_context.flatten()
-
-    context.update(parent_context)
+    if "adapter_context" in context:
+        adapter_context = context["adapter_context"]
+        del context["adapter_context"]
 
-    context["wagtail_fedit_field"]    = adapter.field_name
-    context["wagtail_fedit_instance"] = adapter.object
-    context["request"]                = adapter.request
+    context = _flatten_context(
+        context,
+    )
+    adapter_context = _flatten_context(
+        adapter_context,
+    )
 
-    context.update(adapter.kwargs)
+    context.update(adapter_context)
 
-    return adapter.render_content(context)
+    return adapter.render_content(
+        context,
+    )
 
 
 @register.inclusion_tag("wagtail_fedit/_hook_output.html", name="fedit_scripts", takes_context=True)
 def static_hook_output(context, css_or_js) -> dict:
     css_or_js = css_or_js.lower()
 
     if css_or_js not in ["css", "js"]:
@@ -254,14 +277,18 @@
         
     return {
         "hook_output": files,
     }
 
 @register.simple_tag(takes_context=False, name="tooltip")
 def tooltip(content, wrapping: str = None, **kwargs) -> str:
+
+    if not TIPPY_ENABLED:
+        return ""
+
     kwargs["content"] = content
     s = [
         "data-tooltip='true'"
     ]
     for key, value in kwargs.items():
         s.append(f"data-tooltip-{key}='{escape(value)}'")
     attrs = " ".join(s)
@@ -275,27 +302,24 @@
 def do_with_userbar_model(context, model: Any) -> str:
     if "request" in context:
         context["request"] = with_userbar_model(context["request"], model)
     if PAGE_TEMPLATE_VAR in context and context[PAGE_TEMPLATE_VAR] != model:
         context[PAGE_TEMPLATE_VAR] = model
     return ""
 
-def get_kwargs(parser: Parser, tokens: list[str], kwarg_list: list[str] = None, absolute_tokens: list[str] = None, optional_tokens: dict[str, Any] = None) -> dict:
+def get_kwargs(parser: Parser, tokens: list[str], kwarg_list: list[str] = None, absolute_tokens: list[str] = None) -> dict:
     had_kwargs = False
     kwargs = {}
 
     if not kwarg_list:
         kwarg_list = tuple()
 
     if not absolute_tokens:
         absolute_tokens = tuple()
 
-    if not optional_tokens:
-        optional_tokens = {}
-
     for i, token in enumerate(tokens):
         split = token.split("=")
         if len(split) == 1 and len(kwarg_list) > i:
             if split[0] in absolute_tokens:
                 kwargs[split[0]] = True
                 continue
 
@@ -312,22 +336,23 @@
                 value = parser.compile_filter(key)
                 kwargs[key] = value
         else:
             key = split[0]
             # if key not in kwargs_names:
             #     raise ValueError(f"Unexpected keyword argument {key}")
             if key in absolute_tokens:
-                raise ValueError(f"Keyword argument {key} cannot be resolved; it will not be parsed as a variable.")
+                raise TemplateSyntaxError(
+                    f"Keyword argument {key} cannot be resolved;"
+                    " it can only be used as an absolute argument."
+                )
             
             kwargs[key] = parser.compile_filter(split[1])
             had_kwargs = True
 
-    for kwarg in kwarg_list:
-        if kwarg not in kwargs:
-            raise TemplateSyntaxError(f"Missing required keyword argument {kwarg}")
-        
-    for key, value in optional_tokens.items():
+    for key in kwarg_list:
         if key not in kwargs:
-            kwargs[key] = value
+            raise TemplateSyntaxError(
+                f"Missing required keyword argument {key}"
+            )
 
     return kwargs
```

### Comparing `wagtail_fedit-1.5.4rc9/wagtail_fedit/test/core/migrations/0001_initial.py` & `wagtail_fedit-1.5.5rc1/wagtail_fedit/test/core/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc9/wagtail_fedit/test/core/models.py` & `wagtail_fedit-1.5.5rc1/wagtail_fedit/test/core/models.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc9/wagtail_fedit/test/core/tests/base.py` & `wagtail_fedit-1.5.5rc1/wagtail_fedit/test/core/tests/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -221,14 +221,31 @@
             f"wagtail_fedit:{url_name}",
             kwargs={
                 "object_id": model_id,
                 "app_label": app_label,
                 "model_name": model_name,
             }
         )
+    
+    def get_refetch_url(self, adapter_id, app_label, model_name, model_id, field_name = None):
+        url_name = "refetch"
+        kwgs = {
+            "adapter_id": adapter_id,
+            "app_label": app_label,
+            "model_name": model_name,
+            "model_id": model_id,
+        }
+
+        if field_name:
+            kwgs["field_name"] = field_name
+
+        return reverse(
+            f"wagtail_fedit:{url_name}",
+            kwargs=kwgs
+        )
 
     def get_field_url(self, field_name, app_label, model_name, model_id):
         url_name = "edit"
         return reverse(
             f"wagtail_fedit:{url_name}",
             kwargs={
                 "adapter_id": "field",
```

### Comparing `wagtail_fedit-1.5.4rc9/wagtail_fedit/test/core/tests/test_adapters.py` & `wagtail_fedit-1.5.5rc1/wagtail_fedit/test/core/tests/test_adapters.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,43 +8,53 @@
     Keyword,
     BaseAdapter,
     adapter_registry,
     BlockAdapter,
     FieldAdapter,
     ModelAdapter,
 )
+from wagtail_fedit.adapters.base import (
+    BlockFieldReplacementAdapter,
+)
 from wagtail_fedit.utils import (
     FEDIT_PREVIEW_VAR,
+    FIELD_TEMPLATE_VAR,
+    INSTANCE_TEMPLATE_VAR,
+    base_adapter_context,
     find_block,
 )
 from wagtail_fedit.templatetags.fedit import (
     wrap_adapter,
 )
 from .base import (
     BaseFEditTest,
 )
 
+import json
+
 adapters = {}
 
-class TestAdapter(BaseAdapter):
+class TestAdapter(BlockFieldReplacementAdapter):
     identifier = "test"
     keywords = (
         Keyword("test", help_text="A test keyword argument", type_hint="str"),
     )
     js_constructor = "wagtail_fedit.ThisDoesntGetUsedAnyways"
 
     def __init__(self, object: Model, field_name: str, request: HttpRequest, **kwargs):
         super().__init__(object, field_name, request, **kwargs)
         adapters[self.kwargs["id"]] = self
 
     def get_element_id(self) -> str:
         return f"test-{self.kwargs['id']}"
 
     def render_content(self, parent_context: dict = None) -> str:
-        return f"TestAdapter: {self.field_value}"
+        if "test" not in parent_context:
+            return f"TestAdapter: {self.field_value} ({parent_context['id']})"
+        return f"TestAdapter: {self.field_value} ({parent_context['test']}) ({parent_context['id']})"
 
 class TestContextAdapter(TestAdapter):
     identifier = "test_context"
 
     def render_content(self, parent_context: dict = None) -> str:
         return parent_context["testing"]
 
@@ -109,15 +119,15 @@
                 "request": request,
                 "object": self.basic_model,
             })
         )
 
         self.assertHTMLEqual(
             template_ok,
-            f'TestAdapter: {self.basic_model.title}'
+            f"TestAdapter: {self.basic_model.title} (test) ({id})"
         )
 
         self.assertDictEqual(
             adapters[id].kwargs,
             {"test": "test", "id": id}
         )
 
@@ -304,16 +314,19 @@
                     self.basic_model.pk, self.basic_model._meta.app_label, self.basic_model._meta.model_name,
                 )
             ),
             id=3,
         )
 
         self.assertEqual(
-            adapter.render_content(),
-            f"TestAdapter: {self.basic_model.title}"
+            adapter.render_content(base_adapter_context(
+                adapter=adapter,
+                context={},
+            )),
+            f"TestAdapter: {self.basic_model.title} (3)"
         )
 
     def test_adapter_editable(self):
         id = get_adapter_id()
         self.assertEqual(TestAdapter.required_kwargs, tuple(["test"]))
 
         tpl = Template(
@@ -339,15 +352,200 @@
                 "request": request,
                 "object": self.basic_model,
             })
         )
 
         self.assertHTMLEqual(
             tpl,
-            wrap_adapter(request, adapters[id], {})
+            wrap_adapter(request, adapters[id], base_adapter_context(
+                adapter=adapters[id],
+                context={},
+            ))
+        )
+
+    def test_adapter_editable_equals_refetch(self):
+        id = get_adapter_id()
+        self.assertEqual(TestAdapter.required_kwargs, tuple(["test"]))
+
+        tpl = Template(
+            "{% load fedit %}"
+            f"{{% fedit test object.title test='test' id='{id}' %}}"
+        )
+
+        request = self.request_factory.get(
+            self.get_editable_url(
+                self.basic_model.pk, self.basic_model._meta.app_label, self.basic_model._meta.model_name,
+            )
+        )
+        request.user = self.admin_user
+
+        setattr(
+            request,
+            FEDIT_PREVIEW_VAR,
+            True,
+        )
+
+        tpl = tpl.render(
+            Context({
+                "request": request,
+                "object": self.basic_model,
+            })
+        )
+
+        adapter = adapters[id]
+
+        self.assertEqual(
+            adapter.kwargs["test"],
+            "test",
+        )
+
+        self.assertEqual(
+            adapter.kwargs["id"],
+            id,
+        )
+
+        self.assertHTMLEqual(
+            tpl,
+            wrap_adapter(request, adapters[id], base_adapter_context(
+                adapter=adapter,
+                context={},
+            ))
+        )
+
+        url = self.get_refetch_url(
+            "test",
+            self.basic_model._meta.app_label,
+            self.basic_model._meta.model_name,
+            self.basic_model.pk,
+            "title",
+        )
+
+        self.client.force_login(self.admin_user)
+
+        response = self.client.get(url, {
+            "shared_context":\
+                adapters[id].encode_shared_context(),
+        })
+
+        json_data = json.loads(
+            response.content.decode("utf-8"),
+        )
+
+        if "html" not in json_data:
+            self.fail(f"Expected 'html' in response, got {json_data}")
+
+        if "success" not in json_data\
+            or "success" in json_data and not json_data["success"]:
+            self.fail(f"Expected 'success' in response, got {json_data}")
+
+        if "refetch" not in json_data\
+            or "refetch" in json_data and not json_data["refetch"]:
+            self.fail(f"Expected 'refetch' in response, got {json_data}")
+
+        self.assertHTMLEqual(
+            tpl,
+            json_data["html"],
+        )
+
+
+    def test_adapter_shared_context(self):
+        uid = get_adapter_id()
+        self.assertEqual(TestAdapter.required_kwargs, tuple(["test"]))
+
+        tpl = Template(
+            "{% load fedit %}"
+            f"{{% fedit test object.title test='test' id='{uid}' %}}"
+        )
+
+        request = self.request_factory.get(
+            self.get_editable_url(
+                self.basic_model.pk, self.basic_model._meta.app_label, self.basic_model._meta.model_name,
+            )
+        )
+        request.user = self.admin_user
+
+        setattr(
+            request,
+            FEDIT_PREVIEW_VAR,
+            True,
+        )
+
+        tpl = tpl.render(
+            Context({
+                "request": request,
+                "object": self.basic_model,
+            })
+        )
+
+        adapter = adapters[uid]
+
+        self.assertEqual(
+            adapter.kwargs["test"],
+            "test",
+        )
+
+        self.assertEqual(
+            adapter.kwargs["id"],
+            uid,
+        )
+
+        new_id = get_adapter_id()
+        adapter.kwargs["id"] = new_id
+        context = adapter.encode_shared_context()
+        adapter.kwargs["id"] = uid
+
+        url = self.get_refetch_url(
+            "test",
+            self.basic_model._meta.app_label,
+            self.basic_model._meta.model_name,
+            self.basic_model.pk,
+            "title",
+        )
+
+        self.client.force_login(self.admin_user)
+
+        self.assertFalse(
+            new_id in adapters,
+        )
+
+        response = self.client.get(url, {
+            "shared_context": context,
+        })
+
+        # Load if lazy
+        response.content.decode("utf-8")
+
+        self.assertTrue(
+            new_id in adapters,
+        )
+
+        self.assertFalse(
+            id(adapter) == id(adapters[new_id]),
+        )
+
+        new_adapter = adapters[new_id]
+
+        self.assertEqual(
+            new_adapter.kwargs["test"],
+            "test",
+        )
+
+        self.assertEqual(
+            adapter.kwargs["test"],
+            new_adapter.kwargs["test"],
+        )
+
+        self.assertEqual(
+            new_adapter.kwargs["id"],
+            new_id,
+        )
+
+        self.assertNotEqual(
+            adapter.kwargs["id"],
+            new_adapter.kwargs["id"],
         )
 
     def test_adapter_editable_as_var(self):
         id = get_adapter_id()
         self.assertEqual(TestAdapter.required_kwargs, tuple(["test"]))
 
         tpl = Template(
@@ -374,15 +572,18 @@
                 "request": request,
                 "object": self.basic_model,
             })
         )
 
         self.assertHTMLEqual(
             tpl,
-            wrap_adapter(request, adapters[id], {})
+            wrap_adapter(request, adapters[id], base_adapter_context(
+                adapter=adapters[id],
+                context={},
+            ))
         )
 
     def test_context_processors_run(self):
         id = get_adapter_id()
         tpl = Template(
             "{% load fedit %}"
             f"{{% fedit test_context object.title test='test' id='{id}' %}}"
@@ -408,15 +609,18 @@
                 "object": self.basic_model,
                 "testing": "testing context processor",
             }),
         )
 
         self.assertHTMLEqual(
             tpl,
-            wrap_adapter(request, adapters[id], {}, run_context_processors=True)
+            wrap_adapter(request, adapters[id], base_adapter_context(
+                adapter=adapters[id],
+                context={},
+            ), run_context_processors=True)
         )
 
 
 class TestBlockAdapter(BaseFEditTest):
 
     def test_render(self):
         id = get_adapter_id()
@@ -513,16 +717,16 @@
         )
 
         context = {
             "object": self.basic_model,
             "request": request,
             "block": block_value,
             "block_id": self.BLOCK_ID,
-            "wagtail_fedit_field": "content",
-            "wagtail_fedit_instance": self.basic_model,
+            FIELD_TEMPLATE_VAR: "content",
+            INSTANCE_TEMPLATE_VAR: self.basic_model,
         }
 
         tpl = template.render(Context(context))
 
         self.assertHTMLEqual(
             tpl,
             wrap_adapter(request, adapters[id], context)
@@ -734,15 +938,15 @@
                 "{% load fedit %}"
                 f"{{% fedit test_model from_context test=True id='{id}' %}}"
             )
     
             context = {
                 "object": self.basic_model,
                 "request": request,
-                "wagtail_fedit_instance": self.basic_model,
+                INSTANCE_TEMPLATE_VAR: self.basic_model,
             }
     
             tpl = template.render(Context(context))
     
             self.assertHTMLEqual(
                 tpl,
                 wrap_adapter(request, adapters[id], context)
```

### Comparing `wagtail_fedit-1.5.4rc9/wagtail_fedit/test/core/tests/test_block_edit.py` & `wagtail_fedit-1.5.5rc1/wagtail_fedit/test/core/tests/test_block_edit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc9/wagtail_fedit/test/core/tests/test_blocks.py` & `wagtail_fedit-1.5.5rc1/wagtail_fedit/test/core/tests/test_blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc9/wagtail_fedit/test/core/tests/test_field_edit.py` & `wagtail_fedit-1.5.5rc1/wagtail_fedit/test/core/tests/test_field_edit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc9/wagtail_fedit/test/core/tests/test_generic.py` & `wagtail_fedit-1.5.5rc1/wagtail_fedit/test/core/tests/test_generic.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc9/wagtail_fedit/test/core/tests/test_model_edit.py` & `wagtail_fedit-1.5.5rc1/wagtail_fedit/test/core/tests/test_model_edit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc9/wagtail_fedit/test/core/tests/test_revision.py` & `wagtail_fedit-1.5.5rc1/wagtail_fedit/test/core/tests/test_revision.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc9/wagtail_fedit/test/core/tests/test_submit.py` & `wagtail_fedit-1.5.5rc1/wagtail_fedit/test/core/tests/test_submit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc9/wagtail_fedit/test/manage.py` & `wagtail_fedit-1.5.5rc1/wagtail_fedit/test/manage.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc9/wagtail_fedit/test/testapp/settings.py` & `wagtail_fedit-1.5.5rc1/wagtail_fedit/test/testapp/settings.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc9/wagtail_fedit/test/testapp/urls.py` & `wagtail_fedit-1.5.5rc1/wagtail_fedit/test/testapp/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc9/wagtail_fedit/toolbar.py` & `wagtail_fedit-1.5.5rc1/wagtail_fedit/toolbar.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc9/wagtail_fedit/urls.py` & `wagtail_fedit-1.5.5rc1/wagtail_fedit/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc9/wagtail_fedit/utils.py` & `wagtail_fedit-1.5.5rc1/wagtail_fedit/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,18 @@
-from typing import Any, TYPE_CHECKING
+from typing import (
+    Any, TYPE_CHECKING, Union,
+)
 from collections import namedtuple
 from urllib.parse import urlencode
 from django.db import models
 from django.http import HttpRequest
 from django.utils.safestring import mark_safe
 from django.utils.translation import gettext_lazy as _
 from django.template.loader import render_to_string
+from django.template import Context
 from django.conf import settings
 from django.urls import reverse
 
 from wagtail.models import (
     DraftStateMixin,
     WorkflowMixin,
     LockableMixin,
@@ -36,17 +39,29 @@
 )
 
 
 if TYPE_CHECKING:
     from .adapters.base import BaseAdapter
 
 
+# Name of the template tag
+# Example: `{% fedit adapter_identifier instance.field %}
 TEMPLATE_TAG_NAME = "fedit"
+
+# Context variables
+FIELD_TEMPLATE_VAR = "wagtail_fedit_field"
+INSTANCE_TEMPLATE_VAR = "wagtail_fedit_instance"
+ADAPTER_TEMPLATE_VAR = "wagtail_fedit_adapter"
+
+# Request variables
 FEDIT_PREVIEW_VAR = "_wagtail_fedit_preview"
 USERBAR_MODEL_VAR = "_wagtail_fedit_userbar_model"
+
+# Include log actions in the userbar
+# Breaks in Wagtail 6.1.0
 LOG_ACTION_TEMPLATES_AVAILABLE = WAGTAIL_VERSION < (6, 1, 0)
 
 
 class FeditPermissionCheck:
     @staticmethod
     def has_perms(request: HttpRequest, model: Any) -> bool:
 
@@ -234,16 +249,15 @@
     We wil also check for any hooks which may convert the content.
     """
     _look_for_renderers()
 
     if isinstance(meta_field, str):
         meta_field = instance._meta.get_field(meta_field)
 
-    if hasattr(context, "flatten"):
-        context = context.flatten()
+    context = _flatten_context(context)
 
     if not content:
         # Check for a rendering method if it exists
         if hasattr(instance, f"render_fedit_{meta_field.name}"):
             content = getattr(instance, f"render_fedit_{meta_field.name}")(request, context=context)
         else:
             content = getattr(instance, meta_field.name)
@@ -454,14 +468,35 @@
         )
     else:
         lock = None
         locked_for_user = False
 
     return _lock_info(lock, locked_for_user)
 
+def _flatten_context(context: dict) -> dict:
+    if hasattr(context, "flatten"):
+        return context.flatten()
+    return context
+
+def base_adapter_context(adapter: "BaseAdapter", context: Union[Context, dict]) -> dict:
+    """
+    Return the base context for an adapter.
+    """
+
+    if not context:
+        context = {}
+
+    context.update(adapter.kwargs)
+
+    context[FIELD_TEMPLATE_VAR]    = adapter.field_name
+    context[INSTANCE_TEMPLATE_VAR] = adapter.object
+    context[ADAPTER_TEMPLATE_VAR]  = adapter
+
+    return context
+
 
 def wrap_adapter(request: HttpRequest, adapter: "BaseAdapter", context: dict, run_context_processors: bool = False) -> str:
     if not context:
         context = {}
 
     items: list[FeditAdapterComponent] = [
         *adapter.get_toolbar_buttons(),
@@ -472,17 +507,17 @@
         hook(items=items, adapter=adapter)
 
     items = [item.render() for item in items]
     items = list(filter(None, items))
 
     reverse_kwargs = {
         "adapter_id": adapter.identifier,
-        "app_label": adapter.object._meta.app_label,
+        "app_label":  adapter.object._meta.app_label,
         "model_name": adapter.object._meta.model_name,
-        "model_id": adapter.object.pk,
+        "model_id":   adapter.object.pk,
     }
 
     if adapter.field_name is not None:
         reverse_kwargs["field_name"] = adapter.field_name
 
     shared = adapter.encode_shared_context()
     js_constructor = adapter.get_js_constructor()
@@ -493,15 +528,15 @@
             "identifier": adapter.identifier,
             "adapter": adapter,
             "buttons": items,
             "shared": shared,
             "unique_id": adapter.get_element_id(),
             "js_constructor": js_constructor,
             "shared_context": adapter.kwargs,
-            "parent_context": context,
+            "adapter_context": context,
             "edit_url": reverse(
                 "wagtail_fedit:edit",
                 kwargs=reverse_kwargs,
             ),
             "refetch_url": reverse(
                 "wagtail_fedit:refetch",
                 kwargs=reverse_kwargs,
```

### Comparing `wagtail_fedit-1.5.4rc9/wagtail_fedit/views/adapters.py` & `wagtail_fedit-1.5.5rc1/wagtail_fedit/views/adapters.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,40 +1,50 @@
 from typing import Any
-from django.shortcuts import render
+from django.apps import apps
 from django.utils.translation import gettext as _
 from django.utils.decorators import method_decorator
 from django.template.loader import render_to_string
-from django.views.decorators.clickjacking import xframe_options_sameorigin
+from django.views.decorators.clickjacking import (
+    xframe_options_sameorigin,
+)
 from django.views.generic import View
+from django.shortcuts import render
 from django.http import (
     HttpRequest,
     HttpResponseBadRequest,
     HttpResponseForbidden,
     JsonResponse,
     HttpResponse,
 )
-from django.apps import apps
 from wagtail.models import (
     RevisionMixin,
     PAGE_TEMPLATE_VAR,
     Page,
 )
-from wagtail.admin.views.generic import WagtailAdminTemplateMixin
+from wagtail.admin.views.generic import (
+    WagtailAdminTemplateMixin,
+)
 
 from ..adapters import (
     adapter_registry,
     BaseAdapter,
     RegistryLookUpError,
 )
 from ..utils import (
     FeditPermissionCheck,
     FeditIFrameMixin,
     FEDIT_PREVIEW_VAR,
+    base_adapter_context,
     lock_info,
 )
+from ..errors import (
+    NO_PERMISSION_ACTION,
+    INVALID,
+    REQUIRED,
+)
 from .mixins import (
     LocaleMixin,
 )
 
 @method_decorator(xframe_options_sameorigin, name="dispatch")
 class BaseAdapterView(FeditIFrameMixin, FeditPermissionCheck, WagtailAdminTemplateMixin, View):
     ERROR_TITLE = _("Validation Errors")
@@ -48,39 +58,63 @@
             field_name: str = None,
         ) -> None:
 
         # Fetch the adapter class from the registry
         try:
             self.adapter_class: BaseAdapter = adapter_registry[adapter_id]
         except RegistryLookUpError:
-            return HttpResponseBadRequest("Invalid adapter ID")
+            return HttpResponseBadRequest(
+                INVALID.format(
+                    _("Adapter ID")
+                )
+            )
 
         # Retrieve the model class
         try:
             self.model = apps.get_model(app_label, model_name)
-            if not self.has_perms(request, self.model):
-                return HttpResponseForbidden("You do not have permission to view this page")
         except LookupError:
-            return HttpResponseBadRequest("Invalid model")
+            return HttpResponseBadRequest(
+                INVALID.format(
+                    _("Model")
+                )
+            )
+        
+        # Check if the user has permissions to view the page
+        if not self.has_perms(request, self.model):
+            return HttpResponseForbidden(NO_PERMISSION_ACTION.format(
+                _("view this page")
+            ))
 
         # Only fetch latest reivision if it exists
         # If not; it will be automatically created by the form.
         model_instance = self.model._default_manager.get(pk=model_id)
         if isinstance(model_instance, RevisionMixin) and model_instance.latest_revision_id:
             self.instance = model_instance.latest_revision.as_object()
         else:
             self.instance = model_instance
 
-        LocaleMixin.setup_locale(self.instance)
+        LocaleMixin.setup_locale(
+            self.instance,
+        )
 
         if not field_name and self.adapter_class.field_required:
-            return HttpResponseBadRequest("Field name is required for object")
+            return HttpResponseBadRequest(
+                REQUIRED.format(
+                    _("Field name"),
+                    self.instance,
+                )
+            )
 
         if field_name and not hasattr(self.instance, field_name) and self.adapter_class.field_required:
-            return HttpResponseBadRequest("Invalid field name for object")
+            return HttpResponseBadRequest(
+                INVALID.format(
+                    _("field name"),
+                    self.instance,
+                )
+            )
 
         shared_context = request.GET.get("shared_context")
         if shared_context:
             self.shared_context = self.adapter_class.decode_shared_context(
                 request,
                 self.instance,
                 field_name,
@@ -92,14 +126,21 @@
         self.adapter = self.adapter_class(
             request=request,
             object=self.instance,
             field_name=field_name,
             **self.shared_context,
         )
 
+        if not self.adapter.check_permissions():
+            return HttpResponseForbidden(
+                NO_PERMISSION_ACTION.format(
+                    _("edit this field")
+                )
+            )
+
         self.lock, self.locked_for_user = lock_info(
             self.adapter.object, request.user,
         )
 
         setattr(
             self.request,
             FEDIT_PREVIEW_VAR,
@@ -148,34 +189,41 @@
                 self.request.GET["shared_context"]
 
         verbose_name = self.model._meta.verbose_name
         if self.adapter.field_required:
             verbose_name = self.adapter.meta_field.verbose_name
 
         extra = {}
-        if "form" in kwargs:
-            extra.update(
-                self.adapter.get_form_context(
-                    **kwargs,
-                ),
-            )
 
         if isinstance(self.instance, Page):
             # Add the page template variable to the context.
             # Wagtail uses this internally; for example in `{% wagtailpagecache %}`
             extra[PAGE_TEMPLATE_VAR] = self.instance
 
-        return super().get_context_data(**kwargs) | {
-            "verbose_name": verbose_name,
-            "locked_for_user": self.locked_for_user,
-            "shared_context": shared_context,
-            "form_attrs": self.adapter.get_form_attrs(),
-            "locked": self.lock is not None,
-            **extra,
-        }
+        # Form context; used for rendering the modal.
+        if "form" in kwargs:
+            extra.update({
+                "verbose_name": verbose_name,
+                "locked_for_user": self.locked_for_user,
+                "shared_context": shared_context,
+                "form_attrs": self.adapter.get_form_attrs(),
+                "locked": self.lock is not None,
+                **self.adapter.get_form_context(
+                    **kwargs,
+                ),
+            })
+        # Add adapter context instead of form context
+        else:
+            extra = base_adapter_context(
+                self.adapter,
+                extra,
+            )
+
+        return super().get_context_data(**kwargs)\
+            | extra
     
 class AdapterRefetchView(BaseAdapterView):
     def get(self, request: HttpRequest, *args: Any, **kwargs: Any) -> HttpResponse:
         context = self.get_context_data()
 
         return JsonResponse({
             "success": True,
```

### Comparing `wagtail_fedit-1.5.4rc9/wagtail_fedit/views/editable.py` & `wagtail_fedit-1.5.5rc1/wagtail_fedit/views/editable.py`

 * *Files 10% similar despite different names*

```diff
@@ -28,27 +28,36 @@
     DraftStateMixin,
     WorkflowMixin,
     WorkflowState,
     PageLogEntry,
     ModelLogEntry,
     Page,
 )
-from .. import forms as block_forms
 from ..utils import (
     FEDIT_PREVIEW_VAR,
     USERBAR_MODEL_VAR,
     LOG_ACTION_TEMPLATES_AVAILABLE,
     FeditPermissionCheck,
     with_userbar_model,
     # user_can_publish,
     # user_can_unpublish,
     # user_can_submit_for_moderation,
     # lock_info,
 )
-
+from ..errors import (
+    NO_PERMISSION_VIEW,
+    NO_PERMISSION_ACTION,
+    NO_WORKFLOW_STATE,
+    OBJECT_LOCKED,
+    OBJECT_NOT_LIVE,
+    ACTION_MISSING,
+    INVALID_ACTION,
+    MISSING_REQUIRED_SUPERCLASSES,
+    NO_UNPUBLISHED_CHANGES,
+)
 from .mixins import (
     ObjectViewMixin,
     LockViewMixin,
     LocaleMixin,
 )
 
 
@@ -63,21 +72,22 @@
 
 def get_publish_action(object):
     if isinstance(object, Page):
         return PublishPageRevisionAction
     return PublishRevisionAction
 
 
+
 class BaseFeditView(LocaleMixin, ObjectViewMixin, FeditPermissionCheck, TemplateView):
     def dispatch(self, request: HttpRequest, object_id: Any, app_label: str, model_name: str) -> HttpResponse:
         if self.error_response:
             return self.error_response
 
         if not self.has_perms(request, self.object):
-            return HttpResponseForbidden("You do not have permission to view this page")
+            return HttpResponseForbidden(NO_PERMISSION_VIEW)
 
         if issubclass(self.model, RevisionMixin) and self.object.latest_revision_id:
             instance: RevisionMixin  = self.object
             revision: RevisionMixin = instance.latest_revision
             self.object = revision.as_object()
             self.is_preview = True
         else:
@@ -101,15 +111,15 @@
 
 
 class FEditableView(BaseFeditView):
 
     def checks(self, request: HttpRequest, object: Any) -> None:
         super().checks(request, object)
         if not isinstance(self.object, PreviewableMixin):
-            raise ValueError("Model {} does not inherit from PreviewableMixin, cannot edit.".format(self.model))
+            raise ValueError(MISSING_REQUIRED_SUPERCLASSES.format(self.model))
 
     def get(self, request: HttpRequest, *args: Any, **kwargs: Any) -> HttpResponse:
         # # Check if lock applies to this user
         # if not self.locked_for_user:
         self.request = with_userbar_model(self.request, self.object)
 
         object: PreviewableMixin = self.object
@@ -148,16 +158,18 @@
     
     def setup(self, request: HttpRequest, object_id: Any, app_label: str, model_name: str) -> HttpResponse:
         super().setup(request, object_id, app_label, model_name)
         self.policy = self.object.permissions_for_user(request.user)
 
         if not isinstance(self.object, tuple(self.required_superclasses)):
             self.error_response = HttpResponseBadRequest(
-                "Model {} does not inherit from {}".format(
-                    self.model.__name__, ", ".join([cls.__name__ for cls in self.required_superclasses])
+                MISSING_REQUIRED_SUPERCLASSES.format(
+                    self.model.__name__, ", ".join(
+                        [cls.__name__ for cls in self.required_superclasses],
+                    )
                 )
             )
 
     def get_context_data(self, **kwargs: Any) -> dict[str, Any]:
         return super().get_context_data(**kwargs) | {
             "action": self.get_action_value(),  # e.g. "publishview"
             "action_text": self.get_action(),
@@ -215,24 +227,24 @@
             self.check_policy(request, self.policy)
         except ValueError as e:
             messages.error(request, str(e))
             return self.get(request, *args, **kwargs)
 
         # Check if lock applies to this user
         if self.locked_for_user:
-            messages.error(request, _("This object is locked. It cannot be acted upon."))
+            messages.error(request, OBJECT_LOCKED)
             return self.redirect_to_failsafe_url(request)
         
         if "action" not in request.POST:
-            messages.error(request, _("No action specified"))
-            return self.get(request, *args, **kwargs)
+            messages.error(request, ACTION_MISSING)
+            return redirect(request.path)
         
         if request.POST["action"] != self.get_action_value():
-            messages.error(request, _("Invalid action specified: {}").format(request.POST["action"]))
-            return self.get(request, *args, **kwargs)
+            messages.error(request, INVALID_ACTION.format(request.POST["action"]))
+            return redirect(request.path)
         
         return self.action(request)
 
 
 class PublishView(BaseActionView):
     template_name = "wagtail_fedit/editor/action_publish_confirm.html"
     required_superclasses = [DraftStateMixin, RevisionMixin]
@@ -317,21 +329,23 @@
             "LOG_ACTION_TEMPLATES_AVAILABLE": LOG_ACTION_TEMPLATES_AVAILABLE,
         })
 
         return context
 
     def check_policy(self, request: HttpRequest, policy: FeditPermissionCheck) -> None:
         if not policy.can_publish():
-            raise ValueError("User does not have permission to publish")
+            raise ValueError(str(NO_PERMISSION_ACTION.format(
+                _("publish")
+            )))
         
         if self.locked_for_user:
-            raise ValueError("Object is locked")
+            raise ValueError(str(OBJECT_LOCKED))
         
         if not self.object.has_unpublished_changes:
-            raise ValueError("Object has no unpublished changes")
+            raise ValueError(str(NO_UNPUBLISHED_CHANGES))
 
     def action(self, request: HttpRequest) -> HttpResponse:
         latest_revision = self.object.latest_revision
 
         if not latest_revision:
             latest_revision = self.object.save_revision(
                 user=request.user,
@@ -362,25 +376,27 @@
     ]
 
     def get_action_title(self):
         return _("Unpublishing {} \"{}\"").format(self.object._meta.verbose_name, self.object)
     
     def check_policy(self, request: HttpRequest, policy: FeditPermissionCheck) -> None:
         if not policy.can_unpublish():
-            raise ValueError("User does not have permission to unpublish")
+            raise ValueError(str(NO_PERMISSION_ACTION.format(
+                _("unpublish")
+            )))
         
         if self.locked_for_user:
-            raise ValueError("Object is locked")
+            raise ValueError(str(OBJECT_LOCKED))
         
         if not self.object.live:
-            raise ValueError("Object is not live")
+            raise ValueError(str(OBJECT_NOT_LIVE))
  
     def action(self, request: HttpRequest) -> HttpResponse:
         if not self.object.live:
-            messages.error(request, _("This object is not live"))
+            messages.error(request, OBJECT_NOT_LIVE)
             return self.get(request)
         
         action = get_unpublish_action(self.object)(
             self.object,
             user=request.user,
         )
 
@@ -401,18 +417,20 @@
     ]
 
     def get_action_title(self):
         return _("Submitting {} \"{}\" for moderation").format(self.object._meta.verbose_name, self.object)
 
     def check_policy(self, request: HttpRequest, policy: FeditPermissionCheck) -> None:
         if not policy.can_submit_for_moderation():
-            raise ValueError("User does not have permission to submit for moderation")
+            raise ValueError(str(NO_PERMISSION_ACTION.format(
+                _("submit for moderation")
+            )))
         
         if not self.object.has_unpublished_changes:
-            raise ValueError("Object has no unpublished changes")
+            raise ValueError(str(NO_UNPUBLISHED_CHANGES))
    
     def action(self, request: HttpRequest) -> HttpResponse:
         
         latest_revision = getattr(self.object, "latest_revision", None)
         if not latest_revision:
             latest_revision = self.object.save_revision(
                 user=request.user,
@@ -444,18 +462,20 @@
     ]
 
     def get_action_title(self):
         return _("Cancelling workflow for {} \"{}\"").format(self.object._meta.verbose_name, self.object)
 
     def check_policy(self, request: HttpRequest, policy: FeditPermissionCheck) -> None:
         if not self.workflow_state:
-            raise ValueError("No workflow state found")
+            raise ValueError(str(NO_WORKFLOW_STATE))
         
         if not self.workflow_state.user_can_cancel(request.user):
-            raise ValueError("User does not have permission to cancel this workflow")
+            raise ValueError(str(NO_PERMISSION_ACTION.format(
+                _("cancel the workflow")
+            )))
 
     def action(self, request: HttpRequest) -> HttpResponse:
         if self.workflow_state:
             self.workflow_state.cancel(user=self.request.user)
             return self.redirect_to_success_url(request)
         
         return self.get(request)
```

### Comparing `wagtail_fedit-1.5.4rc9/wagtail_fedit/views/mixins.py` & `wagtail_fedit-1.5.5rc1/wagtail_fedit/views/mixins.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,33 +1,45 @@
 from typing import Any
 from django.utils import translation
+from django.utils.translation import gettext_lazy as _
 from django.apps import apps
 from django.http import (
     HttpRequest,
     HttpResponseBadRequest,
     HttpResponse,
 )
 from ..utils import (
     lock_info,
 )
-
+from ..errors import (
+    INVALID,
+    MODEL_NOT_FOUND,
+)
 
 
 
 class ObjectViewMixin:
     def setup(self, request: HttpRequest, object_id: Any, app_label: str, model_name: str) -> HttpResponse:
         super().setup(request, object_id, app_label, model_name)
         try:
             self.model = apps.get_model(app_label, model_name)
             self.object = self.model._default_manager.get(pk=object_id)
             self.error_response = None
         except (LookupError):
-            self.error_response = HttpResponseBadRequest("Invalid model provided")
+            self.error_response = HttpResponseBadRequest(
+                INVALID.format(_("model provided"))
+            )
+            self.object = None
+            self.model = None
         except (self.model.DoesNotExist):
-            self.error_response = HttpResponseBadRequest("Model not found")
+            self.error_response = HttpResponseBadRequest(
+                MODEL_NOT_FOUND
+            )
+            self.object = None
+            self.model = None
 
 
     def dispatch(self, request: HttpRequest, object_id: Any, app_label: str, model_name: str) -> HttpResponse:
         if self.error_response:
             return self.error_response
 
         return super().dispatch(request, object_id, app_label, model_name)
```

### Comparing `wagtail_fedit-1.5.4rc9/wagtail_fedit/wagtail_hooks/action_menu.py` & `wagtail_fedit-1.5.5rc1/wagtail_fedit/wagtail_hooks/action_menu.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc9/wagtail_fedit/wagtail_hooks/adapter_hooks.py` & `wagtail_fedit-1.5.5rc1/wagtail_fedit/wagtail_hooks/adapter_hooks.py`

 * *Files 11% similar despite different names*

```diff
@@ -74,26 +74,14 @@
             '<link rel="stylesheet" href="{0}">',
             static('wagtail_fedit/css/frontend.css')
         ),
     ]
 
 @hooks.register(REGISTER_JS, order=-1)
 def register_js(request):
-    scripts = []
-    if TIPPY_ENABLED:
-        scripts.extend([
-            format_html(
-                '<script src="{0}"></script>',
-                static('wagtail_fedit/vendor/tippy/popper.min.js')
-            ),
-            format_html(
-                '<script src="{0}"></script>',
-                static('wagtail_fedit/vendor/tippy/tippy-bundle.min.js')
-            ),
-        ])
-    scripts.extend([
+    scripts = [
         format_html(
             '<script src="{0}"></script>',
-            static('wagtail_fedit/js/frontend.js')
+            static('wagtail_fedit/js/edit.js')
         ),
-    ])
+    ]
     return scripts
```

#### html2text {}

```diff
@@ -20,13 +20,9 @@
 (FIELD_EDITOR_SIZE) def field_editor_size(model_instance, model_field): if
 isinstance(model_field, RichTextField): return "large" if isinstance
 (model_field, StreamField): return "full" return None #
 #
 @hooks.register(REGISTER_CSS, order=-1) def register_css(request): return
 [ format_html( '
 ', static('wagtail_fedit/css/frontend.css') ), ] @hooks.register(REGISTER_JS,
-order=-1) def register_js(request): scripts = [] if TIPPY_ENABLED:
-scripts.extend([ format_html( '
-', static('wagtail_fedit/vendor/tippy/popper.min.js') ), format_html( '
-', static('wagtail_fedit/vendor/tippy/tippy-bundle.min.js') ), ])
-scripts.extend([ format_html( '
-', static('wagtail_fedit/js/frontend.js') ), ]) return scripts
+order=-1) def register_js(request): scripts = [ format_html( '
+', static('wagtail_fedit/js/edit.js') ), ] return scripts
```

### Comparing `wagtail_fedit-1.5.4rc9/wagtail_fedit/wagtail_hooks/log_actions.py` & `wagtail_fedit-1.5.5rc1/wagtail_fedit/wagtail_hooks/log_actions.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,14 +44,28 @@
                     "old": old,
                     "new": new,
                 }
             
             except KeyError:
                 return _("Edit Field")
 
+    @actions.register_action("wagtail_fedit.edit_model")
+    class ModelChangedFormatter(LogFormatter):
+        label = _("Model Changed (Frontend)")
+        message = _("A model was changed from the frontend")
+
+        def format_message(self, log_entry):
+            data = log_entry.data
+
+            if not "model_verbose" in data:
+                return self.label
+            
+            return _("Changed '%(model)s' (Frontend)") % {
+                "model": gettext(data["model_verbose"]),
+            }
             
     @actions.register_action("wagtail_fedit.edit_block")
     class BlockChangedFormatter(LogFormatter):
         label = _("Block Changed (Frontend)")
         message = _("A block was changed from the frontend")
         must = [
             "block_id",
```

### Comparing `wagtail_fedit-1.5.4rc9/wagtail_fedit/wagtail_hooks/userbar.py` & `wagtail_fedit-1.5.5rc1/wagtail_fedit/wagtail_hooks/userbar.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc9/wagtail_fedit.egg-info/SOURCES.txt` & `wagtail_fedit-1.5.5rc1/wagtail_fedit.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 wagtail_fedit/__init__.py
 wagtail_fedit/apps.py
+wagtail_fedit/errors.py
 wagtail_fedit/hooks.py
 wagtail_fedit/models.py
 wagtail_fedit/settings.py
 wagtail_fedit/toolbar.py
 wagtail_fedit/urls.py
 wagtail_fedit/utils.py
 wagtail_fedit.egg-info/PKG-INFO
@@ -31,18 +32,17 @@
 wagtail_fedit/locale/nl/LC_MESSAGES/django.mo
 wagtail_fedit/locale/nl/LC_MESSAGES/django.po
 wagtail_fedit/migrations/__init__.py
 wagtail_fedit/migrations/__pycache__/__init__.cpython-311.pyc
 wagtail_fedit/static/wagtail_fedit/css/frontend.css
 wagtail_fedit/static/wagtail_fedit/css/furniture.css
 wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css
+wagtail_fedit/static/wagtail_fedit/js/edit.js
 wagtail_fedit/static/wagtail_fedit/js/frontend.js
-wagtail_fedit/static/wagtail_fedit/vendor/tippy/LICENSE
-wagtail_fedit/static/wagtail_fedit/vendor/tippy/popper.min.js
-wagtail_fedit/static/wagtail_fedit/vendor/tippy/tippy-bundle.min.js
+wagtail_fedit/static/wagtail_fedit/js/licenses/TIPPY.LICENSE
 wagtail_fedit/templates/wagtail_fedit/_hook_output.html
 wagtail_fedit/templates/wagtail_fedit/content/editable_adapter.html
 wagtail_fedit/templates/wagtail_fedit/content/buttons/admin_link.html
 wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_adapter.html
 wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html
 wagtail_fedit/templates/wagtail_fedit/editor/action_publish_confirm.html
 wagtail_fedit/templates/wagtail_fedit/editor/adapter_edit_handler.html
```

