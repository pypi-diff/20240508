# Comparing `tmp/snapctl-0.4.4.tar.gz` & `tmp/snapctl-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snapctl-0.4.4.tar", max compression
+gzip compressed data, was "snapctl-0.4.5.tar", max compression
```

## Comparing `snapctl-0.4.4.tar` & `snapctl-0.4.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     9181 2023-10-05 21:59:19.573785 snapctl-0.4.4/README.md
--rw-r--r--   0        0        0      423 2023-10-11 21:33:12.422337 snapctl-0.4.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-17 15:14:31.467451 snapctl-0.4.4/snapctl/__init__.py
--rw-r--r--   0        0        0       47 2023-03-24 21:28:04.581292 snapctl-0.4.4/snapctl/__main__.py
--rw-r--r--   0        0        0        0 2023-04-11 05:58:03.721459 snapctl-0.4.4/snapctl/commands/__init__.py
--rw-r--r--   0        0        0    13511 2023-10-05 19:30:03.967244 snapctl-0.4.4/snapctl/commands/byogs.py
--rw-r--r--   0        0        0    14509 2023-10-11 21:29:04.638146 snapctl-0.4.4/snapctl/commands/byosnap.py
--rw-r--r--   0        0        0     5095 2023-10-05 19:30:03.968653 snapctl-0.4.4/snapctl/commands/snapend.py
--rw-r--r--   0        0        0        0 2023-08-23 20:47:44.465873 snapctl-0.4.4/snapctl/config/__init__.py
--rw-r--r--   0        0        0      339 2023-10-11 21:33:16.112563 snapctl-0.4.4/snapctl/config/constants.py
--rw-r--r--   0        0        0      171 2023-08-23 20:47:44.467633 snapctl-0.4.4/snapctl/config/endpoints.py
--rw-r--r--   0        0        0     2032 2023-10-05 19:30:03.969907 snapctl-0.4.4/snapctl/config/hashes.py
--rw-r--r--   0        0        0    10239 2023-10-11 21:23:40.788607 snapctl-0.4.4/snapctl/main.py
--rw-r--r--   0        0        0        0 2023-04-11 05:59:24.957443 snapctl-0.4.4/snapctl/types/__init__.py
--rw-r--r--   0        0        0       60 2023-04-11 04:34:25.684424 snapctl-0.4.4/snapctl/types/definitions.py
--rw-r--r--   0        0        0        0 2023-04-11 06:00:21.052854 snapctl-0.4.4/snapctl/utils/__init__.py
--rw-r--r--   0        0        0      321 2023-03-10 06:45:50.660269 snapctl-0.4.4/snapctl/utils/echo.py
--rw-r--r--   0        0        0     1039 2023-10-05 19:30:03.971410 snapctl-0.4.4/snapctl/utils/helper.py
--rw-r--r--   0        0        0     9659 1970-01-01 00:00:00.000000 snapctl-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0     9922 2023-10-17 22:12:29.303596 snapctl-0.4.5/README.md
+-rw-r--r--   0        0        0      423 2023-10-17 22:12:29.304427 snapctl-0.4.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-17 15:14:31.467451 snapctl-0.4.5/snapctl/__init__.py
+-rw-r--r--   0        0        0       47 2023-03-24 21:28:04.581292 snapctl-0.4.5/snapctl/__main__.py
+-rw-r--r--   0        0        0        0 2023-04-11 05:58:03.721459 snapctl-0.4.5/snapctl/commands/__init__.py
+-rw-r--r--   0        0        0    13557 2023-10-17 22:12:29.306048 snapctl-0.4.5/snapctl/commands/byogs.py
+-rw-r--r--   0        0        0    14555 2023-10-17 22:12:29.306740 snapctl-0.4.5/snapctl/commands/byosnap.py
+-rw-r--r--   0        0        0     7771 2023-10-17 22:12:29.307813 snapctl-0.4.5/snapctl/commands/snapend.py
+-rw-r--r--   0        0        0        0 2023-08-23 20:47:44.465873 snapctl-0.4.5/snapctl/config/__init__.py
+-rw-r--r--   0        0        0      378 2023-10-17 22:12:29.308488 snapctl-0.4.5/snapctl/config/constants.py
+-rw-r--r--   0        0        0      171 2023-08-23 20:47:44.467633 snapctl-0.4.5/snapctl/config/endpoints.py
+-rw-r--r--   0        0        0     2300 2023-10-17 22:12:29.309174 snapctl-0.4.5/snapctl/config/hashes.py
+-rw-r--r--   0        0        0    10936 2023-10-17 22:12:29.309621 snapctl-0.4.5/snapctl/main.py
+-rw-r--r--   0        0        0        0 2023-04-11 05:59:24.957443 snapctl-0.4.5/snapctl/types/__init__.py
+-rw-r--r--   0        0        0       60 2023-04-11 04:34:25.684424 snapctl-0.4.5/snapctl/types/definitions.py
+-rw-r--r--   0        0        0        0 2023-04-11 06:00:21.052854 snapctl-0.4.5/snapctl/utils/__init__.py
+-rw-r--r--   0        0        0      321 2023-03-10 06:45:50.660269 snapctl-0.4.5/snapctl/utils/echo.py
+-rw-r--r--   0        0        0     1039 2023-10-05 19:30:03.971410 snapctl-0.4.5/snapctl/utils/helper.py
+-rw-r--r--   0        0        0    10400 1970-01-01 00:00:00.000000 snapctl-0.4.5/PKG-INFO
```

### Comparing `snapctl-0.4.4/README.md` & `snapctl-0.4.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -238,37 +238,56 @@
 #### 1. snapend help
 See all the supported commands
 ```bash {{ title: 'Snapend - Help' }}
 # Help for the byogs command
 snapctl snapend --help
 ```
 
