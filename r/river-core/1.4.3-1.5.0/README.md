# Comparing `tmp/river_core-1.4.3.tar.gz` & `tmp/river_core-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/river_core-1.4.3.tar", last modified: Tue Apr 16 05:21:32 2024, max compression
+gzip compressed data, was "dist/river_core-1.5.0.tar", last modified: Wed May  8 12:37:59 2024, max compression
```

## Comparing `river_core-1.4.3.tar` & `river_core-1.5.0.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 05:21:32.000000 river_core-1.4.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-04-16 05:21:18.000000 river_core-1.4.3/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-04-16 05:21:18.000000 river_core-1.4.3/LICENSE.incore
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-04-16 05:21:18.000000 river_core-1.4.3/LICENSE.tessolve
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-16 05:21:18.000000 river_core-1.4.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-04-16 05:21:32.000000 river_core-1.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-16 05:21:18.000000 river_core-1.4.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 05:21:32.000000 river_core-1.4.3/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-04-16 05:21:18.000000 river_core-1.4.3/examples/sample-config.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 05:21:32.000000 river_core-1.4.3/river_core/
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-16 05:21:18.000000 river_core-1.4.3/river_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3016 2024-04-16 05:21:18.000000 river_core-1.4.3/river_core/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-04-16 05:21:18.000000 river_core-1.4.3/river_core/log.py
--rw-r--r--   0 runner    (1001) docker     (127)     7498 2024-04-16 05:21:18.000000 river_core-1.4.3/river_core/main.py
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-16 05:21:18.000000 river_core-1.4.3/river_core/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)    42358 2024-04-16 05:21:18.000000 river_core-1.4.3/river_core/rivercore.py
--rw-r--r--   0 runner    (1001) docker     (127)     6401 2024-04-16 05:21:18.000000 river_core-1.4.3/river_core/sim_hookspecs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 05:21:32.000000 river_core-1.4.3/river_core/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-04-16 05:21:18.000000 river_core-1.4.3/river_core/templates/coverage_report.html
--rw-r--r--   0 runner    (1001) docker     (127)    14632 2024-04-16 05:21:18.000000 river_core-1.4.3/river_core/templates/report.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 05:21:32.000000 river_core-1.4.3/river_core/templates/setup/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 05:21:32.000000 river_core-1.4.3/river_core/templates/setup/dut/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 05:21:18.000000 river_core-1.4.3/river_core/templates/setup/dut/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 05:21:32.000000 river_core-1.4.3/river_core/templates/setup/dut/boot/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-16 05:21:18.000000 river_core-1.4.3/river_core/templates/setup/dut/boot/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-16 05:21:18.000000 river_core-1.4.3/river_core/templates/setup/dut/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-04-16 05:21:18.000000 river_core-1.4.3/river_core/templates/setup/dut/gen_framework.py
--rw-r--r--   0 runner    (1001) docker     (127)     8461 2024-04-16 05:21:18.000000 river_core-1.4.3/river_core/templates/setup/dut/sample_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 05:21:32.000000 river_core-1.4.3/river_core/templates/setup/generator/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 05:21:18.000000 river_core-1.4.3/river_core/templates/setup/generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-16 05:21:18.000000 river_core-1.4.3/river_core/templates/setup/generator/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-04-16 05:21:18.000000 river_core-1.4.3/river_core/templates/setup/generator/gen_framework.py
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-16 05:21:18.000000 river_core-1.4.3/river_core/templates/setup/generator/sample_gen_config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6026 2024-04-16 05:21:18.000000 river_core-1.4.3/river_core/templates/setup/generator/sample_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 05:21:32.000000 river_core-1.4.3/river_core/templates/setup/reference/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 05:21:18.000000 river_core-1.4.3/river_core/templates/setup/reference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-16 05:21:18.000000 river_core-1.4.3/river_core/templates/setup/reference/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-04-16 05:21:18.000000 river_core-1.4.3/river_core/templates/setup/reference/gen_framework.py
--rw-r--r--   0 runner    (1001) docker     (127)     5699 2024-04-16 05:21:18.000000 river_core-1.4.3/river_core/templates/setup/reference/sample_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4074 2024-04-16 05:21:18.000000 river_core-1.4.3/river_core/templates/style.css
--rw-r--r--   0 runner    (1001) docker     (127)    18760 2024-04-16 05:21:18.000000 river_core-1.4.3/river_core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 05:21:32.000000 river_core-1.4.3/river_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-04-16 05:21:32.000000 river_core-1.4.3/river_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-16 05:21:32.000000 river_core-1.4.3/river_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 05:21:32.000000 river_core-1.4.3/river_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-16 05:21:32.000000 river_core-1.4.3/river_core.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 05:21:32.000000 river_core-1.4.3/river_core.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-16 05:21:32.000000 river_core-1.4.3/river_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-16 05:21:32.000000 river_core-1.4.3/river_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-16 05:21:32.000000 river_core-1.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-04-16 05:21:18.000000 river_core-1.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:37:59.000000 river_core-1.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-05-08 12:37:47.000000 river_core-1.5.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-05-08 12:37:47.000000 river_core-1.5.0/LICENSE.incore
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-05-08 12:37:47.000000 river_core-1.5.0/LICENSE.tessolve
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-08 12:37:47.000000 river_core-1.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-08 12:37:59.000000 river_core-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-08 12:37:47.000000 river_core-1.5.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:37:59.000000 river_core-1.5.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-05-08 12:37:47.000000 river_core-1.5.0/examples/sample-config.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:37:59.000000 river_core-1.5.0/river_core/
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-08 12:37:47.000000 river_core-1.5.0/river_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3016 2024-05-08 12:37:47.000000 river_core-1.5.0/river_core/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-05-08 12:37:47.000000 river_core-1.5.0/river_core/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7641 2024-05-08 12:37:47.000000 river_core-1.5.0/river_core/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-08 12:37:47.000000 river_core-1.5.0/river_core/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    42989 2024-05-08 12:37:47.000000 river_core-1.5.0/river_core/rivercore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6401 2024-05-08 12:37:47.000000 river_core-1.5.0/river_core/sim_hookspecs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:37:59.000000 river_core-1.5.0/river_core/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-05-08 12:37:47.000000 river_core-1.5.0/river_core/templates/coverage_report.html
+-rw-r--r--   0 runner    (1001) docker     (127)    14632 2024-05-08 12:37:47.000000 river_core-1.5.0/river_core/templates/report.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:37:59.000000 river_core-1.5.0/river_core/templates/setup/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:37:59.000000 river_core-1.5.0/river_core/templates/setup/dut/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 12:37:47.000000 river_core-1.5.0/river_core/templates/setup/dut/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:37:59.000000 river_core-1.5.0/river_core/templates/setup/dut/boot/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-08 12:37:47.000000 river_core-1.5.0/river_core/templates/setup/dut/boot/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-08 12:37:47.000000 river_core-1.5.0/river_core/templates/setup/dut/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-05-08 12:37:47.000000 river_core-1.5.0/river_core/templates/setup/dut/gen_framework.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8461 2024-05-08 12:37:47.000000 river_core-1.5.0/river_core/templates/setup/dut/sample_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:37:59.000000 river_core-1.5.0/river_core/templates/setup/generator/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 12:37:47.000000 river_core-1.5.0/river_core/templates/setup/generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-08 12:37:47.000000 river_core-1.5.0/river_core/templates/setup/generator/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-05-08 12:37:47.000000 river_core-1.5.0/river_core/templates/setup/generator/gen_framework.py
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-08 12:37:47.000000 river_core-1.5.0/river_core/templates/setup/generator/sample_gen_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6026 2024-05-08 12:37:47.000000 river_core-1.5.0/river_core/templates/setup/generator/sample_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:37:59.000000 river_core-1.5.0/river_core/templates/setup/reference/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 12:37:47.000000 river_core-1.5.0/river_core/templates/setup/reference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-08 12:37:47.000000 river_core-1.5.0/river_core/templates/setup/reference/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-05-08 12:37:47.000000 river_core-1.5.0/river_core/templates/setup/reference/gen_framework.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5699 2024-05-08 12:37:47.000000 river_core-1.5.0/river_core/templates/setup/reference/sample_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4074 2024-05-08 12:37:47.000000 river_core-1.5.0/river_core/templates/style.css
+-rw-r--r--   0 runner    (1001) docker     (127)    18760 2024-05-08 12:37:47.000000 river_core-1.5.0/river_core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:37:59.000000 river_core-1.5.0/river_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-08 12:37:58.000000 river_core-1.5.0/river_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-05-08 12:37:59.000000 river_core-1.5.0/river_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 12:37:58.000000 river_core-1.5.0/river_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-08 12:37:58.000000 river_core-1.5.0/river_core.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 12:37:58.000000 river_core-1.5.0/river_core.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-08 12:37:58.000000 river_core-1.5.0/river_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-08 12:37:58.000000 river_core-1.5.0/river_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-08 12:37:59.000000 river_core-1.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-05-08 12:37:47.000000 river_core-1.5.0/setup.py
```

### Comparing `river_core-1.4.3/CONTRIBUTING.rst` & `river_core-1.5.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `river_core-1.4.3/LICENSE.incore` & `river_core-1.5.0/LICENSE.incore`

 * *Files identical despite different names*

