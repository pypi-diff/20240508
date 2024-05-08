# Comparing `tmp/django_tbase_post_product-2024.5.117145788.tar.gz` & `tmp/django_tbase_post_product-2024.5.917151916.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_tbase_post_product-2024.5.117145788.tar", last modified: Wed May  1 15:53:49 2024, max compression
+gzip compressed data, was "django_tbase_post_product-2024.5.917151916.tar", last modified: Wed May  8 18:07:06 2024, max compression
```

## Comparing `django_tbase_post_product-2024.5.117145788.tar` & `django_tbase_post_product-2024.5.917151916.tar`

### file list

```diff
@@ -1,60 +1,75 @@
-drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2024-05-01 15:53:49.994354 django_tbase_post_product-2024.5.117145788/
--rw-rw-r--   0 terry     (1000) terry     (1000)      143 2023-12-03 08:49:22.000000 django_tbase_post_product-2024.5.117145788/MANIFEST.in
--rw-rw-r--   0 terry     (1000) terry     (1000)     1961 2024-05-01 15:53:49.994354 django_tbase_post_product-2024.5.117145788/PKG-INFO
--rw-rw-r--   0 terry     (1000) terry     (1000)     1639 2024-05-01 15:48:38.000000 django_tbase_post_product-2024.5.117145788/README.md
-drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2024-05-01 15:53:49.990354 django_tbase_post_product-2024.5.117145788/django_tbase_post_product.egg-info/
--rw-rw-r--   0 terry     (1000) terry     (1000)     1961 2024-05-01 15:53:49.000000 django_tbase_post_product-2024.5.117145788/django_tbase_post_product.egg-info/PKG-INFO
--rw-rw-r--   0 terry     (1000) terry     (1000)     1983 2024-05-01 15:53:49.000000 django_tbase_post_product-2024.5.117145788/django_tbase_post_product.egg-info/SOURCES.txt
--rw-rw-r--   0 terry     (1000) terry     (1000)        1 2024-05-01 15:53:49.000000 django_tbase_post_product-2024.5.117145788/django_tbase_post_product.egg-info/dependency_links.txt
--rw-rw-r--   0 terry     (1000) terry     (1000)       83 2024-05-01 15:53:49.000000 django_tbase_post_product-2024.5.117145788/django_tbase_post_product.egg-info/requires.txt
--rw-rw-r--   0 terry     (1000) terry     (1000)       11 2024-05-01 15:53:49.000000 django_tbase_post_product-2024.5.117145788/django_tbase_post_product.egg-info/top_level.txt
--rw-rw-r--   0 terry     (1000) terry     (1000)       38 2024-05-01 15:53:49.994354 django_tbase_post_product-2024.5.117145788/setup.cfg
--rw-rw-r--   0 terry     (1000) terry     (1000)     2305 2023-12-03 08:49:22.000000 django_tbase_post_product-2024.5.117145788/setup.py
-drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2024-05-01 15:53:49.990354 django_tbase_post_product-2024.5.117145788/tbase_post/
--rw-rw-r--   0 terry     (1000) terry     (1000)     7569 2024-03-12 15:28:36.000000 django_tbase_post_product-2024.5.117145788/tbase_post/0001_initial.py
--rw-rw-r--   0 terry     (1000) terry     (1000)        0 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.117145788/tbase_post/__init__.py
--rw-rw-r--   0 terry     (1000) terry     (1000)     6331 2024-03-13 03:45:25.000000 django_tbase_post_product-2024.5.117145788/tbase_post/admin.py
--rw-rw-r--   0 terry     (1000) terry     (1000)      146 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.117145788/tbase_post/apps.py
-drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2024-05-01 15:53:49.990354 django_tbase_post_product-2024.5.117145788/tbase_post/migrations/
--rw-rw-r--   0 terry     (1000) terry     (1000)        0 2023-12-03 07:39:38.000000 django_tbase_post_product-2024.5.117145788/tbase_post/migrations/__init__.py
--rw-rw-r--   0 terry     (1000) terry     (1000)    10357 2024-04-13 13:06:33.000000 django_tbase_post_product-2024.5.117145788/tbase_post/models.py
--rw-rw-r--   0 terry     (1000) terry     (1000)      616 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.117145788/tbase_post/sitemaps.py
-drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2024-05-01 15:53:49.986354 django_tbase_post_product-2024.5.117145788/tbase_post/static/
-drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2024-05-01 15:53:49.990354 django_tbase_post_product-2024.5.117145788/tbase_post/static/images/
--rw-rw-r--   0 terry     (1000) terry     (1000)    59619 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.117145788/tbase_post/static/images/photo-1578707399887-e6d183c9e598.jpeg
--rw-rw-r--   0 terry     (1000) terry     (1000)       94 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.117145788/tbase_post/static/images/photo-1578707399887-e6d183c9e598.jpeg:Zone.Identifier
-drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2024-05-01 15:53:49.990354 django_tbase_post_product-2024.5.117145788/tbase_post/templates/
-drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2024-05-01 15:53:49.990354 django_tbase_post_product-2024.5.117145788/tbase_post/templates/post/
--rw-rw-r--   0 terry     (1000) terry     (1000)     5494 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.117145788/tbase_post/templates/post/article_list_by_tag.html
--rw-rw-r--   0 terry     (1000) terry     (1000)     2994 2024-04-13 11:28:01.000000 django_tbase_post_product-2024.5.117145788/tbase_post/templates/post/blog_index.html
--rw-rw-r--   0 terry     (1000) terry     (1000)    11328 2024-05-01 15:47:31.000000 django_tbase_post_product-2024.5.117145788/tbase_post/templates/post/detail.html
-drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2024-05-01 15:53:49.994354 django_tbase_post_product-2024.5.117145788/tbase_post/templates/post/extras/
--rw-rw-r--   0 terry     (1000) terry     (1000)      732 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.117145788/tbase_post/templates/post/extras/amazon_ads.html
--rw-rw-r--   0 terry     (1000) terry     (1000)      591 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.117145788/tbase_post/templates/post/extras/amazon_link.html
--rw-rw-r--   0 terry     (1000) terry     (1000)      884 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.117145788/tbase_post/templates/post/extras/hitcount_lowest_post.html
--rw-rw-r--   0 terry     (1000) terry     (1000)      818 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.117145788/tbase_post/templates/post/extras/hitcount_top_post.html
--rw-rw-r--   0 terry     (1000) terry     (1000)     1926 2024-05-01 15:53:21.000000 django_tbase_post_product-2024.5.117145788/tbase_post/templates/post/extras/last_update.html
--rw-rw-r--   0 terry     (1000) terry     (1000)     1822 2024-05-01 15:53:08.000000 django_tbase_post_product-2024.5.117145788/tbase_post/templates/post/extras/related_post_by_tags.html
--rw-rw-r--   0 terry     (1000) terry     (1000)      827 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.117145788/tbase_post/templates/post/extras/seo_top_links.html
--rw-rw-r--   0 terry     (1000) terry     (1000)      569 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.117145788/tbase_post/templates/post/extras/tags.html
--rw-rw-r--   0 terry     (1000) terry     (1000)      132 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.117145788/tbase_post/templates/post/extras/templ.html
--rw-rw-r--   0 terry     (1000) terry     (1000)      576 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.117145788/tbase_post/templates/post/extras/youtube_player.html
--rw-rw-r--   0 terry     (1000) terry     (1000)     2109 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.117145788/tbase_post/templates/post/last_index.html
--rw-rw-r--   0 terry     (1000) terry     (1000)      255 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.117145788/tbase_post/templates/post/prompt_task_detail copy.html
--rw-rw-r--   0 terry     (1000) terry     (1000)     4751 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.117145788/tbase_post/templates/post/prompt_task_detail.html
--rw-rw-r--   0 terry     (1000) terry     (1000)      426 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.117145788/tbase_post/templates/post/prompt_task_list.html
--rw-rw-r--   0 terry     (1000) terry     (1000)     2483 2024-03-13 03:47:25.000000 django_tbase_post_product-2024.5.117145788/tbase_post/templates/post/prompt_task_post_detail.html
--rw-rw-r--   0 terry     (1000) terry     (1000)     4733 2024-03-13 03:36:27.000000 django_tbase_post_product-2024.5.117145788/tbase_post/templates/post/prompt_task_post_list.html
--rw-rw-r--   0 terry     (1000) terry     (1000)      765 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.117145788/tbase_post/templates/post_list.html
--rw-rw-r--   0 terry     (1000) terry     (1000)      391 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.117145788/tbase_post/templates/sitemap.xml
-drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2024-05-01 15:53:49.994354 django_tbase_post_product-2024.5.117145788/tbase_post/templatetags/
--rw-rw-r--   0 terry     (1000) terry     (1000)        0 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.117145788/tbase_post/templatetags/__init__.py
-drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2024-05-01 15:53:49.994354 django_tbase_post_product-2024.5.117145788/tbase_post/templatetags/__pycache__/
--rw-rw-r--   0 terry     (1000) terry     (1000)      196 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.117145788/tbase_post/templatetags/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 terry     (1000) terry     (1000)      190 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.117145788/tbase_post/templatetags/__pycache__/__init__.cpython-39.pyc
--rw-rw-r--   0 terry     (1000) terry     (1000)     6290 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.117145788/tbase_post/templatetags/__pycache__/post_extras.cpython-310.pyc
--rw-rw-r--   0 terry     (1000) terry     (1000)     4111 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.117145788/tbase_post/templatetags/__pycache__/post_extras.cpython-39.pyc
--rw-rw-r--   0 terry     (1000) terry     (1000)    11661 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.117145788/tbase_post/templatetags/post_extras.py
--rw-rw-r--   0 terry     (1000) terry     (1000)       60 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.117145788/tbase_post/tests.py
--rw-rw-r--   0 terry     (1000) terry     (1000)     1571 2024-03-13 03:17:25.000000 django_tbase_post_product-2024.5.117145788/tbase_post/urls.py
--rw-rw-r--   0 terry     (1000) terry     (1000)    11928 2024-03-13 03:43:23.000000 django_tbase_post_product-2024.5.117145788/tbase_post/views.py
+drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2024-05-08 18:07:06.354907 django_tbase_post_product-2024.5.917151916/
+-rw-rw-r--   0 terry     (1000) terry     (1000)      143 2023-12-03 08:49:22.000000 django_tbase_post_product-2024.5.917151916/MANIFEST.in
+-rw-rw-r--   0 terry     (1000) terry     (1000)     2030 2024-05-08 18:07:06.354907 django_tbase_post_product-2024.5.917151916/PKG-INFO
+-rw-rw-r--   0 terry     (1000) terry     (1000)     1708 2024-05-08 18:06:59.000000 django_tbase_post_product-2024.5.917151916/README.md
+drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2024-05-08 18:07:06.346907 django_tbase_post_product-2024.5.917151916/django_tbase_post_product.egg-info/
+-rw-rw-r--   0 terry     (1000) terry     (1000)     2030 2024-05-08 18:07:06.000000 django_tbase_post_product-2024.5.917151916/django_tbase_post_product.egg-info/PKG-INFO
+-rw-rw-r--   0 terry     (1000) terry     (1000)     2634 2024-05-08 18:07:06.000000 django_tbase_post_product-2024.5.917151916/django_tbase_post_product.egg-info/SOURCES.txt
+-rw-rw-r--   0 terry     (1000) terry     (1000)        1 2024-05-08 18:07:06.000000 django_tbase_post_product-2024.5.917151916/django_tbase_post_product.egg-info/dependency_links.txt
+-rw-rw-r--   0 terry     (1000) terry     (1000)       83 2024-05-08 18:07:06.000000 django_tbase_post_product-2024.5.917151916/django_tbase_post_product.egg-info/requires.txt
+-rw-rw-r--   0 terry     (1000) terry     (1000)       11 2024-05-08 18:07:06.000000 django_tbase_post_product-2024.5.917151916/django_tbase_post_product.egg-info/top_level.txt
+-rw-rw-r--   0 terry     (1000) terry     (1000)       38 2024-05-08 18:07:06.354907 django_tbase_post_product-2024.5.917151916/setup.cfg
+-rw-rw-r--   0 terry     (1000) terry     (1000)     2305 2023-12-03 08:49:22.000000 django_tbase_post_product-2024.5.917151916/setup.py
+drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2024-05-08 18:07:06.350907 django_tbase_post_product-2024.5.917151916/tbase_post/
+-rw-rw-r--   0 terry     (1000) terry     (1000)     7569 2024-03-12 15:28:36.000000 django_tbase_post_product-2024.5.917151916/tbase_post/0001_initial.py
+-rw-rw-r--   0 terry     (1000) terry     (1000)        0 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.917151916/tbase_post/__init__.py
+drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2024-05-08 18:07:06.350907 django_tbase_post_product-2024.5.917151916/tbase_post/__pycache__/
+-rw-rw-r--   0 terry     (1000) terry     (1000)      183 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.917151916/tbase_post/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 terry     (1000) terry     (1000)     4983 2024-03-13 03:45:26.000000 django_tbase_post_product-2024.5.917151916/tbase_post/__pycache__/admin.cpython-310.pyc
+-rw-rw-r--   0 terry     (1000) terry     (1000)      464 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.917151916/tbase_post/__pycache__/apps.cpython-310.pyc
+-rw-rw-r--   0 terry     (1000) terry     (1000)     7593 2024-04-13 13:06:34.000000 django_tbase_post_product-2024.5.917151916/tbase_post/__pycache__/models.cpython-310.pyc
+-rw-rw-r--   0 terry     (1000) terry     (1000)     1095 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.917151916/tbase_post/__pycache__/sitemaps.cpython-310.pyc
+-rw-rw-r--   0 terry     (1000) terry     (1000)      224 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.917151916/tbase_post/__pycache__/tests.cpython-310.pyc
+-rw-rw-r--   0 terry     (1000) terry     (1000)     1343 2024-03-13 03:17:26.000000 django_tbase_post_product-2024.5.917151916/tbase_post/__pycache__/urls.cpython-310.pyc
+-rw-rw-r--   0 terry     (1000) terry     (1000)     7307 2024-05-08 16:40:04.000000 django_tbase_post_product-2024.5.917151916/tbase_post/__pycache__/views.cpython-310.pyc
+-rw-rw-r--   0 terry     (1000) terry     (1000)     6331 2024-03-13 03:45:25.000000 django_tbase_post_product-2024.5.917151916/tbase_post/admin.py
+-rw-rw-r--   0 terry     (1000) terry     (1000)      146 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.917151916/tbase_post/apps.py
+drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2024-05-08 18:07:06.350907 django_tbase_post_product-2024.5.917151916/tbase_post/migrations/
+-rw-rw-r--   0 terry     (1000) terry     (1000)     7576 2024-05-08 16:43:18.000000 django_tbase_post_product-2024.5.917151916/tbase_post/migrations/0001_initial.py
+-rw-rw-r--   0 terry     (1000) terry     (1000)        0 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.917151916/tbase_post/migrations/__init__.py
+drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2024-05-08 18:07:06.350907 django_tbase_post_product-2024.5.917151916/tbase_post/migrations/__pycache__/
+-rw-rw-r--   0 terry     (1000) terry     (1000)     5196 2024-05-08 16:43:28.000000 django_tbase_post_product-2024.5.917151916/tbase_post/migrations/__pycache__/0001_initial.cpython-310.pyc
+-rw-rw-r--   0 terry     (1000) terry     (1000)      194 2024-05-08 16:43:17.000000 django_tbase_post_product-2024.5.917151916/tbase_post/migrations/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 terry     (1000) terry     (1000)    10357 2024-04-13 13:06:33.000000 django_tbase_post_product-2024.5.917151916/tbase_post/models.py
+-rw-rw-r--   0 terry     (1000) terry     (1000)      616 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.917151916/tbase_post/sitemaps.py
+drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2024-05-08 18:07:06.346907 django_tbase_post_product-2024.5.917151916/tbase_post/static/
+drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2024-05-08 18:07:06.350907 django_tbase_post_product-2024.5.917151916/tbase_post/static/images/
+-rw-rw-r--   0 terry     (1000) terry     (1000)    59619 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.917151916/tbase_post/static/images/photo-1578707399887-e6d183c9e598.jpeg
+-rw-rw-r--   0 terry     (1000) terry     (1000)       94 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.917151916/tbase_post/static/images/photo-1578707399887-e6d183c9e598.jpeg:Zone.Identifier
+drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2024-05-08 18:07:06.350907 django_tbase_post_product-2024.5.917151916/tbase_post/templates/
+drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2024-05-08 18:07:06.350907 django_tbase_post_product-2024.5.917151916/tbase_post/templates/post/
+-rw-rw-r--   0 terry     (1000) terry     (1000)     5333 2024-05-08 16:49:53.000000 django_tbase_post_product-2024.5.917151916/tbase_post/templates/post/article_list_by_tag.html
+-rw-rw-r--   0 terry     (1000) terry     (1000)     3809 2024-05-08 17:11:30.000000 django_tbase_post_product-2024.5.917151916/tbase_post/templates/post/blog_index.html
+-rw-rw-r--   0 terry     (1000) terry     (1000)    11424 2024-05-08 17:47:08.000000 django_tbase_post_product-2024.5.917151916/tbase_post/templates/post/detail.html
+drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2024-05-08 18:07:06.354907 django_tbase_post_product-2024.5.917151916/tbase_post/templates/post/extras/
+-rw-rw-r--   0 terry     (1000) terry     (1000)      732 2024-05-08 17:02:46.000000 django_tbase_post_product-2024.5.917151916/tbase_post/templates/post/extras/amazon_ads.html
+-rw-rw-r--   0 terry     (1000) terry     (1000)      516 2024-05-08 17:02:35.000000 django_tbase_post_product-2024.5.917151916/tbase_post/templates/post/extras/amazon_link.html
+-rw-rw-r--   0 terry     (1000) terry     (1000)      415 2024-05-08 17:45:22.000000 django_tbase_post_product-2024.5.917151916/tbase_post/templates/post/extras/get_previous_next_by_pk.html
+-rw-rw-r--   0 terry     (1000) terry     (1000)      884 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.917151916/tbase_post/templates/post/extras/hitcount_lowest_post.html
+-rw-rw-r--   0 terry     (1000) terry     (1000)      818 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.917151916/tbase_post/templates/post/extras/hitcount_top_post.html
+-rw-rw-r--   0 terry     (1000) terry     (1000)     1870 2024-05-08 17:02:18.000000 django_tbase_post_product-2024.5.917151916/tbase_post/templates/post/extras/last_update.html
+-rw-rw-r--   0 terry     (1000) terry     (1000)      970 2024-05-08 17:02:05.000000 django_tbase_post_product-2024.5.917151916/tbase_post/templates/post/extras/related_post_by_tags.html
+-rw-rw-r--   0 terry     (1000) terry     (1000)      404 2024-05-08 16:54:27.000000 django_tbase_post_product-2024.5.917151916/tbase_post/templates/post/extras/related_post_by_tags_mini.html
+-rw-rw-r--   0 terry     (1000) terry     (1000)      827 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.917151916/tbase_post/templates/post/extras/seo_top_links.html
+-rw-rw-r--   0 terry     (1000) terry     (1000)      509 2024-05-08 17:00:09.000000 django_tbase_post_product-2024.5.917151916/tbase_post/templates/post/extras/tags.html
+-rw-rw-r--   0 terry     (1000) terry     (1000)      132 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.917151916/tbase_post/templates/post/extras/templ.html
+-rw-rw-r--   0 terry     (1000) terry     (1000)      576 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.917151916/tbase_post/templates/post/extras/youtube_player.html
+-rw-rw-r--   0 terry     (1000) terry     (1000)     2109 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.917151916/tbase_post/templates/post/last_index.html
+-rw-rw-r--   0 terry     (1000) terry     (1000)      255 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.917151916/tbase_post/templates/post/prompt_task_detail copy.html
+-rw-rw-r--   0 terry     (1000) terry     (1000)     4751 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.917151916/tbase_post/templates/post/prompt_task_detail.html
+-rw-rw-r--   0 terry     (1000) terry     (1000)      426 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.917151916/tbase_post/templates/post/prompt_task_list.html
+-rw-rw-r--   0 terry     (1000) terry     (1000)     2483 2024-03-13 03:47:25.000000 django_tbase_post_product-2024.5.917151916/tbase_post/templates/post/prompt_task_post_detail.html
+-rw-rw-r--   0 terry     (1000) terry     (1000)     4733 2024-03-13 03:36:27.000000 django_tbase_post_product-2024.5.917151916/tbase_post/templates/post/prompt_task_post_list.html
+-rw-rw-r--   0 terry     (1000) terry     (1000)      765 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.917151916/tbase_post/templates/post_list.html
+-rw-rw-r--   0 terry     (1000) terry     (1000)      391 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.917151916/tbase_post/templates/sitemap.xml
+drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2024-05-08 18:07:06.354907 django_tbase_post_product-2024.5.917151916/tbase_post/templatetags/
+-rw-rw-r--   0 terry     (1000) terry     (1000)        0 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.917151916/tbase_post/templatetags/__init__.py
+drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2024-05-08 18:07:06.354907 django_tbase_post_product-2024.5.917151916/tbase_post/templatetags/__pycache__/
+-rw-rw-r--   0 terry     (1000) terry     (1000)      196 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.917151916/tbase_post/templatetags/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 terry     (1000) terry     (1000)      190 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.917151916/tbase_post/templatetags/__pycache__/__init__.cpython-39.pyc
+-rw-rw-r--   0 terry     (1000) terry     (1000)     6516 2024-05-08 16:31:29.000000 django_tbase_post_product-2024.5.917151916/tbase_post/templatetags/__pycache__/post_extras.cpython-310.pyc
+-rw-rw-r--   0 terry     (1000) terry     (1000)     4111 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.917151916/tbase_post/templatetags/__pycache__/post_extras.cpython-39.pyc
+-rw-rw-r--   0 terry     (1000) terry     (1000)    14032 2024-05-08 17:56:02.000000 django_tbase_post_product-2024.5.917151916/tbase_post/templatetags/post_extras.py
+-rw-rw-r--   0 terry     (1000) terry     (1000)       60 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.917151916/tbase_post/tests.py
+-rw-rw-r--   0 terry     (1000) terry     (1000)     1571 2024-03-13 03:17:25.000000 django_tbase_post_product-2024.5.917151916/tbase_post/urls.py
+-rw-rw-r--   0 terry     (1000) terry     (1000)    11938 2024-05-08 16:40:03.000000 django_tbase_post_product-2024.5.917151916/tbase_post/views.py
```

### Comparing `django_tbase_post_product-2024.5.117145788/PKG-INFO` & `django_tbase_post_product-2024.5.917151916/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django_tbase_post_product
-Version: 2024.5.117145788
+Version: 2024.5.917151916
 Summary: Terry django base post ,
 Home-page: https://terrychanorg.jetbrains.space/p/django-expand/repositories/tbase_post_product/files/README.md
 Author: Terry Chan
 Author-email: napoler2008@gmail.com
 Description-Content-Type: text/markdown
 
 # django-expand/tbase_post_product
