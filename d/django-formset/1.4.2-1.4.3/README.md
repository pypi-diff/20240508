# Comparing `tmp/django_formset-1.4.2.tar.gz` & `tmp/django_formset-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_formset-1.4.2.tar", last modified: Tue May  7 12:43:58 2024, max compression
+gzip compressed data, was "django_formset-1.4.3.tar", last modified: Wed May  8 15:18:58 2024, max compression
```

## Comparing `django_formset-1.4.2.tar` & `django_formset-1.4.3.tar`

### file list

```diff
@@ -1,470 +1,470 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.422795 django_formset-1.4.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-07 12:43:26.000000 django_formset-1.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-07 12:43:26.000000 django_formset-1.4.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    14761 2024-05-07 12:43:58.418795 django_formset-1.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13679 2024-05-07 12:43:26.000000 django_formset-1.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.418795 django_formset-1.4.2/django_formset.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14761 2024-05-07 12:43:58.000000 django_formset-1.4.2/django_formset.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15360 2024-05-07 12:43:58.000000 django_formset-1.4.2/django_formset.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 12:43:58.000000 django_formset-1.4.2/django_formset.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 12:43:58.000000 django_formset-1.4.2/django_formset.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-07 12:43:58.000000 django_formset-1.4.2/django_formset.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-07 12:43:58.000000 django_formset-1.4.2/django_formset.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.370796 django_formset-1.4.2/formset/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9084 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/boundfield.py
--rw-r--r--   0 runner    (1001) docker     (127)     8500 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/calendar.py
--rw-r--r--   0 runner    (1001) docker     (127)    23321 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3387 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     2310 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/fieldset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.362796 django_formset-1.4.2/formset/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.350796 django_formset-1.4.2/formset/locale/af/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.370796 django_formset-1.4.2/formset/locale/af/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11275 2024-05-07 12:43:56.000000 django_formset-1.4.2/formset/locale/af/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10423 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/locale/af/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.350796 django_formset-1.4.2/formset/locale/ar/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.370796 django_formset-1.4.2/formset/locale/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    13178 2024-05-07 12:43:56.000000 django_formset-1.4.2/formset/locale/ar/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    12326 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/locale/ar/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.350796 django_formset-1.4.2/formset/locale/bg/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.370796 django_formset-1.4.2/formset/locale/bg/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    13577 2024-05-07 12:43:56.000000 django_formset-1.4.2/formset/locale/bg/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    12725 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/locale/bg/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.350796 django_formset-1.4.2/formset/locale/ca/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.374796 django_formset-1.4.2/formset/locale/ca/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11474 2024-05-07 12:43:56.000000 django_formset-1.4.2/formset/locale/ca/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10622 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/locale/ca/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.350796 django_formset-1.4.2/formset/locale/cs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.374796 django_formset-1.4.2/formset/locale/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11368 2024-05-07 12:43:56.000000 django_formset-1.4.2/formset/locale/cs/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10516 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/locale/cs/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.354796 django_formset-1.4.2/formset/locale/da/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.374796 django_formset-1.4.2/formset/locale/da/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11128 2024-05-07 12:43:56.000000 django_formset-1.4.2/formset/locale/da/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10276 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/locale/da/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.354796 django_formset-1.4.2/formset/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.374796 django_formset-1.4.2/formset/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     5609 2024-05-07 12:43:56.000000 django_formset-1.4.2/formset/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10620 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (127)    11333 2024-05-07 12:43:56.000000 django_formset-1.4.2/formset/locale/de/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10481 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/locale/de/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.354796 django_formset-1.4.2/formset/locale/el/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.374796 django_formset-1.4.2/formset/locale/el/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    13953 2024-05-07 12:43:56.000000 django_formset-1.4.2/formset/locale/el/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    13101 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/locale/el/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.354796 django_formset-1.4.2/formset/locale/eo/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.374796 django_formset-1.4.2/formset/locale/eo/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11077 2024-05-07 12:43:56.000000 django_formset-1.4.2/formset/locale/eo/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10225 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/locale/eo/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.354796 django_formset-1.4.2/formset/locale/es/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.374796 django_formset-1.4.2/formset/locale/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11318 2024-05-07 12:43:56.000000 django_formset-1.4.2/formset/locale/es/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10466 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/locale/es/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.354796 django_formset-1.4.2/formset/locale/et/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.374796 django_formset-1.4.2/formset/locale/et/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11114 2024-05-07 12:43:56.000000 django_formset-1.4.2/formset/locale/et/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10262 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/locale/et/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.354796 django_formset-1.4.2/formset/locale/eu/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.374796 django_formset-1.4.2/formset/locale/eu/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11248 2024-05-07 12:43:56.000000 django_formset-1.4.2/formset/locale/eu/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10396 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/locale/eu/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.354796 django_formset-1.4.2/formset/locale/eu_ES/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.374796 django_formset-1.4.2/formset/locale/eu_ES/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11251 2024-05-07 12:43:56.000000 django_formset-1.4.2/formset/locale/eu_ES/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10399 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/locale/eu_ES/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.354796 django_formset-1.4.2/formset/locale/fa/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.378796 django_formset-1.4.2/formset/locale/fa/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    12786 2024-05-07 12:43:56.000000 django_formset-1.4.2/formset/locale/fa/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    11934 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/locale/fa/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.354796 django_formset-1.4.2/formset/locale/fi/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.378796 django_formset-1.4.2/formset/locale/fi/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11039 2024-05-07 12:43:56.000000 django_formset-1.4.2/formset/locale/fi/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10187 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/locale/fi/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.354796 django_formset-1.4.2/formset/locale/fr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.378796 django_formset-1.4.2/formset/locale/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11382 2024-05-07 12:43:56.000000 django_formset-1.4.2/formset/locale/fr/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10530 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/locale/fr/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.354796 django_formset-1.4.2/formset/locale/he/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.378796 django_formset-1.4.2/formset/locale/he/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    12714 2024-05-07 12:43:56.000000 django_formset-1.4.2/formset/locale/he/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    11863 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/locale/he/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.354796 django_formset-1.4.2/formset/locale/he_IL/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.378796 django_formset-1.4.2/formset/locale/he_IL/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    12717 2024-05-07 12:43:56.000000 django_formset-1.4.2/formset/locale/he_IL/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    11866 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/locale/he_IL/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.354796 django_formset-1.4.2/formset/locale/hr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.378796 django_formset-1.4.2/formset/locale/hr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11353 2024-05-07 12:43:56.000000 django_formset-1.4.2/formset/locale/hr/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10501 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/locale/hr/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.354796 django_formset-1.4.2/formset/locale/hu/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.378796 django_formset-1.4.2/formset/locale/hu/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11444 2024-05-07 12:43:56.000000 django_formset-1.4.2/formset/locale/hu/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10592 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/locale/hu/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.354796 django_formset-1.4.2/formset/locale/hy/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.378796 django_formset-1.4.2/formset/locale/hy/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    13923 2024-05-07 12:43:56.000000 django_formset-1.4.2/formset/locale/hy/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    13071 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/locale/hy/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.354796 django_formset-1.4.2/formset/locale/it/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.378796 django_formset-1.4.2/formset/locale/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11188 2024-05-07 12:43:56.000000 django_formset-1.4.2/formset/locale/it/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10336 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/locale/it/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.354796 django_formset-1.4.2/formset/locale/ja/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.378796 django_formset-1.4.2/formset/locale/ja/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    12836 2024-05-07 12:43:56.000000 django_formset-1.4.2/formset/locale/ja/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    11984 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/locale/ja/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.358796 django_formset-1.4.2/formset/locale/ko_KR/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.382796 django_formset-1.4.2/formset/locale/ko_KR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11868 2024-05-07 12:43:56.000000 django_formset-1.4.2/formset/locale/ko_KR/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    11016 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/locale/ko_KR/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.358796 django_formset-1.4.2/formset/locale/lt/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.382796 django_formset-1.4.2/formset/locale/lt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11368 2024-05-07 12:43:56.000000 django_formset-1.4.2/formset/locale/lt/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10516 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/locale/lt/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.358796 django_formset-1.4.2/formset/locale/lv/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.382796 django_formset-1.4.2/formset/locale/lv/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11445 2024-05-07 12:43:56.000000 django_formset-1.4.2/formset/locale/lv/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10593 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/locale/lv/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.358796 django_formset-1.4.2/formset/locale/mn/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.382796 django_formset-1.4.2/formset/locale/mn/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    13211 2024-05-07 12:43:56.000000 django_formset-1.4.2/formset/locale/mn/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    12359 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/locale/mn/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.358796 django_formset-1.4.2/formset/locale/nb/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.382796 django_formset-1.4.2/formset/locale/nb/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11107 2024-05-07 12:43:56.000000 django_formset-1.4.2/formset/locale/nb/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10255 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/locale/nb/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.358796 django_formset-1.4.2/formset/locale/nl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.382796 django_formset-1.4.2/formset/locale/nl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11281 2024-05-07 12:43:56.000000 django_formset-1.4.2/formset/locale/nl/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10429 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/locale/nl/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.358796 django_formset-1.4.2/formset/locale/pl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.382796 django_formset-1.4.2/formset/locale/pl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11205 2024-05-07 12:43:56.000000 django_formset-1.4.2/formset/locale/pl/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10353 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/locale/pl/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.358796 django_formset-1.4.2/formset/locale/pt_BR/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.382796 django_formset-1.4.2/formset/locale/pt_BR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11263 2024-05-07 12:43:56.000000 django_formset-1.4.2/formset/locale/pt_BR/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10411 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/locale/pt_BR/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.358796 django_formset-1.4.2/formset/locale/pt_PT/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.382796 django_formset-1.4.2/formset/locale/pt_PT/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11321 2024-05-07 12:43:56.000000 django_formset-1.4.2/formset/locale/pt_PT/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10469 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/locale/pt_PT/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.358796 django_formset-1.4.2/formset/locale/ro/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.382796 django_formset-1.4.2/formset/locale/ro/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11197 2024-05-07 12:43:56.000000 django_formset-1.4.2/formset/locale/ro/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10345 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/locale/ro/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.358796 django_formset-1.4.2/formset/locale/ru/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.382796 django_formset-1.4.2/formset/locale/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    13828 2024-05-07 12:43:56.000000 django_formset-1.4.2/formset/locale/ru/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    12976 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/locale/ru/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.358796 django_formset-1.4.2/formset/locale/sk/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.386796 django_formset-1.4.2/formset/locale/sk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11294 2024-05-07 12:43:56.000000 django_formset-1.4.2/formset/locale/sk/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10442 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/locale/sk/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.358796 django_formset-1.4.2/formset/locale/sl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.386796 django_formset-1.4.2/formset/locale/sl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11239 2024-05-07 12:43:56.000000 django_formset-1.4.2/formset/locale/sl/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10387 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/locale/sl/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.358796 django_formset-1.4.2/formset/locale/sr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.386796 django_formset-1.4.2/formset/locale/sr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    13565 2024-05-07 12:43:56.000000 django_formset-1.4.2/formset/locale/sr/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    12713 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/locale/sr/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.358796 django_formset-1.4.2/formset/locale/sr_Latn/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.386796 django_formset-1.4.2/formset/locale/sr_Latn/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11233 2024-05-07 12:43:56.000000 django_formset-1.4.2/formset/locale/sr_Latn/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10381 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/locale/sr_Latn/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.362796 django_formset-1.4.2/formset/locale/sr_Latn_BA/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.386796 django_formset-1.4.2/formset/locale/sr_Latn_BA/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11185 2024-05-07 12:43:56.000000 django_formset-1.4.2/formset/locale/sr_Latn_BA/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10333 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/locale/sr_Latn_BA/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.362796 django_formset-1.4.2/formset/locale/sv/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.386796 django_formset-1.4.2/formset/locale/sv/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11228 2024-05-07 12:43:56.000000 django_formset-1.4.2/formset/locale/sv/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10376 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/locale/sv/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.362796 django_formset-1.4.2/formset/locale/tr_TR/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.386796 django_formset-1.4.2/formset/locale/tr_TR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11276 2024-05-07 12:43:56.000000 django_formset-1.4.2/formset/locale/tr_TR/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10424 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/locale/tr_TR/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.362796 django_formset-1.4.2/formset/locale/uk/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.386796 django_formset-1.4.2/formset/locale/uk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    13766 2024-05-07 12:43:56.000000 django_formset-1.4.2/formset/locale/uk/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    12914 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/locale/uk/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.362796 django_formset-1.4.2/formset/locale/zh_CN/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.386796 django_formset-1.4.2/formset/locale/zh_CN/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11598 2024-05-07 12:43:56.000000 django_formset-1.4.2/formset/locale/zh_CN/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10746 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/locale/zh_CN/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.362796 django_formset-1.4.2/formset/locale/zh_Hans/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.386796 django_formset-1.4.2/formset/locale/zh_Hans/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11600 2024-05-07 12:43:56.000000 django_formset-1.4.2/formset/locale/zh_Hans/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10748 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/locale/zh_Hans/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.362796 django_formset-1.4.2/formset/locale/zh_Hant/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.390796 django_formset-1.4.2/formset/locale/zh_Hant/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11401 2024-05-07 12:43:56.000000 django_formset-1.4.2/formset/locale/zh_Hant/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10549 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/locale/zh_Hant/LC_MESSAGES/djangojs.po
--rw-r--r--   0 runner    (1001) docker     (127)     4788 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/ranges.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.390796 django_formset-1.4.2/formset/renderers/
--rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/renderers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6131 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/renderers/bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/renderers/bulma.py
--rw-r--r--   0 runner    (1001) docker     (127)     7416 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/renderers/default.py
--rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/renderers/foundation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5894 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/renderers/tailwind.py
--rw-r--r--   0 runner    (1001) docker     (127)     2984 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/renderers/uikit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.390796 django_formset-1.4.2/formset/richtext/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/richtext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7894 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/richtext/controls.py
--rw-r--r--   0 runner    (1001) docker     (127)     4338 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/richtext/dialogs.py
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/richtext/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/richtext/widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.362796 django_formset-1.4.2/formset/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.362796 django_formset-1.4.2/formset/static/formset/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.390796 django_formset-1.4.2/formset/static/formset/css/
--rw-r--r--   0 runner    (1001) docker     (127)     2445 2024-05-07 12:43:53.000000 django_formset-1.4.2/formset/static/formset/css/bootstrap5-extra.css
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-07 12:43:53.000000 django_formset-1.4.2/formset/static/formset/css/bootstrap5-extra.css.map
--rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-05-07 12:43:53.000000 django_formset-1.4.2/formset/static/formset/css/collections.css
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-07 12:43:53.000000 django_formset-1.4.2/formset/static/formset/css/collections.css.map
--rw-r--r--   0 runner    (1001) docker     (127)    38474 2024-05-07 12:43:54.000000 django_formset-1.4.2/formset/static/formset/css/tailwind.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.394796 django_formset-1.4.2/formset/static/formset/icons/
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/static/formset/icons/file-audio.svg
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/static/formset/icons/file-empty.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/static/formset/icons/file-font.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/static/formset/icons/file-missing.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/static/formset/icons/file-pdf.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/static/formset/icons/file-picture.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/static/formset/icons/file-unknown.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/static/formset/icons/file-video.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/static/formset/icons/file-zip.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.398796 django_formset-1.4.2/formset/static/formset/js/
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-07 12:43:55.000000 django_formset-1.4.2/formset/static/formset/js/Calendar-5KXZG25G.js
--rw-r--r--   0 runner    (1001) docker     (127)    44541 2024-05-07 12:43:55.000000 django_formset-1.4.2/formset/static/formset/js/CountrySelectize-RPAYKZSN.js
--rw-r--r--   0 runner    (1001) docker     (127)    17740 2024-05-07 12:43:55.000000 django_formset-1.4.2/formset/static/formset/js/DateTime-WW4TXK6Y.js
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-07 12:43:55.000000 django_formset-1.4.2/formset/static/formset/js/DjangoSelectize-XUOHPSUG.js
--rw-r--r--   0 runner    (1001) docker     (127)    11534 2024-05-07 12:43:55.000000 django_formset-1.4.2/formset/static/formset/js/DjangoSlug-SHZN726V.js
--rw-r--r--   0 runner    (1001) docker     (127)    14773 2024-05-07 12:43:55.000000 django_formset-1.4.2/formset/static/formset/js/DualSelector-G47GXWWH.js
--rw-r--r--   0 runner    (1001) docker     (127)   270393 2024-05-07 12:43:55.000000 django_formset-1.4.2/formset/static/formset/js/PhoneNumber-RCXY4VXK.js
--rw-r--r--   0 runner    (1001) docker     (127)   313209 2024-05-07 12:43:55.000000 django_formset-1.4.2/formset/static/formset/js/RichtextArea-34WSI64S.js
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-07 12:43:55.000000 django_formset-1.4.2/formset/static/formset/js/SortableSelect-6YQLVCNF.js
--rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-05-07 12:43:55.000000 django_formset-1.4.2/formset/static/formset/js/chunk-65OJRBX6.js
--rw-r--r--   0 runner    (1001) docker     (127)    58061 2024-05-07 12:43:55.000000 django_formset-1.4.2/formset/static/formset/js/chunk-6IBLXZPA.js
--rw-r--r--   0 runner    (1001) docker     (127)    68979 2024-05-07 12:43:55.000000 django_formset-1.4.2/formset/static/formset/js/chunk-B7PX5YAU.js
--rw-r--r--   0 runner    (1001) docker     (127)     9669 2024-05-07 12:43:55.000000 django_formset-1.4.2/formset/static/formset/js/chunk-FDUUONAQ.js
--rw-r--r--   0 runner    (1001) docker     (127)    44439 2024-05-07 12:43:55.000000 django_formset-1.4.2/formset/static/formset/js/chunk-NOGHTXP6.js
--rw-r--r--   0 runner    (1001) docker     (127)      691 2024-05-07 12:43:55.000000 django_formset-1.4.2/formset/static/formset/js/chunk-P2VM2T3G.js
--rw-r--r--   0 runner    (1001) docker     (127)    15239 2024-05-07 12:43:55.000000 django_formset-1.4.2/formset/static/formset/js/chunk-RLE6ONWJ.js
--rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-05-07 12:43:55.000000 django_formset-1.4.2/formset/static/formset/js/chunk-SERXULES.js
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-07 12:43:55.000000 django_formset-1.4.2/formset/static/formset/js/chunk-W5RPWA2M.js
--rw-r--r--   0 runner    (1001) docker     (127)    27118 2024-05-07 12:43:55.000000 django_formset-1.4.2/formset/static/formset/js/chunk-WKRSL2PQ.js
--rw-r--r--   0 runner    (1001) docker     (127)     4096 2024-05-07 12:43:55.000000 django_formset-1.4.2/formset/static/formset/js/chunk-XO2BBJ6P.js
--rw-r--r--   0 runner    (1001) docker     (127)    63688 2024-05-07 12:43:55.000000 django_formset-1.4.2/formset/static/formset/js/django-formset.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.398796 django_formset-1.4.2/formset/static/formset/tiptap-extensions/
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/static/formset/tiptap-extensions/footnote.js
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/static/formset/tiptap-extensions/procurator.js
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/static/formset/tiptap-extensions/simple_image.js
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/static/formset/tiptap-extensions/simple_link.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.366796 django_formset-1.4.2/formset/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.362796 django_formset-1.4.2/formset/templates/admin/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.398796 django_formset-1.4.2/formset/templates/admin/formset/
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/admin/formset/change_form.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.398796 django_formset-1.4.2/formset/templates/calendar/
--rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/calendar/hours.html
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/calendar/months.html
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/calendar/range.html
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/calendar/weeks.html
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/calendar/years.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.398796 django_formset-1.4.2/formset/templates/formset/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.398796 django_formset-1.4.2/formset/templates/formset/bootstrap/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.398796 django_formset-1.4.2/formset/templates/formset/bootstrap/buttons/
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/bootstrap/buttons/add_collection.html
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/bootstrap/buttons/remove_collection.html
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/bootstrap/buttons/richtext_align.html
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/bootstrap/buttons/richtext_color.html
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/bootstrap/buttons/richtext_heading.html
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/bootstrap/field_group.html
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/bootstrap/form.html
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/bootstrap/help_text.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.398796 django_formset-1.4.2/formset/templates/formset/bootstrap/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/bootstrap/widgets/checkbox.html
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/bootstrap/widgets/dual_selector.html
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/bootstrap/widgets/file.html
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/bootstrap/widgets/input_option.html
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/bootstrap/widgets/multiple_input.html
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/bootstrap/widgets/richtextarea.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.402796 django_formset-1.4.2/formset/templates/formset/bulma/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.402796 django_formset-1.4.2/formset/templates/formset/bulma/buttons/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/bulma/buttons/add_collection.html
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/bulma/buttons/remove_collection.html
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/bulma/field_group.html
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/bulma/form.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.402796 django_formset-1.4.2/formset/templates/formset/bulma/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/bulma/widgets/checkbox.html
--rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/bulma/widgets/dual_selector.html
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/bulma/widgets/file.html
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/bulma/widgets/input_option.html
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/bulma/widgets/multiple_input.html
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/bulma/widgets/select.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.402796 django_formset-1.4.2/formset/templates/formset/default/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.402796 django_formset-1.4.2/formset/templates/formset/default/buttons/
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/default/buttons/add_collection.html
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/default/buttons/move_all_left.html
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/default/buttons/move_all_right.html
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/default/buttons/move_selected_left.html
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/default/buttons/move_selected_right.html
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/default/buttons/redo_selected.html
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/default/buttons/remove_collection.html
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/default/buttons/undo_selected.html
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/default/collection.html
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/default/detached_field.html
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/default/field_errors.html
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/default/field_group.html
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/default/fieldset.html
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/default/form.html
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/default/form_dialog.html
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/default/help_text.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.406796 django_formset-1.4.2/formset/templates/formset/default/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/default/widgets/button.html
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/default/widgets/calendar.html
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/default/widgets/country_selectize.html
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/default/widgets/datetime.html
--rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/default/widgets/dual_selector.html
--rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/default/widgets/file.html
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/default/widgets/multiple_input.html
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/default/widgets/richtextarea.html
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/default/widgets/select.html
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/default/widgets/selectize.html
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/form_attrs.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.406796 django_formset-1.4.2/formset/templates/formset/foundation/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.406796 django_formset-1.4.2/formset/templates/formset/foundation/buttons/
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/foundation/buttons/add_collection.html
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/foundation/buttons/remove_collection.html
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/foundation/field_group.html
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/foundation/form.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.406796 django_formset-1.4.2/formset/templates/formset/foundation/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/foundation/widgets/checkbox.html
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/foundation/widgets/dual_selector.html
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/foundation/widgets/file.html
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/foundation/widgets/inlined_input_option.html
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/foundation/widgets/multiple_input.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.414795 django_formset-1.4.2/formset/templates/formset/icons/
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/icons/activator.svg
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/icons/add-fill.svg
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/icons/align-center.svg
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/icons/align-justify.svg
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/icons/align-left.svg
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/icons/align-right.svg
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/icons/arrow-left.svg
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/icons/arrow-right.svg
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/icons/arrow-up.svg
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/icons/blockquote.svg
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/icons/bold.svg
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/icons/bulletlist.svg
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/icons/calendar-today.svg
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/icons/chevron-double-left.svg
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/icons/chevron-double-right.svg
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/icons/chevron-left.svg
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/icons/chevron-right.svg
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/icons/clearformat.svg
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/icons/codeblock.svg
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/icons/decreasemargin.svg
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/icons/delete-back.svg
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/icons/double-chevron-left.svg
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/icons/double-chevron-right.svg
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/icons/footnote.svg
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/icons/hardbreak.svg
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/icons/heading.svg
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/icons/heading1.svg
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/icons/heading2.svg
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/icons/heading3.svg
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/icons/heading4.svg
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/icons/heading5.svg
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/icons/heading6.svg
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/icons/horizontalrule.svg
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/icons/image.svg
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/icons/increasemargin.svg
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/icons/indentfirstline.svg
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/icons/italic.svg
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/icons/letters.svg
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/icons/link.svg
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/icons/orderedlist.svg
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/icons/outdentfirstline.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/icons/placeholder.svg
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/icons/questionmark.svg
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/icons/redo.svg
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/icons/reset.svg
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/icons/send.svg
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/icons/separator.svg
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/icons/strike.svg
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/icons/subscript.svg
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/icons/superscript.svg
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/icons/textcolor.svg
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/icons/trash.svg
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/icons/underline.svg
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/icons/undo.svg
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/icons/unlink.svg
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/non_field_errors.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.414795 django_formset-1.4.2/formset/templates/formset/richtext/
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/richtext/align.html
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/richtext/color.html
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/richtext/control.html
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/richtext/dialog_control.html
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/richtext/form_dialog.html
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/richtext/heading.html
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/richtext/separator.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.414795 django_formset-1.4.2/formset/templates/formset/tailwind/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.414795 django_formset-1.4.2/formset/templates/formset/tailwind/buttons/
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/tailwind/buttons/add_collection.html
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/tailwind/buttons/remove_collection.html
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/tailwind/field_group.html
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/tailwind/form.html
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/tailwind/help_text.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.414795 django_formset-1.4.2/formset/templates/formset/tailwind/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/tailwind/widgets/checkbox.html
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/tailwind/widgets/dual_selector.html
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/tailwind/widgets/file.html
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/tailwind/widgets/input_option.html
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/tailwind/widgets/multiple_input.html
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/tailwind/widgets/radio.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.414795 django_formset-1.4.2/formset/templates/formset/uikit/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.414795 django_formset-1.4.2/formset/templates/formset/uikit/buttons/
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/uikit/buttons/add_collection.html
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/uikit/buttons/remove_collection.html
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/uikit/field_group.html
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/uikit/form.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.414795 django_formset-1.4.2/formset/templates/formset/uikit/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/uikit/widgets/checkbox.html
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/uikit/widgets/file.html
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/uikit/widgets/input_option.html
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/formset/uikit/widgets/multiple_input.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.418795 django_formset-1.4.2/formset/templates/richtext/
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/richtext/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/richtext/bulletlist.html
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/richtext/doc.html
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/richtext/footnote.html
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/richtext/footnote_ref.html
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/richtext/footnotes_list.html
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/richtext/heading.html
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/richtext/horizontalrule.html
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/richtext/listitem.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.418795 django_formset-1.4.2/formset/templates/richtext/marks/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/richtext/marks/bold.html
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/richtext/marks/code.html
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/richtext/marks/italic.html
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/richtext/marks/procurator.html
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/richtext/marks/simple_link.html
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/richtext/marks/textcolor.html
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/richtext/marks/underline.html
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/richtext/orderedlist.html
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/richtext/paragraph.html
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templates/richtext/text.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:58.418795 django_formset-1.4.2/formset/templatetags/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templatetags/formsetify.py
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templatetags/phonenumber.py
--rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/templatetags/richtext.py
--rw-r--r--   0 runner    (1001) docker     (127)     5273 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/upload.py
--rw-r--r--   0 runner    (1001) docker     (127)     7275 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/validators.py
--rw-r--r--   0 runner    (1001) docker     (127)    12184 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/views.py
--rw-r--r--   0 runner    (1001) docker     (127)    21405 2024-05-07 12:43:26.000000 django_formset-1.4.2/formset/widgets.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 12:43:58.422795 django_formset-1.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-05-07 12:43:26.000000 django_formset-1.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.724098 django_formset-1.4.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-08 15:18:32.000000 django_formset-1.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-08 15:18:32.000000 django_formset-1.4.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    14761 2024-05-08 15:18:58.724098 django_formset-1.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13679 2024-05-08 15:18:32.000000 django_formset-1.4.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.724098 django_formset-1.4.3/django_formset.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14761 2024-05-08 15:18:58.000000 django_formset-1.4.3/django_formset.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15360 2024-05-08 15:18:58.000000 django_formset-1.4.3/django_formset.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 15:18:58.000000 django_formset-1.4.3/django_formset.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 15:18:58.000000 django_formset-1.4.3/django_formset.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-08 15:18:58.000000 django_formset-1.4.3/django_formset.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-08 15:18:58.000000 django_formset-1.4.3/django_formset.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.680098 django_formset-1.4.3/formset/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9084 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/boundfield.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8500 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/calendar.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23321 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3387 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2310 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/fieldset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.672098 django_formset-1.4.3/formset/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.664098 django_formset-1.4.3/formset/locale/af/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.680098 django_formset-1.4.3/formset/locale/af/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11275 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/locale/af/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10423 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/locale/af/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.664098 django_formset-1.4.3/formset/locale/ar/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.680098 django_formset-1.4.3/formset/locale/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    13178 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/locale/ar/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    12326 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/locale/ar/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.664098 django_formset-1.4.3/formset/locale/bg/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.680098 django_formset-1.4.3/formset/locale/bg/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    13577 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/locale/bg/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    12725 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/locale/bg/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.664098 django_formset-1.4.3/formset/locale/ca/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.680098 django_formset-1.4.3/formset/locale/ca/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11474 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/locale/ca/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10622 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/locale/ca/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.664098 django_formset-1.4.3/formset/locale/cs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.680098 django_formset-1.4.3/formset/locale/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11368 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/locale/cs/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10516 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/locale/cs/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.664098 django_formset-1.4.3/formset/locale/da/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.680098 django_formset-1.4.3/formset/locale/da/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11128 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/locale/da/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10276 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/locale/da/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.664098 django_formset-1.4.3/formset/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.680098 django_formset-1.4.3/formset/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     5609 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10620 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (127)    11333 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/locale/de/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10481 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/locale/de/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.664098 django_formset-1.4.3/formset/locale/el/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.680098 django_formset-1.4.3/formset/locale/el/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    13953 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/locale/el/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    13101 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/locale/el/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.664098 django_formset-1.4.3/formset/locale/eo/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.680098 django_formset-1.4.3/formset/locale/eo/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11077 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/locale/eo/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10225 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/locale/eo/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.664098 django_formset-1.4.3/formset/locale/es/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.684098 django_formset-1.4.3/formset/locale/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11318 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/locale/es/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10466 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/locale/es/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.664098 django_formset-1.4.3/formset/locale/et/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.684098 django_formset-1.4.3/formset/locale/et/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11114 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/locale/et/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10262 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/locale/et/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.664098 django_formset-1.4.3/formset/locale/eu/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.684098 django_formset-1.4.3/formset/locale/eu/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11248 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/locale/eu/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10396 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/locale/eu/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.664098 django_formset-1.4.3/formset/locale/eu_ES/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.684098 django_formset-1.4.3/formset/locale/eu_ES/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11251 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/locale/eu_ES/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10399 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/locale/eu_ES/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.664098 django_formset-1.4.3/formset/locale/fa/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.684098 django_formset-1.4.3/formset/locale/fa/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    12786 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/locale/fa/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    11934 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/locale/fa/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.664098 django_formset-1.4.3/formset/locale/fi/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.684098 django_formset-1.4.3/formset/locale/fi/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11039 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/locale/fi/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10187 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/locale/fi/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.664098 django_formset-1.4.3/formset/locale/fr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.684098 django_formset-1.4.3/formset/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11382 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/locale/fr/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10530 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/locale/fr/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.664098 django_formset-1.4.3/formset/locale/he/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.684098 django_formset-1.4.3/formset/locale/he/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    12714 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/locale/he/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    11863 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/locale/he/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.664098 django_formset-1.4.3/formset/locale/he_IL/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.684098 django_formset-1.4.3/formset/locale/he_IL/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    12717 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/locale/he_IL/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    11866 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/locale/he_IL/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.664098 django_formset-1.4.3/formset/locale/hr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.684098 django_formset-1.4.3/formset/locale/hr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11353 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/locale/hr/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10501 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/locale/hr/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.668098 django_formset-1.4.3/formset/locale/hu/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.684098 django_formset-1.4.3/formset/locale/hu/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11444 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/locale/hu/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10592 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/locale/hu/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.668098 django_formset-1.4.3/formset/locale/hy/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.684098 django_formset-1.4.3/formset/locale/hy/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    13923 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/locale/hy/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    13071 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/locale/hy/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.668098 django_formset-1.4.3/formset/locale/it/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.688098 django_formset-1.4.3/formset/locale/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11188 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/locale/it/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10336 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/locale/it/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.668098 django_formset-1.4.3/formset/locale/ja/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.688098 django_formset-1.4.3/formset/locale/ja/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    12836 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/locale/ja/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    11984 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/locale/ja/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.668098 django_formset-1.4.3/formset/locale/ko_KR/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.688098 django_formset-1.4.3/formset/locale/ko_KR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11868 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/locale/ko_KR/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    11016 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/locale/ko_KR/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.668098 django_formset-1.4.3/formset/locale/lt/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.688098 django_formset-1.4.3/formset/locale/lt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11368 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/locale/lt/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10516 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/locale/lt/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.668098 django_formset-1.4.3/formset/locale/lv/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.688098 django_formset-1.4.3/formset/locale/lv/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11445 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/locale/lv/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10593 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/locale/lv/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.668098 django_formset-1.4.3/formset/locale/mn/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.688098 django_formset-1.4.3/formset/locale/mn/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    13211 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/locale/mn/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    12359 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/locale/mn/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.668098 django_formset-1.4.3/formset/locale/nb/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.688098 django_formset-1.4.3/formset/locale/nb/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11107 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/locale/nb/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10255 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/locale/nb/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.668098 django_formset-1.4.3/formset/locale/nl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.688098 django_formset-1.4.3/formset/locale/nl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11281 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/locale/nl/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10429 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/locale/nl/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.668098 django_formset-1.4.3/formset/locale/pl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.688098 django_formset-1.4.3/formset/locale/pl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11205 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/locale/pl/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10353 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/locale/pl/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.668098 django_formset-1.4.3/formset/locale/pt_BR/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.688098 django_formset-1.4.3/formset/locale/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11263 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/locale/pt_BR/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10411 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/locale/pt_BR/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.668098 django_formset-1.4.3/formset/locale/pt_PT/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.688098 django_formset-1.4.3/formset/locale/pt_PT/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11321 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/locale/pt_PT/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10469 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/locale/pt_PT/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.668098 django_formset-1.4.3/formset/locale/ro/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.688098 django_formset-1.4.3/formset/locale/ro/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11197 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/locale/ro/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10345 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/locale/ro/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.668098 django_formset-1.4.3/formset/locale/ru/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.688098 django_formset-1.4.3/formset/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    13828 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/locale/ru/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    12976 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/locale/ru/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.668098 django_formset-1.4.3/formset/locale/sk/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.692098 django_formset-1.4.3/formset/locale/sk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11294 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/locale/sk/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10442 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/locale/sk/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.668098 django_formset-1.4.3/formset/locale/sl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.692098 django_formset-1.4.3/formset/locale/sl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11239 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/locale/sl/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10387 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/locale/sl/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.668098 django_formset-1.4.3/formset/locale/sr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.692098 django_formset-1.4.3/formset/locale/sr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    13565 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/locale/sr/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    12713 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/locale/sr/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.668098 django_formset-1.4.3/formset/locale/sr_Latn/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.692098 django_formset-1.4.3/formset/locale/sr_Latn/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11233 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/locale/sr_Latn/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10381 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/locale/sr_Latn/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.672098 django_formset-1.4.3/formset/locale/sr_Latn_BA/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.692098 django_formset-1.4.3/formset/locale/sr_Latn_BA/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11185 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/locale/sr_Latn_BA/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10333 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/locale/sr_Latn_BA/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.672098 django_formset-1.4.3/formset/locale/sv/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.692098 django_formset-1.4.3/formset/locale/sv/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11228 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/locale/sv/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10376 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/locale/sv/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.672098 django_formset-1.4.3/formset/locale/tr_TR/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.692098 django_formset-1.4.3/formset/locale/tr_TR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11276 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/locale/tr_TR/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10424 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/locale/tr_TR/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.672098 django_formset-1.4.3/formset/locale/uk/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.692098 django_formset-1.4.3/formset/locale/uk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    13766 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/locale/uk/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    12914 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/locale/uk/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.672098 django_formset-1.4.3/formset/locale/zh_CN/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.692098 django_formset-1.4.3/formset/locale/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11598 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/locale/zh_CN/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10746 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/locale/zh_CN/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.672098 django_formset-1.4.3/formset/locale/zh_Hans/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.692098 django_formset-1.4.3/formset/locale/zh_Hans/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11600 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/locale/zh_Hans/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10748 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/locale/zh_Hans/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.672098 django_formset-1.4.3/formset/locale/zh_Hant/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.692098 django_formset-1.4.3/formset/locale/zh_Hant/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11401 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/locale/zh_Hant/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10549 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/locale/zh_Hant/LC_MESSAGES/djangojs.po
+-rw-r--r--   0 runner    (1001) docker     (127)     4788 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/ranges.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.696098 django_formset-1.4.3/formset/renderers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/renderers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6131 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/renderers/bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/renderers/bulma.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7416 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/renderers/default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/renderers/foundation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5894 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/renderers/tailwind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2984 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/renderers/uikit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.696098 django_formset-1.4.3/formset/richtext/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/richtext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7894 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/richtext/controls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4338 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/richtext/dialogs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/richtext/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/richtext/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.672098 django_formset-1.4.3/formset/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.672098 django_formset-1.4.3/formset/static/formset/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.696098 django_formset-1.4.3/formset/static/formset/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     2445 2024-05-08 15:18:54.000000 django_formset-1.4.3/formset/static/formset/css/bootstrap5-extra.css
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-08 15:18:54.000000 django_formset-1.4.3/formset/static/formset/css/bootstrap5-extra.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-05-08 15:18:54.000000 django_formset-1.4.3/formset/static/formset/css/collections.css
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-08 15:18:54.000000 django_formset-1.4.3/formset/static/formset/css/collections.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)    38474 2024-05-08 15:18:55.000000 django_formset-1.4.3/formset/static/formset/css/tailwind.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.696098 django_formset-1.4.3/formset/static/formset/icons/
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/static/formset/icons/file-audio.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/static/formset/icons/file-empty.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/static/formset/icons/file-font.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/static/formset/icons/file-missing.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/static/formset/icons/file-pdf.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/static/formset/icons/file-picture.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/static/formset/icons/file-unknown.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/static/formset/icons/file-video.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/static/formset/icons/file-zip.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.704098 django_formset-1.4.3/formset/static/formset/js/
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/static/formset/js/Calendar-6GWQDXEH.js
+-rw-r--r--   0 runner    (1001) docker     (127)    44541 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/static/formset/js/CountrySelectize-SV3ETVIG.js
+-rw-r--r--   0 runner    (1001) docker     (127)    17740 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/static/formset/js/DateTime-7RV5MOXB.js
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/static/formset/js/DjangoSelectize-FCAZIQIK.js
+-rw-r--r--   0 runner    (1001) docker     (127)    11534 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/static/formset/js/DjangoSlug-SHZN726V.js
+-rw-r--r--   0 runner    (1001) docker     (127)    14773 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/static/formset/js/DualSelector-TFBRBEV6.js
+-rw-r--r--   0 runner    (1001) docker     (127)   270424 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/static/formset/js/PhoneNumber-XY2VHR24.js
+-rw-r--r--   0 runner    (1001) docker     (127)   313209 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/static/formset/js/RichtextArea-PVV6GJIQ.js
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/static/formset/js/SortableSelect-3ABJOEP2.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/static/formset/js/chunk-65OJRBX6.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9669 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/static/formset/js/chunk-FDUUONAQ.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4096 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/static/formset/js/chunk-IH7AT57W.js
+-rw-r--r--   0 runner    (1001) docker     (127)    44439 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/static/formset/js/chunk-NOGHTXP6.js
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/static/formset/js/chunk-P2VM2T3G.js
+-rw-r--r--   0 runner    (1001) docker     (127)    58061 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/static/formset/js/chunk-R3EYKSPB.js
+-rw-r--r--   0 runner    (1001) docker     (127)    15239 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/static/formset/js/chunk-RLE6ONWJ.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/static/formset/js/chunk-SERXULES.js
+-rw-r--r--   0 runner    (1001) docker     (127)    27118 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/static/formset/js/chunk-TRJBB73N.js
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/static/formset/js/chunk-W5RPWA2M.js
+-rw-r--r--   0 runner    (1001) docker     (127)    68979 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/static/formset/js/chunk-YMY5H5XX.js
+-rw-r--r--   0 runner    (1001) docker     (127)    64081 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/static/formset/js/django-formset.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.704098 django_formset-1.4.3/formset/static/formset/tiptap-extensions/
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/static/formset/tiptap-extensions/footnote.js
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/static/formset/tiptap-extensions/procurator.js
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/static/formset/tiptap-extensions/simple_image.js
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/static/formset/tiptap-extensions/simple_link.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.676098 django_formset-1.4.3/formset/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.672098 django_formset-1.4.3/formset/templates/admin/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.704098 django_formset-1.4.3/formset/templates/admin/formset/
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/admin/formset/change_form.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.704098 django_formset-1.4.3/formset/templates/calendar/
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/calendar/hours.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/calendar/months.html
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/calendar/range.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/calendar/weeks.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/calendar/years.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.704098 django_formset-1.4.3/formset/templates/formset/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.704098 django_formset-1.4.3/formset/templates/formset/bootstrap/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.704098 django_formset-1.4.3/formset/templates/formset/bootstrap/buttons/
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/bootstrap/buttons/add_collection.html
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/bootstrap/buttons/remove_collection.html
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/bootstrap/buttons/richtext_align.html
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/bootstrap/buttons/richtext_color.html
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/bootstrap/buttons/richtext_heading.html
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/bootstrap/field_group.html
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/bootstrap/form.html
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/bootstrap/help_text.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.704098 django_formset-1.4.3/formset/templates/formset/bootstrap/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/bootstrap/widgets/checkbox.html
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/bootstrap/widgets/dual_selector.html
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/bootstrap/widgets/file.html
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/bootstrap/widgets/input_option.html
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/bootstrap/widgets/multiple_input.html
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/bootstrap/widgets/richtextarea.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.708098 django_formset-1.4.3/formset/templates/formset/bulma/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.708098 django_formset-1.4.3/formset/templates/formset/bulma/buttons/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/bulma/buttons/add_collection.html
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/bulma/buttons/remove_collection.html
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/bulma/field_group.html
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/bulma/form.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.708098 django_formset-1.4.3/formset/templates/formset/bulma/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/bulma/widgets/checkbox.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/bulma/widgets/dual_selector.html
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/bulma/widgets/file.html
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/bulma/widgets/input_option.html
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/bulma/widgets/multiple_input.html
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/bulma/widgets/select.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.708098 django_formset-1.4.3/formset/templates/formset/default/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.708098 django_formset-1.4.3/formset/templates/formset/default/buttons/
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/default/buttons/add_collection.html
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/default/buttons/move_all_left.html
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/default/buttons/move_all_right.html
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/default/buttons/move_selected_left.html
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/default/buttons/move_selected_right.html
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/default/buttons/redo_selected.html
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/default/buttons/remove_collection.html
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/default/buttons/undo_selected.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/default/collection.html
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/default/detached_field.html
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/default/field_errors.html
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/default/field_group.html
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/default/fieldset.html
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/default/form.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/default/form_dialog.html
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/default/help_text.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.712098 django_formset-1.4.3/formset/templates/formset/default/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/default/widgets/button.html
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/default/widgets/calendar.html
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/default/widgets/country_selectize.html
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/default/widgets/datetime.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/default/widgets/dual_selector.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/default/widgets/file.html
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/default/widgets/multiple_input.html
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/default/widgets/richtextarea.html
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/default/widgets/select.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/default/widgets/selectize.html
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/form_attrs.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.712098 django_formset-1.4.3/formset/templates/formset/foundation/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.712098 django_formset-1.4.3/formset/templates/formset/foundation/buttons/
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/foundation/buttons/add_collection.html
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/foundation/buttons/remove_collection.html
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/foundation/field_group.html
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/foundation/form.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.712098 django_formset-1.4.3/formset/templates/formset/foundation/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/foundation/widgets/checkbox.html
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/foundation/widgets/dual_selector.html
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/foundation/widgets/file.html
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/foundation/widgets/inlined_input_option.html
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/foundation/widgets/multiple_input.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.720098 django_formset-1.4.3/formset/templates/formset/icons/
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/icons/activator.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/icons/add-fill.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/icons/align-center.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/icons/align-justify.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/icons/align-left.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/icons/align-right.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/icons/arrow-left.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/icons/arrow-right.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/icons/arrow-up.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/icons/blockquote.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/icons/bold.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/icons/bulletlist.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/icons/calendar-today.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/icons/chevron-double-left.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/icons/chevron-double-right.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/icons/chevron-left.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/icons/chevron-right.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/icons/clearformat.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/icons/codeblock.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/icons/decreasemargin.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/icons/delete-back.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/icons/double-chevron-left.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/icons/double-chevron-right.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/icons/footnote.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/icons/hardbreak.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/icons/heading.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/icons/heading1.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/icons/heading2.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/icons/heading3.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/icons/heading4.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/icons/heading5.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/icons/heading6.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/icons/horizontalrule.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/icons/image.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/icons/increasemargin.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/icons/indentfirstline.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/icons/italic.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/icons/letters.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/icons/link.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/icons/orderedlist.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/icons/outdentfirstline.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/icons/placeholder.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/icons/questionmark.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/icons/redo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/icons/reset.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/icons/send.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/icons/separator.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/icons/strike.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/icons/subscript.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/icons/superscript.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/icons/textcolor.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/icons/trash.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/icons/underline.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/icons/undo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/icons/unlink.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/non_field_errors.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.720098 django_formset-1.4.3/formset/templates/formset/richtext/
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/richtext/align.html
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/richtext/color.html
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/richtext/control.html
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/richtext/dialog_control.html
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/richtext/form_dialog.html
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/richtext/heading.html
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/richtext/separator.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.720098 django_formset-1.4.3/formset/templates/formset/tailwind/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.720098 django_formset-1.4.3/formset/templates/formset/tailwind/buttons/
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/tailwind/buttons/add_collection.html
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/tailwind/buttons/remove_collection.html
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/tailwind/field_group.html
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/tailwind/form.html
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/tailwind/help_text.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.720098 django_formset-1.4.3/formset/templates/formset/tailwind/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/tailwind/widgets/checkbox.html
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/tailwind/widgets/dual_selector.html
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/tailwind/widgets/file.html
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/tailwind/widgets/input_option.html
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/tailwind/widgets/multiple_input.html
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/tailwind/widgets/radio.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.720098 django_formset-1.4.3/formset/templates/formset/uikit/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.720098 django_formset-1.4.3/formset/templates/formset/uikit/buttons/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/uikit/buttons/add_collection.html
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/uikit/buttons/remove_collection.html
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/uikit/field_group.html
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/uikit/form.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.720098 django_formset-1.4.3/formset/templates/formset/uikit/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/uikit/widgets/checkbox.html
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/uikit/widgets/file.html
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/uikit/widgets/input_option.html
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/uikit/widgets/multiple_input.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.724098 django_formset-1.4.3/formset/templates/richtext/
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/richtext/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/richtext/bulletlist.html
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/richtext/doc.html
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/richtext/footnote.html
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/richtext/footnote_ref.html
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/richtext/footnotes_list.html
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/richtext/heading.html
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/richtext/horizontalrule.html
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/richtext/listitem.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.724098 django_formset-1.4.3/formset/templates/richtext/marks/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/richtext/marks/bold.html
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/richtext/marks/code.html
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/richtext/marks/italic.html
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/richtext/marks/procurator.html
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/richtext/marks/simple_link.html
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/richtext/marks/textcolor.html
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/richtext/marks/underline.html
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/richtext/orderedlist.html
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/richtext/paragraph.html
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/richtext/text.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.724098 django_formset-1.4.3/formset/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templatetags/formsetify.py
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templatetags/phonenumber.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templatetags/richtext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5273 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/upload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7275 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12184 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22391 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/widgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 15:18:58.724098 django_formset-1.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-05-08 15:18:32.000000 django_formset-1.4.3/setup.py
```

### Comparing `django_formset-1.4.2/LICENSE` & `django_formset-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/PKG-INFO` & `django_formset-1.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-formset
-Version: 1.4.2
+Version: 1.4.3
 Summary: The missing widgets and form manipulation library for Django
 Home-page: https://github.com/jrief/django-formset
 Author: Jacob Rief
 Author-email: jacob.rief@gmail.com
 License: MIT
 Keywords: Django Forms,webcomponent
 Platform: OS Independent
