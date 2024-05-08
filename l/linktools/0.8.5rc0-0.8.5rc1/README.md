# Comparing `tmp/linktools-0.8.5rc0.tar.gz` & `tmp/linktools-0.8.5rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linktools-0.8.5rc0.tar", last modified: Wed Apr 24 02:46:12 2024, max compression
+gzip compressed data, was "linktools-0.8.5rc1.tar", last modified: Sun May  5 10:14:27 2024, max compression
```

## Comparing `linktools-0.8.5rc0.tar` & `linktools-0.8.5rc1.tar`

### file list

```diff
@@ -1,129 +1,129 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:46:12.554604 linktools-0.8.5rc0/
--rw-r--r--   0 runner    (1001) docker     (127)    11895 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    35049 2024-04-24 02:46:12.554604 linktools-0.8.5rc0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    32999 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 02:46:12.554604 linktools-0.8.5rc0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     4278 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:46:12.534603 linktools-0.8.5rc0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:46:12.538604 linktools-0.8.5rc0/src/linktools/
--rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21680 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    12574 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/_environ.py
--rw-r--r--   0 runner    (1001) docker     (127)    17823 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)    11014 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/_url.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:46:12.538604 linktools-0.8.5rc0/src/linktools/android/
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/android/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23865 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/android/adb.py
--rw-r--r--   0 runner    (1001) docker     (127)    13360 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/android/struct.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:46:12.542604 linktools-0.8.5rc0/src/linktools/assets/
--rw-r--r--   0 runner    (1001) docker     (127)    82987 2024-04-24 02:46:03.000000 linktools-0.8.5rc0/src/linktools/assets/android-tools.apk
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-24 02:46:03.000000 linktools-0.8.5rc0/src/linktools/assets/android-tools.json
--rw-r--r--   0 runner    (1001) docker     (127)      881 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/assets/chrome-driver.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:46:12.534603 linktools-0.8.5rc0/src/linktools/assets/containers/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:46:12.542604 linktools-0.8.5rc0/src/linktools/assets/containers/100-nginx/
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/assets/containers/100-nginx/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/assets/containers/100-nginx/compose.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3219 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/assets/containers/100-nginx/container.py
--rw-r--r--   0 runner    (1001) docker     (127)    47272 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/assets/containers/100-nginx/dnsapi.txt
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/assets/containers/100-nginx/http.conf
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/assets/containers/100-nginx/https.conf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:46:12.542604 linktools-0.8.5rc0/src/linktools/assets/containers/110-portainer/
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/assets/containers/110-portainer/compose.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/assets/containers/110-portainer/container.py
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/assets/containers/110-portainer/nginx.conf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:46:12.542604 linktools-0.8.5rc0/src/linktools/assets/containers/120-flare/
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/assets/containers/120-flare/compose.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4456 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/assets/containers/120-flare/container.py
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/assets/containers/120-flare/nginx.conf
--rw-r--r--   0 runner    (1001) docker     (127)    11530 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/assets/fake_useragent.json
--rw-r--r--   0 runner    (1001) docker     (127)    44744 2024-04-24 02:44:10.000000 linktools-0.8.5rc0/src/linktools/assets/frida.js
--rw-r--r--   0 runner    (1001) docker     (127)    24005 2024-04-24 02:44:10.000000 linktools-0.8.5rc0/src/linktools/assets/frida.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:46:12.534603 linktools-0.8.5rc0/src/linktools/assets/objection/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:46:12.542604 linktools-0.8.5rc0/src/linktools/assets/objection/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)     3021 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/assets/objection/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12275 2024-04-24 02:46:12.000000 linktools-0.8.5rc0/src/linktools/assets/tools.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:46:12.542604 linktools-0.8.5rc0/src/linktools/cli/
--rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6007 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/cli/argparse.py
--rw-r--r--   0 runner    (1001) docker     (127)    31589 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/cli/command.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:46:12.542604 linktools-0.8.5rc0/src/linktools/cli/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/cli/commands/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:46:12.546604 linktools-0.8.5rc0/src/linktools/cli/commands/android/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/cli/commands/android/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2494 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/cli/commands/android/adb.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2140 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/cli/commands/android/agent.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    15066 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/cli/commands/android/app.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2614 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/cli/commands/android/debug.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6205 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/cli/commands/android/frida.py
--rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/cli/commands/android/info.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4881 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/cli/commands/android/intent.py
--rw-r--r--   0 runner    (1001) docker     (127)     5014 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/cli/commands/android/objection.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    15517 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/cli/commands/android/pidcat.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4522 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/cli/commands/android/top.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:46:12.546604 linktools-0.8.5rc0/src/linktools/cli/commands/common/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/cli/commands/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4473 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/cli/commands/common/cert.py
--rw-r--r--   0 runner    (1001) docker     (127)    15194 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/cli/commands/common/cntr.py
--rw-r--r--   0 runner    (1001) docker     (127)     7002 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/cli/commands/common/env.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7674 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/cli/commands/common/grep.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4134 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/cli/commands/common/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:46:12.546604 linktools-0.8.5rc0/src/linktools/cli/commands/ios/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/cli/commands/ios/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5332 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/cli/commands/ios/frida.py
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/cli/commands/ios/ipa.py
--rw-r--r--   0 runner    (1001) docker     (127)     4027 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/cli/commands/ios/objection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/cli/commands/ios/scp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/cli/commands/ios/sib.py
--rw-r--r--   0 runner    (1001) docker     (127)     2898 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/cli/commands/ios/ssh.py
--rw-r--r--   0 runner    (1001) docker     (127)    17530 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/cli/device.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:46:12.546604 linktools-0.8.5rc0/src/linktools/container/
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/container/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16132 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/container/container.py
--rw-r--r--   0 runner    (1001) docker     (127)    21050 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/container/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     4996 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/container/repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     5266 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/device.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:46:12.550604 linktools-0.8.5rc0/src/linktools/frida/
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/frida/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6291 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/frida/android.py
--rw-r--r--   0 runner    (1001) docker     (127)    29987 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/frida/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/frida/ios.py
--rw-r--r--   0 runner    (1001) docker     (127)     5146 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/frida/script.py
--rw-r--r--   0 runner    (1001) docker     (127)     3265 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/frida/server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:46:12.550604 linktools-0.8.5rc0/src/linktools/ida/
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/ida/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6229 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/ida/ida.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:46:12.550604 linktools-0.8.5rc0/src/linktools/ios/
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/ios/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/ios/ipa.py
--rw-r--r--   0 runner    (1001) docker     (127)     8184 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/ios/sib.py
--rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/ios/struct.py
--rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-04-24 02:46:12.000000 linktools-0.8.5rc0/src/linktools/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     4328 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/reactor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:46:12.550604 linktools-0.8.5rc0/src/linktools/references/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/references/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:46:12.550604 linktools-0.8.5rc0/src/linktools/references/fake_useragent/
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/references/fake_useragent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/references/fake_useragent/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     7962 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/references/fake_useragent/fake.py
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/references/fake_useragent/log.py
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/references/fake_useragent/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/references/fake_useragent/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    12209 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/rich.py
--rw-r--r--   0 runner    (1001) docker     (127)    13556 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/ssh.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:46:12.550604 linktools-0.8.5rc0/src/linktools/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/utils/_port.py
--rw-r--r--   0 runner    (1001) docker     (127)     8885 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/utils/_proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)     6557 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/utils/_subprocess.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    19460 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/utils/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:46:12.550604 linktools-0.8.5rc0/src/linktools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    35049 2024-04-24 02:46:12.000000 linktools-0.8.5rc0/src/linktools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3783 2024-04-24 02:46:12.000000 linktools-0.8.5rc0/src/linktools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 02:46:12.000000 linktools-0.8.5rc0/src/linktools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-24 02:46:12.000000 linktools-0.8.5rc0/src/linktools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-24 02:46:12.000000 linktools-0.8.5rc0/src/linktools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-24 02:46:12.000000 linktools-0.8.5rc0/src/linktools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:14:27.784403 linktools-0.8.5rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11895 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    35010 2024-05-05 10:14:27.784403 linktools-0.8.5rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    32960 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 10:14:27.784403 linktools-0.8.5rc1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4278 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:14:27.756403 linktools-0.8.5rc1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:14:27.764403 linktools-0.8.5rc1/src/linktools/
+-rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21680 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12751 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/_environ.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18133 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11014 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/_url.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:14:27.764403 linktools-0.8.5rc1/src/linktools/android/
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/android/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23773 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/android/adb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13360 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/android/struct.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:14:27.768403 linktools-0.8.5rc1/src/linktools/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)    82987 2024-05-05 10:14:22.000000 linktools-0.8.5rc1/src/linktools/assets/android-tools.apk
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-05 10:14:22.000000 linktools-0.8.5rc1/src/linktools/assets/android-tools.json
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/assets/chrome-driver.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:14:27.756403 linktools-0.8.5rc1/src/linktools/assets/containers/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:14:27.768403 linktools-0.8.5rc1/src/linktools/assets/containers/100-nginx/
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/assets/containers/100-nginx/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/assets/containers/100-nginx/compose.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3219 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/assets/containers/100-nginx/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47272 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/assets/containers/100-nginx/dnsapi.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/assets/containers/100-nginx/http.conf
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/assets/containers/100-nginx/https.conf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:14:27.768403 linktools-0.8.5rc1/src/linktools/assets/containers/110-portainer/
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/assets/containers/110-portainer/compose.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/assets/containers/110-portainer/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/assets/containers/110-portainer/nginx.conf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:14:27.768403 linktools-0.8.5rc1/src/linktools/assets/containers/120-flare/
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/assets/containers/120-flare/compose.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4456 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/assets/containers/120-flare/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/assets/containers/120-flare/nginx.conf
+-rw-r--r--   0 runner    (1001) docker     (127)    11530 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/assets/fake_useragent.json
+-rw-r--r--   0 runner    (1001) docker     (127)    44744 2024-05-05 10:12:12.000000 linktools-0.8.5rc1/src/linktools/assets/frida.js
+-rw-r--r--   0 runner    (1001) docker     (127)    24005 2024-05-05 10:12:12.000000 linktools-0.8.5rc1/src/linktools/assets/frida.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:14:27.760403 linktools-0.8.5rc1/src/linktools/assets/objection/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:14:27.768403 linktools-0.8.5rc1/src/linktools/assets/objection/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)     3021 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/assets/objection/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14279 2024-05-05 10:14:27.000000 linktools-0.8.5rc1/src/linktools/assets/tools.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:14:27.768403 linktools-0.8.5rc1/src/linktools/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6007 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/cli/argparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31604 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/cli/command.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:14:27.768403 linktools-0.8.5rc1/src/linktools/cli/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/cli/commands/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:14:27.772403 linktools-0.8.5rc1/src/linktools/cli/commands/android/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/cli/commands/android/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2494 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/cli/commands/android/adb.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2140 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/cli/commands/android/agent.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15066 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/cli/commands/android/app.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2614 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/cli/commands/android/debug.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6205 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/cli/commands/android/frida.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/cli/commands/android/info.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4937 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/cli/commands/android/intent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4963 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/cli/commands/android/objection.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15517 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/cli/commands/android/pidcat.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4383 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/cli/commands/android/top.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:14:27.772403 linktools-0.8.5rc1/src/linktools/cli/commands/common/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/cli/commands/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4473 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/cli/commands/common/cert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15318 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/cli/commands/common/cntr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7052 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/cli/commands/common/env.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7674 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/cli/commands/common/grep.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4143 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/cli/commands/common/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:14:27.776403 linktools-0.8.5rc1/src/linktools/cli/commands/ios/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/cli/commands/ios/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5332 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/cli/commands/ios/frida.py
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/cli/commands/ios/ipa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4027 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/cli/commands/ios/objection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/cli/commands/ios/scp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/cli/commands/ios/sib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2898 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/cli/commands/ios/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17530 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/cli/device.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:14:27.776403 linktools-0.8.5rc1/src/linktools/container/
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/container/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16132 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/container/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21050 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/container/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4996 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/container/repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5266 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/device.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:14:27.776403 linktools-0.8.5rc1/src/linktools/frida/
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/frida/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6291 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/frida/android.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29987 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/frida/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/frida/ios.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5146 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/frida/script.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3265 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/frida/server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:14:27.776403 linktools-0.8.5rc1/src/linktools/ida/
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/ida/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6229 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/ida/ida.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:14:27.776403 linktools-0.8.5rc1/src/linktools/ios/
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/ios/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/ios/ipa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8545 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/ios/sib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/ios/struct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-05-05 10:14:27.000000 linktools-0.8.5rc1/src/linktools/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4369 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/reactor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:14:27.776403 linktools-0.8.5rc1/src/linktools/references/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/references/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:14:27.780403 linktools-0.8.5rc1/src/linktools/references/fake_useragent/
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/references/fake_useragent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/references/fake_useragent/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7962 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/references/fake_useragent/fake.py
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/references/fake_useragent/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/references/fake_useragent/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/references/fake_useragent/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12209 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/rich.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13556 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/ssh.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:14:27.780403 linktools-0.8.5rc1/src/linktools/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/utils/_port.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8885 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/utils/_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6791 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/utils/_subprocess.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    19476 2024-05-05 10:12:06.000000 linktools-0.8.5rc1/src/linktools/utils/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:14:27.780403 linktools-0.8.5rc1/src/linktools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    35010 2024-05-05 10:14:27.000000 linktools-0.8.5rc1/src/linktools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3783 2024-05-05 10:14:27.000000 linktools-0.8.5rc1/src/linktools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 10:14:27.000000 linktools-0.8.5rc1/src/linktools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-05-05 10:14:27.000000 linktools-0.8.5rc1/src/linktools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-05 10:14:27.000000 linktools-0.8.5rc1/src/linktools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-05 10:14:27.000000 linktools-0.8.5rc1/src/linktools.egg-info/top_level.txt
```

### Comparing `linktools-0.8.5rc0/LICENSE` & `linktools-0.8.5rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `linktools-0.8.5rc0/PKG-INFO` & `linktools-0.8.5rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linktools
-Version: 0.8.5rc0
+Version: 0.8.5rc1
 Summary: linktools toolkit
 Author-email: Hu Ji <669898595@qq.com>
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/ice-black-tea/linktools
 Project-URL: Repository, https://github.com/ice-black-tea/linktools.git
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -78,16 +78,16 @@
 eval "$(ct-env --silent completion --shell bash)" # 给命令添加自动补全功能
 
 alias adb="at-adb"
 alias pidcat="at-pidcat"
 alias sib="it-sib"
 
 alias apktool="ct-tools apktool"
-alias burpsuite="ct-tools --set version=2023.10 burpsuite"
-alias jadx="JAVA_OPTS=-Xmx8g ct-tools --set version=1.4.7 jadx-gui" # 指定jadx版本号，配置jvm最大内存
+alias burpsuite="ct-tools burpsuite"
+alias jadx="ct-tools --set version=1.5.0 jadx-gui" # 指定jadx版本号，配置jvm最大内存
 ```
 
 ## 相关功能
 
 ```
 $ python3 -m linktools
     ___       __   __              __
```

