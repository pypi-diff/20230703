# Comparing `tmp/kisters.water.time_series-2.3.5.tar.gz` & `tmp/kisters.water.time_series-2.3.6-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kisters.water.time_series-2.3.5.tar", last modified: Thu Dec 15 18:37:10 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

