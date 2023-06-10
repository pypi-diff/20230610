# Comparing `tmp/jag-panzer-0.1.2.tar.gz` & `tmp/jag-panzer-0.1.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jag-panzer-0.1.2.tar", last modified: Fri Jun  9 12:35:21 2023, max compression
+gzip compressed data, was "jag-panzer-0.1.21.tar", last modified: Sat Jun 10 02:03:13 2023, max compression
```

## Comparing `jag-panzer-0.1.2.tar` & `jag-panzer-0.1.21.tar`

### file list

```diff
@@ -1,103 +1,103 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 12:35:21.140987 jag-panzer-0.1.2/
--rw-rw-rw-   0        0        0      161 2023-06-09 00:40:57.000000 jag-panzer-0.1.2/LICENSE
--rw-rw-rw-   0        0        0       46 2023-06-09 02:05:06.000000 jag-panzer-0.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0      560 2023-06-09 12:35:21.140987 jag-panzer-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0       26 2023-06-09 00:32:58.000000 jag-panzer-0.1.2/README.md
--rw-rw-rw-   0        0        0      108 2023-06-09 00:12:29.000000 jag-panzer-0.1.2/pyproject.toml
--rw-rw-rw-   0        0        0      671 2023-06-09 12:35:21.146964 jag-panzer-0.1.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-09 12:35:20.963061 jag-panzer-0.1.2/src/
-drwxrwxrwx   0        0        0        0 2023-06-09 12:35:20.991047 jag-panzer-0.1.2/src/jag_panzer/
--rw-rw-rw-   0        0        0        0 2023-06-09 00:13:59.000000 jag-panzer-0.1.2/src/jag_panzer/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-09 12:35:21.017031 jag-panzer-0.1.2/src/jag_panzer/assets/
-drwxrwxrwx   0        0        0        0 2023-06-09 12:35:21.029026 jag-panzer-0.1.2/src/jag_panzer/assets/dir_listing/
--rw-rw-rw-   0        0        0      356 2023-06-08 21:39:34.000000 jag-panzer-0.1.2/src/jag_panzer/assets/dir_listing/base.html
--rw-rw-rw-   0        0        0      446 2023-06-06 00:39:53.000000 jag-panzer-0.1.2/src/jag_panzer/assets/dir_listing/dir_icon.svg
--rw-rw-rw-   0        0        0      682 2023-06-07 06:27:42.000000 jag-panzer-0.1.2/src/jag_panzer/assets/dir_listing/download_icon.svg
--rw-rw-rw-   0        0        0      704 2023-06-06 00:40:06.000000 jag-panzer-0.1.2/src/jag_panzer/assets/dir_listing/file_icon.svg
--rw-rw-rw-   0        0        0       21 2023-06-06 01:12:59.000000 jag-panzer-0.1.2/src/jag_panzer/assets/dir_listing/script.js
--rw-rw-rw-   0        0        0     1355 2023-06-07 07:34:01.000000 jag-panzer-0.1.2/src/jag_panzer/assets/dir_listing/style.css
--rw-rw-rw-   0        0        0      260 2023-06-07 02:18:15.000000 jag-panzer-0.1.2/src/jag_panzer/assets/reject.html
--rw-rw-rw-   0        0        0    18350 2023-06-09 12:04:50.000000 jag-panzer-0.1.2/src/jag_panzer/base_room.py
-drwxrwxrwx   0        0        0        0 2023-06-09 12:35:21.035030 jag-panzer-0.1.2/src/jag_panzer/cgi/
--rw-rw-rw-   0        0        0        0 2023-06-09 00:00:24.000000 jag-panzer-0.1.2/src/jag_panzer/cgi/__init__.py
--rw-rw-rw-   0        0        0     5087 2023-06-03 17:16:43.000000 jag-panzer-0.1.2/src/jag_panzer/cgi/burn_power.py
--rw-rw-rw-   0        0        0      451 2023-06-03 17:16:43.000000 jag-panzer-0.1.2/src/jag_panzer/cgi/hitman.py
--rw-rw-rw-   0        0        0     6691 2023-06-03 17:16:43.000000 jag-panzer-0.1.2/src/jag_panzer/cgi/jag.py
-drwxrwxrwx   0        0        0        0 2023-06-09 12:35:21.037041 jag-panzer-0.1.2/src/jag_panzer/cgi/templates/
-drwxrwxrwx   0        0        0        0 2023-06-09 12:35:21.039028 jag-panzer-0.1.2/src/jag_panzer/cgi/templates/light_httpd/
-drwxrwxrwx   0        0        0        0 2023-06-09 12:35:21.043023 jag-panzer-0.1.2/src/jag_panzer/cgi/templates/light_httpd/conf-enabled/
--rw-rw-rw-   0        0        0       91 2023-06-03 17:16:43.000000 jag-panzer-0.1.2/src/jag_panzer/cgi/templates/light_httpd/conf-enabled/10-accesslog.conf
--rw-rw-rw-   0        0        0      306 2023-06-03 17:16:43.000000 jag-panzer-0.1.2/src/jag_panzer/cgi/templates/light_httpd/conf-enabled/10-cgi.conf
--rw-rw-rw-   0        0        0      454 2023-06-03 17:16:43.000000 jag-panzer-0.1.2/src/jag_panzer/cgi/templates/light_httpd/conf-enabled/10-status.conf
--rw-rw-rw-   0        0        0     2245 2023-06-03 17:16:43.000000 jag-panzer-0.1.2/src/jag_panzer/cgi/templates/light_httpd/server_prms.conf
--rw-rw-rw-   0        0        0      403 2023-06-03 17:16:43.000000 jag-panzer-0.1.2/src/jag_panzer/cgi/templates/unit.service
--rw-rw-rw-   0        0        0     2539 2023-06-08 21:42:17.000000 jag-panzer-0.1.2/src/jag_panzer/dir_list.py
--rw-rw-rw-   0        0        0      369 2023-06-07 05:17:03.000000 jag-panzer-0.1.2/src/jag_panzer/jag_util.py
-drwxrwxrwx   0        0        0        0 2023-06-09 12:35:20.970059 jag-panzer-0.1.2/src/jag_panzer/libs/
-drwxrwxrwx   0        0        0        0 2023-06-09 12:35:21.054016 jag-panzer-0.1.2/src/jag_panzer/libs/bs4/
--rw-rw-rw-   0        0        0    33822 2023-06-06 00:22:44.000000 jag-panzer-0.1.2/src/jag_panzer/libs/bs4/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-09 12:35:21.061032 jag-panzer-0.1.2/src/jag_panzer/libs/bs4/builder/
--rw-rw-rw-   0        0        0    24393 2023-06-06 00:22:44.000000 jag-panzer-0.1.2/src/jag_panzer/libs/bs4/builder/__init__.py
--rw-rw-rw-   0        0        0    19078 2023-06-06 00:22:44.000000 jag-panzer-0.1.2/src/jag_panzer/libs/bs4/builder/_html5lib.py
--rw-rw-rw-   0        0        0    14919 2023-06-06 00:22:44.000000 jag-panzer-0.1.2/src/jag_panzer/libs/bs4/builder/_htmlparser.py
--rw-rw-rw-   0        0        0    14904 2023-06-06 00:22:44.000000 jag-panzer-0.1.2/src/jag_panzer/libs/bs4/builder/_lxml.py
--rw-rw-rw-   0        0        0    10077 2023-06-06 00:22:44.000000 jag-panzer-0.1.2/src/jag_panzer/libs/bs4/css.py
--rw-rw-rw-   0        0        0    41158 2023-06-06 00:22:44.000000 jag-panzer-0.1.2/src/jag_panzer/libs/bs4/dammit.py
--rw-rw-rw-   0        0        0     7195 2023-06-06 00:22:44.000000 jag-panzer-0.1.2/src/jag_panzer/libs/bs4/diagnose.py
--rw-rw-rw-   0        0        0    92716 2023-06-06 00:22:44.000000 jag-panzer-0.1.2/src/jag_panzer/libs/bs4/element.py
--rw-rw-rw-   0        0        0     7184 2023-06-06 00:22:44.000000 jag-panzer-0.1.2/src/jag_panzer/libs/bs4/formatter.py
-drwxrwxrwx   0        0        0        0 2023-06-09 12:35:21.092996 jag-panzer-0.1.2/src/jag_panzer/libs/bs4/tests/
--rw-rw-rw-   0        0        0    48391 2023-06-06 00:22:44.000000 jag-panzer-0.1.2/src/jag_panzer/libs/bs4/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-09 12:35:21.113985 jag-panzer-0.1.2/src/jag_panzer/libs/bs4/tests/fuzz/
--rw-rw-rw-   0        0        0       23 2023-06-06 00:22:44.000000 jag-panzer-0.1.2/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-4818336571064320.testcase
--rw-rw-rw-   0        0        0       30 2023-06-06 00:22:44.000000 jag-panzer-0.1.2/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-4999465949331456.testcase
--rw-rw-rw-   0        0        0    19469 2023-06-06 00:22:44.000000 jag-panzer-0.1.2/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-5167584867909632.testcase
--rw-rw-rw-   0        0        0        5 2023-06-06 00:22:44.000000 jag-panzer-0.1.2/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-5703933063462912.testcase
--rw-rw-rw-   0        0        0       35 2023-06-06 00:22:44.000000 jag-panzer-0.1.2/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-5843991618256896.testcase
--rw-rw-rw-   0        0        0    51495 2023-06-06 00:22:44.000000 jag-panzer-0.1.2/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-5984173902397440.testcase
--rw-rw-rw-   0        0        0    10380 2023-06-06 00:22:44.000000 jag-panzer-0.1.2/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-6124268085182464.testcase
--rw-rw-rw-   0        0        0       19 2023-06-06 00:22:44.000000 jag-panzer-0.1.2/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-6241471367348224.testcase
--rw-rw-rw-   0        0        0     3546 2023-06-06 00:22:44.000000 jag-panzer-0.1.2/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-6450958476902400.testcase
--rw-rw-rw-   0        0        0      124 2023-06-06 00:22:44.000000 jag-panzer-0.1.2/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-6600557255327744.testcase
--rw-rw-rw-   0        0        0     2607 2023-06-06 00:22:44.000000 jag-panzer-0.1.2/src/jag_panzer/libs/bs4/tests/fuzz/crash-0d306a50c8ed8bcd0785b67000fcd5dea1d33f08.testcase
--rw-rw-rw-   0        0        0     1115 2023-06-06 00:22:44.000000 jag-panzer-0.1.2/src/jag_panzer/libs/bs4/tests/test_builder.py
--rw-rw-rw-   0        0        0     5114 2023-06-06 00:22:44.000000 jag-panzer-0.1.2/src/jag_panzer/libs/bs4/tests/test_builder_registry.py
--rw-rw-rw-   0        0        0    17279 2023-06-06 00:22:44.000000 jag-panzer-0.1.2/src/jag_panzer/libs/bs4/tests/test_css.py
--rw-rw-rw-   0        0        0    15451 2023-06-06 00:22:44.000000 jag-panzer-0.1.2/src/jag_panzer/libs/bs4/tests/test_dammit.py
--rw-rw-rw-   0        0        0     1127 2023-06-06 00:22:44.000000 jag-panzer-0.1.2/src/jag_panzer/libs/bs4/tests/test_docs.py
--rw-rw-rw-   0        0        0     2377 2023-06-06 00:22:44.000000 jag-panzer-0.1.2/src/jag_panzer/libs/bs4/tests/test_element.py
--rw-rw-rw-   0        0        0     4148 2023-06-06 00:22:44.000000 jag-panzer-0.1.2/src/jag_panzer/libs/bs4/tests/test_formatter.py
--rw-rw-rw-   0        0        0     3637 2023-06-06 00:22:44.000000 jag-panzer-0.1.2/src/jag_panzer/libs/bs4/tests/test_fuzz.py
--rw-rw-rw-   0        0        0     8322 2023-06-06 00:22:44.000000 jag-panzer-0.1.2/src/jag_panzer/libs/bs4/tests/test_html5lib.py
--rw-rw-rw-   0        0        0     6256 2023-06-06 00:22:44.000000 jag-panzer-0.1.2/src/jag_panzer/libs/bs4/tests/test_htmlparser.py
--rw-rw-rw-   0        0        0     7635 2023-06-06 00:22:44.000000 jag-panzer-0.1.2/src/jag_panzer/libs/bs4/tests/test_lxml.py
--rw-rw-rw-   0        0        0     5081 2023-06-06 00:22:44.000000 jag-panzer-0.1.2/src/jag_panzer/libs/bs4/tests/test_navigablestring.py
--rw-rw-rw-   0        0        0    14274 2023-06-06 00:22:44.000000 jag-panzer-0.1.2/src/jag_panzer/libs/bs4/tests/test_pageelement.py
--rw-rw-rw-   0        0        0    19877 2023-06-06 00:22:44.000000 jag-panzer-0.1.2/src/jag_panzer/libs/bs4/tests/test_soup.py
--rw-rw-rw-   0        0        0     9016 2023-06-06 00:22:44.000000 jag-panzer-0.1.2/src/jag_panzer/libs/bs4/tests/test_tag.py
--rw-rw-rw-   0        0        0    48129 2023-06-06 00:22:44.000000 jag-panzer-0.1.2/src/jag_panzer/libs/bs4/tests/test_tree.py
-drwxrwxrwx   0        0        0        0 2023-06-09 12:35:21.128976 jag-panzer-0.1.2/src/jag_panzer/libs/soupsieve/
--rw-rw-rw-   0        0        0     4630 2023-06-06 00:22:44.000000 jag-panzer-0.1.2/src/jag_panzer/libs/soupsieve/__init__.py
--rw-rw-rw-   0        0        0     6842 2023-06-06 00:22:44.000000 jag-panzer-0.1.2/src/jag_panzer/libs/soupsieve/__meta__.py
--rw-rw-rw-   0        0        0    58152 2023-06-06 00:22:44.000000 jag-panzer-0.1.2/src/jag_panzer/libs/soupsieve/css_match.py
--rw-rw-rw-   0        0        0    47063 2023-06-06 00:22:44.000000 jag-panzer-0.1.2/src/jag_panzer/libs/soupsieve/css_parser.py
--rw-rw-rw-   0        0        0    10337 2023-06-06 00:22:44.000000 jag-panzer-0.1.2/src/jag_panzer/libs/soupsieve/css_types.py
--rw-rw-rw-   0        0        0     4053 2023-06-06 00:22:44.000000 jag-panzer-0.1.2/src/jag_panzer/libs/soupsieve/pretty.py
--rw-rw-rw-   0        0        0        0 2023-06-06 00:22:44.000000 jag-panzer-0.1.2/src/jag_panzer/libs/soupsieve/py.typed
--rw-rw-rw-   0        0        0     3374 2023-06-06 00:22:44.000000 jag-panzer-0.1.2/src/jag_panzer/libs/soupsieve/util.py
-drwxrwxrwx   0        0        0        0 2023-06-09 12:35:21.137970 jag-panzer-0.1.2/src/jag_panzer/libs/yattag/
--rw-rw-rw-   0        0        0     1743 2023-03-03 09:07:48.000000 jag-panzer-0.1.2/src/jag_panzer/libs/yattag/__init__.py
--rw-rw-rw-   0        0        0    18197 2020-08-06 21:26:32.000000 jag-panzer-0.1.2/src/jag_panzer/libs/yattag/doc.py
--rw-rw-rw-   0        0        0    12029 2023-01-02 11:12:52.000000 jag-panzer-0.1.2/src/jag_panzer/libs/yattag/indentation.py
--rw-rw-rw-   0        0        0        0 2019-12-25 20:07:02.000000 jag-panzer-0.1.2/src/jag_panzer/libs/yattag/py.typed
--rw-rw-rw-   0        0        0    18081 2019-12-24 00:01:02.000000 jag-panzer-0.1.2/src/jag_panzer/libs/yattag/simpledoc.py
-drwxrwxrwx   0        0        0        0 2023-06-09 12:35:21.139969 jag-panzer-0.1.2/src/jag_panzer/mimes/
--rw-rw-rw-   0        0        0     2762 2023-06-03 17:16:43.000000 jag-panzer-0.1.2/src/jag_panzer/mimes/mime_types_base.py
--rw-rw-rw-   0        0        0     1938 2023-06-03 17:16:43.000000 jag-panzer-0.1.2/src/jag_panzer/response_codes.py
--rw-rw-rw-   0        0        0     7498 2023-06-09 12:34:32.000000 jag-panzer-0.1.2/src/jag_panzer/server.py
--rwxrwxrwx   0        0        0       12 2023-06-07 01:47:22.000000 jag-panzer-0.1.2/src/jag_panzer/test.cmd
-drwxrwxrwx   0        0        0        0 2023-06-09 12:35:21.016042 jag-panzer-0.1.2/src/jag_panzer.egg-info/
--rw-rw-rw-   0        0        0      560 2023-06-09 12:35:20.000000 jag-panzer-0.1.2/src/jag_panzer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3986 2023-06-09 12:35:20.000000 jag-panzer-0.1.2/src/jag_panzer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 12:35:20.000000 jag-panzer-0.1.2/src/jag_panzer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-06-09 12:35:20.000000 jag-panzer-0.1.2/src/jag_panzer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-10 02:03:13.612119 jag-panzer-0.1.21/
+-rw-rw-rw-   0        0        0      161 2023-06-09 00:40:57.000000 jag-panzer-0.1.21/LICENSE
+-rw-rw-rw-   0        0        0       46 2023-06-09 02:05:06.000000 jag-panzer-0.1.21/MANIFEST.in
+-rw-rw-rw-   0        0        0      561 2023-06-10 02:03:13.612119 jag-panzer-0.1.21/PKG-INFO
+-rw-rw-rw-   0        0        0       26 2023-06-09 00:32:58.000000 jag-panzer-0.1.21/README.md
+-rw-rw-rw-   0        0        0      108 2023-06-09 00:12:29.000000 jag-panzer-0.1.21/pyproject.toml
+-rw-rw-rw-   0        0        0      672 2023-06-10 02:03:13.619096 jag-panzer-0.1.21/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-10 02:03:10.393728 jag-panzer-0.1.21/src/
+drwxrwxrwx   0        0        0        0 2023-06-10 02:03:11.383087 jag-panzer-0.1.21/src/jag_panzer/
+-rw-rw-rw-   0        0        0        0 2023-06-09 00:13:59.000000 jag-panzer-0.1.21/src/jag_panzer/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-10 02:03:11.480120 jag-panzer-0.1.21/src/jag_panzer/assets/
+drwxrwxrwx   0        0        0        0 2023-06-10 02:03:11.759076 jag-panzer-0.1.21/src/jag_panzer/assets/dir_listing/
+-rw-rw-rw-   0        0        0      356 2023-06-08 21:39:34.000000 jag-panzer-0.1.21/src/jag_panzer/assets/dir_listing/base.html
+-rw-rw-rw-   0        0        0      446 2023-06-06 00:39:53.000000 jag-panzer-0.1.21/src/jag_panzer/assets/dir_listing/dir_icon.svg
+-rw-rw-rw-   0        0        0      682 2023-06-07 06:27:42.000000 jag-panzer-0.1.21/src/jag_panzer/assets/dir_listing/download_icon.svg
+-rw-rw-rw-   0        0        0      704 2023-06-06 00:40:06.000000 jag-panzer-0.1.21/src/jag_panzer/assets/dir_listing/file_icon.svg
+-rw-rw-rw-   0        0        0       21 2023-06-06 01:12:59.000000 jag-panzer-0.1.21/src/jag_panzer/assets/dir_listing/script.js
+-rw-rw-rw-   0        0        0     1355 2023-06-07 07:34:01.000000 jag-panzer-0.1.21/src/jag_panzer/assets/dir_listing/style.css
+-rw-rw-rw-   0        0        0      260 2023-06-07 02:18:15.000000 jag-panzer-0.1.21/src/jag_panzer/assets/reject.html
+-rw-rw-rw-   0        0        0    20150 2023-06-10 02:01:28.000000 jag-panzer-0.1.21/src/jag_panzer/base_room.py
+drwxrwxrwx   0        0        0        0 2023-06-10 02:03:11.912085 jag-panzer-0.1.21/src/jag_panzer/cgi/
+-rw-rw-rw-   0        0        0        0 2023-06-09 00:00:24.000000 jag-panzer-0.1.21/src/jag_panzer/cgi/__init__.py
+-rw-rw-rw-   0        0        0     5087 2023-06-03 17:16:43.000000 jag-panzer-0.1.21/src/jag_panzer/cgi/burn_power.py
+-rw-rw-rw-   0        0        0      451 2023-06-03 17:16:43.000000 jag-panzer-0.1.21/src/jag_panzer/cgi/hitman.py
+-rw-rw-rw-   0        0        0     6691 2023-06-03 17:16:43.000000 jag-panzer-0.1.21/src/jag_panzer/cgi/jag.py
+drwxrwxrwx   0        0        0        0 2023-06-10 02:03:11.918069 jag-panzer-0.1.21/src/jag_panzer/cgi/templates/
+drwxrwxrwx   0        0        0        0 2023-06-10 02:03:11.941103 jag-panzer-0.1.21/src/jag_panzer/cgi/templates/light_httpd/
+drwxrwxrwx   0        0        0        0 2023-06-10 02:03:11.977094 jag-panzer-0.1.21/src/jag_panzer/cgi/templates/light_httpd/conf-enabled/
+-rw-rw-rw-   0        0        0       91 2023-06-03 17:16:43.000000 jag-panzer-0.1.21/src/jag_panzer/cgi/templates/light_httpd/conf-enabled/10-accesslog.conf
+-rw-rw-rw-   0        0        0      306 2023-06-03 17:16:43.000000 jag-panzer-0.1.21/src/jag_panzer/cgi/templates/light_httpd/conf-enabled/10-cgi.conf
+-rw-rw-rw-   0        0        0      454 2023-06-03 17:16:43.000000 jag-panzer-0.1.21/src/jag_panzer/cgi/templates/light_httpd/conf-enabled/10-status.conf
+-rw-rw-rw-   0        0        0     2245 2023-06-03 17:16:43.000000 jag-panzer-0.1.21/src/jag_panzer/cgi/templates/light_httpd/server_prms.conf
+-rw-rw-rw-   0        0        0      403 2023-06-03 17:16:43.000000 jag-panzer-0.1.21/src/jag_panzer/cgi/templates/unit.service
+-rw-rw-rw-   0        0        0     2539 2023-06-08 21:42:17.000000 jag-panzer-0.1.21/src/jag_panzer/dir_list.py
+-rw-rw-rw-   0        0        0      369 2023-06-07 05:17:03.000000 jag-panzer-0.1.21/src/jag_panzer/jag_util.py
+drwxrwxrwx   0        0        0        0 2023-06-10 02:03:10.720021 jag-panzer-0.1.21/src/jag_panzer/libs/
+drwxrwxrwx   0        0        0        0 2023-06-10 02:03:12.225111 jag-panzer-0.1.21/src/jag_panzer/libs/bs4/
+-rw-rw-rw-   0        0        0    33822 2023-06-06 00:22:44.000000 jag-panzer-0.1.21/src/jag_panzer/libs/bs4/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-10 02:03:12.443199 jag-panzer-0.1.21/src/jag_panzer/libs/bs4/builder/
+-rw-rw-rw-   0        0        0    24393 2023-06-06 00:22:44.000000 jag-panzer-0.1.21/src/jag_panzer/libs/bs4/builder/__init__.py
+-rw-rw-rw-   0        0        0    19078 2023-06-06 00:22:44.000000 jag-panzer-0.1.21/src/jag_panzer/libs/bs4/builder/_html5lib.py
+-rw-rw-rw-   0        0        0    14919 2023-06-06 00:22:44.000000 jag-panzer-0.1.21/src/jag_panzer/libs/bs4/builder/_htmlparser.py
+-rw-rw-rw-   0        0        0    14904 2023-06-06 00:22:44.000000 jag-panzer-0.1.21/src/jag_panzer/libs/bs4/builder/_lxml.py
+-rw-rw-rw-   0        0        0    10077 2023-06-06 00:22:44.000000 jag-panzer-0.1.21/src/jag_panzer/libs/bs4/css.py
+-rw-rw-rw-   0        0        0    41158 2023-06-06 00:22:44.000000 jag-panzer-0.1.21/src/jag_panzer/libs/bs4/dammit.py
+-rw-rw-rw-   0        0        0     7195 2023-06-06 00:22:44.000000 jag-panzer-0.1.21/src/jag_panzer/libs/bs4/diagnose.py
+-rw-rw-rw-   0        0        0    92716 2023-06-06 00:22:44.000000 jag-panzer-0.1.21/src/jag_panzer/libs/bs4/element.py
+-rw-rw-rw-   0        0        0     7184 2023-06-06 00:22:44.000000 jag-panzer-0.1.21/src/jag_panzer/libs/bs4/formatter.py
+drwxrwxrwx   0        0        0        0 2023-06-10 02:03:12.937154 jag-panzer-0.1.21/src/jag_panzer/libs/bs4/tests/
+-rw-rw-rw-   0        0        0    48391 2023-06-06 00:22:44.000000 jag-panzer-0.1.21/src/jag_panzer/libs/bs4/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-10 02:03:13.171061 jag-panzer-0.1.21/src/jag_panzer/libs/bs4/tests/fuzz/
+-rw-rw-rw-   0        0        0       23 2023-06-06 00:22:44.000000 jag-panzer-0.1.21/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-4818336571064320.testcase
+-rw-rw-rw-   0        0        0       30 2023-06-06 00:22:44.000000 jag-panzer-0.1.21/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-4999465949331456.testcase
+-rw-rw-rw-   0        0        0    19469 2023-06-06 00:22:44.000000 jag-panzer-0.1.21/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-5167584867909632.testcase
+-rw-rw-rw-   0        0        0        5 2023-06-06 00:22:44.000000 jag-panzer-0.1.21/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-5703933063462912.testcase
+-rw-rw-rw-   0        0        0       35 2023-06-06 00:22:44.000000 jag-panzer-0.1.21/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-5843991618256896.testcase
+-rw-rw-rw-   0        0        0    51495 2023-06-06 00:22:44.000000 jag-panzer-0.1.21/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-5984173902397440.testcase
+-rw-rw-rw-   0        0        0    10380 2023-06-06 00:22:44.000000 jag-panzer-0.1.21/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-6124268085182464.testcase
+-rw-rw-rw-   0        0        0       19 2023-06-06 00:22:44.000000 jag-panzer-0.1.21/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-6241471367348224.testcase
+-rw-rw-rw-   0        0        0     3546 2023-06-06 00:22:44.000000 jag-panzer-0.1.21/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-6450958476902400.testcase
+-rw-rw-rw-   0        0        0      124 2023-06-06 00:22:44.000000 jag-panzer-0.1.21/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-6600557255327744.testcase
+-rw-rw-rw-   0        0        0     2607 2023-06-06 00:22:44.000000 jag-panzer-0.1.21/src/jag_panzer/libs/bs4/tests/fuzz/crash-0d306a50c8ed8bcd0785b67000fcd5dea1d33f08.testcase
+-rw-rw-rw-   0        0        0     1115 2023-06-06 00:22:44.000000 jag-panzer-0.1.21/src/jag_panzer/libs/bs4/tests/test_builder.py
+-rw-rw-rw-   0        0        0     5114 2023-06-06 00:22:44.000000 jag-panzer-0.1.21/src/jag_panzer/libs/bs4/tests/test_builder_registry.py
+-rw-rw-rw-   0        0        0    17279 2023-06-06 00:22:44.000000 jag-panzer-0.1.21/src/jag_panzer/libs/bs4/tests/test_css.py
+-rw-rw-rw-   0        0        0    15451 2023-06-06 00:22:44.000000 jag-panzer-0.1.21/src/jag_panzer/libs/bs4/tests/test_dammit.py
+-rw-rw-rw-   0        0        0     1127 2023-06-06 00:22:44.000000 jag-panzer-0.1.21/src/jag_panzer/libs/bs4/tests/test_docs.py
+-rw-rw-rw-   0        0        0     2377 2023-06-06 00:22:44.000000 jag-panzer-0.1.21/src/jag_panzer/libs/bs4/tests/test_element.py
+-rw-rw-rw-   0        0        0     4148 2023-06-06 00:22:44.000000 jag-panzer-0.1.21/src/jag_panzer/libs/bs4/tests/test_formatter.py
+-rw-rw-rw-   0        0        0     3637 2023-06-06 00:22:44.000000 jag-panzer-0.1.21/src/jag_panzer/libs/bs4/tests/test_fuzz.py
+-rw-rw-rw-   0        0        0     8322 2023-06-06 00:22:44.000000 jag-panzer-0.1.21/src/jag_panzer/libs/bs4/tests/test_html5lib.py
+-rw-rw-rw-   0        0        0     6256 2023-06-06 00:22:44.000000 jag-panzer-0.1.21/src/jag_panzer/libs/bs4/tests/test_htmlparser.py
+-rw-rw-rw-   0        0        0     7635 2023-06-06 00:22:44.000000 jag-panzer-0.1.21/src/jag_panzer/libs/bs4/tests/test_lxml.py
+-rw-rw-rw-   0        0        0     5081 2023-06-06 00:22:44.000000 jag-panzer-0.1.21/src/jag_panzer/libs/bs4/tests/test_navigablestring.py
+-rw-rw-rw-   0        0        0    14274 2023-06-06 00:22:44.000000 jag-panzer-0.1.21/src/jag_panzer/libs/bs4/tests/test_pageelement.py
+-rw-rw-rw-   0        0        0    19877 2023-06-06 00:22:44.000000 jag-panzer-0.1.21/src/jag_panzer/libs/bs4/tests/test_soup.py
+-rw-rw-rw-   0        0        0     9016 2023-06-06 00:22:44.000000 jag-panzer-0.1.21/src/jag_panzer/libs/bs4/tests/test_tag.py
+-rw-rw-rw-   0        0        0    48129 2023-06-06 00:22:44.000000 jag-panzer-0.1.21/src/jag_panzer/libs/bs4/tests/test_tree.py
+drwxrwxrwx   0        0        0        0 2023-06-10 02:03:13.438156 jag-panzer-0.1.21/src/jag_panzer/libs/soupsieve/
+-rw-rw-rw-   0        0        0     4630 2023-06-06 00:22:44.000000 jag-panzer-0.1.21/src/jag_panzer/libs/soupsieve/__init__.py
+-rw-rw-rw-   0        0        0     6842 2023-06-06 00:22:44.000000 jag-panzer-0.1.21/src/jag_panzer/libs/soupsieve/__meta__.py
+-rw-rw-rw-   0        0        0    58152 2023-06-06 00:22:44.000000 jag-panzer-0.1.21/src/jag_panzer/libs/soupsieve/css_match.py
+-rw-rw-rw-   0        0        0    47063 2023-06-06 00:22:44.000000 jag-panzer-0.1.21/src/jag_panzer/libs/soupsieve/css_parser.py
+-rw-rw-rw-   0        0        0    10337 2023-06-06 00:22:44.000000 jag-panzer-0.1.21/src/jag_panzer/libs/soupsieve/css_types.py
+-rw-rw-rw-   0        0        0     4053 2023-06-06 00:22:44.000000 jag-panzer-0.1.21/src/jag_panzer/libs/soupsieve/pretty.py
+-rw-rw-rw-   0        0        0        0 2023-06-06 00:22:44.000000 jag-panzer-0.1.21/src/jag_panzer/libs/soupsieve/py.typed
+-rw-rw-rw-   0        0        0     3374 2023-06-06 00:22:44.000000 jag-panzer-0.1.21/src/jag_panzer/libs/soupsieve/util.py
+drwxrwxrwx   0        0        0        0 2023-06-10 02:03:13.568591 jag-panzer-0.1.21/src/jag_panzer/libs/yattag/
+-rw-rw-rw-   0        0        0     1743 2023-03-03 09:07:48.000000 jag-panzer-0.1.21/src/jag_panzer/libs/yattag/__init__.py
+-rw-rw-rw-   0        0        0    18197 2020-08-06 21:26:32.000000 jag-panzer-0.1.21/src/jag_panzer/libs/yattag/doc.py
+-rw-rw-rw-   0        0        0    12029 2023-01-02 11:12:52.000000 jag-panzer-0.1.21/src/jag_panzer/libs/yattag/indentation.py
+-rw-rw-rw-   0        0        0        0 2019-12-25 20:07:02.000000 jag-panzer-0.1.21/src/jag_panzer/libs/yattag/py.typed
+-rw-rw-rw-   0        0        0    18081 2019-12-24 00:01:02.000000 jag-panzer-0.1.21/src/jag_panzer/libs/yattag/simpledoc.py
+drwxrwxrwx   0        0        0        0 2023-06-10 02:03:13.608094 jag-panzer-0.1.21/src/jag_panzer/mimes/
+-rw-rw-rw-   0        0        0     2762 2023-06-03 17:16:43.000000 jag-panzer-0.1.21/src/jag_panzer/mimes/mime_types_base.py
+-rw-rw-rw-   0        0        0     1938 2023-06-03 17:16:43.000000 jag-panzer-0.1.21/src/jag_panzer/response_codes.py
+-rw-rw-rw-   0        0        0     7795 2023-06-10 01:24:17.000000 jag-panzer-0.1.21/src/jag_panzer/server.py
+-rwxrwxrwx   0        0        0       12 2023-06-07 01:47:22.000000 jag-panzer-0.1.21/src/jag_panzer/test.cmd
+drwxrwxrwx   0        0        0        0 2023-06-10 02:03:11.475123 jag-panzer-0.1.21/src/jag_panzer.egg-info/
+-rw-rw-rw-   0        0        0      561 2023-06-10 02:03:10.000000 jag-panzer-0.1.21/src/jag_panzer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3986 2023-06-10 02:03:10.000000 jag-panzer-0.1.21/src/jag_panzer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-10 02:03:10.000000 jag-panzer-0.1.21/src/jag_panzer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-06-10 02:03:10.000000 jag-panzer-0.1.21/src/jag_panzer.egg-info/top_level.txt
```

### Comparing `jag-panzer-0.1.2/PKG-INFO` & `jag-panzer-0.1.21/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jag-panzer
-Version: 0.1.2
+Version: 0.1.21
 Summary: Simple HTTP server allowing pure python workflow
 Home-page: https://github.com/MrKleiner/jag
 Author: Mr.Kleiner
 Author-email: megaadrenaline1055@gmail.com
 Project-URL: Bug Tracker, https://github.com/MrKleiner/jag/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `jag-panzer-0.1.2/setup.cfg` & `jag-panzer-0.1.21/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206a 6167 2d70 616e 7a65 720d 0a76   = jag-panzer..v
