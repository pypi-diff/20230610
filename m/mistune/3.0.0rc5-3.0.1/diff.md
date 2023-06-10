# Comparing `tmp/mistune-3.0.0rc5.tar.gz` & `tmp/mistune-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mistune-3.0.0rc5.tar", last modified: Wed Mar 22 13:03:09 2023, max compression
+gzip compressed data, was "mistune-3.0.1.tar", last modified: Fri Jun  9 23:56:47 2023, max compression
```

## Comparing `mistune-3.0.0rc5.tar` & `mistune-3.0.1.tar`

### file list

```diff
@@ -1,60 +1,138 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:03:09.468805 mistune-3.0.0rc5/
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-03-22 13:03:00.000000 mistune-3.0.0rc5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3253 2023-03-22 13:03:09.468805 mistune-3.0.0rc5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-03-22 13:03:00.000000 mistune-3.0.0rc5/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-03-22 13:03:00.000000 mistune-3.0.0rc5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-22 13:03:09.468805 mistune-3.0.0rc5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-03-22 13:03:00.000000 mistune-3.0.0rc5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:03:09.460805 mistune-3.0.0rc5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:03:09.464805 mistune-3.0.0rc5/src/mistune/
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-03-22 13:03:00.000000 mistune-3.0.0rc5/src/mistune/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-03-22 13:03:00.000000 mistune-3.0.0rc5/src/mistune/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16017 2023-03-22 13:03:00.000000 mistune-3.0.0rc5/src/mistune/block_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     5895 2023-03-22 13:03:00.000000 mistune-3.0.0rc5/src/mistune/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:03:09.464805 mistune-3.0.0rc5/src/mistune/directives/
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-03-22 13:03:00.000000 mistune-3.0.0rc5/src/mistune/directives/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-03-22 13:03:00.000000 mistune-3.0.0rc5/src/mistune/directives/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4354 2023-03-22 13:03:00.000000 mistune-3.0.0rc5/src/mistune/directives/_fenced.py
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-03-22 13:03:00.000000 mistune-3.0.0rc5/src/mistune/directives/_rst.py
--rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-03-22 13:03:00.000000 mistune-3.0.0rc5/src/mistune/directives/admonition.py
--rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-03-22 13:03:00.000000 mistune-3.0.0rc5/src/mistune/directives/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-03-22 13:03:00.000000 mistune-3.0.0rc5/src/mistune/directives/include.py
--rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-03-22 13:03:00.000000 mistune-3.0.0rc5/src/mistune/directives/toc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-03-22 13:03:00.000000 mistune-3.0.0rc5/src/mistune/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    12036 2023-03-22 13:03:00.000000 mistune-3.0.0rc5/src/mistune/inline_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     7112 2023-03-22 13:03:00.000000 mistune-3.0.0rc5/src/mistune/list_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-03-22 13:03:00.000000 mistune-3.0.0rc5/src/mistune/markdown.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:03:09.464805 mistune-3.0.0rc5/src/mistune/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-03-22 13:03:00.000000 mistune-3.0.0rc5/src/mistune/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-03-22 13:03:00.000000 mistune-3.0.0rc5/src/mistune/plugins/abbr.py
--rw-r--r--   0 runner    (1001) docker     (123)     3459 2023-03-22 13:03:00.000000 mistune-3.0.0rc5/src/mistune/plugins/def_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     4432 2023-03-22 13:03:00.000000 mistune-3.0.0rc5/src/mistune/plugins/footnotes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4562 2023-03-22 13:03:00.000000 mistune-3.0.0rc5/src/mistune/plugins/formatting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-03-22 13:03:00.000000 mistune-3.0.0rc5/src/mistune/plugins/math.py
--rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-03-22 13:03:00.000000 mistune-3.0.0rc5/src/mistune/plugins/ruby.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-03-22 13:03:00.000000 mistune-3.0.0rc5/src/mistune/plugins/speedup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-03-22 13:03:00.000000 mistune-3.0.0rc5/src/mistune/plugins/spoiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4990 2023-03-22 13:03:00.000000 mistune-3.0.0rc5/src/mistune/plugins/table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-03-22 13:03:00.000000 mistune-3.0.0rc5/src/mistune/plugins/task_lists.py
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-03-22 13:03:00.000000 mistune-3.0.0rc5/src/mistune/plugins/url.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:03:09.464805 mistune-3.0.0rc5/src/mistune/renderers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 13:03:00.000000 mistune-3.0.0rc5/src/mistune/renderers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-03-22 13:03:00.000000 mistune-3.0.0rc5/src/mistune/renderers/_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     4569 2023-03-22 13:03:00.000000 mistune-3.0.0rc5/src/mistune/renderers/html.py
--rw-r--r--   0 runner    (1001) docker     (123)     4685 2023-03-22 13:03:00.000000 mistune-3.0.0rc5/src/mistune/renderers/markdown.py
--rw-r--r--   0 runner    (1001) docker     (123)     5266 2023-03-22 13:03:00.000000 mistune-3.0.0rc5/src/mistune/renderers/rst.py
--rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-03-22 13:03:00.000000 mistune-3.0.0rc5/src/mistune/toc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-03-22 13:03:00.000000 mistune-3.0.0rc5/src/mistune/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:03:09.464805 mistune-3.0.0rc5/src/mistune.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3253 2023-03-22 13:03:09.000000 mistune-3.0.0rc5/src/mistune.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-03-22 13:03:09.000000 mistune-3.0.0rc5/src/mistune.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-22 13:03:09.000000 mistune-3.0.0rc5/src/mistune.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-22 13:03:09.000000 mistune-3.0.0rc5/src/mistune.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:03:09.468805 mistune-3.0.0rc5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-03-22 13:03:00.000000 mistune-3.0.0rc5/tests/test_commonmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-03-22 13:03:00.000000 mistune-3.0.0rc5/tests/test_directives.py
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-03-22 13:03:00.000000 mistune-3.0.0rc5/tests/test_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-03-22 13:03:00.000000 mistune-3.0.0rc5/tests/test_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-03-22 13:03:00.000000 mistune-3.0.0rc5/tests/test_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-03-22 13:03:00.000000 mistune-3.0.0rc5/tests/test_renderers.py
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-03-22 13:03:00.000000 mistune-3.0.0rc5/tests/test_syntax.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:56:47.708738 mistune-3.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-06-09 23:56:38.000000 mistune-3.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-09 23:56:38.000000 mistune-3.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-06-09 23:56:47.708738 mistune-3.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-09 23:56:38.000000 mistune-3.0.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:56:47.692738 mistune-3.0.1/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-06-09 23:56:38.000000 mistune-3.0.1/benchmark/bench.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:56:47.696738 mistune-3.0.1/benchmark/cases/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-09 23:56:38.000000 mistune-3.0.1/benchmark/cases/auto_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-09 23:56:38.000000 mistune-3.0.1/benchmark/cases/axt.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 23:56:38.000000 mistune-3.0.1/benchmark/cases/blockcode.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-09 23:56:38.000000 mistune-3.0.1/benchmark/cases/blockhtml.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-09 23:56:38.000000 mistune-3.0.1/benchmark/cases/blockquote.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-09 23:56:38.000000 mistune-3.0.1/benchmark/cases/emphasis.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-09 23:56:38.000000 mistune-3.0.1/benchmark/cases/fenced.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-09 23:56:38.000000 mistune-3.0.1/benchmark/cases/insane_ol.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-06-09 23:56:38.000000 mistune-3.0.1/benchmark/cases/insane_ul.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-09 23:56:38.000000 mistune-3.0.1/benchmark/cases/normal_ol.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-09 23:56:38.000000 mistune-3.0.1/benchmark/cases/normal_ul.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    15279 2023-06-09 23:56:38.000000 mistune-3.0.1/benchmark/cases/paragraph.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-09 23:56:38.000000 mistune-3.0.1/benchmark/cases/ref_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-09 23:56:38.000000 mistune-3.0.1/benchmark/cases/setext.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-09 23:56:38.000000 mistune-3.0.1/benchmark/cases/std_links.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:56:47.696738 mistune-3.0.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-09 23:56:38.000000 mistune-3.0.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:56:47.696738 mistune-3.0.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-06-09 23:56:38.000000 mistune-3.0.1/docs/_static/dark-icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-06-09 23:56:38.000000 mistune-3.0.1/docs/_static/light-icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     9944 2023-06-09 23:56:38.000000 mistune-3.0.1/docs/_static/logo-black.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     9946 2023-06-09 23:56:38.000000 mistune-3.0.1/docs/_static/logo-white.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:56:47.692738 mistune-3.0.1/docs/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:56:47.696738 mistune-3.0.1/docs/_templates/partials/
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-09 23:56:38.000000 mistune-3.0.1/docs/_templates/partials/sidebar-links.html
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-09 23:56:38.000000 mistune-3.0.1/docs/_templates/partials/webfonts.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4933 2023-06-09 23:56:38.000000 mistune-3.0.1/docs/advanced.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-06-09 23:56:38.000000 mistune-3.0.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-06-09 23:56:38.000000 mistune-3.0.1/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-06-09 23:56:38.000000 mistune-3.0.1/docs/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-09 23:56:38.000000 mistune-3.0.1/docs/community.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-06-09 23:56:38.000000 mistune-3.0.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-06-09 23:56:38.000000 mistune-3.0.1/docs/directives.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-06-09 23:56:38.000000 mistune-3.0.1/docs/guide.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-06-09 23:56:38.000000 mistune-3.0.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-09 23:56:38.000000 mistune-3.0.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)    11318 2023-06-09 23:56:38.000000 mistune-3.0.1/docs/plugins.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-06-09 23:56:38.000000 mistune-3.0.1/docs/renderers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-06-09 23:56:38.000000 mistune-3.0.1/docs/upgrade.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-06-09 23:56:38.000000 mistune-3.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 23:56:47.708738 mistune-3.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-09 23:56:38.000000 mistune-3.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:56:47.692738 mistune-3.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:56:47.700738 mistune-3.0.1/src/mistune/
+-rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-06-09 23:56:38.000000 mistune-3.0.1/src/mistune/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-06-09 23:56:38.000000 mistune-3.0.1/src/mistune/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15988 2023-06-09 23:56:38.000000 mistune-3.0.1/src/mistune/block_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6034 2023-06-09 23:56:38.000000 mistune-3.0.1/src/mistune/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:56:47.700738 mistune-3.0.1/src/mistune/directives/
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-06-09 23:56:38.000000 mistune-3.0.1/src/mistune/directives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-06-09 23:56:38.000000 mistune-3.0.1/src/mistune/directives/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4354 2023-06-09 23:56:38.000000 mistune-3.0.1/src/mistune/directives/_fenced.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-06-09 23:56:38.000000 mistune-3.0.1/src/mistune/directives/_rst.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-06-09 23:56:38.000000 mistune-3.0.1/src/mistune/directives/admonition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-06-09 23:56:38.000000 mistune-3.0.1/src/mistune/directives/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-06-09 23:56:38.000000 mistune-3.0.1/src/mistune/directives/include.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-06-09 23:56:38.000000 mistune-3.0.1/src/mistune/directives/toc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-06-09 23:56:38.000000 mistune-3.0.1/src/mistune/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12015 2023-06-09 23:56:38.000000 mistune-3.0.1/src/mistune/inline_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7112 2023-06-09 23:56:38.000000 mistune-3.0.1/src/mistune/list_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-06-09 23:56:38.000000 mistune-3.0.1/src/mistune/markdown.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:56:47.700738 mistune-3.0.1/src/mistune/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-06-09 23:56:38.000000 mistune-3.0.1/src/mistune/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-06-09 23:56:38.000000 mistune-3.0.1/src/mistune/plugins/abbr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3459 2023-06-09 23:56:38.000000 mistune-3.0.1/src/mistune/plugins/def_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4432 2023-06-09 23:56:38.000000 mistune-3.0.1/src/mistune/plugins/footnotes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4562 2023-06-09 23:56:38.000000 mistune-3.0.1/src/mistune/plugins/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-06-09 23:56:38.000000 mistune-3.0.1/src/mistune/plugins/math.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-06-09 23:56:38.000000 mistune-3.0.1/src/mistune/plugins/ruby.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-09 23:56:38.000000 mistune-3.0.1/src/mistune/plugins/speedup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-06-09 23:56:38.000000 mistune-3.0.1/src/mistune/plugins/spoiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4990 2023-06-09 23:56:38.000000 mistune-3.0.1/src/mistune/plugins/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-06-09 23:56:38.000000 mistune-3.0.1/src/mistune/plugins/task_lists.py
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-06-09 23:56:38.000000 mistune-3.0.1/src/mistune/plugins/url.py
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-09 23:56:38.000000 mistune-3.0.1/src/mistune/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:56:47.700738 mistune-3.0.1/src/mistune/renderers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 23:56:38.000000 mistune-3.0.1/src/mistune/renderers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-06-09 23:56:38.000000 mistune-3.0.1/src/mistune/renderers/_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4577 2023-06-09 23:56:38.000000 mistune-3.0.1/src/mistune/renderers/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4682 2023-06-09 23:56:38.000000 mistune-3.0.1/src/mistune/renderers/markdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5266 2023-06-09 23:56:38.000000 mistune-3.0.1/src/mistune/renderers/rst.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-06-09 23:56:38.000000 mistune-3.0.1/src/mistune/toc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-06-09 23:56:38.000000 mistune-3.0.1/src/mistune/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:56:47.700738 mistune-3.0.1/src/mistune.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-06-09 23:56:47.000000 mistune-3.0.1/src/mistune.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-06-09 23:56:47.000000 mistune-3.0.1/src/mistune.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 23:56:47.000000 mistune-3.0.1/src/mistune.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-09 23:56:47.000000 mistune-3.0.1/src/mistune.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:56:47.704738 mistune-3.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-06-09 23:56:38.000000 mistune-3.0.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:56:47.708738 mistune-3.0.1/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-06-09 23:56:38.000000 mistune-3.0.1/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-06-09 23:56:38.000000 mistune-3.0.1/tests/fixtures/abbr.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   140423 2023-06-09 23:56:38.000000 mistune-3.0.1/tests/fixtures/commonmark.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-06-09 23:56:38.000000 mistune-3.0.1/tests/fixtures/def_list.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-06-09 23:56:38.000000 mistune-3.0.1/tests/fixtures/diff-commonmark.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-06-09 23:56:38.000000 mistune-3.0.1/tests/fixtures/fenced_admonition.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-06-09 23:56:38.000000 mistune-3.0.1/tests/fixtures/fenced_figure.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-06-09 23:56:38.000000 mistune-3.0.1/tests/fixtures/fenced_image.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3656 2023-06-09 23:56:38.000000 mistune-3.0.1/tests/fixtures/fenced_toc.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-06-09 23:56:38.000000 mistune-3.0.1/tests/fixtures/fix-commonmark.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-06-09 23:56:38.000000 mistune-3.0.1/tests/fixtures/footnotes.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-06-09 23:56:38.000000 mistune-3.0.1/tests/fixtures/hook_toc.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:56:47.708738 mistune-3.0.1/tests/fixtures/include/
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-09 23:56:38.000000 mistune-3.0.1/tests/fixtures/include/hello.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-09 23:56:38.000000 mistune-3.0.1/tests/fixtures/include/hello.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-09 23:56:38.000000 mistune-3.0.1/tests/fixtures/include/text.html
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-09 23:56:38.000000 mistune-3.0.1/tests/fixtures/include/text.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-06-09 23:56:38.000000 mistune-3.0.1/tests/fixtures/insert.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-06-09 23:56:38.000000 mistune-3.0.1/tests/fixtures/mark.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-09 23:56:38.000000 mistune-3.0.1/tests/fixtures/math.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-06-09 23:56:38.000000 mistune-3.0.1/tests/fixtures/renderer_markdown.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-06-09 23:56:38.000000 mistune-3.0.1/tests/fixtures/renderer_rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-06-09 23:56:38.000000 mistune-3.0.1/tests/fixtures/rst_admonition.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-06-09 23:56:38.000000 mistune-3.0.1/tests/fixtures/rst_toc.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-06-09 23:56:38.000000 mistune-3.0.1/tests/fixtures/ruby.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-09 23:56:38.000000 mistune-3.0.1/tests/fixtures/spoiler.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-06-09 23:56:38.000000 mistune-3.0.1/tests/fixtures/strikethrough.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-06-09 23:56:38.000000 mistune-3.0.1/tests/fixtures/subscript.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-09 23:56:38.000000 mistune-3.0.1/tests/fixtures/superscript.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-06-09 23:56:38.000000 mistune-3.0.1/tests/fixtures/table.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3104 2023-06-09 23:56:38.000000 mistune-3.0.1/tests/fixtures/task_lists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-09 23:56:38.000000 mistune-3.0.1/tests/fixtures/url.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-06-09 23:56:38.000000 mistune-3.0.1/tests/test_commonmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-06-09 23:56:38.000000 mistune-3.0.1/tests/test_directives.py
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-09 23:56:38.000000 mistune-3.0.1/tests/test_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3699 2023-06-09 23:56:38.000000 mistune-3.0.1/tests/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-06-09 23:56:38.000000 mistune-3.0.1/tests/test_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-09 23:56:38.000000 mistune-3.0.1/tests/test_renderers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-06-09 23:56:38.000000 mistune-3.0.1/tests/test_syntax.py
```

### Comparing `mistune-3.0.0rc5/LICENSE` & `mistune-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mistune-3.0.0rc5/pyproject.toml` & `mistune-3.0.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [project]
 name = "mistune"
 description = "A sane and fast Markdown parser with useful plugins and renderers"
 authors = [{name = "Hsiaoming Yang", email="me@lepture.com"}]
 dependencies = []
