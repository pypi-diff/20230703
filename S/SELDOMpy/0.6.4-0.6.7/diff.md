# Comparing `tmp/SELDOMpy-0.6.4.tar.gz` & `tmp/SELDOMpy-0.6.7-py3.8-win-amd64.egg`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\SELDOMpy-0.6.4.tar", last modified: Mon Jul  3 15:44:32 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

