# Comparing `tmp/nwb4fp-0.6.1.7.tar.gz` & `tmp/nwb4fp-0.6.1.8-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nwb4fp-0.6.1.7.tar", last modified: Wed May  8 16:41:43 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

