# Comparing `tmp/python-ironicclient-5.5.0.tar.gz` & `tmp/python-ironicclient-5.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-ironicclient-5.5.0.tar", last modified: Thu Feb 29 15:06:42 2024, max compression
+gzip compressed data, was "python-ironicclient-5.6.0.tar", last modified: Wed May  8 05:33:10 2024, max compression
```

## Comparing `python-ironicclient-5.5.0.tar` & `python-ironicclient-5.6.0.tar`

### file list

```diff
@@ -1,367 +1,370 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-29 15:06:42.564656 python-ironicclient-5.5.0/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       73 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/.coveragerc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       71 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/.stestr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7243 2024-02-29 15:06:42.000000 python-ironicclient-5.5.0/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      335 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    41027 2024-02-29 15:06:42.000000 python-ironicclient-5.5.0/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4334 2024-02-29 15:06:42.564656 python-ironicclient-5.5.0/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2592 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      127 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/bindep.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-29 15:06:42.512656 python-ironicclient-5.5.0/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      337 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-29 15:06:42.512656 python-ironicclient-5.5.0/doc/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3380 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/doc/source/api_v1.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-29 15:06:42.512656 python-ironicclient-5.5.0/doc/source/cli/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      164 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/doc/source/cli/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-29 15:06:42.508656 python-ironicclient-5.5.0/doc/source/cli/osc/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-29 15:06:42.516656 python-ironicclient-5.5.0/doc/source/cli/osc/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1408 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/doc/source/cli/osc/v1/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2602 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/doc/source/cli/osc_plugin_cli.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2923 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/doc/source/cli/standalone.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2719 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/doc/source/conf.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-29 15:06:42.516656 python-ironicclient-5.5.0/doc/source/contributor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1519 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/doc/source/contributor/contributing.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      180 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/doc/source/contributor/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1956 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/doc/source/contributor/testing.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      657 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/doc/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-29 15:06:42.516656 python-ironicclient-5.5.0/doc/source/reference/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      164 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/doc/source/reference/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-29 15:06:42.516656 python-ironicclient-5.5.0/doc/source/user/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5817 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/doc/source/user/create_command.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-29 15:06:42.516656 python-ironicclient-5.5.0/ironicclient/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      858 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/ironicclient/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6037 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/ironicclient/client.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-29 15:06:42.516656 python-ironicclient-5.5.0/ironicclient/common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/ironicclient/common/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-29 15:06:42.516656 python-ironicclient-5.5.0/ironicclient/common/apiclient/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/ironicclient/common/apiclient/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16928 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/ironicclient/common/apiclient/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13414 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/ironicclient/common/apiclient/exceptions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13786 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/ironicclient/common/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3324 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/ironicclient/common/filecache.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    19501 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/ironicclient/common/http.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      890 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/ironicclient/common/i18n.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16410 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/ironicclient/common/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2695 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/ironicclient/exc.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-29 15:06:42.516656 python-ironicclient-5.5.0/ironicclient/osc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/ironicclient/osc/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5008 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/ironicclient/osc/plugin.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-29 15:06:42.520656 python-ironicclient-5.5.0/ironicclient/osc/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/ironicclient/osc/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14167 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/ironicclient/osc/v1/baremetal_allocation.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11134 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/ironicclient/osc/v1/baremetal_chassis.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     5486 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/ironicclient/osc/v1/baremetal_conductor.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1398 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/ironicclient/osc/v1/baremetal_create.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12397 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/ironicclient/osc/v1/baremetal_deploy_template.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9423 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/ironicclient/osc/v1/baremetal_driver.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)    85752 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/ironicclient/osc/v1/baremetal_node.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    19378 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/ironicclient/osc/v1/baremetal_port.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17413 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/ironicclient/osc/v1/baremetal_portgroup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13536 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/ironicclient/osc/v1/baremetal_volume_connector.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15268 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/ironicclient/osc/v1/baremetal_volume_target.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8614 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/ironicclient/shell.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-29 15:06:42.520656 python-ironicclient-5.5.0/ironicclient/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/ironicclient/tests/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-29 15:06:42.520656 python-ironicclient-5.5.0/ironicclient/tests/functional/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/ironicclient/tests/functional/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17958 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/ironicclient/tests/functional/base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-29 15:06:42.520656 python-ironicclient-5.5.0/ironicclient/tests/functional/osc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/ironicclient/tests/functional/osc/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-29 15:06:42.524656 python-ironicclient-5.5.0/ironicclient/tests/functional/osc/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/ironicclient/tests/functional/osc/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18361 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/ironicclient/tests/functional/osc/v1/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8146 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/ironicclient/tests/functional/osc/v1/test_baremetal_allocation.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3308 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/ironicclient/tests/functional/osc/v1/test_baremetal_chassis_basic.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1424 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/ironicclient/tests/functional/osc/v1/test_baremetal_conductor_basic.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7239 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/ironicclient/tests/functional/osc/v1/test_baremetal_deploy_template_basic.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1364 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/ironicclient/tests/functional/osc/v1/test_baremetal_driver_basic.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9457 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/ironicclient/tests/functional/osc/v1/test_baremetal_node_basic.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1994 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/ironicclient/tests/functional/osc/v1/test_baremetal_node_create_negative.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4970 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/ironicclient/tests/functional/osc/v1/test_baremetal_node_fields.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3438 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/ironicclient/tests/functional/osc/v1/test_baremetal_node_negative.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2393 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/ironicclient/tests/functional/osc/v1/test_baremetal_node_power_states.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3877 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/ironicclient/tests/functional/osc/v1/test_baremetal_node_provision_states.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4800 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/ironicclient/tests/functional/osc/v1/test_baremetal_port_basic.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2963 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/ironicclient/tests/functional/osc/v1/test_baremetal_port_create.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5116 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/ironicclient/tests/functional/osc/v1/test_baremetal_portgroup_basic.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1115 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/ironicclient/tests/functional/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-29 15:06:42.524656 python-ironicclient-5.5.0/ironicclient/tests/unit/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/ironicclient/tests/unit/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-29 15:06:42.524656 python-ironicclient-5.5.0/ironicclient/tests/unit/common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/ironicclient/tests/unit/common/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-29 15:06:42.524656 python-ironicclient-5.5.0/ironicclient/tests/unit/common/apiclient/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/ironicclient/tests/unit/common/apiclient/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7181 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/ironicclient/tests/unit/common/apiclient/test_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5355 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/ironicclient/tests/unit/common/apiclient/test_exceptions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9677 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/ironicclient/tests/unit/common/test_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8411 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/ironicclient/tests/unit/common/test_filecache.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    24336 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/ironicclient/tests/unit/common/test_http.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17668 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/ironicclient/tests/unit/common/test_utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-29 15:06:42.524656 python-ironicclient-5.5.0/ironicclient/tests/unit/osc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/ironicclient/tests/unit/osc/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1841 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/ironicclient/tests/unit/osc/fakes.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7293 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/ironicclient/tests/unit/osc/test_plugin.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-29 15:06:42.528656 python-ironicclient-5.5.0/ironicclient/tests/unit/osc/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/ironicclient/tests/unit/osc/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11576 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/ironicclient/tests/unit/osc/v1/fakes.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    23761 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/ironicclient/tests/unit/osc/v1/test_baremetal_allocation.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17983 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/ironicclient/tests/unit/osc/v1/test_baremetal_chassis.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9451 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/ironicclient/tests/unit/osc/v1/test_baremetal_conductor.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1739 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/ironicclient/tests/unit/osc/v1/test_baremetal_create.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16550 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/ironicclient/tests/unit/osc/v1/test_baremetal_deploy_template.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20501 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/ironicclient/tests/unit/osc/v1/test_baremetal_driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   150179 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/ironicclient/tests/unit/osc/v1/test_baremetal_node.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    29204 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/ironicclient/tests/unit/osc/v1/test_baremetal_port.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    28663 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/ironicclient/tests/unit/osc/v1/test_baremetal_portgroup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    31976 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/ironicclient/tests/unit/osc/v1/test_baremetal_volume_connector.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    38280 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/ironicclient/tests/unit/osc/v1/test_baremetal_volume_target.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11631 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/ironicclient/tests/unit/test_client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2627 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/ironicclient/tests/unit/test_exc.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1393 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/ironicclient/tests/unit/test_import.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5060 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/ironicclient/tests/unit/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-29 15:06:42.528656 python-ironicclient-5.5.0/ironicclient/tests/unit/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/ironicclient/tests/unit/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11950 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/ironicclient/tests/unit/v1/test_allocation.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14520 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/ironicclient/tests/unit/v1/test_chassis.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6113 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/ironicclient/tests/unit/v1/test_client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6549 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/ironicclient/tests/unit/v1/test_conductor.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    22786 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/ironicclient/tests/unit/v1/test_create_resources.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9684 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/ironicclient/tests/unit/v1/test_deploy_template.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9068 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/ironicclient/tests/unit/v1/test_driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1964 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/ironicclient/tests/unit/v1/test_events.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    78296 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/ironicclient/tests/unit/v1/test_node.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11355 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/ironicclient/tests/unit/v1/test_port.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13737 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/ironicclient/tests/unit/v1/test_portgroup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3923 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/ironicclient/tests/unit/v1/test_resource_fields.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11601 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/ironicclient/tests/unit/v1/test_volume_connector.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10998 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/ironicclient/tests/unit/v1/test_volume_target.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-29 15:06:42.532656 python-ironicclient-5.5.0/ironicclient/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/ironicclient/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8839 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/ironicclient/v1/allocation.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8245 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/ironicclient/v1/chassis.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5711 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/ironicclient/v1/client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3713 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/ironicclient/v1/conductor.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13649 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/ironicclient/v1/create_resources.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4538 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/ironicclient/v1/deploy_template.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7352 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/ironicclient/v1/driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      902 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/ironicclient/v1/events.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    54635 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/ironicclient/v1/node.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5979 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/ironicclient/v1/port.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10726 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/ironicclient/v1/portgroup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17991 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/ironicclient/v1/resource_fields.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2370 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/ironicclient/v1/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4938 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/ironicclient/v1/volume_connector.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4928 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/ironicclient/v1/volume_target.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-29 15:06:42.512656 python-ironicclient-5.5.0/playbooks/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-29 15:06:42.532656 python-ironicclient-5.5.0/playbooks/functional/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1689 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/playbooks/functional/run.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      100 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/pyproject.toml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-29 15:06:42.532656 python-ironicclient-5.5.0/python_ironicclient.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4334 2024-02-29 15:06:42.000000 python-ironicclient-5.5.0/python_ironicclient.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16944 2024-02-29 15:06:42.000000 python-ironicclient-5.5.0/python_ironicclient.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-02-29 15:06:42.000000 python-ironicclient-5.5.0/python_ironicclient.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9087 2024-02-29 15:06:42.000000 python-ironicclient-5.5.0/python_ironicclient.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-02-29 15:06:42.000000 python-ironicclient-5.5.0/python_ironicclient.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2024-02-29 15:06:42.000000 python-ironicclient-5.5.0/python_ironicclient.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      427 2024-02-29 15:06:42.000000 python-ironicclient-5.5.0/python_ironicclient.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       13 2024-02-29 15:06:42.000000 python-ironicclient-5.5.0/python_ironicclient.egg-info/top_level.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-29 15:06:42.512656 python-ironicclient-5.5.0/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-29 15:06:42.560656 python-ironicclient-5.5.0/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       80 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/SHA1-hash-auth-token-f8dce46f854c002c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      568 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/accept-valid_interfaces-3b8f5e3e362e04cd.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      131 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/add-allocation-owner-0c6daad4ebfea5e6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      393 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/add-bios-registry-in-list-21974873f146aff7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      155 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/add-chassis_uuid-removal-possibility-5bc0bc3a7953eaa5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      189 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/add-conductor-cli-233249ebc9d5a5f3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      520 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/add-create-command-3df5efbbecc33276.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      888 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/add-deploy-steps-arg-0b127e29c8cf976d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      315 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/add-driver-cli-fields-selector-b0f527eb5f6fb2a9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      177 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/add-environment-variable-to-specify-version-cache-timeout-dfa5f6d4af0ea1d3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      314 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/add-events-support-53c461d28abf010b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      302 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/add-is-smartnic-port-attr-ed46d887aec276ed.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      133 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/add-json-option-0cf29be2a97e0212.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      174 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/add-network-data-node-attr-81dec9cecb7491b9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      432 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/add-neutron-integration-fields-cee7596c49722de6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      193 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/add-no-retired-opt-403bb5e466e4facb.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      132 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/add-node-boot-mode-08ac768649a2fc93.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      151 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/add-node-boot-mode-set-9746b45aa3f80fe8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      274 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/add-node-description-support-6efd0882eaa0c788.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      426 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/add-node-history-b9b9beeb0200f185.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      354 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/add-node-inventory-74e856c019cfa7e2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      127 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/add-node-lessee-c36409eb0415f75d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/add-node-owner-c2dce5a6075ce2b7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      120 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/add-node-resource-class-6040d1d6c734522c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      259 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/add-parent-node-support-450b111533c82440.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      100 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/add-pecan-exc-construction-a776408f7ae110dc.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      186 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/add-port-internal-info-74a03ebd8b0a3dfc.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      235 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/add-portgroup-mode-properties-0a3023cf905adaef.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      361 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/add-portgroups-support-c3cf3826093ee815.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/add-portgroups-to-create-command-6d685277f7af79df.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      396 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/add-rescue-interface-to-node-and-driver-e3ff9b5df2628e5a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      222 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/add-rescue-unrescue-support-f78266514ca59346.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      476 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/add-vif-attach-detach-support-e680d64e4add0fa4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      610 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/add-volume-connector-api-873090474d5e41b8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      710 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/add-volume-connector-cli-873090474d5e41b9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      571 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/add-volume-target-api-e062303f4b3b40ef.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      669 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/add-volume-target-cli-e062303f4b3b40f0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      211 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/add_api_versions-a59e5b6899833c33.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      212 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/add_automated_clean_field-d2a0c824a4e90bf4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      403 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/add_retired_field-6ec9f97c7c2f86ec.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      286 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/address-cross-distro-iso-tools-006711c9f150037a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      314 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/allocation-api-5f13082a8b36d788.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      127 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/allocation-backfill-4d4e51af2f787a72.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      215 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/allow-allocation-update-b4fb715045ab40a2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1226 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/allow-api-user-to-use-latest-6b80e9f584eaaa4e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      286 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/allow-client-to-request-list-of-versions-88f019cad76e6464.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      272 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/bug-1524745-adds-node-create-args-a7ace744515e5943.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      817 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/bug-1524745-extend-driver-list-and-driver-show-800d96393aa17342.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      247 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/bug-1524745-update-baremetal-node-set-c1ac57de0d481efe.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      298 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/bug-1712935-allow-os_baremetal_api_version_env_var_to_be_latest-28c8eed24f389673.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       88 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/bug-1724974-add-wanboot-to-supported-boot-devices.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      244 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/bug-1745099-allow-integer-portgroup-mode-6be4d3b35e216486.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      215 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/client-session-09e6ced1fbc6a9b0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      322 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/conductor-group-9cfab3756aa108e4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      331 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/configdrive-7bd2b67830691b2e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      229 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/configdrive-json-b9d173dde111cf22.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       86 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/continue-del-next-node-8827e67e1c41a0a5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      119 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/debug-e9dd680d783fa4b6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      414 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/deploy-templates-df354ce825b00430.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2705 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/deprecate-http-client-8d664e5ec50ec403.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      231 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/deprecate-ironic-cli-686b7a238ddf3e25.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      160 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/display-empty-string-for-chassis-uuid-if-it-is-empty-a5471c3aa740a27d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      282 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/driver-properties-for-osc-07a99d2d4e166436.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      228 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/drop-py-2-7-b0b950c0c2b6a667.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      238 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/endpoint-plus-version-4248f4f229dbc7dd.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/endpoint-strip-dea59ccb05628a35.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      201 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/extend-vif-attach-commands-ef3a931413ddcee7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      156 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/feature-parity-osc-cli-7606eed15f1c124f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      505 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/firmware-interface-ad0e9d58e4f61b2d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      358 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/fix-negotiate-version-503-c3cb8d1d4901541a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      261 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/fix-owner-feature-2f3f0163ff307727.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      179 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/fix-python3-compatibility-993ace45fefcba34.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      327 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/fix-token-with-vhosts-5d0a6d53e807fa5e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      297 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/implicit-version-warning-d34b99727b50d519.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      303 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/implicit-version-warning-old-cli-fe34d423ae63544a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      170 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/index-error-no-endpoint-eb281187f80a9aa4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      123 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/instance-crash-dump-d845a31e72b5a9f7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1165 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/ironic-cli-version-a5cdec73d585444d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/ironic-create-files-fix-c31e40e566ff86b8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      242 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/json-bytes-2f0085202d5e5796.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      175 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/keystone-token-auth-661a0c0d53c1b4de.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      288 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/latest-baremetal-api-version-a20e3099e3b97a1b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1270 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/latest-default-41fdcc49701c4d70.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      413 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/latest-renegotiation-55daa01b3fc261be.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       89 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/list-nodes-by-driver-b1e1e1018077089b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      243 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/logging-9c452e4869d80de9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      592 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/manual-clean-09f6b49df7d2513f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      397 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/missing-session-cc11e62dc966b4e0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      264 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/multinode-actions-9f682ad5172f032f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      246 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/negative-wrap-fix-4197e91b2ecfb722.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       83 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/network_data-c48b3878a5b04df5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      211 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/no-automated-clean-0e437581ded44eb3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      571 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/no-osc-requirement-411f25fd10f18caa.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      415 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/no-resource-attributeerror-d0cb327abab7dcc0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      358 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/node-deploy-step-061e8925dfee3918.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      540 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/node-driver-support-storage-interface-e93fc8d4de5d24d6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      166 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/node-fault-adbe74fd600063ee.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      164 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/node-shard-support-774ebfe6719fc7c2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      259 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/not-ignore-delete-failtures-0783d33a606ed6f1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      347 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/osc-baremetal-driver-raid-properties-159bd57058c0fc0e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      657 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/osc-baremetal-node-bios-setting-list-b062b31d0d4de337.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1170 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/osc-commands-1-7-d531960472a11ac2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      137 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/osc-default-microver-172d6e69316e70c1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/osc-instance-crash-dump-22634a57104561a5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      103 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/osc-max-microver-22-dc0d91a62f03a2e6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      203 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/osc-node-list-chassis-091d080684cdccf8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      201 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/osc-node-list-no-maintenance-ff1cef7cfbe60fb9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      179 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/osc-node-list-option-driver-a2901ba6b4e1d3b5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      105 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/osc-node-list-provisionstate-cd98dbddaad93e96.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      211 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/osc-node-list-unassociated-60e46958a0abc3e5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      418 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/osc-node-power-on-off-c269980e3b9c79ca.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      258 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/osc-node-rebuild-configdrive-8979d5b1373e8d5f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/osc-node-set-chassis-aae3413489b66b9b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      114 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/osc-plugin-9b5344aceb886cc1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      150 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/osc-plugin-chassis-create-show-fix-ee276d707c5a5bdf.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      525 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/osc-plugin-f87e0fbb472261dd.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1181 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/osc-plugin-ff0d897d8441a9e1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      144 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/osc-plugin-node-create-show-fix-283148c86fbccce2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      285 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/osc-plugin-node-set-target-raid-config-5d538d6253902ecb.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      219 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/osc-plugin-set-unset-target-raid-config-9a1cecb5620eafda.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      153 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/osc-port-create-uuid-5da551b154540ef7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      582 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/osc-port-set-llc-pxeenabled-21fd8ea1982af17e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/osc-soft-reboot-poweroff-121b8043567f54a9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/osc-versioned-endpoint-fix-08f6b7af2f47a5d6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      485 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/osc-wait-option-for-provisioning-commands-b6f5b875d573c9c8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      174 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/oslo-i18n-optional-ff28821441a0807c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       82 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/oslo.config-f67bf37ea35dd7fe.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      303 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/pass-interface-argument-deb92e3feb0bf051.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      124 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/port-physical-network-6ea8860d773e473c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      824 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/prelude-2-0-release-ee44150902d3d399.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      243 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/protected-72d7419245a4f6c3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      279 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/provision-state-adopt-d07b838813cecfb1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      247 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/provision-state-wait-e7ff919ce8e13703.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      509 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/raid_CLI_support-7e816ccd0fb31d2b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      197 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/remove-deprecated-endpoint-argument-fc0bd8099067e4ca.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      144 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/remove-deprecated-http-client-c969f583573251e9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      108 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/remove-deprecated-keystone-args-925ac5f3607a89a3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      932 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/remove-deprecated-osc-cmd-6dc980299d2fbde4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      203 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/remove-ironic-command-5c9f7bc4946996e0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      213 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/remove-llc-short-arg-89c7443acc6c54a4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      163 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/remove-states-field-0242960d121a09a7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      335 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/reset-interface-bbd7a612242db399.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      211 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/reset-interfaces-bec227bf933fea59.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      309 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/retry-on-keystone-auth-retriable-failures-91c08b9f8bdab7f3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      181 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/session-client-endpoint-override-20f1d822b4430afa.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      191 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/session-create-092172964afdb71b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      246 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/show-required-arguments-in-help-commands-of-node-create-port-create-b213bb28bcc94743.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      115 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/soft-reboot-poweroff-e33d078a05db3894.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      406 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/standalone-cli-f07834585909334a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       57 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/start-using-reno-ccd220efa2c7022a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/strip-prefix-when-paginating-6140465b1488828e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      530 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/support-passing-global-request-id-4b96beb31ec906cb.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      197 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/switch-requests-8304d4465a8976b1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      668 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/traits-support-8864f6816abecdb2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      236 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/typerror-132801fe4541fdb4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/update-api-version-to-1.85-0d79e372275061f9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      459 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/version-overrides-4e9ba1266a238c6a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      190 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/vif-attach-port-29a421b245e19f2b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      401 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/wait-for-prov-last-error-5f49b1c488879775.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      240 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/notes/yaml-files-79cd8367d7a4c2f2.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-29 15:06:42.564656 python-ironicclient-5.5.0/releasenotes/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/source/2023.1.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/source/2023.2.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-29 15:06:42.564656 python-ironicclient-5.5.0/releasenotes/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/source/_static/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-29 15:06:42.564656 python-ironicclient-5.5.0/releasenotes/source/_templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/source/_templates/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9019 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      284 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/source/mitaka.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/source/newton.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/source/ocata.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/source/pike.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/source/queens.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/source/rocky.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/source/stein.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      177 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/source/train.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/source/ussuri.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/source/victoria.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/source/wallaby.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/source/xena.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      128 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/source/yoga.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/releasenotes/source/zed.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      792 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10235 2024-02-29 15:06:42.568656 python-ironicclient-5.5.0/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      479 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/test-requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-29 15:06:42.564656 python-ironicclient-5.5.0/tools/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/tools/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6953 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/tools/install_venv_common.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      218 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/tools/with_venv.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3097 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/tox.ini
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-29 15:06:42.564656 python-ironicclient-5.5.0/zuul.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1252 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/zuul.d/ironicclient-jobs.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      609 2024-02-29 15:06:09.000000 python-ironicclient-5.5.0/zuul.d/project.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:33:10.021800 python-ironicclient-5.6.0/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       73 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/.coveragerc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       71 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7243 2024-05-08 05:33:09.000000 python-ironicclient-5.6.0/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      335 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    41230 2024-05-08 05:33:09.000000 python-ironicclient-5.6.0/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4334 2024-05-08 05:33:10.021800 python-ironicclient-5.6.0/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2592 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      127 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/bindep.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:33:09.977777 python-ironicclient-5.6.0/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      119 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:33:09.977777 python-ironicclient-5.6.0/doc/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3380 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/doc/source/api_v1.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:33:09.977777 python-ironicclient-5.6.0/doc/source/cli/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      164 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/doc/source/cli/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:33:09.973774 python-ironicclient-5.6.0/doc/source/cli/osc/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:33:09.977777 python-ironicclient-5.6.0/doc/source/cli/osc/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1408 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/doc/source/cli/osc/v1/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2602 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/doc/source/cli/osc_plugin_cli.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2923 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/doc/source/cli/standalone.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2719 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/doc/source/conf.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:33:09.977777 python-ironicclient-5.6.0/doc/source/contributor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1519 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/doc/source/contributor/contributing.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      180 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/doc/source/contributor/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1956 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/doc/source/contributor/testing.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      657 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/doc/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:33:09.977777 python-ironicclient-5.6.0/doc/source/reference/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      164 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/doc/source/reference/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:33:09.977777 python-ironicclient-5.6.0/doc/source/user/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5817 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/doc/source/user/create_command.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:33:09.977777 python-ironicclient-5.6.0/ironicclient/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      858 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/ironicclient/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6037 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/ironicclient/client.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:33:09.977777 python-ironicclient-5.6.0/ironicclient/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/ironicclient/common/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:33:09.977777 python-ironicclient-5.6.0/ironicclient/common/apiclient/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/ironicclient/common/apiclient/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16928 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/ironicclient/common/apiclient/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13414 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/ironicclient/common/apiclient/exceptions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13786 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/ironicclient/common/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3334 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/ironicclient/common/filecache.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    19501 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/ironicclient/common/http.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      890 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/ironicclient/common/i18n.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16410 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/ironicclient/common/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2695 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/ironicclient/exc.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:33:09.981779 python-ironicclient-5.6.0/ironicclient/osc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/ironicclient/osc/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5008 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/ironicclient/osc/plugin.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:33:09.981779 python-ironicclient-5.6.0/ironicclient/osc/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/ironicclient/osc/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14167 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/ironicclient/osc/v1/baremetal_allocation.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11134 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/ironicclient/osc/v1/baremetal_chassis.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     5486 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/ironicclient/osc/v1/baremetal_conductor.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1398 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/ironicclient/osc/v1/baremetal_create.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12397 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/ironicclient/osc/v1/baremetal_deploy_template.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9423 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/ironicclient/osc/v1/baremetal_driver.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)    86875 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/ironicclient/osc/v1/baremetal_node.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    19378 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/ironicclient/osc/v1/baremetal_port.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17413 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/ironicclient/osc/v1/baremetal_portgroup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13536 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/ironicclient/osc/v1/baremetal_volume_connector.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15268 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/ironicclient/osc/v1/baremetal_volume_target.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8614 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/ironicclient/shell.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:33:09.981779 python-ironicclient-5.6.0/ironicclient/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/ironicclient/tests/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:33:09.981779 python-ironicclient-5.6.0/ironicclient/tests/functional/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/ironicclient/tests/functional/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17958 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/ironicclient/tests/functional/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:33:09.981779 python-ironicclient-5.6.0/ironicclient/tests/functional/osc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/ironicclient/tests/functional/osc/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:33:09.985781 python-ironicclient-5.6.0/ironicclient/tests/functional/osc/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/ironicclient/tests/functional/osc/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18361 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/ironicclient/tests/functional/osc/v1/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8146 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/ironicclient/tests/functional/osc/v1/test_baremetal_allocation.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3308 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/ironicclient/tests/functional/osc/v1/test_baremetal_chassis_basic.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1424 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/ironicclient/tests/functional/osc/v1/test_baremetal_conductor_basic.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7239 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/ironicclient/tests/functional/osc/v1/test_baremetal_deploy_template_basic.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1364 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/ironicclient/tests/functional/osc/v1/test_baremetal_driver_basic.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9457 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/ironicclient/tests/functional/osc/v1/test_baremetal_node_basic.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1994 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/ironicclient/tests/functional/osc/v1/test_baremetal_node_create_negative.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4970 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/ironicclient/tests/functional/osc/v1/test_baremetal_node_fields.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3438 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/ironicclient/tests/functional/osc/v1/test_baremetal_node_negative.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2393 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/ironicclient/tests/functional/osc/v1/test_baremetal_node_power_states.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3877 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/ironicclient/tests/functional/osc/v1/test_baremetal_node_provision_states.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4800 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/ironicclient/tests/functional/osc/v1/test_baremetal_port_basic.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2963 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/ironicclient/tests/functional/osc/v1/test_baremetal_port_create.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5116 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/ironicclient/tests/functional/osc/v1/test_baremetal_portgroup_basic.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1115 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/ironicclient/tests/functional/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:33:09.985781 python-ironicclient-5.6.0/ironicclient/tests/unit/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/ironicclient/tests/unit/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:33:09.985781 python-ironicclient-5.6.0/ironicclient/tests/unit/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/ironicclient/tests/unit/common/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:33:09.985781 python-ironicclient-5.6.0/ironicclient/tests/unit/common/apiclient/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/ironicclient/tests/unit/common/apiclient/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7181 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/ironicclient/tests/unit/common/apiclient/test_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5355 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/ironicclient/tests/unit/common/apiclient/test_exceptions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9677 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/ironicclient/tests/unit/common/test_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8411 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/ironicclient/tests/unit/common/test_filecache.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    24336 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/ironicclient/tests/unit/common/test_http.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17668 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/ironicclient/tests/unit/common/test_utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:33:09.985781 python-ironicclient-5.6.0/ironicclient/tests/unit/osc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/ironicclient/tests/unit/osc/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1841 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/ironicclient/tests/unit/osc/fakes.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7293 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/ironicclient/tests/unit/osc/test_plugin.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:33:09.989783 python-ironicclient-5.6.0/ironicclient/tests/unit/osc/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/ironicclient/tests/unit/osc/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11576 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/ironicclient/tests/unit/osc/v1/fakes.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    23761 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/ironicclient/tests/unit/osc/v1/test_baremetal_allocation.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17983 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/ironicclient/tests/unit/osc/v1/test_baremetal_chassis.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9451 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/ironicclient/tests/unit/osc/v1/test_baremetal_conductor.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1739 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/ironicclient/tests/unit/osc/v1/test_baremetal_create.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16550 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/ironicclient/tests/unit/osc/v1/test_baremetal_deploy_template.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20501 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/ironicclient/tests/unit/osc/v1/test_baremetal_driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   153820 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/ironicclient/tests/unit/osc/v1/test_baremetal_node.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    29204 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/ironicclient/tests/unit/osc/v1/test_baremetal_port.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    28663 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/ironicclient/tests/unit/osc/v1/test_baremetal_portgroup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    31976 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/ironicclient/tests/unit/osc/v1/test_baremetal_volume_connector.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    38280 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/ironicclient/tests/unit/osc/v1/test_baremetal_volume_target.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11631 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/ironicclient/tests/unit/test_client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2627 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/ironicclient/tests/unit/test_exc.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1393 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/ironicclient/tests/unit/test_import.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5060 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/ironicclient/tests/unit/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:33:09.989783 python-ironicclient-5.6.0/ironicclient/tests/unit/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/ironicclient/tests/unit/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11950 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/ironicclient/tests/unit/v1/test_allocation.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14520 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/ironicclient/tests/unit/v1/test_chassis.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6113 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/ironicclient/tests/unit/v1/test_client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6549 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/ironicclient/tests/unit/v1/test_conductor.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    22786 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/ironicclient/tests/unit/v1/test_create_resources.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9684 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/ironicclient/tests/unit/v1/test_deploy_template.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9068 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/ironicclient/tests/unit/v1/test_driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1964 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/ironicclient/tests/unit/v1/test_events.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    78818 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/ironicclient/tests/unit/v1/test_node.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11355 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/ironicclient/tests/unit/v1/test_port.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13737 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/ironicclient/tests/unit/v1/test_portgroup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3923 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/ironicclient/tests/unit/v1/test_resource_fields.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11601 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/ironicclient/tests/unit/v1/test_volume_connector.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10998 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/ironicclient/tests/unit/v1/test_volume_target.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:33:09.993785 python-ironicclient-5.6.0/ironicclient/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/ironicclient/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8839 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/ironicclient/v1/allocation.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8245 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/ironicclient/v1/chassis.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5711 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/ironicclient/v1/client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3713 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/ironicclient/v1/conductor.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13649 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/ironicclient/v1/create_resources.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4538 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/ironicclient/v1/deploy_template.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7352 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/ironicclient/v1/driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      902 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/ironicclient/v1/events.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    55077 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/ironicclient/v1/node.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5979 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/ironicclient/v1/port.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10726 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/ironicclient/v1/portgroup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17991 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/ironicclient/v1/resource_fields.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2476 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/ironicclient/v1/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4938 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/ironicclient/v1/volume_connector.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4928 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/ironicclient/v1/volume_target.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:33:09.973774 python-ironicclient-5.6.0/playbooks/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:33:09.993785 python-ironicclient-5.6.0/playbooks/functional/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1689 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/playbooks/functional/run.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      100 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/pyproject.toml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:33:09.993785 python-ironicclient-5.6.0/python_ironicclient.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4334 2024-05-08 05:33:09.000000 python-ironicclient-5.6.0/python_ironicclient.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17103 2024-05-08 05:33:09.000000 python-ironicclient-5.6.0/python_ironicclient.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-05-08 05:33:09.000000 python-ironicclient-5.6.0/python_ironicclient.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9168 2024-05-08 05:33:09.000000 python-ironicclient-5.6.0/python_ironicclient.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-05-08 05:33:09.000000 python-ironicclient-5.6.0/python_ironicclient.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2024-05-08 05:33:09.000000 python-ironicclient-5.6.0/python_ironicclient.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      406 2024-05-08 05:33:09.000000 python-ironicclient-5.6.0/python_ironicclient.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       13 2024-05-08 05:33:09.000000 python-ironicclient-5.6.0/python_ironicclient.egg-info/top_level.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:33:09.973774 python-ironicclient-5.6.0/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:33:10.017798 python-ironicclient-5.6.0/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       80 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/SHA1-hash-auth-token-f8dce46f854c002c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      568 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/accept-valid_interfaces-3b8f5e3e362e04cd.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      131 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/add-allocation-owner-0c6daad4ebfea5e6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      393 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/add-bios-registry-in-list-21974873f146aff7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      155 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/add-chassis_uuid-removal-possibility-5bc0bc3a7953eaa5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      189 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/add-conductor-cli-233249ebc9d5a5f3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      520 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/add-create-command-3df5efbbecc33276.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      888 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/add-deploy-steps-arg-0b127e29c8cf976d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      315 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/add-driver-cli-fields-selector-b0f527eb5f6fb2a9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      177 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/add-environment-variable-to-specify-version-cache-timeout-dfa5f6d4af0ea1d3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      314 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/add-events-support-53c461d28abf010b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      302 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/add-is-smartnic-port-attr-ed46d887aec276ed.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      133 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/add-json-option-0cf29be2a97e0212.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      174 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/add-network-data-node-attr-81dec9cecb7491b9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      432 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/add-neutron-integration-fields-cee7596c49722de6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      193 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/add-no-retired-opt-403bb5e466e4facb.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      132 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/add-node-boot-mode-08ac768649a2fc93.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      151 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/add-node-boot-mode-set-9746b45aa3f80fe8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      274 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/add-node-description-support-6efd0882eaa0c788.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      426 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/add-node-history-b9b9beeb0200f185.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      354 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/add-node-inventory-74e856c019cfa7e2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      127 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/add-node-lessee-c36409eb0415f75d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/add-node-owner-c2dce5a6075ce2b7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      120 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/add-node-resource-class-6040d1d6c734522c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      259 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/add-parent-node-support-450b111533c82440.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      100 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/add-pecan-exc-construction-a776408f7ae110dc.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      186 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/add-port-internal-info-74a03ebd8b0a3dfc.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      235 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/add-portgroup-mode-properties-0a3023cf905adaef.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      361 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/add-portgroups-support-c3cf3826093ee815.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/add-portgroups-to-create-command-6d685277f7af79df.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      396 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/add-rescue-interface-to-node-and-driver-e3ff9b5df2628e5a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      222 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/add-rescue-unrescue-support-f78266514ca59346.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      216 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/add-service-steps-0c517e64563f6bbe.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      476 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/add-vif-attach-detach-support-e680d64e4add0fa4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      610 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/add-volume-connector-api-873090474d5e41b8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      710 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/add-volume-connector-cli-873090474d5e41b9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      571 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/add-volume-target-api-e062303f4b3b40ef.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      669 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/add-volume-target-cli-e062303f4b3b40f0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      211 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/add_api_versions-a59e5b6899833c33.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      212 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/add_automated_clean_field-d2a0c824a4e90bf4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      403 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/add_retired_field-6ec9f97c7c2f86ec.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      286 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/address-cross-distro-iso-tools-006711c9f150037a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      314 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/allocation-api-5f13082a8b36d788.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      127 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/allocation-backfill-4d4e51af2f787a72.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      215 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/allow-allocation-update-b4fb715045ab40a2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1226 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/allow-api-user-to-use-latest-6b80e9f584eaaa4e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      286 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/allow-client-to-request-list-of-versions-88f019cad76e6464.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      272 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/bug-1524745-adds-node-create-args-a7ace744515e5943.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      817 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/bug-1524745-extend-driver-list-and-driver-show-800d96393aa17342.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      247 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/bug-1524745-update-baremetal-node-set-c1ac57de0d481efe.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      298 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/bug-1712935-allow-os_baremetal_api_version_env_var_to_be_latest-28c8eed24f389673.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       88 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/bug-1724974-add-wanboot-to-supported-boot-devices.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      244 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/bug-1745099-allow-integer-portgroup-mode-6be4d3b35e216486.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      215 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/client-session-09e6ced1fbc6a9b0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      322 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/conductor-group-9cfab3756aa108e4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      331 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/configdrive-7bd2b67830691b2e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      229 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/configdrive-json-b9d173dde111cf22.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       86 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/continue-del-next-node-8827e67e1c41a0a5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      119 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/debug-e9dd680d783fa4b6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      414 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/deploy-templates-df354ce825b00430.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2705 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/deprecate-http-client-8d664e5ec50ec403.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      231 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/deprecate-ironic-cli-686b7a238ddf3e25.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      160 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/display-empty-string-for-chassis-uuid-if-it-is-empty-a5471c3aa740a27d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      282 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/driver-properties-for-osc-07a99d2d4e166436.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      228 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/drop-py-2-7-b0b950c0c2b6a667.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      238 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/endpoint-plus-version-4248f4f229dbc7dd.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/endpoint-strip-dea59ccb05628a35.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      201 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/extend-vif-attach-commands-ef3a931413ddcee7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      156 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/feature-parity-osc-cli-7606eed15f1c124f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      505 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/firmware-interface-ad0e9d58e4f61b2d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      358 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/fix-negotiate-version-503-c3cb8d1d4901541a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      221 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/fix-on-create-field-setting-60eb1ead99c69b12.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      261 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/fix-owner-feature-2f3f0163ff307727.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      179 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/fix-python3-compatibility-993ace45fefcba34.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      327 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/fix-token-with-vhosts-5d0a6d53e807fa5e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      297 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/implicit-version-warning-d34b99727b50d519.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      303 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/implicit-version-warning-old-cli-fe34d423ae63544a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      170 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/index-error-no-endpoint-eb281187f80a9aa4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      123 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/instance-crash-dump-d845a31e72b5a9f7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1165 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/ironic-cli-version-a5cdec73d585444d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/ironic-create-files-fix-c31e40e566ff86b8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      242 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/json-bytes-2f0085202d5e5796.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      175 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/keystone-token-auth-661a0c0d53c1b4de.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      288 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/latest-baremetal-api-version-a20e3099e3b97a1b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1270 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/latest-default-41fdcc49701c4d70.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      413 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/latest-renegotiation-55daa01b3fc261be.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       89 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/list-nodes-by-driver-b1e1e1018077089b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      243 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/logging-9c452e4869d80de9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      592 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/manual-clean-09f6b49df7d2513f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      397 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/missing-session-cc11e62dc966b4e0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      264 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/multinode-actions-9f682ad5172f032f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      246 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/negative-wrap-fix-4197e91b2ecfb722.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       83 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/network_data-c48b3878a5b04df5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      211 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/no-automated-clean-0e437581ded44eb3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      571 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/no-osc-requirement-411f25fd10f18caa.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      415 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/no-resource-attributeerror-d0cb327abab7dcc0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      358 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/node-deploy-step-061e8925dfee3918.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      540 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/node-driver-support-storage-interface-e93fc8d4de5d24d6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      166 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/node-fault-adbe74fd600063ee.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      164 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/node-shard-support-774ebfe6719fc7c2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      259 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/not-ignore-delete-failtures-0783d33a606ed6f1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      347 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/osc-baremetal-driver-raid-properties-159bd57058c0fc0e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      657 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/osc-baremetal-node-bios-setting-list-b062b31d0d4de337.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1170 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/osc-commands-1-7-d531960472a11ac2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      137 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/osc-default-microver-172d6e69316e70c1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/osc-instance-crash-dump-22634a57104561a5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      103 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/osc-max-microver-22-dc0d91a62f03a2e6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      203 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/osc-node-list-chassis-091d080684cdccf8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      201 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/osc-node-list-no-maintenance-ff1cef7cfbe60fb9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      179 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/osc-node-list-option-driver-a2901ba6b4e1d3b5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      105 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/osc-node-list-provisionstate-cd98dbddaad93e96.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      211 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/osc-node-list-unassociated-60e46958a0abc3e5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      418 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/osc-node-power-on-off-c269980e3b9c79ca.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      258 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/osc-node-rebuild-configdrive-8979d5b1373e8d5f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/osc-node-set-chassis-aae3413489b66b9b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      114 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/osc-plugin-9b5344aceb886cc1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      150 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/osc-plugin-chassis-create-show-fix-ee276d707c5a5bdf.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      525 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/osc-plugin-f87e0fbb472261dd.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1181 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/osc-plugin-ff0d897d8441a9e1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      144 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/osc-plugin-node-create-show-fix-283148c86fbccce2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      285 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/osc-plugin-node-set-target-raid-config-5d538d6253902ecb.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      219 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/osc-plugin-set-unset-target-raid-config-9a1cecb5620eafda.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      153 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/osc-port-create-uuid-5da551b154540ef7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      582 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/osc-port-set-llc-pxeenabled-21fd8ea1982af17e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/osc-soft-reboot-poweroff-121b8043567f54a9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/osc-versioned-endpoint-fix-08f6b7af2f47a5d6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      485 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/osc-wait-option-for-provisioning-commands-b6f5b875d573c9c8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      174 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/oslo-i18n-optional-ff28821441a0807c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       82 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/oslo.config-f67bf37ea35dd7fe.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      303 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/pass-interface-argument-deb92e3feb0bf051.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      124 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/port-physical-network-6ea8860d773e473c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      824 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/prelude-2-0-release-ee44150902d3d399.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      243 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/protected-72d7419245a4f6c3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      279 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/provision-state-adopt-d07b838813cecfb1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      247 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/provision-state-wait-e7ff919ce8e13703.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      509 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/raid_CLI_support-7e816ccd0fb31d2b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      197 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/remove-deprecated-endpoint-argument-fc0bd8099067e4ca.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      144 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/remove-deprecated-http-client-c969f583573251e9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      108 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/remove-deprecated-keystone-args-925ac5f3607a89a3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      932 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/remove-deprecated-osc-cmd-6dc980299d2fbde4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      203 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/remove-ironic-command-5c9f7bc4946996e0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      213 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/remove-llc-short-arg-89c7443acc6c54a4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      163 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/remove-states-field-0242960d121a09a7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      335 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/reset-interface-bbd7a612242db399.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      211 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/reset-interfaces-bec227bf933fea59.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      309 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/retry-on-keystone-auth-retriable-failures-91c08b9f8bdab7f3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      181 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/session-client-endpoint-override-20f1d822b4430afa.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      191 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/session-create-092172964afdb71b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      246 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/show-required-arguments-in-help-commands-of-node-create-port-create-b213bb28bcc94743.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      115 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/soft-reboot-poweroff-e33d078a05db3894.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      406 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/standalone-cli-f07834585909334a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       57 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/start-using-reno-ccd220efa2c7022a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/strip-prefix-when-paginating-6140465b1488828e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      530 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/support-passing-global-request-id-4b96beb31ec906cb.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      197 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/switch-requests-8304d4465a8976b1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      668 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/traits-support-8864f6816abecdb2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      236 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/typerror-132801fe4541fdb4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/update-api-version-to-1.85-0d79e372275061f9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      459 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/version-overrides-4e9ba1266a238c6a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      190 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/vif-attach-port-29a421b245e19f2b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      401 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/wait-for-prov-last-error-5f49b1c488879775.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      240 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/notes/yaml-files-79cd8367d7a4c2f2.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:33:10.021800 python-ironicclient-5.6.0/releasenotes/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/source/2023.1.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/source/2023.2.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/source/2024.1.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:33:10.021800 python-ironicclient-5.6.0/releasenotes/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/source/_static/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:33:10.021800 python-ironicclient-5.6.0/releasenotes/source/_templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/source/_templates/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9019 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      294 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/source/mitaka.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/source/newton.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/source/ocata.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/source/pike.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/source/queens.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/source/rocky.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/source/stein.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      177 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/source/train.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/source/ussuri.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/source/victoria.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/source/wallaby.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/source/xena.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      128 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/source/yoga.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      124 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/releasenotes/source/zed.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      567 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10317 2024-05-08 05:33:10.025802 python-ironicclient-5.6.0/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      263 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/test-requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:33:10.021800 python-ironicclient-5.6.0/tools/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/tools/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6953 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/tools/install_venv_common.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      218 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/tools/with_venv.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3097 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:33:10.021800 python-ironicclient-5.6.0/zuul.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1252 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/zuul.d/ironicclient-jobs.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      609 2024-05-08 05:32:40.000000 python-ironicclient-5.6.0/zuul.d/project.yaml
```

### Comparing `python-ironicclient-5.5.0/AUTHORS` & `python-ironicclient-5.6.0/AUTHORS`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.5.0/ChangeLog` & `python-ironicclient-5.6.0/ChangeLog`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,20 @@
 CHANGES
 =======
 
