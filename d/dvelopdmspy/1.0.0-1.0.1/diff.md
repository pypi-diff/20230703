# Comparing `tmp/dvelopdmspy-1.0.0.tar.gz` & `tmp/dvelopdmspy-1.0.1-py2.py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dvelopdmspy-1.0.0.tar", last modified: Mon Jul  3 11:58:09 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

