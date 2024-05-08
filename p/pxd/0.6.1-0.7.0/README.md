# Comparing `tmp/pxd-0.6.1-py3-none-any.whl.zip` & `tmp/pxd-0.7.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,62 +1,63 @@
-Zip file size: 80439 bytes, number of entries: 60
+Zip file size: 82998 bytes, number of entries: 61
 -rw-r--r--  2.0 unx      622 b- defN 22-Mar-14 02:39 deployer/__init__.py
--rw-r--r--  2.0 unx      790 b- defN 23-Sep-28 02:40 deployer/_repo.py
+-rw-r--r--  2.0 unx      790 b- defN 24-Apr-22 03:28 deployer/_repo.py
 -rw-r--r--  2.0 unx      733 b- defN 22-Mar-14 02:39 deployer/logging.yaml
--rw-r--r--  2.0 unx     7178 b- defN 24-Jan-10 01:39 deployer/pxd.py
--rw-r--r--  2.0 unx       44 b- defN 24-Jan-10 01:39 deployer/version.txt
--rw-r--r--  2.0 unx      622 b- defN 23-Sep-28 02:40 deployer/config/__init__.py
--rw-r--r--  2.0 unx     5308 b- defN 23-Sep-28 02:40 deployer/config/config.py
+-rw-r--r--  2.0 unx     7626 b- defN 24-May-08 03:43 deployer/pxd.py
+-rw-r--r--  2.0 unx       44 b- defN 24-May-08 03:44 deployer/version.txt
+-rw-r--r--  2.0 unx      622 b- defN 24-Apr-22 03:28 deployer/config/__init__.py
+-rw-r--r--  2.0 unx     5529 b- defN 24-May-08 03:43 deployer/config/config.py
 -rw-r--r--  2.0 unx     1313 b- defN 22-Mar-14 02:39 deployer/config/log_config.py
 -rw-r--r--  2.0 unx     1080 b- defN 22-Jul-04 02:46 deployer/config/metadb_config.py
 -rw-r--r--  2.0 unx      622 b- defN 22-Mar-14 02:39 deployer/constant/__init__.py
--rw-r--r--  2.0 unx     1195 b- defN 23-Sep-28 02:40 deployer/constant/constant.py
+-rw-r--r--  2.0 unx     1195 b- defN 24-Apr-22 03:28 deployer/constant/constant.py
 -rw-r--r--  2.0 unx      715 b- defN 22-Mar-14 02:39 deployer/constant/table_field.py
 -rw-r--r--  2.0 unx      622 b- defN 22-Mar-14 02:39 deployer/core/__init__.py
 -rw-r--r--  2.0 unx      991 b- defN 22-Mar-14 02:39 deployer/core/context.py
 -rw-r--r--  2.0 unx     1377 b- defN 22-Dec-14 07:49 deployer/core/docker_manager.py
 -rw-r--r--  2.0 unx      623 b- defN 22-Mar-14 02:39 deployer/core/file_manager.py
 -rw-r--r--  2.0 unx      732 b- defN 22-Jul-04 02:46 deployer/core/flow.py
 -rw-r--r--  2.0 unx      622 b- defN 22-Mar-14 02:39 deployer/decorator/__init__.py
--rw-r--r--  2.0 unx     2376 b- defN 24-Jan-10 01:39 deployer/decorator/decorators.py
+-rw-r--r--  2.0 unx     2376 b- defN 24-Apr-22 03:28 deployer/decorator/decorators.py
 -rw-r--r--  2.0 unx      622 b- defN 23-Mar-23 05:37 deployer/download/__init__.py
 -rw-r--r--  2.0 unx     1219 b- defN 23-Apr-03 01:57 deployer/download/constant.py
 -rw-r--r--  2.0 unx    10463 b- defN 23-Mar-31 01:44 deployer/download/polardbx_download.py
 -rw-r--r--  2.0 unx      622 b- defN 22-Mar-14 02:39 deployer/pcn/__init__.py
 -rw-r--r--  2.0 unx      622 b- defN 22-Mar-14 02:39 deployer/pxc/__init__.py
--rw-r--r--  2.0 unx     1070 b- defN 23-Sep-28 02:40 deployer/pxc/gms_consts.py
--rw-r--r--  2.0 unx    43795 b- defN 24-Jan-10 01:39 deployer/pxc/polardbx_cluster.py
--rw-r--r--  2.0 unx     4175 b- defN 24-Jan-10 01:39 deployer/pxc/polardbx_manager.py
+-rw-r--r--  2.0 unx     1070 b- defN 24-Apr-22 03:28 deployer/pxc/gms_consts.py
+-rw-r--r--  2.0 unx    58096 b- defN 24-May-08 03:43 deployer/pxc/polardbx_cluster.py
+-rw-r--r--  2.0 unx     4260 b- defN 24-May-08 03:43 deployer/pxc/polardbx_manager.py
 -rw-r--r--  2.0 unx      930 b- defN 22-Mar-14 02:39 deployer/pxc/polardbx_topology.py
 -rw-r--r--  2.0 unx     1257 b- defN 22-Jul-04 02:46 deployer/pxc/pxc_user.py
 -rw-r--r--  2.0 unx      622 b- defN 22-Mar-14 02:39 deployer/resources/__init__.py
 -rw-r--r--  2.0 unx      260 b- defN 23-Mar-23 05:37 deployer/resources/download/scripts/load_image.sh
+-rw-r--r--  2.0 unx      493 b- defN 24-May-08 03:43 deployer/resources/download/scripts/polardbx-version.sh
 -rw-r--r--  2.0 unx     7330 b- defN 22-Mar-14 02:39 deployer/resources/sql/gms_init.sql
--rw-r--r--  2.0 unx     2137 b- defN 23-Sep-28 02:40 deployer/resources/sql/sqlite_init.sql
+-rw-r--r--  2.0 unx     2137 b- defN 24-Apr-22 03:28 deployer/resources/sql/sqlite_init.sql
 -rw-r--r--  2.0 unx     4872 b- defN 22-Mar-14 02:39 deployer/resources/template/my-8.0.cnf
 -rw-r--r--  2.0 unx     4614 b- defN 22-Dec-14 07:49 deployer/resources/template/my.cnf
 -rw-r--r--  2.0 unx     9148 b- defN 21-Jul-29 15:49 deployer/resources/template/my.cnf-5.7
 -rw-r--r--  2.0 unx     9169 b- defN 22-Dec-15 02:46 deployer/resources/template/my.cnf-5.7-xcluster
--rw-r--r--  2.0 unx    12661 b- defN 24-Jan-10 01:39 deployer/resources/template/my.cnf-8.0-galaxy
--rw-r--r--  2.0 unx    12646 b- defN 23-Sep-28 02:40 deployer/resources/template/my.cnf-8.0-xcluster
+-rw-r--r--  2.0 unx    12684 b- defN 24-May-08 03:43 deployer/resources/template/my.cnf-8.0-galaxy
+-rw-r--r--  2.0 unx    12646 b- defN 24-Apr-22 03:28 deployer/resources/template/my.cnf-8.0-xcluster
 -rw-r--r--  2.0 unx      622 b- defN 22-Jul-04 02:46 deployer/sqlite/__init__.py