+5.6.0
+-----
+
+* reno: Update master for unmaintained/zed
+* Remove old excludes
+* Add Service Steps to client
+* Replace appdirs by platformdirs
+* Fix on-creation ability
+* Update master for stable/2024.1
+
 5.5.0
 -----
 
 * Add missing commands to the documentation
 * Moving functional job to non-voting until we have a fix for it
 * Force constraints when installing a package during tox test
 * reno: Update master for unmaintained/yoga
```

### Comparing `python-ironicclient-5.5.0/LICENSE` & `python-ironicclient-5.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.5.0/PKG-INFO` & `python-ironicclient-5.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-ironicclient
-Version: 5.5.0
+Version: 5.6.0
 Summary: OpenStack Bare Metal Provisioning API Client Library
 Home-page: https://docs.openstack.org/python-ironicclient/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ==================================
         Python bindings for the Ironic API
```

### Comparing `python-ironicclient-5.5.0/README.rst` & `python-ironicclient-5.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.5.0/doc/source/api_v1.rst` & `python-ironicclient-5.6.0/doc/source/api_v1.rst`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.5.0/doc/source/cli/osc/v1/index.rst` & `python-ironicclient-5.6.0/doc/source/cli/osc/v1/index.rst`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.5.0/doc/source/cli/osc_plugin_cli.rst` & `python-ironicclient-5.6.0/doc/source/cli/osc_plugin_cli.rst`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.5.0/doc/source/cli/standalone.rst` & `python-ironicclient-5.6.0/doc/source/cli/standalone.rst`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.5.0/doc/source/conf.py` & `python-ironicclient-5.6.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.5.0/doc/source/contributor/contributing.rst` & `python-ironicclient-5.6.0/doc/source/contributor/contributing.rst`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.5.0/doc/source/contributor/testing.rst` & `python-ironicclient-5.6.0/doc/source/contributor/testing.rst`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.5.0/doc/source/index.rst` & `python-ironicclient-5.6.0/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.5.0/doc/source/user/create_command.rst` & `python-ironicclient-5.6.0/doc/source/user/create_command.rst`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.5.0/ironicclient/__init__.py` & `python-ironicclient-5.6.0/ironicclient/__init__.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.5.0/ironicclient/client.py` & `python-ironicclient-5.6.0/ironicclient/client.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.5.0/ironicclient/common/apiclient/base.py` & `python-ironicclient-5.6.0/ironicclient/common/apiclient/base.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.5.0/ironicclient/common/apiclient/exceptions.py` & `python-ironicclient-5.6.0/ironicclient/common/apiclient/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.5.0/ironicclient/common/base.py` & `python-ironicclient-5.6.0/ironicclient/common/base.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.5.0/ironicclient/common/filecache.py` & `python-ironicclient-5.6.0/ironicclient/common/filecache.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,25 +13,25 @@
 #    WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #    License for the specific language governing permissions and limitations
 #    under the License.
 
 import logging
 import os
 
-import appdirs
 import dogpile.cache
+import platformdirs
 
 
 LOG = logging.getLogger(__name__)
 
 AUTHOR = 'openstack'
 PROGNAME = 'python-ironicclient'
 
 CACHE = None
-CACHE_DIR = appdirs.user_cache_dir(PROGNAME, AUTHOR)
+CACHE_DIR = platformdirs.user_cache_dir(PROGNAME, AUTHOR)
 CACHE_EXPIRY_ENV_VAR = 'IRONICCLIENT_CACHE_EXPIRY'  # environment variable
 CACHE_FILENAME = os.path.join(CACHE_DIR, 'ironic-api-version.dbm')
 DEFAULT_EXPIRY = 300  # seconds
 
 
 def _get_cache():
     """Configure file caching."""
```

