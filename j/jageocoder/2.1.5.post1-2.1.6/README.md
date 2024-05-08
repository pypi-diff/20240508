# Comparing `tmp/jageocoder-2.1.5.post1.tar.gz` & `tmp/jageocoder-2.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jageocoder-2.1.5.post1.tar", max compression
+gzip compressed data, was "jageocoder-2.1.6.tar", max compression
```

## Comparing `jageocoder-2.1.5.post1.tar` & `jageocoder-2.1.6.tar`

### file list

```diff
@@ -1,20 +1,21 @@
--rw-r--r--   0        0        0      113 2023-08-03 02:25:59.197434 jageocoder-2.1.5.post1/LICENSE
--rw-r--r--   0        0        0     8253 2024-04-15 00:39:42.101477 jageocoder-2.1.5.post1/README.md
--rw-r--r--   0        0        0     1370 2024-04-17 07:34:57.054686 jageocoder-2.1.5.post1/jageocoder/__init__.py
--rw-r--r--   0        0        0     5605 2024-04-16 08:30:01.122082 jageocoder-2.1.5.post1/jageocoder/__main__.py
--rw-r--r--   0        0        0     2574 2023-08-03 02:25:59.209435 jageocoder-2.1.5.post1/jageocoder/address.py
--rw-r--r--   0        0        0     1421 2023-08-03 02:25:59.209435 jageocoder-2.1.5.post1/jageocoder/aliases.json
--rw-r--r--   0        0        0     8320 2024-04-15 00:39:35.469528 jageocoder-2.1.5.post1/jageocoder/aza_master.py
--rw-r--r--   0        0        0     1171 2023-08-03 02:25:59.209435 jageocoder-2.1.5.post1/jageocoder/dataset.py
--rw-r--r--   0        0        0      691 2023-08-03 02:25:59.209435 jageocoder-2.1.5.post1/jageocoder/exceptions.py
--rw-r--r--   0        0        0    19415 2024-04-15 00:39:35.469528 jageocoder-2.1.5.post1/jageocoder/itaiji.py
--rw-r--r--   0        0        0    14220 2023-08-03 02:25:59.209435 jageocoder-2.1.5.post1/jageocoder/itaiji_dic.json
--rw-r--r--   0        0        0    12256 2024-04-16 08:41:18.843470 jageocoder-2.1.5.post1/jageocoder/module.py
--rw-r--r--   0        0        0    53418 2024-04-17 06:36:23.572171 jageocoder-2.1.5.post1/jageocoder/node.py
--rw-r--r--   0        0        0     3660 2024-04-17 06:27:31.657403 jageocoder-2.1.5.post1/jageocoder/result.py
--rw-r--r--   0        0        0    15687 2024-04-16 08:33:55.201079 jageocoder-2.1.5.post1/jageocoder/rtree.py
--rw-r--r--   0        0        0     7795 2023-09-27 08:08:26.315234 jageocoder-2.1.5.post1/jageocoder/strlib.py
--rw-r--r--   0        0        0    52841 2024-04-15 00:39:35.473528 jageocoder-2.1.5.post1/jageocoder/tree.py
--rw-r--r--   0        0        0     4995 2023-08-03 02:25:59.213435 jageocoder-2.1.5.post1/jageocoder/trie.py
--rw-r--r--   0        0        0     1294 2024-04-17 07:34:36.614345 jageocoder-2.1.5.post1/pyproject.toml
--rw-r--r--   0        0        0     9772 1970-01-01 00:00:00.000000 jageocoder-2.1.5.post1/PKG-INFO
+-rw-r--r--   0        0        0      113 2024-05-08 05:06:37.205667 jageocoder-2.1.6/LICENSE
+-rw-r--r--   0        0        0    10310 2024-05-08 05:06:37.213667 jageocoder-2.1.6/README.md
+-rw-r--r--   0        0        0     1364 2024-05-08 03:51:15.514717 jageocoder-2.1.6/jageocoder/__init__.py
+-rw-r--r--   0        0        0     5759 2024-05-08 03:51:15.514717 jageocoder-2.1.6/jageocoder/__main__.py
+-rw-r--r--   0        0        0     2574 2023-08-03 02:25:59.209435 jageocoder-2.1.6/jageocoder/address.py
+-rw-r--r--   0        0        0     1421 2023-08-03 02:25:59.209435 jageocoder-2.1.6/jageocoder/aliases.json
+-rw-r--r--   0        0        0     8320 2024-04-15 00:39:35.469528 jageocoder-2.1.6/jageocoder/aza_master.py
+-rw-r--r--   0        0        0     1171 2024-05-02 04:32:53.380509 jageocoder-2.1.6/jageocoder/dataset.py
+-rw-r--r--   0        0        0      837 2024-05-08 03:51:15.514717 jageocoder-2.1.6/jageocoder/exceptions.py
+-rw-r--r--   0        0        0    19415 2024-04-15 00:39:35.469528 jageocoder-2.1.6/jageocoder/itaiji.py
+-rw-r--r--   0        0        0    14220 2023-08-03 02:25:59.209435 jageocoder-2.1.6/jageocoder/itaiji_dic.json
+-rw-r--r--   0        0        0    13645 2024-05-08 03:51:15.514717 jageocoder-2.1.6/jageocoder/module.py
+-rw-r--r--   0        0        0    54152 2024-05-08 03:51:15.514717 jageocoder-2.1.6/jageocoder/node.py
+-rw-r--r--   0        0        0     9824 2024-05-08 03:51:15.514717 jageocoder-2.1.6/jageocoder/remote.py
+-rw-r--r--   0        0        0     3898 2024-05-08 03:51:15.514717 jageocoder-2.1.6/jageocoder/result.py
+-rw-r--r--   0        0        0    15687 2024-04-16 08:33:55.201079 jageocoder-2.1.6/jageocoder/rtree.py
+-rw-r--r--   0        0        0     7795 2023-09-27 08:08:26.315234 jageocoder-2.1.6/jageocoder/strlib.py
+-rw-r--r--   0        0        0    53605 2024-05-08 03:51:15.514717 jageocoder-2.1.6/jageocoder/tree.py
+-rw-r--r--   0        0        0     4995 2023-08-03 02:25:59.213435 jageocoder-2.1.6/jageocoder/trie.py
+-rw-r--r--   0        0        0     1288 2024-05-08 05:06:37.213667 jageocoder-2.1.6/pyproject.toml
+-rw-r--r--   0        0        0    11823 1970-01-01 00:00:00.000000 jageocoder-2.1.6/PKG-INFO
```

### Comparing `jageocoder-2.1.5.post1/README.md` & `jageocoder-2.1.6/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,20 @@
-# jageocoder - A Python Japanese geocoder
+# Jageocoder - A Python Japanese geocoder
 
 日本語版は README_ja.md をお読みください。
 