@@ -32,15 +32,16 @@
     'taggit',
 
  ]
 ```
 
 
 ## 更新
-
+- 2024/05/1
+优化内部链接，增加相关链接和上下文链接
 - 2024/05/1
 注销掉底部广告（banner-amazon-footer）
 
 
 - 2024/04/13
 优化展示
```

### Comparing `django_tbase_post_product-2024.5.117145788/README.md` & `django_tbase_post_product-2024.5.917151916/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,16 @@
     'taggit',
 
  ]
 ```
 
 
 ## 更新
-
+- 2024/05/1
+优化内部链接，增加相关链接和上下文链接
 - 2024/05/1
 注销掉底部广告（banner-amazon-footer）
 
 
 - 2024/04/13
 优化展示
```

### Comparing `django_tbase_post_product-2024.5.117145788/django_tbase_post_product.egg-info/PKG-INFO` & `django_tbase_post_product-2024.5.917151916/django_tbase_post_product.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-tbase-post-product
-Version: 2024.5.117145788
+Version: 2024.5.917151916
 Summary: Terry django base post ,
 Home-page: https://terrychanorg.jetbrains.space/p/django-expand/repositories/tbase_post_product/files/README.md
 Author: Terry Chan
 Author-email: napoler2008@gmail.com
 Description-Content-Type: text/markdown
 
 # django-expand/tbase_post_product
@@ -32,15 +32,16 @@
     'taggit',
 
  ]
 ```
 
 
 ## 更新
-
+- 2024/05/1
+优化内部链接，增加相关链接和上下文链接
 - 2024/05/1
 注销掉底部广告（banner-amazon-footer）
 
 
 - 2024/04/13
 优化展示
```

### Comparing `django_tbase_post_product-2024.5.117145788/django_tbase_post_product.egg-info/SOURCES.txt` & `django_tbase_post_product-2024.5.917151916/django_tbase_post_product.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -11,15 +11,26 @@
 tbase_post/admin.py
 tbase_post/apps.py
 tbase_post/models.py
 tbase_post/sitemaps.py
 tbase_post/tests.py
 tbase_post/urls.py
 tbase_post/views.py
+tbase_post/__pycache__/__init__.cpython-310.pyc
+tbase_post/__pycache__/admin.cpython-310.pyc
+tbase_post/__pycache__/apps.cpython-310.pyc
+tbase_post/__pycache__/models.cpython-310.pyc
+tbase_post/__pycache__/sitemaps.cpython-310.pyc
+tbase_post/__pycache__/tests.cpython-310.pyc
+tbase_post/__pycache__/urls.cpython-310.pyc
+tbase_post/__pycache__/views.cpython-310.pyc
+tbase_post/migrations/0001_initial.py
 tbase_post/migrations/__init__.py
+tbase_post/migrations/__pycache__/0001_initial.cpython-310.pyc
+tbase_post/migrations/__pycache__/__init__.cpython-310.pyc
 tbase_post/static/images/photo-1578707399887-e6d183c9e598.jpeg
 tbase_post/static/images/photo-1578707399887-e6d183c9e598.jpeg:Zone.Identifier
 tbase_post/templates/post_list.html
 tbase_post/templates/sitemap.xml
 tbase_post/templates/post/article_list_by_tag.html
 tbase_post/templates/post/blog_index.html
 tbase_post/templates/post/detail.html
@@ -27,18 +38,20 @@
 tbase_post/templates/post/prompt_task_detail copy.html
 tbase_post/templates/post/prompt_task_detail.html
 tbase_post/templates/post/prompt_task_list.html
 tbase_post/templates/post/prompt_task_post_detail.html
 tbase_post/templates/post/prompt_task_post_list.html
 tbase_post/templates/post/extras/amazon_ads.html
 tbase_post/templates/post/extras/amazon_link.html
+tbase_post/templates/post/extras/get_previous_next_by_pk.html
 tbase_post/templates/post/extras/hitcount_lowest_post.html
 tbase_post/templates/post/extras/hitcount_top_post.html
 tbase_post/templates/post/extras/last_update.html
 tbase_post/templates/post/extras/related_post_by_tags.html
+tbase_post/templates/post/extras/related_post_by_tags_mini.html
 tbase_post/templates/post/extras/seo_top_links.html
 tbase_post/templates/post/extras/tags.html
 tbase_post/templates/post/extras/templ.html
 tbase_post/templates/post/extras/youtube_player.html
 tbase_post/templatetags/__init__.py
 tbase_post/templatetags/post_extras.py
 tbase_post/templatetags/__pycache__/__init__.cpython-310.pyc
```

### Comparing `django_tbase_post_product-2024.5.117145788/setup.py` & `django_tbase_post_product-2024.5.917151916/setup.py`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2024.5.117145788/tbase_post/0001_initial.py` & `django_tbase_post_product-2024.5.917151916/tbase_post/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2024.5.117145788/tbase_post/admin.py` & `django_tbase_post_product-2024.5.917151916/tbase_post/admin.py`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2024.5.117145788/tbase_post/models.py` & `django_tbase_post_product-2024.5.917151916/tbase_post/models.py`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2024.5.117145788/tbase_post/sitemaps.py` & `django_tbase_post_product-2024.5.917151916/tbase_post/sitemaps.py`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2024.5.117145788/tbase_post/static/images/photo-1578707399887-e6d183c9e598.jpeg` & `django_tbase_post_product-2024.5.917151916/tbase_post/static/images/photo-1578707399887-e6d183c9e598.jpeg`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2024.5.117145788/tbase_post/templates/post/article_list_by_tag.html` & `django_tbase_post_product-2024.5.917151916/tbase_post/templates/post/article_list_by_tag.html`

 * *Files 3% similar despite different names*

```diff
@@ -83,30 +83,32 @@
                 <div class="flex items-center justify-center bg-gray-100">
                  <p class="hover:opacity-75">
                      <img alt="{{detail.product_name}}" title="{{detail.title}}" src="{{detail.article_img}}">
                  </p>
                 </div>
                 {%endif%}
                 <div class="bg-white flex flex-col justify-start p-6">
-                    <a href="{% url 'detail_view' detail.pk %}" class="text-3xl font-bold hover:text-gray-700 pb-4">{{detail.title}}</a>
+                    <a href="{% url 'detail_view' detail.pk %}" class="text-xl font-bold hover:text-gray-700 pb-4">{{detail.title}}</a>
                     <p  class="text-sm pb-3">
                        Published on {{detail.created_on}}
                     </p>
 
                     <p class="pb-6">
-                        {% cache 36000 content_truncatechars_128 detail.pk %}  
+          
                         {{detail.content|truncatechars:128}}
-                        {% endcache %}
+               
                     </p>
 
-
-{% cache 36000 tags detail.pk %}
+ 
 {% tags detail.tags 5 detail.pk %}
-{% endcache %}
-                    <a href="{% url 'detail_view' detail.pk %}" class="uppercase text-gray-800 hover:text-black">Continue Reading {{detail.product_name}}<i class="fas fa-arrow-right"></i></a>
+    <!-- 相关链接 开始 -->
+    <p class="related-post-by-tags-block pb-6">
+        {% related_post_by_tags_mini detail.tags 5 detail.pk %}
+    </p>
+                
                 </div>
             </article>
 
  {% endfor %}
```

#### html2text {}

```diff
@@ -11,19 +11,17 @@
 article_list %} {% autoescape off %} {% get_solo 'tbase_post.AmazonSettings' as
 amz %}{{amz.ads_list1}} {% endautoescape %} {% for detail in object_list %}
 {%if detail.article_img%}
 [{{detail.product_name}}]
 {%endif%}
 _{_{_d_e_t_a_i_l_._t_i_t_l_e_}_}
 Published on {{detail.created_on}}
-{% cache 36000 content_truncatechars_128 detail.pk %} {
-{detail.content|truncatechars:128}} {% endcache %}
-{% cache 36000 tags detail.pk %} {% tags detail.tags 5 detail.pk %} {% endcache
-%}
-_C_o_n_t_i_n_u_e_ _R_e_a_d_i_n_g_ _{_{_d_e_t_a_i_l_._p_r_o_d_u_c_t___n_a_m_e_}_}
+{{detail.content|truncatechars:128}}
+{% tags detail.tags 5 detail.pk %}
+{% related_post_by_tags_mini detail.tags 5 detail.pk %}
 {% endfor %} {% comment %}
 {% if page_obj.has_previous %} _«_ _f_i_r_s_t _p_r_e_v_i_o_u_s {% endif %} Page {
 { page_obj.number }} of {{ page_obj.paginator.num_pages }}. {% if
 page_obj.has_next %} _n_e_x_t _l_a_s_t_ _» {% endif %}
 {% endcomment %} {% endblock %} {% block sidebar_section %} {% block about_us
 %}
 {% last_update 10 %}
```

### Comparing `django_tbase_post_product-2024.5.117145788/tbase_post/templates/post/blog_index.html` & `django_tbase_post_product-2024.5.917151916/tbase_post/templates/post/last_index.html`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,14 @@
 {% extends 'blog/blog.html' %}
 {% comment %} {% extends 'base.html' %} {% endcomment %}
 
 {% load post_extras %}
 {% load solo_tags %}
 {% comment %} 标题 {% endcomment %}
-{% block title %}<title>{% get_solo 'tbase_config.General' as site_config %}{{site_config.site_title}}</title>{% endblock %}
-
-
-{% block top_nav %}
-
-{% endblock %}
-
-{% block head %}
-{% endblock %}
-
+{% block title %}<title>{% get_solo 'tbase_config.General' as site_config %}{{site_config.site_title}} Update</title>{% endblock %}
 
 
 {% block top_toolbar %}
     {% comment %} top_toolbar start {% endcomment %}
 
      <nav class="w-full py-2 bg-zinc-800 shadow">
         <div class="w-full container mx-auto flex flex-wrap items-center justify-between">
@@ -26,70 +17,59 @@
                 <ul class="flex items-center justify-between font-bold text-sm text-white uppercase no-underline">
                     <li><a class="hover:text-gray-200 hover:underline px-4" href="{% url 'home'%}">Home</a></li>
                     <li><a class="hover:text-gray-200 hover:underline px-4"  rel="nofollow" href="{% url  'last_index' %}">Update</a></li>
                 </ul>
             </nav>
 
             <div class="flex items-center text-lg no-underline text-white pr-6">
-          
+                <!-- <a class="" href="#">
+                    <i class="fab fa-facebook"></i>
+                </a>
+                <a class="pl-6" href="#">
+                    <i class="fab fa-instagram"></i>
+                </a>
+                <a class="pl-6" href="#">
+                    <i class="fab fa-twitter"></i>
+                </a>
+                <a class="pl-6" href="#">
+                    <i class="fab fa-linkedin"></i>
+                </a> -->
             </div>
         </div>
 
     </nav>
     {% comment %} top_toolbar end {% endcomment %}
 {% endblock %}
 
 
 
 
 
 
 
+{% block top_nav %}
 
+{% endblock %}
 
-
-
-
-
+{% block head %}
+{% endblock %}
 
 {% comment %} article_list start {% endcomment %}
  {% block article_list %}
     <!--object_list start-->
+    <ul class="list-disc pl-1">
+
+
     {% for detail in object_list %}