-#### 2. Snapend SDK download
-Download a Snapser SDK for your snapend
-```bash {{ title: 'Snapend - Download SDK' }}
+#### 2. Snapend Downloads
+Download SDKs and Protos for your Snapend
+```bash {{ title: 'Snapend - Downloads' }}
 # Help for the byogs command
-snapctl snapend download-sdk --help
+snapctl snapend download --help
 
-# Download your Snapend SDK
+# Download your Snapend SDK and Protos
 # $snapend_id = Cluster Id
-# $sdk_type = One of the supported SDK names: unity, unreal, roblox, godot, cocos, ios-objc, ios-swift, android-java, android-kotlin, web-ts, web-js, csharp, cpp, lua, ts, go, python, kotlin, java, c, node, js, perl, php, closure, ruby, rust.
+# $category = client-sdk, server-sdk, protos
+# $sdk_type = One of the supported SDK names:
+# client-sdk(unity, unreal, roblox, godot, cocos, ios-objc, ios-swift, android-java, android-kotlin, web-ts, web-js),
+# server-sdk(csharp, cpp, lua, ts, go, python, kotlin, java, c, node, js, perl, php, closure, ruby, rust),
+# protos(go)
 # Example:
-# snapctl snapend download gx5x6bc0 --type unity
-snapctl snapend download-sdk $snapend_id --type $sdk_type
+# snapctl snapend download gx5x6bc0 --category client-sdk --type unity
+snapctl snapend download $snapend_id --category $category --type $sdk_type
 ```
 
 #### 3. Update Snapend BYOSnap or BYOGs versions
 Update your BYOSnap or BYOGs versions for the Snapend
 ```bash {{ title: 'Snapend - Update BYOSnap or BYOGs' }}
 # Help for the byogs command
 snapctl snapend update --help
 
-# Download your Snapend SDK
+# Update your Snapend with new BYOSnaps and BYOGs
 # $snapend_id = Cluster Id
 # $byosnaps = Comma separated list of BYOSnap ids and version.
 # $byogs = Comma separated list of BYOGs fleet name, id and version.
+# --blocking = (Optional) This makes sure the CLI waits till your Snapend is live.
 # Note atleast one of the two needs to be present
 # Example:
