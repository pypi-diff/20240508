# Comparing `tmp/cengal_light-4.3.1.tar.gz` & `tmp/cengal_light-4.4.0-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cengal_light-4.3.1.tar", last modified: Mon Apr  1 10:50:33 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

