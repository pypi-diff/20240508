# Comparing `tmp/anycrc-0.6.0.tar.gz` & `tmp/anycrc-0.6.1-cp312-cp312-macosx_11_0_arm64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anycrc-0.6.0.tar", last modified: Sat Apr 27 06:20:37 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

