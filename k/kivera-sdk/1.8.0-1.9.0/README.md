# Comparing `tmp/kivera-sdk-1.8.0.tar.gz` & `tmp/kivera-sdk-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kivera-sdk-1.8.0.tar", last modified: Fri Apr  5 00:17:29 2024, max compression
+gzip compressed data, was "kivera-sdk-1.9.0.tar", last modified: Wed May  8 04:19:39 2024, max compression
```

## Comparing `kivera-sdk-1.8.0.tar` & `kivera-sdk-1.9.0.tar`

### file list

```diff
@@ -1,181 +1,156 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:17:29.218516 kivera-sdk-1.8.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-05 00:17:29.218516 kivera-sdk-1.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:17:29.198516 kivera-sdk-1.8.0/kivera/
--rw-r--r--   0 runner    (1001) docker     (127)     7669 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:17:29.198516 kivera-sdk-1.8.0/kivera/cloudtenants/
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/cloudtenants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/cloudtenants/create.py
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/cloudtenants/delete.py
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/cloudtenants/get.py
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/cloudtenants/list.py
--rw-r--r--   0 runner    (1001) docker     (127)      952 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/cloudtenants/update.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:17:29.202516 kivera-sdk-1.8.0/kivera/compliancemappings/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/compliancemappings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/compliancemappings/list.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:17:29.202516 kivera-sdk-1.8.0/kivera/config/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/config/get.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:17:29.202516 kivera-sdk-1.8.0/kivera/counters/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/counters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/counters/get.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:17:29.202516 kivera-sdk-1.8.0/kivera/globalpolicyfunctions/
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/globalpolicyfunctions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/globalpolicyfunctions/get.py
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/globalpolicyfunctions/list.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:17:29.202516 kivera-sdk-1.8.0/kivera/globalservices/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/globalservices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/globalservices/list.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:17:29.202516 kivera-sdk-1.8.0/kivera/identities/
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/identities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3156 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/identities/create.py
--rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/identities/delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     6589 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/identities/get.py
--rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/identities/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/identities/update.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:17:29.202516 kivera-sdk-1.8.0/kivera/identityprofiles/
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/identityprofiles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      879 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/identityprofiles/create.py
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/identityprofiles/delete.py
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/identityprofiles/get.py
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/identityprofiles/list.py
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/identityprofiles/update.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:17:29.202516 kivera-sdk-1.8.0/kivera/identitytypes/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/identitytypes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/identitytypes/get.py
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/identitytypes/list.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:17:29.206516 kivera-sdk-1.8.0/kivera/managedrules/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/managedrules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/managedrules/list.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:17:29.206516 kivera-sdk-1.8.0/kivera/memberships/
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/memberships/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/memberships/create.py
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/memberships/delete.py
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/memberships/get.py
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/memberships/list.py
--rw-r--r--   0 runner    (1001) docker     (127)      962 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/memberships/update.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:17:29.206516 kivera-sdk-1.8.0/kivera/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/metrics/getcounterproxymetrics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:17:29.206516 kivera-sdk-1.8.0/kivera/notificationdestinations/
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/notificationdestinations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/notificationdestinations/get.py
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/notificationdestinations/list.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:17:29.206516 kivera-sdk-1.8.0/kivera/notificationmonitors/
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/notificationmonitors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/notificationmonitors/get.py
--rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/notificationmonitors/list.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:17:29.206516 kivera-sdk-1.8.0/kivera/organizationpolicyfunctions/
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/organizationpolicyfunctions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/organizationpolicyfunctions/create.py
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/organizationpolicyfunctions/delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/organizationpolicyfunctions/get.py
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/organizationpolicyfunctions/list.py
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/organizationpolicyfunctions/update.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:17:29.206516 kivera-sdk-1.8.0/kivera/organizations/
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/organizations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/organizations/get.py
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/organizations/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/organizations/update.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:17:29.206516 kivera-sdk-1.8.0/kivera/plans/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/plans/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/plans/list.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:17:29.210516 kivera-sdk-1.8.0/kivera/profiles/
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/profiles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/profiles/attach.py
--rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/profiles/create.py
--rw-r--r--   0 runner    (1001) docker     (127)     3133 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/profiles/delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/profiles/get.py
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/profiles/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/profiles/update.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:17:29.210516 kivera-sdk-1.8.0/kivera/providers/
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/providers/get.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/providers/list.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:17:29.210516 kivera-sdk-1.8.0/kivera/providerversions/
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/providerversions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/providerversions/list.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:17:29.210516 kivera-sdk-1.8.0/kivera/proxies/
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/proxies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3809 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/proxies/create.py
--rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/proxies/delete.py
--rw-r--r--   0 runner    (1001) docker     (127)    11918 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/proxies/get.py
--rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/proxies/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     9599 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/proxies/update.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:17:29.210516 kivera-sdk-1.8.0/kivera/proxyapikeys/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/proxyapikeys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/proxyapikeys/get.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:17:29.210516 kivera-sdk-1.8.0/kivera/proxydeployments/
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/proxydeployments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      981 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/proxydeployments/create.py
--rw-r--r--   0 runner    (1001) docker     (127)    11107 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/proxydeployments/get.py
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/proxydeployments/list.py
--rw-r--r--   0 runner    (1001) docker     (127)      949 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/proxydeployments/update.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:17:29.210516 kivera-sdk-1.8.0/kivera/proxyproviders/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/proxyproviders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/proxyproviders/list.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:17:29.214516 kivera-sdk-1.8.0/kivera/roles/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/roles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/roles/list.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:17:29.214516 kivera-sdk-1.8.0/kivera/ruledependencies/
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/ruledependencies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      909 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/ruledependencies/attach.py
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/ruledependencies/get.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:17:29.214516 kivera-sdk-1.8.0/kivera/ruledependencyresources/
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/ruledependencyresources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/ruledependencyresources/get.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:17:29.214516 kivera-sdk-1.8.0/kivera/ruleparameters/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/ruleparameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/ruleparameters/get.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:17:29.214516 kivera-sdk-1.8.0/kivera/rules/
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/rules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4847 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/rules/create.py
--rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/rules/delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     4509 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/rules/get.py
--rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/rules/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/rules/update.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:17:29.214516 kivera-sdk-1.8.0/kivera/services/
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/services/create.py
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/services/delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/services/get.py
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/services/list.py
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/services/update.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:17:29.214516 kivera-sdk-1.8.0/kivera/trailblazerapikeys/
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/trailblazerapikeys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/trailblazerapikeys/get.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:17:29.218516 kivera-sdk-1.8.0/kivera/trailblazeridentities/
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/trailblazeridentities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      941 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/trailblazeridentities/create.py
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/trailblazeridentities/delete.py
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/trailblazeridentities/get.py
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/trailblazeridentities/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/trailblazeridentities/update.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:17:29.218516 kivera-sdk-1.8.0/kivera/trailblazers/
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/trailblazers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/trailblazers/create.py
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/trailblazers/delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/trailblazers/get.py
--rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/trailblazers/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     2340 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/trailblazers/update.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:17:29.218516 kivera-sdk-1.8.0/kivera/userapikeys/
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/userapikeys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/userapikeys/get.py
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/userapikeys/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/userapikeys/update.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:17:29.218516 kivera-sdk-1.8.0/kivera/users/
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/users/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/users/delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/users/get.py
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/users/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/users/update.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:17:29.218516 kivera-sdk-1.8.0/kivera_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-05 00:17:29.000000 kivera-sdk-1.8.0/kivera_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4232 2024-04-05 00:17:29.000000 kivera-sdk-1.8.0/kivera_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 00:17:29.000000 kivera-sdk-1.8.0/kivera_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-05 00:17:29.000000 kivera-sdk-1.8.0/kivera_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-05 00:17:29.000000 kivera-sdk-1.8.0/kivera_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-05 00:17:29.218516 kivera-sdk-1.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 04:19:39.656800 kivera-sdk-1.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-08 04:19:19.000000 kivera-sdk-1.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-05-08 04:19:39.656800 kivera-sdk-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-08 04:19:19.000000 kivera-sdk-1.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 04:19:39.640800 kivera-sdk-1.9.0/kivera/
+-rw-r--r--   0 runner    (1001) docker     (127)     7194 2024-05-08 04:19:19.000000 kivera-sdk-1.9.0/kivera/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 04:19:39.640800 kivera-sdk-1.9.0/kivera/cloudtenants/
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-08 04:19:19.000000 kivera-sdk-1.9.0/kivera/cloudtenants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-05-08 04:19:19.000000 kivera-sdk-1.9.0/kivera/cloudtenants/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-08 04:19:19.000000 kivera-sdk-1.9.0/kivera/cloudtenants/delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-05-08 04:19:19.000000 kivera-sdk-1.9.0/kivera/cloudtenants/get.py
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-05-08 04:19:19.000000 kivera-sdk-1.9.0/kivera/cloudtenants/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-05-08 04:19:19.000000 kivera-sdk-1.9.0/kivera/cloudtenants/update.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 04:19:39.640800 kivera-sdk-1.9.0/kivera/compliancemappings/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-08 04:19:19.000000 kivera-sdk-1.9.0/kivera/compliancemappings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-05-08 04:19:19.000000 kivera-sdk-1.9.0/kivera/compliancemappings/list.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 04:19:39.640800 kivera-sdk-1.9.0/kivera/config/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-08 04:19:19.000000 kivera-sdk-1.9.0/kivera/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-05-08 04:19:19.000000 kivera-sdk-1.9.0/kivera/config/get.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 04:19:39.640800 kivera-sdk-1.9.0/kivera/counters/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-08 04:19:19.000000 kivera-sdk-1.9.0/kivera/counters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-08 04:19:19.000000 kivera-sdk-1.9.0/kivera/counters/get.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 04:19:39.640800 kivera-sdk-1.9.0/kivera/globalpolicyfunctions/
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-08 04:19:19.000000 kivera-sdk-1.9.0/kivera/globalpolicyfunctions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-08 04:19:19.000000 kivera-sdk-1.9.0/kivera/globalpolicyfunctions/get.py
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-08 04:19:19.000000 kivera-sdk-1.9.0/kivera/globalpolicyfunctions/list.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 04:19:39.640800 kivera-sdk-1.9.0/kivera/globalservices/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-08 04:19:19.000000 kivera-sdk-1.9.0/kivera/globalservices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-05-08 04:19:19.000000 kivera-sdk-1.9.0/kivera/globalservices/list.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 04:19:39.640800 kivera-sdk-1.9.0/kivera/identities/
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-08 04:19:19.000000 kivera-sdk-1.9.0/kivera/identities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3156 2024-05-08 04:19:19.000000 kivera-sdk-1.9.0/kivera/identities/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-05-08 04:19:19.000000 kivera-sdk-1.9.0/kivera/identities/delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6615 2024-05-08 04:19:19.000000 kivera-sdk-1.9.0/kivera/identities/get.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-05-08 04:19:19.000000 kivera-sdk-1.9.0/kivera/identities/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-05-08 04:19:19.000000 kivera-sdk-1.9.0/kivera/identities/update.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 04:19:39.644800 kivera-sdk-1.9.0/kivera/identityprofiles/
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-08 04:19:19.000000 kivera-sdk-1.9.0/kivera/identityprofiles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2024-05-08 04:19:19.000000 kivera-sdk-1.9.0/kivera/identityprofiles/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-05-08 04:19:19.000000 kivera-sdk-1.9.0/kivera/identityprofiles/delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-08 04:19:19.000000 kivera-sdk-1.9.0/kivera/identityprofiles/get.py
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-08 04:19:19.000000 kivera-sdk-1.9.0/kivera/identityprofiles/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-05-08 04:19:19.000000 kivera-sdk-1.9.0/kivera/identityprofiles/update.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 04:19:39.644800 kivera-sdk-1.9.0/kivera/identitytypes/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-08 04:19:19.000000 kivera-sdk-1.9.0/kivera/identitytypes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-05-08 04:19:19.000000 kivera-sdk-1.9.0/kivera/identitytypes/get.py
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-08 04:19:19.000000 kivera-sdk-1.9.0/kivera/identitytypes/list.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 04:19:39.644800 kivera-sdk-1.9.0/kivera/managedrules/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-08 04:19:19.000000 kivera-sdk-1.9.0/kivera/managedrules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-05-08 04:19:19.000000 kivera-sdk-1.9.0/kivera/managedrules/list.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 04:19:39.644800 kivera-sdk-1.9.0/kivera/memberships/
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-08 04:19:19.000000 kivera-sdk-1.9.0/kivera/memberships/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-05-08 04:19:19.000000 kivera-sdk-1.9.0/kivera/memberships/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-08 04:19:19.000000 kivera-sdk-1.9.0/kivera/memberships/delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-05-08 04:19:19.000000 kivera-sdk-1.9.0/kivera/memberships/get.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-05-08 04:19:19.000000 kivera-sdk-1.9.0/kivera/memberships/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-05-08 04:19:19.000000 kivera-sdk-1.9.0/kivera/memberships/update.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 04:19:39.644800 kivera-sdk-1.9.0/kivera/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-08 04:19:19.000000 kivera-sdk-1.9.0/kivera/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-05-08 04:19:19.000000 kivera-sdk-1.9.0/kivera/metrics/getcounterproxymetrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 04:19:39.644800 kivera-sdk-1.9.0/kivera/organizationpolicyfunctions/
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-08 04:19:19.000000 kivera-sdk-1.9.0/kivera/organizationpolicyfunctions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-05-08 04:19:19.000000 kivera-sdk-1.9.0/kivera/organizationpolicyfunctions/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-08 04:19:19.000000 kivera-sdk-1.9.0/kivera/organizationpolicyfunctions/delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-05-08 04:19:19.000000 kivera-sdk-1.9.0/kivera/organizationpolicyfunctions/get.py
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-08 04:19:19.000000 kivera-sdk-1.9.0/kivera/organizationpolicyfunctions/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-08 04:19:19.000000 kivera-sdk-1.9.0/kivera/organizationpolicyfunctions/update.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 04:19:39.644800 kivera-sdk-1.9.0/kivera/organizations/
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-08 04:19:19.000000 kivera-sdk-1.9.0/kivera/organizations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-08 04:19:19.000000 kivera-sdk-1.9.0/kivera/organizations/get.py
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-08 04:19:19.000000 kivera-sdk-1.9.0/kivera/organizations/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-05-08 04:19:19.000000 kivera-sdk-1.9.0/kivera/organizations/update.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 04:19:39.644800 kivera-sdk-1.9.0/kivera/plans/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-08 04:19:19.000000 kivera-sdk-1.9.0/kivera/plans/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-05-08 04:19:19.000000 kivera-sdk-1.9.0/kivera/plans/list.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 04:19:39.648800 kivera-sdk-1.9.0/kivera/profiles/
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-08 04:19:19.000000 kivera-sdk-1.9.0/kivera/profiles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-05-08 04:19:19.000000 kivera-sdk-1.9.0/kivera/profiles/attach.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-05-08 04:19:19.000000 kivera-sdk-1.9.0/kivera/profiles/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3133 2024-05-08 04:19:19.000000 kivera-sdk-1.9.0/kivera/profiles/delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-05-08 04:19:19.000000 kivera-sdk-1.9.0/kivera/profiles/get.py
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-08 04:19:19.000000 kivera-sdk-1.9.0/kivera/profiles/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-05-08 04:19:19.000000 kivera-sdk-1.9.0/kivera/profiles/update.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 04:19:39.648800 kivera-sdk-1.9.0/kivera/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-08 04:19:19.000000 kivera-sdk-1.9.0/kivera/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-08 04:19:19.000000 kivera-sdk-1.9.0/kivera/providers/get.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-08 04:19:19.000000 kivera-sdk-1.9.0/kivera/providers/list.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 04:19:39.648800 kivera-sdk-1.9.0/kivera/providerversions/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-08 04:19:19.000000 kivera-sdk-1.9.0/kivera/providerversions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-08 04:19:19.000000 kivera-sdk-1.9.0/kivera/providerversions/list.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 04:19:39.648800 kivera-sdk-1.9.0/kivera/proxies/
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-08 04:19:19.000000 kivera-sdk-1.9.0/kivera/proxies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3809 2024-05-08 04:19:19.000000 kivera-sdk-1.9.0/kivera/proxies/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-05-08 04:19:19.000000 kivera-sdk-1.9.0/kivera/proxies/delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11944 2024-05-08 04:19:19.000000 kivera-sdk-1.9.0/kivera/proxies/get.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-05-08 04:19:19.000000 kivera-sdk-1.9.0/kivera/proxies/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9599 2024-05-08 04:19:19.000000 kivera-sdk-1.9.0/kivera/proxies/update.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 04:19:39.648800 kivera-sdk-1.9.0/kivera/proxyapikeys/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-08 04:19:19.000000 kivera-sdk-1.9.0/kivera/proxyapikeys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-05-08 04:19:19.000000 kivera-sdk-1.9.0/kivera/proxyapikeys/get.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 04:19:39.648800 kivera-sdk-1.9.0/kivera/proxydeployments/
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-08 04:19:19.000000 kivera-sdk-1.9.0/kivera/proxydeployments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-05-08 04:19:19.000000 kivera-sdk-1.9.0/kivera/proxydeployments/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11107 2024-05-08 04:19:19.000000 kivera-sdk-1.9.0/kivera/proxydeployments/get.py
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-08 04:19:19.000000 kivera-sdk-1.9.0/kivera/proxydeployments/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-05-08 04:19:19.000000 kivera-sdk-1.9.0/kivera/proxydeployments/update.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 04:19:39.648800 kivera-sdk-1.9.0/kivera/proxyproviders/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-08 04:19:19.000000 kivera-sdk-1.9.0/kivera/proxyproviders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-05-08 04:19:19.000000 kivera-sdk-1.9.0/kivera/proxyproviders/list.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 04:19:39.648800 kivera-sdk-1.9.0/kivera/roles/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-08 04:19:19.000000 kivera-sdk-1.9.0/kivera/roles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-08 04:19:19.000000 kivera-sdk-1.9.0/kivera/roles/list.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 04:19:39.652800 kivera-sdk-1.9.0/kivera/ruledependencies/
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-08 04:19:19.000000 kivera-sdk-1.9.0/kivera/ruledependencies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-05-08 04:19:19.000000 kivera-sdk-1.9.0/kivera/ruledependencies/attach.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-08 04:19:19.000000 kivera-sdk-1.9.0/kivera/ruledependencies/get.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 04:19:39.652800 kivera-sdk-1.9.0/kivera/ruledependencyresources/
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-08 04:19:19.000000 kivera-sdk-1.9.0/kivera/ruledependencyresources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-05-08 04:19:19.000000 kivera-sdk-1.9.0/kivera/ruledependencyresources/get.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 04:19:39.652800 kivera-sdk-1.9.0/kivera/ruleparameters/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-08 04:19:19.000000 kivera-sdk-1.9.0/kivera/ruleparameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-05-08 04:19:19.000000 kivera-sdk-1.9.0/kivera/ruleparameters/get.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 04:19:39.652800 kivera-sdk-1.9.0/kivera/rules/
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-08 04:19:19.000000 kivera-sdk-1.9.0/kivera/rules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4847 2024-05-08 04:19:19.000000 kivera-sdk-1.9.0/kivera/rules/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-05-08 04:19:19.000000 kivera-sdk-1.9.0/kivera/rules/delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4509 2024-05-08 04:19:19.000000 kivera-sdk-1.9.0/kivera/rules/get.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-05-08 04:19:19.000000 kivera-sdk-1.9.0/kivera/rules/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-05-08 04:19:19.000000 kivera-sdk-1.9.0/kivera/rules/update.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 04:19:39.652800 kivera-sdk-1.9.0/kivera/services/
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-08 04:19:19.000000 kivera-sdk-1.9.0/kivera/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-05-08 04:19:19.000000 kivera-sdk-1.9.0/kivera/services/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-08 04:19:19.000000 kivera-sdk-1.9.0/kivera/services/delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-05-08 04:19:19.000000 kivera-sdk-1.9.0/kivera/services/get.py
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-08 04:19:19.000000 kivera-sdk-1.9.0/kivera/services/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-05-08 04:19:19.000000 kivera-sdk-1.9.0/kivera/services/update.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 04:19:39.652800 kivera-sdk-1.9.0/kivera/userapikeys/
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-08 04:19:19.000000 kivera-sdk-1.9.0/kivera/userapikeys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-08 04:19:19.000000 kivera-sdk-1.9.0/kivera/userapikeys/get.py
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-05-08 04:19:19.000000 kivera-sdk-1.9.0/kivera/userapikeys/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3517 2024-05-08 04:19:19.000000 kivera-sdk-1.9.0/kivera/userapikeys/update.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 04:19:39.652800 kivera-sdk-1.9.0/kivera/users/
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-08 04:19:19.000000 kivera-sdk-1.9.0/kivera/users/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-08 04:19:19.000000 kivera-sdk-1.9.0/kivera/users/delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-05-08 04:19:19.000000 kivera-sdk-1.9.0/kivera/users/get.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-05-08 04:19:19.000000 kivera-sdk-1.9.0/kivera/users/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-05-08 04:19:19.000000 kivera-sdk-1.9.0/kivera/users/update.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 04:19:39.652800 kivera-sdk-1.9.0/kivera_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-05-08 04:19:39.000000 kivera-sdk-1.9.0/kivera_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-05-08 04:19:39.000000 kivera-sdk-1.9.0/kivera_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 04:19:39.000000 kivera-sdk-1.9.0/kivera_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-08 04:19:39.000000 kivera-sdk-1.9.0/kivera_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-08 04:19:39.000000 kivera-sdk-1.9.0/kivera_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-08 04:19:19.000000 kivera-sdk-1.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-08 04:19:39.656800 kivera-sdk-1.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-08 04:19:19.000000 kivera-sdk-1.9.0/setup.py
```

### Comparing `kivera-sdk-1.8.0/LICENSE` & `kivera-sdk-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.8.0/PKG-INFO` & `kivera-sdk-1.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kivera-sdk
-Version: 1.8.0
+Version: 1.9.0
 Summary: Python library to interact with the Kivera Graphql API
 Home-page: https://github.com/kivera-io/python-client
 Author: Kivera
 Author-email: support@kivera.io
 License: MIT License
 Keywords: kivera graphql gql sdk client
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `kivera-sdk-1.8.0/kivera/__init__.py` & `kivera-sdk-1.9.0/kivera/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "v1.8.0"
+__version__ = "v1.9.0"
 import json
 import requests
 from gql import Client as GqlClient
 from gql.transport.aiohttp import AIOHTTPTransport
 from gql.transport.exceptions import TransportQueryError
 from jose import jwt, exceptions
 from datetime import datetime, timedelta
@@ -15,16 +15,14 @@
 from kivera.globalservices import GlobalServicesMethods
 from kivera.identities import IdentitiesMethods
 from kivera.identityprofiles import IdentityProfilesMethods
 from kivera.identitytypes import IdentityTypesMethods
 from kivera.managedrules import ManagedRulesMethods
 from kivera.memberships import MembershipsMethods
 from kivera.metrics import MetricsMethods
-from kivera.notificationdestinations import NotificationDestinationsMethods
-from kivera.notificationmonitors import NotificationMonitorsMethods
 from kivera.organizationpolicyfunctions import OrganizationPolicyFunctionsMethods
 from kivera.organizations import OrganizationsMethods
 from kivera.plans import PlansMethods
 from kivera.profiles import ProfilesMethods
 from kivera.providerversions import ProviderVersionsMethods
 from kivera.providers import ProvidersMethods
 from kivera.proxies import ProxiesMethods
@@ -33,17 +31,14 @@
 from kivera.proxyproviders import ProxyProvidersMethods
 from kivera.roles import RolesMethods
 from kivera.ruledependencies import RuleDependenciesMethods
 from kivera.ruledependencyresources import RuleDependencyResourcesMethods
 from kivera.ruleparameters import RuleParametersMethods
 from kivera.rules import RulesMethods
 from kivera.services import ServicesMethods
-from kivera.trailblazeridentities import TrailBlazerIdentitiesMethods
-from kivera.trailblazers import TrailBlazersMethods
-from kivera.trailblazerapikeys import TrailblazerApiKeysMethods
 from kivera.userapikeys import UserApiKeysMethods
 from kivera.users import UsersMethods
 
 class ClientError(Exception):
     def __init__(self, message):
         self.message = message
     def __str__(self):
@@ -59,16 +54,14 @@
 	GlobalServicesMethods,
 	IdentitiesMethods,
 	IdentityProfilesMethods,
 	IdentityTypesMethods,
 	ManagedRulesMethods,
 	MembershipsMethods,
 	MetricsMethods,
-	NotificationDestinationsMethods,
-	NotificationMonitorsMethods,
 	OrganizationPolicyFunctionsMethods,
 	OrganizationsMethods,
 	PlansMethods,
 	ProfilesMethods,
 	ProviderVersionsMethods,
 	ProvidersMethods,
 	ProxiesMethods,
@@ -77,17 +70,14 @@
 	ProxyProvidersMethods,
 	RolesMethods,
 	RuleDependenciesMethods,
 	RuleDependencyResourcesMethods,
 	RuleParametersMethods,
 	RulesMethods,
 	ServicesMethods,
-	TrailBlazerIdentitiesMethods,
-	TrailBlazersMethods,
-	TrailblazerApiKeysMethods,
 	UserApiKeysMethods,
 	UsersMethods
 ):
 
     def __init__(self, credentials={}, url="", headers={}, timeout=30):
         if type(credentials) != dict:
             raise Exception("invalid parameter: credentials must be a dictionary")
```

