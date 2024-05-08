# Comparing `tmp/webtoonscraper-3.3.0.tar.gz` & `tmp/webtoonscraper-3.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webtoonscraper-3.3.0.tar", max compression
+gzip compressed data, was "webtoonscraper-3.3.1.tar", max compression
```

## Comparing `webtoonscraper-3.3.0.tar` & `webtoonscraper-3.3.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0    11558 2024-01-07 03:10:43.270352 webtoonscraper-3.3.0/LICENSE
--rw-r--r--   0        0        0     2068 2024-05-01 05:31:12.217065 webtoonscraper-3.3.0/pyproject.toml
--rw-r--r--   0        0        0     5752 2024-05-01 05:31:12.218074 webtoonscraper-3.3.0/README_build.md
--rw-r--r--   0        0        0     2657 2024-04-22 17:41:08.478691 webtoonscraper-3.3.0/WebtoonScraper/__init__.py
--rw-r--r--   0        0        0    14410 2024-04-23 13:21:19.844233 webtoonscraper-3.3.0/WebtoonScraper/__main__.py
--rw-r--r--   0        0        0    18848 2024-04-22 17:55:56.044946 webtoonscraper-3.3.0/WebtoonScraper/directory_merger.py
--rw-r--r--   0        0        0     5371 2024-05-01 05:28:28.979448 webtoonscraper-3.3.0/WebtoonScraper/exceptions.py
--rw-r--r--   0        0        0      798 2024-05-01 05:30:04.936242 webtoonscraper-3.3.0/WebtoonScraper/miscs.py
--rw-r--r--   0        0        0        0 2023-07-29 17:12:08.910678 webtoonscraper-3.3.0/WebtoonScraper/py.typed
--rw-r--r--   0        0        0    33560 2024-05-01 05:25:46.292406 webtoonscraper-3.3.0/WebtoonScraper/scrapers/_01_scraper.py
--rw-r--r--   0        0        0    16059 2024-05-01 01:44:26.897004 webtoonscraper-3.3.0/WebtoonScraper/scrapers/_02_naver_webtoon.py
--rw-r--r--   0        0        0     3923 2024-04-21 10:34:02.155922 webtoonscraper-3.3.0/WebtoonScraper/scrapers/_03_webtoon_originals.py
--rw-r--r--   0        0        0     4955 2024-04-29 14:31:05.710804 webtoonscraper-3.3.0/WebtoonScraper/scrapers/_04_bufftoon.py
--rw-r--r--   0        0        0     6965 2024-04-22 17:42:46.788825 webtoonscraper-3.3.0/WebtoonScraper/scrapers/_05_naver_post.py
--rw-r--r--   0        0        0     2597 2024-04-21 03:00:08.411749 webtoonscraper-3.3.0/WebtoonScraper/scrapers/_06_naver_game.py
--rw-r--r--   0        0        0    18223 2024-04-22 13:53:52.205309 webtoonscraper-3.3.0/WebtoonScraper/scrapers/_07_lezhin_comics.py
--rw-r--r--   0        0        0     7413 2024-05-01 05:26:01.233128 webtoonscraper-3.3.0/WebtoonScraper/scrapers/_07_lezhin_unshuffler.py
--rw-r--r--   0        0        0    11670 2024-04-22 17:37:35.861653 webtoonscraper-3.3.0/WebtoonScraper/scrapers/_08_kakaopage.py
--rw-r--r--   0        0        0     6083 2024-04-29 14:23:23.280559 webtoonscraper-3.3.0/WebtoonScraper/scrapers/_09_naver_blog.py
--rw-r--r--   0        0        0     4177 2024-04-21 14:40:26.587642 webtoonscraper-3.3.0/WebtoonScraper/scrapers/_10_tistory.py
--rw-r--r--   0        0        0     9243 2024-04-22 17:36:43.427570 webtoonscraper-3.3.0/WebtoonScraper/scrapers/_11_kakao_webtoon.py
--rw-r--r--   0        0        0     1043 2024-04-21 03:02:03.822936 webtoonscraper-3.3.0/WebtoonScraper/scrapers/__init__.py
--rw-r--r--   0        0        0     6871 2024-04-29 15:39:55.842906 webtoonscraper-3.3.0/WebtoonScraper/webtoon.py
--rw-r--r--   0        0        0    18921 2024-04-22 17:42:15.193830 webtoonscraper-3.3.0/WebtoonScraper/webtoon_viewer.py
--rw-r--r--   0        0        0     7152 1970-01-01 00:00:00.000000 webtoonscraper-3.3.0/PKG-INFO
+-rw-r--r--   0        0        0    11558 2024-01-07 03:10:43.270352 webtoonscraper-3.3.1/LICENSE
+-rw-r--r--   0        0        0     2068 2024-05-08 21:28:13.505897 webtoonscraper-3.3.1/pyproject.toml
+-rw-r--r--   0        0        0     5706 2024-05-08 21:28:13.507898 webtoonscraper-3.3.1/README_build.md
+-rw-r--r--   0        0        0     2657 2024-04-22 17:41:08.478691 webtoonscraper-3.3.1/WebtoonScraper/__init__.py
+-rw-r--r--   0        0        0    12293 2024-05-02 04:33:38.407650 webtoonscraper-3.3.1/WebtoonScraper/__main__.py
+-rw-r--r--   0        0        0    18573 2024-05-08 15:36:39.306861 webtoonscraper-3.3.1/WebtoonScraper/directory_merger.py
+-rw-r--r--   0        0        0     5371 2024-05-02 05:00:01.499595 webtoonscraper-3.3.1/WebtoonScraper/exceptions.py
+-rw-r--r--   0        0        0      798 2024-05-08 21:27:55.101417 webtoonscraper-3.3.1/WebtoonScraper/miscs.py
+-rw-r--r--   0        0        0        0 2023-07-29 17:12:08.910678 webtoonscraper-3.3.1/WebtoonScraper/py.typed
+-rw-r--r--   0        0        0    33566 2024-05-02 05:18:11.710249 webtoonscraper-3.3.1/WebtoonScraper/scrapers/_01_scraper.py
+-rw-r--r--   0        0        0    16059 2024-05-01 01:44:26.897004 webtoonscraper-3.3.1/WebtoonScraper/scrapers/_02_naver_webtoon.py
+-rw-r--r--   0        0        0     3923 2024-04-21 10:34:02.155922 webtoonscraper-3.3.1/WebtoonScraper/scrapers/_03_webtoon_originals.py
+-rw-r--r--   0        0        0     4955 2024-04-29 14:31:05.710804 webtoonscraper-3.3.1/WebtoonScraper/scrapers/_04_bufftoon.py
+-rw-r--r--   0        0        0     6965 2024-04-22 17:42:46.788825 webtoonscraper-3.3.1/WebtoonScraper/scrapers/_05_naver_post.py
+-rw-r--r--   0        0        0     2597 2024-04-21 03:00:08.411749 webtoonscraper-3.3.1/WebtoonScraper/scrapers/_06_naver_game.py
+-rw-r--r--   0        0        0    18211 2024-05-02 05:16:43.104078 webtoonscraper-3.3.1/WebtoonScraper/scrapers/_07_lezhin_comics.py
+-rw-r--r--   0        0        0     7387 2024-05-02 05:00:14.974666 webtoonscraper-3.3.1/WebtoonScraper/scrapers/_07_lezhin_unshuffler.py
+-rw-r--r--   0        0        0    11670 2024-04-22 17:37:35.861653 webtoonscraper-3.3.1/WebtoonScraper/scrapers/_08_kakaopage.py
+-rw-r--r--   0        0        0     6083 2024-04-29 14:23:23.280559 webtoonscraper-3.3.1/WebtoonScraper/scrapers/_09_naver_blog.py
+-rw-r--r--   0        0        0     4177 2024-04-21 14:40:26.587642 webtoonscraper-3.3.1/WebtoonScraper/scrapers/_10_tistory.py
+-rw-r--r--   0        0        0     9243 2024-04-22 17:36:43.427570 webtoonscraper-3.3.1/WebtoonScraper/scrapers/_11_kakao_webtoon.py
+-rw-r--r--   0        0        0     1043 2024-05-02 04:58:45.460677 webtoonscraper-3.3.1/WebtoonScraper/scrapers/__init__.py
+-rw-r--r--   0        0        0     6871 2024-04-29 15:39:55.842906 webtoonscraper-3.3.1/WebtoonScraper/webtoon.py
+-rw-r--r--   0        0        0    18889 2024-05-02 04:41:16.651705 webtoonscraper-3.3.1/WebtoonScraper/webtoon_viewer.py
+-rw-r--r--   0        0        0     7106 1970-01-01 00:00:00.000000 webtoonscraper-3.3.1/PKG-INFO
```

### Comparing `webtoonscraper-3.3.0/LICENSE` & `webtoonscraper-3.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `webtoonscraper-3.3.0/pyproject.toml` & `webtoonscraper-3.3.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "WebtoonScraper"
 # Do not change this version manually. This will be matched with WebtoonScraper.__version__ automatically.
-version = "3.3.0"
+version = "3.3.1"
 description = "Scraping webtoons with ease."
 authors = ["ilotoki0804 <ilotoki0804@gmail.com>"]
 license = "Apache-2.0"
 readme = "README_build.md"
 keywords = [
     "Webtoon",
     "Webtoon Scraper",
```

