# Comparing `tmp/Deepurify-2.3.2.tar.gz` & `tmp/Deepurify-2.3.3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Deepurify-2.3.2.tar", last modified: Sat Apr 27 13:27:53 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