--rw-r--r--  2.0 unx     5922 b- defN 23-Sep-28 02:40 deployer/sqlite/dbapi.py
--rw-r--r--  2.0 unx     3181 b- defN 23-Sep-28 02:40 deployer/sqlite/sqlite_manager.py
+-rw-r--r--  2.0 unx     6895 b- defN 24-May-08 03:43 deployer/sqlite/dbapi.py
+-rw-r--r--  2.0 unx     3181 b- defN 24-Apr-22 03:28 deployer/sqlite/sqlite_manager.py
 -rw-r--r--  2.0 unx      622 b- defN 22-Mar-14 02:39 deployer/tests/__init__.py
 -rw-r--r--  2.0 unx      622 b- defN 22-Mar-14 02:39 deployer/tryout/__init__.py
 -rw-r--r--  2.0 unx     1201 b- defN 22-Mar-14 02:39 deployer/tryout/install.py
 -rw-r--r--  2.0 unx      622 b- defN 22-Mar-14 02:39 deployer/util/__init__.py
 -rw-r--r--  2.0 unx     3578 b- defN 23-Jun-18 05:48 deployer/util/file_manager.py
 -rw-r--r--  2.0 unx     2110 b- defN 22-Mar-14 02:39 deployer/util/mysql_manager.py
 -rw-r--r--  2.0 unx      784 b- defN 22-Mar-14 02:39 deployer/util/network_util.py
--rw-r--r--  2.0 unx     1494 b- defN 23-Sep-28 02:40 deployer/util/password_util.py
+-rw-r--r--  2.0 unx     1478 b- defN 24-May-08 03:43 deployer/util/password_util.py
 -rw-r--r--  2.0 unx     2376 b- defN 22-Mar-14 02:39 deployer/util/sqlite_manager.py
 -rw-r--r--  2.0 unx     2585 b- defN 22-Jan-03 07:42 deployer/util/yaml_util.py
 -rw-r--r--  2.0 unx      622 b- defN 22-Mar-14 02:39 deployer/xdb/__init__.py
--rw-r--r--  2.0 unx    23081 b- defN 24-Jan-10 01:39 deployer/xdb/xdb.py
--rw-r--r--  2.0 unx    11358 b- defN 24-Jan-10 01:42 pxd-0.6.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     4525 b- defN 24-Jan-10 01:42 pxd-0.6.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Jan-10 01:42 pxd-0.6.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       42 b- defN 24-Jan-10 01:42 pxd-0.6.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        9 b- defN 24-Jan-10 01:42 pxd-0.6.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     5101 b- defN 24-Jan-10 01:42 pxd-0.6.1.dist-info/RECORD
-60 files, 226348 bytes uncompressed, 72335 bytes compressed:  68.0%
+-rw-r--r--  2.0 unx    23327 b- defN 24-May-08 03:43 deployer/xdb/xdb.py
+-rw-r--r--  2.0 unx    11358 b- defN 24-May-08 05:42 pxd-0.7.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4525 b- defN 24-May-08 05:42 pxd-0.7.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-08 05:42 pxd-0.7.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       42 b- defN 24-May-08 05:42 pxd-0.7.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        9 b- defN 24-May-08 05:42 pxd-0.7.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     5212 b- defN 24-May-08 05:42 pxd-0.7.0.dist-info/RECORD
+61 files, 243233 bytes uncompressed, 74708 bytes compressed:  69.3%
```

## zipnote {}

```diff
@@ -87,14 +87,17 @@
 
 Filename: deployer/resources/__init__.py
 Comment: 
 
 Filename: deployer/resources/download/scripts/load_image.sh
 Comment: 
 
+Filename: deployer/resources/download/scripts/polardbx-version.sh
+Comment: 
+
 Filename: deployer/resources/sql/gms_init.sql
 Comment: 
 
 Filename: deployer/resources/sql/sqlite_init.sql
 Comment: 
 
 Filename: deployer/resources/template/my-8.0.cnf
@@ -156,26 +159,26 @@
 
 Filename: deployer/xdb/__init__.py
 Comment: 
 
 Filename: deployer/xdb/xdb.py
 Comment: 
 
-Filename: pxd-0.6.1.dist-info/LICENSE
+Filename: pxd-0.7.0.dist-info/LICENSE
 Comment: 
 
-Filename: pxd-0.6.1.dist-info/METADATA
+Filename: pxd-0.7.0.dist-info/METADATA
 Comment: 
 
-Filename: pxd-0.6.1.dist-info/WHEEL
+Filename: pxd-0.7.0.dist-info/WHEEL
 Comment: 
 
-Filename: pxd-0.6.1.dist-info/entry_points.txt
+Filename: pxd-0.7.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: pxd-0.6.1.dist-info/top_level.txt
+Filename: pxd-0.7.0.dist-info/top_level.txt
 Comment: 
 
-Filename: pxd-0.6.1.dist-info/RECORD
+Filename: pxd-0.7.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## deployer/pxd.py

```diff
@@ -13,15 +13,15 @@
 #   limitations under the License.
 
 import click
 
 from deployer.config.config import setup_pxd_context, Config
 from deployer.download.polardbx_download import download_polardbx_packages
 from deployer.pxc.polardbx_manager import create_tryout_pxc, list_all_pxc, delete_pxc, cleanup_all_pxc, create_full_pxc, \
-    print_pxd_version, check_pxc
+    print_pxd_version, check_pxc, upgrade_pxc
 
 import warnings
 
 warnings.filterwarnings("ignore")
 
 @click.group()
 def main():
@@ -126,18 +126,28 @@
 @click.option("-r", "--repo", default="", help="Target repo for download images, for example registry:5000")
 @click.option("-i", "--image_list", default="", help="image list file, if specified, override the default images list")
 @click.option("-d", "--dest", default="", help="dest directory for generated install packages")
 def download(env, arch, repo, image_list, dest):
     download_polardbx_packages(env, arch, repo, image_list, dest)
 
 
+@click.command(help="Upgrade polardb-x version, support components: cn, dn, cdc, gms")
+@click.argument("name", default=None)
+@click.option("-t", "--type", default="cn", help='component need to upgrade, support values: [cn, dn, cdc, gms, columnar]')
+@click.option("-i", "--image", default="", help='component image')
+def upgrade(name, type, image):
+    setup_pxd_context()
+    upgrade_pxc(name, type, image)
+
+
 main.add_command(tryout)
 main.add_command(create)
 main.add_command(list)
 main.add_command(cleanup)
 main.add_command(delete)
 main.add_command(version)
 main.add_command(check)
 main.add_command(download)
+main.add_command(upgrade)
 
 if __name__ == '__main__':
     main()
```

## deployer/version.txt

```diff
@@ -1,4 +1,4 @@
 [default]
-version = 0.6.1
-commit = 3512607
+version = 0.7.0
+commit = 697d126
```

## deployer/config/config.py

```diff
@@ -27,18 +27,20 @@
     _instance = None
 
     DOCKER_REPO_URL = "polardbx/"
 
     CN_IMAGE_NAME = "polardbx-sql"
     DN_IMAGE_NAME = "polardbx-engine-2.0"
     CDC_IMAGE_NAME = "polardbx-cdc"
+    COLUMNAR_IMAGE_NAME = "polardbx-col"
 
     CN_IMAGE_VERSION = 'latest'
     DN_IMAGE_VERSION = "latest"
     CDC_IMAGE_VERSION = "latest"
+    COLUMNAR_IMAGE_VERSION = "latest"
 
     CN_TOOL_IMAGE_NAME = "polardbx-init"
     CN_TOOL_IMAGE_VERSION = 'latest'
 
     DN_TOOL_IMAGE_NAME = "xstore-tools"
     DN_TOOL_IMAGE_VERSION = "latest"
 
@@ -104,14 +106,18 @@
     def dn_tool_image(self):
         return f'{self.DOCKER_REPO_URL}{self.DN_TOOL_IMAGE_NAME}:{self.DN_TOOL_IMAGE_VERSION}'
 
     @property
     def cdc_image(self):
         return f'{self.DOCKER_REPO_URL}{self.CDC_IMAGE_NAME}:{self.CDC_IMAGE_VERSION}'
 
+    @property
+    def columnar_image(self):
+        return f'{self.DOCKER_REPO_URL}{self.COLUMNAR_IMAGE_NAME}:{self.COLUMNAR_IMAGE_VERSION}'
+
     @staticmethod
     def host_network_support():
         """
         Docker for mac is run on a virtual machine, so only 'bridge' mode is supported
         :return: Return false is platform is Darwin, otherwise return true.
         """
         if Config.instance().run_host == '127.0.0.1':
@@ -162,15 +168,15 @@
         return "arm" in Config.host_arch()
 
     @staticmethod
     def rpc_protocol_version():
         return Config.instance().RPCProtocolVersion
 
     @staticmethod
-    def dn_passwork_key():
+    def dn_password_key():
         return Config.instance().DN_PASSWORD_KEY
 
 
 def setup_pxd_context():
     setup_pxd_working_dir()
     setup_logging()
     setup_metadb()
```

