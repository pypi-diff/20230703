# Comparing `tmp/sloancone-0.4.1.tar.gz` & `tmp/sloancone-0.4.2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sloancone-0.4.1.tar", last modified: Fri May 20 12:42:20 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