-                <article class="w-full flex flex-col shadow my-4">
-                    <!-- Article Image -->
-              
-                    {%if detail.article_img%}
-                    <div class="flex items-center justify-center bg-gray-100">
-                     <p class="hover:opacity-75">
-                         <img alt="{{detail.product_name}}" title="{{detail.title}}"  src="{{detail.article_img}}">
-                     </p>
-                    </div>
-                    {%endif%}
-              
-
-                    <div class="bg-white flex flex-col justify-start p-6">
-                        <a href="{% url 'detail_view' detail.pk %}" class="text-3xl font-bold hover:text-gray-700 pb-4">{{detail.title|truncatechars:48}}</a>
-                        <p  class="text-sm pb-3">
-                            {% comment %} By <a href="#" class="font-semibold hover:text-gray-800">David Grzyb</a>,  {% endcomment %}
-                            Published on {{detail.created_on}}
-                        </p>
-
-                        <p class="pb-6">
-                            {% comment %} 限制文本长度 {% endcomment %}
-                            {{detail.content|truncatechars:128}}
-                            <a href="{% url 'detail_view' detail.pk %}" class="uppercase text-gray-800 hover:text-black">Continue Reading {{detail.product_name}}<i class="fas fa-arrow-right"></i></a>
-  
-                        </p>
-  {% tags detail.tags 5 detail.pk %}
-    </div>
-    </article>
+   <li class="mb-1">
+     <a href="{% url 'detail_view' detail.pk %}" class="">{{detail.title|truncatechars:128}}</a>
+</li>
     {% endfor %}
      <!--object_list end-->
-
+    </ul>
 {% endblock %}
 {% comment %} article_list end {% endcomment %}
```

#### html2text {}

```diff
@@ -1,20 +1,14 @@
 {% extends 'blog/blog.html' %} {% comment %} {% extends 'base.html' %} {%
 endcomment %} {% load post_extras %} {% load solo_tags %} {% comment %} æ é¢
 {% endcomment %} {% block title %}
-{% endblock %} {% block top_nav %} {% endblock %} {% block head %} {% endblock
-%} {% block top_toolbar %} {% comment %} top_toolbar start {% endcomment %}
+{% endblock %} {% block top_toolbar %} {% comment %} top_toolbar start {%
+endcomment %}
     * _H_o_m_e
     * _U_p_d_a_t_e
-{% comment %} top_toolbar end {% endcomment %} {% endblock %} {% comment %}
-article_list start {% endcomment %} {% block article_list %} {% for detail in
-object_list %} {%if detail.article_img%}
-[{{detail.product_name}}]
-{%endif%}
-_{_{_d_e_t_a_i_l_._t_i_t_l_e_|_t_r_u_n_c_a_t_e_c_h_a_r_s_:_4_8_}_}
-{% comment %} By _D_a_v_i_d_ _G_r_z_y_b, {% endcomment %} Published on {
-{detail.created_on}}
-{% comment %} éå¶ææ¬é¿åº¦ {% endcomment %} {
-{detail.content|truncatechars:128}}
-_C_o_n_t_i_n_u_e_ _R_e_a_d_i_n_g_ _{_{_d_e_t_a_i_l_._p_r_o_d_u_c_t___n_a_m_e_}_}
-{% tags detail.tags 5 detail.pk %}
-{% endfor %} {% endblock %} {% comment %} article_list end {% endcomment %}
+{% comment %} top_toolbar end {% endcomment %} {% endblock %} {% block top_nav
+%} {% endblock %} {% block head %} {% endblock %} {% comment %} article_list
+start {% endcomment %} {% block article_list %}
+    * {% for detail in object_list %}
+    * _{_{_d_e_t_a_i_l_._t_i_t_l_e_|_t_r_u_n_c_a_t_e_c_h_a_r_s_:_1_2_8_}_}
+    * {% endfor %}
+{% endblock %} {% comment %} article_list end {% endcomment %}
```

### Comparing `django_tbase_post_product-2024.5.117145788/tbase_post/templates/post/detail.html` & `django_tbase_post_product-2024.5.917151916/tbase_post/templates/post/detail.html`

 * *Files 6% similar despite different names*

```diff
@@ -335,15 +335,15 @@
 $('#banner-amazon').html(htmlStr)
 
 data={}
 var htmlStr = template('banner-img-tpl', data)
 $('#banner-img').html(htmlStr)
 data={}
 var htmlStr = template('banner-amazon-footer-tpl', data)
-// $('#banner-amazon-footer').html(htmlStr)
+$('#banner-amazon-footer').html(htmlStr)
 
 </script>
 
  
 <!--标签-->
 {% tags object.tags 5 object.pk %}
  <!--标签end-->
@@ -382,25 +382,35 @@
 
 
 <!--上一页下一页链接区域-->
 
 {% block article_previous_next %}
 
 {% if detail.get_previous_by_created_on  %}
-<a href="{% url 'detail_view' detail.get_previous_by_created_on.pk %}" class="w-1/2 bg-white shadow hover:shadow-md text-left p-6">
-<p class="text-lg text-blue-800 font-bold flex items-center"><i class="fas fa-arrow-left pr-1"></i> {{detail.get_previous_by_created_on.title}}</p>
-<p class="pt-2"></p>
-</a>
+<!-- <a href="{% url 'detail_view' detail.get_previous_by_created_on.pk %}" class="w-1/2 bg-white shadow hover:shadow-md text-left p-6">
+<p class="text-lg text-blue-800 font-bold flex items-center">
+    <i class="fas fa-arrow-left pr-1"></i> {{detail.get_previous_by_created_on.title}}
+</p>
+ 
+</a> -->
+
+{% get_previous_next_by_pk "previous" object.pk 5 %}
+ 
+
 
 {%endif%}
 {% if detail.get_next_by_created_on  %}
-<a href="{% url 'detail_view' detail.get_next_by_created_on.pk %}" class="w-1/2 bg-white shadow hover:shadow-md text-right p-6">
-<p class="text-lg text-blue-800 font-bold flex items-center justify-end">{{detail.get_next_by_created_on.title}} <i class="fas fa-arrow-right pl-1"></i></p>
-<p class="pt-2"></p>
-</a>
+<!-- <a href="{% url 'detail_view' detail.get_next_by_created_on.pk %}" class="w-1/2 bg-white shadow hover:shadow-md text-right p-6">
+<p class="text-lg text-blue-800 font-bold flex items-center justify-end">
+    {{detail.get_next_by_created_on.title}} <i class="fas fa-arrow-right pl-1"></i>
+</p>
+ 
+</a> -->
+
+{% get_previous_next_by_pk "next" object.pk 5 %}
 
 {%endif%}
 {% endblock %}
 <!--上一页下一页链接区域 结束-->
```

### Comparing `django_tbase_post_product-2024.5.117145788/tbase_post/templates/post/extras/amazon_ads.html` & `django_tbase_post_product-2024.5.917151916/tbase_post/templates/post/extras/amazon_ads.html`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2024.5.117145788/tbase_post/templates/post/extras/amazon_link.html` & `django_tbase_post_product-2024.5.917151916/tbase_post/templates/post/extras/amazon_link.html`

 * *Files 17% similar despite different names*

```diff
@@ -3,16 +3,15 @@
 # 加载标签
 load post_extras
 
 使用示例：
 tags object.tags.all
 
 -->
-{% load cache %}
-{% cache 36000 amazon_link_block product_id %}
+ 
 
 <div class="amazon_link">
     
     <div class="flex flex-wrap">
      
         {%if product_id and store_id %}
 
@@ -24,8 +23,8 @@
             </a>
     
       {%endif%}
      
      
     </div>
     </div>
-{% endcache %}
+
```

### Comparing `django_tbase_post_product-2024.5.117145788/tbase_post/templates/post/extras/hitcount_lowest_post.html` & `django_tbase_post_product-2024.5.917151916/tbase_post/templates/post/extras/hitcount_lowest_post.html`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2024.5.117145788/tbase_post/templates/post/extras/hitcount_top_post.html` & `django_tbase_post_product-2024.5.917151916/tbase_post/templates/post/extras/hitcount_top_post.html`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2024.5.117145788/tbase_post/templates/post/extras/last_update.html` & `django_tbase_post_product-2024.5.917151916/tbase_post/templates/post/extras/last_update.html`

 * *Files 11% similar despite different names*

```diff
@@ -3,47 +3,49 @@
 # 加载标签
 load post_extras
 
 使用示例：
 last_update 5
 
 -->
-<!-- {% load cache %}
-{% cache 3600 last_update_block pk %} -->
+ 
 
 <div class="last_update">
   <h2 class="text-gray-800 text-lg font-medium mb-2">{{title}}</h2>
   <div class="list-disc" >
-
-
     {%for item in page_obj%}
-     
           <div class="max-w-sm bg-white border border-gray-200 rounded-lg shadow dark:bg-gray-800 dark:border-gray-700 my-2">
             <a  rel="nofollow" href="{% url 'detail_view' item.pk %}" >
                 <img class="h-60 mx-auto" src="{{ item.article_img}}" alt="{{item}}" />
             </a>
             <div class="p-5">
                 <a  href="{% url 'detail_view' item.pk %}"  >
-                    <h5 class="mb-2 text-1xl font-bold tracking-tight text-gray-900 dark:text-white">{{item|truncatechars:32}}</h5>
+                    <h5 class="mb-2 text-xl font-bold tracking-tight text-gray-900 dark:text-white">{{item|truncatechars:32}}</h5>
                 </a>
                 <!-- <p class="mb-3 font-normal text-gray-700 dark:text-gray-400">{{item|truncatechars:32}}
     
                 </p>
                 <a rel="nofollow" href="{% url 'detail_view' item.pk %}" class="inline-flex items-center px-3 py-2 text-sm font-medium text-center text-white bg-blue-700 rounded-lg hover:bg-blue-800 focus:ring-4 focus:outline-none focus:ring-blue-300 dark:bg-blue-600 dark:hover:bg-blue-700 dark:focus:ring-blue-800">
                     Read more
                      <svg class="w-3.5 h-3.5 ml-2" aria-hidden="true" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 14 10">
                         <path stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M1 5h12m0 0L9 1m4 4L9 9"/>
                     </svg>
                 </a> -->
             </div>
         </div>
- 
+        
+    
+    
+    
+    
+    
+    
     
             <!-- <a href="{% url 'detail_view' item.pk %}" class="">{{item|truncatechars:32}}</a> -->
         <!-- </li> -->
     {%endfor%}
       <!-- </ul> -->
     
     </div>
 </div>
 
-<!-- {% endcache %} -->
+
```

### Comparing `django_tbase_post_product-2024.5.117145788/tbase_post/templates/post/extras/seo_top_links.html` & `django_tbase_post_product-2024.5.917151916/tbase_post/templates/post/extras/seo_top_links.html`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2024.5.117145788/tbase_post/templates/post/extras/youtube_player.html` & `django_tbase_post_product-2024.5.917151916/tbase_post/templates/post/extras/youtube_player.html`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2024.5.117145788/tbase_post/templates/post/last_index.html` & `django_tbase_post_product-2024.5.917151916/tbase_post/templates/post/blog_index.html`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,23 @@
 {% extends 'blog/blog.html' %}
 {% comment %} {% extends 'base.html' %} {% endcomment %}
 
 {% load post_extras %}
 {% load solo_tags %}
 {% comment %} 标题 {% endcomment %}
-{% block title %}<title>{% get_solo 'tbase_config.General' as site_config %}{{site_config.site_title}} Update</title>{% endblock %}
+{% block title %}<title>{% get_solo 'tbase_config.General' as site_config %}{{site_config.site_title}}</title>{% endblock %}
+
+
+{% block top_nav %}
+
+{% endblock %}
+
+{% block head %}
+{% endblock %}
+
 
 
 {% block top_toolbar %}
     {% comment %} top_toolbar start {% endcomment %}
 
      <nav class="w-full py-2 bg-zinc-800 shadow">
         <div class="w-full container mx-auto flex flex-wrap items-center justify-between">
@@ -17,59 +26,103 @@
                 <ul class="flex items-center justify-between font-bold text-sm text-white uppercase no-underline">
                     <li><a class="hover:text-gray-200 hover:underline px-4" href="{% url 'home'%}">Home</a></li>
                     <li><a class="hover:text-gray-200 hover:underline px-4"  rel="nofollow" href="{% url  'last_index' %}">Update</a></li>
                 </ul>
             </nav>
 
             <div class="flex items-center text-lg no-underline text-white pr-6">
-                <!-- <a class="" href="#">
-                    <i class="fab fa-facebook"></i>
-                </a>
-                <a class="pl-6" href="#">
-                    <i class="fab fa-instagram"></i>
-                </a>
-                <a class="pl-6" href="#">
-                    <i class="fab fa-twitter"></i>
-                </a>
-                <a class="pl-6" href="#">
-                    <i class="fab fa-linkedin"></i>
-                </a> -->
+          
             </div>
         </div>
 
     </nav>
     {% comment %} top_toolbar end {% endcomment %}
 {% endblock %}
 
 
+ 
+{% comment %} article_list start {% endcomment %}
+ {% block article_list %}
+    <!--object_list start-->
+    {% for detail in object_list %}
+                <article class="w-full flex flex-col shadow my-4">
+                    <!-- Article Image -->
+              
+                    {%if detail.article_img%}
+                    <div class="flex items-center justify-center bg-gray-100">
+                     <p class="hover:opacity-75">
+                         <img alt="{{detail.product_name}}" title="{{detail.title}}"  src="{{detail.article_img}}">
+                     </p>
+                    </div>
+                    {%endif%}
+              
+
+                    <div class="bg-white flex flex-col justify-start p-6">
+                        <a href="{% url 'detail_view' detail.pk %}" class="text-xl font-bold hover:text-gray-700 pb-4">{{detail.title|truncatechars:48}}</a>
+                        <p  class="text-sm pb-3">
+                            {% comment %} By <a href="#" class="font-semibold hover:text-gray-800">David Grzyb</a>,  {% endcomment %}
+                            Published on {{detail.created_on}}
+                        </p>
+
+                        <p class="pb-6">
+                            {% comment %} 限制文本长度 {% endcomment %}
+                            {{detail.content|truncatechars:128}}
+                            <!-- <a href="{% url 'detail_view' detail.pk %}" class="uppercase text-gray-800 hover:text-black">Continue Reading {{detail.product_name}}<i class="fas fa-arrow-right"></i></a>
+   -->
+                        </p>
+
+          
+
+  {% tags detail.tags 5 detail.pk %}
+
+  <!-- 相关链接 开始 -->
+  <p class="related-post-by-tags-block pb-6">
+    {% related_post_by_tags_mini detail.tags 5 detail.pk %}
+</p>
+    </div>
+    </article>
+    {% endfor %}
+     <!--object_list end-->
 
+{% endblock %}
+{% comment %} article_list end {% endcomment %}
 
+ 
 
 
 
-{% block top_nav %}
 
-{% endblock %}
 
-{% block head %}
-{% endblock %}
 
-{% comment %} article_list start {% endcomment %}
- {% block article_list %}
-    <!--object_list start-->
-    <ul class="list-disc pl-1">
 
 
-    {% for detail in object_list %}
-   <li class="mb-1">
-     <a href="{% url 'detail_view' detail.pk %}" class="">{{detail.title|truncatechars:128}}</a>
-</li>
-    {% endfor %}
-     <!--object_list end-->
-    </ul>
-{% endblock %}
-{% comment %} article_list end {% endcomment %}
+{% block sidebar_section %}
+<!-- sidebar_section -->
+ 
+<div class="w-full bg-white shadow flex flex-col my-4 p-6">
+        {% seo_top_links 50 %}
+</div>
+
+
+
+<!-- 广告代码  ads_sidebar-->
+{% autoescape off %}
+ 
+    <!--亚马逊推广链接-->
+    {% get_solo 'tbase_post.AmazonSettings' as amazon %}
+    {% amazon_ads object.product_id detail.product_name amazon.store_id %}
+    <!--亚马逊推广链接结束-->
+
+    
+    {% get_solo 'tbase_post.AmazonSettings' as amz %} 
 
 
+    {% if amz.ads_sidebar %}
+    {{amz.ads_sidebar}}
 
+    {% endif %}
 
+{% endautoescape %}
+<!-- 广告代码结束 -->
 
+    <!-- sidebar_section endblock -->
+   {% endblock %}
```

#### html2text {}

```diff
@@ -1,14 +1,26 @@
 {% extends 'blog/blog.html' %} {% comment %} {% extends 'base.html' %} {%
 endcomment %} {% load post_extras %} {% load solo_tags %} {% comment %} æ é¢
 {% endcomment %} {% block title %}
-{% endblock %} {% block top_toolbar %} {% comment %} top_toolbar start {%
-endcomment %}
+{% endblock %} {% block top_nav %} {% endblock %} {% block head %} {% endblock
+%} {% block top_toolbar %} {% comment %} top_toolbar start {% endcomment %}
     * _H_o_m_e
     * _U_p_d_a_t_e
