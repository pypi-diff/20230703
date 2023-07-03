# Comparing `tmp/collective.faceted.datewidget-1.0.0.tar.gz` & `tmp/collective.faceted.datewidget-1.0a1.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/collective.faceted.datewidget-1.0.0.tar", last modified: Mon Jul  3 10:34:13 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

