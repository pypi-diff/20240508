# Comparing `tmp/gruel-3.0.1.tar.gz` & `tmp/gruel-4.0.0.tar.gz`

## Comparing `gruel-3.0.1.tar` & `gruel-4.0.0.tar`

### file list

```diff
@@ -1,11 +1,13 @@
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 gruel-3.0.1/src/gruel/__init__.py
--rw-r--r--   0        0        0    11789 2020-02-02 00:00:00.000000 gruel-3.0.1/src/gruel/brewer.py
--rw-r--r--   0        0        0     7724 2020-02-02 00:00:00.000000 gruel-3.0.1/src/gruel/grueler.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gruel-3.0.1/src/gruel/py.typed
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 gruel-3.0.1/src/gruel/subgruel.py
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 gruel-3.0.1/src/gruel/template.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 gruel-3.0.1/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 gruel-3.0.1/LICENSE.txt
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 gruel-3.0.1/README.md
--rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 gruel-3.0.1/pyproject.toml
--rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 gruel-3.0.1/PKG-INFO
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 gruel-4.0.0/src/gruel/__init__.py
+-rw-r--r--   0        0        0    10956 2020-02-02 00:00:00.000000 gruel-4.0.0/src/gruel/brewer.py
+-rw-r--r--   0        0        0     9280 2020-02-02 00:00:00.000000 gruel-4.0.0/src/gruel/core.py
+-rw-r--r--   0        0        0    17593 2020-02-02 00:00:00.000000 gruel-4.0.0/src/gruel/crawler.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gruel-4.0.0/src/gruel/py.typed
+-rw-r--r--   0        0        0     7839 2020-02-02 00:00:00.000000 gruel-4.0.0/src/gruel/requests.py
+-rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 gruel-4.0.0/src/gruel/subgruel.py
+-rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 gruel-4.0.0/src/gruel/template.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 gruel-4.0.0/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 gruel-4.0.0/LICENSE.txt
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 gruel-4.0.0/README.md
+-rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 gruel-4.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 gruel-4.0.0/PKG-INFO
```

### Comparing `gruel-3.0.1/src/gruel/brewer.py` & `gruel-4.0.0/src/gruel/brewer.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,28 +7,28 @@
 from typing import Any, Sequence, Type
 
 import loggi
 import quickpool
 from pathier import Pathier, Pathish
 from younotyou import Matcher, younotyou
 
-from gruel.grueler import Gruel
+from .core import ChoresMixin, Gruel
 
 
-class GruelFinder:
+class GruelFinder(loggi.LoggerMixin):
     """Find and load classes that subclass `Gruel`."""
 
     def __init__(
         self,
         subgruel_classes: list[str] = ["*"],
         file_exclude_patterns: list[str] = [],
         scan_path: Pathier | None = None,
         file_include_patterns: list[str] = ["*.py"],
         recursive: bool = True,
-        log_dir: Pathish | None = None,
+        log_dir: Pathish = "logs",
     ):
         """#### :params:
 
         `subgruel_classes`: A list of class names for scrapers that should be loaded.
         In order to be loaded, a scraper class must have a name in this list and have `Gruel` somewhere in its inheritance hierarchy.
         Can use wildcard ('*') patterns for matching.
 
@@ -37,28 +37,25 @@
         `scan_path`: The path to scan for scraper classes.
 
         `file_include_patterns`: Files that match these patterns will be scanned.
 
         `recursive`: Whether the scan should be recursive or not.
 
         `log_dir`: The directory this instance's log should be saved to.
-        If `None`, it will be saved to the current working directory.
 
         Will find and load all classes in the "scrapers" directory that inherit from `Gruel`
         and start with "MySubGruel", but don't contain "Scratch" in the name:
         >>> finder = finder(["MySubGruel*"], ["*Scratch*"], "scrapers")
         >>> gruels = finder.find()"""
         self.subgruel_classes = subgruel_classes
         self.file_exclude_patterns = file_exclude_patterns
         self.scan_path = scan_path or Pathier.cwd()
         self.file_include_patterns = file_include_patterns
         self.recursive = recursive
-        self.logger = loggi.getLogger(
-            "gruel_finder", Pathier(log_dir) if log_dir else Pathier.cwd()
-        )
+        self.init_logger("gruel_finder", log_dir)
 
     def get_bases(self, object: Any) -> list[Any]:
         """Returns a recursive list of all the classes `object` inherits from."""
         parents: list[Any] = []
         bases = object.__bases__
         if not bases:
             return parents
