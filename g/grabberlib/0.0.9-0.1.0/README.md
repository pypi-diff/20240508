# Comparing `tmp/grabberlib-0.0.9.tar.gz` & `tmp/grabberlib-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grabberlib-0.0.9.tar", max compression
+gzip compressed data, was "grabberlib-0.1.0.tar", max compression
```

## Comparing `grabberlib-0.0.9.tar` & `grabberlib-0.1.0.tar`

### file list

```diff
@@ -1,20 +1,24 @@
--rw-r--r--   0        0        0        0 2024-04-20 14:47:15.755675 grabberlib-0.0.9/README.md
--rw-r--r--   0        0        0        1 2024-04-20 14:47:15.755675 grabberlib-0.0.9/assets/pages.txt
--rw-r--r--   0        0        0        0 2024-04-20 14:47:15.759675 grabberlib-0.0.9/grabber/__init__.py
--rw-r--r--   0        0        0     1690 2024-04-20 14:47:15.759675 grabberlib-0.0.9/grabber/__main__.py
--rw-r--r--   0        0        0        0 2024-04-20 14:47:15.759675 grabberlib-0.0.9/grabber/controllers/__init__.py
--rw-r--r--   0        0        0     4066 2024-04-20 15:40:45.571619 grabberlib-0.0.9/grabber/controllers/base.py
--rw-r--r--   0        0        0        0 2024-04-20 14:47:15.759675 grabberlib-0.0.9/grabber/core/__init__.py
--rw-r--r--   0        0        0       65 2024-04-20 14:47:15.759675 grabberlib-0.0.9/grabber/core/exc.py
--rw-r--r--   0        0        0      446 2024-04-20 15:06:51.092892 grabberlib-0.0.9/grabber/core/settings.py
--rw-r--r--   0        0        0        0 2024-04-20 14:47:15.759675 grabberlib-0.0.9/grabber/core/sources/__init__.py
--rw-r--r--   0        0        0     3400 2024-04-20 15:08:46.386081 grabberlib-0.0.9/grabber/core/sources/graph.py
--rw-r--r--   0        0        0     4008 2024-04-20 15:09:05.377639 grabberlib-0.0.9/grabber/core/sources/khd.py
--rw-r--r--   0        0        0     3610 2024-04-20 15:09:24.729188 grabberlib-0.0.9/grabber/core/sources/xasiat.py
--rw-r--r--   0        0        0     3871 2024-04-20 15:32:13.229448 grabberlib-0.0.9/grabber/core/sources/xiuren.py
--rw-r--r--   0        0        0        1 2024-04-20 14:47:15.759675 grabberlib-0.0.9/grabber/core/sources/yellow.py
--rw-r--r--   0        0        0    13127 2024-04-20 15:12:16.745134 grabberlib-0.0.9/grabber/core/utils.py
--rw-r--r--   0        0        0      175 2024-04-20 15:40:55.979342 grabberlib-0.0.9/grabber/core/version.py
--rw-r--r--   0        0        0        0 2024-04-20 14:47:15.759675 grabberlib-0.0.9/grabber/templates/__init__.py
--rw-r--r--   0        0        0     1017 2024-04-20 15:40:50.431490 grabberlib-0.0.9/pyproject.toml
--rw-r--r--   0        0        0     1308 1970-01-01 00:00:00.000000 grabberlib-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-05-03 14:50:36.715508 grabberlib-0.1.0/README.md
+-rw-r--r--   0        0        0        1 2024-05-03 14:50:36.716140 grabberlib-0.1.0/assets/pages.txt
+-rw-r--r--   0        0        0        0 2024-05-03 14:50:36.718507 grabberlib-0.1.0/grabber/__init__.py
+-rw-r--r--   0        0        0     1690 2024-05-03 14:50:36.718702 grabberlib-0.1.0/grabber/__main__.py
+-rw-r--r--   0        0        0        0 2024-05-03 14:50:36.718877 grabberlib-0.1.0/grabber/controllers/__init__.py
+-rw-r--r--   0        0        0     5107 2024-05-03 14:50:36.719117 grabberlib-0.1.0/grabber/controllers/base.py
+-rw-r--r--   0        0        0        0 2024-05-03 14:50:36.719286 grabberlib-0.1.0/grabber/core/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-03 14:50:36.719467 grabberlib-0.1.0/grabber/core/bot/__init__.py
+-rw-r--r--   0        0        0     1184 2024-05-07 14:11:46.736435 grabberlib-0.1.0/grabber/core/bot/core.py
+-rw-r--r--   0        0        0       65 2024-05-03 14:50:36.719818 grabberlib-0.1.0/grabber/core/exc.py
+-rw-r--r--   0        0        0      696 2024-05-03 14:50:36.719968 grabberlib-0.1.0/grabber/core/settings.py
+-rw-r--r--   0        0        0        0 2024-05-03 14:50:36.720132 grabberlib-0.1.0/grabber/core/sources/__init__.py
+-rw-r--r--   0        0        0     3232 2024-05-07 14:22:47.160221 grabberlib-0.1.0/grabber/core/sources/everia.py
+-rw-r--r--   0        0        0     3797 2024-05-08 11:40:49.252100 grabberlib-0.1.0/grabber/core/sources/graph.py
+-rw-r--r--   0        0        0     4630 2024-05-08 11:42:28.376443 grabberlib-0.1.0/grabber/core/sources/khd.py
+-rw-r--r--   0        0        0     3604 2024-05-03 14:50:36.720826 grabberlib-0.1.0/grabber/core/sources/nudecosplay.py
+-rw-r--r--   0        0        0     3989 2024-05-03 14:50:36.720989 grabberlib-0.1.0/grabber/core/sources/xasiat.py
+-rw-r--r--   0        0        0     4107 2024-05-03 14:50:36.721155 grabberlib-0.1.0/grabber/core/sources/xiuren.py
+-rw-r--r--   0        0        0        1 2024-05-03 14:50:36.721312 grabberlib-0.1.0/grabber/core/sources/yellow.py
+-rw-r--r--   0        0        0    16275 2024-05-03 14:50:36.721552 grabberlib-0.1.0/grabber/core/utils.py
+-rw-r--r--   0        0        0      175 2024-05-08 11:41:48.914325 grabberlib-0.1.0/grabber/core/version.py
+-rw-r--r--   0        0        0        0 2024-05-03 14:50:36.721870 grabberlib-0.1.0/grabber/templates/__init__.py
+-rw-r--r--   0        0        0     1036 2024-05-08 11:41:57.715542 grabberlib-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1348 1970-01-01 00:00:00.000000 grabberlib-0.1.0/PKG-INFO
```

### Comparing `grabberlib-0.0.9/grabber/__main__.py` & `grabberlib-0.1.0/grabber/__main__.py`

 * *Files identical despite different names*

### Comparing `grabberlib-0.0.9/grabber/controllers/base.py` & `grabberlib-0.1.0/grabber/controllers/base.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 from cement import Controller, ex
+from telegraph import Telegraph
 
