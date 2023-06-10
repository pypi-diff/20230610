# Comparing `tmp/AmberMDrun-0.0.3.tar.gz` & `tmp/AmberMDrun-0.0.4.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AmberMDrun-0.0.3.tar", last modified: Mon Mar 27 10:47:45 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