-{% comment %} top_toolbar end {% endcomment %} {% endblock %} {% block top_nav
-%} {% endblock %} {% block head %} {% endblock %} {% comment %} article_list
-start {% endcomment %} {% block article_list %}
-    * {% for detail in object_list %}
-    * _{_{_d_e_t_a_i_l_._t_i_t_l_e_|_t_r_u_n_c_a_t_e_c_h_a_r_s_:_1_2_8_}_}
-    * {% endfor %}
-{% endblock %} {% comment %} article_list end {% endcomment %}
+{% comment %} top_toolbar end {% endcomment %} {% endblock %} {% comment %}
+article_list start {% endcomment %} {% block article_list %} {% for detail in
+object_list %} {%if detail.article_img%}
+[{{detail.product_name}}]
+{%endif%}
+_{_{_d_e_t_a_i_l_._t_i_t_l_e_|_t_r_u_n_c_a_t_e_c_h_a_r_s_:_4_8_}_}
+{% comment %} By _D_a_v_i_d_ _G_r_z_y_b, {% endcomment %} Published on {
+{detail.created_on}}
+{% comment %} éå¶ææ¬é¿åº¦ {% endcomment %} {
+{detail.content|truncatechars:128}}
+{% tags detail.tags 5 detail.pk %}
+{% related_post_by_tags_mini detail.tags 5 detail.pk %}
+{% endfor %} {% endblock %} {% comment %} article_list end {% endcomment %} {%
+block sidebar_section %}
+{% seo_top_links 50 %}
+{% autoescape off %} {% get_solo 'tbase_post.AmazonSettings' as amazon %} {%
+amazon_ads object.product_id detail.product_name amazon.store_id %} {% get_solo
+'tbase_post.AmazonSettings' as amz %} {% if amz.ads_sidebar %} {
+{amz.ads_sidebar}} {% endif %} {% endautoescape %} {% endblock %}
```

### Comparing `django_tbase_post_product-2024.5.117145788/tbase_post/templates/post/prompt_task_detail.html` & `django_tbase_post_product-2024.5.917151916/tbase_post/templates/post/prompt_task_detail.html`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2024.5.117145788/tbase_post/templates/post/prompt_task_post_detail.html` & `django_tbase_post_product-2024.5.917151916/tbase_post/templates/post/prompt_task_post_detail.html`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2024.5.117145788/tbase_post/templates/post/prompt_task_post_list.html` & `django_tbase_post_product-2024.5.917151916/tbase_post/templates/post/prompt_task_post_list.html`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2024.5.117145788/tbase_post/templates/post_list.html` & `django_tbase_post_product-2024.5.917151916/tbase_post/templates/post_list.html`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2024.5.117145788/tbase_post/templatetags/__pycache__/post_extras.cpython-310.pyc` & `django_tbase_post_product-2024.5.917151916/tbase_post/templatetags/__pycache__/post_extras.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Mar 12 16:23:05 2024 UTC, .py size: 11661 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-00000000: 6f0d 0d0a 0000 0000 6981 f065 8d2d 0000  o.......i..e.-..
+00000000: 6f0d 0d0a 0000 0000 e0a8 3b66 0731 0000  o.........;f.1..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0005 0000 0040 0000 0073 1202 0000 6400  .....@...s....d.
+00000020: 0005 0000 0040 0000 0073 3002 0000 6400  .....@...s0...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 0100 6400 6403 6c05  m.Z.m.Z...d.d.l.
 00000050: 6d05 5a06 0100 6400 6404 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 0100 6400 6405 6c07 6d09 5a09 0100 6400  ..d.d.l.m.Z...d.
 00000070: 6406 6c0a 6d0b 5a0b 0100 6400 6407 6c0c  d.l.m.Z...d.d.l.
 00000080: 6d0d 5a0d 0100 6400 6408 6c0e 5a0e 6400  m.Z...d.d.l.Z.d.
 00000090: 6409 6c0f 6d10 5a10 0100 6400 640a 6c02  d.l.m.Z...d.d.l.
@@ -12,383 +12,397 @@
 000000b0: 0100 6400 640c 6c07 6d14 5a14 0100 6400  ..d.d.l.m.Z...d.
 000000c0: 640d 6c15 6d16 5a16 6d17 5a17 0100 6400  d.l.m.Z.m.Z...d.
 000000d0: 640e 6c15 6d16 5a16 6d18 5a18 6d17 5a17  d.l.m.Z.m.Z.m.Z.
 000000e0: 6d19 5a19 0100 6501 a016 a100 5a1a 651a  m.Z...e.....Z.e.
 000000f0: 6a1b 640f 6410 8400 8301 5a1c 651a 6a1d  j.d.d.....Z.e.j.
 00000100: 6411 6412 8d01 6413 6414 8400 8301 5a1e  d.d...d.d.....Z.
 00000110: 651a 6a1b 651a 6a1f 6415 6416 6412 8d02  e.j.e.j.d.d.d...
-00000120: 6438 6417 6418 8401 8301 8301 5a20 651a  d8d.d.......Z e.
-00000130: 6a1b 651a 6a1f 6419 6416 6412 8d02 6438  j.e.j.d.d.d...d8
+00000120: 643b 6417 6418 8401 8301 8301 5a20 651a  d;d.d.......Z e.
+00000130: 6a1b 651a 6a1f 6419 6416 6412 8d02 643b  j.e.j.d.d.d...d;
 00000140: 641a 641b 8401 8301 8301 5a21 651a 6a1d  d.d.......Z!e.j.
-00000150: 6416 6412 8d01 6438 641c 641d 8401 8301  d.d...d8d.d.....
+00000150: 6416 6412 8d01 643b 641c 641d 8401 8301  d.d...d;d.d.....
 00000160: 5a22 641e 641f 8400 5a23 651a 6a1d 6416  Z"d.d...Z#e.j.d.
-00000170: 6412 8d01 6439 6421 6422 8401 8301 5a24  d...d9d!d"....Z$
+00000170: 6412 8d01 643c 6421 6422 8401 8301 5a24  d...d<d!d"....Z$
 00000180: 651a 6a1b 651a 6a1f 6423 6416 6412 8d02  e.j.e.j.d#d.d...
-00000190: 643a 6424 6425 8401 8301 8301 5a25 0900  d:d$d%......Z%..
+00000190: 643d 6424 6425 8401 8301 8301 5a25 0900  d=d$d%......Z%..
 000001a0: 651a 6a1f 6426 6416 6412 8d02 6700 6408  e.j.d&d.d...g.d.
 000001b0: 6408 6603 6427 6428 8401 8301 5a26 651a  d.f.d'd(....Z&e.
