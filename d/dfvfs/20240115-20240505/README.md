# Comparing `tmp/dfvfs-20240115.tar.gz` & `tmp/dfvfs-20240505.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dfvfs-20240115.tar", last modified: Wed Jan 17 04:00:08 2024, max compression
+gzip compressed data, was "dfvfs-20240505.tar", last modified: Wed May  8 04:24:45 2024, max compression
```

## Comparing `dfvfs-20240115.tar` & `dfvfs-20240505.tar`

### file list

```diff
@@ -1,703 +1,703 @@
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-17 04:00:08.367552 dfvfs-20240115/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-17 04:00:08.258553 dfvfs-20240115/.github/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-17 04:00:08.264553 dfvfs-20240115/.github/workflows/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3663 2024-01-15 06:55:06.000000 dfvfs-20240115/.github/workflows/test_docker.yml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1887 2024-01-15 06:55:06.000000 dfvfs-20240115/.github/workflows/test_docs.yml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5722 2024-01-15 06:55:06.000000 dfvfs-20240115/.github/workflows/test_tox.yml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23352 2024-01-15 06:55:06.000000 dfvfs-20240115/.pylintrc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      322 2024-01-14 19:37:37.000000 dfvfs-20240115/.readthedocs.yaml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      149 2023-12-03 10:55:51.000000 dfvfs-20240115/.yamllint.yaml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1173 2023-12-03 10:55:50.000000 dfvfs-20240115/ACKNOWLEDGEMENTS
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      360 2023-12-03 10:55:51.000000 dfvfs-20240115/AUTHORS
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11358 2023-12-03 10:55:51.000000 dfvfs-20240115/LICENSE
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      632 2024-01-16 05:16:17.000000 dfvfs-20240115/MANIFEST.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      552 2023-12-03 10:55:50.000000 dfvfs-20240115/MANIFEST.test_data.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      915 2024-01-17 04:00:08.367552 dfvfs-20240115/PKG-INFO
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      473 2023-12-03 10:55:51.000000 dfvfs-20240115/README
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2321 2024-01-15 06:55:06.000000 dfvfs-20240115/appveyor.yml
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-17 04:00:08.258553 dfvfs-20240115/config/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-17 04:00:08.264553 dfvfs-20240115/config/appveyor/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1069 2024-01-15 06:55:06.000000 dfvfs-20240115/config/appveyor/install.ps1
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)      125 2024-01-15 06:55:06.000000 dfvfs-20240115/config/appveyor/install.sh
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)      620 2024-01-15 06:55:06.000000 dfvfs-20240115/config/appveyor/runtests.sh
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-17 04:00:08.265553 dfvfs-20240115/config/dpkg/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      168 2024-01-16 05:15:10.000000 dfvfs-20240115/config/dpkg/changelog
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       32 2023-12-03 10:56:42.000000 dfvfs-20240115/config/dpkg/clean
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        2 2024-01-14 19:37:37.000000 dfvfs-20240115/config/dpkg/compat
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1801 2024-01-15 06:55:06.000000 dfvfs-20240115/config/dpkg/control
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      948 2023-12-03 10:56:42.000000 dfvfs-20240115/config/dpkg/copyright
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)      122 2024-01-14 19:37:37.000000 dfvfs-20240115/config/dpkg/rules
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-17 04:00:08.265553 dfvfs-20240115/config/dpkg/source/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       12 2023-12-03 10:56:42.000000 dfvfs-20240115/config/dpkg/source/format
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-17 04:00:08.265553 dfvfs-20240115/config/pylint/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1673 2023-12-03 10:56:42.000000 dfvfs-20240115/config/pylint/spelling-private-dict
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5379 2024-01-16 05:16:28.000000 dfvfs-20240115/dependencies.ini
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-17 04:00:08.265553 dfvfs-20240115/dfvfs/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      278 2024-01-16 05:15:10.000000 dfvfs-20240115/dfvfs/__init__.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-17 04:00:08.271553 dfvfs-20240115/dfvfs/analyzer/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1488 2023-12-03 10:56:42.000000 dfvfs-20240115/dfvfs/analyzer/__init__.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13902 2023-12-03 10:56:42.000000 dfvfs-20240115/dfvfs/analyzer/analyzer.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2083 2023-12-03 10:56:42.000000 dfvfs-20240115/dfvfs/analyzer/analyzer_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      962 2023-12-03 10:56:42.000000 dfvfs-20240115/dfvfs/analyzer/apfs_analyzer_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1010 2023-12-03 10:56:42.000000 dfvfs-20240115/dfvfs/analyzer/apfs_container_analyzer_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1417 2023-12-03 10:56:42.000000 dfvfs-20240115/dfvfs/analyzer/apm_analyzer_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1120 2023-12-03 10:56:42.000000 dfvfs-20240115/dfvfs/analyzer/bde_analyzer_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1087 2023-12-03 10:56:42.000000 dfvfs-20240115/dfvfs/analyzer/bzip2_analyzer_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1404 2023-12-03 10:56:42.000000 dfvfs-20240115/dfvfs/analyzer/cpio_analyzer_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      978 2023-12-03 10:56:42.000000 dfvfs-20240115/dfvfs/analyzer/cs_analyzer_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1182 2023-12-03 10:56:42.000000 dfvfs-20240115/dfvfs/analyzer/ewf_analyzer_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1182 2023-12-03 10:56:42.000000 dfvfs-20240115/dfvfs/analyzer/ext_analyzer_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1547 2023-12-03 10:56:42.000000 dfvfs-20240115/dfvfs/analyzer/fat_analyzer_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1395 2023-12-03 10:56:42.000000 dfvfs-20240115/dfvfs/analyzer/gpt_analyzer_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      964 2023-12-03 10:56:42.000000 dfvfs-20240115/dfvfs/analyzer/gzip_analyzer_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1370 2023-12-03 10:56:42.000000 dfvfs-20240115/dfvfs/analyzer/hfs_analyzer_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      971 2023-12-03 10:56:42.000000 dfvfs-20240115/dfvfs/analyzer/luksde_analyzer_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1174 2023-12-03 10:56:42.000000 dfvfs-20240115/dfvfs/analyzer/lvm_analyzer_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1168 2023-12-03 10:56:42.000000 dfvfs-20240115/dfvfs/analyzer/modi_analyzer_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1186 2023-12-03 10:56:42.000000 dfvfs-20240115/dfvfs/analyzer/ntfs_analyzer_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1003 2023-12-03 10:56:42.000000 dfvfs-20240115/dfvfs/analyzer/phdi_analyzer_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1246 2023-12-03 10:56:42.000000 dfvfs-20240115/dfvfs/analyzer/qcow_analyzer_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4938 2023-12-03 10:56:42.000000 dfvfs-20240115/dfvfs/analyzer/specification.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1057 2023-12-03 10:56:42.000000 dfvfs-20240115/dfvfs/analyzer/tar_analyzer_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2266 2024-01-14 11:15:22.000000 dfvfs-20240115/dfvfs/analyzer/tsk_analyzer_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1040 2023-12-03 10:56:42.000000 dfvfs-20240115/dfvfs/analyzer/tsk_partition_analyzer_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1192 2023-12-03 10:56:42.000000 dfvfs-20240115/dfvfs/analyzer/vhdi_analyzer_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1194 2023-12-03 10:56:42.000000 dfvfs-20240115/dfvfs/analyzer/vmdk_analyzer_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1071 2023-12-03 10:56:42.000000 dfvfs-20240115/dfvfs/analyzer/vshadow_analyzer_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      955 2023-12-03 10:56:42.000000 dfvfs-20240115/dfvfs/analyzer/xfs_analyzer_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      968 2023-12-03 10:56:42.000000 dfvfs-20240115/dfvfs/analyzer/xz_analyzer_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      950 2023-12-03 10:56:42.000000 dfvfs-20240115/dfvfs/analyzer/zip_analyzer_helper.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-17 04:00:08.272553 dfvfs-20240115/dfvfs/compression/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      247 2023-12-03 10:56:42.000000 dfvfs-20240115/dfvfs/compression/__init__.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1355 2023-12-03 10:56:42.000000 dfvfs-20240115/dfvfs/compression/bzip2_decompressor.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      437 2023-12-03 10:56:42.000000 dfvfs-20240115/dfvfs/compression/decompressor.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2286 2023-12-03 10:56:42.000000 dfvfs-20240115/dfvfs/compression/manager.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2139 2023-12-03 10:56:42.000000 dfvfs-20240115/dfvfs/compression/xz_decompressor.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2118 2023-12-03 10:56:42.000000 dfvfs-20240115/dfvfs/compression/zlib_decompressor.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-17 04:00:08.274553 dfvfs-20240115/dfvfs/credentials/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      313 2023-12-03 10:56:42.000000 dfvfs-20240115/dfvfs/credentials/__init__.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      545 2023-12-03 10:56:42.000000 dfvfs-20240115/dfvfs/credentials/apfs_credentials.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      646 2023-12-03 10:56:42.000000 dfvfs-20240115/dfvfs/credentials/bde_credentials.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      562 2023-12-03 10:56:42.000000 dfvfs-20240115/dfvfs/credentials/credentials.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      544 2023-12-03 10:56:42.000000 dfvfs-20240115/dfvfs/credentials/cs_credentials.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      497 2023-12-03 10:56:42.000000 dfvfs-20240115/dfvfs/credentials/encrypted_stream_credentials.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2696 2023-12-03 10:56:42.000000 dfvfs-20240115/dfvfs/credentials/keychain.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      498 2023-12-03 10:56:42.000000 dfvfs-20240115/dfvfs/credentials/luksde_credentials.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1902 2023-12-03 10:56:42.000000 dfvfs-20240115/dfvfs/credentials/manager.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-17 04:00:08.275553 dfvfs-20240115/dfvfs/encoding/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      191 2023-12-03 10:56:42.000000 dfvfs-20240115/dfvfs/encoding/__init__.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      967 2023-12-03 10:56:42.000000 dfvfs-20240115/dfvfs/encoding/base16_decoder.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      967 2023-12-03 10:56:42.000000 dfvfs-20240115/dfvfs/encoding/base32_decoder.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1198 2023-12-03 10:56:42.000000 dfvfs-20240115/dfvfs/encoding/base64_decoder.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      392 2023-12-03 10:56:42.000000 dfvfs-20240115/dfvfs/encoding/decoder.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1955 2023-12-03 10:56:42.000000 dfvfs-20240115/dfvfs/encoding/manager.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-17 04:00:08.276553 dfvfs-20240115/dfvfs/encryption/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      245 2024-01-14 08:46:30.000000 dfvfs-20240115/dfvfs/encryption/__init__.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3323 2024-01-15 06:55:06.000000 dfvfs-20240115/dfvfs/encryption/aes_decrypter.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3531 2024-01-15 06:55:06.000000 dfvfs-20240115/dfvfs/encryption/blowfish_decrypter.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      953 2024-01-15 06:55:06.000000 dfvfs-20240115/dfvfs/encryption/decrypter.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3491 2024-01-15 06:55:06.000000 dfvfs-20240115/dfvfs/encryption/des3_decrypter.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2274 2023-12-03 10:56:42.000000 dfvfs-20240115/dfvfs/encryption/manager.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1339 2024-01-15 06:55:06.000000 dfvfs-20240115/dfvfs/encryption/rc4_decrypter.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-17 04:00:08.284553 dfvfs-20240115/dfvfs/file_io/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       24 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/file_io/__init__.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3960 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/file_io/apfs_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5561 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/file_io/apm_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/file_io/bde_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9503 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/file_io/compressed_stream_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4645 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/file_io/cpio_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4663 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/file_io/cs_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5995 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/file_io/data_range_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9664 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/file_io/encoded_stream_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10708 2024-01-15 06:55:06.000000 dfvfs-20240115/dfvfs/file_io/encrypted_stream_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2710 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/file_io/ewf_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3948 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/file_io/ext_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4175 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/file_io/fake_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4398 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/file_io/fat_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5057 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/file_io/file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4157 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/file_io/file_object_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5569 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/file_io/gpt_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2401 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/file_io/gzip_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4501 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/file_io/hfs_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1272 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/file_io/luksde_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3978 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/file_io/lvm_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1856 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/file_io/modi_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4540 2023-12-03 10:56:42.000000 dfvfs-20240115/dfvfs/file_io/ntfs_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6180 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/file_io/os_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4378 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/file_io/phdi_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4074 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/file_io/qcow_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2733 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/file_io/raw_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8363 2023-12-27 09:22:15.000000 dfvfs-20240115/dfvfs/file_io/sqlite_blob_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4775 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/file_io/tar_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7991 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/file_io/tsk_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2370 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/file_io/tsk_partition_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4313 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/file_io/vhdi_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4201 2023-12-03 10:56:42.000000 dfvfs-20240115/dfvfs/file_io/vmdk_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4106 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/file_io/vshadow_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3941 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/file_io/xfs_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9026 2023-12-03 10:56:42.000000 dfvfs-20240115/dfvfs/file_io/zip_file_io.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-17 04:00:08.287553 dfvfs-20240115/dfvfs/helpers/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       24 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/helpers/__init__.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29440 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/helpers/command_line.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2093 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/helpers/data_slice.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3992 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/helpers/fake_file_system_builder.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22177 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/helpers/file_system_searcher.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30704 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/helpers/source_scanner.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6081 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/helpers/text_file.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28568 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/helpers/volume_scanner.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9517 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/helpers/windows_path_resolver.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-17 04:00:08.291553 dfvfs-20240115/dfvfs/lib/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       24 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/lib/__init__.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      835 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/lib/apfs_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      722 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/lib/apm_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1710 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/lib/bde_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10516 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/lib/cpio.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4230 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/lib/cpio.yaml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1677 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/lib/cs_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3532 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/lib/data_format.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      710 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/lib/decorators.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4759 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/lib/definitions.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1053 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/lib/errors.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3502 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/lib/ewf_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2345 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/lib/glob2regex.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19596 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/lib/gzipfile.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1489 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/lib/gzipfile.yaml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1160 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/lib/luksde_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      866 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/lib/lvm_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12570 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/lib/raw_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5970 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/lib/sqlite_database.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1775 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/lib/tsk_image.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5460 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/lib/tsk_partition.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      745 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/lib/vshadow_helper.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-17 04:00:08.292553 dfvfs-20240115/dfvfs/mount/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       24 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/mount/__init__.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2036 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/mount/manager.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-17 04:00:08.301553 dfvfs-20240115/dfvfs/path/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1450 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/path/__init__.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1564 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/path/apfs_container_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1547 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/path/apfs_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1473 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/path/apm_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1769 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/path/bde_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1387 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/path/compressed_stream_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      965 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/path/cpio_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2397 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/path/cs_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1517 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/path/data_range_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1332 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/path/encoded_stream_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2414 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/path/encrypted_stream_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      777 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/path/ewf_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1475 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/path/ext_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3742 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/path/factory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      940 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/path/fake_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1560 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/path/fat_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1474 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/path/gpt_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      782 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/path/gzip_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1932 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/path/hfs_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      923 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/path/location_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1217 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/path/luksde_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1482 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/path/lvm_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      798 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/path/modi_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1102 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/path/mount_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2364 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/path/ntfs_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1412 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/path/os_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4043 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/path/path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      784 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/path/phdi_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      779 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/path/qcow_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      800 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/path/raw_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2964 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/path/sqlite_blob_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      947 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/path/tar_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1777 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/path/tsk_partition_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1943 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/path/tsk_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      810 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/path/vhdi_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      784 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/path/vmdk_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1499 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/path/vshadow_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1475 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/path/xfs_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      978 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/path/zip_path_spec.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-17 04:00:08.301553 dfvfs-20240115/dfvfs/resolver/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       24 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/resolver/__init__.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4365 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/resolver/context.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6142 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/resolver/resolver.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-17 04:00:08.310553 dfvfs-20240115/dfvfs/resolver_helpers/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2813 2023-12-03 10:56:44.000000 dfvfs-20240115/dfvfs/resolver_helpers/__init__.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      904 2023-12-03 10:56:44.000000 dfvfs-20240115/dfvfs/resolver_helpers/apfs_container_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1195 2023-12-03 10:56:44.000000 dfvfs-20240115/dfvfs/resolver_helpers/apfs_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1206 2023-12-03 10:56:44.000000 dfvfs-20240115/dfvfs/resolver_helpers/apm_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1195 2023-12-03 10:56:44.000000 dfvfs-20240115/dfvfs/resolver_helpers/bde_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1329 2023-12-03 10:56:44.000000 dfvfs-20240115/dfvfs/resolver_helpers/compressed_stream_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1246 2023-12-03 10:56:44.000000 dfvfs-20240115/dfvfs/resolver_helpers/cpio_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1198 2023-12-03 10:56:44.000000 dfvfs-20240115/dfvfs/resolver_helpers/cs_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1252 2023-12-03 10:56:44.000000 dfvfs-20240115/dfvfs/resolver_helpers/data_range_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1296 2023-12-03 10:56:44.000000 dfvfs-20240115/dfvfs/resolver_helpers/encoded_stream_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1318 2023-12-03 10:56:44.000000 dfvfs-20240115/dfvfs/resolver_helpers/encrypted_stream_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      824 2023-12-03 10:56:44.000000 dfvfs-20240115/dfvfs/resolver_helpers/ewf_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1184 2023-12-03 10:56:44.000000 dfvfs-20240115/dfvfs/resolver_helpers/ext_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      522 2023-12-03 10:56:44.000000 dfvfs-20240115/dfvfs/resolver_helpers/fake_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1184 2023-12-03 10:56:44.000000 dfvfs-20240115/dfvfs/resolver_helpers/fat_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1207 2023-12-03 10:56:44.000000 dfvfs-20240115/dfvfs/resolver_helpers/gpt_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1205 2023-12-03 10:56:44.000000 dfvfs-20240115/dfvfs/resolver_helpers/gzip_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1184 2023-12-03 10:56:44.000000 dfvfs-20240115/dfvfs/resolver_helpers/hfs_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2023-12-03 10:56:44.000000 dfvfs-20240115/dfvfs/resolver_helpers/luksde_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1209 2023-12-03 10:56:44.000000 dfvfs-20240115/dfvfs/resolver_helpers/lvm_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1928 2023-12-03 10:56:44.000000 dfvfs-20240115/dfvfs/resolver_helpers/manager.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      846 2023-12-03 10:56:45.000000 dfvfs-20240115/dfvfs/resolver_helpers/modi_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1195 2023-12-03 10:56:44.000000 dfvfs-20240115/dfvfs/resolver_helpers/ntfs_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1201 2023-12-03 10:56:44.000000 dfvfs-20240115/dfvfs/resolver_helpers/os_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      832 2023-12-03 10:56:45.000000 dfvfs-20240115/dfvfs/resolver_helpers/phdi_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      832 2023-12-03 10:56:44.000000 dfvfs-20240115/dfvfs/resolver_helpers/qcow_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      838 2023-12-03 10:56:44.000000 dfvfs-20240115/dfvfs/resolver_helpers/raw_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1717 2023-12-03 10:56:44.000000 dfvfs-20240115/dfvfs/resolver_helpers/resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1300 2023-12-03 10:56:44.000000 dfvfs-20240115/dfvfs/resolver_helpers/sqlite_blob_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1184 2023-12-03 10:56:44.000000 dfvfs-20240115/dfvfs/resolver_helpers/tar_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1312 2023-12-03 10:56:44.000000 dfvfs-20240115/dfvfs/resolver_helpers/tsk_partition_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1208 2023-12-03 10:56:44.000000 dfvfs-20240115/dfvfs/resolver_helpers/tsk_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      830 2023-12-03 10:56:44.000000 dfvfs-20240115/dfvfs/resolver_helpers/vhdi_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      832 2023-12-03 10:56:44.000000 dfvfs-20240115/dfvfs/resolver_helpers/vmdk_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1246 2023-12-03 10:56:44.000000 dfvfs-20240115/dfvfs/resolver_helpers/vshadow_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1184 2023-12-03 10:56:44.000000 dfvfs-20240115/dfvfs/resolver_helpers/xfs_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1184 2023-12-03 10:56:44.000000 dfvfs-20240115/dfvfs/resolver_helpers/zip_resolver_helper.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-17 04:00:08.310553 dfvfs-20240115/dfvfs/serializer/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       24 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/serializer/__init__.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5458 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/serializer/json_serializer.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      957 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/serializer/serializer.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-17 04:00:08.330553 dfvfs-20240115/dfvfs/vfs/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       24 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/vfs/__init__.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3622 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/vfs/apfs_attribute.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1225 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/vfs/apfs_container_directory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4595 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/vfs/apfs_container_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5539 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/vfs/apfs_container_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/vfs/apfs_directory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8895 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/vfs/apfs_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6044 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/vfs/apfs_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1331 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/vfs/apm_directory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3577 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/vfs/apm_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4352 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/vfs/apm_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2064 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/vfs/attribute.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2188 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/vfs/bde_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2758 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/vfs/bde_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1637 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/vfs/compressed_stream_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2621 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/vfs/compressed_stream_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/vfs/cpio_directory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7019 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/vfs/cpio_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4635 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/vfs/cpio_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1112 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/vfs/cs_directory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4353 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/vfs/cs_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5012 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/vfs/cs_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1335 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/vfs/data_range_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2781 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/vfs/data_range_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      859 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/vfs/data_stream.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      961 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/vfs/directory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/vfs/encoded_stream_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2534 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/vfs/encoded_stream_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1625 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/vfs/encrypted_stream_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2699 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/vfs/encrypted_stream_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3601 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/vfs/ext_attribute.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1434 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/vfs/ext_directory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9823 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/vfs/ext_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5159 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/vfs/ext_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      844 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/vfs/extent.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1212 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/vfs/fake_directory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4684 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/vfs/fake_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5004 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/vfs/fake_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1437 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/vfs/fat_directory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7675 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/vfs/fat_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5634 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/vfs/fat_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11742 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/vfs/file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7136 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/vfs/file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1085 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/vfs/gpt_directory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3656 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/vfs/gpt_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5257 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/vfs/gpt_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1849 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/vfs/gzip_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1019 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/vfs/gzip_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3601 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/vfs/hfs_attribute.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1378 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/vfs/hfs_data_stream.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1437 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/vfs/hfs_directory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10348 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/vfs/hfs_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5316 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/vfs/hfs_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1944 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/vfs/luksde_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2856 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/vfs/luksde_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1129 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/vfs/lvm_directory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3835 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/vfs/lvm_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4750 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/vfs/lvm_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5041 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/vfs/ntfs_attribute.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1411 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/vfs/ntfs_data_stream.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1838 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/vfs/ntfs_directory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12181 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/vfs/ntfs_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5882 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/vfs/ntfs_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3067 2024-01-06 18:42:17.000000 dfvfs-20240115/dfvfs/vfs/os_attribute.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1662 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/vfs/os_directory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9469 2024-01-06 18:39:32.000000 dfvfs-20240115/dfvfs/vfs/os_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6345 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/vfs/os_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      665 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/vfs/root_only_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1699 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/vfs/root_only_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1853 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/vfs/sqlite_blob_directory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4202 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/vfs/sqlite_blob_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3520 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/vfs/sqlite_blob_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2093 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/vfs/tar_directory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6442 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/vfs/tar_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5180 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/vfs/tar_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4281 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/vfs/tsk_attribute.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3018 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/vfs/tsk_data_stream.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4156 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/vfs/tsk_directory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27761 2023-12-29 05:21:46.000000 dfvfs-20240115/dfvfs/vfs/tsk_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7175 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/vfs/tsk_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1865 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/vfs/tsk_partition_directory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4278 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/vfs/tsk_partition_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4196 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/vfs/tsk_partition_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1128 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/vfs/vshadow_directory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4224 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/vfs/vshadow_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4412 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/vfs/vshadow_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3601 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/vfs/xfs_attribute.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1434 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/vfs/xfs_directory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8567 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/vfs/xfs_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5313 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/vfs/xfs_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2261 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/vfs/zip_directory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6332 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/vfs/zip_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4975 2023-12-03 10:56:43.000000 dfvfs-20240115/dfvfs/vfs/zip_file_system.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-17 04:00:08.332553 dfvfs-20240115/dfvfs/volume/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      375 2023-12-03 10:56:44.000000 dfvfs-20240115/dfvfs/volume/__init__.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1563 2023-12-03 10:56:44.000000 dfvfs-20240115/dfvfs/volume/apfs_volume_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1421 2023-12-03 10:56:44.000000 dfvfs-20240115/dfvfs/volume/apm_volume_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1513 2023-12-03 10:56:44.000000 dfvfs-20240115/dfvfs/volume/cs_volume_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1710 2023-12-03 10:56:44.000000 dfvfs-20240115/dfvfs/volume/factory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1427 2023-12-03 10:56:44.000000 dfvfs-20240115/dfvfs/volume/gpt_volume_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1539 2023-12-03 10:56:44.000000 dfvfs-20240115/dfvfs/volume/lvm_volume_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3054 2023-12-03 10:56:44.000000 dfvfs-20240115/dfvfs/volume/tsk_volume_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7299 2023-12-03 10:56:44.000000 dfvfs-20240115/dfvfs/volume/volume_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2017 2023-12-03 10:56:44.000000 dfvfs-20240115/dfvfs/volume/vshadow_volume_system.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-17 04:00:08.266553 dfvfs-20240115/dfvfs.egg-info/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      915 2024-01-17 04:00:06.000000 dfvfs-20240115/dfvfs.egg-info/PKG-INFO
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20887 2024-01-17 04:00:08.000000 dfvfs-20240115/dfvfs.egg-info/SOURCES.txt
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        1 2024-01-17 04:00:06.000000 dfvfs-20240115/dfvfs.egg-info/dependency_links.txt
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      775 2024-01-17 04:00:06.000000 dfvfs-20240115/dfvfs.egg-info/requires.txt
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        6 2024-01-17 04:00:06.000000 dfvfs-20240115/dfvfs.egg-info/top_level.txt
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1017 2023-12-03 10:55:50.000000 dfvfs-20240115/dfvfs.ini
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-17 04:00:08.332553 dfvfs-20240115/docs/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5037 2024-01-14 19:37:37.000000 dfvfs-20240115/docs/conf.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1453 2023-12-03 10:57:15.000000 dfvfs-20240115/docs/index.rst
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      118 2024-01-14 19:37:37.000000 dfvfs-20240115/docs/requirements.txt
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-17 04:00:08.333553 dfvfs-20240115/docs/sources/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3182 2023-12-03 10:57:15.000000 dfvfs-20240115/docs/sources/Code-snippets.md
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14179 2023-12-03 10:57:15.000000 dfvfs-20240115/docs/sources/Path-specifications.md
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4117 2024-01-15 06:55:06.000000 dfvfs-20240115/docs/sources/Supported-formats.md
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-17 04:00:08.336553 dfvfs-20240115/docs/sources/api/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6275 2023-12-03 10:57:16.000000 dfvfs-20240115/docs/sources/api/dfvfs.analyzer.rst
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1125 2023-12-03 10:57:15.000000 dfvfs-20240115/docs/sources/api/dfvfs.compression.rst
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1704 2023-12-03 10:57:16.000000 dfvfs-20240115/docs/sources/api/dfvfs.credentials.rst
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1032 2023-12-03 10:57:15.000000 dfvfs-20240115/docs/sources/api/dfvfs.encoding.rst
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1264 2023-12-03 10:57:16.000000 dfvfs-20240115/docs/sources/api/dfvfs.encryption.rst
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6310 2023-12-03 10:57:16.000000 dfvfs-20240115/docs/sources/api/dfvfs.file_io.rst
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1629 2023-12-03 10:57:16.000000 dfvfs-20240115/docs/sources/api/dfvfs.helpers.rst
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3042 2023-12-03 10:57:16.000000 dfvfs-20240115/docs/sources/api/dfvfs.lib.rst
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      325 2023-12-03 10:57:15.000000 dfvfs-20240115/docs/sources/api/dfvfs.mount.rst
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6712 2023-12-03 10:57:15.000000 dfvfs-20240115/docs/sources/api/dfvfs.path.rst
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      501 2023-12-03 10:57:16.000000 dfvfs-20240115/docs/sources/api/dfvfs.resolver.rst
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8397 2023-12-03 10:57:15.000000 dfvfs-20240115/docs/sources/api/dfvfs.resolver_helpers.rst
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      461 2023-12-03 10:57:16.000000 dfvfs-20240115/docs/sources/api/dfvfs.rst
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      551 2023-12-03 10:57:16.000000 dfvfs-20240115/docs/sources/api/dfvfs.serializer.rst
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15898 2023-12-03 10:57:16.000000 dfvfs-20240115/docs/sources/api/dfvfs.vfs.rst
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1793 2023-12-03 10:57:15.000000 dfvfs-20240115/docs/sources/api/dfvfs.volume.rst
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       52 2023-12-03 10:57:15.000000 dfvfs-20240115/docs/sources/api/modules.rst
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-17 04:00:08.337553 dfvfs-20240115/docs/sources/developer/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6837 2023-12-03 10:57:16.000000 dfvfs-20240115/docs/sources/developer/Adding-new-type.md
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5979 2023-12-03 10:57:16.000000 dfvfs-20240115/docs/sources/developer/Helpers.md
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3991 2023-12-03 10:57:16.000000 dfvfs-20240115/docs/sources/developer/Internals.md
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      447 2023-12-03 10:57:16.000000 dfvfs-20240115/docs/sources/developer/Testing.md
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      398 2023-12-03 10:57:16.000000 dfvfs-20240115/docs/sources/developer/index.rst
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-17 04:00:08.337553 dfvfs-20240115/docs/sources/user/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1597 2023-12-03 10:57:16.000000 dfvfs-20240115/docs/sources/user/Installation-instructions.md
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      282 2023-12-03 10:57:16.000000 dfvfs-20240115/docs/sources/user/index.rst
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       90 2024-01-14 19:37:37.000000 dfvfs-20240115/pyproject.toml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      835 2024-01-15 06:55:06.000000 dfvfs-20240115/requirements.txt
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     1018 2023-12-03 10:55:50.000000 dfvfs-20240115/run_tests.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2452 2024-01-17 04:00:08.368552 dfvfs-20240115/setup.cfg
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)      128 2024-01-14 19:37:37.000000 dfvfs-20240115/setup.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2023-12-03 10:55:51.000000 dfvfs-20240115/test_dependencies.ini
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-14 19:37:37.000000 dfvfs-20240115/test_requirements.txt
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-17 04:00:08.337553 dfvfs-20240115/tests/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       24 2023-12-03 10:57:02.000000 dfvfs-20240115/tests/__init__.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-17 04:00:08.338553 dfvfs-20240115/tests/analyzer/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       24 2023-12-03 10:57:03.000000 dfvfs-20240115/tests/analyzer/__init__.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18453 2023-12-03 10:57:03.000000 dfvfs-20240115/tests/analyzer/analyzer.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      912 2023-12-03 10:57:03.000000 dfvfs-20240115/tests/analyzer/specification.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-17 04:00:08.338553 dfvfs-20240115/tests/compression/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       24 2023-12-03 10:57:03.000000 dfvfs-20240115/tests/compression/__init__.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1231 2023-12-03 10:57:03.000000 dfvfs-20240115/tests/compression/bzip2_decompressor.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2083 2023-12-03 10:57:03.000000 dfvfs-20240115/tests/compression/manager.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      224 2023-12-03 10:57:03.000000 dfvfs-20240115/tests/compression/test_lib.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2425 2023-12-03 10:57:03.000000 dfvfs-20240115/tests/compression/xz_decompressor.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1646 2023-12-03 10:57:03.000000 dfvfs-20240115/tests/compression/zlib_decompressor.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-17 04:00:08.339552 dfvfs-20240115/tests/credentials/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       24 2023-12-03 10:57:08.000000 dfvfs-20240115/tests/credentials/__init__.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      543 2023-12-03 10:57:08.000000 dfvfs-20240115/tests/credentials/apfs_credentials.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      555 2023-12-03 10:57:08.000000 dfvfs-20240115/tests/credentials/bde_credentials.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      475 2023-12-03 10:57:08.000000 dfvfs-20240115/tests/credentials/credentials.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      521 2023-12-03 10:57:08.000000 dfvfs-20240115/tests/credentials/cs_credentials.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      562 2023-12-03 10:57:08.000000 dfvfs-20240115/tests/credentials/encrypted_stream_credentials.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1344 2023-12-03 10:57:08.000000 dfvfs-20240115/tests/credentials/keychain.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      545 2023-12-03 10:57:08.000000 dfvfs-20240115/tests/credentials/luksde_credentials.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2146 2023-12-03 10:57:08.000000 dfvfs-20240115/tests/credentials/manager.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-17 04:00:08.339552 dfvfs-20240115/tests/encoding/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       24 2023-12-03 10:57:03.000000 dfvfs-20240115/tests/encoding/__init__.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      804 2023-12-03 10:57:03.000000 dfvfs-20240115/tests/encoding/base16_decoder.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      804 2023-12-03 10:57:03.000000 dfvfs-20240115/tests/encoding/base32_decoder.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      801 2023-12-03 10:57:03.000000 dfvfs-20240115/tests/encoding/base64_decoder.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1852 2023-12-03 10:57:03.000000 dfvfs-20240115/tests/encoding/manager.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      214 2023-12-03 10:57:03.000000 dfvfs-20240115/tests/encoding/test_lib.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-17 04:00:08.340553 dfvfs-20240115/tests/encryption/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       24 2023-12-03 10:57:08.000000 dfvfs-20240115/tests/encryption/__init__.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3449 2024-01-15 06:55:06.000000 dfvfs-20240115/tests/encryption/aes_decrypter.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3255 2024-01-15 06:55:06.000000 dfvfs-20240115/tests/encryption/blowfish_decrypter.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      559 2024-01-15 06:55:06.000000 dfvfs-20240115/tests/encryption/decrypter.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3449 2024-01-15 06:55:06.000000 dfvfs-20240115/tests/encryption/des3_decrypter.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2302 2023-12-03 10:57:08.000000 dfvfs-20240115/tests/encryption/manager.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1136 2024-01-14 11:15:00.000000 dfvfs-20240115/tests/encryption/rc4_decrypter.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      218 2023-12-03 10:57:08.000000 dfvfs-20240115/tests/encryption/test_lib.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-17 04:00:08.343552 dfvfs-20240115/tests/file_io/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       24 2023-12-03 10:57:04.000000 dfvfs-20240115/tests/file_io/__init__.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4656 2023-12-03 10:57:04.000000 dfvfs-20240115/tests/file_io/apfs_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3037 2023-12-03 10:57:04.000000 dfvfs-20240115/tests/file_io/apm_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6036 2023-12-03 10:57:04.000000 dfvfs-20240115/tests/file_io/bde_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9395 2023-12-03 10:57:04.000000 dfvfs-20240115/tests/file_io/compressed_stream_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6471 2023-12-03 10:57:04.000000 dfvfs-20240115/tests/file_io/cpio_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9118 2023-12-03 10:57:04.000000 dfvfs-20240115/tests/file_io/cs_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2793 2023-12-03 10:57:04.000000 dfvfs-20240115/tests/file_io/data_range_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6975 2023-12-03 10:57:04.000000 dfvfs-20240115/tests/file_io/encoded_stream_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14381 2023-12-03 10:57:04.000000 dfvfs-20240115/tests/file_io/encrypted_stream_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3128 2023-12-03 10:57:04.000000 dfvfs-20240115/tests/file_io/ewf_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4396 2023-12-03 10:57:04.000000 dfvfs-20240115/tests/file_io/ext_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3463 2023-12-03 10:57:04.000000 dfvfs-20240115/tests/file_io/fake_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3104 2023-12-03 10:57:04.000000 dfvfs-20240115/tests/file_io/fat_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1552 2023-12-03 10:57:04.000000 dfvfs-20240115/tests/file_io/gpt_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4168 2023-12-03 10:57:04.000000 dfvfs-20240115/tests/file_io/gzip_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3512 2023-12-03 10:57:04.000000 dfvfs-20240115/tests/file_io/hfs_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3659 2023-12-03 10:57:04.000000 dfvfs-20240115/tests/file_io/luksde_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6235 2023-12-03 10:57:04.000000 dfvfs-20240115/tests/file_io/lvm_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5726 2023-12-03 10:57:04.000000 dfvfs-20240115/tests/file_io/modi_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3082 2023-12-03 10:57:04.000000 dfvfs-20240115/tests/file_io/ntfs_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5213 2023-12-03 10:57:04.000000 dfvfs-20240115/tests/file_io/os_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3042 2023-12-03 10:57:04.000000 dfvfs-20240115/tests/file_io/phdi_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1722 2023-12-03 10:57:04.000000 dfvfs-20240115/tests/file_io/qcow_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2868 2023-12-03 10:57:04.000000 dfvfs-20240115/tests/file_io/raw_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3603 2023-12-03 10:57:04.000000 dfvfs-20240115/tests/file_io/sqlite_blob_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1843 2023-12-03 10:57:04.000000 dfvfs-20240115/tests/file_io/tar_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33122 2023-12-03 10:57:04.000000 dfvfs-20240115/tests/file_io/test_lib.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12616 2023-12-03 10:57:04.000000 dfvfs-20240115/tests/file_io/tsk_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1126 2023-12-03 10:57:04.000000 dfvfs-20240115/tests/file_io/tsk_partition_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16839 2023-12-03 10:57:04.000000 dfvfs-20240115/tests/file_io/vhdi_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1721 2023-12-03 10:57:04.000000 dfvfs-20240115/tests/file_io/vmdk_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5037 2023-12-03 10:57:04.000000 dfvfs-20240115/tests/file_io/vshadow_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4369 2023-12-03 10:57:04.000000 dfvfs-20240115/tests/file_io/xfs_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1895 2023-12-03 10:57:04.000000 dfvfs-20240115/tests/file_io/zip_file_io.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-17 04:00:08.344553 dfvfs-20240115/tests/helpers/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       24 2023-12-03 10:57:04.000000 dfvfs-20240115/tests/helpers/__init__.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39320 2023-12-03 10:57:04.000000 dfvfs-20240115/tests/helpers/command_line.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2714 2023-12-03 10:57:04.000000 dfvfs-20240115/tests/helpers/data_slice.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2644 2023-12-03 10:57:04.000000 dfvfs-20240115/tests/helpers/fake_file_system_builder.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26712 2023-12-03 10:57:04.000000 dfvfs-20240115/tests/helpers/file_system_searcher.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    36588 2023-12-03 10:57:04.000000 dfvfs-20240115/tests/helpers/source_scanner.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8964 2023-12-03 10:57:04.000000 dfvfs-20240115/tests/helpers/text_file.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    38545 2023-12-03 10:57:04.000000 dfvfs-20240115/tests/helpers/volume_scanner.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6744 2023-12-03 10:57:04.000000 dfvfs-20240115/tests/helpers/windows_path_resolver.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-17 04:00:08.345553 dfvfs-20240115/tests/lib/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       24 2023-12-03 10:57:05.000000 dfvfs-20240115/tests/lib/__init__.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3221 2023-12-03 10:57:05.000000 dfvfs-20240115/tests/lib/apfs_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9118 2023-12-03 10:57:05.000000 dfvfs-20240115/tests/lib/cpio.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1756 2023-12-03 10:57:05.000000 dfvfs-20240115/tests/lib/cs_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16350 2023-12-03 10:57:05.000000 dfvfs-20240115/tests/lib/ewf_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1923 2023-12-03 10:57:05.000000 dfvfs-20240115/tests/lib/glob2regex.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5410 2023-12-03 10:57:05.000000 dfvfs-20240115/tests/lib/gzipfile.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1806 2023-12-03 10:57:05.000000 dfvfs-20240115/tests/lib/lvm_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20600 2023-12-03 10:57:05.000000 dfvfs-20240115/tests/lib/raw_helper.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-17 04:00:08.345553 dfvfs-20240115/tests/mount/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       24 2023-12-03 10:57:05.000000 dfvfs-20240115/tests/mount/__init__.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3950 2023-12-03 10:57:05.000000 dfvfs-20240115/tests/mount/manager.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-17 04:00:08.349552 dfvfs-20240115/tests/path/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       24 2023-12-03 10:57:05.000000 dfvfs-20240115/tests/path/__init__.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2784 2023-12-03 10:57:05.000000 dfvfs-20240115/tests/path/apfs_container_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2372 2023-12-03 10:57:05.000000 dfvfs-20240115/tests/path/apfs_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2457 2023-12-03 10:57:05.000000 dfvfs-20240115/tests/path/apm_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1090 2023-12-03 10:57:05.000000 dfvfs-20240115/tests/path/bde_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1601 2023-12-03 10:57:05.000000 dfvfs-20240115/tests/path/compressed_stream_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1335 2023-12-03 10:57:05.000000 dfvfs-20240115/tests/path/cpio_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2429 2023-12-03 10:57:05.000000 dfvfs-20240115/tests/path/cs_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1752 2023-12-03 10:57:05.000000 dfvfs-20240115/tests/path/data_range_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1538 2023-12-03 10:57:05.000000 dfvfs-20240115/tests/path/encoded_stream_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2324 2023-12-03 10:57:05.000000 dfvfs-20240115/tests/path/encryption_stream_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1102 2023-12-03 10:57:05.000000 dfvfs-20240115/tests/path/ewf_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2310 2023-12-03 10:57:05.000000 dfvfs-20240115/tests/path/ext_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1580 2023-12-03 10:57:05.000000 dfvfs-20240115/tests/path/factory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1331 2023-12-03 10:57:05.000000 dfvfs-20240115/tests/path/fake_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2345 2023-12-03 10:57:05.000000 dfvfs-20240115/tests/path/fat_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2457 2023-12-03 10:57:05.000000 dfvfs-20240115/tests/path/gpt_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1113 2023-12-03 10:57:05.000000 dfvfs-20240115/tests/path/gzip_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2843 2023-12-03 10:57:05.000000 dfvfs-20240115/tests/path/hfs_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1129 2023-12-03 10:57:05.000000 dfvfs-20240115/tests/path/luksde_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2463 2023-12-03 10:57:05.000000 dfvfs-20240115/tests/path/lvm_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1129 2023-12-03 10:57:05.000000 dfvfs-20240115/tests/path/modi_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      945 2023-12-03 10:57:05.000000 dfvfs-20240115/tests/path/mount_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3362 2023-12-03 10:57:05.000000 dfvfs-20240115/tests/path/ntfs_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1990 2023-12-03 10:57:05.000000 dfvfs-20240115/tests/path/os_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2585 2023-12-03 10:57:05.000000 dfvfs-20240115/tests/path/path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1115 2023-12-03 10:57:05.000000 dfvfs-20240115/tests/path/phdi_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1115 2023-12-03 10:57:05.000000 dfvfs-20240115/tests/path/qcow_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1130 2023-12-03 10:57:05.000000 dfvfs-20240115/tests/path/raw_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2920 2023-12-03 10:57:05.000000 dfvfs-20240115/tests/path/sqlite_blob_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1320 2023-12-03 10:57:05.000000 dfvfs-20240115/tests/path/tar_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      778 2023-12-03 10:57:05.000000 dfvfs-20240115/tests/path/test_lib.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3228 2023-12-03 10:57:05.000000 dfvfs-20240115/tests/path/tsk_partition_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2808 2023-12-03 10:57:05.000000 dfvfs-20240115/tests/path/tsk_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1141 2023-12-03 10:57:05.000000 dfvfs-20240115/tests/path/vhdi_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1115 2023-12-03 10:57:05.000000 dfvfs-20240115/tests/path/vmdk_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2561 2023-12-03 10:57:05.000000 dfvfs-20240115/tests/path/vshadow_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2310 2023-12-03 10:57:05.000000 dfvfs-20240115/tests/path/xfs_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1320 2023-12-03 10:57:05.000000 dfvfs-20240115/tests/path/zip_path_spec.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-17 04:00:08.349552 dfvfs-20240115/tests/resolver/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5408 2023-12-03 10:57:06.000000 dfvfs-20240115/tests/resolver/context.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-17 04:00:08.352553 dfvfs-20240115/tests/resolver_helpers/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       24 2023-12-03 10:57:02.000000 dfvfs-20240115/tests/resolver_helpers/__init__.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1914 2023-12-03 10:57:02.000000 dfvfs-20240115/tests/resolver_helpers/apfs_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1700 2023-12-03 10:57:02.000000 dfvfs-20240115/tests/resolver_helpers/apm_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2023-12-03 10:57:02.000000 dfvfs-20240115/tests/resolver_helpers/bde_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1682 2023-12-03 10:57:02.000000 dfvfs-20240115/tests/resolver_helpers/compressed_stream_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1587 2023-12-03 10:57:02.000000 dfvfs-20240115/tests/resolver_helpers/cpio_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1846 2023-12-03 10:57:03.000000 dfvfs-20240115/tests/resolver_helpers/cs_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1641 2023-12-03 10:57:02.000000 dfvfs-20240115/tests/resolver_helpers/encoded_stream_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1665 2023-12-03 10:57:02.000000 dfvfs-20240115/tests/resolver_helpers/encrypted_stream_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1428 2023-12-03 10:57:02.000000 dfvfs-20240115/tests/resolver_helpers/ewf_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1697 2023-12-03 10:57:03.000000 dfvfs-20240115/tests/resolver_helpers/ext_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1698 2023-12-03 10:57:03.000000 dfvfs-20240115/tests/resolver_helpers/fat_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1696 2023-12-03 10:57:03.000000 dfvfs-20240115/tests/resolver_helpers/gpt_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1413 2023-12-03 10:57:03.000000 dfvfs-20240115/tests/resolver_helpers/gzip_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1700 2023-12-03 10:57:03.000000 dfvfs-20240115/tests/resolver_helpers/hfs_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1429 2023-12-03 10:57:02.000000 dfvfs-20240115/tests/resolver_helpers/luksde_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1696 2023-12-03 10:57:02.000000 dfvfs-20240115/tests/resolver_helpers/lvm_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1194 2023-12-03 10:57:02.000000 dfvfs-20240115/tests/resolver_helpers/manager.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1463 2023-12-03 10:57:03.000000 dfvfs-20240115/tests/resolver_helpers/modi_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1714 2023-12-03 10:57:02.000000 dfvfs-20240115/tests/resolver_helpers/ntfs_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1378 2023-12-03 10:57:02.000000 dfvfs-20240115/tests/resolver_helpers/os_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1466 2023-12-03 10:57:03.000000 dfvfs-20240115/tests/resolver_helpers/phdi_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1443 2023-12-03 10:57:02.000000 dfvfs-20240115/tests/resolver_helpers/qcow_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1428 2023-12-03 10:57:02.000000 dfvfs-20240115/tests/resolver_helpers/raw_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1617 2023-12-03 10:57:02.000000 dfvfs-20240115/tests/resolver_helpers/sqlite_blob_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1413 2023-12-03 10:57:02.000000 dfvfs-20240115/tests/resolver_helpers/tar_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2525 2023-12-03 10:57:03.000000 dfvfs-20240115/tests/resolver_helpers/test_lib.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1882 2023-12-03 10:57:02.000000 dfvfs-20240115/tests/resolver_helpers/tsk_partition_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1721 2023-12-03 10:57:02.000000 dfvfs-20240115/tests/resolver_helpers/tsk_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1467 2023-12-03 10:57:03.000000 dfvfs-20240115/tests/resolver_helpers/vhdi_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1442 2023-12-03 10:57:03.000000 dfvfs-20240115/tests/resolver_helpers/vmdk_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1748 2023-12-03 10:57:02.000000 dfvfs-20240115/tests/resolver_helpers/vshadow_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1696 2023-12-03 10:57:03.000000 dfvfs-20240115/tests/resolver_helpers/xfs_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1567 2023-12-03 10:57:02.000000 dfvfs-20240115/tests/resolver_helpers/zip_resolver_helper.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-17 04:00:08.352553 dfvfs-20240115/tests/serializer/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       24 2023-12-03 10:57:06.000000 dfvfs-20240115/tests/serializer/__init__.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1978 2023-12-03 10:57:06.000000 dfvfs-20240115/tests/serializer/json_serializer.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1996 2023-12-03 10:57:02.000000 dfvfs-20240115/tests/test_lib.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-17 04:00:08.363552 dfvfs-20240115/tests/vfs/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       24 2023-12-03 10:57:06.000000 dfvfs-20240115/tests/vfs/__init__.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2458 2023-12-03 10:57:07.000000 dfvfs-20240115/tests/vfs/apfs_attribute.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2058 2023-12-03 10:57:07.000000 dfvfs-20240115/tests/vfs/apfs_container_directory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16546 2023-12-03 10:57:06.000000 dfvfs-20240115/tests/vfs/apfs_container_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9379 2023-12-03 10:57:06.000000 dfvfs-20240115/tests/vfs/apfs_container_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2328 2023-12-03 10:57:07.000000 dfvfs-20240115/tests/vfs/apfs_directory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28404 2023-12-03 10:57:06.000000 dfvfs-20240115/tests/vfs/apfs_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4316 2023-12-03 10:57:06.000000 dfvfs-20240115/tests/vfs/apfs_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1883 2023-12-03 10:57:06.000000 dfvfs-20240115/tests/vfs/apm_directory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7699 2023-12-03 10:57:06.000000 dfvfs-20240115/tests/vfs/apm_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5973 2023-12-03 10:57:07.000000 dfvfs-20240115/tests/vfs/apm_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      545 2023-12-03 10:57:07.000000 dfvfs-20240115/tests/vfs/attribute.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6755 2023-12-03 10:57:06.000000 dfvfs-20240115/tests/vfs/bde_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2491 2023-12-03 10:57:06.000000 dfvfs-20240115/tests/vfs/bde_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4742 2023-12-03 10:57:06.000000 dfvfs-20240115/tests/vfs/compressed_stream_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2830 2023-12-03 10:57:06.000000 dfvfs-20240115/tests/vfs/compressed_stream_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1790 2023-12-03 10:57:07.000000 dfvfs-20240115/tests/vfs/cpio_directory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8419 2023-12-03 10:57:06.000000 dfvfs-20240115/tests/vfs/cpio_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3366 2023-12-03 10:57:06.000000 dfvfs-20240115/tests/vfs/cpio_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8349 2023-12-03 10:57:07.000000 dfvfs-20240115/tests/vfs/cs_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6279 2023-12-03 10:57:07.000000 dfvfs-20240115/tests/vfs/cs_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4606 2023-12-03 10:57:06.000000 dfvfs-20240115/tests/vfs/data_range_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2658 2023-12-03 10:57:06.000000 dfvfs-20240115/tests/vfs/data_range_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      883 2023-12-03 10:57:07.000000 dfvfs-20240115/tests/vfs/data_stream.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1379 2023-12-03 10:57:07.000000 dfvfs-20240115/tests/vfs/directory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3796 2023-12-03 10:57:06.000000 dfvfs-20240115/tests/vfs/encoded_stream_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2771 2023-12-03 10:57:06.000000 dfvfs-20240115/tests/vfs/encoded_stream_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4144 2023-12-03 10:57:06.000000 dfvfs-20240115/tests/vfs/encrypted_stream_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2979 2023-12-03 10:57:06.000000 dfvfs-20240115/tests/vfs/encrypted_stream_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2226 2023-12-03 10:57:07.000000 dfvfs-20240115/tests/vfs/ext_attribute.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2113 2023-12-03 10:57:07.000000 dfvfs-20240115/tests/vfs/ext_directory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23810 2023-12-03 10:57:07.000000 dfvfs-20240115/tests/vfs/ext_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3983 2023-12-03 10:57:07.000000 dfvfs-20240115/tests/vfs/ext_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      438 2023-12-03 10:57:07.000000 dfvfs-20240115/tests/vfs/extent.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2323 2023-12-03 10:57:07.000000 dfvfs-20240115/tests/vfs/fake_directory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10644 2023-12-03 10:57:06.000000 dfvfs-20240115/tests/vfs/fake_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2904 2023-12-03 10:57:06.000000 dfvfs-20240115/tests/vfs/fake_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2115 2023-12-03 10:57:07.000000 dfvfs-20240115/tests/vfs/fat_directory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13064 2023-12-03 10:57:07.000000 dfvfs-20240115/tests/vfs/fat_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4069 2023-12-03 10:57:07.000000 dfvfs-20240115/tests/vfs/fat_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11194 2023-12-03 10:57:06.000000 dfvfs-20240115/tests/vfs/file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2749 2023-12-03 10:57:06.000000 dfvfs-20240115/tests/vfs/file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1880 2023-12-03 10:57:07.000000 dfvfs-20240115/tests/vfs/gpt_directory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7790 2023-12-03 10:57:06.000000 dfvfs-20240115/tests/vfs/gpt_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6704 2023-12-03 10:57:06.000000 dfvfs-20240115/tests/vfs/gpt_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4674 2023-12-03 10:57:06.000000 dfvfs-20240115/tests/vfs/gzip_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2511 2023-12-03 10:57:06.000000 dfvfs-20240115/tests/vfs/gzip_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2239 2023-12-03 10:57:07.000000 dfvfs-20240115/tests/vfs/hfs_attribute.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4024 2023-12-03 10:57:07.000000 dfvfs-20240115/tests/vfs/hfs_data_stream.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2116 2023-12-03 10:57:07.000000 dfvfs-20240115/tests/vfs/hfs_directory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17357 2023-12-03 10:57:07.000000 dfvfs-20240115/tests/vfs/hfs_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4062 2023-12-03 10:57:07.000000 dfvfs-20240115/tests/vfs/hfs_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4814 2023-12-03 10:57:06.000000 dfvfs-20240115/tests/vfs/luksde_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2549 2023-12-03 10:57:06.000000 dfvfs-20240115/tests/vfs/luksde_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1880 2023-12-03 10:57:07.000000 dfvfs-20240115/tests/vfs/lvm_directory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8162 2023-12-03 10:57:06.000000 dfvfs-20240115/tests/vfs/lvm_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6462 2023-12-03 10:57:06.000000 dfvfs-20240115/tests/vfs/lvm_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9765 2023-12-03 10:57:07.000000 dfvfs-20240115/tests/vfs/ntfs_attibute.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4168 2023-12-03 10:57:07.000000 dfvfs-20240115/tests/vfs/ntfs_data_stream.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2139 2023-12-03 10:57:07.000000 dfvfs-20240115/tests/vfs/ntfs_directory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27468 2023-12-03 10:57:06.000000 dfvfs-20240115/tests/vfs/ntfs_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4115 2023-12-03 10:57:06.000000 dfvfs-20240115/tests/vfs/ntfs_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1602 2023-12-03 10:57:07.000000 dfvfs-20240115/tests/vfs/os_directory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9917 2023-12-03 10:57:06.000000 dfvfs-20240115/tests/vfs/os_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6182 2023-12-03 10:57:06.000000 dfvfs-20240115/tests/vfs/os_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2628 2023-12-03 10:57:07.000000 dfvfs-20240115/tests/vfs/sqlite_blob_directory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5588 2023-12-03 10:57:06.000000 dfvfs-20240115/tests/vfs/sqlite_blob_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3493 2023-12-03 10:57:06.000000 dfvfs-20240115/tests/vfs/sqlite_blob_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1766 2023-12-03 10:57:07.000000 dfvfs-20240115/tests/vfs/tar_directory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8767 2023-12-03 10:57:06.000000 dfvfs-20240115/tests/vfs/tar_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5544 2023-12-03 10:57:06.000000 dfvfs-20240115/tests/vfs/tar_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4017 2023-12-03 10:57:07.000000 dfvfs-20240115/tests/vfs/tsk_attribute.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11512 2023-12-03 10:57:07.000000 dfvfs-20240115/tests/vfs/tsk_data_stream.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1893 2023-12-03 10:57:07.000000 dfvfs-20240115/tests/vfs/tsk_directory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    95551 2023-12-03 10:57:06.000000 dfvfs-20240115/tests/vfs/tsk_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3941 2023-12-03 10:57:06.000000 dfvfs-20240115/tests/vfs/tsk_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1904 2023-12-03 10:57:07.000000 dfvfs-20240115/tests/vfs/tsk_partition_directory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22354 2023-12-03 10:57:06.000000 dfvfs-20240115/tests/vfs/tsk_partition_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6657 2023-12-03 10:57:06.000000 dfvfs-20240115/tests/vfs/tsk_partition_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1963 2023-12-03 10:57:07.000000 dfvfs-20240115/tests/vfs/vshadow_directory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8488 2023-12-03 10:57:06.000000 dfvfs-20240115/tests/vfs/vshadow_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6413 2023-12-03 10:57:06.000000 dfvfs-20240115/tests/vfs/vshadow_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2228 2023-12-03 10:57:07.000000 dfvfs-20240115/tests/vfs/xfs_attribute.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2112 2023-12-03 10:57:07.000000 dfvfs-20240115/tests/vfs/xfs_directory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13190 2023-12-03 10:57:07.000000 dfvfs-20240115/tests/vfs/xfs_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3985 2023-12-03 10:57:07.000000 dfvfs-20240115/tests/vfs/xfs_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1763 2023-12-03 10:57:07.000000 dfvfs-20240115/tests/vfs/zip_directory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13454 2023-12-03 10:57:06.000000 dfvfs-20240115/tests/vfs/zip_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5641 2023-12-03 10:57:06.000000 dfvfs-20240115/tests/vfs/zip_file_system.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-17 04:00:08.364552 dfvfs-20240115/tests/volume/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       24 2023-12-03 10:57:08.000000 dfvfs-20240115/tests/volume/__init__.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2698 2023-12-03 10:57:08.000000 dfvfs-20240115/tests/volume/apfs_volume_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2808 2023-12-03 10:57:08.000000 dfvfs-20240115/tests/volume/apm_volume_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2088 2023-12-03 10:57:08.000000 dfvfs-20240115/tests/volume/cs_volume_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1474 2023-12-03 10:57:08.000000 dfvfs-20240115/tests/volume/factory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2945 2023-12-03 10:57:08.000000 dfvfs-20240115/tests/volume/gpt_volume_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3695 2023-12-03 10:57:08.000000 dfvfs-20240115/tests/volume/lvm_volume_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8084 2023-12-03 10:57:08.000000 dfvfs-20240115/tests/volume/tsk_volume_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3543 2023-12-03 10:57:08.000000 dfvfs-20240115/tests/volume/vshadow_volume_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1097 2024-01-14 19:37:37.000000 dfvfs-20240115/tox.ini
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-17 04:00:08.367552 dfvfs-20240115/utils/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       24 2023-12-03 10:57:09.000000 dfvfs-20240115/utils/__init__.py
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)      422 2024-01-14 19:37:37.000000 dfvfs-20240115/utils/check_dependencies.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11583 2024-01-14 19:37:37.000000 dfvfs-20240115/utils/dependencies.py
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     2366 2023-12-03 10:57:09.000000 dfvfs-20240115/utils/generate_test_data_bsd.sh
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    14027 2023-12-03 10:57:08.000000 dfvfs-20240115/utils/generate_test_data_linux.sh
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4844 2023-12-03 10:57:08.000000 dfvfs-20240115/utils/generate_test_data_macos.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14212 2023-12-03 10:57:09.000000 dfvfs-20240115/utils/generate_test_data_windows.bat
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)      930 2023-12-06 04:29:50.000000 dfvfs-20240115/utils/update_release.sh
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-08 04:24:45.083782 dfvfs-20240505/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-08 04:24:45.016783 dfvfs-20240505/.github/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-08 04:24:45.020783 dfvfs-20240505/.github/workflows/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3423 2024-05-05 11:34:09.000000 dfvfs-20240505/.github/workflows/test_docker.yml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1882 2024-05-05 11:34:09.000000 dfvfs-20240505/.github/workflows/test_docs.yml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5700 2024-05-05 11:34:09.000000 dfvfs-20240505/.github/workflows/test_tox.yml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23352 2024-05-05 10:07:02.000000 dfvfs-20240505/.pylintrc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      322 2024-05-05 10:07:02.000000 dfvfs-20240505/.readthedocs.yaml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      149 2023-12-03 10:55:51.000000 dfvfs-20240505/.yamllint.yaml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1173 2023-12-03 10:55:50.000000 dfvfs-20240505/ACKNOWLEDGEMENTS
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      360 2023-12-03 10:55:51.000000 dfvfs-20240505/AUTHORS
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11358 2023-12-03 10:55:51.000000 dfvfs-20240505/LICENSE
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      632 2024-05-08 04:24:23.000000 dfvfs-20240505/MANIFEST.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      552 2023-12-03 10:55:50.000000 dfvfs-20240505/MANIFEST.test_data.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2125 2024-05-08 04:24:45.083782 dfvfs-20240505/PKG-INFO
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      473 2023-12-03 10:55:51.000000 dfvfs-20240505/README
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2321 2024-05-05 10:07:02.000000 dfvfs-20240505/appveyor.yml
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-08 04:24:45.016783 dfvfs-20240505/config/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-08 04:24:45.021782 dfvfs-20240505/config/appveyor/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1064 2024-05-05 11:34:09.000000 dfvfs-20240505/config/appveyor/install.ps1
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)      125 2024-05-05 10:07:02.000000 dfvfs-20240505/config/appveyor/install.sh
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)      620 2024-05-05 10:07:02.000000 dfvfs-20240505/config/appveyor/runtests.sh
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-08 04:24:45.021782 dfvfs-20240505/config/dpkg/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      168 2024-05-08 04:06:29.000000 dfvfs-20240505/config/dpkg/changelog
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       32 2023-12-03 10:56:42.000000 dfvfs-20240505/config/dpkg/clean
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        2 2024-05-05 10:07:02.000000 dfvfs-20240505/config/dpkg/compat
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1768 2024-05-05 11:34:09.000000 dfvfs-20240505/config/dpkg/control
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      948 2023-12-03 10:56:42.000000 dfvfs-20240505/config/dpkg/copyright
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)      122 2024-05-05 10:07:02.000000 dfvfs-20240505/config/dpkg/rules
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-08 04:24:45.021782 dfvfs-20240505/config/dpkg/source/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       12 2023-12-03 10:56:42.000000 dfvfs-20240505/config/dpkg/source/format
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-08 04:24:45.021782 dfvfs-20240505/config/pylint/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1673 2023-12-03 10:56:42.000000 dfvfs-20240505/config/pylint/spelling-private-dict
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5246 2024-05-05 11:34:09.000000 dfvfs-20240505/dependencies.ini
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-08 04:24:45.021782 dfvfs-20240505/dfvfs/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      278 2024-05-08 04:06:29.000000 dfvfs-20240505/dfvfs/__init__.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-08 04:24:45.025782 dfvfs-20240505/dfvfs/analyzer/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1488 2023-12-03 10:56:42.000000 dfvfs-20240505/dfvfs/analyzer/__init__.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13902 2023-12-03 10:56:42.000000 dfvfs-20240505/dfvfs/analyzer/analyzer.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2202 2024-01-28 16:33:12.000000 dfvfs-20240505/dfvfs/analyzer/analyzer_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      962 2023-12-03 10:56:42.000000 dfvfs-20240505/dfvfs/analyzer/apfs_analyzer_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1010 2023-12-03 10:56:42.000000 dfvfs-20240505/dfvfs/analyzer/apfs_container_analyzer_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1417 2023-12-03 10:56:42.000000 dfvfs-20240505/dfvfs/analyzer/apm_analyzer_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1120 2023-12-03 10:56:42.000000 dfvfs-20240505/dfvfs/analyzer/bde_analyzer_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1087 2023-12-03 10:56:42.000000 dfvfs-20240505/dfvfs/analyzer/bzip2_analyzer_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1404 2023-12-03 10:56:42.000000 dfvfs-20240505/dfvfs/analyzer/cpio_analyzer_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      978 2023-12-03 10:56:42.000000 dfvfs-20240505/dfvfs/analyzer/cs_analyzer_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1182 2023-12-03 10:56:42.000000 dfvfs-20240505/dfvfs/analyzer/ewf_analyzer_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1182 2023-12-03 10:56:42.000000 dfvfs-20240505/dfvfs/analyzer/ext_analyzer_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1547 2023-12-03 10:56:42.000000 dfvfs-20240505/dfvfs/analyzer/fat_analyzer_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1395 2023-12-03 10:56:42.000000 dfvfs-20240505/dfvfs/analyzer/gpt_analyzer_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      964 2023-12-03 10:56:42.000000 dfvfs-20240505/dfvfs/analyzer/gzip_analyzer_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1370 2023-12-03 10:56:42.000000 dfvfs-20240505/dfvfs/analyzer/hfs_analyzer_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      971 2023-12-03 10:56:42.000000 dfvfs-20240505/dfvfs/analyzer/luksde_analyzer_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1174 2023-12-03 10:56:42.000000 dfvfs-20240505/dfvfs/analyzer/lvm_analyzer_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1168 2023-12-03 10:56:42.000000 dfvfs-20240505/dfvfs/analyzer/modi_analyzer_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1186 2023-12-03 10:56:42.000000 dfvfs-20240505/dfvfs/analyzer/ntfs_analyzer_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1003 2023-12-03 10:56:42.000000 dfvfs-20240505/dfvfs/analyzer/phdi_analyzer_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1246 2023-12-03 10:56:42.000000 dfvfs-20240505/dfvfs/analyzer/qcow_analyzer_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5000 2024-01-28 16:33:12.000000 dfvfs-20240505/dfvfs/analyzer/specification.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1057 2023-12-03 10:56:42.000000 dfvfs-20240505/dfvfs/analyzer/tar_analyzer_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2300 2024-02-10 15:30:29.000000 dfvfs-20240505/dfvfs/analyzer/tsk_analyzer_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1040 2023-12-03 10:56:42.000000 dfvfs-20240505/dfvfs/analyzer/tsk_partition_analyzer_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1192 2023-12-03 10:56:42.000000 dfvfs-20240505/dfvfs/analyzer/vhdi_analyzer_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1194 2023-12-03 10:56:42.000000 dfvfs-20240505/dfvfs/analyzer/vmdk_analyzer_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1071 2023-12-03 10:56:42.000000 dfvfs-20240505/dfvfs/analyzer/vshadow_analyzer_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      955 2023-12-03 10:56:42.000000 dfvfs-20240505/dfvfs/analyzer/xfs_analyzer_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      968 2023-12-03 10:56:42.000000 dfvfs-20240505/dfvfs/analyzer/xz_analyzer_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      950 2023-12-03 10:56:42.000000 dfvfs-20240505/dfvfs/analyzer/zip_analyzer_helper.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-08 04:24:45.025782 dfvfs-20240505/dfvfs/compression/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      247 2023-12-03 10:56:42.000000 dfvfs-20240505/dfvfs/compression/__init__.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1355 2023-12-03 10:56:42.000000 dfvfs-20240505/dfvfs/compression/bzip2_decompressor.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      437 2023-12-03 10:56:42.000000 dfvfs-20240505/dfvfs/compression/decompressor.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2286 2023-12-03 10:56:42.000000 dfvfs-20240505/dfvfs/compression/manager.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2139 2023-12-03 10:56:42.000000 dfvfs-20240505/dfvfs/compression/xz_decompressor.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2118 2023-12-03 10:56:42.000000 dfvfs-20240505/dfvfs/compression/zlib_decompressor.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-08 04:24:45.026783 dfvfs-20240505/dfvfs/credentials/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      313 2023-12-03 10:56:42.000000 dfvfs-20240505/dfvfs/credentials/__init__.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      545 2023-12-03 10:56:42.000000 dfvfs-20240505/dfvfs/credentials/apfs_credentials.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      646 2023-12-03 10:56:42.000000 dfvfs-20240505/dfvfs/credentials/bde_credentials.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      562 2023-12-03 10:56:42.000000 dfvfs-20240505/dfvfs/credentials/credentials.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      544 2023-12-03 10:56:42.000000 dfvfs-20240505/dfvfs/credentials/cs_credentials.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      497 2023-12-03 10:56:42.000000 dfvfs-20240505/dfvfs/credentials/encrypted_stream_credentials.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2696 2024-01-28 16:33:12.000000 dfvfs-20240505/dfvfs/credentials/keychain.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      498 2023-12-03 10:56:42.000000 dfvfs-20240505/dfvfs/credentials/luksde_credentials.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1902 2023-12-03 10:56:42.000000 dfvfs-20240505/dfvfs/credentials/manager.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-08 04:24:45.026783 dfvfs-20240505/dfvfs/encoding/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      191 2023-12-03 10:56:42.000000 dfvfs-20240505/dfvfs/encoding/__init__.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      967 2023-12-03 10:56:42.000000 dfvfs-20240505/dfvfs/encoding/base16_decoder.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      967 2023-12-03 10:56:42.000000 dfvfs-20240505/dfvfs/encoding/base32_decoder.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1198 2023-12-03 10:56:42.000000 dfvfs-20240505/dfvfs/encoding/base64_decoder.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      392 2023-12-03 10:56:42.000000 dfvfs-20240505/dfvfs/encoding/decoder.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1955 2023-12-03 10:56:42.000000 dfvfs-20240505/dfvfs/encoding/manager.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-08 04:24:45.027783 dfvfs-20240505/dfvfs/encryption/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      245 2024-01-14 08:46:30.000000 dfvfs-20240505/dfvfs/encryption/__init__.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3323 2024-01-15 06:55:06.000000 dfvfs-20240505/dfvfs/encryption/aes_decrypter.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3531 2024-01-15 06:55:06.000000 dfvfs-20240505/dfvfs/encryption/blowfish_decrypter.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      953 2024-01-15 06:55:06.000000 dfvfs-20240505/dfvfs/encryption/decrypter.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3491 2024-01-15 06:55:06.000000 dfvfs-20240505/dfvfs/encryption/des3_decrypter.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2274 2023-12-03 10:56:42.000000 dfvfs-20240505/dfvfs/encryption/manager.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1339 2024-01-15 06:55:06.000000 dfvfs-20240505/dfvfs/encryption/rc4_decrypter.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-08 04:24:45.030783 dfvfs-20240505/dfvfs/file_io/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       24 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/file_io/__init__.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3961 2024-01-28 16:33:12.000000 dfvfs-20240505/dfvfs/file_io/apfs_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5561 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/file_io/apm_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/file_io/bde_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9503 2024-01-28 16:33:12.000000 dfvfs-20240505/dfvfs/file_io/compressed_stream_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4645 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/file_io/cpio_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4663 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/file_io/cs_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5994 2024-01-28 16:33:12.000000 dfvfs-20240505/dfvfs/file_io/data_range_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9664 2024-01-28 16:33:12.000000 dfvfs-20240505/dfvfs/file_io/encoded_stream_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10708 2024-01-28 16:33:12.000000 dfvfs-20240505/dfvfs/file_io/encrypted_stream_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2710 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/file_io/ewf_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3949 2024-01-28 16:33:12.000000 dfvfs-20240505/dfvfs/file_io/ext_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4175 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/file_io/fake_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4399 2024-01-28 16:33:12.000000 dfvfs-20240505/dfvfs/file_io/fat_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5057 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/file_io/file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4157 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/file_io/file_object_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5569 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/file_io/gpt_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2666 2024-01-28 16:33:12.000000 dfvfs-20240505/dfvfs/file_io/gzip_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4502 2024-01-28 16:33:12.000000 dfvfs-20240505/dfvfs/file_io/hfs_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1272 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/file_io/luksde_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3978 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/file_io/lvm_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1856 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/file_io/modi_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4540 2023-12-03 10:56:42.000000 dfvfs-20240505/dfvfs/file_io/ntfs_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6180 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/file_io/os_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4378 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/file_io/phdi_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4074 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/file_io/qcow_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2733 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/file_io/raw_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8363 2023-12-27 09:22:15.000000 dfvfs-20240505/dfvfs/file_io/sqlite_blob_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4775 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/file_io/tar_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7991 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/file_io/tsk_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2370 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/file_io/tsk_partition_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4313 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/file_io/vhdi_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4201 2023-12-03 10:56:42.000000 dfvfs-20240505/dfvfs/file_io/vmdk_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4106 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/file_io/vshadow_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3942 2024-01-28 16:33:12.000000 dfvfs-20240505/dfvfs/file_io/xfs_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9026 2023-12-03 10:56:42.000000 dfvfs-20240505/dfvfs/file_io/zip_file_io.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-08 04:24:45.031782 dfvfs-20240505/dfvfs/helpers/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       24 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/helpers/__init__.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29440 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/helpers/command_line.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2093 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/helpers/data_slice.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3992 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/helpers/fake_file_system_builder.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22177 2024-01-28 12:54:32.000000 dfvfs-20240505/dfvfs/helpers/file_system_searcher.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30817 2024-01-28 16:33:12.000000 dfvfs-20240505/dfvfs/helpers/source_scanner.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6081 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/helpers/text_file.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28568 2024-03-09 16:19:59.000000 dfvfs-20240505/dfvfs/helpers/volume_scanner.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9517 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/helpers/windows_path_resolver.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-08 04:24:45.033783 dfvfs-20240505/dfvfs/lib/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       24 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/lib/__init__.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      835 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/lib/apfs_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      722 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/lib/apm_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1710 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/lib/bde_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10516 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/lib/cpio.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4230 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/lib/cpio.yaml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1677 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/lib/cs_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3532 2024-01-28 12:27:46.000000 dfvfs-20240505/dfvfs/lib/data_format.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      710 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/lib/decorators.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4759 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/lib/definitions.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1053 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/lib/errors.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3502 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/lib/ewf_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2345 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/lib/glob2regex.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19651 2024-01-28 16:33:12.000000 dfvfs-20240505/dfvfs/lib/gzipfile.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1489 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/lib/gzipfile.yaml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1160 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/lib/luksde_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      866 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/lib/lvm_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12570 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/lib/raw_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5970 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/lib/sqlite_database.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1775 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/lib/tsk_image.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5460 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/lib/tsk_partition.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      745 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/lib/vshadow_helper.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-08 04:24:45.033783 dfvfs-20240505/dfvfs/mount/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       24 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/mount/__init__.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2036 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/mount/manager.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-08 04:24:45.037783 dfvfs-20240505/dfvfs/path/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1450 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/path/__init__.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1564 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/path/apfs_container_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1547 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/path/apfs_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1473 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/path/apm_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1769 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/path/bde_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1387 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/path/compressed_stream_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      965 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/path/cpio_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2397 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/path/cs_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1517 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/path/data_range_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1332 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/path/encoded_stream_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2414 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/path/encrypted_stream_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      777 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/path/ewf_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1475 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/path/ext_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3742 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/path/factory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      940 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/path/fake_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1560 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/path/fat_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1474 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/path/gpt_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      782 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/path/gzip_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1932 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/path/hfs_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      923 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/path/location_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1217 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/path/luksde_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1482 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/path/lvm_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      798 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/path/modi_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1102 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/path/mount_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2364 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/path/ntfs_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1412 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/path/os_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4043 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/path/path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      784 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/path/phdi_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      779 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/path/qcow_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      800 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/path/raw_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2964 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/path/sqlite_blob_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      947 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/path/tar_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1777 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/path/tsk_partition_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1943 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/path/tsk_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      810 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/path/vhdi_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      784 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/path/vmdk_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1499 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/path/vshadow_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1475 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/path/xfs_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      978 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/path/zip_path_spec.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-08 04:24:45.037783 dfvfs-20240505/dfvfs/resolver/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       24 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/resolver/__init__.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4365 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/resolver/context.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6142 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/resolver/resolver.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-08 04:24:45.040783 dfvfs-20240505/dfvfs/resolver_helpers/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2813 2023-12-03 10:56:44.000000 dfvfs-20240505/dfvfs/resolver_helpers/__init__.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      904 2023-12-03 10:56:44.000000 dfvfs-20240505/dfvfs/resolver_helpers/apfs_container_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1195 2023-12-03 10:56:44.000000 dfvfs-20240505/dfvfs/resolver_helpers/apfs_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1206 2023-12-03 10:56:44.000000 dfvfs-20240505/dfvfs/resolver_helpers/apm_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1195 2023-12-03 10:56:44.000000 dfvfs-20240505/dfvfs/resolver_helpers/bde_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1329 2023-12-03 10:56:44.000000 dfvfs-20240505/dfvfs/resolver_helpers/compressed_stream_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1246 2023-12-03 10:56:44.000000 dfvfs-20240505/dfvfs/resolver_helpers/cpio_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1198 2023-12-03 10:56:44.000000 dfvfs-20240505/dfvfs/resolver_helpers/cs_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1252 2023-12-03 10:56:44.000000 dfvfs-20240505/dfvfs/resolver_helpers/data_range_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1296 2023-12-03 10:56:44.000000 dfvfs-20240505/dfvfs/resolver_helpers/encoded_stream_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1318 2023-12-03 10:56:44.000000 dfvfs-20240505/dfvfs/resolver_helpers/encrypted_stream_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      824 2023-12-03 10:56:44.000000 dfvfs-20240505/dfvfs/resolver_helpers/ewf_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1184 2023-12-03 10:56:44.000000 dfvfs-20240505/dfvfs/resolver_helpers/ext_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      522 2023-12-03 10:56:44.000000 dfvfs-20240505/dfvfs/resolver_helpers/fake_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1184 2023-12-03 10:56:44.000000 dfvfs-20240505/dfvfs/resolver_helpers/fat_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1207 2023-12-03 10:56:44.000000 dfvfs-20240505/dfvfs/resolver_helpers/gpt_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1205 2023-12-03 10:56:44.000000 dfvfs-20240505/dfvfs/resolver_helpers/gzip_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1184 2023-12-03 10:56:44.000000 dfvfs-20240505/dfvfs/resolver_helpers/hfs_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2023-12-03 10:56:44.000000 dfvfs-20240505/dfvfs/resolver_helpers/luksde_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1209 2023-12-03 10:56:44.000000 dfvfs-20240505/dfvfs/resolver_helpers/lvm_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1928 2023-12-03 10:56:44.000000 dfvfs-20240505/dfvfs/resolver_helpers/manager.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      846 2023-12-03 10:56:45.000000 dfvfs-20240505/dfvfs/resolver_helpers/modi_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1195 2023-12-03 10:56:44.000000 dfvfs-20240505/dfvfs/resolver_helpers/ntfs_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1201 2023-12-03 10:56:44.000000 dfvfs-20240505/dfvfs/resolver_helpers/os_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      832 2023-12-03 10:56:45.000000 dfvfs-20240505/dfvfs/resolver_helpers/phdi_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      832 2023-12-03 10:56:44.000000 dfvfs-20240505/dfvfs/resolver_helpers/qcow_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      838 2023-12-03 10:56:44.000000 dfvfs-20240505/dfvfs/resolver_helpers/raw_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1717 2023-12-03 10:56:44.000000 dfvfs-20240505/dfvfs/resolver_helpers/resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1300 2023-12-03 10:56:44.000000 dfvfs-20240505/dfvfs/resolver_helpers/sqlite_blob_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1184 2023-12-03 10:56:44.000000 dfvfs-20240505/dfvfs/resolver_helpers/tar_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1312 2023-12-03 10:56:44.000000 dfvfs-20240505/dfvfs/resolver_helpers/tsk_partition_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1208 2023-12-03 10:56:44.000000 dfvfs-20240505/dfvfs/resolver_helpers/tsk_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      830 2023-12-03 10:56:44.000000 dfvfs-20240505/dfvfs/resolver_helpers/vhdi_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      832 2023-12-03 10:56:44.000000 dfvfs-20240505/dfvfs/resolver_helpers/vmdk_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1246 2023-12-03 10:56:44.000000 dfvfs-20240505/dfvfs/resolver_helpers/vshadow_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1184 2023-12-03 10:56:44.000000 dfvfs-20240505/dfvfs/resolver_helpers/xfs_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1184 2023-12-03 10:56:44.000000 dfvfs-20240505/dfvfs/resolver_helpers/zip_resolver_helper.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-08 04:24:45.040783 dfvfs-20240505/dfvfs/serializer/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       24 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/serializer/__init__.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5458 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/serializer/json_serializer.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      957 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/serializer/serializer.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-08 04:24:45.049782 dfvfs-20240505/dfvfs/vfs/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       24 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/vfs/__init__.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3622 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/vfs/apfs_attribute.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1225 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/vfs/apfs_container_directory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4737 2024-01-28 16:33:12.000000 dfvfs-20240505/dfvfs/vfs/apfs_container_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5539 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/vfs/apfs_container_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/vfs/apfs_directory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8895 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/vfs/apfs_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6044 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/vfs/apfs_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1331 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/vfs/apm_directory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3577 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/vfs/apm_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4352 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/vfs/apm_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2064 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/vfs/attribute.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2188 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/vfs/bde_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2758 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/vfs/bde_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1637 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/vfs/compressed_stream_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2621 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/vfs/compressed_stream_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/vfs/cpio_directory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7019 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/vfs/cpio_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4635 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/vfs/cpio_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1112 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/vfs/cs_directory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4353 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/vfs/cs_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5012 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/vfs/cs_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1335 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/vfs/data_range_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2781 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/vfs/data_range_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      859 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/vfs/data_stream.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1015 2024-01-28 16:33:12.000000 dfvfs-20240505/dfvfs/vfs/directory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/vfs/encoded_stream_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2534 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/vfs/encoded_stream_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1625 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/vfs/encrypted_stream_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2699 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/vfs/encrypted_stream_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3601 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/vfs/ext_attribute.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1434 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/vfs/ext_directory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9823 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/vfs/ext_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5159 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/vfs/ext_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      844 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/vfs/extent.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1212 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/vfs/fake_directory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4684 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/vfs/fake_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5004 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/vfs/fake_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1437 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/vfs/fat_directory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7675 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/vfs/fat_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5634 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/vfs/fat_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12654 2024-01-28 16:33:12.000000 dfvfs-20240505/dfvfs/vfs/file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7136 2024-02-11 08:22:33.000000 dfvfs-20240505/dfvfs/vfs/file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1085 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/vfs/gpt_directory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3656 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/vfs/gpt_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5257 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/vfs/gpt_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1849 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/vfs/gzip_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1019 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/vfs/gzip_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3601 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/vfs/hfs_attribute.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1378 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/vfs/hfs_data_stream.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1437 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/vfs/hfs_directory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10348 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/vfs/hfs_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5316 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/vfs/hfs_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1944 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/vfs/luksde_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2856 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/vfs/luksde_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1129 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/vfs/lvm_directory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3835 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/vfs/lvm_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4750 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/vfs/lvm_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5041 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/vfs/ntfs_attribute.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1411 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/vfs/ntfs_data_stream.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1838 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/vfs/ntfs_directory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12181 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/vfs/ntfs_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5882 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/vfs/ntfs_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3067 2024-01-06 18:42:17.000000 dfvfs-20240505/dfvfs/vfs/os_attribute.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1662 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/vfs/os_directory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9581 2024-04-07 13:04:01.000000 dfvfs-20240505/dfvfs/vfs/os_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6345 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/vfs/os_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      665 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/vfs/root_only_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1699 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/vfs/root_only_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1853 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/vfs/sqlite_blob_directory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4202 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/vfs/sqlite_blob_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3520 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/vfs/sqlite_blob_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2093 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/vfs/tar_directory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6442 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/vfs/tar_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5180 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/vfs/tar_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4281 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/vfs/tsk_attribute.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3018 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/vfs/tsk_data_stream.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4156 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/vfs/tsk_directory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27761 2023-12-29 05:21:46.000000 dfvfs-20240505/dfvfs/vfs/tsk_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7175 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/vfs/tsk_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1865 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/vfs/tsk_partition_directory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4278 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/vfs/tsk_partition_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4196 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/vfs/tsk_partition_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1128 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/vfs/vshadow_directory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4224 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/vfs/vshadow_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4412 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/vfs/vshadow_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3601 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/vfs/xfs_attribute.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1434 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/vfs/xfs_directory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8567 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/vfs/xfs_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5313 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/vfs/xfs_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2261 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/vfs/zip_directory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6332 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/vfs/zip_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4975 2023-12-03 10:56:43.000000 dfvfs-20240505/dfvfs/vfs/zip_file_system.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-08 04:24:45.049782 dfvfs-20240505/dfvfs/volume/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      375 2023-12-03 10:56:44.000000 dfvfs-20240505/dfvfs/volume/__init__.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1563 2023-12-03 10:56:44.000000 dfvfs-20240505/dfvfs/volume/apfs_volume_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1421 2023-12-03 10:56:44.000000 dfvfs-20240505/dfvfs/volume/apm_volume_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1513 2023-12-03 10:56:44.000000 dfvfs-20240505/dfvfs/volume/cs_volume_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1710 2023-12-03 10:56:44.000000 dfvfs-20240505/dfvfs/volume/factory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1427 2023-12-03 10:56:44.000000 dfvfs-20240505/dfvfs/volume/gpt_volume_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1539 2023-12-03 10:56:44.000000 dfvfs-20240505/dfvfs/volume/lvm_volume_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3054 2023-12-03 10:56:44.000000 dfvfs-20240505/dfvfs/volume/tsk_volume_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7770 2024-01-28 16:33:12.000000 dfvfs-20240505/dfvfs/volume/volume_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2017 2023-12-03 10:56:44.000000 dfvfs-20240505/dfvfs/volume/vshadow_volume_system.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-08 04:24:45.083782 dfvfs-20240505/dfvfs.egg-info/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2125 2024-05-08 04:24:44.000000 dfvfs-20240505/dfvfs.egg-info/PKG-INFO
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20887 2024-05-08 04:24:45.000000 dfvfs-20240505/dfvfs.egg-info/SOURCES.txt
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        1 2024-05-08 04:24:44.000000 dfvfs-20240505/dfvfs.egg-info/dependency_links.txt
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      763 2024-05-08 04:24:44.000000 dfvfs-20240505/dfvfs.egg-info/requires.txt
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        6 2024-05-08 04:24:44.000000 dfvfs-20240505/dfvfs.egg-info/top_level.txt
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1017 2023-12-03 10:55:50.000000 dfvfs-20240505/dfvfs.ini
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-08 04:24:45.050782 dfvfs-20240505/docs/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5075 2024-05-05 10:07:02.000000 dfvfs-20240505/docs/conf.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1453 2023-12-03 10:57:15.000000 dfvfs-20240505/docs/index.rst
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      118 2024-05-05 10:07:02.000000 dfvfs-20240505/docs/requirements.txt
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-08 04:24:45.050782 dfvfs-20240505/docs/sources/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3182 2023-12-03 10:57:15.000000 dfvfs-20240505/docs/sources/Code-snippets.md
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14179 2023-12-03 10:57:15.000000 dfvfs-20240505/docs/sources/Path-specifications.md
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4117 2024-01-15 06:55:06.000000 dfvfs-20240505/docs/sources/Supported-formats.md
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-08 04:24:45.051782 dfvfs-20240505/docs/sources/api/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6275 2023-12-03 10:57:16.000000 dfvfs-20240505/docs/sources/api/dfvfs.analyzer.rst
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1125 2023-12-03 10:57:15.000000 dfvfs-20240505/docs/sources/api/dfvfs.compression.rst
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1704 2023-12-03 10:57:16.000000 dfvfs-20240505/docs/sources/api/dfvfs.credentials.rst
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1032 2023-12-03 10:57:15.000000 dfvfs-20240505/docs/sources/api/dfvfs.encoding.rst
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1264 2023-12-03 10:57:16.000000 dfvfs-20240505/docs/sources/api/dfvfs.encryption.rst
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6310 2023-12-03 10:57:16.000000 dfvfs-20240505/docs/sources/api/dfvfs.file_io.rst
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1629 2023-12-03 10:57:16.000000 dfvfs-20240505/docs/sources/api/dfvfs.helpers.rst
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3042 2023-12-03 10:57:16.000000 dfvfs-20240505/docs/sources/api/dfvfs.lib.rst
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      325 2023-12-03 10:57:15.000000 dfvfs-20240505/docs/sources/api/dfvfs.mount.rst
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6712 2023-12-03 10:57:15.000000 dfvfs-20240505/docs/sources/api/dfvfs.path.rst
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      501 2023-12-03 10:57:16.000000 dfvfs-20240505/docs/sources/api/dfvfs.resolver.rst
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8397 2023-12-03 10:57:15.000000 dfvfs-20240505/docs/sources/api/dfvfs.resolver_helpers.rst
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      461 2023-12-03 10:57:16.000000 dfvfs-20240505/docs/sources/api/dfvfs.rst
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      551 2023-12-03 10:57:16.000000 dfvfs-20240505/docs/sources/api/dfvfs.serializer.rst
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15898 2023-12-03 10:57:16.000000 dfvfs-20240505/docs/sources/api/dfvfs.vfs.rst
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1793 2023-12-03 10:57:15.000000 dfvfs-20240505/docs/sources/api/dfvfs.volume.rst
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       52 2023-12-03 10:57:15.000000 dfvfs-20240505/docs/sources/api/modules.rst
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-08 04:24:45.052782 dfvfs-20240505/docs/sources/developer/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6837 2023-12-03 10:57:16.000000 dfvfs-20240505/docs/sources/developer/Adding-new-type.md
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5979 2023-12-03 10:57:16.000000 dfvfs-20240505/docs/sources/developer/Helpers.md
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3991 2023-12-03 10:57:16.000000 dfvfs-20240505/docs/sources/developer/Internals.md
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      447 2023-12-03 10:57:16.000000 dfvfs-20240505/docs/sources/developer/Testing.md
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      398 2023-12-03 10:57:16.000000 dfvfs-20240505/docs/sources/developer/index.rst
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-08 04:24:45.052782 dfvfs-20240505/docs/sources/user/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1602 2024-02-10 15:30:29.000000 dfvfs-20240505/docs/sources/user/Installation-instructions.md
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      282 2023-12-03 10:57:16.000000 dfvfs-20240505/docs/sources/user/index.rst
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      296 2024-05-05 10:07:02.000000 dfvfs-20240505/pyproject.toml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      821 2024-05-05 11:34:09.000000 dfvfs-20240505/requirements.txt
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     1018 2023-12-03 10:55:50.000000 dfvfs-20240505/run_tests.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1179 2024-05-08 04:24:45.084782 dfvfs-20240505/setup.cfg
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)      128 2024-05-05 10:07:02.000000 dfvfs-20240505/setup.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2023-12-03 10:55:51.000000 dfvfs-20240505/test_dependencies.ini
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 10:07:02.000000 dfvfs-20240505/test_requirements.txt
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-08 04:24:45.052782 dfvfs-20240505/tests/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       24 2023-12-03 10:57:02.000000 dfvfs-20240505/tests/__init__.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-08 04:24:45.053782 dfvfs-20240505/tests/analyzer/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       24 2023-12-03 10:57:03.000000 dfvfs-20240505/tests/analyzer/__init__.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18453 2023-12-03 10:57:03.000000 dfvfs-20240505/tests/analyzer/analyzer.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      912 2023-12-03 10:57:03.000000 dfvfs-20240505/tests/analyzer/specification.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-08 04:24:45.053782 dfvfs-20240505/tests/compression/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       24 2023-12-03 10:57:03.000000 dfvfs-20240505/tests/compression/__init__.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1231 2023-12-03 10:57:03.000000 dfvfs-20240505/tests/compression/bzip2_decompressor.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2083 2023-12-03 10:57:03.000000 dfvfs-20240505/tests/compression/manager.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      224 2023-12-03 10:57:03.000000 dfvfs-20240505/tests/compression/test_lib.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2425 2023-12-03 10:57:03.000000 dfvfs-20240505/tests/compression/xz_decompressor.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1646 2023-12-03 10:57:03.000000 dfvfs-20240505/tests/compression/zlib_decompressor.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-08 04:24:45.054782 dfvfs-20240505/tests/credentials/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       24 2023-12-03 10:57:08.000000 dfvfs-20240505/tests/credentials/__init__.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      543 2023-12-03 10:57:08.000000 dfvfs-20240505/tests/credentials/apfs_credentials.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      555 2023-12-03 10:57:08.000000 dfvfs-20240505/tests/credentials/bde_credentials.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      475 2023-12-03 10:57:08.000000 dfvfs-20240505/tests/credentials/credentials.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      521 2023-12-03 10:57:08.000000 dfvfs-20240505/tests/credentials/cs_credentials.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      562 2023-12-03 10:57:08.000000 dfvfs-20240505/tests/credentials/encrypted_stream_credentials.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1344 2023-12-03 10:57:08.000000 dfvfs-20240505/tests/credentials/keychain.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      545 2023-12-03 10:57:08.000000 dfvfs-20240505/tests/credentials/luksde_credentials.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2146 2023-12-03 10:57:08.000000 dfvfs-20240505/tests/credentials/manager.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-08 04:24:45.054782 dfvfs-20240505/tests/encoding/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       24 2023-12-03 10:57:03.000000 dfvfs-20240505/tests/encoding/__init__.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      804 2023-12-03 10:57:03.000000 dfvfs-20240505/tests/encoding/base16_decoder.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      804 2023-12-03 10:57:03.000000 dfvfs-20240505/tests/encoding/base32_decoder.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      801 2023-12-03 10:57:03.000000 dfvfs-20240505/tests/encoding/base64_decoder.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1852 2023-12-03 10:57:03.000000 dfvfs-20240505/tests/encoding/manager.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      214 2023-12-03 10:57:03.000000 dfvfs-20240505/tests/encoding/test_lib.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-08 04:24:45.055782 dfvfs-20240505/tests/encryption/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       24 2023-12-03 10:57:08.000000 dfvfs-20240505/tests/encryption/__init__.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3449 2024-01-15 06:55:06.000000 dfvfs-20240505/tests/encryption/aes_decrypter.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3255 2024-01-15 06:55:06.000000 dfvfs-20240505/tests/encryption/blowfish_decrypter.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      559 2024-01-15 06:55:06.000000 dfvfs-20240505/tests/encryption/decrypter.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3449 2024-01-15 06:55:06.000000 dfvfs-20240505/tests/encryption/des3_decrypter.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2302 2023-12-03 10:57:08.000000 dfvfs-20240505/tests/encryption/manager.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1136 2024-01-14 11:15:00.000000 dfvfs-20240505/tests/encryption/rc4_decrypter.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      218 2023-12-03 10:57:08.000000 dfvfs-20240505/tests/encryption/test_lib.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-08 04:24:45.058782 dfvfs-20240505/tests/file_io/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       24 2023-12-03 10:57:04.000000 dfvfs-20240505/tests/file_io/__init__.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4656 2023-12-03 10:57:04.000000 dfvfs-20240505/tests/file_io/apfs_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3037 2023-12-03 10:57:04.000000 dfvfs-20240505/tests/file_io/apm_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6036 2023-12-03 10:57:04.000000 dfvfs-20240505/tests/file_io/bde_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9395 2023-12-03 10:57:04.000000 dfvfs-20240505/tests/file_io/compressed_stream_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6471 2023-12-03 10:57:04.000000 dfvfs-20240505/tests/file_io/cpio_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9118 2023-12-03 10:57:04.000000 dfvfs-20240505/tests/file_io/cs_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2793 2023-12-03 10:57:04.000000 dfvfs-20240505/tests/file_io/data_range_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6975 2023-12-03 10:57:04.000000 dfvfs-20240505/tests/file_io/encoded_stream_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14381 2023-12-03 10:57:04.000000 dfvfs-20240505/tests/file_io/encrypted_stream_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3128 2023-12-03 10:57:04.000000 dfvfs-20240505/tests/file_io/ewf_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4396 2023-12-03 10:57:04.000000 dfvfs-20240505/tests/file_io/ext_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3463 2023-12-03 10:57:04.000000 dfvfs-20240505/tests/file_io/fake_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3104 2023-12-03 10:57:04.000000 dfvfs-20240505/tests/file_io/fat_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1552 2023-12-03 10:57:04.000000 dfvfs-20240505/tests/file_io/gpt_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4168 2023-12-03 10:57:04.000000 dfvfs-20240505/tests/file_io/gzip_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3512 2023-12-03 10:57:04.000000 dfvfs-20240505/tests/file_io/hfs_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3659 2023-12-03 10:57:04.000000 dfvfs-20240505/tests/file_io/luksde_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6235 2023-12-03 10:57:04.000000 dfvfs-20240505/tests/file_io/lvm_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5726 2023-12-03 10:57:04.000000 dfvfs-20240505/tests/file_io/modi_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3082 2023-12-03 10:57:04.000000 dfvfs-20240505/tests/file_io/ntfs_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5213 2023-12-03 10:57:04.000000 dfvfs-20240505/tests/file_io/os_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3042 2023-12-03 10:57:04.000000 dfvfs-20240505/tests/file_io/phdi_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1722 2023-12-03 10:57:04.000000 dfvfs-20240505/tests/file_io/qcow_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2868 2023-12-03 10:57:04.000000 dfvfs-20240505/tests/file_io/raw_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3603 2023-12-03 10:57:04.000000 dfvfs-20240505/tests/file_io/sqlite_blob_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1843 2023-12-03 10:57:04.000000 dfvfs-20240505/tests/file_io/tar_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33122 2023-12-03 10:57:04.000000 dfvfs-20240505/tests/file_io/test_lib.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12616 2023-12-03 10:57:04.000000 dfvfs-20240505/tests/file_io/tsk_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1126 2023-12-03 10:57:04.000000 dfvfs-20240505/tests/file_io/tsk_partition_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16839 2023-12-03 10:57:04.000000 dfvfs-20240505/tests/file_io/vhdi_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1721 2023-12-03 10:57:04.000000 dfvfs-20240505/tests/file_io/vmdk_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5037 2023-12-03 10:57:04.000000 dfvfs-20240505/tests/file_io/vshadow_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4369 2023-12-03 10:57:04.000000 dfvfs-20240505/tests/file_io/xfs_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1895 2023-12-03 10:57:04.000000 dfvfs-20240505/tests/file_io/zip_file_io.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-08 04:24:45.059782 dfvfs-20240505/tests/helpers/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       24 2023-12-03 10:57:04.000000 dfvfs-20240505/tests/helpers/__init__.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39320 2023-12-03 10:57:04.000000 dfvfs-20240505/tests/helpers/command_line.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2714 2023-12-03 10:57:04.000000 dfvfs-20240505/tests/helpers/data_slice.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2644 2023-12-03 10:57:04.000000 dfvfs-20240505/tests/helpers/fake_file_system_builder.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26712 2023-12-03 10:57:04.000000 dfvfs-20240505/tests/helpers/file_system_searcher.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    36588 2023-12-03 10:57:04.000000 dfvfs-20240505/tests/helpers/source_scanner.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8964 2023-12-03 10:57:04.000000 dfvfs-20240505/tests/helpers/text_file.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    38545 2023-12-03 10:57:04.000000 dfvfs-20240505/tests/helpers/volume_scanner.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6744 2023-12-03 10:57:04.000000 dfvfs-20240505/tests/helpers/windows_path_resolver.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-08 04:24:45.060782 dfvfs-20240505/tests/lib/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       24 2023-12-03 10:57:05.000000 dfvfs-20240505/tests/lib/__init__.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3221 2023-12-03 10:57:05.000000 dfvfs-20240505/tests/lib/apfs_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9118 2023-12-03 10:57:05.000000 dfvfs-20240505/tests/lib/cpio.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1756 2023-12-03 10:57:05.000000 dfvfs-20240505/tests/lib/cs_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16350 2023-12-03 10:57:05.000000 dfvfs-20240505/tests/lib/ewf_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1923 2023-12-03 10:57:05.000000 dfvfs-20240505/tests/lib/glob2regex.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5410 2023-12-03 10:57:05.000000 dfvfs-20240505/tests/lib/gzipfile.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1806 2023-12-03 10:57:05.000000 dfvfs-20240505/tests/lib/lvm_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20600 2023-12-03 10:57:05.000000 dfvfs-20240505/tests/lib/raw_helper.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-08 04:24:45.060782 dfvfs-20240505/tests/mount/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       24 2023-12-03 10:57:05.000000 dfvfs-20240505/tests/mount/__init__.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3950 2023-12-03 10:57:05.000000 dfvfs-20240505/tests/mount/manager.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-08 04:24:45.063782 dfvfs-20240505/tests/path/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       24 2023-12-03 10:57:05.000000 dfvfs-20240505/tests/path/__init__.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2784 2023-12-03 10:57:05.000000 dfvfs-20240505/tests/path/apfs_container_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2372 2023-12-03 10:57:05.000000 dfvfs-20240505/tests/path/apfs_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2457 2023-12-03 10:57:05.000000 dfvfs-20240505/tests/path/apm_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1090 2023-12-03 10:57:05.000000 dfvfs-20240505/tests/path/bde_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1601 2023-12-03 10:57:05.000000 dfvfs-20240505/tests/path/compressed_stream_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1335 2023-12-03 10:57:05.000000 dfvfs-20240505/tests/path/cpio_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2429 2023-12-03 10:57:05.000000 dfvfs-20240505/tests/path/cs_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1752 2023-12-03 10:57:05.000000 dfvfs-20240505/tests/path/data_range_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1538 2023-12-03 10:57:05.000000 dfvfs-20240505/tests/path/encoded_stream_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2324 2023-12-03 10:57:05.000000 dfvfs-20240505/tests/path/encryption_stream_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1102 2023-12-03 10:57:05.000000 dfvfs-20240505/tests/path/ewf_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2310 2023-12-03 10:57:05.000000 dfvfs-20240505/tests/path/ext_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1580 2023-12-03 10:57:05.000000 dfvfs-20240505/tests/path/factory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1331 2023-12-03 10:57:05.000000 dfvfs-20240505/tests/path/fake_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2345 2023-12-03 10:57:05.000000 dfvfs-20240505/tests/path/fat_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2457 2023-12-03 10:57:05.000000 dfvfs-20240505/tests/path/gpt_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1113 2023-12-03 10:57:05.000000 dfvfs-20240505/tests/path/gzip_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2843 2023-12-03 10:57:05.000000 dfvfs-20240505/tests/path/hfs_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1129 2023-12-03 10:57:05.000000 dfvfs-20240505/tests/path/luksde_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2463 2023-12-03 10:57:05.000000 dfvfs-20240505/tests/path/lvm_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1129 2023-12-03 10:57:05.000000 dfvfs-20240505/tests/path/modi_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      945 2023-12-03 10:57:05.000000 dfvfs-20240505/tests/path/mount_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3362 2023-12-03 10:57:05.000000 dfvfs-20240505/tests/path/ntfs_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1990 2023-12-03 10:57:05.000000 dfvfs-20240505/tests/path/os_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2585 2023-12-03 10:57:05.000000 dfvfs-20240505/tests/path/path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1115 2023-12-03 10:57:05.000000 dfvfs-20240505/tests/path/phdi_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1115 2023-12-03 10:57:05.000000 dfvfs-20240505/tests/path/qcow_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1130 2023-12-03 10:57:05.000000 dfvfs-20240505/tests/path/raw_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2920 2023-12-03 10:57:05.000000 dfvfs-20240505/tests/path/sqlite_blob_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1320 2023-12-03 10:57:05.000000 dfvfs-20240505/tests/path/tar_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      778 2023-12-03 10:57:05.000000 dfvfs-20240505/tests/path/test_lib.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3228 2023-12-03 10:57:05.000000 dfvfs-20240505/tests/path/tsk_partition_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2808 2023-12-03 10:57:05.000000 dfvfs-20240505/tests/path/tsk_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1141 2023-12-03 10:57:05.000000 dfvfs-20240505/tests/path/vhdi_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1115 2023-12-03 10:57:05.000000 dfvfs-20240505/tests/path/vmdk_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2561 2023-12-03 10:57:05.000000 dfvfs-20240505/tests/path/vshadow_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2310 2023-12-03 10:57:05.000000 dfvfs-20240505/tests/path/xfs_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1320 2023-12-03 10:57:05.000000 dfvfs-20240505/tests/path/zip_path_spec.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-08 04:24:45.063782 dfvfs-20240505/tests/resolver/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5408 2023-12-03 10:57:06.000000 dfvfs-20240505/tests/resolver/context.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-08 04:24:45.067782 dfvfs-20240505/tests/resolver_helpers/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       24 2023-12-03 10:57:02.000000 dfvfs-20240505/tests/resolver_helpers/__init__.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1914 2023-12-03 10:57:02.000000 dfvfs-20240505/tests/resolver_helpers/apfs_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1700 2023-12-03 10:57:02.000000 dfvfs-20240505/tests/resolver_helpers/apm_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2023-12-03 10:57:02.000000 dfvfs-20240505/tests/resolver_helpers/bde_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1682 2023-12-03 10:57:02.000000 dfvfs-20240505/tests/resolver_helpers/compressed_stream_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1587 2023-12-03 10:57:02.000000 dfvfs-20240505/tests/resolver_helpers/cpio_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1846 2023-12-03 10:57:03.000000 dfvfs-20240505/tests/resolver_helpers/cs_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1641 2023-12-03 10:57:02.000000 dfvfs-20240505/tests/resolver_helpers/encoded_stream_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1665 2023-12-03 10:57:02.000000 dfvfs-20240505/tests/resolver_helpers/encrypted_stream_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1428 2023-12-03 10:57:02.000000 dfvfs-20240505/tests/resolver_helpers/ewf_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1697 2023-12-03 10:57:03.000000 dfvfs-20240505/tests/resolver_helpers/ext_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1698 2023-12-03 10:57:03.000000 dfvfs-20240505/tests/resolver_helpers/fat_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1696 2023-12-03 10:57:03.000000 dfvfs-20240505/tests/resolver_helpers/gpt_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1413 2023-12-03 10:57:03.000000 dfvfs-20240505/tests/resolver_helpers/gzip_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1700 2023-12-03 10:57:03.000000 dfvfs-20240505/tests/resolver_helpers/hfs_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1429 2023-12-03 10:57:02.000000 dfvfs-20240505/tests/resolver_helpers/luksde_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1696 2023-12-03 10:57:02.000000 dfvfs-20240505/tests/resolver_helpers/lvm_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1194 2023-12-03 10:57:02.000000 dfvfs-20240505/tests/resolver_helpers/manager.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1463 2023-12-03 10:57:03.000000 dfvfs-20240505/tests/resolver_helpers/modi_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1714 2023-12-03 10:57:02.000000 dfvfs-20240505/tests/resolver_helpers/ntfs_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1378 2023-12-03 10:57:02.000000 dfvfs-20240505/tests/resolver_helpers/os_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1466 2023-12-03 10:57:03.000000 dfvfs-20240505/tests/resolver_helpers/phdi_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1443 2023-12-03 10:57:02.000000 dfvfs-20240505/tests/resolver_helpers/qcow_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1428 2023-12-03 10:57:02.000000 dfvfs-20240505/tests/resolver_helpers/raw_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1617 2023-12-03 10:57:02.000000 dfvfs-20240505/tests/resolver_helpers/sqlite_blob_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1413 2023-12-03 10:57:02.000000 dfvfs-20240505/tests/resolver_helpers/tar_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2525 2023-12-03 10:57:03.000000 dfvfs-20240505/tests/resolver_helpers/test_lib.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1882 2023-12-03 10:57:02.000000 dfvfs-20240505/tests/resolver_helpers/tsk_partition_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1721 2023-12-03 10:57:02.000000 dfvfs-20240505/tests/resolver_helpers/tsk_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1467 2023-12-03 10:57:03.000000 dfvfs-20240505/tests/resolver_helpers/vhdi_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1442 2023-12-03 10:57:03.000000 dfvfs-20240505/tests/resolver_helpers/vmdk_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1748 2023-12-03 10:57:02.000000 dfvfs-20240505/tests/resolver_helpers/vshadow_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1696 2023-12-03 10:57:03.000000 dfvfs-20240505/tests/resolver_helpers/xfs_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1567 2023-12-03 10:57:02.000000 dfvfs-20240505/tests/resolver_helpers/zip_resolver_helper.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-08 04:24:45.067782 dfvfs-20240505/tests/serializer/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       24 2023-12-03 10:57:06.000000 dfvfs-20240505/tests/serializer/__init__.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1978 2023-12-03 10:57:06.000000 dfvfs-20240505/tests/serializer/json_serializer.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1996 2023-12-03 10:57:02.000000 dfvfs-20240505/tests/test_lib.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-08 04:24:45.080782 dfvfs-20240505/tests/vfs/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       24 2024-01-28 12:31:03.000000 dfvfs-20240505/tests/vfs/__init__.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2458 2024-01-28 12:31:03.000000 dfvfs-20240505/tests/vfs/apfs_attribute.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2058 2024-01-28 12:31:03.000000 dfvfs-20240505/tests/vfs/apfs_container_directory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16546 2024-01-28 16:33:12.000000 dfvfs-20240505/tests/vfs/apfs_container_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9379 2024-01-28 12:31:03.000000 dfvfs-20240505/tests/vfs/apfs_container_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2328 2024-01-28 12:31:03.000000 dfvfs-20240505/tests/vfs/apfs_directory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28404 2024-01-28 16:33:12.000000 dfvfs-20240505/tests/vfs/apfs_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4316 2024-01-28 12:31:03.000000 dfvfs-20240505/tests/vfs/apfs_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1883 2024-01-28 12:31:03.000000 dfvfs-20240505/tests/vfs/apm_directory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7699 2024-01-28 16:33:12.000000 dfvfs-20240505/tests/vfs/apm_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5973 2024-01-28 12:31:03.000000 dfvfs-20240505/tests/vfs/apm_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      545 2024-01-28 12:31:03.000000 dfvfs-20240505/tests/vfs/attribute.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6755 2024-01-28 12:31:03.000000 dfvfs-20240505/tests/vfs/bde_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2491 2024-01-28 12:31:03.000000 dfvfs-20240505/tests/vfs/bde_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4742 2024-01-28 16:33:12.000000 dfvfs-20240505/tests/vfs/compressed_stream_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2830 2024-01-28 12:31:03.000000 dfvfs-20240505/tests/vfs/compressed_stream_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1790 2024-01-28 12:31:03.000000 dfvfs-20240505/tests/vfs/cpio_directory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8419 2024-01-28 16:33:12.000000 dfvfs-20240505/tests/vfs/cpio_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3366 2024-01-28 12:31:03.000000 dfvfs-20240505/tests/vfs/cpio_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8349 2024-01-28 16:33:12.000000 dfvfs-20240505/tests/vfs/cs_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6279 2024-01-28 12:31:03.000000 dfvfs-20240505/tests/vfs/cs_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4606 2024-01-28 16:33:12.000000 dfvfs-20240505/tests/vfs/data_range_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2658 2024-01-28 12:31:03.000000 dfvfs-20240505/tests/vfs/data_range_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      883 2024-01-28 12:31:03.000000 dfvfs-20240505/tests/vfs/data_stream.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1379 2024-01-28 12:31:03.000000 dfvfs-20240505/tests/vfs/directory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3796 2024-01-28 16:33:12.000000 dfvfs-20240505/tests/vfs/encoded_stream_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2771 2024-01-28 12:31:03.000000 dfvfs-20240505/tests/vfs/encoded_stream_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4144 2024-01-28 16:33:12.000000 dfvfs-20240505/tests/vfs/encrypted_stream_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2979 2024-01-28 12:31:03.000000 dfvfs-20240505/tests/vfs/encrypted_stream_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2226 2024-01-28 12:31:03.000000 dfvfs-20240505/tests/vfs/ext_attribute.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2113 2024-01-28 12:31:03.000000 dfvfs-20240505/tests/vfs/ext_directory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23810 2024-01-28 16:33:12.000000 dfvfs-20240505/tests/vfs/ext_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3983 2024-01-28 12:31:03.000000 dfvfs-20240505/tests/vfs/ext_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      438 2024-01-28 12:31:03.000000 dfvfs-20240505/tests/vfs/extent.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2323 2024-01-28 12:31:03.000000 dfvfs-20240505/tests/vfs/fake_directory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10644 2024-01-28 16:33:12.000000 dfvfs-20240505/tests/vfs/fake_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2904 2024-01-28 12:31:03.000000 dfvfs-20240505/tests/vfs/fake_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2115 2024-01-28 12:31:03.000000 dfvfs-20240505/tests/vfs/fat_directory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13064 2024-01-28 16:33:12.000000 dfvfs-20240505/tests/vfs/fat_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4069 2024-01-28 12:31:03.000000 dfvfs-20240505/tests/vfs/fat_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11194 2024-01-28 12:31:03.000000 dfvfs-20240505/tests/vfs/file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2749 2024-01-28 12:31:03.000000 dfvfs-20240505/tests/vfs/file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1880 2024-01-28 12:31:03.000000 dfvfs-20240505/tests/vfs/gpt_directory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7790 2024-01-28 16:33:12.000000 dfvfs-20240505/tests/vfs/gpt_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6704 2024-01-28 12:31:03.000000 dfvfs-20240505/tests/vfs/gpt_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4674 2024-01-28 16:33:12.000000 dfvfs-20240505/tests/vfs/gzip_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2511 2024-01-28 12:31:03.000000 dfvfs-20240505/tests/vfs/gzip_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2239 2024-01-28 12:31:03.000000 dfvfs-20240505/tests/vfs/hfs_attribute.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4024 2024-01-28 12:31:03.000000 dfvfs-20240505/tests/vfs/hfs_data_stream.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2116 2024-01-28 12:31:03.000000 dfvfs-20240505/tests/vfs/hfs_directory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17357 2024-01-28 16:33:12.000000 dfvfs-20240505/tests/vfs/hfs_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4062 2024-01-28 12:31:03.000000 dfvfs-20240505/tests/vfs/hfs_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4814 2024-01-28 16:33:12.000000 dfvfs-20240505/tests/vfs/luksde_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2549 2024-01-28 12:31:03.000000 dfvfs-20240505/tests/vfs/luksde_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1880 2024-01-28 12:31:03.000000 dfvfs-20240505/tests/vfs/lvm_directory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8162 2024-01-28 16:33:12.000000 dfvfs-20240505/tests/vfs/lvm_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6462 2024-01-28 12:31:03.000000 dfvfs-20240505/tests/vfs/lvm_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9765 2024-01-28 12:31:03.000000 dfvfs-20240505/tests/vfs/ntfs_attibute.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4168 2024-01-28 12:31:03.000000 dfvfs-20240505/tests/vfs/ntfs_data_stream.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2139 2024-01-28 12:31:03.000000 dfvfs-20240505/tests/vfs/ntfs_directory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27468 2024-01-28 12:31:03.000000 dfvfs-20240505/tests/vfs/ntfs_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4115 2024-01-28 12:31:03.000000 dfvfs-20240505/tests/vfs/ntfs_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1602 2024-01-28 12:31:03.000000 dfvfs-20240505/tests/vfs/os_directory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9917 2024-01-28 16:33:12.000000 dfvfs-20240505/tests/vfs/os_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6183 2024-01-28 16:33:12.000000 dfvfs-20240505/tests/vfs/os_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2628 2024-01-28 12:31:03.000000 dfvfs-20240505/tests/vfs/sqlite_blob_directory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5588 2024-01-28 16:33:12.000000 dfvfs-20240505/tests/vfs/sqlite_blob_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3493 2024-01-28 12:31:03.000000 dfvfs-20240505/tests/vfs/sqlite_blob_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1766 2024-01-28 12:31:03.000000 dfvfs-20240505/tests/vfs/tar_directory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8767 2024-01-28 16:33:12.000000 dfvfs-20240505/tests/vfs/tar_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5544 2024-01-28 12:31:03.000000 dfvfs-20240505/tests/vfs/tar_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4017 2024-01-28 12:31:03.000000 dfvfs-20240505/tests/vfs/tsk_attribute.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11512 2024-01-28 12:31:03.000000 dfvfs-20240505/tests/vfs/tsk_data_stream.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1893 2024-01-28 12:31:03.000000 dfvfs-20240505/tests/vfs/tsk_directory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    95551 2024-01-28 16:33:12.000000 dfvfs-20240505/tests/vfs/tsk_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3941 2024-01-28 12:31:03.000000 dfvfs-20240505/tests/vfs/tsk_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1904 2024-01-28 12:31:03.000000 dfvfs-20240505/tests/vfs/tsk_partition_directory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22354 2024-01-28 16:33:12.000000 dfvfs-20240505/tests/vfs/tsk_partition_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6657 2024-01-28 12:31:03.000000 dfvfs-20240505/tests/vfs/tsk_partition_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1963 2024-01-28 12:31:03.000000 dfvfs-20240505/tests/vfs/vshadow_directory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8488 2024-01-28 16:33:12.000000 dfvfs-20240505/tests/vfs/vshadow_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6413 2024-01-28 12:31:03.000000 dfvfs-20240505/tests/vfs/vshadow_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2228 2024-01-28 12:31:03.000000 dfvfs-20240505/tests/vfs/xfs_attribute.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2112 2024-01-28 12:31:03.000000 dfvfs-20240505/tests/vfs/xfs_directory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13190 2024-01-28 16:33:12.000000 dfvfs-20240505/tests/vfs/xfs_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3985 2024-01-28 12:31:03.000000 dfvfs-20240505/tests/vfs/xfs_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1763 2024-01-28 12:31:03.000000 dfvfs-20240505/tests/vfs/zip_directory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13454 2024-01-28 12:31:03.000000 dfvfs-20240505/tests/vfs/zip_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5641 2024-01-28 12:31:03.000000 dfvfs-20240505/tests/vfs/zip_file_system.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-08 04:24:45.082782 dfvfs-20240505/tests/volume/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       24 2023-12-03 10:57:08.000000 dfvfs-20240505/tests/volume/__init__.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2698 2023-12-03 10:57:08.000000 dfvfs-20240505/tests/volume/apfs_volume_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2808 2023-12-03 10:57:08.000000 dfvfs-20240505/tests/volume/apm_volume_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2088 2023-12-03 10:57:08.000000 dfvfs-20240505/tests/volume/cs_volume_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1474 2023-12-03 10:57:08.000000 dfvfs-20240505/tests/volume/factory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2945 2023-12-03 10:57:08.000000 dfvfs-20240505/tests/volume/gpt_volume_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3695 2023-12-03 10:57:08.000000 dfvfs-20240505/tests/volume/lvm_volume_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8084 2023-12-03 10:57:08.000000 dfvfs-20240505/tests/volume/tsk_volume_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3543 2023-12-03 10:57:08.000000 dfvfs-20240505/tests/volume/vshadow_volume_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1347 2024-05-05 10:07:02.000000 dfvfs-20240505/tox.ini
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-08 04:24:45.083782 dfvfs-20240505/utils/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       24 2023-12-03 10:57:09.000000 dfvfs-20240505/utils/__init__.py
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)      422 2024-05-05 10:07:02.000000 dfvfs-20240505/utils/check_dependencies.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11583 2024-05-05 10:07:02.000000 dfvfs-20240505/utils/dependencies.py
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     2366 2023-12-03 10:57:09.000000 dfvfs-20240505/utils/generate_test_data_bsd.sh
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    14027 2023-12-03 10:57:08.000000 dfvfs-20240505/utils/generate_test_data_linux.sh
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4844 2023-12-03 10:57:08.000000 dfvfs-20240505/utils/generate_test_data_macos.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14212 2023-12-03 10:57:09.000000 dfvfs-20240505/utils/generate_test_data_windows.bat
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)      943 2024-01-28 16:33:12.000000 dfvfs-20240505/utils/update_release.sh
```

### Comparing `dfvfs-20240115/.github/workflows/test_docker.yml` & `dfvfs-20240505/.github/workflows/test_docker.yml`

 * *Files 10% similar despite different names*

```diff
@@ -3,82 +3,71 @@
 on: [push]
 permissions: read-all
 jobs:
   test_fedora:
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        version: ['38']
+        version: ['39', '40']
     container:
       image: registry.fedoraproject.org/fedora:${{ matrix.version }}
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
     - name: Set up container
       run: |
         dnf install -y dnf-plugins-core langpacks-en
     - name: Install dependencies
       run: |
         dnf copr -y enable @gift/dev