### Comparing `webtoonscraper-3.3.0/README_build.md` & `webtoonscraper-3.3.1/README_build.md`

 * *Files 1% similar despite different names*

```diff
@@ -77,17 +77,17 @@
 
 ```console
 webtoon download "https://comic.naver.com/webtoon/list?titleId=819217"
 ```
 
 만약 더 많은 WebtoonScraper의 기능(범위 설정 다운로드, 모아서 보기, 다운로드할 디렉토리 설정, 에피소드 리스팅, 파이썬으로 사용 등)을 알고 싶거나 위에서 소개한 방식으로는 잘 작동하지 않는 경우(특히 버프툰, 레진코믹스의 경우 추가적인 설정이 필수적입니다.)에는 [`사용 방법` 문서](https://github.com/ilotoki0804/WebtoonScraper/blob/master/docs/how_to_use.md)를 참고해 주세요.
 
-## 이 라이브러리가 다운로드 가능한 웹툰/에피소드의 종류
+## 다운로드 가능한 웹툰/에피소드의 종류
 
-[이 라이브러리가 다운로드 가능한 웹툰/에피소드의 종류 문서](https://github.com/ilotoki0804/WebtoonScraper/blob/master/docs/download_availability.md)를 참고하세요.
+[다운로드 가능한 웹툰/에피소드의 종류 문서](https://github.com/ilotoki0804/WebtoonScraper/blob/master/docs/download_availability.md)를 참고하세요.
 
 ## Build from source
 
 우선 git과 python을 설치하고 레포지토리를 클론하세요.
 
 ```console
 git clone https://github.com/ilotoki0804/WebtoonScraper.git