```

### Comparing `django_formset-1.4.2/README.md` & `django_formset-1.4.3/README.md`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/django_formset.egg-info/PKG-INFO` & `django_formset-1.4.3/django_formset.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-formset
-Version: 1.4.2
+Version: 1.4.3
 Summary: The missing widgets and form manipulation library for Django
 Home-page: https://github.com/jrief/django-formset
 Author: Jacob Rief
 Author-email: jacob.rief@gmail.com
 License: MIT
 Keywords: Django Forms,webcomponent
 Platform: OS Independent
```

### Comparing `django_formset-1.4.2/django_formset.egg-info/SOURCES.txt` & `django_formset-1.4.3/django_formset.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -136,34 +136,34 @@
 formset/static/formset/icons/file-font.svg
 formset/static/formset/icons/file-missing.svg
 formset/static/formset/icons/file-pdf.svg
 formset/static/formset/icons/file-picture.svg
 formset/static/formset/icons/file-unknown.svg
 formset/static/formset/icons/file-video.svg
 formset/static/formset/icons/file-zip.svg
-formset/static/formset/js/Calendar-5KXZG25G.js
-formset/static/formset/js/CountrySelectize-RPAYKZSN.js
-formset/static/formset/js/DateTime-WW4TXK6Y.js
-formset/static/formset/js/DjangoSelectize-XUOHPSUG.js
+formset/static/formset/js/Calendar-6GWQDXEH.js
+formset/static/formset/js/CountrySelectize-SV3ETVIG.js
+formset/static/formset/js/DateTime-7RV5MOXB.js
+formset/static/formset/js/DjangoSelectize-FCAZIQIK.js
 formset/static/formset/js/DjangoSlug-SHZN726V.js