@@ -119,15 +116,15 @@
         modules: list[ModuleType] = []
         for file in files:
             if module := self.load_module_from_file(file):
                 modules.append(module)
         return self.strain_for_gruel(modules)
 
 
-class Brewer:
+class Brewer(loggi.LoggerMixin, ChoresMixin):
     """Use to do multithreaded execution of a list of scrapers.
 
     Intended to be used with `Gruel` scrapers, but anything with a `scrape` method can be passed.
 
     To run any `Gruel` scrapers from the current directory:
     >>> Brewer(GruelFinder().find()).brew()
 
@@ -147,27 +144,27 @@
     except `brew()` has some logging."""
 
     def __init__(
         self,
         scrapers: Sequence[Type[Gruel]],
         scraper_args: Sequence[Sequence[Any]] = [],
         scraper_kwargs: Sequence[dict[str, Any]] = [],
-        log_dir: Pathish | None = None,
+        log_dir: Pathish = "logs",
     ):
         """#### :params:
 
         `scrapers`: A list of scraper classes to initialize and execute.
         A scraper should not be instantiated before being passed.
         When `Brewer` runs a scraper it will instantiate the object at execution time and call it's `scrape` method.
 
         `scraper_args`: A list where each element is a list of positional arguments to be passed to the corresponding scraper's `__init__` function.
 
         `scraper_kwargs`: A list of dictionaries where each dictionary is a set of keyword arguments to be passed to the corresponding scraper's `__init__` function.
 
-        `log_dir`: The directory to store `Brewer` logs in. Defaults to the current working directory.
+        `log_dir`: The directory to store `Brewer` logs in. Defaults to "logs".
 
         e.g.
         >>> class MyGruel(Gruel):
         >>>   def __init__(self, value:int):
         >>>     super().__init__()
         >>>     self.value = value
         >>>
@@ -178,41 +175,23 @@
         >>> values = list(range(5))
         >>> brewer = Brewer(
         >>>   [MyGruel]*num_scrapers,
         >>>   [(val,) for val in values]
         >>> results = brewer.brew()
         >>> print(results)
         >>> [0, 1, 2, 3, 4]"""
-        self._init_logger(log_dir)
+        self.init_logger(log_dir=log_dir)
         self.scrapers = scrapers
         num_scrapers = len(self.scrapers)
         # Pad args and kwargs if there aren't any given
         self.scraper_args: Sequence[Any] = scraper_args or [[]] * num_scrapers
         self.scraper_kwargs: Sequence[dict[str, Any]] = (
             scraper_kwargs or [{}] * num_scrapers
         )
 
-    def _init_logger(self, log_dir: Pathish | None = None):
-        # When Brewer is subclassed, use that file's stem instead of `brewer`
-        log_dir = Pathier(log_dir) if log_dir else Pathier.cwd()
-        source_file = inspect.getsourcefile(type(self))
-        if source_file:
-            log_name = Pathier(source_file).stem
-        else:
-            log_name = Pathier(__file__).stem
-        self.logger = loggi.getLogger(log_name, log_dir)
-
-    def prescrape_chores(self):
-        """Override to add any tasks to be done before running the scrapers."""
-        ...
-
-    def postscrape_chores(self):
-        """Override to add any tasks to be done after running the scrapers."""
-        ...
-
     def _prep_scrapers(self) -> list[tuple[Any, Sequence[Any], dict[str, Any]]]:
         return [
             (scraper, args, kwargs)
             for scraper, args, kwargs in zip(
                 self.scrapers, self.scraper_args, self.scraper_kwargs
             )
         ]
@@ -296,15 +275,15 @@
         action="store_true",
         help=""" Whether -p/--path should be scanned recursively or not. """,
     )
     parser.add_argument(
         "-l",
         "--log_dir",
         type=str,
-        default=None,
+        default="logs",
         help=""" The directory to save the brew log to.""",
     )
     args = parser.parse_args()
     args.path = Pathier(args.path)
 
     return args
```

### Comparing `gruel-3.0.1/src/gruel/grueler.py` & `gruel-4.0.0/src/gruel/core.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,197 +1,215 @@
+import abc
 import inspect
-import time
-from typing import Any
 
 import loggi
-import requests
-import whosyouragent
-from bs4 import BeautifulSoup, Tag
 from noiftimer import Timer
 from pathier import Pathier, Pathish
 from printbuddies import track