-# snapctl snapend update --byosnaps service-1:v1.0.0,service-2:v1.0.0 --byogs my-fleet-one:gs-1:v0.0.1,my-fleet-two:gs-2:v0.0.4
-snapctl snapend update --byosnaps $byosnaps --byogs $byogs
+# snapctl snapend update gx5x6bc0 --byosnaps byosnap-service-1:v1.0.0,byosnap-service--2:v1.0.0 --byogs byogs-fleet-one:gs-1:v0.0.1,my-fleet-two:gs-2:v0.0.4
+# snapctl snapend update gx5x6bc0 --byosnaps byosnap-service-1:v1.0.0,byosnap-service--2:v1.0.0 --byogs byogs-fleet-one:gs-1:v0.0.1,my-fleet-two:gs-2:v0.0.4 --blocking
+snapctl snapend update $snapend_id --byosnaps $byosnaps --byogs $byogs --blocking
+```
+
+#### 4. Get the Snapend state
+Get the Snapend state
+```bash {{ title: 'Snapend - Get state' }}
+# Help for the byogs command
+snapctl snapend state --help
+
+# Get the Snapend state
+# $snapend_id = Cluster Id
+# Example:
+# snapctl snapend state gx5x6bc0
+snapctl snapend state $snapend_id
 ```
```

### Comparing `snapctl-0.4.4/snapctl/commands/byogs.py` & `snapctl-0.4.5/snapctl/commands/byogs.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,26 +16,26 @@
 class ByoGs:
   ID_PREFIX = 'byogs-'
   SUBCOMMANDS = ['create', 'publish-image', 'publish-version']
   PLATFORMS = ['linux/amd64']
   LANGUAGES = ['go', 'python', 'ruby', 'c#', 'c++', 'rust', 'java', 'node']
   DEFAULT_BUILD_PLATFORM = 'linux/amd64'
 
-  def __init__(self, subcommand: str, base_url: str, api_key: str, sid: str, name: str, desc: str, platform: str, language: str, tag: str, path: Union[str, None], dockerfile: str, version: Union[str, None], http_port: Union[int, None]) -> None:
+  def __init__(self, subcommand: str, base_url: str, api_key: str, sid: str, name: str, desc: str, platform: str, language: str, tag: Union[str, None], path: Union[str, None], dockerfile: str, version: Union[str, None], http_port: Union[int, None]) -> None:
     self.subcommand: str = subcommand
     self.base_url: str = base_url
     self.api_key: str = api_key
     self.sid: str = sid
     self.name: str = name
     self.desc: str = desc
     self.platform: str = platform
     self.language: str = language
     self.token: Union[str, None] = get_composite_token(base_url, api_key, 'byogs', {'service_id': sid}) if subcommand != 'create' else None
     self.token_parts: Union[list, None] = ByoGs.get_token_values(self.token) if self.token is not None else None
-    self.tag: str = tag
+    self.tag: Union[str, None] = tag
     self.path: Union[str, None] = path
     self.dockerfile: str = dockerfile
     self.version: Union[str, None] = version
     self.http_port: Union[int, None] = http_port
 
   @staticmethod
   def get_token_values(token: str) -> None | list:
@@ -82,15 +82,15 @@
         response['msg'] = f"Invalid platform. Valid platforms are {', '.join(ByoGs.PLATFORMS)}."
         return response
     else:
       if self.token_parts is None:
         response['msg'] = 'Invalid token. Please reach out to your support team'
         return response
       # Check tag
-      if len(self.tag.split()) > 1 or len(self.tag) > 25:
+      if self.tag is None or len(self.tag.split()) > 1 or len(self.tag) > 25:
         response['msg'] = f"Tag should be a single word with maximum of 25 characters"
         return response
       if self.subcommand == 'publish-image':
         if not self.path:
           response['msg'] = f"Missing path"
           return response
         # Check path
```

### Comparing `snapctl-0.4.4/snapctl/commands/byosnap.py` & `snapctl-0.4.5/snapctl/commands/byosnap.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,26 +16,26 @@
 class ByoSnap:
   ID_PREFIX = 'byosnap-'
   SUBCOMMANDS = ['create', 'publish-image', 'publish-version', 'upload-docs']
   PLATFORMS = ['linux/arm64', 'linux/amd64']
   LANGUAGES = ['go', 'python', 'ruby', 'c#', 'c++', 'rust', 'java', 'node']
   DEFAULT_BUILD_PLATFORM = 'linux/arm64'
 