### Comparing `python-ironicclient-5.5.0/ironicclient/common/http.py` & `python-ironicclient-5.6.0/ironicclient/common/http.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
 # NOTE(deva): Record the latest version that this client was tested with.
 #             We still have a lot of work to do in the client to implement
 #             microversion support in the client properly! See
 #             http://specs.openstack.org/openstack/ironic-specs/specs/kilo/api-microversions.html # noqa
 #             for full details.
 DEFAULT_VER = '1.9'
-LAST_KNOWN_API_VERSION = 86
+LAST_KNOWN_API_VERSION = 87
 LATEST_VERSION = '1.{}'.format(LAST_KNOWN_API_VERSION)
 
 LOG = logging.getLogger(__name__)
 USER_AGENT = 'python-ironicclient'
 CHUNKSIZE = 1024 * 64  # 64kB
 
 _MAJOR_VERSION = 1
```

### Comparing `python-ironicclient-5.5.0/ironicclient/common/i18n.py` & `python-ironicclient-5.6.0/ironicclient/common/i18n.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.5.0/ironicclient/common/utils.py` & `python-ironicclient-5.6.0/ironicclient/common/utils.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.5.0/ironicclient/exc.py` & `python-ironicclient-5.6.0/ironicclient/exc.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.5.0/ironicclient/osc/plugin.py` & `python-ironicclient-5.6.0/ironicclient/osc/plugin.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.5.0/ironicclient/osc/v1/baremetal_allocation.py` & `python-ironicclient-5.6.0/ironicclient/osc/v1/baremetal_allocation.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.5.0/ironicclient/osc/v1/baremetal_chassis.py` & `python-ironicclient-5.6.0/ironicclient/osc/v1/baremetal_chassis.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.5.0/ironicclient/osc/v1/baremetal_conductor.py` & `python-ironicclient-5.6.0/ironicclient/osc/v1/baremetal_conductor.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.5.0/ironicclient/osc/v1/baremetal_create.py` & `python-ironicclient-5.6.0/ironicclient/osc/v1/baremetal_create.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.5.0/ironicclient/osc/v1/baremetal_deploy_template.py` & `python-ironicclient-5.6.0/ironicclient/osc/v1/baremetal_deploy_template.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.5.0/ironicclient/osc/v1/baremetal_driver.py` & `python-ironicclient-5.6.0/ironicclient/osc/v1/baremetal_driver.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.5.0/ironicclient/osc/v1/baremetal_node.py` & `python-ironicclient-5.6.0/ironicclient/osc/v1/baremetal_node.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,14 +82,17 @@
 
         clean_steps = getattr(parsed_args, 'clean_steps', None)
         clean_steps = utils.handle_json_arg(clean_steps, 'clean steps')
 
         deploy_steps = getattr(parsed_args, 'deploy_steps', None)
         deploy_steps = utils.handle_json_arg(deploy_steps, 'deploy steps')
 
