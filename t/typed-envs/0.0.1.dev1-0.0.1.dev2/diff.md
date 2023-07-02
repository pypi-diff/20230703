# Comparing `tmp/typed-envs-0.0.1.dev1.tar.gz` & `tmp/typed_envs-0.0.1.dev2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typed-envs-0.0.1.dev1.tar", last modified: Sun Jul  2 23:07:24 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

