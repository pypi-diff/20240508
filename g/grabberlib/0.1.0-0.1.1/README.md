# Comparing `tmp/grabberlib-0.1.0.tar.gz` & `tmp/grabberlib-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grabberlib-0.1.0.tar", max compression
+gzip compressed data, was "grabberlib-0.1.1.tar", max compression
```

## Comparing `grabberlib-0.1.0.tar` & `grabberlib-0.1.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0        0 2024-05-03 14:50:36.715508 grabberlib-0.1.0/README.md
--rw-r--r--   0        0        0        1 2024-05-03 14:50:36.716140 grabberlib-0.1.0/assets/pages.txt
--rw-r--r--   0        0        0        0 2024-05-03 14:50:36.718507 grabberlib-0.1.0/grabber/__init__.py
--rw-r--r--   0        0        0     1690 2024-05-03 14:50:36.718702 grabberlib-0.1.0/grabber/__main__.py
--rw-r--r--   0        0        0        0 2024-05-03 14:50:36.718877 grabberlib-0.1.0/grabber/controllers/__init__.py
--rw-r--r--   0        0        0     5107 2024-05-03 14:50:36.719117 grabberlib-0.1.0/grabber/controllers/base.py
--rw-r--r--   0        0        0        0 2024-05-03 14:50:36.719286 grabberlib-0.1.0/grabber/core/__init__.py
--rw-r--r--   0        0        0        0 2024-05-03 14:50:36.719467 grabberlib-0.1.0/grabber/core/bot/__init__.py
--rw-r--r--   0        0        0     1184 2024-05-07 14:11:46.736435 grabberlib-0.1.0/grabber/core/bot/core.py
--rw-r--r--   0        0        0       65 2024-05-03 14:50:36.719818 grabberlib-0.1.0/grabber/core/exc.py
--rw-r--r--   0        0        0      696 2024-05-03 14:50:36.719968 grabberlib-0.1.0/grabber/core/settings.py
--rw-r--r--   0        0        0        0 2024-05-03 14:50:36.720132 grabberlib-0.1.0/grabber/core/sources/__init__.py
--rw-r--r--   0        0        0     3232 2024-05-07 14:22:47.160221 grabberlib-0.1.0/grabber/core/sources/everia.py
--rw-r--r--   0        0        0     3797 2024-05-08 11:40:49.252100 grabberlib-0.1.0/grabber/core/sources/graph.py
--rw-r--r--   0        0        0     4630 2024-05-08 11:42:28.376443 grabberlib-0.1.0/grabber/core/sources/khd.py
--rw-r--r--   0        0        0     3604 2024-05-03 14:50:36.720826 grabberlib-0.1.0/grabber/core/sources/nudecosplay.py
--rw-r--r--   0        0        0     3989 2024-05-03 14:50:36.720989 grabberlib-0.1.0/grabber/core/sources/xasiat.py
--rw-r--r--   0        0        0     4107 2024-05-03 14:50:36.721155 grabberlib-0.1.0/grabber/core/sources/xiuren.py
--rw-r--r--   0        0        0        1 2024-05-03 14:50:36.721312 grabberlib-0.1.0/grabber/core/sources/yellow.py
--rw-r--r--   0        0        0    16275 2024-05-03 14:50:36.721552 grabberlib-0.1.0/grabber/core/utils.py
--rw-r--r--   0        0        0      175 2024-05-08 11:41:48.914325 grabberlib-0.1.0/grabber/core/version.py
--rw-r--r--   0        0        0        0 2024-05-03 14:50:36.721870 grabberlib-0.1.0/grabber/templates/__init__.py
--rw-r--r--   0        0        0     1036 2024-05-08 11:41:57.715542 grabberlib-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1348 1970-01-01 00:00:00.000000 grabberlib-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-05-03 14:50:36.715508 grabberlib-0.1.1/README.md
+-rw-r--r--   0        0        0        1 2024-05-03 14:50:36.716140 grabberlib-0.1.1/assets/pages.txt
+-rw-r--r--   0        0        0        0 2024-05-03 14:50:36.718507 grabberlib-0.1.1/grabber/__init__.py
+-rw-r--r--   0        0        0     1690 2024-05-03 14:50:36.718702 grabberlib-0.1.1/grabber/__main__.py
+-rw-r--r--   0        0        0        0 2024-05-03 14:50:36.718877 grabberlib-0.1.1/grabber/controllers/__init__.py
+-rw-r--r--   0        0        0     5057 2024-05-08 12:59:24.763016 grabberlib-0.1.1/grabber/controllers/base.py
+-rw-r--r--   0        0        0        0 2024-05-03 14:50:36.719286 grabberlib-0.1.1/grabber/core/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-03 14:50:36.719467 grabberlib-0.1.1/grabber/core/bot/__init__.py
+-rw-r--r--   0        0        0      997 2024-05-08 13:00:46.779103 grabberlib-0.1.1/grabber/core/bot/core.py
+-rw-r--r--   0        0        0       65 2024-05-03 14:50:36.719818 grabberlib-0.1.1/grabber/core/exc.py
+-rw-r--r--   0        0        0      772 2024-05-08 11:57:16.753731 grabberlib-0.1.1/grabber/core/settings.py
+-rw-r--r--   0        0        0        0 2024-05-03 14:50:36.720132 grabberlib-0.1.1/grabber/core/sources/__init__.py
+-rw-r--r--   0        0        0     3543 2024-05-08 12:59:24.763764 grabberlib-0.1.1/grabber/core/sources/everia.py
+-rw-r--r--   0        0        0     2666 2024-05-08 12:55:29.819062 grabberlib-0.1.1/grabber/core/sources/graph.py
+-rw-r--r--   0        0        0     3061 2024-05-08 12:05:40.276104 grabberlib-0.1.1/grabber/core/sources/khd.py
+-rw-r--r--   0        0        0     2445 2024-05-08 12:59:24.762443 grabberlib-0.1.1/grabber/core/sources/nudecosplay.py
+-rw-r--r--   0        0        0     2818 2024-05-08 12:08:31.466179 grabberlib-0.1.1/grabber/core/sources/xasiat.py
+-rw-r--r--   0        0        0     3143 2024-05-08 12:49:26.255753 grabberlib-0.1.1/grabber/core/sources/xiuren.py
+-rw-r--r--   0        0        0        1 2024-05-03 14:50:36.721312 grabberlib-0.1.1/grabber/core/sources/yellow.py
+-rw-r--r--   0        0        0    19185 2024-05-08 13:07:33.380714 grabberlib-0.1.1/grabber/core/utils.py
+-rw-r--r--   0        0        0      175 2024-05-08 13:29:13.280795 grabberlib-0.1.1/grabber/core/version.py
+-rw-r--r--   0        0        0        0 2024-05-03 14:50:36.721870 grabberlib-0.1.1/grabber/templates/__init__.py
+-rw-r--r--   0        0        0     1036 2024-05-08 13:29:17.781585 grabberlib-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1348 1970-01-01 00:00:00.000000 grabberlib-0.1.1/PKG-INFO
```

### Comparing `grabberlib-0.1.0/grabber/__main__.py` & `grabberlib-0.1.1/grabber/__main__.py`

 * *Files identical despite different names*

### Comparing `grabberlib-0.1.0/grabber/controllers/base.py` & `grabberlib-0.1.1/grabber/controllers/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,15 +31,15 @@
             ### add a version banner
             (
                 ["-e", "--entity"],
                 {
                     "dest": "entity",
                     "type": str,
                     "help": "Webtsite name from where it will be download",
-               },
+                },
             ),
             (
                 ["-s", "--sources"],
                 {
                     "dest": "sources",
                     "type": str,
                     "help": "List of links",
@@ -147,10 +147,9 @@
             getter_images(
                 sources=sources,
                 entity=entity,
                 final_dest=folder,
                 save_to_telegraph=publish,
                 is_tag=is_tag,
                 limit=limit,
-                send_to_telegram=send_to_telegram,
                 telegraph_client=telegraph_client,
             )
```

### Comparing `grabberlib-0.1.0/grabber/core/bot/core.py` & `grabberlib-0.1.1/grabber/core/bot/core.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,32 +9,25 @@
     post_text: str,
     retry: Optional[bool] = False,
     posts_counter: Optional[int] = 0,
     retry_counter: Optional[int] = 0,
     sleep_time: Optional[int] = 0,
 ) -> None:
     try:
-        await send_message(
-            post_text=post_text,
-            retry=retry and retry_counter <= 50,
-            posts_counter=posts_counter,
-            retry_counter=retry_counter,
-        )
+        bot = Bot(token=f"{BOT_TOKEN}")
+        async with bot.context():
+            await bot.send_message(chat_id="@cspmst", text=post_text)
+            print(f"Post sent to the channel: {post_text}")
     except Exception:
         sleep_time = 15
         if retry or posts_counter >= 15:
             retry_counter += 1
             asyncio.sleep(sleep_time)
             print(f"Retry number {retry_counter} sending post to channel")
 
         await send_message(
             post_text=post_text,
             retry=retry and retry_counter <= 50,
             posts_counter=posts_counter,
             retry_counter=retry_counter,
-            sleep_time=sleep_time
+            sleep_time=sleep_time,
         )
-
-    bot  = Bot(token=f"{BOT_TOKEN}")
-    async with bot.context():
-        await bot.send_message(chat_id="@cspmst", text=post_text)
-        print(f"Post sent to the channel: {post_text}")
```

### Comparing `grabberlib-0.1.0/grabber/core/settings.py` & `grabberlib-0.1.1/grabber/core/settings.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import multiprocessing
 import pathlib
 
 from environs import Env
 
 env = Env()
 env.read_env()
 APP_ROOT = pathlib.Path(__file__).parent.parent.parent
@@ -9,14 +10,15 @@
 MEDIA_ROOT = APP_ROOT / "media"
 KEY = env.str("KEY", "default")
 BOT_TOKEN = env.str("BOT_TOKEN", "")
 TELEGRAPH_TOKEN = env.str("TELEGRAPH_TOKEN")
 SHORT_NAME = env.str("SHORT_NAME")
 AUTHOR_NAME = env.str("AUTHOR_NAME")
 AUTHOR_URL = env.str("AUTHOR_URL")
+DEFAULT_THREADS_NUMBER = multiprocessing.cpu_count()
 
 
 def get_media_root() -> pathlib.Path:
     USER_MEDIA_ROOT_PATH = env.str("USER_MEDIA_ROOT", None)
 
     if USER_MEDIA_ROOT_PATH is not None:
         media_root = pathlib.Path(USER_MEDIA_ROOT_PATH)
```

### Comparing `grabberlib-0.1.0/grabber/core/sources/everia.py` & `grabberlib-0.1.1/grabber/core/sources/everia.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,31 +1,29 @@
-import asyncio
-from time import sleep
+import pathlib
 from typing import List
 
 from telegraph import Telegraph
 from tqdm import tqdm
 
-from grabber.core.bot.core import send_message
 from grabber.core.utils import (
-    create_html_template,
-    create_page,
+    downloader,
     query_mapping,
     headers_mapping,
     get_tags,
     get_soup,
+    telegraph_uploader,
 )
 
 
 def get_pages_from_pagination(url: str) -> List[str]:
     pagination_pages_query = "div.oceanwp-pagination.clr ul.page-numbers a.page-numbers"
     articles_from_pagination_query = "div.entries article.blog-entry a"
     next_page_url_base = f"{url}page/"
     source_urls = set()
-    
+
     first_page = get_soup(url)
     articles = set(first_page.select(articles_from_pagination_query))
     pages = first_page.select(pagination_pages_query)
 
     if pages:
         pages_links = set()
         last_page = pages[-2]
@@ -44,61 +42,72 @@
     return source_urls
 
 
 def get_sources_for_everia(
     sources: List[str],
     entity: str,
     telegraph_client: Telegraph,
+    final_dest: str | pathlib.Path = "",
+    save_to_telegraph: bool | None = False,
     **kwargs,
 ) -> None:
-    is_tag = kwargs.get('is_tag', False)
+    is_tag = kwargs.get("is_tag", False)
     query, src_attr = query_mapping[entity]
     headers = headers_mapping.get(entity, None)
     title = None
-    posted_title = False
+    title_folder_mapping = {}
+    posts_sent_counter = 0
+    titles = []
+
+    if final_dest:
+        final_dest = pathlib.Path(final_dest)
+        if not final_dest.exists():
+            final_dest.mkdir(parents=True, exist_ok=True)
 
     if is_tag:
         soup = get_soup(target_url=sources[0], headers=headers)
         title = soup.get_text(strip=True).split(" – EVERIA.CLUB")[0]
         sources = list(get_pages_from_pagination(sources[0]))
 
     tqdm_sources_iterable = tqdm(
         enumerate(sources),
         total=len(sources),
         desc="Retrieving URLs...",
     )
-    is_tag = kwargs.get('is_tag', False)
-    posts_sent_counter = 0
 
     for idx, source_url in tqdm_sources_iterable:
         image_tags, soup = get_tags(source_url, headers=headers, query=query)
         page_title = soup.get_text(strip=True).split(" – EVERIA.CLUB")[0]
 
         if title is None:
             title = soup.get_text(strip=True)
+            titles.append(title)
 
         unique_img_urls = set()
-
         for idx, img_tag in enumerate(image_tags):
             img_src = img_tag.attrs[src_attr]
             img_name: str = img_src.split("/")[-1].split("?")[0]
             img_name = img_name.strip().rstrip()
             unique_img_urls.add((f"{page_title} {idx + 1}", img_src))
 
-        html_post = create_html_template(unique_img_urls)
-        post_url = create_page(title=page_title, html_content=html_post, telegraph_client=telegraph_client)
-        telegraph_post_link = f"{page_title} - {post_url}"
-
-        if posts_sent_counter == 10:
-            sleep(10)
-
-        try:
-            if not posted_title:
-                asyncio.run(send_message(title))
-                posted_title = True
+        tqdm_sources_iterable.set_description(f"Finished retrieving images for {title}")
 
-            asyncio.run(send_message(telegraph_post_link))
+        if final_dest:
+            folder_name = title.strip().rstrip()
+            title_dest = final_dest / folder_name
+            title_folder_mapping[title] = (unique_img_urls, title_dest)
+
+        if save_to_telegraph:
+            telegraph_uploader(
+                unique_img_urls=unique_img_urls,
+                page_title=page_title,
+                posts_sent_counter=posts_sent_counter,
+                telegraph_client=telegraph_client,
+            )
             posts_sent_counter += 1
-        except Exception:
-            sleep(20)
-            asyncio.run(send_message(telegraph_post_link))
 
+    if final_dest:
+        downloader(
+            titles=titles,
+            title_folder_mapping=title_folder_mapping,
+            headers=headers,
+        )
```

### Comparing `grabberlib-0.1.0/grabber/core/utils.py` & `grabberlib-0.1.1/grabber/core/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,15 +27,18 @@
 PAGINATION_BASE_URL_QUERY = "div.jeg_navigation.jeg_pagination a.page_number"
 POSTS_QUERY_XPATH = "/html/body/div[2]/div[5]/div/div[1]/div/div/div[2]/div/div/div[2]/div/div[1]/div/div/div/article/div/div/a"
 
 
 query_mapping = {
     "xiuren": ("div.content-inner img", "src"),
     "nudebird": ("div.thecontent a", "href"),
-    "nudecosplay": ("img[src^='https://static9.hentai-cosplays.com/'][alt^='PureMedia']", "src"),
+    "nudecosplay": (
+        "img[src^='https://static9.hentai-cosplays.com/'][alt^='PureMedia']",
+        "src",
+    ),
     "v2ph": ("div.photos-list.text-center img", "src"),  # Needs to handle pagination
     "cgcosplay": ("div.gallery-icon.portrait img", "src"),
     "mitaku": ("img.msacwl-img", "data-lazy"),
     "xasiat": ("div.images a", "href"),
     "telegraph": ("img", "src"),
     "4khd": (
         "div.is-layout-constrained.entry-content.wp-block-post-content img",
@@ -170,14 +173,44 @@
     target_url: str,
     headers: dict[str, str] | None = None,
 ) -> BeautifulSoup:
     response = requests.get(target_url, headers=headers)
     return BeautifulSoup(response.content, features="lxml")
 
 
+def downloader(
+    titles: List[str],
+    title_folder_mapping: Dict[str, Tuple[Tuple[str, str], pathlib.Path]],
+    headers: Optional[Dict[str, str]] = None,
+) -> None:
+    with ThreadPoolExecutor(max_workers=DEFAULT_THREADS_NUMBER) as executor:
+        # Dictionary to hold Future objects
+        futures_to_title = {}
+        future_counter = 0
+        for title in titles:
+            images_set, folder_dest = title_folder_mapping[title]
+            partial_download = partial(
+                download_images,
+                new_folder=folder_dest,
+                headers=headers,
+                title=title,
+            )
+            future = executor.submit(partial_download, images_set)
+            futures_to_title[future] = title
+            future_counter += 1
+
+        # Handling futures as they complete
+        for future in tqdm(
+            as_completed(futures_to_title),
+            total=future_counter,
+            desc=f"Retrieving {future_counter} tasks of downloading images",
+        ):
+            print(future.result())  # Get the result from the future object
+
+
 def download_images(
     images_set,
     new_folder: pathlib.Path,
     title: str,
     headers: Optional[Dict[str, str]] = None,
 ):
     """Download an image from a given URL and save it to the specified filename.
@@ -210,14 +243,75 @@
             resp.raw.decode_content = True
             shutil.copyfileobj(resp.raw, img_file)
 
     convert_from_webp_to_jpg(new_folder)
     return "Done"
 
 
+def telegraph_uploader(
+    unique_img_urls: Tuple[Tuple[str, str]],
+    page_title: str,
+    posts_sent_counter: Optional[int] = 0,
+    telegraph_client: Optional[Telegraph] = None,
+) -> None:
+    is_title_posted = False
+    if telegraph_client is None:
+        telegraph_client = get_new_telegraph_client()
+
+    posts = []
+    html_post = create_html_template(unique_img_urls)
+    post_url = create_page(
+        title=page_title, html_content=html_post, telegraph_client=telegraph_client
+    )
+    telegraph_post = f"{page_title} - {post_url}"
+    posts.append(telegraph_post)
+
+    if posts_sent_counter == 10:
+        sleep(10)
+
+    try:
+        if not is_title_posted:
+            asyncio.run(
+                send_message(
+                    post_text=page_title,
+                    retry=True,
+                    posts_counter=posts_sent_counter,
+                )
+            )
+            is_title_posted = True
+
+        asyncio.run(
+            send_message(
+                post_text=telegraph_post,
+                retry=True,
+                posts_counter=posts_sent_counter,
+            )
+        )
+    except Exception:
+        sleep(20)
+        asyncio.run(
+            send_message(
+                post_text=telegraph_post,
+                retry=True,
+                posts_counter=posts_sent_counter,
+            )
+        )
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
+
+
 def sort_file(file: pathlib.Path) -> str:
     filename = file.name.split(".")[0]
     filename = filename.zfill(2)
     return filename
 
 
 def convert_from_webp_to_jpg(folder: pathlib.Path) -> None:
@@ -253,38 +347,48 @@
 def upload_file(
     file: pathlib.Path,
     telegraph_client: Telegraph,
     try_again: Optional[bool] = True,
 ) -> Optional[str]:
     try:
         uploaded = telegraph_client.upload_file(file)
-    except (Exception, exceptions.TelegraphException, exceptions.RetryAfterError) as exc:
+    except (
+        Exception,
+        exceptions.TelegraphException,
+        exceptions.RetryAfterError,
+    ) as exc:
         error_message = str(exc)
-        if 'try again' in error_message.lower() or 'retry' in error_message.lower():
+        if "try again" in error_message.lower() or "retry" in error_message.lower():
             sleep(5)
             if try_again:
                 telegraph_client = get_new_telegraph_client()
-                return upload_file(file=file, telegraph_client=telegraph_client, try_again=False)
+                return upload_file(
+                    file=file, telegraph_client=telegraph_client, try_again=False
+                )
         return
     if uploaded:
         return uploaded[0]["src"]
 
 
 def create_page(
     title: str,
     html_content: str,
     telegraph_client: Telegraph,
     try_again: Optional[bool] = True,
 ) -> str:
     try:
         page = telegraph_client.create_page(title=title, html_content=html_content)
         return page["url"]
-    except (Exception, exceptions.TelegraphException, exceptions.RetryAfterError) as exc:
+    except (
+        Exception,
+        exceptions.TelegraphException,
+        exceptions.RetryAfterError,
+    ) as exc:
         error_message = str(exc)
-        if 'try again' in error_message.lower() or 'retry' in error_message.lower():
+        if "try again" in error_message.lower() or "retry" in error_message.lower():
             sleep(5)
             if try_again:
                 telegraph_client = get_new_telegraph_client()
                 return create_page(
                     title=title,
                     html_content=html_content,
                     telegraph_client=telegraph_client,
```

### Comparing `grabberlib-0.1.0/pyproject.toml` & `grabberlib-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "grabberlib"
-version = "0.1.0"
+version = "0.1.1"
 description = ""
 authors = ["grabber"]
 readme = "README.md"
 packages = [
     { include = "grabber/**/*.py" },
     { include = "assets/pages.txt" },
 ]
@@ -19,15 +19,15 @@
 httpx = "^0.23.3"
 patool = "^2.1.1"
 psycopg = {extras = ["binary", "pool"], version = "^3.1.13"}
 python-twitter = "^3.5"
 requests = "^2.31.0"
 requests-html = "^0.10.0"
 tenacity = "^8.2.3"
-tqdm = "^4.66.2"
+tqdm = "^4.66.4"
 unipath = "^1.1"
 cement = "^3.0.8"
 defusedxml = "^0.7.1"
 olefile = "^0.47"
 pillow = "^10.3.0"
 telegraph = "^2.2.0"
 lxml = "^5.2.1"
```

### Comparing `grabberlib-0.1.0/PKG-INFO` & `grabberlib-0.1.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grabberlib
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: grabber
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
@@ -26,12 +26,12 @@
 Requires-Dist: psycopg[binary,pool] (>=3.1.13,<4.0.0)
 Requires-Dist: python-twitter (>=3.5,<4.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: requests-html (>=0.10.0,<0.11.0)
 Requires-Dist: rich (>=13.7.1,<14.0.0)
 Requires-Dist: telegraph (>=2.2.0,<3.0.0)
 Requires-Dist: tenacity (>=8.2.3,<9.0.0)
-Requires-Dist: tqdm (>=4.66.2,<5.0.0)
+Requires-Dist: tqdm (>=4.66.4,<5.0.0)
 Requires-Dist: unipath (>=1.1,<2.0)
 Description-Content-Type: text/markdown
```