-        dnf install -y @development-tools python3 python3-devel libbde-python3 libcaes-python3 libewf-python3 libfcrypto-python3 libfsapfs-python3 libfsext-python3 libfsfat-python3 libfshfs-python3 libfsntfs-python3 libfsxfs-python3 libfvde-python3 libfwnt-python3 libluksde-python3 libmodi-python3 libphdi-python3 libqcow-python3 libsigscan-python3 libsmdev-python3 libsmraw-python3 libvhdi-python3 libvmdk-python3 libvsapm-python3 libvsgpt-python3 libvshadow-python3 libvslvm-python3 python3-cffi python3-dfdatetime python3-dtfabric python3-idna python3-pytsk3 python3-pyyaml python3-setuptools python3-xattr
+        dnf install -y @development-tools libbde-python3 libcaes-python3 libewf-python3 libfcrypto-python3 libfsapfs-python3 libfsext-python3 libfsfat-python3 libfshfs-python3 libfsntfs-python3 libfsxfs-python3 libfvde-python3 libfwnt-python3 libluksde-python3 libmodi-python3 libphdi-python3 libqcow-python3 libsigscan-python3 libsmdev-python3 libsmraw-python3 libvhdi-python3 libvmdk-python3 libvsapm-python3 libvsgpt-python3 libvshadow-python3 libvslvm-python3 python3 python3-build python3-devel python3-dfdatetime python3-dtfabric python3-idna python3-pytsk3 python3-pyyaml python3-setuptools python3-wheel python3-xattr
     - name: Run tests
       env:
         LANG: C.utf8
       run: |
         python3 ./run_tests.py
     - name: Run end-to-end tests
       run: |
         if test -f tests/end-to-end.py; then PYTHONPATH=. python3 ./tests/end-to-end.py --debug -c config/end-to-end.ini; fi
