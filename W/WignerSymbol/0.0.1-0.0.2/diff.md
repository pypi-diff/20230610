# Comparing `tmp/WignerSymbol-0.0.1.tar.gz` & `tmp/WignerSymbol-0.0.2-cp310-cp310-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "WignerSymbol-0.0.1.tar", last modified: Sat Jun 10 12:38:02 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

