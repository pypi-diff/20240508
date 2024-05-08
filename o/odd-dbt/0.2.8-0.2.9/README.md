# Comparing `tmp/odd_dbt-0.2.8.tar.gz` & `tmp/odd_dbt-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odd_dbt-0.2.8.tar", max compression
+gzip compressed data, was "odd_dbt-0.2.9.tar", max compression
```

## Comparing `odd_dbt-0.2.8.tar` & `odd_dbt-0.2.9.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0    11357 2023-09-22 07:35:52.675668 odd_dbt-0.2.8/LICENSE
--rw-r--r--   0        0        0     3408 2023-09-22 07:35:52.675668 odd_dbt-0.2.8/README.md
--rw-r--r--   0        0        0      257 2023-09-22 07:35:52.675668 odd_dbt-0.2.8/odd_dbt/__init__.py
--rw-r--r--   0        0        0       18 2023-09-22 07:36:11.051766 odd_dbt-0.2.8/odd_dbt/__version__.py
--rw-r--r--   0        0        0     5126 2023-09-22 07:35:52.675668 odd_dbt-0.2.8/odd_dbt/app.py
--rw-r--r--   0        0        0      323 2023-09-22 07:35:52.675668 odd_dbt-0.2.8/odd_dbt/config.py
--rw-r--r--   0        0        0      160 2023-09-22 07:35:52.675668 odd_dbt-0.2.8/odd_dbt/domain/__init__.py
--rw-r--r--   0        0        0      835 2023-09-22 07:35:52.675668 odd_dbt-0.2.8/odd_dbt/domain/cli_args.py
--rw-r--r--   0        0        0     1526 2023-09-22 07:35:52.675668 odd_dbt-0.2.8/odd_dbt/domain/context.py
--rw-r--r--   0        0        0      210 2023-09-22 07:35:52.675668 odd_dbt-0.2.8/odd_dbt/domain/credentials.py
--rw-r--r--   0        0        0     1114 2023-09-22 07:35:52.675668 odd_dbt-0.2.8/odd_dbt/domain/manifest.py
--rw-r--r--   0        0        0     1729 2023-09-22 07:35:52.675668 odd_dbt-0.2.8/odd_dbt/domain/model.py
--rw-r--r--   0        0        0      764 2023-09-22 07:35:52.675668 odd_dbt-0.2.8/odd_dbt/domain/project.py
--rw-r--r--   0        0        0      765 2023-09-22 07:35:52.675668 odd_dbt-0.2.8/odd_dbt/domain/result.py
--rw-r--r--   0        0        0      597 2023-09-22 07:35:52.675668 odd_dbt-0.2.8/odd_dbt/domain/run_results.py
--rw-r--r--   0        0        0      310 2023-09-22 07:35:52.675668 odd_dbt-0.2.8/odd_dbt/domain/source.py
--rw-r--r--   0        0        0      291 2023-09-22 07:35:52.675668 odd_dbt-0.2.8/odd_dbt/errors.py
--rw-r--r--   0        0        0        0 2023-09-22 07:35:52.675668 odd_dbt-0.2.8/odd_dbt/libs/__init__.py
--rw-r--r--   0        0        0      872 2023-09-22 07:35:52.675668 odd_dbt-0.2.8/odd_dbt/libs/dbt.py
--rw-r--r--   0        0        0      515 2023-09-22 07:35:52.675668 odd_dbt-0.2.8/odd_dbt/libs/odd.py
--rw-r--r--   0        0        0       54 2023-09-22 07:35:52.675668 odd_dbt-0.2.8/odd_dbt/logger.py
--rw-r--r--   0        0        0        0 2023-09-22 07:35:52.675668 odd_dbt-0.2.8/odd_dbt/mapper/__init__.py
--rw-r--r--   0        0        0     3668 2023-09-22 07:35:52.675668 odd_dbt-0.2.8/odd_dbt/mapper/generator.py
--rw-r--r--   0        0        0      255 2023-09-22 07:35:52.675668 odd_dbt-0.2.8/odd_dbt/mapper/helpers.py
--rw-r--r--   0        0        0     4468 2023-09-22 07:35:52.675668 odd_dbt-0.2.8/odd_dbt/mapper/lineage.py
--rw-r--r--   0        0        0     1792 2023-09-22 07:35:52.675668 odd_dbt-0.2.8/odd_dbt/mapper/metadata.py
--rw-r--r--   0        0        0     6280 2023-09-22 07:35:52.675668 odd_dbt-0.2.8/odd_dbt/mapper/status_reason.py
--rw-r--r--   0        0        0     6204 2023-09-22 07:35:52.675668 odd_dbt-0.2.8/odd_dbt/mapper/test_results.py
--rw-r--r--   0        0        0      935 2023-09-22 07:35:52.675668 odd_dbt-0.2.8/odd_dbt/mapper/types.py
--rw-r--r--   0        0        0        0 2023-09-22 07:35:52.675668 odd_dbt-0.2.8/odd_dbt/service/__init__.py
--rw-r--r--   0        0        0      857 2023-09-22 07:35:52.675668 odd_dbt-0.2.8/odd_dbt/service/dbt.py
--rw-r--r--   0        0        0      974 2023-09-22 07:35:52.675668 odd_dbt-0.2.8/odd_dbt/service/odd.py
--rw-r--r--   0        0        0      283 2023-09-22 07:35:52.675668 odd_dbt-0.2.8/odd_dbt/utils/__init__.py
--rw-r--r--   0        0        0      970 2023-09-22 07:36:10.659764 odd_dbt-0.2.8/pyproject.toml
--rw-r--r--   0        0        0     4563 1970-01-01 00:00:00.000000 odd_dbt-0.2.8/setup.py
--rw-r--r--   0        0        0     4380 1970-01-01 00:00:00.000000 odd_dbt-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-09-22 07:54:00.328881 odd_dbt-0.2.9/LICENSE
+-rw-r--r--   0        0        0     3408 2023-09-22 07:54:00.328881 odd_dbt-0.2.9/README.md
+-rw-r--r--   0        0        0      257 2023-09-22 07:54:00.328881 odd_dbt-0.2.9/odd_dbt/__init__.py
+-rw-r--r--   0        0        0       18 2023-09-22 07:54:26.441259 odd_dbt-0.2.9/odd_dbt/__version__.py
+-rw-r--r--   0        0        0     5551 2023-09-22 07:54:00.328881 odd_dbt-0.2.9/odd_dbt/app.py
+-rw-r--r--   0        0        0      323 2023-09-22 07:54:00.328881 odd_dbt-0.2.9/odd_dbt/config.py
+-rw-r--r--   0        0        0      160 2023-09-22 07:54:00.328881 odd_dbt-0.2.9/odd_dbt/domain/__init__.py
+-rw-r--r--   0        0        0      835 2023-09-22 07:54:00.328881 odd_dbt-0.2.9/odd_dbt/domain/cli_args.py
+-rw-r--r--   0        0        0     1526 2023-09-22 07:54:00.328881 odd_dbt-0.2.9/odd_dbt/domain/context.py
+-rw-r--r--   0        0        0      210 2023-09-22 07:54:00.328881 odd_dbt-0.2.9/odd_dbt/domain/credentials.py
+-rw-r--r--   0        0        0     1114 2023-09-22 07:54:00.328881 odd_dbt-0.2.9/odd_dbt/domain/manifest.py
+-rw-r--r--   0        0        0     1729 2023-09-22 07:54:00.328881 odd_dbt-0.2.9/odd_dbt/domain/model.py
+-rw-r--r--   0        0        0      764 2023-09-22 07:54:00.328881 odd_dbt-0.2.9/odd_dbt/domain/project.py
+-rw-r--r--   0        0        0      765 2023-09-22 07:54:00.328881 odd_dbt-0.2.9/odd_dbt/domain/result.py
+-rw-r--r--   0        0        0      597 2023-09-22 07:54:00.328881 odd_dbt-0.2.9/odd_dbt/domain/run_results.py
+-rw-r--r--   0        0        0      310 2023-09-22 07:54:00.328881 odd_dbt-0.2.9/odd_dbt/domain/source.py
+-rw-r--r--   0        0        0      291 2023-09-22 07:54:00.328881 odd_dbt-0.2.9/odd_dbt/errors.py
+-rw-r--r--   0        0        0        0 2023-09-22 07:54:00.328881 odd_dbt-0.2.9/odd_dbt/libs/__init__.py
+-rw-r--r--   0        0        0      872 2023-09-22 07:54:00.328881 odd_dbt-0.2.9/odd_dbt/libs/dbt.py
+-rw-r--r--   0        0        0      515 2023-09-22 07:54:00.328881 odd_dbt-0.2.9/odd_dbt/libs/odd.py
+-rw-r--r--   0        0        0       54 2023-09-22 07:54:00.328881 odd_dbt-0.2.9/odd_dbt/logger.py
+-rw-r--r--   0        0        0        0 2023-09-22 07:54:00.328881 odd_dbt-0.2.9/odd_dbt/mapper/__init__.py
+-rw-r--r--   0        0        0     3668 2023-09-22 07:54:00.328881 odd_dbt-0.2.9/odd_dbt/mapper/generator.py
+-rw-r--r--   0        0        0      255 2023-09-22 07:54:00.328881 odd_dbt-0.2.9/odd_dbt/mapper/helpers.py
+-rw-r--r--   0        0        0     4468 2023-09-22 07:54:00.328881 odd_dbt-0.2.9/odd_dbt/mapper/lineage.py
+-rw-r--r--   0        0        0     1792 2023-09-22 07:54:00.328881 odd_dbt-0.2.9/odd_dbt/mapper/metadata.py
+-rw-r--r--   0        0        0     6280 2023-09-22 07:54:00.328881 odd_dbt-0.2.9/odd_dbt/mapper/status_reason.py
+-rw-r--r--   0        0        0     6204 2023-09-22 07:54:00.328881 odd_dbt-0.2.9/odd_dbt/mapper/test_results.py
+-rw-r--r--   0        0        0      935 2023-09-22 07:54:00.328881 odd_dbt-0.2.9/odd_dbt/mapper/types.py
+-rw-r--r--   0        0        0        0 2023-09-22 07:54:00.332881 odd_dbt-0.2.9/odd_dbt/service/__init__.py
+-rw-r--r--   0        0        0      857 2023-09-22 07:54:00.332881 odd_dbt-0.2.9/odd_dbt/service/dbt.py
+-rw-r--r--   0        0        0      974 2023-09-22 07:54:00.332881 odd_dbt-0.2.9/odd_dbt/service/odd.py
+-rw-r--r--   0        0        0      283 2023-09-22 07:54:00.332881 odd_dbt-0.2.9/odd_dbt/utils/__init__.py
+-rw-r--r--   0        0        0      970 2023-09-22 07:54:25.941252 odd_dbt-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0     4563 1970-01-01 00:00:00.000000 odd_dbt-0.2.9/setup.py
+-rw-r--r--   0        0        0     4380 1970-01-01 00:00:00.000000 odd_dbt-0.2.9/PKG-INFO
```

### Comparing `odd_dbt-0.2.8/LICENSE` & `odd_dbt-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `odd_dbt-0.2.8/README.md` & `odd_dbt-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `odd_dbt-0.2.8/odd_dbt/app.py` & `odd_dbt-0.2.9/odd_dbt/app.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import contextlib
 import traceback
 from pathlib import Path
 from typing import Optional
 
 import typer
 from dbt.cli.params import default_profiles_dir, default_project_dir
 
