# Comparing `tmp/nexus_scraper-0.1.0.tar.gz` & `tmp/nexus_scraper-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nexus_scraper-0.1.0.tar", max compression
+gzip compressed data, was "nexus_scraper-0.1.8.tar", max compression
```

## Comparing `nexus_scraper-0.1.0.tar` & `nexus_scraper-0.1.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1063 2024-05-03 04:37:29.166091 nexus_scraper-0.1.0/LICENSE
--rw-r--r--   0        0        0     1540 2024-05-06 05:59:50.677752 nexus_scraper-0.1.0/Nexus/__init__.py
--rw-r--r--   0        0        0      832 2024-05-06 05:51:40.167842 nexus_scraper-0.1.0/Nexus/exceptions.py
--rw-r--r--   0        0        0     3925 2024-05-06 05:54:07.757815 nexus_scraper-0.1.0/Nexus/models.py
--rw-r--r--   0        0        0     2154 2024-05-06 05:42:36.547944 nexus_scraper-0.1.0/Nexus/scraper.py
--rw-r--r--   0        0        0        0 2024-05-04 17:38:42.456288 nexus_scraper-0.1.0/Nexus/scrapers/__init__.py
--rw-r--r--   0        0        0      376 2024-05-06 05:52:53.947829 nexus_scraper-0.1.0/Nexus/scrapers/annatar.py
--rw-r--r--   0        0        0      398 2024-05-06 03:35:41.609356 nexus_scraper-0.1.0/Nexus/scrapers/jackett.py
--rw-r--r--   0        0        0     4114 2024-05-06 05:52:35.907832 nexus_scraper-0.1.0/Nexus/scrapers/orionoid.py
--rw-r--r--   0        0        0     2814 2024-05-06 06:24:12.717481 nexus_scraper-0.1.0/Nexus/scrapers/prowlarr.py
--rw-r--r--   0        0        0      364 2024-05-06 03:35:56.149353 nexus_scraper-0.1.0/Nexus/scrapers/torbox.py
--rw-r--r--   0        0        0     2527 2024-05-06 06:24:56.187473 nexus_scraper-0.1.0/Nexus/scrapers/torrentio.py
--rw-r--r--   0        0        0       14 2024-05-03 04:37:29.166091 nexus_scraper-0.1.0/README.md
--rw-r--r--   0        0        0      594 2024-05-06 06:30:36.467410 nexus_scraper-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      620 1970-01-01 00:00:00.000000 nexus_scraper-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-05-03 04:37:29.166091 nexus_scraper-0.1.8/LICENSE
+-rw-r--r--   0        0        0     1540 2024-05-06 05:59:50.677752 nexus_scraper-0.1.8/Nexus/__init__.py
+-rw-r--r--   0        0        0      832 2024-05-06 05:51:40.167842 nexus_scraper-0.1.8/Nexus/exceptions.py
+-rw-r--r--   0        0        0     4317 2024-05-07 11:58:16.129014 nexus_scraper-0.1.8/Nexus/models.py
+-rw-r--r--   0        0        0     5019 2024-05-07 11:59:35.878999 nexus_scraper-0.1.8/Nexus/scraper.py
+-rw-r--r--   0        0        0        0 2024-05-04 17:38:42.456288 nexus_scraper-0.1.8/Nexus/scrapers/__init__.py
+-rw-r--r--   0        0        0     2718 2024-05-07 11:56:49.419030 nexus_scraper-0.1.8/Nexus/scrapers/annatar.py
+-rw-r--r--   0        0        0     2731 2024-05-07 11:57:08.859026 nexus_scraper-0.1.8/Nexus/scrapers/jackett.py
+-rw-r--r--   0        0        0     5207 2024-05-07 11:11:04.229539 nexus_scraper-0.1.8/Nexus/scrapers/orionoid.py
+-rw-r--r--   0        0        0     3862 2024-05-07 11:57:22.469024 nexus_scraper-0.1.8/Nexus/scrapers/prowlarr.py
+-rw-r--r--   0        0        0     2185 2024-05-07 11:57:29.909022 nexus_scraper-0.1.8/Nexus/scrapers/torbox.py
+-rw-r--r--   0        0        0     2572 2024-05-07 11:58:35.879011 nexus_scraper-0.1.8/Nexus/scrapers/torrentio.py
+-rw-r--r--   0        0        0       14 2024-05-03 04:37:29.166091 nexus_scraper-0.1.8/README.md
+-rw-r--r--   0        0        0      594 2024-05-07 12:02:20.828968 nexus_scraper-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      620 1970-01-01 00:00:00.000000 nexus_scraper-0.1.8/PKG-INFO
```

### Comparing `nexus_scraper-0.1.0/LICENSE` & `nexus_scraper-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `nexus_scraper-0.1.0/Nexus/__init__.py` & `nexus_scraper-0.1.8/Nexus/__init__.py`

 * *Files identical despite different names*