### Comparing `linktools-0.8.5rc0/README.md` & `linktools-0.8.5rc1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -27,16 +27,16 @@
 eval "$(ct-env --silent completion --shell bash)" # 给命令添加自动补全功能
 
 alias adb="at-adb"
 alias pidcat="at-pidcat"
 alias sib="it-sib"
 
 alias apktool="ct-tools apktool"
-alias burpsuite="ct-tools --set version=2023.10 burpsuite"
-alias jadx="JAVA_OPTS=-Xmx8g ct-tools --set version=1.4.7 jadx-gui" # 指定jadx版本号，配置jvm最大内存
+alias burpsuite="ct-tools burpsuite"
+alias jadx="ct-tools --set version=1.5.0 jadx-gui" # 指定jadx版本号，配置jvm最大内存
 ```
 
 ## 相关功能
 
 ```
 $ python3 -m linktools
     ___       __   __              __
```

### Comparing `linktools-0.8.5rc0/pyproject.toml` & `linktools-0.8.5rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `linktools-0.8.5rc0/setup.py` & `linktools-0.8.5rc1/setup.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.5rc0/src/linktools/__init__.py` & `linktools-0.8.5rc1/src/linktools/__init__.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.5rc0/src/linktools/__main__.py` & `linktools-0.8.5rc1/src/linktools/__main__.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.5rc0/src/linktools/_config.py` & `linktools-0.8.5rc1/src/linktools/_config.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.5rc0/src/linktools/_environ.py` & `linktools-0.8.5rc1/src/linktools/_environ.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 import json
 import logging
 import os
 import pathlib
 import shutil
 import sys
 import time
-from typing import TYPE_CHECKING, TypeVar, Type, Any
+from typing import TYPE_CHECKING, TypeVar, Type, Any, Dict
 
 from . import utils, metadata
 from .decorator import cached_property, cached_classproperty
 
 if TYPE_CHECKING:
     from ._config import ConfigDict, Config
     from ._tools import Tools, Tool
@@ -307,38 +307,41 @@
         """
         更新配置
         :param key: 配置键
         :param value: 配置值
         """
         self.config.set(key, value)
 
-    def _create_tools(self) -> "Tools":
+    def _create_tools(self) -> "Dict[str, Tool]":
         from ._tools import Tools
 
-        tools = Tools(self)
+        result = dict()
 
         # set environment variable
         index = 0
         dir_names = os.environ["PATH"].split(os.pathsep)
-        for tool in tools:
-            if not tool.executable:
+        for tool in Tools(self):
+            if not tool.supported:
+                if self.debug:
+                    self.logger.debug(f"Tool not supported: {tool.name}")
                 continue
-            # dirname(executable[0]) -> environ["PATH"]
-            dir_name = tool.dirname
-            if dir_name and dir_name not in dir_names:
-                # insert to head
-                dir_names.insert(index, tool.dirname)
-                index += 1
-        # add all paths to environment variables
+            if tool.executable:
+                # dirname(executable[0]) -> environ["PATH"]
+                dir_name = tool.dirname
+                if dir_name and dir_name not in dir_names:
+                    # insert to head
+                    dir_names.insert(index, tool.dirname)
+                    index += 1
+            result[tool.name] = tool
         os.environ["PATH"] = os.pathsep.join(dir_names)
 
-        return tools
+        return result
 
     @cached_property
-    def tools(self) -> "Tools":
+    def tools(self) -> "Dict[str, Tool]":
         """
         工具集
         """
         return self._create_tools()
 
     def get_tool(self, name: str, **kwargs) -> "Tool":
         """
```

