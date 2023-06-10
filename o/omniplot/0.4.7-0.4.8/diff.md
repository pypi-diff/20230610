# Comparing `tmp/omniplot-0.4.7.tar.gz` & `tmp/omniplot-0.4.8-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omniplot-0.4.7.tar", last modified: Mon May 22 02:44:37 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

