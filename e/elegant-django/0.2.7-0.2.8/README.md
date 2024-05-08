# Comparing `tmp/elegant_django-0.2.7.tar.gz` & `tmp/elegant_django-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elegant_django-0.2.7.tar", max compression
+gzip compressed data, was "elegant_django-0.2.8.tar", max compression
```

## Comparing `elegant_django-0.2.7.tar` & `elegant_django-0.2.8.tar`

### file list

```diff
@@ -1,138 +1,157 @@
--rw-r--r--   0        0        0    18512 2024-02-28 02:21:27.175943 elegant_django-0.2.7/LICENSE
--rw-r--r--   0        0        0     1174 2024-02-28 02:21:27.175943 elegant_django-0.2.7/README.md
--rw-r--r--   0        0        0      250 2024-02-28 02:21:27.175943 elegant_django-0.2.7/elegant/__init__.py
--rw-r--r--   0        0        0     6743 2024-02-28 02:21:27.183942 elegant_django-0.2.7/elegant/admin.py
--rw-r--r--   0        0        0      184 2024-02-28 02:21:27.183942 elegant_django-0.2.7/elegant/apps.py
--rw-r--r--   0        0        0     2142 2024-02-28 02:21:27.183942 elegant_django-0.2.7/elegant/cache.py
--rw-r--r--   0        0        0      244 2024-02-28 02:21:27.183942 elegant_django-0.2.7/elegant/compat.py
--rw-r--r--   0        0        0      777 2024-02-28 02:21:27.183942 elegant_django-0.2.7/elegant/components.py
--rw-r--r--   0        0        0     2262 2024-02-28 02:21:27.183942 elegant_django-0.2.7/elegant/config.py
--rw-r--r--   0        0        0      675 2024-02-28 02:21:27.183942 elegant_django-0.2.7/elegant/constants.py
--rwxr-xr-x   0        0        0      670 2024-02-28 02:21:27.183942 elegant_django-0.2.7/elegant/context_processors.py
--rw-r--r--   0        0        0      137 2024-02-28 02:21:27.183942 elegant_django-0.2.7/elegant/mixins/__init__.py
--rw-r--r--   0        0        0     6728 2024-02-28 02:21:27.183942 elegant_django-0.2.7/elegant/mixins/actions.py
--rw-r--r--   0        0        0    19214 2024-02-28 02:21:27.183942 elegant_django-0.2.7/elegant/mixins/confirm.py
--rw-r--r--   0        0        0    12300 2024-02-28 02:21:27.183942 elegant_django-0.2.7/elegant/mixins/objects.py
--rw-r--r--   0        0        0   107369 2024-02-28 02:21:27.183942 elegant_django-0.2.7/elegant/static/elegant/bootstrap/css/bootstrap.min.css
--rw-r--r--   0        0        0    27257 2024-02-28 02:21:27.183942 elegant_django-0.2.7/elegant/static/elegant/bootstrap/img/glyphicons-halflings-white-shadow.png
--rw-r--r--   0        0        0     8777 2024-02-28 02:21:27.191942 elegant_django-0.2.7/elegant/static/elegant/bootstrap/img/glyphicons-halflings-white.png
--rw-r--r--   0        0        0    12799 2024-02-28 02:21:27.191942 elegant_django-0.2.7/elegant/static/elegant/bootstrap/img/glyphicons-halflings.png
--rw-r--r--   0        0        0    15753 2024-02-28 02:21:27.191942 elegant_django-0.2.7/elegant/static/elegant/bootstrap/js/bootstrap.min.js
--rw-r--r--   0        0        0      528 2024-02-28 02:21:27.191942 elegant_django-0.2.7/elegant/static/elegant/css/confirmation.css
--rw-r--r--   0        0        0      615 2024-02-28 02:21:27.191942 elegant_django-0.2.7/elegant/static/elegant/css/dashboard.css
--rw-r--r--   0        0        0      408 2024-02-28 02:21:27.191942 elegant_django-0.2.7/elegant/static/elegant/css/date_range_filter.css
--rw-r--r--   0        0        0    25774 2024-02-28 02:21:27.191942 elegant_django-0.2.7/elegant/static/elegant/css/djangocms.css
--rw-r--r--   0        0        0    62642 2024-02-28 02:21:27.195942 elegant_django-0.2.7/elegant/static/elegant/css/elegant.css
--rw-r--r--   0        0        0      150 2024-02-28 02:21:27.195942 elegant_django-0.2.7/elegant/static/elegant/css/extra.css
--rw-r--r--   0        0        0     3881 2024-02-28 02:21:27.195942 elegant_django-0.2.7/elegant/static/elegant/css/filer.css
--rw-r--r--   0        0        0       63 2024-02-28 02:21:27.195942 elegant_django-0.2.7/elegant/static/elegant/css/forms.css
--rw-r--r--   0        0        0     2362 2024-02-28 02:21:27.195942 elegant_django-0.2.7/elegant/static/elegant/css/jquery.dropdown.min.css
--rw-r--r--   0        0        0        0 2024-02-28 02:21:27.195942 elegant_django-0.2.7/elegant/static/elegant/css/shortcuts.css
--rw-r--r--   0        0        0     1737 2024-02-28 02:21:27.195942 elegant_django-0.2.7/elegant/static/elegant/img/ajax-loader.gif
--rw-r--r--   0        0        0      105 2024-02-28 02:21:27.195942 elegant_django-0.2.7/elegant/static/elegant/img/bg_left_white.gif
--rw-r--r--   0        0        0    41210 2024-02-28 02:21:27.195942 elegant_django-0.2.7/elegant/static/elegant/img/bg_pattern.jpg
--rw-r--r--   0        0        0      432 2024-02-28 02:21:27.195942 elegant_django-0.2.7/elegant/static/elegant/img/cc_active_nav.png
--rw-r--r--   0        0        0      132 2024-02-28 02:21:27.195942 elegant_django-0.2.7/elegant/static/elegant/img/drag-handle.png
--rw-r--r--   0        0        0    40145 2024-02-28 02:21:27.195942 elegant_django-0.2.7/elegant/static/elegant/img/glyphicons-halflings-white-nav.png
--rw-r--r--   0        0        0    27257 2024-02-28 02:21:27.195942 elegant_django-0.2.7/elegant/static/elegant/img/glyphicons-halflings-white-shadow.png
--rw-r--r--   0        0        0      394 2024-02-28 02:21:27.195942 elegant_django-0.2.7/elegant/static/elegant/js/djangocms.js
--rw-r--r--   0        0        0     2305 2024-02-28 02:21:27.203942 elegant_django-0.2.7/elegant/static/elegant/js/elegant-form-confirm.js
--rw-r--r--   0        0        0     6912 2024-02-28 02:21:27.203942 elegant_django-0.2.7/elegant/static/elegant/js/elegant.js
--rw-r--r--   0        0        0    85578 2024-02-28 02:21:27.203942 elegant_django-0.2.7/elegant/static/elegant/js/jquery-2.2.4.min.js
--rw-r--r--   0        0        0    37490 2024-02-28 02:21:27.203942 elegant_django-0.2.7/elegant/static/elegant/js/jquery-ui-1.10.3.sortable.min.js
--rw-r--r--   0        0        0     3270 2024-02-28 02:21:27.203942 elegant_django-0.2.7/elegant/static/elegant/js/jquery.autosize-min.js
--rw-r--r--   0        0        0     5165 2024-02-28 02:21:27.203942 elegant_django-0.2.7/elegant/static/elegant/js/jquery.dropdown.js
--rw-r--r--   0        0        0     1490 2024-02-28 02:21:27.203942 elegant_django-0.2.7/elegant/static/elegant/js/jquery.dropdown.min.js
--rw-r--r--   0        0        0     1066 2024-02-28 02:21:27.203942 elegant_django-0.2.7/elegant/static/elegant/js/sortable.changelist.js
--rw-r--r--   0        0        0     1074 2024-02-28 02:21:27.203942 elegant_django-0.2.7/elegant/static/elegant/js/sortable.stacked.inline.js
--rw-r--r--   0        0        0     1039 2024-02-28 02:21:27.203942 elegant_django-0.2.7/elegant/static/elegant/js/sortable.tabular.inline.js
--rw-r--r--   0        0        0     6895 2024-02-28 02:21:27.203942 elegant_django-0.2.7/elegant/static/elegant/js/sortables.js
--rw-r--r--   0        0        0     3318 2024-02-28 02:21:27.203942 elegant_django-0.2.7/elegant/static/elegant/js/utils.js
--rw-r--r--   0        0        0      289 2024-02-28 02:21:27.203942 elegant_django-0.2.7/elegant/templates/403.html
--rw-r--r--   0        0        0      290 2024-02-28 02:21:27.203942 elegant_django-0.2.7/elegant/templates/404.html
--rw-r--r--   0        0        0      367 2024-02-28 02:21:27.203942 elegant_django-0.2.7/elegant/templates/500.html
--rw-r--r--   0        0        0     1168 2024-02-28 02:21:27.203942 elegant_django-0.2.7/elegant/templates/actions/dropdown.html
--rw-r--r--   0        0        0     1271 2024-02-28 02:21:27.207942 elegant_django-0.2.7/elegant/templates/admin/actions.html
--rw-r--r--   0        0        0      549 2024-02-28 02:21:27.207942 elegant_django-0.2.7/elegant/templates/admin/app_index.html
--rw-r--r--   0        0        0      443 2024-02-28 02:21:27.207942 elegant_django-0.2.7/elegant/templates/admin/auth/user/add_form.html
--rw-r--r--   0        0        0     3407 2024-02-28 02:21:27.207942 elegant_django-0.2.7/elegant/templates/admin/auth/user/change_password.html
--rw-r--r--   0        0        0     8241 2024-02-28 02:21:27.207942 elegant_django-0.2.7/elegant/templates/admin/base.html
--rw-r--r--   0        0        0     3699 2024-02-28 02:21:27.207942 elegant_django-0.2.7/elegant/templates/admin/base_site.html
--rw-r--r--   0        0        0     7776 2024-02-28 02:21:27.207942 elegant_django-0.2.7/elegant/templates/admin/change_form.html
--rw-r--r--   0        0        0     5271 2024-02-28 02:21:27.207942 elegant_django-0.2.7/elegant/templates/admin/change_list.html
--rw-r--r--   0        0        0     2478 2024-02-28 02:21:27.207942 elegant_django-0.2.7/elegant/templates/admin/change_list_results.html
--rw-r--r--   0        0        0     9038 2024-02-28 02:21:27.211942 elegant_django-0.2.7/elegant/templates/admin/cms/page/change_form.html
--rw-r--r--   0        0        0     6470 2024-02-28 02:21:27.211942 elegant_django-0.2.7/elegant/templates/admin/cms/page/change_list.html
--rw-r--r--   0        0        0       45 2024-02-28 02:21:27.211942 elegant_django-0.2.7/elegant/templates/admin/cms/page/includes/fieldset.html
--rw-r--r--   0        0        0     5063 2024-02-28 02:21:27.211942 elegant_django-0.2.7/elegant/templates/admin/cms/page/plugin_change_form.html
--rw-r--r--   0        0        0      373 2024-02-28 02:21:27.211942 elegant_django-0.2.7/elegant/templates/admin/cms/page/widgets/plugin_item.html
--rw-r--r--   0        0        0      536 2024-02-28 02:21:27.211942 elegant_django-0.2.7/elegant/templates/admin/date_hierarchy.html
--rw-r--r--   0        0        0      208 2024-02-28 02:21:27.211942 elegant_django-0.2.7/elegant/templates/admin/date_range_filter.html
--rw-r--r--   0        0        0     2899 2024-02-28 02:21:27.211942 elegant_django-0.2.7/elegant/templates/admin/delete_confirmation.html
--rw-r--r--   0        0        0     2629 2024-02-28 02:21:27.211942 elegant_django-0.2.7/elegant/templates/admin/delete_selected_confirmation.html
--rw-r--r--   0        0        0     5193 2024-02-28 02:21:27.211942 elegant_django-0.2.7/elegant/templates/admin/edit_inline/stacked.html
--rw-r--r--   0        0        0     7544 2024-02-28 02:21:27.211942 elegant_django-0.2.7/elegant/templates/admin/edit_inline/tabular.html
--rw-r--r--   0        0        0      667 2024-02-28 02:21:27.211942 elegant_django-0.2.7/elegant/templates/admin/filter.html
--rw-r--r--   0        0        0      528 2024-02-28 02:21:27.219942 elegant_django-0.2.7/elegant/templates/admin/import_export/export.html
--rw-r--r--   0        0        0     3431 2024-02-28 02:21:27.219942 elegant_django-0.2.7/elegant/templates/admin/import_export/import.html
--rw-r--r--   0        0        0     3211 2024-02-28 02:21:27.219942 elegant_django-0.2.7/elegant/templates/admin/includes/fieldset.html
--rw-r--r--   0        0        0     3555 2024-02-28 02:21:27.219942 elegant_django-0.2.7/elegant/templates/admin/index.html
--rw-r--r--   0        0        0     3547 2024-02-28 02:21:27.219942 elegant_django-0.2.7/elegant/templates/admin/login.html
--rw-r--r--   0        0        0      790 2024-02-28 02:21:27.219942 elegant_django-0.2.7/elegant/templates/admin/mptt_change_list_results.html
--rw-r--r--   0        0        0      728 2024-02-28 02:21:27.219942 elegant_django-0.2.7/elegant/templates/admin/object_actions/change_form.html
--rw-r--r--   0        0        0      672 2024-02-28 02:21:27.219942 elegant_django-0.2.7/elegant/templates/admin/object_actions/change_list.html
--rw-r--r--   0        0        0     2100 2024-02-28 02:21:27.219942 elegant_django-0.2.7/elegant/templates/admin/object_history.html
--rw-r--r--   0        0        0     1791 2024-02-28 02:21:27.219942 elegant_django-0.2.7/elegant/templates/admin/page_submit_line.html
--rw-r--r--   0        0        0      816 2024-02-28 02:21:27.219942 elegant_django-0.2.7/elegant/templates/admin/pagination.html
--rw-r--r--   0        0        0     1044 2024-02-28 02:21:27.219942 elegant_django-0.2.7/elegant/templates/admin/row_actions/dropdown.html
--rw-r--r--   0        0        0     2164 2024-02-28 02:21:27.219942 elegant_django-0.2.7/elegant/templates/admin/search_form.html
--rw-r--r--   0        0        0     1015 2024-02-28 02:21:27.219942 elegant_django-0.2.7/elegant/templates/admin/submit_line.html
--rw-r--r--   0        0        0      149 2024-02-28 02:21:27.219942 elegant_django-0.2.7/elegant/templates/admin/widgets/date.html
--rw-r--r--   0        0        0      158 2024-02-28 02:21:27.219942 elegant_django-0.2.7/elegant/templates/admin/widgets/time.html
--rw-r--r--   0        0        0     2393 2024-02-28 02:21:27.219942 elegant_django-0.2.7/elegant/templates/confirm/action_confirmation.html
--rw-r--r--   0        0        0     2830 2024-02-28 02:21:27.219942 elegant_django-0.2.7/elegant/templates/confirm/change_confirmation.html
--rw-r--r--   0        0        0      532 2024-02-28 02:21:27.219942 elegant_django-0.2.7/elegant/templates/confirm/change_data.html
--rw-r--r--   0        0        0      328 2024-02-28 02:21:27.219942 elegant_django-0.2.7/elegant/templates/confirm/submit_line.html
--rw-r--r--   0        0        0     1168 2024-02-28 02:21:27.219942 elegant_django-0.2.7/elegant/templates/elegant/actions/dropdown.html
--rw-r--r--   0        0        0     2393 2024-02-28 02:21:27.219942 elegant_django-0.2.7/elegant/templates/elegant/confirm/action_confirmation.html
--rw-r--r--   0        0        0     2826 2024-02-28 02:21:27.219942 elegant_django-0.2.7/elegant/templates/elegant/confirm/change_confirmation.html
--rw-r--r--   0        0        0      532 2024-02-28 02:21:27.219942 elegant_django-0.2.7/elegant/templates/elegant/confirm/change_data.html
--rw-r--r--   0        0        0      328 2024-02-28 02:21:27.219942 elegant_django-0.2.7/elegant/templates/elegant/confirm/submit_line.html
--rw-r--r--   0        0        0      208 2024-02-28 02:21:27.219942 elegant_django-0.2.7/elegant/templates/elegant/date_range_filter.html
--rw-r--r--   0        0        0     2962 2024-02-28 02:21:27.223942 elegant_django-0.2.7/elegant/templates/elegant/error_base.html
--rw-r--r--   0        0        0      421 2024-02-28 02:21:27.223942 elegant_django-0.2.7/elegant/templates/elegant/form_as_fieldset.html
--rw-r--r--   0        0        0      312 2024-02-28 02:21:27.223942 elegant_django-0.2.7/elegant/templates/elegant/includes/change_form_includes.html
--rw-r--r--   0        0        0     1253 2024-02-28 02:21:27.223942 elegant_django-0.2.7/elegant/templates/elegant/menu.html
--rw-r--r--   0        0        0      728 2024-02-28 02:21:27.223942 elegant_django-0.2.7/elegant/templates/elegant/objects/change_form.html
--rw-r--r--   0        0        0      794 2024-02-28 02:21:27.223942 elegant_django-0.2.7/elegant/templates/elegant/objects/change_list.html
--rw-r--r--   0        0        0      728 2024-02-28 02:21:27.223942 elegant_django-0.2.7/elegant/templates/object_actions/change_form.html
--rw-r--r--   0        0        0      794 2024-02-28 02:21:27.223942 elegant_django-0.2.7/elegant/templates/object_actions/change_list.html
--rw-r--r--   0        0        0     3850 2024-02-28 02:21:27.223942 elegant_django-0.2.7/elegant/templates/otto/analytics.html
--rw-r--r--   0        0        0      475 2024-02-28 02:21:27.223942 elegant_django-0.2.7/elegant/templates/registration/logged_out.html
--rw-r--r--   0        0        0     3254 2024-02-28 02:21:27.223942 elegant_django-0.2.7/elegant/templates/registration/password_change_form.html
--rw-r--r--   0        0        0      397 2024-02-28 02:21:27.223942 elegant_django-0.2.7/elegant/templates/reversion/change_list.html
--rw-r--r--   0        0        0     1545 2024-02-28 02:21:27.223942 elegant_django-0.2.7/elegant/templates/reversion/object_history.html
--rw-r--r--   0        0        0     1247 2024-02-28 02:21:27.223942 elegant_django-0.2.7/elegant/templates/reversion/recover_form.html
--rw-r--r--   0        0        0     1743 2024-02-28 02:21:27.223942 elegant_django-0.2.7/elegant/templates/reversion/recover_list.html
--rw-r--r--   0        0        0     1413 2024-02-28 02:21:27.223942 elegant_django-0.2.7/elegant/templates/reversion/revision_form.html
--rw-r--r--   0        0        0      161 2024-02-28 02:21:27.223942 elegant_django-0.2.7/elegant/templates/shortcuts/base.css
--rw-r--r--   0        0        0      700 2024-02-28 02:21:27.223942 elegant_django-0.2.7/elegant/templates/shortcuts/base.html
--rw-r--r--   0        0        0      433 2024-02-28 02:21:27.223942 elegant_django-0.2.7/elegant/templates/shortcuts/js.html
--rw-r--r--   0        0        0      500 2024-02-28 02:21:27.223942 elegant_django-0.2.7/elegant/templates/shortcuts/shortcut.html
--rw-r--r--   0        0        0     2818 2024-02-28 02:21:27.231942 elegant_django-0.2.7/elegant/templates/shortcuts/style.css
--rw-r--r--   0        0        0     1384 2024-02-28 02:21:27.231942 elegant_django-0.2.7/elegant/templates/suit_object_tools/change_form.html
--rw-r--r--   0        0        0        0 2024-02-28 02:21:27.231942 elegant_django-0.2.7/elegant/templatetags/__init__.py
--rw-r--r--   0        0        0     1507 2024-02-28 02:21:27.231942 elegant_django-0.2.7/elegant/templatetags/elegant_analytics.py
--rw-r--r--   0        0        0      176 2024-02-28 02:21:27.231942 elegant_django-0.2.7/elegant/templatetags/elegant_compat.py
--rw-r--r--   0        0        0      660 2024-02-28 02:21:27.231942 elegant_django-0.2.7/elegant/templatetags/elegant_formatting.py
--rw-r--r--   0        0        0     9159 2024-02-28 02:21:27.231942 elegant_django-0.2.7/elegant/templatetags/elegant_list.py
--rw-r--r--   0        0        0    17220 2024-02-28 02:21:27.231942 elegant_django-0.2.7/elegant/templatetags/elegant_menu.py
--rw-r--r--   0        0        0     7434 2024-02-28 02:21:27.231942 elegant_django-0.2.7/elegant/templatetags/elegant_shortcuts.py
--rw-r--r--   0        0        0     3796 2024-02-28 02:21:27.231942 elegant_django-0.2.7/elegant/templatetags/elegant_tags.py
--rw-r--r--   0        0        0      660 2024-02-28 02:21:27.231942 elegant_django-0.2.7/elegant/templatetags/formatting.py
--rw-r--r--   0        0        0     3285 2024-02-28 02:21:27.231942 elegant_django-0.2.7/elegant/utils.py
--rw-r--r--   0        0        0       60 2024-02-28 02:21:27.231942 elegant_django-0.2.7/elegant/widgets/__init__.py
--rw-r--r--   0        0        0     6021 2024-02-28 02:21:27.231942 elegant_django-0.2.7/elegant/widgets/elegant.py
--rw-r--r--   0        0        0     2943 2024-02-28 02:21:27.231942 elegant_django-0.2.7/elegant/widgets/filter.py
--rw-r--r--   0        0        0     2046 2024-02-28 02:21:27.231942 elegant_django-0.2.7/pyproject.toml
--rw-r--r--   0        0        0     2168 1970-01-01 00:00:00.000000 elegant_django-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0    18512 2024-05-08 09:44:21.330788 elegant_django-0.2.8/LICENSE
+-rw-r--r--   0        0        0     1175 2024-05-08 09:44:21.330788 elegant_django-0.2.8/README.md
+-rw-r--r--   0        0        0      250 2024-05-08 09:44:21.330788 elegant_django-0.2.8/elegant/__init__.py
+-rw-r--r--   0        0        0     6743 2024-05-08 09:44:21.330788 elegant_django-0.2.8/elegant/admin.py
+-rw-r--r--   0        0        0      184 2024-05-08 09:44:21.330788 elegant_django-0.2.8/elegant/apps.py
+-rw-r--r--   0        0        0     2142 2024-05-08 09:44:21.330788 elegant_django-0.2.8/elegant/cache.py
+-rw-r--r--   0        0        0      244 2024-05-08 09:44:21.330788 elegant_django-0.2.8/elegant/compat.py
+-rw-r--r--   0        0        0      777 2024-05-08 09:44:21.330788 elegant_django-0.2.8/elegant/components.py
+-rw-r--r--   0        0        0     2262 2024-05-08 09:44:21.330788 elegant_django-0.2.8/elegant/config.py
+-rw-r--r--   0        0        0      675 2024-05-08 09:44:21.330788 elegant_django-0.2.8/elegant/constants.py
+-rwxr-xr-x   0        0        0      670 2024-05-08 09:44:21.330788 elegant_django-0.2.8/elegant/context_processors.py
+-rw-r--r--   0        0        0        0 2024-05-08 09:44:21.330788 elegant_django-0.2.8/elegant/contrib/audit/__init__.py
+-rw-r--r--   0        0        0     5569 2024-05-08 09:44:21.330788 elegant_django-0.2.8/elegant/contrib/audit/admin.py
+-rw-r--r--   0        0        0     4976 2024-05-08 09:44:21.330788 elegant_django-0.2.8/elegant/contrib/audit/admin_helpers.py
+-rw-r--r--   0        0        0      430 2024-05-08 09:44:21.330788 elegant_django-0.2.8/elegant/contrib/audit/apps.py
+-rw-r--r--   0        0        0      477 2024-05-08 09:44:21.330788 elegant_django-0.2.8/elegant/contrib/audit/backends.py
+-rw-r--r--   0        0        0     3673 2024-05-08 09:44:21.330788 elegant_django-0.2.8/elegant/contrib/audit/crudhistory_admin_mixin.py
+-rw-r--r--   0        0        0        0 2024-05-08 09:44:21.330788 elegant_django-0.2.8/elegant/contrib/audit/middleware/__init__.py
+-rw-r--r--   0        0        0     1807 2024-05-08 09:44:21.330788 elegant_django-0.2.8/elegant/contrib/audit/middleware/audit.py
+-rw-r--r--   0        0        0        0 2024-05-08 09:44:21.330788 elegant_django-0.2.8/elegant/contrib/audit/migrations/__init__.py
+-rw-r--r--   0        0        0     4305 2024-05-08 09:44:21.330788 elegant_django-0.2.8/elegant/contrib/audit/models.py
+-rw-r--r--   0        0        0     6548 2024-05-08 09:44:21.330788 elegant_django-0.2.8/elegant/contrib/audit/settings.py
+-rw-r--r--   0        0        0        0 2024-05-08 09:44:21.330788 elegant_django-0.2.8/elegant/contrib/audit/signals/__init__.py
+-rw-r--r--   0        0        0     2368 2024-05-08 09:44:21.330788 elegant_django-0.2.8/elegant/contrib/audit/signals/auth_signals.py
+-rw-r--r--   0        0        0    15333 2024-05-08 09:44:21.330788 elegant_django-0.2.8/elegant/contrib/audit/signals/model_signals.py
+-rw-r--r--   0        0        0     3369 2024-05-08 09:44:21.330788 elegant_django-0.2.8/elegant/contrib/audit/signals/request_signals.py
+-rw-r--r--   0        0        0      531 2024-05-08 09:44:21.330788 elegant_django-0.2.8/elegant/contrib/audit/templates/admin/audit/change_list.html
+-rw-r--r--   0        0        0     1202 2024-05-08 09:44:21.330788 elegant_django-0.2.8/elegant/contrib/audit/templates/admin/audit/purge_confirmation.html
+-rw-r--r--   0        0        0     2886 2024-05-08 09:44:21.330788 elegant_django-0.2.8/elegant/contrib/audit/utils.py
+-rw-r--r--   0        0        0     4943 2024-05-08 09:44:21.334788 elegant_django-0.2.8/elegant/locale/zh_Hans/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      137 2024-05-08 09:44:21.334788 elegant_django-0.2.8/elegant/mixins/__init__.py
+-rw-r--r--   0        0        0     6728 2024-05-08 09:44:21.334788 elegant_django-0.2.8/elegant/mixins/actions.py
+-rw-r--r--   0        0        0    19214 2024-05-08 09:44:21.334788 elegant_django-0.2.8/elegant/mixins/confirm.py
+-rw-r--r--   0        0        0    12300 2024-05-08 09:44:21.334788 elegant_django-0.2.8/elegant/mixins/objects.py
+-rw-r--r--   0        0        0   107369 2024-05-08 09:44:21.334788 elegant_django-0.2.8/elegant/static/elegant/bootstrap/css/bootstrap.min.css
+-rw-r--r--   0        0        0    27257 2024-05-08 09:44:21.334788 elegant_django-0.2.8/elegant/static/elegant/bootstrap/img/glyphicons-halflings-white-shadow.png
+-rw-r--r--   0        0        0     8777 2024-05-08 09:44:21.334788 elegant_django-0.2.8/elegant/static/elegant/bootstrap/img/glyphicons-halflings-white.png
+-rw-r--r--   0        0        0    12799 2024-05-08 09:44:21.334788 elegant_django-0.2.8/elegant/static/elegant/bootstrap/img/glyphicons-halflings.png
+-rw-r--r--   0        0        0    15753 2024-05-08 09:44:21.334788 elegant_django-0.2.8/elegant/static/elegant/bootstrap/js/bootstrap.min.js
+-rw-r--r--   0        0        0      528 2024-05-08 09:44:21.334788 elegant_django-0.2.8/elegant/static/elegant/css/confirmation.css
+-rw-r--r--   0        0        0      615 2024-05-08 09:44:21.334788 elegant_django-0.2.8/elegant/static/elegant/css/dashboard.css
+-rw-r--r--   0        0        0      408 2024-05-08 09:44:21.334788 elegant_django-0.2.8/elegant/static/elegant/css/date_range_filter.css
+-rw-r--r--   0        0        0    25774 2024-05-08 09:44:21.334788 elegant_django-0.2.8/elegant/static/elegant/css/djangocms.css
+-rw-r--r--   0        0        0    62642 2024-05-08 09:44:21.334788 elegant_django-0.2.8/elegant/static/elegant/css/elegant.css
+-rw-r--r--   0        0        0      150 2024-05-08 09:44:21.334788 elegant_django-0.2.8/elegant/static/elegant/css/extra.css
+-rw-r--r--   0        0        0     3881 2024-05-08 09:44:21.334788 elegant_django-0.2.8/elegant/static/elegant/css/filer.css
+-rw-r--r--   0        0        0       63 2024-05-08 09:44:21.334788 elegant_django-0.2.8/elegant/static/elegant/css/forms.css
+-rw-r--r--   0        0        0     2362 2024-05-08 09:44:21.334788 elegant_django-0.2.8/elegant/static/elegant/css/jquery.dropdown.min.css
+-rw-r--r--   0        0        0        0 2024-05-08 09:44:21.338788 elegant_django-0.2.8/elegant/static/elegant/css/shortcuts.css
+-rw-r--r--   0        0        0     1737 2024-05-08 09:44:21.338788 elegant_django-0.2.8/elegant/static/elegant/img/ajax-loader.gif
+-rw-r--r--   0        0        0      105 2024-05-08 09:44:21.338788 elegant_django-0.2.8/elegant/static/elegant/img/bg_left_white.gif
+-rw-r--r--   0        0        0    41210 2024-05-08 09:44:21.338788 elegant_django-0.2.8/elegant/static/elegant/img/bg_pattern.jpg
+-rw-r--r--   0        0        0      432 2024-05-08 09:44:21.338788 elegant_django-0.2.8/elegant/static/elegant/img/cc_active_nav.png
+-rw-r--r--   0        0        0      132 2024-05-08 09:44:21.338788 elegant_django-0.2.8/elegant/static/elegant/img/drag-handle.png
+-rw-r--r--   0        0        0    40145 2024-05-08 09:44:21.338788 elegant_django-0.2.8/elegant/static/elegant/img/glyphicons-halflings-white-nav.png
+-rw-r--r--   0        0        0    27257 2024-05-08 09:44:21.338788 elegant_django-0.2.8/elegant/static/elegant/img/glyphicons-halflings-white-shadow.png
+-rw-r--r--   0        0        0      394 2024-05-08 09:44:21.338788 elegant_django-0.2.8/elegant/static/elegant/js/djangocms.js
+-rw-r--r--   0        0        0     2305 2024-05-08 09:44:21.338788 elegant_django-0.2.8/elegant/static/elegant/js/elegant-form-confirm.js
+-rw-r--r--   0        0        0     6912 2024-05-08 09:44:21.338788 elegant_django-0.2.8/elegant/static/elegant/js/elegant.js
+-rw-r--r--   0        0        0    85578 2024-05-08 09:44:21.338788 elegant_django-0.2.8/elegant/static/elegant/js/jquery-2.2.4.min.js
+-rw-r--r--   0        0        0    37490 2024-05-08 09:44:21.338788 elegant_django-0.2.8/elegant/static/elegant/js/jquery-ui-1.10.3.sortable.min.js
+-rw-r--r--   0        0        0     3270 2024-05-08 09:44:21.338788 elegant_django-0.2.8/elegant/static/elegant/js/jquery.autosize-min.js
+-rw-r--r--   0        0        0     5165 2024-05-08 09:44:21.338788 elegant_django-0.2.8/elegant/static/elegant/js/jquery.dropdown.js
+-rw-r--r--   0        0        0     1490 2024-05-08 09:44:21.338788 elegant_django-0.2.8/elegant/static/elegant/js/jquery.dropdown.min.js
+-rw-r--r--   0        0        0     1066 2024-05-08 09:44:21.338788 elegant_django-0.2.8/elegant/static/elegant/js/sortable.changelist.js
+-rw-r--r--   0        0        0     1074 2024-05-08 09:44:21.338788 elegant_django-0.2.8/elegant/static/elegant/js/sortable.stacked.inline.js
+-rw-r--r--   0        0        0     1039 2024-05-08 09:44:21.338788 elegant_django-0.2.8/elegant/static/elegant/js/sortable.tabular.inline.js
+-rw-r--r--   0        0        0     6895 2024-05-08 09:44:21.338788 elegant_django-0.2.8/elegant/static/elegant/js/sortables.js
+-rw-r--r--   0        0        0     3318 2024-05-08 09:44:21.338788 elegant_django-0.2.8/elegant/static/elegant/js/utils.js
+-rw-r--r--   0        0        0      289 2024-05-08 09:44:21.338788 elegant_django-0.2.8/elegant/templates/403.html
+-rw-r--r--   0        0        0      290 2024-05-08 09:44:21.338788 elegant_django-0.2.8/elegant/templates/404.html
+-rw-r--r--   0        0        0      367 2024-05-08 09:44:21.338788 elegant_django-0.2.8/elegant/templates/500.html
+-rw-r--r--   0        0        0     1168 2024-05-08 09:44:21.338788 elegant_django-0.2.8/elegant/templates/actions/dropdown.html
+-rw-r--r--   0        0        0     1271 2024-05-08 09:44:21.338788 elegant_django-0.2.8/elegant/templates/admin/actions.html
+-rw-r--r--   0        0        0      549 2024-05-08 09:44:21.342788 elegant_django-0.2.8/elegant/templates/admin/app_index.html
+-rw-r--r--   0        0        0      443 2024-05-08 09:44:21.342788 elegant_django-0.2.8/elegant/templates/admin/auth/user/add_form.html
+-rw-r--r--   0        0        0     3407 2024-05-08 09:44:21.342788 elegant_django-0.2.8/elegant/templates/admin/auth/user/change_password.html
+-rw-r--r--   0        0        0     8241 2024-05-08 09:44:21.342788 elegant_django-0.2.8/elegant/templates/admin/base.html
+-rw-r--r--   0        0        0     3699 2024-05-08 09:44:21.342788 elegant_django-0.2.8/elegant/templates/admin/base_site.html
+-rw-r--r--   0        0        0     7776 2024-05-08 09:44:21.342788 elegant_django-0.2.8/elegant/templates/admin/change_form.html
+-rw-r--r--   0        0        0     5271 2024-05-08 09:44:21.342788 elegant_django-0.2.8/elegant/templates/admin/change_list.html
+-rw-r--r--   0        0        0     2478 2024-05-08 09:44:21.342788 elegant_django-0.2.8/elegant/templates/admin/change_list_results.html
+-rw-r--r--   0        0        0     9038 2024-05-08 09:44:21.342788 elegant_django-0.2.8/elegant/templates/admin/cms/page/change_form.html
+-rw-r--r--   0        0        0     6470 2024-05-08 09:44:21.342788 elegant_django-0.2.8/elegant/templates/admin/cms/page/change_list.html
+-rw-r--r--   0        0        0       45 2024-05-08 09:44:21.342788 elegant_django-0.2.8/elegant/templates/admin/cms/page/includes/fieldset.html
+-rw-r--r--   0        0        0     5063 2024-05-08 09:44:21.342788 elegant_django-0.2.8/elegant/templates/admin/cms/page/plugin_change_form.html
+-rw-r--r--   0        0        0      373 2024-05-08 09:44:21.342788 elegant_django-0.2.8/elegant/templates/admin/cms/page/widgets/plugin_item.html
+-rw-r--r--   0        0        0      536 2024-05-08 09:44:21.342788 elegant_django-0.2.8/elegant/templates/admin/date_hierarchy.html
+-rw-r--r--   0        0        0      208 2024-05-08 09:44:21.342788 elegant_django-0.2.8/elegant/templates/admin/date_range_filter.html
+-rw-r--r--   0        0        0     2899 2024-05-08 09:44:21.342788 elegant_django-0.2.8/elegant/templates/admin/delete_confirmation.html
+-rw-r--r--   0        0        0     2629 2024-05-08 09:44:21.342788 elegant_django-0.2.8/elegant/templates/admin/delete_selected_confirmation.html
+-rw-r--r--   0        0        0     5193 2024-05-08 09:44:21.342788 elegant_django-0.2.8/elegant/templates/admin/edit_inline/stacked.html
+-rw-r--r--   0        0        0     7544 2024-05-08 09:44:21.342788 elegant_django-0.2.8/elegant/templates/admin/edit_inline/tabular.html
+-rw-r--r--   0        0        0      667 2024-05-08 09:44:21.342788 elegant_django-0.2.8/elegant/templates/admin/filter.html
+-rw-r--r--   0        0        0      528 2024-05-08 09:44:21.342788 elegant_django-0.2.8/elegant/templates/admin/import_export/export.html
+-rw-r--r--   0        0        0     3431 2024-05-08 09:44:21.342788 elegant_django-0.2.8/elegant/templates/admin/import_export/import.html
+-rw-r--r--   0        0        0     3211 2024-05-08 09:44:21.342788 elegant_django-0.2.8/elegant/templates/admin/includes/fieldset.html
+-rw-r--r--   0        0        0     3555 2024-05-08 09:44:21.342788 elegant_django-0.2.8/elegant/templates/admin/index.html
+-rw-r--r--   0        0        0     3547 2024-05-08 09:44:21.342788 elegant_django-0.2.8/elegant/templates/admin/login.html
+-rw-r--r--   0        0        0      790 2024-05-08 09:44:21.342788 elegant_django-0.2.8/elegant/templates/admin/mptt_change_list_results.html
+-rw-r--r--   0        0        0      728 2024-05-08 09:44:21.342788 elegant_django-0.2.8/elegant/templates/admin/object_actions/change_form.html
+-rw-r--r--   0        0        0      672 2024-05-08 09:44:21.342788 elegant_django-0.2.8/elegant/templates/admin/object_actions/change_list.html
+-rw-r--r--   0        0        0     2100 2024-05-08 09:44:21.342788 elegant_django-0.2.8/elegant/templates/admin/object_history.html
+-rw-r--r--   0        0        0     1791 2024-05-08 09:44:21.342788 elegant_django-0.2.8/elegant/templates/admin/page_submit_line.html
+-rw-r--r--   0        0        0      816 2024-05-08 09:44:21.342788 elegant_django-0.2.8/elegant/templates/admin/pagination.html
+-rw-r--r--   0        0        0     1044 2024-05-08 09:44:21.342788 elegant_django-0.2.8/elegant/templates/admin/row_actions/dropdown.html
+-rw-r--r--   0        0        0     2164 2024-05-08 09:44:21.342788 elegant_django-0.2.8/elegant/templates/admin/search_form.html
+-rw-r--r--   0        0        0     1015 2024-05-08 09:44:21.342788 elegant_django-0.2.8/elegant/templates/admin/submit_line.html
+-rw-r--r--   0        0        0      149 2024-05-08 09:44:21.342788 elegant_django-0.2.8/elegant/templates/admin/widgets/date.html
+-rw-r--r--   0        0        0      158 2024-05-08 09:44:21.342788 elegant_django-0.2.8/elegant/templates/admin/widgets/time.html
+-rw-r--r--   0        0        0     2393 2024-05-08 09:44:21.342788 elegant_django-0.2.8/elegant/templates/confirm/action_confirmation.html
+-rw-r--r--   0        0        0     2830 2024-05-08 09:44:21.342788 elegant_django-0.2.8/elegant/templates/confirm/change_confirmation.html
+-rw-r--r--   0        0        0      532 2024-05-08 09:44:21.342788 elegant_django-0.2.8/elegant/templates/confirm/change_data.html
+-rw-r--r--   0        0        0      328 2024-05-08 09:44:21.342788 elegant_django-0.2.8/elegant/templates/confirm/submit_line.html
+-rw-r--r--   0        0        0     1168 2024-05-08 09:44:21.346788 elegant_django-0.2.8/elegant/templates/elegant/actions/dropdown.html
+-rw-r--r--   0        0        0     2393 2024-05-08 09:44:21.346788 elegant_django-0.2.8/elegant/templates/elegant/confirm/action_confirmation.html
+-rw-r--r--   0        0        0     2826 2024-05-08 09:44:21.346788 elegant_django-0.2.8/elegant/templates/elegant/confirm/change_confirmation.html
+-rw-r--r--   0        0        0      532 2024-05-08 09:44:21.346788 elegant_django-0.2.8/elegant/templates/elegant/confirm/change_data.html
+-rw-r--r--   0        0        0      328 2024-05-08 09:44:21.346788 elegant_django-0.2.8/elegant/templates/elegant/confirm/submit_line.html
+-rw-r--r--   0        0        0      208 2024-05-08 09:44:21.346788 elegant_django-0.2.8/elegant/templates/elegant/date_range_filter.html
+-rw-r--r--   0        0        0     2962 2024-05-08 09:44:21.346788 elegant_django-0.2.8/elegant/templates/elegant/error_base.html
+-rw-r--r--   0        0        0      421 2024-05-08 09:44:21.346788 elegant_django-0.2.8/elegant/templates/elegant/form_as_fieldset.html
+-rw-r--r--   0        0        0      312 2024-05-08 09:44:21.346788 elegant_django-0.2.8/elegant/templates/elegant/includes/change_form_includes.html
+-rw-r--r--   0        0        0     1253 2024-05-08 09:44:21.346788 elegant_django-0.2.8/elegant/templates/elegant/menu.html
+-rw-r--r--   0        0        0      728 2024-05-08 09:44:21.346788 elegant_django-0.2.8/elegant/templates/elegant/objects/change_form.html
+-rw-r--r--   0        0        0      794 2024-05-08 09:44:21.346788 elegant_django-0.2.8/elegant/templates/elegant/objects/change_list.html
+-rw-r--r--   0        0        0      728 2024-05-08 09:44:21.346788 elegant_django-0.2.8/elegant/templates/object_actions/change_form.html
+-rw-r--r--   0        0        0      794 2024-05-08 09:44:21.346788 elegant_django-0.2.8/elegant/templates/object_actions/change_list.html
+-rw-r--r--   0        0        0     3850 2024-05-08 09:44:21.346788 elegant_django-0.2.8/elegant/templates/otto/analytics.html
+-rw-r--r--   0        0        0      475 2024-05-08 09:44:21.346788 elegant_django-0.2.8/elegant/templates/registration/logged_out.html
+-rw-r--r--   0        0        0     3254 2024-05-08 09:44:21.346788 elegant_django-0.2.8/elegant/templates/registration/password_change_form.html
+-rw-r--r--   0        0        0      397 2024-05-08 09:44:21.346788 elegant_django-0.2.8/elegant/templates/reversion/change_list.html
+-rw-r--r--   0        0        0     1545 2024-05-08 09:44:21.346788 elegant_django-0.2.8/elegant/templates/reversion/object_history.html
+-rw-r--r--   0        0        0     1247 2024-05-08 09:44:21.346788 elegant_django-0.2.8/elegant/templates/reversion/recover_form.html
+-rw-r--r--   0        0        0     1743 2024-05-08 09:44:21.346788 elegant_django-0.2.8/elegant/templates/reversion/recover_list.html
+-rw-r--r--   0        0        0     1413 2024-05-08 09:44:21.346788 elegant_django-0.2.8/elegant/templates/reversion/revision_form.html
+-rw-r--r--   0        0        0      161 2024-05-08 09:44:21.346788 elegant_django-0.2.8/elegant/templates/shortcuts/base.css
+-rw-r--r--   0        0        0      700 2024-05-08 09:44:21.346788 elegant_django-0.2.8/elegant/templates/shortcuts/base.html
+-rw-r--r--   0        0        0      433 2024-05-08 09:44:21.346788 elegant_django-0.2.8/elegant/templates/shortcuts/js.html
+-rw-r--r--   0        0        0      500 2024-05-08 09:44:21.346788 elegant_django-0.2.8/elegant/templates/shortcuts/shortcut.html
+-rw-r--r--   0        0        0     2818 2024-05-08 09:44:21.346788 elegant_django-0.2.8/elegant/templates/shortcuts/style.css
+-rw-r--r--   0        0        0     1384 2024-05-08 09:44:21.346788 elegant_django-0.2.8/elegant/templates/suit_object_tools/change_form.html
+-rw-r--r--   0        0        0        0 2024-05-08 09:44:21.346788 elegant_django-0.2.8/elegant/templatetags/__init__.py
+-rw-r--r--   0        0        0     1507 2024-05-08 09:44:21.346788 elegant_django-0.2.8/elegant/templatetags/elegant_analytics.py
+-rw-r--r--   0        0        0      176 2024-05-08 09:44:21.346788 elegant_django-0.2.8/elegant/templatetags/elegant_compat.py
+-rw-r--r--   0        0        0      660 2024-05-08 09:44:21.346788 elegant_django-0.2.8/elegant/templatetags/elegant_formatting.py
+-rw-r--r--   0        0        0     9159 2024-05-08 09:44:21.346788 elegant_django-0.2.8/elegant/templatetags/elegant_list.py
+-rw-r--r--   0        0        0    17220 2024-05-08 09:44:21.346788 elegant_django-0.2.8/elegant/templatetags/elegant_menu.py
+-rw-r--r--   0        0        0     7434 2024-05-08 09:44:21.346788 elegant_django-0.2.8/elegant/templatetags/elegant_shortcuts.py
+-rw-r--r--   0        0        0     3796 2024-05-08 09:44:21.346788 elegant_django-0.2.8/elegant/templatetags/elegant_tags.py
+-rw-r--r--   0        0        0      660 2024-05-08 09:44:21.346788 elegant_django-0.2.8/elegant/templatetags/formatting.py
+-rw-r--r--   0        0        0     3285 2024-05-08 09:44:21.346788 elegant_django-0.2.8/elegant/utils.py
+-rw-r--r--   0        0        0       60 2024-05-08 09:44:21.346788 elegant_django-0.2.8/elegant/widgets/__init__.py
+-rw-r--r--   0        0        0     6021 2024-05-08 09:44:21.346788 elegant_django-0.2.8/elegant/widgets/elegant.py
+-rw-r--r--   0        0        0     2943 2024-05-08 09:44:21.346788 elegant_django-0.2.8/elegant/widgets/filter.py
+-rw-r--r--   0        0        0     2046 2024-05-08 09:44:21.346788 elegant_django-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0     2169 1970-01-01 00:00:00.000000 elegant_django-0.2.8/PKG-INFO
```

### Comparing `elegant_django-0.2.7/LICENSE` & `elegant_django-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `elegant_django-0.2.7/README.md` & `elegant_django-0.2.8/README.md`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -24,8 +24,8 @@
 
 ## 安装方法
 
 > 新手建议使用 `pip install elegant-django` 安装
 
 ## Stargazers over time
 
