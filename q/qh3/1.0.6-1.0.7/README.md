# Comparing `tmp/qh3-1.0.6.tar.gz` & `tmp/qh3-1.0.7-pp37-pypy37_pp73-macosx_10_12_x86_64.macosx_11_0_arm64.macosx_10_12_universal2.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