+        service_steps = getattr(parsed_args, 'service_steps', None)
+        service_steps = utils.handle_json_arg(service_steps, 'service steps')
+
         config_drive = getattr(parsed_args, 'config_drive', None)
         if config_drive:
             try:
                 config_drive_dict = json.loads(config_drive)
             except (ValueError, TypeError):
                 pass
             else:
@@ -101,15 +104,16 @@
         for node in parsed_args.nodes:
             baremetal_client.node.set_provision_state(
                 node,
                 parsed_args.provision_state,
                 configdrive=config_drive,
                 cleansteps=clean_steps,
                 deploysteps=deploy_steps,
-                rescue_password=rescue_password)
+                rescue_password=rescue_password,
+                servicesteps=service_steps)
 
 
 class ProvisionStateWithWait(ProvisionStateBaremetalNode):
     """Provision state class adding --wait flag."""
 
     log = logging.getLogger(__name__ + ".ProvisionStateWithWait")
 
@@ -296,14 +300,37 @@
                    "being read from standard input; OR a JSON string. The "
                    "value should be a list of clean-step dictionaries; each "
                    "dictionary should have keys 'interface' and 'step', and "
                    "optional key 'args'."))
         return parser
 
 
+class ServiceBaremetalNode(ProvisionStateWithWait):
+    """Set provision state of baremetal node to 'service'"""
+
+    log = logging.getLogger(__name__ + ".ServiceBaremetalNode")
+    PROVISION_STATE = 'service'
+
+    def get_parser(self, prog_name):
+        parser = super(ServiceBaremetalNode, self).get_parser(prog_name)
+
+        parser.add_argument(
+            '--service-steps',
+            metavar='<service-steps>',
+            required=True,
+            default=None,
+            help=_("The service steps. May be the path to a YAML file "
+                   "containing the service steps; OR '-', with the service "
+                   " steps being read from standard input; OR a JSON string. "
+                   "The value should be a list of service-step dictionaries; "
+                   "each dictionary should have keys 'interface' and 'step', "
+                   "and optional key 'args'."))
+        return parser
+
+
 class ConsoleDisableBaremetalNode(command.Command):
     """Disable console access for a node"""
 
     log = logging.getLogger(__name__ + ".ConsoleDisableBaremetalNode")
 
     def get_parser(self, prog_name):
         parser = super(ConsoleDisableBaremetalNode, self).get_parser(prog_name)