### Comparing `kivera-sdk-1.8.0/kivera/cloudtenants/create.py` & `kivera-sdk-1.9.0/kivera/cloudtenants/create.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.8.0/kivera/cloudtenants/delete.py` & `kivera-sdk-1.9.0/kivera/cloudtenants/delete.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.8.0/kivera/cloudtenants/get.py` & `kivera-sdk-1.9.0/kivera/cloudtenants/get.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.8.0/kivera/cloudtenants/list.py` & `kivera-sdk-1.9.0/kivera/cloudtenants/list.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.8.0/kivera/cloudtenants/update.py` & `kivera-sdk-1.9.0/kivera/cloudtenants/update.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.8.0/kivera/compliancemappings/list.py` & `kivera-sdk-1.9.0/kivera/compliancemappings/list.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.8.0/kivera/config/get.py` & `kivera-sdk-1.9.0/kivera/config/get.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.8.0/kivera/counters/get.py` & `kivera-sdk-1.9.0/kivera/counters/get.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.8.0/kivera/globalpolicyfunctions/get.py` & `kivera-sdk-1.9.0/kivera/globalpolicyfunctions/get.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.8.0/kivera/globalpolicyfunctions/list.py` & `kivera-sdk-1.9.0/kivera/globalpolicyfunctions/list.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.8.0/kivera/globalservices/list.py` & `kivera-sdk-1.9.0/kivera/globalservices/list.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.8.0/kivera/identities/create.py` & `kivera-sdk-1.9.0/kivera/identities/create.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.8.0/kivera/identities/delete.py` & `kivera-sdk-1.9.0/kivera/identities/delete.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.8.0/kivera/identities/get.py` & `kivera-sdk-1.9.0/kivera/identities/get.py`

 * *Files 1% similar despite different names*