+from typing_extensions import Any, Sequence, override
 
-ParsableItem = dict[str, Any] | str | Tag
+from .requests import Response, request
 
 
-def request(
-    url: str,
-    method: str = "get",
-    headers: dict[str, str] = {},
-    params: dict[str, Any] | None = None,
-    data: dict[str, Any] | None = None,
-    timeout: int | None = None,
-    retry_on_fail: bool = True,
-    json_: Any | None = None,
-) -> requests.Response:
-    """Send a request to `url` and return the `requests.Response` object.
-
-    By default, the only header sent is a randomized user agent string.
-
-    This can be overridden by supplying a user agent in the `headers` param.
-
-    If `retry_on_fail` is `True`, the request will be repeated after 1 second if the originally request causes an exception to be thrown.
-    Otherwise, the exception will be raised."""
-    request_args = [method, url]
-    headers = whosyouragent.get_header() | headers
-    request_kwargs = {
-        "headers": headers,
-        "timeout": timeout,
-        "params": params,
-        "data": data,
-        "json": json_,
-    }
-    try:
-        response = requests.request(*request_args, **request_kwargs)
-        return response
-    except Exception as e:
-        if retry_on_fail:
-            time.sleep(1)
-            return requests.request(*request_args, **request_kwargs)
-        else:
-            raise e
-
-
-class Gruel:
-    """Scraper base class.
-
-    Classes subclassing `Gruel` need to implement the following methods:
-
-    * `get_parsable_items(self) -> list[Any]`
-    * `parse_item(self, item: Any)->Any`
-    * `store_item(self, item: Any)`
-
-    Calling the `scrape()` method will execute:
-    1. `self.prescrape_chores()` (does nothing unless overridden)
-    2. `self.get_parsable_items()`
-    3. `self.parse_item()` for each item returned by `self.get_parsable_items()`
-    4. `self.store_item()` for each successfully parsed item
-    5. `self.postscrape_chores()` (only closes this instance's log file unless overridden)
-
-    When overriding `self.postscrape_chores`, it's recommended to either
-    call `super().postscrape_chores()` or make sure to call `self.log.close()`.
-    Otherwise running a large number of scrapers can cause file handle limit issues."""
+class ChoresMixin:
+    """Adds `prescrape_chores` and `postscrape_chores` methods to inheriting classes."""
 
-    def __init__(self, name: str | None = None, log_dir: Pathish | None = None):
+    def postscrape_chores(self):
+        """Chores to do after scraping."""
+        ...
+
+    # ? def interscrape_chores(self):
+
+    def prescrape_chores(self):
+        """Chores to do before scraping."""
+        ...
+
+
+class ParserMixin(abc.ABC):
+    """Core parser functionality for scraper classes."""
+
+    def __init__(self):
+        super().__init__()
+        self.flush_items()
+
+    def flush_items(self):
+        """Flush `parsable_items` and `parsed_items`."""
+        self.parsable_items: list[Any] = []
+        self.parsed_items: list[Any] = []
+
+    @abc.abstractmethod
+    def get_parsable_items(self, source: Any) -> list[Any]:
+        """Get atomic chunks to be parsed from `source` and return as a list."""
+
+    @abc.abstractmethod
+    def parse_item(self, item: Any) -> Any:
+        """Parse `item` and return parsed data."""
+
+    def parse_item_wrapper(self, item: Any) -> Any:
         """
-        :params:
-        * `name`: The name of this scraper. If `None`, the name will be the stem of the file this class/subclass was defined in.
-        i.e. A `Gruel` subclass located in a file called `myscraper.py` will have the name `"myscraper"`.
-        * `log_dir`: The directory this scraper's logs should be saved to.
-        If `None`, the logs will be written to a folder called `"gruel_logs"` within the current working directory.
+        Override this to control what happens around `self.parse_item()` for each item (error handling etc.).
+
+        This way related subclasses can have the same auxillary things happen on calls to `parse_item`
+        while having different `parse_item` implementations.
+
+        This method will be called by `parse_items` for each item.
+
+        When overriding, you should call `parse_item`, pass it `item`, and return the result.
+
+        Without overriding, this function simply calls and returns `self.parse_item(item)`.
+
+        basic e.g.:
+        >>> def parse_item_wrapper(self, item:Any)->Any:
+        >>>   try:
+        >>>     return self.parse_item(item)
+        >>>   except Exception as e:
+        >>>     print(e)
         """