### Comparing `nexus_scraper-0.1.0/Nexus/exceptions.py` & `nexus_scraper-0.1.8/Nexus/exceptions.py`

 * *Files identical despite different names*

### Comparing `nexus_scraper-0.1.0/Nexus/models.py` & `nexus_scraper-0.1.8/Nexus/models.py`

 * *Files 15% similar despite different names*

```diff
@@ -20,14 +20,17 @@
     """    
     jackett_url: Optional[str] = "http://localhost:9117"
     jackett_apikey: Optional[str] = None
     prowlarr_url: Optional[str] = "http://localhost:9696"
     prowlarr_apikey: Optional[str] = None
     orionoid_client: Optional[str] = None
     orionoid_apikey: Optional[str] = None
+    torrentio_url: Optional[str] = "https://torrentio.strem.fun"
+    torrentio_filters: Optional[str] = "qualityfilter=other,scr,cam"
+    annatar_url: Optional[str] = "http://annatar.elfhosted.com"
 
     model_config = {
         "env_file": ".env",
         "env_file_encoding": "utf-8",
     }
 
     @field_validator("prowlarr_apikey", "jackett_apikey", "orionoid_apikey", mode="before")
@@ -48,17 +51,17 @@
     Guids class for storing scrape results.
 
     Attributes:
     - `imdb_id`: Optional[str] - IMDb identifier
     - `tmdb_id`: Optional[str] - TMDb identifier
     - `tvdb_id`: Optional[str] - TVDb identifier
     """
-    imdb_id: Optional[str]
-    tmdb_id: Optional[int]
-    tvdb_id: Optional[int]
+    imdb_id: Optional[str] = None
+    tmdb_id: Optional[int] = None
+    tvdb_id: Optional[int] = None
 
     @field_validator("imdb_id", mode="before")
     def validate_imdb(cls, v):
         """Validate and format the IMDb ID."""
         if v == 0 or v is None:
             return None
         elif isinstance(v, str) and v.startswith("tt"):
@@ -92,27 +95,31 @@
             return None
         return f"magnet:?xt=urn:btih:{self.infohash}"
 
     @field_validator("infohash", mode="before")
     def validate_infohash(cls, v):
         if not v or not isinstance(v, str) or len(v) != 40:
             raise NexusInvalidInfohash("Valid Infohash is required.")
-        return v
+        return v.upper()
 
     @field_validator("source")
     def validate_source(cls, v):
         sources = ["annatar", "jackett", "orionoid", "prowlarr", "torbox", "torrentio"]
         if v not in sources:
             return "torrentio"
         return v
 
     @field_validator("media_type")
     def validate_media_type(cls, v):
-        v = v.split("/")[0].lower()
+        if not v or not isinstance(v, str):
+            return None
+
+        v = v.split("/")[0].lower() # cleanup torznab categories
         match v:
+            # Need to standardize the media types across the board
             case "tv" | "show" | "series" | "episode" | "ep" | "season":
                 return "show"
             case _:
                 return "movie"
 
     def __eq__(self, other):
         return self.infohash == other.infohash
```

### Comparing `nexus_scraper-0.1.0/Nexus/scrapers/orionoid.py` & `nexus_scraper-0.1.8/Nexus/scrapers/orionoid.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from types import SimpleNamespace
+from concurrent.futures import ThreadPoolExecutor, as_completed
 
 import requests
 
-from Nexus.exceptions import OrionoidException
+from Nexus.exceptions import NexusInvalidInfohash, OrionoidException
 from Nexus.models import Guids, NexusSettings, ScrapeResult
 
 
 class Orionoid:
     """Orionoid class for Orionoid API operations."""
 
     def __init__(self, settings: NexusSettings):