```diff
@@ -254,14 +254,15 @@
       service_id
       type_id
       enable_cfn_scan
       enforce
       log_request_body
       dependencies_enabled
       tags
+      compliance_mappings
       risk_rating
       policy
       ruleDependenciesByRuleId(where: { deleted: { _eq: false } }) {
         id
         dependent_rule_id
         rule_id
         Rule {
```

### Comparing `kivera-sdk-1.8.0/kivera/identities/list.py` & `kivera-sdk-1.9.0/kivera/identities/list.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.8.0/kivera/identities/update.py` & `kivera-sdk-1.9.0/kivera/identities/update.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.8.0/kivera/identityprofiles/create.py` & `kivera-sdk-1.9.0/kivera/identityprofiles/create.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.8.0/kivera/identityprofiles/delete.py` & `kivera-sdk-1.9.0/kivera/identityprofiles/delete.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.8.0/kivera/identityprofiles/get.py` & `kivera-sdk-1.9.0/kivera/identityprofiles/get.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.8.0/kivera/identityprofiles/list.py` & `kivera-sdk-1.9.0/kivera/identityprofiles/list.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.8.0/kivera/identityprofiles/update.py` & `kivera-sdk-1.9.0/kivera/identityprofiles/update.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.8.0/kivera/identitytypes/get.py` & `kivera-sdk-1.9.0/kivera/identitytypes/get.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.8.0/kivera/identitytypes/list.py` & `kivera-sdk-1.9.0/kivera/identitytypes/list.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.8.0/kivera/managedrules/list.py` & `kivera-sdk-1.9.0/kivera/managedrules/list.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.8.0/kivera/memberships/create.py` & `kivera-sdk-1.9.0/kivera/memberships/create.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.8.0/kivera/memberships/delete.py` & `kivera-sdk-1.9.0/kivera/memberships/delete.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.8.0/kivera/memberships/get.py` & `kivera-sdk-1.9.0/kivera/memberships/get.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.8.0/kivera/memberships/list.py` & `kivera-sdk-1.9.0/kivera/memberships/list.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.8.0/kivera/memberships/update.py` & `kivera-sdk-1.9.0/kivera/memberships/update.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.8.0/kivera/metrics/getcounterproxymetrics.py` & `kivera-sdk-1.9.0/kivera/metrics/getcounterproxymetrics.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.8.0/kivera/notificationmonitors/get.py` & `kivera-sdk-1.9.0/kivera/users/list.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,68 +1,63 @@
 from gql import gql
 from typing import Sequence
 