-00000020: 6572 7369 6f6e 203d 2030 2e31 2e32 0d0a  ersion = 0.1.2..
-00000030: 6175 7468 6f72 203d 204d 722e 4b6c 6569  author = Mr.Klei
-00000040: 6e65 720d 0a61 7574 686f 725f 656d 6169  ner..author_emai
-00000050: 6c20 3d20 6d65 6761 6164 7265 6e61 6c69  l = megaadrenali
-00000060: 6e65 3130 3535 4067 6d61 696c 2e63 6f6d  ne1055@gmail.com
-00000070: 0d0a 6465 7363 7269 7074 696f 6e20 3d20  ..description = 
-00000080: 5369 6d70 6c65 2048 5454 5020 7365 7276  Simple HTTP serv
-00000090: 6572 2061 6c6c 6f77 696e 6720 7075 7265  er allowing pure
-000000a0: 2070 7974 686f 6e20 776f 726b 666c 6f77   python workflow
-000000b0: 0d0a 6c6f 6e67 5f64 6573 6372 6970 7469  ..long_descripti
-000000c0: 6f6e 203d 2066 696c 653a 2052 4541 444d  on = file: READM
-000000d0: 452e 6d64 0d0a 6c6f 6e67 5f64 6573 6372  E.md..long_descr
-000000e0: 6970 7469 6f6e 5f63 6f6e 7465 6e74 5f74  iption_content_t
-000000f0: 7970 6520 3d20 7465 7874 2f6d 6172 6b64  ype = text/markd
-00000100: 6f77 6e0d 0a75 726c 203d 2068 7474 7073  own..url = https
-00000110: 3a2f 2f67 6974 6875 622e 636f 6d2f 4d72  ://github.com/Mr
-00000120: 4b6c 6569 6e65 722f 6a61 670d 0a70 726f  Kleiner/jag..pro
-00000130: 6a65 6374 5f75 726c 7320 3d20 0d0a 0942  ject_urls = ...B
-00000140: 7567 2054 7261 636b 6572 203d 2068 7474  ug Tracker = htt
-00000150: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000160: 4d72 4b6c 6569 6e65 722f 6a61 672f 6973  MrKleiner/jag/is
-00000170: 7375 6573 0d0a 636c 6173 7369 6669 6572  sues..classifier
-00000180: 7320 3d20 0d0a 0950 726f 6772 616d 6d69  s = ...Programmi
-00000190: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
-000001a0: 7974 686f 6e20 3a3a 2033 0d0a 094c 6963  ython :: 3...Lic
-000001b0: 656e 7365 203a 3a20 4f53 4920 4170 7072  ense :: OSI Appr
-000001c0: 6f76 6564 203a 3a20 4d49 5420 4c69 6365  oved :: MIT Lice
-000001d0: 6e73 650d 0a09 4f70 6572 6174 696e 6720  nse...Operating 
-000001e0: 5379 7374 656d 203a 3a20 4f53 2049 6e64  System :: OS Ind
-000001f0: 6570 656e 6465 6e74 0d0a 0d0a 5b6f 7074  ependent....[opt
-00000200: 696f 6e73 5d0d 0a70 6163 6b61 6765 5f64  ions]..package_d
-00000210: 6972 203d 200d 0a09 3d20 7372 630d 0a70  ir = ...= src..p
-00000220: 6163 6b61 6765 7320 3d20 6669 6e64 3a0d  ackages = find:.
-00000230: 0a70 7974 686f 6e5f 7265 7175 6972 6573  .python_requires
-00000240: 203d 203e 3d33 2e31 300d 0a0d 0a5b 6f70   = >=3.10....[op
-00000250: 7469 6f6e 732e 7061 636b 6167 6573 2e66  tions.packages.f
-00000260: 696e 645d 0d0a 7768 6572 6520 3d20 7372  ind]..where = sr
-00000270: 630d 0a0d 0a5b 6567 675f 696e 666f 5d0d  c....[egg_info].
-00000280: 0a74 6167 5f62 7569 6c64 203d 200d 0a74  .tag_build = ..t
-00000290: 6167 5f64 6174 6520 3d20 300d 0a0d 0a    ag_date = 0....
+00000020: 6572 7369 6f6e 203d 2030 2e31 2e32 310d  ersion = 0.1.21.
+00000030: 0a61 7574 686f 7220 3d20 4d72 2e4b 6c65  .author = Mr.Kle
+00000040: 696e 6572 0d0a 6175 7468 6f72 5f65 6d61  iner..author_ema
+00000050: 696c 203d 206d 6567 6161 6472 656e 616c  il = megaadrenal
+00000060: 696e 6531 3035 3540 676d 6169 6c2e 636f  ine1055@gmail.co
+00000070: 6d0d 0a64 6573 6372 6970 7469 6f6e 203d  m..description =
+00000080: 2053 696d 706c 6520 4854 5450 2073 6572   Simple HTTP ser
+00000090: 7665 7220 616c 6c6f 7769 6e67 2070 7572  ver allowing pur
+000000a0: 6520 7079 7468 6f6e 2077 6f72 6b66 6c6f  e python workflo
+000000b0: 770d 0a6c 6f6e 675f 6465 7363 7269 7074  w..long_descript
+000000c0: 696f 6e20 3d20 6669 6c65 3a20 5245 4144  ion = file: READ
+000000d0: 4d45 2e6d 640d 0a6c 6f6e 675f 6465 7363  ME.md..long_desc
+000000e0: 7269 7074 696f 6e5f 636f 6e74 656e 745f  ription_content_
+000000f0: 7479 7065 203d 2074 6578 742f 6d61 726b  type = text/mark
+00000100: 646f 776e 0d0a 7572 6c20 3d20 6874 7470  down..url = http
+00000110: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f4d  s://github.com/M
+00000120: 724b 6c65 696e 6572 2f6a 6167 0d0a 7072  rKleiner/jag..pr
+00000130: 6f6a 6563 745f 7572 6c73 203d 200d 0a09  oject_urls = ...
+00000140: 4275 6720 5472 6163 6b65 7220 3d20 6874  Bug Tracker = ht
+00000150: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000160: 2f4d 724b 6c65 696e 6572 2f6a 6167 2f69  /MrKleiner/jag/i
+00000170: 7373 7565 730d 0a63 6c61 7373 6966 6965  ssues..classifie
+00000180: 7273 203d 200d 0a09 5072 6f67 7261 6d6d  rs = ...Programm
+00000190: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
+000001a0: 5079 7468 6f6e 203a 3a20 330d 0a09 4c69  Python :: 3...Li
+000001b0: 6365 6e73 6520 3a3a 204f 5349 2041 7070  cense :: OSI App
+000001c0: 726f 7665 6420 3a3a 204d 4954 204c 6963  roved :: MIT Lic
+000001d0: 656e 7365 0d0a 094f 7065 7261 7469 6e67  ense...Operating
+000001e0: 2053 7973 7465 6d20 3a3a 204f 5320 496e   System :: OS In
+000001f0: 6465 7065 6e64 656e 740d 0a0d 0a5b 6f70  dependent....[op
+00000200: 7469 6f6e 735d 0d0a 7061 636b 6167 655f  tions]..package_
+00000210: 6469 7220 3d20 0d0a 093d 2073 7263 0d0a  dir = ...= src..
+00000220: 7061 636b 6167 6573 203d 2066 696e 643a  packages = find:
+00000230: 0d0a 7079 7468 6f6e 5f72 6571 7569 7265  ..python_require
+00000240: 7320 3d20 3e3d 332e 3130 0d0a 0d0a 5b6f  s = >=3.10....[o
+00000250: 7074 696f 6e73 2e70 6163 6b61 6765 732e  ptions.packages.
+00000260: 6669 6e64 5d0d 0a77 6865 7265 203d 2073  find]..where = s
+00000270: 7263 0d0a 0d0a 5b65 6767 5f69 6e66 6f5d  rc....[egg_info]
+00000280: 0d0a 7461 675f 6275 696c 6420 3d20 0d0a  ..tag_build = ..
+00000290: 7461 675f 6461 7465 203d 2030 0d0a 0d0a  tag_date = 0....
```

### Comparing `jag-panzer-0.1.2/src/jag_panzer/assets/dir_listing/download_icon.svg` & `jag-panzer-0.1.21/src/jag_panzer/assets/dir_listing/download_icon.svg`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.2/src/jag_panzer/assets/dir_listing/file_icon.svg` & `jag-panzer-0.1.21/src/jag_panzer/assets/dir_listing/file_icon.svg`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.2/src/jag_panzer/assets/dir_listing/style.css` & `jag-panzer-0.1.21/src/jag_panzer/assets/dir_listing/style.css`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.2/src/jag_panzer/base_room.py` & `jag-panzer-0.1.21/src/jag_panzer/base_room.py`

 * *Files 5% similar despite different names*