-This is a Python port of the Japanese-address geocoder used in CSIS at the University of Tokyo's ["Address Matching Service"](https://newspat.csis.u-tokyo.ac.jp/geocode/modules/addmatch/index.php?content_id=1) and [GSI Maps](https://maps.gsi.go.jp/).
+This is a Python port of the Japanese-address geocoder `DAMS` used in CSIS at the University of Tokyo's ["Address Matching Service"](https://newspat.csis.u-tokyo.ac.jp/geocode/modules/addmatch/index.php?content_id=1) and [GSI Maps](https://maps.gsi.go.jp/).
 
 # Getting Started
 
 This package provides address-geocoding functionality for Python programs. The basic usage is to specify a dictionary with `init()` then call `search()` to get geocoding results.
 
 ```python
-python
 >>> import jageocoder
->>> jageocoder.init()
+>>> jageocoder.init(url='https://jageocoder.info-proto.com/jsonrpc')
 >>> jageocoder.search('新宿区西新宿2-8-1')
 {'matched': '新宿区西新宿2-8-', 'candidates': [{'id': 5961406, 'name': '8番', 'x': 139.691778, 'y': 35.689627, 'level': 7, 'note': None, 'fullname': ['東京都', '新宿区', '西新宿', '二丁目', '8番']}]}
 ```
 
 # How to install
 
 ## Prerequisites
@@ -23,99 +22,113 @@
 Requires Python 3.7.x or later.
 
 All other required packages will be installed automatically.
 
 ## Install instructions
 
 - Install the package with `pip install jageocoder`