### Comparing `river_core-1.4.3/LICENSE.tessolve` & `river_core-1.5.0/LICENSE.tessolve`

 * *Files identical despite different names*

### Comparing `river_core-1.4.3/PKG-INFO` & `river_core-1.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: river_core
-Version: 1.4.3
+Version: 1.5.0
 Summary: RiVer Core Verification Framework
 Home-page: https://github.com/incoresemi/river_core
 Author: InCore Semiconductors Pvt. Ltd.; Tessolve
 Author-email: neelgala@incoresemi.com
 License: BSD-3-Clause
 Description: **RiVer Core** : RISC-V Core Verification Framework 
         ###################################################################################
```

### Comparing `river_core-1.4.3/examples/sample-config.ini` & `river_core-1.5.0/examples/sample-config.ini`

 * *Files identical despite different names*

### Comparing `river_core-1.4.3/river_core/constants.py` & `river_core-1.5.0/river_core/constants.py`

 * *Files identical despite different names*

### Comparing `river_core-1.4.3/river_core/log.py` & `river_core-1.5.0/river_core/log.py`

 * *Files identical despite different names*

### Comparing `river_core-1.4.3/river_core/main.py` & `river_core-1.5.0/river_core/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -186,23 +186,28 @@
 @click.option(
     '-c',
     '--config',
     type=click.Path(dir_okay=False, exists=True),
     help=
     'Read option defaults from the INI file\nAuto detects river_core.ini in current directory or in the ~ directory'
 )
