# Comparing `tmp/ftmq-0.6.1.tar.gz` & `tmp/ftmq-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ftmq-0.6.1.tar", max compression
+gzip compressed data, was "ftmq-0.6.2.tar", max compression
```

## Comparing `ftmq-0.6.1.tar` & `ftmq-0.6.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1077 2023-04-04 14:31:45.930293 ftmq-0.6.1/LICENSE
--rw-r--r--   0        0        0     4741 2024-01-31 02:14:30.592540 ftmq-0.6.1/README.md
--rw-r--r--   0        0        0       72 2024-03-14 09:14:42.835871 ftmq-0.6.1/ftmq/__init__.py
--rw-r--r--   0        0        0     2011 2024-01-03 16:54:37.194210 ftmq-0.6.1/ftmq/aggregate.py
--rw-r--r--   0        0        0     4790 2024-03-14 08:37:57.172570 ftmq-0.6.1/ftmq/aggregations.py
--rw-r--r--   0        0        0     4046 2023-10-14 09:45:57.810196 ftmq-0.6.1/ftmq/aleph.py
--rw-r--r--   0        0        0     9799 2024-03-14 05:59:16.854543 ftmq-0.6.1/ftmq/cli.py
--rw-r--r--   0        0        0      580 2024-02-23 20:01:04.717383 ftmq-0.6.1/ftmq/dedupe.py
--rw-r--r--   0        0        0     2517 2024-02-24 16:21:44.983220 ftmq-0.6.1/ftmq/enums.py
--rw-r--r--   0        0        0       93 2023-10-14 09:45:57.814196 ftmq-0.6.1/ftmq/exceptions.py
--rw-r--r--   0        0        0     7069 2023-10-14 09:45:57.814196 ftmq-0.6.1/ftmq/filters.py
--rw-r--r--   0        0        0     2807 2024-02-24 16:21:02.863390 ftmq-0.6.1/ftmq/io.py
--rw-r--r--   0        0        0      292 2024-03-13 18:50:42.659003 ftmq-0.6.1/ftmq/model/__init__.py
--rw-r--r--   0        0        0     4090 2024-03-13 19:40:59.788009 ftmq-0.6.1/ftmq/model/coverage.py
--rw-r--r--   0        0        0     4804 2024-02-26 13:12:38.773692 ftmq-0.6.1/ftmq/model/dataset.py
--rw-r--r--   0        0        0      482 2024-02-26 10:46:34.773368 ftmq-0.6.1/ftmq/model/mixins.py
--rw-r--r--   0        0        0     1802 2024-02-23 20:01:34.917196 ftmq-0.6.1/ftmq/model/proxy.py
--rw-r--r--   0        0        0    10276 2024-03-14 08:34:41.217377 ftmq-0.6.1/ftmq/query.py
--rw-r--r--   0        0        0    12223 2024-03-14 07:39:24.177208 ftmq-0.6.1/ftmq/sql.py
--rw-r--r--   0        0        0     2054 2024-03-14 05:58:47.124786 ftmq-0.6.1/ftmq/store/__init__.py
--rw-r--r--   0        0        0     1310 2024-02-24 16:21:45.719217 ftmq-0.6.1/ftmq/store/aleph.py
--rw-r--r--   0        0        0     3362 2024-03-14 08:35:41.593130 ftmq-0.6.1/ftmq/store/base.py
--rw-r--r--   0        0        0      768 2024-02-24 16:21:45.719217 ftmq-0.6.1/ftmq/store/level.py
--rw-r--r--   0        0        0      550 2024-03-13 18:57:03.036638 ftmq-0.6.1/ftmq/store/memory.py
--rw-r--r--   0        0        0      441 2024-02-23 20:01:36.309188 ftmq-0.6.1/ftmq/store/redis.py
--rw-r--r--   0        0        0     4878 2024-03-13 18:57:03.036638 ftmq-0.6.1/ftmq/store/sql.py
--rw-r--r--   0        0        0     1096 2024-01-03 16:54:37.198210 ftmq-0.6.1/ftmq/types.py
--rw-r--r--   0        0        0     5756 2024-03-14 08:37:57.176570 ftmq-0.6.1/ftmq/util.py
--rw-r--r--   0        0        0     1792 2024-03-14 09:14:42.835871 ftmq-0.6.1/pyproject.toml
--rw-r--r--   0        0        0     6241 1970-01-01 00:00:00.000000 ftmq-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-04-04 14:31:45.930293 ftmq-0.6.2/LICENSE
+-rw-r--r--   0        0        0     4741 2024-01-31 02:14:30.592540 ftmq-0.6.2/README.md
+-rw-r--r--   0        0        0       72 2024-05-08 05:01:58.249505 ftmq-0.6.2/ftmq/__init__.py
+-rw-r--r--   0        0        0     2011 2024-01-03 16:54:37.194210 ftmq-0.6.2/ftmq/aggregate.py
+-rw-r--r--   0        0        0     4790 2024-03-14 08:37:57.172570 ftmq-0.6.2/ftmq/aggregations.py
+-rw-r--r--   0        0        0     4059 2024-03-14 17:13:11.419765 ftmq-0.6.2/ftmq/aleph.py
+-rw-r--r--   0        0        0    10790 2024-04-04 12:20:24.054303 ftmq-0.6.2/ftmq/cli.py
+-rw-r--r--   0        0        0      580 2024-02-23 20:01:04.717383 ftmq-0.6.2/ftmq/dedupe.py
+-rw-r--r--   0        0        0     2517 2024-02-24 16:21:44.983220 ftmq-0.6.2/ftmq/enums.py
+-rw-r--r--   0        0        0       93 2023-10-14 09:45:57.814196 ftmq-0.6.2/ftmq/exceptions.py
+-rw-r--r--   0        0        0     7069 2023-10-14 09:45:57.814196 ftmq-0.6.2/ftmq/filters.py
+-rw-r--r--   0        0        0     2807 2024-02-24 16:21:02.863390 ftmq-0.6.2/ftmq/io.py
+-rw-r--r--   0        0        0      292 2024-03-13 18:50:42.659003 ftmq-0.6.2/ftmq/model/__init__.py
+-rw-r--r--   0        0        0     4090 2024-03-13 19:40:59.788009 ftmq-0.6.2/ftmq/model/coverage.py
+-rw-r--r--   0        0        0     4872 2024-05-08 04:44:59.827595 ftmq-0.6.2/ftmq/model/dataset.py
+-rw-r--r--   0        0        0      482 2024-02-26 10:46:34.773368 ftmq-0.6.2/ftmq/model/mixins.py
+-rw-r--r--   0        0        0     1866 2024-04-04 13:32:02.291870 ftmq-0.6.2/ftmq/model/proxy.py
+-rw-r--r--   0        0        0    10276 2024-03-14 08:34:41.217377 ftmq-0.6.2/ftmq/query.py
+-rw-r--r--   0        0        0    12223 2024-03-14 07:39:24.177208 ftmq-0.6.2/ftmq/sql.py
+-rw-r--r--   0        0        0     2054 2024-03-14 05:58:47.124786 ftmq-0.6.2/ftmq/store/__init__.py
+-rw-r--r--   0        0        0     1310 2024-02-24 16:21:45.719217 ftmq-0.6.2/ftmq/store/aleph.py
+-rw-r--r--   0        0        0     3362 2024-03-14 08:35:41.593130 ftmq-0.6.2/ftmq/store/base.py
+-rw-r--r--   0        0        0      768 2024-02-24 16:21:45.719217 ftmq-0.6.2/ftmq/store/level.py
+-rw-r--r--   0        0        0      550 2024-03-13 18:57:03.036638 ftmq-0.6.2/ftmq/store/memory.py
+-rw-r--r--   0        0        0      441 2024-02-23 20:01:36.309188 ftmq-0.6.2/ftmq/store/redis.py
+-rw-r--r--   0        0        0     4878 2024-03-13 18:57:03.036638 ftmq-0.6.2/ftmq/store/sql.py
+-rw-r--r--   0        0        0     1118 2024-04-04 12:11:45.481029 ftmq-0.6.2/ftmq/types.py
+-rw-r--r--   0        0        0     5963 2024-04-04 12:14:29.656166 ftmq-0.6.2/ftmq/util.py
+-rw-r--r--   0        0        0     1750 2024-05-08 05:01:58.249505 ftmq-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0     6190 1970-01-01 00:00:00.000000 ftmq-0.6.2/PKG-INFO
```

### Comparing `ftmq-0.6.1/LICENSE` & `ftmq-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ftmq-0.6.1/README.md` & `ftmq-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `ftmq-0.6.1/ftmq/aggregate.py` & `ftmq-0.6.2/ftmq/aggregate.py`

 * *Files identical despite different names*