-000001c0: 6a1f 6429 6416 6412 8d02 643a 642a 642b  j.d)d.d...d:d*d+
-000001d0: 8401 8301 5a27 651a 6a1f 642c 6416 6412  ....Z'e.j.d,d.d.
-000001e0: 8d02 643a 642d 642e 8401 8301 5a28 651a  ..d:d-d.....Z(e.
-000001f0: 6a1f 642f 6416 6412 8d02 643b 6430 6431  j.d/d.d...d;d0d1
-00000200: 8401 8301 5a29 651a 6a1f 6432 6416 6412  ....Z)e.j.d2d.d.
-00000210: 8d02 643b 6433 6434 8401 8301 5a2a 651a  ..d;d3d4....Z*e.
-00000220: 6a1b 651a 6a1f 6435 6416 6412 8d02 6438  j.e.j.d5d.d...d8
-00000230: 6436 6437 8401 8301 8301 5a2b 6408 5300  d6d7......Z+d.S.
-00000240: 293c e900 0000 0029 01da 0874 656d 706c  )<.....)...templ
-00000250: 6174 6529 02da 0450 6f73 74da 044c 696e  ate)...Post..Lin
-00000260: 6b29 01da 0670 7072 696e 7429 01da 0146  k)...pprint)...F
-00000270: 2901 da05 436f 756e 7429 01da 0d63 6163  )...Count)...cac
-00000280: 6865 5f63 6f6e 7472 6f6c 2901 da05 6361  he_control)...ca
-00000290: 6368 654e 2901 da10 7265 6e64 6572 5f74  cheN)...render_t
-000002a0: 6f5f 7374 7269 6e67 2901 da0c 506f 7374  o_string)...Post
-000002b0: 5365 7474 696e 6773 2901 da0a 6974 656d  Settings)...item
-000002c0: 6765 7474 6572 2901 da01 5129 02da 074c  getter)...Q)...L
-000002d0: 6962 7261 7279 da08 5465 6d70 6c61 7465  ibrary..Template
-000002e0: 2904 720e 0000 00da 044e 6f64 6572 0f00  ).r......Noder..
-000002f0: 0000 da07 436f 6e74 6578 7463 0200 0000  ....Contextc....
-00000300: 0000 0000 0000 0000 0200 0000 0400 0000  ................
-00000310: 4300 0000 730c 0000 007c 00a0 007c 0164  C...s....|...|.d
-00000320: 01a1 0253 0029 027a 2f52 656d 6f76 6573  ...S.).z/Removes
-00000330: 2061 6c6c 2076 616c 7565 7320 6f66 2061   all values of a
-00000340: 7267 2066 726f 6d20 7468 6520 6769 7665  rg from the give
-00000350: 6e20 7374 7269 6e67 da00 2901 da07 7265  n string..)...re
-00000360: 706c 6163 6529 02da 0576 616c 7565 da03  place)...value..
-00000370: 6172 67a9 0072 1600 0000 fa6a 2f68 6f6d  arg..r.....j/hom
-00000380: 652f 7465 7272 792f 6d69 6e69 636f 6e64  e/terry/minicond
-00000390: 6133 2f65 6e76 732f 6663 5f70 706f 6e6e  a3/envs/fc_pponn
-000003a0: 6574 2f6c 6962 2f70 7974 686f 6e33 2e31  et/lib/python3.1
-000003b0: 302f 7369 7465 2d70 6163 6b61 6765 732f  0/site-packages/
-000003c0: 7462 6173 655f 706f 7374 2f74 656d 706c  tbase_post/templ
-000003d0: 6174 6574 6167 732f 706f 7374 5f65 7874  atetags/post_ext
-000003e0: 7261 732e 7079 da03 6375 7419 0000 0073  ras.py..cut....s
-000003f0: 0200 0000 0c03 7218 0000 0054 2901 5a0d  ......r....T).Z.
-00000400: 7461 6b65 735f 636f 6e74 6578 7463 0200  takes_contextc..
-00000410: 0000 0000 0000 0000 0000 0500 0000 0300  ................
-00000420: 0000 4f00 0000 7312 0000 0074 007c 0183  ..O...s....t.|..
-00000430: 017d 047c 04a0 017c 00a1 0153 0029 0175  .}.|...|...S.).u
-00000440: aa00 0000 0a20 20e6 b8b2 e69f 93e6 a8a1  .....  .........
-00000450: e69d bfe5 8685 e5ae b9e4 b8ba 2048 544d  ............ HTM
-00000460: 4ce3 8082 0a0a 2020 e4bd bfe7 94a8 e7a4  L.....  ........
-00000470: bae4 be8b 0a20 207b 2520 7265 6e64 6572  .....  {% render
-00000480: 5f68 746d 6c20 7072 6f6d 7074 2e74 656d  _html prompt.tem
-00000490: 706c 2070 6f73 743d 706f 7374 2070 726f  pl post=post pro
-000004a0: 6d70 743d 7072 6f6d 7074 2020 257d 0a20  mpt=prompt  %}. 
-000004b0: 207b 2520 7265 6e64 6572 5f68 746d 6c20   {% render_html 
-000004c0: e6a8 a1e6 9dbf 20e5 8f82 e695 b031 3de5  ...... ......1=.
-000004d0: 8f82 e695 b031 20e5 8f82 e695 b032 3de5  .....1 ......2=.
-000004e0: 8f82 e695 b032 2020 257d 0a0a 2020 2902  .....2  %}..  ).
-000004f0: 720f 0000 00da 0672 656e 6465 7229 05da  r......render)..
-00000500: 0763 6f6e 7465 7874 7202 0000 00da 0461  .contextr......a
-00000510: 7267 73da 066b 7761 7267 73da 0174 7216  rgs..kwargs..tr.
-00000520: 0000 0072 1600 0000 7217 0000 00da 0b72  ...r....r......r
-00000530: 656e 6465 725f 6874 6d6c 1f00 0000 7304  ender_html....s.
-00000540: 0000 0008 0f0a 0172 1e00 0000 7a1c 706f  .......r....z.po
-00000550: 7374 2f65 7874 7261 732f 616d 617a 6f6e  st/extras/amazon
-00000560: 5f6c 696e 6b2e 6874 6d6c 4663 0300 0000  _link.htmlFc....
-00000570: 0000 0000 0000 0000 0500 0000 0700 0000  ................
-00000580: 4f00 0000 f31a 0000 007c 007c 027c 0164  O........|.|.|.d
-00000590: 017c 009b 0064 027c 029b 009d 0464 039c  .|...d.|.....d..
-000005a0: 0453 00a9 04f5 3100 0000 0a20 2020 2020  .S....1....     
-000005b0: e794 9fe6 8890 e4ba 9ae9 a9ac e980 8ae6  ................
-000005c0: 8ea8 e5b9 bfe7 9a84 6261 6e6e 6572 e993  ........banner..
-000005d0: bee6 8ea5 0a0a 0a20 2020 20fa 1a68 7474  .......    ..htt
-000005e0: 7073 3a2f 2f77 7777 2e61 6d61 7a6f 6e2e  ps://www.amazon.
-000005f0: 636f 6d2f 6470 2ffa 062f 3f74 6167 3d29  com/dp/../?tag=)
-00000600: 04da 0a70 726f 6475 6374 5f69 64da 0873  ...product_id..s
-00000610: 746f 7265 5f69 64da 0c70 726f 6475 6374  tore_id..product
-00000620: 5f6e 616d 65da 046c 696e 6b72 1600 0000  _name..linkr....
-00000630: a905 7224 0000 0072 2600 0000 7225 0000  ..r$...r&...r%..
-00000640: 0072 1b00 0000 721c 0000 0072 1600 0000  .r....r....r....
-00000650: 7216 0000 0072 1700 0000 da0b 616d 617a  r....r......amaz
-00000660: 6f6e 5f6c 696e 6b35 0000 00f3 0a00 0000  on_link5........
-00000670: 0209 0201 0201 0e02 06fb 7229 0000 007a  ..........r)...z
-00000680: 1b70 6f73 742f 6578 7472 6173 2f61 6d61  .post/extras/ama
-00000690: 7a6f 6e5f 6164 732e 6874 6d6c 6303 0000  zon_ads.htmlc...
-000006a0: 0000 0000 0000 0000 0005 0000 0007 0000  ................
-000006b0: 004f 0000 0072 1f00 0000 7220 0000 0072  .O...r....r ...r
-000006c0: 1600 0000 7228 0000 0072 1600 0000 7216  ....r(...r....r.
-000006d0: 0000 0072 1700 0000 da0a 616d 617a 6f6e  ...r......amazon
-000006e0: 5f61 6473 4a00 0000 722a 0000 0072 2b00  _adsJ...r*...r+.
-000006f0: 0000 6303 0000 0000 0000 0000 0000 0005  ..c.............
-00000700: 0000 0004 0000 004f 0000 0073 1000 0000  .......O...s....
-00000710: 6401 7c00 9b00 6402 7c02 9b00 9d04 5300  d.|...d.|.....S.
-00000720: 2903 7221 0000 0072 2200 0000 7223 0000  ).r!...r"...r#..
-00000730: 0072 1600 0000 7228 0000 0072 1600 0000  .r....r(...r....
-00000740: 7216 0000 0072 1700 0000 da10 616d 617a  r....r......amaz
-00000750: 6f6e 5f62 6173 655f 6c69 6e6b 5a00 0000  on_base_linkZ...
-00000760: 7302 0000 0010 0872 2c00 0000 6301 0000  s......r,...c...
-00000770: 0000 0000 0000 0000 0005 0000 0005 0000  ................
-00000780: 0043 0000 0073 9c00 0000 6401 a000 7401  .C...s....d...t.
-00000790: 7c00 a002 a100 8301 a101 7d01 6402 7c01  |.........}.d.|.
-000007a0: 9b00 9d02 7d01 7403 a004 7c01 a101 7d02  ....}.t...|...}.
-000007b0: 7c02 6403 7501 7219 7c02 5300 7403 a004  |.d.u.r.|.S.t...
-000007c0: 6404 a101 7d03 7c03 6403 7500 7236 7c00  d...}.|.d.u.r6|.
-000007d0: 6a05 6a06 a007 6405 a101 6a08 7409 6405  j.j...d...j.t.d.
-000007e0: 8301 6406 8d01 7d03 7403 a00a 6404 7c03  ..d...}.t...d.|.
-000007f0: 6407 a103 0100 6900 7d02 7c03 4400 5d0a  d.....i.}.|.D.].
-00000800: 7d04 7c04 6408 1900 7c02 7c04 6405 1900  }.|.d...|.|.d...
-00000810: 3c00 713a 7403 a00a 7c01 7c02 6407 a103  <.q:t...|.|.d...
-00000820: 0100 7c02 5300 2909 7537 0000 000a 2020  ..|.S.).u7....  
-00000830: 2020 e5b0 86e6 a087 e7ad bee6 95b0 e987    ..............
-00000840: 8fe6 b7bb e58a a0e5 88b0 e6af 8fe4 b8aa  ................
-00000850: e6a0 87e7 adbe e5af b9e8 b1a1 e4b8 ad0a  ................
-00000860: 2020 2020 fa01 2d5a 1074 6167 735f 7769      ..-Z.tags_wi
-00000870: 7468 5f63 6f75 6e74 5f4e da0f 7461 6773  th_count_N..tags
-00000880: 5f77 6974 685f 636f 756e 745a 0774 6167  _with_countZ.tag
-00000890: 5f5f 706b 2901 da05 636f 756e 7469 8051  __pk)...counti.Q
-000008a0: 0100 722f 0000 0029 0bda 046a 6f69 6eda  ..r/...)...join.
-000008b0: 046c 6973 74da 0573 6c75 6773 7209 0000  .list..slugsr...
-000008c0: 00da 0367 6574 5a07 7468 726f 7567 68da  ...getZ.through.
-000008d0: 076f 626a 6563 7473 da06 7661 6c75 6573  .objects..values
-000008e0: 5a08 616e 6e6f 7461 7465 7207 0000 00da  Z.annotater.....
-000008f0: 0373 6574 2905 da04 7461 6773 da03 6b65  .set)...tags..ke
-00000900: 795a 1474 6167 735f 7769 7468 5f63 6f75  yZ.tags_with_cou
-00000910: 6e74 5f64 6963 7472 2e00 0000 da03 7461  nt_dictr......ta
-00000920: 6772 1600 0000 7216 0000 0072 1700 0000  gr....r....r....
-00000930: 722e 0000 0064 0000 0073 1c00 0000 1204  r....d...s......
-00000940: 0a01 0a02 0801 0401 0a07 0801 1a01 0e02  ................
-00000950: 0406 0801 1201 0e02 0401 722e 0000 00e9  ..........r.....
-00000960: 0500 0000 6302 0000 0000 0000 0000 0000  ....c...........
-00000970: 0008 0000 0004 0000 004f 0000 0073 4e00  .........O...sN.
-00000980: 0000 7400 7c00 8301 7d04 6700 7d05 6401  ..t.|...}.g.}.d.
-00000990: 7d06 7c00 a001 a100 4400 5d12 7d07 7c06  }.|.....D.].}.|.
-000009a0: 7c01 6b04 7214 0100 6e0b 7c05 a002 7c07  |.k.r...n.|...|.
-000009b0: 6a03 a101 0100 7c06 6402 1700 7d06 710c  j.....|.d...}.q.
-000009c0: 7c05 6403 a004 7c05 a101 6404 9c02 5300  |.d...|...d...S.
-000009d0: 2905 754e 0000 000a 2020 2020 e88e b7e5  ).uN....    ....
-000009e0: 8f96 e6a0 87e7 adbe e79a 84e5 908d e7a7  ................
-000009f0: b0ef bc8c e999 90e5 88b6 e8be 93e5 87ba  ................
-00000a00: e4b8 aae6 95b0 2ce5 8faf e4bb a5e7 94a8  ......,.........
-00000a10: e4ba 8e6b 6579 776f 7264 e8be 93e5 87ba  ...keyword......
-00000a20: 0a20 2020 2072 0100 0000 e901 0000 00fa  .    r..........
-00000a30: 012c 2902 da05 6e61 6d65 735a 0a6e 616d  .,)...namesZ.nam
-00000a40: 6573 5f74 6578 7429 0572 2e00 0000 da03  es_text).r......
-00000a50: 616c 6cda 0661 7070 656e 64da 046e 616d  all..append..nam
-00000a60: 6572 3000 0000 2908 7237 0000 00da 056c  er0...).r7.....l
-00000a70: 696d 6974 721b 0000 0072 1c00 0000 da10  imitr....r......
-00000a80: 6974 656d 735f 7769 7468 5f63 6f75 6e74  items_with_count
-00000a90: 723d 0000 00da 0169 da04 6974 656d 7216  r=.....i..itemr.
-00000aa0: 0000 0072 1600 0000 7217 0000 00da 0974  ...r....r......t
-00000ab0: 6167 5f6e 616d 6573 8700 0000 7316 0000  ag_names....s...
-00000ac0: 0008 0804 0204 010c 0108 0204 010c 030a  ................
-00000ad0: 0102 0608 0106 ff72 4500 0000 7a15 706f  .......rE...z.po
-00000ae0: 7374 2f65 7874 7261 732f 7461 6773 2e68  st/extras/tags.h
-00000af0: 746d 6c63 0300 0000 0000 0000 0000 0000  tmlc............
-00000b00: 0a00 0000 0800 0000 4f00 0000 7372 0000  ........O...sr..
-00000b10: 0074 007c 0083 017d 0567 007d 0664 017d  .t.|...}.g.}.d.}
-00000b20: 077c 00a0 01a1 0044 005d 1c7d 087c 077c  .|.....D.].}.|.|
-00000b30: 016b 0472 1401 006e 157c 06a0 027c 086a  .k.r...n.|...|.j
-00000b40: 037c 086a 047c 05a0 057c 086a 04a1 017c  .|.j.|...|.j...|
-00000b50: 0864 029c 04a1 0101 007c 0764 0317 007d  .d.......|.d...}
-00000b60: 0771 0c64 04a0 0674 077c 00a0 08a1 0083  .q.d...t.|......
-00000b70: 01a1 017d 0964 057c 067c 007c 0964 069c  ...}.d.|.|.|.d..
-00000b80: 0453 0029 074e 7201 0000 0029 0472 4000  .S.).Nr....).r@.
-00000b90: 0000 da02 706b 722f 0000 00da 066f 626a  ....pkr/.....obj
-00000ba0: 6563 7472 3b00 0000 722d 0000 007a 0554  ectr;...r-...z.T
-00000bb0: 6167 733a 2904 da05 7469 746c 65da 0569  ags:)...title..i
-00000bc0: 7465 6d73 7237 0000 0072 4600 0000 2909  temsr7...rF...).
-00000bd0: 722e 0000 0072 3e00 0000 723f 0000 0072  r....r>...r?...r
-00000be0: 4000 0000 7246 0000 0072 3300 0000 7230  @...rF...r3...r0
-00000bf0: 0000 0072 3100 0000 7232 0000 0029 0a72  ...r1...r2...).r
-00000c00: 3700 0000 7241 0000 0072 4600 0000 721b  7...rA...rF...r.
-00000c10: 0000 0072 1c00 0000 7242 0000 0072 4900  ...r....rB...rI.
-00000c20: 0000 7243 0000 0072 4400 0000 7238 0000  ..rC...rD...r8..
-00000c30: 0072 1600 0000 7216 0000 0072 1700 0000  .r....r....r....
-00000c40: 7237 0000 00a6 0000 0073 2600 0000 0806  r7.......s&.....
-00000c50: 0401 0401 0c01 0801 0401 0403 0401 0401  ................
-00000c60: 0a01 0201 08fc 0a07 1203 0202 0202 0201  ................
-00000c70: 0201 06fb 7237 0000 007a 2570 6f73 742f  ....r7...z%post/
-00000c80: 6578 7472 6173 2f72 656c 6174 6564 5f70  extras/related_p
-00000c90: 6f73 745f 6279 5f74 6167 732e 6874 6d6c  ost_by_tags.html
-00000ca0: 6303 0000 0000 0000 0000 0000 0007 0000  c...............
-00000cb0: 000a 0000 0043 0000 0073 7600 0000 7400  .....C...sv...t.
-00000cc0: a001 a100 7d03 7c03 6a02 7d01 7a1a 6401  ....}.|.j.}.z.d.
-00000cd0: a003 7404 7c00 a005 a100 8301 a101 7d04  ..t.|.........}.
-00000ce0: 7c00 a006 a100 6400 7c01 8502 1900 7d05  |.....d.|.....}.
-00000cf0: 6402 6403 6404 7c05 7c04 6405 9c05 5700  d.d.d.|.|.d...W.
-00000d00: 5300 0400 7407 793a 0100 7d06 0100 7a0d  S...t.y:..}...z.
-00000d10: 6406 6403 6404 6700 6407 9c04 5700 0600  d.d.d.g.d...W...
-00000d20: 5900 6400 7d06 7e06 5300 6400 7d06 7e06  Y.d.}.~.S.d.}.~.
-00000d30: 7701 7700 2908 4e72 2d00 0000 54fa 1463  w.w.).Nr-...T..c
-00000d40: 6f6e 7465 7874 5b27 686f 6d65 5f6c 696e  ontext['home_lin
-00000d50: 6b27 5d7a 0f52 656c 6174 6564 2043 6f6e  k']z.Related Con
-00000d60: 7465 6e74 a905 da05 7374 6174 6572 2700  tent....stater'.
-00000d70: 0000 7248 0000 00da 0870 6167 655f 6f62  ..rH.....page_ob
-00000d80: 6a72 4600 0000 4629 0472 4c00 0000 7227  jrF...F).rL...r'
-00000d90: 0000 0072 4800 0000 724d 0000 0029 0872  ...rH...rM...).r
-00000da0: 0b00 0000 da08 6765 745f 736f 6c6f 5a12  ......get_soloZ.
-00000db0: 7265 6c61 7465 645f 706f 7374 5f6c 696d  related_post_lim
-00000dc0: 6974 7230 0000 0072 3100 0000 7232 0000  itr0...r1...r2..
-00000dd0: 005a 0f73 696d 696c 6172 5f6f 626a 6563  .Z.similar_objec
-00000de0: 7473 da09 4578 6365 7074 696f 6e29 0772  ts..Exception).r
-00000df0: 3700 0000 7241 0000 00da 0a65 7863 6c75  7...rA.....exclu
-00000e00: 6465 5f70 6bda 0663 6f6e 6669 6772 3800  de_pk..configr8.
-00000e10: 0000 724d 0000 00da 0165 7216 0000 0072  ..rM.....er....r
-00000e20: 1600 0000 7217 0000 00da 1472 656c 6174  ....r......relat
-00000e30: 6564 5f70 6f73 745f 6279 5f74 6167 73d5  ed_post_by_tags.
-00000e40: 0000 0073 2600 0000 0804 0601 0201 1202  ...s&...........
-00000e50: 1001 020c 0201 0201 0201 0201 08fb 0e08  ................
-00000e60: 0203 0201 0201 0201 12fc 0880 02fe 7253  ..............rS
-00000e70: 0000 007a 1c70 6f73 742f 6578 7472 6173  ...z.post/extras
-00000e80: 2f6c 6173 745f 7570 6461 7465 2e68 746d  /last_update.htm
-00000e90: 6c63 0200 0000 0000 0000 0000 0000 0500  lc..............
-00000ea0: 0000 0a00 0000 4300 0000 73b0 0000 0074  ......C...s....t
-00000eb0: 00a0 01a1 007d 027c 026a 027d 007a 367c  .....}.|.j.}.z6|
-00000ec0: 0164 016b 0272 1f74 036a 04a0 0574 0664  .d.k.r.t.j...t.d
-00000ed0: 0264 038d 01a1 01a0 0764 04a1 01a0 08a1  .d.......d......
-00000ee0: 0064 017c 0085 0219 007d 036e 1674 036a  .d.|.....}.n.t.j
-00000ef0: 04a0 0574 0664 0264 038d 01a1 016a 097c  ...t.d.d.....j.|
-00000f00: 0164 058d 01a0 0764 04a1 01a0 08a1 0064  .d.....d.......d
-00000f10: 017c 0085 0219 007d 0364 0664 0764 087c  .|.....}.d.d.d.|
-00000f20: 0364 0964 0a9c 0557 0053 0004 0074 0a79  .d.d...W.S...t.y
-00000f30: 5701 007d 0401 007a 0e64 0b64 0764 0867  W..}...z.d.d.d.g
-00000f40: 0064 0964 0a9c 0557 0006 0059 0064 017d  .d.d...W...Y.d.}
-00000f50: 047e 0453 0064 017d 047e 0477 0177 0029  .~.S.d.}.~.w.w.)
-00000f60: 0c7a 0f0a 2020 2020 0a20 2020 200a 2020  .z..    .    .  
-00000f70: 2020 4e5a 0970 7562 6c69 7368 6564 2901    NZ.published).
-00000f80: 5a0e 7075 626c 6973 685f 7374 6174 7573  Z.publish_status
-00000f90: fa0b 2d75 7064 6174 6564 5f6f 6e29 0172  ..-updated_on).r
-00000fa0: 4600 0000 5472 4a00 0000 7a0b 4c61 7374  F...TrJ...z.Last
-00000fb0: 2055 7064 6174 65da 0b6c 6173 745f 7570   Update..last_up
-00000fc0: 6461 7465 724b 0000 0046 290b 720b 0000  daterK...F).r...
-00000fd0: 0072 4e00 0000 5a11 6c61 7374 5f75 7064  .rN...Z.last_upd
-00000fe0: 6174 655f 6c69 6d69 7472 0300 0000 7234  ate_limitr....r4
-00000ff0: 0000 00da 0666 696c 7465 7272 0d00 0000  .....filterr....
-00001000: da08 6f72 6465 725f 6279 da08 6469 7374  ..order_by..dist
-00001010: 696e 6374 da07 6578 636c 7564 6572 4f00  inct..excluderO.
-00001020: 0000 2905 7241 0000 0072 5000 0000 7251  ..).rA...rP...rQ
-00001030: 0000 0072 4d00 0000 7252 0000 0072 1600  ...rM...rR...r..
-00001040: 0000 7216 0000 0072 1700 0000 7255 0000  ..r....r....rU..
-00001050: 00fb 0000 0073 3200 0000 0807 0601 0201  .....s2.........
-00001060: 0802 2601 1202 0201 04ff 1001 04ff 0205  ..&.............
-00001070: 0201 0201 0201 0201 08fb 0e08 0203 0201  ................
-00001080: 0201 0201 0201 12fb 0880 02fe 7255 0000  ............rU..
-00001090: 007a 1e70 6f73 742f 6578 7472 6173 2f73  .z.post/extras/s
-000010a0: 656f 5f74 6f70 5f6c 696e 6b73 2e68 746d  eo_top_links.htm
-000010b0: 6c63 0200 0000 0000 0000 0000 0000 0400  lc..............
-000010c0: 0000 0a00 0000 4300 0000 7364 0000 007a  ......C...sd...z
-000010d0: 1774 006a 01a0 02a1 00a0 0364 01a1 01a0  .t.j.......d....
-000010e0: 04a1 0064 027c 0085 0219 007d 0264 0364  ...d.|.....}.d.d
-000010f0: 0464 057c 0264 0664 079c 0557 0053 0004  .d.|.d.d...W.S..
-00001100: 0074 0579 3101 007d 0301 007a 0e64 0864  .t.y1..}...z.d.d
-00001110: 0464 0567 0064 0964 079c 0557 0006 0059  .d.g.d.d...W...Y
-00001120: 0064 027d 037e 0353 0064 027d 037e 0377  .d.}.~.S.d.}.~.w
-00001130: 0177 0029 0a75 2e00 0000 0a20 2020 200a  .w.).u.....    .
-00001140: 2020 2020 e794 a8e4 ba8e e690 9ce7 b4a2      ............
-00001150: e4bc 98e5 8c96 20e5 8685 e983 a8e9 93be  ...... .........
-00001160: e68e a50a 2020 2020 7254 0000 004e 5472  ....    rT...NTr
-00001170: 4a00 0000 7a09 546f 7020 4c69 6e6b 73da  J...z.Top Links.
-00001180: 0d73 656f 5f74 6f70 5f6c 696e 6b73 724b  .seo_top_linksrK
-00001190: 0000 0046 5a18 6c61 7374 5f75 7064 7365  ...FZ.last_updse
-000011a0: 6f5f 746f 705f 6c69 6e6b 7361 7465 2906  o_top_linksate).
-000011b0: 7204 0000 0072 3400 0000 723e 0000 0072  r....r4...r>...r
-000011c0: 5700 0000 7258 0000 0072 4f00 0000 2904  W...rX...rO...).
-000011d0: 7241 0000 0072 5000 0000 724d 0000 0072  rA...rP...rM...r
-000011e0: 5200 0000 7216 0000 0072 1600 0000 7217  R...r....r....r.
-000011f0: 0000 0072 5a00 0000 2601 0000 7322 0000  ...rZ...&...s"..
-00001200: 0002 081c 0202 0202 0102 0102 0102 0108  ................
-00001210: fb0e 0802 0302 0102 0102 0102 0112 fb08  ................
-00001220: 8002 fe72 5a00 0000 7a22 706f 7374 2f65  ...rZ...z"post/e
-00001230: 7874 7261 732f 6869 7463 6f75 6e74 5f74  xtras/hitcount_t
-00001240: 6f70 5f70 6f73 742e 6874 6d6c 6303 0000  op_post.htmlc...
-00001250: 0000 0000 0000 0000 0006 0000 000a 0000  ................
-00001260: 0043 0000 00f3 7800 0000 7a21 7c01 6401  .C....x...z!|.d.
-00001270: 1600 7d03 7400 6a01 a002 a100 a003 6402  ..}.t.j.......d.
-00001280: a101 a004 a100 7c03 7c00 1400 7c03 6403  ......|.|...|.d.
-00001290: 1700 7c00 1400 8502 1900 7d04 6404 6405  ..|.......}.d.d.
-000012a0: 6406 7c04 6407 6408 9c05 5700 5300 0400  d.|.d.d...W.S...
-000012b0: 7405 793b 0100 7d05 0100 7a0e 6409 6405  t.y;..}...z.d.d.
-000012c0: 6406 6700 6407 6408 9c05 5700 0600 5900  d.g.d.d...W...Y.
-000012d0: 640a 7d05 7e05 5300 640a 7d05 7e05 7701  d.}.~.S.d.}.~.w.
-000012e0: 7700 290b 757f 0000 000a 2020 2020 0a20  w.).u.....    . 
-000012f0: 2020 20e7 94a8 e4ba 8ee6 909c e7b4 a2e4     .............
-00001300: bc98 e58c 9620 e586 85e9 83a8 e993 bee6  ..... ..........
-00001310: 8ea5 20e5 9bba e5ae 9ae4 bc98 e58c 96ef  .. .............
-00001320: bc8c e59f bae4 ba8e e78e b0e6 9c89 e79a  ................
-00001330: 84e6 b581 e987 8fe7 bb9f e8ae a10a 2020  ..............  
-00001340: 2020 e4bc 98e5 8c96 746f 7020 6c69 6d69    ......top limi
-00001350: 742a 3130 e4bb a5e5 8685 e79a 84e9 93be  t*10............
-00001360: e68e a50a 2020 2020 e90a 0000 007a 182d  ....    .....z.-
-00001370: 6869 745f 636f 756e 745f 6765 6e65 7269  hit_count_generi
-00001380: 635f 5f68 6974 7372 3b00 0000 5472 4a00  c__hitsr;...TrJ.
-00001390: 0000 5a03 486f 74da 1168 6974 636f 756e  ..Z.Hot..hitcoun
-000013a0: 745f 746f 705f 706f 7374 724b 0000 0046  t_top_postrK...F
-000013b0: 4ea9 0672 0300 0000 7234 0000 0072 3e00  N..r....r4...r>.
-000013c0: 0000 7257 0000 0072 5800 0000 724f 0000  ..rW...rX...rO..
-000013d0: 00a9 0672 4100 0000 5a07 6261 7365 5f69  ...rA...Z.base_i
-000013e0: 6472 5000 0000 da03 6269 6472 4d00 0000  drP.....bidrM...
-000013f0: 7252 0000 0072 1600 0000 7216 0000 0072  rR...r....r....r
-00001400: 1700 0000 725d 0000 004a 0100 00f3 2400  ....r]...J....$.
-00001410: 0000 0209 0802 2801 0206 0201 0201 0201  ......(.........
-00001420: 0201 08fb 0e08 0203 0201 0201 0201 0201  ................
-00001430: 12fb 0880 02fe 725d 0000 007a 2570 6f73  ......r]...z%pos
-00001440: 742f 6578 7472 6173 2f68 6974 636f 756e  t/extras/hitcoun
-00001450: 745f 6c6f 7765 7374 5f70 6f73 742e 6874  t_lowest_post.ht
-00001460: 6d6c 6303 0000 0000 0000 0000 0000 0006  mlc.............
-00001470: 0000 000a 0000 0043 0000 0072 5b00 0000  .......C...r[...
-00001480: 290b 7591 0000 000a 2020 2020 0a20 2020  ).u.....    .   
-00001490: 20e7 94a8 e4ba 8ee6 909c e7b4 a2e4 bc98   ...............
-000014a0: e58c 9620 e586 85e9 83a8 e993 bee6 8ea5  ... ............
-000014b0: 20e5 9bba e5ae 9ae4 bc98 e58c 96ef bc8c   ...............
-000014c0: e59f bae4 ba8e e78e b0e6 9c89 e79a 84e6  ................
-000014d0: b581 e987 8fe7 bb9f e8ae a10a 2020 2020  ............    
-000014e0: e4bc 98e5 8c96 e8ae bfe9 97ae e69c 80e4  ................
-000014f0: bd8e e79a 84e5 8685 e5ae b920 6c69 6d69  ........... limi
-00001500: 742a 3130 e4bb a5e5 8685 e79a 84e9 93be  t*10............
-00001510: e68e a50a 2020 2020 725c 0000 005a 1768  ....    r\...Z.h
-00001520: 6974 5f63 6f75 6e74 5f67 656e 6572 6963  it_count_generic
-00001530: 5f5f 6869 7473 723b 0000 0054 724a 0000  __hitsr;...TrJ..
-00001540: 005a 0745 7870 6c6f 7265 da14 6869 7463  .Z.Explore..hitc
-00001550: 6f75 6e74 5f6c 6f77 6573 745f 706f 7374  ount_lowest_post
-00001560: 724b 0000 0046 4e72 5e00 0000 725f 0000  rK...FNr^...r_..
-00001570: 0072 1600 0000 7216 0000 0072 1700 0000  .r....r....r....
-00001580: 7262 0000 0071 0100 0072 6100 0000 7262  rb...q...ra...rb
-00001590: 0000 007a 1f70 6f73 742f 6578 7472 6173  ...z.post/extras
-000015a0: 2f79 6f75 7475 6265 5f70 6c61 7965 722e  /youtube_player.
-000015b0: 6874 6d6c 6303 0000 0000 0000 0000 0000  htmlc...........
-000015c0: 0005 0000 0003 0000 004f 0000 0073 1000  .........O...s..
-000015d0: 0000 7c00 6401 7c00 9b00 9d02 6402 9c02  ..|.d.|.....d...
-000015e0: 5300 2903 7221 0000 007a 2768 7474 7073  S.).r!...z'https
-000015f0: 3a2f 2f77 7777 2e79 6f75 7475 6265 2d6e  ://www.youtube-n
-00001600: 6f63 6f6f 6b69 652e 636f 6d2f 656d 6265  ocookie.com/embe
-00001610: 642f 2902 da0a 796f 7574 7562 655f 6964  d/)...youtube_id
-00001620: 7227 0000 0072 1600 0000 2905 7263 0000  r'...r....).rc..
-00001630: 0072 2600 0000 7225 0000 0072 1b00 0000  .r&...r%...r....
-00001640: 721c 0000 0072 1600 0000 7216 0000 0072  r....r....r....r
-00001650: 1700 0000 da0e 796f 7574 7562 655f 706c  ......youtube_pl
-00001660: 6179 6572 9901 0000 7306 0000 0002 0b08  ayer....s.......
-00001670: 0306 fc72 6400 0000 2903 4e4e 4e29 0172  ...rd...).NNN).r
-00001680: 3a00 0000 2902 723a 0000 004e 2903 723a  :...).r:...N).r:
-00001690: 0000 0072 0100 0000 4e29 2cda 0664 6a61  ...r....N),..dja
-000016a0: 6e67 6f72 0200 0000 5a11 7462 6173 655f  ngor....Z.tbase_
-000016b0: 706f 7374 2e6d 6f64 656c 7372 0300 0000  post.modelsr....
-000016c0: 7204 0000 0072 0500 0000 da02 7070 5a10  r....r......ppZ.
-000016d0: 646a 616e 676f 2e64 622e 6d6f 6465 6c73  django.db.models
-000016e0: 7206 0000 0072 0700 0000 5a1d 646a 616e  r....r....Z.djan
-000016f0: 676f 2e76 6965 7773 2e64 6563 6f72 6174  go.views.decorat
-00001700: 6f72 732e 6361 6368 6572 0800 0000 5a11  ors.cacher....Z.
-00001710: 646a 616e 676f 2e63 6f72 652e 6361 6368  django.core.cach
-00001720: 6572 0900 0000 da06 7261 6e64 6f6d 5a16  er......randomZ.
-00001730: 646a 616e 676f 2e74 656d 706c 6174 652e  django.template.
-00001740: 6c6f 6164 6572 720a 0000 0072 0b00 0000  loaderr....r....
-00001750: da08 6f70 6572 6174 6f72 720c 0000 0072  ..operatorr....r
-00001760: 0d00 0000 5a0f 646a 616e 676f 2e74 656d  ....Z.django.tem
-00001770: 706c 6174 6572 0e00 0000 720f 0000 0072  plater....r....r
-00001780: 1000 0000 7211 0000 00da 0872 6567 6973  ....r......regis
-00001790: 7465 7272 5600 0000 7218 0000 005a 0a73  terrV...r....Z.s
-000017a0: 696d 706c 655f 7461 6772 1e00 0000 5a0d  imple_tagr....Z.
-000017b0: 696e 636c 7573 696f 6e5f 7461 6772 2900  inclusion_tagr).
-000017c0: 0000 722b 0000 0072 2c00 0000 722e 0000  ..r+...r,...r...
-000017d0: 0072 4500 0000 7237 0000 0072 5300 0000  .rE...r7...rS...
-000017e0: 7255 0000 0072 5a00 0000 725d 0000 0072  rU...rZ...r]...r
-000017f0: 6200 0000 7264 0000 0072 1600 0000 7216  b...rd...r....r.
-00001800: 0000 0072 1600 0000 7217 0000 00da 083c  ...r....r......<
-00001810: 6d6f 6475 6c65 3e01 0000 0073 7200 0000  module>....sr...
-00001820: 0c00 1001 0c01 0c01 0c01 0c01 0c01 0801  ................
-00001830: 0c01 0c01 0c01 0c01 1002 1801 0802 0408  ................
-00001840: 0a01 0a05 0a01 0415 0c01 0e01 0413 0c01  ................
-00001850: 0e01 0a0e 0c02 0808 0a23 0c01 041e 0c01  .........#......
-00001860: 0e01 0222 060b 0201 04ff 1202 0624 0201  ...".........$..
-00001870: 04ff 0c02 0629 0201 04ff 0c02 0622 0201  .....)......."..
-00001880: 04ff 0c02 0625 0201 04ff 0c02 0426 0c01  .....%.......&..
-00001890: 1201                                     ..
+000001c0: 6a1f 6429 6416 6412 8d02 6700 6408 6408  j.d)d.d...g.d.d.
+000001d0: 6603 642a 642b 8401 8301 5a27 651a 6a1f  f.d*d+....Z'e.j.
+000001e0: 642c 6416 6412 8d02 643d 642d 642e 8401  d,d.d...d=d-d...
+000001f0: 8301 5a28 651a 6a1f 642f 6416 6412 8d02  ..Z(e.j.d/d.d...
+00000200: 643d 6430 6431 8401 8301 5a29 651a 6a1f  d=d0d1....Z)e.j.
+00000210: 6432 6416 6412 8d02 643e 6433 6434 8401  d2d.d...d>d3d4..
+00000220: 8301 5a2a 651a 6a1f 6435 6416 6412 8d02  ..Z*e.j.d5d.d...
+00000230: 643e 6436 6437 8401 8301 5a2b 651a 6a1b  d>d6d7....Z+e.j.
+00000240: 651a 6a1f 6438 6416 6412 8d02 643b 6439  e.j.d8d.d...d;d9
+00000250: 643a 8401 8301 8301 5a2c 6408 5300 293f  d:......Z,d.S.)?
+00000260: e900 0000 0029 01da 0874 656d 706c 6174  .....)...templat
+00000270: 6529 02da 0450 6f73 74da 044c 696e 6b29  e)...Post..Link)
+00000280: 01da 0670 7072 696e 7429 01da 0146 2901  ...pprint)...F).
+00000290: da05 436f 756e 7429 01da 0d63 6163 6865  ..Count)...cache
+000002a0: 5f63 6f6e 7472 6f6c 2901 da05 6361 6368  _control)...cach
+000002b0: 654e 2901 da10 7265 6e64 6572 5f74 6f5f  eN)...render_to_
+000002c0: 7374 7269 6e67 2901 da0c 506f 7374 5365  string)...PostSe
+000002d0: 7474 696e 6773 2901 da0a 6974 656d 6765  ttings)...itemge
+000002e0: 7474 6572 2901 da01 5129 02da 074c 6962  tter)...Q)...Lib
+000002f0: 7261 7279 da08 5465 6d70 6c61 7465 2904  rary..Template).
+00000300: 720e 0000 00da 044e 6f64 6572 0f00 0000  r......Noder....
+00000310: da07 436f 6e74 6578 7463 0200 0000 0000  ..Contextc......
+00000320: 0000 0000 0000 0200 0000 0400 0000 4300  ..............C.
+00000330: 0000 730c 0000 007c 00a0 007c 0164 01a1  ..s....|...|.d..
+00000340: 0253 0029 027a 2f52 656d 6f76 6573 2061  .S.).z/Removes a
+00000350: 6c6c 2076 616c 7565 7320 6f66 2061 7267  ll values of arg
+00000360: 2066 726f 6d20 7468 6520 6769 7665 6e20   from the given 
+00000370: 7374 7269 6e67 da00 2901 da07 7265 706c  string..)...repl
+00000380: 6163 6529 02da 0576 616c 7565 da03 6172  ace)...value..ar
+00000390: 67a9 0072 1600 0000 fa6a 2f68 6f6d 652f  g..r.....j/home/
+000003a0: 7465 7272 792f 6d69 6e69 636f 6e64 6133  terry/miniconda3
+000003b0: 2f65 6e76 732f 6663 5f70 706f 6e6e 6574  /envs/fc_pponnet
+000003c0: 2f6c 6962 2f70 7974 686f 6e33 2e31 302f  /lib/python3.10/
+000003d0: 7369 7465 2d70 6163 6b61 6765 732f 7462  site-packages/tb
+000003e0: 6173 655f 706f 7374 2f74 656d 706c 6174  ase_post/templat
+000003f0: 6574 6167 732f 706f 7374 5f65 7874 7261  etags/post_extra
+00000400: 732e 7079 da03 6375 7419 0000 0073 0200  s.py..cut....s..
+00000410: 0000 0c03 7218 0000 0054 2901 da0d 7461  ....r....T)...ta
+00000420: 6b65 735f 636f 6e74 6578 7463 0200 0000  kes_contextc....
+00000430: 0000 0000 0000 0000 0500 0000 0300 0000  ................
+00000440: 4f00 0000 7312 0000 0074 007c 0183 017d  O...s....t.|...}
+00000450: 047c 04a0 017c 00a1 0153 0029 0175 aa00  .|...|...S.).u..
+00000460: 0000 0a20 20e6 b8b2 e69f 93e6 a8a1 e69d  ...  ...........
+00000470: bfe5 8685 e5ae b9e4 b8ba 2048 544d 4ce3  .......... HTML.
+00000480: 8082 0a0a 2020 e4bd bfe7 94a8 e7a4 bae4  ....  ..........
+00000490: be8b 0a20 207b 2520 7265 6e64 6572 5f68  ...  {% render_h
+000004a0: 746d 6c20 7072 6f6d 7074 2e74 656d 706c  tml prompt.templ
+000004b0: 2070 6f73 743d 706f 7374 2070 726f 6d70   post=post promp
+000004c0: 743d 7072 6f6d 7074 2020 257d 0a20 207b  t=prompt  %}.  {
+000004d0: 2520 7265 6e64 6572 5f68 746d 6c20 e6a8  % render_html ..
+000004e0: a1e6 9dbf 20e5 8f82 e695 b031 3de5 8f82  .... ......1=...
+000004f0: e695 b031 20e5 8f82 e695 b032 3de5 8f82  ...1 ......2=...
+00000500: e695 b032 2020 257d 0a0a 2020 2902 720f  ...2  %}..  ).r.
+00000510: 0000 00da 0672 656e 6465 7229 05da 0763  .....render)...c
+00000520: 6f6e 7465 7874 7202 0000 00da 0461 7267  ontextr......arg
+00000530: 73da 066b 7761 7267 73da 0174 7216 0000  s..kwargs..tr...
+00000540: 0072 1600 0000 7217 0000 00da 0b72 656e  .r....r......ren
+00000550: 6465 725f 6874 6d6c 1f00 0000 7304 0000  der_html....s...
+00000560: 0008 0f0a 0172 1f00 0000 7a1c 706f 7374  .....r....z.post
+00000570: 2f65 7874 7261 732f 616d 617a 6f6e 5f6c  /extras/amazon_l
+00000580: 696e 6b2e 6874 6d6c 4663 0300 0000 0000  ink.htmlFc......
+00000590: 0000 0000 0000 0500 0000 0700 0000 4f00  ..............O.
+000005a0: 0000 f31a 0000 007c 007c 027c 0164 017c  .......|.|.|.d.|
+000005b0: 009b 0064 027c 029b 009d 0464 039c 0453  ...d.|.....d...S
+000005c0: 00a9 04f5 3100 0000 0a20 2020 2020 e794  ....1....     ..
+000005d0: 9fe6 8890 e4ba 9ae9 a9ac e980 8ae6 8ea8  ................
+000005e0: e5b9 bfe7 9a84 6261 6e6e 6572 e993 bee6  ......banner....
+000005f0: 8ea5 0a0a 0a20 2020 20fa 1a68 7474 7073  .....    ..https
+00000600: 3a2f 2f77 7777 2e61 6d61 7a6f 6e2e 636f  ://www.amazon.co
+00000610: 6d2f 6470 2ffa 062f 3f74 6167 3d29 04da  m/dp/../?tag=)..
+00000620: 0a70 726f 6475 6374 5f69 64da 0873 746f  .product_id..sto
+00000630: 7265 5f69 64da 0c70 726f 6475 6374 5f6e  re_id..product_n
+00000640: 616d 65da 046c 696e 6b72 1600 0000 a905  ame..linkr......
+00000650: 7225 0000 0072 2700 0000 7226 0000 0072  r%...r'...r&...r
+00000660: 1c00 0000 721d 0000 0072 1600 0000 7216  ....r....r....r.
+00000670: 0000 0072 1700 0000 da0b 616d 617a 6f6e  ...r......amazon
+00000680: 5f6c 696e 6b35 0000 00f3 0a00 0000 0209  _link5..........
+00000690: 0201 0201 0e02 06fb 722a 0000 007a 1b70  ........r*...z.p
+000006a0: 6f73 742f 6578 7472 6173 2f61 6d61 7a6f  ost/extras/amazo
+000006b0: 6e5f 6164 732e 6874 6d6c 6303 0000 0000  n_ads.htmlc.....
+000006c0: 0000 0000 0000 0005 0000 0007 0000 004f  ...............O
+000006d0: 0000 0072 2000 0000 7221 0000 0072 1600  ...r ...r!...r..
+000006e0: 0000 7229 0000 0072 1600 0000 7216 0000  ..r)...r....r...
+000006f0: 0072 1700 0000 da0a 616d 617a 6f6e 5f61  .r......amazon_a
+00000700: 6473 4a00 0000 722b 0000 0072 2c00 0000  dsJ...r+...r,...
+00000710: 6303 0000 0000 0000 0000 0000 0005 0000  c...............
+00000720: 0004 0000 004f 0000 0073 1000 0000 6401  .....O...s....d.
+00000730: 7c00 9b00 6402 7c02 9b00 9d04 5300 2903  |...d.|.....S.).
+00000740: 7222 0000 0072 2300 0000 7224 0000 0072  r"...r#...r$...r
+00000750: 1600 0000 7229 0000 0072 1600 0000 7216  ....r)...r....r.
+00000760: 0000 0072 1700 0000 da10 616d 617a 6f6e  ...r......amazon
+00000770: 5f62 6173 655f 6c69 6e6b 5a00 0000 7302  _base_linkZ...s.
+00000780: 0000 0010 0872 2d00 0000 6301 0000 0000  .....r-...c.....
+00000790: 0000 0000 0000 0005 0000 0005 0000 0043  ...............C
+000007a0: 0000 0073 9c00 0000 6401 a000 7401 7c00  ...s....d...t.|.
+000007b0: a002 a100 8301 a101 7d01 6402 7c01 9b00  ........}.d.|...
+000007c0: 9d02 7d01 7403 a004 7c01 a101 7d02 7c02  ..}.t...|...}.|.
+000007d0: 6403 7501 7219 7c02 5300 7403 a004 6404  d.u.r.|.S.t...d.
+000007e0: a101 7d03 7c03 6403 7500 7236 7c00 6a05  ..}.|.d.u.r6|.j.
+000007f0: 6a06 a007 6405 a101 6a08 7409 6405 8301  j...d...j.t.d...
+00000800: 6406 8d01 7d03 7403 a00a 6404 7c03 6407  d...}.t...d.|.d.
+00000810: a103 0100 6900 7d02 7c03 4400 5d0a 7d04  ....i.}.|.D.].}.
+00000820: 7c04 6408 1900 7c02 7c04 6405 1900 3c00  |.d...|.|.d...<.
+00000830: 713a 7403 a00a 7c01 7c02 6407 a103 0100  q:t...|.|.d.....
+00000840: 7c02 5300 2909 7537 0000 000a 2020 2020  |.S.).u7....    
+00000850: e5b0 86e6 a087 e7ad bee6 95b0 e987 8fe6  ................
+00000860: b7bb e58a a0e5 88b0 e6af 8fe4 b8aa e6a0  ................
+00000870: 87e7 adbe e5af b9e8 b1a1 e4b8 ad0a 2020  ..............  
+00000880: 2020 da01 2d5a 1074 6167 735f 7769 7468    ..-Z.tags_with
+00000890: 5f63 6f75 6e74 5f4e da0f 7461 6773 5f77  _count_N..tags_w
+000008a0: 6974 685f 636f 756e 745a 0774 6167 5f5f  ith_countZ.tag__
+000008b0: 706b 2901 da05 636f 756e 7469 8051 0100  pk)...counti.Q..
+000008c0: 7230 0000 0029 0bda 046a 6f69 6eda 046c  r0...)...join..l
+000008d0: 6973 74da 0573 6c75 6773 7209 0000 00da  ist..slugsr.....
+000008e0: 0367 6574 da07 7468 726f 7567 68da 076f  .get..through..o
+000008f0: 626a 6563 7473 da06 7661 6c75 6573 da08  bjects..values..
+00000900: 616e 6e6f 7461 7465 7207 0000 00da 0373  annotater......s
+00000910: 6574 2905 da04 7461 6773 da03 6b65 795a  et)...tags..keyZ
+00000920: 1474 6167 735f 7769 7468 5f63 6f75 6e74  .tags_with_count
+00000930: 5f64 6963 7472 2f00 0000 da03 7461 6772  _dictr/.....tagr
+00000940: 1600 0000 7216 0000 0072 1700 0000 722f  ....r....r....r/
+00000950: 0000 0064 0000 0073 1c00 0000 1204 0a01  ...d...s........
+00000960: 0a02 0801 0401 0a07 0801 1a01 0e02 0406  ................
+00000970: 0801 1201 0e02 0401 722f 0000 00e9 0500  ........r/......
+00000980: 0000 6302 0000 0000 0000 0000 0000 0008  ..c.............
+00000990: 0000 0004 0000 004f 0000 0073 4e00 0000  .......O...sN...
+000009a0: 7400 7c00 8301 7d04 6700 7d05 6401 7d06  t.|...}.g.}.d.}.
+000009b0: 7c00 a001 a100 4400 5d12 7d07 7c06 7c01  |.....D.].}.|.|.
+000009c0: 6b04 7214 0100 6e0b 7c05 a002 7c07 6a03  k.r...n.|...|.j.
+000009d0: a101 0100 7c06 6402 1700 7d06 710c 7c05  ....|.d...}.q.|.
+000009e0: 6403 a004 7c05 a101 6404 9c02 5300 2905  d...|...d...S.).
+000009f0: 754e 0000 000a 2020 2020 e88e b7e5 8f96  uN....    ......
+00000a00: e6a0 87e7 adbe e79a 84e5 908d e7a7 b0ef  ................
+00000a10: bc8c e999 90e5 88b6 e8be 93e5 87ba e4b8  ................
+00000a20: aae6 95b0 2ce5 8faf e4bb a5e7 94a8 e4ba  ....,...........
+00000a30: 8e6b 6579 776f 7264 e8be 93e5 87ba 0a20  .keyword....... 
+00000a40: 2020 2072 0100 0000 e901 0000 00fa 012c     r...........,
+00000a50: 2902 da05 6e61 6d65 735a 0a6e 616d 6573  )...namesZ.names
+00000a60: 5f74 6578 7429 0572 2f00 0000 da03 616c  _text).r/.....al
+00000a70: 6cda 0661 7070 656e 64da 046e 616d 6572  l..append..namer
+00000a80: 3100 0000 2908 723a 0000 00da 056c 696d  1...).r:.....lim
+00000a90: 6974 721c 0000 0072 1d00 0000 da10 6974  itr....r......it
+00000aa0: 656d 735f 7769 7468 5f63 6f75 6e74 7240  ems_with_countr@
+00000ab0: 0000 00da 0169 da04 6974 656d 7216 0000  .....i..itemr...
+00000ac0: 0072 1600 0000 7217 0000 00da 0974 6167  .r....r......tag
+00000ad0: 5f6e 616d 6573 8700 0000 7316 0000 0008  _names....s.....
+00000ae0: 0804 0204 010c 0108 0204 010c 030a 0102  ................
+00000af0: 0608 0106 ff72 4800 0000 7a15 706f 7374  .....rH...z.post
+00000b00: 2f65 7874 7261 732f 7461 6773 2e68 746d  /extras/tags.htm
+00000b10: 6c63 0300 0000 0000 0000 0000 0000 0a00  lc..............
+00000b20: 0000 0800 0000 4f00 0000 7372 0000 0074  ......O...sr...t
+00000b30: 007c 0083 017d 0567 007d 0664 017d 077c  .|...}.g.}.d.}.|
+00000b40: 00a0 01a1 0044 005d 1c7d 087c 077c 016b  .....D.].}.|.|.k
+00000b50: 0472 1401 006e 157c 06a0 027c 086a 037c  .r...n.|...|.j.|
+00000b60: 086a 047c 05a0 057c 086a 04a1 017c 0864  .j.|...|.j...|.d
+00000b70: 029c 04a1 0101 007c 0764 0317 007d 0771  .......|.d...}.q
+00000b80: 0c64 04a0 0674 077c 00a0 08a1 0083 01a1  .d...t.|........
+00000b90: 017d 0964 057c 067c 007c 0964 069c 0453  .}.d.|.|.|.d...S
+00000ba0: 0029 074e 7201 0000 0029 0472 4300 0000  .).Nr....).rC...
+00000bb0: da02 706b 7230 0000 00da 066f 626a 6563  ..pkr0.....objec
+00000bc0: 7472 3e00 0000 722e 0000 007a 0554 6167  tr>...r....z.Tag
+00000bd0: 733a 2904 da05 7469 746c 65da 0569 7465  s:)...title..ite
+00000be0: 6d73 723a 0000 0072 4900 0000 2909 722f  msr:...rI...).r/
+00000bf0: 0000 0072 4100 0000 7242 0000 0072 4300  ...rA...rB...rC.
+00000c00: 0000 7249 0000 0072 3400 0000 7231 0000  ..rI...r4...r1..
+00000c10: 0072 3200 0000 7233 0000 0029 0a72 3a00  .r2...r3...).r:.
+00000c20: 0000 7244 0000 0072 4900 0000 721c 0000  ..rD...rI...r...
+00000c30: 0072 1d00 0000 7245 0000 0072 4c00 0000  .r....rE...rL...
+00000c40: 7246 0000 0072 4700 0000 723b 0000 0072  rF...rG...r;...r
+00000c50: 1600 0000 7216 0000 0072 1700 0000 723a  ....r....r....r:
+00000c60: 0000 00a6 0000 0073 2600 0000 0806 0401  .......s&.......
+00000c70: 0401 0c01 0801 0401 0403 0401 0401 0a01  ................
+00000c80: 0201 08fc 0a07 1203 0202 0202 0201 0201  ................
+00000c90: 06fb 723a 0000 007a 2570 6f73 742f 6578  ..r:...z%post/ex
+00000ca0: 7472 6173 2f72 656c 6174 6564 5f70 6f73  tras/related_pos
+00000cb0: 745f 6279 5f74 6167 732e 6874 6d6c 6303  t_by_tags.htmlc.
+00000cc0: 0000 0000 0000 0000 0000 0007 0000 000a  ................
+00000cd0: 0000 0043 0000 00f3 7600 0000 7400 a001  ...C....v...t...
+00000ce0: a100 7d03 7c03 6a02 7d01 7a1a 6401 a003  ..}.|.j.}.z.d...
+00000cf0: 7404 7c00 a005 a100 8301 a101 7d04 7c00  t.|.........}.|.
+00000d00: a006 a100 6400 7c01 8502 1900 7d05 6402  ....d.|.....}.d.
+00000d10: 6403 6404 7c05 7c04 6405 9c05 5700 5300  d.d.|.|.d...W.S.
+00000d20: 0400 7407 793a 0100 7d06 0100 7a0d 6406  ..t.y:..}...z.d.
+00000d30: 6403 6404 6700 6407 9c04 5700 0600 5900  d.d.g.d...W...Y.
+00000d40: 6400 7d06 7e06 5300 6400 7d06 7e06 7701  d.}.~.S.d.}.~.w.
+00000d50: 7700 a908 4e72 2e00 0000 54fa 1463 6f6e  w...Nr....T..con
+00000d60: 7465 7874 5b27 686f 6d65 5f6c 696e 6b27  text['home_link'
+00000d70: 5d7a 0f52 656c 6174 6564 2043 6f6e 7465  ]z.Related Conte
+00000d80: 6e74 a905 da05 7374 6174 6572 2800 0000  nt....stater(...
+00000d90: 724b 0000 00da 0870 6167 655f 6f62 6a72  rK.....page_objr
+00000da0: 4900 0000 4629 0472 5100 0000 7228 0000  I...F).rQ...r(..
+00000db0: 0072 4b00 0000 7252 0000 00a9 0872 0b00  .rK...rR.....r..
+00000dc0: 0000 da08 6765 745f 736f 6c6f da12 7265  ....get_solo..re
+00000dd0: 6c61 7465 645f 706f 7374 5f6c 696d 6974  lated_post_limit
+00000de0: 7231 0000 0072 3200 0000 7233 0000 00da  r1...r2...r3....
+00000df0: 0f73 696d 696c 6172 5f6f 626a 6563 7473  .similar_objects
+00000e00: da09 4578 6365 7074 696f 6ea9 0772 3a00  ..Exception..r:.
+00000e10: 0000 7244 0000 00da 0a65 7863 6c75 6465  ..rD.....exclude
+00000e20: 5f70 6bda 0663 6f6e 6669 6772 3b00 0000  _pk..configr;...
+00000e30: 7252 0000 00da 0165 7216 0000 0072 1600  rR.....er....r..
+00000e40: 0000 7217 0000 00da 1472 656c 6174 6564  ..r......related
+00000e50: 5f70 6f73 745f 6279 5f74 6167 73d5 0000  _post_by_tags...
+00000e60: 0073 2600 0000 0804 0601 0201 1202 1001  .s&.............
+00000e70: 020c 0201 0201 0201 0201 08fb 0e08 0203  ................
+00000e80: 0201 0201 0201 12fc 0880 02fe 725c 0000  ............r\..
+00000e90: 007a 2a70 6f73 742f 6578 7472 6173 2f72  .z*post/extras/r
+00000ea0: 656c 6174 6564 5f70 6f73 745f 6279 5f74  elated_post_by_t
+00000eb0: 6167 735f 6d69 6e69 2e68 746d 6c63 0300  ags_mini.htmlc..
+00000ec0: 0000 0000 0000 0000 0000 0700 0000 0a00  ................
+00000ed0: 0000 4300 0000 724d 0000 0072 4e00 0000  ..C...rM...rN...
+00000ee0: 7253 0000 0072 5800 0000 7216 0000 0072  rS...rX...r....r
+00000ef0: 1600 0000 7217 0000 00da 1972 656c 6174  ....r......relat
+00000f00: 6564 5f70 6f73 745f 6279 5f74 6167 735f  ed_post_by_tags_
+00000f10: 6d69 6e69 fe00 0000 7326 0000 0008 0406  mini....s&......
+00000f20: 0102 0112 0210 0102 0302 0102 0102 0102  ................
+00000f30: 0108 fb0e 0802 0302 0102 0102 0112 fc08  ................
+00000f40: 8002 fe72 5d00 0000 7a1c 706f 7374 2f65  ...r]...z.post/e
+00000f50: 7874 7261 732f 6c61 7374 5f75 7064 6174  xtras/last_updat
+00000f60: 652e 6874 6d6c 6302 0000 0000 0000 0000  e.htmlc.........
+00000f70: 0000 0005 0000 000a 0000 0043 0000 0073  ...........C...s
+00000f80: b000 0000 7400 a001 a100 7d02 7c02 6a02  ....t.....}.|.j.
+00000f90: 7d00 7a36 7c01 6401 6b02 721f 7403 6a04  }.z6|.d.k.r.t.j.
+00000fa0: a005 7406 6402 6403 8d01 a101 a007 6404  ..t.d.d.......d.
+00000fb0: a101 a008 a100 6401 7c00 8502 1900 7d03  ......d.|.....}.
+00000fc0: 6e16 7403 6a04 a005 7406 6402 6403 8d01  n.t.j...t.d.d...
+00000fd0: a101 6a09 7c01 6405 8d01 a007 6404 a101  ..j.|.d.....d...
+00000fe0: a008 a100 6401 7c00 8502 1900 7d03 6406  ....d.|.....}.d.
+00000ff0: 6407 6408 7c03 6409 640a 9c05 5700 5300  d.d.|.d.d...W.S.
+00001000: 0400 740a 7957 0100 7d04 0100 7a0e 640b  ..t.yW..}...z.d.
+00001010: 6407 6408 6700 6409 640a 9c05 5700 0600  d.d.g.d.d...W...
+00001020: 5900 6401 7d04 7e04 5300 6401 7d04 7e04  Y.d.}.~.S.d.}.~.
+00001030: 7701 7700 290c 7a0f 0a20 2020 200a 2020  w.w.).z..    .  
+00001040: 2020 0a20 2020 204e da09 7075 626c 6973    .    N..publis
+00001050: 6865 6429 01da 0e70 7562 6c69 7368 5f73  hed)...publish_s
+00001060: 7461 7475 73fa 0b2d 7570 6461 7465 645f  tatus..-updated_
+00001070: 6f6e 2901 7249 0000 0054 724f 0000 007a  on).rI...TrO...z
+00001080: 0b4c 6173 7420 5570 6461 7465 da0b 6c61  .Last Update..la
+00001090: 7374 5f75 7064 6174 6572 5000 0000 4629  st_updaterP...F)
+000010a0: 0b72 0b00 0000 7254 0000 00da 116c 6173  .r....rT.....las
+000010b0: 745f 7570 6461 7465 5f6c 696d 6974 7203  t_update_limitr.
+000010c0: 0000 0072 3600 0000 da06 6669 6c74 6572  ...r6.....filter
+000010d0: 720d 0000 00da 086f 7264 6572 5f62 79da  r......order_by.
+000010e0: 0864 6973 7469 6e63 74da 0765 7863 6c75  .distinct..exclu
+000010f0: 6465 7257 0000 0029 0572 4400 0000 7259  derW...).rD...rY
+00001100: 0000 0072 5a00 0000 7252 0000 0072 5b00  ...rZ...rR...r[.
+00001110: 0000 7216 0000 0072 1600 0000 7217 0000  ..r....r....r...
+00001120: 0072 6100 0000 2001 0000 7332 0000 0008  .ra... ...s2....
+00001130: 0706 0102 0108 0226 0112 0202 0104 ff10  .......&........
+00001140: 0104 ff02 0502 0102 0102 0102 0108 fb0e  ................
+00001150: 0802 0302 0102 0102 0102 0112 fb08 8002  ................
+00001160: fe72 6100 0000 7a1e 706f 7374 2f65 7874  .ra...z.post/ext
+00001170: 7261 732f 7365 6f5f 746f 705f 6c69 6e6b  ras/seo_top_link
+00001180: 732e 6874 6d6c 6302 0000 0000 0000 0000  s.htmlc.........
+00001190: 0000 0004 0000 000a 0000 0043 0000 0073  ...........C...s
+000011a0: 6400 0000 7a17 7400 6a01 a002 a100 a003  d...z.t.j.......
+000011b0: 6401 a101 a004 a100 6402 7c00 8502 1900  d.......d.|.....
+000011c0: 7d02 6403 6404 6405 7c02 6406 6407 9c05  }.d.d.d.|.d.d...
+000011d0: 5700 5300 0400 7405 7931 0100 7d03 0100  W.S...t.y1..}...
+000011e0: 7a0e 6408 6404 6405 6700 6409 6407 9c05  z.d.d.d.g.d.d...
+000011f0: 5700 0600 5900 6402 7d03 7e03 5300 6402  W...Y.d.}.~.S.d.
+00001200: 7d03 7e03 7701 7700 290a 752e 0000 000a  }.~.w.w.).u.....
+00001210: 2020 2020 0a20 2020 20e7 94a8 e4ba 8ee6      .    .......
+00001220: 909c e7b4 a2e4 bc98 e58c 9620 e586 85e9  ........... ....
+00001230: 83a8 e993 bee6 8ea5 0a20 2020 2072 6000  .........    r`.
+00001240: 0000 4e54 724f 0000 007a 0954 6f70 204c  ..NTrO...z.Top L
+00001250: 696e 6b73 da0d 7365 6f5f 746f 705f 6c69  inks..seo_top_li
+00001260: 6e6b 7372 5000 0000 465a 186c 6173 745f  nksrP...FZ.last_
+00001270: 7570 6473 656f 5f74 6f70 5f6c 696e 6b73  updseo_top_links
+00001280: 6174 6529 0672 0400 0000 7236 0000 0072  ate).r....r6...r
+00001290: 4100 0000 7264 0000 0072 6500 0000 7257  A...rd...re...rW
+000012a0: 0000 0029 0472 4400 0000 7259 0000 0072  ...).rD...rY...r
+000012b0: 5200 0000 725b 0000 0072 1600 0000 7216  R...r[...r....r.
+000012c0: 0000 0072 1700 0000 7267 0000 004b 0100  ...r....rg...K..
+000012d0: 0073 2200 0000 0208 1c02 0202 0201 0201  .s".............
+000012e0: 0201 0201 08fb 0e08 0203 0201 0201 0201  ................
+000012f0: 0201 12fb 0880 02fe 7267 0000 007a 2270  ........rg...z"p
+00001300: 6f73 742f 6578 7472 6173 2f68 6974 636f  ost/extras/hitco
+00001310: 756e 745f 746f 705f 706f 7374 2e68 746d  unt_top_post.htm
+00001320: 6c63 0300 0000 0000 0000 0000 0000 0600  lc..............
+00001330: 0000 0a00 0000 4300 0000 f378 0000 007a  ......C....x...z
+00001340: 217c 0164 0116 007d 0374 006a 01a0 02a1  !|.d...}.t.j....
+00001350: 00a0 0364 02a1 01a0 04a1 007c 037c 0014  ...d.......|.|..
+00001360: 007c 0364 0317 007c 0014 0085 0219 007d  .|.d...|.......}
+00001370: 0464 0464 0564 067c 0464 0764 089c 0557  .d.d.d.|.d.d...W
+00001380: 0053 0004 0074 0579 3b01 007d 0501 007a  .S...t.y;..}...z
+00001390: 0e64 0964 0564 0667 0064 0764 089c 0557  .d.d.d.g.d.d...W
+000013a0: 0006 0059 0064 0a7d 057e 0553 0064 0a7d  ...Y.d.}.~.S.d.}
+000013b0: 057e 0577 0177 0029 0b75 7f00 0000 0a20  .~.w.w.).u..... 
+000013c0: 2020 200a 2020 2020 e794 a8e4 ba8e e690     .    ........
+000013d0: 9ce7 b4a2 e4bc 98e5 8c96 20e5 8685 e983  .......... .....
+000013e0: a8e9 93be e68e a520 e59b bae5 ae9a e4bc  ....... ........
+000013f0: 98e5 8c96 efbc 8ce5 9fba e4ba 8ee7 8eb0  ................
+00001400: e69c 89e7 9a84 e6b5 81e9 878f e7bb 9fe8  ................
+00001410: aea1 0a20 2020 20e4 bc98 e58c 9674 6f70  ...    ......top
+00001420: 206c 696d 6974 2a31 30e4 bba5 e586 85e7   limit*10.......
+00001430: 9a84 e993 bee6 8ea5 0a20 2020 20e9 0a00  .........    ...
+00001440: 0000 7a18 2d68 6974 5f63 6f75 6e74 5f67  ..z.-hit_count_g
+00001450: 656e 6572 6963 5f5f 6869 7473 723e 0000  eneric__hitsr>..
+00001460: 0054 724f 0000 005a 0348 6f74 da11 6869  .TrO...Z.Hot..hi
+00001470: 7463 6f75 6e74 5f74 6f70 5f70 6f73 7472  tcount_top_postr
+00001480: 5000 0000 464e a906 7203 0000 0072 3600  P...FN..r....r6.
+00001490: 0000 7241 0000 0072 6400 0000 7265 0000  ..rA...rd...re..
+000014a0: 0072 5700 0000 a906 7244 0000 005a 0762  .rW.....rD...Z.b
+000014b0: 6173 655f 6964 7259 0000 00da 0362 6964  ase_idrY.....bid
+000014c0: 7252 0000 0072 5b00 0000 7216 0000 0072  rR...r[...r....r
+000014d0: 1600 0000 7217 0000 0072 6a00 0000 6f01  ....r....rj...o.
+000014e0: 0000 f324 0000 0002 0908 0228 0102 0602  ...$.......(....
+000014f0: 0102 0102 0102 0108 fb0e 0802 0302 0102  ................
+00001500: 0102 0102 0112 fb08 8002 fe72 6a00 0000  ...........rj...
+00001510: 7a25 706f 7374 2f65 7874 7261 732f 6869  z%post/extras/hi
+00001520: 7463 6f75 6e74 5f6c 6f77 6573 745f 706f  tcount_lowest_po
+00001530: 7374 2e68 746d 6c63 0300 0000 0000 0000  st.htmlc........
+00001540: 0000 0000 0600 0000 0a00 0000 4300 0000  ............C...
+00001550: 7268 0000 0029 0b75 9100 0000 0a20 2020  rh...).u.....   
+00001560: 200a 2020 2020 e794 a8e4 ba8e e690 9ce7   .    ..........
+00001570: b4a2 e4bc 98e5 8c96 20e5 8685 e983 a8e9  ........ .......
+00001580: 93be e68e a520 e59b bae5 ae9a e4bc 98e5  ..... ..........
+00001590: 8c96 efbc 8ce5 9fba e4ba 8ee7 8eb0 e69c  ................
+000015a0: 89e7 9a84 e6b5 81e9 878f e7bb 9fe8 aea1  ................
+000015b0: 0a20 2020 20e4 bc98 e58c 96e8 aebf e997  .    ...........
+000015c0: aee6 9c80 e4bd 8ee7 9a84 e586 85e5 aeb9  ................
+000015d0: 206c 696d 6974 2a31 30e4 bba5 e586 85e7   limit*10.......
+000015e0: 9a84 e993 bee6 8ea5 0a20 2020 2072 6900  .........    ri.
+000015f0: 0000 da17 6869 745f 636f 756e 745f 6765  ....hit_count_ge
+00001600: 6e65 7269 635f 5f68 6974 7372 3e00 0000  neric__hitsr>...
+00001610: 5472 4f00 0000 5a07 4578 706c 6f72 65da  TrO...Z.Explore.
+00001620: 1468 6974 636f 756e 745f 6c6f 7765 7374  .hitcount_lowest
+00001630: 5f70 6f73 7472 5000 0000 464e 726b 0000  _postrP...FNrk..
+00001640: 0072 6c00 0000 7216 0000 0072 1600 0000  .rl...r....r....
+00001650: 7217 0000 0072 7000 0000 9601 0000 726e  r....rp.......rn
+00001660: 0000 0072 7000 0000 7a1f 706f 7374 2f65  ...rp...z.post/e
+00001670: 7874 7261 732f 796f 7574 7562 655f 706c  xtras/youtube_pl
+00001680: 6179 6572 2e68 746d 6c63 0300 0000 0000  ayer.htmlc......
+00001690: 0000 0000 0000 0500 0000 0300 0000 4f00  ..............O.
+000016a0: 0000 7310 0000 007c 0064 017c 009b 009d  ..s....|.d.|....
+000016b0: 0264 029c 0253 0029 0372 2200 0000 7a27  .d...S.).r"...z'
+000016c0: 6874 7470 733a 2f2f 7777 772e 796f 7574  https://www.yout
+000016d0: 7562 652d 6e6f 636f 6f6b 6965 2e63 6f6d  ube-nocookie.com
+000016e0: 2f65 6d62 6564 2f29 02da 0a79 6f75 7475  /embed/)...youtu
+000016f0: 6265 5f69 6472 2800 0000 7216 0000 0029  be_idr(...r....)
+00001700: 0572 7100 0000 7227 0000 0072 2600 0000  .rq...r'...r&...
+00001710: 721c 0000 0072 1d00 0000 7216 0000 0072  r....r....r....r
+00001720: 1600 0000 7217 0000 00da 0e79 6f75 7475  ....r......youtu
+00001730: 6265 5f70 6c61 7965 72be 0100 0073 0600  be_player....s..
+00001740: 0000 020b 0803 06fc 7272 0000 0029 034e  ........rr...).N
+00001750: 4e4e 2901 723d 0000 0029 0272 3d00 0000  NN).r=...).r=...
+00001760: 4e29 0372 3d00 0000 7201 0000 004e 292d  N).r=...r....N)-
+00001770: da06 646a 616e 676f 7202 0000 005a 1174  ..djangor....Z.t
+00001780: 6261 7365 5f70 6f73 742e 6d6f 6465 6c73  base_post.models
+00001790: 7203 0000 0072 0400 0000 7205 0000 00da  r....r....r.....
+000017a0: 0270 70da 1064 6a61 6e67 6f2e 6462 2e6d  .pp..django.db.m
+000017b0: 6f64 656c 7372 0600 0000 7207 0000 00da  odelsr....r.....
+000017c0: 1d64 6a61 6e67 6f2e 7669 6577 732e 6465  .django.views.de
+000017d0: 636f 7261 746f 7273 2e63 6163 6865 7208  corators.cacher.
+000017e0: 0000 00da 1164 6a61 6e67 6f2e 636f 7265  .....django.core
+000017f0: 2e63 6163 6865 7209 0000 00da 0672 616e  .cacher......ran
+00001800: 646f 6dda 1664 6a61 6e67 6f2e 7465 6d70  dom..django.temp
+00001810: 6c61 7465 2e6c 6f61 6465 7272 0a00 0000  late.loaderr....
+00001820: 720b 0000 00da 086f 7065 7261 746f 7272  r......operatorr
+00001830: 0c00 0000 720d 0000 00da 0f64 6a61 6e67  ....r......djang
+00001840: 6f2e 7465 6d70 6c61 7465 720e 0000 0072  o.templater....r
+00001850: 0f00 0000 7210 0000 0072 1100 0000 da08  ....r....r......
+00001860: 7265 6769 7374 6572 7263 0000 0072 1800  registerrc...r..
+00001870: 0000 da0a 7369 6d70 6c65 5f74 6167 721f  ....simple_tagr.
+00001880: 0000 00da 0d69 6e63 6c75 7369 6f6e 5f74  .....inclusion_t
+00001890: 6167 722a 0000 0072 2c00 0000 722d 0000  agr*...r,...r-..
+000018a0: 0072 2f00 0000 7248 0000 0072 3a00 0000  .r/...rH...r:...
+000018b0: 725c 0000 0072 5d00 0000 7261 0000 0072  r\...r]...ra...r
+000018c0: 6700 0000 726a 0000 0072 7000 0000 7272  g...rj...rp...rr
+000018d0: 0000 0072 1600 0000 7216 0000 0072 1600  ...r....r....r..
+000018e0: 0000 7217 0000 00da 083c 6d6f 6475 6c65  ..r......<module
+000018f0: 3e01 0000 0073 7a00 0000 0c00 1001 0c01  >....sz.........
+00001900: 0c01 0c01 0c01 0c01 0801 0c01 0c01 0c01  ................
+00001910: 0c01 1002 1801 0802 0408 0a01 0a05 0a01  ................
+00001920: 0415 0c01 0e01 0413 0c01 0e01 0a0e 0c02  ................
+00001930: 0808 0a23 0c01 041e 0c01 0e01 0222 060b  ...#........."..
+00001940: 0201 04ff 1202 0627 0201 04ff 1202 0620  .......'....... 
+00001950: 0201 04ff 0c02 0629 0201 04ff 0c02 0622  .......)......."
+00001960: 0201 04ff 0c02 0625 0201 04ff 0c02 0426  .......%.......&
+00001970: 0c01 1201                                ....
```