-    - name: Build source distribution
+    - name: Build source distribution (sdist)
       run: |
-        python3 ./setup.py sdist
-    - name: Build binary distribution
+        python3 -m build --no-isolation --sdist
+    - name: Build binary distribution (wheel)
       run: |
-        python3 ./setup.py bdist
-    - name: Run build and install test
-      run: |
-        python3 ./setup.py build
-        python3 ./setup.py install
+        python3 -m build --no-isolation --wheel
   test_ubuntu:
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        version: ['22.04']
+        version: ['24.04']
     container:
       image: ubuntu:${{ matrix.version }}
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
     - name: Set up container
       env:
         DEBIAN_FRONTEND: noninteractive
       run: |
         apt-get update -q
         apt-get install -y libterm-readline-gnu-perl locales software-properties-common
         locale-gen en_US.UTF-8
         ln -f -s /usr/share/zoneinfo/UTC /etc/localtime
     - name: Install dependencies
       run: |
         add-apt-repository -y ppa:gift/dev
         apt-get update -q
-        apt-get install -y build-essential python3 python3-dev libbde-python3 libcaes-python3 libewf-python3 libfcrypto-python3 libfsapfs-python3 libfsext-python3 libfsfat-python3 libfshfs-python3 libfsntfs-python3 libfsxfs-python3 libfvde-python3 libfwnt-python3 libluksde-python3 libmodi-python3 libphdi-python3 libqcow-python3 libsigscan-python3 libsmdev-python3 libsmraw-python3 libvhdi-python3 libvmdk-python3 libvsapm-python3 libvsgpt-python3 libvshadow-python3 libvslvm-python3 python3-cffi-backend python3-dfdatetime python3-distutils python3-dtfabric python3-idna python3-pip python3-pytsk3 python3-setuptools python3-wheel python3-xattr python3-yaml
+        apt-get install -y build-essential libbde-python3 libcaes-python3 libewf-python3 libfcrypto-python3 libfsapfs-python3 libfsext-python3 libfsfat-python3 libfshfs-python3 libfsntfs-python3 libfsxfs-python3 libfvde-python3 libfwnt-python3 libluksde-python3 libmodi-python3 libphdi-python3 libqcow-python3 libsigscan-python3 libsmdev-python3 libsmraw-python3 libvhdi-python3 libvmdk-python3 libvsapm-python3 libvsgpt-python3 libvshadow-python3 libvslvm-python3 python3 python3-build python3-dev python3-dfdatetime python3-dtfabric python3-idna python3-pip python3-pytsk3 python3-setuptools python3-wheel python3-xattr python3-yaml
     - name: Run tests
       env:
         LANG: en_US.UTF-8
       run: |
         python3 ./run_tests.py
     - name: Run end-to-end tests
       env:
         LANG: en_US.UTF-8
       run: |
         if test -f tests/end-to-end.py; then PYTHONPATH=. python3 ./tests/end-to-end.py --debug -c config/end-to-end.ini; fi
