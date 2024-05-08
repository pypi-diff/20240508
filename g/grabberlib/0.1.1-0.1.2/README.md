# Comparing `tmp/grabberlib-0.1.1.tar.gz` & `tmp/grabberlib-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grabberlib-0.1.1.tar", max compression
+gzip compressed data, was "grabberlib-0.1.2.tar", max compression
```

## Comparing `grabberlib-0.1.1.tar` & `grabberlib-0.1.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0        0 2024-05-03 14:50:36.715508 grabberlib-0.1.1/README.md
--rw-r--r--   0        0        0        1 2024-05-03 14:50:36.716140 grabberlib-0.1.1/assets/pages.txt
--rw-r--r--   0        0        0        0 2024-05-03 14:50:36.718507 grabberlib-0.1.1/grabber/__init__.py
--rw-r--r--   0        0        0     1690 2024-05-03 14:50:36.718702 grabberlib-0.1.1/grabber/__main__.py
--rw-r--r--   0        0        0        0 2024-05-03 14:50:36.718877 grabberlib-0.1.1/grabber/controllers/__init__.py
--rw-r--r--   0        0        0     5057 2024-05-08 12:59:24.763016 grabberlib-0.1.1/grabber/controllers/base.py
--rw-r--r--   0        0        0        0 2024-05-03 14:50:36.719286 grabberlib-0.1.1/grabber/core/__init__.py
--rw-r--r--   0        0        0        0 2024-05-03 14:50:36.719467 grabberlib-0.1.1/grabber/core/bot/__init__.py
--rw-r--r--   0        0        0      997 2024-05-08 13:00:46.779103 grabberlib-0.1.1/grabber/core/bot/core.py
--rw-r--r--   0        0        0       65 2024-05-03 14:50:36.719818 grabberlib-0.1.1/grabber/core/exc.py
--rw-r--r--   0        0        0      772 2024-05-08 11:57:16.753731 grabberlib-0.1.1/grabber/core/settings.py
--rw-r--r--   0        0        0        0 2024-05-03 14:50:36.720132 grabberlib-0.1.1/grabber/core/sources/__init__.py
--rw-r--r--   0        0        0     3543 2024-05-08 12:59:24.763764 grabberlib-0.1.1/grabber/core/sources/everia.py
--rw-r--r--   0        0        0     2666 2024-05-08 12:55:29.819062 grabberlib-0.1.1/grabber/core/sources/graph.py
--rw-r--r--   0        0        0     3061 2024-05-08 12:05:40.276104 grabberlib-0.1.1/grabber/core/sources/khd.py
--rw-r--r--   0        0        0     2445 2024-05-08 12:59:24.762443 grabberlib-0.1.1/grabber/core/sources/nudecosplay.py
--rw-r--r--   0        0        0     2818 2024-05-08 12:08:31.466179 grabberlib-0.1.1/grabber/core/sources/xasiat.py
--rw-r--r--   0        0        0     3143 2024-05-08 12:49:26.255753 grabberlib-0.1.1/grabber/core/sources/xiuren.py
--rw-r--r--   0        0        0        1 2024-05-03 14:50:36.721312 grabberlib-0.1.1/grabber/core/sources/yellow.py
--rw-r--r--   0        0        0    19185 2024-05-08 13:07:33.380714 grabberlib-0.1.1/grabber/core/utils.py
--rw-r--r--   0        0        0      175 2024-05-08 13:29:13.280795 grabberlib-0.1.1/grabber/core/version.py
--rw-r--r--   0        0        0        0 2024-05-03 14:50:36.721870 grabberlib-0.1.1/grabber/templates/__init__.py
--rw-r--r--   0        0        0     1036 2024-05-08 13:29:17.781585 grabberlib-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1348 1970-01-01 00:00:00.000000 grabberlib-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-05-03 14:50:36.715508 grabberlib-0.1.2/README.md
+-rw-r--r--   0        0        0        1 2024-05-03 14:50:36.716140 grabberlib-0.1.2/assets/pages.txt
+-rw-r--r--   0        0        0        0 2024-05-03 14:50:36.718507 grabberlib-0.1.2/grabber/__init__.py
+-rw-r--r--   0        0        0     1690 2024-05-03 14:50:36.718702 grabberlib-0.1.2/grabber/__main__.py
+-rw-r--r--   0        0        0        0 2024-05-03 14:50:36.718877 grabberlib-0.1.2/grabber/controllers/__init__.py
+-rw-r--r--   0        0        0     5057 2024-05-08 12:59:24.763016 grabberlib-0.1.2/grabber/controllers/base.py
+-rw-r--r--   0        0        0        0 2024-05-03 14:50:36.719286 grabberlib-0.1.2/grabber/core/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-03 14:50:36.719467 grabberlib-0.1.2/grabber/core/bot/__init__.py
+-rw-r--r--   0        0        0      997 2024-05-08 13:00:46.779103 grabberlib-0.1.2/grabber/core/bot/core.py
+-rw-r--r--   0        0        0       65 2024-05-03 14:50:36.719818 grabberlib-0.1.2/grabber/core/exc.py
+-rw-r--r--   0        0        0      772 2024-05-08 11:57:16.753731 grabberlib-0.1.2/grabber/core/settings.py
+-rw-r--r--   0        0        0        0 2024-05-03 14:50:36.720132 grabberlib-0.1.2/grabber/core/sources/__init__.py
+-rw-r--r--   0        0        0     3553 2024-05-08 14:28:11.206371 grabberlib-0.1.2/grabber/core/sources/everia.py
+-rw-r--r--   0        0        0     2666 2024-05-08 12:55:29.819062 grabberlib-0.1.2/grabber/core/sources/graph.py
+-rw-r--r--   0        0        0     3061 2024-05-08 12:05:40.276104 grabberlib-0.1.2/grabber/core/sources/khd.py
+-rw-r--r--   0        0        0     2445 2024-05-08 12:59:24.762443 grabberlib-0.1.2/grabber/core/sources/nudecosplay.py
+-rw-r--r--   0        0        0     2818 2024-05-08 12:08:31.466179 grabberlib-0.1.2/grabber/core/sources/xasiat.py
+-rw-r--r--   0        0        0     3143 2024-05-08 12:49:26.255753 grabberlib-0.1.2/grabber/core/sources/xiuren.py
+-rw-r--r--   0        0        0        1 2024-05-03 14:50:36.721312 grabberlib-0.1.2/grabber/core/sources/yellow.py
+-rw-r--r--   0        0        0    19185 2024-05-08 13:07:33.380714 grabberlib-0.1.2/grabber/core/utils.py
+-rw-r--r--   0        0        0      175 2024-05-08 14:28:16.288787 grabberlib-0.1.2/grabber/core/version.py
+-rw-r--r--   0        0        0        0 2024-05-03 14:50:36.721870 grabberlib-0.1.2/grabber/templates/__init__.py
+-rw-r--r--   0        0        0     1036 2024-05-08 14:28:19.400870 grabberlib-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1348 1970-01-01 00:00:00.000000 grabberlib-0.1.2/PKG-INFO
```

### Comparing `grabberlib-0.1.1/grabber/__main__.py` & `grabberlib-0.1.2/grabber/__main__.py`

 * *Files identical despite different names*

### Comparing `grabberlib-0.1.1/grabber/controllers/base.py` & `grabberlib-0.1.2/grabber/controllers/base.py`

 * *Files identical despite different names*

### Comparing `grabberlib-0.1.1/grabber/core/bot/core.py` & `grabberlib-0.1.2/grabber/core/bot/core.py`

 * *Files identical despite different names*

### Comparing `grabberlib-0.1.1/grabber/core/settings.py` & `grabberlib-0.1.2/grabber/core/settings.py`

 * *Files identical despite different names*

### Comparing `grabberlib-0.1.1/grabber/core/sources/everia.py` & `grabberlib-0.1.2/grabber/core/sources/everia.py`

 * *Files 11% similar despite different names*

```diff
@@ -49,56 +49,55 @@
     final_dest: str | pathlib.Path = "",
     save_to_telegraph: bool | None = False,
     **kwargs,
 ) -> None:
     is_tag = kwargs.get("is_tag", False)
     query, src_attr = query_mapping[entity]
     headers = headers_mapping.get(entity, None)