### Comparing `linktools-0.8.5rc0/src/linktools/_tools.py` & `linktools-0.8.5rc1/src/linktools/_tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
  /_==__==========__==_ooo__ooo=_/'   /___________,"
 """
 
 import os
 import pickle
 import shutil
 import warnings
-from typing import TYPE_CHECKING, Dict, Union, Mapping, Iterator, Any, Tuple, List, Type
+from typing import TYPE_CHECKING, Dict, Union, Mapping, Iterator, Any, Tuple, List, Type, Optional
 
 from . import utils
 from .decorator import cached_property
 from .metadata import __missing__
 
 if TYPE_CHECKING:
     from ._environ import BaseEnviron
@@ -62,15 +62,14 @@
             #       - when: {system: [darwin, linux]}
             #         then: xxx
             #       - when: {system: windows}
             #         then: yyy
             #       - else: ~
             # -----------------------------------------
             case_block = value.get("case")
-
             for cond_block in case_block:
 
                 when_block = utils.get_item(cond_block, "when")
                 if when_block is not None:
                     # if it is a "when" block, verify it
                     # -----------------------------------------
                     #   field:
@@ -199,42 +198,39 @@
     target_path: bool = ToolProperty(default=__missing__)
     root_path: str = ToolProperty(default=__missing__)
     unpack_path: str = ToolProperty(default=__missing__)
     absolute_path: str = ToolProperty(default=__missing__)
     cmdline: str = ToolProperty(default=__missing__)
     executable: bool = ToolProperty(default=True)
     executable_cmdline: tuple = ToolProperty(default=[])
-
-    exists: bool = property(lambda self: self.absolute_path and os.path.exists(self.absolute_path))
-    dirname: bool = property(lambda self: None if not self.absolute_path else os.path.dirname(self.absolute_path))
+    environment: Dict[str, str] = ToolProperty(default={})
 
     def __init__(self, tools: "Tools", config: Union[dict, str], **kwargs):
         self._tools = tools
         self._config = config
 
         self._raw_config = pickle.loads(pickle.dumps(self.__default__))
         self._raw_config.update(tools.config)
         self._raw_config.update(config)
         self._raw_config.update(kwargs)
 
     @cached_property
     def config(self) -> dict:
         config = self.__parser__.parse(self._raw_config)
 
-        depends_on = utils.get_item(config, "depends_on")
-        if depends_on:
-            assert isinstance(depends_on, (str, Tuple, List)), \
-                f"Tool<{config['name']}>.depends_on type error, " \
-                f"str/tuple/list was expects, got {type(depends_on)}"
-            if isinstance(depends_on, str):
-                depends_on = [depends_on]
-            for dependency in depends_on:
-                assert dependency in self._tools.items, \
-                    f"Tool<{config['name']}>.depends_on error: not found Tool<{dependency}>"
-            config["depends_on"] = depends_on
+        depends_on = utils.get_item(config, "depends_on") or []
+        assert isinstance(depends_on, (str, Tuple, List)), \
+            f"Tool<{config['name']}>.depends_on type error, " \
+            f"str/tuple/list was expects, got {type(depends_on)}"
+        if isinstance(depends_on, str):
+            depends_on = [depends_on]
+        for dependency in depends_on:
+            assert dependency in self._tools.items, \
+                f"Tool<{config['name']}>.depends_on error: not found Tool<{dependency}>"
+        config["depends_on"] = depends_on
 
         # download url
         download_url = utils.get_item(config, "download_url") or ""
         if download_url == __missing__:
             download_url = ""
         assert isinstance(download_url, str), \
             f"Tool<{config['name']}>.download_url type error, " \
@@ -308,35 +304,48 @@
                 config["executable"] = False
             else:
                 # if executable_cmdline is empty,
                 # set absolute_path as executable_cmdline
                 executable_cmdline = config["absolute_path"]
             if isinstance(executable_cmdline, str):
                 executable_cmdline = [executable_cmdline]
-            config["executable_cmdline"] = [str(i).format(tools=self._tools, **config) \
-                                            for i in executable_cmdline]
+            config["executable_cmdline"] = [
+                str(cmd).format(tools=self._tools, **config)
+                for cmd in executable_cmdline
+            ]
 
         return config
 
-    def copy(self, **kwargs):
+    @property
+    def supported(self) -> bool:
+        return True if self.exists or self.absolute_path else False
+
+    @property
+    def exists(self) -> bool:
+        return True if self.absolute_path and os.path.exists(self.absolute_path) else False
+
+    @property
+    def dirname(self) -> Optional[str]:
+        return None if not self.absolute_path else os.path.dirname(self.absolute_path)
+
+    def copy(self, **kwargs) -> "Tool":
         return Tool(self._tools, self._config, **kwargs)
 
     def prepare(self) -> None:
         for dependency in self.depends_on:
             tool = self._tools[dependency]
             tool.prepare()
 
         # download and unzip file
-        if self.exists:
-            pass
-        elif not self.download_url or not self.absolute_path:
+        if not self.supported:
             raise ToolError(
                 f"{self} does not support on "
                 f"{self._tools.environ.system} ({self._tools.environ.machine})")
-        else:
+
+        if not self.exists:
             self._tools.logger.info(f"Download {self}: {self.download_url}")
             url_file = self._tools.environ.get_url_file(self.download_url)
             temp_dir = self._tools.environ.get_temp_path("tools", "cache")
             temp_path = url_file.save(to_dir=temp_dir)
             if not utils.is_empty(self.unpack_path):
                 self._tools.logger.debug(f"Unpack {self} to {self.root_path}")
                 shutil.unpack_archive(temp_path, self.root_path)
@@ -360,14 +369,20 @@
         elif self.absolute_path.startswith(self.root_path):
             self._tools.logger.debug(f"Delete {self.absolute_path}")
             os.remove(self.absolute_path)
 
     def popen(self, *args: [Any], **kwargs) -> utils.Process:
         self.prepare()
 
+        if self.environment:
+            env = kwargs.get("default_env", {})
+            for key, value in self.environment.items():
+                env.setdefault(key, value)
+            kwargs["default_env"] = env
+
         # java or other
         executable_cmdline = self.executable_cmdline
         if executable_cmdline[0] in self._tools.items:
             args = [*executable_cmdline[1:], *args]
             tool = self._tools.items[executable_cmdline[0]]
             return tool.popen(*args, **kwargs)
 
@@ -424,31 +439,30 @@
 
 
 class Tools(object):
 
     def __init__(self, environ: "BaseEnviron"):
         self.environ = environ
         self.logger = environ.get_logger("tools")
-
-        self.config = dict()
-        self.config.setdefault("system", environ.system)
-        self.config.setdefault("machine", environ.machine)
+        self.config = dict(
+            system=environ.system,
+            machine=environ.machine,
+        )
 
     @cached_property
     def items(self) -> Mapping[str, Tool]:
         items = {}
         for key in self.environ.config.keys():
             if not key.startswith("TOOL_"):
                 continue
             value = self.environ.config.get(key)
             if not isinstance(value, dict):
                 warnings.warn(f"dict was expected, got {type(value)}, ignored.")
                 continue
-            key = key[len("TOOL_"):]
-            key = key.lower()
+            key = key[len("TOOL_"):].lower()
             name = value.setdefault("name", key)
             items[name] = Tool(self, value)
         return items
 
     def __iter__(self) -> Iterator[Tool]:
         return iter(self.items.values())
```

### Comparing `linktools-0.8.5rc0/src/linktools/_url.py` & `linktools-0.8.5rc1/src/linktools/_url.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.5rc0/src/linktools/android/__init__.py` & `linktools-0.8.5rc1/src/linktools/android/__init__.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.5rc0/src/linktools/android/adb.py` & `linktools-0.8.5rc1/src/linktools/android/adb.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
   / ==ooooooooooooooo==.o.  ooo= //   ,`\--{)B     ,"
  /_==__==========__==_ooo__ooo=_/'   /___________,"
 """
 
 import json
 import re
 import time
-from typing import Optional, Any, Generator, List
+from typing import Any, Generator, List
 
 from .struct import App, UnixSocket, InetSocket, Process
 from .. import utils, environ
 from ..decorator import cached_property, cached_classproperty
 from ..device import BridgeError, Bridge, BaseDevice
 from ..reactor import Stoppable
 
@@ -126,45 +126,45 @@
     def uid(self) -> int:
         """
         获取shell的uid
         :return: uid
         """
         return self.get_uid()
 
-    def popen(self, *args: [Any], **kwargs) -> utils.Process:
+    def popen(self, *args: Any, **kwargs) -> utils.Process:
         """
         执行命令
         :param args: 命令行参数
         :return: 打开的进程
         """
         args = ["-s", self.id, *args]
         return self._adb.popen(*args, **kwargs)
 
     @utils.timeoutable
-    def exec(self, *args: [Any], **kwargs) -> str:
+    def exec(self, *args: Any, **kwargs) -> str:
         """
         执行命令
         :param args: 命令行参数
         :return: adb输出结果
         """
         args = ["-s", self.id, *args]
         return self._adb.exec(*args, **kwargs)
 
-    def make_shell_args(self, *args: [Any], privilege: bool = False, user: str = None):
+    def make_shell_args(self, *args: Any, privilege: bool = False, user: str = None):
         cmd = utils.list2cmdline([str(arg) for arg in args])
         if privilege and self.uid != 0:
             args = ["shell", "su", "-c", cmd]
         elif user:
             args = ["shell", "su", user, "-c", cmd]
         else:
             args = ["shell", cmd]
         return args
 
     @utils.timeoutable
-    def shell(self, *args: [Any], privilege: bool = False, user: str = None, **kwargs) -> str:
+    def shell(self, *args: Any, privilege: bool = False, user: str = None, **kwargs) -> str:
         """
         执行shell
         :param args: shell命令
         :param privilege: 是否以root权限运行
         :param user: 以指定user运行
         :return: adb输出结果
         """
@@ -193,28 +193,26 @@
             environ.logger.info(f"Download file: {path_or_url}")
             file = environ.get_url_file(path_or_url)
             apk_path = file.save()
             environ.logger.info(f"Save file to local: {apk_path}")
 
         remote_path = self.get_data_path("apk", f"{int(time.time())}.apk")
         try:
-            environ.logger.debug(f"Push file to remote: {remote_path}")
             self.push(apk_path, remote_path, **kwargs)
             if self.uid >= 10000:
                 self.shell("am", "start", "--user", "0",
                            "-a", "android.intent.action.VIEW",
                            "-t", "application/vnd.android.package-archive",
                            "-d", "file://%s" % remote_path,
                            **kwargs)
             else:
                 self.shell("pm", "install", *(opts or tuple()), remote_path,
                            **kwargs)
         finally:
-            environ.logger.debug(f"Clear remote file: {remote_path}")
-            self.shell("rm", remote_path, **kwargs)
+            self.shell("rm", remote_path, **kwargs, ignore_errors=True)
 
     @utils.timeoutable
     def uninstall(self, package_name: str, **kwargs):
         """
         卸载apk
         :param package_name: 包名
         :return: adb输出结果
@@ -542,49 +540,51 @@
             match = re.search(r"^.*package:\s*(.*)[\s\S]*$", out)
             if match is not None:
                 return match.group(1).strip()
         obj = self.get_apps(package_name, **kwargs)
         return utils.get_item(obj, 0, "sourceDir", default="")
 
     @utils.timeoutable
-    def get_uid(self, package_name: str = None, timeout: utils.Timeout = None) -> Optional[int]:
+    def get_uid(self, package_name: str = None, timeout: utils.Timeout = None) -> int:
         """
         根据包名获取uid
-        :param package_name: 包名
+        :param package_name: 包名，为空则返回当前uid
         :param timeout: 超时时间
         :return: uid
         """
         if package_name:
             app = self.get_app(package_name, timeout=timeout)
-            return app.user_id if app else None
+            return app.user_id
         else:
             default = -1
             out = self.shell("id", "-u", timeout=timeout)
             uid = utils.int(out, default=default)
             if uid != default:
                 return uid
             out = self.shell("echo", "-n", "${USER_ID}", timeout=timeout)
             uid = utils.int(out, default=default)
             if uid != default:
                 return uid
             raise AdbError("unknown adb uid: %s" % out)
 
     @utils.timeoutable
-    def get_app(self, package_name: str, detail: bool = None, **kwargs) -> Optional[App]:
+    def get_app(self, package_name: str, detail: bool = None, **kwargs) -> App:
         """
         根据包名获取包信息
         :param package_name: 包名
         :param detail: 获取详细信息
         :return: 包信息
         """
         args = ["package", "--packages", package_name]
         if detail is not True:
             args.append("--simple")
         objs = json.loads(self.call_agent(*args, **kwargs))
-        return App(objs[0]) if len(objs) > 0 else None
+        if len(objs) == 0:
+            raise AdbError(f"App '{package_name}' not found")
+        return App(objs[0])
 
     @utils.timeoutable
     def get_apps(self, *package_names: str, system: bool = None, detail: bool = False, **kwargs) -> [App]:
         """
         获取包信息
         :param package_names: 需要匹配的所有包名，为空则匹配所有
         :param system: true只匹配系统应用，false只匹配非系统应用，为空则全匹配
