# Comparing `tmp/bidfx-api-1.1.1.tar.gz` & `tmp/bidfx-api-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bidfx-api-1.1.1.tar", last modified: Fri Jan  5 17:49:42 2024, max compression
+gzip compressed data, was "bidfx-api-1.1.2.tar", last modified: Wed May  8 11:33:58 2024, max compression
```

## Comparing `bidfx-api-1.1.1.tar` & `bidfx-api-1.1.2.tar`

### file list

```diff
@@ -1,75 +1,74 @@
-drwxrwxrwx   0        0        0        0 2024-01-05 17:49:42.570278 bidfx-api-1.1.1/
--rw-rw-rw-   0        0        0     4627 2022-03-09 16:38:13.000000 bidfx-api-1.1.1/DEVELOPMENT.md
--rw-rw-rw-   0        0        0    11357 2022-03-09 12:03:11.000000 bidfx-api-1.1.1/LICENSE-2.0.txt
--rw-rw-rw-   0        0        0      165 2022-03-09 12:03:11.000000 bidfx-api-1.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0     2649 2024-01-05 17:49:42.568284 bidfx-api-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1692 2024-01-05 17:40:37.000000 bidfx-api-1.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-01-05 17:49:42.441261 bidfx-api-1.1.1/bidfx/
--rw-rw-rw-   0        0        0      160 2024-01-05 17:36:56.000000 bidfx-api-1.1.1/bidfx/__init__.py
--rw-rw-rw-   0        0        0      776 2024-01-05 17:36:56.000000 bidfx-api-1.1.1/bidfx/_bidfx_api.py
--rw-rw-rw-   0        0        0      718 2022-03-09 12:03:11.000000 bidfx-api-1.1.1/bidfx/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-01-05 17:49:42.462263 bidfx-api-1.1.1/bidfx/pricing/
--rw-rw-rw-   0        0        0      530 2022-03-09 12:03:11.000000 bidfx-api-1.1.1/bidfx/pricing/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-05 17:49:42.470267 bidfx-api-1.1.1/bidfx/pricing/_pixie/
--rw-rw-rw-   0        0        0        0 2022-03-09 12:03:11.000000 bidfx-api-1.1.1/bidfx/pricing/_pixie/__init__.py
--rw-rw-rw-   0        0        0       62 2022-03-09 12:03:11.000000 bidfx-api-1.1.1/bidfx/pricing/_pixie/control_operations.py
-drwxrwxrwx   0        0        0        0 2024-01-05 17:49:42.490266 bidfx-api-1.1.1/bidfx/pricing/_pixie/message/
--rw-rw-rw-   0        0        0        0 2022-03-09 12:03:11.000000 bidfx-api-1.1.1/bidfx/pricing/_pixie/message/__init__.py
--rw-rw-rw-   0        0        0     1183 2022-03-09 12:03:11.000000 bidfx-api-1.1.1/bidfx/pricing/_pixie/message/ack_message.py
--rw-rw-rw-   0        0        0     1149 2022-03-09 12:03:11.000000 bidfx-api-1.1.1/bidfx/pricing/_pixie/message/data_dictionary_message.py
--rw-rw-rw-   0        0        0     4023 2022-03-09 12:03:11.000000 bidfx-api-1.1.1/bidfx/pricing/_pixie/message/field_def_message.py
--rw-rw-rw-   0        0        0      543 2022-03-09 12:03:11.000000 bidfx-api-1.1.1/bidfx/pricing/_pixie/message/grant_message.py
--rw-rw-rw-   0        0        0      445 2022-03-09 12:03:11.000000 bidfx-api-1.1.1/bidfx/pricing/_pixie/message/heartbeat_message.py
--rw-rw-rw-   0        0        0     1534 2022-03-09 12:03:11.000000 bidfx-api-1.1.1/bidfx/pricing/_pixie/message/login_message.py
--rw-rw-rw-   0        0        0      244 2022-03-09 12:03:11.000000 bidfx-api-1.1.1/bidfx/pricing/_pixie/message/pixie_message_type.py
--rw-rw-rw-   0        0        0     3587 2024-01-04 18:15:30.000000 bidfx-api-1.1.1/bidfx/pricing/_pixie/message/price_sync_message.py
--rw-rw-rw-   0        0        0     2756 2022-03-09 12:03:11.000000 bidfx-api-1.1.1/bidfx/pricing/_pixie/message/subscription_sync_message.py
--rw-rw-rw-   0        0        0      644 2022-03-09 12:03:11.000000 bidfx-api-1.1.1/bidfx/pricing/_pixie/message/welcome_message.py
--rw-rw-rw-   0        0        0    11049 2024-01-05 17:40:37.000000 bidfx-api-1.1.1/bidfx/pricing/_pixie/pixie_provider.py
--rw-rw-rw-   0        0        0     2860 2022-03-09 12:03:11.000000 bidfx-api-1.1.1/bidfx/pricing/_pixie/subscription_register.py
-drwxrwxrwx   0        0        0        0 2024-01-05 17:49:42.497266 bidfx-api-1.1.1/bidfx/pricing/_pixie/util/
--rw-rw-rw-   0        0        0        0 2022-03-09 12:03:11.000000 bidfx-api-1.1.1/bidfx/pricing/_pixie/util/__init__.py
--rw-rw-rw-   0        0        0     1754 2022-03-09 12:03:11.000000 bidfx-api-1.1.1/bidfx/pricing/_pixie/util/buffer_reads.py
--rw-rw-rw-   0        0        0      525 2022-03-09 12:03:11.000000 bidfx-api-1.1.1/bidfx/pricing/_pixie/util/compression.py
--rw-rw-rw-   0        0        0     2354 2024-01-05 17:40:37.000000 bidfx-api-1.1.1/bidfx/pricing/_pixie/util/varint.py
-drwxrwxrwx   0        0        0        0 2024-01-05 17:49:42.508268 bidfx-api-1.1.1/bidfx/pricing/_puffin/
--rw-rw-rw-   0        0        0        0 2022-03-09 12:03:11.000000 bidfx-api-1.1.1/bidfx/pricing/_puffin/__init__.py
--rw-rw-rw-   0        0        0     3265 2022-03-09 12:03:11.000000 bidfx-api-1.1.1/bidfx/pricing/_puffin/element.py
--rw-rw-rw-   0        0        0     1734 2022-03-09 12:03:11.000000 bidfx-api-1.1.1/bidfx/pricing/_puffin/message_compressor.py
--rw-rw-rw-   0        0        0     4104 2022-03-09 12:03:11.000000 bidfx-api-1.1.1/bidfx/pricing/_puffin/message_decompressor.py
--rw-rw-rw-   0        0        0    12051 2024-01-05 17:40:37.000000 bidfx-api-1.1.1/bidfx/pricing/_puffin/puffin_provider.py
--rw-rw-rw-   0        0        0     6728 2022-03-09 12:03:11.000000 bidfx-api-1.1.1/bidfx/pricing/_puffin/token_dictionary.py
--rw-rw-rw-   0        0        0     3803 2024-01-05 17:40:37.000000 bidfx-api-1.1.1/bidfx/pricing/_service_connector.py
--rw-rw-rw-   0        0        0    14650 2022-03-09 12:03:11.000000 bidfx-api-1.1.1/bidfx/pricing/_subject_builder.py
--rw-rw-rw-   0        0        0      964 2022-03-09 12:03:11.000000 bidfx-api-1.1.1/bidfx/pricing/callbacks.py
--rw-rw-rw-   0        0        0     7903 2022-03-09 12:03:11.000000 bidfx-api-1.1.1/bidfx/pricing/events.py
--rw-rw-rw-   0        0        0     4538 2022-03-09 12:03:11.000000 bidfx-api-1.1.1/bidfx/pricing/field.py
--rw-rw-rw-   0        0        0     5707 2022-03-09 12:03:11.000000 bidfx-api-1.1.1/bidfx/pricing/pricing.py
--rw-rw-rw-   0        0        0     1087 2022-03-09 12:03:11.000000 bidfx-api-1.1.1/bidfx/pricing/provider.py
--rw-rw-rw-   0        0        0     4792 2022-03-09 12:03:11.000000 bidfx-api-1.1.1/bidfx/pricing/subject.py
--rw-rw-rw-   0        0        0     5173 2022-03-09 12:03:11.000000 bidfx-api-1.1.1/bidfx/pricing/tenor.py
--rw-rw-rw-   0        0        0     1659 2022-03-09 12:03:11.000000 bidfx-api-1.1.1/bidfx/session.py
-drwxrwxrwx   0        0        0        0 2024-01-05 17:49:42.566278 bidfx-api-1.1.1/bidfx_api.egg-info/
--rw-rw-rw-   0        0        0     2649 2024-01-05 17:49:42.000000 bidfx-api-1.1.1/bidfx_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2290 2024-01-05 17:49:42.000000 bidfx-api-1.1.1/bidfx_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-05 17:49:42.000000 bidfx-api-1.1.1/bidfx_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2024-01-05 17:49:42.000000 bidfx-api-1.1.1/bidfx_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-01-05 17:49:42.000000 bidfx-api-1.1.1/bidfx_api.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-01-05 17:49:42.540276 bidfx-api-1.1.1/examples/
--rw-rw-rw-   0        0        0     2535 2024-01-05 17:40:37.000000 bidfx-api-1.1.1/examples/config_example.ini
-drwxrwxrwx   0        0        0        0 2024-01-05 17:49:42.562295 bidfx-api-1.1.1/examples/pricing/
--rw-rw-rw-   0        0        0     2563 2024-01-04 09:26:17.000000 bidfx-api-1.1.1/examples/pricing/capstone_demo.py
--rw-rw-rw-   0        0        0     2196 2024-01-05 17:40:37.000000 bidfx-api-1.1.1/examples/pricing/example_fx_spot_and_ndf_quotes.py
--rw-rw-rw-   0        0        0     3259 2024-01-05 15:24:52.000000 bidfx-api-1.1.1/examples/pricing/example_fx_spot_stream.py
--rw-rw-rw-   0        0        0     2170 2022-03-09 12:03:11.000000 bidfx-api-1.1.1/examples/pricing/example_fx_spot_with_random_resubscribe.py
--rw-rw-rw-   0        0        0     1849 2023-11-29 16:24:05.000000 bidfx-api-1.1.1/examples/pricing/example_fx_stream_forwards.py
--rw-rw-rw-   0        0        0     1209 2024-01-05 12:26:45.000000 bidfx-api-1.1.1/examples/pricing/example_indicative_fx.py
--rw-rw-rw-   0        0        0     2274 2022-03-09 12:03:11.000000 bidfx-api-1.1.1/examples/pricing/example_indicative_fx_and_equity_depth.py
--rw-rw-rw-   0        0        0     1758 2022-03-09 12:03:11.000000 bidfx-api-1.1.1/examples/pricing/example_indicative_fx_with_unsubscribe.py
--rw-rw-rw-   0        0        0      579 2024-01-05 17:40:37.000000 bidfx-api-1.1.1/examples/pricing/example_minimal.py
--rw-rw-rw-   0        0        0     2335 2022-03-09 12:03:11.000000 bidfx-api-1.1.1/examples/pricing/example_mixed_streaming_and_indicative_spot.py
--rw-rw-rw-   0        0        0     2136 2022-03-09 12:03:11.000000 bidfx-api-1.1.1/examples/pricing/example_stream_fx_spot_and_ndf.py
--rw-rw-rw-   0        0        0      881 2022-03-09 12:03:11.000000 bidfx-api-1.1.1/requirements-dev.txt
--rw-rw-rw-   0        0        0       20 2022-03-09 12:03:11.000000 bidfx-api-1.1.1/requirements.txt
--rw-rw-rw-   0        0        0      443 2024-01-05 17:49:42.574276 bidfx-api-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1314 2024-01-05 17:36:56.000000 bidfx-api-1.1.1/setup.py
+drwxrwxrwx   0 mihber    (1000) mihber    (1000)        0 2024-05-08 11:33:58.550162 bidfx-api-1.1.2/
+-rwxrwxrwx   0 mihber    (1000) mihber    (1000)     4627 2024-03-28 12:47:47.000000 bidfx-api-1.1.2/DEVELOPMENT.md
+-rwxrwxrwx   0 mihber    (1000) mihber    (1000)    11357 2024-03-28 12:47:47.000000 bidfx-api-1.1.2/LICENSE-2.0.txt
+-rwxrwxrwx   0 mihber    (1000) mihber    (1000)      165 2024-03-28 12:47:47.000000 bidfx-api-1.1.2/MANIFEST.in
+-rwxrwxrwx   0 mihber    (1000) mihber    (1000)     2560 2024-05-08 11:33:58.550162 bidfx-api-1.1.2/PKG-INFO
+-rwxrwxrwx   0 mihber    (1000) mihber    (1000)     1692 2024-03-28 12:47:47.000000 bidfx-api-1.1.2/README.md
+drwxrwxrwx   0 mihber    (1000) mihber    (1000)        0 2024-05-08 11:33:57.663391 bidfx-api-1.1.2/bidfx/
+-rwxrwxrwx   0 mihber    (1000) mihber    (1000)      160 2024-05-08 11:21:50.000000 bidfx-api-1.1.2/bidfx/__init__.py
+-rwxrwxrwx   0 mihber    (1000) mihber    (1000)      776 2024-05-08 11:21:50.000000 bidfx-api-1.1.2/bidfx/_bidfx_api.py
+-rwxrwxrwx   0 mihber    (1000) mihber    (1000)      718 2024-03-28 12:47:47.000000 bidfx-api-1.1.2/bidfx/exceptions.py
+drwxrwxrwx   0 mihber    (1000) mihber    (1000)        0 2024-05-08 11:33:57.785797 bidfx-api-1.1.2/bidfx/pricing/
+-rwxrwxrwx   0 mihber    (1000) mihber    (1000)      530 2024-03-28 12:47:47.000000 bidfx-api-1.1.2/bidfx/pricing/__init__.py
+drwxrwxrwx   0 mihber    (1000) mihber    (1000)        0 2024-05-08 11:33:57.848296 bidfx-api-1.1.2/bidfx/pricing/_pixie/
+-rwxrwxrwx   0 mihber    (1000) mihber    (1000)        0 2024-03-28 12:47:47.000000 bidfx-api-1.1.2/bidfx/pricing/_pixie/__init__.py
+-rwxrwxrwx   0 mihber    (1000) mihber    (1000)       62 2024-03-28 12:47:47.000000 bidfx-api-1.1.2/bidfx/pricing/_pixie/control_operations.py
+drwxrwxrwx   0 mihber    (1000) mihber    (1000)        0 2024-05-08 11:33:58.086583 bidfx-api-1.1.2/bidfx/pricing/_pixie/message/
+-rwxrwxrwx   0 mihber    (1000) mihber    (1000)        0 2024-03-28 12:47:47.000000 bidfx-api-1.1.2/bidfx/pricing/_pixie/message/__init__.py
+-rwxrwxrwx   0 mihber    (1000) mihber    (1000)     1183 2024-03-28 12:47:47.000000 bidfx-api-1.1.2/bidfx/pricing/_pixie/message/ack_message.py
+-rwxrwxrwx   0 mihber    (1000) mihber    (1000)     1149 2024-03-28 12:47:47.000000 bidfx-api-1.1.2/bidfx/pricing/_pixie/message/data_dictionary_message.py
+-rwxrwxrwx   0 mihber    (1000) mihber    (1000)     4023 2024-03-28 12:47:47.000000 bidfx-api-1.1.2/bidfx/pricing/_pixie/message/field_def_message.py
+-rwxrwxrwx   0 mihber    (1000) mihber    (1000)      543 2024-03-28 12:47:47.000000 bidfx-api-1.1.2/bidfx/pricing/_pixie/message/grant_message.py
+-rwxrwxrwx   0 mihber    (1000) mihber    (1000)      445 2024-03-28 12:47:47.000000 bidfx-api-1.1.2/bidfx/pricing/_pixie/message/heartbeat_message.py
+-rwxrwxrwx   0 mihber    (1000) mihber    (1000)     1534 2024-03-28 12:47:47.000000 bidfx-api-1.1.2/bidfx/pricing/_pixie/message/login_message.py
+-rwxrwxrwx   0 mihber    (1000) mihber    (1000)      244 2024-03-28 12:47:47.000000 bidfx-api-1.1.2/bidfx/pricing/_pixie/message/pixie_message_type.py
+-rwxrwxrwx   0 mihber    (1000) mihber    (1000)     3587 2024-03-28 12:47:47.000000 bidfx-api-1.1.2/bidfx/pricing/_pixie/message/price_sync_message.py
+-rwxrwxrwx   0 mihber    (1000) mihber    (1000)     2756 2024-03-28 12:47:47.000000 bidfx-api-1.1.2/bidfx/pricing/_pixie/message/subscription_sync_message.py
+-rwxrwxrwx   0 mihber    (1000) mihber    (1000)      644 2024-03-28 12:47:47.000000 bidfx-api-1.1.2/bidfx/pricing/_pixie/message/welcome_message.py
+-rwxrwxrwx   0 mihber    (1000) mihber    (1000)    11049 2024-03-28 12:47:47.000000 bidfx-api-1.1.2/bidfx/pricing/_pixie/pixie_provider.py
+-rwxrwxrwx   0 mihber    (1000) mihber    (1000)     2860 2024-03-28 12:47:47.000000 bidfx-api-1.1.2/bidfx/pricing/_pixie/subscription_register.py
+drwxrwxrwx   0 mihber    (1000) mihber    (1000)        0 2024-05-08 11:33:58.186847 bidfx-api-1.1.2/bidfx/pricing/_pixie/util/
+-rwxrwxrwx   0 mihber    (1000) mihber    (1000)        0 2024-03-28 12:47:47.000000 bidfx-api-1.1.2/bidfx/pricing/_pixie/util/__init__.py
+-rwxrwxrwx   0 mihber    (1000) mihber    (1000)     1754 2024-03-28 12:47:47.000000 bidfx-api-1.1.2/bidfx/pricing/_pixie/util/buffer_reads.py
+-rwxrwxrwx   0 mihber    (1000) mihber    (1000)      525 2024-03-28 12:47:47.000000 bidfx-api-1.1.2/bidfx/pricing/_pixie/util/compression.py
+-rwxrwxrwx   0 mihber    (1000) mihber    (1000)     2346 2024-05-08 11:29:30.000000 bidfx-api-1.1.2/bidfx/pricing/_pixie/util/varint.py
+drwxrwxrwx   0 mihber    (1000) mihber    (1000)        0 2024-05-08 11:33:58.287112 bidfx-api-1.1.2/bidfx/pricing/_puffin/
+-rwxrwxrwx   0 mihber    (1000) mihber    (1000)        0 2024-03-28 12:47:47.000000 bidfx-api-1.1.2/bidfx/pricing/_puffin/__init__.py
+-rwxrwxrwx   0 mihber    (1000) mihber    (1000)     3265 2024-03-28 12:47:47.000000 bidfx-api-1.1.2/bidfx/pricing/_puffin/element.py
+-rwxrwxrwx   0 mihber    (1000) mihber    (1000)     1734 2024-03-28 12:47:47.000000 bidfx-api-1.1.2/bidfx/pricing/_puffin/message_compressor.py
+-rwxrwxrwx   0 mihber    (1000) mihber    (1000)     4104 2024-03-28 12:47:47.000000 bidfx-api-1.1.2/bidfx/pricing/_puffin/message_decompressor.py
+-rwxrwxrwx   0 mihber    (1000) mihber    (1000)    12064 2024-05-08 11:20:47.000000 bidfx-api-1.1.2/bidfx/pricing/_puffin/puffin_provider.py
+-rwxrwxrwx   0 mihber    (1000) mihber    (1000)     6728 2024-03-28 12:47:47.000000 bidfx-api-1.1.2/bidfx/pricing/_puffin/token_dictionary.py
+-rwxrwxrwx   0 mihber    (1000) mihber    (1000)     3803 2024-03-28 12:47:47.000000 bidfx-api-1.1.2/bidfx/pricing/_service_connector.py
+-rwxrwxrwx   0 mihber    (1000) mihber    (1000)    14650 2024-03-28 12:47:47.000000 bidfx-api-1.1.2/bidfx/pricing/_subject_builder.py
+-rwxrwxrwx   0 mihber    (1000) mihber    (1000)      964 2024-03-28 12:47:47.000000 bidfx-api-1.1.2/bidfx/pricing/callbacks.py
+-rwxrwxrwx   0 mihber    (1000) mihber    (1000)     7903 2024-03-28 12:47:47.000000 bidfx-api-1.1.2/bidfx/pricing/events.py
+-rwxrwxrwx   0 mihber    (1000) mihber    (1000)     4538 2024-03-28 12:47:47.000000 bidfx-api-1.1.2/bidfx/pricing/field.py
+-rwxrwxrwx   0 mihber    (1000) mihber    (1000)     5707 2024-03-28 12:47:47.000000 bidfx-api-1.1.2/bidfx/pricing/pricing.py
+-rwxrwxrwx   0 mihber    (1000) mihber    (1000)     1087 2024-03-28 12:47:47.000000 bidfx-api-1.1.2/bidfx/pricing/provider.py
+-rwxrwxrwx   0 mihber    (1000) mihber    (1000)     4792 2024-03-28 12:47:47.000000 bidfx-api-1.1.2/bidfx/pricing/subject.py
+-rwxrwxrwx   0 mihber    (1000) mihber    (1000)     5173 2024-03-28 12:47:47.000000 bidfx-api-1.1.2/bidfx/pricing/tenor.py
+-rwxrwxrwx   0 mihber    (1000) mihber    (1000)     1659 2024-03-28 12:47:47.000000 bidfx-api-1.1.2/bidfx/session.py
+drwxrwxrwx   0 mihber    (1000) mihber    (1000)        0 2024-05-08 11:33:58.349612 bidfx-api-1.1.2/bidfx_api.egg-info/
+-rwxrwxrwx   0 mihber    (1000) mihber    (1000)     2560 2024-05-08 11:33:57.000000 bidfx-api-1.1.2/bidfx_api.egg-info/PKG-INFO
+-rwxrwxrwx   0 mihber    (1000) mihber    (1000)     2256 2024-05-08 11:33:57.000000 bidfx-api-1.1.2/bidfx_api.egg-info/SOURCES.txt
+-rwxrwxrwx   0 mihber    (1000) mihber    (1000)        1 2024-05-08 11:33:57.000000 bidfx-api-1.1.2/bidfx_api.egg-info/dependency_links.txt
+-rwxrwxrwx   0 mihber    (1000) mihber    (1000)       21 2024-05-08 11:33:57.000000 bidfx-api-1.1.2/bidfx_api.egg-info/requires.txt
+-rwxrwxrwx   0 mihber    (1000) mihber    (1000)       12 2024-05-08 11:33:57.000000 bidfx-api-1.1.2/bidfx_api.egg-info/top_level.txt
+drwxrwxrwx   0 mihber    (1000) mihber    (1000)        0 2024-05-08 11:33:58.365243 bidfx-api-1.1.2/examples/
+-rwxrwxrwx   0 mihber    (1000) mihber    (1000)     2535 2024-03-28 12:47:47.000000 bidfx-api-1.1.2/examples/config_example.ini
+drwxrwxrwx   0 mihber    (1000) mihber    (1000)        0 2024-05-08 11:33:58.534538 bidfx-api-1.1.2/examples/pricing/
+-rwxrwxrwx   0 mihber    (1000) mihber    (1000)     2196 2024-03-28 12:47:47.000000 bidfx-api-1.1.2/examples/pricing/example_fx_spot_and_ndf_quotes.py
+-rwxrwxrwx   0 mihber    (1000) mihber    (1000)     1634 2024-05-08 11:11:35.000000 bidfx-api-1.1.2/examples/pricing/example_fx_spot_stream.py
+-rwxrwxrwx   0 mihber    (1000) mihber    (1000)     2171 2024-05-08 11:11:39.000000 bidfx-api-1.1.2/examples/pricing/example_fx_spot_with_random_resubscribe.py
+-rwxrwxrwx   0 mihber    (1000) mihber    (1000)     1849 2024-03-28 12:47:47.000000 bidfx-api-1.1.2/examples/pricing/example_fx_stream_forwards.py
+-rwxrwxrwx   0 mihber    (1000) mihber    (1000)     1209 2024-03-28 12:47:47.000000 bidfx-api-1.1.2/examples/pricing/example_indicative_fx.py
+-rwxrwxrwx   0 mihber    (1000) mihber    (1000)     2274 2024-03-28 12:47:47.000000 bidfx-api-1.1.2/examples/pricing/example_indicative_fx_and_equity_depth.py
+-rwxrwxrwx   0 mihber    (1000) mihber    (1000)     1758 2024-03-28 12:47:47.000000 bidfx-api-1.1.2/examples/pricing/example_indicative_fx_with_unsubscribe.py
+-rwxrwxrwx   0 mihber    (1000) mihber    (1000)      579 2024-03-28 12:47:47.000000 bidfx-api-1.1.2/examples/pricing/example_minimal.py
+-rwxrwxrwx   0 mihber    (1000) mihber    (1000)     2335 2024-03-28 12:47:47.000000 bidfx-api-1.1.2/examples/pricing/example_mixed_streaming_and_indicative_spot.py
+-rwxrwxrwx   0 mihber    (1000) mihber    (1000)     2136 2024-03-28 12:47:47.000000 bidfx-api-1.1.2/examples/pricing/example_stream_fx_spot_and_ndf.py
+-rwxrwxrwx   0 mihber    (1000) mihber    (1000)      881 2024-03-28 15:29:28.000000 bidfx-api-1.1.2/requirements-dev.txt
+-rwxrwxrwx   0 mihber    (1000) mihber    (1000)       20 2024-03-28 12:47:47.000000 bidfx-api-1.1.2/requirements.txt
+-rwxrwxrwx   0 mihber    (1000) mihber    (1000)      420 2024-05-08 11:33:58.550162 bidfx-api-1.1.2/setup.cfg
+-rwxrwxrwx   0 mihber    (1000) mihber    (1000)     1314 2024-05-08 11:21:51.000000 bidfx-api-1.1.2/setup.py
```

### Comparing `bidfx-api-1.1.1/DEVELOPMENT.md` & `bidfx-api-1.1.2/DEVELOPMENT.md`

 * *Files identical despite different names*

### Comparing `bidfx-api-1.1.1/LICENSE-2.0.txt` & `bidfx-api-1.1.2/LICENSE-2.0.txt`

 * *Files identical despite different names*

### Comparing `bidfx-api-1.1.1/PKG-INFO` & `bidfx-api-1.1.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,68 +1,70 @@
-Metadata-Version: 2.1
-Name: bidfx-api
-Version: 1.1.1
-Summary: Public API for accessing the BidFX platform for pricing
-Home-page: https://github.com/bidfx/bidfx-api-py
-Download-URL: https://github.com/bidfx/bidfx-api-py/tarball/v1.1.1
-Author: Paul Sweeny
-Author-email: paul.sweeny@bidfx.com
-License: Apache License 2.0
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Classifier: Intended Audience :: Financial and Insurance Industry
-Classifier: Topic :: Office/Business :: Financial :: Investment
-Classifier: Natural Language :: English
-Classifier: Development Status :: 5 - Production/Stable
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE-2.0.txt
-Requires-Dist: pycryptodomex==3.9.4
-
-# BidFX Public API for Python
-
-[![Release](https://img.shields.io/pypi/v/bidfx-api)](https://pypi.org/project/bidfx-api)
-[![Status](https://img.shields.io/pypi/status/bidfx-api)](https://pypi.org/project/bidfx-api)
-[![Source Release](https://img.shields.io/github/v/release/bidfx/bidfx-api-py?sort=semver)](https://github.com/bidfx/bidfx-api-py)
-[![License](https://img.shields.io/badge/license-Apache%202-4EB1BA.svg)](https://www.apache.org/licenses/LICENSE-2.0.html)
-[![Docs](https://img.shields.io/badge/docs-docs.bidfx.com-green)](https://docs.bidfx.com/api-py/index.html)
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-
-![BidFX-API-Python](https://user-images.githubusercontent.com/2197551/76171801-35d74100-6187-11ea-8cc5-7f29b66d00ea.png)
-
--------
-
-
-A *pricing* API that connects to the BidFX trading platform 
-to subscribe to realtime FX pricing. The API supports:
-
- - FX request for stream (RFS) pricing
- - FX request for quote (RFQ) pricing
-
-
-## Quick start
-
-### Installation
-
-```sh
-pip install bidfx-api
-```
-
-### API docs
-
-Read the documentation [here](https://docs.bidfx.com/api-py/index.html).
-
-
-## Python version
-
-The API is compatible with Python 3.6 and greater.
-If you do not have Python, please install the latest 3.x version from [python.org](https://python.org) 
-or refer to the [Installing Python](http://docs.python-guide.org/en/latest/starting/installation/) section 
-of the Hitchhikerâ€™s Guide to Python.
-
-
-## Alternative APIs
-
-If you prefer not to code in Python, you can read about the complete BidFX API range, and their different capabilities,
-at [BidFX API Overview](https://www.bidfx.com/apis).
+Metadata-Version: 2.1
+Name: bidfx-api
+Version: 1.1.2
+Summary: Public API for accessing the BidFX platform for pricing
+Home-page: https://github.com/bidfx/bidfx-api-py
+Author: Paul Sweeny
+Author-email: paul.sweeny@bidfx.com
+License: Apache License 2.0
+Download-URL: https://github.com/bidfx/bidfx-api-py/tarball/v1.1.2
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Classifier: Intended Audience :: Financial and Insurance Industry
+Classifier: Topic :: Office/Business :: Financial :: Investment
+Classifier: Natural Language :: English
+Classifier: Development Status :: 5 - Production/Stable
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE-2.0.txt
+
+# BidFX Public API for Python
+
+[![Release](https://img.shields.io/pypi/v/bidfx-api)](https://pypi.org/project/bidfx-api)
+[![Status](https://img.shields.io/pypi/status/bidfx-api)](https://pypi.org/project/bidfx-api)
+[![Source Release](https://img.shields.io/github/v/release/bidfx/bidfx-api-py?sort=semver)](https://github.com/bidfx/bidfx-api-py)
+[![License](https://img.shields.io/badge/license-Apache%202-4EB1BA.svg)](https://www.apache.org/licenses/LICENSE-2.0.html)
+[![Docs](https://img.shields.io/badge/docs-docs.bidfx.com-green)](https://docs.bidfx.com/api-py/index.html)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+
+![BidFX-API-Python](https://user-images.githubusercontent.com/2197551/76171801-35d74100-6187-11ea-8cc5-7f29b66d00ea.png)
+
+-------
+
+
+A *pricing* API that connects to the BidFX trading platform 
+to subscribe to realtime FX pricing. The API supports:
+
+ - FX request for stream (RFS) pricing
+ - FX request for quote (RFQ) pricing
+
+
+## Quick start
+
+### Installation
+
+```sh
+pip install bidfx-api
+```
+
+### API docs
+
+Read the documentation [here](https://docs.bidfx.com/api-py/index.html).
+
+
+## Python version
+
+The API is compatible with Python 3.6 and greater.
+If you do not have Python, please install the latest 3.x version from [python.org](https://python.org) 
+or refer to the [Installing Python](http://docs.python-guide.org/en/latest/starting/installation/) section 
+of the Hitchhiker’s Guide to Python.
+
+
+## Alternative APIs
+
+If you prefer not to code in Python, you can read about the complete BidFX API range, and their different capabilities,
+at [BidFX API Overview](https://www.bidfx.com/apis).
+
+
```

### Comparing `bidfx-api-1.1.1/README.md` & `bidfx-api-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `bidfx-api-1.1.1/bidfx/_bidfx_api.py` & `bidfx-api-1.1.2/bidfx/_bidfx_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 class _BidFxAPI:
     """
     This class provides the identifying information for the BidFX Python API including its version.
     """
 
-    def __init__(self, version="1.1.1"):
+    def __init__(self, version="1.1.2"):
         self._name = "bidfx-public-api-py"
         self._product = "BidFXPython"
         self._version = version
         self._guid = uuid.uuid4().hex
 
     @property
     def name(self):
```

### Comparing `bidfx-api-1.1.1/bidfx/exceptions.py` & `bidfx-api-1.1.2/bidfx/exceptions.py`

 * *Files identical despite different names*

### Comparing `bidfx-api-1.1.1/bidfx/pricing/__init__.py` & `bidfx-api-1.1.2/bidfx/pricing/__init__.py`

 * *Files identical despite different names*

### Comparing `bidfx-api-1.1.1/bidfx/pricing/_pixie/message/ack_message.py` & `bidfx-api-1.1.2/bidfx/pricing/_pixie/message/ack_message.py`

 * *Files identical despite different names*

### Comparing `bidfx-api-1.1.1/bidfx/pricing/_pixie/message/data_dictionary_message.py` & `bidfx-api-1.1.2/bidfx/pricing/_pixie/message/data_dictionary_message.py`

 * *Files identical despite different names*

### Comparing `bidfx-api-1.1.1/bidfx/pricing/_pixie/message/field_def_message.py` & `bidfx-api-1.1.2/bidfx/pricing/_pixie/message/field_def_message.py`

 * *Files identical despite different names*

### Comparing `bidfx-api-1.1.1/bidfx/pricing/_pixie/message/grant_message.py` & `bidfx-api-1.1.2/bidfx/pricing/_pixie/message/grant_message.py`

 * *Files identical despite different names*

### Comparing `bidfx-api-1.1.1/bidfx/pricing/_pixie/message/login_message.py` & `bidfx-api-1.1.2/bidfx/pricing/_pixie/message/login_message.py`

 * *Files identical despite different names*

### Comparing `bidfx-api-1.1.1/bidfx/pricing/_pixie/message/price_sync_message.py` & `bidfx-api-1.1.2/bidfx/pricing/_pixie/message/price_sync_message.py`

 * *Files identical despite different names*

### Comparing `bidfx-api-1.1.1/bidfx/pricing/_pixie/message/subscription_sync_message.py` & `bidfx-api-1.1.2/bidfx/pricing/_pixie/message/subscription_sync_message.py`

 * *Files identical despite different names*

### Comparing `bidfx-api-1.1.1/bidfx/pricing/_pixie/message/welcome_message.py` & `bidfx-api-1.1.2/bidfx/pricing/_pixie/message/welcome_message.py`

 * *Files identical despite different names*

### Comparing `bidfx-api-1.1.1/bidfx/pricing/_pixie/pixie_provider.py` & `bidfx-api-1.1.2/bidfx/pricing/_pixie/pixie_provider.py`

 * *Files identical despite different names*

### Comparing `bidfx-api-1.1.1/bidfx/pricing/_pixie/subscription_register.py` & `bidfx-api-1.1.2/bidfx/pricing/_pixie/subscription_register.py`

 * *Files identical despite different names*

### Comparing `bidfx-api-1.1.1/bidfx/pricing/_pixie/util/buffer_reads.py` & `bidfx-api-1.1.2/bidfx/pricing/_pixie/util/buffer_reads.py`

 * *Files identical despite different names*

### Comparing `bidfx-api-1.1.1/bidfx/pricing/_pixie/util/compression.py` & `bidfx-api-1.1.2/bidfx/pricing/_pixie/util/compression.py`

 * *Files identical despite different names*

### Comparing `bidfx-api-1.1.1/bidfx/pricing/_pixie/util/varint.py` & `bidfx-api-1.1.2/bidfx/pricing/_pixie/util/varint.py`

 * *Files 0% similar despite different names*

```diff
@@ -99,9 +99,9 @@
     result = b""
 
     while len(result) != length:
         byte_ = socket_connection.recv(length - len(result))
         if byte_ == b"":
             raise socket.error("end of socket stream")
         result += byte_
-        
+
     return result
```

### Comparing `bidfx-api-1.1.1/bidfx/pricing/_puffin/element.py` & `bidfx-api-1.1.2/bidfx/pricing/_puffin/element.py`

 * *Files identical despite different names*

### Comparing `bidfx-api-1.1.1/bidfx/pricing/_puffin/message_compressor.py` & `bidfx-api-1.1.2/bidfx/pricing/_puffin/message_compressor.py`

 * *Files identical despite different names*

### Comparing `bidfx-api-1.1.1/bidfx/pricing/_puffin/message_decompressor.py` & `bidfx-api-1.1.2/bidfx/pricing/_puffin/message_decompressor.py`

 * *Files identical despite different names*

### Comparing `bidfx-api-1.1.1/bidfx/pricing/_puffin/puffin_provider.py` & `bidfx-api-1.1.2/bidfx/pricing/_puffin/puffin_provider.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __all__ = ["PuffinProvider"]
 
+import getpass
 import logging
-import os
 import threading
 import time
 from base64 import b64decode, b64encode
 
 from Cryptodome.Cipher import PKCS1_v1_5
 from Cryptodome.PublicKey import RSA
 
@@ -233,15 +233,15 @@
             password = self._encrypted_password(public_key, password).decode("ascii")
         login_message = (
             Element("Login")
             .set("Name", self._username)
             .set("Password", password)
             .set("Version", str(8))
             .set("Description", description)
-            .set("Alias", None or os.getlogin())
+            .set("Alias", None or getpass.getuser())
         )
         self._send_message(login_message, compress=False)
 
     @staticmethod
     def _encrypted_password(public_key, password):
         try:
             raw_key = b64decode(public_key)
@@ -272,15 +272,15 @@
         service_description_msg = parser.parse_element()
         log.debug(f"Puffin sent message: {service_description_msg}")
 
         if grant_msg["Access"] == "true":
             message = (
                 Element("ServiceDescription")
                 .set("username", self._username)
-                .set("alias", os.getlogin())
+                .set("alias", getpass.getuser())
                 .set("server", "false")
                 .set("discoverable", "false")
             )
             self._send_message(message, compress=False)
         else:
             raise PricingError(
                 f"login to {self._provider_name} rejected due to {grant_msg.text}"
```

### Comparing `bidfx-api-1.1.1/bidfx/pricing/_puffin/token_dictionary.py` & `bidfx-api-1.1.2/bidfx/pricing/_puffin/token_dictionary.py`

 * *Files identical despite different names*

### Comparing `bidfx-api-1.1.1/bidfx/pricing/_service_connector.py` & `bidfx-api-1.1.2/bidfx/pricing/_service_connector.py`

 * *Files identical despite different names*

### Comparing `bidfx-api-1.1.1/bidfx/pricing/_subject_builder.py` & `bidfx-api-1.1.2/bidfx/pricing/_subject_builder.py`

 * *Files identical despite different names*

### Comparing `bidfx-api-1.1.1/bidfx/pricing/callbacks.py` & `bidfx-api-1.1.2/bidfx/pricing/callbacks.py`

 * *Files identical despite different names*

### Comparing `bidfx-api-1.1.1/bidfx/pricing/events.py` & `bidfx-api-1.1.2/bidfx/pricing/events.py`

 * *Files identical despite different names*

### Comparing `bidfx-api-1.1.1/bidfx/pricing/field.py` & `bidfx-api-1.1.2/bidfx/pricing/field.py`

 * *Files identical despite different names*

### Comparing `bidfx-api-1.1.1/bidfx/pricing/pricing.py` & `bidfx-api-1.1.2/bidfx/pricing/pricing.py`

 * *Files identical despite different names*

### Comparing `bidfx-api-1.1.1/bidfx/pricing/provider.py` & `bidfx-api-1.1.2/bidfx/pricing/provider.py`

 * *Files identical despite different names*

### Comparing `bidfx-api-1.1.1/bidfx/pricing/subject.py` & `bidfx-api-1.1.2/bidfx/pricing/subject.py`

 * *Files identical despite different names*

### Comparing `bidfx-api-1.1.1/bidfx/pricing/tenor.py` & `bidfx-api-1.1.2/bidfx/pricing/tenor.py`

 * *Files identical despite different names*

### Comparing `bidfx-api-1.1.1/bidfx/session.py` & `bidfx-api-1.1.2/bidfx/session.py`

 * *Files identical despite different names*

### Comparing `bidfx-api-1.1.1/bidfx_api.egg-info/PKG-INFO` & `bidfx-api-1.1.2/bidfx_api.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,68 +1,70 @@
-Metadata-Version: 2.1
-Name: bidfx-api
-Version: 1.1.1
-Summary: Public API for accessing the BidFX platform for pricing
-Home-page: https://github.com/bidfx/bidfx-api-py
-Download-URL: https://github.com/bidfx/bidfx-api-py/tarball/v1.1.1
-Author: Paul Sweeny
-Author-email: paul.sweeny@bidfx.com
-License: Apache License 2.0
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Classifier: Intended Audience :: Financial and Insurance Industry
-Classifier: Topic :: Office/Business :: Financial :: Investment
-Classifier: Natural Language :: English
-Classifier: Development Status :: 5 - Production/Stable
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE-2.0.txt
-Requires-Dist: pycryptodomex==3.9.4
-
-# BidFX Public API for Python
-
-[![Release](https://img.shields.io/pypi/v/bidfx-api)](https://pypi.org/project/bidfx-api)
-[![Status](https://img.shields.io/pypi/status/bidfx-api)](https://pypi.org/project/bidfx-api)
-[![Source Release](https://img.shields.io/github/v/release/bidfx/bidfx-api-py?sort=semver)](https://github.com/bidfx/bidfx-api-py)
-[![License](https://img.shields.io/badge/license-Apache%202-4EB1BA.svg)](https://www.apache.org/licenses/LICENSE-2.0.html)
-[![Docs](https://img.shields.io/badge/docs-docs.bidfx.com-green)](https://docs.bidfx.com/api-py/index.html)
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-
-![BidFX-API-Python](https://user-images.githubusercontent.com/2197551/76171801-35d74100-6187-11ea-8cc5-7f29b66d00ea.png)
-
--------
-
-
-A *pricing* API that connects to the BidFX trading platform 
-to subscribe to realtime FX pricing. The API supports:
-
- - FX request for stream (RFS) pricing
- - FX request for quote (RFQ) pricing
-
-
-## Quick start
-
-### Installation
-
-```sh
-pip install bidfx-api
-```
-
-### API docs
-
-Read the documentation [here](https://docs.bidfx.com/api-py/index.html).
-
-
-## Python version
-
-The API is compatible with Python 3.6 and greater.
-If you do not have Python, please install the latest 3.x version from [python.org](https://python.org) 
-or refer to the [Installing Python](http://docs.python-guide.org/en/latest/starting/installation/) section 
-of the Hitchhikerâ€™s Guide to Python.
-
-
-## Alternative APIs
-
-If you prefer not to code in Python, you can read about the complete BidFX API range, and their different capabilities,
-at [BidFX API Overview](https://www.bidfx.com/apis).
+Metadata-Version: 2.1
+Name: bidfx-api
+Version: 1.1.2
+Summary: Public API for accessing the BidFX platform for pricing
+Home-page: https://github.com/bidfx/bidfx-api-py
+Author: Paul Sweeny
+Author-email: paul.sweeny@bidfx.com
+License: Apache License 2.0
+Download-URL: https://github.com/bidfx/bidfx-api-py/tarball/v1.1.2
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Classifier: Intended Audience :: Financial and Insurance Industry
+Classifier: Topic :: Office/Business :: Financial :: Investment
+Classifier: Natural Language :: English
+Classifier: Development Status :: 5 - Production/Stable
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE-2.0.txt
+
+# BidFX Public API for Python
+
+[![Release](https://img.shields.io/pypi/v/bidfx-api)](https://pypi.org/project/bidfx-api)
+[![Status](https://img.shields.io/pypi/status/bidfx-api)](https://pypi.org/project/bidfx-api)
+[![Source Release](https://img.shields.io/github/v/release/bidfx/bidfx-api-py?sort=semver)](https://github.com/bidfx/bidfx-api-py)
+[![License](https://img.shields.io/badge/license-Apache%202-4EB1BA.svg)](https://www.apache.org/licenses/LICENSE-2.0.html)
+[![Docs](https://img.shields.io/badge/docs-docs.bidfx.com-green)](https://docs.bidfx.com/api-py/index.html)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+
+![BidFX-API-Python](https://user-images.githubusercontent.com/2197551/76171801-35d74100-6187-11ea-8cc5-7f29b66d00ea.png)
+
+-------
+
+
+A *pricing* API that connects to the BidFX trading platform 
+to subscribe to realtime FX pricing. The API supports:
+
+ - FX request for stream (RFS) pricing
+ - FX request for quote (RFQ) pricing
+
+
+## Quick start
+
+### Installation
+
+```sh
+pip install bidfx-api
+```
+
+### API docs
+
+Read the documentation [here](https://docs.bidfx.com/api-py/index.html).
+
+
+## Python version
+
+The API is compatible with Python 3.6 and greater.
+If you do not have Python, please install the latest 3.x version from [python.org](https://python.org) 
+or refer to the [Installing Python](http://docs.python-guide.org/en/latest/starting/installation/) section 
+of the Hitchhiker’s Guide to Python.
+
+
+## Alternative APIs
+
+If you prefer not to code in Python, you can read about the complete BidFX API range, and their different capabilities,
+at [BidFX API Overview](https://www.bidfx.com/apis).
+
+
```

### Comparing `bidfx-api-1.1.1/bidfx_api.egg-info/SOURCES.txt` & `bidfx-api-1.1.2/bidfx_api.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -47,15 +47,14 @@
 bidfx/pricing/_puffin/token_dictionary.py
 bidfx_api.egg-info/PKG-INFO
 bidfx_api.egg-info/SOURCES.txt
 bidfx_api.egg-info/dependency_links.txt
 bidfx_api.egg-info/requires.txt
 bidfx_api.egg-info/top_level.txt
 examples/config_example.ini
-examples/pricing/capstone_demo.py
 examples/pricing/example_fx_spot_and_ndf_quotes.py
 examples/pricing/example_fx_spot_stream.py
 examples/pricing/example_fx_spot_with_random_resubscribe.py
 examples/pricing/example_fx_stream_forwards.py
 examples/pricing/example_indicative_fx.py
 examples/pricing/example_indicative_fx_and_equity_depth.py
 examples/pricing/example_indicative_fx_with_unsubscribe.py
```

### Comparing `bidfx-api-1.1.1/examples/config_example.ini` & `bidfx-api-1.1.2/examples/config_example.ini`

 * *Files identical despite different names*

### Comparing `bidfx-api-1.1.1/examples/pricing/example_fx_spot_and_ndf_quotes.py` & `bidfx-api-1.1.2/examples/pricing/example_fx_spot_and_ndf_quotes.py`

 * *Files identical despite different names*

### Comparing `bidfx-api-1.1.1/examples/pricing/example_fx_spot_stream.py` & `bidfx-api-1.1.2/examples/pricing/example_fx_spot_stream.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,101 +1,68 @@
 #!/usr/bin/env python
 
 import logging
 from time import sleep
 
 from bidfx import Session, Subject
-from bidfx.pricing.tenor import Tenor
 
 """
 Example of streaming (RFS) firm spot rates direct from LPs.
 """
 
+
 def on_price_event(event):
     if event.price:
-        logging.info(
+        print(
             "{} {} {} {} {} -> {}".format(
                 event.subject[Subject.CURRENCY_PAIR],
                 event.subject[Subject.LIQUIDITY_PROVIDER],
                 event.subject[Subject.DEAL_TYPE],
                 event.subject[Subject.CURRENCY],
                 event.subject[Subject.QUANTITY],
                 event.price,
             )
         )
 
+
 def on_subscription_event(event):
-    logging.info(f"Subscription to {event}")
+    print(f"Subscription to {event}")
+
 
 def on_provider_event(event):
-    logging.info(f"Provider {event}")
+    print(f"Provider {event}")
+
 
 def main():
     logging.basicConfig(
         level=logging.INFO,
         format="%(asctime)s %(levelname)-7s %(threadName)-12s %(message)s",
-#       filename="api.log",
     )
-
-    session = Session.create_from_ini_file("~/.bidfx/api/config_DEV.ini")
+    session = Session.create_from_ini_file()
     pricing = session.pricing
     pricing.callbacks.price_event_fn = on_price_event
     pricing.callbacks.subscription_event_fn = on_subscription_event
     pricing.callbacks.provider_event_fn = on_provider_event
     pricing.start()
 
-    xtx_pairs = ["EURUSD", "AUDUSD", "EURCHF", "EURGBP", "EURJPY", "EURNOK", "EURPLN", "EURSEK", "GBPUSD"]#"NOKSEK", "USDCAD", "USDCHF", "USDJPY", "USDMXN", "USDRUB", "USDTRY", "USDZAR"]
-    tenors = [Tenor.IN_1_WEEK, Tenor.IN_2_WEEKS]
-
-    for q in range(1000000, 1000001, 1000000):
-        for pair in xtx_pairs:
-            pricing.subscribe(
-                pricing.build.fx.stream.spot.liquidity_provider("JPMCFX")
-                .currency_pair(pair)
-                .currency(pair[0:3])
-                .quantity(q)
-                .create_subject()
-            )
-
-            pricing.subscribe(
-                pricing.build.fx.stream.forward.liquidity_provider("JPMCFX")
-                .currency_pair(pair)
-                .currency(pair[0:3])
-                .quantity(q)
-                .tenor(Tenor.IN_1_MONTH)
-                .create_subject()
-            )
+    pricing.subscribe(
+        pricing.build.fx.stream.spot.liquidity_provider("DBFX")
+        .currency_pair("EURUSD")
+        .currency("EUR")
+        .quantity(1000000)
+        .create_subject()
+    )
+    pricing.subscribe(
+        pricing.build.fx.stream.spot.liquidity_provider("DBFX")
+        .currency_pair("USDJPY")
+        .currency("USD")
+        .quantity(5000000)
+        .create_subject()
+    )
 
-#   for i in range(len(currencies)):
-#       for j in range(i + 1, len(currencies)):
-#           for q in quantities:
-#               pricing.subscribe(
-#                   pricing.build.fx.stream.spot.liquidity_provider("XTXFX")
-#                   .currency_pair(currencies[i] + currencies[j])
-#                   .currency(currencies[i])
-#                   .quantity(q)
-#                   .create_subject()
-#               
-#               for t in tenors:
-#                   pricing.subscribe(
-#                       pricing.build.fx.stream.forward.liquidity_provider("XTXFX")
-#                       .currency_pair(currencies[i] + currencies[j])
-#                       .currency(currencies[i])
-#                       .tenor(t)
-#                       .quantity(q)
-#                       .create_subject()
-#                   )
- 
-#   pricing.subscribe(
-#       pricing.build.fx.stream.spot.liquidity_provider("HSBCFX")
-#       .currency_pair("EURUSD")
-#       .currency("USD")
-#       .quantity(500000)
-#       .create_subject()
-#   )
+    sleep(60)
 
-    sleep(3600)
     pricing.stop()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `bidfx-api-1.1.1/examples/pricing/example_fx_spot_with_random_resubscribe.py` & `bidfx-api-1.1.2/examples/pricing/example_fx_spot_with_random_resubscribe.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,14 +63,15 @@
     session = Session.create_from_ini_file()
     pricing = session.pricing
     pricing.callbacks.price_event_fn = on_price_event
     pricing.callbacks.subscription_event_fn = on_subscription_event
     pricing.callbacks.provider_event_fn = on_provider_event
     pricing.start()
     subjects = create_subjects(pricing)
+
     for subject in subjects:
         pricing.subscribe(subject)
     for _ in range(10):
         sleep(2)
         shuffle(subjects)
         for subject in subjects[:3]:
             pricing.unsubscribe(subject)
```

### Comparing `bidfx-api-1.1.1/examples/pricing/example_fx_stream_forwards.py` & `bidfx-api-1.1.2/examples/pricing/example_fx_stream_forwards.py`

 * *Files identical despite different names*

### Comparing `bidfx-api-1.1.1/examples/pricing/example_indicative_fx.py` & `bidfx-api-1.1.2/examples/pricing/example_indicative_fx.py`

 * *Files identical despite different names*

### Comparing `bidfx-api-1.1.1/examples/pricing/example_indicative_fx_and_equity_depth.py` & `bidfx-api-1.1.2/examples/pricing/example_indicative_fx_and_equity_depth.py`

 * *Files identical despite different names*

### Comparing `bidfx-api-1.1.1/examples/pricing/example_indicative_fx_with_unsubscribe.py` & `bidfx-api-1.1.2/examples/pricing/example_indicative_fx_with_unsubscribe.py`

 * *Files identical despite different names*

### Comparing `bidfx-api-1.1.1/examples/pricing/example_minimal.py` & `bidfx-api-1.1.2/examples/pricing/example_minimal.py`

 * *Files identical despite different names*

### Comparing `bidfx-api-1.1.1/examples/pricing/example_mixed_streaming_and_indicative_spot.py` & `bidfx-api-1.1.2/examples/pricing/example_mixed_streaming_and_indicative_spot.py`

 * *Files identical despite different names*

### Comparing `bidfx-api-1.1.1/examples/pricing/example_stream_fx_spot_and_ndf.py` & `bidfx-api-1.1.2/examples/pricing/example_stream_fx_spot_and_ndf.py`

 * *Files identical despite different names*

### Comparing `bidfx-api-1.1.1/requirements-dev.txt` & `bidfx-api-1.1.2/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `bidfx-api-1.1.1/setup.py` & `bidfx-api-1.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 with open("requirements.txt") as f:
     requirements = f.read().splitlines()
 
-version = "1.1.1"
+version = "1.1.2"
 
 setuptools.setup(
     name="bidfx-api",
     version=version,
     author="Paul Sweeny",
     author_email="paul.sweeny@bidfx.com",
     description="Public API for accessing the BidFX platform for pricing",
```

