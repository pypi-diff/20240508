# Comparing `tmp/grpcio_csds-1.63.0rc2.tar.gz` & `tmp/grpcio_csds-1.64.0rc1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grpcio_csds-1.63.0rc2.tar", last modified: Wed Apr 17 21:53:55 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