-        self._name = name
-        self._init_logger(log_dir)
-        self.timer = Timer()
-        self.success_count = 0
-        self.fail_count = 0
-        self.failed_to_get_parsable_items = False
-        self.unexpected_failure_occured = False
-        self.parsable_items: list[ParsableItem] = []
-        self.parsed_items: list[Any] = []
+        return self.parse_item(item)
 
-    @property
-    def name(self) -> str:
-        """Returns the name given to __init__ or the stem of the file this instance was defined in if one wasn't given."""
-        return self._name or Pathier(inspect.getsourcefile(type(self))).stem  # type: ignore
+    def parse_items(
+        self, parsable_items: Sequence[Any], show_progress: bool
+    ) -> list[Any]:
+        """Parse items and return them."""
+        parsed_items: list[Any] = []
+        for item in track(parsable_items, disable=not show_progress):
+            parsed_item = self.parse_item_wrapper(item)
+            parsed_items.append(parsed_item)
+        return parsed_items
+
+
+class ScraperMetricsMixin:
+    """Mixin for various run time scraper stats."""
+
+    def __init__(self):
+        super().__init__()
+        self.timer: Timer = Timer()
+        self.success_count: int = 0
+        self.fail_count: int = 0
+        self.failed_to_get_parsable_items: bool = False
+        self.unexpected_failure_occured: bool = False
 
     @property
     def had_failures(self) -> bool:
         """`True` if getting parsable items, parsing items, or unexpected failures occured."""
         return (
-            (self.fail_count > 0)
+            self.fail_count > 0
             or self.failed_to_get_parsable_items
             or self.unexpected_failure_occured
         )
 
-    def _init_logger(self, log_dir: Pathish | None):
-        log_dir = Pathier.cwd() / "gruel_logs" if not log_dir else Pathier(log_dir)
-        self.logger = loggi.getLogger(self.name, log_dir)
-
-    @staticmethod
-    def as_soup(response: requests.Response) -> BeautifulSoup:
-        """Returns the text content of `response` as a `BeautifulSoup` object."""
-        return BeautifulSoup(response.text, "html.parser")
-
-    def get_soup(
-        self, url: str, method: str = "get", headers: dict[str, str] = {}
-    ) -> BeautifulSoup:
-        """Request `url` with `headers` and return `BeautifulSoup` object."""
-        return self.as_soup(request(url, method, headers))
-
-    def clean_string(self, text: str) -> str:
-        """Strip `\\n\\r\\t` and whitespace from `text`."""
-        return text.strip(" \n\t\r")
-
-    # |==============================================================================|
-    # Overridables
-    # |==============================================================================|
-    def prescrape_chores(self):
-        """Chores to do before scraping."""
-        ...
 
-    def postscrape_chores(self):
-        """Chores to do after scraping."""
-        loggi.close(self.logger)
+class Gruel(ParserMixin, ScraperMetricsMixin, loggi.LoggerMixin, ChoresMixin):
+    def __init__(self, name: str | None = None, log_dir: Pathish = "logs"):
+        """
+        :params:
+        * `name`: The name of this scraper. If `None`, the name will be the stem of the file this class/subclass was defined in.
+        i.e. A `Gruel` subclass located in a file called `myscraper.py` will have the name `"myscraper"`.
+        * `log_dir`: The directory this scraper's logs should be saved to.
+        """
+        super().__init__()
+        self._name = name
+        self.init_logger(self.name, log_dir)
 
-    def get_parsable_items(self) -> list[Any]:
-        """Get relevant webpages and extract raw data that needs to be parsed.
+    @property
+    def name(self) -> str:
+        """Returns the name given to __init__ or the stem of the file this instance was defined in if one wasn't given."""
+        return self._name or Pathier(inspect.getsourcefile(type(self))).stem  # type: ignore
 