```diff
@@ -50,14 +50,21 @@
 	def __init__(self, request, response):
 		self.request = request
 		self.response = response
 
 	# Serve a file to the client in a CDN manner
 	# If no file is provided - serve path from the request
 	def serve_file(self, tgt_file=None, respect_range=True):
+		"""
+		Serve a file to the client.
+		It's possible to specify a target file.
+		If no target file is specified, then reuqest path is used.
+		- tgt_file: Path to the file to serve, defaults to request path.
+		- respect_range: Take the "Range" header into account.
+		"""
 		request = self.request
 		response = self.response
 
 		if not request.abspath.is_file():
 			self.request.reject()
 			return
 
@@ -67,70 +74,90 @@
 			or
 			'application/octet-stream'
 		)
 
 		# if the size is too big for a single flush - stream in chunks
 		# This is very important, because serving a 2kb svg in chunks slows the response time
 		# and serving an 18gb .mkv Blu-ray remux in a single flush is impossible
-		if request.abspath.stat().st_size > request.srv_res.cfg['static_cdn']['max_buffered_size']:
+		if request.abspath.stat().st_size > request.srv_res.cfg['buffers']['max_file_len']:
 			with open(str(request.abspath), 'r+b') as f:
 				# if request comes with a Range header - try serving the requested byterange
 				# '0-' VERY funny, fuck right off
-				if request.byterange and (request.headers['range'].strip() != '0-') and respect_range:
+				if request.byterange and (request.headers.get('range', 'bytes=0-').strip() != 'bytes=0-') and respect_range:
+					conlog('The client has fucked us over:', request.headers.get('range', '0-').strip())
 					response.serve_range(f)
 				else:
 					response.stream_buffer(f, (1024*1024)*5)
 		else:
 			response.flush_buffer(request.abspath.read_bytes())
 
 		self.request.terminate()
 
 	# List directory as an html page
-	def list_dir(self, respect_htaccess=True):
+	def list_dir(self):
+		"""
+		- Set content type to text/html
+		- Progressively generate listing for a directory and stream it to the client
+		- Close connection
+		"""
 		self.response.content_type = 'text/html'
 
 		with self.response.stream_bytechunks() as stream:
 			for chunk in self.request.srv_res.list_dir.dir_as_html(self.request.abspath):
 				stream.send(chunk)
 
-		self.request.terminate()
 
 	# Serve "index.html" from the requested path
 	# according to server config
 	def serve_dir_index(self):
+		"""
+		Serve "index.html" from the requested path
+		If the file mentioned above doesn't exist in the dir - reject
+		"""
 		if not (self.request.abspath / 'index.html').is_file():
 			self.request.reject()
 
 		self.response.content_type = 'text/html'
 		self.response.flush_buffer(
 			(self.request.abspath / 'index.html').read_bytes()
 		)
 
 	# Because why not
 	def default(self):
+		"""
+		Execute default stack of actions:
+		- if it's a GET request (reject otherwise):
+			- If request path is not relative to the doc root - reject
+			- If request points to a file - serve it
+			- If request points to a directory - list it IF dir listing is enabled
+		"""
 		_default_room(self.request, self.response, self)
 
 
 
 
 
 
 
 # Stream chunks
 class _chunkstream:
-	def __init__(self, cl_con):
+	def __init__(self, request, cl_con, self_terminate):
 		self.cl_con = cl_con
+		self.request = request
+		self.auto_term = self_terminate
 
 	def __enter__(self):
 		return self
 
 	def __exit__(self, type, value, traceback):
 		self.cl_con.sendall(b'0\r\n\r\n')
-		# No termination, because it's speculated,
-		# that it's possible to send some sort of trailing headers
+		# No auto termination, because it's speculated,
+		# that it's possible to send some sort of trailing headers or whatever
+		if self.auto_term:
+			self.request.terminate()
 
 	def send(self, data):
 		# send the chunk size
 		self.cl_con.sendall(f"""{hex(len(data)).lstrip('0x')}\r\n""".encode())
 		# send the chunk itself
 		self.cl_con.sendall(data)
 		# send separator
@@ -142,19 +169,21 @@
 # Read part of a buffer in chunks (start:end)
 # todo: There are 0 validations
 # (neither end or start can be negative)
 # (end cannot be smaller than start)
 # (start and end cannot be the same)
 # (start and end should not result into 0 bytes read)
 
-# src  ------------------------
-# rng        ^         ^
-# prog       -----
-# want            ---------
-# let             -----
+# src  -----------------------
+# rng        ^         ^      
+# prog       -----            
+# want            ---------   
+# let             ------      
+
+# RANGES ARE INCLUSIVE IN HTTP !
 class aligned_buf_read:
 	def __init__(self, buf, start, end):
 		# START is inclusive
 		# END is NOT inclusive
 		self.buf = buf
 		self.start = start
 		self.end = end
@@ -224,15 +253,15 @@
 		as a file download by the client.
 		Useful when a media file, like .mp4 video should be downloaded
 		by the client instead of playing back.
 		"""
 		self.headers['Content-Disposition'] = f'attachment; filename="{str(filename)}"'
 
 	# - Send headers to the client
-	# - Send the entirety of the provided buffer in one go
+	# - Send the entirety of the provided buffer/bytes in one go
 	# - Collapse connection
 	def flush_buffer(self, data):
 		if not isinstance(data, bytes):
 			data = data.getvalue()
 
 		# important todo: the response should either be chunked or have Content-Length header
 		self.headers['Content-Length'] = len(data)
@@ -242,54 +271,65 @@
 
 		# send the body
 		self.cl_con.sendall(data)
 
 		# terminate
 		self.request.terminate()
 
-	def stream_bytechunks(self):
+	def stream_bytechunks(self, self_terminate=True):
+		"""
+		Stream data to the client in HTTP chunks:
+		- set 'Transfer-Encoding' header to 'chunked'
+		- Dump headers
+		- Start streaming chunks:
+			- This returns an object for use with "with" keyword.
+			- The object only has 1 method: send()
+			  Which only takes 1 argument: Bytes to send
+		"""
+
 		# This cannot be otherwise
 		self.headers['Transfer-Encoding'] = 'chunked'
 		# It's impossible to stream multiple groups of chunks
 		self.send_preflight()
 
-		return _chunkstream(self.cl_con)
+		return _chunkstream(self.request, self.cl_con, self_terminate)
 
 	# Automated action:
 	# - Add 'Transfer-Encoding: chunked' header
 	# - Send headers to the client
 	# - Stream the entirety of the provided buffer in chunks
 	# - Collapse the connection
-	def stream_buffer(self, data, chunk_size=65535):
+	def stream_buffer(self, data, chunk_size=None):
 		"""
 		Send the data in chunks.
 		data = io.BytesIO object.
-		chunk_size = the size of a single chunk in bytes
+		chunk_size = the size of a single chunk in bytes, default to server config
+		Example usage: Pass buffer of an open file to stream it to the client.
 		"""
 
 		# The response is EITHER chunked OR has Content-Length
 		self.headers['Transfer-Encoding'] = 'chunked'
 
 		# first - dump headers
 		self.send_preflight()
 
 		# Safety (tin foil hat): Move the carret to the very beginning of the buffer
 		data.seek(0, 0)
 		# stream chunks
 		with self.stream_bytechunks() as stream:
 			while True:
 				# read chunk
-				chunk = data.read(chunk_size)
+				chunk = data.read(
+					chunk_size or self.srv_res.cfg['buffers']['bufstream_chunk_len']
+				)
 				# check if there's still any data
 				if not chunk:
 					break
 				stream.send(chunk)
 
-		# collapse the connection
-		self.request.terminate()
 
 	# Serve specified buffer according to the Range header
 	# important todo: This is 100% raw/bare
 	# nothing is checked or validated
 	def serve_range(self, buf):
 		# Set code to partial-content
 		self.code = 206
@@ -304,29 +344,30 @@
 			# stream all chunk groups
 			# (order is preserved)
 			for chunk_start, chunk_end in self.request.byterange:
 				# Python is amazing: array[37:None] is a valid syntax
 				_start = chunk_start
 				_end = chunk_end or buf_size
 
+				conlog('Serving partial content', self.request.byterange, _start, _end)
+
 				# If only end is specified - stream suffix
 				# Todo: current implementation requires calculating
 				# start offset, which means that buffer should be of known size
 				if chunk_end and not chunk_start:
 					_end = buf_size
 					_start = _end - chunk_end
 
 				aligned_reader = aligned_buf_read(buf, _start, _end)
 				while True:
-					data = aligned_reader.read(self.srv_res.cfg['chunk_stream_piece_size'])
+					data = aligned_reader.read(self.srv_res.cfg['buffers']['bufstream_chunk_len'])
 					if not data:
 						break
 					stream.send(data)
 
-		self.request.terminate()
 
 
 
 
 
 class cl_request:
 	def __init__(self, cl_con, cl_addr, srv_res):
@@ -409,19 +450,21 @@
 					# conlog('Writing to body buffer:', bytes(data[(idx+1):]))
 					self.body_buf.write(bytes(data[(idx+1):]))
 					self.head_buf.write(bytes(data[:idx]))
 					break
 
 			if double_rn == 2:
 				conlog('Header Buf', self.head_buf.getvalue().decode())
-				# conlog('Body Buf', self.body_buf.getvalue())
 				break
 
 			self.head_buf.write(data)
 
+			if self.head_buf.tell() >= self.srv_res.cfg['buffers']['max_header_len']:
+				self.response.reject(431)
+
 	# Request evaluation has a dedicated function for easier error handling
 	def _eval_request(self):
 		# io = self.srv_res.pylib.io
 		# sys = self.srv_res.pylib.sys
 		urllib = self.srv_res.pylib.urllib
 		Path = self.srv_res.pylib.Path
 
@@ -515,14 +558,18 @@
 				return func(self, self.response, self.response.offered_services, *args)
 
 		# if no match was found - return false
 		return False
 
 
 	def read_body_stream(self):
+		"""
+		(Generator)
+		Progressively read the incoming body of the request
+		"""
 		content_length = int(self.headers['content-length'])
 		read_progress = self.body_buf.seek(0, 2)
 		yield self.body_buf.getvalue()
 		while True:
 			if read_progress >= content_length:
 				break
 			# todo: finetune this value
@@ -564,14 +611,17 @@
 
 
 	# Processed headers
 	# =================
 
 	@property
 	def cookie(self):
+		"""
+		Nicely formatted cookie header
+		"""
 		if self._cookie:
 			return self._cookie
 
 		cookie_data = self.headers.get('cookie')
 		if not cookie_data:
 			return None
 
@@ -605,16 +655,16 @@
 
 		# todo: it's always assumed that range is in bytes
 		ranges = range_data.split('=')[1].split(',')
 
 		self._byterange = []
 		for chunk in ranges:
 			chunk_split = chunk.strip().split('-')
-			rstart = int(chunk_split[0]) if chunk_split[0] else None
-			rend =   int(chunk_split[1]) if chunk_split[1] else None
+			rstart = max(int(chunk_split[0]) - 1, 0) if chunk_split[0] else None
+			rend =   max(int(chunk_split[1]) - 1, 0) if chunk_split[1] else None
 			self._byterange.append(
 				(rstart, rend)
 			)
 
 		return self._byterange
```

