# Comparing `tmp/gitcoll-0.0.19.tar.gz` & `tmp/gitcoll-0.0.20-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitcoll-0.0.19.tar", last modified: Mon Jul  3 05:28:15 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

