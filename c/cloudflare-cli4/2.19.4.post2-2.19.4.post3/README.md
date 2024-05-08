# Comparing `tmp/cloudflare_cli4-2.19.4.post2.tar.gz` & `tmp/cloudflare_cli4-2.19.4.post3.tar.gz`

## Comparing `cloudflare_cli4-2.19.4.post2.tar` & `cloudflare_cli4-2.19.4.post3.tar`

### file list

```diff
@@ -1,105 +1,106 @@
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post2/.coveragerc
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post2/.git
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post2/.mypy.ini
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post2/.python-version
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post2/.readthedocs.yaml
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post2/.travis.yml
--rw-r--r--   0        0        0   116899 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post2/CHANGELOG.md
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post2/MANIFEST.in
--rw-r--r--   0        0        0     4890 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post2/Makefile
--rw-r--r--   0        0        0    54459 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post2/TABLE-OF-COMMANDS.md
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post2/pylintrc
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post2/requirements-dev.lock
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post2/requirements.lock
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post2/requirements.txt
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post2/setup.cfg
--rwxr-xr-x   0        0        0     2370 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post2/setup.py
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post2/CloudFlare/__init__.py
--rw-r--r--   0        0        0     3503 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post2/CloudFlare/api_decode_from_openapi.py
--rw-r--r--   0        0        0     1772 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post2/CloudFlare/api_extras.py
--rw-r--r--   0        0        0    60491 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post2/CloudFlare/api_v4.py
--rw-r--r--   0        0        0    54686 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post2/CloudFlare/cloudflare.py
--rw-r--r--   0        0        0     3316 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post2/CloudFlare/exceptions.py
--rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post2/CloudFlare/logging_helper.py
--rw-r--r--   0        0        0     3974 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post2/CloudFlare/network.py
--rw-r--r--   0        0        0     5621 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post2/CloudFlare/read_configs.py
--rw-r--r--   0        0        0     4081 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post2/CloudFlare/utils.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post2/CloudFlare/tests/__init__.py
--rw-r--r--   0        0        0    13359 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post2/CloudFlare/tests/dummy_loa_document.pdf
--rw-r--r--   0        0        0     1981 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post2/CloudFlare/tests/test_add.py
--rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post2/CloudFlare/tests/test_api_dump.py
--rw-r--r--   0        0        0     2225 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post2/CloudFlare/tests/test_certificates.py
--rwxr-xr-x   0        0        0     3489 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post2/CloudFlare/tests/test_cloudflare.py
--rw-r--r--   0        0        0     5983 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post2/CloudFlare/tests/test_cloudflare_calls.py
--rw-r--r--   0        0        0     3781 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post2/CloudFlare/tests/test_dns_import_export.py
--rw-r--r--   0        0        0     5754 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post2/CloudFlare/tests/test_dns_records.py
--rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post2/CloudFlare/tests/test_find.py
--rw-r--r--   0        0        0     6722 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post2/CloudFlare/tests/test_graphql.py
--rw-r--r--   0        0        0     5887 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post2/CloudFlare/tests/test_images_v2_direct_upload.py
--rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post2/CloudFlare/tests/test_ips.py
--rw-r--r--   0        0        0     9169 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post2/CloudFlare/tests/test_issue114.py
--rw-r--r--   0        0        0     6512 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post2/CloudFlare/tests/test_loa_documents.py
--rw-r--r--   0        0        0    10741 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post2/CloudFlare/tests/test_load_balancers.py
--rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post2/CloudFlare/tests/test_log_received.py
--rw-r--r--   0        0        0     2958 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post2/CloudFlare/tests/test_paging_thru_zones.py
--rw-r--r--   0        0        0     2491 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post2/CloudFlare/tests/test_purge_cache.py
--rw-r--r--   0        0        0     1432 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post2/CloudFlare/tests/test_radar_returning_csv.py
--rw-r--r--   0        0        0     7229 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post2/CloudFlare/tests/test_rulesets.py
--rw-r--r--   0        0        0     3824 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post2/CloudFlare/tests/test_urlscanner.py
--rw-r--r--   0        0        0     3687 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post2/CloudFlare/tests/test_waiting_room.py
--rw-r--r--   0        0        0     4304 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post2/CloudFlare/tests/test_workers.py
--rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post2/CloudFlare/tests/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post2/cli4/__init__.py
--rwxr-xr-x   0        0        0      262 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post2/cli4/__main__.py
--rw-r--r--   0        0        0     4610 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post2/cli4/cli4.1
--rw-r--r--   0        0        0    21628 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post2/cli4/cli4.py
--rw-r--r--   0        0        0     5829 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post2/cli4/converters.py
--rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post2/cli4/dump.py
--rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post2/cli4/examples.py
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post2/cli4/myjsonlines.py
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post2/cli4/myyaml.py
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post2/docs/Makefile
--rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post2/docs/conf.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post2/docs/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post2/examples/__init__.py
--rwxr-xr-x   0        0        0     2779 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post2/examples/example_account_rules_lists_items.py
--rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post2/examples/example_ai_images.py
--rw-r--r--   0        0        0     4612 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post2/examples/example_ai_speechrecognition.py
--rw-r--r--   0        0        0     1866 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post2/examples/example_ai_translate.py
--rwxr-xr-x   0        0        0     1988 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post2/examples/example_always_use_https.py
--rwxr-xr-x   0        0        0     1875 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post2/examples/example_are_zones_ipv6.py
--rwxr-xr-x   0        0        0      557 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post2/examples/example_are_zones_ipv6_simple.py
--rwxr-xr-x   0        0        0     1732 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post2/examples/example_bot_management.py
--rwxr-xr-x   0        0        0     2672 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post2/examples/example_certificates.py
--rwxr-xr-x   0        0        0     3934 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post2/examples/example_create_zone_and_populate.py
--rwxr-xr-x   0        0        0     2279 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post2/examples/example_custom_hostnames.py
--rwxr-xr-x   0        0        0     2033 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post2/examples/example_delete_zone_entry.py
--rwxr-xr-x   0        0        0     1378 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post2/examples/example_dns_export.py
--rwxr-xr-x   0        0        0     1463 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post2/examples/example_dns_import.py
--rwxr-xr-x   0        0        0     1458 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post2/examples/example_dnssec_settings.py
--rw-r--r--   0        0        0     3512 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post2/examples/example_firewall_rules.py
--rwxr-xr-x   0        0        0     2380 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post2/examples/example_graphql.py
--rwxr-xr-x   0        0        0      981 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post2/examples/example_graphql.sh
--rw-r--r--   0        0        0     8092 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post2/examples/example_images_v2_direct_upload.py
--rwxr-xr-x   0        0        0      762 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post2/examples/example_ips.py
--rwxr-xr-x   0        0        0     1915 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post2/examples/example_list_api_from_web.py
--rwxr-xr-x   0        0        0     2206 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post2/examples/example_page_rules.py
--rwxr-xr-x   0        0        0      440 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post2/examples/example_page_rules.sh
--rwxr-xr-x   0        0        0     1202 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post2/examples/example_paging_thru_zones.py
--rwxr-xr-x   0        0        0      782 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post2/examples/example_paging_thru_zones.sh
--rwxr-xr-x   0        0        0     3387 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post2/examples/example_proxied.py
--rwxr-xr-x   0        0        0     1841 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post2/examples/example_settings.py
--rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post2/examples/example_show_zones_email.py
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post2/examples/example_time_calls.py
--rwxr-xr-x   0        0        0     4320 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post2/examples/example_update_dynamic_dns.py
--rwxr-xr-x   0        0        0     5570 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post2/examples/example_user.py
--rwxr-xr-x   0        0        0     2188 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post2/examples/example_user_tokens.py
--rwxr-xr-x   0        0        0      676 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post2/examples/example_with_usage.py
--rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post2/examples/example_zone_purge_cache.py
--rwxr-xr-x   0        0        0      421 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post2/examples/example_zone_search.sh
--rwxr-xr-x   0        0        0     2368 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post2/examples/example_zones.py
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post2/.gitignore
--rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post2/LICENSE
--rw-r--r--   0        0        0    35977 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post2/README.md
--rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post2/pyproject.toml
--rw-r--r--   0        0        0    37201 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post2/PKG-INFO
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post3/.coveragerc
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post3/.mypy.ini
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post3/.python-version
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post3/.readthedocs.yaml
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post3/.travis.yml
+-rw-r--r--   0        0        0   116899 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post3/CHANGELOG.md
+-rw-r--r--   0        0        0     3021 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post3/HOW-TO-PACKAGE.md
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post3/MANIFEST.in
+-rw-r--r--   0        0        0     4862 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post3/Makefile
+-rw-r--r--   0        0        0    54459 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post3/TABLE-OF-COMMANDS.md
+-rw-r--r--   0        0        0     3076 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post3/brew-formula-cloudflare-cli4.rb
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post3/pylintrc
+-rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post3/requirements-dev.lock
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post3/requirements.lock
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post3/requirements.txt
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post3/setup.cfg
+-rwxr-xr-x   0        0        0     2370 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post3/setup.py
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post3/CloudFlare/__init__.py
+-rw-r--r--   0        0        0     3503 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post3/CloudFlare/api_decode_from_openapi.py
+-rw-r--r--   0        0        0     1772 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post3/CloudFlare/api_extras.py
+-rw-r--r--   0        0        0    60491 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post3/CloudFlare/api_v4.py
+-rw-r--r--   0        0        0    54623 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post3/CloudFlare/cloudflare.py
+-rw-r--r--   0        0        0     3316 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post3/CloudFlare/exceptions.py
+-rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post3/CloudFlare/logging_helper.py
+-rw-r--r--   0        0        0     3974 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post3/CloudFlare/network.py
+-rw-r--r--   0        0        0     5621 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post3/CloudFlare/read_configs.py
+-rw-r--r--   0        0        0     4081 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post3/CloudFlare/utils.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post3/CloudFlare/tests/__init__.py
+-rw-r--r--   0        0        0    13359 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post3/CloudFlare/tests/dummy_loa_document.pdf
+-rw-r--r--   0        0        0     1981 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post3/CloudFlare/tests/test_add.py
+-rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post3/CloudFlare/tests/test_api_dump.py
+-rw-r--r--   0        0        0     2225 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post3/CloudFlare/tests/test_certificates.py
+-rwxr-xr-x   0        0        0     3489 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post3/CloudFlare/tests/test_cloudflare.py
+-rw-r--r--   0        0        0     5983 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post3/CloudFlare/tests/test_cloudflare_calls.py
+-rw-r--r--   0        0        0     3781 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post3/CloudFlare/tests/test_dns_import_export.py
+-rw-r--r--   0        0        0     5754 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post3/CloudFlare/tests/test_dns_records.py
+-rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post3/CloudFlare/tests/test_find.py
+-rw-r--r--   0        0        0     6722 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post3/CloudFlare/tests/test_graphql.py
+-rw-r--r--   0        0        0     5887 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post3/CloudFlare/tests/test_images_v2_direct_upload.py
+-rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post3/CloudFlare/tests/test_ips.py
+-rw-r--r--   0        0        0     9169 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post3/CloudFlare/tests/test_issue114.py
+-rw-r--r--   0        0        0     6512 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post3/CloudFlare/tests/test_loa_documents.py
+-rw-r--r--   0        0        0    10741 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post3/CloudFlare/tests/test_load_balancers.py
+-rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post3/CloudFlare/tests/test_log_received.py
+-rw-r--r--   0        0        0     2958 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post3/CloudFlare/tests/test_paging_thru_zones.py
+-rw-r--r--   0        0        0     2491 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post3/CloudFlare/tests/test_purge_cache.py
+-rw-r--r--   0        0        0     1432 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post3/CloudFlare/tests/test_radar_returning_csv.py
+-rw-r--r--   0        0        0     7229 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post3/CloudFlare/tests/test_rulesets.py
+-rw-r--r--   0        0        0     3824 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post3/CloudFlare/tests/test_urlscanner.py
+-rw-r--r--   0        0        0     3687 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post3/CloudFlare/tests/test_waiting_room.py
+-rw-r--r--   0        0        0     4304 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post3/CloudFlare/tests/test_workers.py
+-rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post3/CloudFlare/tests/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post3/cli4/__init__.py
+-rwxr-xr-x   0        0        0      262 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post3/cli4/__main__.py
+-rw-r--r--   0        0        0     4610 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post3/cli4/cli4.1
+-rw-r--r--   0        0        0    21628 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post3/cli4/cli4.py
+-rw-r--r--   0        0        0     5829 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post3/cli4/converters.py
+-rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post3/cli4/dump.py
+-rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post3/cli4/examples.py
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post3/cli4/myjsonlines.py
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post3/cli4/myyaml.py
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post3/docs/Makefile
+-rw-r--r--   0        0        0     1343 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post3/docs/conf.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post3/docs/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post3/examples/__init__.py
+-rwxr-xr-x   0        0        0     2779 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post3/examples/example_account_rules_lists_items.py
+-rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post3/examples/example_ai_images.py
+-rw-r--r--   0        0        0     4612 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post3/examples/example_ai_speechrecognition.py
+-rw-r--r--   0        0        0     1866 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post3/examples/example_ai_translate.py
+-rwxr-xr-x   0        0        0     1988 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post3/examples/example_always_use_https.py
+-rwxr-xr-x   0        0        0     1875 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post3/examples/example_are_zones_ipv6.py
+-rwxr-xr-x   0        0        0      557 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post3/examples/example_are_zones_ipv6_simple.py
+-rwxr-xr-x   0        0        0     1732 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post3/examples/example_bot_management.py
+-rwxr-xr-x   0        0        0     2672 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post3/examples/example_certificates.py
+-rwxr-xr-x   0        0        0     3934 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post3/examples/example_create_zone_and_populate.py
+-rwxr-xr-x   0        0        0     2279 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post3/examples/example_custom_hostnames.py
+-rwxr-xr-x   0        0        0     2033 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post3/examples/example_delete_zone_entry.py
+-rwxr-xr-x   0        0        0     1378 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post3/examples/example_dns_export.py
+-rwxr-xr-x   0        0        0     1463 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post3/examples/example_dns_import.py
+-rwxr-xr-x   0        0        0     1458 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post3/examples/example_dnssec_settings.py
+-rw-r--r--   0        0        0     3512 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post3/examples/example_firewall_rules.py
+-rwxr-xr-x   0        0        0     2380 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post3/examples/example_graphql.py
+-rwxr-xr-x   0        0        0      981 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post3/examples/example_graphql.sh
+-rw-r--r--   0        0        0     8092 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post3/examples/example_images_v2_direct_upload.py
+-rwxr-xr-x   0        0        0      762 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post3/examples/example_ips.py
+-rwxr-xr-x   0        0        0     1915 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post3/examples/example_list_api_from_web.py
+-rwxr-xr-x   0        0        0     2206 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post3/examples/example_page_rules.py
+-rwxr-xr-x   0        0        0      440 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post3/examples/example_page_rules.sh
+-rwxr-xr-x   0        0        0     1202 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post3/examples/example_paging_thru_zones.py
+-rwxr-xr-x   0        0        0      782 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post3/examples/example_paging_thru_zones.sh
+-rwxr-xr-x   0        0        0     3387 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post3/examples/example_proxied.py
+-rwxr-xr-x   0        0        0     1841 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post3/examples/example_settings.py
+-rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post3/examples/example_show_zones_email.py
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post3/examples/example_time_calls.py
+-rwxr-xr-x   0        0        0     4320 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post3/examples/example_update_dynamic_dns.py
+-rwxr-xr-x   0        0        0     5570 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post3/examples/example_user.py
+-rwxr-xr-x   0        0        0     2188 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post3/examples/example_user_tokens.py
+-rwxr-xr-x   0        0        0      676 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post3/examples/example_with_usage.py
+-rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post3/examples/example_zone_purge_cache.py
+-rwxr-xr-x   0        0        0      421 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post3/examples/example_zone_search.sh
+-rwxr-xr-x   0        0        0     2368 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post3/examples/example_zones.py
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post3/.gitignore
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post3/LICENSE
+-rw-r--r--   0        0        0    35913 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post3/README.md
+-rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post3/pyproject.toml
+-rw-r--r--   0        0        0    37131 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post3/PKG-INFO
```