```

### Comparing `python-ironicclient-5.5.0/ironicclient/osc/v1/baremetal_port.py` & `python-ironicclient-5.6.0/ironicclient/osc/v1/baremetal_port.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.5.0/ironicclient/osc/v1/baremetal_portgroup.py` & `python-ironicclient-5.6.0/ironicclient/osc/v1/baremetal_portgroup.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.5.0/ironicclient/osc/v1/baremetal_volume_connector.py` & `python-ironicclient-5.6.0/ironicclient/osc/v1/baremetal_volume_connector.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.5.0/ironicclient/osc/v1/baremetal_volume_target.py` & `python-ironicclient-5.6.0/ironicclient/osc/v1/baremetal_volume_target.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.5.0/ironicclient/shell.py` & `python-ironicclient-5.6.0/ironicclient/shell.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.5.0/ironicclient/tests/functional/base.py` & `python-ironicclient-5.6.0/ironicclient/tests/functional/base.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.5.0/ironicclient/tests/functional/osc/v1/base.py` & `python-ironicclient-5.6.0/ironicclient/tests/functional/osc/v1/base.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.5.0/ironicclient/tests/functional/osc/v1/test_baremetal_allocation.py` & `python-ironicclient-5.6.0/ironicclient/tests/functional/osc/v1/test_baremetal_allocation.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.5.0/ironicclient/tests/functional/osc/v1/test_baremetal_chassis_basic.py` & `python-ironicclient-5.6.0/ironicclient/tests/functional/osc/v1/test_baremetal_chassis_basic.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.5.0/ironicclient/tests/functional/osc/v1/test_baremetal_conductor_basic.py` & `python-ironicclient-5.6.0/ironicclient/tests/functional/osc/v1/test_baremetal_conductor_basic.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.5.0/ironicclient/tests/functional/osc/v1/test_baremetal_deploy_template_basic.py` & `python-ironicclient-5.6.0/ironicclient/tests/functional/osc/v1/test_baremetal_deploy_template_basic.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.5.0/ironicclient/tests/functional/osc/v1/test_baremetal_driver_basic.py` & `python-ironicclient-5.6.0/ironicclient/tests/functional/osc/v1/test_baremetal_driver_basic.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.5.0/ironicclient/tests/functional/osc/v1/test_baremetal_node_basic.py` & `python-ironicclient-5.6.0/ironicclient/tests/functional/osc/v1/test_baremetal_node_basic.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.5.0/ironicclient/tests/functional/osc/v1/test_baremetal_node_create_negative.py` & `python-ironicclient-5.6.0/ironicclient/tests/functional/osc/v1/test_baremetal_node_create_negative.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.5.0/ironicclient/tests/functional/osc/v1/test_baremetal_node_fields.py` & `python-ironicclient-5.6.0/ironicclient/tests/functional/osc/v1/test_baremetal_node_fields.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.5.0/ironicclient/tests/functional/osc/v1/test_baremetal_node_negative.py` & `python-ironicclient-5.6.0/ironicclient/tests/functional/osc/v1/test_baremetal_node_negative.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.5.0/ironicclient/tests/functional/osc/v1/test_baremetal_node_power_states.py` & `python-ironicclient-5.6.0/ironicclient/tests/functional/osc/v1/test_baremetal_node_power_states.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.5.0/ironicclient/tests/functional/osc/v1/test_baremetal_node_provision_states.py` & `python-ironicclient-5.6.0/ironicclient/tests/functional/osc/v1/test_baremetal_node_provision_states.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.5.0/ironicclient/tests/functional/osc/v1/test_baremetal_port_basic.py` & `python-ironicclient-5.6.0/ironicclient/tests/functional/osc/v1/test_baremetal_port_basic.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.5.0/ironicclient/tests/functional/osc/v1/test_baremetal_port_create.py` & `python-ironicclient-5.6.0/ironicclient/tests/functional/osc/v1/test_baremetal_port_create.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.5.0/ironicclient/tests/functional/osc/v1/test_baremetal_portgroup_basic.py` & `python-ironicclient-5.6.0/ironicclient/tests/functional/osc/v1/test_baremetal_portgroup_basic.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.5.0/ironicclient/tests/functional/utils.py` & `python-ironicclient-5.6.0/ironicclient/tests/functional/utils.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.5.0/ironicclient/tests/unit/common/apiclient/test_base.py` & `python-ironicclient-5.6.0/ironicclient/tests/unit/common/apiclient/test_base.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.5.0/ironicclient/tests/unit/common/apiclient/test_exceptions.py` & `python-ironicclient-5.6.0/ironicclient/tests/unit/common/apiclient/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.5.0/ironicclient/tests/unit/common/test_base.py` & `python-ironicclient-5.6.0/ironicclient/tests/unit/common/test_base.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.5.0/ironicclient/tests/unit/common/test_filecache.py` & `python-ironicclient-5.6.0/ironicclient/tests/unit/common/test_filecache.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.5.0/ironicclient/tests/unit/common/test_http.py` & `python-ironicclient-5.6.0/ironicclient/tests/unit/common/test_http.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.5.0/ironicclient/tests/unit/common/test_utils.py` & `python-ironicclient-5.6.0/ironicclient/tests/unit/common/test_utils.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.5.0/ironicclient/tests/unit/osc/fakes.py` & `python-ironicclient-5.6.0/ironicclient/tests/unit/osc/fakes.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.5.0/ironicclient/tests/unit/osc/test_plugin.py` & `python-ironicclient-5.6.0/ironicclient/tests/unit/osc/test_plugin.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.5.0/ironicclient/tests/unit/osc/v1/fakes.py` & `python-ironicclient-5.6.0/ironicclient/tests/unit/osc/v1/fakes.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.5.0/ironicclient/tests/unit/osc/v1/test_baremetal_allocation.py` & `python-ironicclient-5.6.0/ironicclient/tests/unit/osc/v1/test_baremetal_allocation.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.5.0/ironicclient/tests/unit/osc/v1/test_baremetal_chassis.py` & `python-ironicclient-5.6.0/ironicclient/tests/unit/osc/v1/test_baremetal_chassis.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.5.0/ironicclient/tests/unit/osc/v1/test_baremetal_conductor.py` & `python-ironicclient-5.6.0/ironicclient/tests/unit/osc/v1/test_baremetal_conductor.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.5.0/ironicclient/tests/unit/osc/v1/test_baremetal_create.py` & `python-ironicclient-5.6.0/ironicclient/tests/unit/osc/v1/test_baremetal_create.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.5.0/ironicclient/tests/unit/osc/v1/test_baremetal_deploy_template.py` & `python-ironicclient-5.6.0/ironicclient/tests/unit/osc/v1/test_baremetal_deploy_template.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.5.0/ironicclient/tests/unit/osc/v1/test_baremetal_driver.py` & `python-ironicclient-5.6.0/ironicclient/tests/unit/osc/v1/test_baremetal_driver.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.5.0/ironicclient/tests/unit/osc/v1/test_baremetal_node.py` & `python-ironicclient-5.6.0/ironicclient/tests/unit/osc/v1/test_baremetal_node.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.cmd.take_action(parsed_args)
 
         self.baremetal_mock.node.set_provision_state.assert_called_once_with(
             'node_uuid', 'abort', cleansteps=None, configdrive=None,
-            deploysteps=None, rescue_password=None)
+            deploysteps=None, rescue_password=None, servicesteps=None)
 
 
 class TestAdopt(TestBaremetal):
     def setUp(self):
         super(TestAdopt, self).setUp()
 
         # Get the command object to test