### Comparing `ftmq-0.6.1/ftmq/aggregations.py` & `ftmq-0.6.2/ftmq/aggregations.py`

 * *Files identical despite different names*

### Comparing `ftmq-0.6.1/ftmq/aleph.py` & `ftmq-0.6.2/ftmq/aleph.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from nomenklatura.store import Store, View, Writer
 
 from ftmq.util import make_proxy
 
 uns = Namespace()
 
 
-def parse_uri(uri: str) -> tuple[str, str, str]:
+def parse_uri(uri: str) -> tuple[str, str | None, str | None]:
     """
     http+aleph://host.org
     http+aleph://dataset@host.org
     https+aleph://dataset:api_key@host.org
     """
     api_key = API_KEY
     dataset = None
@@ -30,15 +30,14 @@
     scheme = parsed.scheme.split("+")[0]
     *datasets, host = parsed.netloc.split("@", 1)
     host = urlunparse([scheme, host, *parsed[2:]])
     if len(datasets) == 1:
         dataset, *api_key = datasets[0].split(":", 1)
         if len(api_key) == 1:
             api_key = api_key[0]
-
     return host, api_key or None, dataset
 
 
 class AlephStore(Store[CE, DS]):
     def __init__(
         self,
         dataset: DS,
```

### Comparing `ftmq-0.6.1/ftmq/cli.py` & `ftmq-0.6.2/ftmq/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 from ftmq.io import apply_datasets, smart_read_proxies, smart_write_proxies
 from ftmq.model.coverage import Collector
 from ftmq.model.dataset import Catalog, Dataset
 from ftmq.query import Query
 from ftmq.store import get_store
 from ftmq.util import parse_unknown_filters
 
+log = logging.getLogger(__name__)
+
 
 @click.group(cls=DefaultGroup, default="q", default_if_no_args=True)
 def cli() -> None:
     logging.basicConfig(level=logging.INFO)
 
 
 @cli.command(
@@ -181,14 +183,44 @@
     "-o", "--output-uri", default="-", show_default=True, help="output file or uri"
 )
 def dataset_iterate(input_uri: str | None = "-", output_uri: str | None = "-"):
     dataset = Dataset._from_uri(input_uri)
     smart_write_proxies(output_uri, dataset.iterate(), serialize=True)
 
 
+@dataset.command("generate")
+@click.option(
+    "-i", "--input-uri", default="-", show_default=True, help="input file or uri"
+)
+@click.option(
+    "-o", "--output-uri", default="-", show_default=True, help="output file or uri"
+)
+@click.option(
+    "--stats",
+    is_flag=True,
+    default=False,
+    show_default=True,
+    help="Calculate stats",
+)
+def make_dataset(
+    input_uri: str | None = "-",
+    output_uri: str | None = "-",
+    stats: bool | None = False,
+):
+    """
+    Convert dataset YAML specification into json and optionally calculate statistics
+    """
+    dataset = Dataset._from_uri(input_uri)
+    if stats:
+        collector = Collector()
+        statistics = collector.collect_many(dataset.iterate())
+        dataset.apply_stats(statistics)
+    smart_write(output_uri, dataset.model_dump_json().encode())
+
+
 @cli.group()
 def catalog():
     pass
 
 
 @catalog.command("iterate")
 @click.option(
@@ -198,14 +230,46 @@
     "-o", "--output-uri", default="-", show_default=True, help="output file or uri"
 )
 def catalog_iterate(input_uri: str | None = "-", output_uri: str | None = "-"):
     catalog = Catalog._from_uri(input_uri)
     smart_write_proxies(output_uri, catalog.iterate(), serialize=True)
 
 
+@catalog.command("generate")
+@click.option(
+    "-i", "--input-uri", default="-", show_default=True, help="input file or uri"
+)
+@click.option(
+    "-o", "--output-uri", default="-", show_default=True, help="output file or uri"
+)
+@click.option(
+    "--stats",
+    is_flag=True,
+    default=False,
+    show_default=True,
+    help="Calculate stats for each dataset",
+)
+def make_catalog(
+    input_uri: str | None = "-",
+    output_uri: str | None = "-",
+    stats: bool | None = False,
+):
+    """
+    Convert catalog YAML specification into json and fetch dataset metadata
+    """
+    catalog = Catalog._from_uri(input_uri)
+    if stats:
+        for dataset in catalog.datasets:
+            log.info(f"Generating stats for `{dataset.name}` ...")
+            collector = Collector()
+            statistics = collector.collect_many(dataset.iterate())
+            dataset.apply_stats(statistics)
+    smart_write(output_uri, catalog.model_dump_json().encode())
+
+
 @cli.group()
 def store():
     pass
 
 
 @store.command("list-datasets")
 @click.option(
@@ -270,44 +334,14 @@
     """
     Iterate all entities from in to out
     """
     store = get_store(input_uri)
     smart_write_proxies(output_uri, store.iterate(), serialize=True)
 
 
-@cli.command("make-dataset")
-@click.option(
-    "-i", "--input-uri", default="-", show_default=True, help="input file or uri"
-)
-@click.option(
-    "-o", "--output-uri", default="-", show_default=True, help="output file or uri"
-)
-@click.option(
-    "--stats",
-    is_flag=True,
-    default=False,
-    show_default=True,
-    help="Calculate stats",
-)
-def make_dataset(
-    input_uri: str | None = "-",
-    output_uri: str | None = "-",
-    stats: bool | None = False,
-):
-    """
-    Convert dataset YAML specification into json and optionally calculate statistics
-    """
-    dataset = Dataset._from_uri(input_uri)
-    if stats:
-        collector = Collector()
-        statistics = collector.collect_many(dataset.iterate())
-        dataset.apply_stats(statistics)
-    smart_write(output_uri, dataset.model_dump_json().encode())
-
-
 @cli.command("aggregate")
 @click.option(
     "-i", "--input-uri", default="-", show_default=True, help="input file or uri"
 )
 @click.option(
     "-o", "--output-uri", default="-", show_default=True, help="output file or uri"
 )
```

### Comparing `ftmq-0.6.1/ftmq/dedupe.py` & `ftmq-0.6.2/ftmq/dedupe.py`

 * *Files identical despite different names*

### Comparing `ftmq-0.6.1/ftmq/enums.py` & `ftmq-0.6.2/ftmq/enums.py`

 * *Files identical despite different names*

### Comparing `ftmq-0.6.1/ftmq/filters.py` & `ftmq-0.6.2/ftmq/filters.py`

 * *Files identical despite different names*

### Comparing `ftmq-0.6.1/ftmq/io.py` & `ftmq-0.6.2/ftmq/io.py`

 * *Files identical despite different names*

### Comparing `ftmq-0.6.1/ftmq/model/coverage.py` & `ftmq-0.6.2/ftmq/model/coverage.py`

 * *Files identical despite different names*

### Comparing `ftmq-0.6.1/ftmq/model/dataset.py` & `ftmq-0.6.2/ftmq/model/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,14 +44,16 @@
 class Maintainer(BaseModel):
     """
     this is our own addition
     """
 
     name: str
     description: str | None = None
+    country: str | None = None
+    country_label: str | None = None
     url: HttpUrl | None = None
     logo_url: HttpUrl | None = None
 
 
 class Dataset(BaseModel):
     # nk props
     name: str
```

### Comparing `ftmq-0.6.1/ftmq/model/proxy.py` & `ftmq-0.6.2/ftmq/model/proxy.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,31 @@
-from typing import Any, Iterable, TypeAlias, Union
+from typing import Any, Iterable, Self, TypeAlias, TypeVar, Union
 
 from followthemoney.types import registry
 from pydantic import BaseModel, ConfigDict, Field, model_validator
 
 from ftmq.types import CE
 from ftmq.util import make_proxy
 
-Properties: TypeAlias = dict[str, list[Union[str, "Entity"]]]
+EntityProp = TypeVar("EntityProp", bound="Entity")
+Properties: TypeAlias = dict[str, list[Union[str, EntityProp]]]
 
 
 class Entity(BaseModel):
     model_config = ConfigDict(populate_by_name=True)
 
     id: str = Field(..., examples=["NK-A7z...."])
-    caption: str = Field(..., examples=["John Doe"])
+    caption: str = Field(..., examples=["Jane Doe"])
     schema_: str = Field(..., examples=["LegalEntity"], alias="schema")
-    properties: Properties = Field(..., examples=[{"name": ["John Doe"]}])
+    properties: Properties = Field(..., examples=[{"name": ["Jane Doe"]}])
     datasets: list[str] = Field([], examples=[["us_ofac_sdn"]])
     referents: list[str] = Field([], examples=[["ofac-1234"]])
 
     @classmethod
-    def from_proxy(cls, entity: CE, adjacents: Iterable[CE] | None = None) -> "Entity":
+    def from_proxy(cls, entity: CE, adjacents: Iterable[CE] | None = None) -> Self:
         properties = dict(entity.properties)
         if adjacents:
             adjacents = {e.id: Entity.from_proxy(e) for e in adjacents}
             for prop in entity.iterprops():
                 if prop.type == registry.entity:
                     properties[prop.name] = [
                         adjacents.get(i, i) for i in entity.get(prop)
```

### Comparing `ftmq-0.6.1/ftmq/query.py` & `ftmq-0.6.2/ftmq/query.py`

 * *Files identical despite different names*

### Comparing `ftmq-0.6.1/ftmq/sql.py` & `ftmq-0.6.2/ftmq/sql.py`

 * *Files identical despite different names*

### Comparing `ftmq-0.6.1/ftmq/store/__init__.py` & `ftmq-0.6.2/ftmq/store/__init__.py`

 * *Files identical despite different names*

### Comparing `ftmq-0.6.1/ftmq/store/aleph.py` & `ftmq-0.6.2/ftmq/store/aleph.py`

 * *Files identical despite different names*

### Comparing `ftmq-0.6.1/ftmq/store/base.py` & `ftmq-0.6.2/ftmq/store/base.py`

 * *Files identical despite different names*

### Comparing `ftmq-0.6.1/ftmq/store/level.py` & `ftmq-0.6.2/ftmq/store/level.py`

 * *Files identical despite different names*

### Comparing `ftmq-0.6.1/ftmq/store/memory.py` & `ftmq-0.6.2/ftmq/store/memory.py`

 * *Files identical despite different names*

### Comparing `ftmq-0.6.1/ftmq/store/sql.py` & `ftmq-0.6.2/ftmq/store/sql.py`

 * *Files identical despite different names*

### Comparing `ftmq-0.6.1/ftmq/types.py` & `ftmq-0.6.2/ftmq/types.py`

 * *Files 11% similar despite different names*

```diff
@@ -26,19 +26,19 @@
 Properties: TypeAlias = Literal[tuple(p.name for p in enums.Properties)]
 Frequencies: TypeAlias = Literal[tuple(f.name for f in enums.Frequencies)]
 
 PathLike: TypeAlias = str | os.PathLike[str] | Path
 DateLike: TypeAlias = date | datetime
 
 __all__ = [
-    BytesGenerator,
-    CE,
-    CEGenerator,
-    Frequencies,
-    PathLike,
-    Properties,
-    Schemata,
-    SDict,
-    SGenerator,
-    StrGenerator,
-    Value,
+    "BytesGenerator",
+    "CE",
+    "CEGenerator",
+    "Frequencies",
+    "PathLike",
+    "Properties",
+    "Schemata",
+    "SDict",
+    "SGenerator",
+    "StrGenerator",
+    "Value",
 ]
```

### Comparing `ftmq-0.6.1/ftmq/util.py` & `ftmq-0.6.2/ftmq/util.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from banal import ensure_list
 from followthemoney.schema import Schema
 from followthemoney.types import registry
 from followthemoney.util import make_entity_id, sanitize_text
 from nomenklatura.dataset import Dataset
 from nomenklatura.entity import CE, CompositeEntity
 from nomenklatura.statement import Statement
-from normality import slugify
+from normality import collapse_spaces, slugify
 
 from ftmq.enums import Comparators
 from ftmq.exceptions import ValidationError
 from ftmq.types import SGenerator
 
 
 @cache
@@ -137,15 +137,21 @@
         return None
     texts = [p for p in sections if p is not None]
     if not len(texts):
         return None
     prefix = slugify(prefix, sep=sep)
     if prefix is not None:
         texts = [prefix, *texts]
-    return sep.join(texts)[:max_len].strip(sep)
+    slug = sep.join(texts)
+    if len(slug) <= max_len:
+        return slug
+    # shorten slug but ensure unique
+    ident = make_entity_id(slug)[:8]
+    slug = slug[: max_len - 9].strip(sep)
+    return f"{slug}-{ident}"
 
 
 def get_year(value: Any) -> int | None:
     if not value:
         return
     try:
         return int(str(value)[:4])
@@ -157,15 +163,15 @@
 def clean_string(value: Any) -> str | None:
     """
     Convert a value to None or a sanitized string without linebreaks
     """
     value = sanitize_text(value)
     if value is None:
         return
-    return " ".join(value.split())
+    return collapse_spaces(value)
 
 
 @lru_cache(1024)
 def clean_name(value: Any) -> str | None:
     """
     Clean a value and only return it if it is a "name" in the sense of, doesn't
     contain exclusively of special chars
@@ -186,21 +192,21 @@
     value = clean_name(value)
     if value is None:
         return
     return " ".join(sorted(set(slugify(value).split("-"))))
 
 
 @lru_cache(1024)
-def make_string_id(value: Any) -> str | None:
-    return make_entity_id(clean_name(value))
+def make_string_id(*values: Any) -> str | None:
+    return make_entity_id(*map(clean_name, values))
 
 
 @lru_cache(1024)
-def make_fingerprint_id(value: Any) -> str | None:
-    return make_entity_id(make_fingerprint(value))
+def make_fingerprint_id(*values: Any) -> str | None:
+    return make_entity_id(*map(make_fingerprint, values))
 
 
 @cache
 def prop_is_numeric(schema: Schema, prop: str) -> bool:
     prop = schema.get(prop)
     if prop is not None:
         return prop.type == registry.number
```

### Comparing `ftmq-0.6.1/pyproject.toml` & `ftmq-0.6.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 [tool.poetry]
 name = "ftmq"
-version = "0.6.1"
+version = "0.6.2"
 description = "followthemoney query dsl and io helpers"
 authors = ["Simon Wörpel <simon.woerpel@pm.me>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/investigativedata/ftmq"
 repository = "https://github.com/investigativedata/ftmq"
 documentation = "https://github.com/investigativedata/ftmq"
 classifiers = [
     "Intended Audience :: Developers",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
-    "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 packages = [{include = "ftmq"}]
 
 [tool.poetry.scripts]
 ftmq = "ftmq.cli:cli"
 
@@ -35,21 +34,21 @@
 cryptography = "^42.0.4"
 certifi = ">=2024.2.2"
 scipy = "^1.12.0"
 pydantic = "^2.6.2"
 sqlalchemy = "^2.0.27"
 alephclient = "^2.3.6"
 pycountry = "^23.12.11"
-urllib3 = "<2"
+urllib3 = "<3"
 nomenklatura = "^3.10.4"
-anystore = "^0.1.1"
+anystore = "^0.1.3"
 
 [tool.poetry.group.dev.dependencies]
 pytest = ">=7.4.3,<9.0.0"
-pytest-cov = "^4.1.0"
+pytest-cov = ">=4.1,<6.0"
 black = ">=23.11,<25.0"
 isort = "^5.12.0"
 mypy = "^1.7.0"
 pre-commit = "^3.5.0"
 flake8 = ">=6.1,<8.0"
 ipdb = "^0.13.13"
 bump2version = "^1.0.1"
```

### Comparing `ftmq-0.6.1/PKG-INFO` & `ftmq-0.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,39 +1,38 @@
 Metadata-Version: 2.1
 Name: ftmq
-Version: 0.6.1
+Version: 0.6.2
 Summary: followthemoney query dsl and io helpers
 Home-page: https://github.com/investigativedata/ftmq
 License: MIT
 Author: Simon Wörpel
 Author-email: simon.woerpel@pm.me
 Requires-Python: >=3.11,<3.12
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: PyICU (>=2.12,<3.0)
 Requires-Dist: alephclient (>=2.3.6,<3.0.0)
-Requires-Dist: anystore (>=0.1.1,<0.2.0)
+Requires-Dist: anystore (>=0.1.3,<0.2.0)
 Requires-Dist: banal (>=1.0.6,<2.0.0)
 Requires-Dist: certifi (>=2024.2.2)
 Requires-Dist: click (>=8.1.7,<9.0.0)
 Requires-Dist: click-default-group (>=1.2.4,<2.0.0)
 Requires-Dist: cryptography (>=42.0.4,<43.0.0)
 Requires-Dist: followthemoney (>=3.5.9,<4.0.0)
 Requires-Dist: nomenklatura (>=3.10.4,<4.0.0)
 Requires-Dist: orjson (>=3.9.15,<4.0.0)
 Requires-Dist: pycountry (>=23.12.11,<24.0.0)
 Requires-Dist: pydantic (>=2.6.2,<3.0.0)
 Requires-Dist: scipy (>=1.12.0,<2.0.0)
 Requires-Dist: sqlalchemy (>=2.0.27,<3.0.0)
-Requires-Dist: urllib3 (<2)
+Requires-Dist: urllib3 (<3)
 Project-URL: Bug Tracker, https://github.com/investigativedata/ftmq/issues
 Project-URL: Documentation, https://github.com/investigativedata/ftmq
 Project-URL: Repository, https://github.com/investigativedata/ftmq
 Description-Content-Type: text/markdown
 
 [![ftmq on pypi](https://img.shields.io/pypi/v/ftmq)](https://pypi.org/project/ftmq/) [![Python test and package](https://github.com/investigativedata/ftmq/actions/workflows/python.yml/badge.svg)](https://github.com/investigativedata/ftmq/actions/workflows/python.yml) [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit)](https://github.com/pre-commit/pre-commit) [![Coverage Status](https://coveralls.io/repos/github/investigativedata/ftmq/badge.svg?branch=main)](https://coveralls.io/github/investigativedata/ftmq?branch=main) [![MIT License](https://img.shields.io/pypi/l/ftmq)](./LICENSE)
```

