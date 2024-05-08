# Comparing `tmp/power_grid_model_io-1.2.83.tar.gz` & `tmp/power_grid_model_io-1.2.9-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "power_grid_model_io-1.2.83.tar", last modified: Wed May  8 13:42:12 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