@@ -711,8 +711,8 @@
         :return: 路径
         """
         return "/data/local/tmp/%s" % (
             "/".join([cls.get_safe_path(o) for o in paths])
         )
 
     def __repr__(self):
-        return f"AndroidDevice<{self.id}>"
+        return f"AdbDevice<{self.id}>"
```

### Comparing `linktools-0.8.5rc0/src/linktools/android/struct.py` & `linktools-0.8.5rc1/src/linktools/android/struct.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.5rc0/src/linktools/assets/android-tools.apk` & `linktools-0.8.5rc1/src/linktools/assets/android-tools.apk`

 * *Files identical despite different names*

### Comparing `linktools-0.8.5rc0/src/linktools/assets/android-tools.json` & `linktools-0.8.5rc1/src/linktools/assets/android-tools.json`

 * *Files 15% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.975%*

 * *Differences: {"'ANDROID_TOOL_BRIDGE_APK'": "{'time': '2024-05-05 18:14:22'}"}*

```diff
@@ -1,14 +1,14 @@
 {
     "ANDROID_TOOL_BRIDGE_APK": {
         "main": "android.tools.Main",
         "md5": "c419cb85594b69ee31bae8730718c425",
         "name": "android-tools.apk",
         "size": 82987,
-        "time": "2024-04-24 10:46:03"
+        "time": "2024-05-05 18:14:22"
     },
     "ANDROID_TOOL_FRIDA_SERVER": [
         {
             "min_version": "15.1.8",
             "name": "strong-frida-server-{version}-android-{abi}",
             "url": "https://github.com/hzzheyang/strongR-frida-android/releases/download/{version}/hluda-server-{version}-android-{abi}.xz"
         },
```

### Comparing `linktools-0.8.5rc0/src/linktools/assets/chrome-driver.json` & `linktools-0.8.5rc1/src/linktools/assets/chrome-driver.json`

 * *Files identical despite different names*

### Comparing `linktools-0.8.5rc0/src/linktools/assets/containers/100-nginx/Dockerfile` & `linktools-0.8.5rc1/src/linktools/assets/containers/100-nginx/Dockerfile`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 FROM nginx:{{ NGINX_TAG }}
 
 RUN apk --no-cache add openssl socat
+
 RUN curl https://get.acme.sh | sh -s email=acme@google.com && \
     ln -s ~/.acme.sh/acme.sh /usr/bin/acme.sh && \
     acme.sh --set-default-ca --server letsencrypt
 
-RUN echo "#!/bin/sh" > /docker-entrypoint.d/99-start-crond.sh \
-    && echo "crond" >> /docker-entrypoint.d/99-start-crond.sh \
-    && chmod +x /docker-entrypoint.d/99-start-crond.sh
-
-RUN mkdir -p /etc/certs
+RUN mkdir -p /etc/certs && \
+    echo "#!/bin/sh" >> /docker-entrypoint.d/99-start-crond.sh && \
+    echo "crond" >> /docker-entrypoint.d/99-start-crond.sh && \
+    chmod +x /docker-entrypoint.d/99-start-crond.sh
 
 {% for key in container.keys -%}
     {% with value = config.get(key, default=None) -%}
         {% if value %}
 ENV {{ key }} {{ value }}
         {% endif %}
     {%- endwith %}
 {%- endfor %}
 
 RUN acme.sh --issue --domain {{ ROOT_DOMAIN }} --domain *.{{ ROOT_DOMAIN }} --dns {{ ACME_DNS_API }} --debug 2
-
 RUN acme.sh --install-cert --domain {{ ROOT_DOMAIN }} --domain *.{{ ROOT_DOMAIN }} \
     --cert-file /etc/certs/{{ ROOT_DOMAIN }}_cert.pem \
     --key-file /etc/certs/{{ ROOT_DOMAIN }}_key.pem \
     --fullchain-file /etc/certs/{{ ROOT_DOMAIN }}_fullchain.pem \
     --reloadcmd "killall nginx 2>/dev/null || true"
```

### Comparing `linktools-0.8.5rc0/src/linktools/assets/containers/100-nginx/container.py` & `linktools-0.8.5rc1/src/linktools/assets/containers/100-nginx/container.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.5rc0/src/linktools/assets/containers/100-nginx/dnsapi.txt` & `linktools-0.8.5rc1/src/linktools/assets/containers/100-nginx/dnsapi.txt`

 * *Files identical despite different names*

### Comparing `linktools-0.8.5rc0/src/linktools/assets/containers/110-portainer/container.py` & `linktools-0.8.5rc1/src/linktools/assets/containers/110-portainer/container.py`

 * *Files 14% similar despite different names*

```diff
@@ -49,13 +49,7 @@
         ]
 
     def on_starting(self):
         self.write_nginx_conf(
             self.manager.config.get("PORTAINER_DOMAIN"),
             self.get_path("nginx.conf"),
         )
-
-    def on_started(self):
-        self.manager.change_owner(
-            self.get_path("nginx.conf"),
-            self.manager.user
-        )
```

### Comparing `linktools-0.8.5rc0/src/linktools/assets/containers/120-flare/compose.yml` & `linktools-0.8.5rc1/src/linktools/assets/containers/120-flare/compose.yml`

 * *Files identical despite different names*

### Comparing `linktools-0.8.5rc0/src/linktools/assets/containers/120-flare/container.py` & `linktools-0.8.5rc1/src/linktools/assets/containers/120-flare/container.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.5rc0/src/linktools/assets/containers/120-flare/nginx.conf` & `linktools-0.8.5rc1/src/linktools/assets/containers/120-flare/nginx.conf`

 * *Files identical despite different names*

### Comparing `linktools-0.8.5rc0/src/linktools/assets/fake_useragent.json` & `linktools-0.8.5rc1/src/linktools/assets/fake_useragent.json`

 * *Files identical despite different names*

### Comparing `linktools-0.8.5rc0/src/linktools/assets/frida.js` & `linktools-0.8.5rc1/src/linktools/assets/frida.js`

 * *Files identical despite different names*

### Comparing `linktools-0.8.5rc0/src/linktools/assets/frida.min.js` & `linktools-0.8.5rc1/src/linktools/assets/frida.min.js`

 * *Files identical despite different names*

### Comparing `linktools-0.8.5rc0/src/linktools/assets/objection/plugins/__init__.py` & `linktools-0.8.5rc1/src/linktools/assets/objection/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.5rc0/src/linktools/assets/tools.json` & `linktools-0.8.5rc1/src/linktools/assets/tools.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8758298611111113%*

 * *Differences: {"'TOOL_ADB'": "{'target_path': {'case': {1: {'then': 'platform-tools\\\\{name}.exe'}}}}",*

 * * "'TOOL_COMPACT_DEX_CONVERTER'": "OrderedDict([('version', '20240430'), ('depends_on', "*

 * *                                 "OrderedDict([('case', [OrderedDict([('when', "*

 * *                                 "OrderedDict([('system', 'windows')])), ('then', 'flinux')]), "*

 * *                                 "OrderedDict([('else', None)])])])), ('download_url', "*

 * *                                 "'https://github.com/ice-black-t […]*

```diff
@@ -61,15 +61,15 @@
                         "system": [
                             "darwin",
                             "linux"
                         ]
                     }
                 },
                 {
-                    "then": "platform-tools\\\\{name}.exe",
+                    "then": "platform-tools\\{name}.exe",
                     "when": {
                         "system": "windows"
                     }
                 },
                 {
                     "else": null
                 }
@@ -273,29 +273,94 @@
                     "else": null
                 }
             ]
         },
         "unpack_path": "chromedriver-{version}",
         "version": "80.0.3987.106"
     },
+    "TOOL_COMPACT_DEX_CONVERTER": {
+        "depends_on": {
+            "case": [
+                {
+                    "then": "flinux",
+                    "when": {
+                        "system": "windows"
+                    }
+                },
+                {
+                    "else": null
+                }
+            ]
+        },
+        "download_url": "https://github.com/ice-black-tea/archives/releases/download/compact_dex_converter-{version}/compact_dex_converter.zip",
+        "executable_cmdline": {
+            "case": [
+                {
+                    "then": [
+                        "flinux",
+                        "\\??\\{absolute_path}"
+                    ],
+                    "when": {
+                        "system": "windows"
+                    }
+                },
+                {
+                    "else": null
+                }
+            ]
+        },
+        "target_path": {
+            "case": [
+                {
+                    "then": "compact_dex_converter_mac",
+                    "when": {
+                        "machine": [
+                            "x86_64",
+                            "arm64"
+                        ],
+                        "system": "darwin"
+                    }
+                },
+                {
+                    "then": "compact_dex_converter_linux64",
+                    "when": {
+                        "machine": "x86_64",
+                        "system": "linux"
+                    }
+                },
+                {
+                    "then": "compact_dex_converter_linux",
+                    "when": {
+                        "machine": "amd64",
+                        "system": "windows"
+                    }
+                },
+                {
+                    "else": null
+                }
+            ]
+        },
+        "unpack_path": "compact_dex_converter-{version}",
+        "version": "20240430"
+    },
     "TOOL_DEX2JAR": {
         "download_url": "https://github.com/pxb1988/dex2jar/releases/download/v{version}{version_suffix}/dex-tools-{version}{version_suffix}.zip",
         "target_path": {
             "case": [
                 {
                     "then": "dex-tools-{version}/d2j-{name}.sh",
                     "when": {
                         "system": [
                             "darwin",
                             "linux"
                         ]
                     }
                 },
                 {
-                    "then": "dex-tools-{version}\\\\d2j-{name}.bat",
+                    "then": "dex-tools-{version}\\d2j-{name}.bat",
                     "when": {
                         "system": "windows"
                     }
                 },
                 {
                     "else": null
                 }
@@ -315,26 +380,55 @@
                         "system": [
                             "darwin",
                             "linux"
                         ]
                     }
                 },
                 {
-                    "then": "platform-tools\\\\{name}.exe",
+                    "then": "platform-tools\\{name}.exe",
                     "when": {
                         "system": "windows"
                     }
                 },
                 {
                     "else": null
                 }
             ]
         },
         "unpack_path": "platform-tools"
     },
+    "TOOL_FLINUX": {
+        "download_url": {
+            "case": [
+                {
+                    "then": "https://github.com/ice-black-tea/archives/releases/download/flinux-20240505/flinux.exe",
+                    "when": {
+                        "system": "windows"
+                    }
+                },
+                {
+                    "else": null
+                }
+            ]
+        },
+        "target_path": {
+            "case": [
+                {
+                    "then": "flinux.exe",
+                    "when": {
+                        "system": "windows"
+                    }
+                },
+                {
+                    "else": null
+                }
+            ]
+        },
+        "version": "0.21"
+    },
     "TOOL_IPATOOL": {
         "download_url": {
             "case": [
                 {
                     "then": "https://github.com/majd/ipatool/releases/download/v{version}/ipatool-{version}-macos-arm64.tar.gz",
                     "when": {
                         "machine": "arm64",
@@ -387,15 +481,15 @@
                     "then": "bin/ipatool-{version}-linux-amd64",
                     "when": {
                         "machine": "x86_64",
                         "system": "linux"
                     }
                 },
                 {
-                    "then": "bin\\\\ipatool-{version}-windows-amd64.exe",
+                    "then": "bin\\ipatool-{version}-windows-amd64.exe",
                     "when": {
                         "machine": "amd64",
                         "system": "windows"
                     }
                 },
                 {
                     "else": null
@@ -415,43 +509,46 @@
                         "system": [
                             "darwin",
                             "linux"
                         ]
                     }
                 },
                 {
-                    "then": "bin\\\\{name}.bat",
+                    "then": "bin\\{name}.bat",
                     "when": {
                         "system": "windows"
                     }
                 },
                 {
                     "else": null
                 }
             ]
         },
         "unpack_path": "jadx-{version}",
         "version": "1.5.0"
     },
     "TOOL_JADX_GUI": {
         "download_url": "https://github.com/skylot/jadx/releases/download/v{version}/jadx-{version}.zip",
+        "environment": {
+            "JAVA_OPTS": "-Xmx8g"
+        },
         "name": "jadx-gui",
         "target_path": {
             "case": [
                 {
                     "then": "bin/{name}",
                     "when": {
                         "system": [
                             "darwin",
                             "linux"
                         ]
                     }
                 },
                 {
-                    "then": "bin\\\\{name}.bat",
+                    "then": "bin\\{name}.bat",
                     "when": {
                         "system": "windows"
                     }
                 },
                 {
                     "else": null
                 }
@@ -470,15 +567,15 @@
                         "system": [
                             "darwin",
                             "linux"
                         ]
                     }
                 },
                 {
-                    "then": "dex-tools-{version}\\\\d2j-{name}.bat",
+                    "then": "dex-tools-{version}\\d2j-{name}.bat",
                     "when": {
                         "system": "windows"
                     }
                 },
                 {
                     "else": null
                 }
@@ -535,15 +632,15 @@
                 {
                     "then": "sapmachine-jdk-{version}/bin/{name}",
                     "when": {
                         "system": "linux"
                     }
                 },
                 {
-                    "then": "sapmachine-jdk-{version}\\\\bin\\\\{name}.exe",
+                    "then": "sapmachine-jdk-{version}\\bin\\{name}.exe",
                     "when": {
                         "system": "windows"
                     }
                 },
                 {
                     "else": null
                 }
@@ -599,15 +696,15 @@
                 {
                     "then": "sapmachine-jdk-{version}/bin/{name}",
                     "when": {
                         "system": "linux"
                     }
                 },
                 {
-                    "then": "sapmachine-jdk-{version}\\\\bin\\\\{name}.exe",
+                    "then": "sapmachine-jdk-{version}\\bin\\{name}.exe",
                     "when": {
                         "system": "windows"
                     }
                 },
                 {
                     "else": null
                 }
@@ -692,14 +789,65 @@
         "depends_on": "python",
         "executable_cmdline": [
             "python",
             "-m",
             "{name}"
         ]
     },
+    "TOOL_VDEX_EXTRACTOR": {
+        "depends_on": {
+            "case": [
+                {
+                    "then": "flinux",
+                    "when": {
+                        "system": "windows"
+                    }
+                },
+                {
+                    "else": null
+                }
+            ]
+        },
+        "download_url": {
+            "case": [
+                {
+                    "then": "https://github.com/ice-black-tea/archives/releases/download/vdexExtractor-{version}/vdexExtractor-macos-arm64",
+                    "when": {
+                        "machine": "arm64",
+                        "system": "darwin"
+                    }
+                },
+                {
+                    "then": "https://github.com/ice-black-tea/archives/releases/download/vdexExtractor-{version}/vdexExtractor-macos-amd64",
+                    "when": {
+                        "machine": "x86_64",
+                        "system": "darwin"
+                    }
+                },
+                {
+                    "then": "https://github.com/ice-black-tea/archives/releases/download/vdexExtractor-{version}/vdexExtractor-linux-amd64",
+                    "when": {
+                        "machine": "x86_64",
+                        "system": "linux"
+                    }
+                },
+                {
+                    "then": "https://github.com/ice-black-tea/archives/releases/download/vdexExtractor-{version}/vdexExtractor-windows-amd64.exe",
+                    "when": {
+                        "machine": "amd64",
+                        "system": "windows"
+                    }
+                },
+                {
+                    "else": null
+                }
+            ]
+        },
+        "version": "20240430"
+    },
     "TOOL_XPATCH": {
         "depends_on": "java",
         "download_url": "https://github.com/WindySha/Xpatch/releases/download/v{version}/xpatch-{version}.jar",
         "executable_cmdline": [
             "java",
             "-jar",
             "{absolute_path}"
```

### Comparing `linktools-0.8.5rc0/src/linktools/cli/__init__.py` & `linktools-0.8.5rc1/src/linktools/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.5rc0/src/linktools/cli/argparse.py` & `linktools-0.8.5rc1/src/linktools/cli/argparse.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.5rc0/src/linktools/cli/command.py` & `linktools-0.8.5rc1/src/linktools/cli/command.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,14 +27,15 @@
  /_==__==========__==_ooo__ooo=_/'   /___________,"
 """
 
 import abc
 import inspect
 import logging
 import os