-    title = None
+    page_title = None
     title_folder_mapping = {}
     posts_sent_counter = 0
     titles = []
 
     if final_dest:
         final_dest = pathlib.Path(final_dest)
         if not final_dest.exists():
             final_dest.mkdir(parents=True, exist_ok=True)
 
     if is_tag:
         soup = get_soup(target_url=sources[0], headers=headers)
-        title = soup.get_text(strip=True).split(" – EVERIA.CLUB")[0]
+        page_title = soup.get_text(strip=True).split(" – EVERIA.CLUB")[0].strip().rstrip()
         sources = list(get_pages_from_pagination(sources[0]))
 
     tqdm_sources_iterable = tqdm(
         enumerate(sources),
         total=len(sources),
         desc="Retrieving URLs...",
     )
 
     for idx, source_url in tqdm_sources_iterable:
         image_tags, soup = get_tags(source_url, headers=headers, query=query)
-        page_title = soup.get_text(strip=True).split(" – EVERIA.CLUB")[0]
 
-        if title is None:
-            title = soup.get_text(strip=True)
-            titles.append(title)
+        if page_title is None:
+            page_title = soup.get_text(strip=True).split(" – EVERIA.CLUB")[0].strip().rstrip()
+            titles.append(page_title)
 
         unique_img_urls = set()
         for idx, img_tag in enumerate(image_tags):
             img_src = img_tag.attrs[src_attr]
             img_name: str = img_src.split("/")[-1].split("?")[0]
             img_name = img_name.strip().rstrip()
             unique_img_urls.add((f"{page_title} {idx + 1}", img_src))
 