### Comparing `cloudflare_cli4-2.19.4.post2/.readthedocs.yaml` & `cloudflare_cli4-2.19.4.post3/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4.post2/CHANGELOG.md` & `cloudflare_cli4-2.19.4.post3/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4.post2/Makefile` & `cloudflare_cli4-2.19.4.post3/Makefile`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # PANDOC = pandoc
 PYLINT = pylint
 TWINE = twine
 PYTEST = pytest
 
 SPHINX_RELEASE = 2.20.0
 SPHINX_AUTHOR = Martin J. Levy
-SPHINX_COPYRIGHT = Copyright (c) 2016 thru 2024, Cloudflare. 2024 onward, Stainless Inc. All rights reserved.
+SPHINX_COPYRIGHT = Copyright (c) 2016 thru 2024, Cloudflare. All rights reserved.
 
 EMAIL = "mahtin@mahtin.com"
 NAME = "cloudflare"
 
 #all:	README.rst CHANGELOG.md build
 all:	CHANGELOG.md build
```

### Comparing `cloudflare_cli4-2.19.4.post2/TABLE-OF-COMMANDS.md` & `cloudflare_cli4-2.19.4.post3/TABLE-OF-COMMANDS.md`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4.post2/pylintrc` & `cloudflare_cli4-2.19.4.post3/pylintrc`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4.post2/setup.py` & `cloudflare_cli4-2.19.4.post3/setup.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4.post2/CloudFlare/api_decode_from_openapi.py` & `cloudflare_cli4-2.19.4.post3/CloudFlare/api_decode_from_openapi.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4.post2/CloudFlare/api_extras.py` & `cloudflare_cli4-2.19.4.post3/CloudFlare/api_extras.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4.post2/CloudFlare/api_v4.py` & `cloudflare_cli4-2.19.4.post3/CloudFlare/api_v4.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4.post2/CloudFlare/cloudflare.py` & `cloudflare_cli4-2.19.4.post3/CloudFlare/cloudflare.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """ Cloudflare v4 API
 
 A Python interface Cloudflare's v4 API.
 
 See README.md for detailed/further reading.
 
 Copyright (c) 2016 thru 2024, Cloudflare. All rights reserved.
-Copyright (c) 2024 onward, Stainless Inc. All rights reserved.
 """
 
 import json
 import keyword
 
 from .network import CFnetwork, CFnetworkError
 from .logging_helper import CFlogger