-  def __init__(self, subcommand: str, base_url: str, api_key: str, sid: str, name: str, desc: str, platform: str, language: str, tag: str, path: Union[str, None], dockerfile: str, prefix: str, version: Union[str, None], http_port: Union[int, None]) -> None:
+  def __init__(self, subcommand: str, base_url: str, api_key: str, sid: str, name: str, desc: str, platform: str, language: str, tag: Union[str, None], path: Union[str, None], dockerfile: str, prefix: str, version: Union[str, None], http_port: Union[int, None]) -> None:
     self.subcommand: str = subcommand
     self.base_url: str = base_url
     self.api_key: str = api_key
     self.sid: str = sid
     self.name: str = name
     self.desc: str = desc
     self.platform: str = platform
     self.language: str = language
     self.token: Union[str, None] = get_composite_token(base_url, api_key, 'byosnap', {'service_id': sid}) if subcommand != 'create' else None
     self.token_parts: Union[list, None] = ByoSnap.get_token_values(self.token) if self.token is not None else None
-    self.tag: str = tag
+    self.tag: Union[str, None] = tag
     self.path: Union[str, None] = path
     self.dockerfile: str = dockerfile
     self.prefix: str = prefix
     self.version: Union[str, None] = version
     self.http_port: Union[int, None] = http_port
 
   @staticmethod
@@ -84,15 +84,15 @@
         return response
     else:
       # Check the token
       if self.token_parts is None:
         response['msg'] = 'Invalid token. Please reach out to your support team.'
         return response
       # Check tag
-      if len(self.tag.split()) > 1 or len(self.tag) > 25:
+      if self.tag is None or len(self.tag.split()) > 1 or len(self.tag) > 25:
         response['msg'] = f"Tag should be a single word with maximum of 25 characters"
         return response
       if self.subcommand == 'publish-image':
         if not self.path:
           response['msg'] = f"Missing required parameter: path"
           return response
         # Check path