-        tqdm_sources_iterable.set_description(f"Finished retrieving images for {title}")
+        tqdm_sources_iterable.set_description(f"Finished retrieving images for {page_title}")
 
         if final_dest:
-            folder_name = title.strip().rstrip()
+            folder_name = page_title
             title_dest = final_dest / folder_name
-            title_folder_mapping[title] = (unique_img_urls, title_dest)
+            title_folder_mapping[page_title] = (unique_img_urls, title_dest)
 
         if save_to_telegraph:
             telegraph_uploader(
                 unique_img_urls=unique_img_urls,
                 page_title=page_title,
                 posts_sent_counter=posts_sent_counter,
                 telegraph_client=telegraph_client,
```

### Comparing `grabberlib-0.1.1/grabber/core/sources/graph.py` & `grabberlib-0.1.2/grabber/core/sources/graph.py`

 * *Files identical despite different names*

### Comparing `grabberlib-0.1.1/grabber/core/sources/khd.py` & `grabberlib-0.1.2/grabber/core/sources/khd.py`

 * *Files identical despite different names*

### Comparing `grabberlib-0.1.1/grabber/core/sources/nudecosplay.py` & `grabberlib-0.1.2/grabber/core/sources/nudecosplay.py`

 * *Files identical despite different names*

### Comparing `grabberlib-0.1.1/grabber/core/sources/xasiat.py` & `grabberlib-0.1.2/grabber/core/sources/xasiat.py`

 * *Files identical despite different names*

### Comparing `grabberlib-0.1.1/grabber/core/sources/xiuren.py` & `grabberlib-0.1.2/grabber/core/sources/xiuren.py`

 * *Files identical despite different names*

### Comparing `grabberlib-0.1.1/grabber/core/utils.py` & `grabberlib-0.1.2/grabber/core/utils.py`

 * *Files identical despite different names*

### Comparing `grabberlib-0.1.1/pyproject.toml` & `grabberlib-0.1.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "grabberlib"
-version = "0.1.1"
+version = "0.1.2"
 description = ""
 authors = ["grabber"]
 readme = "README.md"
 packages = [
     { include = "grabber/**/*.py" },
     { include = "assets/pages.txt" },
 ]
```

### Comparing `grabberlib-0.1.1/PKG-INFO` & `grabberlib-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grabberlib
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: grabber
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