+import sys
 import textwrap
 import traceback
 from argparse import ArgumentParser, Action, Namespace
 from argparse import RawDescriptionHelpFormatter, SUPPRESS, FileType, HelpFormatter
 from pkgutil import walk_packages
 from types import ModuleType, GeneratorType
 from typing import TYPE_CHECKING, Optional, Callable, List, Type, Tuple, Generator, Any, Iterable, Union, Set, Dict
@@ -836,15 +837,15 @@
             result = e.code
         except:
             get_console().print_exception(show_locals=True) \
                 if environ.debug \
                 else self.logger.error(traceback.format_exc())
             result = 1
 
-        exit(result)
+        sys.exit(result)
 
     def __call__(self, args: Union[List[str], Namespace] = None) -> int:
         """
         内部调用命令入口
         """
         try:
             if not isinstance(args, Namespace):
```

### Comparing `linktools-0.8.5rc0/src/linktools/cli/commands/android/adb.py` & `linktools-0.8.5rc1/src/linktools/cli/commands/android/adb.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.5rc0/src/linktools/cli/commands/android/agent.py` & `linktools-0.8.5rc1/src/linktools/cli/commands/android/agent.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.5rc0/src/linktools/cli/commands/android/app.py` & `linktools-0.8.5rc1/src/linktools/cli/commands/android/app.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.5rc0/src/linktools/cli/commands/android/debug.py` & `linktools-0.8.5rc1/src/linktools/cli/commands/android/debug.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.5rc0/src/linktools/cli/commands/android/frida.py` & `linktools-0.8.5rc1/src/linktools/cli/commands/android/frida.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.5rc0/src/linktools/cli/commands/android/info.py` & `linktools-0.8.5rc1/src/linktools/cli/commands/android/info.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.5rc0/src/linktools/cli/commands/android/intent.py` & `linktools-0.8.5rc1/src/linktools/cli/commands/android/intent.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,15 +26,14 @@
   / ==ooooooooooooooo==.o.  ooo= //   ,`\--{)B     ,"
  /_==__==========__==_ooo__ooo=_/'   /___________,"
 """
 import os
 from argparse import ArgumentParser, Namespace
 from typing import Optional
 
-from linktools import utils
 from linktools.cli import subcommand, subcommand_argument, AndroidCommand
 
 
 class Command(AndroidCommand):
     """
     Common intent actions
     """
@@ -68,38 +67,38 @@
         device.shell("am", "start", "--user", "0",
                      "-a", "android.intent.action.View",
                      "com.android.settings/com.android.settings.DevelopmentSettings",
                      log_output=True)
 
     @subcommand("setting-app", help="start application setting activity (default: current running package)",
                 pass_args=True)
-    @subcommand_argument("package")
+    @subcommand_argument("package", nargs="?", help="package name")
     def on_setting_app(self, args: Namespace, package: str = None):
         device = args.device_picker.pick()
         package = package or device.get_current_package()
         device.shell("am", "start", "--user", "0",
                      "-a", "android.settings.APPLICATION_DETAILS_SETTINGS",
                      "-d", "package:%s" % package,
                      log_output=True)
 
     @subcommand("setting-cert", help="install cert (require \'/data/local/tmp\' write permission)", pass_args=True)
-    @subcommand_argument("path")
+    @subcommand_argument("path", help="cert file path")
     def on_setting_cert(self, args: Namespace, path: str):
         device = args.device_picker.pick()
         remote_path = device.get_data_path("cert", os.path.basename(path))
         device.push(path, remote_path, log_output=True)
         device.shell("am", "start", "--user", "0",
                      "-n", "com.android.certinstaller/.CertInstallerMain",
                      "-a", "android.intent.action.VIEW",
                      "-t", "application/x-x509-ca-cert",
                      "-d", "file://%s" % remote_path,
                      log_output=True)
 
     @subcommand("install", help="install apk file (require \'/data/local/tmp\' write permission)", pass_args=True)
-    @subcommand_argument("path")
+    @subcommand_argument("path", help="apk file path or url")
     def on_install(self, args: Namespace, path: str):
         device = args.device_picker.pick()
         device.install(path,
                        opts=["-r", "-t", "-d", "-f"],
                        log_output=True)
 
     @subcommand("browser", help="start browser activity and jump to url", pass_args=True)
```

### Comparing `linktools-0.8.5rc0/src/linktools/cli/commands/android/objection.py` & `linktools-0.8.5rc1/src/linktools/cli/commands/android/objection.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,16 +94,15 @@
             if args.plugin_folder:
                 objection_args += ["--plugin-folder", args.plugin_folder]
 
             if args.redirect_address or args.redirect_port:
                 # 如果需要重定向到本地端口
                 address = args.redirect_address
                 port = args.redirect_port or 8080
-                app = device.get_app(package)
-                uid = app.user_id if app else None
+                uid = device.get_uid(package)
                 with device.redirect(address, port, uid):
                     return utils.Process(*objection_args).call()
             else:
                 return utils.Process(*objection_args).call()
 
 
 command = Command()
```

### Comparing `linktools-0.8.5rc0/src/linktools/cli/commands/android/pidcat.py` & `linktools-0.8.5rc1/src/linktools/cli/commands/android/pidcat.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.5rc0/src/linktools/cli/commands/android/top.py` & `linktools-0.8.5rc1/src/linktools/cli/commands/android/top.py`

 * *Files 3% similar despite different names*

```diff
@@ -56,46 +56,45 @@
         group.add_argument('--screen', metavar='DEST', action='store', type=str, nargs='?', default=".",
                            help='capture screen and pull file')
 
     def run(self, args: Namespace) -> Optional[int]:
         device = args.device_picker.pick()
 
         if args.package:
-            environ.logger.info(device.get_current_package())
+            print(device.get_current_package())
         elif args.activity:
-            environ.logger.info(device.get_current_activity())
+            print(device.get_current_activity())
         elif args.path:
-            environ.logger.info(device.get_apk_path(device.get_current_package()))
+            print(device.get_apk_path(device.get_current_package()))
         elif args.kill:
             device.shell("am", "force-stop", device.get_current_package(), log_output=True)
         elif "--apk" in sys.argv:
-            package_name = device.get_current_package()
-            environ.logger.info("find current package: {}".format(package_name))
-            app = device.get_app(package_name)
-            if app is not None:
-                environ.logger.info("find current apk path: {}".format(app.source_dir))
-                path = device.get_storage_path("{}_{}.apk".format(app.name, app.version_name))
-                dest = args.apk if not utils.is_empty(args.apk) else "."
-                device.shell("mkdir", "-p", device.get_storage_path(), log_output=True)
-                device.shell("cp", app.source_dir, path, log_output=True)
-                device.pull(path, dest, log_output=True)
-                device.shell("rm", path)
+            name = device.get_current_package()
+            environ.logger.info(f"Find current package: {name}")
+            app = device.get_app(name)
+            environ.logger.info(f"Find current apk path: {app.source_dir}")
+            path = device.get_storage_path("{}_{}.apk".format(app.name, app.version_name))
+            dest = args.apk if not utils.is_empty(args.apk) else "."
+            device.shell("mkdir", "-p", device.get_storage_path(), log_output=True)
+            device.shell("cp", app.source_dir, path, log_output=True)
+            device.pull(path, dest, log_output=True)
+            device.shell("rm", path)
         elif "--screen" in sys.argv:
             now = datetime.datetime.now()
             path = device.get_storage_path("screenshot-" + now.strftime("%Y-%m-%d-%H-%M-%S") + ".png")
             dest = args.screen if not utils.is_empty(args.screen) else "."
             device.shell("mkdir", "-p", device.get_storage_path(), log_output=True)
             device.shell("screencap", "-p", path, log_output=True)
             device.pull(path, dest, log_output=True)
             device.shell("rm", path)
         else:
             app = device.get_current_package()
-            environ.logger.info("package:  ", app)
-            environ.logger.info("activity: ", device.get_current_activity())
-            environ.logger.info("path:     ", device.get_apk_path(app))
+            environ.logger.info(f"Package:  {app}")
+            environ.logger.info(f"Activity: {device.get_current_activity()}")
+            environ.logger.info(f"Path:     {device.get_apk_path(app)}")
 
         return
 
 
 command = Command()
 if __name__ == "__main__":
     command.main()
```

### Comparing `linktools-0.8.5rc0/src/linktools/cli/commands/common/cert.py` & `linktools-0.8.5rc1/src/linktools/cli/commands/common/cert.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.5rc0/src/linktools/cli/commands/common/cntr.py` & `linktools-0.8.5rc1/src/linktools/cli/commands/common/cntr.py`

 * *Files 2% similar despite different names*

```diff
@@ -272,14 +272,15 @@
     @subcommand("up", help="deploy installed containers")
     @subcommand_argument("--build", action=BooleanOptionalAction, help="build images before starting")
     @subcommand_argument("--pull", help="pull image before running", choices=["always", "missing", "never"])
     @subcommand_argument("name", metavar="CONTAINER", nargs="?", help="container name",
                          choices=utils.lazy_iter(_iter_installed_container_names))
     def on_command_up(self, name: str = None, build: str = True, pull: str = None):
         containers = manager.prepare_installed_containers()
+        target_containers = [c for c in containers if not name or c.name == name]
 
         options = ["--detach"]
         if build:
             options.extend(["--build"])
         if pull:
             options.extend(["--pull", pull])
 
@@ -287,31 +288,31 @@
         if name:
             services.extend(manager.containers[name].services.keys())
             if not services:
                 raise ContainerError(f"No service found in container `{name}`")
         else:
             options.extend(["--remove-orphans"])
 
-        for container in containers:
+        for container in target_containers:
             container.on_starting()
         manager.create_docker_compose_process(
             containers,
             "up", *options, *services
         ).check_call()
-        for container in reversed(containers):
+        for container in reversed(target_containers):
             container.on_started()
 
     @subcommand("restart", help="restart installed containers")
     @subcommand_argument("--build", action=BooleanOptionalAction, help="build images before starting")
     @subcommand_argument("--pull", help="pull image before running", choices=["always", "missing", "never"])
     @subcommand_argument("name", metavar="CONTAINER", nargs="?", help="container name",
                          choices=utils.lazy_iter(_iter_installed_container_names))
     def on_command_restart(self, name: str = None, build: str = True, pull: str = None):
         containers = manager.prepare_installed_containers()
-        stop_containers = [c for c in containers if not name or c.name == name]
+        target_containers = [c for c in containers if not name or c.name == name]
 
         options = ["--detach"]
         if build:
             options.extend(["--build"])
         if pull:
             options.extend(["--pull", pull])
 
@@ -319,54 +320,54 @@
         if name:
             services.extend(manager.containers[name].services.keys())
             if not services:
                 raise ContainerError(f"No service found in container `{name}`")
         else:
             options.extend(["--remove-orphans"])
 
-        for container in reversed(stop_containers):
+        for container in reversed(target_containers):
             container.on_stopping()
         manager.create_docker_compose_process(
             containers,
             "stop", *services
         ).check_call()
-        for container in stop_containers:
+        for container in target_containers:
             container.on_stopped()
 
-        for container in containers:
+        for container in target_containers:
             container.on_starting()
         manager.create_docker_compose_process(
             containers,
             "up", *options, *services
         ).check_call()
-        for container in reversed(containers):
+        for container in reversed(target_containers):
             container.on_started()
 
     @subcommand("down", help="stop installed containers")
     @subcommand_argument("name", metavar="CONTAINER", nargs="?", help="container name",
                          choices=utils.lazy_iter(_iter_installed_container_names))
     def on_command_down(self, name: str = None):
         containers = manager.prepare_installed_containers()
-        stop_containers = [c for c in containers if not name or c.name == name]
+        target_containers = [c for c in containers if not name or c.name == name]
 
         services = []
         if name:
             services.extend(manager.containers[name].services.keys())
             if not services:
                 raise ContainerError(f"No service found in container `{name}`")
 
-        for container in reversed(stop_containers):
+        for container in reversed(target_containers):
             container.on_stopping()
         manager.create_docker_compose_process(
             containers,
             "down", *services
         ).check_call()
-        for container in stop_containers:
+        for container in target_containers:
             container.on_stopped()
 
-        for container in stop_containers:
+        for container in target_containers:
             container.on_removed()
 
 
 command = Command()
 if __name__ == '__main__':
     command.main()
```

### Comparing `linktools-0.8.5rc0/src/linktools/cli/commands/common/env.py` & `linktools-0.8.5rc1/src/linktools/cli/commands/common/env.py`

 * *Files 5% similar despite different names*

```diff
@@ -102,15 +102,15 @@
                          choices=["bash", "zsh", "tcsh", "fish", "powershell"])
     @subcommand_argument("--sync", action="store_true", help="sync complete script")
     def on_completion(self, shell: str = DEFAULT_SHELL, sync: bool = False):
         if not auto_complete:
             self.logger.warning("argcomplete module not found")
             return
 
-        path = self.environ.get_data_path("scripts", "complete", create_parent=True)
+        path = self.environ.get_data_path("scripts", f"completion_{self.environ.version}", create_parent=True)
         if not sync and os.path.exists(path):
             self.logger.info(f"Found complete script: {path}")
             print(utils.read_file(path, text=True), flush=True)
             return 0
 
         executables = []
         modules = {c.name: c for c in iter_command_modules(commands, onerror="warn")}
@@ -130,15 +130,15 @@
         print(result, flush=True)
 
     @subcommand("alias", help="generate shell alias script")
     @subcommand_argument("-s", "--shell", help="output code for the specified shell",
                          choices=["bash", "zsh", "tcsh", "fish", "powershell"])
     @subcommand_argument("--sync", action="store_true", help="sync alias script")
     def on_alias(self, shell: str = DEFAULT_SHELL, sync: bool = False):
-        path = self.environ.get_data_path("scripts", "alias", create_parent=True)
+        path = self.environ.get_data_path("scripts", f"alias_{self.environ.version}", create_parent=True)
         if not sync and os.path.exists(path):
             self.logger.info(f"Found alias script: {path}")
             print(utils.read_file(path, text=True), flush=True)
             return 0
 
         lines = []
         if shell not in ("powershell",):
```

### Comparing `linktools-0.8.5rc0/src/linktools/cli/commands/common/grep.py` & `linktools-0.8.5rc1/src/linktools/cli/commands/common/grep.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.5rc0/src/linktools/cli/commands/common/tools.py` & `linktools-0.8.5rc1/src/linktools/cli/commands/common/tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 from linktools import ToolError, DownloadError
 from linktools.cli import BaseCommand
 from linktools.cli.argparse import KeyValueAction
 
 
 class Command(BaseCommand):
     """