```

### Comparing `cloudflare_cli4-2.19.4.post2/CloudFlare/exceptions.py` & `cloudflare_cli4-2.19.4.post3/CloudFlare/exceptions.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4.post2/CloudFlare/logging_helper.py` & `cloudflare_cli4-2.19.4.post3/CloudFlare/logging_helper.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4.post2/CloudFlare/network.py` & `cloudflare_cli4-2.19.4.post3/CloudFlare/network.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4.post2/CloudFlare/read_configs.py` & `cloudflare_cli4-2.19.4.post3/CloudFlare/read_configs.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4.post2/CloudFlare/utils.py` & `cloudflare_cli4-2.19.4.post3/CloudFlare/utils.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4.post2/CloudFlare/tests/dummy_loa_document.pdf` & `cloudflare_cli4-2.19.4.post3/CloudFlare/tests/dummy_loa_document.pdf`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4.post2/CloudFlare/tests/test_add.py` & `cloudflare_cli4-2.19.4.post3/CloudFlare/tests/test_add.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4.post2/CloudFlare/tests/test_api_dump.py` & `cloudflare_cli4-2.19.4.post3/CloudFlare/tests/test_api_dump.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4.post2/CloudFlare/tests/test_certificates.py` & `cloudflare_cli4-2.19.4.post3/CloudFlare/tests/test_certificates.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4.post2/CloudFlare/tests/test_cloudflare.py` & `cloudflare_cli4-2.19.4.post3/CloudFlare/tests/test_cloudflare.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4.post2/CloudFlare/tests/test_cloudflare_calls.py` & `cloudflare_cli4-2.19.4.post3/CloudFlare/tests/test_cloudflare_calls.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4.post2/CloudFlare/tests/test_dns_import_export.py` & `cloudflare_cli4-2.19.4.post3/CloudFlare/tests/test_dns_import_export.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4.post2/CloudFlare/tests/test_dns_records.py` & `cloudflare_cli4-2.19.4.post3/CloudFlare/tests/test_dns_records.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4.post2/CloudFlare/tests/test_find.py` & `cloudflare_cli4-2.19.4.post3/CloudFlare/tests/test_find.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4.post2/CloudFlare/tests/test_graphql.py` & `cloudflare_cli4-2.19.4.post3/CloudFlare/tests/test_graphql.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4.post2/CloudFlare/tests/test_images_v2_direct_upload.py` & `cloudflare_cli4-2.19.4.post3/CloudFlare/tests/test_images_v2_direct_upload.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4.post2/CloudFlare/tests/test_ips.py` & `cloudflare_cli4-2.19.4.post3/CloudFlare/tests/test_ips.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4.post2/CloudFlare/tests/test_issue114.py` & `cloudflare_cli4-2.19.4.post3/CloudFlare/tests/test_issue114.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4.post2/CloudFlare/tests/test_loa_documents.py` & `cloudflare_cli4-2.19.4.post3/CloudFlare/tests/test_loa_documents.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4.post2/CloudFlare/tests/test_load_balancers.py` & `cloudflare_cli4-2.19.4.post3/CloudFlare/tests/test_load_balancers.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4.post2/CloudFlare/tests/test_log_received.py` & `cloudflare_cli4-2.19.4.post3/CloudFlare/tests/test_log_received.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4.post2/CloudFlare/tests/test_paging_thru_zones.py` & `cloudflare_cli4-2.19.4.post3/CloudFlare/tests/test_paging_thru_zones.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4.post2/CloudFlare/tests/test_purge_cache.py` & `cloudflare_cli4-2.19.4.post3/CloudFlare/tests/test_purge_cache.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4.post2/CloudFlare/tests/test_radar_returning_csv.py` & `cloudflare_cli4-2.19.4.post3/CloudFlare/tests/test_radar_returning_csv.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4.post2/CloudFlare/tests/test_rulesets.py` & `cloudflare_cli4-2.19.4.post3/CloudFlare/tests/test_rulesets.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4.post2/CloudFlare/tests/test_urlscanner.py` & `cloudflare_cli4-2.19.4.post3/CloudFlare/tests/test_urlscanner.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4.post2/CloudFlare/tests/test_waiting_room.py` & `cloudflare_cli4-2.19.4.post3/CloudFlare/tests/test_waiting_room.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4.post2/CloudFlare/tests/test_workers.py` & `cloudflare_cli4-2.19.4.post3/CloudFlare/tests/test_workers.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4.post2/CloudFlare/tests/utils.py` & `cloudflare_cli4-2.19.4.post3/CloudFlare/tests/utils.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4.post2/cli4/cli4.1` & `cloudflare_cli4-2.19.4.post3/cli4/cli4.1`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4.post2/cli4/cli4.py` & `cloudflare_cli4-2.19.4.post3/cli4/cli4.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4.post2/cli4/converters.py` & `cloudflare_cli4-2.19.4.post3/cli4/converters.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4.post2/cli4/dump.py` & `cloudflare_cli4-2.19.4.post3/cli4/dump.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4.post2/cli4/examples.py` & `cloudflare_cli4-2.19.4.post3/cli4/examples.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4.post2/cli4/myyaml.py` & `cloudflare_cli4-2.19.4.post3/cli4/myyaml.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4.post2/docs/Makefile` & `cloudflare_cli4-2.19.4.post3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4.post2/docs/conf.py` & `cloudflare_cli4-2.19.4.post3/docs/conf.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # For the full list of built-in configuration values, see the documentation:
 # https://www.sphinx-doc.org/en/master/usage/configuration.html
 
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 
 project = 'python-cloudflare'
