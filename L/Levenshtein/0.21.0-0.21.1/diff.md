# Comparing `tmp/Levenshtein-0.21.0.tar.gz` & `tmp/Levenshtein-0.21.1-pp37-pypy37_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Levenshtein-0.21.0.tar", last modified: Wed Apr 19 21:44:29 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

