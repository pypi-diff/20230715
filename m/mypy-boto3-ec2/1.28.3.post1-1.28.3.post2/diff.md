# Comparing `tmp/mypy-boto3-ec2-1.28.3.post1.tar.gz` & `tmp/mypy_boto3_ec2-1.28.3.post2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-ec2-1.28.3.post1.tar", last modified: Fri Jul 14 16:17:59 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