@@ -79,15 +79,15 @@
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.cmd.take_action(parsed_args)
 
         self.baremetal_mock.node.set_provision_state.assert_called_once_with(
             'node_uuid', 'adopt',
             cleansteps=None, deploysteps=None, configdrive=None,
-            rescue_password=None)
+            rescue_password=None, servicesteps=None)
         self.baremetal_mock.node.wait_for_provision_state.assert_not_called()
 
     def test_adopt_baremetal_provision_state_active_and_wait(self):
         arglist = ['node_uuid',
                    '--wait', '15']
         verifylist = [
             ('nodes', ['node_uuid']),
@@ -99,15 +99,15 @@
 
         self.cmd.take_action(parsed_args)
 
         test_node = self.baremetal_mock.node
         test_node.set_provision_state.assert_called_once_with(
             'node_uuid', 'adopt',
             cleansteps=None, deploysteps=None, configdrive=None,
-            rescue_password=None)
+            rescue_password=None, servicesteps=None)
         test_node.wait_for_provision_state.assert_called_once_with(
             ['node_uuid'], expected_state='active',
             poll_interval=2, timeout=15)
 
     def test_adopt_baremetal_provision_state_default_wait(self):
         arglist = ['node_uuid',
                    '--wait']
@@ -121,15 +121,15 @@
 
         self.cmd.take_action(parsed_args)
 
         test_node = self.baremetal_mock.node
         test_node.set_provision_state.assert_called_once_with(
             'node_uuid', 'adopt',
             cleansteps=None, deploysteps=None, configdrive=None,
-            rescue_password=None)
+            rescue_password=None, servicesteps=None)
         test_node.wait_for_provision_state.assert_called_once_with(
             ['node_uuid'], expected_state='active',
             poll_interval=2, timeout=0)
 
 
 class TestClean(TestBaremetal):
     def setUp(self):
@@ -170,15 +170,51 @@
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.cmd.take_action(parsed_args)
 
         self.baremetal_mock.node.set_provision_state.assert_called_once_with(
             'node_uuid', 'clean', cleansteps=steps_dict, configdrive=None,
-            deploysteps=None, rescue_password=None)
+            deploysteps=None, rescue_password=None, servicesteps=None)
+
+
+class TestService(TestBaremetal):
+    def setUp(self):
+        super(TestService, self).setUp()
+
+        # Get the command object to test
+        self.cmd = baremetal_node.ServiceBaremetalNode(self.app, None)
+
+    def test_service_with_steps(self):
+        steps_dict = {
+            "service_steps": [{
+                "interface": "raid",
+                "step": "create_configuration",
+                "args": {"create_nonroot_volumes": False}
+            }, {
+                "interface": "deploy",
+                "step": "erase_devices"
+            }]
+        }
+        steps_json = json.dumps(steps_dict)
+
+        arglist = ['--service-steps', steps_json, 'node_uuid']
+        verifylist = [
+            ('service_steps', steps_json),
+            ('provision_state', 'service'),
+            ('nodes', ['node_uuid']),
+        ]
+
+        parsed_args = self.check_parser(self.cmd, arglist, verifylist)
+
+        self.cmd.take_action(parsed_args)
+
+        self.baremetal_mock.node.set_provision_state.assert_called_once_with(
+            'node_uuid', 'service', cleansteps=None, configdrive=None,
+            deploysteps=None, rescue_password=None, servicesteps=steps_dict)
 
 
 class TestInspect(TestBaremetal):
     def setUp(self):
         super(TestInspect, self).setUp()
 
         # Get the command object to test
@@ -193,15 +229,15 @@
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.cmd.take_action(parsed_args)
 
         self.baremetal_mock.node.set_provision_state.assert_called_once_with(
             'node_uuid', 'inspect', cleansteps=None, configdrive=None,
-            deploysteps=None, rescue_password=None)
+            deploysteps=None, rescue_password=None, servicesteps=None)
 
 
 class TestManage(TestBaremetal):
     def setUp(self):
         super(TestManage, self).setUp()
 
         # Get the command object to test
@@ -216,15 +252,15 @@
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.cmd.take_action(parsed_args)
 
         self.baremetal_mock.node.set_provision_state.assert_called_once_with(
             'node_uuid', 'manage', cleansteps=None, configdrive=None,
-            deploysteps=None, rescue_password=None)
+            deploysteps=None, rescue_password=None, servicesteps=None)
 
 
 class TestProvide(TestBaremetal):
     def setUp(self):
         super(TestProvide, self).setUp()
 
         # Get the command object to test
@@ -239,15 +275,15 @@
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.cmd.take_action(parsed_args)
 
         self.baremetal_mock.node.set_provision_state.assert_called_once_with(
             'node_uuid', 'provide', cleansteps=None, configdrive=None,
-            deploysteps=None, rescue_password=None)
+            deploysteps=None, rescue_password=None, servicesteps=None)
 
 
 class TestRebuild(TestBaremetal):
     def setUp(self):
         super(TestRebuild, self).setUp()
 
         # Get the command object to test
@@ -262,15 +298,15 @@
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.cmd.take_action(parsed_args)
 
         self.baremetal_mock.node.set_provision_state.assert_called_once_with(
             'node_uuid', 'rebuild', cleansteps=None, configdrive=None,
-            deploysteps=None, rescue_password=None)
+            deploysteps=None, rescue_password=None, servicesteps=None)
 
 
 class TestUndeploy(TestBaremetal):
     def setUp(self):
         super(TestUndeploy, self).setUp()
 
         # Get the command object to test
@@ -285,15 +321,15 @@
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.cmd.take_action(parsed_args)
 
         self.baremetal_mock.node.set_provision_state.assert_called_once_with(
             'node_uuid', 'deleted', cleansteps=None, configdrive=None,
-            deploysteps=None, rescue_password=None)
+            deploysteps=None, rescue_password=None, servicesteps=None)
 
 
 class TestBootdeviceSet(TestBaremetal):
     def setUp(self):
         super(TestBootdeviceSet, self).setUp()
 
         # Get the command object to test
@@ -1871,15 +1907,16 @@
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.cmd.take_action(parsed_args)
 
         self.baremetal_mock.node.set_provision_state.assert_called_once_with(
             'node_uuid', 'active',
             cleansteps=None, deploysteps=[{"interface": "deploy"}],
-            configdrive='path/to/drive', rescue_password=None)
+            configdrive='path/to/drive', rescue_password=None,
+            servicesteps=None)
 
     def test_deploy_baremetal_provision_state_active_and_configdrive_dict(
             self):
         arglist = ['node_uuid',
                    '--config-drive', '{"meta_data": {}}']
         verifylist = [
             ('nodes', ['node_uuid']),
@@ -1890,15 +1927,15 @@
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.cmd.take_action(parsed_args)
 
         self.baremetal_mock.node.set_provision_state.assert_called_once_with(
             'node_uuid', 'active',
             cleansteps=None, deploysteps=None, configdrive={'meta_data': {}},
-            rescue_password=None)
+            rescue_password=None, servicesteps=None)
 
     def test_deploy_no_wait(self):
         arglist = ['node_uuid']
         verifylist = [
             ('nodes', ['node_uuid']),
             ('provision_state', 'active')
         ]
@@ -1954,15 +1991,16 @@
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.cmd.take_action(parsed_args)
 
         test_node = self.baremetal_mock.node
         test_node.set_provision_state.assert_has_calls([
             mock.call(n, 'active', cleansteps=None, deploysteps=None,
-                      configdrive=None, rescue_password=None)
+                      configdrive=None, rescue_password=None,
+                      servicesteps=None)
             for n in ['node_uuid', 'node_name']
         ])
         test_node.wait_for_provision_state.assert_called_once_with(
             ['node_uuid', 'node_name'], expected_state='active',
             poll_interval=10, timeout=15)
 
     def test_deploy_baremetal_provision_state_mismatch(self):
@@ -2093,14 +2131,76 @@
 
         test_node = self.baremetal_mock.node
         test_node.wait_for_provision_state.assert_called_once_with(
             ['node_uuid'], expected_state='manageable',
             poll_interval=10, timeout=0)
 
 
+class TestServiceBaremetalProvisionState(TestBaremetal):
+    def setUp(self):
+        super(TestServiceBaremetalProvisionState, self).setUp()
+
+        # Get the command object to test
+        self.cmd = baremetal_node.ServiceBaremetalNode(self.app, None)
+
+    def test_service_no_wait(self):
+        arglist = ['node_uuid', '--service-steps', '-']
+        verifylist = [
+            ('nodes', ['node_uuid']),
+            ('provision_state', 'service'),
+            ('service_steps', '-')
+        ]
+
+        parsed_args = self.check_parser(self.cmd, arglist, verifylist)
+
+        self.cmd.take_action(parsed_args)
+
+        self.baremetal_mock.node.wait_for_provision_state.assert_not_called()
+
+    def test_service_baremetal_provision_state_manageable_and_wait(self):
+        arglist = ['node_uuid',
+                   '--wait', '15',
+                   '--service-steps', '-']
+        verifylist = [
+            ('nodes', ['node_uuid']),
+            ('provision_state', 'service'),
+            ('wait_timeout', 15),
+            ('service_steps', '-')
+        ]
+
+        parsed_args = self.check_parser(self.cmd, arglist, verifylist)
+
+        self.cmd.take_action(parsed_args)
+
+        test_node = self.baremetal_mock.node
+        test_node.wait_for_provision_state.assert_called_once_with(
+            ['node_uuid'], expected_state='active',
+            poll_interval=10, timeout=15)
+
+    def test_service_baremetal_provision_state_default_wait(self):
+        arglist = ['node_uuid',
+                   '--wait',
+                   '--service-steps', '-']
+        verifylist = [
+            ('nodes', ['node_uuid']),
+            ('provision_state', 'service'),
+            ('wait_timeout', 0),
+            ('service_steps', '-')
+        ]
+
+        parsed_args = self.check_parser(self.cmd, arglist, verifylist)
+
+        self.cmd.take_action(parsed_args)
+
+        test_node = self.baremetal_mock.node
+        test_node.wait_for_provision_state.assert_called_once_with(
+            ['node_uuid'], expected_state='active',
+            poll_interval=10, timeout=0)
+
+
 class TestRescueBaremetalProvisionState(TestBaremetal):
     def setUp(self):
         super(TestRescueBaremetalProvisionState, self).setUp()
 
         # Get the command object to test
         self.cmd = baremetal_node.RescueBaremetalNode(self.app, None)
 
@@ -2115,15 +2215,16 @@
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.cmd.take_action(parsed_args)
 
         self.baremetal_mock.node.set_provision_state.assert_called_once_with(
             'node_uuid', 'rescue', cleansteps=None, deploysteps=None,
-            configdrive=None, rescue_password='supersecret')
+            configdrive=None, rescue_password='supersecret',
+            servicesteps=None)
 
     def test_rescue_baremetal_provision_state_rescue_and_wait(self):
         arglist = ['node_uuid',
                    '--wait', '15',
                    '--rescue-password', 'supersecret']
         verifylist = [
             ('nodes', ['node_uuid']),
@@ -2306,15 +2407,16 @@
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.cmd.take_action(parsed_args)
 
         self.baremetal_mock.node.set_provision_state.assert_called_once_with(
             'node_uuid', 'rebuild',
             cleansteps=None, deploysteps=[{"interface": "deploy"}],
-            configdrive='path/to/drive', rescue_password=None)
+            configdrive='path/to/drive', rescue_password=None,
+            servicesteps=None)
 
     def test_rebuild_no_wait(self):
         arglist = ['node_uuid']
         verifylist = [
             ('nodes', ['node_uuid']),
             ('provision_state', 'rebuild')
         ]