```

### Comparing `snapctl-0.4.4/snapctl/config/hashes.py` & `snapctl-0.4.5/snapctl/config/hashes.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,28 @@
-SDK_TYPES = {
+CLIENT_SDK_TYPES: dict[str, dict[str, str]] = {
     'unity': {
-        'type': 'csharp-netcore',
+        'type': 'csharp',
         'subtype': 'unity',
     },
     'unreal': {
         'type': 'cpp-ue4',
         'subtype': 'unreal',
     },
     'roblox': {
         'type': 'lua',
         'subtype': 'roblox',
     },
-    'godot': {
+    'godot-csharp': {
         'type': 'csharp',
         'subtype': 'godot',
     },
+    'godot-cpp': {
+        'type': 'cpp-restsdk',
+        'subtype': 'godot',
+    },
     'cocos': {
         'type': 'cpp-restsdk',
         'subtype': 'cocos',
     },
     'ios-objc': {
         'type': 'objc',
         'subtype': 'ios',
@@ -39,16 +43,19 @@
         'type': 'typescript-axios',
         'subtype': 'web',
     },
     'web-js': {
         'type': 'javascript',
         'subtype': 'web',
     },
-    'csharp': {
-        'type': 'csharp-netcore',
+}
+
+SERVER_SDK_TYPES: dict[str, dict[str, str]] = {
+  'csharp': {
+        'type': 'csharp',
         'subtype': '',
     },
     'cpp': {
         'type': 'cpp-restsdk',
         'subtype': '',
     },
     'lua': {
@@ -91,20 +98,27 @@
         'type': 'perl',
         'subtype': '',
     },
     'php': {
         'type': 'php',
         'subtype': '',
     },
-    'closure': {
-        'type': 'closure',
+    'clojure': {
+        'type': 'clojure',
         'subtype': '',
     },
     'ruby': {
         'type': 'ruby',
         'subtype': '',
     },
     'rust': {
         'type': 'rust',
         'subtype': '',
     },
+}
+
+PROTOS_TYPES: dict[str, dict[str, str]] = {
+  'go': {
+        'type': 'go',
+        'subtype': '',
+    },
 }
```

### Comparing `snapctl-0.4.4/snapctl/main.py` & `snapctl-0.4.5/snapctl/main.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import configparser
 import os
 import typer
 
 from snapctl.commands.byosnap import ByoSnap
 from snapctl.commands.byogs import ByoGs
 from snapctl.commands.snapend import Snapend
-from snapctl.config.constants import API_KEY, CONFIG_FILE_MAC, CONFIG_FILE_WIN, DEFAULT_PROFILE, VERSION
+from snapctl.config.constants import API_KEY, CONFIG_FILE_MAC, CONFIG_FILE_WIN, DEFAULT_PROFILE, VERSION, SNAPCTL_SUCCESS, SNAPCTL_ERROR
 from snapctl.config.endpoints import ENDPOINTS
-from snapctl.config.hashes import SDK_TYPES
+from snapctl.config.hashes import CLIENT_SDK_TYPES, SERVER_SDK_TYPES, PROTOS_TYPES
 from snapctl.types.definitions import ResponseType
 from snapctl.utils.echo import error, success, info
 from sys import platform
 from typing import Union
 
 app = typer.Typer()
 
@@ -70,27 +70,27 @@
       if platform == 'win32':
         conf_file = os.path.expandvars(CONFIG_FILE_WIN)
       else:
         conf_file = os.path.expanduser(CONFIG_FILE_MAC)
       error(f'Invalid profile. Please check your snap config file at {conf_file} and try again.')
     else:
       error('API Key not found. Please generate a new one from the Snapser dashboard.')
-    raise typer.Exit()
+    raise typer.Exit(SNAPCTL_ERROR)
   # Set the context
   ctx.obj['version'] = VERSION
   ctx.obj['api_key'] = api_key
   ctx.obj['profile'] = profile if profile else DEFAULT_PROFILE
   ctx.obj['base_url'] = get_base_url(api_key)
 
 
 # Presently in typer this is the only way we can expose the `--version`
 def version_callback(value: bool = True):
   if value:
-    typer.echo(f"Snapctl version: {VERSION}")
-    raise typer.Exit()
+    success(f"Snapctl version: {VERSION}")
+    raise typer.Exit(SNAPCTL_SUCCESS)
 
 @app.callback()
 def common(
     ctx: typer.Context,
     version: bool = typer.Option(
       None, "--version",
       help="Get the Snapctl version.",
@@ -104,15 +104,15 @@
     # Note this executes only when the user runs a command and not for --help or --version
     if platform == 'win32':
       config_file_path = os.path.expandvars(CONFIG_FILE_WIN)
     else:
       config_file_path = os.path.expanduser(CONFIG_FILE_MAC)
     if not os.path.isfile(config_file_path):
       error(f'Snapser configuration file not found at {config_file_path} ')
-      raise typer.Exit()
+      raise typer.Exit(SNAPCTL_ERROR)
     # Set the main context this always sets the default context
     set_context_callback(ctx)
 
 ######### TYPER COMMANDS #########
 @app.command()
 def validate(
   profile: str = typer.Option(None, "--profile", help="Profile to use.", callback=set_context_callback),
@@ -148,20 +148,21 @@
   """
     Bring your own snap commands
   """
   # token = get_composite_token(ctx.obj['base_url'], ctx.obj['api_key'], ctx.command.name, {'service_id': sid})
   byosnap: ByoSnap = ByoSnap(subcommand, ctx.obj['base_url'], ctx.obj['api_key'], sid, name, desc, platform, language, tag, path, docker_file, prefix, version, http_port)
   validate_input_response: ResponseType = byosnap.validate_input()
   if validate_input_response['error']:
-    return error(validate_input_response['msg'])
+    error(validate_input_response['msg'])
+    raise typer.Exit(SNAPCTL_ERROR)
   command_method = subcommand.replace('-', '_')
-  info(command_method)
   method: function = getattr(byosnap, command_method)
   if not method():
-    return error(f"BYOSnap {subcommand} failed")
+    error(f"BYOSnap {subcommand} failed")
+    raise typer.Exit(SNAPCTL_ERROR)
   success(f"BYOSnap {subcommand} complete")
 
 @app.command()
 def byogs(
   ctx: typer.Context,
   # Required fields
   subcommand: str = typer.Argument(..., help="BYOGs Subcommands: " + ", ".join(ByoGs.SUBCOMMANDS) + "."),
@@ -184,41 +185,47 @@
 ) -> None:
   """
     Bring your own game server commands
   """
   byogs: ByoGs = ByoGs(subcommand, ctx.obj['base_url'], ctx.obj['api_key'], sid, name, desc, platform, language, tag, path, docker_file, version, http_port)
   validate_input_response: ResponseType = byogs.validate_input()
   if validate_input_response['error']:
-    return error(validate_input_response['msg'])
+    error(validate_input_response['msg'])
+    raise typer.Exit(SNAPCTL_ERROR)
   command_method = subcommand.replace('-', '_')
   method: function = getattr(byogs, command_method)
   if not method():
-    return error(f"BYOGs {subcommand} failed")
+    error(f"BYOGs {subcommand} failed")
+    raise typer.Exit(SNAPCTL_ERROR)
   success(f"BYOGs {subcommand} complete")
 
 @app.command()
 def snapend(
   ctx: typer.Context,
   # Required fields
   subcommand: str = typer.Argument(..., help="Snapend Subcommands: " + ", ".join(Snapend.SUBCOMMANDS) + "."),
   snapend_id: str = typer.Argument(..., help="Snapend Id"),
-  # download-sdk
-  sdk_type: str = typer.Option(None, "--type", help="(req: download-sdk) SDK Types: " + ", ".join(SDK_TYPES.keys()) + "."),
-  path: Union[str, None] = typer.Option(None, "--path", help="(req: download-sdk) Path to save the SDK"),
-  snaps: Union[str, None] = typer.Option(None, "--snaps", help="(optional: download-sdk) Comma separated list of snap ids to include in the SDK"),
+  # download
+  category: str = typer.Option(None, "--category", help="(req: download) Category of the Download: " + ", ".join(Snapend.DOWNLOAD_TYPES) + "."),
+  download_type: str = typer.Option(None, "--type", help="(req: download) SDK Types: client-sdk(" + ", ".join(CLIENT_SDK_TYPES.keys()) + ") server-sdk(" + ", ".join(SERVER_SDK_TYPES.keys()) + ") protos(" + ", ".join(PROTOS_TYPES.keys()) + ")"),
+  path: Union[str, None] = typer.Option(None, "--path", help="(req: download) Path to save the SDK"),
+  snaps: Union[str, None] = typer.Option(None, "--snaps", help="(optional: download) Comma separated list of snap ids to include in the SDK"),
   # update
   byosnaps: str = typer.Option(None, "--byosnaps", help="(optional: update) Comma separated list of BYOSnap ids and versions. Eg: service-1:v1.0.0,service-2:v1.0.0"),
   byogs: str = typer.Option(None, "--byogs", help="(optional: update) Comma separated list of BYOGs fleet name, ids and versions. Eg: fleet-1:service-1:v1.0.0,fleet-2:service-2:v1.0.0"),
+  blocking: bool = typer.Option(False, "--blocking", help="(optional: update) Set to true if you want to wait for the update to complete before returning."),
   profile: Union[str, None] = typer.Option(None, "--profile", help="Profile to use.", callback=set_context_callback),
 ) -> None:
   """
     Snapend commands
   """
-  snapend: Snapend = Snapend(subcommand, ctx.obj['base_url'], ctx.obj['api_key'], snapend_id, sdk_type, path, snaps, byosnaps, byogs)
+  snapend: Snapend = Snapend(subcommand, ctx.obj['base_url'], ctx.obj['api_key'], snapend_id, category, download_type, path, snaps, byosnaps, byogs, blocking)
   validate_input_response: ResponseType = snapend.validate_input()
   if validate_input_response['error']:
-    return error(validate_input_response['msg'])
+    error(validate_input_response['msg'])
+    raise typer.Exit(SNAPCTL_ERROR)
   command_method = subcommand.replace('-', '_')
   method: function = getattr(snapend, command_method)
   if not method():
-    return error(f"Snapend {subcommand} failed")
+    error(f"Snapend {subcommand} failed")
+    raise typer.Exit(SNAPCTL_ERROR)
   success(f"Snapend {subcommand} complete")
```

### Comparing `snapctl-0.4.4/snapctl/utils/helper.py` & `snapctl-0.4.5/snapctl/utils/helper.py`

 * *Files identical despite different names*

### Comparing `snapctl-0.4.4/PKG-INFO` & `snapctl-0.4.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snapctl
-Version: 0.4.4
+Version: 0.4.5
 Summary: Snapser CLI Tool
 Author: Ajinkya Apte
 Author-email: aj@snapser.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -253,38 +253,57 @@
 #### 1. snapend help
 See all the supported commands
 ```bash {{ title: 'Snapend - Help' }}
 # Help for the byogs command
 snapctl snapend --help
 ```
 
-#### 2. Snapend SDK download
-Download a Snapser SDK for your snapend
-```bash {{ title: 'Snapend - Download SDK' }}
+#### 2. Snapend Downloads
+Download SDKs and Protos for your Snapend
+```bash {{ title: 'Snapend - Downloads' }}
 # Help for the byogs command
-snapctl snapend download-sdk --help
+snapctl snapend download --help
 
-# Download your Snapend SDK
+# Download your Snapend SDK and Protos
 # $snapend_id = Cluster Id
-# $sdk_type = One of the supported SDK names: unity, unreal, roblox, godot, cocos, ios-objc, ios-swift, android-java, android-kotlin, web-ts, web-js, csharp, cpp, lua, ts, go, python, kotlin, java, c, node, js, perl, php, closure, ruby, rust.
+# $category = client-sdk, server-sdk, protos
+# $sdk_type = One of the supported SDK names:
+# client-sdk(unity, unreal, roblox, godot, cocos, ios-objc, ios-swift, android-java, android-kotlin, web-ts, web-js),
+# server-sdk(csharp, cpp, lua, ts, go, python, kotlin, java, c, node, js, perl, php, closure, ruby, rust),
+# protos(go)
 # Example:
-# snapctl snapend download gx5x6bc0 --type unity
-snapctl snapend download-sdk $snapend_id --type $sdk_type
+# snapctl snapend download gx5x6bc0 --category client-sdk --type unity
+snapctl snapend download $snapend_id --category $category --type $sdk_type
 ```
 
 #### 3. Update Snapend BYOSnap or BYOGs versions
 Update your BYOSnap or BYOGs versions for the Snapend
 ```bash {{ title: 'Snapend - Update BYOSnap or BYOGs' }}
 # Help for the byogs command
 snapctl snapend update --help
 
-# Download your Snapend SDK
+# Update your Snapend with new BYOSnaps and BYOGs
 # $snapend_id = Cluster Id
 # $byosnaps = Comma separated list of BYOSnap ids and version.
 # $byogs = Comma separated list of BYOGs fleet name, id and version.
+# --blocking = (Optional) This makes sure the CLI waits till your Snapend is live.
 # Note atleast one of the two needs to be present
 # Example:
-# snapctl snapend update --byosnaps service-1:v1.0.0,service-2:v1.0.0 --byogs my-fleet-one:gs-1:v0.0.1,my-fleet-two:gs-2:v0.0.4
-snapctl snapend update --byosnaps $byosnaps --byogs $byogs
+# snapctl snapend update gx5x6bc0 --byosnaps byosnap-service-1:v1.0.0,byosnap-service--2:v1.0.0 --byogs byogs-fleet-one:gs-1:v0.0.1,my-fleet-two:gs-2:v0.0.4
+# snapctl snapend update gx5x6bc0 --byosnaps byosnap-service-1:v1.0.0,byosnap-service--2:v1.0.0 --byogs byogs-fleet-one:gs-1:v0.0.1,my-fleet-two:gs-2:v0.0.4 --blocking
+snapctl snapend update $snapend_id --byosnaps $byosnaps --byogs $byogs --blocking
+```
+
+#### 4. Get the Snapend state
+Get the Snapend state
+```bash {{ title: 'Snapend - Get state' }}
+# Help for the byogs command
+snapctl snapend state --help
+
+# Get the Snapend state
+# $snapend_id = Cluster Id
+# Example:
+# snapctl snapend state gx5x6bc0
+snapctl snapend state $snapend_id
 ```
```

