# Comparing `tmp/rc3-0.0.3.tar.gz` & `tmp/rc3-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rc3-0.0.3.tar", last modified: Tue May  7 00:50:11 2024, max compression
+gzip compressed data, was "rc3-0.0.4.tar", last modified: Wed May  8 19:50:09 2024, max compression
```

## Comparing `rc3-0.0.3.tar` & `rc3-0.0.4.tar`

### file list

```diff
@@ -1,154 +1,152 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 00:50:11.111009 rc3-0.0.3/
--rw-rw-rw-   0        0        0     3141 2024-05-06 19:59:38.000000 rc3-0.0.3/.gitignore
--rw-rw-rw-   0        0        0     1087 2024-05-06 20:36:33.000000 rc3-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     9394 2024-05-07 00:50:11.110012 rc3-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     7344 2024-05-06 23:46:57.000000 rc3-0.0.3/README.md
--rw-rw-rw-   0        0        0      822 2024-05-06 20:35:45.000000 rc3-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0      475 2024-05-06 20:07:47.000000 rc3-0.0.3/rc3.iml
--rw-rw-rw-   0        0        0       42 2024-05-07 00:50:11.111009 rc3-0.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-07 00:50:10.927996 rc3-0.0.3/src/
-drwxrwxrwx   0        0        0        0 2024-05-07 00:50:10.947983 rc3-0.0.3/src/rc3/
--rw-rw-rw-   0        0        0      246 2024-05-06 19:59:38.000000 rc3-0.0.3/src/rc3/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-07 00:50:10.961975 rc3-0.0.3/src/rc3/archive/
--rw-rw-rw-   0        0        0        0 2024-05-06 19:59:38.000000 rc3-0.0.3/src/rc3/archive/__init__.py
--rw-rw-rw-   0        0        0      406 2024-05-06 20:00:31.000000 rc3-0.0.3/src/rc3/archive/cmd_home.py
--rw-rw-rw-   0        0        0      637 2024-05-06 20:00:31.000000 rc3-0.0.3/src/rc3/archive/cmd_root.py
--rw-rw-rw-   0        0        0     1125 2024-05-06 20:00:31.000000 rc3-0.0.3/src/rc3/archive/cmd_subs.py
--rw-rw-rw-   0        0        0     1864 2024-05-06 22:41:56.000000 rc3-0.0.3/src/rc3/cli.py
-drwxrwxrwx   0        0        0        0 2024-05-07 00:50:10.972968 rc3-0.0.3/src/rc3/commands/
--rw-rw-rw-   0        0        0        0 2024-05-06 19:59:38.000000 rc3-0.0.3/src/rc3/commands/__init__.py
--rw-rw-rw-   0        0        0     3415 2024-05-06 22:52:43.000000 rc3-0.0.3/src/rc3/commands/cmd_collection.py
--rw-rw-rw-   0        0        0     5463 2024-05-06 20:00:31.000000 rc3-0.0.3/src/rc3/commands/cmd_environment.py
--rw-rw-rw-   0        0        0      524 2024-05-06 19:59:38.000000 rc3-0.0.3/src/rc3/commands/cmd_hello.py
--rw-rw-rw-   0        0        0     2559 2024-05-06 23:00:33.000000 rc3-0.0.3/src/rc3/commands/cmd_init.py
--rw-rw-rw-   0        0        0     2133 2024-05-06 20:00:31.000000 rc3-0.0.3/src/rc3/commands/cmd_list.py
--rw-rw-rw-   0        0        0     4322 2024-05-06 20:00:31.000000 rc3-0.0.3/src/rc3/commands/cmd_request.py
--rw-rw-rw-   0        0        0     9063 2024-05-06 20:00:31.000000 rc3-0.0.3/src/rc3/commands/cmd_send.py
--rw-rw-rw-   0        0        0      452 2024-05-06 20:00:31.000000 rc3-0.0.3/src/rc3/commands/cmd_settings.py
-drwxrwxrwx   0        0        0        0 2024-05-07 00:50:10.983961 rc3-0.0.3/src/rc3/common/
--rw-rw-rw-   0        0        0        0 2024-05-06 19:59:39.000000 rc3-0.0.3/src/rc3/common/__init__.py
--rw-rw-rw-   0        0        0      524 2024-05-06 19:59:39.000000 rc3-0.0.3/src/rc3/common/config_helper.py
--rw-rw-rw-   0        0        0      869 2024-05-06 22:59:13.000000 rc3-0.0.3/src/rc3/common/data_helper.py
--rw-rw-rw-   0        0        0      936 2024-05-06 19:59:39.000000 rc3-0.0.3/src/rc3/common/decorators.py
--rw-rw-rw-   0        0        0     2670 2024-05-06 20:00:31.000000 rc3-0.0.3/src/rc3/common/env_helper.py
--rw-rw-rw-   0        0        0     1364 2024-05-06 22:52:57.000000 rc3-0.0.3/src/rc3/common/inherit_helper.py
--rw-rw-rw-   0        0        0    10401 2024-05-06 23:04:59.000000 rc3-0.0.3/src/rc3/common/json_helper.py
--rw-rw-rw-   0        0        0     2423 2024-05-06 20:00:31.000000 rc3-0.0.3/src/rc3/common/print_helper.py
--rw-rw-rw-   0        0        0       86 2024-05-06 19:59:39.000000 rc3-0.0.3/src/rc3/common/rc_globals.py
-drwxrwxrwx   0        0        0        0 2024-05-07 00:50:10.985960 rc3-0.0.3/src/rc3/data/
--rw-rw-rw-   0        0        0        0 2024-05-06 19:59:39.000000 rc3-0.0.3/src/rc3/data/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-07 00:50:10.986959 rc3-0.0.3/src/rc3/data/collection/
-drwxrwxrwx   0        0        0        0 2024-05-07 00:50:10.988957 rc3-0.0.3/src/rc3/data/collection/environments/
--rw-rw-rw-   0        0        0      270 2024-05-06 19:59:39.000000 rc3-0.0.3/src/rc3/data/collection/environments/dev.json
--rw-rw-rw-   0        0        0      300 2024-05-06 19:59:39.000000 rc3-0.0.3/src/rc3/data/collection/environments/localhost.json
-drwxrwxrwx   0        0        0        0 2024-05-07 00:50:11.006946 rc3-0.0.3/src/rc3/data/collection/examples/
--rw-rw-rw-   0        0        0      240 2024-05-06 19:59:39.000000 rc3-0.0.3/src/rc3/data/collection/examples/example_Auth_Basic.request
--rw-rw-rw-   0        0        0      907 2024-05-06 19:59:39.000000 rc3-0.0.3/src/rc3/data/collection/examples/example_Auth_Bearer.request
--rw-rw-rw-   0        0        0      953 2024-05-06 19:59:39.000000 rc3-0.0.3/src/rc3/data/collection/examples/example_Auth_Token.request
--rw-rw-rw-   0        0        0      429 2024-05-06 19:59:39.000000 rc3-0.0.3/src/rc3/data/collection/examples/example_Extract_JsonPath.request
--rw-rw-rw-   0        0        0      448 2024-05-06 19:59:39.000000 rc3-0.0.3/src/rc3/data/collection/examples/example_Extract_Regex.request
--rw-rw-rw-   0        0        0      183 2024-05-06 19:59:39.000000 rc3-0.0.3/src/rc3/data/collection/examples/example_GET.request
--rw-rw-rw-   0        0        0      792 2024-05-06 19:59:39.000000 rc3-0.0.3/src/rc3/data/collection/examples/example_KitchenSink.request
--rw-rw-rw-   0        0        0      394 2024-05-06 19:59:39.000000 rc3-0.0.3/src/rc3/data/collection/examples/example_MintOauth2Token.request
--rw-rw-rw-   0        0        0      268 2024-05-06 19:59:39.000000 rc3-0.0.3/src/rc3/data/collection/examples/example_POST_json.request
--rw-rw-rw-   0        0        0      224 2024-05-06 19:59:39.000000 rc3-0.0.3/src/rc3/data/collection/examples/example_POST_text-plain.request
--rw-rw-rw-   0        0        0      233 2024-05-06 19:59:39.000000 rc3-0.0.3/src/rc3/data/collection/examples/example_QueryParams.request
--rw-rw-rw-   0        0        0      220 2024-05-06 19:59:39.000000 rc3-0.0.3/src/rc3/data/collection/examples/example_UseOauth2Token.request
--rw-rw-rw-   0        0        0      265 2024-05-06 19:59:39.000000 rc3-0.0.3/src/rc3/data/collection/examples/folder.json
-drwxrwxrwx   0        0        0        0 2024-05-07 00:50:11.017941 rc3-0.0.3/src/rc3/data/collection/greetings-basic/
--rw-rw-rw-   0        0        0      377 2024-05-06 19:59:39.000000 rc3-0.0.3/src/rc3/data/collection/greetings-basic/greeting.request
--rw-rw-rw-   0        0        0      173 2024-05-06 19:59:39.000000 rc3-0.0.3/src/rc3/data/collection/greetings-basic/greetings.request
--rw-rw-rw-   0        0        0      284 2024-05-06 19:59:39.000000 rc3-0.0.3/src/rc3/data/collection/greetings-basic/new-greeting.request
--rw-rw-rw-   0        0        0      290 2024-05-06 19:59:39.000000 rc3-0.0.3/src/rc3/data/collection/greetings-basic/rc-folder.json
--rw-rw-rw-   0        0        0      178 2024-05-06 19:59:39.000000 rc3-0.0.3/src/rc3/data/collection/greetings-basic/remove-greeting.request
--rw-rw-rw-   0        0        0      306 2024-05-06 19:59:39.000000 rc3-0.0.3/src/rc3/data/collection/greetings-basic/update-greeting.request
-drwxrwxrwx   0        0        0        0 2024-05-07 00:50:11.021937 rc3-0.0.3/src/rc3/data/collection/greetings-oauth2/
--rw-rw-rw-   0        0        0      211 2024-05-06 19:59:39.000000 rc3-0.0.3/src/rc3/data/collection/greetings-oauth2/greeting.request
--rw-rw-rw-   0        0        0      459 2024-05-06 19:59:39.000000 rc3-0.0.3/src/rc3/data/collection/greetings-oauth2/mint-admin-token.request
--rw-rw-rw-   0        0        0      458 2024-05-06 19:59:39.000000 rc3-0.0.3/src/rc3/data/collection/greetings-oauth2/mint-token.request
--rw-rw-rw-   0        0        0      224 2024-05-06 19:59:39.000000 rc3-0.0.3/src/rc3/data/collection/rc-collection.json
-drwxrwxrwx   0        0        0        0 2024-05-07 00:50:11.024936 rc3-0.0.3/src/rc3/data/home/
--rw-rw-rw-   0        0        0      123 2024-05-06 19:59:39.000000 rc3-0.0.3/src/rc3/data/home/rc-global.json
--rw-rw-rw-   0        0        0      347 2024-05-06 19:59:39.000000 rc3-0.0.3/src/rc3/data/home/rc-settings.json
-drwxrwxrwx   0        0        0        0 2024-05-07 00:50:11.031931 rc3-0.0.3/src/rc3/data/home/schemas/
--rw-rw-rw-   0        0        0     1144 2024-05-06 19:59:39.000000 rc3-0.0.3/src/rc3/data/home/schemas/rc3-auth-0.0.3.json
--rw-rw-rw-   0        0        0      904 2024-05-06 19:59:39.000000 rc3-0.0.3/src/rc3/data/home/schemas/rc3-collection-0.0.3.json
--rw-rw-rw-   0        0        0      466 2024-05-06 19:59:39.000000 rc3-0.0.3/src/rc3/data/home/schemas/rc3-environment-0.0.3.json
--rw-rw-rw-   0        0        0      591 2024-05-06 19:59:39.000000 rc3-0.0.3/src/rc3/data/home/schemas/rc3-folder-0.0.3.json
--rw-rw-rw-   0        0        0     3227 2024-05-06 19:59:39.000000 rc3-0.0.3/src/rc3/data/home/schemas/rc3-request-0.0.3.json
--rw-rw-rw-   0        0        0     2252 2024-05-06 19:59:39.000000 rc3-0.0.3/src/rc3/data/home/schemas/rc3-settings-0.0.3.json
-drwxrwxrwx   0        0        0        0 2024-05-07 00:50:11.108013 rc3-0.0.3/src/rc3.egg-info/
--rw-rw-rw-   0        0        0     9394 2024-05-07 00:50:10.000000 rc3-0.0.3/src/rc3.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     5354 2024-05-07 00:50:10.000000 rc3-0.0.3/src/rc3.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 00:50:10.000000 rc3-0.0.3/src/rc3.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2024-05-07 00:50:10.000000 rc3-0.0.3/src/rc3.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      100 2024-05-07 00:50:10.000000 rc3-0.0.3/src/rc3.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-05-07 00:50:10.000000 rc3-0.0.3/src/rc3.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-07 00:50:11.033930 rc3-0.0.3/temp-collection/
-drwxrwxrwx   0        0        0        0 2024-05-07 00:50:11.035929 rc3-0.0.3/temp-collection/environments/
--rw-rw-rw-   0        0        0      270 2024-05-06 19:59:39.000000 rc3-0.0.3/temp-collection/environments/dev.json
--rw-rw-rw-   0        0        0      300 2024-05-06 19:59:39.000000 rc3-0.0.3/temp-collection/environments/localhost.json
-drwxrwxrwx   0        0        0        0 2024-05-07 00:50:11.051919 rc3-0.0.3/temp-collection/examples/
--rw-rw-rw-   0        0        0      240 2024-05-06 19:59:39.000000 rc3-0.0.3/temp-collection/examples/example_Auth_Basic.request
--rw-rw-rw-   0        0        0      907 2024-05-06 19:59:39.000000 rc3-0.0.3/temp-collection/examples/example_Auth_Bearer.request
--rw-rw-rw-   0        0        0      953 2024-05-06 19:59:39.000000 rc3-0.0.3/temp-collection/examples/example_Auth_Token.request
--rw-rw-rw-   0        0        0      429 2024-05-06 19:59:39.000000 rc3-0.0.3/temp-collection/examples/example_Extract_JsonPath.request
--rw-rw-rw-   0        0        0      448 2024-05-06 19:59:39.000000 rc3-0.0.3/temp-collection/examples/example_Extract_Regex.request
--rw-rw-rw-   0        0        0      183 2024-05-06 19:59:39.000000 rc3-0.0.3/temp-collection/examples/example_GET.request
--rw-rw-rw-   0        0        0      792 2024-05-06 19:59:39.000000 rc3-0.0.3/temp-collection/examples/example_KitchenSink.request
--rw-rw-rw-   0        0        0      394 2024-05-06 19:59:39.000000 rc3-0.0.3/temp-collection/examples/example_MintOauth2Token.request
--rw-rw-rw-   0        0        0      268 2024-05-06 19:59:39.000000 rc3-0.0.3/temp-collection/examples/example_POST_json.request
--rw-rw-rw-   0        0        0      224 2024-05-06 19:59:39.000000 rc3-0.0.3/temp-collection/examples/example_POST_text-plain.request
--rw-rw-rw-   0        0        0      233 2024-05-06 19:59:39.000000 rc3-0.0.3/temp-collection/examples/example_QueryParams.request
--rw-rw-rw-   0        0        0      220 2024-05-06 19:59:39.000000 rc3-0.0.3/temp-collection/examples/example_UseOauth2Token.request
--rw-rw-rw-   0        0        0      265 2024-05-06 19:59:39.000000 rc3-0.0.3/temp-collection/examples/folder.json
-drwxrwxrwx   0        0        0        0 2024-05-07 00:50:11.066910 rc3-0.0.3/temp-collection/greetings-basic/
--rw-rw-rw-   0        0        0      377 2024-05-06 19:59:39.000000 rc3-0.0.3/temp-collection/greetings-basic/greeting.request
--rw-rw-rw-   0        0        0     1038 2024-05-06 22:57:40.000000 rc3-0.0.3/temp-collection/greetings-basic/greeting.response
--rw-rw-rw-   0        0        0      173 2024-05-06 19:59:39.000000 rc3-0.0.3/temp-collection/greetings-basic/greetings.request
--rw-rw-rw-   0        0        0     1480 2024-05-06 23:33:37.000000 rc3-0.0.3/temp-collection/greetings-basic/greetings.response
--rw-rw-rw-   0        0        0      284 2024-05-06 19:59:39.000000 rc3-0.0.3/temp-collection/greetings-basic/new-greeting.request
--rw-rw-rw-   0        0        0      919 2024-05-06 23:34:13.000000 rc3-0.0.3/temp-collection/greetings-basic/new-greeting.response
--rw-rw-rw-   0        0        0      290 2024-05-06 19:59:39.000000 rc3-0.0.3/temp-collection/greetings-basic/rc-folder.json
--rw-rw-rw-   0        0        0      178 2024-05-06 19:59:39.000000 rc3-0.0.3/temp-collection/greetings-basic/remove-greeting.request
--rw-rw-rw-   0        0        0      877 2024-05-06 23:34:18.000000 rc3-0.0.3/temp-collection/greetings-basic/remove-greeting.response
--rw-rw-rw-   0        0        0      306 2024-05-06 19:59:39.000000 rc3-0.0.3/temp-collection/greetings-basic/update-greeting.request
--rw-rw-rw-   0        0        0      919 2024-05-06 23:34:25.000000 rc3-0.0.3/temp-collection/greetings-basic/update-greeting.response
-drwxrwxrwx   0        0        0        0 2024-05-07 00:50:11.075688 rc3-0.0.3/temp-collection/greetings-oauth2/
--rw-rw-rw-   0        0        0      211 2024-05-06 19:59:39.000000 rc3-0.0.3/temp-collection/greetings-oauth2/greeting.request
--rw-rw-rw-   0        0        0      919 2024-05-06 23:34:54.000000 rc3-0.0.3/temp-collection/greetings-oauth2/greeting.response
--rw-rw-rw-   0        0        0      459 2024-05-06 19:59:39.000000 rc3-0.0.3/temp-collection/greetings-oauth2/mint-admin-token.request
--rw-rw-rw-   0        0        0      458 2024-05-06 19:59:39.000000 rc3-0.0.3/temp-collection/greetings-oauth2/mint-token.request
--rw-rw-rw-   0        0        0      232 2024-05-06 22:58:18.000000 rc3-0.0.3/temp-collection/rc-collection.json
-drwxrwxrwx   0        0        0        0 2024-05-07 00:50:11.079688 rc3-0.0.3/tests/
--rw-rw-rw-   0        0        0        0 2024-05-06 19:59:39.000000 rc3-0.0.3/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-07 00:50:11.087684 rc3-0.0.3/tests/commands/
--rw-rw-rw-   0        0        0        0 2024-05-06 19:59:39.000000 rc3-0.0.3/tests/commands/__init__.py
--rw-rw-rw-   0        0        0      599 2024-05-06 20:00:31.000000 rc3-0.0.3/tests/commands/test_collection.py
--rw-rw-rw-   0        0        0     5698 2024-05-06 20:00:31.000000 rc3-0.0.3/tests/commands/test_environment.py
--rw-rw-rw-   0        0        0     1840 2024-05-06 23:01:32.000000 rc3-0.0.3/tests/commands/test_init.py
--rw-rw-rw-   0        0        0      427 2024-05-06 20:00:31.000000 rc3-0.0.3/tests/commands/test_list.py
--rw-rw-rw-   0        0        0     5923 2024-05-06 20:00:31.000000 rc3-0.0.3/tests/commands/test_request.py
--rw-rw-rw-   0        0        0     6322 2024-05-06 20:00:31.000000 rc3-0.0.3/tests/commands/test_send.py
-drwxrwxrwx   0        0        0        0 2024-05-07 00:50:11.099017 rc3-0.0.3/tests/commands/test_send_files/
--rw-rw-rw-   0        0        0      263 2024-05-06 19:59:39.000000 rc3-0.0.3/tests/commands/test_send_files/test_is_verbose.yaml
--rw-rw-rw-   0        0        0     1178 2024-05-06 19:59:39.000000 rc3-0.0.3/tests/commands/test_send_files/test_mint_extract_use_token.yaml
--rw-rw-rw-   0        0        0      263 2024-05-06 19:59:39.000000 rc3-0.0.3/tests/commands/test_send_files/test_not_verbose.yaml
--rw-rw-rw-   0        0        0      263 2024-05-06 19:59:39.000000 rc3-0.0.3/tests/commands/test_send_files/test_request_no_responses.yaml
--rw-rw-rw-   0        0        0      263 2024-05-06 19:59:39.000000 rc3-0.0.3/tests/commands/test_send_files/test_send_1.yaml
--rw-rw-rw-   0        0        0      663 2024-05-06 19:59:39.000000 rc3-0.0.3/tests/commands/test_send_files/test_send_2.yaml
--rw-rw-rw-   0        0        0     1098 2024-05-06 19:59:39.000000 rc3-0.0.3/tests/commands/test_send_files/test_send_basics.yaml
--rw-rw-rw-   0        0        0      263 2024-05-06 19:59:39.000000 rc3-0.0.3/tests/commands/test_send_files/test_settings_no_responses.yaml
--rw-rw-rw-   0        0        0      263 2024-05-06 19:59:39.000000 rc3-0.0.3/tests/commands/test_send_files/test_settings_with_responses.yaml
-drwxrwxrwx   0        0        0        0 2024-05-07 00:50:11.102021 rc3-0.0.3/tests/common/
--rw-rw-rw-   0        0        0        0 2024-05-06 19:59:39.000000 rc3-0.0.3/tests/common/__init__.py
--rw-rw-rw-   0        0        0     5211 2024-05-06 20:00:31.000000 rc3-0.0.3/tests/common/test_env_helper.py
--rw-rw-rw-   0        0        0     3345 2024-05-06 22:51:48.000000 rc3-0.0.3/tests/common/test_inherit_helper.py
--rw-rw-rw-   0        0        0     1124 2024-05-06 20:00:31.000000 rc3-0.0.3/tests/conftest.py
-drwxrwxrwx   0        0        0        0 2024-05-07 00:50:11.104014 rc3-0.0.3/tests/learning/
--rw-rw-rw-   0        0        0        0 2024-05-06 19:59:39.000000 rc3-0.0.3/tests/learning/__init__.py
--rw-rw-rw-   0        0        0      518 2024-05-06 19:59:39.000000 rc3-0.0.3/tests/learning/test_sample.py
--rw-rw-rw-   0        0        0     1665 2024-05-06 20:00:31.000000 rc3-0.0.3/tests/test_cli.py
-drwxrwxrwx   0        0        0        0 2024-05-07 00:50:11.106012 rc3-0.0.3/tests/util/
--rw-rw-rw-   0        0        0        0 2024-05-06 19:59:39.000000 rc3-0.0.3/tests/util/__init__.py
--rw-rw-rw-   0        0        0     1407 2024-05-06 19:59:39.000000 rc3-0.0.3/tests/util/decorators.py
+drwxrwxrwx   0        0        0        0 2024-05-08 19:50:09.352792 rc3-0.0.4/
+-rw-rw-rw-   0        0        0     3141 2024-05-06 19:59:38.000000 rc3-0.0.4/.gitignore
+-rw-rw-rw-   0        0        0     1087 2024-05-06 20:36:33.000000 rc3-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0    11429 2024-05-08 19:50:09.351793 rc3-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     9378 2024-05-08 19:25:58.000000 rc3-0.0.4/README.md
+-rw-rw-rw-   0        0        0     1044 2024-05-07 23:16:04.000000 rc3-0.0.4/WINDOWS_SETUP.md
+-rw-rw-rw-   0        0        0      823 2024-05-08 19:40:54.000000 rc3-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0      475 2024-05-06 20:07:47.000000 rc3-0.0.4/rc3.iml
+-rw-rw-rw-   0        0        0       42 2024-05-08 19:50:09.352792 rc3-0.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-08 19:50:09.192160 rc3-0.0.4/src/
+drwxrwxrwx   0        0        0        0 2024-05-08 19:50:09.210349 rc3-0.0.4/src/rc3/
+-rw-rw-rw-   0        0        0      246 2024-05-06 19:59:38.000000 rc3-0.0.4/src/rc3/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 19:50:09.222689 rc3-0.0.4/src/rc3/archive/
+-rw-rw-rw-   0        0        0        0 2024-05-06 19:59:38.000000 rc3-0.0.4/src/rc3/archive/__init__.py
+-rw-rw-rw-   0        0        0      406 2024-05-06 20:00:31.000000 rc3-0.0.4/src/rc3/archive/cmd_home.py
+-rw-rw-rw-   0        0        0      637 2024-05-06 20:00:31.000000 rc3-0.0.4/src/rc3/archive/cmd_root.py
+-rw-rw-rw-   0        0        0     1125 2024-05-06 20:00:31.000000 rc3-0.0.4/src/rc3/archive/cmd_subs.py
+-rw-rw-rw-   0        0        0     1924 2024-05-07 23:36:03.000000 rc3-0.0.4/src/rc3/cli.py
+drwxrwxrwx   0        0        0        0 2024-05-08 19:50:09.234641 rc3-0.0.4/src/rc3/commands/
+-rw-rw-rw-   0        0        0        0 2024-05-06 19:59:38.000000 rc3-0.0.4/src/rc3/commands/__init__.py
+-rw-rw-rw-   0        0        0     3415 2024-05-06 22:52:43.000000 rc3-0.0.4/src/rc3/commands/cmd_collection.py
+-rw-rw-rw-   0        0        0     5467 2024-05-07 23:33:42.000000 rc3-0.0.4/src/rc3/commands/cmd_environment.py
+-rw-rw-rw-   0        0        0     1454 2024-05-07 23:35:00.000000 rc3-0.0.4/src/rc3/commands/cmd_global.py
+-rw-rw-rw-   0        0        0      524 2024-05-06 19:59:38.000000 rc3-0.0.4/src/rc3/commands/cmd_hello.py
+-rw-rw-rw-   0        0        0     2559 2024-05-06 23:00:33.000000 rc3-0.0.4/src/rc3/commands/cmd_init.py
+-rw-rw-rw-   0        0        0     2136 2024-05-08 19:24:17.000000 rc3-0.0.4/src/rc3/commands/cmd_list.py
+-rw-rw-rw-   0        0        0     4322 2024-05-06 20:00:31.000000 rc3-0.0.4/src/rc3/commands/cmd_request.py
+-rw-rw-rw-   0        0        0     9478 2024-05-08 18:59:18.000000 rc3-0.0.4/src/rc3/commands/cmd_send.py
+-rw-rw-rw-   0        0        0     1368 2024-05-08 18:10:08.000000 rc3-0.0.4/src/rc3/commands/cmd_settings.py
+drwxrwxrwx   0        0        0        0 2024-05-08 19:50:09.244942 rc3-0.0.4/src/rc3/common/
+-rw-rw-rw-   0        0        0        0 2024-05-06 19:59:39.000000 rc3-0.0.4/src/rc3/common/__init__.py
+-rw-rw-rw-   0        0        0      524 2024-05-06 19:59:39.000000 rc3-0.0.4/src/rc3/common/config_helper.py
+-rw-rw-rw-   0        0        0      869 2024-05-06 22:59:13.000000 rc3-0.0.4/src/rc3/common/data_helper.py
+-rw-rw-rw-   0        0        0      936 2024-05-06 19:59:39.000000 rc3-0.0.4/src/rc3/common/decorators.py
+-rw-rw-rw-   0        0        0     2670 2024-05-06 20:00:31.000000 rc3-0.0.4/src/rc3/common/env_helper.py
+-rw-rw-rw-   0        0        0     1364 2024-05-06 22:52:57.000000 rc3-0.0.4/src/rc3/common/inherit_helper.py
+-rw-rw-rw-   0        0        0    10723 2024-05-08 18:47:05.000000 rc3-0.0.4/src/rc3/common/json_helper.py
+-rw-rw-rw-   0        0        0     2503 2024-05-08 19:08:29.000000 rc3-0.0.4/src/rc3/common/print_helper.py
+-rw-rw-rw-   0        0        0       86 2024-05-06 19:59:39.000000 rc3-0.0.4/src/rc3/common/rc_globals.py
+drwxrwxrwx   0        0        0        0 2024-05-08 19:50:09.245941 rc3-0.0.4/src/rc3/data/
+-rw-rw-rw-   0        0        0        0 2024-05-06 19:59:39.000000 rc3-0.0.4/src/rc3/data/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 19:50:09.246940 rc3-0.0.4/src/rc3/data/collection/
+drwxrwxrwx   0        0        0        0 2024-05-08 19:50:09.249938 rc3-0.0.4/src/rc3/data/collection/environments/
+-rw-rw-rw-   0        0        0      277 2024-05-07 23:02:08.000000 rc3-0.0.4/src/rc3/data/collection/environments/dev.json
+-rw-rw-rw-   0        0        0      307 2024-05-07 23:02:08.000000 rc3-0.0.4/src/rc3/data/collection/environments/localhost.json
+drwxrwxrwx   0        0        0        0 2024-05-08 19:50:09.263930 rc3-0.0.4/src/rc3/data/collection/examples/
+-rw-rw-rw-   0        0        0      247 2024-05-07 23:02:08.000000 rc3-0.0.4/src/rc3/data/collection/examples/example_Auth_Basic.request
+-rw-rw-rw-   0        0        0      914 2024-05-07 23:02:08.000000 rc3-0.0.4/src/rc3/data/collection/examples/example_Auth_Bearer.request
+-rw-rw-rw-   0        0        0      960 2024-05-07 23:02:08.000000 rc3-0.0.4/src/rc3/data/collection/examples/example_Auth_Token.request
+-rw-rw-rw-   0        0        0      436 2024-05-07 23:02:08.000000 rc3-0.0.4/src/rc3/data/collection/examples/example_Extract_JsonPath.request
+-rw-rw-rw-   0        0        0      455 2024-05-07 23:02:08.000000 rc3-0.0.4/src/rc3/data/collection/examples/example_Extract_Regex.request
+-rw-rw-rw-   0        0        0      190 2024-05-07 23:02:08.000000 rc3-0.0.4/src/rc3/data/collection/examples/example_GET.request
+-rw-rw-rw-   0        0        0      799 2024-05-07 23:02:08.000000 rc3-0.0.4/src/rc3/data/collection/examples/example_KitchenSink.request
+-rw-rw-rw-   0        0        0      401 2024-05-07 23:02:08.000000 rc3-0.0.4/src/rc3/data/collection/examples/example_MintOauth2Token.request
+-rw-rw-rw-   0        0        0      275 2024-05-07 23:02:08.000000 rc3-0.0.4/src/rc3/data/collection/examples/example_POST_json.request
+-rw-rw-rw-   0        0        0      231 2024-05-07 23:02:08.000000 rc3-0.0.4/src/rc3/data/collection/examples/example_POST_text-plain.request
+-rw-rw-rw-   0        0        0      240 2024-05-07 23:02:08.000000 rc3-0.0.4/src/rc3/data/collection/examples/example_QueryParams.request
+-rw-rw-rw-   0        0        0      227 2024-05-07 23:02:08.000000 rc3-0.0.4/src/rc3/data/collection/examples/example_UseOauth2Token.request
+-rw-rw-rw-   0        0        0      272 2024-05-07 23:02:08.000000 rc3-0.0.4/src/rc3/data/collection/examples/folder.json
+drwxrwxrwx   0        0        0        0 2024-05-08 19:50:09.270926 rc3-0.0.4/src/rc3/data/collection/greetings-basic/
+-rw-rw-rw-   0        0        0      384 2024-05-07 23:02:08.000000 rc3-0.0.4/src/rc3/data/collection/greetings-basic/greeting.request
+-rw-rw-rw-   0        0        0      180 2024-05-07 23:02:08.000000 rc3-0.0.4/src/rc3/data/collection/greetings-basic/greetings.request
+-rw-rw-rw-   0        0        0      291 2024-05-07 23:02:08.000000 rc3-0.0.4/src/rc3/data/collection/greetings-basic/new-greeting.request
+-rw-rw-rw-   0        0        0      297 2024-05-07 23:02:08.000000 rc3-0.0.4/src/rc3/data/collection/greetings-basic/rc-folder.json
+-rw-rw-rw-   0        0        0      185 2024-05-07 23:02:08.000000 rc3-0.0.4/src/rc3/data/collection/greetings-basic/remove-greeting.request
+-rw-rw-rw-   0        0        0      313 2024-05-07 23:02:08.000000 rc3-0.0.4/src/rc3/data/collection/greetings-basic/update-greeting.request
+drwxrwxrwx   0        0        0        0 2024-05-08 19:50:09.274922 rc3-0.0.4/src/rc3/data/collection/greetings-oauth2/
+-rw-rw-rw-   0        0        0      218 2024-05-07 23:02:08.000000 rc3-0.0.4/src/rc3/data/collection/greetings-oauth2/greeting.request
+-rw-rw-rw-   0        0        0      466 2024-05-07 23:02:08.000000 rc3-0.0.4/src/rc3/data/collection/greetings-oauth2/mint-admin-token.request
+-rw-rw-rw-   0        0        0      465 2024-05-07 23:02:08.000000 rc3-0.0.4/src/rc3/data/collection/greetings-oauth2/mint-token.request
+-rw-rw-rw-   0        0        0      247 2024-05-08 14:58:01.000000 rc3-0.0.4/src/rc3/data/collection/rc-collection.json
+drwxrwxrwx   0        0        0        0 2024-05-08 19:50:09.276922 rc3-0.0.4/src/rc3/data/home/
+-rw-rw-rw-   0        0        0      130 2024-05-07 23:02:08.000000 rc3-0.0.4/src/rc3/data/home/rc-global.json
+-rw-rw-rw-   0        0        0      354 2024-05-07 23:02:39.000000 rc3-0.0.4/src/rc3/data/home/rc-settings.json
+drwxrwxrwx   0        0        0        0 2024-05-08 19:50:09.284917 rc3-0.0.4/src/rc3/data/home/schemas/
+-rw-rw-rw-   0        0        0     1151 2024-05-07 23:02:08.000000 rc3-0.0.4/src/rc3/data/home/schemas/rc3-auth-0.0.3.json
+-rw-rw-rw-   0        0        0      918 2024-05-07 23:02:08.000000 rc3-0.0.4/src/rc3/data/home/schemas/rc3-collection-0.0.3.json
+-rw-rw-rw-   0        0        0      473 2024-05-07 23:02:08.000000 rc3-0.0.4/src/rc3/data/home/schemas/rc3-environment-0.0.3.json
+-rw-rw-rw-   0        0        0      605 2024-05-07 23:02:08.000000 rc3-0.0.4/src/rc3/data/home/schemas/rc3-folder-0.0.3.json
+-rw-rw-rw-   0        0        0     3241 2024-05-07 23:02:08.000000 rc3-0.0.4/src/rc3/data/home/schemas/rc3-request-0.0.3.json
+-rw-rw-rw-   0        0        0     2259 2024-05-07 23:02:08.000000 rc3-0.0.4/src/rc3/data/home/schemas/rc3-settings-0.0.3.json
+drwxrwxrwx   0        0        0        0 2024-05-08 19:50:09.349590 rc3-0.0.4/src/rc3.egg-info/
+-rw-rw-rw-   0        0        0    11429 2024-05-08 19:50:08.000000 rc3-0.0.4/src/rc3.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     5183 2024-05-08 19:50:09.000000 rc3-0.0.4/src/rc3.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 19:50:08.000000 rc3-0.0.4/src/rc3.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2024-05-08 19:50:08.000000 rc3-0.0.4/src/rc3.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      100 2024-05-08 19:50:08.000000 rc3-0.0.4/src/rc3.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-05-08 19:50:08.000000 rc3-0.0.4/src/rc3.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-08 19:50:09.285915 rc3-0.0.4/temp-collection/
+drwxrwxrwx   0        0        0        0 2024-05-08 19:50:09.287915 rc3-0.0.4/temp-collection/environments/
+-rw-rw-rw-   0        0        0      277 2024-05-07 23:02:08.000000 rc3-0.0.4/temp-collection/environments/dev.json
+-rw-rw-rw-   0        0        0      307 2024-05-07 23:02:08.000000 rc3-0.0.4/temp-collection/environments/localhost.json
+drwxrwxrwx   0        0        0        0 2024-05-08 19:50:09.304921 rc3-0.0.4/temp-collection/examples/
+-rw-rw-rw-   0        0        0      247 2024-05-07 23:02:08.000000 rc3-0.0.4/temp-collection/examples/example_Auth_Basic.request
+-rw-rw-rw-   0        0        0      914 2024-05-07 23:02:08.000000 rc3-0.0.4/temp-collection/examples/example_Auth_Bearer.request
+-rw-rw-rw-   0        0        0      960 2024-05-07 23:02:08.000000 rc3-0.0.4/temp-collection/examples/example_Auth_Token.request
+-rw-rw-rw-   0        0        0      436 2024-05-07 23:02:08.000000 rc3-0.0.4/temp-collection/examples/example_Extract_JsonPath.request
+-rw-rw-rw-   0        0        0      455 2024-05-07 23:02:08.000000 rc3-0.0.4/temp-collection/examples/example_Extract_Regex.request
+-rw-rw-rw-   0        0        0      190 2024-05-07 23:02:08.000000 rc3-0.0.4/temp-collection/examples/example_GET.request
+-rw-rw-rw-   0        0        0      799 2024-05-07 23:02:08.000000 rc3-0.0.4/temp-collection/examples/example_KitchenSink.request
+-rw-rw-rw-   0        0        0      401 2024-05-07 23:02:08.000000 rc3-0.0.4/temp-collection/examples/example_MintOauth2Token.request
+-rw-rw-rw-   0        0        0      275 2024-05-07 23:02:08.000000 rc3-0.0.4/temp-collection/examples/example_POST_json.request
+-rw-rw-rw-   0        0        0      231 2024-05-07 23:02:08.000000 rc3-0.0.4/temp-collection/examples/example_POST_text-plain.request
+-rw-rw-rw-   0        0        0      240 2024-05-07 23:02:08.000000 rc3-0.0.4/temp-collection/examples/example_QueryParams.request
+-rw-rw-rw-   0        0        0      227 2024-05-07 23:02:08.000000 rc3-0.0.4/temp-collection/examples/example_UseOauth2Token.request
+-rw-rw-rw-   0        0        0      272 2024-05-07 23:02:08.000000 rc3-0.0.4/temp-collection/examples/folder.json
+drwxrwxrwx   0        0        0        0 2024-05-08 19:50:09.315029 rc3-0.0.4/temp-collection/greetings-basic/
+-rw-rw-rw-   0        0        0      384 2024-05-07 23:02:08.000000 rc3-0.0.4/temp-collection/greetings-basic/greeting.request
+-rw-rw-rw-   0        0        0     1038 2024-05-08 19:32:46.000000 rc3-0.0.4/temp-collection/greetings-basic/greeting.response
+-rw-rw-rw-   0        0        0      180 2024-05-07 23:02:08.000000 rc3-0.0.4/temp-collection/greetings-basic/greetings.request
+-rw-rw-rw-   0        0        0     1480 2024-05-08 19:32:39.000000 rc3-0.0.4/temp-collection/greetings-basic/greetings.response
+-rw-rw-rw-   0        0        0      291 2024-05-07 23:02:08.000000 rc3-0.0.4/temp-collection/greetings-basic/new-greeting.request
+-rw-rw-rw-   0        0        0      297 2024-05-07 23:02:08.000000 rc3-0.0.4/temp-collection/greetings-basic/rc-folder.json
+-rw-rw-rw-   0        0        0      185 2024-05-07 23:02:08.000000 rc3-0.0.4/temp-collection/greetings-basic/remove-greeting.request
+-rw-rw-rw-   0        0        0      313 2024-05-07 23:02:08.000000 rc3-0.0.4/temp-collection/greetings-basic/update-greeting.request
+drwxrwxrwx   0        0        0        0 2024-05-08 19:50:09.318027 rc3-0.0.4/temp-collection/greetings-oauth2/
+-rw-rw-rw-   0        0        0      218 2024-05-07 23:02:08.000000 rc3-0.0.4/temp-collection/greetings-oauth2/greeting.request
+-rw-rw-rw-   0        0        0      466 2024-05-07 23:02:08.000000 rc3-0.0.4/temp-collection/greetings-oauth2/mint-admin-token.request
+-rw-rw-rw-   0        0        0      465 2024-05-07 23:02:08.000000 rc3-0.0.4/temp-collection/greetings-oauth2/mint-token.request
+-rw-rw-rw-   0        0        0      255 2024-05-08 19:32:46.000000 rc3-0.0.4/temp-collection/rc-collection.json
+drwxrwxrwx   0        0        0        0 2024-05-08 19:50:09.321878 rc3-0.0.4/tests/
+-rw-rw-rw-   0        0        0        0 2024-05-06 19:59:39.000000 rc3-0.0.4/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 19:50:09.329602 rc3-0.0.4/tests/commands/
+-rw-rw-rw-   0        0        0        0 2024-05-06 19:59:39.000000 rc3-0.0.4/tests/commands/__init__.py
+-rw-rw-rw-   0        0        0      599 2024-05-06 20:00:31.000000 rc3-0.0.4/tests/commands/test_collection.py
+-rw-rw-rw-   0        0        0     5698 2024-05-06 20:00:31.000000 rc3-0.0.4/tests/commands/test_environment.py
+-rw-rw-rw-   0        0        0     1856 2024-05-08 19:17:23.000000 rc3-0.0.4/tests/commands/test_init.py
+-rw-rw-rw-   0        0        0      427 2024-05-06 20:00:31.000000 rc3-0.0.4/tests/commands/test_list.py
+-rw-rw-rw-   0        0        0     5923 2024-05-06 20:00:31.000000 rc3-0.0.4/tests/commands/test_request.py
+-rw-rw-rw-   0        0        0     6322 2024-05-06 20:00:31.000000 rc3-0.0.4/tests/commands/test_send.py
+drwxrwxrwx   0        0        0        0 2024-05-08 19:50:09.339597 rc3-0.0.4/tests/commands/test_send_files/
+-rw-rw-rw-   0        0        0      263 2024-05-06 19:59:39.000000 rc3-0.0.4/tests/commands/test_send_files/test_is_verbose.yaml
+-rw-rw-rw-   0        0        0     1178 2024-05-06 19:59:39.000000 rc3-0.0.4/tests/commands/test_send_files/test_mint_extract_use_token.yaml
+-rw-rw-rw-   0        0        0      263 2024-05-06 19:59:39.000000 rc3-0.0.4/tests/commands/test_send_files/test_not_verbose.yaml
+-rw-rw-rw-   0        0        0      263 2024-05-06 19:59:39.000000 rc3-0.0.4/tests/commands/test_send_files/test_request_no_responses.yaml
+-rw-rw-rw-   0        0        0      263 2024-05-06 19:59:39.000000 rc3-0.0.4/tests/commands/test_send_files/test_send_1.yaml
+-rw-rw-rw-   0        0        0      663 2024-05-06 19:59:39.000000 rc3-0.0.4/tests/commands/test_send_files/test_send_2.yaml
+-rw-rw-rw-   0        0        0     1098 2024-05-06 19:59:39.000000 rc3-0.0.4/tests/commands/test_send_files/test_send_basics.yaml
+-rw-rw-rw-   0        0        0      263 2024-05-06 19:59:39.000000 rc3-0.0.4/tests/commands/test_send_files/test_settings_no_responses.yaml
+-rw-rw-rw-   0        0        0      263 2024-05-06 19:59:39.000000 rc3-0.0.4/tests/commands/test_send_files/test_settings_with_responses.yaml
+drwxrwxrwx   0        0        0        0 2024-05-08 19:50:09.342594 rc3-0.0.4/tests/common/
+-rw-rw-rw-   0        0        0        0 2024-05-06 19:59:39.000000 rc3-0.0.4/tests/common/__init__.py
+-rw-rw-rw-   0        0        0     5211 2024-05-06 20:00:31.000000 rc3-0.0.4/tests/common/test_env_helper.py
+-rw-rw-rw-   0        0        0     3345 2024-05-06 22:51:48.000000 rc3-0.0.4/tests/common/test_inherit_helper.py
+-rw-rw-rw-   0        0        0     1124 2024-05-06 20:00:31.000000 rc3-0.0.4/tests/conftest.py
+drwxrwxrwx   0        0        0        0 2024-05-08 19:50:09.345591 rc3-0.0.4/tests/learning/
+-rw-rw-rw-   0        0        0        0 2024-05-06 19:59:39.000000 rc3-0.0.4/tests/learning/__init__.py
+-rw-rw-rw-   0        0        0      518 2024-05-06 19:59:39.000000 rc3-0.0.4/tests/learning/test_sample.py
+-rw-rw-rw-   0        0        0     1665 2024-05-06 20:00:31.000000 rc3-0.0.4/tests/test_cli.py
+drwxrwxrwx   0        0        0        0 2024-05-08 19:50:09.347591 rc3-0.0.4/tests/util/
+-rw-rw-rw-   0        0        0        0 2024-05-06 19:59:39.000000 rc3-0.0.4/tests/util/__init__.py
+-rw-rw-rw-   0        0        0     1407 2024-05-06 19:59:39.000000 rc3-0.0.4/tests/util/decorators.py
```

### Comparing `rc3-0.0.3/.gitignore` & `rc3-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `rc3-0.0.3/LICENSE` & `rc3-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `rc3-0.0.3/PKG-INFO` & `rc3-0.0.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,53 +1,7 @@
-Metadata-Version: 2.1
-Name: rc3
-Version: 0.0.3
-Summary: Rest CLI (rc)
-Author-email: Gary Wilcox <gary@dugan-wilcox.com>
-License: MIT License
-        
-        Copyright (c) 2018 Real Python
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-Project-URL: repository, https://github.com/gswilcox01/rc3
-Keywords: rest,cli,postman
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: click>=8.1
-Requires-Dist: requests>=2.31
-Requires-Dist: jsonschema
-Requires-Dist: jsonpath-ng
-Requires-Dist: funcy
-Provides-Extra: build
-Requires-Dist: build; extra == "build"
-Requires-Dist: twine; extra == "build"
-Provides-Extra: dev
-Requires-Dist: pytest; extra == "dev"
-Requires-Dist: responses; extra == "dev"
-
 # rc
 rc = REST CLI  
 
 rc is a tool to help execute REST API requests.  
 rc is based on Collections, Environments and Requests.  Similar to the tool we all love/hate --- Postman.  
 
 ## Overview
