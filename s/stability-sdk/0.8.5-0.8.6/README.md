# Comparing `tmp/stability-sdk-0.8.5.tar.gz` & `tmp/stability_sdk-0.8.6-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stability-sdk-0.8.5.tar", last modified: Mon Nov 20 17:29:25 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