-copyright = 'Copyright (c) 2016 thru 2024, Cloudflare. 2024 onward, Stainless Inc. All rights reserved. '
+copyright = 'Copyright (c) 2016 thru 2024, Cloudflare. All rights reserved. '
 author = 'Martin J Levy'
 
 version = '2.20.0'
 release = '2.20.0'
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
```

### Comparing `cloudflare_cli4-2.19.4.post2/examples/example_account_rules_lists_items.py` & `cloudflare_cli4-2.19.4.post3/examples/example_account_rules_lists_items.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4.post2/examples/example_ai_images.py` & `cloudflare_cli4-2.19.4.post3/examples/example_ai_images.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4.post2/examples/example_ai_speechrecognition.py` & `cloudflare_cli4-2.19.4.post3/examples/example_ai_speechrecognition.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4.post2/examples/example_ai_translate.py` & `cloudflare_cli4-2.19.4.post3/examples/example_ai_translate.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4.post2/examples/example_always_use_https.py` & `cloudflare_cli4-2.19.4.post3/examples/example_always_use_https.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4.post2/examples/example_are_zones_ipv6.py` & `cloudflare_cli4-2.19.4.post3/examples/example_are_zones_ipv6.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4.post2/examples/example_are_zones_ipv6_simple.py` & `cloudflare_cli4-2.19.4.post3/examples/example_are_zones_ipv6_simple.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4.post2/examples/example_bot_management.py` & `cloudflare_cli4-2.19.4.post3/examples/example_bot_management.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4.post2/examples/example_certificates.py` & `cloudflare_cli4-2.19.4.post3/examples/example_certificates.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4.post2/examples/example_create_zone_and_populate.py` & `cloudflare_cli4-2.19.4.post3/examples/example_create_zone_and_populate.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4.post2/examples/example_custom_hostnames.py` & `cloudflare_cli4-2.19.4.post3/examples/example_custom_hostnames.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4.post2/examples/example_delete_zone_entry.py` & `cloudflare_cli4-2.19.4.post3/examples/example_delete_zone_entry.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4.post2/examples/example_dns_export.py` & `cloudflare_cli4-2.19.4.post3/examples/example_dns_export.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4.post2/examples/example_dns_import.py` & `cloudflare_cli4-2.19.4.post3/examples/example_dns_import.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4.post2/examples/example_dnssec_settings.py` & `cloudflare_cli4-2.19.4.post3/examples/example_dnssec_settings.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4.post2/examples/example_firewall_rules.py` & `cloudflare_cli4-2.19.4.post3/examples/example_firewall_rules.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4.post2/examples/example_graphql.py` & `cloudflare_cli4-2.19.4.post3/examples/example_graphql.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4.post2/examples/example_graphql.sh` & `cloudflare_cli4-2.19.4.post3/examples/example_graphql.sh`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4.post2/examples/example_images_v2_direct_upload.py` & `cloudflare_cli4-2.19.4.post3/examples/example_images_v2_direct_upload.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4.post2/examples/example_ips.py` & `cloudflare_cli4-2.19.4.post3/examples/example_ips.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4.post2/examples/example_list_api_from_web.py` & `cloudflare_cli4-2.19.4.post3/examples/example_list_api_from_web.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4.post2/examples/example_page_rules.py` & `cloudflare_cli4-2.19.4.post3/examples/example_page_rules.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4.post2/examples/example_paging_thru_zones.py` & `cloudflare_cli4-2.19.4.post3/examples/example_paging_thru_zones.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4.post2/examples/example_paging_thru_zones.sh` & `cloudflare_cli4-2.19.4.post3/examples/example_paging_thru_zones.sh`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4.post2/examples/example_proxied.py` & `cloudflare_cli4-2.19.4.post3/examples/example_proxied.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4.post2/examples/example_settings.py` & `cloudflare_cli4-2.19.4.post3/examples/example_settings.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4.post2/examples/example_show_zones_email.py` & `cloudflare_cli4-2.19.4.post3/examples/example_show_zones_email.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4.post2/examples/example_time_calls.py` & `cloudflare_cli4-2.19.4.post3/examples/example_time_calls.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4.post2/examples/example_update_dynamic_dns.py` & `cloudflare_cli4-2.19.4.post3/examples/example_update_dynamic_dns.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4.post2/examples/example_user.py` & `cloudflare_cli4-2.19.4.post3/examples/example_user.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4.post2/examples/example_user_tokens.py` & `cloudflare_cli4-2.19.4.post3/examples/example_user_tokens.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4.post2/examples/example_with_usage.py` & `cloudflare_cli4-2.19.4.post3/examples/example_with_usage.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4.post2/examples/example_zone_purge_cache.py` & `cloudflare_cli4-2.19.4.post3/examples/example_zone_purge_cache.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4.post2/examples/example_zones.py` & `cloudflare_cli4-2.19.4.post3/examples/example_zones.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4.post2/.gitignore` & `cloudflare_cli4-2.19.4.post3/.gitignore`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4.post2/LICENSE` & `cloudflare_cli4-2.19.4.post3/LICENSE`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 The MIT License (MIT)
 
 Copyright (c) 2016 Felix Wong and contributors
 Copyright (c) 2016 thru 2024, Cloudflare and contributors