```

### Comparing `webtoonscraper-3.3.0/WebtoonScraper/__init__.py` & `webtoonscraper-3.3.1/WebtoonScraper/__init__.py`

 * *Files identical despite different names*

### Comparing `webtoonscraper-3.3.0/WebtoonScraper/__main__.py` & `webtoonscraper-3.3.1/WebtoonScraper/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,21 +12,15 @@
 from typing import Any, Callable, Literal
 
 from rich.console import Console
 from rich.table import Table
 
 import WebtoonScraper
 from WebtoonScraper import __version__, webtoon
-from WebtoonScraper.directory_merger import (
-    MERGED_WEBTOON_DIRECTORY,
-    NORMAL_WEBTOON_DIRECTORY,
-    ContainerStates,
-    check_container_state,
-    select_from_directory,
-)
+from WebtoonScraper.directory_merger import select_from_directory
 from WebtoonScraper.miscs import EpisodeNoRange, WebtoonId, logger
 from WebtoonScraper.scrapers import CommentsDownloadOption
 
 # currently Lezhin uses only lower case alphabet, numbers, and underscore. Rest of them are added for just in case.
 ACCEPTABLE_CHARS = set("abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789-_")
 
 
@@ -150,15 +144,15 @@
                 )
 
             case _:
                 SEP = "', '"
                 return (
                     f"⚠️  Extra dependencies '{SEP.join(missing_dependencies)}' are not installed.\n"
                     "You won't be able to download webtoons from following platforms: "
-                    f"'{SEP.join(ALL_DEPENDENCIES[missing] for missing in missing_dependencies)}'."
+                    f"'{', '.join(ALL_DEPENDENCIES[missing] for missing in missing_dependencies)}'."
                 )
 
     return f"WebtoonScraper {__version__} of Python {sys.version} at {str(files(WebtoonScraper))}\n{check_imported()}"
 
 
 parser = argparse.ArgumentParser(
     prog="WebtoonScraper",
@@ -317,72 +311,14 @@
         scraper.download_webtoon(
             args.range,
             merge_number=args.merge_number,
             add_viewer=True,
         )
 
 
-CONTAINER_STATE_PER_ARGS: dict[str, ContainerStates] = {
-    "m": NORMAL_WEBTOON_DIRECTORY,
-    "merge": NORMAL_WEBTOON_DIRECTORY,
-    "r": MERGED_WEBTOON_DIRECTORY,
-    "restore": MERGED_WEBTOON_DIRECTORY,
-}
-
-ABBR_TO_FULL_STATE: dict[str, Literal["merge", "restore", "auto"]] = {
-    "m": "merge",
-    "r": "restore",
-    "a": "auto",
-}
-
-
-CONTAINER_STATE_TO_DO_STATE: dict[ContainerStates, Literal["merge", "restore"]] = {
-    NORMAL_WEBTOON_DIRECTORY: "merge",
-    MERGED_WEBTOON_DIRECTORY: "restore",
-}
-
-
-def get_state(source_directory: Path) -> ContainerStates:
-    states: dict[Path, ContainerStates] = {
-        webtoon_directory: check_container_state(webtoon_directory) for webtoon_directory in source_directory.iterdir()
-    }
-    all_unique_states = set(states.values())
-    if len(all_unique_states) != 1:
-        raise ValueError(
-            "All webtoons in source directory should have same state when using 'auto' action.\n"
-            "Please specify --action(-a) or check directory state."
-            f"States: {all_unique_states}"
-        )
-
-    (directories_state,) = all_unique_states
-    return directories_state
-
-
-def get_string_todo(state: ContainerStates) -> Literal["merge", "restore"]:
-    try:
-        return CONTAINER_STATE_TO_DO_STATE[state]
-    except KeyError:
-        raise ValueError(f"State {state} is not supported.")
-
-
-def list_directories(parent_directory: Path) -> None:
-    table = Table(show_header=True, header_style="bold blue", box=None)
-    table.add_column("Webtoon Directory Name", style="bold")
-    table.add_column("Directory State")
-    table.add_column("Action If Auto")
-    for webtoon_directory in parent_directory.iterdir():
-        directory_state = check_container_state(webtoon_directory)
-        table.add_row(
-            webtoon_directory.name,
-            directory_state,
-            CONTAINER_STATE_TO_DO_STATE.get(directory_state),
-        )
-    Console().print(table)
-
-
 def parse_merge(args: argparse.Namespace) -> None:
     select_from_directory(
         args.webtoons_directory_name,
         args.target_parent_directory,
         True,
         args.merge_number,
     )
```

### Comparing `webtoonscraper-3.3.0/WebtoonScraper/directory_merger.py` & `webtoonscraper-3.3.1/WebtoonScraper/directory_merger.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,27 +8,23 @@
 from collections import defaultdict
 from pathlib import Path
 from typing import Final, Literal, TypeAlias
 
 from .exceptions import DirectoryStateUnmatchedError, Unreachable
 from .miscs import logger
 
-# container는 file을 담고 있는 것을 의미합니다.
-# container에 들어가는 file이 directory일 수 있기 때문에
-# directory라는 말을 사용할 경우 오해가 생길 수 있어 container라는 유사어로 대체하여 표현합니다.
-# episode directory 같은 경우엔 image의 container이면서도 webtoon directory의 content입니다.
 NORMAL_IMAGE: Final = "normal_image"
 NORMAL_EPISODE_DIRECTORY: Final = "normal_episode_directory"
 NORMAL_WEBTOON_DIRECTORY: Final = "normal_webtoon_directory"
 
 MERGED_IMAGE: Final = "merged_image"
 MERGED_EPISODE_DIRECTORY: Final = "merged_episode_directory"
 MERGED_WEBTOON_DIRECTORY: Final = "merged_webtoon_directory"
 
-# 만약 이름을 WEBTOONS_DIRECTORY로 한다면 매우 햇갈릴 가능성이 높기에 굳이 WEBTOON_DIRECTORY_CONTAINER라는 이름을 사용합니다.
+# 만약 이름을 WEBTOONS_DIRECTORY로 한다면 매우 햇갈릴 가능성이 높기에 대신 WEBTOON_DIRECTORY_CONTAINER라는 이름을 사용함
 WEBTOON_DIRECTORY: Final = "webtoon_directory"
 WEBTOON_DIRECTORY_CONTAINER: Final = "webtoon_directory_container"
 
 NOT_MATCHED: Final = "not_matched"
 
 ContainerStates = Literal[
     "normal_webtoon_directory",
@@ -53,43 +49,68 @@
     NORMAL_IMAGE: NORMAL_EPISODE_DIRECTORY,
     NORMAL_EPISODE_DIRECTORY: NORMAL_WEBTOON_DIRECTORY,
     MERGED_IMAGE: MERGED_EPISODE_DIRECTORY,
     MERGED_EPISODE_DIRECTORY: MERGED_WEBTOON_DIRECTORY,
     WEBTOON_DIRECTORY: WEBTOON_DIRECTORY_CONTAINER,
 }
 
-CONTAINER_TO_FILE: Final[dict[ContainerStates, FileStates]] = {value: key for key, value in FILE_TO_CONTAINER.items()}
 
-
-# 각 라인 끝 주석 처리된 부분: 덜 예민한 버전(거의 대부분 매치 개수 관련임)의 regex; 만약 현재 regex가 잘 작동하지 않을 경우 사용할 것. 없을 수도 있음.
-webtoon_regexes: dict[FileStates, re.Pattern[str]] = {
-    NORMAL_IMAGE: re.compile(r"^(?P<image_no>\d{3})[.](?P<extension>[a-zA-Z0-9]{3,4})$"),  # 023.jpg
-    # ^(?P<image_no>\d+)[.](?P<extension>[a-zA-Z0-9]+)$
-    NORMAL_EPISODE_DIRECTORY: re.compile(r"^(?P<episode_no>\d{4})\. (?P<episode_name>.+)$"),  # 0001. episode_name
-    MERGED_IMAGE: re.compile(
-        r"^(?P<episode_no>\d{4})[.](?P<image_no>\d{3})[.] (?P<episode_name>.+)[.](?P<extension>[a-zA-Z]{3,4})$"
-    ),  # 0001.001. episode_name.jpg
-    # ^(?P<episode_no>\d+)[.](?P<image_no>\d+)[.] (?P<episode_name>.+)[.](?P<extension>[a-zA-Z]+)$
-    MERGED_EPISODE_DIRECTORY: re.compile(r"^(?P<from>\d{4})~(?P<to>\d{4})$"),  # 0001~0005
-    # ^(?P<from>\d+)~(?P<to>\d+)$
-    WEBTOON_DIRECTORY: re.compile(
-        r"^(?P<webtoon_name>.+)[(](?P<titleid>(?!merged).+?)[)](?:[(]merged[)])?$"
-    ),  # webtoon_name(titleid)[(merged)]
+# fmt: off
+DIRECTORY_PATTERNS: dict[FileStates, re.Pattern[str]] = {
+    # 023.jpg
+    NORMAL_IMAGE: re.compile(r"^(?P<image_no>\d{3})[.](?P<extension>[a-zA-Z0-9]{3,4})$"),
+    # 0001. episode_name
+    NORMAL_EPISODE_DIRECTORY: re.compile(r"^(?P<episode_no>\d{4})\. (?P<episode_name>.+)$"),
+    # 0001.001. episode_name.jpg
+    MERGED_IMAGE: re.compile(r"^(?P<episode_no>\d{4})[.](?P<image_no>\d{3})[.] (?P<episode_name>.+)[.](?P<extension>[a-zA-Z]{3,4})$"),
+    # 0001~0005
+    MERGED_EPISODE_DIRECTORY: re.compile(r"^(?P<from>\d{4})~(?P<to>\d{4})$"),
+    # webtoon_name(titleid[, HD][, shuffled])
+    WEBTOON_DIRECTORY: re.compile(r"^(?P<webtoon_name>.+)[(](?P<titleid>.+?)(?:, (?:HD|shuffled))*[)]$"),
+}
+DIRECTORY_PATTERNS_TOLERANT: dict[FileStates, re.Pattern[str]] = {
+    # 023.jpg
+    NORMAL_IMAGE: re.compile(r"^(?P<image_no>\d+)[.](?P<extension>[a-zA-Z0-9]+)$"),
+    # 0001. episode_name
+    NORMAL_EPISODE_DIRECTORY: re.compile(r"^(?P<episode_no>\d+)\. (?P<episode_name>.+)$"),
+    # 0001.001. episode_name.jpg
+    MERGED_IMAGE: re.compile(r"^(?P<episode_no>\d+)[.](?P<image_no>\d+)[.] (?P<episode_name>.+)[.](?P<extension>[a-zA-Z]+)$"),
+    # 0001~0005
+    MERGED_EPISODE_DIRECTORY: re.compile(r"^(?P<from>\d+)~(?P<to>\d+)$"),
+    # webtoon_name(titleid[, meta]*)
+    WEBTOON_DIRECTORY: re.compile(r"^(?P<webtoon_name>.+)[(](?P<titleid>.+?)(?:, (?:\w+))*[)]$"),
 }
+# fmt: on
+
+
+def _directories_and_files_of(
+    directory: PathOrStr,
+    treat_underscored_directories_as_file: bool = True,
+    /,
+) -> tuple[list[Path], list[Path]]:
+    directories: list[Path] = []
+    files: list[Path] = []
+    for path in Path(directory).iterdir():
+        is_underscored = (
+            treat_underscored_directories_as_file and path.name.startswith("_") and not path.name.startswith("__")
+        )
+        if path.is_dir() and not is_underscored:
+            directories.append(path)
+        else:
+            files.append(path)
+    return sorted(directories), sorted(files)
 
 
 def select_from_directory(
     source_parent_directory: Path,
     target_parent_directory: Path | None,
     rebuild_webtoon_viewer: bool,
     merge_number: int | None = None,
-):
-    directories, files = _iterdir_seperating_directories_and_files(
-        source_parent_directory, treat_underscored_directories_as_file=False
-    )
+) -> None:
+    directories, files = _directories_and_files_of(source_parent_directory, False)
 
     not_webtoon_directories: list[Path] = []
     normal_webtoon_directories: list[Path] = []
     merged_webtoon_directories: list[Path] = []
     for directory in directories:
         container_state = check_container_state(directory)
         if container_state == NORMAL_WEBTOON_DIRECTORY:
@@ -202,15 +223,15 @@
 
         for operated_path in operated_paths:
             if (operated_path / "webtoon.html").exists():
                 add_html_webtoon_viewer(operated_path)
 
 
 def _get_episode_no(directory_name: str) -> int:
-    directory_name_matched = webtoon_regexes[NORMAL_EPISODE_DIRECTORY].match(directory_name)
+    directory_name_matched = DIRECTORY_PATTERNS[NORMAL_EPISODE_DIRECTORY].match(directory_name)
     assert directory_name_matched is not None, f"Directory state is invalid. {directory_name = }"
     return int(directory_name_matched.group("episode_no"))
 
 
 def merge_webtoon(
     source_webtoon_directory: Path,
     target_webtoon_directory: Path | None,
@@ -241,15 +262,15 @@
             + (" Maybe what you need was restore_webtoon." if directory_state == MERGED_WEBTOON_DIRECTORY else "")
             + f"\nsource webtoon directory: {source_webtoon_directory}"
         )
 
     # source_webtoon_directory == target_webtoon_directory인 경우 때문에 exist_ok는 True여야 한다.
     target_webtoon_directory.mkdir(parents=True, exist_ok=True)
 
-    directories, files = _iterdir_seperating_directories_and_files(source_webtoon_directory)
+    directories, files = _directories_and_files_of(source_webtoon_directory)
 
     # 디렉토리 그룹핑
     grouped_directories: defaultdict[int, list[Path]] = defaultdict(list)
     for directory in directories:
         episode_no = _get_episode_no(directory.name)
         grouped_directories[(episode_no - 1) // merge_number].append(directory)
 
@@ -279,18 +300,18 @@
             os.rename(file, target_webtoon_directory / file.name)
         if not os.listdir(source_webtoon_directory):
             source_webtoon_directory.rmdir()
 
 
 def _get_merged_image_name(image_name: str, episode_name: str) -> str:
     """merged 상태의 image가 가져야 할 이름을 내놓습니다."""
-    image_name_processed: re.Match[str] | None = webtoon_regexes[NORMAL_IMAGE].match(image_name)
-    episode_name_processed: re.Match[str] | None = webtoon_regexes[NORMAL_EPISODE_DIRECTORY].match(episode_name)
+    image_name_processed: re.Match[str] | None = DIRECTORY_PATTERNS[NORMAL_IMAGE].match(image_name)
+    episode_name_processed: re.Match[str] | None = DIRECTORY_PATTERNS[NORMAL_EPISODE_DIRECTORY].match(episode_name)
     if not episode_name_processed:
-        if webtoon_regexes[MERGED_EPISODE_DIRECTORY].match(episode_name):
+        if DIRECTORY_PATTERNS[MERGED_EPISODE_DIRECTORY].match(episode_name):
             raise ValueError(
                 "Episode name is not valid. It's because you tried to merge already merged webtoon directory."
             )
         raise ValueError(f"Episode name is not valid. Episode name: {episode_name}")
     if not image_name_processed:
         raise ValueError(f"Image name is not vaild. Image name: {image_name}")
 
@@ -301,34 +322,18 @@
 
     return f"{episode_no}.{image_no}. {episode_name}.{image_extension}"
 
 
 ############### CHECKING FUNCTIONALITY ###############
 
 
-def _iterdir_seperating_directories_and_files(
-    directory: PathOrStr,
-    treat_underscored_directories_as_file: bool = True,
-) -> tuple[list[Path], list[Path]]:
-    directories: list[Path] = []
-    files: list[Path] = []
-    for path in Path(directory).iterdir():
-        if path.is_dir() and not (
-            treat_underscored_directories_as_file and path.name.startswith("_") and not path.name.startswith("__")
-        ):
-            directories.append(path)
-        else:
-            files.append(path)
-    return directories, files
-
-
 def check_filename_state(file_or_directory_name: str) -> FileStates:
     """한 파일(혹은 디렉토리) 이름의 상태를 확인합니다."""
     # sourcery skip: use-next; for simplicity and extensibility, I decide to not apply 'use-next'
-    for state_name, regex in webtoon_regexes.items():
+    for state_name, regex in DIRECTORY_PATTERNS.items():
         if regex.match(file_or_directory_name):
             return state_name
     return NOT_MATCHED
 
 
 def check_container_state(directory: PathOrStr, *, warn: bool = False) -> ContainerStates:
     """해당 path에 있는 디렉토리의 상태를 확인합니다."""
@@ -339,34 +344,35 @@
         return NOT_MATCHED
 
     if directory.is_file():
         if warn:
             logger.warning(f"It looks like the file({directory}) is not a directory.")
         return NOT_MATCHED
 
-    directories, _ = _iterdir_seperating_directories_and_files(directory)
+    directories, files = _directories_and_files_of(directory)
 
     if not directories:
-        if warn:
-            logger.warning(f"It looks like the directory({directory}) is empty. It cannot be something")
+        states: set[FileStates] = {check_filename_state(file.name) for file in files if not file.name.startswith("_")}
+        if len(states) == 1:
+            return FILE_TO_CONTAINER.get(states.pop(), NOT_MATCHED)
         return NOT_MATCHED
 
-    for state_name, regex in webtoon_regexes.items():
+    for state_name, regex in DIRECTORY_PATTERNS.items():
         # 매치되지 '않은' 것의 개수를 세는 것을 주의!!!
         if not sum(not regex.match(episode_or_image.name) for episode_or_image in directories):
             return FILE_TO_CONTAINER.get(state_name, NOT_MATCHED)
 
     return NOT_MATCHED
 
 
 ############### RESTORE FUNCTIONALITY ###############
 
 
-def _get_directory_and_image_name_from_merged_image_name(merged_image_name: str):
-    image_info = webtoon_regexes[MERGED_IMAGE].match(merged_image_name)
+def restore_name(merged_image_name: str):
+    image_info = DIRECTORY_PATTERNS[MERGED_IMAGE].match(merged_image_name)
     assert image_info, "image name is not merged image."
     episode_no = image_info.group("episode_no")
     image_no = image_info.group("image_no")
     episode_name = image_info.group("episode_name")
     image_extension = image_info.group("extension")
 
     new_episode_directory_name = f"{episode_no}. {episode_name}"
@@ -386,21 +392,18 @@
     if directory_state != MERGED_WEBTOON_DIRECTORY:
         raise DirectoryStateUnmatchedError(
             f"State of directory is {directory_state}, which cannot be restored."
             + (" Maybe what you need was merge_webtoon." if directory_state == NORMAL_WEBTOON_DIRECTORY else "")
             + f"\nsorce webtoon directory: {source_webtoon_directory}"
         )
 
-    directories, files = _iterdir_seperating_directories_and_files(source_webtoon_directory)
+    directories, files = _directories_and_files_of(source_webtoon_directory)
     for directory in directories:
         for image_name in os.listdir(directory):
-            (
-                target_episode_directory_name,
-                target_image_name,
-            ) = _get_directory_and_image_name_from_merged_image_name(image_name)
+            target_episode_directory_name, target_image_name = restore_name(image_name)
             target_episode_directory = target_webtoon_directory / target_episode_directory_name
             target_episode_directory.mkdir(exist_ok=True)
             os.rename(directory / image_name, target_episode_directory / target_image_name)
         directory.rmdir()
 
     # 남은 폴더가 아닌 파일들 옮기기
     if source_webtoon_directory != target_webtoon_directory and files:
```

### Comparing `webtoonscraper-3.3.0/WebtoonScraper/exceptions.py` & `webtoonscraper-3.3.1/WebtoonScraper/exceptions.py`

 * *Files identical despite different names*

### Comparing `webtoonscraper-3.3.0/WebtoonScraper/miscs.py` & `webtoonscraper-3.3.1/WebtoonScraper/miscs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 from typing import TYPE_CHECKING, Iterable, TypeAlias
 
 from rich.logging import RichHandler
 
 __url__ = "https://github.com/ilotoki0804/WebtoonScraper"
-__version_info__ = (3, 3, 0)
+__version_info__ = (3, 3, 1)
 __version__ = str.join(".", map(str, __version_info__))
 
 if TYPE_CHECKING:
     from .scrapers import NaverBlogWebtoonId as _NaverBlogWebtoonId
     from .scrapers import NaverPostWebtoonId as _NaverPostWebtoonId
 
 WebtoonId: TypeAlias = (
```

### Comparing `webtoonscraper-3.3.0/WebtoonScraper/scrapers/_01_scraper.py` & `webtoonscraper-3.3.1/WebtoonScraper/scrapers/_01_scraper.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,22 +30,22 @@
 import hxsoup
 import pyfilename as pf
 from rich.console import Console
 from rich.table import Table
 from tqdm import tqdm
 
 from ..directory_merger import (
+    DIRECTORY_PATTERNS,
     MERGED_WEBTOON_DIRECTORY,
     NORMAL_IMAGE,
     NORMAL_WEBTOON_DIRECTORY,
     ContainerStates,
     check_container_state,
     merge_webtoon,
     restore_webtoon,
-    webtoon_regexes,
 )
 from ..exceptions import (
     DirectoryStateUnmatchedError,
     InvalidURLError,
     InvalidWebtoonIdError,
     NotImplementedCommentsDownloadOptionError,
     UseFetchEpisode,
@@ -603,15 +603,15 @@
         """episode_directory를 생성하고 이미 있다면 해당 폴더 내 내용물이 적합한지 조사합니다.
 
         False를 return한다면 회차를 다운로드해야 한다는 의미입니다.
         True를 return하면 해당 회차가 이미 완전히 다운로드되어 있으며, 따라서 다운로드를 지속할 이유가 없음을 의미합니다.
         """
 
         does_filename_inappropriate = any(
-            not webtoon_regexes[NORMAL_IMAGE].match(file) for file in os.listdir(episode_directory)
+            not DIRECTORY_PATTERNS[NORMAL_IMAGE].match(file) for file in os.listdir(episode_directory)
         )
         does_file_count_inappropriate = len(image_urls) != len(os.listdir(episode_directory))
         return does_filename_inappropriate or does_file_count_inappropriate
 
     async def _download_episode(self, episode_no: int, webtoon_directory: Path, client: hxsoup.AsyncClient) -> bool:
         """한 회차를 다운로드받습니다.
```

### Comparing `webtoonscraper-3.3.0/WebtoonScraper/scrapers/_02_naver_webtoon.py` & `webtoonscraper-3.3.1/WebtoonScraper/scrapers/_02_naver_webtoon.py`

 * *Files identical despite different names*

### Comparing `webtoonscraper-3.3.0/WebtoonScraper/scrapers/_03_webtoon_originals.py` & `webtoonscraper-3.3.1/WebtoonScraper/scrapers/_03_webtoon_originals.py`

 * *Files identical despite different names*

### Comparing `webtoonscraper-3.3.0/WebtoonScraper/scrapers/_04_bufftoon.py` & `webtoonscraper-3.3.1/WebtoonScraper/scrapers/_04_bufftoon.py`

 * *Files identical despite different names*

### Comparing `webtoonscraper-3.3.0/WebtoonScraper/scrapers/_05_naver_post.py` & `webtoonscraper-3.3.1/WebtoonScraper/scrapers/_05_naver_post.py`

 * *Files identical despite different names*

### Comparing `webtoonscraper-3.3.0/WebtoonScraper/scrapers/_06_naver_game.py` & `webtoonscraper-3.3.1/WebtoonScraper/scrapers/_06_naver_game.py`

 * *Files identical despite different names*

### Comparing `webtoonscraper-3.3.0/WebtoonScraper/scrapers/_07_lezhin_comics.py` & `webtoonscraper-3.3.1/WebtoonScraper/scrapers/_07_lezhin_comics.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,20 +79,19 @@
         self.do_not_unshuffle: bool = False
         self.delete_shuffled_file: bool = False
         self.get_paid_episode: bool = False
         self.is_fhd_downloaded: bool | None = False
 
     async def async_download_webtoon(self, *args, **kwargs):
         await super().async_download_webtoon(*args, **kwargs)
-        if self._unshuffled_webtoon_directory is None:
-            return
-        shutil.copy(
-            self._unshuffled_webtoon_directory / "information.json",
-            self._webtoon_directory / "information.json",
-        )
+        if self._unshuffled_webtoon_directory:
+            shutil.copy(
+                self._unshuffled_webtoon_directory / "information.json",
+                self._webtoon_directory / "information.json",
+            )
 
     def fetch_all(self, reload: bool = False) -> None:
         super().fetch_all(reload)
         with suppress(InvalidAuthenticationError):
             self.fetch_user_information(reload=reload)
 
     def get_webtoon_directory_name(self) -> str:
```

### Comparing `webtoonscraper-3.3.0/WebtoonScraper/scrapers/_07_lezhin_unshuffler.py` & `webtoonscraper-3.3.1/WebtoonScraper/scrapers/_07_lezhin_unshuffler.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,19 +10,19 @@
 from pathlib import Path
 from types import ModuleType
 from typing import TYPE_CHECKING
 
 from tqdm import tqdm
 
 from ..directory_merger import (
+    DIRECTORY_PATTERNS,
     NORMAL_EPISODE_DIRECTORY,
     NORMAL_WEBTOON_DIRECTORY,
-    _iterdir_seperating_directories_and_files,
+    _directories_and_files_of,
     check_container_state,
-    webtoon_regexes,
 )
 from ..exceptions import DirectoryStateUnmatchedError, MissingOptionalDependencyError
 from ..miscs import logger
 
 if TYPE_CHECKING:
     from PIL import Image
 else:
@@ -63,29 +63,29 @@
     check_directory_state: bool = True,
 ) -> None:
     if episode_int_ids is None:
         episode_int_ids = _search_episode_int_ids(source_webtoon_directory)
 
     target_webtoon_directory.mkdir(exist_ok=True)
 
-    directories, files = _iterdir_seperating_directories_and_files(source_webtoon_directory)
+    directories, files = _directories_and_files_of(source_webtoon_directory)
     for file in files:
         shutil.copy(file, target_webtoon_directory / file.name)
 
     if check_directory_state:
         directory_state = check_container_state(source_webtoon_directory)
         if directory_state != NORMAL_WEBTOON_DIRECTORY:
             raise DirectoryStateUnmatchedError.from_state(directory_state, source_webtoon_directory)
 
     unshuffle_parameters = []
     for episode_directory_name in sorted(os.listdir(source_webtoon_directory)):
         source_episode_directory = source_webtoon_directory / episode_directory_name
         target_episode_directory = target_webtoon_directory / episode_directory_name
 
-        processed_directory_name = webtoon_regexes[NORMAL_EPISODE_DIRECTORY].match(episode_directory_name)
+        processed_directory_name = DIRECTORY_PATTERNS[NORMAL_EPISODE_DIRECTORY].match(episode_directory_name)
         if processed_directory_name is None:
             logger.debug(f"{episode_directory_name} is passed and it assumed to be thumbnail, so just ignored.")
             continue
 
         episode_no = int(processed_directory_name.group("episode_no"))
         episode_id = episode_int_ids[episode_no - 1]
```

### Comparing `webtoonscraper-3.3.0/WebtoonScraper/scrapers/_08_kakaopage.py` & `webtoonscraper-3.3.1/WebtoonScraper/scrapers/_08_kakaopage.py`

 * *Files identical despite different names*

### Comparing `webtoonscraper-3.3.0/WebtoonScraper/scrapers/_09_naver_blog.py` & `webtoonscraper-3.3.1/WebtoonScraper/scrapers/_09_naver_blog.py`

 * *Files identical despite different names*

### Comparing `webtoonscraper-3.3.0/WebtoonScraper/scrapers/_10_tistory.py` & `webtoonscraper-3.3.1/WebtoonScraper/scrapers/_10_tistory.py`

 * *Files identical despite different names*

### Comparing `webtoonscraper-3.3.0/WebtoonScraper/scrapers/_11_kakao_webtoon.py` & `webtoonscraper-3.3.1/WebtoonScraper/scrapers/_11_kakao_webtoon.py`

 * *Files identical despite different names*

### Comparing `webtoonscraper-3.3.0/WebtoonScraper/scrapers/__init__.py` & `webtoonscraper-3.3.1/WebtoonScraper/scrapers/__init__.py`

 * *Files identical despite different names*

### Comparing `webtoonscraper-3.3.0/WebtoonScraper/webtoon.py` & `webtoonscraper-3.3.1/WebtoonScraper/webtoon.py`

 * *Files identical despite different names*

### Comparing `webtoonscraper-3.3.0/WebtoonScraper/webtoon_viewer.py` & `webtoonscraper-3.3.1/WebtoonScraper/webtoon_viewer.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import json
 import os
 from datetime import datetime
 from html import escape
 from pathlib import Path
 from typing import Any, Sequence, TypeVar
 
-from .directory_merger import _iterdir_seperating_directories_and_files
+from .directory_merger import _directories_and_files_of
 from .miscs import __version__ as version
 
 HTML_TEMPLATE = """\
 <!-- With WebtoonScraper {version} at {created_time} -->
 <!DOCTYPE html>
 <html lang="en">
 <head>
@@ -420,15 +420,15 @@
         >>> from pathlib import Path
         >>> from WebtoonScraper.webtoon_viewer import add_html_webtoon_viewer
         >>> add_html_webtoon_viewer(Path("./webtoon/웹툰 이름(1234567)"))
         ```
     """
 
     # 웹툰 정보 불러옴. 이때 선택적 정보가 없는 경우 빈 값으로 설정함.
-    directories, files = _iterdir_seperating_directories_and_files(webtoon_directory)
+    directories, files = _directories_and_files_of(webtoon_directory)
     for file in files:
         if file.name == "information.json":
             with file.open("r", encoding="utf-8") as f:
                 information: dict[str, Any] = json.load(f)
             webtoon_title = information["title"]
             thumbnail_name = information["thumbnail_name"]
             comments_data = information.get("comments_data", {})
```

### Comparing `webtoonscraper-3.3.0/PKG-INFO` & `webtoonscraper-3.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WebtoonScraper
-Version: 3.3.0
+Version: 3.3.1
 Summary: Scraping webtoons with ease.
 License: Apache-2.0
 Keywords: Webtoon,Webtoon Scraper,Naver Webtoon,Webtoon Downloader,Download Webtoon
 Author: ilotoki0804
 Author-email: ilotoki0804@gmail.com
 Requires-Python: >=3.10,<3.13
 Classifier: License :: OSI Approved :: Apache Software License
@@ -110,17 +110,17 @@
 
 ```console
 webtoon download "https://comic.naver.com/webtoon/list?titleId=819217"
 ```
 
 만약 더 많은 WebtoonScraper의 기능(범위 설정 다운로드, 모아서 보기, 다운로드할 디렉토리 설정, 에피소드 리스팅, 파이썬으로 사용 등)을 알고 싶거나 위에서 소개한 방식으로는 잘 작동하지 않는 경우(특히 버프툰, 레진코믹스의 경우 추가적인 설정이 필수적입니다.)에는 [`사용 방법` 문서](https://github.com/ilotoki0804/WebtoonScraper/blob/master/docs/how_to_use.md)를 참고해 주세요.
 
-## 이 라이브러리가 다운로드 가능한 웹툰/에피소드의 종류
+## 다운로드 가능한 웹툰/에피소드의 종류
 
-[이 라이브러리가 다운로드 가능한 웹툰/에피소드의 종류 문서](https://github.com/ilotoki0804/WebtoonScraper/blob/master/docs/download_availability.md)를 참고하세요.
+[다운로드 가능한 웹툰/에피소드의 종류 문서](https://github.com/ilotoki0804/WebtoonScraper/blob/master/docs/download_availability.md)를 참고하세요.
 
 ## Build from source
 
 우선 git과 python을 설치하고 레포지토리를 클론하세요.
 
 ```console
 git clone https://github.com/ilotoki0804/WebtoonScraper.git
```

