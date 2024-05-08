# Comparing `tmp/datamaxi-0.1.0.tar.gz` & `tmp/datamaxi-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datamaxi-0.1.0.tar", last modified: Mon Apr 15 12:54:00 2024, max compression
+gzip compressed data, was "datamaxi-0.2.0.tar", last modified: Wed May  8 07:44:30 2024, max compression
```

## Comparing `datamaxi-0.1.0.tar` & `datamaxi-0.2.0.tar`

### file list

```diff
@@ -1,33 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:54:00.712904 datamaxi-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-15 12:53:56.000000 datamaxi-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-15 12:53:56.000000 datamaxi-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4634 2024-04-15 12:54:00.712904 datamaxi-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3847 2024-04-15 12:53:56.000000 datamaxi-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:54:00.708904 datamaxi-0.1.0/datamaxi/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 12:53:56.000000 datamaxi-0.1.0/datamaxi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-15 12:53:56.000000 datamaxi-0.1.0/datamaxi/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4549 2024-04-15 12:53:56.000000 datamaxi-0.1.0/datamaxi/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:54:00.712904 datamaxi-0.1.0/datamaxi/binance/
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-04-15 12:53:56.000000 datamaxi-0.1.0/datamaxi/binance/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:54:00.712904 datamaxi-0.1.0/datamaxi/defillama/
--rw-r--r--   0 runner    (1001) docker     (127)    15894 2024-04-15 12:53:56.000000 datamaxi-0.1.0/datamaxi/defillama/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-15 12:53:56.000000 datamaxi-0.1.0/datamaxi/error.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:54:00.712904 datamaxi-0.1.0/datamaxi/google/
--rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-04-15 12:53:56.000000 datamaxi-0.1.0/datamaxi/google/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:54:00.712904 datamaxi-0.1.0/datamaxi/lib/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-15 12:53:56.000000 datamaxi-0.1.0/datamaxi/lib/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-04-15 12:53:56.000000 datamaxi-0.1.0/datamaxi/lib/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:54:00.712904 datamaxi-0.1.0/datamaxi/naver/
--rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-04-15 12:53:56.000000 datamaxi-0.1.0/datamaxi/naver/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:54:00.712904 datamaxi-0.1.0/datamaxi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4634 2024-04-15 12:54:00.000000 datamaxi-0.1.0/datamaxi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-15 12:54:00.000000 datamaxi-0.1.0/datamaxi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 12:54:00.000000 datamaxi-0.1.0/datamaxi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-15 12:54:00.000000 datamaxi-0.1.0/datamaxi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-15 12:54:00.000000 datamaxi-0.1.0/datamaxi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-15 12:53:56.000000 datamaxi-0.1.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:54:00.712904 datamaxi-0.1.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-15 12:53:56.000000 datamaxi-0.1.0/requirements/common.txt
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-15 12:54:00.712904 datamaxi-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:54:00.712904 datamaxi-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-04-15 12:53:56.000000 datamaxi-0.1.0/tests/test_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:44:30.348146 datamaxi-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-08 07:44:24.000000 datamaxi-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-08 07:44:24.000000 datamaxi-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5171 2024-05-08 07:44:30.348146 datamaxi-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4384 2024-05-08 07:44:24.000000 datamaxi-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:44:30.344146 datamaxi-0.2.0/datamaxi/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 07:44:24.000000 datamaxi-0.2.0/datamaxi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-08 07:44:24.000000 datamaxi-0.2.0/datamaxi/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4548 2024-05-08 07:44:24.000000 datamaxi-0.2.0/datamaxi/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:44:30.344146 datamaxi-0.2.0/datamaxi/binance/
+-rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-05-08 07:44:24.000000 datamaxi-0.2.0/datamaxi/binance/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:44:30.344146 datamaxi-0.2.0/datamaxi/bithumb/
+-rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-05-08 07:44:24.000000 datamaxi-0.2.0/datamaxi/bithumb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:44:30.344146 datamaxi-0.2.0/datamaxi/bybit/
+-rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-05-08 07:44:24.000000 datamaxi-0.2.0/datamaxi/bybit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:44:30.344146 datamaxi-0.2.0/datamaxi/coinone/
+-rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-05-08 07:44:24.000000 datamaxi-0.2.0/datamaxi/coinone/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:44:30.344146 datamaxi-0.2.0/datamaxi/defillama/
+-rw-r--r--   0 runner    (1001) docker     (127)    15894 2024-05-08 07:44:24.000000 datamaxi-0.2.0/datamaxi/defillama/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-05-08 07:44:24.000000 datamaxi-0.2.0/datamaxi/error.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:44:30.344146 datamaxi-0.2.0/datamaxi/google/
+-rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-05-08 07:44:24.000000 datamaxi-0.2.0/datamaxi/google/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:44:30.344146 datamaxi-0.2.0/datamaxi/huobi/
+-rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-05-08 07:44:24.000000 datamaxi-0.2.0/datamaxi/huobi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:44:30.344146 datamaxi-0.2.0/datamaxi/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-08 07:44:24.000000 datamaxi-0.2.0/datamaxi/lib/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-05-08 07:44:24.000000 datamaxi-0.2.0/datamaxi/lib/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:44:30.344146 datamaxi-0.2.0/datamaxi/naver/
+-rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-05-08 07:44:24.000000 datamaxi-0.2.0/datamaxi/naver/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:44:30.344146 datamaxi-0.2.0/datamaxi/okx/
+-rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-05-08 07:44:24.000000 datamaxi-0.2.0/datamaxi/okx/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:44:30.344146 datamaxi-0.2.0/datamaxi/upbit/
+-rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-05-08 07:44:24.000000 datamaxi-0.2.0/datamaxi/upbit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:44:30.348146 datamaxi-0.2.0/datamaxi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5171 2024-05-08 07:44:30.000000 datamaxi-0.2.0/datamaxi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-08 07:44:30.000000 datamaxi-0.2.0/datamaxi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 07:44:30.000000 datamaxi-0.2.0/datamaxi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-08 07:44:30.000000 datamaxi-0.2.0/datamaxi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-08 07:44:30.000000 datamaxi-0.2.0/datamaxi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-08 07:44:24.000000 datamaxi-0.2.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:44:30.344146 datamaxi-0.2.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-08 07:44:24.000000 datamaxi-0.2.0/requirements/common.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-08 07:44:30.348146 datamaxi-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:44:30.348146 datamaxi-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-05-08 07:44:24.000000 datamaxi-0.2.0/tests/test_api.py
```

### Comparing `datamaxi-0.1.0/LICENSE` & `datamaxi-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `datamaxi-0.1.0/PKG-INFO` & `datamaxi-0.2.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datamaxi
-Version: 0.1.0
+Version: 0.2.0
 Summary: Official Python client for DataMaxi+ API
 Author-email: Bisonai <business@bisonai.com>
 Project-URL: Homepage, https://github.com/bisonai/datamaxi-python
 Project-URL: Issues, https://github.com/bisonai/datamaxi-python/issues
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: License :: OSI Approved :: MIT License
@@ -15,111 +15,140 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests>=2.31.0
 Requires-Dist: pandas
 
 # DataMaxi+ Python Client
+
 [![PyPI version](https://img.shields.io/pypi/v/datamaxi)](https://pypi.python.org/pypi/datamaxi)
 [![Python version](https://img.shields.io/pypi/pyversions/datamaxi)](https://www.python.org/downloads/)
 [![Documentation](https://img.shields.io/badge/docs-latest-blue)](https://datamaxi.readthedocs.io/en/stable/)
 [![Code Style](https://img.shields.io/badge/code_style-black-black)](https://black.readthedocs.io/en/stable/)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 This is the official implementation of Python client for DataMaxi+ API.
-The package can be used to fetch both historical and latest data using [DataMaxi+ API](https://docs.neverest.finance/).
+The package can be used to fetch both historical and latest data using [DataMaxi+ API](https://docs.datamaxiplus.com/).
 This package is compatible with Python v3.8+.
 
-* [Installation](#installation)
-* [Configuration](#configuration)
-  * [Environment Variables](#environment-variables)
-* [Quickstart](#quickstart)
-* [Local Development](#local-development)
-  * [Setup](#setup)
-  * [Testing](#testing)
-* [Links](#links)
-* [Contributing](#contributing)
-* [License](#license)
+- [Installation](#installation)
+- [Configuration](#configuration)
+  - [Environment Variables](#environment-variables)
+- [Quickstart](#quickstart)
+- [Local Development](#local-development)
+  - [Setup](#setup)
+  - [Testing](#testing)
+- [Links](#links)
+- [Contributing](#contributing)
+- [License](#license)
 
 ## Installation
 
 ```shell
