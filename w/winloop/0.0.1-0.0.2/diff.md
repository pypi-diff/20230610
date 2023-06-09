# Comparing `tmp/winloop-0.0.1.tar.gz` & `tmp/winloop-0.0.2-cp39-cp39-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "winloop-0.0.1.tar", last modified: Fri Jun  9 20:52:27 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

