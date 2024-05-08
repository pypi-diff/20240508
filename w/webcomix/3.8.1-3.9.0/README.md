# Comparing `tmp/webcomix-3.8.1.tar.gz` & `tmp/webcomix-3.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webcomix-3.8.1.tar", max compression
+gzip compressed data, was "webcomix-3.9.0.tar", max compression
```

## Comparing `webcomix-3.8.1.tar` & `webcomix-3.9.0.tar`

### file list

```diff
@@ -1,59 +1,59 @@
--rw-r--r--   0        0        0     1069 2024-02-20 03:24:30.969756 webcomix-3.8.1/LICENSE
--rw-r--r--   0        0        0     4434 2024-02-20 03:24:30.969756 webcomix-3.8.1/README.md
--rw-r--r--   0        0        0     1344 2024-02-20 03:24:30.969756 webcomix-3.8.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-02-20 03:24:30.969756 webcomix-3.8.1/webcomix/__init__.py
--rw-r--r--   0        0        0     7436 2024-02-20 03:24:30.973756 webcomix-3.8.1/webcomix/cli.py
--rw-r--r--   0        0        0     7545 2024-02-20 03:24:30.973756 webcomix-3.8.1/webcomix/comic.py
--rw-r--r--   0        0        0     1273 2024-02-20 03:24:30.973756 webcomix-3.8.1/webcomix/docker.py
--rw-r--r--   0        0        0      216 2024-02-20 03:24:30.973756 webcomix-3.8.1/webcomix/exceptions.py
--rw-r--r--   0        0        0        0 2024-02-20 03:24:30.973756 webcomix-3.8.1/webcomix/scrapy/__init__.py
--rw-r--r--   0        0        0     1493 2024-02-20 03:24:30.973756 webcomix-3.8.1/webcomix/scrapy/crawler_worker.py
--rw-r--r--   0        0        0        0 2024-02-20 03:24:30.973756 webcomix-3.8.1/webcomix/scrapy/download/__init__.py
--rw-r--r--   0        0        0      154 2024-02-20 03:24:30.973756 webcomix-3.8.1/webcomix/scrapy/download/comic_page.py
--rw-r--r--   0        0        0     2131 2024-02-20 03:24:30.973756 webcomix-3.8.1/webcomix/scrapy/download/comic_pipeline.py
--rw-r--r--   0        0        0     2359 2024-02-20 03:24:30.973756 webcomix-3.8.1/webcomix/scrapy/download/comic_spider.py
--rw-r--r--   0        0        0        0 2024-02-20 03:24:30.973756 webcomix-3.8.1/webcomix/scrapy/download/tests/__init__.py
--rw-r--r--   0        0        0     3785 2024-02-20 03:24:30.973756 webcomix-3.8.1/webcomix/scrapy/download/tests/test_comic_pipeline.py
--rw-r--r--   0        0        0     4668 2024-02-20 03:24:30.973756 webcomix-3.8.1/webcomix/scrapy/download/tests/test_comic_spider.py
--rw-r--r--   0        0        0      387 2024-02-20 03:24:30.973756 webcomix-3.8.1/webcomix/scrapy/request_factory.py
--rw-r--r--   0        0        0        0 2024-02-20 03:24:30.973756 webcomix-3.8.1/webcomix/scrapy/tests/__init__.py
--rw-r--r--   0        0        0      701 2024-02-20 03:24:30.973756 webcomix-3.8.1/webcomix/scrapy/tests/test_crawler_worker.py
--rw-r--r--   0        0        0      566 2024-02-20 03:24:30.973756 webcomix-3.8.1/webcomix/scrapy/tests/test_request_factory.py
--rw-r--r--   0        0        0      410 2024-02-20 03:24:30.973756 webcomix-3.8.1/webcomix/scrapy/util.py
--rw-r--r--   0        0        0        0 2024-02-20 03:24:30.973756 webcomix-3.8.1/webcomix/scrapy/verification/__init__.py
--rw-r--r--   0        0        0     2591 2024-02-20 03:24:30.973756 webcomix-3.8.1/webcomix/scrapy/verification/verification_spider.py
--rw-r--r--   0        0        0      157 2024-02-20 03:24:30.973756 webcomix-3.8.1/webcomix/scrapy/verification/web_page.py
--rw-r--r--   0        0        0     2585 2024-02-20 03:24:30.973756 webcomix-3.8.1/webcomix/search.py
--rw-r--r--   0        0        0     6813 2024-02-20 03:24:30.973756 webcomix-3.8.1/webcomix/supported_comics.py
--rw-r--r--   0        0        0        1 2024-02-20 03:24:30.973756 webcomix-3.8.1/webcomix/tests/__init__.py
--rw-r--r--   0        0        0     1027 2024-02-20 03:24:30.973756 webcomix-3.8.1/webcomix/tests/fake_websites/fixture.py
--rw-r--r--   0        0        0      169 2024-02-20 03:24:30.973756 webcomix-3.8.1/webcomix/tests/fake_websites/one_webpage/1.html
--rw-r--r--   0        0        0    25483 2024-02-20 03:24:30.973756 webcomix-3.8.1/webcomix/tests/fake_websites/one_webpage/1.jpeg
--rw-r--r--   0        0        0    31690 2024-02-20 03:24:30.973756 webcomix-3.8.1/webcomix/tests/fake_websites/one_webpage/2.jpeg
--rw-r--r--   0        0        0      197 2024-02-20 03:24:30.973756 webcomix-3.8.1/webcomix/tests/fake_websites/one_webpage_searchable/1.html
--rw-r--r--   0        0        0    25483 2024-02-20 03:24:30.973756 webcomix-3.8.1/webcomix/tests/fake_websites/one_webpage_searchable/1.jpeg
--rw-r--r--   0        0        0    31690 2024-02-20 03:24:30.973756 webcomix-3.8.1/webcomix/tests/fake_websites/one_webpage_searchable/2.jpeg
--rw-r--r--   0        0        0      170 2024-02-20 03:24:30.973756 webcomix-3.8.1/webcomix/tests/fake_websites/three_webpages/1.html
--rw-r--r--   0        0        0    25483 2024-02-20 03:24:30.973756 webcomix-3.8.1/webcomix/tests/fake_websites/three_webpages/1.jpeg
--rw-r--r--   0        0        0      170 2024-02-20 03:24:30.973756 webcomix-3.8.1/webcomix/tests/fake_websites/three_webpages/2.html
--rw-r--r--   0        0        0    31690 2024-02-20 03:24:30.973756 webcomix-3.8.1/webcomix/tests/fake_websites/three_webpages/2.jpeg
--rw-r--r--   0        0        0      115 2024-02-20 03:24:30.973756 webcomix-3.8.1/webcomix/tests/fake_websites/three_webpages/3.html
--rw-r--r--   0        0        0      189 2024-02-20 03:24:30.973756 webcomix-3.8.1/webcomix/tests/fake_websites/three_webpages_alt_text/1.html
--rw-r--r--   0        0        0    25483 2024-02-20 03:24:30.973756 webcomix-3.8.1/webcomix/tests/fake_websites/three_webpages_alt_text/1.jpeg
--rw-r--r--   0        0        0      190 2024-02-20 03:24:30.973756 webcomix-3.8.1/webcomix/tests/fake_websites/three_webpages_alt_text/2.html
--rw-r--r--   0        0        0    31690 2024-02-20 03:24:30.973756 webcomix-3.8.1/webcomix/tests/fake_websites/three_webpages_alt_text/2.jpeg
--rw-r--r--   0        0        0      115 2024-02-20 03:24:30.977756 webcomix-3.8.1/webcomix/tests/fake_websites/three_webpages_alt_text/3.html
--rw-r--r--   0        0        0      197 2024-02-20 03:24:30.977756 webcomix-3.8.1/webcomix/tests/fake_websites/three_webpages_classes/1.html
--rw-r--r--   0        0        0    25483 2024-02-20 03:24:30.977756 webcomix-3.8.1/webcomix/tests/fake_websites/three_webpages_classes/1.jpeg
--rw-r--r--   0        0        0      197 2024-02-20 03:24:30.977756 webcomix-3.8.1/webcomix/tests/fake_websites/three_webpages_classes/2.html
--rw-r--r--   0        0        0    31690 2024-02-20 03:24:30.977756 webcomix-3.8.1/webcomix/tests/fake_websites/three_webpages_classes/2.jpeg
--rw-r--r--   0        0        0      205 2024-02-20 03:24:30.977756 webcomix-3.8.1/webcomix/tests/fake_websites/three_webpages_classes/3.html
--rw-r--r--   0        0        0    31690 2024-02-20 03:24:30.977756 webcomix-3.8.1/webcomix/tests/fake_websites/three_webpages_classes/3.jpeg
--rw-r--r--   0        0        0      115 2024-02-20 03:24:30.977756 webcomix-3.8.1/webcomix/tests/fake_websites/three_webpages_classes/4.html
--rw-r--r--   0        0        0    11637 2024-02-20 03:24:30.977756 webcomix-3.8.1/webcomix/tests/test_cli.py
--rw-r--r--   0        0        0    11323 2024-02-20 03:24:30.977756 webcomix-3.8.1/webcomix/tests/test_comic.py
--rw-r--r--   0        0        0      635 2024-02-20 03:24:30.977756 webcomix-3.8.1/webcomix/tests/test_comic_availability.py
--rw-r--r--   0        0        0      934 2024-02-20 03:24:30.977756 webcomix-3.8.1/webcomix/tests/test_docker.py
--rw-r--r--   0        0        0     4068 2024-02-20 03:24:30.977756 webcomix-3.8.1/webcomix/tests/test_search.py
--rw-r--r--   0        0        0      440 2024-02-20 03:24:30.977756 webcomix-3.8.1/webcomix/util.py
--rw-r--r--   0        0        0     5721 1970-01-01 00:00:00.000000 webcomix-3.8.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-02-20 04:12:43.112151 webcomix-3.9.0/LICENSE
+-rw-r--r--   0        0        0     4434 2024-02-20 04:12:43.112151 webcomix-3.9.0/README.md
+-rw-r--r--   0        0        0     1344 2024-02-20 04:12:43.112151 webcomix-3.9.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-02-20 04:12:43.112151 webcomix-3.9.0/webcomix/__init__.py
+-rw-r--r--   0        0        0     7611 2024-02-20 04:12:43.112151 webcomix-3.9.0/webcomix/cli.py
+-rw-r--r--   0        0        0     7545 2024-02-20 04:12:43.112151 webcomix-3.9.0/webcomix/comic.py
+-rw-r--r--   0        0        0     1273 2024-02-20 04:12:43.112151 webcomix-3.9.0/webcomix/docker.py
+-rw-r--r--   0        0        0      216 2024-02-20 04:12:43.112151 webcomix-3.9.0/webcomix/exceptions.py
+-rw-r--r--   0        0        0        0 2024-02-20 04:12:43.112151 webcomix-3.9.0/webcomix/scrapy/__init__.py
+-rw-r--r--   0        0        0     1493 2024-02-20 04:12:43.112151 webcomix-3.9.0/webcomix/scrapy/crawler_worker.py
+-rw-r--r--   0        0        0        0 2024-02-20 04:12:43.112151 webcomix-3.9.0/webcomix/scrapy/download/__init__.py
+-rw-r--r--   0        0        0      154 2024-02-20 04:12:43.112151 webcomix-3.9.0/webcomix/scrapy/download/comic_page.py
+-rw-r--r--   0        0        0     2131 2024-02-20 04:12:43.112151 webcomix-3.9.0/webcomix/scrapy/download/comic_pipeline.py
+-rw-r--r--   0        0        0     2359 2024-02-20 04:12:43.112151 webcomix-3.9.0/webcomix/scrapy/download/comic_spider.py
+-rw-r--r--   0        0        0        0 2024-02-20 04:12:43.112151 webcomix-3.9.0/webcomix/scrapy/download/tests/__init__.py
+-rw-r--r--   0        0        0     3785 2024-02-20 04:12:43.112151 webcomix-3.9.0/webcomix/scrapy/download/tests/test_comic_pipeline.py
+-rw-r--r--   0        0        0     4668 2024-02-20 04:12:43.112151 webcomix-3.9.0/webcomix/scrapy/download/tests/test_comic_spider.py
+-rw-r--r--   0        0        0      387 2024-02-20 04:12:43.112151 webcomix-3.9.0/webcomix/scrapy/request_factory.py
+-rw-r--r--   0        0        0        0 2024-02-20 04:12:43.112151 webcomix-3.9.0/webcomix/scrapy/tests/__init__.py
+-rw-r--r--   0        0        0      701 2024-02-20 04:12:43.112151 webcomix-3.9.0/webcomix/scrapy/tests/test_crawler_worker.py
+-rw-r--r--   0        0        0      566 2024-02-20 04:12:43.112151 webcomix-3.9.0/webcomix/scrapy/tests/test_request_factory.py
+-rw-r--r--   0        0        0      410 2024-02-20 04:12:43.112151 webcomix-3.9.0/webcomix/scrapy/util.py
+-rw-r--r--   0        0        0        0 2024-02-20 04:12:43.112151 webcomix-3.9.0/webcomix/scrapy/verification/__init__.py
+-rw-r--r--   0        0        0     2591 2024-02-20 04:12:43.112151 webcomix-3.9.0/webcomix/scrapy/verification/verification_spider.py
+-rw-r--r--   0        0        0      157 2024-02-20 04:12:43.112151 webcomix-3.9.0/webcomix/scrapy/verification/web_page.py
+-rw-r--r--   0        0        0     2653 2024-02-20 04:12:43.112151 webcomix-3.9.0/webcomix/search.py
+-rw-r--r--   0        0        0     6813 2024-02-20 04:12:43.116151 webcomix-3.9.0/webcomix/supported_comics.py
+-rw-r--r--   0        0        0        1 2024-02-20 04:12:43.116151 webcomix-3.9.0/webcomix/tests/__init__.py
+-rw-r--r--   0        0        0     1027 2024-02-20 04:12:43.116151 webcomix-3.9.0/webcomix/tests/fake_websites/fixture.py
+-rw-r--r--   0        0        0      169 2024-02-20 04:12:43.116151 webcomix-3.9.0/webcomix/tests/fake_websites/one_webpage/1.html
+-rw-r--r--   0        0        0    25483 2024-02-20 04:12:43.116151 webcomix-3.9.0/webcomix/tests/fake_websites/one_webpage/1.jpeg
+-rw-r--r--   0        0        0    31690 2024-02-20 04:12:43.116151 webcomix-3.9.0/webcomix/tests/fake_websites/one_webpage/2.jpeg
+-rw-r--r--   0        0        0      197 2024-02-20 04:12:43.116151 webcomix-3.9.0/webcomix/tests/fake_websites/one_webpage_searchable/1.html
+-rw-r--r--   0        0        0    25483 2024-02-20 04:12:43.116151 webcomix-3.9.0/webcomix/tests/fake_websites/one_webpage_searchable/1.jpeg
+-rw-r--r--   0        0        0    31690 2024-02-20 04:12:43.116151 webcomix-3.9.0/webcomix/tests/fake_websites/one_webpage_searchable/2.jpeg
+-rw-r--r--   0        0        0      170 2024-02-20 04:12:43.116151 webcomix-3.9.0/webcomix/tests/fake_websites/three_webpages/1.html
+-rw-r--r--   0        0        0    25483 2024-02-20 04:12:43.116151 webcomix-3.9.0/webcomix/tests/fake_websites/three_webpages/1.jpeg
+-rw-r--r--   0        0        0      170 2024-02-20 04:12:43.116151 webcomix-3.9.0/webcomix/tests/fake_websites/three_webpages/2.html
+-rw-r--r--   0        0        0    31690 2024-02-20 04:12:43.116151 webcomix-3.9.0/webcomix/tests/fake_websites/three_webpages/2.jpeg
+-rw-r--r--   0        0        0      115 2024-02-20 04:12:43.116151 webcomix-3.9.0/webcomix/tests/fake_websites/three_webpages/3.html
+-rw-r--r--   0        0        0      189 2024-02-20 04:12:43.116151 webcomix-3.9.0/webcomix/tests/fake_websites/three_webpages_alt_text/1.html
+-rw-r--r--   0        0        0    25483 2024-02-20 04:12:43.116151 webcomix-3.9.0/webcomix/tests/fake_websites/three_webpages_alt_text/1.jpeg
+-rw-r--r--   0        0        0      190 2024-02-20 04:12:43.116151 webcomix-3.9.0/webcomix/tests/fake_websites/three_webpages_alt_text/2.html
+-rw-r--r--   0        0        0    31690 2024-02-20 04:12:43.116151 webcomix-3.9.0/webcomix/tests/fake_websites/three_webpages_alt_text/2.jpeg
+-rw-r--r--   0        0        0      115 2024-02-20 04:12:43.116151 webcomix-3.9.0/webcomix/tests/fake_websites/three_webpages_alt_text/3.html
+-rw-r--r--   0        0        0      197 2024-02-20 04:12:43.116151 webcomix-3.9.0/webcomix/tests/fake_websites/three_webpages_classes/1.html
+-rw-r--r--   0        0        0    25483 2024-02-20 04:12:43.116151 webcomix-3.9.0/webcomix/tests/fake_websites/three_webpages_classes/1.jpeg
+-rw-r--r--   0        0        0      197 2024-02-20 04:12:43.116151 webcomix-3.9.0/webcomix/tests/fake_websites/three_webpages_classes/2.html
+-rw-r--r--   0        0        0    31690 2024-02-20 04:12:43.116151 webcomix-3.9.0/webcomix/tests/fake_websites/three_webpages_classes/2.jpeg
+-rw-r--r--   0        0        0      205 2024-02-20 04:12:43.116151 webcomix-3.9.0/webcomix/tests/fake_websites/three_webpages_classes/3.html
+-rw-r--r--   0        0        0    31690 2024-02-20 04:12:43.116151 webcomix-3.9.0/webcomix/tests/fake_websites/three_webpages_classes/3.jpeg
+-rw-r--r--   0        0        0      115 2024-02-20 04:12:43.116151 webcomix-3.9.0/webcomix/tests/fake_websites/three_webpages_classes/4.html
+-rw-r--r--   0        0        0    11637 2024-02-20 04:12:43.116151 webcomix-3.9.0/webcomix/tests/test_cli.py
+-rw-r--r--   0        0        0    11323 2024-02-20 04:12:43.116151 webcomix-3.9.0/webcomix/tests/test_comic.py
+-rw-r--r--   0        0        0      635 2024-02-20 04:12:43.116151 webcomix-3.9.0/webcomix/tests/test_comic_availability.py
+-rw-r--r--   0        0        0      934 2024-02-20 04:12:43.116151 webcomix-3.9.0/webcomix/tests/test_docker.py
+-rw-r--r--   0        0        0     5281 2024-02-20 04:12:43.116151 webcomix-3.9.0/webcomix/tests/test_search.py
+-rw-r--r--   0        0        0      440 2024-02-20 04:12:43.116151 webcomix-3.9.0/webcomix/util.py
+-rw-r--r--   0        0        0     5721 1970-01-01 00:00:00.000000 webcomix-3.9.0/PKG-INFO
```

### Comparing `webcomix-3.8.1/LICENSE` & `webcomix-3.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `webcomix-3.8.1/README.md` & `webcomix-3.9.0/README.md`

 * *Files identical despite different names*

