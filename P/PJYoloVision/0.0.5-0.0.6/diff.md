# Comparing `tmp/PJYoloVision-0.0.5.tar.gz` & `tmp/PJYoloVision-0.0.6-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PJYoloVision-0.0.5.tar", last modified: Mon Jul  3 13:22:52 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