### Comparing `jag-panzer-0.1.2/src/jag_panzer/cgi/burn_power.py` & `jag-panzer-0.1.21/src/jag_panzer/cgi/burn_power.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.2/src/jag_panzer/cgi/jag.py` & `jag-panzer-0.1.21/src/jag_panzer/cgi/jag.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.2/src/jag_panzer/cgi/templates/light_httpd/server_prms.conf` & `jag-panzer-0.1.21/src/jag_panzer/cgi/templates/light_httpd/server_prms.conf`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.2/src/jag_panzer/dir_list.py` & `jag-panzer-0.1.21/src/jag_panzer/dir_list.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.2/src/jag_panzer/libs/bs4/__init__.py` & `jag-panzer-0.1.21/src/jag_panzer/libs/bs4/__init__.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.2/src/jag_panzer/libs/bs4/builder/__init__.py` & `jag-panzer-0.1.21/src/jag_panzer/libs/bs4/builder/__init__.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.2/src/jag_panzer/libs/bs4/builder/_html5lib.py` & `jag-panzer-0.1.21/src/jag_panzer/libs/bs4/builder/_html5lib.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.2/src/jag_panzer/libs/bs4/builder/_htmlparser.py` & `jag-panzer-0.1.21/src/jag_panzer/libs/bs4/builder/_htmlparser.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.2/src/jag_panzer/libs/bs4/builder/_lxml.py` & `jag-panzer-0.1.21/src/jag_panzer/libs/bs4/builder/_lxml.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.2/src/jag_panzer/libs/bs4/css.py` & `jag-panzer-0.1.21/src/jag_panzer/libs/bs4/css.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.2/src/jag_panzer/libs/bs4/dammit.py` & `jag-panzer-0.1.21/src/jag_panzer/libs/bs4/dammit.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.2/src/jag_panzer/libs/bs4/diagnose.py` & `jag-panzer-0.1.21/src/jag_panzer/libs/bs4/diagnose.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.2/src/jag_panzer/libs/bs4/element.py` & `jag-panzer-0.1.21/src/jag_panzer/libs/bs4/element.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.2/src/jag_panzer/libs/bs4/formatter.py` & `jag-panzer-0.1.21/src/jag_panzer/libs/bs4/formatter.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.2/src/jag_panzer/libs/bs4/tests/__init__.py` & `jag-panzer-0.1.21/src/jag_panzer/libs/bs4/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.2/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-5167584867909632.testcase` & `jag-panzer-0.1.21/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-5167584867909632.testcase`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.2/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-5984173902397440.testcase` & `jag-panzer-0.1.21/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-5984173902397440.testcase`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.2/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-6124268085182464.testcase` & `jag-panzer-0.1.21/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-6124268085182464.testcase`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.2/src/jag_panzer/libs/bs4/tests/fuzz/crash-0d306a50c8ed8bcd0785b67000fcd5dea1d33f08.testcase` & `jag-panzer-0.1.21/src/jag_panzer/libs/bs4/tests/fuzz/crash-0d306a50c8ed8bcd0785b67000fcd5dea1d33f08.testcase`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.2/src/jag_panzer/libs/bs4/tests/test_builder.py` & `jag-panzer-0.1.21/src/jag_panzer/libs/bs4/tests/test_builder.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.2/src/jag_panzer/libs/bs4/tests/test_builder_registry.py` & `jag-panzer-0.1.21/src/jag_panzer/libs/bs4/tests/test_builder_registry.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.2/src/jag_panzer/libs/bs4/tests/test_css.py` & `jag-panzer-0.1.21/src/jag_panzer/libs/bs4/tests/test_css.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.2/src/jag_panzer/libs/bs4/tests/test_dammit.py` & `jag-panzer-0.1.21/src/jag_panzer/libs/bs4/tests/test_dammit.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.2/src/jag_panzer/libs/bs4/tests/test_docs.py` & `jag-panzer-0.1.21/src/jag_panzer/libs/bs4/tests/test_docs.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.2/src/jag_panzer/libs/bs4/tests/test_element.py` & `jag-panzer-0.1.21/src/jag_panzer/libs/bs4/tests/test_element.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.2/src/jag_panzer/libs/bs4/tests/test_formatter.py` & `jag-panzer-0.1.21/src/jag_panzer/libs/bs4/tests/test_formatter.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.2/src/jag_panzer/libs/bs4/tests/test_fuzz.py` & `jag-panzer-0.1.21/src/jag_panzer/libs/bs4/tests/test_fuzz.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.2/src/jag_panzer/libs/bs4/tests/test_html5lib.py` & `jag-panzer-0.1.21/src/jag_panzer/libs/bs4/tests/test_html5lib.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.2/src/jag_panzer/libs/bs4/tests/test_htmlparser.py` & `jag-panzer-0.1.21/src/jag_panzer/libs/bs4/tests/test_htmlparser.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.2/src/jag_panzer/libs/bs4/tests/test_lxml.py` & `jag-panzer-0.1.21/src/jag_panzer/libs/bs4/tests/test_lxml.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.2/src/jag_panzer/libs/bs4/tests/test_navigablestring.py` & `jag-panzer-0.1.21/src/jag_panzer/libs/bs4/tests/test_navigablestring.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.2/src/jag_panzer/libs/bs4/tests/test_pageelement.py` & `jag-panzer-0.1.21/src/jag_panzer/libs/bs4/tests/test_pageelement.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.2/src/jag_panzer/libs/bs4/tests/test_soup.py` & `jag-panzer-0.1.21/src/jag_panzer/libs/bs4/tests/test_soup.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.2/src/jag_panzer/libs/bs4/tests/test_tag.py` & `jag-panzer-0.1.21/src/jag_panzer/libs/bs4/tests/test_tag.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.2/src/jag_panzer/libs/bs4/tests/test_tree.py` & `jag-panzer-0.1.21/src/jag_panzer/libs/bs4/tests/test_tree.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.2/src/jag_panzer/libs/soupsieve/__init__.py` & `jag-panzer-0.1.21/src/jag_panzer/libs/soupsieve/__init__.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.2/src/jag_panzer/libs/soupsieve/__meta__.py` & `jag-panzer-0.1.21/src/jag_panzer/libs/soupsieve/__meta__.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.2/src/jag_panzer/libs/soupsieve/css_match.py` & `jag-panzer-0.1.21/src/jag_panzer/libs/soupsieve/css_match.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.2/src/jag_panzer/libs/soupsieve/css_parser.py` & `jag-panzer-0.1.21/src/jag_panzer/libs/soupsieve/css_parser.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.2/src/jag_panzer/libs/soupsieve/css_types.py` & `jag-panzer-0.1.21/src/jag_panzer/libs/soupsieve/css_types.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.2/src/jag_panzer/libs/soupsieve/pretty.py` & `jag-panzer-0.1.21/src/jag_panzer/libs/soupsieve/pretty.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.2/src/jag_panzer/libs/soupsieve/util.py` & `jag-panzer-0.1.21/src/jag_panzer/libs/soupsieve/util.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.2/src/jag_panzer/libs/yattag/__init__.py` & `jag-panzer-0.1.21/src/jag_panzer/libs/yattag/__init__.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.2/src/jag_panzer/libs/yattag/doc.py` & `jag-panzer-0.1.21/src/jag_panzer/libs/yattag/doc.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.2/src/jag_panzer/libs/yattag/indentation.py` & `jag-panzer-0.1.21/src/jag_panzer/libs/yattag/indentation.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.2/src/jag_panzer/libs/yattag/simpledoc.py` & `jag-panzer-0.1.21/src/jag_panzer/libs/yattag/simpledoc.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.2/src/jag_panzer/mimes/mime_types_base.py` & `jag-panzer-0.1.21/src/jag_panzer/mimes/mime_types_base.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.2/src/jag_panzer/response_codes.py` & `jag-panzer-0.1.21/src/jag_panzer/response_codes.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.2/src/jag_panzer/server.py` & `jag-panzer-0.1.21/src/jag_panzer/server.py`

 * *Files 6% similar despite different names*