-        e.g. first 10 results for an endpoint that returns json content
-        >>> return self.get_page(some_url).json()[:10]"""
-        raise NotImplementedError
+    @abc.abstractmethod
+    def get_source(self) -> Any:
+        """Should fetch and return the raw data to be scraped.
+
+        Typically would request a webpage and return the response."""
+
+    @override
+    def parse_item_wrapper(self, item: Any) -> Any:
+        """Returns a parsed item or `None` if parsing failed."""
+        try:
+            parsed_item = self.parse_item(item)
+            self.success_count += 1
+            return parsed_item
+        except Exception as e:
+            self.logger.exception("Failure to parse item:")
+            self.logger.error(str(item))
+            self.fail_count += 1
+            return None
 
-    def parse_item(self, item: Any) -> Any:
-        """Parse `item` and return parsed data.
+    def request(self, *args: Any, **kwargs: Any) -> Response:
+        """
+        Note: For convenience, passes this instances logger to the request functions
 
-        e.g.
-        >>> try:
-        >>>     parsed = {}
-        >>>     parsed["thing1"] = item["element"].split()[0]
-        >>>     self.successes += 1
-        >>>     return parsed
-        >>> except Exception:
-        >>>     self.logger.exception("message")
-        >>>     self.failures += 1
-        >>>     return None"""
-        raise NotImplementedError
-
-    def store_item(self, item: Any) -> Any:
-        """Store `item`."""
-        raise NotImplementedError
+        Constructs and sends a :class:`Request <Request>`.
 
-    def parse_items(self, show_progress: bool) -> Any:
-        for item in track(self.parsable_items, disable=not show_progress):
-            parsed_item = self.parse_item(item)
-            if parsed_item:
-                self.store_item(parsed_item)
-            # Append to `self.parsable_items` even if `None`
-            # so `parsable_items` and `parsed_items` are equal length
-            self.parsed_items.append(parsed_item)
+        `url`: URL for the new :class:`Request` object.
+        `method`: method for the new :class:`Request` object: ``GET``, ``OPTIONS``, ``HEAD``, ``POST``, ``PUT``, ``PATCH``, or ``DELETE``.
+
+        * `retry_count`: The number of times to retry a failed request.
+        * `retry_backoff_factor`: For each failed request, the time before retrying will be `retry_backoff_factor * (2 ** retry_number)`
+        * `retry_on_codes`: List of status codes to retry requests on. Default is `[408, 413, 444, 499, 500, 502, 503, 504]`.
+
+        `params`: dict, list of tuples or bytes to send in the query string for the :class:`Request`.
+        `data`: dict, list of tuples, bytes, or file-like object to send in the body of the :class:`Request`.
+        `json`: A JSON serializable Python object to send in the body of the :class:`Request`.
+        `headers`: dict of HTTP Headers to send with the :class:`Request`. The `User-Agent` header will be randomized unless supplied.
+        `cookies`: dict or CookieJar object to send with the :class:`Request`.
+        `files`: dict of ``'name': file-like-objects`` (or ``{'name': file-tuple}``) for multipart encoding upload.
+            ``file-tuple`` can be a 2-tuple ``('filename', fileobj)``, 3-tuple ``('filename', fileobj, 'content_type')``
+            or a 4-tuple ``('filename', fileobj, 'content_type', custom_headers)``, where ``'content-type'`` is a string
+            defining the content type of the given file and ``custom_headers`` a dict-like object containing additional headers
+            to add for the file.
+        `auth`: Auth tuple to enable Basic/Digest/Custom HTTP Auth.
+        `timeout`: float | tuple, How many seconds to wait for the server to send data
+            before giving up, as a float, or a :ref:`(connect timeout, read
+            timeout) <timeouts>` tuple.
+        `allow_redirects`: bool. Enable/disable GET/OPTIONS/POST/PUT/PATCH/DELETE/HEAD redirection. Defaults to ``True``.
+        `proxies`: dict mapping protocol to the URL of the proxy.
+        `verify`: Either a bool, in which case it controls whether we verify
+                the server's TLS certificate, or a string, in which case it must be a path
+                to a CA bundle to use. Defaults to ``True``.
+        `stream`: if ``False``, the response content will be immediately downloaded.
+        `cert`: if String, path to ssl client cert file (.pem). If Tuple, ('cert', 'key') pair.
+        """
+        kwargs["logger"] = self.logger
+        return request(*args, **kwargs)
 
     def scrape(self, parse_items_prog_bar_display: bool = False):
         """Run the scraper:
         1. prescrape chores
         2. get parsable items
