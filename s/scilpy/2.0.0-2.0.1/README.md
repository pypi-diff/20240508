# Comparing `tmp/scilpy-2.0.0.tar.gz` & `tmp/scilpy-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scilpy-2.0.0.tar", last modified: Tue Apr 23 18:30:18 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