-[![Stargazers over time](https://starchart.cc/bopo/elegant-django.svg)](https://starchart.cc/bopo/elegant-django)
+[![Stargazers over time](https://starchart.cc/bopo/elegant-django.svg)](https://starchart.cc/bopo/elegant-django)
```

### Comparing `elegant_django-0.2.7/elegant/admin.py` & `elegant_django-0.2.8/elegant/admin.py`

 * *Files identical despite different names*

### Comparing `elegant_django-0.2.7/elegant/cache.py` & `elegant_django-0.2.8/elegant/cache.py`

 * *Files identical despite different names*

### Comparing `elegant_django-0.2.7/elegant/components.py` & `elegant_django-0.2.8/elegant/components.py`

 * *Files identical despite different names*

### Comparing `elegant_django-0.2.7/elegant/config.py` & `elegant_django-0.2.8/elegant/config.py`

 * *Files identical despite different names*

### Comparing `elegant_django-0.2.7/elegant/constants.py` & `elegant_django-0.2.8/elegant/constants.py`

 * *Files identical despite different names*

### Comparing `elegant_django-0.2.7/elegant/context_processors.py` & `elegant_django-0.2.8/elegant/context_processors.py`

 * *Files identical despite different names*

### Comparing `elegant_django-0.2.7/elegant/mixins/actions.py` & `elegant_django-0.2.8/elegant/mixins/actions.py`

 * *Files identical despite different names*

### Comparing `elegant_django-0.2.7/elegant/mixins/confirm.py` & `elegant_django-0.2.8/elegant/mixins/confirm.py`

 * *Files identical despite different names*

### Comparing `elegant_django-0.2.7/elegant/mixins/objects.py` & `elegant_django-0.2.8/elegant/mixins/objects.py`

 * *Files identical despite different names*

### Comparing `elegant_django-0.2.7/elegant/static/elegant/bootstrap/css/bootstrap.min.css` & `elegant_django-0.2.8/elegant/static/elegant/bootstrap/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `elegant_django-0.2.7/elegant/static/elegant/bootstrap/img/glyphicons-halflings-white-shadow.png` & `elegant_django-0.2.8/elegant/static/elegant/bootstrap/img/glyphicons-halflings-white-shadow.png`

 * *Files identical despite different names*

### Comparing `elegant_django-0.2.7/elegant/static/elegant/bootstrap/img/glyphicons-halflings-white.png` & `elegant_django-0.2.8/elegant/static/elegant/bootstrap/img/glyphicons-halflings-white.png`

 * *Files identical despite different names*

### Comparing `elegant_django-0.2.7/elegant/static/elegant/bootstrap/img/glyphicons-halflings.png` & `elegant_django-0.2.8/elegant/static/elegant/bootstrap/img/glyphicons-halflings.png`

 * *Files identical despite different names*

### Comparing `elegant_django-0.2.7/elegant/static/elegant/bootstrap/js/bootstrap.min.js` & `elegant_django-0.2.8/elegant/static/elegant/bootstrap/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `elegant_django-0.2.7/elegant/static/elegant/css/confirmation.css` & `elegant_django-0.2.8/elegant/static/elegant/css/confirmation.css`

 * *Files identical despite different names*

### Comparing `elegant_django-0.2.7/elegant/static/elegant/css/dashboard.css` & `elegant_django-0.2.8/elegant/static/elegant/css/dashboard.css`

 * *Files identical despite different names*

### Comparing `elegant_django-0.2.7/elegant/static/elegant/css/djangocms.css` & `elegant_django-0.2.8/elegant/static/elegant/css/djangocms.css`

 * *Files identical despite different names*

### Comparing `elegant_django-0.2.7/elegant/static/elegant/css/elegant.css` & `elegant_django-0.2.8/elegant/static/elegant/css/elegant.css`

 * *Files identical despite different names*

### Comparing `elegant_django-0.2.7/elegant/static/elegant/css/filer.css` & `elegant_django-0.2.8/elegant/static/elegant/css/filer.css`

 * *Files identical despite different names*

### Comparing `elegant_django-0.2.7/elegant/static/elegant/css/jquery.dropdown.min.css` & `elegant_django-0.2.8/elegant/static/elegant/css/jquery.dropdown.min.css`

 * *Files identical despite different names*

### Comparing `elegant_django-0.2.7/elegant/static/elegant/img/ajax-loader.gif` & `elegant_django-0.2.8/elegant/static/elegant/img/ajax-loader.gif`

 * *Files identical despite different names*

### Comparing `elegant_django-0.2.7/elegant/static/elegant/img/bg_pattern.jpg` & `elegant_django-0.2.8/elegant/static/elegant/img/bg_pattern.jpg`

 * *Files identical despite different names*

### Comparing `elegant_django-0.2.7/elegant/static/elegant/img/glyphicons-halflings-white-nav.png` & `elegant_django-0.2.8/elegant/static/elegant/img/glyphicons-halflings-white-nav.png`

 * *Files identical despite different names*

### Comparing `elegant_django-0.2.7/elegant/static/elegant/img/glyphicons-halflings-white-shadow.png` & `elegant_django-0.2.8/elegant/static/elegant/img/glyphicons-halflings-white-shadow.png`

 * *Files identical despite different names*

### Comparing `elegant_django-0.2.7/elegant/static/elegant/js/elegant-form-confirm.js` & `elegant_django-0.2.8/elegant/static/elegant/js/elegant-form-confirm.js`

 * *Files identical despite different names*

### Comparing `elegant_django-0.2.7/elegant/static/elegant/js/elegant.js` & `elegant_django-0.2.8/elegant/static/elegant/js/elegant.js`

 * *Files identical despite different names*

### Comparing `elegant_django-0.2.7/elegant/static/elegant/js/jquery-2.2.4.min.js` & `elegant_django-0.2.8/elegant/static/elegant/js/jquery-2.2.4.min.js`

 * *Files identical despite different names*

### Comparing `elegant_django-0.2.7/elegant/static/elegant/js/jquery-ui-1.10.3.sortable.min.js` & `elegant_django-0.2.8/elegant/static/elegant/js/jquery-ui-1.10.3.sortable.min.js`

 * *Files identical despite different names*

### Comparing `elegant_django-0.2.7/elegant/static/elegant/js/jquery.autosize-min.js` & `elegant_django-0.2.8/elegant/static/elegant/js/jquery.autosize-min.js`

 * *Files identical despite different names*

### Comparing `elegant_django-0.2.7/elegant/static/elegant/js/jquery.dropdown.js` & `elegant_django-0.2.8/elegant/static/elegant/js/jquery.dropdown.js`

 * *Files identical despite different names*

### Comparing `elegant_django-0.2.7/elegant/static/elegant/js/jquery.dropdown.min.js` & `elegant_django-0.2.8/elegant/static/elegant/js/jquery.dropdown.min.js`

 * *Files identical despite different names*

### Comparing `elegant_django-0.2.7/elegant/static/elegant/js/sortable.changelist.js` & `elegant_django-0.2.8/elegant/static/elegant/js/sortable.changelist.js`

 * *Files identical despite different names*

### Comparing `elegant_django-0.2.7/elegant/static/elegant/js/sortable.stacked.inline.js` & `elegant_django-0.2.8/elegant/static/elegant/js/sortable.stacked.inline.js`

 * *Files identical despite different names*

### Comparing `elegant_django-0.2.7/elegant/static/elegant/js/sortable.tabular.inline.js` & `elegant_django-0.2.8/elegant/static/elegant/js/sortable.tabular.inline.js`

 * *Files identical despite different names*

### Comparing `elegant_django-0.2.7/elegant/static/elegant/js/sortables.js` & `elegant_django-0.2.8/elegant/static/elegant/js/sortables.js`

 * *Files identical despite different names*

### Comparing `elegant_django-0.2.7/elegant/static/elegant/js/utils.js` & `elegant_django-0.2.8/elegant/static/elegant/js/utils.js`

 * *Files identical despite different names*

### Comparing `elegant_django-0.2.7/elegant/templates/actions/dropdown.html` & `elegant_django-0.2.8/elegant/templates/actions/dropdown.html`

 * *Files identical despite different names*

### Comparing `elegant_django-0.2.7/elegant/templates/admin/actions.html` & `elegant_django-0.2.8/elegant/templates/admin/actions.html`

 * *Files identical despite different names*

### Comparing `elegant_django-0.2.7/elegant/templates/admin/app_index.html` & `elegant_django-0.2.8/elegant/templates/admin/app_index.html`

 * *Files identical despite different names*

### Comparing `elegant_django-0.2.7/elegant/templates/admin/auth/user/change_password.html` & `elegant_django-0.2.8/elegant/templates/admin/auth/user/change_password.html`

 * *Files identical despite different names*

### Comparing `elegant_django-0.2.7/elegant/templates/admin/base.html` & `elegant_django-0.2.8/elegant/templates/admin/base.html`

 * *Files identical despite different names*

### Comparing `elegant_django-0.2.7/elegant/templates/admin/base_site.html` & `elegant_django-0.2.8/elegant/templates/admin/base_site.html`

 * *Files identical despite different names*

### Comparing `elegant_django-0.2.7/elegant/templates/admin/change_form.html` & `elegant_django-0.2.8/elegant/templates/admin/change_form.html`

 * *Files identical despite different names*

### Comparing `elegant_django-0.2.7/elegant/templates/admin/change_list.html` & `elegant_django-0.2.8/elegant/templates/admin/change_list.html`

 * *Files identical despite different names*

### Comparing `elegant_django-0.2.7/elegant/templates/admin/change_list_results.html` & `elegant_django-0.2.8/elegant/templates/admin/change_list_results.html`

 * *Files identical despite different names*

### Comparing `elegant_django-0.2.7/elegant/templates/admin/cms/page/change_form.html` & `elegant_django-0.2.8/elegant/templates/admin/cms/page/change_form.html`

 * *Files identical despite different names*

### Comparing `elegant_django-0.2.7/elegant/templates/admin/cms/page/change_list.html` & `elegant_django-0.2.8/elegant/templates/admin/cms/page/change_list.html`

 * *Files identical despite different names*

### Comparing `elegant_django-0.2.7/elegant/templates/admin/cms/page/plugin_change_form.html` & `elegant_django-0.2.8/elegant/templates/admin/cms/page/plugin_change_form.html`

 * *Files identical despite different names*

### Comparing `elegant_django-0.2.7/elegant/templates/admin/date_hierarchy.html` & `elegant_django-0.2.8/elegant/templates/admin/date_hierarchy.html`

 * *Files identical despite different names*

### Comparing `elegant_django-0.2.7/elegant/templates/admin/delete_confirmation.html` & `elegant_django-0.2.8/elegant/templates/admin/delete_confirmation.html`

 * *Files identical despite different names*

### Comparing `elegant_django-0.2.7/elegant/templates/admin/delete_selected_confirmation.html` & `elegant_django-0.2.8/elegant/templates/admin/delete_selected_confirmation.html`

 * *Files identical despite different names*

### Comparing `elegant_django-0.2.7/elegant/templates/admin/edit_inline/stacked.html` & `elegant_django-0.2.8/elegant/templates/admin/edit_inline/stacked.html`

 * *Files identical despite different names*

### Comparing `elegant_django-0.2.7/elegant/templates/admin/edit_inline/tabular.html` & `elegant_django-0.2.8/elegant/templates/admin/edit_inline/tabular.html`

 * *Files identical despite different names*

### Comparing `elegant_django-0.2.7/elegant/templates/admin/filter.html` & `elegant_django-0.2.8/elegant/templates/admin/filter.html`

 * *Files identical despite different names*

### Comparing `elegant_django-0.2.7/elegant/templates/admin/import_export/export.html` & `elegant_django-0.2.8/elegant/templates/admin/import_export/export.html`

 * *Files identical despite different names*

### Comparing `elegant_django-0.2.7/elegant/templates/admin/import_export/import.html` & `elegant_django-0.2.8/elegant/templates/admin/import_export/import.html`

 * *Files identical despite different names*

### Comparing `elegant_django-0.2.7/elegant/templates/admin/includes/fieldset.html` & `elegant_django-0.2.8/elegant/templates/admin/includes/fieldset.html`

 * *Files identical despite different names*

### Comparing `elegant_django-0.2.7/elegant/templates/admin/index.html` & `elegant_django-0.2.8/elegant/templates/admin/index.html`

 * *Files identical despite different names*

### Comparing `elegant_django-0.2.7/elegant/templates/admin/login.html` & `elegant_django-0.2.8/elegant/templates/admin/login.html`

 * *Files identical despite different names*

### Comparing `elegant_django-0.2.7/elegant/templates/admin/mptt_change_list_results.html` & `elegant_django-0.2.8/elegant/templates/admin/mptt_change_list_results.html`

 * *Files identical despite different names*

### Comparing `elegant_django-0.2.7/elegant/templates/admin/object_actions/change_form.html` & `elegant_django-0.2.8/elegant/templates/admin/object_actions/change_form.html`

 * *Files identical despite different names*

### Comparing `elegant_django-0.2.7/elegant/templates/admin/object_actions/change_list.html` & `elegant_django-0.2.8/elegant/templates/admin/object_actions/change_list.html`

 * *Files identical despite different names*

### Comparing `elegant_django-0.2.7/elegant/templates/admin/object_history.html` & `elegant_django-0.2.8/elegant/templates/admin/object_history.html`

 * *Files identical despite different names*

### Comparing `elegant_django-0.2.7/elegant/templates/admin/page_submit_line.html` & `elegant_django-0.2.8/elegant/templates/admin/page_submit_line.html`

 * *Files identical despite different names*

### Comparing `elegant_django-0.2.7/elegant/templates/admin/pagination.html` & `elegant_django-0.2.8/elegant/templates/admin/pagination.html`

 * *Files identical despite different names*

### Comparing `elegant_django-0.2.7/elegant/templates/admin/row_actions/dropdown.html` & `elegant_django-0.2.8/elegant/templates/admin/row_actions/dropdown.html`

 * *Files identical despite different names*

### Comparing `elegant_django-0.2.7/elegant/templates/admin/search_form.html` & `elegant_django-0.2.8/elegant/templates/admin/search_form.html`

 * *Files identical despite different names*

### Comparing `elegant_django-0.2.7/elegant/templates/admin/submit_line.html` & `elegant_django-0.2.8/elegant/templates/admin/submit_line.html`

 * *Files identical despite different names*

### Comparing `elegant_django-0.2.7/elegant/templates/confirm/action_confirmation.html` & `elegant_django-0.2.8/elegant/templates/confirm/action_confirmation.html`

 * *Files identical despite different names*

### Comparing `elegant_django-0.2.7/elegant/templates/confirm/change_confirmation.html` & `elegant_django-0.2.8/elegant/templates/confirm/change_confirmation.html`

 * *Files identical despite different names*

### Comparing `elegant_django-0.2.7/elegant/templates/confirm/change_data.html` & `elegant_django-0.2.8/elegant/templates/confirm/change_data.html`

 * *Files identical despite different names*

### Comparing `elegant_django-0.2.7/elegant/templates/elegant/actions/dropdown.html` & `elegant_django-0.2.8/elegant/templates/elegant/actions/dropdown.html`

 * *Files identical despite different names*

### Comparing `elegant_django-0.2.7/elegant/templates/elegant/confirm/action_confirmation.html` & `elegant_django-0.2.8/elegant/templates/elegant/confirm/action_confirmation.html`

 * *Files identical despite different names*

### Comparing `elegant_django-0.2.7/elegant/templates/elegant/confirm/change_confirmation.html` & `elegant_django-0.2.8/elegant/templates/elegant/confirm/change_confirmation.html`

 * *Files identical despite different names*

### Comparing `elegant_django-0.2.7/elegant/templates/elegant/confirm/change_data.html` & `elegant_django-0.2.8/elegant/templates/elegant/confirm/change_data.html`

 * *Files identical despite different names*

### Comparing `elegant_django-0.2.7/elegant/templates/elegant/error_base.html` & `elegant_django-0.2.8/elegant/templates/elegant/error_base.html`

 * *Files identical despite different names*

### Comparing `elegant_django-0.2.7/elegant/templates/elegant/menu.html` & `elegant_django-0.2.8/elegant/templates/elegant/menu.html`

 * *Files identical despite different names*

### Comparing `elegant_django-0.2.7/elegant/templates/elegant/objects/change_form.html` & `elegant_django-0.2.8/elegant/templates/elegant/objects/change_form.html`

 * *Files identical despite different names*

### Comparing `elegant_django-0.2.7/elegant/templates/elegant/objects/change_list.html` & `elegant_django-0.2.8/elegant/templates/elegant/objects/change_list.html`

 * *Files identical despite different names*

### Comparing `elegant_django-0.2.7/elegant/templates/object_actions/change_form.html` & `elegant_django-0.2.8/elegant/templates/object_actions/change_form.html`

 * *Files identical despite different names*

### Comparing `elegant_django-0.2.7/elegant/templates/object_actions/change_list.html` & `elegant_django-0.2.8/elegant/templates/object_actions/change_list.html`

 * *Files identical despite different names*

### Comparing `elegant_django-0.2.7/elegant/templates/otto/analytics.html` & `elegant_django-0.2.8/elegant/templates/otto/analytics.html`

 * *Files identical despite different names*

### Comparing `elegant_django-0.2.7/elegant/templates/registration/password_change_form.html` & `elegant_django-0.2.8/elegant/templates/registration/password_change_form.html`

 * *Files identical despite different names*

### Comparing `elegant_django-0.2.7/elegant/templates/reversion/object_history.html` & `elegant_django-0.2.8/elegant/templates/reversion/object_history.html`

 * *Files identical despite different names*

### Comparing `elegant_django-0.2.7/elegant/templates/reversion/recover_form.html` & `elegant_django-0.2.8/elegant/templates/reversion/recover_form.html`

 * *Files identical despite different names*

### Comparing `elegant_django-0.2.7/elegant/templates/reversion/recover_list.html` & `elegant_django-0.2.8/elegant/templates/reversion/recover_list.html`

 * *Files identical despite different names*

### Comparing `elegant_django-0.2.7/elegant/templates/reversion/revision_form.html` & `elegant_django-0.2.8/elegant/templates/reversion/revision_form.html`

 * *Files identical despite different names*

### Comparing `elegant_django-0.2.7/elegant/templates/shortcuts/base.html` & `elegant_django-0.2.8/elegant/templates/shortcuts/base.html`

 * *Files identical despite different names*

### Comparing `elegant_django-0.2.7/elegant/templates/shortcuts/style.css` & `elegant_django-0.2.8/elegant/templates/shortcuts/style.css`

 * *Files identical despite different names*

### Comparing `elegant_django-0.2.7/elegant/templates/suit_object_tools/change_form.html` & `elegant_django-0.2.8/elegant/templates/suit_object_tools/change_form.html`

 * *Files identical despite different names*

### Comparing `elegant_django-0.2.7/elegant/templatetags/elegant_analytics.py` & `elegant_django-0.2.8/elegant/templatetags/elegant_analytics.py`

 * *Files identical despite different names*

### Comparing `elegant_django-0.2.7/elegant/templatetags/elegant_formatting.py` & `elegant_django-0.2.8/elegant/templatetags/elegant_formatting.py`

 * *Files identical despite different names*

### Comparing `elegant_django-0.2.7/elegant/templatetags/elegant_list.py` & `elegant_django-0.2.8/elegant/templatetags/elegant_list.py`

 * *Files identical despite different names*

### Comparing `elegant_django-0.2.7/elegant/templatetags/elegant_menu.py` & `elegant_django-0.2.8/elegant/templatetags/elegant_menu.py`

 * *Files identical despite different names*

### Comparing `elegant_django-0.2.7/elegant/templatetags/elegant_shortcuts.py` & `elegant_django-0.2.8/elegant/templatetags/elegant_shortcuts.py`

 * *Files identical despite different names*

### Comparing `elegant_django-0.2.7/elegant/templatetags/elegant_tags.py` & `elegant_django-0.2.8/elegant/templatetags/elegant_tags.py`

 * *Files identical despite different names*

### Comparing `elegant_django-0.2.7/elegant/templatetags/formatting.py` & `elegant_django-0.2.8/elegant/templatetags/formatting.py`

 * *Files identical despite different names*

### Comparing `elegant_django-0.2.7/elegant/utils.py` & `elegant_django-0.2.8/elegant/utils.py`

 * *Files identical despite different names*

### Comparing `elegant_django-0.2.7/elegant/widgets/elegant.py` & `elegant_django-0.2.8/elegant/widgets/elegant.py`

 * *Files identical despite different names*

### Comparing `elegant_django-0.2.7/elegant/widgets/filter.py` & `elegant_django-0.2.8/elegant/widgets/filter.py`

 * *Files identical despite different names*

### Comparing `elegant_django-0.2.7/pyproject.toml` & `elegant_django-0.2.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "elegant-django"
-version = "0.2.7"
+version = "0.2.8"
 description = 'Modern theme for Django admin interface.'
 authors = ["bopo <ibopo@126.com>"]
 readme = "README.md"
 packages = [{ include = "elegant" }]
 classifiers = [
     'Development Status :: 5 - Production/Stable',
     'Framework :: Django',
```

### Comparing `elegant_django-0.2.7/PKG-INFO` & `elegant_django-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elegant-django
-Version: 0.2.7
+Version: 0.2.8
 Summary: Modern theme for Django admin interface.
 Author: bopo
 Author-email: ibopo@126.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -50,7 +50,8 @@
 ## 安装方法
 
 > 新手建议使用 `pip install elegant-django` 安装
 
 ## Stargazers over time
 
 [![Stargazers over time](https://starchart.cc/bopo/elegant-django.svg)](https://starchart.cc/bopo/elegant-django)
+
```