-    Download and use tools
+    Use the tool from remote url
     """
 
     def main(self, *args, **kwargs) -> None:
         self.environ.config.set_default("SHOW_LOG_LEVEL", False)
         self.environ.config.set_default("SHOW_LOG_TIME", False)
         return super().main(*args, **kwargs)
 
@@ -60,15 +60,15 @@
         group.add_argument("--download", action="store_true", default=False,
                            help="download tool files")
         group.add_argument("--clear", action="store_true", default=False,
                            help="clear tool files")
         group.add_argument("-d", "--daemon", action="store_true", default=False,
                            help="execute tools as a daemon")
 
-        tool_names = sorted([tool.name for tool in iter(self.environ.tools)])
+        tool_names = sorted([tool.name for tool in self.environ.tools.values()])
         subparsers = parser.add_subparsers(metavar="TOOL", help=f"{{{','.join(tool_names)}}}")
         subparsers.required = True
         for tool_name in tool_names:
             tool_parser = subparsers.add_parser(tool_name, prefix_chars=chr(0), add_help=False)
             tool_parser.add_argument("tool_args", metavar="args", nargs="...")
             tool_parser.set_defaults(tool_name=tool_name)
```

### Comparing `linktools-0.8.5rc0/src/linktools/cli/commands/ios/frida.py` & `linktools-0.8.5rc1/src/linktools/cli/commands/ios/frida.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.5rc0/src/linktools/cli/commands/ios/ipa.py` & `linktools-0.8.5rc1/src/linktools/cli/commands/ios/ipa.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.5rc0/src/linktools/cli/commands/ios/objection.py` & `linktools-0.8.5rc1/src/linktools/cli/commands/ios/objection.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.5rc0/src/linktools/cli/commands/ios/scp.py` & `linktools-0.8.5rc1/src/linktools/cli/commands/ios/scp.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.5rc0/src/linktools/cli/commands/ios/sib.py` & `linktools-0.8.5rc1/src/linktools/cli/commands/ios/sib.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.5rc0/src/linktools/cli/commands/ios/ssh.py` & `linktools-0.8.5rc1/src/linktools/cli/commands/ios/ssh.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.5rc0/src/linktools/cli/device.py` & `linktools-0.8.5rc1/src/linktools/cli/device.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.5rc0/src/linktools/container/__init__.py` & `linktools-0.8.5rc1/src/linktools/container/__init__.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.5rc0/src/linktools/container/container.py` & `linktools-0.8.5rc1/src/linktools/container/container.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.5rc0/src/linktools/container/manager.py` & `linktools-0.8.5rc1/src/linktools/container/manager.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.5rc0/src/linktools/container/repository.py` & `linktools-0.8.5rc1/src/linktools/container/repository.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.5rc0/src/linktools/decorator.py` & `linktools-0.8.5rc1/src/linktools/decorator.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.5rc0/src/linktools/device.py` & `linktools-0.8.5rc1/src/linktools/device.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.5rc0/src/linktools/frida/__init__.py` & `linktools-0.8.5rc1/src/linktools/frida/__init__.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.5rc0/src/linktools/frida/android.py` & `linktools-0.8.5rc1/src/linktools/frida/android.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.5rc0/src/linktools/frida/app.py` & `linktools-0.8.5rc1/src/linktools/frida/app.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.5rc0/src/linktools/frida/ios.py` & `linktools-0.8.5rc1/src/linktools/frida/ios.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.5rc0/src/linktools/frida/script.py` & `linktools-0.8.5rc1/src/linktools/frida/script.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.5rc0/src/linktools/frida/server.py` & `linktools-0.8.5rc1/src/linktools/frida/server.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.5rc0/src/linktools/ida/__init__.py` & `linktools-0.8.5rc1/src/linktools/ida/__init__.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.5rc0/src/linktools/ida/ida.py` & `linktools-0.8.5rc1/src/linktools/ida/ida.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.5rc0/src/linktools/ios/ipa.py` & `linktools-0.8.5rc1/src/linktools/ios/ipa.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,79 +3,72 @@
 
 # Author    : HuJi <jihu.hj@alibaba-inc.com>
 # Datetime  : 2022/1/13 下午8:53
 # User      : huji
 # Product   : PyCharm
 # Project   : link
 
-import os
 import plistlib
 import re
 import zipfile
-from typing import Optional
+from typing import Optional, Dict, Any, List
+
+_INFO_PLIST = "Info.plist"
 
 
 class IPAError(Exception):
     pass
 
 
 class IPA(object):
-    _INFO_PLIST = "Info.plist"
 
     def __init__(self, filename: str):
         self.filename = filename
         self.zip = zipfile.ZipFile(self.filename)
         self._plist = {}
         self._analysis()
 
     def _analysis(self):
-        plist_path = self.find_file(self._INFO_PLIST)
+        plist_path = self.find_file(_INFO_PLIST)
         if plist_path is None:
-            raise IPAError("missing Info.plist")
+            raise IPAError("Missing Info.plist")
         plist_data = self.zip.read(plist_path)
-        self._plist[self._INFO_PLIST] = plistlib.loads(plist_data)
+        self._plist[_INFO_PLIST] = plistlib.loads(plist_data)
 
     def find_file(self, name) -> Optional[str]:
         name_list = self.zip.namelist()
         pattern = re.compile(rf'Payload/[^/]+\.app/{name}$')
         for path in name_list:
             m = pattern.match(path)
             if m is not None:
                 return m.group()
         return None
 
-    def get_files(self):
+    def list_files(self) -> List[str]:
         return self.zip.namelist()
 
-    def get_file(self, filename):
+    def read_file(self, filename) -> bytes:
         try:
             return self.zip.read(filename)
         except KeyError:
-            raise IPAError(f"file not found: {filename}")
+            raise IPAError(f"Not found {filename}")
 
-    def get_info_plist(self):
-        return self._plist[self._INFO_PLIST]
+    def get_info_plist(self) -> Dict[str, Any]:
+        return self._plist[_INFO_PLIST]
 
-    def get_launch_storyboard_name(self):
+    def get_launch_storyboard_name(self) -> str:
         return self.get_info_plist().get("UILaunchStoryboardName")
 
-    def get_display_name(self):
+    def get_display_name(self) -> str:
         return self.get_info_plist().get("CFBundleDisplayName")
 
-    def get_bundle_id(self):
+    def get_bundle_id(self) -> str:
         return self.get_info_plist().get("CFBundleIdentifier")
 
-    def get_version(self):
+    def get_version(self) -> str:
         return self.get_info_plist().get("CFBundleVersion")
 
-    def get_version_string(self):
+    def get_version_string(self) -> str:
         return self.get_info_plist().get("CFBundleShortVersionString")
 
-    def get_permssions(self):
-        plist = self.get_info_plist()
-        for key in plist:
-            if key.endswith("Description"):
-                print(key, plist[key])
-
-
-if __name__ == '__main__':
-    IPA(os.path.expanduser("~/Downloads/201200@蜂鸟跑腿.ipa")).get_permssions()
+    def get_permissions(self) -> Dict[str, str]:
+        return {k: v for k, v in self.get_info_plist().items() if k.endswith("Description")}
```

### Comparing `linktools-0.8.5rc0/src/linktools/ios/sib.py` & `linktools-0.8.5rc1/src/linktools/ios/sib.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 # -*- coding:utf-8 -*-
 
 import json
 import subprocess
 import time
 from subprocess import TimeoutExpired
-from typing import Any, Generator, List, Optional
+from typing import Any, Generator, List
 
 from .struct import Process, App
 from .. import utils
 from .._environ import environ
 from ..decorator import cached_property
 from ..device import BridgeError, Bridge, BaseDevice
 from ..reactor import Stoppable
@@ -119,27 +119,33 @@
         :param args: 命令行参数
         :return: sib输出结果
         """
         args = ["--udid", self.id, *args]
         return self._sib.exec(*args, **kwargs)
 
     @utils.timeoutable
