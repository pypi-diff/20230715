# Comparing `tmp/aws-sm-1.2.0.tar.gz` & `tmp/aws_sm-1.2.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws-sm-1.2.0.tar", last modified: Fri Jan  6 13:21:46 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