@@ -17,14 +18,24 @@
 
 app = typer.Typer(
     short_help="Run dbt tests and inject results to ODD platform",
     pretty_exceptions_show_locals=False,
 )
 
 
+@contextlib.contextmanager
+def handle_errors():
+    try:
+        yield
+    except Exception as e:
+        logger.debug(traceback.format_exc())
+        logger.error(e)
+        raise typer.Exit(1)
+
+
 @app.command()
 def test(
     project_dir: Path = typer.Option(default=default_project_dir()),
     profiles_dir: Path = typer.Option(default=default_profiles_dir()),
     target: Optional[str] = typer.Option(default=None),
     profile: Optional[str] = typer.Option(default=None),
     platform_host: str = typer.Option(..., "--host", "-h", envvar="ODD_PLATFORM_HOST"),
@@ -67,22 +78,23 @@
     data_source_name=typer.Option(..., "--name", "-n"),
     dbt_host: str = typer.Option(default="localhost"),
     platform_host: str = typer.Option(..., "--host", "-h", envvar="ODD_PLATFORM_HOST"),
     platform_token: str = typer.Option(
         ..., "--token", "-t", envvar="ODD_PLATFORM_TOKEN"
     ),
 ):
-    client = config.create_odd_client(host=platform_host, token=platform_token)
-    oddrn = odd_api.create_datasource(data_source_name, dbt_host, client)
+    with handle_errors():
+        client = config.create_odd_client(host=platform_host, token=platform_token)
+        oddrn = odd_api.create_datasource(data_source_name, dbt_host, client)
 