-    def install(self, path: str, **kwargs) -> str:
-        return self.exec("app", "install", "--path", path, **kwargs)
+    def install(self, path_or_url: str, **kwargs) -> str:
+        ipa_path = path_or_url
+        if path_or_url.startswith("http://") or path_or_url.startswith("https://"):
+            environ.logger.info(f"Download file: {path_or_url}")
+            file = environ.get_url_file(path_or_url)
+            ipa_path = file.save()
+            environ.logger.info(f"Save file to local: {ipa_path}")
+        return self.exec("app", "install", "--path", ipa_path, **kwargs)
 
     @utils.timeoutable
     def uninstall(self, bundle_id: str, **kwargs) -> str:
         return self.exec("app", "uninstall", "--bundleId", bundle_id, **kwargs)
 
     @utils.timeoutable
     def kill(self, bundle_id: str, **kwargs) -> str:
         return self.exec("app", "kill", "--bundleId", bundle_id, **kwargs)
 
     @utils.timeoutable
-    def get_app(self, bundle_id: str, detail: bool = None, **kwargs) -> Optional[App]:
+    def get_app(self, bundle_id: str, detail: bool = None, **kwargs) -> App:
         """
         根据包名获取包信息
         :param bundle_id: 包名
         :param detail: 获取详细信息
         :return: 包信息
         """
         options = ["--format", "--system"]
@@ -148,15 +154,15 @@
 
         out = json.loads(self.exec("app", "list", *options, **kwargs))
         for obj in utils.get_list_item(out, "appList"):
             app = App(obj)
             if bundle_id == app.bundle_id:
                 return app
 
-        return None
+        raise SibError(f"App '{bundle_id}' not found")
 
     @utils.timeoutable
     def get_apps(self, *bundle_ids: str, system: bool = None, detail: bool = False, **kwargs) -> [App]:
         """
         获取包信息
         :param bundle_ids: 需要匹配的所有包名，为空则匹配所有
         :param system: true只匹配系统应用，false只匹配非系统应用，为空则全匹配
@@ -260,8 +266,8 @@
             def stop(self):
                 reverse.stop()
                 forward.stop()
 
         return Reverse()
 
     def __repr__(self):
-        return f"iOSDevice<{self.id}>"
+        return f"SibDevice<{self.id}>"
```

### Comparing `linktools-0.8.5rc0/src/linktools/ios/struct.py` & `linktools-0.8.5rc1/src/linktools/ios/struct.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.5rc0/src/linktools/metadata.py` & `linktools-0.8.5rc1/src/linktools/metadata.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,20 +27,21 @@
  /_==__==========__==_ooo__ooo=_/'   /___________,"
 """
 
 
 class __MissingType:
     __eq__ = lambda l, r: \
         l is r or type(l) is type(r)
+    __repr__ = lambda _: "__missing__"
 
 
 __name__ = "linktools"
 __release__ = True
-__version__ = "0.8.5rc0"
+__version__ = "0.8.5rc1"
 __missing__ = __MissingType()
 __description__ = f"""\
     ___       __   __              __
    / (_)___  / /__/ /_____  ____  / /____
-  / / / __ \\/ //_/ __/ __ \\/ __ \\/ / ___/  linktools toolkit (v0.8.5rc0)
+  / / / __ \\/ //_/ __/ __ \\/ __ \\/ / ___/  linktools toolkit (v0.8.5rc1)
  / / / / / / ,< / /_/ /_/ / /_/ / (__  )   by: Hu Ji <669898595@qq.com>
 /_/_/_/ /_/_/|_|\\__/\\____/\\____/_/____/
 """
```

### Comparing `linktools-0.8.5rc0/src/linktools/reactor.py` & `linktools-0.8.5rc1/src/linktools/reactor.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import threading
 import time
 import traceback
 from collections import deque
 from typing import Optional, Callable, Any, Coroutine
 
 from ._environ import environ
+from .utils import InterruptableEvent
 
 _logger = environ.get_logger("reactor")
 
 
 class Stoppable(abc.ABC):
 
     @abc.abstractmethod
@@ -129,15 +130,15 @@
         def run():
             self._loop = asyncio.new_event_loop()
             event.set()
             self._loop.run_forever()
 
         super().__init__(target=run)
 
