# Comparing `tmp/fzf_bin-0.51.0.tar.gz` & `tmp/fzf_bin-0.52.0-py3-none-macosx_11_0_arm64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fzf_bin-0.51.0.tar", last modified: Wed May  1 07:20:12 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