-license = {file = "LICENSE"}
+license = {text = "BSD-3-Clause"}
 dynamic = ["version"]
 requires-python = ">=3.7"
 readme = "README.rst"
 classifiers = [
   "Development Status :: 4 - Beta",
   "Environment :: Console",
   "Environment :: Web Environment",
@@ -37,14 +37,17 @@
 
 [tool.setuptools.dynamic]
 version = {attr = "mistune.__version__"}
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
+[tool.setuptools.package-data]
+mistune = ["py.typed"]
+
 [tool.pytest.ini_options]
 pythonpath = ["src", "."]
 testpaths = ["tests"]
 filterwarnings = ["error"]
 
 [tool.coverage.run]
 branch = true
```

### Comparing `mistune-3.0.0rc5/src/mistune/__init__.py` & `mistune-3.0.1/src/mistune/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from .block_parser import BlockParser
 from .inline_parser import InlineParser
 from .renderers.html import HTMLRenderer
 from .util import escape, escape_url, safe_entity, unikey
 from .plugins import import_plugin
 
 
-def create_markdown(escape=True, hard_wrap=False, renderer='html', plugins=None):
+def create_markdown(escape: bool=True, hard_wrap: bool=False, renderer='html', plugins=None) -> Markdown:
     """Create a Markdown instance based on the given condition.
 
     :param escape: Boolean. If using html renderer, escape html.
     :param hard_wrap: Boolean. Break every new line into ``<br>``.
     :param renderer: renderer instance, default is HTMLRenderer.
     :param plugins: List of plugins.
 
@@ -30,33 +30,39 @@
         markdown = create_markdown(
             escape=False,
             hard_wrap=True,
         )
         # re-use markdown function
         markdown('.... your text ...')
     """
-    if renderer == 'html':
+    if renderer == 'ast':
+        # explicit and more similar to 2.x's API
+        renderer = None
+    elif renderer == 'html':
         renderer = HTMLRenderer(escape=escape)
 
     inline = InlineParser(hard_wrap=hard_wrap)
     if plugins is not None:
         plugins = [import_plugin(n) for n in plugins]
     return Markdown(renderer=renderer, inline=inline, plugins=plugins)
 
 
-html = create_markdown(
+html: Markdown = create_markdown(
     escape=False,
     plugins=['strikethrough', 'footnotes', 'table', 'speedup']
 )
 
 
 __cached_parsers = {}
 
 
-def markdown(text, escape=True, renderer='html', plugins=None):
+def markdown(text, escape=True, renderer='html', plugins=None) -> str:
+    if renderer == 'ast':
+        # explicit and more similar to 2.x's API
+        renderer = None
     key = (escape, renderer, plugins)
     if key in __cached_parsers:
         return __cached_parsers[key](text)
 
     md = create_markdown(escape=escape, renderer=renderer, plugins=plugins)
     # improve the speed for markdown parser creation
     __cached_parsers[key] = md
@@ -67,9 +73,9 @@
     'Markdown', 'HTMLRenderer',
     'BlockParser', 'BlockState', 'BaseRenderer',
     'InlineParser', 'InlineState',
     'escape', 'escape_url', 'safe_entity', 'unikey',
     'html', 'create_markdown', 'markdown',
 ]
 
-__version__ = '3.0.0rc5'
+__version__ = '3.0.1'
 __homepage__ = 'https://mistune.lepture.com/'
```

### Comparing `mistune-3.0.0rc5/src/mistune/__main__.py` & `mistune-3.0.1/src/mistune/__main__.py`

 * *Files identical despite different names*

### Comparing `mistune-3.0.0rc5/src/mistune/block_parser.py` & `mistune-3.0.1/src/mistune/block_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import re
-from typing import Optional, List, Tuple
+from typing import Optional, List, Tuple, Match
 from .util import (
     unikey,
     escape_url,
     expand_tab,
     expand_leading_tab,
 )
 from .core import Parser, BlockState
@@ -105,40 +105,40 @@
         self.list_rules = list_rules
         self.max_nested_level = max_nested_level
         # register default parse methods
         self._methods = {
             name: getattr(self, 'parse_' + name) for name in self.SPECIFICATION
         }
 
-    def parse_blank_line(self, m: re.Match, state: BlockState) -> int:
+    def parse_blank_line(self, m: Match, state: BlockState) -> int:
         """Parse token for blank lines."""
         state.append_token({'type': 'blank_line'})
         return m.end()
 
-    def parse_thematic_break(self, m: re.Match, state: BlockState) -> int:
+    def parse_thematic_break(self, m: Match, state: BlockState) -> int:
         """Parse token for thematic break, e.g. ``<hr>`` tag in HTML."""
         state.append_token({'type': 'thematic_break'})
         # $ does not count '\n'
         return m.end() + 1
 
-    def parse_indent_code(self, m: re.Match, state: BlockState) -> int:
+    def parse_indent_code(self, m: Match, state: BlockState) -> int:
         """Parse token for code block which is indented by 4 spaces."""
         # it is a part of the paragraph
         end_pos = state.append_paragraph()
         if end_pos:
             return end_pos
 
         code = m.group(0)
         code = expand_leading_tab(code)
         code = _INDENT_CODE_TRIM.sub('', code)
         code = code.strip('\n')
         state.append_token({'type': 'block_code', 'raw': code, 'style': 'indent'})
         return m.end()
 
-    def parse_fenced_code(self, m: re.Match, state: BlockState) -> Optional[int]:
+    def parse_fenced_code(self, m: Match, state: BlockState) -> Optional[int]:
         """Parse token for fenced code block. A fenced code block is started with
         3 or more backtick(`) or tilde(~).
 
         An example of a fenced code block:
 
         .. code-block:: markdown
 
@@ -178,28 +178,28 @@
         if info:
             info = unescape_char(info)
             token['attrs'] = {'info': info.strip()}
 
         state.append_token(token)
         return end_pos
 
-    def parse_axt_heading(self, m: re.Match, state: BlockState) -> int:
+    def parse_axt_heading(self, m: Match, state: BlockState) -> int:
         """Parse token for AXT heading. An AXT heading is started with 1 to 6
         symbol of ``#``."""
         level = len(m.group('axt_1'))
         text = m.group('axt_2').strip()
         # remove last #
         if text:
             text = _AXT_HEADING_TRIM.sub('', text)
 
         token = {'type': 'heading', 'text': text, 'attrs': {'level': level}, 'style': 'axt'}
         state.append_token(token)
         return m.end() + 1
 
-    def parse_setex_heading(self, m: re.Match, state: BlockState) -> Optional[int]:
+    def parse_setex_heading(self, m: Match, state: BlockState) -> Optional[int]:
         """Parse token for setex style heading. A setex heading syntax looks like:
 
         .. code-block:: markdown
 
             H1 title
             ========
         """
@@ -212,15 +212,15 @@
             return m.end() + 1
 
         sc = self.compile_sc(['thematic_break', 'list'])
         m = sc.match(state.src, state.cursor)
         if m:
             return self.parse_method(m, state)
 
-    def parse_ref_link(self, m: re.Match, state: BlockState) -> Optional[int]:
+    def parse_ref_link(self, m: Match, state: BlockState) -> Optional[int]:
         """Parse link references and save the link information into ``state.env``.
 
         Here is an example of a link reference:
 
         .. code-block:: markdown
 
             a [link][example]
@@ -278,15 +278,15 @@
             href = unescape_char(href)
             data = {'url': escape_url(href), 'label': label}
             if title:
                 data['title'] = title
             state.env['ref_links'][key] = data
         return end_pos
 
-    def extract_block_quote(self, m: re.Match, state: BlockState) -> Tuple[str, int]:
+    def extract_block_quote(self, m: Match, state: BlockState) -> Tuple[str, int]:
         """Extract text and cursor end position of a block quote."""
 
         # cleanup at first to detect if it is code block
         text = m.group('quote_1') + '\n'
         text = expand_leading_tab(text, 3)
         text = _BLOCK_QUOTE_TRIM.sub('', text)
 
@@ -345,15 +345,15 @@
                 text += line
                 state.cursor = pos
 
         # according to CommonMark Example 6, the second tab should be
         # treated as 4 spaces
         return expand_tab(text), end_pos
 
-    def parse_block_quote(self, m: re.Match, state: BlockState) -> int:
+    def parse_block_quote(self, m: Match, state: BlockState) -> int:
         """Parse token for block quote. Here is an example of the syntax:
 
         .. code-block:: markdown
 
             > a block quote starts
             > with right arrows
         """
@@ -370,22 +370,22 @@
         token = {'type': 'block_quote', 'children': child.tokens}
         if end_pos:
             state.prepend_token(token)
             return end_pos
         state.append_token(token)
         return state.cursor
 
-    def parse_list(self, m: re.Match, state: BlockState) -> int:
+    def parse_list(self, m: Match, state: BlockState) -> int:
         """Parse tokens for ordered and unordered list."""
         return parse_list(self, m, state)
 
-    def parse_block_html(self, m: re.Match, state: BlockState) -> Optional[int]:
+    def parse_block_html(self, m: Match, state: BlockState) -> Optional[int]:
         return self.parse_raw_html(m, state)
 
-    def parse_raw_html(self, m: re.Match, state: BlockState) -> Optional[int]:
+    def parse_raw_html(self, m: Match, state: BlockState) -> Optional[int]:
         marker = m.group(0).strip()
 
         # rule 2
         if marker == '<!--':
             return _parse_html_to_end(state, '-->', m.end())
 
         # rule 3
```

### Comparing `mistune-3.0.0rc5/src/mistune/core.py` & `mistune-3.0.1/src/mistune/core.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import re
+from typing import Dict, Any
 
 _LINE_END = re.compile(r'\n|$')
 
 
 class BlockState:
     """The state to save block parser's cursor and tokens."""
     def __init__(self, parent=None):
@@ -19,43 +20,43 @@
 
         # for saving def references
         if parent:
             self.env = parent.env
         else:
             self.env = {'ref_links': {}}
 
-    def child_state(self, src):
+    def child_state(self, src: str):
         child = self.__class__(self)
         child.process(src)
         return child
 
-    def process(self, src):
+    def process(self, src: str):
         self.src = src
         self.cursor_max = len(src)
 
     def find_line_end(self):
         m = _LINE_END.search(self.src, self.cursor)
         return m.end()
 
-    def get_text(self, end_pos):
+    def get_text(self, end_pos: int):
         return self.src[self.cursor:end_pos]
 
     def last_token(self):
         if self.tokens:
             return self.tokens[-1]
 
-    def prepend_token(self, token):
+    def prepend_token(self, token: Dict[str, Any]):
         """Insert token before the last token."""
         self.tokens.insert(len(self.tokens) - 1, token)
 
-    def append_token(self, token):
+    def append_token(self, token: Dict[str, Any]):
         """Add token to the end of token list."""
         self.tokens.append(token)
 
-    def add_paragraph(self, text):
+    def add_paragraph(self, text: str):
         last_token = self.last_token()
         if last_token and last_token['type'] == 'paragraph':
             last_token['text'] += text
         else:
             self.tokens.append({'type': 'paragraph', 'text': text})
 
     def append_paragraph(self):
@@ -72,28 +73,28 @@
             d += 1
             parent = parent.parent
         return d
 
 
 class InlineState:
     """The state to save inline parser's tokens."""
-    def __init__(self, env):
+    def __init__(self, env: Dict[str, Any]):
         self.env = env
         self.src = ''
         self.tokens = []
         self.in_image = False
         self.in_link = False
         self.in_emphasis = False
         self.in_strong = False
 
-    def prepend_token(self, token):
+    def prepend_token(self, token: Dict[str, Any]):
         """Insert token before the last token."""
         self.tokens.insert(len(self.tokens) - 1, token)
 
-    def append_token(self, token):
+    def append_token(self, token: Dict[str, Any]):
         """Add token to the end of token list."""
         self.tokens.append(token)
 
     def copy(self):
         """Create a copy of current state."""
         state = self.__class__(self.env)
         state.in_image = self.in_image
@@ -129,15 +130,15 @@
             return sc
 
         regex = '|'.join(r'(?P<%s>%s)' % (k, self.specification[k]) for k in rules)
         sc = re.compile(regex, self.sc_flag)
         self.__sc[key] = sc
         return sc
 
-    def register(self, name, pattern, func, before=None):
+    def register(self, name: str, pattern, func, before=None):
         """Register a new rule to parse the token. This method is usually used to
         create a new plugin.
 
         :param name: name of the new grammar
         :param pattern: regex pattern in string
         :param func: the parsing function
         :param before: insert this rule before a built-in rule
@@ -169,15 +170,15 @@
 
 class BaseRenderer(object):
     NAME = 'base'
 
     def __init__(self):
         self.__methods = {}
 
-    def register(self, name, method):
+    def register(self, name: str, method):
         """Register a render method for the named token. For example::
 
             def render_wiki(renderer, key, title):
                 return f'<a href="/wiki/{key}">{title}</a>'
 
             renderer.register('wiki', render_wiki)
         """
```

### Comparing `mistune-3.0.0rc5/src/mistune/directives/__init__.py` & `mistune-3.0.1/src/mistune/directives/__init__.py`

 * *Files identical despite different names*

### Comparing `mistune-3.0.0rc5/src/mistune/directives/_base.py` & `mistune-3.0.1/src/mistune/directives/_base.py`

 * *Files identical despite different names*

### Comparing `mistune-3.0.0rc5/src/mistune/directives/_fenced.py` & `mistune-3.0.1/src/mistune/directives/_fenced.py`

 * *Files identical despite different names*

### Comparing `mistune-3.0.0rc5/src/mistune/directives/_rst.py` & `mistune-3.0.1/src/mistune/directives/_rst.py`

 * *Files identical despite different names*

### Comparing `mistune-3.0.0rc5/src/mistune/directives/admonition.py` & `mistune-3.0.1/src/mistune/directives/admonition.py`

 * *Files identical despite different names*

### Comparing `mistune-3.0.0rc5/src/mistune/directives/image.py` & `mistune-3.0.1/src/mistune/directives/image.py`

 * *Files identical despite different names*

### Comparing `mistune-3.0.0rc5/src/mistune/directives/include.py` & `mistune-3.0.1/src/mistune/directives/include.py`

 * *Files identical despite different names*

### Comparing `mistune-3.0.0rc5/src/mistune/directives/toc.py` & `mistune-3.0.1/src/mistune/directives/toc.py`

 * *Files identical despite different names*

### Comparing `mistune-3.0.0rc5/src/mistune/helpers.py` & `mistune-3.0.1/src/mistune/helpers.py`

 * *Files identical despite different names*

### Comparing `mistune-3.0.0rc5/src/mistune/inline_parser.py` & `mistune-3.0.1/src/mistune/inline_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import re
-from typing import Optional, List, Dict, Any
+from typing import Optional, List, Dict, Any, Match
 from .core import Parser, InlineState
 from .util import (
     escape,
     escape_url,
     unikey,
 )
 from .helpers import (
@@ -89,38 +89,38 @@
         'link',
         'auto_link',
         'auto_email',
         'inline_html',
         'linebreak',
     )
 
-    def __init__(self, hard_wrap=False):
+    def __init__(self, hard_wrap: bool=False):
         super(InlineParser, self).__init__()
 
         self.hard_wrap = hard_wrap
         # lazy add linebreak
         if hard_wrap:
             self.specification['linebreak'] = self.HARD_LINEBREAK
         else:
             self.rules.append('softbreak')
 
         self._methods = {
             name: getattr(self, 'parse_' + name) for name in self.rules
         }
 
-    def parse_escape(self, m: re.Match, state: InlineState) -> int:
+    def parse_escape(self, m: Match, state: InlineState) -> int:
         text = m.group(0)
         text = unescape_char(text)
         state.append_token({
             'type': 'text',
             'raw': text,
         })
         return m.end()
 
-    def parse_link(self, m: re.Match, state: InlineState) -> Optional[int]:
+    def parse_link(self, m: Match, state: InlineState) -> Optional[int]:
         pos = m.end()
 
         marker = m.group(0)
         is_image = marker[0] == '!'
         if is_image and state.in_image:
             state.append_token({'type': 'text', 'raw': marker})
             return pos
@@ -196,26 +196,26 @@
             token = {
                 'type': 'link',
                 'children': self.render(new_state),
                 'attrs': attrs,
             }
         return token
 
-    def parse_auto_link(self, m: re.Match, state: InlineState) -> int:
+    def parse_auto_link(self, m: Match, state: InlineState) -> int:
         text = m.group(0)
         pos = m.end()
         if state.in_link:
             self.process_text(text, state)
             return pos
 
         text = text[1:-1]
         self._add_auto_link(text, text, state)
         return pos
 
-    def parse_auto_email(self, m: re.Match, state: InlineState) -> int:
+    def parse_auto_email(self, m: Match, state: InlineState) -> int:
         text = m.group(0)
         pos = m.end()
         if state.in_link:
             self.process_text(text, state)
             return pos
 
         text = text[1:-1]
@@ -226,15 +226,15 @@
     def _add_auto_link(self, url, text, state):
         state.append_token({
             'type': 'link',
             'children': [{'type': 'text', 'raw': text}],
             'attrs': {'url': escape_url(url)},
         })
 
-    def parse_emphasis(self, m: re.Match, state: InlineState) -> int:
+    def parse_emphasis(self, m: Match, state: InlineState) -> int:
         pos = m.end()
 
         marker = m.group(0)
         mlen = len(marker)
         if mlen == 1 and state.in_emphasis:
             state.append_token({'type': 'text', 'raw': marker})
             return pos
@@ -275,19 +275,19 @@
             }]
             state.append_token({
                 'type': 'emphasis',
                 'children': children,
             })
         return end_pos
 
-    def parse_codespan(self, m: re.Match, state: InlineState) -> int:
+    def parse_codespan(self, m: Match, state: InlineState) -> int:
         marker = m.group(0)
         # require same marker with same length at end
 
-        pattern = re.compile(r'(.*?(?:[^`]))' + marker + r'(?!`)', re.S)
+        pattern = re.compile(r'(.*?[^`])' + marker + r'(?!`)', re.S)
 
         pos = m.end()
         m = pattern.match(state.src, pos)
         if m:
             end_pos = m.end()
             code = m.group(1)
             # Line endings are treated like spaces
@@ -297,23 +297,23 @@
                     code = code[1:-1]
             state.append_token({'type': 'codespan', 'raw': escape(code)})
             return end_pos
         else:
             state.append_token({'type': 'text', 'raw': marker})
             return pos
 
-    def parse_linebreak(self, m: re.Match, state: InlineState) -> int:
+    def parse_linebreak(self, m: Match, state: InlineState) -> int:
         state.append_token({'type': 'linebreak'})
         return m.end()
 
-    def parse_softbreak(self, m: re.Match, state: InlineState) -> int:
+    def parse_softbreak(self, m: Match, state: InlineState) -> int:
         state.append_token({'type': 'softbreak'})
         return m.end()
 
-    def parse_inline_html(self, m: re.Match, state: InlineState) -> int:
+    def parse_inline_html(self, m: Match, state: InlineState) -> int:
         end_pos = m.end()
         html = m.group(0)
         state.append_token({'type': 'inline_html', 'raw': html})
         if html.startswith(('<a ', '<a>', '<A ', '<A>')):
             state.in_link = True
         elif html.startswith(('</a ', '</a>', '</A ', '</A>')):
             state.in_link = False
@@ -347,15 +347,15 @@
         if pos == 0:
             # special case, just pure text
             self.process_text(state.src, state)
         elif pos < len(state.src):
             self.process_text(state.src[pos:], state)
         return state.tokens
 
-    def precedence_scan(self, m: re.Match, state: InlineState, end_pos: int, rules=None):
+    def precedence_scan(self, m: Match, state: InlineState, end_pos: int, rules=None):
         if rules is None:
             rules = ['codespan', 'link', 'prec_auto_link', 'prec_inline_html']
 
         mark_pos = m.end()
         sc = self.compile_sc(rules)
         m1 = sc.search(state.src, mark_pos, end_pos)
         if not m1:
```

### Comparing `mistune-3.0.0rc5/src/mistune/list_parser.py` & `mistune-3.0.1/src/mistune/list_parser.py`

 * *Files identical despite different names*

### Comparing `mistune-3.0.0rc5/src/mistune/markdown.py` & `mistune-3.0.1/src/mistune/markdown.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,24 +14,27 @@
         md('hello **world**')
 
     :param renderer: a renderer to convert parsed tokens
     :param block: block level syntax parser
     :param inline: inline level syntax parser
     :param plugins: mistune plugins to use
     """
-    def __init__(self, renderer=None, block=None, inline=None, plugins=None):
+    def __init__(self, renderer=None,
+                 block: Optional[BlockParser]=None,
+                 inline: Optional[InlineParser]=None,
+                 plugins=None):
         if block is None:
             block = BlockParser()
 
         if inline is None:
             inline = InlineParser()
 
         self.renderer = renderer
-        self.block = block
-        self.inline = inline
+        self.block: BlockParser = block
+        self.inline: InlineParser = inline
         self.before_parse_hooks = []
         self.before_render_hooks = []
         self.after_render_hooks = []
 
         if plugins:
             for plugin in plugins:
                 plugin(self)
@@ -49,15 +52,16 @@
         for tok in tokens:
             if 'children' in tok:
                 children = self._iter_render(tok['children'], state)
                 tok['children'] = list(children)
             elif 'text' in tok:
                 text = tok.pop('text')
                 # process inline text
-                tok['children'] = self.inline(text.strip(), state.env)
+                # avoid striping emsp or other unicode spaces
+                tok['children'] = self.inline(text.strip(' \r\n\t\f'), state.env)
             yield tok
 
     def parse(self, s: str, state: Optional[BlockState]=None):
         """Parse and convert the given markdown string. If renderer is None,
         the returned **result** will be parsed markdown tokens.
 
         :param s: markdown string
@@ -66,14 +70,16 @@
         """
         if state is None:
             state = self.block.state_cls()
 
         # normalize line separator
         s = s.replace('\r\n', '\n')
         s = s.replace('\r', '\n')
+        if not s.endswith('\n'):
+            s += '\n'
 
         state.process(s)
 
         for hook in self.before_parse_hooks:
             hook(self, state)
 
         self.block.parse(state)
```

### Comparing `mistune-3.0.0rc5/src/mistune/plugins/__init__.py` & `mistune-3.0.1/src/mistune/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `mistune-3.0.0rc5/src/mistune/plugins/abbr.py` & `mistune-3.0.1/src/mistune/plugins/abbr.py`

 * *Files identical despite different names*

### Comparing `mistune-3.0.0rc5/src/mistune/plugins/def_list.py` & `mistune-3.0.1/src/mistune/plugins/def_list.py`

 * *Files identical despite different names*

### Comparing `mistune-3.0.0rc5/src/mistune/plugins/footnotes.py` & `mistune-3.0.1/src/mistune/plugins/footnotes.py`

 * *Files identical despite different names*

### Comparing `mistune-3.0.0rc5/src/mistune/plugins/formatting.py` & `mistune-3.0.1/src/mistune/plugins/formatting.py`

 * *Files identical despite different names*

### Comparing `mistune-3.0.0rc5/src/mistune/plugins/math.py` & `mistune-3.0.1/src/mistune/plugins/math.py`

 * *Files identical despite different names*

### Comparing `mistune-3.0.0rc5/src/mistune/plugins/ruby.py` & `mistune-3.0.1/src/mistune/plugins/ruby.py`

 * *Files identical despite different names*

### Comparing `mistune-3.0.0rc5/src/mistune/plugins/speedup.py` & `mistune-3.0.1/src/mistune/plugins/speedup.py`

 * *Files identical despite different names*

### Comparing `mistune-3.0.0rc5/src/mistune/plugins/spoiler.py` & `mistune-3.0.1/src/mistune/plugins/spoiler.py`

 * *Files identical despite different names*

### Comparing `mistune-3.0.0rc5/src/mistune/plugins/table.py` & `mistune-3.0.1/src/mistune/plugins/table.py`

 * *Files identical despite different names*

### Comparing `mistune-3.0.0rc5/src/mistune/plugins/task_lists.py` & `mistune-3.0.1/src/mistune/plugins/task_lists.py`

 * *Files identical despite different names*

### Comparing `mistune-3.0.0rc5/src/mistune/plugins/url.py` & `mistune-3.0.1/src/mistune/plugins/url.py`

 * *Files identical despite different names*

### Comparing `mistune-3.0.0rc5/src/mistune/renderers/_list.py` & `mistune-3.0.1/src/mistune/renderers/_list.py`

 * *Files identical despite different names*

### Comparing `mistune-3.0.0rc5/src/mistune/renderers/html.py` & `mistune-3.0.1/src/mistune/renderers/html.py`

 * *Files 0% similar despite different names*

```diff
@@ -128,15 +128,15 @@
         return html + '>' + escape_text(code) + '</code></pre>\n'
 
     def block_quote(self, text: str) -> str:
         return '<blockquote>\n' + text + '</blockquote>\n'
 
     def block_html(self, html: str) -> str:
         if self._escape:
-            return '<p>' + escape_text(html) + '</p>\n'
+            return '<p>' + escape_text(html.strip()) + '</p>\n'
         return html + '\n'
 
     def block_error(self, text: str) -> str:
         return '<div class="error"><pre>' + text + '</pre></div>\n'
 
     def list(self, text: str, ordered: bool, **attrs) -> str:
         if ordered:
```

### Comparing `mistune-3.0.0rc5/src/mistune/renderers/markdown.py` & `mistune-3.0.1/src/mistune/renderers/markdown.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import re
 from typing import Dict, Any
 from textwrap import indent
 from ._list import render_list
 from ..core import BaseRenderer, BlockState
 from ..util import strip_end
 
-fenced_re = re.compile(r'^(?:`|~)+', re.M)
+fenced_re = re.compile(r'^[`~]+', re.M)
 
 
 class MarkdownRenderer(BaseRenderer):
     """A renderer to re-format Markdown text."""
     NAME = 'markdown'
 
     def __call__(self, tokens, state: BlockState):
```

### Comparing `mistune-3.0.0rc5/src/mistune/renderers/rst.py` & `mistune-3.0.1/src/mistune/renderers/rst.py`

 * *Files identical despite different names*

### Comparing `mistune-3.0.0rc5/src/mistune/toc.py` & `mistune-3.0.1/src/mistune/toc.py`

 * *Files identical despite different names*

### Comparing `mistune-3.0.0rc5/src/mistune/util.py` & `mistune-3.0.1/src/mistune/util.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,80 +2,80 @@
 from urllib.parse import quote
 from html import _replace_charref
 
 
 _expand_tab_re = re.compile(r'^( {0,3})\t', flags=re.M)
 
 
-def expand_leading_tab(text, width=4):
+def expand_leading_tab(text: str, width=4):
     def repl(m):
         s = m.group(1)
         return s + ' ' * (width - len(s))
     return _expand_tab_re.sub(repl, text)
 
 
-def expand_tab(text, space='    '):
+def expand_tab(text: str, space: str='    '):
     repl = r'\1' + space
     return _expand_tab_re.sub(repl, text)
 
 
-def escape(s, quote=True):
+def escape(s: str, quote: bool=True):
     """Escape characters of ``&<>``. If quote=True, ``"`` will be
     converted to ``&quote;``."""
     s = s.replace("&", "&amp;")
     s = s.replace("<", "&lt;")
     s = s.replace(">", "&gt;")
     if quote:
         s = s.replace('"', "&quot;")
     return s
 
 
-def escape_url(link):
+def escape_url(link: str):
     """Escape URL for safety."""
     safe = (
         ':/?#@'           # gen-delims - '[]' (rfc3986)
         '!$&()*+,;='      # sub-delims - "'" (rfc3986)
         '%'               # leave already-encoded octets alone
     )
     return escape(quote(unescape(link), safe=safe))
 
 
-def safe_entity(s):
+def safe_entity(s: str):
     """Escape characters for safety."""
     return escape(unescape(s))
 
 
-def unikey(s):
+def unikey(s: str):
     """Generate a unique key for links and footnotes."""
     key = ' '.join(s.split()).strip()
     return key.lower().upper()
 
 
 _charref_re = re.compile(
     r'&(#[0-9]{1,7};'
     r'|#[xX][0-9a-fA-F]+;'
     r'|[^\t\n\f <&#;]{1,32};)'
 )
 
 
-def unescape(s):
+def unescape(s: str):
     """
     Copy from `html.unescape`, but `_charref` is different. CommonMark
     does not accept entity references without a trailing semicolon
     """
     if '&' not in s:
         return s
     return _charref_re.sub(_replace_charref, s)
 
 
 _striptags_re = re.compile(r'(<!--.*?-->|<[^>]*>)')
 
 
-def striptags(s):
+def striptags(s: str):
     return _striptags_re.sub('', s)
 
 
 _strip_end_re = re.compile(r'\n\s+$')
 
 
-def strip_end(src):
+def strip_end(src: str):
     return _strip_end_re.sub('\n', src)
```

### Comparing `mistune-3.0.0rc5/tests/test_commonmark.py` & `mistune-3.0.1/tests/test_commonmark.py`

 * *Files identical despite different names*

### Comparing `mistune-3.0.0rc5/tests/test_directives.py` & `mistune-3.0.1/tests/test_directives.py`

 * *Files identical despite different names*

### Comparing `mistune-3.0.0rc5/tests/test_hooks.py` & `mistune-3.0.1/tests/test_hooks.py`

 * *Files identical despite different names*

### Comparing `mistune-3.0.0rc5/tests/test_misc.py` & `mistune-3.0.1/tests/test_misc.py`

 * *Files 9% similar despite different names*

```diff
@@ -38,14 +38,19 @@
         self.assertEqual(result.strip(), expected)
 
     def test_harmful_links(self):
         result = mistune.html('[h](javAscript:alert)')
         expected = '<p><a href="#harmful-link">h</a></p>'
         self.assertEqual(result.strip(), expected)
 
+    def test_ref_link(self):
+        result = mistune.html('[link][h]\n\n[h]: /foo')
+        expected = '<p><a href="/foo">link</a></p>'
+        self.assertEqual(result.strip(), expected)
+
     def test_allow_harmful_protocols(self):
         renderer = mistune.HTMLRenderer(allow_harmful_protocols=True)
         md = mistune.Markdown(renderer)
         result = md('[h](javascript:alert)')
         expected = '<p><a href="javascript:alert">h</a></p>'
         self.assertEqual(result.strip(), expected)
 
@@ -87,7 +92,14 @@
                 'children': [
                     {'type': 'text', 'raw': 'foo '},
                     {'type': 'strong', 'children': [{'type': 'text', 'raw': 'bar'}]}
                 ]
             },
         ]
         self.assertEqual(result, expected)
+
+
+    def test_emsp(self):
+        md = mistune.create_markdown(escape=False, hard_wrap=True)
+        result = md('\u2003\u2003foo\nbar\n\n\u2003\u2003foobar')
+        expected = '<p>\u2003\u2003foo<br />\nbar</p>\n<p>\u2003\u2003foobar</p>'
+        self.assertEqual(result.strip(), expected)
```

### Comparing `mistune-3.0.0rc5/tests/test_plugins.py` & `mistune-3.0.1/tests/test_plugins.py`

 * *Files identical despite different names*