-pip install datamaxi
+pip3 install datamaxi
 ```
 
 ## Configuration
 
 Access to DataMaxi+ is protected by API Key.
-If you are interested to try DataMaxi+, you can request your API key at [business@bisonai.com](mailto:business@bisonai.com).
+If you are interested to try DataMaxi+, you can simply sign up for DataMaxi+ through [this login/singup page](https://datamaxiplus.com/auth) and get free API key for two months.
 
 | Option             | Explanation                                                                           |
-|--------------------|---------------------------------------------------------------------------------------|
+| ------------------ | ------------------------------------------------------------------------------------- |
 | `api_key`          | Your API key                                                                          |
-| `base_url`         | If `base_url` is not provided, it defaults to `api.neverest.finance`.                 |
+| `base_url`         | If `base_url` is not provided, it defaults to `api.datamaxiplus.com`.                 |
 | `timeout`          | Number of seconds to wait for a server response. By default requests do not time out. |
 | `proxies`          | Proxy through which the request is queried                                            |
-| `show_limit_usage` | Return response as dictionary including including `"limit_usage"` and `"data"` keys   |
-| `show_header`      | Return response as dictionary including including `"header"` and `"data"` keys        |
+| `show_limit_usage` | Return response as dictionary including `"limit_usage"` and `"data"` keys   |
+| `show_header`      | Return response as dictionary including `"header"` and `"data"` keys        |
 
 ### Environment Variables
 
 You may use environment variables to configure the DataMaxi+ client to avoid any inline boilerplate.
 
 | Env                | Description                                  |
-|--------------------|----------------------------------------------|
-| `NEVEREST_API_KEY` | Used instead of `api_key` if none is passed. |
+| ------------------ | -------------------------------------------- |
+| `DATAMAXI_API_KEY` | Used instead of `api_key` if none is passed. |
 
 ## Quickstart
 
 DataMaxi+ Python package currently includes the following clients:
 
-* `Binance`
-* `Defillama`
-* `Naver`
-* `Google`
+- `Binance`
+- `Bithumb`
+- `Bybit`
+- `Coinone`
+- `Huobi`
+- `Okx`
+- `Upbit`
+- `Defillama`
+- `Naver`
+- `Google`
 
 All clients accept the same parameters that are described at [Configuration](#configuration) section.
 First, import the clients,
 
 ```python