## deployer/pxc/polardbx_cluster.py

```diff
@@ -26,14 +26,15 @@
 
 import click
 import docker
 from humanfriendly import parse_size
 from retrying import retry
 
 import deployer.core.docker_manager as DockerManager
+from deployer._repo import pxd_working_dir
 from deployer.config.config import Config
 from deployer.constant import constant
 from deployer.constant.constant import PXC_ROOT_ACCOUNT, STORAGE_KIND_GMS, STORAGE_KIND_DN, \
     STORAGE_TYPE_GALAXY_LEADER_ONLY, STORAGE_TYPE_GALAXY_PAXOS
 from deployer.core.flow import Flow
 from deployer.decorator.decorators import pxc_create_task
 from deployer.pxc.gms_consts import SERVER_INFO_DATA_ID_FORMAT, STORAGE_INFO_DATA_ID_FORMAT, CONFIG_DATA_ID_FORMAT, \
@@ -51,16 +52,15 @@
 CN_DEFAULT_PARAMS = {
     "CONN_POOL_MAX_POOL_SIZE": "500",
     "max_prepared_stmt_count": "500000",
 }
 
 
 def _extract_resources(topology, role):
-    gms_or_dn = (role == 'gms' or role == 'dn')
-    cpu_limit = 16 if gms_or_dn else 2
+    cpu_limit = 16
     mem_limit = 4294967296
     logger.info("extract resources for %s" % role)
     if 'resources' not in topology[role]:
         logger.info("no resources in %s" % role)
         return cpu_limit, mem_limit
 
     logger.info("topology info: %s" % str(topology[role]['resources']))
@@ -69,53 +69,62 @@
 
     if 'mem_limit' in topology[role]['resources']:
         mem_limit = parse_size(topology[role]['resources']['mem_limit'], binary=True)
 
     logger.info("cpu: %s, mem: %s" % (str(cpu_limit), str(mem_limit)))
     return cpu_limit, mem_limit
 
+
 class PolarDBXCluster:
 
     def __init__(self, pxc_name, cn_replica=0, cn_version=None, dn_replica=0, dn_version=None, cdc_replica=0,
-                 cdc_version=None, leader_only=True, hosts=['127.0.0.1'], mem_limit='4294967296', topology=None):
+                 cdc_version=None, columnar_replica=0, columnar_version=None, columnar_engine="OSS",
+                 leader_only=True, hosts=['127.0.0.1'], mem_limit='4294967296', topology=None):
         self.pxc_name = pxc_name
         self.pxc_status = 'pending'
         self.cn_replica = cn_replica
         self.cn_version = cn_version
         self.dn_replica = dn_replica
         self.dn_version = dn_version
         self.cdc_replica = cdc_replica
         self.cdc_version = cdc_version
+        self.columnar_replica = columnar_replica
+        self.columnar_version = columnar_version
+        self.columnar_engine = columnar_engine
         self.leader_only = leader_only
 
         self.gms_image = None
         self.cn_image = None
         self.dn_image = None
         self.cdc_image = None
 
         self.gms = None
         self.dn_list = []
         self.cn_list = []
         self.cdc_list = []
+        self.columnar_list = []
 
         self.root_account = None
         self.root_password = None
         self.mem_limit = mem_limit
         self.hosts = hosts
         self.topology = topology
         self.error = None
-        self.password_key = random_str(16)
+        self.password_key = Config.instance().dn_password_key() if Config.instance().dn_password_key() != '' \
+            else random_str(16)
 
         # cpuset and memory related params
         self.cn_cpu_cores = []
         self.cn_cpu_mems = []
         self.dn_cpu_cores_group = []
         self.dn_cpu_mems_group = []
         self.cdc_cpu_cores = []
         self.cdc_cpu_mems = []
+        self.columnar_cpu_cores = []
+        self.colunmar_cpu_mems = []
 
         self.dn_engine = 'galaxy'
         self.dn_engine_version = '8.0'
         self.gms_engine = 'galaxy'
         self.gms_engine_version = '8.0'
 
         self.create_tasks = [
@@ -127,15 +136,16 @@
             self._init_gms_schema,
             self._create_root_account,
             self._create_dn,
             self._insert_dn_list_into_gms,
             self._create_cn_containers,
             self._wait_container_running,
             self._create_cdc_containers,
-            self._finish_create_pxc
+            self._create_columnar_containers,
+            self._finish_create_pxc,
         ]
 
     def create(self):
         """
         Create a PolarDB-X cluster according to input params.
         """
         logger.info("start create")
@@ -157,15 +167,15 @@
             self.gms_image = Config.instance().dn_image
             self.cn_image = Config.instance().cn_image
             self.dn_image = Config.instance().dn_image
             self.cdc_image = Config.instance().cdc_image
 
             if self.cn_replica > 0:
                 self.gms = Xdb(self.pxc_name + '-gms', pxc_name=self.pxc_name, xdb_type='gms', version=self.dn_version,
-                            leader_only=self.leader_only)
+                               leader_only=self.leader_only)
 
             for i in range(self.cn_replica):
                 self.cn_list.append(PolarDBXCN(self.pxc_name, self.cn_version, self.gms))
             for i in range(self.dn_replica):
                 xdb = Xdb(self.pxc_name + '-dn-' + str(i), pxc_name=self.pxc_name, xdb_type='dn',
                           version=self.dn_version, leader_only=self.leader_only)
                 self.dn_list.append(xdb)
@@ -191,14 +201,17 @@
 
         if 'dn' in topology['cluster']:
             self.parse_dn_topology(topology)
 
         if 'cdc' in topology['cluster']:
             self.parse_cdc_topology(topology)
 
+        if 'columnar' in topology['cluster']:
+            self.parse_columnar_topology(topology)
+
     def parse_cdc_topology(self, topology):
         self.cdc_replica = topology['cluster']['cdc']['replica']
         if 'image' in topology['cluster']['cdc']:
             self.cdc_image = topology['cluster']['cdc']['image']
         else:
             self.cdc_image = Config.instance().cdc_image
         if self.cdc_replica == 0:
@@ -217,14 +230,44 @@
                 self.cdc_cpu_cores.append(cdc_cpuset)
                 cdc.cpusets = cdc_cpuset
             if 'memsets' in topology['cluster']['cdc']:
                 cdc_memset = topology['cluster']['cdc']['memsets'][i]['mem']
                 self.cdc_cpu_mems.append(cdc_memset)
                 cdc.memsets = cdc_memset
 
+    def parse_columnar_topology(self, topology):
+        self.columnar_replica = topology['cluster']['columnar']['replica']
+        if 'image' in topology['cluster']['columnar']:
+            self.columnar_image = topology['cluster']['columnar']['image']
+        else:
+            self.columnar_image = Config.instance().cdc_image
+
+        if self.columnar_replica == 0:
+            return
+
+        if 'engine' in topology['cluster']['columnar']:
+            self.columnar_engine = topology['cluster']['columnar']['engine']
+
+        columnar_cpu_limit, columnar_mem_limit = _extract_resources(topology['cluster'], 'columnar')
+        for i in range(self.columnar_replica):
+            columnar_host = topology['cluster']['columnar']['nodes'][i]['host']
+            self.hosts.append(columnar_host)
+            columnar = PolarDBXColumnar(self.pxc_name, self.cn_version, self.gms,
+                                        host=columnar_host, cpu_limit=columnar_cpu_limit,
+                                        mem_limit=columnar_mem_limit, engine=self.columnar_engine)
+            self.columnar_list.append(columnar)
+            if 'cpusets' in topology['cluster']['columnar']:
+                columnar_cpuset = topology['cluster']['columnar']['cpusets'][i]['cpu']
+                self.columnar_cpu_cores.append(columnar_cpuset)
+                columnar.cpusets = columnar_cpuset
+            if 'memsets' in topology['cluster']['columnar']:
+                columnar_memset = topology['cluster']['columnar']['memsets'][i]['mem']
+                self.columnar_cpu_mems.append(columnar_memset)
+                columnar.memsets = columnar_memset
+
     def parse_dn_topology(self, topology):
         if 'image' in topology['cluster']['dn']:
             self.dn_image = topology['cluster']['dn']['image']
         else:
             self.dn_image = Config.instance().dn_image
 
         self.dn_replica = topology['cluster']['dn']['replica']
@@ -313,28 +356,14 @@
 
     @pxc_create_task(task_name="pull images")
     def _pull_polardbx_related_images(self):
         if not Config.pull_latest_images():
             logger.info("Skip pull latest images")
             return
 
-        def _pull_images(host, image_list):
-            for image in image_list:
-                if not image:
-                    continue
-                click.echo("Pull image: %s at %s" % (image, host))
-                client = DockerManager.get_client(host)
-                click.echo("\n")
-                for info in client.api.pull(image, stream=True, decode=True):
-                    if 'id' in info:
-                        progress = info['progress'] if 'progress' in info else ''
-                        click.echo(info['id'] + ":" + info['status'] + ' ' + progress)
-                    else:
-                        click.echo(info['status'])
-
         max_workers = min(len(self.hosts), 8)
         images_list = [self.dn_image,
                        Config.instance().dn_tool_image]
         if self.cn_replica > 0:
             images_list.append(self.cn_image)
             images_list.append(Config.instance().cn_tool_image)
         if self.cdc_replica > 0:
@@ -489,14 +518,17 @@
     @retry(stop_max_attempt_number=5, wait_fixed=2000, retry_on_result=retry_if_result_none)
     def _start_cn_container(self, cn):
         try:
             client = DockerManager.get_client(cn.host)
             ports = cn.generate_ports()
             export_ports = cn.generate_export_ports()
             volumes = cn.generate_volumes()
+            if len(self.columnar_list) > 0:
+                nfs_dir = f'{pxd_working_dir}/nfs/'
+                volumes[nfs_dir] = {"bind": "/home/admin/polardbx-external-disk", "mode": "rw"}
             envs = cn.generate_envs(self.password_key, self.dn_engine)
             entrypoint = '/home/admin/entrypoint.sh 20'
             if self.dn_engine == 'xcluster':
                 entrypoint = 'bash -c "/home/admin/basic_init/init.sh /home/admin/app.sh"'
 
             if Config.host_network_support():
                 for log in client.containers.run(
@@ -580,27 +612,75 @@
                                               cpuset_mems=cdc.memsets
                                               )
 
             dbapi.update_container(self.pxc_name, container,
                                    host=cdc.host, role='cdc-engine',
                                    volumes=json.dumps(volumes), ports=json.dumps(ports), envs=json.dumps(envs))
 
+    @pxc_create_task(task_name='create columnar containers', task_type="enterprise")
+    def _create_columnar_containers(self):
+        if len(self.columnar_list) == 0:
+            logger.info("columnar list is empty, does not need to create")
+            return
+
+        for columnar in self.columnar_list:
+            client = DockerManager.get_client(columnar.host)
+            ports = columnar.generate_ports()
+            volumes = columnar.generate_volumes()
+
+            envs = columnar.generate_envs(self.cn_list, self.root_account, self.root_password, self.password_key)
+
+            container = client.containers.run(self.columnar_image,
+                                              command="",
+                                              detach=True,
+                                              mem_limit=columnar.mem_limit,
+                                              entrypoint="",
+                                              privileged=True,
+                                              environment=envs,
+                                              volumes=volumes,
+                                              name=columnar.name,
+                                              network_mode='host' if Config.instance().host_network_support() else 'bridge',
+                                              cpuset_cpus=columnar.cpusets,
+                                              cpuset_mems=columnar.memsets
+                                              )
+
+            dbapi.update_container(self.pxc_name, container,
+                                   host=columnar.host, role='columnar-engine',
+                                   volumes=json.dumps(volumes), ports=json.dumps(ports), envs=json.dumps(envs))
+
     @retry(stop_max_attempt_number=20, wait_fixed=5000, retry_on_result=retry_if_result_none)
     def _wait_pxc_ready(self):
         for cn in self.cn_list:
             try:
                 logger.info("try probe cn: %s" % str(cn))
                 MySQLManager.execute_cn_sql(cn, self.root_password, 'show storage')
                 return True
             except Exception as e:
                 logger.info("failed to check pxc status, cn: %s,  ex: %s" % (str(cn), str(e)))
                 return None
 
         return True
 
+    @pxc_create_task(task_name='create file storage', task_type="enterprise")
+    def _create_file_storage(self):
+        if len(self.columnar_list) < 1:
+            return Flow.SUCCESS
+
+        self._wait_pxc_ready()
+
+        if self.columnar_engine == 'oss':
+            pass
+        elif self.columnar_engine == 'local_storage':
+            pass
+        elif self.columnar_engine == 'external_storage':
+            pass
+        else:
+            logger.error("Specified columnar engine is not supported")
+            return Flow.FAIL
+
     @pxc_create_task(task_name='wait PolarDB-X ready')
     def _finish_create_pxc(self):
         try:
             self._wait_pxc_ready()
         except Exception as ex:
             logger.warn("pxc status check failed, but not block. %s" % str(ex))
         self.pxc_status = 'running'
@@ -681,15 +761,14 @@
             results = []
             for xdb in xdbs:
                 results.append(executor.submit(check_and_repair_dn, xdb, repair))
 
             for f in as_completed(results):
                 logger.info(f.result())
 
-
     @staticmethod
     def check_cn_alive(pxc_name, repair=False):
         cn_containers = dbapi.list_cn_containers_by_pxc(pxc_name)
 
         for container in cn_containers:
             container_name = container['container_name']
             container_id = container['container_id']
@@ -709,14 +788,34 @@
                     if not restart_result:
                         click.echo("restart cn fail, container: %s, host: %s" % (container_name, container_host))
                     else:
                         click.echo("restart cn success, container: %s, host: %s" % (container_name, container_host))
             else:
                 click.echo("cn: %s host: %s is OK!" % (container_name, container_host))
 
+    @staticmethod
+    def upgrade(pxc_name, type, image):
+        if type in ('cn', 'cdc', 'columnar'):
+            containers = dbapi.list_containers_by_pxc_and_type(pxc_name, type)
+            for container in containers:
+                restart_container_with_new_image(container, image)
+        elif type in ('gms', 'dn'):
+            xdbs = dbapi.list_xdbs_by_type(pxc_name, type)
+            for xdb in xdbs:
+                click.echo("prepare upgrade xdb: %s" % xdb['xdb_name'])
+                containers = dbapi.list_containers_by_pxc_and_type(xdb['xdb_name'], type)
+                containers = reorder_xdb_containers_for_restart(xdb['xdb_name'], containers)
+                if containers is None:
+                    return
+                for container in containers:
+                    click.echo(container['container_name'])
+                    restart_container_with_new_image(container, image)
+        else:
+            click.echo("unknown component type: %s" % type)
+
 
 class PolarDBXCN:
     existing_ip_pots = {}
 
     def __init__(self, pxc_name, version, gms, host='127.0.0.1', cpu_limit=1, mem_limit='2147483648'):
         self.version = version
         self.pxc_name = pxc_name
@@ -827,14 +926,15 @@
 
 
 class PolarDBXCDC:
 
     def __init__(self, pxc_name, version, gms, host='127.0.0.1', cpu_limit=1, mem_limit='2147483648'):
         self.pxc_name = pxc_name
         self.name = pxc_name + '-cdc-' + random_str(4)
+        self.daemon_port = random.randint(3000, 3300)
         self.version = version
         self.gms = gms
         self.host = host
         self.container_id = None
         self.container_ip = None
         self.cpu_limit = cpu_limit
         self.mem_limit = mem_limit
@@ -855,20 +955,36 @@
         leader = self.gms.leader_node
         leader_ip = leader.host if Config.instance().host_network_support() else leader.container_ip
         gms_jdbc_url = "jdbc:mysql://%s:%s/polardbx_meta_db?useSSL=false" % (leader_ip, leader.mysql_port)
         cn = cn_list[0]
         cn_ip = cn.host if Config.instance().host_network_support() else cn.container_ip
         polarx_jdbc_url = "jdbc:mysql://%s:%s/__cdc__?useSSL=false" % (cn_ip, cn.mysql_port)
 
+        common_ports = {
+            "ssh_port": "2200",
+            "access_port": "%s" % self.daemon_port,
+            "link": "0",
+            "cdc1_port": "6061",
+            "cdc2_port": "6062",
+            "cdc3_port": "6063",
+            "cdc4_port": "6064",
+            "cdc5_port": "6065",
+            "cdc6_port": "6066"
+        }
+
         envs = ['switchCloud=aliyun',
+                'topology_node_minsize=1',
                 'cluster_id=' + self.pxc_name,
                 'ins_id=' + self.name,
-                'daemonPort=3300',
+                'daemonPort=' + str(self.daemon_port),
+                'daemon_port=' + str(self.daemon_port),
                 'port={"' + self.name + '":{"ssh_port":[2200],"access_port":[3300],"link":[0],"cdc1_port":[6061],"cdc2_port":[6062],"cdc3_port":[6063],"cdc4_port":[6064],"cdc5_port":[6065],"cdc6_port":[6066]}}',
-                'cpu_cores=2',
+                'common_ports=' + json.dumps(common_ports),
+                'cpu_cores=' + str(self.cpu_limit),
+                'cpuCore=' + str(self.cpu_limit),
                 'mem_size=' + str(math.floor(int(self.mem_limit) / 1024 / 1024)),
                 'disk_size=10240',
                 'disk_quota=10240',
                 'metaDb_url=' + gms_jdbc_url,
                 'metaDb_username=' + self.gms.user_name,
                 'metaDb_password=' + self.gms.password,
                 'polarx_url=' + polarx_jdbc_url,
@@ -881,29 +997,186 @@
 
         if self.host != '127.0.0.1':
             envs.append("ins_ip=" + self.host)
 
         return envs
 
 
+class PolarDBXColumnar:
+
+    def __init__(self, pxc_name, version, gms, host='127.0.0.1', cpu_limit=1, mem_limit='2147483648',
+                 engine="OSS"):
+        self.pxc_name = pxc_name
+        self.name = pxc_name + '-columnar-' + random_str(4)
+        self.version = version
+        self.gms = gms
+        self.host = host
+        self.container_id = None
+        self.container_ip = None
+        self.cpu_limit = cpu_limit
+        self.mem_limit = mem_limit
+        self.engine = engine
+
+        self.cpusets = None
+        self.memsets = None
+
+    def generate_ports(self):
+        return {
+            '3007/tcp': 3007,
+            '3070/tcp': 3070}
+
+    def generate_volumes(self):
+        columnar_log_dir = f'{pxd_working_dir}/data/polarx-log/{self.name}'
+        nfs_dir = f'{pxd_working_dir}/nfs/'
+        volumes = {
+            columnar_log_dir: {"bind": "/home/admin/polardbx-columnar/logs", "mode": "rw"},
+            nfs_dir: {"bind": "/home/admin/polardbx-external-disk", "mode": "rw"}
+        }
+        self.create_volume_dirs_if_needed(volumes)
+        volumes.update({
+            "/etc/localtime": {"bind": "/etc/localtime", "mode": "ro"},
+            "/usr/share/zoneinfo": {"bind": "/usr/share/zoneinfo", "mode": "ro"}
+        })
+        return volumes
+
+    def create_volume_dirs_if_needed(self, volumes):
+        logger.info("try to mkdirs, host: %s, dirs: %s" % (self.host, volumes.keys()))
+        FileManager.mkdirs(self.host, volumes.keys())
+
+    def generate_envs(self, cn_list, pxc_root_account, pxc_root_password, password_key):
+        leader = self.gms.leader_node
+        leader_ip = leader.host if Config.instance().host_network_support() else leader.container_ip
+        gms_jdbc_url = "jdbc:mysql://%s:%s/polardbx_meta_db?useSSL=false" % (leader_ip, leader.mysql_port)
+        cn = cn_list[0]
+        cn_ip = cn.host if Config.instance().host_network_support() else cn.container_ip
+        polarx_jdbc_url = "jdbc:mysql://%s:%s/__cdc__?useSSL=false" % (cn_ip, cn.mysql_port)
+
+        envs = ['switchCloud=aliyun',
+                'cluster_id=' + self.pxc_name + 'columnar',
+                'ins_id=' + self.name,
+                'port={"' + self.name + '":{"ssh_port":[2200],"access_port":[3300],"link":[0],"cdc1_port":[6061],"cdc2_port":[6062],"cdc3_port":[6063],"cdc4_port":[6064],"cdc5_port":[6065],"cdc6_port":[6066]}}',
+                'cpu_cores=' + str(self.cpu_limit),
+                'cpuCore=' + str(self.cpu_limit),
+                'mem_size=' + str(math.floor(int(self.mem_limit) / 1024 / 1024)),
+                'disk_size=10240',
+                'disk_quota=10240',
+                'metaDb_url=' + gms_jdbc_url,
+                'metaDbAddr=%s:%s' % (leader_ip, leader.mysql_port),
+                'metaDbName=polardbx_meta_db',
+                'metaDbUser=' + self.gms.user_name,
+                'metaDbPasswd=' + PasswordUtil().encrypt(password_key, self.gms.password),
+                'metaDb_username=' + self.gms.user_name,
+                'metaDb_password=' + self.gms.password,
+                'metaDbXprotoPort=' + str(leader.polarx_port),
+                'storageDbXprotoPort=0',
+                'polarx_url=' + polarx_jdbc_url,
+                'polarx_username=' + pxc_root_account,
+                'polarx_password=' + pxc_root_password,
+                'dnPasswordKey=' + password_key,
+                'LANG=en_US.utf8',
+                'LC_ALL=en_US.utf8',
+                'columnar_ports={"columnar_port": "3070"}',
+                'cluster_type=COLUMNAR',
+                'daemon_port=3007',
+                'columnarPort=3070',
+                'columnar_engine=' + self.engine
+                ]
+
+        if self.host != '127.0.0.1':
+            envs.append("ins_ip=" + self.host)
+
+        return envs
+
+
 def stop_and_remove_container(host, container_id):
     client = DockerManager.get_client(host)
     try:
         container = client.containers.get(container_id)
         if container.status == 'running':
             container.stop()
         # remove docker container and its volumes
         container.remove(v=True, force=True)
     except docker.errors.NotFound:
         click.echo('container: %s is not existing at %s.' % (container_id, host))
 
 
+def restart_container_with_new_image(container: dict, new_image: str):
+    container_name = container['container_name']
+    container_id = container['container_id']
+    envs = json.loads(container['env'])
+    volumes = json.loads(container['local_volumes'])
+
+    host = container['host']
+    image, mem_limit, cpuset_cpus, cpuset_mems, network_mode, ports, entrypoint, command = \
+        query_container_infos(host, container_id)
+    if image == new_image:
+        click.echo("host: %s, container: %s is the new image, skip upgrade" % (host, container_name))
+        return
+
+    click.echo("Prepare upgrade container: %s" % container_name)
+    _pull_images(host, [new_image])
+
+    stop_and_remove_container(host, container_id)
+    client = DockerManager.get_client(host)
+    if network_mode == 'host':
+        new_container = client.containers.run(new_image,
+                                              detach=True,
+                                              privileged=True,
+                                              mem_limit=mem_limit,
+                                              volumes=volumes,
+                                              command=command,
+                                              entrypoint=entrypoint,
+                                              environment=envs,
+                                              name=container_name,
+                                              network_mode=network_mode,
+                                              cpuset_cpus=cpuset_cpus,
+                                              cpuset_mems=cpuset_mems
+                                              )
+    else:
+        new_container = client.containers.run(new_image,
+                                              detach=True,
+                                              privileged=True,
+                                              mem_limit=mem_limit,
+                                              volumes=volumes,
+                                              command=command,
+                                              entrypoint=entrypoint,
+                                              environment=envs,
+                                              name=container_name,
+                                              ports=ports,
+                                              cpuset_cpus=cpuset_cpus,
+                                              cpuset_mems=cpuset_mems
+                                              )
+    dbapi.update_container_id_and_ip(container_name, new_container.short_id,
+                                     new_container.attrs['NetworkSettings']['IPAddress'])
+    click.echo("Upgrade container: %s success" % container_name)
+
+
+def query_container_infos(host, container_id):
+    client = DockerManager.get_client(host)
+    try:
+        container = client.containers.get(container_id)
+        image = container.attrs['Config']['Image']
+        mem_limit = container.attrs['HostConfig']['Memory']
+        cpuset_cpus = container.attrs['HostConfig']['CpusetCpus']
+        cpuset_mems = container.attrs['HostConfig']['CpusetMems']
+        network_mode = container.attrs['HostConfig']['NetworkMode']
+        ports = container.attrs['NetworkSettings']['Ports']
+        entrypoint = container.attrs['Config']['Entrypoint']
+        command = container.attrs['Config']['Cmd']
+        return image, mem_limit, cpuset_cpus, cpuset_mems, network_mode, ports, entrypoint, command
+    except docker.errors.NotFound:
+        click.echo('container: %s is not existing at %s.' % (container_id, host))
+        return None
+
+
 def rm_volumes_if_needed(host, volumes):
     for dir in volumes.keys():
-        if "mysql" not in dir and "shared" not in dir and "polarx"  not in dir:
+        if "mysql" not in dir and "shared" not in dir and "polarx" not in dir:
+            continue
+        if "columnar" in dir:
             continue
         if FileManager.exists(host, dir):
             logger.info("rm directory: %s at: %s" % (dir, host))
             FileManager.rmdir(host, dir)
 
 
 def exec_cmd_for_cn(host, container_name, container_id, cmd):
@@ -957,7 +1230,42 @@
                                              cur_leader_container_id=container_id,
                                              cur_leader_container_name=container_name,
                                              expect_leader_container_name=expect_leader_container)
             if result:
                 click.echo("succeed to change leader for %s" % expect_leader_container)
             else:
                 click.echo("failed to change leader for %s" % expect_leader_container)
+
+
+def reorder_xdb_containers_for_restart(xdb_name, xdb_containers):
+    leader_container = None
+
+    for xdb_container in xdb_containers:
+        container_name = xdb_container['container_name']
+        container_id = xdb_container['container_id']
+        container_host = xdb_container['host']
+        role = query_container_role(container_host, container_name, container_id)
+        if role == constant.ROLE_LEADER:
+            leader_container = xdb_container
+
+    if not leader_container:
+        click.echo("can not find leader container for xdb: %s" % xdb_name)
+        return None
+
+    xdb_containers.remove(leader_container)
+    xdb_containers.append(leader_container)
+    return xdb_containers
+
+
+def _pull_images(host, image_list):
+    for image in image_list:
+        if not image:
+            continue
+        click.echo("Pull image: %s at %s" % (image, host))
+        client = DockerManager.get_client(host)
+        click.echo("\n")
+        for info in client.api.pull(image, stream=True, decode=True):
+            if 'id' in info:
+                progress = info['progress'] if 'progress' in info else ''
+                click.echo(info['id'] + ":" + info['status'] + ' ' + progress)
+            else:
+                click.echo(info['status'])
```