```diff
@@ -109,15 +109,18 @@
 
 		# HTTP response codes
 		self.response_codes = _rcodes
 
 		# Reject document precache
 		self.reject_precache = (self.sysroot / 'assets' / 'reject.html').read_bytes()
 
+
+		#
 		# Base config
+		#
 		self.cfg = {
 			# Port to run the server on
 			'port': 0,
 
 			# Document root (where index.html is)
 			'doc_root': None,
 
@@ -128,34 +131,36 @@
 			# Could possibly be treated as bootleg anti-ddos/spam
 			'max_connections': 0,
 
 			# The name of the html file to serve when request path is '/'
 			'root_index': None,
 			'enable_indexes': True,
 			'index_names': ['index.html'],
-
-			# The size of a single chunk when streaming content in HTTP chunks
-			'chunk_stream_piece_size': (1024*1024)*10,
 		} | config
 
 		self.doc_root = Path(self.cfg['doc_root'])
 
+
+		#
 		# Directory Listing
+		# 
 		self.cfg['dir_listing'] = {
 			'enabled': True,
 			'dark_theme': False,
 		} | (config.get('dir_listing') or {})
 
 		if self.cfg['dir_listing']['enabled']:
 			from dir_list import dirlist
 			self.list_dir = dirlist(self)
 
+
+		# 
 		# Advanced CDN serving
+		# 
 		self.cfg['static_cdn'] = {
-			'max_buffered_size': (1024*1024)*10,
 			# Path to the static CDN
 			# can point anywhere
 			'path': None,
 			# Relieve the filesystem stress by precaching items inside this folder
 			# only useful if folder contains a big amount of small files
 			'precache': True,
 			# An array of paths relative to the root cdn path
@@ -171,14 +176,33 @@
 		self.cdn_path = None
 		self.cdn_cache = {}
 
 		if self.cfg['static_cdn']['path']:
 			self.cdn_path = Path(self.cfg['static_cdn']['path'])
 			self.precache_cdn()
 
+
+		# 
+		# Buffer sizes
+		# 
+		self.cfg['buffers'] = {
+			# Max file size when serving a file through built-in server services
+			# Default to 8mb
+			'max_file_len': (1024**2)*8,
+
+			# Max size of the header buffer
+			# Default to 512kb
+			'max_header_len': 1024*512,
+
+			# Default size of a single chunk when streaming buffers
+			# Default to 8mb
+			'bufstream_chunk_len': (1024**2)*8,
+		} | (config.get('buffers') or {})
+
+
 	def precache_cdn(self):
 		for file in self.cdn_path.rglob(self.cfg['static_cdn']['pattern'] or '*'):
 			self.cdn_cache[file.relative_to(self.cdn_path).as_posix()] = \
 				io.BytesIO(file.read_bytes())
 
 		print(
 			_server_proc,
```

### Comparing `jag-panzer-0.1.2/src/jag_panzer.egg-info/PKG-INFO` & `jag-panzer-0.1.21/src/jag_panzer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jag-panzer
-Version: 0.1.2
+Version: 0.1.21
 Summary: Simple HTTP server allowing pure python workflow
 Home-page: https://github.com/MrKleiner/jag
 Author: Mr.Kleiner
 Author-email: megaadrenaline1055@gmail.com
 Project-URL: Bug Tracker, https://github.com/MrKleiner/jag/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `jag-panzer-0.1.2/src/jag_panzer.egg-info/SOURCES.txt` & `jag-panzer-0.1.21/src/jag_panzer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

