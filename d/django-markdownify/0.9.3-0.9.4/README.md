# Comparing `tmp/django-markdownify-0.9.3.tar.gz` & `tmp/django_markdownify-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-markdownify-0.9.3.tar", last modified: Thu Mar 16 16:06:13 2023, max compression
+gzip compressed data, was "django_markdownify-0.9.4.tar", last modified: Wed May  8 07:28:48 2024, max compression
```

## Comparing `django-markdownify-0.9.3.tar` & `django_markdownify-0.9.4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 erwin     (1000) erwin     (1000)        0 2023-03-16 16:06:13.292749 django-markdownify-0.9.3/
--rwxrwxrwx   0 erwin     (1000) erwin     (1000)     1080 2020-10-02 20:03:12.000000 django-markdownify-0.9.3/LICENSE
--rwxrwxrwx   0 erwin     (1000) erwin     (1000)       60 2020-10-02 20:03:12.000000 django-markdownify-0.9.3/MANIFEST.in
--rw-rw-r--   0 erwin     (1000) erwin     (1000)     2301 2023-03-16 16:06:13.288749 django-markdownify-0.9.3/PKG-INFO
--rw-rw-r--   0 erwin     (1000) erwin     (1000)     1730 2021-03-24 08:08:29.000000 django-markdownify-0.9.3/README.md
-drwxrwxr-x   0 erwin     (1000) erwin     (1000)        0 2023-03-16 16:06:13.288749 django-markdownify-0.9.3/django_markdownify.egg-info/
--rw-rw-r--   0 erwin     (1000) erwin     (1000)     2301 2023-03-16 16:06:13.000000 django-markdownify-0.9.3/django_markdownify.egg-info/PKG-INFO
--rw-rw-r--   0 erwin     (1000) erwin     (1000)      717 2023-03-16 16:06:13.000000 django-markdownify-0.9.3/django_markdownify.egg-info/SOURCES.txt
--rw-rw-r--   0 erwin     (1000) erwin     (1000)        1 2023-03-16 16:06:13.000000 django-markdownify-0.9.3/django_markdownify.egg-info/dependency_links.txt
--rw-rw-r--   0 erwin     (1000) erwin     (1000)       35 2023-03-16 16:06:13.000000 django-markdownify-0.9.3/django_markdownify.egg-info/requires.txt
--rw-rw-r--   0 erwin     (1000) erwin     (1000)       12 2023-03-16 16:06:13.000000 django-markdownify-0.9.3/django_markdownify.egg-info/top_level.txt
-drwxrwxr-x   0 erwin     (1000) erwin     (1000)        0 2023-03-16 16:06:13.288749 django-markdownify-0.9.3/markdownify/
--rwxrwxrwx   0 erwin     (1000) erwin     (1000)        0 2020-10-02 20:03:12.000000 django-markdownify-0.9.3/markdownify/__init__.py
--rw-rw-r--   0 erwin     (1000) erwin     (1000)      153 2021-03-02 21:09:08.000000 django-markdownify-0.9.3/markdownify/apps.py
--rw-rw-r--   0 erwin     (1000) erwin     (1000)      860 2021-03-24 08:08:26.000000 django-markdownify-0.9.3/markdownify/checks.py
-drwxrwxr-x   0 erwin     (1000) erwin     (1000)        0 2023-03-16 16:06:13.288749 django-markdownify-0.9.3/markdownify/templatetags/
--rwxrwxrwx   0 erwin     (1000) erwin     (1000)        0 2020-10-02 20:03:12.000000 django-markdownify-0.9.3/markdownify/templatetags/__init__.py
--rw-rw-r--   0 erwin     (1000) erwin     (1000)     4647 2023-03-16 16:01:43.000000 django-markdownify-0.9.3/markdownify/templatetags/markdownify.py
-drwxrwxr-x   0 erwin     (1000) erwin     (1000)        0 2023-03-16 16:06:13.288749 django-markdownify-0.9.3/markdownify/tests/
--rwxrwxrwx   0 erwin     (1000) erwin     (1000)        0 2021-01-14 16:04:00.000000 django-markdownify-0.9.3/markdownify/tests/__init__.py
--rw-rw-r--   0 erwin     (1000) erwin     (1000)       31 2021-03-02 21:09:08.000000 django-markdownify-0.9.3/markdownify/tests/input_text_alternative.md
--rwxrwxrwx   0 erwin     (1000) erwin     (1000)      174 2021-03-02 20:47:03.000000 django-markdownify-0.9.3/markdownify/tests/input_text_bleach.md
--rw-rw-r--   0 erwin     (1000) erwin     (1000)      732 2022-06-13 17:13:57.000000 django-markdownify-0.9.3/markdownify/tests/input_text_default.md
--rwxrwxrwx   0 erwin     (1000) erwin     (1000)       93 2021-03-02 20:48:18.000000 django-markdownify-0.9.3/markdownify/tests/input_text_extensions.md
--rwxrwxrwx   0 erwin     (1000) erwin     (1000)       90 2021-03-02 20:48:22.000000 django-markdownify-0.9.3/markdownify/tests/input_text_linkify.md
--rwxrwxrwx   0 erwin     (1000) erwin     (1000)       72 2021-03-02 20:48:25.000000 django-markdownify-0.9.3/markdownify/tests/input_text_strip.md
--rw-rw-r--   0 erwin     (1000) erwin     (1000)    24095 2023-03-16 16:01:43.000000 django-markdownify-0.9.3/markdownify/tests/test_markdownify.py
--rw-rw-r--   0 erwin     (1000) erwin     (1000)       84 2022-04-15 06:22:01.000000 django-markdownify-0.9.3/pyproject.toml
--rw-rw-r--   0 erwin     (1000) erwin     (1000)       38 2023-03-16 16:06:13.292749 django-markdownify-0.9.3/setup.cfg
--rw-rw-r--   0 erwin     (1000) erwin     (1000)     1138 2023-03-16 16:01:43.000000 django-markdownify-0.9.3/setup.py
+drwxrwxr-x   0 erwin     (1000) erwin     (1000)        0 2024-05-08 07:28:48.648609 django_markdownify-0.9.4/
+-rwxrwxrwx   0 erwin     (1000) erwin     (1000)     1080 2020-10-02 20:03:12.000000 django_markdownify-0.9.4/LICENSE
+-rwxrwxrwx   0 erwin     (1000) erwin     (1000)       60 2020-10-02 20:03:12.000000 django_markdownify-0.9.4/MANIFEST.in
+-rw-r--r--   0 erwin     (1000) erwin     (1000)     3034 2024-05-08 07:28:48.648609 django_markdownify-0.9.4/PKG-INFO
+-rw-rw-r--   0 erwin     (1000) erwin     (1000)     2383 2024-05-08 07:24:44.000000 django_markdownify-0.9.4/README.md
+drwxrwxr-x   0 erwin     (1000) erwin     (1000)        0 2024-05-08 07:28:48.648609 django_markdownify-0.9.4/django_markdownify.egg-info/
+-rw-r--r--   0 erwin     (1000) erwin     (1000)     3034 2024-05-08 07:28:48.000000 django_markdownify-0.9.4/django_markdownify.egg-info/PKG-INFO
+-rw-rw-r--   0 erwin     (1000) erwin     (1000)      717 2024-05-08 07:28:48.000000 django_markdownify-0.9.4/django_markdownify.egg-info/SOURCES.txt
+-rw-rw-r--   0 erwin     (1000) erwin     (1000)        1 2024-05-08 07:28:48.000000 django_markdownify-0.9.4/django_markdownify.egg-info/dependency_links.txt
+-rw-rw-r--   0 erwin     (1000) erwin     (1000)       35 2024-05-08 07:28:48.000000 django_markdownify-0.9.4/django_markdownify.egg-info/requires.txt
+-rw-rw-r--   0 erwin     (1000) erwin     (1000)       12 2024-05-08 07:28:48.000000 django_markdownify-0.9.4/django_markdownify.egg-info/top_level.txt
+drwxrwxr-x   0 erwin     (1000) erwin     (1000)        0 2024-05-08 07:28:48.648609 django_markdownify-0.9.4/markdownify/
+-rw-rw-r--   0 erwin     (1000) erwin     (1000)        0 2023-03-20 14:40:26.000000 django_markdownify-0.9.4/markdownify/__init__.py
+-rw-rw-r--   0 erwin     (1000) erwin     (1000)      153 2023-03-20 14:40:26.000000 django_markdownify-0.9.4/markdownify/apps.py
+-rw-rw-r--   0 erwin     (1000) erwin     (1000)      860 2023-03-20 14:40:26.000000 django_markdownify-0.9.4/markdownify/checks.py
+drwxrwxr-x   0 erwin     (1000) erwin     (1000)        0 2024-05-08 07:28:48.648609 django_markdownify-0.9.4/markdownify/templatetags/
+-rw-rw-r--   0 erwin     (1000) erwin     (1000)        0 2023-03-20 14:40:26.000000 django_markdownify-0.9.4/markdownify/templatetags/__init__.py
+-rw-rw-r--   0 erwin     (1000) erwin     (1000)     3477 2024-05-08 07:24:29.000000 django_markdownify-0.9.4/markdownify/templatetags/markdownify.py
+drwxrwxr-x   0 erwin     (1000) erwin     (1000)        0 2024-05-08 07:28:48.648609 django_markdownify-0.9.4/markdownify/tests/
+-rw-rw-r--   0 erwin     (1000) erwin     (1000)        0 2023-03-20 14:40:26.000000 django_markdownify-0.9.4/markdownify/tests/__init__.py
+-rw-rw-r--   0 erwin     (1000) erwin     (1000)       31 2023-03-20 14:40:26.000000 django_markdownify-0.9.4/markdownify/tests/input_text_alternative.md
+-rw-rw-r--   0 erwin     (1000) erwin     (1000)      174 2023-03-20 14:40:26.000000 django_markdownify-0.9.4/markdownify/tests/input_text_bleach.md
+-rw-rw-r--   0 erwin     (1000) erwin     (1000)      732 2023-03-20 14:40:26.000000 django_markdownify-0.9.4/markdownify/tests/input_text_default.md
+-rw-rw-r--   0 erwin     (1000) erwin     (1000)       93 2023-03-20 14:40:26.000000 django_markdownify-0.9.4/markdownify/tests/input_text_extensions.md
+-rw-rw-r--   0 erwin     (1000) erwin     (1000)       90 2023-03-20 14:40:26.000000 django_markdownify-0.9.4/markdownify/tests/input_text_linkify.md
+-rw-rw-r--   0 erwin     (1000) erwin     (1000)       72 2023-03-20 14:40:26.000000 django_markdownify-0.9.4/markdownify/tests/input_text_strip.md
+-rw-rw-r--   0 erwin     (1000) erwin     (1000)    13273 2024-05-08 07:24:29.000000 django_markdownify-0.9.4/markdownify/tests/test_markdownify.py
+-rw-rw-r--   0 erwin     (1000) erwin     (1000)       84 2022-04-15 06:22:01.000000 django_markdownify-0.9.4/pyproject.toml
+-rw-rw-r--   0 erwin     (1000) erwin     (1000)       38 2024-05-08 07:28:48.648609 django_markdownify-0.9.4/setup.cfg
+-rw-rw-r--   0 erwin     (1000) erwin     (1000)     1138 2024-05-08 07:24:29.000000 django_markdownify-0.9.4/setup.py
```

### Comparing `django-markdownify-0.9.3/LICENSE` & `django_markdownify-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `django-markdownify-0.9.3/PKG-INFO` & `django_markdownify-0.9.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,40 @@
 Metadata-Version: 2.1
 Name: django-markdownify
-Version: 0.9.3
+Version: 0.9.4
 Summary: Markdown template filter for Django.
 Home-page: https://github.com/erwinmatijsen/django-markdownify
-Download-URL: https://github.com/erwinmatijsen/django-markdownify/archive/0.9.3.tar.gz
+Download-URL: https://github.com/erwinmatijsen/django-markdownify/archive/0.9.4.tar.gz
 Author: Erwin Matijsen, R Moelker
 Author-email: erwin@erwinmatijsen.nl
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: Django
+Requires-Dist: markdown
+Requires-Dist: bleach[css]>=5.0.0
 
 # Django Markdownify - A Django Markdown filter
 
+![PyPi Downloads](https://img.shields.io/pypi/dm/django-markdownify) 
+![License](https://img.shields.io/pypi/l/django-markdownify?color=brightgreen)
+[![Documentation Status](https://readthedocs.org/projects/django-markdownify/badge/?version=latest)](https://django-markdownify.readthedocs.io/en/latest/?badge=latest)
+![Version](https://img.shields.io/pypi/v/django-markdownify)
+
 Django Markdownify is a template filter to convert Markdown to HTML in Django. Markdown is converted to HTML and sanitized.
 
 Read the full documentation on [Read the docs](http://django-markdownify.readthedocs.io/en/latest/) or check out the package on [pypi](https://pypi.python.org/pypi/django-markdownify).
 
+> [!WARNING]  
+> The [old settings](https://django-markdownify.readthedocs.io/en/latest/settings-old.html#oldsettings) are removed in release 0.9.4! Please update to the [new settings](https://django-markdownify.readthedocs.io/en/latest/settings.html) as soon as possible.
+
 ## Usage
 
 Load the tag inside your template:
 
 ```
 {% load markdownify %}
 ```
```