-        3. parse and store items
+        3. parse items
+        4. store items
         5. postscrape chores"""
         try:
             self.timer.start()
             self.logger.info("Scrape started.")
             self.prescrape_chores()
             try:
-                self.parsable_items = self.get_parsable_items()
-                self.logger.info(
-                    f"{self.name}:get_parsable_items() returned {(len(self.parsable_items))} items"
-                )
-            except Exception:
-                self.failed_to_get_parsable_items = True
-                self.logger.exception(f"Error in {self.name}:get_parsable_items().")
+                source = self.get_source()
+            except Exception as e:
+                self.logger.exception(f"Error getting source data.")
             else:
-                self.parse_items(parse_items_prog_bar_display)
-                self.logger.info(
-                    f"Scrape completed in {self.timer.elapsed_str} with {self.success_count} successes and {self.fail_count} failures."
-                )
+                try:
+                    self.parsable_items = self.get_parsable_items(source)
+                    self.logger.info(
+                        f"{self.name}:get_parsable_items() returned {len(self.parsable_items)} items."
+                    )
+                except Exception:
+                    self.failed_to_get_parsable_items = True
+                    self.logger.exception(f"Error in {self.name}:get_parsable_items().")
+                else:
+                    self.parsed_items = self.parse_items(
+                        self.parsable_items, parse_items_prog_bar_display
+                    )
+                    self.logger.info(
+                        f"Scrape completed in {self.timer.elapsed_str} with {self.success_count} successes and {self.fail_count} failures."
+                    )
+            self.store_items(self.parsed_items)
         except Exception:
             self.unexpected_failure_occured = True
             self.logger.exception(f"Unexpected failure in {self.name}:scrape()")
         self.postscrape_chores()
+        self.logger.close()
+
+    @abc.abstractmethod
+    def store_items(self, items: Sequence[Any]) -> None:
+        """Store parsed items."""
```

### Comparing `gruel-3.0.1/src/gruel/subgruel.py` & `gruel-4.0.0/src/gruel/subgruel.py`

 * *Files identical despite different names*

### Comparing `gruel-3.0.1/LICENSE.txt` & `gruel-4.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gruel-3.0.1/pyproject.toml` & `gruel-4.0.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [project]
 name = "gruel"
 description = "Another scraping framework"
-version = "3.0.1"
-dependencies = ["pathier", "printbuddies", "younotyou", "noiftimer", "requests", "whosyouragent", "quickpool", "loggi", "beautifulsoup4"]
+version = "4.0.0"
+dependencies = ["pathier", "printbuddies", "younotyou", "noiftimer", "requests", "whosyouragent", "quickpool", "loggi", "beautifulsoup4", "rich", "scrapetools", "typing_extensions", "urllib3"]
 readme = "README.md"
 keywords = ["scrape", "scraping", "webscraping", "webscraper", "beautifulsoup", "framework"]
 classifiers = ["Programming Language :: Python :: 3", "License :: OSI Approved :: MIT License", "Operating System :: OS Independent"]
 requires-python = ">=3.10, <=3.12"
 
 [[project.authors]]
 name = "Matt Manes"
@@ -23,12 +23,12 @@
 
 [tool]
 [tool.pytest.ini_options]
 addopts = ["--import-mode=importlib"]
 pythonpath = "src"
 
 [tool.hatch.build.targets.sdist]
-exclude = [".coverage", ".pytest_cache", ".vscode", "tests", "htmlcov", "docs", "*log*", "*.md"]
+exclude = [".coverage", ".pytest_cache", ".vscode", "tests", "htmlcov", "docs", "*log*", "*.md", "*.gaphor"]
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
```

### Comparing `gruel-3.0.1/PKG-INFO` & `gruel-4.0.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: gruel
-Version: 3.0.1
+Version: 4.0.0
 Summary: Another scraping framework
 Project-URL: Homepage, https://github.com/matt-manes/gruel
 Project-URL: Documentation, https://github.com/matt-manes/gruel/tree/main/docs
 Project-URL: Source code, https://github.com/matt-manes/gruel/tree/main/src/gruel
 Author-email: Matt Manes <mattmanes@pm.me>
 License-File: LICENSE.txt
 Keywords: beautifulsoup,framework,scrape,scraping,webscraper,webscraping
@@ -15,23 +15,26 @@
 Requires-Dist: beautifulsoup4
 Requires-Dist: loggi
 Requires-Dist: noiftimer
 Requires-Dist: pathier
 Requires-Dist: printbuddies
 Requires-Dist: quickpool
 Requires-Dist: requests
+Requires-Dist: rich
+Requires-Dist: scrapetools
+Requires-Dist: typing-extensions
+Requires-Dist: urllib3
 Requires-Dist: whosyouragent
 Requires-Dist: younotyou
 Description-Content-Type: text/markdown
 
 # gruel
 
 Another scraping framework
 
 ## Installation
 
 Install with:
 
-<pre>
+```console
 pip install gruel
-</pre>
-
+```
```