### Comparing `webcomix-3.8.1/pyproject.toml` & `webcomix-3.9.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "webcomix"
-version = "3.8.1"
+version = "3.9.0"
 description = "Webcomic downloader"
 authors = ["Jean-Christophe Pelletier <pelletierj97@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/J-CPelletier/webcomix"
 homepage = "https://github.com/J-CPelletier/webcomix"
 license = "MIT"
 classifiers = [
```

### Comparing `webcomix-3.8.1/webcomix/cli.py` & `webcomix-3.9.0/webcomix/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,14 +54,21 @@
     "--start-url",
     "--start_url",
     prompt=True,
     type=click.STRING,
     help="URL of the comic's first page",
 )
 @click.option(
+    "--end-url",
+    "--end_url",
+    prompt=False,
+    type=click.STRING,
+    help="URL of the comic's last page",
+)
+@click.option(
     "--start-page",
     "--start_page",
     type=click.INT,
     default=1,
     help="Number of comic's first page to be downloaded",
 )
 @click.option(
@@ -97,14 +104,15 @@
 )
 @click.option(
     "--verbose", "-v", is_flag=True, default=False, help="Add debugging output"
 )
 def search(
     name,
     start_url,
+    end_url,
     start_page,
     cbz,
     single_page,
     javascript,
     title,
     alt_text,
     yes,
@@ -113,14 +121,15 @@
     """
     Downloads a webcomic using a general XPath
     """
     with DockerManager(javascript):
         comic, validation = discovery(
             name,
             start_url,
+            end_url=end_url,
             start_page=start_page,
             alt_text=alt_text,
             single_page=single_page,
             javascript=javascript,
             title=title,
             debug=verbose,
         )
```

### Comparing `webcomix-3.8.1/webcomix/comic.py` & `webcomix-3.9.0/webcomix/comic.py`

 * *Files identical despite different names*

### Comparing `webcomix-3.8.1/webcomix/docker.py` & `webcomix-3.9.0/webcomix/docker.py`

 * *Files identical despite different names*

### Comparing `webcomix-3.8.1/webcomix/scrapy/crawler_worker.py` & `webcomix-3.9.0/webcomix/scrapy/crawler_worker.py`

 * *Files identical despite different names*

### Comparing `webcomix-3.8.1/webcomix/scrapy/download/comic_pipeline.py` & `webcomix-3.9.0/webcomix/scrapy/download/comic_pipeline.py`

 * *Files identical despite different names*

### Comparing `webcomix-3.8.1/webcomix/scrapy/download/comic_spider.py` & `webcomix-3.9.0/webcomix/scrapy/download/comic_spider.py`

 * *Files identical despite different names*

### Comparing `webcomix-3.8.1/webcomix/scrapy/download/tests/test_comic_pipeline.py` & `webcomix-3.9.0/webcomix/scrapy/download/tests/test_comic_pipeline.py`

 * *Files identical despite different names*

### Comparing `webcomix-3.8.1/webcomix/scrapy/download/tests/test_comic_spider.py` & `webcomix-3.9.0/webcomix/scrapy/download/tests/test_comic_spider.py`

 * *Files identical despite different names*

### Comparing `webcomix-3.8.1/webcomix/scrapy/tests/test_crawler_worker.py` & `webcomix-3.9.0/webcomix/scrapy/tests/test_crawler_worker.py`

 * *Files identical despite different names*

### Comparing `webcomix-3.8.1/webcomix/scrapy/tests/test_request_factory.py` & `webcomix-3.9.0/webcomix/scrapy/tests/test_request_factory.py`

 * *Files identical despite different names*

### Comparing `webcomix-3.8.1/webcomix/scrapy/verification/verification_spider.py` & `webcomix-3.9.0/webcomix/scrapy/verification/verification_spider.py`

 * *Files identical despite different names*

### Comparing `webcomix-3.8.1/webcomix/search.py` & `webcomix-3.9.0/webcomix/search.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 possible_attributes_image = [".", "@src", "@class", "@id", "@alt"]
 possible_attributes_next = [".", "text()", "@class", "@id", "@alt", "@rel"]
 
 
 def discovery(
     name: str,
     url: str,
+    end_url: Optional[str] = None,
     start_page: int = 1,
     alt_text: Optional[str] = None,
     single_page: bool = False,
     javascript: bool = False,
     title: bool = False,
     debug: bool = False,
 ) -> Tuple[Optional[Comic], Optional[List[Mapping]]]:
@@ -62,14 +63,15 @@
         )
         try:
             comic = Comic(
                 name,
                 url,
                 image_xpath,
                 next_page_xpath,
+                end_url=end_url,
                 start_page=start_page,
                 alt_text=alt_text,
                 single_page=single_page,
                 javascript=javascript,
                 title=title,
                 debug=debug,
             )
```

### Comparing `webcomix-3.8.1/webcomix/supported_comics.py` & `webcomix-3.9.0/webcomix/supported_comics.py`

 * *Files identical despite different names*

### Comparing `webcomix-3.8.1/webcomix/tests/fake_websites/fixture.py` & `webcomix-3.9.0/webcomix/tests/fake_websites/fixture.py`

 * *Files identical despite different names*

### Comparing `webcomix-3.8.1/webcomix/tests/fake_websites/one_webpage/1.jpeg` & `webcomix-3.9.0/webcomix/tests/fake_websites/one_webpage/1.jpeg`

 * *Files identical despite different names*

### Comparing `webcomix-3.8.1/webcomix/tests/fake_websites/one_webpage/2.jpeg` & `webcomix-3.9.0/webcomix/tests/fake_websites/one_webpage/2.jpeg`

 * *Files identical despite different names*

### Comparing `webcomix-3.8.1/webcomix/tests/fake_websites/one_webpage_searchable/1.jpeg` & `webcomix-3.9.0/webcomix/tests/fake_websites/one_webpage_searchable/1.jpeg`

 * *Files identical despite different names*

### Comparing `webcomix-3.8.1/webcomix/tests/fake_websites/one_webpage_searchable/2.jpeg` & `webcomix-3.9.0/webcomix/tests/fake_websites/one_webpage_searchable/2.jpeg`

 * *Files identical despite different names*

### Comparing `webcomix-3.8.1/webcomix/tests/fake_websites/three_webpages/1.jpeg` & `webcomix-3.9.0/webcomix/tests/fake_websites/three_webpages/1.jpeg`

 * *Files identical despite different names*

### Comparing `webcomix-3.8.1/webcomix/tests/fake_websites/three_webpages/2.jpeg` & `webcomix-3.9.0/webcomix/tests/fake_websites/three_webpages/2.jpeg`

 * *Files identical despite different names*

### Comparing `webcomix-3.8.1/webcomix/tests/fake_websites/three_webpages_alt_text/1.jpeg` & `webcomix-3.9.0/webcomix/tests/fake_websites/three_webpages_alt_text/1.jpeg`

 * *Files identical despite different names*

### Comparing `webcomix-3.8.1/webcomix/tests/fake_websites/three_webpages_alt_text/2.jpeg` & `webcomix-3.9.0/webcomix/tests/fake_websites/three_webpages_alt_text/2.jpeg`

 * *Files identical despite different names*

### Comparing `webcomix-3.8.1/webcomix/tests/fake_websites/three_webpages_classes/1.jpeg` & `webcomix-3.9.0/webcomix/tests/fake_websites/three_webpages_classes/1.jpeg`

 * *Files identical despite different names*

### Comparing `webcomix-3.8.1/webcomix/tests/fake_websites/three_webpages_classes/2.jpeg` & `webcomix-3.9.0/webcomix/tests/fake_websites/three_webpages_classes/2.jpeg`

 * *Files identical despite different names*

### Comparing `webcomix-3.8.1/webcomix/tests/fake_websites/three_webpages_classes/3.jpeg` & `webcomix-3.9.0/webcomix/tests/fake_websites/three_webpages_classes/3.jpeg`

 * *Files identical despite different names*

### Comparing `webcomix-3.8.1/webcomix/tests/test_cli.py` & `webcomix-3.9.0/webcomix/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `webcomix-3.8.1/webcomix/tests/test_comic.py` & `webcomix-3.9.0/webcomix/tests/test_comic.py`

 * *Files identical despite different names*

### Comparing `webcomix-3.8.1/webcomix/tests/test_comic_availability.py` & `webcomix-3.9.0/webcomix/tests/test_comic_availability.py`

 * *Files identical despite different names*

### Comparing `webcomix-3.8.1/webcomix/tests/test_docker.py` & `webcomix-3.9.0/webcomix/tests/test_docker.py`

 * *Files identical despite different names*

### Comparing `webcomix-3.8.1/webcomix/tests/test_search.py` & `webcomix-3.9.0/webcomix/tests/test_search.py`

 * *Files 18% similar despite different names*

```diff
@@ -47,14 +47,40 @@
     ]
 
     assert comic.start_url == expected.start_url
     assert comic.next_page_selector == expected.next_page_selector
     assert comic.comic_image_selector == expected.comic_image_selector
 
 
+def test_search_searchable_website_adds_end_url(mocker, three_webpages_classes_uri):
+    three_webpages_classes_folder = three_webpages_classes_uri.strip("1.html")
+
+    expected = Comic(
+        "Blindsprings",
+        three_webpages_classes_uri,
+        "//*[contains(translate(@class, 'ABCDEFGHIJKLMNOPQRSTUVWXYZ','abcdefghijklmnopqrstuvwxyz'), 'comic')]//@src",
+        "//*[contains(translate(@class, 'ABCDEFGHIJKLMNOPQRSTUVWXYZ','abcdefghijklmnopqrstuvwxyz'), 'next')]//@href",
+        end_url=three_webpages_classes_folder + "2.html",
+    )
+    mocker.patch("webcomix.search.possible_image_xpath", ["comic"])
+    mocker.patch("webcomix.search.possible_next_page_xpath", ["next"])
+    mocker.patch("webcomix.search.possible_tags_image", ["*"])
+    mocker.patch("webcomix.search.possible_tags_next", ["*"])
+    mocker.patch("webcomix.search.possible_attributes_image", ["@class"])
+    mocker.patch("webcomix.search.possible_attributes_next", ["@class"])
+    mocker.patch("webcomix.util.check_first_pages")
+    comic, result = discovery(
+        "Blindsprings",
+        three_webpages_classes_uri,
+        end_url=three_webpages_classes_folder + "2.html",
+    )
+
+    assert comic.end_url == expected.end_url
+
+
 def test_search_unsearchable_website(mocker, three_webpages_uri):
     mocker.patch("webcomix.search.possible_image_xpath", ["comic"])
     mocker.patch("webcomix.search.possible_next_page_xpath", ["next"])
     mocker.patch("webcomix.search.possible_tags_image", ["*"])
     mocker.patch("webcomix.search.possible_tags_next", ["*"])
     mocker.patch("webcomix.search.possible_attributes_image", ["@class"])
     mocker.patch("webcomix.search.possible_attributes_next", ["@class"])
```

### Comparing `webcomix-3.8.1/PKG-INFO` & `webcomix-3.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webcomix
-Version: 3.8.1
+Version: 3.9.0
 Summary: Webcomic downloader
 Home-page: https://github.com/J-CPelletier/webcomix
 License: MIT
 Author: Jean-Christophe Pelletier
 Author-email: pelletierj97@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