@@ -19,76 +19,102 @@
         self.is_initialized = False
         self.session = requests.Session()
         self.check_api_key_validity()
 
     def check_api_key_validity(self):
         """Validate the API key and initialize parameters based on the account type."""
         url = f"{self.base_url}?keyapp={self.client_id}&keyuser={self.api_key}&mode=user&action=retrieve"
-        response = self.session.get(url)
+        try:
+            response = self.session.get(url, timeout=60)
+        except requests.exceptions.ReadTimeout as e:
+            raise OrionoidException(f"API request timed out: {str(e)}")
         if response.status_code != 200:
             raise OrionoidException(f"API key validation failed with status code {response.status_code}")
 
         data = response.json()
         if data.get('result', {}).get('status') == 'success' and data.get('data', {}).get('status') == 'active':
             self.is_premium = data['data']['subscription']['package']['premium']
             self.max_calls = 1000 if self.is_premium else 100
             self.period = 3600 if self.is_premium else 86400
             self.is_initialized = True
         else:
             raise OrionoidException("Failed to initialize Orionoid due to invalid API key or account status.")
 
-    def scrape(self, imdb_id: str, media_type: str = "movie", season=None, episode=None, limit: int = 50) -> list[ScrapeResult]:
+    def scrape(self, query: str, media_type: str = "movie", season=None, episode=None, timeout=60) -> list[ScrapeResult]:
         """Scrape Orionoid for a given media type and ID."""
         if not self.is_initialized:
             raise OrionoidException("Orionoid API not initialized.")
 
         if media_type not in ["movie", "show"]:
             raise OrionoidException("Invalid media type. Must be 'movie' or 'show'.")
 
-        url = self.construct_url(media_type, imdb_id, season, episode, limit)
-        response = self.session.get(url, timeout=10)
+        url = self.construct_url(query, media_type, season, episode)
+        try:
+            response = self.session.get(url, timeout=timeout)
+        except requests.exceptions.ReadTimeout as e:
+            raise OrionoidException(f"API request timed out: {str(e)}")
+
         if response.status_code != 200:
             raise OrionoidException(f"API request failed with status code {response.status_code}")
 
         if 'application/json' not in response.headers.get('Content-Type', ''):
             raise OrionoidException("Expected JSON response but received a different format.")
 
-        data = response.json()["data"]["streams"]
-        streams = [SimpleNamespace(**stream) for stream in data]
-        return self.parse_response(streams, imdb_id, media_type)
+        data = response.json()
+        streams = data["data"]["streams"]
+        return self.parse_response(streams, query, media_type)
 
-    def construct_url(self, media_type, imdb_id, season=None, episode=None, limit = 50) -> str:
+    def construct_url(self, query, media_type, season=None, episode=None) -> str:
         """Construct the URL for the Orionoid API based on media type and identifiers."""
         params = {
             "keyapp": self.client_id,
             "keyuser": self.api_key,
             "mode": "stream",
             "action": "retrieve",
             "type": media_type,
-            "idimdb": imdb_id,
             "streamtype": "torrent",
             "filename": "true",
-            "limitcount": limit,
+            "limitcount": 200 if self.is_premium else 5,
             "sortorder": "descending",
             "sortvalue": "best" if self.is_premium else "popularity",
         }
-        if media_type == "show":
+        if season and episode:
             params.update({"numberseason": season, "numberepisode": episode})
+        elif season:
+            params.update({"numberseason": season})
+        if query.startswith("tt"):
+            params.update({"idimdb": query})
+        else:
+            params.update({"query": query})
         return f"{self.base_url}?{'&'.join([f'{key}={value}' for key, value in params.items()])}"
 
     def parse_response(self, streams, imdb_id, media_type) -> list[ScrapeResult]:
-        """Parse the response from Orionoid and create ScrapeResult objects."""
+        """Parse the response from Orionoid and create ScrapeResult objects using concurrency."""
         if not streams:
             return []
