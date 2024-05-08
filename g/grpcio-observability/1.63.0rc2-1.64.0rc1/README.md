# Comparing `tmp/grpcio_observability-1.63.0rc2.tar.gz` & `tmp/grpcio_observability-1.64.0rc1-cp310-cp310-manylinux_2_17_i686.manylinux2014_i686.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grpcio_observability-1.63.0rc2.tar", last modified: Wed Apr 17 22:28:24 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

