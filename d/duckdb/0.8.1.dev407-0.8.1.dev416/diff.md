# Comparing `tmp/duckdb-0.8.1.dev407.tar.gz` & `tmp/duckdb-0.8.1.dev416-cp310-cp310-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/duckdb-0.8.1.dev407.tar", last modified: Fri Jun  9 03:08:10 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