-        return [
-            ScrapeResult(
-                raw_title=stream.file["name"],
-                infohash=stream.file["hash"],
-                guids=Guids(
-                    imdb_id=imdb_id,
-                    tmdb_id=None,
-                    tvdb_id=None
-                ),
+
+        results = []
+        with ThreadPoolExecutor() as executor:
+            futures = {executor.submit(self.create_scrape_result, stream, imdb_id, media_type): stream for stream in streams}
+            for future in as_completed(futures):
+                result = future.result()
+                if result:
+                    results.append(result)
+        return results
+
+    def create_scrape_result(self, stream, imdb_id, media_type):
+        """Helper function to create a ScrapeResult object."""
+        try:
+            guids = Guids(
+                imdb_id=imdb_id if imdb_id.startswith("tt") else None,
+                tmdb_id=None,
+                tvdb_id=None
+            )
+            return ScrapeResult(
+                raw_title=stream["file"]["name"],
+                infohash=stream["file"]["hash"],
+                guids=guids,
                 media_type=media_type,
                 source="orionoid"
-            ) for stream in streams
-        ]
+            )
+        except NexusInvalidInfohash:
+            return None
```

### Comparing `nexus_scraper-0.1.0/Nexus/scrapers/prowlarr.py` & `nexus_scraper-0.1.8/Nexus/scrapers/jackett.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,75 +1,69 @@
-from types import SimpleNamespace
+import concurrent.futures
+from typing import List
 
 import requests
 
-from Nexus.exceptions import ProwlarrException
+from Nexus.exceptions import JackettException, NexusInvalidInfohash
 from Nexus.models import Guids, NexusSettings, ScrapeResult
 
 
-class Prowlarr:
-    """Prowlarr class for Prowlarr API operations."""
-
+class Jackett:
     def __init__(self, settings: NexusSettings):
-        if not settings.prowlarr_url or not settings.prowlarr_apikey != 32:
-            raise ProwlarrException("Prowlarr: URL and API key are required.")
-
-        self.api_key = settings.prowlarr_apikey
-        self.base_url = settings.prowlarr_url
+        self.settings = settings
+        if not self.settings.jackett_url or not self.settings.jackett_apikey:
+            raise JackettException("URL and API key are required.")
+        self.base_url = self.settings.jackett_url
+        self.api_key = self.settings.jackett_apikey
         self.session = requests.Session()
-        self.session.headers.update({"Authorization": f"Bearer {self.api_key}"})
 
     def _request(self, endpoint, method="GET", params=None, data=None, timeout=60):
-        if endpoint.startswith("/"):
-            url = f"{self.base_url}{endpoint}"
-        else:
-            url = f"{self.base_url}/api/v1/{endpoint}"
+        """Private method to handle API requests."""
+        url = f"{self.base_url}/{endpoint}"
         try:
             response = self.session.request(method, url, params=params, json=data, timeout=timeout)
             response.raise_for_status()
             return response.json()
+        except requests.exceptions.ReadTimeout as e:
+            raise TimeoutError(f"API request timed out: {e}")
         except requests.exceptions.RequestException as e:
-            raise ProwlarrException(f"Prowlarr: API request error: {str(e)}")
+            raise JackettException(f"API request error: {e}")
 
-    def scrape(self, query, media_type = None, limit = 50, timeout = 60) -> list[ScrapeResult]:
-        """Scrape Prowlarr for a given query."""
-        if not isinstance(limit, int):
-            raise ProwlarrException("Prowlarr: Limit must be an integer.")
-
-        if query.startswith("tt"):
+    def scrape(self, query, media_type="movie", timeout=60) -> List[ScrapeResult]:
+        """Method to scrape data based on a query and media type."""
+        if not query:
             return []
 
-        data = self._request("search", params={"categories": [2000, 5000], "query": query, "limit": limit}, timeout=timeout)
-        if not data:
-            return []
+        category_map = {"movie": "2000", "show": "5000"}
+        category = category_map.get(media_type.lower(), "2000,5000")
 
-        container = [SimpleNamespace(**result) for result in data]
+        params = {"apikey": self.api_key, "q": query, "cat": category}
+        data = self._request("api/v2.0/indexers/all/results", params=params, timeout=timeout)
+
+        if not data or "Results" not in data:
+            return []
 
         results = []
-        for result in container:
-            try:
-                guids = Guids(
-                    imdb_id=result.imdbId if result.imdbId != 0 else None,
-                    tmdb_id=result.tmdbId if result.tmdbId != 0 else None,
-                    tvdb_id=result.tvdbId if result.tvdbId != 0 else None,
-                )
-                scrape_result = ScrapeResult(
-                    raw_title=result.title,
-                    infohash=result.infoHash,
-                    guids=guids,
-                    media_type=result.categories[0].get("name", None),
-                    source="prowlarr",
-                    size=result.size,
-                    seeders=result.seeders,
-                    leechers=result.leechers,
-                )
-                results.append(scrape_result)
-            except AttributeError:
-                continue
+        with concurrent.futures.ThreadPoolExecutor() as executor:
+            futures = {executor.submit(self._process_result, result, category): result for result in data["Results"]}
+            for future in concurrent.futures.as_completed(futures):
+                result = future.result()
+                if result:
+                    results.append(result)
 