@@ -59,53 +13,95 @@
 
 ## Installation
 * Pre-reqs
     * Python 3.12+ (required)
     * VSCode (optional, but highly recommended)
 * Install
     * pip install rc3
+* Windows User?
+    * See:  [Windows Setup Issues](WINDOWS_SETUP.md)
 
-## RC Setup & Sending your first request
-* mkdir example-collection
-* cd example-collection
-* rc init
-    * Will do 0-4 things
-      1. Will create the RC_HOME directory if it doesn't exist.
-      2. Will create RC_HOME/settings, global env, and schemas dir if they don't exist.
-      3. Will initialize a new example Collection if ran from an empty directory.
-      4. Will import the current directory if it contains a valid collection.json file.
-* rc send greeting
-    * Will send the first request named "greeting" in the example Collection
-    * Wait for it…  
-      * A greetings-demo project is running on Google Cloud Run
-      * And it scales down to 0 instances when there is no demand (i.e. your first few requests will be SLOW…)
-* cat greetings-basic/greeting.response
-    * Will show more verbose output from the "rc send greeting" cmd you just sent
+## Setup & Sending your first request
+* First create an empty directory somewhere (any name & location is fine)
+  ```
+  $ mkdir temp-collection
+  $ cd temp-collection
+  ```
+* Next run "rc init" to do 0-4 things
+  1. Will create the RC_HOME directory if it doesn't exist.
+  2. Will create RC_HOME/settings, global env, and schemas dir if they don't exist.
+  3. Will initialize a new example Collection if ran from an empty directory.
+  4. Will import the current directory if it contains a valid collection.json file.
+  ```
+  $ rc init
+  Creating C:\Users\Gary\.rc\rc-settings.json
+  Creating C:\Users\Gary\.rc\rc-global.json                            
+  Creating C:\Users\Gary\.rc\schemas                                   
+  CWD is empty, creating sample Collection here: C:\dev\temp-collection
+  Importing collection from: C:\dev\temp-collection
+  Adding collection to global settings: example-collection
+  ```
+* Next send the "greeting" request with the rc send command
+  * Wait for it…
+    * A greetings-demo project is running on Google Cloud Run
+    * And it scales down to 0 instances when there is no demand (i.e. your first few requests will be SLOW…)  
+  ```
+  $ rc send greeting
+  {                        
+      "id": 1,             
+      "text": "Hello",     
+      "language": "English"
+  }
+  ```
+* Next "cat" the generated greeting.response file that will have more verbose output from the send command
+  ```
+  $ cat greetings-basic/greeting.response
+  {                                                                                     
+    "status_code": 200,                                                               
+    "time": "845.772ms",                                                              
+    "size": {                                                                         
+        "body": 44,                                                                   
+        "headers": 442,                                                               
+        "total": 486                                                                  
+    },                                                                                
+    "headers": {                                                                      
+        "vary": "Origin,Access-Control-Request-Method,Access-Control-Request-Headers",
+        "Date": "Wed, 08 May 2024 15:06:54 GMT",                                      
+        "Server": "Google Frontend",
+  
+    ...
+                                                    
+  }
+  ``` 
 
 ## Sending more requests from the example collection
