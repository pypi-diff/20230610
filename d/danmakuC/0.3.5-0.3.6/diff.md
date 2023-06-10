# Comparing `tmp/danmakuC-0.3.5.tar.gz` & `tmp/danmakuC-0.3.6-cp38-cp38-win32.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "danmakuC-0.3.5.tar", last modified: Sun Apr 23 07:10:17 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