-        if not results:
-            return []
         return results
 
-    def ping(self):
-        """Ping the Prowlarr API."""
-        return self._request("/ping")
+    def _process_result(self, result, category):
+        """Helper method to process each result independently."""
+        try:
+            return ScrapeResult(
+                raw_title=result["Title"],
+                infohash=result.get("InfoHash"),
+                guids=Guids(),
+                media_type=category,
+                source="jackett",
+                size=result.get("Size", 0),
+                seeders=result.get("Seeders", 0),
+                leechers=result.get("Peers", 0)
+            )
+        except NexusInvalidInfohash:
+            return None
```

### Comparing `nexus_scraper-0.1.0/Nexus/scrapers/torrentio.py` & `nexus_scraper-0.1.8/Nexus/scrapers/torrentio.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,48 +1,47 @@
 import requests
 
 from Nexus.exceptions import TorrentioException
-from Nexus.models import Guids, ScrapeResult
+from Nexus.models import Guids, NexusSettings, ScrapeResult
 
 
 class Torrentio:
     """Torrentio class for Torrent API operations."""
 
-    def __init__(self, url: str = "https://torrentio.strem.fun", filters: str = "qualityfilter=other,scr,cam"):
-        self.base_url = url
-        self.filters = filters
+    def __init__(self, settings: NexusSettings):
+        self.base_url = settings.torrentio_url
+        self.filters = settings.torrentio_filters
         self.session = requests.Session()
 
     def _request(self, endpoint: str):
         url = f"{self.base_url}/{self.filters}/{endpoint}.json"
         try:
             response = self.session.get(url, timeout=10)
             response.raise_for_status()
             return response.json()
+        except requests.exceptions.ReadTimeout as e:
+            raise TorrentioException(f"API request timed out: {e}")
         except requests.exceptions.RequestException as e:
-            raise TorrentioException(f"Torrentio: API request error: {e}")
+            raise TorrentioException(f"API request error: {e}")
 
-    def scrape(self, imdbid: str, media_type: str = "", season: int = 9999, episode: int = 9999, limit: int = 50) -> list[ScrapeResult]:
+    def scrape(self, imdbid: str, media_type: str = "", season: int = 9999, episode: int = 9999) -> list[ScrapeResult]:
         """Scrape Torrentio for a given query."""
         if not imdbid:
-            raise TorrentioException("Torrentio: IMDB ID is required.")
-
+            raise TorrentioException("IMDB ID is required.")
         if not imdbid.startswith("tt"):
-            raise TorrentioException("Torrentio: Invalid IMDB ID.")
-
+            raise TorrentioException("Invalid IMDB ID.")
         if not media_type:
-            raise TorrentioException("Torrentio: Media type is required.")
+            raise TorrentioException("Media type is required.")
+        if media_type not in ["movie", "show"]:
+            raise TorrentioException("Invalid media type. Must be 'movie' or 'show'.")
 
         # lets de-normalize it here
         if media_type.lower() == "show":
             media_type = "series"
 
-        if media_type not in ["movie", "series"]:
-            raise TorrentioException("Invalid media type. Must be 'movie' or 'show'.")
-
         endpoint = f"stream/movie/{imdbid}"
         if media_type.lower() == "series" and season != 9999 and episode != 9999:
             endpoint = f"stream/series/{imdbid}:{season}:{episode}"
 
         res = self._request(endpoint)
         if not res or "streams" not in res:
             return []
```

### Comparing `nexus_scraper-0.1.0/pyproject.toml` & `nexus_scraper-0.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nexus-scraper"
-version = "0.1.0"
+version = "0.1.8"
 description = ""
 authors = ["Spoked <dreu.lavelle@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `nexus_scraper-0.1.0/PKG-INFO` & `nexus_scraper-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nexus-scraper
-Version: 0.1.0
+Version: 0.1.8
 Summary: 
 License: MIT
 Author: Spoked
 Author-email: dreu.lavelle@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