-* All the requests in the example collection can be sent to the greetings-demo app
+* All the requests in the example collection can be sent to the greetings-demo app running on Google Cloud Run
+* To view all requests in the example collection run "rc request --list"
   ```
+  $ rc request --list
   Listing REQUESTS found in current_collection:
-  NUM:   FOLDER:             MET:     NAME:              
+  NUM:   FOLDER:             METHOD:  NAME:              
   1*     /greetings-basic    GET      greeting
   2      /greetings-basic    GET      greetings
   3      /greetings-basic    POST     new-greeting
   4      /greetings-basic    DELETE   remove-greeting
   5      /greetings-basic    PUT      update-greeting
   6      /greetings-oauth2   GET      greeting
   7      /greetings-oauth2   POST     mint-admin-token
   8      /greetings-oauth2   POST     mint-token
   ```
-* For example:
-    * rc send 1
-    * rc send 2
-    * rc send 3
+* Try sending requests by NUMBER instead of by NAME using these commands:
+  ```
+  $ rc send 1
+  $ rc send 2
+  $ rc send 3
+  ```
 * Notes:
   * Make sure there is a greeting #8 before sending request 4, or you'll get a 404
-  * Make sure you run request 7, before request 6, so you have an access_token
+  * Make sure you run request 7, before request 6, so you have a {{ token }} available in your global environment
 
 ## More command examples
 * View all Collections, Environments, and Requests you have setup on this machine
     * rc list
 * View all Requests for the current Collection (the following commands are equivalent):
     * rc list requests
     * rc list r