## deployer/pxc/polardbx_manager.py

```diff
@@ -93,14 +93,18 @@
 
             pxc = PolarDBXCluster(pxc_name, topology=data)
             pxc.create()
         except yaml.YAMLError as ex:
             click.echo("Please check yaml format, error: %s" % str(ex))
 
 
+def upgrade_pxc(name, type, image):
+    PolarDBXCluster.upgrade(name, type, image)
+
+
 def print_pxd_version():
     Config.instance().load_config()
     version_file = repo_dir.joinpath("deployer/version.txt")
     config = configparser.RawConfigParser()
     config.read(version_file)
     click.echo('pxd version: ' + config.get('default', 'version').strip())
     click.echo('commit id: ' + config.get('default', 'commit').strip())
```

## deployer/resources/template/my.cnf-8.0-galaxy

```diff
@@ -334,12 +334,13 @@
 tmp_table_size = 2097152
 transaction_alloc_block_size = 8192
 transaction_isolation = REPEATABLE-READ
 transaction_prealloc_size = 4096
 transaction_write_set_extraction = XXHASH64
 updatable_views_with_limit = YES
 wait_timeout = 28800
+consensuslog_revise=ON
 loose_optimizer_switch=index_merge=on,index_merge_union=on,index_merge_sort_union=on,index_merge_intersection=on,engine_condition_pushdown=on,index_condition_pushdown=on,mrr=on,mrr_cost_based=on,block_nested_loop=on,batched_key_access=off,materialization=on,semijoin=on,loosescan=on,firstmatch=on,subquery_materialization_cost_based=on,use_index_extensions=on,skip_scan=off
 tls_version=TLSv1.2,TLSv1.3
 
 [mysqld_safe]
 pid_file = /data/mysql/run/mysql.pid
```