-    - name: Update setuptools
-      run: |
-        python3 -m pip install -U setuptools
-    - name: Build source distribution
-      run: |
-        python3 ./setup.py sdist
-    - name: Build binary distribution
+    - name: Build source distribution (sdist)
       run: |
-        python3 ./setup.py bdist
-    - name: Run build and install test
+        python3 -m build --no-isolation --sdist
+    - name: Build binary distribution (wheel)
       run: |
-        python3 ./setup.py build
-        python3 ./setup.py install
+        python3 -m build --no-isolation --wheel
```

### Comparing `dfvfs-20240115/.github/workflows/test_docs.yml` & `dfvfs-20240505/.github/workflows/test_docs.yml`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
       matrix:
         include:
         - python-version: '3.12'
           toxenv: 'docs'
     container:
       image: ubuntu:22.04
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
     - name: Set up container
       env:
         DEBIAN_FRONTEND: noninteractive
       run: |
         apt-get update -q
         apt-get install -y libterm-readline-gnu-perl locales software-properties-common
         locale-gen en_US.UTF-8
@@ -32,15 +32,15 @@
       env:
         DEBIAN_FRONTEND: noninteractive
       run: |
         add-apt-repository -y universe
         add-apt-repository -y ppa:deadsnakes/ppa
         add-apt-repository -y ppa:gift/dev
         apt-get update -q
-        apt-get install -y build-essential git libffi-dev python${{ matrix.python-version }} python${{ matrix.python-version }}-dev python${{ matrix.python-version }}-venv libbde-python3 libcaes-python3 libewf-python3 libfcrypto-python3 libfsapfs-python3 libfsext-python3 libfsfat-python3 libfshfs-python3 libfsntfs-python3 libfsxfs-python3 libfvde-python3 libfwnt-python3 libluksde-python3 libmodi-python3 libphdi-python3 libqcow-python3 libsigscan-python3 libsmdev-python3 libsmraw-python3 libvhdi-python3 libvmdk-python3 libvsapm-python3 libvsgpt-python3 libvshadow-python3 libvslvm-python3 python3-cffi-backend python3-dfdatetime python3-distutils python3-dtfabric python3-idna python3-pip python3-pytsk3 python3-setuptools python3-xattr python3-yaml
+        apt-get install -y build-essential git libffi-dev python${{ matrix.python-version }} python${{ matrix.python-version }}-dev python${{ matrix.python-version }}-venv libbde-python3 libcaes-python3 libewf-python3 libfcrypto-python3 libfsapfs-python3 libfsext-python3 libfsfat-python3 libfshfs-python3 libfsntfs-python3 libfsxfs-python3 libfvde-python3 libfwnt-python3 libluksde-python3 libmodi-python3 libphdi-python3 libqcow-python3 libsigscan-python3 libsmdev-python3 libsmraw-python3 libvhdi-python3 libvmdk-python3 libvsapm-python3 libvsgpt-python3 libvshadow-python3 libvslvm-python3 python3-dfdatetime python3-distutils python3-dtfabric python3-idna python3-lib2to3 python3-pip python3-pytsk3 python3-setuptools python3-xattr python3-yaml
     - name: Install tox
       run: |
         python3 -m pip install tox
     - name: Run tests
       env:
         LANG: en_US.UTF-8
       run: |
```

### Comparing `dfvfs-20240115/.github/workflows/test_tox.yml` & `dfvfs-20240505/.github/workflows/test_tox.yml`

 * *Files 12% similar despite different names*