### Comparing `django_tbase_post_product-2024.5.117145788/tbase_post/templatetags/__pycache__/post_extras.cpython-39.pyc` & `django_tbase_post_product-2024.5.917151916/tbase_post/templatetags/__pycache__/post_extras.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2024.5.117145788/tbase_post/templatetags/post_extras.py` & `django_tbase_post_product-2024.5.917151916/tbase_post/templatetags/post_extras.py`

 * *Files 11% similar despite different names*

```diff
@@ -244,14 +244,107 @@
             'state': False,
             'link': "context['home_link']",
             'title': "Related Content",
             "page_obj": [],
             # "content": context
         }
 
+
+
+
+@register.inclusion_tag('post/extras/related_post_by_tags_mini.html',
+                        takes_context=False)
+def related_post_by_tags_mini(tags=[], limit=None,exclude_pk=None):
+
+    config = PostSettings.get_solo()
+    # limit=config.related_post_limit
+    try:
+        # page_obj=tags.similar_objects()[-limit:]
+        key = "-".join(list(tags.slugs()))
+        page_obj=tags.similar_objects()[:limit]
+
+        return {
+            'state': True,
+            'link': "context['home_link']",
+            'title': "Related Content",
+            "page_obj": page_obj,
+            "pk":key
+            # "content": context
+        }
+    except Exception as e:
+        # print(e)
+        return {
+            'state': False,
+            'link': "context['home_link']",
+            'title': "Related Content",
+            "page_obj": [],
+            # "content": context
+        }
+
+
+
+
+@register.inclusion_tag('post/extras/get_previous_next_by_pk.html',
+                        takes_context=False)
+def get_previous_next_by_pk(do_type="next",pk=0, limit=5):
+    """
+    关于函数get_previous_next_by_pk(do_type="previous",pk=0, limit=5)
+
+    do_type:
+    Fetches 'previous' or 'next' related posts based on primary key.
+    主题模板中使用
+    # 加载
+    
+    {% load post_extras %}
+
+    {% get_previous_next_by_pk "previous" 10 5 %}
+
+    {% get_previous_next_by_pk "next" 10 5 %}
+
+    """
+
+    try:
+        # operator = Q(pk__lt=pk) if do_type == 'previous' else Q(pk__gt=pk)
+        # queryset = Post.objects.filter(operator).order_by('pk')[:limit]
+        if do_type == 'previous':
+            operator=Q(pk__gt=pk)
+            queryset = Post.objects.filter(operator).order_by('pk')[:limit]
+        else:
+            operator=Q(pk__lt=pk)
+            queryset = Post.objects.filter(operator).order_by('-pk')[:limit]
+ 
+
+        return {
+            'state': True,
+            # 'link': "context['home_link']",
+            # 'title': "Related Content",
+            "page_obj": queryset,
+            "id":f"get_next_by_pk_{pk}"
+            # "content": context
+        }
+    except Exception as e:
+ 
+        return {
+            'state': False,
+            # 'link': "context['home_link']",
+            # 'title': "Related Content",
+            "page_obj": [],
+            "id":f"get_next_by_pk_{pk}"
+            # "content": context
+        }
+
+
+
+ 
+
+
+
+
+
+
 @register.inclusion_tag('post/extras/last_update.html',
                         takes_context=False)
 def last_update( limit=5,exclude_pk=None):
     """
     
     
     """
```

### Comparing `django_tbase_post_product-2024.5.117145788/tbase_post/urls.py` & `django_tbase_post_product-2024.5.917151916/tbase_post/urls.py`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2024.5.117145788/tbase_post/views.py` & `django_tbase_post_product-2024.5.917151916/tbase_post/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -300,14 +300,16 @@
         # print("kwargs",kwargs)
         # context = Post.objects.get(id=pk)
         context = super().get_context_data(**kwargs)
         # context['now'] = timezone.now()
         # context['title'] = "Post Details"
         # print(context)
         return context
+    
+    
 # @cache_page(60*2)
 class LastUpdateView(generic.ListView):
     """
     最后更新页面
     """
 
     # def get(self, request, *args, **kwargs):
```