-- Download an address database file compatible with that version from 
-  [here](https://www.info-proto.com/static/jageocoder/latest/v2/)
-- Install the dictionary with `install-dictionary` command
 
-```sh
-pip install jageocoder
-wget https://www.info-proto.com/static/jageocoder/latest/v2/jukyo_all_v21.zip
-jageocoder install-dictionary jukyo_all_v20.zip
-```
+To use Jageocoder, you need to install the "Dictionary Database" on the same machine or connect to the RPC service provided by [jageocoder-server](https://t-sagara.github.io/jageocoder/server/) .
+
+### Install Dictionary Database
+
+Large amounts of data can be processed at high speed when a dictionary database is installed. A database covering addresses in Japan requires 30 GB or more of storage.
+
+- Download an address database file compatible with that version from [here](https://www.info-proto.com/static/jageocoder/latest/v2/)
 
-The dictionary database will be installed under
-`{sys.prefix}/jageocoder/db2/` by default,
-however if the user doesn't have write permission there,
-`{site.USER_DATA}/jageocoder/db2/` instead.
+      wget https://www.info-proto.com/static/jageocoder/latest/v2/jukyo_all_v21.zip 
+
+- Install the dictionary with `install-dictionary` command
+
+      jageocoder install-dictionary jukyo_all_v21.zip
 
 If you need to know the location of the dictionary directory,
 perform `get-db-dir` command as follows. (Or call
 `jageocoder.get_db_dir()` in your script)
 
-```sh
+```bash
 jageocoder get-db-dir
 ```
 
-If you prefer to create it in another location, set the environment
-variable `JAGEOCODER_DB2_DIR` before executing `install_dictionary()`
-to specify the directory.
+If you prefer to create the database in another location, set the environment variable `JAGEOCODER_DB2_DIR` before executing `install_dictionary()` to specify the directory.
 
-```sh
+```bash
 export JAGEOCODER_DB2_DIR='/usr/local/share/jageocoder/db2'
 install-dictionary <db-file>
 ```
 
+### Connect to the Jageocoder server
+
+Since dictionary databases are large in size, installing them on multiple machines consumes storage and requires time and effort to update them.
+Instead of installing a dictionary database on each machine, you can connect to a Jageocoder server to perform the search process.
+
+If you want to use a server, specify the server endpoint in the environment variable `JAGEOCODER_SERVER_URL`. For a public demonstration server, use the following
+
+```bash
+export JAGEOCODER_SERVER_URL=https://jageocoder.info-proto.com/jsonrpc
+```
+
+However, the server for public demonstrations cannot withstand the load when accesses are concentrated, so it is limited to one request per second.
+If you want to process a large number of requests, please refer to [here](https://t-sagara.github.io/jageocoder/server/) to set up your own Jageocoder server. The endpoint is '/jsonrpc' on the server.
+
 ## Uninstall instructions
 
 Remove the directory containing the database, or perform 
 `uninstall-dictionary` command as follows.
 
-```sh
+```bash
 jageocoder uninstall-dictionary
 ```
 
 Then, uninstall the package with `pip` command.
 
-```sh
+```bash
 pip uninstall jageocoder
 ```
 
 # How to use
 
 ## Use from the command line
 
-We assume that jageocoder will be embedded in applications
-as a library and used by calling the API, but for testing purposes,
-you can check the geocoding results with the following command.
+Jageocoder is intended to be embedded in applications as a library and used by calling the API, but a simple command line interface is also provided.
 
-```sh
+For example, to geocode an address, execute the following command.
+
+```bash
 jageocoder search 新宿区西新宿２－８－１
 ```
 
 You can check the list of available commands with `--help`.
 
-```sh
+```bash
 jageocoder --help
 ```
 
 ## Using API
 
 First, import jageocoder and initialize it with `init()`.
 
-```
+```python
 >>> import jageocoder
 >>> jageocoder.init()
 ```
 
+The parameter `db_dir` of `init()` can be used to specify the directory where the address database is installed. Alternatively, you can specify the endpoint URL of the Jageocoder server with `url`. If it is omitted, the value of the environment variable is used.
+
 ### Search for latitude and longitude by address
 
 Use `search()` to search for the address you want to check the longitude and latitude of.
 
 The `search()` function returns a dict with `matched` as
 the matched string and `candidates` as the list of search results.
 (The results are formatted for better viewing)
 
 Each element of `candidates` contains the information of an address node (AddressNode).
 
-```
+```python
 >>> jageocoder.search('新宿区西新宿２－８－１')
 {
   'matched': '新宿区西新宿２－８－',
   'candidates': [{
     'id': 12299846, 'name': '8番',
     'x': 139.691778, 'y': 35.689627, 'level': 7, 'note': None,
     'fullname': ['東京都', '新宿区', '西新宿', '二丁目', '8番']
@@ -132,24 +145,42 @@
 - level: Address level (1:Prefecture, 2:County, 3:City and 23 district,
     4:Ward, 5:Oaza, 6:Aza and Chome, 7:Block, 8:Building)
 - note: Notes such as city codes
 - fullname: List of address notations from the prefecture level to this node
 
 ### Search for addresses by longitude and latitude
 
-Note: This method is not available in v2 series.
+You can specify the latitude and longitude of a point and look up the address of that point (so-called reverse geocoding).
+
+When you pass the longitude and latitude of the point you wish to look up to `reverse()`, you can retrieve up to three address nodes surrounding the specified point.
+
+```python
+>>> import jageocoder
+>>> jageocoder.init()
+>>> triangle = jageocoder.reverse(139.6917, 35.6896, level=7)
+>>> if len(triangle) > 0:
+...     print(triangle[0]['candidate']['fullname'])
+...
+['東京都', '新宿区', '西新宿', '二丁目', '8番']
+```
+
+In the example above, the ``level`` optional parameter is set to 7 to search down to the block (街区・地番) level.
+
+> [!NOTE]
+>
+> Indexes for reverse geocoding are automatically created the first time you perform reverse geocoding. Note that this process can take a long time.
 
 ### Explore the attribute information of an address
 
 Use `searchNode()` to retrieve information about an address.
 
 This function returns a list of type `jageocoder.result.Result` .
 You can access the address node from node element of the Result object.
 
-```
+```python
 >>> results = jageocoder.searchNode('新宿区西新宿２－８－１')
 >>> len(results)
 1
 >>> results[0].matched
 '新宿区西新宿２－８－'
 >>> type(results[0].node)
 <class 'jageocoder.node.AddressNode'>
@@ -159,56 +190,55 @@
 ```
 
 #### Get GeoJSON representation
 
 You can use the `as_geojson()` method of the Result and AddressNode
 objects to obtain the GeoJSON representation.
 
-```
+```python
 >>> results[0].as_geojson()
 {'type': 'Feature', 'geometry': {'type': 'Point', 'coordinates': [139.691778, 35.689627]}, 'properties': {'id': 12299851, 'name': '8番', 'level': 7, 'note': None, 'fullname': ['東京都', '新宿区', '西新宿', '二丁目', '8番'], 'matched': '新宿区西新宿２－８－'}}
 >>> results[0].node.as_geojson()
 {'type': 'Feature', 'geometry': {'type': 'Point', 'coordinates': [139.691778, 35.689627]}, 'properties': {'id': 12299851, 'name': '8番', 'level': 7, 'note': None, 'fullname': ['東京都', '新宿区', '西新宿', '二丁目', '8番']}}
 ```
 
 #### Get the local government codes
 
-There are two types of local government codes: JISX0402 (5-digit) and
-Local Government Code (6-digit).
+There are two types of local government codes: JISX0402 (5-digit) and Local Government Code (6-digit).
 
 You can also obtain the prefecture code JISX0401 (2 digits).
 
-```
+```python
 >>> node.get_city_jiscode()  # 5-digit code
 '13104'
 >>> node.get_city_local_authority_code() # 6-digit code
 '131041'
 >>> node.get_pref_jiscode()  # prefecture code
 '13'
 ```
 
 #### Get link URLs to maps
 
 Generate URLs to link to GSI and Google maps.
 
-```
+```python
 >>> node.get_gsimap_link()
 'https://maps.gsi.go.jp/#16/35.689627/139.691778/'
 >>> node.get_googlemap_link()
 'https://maps.google.com/maps?q=35.689627,139.691778&z=16'
 ```
 
 #### Traverse the parent node
 
 A "parent node" is a node that represents a level above the address.
 Get the node by attribute `parent`.
 
 Now the `node` points to '8番', so the parent node will be '二丁目'.
 
-```
+```python
 >>> parent = node.parent
 >>> parent.get_fullname()
 ['東京都', '新宿区', '西新宿', '二丁目']
 >>> parent.x, parent.y
 (139.691774, 35.68945)
 ```
 
@@ -220,33 +250,25 @@
 There is one parent node, but there are multiple child nodes.
 The actual return is a SQL query object, but it can be looped through
 with an iterator or cast to a list.
 
 Now the `parent` points to '二丁目', so the child node will be
 the block number (○番) contained therein.
 
-```
+```python
 >>> parent.children
 <sqlalchemy.orm.dynamic.AppenderQuery object at 0x7fbc08404b38>
 >>> [child.name for child in parent.children]
 ['10番', '11番', '1番', '2番', '3番', '4番', '5番', '6番', '7番', '8番', '9番']
 ```
 
 ## Create your own dictionary
 
 Consider using [jageocoder-converter](https://github.com/t-sagara/jageocoder-converter).
 
-## ToDos
-
-- Supporting address changes
-
-    The functionality to handle address changes due to municipal consolidation, etc.
-    has already been implemented in the C++ version, but will be implemented
-    in this package in the future.
-
 ## Contributing
 
 Address notation varies. So suggestions for logic improvements are welcome.
 Please submit an issue with examples of address notations in use and how they should be parsed.
 
 ## Authors
 
@@ -256,13 +278,10 @@
 
 This project is licensed under [the MIT License](https://opensource.org/licenses/mit-license.php).
 
 This is not the scope of the dictionary data license. Please follow the license of the respective dictionary data.
 
 ## Acknowledgements
 
-We would like to thank CSIS for allowing us to provide address matching services
-on their institutional website for over 20 years.
+We would like to thank CSIS for allowing us to provide address matching services on their institutional website for over 20 years.
 
-We would also like to thank Professor Asanobu Kitamoto of NII for providing us
-with a large sample of areas using the older address system and for his many help
-in confirming the results of our analysis.
+We would also like to thank Professor Asanobu Kitamoto of NII for providing us with a large sample of areas using the older address system and for his many help in confirming the results of our analysis.
```

### Comparing `jageocoder-2.1.5.post1/jageocoder/__init__.py` & `jageocoder-2.1.6/jageocoder/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 running the following steps.
 
     >>> import jageocoder
     >>> jageocoder.init()
     >>> jageocoder.searchNode('<Japanese-address>')
 """
 
-__version__ = '2.1.5.post1'  # The package version
+__version__ = '2.1.6'  # The package version
 __dictionary_version__ = '20230927'  # Compatible dictionary version
 __author__ = 'Takeshi Sagara <sagara@info-proto.com>'
 
 __all__ = [
     'init',
     'free',
     'is_initialized',
```

### Comparing `jageocoder-2.1.5.post1/jageocoder/__main__.py` & `jageocoder-2.1.6/jageocoder/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,29 +8,30 @@
 
 HELP = """
 'jageocoder' は日本の住所ジオコーダを実装した Python パッケージです。
 
 Usage:
   {p} -h
   {p} -v
-  {p} search [-d] [--area=<area>] [--db-dir=<dir>] <address>
-  {p} reverse [-d] [--level=<level>] [--db-dir=<dir>] <longitude> <latitude>
+  {p} search [-d] [--area=<area>] [--db-dir=<dir>|--url=<url>] <address>
+  {p} reverse [-d] [--level=<level>] [--db-dir=<dir>|--url=<url>] <longitude> <latitude>
   {p} get-db-dir [-d]
   {p} download-dictionary [-d] <url>
   {p} install-dictionary [-d] [-y] [--db-dir=<dir>] <path>
   {p} uninstall-dictionary [-d] [--db-dir=<dir>]
 
 Options:
   -h --help           このヘルプメッセージを表示します.
   -v --version        バージョン番号を表示します.
   -d --debug          実行時にデバッグメッセージを表示します.
   -y --yes            確認メッセージに対して自動的に y と答えます。
   --area=<area>       検索対象地域の都道府県・市区町村名を指定します。
   --level=<level>     検索する住所レベルを指定します。
   --db-dir=<dir>      住所データベースのディレクトリを指定します。
+  --url=<url>         Jageocoderサーバのエンドポイント URL を指定します。
 
 Examples:
 
 - 住所を検索します。
 
   {p} search 多摩市落合1-15
   {p} search --area=14152 中央1-1
@@ -90,15 +91,15 @@
     console_handler.setFormatter(
         logging.Formatter(
             '%(levelname)s:%(name)s:%(lineno)s:%(funcName)s:%(message)s')
     )
     logger.addHandler(console_handler)
 
     if args['search']:
-        jageocoder.init(db_dir=args['--db-dir'], mode='r')
+        jageocoder.init(db_dir=args['--db-dir'], mode='r', url=args['--url'])
         target_area = None
         if args.get('--area'):
             target_area = args['--area'].split(',')
 
         try:
             jageocoder.set_search_config(target_area=target_area)
         except RuntimeError:
@@ -116,15 +117,15 @@
             print(
                 "An error occurred during the search: {}".format(e),
                 file=sys.stderr)
             exit(1)
 
     elif args['reverse']:
         from jageocoder.address import AddressLevel
-        jageocoder.init(db_dir=args['--db-dir'], mode='r')
+        jageocoder.init(db_dir=args['--db-dir'], mode='r', url=args['--url'])
         print(json.dumps(
             jageocoder.reverse(
                 x=float(args['<longitude>']),
                 y=float(args['<latitude>']),
                 level=int(args['--level'] or AddressLevel.AZA)),
             ensure_ascii=False))
```

### Comparing `jageocoder-2.1.5.post1/jageocoder/address.py` & `jageocoder-2.1.6/jageocoder/address.py`

 * *Files identical despite different names*

### Comparing `jageocoder-2.1.5.post1/jageocoder/aliases.json` & `jageocoder-2.1.6/jageocoder/aliases.json`

 * *Files identical despite different names*

### Comparing `jageocoder-2.1.5.post1/jageocoder/aza_master.py` & `jageocoder-2.1.6/jageocoder/aza_master.py`

 * *Files identical despite different names*

### Comparing `jageocoder-2.1.5.post1/jageocoder/dataset.py` & `jageocoder-2.1.6/jageocoder/dataset.py`

 * *Files identical despite different names*

### Comparing `jageocoder-2.1.5.post1/jageocoder/exceptions.py` & `jageocoder-2.1.6/jageocoder/exceptions.py`

 * *Files 12% similar despite different names*

```diff
@@ -27,12 +27,19 @@
 class AddressTreeException(RuntimeError):
     """
     Custom exception classes sent out by jageocoder.tree submodule.
     """
     pass
 
 
+class RemoteTreeException(AddressTreeException):
+    """
+    Custom exception classes sent out by jageocoder.remote submodule.
+    """
+    pass
+
+
 class AddressTrieError(RuntimeError):
     """
     Custom exception classes sent out by jageocoder.trie submodule.
     """
     pass
```

### Comparing `jageocoder-2.1.5.post1/jageocoder/itaiji.py` & `jageocoder-2.1.6/jageocoder/itaiji.py`

 * *Files identical despite different names*

### Comparing `jageocoder-2.1.5.post1/jageocoder/itaiji_dic.json` & `jageocoder-2.1.6/jageocoder/itaiji_dic.json`

 * *Files identical despite different names*

### Comparing `jageocoder-2.1.5.post1/jageocoder/module.py` & `jageocoder-2.1.6/jageocoder/module.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,23 +5,25 @@
 from typing import Optional, Union, List
 import urllib.request
 from urllib.error import URLError
 
 import jageocoder
 from jageocoder.exceptions import JageocoderError
 from jageocoder.tree import AddressTree, get_db_dir
+from jageocoder.remote import RemoteTree
 from jageocoder.result import Result
 
 _tree = None  # The default AddressTree
 logger = logging.getLogger(__name__)
 
 
 def init(db_dir: Optional[os.PathLike] = None,
          mode: Optional[str] = 'r',
          debug: Optional[bool] = False,
+         url: Optional[str] = None,
          **kwargs) -> None:
     """
     Initialize the module-level AddressTree object `jageocoder.tree`
     ready for use.
 
     Parameters
     ----------
@@ -37,23 +39,52 @@
 
         - In the case of 'w', if the database already exists, delete it first.
           Then create a new one.
 
         - In the case of 'r', if the database already exists, it will be used.
           Otherwise raise a JageocoderError exception.
 
-    debug: bool, Optional(default=False)
+    debug: bool, optional(default=False)
         Debugging flag.
+
+    url: str, optional
+        URL of the Jageocoder server endpoint.
+
+    Notes
+    -----
+    - If both 'db_dir' and 'url' are specified, 'db_dir' has priority.
+    - If both 'db_dir' and 'url' are omitted, it looks for a dictionary
+        installed in the jageocoder package dcirectory.
+        If not found, a 'JageocoderError' exception is thrown.
     """
     global _tree
 
     if _tree:
         del _tree
 
-    _tree = AddressTree(db_dir=db_dir, mode=mode, debug=debug)
+    _url = None
+    _db_dir = None
+    if db_dir is not None:
+        _db_dir = db_dir
+    elif url is not None and mode == 'r':
+        _url = url
+    elif os.environ.get('JAGEOCODER_DB2_DIR'):
+        _db_dir = get_db_dir(mode=mode)
+
+    if _db_dir is None and _url is None:
+        _url = os.environ.get('JAGEOCODER_SERVER_URL')
+
+    if _db_dir:
+        _tree = AddressTree(db_dir=_db_dir, mode=mode, debug=debug)
+    elif _url:
+        _tree = RemoteTree(url=_url, debug=debug)
+    else:
+        raise JageocoderError(
+            "Neither 'db_dir' nor 'url' could be determined.")
+
     set_search_config(**kwargs)
 
 
 def free():
     """
     Frees all objects created by 'init()'.
     """
@@ -244,31 +275,40 @@
     # Remove the directory
     logger.info('Removing directory {}'.format(db_dir))
     import shutil
     shutil.rmtree(db_dir)
     logger.info('Dictionary has been uninstalled.')
 
 
-def installed_dictionary_version(db_dir: Optional[os.PathLike] = None) -> str:
+def installed_dictionary_version(
+    db_dir: Optional[os.PathLike] = None,
+    url: Optional[str] = None
+) -> str:
     """
     Get the installed dictionary version.
 
     Parameters
     ----------
     db_dir: os.PathLike, optional
         The directory where the database files has been installed.
         If omitted, it will be determined by `get_db_dir()`.
 
+    url: str, optional
+        URL of the Jageocoder server endpoint.        
+
     Returns
     -------
     str
-        The version string of the installed dicitionary.
+        The version string of the installed dicitionary or the server.
     """
     if db_dir is None:
-        db_dir = get_db_dir(mode='a')
+        if url is not None:
+            return RemoteTree(url=url).installed_dictionary_version()
+
+        db_dir = get_db_dir(mode='r')
 
     metadata_path = os.path.join(db_dir, "metadata.txt")
     if os.path.exists(metadata_path):
         with open(metadata_path, "r") as f:
             version = f.readline().rstrip()
 
     else:
@@ -279,31 +319,40 @@
                 '%Y%m%d')
         else:
             version = '(Unknown)'
 
     return version
 
 
-def installed_dictionary_readme(db_dir: Optional[os.PathLike] = None) -> str:
+def installed_dictionary_readme(
+    db_dir: Optional[os.PathLike] = None,
+    url: Optional[str] = None
+) -> str:
     """
     Get the content of README.txt attached to the installed dictionary.
 
     Parameters
     ----------
     db_dir: os.PathLike, optional
         The directory where the database files has been installed.
         If omitted, it will be determined by `get_db_dir()`.
 
+    url: str, optional
+        URL of the Jageocoder server endpoint.        
+
     Returns
     -------
     str
         The content of the text.
     """
     if db_dir is None:
-        db_dir = get_db_dir(mode='a')
+        if url is not None:
+            return RemoteTree(url=url).installed_dictionary_readme()
+
+        db_dir = get_db_dir(mode='r')
 
     readme_path = os.path.join(db_dir, "README.md")
     if not os.path.exists(readme_path):
         return "(no README information)"
 
     with open(readme_path, "r") as f:
         content = f.read()
@@ -330,15 +379,14 @@
         List of dict representation of nodes with
         the longest match to the query string.
     """
     if not is_initialized():
         raise JageocoderError("Not initialized. Call 'init()' first.")
 
     global _tree
-    # set_search_config(best_only=True)
     results = _tree.searchNode(query)
 
     if _tree.get_config('best_only'):
         if len(results) == 0:
             return {'matched': '', 'candidates': []}
 
         return {
@@ -425,31 +473,32 @@
     -----
     - The result list contains up to 3 nodes.
     - Each element is a dict type with the following structure:
         {"candidate":AddressNode, "dist":float} 
     """
     if not is_initialized():
         raise JageocoderError("Not initialized. Call 'init()' first.")
-    from jageocoder.rtree import Index
 
     global _tree
-    idx = Index(tree=_tree)
-    return idx.nearest(x=x, y=y, level=level, as_dict=as_dict)
+    return _tree.reverse(x, y, level, as_dict)
 
 
 def create_trie_index() -> None:
     """
     Create the TRIE index from the database file.
 
     This function is a shortcut for AddressTree.create_trie_index().
     """
     if not is_initialized():
         raise JageocoderError("Not initialized. Call 'init()' first.")
 
     global _tree
+    if isinstance(_tree, RemoteTree):
+        raise JageocoderError("Can't update TRIE index on remote server.")
+
     _tree.create_trie_index()
 
 
 def version():
     return jageocoder.__version__
```

### Comparing `jageocoder-2.1.5.post1/jageocoder/node.py` & `jageocoder-2.1.6/jageocoder/node.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,30 +4,30 @@
 from functools import lru_cache
 import json
 import logging
 import os
 import re
 from typing import List, Set, Tuple, Optional, Union, TYPE_CHECKING
 
-from PortableTab import BaseTable
+import PortableTab
 
 from jageocoder.address import AddressLevel
 from jageocoder.dataset import Dataset
 from jageocoder.itaiji import Converter
 from jageocoder.result import Result
 from jageocoder.strlib import strlib
 
 if TYPE_CHECKING:
     from jageocoder.tree import AddressTree
 
 logger = logging.getLogger(__name__)
 default_itaiji_converter = Converter()  # With default settings
 
 
-class AddressNodeTable(BaseTable):
+class AddressNodeTable(PortableTab.BaseTable):
     """
     The address node table.
     """
 
     __tablename__ = "address_node"
     __schema__ = """
         struct AddressNode {
@@ -86,18 +86,29 @@
                 v = re.sub(r'\\([:/])', r'\g<1>', v)
                 if k not in ('ref', 'geoshape_city_id'):
                     # Do not include these attributes in the search index.
                     notes.append(attr)
 
             return notes
 
-        self.create_trie_on("nameIndex")
-        self.create_trie_on(
-            attr="note",
-            func=_split_note)
+        if PortableTab.__version__ < '0.3.5':
+            self.create_trie_on("nameIndex")
+            self.create_trie_on(
+                attr="note",
+                func=_split_note)
+        else:
+            self.create_trie_on(
+                attr="nameIndex",
+                filter_func=lambda r: r.level <= AddressLevel.AZA
+            )
+            self.create_trie_on(
+                attr="note",
+                key_func=_split_note,
+                filter_func=lambda r: r.level <= AddressLevel.AZA
+            )
 
 
 class AddressNode(object):
     """
     The address node stored in 'address_node' table.
 
     Parameters
@@ -1205,14 +1216,26 @@
             "y": self.y,
             "level": self.level,
             "priority": self.priority,
             "note": self.note,
             "fullname": self.get_fullname(),
         }
 
+    @classmethod
+    def from_dict(cls, jsonable: dict):
+        return AddressNode(
+            id=jsonable["id"],
+            name=jsonable["name"],
+            x=jsonable["x"],
+            y=jsonable["y"],
+            level=jsonable["level"],
+            priority=jsonable["priority"],
+            note=jsonable["note"]
+        )
+
     def as_geojson(self):
         """
         Return the geojson notation of the node.
         """
         return {
             "type": "Feature",
             "geometry": {
```

### Comparing `jageocoder-2.1.5.post1/jageocoder/result.py` & `jageocoder-2.1.6/jageocoder/result.py`

 * *Files 4% similar despite different names*

```diff
@@ -125,14 +125,22 @@
                 The substring matching the query.
         """
         return {
             "node": self.node.as_dict(),
             "matched": self.matched,
         }
 
+    @classmethod
+    def from_dict(cls, jsonable: dict):
+        from jageocoder.node import AddressNode
+        return Result(
+            node=AddressNode.from_dict(jsonable["node"]),
+            matched=jsonable["matched"],
+        )
+
     def as_geojson(self) -> dict:
         """
         Convert Result to GeoJSON dict type for display.
 
         Return
         ------
         dict
```

### Comparing `jageocoder-2.1.5.post1/jageocoder/rtree.py` & `jageocoder-2.1.6/jageocoder/rtree.py`

 * *Files identical despite different names*

### Comparing `jageocoder-2.1.5.post1/jageocoder/strlib.py` & `jageocoder-2.1.6/jageocoder/strlib.py`

 * *Files identical despite different names*

### Comparing `jageocoder-2.1.5.post1/jageocoder/tree.py` & `jageocoder-2.1.6/jageocoder/tree.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,19 @@
     """
     if mode not in ('a', 'w', 'r'):
         raise AddressTreeException(
             'Invalid mode value. Specify one of "a", "w", or "r".')
 
     db_dirs: List[Path] = []
     if 'JAGEOCODER_DB2_DIR' in os.environ:
-        db_dirs.append(Path(os.environ['JAGEOCODER_DB2_DIR']))
+        db_dir = os.environ.get('JAGEOCODER_DB2_DIR')
+        if db_dir.lower().startswith('http'):
+            return db_dir
+
+        db_dirs.append(Path(db_dir))
 
     db_dirs += [
         Path(sys.prefix) / 'jageocoder/db2/',
         Path(site.USER_BASE) / 'jageocoder/db2/',
     ]
 
     for db_dir in db_dirs:
@@ -112,34 +116,34 @@
 
 class AddressTree(object):
     """
     The address-tree structure.
 
     Attributes
     ----------
-    db_path: str
-        Path to the sqlite3 database file.
-    dsn: str
-        RFC-1738 based database-url, so called "data source name".
-    trie_path: str
-        Path to the TRIE index file.
-    engine : sqlalchemy.engine.Engine
-        The database engine which is used to connect to the database.
-    conn : sqlalchemy.engine.Connection
-        The connection object which is used to communicate witht the database.
-    session : sqlalchemy.orm.Session
-        The session object used for a series of database operations.
-    root : AddressNode
-        The root node of the tree.
-    trie : AddressTrie
-        The TRIE index of the tree.
     mode: str
-        The mode in which this tree was opened.
+        Read (r) or Write (w).
+    db_dir: PathLike
+        Directory path where the database files are located.
+    address_nodes: AddressNodeTable
+        Table of address-nodes.
+    aza_masters: AzaMaster
+        Aza master table from the Address Base registry.
+    trie_nodes: TrieNode
+        Table of trie-nodes.
+    trie_path: PathLike
+        Path to the AddressTrie file.
+    debug: bool
+        Debug mode flag.
+    root: AddressTrie
+        The root-node of the address TRIE index.
     config: dict
-        Settings the search method in this tree.
+        Configuration parameters.
+    converter: itaiji.Converter
+        Converter object of character-variants.
     """
 
     def __init__(self,
                  db_dir: Optional[os.PathLike] = None,
                  mode: str = 'a',
                  debug: Optional[bool] = None):
         """
@@ -194,14 +198,15 @@
         if self.mode == 'w':
             self.address_nodes.delete()
             if os.path.exists(self.trie_path):
                 os.remove(self.trie_path)
 
         self.root = None
         self.trie = AddressTrie(self.trie_path)
+        self.reverse_index = None
 
         # Regular expression
         self.re_float = re.compile(r'^\-?\d+\.?\d*$')
         self.re_int = re.compile(r'^\-?\d+$')
         self.re_address = re.compile(r'^(\d+);(.*)$')
 
         # Set default settings
@@ -1395,20 +1400,14 @@
             An address notation to be searched.
 
         Return
         ------
         list:
             A list of AddressNode and matched substring pairs.
 
-        Note
-        ----
-        The `search_by_trie` function returns the standardized string
-        as the match string. In contrast, the `searchNode` function
-        returns the de-starndized string.
-
         Example
         -------
         >>> import jageocoder
         >>> jageocoder.init()
         >>> tree = jageocoder.get_module_tree()
         >>> tree.searchNode('多摩市落合1-15-2')
         [[[11460207:東京都(139.69178,35.68963)1(lasdec:130001/jisx0401:13)]>[12063502:多摩市(139.446366,35.636959)3(jisx0402:13224)]>[12065383:落合(139.427097,35.624877)5(None)]>[12065384:一丁目(139.427097,35.624877)6(None)]>[12065390:15番地(139.428969,35.625779)7(None)], '多摩市落合1-15-']]
@@ -1508,7 +1507,44 @@
         self.address_nodes.create_indexes()
 
     def get_cache_info(self) -> dict:
         cache_info = {
             "get_record": AddressNodeTable.get_record.cache_info(),
         }
         return cache_info
+
+    def reverse(
+        self,
+        x: float,
+        y: float,
+        level: Optional[int] = None,
+        as_dict: Optional[bool] = True
+    ) -> list:
+        """
+        Reverse geocoding.
+
+        Parameters
+        ----------
+        x: float
+            Longitude of the point.
+        y: float
+            Latitude of the point.
+        level: int, optional
+            Target node level.
+        as_dict: bool, default=True
+            If True, returns candidates as dict objects.
+
+        Returns
+        -------
+        list
+
+        Notes
+        -----
+        - The result list contains up to 3 nodes.
+        - Each element is a dict type with the following structure:
+            {"candidate":AddressNode, "dist":float} 
+        """
+        if self.reverse_index is None:
+            from jageocoder.rtree import Index
+            self.reverse_index = Index(tree=self)
+
+        return self.reverse_index.nearest(x=x, y=y, level=level, as_dict=as_dict)
```

### Comparing `jageocoder-2.1.5.post1/jageocoder/trie.py` & `jageocoder-2.1.6/jageocoder/trie.py`

 * *Files identical despite different names*

### Comparing `jageocoder-2.1.5.post1/pyproject.toml` & `jageocoder-2.1.6/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jageocoder"
-version = "2.1.5.post1"
+version = "2.1.6"
 description = "A Japanese-address geocoder for Python."
 authors = ["Takeshi Sagara <sagara@info-proto.com>"]
 repository = "https://github.com/t-sagara/jageocoder/"
 license = "The MIT License"
 readme = "README.md"
 documentation = "https://jageocoder.readthedocs.io/"
 packages = [
```

### Comparing `jageocoder-2.1.5.post1/PKG-INFO` & `jageocoder-2.1.6/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jageocoder
-Version: 2.1.5.post1
+Version: 2.1.6
 Summary: A Japanese-address geocoder for Python.
 Home-page: https://github.com/t-sagara/jageocoder/
 License: The MIT License
 Author: Takeshi Sagara
 Author-email: sagara@info-proto.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -32,28 +32,27 @@
 Requires-Dist: rtree (>=1.0.0,<2.0.0)
 Requires-Dist: tqdm (>=4.00.0,<5.0.0)
 Requires-Dist: urllib3 (>=2.0.6)
 Project-URL: Documentation, https://jageocoder.readthedocs.io/
 Project-URL: Repository, https://github.com/t-sagara/jageocoder/
 Description-Content-Type: text/markdown
 
-# jageocoder - A Python Japanese geocoder
+# Jageocoder - A Python Japanese geocoder
 
 日本語版は README_ja.md をお読みください。
 
-This is a Python port of the Japanese-address geocoder used in CSIS at the University of Tokyo's ["Address Matching Service"](https://newspat.csis.u-tokyo.ac.jp/geocode/modules/addmatch/index.php?content_id=1) and [GSI Maps](https://maps.gsi.go.jp/).
+This is a Python port of the Japanese-address geocoder `DAMS` used in CSIS at the University of Tokyo's ["Address Matching Service"](https://newspat.csis.u-tokyo.ac.jp/geocode/modules/addmatch/index.php?content_id=1) and [GSI Maps](https://maps.gsi.go.jp/).
 
 # Getting Started
 
 This package provides address-geocoding functionality for Python programs. The basic usage is to specify a dictionary with `init()` then call `search()` to get geocoding results.
 
 ```python
-python
 >>> import jageocoder
->>> jageocoder.init()
+>>> jageocoder.init(url='https://jageocoder.info-proto.com/jsonrpc')
 >>> jageocoder.search('新宿区西新宿2-8-1')
 {'matched': '新宿区西新宿2-8-', 'candidates': [{'id': 5961406, 'name': '8番', 'x': 139.691778, 'y': 35.689627, 'level': 7, 'note': None, 'fullname': ['東京都', '新宿区', '西新宿', '二丁目', '8番']}]}
 ```
 
 # How to install
 
 ## Prerequisites
@@ -61,99 +60,113 @@
 Requires Python 3.7.x or later.
 
 All other required packages will be installed automatically.
 
 ## Install instructions
 
 - Install the package with `pip install jageocoder`
-- Download an address database file compatible with that version from 
-  [here](https://www.info-proto.com/static/jageocoder/latest/v2/)
-- Install the dictionary with `install-dictionary` command
 
-```sh
-pip install jageocoder
-wget https://www.info-proto.com/static/jageocoder/latest/v2/jukyo_all_v21.zip
-jageocoder install-dictionary jukyo_all_v20.zip
-```
+To use Jageocoder, you need to install the "Dictionary Database" on the same machine or connect to the RPC service provided by [jageocoder-server](https://t-sagara.github.io/jageocoder/server/) .
+
+### Install Dictionary Database
+
+Large amounts of data can be processed at high speed when a dictionary database is installed. A database covering addresses in Japan requires 30 GB or more of storage.
+
+- Download an address database file compatible with that version from [here](https://www.info-proto.com/static/jageocoder/latest/v2/)
 
-The dictionary database will be installed under
-`{sys.prefix}/jageocoder/db2/` by default,
-however if the user doesn't have write permission there,
-`{site.USER_DATA}/jageocoder/db2/` instead.
+      wget https://www.info-proto.com/static/jageocoder/latest/v2/jukyo_all_v21.zip 
+
+- Install the dictionary with `install-dictionary` command
+
+      jageocoder install-dictionary jukyo_all_v21.zip
 
 If you need to know the location of the dictionary directory,
 perform `get-db-dir` command as follows. (Or call
 `jageocoder.get_db_dir()` in your script)
 
-```sh
+```bash
 jageocoder get-db-dir
 ```
 
-If you prefer to create it in another location, set the environment
-variable `JAGEOCODER_DB2_DIR` before executing `install_dictionary()`
-to specify the directory.
+If you prefer to create the database in another location, set the environment variable `JAGEOCODER_DB2_DIR` before executing `install_dictionary()` to specify the directory.
 
-```sh
+```bash
 export JAGEOCODER_DB2_DIR='/usr/local/share/jageocoder/db2'
 install-dictionary <db-file>
 ```
 
+### Connect to the Jageocoder server
+
+Since dictionary databases are large in size, installing them on multiple machines consumes storage and requires time and effort to update them.
+Instead of installing a dictionary database on each machine, you can connect to a Jageocoder server to perform the search process.
+
+If you want to use a server, specify the server endpoint in the environment variable `JAGEOCODER_SERVER_URL`. For a public demonstration server, use the following
+
+```bash
+export JAGEOCODER_SERVER_URL=https://jageocoder.info-proto.com/jsonrpc
+```
+
+However, the server for public demonstrations cannot withstand the load when accesses are concentrated, so it is limited to one request per second.
+If you want to process a large number of requests, please refer to [here](https://t-sagara.github.io/jageocoder/server/) to set up your own Jageocoder server. The endpoint is '/jsonrpc' on the server.
+
 ## Uninstall instructions
 
 Remove the directory containing the database, or perform 
 `uninstall-dictionary` command as follows.
 
-```sh
+```bash
 jageocoder uninstall-dictionary
 ```
 
 Then, uninstall the package with `pip` command.
 
-```sh
+```bash
 pip uninstall jageocoder
 ```
 
 # How to use
 
 ## Use from the command line
 
-We assume that jageocoder will be embedded in applications
-as a library and used by calling the API, but for testing purposes,
-you can check the geocoding results with the following command.
+Jageocoder is intended to be embedded in applications as a library and used by calling the API, but a simple command line interface is also provided.
 
-```sh
+For example, to geocode an address, execute the following command.
+
+```bash
 jageocoder search 新宿区西新宿２－８－１
 ```
 
 You can check the list of available commands with `--help`.
 
-```sh
+```bash
 jageocoder --help
 ```
 
 ## Using API
 
 First, import jageocoder and initialize it with `init()`.
 
-```
+```python
 >>> import jageocoder
 >>> jageocoder.init()
 ```
 
+The parameter `db_dir` of `init()` can be used to specify the directory where the address database is installed. Alternatively, you can specify the endpoint URL of the Jageocoder server with `url`. If it is omitted, the value of the environment variable is used.
+
 ### Search for latitude and longitude by address
 
 Use `search()` to search for the address you want to check the longitude and latitude of.
 
 The `search()` function returns a dict with `matched` as
 the matched string and `candidates` as the list of search results.
 (The results are formatted for better viewing)
 
 Each element of `candidates` contains the information of an address node (AddressNode).
 
-```
+```python
 >>> jageocoder.search('新宿区西新宿２－８－１')
 {
   'matched': '新宿区西新宿２－８－',
   'candidates': [{
     'id': 12299846, 'name': '8番',
     'x': 139.691778, 'y': 35.689627, 'level': 7, 'note': None,
     'fullname': ['東京都', '新宿区', '西新宿', '二丁目', '8番']
@@ -170,24 +183,42 @@
 - level: Address level (1:Prefecture, 2:County, 3:City and 23 district,
     4:Ward, 5:Oaza, 6:Aza and Chome, 7:Block, 8:Building)
 - note: Notes such as city codes
 - fullname: List of address notations from the prefecture level to this node
 
 ### Search for addresses by longitude and latitude
 
-Note: This method is not available in v2 series.
+You can specify the latitude and longitude of a point and look up the address of that point (so-called reverse geocoding).
+
+When you pass the longitude and latitude of the point you wish to look up to `reverse()`, you can retrieve up to three address nodes surrounding the specified point.
+
+```python
+>>> import jageocoder
+>>> jageocoder.init()
+>>> triangle = jageocoder.reverse(139.6917, 35.6896, level=7)
+>>> if len(triangle) > 0:
+...     print(triangle[0]['candidate']['fullname'])
+...
+['東京都', '新宿区', '西新宿', '二丁目', '8番']
+```
+
+In the example above, the ``level`` optional parameter is set to 7 to search down to the block (街区・地番) level.
+
+> [!NOTE]
+>
+> Indexes for reverse geocoding are automatically created the first time you perform reverse geocoding. Note that this process can take a long time.
 
 ### Explore the attribute information of an address
 
 Use `searchNode()` to retrieve information about an address.
 
 This function returns a list of type `jageocoder.result.Result` .
 You can access the address node from node element of the Result object.
 
-```
+```python
 >>> results = jageocoder.searchNode('新宿区西新宿２－８－１')
 >>> len(results)
 1
 >>> results[0].matched
 '新宿区西新宿２－８－'
 >>> type(results[0].node)
 <class 'jageocoder.node.AddressNode'>
@@ -197,56 +228,55 @@
 ```
 
 #### Get GeoJSON representation
 
 You can use the `as_geojson()` method of the Result and AddressNode
 objects to obtain the GeoJSON representation.
 
-```
+```python
 >>> results[0].as_geojson()
 {'type': 'Feature', 'geometry': {'type': 'Point', 'coordinates': [139.691778, 35.689627]}, 'properties': {'id': 12299851, 'name': '8番', 'level': 7, 'note': None, 'fullname': ['東京都', '新宿区', '西新宿', '二丁目', '8番'], 'matched': '新宿区西新宿２－８－'}}
 >>> results[0].node.as_geojson()
 {'type': 'Feature', 'geometry': {'type': 'Point', 'coordinates': [139.691778, 35.689627]}, 'properties': {'id': 12299851, 'name': '8番', 'level': 7, 'note': None, 'fullname': ['東京都', '新宿区', '西新宿', '二丁目', '8番']}}
 ```
 
 #### Get the local government codes
 
-There are two types of local government codes: JISX0402 (5-digit) and
-Local Government Code (6-digit).
+There are two types of local government codes: JISX0402 (5-digit) and Local Government Code (6-digit).
 
 You can also obtain the prefecture code JISX0401 (2 digits).
 
-```
+```python
 >>> node.get_city_jiscode()  # 5-digit code
 '13104'
 >>> node.get_city_local_authority_code() # 6-digit code
 '131041'
 >>> node.get_pref_jiscode()  # prefecture code
 '13'
 ```
 
 #### Get link URLs to maps
 
 Generate URLs to link to GSI and Google maps.
 
-```
+```python
 >>> node.get_gsimap_link()
 'https://maps.gsi.go.jp/#16/35.689627/139.691778/'
 >>> node.get_googlemap_link()
 'https://maps.google.com/maps?q=35.689627,139.691778&z=16'
 ```
 
 #### Traverse the parent node
 
 A "parent node" is a node that represents a level above the address.
 Get the node by attribute `parent`.
 
 Now the `node` points to '8番', so the parent node will be '二丁目'.
 
-```
+```python
 >>> parent = node.parent
 >>> parent.get_fullname()
 ['東京都', '新宿区', '西新宿', '二丁目']
 >>> parent.x, parent.y
 (139.691774, 35.68945)
 ```
 
@@ -258,33 +288,25 @@
 There is one parent node, but there are multiple child nodes.
 The actual return is a SQL query object, but it can be looped through
 with an iterator or cast to a list.
 
 Now the `parent` points to '二丁目', so the child node will be
 the block number (○番) contained therein.
 
-```
+```python
 >>> parent.children
 <sqlalchemy.orm.dynamic.AppenderQuery object at 0x7fbc08404b38>
 >>> [child.name for child in parent.children]
 ['10番', '11番', '1番', '2番', '3番', '4番', '5番', '6番', '7番', '8番', '9番']
 ```
 
 ## Create your own dictionary
 
 Consider using [jageocoder-converter](https://github.com/t-sagara/jageocoder-converter).
 
-## ToDos
-
-- Supporting address changes
-
-    The functionality to handle address changes due to municipal consolidation, etc.
-    has already been implemented in the C++ version, but will be implemented
-    in this package in the future.
-
 ## Contributing
 
 Address notation varies. So suggestions for logic improvements are welcome.
 Please submit an issue with examples of address notations in use and how they should be parsed.
 
 ## Authors
 
@@ -294,14 +316,11 @@
 
 This project is licensed under [the MIT License](https://opensource.org/licenses/mit-license.php).
 
 This is not the scope of the dictionary data license. Please follow the license of the respective dictionary data.
 
 ## Acknowledgements
 
-We would like to thank CSIS for allowing us to provide address matching services
-on their institutional website for over 20 years.
+We would like to thank CSIS for allowing us to provide address matching services on their institutional website for over 20 years.
 
-We would also like to thank Professor Asanobu Kitamoto of NII for providing us
-with a large sample of areas using the older address system and for his many help
-in confirming the results of our analysis.
+We would also like to thank Professor Asanobu Kitamoto of NII for providing us with a large sample of areas using the older address system and for his many help in confirming the results of our analysis.
```

