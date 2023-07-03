# Comparing `tmp/pyamg-5.0.0a3.tar.gz` & `tmp/pyamg-5.0.1-cp311-cp311-win32.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyamg-5.0.0a3.tar", last modified: Mon Apr 17 18:05:15 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