## deployer/sqlite/dbapi.py

```diff
@@ -94,14 +94,24 @@
             'ports': kwargs['ports'],
             'envs': kwargs['envs']
         })
     except Exception as ex:
         logger.error("failed to update polardbx container record", ex)
 
 
+def update_container_id_and_ip(container_name, container_id, container_ip):
+    sql = """
+    update container set container_id=:container_id, container_ip=:container_ip where container_name=:container_name"""
+    SQLiteManager.execute_query(sql, {
+        'container_name': container_name,
+        'container_id': container_id,
+        'container_ip': container_ip
+    })
+
+
 def list_containers_by_pxc(pxc_name):
     sql = """select * from container where resource_name=:resource_name
     """
     containers = SQLiteManager.execute_query(sql, {
         'resource_name': pxc_name
     })
     return containers
@@ -110,23 +120,41 @@
     sql = """select * from container where container_type = 'cn-engine' and resource_name=:resource_name
     """
     containers = SQLiteManager.execute_query(sql, {
         'resource_name': pxc_name
     })
     return containers
 
+def list_containers_by_pxc_and_type(pxc_name, type):
+    sql = """select * from container where container_type = :container_type and resource_name=:resource_name
+    """
+    containers = SQLiteManager.execute_query(sql, {
+        'resource_name': pxc_name,
+        'container_type': type + '-engine'
+    })
+    return containers
+
 
 def list_xdbs_by_pxc(pxc_name):
     sql = """select * from polardbx_xdb where pxc_name=:pxc_name
     """
     xdbs = SQLiteManager.execute_query(sql, {
         'pxc_name': pxc_name
     })
     return xdbs
 
+def list_xdbs_by_type(pxc_name, xdb_type):
+    sql = """select * from polardbx_xdb where pxc_name=:pxc_name and xdb_type=:xdb_type
+    """
+    xdbs = SQLiteManager.execute_query(sql, {
+        'pxc_name': pxc_name,
+        'xdb_type': xdb_type
+    })
+    return xdbs
+
 
 def list_xdb_containers_by_names(xdb_names):
     sql = f"select * from container where resource_name in ({','.join(xdb_names)})"
     containers = SQLiteManager.execute_query(sql)
     return containers
 
 def list_xdb_containers_by_name(xdb_name):
```