-formset/static/formset/js/DualSelector-G47GXWWH.js
-formset/static/formset/js/PhoneNumber-RCXY4VXK.js
-formset/static/formset/js/RichtextArea-34WSI64S.js
-formset/static/formset/js/SortableSelect-6YQLVCNF.js
+formset/static/formset/js/DualSelector-TFBRBEV6.js
+formset/static/formset/js/PhoneNumber-XY2VHR24.js
+formset/static/formset/js/RichtextArea-PVV6GJIQ.js
+formset/static/formset/js/SortableSelect-3ABJOEP2.js
 formset/static/formset/js/chunk-65OJRBX6.js
-formset/static/formset/js/chunk-6IBLXZPA.js
-formset/static/formset/js/chunk-B7PX5YAU.js
 formset/static/formset/js/chunk-FDUUONAQ.js
+formset/static/formset/js/chunk-IH7AT57W.js
 formset/static/formset/js/chunk-NOGHTXP6.js
 formset/static/formset/js/chunk-P2VM2T3G.js
+formset/static/formset/js/chunk-R3EYKSPB.js
 formset/static/formset/js/chunk-RLE6ONWJ.js
 formset/static/formset/js/chunk-SERXULES.js
+formset/static/formset/js/chunk-TRJBB73N.js
 formset/static/formset/js/chunk-W5RPWA2M.js