-    logger.info(f"Data source oddrn: '{oddrn}'")
-    logger.info(
-        "You can use command below to add newly created ODDRN for next commands:"
-    )
-    logger.info(f"export DBT_DATA_SOURCE_ODDRN={oddrn}")
+        logger.info(f"Data source oddrn: '{oddrn}'")
+        logger.info(
+            "You can use command below to add newly created ODDRN for next commands:"
+        )
+        logger.info(f"export DBT_DATA_SOURCE_ODDRN={oddrn}")
 
 
 @app.command()
 def ingest_test(
     project_dir: Path = typer.Option(default=default_project_dir()),
     profiles_dir: Path = typer.Option(default=default_profiles_dir()),
     target: Optional[str] = typer.Option(default=None),
@@ -91,28 +103,29 @@
     platform_token: str = typer.Option(
         ..., "--token", "-t", envvar="ODD_PLATFORM_TOKEN"
     ),
     dbt_data_source_oddrn: str = typer.Option(
         ..., "--dbt-oddrn", "-oddrn", envvar="DBT_DATA_SOURCE_ODDRN"
     ),
 ):
-    cli_args = CliArgs(
-        project_dir=project_dir,
-        profiles_dir=profiles_dir,
-        profile=profile,
-        target=target,
-        threads=1,
-        vars={},
-    )
-    context = dbt.get_context(cli_args=cli_args)
-    client = config.create_odd_client(host=platform_host, token=platform_token)
-    generator = odd.create_dbt_generator_from_oddrn(oddrn=dbt_data_source_oddrn)
+    with handle_errors():
+        cli_args = CliArgs(
+            project_dir=project_dir,
+            profiles_dir=profiles_dir,
+            profile=profile,
+            target=target,
+            threads=1,
+            vars={},
+        )
+        context = dbt.get_context(cli_args=cli_args)
+        client = config.create_odd_client(host=platform_host, token=platform_token)
+        generator = odd.create_dbt_generator_from_oddrn(oddrn=dbt_data_source_oddrn)
 