## deployer/util/password_util.py

```diff
@@ -32,12 +32,12 @@
         cryptos = AES.new(key.encode('utf-8'), AES.MODE_ECB)
         decrpytBytes = base64.b64decode(data)
         meg = cryptos.decrypt(decrpytBytes).decode('utf-8')
         return meg[:-ord(meg[-1])]
 
 
 if __name__ == '__main__':
-    print(PasswordUtil().decrypt("HQlIoYbRinjMlsAZ", "0D9yHgkENcFF3wrLdRneDw=="))
+    print(PasswordUtil().encrypt("9cx2r2c2574ktbdb", "lpxlc4sd"))
 
 
 def random_str(count):
     return ''.join(secrets.choice(string.ascii_letters) for _ in range(count))
```

## deployer/xdb/xdb.py

```diff
@@ -17,14 +17,15 @@
 import os
 import random
 import secrets
 import string
 from pathlib import Path
 
 import click
+import docker
 from retrying import retry
 
 import deployer.constant.constant as constant
 import deployer.core.docker_manager as DockerManager
 from deployer._repo import pxd_working_dir
 from deployer.config.config import Config
 from deployer.core.flow import Flow
@@ -227,14 +228,15 @@
                                          )
             logger.info("xstore tools logs")
             for log in logs:
                 logger.info("%s" % log)
 
     @xdb_create_task(task_name='start xdb containers')
     def _start_xdb_container(self):
+        nofile_limit = docker.types.Ulimit(name='nofile', soft=655535, hard=655535)
         for node in self.nodes:
             volumes = self._generate_xdb_volumes(node)
             self._create_volume_dirs_if_needed(volumes)
             volumes.update(self._generate_system_volumes())
             self._write_pod_info(node)
             ports = self._generate_xdb_export_ports(node)
             command = self._generate_xdb_container_command()
@@ -246,26 +248,28 @@
                                                   entrypoint='',
                                                   privileged=True,
                                                   environment=env, working_dir='/', name=node.name,
                                                   network_mode='host',
                                                   mem_limit=mem_limit,
                                                   cpuset_cpus=node.cpusets,
                                                   cpuset_mems=node.memsets,
-                                                  memswap_limit=-1
+                                                  memswap_limit=-1,
+                                                  ulimits=[nofile_limit]
                                                   )
             else:
                 container = client.containers.run(self.engine_image, command, volumes=volumes, detach=True,
                                                   entrypoint='',
                                                   privileged=True,
                                                   environment=env, working_dir='/', name=node.name,
                                                   ports=ports,
                                                   mem_limit=mem_limit,
                                                   cpuset_cpus=node.cpusets,
                                                   cpuset_mems=node.memsets,
-                                                  memswap_limit=-1
+                                                  memswap_limit=-1,
+                                                  ulimits=[nofile_limit]
                                                   )
             node.container_id = container.short_id
             dbapi.update_container(self.name, container,
                                    host=node.host, role=self.xdb_type + '-engine',
                                    volumes=json.dumps(volumes), ports=json.dumps(ports), envs=json.dumps(env))
 
     def _generate_xdb_volumes(self, node):
```