-        event = threading.Event()
+        event = InterruptableEvent()
         self.daemon = True
         self._loop: Optional[asyncio.AbstractEventLoop] = None
         self.start()
         event.wait()
         atexit.register(self.stop)
 
     def stop(self):
```

### Comparing `linktools-0.8.5rc0/src/linktools/references/fake_useragent/fake.py` & `linktools-0.8.5rc1/src/linktools/references/fake_useragent/fake.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.5rc0/src/linktools/references/fake_useragent/utils.py` & `linktools-0.8.5rc1/src/linktools/references/fake_useragent/utils.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.5rc0/src/linktools/rich.py` & `linktools-0.8.5rc1/src/linktools/rich.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.5rc0/src/linktools/ssh.py` & `linktools-0.8.5rc1/src/linktools/ssh.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.5rc0/src/linktools/utils/__init__.py` & `linktools-0.8.5rc1/src/linktools/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.5rc0/src/linktools/utils/_port.py` & `linktools-0.8.5rc1/src/linktools/utils/_port.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.5rc0/src/linktools/utils/_proxy.py` & `linktools-0.8.5rc1/src/linktools/utils/_proxy.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.5rc0/src/linktools/utils/_subprocess.py` & `linktools-0.8.5rc1/src/linktools/utils/_subprocess.py`

 * *Files 6% similar despite different names*

```diff
@@ -53,84 +53,92 @@
     def is_alive(self):
         if self._stdout_finished and not self._stdout_finished.is_set():
             return True
         if self._stderr_finished and not self._stderr_finished.is_set():
             return True
         return False
 
-    def _iter_lines(self, io: IO[AnyStr], flag: int, event: threading.Event):
+    def _iter_lines(self, io: IO[AnyStr], code: int, event: threading.Event):
         try:
             while True:
                 data = io.readline()
                 if not data:
                     break
-                self._queue.put((flag, data))
+                self._queue.put((code, data))
         except OSError as e:
             if e.errno != errno.EBADF:
                 environ.logger.debug(f"Handle output error: {e}")
         finally:
             event.set()
             self._queue.put((None, None))
 
     def get_lines(self, timeout: Timeout):
         while self.is_alive:
             try:
                 # 给个1秒超时时间防止有多个线程消费的时候死锁
-                flag, data = self._queue.get(timeout=min(timeout.remain or 1, 1))
-                if flag is not None:
-                    yield flag, data
+                code, data = self._queue.get(timeout=min(timeout.remain or 1, 1))
+                if code is not None:
+                    yield code, data
             except queue.Empty:
                 if not timeout.check():
                     break
 
         while True:
             try:
                 # 需要把剩余可消费的数据消费完
-                flag, data = self._queue.get_nowait()
-                if flag is not None:
-                    yield flag, data
+                code, data = self._queue.get_nowait()
+                if code is not None:
+                    yield code, data
             except queue.Empty:
                 break
 
 
 class Process(subprocess.Popen):
 
     def __init__(
             self,
             *args: Any,
             capture_output: bool = False,
             stdin: Union[int, IO] = None, stdout: Union[int, IO] = None, stderr: Union[int, IO] = None,
             shell: bool = False, cwd: str = None,
-            env: Dict[str, str] = None, append_env: Dict[str, str] = None,
+            env: Dict[str, str] = None, append_env: Dict[str, str] = None, default_env: Dict[str, str] = None,
             **kwargs,
     ):
+        args = [str(arg) for arg in args]
+
         if capture_output is True:
             if stdout is not None or stderr is not None:
                 raise ValueError("stdout and stderr arguments may not be used "
                                  "with capture_output.")
             stdout = subprocess.PIPE
             stderr = subprocess.PIPE
-        if cwd:
+
+        if not cwd:
             try:
                 cwd = os.getcwd()
             except FileNotFoundError:
                 cwd = environ.get_temp_dir(create=True)
-        if append_env:
+
+        if append_env or default_env:
             env = dict(env) if env else dict(os.environ)
-            env.update(append_env)
+            if default_env:
+                for key, value in default_env.items():
+                    env.setdefault(key, value)
+            if append_env:
+                env.update(append_env)
 
         super().__init__(
-            [str(arg) for arg in args],
+            args,
             stdin=stdin, stdout=stdout, stderr=stderr,
             shell=shell, cwd=cwd,
             env=env,
             **kwargs
         )
 
-        environ.logger.debug(f"Exec cmdline: {list2cmdline(self.args)}")
+        environ.logger.debug(f"Exec cmdline: {list2cmdline(args)}")
 
     @timeoutable
     def call(self, timeout: Timeout = None) -> int:
         with self:
             try:
                 return self.wait(timeout=timeout.remain)
             except Exception:
@@ -171,24 +179,24 @@
         :return: 返回stdout输出内容
         """
 
         out = err = None
 
         if self.stdout or self.stderr:
 
-            for flag, data in self._output.get_lines(timeout):
-                if flag == self._output.STDOUT:
+            for code, data in self._output.get_lines(timeout):
+                if code == self._output.STDOUT:
                     out = data if out is None else out + data
                     if on_stdout:
                         data = data.decode(errors="ignore") if isinstance(data, bytes) else data
                         data = data.rstrip()
                         if data:
                             on_stdout(data)
 
-                elif flag == self._output.STDERR:
+                elif code == self._output.STDERR:
                     err = data if err is None else err + data
                     if on_stderr:
                         data = data.decode(errors="ignore") if isinstance(data, bytes) else data
                         data = data.rstrip()
                         if data:
                             on_stderr(data)
         else:
```

### Comparing `linktools-0.8.5rc0/src/linktools/utils/_utils.py` & `linktools-0.8.5rc1/src/linktools/utils/_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,14 +56,16 @@
 if TYPE_CHECKING:
     from typing import ParamSpec
 
     T = TypeVar("T")
     P = ParamSpec("P")
 
 DEFAULT_ENCODING = "utf-8"
+SYSTEM = platform.system().lower()
+MACHINE = platform.machine().lower()
 
 
 class Timeout:
 
     def __init__(self, timeout: Union[float, int] = None):
         self._deadline = None
         self._timeout = timeout
@@ -94,15 +96,15 @@
         if not self.check():
             raise err_type(message)
 
     def __repr__(self):
         return f"Timeout(timeout={self._timeout})"
 
 
-def timeoutable(fn: "Callable[P, T]") -> "Callable[P, T]":
+def _timeoutable(fn: "Callable[P, T]") -> "Callable[P, T]":
     timeout_keyword = "timeout"
 
     timeout_index = -1
     positional_index = -1
     keyword_index = -1
 
     index = 0
@@ -146,14 +148,17 @@
             kwargs[timeout_keyword] = Timeout()
 
         return fn(*args, **kwargs)
 
     return wrapper
 
 
+timeoutable: Any = _timeoutable
+
+
 class InterruptableEvent(threading.Event):
     """
     解决 Windows 上 event.wait 不支持 ctrl+c 中断的问题
     """
 
     @timeoutable
     def wait(self, timeout: Timeout = None):
@@ -167,15 +172,15 @@
                 break
             if wait(min(t, interval)):
                 break
 
 
 def ignore_error(
         fn: "Callable[P, T]", *,
-        args: Tuple[Any, ...] = None, kwargs: Dict[str, Any] = None,
+        args: "P.args" = None, kwargs: "P.kwargs" = None,
         default: "T" = None) -> "T":
     try:
         if args is None:
             args = tuple()
         if kwargs is None:
             kwargs = dict()
         return fn(*args, **kwargs)
@@ -643,30 +648,26 @@
     cookies = {}
     for item in cookie.split(";"):
         key_value = item.split("=", 1)
         cookies[key_value[0].strip()] = key_value[1].strip() if len(key_value) > 1 else ''
     return cookies
 
 
-_SYSTEM = platform.system().lower()
-_MACHINE = platform.machine().lower()
-
-
 def get_system():
     """
     获取系统类型
     """
-    return _SYSTEM
+    return SYSTEM
 
 
 def get_machine():
     """
     获取机器类型
     """
-    return _MACHINE
+    return MACHINE
 
 
 def get_user():
     """
     获取当前用户
     """
     return getpass.getuser()
@@ -701,26 +702,26 @@
 
 
 def get_shell_path():
     """
     获取当前用户shell路径
     """
 
-    if _SYSTEM in ["darwin", "linux"]:
+    if SYSTEM in ["darwin", "linux"]:
         if "SHELL" in os.environ:
             shell_path = os.environ["SHELL"]
             if shell_path and os.path.exists(shell_path):
                 return shell_path
         try:
             import pwd
             return pwd.getpwnam(get_user()).pw_shell
         except:
             return shutil.which("zsh") or shutil.which("bash") or shutil.which("sh")
 
-    elif _SYSTEM in ["windows"]:
+    elif SYSTEM in ["windows"]:
         if "ComSpec" in os.environ:
             shell_path = os.environ["ComSpec"]
             if shell_path and os.path.exists(shell_path):
                 return shell_path
         return shutil.which("powershell") or shutil.which("cmd")
 
     return ""
```

### Comparing `linktools-0.8.5rc0/src/linktools.egg-info/PKG-INFO` & `linktools-0.8.5rc1/src/linktools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linktools
-Version: 0.8.5rc0
+Version: 0.8.5rc1
 Summary: linktools toolkit
 Author-email: Hu Ji <669898595@qq.com>
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/ice-black-tea/linktools
 Project-URL: Repository, https://github.com/ice-black-tea/linktools.git
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -78,16 +78,16 @@
 eval "$(ct-env --silent completion --shell bash)" # 给命令添加自动补全功能
 
 alias adb="at-adb"
 alias pidcat="at-pidcat"
 alias sib="it-sib"
 
 alias apktool="ct-tools apktool"
-alias burpsuite="ct-tools --set version=2023.10 burpsuite"
-alias jadx="JAVA_OPTS=-Xmx8g ct-tools --set version=1.4.7 jadx-gui" # 指定jadx版本号，配置jvm最大内存
+alias burpsuite="ct-tools burpsuite"
+alias jadx="ct-tools --set version=1.5.0 jadx-gui" # 指定jadx版本号，配置jvm最大内存
 ```
 
 ## 相关功能
 
 ```
 $ python3 -m linktools
     ___       __   __              __
```

### Comparing `linktools-0.8.5rc0/src/linktools.egg-info/SOURCES.txt` & `linktools-0.8.5rc1/src/linktools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `linktools-0.8.5rc0/src/linktools.egg-info/entry_points.txt` & `linktools-0.8.5rc1/src/linktools.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `linktools-0.8.5rc0/src/linktools.egg-info/requires.txt` & `linktools-0.8.5rc1/src/linktools.egg-info/requires.txt`

 * *Files identical despite different names*

