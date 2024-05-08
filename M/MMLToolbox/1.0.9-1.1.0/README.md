# Comparing `tmp/MMLToolbox-1.0.9.tar.gz` & `tmp/MMLToolbox-1.1.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MMLToolbox-1.0.9.tar", last modified: Sun Mar 24 14:11:08 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