## Comparing `pxd-0.6.1.dist-info/LICENSE` & `pxd-0.7.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pxd-0.6.1.dist-info/METADATA` & `pxd-0.7.0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pxd
-Version: 0.6.1
+Version: 0.7.0
 Summary: This is a tool to download and install PolarDB-X
 Author: polardbx
 Author-email: vettal.wd@alibaba-inc.com
 Platform: all
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
```

## Comparing `pxd-0.6.1.dist-info/RECORD` & `pxd-0.7.0.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 deployer/__init__.py,sha256=KOPBclqMVKfeguAHku6DZHy0C95GLGko03sSt87DBaY,622
 deployer/_repo.py,sha256=VMggl-rwEKx9t-J_GI9RG4qLj2SaXKiAmAxj1coEzkE,790
 deployer/logging.yaml,sha256=2LLVJUa2gjfxf-WZT9l2doNyMflxftLJ0TaKa2L5A9I,733
-deployer/pxd.py,sha256=onoAFdhFYgnZ7kBvLjc_uyhawy1frTiKcyksGuBoEpg,7178
-deployer/version.txt,sha256=WEmJ5HAqPj8Go2ZyYd-uXm7XnrNWvDxtqKSZub0RcOI,44
+deployer/pxd.py,sha256=55GYfaOI2CPgsL-wFh_61L6mnr3fVTa_87AIEpooBW8,7626
+deployer/version.txt,sha256=5o1ZtUxNeetafikLfllV46PhJWYapxR8uX9NgDTiXjw,44
 deployer/config/__init__.py,sha256=KOPBclqMVKfeguAHku6DZHy0C95GLGko03sSt87DBaY,622
-deployer/config/config.py,sha256=vJbXoOnUAfGcKWX2iMH4nvRCF0tkZraZsvP9Cqum9Bk,5308
+deployer/config/config.py,sha256=dJrrHmO2Jk688DrctnseOGabUaKiqQtRPgIWwUNMehs,5529
 deployer/config/log_config.py,sha256=wOyxszPQtN4i--ePMSU2MNUm6KW8IYfA0rMSRezTTyo,1313
 deployer/config/metadb_config.py,sha256=Uv4M1azARRYIk09qPD4AXZgzFNzNLm4h2d0AEdEMsks,1080
 deployer/constant/__init__.py,sha256=KOPBclqMVKfeguAHku6DZHy0C95GLGko03sSt87DBaY,622
 deployer/constant/constant.py,sha256=z39ZTUSAw6H1BJHjs6ixtL1y9Zc-EhFgx2tgTh90xQM,1195
 deployer/constant/table_field.py,sha256=qcrYPTeJbz-rhAhxqhlbLz0hA-LPakLplHqkweAlqEc,715
 deployer/core/__init__.py,sha256=KOPBclqMVKfeguAHku6DZHy0C95GLGko03sSt87DBaY,622
 deployer/core/context.py,sha256=19Jf75z0vmu5Q27QnkzCo6PXVEXCgI8Mrr9Yff8Fw5g,991
@@ -19,42 +19,43 @@
 deployer/decorator/decorators.py,sha256=yW_TPlyQ2AKMhdTN3N8FY2a-VHpJEQcs8OIWPpptXg0,2376
 deployer/download/__init__.py,sha256=KOPBclqMVKfeguAHku6DZHy0C95GLGko03sSt87DBaY,622
 deployer/download/constant.py,sha256=r8PAS4deCjpPqxukj5v2txr7HVpaQeF--Pzmgfb15Io,1219
 deployer/download/polardbx_download.py,sha256=bU4NQ4YJ97djyy7mb9M1JRMJB6emDRTN24KW0Q28bO0,10463
 deployer/pcn/__init__.py,sha256=KOPBclqMVKfeguAHku6DZHy0C95GLGko03sSt87DBaY,622
 deployer/pxc/__init__.py,sha256=KOPBclqMVKfeguAHku6DZHy0C95GLGko03sSt87DBaY,622
 deployer/pxc/gms_consts.py,sha256=swwK1mhn7-uHWcXNilbm0efksyumoYszkwyP79BoD9Y,1070