```diff
@@ -10,30 +10,28 @@
 permissions: read-all
 jobs:
   build:
     runs-on: ubuntu-latest
     strategy:
       matrix:
         include:
-        - python-version: '3.7'
-          toxenv: 'py37,wheel'
         - python-version: '3.8'
           toxenv: 'py38,wheel'
         - python-version: '3.9'
           toxenv: 'py39,wheel'
         - python-version: '3.10'
           toxenv: 'py310,wheel'
         - python-version: '3.11'
           toxenv: 'py311,wheel'
         - python-version: '3.12'
           toxenv: 'py312,wheel'
     container:
       image: ubuntu:22.04
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
     - name: Set up container
       env:
         DEBIAN_FRONTEND: noninteractive
       run: |
         apt-get update -q
         apt-get install -y libterm-readline-gnu-perl locales software-properties-common
         locale-gen en_US.UTF-8
@@ -42,15 +40,15 @@
       env:
         DEBIAN_FRONTEND: noninteractive
       run: |
         add-apt-repository -y universe
         add-apt-repository -y ppa:deadsnakes/ppa
         add-apt-repository -y ppa:gift/dev
         apt-get update -q
-        apt-get install -y build-essential git libffi-dev python${{ matrix.python-version }} python${{ matrix.python-version }}-dev python${{ matrix.python-version }}-venv libbde-python3 libcaes-python3 libewf-python3 libfcrypto-python3 libfsapfs-python3 libfsext-python3 libfsfat-python3 libfshfs-python3 libfsntfs-python3 libfsxfs-python3 libfvde-python3 libfwnt-python3 libluksde-python3 libmodi-python3 libphdi-python3 libqcow-python3 libsigscan-python3 libsmdev-python3 libsmraw-python3 libvhdi-python3 libvmdk-python3 libvsapm-python3 libvsgpt-python3 libvshadow-python3 libvslvm-python3 python3-cffi-backend python3-dfdatetime python3-distutils python3-dtfabric python3-idna python3-pip python3-pytsk3 python3-setuptools python3-xattr python3-yaml
+        apt-get install -y build-essential git libffi-dev python${{ matrix.python-version }} python${{ matrix.python-version }}-dev python${{ matrix.python-version }}-venv libbde-python3 libcaes-python3 libewf-python3 libfcrypto-python3 libfsapfs-python3 libfsext-python3 libfsfat-python3 libfshfs-python3 libfsntfs-python3 libfsxfs-python3 libfvde-python3 libfwnt-python3 libluksde-python3 libmodi-python3 libphdi-python3 libqcow-python3 libsigscan-python3 libsmdev-python3 libsmraw-python3 libvhdi-python3 libvmdk-python3 libvsapm-python3 libvsgpt-python3 libvshadow-python3 libvslvm-python3 python3-dfdatetime python3-distutils python3-dtfabric python3-idna python3-lib2to3 python3-pip python3-pytsk3 python3-setuptools python3-xattr python3-yaml
     - name: Install tox
       run: |
         python3 -m pip install tox
     - name: Run tests
       env:
         LANG: en_US.UTF-8
       run: |
@@ -61,15 +59,15 @@
       matrix:
         include:
         - python-version: '3.10'
           toxenv: 'coverage'
     container:
       image: ubuntu:22.04
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
     - name: Set up container
       env:
         DEBIAN_FRONTEND: noninteractive
       run: |
         apt-get update -q
         apt-get install -y libterm-readline-gnu-perl locales software-properties-common
         locale-gen en_US.UTF-8
@@ -78,36 +76,38 @@
       env:
         DEBIAN_FRONTEND: noninteractive
       run: |
         add-apt-repository -y universe
         add-apt-repository -y ppa:deadsnakes/ppa
         add-apt-repository -y ppa:gift/dev
         apt-get update -q
-        apt-get install -y build-essential git libffi-dev python${{ matrix.python-version }} python${{ matrix.python-version }}-dev python${{ matrix.python-version }}-venv libbde-python3 libcaes-python3 libewf-python3 libfcrypto-python3 libfsapfs-python3 libfsext-python3 libfsfat-python3 libfshfs-python3 libfsntfs-python3 libfsxfs-python3 libfvde-python3 libfwnt-python3 libluksde-python3 libmodi-python3 libphdi-python3 libqcow-python3 libsigscan-python3 libsmdev-python3 libsmraw-python3 libvhdi-python3 libvmdk-python3 libvsapm-python3 libvsgpt-python3 libvshadow-python3 libvslvm-python3 python3-cffi-backend python3-dfdatetime python3-distutils python3-dtfabric python3-idna python3-pip python3-pytsk3 python3-setuptools python3-xattr python3-yaml
+        apt-get install -y build-essential git libffi-dev python${{ matrix.python-version }} python${{ matrix.python-version }}-dev python${{ matrix.python-version }}-venv libbde-python3 libcaes-python3 libewf-python3 libfcrypto-python3 libfsapfs-python3 libfsext-python3 libfsfat-python3 libfshfs-python3 libfsntfs-python3 libfsxfs-python3 libfvde-python3 libfwnt-python3 libluksde-python3 libmodi-python3 libphdi-python3 libqcow-python3 libsigscan-python3 libsmdev-python3 libsmraw-python3 libvhdi-python3 libvmdk-python3 libvsapm-python3 libvsgpt-python3 libvshadow-python3 libvslvm-python3 python3-dfdatetime python3-distutils python3-dtfabric python3-idna python3-lib2to3 python3-pip python3-pytsk3 python3-setuptools python3-xattr python3-yaml
     - name: Install tox
       run: |
         python3 -m pip install tox
     - name: Run tests with coverage
       env:
         LANG: en_US.UTF-8
       run: |
         tox -e${{ matrix.toxenv }}
     - name: Upload coverage report to Codecov
-      uses: codecov/codecov-action@v3
+      uses: codecov/codecov-action@v4
+      with:
+        token: ${{ secrets.CODECOV_TOKEN }}
   lint:
     runs-on: ubuntu-latest
     strategy:
       matrix:
         include:
         - python-version: '3.12'
           toxenv: 'lint'
     container:
       image: ubuntu:22.04
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
     - name: Set up container
       env:
         DEBIAN_FRONTEND: noninteractive
       run: |
         apt-get update -q
         apt-get install -y libterm-readline-gnu-perl locales software-properties-common
         locale-gen en_US.UTF-8
@@ -116,15 +116,15 @@
       env:
         DEBIAN_FRONTEND: noninteractive
       run: |
         add-apt-repository -y universe
         add-apt-repository -y ppa:deadsnakes/ppa
         add-apt-repository -y ppa:gift/dev
         apt-get update -q
-        apt-get install -y build-essential git libffi-dev python${{ matrix.python-version }} python${{ matrix.python-version }}-dev python${{ matrix.python-version }}-venv libbde-python3 libcaes-python3 libewf-python3 libfcrypto-python3 libfsapfs-python3 libfsext-python3 libfsfat-python3 libfshfs-python3 libfsntfs-python3 libfsxfs-python3 libfvde-python3 libfwnt-python3 libluksde-python3 libmodi-python3 libphdi-python3 libqcow-python3 libsigscan-python3 libsmdev-python3 libsmraw-python3 libvhdi-python3 libvmdk-python3 libvsapm-python3 libvsgpt-python3 libvshadow-python3 libvslvm-python3 python3-cffi-backend python3-dfdatetime python3-distutils python3-dtfabric python3-idna python3-pip python3-pytsk3 python3-setuptools python3-xattr python3-yaml
+        apt-get install -y build-essential git libffi-dev python${{ matrix.python-version }} python${{ matrix.python-version }}-dev python${{ matrix.python-version }}-venv libbde-python3 libcaes-python3 libewf-python3 libfcrypto-python3 libfsapfs-python3 libfsext-python3 libfsfat-python3 libfshfs-python3 libfsntfs-python3 libfsxfs-python3 libfvde-python3 libfwnt-python3 libluksde-python3 libmodi-python3 libphdi-python3 libqcow-python3 libsigscan-python3 libsmdev-python3 libsmraw-python3 libvhdi-python3 libvmdk-python3 libvsapm-python3 libvsgpt-python3 libvshadow-python3 libvslvm-python3 python3-dfdatetime python3-distutils python3-dtfabric python3-idna python3-lib2to3 python3-pip python3-pytsk3 python3-setuptools python3-xattr python3-yaml
     - name: Install tox
       run: |
         python3 -m pip install tox
     - name: Run linter
       env:
         LANG: en_US.UTF-8
       run: |
```

### Comparing `dfvfs-20240115/.pylintrc` & `dfvfs-20240505/.pylintrc`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/ACKNOWLEDGEMENTS` & `dfvfs-20240505/ACKNOWLEDGEMENTS`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/LICENSE` & `dfvfs-20240505/LICENSE`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/MANIFEST.in` & `dfvfs-20240505/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/MANIFEST.test_data.in` & `dfvfs-20240505/MANIFEST.test_data.in`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/appveyor.yml` & `dfvfs-20240505/appveyor.yml`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/config/appveyor/install.ps1` & `dfvfs-20240505/config/appveyor/install.ps1`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Script to set up tests on AppVeyor Windows.
 