@@ -2322,15 +2424,15 @@
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.cmd.take_action(parsed_args)
 
         self.baremetal_mock.node.set_provision_state.assert_called_once_with(
             'node_uuid', 'rebuild',
             cleansteps=None, deploysteps=None, configdrive=None,
-            rescue_password=None)
+            rescue_password=None, servicesteps=None)
 
         self.baremetal_mock.node.wait_for_provision_state.assert_not_called()
 
     def test_rebuild_baremetal_provision_state_active_and_wait(self):
         arglist = ['node_uuid',
                    '--wait', '15']
         verifylist = [
@@ -2440,15 +2542,15 @@
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.cmd.take_action(parsed_args)
 
         self.baremetal_mock.node.set_provision_state.assert_called_once_with(
             'node_uuid', 'unrescue', cleansteps=None, deploysteps=None,
-            configdrive=None, rescue_password=None)
+            configdrive=None, rescue_password=None, servicesteps=None)
 
     def test_unrescue_baremetal_provision_state_active_and_wait(self):
         arglist = ['node_uuid',
                    '--wait', '15']
         verifylist = [
             ('nodes', ['node_uuid']),
             ('provision_state', 'unrescue'),
@@ -4555,15 +4657,15 @@
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.cmd.take_action(parsed_args)
 
         self.baremetal_mock.node.set_provision_state.assert_called_once_with(
             'node_uuid', 'unhold', cleansteps=None, deploysteps=None,
-            configdrive=None, rescue_password=None)
+            configdrive=None, rescue_password=None, servicesteps=None)
 
 
 class TestListFirmwareComponents(TestBaremetal):
     def setUp(self):
         super(TestListFirmwareComponents, self).setUp()
 
         self.baremetal_mock.node.list_firmware_components.return_value = (
```

### Comparing `python-ironicclient-5.5.0/ironicclient/tests/unit/osc/v1/test_baremetal_port.py` & `python-ironicclient-5.6.0/ironicclient/tests/unit/osc/v1/test_baremetal_port.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.5.0/ironicclient/tests/unit/osc/v1/test_baremetal_portgroup.py` & `python-ironicclient-5.6.0/ironicclient/tests/unit/osc/v1/test_baremetal_portgroup.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.5.0/ironicclient/tests/unit/osc/v1/test_baremetal_volume_connector.py` & `python-ironicclient-5.6.0/ironicclient/tests/unit/osc/v1/test_baremetal_volume_connector.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.5.0/ironicclient/tests/unit/osc/v1/test_baremetal_volume_target.py` & `python-ironicclient-5.6.0/ironicclient/tests/unit/osc/v1/test_baremetal_volume_target.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.5.0/ironicclient/tests/unit/test_client.py` & `python-ironicclient-5.6.0/ironicclient/tests/unit/test_client.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.5.0/ironicclient/tests/unit/test_exc.py` & `python-ironicclient-5.6.0/ironicclient/tests/unit/test_exc.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.5.0/ironicclient/tests/unit/test_import.py` & `python-ironicclient-5.6.0/ironicclient/tests/unit/test_import.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.5.0/ironicclient/tests/unit/utils.py` & `python-ironicclient-5.6.0/ironicclient/tests/unit/utils.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.5.0/ironicclient/tests/unit/v1/test_allocation.py` & `python-ironicclient-5.6.0/ironicclient/tests/unit/v1/test_allocation.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.5.0/ironicclient/tests/unit/v1/test_chassis.py` & `python-ironicclient-5.6.0/ironicclient/tests/unit/v1/test_chassis.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.5.0/ironicclient/tests/unit/v1/test_client.py` & `python-ironicclient-5.6.0/ironicclient/tests/unit/v1/test_client.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.5.0/ironicclient/tests/unit/v1/test_conductor.py` & `python-ironicclient-5.6.0/ironicclient/tests/unit/v1/test_conductor.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.5.0/ironicclient/tests/unit/v1/test_create_resources.py` & `python-ironicclient-5.6.0/ironicclient/tests/unit/v1/test_create_resources.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.5.0/ironicclient/tests/unit/v1/test_deploy_template.py` & `python-ironicclient-5.6.0/ironicclient/tests/unit/v1/test_deploy_template.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.5.0/ironicclient/tests/unit/v1/test_driver.py` & `python-ironicclient-5.6.0/ironicclient/tests/unit/v1/test_driver.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.5.0/ironicclient/tests/unit/v1/test_events.py` & `python-ironicclient-5.6.0/ironicclient/tests/unit/v1/test_events.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.5.0/ironicclient/tests/unit/v1/test_node.py` & `python-ironicclient-5.6.0/ironicclient/tests/unit/v1/test_node.py`

 * *Files 0% similar despite different names*

```diff
@@ -1774,14 +1774,25 @@
                 'configdrive': {'user_data': ''},
                 'deploy_steps': deploysteps}
         expect = [
             ('PUT', '/v1/nodes/%s/states/provision' % NODE1['uuid'], {}, body),
         ]
         self.assertEqual(expect, self.api.calls)
 
+    def test_node_set_provision_state_with_servicesteps(self):
+        servicesteps = [{"step": "magic", "interface": "deploy"}]
+        target_state = 'service'
+        self.mgr.set_provision_state(NODE1['uuid'], target_state,
+                                     servicesteps=servicesteps)
+        body = {'target': target_state, 'service_steps': servicesteps}
+        expect = [
+            ('PUT', '/v1/nodes/%s/states/provision' % NODE1['uuid'], {}, body),
+        ]
+        self.assertEqual(expect, self.api.calls)
+
     def test_node_set_provision_state_with_rescue_password(self):
         rescue_password = 'supersecret'
         target_state = 'rescue'
         self.mgr.set_provision_state(NODE1['uuid'], target_state,
                                      rescue_password=rescue_password)
         body = {'target': target_state, 'rescue_password': rescue_password}
         expect = [
```

### Comparing `python-ironicclient-5.5.0/ironicclient/tests/unit/v1/test_port.py` & `python-ironicclient-5.6.0/ironicclient/tests/unit/v1/test_port.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.5.0/ironicclient/tests/unit/v1/test_portgroup.py` & `python-ironicclient-5.6.0/ironicclient/tests/unit/v1/test_portgroup.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.5.0/ironicclient/tests/unit/v1/test_resource_fields.py` & `python-ironicclient-5.6.0/ironicclient/tests/unit/v1/test_resource_fields.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.5.0/ironicclient/tests/unit/v1/test_volume_connector.py` & `python-ironicclient-5.6.0/ironicclient/tests/unit/v1/test_volume_connector.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.5.0/ironicclient/tests/unit/v1/test_volume_target.py` & `python-ironicclient-5.6.0/ironicclient/tests/unit/v1/test_volume_target.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.5.0/ironicclient/v1/allocation.py` & `python-ironicclient-5.6.0/ironicclient/v1/allocation.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.5.0/ironicclient/v1/chassis.py` & `python-ironicclient-5.6.0/ironicclient/v1/chassis.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.5.0/ironicclient/v1/client.py` & `python-ironicclient-5.6.0/ironicclient/v1/client.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.5.0/ironicclient/v1/conductor.py` & `python-ironicclient-5.6.0/ironicclient/v1/conductor.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.5.0/ironicclient/v1/create_resources.py` & `python-ironicclient-5.6.0/ironicclient/v1/create_resources.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.5.0/ironicclient/v1/deploy_template.py` & `python-ironicclient-5.6.0/ironicclient/v1/deploy_template.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.5.0/ironicclient/v1/driver.py` & `python-ironicclient-5.6.0/ironicclient/v1/driver.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.5.0/ironicclient/v1/events.py` & `python-ironicclient-5.6.0/ironicclient/v1/events.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.5.0/ironicclient/v1/node.py` & `python-ironicclient-5.6.0/ironicclient/v1/node.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,17 +48,18 @@
                             'extra', 'uuid', 'properties', 'name',
                             'bios_interface', 'boot_interface',
                             'console_interface', 'deploy_interface',
                             'inspect_interface', 'management_interface',
                             'network_interface', 'power_interface',
                             'raid_interface', 'rescue_interface',
                             'storage_interface', 'vendor_interface',
-                            'resource_class', 'conductor_group',
-                            'automated_clean', 'network_data',
-                            'parent_node']
+                            'firmware_interface', 'resource_class',
+                            'conductor_group', 'automated_clean',
+                            'network_data', 'parent_node',
+                            'owner', 'lessee', 'shard', 'description']
     _resource_name = 'nodes'
 
     def list(self, associated=None, maintenance=None, marker=None,
              limit=None, detail=False, sort_key=None, sort_dir=None,
              fields=None, provision_state=None, driver=None,
              resource_class=None, chassis=None, fault=None,
              os_ironic_api_version=None, conductor_group=None,
@@ -718,15 +719,16 @@
         path = "%s/validate" % node_uuid
         return self.get(path, os_ironic_api_version=os_ironic_api_version,
                         global_request_id=global_request_id)
 
     def set_provision_state(
             self, node_uuid, state, configdrive=None, cleansteps=None,
             rescue_password=None, os_ironic_api_version=None,
-            global_request_id=None, deploysteps=None):
+            global_request_id=None, deploysteps=None,
+            servicesteps=None):
         """Set the provision state for the node.
 
         :param node_uuid: The UUID or name of the node.
         :param state: The desired provision state. One of 'active', 'deleted',
              'rebuild', 'inspect', 'provide', 'manage', 'clean', 'abort',
              'rescue', 'unrescue'.
         :param configdrive: One of:
@@ -752,14 +754,18 @@
             the request.  If not specified, the client's default is used.
         :param global_request_id: String containing global request ID header
             value (in form "req-<UUID>") to use for the request.
         :param deploysteps: The deploy steps as a list of deploy-step
             dictionaries; each dictionary should have keys 'interface', 'step',
             'priority', and optional key 'args'. This is optional and is
             only valid when setting provision-state to 'active' or 'rebuild'.
+        :param servicesteps: The service steps as list of service-step
+            dictionaries; each dictonary should have keys 'interface', 'step',
+            and optional key 'args' when setting an 'active' nodes to
+            'service'.
         :raises: InvalidAttribute if there was an error with the clean steps or
             deploy steps
         :returns: The status of the request
         """
 
         path = "%s/states/provision" % node_uuid
         body = {'target': state}
@@ -789,14 +795,17 @@
             body['clean_steps'] = cleansteps
         elif rescue_password:
             body['rescue_password'] = rescue_password
 
         if deploysteps:
             body['deploy_steps'] = deploysteps
 
+        if servicesteps:
+            body['service_steps'] = servicesteps
+
         return self.update(path, body, http_method='PUT',
                            os_ironic_api_version=os_ironic_api_version,
                            global_request_id=global_request_id)
 
     def states(self, node_uuid, os_ironic_api_version=None,
                global_request_id=None):
         path = "%s/states" % node_uuid
```

### Comparing `python-ironicclient-5.5.0/ironicclient/v1/port.py` & `python-ironicclient-5.6.0/ironicclient/v1/port.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.5.0/ironicclient/v1/portgroup.py` & `python-ironicclient-5.6.0/ironicclient/v1/portgroup.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.5.0/ironicclient/v1/resource_fields.py` & `python-ironicclient-5.6.0/ironicclient/v1/resource_fields.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.5.0/ironicclient/v1/utils.py` & `python-ironicclient-5.6.0/ironicclient/v1/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,10 +43,12 @@
     'adopt': {'expected_state': 'active',
               'poll_interval': _SHORT_ACTION_POLL_INTERVAL},
     'abort': None,  # no support for --wait in abort
     'rescue': {'expected_state': 'rescue',
                'poll_interval': _LONG_ACTION_POLL_INTERVAL},
     'unrescue': {'expected_state': 'active',
                  'poll_interval': _LONG_ACTION_POLL_INTERVAL},
+    'service': {'expected_state': 'active',
+                'poll_interval': _LONG_ACTION_POLL_INTERVAL},
 }
 
 PROVISION_STATES = list(PROVISION_ACTIONS)
```

### Comparing `python-ironicclient-5.5.0/ironicclient/v1/volume_connector.py` & `python-ironicclient-5.6.0/ironicclient/v1/volume_connector.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.5.0/ironicclient/v1/volume_target.py` & `python-ironicclient-5.6.0/ironicclient/v1/volume_target.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.5.0/playbooks/functional/run.yaml` & `python-ironicclient-5.6.0/playbooks/functional/run.yaml`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.5.0/python_ironicclient.egg-info/PKG-INFO` & `python-ironicclient-5.6.0/python_ironicclient.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-ironicclient
-Version: 5.5.0
+Version: 5.6.0
 Summary: OpenStack Bare Metal Provisioning API Client Library
 Home-page: https://docs.openstack.org/python-ironicclient/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ==================================
         Python bindings for the Ironic API
```

### Comparing `python-ironicclient-5.5.0/python_ironicclient.egg-info/SOURCES.txt` & `python-ironicclient-5.6.0/python_ironicclient.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -171,14 +171,15 @@
 releasenotes/notes/add-pecan-exc-construction-a776408f7ae110dc.yaml
 releasenotes/notes/add-port-internal-info-74a03ebd8b0a3dfc.yaml
 releasenotes/notes/add-portgroup-mode-properties-0a3023cf905adaef.yaml
 releasenotes/notes/add-portgroups-support-c3cf3826093ee815.yaml
 releasenotes/notes/add-portgroups-to-create-command-6d685277f7af79df.yaml
 releasenotes/notes/add-rescue-interface-to-node-and-driver-e3ff9b5df2628e5a.yaml
 releasenotes/notes/add-rescue-unrescue-support-f78266514ca59346.yaml
