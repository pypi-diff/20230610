# Comparing `tmp/miniosl-0.0.3a1.tar.gz` & `tmp/miniosl-0.0.4-cp310-cp310-manylinux_2_28_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "miniosl-0.0.3a1.tar", last modified: Sat Jun  3 06:34:50 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