-    data_entities = DbtTestMapper(context=context, generator=generator).map()
-    odd_api.ingest_entities(data_entities, client)
+        data_entities = DbtTestMapper(context=context, generator=generator).map()
+        odd_api.ingest_entities(data_entities, client)
 
 
 @app.command()
 def ingest_lineage(
     project_dir: Path = typer.Option(default=default_project_dir()),
     profiles_dir: Path = typer.Option(default=default_profiles_dir()),
     target: Optional[str] = typer.Option(default=None),
@@ -121,25 +134,26 @@
     platform_token: str = typer.Option(
         ..., "--token", "-t", envvar="ODD_PLATFORM_TOKEN"
     ),
     dbt_data_source_oddrn: str = typer.Option(
         ..., "--dbt-oddrn", "-oddrn", envvar="DBT_DATA_SOURCE_ODDRN"
     ),
 ):
-    cli_args = CliArgs(
-        project_dir=project_dir,
-        profiles_dir=profiles_dir,
-        profile=profile,
-        target=target,
-        threads=1,
-        vars={},
-    )
-    context = dbt.get_context(cli_args=cli_args)
-    client = config.create_odd_client(host=platform_host, token=platform_token)
-    generator = odd.create_dbt_generator_from_oddrn(oddrn=dbt_data_source_oddrn)
+    with handle_errors():
+        cli_args = CliArgs(
+            project_dir=project_dir,
+            profiles_dir=profiles_dir,
+            profile=profile,
+            target=target,
+            threads=1,
+            vars={},
+        )
+        context = dbt.get_context(cli_args=cli_args)
+        client = config.create_odd_client(host=platform_host, token=platform_token)
+        generator = odd.create_dbt_generator_from_oddrn(oddrn=dbt_data_source_oddrn)
 
-    data_entities = DbtLineageMapper(context=context, generator=generator).map()
-    odd_api.ingest_entities(data_entities, client)
+        data_entities = DbtLineageMapper(context=context, generator=generator).map()
+        odd_api.ingest_entities(data_entities, client)
 
 
 if __name__ == "__main__":
     app()