-$Dependencies = "PyYAML cffi dfdatetime dtfabric idna libbde libcaes libewf libfcrypto libfsapfs libfsext libfsfat libfshfs libfsntfs libfsxfs libfvde libfwnt libluksde libmodi libphdi libqcow libsigscan libsmdev libsmraw libvhdi libvmdk libvsapm libvsgpt libvshadow libvslvm pytsk3 xattr"
+$Dependencies = "PyYAML dfdatetime dtfabric idna libbde libcaes libewf libfcrypto libfsapfs libfsext libfsfat libfshfs libfsntfs libfsxfs libfvde libfwnt libluksde libmodi libphdi libqcow libsigscan libsmdev libsmraw libvhdi libvmdk libvsapm libvsgpt libvshadow libvslvm pytsk3 xattr"
 
 If ($Dependencies.Length -gt 0)
 {
 	$Dependencies = ${Dependencies} -split " "
 
 	$Output = Invoke-Expression -Command "git clone https://github.com/log2timeline/l2tdevtools.git ..\l2tdevtools 2>&1" | %{ "$_" }
 	Write-Host (${Output} | Out-String)
```

### Comparing `dfvfs-20240115/config/appveyor/runtests.sh` & `dfvfs-20240505/config/appveyor/runtests.sh`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/config/dpkg/control` & `dfvfs-20240505/config/dpkg/control`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,14 @@
 Build-Depends: debhelper (>= 9), dh-python, python3-all (>= 3.6~), python3-setuptools
 Standards-Version: 4.1.4
 X-Python3-Version: >= 3.6
 Homepage: https://github.com/log2timeline/dfvfs
 
 Package: python3-dfvfs
 Architecture: all
-Depends: libbde-python3 (>= 20220121), libcaes-python3 (>= 20240114), libewf-python3 (>= 20131210), libfcrypto-python3 (>= 20240114), libfsapfs-python3 (>= 20220709), libfsext-python3 (>= 20220829), libfsfat-python3 (>= 20220925), libfshfs-python3 (>= 20220831), libfsntfs-python3 (>= 20211229), libfsxfs-python3 (>= 20220829), libfvde-python3 (>= 20220121), libfwnt-python3 (>= 20210717), libluksde-python3 (>= 20220121), libmodi-python3 (>= 20210405), libphdi-python3 (>= 20220228), libqcow-python3 (>= 20201213), libsigscan-python3 (>= 20230109), libsmdev-python3 (>= 20140529), libsmraw-python3 (>= 20140612), libvhdi-python3 (>= 20201014), libvmdk-python3 (>= 20140421), libvsapm-python3 (>= 20230506), libvsgpt-python3 (>= 20211115), libvshadow-python3 (>= 20160109), libvslvm-python3 (>= 20160109), python3-cffi-backend (>= 1.9.1), python3-dfdatetime (>= 20221112), python3-dtfabric (>= 20230518), python3-idna (>= 2.5), python3-pytsk3 (>= 20210419), python3-xattr (>= 0.7.2), python3-yaml (>= 3.10), ${misc:Depends}
+Depends: libbde-python3 (>= 20220121), libcaes-python3 (>= 20240114), libewf-python3 (>= 20131210), libfcrypto-python3 (>= 20240114), libfsapfs-python3 (>= 20220709), libfsext-python3 (>= 20220829), libfsfat-python3 (>= 20220925), libfshfs-python3 (>= 20220831), libfsntfs-python3 (>= 20211229), libfsxfs-python3 (>= 20220829), libfvde-python3 (>= 20220121), libfwnt-python3 (>= 20210717), libluksde-python3 (>= 20220121), libmodi-python3 (>= 20210405), libphdi-python3 (>= 20220228), libqcow-python3 (>= 20201213), libsigscan-python3 (>= 20230109), libsmdev-python3 (>= 20140529), libsmraw-python3 (>= 20140612), libvhdi-python3 (>= 20201014), libvmdk-python3 (>= 20140421), libvsapm-python3 (>= 20230506), libvsgpt-python3 (>= 20211115), libvshadow-python3 (>= 20160109), libvslvm-python3 (>= 20160109), python3-dfdatetime (>= 20221112), python3-dtfabric (>= 20230518), python3-idna (>= 2.5), python3-pytsk3 (>= 20210419), python3-xattr (>= 0.7.2), python3-yaml (>= 3.10), ${misc:Depends}
 Description: Python 3 module of dfVFS
  dfVFS, or Digital Forensics Virtual File System, provides read-only access to
  file-system objects from various storage media types and file formats. The goal
  of dfVFS is to provide a generic interface for accessing file-system objects,
  for which it uses several back-ends that provide the actual implementation of
  the various storage media types, volume systems and file systems.
```

### Comparing `dfvfs-20240115/config/dpkg/copyright` & `dfvfs-20240505/config/dpkg/copyright`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/config/pylint/spelling-private-dict` & `dfvfs-20240505/config/pylint/spelling-private-dict`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dependencies.ini` & `dfvfs-20240505/dependencies.ini`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,7 @@
-[cffi]
-skip_check: true
-dpkg_name: python3-cffi-backend
-minimum_version: 1.9.1
-rpm_name: python3-cffi
-version_property: __version__
-
 [dfdatetime]
 dpkg_name: python3-dfdatetime
 minimum_version: 20221112
 rpm_name: python3-dfdatetime
 version_property: __version__
 
 [dtfabric]
```

### Comparing `dfvfs-20240115/dfvfs/analyzer/__init__.py` & `dfvfs-20240505/dfvfs/analyzer/__init__.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/analyzer/analyzer.py` & `dfvfs-20240505/dfvfs/analyzer/analyzer.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/analyzer/analyzer_helper.py` & `dfvfs-20240505/dfvfs/analyzer/analyzer_helper.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,26 +22,32 @@
       raise ValueError('Missing type indicator.')
 
     if not getattr(self, 'FORMAT_CATEGORIES', None):
       raise ValueError('Missing format categories.')
 
   @property
   def format_categories(self):
-    """set[str]: format categories, such as archive file or file system.
+    """Retrieves the format categories.
 
     The format categories are defined in definitions.FORMAT_CATEGORIES.
+
+    Returns:
+      set[str]: format categories, such as archive file or file system.
     """
     # pylint: disable=no-member
     return self.FORMAT_CATEGORIES
 
   @property
   def type_indicator(self):
-    """str: type indicator."""
-    # pylint: disable=no-member
-    return self.TYPE_INDICATOR
+    """Retrieves the type indicator.
+
+    Returns:
+      str: type indicator or None if not available.
+    """
+    return getattr(self, 'TYPE_INDICATOR', None)
 
   def AnalyzeFileObject(self, file_object):  # pylint: disable=useless-type-doc
     """Retrieves the format specification.
 
     This is the fall through implementation that raises a RuntimeError.
 
     Args:
```

### Comparing `dfvfs-20240115/dfvfs/analyzer/apfs_analyzer_helper.py` & `dfvfs-20240505/dfvfs/analyzer/apfs_analyzer_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/analyzer/apfs_container_analyzer_helper.py` & `dfvfs-20240505/dfvfs/analyzer/apfs_container_analyzer_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/analyzer/apm_analyzer_helper.py` & `dfvfs-20240505/dfvfs/analyzer/apm_analyzer_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/analyzer/bde_analyzer_helper.py` & `dfvfs-20240505/dfvfs/analyzer/bde_analyzer_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/analyzer/bzip2_analyzer_helper.py` & `dfvfs-20240505/dfvfs/analyzer/bzip2_analyzer_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/analyzer/cpio_analyzer_helper.py` & `dfvfs-20240505/dfvfs/analyzer/cpio_analyzer_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/analyzer/cs_analyzer_helper.py` & `dfvfs-20240505/dfvfs/analyzer/cs_analyzer_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/analyzer/ewf_analyzer_helper.py` & `dfvfs-20240505/dfvfs/analyzer/ewf_analyzer_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/analyzer/ext_analyzer_helper.py` & `dfvfs-20240505/dfvfs/analyzer/ext_analyzer_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/analyzer/fat_analyzer_helper.py` & `dfvfs-20240505/dfvfs/analyzer/fat_analyzer_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/analyzer/gpt_analyzer_helper.py` & `dfvfs-20240505/dfvfs/analyzer/gpt_analyzer_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/analyzer/gzip_analyzer_helper.py` & `dfvfs-20240505/dfvfs/analyzer/gzip_analyzer_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/analyzer/hfs_analyzer_helper.py` & `dfvfs-20240505/dfvfs/analyzer/hfs_analyzer_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/analyzer/luksde_analyzer_helper.py` & `dfvfs-20240505/dfvfs/analyzer/luksde_analyzer_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/analyzer/lvm_analyzer_helper.py` & `dfvfs-20240505/dfvfs/analyzer/lvm_analyzer_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/analyzer/modi_analyzer_helper.py` & `dfvfs-20240505/dfvfs/analyzer/modi_analyzer_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/analyzer/ntfs_analyzer_helper.py` & `dfvfs-20240505/dfvfs/analyzer/ntfs_analyzer_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/analyzer/phdi_analyzer_helper.py` & `dfvfs-20240505/dfvfs/analyzer/phdi_analyzer_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/analyzer/qcow_analyzer_helper.py` & `dfvfs-20240505/dfvfs/analyzer/qcow_analyzer_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/analyzer/specification.py` & `dfvfs-20240505/dfvfs/analyzer/specification.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,15 +77,19 @@
     super(FormatSpecificationStore, self).__init__()
     self._format_specifications = {}
     # Maps signature identifiers to format specifications.
     self._signature_map = {}
 
   @property
   def specifications(self):
-    """generator[FormatSpecification]: format specifications."""
+    """Retrieves the format specifications.
+
+    Returns:
+      generator[FormatSpecification]: format specifications.
+    """
     return iter(self._format_specifications.values())
 
   def AddNewSpecification(self, identifier):
     """Adds a new format specification.
 
     Args:
       identifier (str): unique signature identifier for a specification store.
```

### Comparing `dfvfs-20240115/dfvfs/analyzer/tar_analyzer_helper.py` & `dfvfs-20240505/dfvfs/analyzer/tar_analyzer_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/analyzer/tsk_analyzer_helper.py` & `dfvfs-20240505/dfvfs/analyzer/tsk_analyzer_helper.py`

 * *Files 7% similar despite different names*

```diff
@@ -56,13 +56,15 @@
     if definitions.PREFERRED_EXT_BACK_END == self.TYPE_INDICATOR:
       # Ext file system signature.
       format_specification.AddNewSignature(b'\x53\xef', offset=1080)
 
     # ISO9660 file system signature.
     format_specification.AddNewSignature(b'CD001', offset=32769)
 
+    # UFS file system signature.
+
     # YAFFS file system signature.
 
     return format_specification
 
 
 analyzer.Analyzer.RegisterHelper(TSKAnalyzerHelper())
```

### Comparing `dfvfs-20240115/dfvfs/analyzer/tsk_partition_analyzer_helper.py` & `dfvfs-20240505/dfvfs/analyzer/tsk_partition_analyzer_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/analyzer/vhdi_analyzer_helper.py` & `dfvfs-20240505/dfvfs/analyzer/vhdi_analyzer_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/analyzer/vmdk_analyzer_helper.py` & `dfvfs-20240505/dfvfs/analyzer/vmdk_analyzer_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/analyzer/vshadow_analyzer_helper.py` & `dfvfs-20240505/dfvfs/analyzer/vshadow_analyzer_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/analyzer/xfs_analyzer_helper.py` & `dfvfs-20240505/dfvfs/analyzer/xfs_analyzer_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/analyzer/xz_analyzer_helper.py` & `dfvfs-20240505/dfvfs/analyzer/xz_analyzer_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/analyzer/zip_analyzer_helper.py` & `dfvfs-20240505/dfvfs/analyzer/zip_analyzer_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/compression/bzip2_decompressor.py` & `dfvfs-20240505/dfvfs/compression/bzip2_decompressor.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/compression/manager.py` & `dfvfs-20240505/dfvfs/compression/manager.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/compression/xz_decompressor.py` & `dfvfs-20240505/dfvfs/compression/xz_decompressor.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/compression/zlib_decompressor.py` & `dfvfs-20240505/dfvfs/compression/zlib_decompressor.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/credentials/apfs_credentials.py` & `dfvfs-20240505/dfvfs/credentials/apfs_credentials.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/credentials/bde_credentials.py` & `dfvfs-20240505/dfvfs/credentials/bde_credentials.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/credentials/credentials.py` & `dfvfs-20240505/dfvfs/credentials/credentials.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/credentials/cs_credentials.py` & `dfvfs-20240505/dfvfs/credentials/cs_credentials.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/credentials/keychain.py` & `dfvfs-20240505/dfvfs/credentials/keychain.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 """The path specification key chain.
 
-The key chain is used to manage credentials for path specifications.
-E.g. BitLocker Drive Encryption (BDE) encrypted volumes can require a
-credential (e.g. password) to access the unencrypted data (unlock).
+The key chain is used to manage credentials for path specifications. E.g.
+BitLocker Drive Encryption (BDE) encrypted volumes can require a credential
+(e.g. password) to access the unencrypted data (unlock).
 """
 
 from dfvfs.credentials import manager
 
 
 class KeyChain(object):
   """Key chain."""
```

### Comparing `dfvfs-20240115/dfvfs/credentials/manager.py` & `dfvfs-20240505/dfvfs/credentials/manager.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/encoding/base16_decoder.py` & `dfvfs-20240505/dfvfs/encoding/base16_decoder.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/encoding/base32_decoder.py` & `dfvfs-20240505/dfvfs/encoding/base32_decoder.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/encoding/base64_decoder.py` & `dfvfs-20240505/dfvfs/encoding/base64_decoder.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/encoding/manager.py` & `dfvfs-20240505/dfvfs/encoding/manager.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/encryption/aes_decrypter.py` & `dfvfs-20240505/dfvfs/encryption/aes_decrypter.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/encryption/blowfish_decrypter.py` & `dfvfs-20240505/dfvfs/encryption/blowfish_decrypter.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/encryption/decrypter.py` & `dfvfs-20240505/dfvfs/encryption/decrypter.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/encryption/des3_decrypter.py` & `dfvfs-20240505/dfvfs/encryption/des3_decrypter.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/encryption/manager.py` & `dfvfs-20240505/dfvfs/encryption/manager.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/encryption/rc4_decrypter.py` & `dfvfs-20240505/dfvfs/encryption/rc4_decrypter.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/file_io/apfs_file_io.py` & `dfvfs-20240505/dfvfs/file_io/apfs_file_io.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from dfvfs.file_io import file_io
 from dfvfs.lib import errors
 from dfvfs.resolver import resolver
 
 
 class APFSFile(file_io.FileIO):
-  """File input/output (IO) object using pyfsapfs.file_entry"""
+  """File input/output (IO) object using pyfsapfs.file_entry."""
 
   def __init__(self, resolver_context, path_spec):
     """Initializes a file input/output (IO) object.
 
     Args:
       resolver_context (Context): resolver context.
       path_spec (PathSpec): a path specification.
```

### Comparing `dfvfs-20240115/dfvfs/file_io/apm_file_io.py` & `dfvfs-20240505/dfvfs/file_io/apm_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/file_io/bde_file_io.py` & `dfvfs-20240505/dfvfs/file_io/bde_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/file_io/compressed_stream_io.py` & `dfvfs-20240505/dfvfs/file_io/compressed_stream_io.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,17 +33,17 @@
     self._uncompressed_data_offset = 0
     self._uncompressed_data_size = 0
     self._uncompressed_stream_size = None
 
   def _Close(self):
     """Closes the file-like object.
 
-    If the file-like object was passed in the init function
-    the compressed stream file-like object does not control
-    the file-like object and should not actually close it.
+    If the file-like object was passed in the init function the compressed
+    stream file-like object does not control the file-like object and should not
+    actually close it.
     """
     self._compressed_data = b''
     self._file_object = None
     self._decompressor = None
     self._uncompressed_data = b''
 
   def _GetDecompressor(self):
```

### Comparing `dfvfs-20240115/dfvfs/file_io/cpio_file_io.py` & `dfvfs-20240505/dfvfs/file_io/cpio_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/file_io/cs_file_io.py` & `dfvfs-20240505/dfvfs/file_io/cs_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/file_io/data_range_io.py` & `dfvfs-20240505/dfvfs/file_io/data_range_io.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,18 +7,17 @@
 from dfvfs.lib import errors
 from dfvfs.resolver import resolver
 
 
 class DataRange(file_io.FileIO):
   """File input/output (IO) object that maps an in-file data range.
 
-  The data range object allows to expose a single partition within
-  a full disk image as a separate file-like object by mapping
-  the data range (offset and size) of the volume on top of the full disk
-  image.
+  The data range object allows to expose a single partition within a full disk
+  image as a separate file-like object by mapping the data range (offset and
+  size) of the volume on top of the full disk image.
   """
 
   def __init__(self, resolver_context, path_spec):
     """Initializes a file input/output (IO) object.
 
     Args:
       resolver_context (Context): resolver context.
@@ -29,17 +28,17 @@
     self._file_object = None
     self._range_offset = -1
     self._range_size = -1
 
   def _Close(self):
     """Closes the file-like object.
 
-    If the file-like object was passed in the init function
-    the data range file-like object does not control the file-like object
-    and should not actually close it.
+    If the file-like object was passed in the init function the data range file-
+    like object does not control the file-like object and should not actually
+    close it.
     """
     self._file_object = None
     self._range_offset = -1
     self._range_size = -1
 
   def _Open(self, mode='rb'):
     """Opens the file-like object.
```

### Comparing `dfvfs-20240115/dfvfs/file_io/encoded_stream_io.py` & `dfvfs-20240505/dfvfs/file_io/encoded_stream_io.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,17 +33,17 @@
     self._encoding_method = None
     self._file_object = None
     self._realign_offset = True
 
   def _Close(self):
     """Closes the file-like object.
 
-    If the file-like object was passed in the init function
-    the encoded stream file-like object does not control
-    the file-like object and should not actually close it.
+    If the file-like object was passed in the init function the encoded stream
+    file-like object does not control the file-like object and should not
+    actually close it.
     """
     self._decoder = None
     self._decoded_data = b''
     self._encoded_data = b''
     self._file_object = None
 
   def _GetDecoder(self):
```

### Comparing `dfvfs-20240115/dfvfs/file_io/encrypted_stream_io.py` & `dfvfs-20240505/dfvfs/file_io/encrypted_stream_io.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,17 +33,17 @@
     self._encryption_method = None
     self._file_object = None
     self._realign_offset = True
 
   def _Close(self):
     """Closes the file-like object.
 
-    If the file-like object was passed in the init function
-    the encrypted stream file-like object does not control
-    the file-like object and should not actually close it.
+    If the file-like object was passed in the init function the encrypted stream
+    file-like object does not control the file-like object and should not
+    actually close it.
     """
     self._decrypter = None
     self._decrypted_data = b''
     self._encrypted_data = b''
     self._file_object = None
 
   def _GetDecrypter(self):
```

### Comparing `dfvfs-20240115/dfvfs/file_io/ewf_file_io.py` & `dfvfs-20240505/dfvfs/file_io/ewf_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/file_io/ext_file_io.py` & `dfvfs-20240505/dfvfs/file_io/ext_file_io.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from dfvfs.file_io import file_io
 from dfvfs.lib import errors
 from dfvfs.resolver import resolver
 
 
 class EXTFile(file_io.FileIO):
-  """File input/output (IO) object using pyfsext.file_entry"""
+  """File input/output (IO) object using pyfsext.file_entry."""
 
   def __init__(self, resolver_context, path_spec):
     """Initializes a file input/output (IO) object.
 
     Args:
       resolver_context (Context): resolver context.
       path_spec (PathSpec): a path specification.
```

### Comparing `dfvfs-20240115/dfvfs/file_io/fake_file_io.py` & `dfvfs-20240505/dfvfs/file_io/fake_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/file_io/fat_file_io.py` & `dfvfs-20240505/dfvfs/file_io/fat_file_io.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import os
 
 from dfvfs.file_io import file_io
 from dfvfs.resolver import resolver
 
 
 class FATFile(file_io.FileIO):
-  """File input/output (IO) object using pyfsfat.file_entry"""
+  """File input/output (IO) object using pyfsfat.file_entry."""
 
   def __init__(self, resolver_context, path_spec):
     """Initializes a file input/output (IO) object.
 
     Args:
       resolver_context (Context): resolver context.
       path_spec (PathSpec): a path specification.
```

### Comparing `dfvfs-20240115/dfvfs/file_io/file_io.py` & `dfvfs-20240505/dfvfs/file_io/file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/file_io/file_object_io.py` & `dfvfs-20240505/dfvfs/file_io/file_object_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/file_io/gpt_file_io.py` & `dfvfs-20240505/dfvfs/file_io/gpt_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/file_io/gzip_file_io.py` & `dfvfs-20240505/dfvfs/file_io/gzip_file_io.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,35 +8,55 @@
 
 
 class GzipFile(file_object_io.FileObjectIO):
   """File input/output (IO) object of a gzip file."""
 
   @property
   def comments(self):
-    """list(str): comments in the gzip file."""
+    """Retrieves the comments.
+
+    Returns:
+      list[str]: comments of the members.
+    """
     return [member.comment for member in self._file_object.members]
 
   @property
   def modification_times(self):
-    """list(int): modification times stored in the gzip file."""
+    """Retrieves the modification times.
+
+    Returns:
+      list[str]: modification times of the members.
+    """
     return [member.modification_time for member in self._file_object.members]
 
   @property
   def original_filenames(self):
-    """list(str): original filenames stored in the gzip file."""
+    """Retrieves the original filenames.
+
+    Returns:
+      list[str]: original filenames of the members.
+    """
     return [member.original_filename for member in self._file_object.members]
 
   @property
   def operating_systems(self):
-    """list(int): operating system values stored in the gzip file."""
+    """Retrieves the operating system values.
+
+    Returns:
+      list[str]: operating system values of the members.
+    """
     return [member.operating_system for member in self._file_object.members]
 
   @property
   def uncompressed_data_size(self):
-    """int: uncompressed data size."""
+    """Retrieves the uncompressed data size.
+
+    Returns:
+      int: uncompressed data size.
+    """
     return self._file_object.uncompressed_data_size
 
   def _OpenFileObject(self, path_spec):
     """Opens the file-like object defined by path specification.
 
     Args:
       path_spec (PathSpec): path specification.
```

### Comparing `dfvfs-20240115/dfvfs/file_io/hfs_file_io.py` & `dfvfs-20240505/dfvfs/file_io/hfs_file_io.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import os
 
 from dfvfs.file_io import file_io
 from dfvfs.resolver import resolver
 
 
 class HFSFile(file_io.FileIO):
-  """File input/output (IO) object using pyfshfs.file_entry"""
+  """File input/output (IO) object using pyfshfs.file_entry."""
 
   def __init__(self, resolver_context, path_spec):
     """Initializes a file input/output (IO) object.
 
     Args:
       resolver_context (Context): resolver context.
       path_spec (PathSpec): a path specification.
```

### Comparing `dfvfs-20240115/dfvfs/file_io/luksde_file_io.py` & `dfvfs-20240505/dfvfs/file_io/luksde_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/file_io/lvm_file_io.py` & `dfvfs-20240505/dfvfs/file_io/lvm_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/file_io/modi_file_io.py` & `dfvfs-20240505/dfvfs/file_io/modi_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/file_io/ntfs_file_io.py` & `dfvfs-20240505/dfvfs/file_io/ntfs_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/file_io/os_file_io.py` & `dfvfs-20240505/dfvfs/file_io/os_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/file_io/phdi_file_io.py` & `dfvfs-20240505/dfvfs/file_io/phdi_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/file_io/qcow_file_io.py` & `dfvfs-20240505/dfvfs/file_io/qcow_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/file_io/raw_file_io.py` & `dfvfs-20240505/dfvfs/file_io/raw_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/file_io/sqlite_blob_file_io.py` & `dfvfs-20240505/dfvfs/file_io/sqlite_blob_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/file_io/tar_file_io.py` & `dfvfs-20240505/dfvfs/file_io/tar_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/file_io/tsk_file_io.py` & `dfvfs-20240505/dfvfs/file_io/tsk_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/file_io/tsk_partition_file_io.py` & `dfvfs-20240505/dfvfs/file_io/tsk_partition_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/file_io/vhdi_file_io.py` & `dfvfs-20240505/dfvfs/file_io/vhdi_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/file_io/vmdk_file_io.py` & `dfvfs-20240505/dfvfs/file_io/vmdk_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/file_io/vshadow_file_io.py` & `dfvfs-20240505/dfvfs/file_io/vshadow_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/file_io/xfs_file_io.py` & `dfvfs-20240505/dfvfs/file_io/xfs_file_io.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from dfvfs.file_io import file_io
 from dfvfs.lib import errors
 from dfvfs.resolver import resolver
 
 
 class XFSFile(file_io.FileIO):
-  """File input/output (IO) object using pyfsxfs.file_entry"""
+  """File input/output (IO) object using pyfsxfs.file_entry."""
 
   def __init__(self, resolver_context, path_spec):
     """Initializes a file input/output (IO) object.
 
     Args:
       resolver_context (Context): resolver context.
       path_spec (PathSpec): a path specification.
```

### Comparing `dfvfs-20240115/dfvfs/file_io/zip_file_io.py` & `dfvfs-20240505/dfvfs/file_io/zip_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/helpers/command_line.py` & `dfvfs-20240505/dfvfs/helpers/command_line.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/helpers/data_slice.py` & `dfvfs-20240505/dfvfs/helpers/data_slice.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/helpers/fake_file_system_builder.py` & `dfvfs-20240505/dfvfs/helpers/fake_file_system_builder.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/helpers/file_system_searcher.py` & `dfvfs-20240505/dfvfs/helpers/file_system_searcher.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/helpers/source_scanner.py` & `dfvfs-20240505/dfvfs/helpers/source_scanner.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,19 @@
     self.path_spec = path_spec
     self.parent_node = None
     self.scanned = False
     self.sub_nodes = []
 
   @property
   def type_indicator(self):
-    """str: path specification type indicator."""
+    """Retrieves the type indicator.
+
+    Returns:
+      str: path specification type indicator.
+    """
     return self.path_spec.type_indicator
 
   def GetSubNodeByLocation(self, location):
     """Retrieves a sub scan node based on the location.
 
     Args:
       location (str): location that should match the location of the path
@@ -161,15 +165,19 @@
     self._scan_nodes = {}
 
     self.source_type = None
     self.updated = False
 
   @property
   def locked_scan_nodes(self):
-    """list[SourceScanNode]: locked scan nodes."""
+    """Retrieves the locked scan nodes.
+
+    Returns:
+      list[SourceScanNode]: locked scan nodes.
+    """
     return list(self._locked_scan_nodes.values())
 
   def AddScanNode(self, path_spec, parent_scan_node):
     """Adds a scan node for a certain path specification.
 
     Args:
       path_spec (PathSpec): path specification.
```

### Comparing `dfvfs-20240115/dfvfs/helpers/text_file.py` & `dfvfs-20240505/dfvfs/helpers/text_file.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/helpers/volume_scanner.py` & `dfvfs-20240505/dfvfs/helpers/volume_scanner.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/helpers/windows_path_resolver.py` & `dfvfs-20240505/dfvfs/helpers/windows_path_resolver.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/lib/apfs_helper.py` & `dfvfs-20240505/dfvfs/lib/apfs_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/lib/apm_helper.py` & `dfvfs-20240505/dfvfs/lib/apm_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/lib/bde_helper.py` & `dfvfs-20240505/dfvfs/lib/bde_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/lib/cpio.py` & `dfvfs-20240505/dfvfs/lib/cpio.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/lib/cpio.yaml` & `dfvfs-20240505/dfvfs/lib/cpio.yaml`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/lib/cs_helper.py` & `dfvfs-20240505/dfvfs/lib/cs_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/lib/data_format.py` & `dfvfs-20240505/dfvfs/lib/data_format.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/lib/decorators.py` & `dfvfs-20240505/dfvfs/lib/decorators.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/lib/definitions.py` & `dfvfs-20240505/dfvfs/lib/definitions.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/lib/errors.py` & `dfvfs-20240505/dfvfs/lib/errors.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/lib/ewf_helper.py` & `dfvfs-20240505/dfvfs/lib/ewf_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/lib/glob2regex.py` & `dfvfs-20240505/dfvfs/lib/glob2regex.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/lib/gzipfile.py` & `dfvfs-20240505/dfvfs/lib/gzipfile.py`

 * *Files 1% similar despite different names*

```diff
@@ -423,15 +423,19 @@
     self._file_object = None
     self._members_by_end_offset = collections.OrderedDict()
 
     self.uncompressed_data_size = 0
 
   @property
   def members(self):
-    """list(GzipMember): members in the gzip file."""
+    """Retrieves the members in the file.
+
+    Returns:
+      list[GzipMember]: members in the file.
+    """
     return list(self._members_by_end_offset.values())
 
   def _GetMemberForOffset(self, offset):
     """Finds the member whose data includes the provided offset.
 
     Args:
       offset (int): offset in the uncompressed data to find the
```

### Comparing `dfvfs-20240115/dfvfs/lib/gzipfile.yaml` & `dfvfs-20240505/dfvfs/lib/gzipfile.yaml`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/lib/luksde_helper.py` & `dfvfs-20240505/dfvfs/lib/luksde_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/lib/lvm_helper.py` & `dfvfs-20240505/dfvfs/lib/lvm_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/lib/raw_helper.py` & `dfvfs-20240505/dfvfs/lib/raw_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/lib/sqlite_database.py` & `dfvfs-20240505/dfvfs/lib/sqlite_database.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/lib/tsk_image.py` & `dfvfs-20240505/dfvfs/lib/tsk_image.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/lib/tsk_partition.py` & `dfvfs-20240505/dfvfs/lib/tsk_partition.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/lib/vshadow_helper.py` & `dfvfs-20240505/dfvfs/lib/vshadow_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/mount/manager.py` & `dfvfs-20240505/dfvfs/mount/manager.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/path/__init__.py` & `dfvfs-20240505/dfvfs/path/__init__.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/path/apfs_container_path_spec.py` & `dfvfs-20240505/dfvfs/path/apfs_container_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/path/apfs_path_spec.py` & `dfvfs-20240505/dfvfs/path/apfs_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/path/apm_path_spec.py` & `dfvfs-20240505/dfvfs/path/apm_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/path/bde_path_spec.py` & `dfvfs-20240505/dfvfs/path/bde_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/path/compressed_stream_path_spec.py` & `dfvfs-20240505/dfvfs/path/compressed_stream_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/path/cpio_path_spec.py` & `dfvfs-20240505/dfvfs/path/cpio_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/path/cs_path_spec.py` & `dfvfs-20240505/dfvfs/path/cs_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/path/data_range_path_spec.py` & `dfvfs-20240505/dfvfs/path/data_range_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/path/encoded_stream_path_spec.py` & `dfvfs-20240505/dfvfs/path/encoded_stream_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/path/encrypted_stream_path_spec.py` & `dfvfs-20240505/dfvfs/path/encrypted_stream_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/path/ewf_path_spec.py` & `dfvfs-20240505/dfvfs/path/ewf_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/path/ext_path_spec.py` & `dfvfs-20240505/dfvfs/path/ext_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/path/factory.py` & `dfvfs-20240505/dfvfs/path/factory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/path/fake_path_spec.py` & `dfvfs-20240505/dfvfs/path/fake_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/path/fat_path_spec.py` & `dfvfs-20240505/dfvfs/path/fat_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/path/gpt_path_spec.py` & `dfvfs-20240505/dfvfs/path/gpt_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/path/gzip_path_spec.py` & `dfvfs-20240505/dfvfs/path/gzip_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/path/hfs_path_spec.py` & `dfvfs-20240505/dfvfs/path/hfs_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/path/location_path_spec.py` & `dfvfs-20240505/dfvfs/path/location_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/path/luksde_path_spec.py` & `dfvfs-20240505/dfvfs/path/luksde_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/path/lvm_path_spec.py` & `dfvfs-20240505/dfvfs/path/lvm_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/path/modi_path_spec.py` & `dfvfs-20240505/dfvfs/path/modi_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/path/mount_path_spec.py` & `dfvfs-20240505/dfvfs/path/mount_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/path/ntfs_path_spec.py` & `dfvfs-20240505/dfvfs/path/ntfs_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/path/os_path_spec.py` & `dfvfs-20240505/dfvfs/path/os_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/path/path_spec.py` & `dfvfs-20240505/dfvfs/path/path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/path/phdi_path_spec.py` & `dfvfs-20240505/dfvfs/path/phdi_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/path/qcow_path_spec.py` & `dfvfs-20240505/dfvfs/path/qcow_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/path/raw_path_spec.py` & `dfvfs-20240505/dfvfs/path/raw_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/path/sqlite_blob_path_spec.py` & `dfvfs-20240505/dfvfs/path/sqlite_blob_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/path/tar_path_spec.py` & `dfvfs-20240505/dfvfs/path/tar_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/path/tsk_partition_path_spec.py` & `dfvfs-20240505/dfvfs/path/tsk_partition_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/path/tsk_path_spec.py` & `dfvfs-20240505/dfvfs/path/tsk_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/path/vhdi_path_spec.py` & `dfvfs-20240505/dfvfs/path/vhdi_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/path/vmdk_path_spec.py` & `dfvfs-20240505/dfvfs/path/vmdk_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/path/vshadow_path_spec.py` & `dfvfs-20240505/dfvfs/path/vshadow_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/path/xfs_path_spec.py` & `dfvfs-20240505/dfvfs/path/xfs_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/path/zip_path_spec.py` & `dfvfs-20240505/dfvfs/path/zip_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/resolver/context.py` & `dfvfs-20240505/dfvfs/resolver/context.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/resolver/resolver.py` & `dfvfs-20240505/dfvfs/resolver/resolver.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/resolver_helpers/__init__.py` & `dfvfs-20240505/dfvfs/resolver_helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/resolver_helpers/apfs_container_resolver_helper.py` & `dfvfs-20240505/dfvfs/resolver_helpers/apfs_container_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/resolver_helpers/apfs_resolver_helper.py` & `dfvfs-20240505/dfvfs/resolver_helpers/apfs_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/resolver_helpers/apm_resolver_helper.py` & `dfvfs-20240505/dfvfs/resolver_helpers/apm_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/resolver_helpers/bde_resolver_helper.py` & `dfvfs-20240505/dfvfs/resolver_helpers/bde_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/resolver_helpers/compressed_stream_resolver_helper.py` & `dfvfs-20240505/dfvfs/resolver_helpers/compressed_stream_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/resolver_helpers/cpio_resolver_helper.py` & `dfvfs-20240505/dfvfs/resolver_helpers/cpio_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/resolver_helpers/cs_resolver_helper.py` & `dfvfs-20240505/dfvfs/resolver_helpers/cs_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/resolver_helpers/data_range_resolver_helper.py` & `dfvfs-20240505/dfvfs/resolver_helpers/data_range_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/resolver_helpers/encoded_stream_resolver_helper.py` & `dfvfs-20240505/dfvfs/resolver_helpers/encoded_stream_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/resolver_helpers/encrypted_stream_resolver_helper.py` & `dfvfs-20240505/dfvfs/resolver_helpers/encrypted_stream_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/resolver_helpers/ewf_resolver_helper.py` & `dfvfs-20240505/dfvfs/resolver_helpers/ewf_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/resolver_helpers/ext_resolver_helper.py` & `dfvfs-20240505/dfvfs/resolver_helpers/ext_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/resolver_helpers/fake_resolver_helper.py` & `dfvfs-20240505/dfvfs/resolver_helpers/fake_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/resolver_helpers/fat_resolver_helper.py` & `dfvfs-20240505/dfvfs/resolver_helpers/fat_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/resolver_helpers/gpt_resolver_helper.py` & `dfvfs-20240505/dfvfs/resolver_helpers/gpt_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/resolver_helpers/gzip_resolver_helper.py` & `dfvfs-20240505/dfvfs/resolver_helpers/gzip_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/resolver_helpers/hfs_resolver_helper.py` & `dfvfs-20240505/dfvfs/resolver_helpers/hfs_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/resolver_helpers/luksde_resolver_helper.py` & `dfvfs-20240505/dfvfs/resolver_helpers/luksde_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/resolver_helpers/lvm_resolver_helper.py` & `dfvfs-20240505/dfvfs/resolver_helpers/lvm_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/resolver_helpers/manager.py` & `dfvfs-20240505/dfvfs/resolver_helpers/manager.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/resolver_helpers/modi_resolver_helper.py` & `dfvfs-20240505/dfvfs/resolver_helpers/modi_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/resolver_helpers/ntfs_resolver_helper.py` & `dfvfs-20240505/dfvfs/resolver_helpers/ntfs_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/resolver_helpers/os_resolver_helper.py` & `dfvfs-20240505/dfvfs/resolver_helpers/os_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/resolver_helpers/phdi_resolver_helper.py` & `dfvfs-20240505/dfvfs/resolver_helpers/phdi_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/resolver_helpers/qcow_resolver_helper.py` & `dfvfs-20240505/dfvfs/resolver_helpers/qcow_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/resolver_helpers/raw_resolver_helper.py` & `dfvfs-20240505/dfvfs/resolver_helpers/raw_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/resolver_helpers/resolver_helper.py` & `dfvfs-20240505/dfvfs/resolver_helpers/resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/resolver_helpers/sqlite_blob_resolver_helper.py` & `dfvfs-20240505/dfvfs/resolver_helpers/sqlite_blob_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/resolver_helpers/tar_resolver_helper.py` & `dfvfs-20240505/dfvfs/resolver_helpers/tar_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/resolver_helpers/tsk_partition_resolver_helper.py` & `dfvfs-20240505/dfvfs/resolver_helpers/tsk_partition_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/resolver_helpers/tsk_resolver_helper.py` & `dfvfs-20240505/dfvfs/resolver_helpers/tsk_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/resolver_helpers/vhdi_resolver_helper.py` & `dfvfs-20240505/dfvfs/resolver_helpers/vhdi_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/resolver_helpers/vmdk_resolver_helper.py` & `dfvfs-20240505/dfvfs/resolver_helpers/vmdk_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/resolver_helpers/vshadow_resolver_helper.py` & `dfvfs-20240505/dfvfs/resolver_helpers/vshadow_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/resolver_helpers/xfs_resolver_helper.py` & `dfvfs-20240505/dfvfs/resolver_helpers/xfs_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/resolver_helpers/zip_resolver_helper.py` & `dfvfs-20240505/dfvfs/resolver_helpers/zip_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/serializer/json_serializer.py` & `dfvfs-20240505/dfvfs/serializer/json_serializer.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/serializer/serializer.py` & `dfvfs-20240505/dfvfs/serializer/serializer.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/vfs/apfs_attribute.py` & `dfvfs-20240505/dfvfs/vfs/apfs_attribute.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/vfs/apfs_container_directory.py` & `dfvfs-20240505/dfvfs/vfs/apfs_container_directory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/vfs/apfs_container_file_entry.py` & `dfvfs-20240505/dfvfs/vfs/apfs_container_file_entry.py`

 * *Files 6% similar despite different names*

```diff
@@ -76,15 +76,19 @@
         yield APFSContainerFileEntry(
             self._resolver_context, self._file_system, path_spec)
 
   # TODO: expose date and time values.
 
   @property
   def name(self):
-    """str: name of the file entry, which does not include the full path."""
+    """Retrieves the name.
+
+    Return:
+      str: name of the file entry, which does not include the full path.
+    """
     if self._name is None:
       self._name = ''
 
       # Prefer generating the name seeing that the APFS container back-end
       # supports aliases, such as "/apfs1" and "/apfs{UUID}".
       if self._volume_index is not None:
         apfs_volume_index = self._volume_index + 1
@@ -94,24 +98,32 @@
         if location is not None:
           self._name = self._file_system.BasenamePath(location)
 
     return self._name
 
   @property
   def size(self):
-    """int: size of the file entry in bytes or None if not available."""
+    """Retrieves the size.
+
+    Returns:
+      int: size of the file entry in bytes or None if not available.
+    """
     if self._fsapfs_volume is None:
       return None
 
     # TODO: change libfsapfs so self._fsapfs_volume.size works
     return 0
 
   @property
   def sub_file_entries(self):
-    """generator[APFSContainerFileEntry]: sub file entries."""
+    """Retrieves sub file entries.
+
+    Returns:
+      generator[APFSContainerFileEntry]: sub file entries.
+    """
     return self._GetSubFileEntries()
 
   def GetAPFSVolume(self):
     """Retrieves an APFS volume.
 
     Returns:
       pyfsapfs.volume: an APFS volume or None if not available.
```

### Comparing `dfvfs-20240115/dfvfs/vfs/apfs_container_file_system.py` & `dfvfs-20240505/dfvfs/vfs/apfs_container_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/vfs/apfs_directory.py` & `dfvfs-20240505/dfvfs/vfs/apfs_directory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/vfs/apfs_file_entry.py` & `dfvfs-20240505/dfvfs/vfs/apfs_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/vfs/apfs_file_system.py` & `dfvfs-20240505/dfvfs/vfs/apfs_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/vfs/apm_directory.py` & `dfvfs-20240505/dfvfs/vfs/apm_directory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/vfs/apm_file_entry.py` & `dfvfs-20240505/dfvfs/vfs/apm_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/vfs/apm_file_system.py` & `dfvfs-20240505/dfvfs/vfs/apm_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/vfs/attribute.py` & `dfvfs-20240505/dfvfs/vfs/attribute.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/vfs/bde_file_entry.py` & `dfvfs-20240505/dfvfs/vfs/bde_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/vfs/bde_file_system.py` & `dfvfs-20240505/dfvfs/vfs/bde_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/vfs/compressed_stream_file_entry.py` & `dfvfs-20240505/dfvfs/vfs/compressed_stream_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/vfs/compressed_stream_file_system.py` & `dfvfs-20240505/dfvfs/vfs/compressed_stream_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/vfs/cpio_directory.py` & `dfvfs-20240505/dfvfs/vfs/cpio_directory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/vfs/cpio_file_entry.py` & `dfvfs-20240505/dfvfs/vfs/cpio_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/vfs/cpio_file_system.py` & `dfvfs-20240505/dfvfs/vfs/cpio_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/vfs/cs_directory.py` & `dfvfs-20240505/dfvfs/vfs/cs_directory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/vfs/cs_file_entry.py` & `dfvfs-20240505/dfvfs/vfs/cs_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/vfs/cs_file_system.py` & `dfvfs-20240505/dfvfs/vfs/cs_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/vfs/data_range_file_entry.py` & `dfvfs-20240505/dfvfs/vfs/data_range_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/vfs/data_range_file_system.py` & `dfvfs-20240505/dfvfs/vfs/data_range_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/vfs/data_stream.py` & `dfvfs-20240505/dfvfs/vfs/data_stream.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/vfs/directory.py` & `dfvfs-20240505/dfvfs/vfs/directory.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,9 +30,13 @@
     Returns:
       generator[PathSpec]: path specification generator.
     """
     return iter(())
 
   @property
   def entries(self):
-    """generator[PathSpec]: path specifications of the directory entries."""
+    """Retrieves directory entries.
+
+    Returns:
+      generator[PathSpec]: path specifications of the directory entries.
+    """
     return self._EntriesGenerator()
```

### Comparing `dfvfs-20240115/dfvfs/vfs/encoded_stream_file_entry.py` & `dfvfs-20240505/dfvfs/vfs/encoded_stream_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/vfs/encoded_stream_file_system.py` & `dfvfs-20240505/dfvfs/vfs/encoded_stream_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/vfs/encrypted_stream_file_entry.py` & `dfvfs-20240505/dfvfs/vfs/encrypted_stream_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/vfs/encrypted_stream_file_system.py` & `dfvfs-20240505/dfvfs/vfs/encrypted_stream_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/vfs/ext_attribute.py` & `dfvfs-20240505/dfvfs/vfs/ext_attribute.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/vfs/ext_directory.py` & `dfvfs-20240505/dfvfs/vfs/ext_directory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/vfs/ext_file_entry.py` & `dfvfs-20240505/dfvfs/vfs/ext_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/vfs/ext_file_system.py` & `dfvfs-20240505/dfvfs/vfs/ext_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/vfs/extent.py` & `dfvfs-20240505/dfvfs/vfs/extent.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/vfs/fake_directory.py` & `dfvfs-20240505/dfvfs/vfs/fake_directory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/vfs/fake_file_entry.py` & `dfvfs-20240505/dfvfs/vfs/fake_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/vfs/fake_file_system.py` & `dfvfs-20240505/dfvfs/vfs/fake_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/vfs/fat_directory.py` & `dfvfs-20240505/dfvfs/vfs/fat_directory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/vfs/fat_file_entry.py` & `dfvfs-20240505/dfvfs/vfs/fat_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/vfs/fat_file_system.py` & `dfvfs-20240505/dfvfs/vfs/fat_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/vfs/file_entry.py` & `dfvfs-20240505/dfvfs/vfs/file_entry.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 """The Virtual File System (VFS) file entry interface.
 
-The file entry can be various file system elements like a regular file,
-a directory or file system metadata.
+The file entry can be various file system elements like a regular file, a
+directory or file system metadata.
 """
 
 import abc
 
 from dfvfs.lib import definitions
 from dfvfs.resolver import resolver
 from dfvfs.vfs import data_stream
@@ -118,108 +118,175 @@
 
     Yields:
       FileEntry: a sub file entry.
     """
 
   @property
   def access_time(self):
-    """dfdatetime.DateTimeValues: access time or None if not available."""
+    """Retrieves the access time.
+
+    Returns:
+      dfdatetime.DateTimeValues: access time or None if not available.
+    """
     return None
 
   @property
   def added_time(self):
-    """dfdatetime.DateTimeValues: added time or None if not available."""
+    """Retrieves the added time.
+
+    Returns:
+      dfdatetime.DateTimeValues: added time or None if not available.
+    """
     return None
 
   @property
   def attributes(self):
-    """generator[Attribute]: attributes."""
+    """Retrieves attributes.
+
+    Returns:
+      generator[Attribute]: attributes.
+    """
     return self._GetAttributes()
 
   @property
   def backup_time(self):
-    """dfdatetime.DateTimeValues: backup time or None if not available."""
+    """Retrieves the backup time.
+
+    Returns:
+      dfdatetime.DateTimeValues: backup time or None if not available.
+    """
     return None
 
   @property
   def change_time(self):
-    """dfdatetime.DateTimeValues: change time or None if not available."""
+    """Retrieves the change time.
+
+    Returns:
+      dfdatetime.DateTimeValues: change time or None if not available.
+    """
     return None
 
   @property
   def creation_time(self):
-    """dfdatetime.DateTimeValues: creation time or None if not available."""
+    """Retrieves the creation time.
+
+    Returns:
+      dfdatetime.DateTimeValues: creation time or None if not available.
+    """
     return None
 
   @property
   def deletion_time(self):
-    """dfdatetime.DateTimeValues: deletion time or None if not available."""
+    """Retrieves the deletion time.
+
+    Returns:
+      dfdatetime.DateTimeValues: deletion time or None if not available.
+    """
     return None
 
   @property
   def data_streams(self):
-    """generator[DataStream]: data streams."""
+    """Retrieves data streams.
+
+    Returns:
+      generator[DataStream]: data streams.
+    """
     return self._GetDataStreams()
 
   @property
   def link(self):
-    """str: full path of the linked file entry or None if not available."""
+    """Retrieves the path of a linked file entry.
+
+    Returns:
+      str: full path of the linked file entry or None if not available.
+    """
     if not self.IsLink():
       return None
 
     return self._GetLink()
 
   @property
   def modification_time(self):
-    """dfdatetime.DateTimeValues: modification time or None if not available."""
+    """Retrieves the modification time.
+
+    Returns:
+      dfdatetime.DateTimeValues: modification time or None if not available.
+    """
     return None
 
   @property
   @abc.abstractmethod
   def name(self):
-    """str: name of the file entry, without the full path."""
+    """Retrieves the name.
+
+    Returns:
+      str: name of the file entry, without the full path.
+    """
 
   @property
   def number_of_attributes(self):
-    """int: number of attributes."""
+    """Retrieves the number of attributes.
+
+    Returns:
+      int: number of attributes.
+    """
     attributes = self._GetAttributes()
     return len(attributes)
 
   @property
   def number_of_data_streams(self):
-    """int: number of data streams."""
+    """Retrieves the number of data streams.
+
+    Returns:
+      int: number of data streams.
+    """
     data_streams = self._GetDataStreams()
     return len(data_streams)
 
   @property
   def number_of_sub_file_entries(self):
-    """int: number of sub file entries."""
+    """Retrieves the number of sub file entries.
+
+    Returns:
+      int: number of sub file entries.
+    """
     number_of_sub_file_entries = 0
     if self.entry_type == definitions.FILE_ENTRY_TYPE_DIRECTORY:
       directory = self._GetDirectory()
       # We cannot use len(directory.entries) since entries is a generator.
       number_of_sub_file_entries = sum(1 for path_spec in directory.entries)
 
     return number_of_sub_file_entries
 
   @property
   def size(self):
-    """int: size of the file entry in bytes or None if not available."""
+    """Retrieves the size.
+
+    Returns:
+      int: size of the file entry in bytes or None if not available.
+    """
     return None
 
   @property
   def sub_file_entries(self):
-    """generator[FileEntry]: sub file entries."""
+    """Retrieves sub file entries.
+
+    Returns:
+      generator[FileEntry]: sub file entries.
+    """
     return self._GetSubFileEntries()
 
   @property
   def type_indicator(self):
-    """str: type indicator."""
-    # pylint: disable=no-member
-    return self.TYPE_INDICATOR
+    """Retrieves the type indicator.
+
+    Returns:
+      str: type indicator.
+    """
+    return getattr(self, 'TYPE_INDICATOR', None)
 
   def GetDataStream(self, name, case_sensitive=True):
     """Retrieves a data stream by name.
 
     Args:
       name (str): name of the data stream.
       case_sensitive (Optional[bool]): True if the name is case sensitive.
```

### Comparing `dfvfs-20240115/dfvfs/vfs/file_system.py` & `dfvfs-20240505/dfvfs/vfs/file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/vfs/gpt_directory.py` & `dfvfs-20240505/dfvfs/vfs/gpt_directory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/vfs/gpt_file_entry.py` & `dfvfs-20240505/dfvfs/vfs/gpt_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/vfs/gpt_file_system.py` & `dfvfs-20240505/dfvfs/vfs/gpt_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/vfs/gzip_file_entry.py` & `dfvfs-20240505/dfvfs/vfs/gzip_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/vfs/gzip_file_system.py` & `dfvfs-20240505/dfvfs/vfs/gzip_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/vfs/hfs_attribute.py` & `dfvfs-20240505/dfvfs/vfs/hfs_attribute.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/vfs/hfs_data_stream.py` & `dfvfs-20240505/dfvfs/vfs/hfs_data_stream.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/vfs/hfs_directory.py` & `dfvfs-20240505/dfvfs/vfs/hfs_directory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/vfs/hfs_file_entry.py` & `dfvfs-20240505/dfvfs/vfs/hfs_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/vfs/hfs_file_system.py` & `dfvfs-20240505/dfvfs/vfs/hfs_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/vfs/luksde_file_entry.py` & `dfvfs-20240505/dfvfs/vfs/luksde_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/vfs/luksde_file_system.py` & `dfvfs-20240505/dfvfs/vfs/luksde_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/vfs/lvm_directory.py` & `dfvfs-20240505/dfvfs/vfs/lvm_directory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/vfs/lvm_file_entry.py` & `dfvfs-20240505/dfvfs/vfs/lvm_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/vfs/lvm_file_system.py` & `dfvfs-20240505/dfvfs/vfs/lvm_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/vfs/ntfs_attribute.py` & `dfvfs-20240505/dfvfs/vfs/ntfs_attribute.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/vfs/ntfs_data_stream.py` & `dfvfs-20240505/dfvfs/vfs/ntfs_data_stream.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/vfs/ntfs_directory.py` & `dfvfs-20240505/dfvfs/vfs/ntfs_directory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/vfs/ntfs_file_entry.py` & `dfvfs-20240505/dfvfs/vfs/ntfs_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/vfs/ntfs_file_system.py` & `dfvfs-20240505/dfvfs/vfs/ntfs_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/vfs/os_attribute.py` & `dfvfs-20240505/dfvfs/vfs/os_attribute.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/vfs/os_directory.py` & `dfvfs-20240505/dfvfs/vfs/os_directory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/vfs/os_file_entry.py` & `dfvfs-20240505/dfvfs/vfs/os_file_entry.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # -*- coding: utf-8 -*-
 """The operating system file entry implementation."""
 
 import os
 import platform
 import stat
+import sys
 
 import pysmdev
 
 try:
   import xattr
 except ImportError:
   xattr = None
@@ -24,14 +25,15 @@
 
 class OSFileEntry(file_entry.FileEntry):
   """File system file entry that uses os."""
 
   TYPE_INDICATOR = definitions.TYPE_INDICATOR_OS
 
   _OS_IS_WINDOWS = platform.system() == 'Windows'
+  _PY_3_11_AND_EARLIER = bool(tuple(sys.version_info[0:2]) <= (3, 11))
 
   def __init__(self, resolver_context, file_system, path_spec, is_root=False):
     """Initializes a file entry.
 
     Args:
       resolver_context (Context): resolver context.
       file_system (FileSystem): file system.
@@ -222,15 +224,15 @@
   def creation_time(self):
     """dfdatetime.DateTimeValues: creation time or None if not available."""
     if self._stat_info is None:
       return None
 
     # Per Python os.stat() documentation the value of stat_results.st_ctime
     # contains the creation time on Windows.
-    if self._OS_IS_WINDOWS:
+    if self._OS_IS_WINDOWS and self._PY_3_11_AND_EARLIER:
       timestamp = getattr(self._stat_info, 'st_ctime_ns', None)
       if timestamp is not None:
         return dfdatetime_posix_time.PosixTimeInNanoseconds(timestamp=timestamp)
 
       timestamp = int(self._stat_info.st_ctime)
 
     else:
```

### Comparing `dfvfs-20240115/dfvfs/vfs/os_file_system.py` & `dfvfs-20240505/dfvfs/vfs/os_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/vfs/root_only_file_entry.py` & `dfvfs-20240505/dfvfs/vfs/root_only_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/vfs/root_only_file_system.py` & `dfvfs-20240505/dfvfs/vfs/root_only_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/vfs/sqlite_blob_directory.py` & `dfvfs-20240505/dfvfs/vfs/sqlite_blob_directory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/vfs/sqlite_blob_file_entry.py` & `dfvfs-20240505/dfvfs/vfs/sqlite_blob_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/vfs/sqlite_blob_file_system.py` & `dfvfs-20240505/dfvfs/vfs/sqlite_blob_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/vfs/tar_directory.py` & `dfvfs-20240505/dfvfs/vfs/tar_directory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/vfs/tar_file_entry.py` & `dfvfs-20240505/dfvfs/vfs/tar_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/vfs/tar_file_system.py` & `dfvfs-20240505/dfvfs/vfs/tar_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/vfs/tsk_attribute.py` & `dfvfs-20240505/dfvfs/vfs/tsk_attribute.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/vfs/tsk_data_stream.py` & `dfvfs-20240505/dfvfs/vfs/tsk_data_stream.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/vfs/tsk_directory.py` & `dfvfs-20240505/dfvfs/vfs/tsk_directory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/vfs/tsk_file_entry.py` & `dfvfs-20240505/dfvfs/vfs/tsk_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/vfs/tsk_file_system.py` & `dfvfs-20240505/dfvfs/vfs/tsk_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/vfs/tsk_partition_directory.py` & `dfvfs-20240505/dfvfs/vfs/tsk_partition_directory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/vfs/tsk_partition_file_entry.py` & `dfvfs-20240505/dfvfs/vfs/tsk_partition_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/vfs/tsk_partition_file_system.py` & `dfvfs-20240505/dfvfs/vfs/tsk_partition_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/vfs/vshadow_directory.py` & `dfvfs-20240505/dfvfs/vfs/vshadow_directory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/vfs/vshadow_file_entry.py` & `dfvfs-20240505/dfvfs/vfs/vshadow_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/vfs/vshadow_file_system.py` & `dfvfs-20240505/dfvfs/vfs/vshadow_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/vfs/xfs_attribute.py` & `dfvfs-20240505/dfvfs/vfs/xfs_attribute.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/vfs/xfs_directory.py` & `dfvfs-20240505/dfvfs/vfs/xfs_directory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/vfs/xfs_file_entry.py` & `dfvfs-20240505/dfvfs/vfs/xfs_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/vfs/xfs_file_system.py` & `dfvfs-20240505/dfvfs/vfs/xfs_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/vfs/zip_directory.py` & `dfvfs-20240505/dfvfs/vfs/zip_directory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/vfs/zip_file_entry.py` & `dfvfs-20240505/dfvfs/vfs/zip_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/vfs/zip_file_system.py` & `dfvfs-20240505/dfvfs/vfs/zip_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/volume/apfs_volume_system.py` & `dfvfs-20240505/dfvfs/volume/apfs_volume_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/volume/apm_volume_system.py` & `dfvfs-20240505/dfvfs/volume/apm_volume_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/volume/cs_volume_system.py` & `dfvfs-20240505/dfvfs/volume/cs_volume_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/volume/factory.py` & `dfvfs-20240505/dfvfs/volume/factory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/volume/gpt_volume_system.py` & `dfvfs-20240505/dfvfs/volume/gpt_volume_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/volume/lvm_volume_system.py` & `dfvfs-20240505/dfvfs/volume/lvm_volume_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/volume/tsk_volume_system.py` & `dfvfs-20240505/dfvfs/volume/tsk_volume_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs/volume/volume_system.py` & `dfvfs-20240505/dfvfs/volume/volume_system.py`

 * *Files 8% similar despite different names*

```diff
@@ -76,42 +76,58 @@
 
   @abc.abstractmethod
   def _Parse(self):
     """Extracts attributes and extents from the volume."""
 
   @property
   def attributes(self):
-    """generator[VolumeAttribute]: volume attributes generator."""
+    """Retrieves attributes.
+
+    Returns:
+      generator[VolumeAttribute]: volume attributes generator.
+    """
     if not self._is_parsed:
       self._Parse()
       self._is_parsed = True
 
     return iter(self._attributes.values())
 
   @property
   def extents(self):
-    """list[VolumeExtent]: volume extents."""
+    """Retrieves extents.
+
+    Returns:
+      list[VolumeExtent]: volume extents.
+    """
     if not self._is_parsed:
       self._Parse()
       self._is_parsed = True
 
     return self._extents
 
   @property
   def number_of_attributes(self):
-    """int: number of attributes."""
+    """Retrieves the number of attributes.
+
+    Returns:
+      int: number of attributes.
+    """
     if not self._is_parsed:
       self._Parse()
       self._is_parsed = True
 
     return len(self._attributes)
 
   @property
   def number_of_extents(self):
-    """int: number of extents."""
+    """Retrieves the number of extents.
+
+    Returns:
+      int: number of extents.
+    """
     if not self._is_parsed:
       self._Parse()
       self._is_parsed = True
 
     return len(self._extents)
 
   def GetAttribute(self, identifier):
@@ -177,51 +193,71 @@
 
   @abc.abstractmethod
   def _Parse(self):
     """Extracts sections and volumes from the volume system."""
 
   @property
   def number_of_sections(self):
-    """int: number of sections."""
+    """Retrieves the number of sections.
+
+    Returns:
+      int: number of sections.
+    """
     if not self._is_parsed:
       self._Parse()
       self._is_parsed = True
 
     return len(self._sections)
 
   @property
   def number_of_volumes(self):
-    """int: number of volumes."""
+    """Retrieves the number of volumes.
+
+    Returns:
+      int: number of volumes.
+    """
     if not self._is_parsed:
       self._Parse()
       self._is_parsed = True
 
     return len(self._volumes)
 
   @property
   def sections(self):
-    """list[VolumeExtent]: sections."""
+    """Retrieves sections.
+
+    Returns:
+      list[VolumeExtent]: sections.
+    """
     if not self._is_parsed:
       self._Parse()
       self._is_parsed = True
 
     return self._sections
 
   @property
   def volume_identifiers(self):
-    """list[str]: volume identifiers."""
+    """Retrieves volume identifiers.
+
+    Returns:
+      list[str]: volume identifiers.
+    """
     if not self._is_parsed:
       self._Parse()
       self._is_parsed = True
 
     return list(self._volume_identifiers)
 
   @property
   def volumes(self):
-    """generator(Volume): volumes generator."""
+    """Retrieves volumes.
+
+    Returns:
+      generator(Volume): volumes generator.
+    """
     if not self._is_parsed:
       self._Parse()
       self._is_parsed = True
 
     return iter(self._volumes.values())
 
   def GetSectionByIndex(self, section_index):
```

### Comparing `dfvfs-20240115/dfvfs/volume/vshadow_volume_system.py` & `dfvfs-20240505/dfvfs/volume/vshadow_volume_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs.egg-info/SOURCES.txt` & `dfvfs-20240505/dfvfs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/dfvfs.egg-info/requires.txt` & `dfvfs-20240505/dfvfs.egg-info/requires.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 PyYAML>=3.10
-cffi>=1.9.1
 dfdatetime>=20221112
 dtfabric>=20230518
 libbde-python>=20220121
 libcaes-python>=20240114
 libewf-python>=20131210
 libfcrypto-python>=20240114
 libfsapfs-python>=20220709
```

### Comparing `dfvfs-20240115/dfvfs.ini` & `dfvfs-20240505/dfvfs.ini`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/docs/conf.py` & `dfvfs-20240505/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,14 +48,15 @@
 
 autodoc_mock_imports = sorted(modules_to_mock)
 
 # Options for the Sphinx Napoleon extension, which reads Google-style
 # docstrings.
 napoleon_google_docstring = True
 napoleon_numpy_docstring = False
+napoleon_include_init_with_doc = True
 napoleon_include_private_with_doc = False
 napoleon_include_special_with_doc = True
 
 # General information about the project.
 # pylint: disable=redefined-builtin
 project = 'dfVFS'
 copyright = 'The dfVFS authors'
```

### Comparing `dfvfs-20240115/docs/index.rst` & `dfvfs-20240505/docs/index.rst`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/docs/sources/Code-snippets.md` & `dfvfs-20240505/docs/sources/Code-snippets.md`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/docs/sources/Path-specifications.md` & `dfvfs-20240505/docs/sources/Path-specifications.md`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/docs/sources/Supported-formats.md` & `dfvfs-20240505/docs/sources/Supported-formats.md`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/docs/sources/api/dfvfs.analyzer.rst` & `dfvfs-20240505/docs/sources/api/dfvfs.analyzer.rst`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/docs/sources/api/dfvfs.compression.rst` & `dfvfs-20240505/docs/sources/api/dfvfs.compression.rst`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/docs/sources/api/dfvfs.credentials.rst` & `dfvfs-20240505/docs/sources/api/dfvfs.credentials.rst`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/docs/sources/api/dfvfs.encoding.rst` & `dfvfs-20240505/docs/sources/api/dfvfs.encoding.rst`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/docs/sources/api/dfvfs.encryption.rst` & `dfvfs-20240505/docs/sources/api/dfvfs.encryption.rst`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/docs/sources/api/dfvfs.file_io.rst` & `dfvfs-20240505/docs/sources/api/dfvfs.file_io.rst`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/docs/sources/api/dfvfs.helpers.rst` & `dfvfs-20240505/docs/sources/api/dfvfs.helpers.rst`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/docs/sources/api/dfvfs.lib.rst` & `dfvfs-20240505/docs/sources/api/dfvfs.lib.rst`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/docs/sources/api/dfvfs.path.rst` & `dfvfs-20240505/docs/sources/api/dfvfs.path.rst`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/docs/sources/api/dfvfs.resolver_helpers.rst` & `dfvfs-20240505/docs/sources/api/dfvfs.resolver_helpers.rst`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/docs/sources/api/dfvfs.serializer.rst` & `dfvfs-20240505/docs/sources/api/dfvfs.serializer.rst`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/docs/sources/api/dfvfs.vfs.rst` & `dfvfs-20240505/docs/sources/api/dfvfs.vfs.rst`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/docs/sources/api/dfvfs.volume.rst` & `dfvfs-20240505/docs/sources/api/dfvfs.volume.rst`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/docs/sources/developer/Adding-new-type.md` & `dfvfs-20240505/docs/sources/developer/Adding-new-type.md`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/docs/sources/developer/Helpers.md` & `dfvfs-20240505/docs/sources/developer/Helpers.md`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/docs/sources/developer/Internals.md` & `dfvfs-20240505/docs/sources/developer/Internals.md`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/docs/sources/user/Installation-instructions.md` & `dfvfs-20240505/docs/sources/user/Installation-instructions.md`

 * *Files 8% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 To deactivate the virtualenv run:
 
 ```bash
 deactivate
 ```
 
-## Ubuntu 18.04 and 20.04 LTS
+## Ubuntu 22.04 LTS
 
 To install dfVFS from the [GIFT Personal Package Archive (PPA)](https://launchpad.net/~gift):
 
 ```bash
 sudo add-apt-repository ppa:gift/stable
 ```
 
@@ -45,22 +45,22 @@
 ## Windows
 
 The [l2tbinaries](https://github.com/log2timeline/l2tbinaries) contains the
 necessary packages for running dfVFS. l2tbinaries provides the following
 branches:
 
 * main; branch intended for the "packaged release" of dfVFS and dependencies;
+* staging; branch intended for testing pre-releases of dfVFS;
 * dev; branch intended for the "development release" of dfVFS;
 * testing; branch intended for testing newly created packages.
 
 The l2tdevtools project provides [an update script](https://github.com/log2timeline/l2tdevtools/wiki/Update-script)
 to ease the process of keeping the dependencies up to date.
 
-The script requires [pywin32](https://github.com/mhammond/pywin32/releases) and
-[Python WMI](https://pypi.org/project/WMI).
+The script requires [pywin32](https://github.com/mhammond/pywin32/releases).
 
 To install the release versions of the dependencies run:
 
 ```
 set PYTHONPATH=.
 
 C:\Python3\python.exe tools\update.py --preset dfvfs
```

### Comparing `dfvfs-20240115/requirements.txt` & `dfvfs-20240505/requirements.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 PyYAML >= 3.10
-cffi >= 1.9.1
 dfdatetime >= 20221112
 dtfabric >= 20230518
 libbde-python >= 20220121
 libcaes-python >= 20240114
 libewf-python >= 20131210
 libfcrypto-python >= 20240114
 libfsapfs-python >= 20220709
```

### Comparing `dfvfs-20240115/run_tests.py` & `dfvfs-20240505/run_tests.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/analyzer/analyzer.py` & `dfvfs-20240505/tests/analyzer/analyzer.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/analyzer/specification.py` & `dfvfs-20240505/tests/analyzer/specification.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/compression/bzip2_decompressor.py` & `dfvfs-20240505/tests/compression/bzip2_decompressor.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/compression/manager.py` & `dfvfs-20240505/tests/compression/manager.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/compression/xz_decompressor.py` & `dfvfs-20240505/tests/compression/xz_decompressor.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/compression/zlib_decompressor.py` & `dfvfs-20240505/tests/compression/zlib_decompressor.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/credentials/apfs_credentials.py` & `dfvfs-20240505/tests/credentials/apfs_credentials.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/credentials/bde_credentials.py` & `dfvfs-20240505/tests/credentials/bde_credentials.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/credentials/cs_credentials.py` & `dfvfs-20240505/tests/credentials/cs_credentials.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/credentials/encrypted_stream_credentials.py` & `dfvfs-20240505/tests/credentials/encrypted_stream_credentials.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/credentials/keychain.py` & `dfvfs-20240505/tests/credentials/keychain.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/credentials/luksde_credentials.py` & `dfvfs-20240505/tests/credentials/luksde_credentials.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/credentials/manager.py` & `dfvfs-20240505/tests/credentials/manager.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/encoding/base16_decoder.py` & `dfvfs-20240505/tests/encoding/base16_decoder.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/encoding/base32_decoder.py` & `dfvfs-20240505/tests/encoding/base32_decoder.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/encoding/base64_decoder.py` & `dfvfs-20240505/tests/encoding/base64_decoder.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/encoding/manager.py` & `dfvfs-20240505/tests/encoding/manager.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/encryption/aes_decrypter.py` & `dfvfs-20240505/tests/encryption/aes_decrypter.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/encryption/blowfish_decrypter.py` & `dfvfs-20240505/tests/encryption/blowfish_decrypter.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/encryption/decrypter.py` & `dfvfs-20240505/tests/encryption/decrypter.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/encryption/des3_decrypter.py` & `dfvfs-20240505/tests/encryption/des3_decrypter.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/encryption/manager.py` & `dfvfs-20240505/tests/encryption/manager.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/encryption/rc4_decrypter.py` & `dfvfs-20240505/tests/encryption/rc4_decrypter.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/file_io/apfs_file_io.py` & `dfvfs-20240505/tests/file_io/apfs_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/file_io/apm_file_io.py` & `dfvfs-20240505/tests/file_io/apm_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/file_io/bde_file_io.py` & `dfvfs-20240505/tests/file_io/bde_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/file_io/compressed_stream_io.py` & `dfvfs-20240505/tests/file_io/compressed_stream_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/file_io/cpio_file_io.py` & `dfvfs-20240505/tests/file_io/cpio_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/file_io/cs_file_io.py` & `dfvfs-20240505/tests/file_io/cs_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/file_io/data_range_io.py` & `dfvfs-20240505/tests/file_io/data_range_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/file_io/encoded_stream_io.py` & `dfvfs-20240505/tests/file_io/encoded_stream_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/file_io/encrypted_stream_io.py` & `dfvfs-20240505/tests/file_io/encrypted_stream_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/file_io/ewf_file_io.py` & `dfvfs-20240505/tests/file_io/ewf_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/file_io/ext_file_io.py` & `dfvfs-20240505/tests/file_io/ext_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/file_io/fake_file_io.py` & `dfvfs-20240505/tests/file_io/fake_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/file_io/fat_file_io.py` & `dfvfs-20240505/tests/file_io/fat_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/file_io/gpt_file_io.py` & `dfvfs-20240505/tests/file_io/gpt_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/file_io/gzip_file_io.py` & `dfvfs-20240505/tests/file_io/gzip_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/file_io/hfs_file_io.py` & `dfvfs-20240505/tests/file_io/hfs_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/file_io/luksde_file_io.py` & `dfvfs-20240505/tests/file_io/luksde_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/file_io/lvm_file_io.py` & `dfvfs-20240505/tests/file_io/lvm_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/file_io/modi_file_io.py` & `dfvfs-20240505/tests/file_io/modi_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/file_io/ntfs_file_io.py` & `dfvfs-20240505/tests/file_io/ntfs_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/file_io/os_file_io.py` & `dfvfs-20240505/tests/file_io/os_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/file_io/phdi_file_io.py` & `dfvfs-20240505/tests/file_io/phdi_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/file_io/qcow_file_io.py` & `dfvfs-20240505/tests/file_io/qcow_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/file_io/raw_file_io.py` & `dfvfs-20240505/tests/file_io/raw_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/file_io/sqlite_blob_file_io.py` & `dfvfs-20240505/tests/file_io/sqlite_blob_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/file_io/tar_file_io.py` & `dfvfs-20240505/tests/file_io/tar_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/file_io/test_lib.py` & `dfvfs-20240505/tests/file_io/test_lib.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/file_io/tsk_file_io.py` & `dfvfs-20240505/tests/file_io/tsk_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/file_io/tsk_partition_file_io.py` & `dfvfs-20240505/tests/file_io/tsk_partition_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/file_io/vhdi_file_io.py` & `dfvfs-20240505/tests/file_io/vhdi_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/file_io/vmdk_file_io.py` & `dfvfs-20240505/tests/file_io/vmdk_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/file_io/vshadow_file_io.py` & `dfvfs-20240505/tests/file_io/vshadow_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/file_io/xfs_file_io.py` & `dfvfs-20240505/tests/file_io/xfs_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/file_io/zip_file_io.py` & `dfvfs-20240505/tests/file_io/zip_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/helpers/command_line.py` & `dfvfs-20240505/tests/helpers/command_line.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/helpers/data_slice.py` & `dfvfs-20240505/tests/helpers/data_slice.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/helpers/fake_file_system_builder.py` & `dfvfs-20240505/tests/helpers/fake_file_system_builder.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/helpers/file_system_searcher.py` & `dfvfs-20240505/tests/helpers/file_system_searcher.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/helpers/source_scanner.py` & `dfvfs-20240505/tests/helpers/source_scanner.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/helpers/text_file.py` & `dfvfs-20240505/tests/helpers/text_file.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/helpers/volume_scanner.py` & `dfvfs-20240505/tests/helpers/volume_scanner.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/helpers/windows_path_resolver.py` & `dfvfs-20240505/tests/helpers/windows_path_resolver.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/lib/apfs_helper.py` & `dfvfs-20240505/tests/lib/apfs_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/lib/cpio.py` & `dfvfs-20240505/tests/lib/cpio.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/lib/cs_helper.py` & `dfvfs-20240505/tests/lib/cs_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/lib/ewf_helper.py` & `dfvfs-20240505/tests/lib/ewf_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/lib/glob2regex.py` & `dfvfs-20240505/tests/lib/glob2regex.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/lib/gzipfile.py` & `dfvfs-20240505/tests/lib/gzipfile.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/lib/lvm_helper.py` & `dfvfs-20240505/tests/lib/lvm_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/lib/raw_helper.py` & `dfvfs-20240505/tests/lib/raw_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/mount/manager.py` & `dfvfs-20240505/tests/mount/manager.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/path/apfs_container_path_spec.py` & `dfvfs-20240505/tests/path/apfs_container_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/path/apfs_path_spec.py` & `dfvfs-20240505/tests/path/apfs_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/path/apm_path_spec.py` & `dfvfs-20240505/tests/path/apm_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/path/bde_path_spec.py` & `dfvfs-20240505/tests/path/bde_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/path/compressed_stream_path_spec.py` & `dfvfs-20240505/tests/path/compressed_stream_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/path/cpio_path_spec.py` & `dfvfs-20240505/tests/path/cpio_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/path/cs_path_spec.py` & `dfvfs-20240505/tests/path/cs_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/path/data_range_path_spec.py` & `dfvfs-20240505/tests/path/data_range_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/path/encoded_stream_path_spec.py` & `dfvfs-20240505/tests/path/encoded_stream_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/path/encryption_stream_path_spec.py` & `dfvfs-20240505/tests/path/encryption_stream_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/path/ewf_path_spec.py` & `dfvfs-20240505/tests/path/ewf_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/path/ext_path_spec.py` & `dfvfs-20240505/tests/path/ext_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/path/factory.py` & `dfvfs-20240505/tests/path/factory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/path/fake_path_spec.py` & `dfvfs-20240505/tests/path/fake_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/path/fat_path_spec.py` & `dfvfs-20240505/tests/path/fat_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/path/gpt_path_spec.py` & `dfvfs-20240505/tests/path/gpt_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/path/gzip_path_spec.py` & `dfvfs-20240505/tests/path/gzip_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/path/hfs_path_spec.py` & `dfvfs-20240505/tests/path/hfs_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/path/luksde_path_spec.py` & `dfvfs-20240505/tests/path/luksde_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/path/lvm_path_spec.py` & `dfvfs-20240505/tests/path/lvm_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/path/modi_path_spec.py` & `dfvfs-20240505/tests/path/modi_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/path/mount_path_spec.py` & `dfvfs-20240505/tests/path/mount_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/path/ntfs_path_spec.py` & `dfvfs-20240505/tests/path/ntfs_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/path/os_path_spec.py` & `dfvfs-20240505/tests/path/os_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/path/path_spec.py` & `dfvfs-20240505/tests/path/path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/path/phdi_path_spec.py` & `dfvfs-20240505/tests/path/phdi_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/path/qcow_path_spec.py` & `dfvfs-20240505/tests/path/qcow_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/path/raw_path_spec.py` & `dfvfs-20240505/tests/path/raw_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/path/sqlite_blob_path_spec.py` & `dfvfs-20240505/tests/path/sqlite_blob_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/path/tar_path_spec.py` & `dfvfs-20240505/tests/path/tar_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/path/test_lib.py` & `dfvfs-20240505/tests/path/test_lib.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/path/tsk_partition_path_spec.py` & `dfvfs-20240505/tests/path/tsk_partition_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/path/tsk_path_spec.py` & `dfvfs-20240505/tests/path/tsk_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/path/vhdi_path_spec.py` & `dfvfs-20240505/tests/path/vhdi_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/path/vmdk_path_spec.py` & `dfvfs-20240505/tests/path/vmdk_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/path/vshadow_path_spec.py` & `dfvfs-20240505/tests/path/vshadow_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/path/xfs_path_spec.py` & `dfvfs-20240505/tests/path/xfs_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/path/zip_path_spec.py` & `dfvfs-20240505/tests/path/zip_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/resolver/context.py` & `dfvfs-20240505/tests/resolver/context.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/resolver_helpers/apfs_resolver_helper.py` & `dfvfs-20240505/tests/resolver_helpers/apfs_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/resolver_helpers/apm_resolver_helper.py` & `dfvfs-20240505/tests/resolver_helpers/apm_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/resolver_helpers/bde_resolver_helper.py` & `dfvfs-20240505/tests/resolver_helpers/bde_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/resolver_helpers/compressed_stream_resolver_helper.py` & `dfvfs-20240505/tests/resolver_helpers/compressed_stream_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/resolver_helpers/cpio_resolver_helper.py` & `dfvfs-20240505/tests/resolver_helpers/cpio_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/resolver_helpers/cs_resolver_helper.py` & `dfvfs-20240505/tests/resolver_helpers/cs_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/resolver_helpers/encoded_stream_resolver_helper.py` & `dfvfs-20240505/tests/resolver_helpers/encoded_stream_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/resolver_helpers/encrypted_stream_resolver_helper.py` & `dfvfs-20240505/tests/resolver_helpers/encrypted_stream_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/resolver_helpers/ewf_resolver_helper.py` & `dfvfs-20240505/tests/resolver_helpers/ewf_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/resolver_helpers/ext_resolver_helper.py` & `dfvfs-20240505/tests/resolver_helpers/ext_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/resolver_helpers/fat_resolver_helper.py` & `dfvfs-20240505/tests/resolver_helpers/fat_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/resolver_helpers/gpt_resolver_helper.py` & `dfvfs-20240505/tests/resolver_helpers/gpt_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/resolver_helpers/gzip_resolver_helper.py` & `dfvfs-20240505/tests/resolver_helpers/gzip_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/resolver_helpers/hfs_resolver_helper.py` & `dfvfs-20240505/tests/resolver_helpers/hfs_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/resolver_helpers/luksde_resolver_helper.py` & `dfvfs-20240505/tests/resolver_helpers/luksde_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/resolver_helpers/lvm_resolver_helper.py` & `dfvfs-20240505/tests/resolver_helpers/lvm_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/resolver_helpers/manager.py` & `dfvfs-20240505/tests/resolver_helpers/manager.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/resolver_helpers/modi_resolver_helper.py` & `dfvfs-20240505/tests/resolver_helpers/modi_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/resolver_helpers/ntfs_resolver_helper.py` & `dfvfs-20240505/tests/resolver_helpers/ntfs_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/resolver_helpers/os_resolver_helper.py` & `dfvfs-20240505/tests/resolver_helpers/os_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/resolver_helpers/phdi_resolver_helper.py` & `dfvfs-20240505/tests/resolver_helpers/phdi_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/resolver_helpers/qcow_resolver_helper.py` & `dfvfs-20240505/tests/resolver_helpers/qcow_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/resolver_helpers/raw_resolver_helper.py` & `dfvfs-20240505/tests/resolver_helpers/raw_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/resolver_helpers/sqlite_blob_resolver_helper.py` & `dfvfs-20240505/tests/resolver_helpers/sqlite_blob_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/resolver_helpers/tar_resolver_helper.py` & `dfvfs-20240505/tests/resolver_helpers/tar_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/resolver_helpers/test_lib.py` & `dfvfs-20240505/tests/resolver_helpers/test_lib.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/resolver_helpers/tsk_partition_resolver_helper.py` & `dfvfs-20240505/tests/resolver_helpers/tsk_partition_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/resolver_helpers/tsk_resolver_helper.py` & `dfvfs-20240505/tests/resolver_helpers/tsk_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/resolver_helpers/vhdi_resolver_helper.py` & `dfvfs-20240505/tests/resolver_helpers/vhdi_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/resolver_helpers/vmdk_resolver_helper.py` & `dfvfs-20240505/tests/resolver_helpers/vmdk_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/resolver_helpers/vshadow_resolver_helper.py` & `dfvfs-20240505/tests/resolver_helpers/vshadow_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/resolver_helpers/xfs_resolver_helper.py` & `dfvfs-20240505/tests/resolver_helpers/xfs_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/resolver_helpers/zip_resolver_helper.py` & `dfvfs-20240505/tests/resolver_helpers/zip_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/serializer/json_serializer.py` & `dfvfs-20240505/tests/serializer/json_serializer.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/test_lib.py` & `dfvfs-20240505/tests/test_lib.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/vfs/apfs_attribute.py` & `dfvfs-20240505/tests/vfs/apfs_attribute.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/vfs/apfs_container_directory.py` & `dfvfs-20240505/tests/vfs/apfs_container_directory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/vfs/apfs_container_file_entry.py` & `dfvfs-20240505/tests/vfs/apfs_container_file_entry.py`

 * *Files 0% similar despite different names*

```diff
@@ -174,15 +174,15 @@
     file_entry = self._file_system.GetFileEntryByPathSpec(path_spec)
     self.assertIsNotNone(file_entry)
 
     parent_file_entry = file_entry.GetParentFileEntry()
     self.assertIsNone(parent_file_entry)
 
   def testIsFunctions(self):
-    """Test the Is? functions."""
+    """Test the Is* functions."""
     path_spec = path_spec_factory.Factory.NewPathSpec(
         definitions.TYPE_INDICATOR_APFS_CONTAINER, parent=self._raw_path_spec,
         volume_index=0)
     file_entry = self._file_system.GetFileEntryByPathSpec(path_spec)
     self.assertIsNotNone(file_entry)
 
     self.assertFalse(file_entry.IsRoot())
@@ -390,15 +390,15 @@
     file_entry = self._file_system.GetFileEntryByPathSpec(path_spec)
     self.assertIsNotNone(file_entry)
 
     parent_file_entry = file_entry.GetParentFileEntry()
     self.assertIsNone(parent_file_entry)
 
   def testIsFunctions(self):
-    """Test the Is? functions."""
+    """Test the Is* functions."""
     path_spec = path_spec_factory.Factory.NewPathSpec(
         definitions.TYPE_INDICATOR_APFS_CONTAINER, parent=self._gpt_path_spec,
         volume_index=0)
     file_entry = self._file_system.GetFileEntryByPathSpec(path_spec)
     self.assertIsNotNone(file_entry)
 
     self.assertFalse(file_entry.IsRoot())
```

### Comparing `dfvfs-20240115/tests/vfs/apfs_container_file_system.py` & `dfvfs-20240505/tests/vfs/apfs_container_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/vfs/apfs_directory.py` & `dfvfs-20240505/tests/vfs/apfs_directory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/vfs/apfs_file_entry.py` & `dfvfs-20240505/tests/vfs/apfs_file_entry.py`

 * *Files 0% similar despite different names*

```diff
@@ -268,15 +268,15 @@
     parent_file_entry = file_entry.GetParentFileEntry()
 
     self.assertIsNotNone(parent_file_entry)
 
     self.assertEqual(parent_file_entry.name, 'a_directory')
 
   def testIsFunctions(self):
-    """Tests the Is? functions."""
+    """Tests the Is* functions."""
     path_spec = path_spec_factory.Factory.NewPathSpec(
         definitions.TYPE_INDICATOR_APFS,
         identifier=self._IDENTIFIER_ANOTHER_FILE,
         location='/a_directory/another_file',
         parent=self._apfs_container_path_spec)
     file_entry = self._file_system.GetFileEntryByPathSpec(path_spec)
     self.assertIsNotNone(file_entry)
@@ -611,15 +611,15 @@
     parent_file_entry = file_entry.GetParentFileEntry()
 
     self.assertIsNotNone(parent_file_entry)
 
     self.assertEqual(parent_file_entry.name, 'a_directory')
 
   def testIsFunctions(self):
-    """Tests the Is? functions."""
+    """Tests the Is* functions."""
     path_spec = path_spec_factory.Factory.NewPathSpec(
         definitions.TYPE_INDICATOR_APFS,
         identifier=self._IDENTIFIER_ANOTHER_FILE,
         location='/a_directory/another_file',
         parent=self._apfs_container_path_spec)
     file_entry = self._file_system.GetFileEntryByPathSpec(path_spec)
     self.assertIsNotNone(file_entry)
```

### Comparing `dfvfs-20240115/tests/vfs/apfs_file_system.py` & `dfvfs-20240505/tests/vfs/apfs_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/vfs/apm_directory.py` & `dfvfs-20240505/tests/vfs/apm_directory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/vfs/apm_file_entry.py` & `dfvfs-20240505/tests/vfs/apm_file_entry.py`

 * *Files 0% similar despite different names*

```diff
@@ -112,15 +112,15 @@
     file_entry = self._file_system.GetFileEntryByPathSpec(path_spec)
     self.assertIsNotNone(file_entry)
 
     parent_file_entry = file_entry.GetParentFileEntry()
     self.assertIsNone(parent_file_entry)
 
   def testIsFunctions(self):
-    """Test the Is? functions."""
+    """Test the Is* functions."""
     path_spec = path_spec_factory.Factory.NewPathSpec(
         definitions.TYPE_INDICATOR_APM, entry_index=0,
         parent=self._raw_path_spec)
     file_entry = self._file_system.GetFileEntryByPathSpec(path_spec)
     self.assertIsNotNone(file_entry)
 
     self.assertFalse(file_entry.IsRoot())
```

### Comparing `dfvfs-20240115/tests/vfs/apm_file_system.py` & `dfvfs-20240505/tests/vfs/apm_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/vfs/attribute.py` & `dfvfs-20240505/tests/vfs/attribute.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/vfs/bde_file_entry.py` & `dfvfs-20240505/tests/vfs/bde_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/vfs/bde_file_system.py` & `dfvfs-20240505/tests/vfs/bde_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/vfs/compressed_stream_file_entry.py` & `dfvfs-20240505/tests/vfs/compressed_stream_file_entry.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,15 @@
         self._compressed_stream_path_spec)
     self.assertIsNotNone(file_entry)
 
     parent_file_entry = file_entry.GetParentFileEntry()
     self.assertIsNone(parent_file_entry)
 
   def testIsFunctions(self):
-    """Test the Is? functions."""
+    """Test the Is* functions."""
     file_entry = self._file_system.GetFileEntryByPathSpec(
         self._compressed_stream_path_spec)
     self.assertIsNotNone(file_entry)
 
     self.assertTrue(file_entry.IsRoot())
     self.assertTrue(file_entry.IsVirtual())
     self.assertTrue(file_entry.IsAllocated())
```

### Comparing `dfvfs-20240115/tests/vfs/compressed_stream_file_system.py` & `dfvfs-20240505/tests/vfs/compressed_stream_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/vfs/cpio_directory.py` & `dfvfs-20240505/tests/vfs/cpio_directory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/vfs/cpio_file_entry.py` & `dfvfs-20240505/tests/vfs/cpio_file_entry.py`

 * *Files 0% similar despite different names*

```diff
@@ -119,15 +119,15 @@
     self.assertIsNotNone(file_entry)
 
     parent_file_entry = file_entry.GetParentFileEntry()
     self.assertIsNotNone(parent_file_entry)
     self.assertEqual(parent_file_entry.name, '')
 
   def testIsFunctions(self):
-    """Test the Is? functions."""
+    """Test the Is* functions."""
     path_spec = path_spec_factory.Factory.NewPathSpec(
         definitions.TYPE_INDICATOR_CPIO, location='/syslog',
         parent=self._os_path_spec)
     file_entry = self._file_system.GetFileEntryByPathSpec(path_spec)
     self.assertIsNotNone(file_entry)
 
     self.assertFalse(file_entry.IsRoot())
```

### Comparing `dfvfs-20240115/tests/vfs/cpio_file_system.py` & `dfvfs-20240505/tests/vfs/cpio_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/vfs/cs_file_entry.py` & `dfvfs-20240505/tests/vfs/cs_file_entry.py`

 * *Files 1% similar despite different names*

```diff
@@ -183,15 +183,15 @@
     file_entry = self._file_system.GetFileEntryByPathSpec(path_spec)
     self.assertIsNotNone(file_entry)
 
     parent_file_entry = file_entry.GetParentFileEntry()
     self.assertIsNone(parent_file_entry)
 
   def testIsFunctions(self):
-    """Test the Is? functions."""
+    """Test the Is* functions."""
     path_spec = path_spec_factory.Factory.NewPathSpec(
         definitions.TYPE_INDICATOR_CS, parent=self._gpt_path_spec,
         volume_index=0)
     file_entry = self._file_system.GetFileEntryByPathSpec(path_spec)
     self.assertIsNotNone(file_entry)
 
     self.assertFalse(file_entry.IsRoot())
```

### Comparing `dfvfs-20240115/tests/vfs/cs_file_system.py` & `dfvfs-20240505/tests/vfs/cs_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/vfs/data_range_file_entry.py` & `dfvfs-20240505/tests/vfs/data_range_file_entry.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,15 @@
         self._data_range_path_spec)
     self.assertIsNotNone(file_entry)
 
     parent_file_entry = file_entry.GetParentFileEntry()
     self.assertIsNone(parent_file_entry)
 
   def testIsFunctions(self):
-    """Test the Is? functions."""
+    """Test the Is* functions."""
     file_entry = self._file_system.GetFileEntryByPathSpec(
         self._data_range_path_spec)
     self.assertIsNotNone(file_entry)
 
     self.assertTrue(file_entry.IsRoot())
     self.assertTrue(file_entry.IsVirtual())
     self.assertTrue(file_entry.IsAllocated())
```

### Comparing `dfvfs-20240115/tests/vfs/data_range_file_system.py` & `dfvfs-20240505/tests/vfs/data_range_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/vfs/data_stream.py` & `dfvfs-20240505/tests/vfs/data_stream.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/vfs/directory.py` & `dfvfs-20240505/tests/vfs/directory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/vfs/encoded_stream_file_entry.py` & `dfvfs-20240505/tests/vfs/encoded_stream_file_entry.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
         self._encoded_stream_path_spec)
     self.assertIsNotNone(file_entry)
 
     parent_file_entry = file_entry.GetParentFileEntry()
     self.assertIsNone(parent_file_entry)
 
   def testIsFunctions(self):
-    """Test the Is? functions."""
+    """Test the Is* functions."""
     file_entry = self._file_system.GetFileEntryByPathSpec(
         self._encoded_stream_path_spec)
     self.assertIsNotNone(file_entry)
 
     self.assertTrue(file_entry.IsRoot())
     self.assertTrue(file_entry.IsVirtual())
     self.assertTrue(file_entry.IsAllocated())
```

### Comparing `dfvfs-20240115/tests/vfs/encoded_stream_file_system.py` & `dfvfs-20240505/tests/vfs/encoded_stream_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/vfs/encrypted_stream_file_entry.py` & `dfvfs-20240505/tests/vfs/encrypted_stream_file_entry.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,15 @@
         self._encrypted_stream_path_spec)
     self.assertIsNotNone(file_entry)
 
     parent_file_entry = file_entry.GetParentFileEntry()
     self.assertIsNone(parent_file_entry)
 
   def testIsFunctions(self):
-    """Test the Is? functions."""
+    """Test the Is* functions."""
     file_entry = self._file_system.GetFileEntryByPathSpec(
         self._encrypted_stream_path_spec)
     self.assertIsNotNone(file_entry)
 
     self.assertTrue(file_entry.IsRoot())
     self.assertTrue(file_entry.IsVirtual())
     self.assertTrue(file_entry.IsAllocated())
```

### Comparing `dfvfs-20240115/tests/vfs/encrypted_stream_file_system.py` & `dfvfs-20240505/tests/vfs/encrypted_stream_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/vfs/ext_attribute.py` & `dfvfs-20240505/tests/vfs/ext_attribute.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/vfs/ext_directory.py` & `dfvfs-20240505/tests/vfs/ext_directory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/vfs/ext_file_entry.py` & `dfvfs-20240505/tests/vfs/ext_file_entry.py`

 * *Files 0% similar despite different names*

```diff
@@ -192,15 +192,15 @@
     parent_file_entry = file_entry.GetParentFileEntry()
 
     self.assertIsNotNone(parent_file_entry)
 
     self.assertEqual(parent_file_entry.name, 'a_directory')
 
   def testIsFunctions(self):
-    """Tests the Is? functions."""
+    """Tests the Is* functions."""
     path_spec = path_spec_factory.Factory.NewPathSpec(
         definitions.TYPE_INDICATOR_EXT, inode=self._INODE_ANOTHER_FILE,
         location='/a_directory/another_file', parent=self._raw_path_spec)
     file_entry = self._file_system.GetFileEntryByPathSpec(path_spec)
     self.assertIsNotNone(file_entry)
 
     self.assertFalse(file_entry.IsRoot())
@@ -470,15 +470,15 @@
     parent_file_entry = file_entry.GetParentFileEntry()
 
     self.assertIsNotNone(parent_file_entry)
 
     self.assertEqual(parent_file_entry.name, 'a_directory')
 
   def testIsFunctions(self):
-    """Tests the Is? functions."""
+    """Tests the Is* functions."""
     path_spec = path_spec_factory.Factory.NewPathSpec(
         definitions.TYPE_INDICATOR_EXT, inode=self._INODE_ANOTHER_FILE,
         location='/a_directory/another_file', parent=self._raw_path_spec)
     file_entry = self._file_system.GetFileEntryByPathSpec(path_spec)
     self.assertIsNotNone(file_entry)
 
     self.assertFalse(file_entry.IsRoot())
```

### Comparing `dfvfs-20240115/tests/vfs/ext_file_system.py` & `dfvfs-20240505/tests/vfs/ext_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/vfs/fake_directory.py` & `dfvfs-20240505/tests/vfs/fake_directory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/vfs/fake_file_entry.py` & `dfvfs-20240505/tests/vfs/fake_file_entry.py`

 * *Files 0% similar despite different names*

```diff
@@ -149,15 +149,15 @@
     parent_file_entry = file_entry.GetParentFileEntry()
 
     self.assertIsNotNone(parent_file_entry)
 
     self.assertEqual(parent_file_entry.name, 'testdir_fake')
 
   def testIsFunctions(self):
-    """Test the Is? functions."""
+    """Test the Is* functions."""
     test_file = '/test_data/testdir_fake/file1.txt'
     path_spec = fake_path_spec.FakePathSpec(location=test_file)
     file_entry = self._file_system.GetFileEntryByPathSpec(path_spec)
     self.assertIsNotNone(file_entry)
 
     self.assertFalse(file_entry.IsRoot())
     self.assertTrue(file_entry.IsVirtual())
```

### Comparing `dfvfs-20240115/tests/vfs/fake_file_system.py` & `dfvfs-20240505/tests/vfs/fake_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/vfs/fat_directory.py` & `dfvfs-20240505/tests/vfs/fat_directory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/vfs/fat_file_entry.py` & `dfvfs-20240505/tests/vfs/fat_file_entry.py`

 * *Files 0% similar despite different names*

```diff
@@ -285,15 +285,15 @@
     parent_file_entry = file_entry.GetParentFileEntry()
 
     self.assertIsNotNone(parent_file_entry)
 
     self.assertEqual(parent_file_entry.name, 'a_directory')
 
   def testIsFunctions(self):
-    """Tests the Is? functions."""
+    """Tests the Is* functions."""
     path_spec = path_spec_factory.Factory.NewPathSpec(
         definitions.TYPE_INDICATOR_FAT,
         identifier=self._IDENTIFIER_ANOTHER_FILE,
         location='\\a_directory\\another_file',
         parent=self._raw_path_spec)
     file_entry = self._file_system.GetFileEntryByPathSpec(path_spec)
     self.assertIsNotNone(file_entry)
```

### Comparing `dfvfs-20240115/tests/vfs/fat_file_system.py` & `dfvfs-20240505/tests/vfs/fat_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/vfs/file_entry.py` & `dfvfs-20240505/tests/vfs/file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/vfs/file_system.py` & `dfvfs-20240505/tests/vfs/file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/vfs/gpt_directory.py` & `dfvfs-20240505/tests/vfs/gpt_directory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/vfs/gpt_file_entry.py` & `dfvfs-20240505/tests/vfs/gpt_file_entry.py`

 * *Files 0% similar despite different names*

```diff
@@ -109,15 +109,15 @@
     file_entry = self._file_system.GetFileEntryByPathSpec(path_spec)
     self.assertIsNotNone(file_entry)
 
     parent_file_entry = file_entry.GetParentFileEntry()
     self.assertIsNone(parent_file_entry)
 
   def testIsFunctions(self):
-    """Test the Is? functions."""
+    """Test the Is* functions."""
     path_spec = path_spec_factory.Factory.NewPathSpec(
         definitions.TYPE_INDICATOR_GPT, entry_index=0,
         parent=self._raw_path_spec)
     file_entry = self._file_system.GetFileEntryByPathSpec(path_spec)
     self.assertIsNotNone(file_entry)
 
     self.assertFalse(file_entry.IsRoot())
```

### Comparing `dfvfs-20240115/tests/vfs/gpt_file_system.py` & `dfvfs-20240505/tests/vfs/gpt_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/vfs/gzip_file_entry.py` & `dfvfs-20240505/tests/vfs/gzip_file_entry.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,15 @@
     self.assertIsNotNone(file_entry)
 
     parent_file_entry = file_entry.GetParentFileEntry()
 
     self.assertIsNone(parent_file_entry)
 
   def testIsFunctions(self):
-    """Test the Is? functions."""
+    """Test the Is* functions."""
     file_entry = self._file_system.GetFileEntryByPathSpec(self._gzip_path_spec)
     self.assertIsNotNone(file_entry)
 
     self.assertTrue(file_entry.IsRoot())
     self.assertTrue(file_entry.IsVirtual())
     self.assertTrue(file_entry.IsAllocated())
```

### Comparing `dfvfs-20240115/tests/vfs/gzip_file_system.py` & `dfvfs-20240505/tests/vfs/gzip_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/vfs/hfs_attribute.py` & `dfvfs-20240505/tests/vfs/hfs_attribute.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/vfs/hfs_data_stream.py` & `dfvfs-20240505/tests/vfs/hfs_data_stream.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/vfs/hfs_directory.py` & `dfvfs-20240505/tests/vfs/hfs_directory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/vfs/hfs_file_entry.py` & `dfvfs-20240505/tests/vfs/hfs_file_entry.py`

 * *Files 0% similar despite different names*

```diff
@@ -394,15 +394,15 @@
     parent_file_entry = file_entry.GetParentFileEntry()
 
     self.assertIsNotNone(parent_file_entry)
 
     self.assertEqual(parent_file_entry.name, 'a_directory')
 
   def testIsFunctions(self):
-    """Tests the Is? functions."""
+    """Tests the Is* functions."""
     path_spec = path_spec_factory.Factory.NewPathSpec(
         definitions.TYPE_INDICATOR_HFS,
         identifier=self._IDENTIFIER_ANOTHER_FILE,
         location='/a_directory/another_file',
         parent=self._raw_path_spec)
     file_entry = self._file_system.GetFileEntryByPathSpec(path_spec)
     self.assertIsNotNone(file_entry)
```

### Comparing `dfvfs-20240115/tests/vfs/hfs_file_system.py` & `dfvfs-20240505/tests/vfs/hfs_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/vfs/luksde_file_entry.py` & `dfvfs-20240505/tests/vfs/luksde_file_entry.py`

 * *Files 0% similar despite different names*

```diff
@@ -113,15 +113,15 @@
         self._luksde_path_spec)
     self.assertIsNotNone(file_entry)
 
     parent_file_entry = file_entry.GetParentFileEntry()
     self.assertIsNone(parent_file_entry)
 
   def testIsFunctions(self):
-    """Test the Is? functions."""
+    """Test the Is* functions."""
     file_entry = self._file_system.GetFileEntryByPathSpec(
         self._luksde_path_spec)
     self.assertIsNotNone(file_entry)
 
     self.assertTrue(file_entry.IsRoot())
     self.assertTrue(file_entry.IsVirtual())
     self.assertTrue(file_entry.IsAllocated())
```

### Comparing `dfvfs-20240115/tests/vfs/luksde_file_system.py` & `dfvfs-20240505/tests/vfs/luksde_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/vfs/lvm_directory.py` & `dfvfs-20240505/tests/vfs/lvm_directory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/vfs/lvm_file_entry.py` & `dfvfs-20240505/tests/vfs/lvm_file_entry.py`

 * *Files 0% similar despite different names*

```diff
@@ -185,15 +185,15 @@
     file_entry = self._file_system.GetFileEntryByPathSpec(path_spec)
     self.assertIsNotNone(file_entry)
 
     parent_file_entry = file_entry.GetParentFileEntry()
     self.assertIsNone(parent_file_entry)
 
   def testIsFunctions(self):
-    """Test the Is? functions."""
+    """Test the Is* functions."""
     path_spec = path_spec_factory.Factory.NewPathSpec(
         definitions.TYPE_INDICATOR_LVM, parent=self._raw_path_spec,
         volume_index=0)
     file_entry = self._file_system.GetFileEntryByPathSpec(path_spec)
     self.assertIsNotNone(file_entry)
 
     self.assertFalse(file_entry.IsRoot())
```

### Comparing `dfvfs-20240115/tests/vfs/lvm_file_system.py` & `dfvfs-20240505/tests/vfs/lvm_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/vfs/ntfs_attibute.py` & `dfvfs-20240505/tests/vfs/ntfs_attibute.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/vfs/ntfs_data_stream.py` & `dfvfs-20240505/tests/vfs/ntfs_data_stream.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/vfs/ntfs_directory.py` & `dfvfs-20240505/tests/vfs/ntfs_directory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/vfs/ntfs_file_entry.py` & `dfvfs-20240505/tests/vfs/ntfs_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/vfs/ntfs_file_system.py` & `dfvfs-20240505/tests/vfs/ntfs_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/vfs/os_directory.py` & `dfvfs-20240505/tests/vfs/os_directory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/vfs/os_file_entry.py` & `dfvfs-20240505/tests/vfs/os_file_entry.py`

 * *Files 1% similar despite different names*

```diff
@@ -162,15 +162,15 @@
     parent_file_entry = file_entry.GetParentFileEntry()
 
     self.assertIsNotNone(parent_file_entry)
 
     self.assertEqual(parent_file_entry.name, 'testdir_os')
 
   def testIsFunctions(self):
-    """Test the Is? functions."""
+    """Test the Is* functions."""
     test_path = self._GetTestFilePath(['testdir_os', 'file1.txt'])
     self._SkipIfPathNotExists(test_path)
 
     path_spec = path_spec_factory.Factory.NewPathSpec(
         definitions.TYPE_INDICATOR_OS, location=test_path)
     file_entry = self._file_system.GetFileEntryByPathSpec(path_spec)
     self.assertIsNotNone(file_entry)
```

### Comparing `dfvfs-20240115/tests/vfs/os_file_system.py` & `dfvfs-20240505/tests/vfs/os_file_system.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from dfvfs.resolver import context
 from dfvfs.vfs import os_file_system
 
 from tests import test_lib as shared_test_lib
 
 
 def TestPlatformSystem():
-  """Test function to emulate platform.system() == 'Windows'"""
+  """Test function to emulate platform.system() == 'Windows'."""
   return 'Windows'
 
 
 class OSFileSystemTest(shared_test_lib.BaseTestCase):
   """Tests the operating system file system."""
 
   def setUp(self):
```

### Comparing `dfvfs-20240115/tests/vfs/sqlite_blob_directory.py` & `dfvfs-20240505/tests/vfs/sqlite_blob_directory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/vfs/sqlite_blob_file_entry.py` & `dfvfs-20240505/tests/vfs/sqlite_blob_file_entry.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,15 +111,15 @@
     parent_file_entry = file_entry.GetParentFileEntry()
 
     self.assertIsNotNone(parent_file_entry)
 
     self.assertEqual(parent_file_entry.name, 'myblobs.blobs')
 
   def testIsFunctions(self):
-    """Test the Is? functions."""
+    """Test the Is* functions."""
     file_entry = self._file_system.GetFileEntryByPathSpec(
         self._sqlite_blob_path_spec)
 
     self.assertFalse(file_entry.IsRoot())
     self.assertFalse(file_entry.IsVirtual())
     self.assertTrue(file_entry.IsAllocated())
```

### Comparing `dfvfs-20240115/tests/vfs/sqlite_blob_file_system.py` & `dfvfs-20240505/tests/vfs/sqlite_blob_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/vfs/tar_directory.py` & `dfvfs-20240505/tests/vfs/tar_directory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/vfs/tar_file_entry.py` & `dfvfs-20240505/tests/vfs/tar_file_entry.py`

 * *Files 0% similar despite different names*

```diff
@@ -102,15 +102,15 @@
     parent_file_entry = file_entry.GetParentFileEntry()
     self.assertIsNotNone(parent_file_entry)
     self.assertEqual(parent_file_entry.name, '')
 
   # TODO: add tests for GetTARInfo
 
   def testIsFunctions(self):
-    """Test the Is? functions."""
+    """Test the Is* functions."""
     path_spec = path_spec_factory.Factory.NewPathSpec(
         definitions.TYPE_INDICATOR_TAR, location='/syslog',
         parent=self._os_path_spec)
     file_entry = self._file_system.GetFileEntryByPathSpec(path_spec)
     self.assertIsNotNone(file_entry)
 
     self.assertFalse(file_entry.IsRoot())
```

### Comparing `dfvfs-20240115/tests/vfs/tar_file_system.py` & `dfvfs-20240505/tests/vfs/tar_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/vfs/tsk_attribute.py` & `dfvfs-20240505/tests/vfs/tsk_attribute.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/vfs/tsk_data_stream.py` & `dfvfs-20240505/tests/vfs/tsk_data_stream.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/vfs/tsk_directory.py` & `dfvfs-20240505/tests/vfs/tsk_directory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/vfs/tsk_file_entry.py` & `dfvfs-20240505/tests/vfs/tsk_file_entry.py`

 * *Files 0% similar despite different names*

```diff
@@ -396,15 +396,15 @@
     self.assertIsNotNone(parent_file_entry)
 
     self.assertEqual(parent_file_entry.name, 'a_directory')
 
   # TODO: add tests for GetTSKFile
 
   def testIsFunctions(self):
-    """Tests the Is? functions."""
+    """Tests the Is* functions."""
     path_spec = path_spec_factory.Factory.NewPathSpec(
         definitions.TYPE_INDICATOR_TSK, inode=self._INODE_ANOTHER_FILE,
         location='/a_directory/another_file', parent=self._raw_path_spec)
     file_entry = self._file_system.GetFileEntryByPathSpec(path_spec)
     self.assertIsNotNone(file_entry)
 
     self.assertFalse(file_entry.IsRoot())
@@ -750,15 +750,15 @@
     self.assertIsNotNone(parent_file_entry)
 
     self.assertEqual(parent_file_entry.name, 'a_directory')
 
   # TODO: add tests for GetTSKFile
 
   def testIsFunctions(self):
-    """Tests the Is? functions."""
+    """Tests the Is* functions."""
     path_spec = path_spec_factory.Factory.NewPathSpec(
         definitions.TYPE_INDICATOR_TSK, inode=self._INODE_ANOTHER_FILE,
         location='/a_directory/another_file', parent=self._raw_path_spec)
     file_entry = self._file_system.GetFileEntryByPathSpec(path_spec)
     self.assertIsNotNone(file_entry)
 
     self.assertFalse(file_entry.IsRoot())
@@ -1168,15 +1168,15 @@
     self.assertIsNotNone(parent_file_entry)
 
     self.assertEqual(parent_file_entry.name, 'a_directory')
 
   # TODO: add tests for GetTSKFile
 
   def testIsFunctions(self):
-    """Tests the Is? functions."""
+    """Tests the Is* functions."""
     path_spec = path_spec_factory.Factory.NewPathSpec(
         definitions.TYPE_INDICATOR_TSK, inode=self._INODE_ANOTHER_FILE,
         location='/a_directory/another_file', parent=self._raw_path_spec)
     file_entry = self._file_system.GetFileEntryByPathSpec(path_spec)
     self.assertIsNotNone(file_entry)
 
     self.assertFalse(file_entry.IsRoot())
@@ -1579,15 +1579,15 @@
     self.assertIsNotNone(parent_file_entry)
 
     self.assertEqual(parent_file_entry.name, 'A_DIRECTORY')
 
   # TODO: add tests for GetTSKFile
 
   def testIsFunctions(self):
-    """Tests the Is? functions."""
+    """Tests the Is* functions."""
     path_spec = path_spec_factory.Factory.NewPathSpec(
         definitions.TYPE_INDICATOR_TSK, inode=self._INODE_ANOTHER_FILE,
         location='/A_DIRECTORY/ANOTHER_FILE', parent=self.test_os_path_spec)
     file_entry = self._file_system.GetFileEntryByPathSpec(path_spec)
     self.assertIsNotNone(file_entry)
 
     self.assertFalse(file_entry.IsRoot())
@@ -2291,15 +2291,15 @@
     self.assertIsNotNone(parent_file_entry)
 
     self.assertEqual(parent_file_entry.name, 'a_directory')
 
   # TODO: add tests for GetTSKFile
 
   def testIsFunctions(self):
-    """Tests the Is? functions."""
+    """Tests the Is* functions."""
     path_spec = path_spec_factory.Factory.NewPathSpec(
         definitions.TYPE_INDICATOR_TSK, inode=self._INODE_ANOTHER_FILE,
         location='/a_directory/another_file',
         parent=self._tsk_partition_path_spec)
     file_entry = self._file_system.GetFileEntryByPathSpec(path_spec)
     self.assertIsNotNone(file_entry)
```

### Comparing `dfvfs-20240115/tests/vfs/tsk_file_system.py` & `dfvfs-20240505/tests/vfs/tsk_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/vfs/tsk_partition_directory.py` & `dfvfs-20240505/tests/vfs/tsk_partition_directory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/vfs/tsk_partition_file_entry.py` & `dfvfs-20240505/tests/vfs/tsk_partition_file_entry.py`

 * *Files 0% similar despite different names*

```diff
@@ -98,15 +98,15 @@
     file_entry = self._file_system.GetFileEntryByPathSpec(path_spec)
 
     self.assertIsNotNone(file_entry)
     tsk_vs_part = file_entry.GetTSKVsPart()
     self.assertIsNotNone(tsk_vs_part)
 
   def testIsFunctions(self):
-    """Test the Is? functions."""
+    """Test the Is* functions."""
     path_spec = path_spec_factory.Factory.NewPathSpec(
         definitions.TYPE_INDICATOR_TSK_PARTITION, part_index=0,
         parent=self._os_path_spec)
     file_entry = self._file_system.GetFileEntryByPathSpec(path_spec)
     self.assertIsNotNone(file_entry)
 
     self.assertFalse(file_entry.IsRoot())
@@ -288,15 +288,15 @@
     file_entry = self._file_system.GetFileEntryByPathSpec(path_spec)
 
     self.assertIsNotNone(file_entry)
     tsk_vs_part = file_entry.GetTSKVsPart()
     self.assertIsNotNone(tsk_vs_part)
 
   def testIsFunctions(self):
-    """Test the Is? functions."""
+    """Test the Is* functions."""
     path_spec = path_spec_factory.Factory.NewPathSpec(
         definitions.TYPE_INDICATOR_TSK_PARTITION, part_index=2,
         parent=self._os_path_spec)
     file_entry = self._file_system.GetFileEntryByPathSpec(path_spec)
     self.assertIsNotNone(file_entry)
 
     self.assertFalse(file_entry.IsRoot())
@@ -483,15 +483,15 @@
     file_entry = self._file_system.GetFileEntryByPathSpec(path_spec)
 
     self.assertIsNotNone(file_entry)
     tsk_vs_part = file_entry.GetTSKVsPart()
     self.assertIsNotNone(tsk_vs_part)
 
   def testIsFunctions(self):
-    """Test the Is? functions."""
+    """Test the Is* functions."""
     path_spec = path_spec_factory.Factory.NewPathSpec(
         definitions.TYPE_INDICATOR_TSK_PARTITION, part_index=1,
         parent=self._os_path_spec)
     file_entry = self._file_system.GetFileEntryByPathSpec(path_spec)
     self.assertIsNotNone(file_entry)
 
     self.assertFalse(file_entry.IsRoot())
```

### Comparing `dfvfs-20240115/tests/vfs/tsk_partition_file_system.py` & `dfvfs-20240505/tests/vfs/tsk_partition_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/vfs/vshadow_directory.py` & `dfvfs-20240505/tests/vfs/vshadow_directory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/vfs/vshadow_file_entry.py` & `dfvfs-20240505/tests/vfs/vshadow_file_entry.py`

 * *Files 0% similar despite different names*

```diff
@@ -121,15 +121,15 @@
     parent_file_entry = file_entry.GetParentFileEntry()
     self.assertIsNone(parent_file_entry)
 
   # TODO: add tests for GetVShadowStore
   # TODO: add tests for HasExternalData
 
   def testIsFunctions(self):
-    """Test the Is? functions."""
+    """Test the Is* functions."""
     path_spec = path_spec_factory.Factory.NewPathSpec(
         definitions.TYPE_INDICATOR_VSHADOW, parent=self._raw_path_spec,
         store_index=1)
     file_entry = self._file_system.GetFileEntryByPathSpec(path_spec)
     self.assertIsNotNone(file_entry)
 
     self.assertFalse(file_entry.IsRoot())
```

### Comparing `dfvfs-20240115/tests/vfs/vshadow_file_system.py` & `dfvfs-20240505/tests/vfs/vshadow_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/vfs/xfs_attribute.py` & `dfvfs-20240505/tests/vfs/xfs_attribute.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/vfs/xfs_directory.py` & `dfvfs-20240505/tests/vfs/xfs_directory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/vfs/xfs_file_entry.py` & `dfvfs-20240505/tests/vfs/xfs_file_entry.py`

 * *Files 0% similar despite different names*

```diff
@@ -202,15 +202,15 @@
     parent_file_entry = file_entry.GetParentFileEntry()
 
     self.assertIsNotNone(parent_file_entry)
 
     self.assertEqual(parent_file_entry.name, 'a_directory')
 
   def testIsFunctions(self):
-    """Tests the Is? functions."""
+    """Tests the Is* functions."""
     path_spec = path_spec_factory.Factory.NewPathSpec(
         definitions.TYPE_INDICATOR_XFS, inode=self._INODE_ANOTHER_FILE,
         location='/a_directory/another_file', parent=self._raw_path_spec)
     file_entry = self._file_system.GetFileEntryByPathSpec(path_spec)
     self.assertIsNotNone(file_entry)
 
     self.assertFalse(file_entry.IsRoot())
```

### Comparing `dfvfs-20240115/tests/vfs/xfs_file_system.py` & `dfvfs-20240505/tests/vfs/xfs_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/vfs/zip_directory.py` & `dfvfs-20240505/tests/vfs/zip_directory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/vfs/zip_file_entry.py` & `dfvfs-20240505/tests/vfs/zip_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/vfs/zip_file_system.py` & `dfvfs-20240505/tests/vfs/zip_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/volume/apfs_volume_system.py` & `dfvfs-20240505/tests/volume/apfs_volume_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/volume/apm_volume_system.py` & `dfvfs-20240505/tests/volume/apm_volume_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/volume/cs_volume_system.py` & `dfvfs-20240505/tests/volume/cs_volume_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/volume/factory.py` & `dfvfs-20240505/tests/volume/factory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/volume/gpt_volume_system.py` & `dfvfs-20240505/tests/volume/gpt_volume_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/volume/lvm_volume_system.py` & `dfvfs-20240505/tests/volume/lvm_volume_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/volume/tsk_volume_system.py` & `dfvfs-20240505/tests/volume/tsk_volume_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tests/volume/vshadow_volume_system.py` & `dfvfs-20240505/tests/volume/vshadow_volume_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/tox.ini` & `dfvfs-20240505/tox.ini`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [tox]
-envlist = py3{7,8,9,10,11,12},coverage,docs,lint,wheel
+envlist = py3{8,9,10,11,12},coverage,docformatter,docs,lint,wheel
 
 [testenv]
 allowlist_externals = ./run_tests.py
 pip_pre = True
 passenv =
   CFLAGS
   CPPFLAGS
@@ -15,20 +15,27 @@
   -rtest_requirements.txt
   coverage: coverage
   wheel:
     build
     setuptools >= 65
     wheel
 commands =
-  py3{7,8,9,10,11,12}: ./run_tests.py
+  py3{8,9,10,11,12}: ./run_tests.py
   coverage: coverage erase
   coverage: coverage run --source=dfvfs --omit="*_test*,*__init__*,*test_lib*" run_tests.py
   coverage: coverage xml
   wheel: python -m build --no-isolation --wheel
 
+[testenv:docformatter]
+usedevelop = True
+deps =
+  docformatter
+commands =
+  docformatter --in-place --recursive dfvfs tests
+
 [testenv:docs]
 usedevelop = True
 deps =
   -rdocs/requirements.txt
 commands =
   sphinx-build -b html -d build/doctrees docs dist/docs
   sphinx-build -b linkcheck docs dist/docs
@@ -41,14 +48,18 @@
   CPPFLAGS
   LDFLAGS
 setenv =
   PYTHONPATH = {toxinidir}
 deps =
   -rrequirements.txt
   -rtest_requirements.txt
+  docformatter
   pylint >= 3.0.0, < 3.1.0
+  setuptools
   yamllint >= 1.26.0
 commands =
+  docformatter --version
   pylint --version
   yamllint -v
+  docformatter --check --diff --recursive dfvfs setup.py tests
   pylint --rcfile=.pylintrc dfvfs setup.py tests
   yamllint -c .yamllint.yaml dfvfs
```

### Comparing `dfvfs-20240115/utils/dependencies.py` & `dfvfs-20240505/utils/dependencies.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/utils/generate_test_data_bsd.sh` & `dfvfs-20240505/utils/generate_test_data_bsd.sh`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/utils/generate_test_data_linux.sh` & `dfvfs-20240505/utils/generate_test_data_linux.sh`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/utils/generate_test_data_macos.sh` & `dfvfs-20240505/utils/generate_test_data_macos.sh`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/utils/generate_test_data_windows.bat` & `dfvfs-20240505/utils/generate_test_data_windows.bat`

 * *Files identical despite different names*

### Comparing `dfvfs-20240115/utils/update_release.sh` & `dfvfs-20240505/utils/update_release.sh`

 * *Files 18% similar despite different names*

```diff
@@ -25,11 +25,11 @@
 EOT
 
 # Regenerate the supported formats documentation.
 # TODO: generate supported formats.
 # PYTHONPATH=. ./utils/export_supported_formats.py > docs/sources/Supported-formats.md
 
 # Regenerate the API documentation.
-tox -edocs
+tox -edocformatter,docs
 
 exit ${EXIT_SUCCESS};
```