+# CEX
 from datamaxi.binance import Binance
+from datamaxi.bithumb import Bithumb
+from datamaxi.bybit import Bybit
+from datamaxi.coinone import Coinone
+from datamaxi.huobi import Huobi
+from datamaxi.okx import Okx
+from datamaxi.upbit import Upbit
+
+# DeFi
 from datamaxi.defillama import Defillama
+
+# Trend
 from datamaxi.naver import Naver
 from datamaxi.google import Google
 ```
 
 and initialize them.
 
 ```python
+# CEX
 binance = Binance(api_key=api_key)
+bithumb = Bithumb(api_key=api_key)
+bybit = Bybit(api_key=api_key)
+coinone = Coinone(api_key=api_key)
+huobi = Huobi(api_key=api_key)
+okx = Okx(api_key=api_key)
+upbit = Upbit(api_key=api_key)
+
+# DeFi
 defillama = Defillama(api_key=api_key)
+
+# Trend
 naver = Naver(api_key=api_key)
 google = Google(api_key=api_key)
 ```
 
 ## Local Development
 
 ### Setup
 
 If you wish to work on local development please clone/fork the git repo and use `pip install -r requirements.txt` to setup the project.
 
 ### Testing
 
 ```shell
 # In case packages are not installed yet
-pip install -r requirements/requirements-test.txt
+pip3 install -r requirements/requirements-test.txt
 
-python -m pytest tests/
+python3 -m pytest tests/
 ```
 
 ## Links
 
-* [DataMaxi+](https://datamaxiplus.com/)
-* [DataMaxi+ API](https://api.neverest.finance/)
-* [DataMaxi+ API Documentation](https://docs.neverest.finance/)
+- [DataMaxi+](https://datamaxiplus.com/)
+- [DataMaxi+ API](https://api.datamaxiplus.com/)
+- [DataMaxi+ API Documentation](https://docs.datamaxiplus.com/)
 
 ## Contributing
 
 We welcome contributions!
 If you discover a bug in this project, please feel free to open an issue to discuss the changes you would like to propose.
 
 ## License
```

### Comparing `datamaxi-0.1.0/README.md` & `datamaxi-0.2.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,105 +1,134 @@
 # DataMaxi+ Python Client