-Copyright (c) 2024, Stainless Inc. and contributors
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `cloudflare_cli4-2.19.4.post2/README.md` & `cloudflare_cli4-2.19.4.post3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -12,23 +12,23 @@
 Starting with `cloudflare` v3 this Python CLI will be packaged separately and won't be actively developped anymore.
 
 ## Install
 
 ### Using `rye`
 
 ```shell
-$ git clone https://github.com/stainless-api/python-cloudflare-cli4
+$ git clone https://github.com/cloudflare/python-cloudflare-cli4
 $ cd python-cloudflare-cli4
 $ rye sync
 ```
 
 ### Using `pip`
 
 ```shell
-$ git clone https://github.com/stainless-api/python-cloudflare-cli4
+$ git clone https://github.com/cloudflare/python-cloudflare-cli4
 $ cd python-cloudflare-cli4
 $ pyton -m pip install .
 ```
 
 ### Using shell environment variables
 
 Note (for latest version of code):
@@ -985,24 +985,24 @@
 As of late 2023 the code is Python3.11 clean.
 
 As of April 2024 the code is officially marked as 3.x only (3.6 and above to be specific) such that it can become PEP561 specific.
 
 ## pypi and GitHub signed releases
 
 As of October 2022, the code is signed by the maintainers personal email address: `mahtin@mahtin.com` `7EA1 39C4 0C1C 842F 9D41 AAF9 4A34 925D 0517 2859`
-As of May 2024, the code has been moved to [Stainless Inc.](https://github.com/stainless-api) GitHub's organization.
+As of May 2024, the code has been moved from [cloudflare/cloudflare-python](https://github.com/cloudflare/cloudflare-python) to [cloudflare/python-cloudflare-cli4](https://github.com/cloudflare/python-cloudflare-cli4).
 
 ## Credit
 
 Based on original work from [Felix Wong (gnowxilef)](https://github.com/gnowxilef) found [here](https://github.com/cloudflare-api/python-cloudflare-v4).
+
 Maintained until 2024 by [Martin J. Levy (mahtin)](https://github.com/mahtin).
-The ownership has been officially transferred to [Stainless Inc](http://stainlessapi.com) in 2024.
 
 ## Changelog
 
 An automatically generated CHANGELOG is provided [here](CHANGELOG.md).
 
 ## Copyright
 
 Copyright (c) 2016 thru 2024, Cloudflare. All rights reserved.
-Copyright (c) 2024 onward, Stainless Inc. All rights reserved.
+
 Previous portions copyright [Felix Wong (gnowxilef)](https://github.com/gnowxilef).
```