@@ -201,17 +197,17 @@
 
 ## CA certificates:
 * By default rc will follow Python Requests default behaviour
   * Using the Python 'certifi' module truststore file
   * And verifying certs
 * You can turn off cert verification in RC_HOME/settings.json with:
   * "ca_cert_verification": false,
-* You can set a custom cert ca_bundle file with:
+* You can set a custom cert ca_bundle file in RC_HOME/settings.json with:
   * "ca_bundle": "/path/to/ca/bundlefile",
-* You can alternativelly set the path to a ca_bundle file with one of these ENV VARS:
+* You can alternatively set the path to a ca_bundle file with one of these ENV VARS:
   * REQUESTS_CA_BUNDLE
   * CURL_CA_BUNDLE
 * For more details see:
   * https://requests.readthedocs.io/en/latest/user/advanced/#ssl-cert-verification
 
 ## VSCode setup:
 * Associate *.request & *.response files with the JSON editor
```

### Comparing `rc3-0.0.3/pyproject.toml` & `rc3-0.0.4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [build-system]
 requires = ["setuptools>=61.0","setuptools-scm","wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "rc3"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Gary Wilcox", email="gary@dugan-wilcox.com" },
 ]
 readme = "README.md"
 license = { file = "LICENSE" }
 description = "Rest CLI (rc)"