+
 [![PyPI version](https://img.shields.io/pypi/v/datamaxi)](https://pypi.python.org/pypi/datamaxi)
 [![Python version](https://img.shields.io/pypi/pyversions/datamaxi)](https://www.python.org/downloads/)
 [![Documentation](https://img.shields.io/badge/docs-latest-blue)](https://datamaxi.readthedocs.io/en/stable/)
 [![Code Style](https://img.shields.io/badge/code_style-black-black)](https://black.readthedocs.io/en/stable/)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 This is the official implementation of Python client for DataMaxi+ API.
-The package can be used to fetch both historical and latest data using [DataMaxi+ API](https://docs.neverest.finance/).
+The package can be used to fetch both historical and latest data using [DataMaxi+ API](https://docs.datamaxiplus.com/).
 This package is compatible with Python v3.8+.
 
-* [Installation](#installation)
-* [Configuration](#configuration)
-  * [Environment Variables](#environment-variables)
-* [Quickstart](#quickstart)
-* [Local Development](#local-development)
-  * [Setup](#setup)
-  * [Testing](#testing)
-* [Links](#links)
-* [Contributing](#contributing)
-* [License](#license)
+- [Installation](#installation)
+- [Configuration](#configuration)
+  - [Environment Variables](#environment-variables)
+- [Quickstart](#quickstart)
+- [Local Development](#local-development)
+  - [Setup](#setup)
+  - [Testing](#testing)
+- [Links](#links)
+- [Contributing](#contributing)
+- [License](#license)
 
 ## Installation
 
 ```shell
-pip install datamaxi
+pip3 install datamaxi
 ```
 
 ## Configuration
 
 Access to DataMaxi+ is protected by API Key.
-If you are interested to try DataMaxi+, you can request your API key at [business@bisonai.com](mailto:business@bisonai.com).
+If you are interested to try DataMaxi+, you can simply sign up for DataMaxi+ through [this login/singup page](https://datamaxiplus.com/auth) and get free API key for two months.
 
 | Option             | Explanation                                                                           |
-|--------------------|---------------------------------------------------------------------------------------|
+| ------------------ | ------------------------------------------------------------------------------------- |
 | `api_key`          | Your API key                                                                          |
-| `base_url`         | If `base_url` is not provided, it defaults to `api.neverest.finance`.                 |
+| `base_url`         | If `base_url` is not provided, it defaults to `api.datamaxiplus.com`.                 |
 | `timeout`          | Number of seconds to wait for a server response. By default requests do not time out. |
 | `proxies`          | Proxy through which the request is queried                                            |
-| `show_limit_usage` | Return response as dictionary including including `"limit_usage"` and `"data"` keys   |
-| `show_header`      | Return response as dictionary including including `"header"` and `"data"` keys        |
+| `show_limit_usage` | Return response as dictionary including `"limit_usage"` and `"data"` keys   |
+| `show_header`      | Return response as dictionary including `"header"` and `"data"` keys        |
 
 ### Environment Variables
 
 You may use environment variables to configure the DataMaxi+ client to avoid any inline boilerplate.
 
 | Env                | Description                                  |
-|--------------------|----------------------------------------------|
-| `NEVEREST_API_KEY` | Used instead of `api_key` if none is passed. |
+| ------------------ | -------------------------------------------- |
+| `DATAMAXI_API_KEY` | Used instead of `api_key` if none is passed. |
 
 ## Quickstart
 
 DataMaxi+ Python package currently includes the following clients:
 
-* `Binance`
-* `Defillama`
-* `Naver`
-* `Google`
+- `Binance`
+- `Bithumb`
+- `Bybit`
+- `Coinone`
+- `Huobi`
+- `Okx`
+- `Upbit`
+- `Defillama`
+- `Naver`
+- `Google`
 
 All clients accept the same parameters that are described at [Configuration](#configuration) section.
 First, import the clients,
 
 ```python
+# CEX
 from datamaxi.binance import Binance
+from datamaxi.bithumb import Bithumb
+from datamaxi.bybit import Bybit
+from datamaxi.coinone import Coinone
+from datamaxi.huobi import Huobi
+from datamaxi.okx import Okx
+from datamaxi.upbit import Upbit
+
+# DeFi
 from datamaxi.defillama import Defillama
+
+# Trend
 from datamaxi.naver import Naver
 from datamaxi.google import Google
 ```
 
 and initialize them.
 
 ```python
+# CEX
 binance = Binance(api_key=api_key)
+bithumb = Bithumb(api_key=api_key)
+bybit = Bybit(api_key=api_key)
+coinone = Coinone(api_key=api_key)
+huobi = Huobi(api_key=api_key)
+okx = Okx(api_key=api_key)
+upbit = Upbit(api_key=api_key)
+
+# DeFi
 defillama = Defillama(api_key=api_key)
+
+# Trend
 naver = Naver(api_key=api_key)
 google = Google(api_key=api_key)
 ```
 
 ## Local Development
 
 ### Setup
 
 If you wish to work on local development please clone/fork the git repo and use `pip install -r requirements.txt` to setup the project.
 
 ### Testing
 
 ```shell
 # In case packages are not installed yet
-pip install -r requirements/requirements-test.txt
+pip3 install -r requirements/requirements-test.txt
 
-python -m pytest tests/
+python3 -m pytest tests/
 ```
 
 ## Links
 
-* [DataMaxi+](https://datamaxiplus.com/)
-* [DataMaxi+ API](https://api.neverest.finance/)
-* [DataMaxi+ API Documentation](https://docs.neverest.finance/)
+- [DataMaxi+](https://datamaxiplus.com/)
+- [DataMaxi+ API](https://api.datamaxiplus.com/)
+- [DataMaxi+ API Documentation](https://docs.datamaxiplus.com/)
 
 ## Contributing
 
 We welcome contributions!
 If you discover a bug in this project, please feel free to open an issue to discuss the changes you would like to propose.
 
 ## License
```

### Comparing `datamaxi-0.1.0/datamaxi/api.py` & `datamaxi-0.2.0/datamaxi/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,50 +7,50 @@
 from datamaxi.error import ClientError, ServerError
 from datamaxi.lib.utils import cleanNoneValue
 from datamaxi.lib.utils import encoded_string
 
 
 class API(object):
     """The base class for all DataMaxi+ Python clients. `api_key` can be set
-    as an environment variable `NEVEREST_API_KEY`.
+    as an environment variable `DATAMAXI_API_KEY`.
     """
 
     def __init__(
         self,
         api_key=None,
         base_url=None,
         timeout=None,
         proxies=None,
         show_limit_usage=False,
         show_header=False,
     ):
         """Client API constructor. `api_key` can be set
-        as an environment variable `NEVEREST_API_KEY`.
+        as an environment variable `DATAMAXI_API_KEY`.
 
         Args:
             api_key (str): The API key for the DataMaxi+ API.
             base_url (str): The base URL for the DataMaxi+ API.
             timeout (int): The timeout for the requests.
             proxies (dict): The proxies for the requests.
             show_limit_usage (bool): Show the limit usage.
             show_header (bool): Show the header.
         """
-        self.api_key = api_key or os.environ.get("NEVEREST_API_KEY")
+        self.api_key = api_key or os.environ.get("DATAMAXI_API_KEY")
         self.base_url = base_url
         self.timeout = timeout
         self.proxies = None
         self.show_limit_usage = False
         self.show_header = False
 
         self.session = requests.Session()
         self.session.headers.update(
             {
                 "Content-Type": "application/json;charset=utf-8",
                 "User-Agent": "datamaxi/" + __version__,
-                "Authorization": "X-NVRST-APIKEY " + str(self.api_key),
+                "Authorization": "X-DTMX-APIKEY " + str(self.api_key),
             }
         )
 
         if show_limit_usage is True:
             self.show_limit_usage = True
 
         if show_header is True:
```

### Comparing `datamaxi-0.1.0/datamaxi/binance/__init__.py` & `datamaxi-0.2.0/datamaxi/binance/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,43 +14,57 @@
 
         Args:
             api_key (str): The DataMaxi+ API key
             **kwargs: Keyword arguments used by `datamaxi.api.API`.
         """
         if "base_url" not in kwargs:
             kwargs["base_url"] = BASE_URL
-            super().__init__(api_key, **kwargs)
+
+        super().__init__(api_key, **kwargs)
 
     def symbols(self) -> List[str]:
         """Supported Binance supported symbols
 
         `GET /v1/raw/binance/symbols`
 
-        <https://docs.neverest.finance/cex/binance/symbols>
+        <https://docs.datamaxiplus.com/cex/binance/symbols>
 
         Returns:
             List of supported Binance symbols
         """
         url_path = "/v1/raw/binance/symbols"
         return self.query(url_path)
 
+    def intervals(self) -> List[str]:
+        """Supported Binance supported intervals
+
+        `GET /v1/raw/binance/intervals`
+
+        <https://docs.datamaxiplus.com/cex/binance/intervals>
+
+        Returns:
+            List of supported Binance intervals
+        """
+        url_path = "/v1/raw/binance/intervals"
+        return self.query(url_path)
+
     @postprocess()
-    def kline(
+    def candle(
         self, symbol: str, interval: str = "1d", pandas: bool = True
     ) -> Union[List, pd.DataFrame]:
-        """Get Binance k-line data
+        """Get Binance candle data
 
-        `GET /v1/raw/binance/kline`
+        `GET /v1/raw/binance/candle`
 
-        <https://docs.neverest.finance/cex/binance/kline>
+        <https://docs.datamaxiplus.com/cex/binance/candle>
 
         Args:
             symbol (str): Binance symbol
-            interval (str): Kline interval
+            interval (str): Candle interval
             pandas (bool): Return data as pandas DataFrame
 
         Returns:
-            Binance kline data for a given symbol and interval in pandas DataFrame
+            Binance candle data for a given symbol and interval in pandas DataFrame
         """
         check_required_parameters([[symbol, "symbol"], [interval, "interval"]])
         params = {"symbol": symbol, "interval": interval}
-        return self.query("/v1/raw/binance/kline", params)
+        return self.query("/v1/raw/binance/candle", params)
```

### Comparing `datamaxi-0.1.0/datamaxi/defillama/__init__.py` & `datamaxi-0.2.0/datamaxi/defillama/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,81 +25,81 @@
             super().__init__(api_key, **kwargs)
 
     def protocols(self) -> List[str]:
         """Get supported protocols
 
         `GET /v1/defillama/protocol`
 
-        <https://docs.neverest.finance/defillama/protocol>
+        <https://docs.datamaxiplus.com/defillama/protocol>
 
         Returns:
             List of supported protocols
         """
         url_path = "/v1/defillama/protocol"
         return self.query(url_path)
 
     def chains(self) -> List[str]:
         """Get supported chains
 
         `GET /v1/defillama/chain`
 
-        <https://docs.neverest.finance/defillama/chain>
+        <https://docs.datamaxiplus.com/defillama/chain>
 
         Returns:
             List of supported chains
         """
         url_path = "/v1/defillama/chain"
         return self.query(url_path)
 
     def tokens(self) -> List[str]:
         """Get supported tokens
 
         `GET /v1/defillama/token`
 
-        <https://docs.neverest.finance/defillama/token>
+        <https://docs.datamaxiplus.com/defillama/token>
 
         Returns:
             List of supported tokens
         """
         url_path = "/v1/defillama/token"
         return self.query(url_path)
 
     def pools(self) -> List[str]:
         """Get supported pools
 
         `GET /v1/defillama/pool`
 
-        <https://docs.neverest.finance/defillama/pool>
+        <https://docs.datamaxiplus.com/defillama/pool>
 
         Returns:
             List of supported pools
         """
         url_path = "/v1/defillama/pool"
         return self.query(url_path)
 
     def stablecoins(self) -> List[str]:
         """Get supported stablecoins
 
         `GET /v1/defillama/stablecoin`
 
-        <https://docs.neverest.finance/defillama/stablecoin>
+        <https://docs.datamaxiplus.com/defillama/stablecoin>
 
         Returns:
             List of supported stablecoins
         """
         url_path = "/v1/defillama/stablecoin"
         return self.query(url_path)
 
     @postprocess()
     def tvl(self, pandas: bool = True) -> Union[List, pd.DataFrame]:
         """Get total TVL across all chains and protocols
 
         `GET /v1/defillama/tvl`
 
-        <https://docs.neverest.finance/defillama/tvl>
+        <https://docs.datamaxiplus.com/defillama/tvl>
 
         Args:
             pandas (bool): Return data as pandas DataFrame
 
         Returns:
             Timeseries of total TVL
         """
@@ -110,15 +110,15 @@
     def protocol_tvl(
         self, protocols: Union[str, List[str]] = None, pandas: bool = True
     ) -> Union[List, pd.DataFrame]:
         """Get TVL for given protocols
 
         `GET /v1/defillama/tvl`
 
-        <https://docs.neverest.finance/defillama/tvl>
+        <https://docs.datamaxiplus.com/defillama/tvl>
 
         Args:
             protocols (Union[str, List[str]]): single protocol or multiple protocol names
             pandas (bool): Return data as pandas DataFrame
 
         Returns:
             Timeseries of protocol TVLs
@@ -132,15 +132,15 @@
     def chain_tvl(
         self, chains: Union[str, List[str]] = None, pandas: bool = True
     ) -> Union[List, pd.DataFrame]:
         """Get TVL for given chains
 
         `GET /v1/defillama/tvl`
 
-        <https://docs.neverest.finance/defillama/tvl>
+        <https://docs.datamaxiplus.com/defillama/tvl>
 
         Args:
             chains (Union[str, List[str]]): single chain or multiple chain names
             pandas (bool): Return data as pandas DataFrame
 
         Returns:
             Timeseries of chain TVLs
@@ -154,15 +154,15 @@
     def protocol_chain_tvl(
         self, protocol: str, chain: str, pandas: bool = True
     ) -> Union[List, pd.DataFrame]:
         """Get TVL for given protocol and chain
 
         `GET /v1/defillama/tvl`
 
-        <https://docs.neverest.finance/defillama/tvl>
+        <https://docs.datamaxiplus.com/defillama/tvl>
 
         Args:
             protocol (str): protocol name
             chain (str): chain name
             pandas (bool): Return data as pandas DataFrame
 
         Returns:
@@ -176,15 +176,15 @@
     def protocol_token_tvl(
         self, protocol: str, usd: bool = True, pandas: bool = True
     ) -> Union[List, pd.DataFrame]:
         """Get token TVL on a given protocol
 
         `GET /v1/defillama/tvl`
 
-        <https://docs.neverest.finance/defillama/tvl>
+        <https://docs.datamaxiplus.com/defillama/tvl>
 
         Args:
             protocol (str): protocol name
             usd (bool): Convert to USD otherwise return token amount
             pandas (bool): Return data as pandas DataFrame
 
         Returns:
@@ -202,15 +202,15 @@
     def protocol_chain_token_tvl(
         self, protocol: str, chain: str, usd: bool = True, pandas: bool = True
     ) -> Union[List, pd.DataFrame]:
         """Get token TVL on a given protocol and chain
 
         `GET /v1/defillama/tvl`
 
-        <https://docs.neverest.finance/defillama/tvl>
+        <https://docs.datamaxiplus.com/defillama/tvl>
 
         Args:
             protocol (str): protocol name
             chain (str): chain name
             usd (bool): Convert to USD otherwise return token amount
             pandas (bool): Return data as pandas DataFrame
 
@@ -232,15 +232,15 @@
     def protocol_mcap(
         self, protocols: Union[str, List[str]] = None, pandas: bool = True
     ) -> Union[List, pd.DataFrame]:
         """Get market cap for given protocols
 
         `GET /v1/defillama/mcap`
 
-        <https://docs.neverest.finance/defillama/mcap>
+        <https://docs.datamaxiplus.com/defillama/mcap>
 
         Args:
             protocols (Union[str, List[str]]): single protocol or multiple protocol names
             pandas (bool): Return data as pandas DataFrame
 
         Returns:
             Timeseries of market cap for given protocols
@@ -256,15 +256,15 @@
     def token_price(
         self, addresses: Union[str, List[str]] = None, pandas: bool = True
     ) -> Union[List, pd.DataFrame]:
         """Get token prices
 
         `GET /v1/defillama/token`
 
-        <https://docs.neverest.finance/defillama/token-price>
+        <https://docs.datamaxiplus.com/defillama/token-price>
 
         Args:
             addresses (Union[str, List[str]]): single address or multiple addresses
             pandas (bool): Return data as pandas DataFrame
 
         Returns:
             Timeseries of token prices
@@ -288,15 +288,15 @@
     def stablecoin_mcap(
         self, stablecoin: str = None, pandas: bool = True
     ) -> Union[List, pd.DataFrame]:
         """Get market cap for given stablecoin
 
         `GET /v1/defillama/stablecoin`
 
-        <https://docs.neverest.finance/defillama/stablecoin-mcap>
+        <https://docs.datamaxiplus.com/defillama/stablecoin-mcap>
 
         Args:
             stablecoin (str): stablecoin name
             pandas (bool): Return data as pandas DataFrame
 
         Returns:
             Timeseries of market cap for given stablecoin
@@ -311,15 +311,15 @@
     def stablecoin_chain_mcap(
         self, stablecoin: str, chain: str, pandas: bool = True
     ) -> Union[List, pd.DataFrame]:
         """Get market cap for a given stablecoin on a specific chain
 
         `GET /v1/defillama/stablecoin`
 
-        <https://docs.neverest.finance/defillama/stablecoin-mcap>
+        <https://docs.datamaxiplus.com/defillama/stablecoin-mcap>
 
         Args:
             stablecoin (str): stablecoin name
             chain (str): chain name
             pandas (bool): Return data as pandas DataFrame
 
         Returns:
@@ -336,15 +336,15 @@
     def stablecoin_price(
         self, stablecoins: Union[str, List[str]] = None, pandas: bool = True
     ) -> Union[List, pd.DataFrame]:
         """Get price for given stablecoins
 
         `GET /v1/defillama/stablecoin/price`
 
-        <https://docs.neverest.finance/defillama/stablecoin-price>
+        <https://docs.datamaxiplus.com/defillama/stablecoin-price>
 
         Args:
             stablecoins (Union[str, List[str]]): single stablecoin or multiple stablecoin names
             pandas (bool): Return data as pandas DataFrame
 
         Returns:
             Timeseries of stablecoin prices
@@ -364,15 +364,15 @@
         daily: bool = True,
         pandas: bool = True,
     ) -> Union[List, pd.DataFrame]:
         """Get fee for given protocols or chains
 
         `GET /v1/defillama/fee`
 
-        <https://docs.neverest.finance/defillama/fee>
+        <https://docs.datamaxiplus.com/defillama/fee>
 
         Args:
             protocols (Union[str, List[str]]): single protocol or multiple protocol names
             chains (Union[str, List[str]]): single chain or multiple chain names
             daily (bool): daily fee or total fee
             pandas (bool): Return data as pandas DataFrame
 
@@ -406,15 +406,15 @@
         daily: bool = True,
         pandas: bool = True,
     ) -> Union[List, pd.DataFrame]:
         """Get revenue for given protocols or chains
 
         `GET /v1/defillama/revenue`
 
-        <https://docs.neverest.finance/defillama/revenue>
+        <https://docs.datamaxiplus.com/defillama/revenue>
 
         Args:
             protocols (Union[str, List[str]]): single protocol or multiple protocol names
             chains (Union[str, List[str]]): single chain or multiple chain names
             daily (bool): daily revenue or total revenue
             pandas (bool): Return data as pandas DataFrame
 
@@ -444,15 +444,15 @@
     def fee_detail(
         self, protocol: str, chain: str = None, daily: bool = True, pandas: bool = True
     ) -> Union[List, pd.DataFrame]:
         """Get fee detail for given protocol and chain
 
         `GET /v1/defillama/fee/detail`
 
-        <https://docs.neverest.finance/defillama/fee-detail>
+        <https://docs.datamaxiplus.com/defillama/fee-detail>
 
         Args:
             protocol (str): protocol name
             chain (str): chain name (optional)
             daily (bool): daily fee or total fee
             pandas (bool): Return data as pandas DataFrame
 
@@ -473,15 +473,15 @@
     def revenue_detail(
         self, protocol: str, chain: str = None, daily: bool = True, pandas: bool = True
     ) -> Union[List, pd.DataFrame]:
         """Get revenue detail for given protocol and chain
 
         `GET /v1/defillama/revenue/detail`
 
-        <https://docs.neverest.finance/defillama/revenue-detail>
+        <https://docs.datamaxiplus.com/defillama/revenue-detail>
 
         Args:
             protocol (str): protocol name
             chain (str): chain name (optional)
             daily (bool): daily revenue or total revenue
             pandas (bool): Return data as pandas DataFrame
```

### Comparing `datamaxi-0.1.0/datamaxi/error.py` & `datamaxi-0.2.0/datamaxi/error.py`

 * *Files identical despite different names*

### Comparing `datamaxi-0.1.0/datamaxi/google/__init__.py` & `datamaxi-0.2.0/datamaxi/google/__init__.py`

 * *Files identical despite different names*

### Comparing `datamaxi-0.1.0/datamaxi/lib/utils.py` & `datamaxi-0.2.0/datamaxi/lib/utils.py`

 * *Files identical despite different names*

### Comparing `datamaxi-0.1.0/datamaxi/naver/__init__.py` & `datamaxi-0.2.0/datamaxi/naver/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
     @postprocess()
     def trend(self, keyword: str, pandas: bool = True) -> Union[List, pd.DataFrame]:
         """Get Naver trend for given keyword
 
         `GET /v1/naver/trend`
 
-        <https://docs.neverest.finance/naver/trend>
+        <https://docs.datamaxiplus.com/naver/trend>
 
         Args:
             keyword (str): keyword to search for
             pandas (bool): Return data as pandas DataFrame
 
         Returns:
             Naver trend data
```

### Comparing `datamaxi-0.1.0/datamaxi.egg-info/PKG-INFO` & `datamaxi-0.2.0/datamaxi.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datamaxi
-Version: 0.1.0
+Version: 0.2.0
 Summary: Official Python client for DataMaxi+ API
 Author-email: Bisonai <business@bisonai.com>
 Project-URL: Homepage, https://github.com/bisonai/datamaxi-python
 Project-URL: Issues, https://github.com/bisonai/datamaxi-python/issues
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: License :: OSI Approved :: MIT License
@@ -15,111 +15,140 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests>=2.31.0
 Requires-Dist: pandas
 
 # DataMaxi+ Python Client
+
 [![PyPI version](https://img.shields.io/pypi/v/datamaxi)](https://pypi.python.org/pypi/datamaxi)
 [![Python version](https://img.shields.io/pypi/pyversions/datamaxi)](https://www.python.org/downloads/)
 [![Documentation](https://img.shields.io/badge/docs-latest-blue)](https://datamaxi.readthedocs.io/en/stable/)
 [![Code Style](https://img.shields.io/badge/code_style-black-black)](https://black.readthedocs.io/en/stable/)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 This is the official implementation of Python client for DataMaxi+ API.
-The package can be used to fetch both historical and latest data using [DataMaxi+ API](https://docs.neverest.finance/).
+The package can be used to fetch both historical and latest data using [DataMaxi+ API](https://docs.datamaxiplus.com/).
 This package is compatible with Python v3.8+.
 
-* [Installation](#installation)
-* [Configuration](#configuration)
-  * [Environment Variables](#environment-variables)
-* [Quickstart](#quickstart)
-* [Local Development](#local-development)
-  * [Setup](#setup)
-  * [Testing](#testing)
-* [Links](#links)
-* [Contributing](#contributing)
-* [License](#license)
+- [Installation](#installation)
+- [Configuration](#configuration)
+  - [Environment Variables](#environment-variables)
+- [Quickstart](#quickstart)
+- [Local Development](#local-development)
+  - [Setup](#setup)
+  - [Testing](#testing)
+- [Links](#links)
+- [Contributing](#contributing)
+- [License](#license)
 
 ## Installation
 
 ```shell
-pip install datamaxi
+pip3 install datamaxi
 ```
 
 ## Configuration
 
 Access to DataMaxi+ is protected by API Key.
-If you are interested to try DataMaxi+, you can request your API key at [business@bisonai.com](mailto:business@bisonai.com).
+If you are interested to try DataMaxi+, you can simply sign up for DataMaxi+ through [this login/singup page](https://datamaxiplus.com/auth) and get free API key for two months.
 
 | Option             | Explanation                                                                           |
-|--------------------|---------------------------------------------------------------------------------------|
+| ------------------ | ------------------------------------------------------------------------------------- |
 | `api_key`          | Your API key                                                                          |
-| `base_url`         | If `base_url` is not provided, it defaults to `api.neverest.finance`.                 |
+| `base_url`         | If `base_url` is not provided, it defaults to `api.datamaxiplus.com`.                 |
 | `timeout`          | Number of seconds to wait for a server response. By default requests do not time out. |
 | `proxies`          | Proxy through which the request is queried                                            |
-| `show_limit_usage` | Return response as dictionary including including `"limit_usage"` and `"data"` keys   |
-| `show_header`      | Return response as dictionary including including `"header"` and `"data"` keys        |
+| `show_limit_usage` | Return response as dictionary including `"limit_usage"` and `"data"` keys   |
+| `show_header`      | Return response as dictionary including `"header"` and `"data"` keys        |
 
 ### Environment Variables
 
 You may use environment variables to configure the DataMaxi+ client to avoid any inline boilerplate.
 
 | Env                | Description                                  |
-|--------------------|----------------------------------------------|
-| `NEVEREST_API_KEY` | Used instead of `api_key` if none is passed. |
+| ------------------ | -------------------------------------------- |
+| `DATAMAXI_API_KEY` | Used instead of `api_key` if none is passed. |
 
 ## Quickstart
 
 DataMaxi+ Python package currently includes the following clients:
 
-* `Binance`
-* `Defillama`
-* `Naver`
-* `Google`
+- `Binance`
+- `Bithumb`
+- `Bybit`
+- `Coinone`
+- `Huobi`
+- `Okx`
+- `Upbit`
+- `Defillama`
+- `Naver`
+- `Google`
 
 All clients accept the same parameters that are described at [Configuration](#configuration) section.
 First, import the clients,
 
 ```python
+# CEX
 from datamaxi.binance import Binance
+from datamaxi.bithumb import Bithumb
+from datamaxi.bybit import Bybit
+from datamaxi.coinone import Coinone
+from datamaxi.huobi import Huobi
+from datamaxi.okx import Okx
+from datamaxi.upbit import Upbit
+
+# DeFi
 from datamaxi.defillama import Defillama
+
+# Trend
 from datamaxi.naver import Naver
 from datamaxi.google import Google
 ```
 
 and initialize them.
 
 ```python
+# CEX
 binance = Binance(api_key=api_key)
+bithumb = Bithumb(api_key=api_key)
+bybit = Bybit(api_key=api_key)
+coinone = Coinone(api_key=api_key)
+huobi = Huobi(api_key=api_key)
+okx = Okx(api_key=api_key)
+upbit = Upbit(api_key=api_key)
+
+# DeFi
 defillama = Defillama(api_key=api_key)
+
+# Trend
 naver = Naver(api_key=api_key)
 google = Google(api_key=api_key)
 ```
 
 ## Local Development
 
 ### Setup
 
 If you wish to work on local development please clone/fork the git repo and use `pip install -r requirements.txt` to setup the project.
 
 ### Testing
 
 ```shell
 # In case packages are not installed yet
-pip install -r requirements/requirements-test.txt
+pip3 install -r requirements/requirements-test.txt
 
-python -m pytest tests/
+python3 -m pytest tests/
 ```
 
 ## Links
 
-* [DataMaxi+](https://datamaxiplus.com/)
-* [DataMaxi+ API](https://api.neverest.finance/)
-* [DataMaxi+ API Documentation](https://docs.neverest.finance/)
+- [DataMaxi+](https://datamaxiplus.com/)
+- [DataMaxi+ API](https://api.datamaxiplus.com/)
+- [DataMaxi+ API Documentation](https://docs.datamaxiplus.com/)
 
 ## Contributing
 
 We welcome contributions!
 If you discover a bug in this project, please feel free to open an issue to discuss the changes you would like to propose.
 
 ## License
```

### Comparing `datamaxi-0.1.0/pyproject.toml` & `datamaxi-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "datamaxi"
-version = "0.1.0"
+version = "0.2.0"
 authors = [
   { name="Bisonai", email="business@bisonai.com" },
 ]
 description = "Official Python client for DataMaxi+ API"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `datamaxi-0.1.0/tests/test_api.py` & `datamaxi-0.2.0/tests/test_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,31 +20,31 @@
     client.session.headers.should.have.key("Content-Type").which.should.equal(
         "application/json;charset=utf-8"
     )
     client.session.headers.should.have.key("User-Agent").which.should.equal(
         "datamaxi/" + __version__
     )
     client.session.headers.should.have.key("Authorization").which.should.be.equal(
-        "X-NVRST-APIKEY None"
+        "X-DTMX-APIKEY None"
     )
 
     client._logger.should.be(logging.getLogger("datamaxi.api"))
 
 
 def test_API_env_key():
     """Tests the API initialization with API key in environment variable"""
 
     api_key = random_str()
-    os.environ["NEVEREST_API_KEY"] = api_key
+    os.environ["DATAMAXI_API_KEY"] = api_key
     client = API()
 
     client.should.be.a(API)
     client.api_key.should.be.equal(api_key)
     client.session.headers.should.have.key("Authorization").which.should.be.equal(
-        f"X-NVRST-APIKEY {api_key}"
+        f"X-DTMX-APIKEY {api_key}"
     )
 
 
 def test_API_with_extra_parameters():
     """Tests the API initialization with extra parameters"""
 
     api_key = random_str()
@@ -64,9 +64,9 @@
     client.api_key.should.equal(api_key)
     client.timeout.should.equal(0.1)
     client.base_url.should.equal(base_url)
     client.show_limit_usage.should.be.true
     client.show_header.should.be.true
     client.proxies.should.equal(proxies)
     client.session.headers.should.have.key("Authorization").which.should.equal(
-        f"X-NVRST-APIKEY {api_key}"
+        f"X-DTMX-APIKEY {api_key}"
     )
```