+from grabber.core.settings import TELEGRAPH_TOKEN
+from grabber.core.sources.everia import get_sources_for_everia
 from grabber.core.sources.graph import get_for_telegraph
 from grabber.core.sources.khd import get_sources_for_4khd
+from grabber.core.sources.nudecosplay import get_sources_for_nudecosplay
 from grabber.core.sources.xiuren import get_sources_for_xiuren
 from grabber.core.utils import upload_folders_to_telegraph
 
 from ..core.version import get_version
 
 VERSION_BANNER = f"""
 A beautiful CLI utility to download images from the web! {get_version()}
@@ -81,14 +85,22 @@
                 {
                     "dest": "is_tag",
                     "action": "store_true",
                     "help": "Indicates that the link(s) passed is a tag in which the posts are paginated",
                 },
             ),
             (
+                ["-b", "--bot"],
+                {
+                    "dest": "bot",
+                    "action": "store_true",
+                    "help": "Should the newly post be sent to telegram?",
+                },
+            ),
+            (
                 ["-v", "--version"],
                 {
                     "action": "store_true",
                     "dest": "version",
                     "help": "Version of the lib",
                 },
             ),
@@ -102,29 +114,43 @@
         sources = self.app.pargs.sources
         folder = self.app.pargs.folder
         publish = self.app.pargs.publish
         upload = self.app.pargs.upload
         is_tag = self.app.pargs.is_tag
         limit = self.app.pargs.limit
         version = self.app.pargs.version
+        send_to_telegram = self.app.pargs.bot
+        telegraph_client = Telegraph(access_token=TELEGRAPH_TOKEN)
+
         if version:
             print(VERSION_BANNER)
             return
 
         getter_mapping = {
             "4khd": get_sources_for_4khd,
             "telegraph": get_for_telegraph,
             "xiuren": get_sources_for_xiuren,
+            "nudecosplay": get_sources_for_nudecosplay,
+            "nudebird": get_sources_for_nudecosplay,
+            "hotgirl": get_sources_for_nudecosplay,
+            "everia": get_sources_for_everia,
         }
 
         if upload:
-            upload_folders_to_telegraph(folder_name=folder, limit=limit)
+            upload_folders_to_telegraph(
+                folder_name=folder,
+                limit=limit,
+                send_to_channel=send_to_telegram,
+                telegraph_client=telegraph_client,
+            )
         else:
             getter_images = getter_mapping.get(entity, get_for_telegraph)
             getter_images(
                 sources=sources,
                 entity=entity,
                 final_dest=folder,
                 save_to_telegraph=publish,
                 is_tag=is_tag,
                 limit=limit,
+                send_to_telegram=send_to_telegram,
+                telegraph_client=telegraph_client,
             )
```

### Comparing `grabberlib-0.0.9/grabber/core/sources/graph.py` & `grabberlib-0.1.0/grabber/core/sources/xasiat.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,38 @@
 import multiprocessing
 import pathlib
 from concurrent.futures import ThreadPoolExecutor
 from functools import partial
 from typing import List
 
+from telegraph import Telegraph
 from tqdm import tqdm
 
 from grabber.core.settings import get_media_root
 from grabber.core.utils import (
+    print_albums_message,
     query_mapping,
     headers_mapping,
     get_tags,
     download_images,
     upload_to_telegraph,
 )
 
 DEFAULT_THREADS_NUMBER = multiprocessing.cpu_count()
 
 
-def get_for_telegraph(
+def get_for_xasiat(
     sources: List[str],
     entity: str,
+    telegraph_client: Telegraph,
     final_dest: str | pathlib.Path = "",
     save_to_telegraph: bool | None = False,
     **kwargs,
 ) -> None:
+    send_to_telegram = kwargs.get("send_to_telegram", False)
     titles = set()
     tqdm_sources_iterable = tqdm(
         enumerate(sources),
         total=len(sources),
     )
     query, src_attr = query_mapping[entity]
     headers = headers_mapping.get(entity, None)
@@ -40,14 +44,15 @@
         final_dest_folder = get_media_root() / final_dest
         if not final_dest_folder.exists():
             final_dest_folder.mkdir(parents=True, exist_ok=True)
             final_dest = final_dest_folder
 
     for idx, source_url in tqdm_sources_iterable:
         folder_name = ""
+        tqdm_sources_iterable.set_description(f"Retrieving URLs from {source_url}")
         tags, soup = get_tags(
             source_url,
             headers=headers,
             query=query,
         )
 
         title_tag = soup.select("title")[0]  # type: ignore
@@ -65,22 +70,27 @@
             new_folder.mkdir(parents=True, exist_ok=True)
 
         folders.add(new_folder)
         unique_img_urls = set()
 
         for idx, img_tag in enumerate(tags or []):
             img_src = img_tag.attrs[src_attr]
-            img_name: str = img_src.split("/")[-1]
-            img_name = img_name.strip().rstrip()
-            if "images.hotgirl.asia" not in img_src:
-                unique_img_urls.add(
-                    (f"{idx + 1}-{img_name}", f"https://telegra.ph{img_src}")
-                )
+
+            if "xasiat" in img_src:
+                img_name: str = img_src.split("/")[-2]
+                img_name = img_name.strip().rstrip()
+                img_extension: str = img_name.split(".")[-1]
             else:
-                unique_img_urls.add((f"{idx + 1}-{img_name}", img_src))
+                img_name: str = img_src.split("/")[-1]
+                img_name = img_name.strip().rstrip()
+                img_extension: str = img_name.split(".")[-1]
+
+            unique_img_urls.add(
+                (title, f"{idx + 1}.{img_extension}", img_src),
+            )
 
         title_folder_mapping[title] = (unique_img_urls, new_folder)
 
     futures = []
     with ThreadPoolExecutor(max_workers=DEFAULT_THREADS_NUMBER) as executor:
         for title, (images_set, folder_dest) in title_folder_mapping.items():
             partial_download = partial(
@@ -95,19 +105,26 @@
     for future in tqdm(
         futures,
         total=len(futures),
         desc="Finishing download...",
     ):
         future.result()
 
+    posts = []
     if save_to_telegraph:
-        for folder in folders:
-            print(f"Uploading to telegraph {folder}")
-            upload_to_telegraph(folder)
-
-    albums_message = "".join([f"- {title}\n" for title in titles])
-    message = f"""
-    All images have been downloaded and saved to the specified folder.
-    Albums saved are the following:
-        {albums_message}
-    """
-    print(message)
+        for title, (_, folder_dest) in title_folder_mapping.items():
+            posts.append(
+                upload_to_telegraph(
+                    folder_dest,
+                    page_title=title,
+                    send_to_telegram=send_to_telegram,
+                    telegraph_client=telegraph_client,
+                )
+            )
+
+    albums_file = pathlib.Path(get_media_root() / "assets/pages.txt")
+    if albums_file.exists():
+        albums_links = albums_file.read_text().split("\n")
+    else:
+        albums_links = posts
+
+    print_albums_message(albums_links)
```

### Comparing `grabberlib-0.0.9/grabber/core/sources/khd.py` & `grabberlib-0.1.0/grabber/core/sources/graph.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,121 +1,126 @@
 import multiprocessing
 import pathlib
-from concurrent.futures import ThreadPoolExecutor, as_completed
+from concurrent.futures import ThreadPoolExecutor
 from functools import partial
-from typing import List, Optional
+from typing import List
 
+from telegraph import Telegraph
 from tqdm import tqdm
 
 from grabber.core.settings import get_media_root
 from grabber.core.utils import (
+    print_albums_message,
     query_mapping,
     headers_mapping,
     get_tags,
     download_images,
     upload_to_telegraph,
 )
 
 DEFAULT_THREADS_NUMBER = multiprocessing.cpu_count()
-page_nav_query = "div.page-link-box li a.page-numbers"
 
 
-def get_images_from_pagination(url: str, headers: Optional[dict] = None) -> List[str]:
-    tags, _ = get_tags(url, headers=headers, query=page_nav_query)
-    return [a.attrs["href"] for a in tags if tags]
-
-
-def get_sources_for_4khd(
+def get_for_telegraph(
     sources: List[str],
     entity: str,
+    telegraph_client: Telegraph,
     final_dest: str | pathlib.Path = "",
     save_to_telegraph: bool | None = False,
     **kwargs,
 ) -> None:
+    send_to_telegram = kwargs.get("send_to_telegram", False)
     titles = set()
     tqdm_sources_iterable = tqdm(
         enumerate(sources),
         total=len(sources),
-        desc="Retrieving URLs...",
     )
     query, src_attr = query_mapping[entity]
     headers = headers_mapping.get(entity, None)
     folders = set()
     titles_and_folders = set()
     title_folder_mapping = {}
 
     if final_dest:
-        final_dest_folder = get_media_root() / pathlib.Path(final_dest)
-        if not final_dest_folder.exists():
-            final_dest_folder.mkdir(parents=True, exist_ok=True)
-            final_dest = final_dest_folder
+        final_dest = pathlib.Path(final_dest)
+        if not final_dest.exists():
+            final_dest.mkdir(parents=True, exist_ok=True)
 
     for idx, source_url in tqdm_sources_iterable:
-        current_folder = None
-        current_title = None
         folder_name = ""
-        urls = [
+        tags, soup = get_tags(
             source_url,
-            *get_images_from_pagination(url=source_url, headers=headers),
-        ]
-        image_tags = []
-
-        for index, url in enumerate(urls):
-            tags, soup = get_tags(
-                url,
-                headers=headers,
-                query=query,
-            )
-            image_tags.extend(tags or [])
-
-            if index == 0:
-                folder_name = soup.select("title")[0].get_text()  # type: ignore
-                title = folder_name.strip().rstrip()
-                titles.add(title)
-                titles_and_folders.add((title, folder_name))
-                current_title = title
+            headers=headers,
+            query=query,
+        )
+
+        title_tag = soup.select("title")[0]  # type: ignore
+        folder_name = title_tag.get_text().strip().rstrip()
+        title = folder_name
+        titles.add(title)
+        titles_and_folders.add((title, folder_name))
 
         if final_dest:
-            new_folder = get_media_root() / final_dest / folder_name
+            new_folder = final_dest / folder_name
         else:
             new_folder = get_media_root() / folder_name
 
         if not new_folder.exists():
             new_folder.mkdir(parents=True, exist_ok=True)
 
-        current_folder = new_folder
-        folders.add(current_folder)
+        folders.add(new_folder)
         unique_img_urls = set()
 
-        for idx, img_tag in enumerate(image_tags):
+        for idx, img_tag in enumerate(tags or []):
             img_src = img_tag.attrs[src_attr]
-            img_name: str = img_src.split("/")[-1].split("?")[0]
+            img_name: str = img_src.split("/")[-1]
             img_name = img_name.strip().rstrip()
-            unique_img_urls.add((f"{idx + 1}-{img_name}", img_src))
-        title_folder_mapping[current_title] = (unique_img_urls, new_folder)
+            if "images.hotgirl.asia" not in img_src:
+                unique_img_urls.add(
+                    (f"{idx + 1}-{img_name}", f"https://telegra.ph{img_src}")
+                )
+            else:
+                unique_img_urls.add((f"{idx + 1}-{img_name}", img_src))
+
+        title_folder_mapping[title] = (unique_img_urls, new_folder)
 
+    futures = []
     with ThreadPoolExecutor(max_workers=DEFAULT_THREADS_NUMBER) as executor:
-        # Dictionary to hold Future objects
-        futures_to_title = {}
-        future_counter = 0
         for title, (images_set, folder_dest) in title_folder_mapping.items():
             partial_download = partial(
                 download_images,
                 new_folder=folder_dest,
                 headers=headers,
                 title=title,
             )
-            future = executor.submit(partial_download, images_set)
-            futures_to_title[future] = title
-            future_counter += 1
-
-        # Handling futures as they complete
-        for future in tqdm(
-            as_completed(futures_to_title),
-            total=future_counter,
-            desc=f"Retrieving {future_counter} tasks of downloading images",
-        ):
-            future.result()  # Get the result from the future object
+            future = executor.submit(partial_download, images_set, title=title)
+            futures.append(future)
 
+    for future in tqdm(
+        futures,
+        total=len(futures),
+        desc="Finishing download...",
+    ):
+        future.result()
+
+    posts = []
     if save_to_telegraph:
         for title, (_, folder_dest) in title_folder_mapping.items():
-            upload_to_telegraph(folder_dest, page_title=title)
+            posts.append(
+                upload_to_telegraph(
+                    folder_dest,
+                    page_title=title,
+                    send_to_telegram=send_to_telegram,
+                    telegraph_client=telegraph_client,
+                )
+            )
+
+        albums_dir = pathlib.Path.home() / ".albums_data"
+        albums_dir.mkdir(parents=True, exist_ok=True)
+        albums_file = albums_dir / "pages.txt"
+
+        with albums_file.open("w") as f:
+            f.write("\n".join(posts))
+
+        albums_links = albums_file.read_text().split("\n")
+
+        print_albums_message(albums_links)
```

### Comparing `grabberlib-0.0.9/grabber/core/sources/xasiat.py` & `grabberlib-0.1.0/grabber/core/sources/nudecosplay.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,38 +1,44 @@
+
 import multiprocessing
 import pathlib
 from concurrent.futures import ThreadPoolExecutor
 from functools import partial
 from typing import List
 
+from telegraph import Telegraph
 from tqdm import tqdm
 
 from grabber.core.settings import get_media_root
 from grabber.core.utils import (
+    print_albums_message,
     query_mapping,
     headers_mapping,
     get_tags,
     download_images,
     upload_to_telegraph,
 )
 
 DEFAULT_THREADS_NUMBER = multiprocessing.cpu_count()
 
 
-def get_for_xasiat(
+def get_sources_for_nudecosplay(
     sources: List[str],
     entity: str,
+    telegraph_client: Telegraph,
     final_dest: str | pathlib.Path = "",
     save_to_telegraph: bool | None = False,
     **kwargs,
 ) -> None:
+    send_to_telegram = kwargs.get("send_to_telegram", False)
     titles = set()
     tqdm_sources_iterable = tqdm(
         enumerate(sources),
         total=len(sources),
+        desc="Retrieving URLs...",
     )
     query, src_attr = query_mapping[entity]
     headers = headers_mapping.get(entity, None)
     folders = set()
     titles_and_folders = set()
     title_folder_mapping = {}
 
@@ -40,15 +46,14 @@
         final_dest_folder = get_media_root() / final_dest
         if not final_dest_folder.exists():
             final_dest_folder.mkdir(parents=True, exist_ok=True)
             final_dest = final_dest_folder
 
     for idx, source_url in tqdm_sources_iterable:
         folder_name = ""
-        tqdm_sources_iterable.set_description(f"Retrieving URLs from {source_url}")
         tags, soup = get_tags(
             source_url,
             headers=headers,
             query=query,
         )
 
         title_tag = soup.select("title")[0]  # type: ignore
@@ -66,54 +71,51 @@
             new_folder.mkdir(parents=True, exist_ok=True)
 
         folders.add(new_folder)
         unique_img_urls = set()
 
         for idx, img_tag in enumerate(tags or []):
             img_src = img_tag.attrs[src_attr]
-
-            if "xasiat" in img_src:
-                img_name: str = img_src.split("/")[-2]
-                img_name = img_name.strip().rstrip()
-                img_extension: str = img_name.split(".")[-1]
-            else:
-                img_name: str = img_src.split("/")[-1]
-                img_name = img_name.strip().rstrip()
-                img_extension: str = img_name.split(".")[-1]
-
-            unique_img_urls.add(
-                (title, f"{idx + 1}.{img_extension}", img_src),
-            )
+            img_name: str = img_src.split("/")[-1]
+            img_name = img_name.strip().rstrip()
+            unique_img_urls.add((f"{idx + 1}-{img_name}", img_src))
 
         title_folder_mapping[title] = (unique_img_urls, new_folder)
 
     futures = []
     with ThreadPoolExecutor(max_workers=DEFAULT_THREADS_NUMBER) as executor:
         for title, (images_set, folder_dest) in title_folder_mapping.items():
             partial_download = partial(
                 download_images,
                 new_folder=folder_dest,
                 headers=headers,
                 title=title,
             )
-            future = executor.submit(partial_download, images_set, title=title)
+            future = executor.submit(partial_download, images_set)
             futures.append(future)
 
     for future in tqdm(
         futures,
         total=len(futures),
         desc="Finishing download...",
     ):
         future.result()
 
+    posts = []
     if save_to_telegraph:
-        for folder in folders:
-            print(f"Uploading to telegraph {folder}")
-            upload_to_telegraph(folder)
-
-    albums_message = "".join([f"- {title}\n" for title in titles])
-    message = f"""
-    All images have been downloaded and saved to the specified folder.
-    Albums saved are the following:
-        {albums_message}
-    """
-    print(message)
+        for title, (_, folder_dest) in title_folder_mapping.items():
+            posts.append(
+                upload_to_telegraph(
+                    folder_dest,
+                    telegraph_client=telegraph_client,
+                    page_title=title,
+                    send_to_telegram=send_to_telegram,
+                )
+            )
+
+    albums_file = pathlib.Path(get_media_root() / "assets/pages.txt")
+    if albums_file.exists():
+        albums_links = albums_file.read_text().split("\n")
+    else:
+        albums_links = posts
+
+    print_albums_message(albums_links)
```

### Comparing `grabberlib-0.0.9/grabber/core/sources/xiuren.py` & `grabberlib-0.1.0/grabber/core/sources/xiuren.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,35 +1,39 @@
 import multiprocessing
 import pathlib
 from concurrent.futures import ThreadPoolExecutor
 from functools import partial
 from typing import List
 
+import telegraph
 from tqdm import tqdm
 
 from grabber.core.settings import get_media_root
 from grabber.core.utils import (
     get_pages_from_pagination,
+    print_albums_message,
     query_mapping,
     headers_mapping,
     get_tags,
     download_images,
     upload_to_telegraph,
 )
 
 DEFAULT_THREADS_NUMBER = multiprocessing.cpu_count()
 
 
 def get_sources_for_xiuren(
     sources: List[str],
     entity: str,
+    telegraph_client: telegraph.Telegraph,
     final_dest: str | pathlib.Path = "",
     save_to_telegraph: bool | None = False,
     **kwargs,
 ) -> None:
+    send_to_telegram = kwargs.get("send_to_telegram", False)
     titles = set()
     is_tag: bool = kwargs.get("is_tag", False)
     limit: int = kwargs.get("limit", 0)
     tqdm_sources_iterable = tqdm(
         enumerate(sources),
         total=len(sources),
         desc="Retrieving URLs...",
@@ -106,20 +110,26 @@
     for future in tqdm(
         futures,
         total=len(futures),
         desc="Finishing download...",
     ):
         future.result()
 
+    posts = []
     if save_to_telegraph:
         for title, (_, folder_dest) in title_folder_mapping.items():
-            upload_to_telegraph(folder_dest, page_title=title)
+            posts.append(
+                upload_to_telegraph(
+                    folder_dest,
+                    page_title=title,
+                    send_to_telegram=send_to_telegram,
+                    telegraph_client=telegraph_client,
+                )
+            )
 
     albums_file = pathlib.Path(get_media_root() / "assets/pages.txt")
-    albums_links = albums_file.read_text().split("\n")
-    albums_message = "".join([f"- {album}\n" for album in albums_links])
-    message = f"""
-    All albums have been downloaded and saved to the specified folder.
-    Albums saved are the following:
-        {albums_message}
-    """
-    print(message)
+    if albums_file.exists():
+        albums_links = albums_file.read_text().split("\n")
+    else:
+        albums_links = posts
+
+    print_albums_message(albums_links)
```

### Comparing `grabberlib-0.0.9/grabber/core/utils.py` & `grabberlib-0.1.0/grabber/core/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,90 +1,98 @@
+import asyncio
 import multiprocessing
 import pathlib
 import shutil
 from concurrent.futures import ThreadPoolExecutor, as_completed
 from functools import partial
 from dataclasses import dataclass
+from time import sleep
 from typing import Any, Dict, List, Optional, Tuple
 
 import requests
 from bs4 import BeautifulSoup, Tag
 from casefy.casefy import snakecase
 from lxml import etree
 from PIL import Image
 from telegraph import Telegraph
 from telegraph import exceptions
 from tenacity import retry, wait_chain, wait_fixed
 from tqdm import tqdm
 
-from grabber.core.settings import get_media_root
+from grabber.core.bot.core import send_message
+from grabber.core.settings import AUTHOR_NAME, AUTHOR_URL, SHORT_NAME, get_media_root
 
 DEFAULT_THREADS_NUMBER = multiprocessing.cpu_count()
 PAGINATION_QUERY = "div.jeg_navigation.jeg_pagination"
 PAGINATION_PAGES_COUNT_QUERY = f"{PAGINATION_QUERY} span.page_info"
 PAGINATION_BASE_URL_QUERY = "div.jeg_navigation.jeg_pagination a.page_number"
 POSTS_QUERY_XPATH = "/html/body/div[2]/div[5]/div/div[1]/div/div/div[2]/div/div/div[2]/div/div[1]/div/div/div/article/div/div/a"
 
 
 query_mapping = {
     "xiuren": ("div.content-inner img", "src"),
     "nudebird": ("div.thecontent a", "href"),
-    "nudecosplay": ("div.content-inner img", "src"),
+    "nudecosplay": ("img[src^='https://static9.hentai-cosplays.com/'][alt^='PureMedia']", "src"),
     "v2ph": ("div.photos-list.text-center img", "src"),  # Needs to handle pagination
     "cgcosplay": ("div.gallery-icon.portrait img", "src"),
     "mitaku": ("img.msacwl-img", "data-lazy"),
     "xasiat": ("div.images a", "href"),
     "telegraph": ("img", "src"),
     "4khd": (
         "div.is-layout-constrained.entry-content.wp-block-post-content img",
         "src",
     ),
     "yellow": (
         "div.elementor-widget-container a[href^='https://terabox.com']",
         "href",
     ),
+    "everia": ("div.entry-content img", "src"),
 }
 
 
 @dataclass(kw_only=True)
-class Pagination:
+class PaginationXPath:
     pagination_query: str
     pages_count_query: str
     pagination_base_url_query: str
     posts_query_xpath: str
 
     def __post_init__(self) -> None:
         self.pages_count_query = f"{self.pagination_query} {self.pages_count_query}"
 
 
 query_pagination_mapping = {
-    "xiuren": Pagination(
+    "xiuren": PaginationXPath(
         pagination_query="div.jeg_navigation.jeg_pagination",
         pages_count_query="span.page_info",
         pagination_base_url_query="div.jeg_navigation.jeg_pagination a.page_number",
         posts_query_xpath=(
             "/html/body/div[2]/div[5]/div/div[1]/div/div/div[2]/"
             "div/div/div[2]/div/div[1]/div/div/div/article/div/div/a"
         ),
     ),
-    "yellow": Pagination(
+    "yellow": PaginationXPath(
         pagination_query="div.jeg_navigation.jeg_pagination",
         pages_count_query="span.page_info",
         pagination_base_url_query="div.jeg_navigation.jeg_pagination a.page_number",
         posts_query_xpath=(
             "/html/body/div[3]/div[4]/div/div[1]/div/div/div[2]/"
             "div/div/div[2]/div/div[1]/div/div/div/article/div/div/a"
         ),
     ),
 }
 headers_mapping = {
     "nudebird": {
         "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.7",
         "User-Agent": "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/123.0.0.0 Safari/537.36",
     },
+    "nudecosplay": {
+        "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.7",
+        "User-Agent": "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/123.0.0.0 Safari/537.36",
+    },
     "v2ph": {
         "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.7",
         "User-Agent": "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/123.0.0.0 Safari/537.36",
     },
     "cgcosplay": {
         "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.7",
         "User-Agent": "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/123.0.0.0 Safari/537.36",
@@ -225,46 +233,96 @@
         if file.suffix == ".webp":
             image = Image.open(file).convert("RGB")
             new_file = file.with_suffix(".jpg")
             image.save(new_file, "JPEG")
             file.unlink()
 
 
-def upload_file(file: pathlib.Path, telegraph_client: Telegraph) -> Optional[str]:
+def get_new_telegraph_client() -> Telegraph:
+    telegraph_factory = Telegraph()
+    resp = telegraph_factory.create_account(
+        short_name=SHORT_NAME,
+        author_name=AUTHOR_NAME,
+        author_url=AUTHOR_URL,
+        replace_token=True,
+    )
+    access_token = resp["access_token"]
+    telegraph_client = Telegraph(access_token=access_token)
+    return telegraph_client
+
+
+def upload_file(
+    file: pathlib.Path,
+    telegraph_client: Telegraph,
+    try_again: Optional[bool] = True,
+) -> Optional[str]:
     try:
         uploaded = telegraph_client.upload_file(file)
-    except (Exception, exceptions.TelegraphException):
+    except (Exception, exceptions.TelegraphException, exceptions.RetryAfterError) as exc:
+        error_message = str(exc)
+        if 'try again' in error_message.lower() or 'retry' in error_message.lower():
+            sleep(5)
+            if try_again:
+                telegraph_client = get_new_telegraph_client()
+                return upload_file(file=file, telegraph_client=telegraph_client, try_again=False)
         return
     if uploaded:
         return uploaded[0]["src"]
 
 
-def create_page(title: str, html_content: str, telegraph_client: Telegraph) -> str:
-    page = telegraph_client.create_page(title=title, html_content=html_content)
-    return page["url"]
+def create_page(
+    title: str,
+    html_content: str,
+    telegraph_client: Telegraph,
+    try_again: Optional[bool] = True,
+) -> str:
+    try:
+        page = telegraph_client.create_page(title=title, html_content=html_content)
+        return page["url"]
+    except (Exception, exceptions.TelegraphException, exceptions.RetryAfterError) as exc:
+        error_message = str(exc)
+        if 'try again' in error_message.lower() or 'retry' in error_message.lower():
+            sleep(5)
+            if try_again:
+                telegraph_client = get_new_telegraph_client()
+                return create_page(
+                    title=title,
+                    html_content=html_content,
+                    telegraph_client=telegraph_client,
+                    try_again=False,
+                )
+
+
+def create_html_template(image_tags: Tuple[str, str]) -> str:
+    html_template = """<figure contenteditable="false"><img src="{file_path}"><figcaption dir="auto" class="editable_text" data-placeholder="{title}"></figcaption></figure>"""
+    template_tags = []
+    for title, image_src in image_tags:
+        template_tags.append(html_template.format(file_path=image_src, title=title))
+
+    html_post = "\n".join(template_tags)
+    return html_post
 
 
 def upload_to_telegraph(
     folder: pathlib.Path,
+    telegraph_client: Telegraph,
     page_title: Optional[str] = "",
+    send_to_telegram: Optional[bool] = False,
 ) -> str:
-    telegraph_client = Telegraph(
-        access_token="d3f83ad3b88a5028de2a7a5b53eecad7e7defc2c392b87f5fab0f72cca5d"
-    )
     files = sorted(list(folder.iterdir()), key=sort_file)
     title = page_title or folder.name
     title = title.strip().rstrip()
 
     contents = []
     files_urls = []
     html_template = """<figure contenteditable="false"><img src="{file_path}"><figcaption dir="auto" class="editable_text" data-placeholder="{title}"></figcaption></figure>"""
 
     uploaded_files_url_path = pathlib.Path(f"{snakecase(title)}.txt")
-    if uploaded_files_url_path.exists():
-        files_urls = uploaded_files_url_path.read_text().split("\n")
+    if uploaded_files_url_path.exists() and uploaded_files_url_path.stat().st_size > 0:
+        contents = uploaded_files_url_path.read_text().split("\n")
     else:
         iterable_files = tqdm(
             files,
             total=len(files),
             desc=f"Uploading files for {folder.name}",
             leave=False,
         )
@@ -272,37 +330,48 @@
         for file in iterable_files:
             file_url = upload_file(file, telegraph_client=telegraph_client)
             if not file_url:
                 continue
             files_urls.append(file_url)
             contents.append(html_template.format(file_path=file_url, title=image_title))
 
-    content = "\n".join(contents)
-    try:
-        page_url = create_page(
-            title=title,
-            html_content=content,
-            telegraph_client=telegraph_client,
-        )
-    except exceptions.TelegraphException as exc:
-        print(f"Error: {exc} - {title} - {folder}")
-        if "None" not in content:
-            with open(uploaded_files_url_path, "w") as f:
-                f.write("\n".join(files_urls))
-        return
+    if contents:
+        content = "\n".join(contents)
+        try:
+            page_url = create_page(
+                title=title,
+                html_content=content,
+                telegraph_client=telegraph_client,
+            )
+        except exceptions.TelegraphException as exc:
+            return f"Error: {exc} - {title} - {folder}"
+
+        post = f"{title} - {page_url}"
+
+        if send_to_telegram:
+            asyncio.run(send_message(post))
+
+        pages_file = get_media_root() / "assets/pages.txt"
 
-    with open(get_media_root() / "assets/pages.txt", "a") as f:
-        f.write(f"{title} - {page_url}\n")
+        if not pages_file.exists():
+            pages_file.touch(exist_ok=True)
 
-    return page_url
+        with open(pages_file, "a") as f:
+            f.write(f"{post}\n")
+
+        return post
+
+    return "No content, please try again later"
 
 
 def upload_folders_to_telegraph(
-    folder_name: Optional[str] = "",
+    folder_name: str,
+    telegraph_client: Telegraph,
     limit: Optional[int] = 0,
+    send_to_channel: Optional[bool] = False,
 ) -> None:
     folders = []
 
     if folder_name:
         root = get_media_root() / folder_name
         folders += [f for f in list(root.iterdir()) if f.is_dir()]
     else:
@@ -318,15 +387,20 @@
                     folders = root_folders
 
     futures_to_folder = {}
     selected_folders = folders[:limit] if limit else folders
     with ThreadPoolExecutor(max_workers=DEFAULT_THREADS_NUMBER) as executor:
         future_counter = 0
         for folder in selected_folders:
-            partial_upload = partial(upload_to_telegraph, folder)
+            partial_upload = partial(
+                upload_to_telegraph,
+                folder,
+                send_to_telegram=send_to_channel,
+                telegraph_client=telegraph_client,
+            )
             future = executor.submit(partial_upload)
             futures_to_folder[future] = folder
             future_counter += 1
 
         page_urls: list[tuple[str, str]] = []
         for future in tqdm(
             as_completed(futures_to_folder),
@@ -377,7 +451,19 @@
             [
                 a_tag.attrib["href"]
                 for a_tag in dom.xpath(pagination_params.posts_query_xpath)
             ]
         )
 
     return source_urls
+
+
+def print_albums_message(albums_links: List[str]) -> None:
+    albums_message = ""
+
+    for album in albums_links:
+        albums_message += f"\t- {album}\n"
+
+    message = "All albums have been downloaded and saved to the specified folder.\n"
+    message += "Albums saved are the following:\n"
+    message += f"{albums_message}"
+    print(message)
```

### Comparing `grabberlib-0.0.9/pyproject.toml` & `grabberlib-0.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "grabberlib"
-version = "0.0.9"
+version = "0.1.0"
 description = ""
 authors = ["grabber"]
 readme = "README.md"
 packages = [
     { include = "grabber/**/*.py" },
     { include = "assets/pages.txt" },
 ]
@@ -30,14 +30,15 @@
 olefile = "^0.47"
 pillow = "^10.3.0"
 telegraph = "^2.2.0"
 lxml = "^5.2.1"
 rich = "^13.7.1"
 colorlog = "^6.8.2"
 jinja2 = "^3.1.3"
+aiogram = "^3.4.1"
 
 [tool.poetry.group.dev.dependencies]
 ipython = "^8.18.0"
 nest-asyncio = "^1.5.6"
 pendulum = "3.0.0b1"
 ruff = "^0.3.7"
```

### Comparing `grabberlib-0.0.9/PKG-INFO` & `grabberlib-0.1.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: grabberlib
-Version: 0.0.9
+Version: 0.1.0
 Summary: 
 Author: grabber
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: aiogram (>=3.4.1,<4.0.0)
 Requires-Dist: alive-progress (>=3.1.5,<4.0.0)
 Requires-Dist: beautifulsoup4 (>=4.12.3,<5.0.0)
 Requires-Dist: casefy (>=0.1.7,<0.2.0)
 Requires-Dist: cement (>=3.0.8,<4.0.0)
 Requires-Dist: colorama (>=0.4.6,<0.5.0)
 Requires-Dist: colorlog (>=6.8.2,<7.0.0)
 Requires-Dist: defusedxml (>=0.7.1,<0.8.0)
```