-formset/static/formset/js/chunk-WKRSL2PQ.js
-formset/static/formset/js/chunk-XO2BBJ6P.js
+formset/static/formset/js/chunk-YMY5H5XX.js
 formset/static/formset/js/django-formset.js
 formset/static/formset/tiptap-extensions/footnote.js
 formset/static/formset/tiptap-extensions/procurator.js
 formset/static/formset/tiptap-extensions/simple_image.js
 formset/static/formset/tiptap-extensions/simple_link.js
 formset/templates/admin/formset/change_form.html
 formset/templates/calendar/hours.html
```

### Comparing `django_formset-1.4.2/formset/boundfield.py` & `django_formset-1.4.3/formset/boundfield.py`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/calendar.py` & `django_formset-1.4.3/formset/calendar.py`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/collection.py` & `django_formset-1.4.3/formset/collection.py`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/dialog.py` & `django_formset-1.4.3/formset/dialog.py`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/fields.py` & `django_formset-1.4.3/formset/fields.py`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/fieldset.py` & `django_formset-1.4.3/formset/fieldset.py`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/locale/af/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.3/formset/locale/af/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/locale/af/LC_MESSAGES/djangojs.po` & `django_formset-1.4.3/formset/locale/af/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/locale/ar/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.3/formset/locale/ar/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/locale/ar/LC_MESSAGES/djangojs.po` & `django_formset-1.4.3/formset/locale/ar/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/locale/bg/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.3/formset/locale/bg/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/locale/bg/LC_MESSAGES/djangojs.po` & `django_formset-1.4.3/formset/locale/bg/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/locale/ca/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.3/formset/locale/ca/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/locale/ca/LC_MESSAGES/djangojs.po` & `django_formset-1.4.3/formset/locale/ca/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/locale/cs/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.3/formset/locale/cs/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/locale/cs/LC_MESSAGES/djangojs.po` & `django_formset-1.4.3/formset/locale/cs/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/locale/da/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.3/formset/locale/da/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/locale/da/LC_MESSAGES/djangojs.po` & `django_formset-1.4.3/formset/locale/da/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/locale/de/LC_MESSAGES/django.mo` & `django_formset-1.4.3/formset/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/locale/de/LC_MESSAGES/django.po` & `django_formset-1.4.3/formset/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/locale/de/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.3/formset/locale/de/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/locale/de/LC_MESSAGES/djangojs.po` & `django_formset-1.4.3/formset/locale/de/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/locale/el/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.3/formset/locale/el/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/locale/el/LC_MESSAGES/djangojs.po` & `django_formset-1.4.3/formset/locale/el/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/locale/eo/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.3/formset/locale/eo/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/locale/eo/LC_MESSAGES/djangojs.po` & `django_formset-1.4.3/formset/locale/eo/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/locale/es/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.3/formset/locale/es/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/locale/es/LC_MESSAGES/djangojs.po` & `django_formset-1.4.3/formset/locale/es/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/locale/et/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.3/formset/locale/et/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/locale/et/LC_MESSAGES/djangojs.po` & `django_formset-1.4.3/formset/locale/et/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/locale/eu/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.3/formset/locale/eu/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/locale/eu/LC_MESSAGES/djangojs.po` & `django_formset-1.4.3/formset/locale/eu/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/locale/eu_ES/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.3/formset/locale/eu_ES/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/locale/eu_ES/LC_MESSAGES/djangojs.po` & `django_formset-1.4.3/formset/locale/eu_ES/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/locale/fa/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.3/formset/locale/fa/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/locale/fa/LC_MESSAGES/djangojs.po` & `django_formset-1.4.3/formset/locale/fa/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/locale/fi/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.3/formset/locale/fi/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/locale/fi/LC_MESSAGES/djangojs.po` & `django_formset-1.4.3/formset/locale/fi/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/locale/fr/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.3/formset/locale/fr/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/locale/fr/LC_MESSAGES/djangojs.po` & `django_formset-1.4.3/formset/locale/fr/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/locale/he/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.3/formset/locale/he/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/locale/he/LC_MESSAGES/djangojs.po` & `django_formset-1.4.3/formset/locale/he/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/locale/he_IL/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.3/formset/locale/he_IL/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/locale/he_IL/LC_MESSAGES/djangojs.po` & `django_formset-1.4.3/formset/locale/he_IL/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/locale/hr/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.3/formset/locale/hr/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/locale/hr/LC_MESSAGES/djangojs.po` & `django_formset-1.4.3/formset/locale/hr/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/locale/hu/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.3/formset/locale/hu/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/locale/hu/LC_MESSAGES/djangojs.po` & `django_formset-1.4.3/formset/locale/hu/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/locale/hy/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.3/formset/locale/hy/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/locale/hy/LC_MESSAGES/djangojs.po` & `django_formset-1.4.3/formset/locale/hy/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/locale/it/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.3/formset/locale/it/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/locale/it/LC_MESSAGES/djangojs.po` & `django_formset-1.4.3/formset/locale/it/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/locale/ja/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.3/formset/locale/ja/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/locale/ja/LC_MESSAGES/djangojs.po` & `django_formset-1.4.3/formset/locale/ja/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/locale/ko_KR/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.3/formset/locale/ko_KR/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/locale/ko_KR/LC_MESSAGES/djangojs.po` & `django_formset-1.4.3/formset/locale/ko_KR/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/locale/lt/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.3/formset/locale/lt/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/locale/lt/LC_MESSAGES/djangojs.po` & `django_formset-1.4.3/formset/locale/lt/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/locale/lv/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.3/formset/locale/lv/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/locale/lv/LC_MESSAGES/djangojs.po` & `django_formset-1.4.3/formset/locale/lv/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/locale/mn/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.3/formset/locale/mn/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/locale/mn/LC_MESSAGES/djangojs.po` & `django_formset-1.4.3/formset/locale/mn/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/locale/nb/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.3/formset/locale/nb/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/locale/nb/LC_MESSAGES/djangojs.po` & `django_formset-1.4.3/formset/locale/nb/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/locale/nl/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.3/formset/locale/nl/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/locale/nl/LC_MESSAGES/djangojs.po` & `django_formset-1.4.3/formset/locale/nl/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/locale/pl/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.3/formset/locale/pl/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/locale/pl/LC_MESSAGES/djangojs.po` & `django_formset-1.4.3/formset/locale/pl/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/locale/pt_BR/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.3/formset/locale/pt_BR/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/locale/pt_BR/LC_MESSAGES/djangojs.po` & `django_formset-1.4.3/formset/locale/pt_BR/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/locale/pt_PT/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.3/formset/locale/pt_PT/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/locale/pt_PT/LC_MESSAGES/djangojs.po` & `django_formset-1.4.3/formset/locale/pt_PT/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/locale/ro/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.3/formset/locale/ro/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/locale/ro/LC_MESSAGES/djangojs.po` & `django_formset-1.4.3/formset/locale/ro/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/locale/ru/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.3/formset/locale/ru/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/locale/ru/LC_MESSAGES/djangojs.po` & `django_formset-1.4.3/formset/locale/ru/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/locale/sk/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.3/formset/locale/sk/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/locale/sk/LC_MESSAGES/djangojs.po` & `django_formset-1.4.3/formset/locale/sk/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/locale/sl/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.3/formset/locale/sl/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/locale/sl/LC_MESSAGES/djangojs.po` & `django_formset-1.4.3/formset/locale/sl/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/locale/sr/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.3/formset/locale/sr/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/locale/sr/LC_MESSAGES/djangojs.po` & `django_formset-1.4.3/formset/locale/sr/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/locale/sr_Latn/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.3/formset/locale/sr_Latn/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/locale/sr_Latn/LC_MESSAGES/djangojs.po` & `django_formset-1.4.3/formset/locale/sr_Latn/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/locale/sr_Latn_BA/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.3/formset/locale/sr_Latn_BA/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/locale/sr_Latn_BA/LC_MESSAGES/djangojs.po` & `django_formset-1.4.3/formset/locale/sr_Latn_BA/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/locale/sv/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.3/formset/locale/sv/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/locale/sv/LC_MESSAGES/djangojs.po` & `django_formset-1.4.3/formset/locale/sv/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/locale/tr_TR/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.3/formset/locale/tr_TR/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/locale/tr_TR/LC_MESSAGES/djangojs.po` & `django_formset-1.4.3/formset/locale/tr_TR/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/locale/uk/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.3/formset/locale/uk/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/locale/uk/LC_MESSAGES/djangojs.po` & `django_formset-1.4.3/formset/locale/uk/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/locale/zh_CN/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.3/formset/locale/zh_CN/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/locale/zh_CN/LC_MESSAGES/djangojs.po` & `django_formset-1.4.3/formset/locale/zh_CN/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/locale/zh_Hans/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.3/formset/locale/zh_Hans/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/locale/zh_Hans/LC_MESSAGES/djangojs.po` & `django_formset-1.4.3/formset/locale/zh_Hans/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/locale/zh_Hant/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.3/formset/locale/zh_Hant/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/locale/zh_Hant/LC_MESSAGES/djangojs.po` & `django_formset-1.4.3/formset/locale/zh_Hant/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/ranges.py` & `django_formset-1.4.3/formset/ranges.py`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/renderers/__init__.py` & `django_formset-1.4.3/formset/renderers/__init__.py`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/renderers/bootstrap.py` & `django_formset-1.4.3/formset/renderers/bootstrap.py`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/renderers/bulma.py` & `django_formset-1.4.3/formset/renderers/bulma.py`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/renderers/default.py` & `django_formset-1.4.3/formset/renderers/default.py`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/renderers/foundation.py` & `django_formset-1.4.3/formset/renderers/foundation.py`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/renderers/tailwind.py` & `django_formset-1.4.3/formset/renderers/tailwind.py`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/renderers/uikit.py` & `django_formset-1.4.3/formset/renderers/uikit.py`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/richtext/controls.py` & `django_formset-1.4.3/formset/richtext/controls.py`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/richtext/dialogs.py` & `django_formset-1.4.3/formset/richtext/dialogs.py`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/richtext/widgets.py` & `django_formset-1.4.3/formset/richtext/widgets.py`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/static/formset/css/bootstrap5-extra.css` & `django_formset-1.4.3/formset/static/formset/css/bootstrap5-extra.css`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/static/formset/css/bootstrap5-extra.css.map` & `django_formset-1.4.3/formset/static/formset/css/bootstrap5-extra.css.map`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/static/formset/css/collections.css` & `django_formset-1.4.3/formset/static/formset/css/collections.css`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/static/formset/css/tailwind.css` & `django_formset-1.4.3/formset/static/formset/css/tailwind.css`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/static/formset/icons/file-audio.svg` & `django_formset-1.4.3/formset/static/formset/icons/file-audio.svg`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/static/formset/icons/file-empty.svg` & `django_formset-1.4.3/formset/static/formset/icons/file-empty.svg`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/static/formset/icons/file-font.svg` & `django_formset-1.4.3/formset/static/formset/icons/file-font.svg`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/static/formset/icons/file-missing.svg` & `django_formset-1.4.3/formset/static/formset/icons/file-missing.svg`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/static/formset/icons/file-pdf.svg` & `django_formset-1.4.3/formset/static/formset/icons/file-pdf.svg`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/static/formset/icons/file-picture.svg` & `django_formset-1.4.3/formset/static/formset/icons/file-picture.svg`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/static/formset/icons/file-unknown.svg` & `django_formset-1.4.3/formset/static/formset/icons/file-unknown.svg`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/static/formset/icons/file-video.svg` & `django_formset-1.4.3/formset/static/formset/icons/file-video.svg`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/static/formset/icons/file-zip.svg` & `django_formset-1.4.3/formset/static/formset/icons/file-zip.svg`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/static/formset/js/CountrySelectize-RPAYKZSN.js` & `django_formset-1.4.3/formset/static/formset/js/CountrySelectize-SV3ETVIG.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 import {
     a as c
-} from "./chunk-6IBLXZPA.js";
+} from "./chunk-R3EYKSPB.js";
 import "./chunk-SERXULES.js";
 import "./chunk-W5RPWA2M.js";
 import {
     a as r
 } from "./chunk-FDUUONAQ.js";
 import "./chunk-65OJRBX6.js";
 import {
```

### Comparing `django_formset-1.4.2/formset/static/formset/js/DateTime-WW4TXK6Y.js` & `django_formset-1.4.3/formset/static/formset/js/DateTime-7RV5MOXB.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 import {
     a as v
-} from "./chunk-WKRSL2PQ.js";
+} from "./chunk-TRJBB73N.js";
 import {
     b as m
 } from "./chunk-W5RPWA2M.js";
 import {
     a as x,
     c as f,
     d as g,
```

### Comparing `django_formset-1.4.2/formset/static/formset/js/DjangoSlug-SHZN726V.js` & `django_formset-1.4.3/formset/static/formset/js/DjangoSlug-SHZN726V.js`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/static/formset/js/DualSelector-G47GXWWH.js` & `django_formset-1.4.3/formset/static/formset/js/DualSelector-TFBRBEV6.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,14 +1,14 @@
 import {
     a as d
 } from "./chunk-SERXULES.js";
 import "./chunk-W5RPWA2M.js";
 import {
     a as p
-} from "./chunk-XO2BBJ6P.js";
+} from "./chunk-IH7AT57W.js";
 import "./chunk-NOGHTXP6.js";
 import {
     a as v
 } from "./chunk-FDUUONAQ.js";
 import {
     a as r
 } from "./chunk-65OJRBX6.js";
```

### Comparing `django_formset-1.4.2/formset/static/formset/js/PhoneNumber-RCXY4VXK.js` & `django_formset-1.4.3/formset/static/formset/js/PhoneNumber-XY2VHR24.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -5835,14 +5835,15 @@
             let t = this.internationalSelector.getBoundingClientRect();
             this.internationalSelector.style.width = `${Math.round(t.width)}px`, this.isOpen = !0, this.isPristine = !0, this.countryLookupField.value = "", this.deselectAll();
             let d = this.asYouType.getCountry();
             if (d) {
                 let a = this.internationalSelector.querySelector(`[data-country="${d}"]`);
                 a instanceof HTMLLIElement && (a.classList.add("selected"), a.scrollIntoView())
             }
+            this.countryLookupField.focus()
         }
         closeInternationalSelector() {
             var t;
             this.isOpen = !1, this.textBox.setAttribute("aria-expanded", "false"), (t = this.cleanup) == null || t.call(this)
         }
         setInternationalCode(t, d) {
             var i;
```

### Comparing `django_formset-1.4.2/formset/static/formset/js/RichtextArea-34WSI64S.js` & `django_formset-1.4.3/formset/static/formset/js/RichtextArea-PVV6GJIQ.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,13 +1,13 @@
 import {
     a as fa,
     b as ha,
     c as pa,
     f as Vi
-} from "./chunk-B7PX5YAU.js";
+} from "./chunk-YMY5H5XX.js";
 import {
     a as ma
 } from "./chunk-FDUUONAQ.js";
 import {
     e as ji
 } from "./chunk-RLE6ONWJ.js";
 import {
```

### Comparing `django_formset-1.4.2/formset/static/formset/js/chunk-65OJRBX6.js` & `django_formset-1.4.3/formset/static/formset/js/chunk-65OJRBX6.js`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/static/formset/js/chunk-6IBLXZPA.js` & `django_formset-1.4.3/formset/static/formset/js/chunk-R3EYKSPB.js`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/static/formset/js/chunk-B7PX5YAU.js` & `django_formset-1.4.3/formset/static/formset/js/chunk-YMY5H5XX.js`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/static/formset/js/chunk-FDUUONAQ.js` & `django_formset-1.4.3/formset/static/formset/js/chunk-FDUUONAQ.js`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/static/formset/js/chunk-NOGHTXP6.js` & `django_formset-1.4.3/formset/static/formset/js/chunk-NOGHTXP6.js`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/static/formset/js/chunk-P2VM2T3G.js` & `django_formset-1.4.3/formset/static/formset/js/chunk-P2VM2T3G.js`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/static/formset/js/chunk-RLE6ONWJ.js` & `django_formset-1.4.3/formset/static/formset/js/chunk-RLE6ONWJ.js`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/static/formset/js/chunk-SERXULES.js` & `django_formset-1.4.3/formset/static/formset/js/chunk-SERXULES.js`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/static/formset/js/chunk-W5RPWA2M.js` & `django_formset-1.4.3/formset/static/formset/js/chunk-W5RPWA2M.js`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/static/formset/js/chunk-WKRSL2PQ.js` & `django_formset-1.4.3/formset/static/formset/js/chunk-TRJBB73N.js`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/static/formset/js/chunk-XO2BBJ6P.js` & `django_formset-1.4.3/formset/static/formset/js/chunk-IH7AT57W.js`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/static/formset/js/django-formset.js` & `django_formset-1.4.3/formset/static/formset/js/django-formset.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -7,26 +7,26 @@
 import {
     a as er,
     b as tr,
     c as rr,
     d as M,
     e as ot,
     f as lt
-} from "./chunk-B7PX5YAU.js";
+} from "./chunk-YMY5H5XX.js";
 import {
     a as it
 } from "./chunk-FDUUONAQ.js";
 import {
     a as st
 } from "./chunk-65OJRBX6.js";
 import {
     a as Zt,
     b as B
 } from "./chunk-P2VM2T3G.js";
-var At = Zt((ai, wt) => {
+var Tt = Zt((ai, wt) => {
     var ir = "Expected a function",
         ft = "__lodash_hash_undefined__",
         pt = 1 / 0,
         nr = 9007199254740991,
         sr = "[object Function]",
         or = "[object GeneratorFunction]",
         lr = "[object Symbol]",
@@ -36,15 +36,15 @@
         ur = /[^.[\]]+|\[(?:(-?\d+(?:\.\d+)?)|(["'])((?:(?!\2)[^\\]|\\.)*?)\2)\]|(?=(?:\.|\[\])(?:\.|\[\]|$))/g,
         hr = /[\\^$.*+?()[\]{}|]/g,
         fr = /\\(\\)?/g,
         pr = /^\[object .+?Constructor\]$/,
         mr = /^(?:0|[1-9]\d*)$/,
         gr = typeof global == "object" && global && global.Object === Object && global,
         br = typeof self == "object" && self && self.Object === Object && self,
-        Te = gr || br || Function("return this")();
+        Ae = gr || br || Function("return this")();
 
     function vr(n, e) {
         return n == null ? void 0 : n[e]
     }
 
     function yr(n) {
         var e = !1;
@@ -52,64 +52,64 @@
             e = !!(n + "")
         } catch {}
         return e
     }
     var Er = Array.prototype,
         wr = Function.prototype,
         mt = Object.prototype,
-        Ae = Te["__core-js_shared__"],
+        Te = Ae["__core-js_shared__"],
         ct = function() {
-            var n = /[^.]+$/.exec(Ae && Ae.keys && Ae.keys.IE_PROTO || "");
+            var n = /[^.]+$/.exec(Te && Te.keys && Te.keys.IE_PROTO || "");
             return n ? "Symbol(src)_1." + n : ""
         }(),
         gt = wr.toString,
         se = mt.hasOwnProperty,
         bt = mt.toString,
-        Ar = RegExp("^" + gt.call(se).replace(hr, "\\$&").replace(/hasOwnProperty|(function).*?(?=\\\()| for .+?(?=\\\])/g, "$1.*?") + "$"),
-        dt = Te.Symbol,
-        Tr = Er.splice,
-        Fr = vt(Te, "Map"),
-        K = vt(Object, "create"),
+        Tr = RegExp("^" + gt.call(se).replace(hr, "\\$&").replace(/hasOwnProperty|(function).*?(?=\\\()| for .+?(?=\\\])/g, "$1.*?") + "$"),
+        dt = Ae.Symbol,
+        Ar = Er.splice,
+        Fr = vt(Ae, "Map"),
+        X = vt(Object, "create"),
         ut = dt ? dt.prototype : void 0,
         ht = ut ? ut.toString : void 0;
 
     function I(n) {
         var e = -1,
             t = n ? n.length : 0;
         for (this.clear(); ++e < t;) {
             var r = n[e];
             this.set(r[0], r[1])
         }
     }
 
     function Cr() {
-        this.__data__ = K ? K(null) : {}
+        this.__data__ = X ? X(null) : {}
     }
 
     function jr(n) {
         return this.has(n) && delete this.__data__[n]
     }
 
     function xr(n) {
         var e = this.__data__;
-        if (K) {
+        if (X) {
             var t = e[n];
             return t === ft ? void 0 : t
         }
         return se.call(e, n) ? e[n] : void 0
     }
 
     function Lr(n) {
         var e = this.__data__;
-        return K ? e[n] !== void 0 : se.call(e, n)
+        return X ? e[n] !== void 0 : se.call(e, n)
     }
 
     function Sr(n, e) {
         var t = this.__data__;
-        return t[n] = K && e === void 0 ? ft : e, this
+        return t[n] = X && e === void 0 ? ft : e, this
     }
     I.prototype.clear = Cr;
     I.prototype.delete = jr;
     I.prototype.get = xr;
     I.prototype.has = Lr;
     I.prototype.set = Sr;
 
@@ -127,15 +127,15 @@
     }
 
     function Mr(n) {
         var e = this.__data__,
             t = oe(e, n);
         if (t < 0) return !1;
         var r = e.length - 1;
-        return t == r ? e.pop() : Tr.call(e, t, 1), !0
+        return t == r ? e.pop() : Ar.call(e, t, 1), !0
     }
 
     function Dr(n) {
         var e = this.__data__,
             t = oe(e, n);
         return t < 0 ? void 0 : e[t][1]
     }
@@ -201,43 +201,43 @@
     function oe(n, e) {
         for (var t = n.length; t--;)
             if (yt(n[t][0], e)) return t;
         return -1
     }
 
     function Vr(n) {
-        if (!ne(n) || Kr(n)) return !1;
-        var e = Yr(n) || yr(n) ? Ar : pr;
+        if (!ne(n) || Xr(n)) return !1;
+        var e = Yr(n) || yr(n) ? Tr : pr;
         return e.test(Qr(n))
     }
 
-    function $r(n, e, t, r) {
+    function Nr(n, e, t, r) {
         if (!ne(n)) return n;
         e = zr(e, n) ? [e] : Gr(e);
         for (var i = -1, s = e.length, o = s - 1, u = n; u != null && ++i < s;) {
-            var d = Jr(e[i]),
+            var d = Kr(e[i]),
                 c = t;
             if (i != o) {
                 var l = u[d];
                 c = r ? r(l, d, u) : void 0, c === void 0 && (c = ne(l) ? l : Ur(e[i + 1]) ? [] : {})
             }
             _r(u, d, c), u = u[d]
         }
         return n
     }
 
-    function Nr(n) {
+    function $r(n) {
         if (typeof n == "string") return n;
         if (Ce(n)) return ht ? ht.call(n) : "";
         var e = n + "";
         return e == "0" && 1 / n == -pt ? "-0" : e
     }
 
     function Gr(n) {
-        return Et(n) ? n : Xr(n)
+        return Et(n) ? n : Jr(n)
     }
 
     function le(n, e) {
         var t = n.__data__;
         return Wr(e) ? t[typeof e == "string" ? "string" : "hash"] : t.map
     }
 
@@ -257,26 +257,26 @@
     }
 
     function Wr(n) {
         var e = typeof n;
         return e == "string" || e == "number" || e == "symbol" || e == "boolean" ? n !== "__proto__" : n === null
     }
 
-    function Kr(n) {
+    function Xr(n) {
         return !!ct && ct in n
     }
-    var Xr = Fe(function(n) {
+    var Jr = Fe(function(n) {
         n = ei(n);
         var e = [];
         return dr.test(n) && e.push(""), n.replace(ur, function(t, r, i, s) {
             e.push(i ? s.replace(fr, "$1") : r || t)
         }), e
     });
 
-    function Jr(n) {
+    function Kr(n) {
         if (typeof n == "string" || Ce(n)) return n;
         var e = n + "";
         return e == "0" && 1 / n == -pt ? "-0" : e
     }
 
     function Qr(n) {
         if (n != null) {
@@ -324,19 +324,19 @@
     }
 
     function Ce(n) {
         return typeof n == "symbol" || Zr(n) && bt.call(n) == lr
     }
 
     function ei(n) {
-        return n == null ? "" : Nr(n)
+        return n == null ? "" : $r(n)
     }
 
     function ti(n, e, t) {
-        return n == null ? n : $r(n, e, t)
+        return n == null ? n : Nr(n, e, t)
     }
     wt.exports = ti
 });
 (function() {
     "use strict";
     var n = function(h, a) {
         var f = function(y) {
@@ -432,21 +432,21 @@
     var i = !0,
         s = !1,
         o = "querySelectorAll",
         u = function(a) {
             var f = arguments.length > 1 && arguments[1] !== void 0 ? arguments[1] : document,
                 p = arguments.length > 2 && arguments[2] !== void 0 ? arguments[2] : MutationObserver,
                 m = arguments.length > 3 && arguments[3] !== void 0 ? arguments[3] : ["*"],
-                y = function w(P, H, F, b, E, A) {
+                y = function w(P, H, F, b, E, T) {
                     var C = r(P),
                         q;
                     try {
                         for (C.s(); !(q = C.n()).done;) {
-                            var T = q.value;
-                            (A || o in T) && (E ? F.has(T) || (F.add(T), b.delete(T), a(T, E)) : b.has(T) || (b.add(T), F.delete(T), a(T, E)), A || w(T[o](H), H, F, b, E, i))
+                            var A = q.value;
+                            (T || o in A) && (E ? F.has(A) || (F.add(A), b.delete(A), a(A, E)) : b.has(A) || (b.add(A), F.delete(A), a(A, E)), T || w(A[o](H), H, F, b, E, i))
                         }
                     } catch (we) {
                         C.e(we)
                     } finally {
                         C.f()
                     }
                 },
@@ -455,21 +455,21 @@
                         var P = m.join(","),
                             H = new Set,
                             F = new Set,
                             b = r(w),
                             E;
                         try {
                             for (b.s(); !(E = b.n()).done;) {
-                                var A = E.value,
-                                    C = A.addedNodes,
-                                    q = A.removedNodes;
+                                var T = E.value,
+                                    C = T.addedNodes,
+                                    q = T.removedNodes;
                                 y(q, P, H, F, s, s), y(C, P, H, F, i, s)
                             }
-                        } catch (T) {
-                            b.e(T)
+                        } catch (A) {
+                            b.e(A)
                         } finally {
                             b.f()
                         }
                     }
                 }),
                 v = g.observe;
             return (g.observe = function(w) {
@@ -489,32 +489,32 @@
         He = function(a) {
             return d in a
         },
         Ie = [].filter,
         fe = function(h) {
             var a = new Dt,
                 f = function(b) {
-                    for (var E = 0, A = b.length; E < A; E++) a.delete(b[E])
+                    for (var E = 0, T = b.length; E < T; E++) a.delete(b[E])
                 },
                 p = function() {
-                    for (var b = P.takeRecords(), E = 0, A = b.length; E < A; E++) g(Ie.call(b[E].removedNodes, He), !1), g(Ie.call(b[E].addedNodes, He), !0)
+                    for (var b = P.takeRecords(), E = 0, T = b.length; E < T; E++) g(Ie.call(b[E].removedNodes, He), !1), g(Ie.call(b[E].addedNodes, He), !0)
                 },
                 m = function(b) {
                     return b.matches || b.webkitMatchesSelector || b.msMatchesSelector
                 },
                 y = function(b, E) {
-                    var A;
+                    var T;
                     if (E)
-                        for (var C, q = m(b), T = 0, we = v.length; T < we; T++) q.call(b, C = v[T]) && (a.has(b) || a.set(b, new Mt), A = a.get(b), A.has(C) || (A.add(C), h.handle(b, E, C)));
-                    else a.has(b) && (A = a.get(b), a.delete(b), A.forEach(function(Yt) {
+                        for (var C, q = m(b), A = 0, we = v.length; A < we; A++) q.call(b, C = v[A]) && (a.has(b) || a.set(b, new Mt), T = a.get(b), T.has(C) || (T.add(C), h.handle(b, E, C)));
+                    else a.has(b) && (T = a.get(b), a.delete(b), T.forEach(function(Yt) {
                         h.handle(b, E, Yt)
                     }))
                 },
                 g = function(b) {
-                    for (var E = arguments.length > 1 && arguments[1] !== void 0 ? arguments[1] : !0, A = 0, C = b.length; A < C; A++) y(b[A], E)
+                    for (var E = arguments.length > 1 && arguments[1] !== void 0 ? arguments[1] : !0, T = 0, C = b.length; T < C; T++) y(b[T], E)
                 },
                 v = h.query,
                 w = h.root || l,
                 P = u(y, w, G, v),
                 H = k.prototype.attachShadow;
             return H && (k.prototype.attachShadow = function(F) {
                 var b = H.call(this, F);
@@ -526,29 +526,29 @@
                 parse: g
             }
         },
         j = self,
         x = j.document,
         D = j.Map,
         Oe = j.MutationObserver,
-        X = j.Object,
+        J = j.Object,
         Re = j.Set,
         Pt = j.WeakMap,
         qe = j.Element,
         Ht = j.HTMLElement,
         Be = j.Node,
         _e = j.Error,
         Ve = j.TypeError,
         It = j.Reflect,
-        J = X.defineProperty,
-        Ot = X.keys,
-        Rt = X.getOwnPropertyNames,
-        U = X.setPrototypeOf,
+        K = J.defineProperty,
+        Ot = J.keys,
+        Rt = J.getOwnPropertyNames,
+        U = J.setPrototypeOf,
         z = !self.customElements,
-        $e = function(a) {
+        Ne = function(a) {
             for (var f = Ot(a), p = [], m = new Re, y = f.length, g = 0; g < y; g++) {
                 p[g] = a[f[g]];
                 try {
                     delete a[f[g]]
                 } catch {
                     m.add(g)
                 }
@@ -559,27 +559,27 @@
         };
     if (z) {
         var pe = function() {
                 var a = this.constructor;
                 if (!me.has(a)) throw new Ve("Illegal constructor");
                 var f = me.get(a);
                 if (Y) return ze(Y, f);
-                var p = Ne.call(x, f);
+                var p = $e.call(x, f);
                 return ze(U(p, a.prototype), f)
             },
-            Ne = x.createElement,
+            $e = x.createElement,
             me = new D,
             Q = new D,
             Ge = new D,
             W = new D,
             Ue = [],
             qt = function(a, f, p) {
                 var m = Ge.get(p);
                 if (f && !m.isPrototypeOf(a)) {
-                    var y = $e(a);
+                    var y = Ne(a);
                     Y = U(a, m);
                     try {
                         new m.constructor
                     } finally {
                         Y = null, y()
                     }
                 }
@@ -612,55 +612,55 @@
                     _t(x.querySelectorAll(a))
                 }), Q.get(a)._(f)
             },
             get: function(a) {
                 return W.get(a)
             },
             whenDefined: ge
-        }, J(pe.prototype = Ht.prototype, "constructor", {
+        }, K(pe.prototype = Ht.prototype, "constructor", {
             value: pe
         }), self.HTMLElement = pe, x.createElement = function(h, a) {
             var f = a && a.is,
                 p = f ? W.get(f) : W.get(h);
-            return p ? new p : Ne.call(x, h)
-        }, "isConnected" in Be.prototype || J(Be.prototype, "isConnected", {
+            return p ? new p : $e.call(x, h)
+        }, "isConnected" in Be.prototype || K(Be.prototype, "isConnected", {
             configurable: !0,
             get: function() {
                 return !(this.ownerDocument.compareDocumentPosition(this) & this.DOCUMENT_POSITION_DISCONNECTED)
             }
         })
     } else if (z = !self.customElements.get("extends-br"), z) try {
         var We = function h() {
             return self.Reflect.construct(HTMLBRElement, [], h)
         };
         We.prototype = HTMLLIElement.prototype;
-        var Ke = "extends-br";
+        var Xe = "extends-br";
         self.customElements.define("extends-br", We, {
             extends: "br"
         }), z = x.createElement("br", {
-            is: Ke
-        }).outerHTML.indexOf(Ke) < 0;
-        var Xe = self.customElements,
-            Vt = Xe.get,
-            $t = Xe.whenDefined;
+            is: Xe
+        }).outerHTML.indexOf(Xe) < 0;
+        var Je = self.customElements,
+            Vt = Je.get,
+            Nt = Je.whenDefined;
         self.customElements.whenDefined = function(h) {
             var a = this;
-            return $t.call(this, h).then(function(f) {
+            return Nt.call(this, h).then(function(f) {
                 return f || Vt.call(a, h)
             })
         }
     } catch {}
     if (z) {
-        var Je = function(a) {
+        var Ke = function(a) {
                 var f = be.get(a);
                 tt(f.querySelectorAll(this), a.isConnected)
             },
             L = self.customElements,
             Qe = x.createElement,
-            Nt = L.define,
+            $t = L.define,
             Gt = L.get,
             Ut = L.upgrade,
             zt = It || {
                 construct: function(a) {
                     return a.call(this)
                 }
             },
@@ -672,40 +672,40 @@
             Ye = new D,
             te = new D,
             Ze = [],
             re = [],
             et = function(a) {
                 return te.get(a) || Gt.call(L, a)
             },
-            Kt = function(a, f, p) {
+            Xt = function(a, f, p) {
                 var m = Ye.get(p);
                 if (f && !m.isPrototypeOf(a)) {
-                    var y = $e(a);
+                    var y = Ne(a);
                     ie = U(a, m);
                     try {
                         new m.constructor
                     } finally {
                         ie = null, y()
                     }
                 }
                 var g = "".concat(f ? "" : "dis", "connectedCallback");
                 g in m && a[g]()
             },
-            Xt = fe({
+            Jt = fe({
                 query: re,
-                handle: Kt
+                handle: Xt
             }),
-            tt = Xt.parse,
-            Jt = fe({
+            tt = Jt.parse,
+            Kt = fe({
                 query: Ze,
                 handle: function(a, f) {
-                    be.has(a) && (f ? ve.add(a) : ve.delete(a), re.length && Je.call(re, a))
+                    be.has(a) && (f ? ve.add(a) : ve.delete(a), re.length && Ke.call(re, a))
                 }
             }),
-            Qt = Jt.parse,
+            Qt = Kt.parse,
             rt = qe.prototype.attachShadow;
         rt && (qe.prototype.attachShadow = function(h) {
             var a = rt.call(this, h);
             return be.set(this, a), a
         });
         var ye = function(a) {
                 if (!ee.has(a)) {
@@ -734,17 +734,17 @@
                     g = m.tag;
                 if (y) {
                     if (ie) return Ee(ie, y);
                     var v = Qe.call(x, g);
                     return v.setAttribute("is", y), Ee(U(v, p.prototype), y)
                 } else return Wt.call(this, a, [], p)
             }
-            J(f.prototype = a.prototype, "constructor", {
+            K(f.prototype = a.prototype, "constructor", {
                 value: f
-            }), J(self, h, {
+            }), K(self, h, {
                 value: f
             })
         }), x.createElement = function(h, a) {
             var f = a && a.is;
             if (f) {
                 var p = te.get(f);
                 if (p && Z.get(p).tag === h) return new p
@@ -766,60 +766,74 @@
             var p, m = f && f.extends;
             Z.set(a, m ? {
                 is: h,
                 tag: m
             } : {
                 is: "",
                 tag: h
-            }), m ? (p = "".concat(m, '[is="').concat(h, '"]'), Ye.set(p, a.prototype), te.set(h, a), re.push(p)) : (Nt.apply(L, arguments), Ze.push(p = h)), ye(h).then(function() {
-                m ? (tt(x.querySelectorAll(p)), ve.forEach(Je, [p])) : Qt(x.querySelectorAll(p))
+            }), m ? (p = "".concat(m, '[is="').concat(h, '"]'), Ye.set(p, a.prototype), te.set(h, a), re.push(p)) : ($t.apply(L, arguments), Ze.push(p = h)), ye(h).then(function() {
+                m ? (tt(x.querySelectorAll(p)), ve.forEach(Ke, [p])) : Qt(x.querySelectorAll(p))
             }), ee.get(h)._(a)
         }
     }
 })();
-var $ = B(er()),
-    xt = B(At()),
+var N = B(er()),
+    xt = B(Tt()),
     Pe = B(tr()),
     Lt = B(rr()),
     St = B(it());
-var Tt = B(it()),
+var At = B(it()),
     ae = class {
         constructor(e, t) {
             this.progressBar = null;
             this.fileDrop = e => {
-                this.swallowEvent(e), e.dataTransfer && (this.fieldGroup.touch(), this.inputElement.files = e.dataTransfer.files, this.uploadFiles(this.inputElement.files).then(() => {
-                    this.fieldGroup.inputted(), this.fieldGroup.validate()
-                }))
+                if (this.swallowEvent(e), e.dataTransfer) {
+                    for (let t of e.dataTransfer.files)
+                        if (!this.matchesMimeType(t.type)) {
+                            e.dataTransfer.clearData(), this.fieldGroup.reportFailedUpload();
+                            return
+                        } this.fieldGroup.touch(), this.inputElement.files = e.dataTransfer.files, this.uploadFiles(this.inputElement.files).then(() => {
+                        this.fieldGroup.inputted(), this.fieldGroup.validate()
+                    })
+                }
             };
             this.fileRemove = () => {
                 for (this.inputElement.value = "", this.uploadedFiles = this.initialData.length > 0 ? [{}] : []; this.dropbox.firstChild;) this.dropbox.removeChild(this.dropbox.firstChild);
                 this.dropbox.appendChild(this.emptyDropboxItem), this.fieldGroup.touch(), this.fieldGroup.inputted(), this.fieldGroup.validate()
             };
             this.swallowEvent = e => {
                 e.stopPropagation(), e.preventDefault()
             };
             if (this.fieldGroup = e, this.inputElement = t, this.maxUploadSize = parseInt(this.inputElement.getAttribute("max-size") ?? "0"), this.dropbox = this.fieldGroup.element.querySelector("figure.dj-dropbox"), !this.dropbox) throw new Error('Element <input type="file"> requires sibling element <figure class="dj-dropbox"></figure>');
             if (this.chooseFileButton = this.fieldGroup.element.querySelector("button.dj-choose-file"), !this.chooseFileButton) throw new Error('Element <input type="file"> requires sibling element <button class="dj-choose-file"></button>');
             if (this.progressBar = this.fieldGroup.element.querySelector("progress"), this.progressBar && (this.progressBar.style.visibility = "hidden"), this.emptyDropboxItem = this.dropbox.querySelector("div.dj-empty-item"), !this.emptyDropboxItem) throw new Error('Element <input type="file"> requires sibling element <figure><div class="dj-empty-item"></div></figure>');
             let r = this.fieldGroup.element.querySelector(".dj-dropbox-items");
             if (!r) throw new Error('Element <input type="file"> requires sibling element <template class="dj-dropbox-items"></template>');
-            this.dropboxItemTemplate = (0, Tt.default)(r.innerHTML), this.observer = new MutationObserver(s => this.attributesChanged(s)), this.observer.observe(this.inputElement, {
+            this.dropboxItemTemplate = (0, At.default)(r.innerHTML), this.observer = new MutationObserver(s => this.attributesChanged(s)), this.observer.observe(this.inputElement, {
                 attributes: !0
             }), this.chooseFileButton.disabled = t.disabled;
             let i = document.getElementById(`initial_${t.id}`);
             i != null && i.textContent ? (this.uploadedFiles = this.initialData = [JSON.parse(i.textContent)], this.renderDropbox()) : this.uploadedFiles = this.initialData = [], this.dropbox.addEventListener("dragenter", this.swallowEvent), this.dropbox.addEventListener("dragover", this.swallowEvent), this.dropbox.addEventListener("drop", this.fileDrop), this.chooseFileButton.addEventListener("click", () => {
                 t.click()
             }), t.addEventListener("change", () => this.uploadFiles(this.inputElement.files).then(() => {
                 this.fieldGroup.inputted(), this.fieldGroup.validate()
             }).catch(() => {
                 this.fieldGroup.reportFailedUpload()
             }).finally(() => {
                 this.chooseFileButton.blur(), this.fieldGroup.touch()
             }))
         }
+        matchesMimeType(e) {
+            let t = this.inputElement.accept.split(",").map(s => s.trim());
+            if (t.length === 0) return !0;
+            let [r, i] = e.split("/");
+            for (let s of t)
+                if (s === e || i === "*" && s.split("/")[0] === r) return !0;
+            return !1
+        }
         async uploadFiles(e) {
             return !e || e.length === 0 ? Promise.reject() : new Promise((t, r) => {
                 let i = e.item(0);
                 i && (!this.maxUploadSize || i.size <= this.maxUploadSize) ? this.uploadFile(i, this.dropbox.clientHeight).then(s => {
                     this.uploadedFiles = [s], this.renderDropbox(), this.fieldGroup.inputted(), this.inputElement.dataset.fileupload = JSON.stringify(s), t()
                 }).catch(() => {
                     r()
@@ -841,17 +855,16 @@
                 let c = new XMLHttpRequest;
                 r.progressBar && (c.addEventListener("loadstart", i), c.upload.addEventListener("progress", i, !1)), c.addEventListener("loadend", d), c.open("POST", this.fieldGroup.form.formset.endpoint, !0);
                 let l = this.fieldGroup.form.formset.CSRFToken;
                 l && c.setRequestHeader("X-CSRFToken", l), c.responseType = "json", c.send(s)
             })
         }
         renderDropbox() {
-            let e = [];
-            for (let t of this.uploadedFiles) e.push(this.dropboxItemTemplate(t));
-            e.length > 0 ? this.dropbox.innerHTML = e.join("") : this.dropbox.replaceChildren(this.emptyDropboxItem)
+            let e = this.uploadedFiles.map(this.dropboxItemTemplate);
+            e.length > 0 ? (this.dropbox.innerHTML = e.join(""), this.inputElement.dataset.fileupload = JSON.stringify(this.uploadedFiles[0])) : this.dropbox.replaceChildren(this.emptyDropboxItem)
         }
         attributesChanged(e) {
             for (let t of e)
                 if (t.type === "attributes" && (t.attributeName === "disabled" && this.chooseFileButton.disabled != this.inputElement.disabled && (this.chooseFileButton.disabled = this.inputElement.disabled), t.attributeName === "data-fileupload")) {
                     let r = this.inputElement.dataset.fileupload;
                     if (r) {
                         this.dropbox.innerHTML = this.dropboxItemTemplate(JSON.parse(r));
@@ -1115,15 +1128,15 @@
         }
     },
     ce = class {
         constructor(e, t) {
             this.func = e, this.args = t
         }
     },
-    N = class {
+    $ = class {
         constructor(e, t) {
             this.successChain = e, this.rejectChain = t
         }
     },
     Le = class {
         constructor(e, t, r) {
             this.condition = e, this.fulfilled = t, this.otherwise = r
@@ -1293,32 +1306,32 @@
                         var l;
                         (l = r(o.rejectChain, c)) == null || l.finally(() => {
                             this.restore.apply(this)
                         })
                     })
                 },
                 s = o => {
-                    o.condition.call(this) ? o.fulfilled instanceof N ? i(o.fulfilled) : s(o.fulfilled) : o.otherwise instanceof N ? i(o.otherwise) : s(o.otherwise)
+                    o.condition.call(this) ? o.fulfilled instanceof $ ? i(o.fulfilled) : s(o.fulfilled) : o.otherwise instanceof $ ? i(o.otherwise) : s(o.otherwise)
                 };
             this.clickHandler = () => {
-                e instanceof N ? i(e) : s(e)
+                e instanceof $ ? i(e) : s(e)
             }
         }
         parseActionsQueue(e) {
             if (!e) return;
             let t = i => {
                     let s = new Array;
                     for (let o of i) {
                         let u = this[o.funcname];
                         if (typeof u != "function") throw new Error(`Unknown function '${o.funcname}'.`);
                         s.push(new ce(u, o.args))
                     }
                     return s.length === 0 && s.push(new ce(this.noop, [])), s
                 },
-                r = i => i.condition === !0 ? new N(t(i.fulfilled.successChain), t(i.fulfilled.rejectChain)) : new Le(Function(i.condition), r(i.fulfilled), r(i.otherwise));
+                r = i => i.condition === !0 ? new $(t(i.fulfilled.successChain), t(i.fulfilled.rejectChain)) : new Le(Function(i.condition), r(i.fulfilled), r(i.otherwise));
             try {
                 let i = M(e, {
                         startRule: "Ternary"
                     }),
                     s = r(i);
                 this.setClickHandler(s)
             } catch (i) {
@@ -1894,28 +1907,28 @@
                     if (!Array.isArray(u)) throw new Error("Invalid form structure: Inner array is missing.");
                     r(u, o.slice(1)), s[o[0]] = u
                 }
             }
             let i = {};
             for (let s of this.emptyCollectionPrefixes) {
                 let o = ["formset_data", ...s.split(".")];
-                t = (0, $.default)(i, o), r(i, o)
+                t = (0, N.default)(i, o), r(i, o)
             }
             for (let s of this.forms) {
                 if (!s.name) {
                     let u = Object.fromEntries(s.aggregateValues());
                     return Object.assign({}, {
                         formset_data: u
                     }, {
                         _extra: e
                     })
                 }
                 if (s.isTransient) continue;
                 let o = s.getAbsPath();
-                t = (0, $.default)(this.data, o), s.markedForRemoval && (t[li] = !0), r(i, o)
+                t = (0, N.default)(this.data, o), s.markedForRemoval && (t[li] = !0), r(i, o)
             }
             return Object.assign({}, i, {
                 _extra: e
             })
         }
         async submit(e) {
             let t = !0;
@@ -1953,21 +1966,21 @@
                 this.clearErrors();
                 for (let r of this.forms) r.reportValidity()
             }
         }
         reportErrors(e) {
             console.info("Response from server:", e);
             for (let t of this.forms) {
-                let r = t.name ? (0, $.default)(e, t.name.split("."), null) : e;
+                let r = t.name ? (0, N.default)(e, t.name.split("."), null) : e;
                 (0, Lt.default)(r) ? t.clearCustomErrors(): (t.reportCustomErrors(new Map(Object.entries(r))), t.reportValidity())
             }
             for (let [t, r] of this.collectionErrorsList) {
                 let i = t ? t.split(".") : [];
                 i = [...i, "0", oi];
-                for (let s of (0, $.default)(e, i, [])) {
+                for (let s of (0, N.default)(e, i, [])) {
                     let o = document.createElement("li");
                     o.classList.add("dj-placeholder"), o.innerText = s, r.appendChild(o)
                 }
             }
         }
         resetToInitial() {
             var e;
@@ -1978,15 +1991,15 @@
             this.abortController.abort()
         }
         setSubmitted() {
             for (let e of this.forms) e.setSubmitted()
         }
         getDataValue(e) {
             let t = ["formset_data", ...e];
-            return (0, $.default)(this.data, t, null)
+            return (0, N.default)(this.data, t, null)
         }
         findFirstErrorReport() {
             for (let e of this.forms) {
                 let t = e.findFirstErrorReport();
                 if (t) return t
             }
             return null
@@ -2025,65 +2038,65 @@
 
     function r(o, u, d, c = void 0) {
         customElements.get(u) instanceof Function ? o() : (window.customElements.define(u, d, c), window.customElements.whenDefined(u).then(() => o()))
     }
 
     function i(o) {
         o.querySelector('select[is="django-selectize"]') && t.push(new Promise((d, c) => {
-            import("./DjangoSelectize-XUOHPSUG.js").then(({
+            import("./DjangoSelectize-FCAZIQIK.js").then(({
                 DjangoSelectizeElement: l
             }) => {
                 r(d, "django-selectize", l, {
                     extends: "select"
                 })
             }).catch(l => c(l))
         })), o.querySelector('select[is="django-country-selectize"]') && t.push(new Promise((d, c) => {
-            import("./CountrySelectize-RPAYKZSN.js").then(({
+            import("./CountrySelectize-SV3ETVIG.js").then(({
                 CountrySelectizeElement: l
             }) => {
                 r(d, "django-country-selectize", l, {
                     extends: "select"
                 })
             }).catch(l => c(l))
         })), o.querySelector("django-sortable-select") ? t.push(new Promise((d, c) => {
-            import("./SortableSelect-6YQLVCNF.js").then(({
+            import("./SortableSelect-3ABJOEP2.js").then(({
                 SortableSelectElement: l
             }) => {
-                customElements.get("django-sortable-select") instanceof Function ? d() : window.customElements.define("django-sortable-select", l), import("./DualSelector-G47GXWWH.js").then(({
+                customElements.get("django-sortable-select") instanceof Function ? d() : window.customElements.define("django-sortable-select", l), import("./DualSelector-TFBRBEV6.js").then(({
                     DualSelectorElement: k
                 }) => {
                     customElements.get("django-dual-selector") instanceof Function ? d() : (window.customElements.define("django-dual-selector", k, {
                         extends: "select"
                     }), Promise.all([window.customElements.whenDefined("django-sortable-select"), window.customElements.whenDefined("django-dual-selector")]).then(() => d()))
                 }).catch(k => c(k))
             }).catch(l => c(l))
         })) : o.querySelector('select[is="django-dual-selector"]') && t.push(new Promise((d, c) => {
-            import("./DualSelector-G47GXWWH.js").then(({
+            import("./DualSelector-TFBRBEV6.js").then(({
                 DualSelectorElement: l
             }) => {
                 r(d, "django-dual-selector", l, {
                     extends: "select"
                 })
             }).catch(l => c(l))
         })), o.querySelector('input[is="django-phone-number"]') && t.push(new Promise((d, c) => {
-            import("./PhoneNumber-RCXY4VXK.js").then(({
+            import("./PhoneNumber-XY2VHR24.js").then(({
                 PhoneNumberElement: l
             }) => {
                 r(d, "django-phone-number", l, {
                     extends: "input"
                 })
             }).catch(l => c(l))
         })), o.querySelectorAll('textarea[is="django-richtext"]').forEach(d => {
             t.push(new Promise((c, l) => {
                 let k = () => {
                     d.isInitialized ? c() : d.addEventListener("connected", () => c(), {
                         once: !0
                     })
                 };
-                import("./RichtextArea-34WSI64S.js").then(({
+                import("./RichtextArea-PVV6GJIQ.js").then(({
                     RichTextAreaElement: G
                 }) => {
                     customElements.get("django-richtext") instanceof Function ? k() : (window.customElements.define("django-richtext", G, {
                         extends: "textarea"
                     }), window.customElements.whenDefined("django-richtext").then(k))
                 }).catch(G => l(G))
             }))
@@ -2092,103 +2105,103 @@
                 DjangoSlugElement: l
             }) => {
                 r(d, "django-slug", l, {
                     extends: "input"
                 })
             }).catch(l => c(l))
         })), o.querySelector('input[is="django-datefield"]') && t.push(new Promise((d, c) => {
-            import("./DateTime-WW4TXK6Y.js").then(({
+            import("./DateTime-7RV5MOXB.js").then(({
                 DateFieldElement: l
             }) => {
                 r(d, "django-datefield", l, {
                     extends: "input"
                 })
             }).catch(l => c(l))
         })), o.querySelector('input[is="django-datecalendar"]') && t.push(new Promise((d, c) => {
-            import("./Calendar-5KXZG25G.js").then(({
+            import("./Calendar-6GWQDXEH.js").then(({
                 DateCalendarElement: l
             }) => {
                 r(d, "django-datecalendar", l, {
                     extends: "input"
                 })
             }).catch(l => c(l))
         })), o.querySelector('input[is="django-datepicker"]') && t.push(new Promise((d, c) => {
-            import("./DateTime-WW4TXK6Y.js").then(({
+            import("./DateTime-7RV5MOXB.js").then(({
                 DatePickerElement: l
             }) => {
                 r(d, "django-datepicker", l, {
                     extends: "input"
                 })
             }).catch(l => c(l))
         })), o.querySelector('input[is="django-datetimefield"]') && t.push(new Promise((d, c) => {
-            import("./DateTime-WW4TXK6Y.js").then(({
+            import("./DateTime-7RV5MOXB.js").then(({
                 DateTimeFieldElement: l
             }) => {
                 r(d, "django-datetimefield", l, {
                     extends: "input"
                 })
             }).catch(l => c(l))
         })), o.querySelector('input[is="django-datetimecalendar"]') && t.push(new Promise((d, c) => {
-            import("./Calendar-5KXZG25G.js").then(({
+            import("./Calendar-6GWQDXEH.js").then(({
                 DateCalendarElement: l
             }) => {
                 r(d, "django-datetimecalendar", l, {
                     extends: "input"
                 })
             }).catch(l => c(l))
         })), o.querySelector('input[is="django-datetimepicker"]') && t.push(new Promise((d, c) => {
-            import("./DateTime-WW4TXK6Y.js").then(({
+            import("./DateTime-7RV5MOXB.js").then(({
                 DateTimePickerElement: l
             }) => {
                 r(d, "django-datetimepicker", l, {
                     extends: "input"
                 })
             }).catch(l => c(l))
         })), o.querySelector('input[is="django-daterangefield"]') && t.push(new Promise((d, c) => {
-            import("./DateTime-WW4TXK6Y.js").then(({
+            import("./DateTime-7RV5MOXB.js").then(({
                 DateRangeFieldElement: l
             }) => {
                 r(d, "django-daterangefield", l, {
                     extends: "input"
                 })
             }).catch(l => c(l))
         })), o.querySelector('input[is="django-daterangecalendar"]') && t.push(new Promise((d, c) => {
-            import("./Calendar-5KXZG25G.js").then(({
+            import("./Calendar-6GWQDXEH.js").then(({
                 DateCalendarElement: l
             }) => {
                 r(d, "django-daterangecalendar", l, {
                     extends: "input"
                 })
             }).catch(l => c(l))
         })), o.querySelector('input[is="django-daterangepicker"]') && t.push(new Promise((d, c) => {
-            import("./DateTime-WW4TXK6Y.js").then(({
+            import("./DateTime-7RV5MOXB.js").then(({
                 DateRangePickerElement: l
             }) => {
                 r(d, "django-daterangepicker", l, {
                     extends: "input"
                 })
             }).catch(l => c(l))
         })), o.querySelector('input[is="django-datetimerangefield"]') && t.push(new Promise((d, c) => {
-            import("./DateTime-WW4TXK6Y.js").then(({
+            import("./DateTime-7RV5MOXB.js").then(({
                 DateTimeRangeFieldElement: l
             }) => {
                 r(d, "django-datetimerangefield", l, {
                     extends: "input"
                 })
             }).catch(l => c(l))
         })), o.querySelector('input[is="django-datetimerangecalendar"]') && t.push(new Promise((d, c) => {
-            import("./Calendar-5KXZG25G.js").then(({
+            import("./Calendar-6GWQDXEH.js").then(({
                 DateCalendarElement: l
             }) => {
                 r(d, "django-datetimerangecalendar", l, {
                     extends: "input"
                 })
             }).catch(l => c(l))
         })), o.querySelector('input[is="django-datetimerangepicker"]') && t.push(new Promise((d, c) => {
-            import("./DateTime-WW4TXK6Y.js").then(({
+            import("./DateTime-7RV5MOXB.js").then(({
                 DateTimeRangePickerElement: l
             }) => {
                 r(d, "django-datetimerangepicker", l, {
                     extends: "input"
                 })
             }).catch(l => c(l))
         }))
```

### Comparing `django_formset-1.4.2/formset/static/formset/tiptap-extensions/footnote.js` & `django_formset-1.4.3/formset/static/formset/tiptap-extensions/footnote.js`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/templates/calendar/hours.html` & `django_formset-1.4.3/formset/templates/calendar/hours.html`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/templates/calendar/months.html` & `django_formset-1.4.3/formset/templates/calendar/months.html`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/templates/calendar/weeks.html` & `django_formset-1.4.3/formset/templates/calendar/weeks.html`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/templates/calendar/years.html` & `django_formset-1.4.3/formset/templates/calendar/years.html`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/templates/formset/bootstrap/widgets/dual_selector.html` & `django_formset-1.4.3/formset/templates/formset/bootstrap/widgets/dual_selector.html`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/templates/formset/bootstrap/widgets/file.html` & `django_formset-1.4.3/formset/templates/formset/bootstrap/widgets/file.html`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/templates/formset/bulma/widgets/dual_selector.html` & `django_formset-1.4.3/formset/templates/formset/bulma/widgets/dual_selector.html`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/templates/formset/bulma/widgets/file.html` & `django_formset-1.4.3/formset/templates/formset/bulma/widgets/file.html`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/templates/formset/default/collection.html` & `django_formset-1.4.3/formset/templates/formset/default/collection.html`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/templates/formset/default/fieldset.html` & `django_formset-1.4.3/formset/templates/formset/default/fieldset.html`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/templates/formset/default/form_dialog.html` & `django_formset-1.4.3/formset/templates/formset/default/form_dialog.html`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/templates/formset/default/widgets/dual_selector.html` & `django_formset-1.4.3/formset/templates/formset/default/widgets/dual_selector.html`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/templates/formset/default/widgets/file.html` & `django_formset-1.4.3/formset/templates/formset/default/widgets/file.html`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/templates/formset/default/widgets/selectize.html` & `django_formset-1.4.3/formset/templates/formset/default/widgets/selectize.html`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/templates/formset/foundation/widgets/dual_selector.html` & `django_formset-1.4.3/formset/templates/formset/foundation/widgets/dual_selector.html`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/templates/formset/foundation/widgets/file.html` & `django_formset-1.4.3/formset/templates/formset/foundation/widgets/file.html`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/templates/formset/icons/blockquote.svg` & `django_formset-1.4.3/formset/templates/formset/icons/blockquote.svg`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/templates/formset/icons/calendar-today.svg` & `django_formset-1.4.3/formset/templates/formset/icons/calendar-today.svg`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/templates/formset/icons/footnote.svg` & `django_formset-1.4.3/formset/templates/formset/icons/footnote.svg`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/templates/formset/icons/letters.svg` & `django_formset-1.4.3/formset/templates/formset/icons/letters.svg`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/templates/formset/icons/placeholder.svg` & `django_formset-1.4.3/formset/templates/formset/icons/placeholder.svg`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/templates/formset/icons/questionmark.svg` & `django_formset-1.4.3/formset/templates/formset/icons/questionmark.svg`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/templates/formset/icons/strike.svg` & `django_formset-1.4.3/formset/templates/formset/icons/strike.svg`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/templates/formset/icons/subscript.svg` & `django_formset-1.4.3/formset/templates/formset/icons/subscript.svg`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/templates/formset/icons/unlink.svg` & `django_formset-1.4.3/formset/templates/formset/icons/unlink.svg`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/templates/formset/richtext/align.html` & `django_formset-1.4.3/formset/templates/formset/richtext/align.html`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/templates/formset/richtext/color.html` & `django_formset-1.4.3/formset/templates/formset/richtext/color.html`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/templates/formset/richtext/heading.html` & `django_formset-1.4.3/formset/templates/formset/richtext/heading.html`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/templates/formset/tailwind/widgets/dual_selector.html` & `django_formset-1.4.3/formset/templates/formset/tailwind/widgets/dual_selector.html`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/templates/formset/tailwind/widgets/file.html` & `django_formset-1.4.3/formset/templates/formset/tailwind/widgets/file.html`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/templates/formset/uikit/widgets/file.html` & `django_formset-1.4.3/formset/templates/formset/uikit/widgets/file.html`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/templatetags/formsetify.py` & `django_formset-1.4.3/formset/templatetags/formsetify.py`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/templatetags/phonenumber.py` & `django_formset-1.4.3/formset/templatetags/phonenumber.py`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/templatetags/richtext.py` & `django_formset-1.4.3/formset/templatetags/richtext.py`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/upload.py` & `django_formset-1.4.3/formset/upload.py`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/utils.py` & `django_formset-1.4.3/formset/utils.py`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/views.py` & `django_formset-1.4.3/formset/views.py`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.2/formset/widgets.py` & `django_formset-1.4.3/formset/widgets.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 
 from django.core.exceptions import ImproperlyConfigured, ObjectDoesNotExist
 from django.core.files.storage import default_storage
 from django.core.files.uploadedfile import UploadedFile
 from django.core.signing import get_cookie_signer
 from django.db.models.query_utils import Q
 from django.forms.models import ModelChoiceIterator, ModelChoiceIteratorValue
-from django.forms.widgets import DateTimeBaseInput, FileInput, Select, SelectMultiple, TextInput, Widget
+from django.forms.widgets import (FILE_INPUT_CONTRADICTION, DateTimeBaseInput, FileInput, Select, SelectMultiple,
+                                  TextInput, Widget)
 from django.template.loader import get_template
 from django.utils.encoding import uri_to_iri
 from django.utils.functional import cached_property
 from django.utils.timezone import datetime, now
 from django.utils.translation import gettext_lazy as _
 
 from formset.calendar import CalendarRenderer
@@ -367,16 +368,32 @@
             return handle
         if hasattr(handle, '__iter__'):
             handle = next(iter(handle), None)
         if isinstance(handle, dict):
             if not handle:
                 return False  # marked as deleted
             if 'upload_temp_name' not in handle:
-                return
-            # file has just been uploaded
+                return  # widget already initialized, skip checks
+
+            # check if the file type corresponds to the allowed types
+            if accept := self.attrs.get('accept'):
+                main_type, sub_type = handle['content_type'].split('/')
+                try:
+                    accepted = [a.strip().split('/') for a in accept.split(',')]
+                    for acc_main, acc_sub in accepted:
+                        if acc_main == '*' or acc_main == main_type and acc_sub in ['*', sub_type]:
+                            break
+                    else:
+                        # apparently the user has tampered with the content type and bypassed the browser check
+                        # hence prevent the temporarily uploaded file from being moved to its final destination
+                        return FILE_INPUT_CONTRADICTION
+                except ValueError:
+                    pass
+
+            # check if the uploaded file has been signed by the server
             signer = get_cookie_signer(salt='formset')
             upload_temp_name = signer.unsign(handle['upload_temp_name'])
             file = default_storage.open(upload_temp_name, 'rb')
             file.seek(0, os.SEEK_END)
             size = file.tell()
             file.seek(0)
             # create pseudo unique prefix to avoid file name collisions
```

### Comparing `django_formset-1.4.2/setup.py` & `django_formset-1.4.3/setup.py`

 * *Files identical despite different names*