-deployer/pxc/polardbx_cluster.py,sha256=IneA0XZia6TreHxROzn4P42KH9096eVnXnDwShD31fU,43795
-deployer/pxc/polardbx_manager.py,sha256=jzUPnYUIWlaadIEQVp8PxwFSSPROrRcHe4nfBqWF9Gc,4175
+deployer/pxc/polardbx_cluster.py,sha256=gLDctIJ5WPalSJhkryjlRDuViZTjF28LsTqBDygUcwg,58096
+deployer/pxc/polardbx_manager.py,sha256=FJf8I1YqN3cSOuiza28ocDEl54kTexK6K0qvNA2CJa8,4260
 deployer/pxc/polardbx_topology.py,sha256=Bb3sUS25ZczHb8MVVE3CgskBOxJC8MH7NO9ubQhLFvc,930
 deployer/pxc/pxc_user.py,sha256=cNmzwcib2t3Bdx2NTgMfQy-brNnFfya-wyTrPk7cSk4,1257
 deployer/resources/__init__.py,sha256=KOPBclqMVKfeguAHku6DZHy0C95GLGko03sSt87DBaY,622
 deployer/resources/download/scripts/load_image.sh,sha256=X7ZheHT5dCfyndmfp0ZV_MDWICy0-pu9ZSAhfdXYqiQ,260
+deployer/resources/download/scripts/polardbx-version.sh,sha256=RFTfy21bs1xLoZY0yyVrLVRyuOuw62CtV7n7MwmbKzY,493
 deployer/resources/sql/gms_init.sql,sha256=i_z249y27cMYewtS72cemWcKF0X6FlGk9c7vid_20xs,7330
 deployer/resources/sql/sqlite_init.sql,sha256=aRlR_zoiAio4NXz385WfrCz2nVy647f3VpP6YDfqbbk,2137
 deployer/resources/template/my-8.0.cnf,sha256=4Z2L1g97__AF-Eb-eEzNeeZCcRX8N2da-tUqTFMHbVU,4872
 deployer/resources/template/my.cnf,sha256=WfpblNPohW0zKQQ_bnhTAOZ9sbppqo59ClISiR6BgV0,4614
 deployer/resources/template/my.cnf-5.7,sha256=Lj8Ea5Gdq7t7szLSjIDRRZY_F8ETzhJH1OosJCZsMFo,9148
 deployer/resources/template/my.cnf-5.7-xcluster,sha256=eUTIeggn2EgkmqiH_HjLAJb35VbJPHhJlByzorLuvoI,9169
-deployer/resources/template/my.cnf-8.0-galaxy,sha256=P8x0RnPulHzldabO6sjDTQq_x0EeQybG47TEuM6Wu1Q,12661
+deployer/resources/template/my.cnf-8.0-galaxy,sha256=2QP50ANwaCvvMgPPb6ZKnaaS-CGbK2iCDXlDMSfuIxk,12684
 deployer/resources/template/my.cnf-8.0-xcluster,sha256=ZfsgLuoPG19fiWOTABvyV9upFnLKYNJ9VJmEPFAOhss,12646
 deployer/sqlite/__init__.py,sha256=KOPBclqMVKfeguAHku6DZHy0C95GLGko03sSt87DBaY,622
-deployer/sqlite/dbapi.py,sha256=gsQnJOAxa4OB6bXk97LpthkyV5Xz5FJBcfnjs4Czejw,5922
+deployer/sqlite/dbapi.py,sha256=N79qfecex1j-UMmuqt3dsfCve2BGAIV49EBnfkHm_Bo,6895
 deployer/sqlite/sqlite_manager.py,sha256=XAUuhQWIg_JSiKmaYwoMKMReoE0mP5QAZoGsbIO4Sy0,3181
 deployer/tests/__init__.py,sha256=KOPBclqMVKfeguAHku6DZHy0C95GLGko03sSt87DBaY,622
 deployer/tryout/__init__.py,sha256=KOPBclqMVKfeguAHku6DZHy0C95GLGko03sSt87DBaY,622
 deployer/tryout/install.py,sha256=lSrL_WYbfmiFIHwlVG0yvBNj6JuKwBqmQxenH5Vol6M,1201
 deployer/util/__init__.py,sha256=KOPBclqMVKfeguAHku6DZHy0C95GLGko03sSt87DBaY,622
 deployer/util/file_manager.py,sha256=aquq6ALCZJSsQv4gEBMJRmldf3YgpGEgp0VDLxveyP0,3578
 deployer/util/mysql_manager.py,sha256=TRnHe70bIjGbEnFsGjQAc9MY9wUMvRrFI7CFHRFUR4Q,2110
 deployer/util/network_util.py,sha256=n1vT1RicjJ3Mb75ygZq8yzgYBOS60XXjKyLmKNok_co,784
-deployer/util/password_util.py,sha256=Qcxr2kJ0gOA5Z2NO50m0NTt05v6gbwnM5WE1cUyIMXM,1494
+deployer/util/password_util.py,sha256=Zi1U8kL7PunMruLAxHAENsTj-rvTLLrQqxgs2q1AzqE,1478
 deployer/util/sqlite_manager.py,sha256=8_ZvNi0UGBHyhJfngb0PYr_fA3_Wgp_jXqNkXSvqSO4,2376
 deployer/util/yaml_util.py,sha256=ndvgjVg0op0fU4p-Yk38rLnniRTK-Z2F0s4bOgFw6vA,2585
 deployer/xdb/__init__.py,sha256=KOPBclqMVKfeguAHku6DZHy0C95GLGko03sSt87DBaY,622
-deployer/xdb/xdb.py,sha256=18bU2Q2uE9RP20qGO4UHuzw_R1jBHUvS__8Ra_HcmA0,23081
-pxd-0.6.1.dist-info/LICENSE,sha256=z8d0m5b2O9McPEK1xHG_dWgUBT6EfBDz6wA0F7xSPTA,11358
-pxd-0.6.1.dist-info/METADATA,sha256=nmM_ZY0T8DHsuba6jNnEIvoBPFCx5Z35l6KxW7An-fM,4525
-pxd-0.6.1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-pxd-0.6.1.dist-info/entry_points.txt,sha256=uiz9xUO94F_TRBe74tU2MryX9VySXWgNofPuc-wvZvE,42
-pxd-0.6.1.dist-info/top_level.txt,sha256=TwI8aV0C_V0Au2_1ouGA25hHdF5_e7_RjipVDY1w0lk,9
-pxd-0.6.1.dist-info/RECORD,,
+deployer/xdb/xdb.py,sha256=b1NdzjcRyVpdsg95I4yIdokko9hGAUXJ2yL1yZFQDK4,23327
+pxd-0.7.0.dist-info/LICENSE,sha256=z8d0m5b2O9McPEK1xHG_dWgUBT6EfBDz6wA0F7xSPTA,11358
+pxd-0.7.0.dist-info/METADATA,sha256=IGtZkpDntzsVCvMOzPIZuMdwGfcJggRu6SxRjGuX_mA,4525
+pxd-0.7.0.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+pxd-0.7.0.dist-info/entry_points.txt,sha256=uiz9xUO94F_TRBe74tU2MryX9VySXWgNofPuc-wvZvE,42
+pxd-0.7.0.dist-info/top_level.txt,sha256=TwI8aV0C_V0Au2_1ouGA25hHdF5_e7_RjipVDY1w0lk,9
+pxd-0.7.0.dist-info/RECORD,,
```