+releasenotes/notes/add-service-steps-0c517e64563f6bbe.yaml
 releasenotes/notes/add-vif-attach-detach-support-e680d64e4add0fa4.yaml
 releasenotes/notes/add-volume-connector-api-873090474d5e41b8.yaml
 releasenotes/notes/add-volume-connector-cli-873090474d5e41b9.yaml
 releasenotes/notes/add-volume-target-api-e062303f4b3b40ef.yaml
 releasenotes/notes/add-volume-target-cli-e062303f4b3b40f0.yaml
 releasenotes/notes/add_api_versions-a59e5b6899833c33.yaml
 releasenotes/notes/add_automated_clean_field-d2a0c824a4e90bf4.yaml
@@ -209,14 +210,15 @@
 releasenotes/notes/drop-py-2-7-b0b950c0c2b6a667.yaml
 releasenotes/notes/endpoint-plus-version-4248f4f229dbc7dd.yaml
 releasenotes/notes/endpoint-strip-dea59ccb05628a35.yaml
 releasenotes/notes/extend-vif-attach-commands-ef3a931413ddcee7.yaml
 releasenotes/notes/feature-parity-osc-cli-7606eed15f1c124f.yaml
 releasenotes/notes/firmware-interface-ad0e9d58e4f61b2d.yaml
 releasenotes/notes/fix-negotiate-version-503-c3cb8d1d4901541a.yaml
+releasenotes/notes/fix-on-create-field-setting-60eb1ead99c69b12.yaml
 releasenotes/notes/fix-owner-feature-2f3f0163ff307727.yaml
 releasenotes/notes/fix-python3-compatibility-993ace45fefcba34.yaml
 releasenotes/notes/fix-token-with-vhosts-5d0a6d53e807fa5e.yaml
 releasenotes/notes/implicit-version-warning-d34b99727b50d519.yaml
 releasenotes/notes/implicit-version-warning-old-cli-fe34d423ae63544a.yaml
 releasenotes/notes/index-error-no-endpoint-eb281187f80a9aa4.yaml
 releasenotes/notes/instance-crash-dump-d845a31e72b5a9f7.yaml
@@ -301,14 +303,15 @@
 releasenotes/notes/update-api-version-to-1.85-0d79e372275061f9.yaml
 releasenotes/notes/version-overrides-4e9ba1266a238c6a.yaml
 releasenotes/notes/vif-attach-port-29a421b245e19f2b.yaml
 releasenotes/notes/wait-for-prov-last-error-5f49b1c488879775.yaml
 releasenotes/notes/yaml-files-79cd8367d7a4c2f2.yaml
 releasenotes/source/2023.1.rst
 releasenotes/source/2023.2.rst
+releasenotes/source/2024.1.rst
 releasenotes/source/conf.py
 releasenotes/source/index.rst
 releasenotes/source/mitaka.rst
 releasenotes/source/newton.rst
 releasenotes/source/ocata.rst
 releasenotes/source/pike.rst
 releasenotes/source/queens.rst
```

### Comparing `python-ironicclient-5.5.0/python_ironicclient.egg-info/entry_points.txt` & `python-ironicclient-5.6.0/python_ironicclient.egg-info/entry_points.txt`

 * *Files 1% similar despite different names*

```diff
@@ -62,14 +62,15 @@
 baremetal_node_provide = ironicclient.osc.v1.baremetal_node:ProvideBaremetalNode
 baremetal_node_reboot = ironicclient.osc.v1.baremetal_node:RebootBaremetalNode
 baremetal_node_rebuild = ironicclient.osc.v1.baremetal_node:RebuildBaremetalNode
 baremetal_node_remove_trait = ironicclient.osc.v1.baremetal_node:RemoveTraitBaremetalNode
 baremetal_node_rescue = ironicclient.osc.v1.baremetal_node:RescueBaremetalNode
 baremetal_node_secure_boot_off = ironicclient.osc.v1.baremetal_node:SecurebootOffBaremetalNode
 baremetal_node_secure_boot_on = ironicclient.osc.v1.baremetal_node:SecurebootOnBaremetalNode
+baremetal_node_service = ironicclient.osc.v1.baremetal_node:ServiceBaremetalNode
 baremetal_node_set = ironicclient.osc.v1.baremetal_node:SetBaremetalNode
 baremetal_node_show = ironicclient.osc.v1.baremetal_node:ShowBaremetalNode
 baremetal_node_trait_list = ironicclient.osc.v1.baremetal_node:ListTraitsBaremetalNode
 baremetal_node_undeploy = ironicclient.osc.v1.baremetal_node:UndeployBaremetalNode
 baremetal_node_unhold = ironicclient.osc.v1.baremetal_node:UnholdBaremetalNode
 baremetal_node_unrescue = ironicclient.osc.v1.baremetal_node:UnrescueBaremetalNode
 baremetal_node_unset = ironicclient.osc.v1.baremetal_node:UnsetBaremetalNode
```

### Comparing `python-ironicclient-5.5.0/releasenotes/notes/accept-valid_interfaces-3b8f5e3e362e04cd.yaml` & `python-ironicclient-5.6.0/releasenotes/notes/accept-valid_interfaces-3b8f5e3e362e04cd.yaml`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.5.0/releasenotes/notes/add-create-command-3df5efbbecc33276.yaml` & `python-ironicclient-5.6.0/releasenotes/notes/add-create-command-3df5efbbecc33276.yaml`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.5.0/releasenotes/notes/add-deploy-steps-arg-0b127e29c8cf976d.yaml` & `python-ironicclient-5.6.0/releasenotes/notes/add-deploy-steps-arg-0b127e29c8cf976d.yaml`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.5.0/releasenotes/notes/add-volume-connector-api-873090474d5e41b8.yaml` & `python-ironicclient-5.6.0/releasenotes/notes/add-volume-connector-api-873090474d5e41b8.yaml`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.5.0/releasenotes/notes/add-volume-connector-cli-873090474d5e41b9.yaml` & `python-ironicclient-5.6.0/releasenotes/notes/add-volume-connector-cli-873090474d5e41b9.yaml`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.5.0/releasenotes/notes/add-volume-target-api-e062303f4b3b40ef.yaml` & `python-ironicclient-5.6.0/releasenotes/notes/add-volume-target-api-e062303f4b3b40ef.yaml`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.5.0/releasenotes/notes/add-volume-target-cli-e062303f4b3b40f0.yaml` & `python-ironicclient-5.6.0/releasenotes/notes/add-volume-target-cli-e062303f4b3b40f0.yaml`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.5.0/releasenotes/notes/allow-api-user-to-use-latest-6b80e9f584eaaa4e.yaml` & `python-ironicclient-5.6.0/releasenotes/notes/allow-api-user-to-use-latest-6b80e9f584eaaa4e.yaml`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.5.0/releasenotes/notes/bug-1524745-extend-driver-list-and-driver-show-800d96393aa17342.yaml` & `python-ironicclient-5.6.0/releasenotes/notes/bug-1524745-extend-driver-list-and-driver-show-800d96393aa17342.yaml`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.5.0/releasenotes/notes/deprecate-http-client-8d664e5ec50ec403.yaml` & `python-ironicclient-5.6.0/releasenotes/notes/deprecate-http-client-8d664e5ec50ec403.yaml`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.5.0/releasenotes/notes/ironic-cli-version-a5cdec73d585444d.yaml` & `python-ironicclient-5.6.0/releasenotes/notes/ironic-cli-version-a5cdec73d585444d.yaml`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.5.0/releasenotes/notes/latest-default-41fdcc49701c4d70.yaml` & `python-ironicclient-5.6.0/releasenotes/notes/latest-default-41fdcc49701c4d70.yaml`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.5.0/releasenotes/notes/manual-clean-09f6b49df7d2513f.yaml` & `python-ironicclient-5.6.0/releasenotes/notes/manual-clean-09f6b49df7d2513f.yaml`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.5.0/releasenotes/notes/no-osc-requirement-411f25fd10f18caa.yaml` & `python-ironicclient-5.6.0/releasenotes/notes/no-osc-requirement-411f25fd10f18caa.yaml`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.5.0/releasenotes/notes/node-driver-support-storage-interface-e93fc8d4de5d24d6.yaml` & `python-ironicclient-5.6.0/releasenotes/notes/node-driver-support-storage-interface-e93fc8d4de5d24d6.yaml`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.5.0/releasenotes/notes/osc-baremetal-node-bios-setting-list-b062b31d0d4de337.yaml` & `python-ironicclient-5.6.0/releasenotes/notes/osc-baremetal-node-bios-setting-list-b062b31d0d4de337.yaml`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.5.0/releasenotes/notes/osc-commands-1-7-d531960472a11ac2.yaml` & `python-ironicclient-5.6.0/releasenotes/notes/osc-commands-1-7-d531960472a11ac2.yaml`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.5.0/releasenotes/notes/osc-plugin-f87e0fbb472261dd.yaml` & `python-ironicclient-5.6.0/releasenotes/notes/osc-plugin-f87e0fbb472261dd.yaml`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.5.0/releasenotes/notes/osc-plugin-ff0d897d8441a9e1.yaml` & `python-ironicclient-5.6.0/releasenotes/notes/osc-plugin-ff0d897d8441a9e1.yaml`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.5.0/releasenotes/notes/osc-port-set-llc-pxeenabled-21fd8ea1982af17e.yaml` & `python-ironicclient-5.6.0/releasenotes/notes/osc-port-set-llc-pxeenabled-21fd8ea1982af17e.yaml`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.5.0/releasenotes/notes/prelude-2-0-release-ee44150902d3d399.yaml` & `python-ironicclient-5.6.0/releasenotes/notes/prelude-2-0-release-ee44150902d3d399.yaml`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.5.0/releasenotes/notes/remove-deprecated-osc-cmd-6dc980299d2fbde4.yaml` & `python-ironicclient-5.6.0/releasenotes/notes/remove-deprecated-osc-cmd-6dc980299d2fbde4.yaml`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.5.0/releasenotes/notes/support-passing-global-request-id-4b96beb31ec906cb.yaml` & `python-ironicclient-5.6.0/releasenotes/notes/support-passing-global-request-id-4b96beb31ec906cb.yaml`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.5.0/releasenotes/notes/traits-support-8864f6816abecdb2.yaml` & `python-ironicclient-5.6.0/releasenotes/notes/traits-support-8864f6816abecdb2.yaml`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.5.0/releasenotes/source/conf.py` & `python-ironicclient-5.6.0/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.5.0/setup.cfg` & `python-ironicclient-5.6.0/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -87,14 +87,15 @@
 	baremetal_node_provide = ironicclient.osc.v1.baremetal_node:ProvideBaremetalNode
 	baremetal_node_reboot = ironicclient.osc.v1.baremetal_node:RebootBaremetalNode
 	baremetal_node_rebuild = ironicclient.osc.v1.baremetal_node:RebuildBaremetalNode
 	baremetal_node_remove_trait = ironicclient.osc.v1.baremetal_node:RemoveTraitBaremetalNode
 	baremetal_node_rescue = ironicclient.osc.v1.baremetal_node:RescueBaremetalNode
 	baremetal_node_secure_boot_on = ironicclient.osc.v1.baremetal_node:SecurebootOnBaremetalNode
 	baremetal_node_secure_boot_off = ironicclient.osc.v1.baremetal_node:SecurebootOffBaremetalNode
+	baremetal_node_service = ironicclient.osc.v1.baremetal_node:ServiceBaremetalNode
 	baremetal_node_set = ironicclient.osc.v1.baremetal_node:SetBaremetalNode
 	baremetal_node_show = ironicclient.osc.v1.baremetal_node:ShowBaremetalNode
 	baremetal_node_trait_list = ironicclient.osc.v1.baremetal_node:ListTraitsBaremetalNode
 	baremetal_node_undeploy = ironicclient.osc.v1.baremetal_node:UndeployBaremetalNode
 	baremetal_node_unhold = ironicclient.osc.v1.baremetal_node:UnholdBaremetalNode
 	baremetal_node_unrescue = ironicclient.osc.v1.baremetal_node:UnrescueBaremetalNode
 	baremetal_node_unset = ironicclient.osc.v1.baremetal_node:UnsetBaremetalNode
```

### Comparing `python-ironicclient-5.5.0/setup.py` & `python-ironicclient-5.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.5.0/tools/install_venv_common.py` & `python-ironicclient-5.6.0/tools/install_venv_common.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.5.0/tox.ini` & `python-ironicclient-5.6.0/tox.ini`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.5.0/zuul.d/ironicclient-jobs.yaml` & `python-ironicclient-5.6.0/zuul.d/ironicclient-jobs.yaml`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.5.0/zuul.d/project.yaml` & `python-ironicclient-5.6.0/zuul.d/project.yaml`

 * *Files identical despite different names*