-requires-python = ">=3.8"
+requires-python = ">=3.12"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 keywords = ["rest", "cli", "postman"]
 dependencies = [
```

### Comparing `rc3-0.0.3/src/rc3/archive/cmd_root.py` & `rc3-0.0.4/src/rc3/archive/cmd_root.py`

 * *Files identical despite different names*

### Comparing `rc3-0.0.3/src/rc3/archive/cmd_subs.py` & `rc3-0.0.4/src/rc3/archive/cmd_subs.py`

 * *Files identical despite different names*

### Comparing `rc3-0.0.3/src/rc3/cli.py` & `rc3-0.0.4/src/rc3/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,17 @@
 
     def get_command(self, ctx, name):
         # See more options like unique prefix matching here:
         # https://click.palletsprojects.com/en/8.1.x/advanced/#command-aliases
         aliases = {
             'r': 'request',
             'c': 'collection',
-            'e': 'environment'
+            'e': 'environment',
+            'g': 'global',
+            'globals': 'global'
         }
         name = aliases.get(name, name)
         try:
             mod = __import__(f"rc3.commands.cmd_{name}", None, None, ["cli"])
         except ImportError:
             return
         return mod.cli
```

### Comparing `rc3-0.0.3/src/rc3/commands/cmd_collection.py` & `rc3-0.0.4/src/rc3/commands/cmd_collection.py`

 * *Files identical despite different names*

### Comparing `rc3-0.0.3/src/rc3/commands/cmd_environment.py` & `rc3-0.0.4/src/rc3/commands/cmd_environment.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,15 @@
 
 def internal_edit(r):
     json_string = print_helper.get_json_string(r.get('_original'))
     new_string = click.edit(json_string)
     if new_string is not None:
         new_e = json_helper.parse_json(new_string)
         if new_e is None:
-            raise click.ClickException("new REQUEST must be valid JSON.")
+            raise click.ClickException("new ENVIRONMENT must be valid JSON.")
         if json_helper.validate(new_e, 'environment'):
             return new_e
     else:
         return None
 
 
 def lookup_or_prompt(name, prompt="Which ENVIRONMENT do you want to pick?"):
```

### Comparing `rc3-0.0.3/src/rc3/commands/cmd_hello.py` & `rc3-0.0.4/src/rc3/commands/cmd_hello.py`

 * *Files identical despite different names*

### Comparing `rc3-0.0.3/src/rc3/commands/cmd_init.py` & `rc3-0.0.4/src/rc3/commands/cmd_init.py`

 * *Files identical despite different names*

### Comparing `rc3-0.0.3/src/rc3/commands/cmd_list.py` & `rc3-0.0.4/src/rc3/commands/cmd_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,11 +66,11 @@
 
     if len(_list) == 0:
         click.echo("No REQUESTS found in current_collection")
         raise click.Abort()
     click.echo("Listing REQUESTS found in current_collection:")
 
     # now display table
-    header = ['NUM:', 'FOLDER:', 'MET:', 'NAME:']
+    header = ['NUM:', 'FOLDER:', 'METHOD:', 'NAME:']
     fields = ['display_num', 'folder', 'method', 'name']
     print_helper.print_formatted_table(header, fields, _list)
```

### Comparing `rc3-0.0.3/src/rc3/commands/cmd_request.py` & `rc3-0.0.4/src/rc3/commands/cmd_request.py`

 * *Files identical despite different names*

### Comparing `rc3-0.0.3/src/rc3/commands/cmd_send.py` & `rc3-0.0.4/src/rc3/commands/cmd_send.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import os
 import re
 
 import click
 import requests
 from jsonpath_ng import parse
 from requests.auth import HTTPBasicAuth, AuthBase
+from requests.exceptions import SSLError
 
 from rc3.commands import cmd_request
 from rc3.common import json_helper, print_helper, env_helper, inherit_helper, rc_globals
 
 
 @click.command("send", short_help="Sends an HTTP request & writes results to a response file.")
 @click.option('-p', '--pick', is_flag=True, default=False, help="Pick a REQUEST then send it.")
@@ -87,23 +88,30 @@
     if verify and len(settings.get('ca_bundle','')) > 0:
         verify = settings.get('ca_bundle')
         if not os.path.exists(verify):
             raise click.ClickException(f'settings.json ca_bundle file [{verify}] does not exist!')
     if settings.get('headers_send_nocache', True):
         headers['Cache-Control'] = 'no-cache'
 
-    response = requests.request(request.get('method'), request.get('url'),
-                                headers=headers,
-                                json=_json,
-                                auth=create_auth(inherit_helper.find_auth(wrapper)),
-                                params=request.get('params', None),
-                                data=_data,
-                                timeout=timeout,
-                                allow_redirects=allow_redirects,
-                                verify=verify)
+    try:
+        response = requests.request(request.get('method'), request.get('url'),
+                                    headers=headers,
+                                    json=_json,
+                                    auth=create_auth(inherit_helper.find_auth(wrapper)),
+                                    params=request.get('params', None),
+                                    data=_data,
+                                    timeout=timeout,
+                                    allow_redirects=allow_redirects,
+                                    verify=verify)
+    except SSLError as e:
+        print()
+        print(type(e).__name__ + ": " + str(e))
+        click.echo("SSLError: Try setting REQUESTS_CA_BUNDLE, CURL_CA_BUNDLE, or rc-settings.ca_bundle")
+        click.echo("See: https://github.com/gswilcox01/rc3/tree/master?tab=readme-ov-file#ca-certificates")
+        raise click.Abort
 
     process_output(wrapper, response)
 
 
 def process_output(wrapper, response):
     settings = json_helper.read_settings()
     cli_options = rc_globals.get_cli_options()
```

### Comparing `rc3-0.0.3/src/rc3/common/config_helper.py` & `rc3-0.0.4/src/rc3/common/config_helper.py`

 * *Files identical despite different names*

### Comparing `rc3-0.0.3/src/rc3/common/data_helper.py` & `rc3-0.0.4/src/rc3/common/data_helper.py`

 * *Files identical despite different names*

### Comparing `rc3-0.0.3/src/rc3/common/decorators.py` & `rc3-0.0.4/src/rc3/common/decorators.py`

 * *Files identical despite different names*

### Comparing `rc3-0.0.3/src/rc3/common/env_helper.py` & `rc3-0.0.4/src/rc3/common/env_helper.py`

 * *Files identical despite different names*

### Comparing `rc3-0.0.3/src/rc3/common/inherit_helper.py` & `rc3-0.0.4/src/rc3/common/inherit_helper.py`

 * *Files identical despite different names*

### Comparing `rc3-0.0.3/src/rc3/common/json_helper.py` & `rc3-0.0.4/src/rc3/common/json_helper.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import json
 import os
 import sys
+from json import JSONDecodeError
 
+import click
 from funcy import print_durations
 from jsonschema import Draft7Validator
 from referencing import Registry, Resource
 from rc3.common import config_helper, data_helper
 from rc3.common.data_helper import SCHEMA_PREFIX, SCHEMA_VERSION, COLLECTION_FILENAME, SETTINGS_FILENAME, \
     FOLDER_FILENAME, GLOBAL_ENV_FILENAME
 from rc3.common.decorators import rc_print_durations, rc_memoized
@@ -85,15 +87,17 @@
     # https://readthedocs.org/projects/python-jsonschema/downloads/pdf/latest/
     validator = Draft7Validator(schema_dict, registry=create_registry())
 
     validator.check_schema(schema_dict)
     if validator.is_valid(_dict):
         return _dict
 
-    print(filename + " is invalid:")
+    print()
+    print("Error: file doesn't pass JSON schema validation: " + file)
+    # print(filename + " is invalid:")
     for error in validator.iter_errors(_dict):
         # print(vars(error)) # use to look at what other attributes are available...
         print(" * json path: /" + '.'.join(error.path))
         print(" * error: " + error.message)
     print("If needed, please use VSCode to see validation errors w/ squiggles & hovers")
     sys.exit()
 
@@ -132,16 +136,21 @@
     validator = Draft7Validator(_dict, registry=create_registry())
     validator.check_schema(_dict)
 
 
 def read_json(filename):
     if not os.path.exists(filename):
         return None
-    with open(filename, 'r') as f:
-        return json.load(f)
+    try:
+        with open(filename, 'r') as f:
+            return json.load(f)
+    except JSONDecodeError as e:
+        print()
+        print(type(e).__name__ + " " + str(e))
+        raise click.ClickException("unable to load file as JSON: " + filename)
 
 
 def parse_json(json_string):
     try:
         _json = json.loads(json_string)
     except ValueError:  # includes simplejson.decoder.JSONDecodeError
         return None
```

### Comparing `rc3-0.0.3/src/rc3/common/print_helper.py` & `rc3-0.0.4/src/rc3/common/print_helper.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,15 +44,16 @@
             print_text(response)
         # ignore broken pipes
 
 
 def print_text(response):
     try:
         if len(response.text) == 0:
-            pass
+            print("Status: " + str(response.status_code))
+            print("No response body.")
         else:
             print(response.text)
     except socket.error as e:
         if e.errno != errno.EPIPE:
             raise
         # ignore broken pipes
```

### Comparing `rc3-0.0.3/src/rc3/data/collection/examples/example_Auth_Bearer.request` & `rc3-0.0.4/src/rc3/data/collection/examples/example_Auth_Bearer.request`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.875%*

 * *Differences: {"'$schema'": "'https://json.schemastore.org/rc3-request-0.0.3.json'"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "$schema": "http://localhost:8000/rc3-request-0.0.3.json",
+    "$schema": "https://json.schemastore.org/rc3-request-0.0.3.json",
     "auth": {
         "bearer_token": "eyJraWQiOiJjMWU3MTIyYi0xZGNjLTQ0NGUtYTIxYS0yNzE5NjkzOTAzNTciLCJhbGciOiJSUzI1NiJ9.eyJzdWIiOiJncmVldGluZ3MtYWRtaW4iLCJhdWQiOiJncmVldGluZ3MtYWRtaW4iLCJuYmYiOjE3MTQ0MzA1MjcsInNjb3BlIjpbImdyZWV0aW5ncy53cml0ZSJdLCJpc3MiOiJodHRwOi8vbG9jYWxob3N0OjkwMDAiLCJleHAiOjE3MTQ0MzQxMjcsImlhdCI6MTcxNDQzMDUyNywianRpIjoiMzEyMGVmZGItMTdhZS00YTYwLTlmY2QtZDQxNWViZmU1NTU1In0.yjJXlMqXZdLc6prXpXhgV7R2vNxC0AunKEru1Ua3n57Gw4K471hHv7LVssX8j9pYQtdw5W6-XzyIBVirgErE2RbnypChfA5EjJrj0jCD0BF5DOfcowkb6NOTsqqB7qtvaCm2VPO48jpWuyOsKBaZ3GP-cVqOyCeYypyYMg620tqPU-ZAMLqEz8Xxp12fpEaWncnm5_dBVzXTmZP9iqp4VvH0uXKZ9WSLvl7QmUSudkBUJTxTelkMglkHoLUgtJpM1ZpL_F2MtQs2ZDL_BM2Oycq8KCF9iDq8F0k3TXadigz4tpAn39nir1kh1aBssig1KYkl8Hu8n6gSD1nFNO1mrw",
         "type": "bearer"
     },
     "method": "GET",
     "url": "http://localhost:8080/v3/greetings/1"
 }
```

### Comparing `rc3-0.0.3/src/rc3/data/collection/examples/example_Auth_Token.request` & `rc3-0.0.4/temp-collection/examples/example_Auth_Bearer.request`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.765625%*

 * *Differences: {"'$schema'": "'https://json.schemastore.org/rc3-request-0.0.3.json'",*

 * * "'auth'": "{'type': 'bearer', 'bearer_token': "*

 * *           "'eyJraWQiOiJjMWU3MTIyYi0xZGNjLTQ0NGUtYTIxYS0yNzE5NjkzOTAzNTciLCJhbGciOiJSUzI1NiJ9.eyJzdWIiOiJncmVldGluZ3MtYWRtaW4iLCJhdWQiOiJncmVldGluZ3MtYWRtaW4iLCJuYmYiOjE3MTQ0MzA1MjcsInNjb3BlIjpbImdyZWV0aW5ncy53cml0ZSJdLCJpc3MiOiJodHRwOi8vbG9jYWxob3N0OjkwMDAiLCJleHAiOjE3MTQ0MzQxMjcsImlhdCI6MTcxNDQzMDUyNywianRpIjoiMzEyMGVmZGItMTdhZS00YTYwLTlmY2QtZDQxNWViZmU1NTU1In0.yjJXlMqXZdLc6prXpXhgV7R2vN […]*

```diff
@@ -1,10 +1,9 @@
 {
-    "$schema": "http://localhost:8000/rc3-request-0.0.3.json",
+    "$schema": "https://json.schemastore.org/rc3-request-0.0.3.json",
     "auth": {
-        "token_header": "Authorization",
-        "token_value": "Bearer eyJraWQiOiJjMWU3MTIyYi0xZGNjLTQ0NGUtYTIxYS0yNzE5NjkzOTAzNTciLCJhbGciOiJSUzI1NiJ9.eyJzdWIiOiJncmVldGluZ3MtYWRtaW4iLCJhdWQiOiJncmVldGluZ3MtYWRtaW4iLCJuYmYiOjE3MTQ0MzA1MjcsInNjb3BlIjpbImdyZWV0aW5ncy53cml0ZSJdLCJpc3MiOiJodHRwOi8vbG9jYWxob3N0OjkwMDAiLCJleHAiOjE3MTQ0MzQxMjcsImlhdCI6MTcxNDQzMDUyNywianRpIjoiMzEyMGVmZGItMTdhZS00YTYwLTlmY2QtZDQxNWViZmU1NTU1In0.yjJXlMqXZdLc6prXpXhgV7R2vNxC0AunKEru1Ua3n57Gw4K471hHv7LVssX8j9pYQtdw5W6-XzyIBVirgErE2RbnypChfA5EjJrj0jCD0BF5DOfcowkb6NOTsqqB7qtvaCm2VPO48jpWuyOsKBaZ3GP-cVqOyCeYypyYMg620tqPU-ZAMLqEz8Xxp12fpEaWncnm5_dBVzXTmZP9iqp4VvH0uXKZ9WSLvl7QmUSudkBUJTxTelkMglkHoLUgtJpM1ZpL_F2MtQs2ZDL_BM2Oycq8KCF9iDq8F0k3TXadigz4tpAn39nir1kh1aBssig1KYkl8Hu8n6gSD1nFNO1mrw",
-        "type": "token"
+        "bearer_token": "eyJraWQiOiJjMWU3MTIyYi0xZGNjLTQ0NGUtYTIxYS0yNzE5NjkzOTAzNTciLCJhbGciOiJSUzI1NiJ9.eyJzdWIiOiJncmVldGluZ3MtYWRtaW4iLCJhdWQiOiJncmVldGluZ3MtYWRtaW4iLCJuYmYiOjE3MTQ0MzA1MjcsInNjb3BlIjpbImdyZWV0aW5ncy53cml0ZSJdLCJpc3MiOiJodHRwOi8vbG9jYWxob3N0OjkwMDAiLCJleHAiOjE3MTQ0MzQxMjcsImlhdCI6MTcxNDQzMDUyNywianRpIjoiMzEyMGVmZGItMTdhZS00YTYwLTlmY2QtZDQxNWViZmU1NTU1In0.yjJXlMqXZdLc6prXpXhgV7R2vNxC0AunKEru1Ua3n57Gw4K471hHv7LVssX8j9pYQtdw5W6-XzyIBVirgErE2RbnypChfA5EjJrj0jCD0BF5DOfcowkb6NOTsqqB7qtvaCm2VPO48jpWuyOsKBaZ3GP-cVqOyCeYypyYMg620tqPU-ZAMLqEz8Xxp12fpEaWncnm5_dBVzXTmZP9iqp4VvH0uXKZ9WSLvl7QmUSudkBUJTxTelkMglkHoLUgtJpM1ZpL_F2MtQs2ZDL_BM2Oycq8KCF9iDq8F0k3TXadigz4tpAn39nir1kh1aBssig1KYkl8Hu8n6gSD1nFNO1mrw",
+        "type": "bearer"
     },
     "method": "GET",
     "url": "http://localhost:8080/v3/greetings/1"
 }
```

### Comparing `rc3-0.0.3/src/rc3/data/collection/examples/example_KitchenSink.request` & `rc3-0.0.4/src/rc3/data/collection/examples/example_KitchenSink.request`

 * *Files 17% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.95%*

 * *Differences: {"'$schema'": "'https://json.schemastore.org/rc3-request-0.0.3.json'"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "$schema": "http://localhost:8000/rc3-request-0.0.3.json",
+    "$schema": "https://json.schemastore.org/rc3-request-0.0.3.json",
     "auth": {
         "password": "is-cool",
         "type": "basic",
         "username": "gary"
     },
     "body": {
         "json": {
```

### Comparing `rc3-0.0.3/src/rc3/data/home/schemas/rc3-auth-0.0.3.json` & `rc3-0.0.4/src/rc3/data/home/schemas/rc3-auth-0.0.3.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9285714285714286%*

 * *Differences: {"'$id'": "'https://json.schemastore.org/rc3-auth-0.0.3.json'"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "$id": "http://localhost:8000/rc3-auth-0.0.3.json",
+    "$id": "https://json.schemastore.org/rc3-auth-0.0.3.json",
     "$schema": "http://json-schema.org/draft-07/schema#",
     "additionalProperties": false,
     "description": "RC auth that can be stored at Collection, Folder, or Request levels",
     "properties": {
         "bearer_token": {
             "description": "The bearer token (for bearer auth type)",
             "type": "string"
```

### Comparing `rc3-0.0.3/src/rc3/data/home/schemas/rc3-collection-0.0.3.json` & `rc3-0.0.4/src/rc3/data/home/schemas/rc3-collection-0.0.3.json`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9249999999999999%*

 * *Differences: {"'$id'": "'https://json.schemastore.org/rc3-collection-0.0.3.json'",*

 * * "'properties'": "{'auth': {'$ref': 'https://json.schemastore.org/rc3-auth-0.0.3.json'}}"}*

```diff
@@ -1,19 +1,19 @@
 {
-    "$id": "http://localhost:8000/rc3-collection-0.0.3.json",
+    "$id": "https://json.schemastore.org/rc3-collection-0.0.3.json",
     "$schema": "http://json-schema.org/draft-07/schema#",
     "additionalProperties": false,
     "description": "RC collection information",
     "properties": {
         "$schema": {
             "description": "The JSON schema to use for validation",
             "type": "string"
         },
         "auth": {
-            "$ref": "http://localhost:8000/rc3-auth-0.0.3.json"
+            "$ref": "https://json.schemastore.org/rc3-auth-0.0.3.json"
         },
         "current_environment": {
             "description": "The current environment in the collection",
             "type": "string"
         },
         "current_request": {
             "description": "The current request in the collection",
```

### Comparing `rc3-0.0.3/src/rc3/data/home/schemas/rc3-folder-0.0.3.json` & `rc3-0.0.4/src/rc3/data/home/schemas/rc3-folder-0.0.3.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9226190476190476%*

 * *Differences: {"'$id'": "'https://json.schemastore.org/rc3-folder-0.0.3.json'",*

 * * "'properties'": "{'auth': {'$ref': 'https://json.schemastore.org/rc3-auth-0.0.3.json'}}"}*

```diff
@@ -1,19 +1,19 @@
 {
-    "$id": "http://localhost:8000/rc3-folder-0.0.3.json",
+    "$id": "https://json.schemastore.org/rc3-folder-0.0.3.json",
     "$schema": "http://json-schema.org/draft-07/schema#",
     "additionalProperties": false,
     "description": "RC folder information",
     "properties": {
         "$schema": {
             "description": "The JSON schema to use for validation",
             "type": "string"
         },
         "auth": {
-            "$ref": "http://localhost:8000/rc3-auth-0.0.3.json"
+            "$ref": "https://json.schemastore.org/rc3-auth-0.0.3.json"
         },
         "comment": {
             "description": "Ummm",
             "type": "string"
         }
     },
     "title": "rc3 folder",
```

### Comparing `rc3-0.0.3/src/rc3/data/home/schemas/rc3-request-0.0.3.json` & `rc3-0.0.4/src/rc3/data/home/schemas/rc3-request-0.0.3.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9360795454545454%*

 * *Differences: {"'$id'": "'https://json.schemastore.org/rc3-request-0.0.3.json'",*

 * * "'properties'": "{'auth': {'$ref': 'https://json.schemastore.org/rc3-auth-0.0.3.json'}}"}*

```diff
@@ -8,25 +8,25 @@
                 "name": {
                     "type": "string"
                 }
             },
             "type": "object"
         }
     },
-    "$id": "http://localhost:8000/rc3-request-0.0.3.json",
+    "$id": "https://json.schemastore.org/rc3-request-0.0.3.json",
     "$schema": "http://json-schema.org/draft-07/schema#",
     "additionalProperties": false,
     "description": "RC request information",
     "properties": {
         "$schema": {
             "description": "The JSON schema to use for validation",
             "type": "string"
         },
         "auth": {
-            "$ref": "http://localhost:8000/rc3-auth-0.0.3.json"
+            "$ref": "https://json.schemastore.org/rc3-auth-0.0.3.json"
         },
         "body": {
             "additionalProperties": false,
             "description": "The body of the request",
             "properties": {
                 "json": {
                     "type": "object"
```

### Comparing `rc3-0.0.3/src/rc3/data/home/schemas/rc3-settings-0.0.3.json` & `rc3-0.0.4/src/rc3/data/home/schemas/rc3-settings-0.0.3.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9375%*

 * *Differences: {"'$id'": "'https://json.schemastore.org/rc3-settings-0.0.3.json'"}*

```diff
@@ -9,15 +9,15 @@
                 "name": {
                     "type": "string"
                 }
             },
             "type": "object"
         }
     },
-    "$id": "http://localhost:8000/rc3-settings-0.0.3.json",
+    "$id": "https://json.schemastore.org/rc3-settings-0.0.3.json",
     "$schema": "http://json-schema.org/draft-07/schema#",
     "additionalProperties": false,
     "description": "RC settings stored in the users RC_HOME directory",
     "properties": {
         "$schema": {
             "description": "The JSON schema to use for validation",
             "type": "string"
```

### Comparing `rc3-0.0.3/src/rc3.egg-info/PKG-INFO` & `rc3-0.0.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rc3
-Version: 0.0.3
+Version: 0.0.4
 Summary: Rest CLI (rc)
 Author-email: Gary Wilcox <gary@dugan-wilcox.com>
 License: MIT License
         
         Copyright (c) 2018 Real Python
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -25,15 +25,15 @@
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
 Project-URL: repository, https://github.com/gswilcox01/rc3
 Keywords: rest,cli,postman
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: click>=8.1
 Requires-Dist: requests>=2.31
 Requires-Dist: jsonschema
 Requires-Dist: jsonpath-ng
 Requires-Dist: funcy
@@ -59,53 +59,95 @@
 
 ## Installation
 * Pre-reqs
     * Python 3.12+ (required)
     * VSCode (optional, but highly recommended)
 * Install
     * pip install rc3
+* Windows User?
+    * See:  [Windows Setup Issues](WINDOWS_SETUP.md)
 
-## RC Setup & Sending your first request
-* mkdir example-collection
-* cd example-collection
-* rc init
-    * Will do 0-4 things
-      1. Will create the RC_HOME directory if it doesn't exist.
-      2. Will create RC_HOME/settings, global env, and schemas dir if they don't exist.
-      3. Will initialize a new example Collection if ran from an empty directory.
-      4. Will import the current directory if it contains a valid collection.json file.
-* rc send greeting
-    * Will send the first request named "greeting" in the example Collection
-    * Wait for it…  
-      * A greetings-demo project is running on Google Cloud Run
-      * And it scales down to 0 instances when there is no demand (i.e. your first few requests will be SLOW…)
-* cat greetings-basic/greeting.response
-    * Will show more verbose output from the "rc send greeting" cmd you just sent
+## Setup & Sending your first request
+* First create an empty directory somewhere (any name & location is fine)
+  ```
+  $ mkdir temp-collection
+  $ cd temp-collection
+  ```
+* Next run "rc init" to do 0-4 things
+  1. Will create the RC_HOME directory if it doesn't exist.
+  2. Will create RC_HOME/settings, global env, and schemas dir if they don't exist.
+  3. Will initialize a new example Collection if ran from an empty directory.
+  4. Will import the current directory if it contains a valid collection.json file.
+  ```
+  $ rc init
+  Creating C:\Users\Gary\.rc\rc-settings.json
+  Creating C:\Users\Gary\.rc\rc-global.json                            
+  Creating C:\Users\Gary\.rc\schemas                                   
+  CWD is empty, creating sample Collection here: C:\dev\temp-collection
+  Importing collection from: C:\dev\temp-collection
+  Adding collection to global settings: example-collection
+  ```
+* Next send the "greeting" request with the rc send command
+  * Wait for it…
+    * A greetings-demo project is running on Google Cloud Run
+    * And it scales down to 0 instances when there is no demand (i.e. your first few requests will be SLOW…)  
+  ```
+  $ rc send greeting
+  {                        
+      "id": 1,             
+      "text": "Hello",     
+      "language": "English"
+  }
+  ```
+* Next "cat" the generated greeting.response file that will have more verbose output from the send command
+  ```
+  $ cat greetings-basic/greeting.response
+  {                                                                                     
+    "status_code": 200,                                                               
+    "time": "845.772ms",                                                              
+    "size": {                                                                         
+        "body": 44,                                                                   
+        "headers": 442,                                                               
+        "total": 486                                                                  
+    },                                                                                
+    "headers": {                                                                      
+        "vary": "Origin,Access-Control-Request-Method,Access-Control-Request-Headers",
+        "Date": "Wed, 08 May 2024 15:06:54 GMT",                                      
+        "Server": "Google Frontend",
+  
+    ...
+                                                    
+  }
+  ``` 
 
 ## Sending more requests from the example collection
-* All the requests in the example collection can be sent to the greetings-demo app
+* All the requests in the example collection can be sent to the greetings-demo app running on Google Cloud Run
+* To view all requests in the example collection run "rc request --list"
   ```
+  $ rc request --list
   Listing REQUESTS found in current_collection:
-  NUM:   FOLDER:             MET:     NAME:              
+  NUM:   FOLDER:             METHOD:  NAME:              
   1*     /greetings-basic    GET      greeting
   2      /greetings-basic    GET      greetings
   3      /greetings-basic    POST     new-greeting
   4      /greetings-basic    DELETE   remove-greeting
   5      /greetings-basic    PUT      update-greeting
   6      /greetings-oauth2   GET      greeting
   7      /greetings-oauth2   POST     mint-admin-token
   8      /greetings-oauth2   POST     mint-token
   ```
-* For example:
-    * rc send 1
-    * rc send 2
-    * rc send 3
+* Try sending requests by NUMBER instead of by NAME using these commands:
+  ```
+  $ rc send 1
+  $ rc send 2
+  $ rc send 3
+  ```
 * Notes:
   * Make sure there is a greeting #8 before sending request 4, or you'll get a 404
-  * Make sure you run request 7, before request 6, so you have an access_token
+  * Make sure you run request 7, before request 6, so you have a {{ token }} available in your global environment
 
 ## More command examples
 * View all Collections, Environments, and Requests you have setup on this machine
     * rc list
 * View all Requests for the current Collection (the following commands are equivalent):
     * rc list requests
     * rc list r
@@ -201,17 +243,17 @@
 
 ## CA certificates:
 * By default rc will follow Python Requests default behaviour
   * Using the Python 'certifi' module truststore file
   * And verifying certs
 * You can turn off cert verification in RC_HOME/settings.json with:
   * "ca_cert_verification": false,
-* You can set a custom cert ca_bundle file with:
+* You can set a custom cert ca_bundle file in RC_HOME/settings.json with:
   * "ca_bundle": "/path/to/ca/bundlefile",
-* You can alternativelly set the path to a ca_bundle file with one of these ENV VARS:
+* You can alternatively set the path to a ca_bundle file with one of these ENV VARS:
   * REQUESTS_CA_BUNDLE
   * CURL_CA_BUNDLE
 * For more details see:
   * https://requests.readthedocs.io/en/latest/user/advanced/#ssl-cert-verification
 
 ## VSCode setup:
 * Associate *.request & *.response files with the JSON editor
```

### Comparing `rc3-0.0.3/src/rc3.egg-info/SOURCES.txt` & `rc3-0.0.4/src/rc3.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 .gitignore
 LICENSE
 README.md
+WINDOWS_SETUP.md
 pyproject.toml
 rc3.iml
 src/rc3/__init__.py
 src/rc3/cli.py
 src/rc3.egg-info/PKG-INFO
 src/rc3.egg-info/SOURCES.txt
 src/rc3.egg-info/dependency_links.txt
@@ -14,14 +15,15 @@
 src/rc3/archive/__init__.py
 src/rc3/archive/cmd_home.py
 src/rc3/archive/cmd_root.py
 src/rc3/archive/cmd_subs.py
 src/rc3/commands/__init__.py
 src/rc3/commands/cmd_collection.py
 src/rc3/commands/cmd_environment.py
+src/rc3/commands/cmd_global.py
 src/rc3/commands/cmd_hello.py
 src/rc3/commands/cmd_init.py
 src/rc3/commands/cmd_list.py
 src/rc3/commands/cmd_request.py
 src/rc3/commands/cmd_send.py
 src/rc3/commands/cmd_settings.py
 src/rc3/common/__init__.py
@@ -84,22 +86,18 @@
 temp-collection/examples/example_UseOauth2Token.request
 temp-collection/examples/folder.json
 temp-collection/greetings-basic/greeting.request
 temp-collection/greetings-basic/greeting.response
 temp-collection/greetings-basic/greetings.request
 temp-collection/greetings-basic/greetings.response
 temp-collection/greetings-basic/new-greeting.request
-temp-collection/greetings-basic/new-greeting.response
 temp-collection/greetings-basic/rc-folder.json
 temp-collection/greetings-basic/remove-greeting.request
-temp-collection/greetings-basic/remove-greeting.response
 temp-collection/greetings-basic/update-greeting.request
-temp-collection/greetings-basic/update-greeting.response
 temp-collection/greetings-oauth2/greeting.request
-temp-collection/greetings-oauth2/greeting.response
 temp-collection/greetings-oauth2/mint-admin-token.request
 temp-collection/greetings-oauth2/mint-token.request
 tests/__init__.py
 tests/conftest.py
 tests/test_cli.py
 tests/commands/__init__.py
 tests/commands/test_collection.py
```

### Comparing `rc3-0.0.3/temp-collection/examples/example_Auth_Bearer.request` & `rc3-0.0.4/src/rc3/data/collection/examples/example_Auth_Token.request`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.765625%*

 * *Differences: {"'$schema'": "'https://json.schemastore.org/rc3-request-0.0.3.json'",*

 * * "'auth'": "{'type': 'token', 'token_header': 'Authorization', 'token_value': 'Bearer "*

 * *           "eyJraWQiOiJjMWU3MTIyYi0xZGNjLTQ0NGUtYTIxYS0yNzE5NjkzOTAzNTciLCJhbGciOiJSUzI1NiJ9.eyJzdWIiOiJncmVldGluZ3MtYWRtaW4iLCJhdWQiOiJncmVldGluZ3MtYWRtaW4iLCJuYmYiOjE3MTQ0MzA1MjcsInNjb3BlIjpbImdyZWV0aW5ncy53cml0ZSJdLCJpc3MiOiJodHRwOi8vbG9jYWxob3N0OjkwMDAiLCJleHAiOjE3MTQ0MzQxMjcsImlhdCI6MTcxNDQzMDUyNywianRpIjoiMzEyMGVmZGItMTdhZS00YTYwLTlmY2QtZDQxNWVi […]*

```diff
@@ -1,9 +1,10 @@
 {
-    "$schema": "http://localhost:8000/rc3-request-0.0.3.json",
+    "$schema": "https://json.schemastore.org/rc3-request-0.0.3.json",
     "auth": {
-        "bearer_token": "eyJraWQiOiJjMWU3MTIyYi0xZGNjLTQ0NGUtYTIxYS0yNzE5NjkzOTAzNTciLCJhbGciOiJSUzI1NiJ9.eyJzdWIiOiJncmVldGluZ3MtYWRtaW4iLCJhdWQiOiJncmVldGluZ3MtYWRtaW4iLCJuYmYiOjE3MTQ0MzA1MjcsInNjb3BlIjpbImdyZWV0aW5ncy53cml0ZSJdLCJpc3MiOiJodHRwOi8vbG9jYWxob3N0OjkwMDAiLCJleHAiOjE3MTQ0MzQxMjcsImlhdCI6MTcxNDQzMDUyNywianRpIjoiMzEyMGVmZGItMTdhZS00YTYwLTlmY2QtZDQxNWViZmU1NTU1In0.yjJXlMqXZdLc6prXpXhgV7R2vNxC0AunKEru1Ua3n57Gw4K471hHv7LVssX8j9pYQtdw5W6-XzyIBVirgErE2RbnypChfA5EjJrj0jCD0BF5DOfcowkb6NOTsqqB7qtvaCm2VPO48jpWuyOsKBaZ3GP-cVqOyCeYypyYMg620tqPU-ZAMLqEz8Xxp12fpEaWncnm5_dBVzXTmZP9iqp4VvH0uXKZ9WSLvl7QmUSudkBUJTxTelkMglkHoLUgtJpM1ZpL_F2MtQs2ZDL_BM2Oycq8KCF9iDq8F0k3TXadigz4tpAn39nir1kh1aBssig1KYkl8Hu8n6gSD1nFNO1mrw",
-        "type": "bearer"
+        "token_header": "Authorization",
+        "token_value": "Bearer eyJraWQiOiJjMWU3MTIyYi0xZGNjLTQ0NGUtYTIxYS0yNzE5NjkzOTAzNTciLCJhbGciOiJSUzI1NiJ9.eyJzdWIiOiJncmVldGluZ3MtYWRtaW4iLCJhdWQiOiJncmVldGluZ3MtYWRtaW4iLCJuYmYiOjE3MTQ0MzA1MjcsInNjb3BlIjpbImdyZWV0aW5ncy53cml0ZSJdLCJpc3MiOiJodHRwOi8vbG9jYWxob3N0OjkwMDAiLCJleHAiOjE3MTQ0MzQxMjcsImlhdCI6MTcxNDQzMDUyNywianRpIjoiMzEyMGVmZGItMTdhZS00YTYwLTlmY2QtZDQxNWViZmU1NTU1In0.yjJXlMqXZdLc6prXpXhgV7R2vNxC0AunKEru1Ua3n57Gw4K471hHv7LVssX8j9pYQtdw5W6-XzyIBVirgErE2RbnypChfA5EjJrj0jCD0BF5DOfcowkb6NOTsqqB7qtvaCm2VPO48jpWuyOsKBaZ3GP-cVqOyCeYypyYMg620tqPU-ZAMLqEz8Xxp12fpEaWncnm5_dBVzXTmZP9iqp4VvH0uXKZ9WSLvl7QmUSudkBUJTxTelkMglkHoLUgtJpM1ZpL_F2MtQs2ZDL_BM2Oycq8KCF9iDq8F0k3TXadigz4tpAn39nir1kh1aBssig1KYkl8Hu8n6gSD1nFNO1mrw",
+        "type": "token"
     },
     "method": "GET",
     "url": "http://localhost:8080/v3/greetings/1"
 }
```

### Comparing `rc3-0.0.3/temp-collection/examples/example_Auth_Token.request` & `rc3-0.0.4/temp-collection/examples/example_Auth_Token.request`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.875%*

 * *Differences: {"'$schema'": "'https://json.schemastore.org/rc3-request-0.0.3.json'"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "$schema": "http://localhost:8000/rc3-request-0.0.3.json",
+    "$schema": "https://json.schemastore.org/rc3-request-0.0.3.json",
     "auth": {
         "token_header": "Authorization",
         "token_value": "Bearer eyJraWQiOiJjMWU3MTIyYi0xZGNjLTQ0NGUtYTIxYS0yNzE5NjkzOTAzNTciLCJhbGciOiJSUzI1NiJ9.eyJzdWIiOiJncmVldGluZ3MtYWRtaW4iLCJhdWQiOiJncmVldGluZ3MtYWRtaW4iLCJuYmYiOjE3MTQ0MzA1MjcsInNjb3BlIjpbImdyZWV0aW5ncy53cml0ZSJdLCJpc3MiOiJodHRwOi8vbG9jYWxob3N0OjkwMDAiLCJleHAiOjE3MTQ0MzQxMjcsImlhdCI6MTcxNDQzMDUyNywianRpIjoiMzEyMGVmZGItMTdhZS00YTYwLTlmY2QtZDQxNWViZmU1NTU1In0.yjJXlMqXZdLc6prXpXhgV7R2vNxC0AunKEru1Ua3n57Gw4K471hHv7LVssX8j9pYQtdw5W6-XzyIBVirgErE2RbnypChfA5EjJrj0jCD0BF5DOfcowkb6NOTsqqB7qtvaCm2VPO48jpWuyOsKBaZ3GP-cVqOyCeYypyYMg620tqPU-ZAMLqEz8Xxp12fpEaWncnm5_dBVzXTmZP9iqp4VvH0uXKZ9WSLvl7QmUSudkBUJTxTelkMglkHoLUgtJpM1ZpL_F2MtQs2ZDL_BM2Oycq8KCF9iDq8F0k3TXadigz4tpAn39nir1kh1aBssig1KYkl8Hu8n6gSD1nFNO1mrw",
         "type": "token"
     },
     "method": "GET",
     "url": "http://localhost:8080/v3/greetings/1"
```

### Comparing `rc3-0.0.3/temp-collection/examples/example_KitchenSink.request` & `rc3-0.0.4/temp-collection/examples/example_KitchenSink.request`

 * *Files 17% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.95%*

 * *Differences: {"'$schema'": "'https://json.schemastore.org/rc3-request-0.0.3.json'"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "$schema": "http://localhost:8000/rc3-request-0.0.3.json",
+    "$schema": "https://json.schemastore.org/rc3-request-0.0.3.json",
     "auth": {
         "password": "is-cool",
         "type": "basic",
         "username": "gary"
     },
     "body": {
         "json": {
```

### Comparing `rc3-0.0.3/temp-collection/greetings-basic/greeting.response` & `rc3-0.0.4/temp-collection/greetings-basic/greeting.response`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9138888888888889%*

 * *Differences: {"'headers'": "{'Date': 'Wed, 08 May 2024 19:32:46 GMT'}", "'time'": "'581.414ms'"}*

```diff
@@ -5,15 +5,15 @@
             "language": "English",
             "text": "Hello"
         }
     },
     "extract_errors": [],
     "headers": {
         "Alt-Svc": "h3=\":443\"; ma=2592000,h3-29=\":443\"; ma=2592000",
-        "Date": "Mon, 06 May 2024 22:57:40 GMT",
+        "Date": "Wed, 08 May 2024 19:32:46 GMT",
         "Server": "Google Frontend",
         "Transfer-Encoding": "chunked",
         "cache-control": "no-cache, no-store, max-age=0, must-revalidate",
         "content-type": "application/json",
         "expires": "0",
         "pragma": "no-cache",
         "set-cookie": "search=bob*, page=2, page_size=100",
@@ -26,9 +26,9 @@
     },
     "size": {
         "body": 44,
         "headers": 442,
         "total": 486
     },
     "status_code": 200,
-    "time": "603.421ms"
+    "time": "581.414ms"
 }
```

### Comparing `rc3-0.0.3/temp-collection/greetings-basic/greetings.response` & `rc3-0.0.4/temp-collection/greetings-basic/greetings.response`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9131944444444445%*

 * *Differences: {"'headers'": "{'Date': 'Wed, 08 May 2024 19:32:39 GMT'}", "'time'": "'605.681ms'"}*

```diff
@@ -27,15 +27,15 @@
                 "text": "Hej"
             }
         ]
     },
     "extract_errors": [],
     "headers": {
         "Alt-Svc": "h3=\":443\"; ma=2592000,h3-29=\":443\"; ma=2592000",
-        "Date": "Mon, 06 May 2024 23:33:37 GMT",
+        "Date": "Wed, 08 May 2024 19:32:39 GMT",
         "Server": "Google Frontend",
         "Transfer-Encoding": "chunked",
         "cache-control": "no-cache, no-store, max-age=0, must-revalidate",
         "content-type": "application/json",
         "expires": "0",
         "pragma": "no-cache",
         "vary": "Origin,Access-Control-Request-Method,Access-Control-Request-Headers",
@@ -45,9 +45,9 @@
     },
     "size": {
         "body": 222,
         "headers": 376,
         "total": 598
     },
     "status_code": 200,
-    "time": "189.219ms"
+    "time": "605.681ms"
 }
```

### Comparing `rc3-0.0.3/tests/commands/test_collection.py` & `rc3-0.0.4/tests/commands/test_collection.py`

 * *Files identical despite different names*

### Comparing `rc3-0.0.3/tests/commands/test_environment.py` & `rc3-0.0.4/tests/commands/test_environment.py`

 * *Files identical despite different names*

### Comparing `rc3-0.0.3/tests/commands/test_init.py` & `rc3-0.0.4/tests/commands/test_init.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     assert os.listdir(rc_home) == [GLOBAL_ENV_FILENAME, SETTINGS_FILENAME, 'schemas']
     assert os.listdir(clean_empty) == ['environments',
                                        'examples',
                                        'greetings-basic',
                                        'greetings-oauth2',
                                        COLLECTION_FILENAME]
     settings = json_helper.read_settings()
-    assert settings.get('current_collection') == "c1"
+    assert settings.get('current_collection') == "example-collection"
 
 
 def test_init_from_NOT_empty(clean_home, clean_empty, runner):
     # pre-test RC_HOME doesn't exist
     rc_home = os.path.join(clean_home, '.rc')
     assert not os.path.exists(rc_home)
```

### Comparing `rc3-0.0.3/tests/commands/test_request.py` & `rc3-0.0.4/tests/commands/test_request.py`

 * *Files identical despite different names*

### Comparing `rc3-0.0.3/tests/commands/test_send.py` & `rc3-0.0.4/tests/commands/test_send.py`

 * *Files identical despite different names*

### Comparing `rc3-0.0.3/tests/commands/test_send_files/test_mint_extract_use_token.yaml` & `rc3-0.0.4/tests/commands/test_send_files/test_mint_extract_use_token.yaml`

 * *Files identical despite different names*

### Comparing `rc3-0.0.3/tests/commands/test_send_files/test_send_2.yaml` & `rc3-0.0.4/tests/commands/test_send_files/test_send_2.yaml`

 * *Files identical despite different names*

### Comparing `rc3-0.0.3/tests/commands/test_send_files/test_send_basics.yaml` & `rc3-0.0.4/tests/commands/test_send_files/test_send_basics.yaml`

 * *Files identical despite different names*

### Comparing `rc3-0.0.3/tests/common/test_env_helper.py` & `rc3-0.0.4/tests/common/test_env_helper.py`

 * *Files identical despite different names*

### Comparing `rc3-0.0.3/tests/common/test_inherit_helper.py` & `rc3-0.0.4/tests/common/test_inherit_helper.py`

 * *Files identical despite different names*

### Comparing `rc3-0.0.3/tests/conftest.py` & `rc3-0.0.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `rc3-0.0.3/tests/learning/test_sample.py` & `rc3-0.0.4/tests/learning/test_sample.py`

 * *Files identical despite different names*

### Comparing `rc3-0.0.3/tests/test_cli.py` & `rc3-0.0.4/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `rc3-0.0.3/tests/util/decorators.py` & `rc3-0.0.4/tests/util/decorators.py`

 * *Files identical despite different names*

