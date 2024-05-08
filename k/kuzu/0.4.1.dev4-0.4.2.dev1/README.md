# Comparing `tmp/kuzu-0.4.1.dev4.tar.gz` & `tmp/kuzu-0.4.2.dev1-cp38-cp38-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kuzu-0.4.1.dev4.tar", last modified: Tue May  7 08:04:31 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```
