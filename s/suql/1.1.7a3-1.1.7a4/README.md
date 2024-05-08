# Comparing `tmp/suql-1.1.7a3.tar.gz` & `tmp/suql-1.1.7a4-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "suql-1.1.7a3.tar", last modified: Tue May  7 05:23:46 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

