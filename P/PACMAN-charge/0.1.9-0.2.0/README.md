# Comparing `tmp/PACMAN-charge-0.1.9.tar.gz` & `tmp/PACMAN_charge-0.2.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PACMAN-charge-0.1.9.tar", last modified: Tue May  7 08:19:18 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