+@click.option(
+    '--filter_testgen',
+    help=
+    'Override the test generators given by the config file'
+)
 @cli.command()
-def generate(config, verbosity):
+def generate(config, verbosity, filter_testgen):
     """
     subcommand to generate programs.
     """
     logger.info(constants.header_temp.format(__version__))
     if not config:
         config = check_config()
-    rivercore_generate(config, verbosity)
+    rivercore_generate(config, verbosity, filter_testgen)
 
 
 @click.version_option(version=__version__)
 @click.option(
     '-c',
     '--config',
     type=click.Path(dir_okay=False, exists=True),
```

### Comparing `river_core-1.4.3/river_core/rivercore.py` & `river_core-1.5.0/river_core/rivercore.py`

 * *Files 1% similar despite different names*

```diff
@@ -270,15 +270,15 @@
         logger.info('Hope you took a backup of the reports')
         res = confirm()
         if res:
             shutil.rmtree(output_dir)
             logger.info(output_dir + ' directory deleted')
 
 
-def rivercore_generate(config_file, verbosity):
+def rivercore_generate(config_file, verbosity, filter_testgen):
     '''
         Function to generate the assembly programs using the plugin as configured in the config.ini.
 
         :param config_file: Config.ini file for generation
 
         :param verbosity: Verbosity level for the framework
 
@@ -308,16 +308,30 @@
     logger.info(
         "The river_core is currently configured to run with following parameters"
     )
     logger.info("The Output Directory (work_dir) : {0}".format(output_dir))
     logger.info("ISA : {0}".format(config['river_core']['isa']))
     test_list = {}
 
+    if filter_testgen:
+        filter_testgen = filter_testgen.rstrip().split(',')
+        # check if chosen test generators does not exist in the config[generator]
+        suite_list_set = set(suite_list)
+        filter_testgen_set = set(filter_testgen)
+        if not filter_testgen_set.issubset(suite_list_set):
+            logger.err("Test generator(s) passed does not exist in the config file")
+        suite_list = list(suite_list_set.intersection(filter_testgen_set))
+
     for suite in suite_list:
 
+        # for suite not in filter_testgen
+        if filter_testgen:
+            if suite not in filter_testgen:
+                continue
+
         # Give Plugin Info
         logger.info("Plugin Jobs : {0}".format(config[suite]['jobs']))
         logger.info("Plugin Seed : {0}".format(config[suite]['seed']))
         logger.info("Plugin Count (Times to run the test) : {0}".format(
             config[suite]['count']))
         generatorpm = pluggy.PluginManager("generator")
         generatorpm.add_hookspecs(RandomGeneratorSpec)
```

### Comparing `river_core-1.4.3/river_core/sim_hookspecs.py` & `river_core-1.5.0/river_core/sim_hookspecs.py`

 * *Files identical despite different names*

### Comparing `river_core-1.4.3/river_core/templates/coverage_report.html` & `river_core-1.5.0/river_core/templates/coverage_report.html`

 * *Files identical despite different names*

### Comparing `river_core-1.4.3/river_core/templates/report.html` & `river_core-1.5.0/river_core/templates/report.html`

 * *Files identical despite different names*

### Comparing `river_core-1.4.3/river_core/templates/setup/dut/gen_framework.py` & `river_core-1.5.0/river_core/templates/setup/dut/gen_framework.py`

 * *Files identical despite different names*

### Comparing `river_core-1.4.3/river_core/templates/setup/dut/sample_plugin.py` & `river_core-1.5.0/river_core/templates/setup/dut/sample_plugin.py`

 * *Files identical despite different names*

### Comparing `river_core-1.4.3/river_core/templates/setup/generator/gen_framework.py` & `river_core-1.5.0/river_core/templates/setup/generator/gen_framework.py`

 * *Files identical despite different names*

### Comparing `river_core-1.4.3/river_core/templates/setup/generator/sample_plugin.py` & `river_core-1.5.0/river_core/templates/setup/generator/sample_plugin.py`

 * *Files identical despite different names*

### Comparing `river_core-1.4.3/river_core/templates/setup/reference/gen_framework.py` & `river_core-1.5.0/river_core/templates/setup/reference/gen_framework.py`

 * *Files identical despite different names*

### Comparing `river_core-1.4.3/river_core/templates/setup/reference/sample_plugin.py` & `river_core-1.5.0/river_core/templates/setup/reference/sample_plugin.py`

 * *Files identical despite different names*

### Comparing `river_core-1.4.3/river_core/templates/style.css` & `river_core-1.5.0/river_core/templates/style.css`

 * *Files identical despite different names*

### Comparing `river_core-1.4.3/river_core/utils.py` & `river_core-1.5.0/river_core/utils.py`

 * *Files identical despite different names*

### Comparing `river_core-1.4.3/river_core.egg-info/PKG-INFO` & `river_core-1.5.0/river_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: river-core
-Version: 1.4.3
+Version: 1.5.0
 Summary: RiVer Core Verification Framework
 Home-page: https://github.com/incoresemi/river_core
 Author: InCore Semiconductors Pvt. Ltd.; Tessolve
 Author-email: neelgala@incoresemi.com
 License: BSD-3-Clause
 Description: **RiVer Core** : RISC-V Core Verification Framework 
         ###################################################################################
```

### Comparing `river_core-1.4.3/river_core.egg-info/SOURCES.txt` & `river_core-1.5.0/river_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `river_core-1.4.3/setup.py` & `river_core-1.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,10 +58,10 @@
         ]
     },
     setup_requires=setup_requirements,
     test_suite='',
     tests_require=test_requirements,
     url=
     'https://github.com/incoresemi/river_core',
-    version='1.4.3',
+    version='1.5.0',
     zip_safe=False,
 )
```