```

### Comparing `odd_dbt-0.2.8/odd_dbt/domain/cli_args.py` & `odd_dbt-0.2.9/odd_dbt/domain/cli_args.py`

 * *Files identical despite different names*

### Comparing `odd_dbt-0.2.8/odd_dbt/domain/context.py` & `odd_dbt-0.2.9/odd_dbt/domain/context.py`

 * *Files identical despite different names*

### Comparing `odd_dbt-0.2.8/odd_dbt/domain/manifest.py` & `odd_dbt-0.2.9/odd_dbt/domain/manifest.py`

 * *Files identical despite different names*

### Comparing `odd_dbt-0.2.8/odd_dbt/domain/model.py` & `odd_dbt-0.2.9/odd_dbt/domain/model.py`

 * *Files identical despite different names*

### Comparing `odd_dbt-0.2.8/odd_dbt/domain/project.py` & `odd_dbt-0.2.9/odd_dbt/domain/project.py`

 * *Files identical despite different names*

### Comparing `odd_dbt-0.2.8/odd_dbt/domain/result.py` & `odd_dbt-0.2.9/odd_dbt/domain/result.py`

 * *Files identical despite different names*

### Comparing `odd_dbt-0.2.8/odd_dbt/domain/run_results.py` & `odd_dbt-0.2.9/odd_dbt/domain/run_results.py`

 * *Files identical despite different names*

### Comparing `odd_dbt-0.2.8/odd_dbt/libs/dbt.py` & `odd_dbt-0.2.9/odd_dbt/libs/dbt.py`

 * *Files identical despite different names*

### Comparing `odd_dbt-0.2.8/odd_dbt/libs/odd.py` & `odd_dbt-0.2.9/odd_dbt/libs/odd.py`

 * *Files identical despite different names*

### Comparing `odd_dbt-0.2.8/odd_dbt/mapper/generator.py` & `odd_dbt-0.2.9/odd_dbt/mapper/generator.py`

 * *Files identical despite different names*

### Comparing `odd_dbt-0.2.8/odd_dbt/mapper/lineage.py` & `odd_dbt-0.2.9/odd_dbt/mapper/lineage.py`

 * *Files identical despite different names*

### Comparing `odd_dbt-0.2.8/odd_dbt/mapper/metadata.py` & `odd_dbt-0.2.9/odd_dbt/mapper/metadata.py`

 * *Files identical despite different names*

### Comparing `odd_dbt-0.2.8/odd_dbt/mapper/status_reason.py` & `odd_dbt-0.2.9/odd_dbt/mapper/status_reason.py`

 * *Files identical despite different names*

### Comparing `odd_dbt-0.2.8/odd_dbt/mapper/test_results.py` & `odd_dbt-0.2.9/odd_dbt/mapper/test_results.py`

 * *Files identical despite different names*

### Comparing `odd_dbt-0.2.8/odd_dbt/mapper/types.py` & `odd_dbt-0.2.9/odd_dbt/mapper/types.py`

 * *Files identical despite different names*

### Comparing `odd_dbt-0.2.8/odd_dbt/service/dbt.py` & `odd_dbt-0.2.9/odd_dbt/service/dbt.py`

 * *Files identical despite different names*

### Comparing `odd_dbt-0.2.8/odd_dbt/service/odd.py` & `odd_dbt-0.2.9/odd_dbt/service/odd.py`

 * *Files identical despite different names*

### Comparing `odd_dbt-0.2.8/pyproject.toml` & `odd_dbt-0.2.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "odd-dbt"
-version = "0.2.8"
+version = "0.2.9"
 description = "OpenDataDiscovery Action for dbt"
 authors = ["Mateusz Kulas <mkulas@provectus.com>"]
 readme = "README.md"
 license = "Apache-2.0"
 keywords = [
     'Open Data Discovery',
     'dbt',
```

### Comparing `odd_dbt-0.2.8/setup.py` & `odd_dbt-0.2.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
  'typer[all]>=0.7.0,<0.8.0']
 
 entry_points = \
 {'console_scripts': ['odd_dbt_test = odd_dbt.app:app']}
 
 setup_kwargs = {
     'name': 'odd-dbt',
-    'version': '0.2.8',
+    'version': '0.2.9',
     'description': 'OpenDataDiscovery Action for dbt',
     'long_description': "# OpenDataDiscovery dbt tests metadata collecting\n\n[![PyPI version](https://badge.fury.io/py/odd-dbt.svg)](https://badge.fury.io/py/odd-dbt)\n\nCLI tool helps run and ingest dbt test to platform.\n\nIt can be used as separated CLI tool or within [ODD CLI](https://github.com/opendatadiscovery/odd-cli) package which\nprovides some useful additional features for working with OpenDataDiscovery.\n\n## Supported adapters\n\n| Adapter   | version |\n|-----------|---------|\n| Snowflake | ^1.6    |\n| Postgres  | ^1.6    |\n\nProfiles inside the file looks different for each type of data source.\n\n**Snowflake** host_settings value is created from field `account`. Field value should be `<account_identifier>`\nFor example the URL for an account uses the following format: `<account_identifier>`.snowflakecomputing.com\nExample Snowflake account identifier `hj1234.eu-central-1`.\n\n## Supported tests types\n\n1. [x]  Generic tests\n2. [ ] Singular tests. Currently Singular tests are not supported.\n\n## Installation\n```pip install odd-dbt```\n\n## To see all available commands\n```\nodd_dbt_test --help\n```\n\n## Example\nFor each command that involves sending information to OpenDataDiscovery platform exists set of env variables:\n1. `ODD_PLATFORM_HOST` - Where you platform is\n2. `ODD_PLATFORM_TOKEN` - Token for ingesting data to platform (How to create [token](https://docs.opendatadiscovery.org/configuration-and-deployment/trylocally#create-collector-entity)?)\n3. `DBT_DATA_SOURCE_ODDRN` - Unique oddrn string describes dbt source, i.e '//dbt/host/localhost'\n\nIt is recommended to add them as ENV variables or provide as flags to each command\n```\nexport ODD_PLATFORM_HOST=http://localhost:8080\nexport ODD_PLATFORM_TOKEN=token***\nexport DBT_DATA_SOURCE_ODDRN=//dbt/host/localhost\n```\n\n### Commands\n`create-datasource` - helps to register dbt as data source at OpenDataDiscovery platform. User later for ingesting metadata.\n```commandline\nodd_dbt_test create-datasource --name=my_local_dbt --dbt-host=localhost\n```\n\n`ingest-test` - Read results_run file under the target folder to parse and ingest metadata.\n```commandline\nodd_dbt_test ingest-test --profile=my_profile\n```\n\n`test` - Proxy command to `dbt test`, then reads results_run file under the target folder to parse and ingest metadata.\n```commandline\nodd_dbt_test test --profile=my_profile\n```\n\n### Run commands programmatically\nYou could run that scrip to read, parse and ingest test results to the platform.\n\n```python\n# ingest_test_result.py\n\nfrom odd_dbt import config\nfrom odd_dbt.domain.cli_args import CliArgs\nfrom odd_dbt.libs.dbt import get_context\nfrom odd_dbt.libs.odd import create_dbt_generator_from_oddrn\nfrom odd_dbt.service.odd import ingest_entities\nfrom odd_dbt.mapper.test_results import DbtTestMapper\nfrom odd_dbt.mapper.lineage import DbtLineageMapper\n\ncfg = config.Config()  # All fields can be set manually or read from ENV variables\nclient = config.create_odd_client(host=cfg.odd_platform_host, token=cfg.odd_platform_token)\ngenerator = create_dbt_generator_from_oddrn(oddrn=cfg.dbt_data_source_oddrn)\n\ncli_args = CliArgs.default()\ncontext = get_context(cli_args=cli_args)\n\n# Ingest lineage\ndata_entities = DbtLineageMapper(context=context, generator=generator).map()\ningest_entities(data_entities, client)\n\n# Or ingest test results\ndata_entities = DbtTestMapper(context=context, generator=generator).map()\ningest_entities(data_entities, client)\n```",
     'author': 'Mateusz Kulas',
     'author_email': 'mkulas@provectus.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `odd_dbt-0.2.8/PKG-INFO` & `odd_dbt-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odd-dbt
-Version: 0.2.8
+Version: 0.2.9
 Summary: OpenDataDiscovery Action for dbt
 License: Apache-2.0
 Keywords: Open Data Discovery,dbt,Metadata,Data Discovery,Data Observability
 Author: Mateusz Kulas
 Author-email: mkulas@provectus.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