### Comparing `cloudflare_cli4-2.19.4.post2/pyproject.toml` & `cloudflare_cli4-2.19.4.post3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "cloudflare-cli4"
-version = "2.19.4-2"
+version = "2.19.4-3"
 readme = "README.md"
 description = "Command line tool to interact with Cloudflare API v4"
 authors = [
     { name = "Stainless Inc.", email = "support@stainlessapi.com" },
     { name = "Martin J. Levy", email = "mahtin@mahtin.com" },
 ]
 classifiers = [
@@ -25,16 +25,16 @@
 requires-python = ">3.6.0"
 license = { text = "MIT" }
 
 keywords = ["cloudflare", "API", "wrapper"]
 dependencies = ["requests", "pyyaml", "jsonlines"]
 
 [project.urls]
-documentation = "https://github.com/stainless-api/python-cloudflare-cli4"
-source-code = "https://github.com/stainless-api/python-cloudflare-cli4"
+documentation = "https://github.com/cloudflare/python-cloudflare-cli4"
+source-code = "https://github.com/cloudflare/python-cloudflare-cli4"
 
 [project.scripts]
 cli4 = "cli4.__main__:main"
 
 [project.data-files]
 "share/man/man1" = ["cli4/cli4.1"]
```

### Comparing `cloudflare_cli4-2.19.4.post2/PKG-INFO` & `cloudflare_cli4-2.19.4.post3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.3
 Name: cloudflare-cli4
-Version: 2.19.4.post2
+Version: 2.19.4.post3
 Summary: Command line tool to interact with Cloudflare API v4
-Project-URL: documentation, https://github.com/stainless-api/python-cloudflare-cli4
-Project-URL: source-code, https://github.com/stainless-api/python-cloudflare-cli4
+Project-URL: documentation, https://github.com/cloudflare/python-cloudflare-cli4
+Project-URL: source-code, https://github.com/cloudflare/python-cloudflare-cli4
 Author-email: "Stainless Inc." <support@stainlessapi.com>, "Martin J. Levy" <mahtin@mahtin.com>
 License: MIT
 License-File: LICENSE
 Keywords: API,cloudflare,wrapper
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -40,23 +40,23 @@
 Starting with `cloudflare` v3 this Python CLI will be packaged separately and won't be actively developped anymore.
 
 ## Install
 
 ### Using `rye`
 
 ```shell
-$ git clone https://github.com/stainless-api/python-cloudflare-cli4
+$ git clone https://github.com/cloudflare/python-cloudflare-cli4
 $ cd python-cloudflare-cli4
 $ rye sync
 ```
 
 ### Using `pip`
 
 ```shell
-$ git clone https://github.com/stainless-api/python-cloudflare-cli4
+$ git clone https://github.com/cloudflare/python-cloudflare-cli4
 $ cd python-cloudflare-cli4
 $ pyton -m pip install .
 ```
 
 ### Using shell environment variables
 
 Note (for latest version of code):
@@ -1013,24 +1013,24 @@
 As of late 2023 the code is Python3.11 clean.
 
 As of April 2024 the code is officially marked as 3.x only (3.6 and above to be specific) such that it can become PEP561 specific.
 
 ## pypi and GitHub signed releases
 
 As of October 2022, the code is signed by the maintainers personal email address: `mahtin@mahtin.com` `7EA1 39C4 0C1C 842F 9D41 AAF9 4A34 925D 0517 2859`
-As of May 2024, the code has been moved to [Stainless Inc.](https://github.com/stainless-api) GitHub's organization.
+As of May 2024, the code has been moved from [cloudflare/cloudflare-python](https://github.com/cloudflare/cloudflare-python) to [cloudflare/python-cloudflare-cli4](https://github.com/cloudflare/python-cloudflare-cli4).
 
 ## Credit
 
 Based on original work from [Felix Wong (gnowxilef)](https://github.com/gnowxilef) found [here](https://github.com/cloudflare-api/python-cloudflare-v4).
+
 Maintained until 2024 by [Martin J. Levy (mahtin)](https://github.com/mahtin).
-The ownership has been officially transferred to [Stainless Inc](http://stainlessapi.com) in 2024.
 
 ## Changelog
 
 An automatically generated CHANGELOG is provided [here](CHANGELOG.md).
 
 ## Copyright
 
 Copyright (c) 2016 thru 2024, Cloudflare. All rights reserved.
-Copyright (c) 2024 onward, Stainless Inc. All rights reserved.
+
 Previous portions copyright [Felix Wong (gnowxilef)](https://github.com/gnowxilef).
```