-class getMethods:
+class listMethods:
 
-    _GetNotificationMonitorQuery = """
-    query GetNotificationMonitor ($id: String!) {
-  NotificationMonitors(where: {id: {_eq: $id}}) {
+    _ListUsersQuery = """
+    query ListUsers {
+  Users {
     id
-    name
-    description
-    org_id
-    enabled
-    query_parameters
-    interval
-    severity
-    NotificationMonitorDestinations {
-      destination_id
+    verified
+    email
+    given_name
+    family_name
+    created_at
+    Memberships {
+      id
+      MembershipRoles {
+        Role {
+          role_name
+          id
+        }
+      }
     }
   }
 }
     """
 
-    def GetNotificationMonitor(self, id: str):
-        query = gql(self._GetNotificationMonitorQuery)
+    def ListUsers(self):
+        query = gql(self._ListUsersQuery)
         variables = {
-            "id": id,
         }
-        operation_name = "GetNotificationMonitor"
+        operation_name = "ListUsers"
         operation_type = "read"
         return self.execute(
             query,
             variable_values=variables,
             operation_name=operation_name,
             operation_type=operation_type,
         )
 
-    _GetNotificationMonitorV2Query = """
-    query GetNotificationMonitorV2($id: String!) {
-  NotificationMonitors_by_pk(id: $id) {
+    _ListVerifiedUsersQuery = """
+    query ListVerifiedUsers {
+  Users(where: {verified: {_eq: true}}) {
     id
-    name
-    description
-    org_id
-    enabled
-    query_parameters
-    interval
-    severity
-    NotificationMonitorDestinations {
-      destination_id
-    }
+    email
+    given_name
+    family_name
   }
 }
     """
 
-    def GetNotificationMonitorV2(self, id: str):
-        query = gql(self._GetNotificationMonitorV2Query)
+    def ListVerifiedUsers(self):
+        query = gql(self._ListVerifiedUsersQuery)
         variables = {
-            "id": id,
         }
-        operation_name = "GetNotificationMonitorV2"
+        operation_name = "ListVerifiedUsers"
         operation_type = "read"
         return self.execute(
             query,
             variable_values=variables,
             operation_name=operation_name,
             operation_type=operation_type,
         )
```

### Comparing `kivera-sdk-1.8.0/kivera/organizationpolicyfunctions/create.py` & `kivera-sdk-1.9.0/kivera/organizationpolicyfunctions/create.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.8.0/kivera/organizationpolicyfunctions/delete.py` & `kivera-sdk-1.9.0/kivera/organizationpolicyfunctions/delete.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.8.0/kivera/organizationpolicyfunctions/get.py` & `kivera-sdk-1.9.0/kivera/organizationpolicyfunctions/get.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.8.0/kivera/organizationpolicyfunctions/list.py` & `kivera-sdk-1.9.0/kivera/organizationpolicyfunctions/list.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.8.0/kivera/organizationpolicyfunctions/update.py` & `kivera-sdk-1.9.0/kivera/organizationpolicyfunctions/update.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.8.0/kivera/organizations/get.py` & `kivera-sdk-1.9.0/kivera/organizations/get.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.8.0/kivera/organizations/list.py` & `kivera-sdk-1.9.0/kivera/organizations/list.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.8.0/kivera/organizations/update.py` & `kivera-sdk-1.9.0/kivera/organizations/update.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.8.0/kivera/plans/list.py` & `kivera-sdk-1.9.0/kivera/plans/list.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.8.0/kivera/profiles/attach.py` & `kivera-sdk-1.9.0/kivera/profiles/attach.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.8.0/kivera/profiles/create.py` & `kivera-sdk-1.9.0/kivera/profiles/create.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.8.0/kivera/profiles/delete.py` & `kivera-sdk-1.9.0/kivera/profiles/delete.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.8.0/kivera/profiles/get.py` & `kivera-sdk-1.9.0/kivera/profiles/get.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.8.0/kivera/profiles/list.py` & `kivera-sdk-1.9.0/kivera/profiles/list.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.8.0/kivera/profiles/update.py` & `kivera-sdk-1.9.0/kivera/profiles/update.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.8.0/kivera/providers/get.py` & `kivera-sdk-1.9.0/kivera/providers/get.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.8.0/kivera/providers/list.py` & `kivera-sdk-1.9.0/kivera/providers/list.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.8.0/kivera/providerversions/list.py` & `kivera-sdk-1.9.0/kivera/providerversions/list.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.8.0/kivera/proxies/create.py` & `kivera-sdk-1.9.0/kivera/proxies/create.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.8.0/kivera/proxies/delete.py` & `kivera-sdk-1.9.0/kivera/proxies/delete.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.8.0/kivera/proxies/get.py` & `kivera-sdk-1.9.0/kivera/proxies/get.py`

 * *Files 0% similar despite different names*

```diff
@@ -388,14 +388,15 @@
       service_id
       type_id
       enable_cfn_scan
       enforce
       log_request_body
       dependencies_enabled
       tags
+      compliance_mappings
       risk_rating
       policy
       ruleDependenciesByRuleId(where: { deleted: { _eq: false } }) {
         id
         dependent_rule_id
         rule_id
         Rule {
```

### Comparing `kivera-sdk-1.8.0/kivera/proxies/list.py` & `kivera-sdk-1.9.0/kivera/proxies/list.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.8.0/kivera/proxies/update.py` & `kivera-sdk-1.9.0/kivera/proxies/update.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.8.0/kivera/proxyapikeys/get.py` & `kivera-sdk-1.9.0/kivera/proxyapikeys/get.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.8.0/kivera/proxydeployments/create.py` & `kivera-sdk-1.9.0/kivera/proxydeployments/create.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.8.0/kivera/proxydeployments/get.py` & `kivera-sdk-1.9.0/kivera/proxydeployments/get.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.8.0/kivera/proxydeployments/list.py` & `kivera-sdk-1.9.0/kivera/proxydeployments/list.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.8.0/kivera/proxydeployments/update.py` & `kivera-sdk-1.9.0/kivera/proxydeployments/update.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.8.0/kivera/proxyproviders/list.py` & `kivera-sdk-1.9.0/kivera/proxyproviders/list.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.8.0/kivera/roles/list.py` & `kivera-sdk-1.9.0/kivera/roles/list.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.8.0/kivera/ruledependencies/attach.py` & `kivera-sdk-1.9.0/kivera/ruledependencies/attach.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.8.0/kivera/ruledependencies/get.py` & `kivera-sdk-1.9.0/kivera/ruledependencies/get.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.8.0/kivera/ruledependencyresources/get.py` & `kivera-sdk-1.9.0/kivera/ruledependencyresources/get.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.8.0/kivera/ruleparameters/get.py` & `kivera-sdk-1.9.0/kivera/ruleparameters/get.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.8.0/kivera/rules/create.py` & `kivera-sdk-1.9.0/kivera/rules/create.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.8.0/kivera/rules/delete.py` & `kivera-sdk-1.9.0/kivera/rules/delete.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.8.0/kivera/rules/get.py` & `kivera-sdk-1.9.0/kivera/rules/get.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.8.0/kivera/rules/list.py` & `kivera-sdk-1.9.0/kivera/rules/list.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.8.0/kivera/rules/update.py` & `kivera-sdk-1.9.0/kivera/rules/update.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.8.0/kivera/services/create.py` & `kivera-sdk-1.9.0/kivera/services/create.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.8.0/kivera/services/delete.py` & `kivera-sdk-1.9.0/kivera/services/delete.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.8.0/kivera/services/get.py` & `kivera-sdk-1.9.0/kivera/services/get.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.8.0/kivera/services/list.py` & `kivera-sdk-1.9.0/kivera/services/list.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.8.0/kivera/services/update.py` & `kivera-sdk-1.9.0/kivera/services/update.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.8.0/kivera/trailblazeridentities/delete.py` & `kivera-sdk-1.9.0/kivera/users/delete.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,31 +1,39 @@
 from gql import gql
 from typing import Sequence
 
 class deleteMethods:
 
-    _DeleteTrailBlazerIdentityQuery = """
-    mutation DeleteTrailBlazerIdentity($id: Int!) {
-  update_TrailBlazerIdentities( where: {id: {_eq: $id}}, _set: {deleted: false}) {
-    returning {
-      deleted
-      id
-      identity_id
-      trailblazer_id
+    _DeleteUserFromOrganizationQuery = """
+    mutation DeleteUserFromOrganization($org_id: Int!, $user_id: String!) {
+    delete_MembershipRoles(where: {Membership: {org_id: {_eq: $org_id}, user_id: {_eq: $user_id}}}) {
+        returning {
+            id
+            membership_id
+            role_id
+        }
+    }
+    delete_Memberships(where: {org_id: {_eq: $org_id}, user_id: {_eq: $user_id}}) {
+        returning {
+            id
+            org_id
+            review_weekly_summary
+            user_id
+        }
     }
-  }
 }
     """
 
-    def DeleteTrailBlazerIdentity(self, id: int):
-        query = gql(self._DeleteTrailBlazerIdentityQuery)
+    def DeleteUserFromOrganization(self, org_id: int, user_id: str):
+        query = gql(self._DeleteUserFromOrganizationQuery)
         variables = {
-            "id": id,
+            "org_id": org_id,
+            "user_id": user_id,
         }
-        operation_name = "DeleteTrailBlazerIdentity"
+        operation_name = "DeleteUserFromOrganization"
         operation_type = "write"
         return self.execute(
             query,
             variable_values=variables,
             operation_name=operation_name,
             operation_type=operation_type,
         )
```

### Comparing `kivera-sdk-1.8.0/kivera/trailblazers/list.py` & `kivera-sdk-1.9.0/kivera/users/get.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,52 +1,83 @@
 from gql import gql
 from typing import Sequence
 
-class listMethods:
+class getMethods:
 
-    _ListTrailBlazersQuery = """
-    query ListTrailBlazers($orgID: Int!) {
-  TrailBlazers(where: {deleted: {_eq: false}, org_id: {_eq: $orgID}}) {
-    description
-    healthcheck_info
+    _GetUserByIdQuery = """
+    query GetUserById($user_id: String!) {
+  Users_by_pk(id: $user_id) {
     id
-    name
-    org_id
-    status
-    tags
-    TrailBlazerSettings {
-      debug
+    verified
+    email
+    given_name
+    family_name
+    created_at
+    timezone
+    country_iso_code
+    Memberships {
       id
-      trailblazer_mode
-    }
-    TrailBlazerIdentities(where: {deleted: {_eq: false}}) {
-      identity_id
-      trailblazer_id
-      deleted
+      Organization {
+        company_name
+        id
+        beta_access
+        Plan {
+          id
+          name
+          proxy_limit
+        }
+      }
     }
-    TrailBlazerCounters_aggregate{
-      aggregate {
-        sum {
-          counter_accepts
-          counter_denials
-          counter_notifies
-          counter_total_request
+  }
+}
+    """
+
+    def GetUserById(self, user_id: str):
+        query = gql(self._GetUserByIdQuery)
+        variables = {
+            "user_id": user_id,
         }
+        operation_name = "GetUserById"
+        operation_type = "read"
+        return self.execute(
+            query,
+            variable_values=variables,
+            operation_name=operation_name,
+            operation_type=operation_type,
+        )
+
+    _GetUserDetailsQuery = """
+    query GetUserDetails($email: String!) {
+  Users(where: {email: {_eq: $email}}) {
+    id
+    verified
+    email
+    given_name
+    family_name
+    created_at
+    timezone
+    country_iso_code
+    Memberships {
+      id
+      Organization {
+        company_name
+        id
+        beta_access
       }
     }
   }
 }
     """
 
-    def ListTrailBlazers(self, orgID: int):
-        query = gql(self._ListTrailBlazersQuery)
+    def GetUserDetails(self, email: str):
+        query = gql(self._GetUserDetailsQuery)
         variables = {
-            "orgID": orgID,
+            "email": email,
         }
-        operation_name = "ListTrailBlazers"
+        operation_name = "GetUserDetails"
         operation_type = "read"
         return self.execute(
             query,
             variable_values=variables,
             operation_name=operation_name,
             operation_type=operation_type,
         )
```

### Comparing `kivera-sdk-1.8.0/kivera/userapikeys/get.py` & `kivera-sdk-1.9.0/kivera/userapikeys/get.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.8.0/kivera/userapikeys/list.py` & `kivera-sdk-1.9.0/kivera/userapikeys/list.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     UserApiKeys {
         client_id
         id
         org_id
         status
         user_id
         created
+        description
         Organization {
             domain
             company_name
         }
     }
 }
     """
```

### Comparing `kivera-sdk-1.8.0/kivera/userapikeys/update.py` & `kivera-sdk-1.9.0/kivera/userapikeys/update.py`

 * *Files 20% similar despite different names*

```diff
@@ -58,14 +58,45 @@
         return self.execute(
             query,
             variable_values=variables,
             operation_name=operation_name,
             operation_type=operation_type,
         )
 
+    _UpdateUserApiKeyDescriptionQuery = """
+    mutation UpdateUserApiKeyDescription($id: Int!, $description: String!) {
+    update_UserApiKeys(where: {id: {_eq: $id}}, _set: {description: $description}) {
+        returning {
+            client_id
+            created
+            id
+            org_id
+            status
+            user_id
+            description
+        }
+    }
+}
+    """
+
+    def UpdateUserApiKeyDescription(self, id: int, description: str):
+        query = gql(self._UpdateUserApiKeyDescriptionQuery)
+        variables = {
+            "id": id,
+            "description": description,
+        }
+        operation_name = "UpdateUserApiKeyDescription"
+        operation_type = "write"
+        return self.execute(
+            query,
+            variable_values=variables,
+            operation_name=operation_name,
+            operation_type=operation_type,
+        )
+
     _UpdateUserApiKeysQuery = """
     mutation UpdateUserApiKeys($user_id: String!, $org_id: Int!, $status: Boolean!) {
     update_UserApiKeys(where: {user_id: {_eq: $user_id}, org_id: {_eq: $org_id}}, _set: {status: $status}) {
         returning {
             client_id
             created
             id
```

### Comparing `kivera-sdk-1.8.0/kivera/users/update.py` & `kivera-sdk-1.9.0/kivera/users/update.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.8.0/kivera_sdk.egg-info/PKG-INFO` & `kivera-sdk-1.9.0/kivera_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kivera-sdk
-Version: 1.8.0
+Version: 1.9.0
 Summary: Python library to interact with the Kivera Graphql API
 Home-page: https://github.com/kivera-io/python-client
 Author: Kivera
 Author-email: support@kivera.io
 License: MIT License
 Keywords: kivera graphql gql sdk client
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `kivera-sdk-1.8.0/kivera_sdk.egg-info/SOURCES.txt` & `kivera-sdk-1.9.0/kivera_sdk.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -42,20 +42,14 @@
 kivera/memberships/create.py
 kivera/memberships/delete.py
 kivera/memberships/get.py
 kivera/memberships/list.py
 kivera/memberships/update.py
 kivera/metrics/__init__.py
 kivera/metrics/getcounterproxymetrics.py
-kivera/notificationdestinations/__init__.py
-kivera/notificationdestinations/get.py
-kivera/notificationdestinations/list.py
-kivera/notificationmonitors/__init__.py
-kivera/notificationmonitors/get.py
-kivera/notificationmonitors/list.py
 kivera/organizationpolicyfunctions/__init__.py
 kivera/organizationpolicyfunctions/create.py
 kivera/organizationpolicyfunctions/delete.py
 kivera/organizationpolicyfunctions/get.py
 kivera/organizationpolicyfunctions/list.py
 kivera/organizationpolicyfunctions/update.py
 kivera/organizations/__init__.py
@@ -108,28 +102,14 @@
 kivera/rules/update.py
 kivera/services/__init__.py
 kivera/services/create.py
 kivera/services/delete.py
 kivera/services/get.py
 kivera/services/list.py
 kivera/services/update.py
-kivera/trailblazerapikeys/__init__.py
-kivera/trailblazerapikeys/get.py
-kivera/trailblazeridentities/__init__.py
-kivera/trailblazeridentities/create.py
-kivera/trailblazeridentities/delete.py
-kivera/trailblazeridentities/get.py
-kivera/trailblazeridentities/list.py
-kivera/trailblazeridentities/update.py
-kivera/trailblazers/__init__.py
-kivera/trailblazers/create.py
-kivera/trailblazers/delete.py
-kivera/trailblazers/get.py
-kivera/trailblazers/list.py
-kivera/trailblazers/update.py
 kivera/userapikeys/__init__.py
 kivera/userapikeys/get.py
 kivera/userapikeys/list.py
 kivera/userapikeys/update.py
 kivera/users/__init__.py
 kivera/users/delete.py
 kivera/users/get.py
```

### Comparing `kivera-sdk-1.8.0/setup.py` & `kivera-sdk-1.9.0/setup.py`

 * *Files identical despite different names*