#### html2text {}

```diff
@@ -1,23 +1,33 @@
-Metadata-Version: 2.1 Name: django-markdownify Version: 0.9.3 Summary: Markdown
+Metadata-Version: 2.1 Name: django-markdownify Version: 0.9.4 Summary: Markdown
 template filter for Django. Home-page: https://github.com/erwinmatijsen/django-
 markdownify Download-URL: https://github.com/erwinmatijsen/django-markdownify/
-archive/0.9.3.tar.gz Author: Erwin Matijsen, R Moelker Author-email:
+archive/0.9.4.tar.gz Author: Erwin Matijsen, R Moelker Author-email:
 erwin@erwinmatijsen.nl License: MIT Classifier: Environment :: Web Environment
 Classifier: Framework :: Django Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent Description-Content-Type: text/
-markdown License-File: LICENSE # Django Markdownify - A Django Markdown filter
+markdown License-File: LICENSE Requires-Dist: Django Requires-Dist: markdown
+Requires-Dist: bleach[css]>=5.0.0 # Django Markdownify - A Django Markdown
+filter ![PyPi Downloads](https://img.shields.io/pypi/dm/django-markdownify) !
+[License](https://img.shields.io/pypi/l/django-markdownify?color=brightgreen)
+[![Documentation Status](https://readthedocs.org/projects/django-markdownify/
+badge/?version=latest)](https://django-markdownify.readthedocs.io/en/latest/
+?badge=latest) ![Version](https://img.shields.io/pypi/v/django-markdownify)
 Django Markdownify is a template filter to convert Markdown to HTML in Django.
 Markdown is converted to HTML and sanitized. Read the full documentation on
 [Read the docs](http://django-markdownify.readthedocs.io/en/latest/) or check
-out the package on [pypi](https://pypi.python.org/pypi/django-markdownify). ##
-Usage Load the tag inside your template: ``` {% load markdownify %} ``` Then
-you can change markdown to html as follows: ``` {{ 'text'|markdownify }} ``` or
-``` {{ somevariable|markdownify }} ``` ## Example ``` {% load markdownify %} {
-{'Some *test* [link](#)'|markdownify }} ``` Is transformed to: ```html
+out the package on [pypi](https://pypi.python.org/pypi/django-markdownify). >
+[!WARNING] > The [old settings](https://django-markdownify.readthedocs.io/en/
+latest/settings-old.html#oldsettings) are removed in release 0.9.4! Please
+update to the [new settings](https://django-markdownify.readthedocs.io/en/
+latest/settings.html) as soon as possible. ## Usage Load the tag inside your
+template: ``` {% load markdownify %} ``` Then you can change markdown to html
+as follows: ``` {{ 'text'|markdownify }} ``` or ``` {{ somevariable|markdownify
+}} ``` ## Example ``` {% load markdownify %} {{'Some *test* [link]
+(#)'|markdownify }} ``` Is transformed to: ```html
 Some tteesstt _l_i_n_k
 ``` The filter is a wrapper around [Markdown](https://pypi.python.org/pypi/
 Markdown) and [Bleach](http://pythonhosted.org/bleach/index.html) and as such
 supports their settings. It is possible to define multiple settings for
 multiple usecases. For example: ```python # settings.py MARKDOWNIFY =
 { "default": { "WHITELIST_TAGS": ["a", "p", "h1", ] }, "alternative":
 { "WHITELIST_TAGS": ["a", "p", ], "MARKDOWN_EXTENSIONS":
```

### Comparing `django-markdownify-0.9.3/README.md` & `django_markdownify-0.9.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,21 @@
 # Django Markdownify - A Django Markdown filter
 
+![PyPi Downloads](https://img.shields.io/pypi/dm/django-markdownify) 
+![License](https://img.shields.io/pypi/l/django-markdownify?color=brightgreen)
+[![Documentation Status](https://readthedocs.org/projects/django-markdownify/badge/?version=latest)](https://django-markdownify.readthedocs.io/en/latest/?badge=latest)
+![Version](https://img.shields.io/pypi/v/django-markdownify)
+
 Django Markdownify is a template filter to convert Markdown to HTML in Django. Markdown is converted to HTML and sanitized.
 
 Read the full documentation on [Read the docs](http://django-markdownify.readthedocs.io/en/latest/) or check out the package on [pypi](https://pypi.python.org/pypi/django-markdownify).
 
+> [!WARNING]  
+> The [old settings](https://django-markdownify.readthedocs.io/en/latest/settings-old.html#oldsettings) are removed in release 0.9.4! Please update to the [new settings](https://django-markdownify.readthedocs.io/en/latest/settings.html) as soon as possible.
+
 ## Usage
 
 Load the tag inside your template:
 
 ```
 {% load markdownify %}
 ```
```

#### html2text {}

```diff
@@ -1,16 +1,25 @@
-# Django Markdownify - A Django Markdown filter Django Markdownify is a
-template filter to convert Markdown to HTML in Django. Markdown is converted to
-HTML and sanitized. Read the full documentation on [Read the docs](http://
-django-markdownify.readthedocs.io/en/latest/) or check out the package on
-[pypi](https://pypi.python.org/pypi/django-markdownify). ## Usage Load the tag
-inside your template: ``` {% load markdownify %} ``` Then you can change
-markdown to html as follows: ``` {{ 'text'|markdownify }} ``` or ``` {
-{ somevariable|markdownify }} ``` ## Example ``` {% load markdownify %} {{'Some
-*test* [link](#)'|markdownify }} ``` Is transformed to: ```html
+# Django Markdownify - A Django Markdown filter ![PyPi Downloads](https://
+img.shields.io/pypi/dm/django-markdownify) ![License](https://img.shields.io/
+pypi/l/django-markdownify?color=brightgreen) [![Documentation Status](https://
+readthedocs.org/projects/django-markdownify/badge/?version=latest)](https://
+django-markdownify.readthedocs.io/en/latest/?badge=latest) ![Version](https://
+img.shields.io/pypi/v/django-markdownify) Django Markdownify is a template
+filter to convert Markdown to HTML in Django. Markdown is converted to HTML and
+sanitized. Read the full documentation on [Read the docs](http://django-
+markdownify.readthedocs.io/en/latest/) or check out the package on [pypi]
+(https://pypi.python.org/pypi/django-markdownify). > [!WARNING] > The [old
+settings](https://django-markdownify.readthedocs.io/en/latest/settings-
+old.html#oldsettings) are removed in release 0.9.4! Please update to the [new
+settings](https://django-markdownify.readthedocs.io/en/latest/settings.html) as
+soon as possible. ## Usage Load the tag inside your template: ``` {% load
+markdownify %} ``` Then you can change markdown to html as follows: ``` {
+{ 'text'|markdownify }} ``` or ``` {{ somevariable|markdownify }} ``` ##
+Example ``` {% load markdownify %} {{'Some *test* [link](#)'|markdownify }} ```
+Is transformed to: ```html
 Some tteesstt _l_i_n_k
 ``` The filter is a wrapper around [Markdown](https://pypi.python.org/pypi/
 Markdown) and [Bleach](http://pythonhosted.org/bleach/index.html) and as such
 supports their settings. It is possible to define multiple settings for
 multiple usecases. For example: ```python # settings.py MARKDOWNIFY =
 { "default": { "WHITELIST_TAGS": ["a", "p", "h1", ] }, "alternative":
 { "WHITELIST_TAGS": ["a", "p", ], "MARKDOWN_EXTENSIONS":
```

### Comparing `django-markdownify-0.9.3/django_markdownify.egg-info/PKG-INFO` & `django_markdownify-0.9.4/django_markdownify.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,40 @@
 Metadata-Version: 2.1
 Name: django-markdownify
-Version: 0.9.3
+Version: 0.9.4
 Summary: Markdown template filter for Django.
 Home-page: https://github.com/erwinmatijsen/django-markdownify
-Download-URL: https://github.com/erwinmatijsen/django-markdownify/archive/0.9.3.tar.gz
+Download-URL: https://github.com/erwinmatijsen/django-markdownify/archive/0.9.4.tar.gz
 Author: Erwin Matijsen, R Moelker
 Author-email: erwin@erwinmatijsen.nl
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: Django
+Requires-Dist: markdown
+Requires-Dist: bleach[css]>=5.0.0
 
 # Django Markdownify - A Django Markdown filter
 
+![PyPi Downloads](https://img.shields.io/pypi/dm/django-markdownify) 
+![License](https://img.shields.io/pypi/l/django-markdownify?color=brightgreen)
+[![Documentation Status](https://readthedocs.org/projects/django-markdownify/badge/?version=latest)](https://django-markdownify.readthedocs.io/en/latest/?badge=latest)
+![Version](https://img.shields.io/pypi/v/django-markdownify)
+
 Django Markdownify is a template filter to convert Markdown to HTML in Django. Markdown is converted to HTML and sanitized.
 
 Read the full documentation on [Read the docs](http://django-markdownify.readthedocs.io/en/latest/) or check out the package on [pypi](https://pypi.python.org/pypi/django-markdownify).
 
+> [!WARNING]  
+> The [old settings](https://django-markdownify.readthedocs.io/en/latest/settings-old.html#oldsettings) are removed in release 0.9.4! Please update to the [new settings](https://django-markdownify.readthedocs.io/en/latest/settings.html) as soon as possible.
+
 ## Usage
 
 Load the tag inside your template:
 
 ```
 {% load markdownify %}
 ```
```

#### html2text {}

```diff
@@ -1,23 +1,33 @@
-Metadata-Version: 2.1 Name: django-markdownify Version: 0.9.3 Summary: Markdown
+Metadata-Version: 2.1 Name: django-markdownify Version: 0.9.4 Summary: Markdown
 template filter for Django. Home-page: https://github.com/erwinmatijsen/django-
 markdownify Download-URL: https://github.com/erwinmatijsen/django-markdownify/
-archive/0.9.3.tar.gz Author: Erwin Matijsen, R Moelker Author-email:
+archive/0.9.4.tar.gz Author: Erwin Matijsen, R Moelker Author-email:
 erwin@erwinmatijsen.nl License: MIT Classifier: Environment :: Web Environment
 Classifier: Framework :: Django Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent Description-Content-Type: text/
-markdown License-File: LICENSE # Django Markdownify - A Django Markdown filter
+markdown License-File: LICENSE Requires-Dist: Django Requires-Dist: markdown
+Requires-Dist: bleach[css]>=5.0.0 # Django Markdownify - A Django Markdown
+filter ![PyPi Downloads](https://img.shields.io/pypi/dm/django-markdownify) !
+[License](https://img.shields.io/pypi/l/django-markdownify?color=brightgreen)
+[![Documentation Status](https://readthedocs.org/projects/django-markdownify/
+badge/?version=latest)](https://django-markdownify.readthedocs.io/en/latest/
+?badge=latest) ![Version](https://img.shields.io/pypi/v/django-markdownify)
 Django Markdownify is a template filter to convert Markdown to HTML in Django.
 Markdown is converted to HTML and sanitized. Read the full documentation on
 [Read the docs](http://django-markdownify.readthedocs.io/en/latest/) or check
-out the package on [pypi](https://pypi.python.org/pypi/django-markdownify). ##
-Usage Load the tag inside your template: ``` {% load markdownify %} ``` Then
-you can change markdown to html as follows: ``` {{ 'text'|markdownify }} ``` or
-``` {{ somevariable|markdownify }} ``` ## Example ``` {% load markdownify %} {
-{'Some *test* [link](#)'|markdownify }} ``` Is transformed to: ```html
+out the package on [pypi](https://pypi.python.org/pypi/django-markdownify). >
+[!WARNING] > The [old settings](https://django-markdownify.readthedocs.io/en/
+latest/settings-old.html#oldsettings) are removed in release 0.9.4! Please
+update to the [new settings](https://django-markdownify.readthedocs.io/en/
+latest/settings.html) as soon as possible. ## Usage Load the tag inside your
+template: ``` {% load markdownify %} ``` Then you can change markdown to html
+as follows: ``` {{ 'text'|markdownify }} ``` or ``` {{ somevariable|markdownify
+}} ``` ## Example ``` {% load markdownify %} {{'Some *test* [link]
+(#)'|markdownify }} ``` Is transformed to: ```html
 Some tteesstt _l_i_n_k
 ``` The filter is a wrapper around [Markdown](https://pypi.python.org/pypi/
 Markdown) and [Bleach](http://pythonhosted.org/bleach/index.html) and as such
 supports their settings. It is possible to define multiple settings for
 multiple usecases. For example: ```python # settings.py MARKDOWNIFY =
 { "default": { "WHITELIST_TAGS": ["a", "p", "h1", ] }, "alternative":
 { "WHITELIST_TAGS": ["a", "p", ], "MARKDOWN_EXTENSIONS":
```

### Comparing `django-markdownify-0.9.3/django_markdownify.egg-info/SOURCES.txt` & `django_markdownify-0.9.4/django_markdownify.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-markdownify-0.9.3/markdownify/checks.py` & `django_markdownify-0.9.4/markdownify/checks.py`

 * *Files identical despite different names*

### Comparing `django-markdownify-0.9.3/markdownify/tests/input_text_default.md` & `django_markdownify-0.9.4/markdownify/tests/input_text_default.md`

 * *Files identical despite different names*

### Comparing `django-markdownify-0.9.3/setup.py` & `django_markdownify-0.9.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 README = open(os.path.join(os.path.dirname(__file__), 'README.md')).read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='django-markdownify',
-    version='0.9.3',
+    version='0.9.4',
     packages=['markdownify'],
     package_dir={'markdownify': 'markdownify'},
     package_data={'markdownify': ['tests/*.md']},
     include_package_data=True,
     license='MIT',
     description='Markdown template filter for Django.',
     long_description=README,
     long_description_content_type="text/markdown",
     url='https://github.com/erwinmatijsen/django-markdownify',
-    download_url='https://github.com/erwinmatijsen/django-markdownify/archive/0.9.3.tar.gz',
+    download_url='https://github.com/erwinmatijsen/django-markdownify/archive/0.9.4.tar.gz',
     author='Erwin Matijsen, R Moelker',
     author_email='erwin@erwinmatijsen.nl',
     classifiers=[
         'Environment :: Web Environment',
         'Framework :: Django',
         'Intended Audience :: Developers',
         'Operating System :: OS Independent',
```

