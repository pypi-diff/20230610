# Comparing `tmp/xia_git_gitlab-0.0.6-cp39-none-win_amd64.whl.zip` & `tmp/xia_git_gitlab-0.0.7-cp39-none-macosx_11_0_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 166530 bytes, number of entries: 7
--rw-r--r--  2.0 unx       95 b- defN 23-Jun-08 20:02 xia_git_gitlab/__init__.py
--rw-r--r--  2.0 unx   430080 b- defN 23-Jun-08 20:06 xia_git_gitlab/git.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-08 20:06 xia_git_gitlab-0.0.6.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      700 b- defN 23-Jun-08 20:06 xia_git_gitlab-0.0.6.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-08 20:06 xia_git_gitlab-0.0.6.dist-info/WHEEL
--rw-r--r--  2.0 unx       15 b- defN 23-Jun-08 20:06 xia_git_gitlab-0.0.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      600 b- defN 23-Jun-08 20:06 xia_git_gitlab-0.0.6.dist-info/RECORD
-7 files, 431740 bytes uncompressed, 165454 bytes compressed:  61.7%
+Zip file size: 136945 bytes, number of entries: 7
+-rw-r--r--  2.0 unx       95 b- defN 23-Jun-10 15:35 xia_git_gitlab/__init__.py
+-rw-r--r--  2.0 unx   371528 b- defN 23-Jun-10 15:35 xia_git_gitlab/git.cpython-310-darwin.so
+-rw-r--r--  2.0 unx      151 b- defN 23-Jun-10 15:35 xia_git_gitlab-0.0.7.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      663 b- defN 23-Jun-10 15:35 xia_git_gitlab-0.0.7.dist-info/METADATA
+-rw-r--r--  2.0 unx      108 b- defN 23-Jun-10 15:35 xia_git_gitlab-0.0.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx       15 b- defN 23-Jun-10 15:35 xia_git_gitlab-0.0.7.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      604 b- defN 23-Jun-10 15:35 xia_git_gitlab-0.0.7.dist-info/RECORD
+7 files, 373164 bytes uncompressed, 135863 bytes compressed:  63.6%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_git_gitlab/__init__.py
 Comment: 
 
-Filename: xia_git_gitlab/git.cp39-win_amd64.pyd
+Filename: xia_git_gitlab/git.cpython-310-darwin.so
 Comment: 
 
-Filename: xia_git_gitlab-0.0.6.dist-info/LICENSE.txt
+Filename: xia_git_gitlab-0.0.7.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_git_gitlab-0.0.6.dist-info/METADATA
+Filename: xia_git_gitlab-0.0.7.dist-info/METADATA
 Comment: 
 
-Filename: xia_git_gitlab-0.0.6.dist-info/WHEEL
+Filename: xia_git_gitlab-0.0.7.dist-info/WHEEL
 Comment: 
 
-Filename: xia_git_gitlab-0.0.6.dist-info/top_level.txt
+Filename: xia_git_gitlab-0.0.7.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_git_gitlab-0.0.6.dist-info/RECORD
+Filename: xia_git_gitlab-0.0.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_git_gitlab/__init__.py

```diff
@@ -1,7 +1,7 @@
 from xia_git_gitlab.git import GitlabGit
 
 __all__ = [
     "GitlabGit"
 ]
 
-__version__ = "0.0.6"
+__version__ = "0.0.7"
```

## Comparing `xia_git_gitlab-0.0.6.dist-info/METADATA` & `xia_git_gitlab-0.0.7.dist-info/METADATA`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: xia-git-gitlab
-Version: 0.0.6
+Version: 0.0.7
 Summary: X-I-A
-Home-page: https://develop.x-i-a.com/docs/xia-git-gitlab/0.0.6/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-git-gitlab/0.0.7/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
-License: UNKNOWN
-Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 Requires-Dist: requests
 Requires-Dist: GitPython
 Requires-Dist: xia-git
 
@@ -28,9 +26,7 @@
 =============================
 
 Install the package::
 
     pip install
 
 
-
-
```

