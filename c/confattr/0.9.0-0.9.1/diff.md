# Comparing `tmp/confattr-0.9.0.tar.gz` & `tmp/confattr-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "confattr-0.9.0.tar", last modified: Mon Mar  6 11:59:56 2023, max compression
+gzip compressed data, was "confattr-0.9.1.tar", last modified: Mon Mar  6 18:53:59 2023, max compression
```

## Comparing `confattr-0.9.0.tar` & `confattr-0.9.1.tar`

### file list

```diff
@@ -1,204 +1,218 @@
--rw-r--r--   0        0        0      338 2023-02-17 06:19:22.676674 confattr-0.9.0/.gitignore
--rw-r--r--   0        0        0      119 2023-02-17 06:19:22.743340 confattr-0.9.0/.gitlab-ci.yml
--rw-r--r--   0        0        0      657 2022-11-21 06:04:24.790000 confattr-0.9.0/LICENSE
--rw-r--r--   0        0        0      173 2023-02-17 06:19:22.723340 confattr-0.9.0/README.md
--rw-r--r--   0        0        0      213 2023-02-17 06:19:22.930007 confattr-0.9.0/conftest.py
--rw-r--r--   0        0        0      638 2023-02-17 06:19:22.676674 confattr-0.9.0/docs/Makefile
--rw-r--r--   0        0        0      133 2023-03-03 15:36:20.916820 confattr-0.9.0/docs/build/html/_sources/confattr.config.rst.txt
--rw-r--r--   0        0        0      145 2023-03-03 15:36:20.916820 confattr-0.9.0/docs/build/html/_sources/confattr.configfile.rst.txt
--rw-r--r--   0        0        0      289 2023-03-03 15:36:20.916820 confattr-0.9.0/docs/build/html/_sources/confattr.rst.txt
--rw-r--r--   0        0        0      162 2023-03-03 15:36:20.920153 confattr-0.9.0/docs/build/html/_sources/confattr.subprocess_pipe.rst.txt
--rw-r--r--   0        0        0      130 2023-03-03 15:36:20.920153 confattr-0.9.0/docs/build/html/_sources/confattr.types.rst.txt
--rw-r--r--   0        0        0      130 2023-03-03 15:36:20.920153 confattr-0.9.0/docs/build/html/_sources/confattr.utils.rst.txt
--rw-r--r--   0        0        0     2811 2023-03-03 15:36:20.920153 confattr-0.9.0/docs/build/html/_sources/index.rst.txt
--rw-r--r--   0        0        0    24838 2023-03-06 11:58:30.580027 confattr-0.9.0/docs/build/html/_sources/intro.rst.txt
--rw-r--r--   0        0        0       61 2023-03-03 15:36:20.920153 confattr-0.9.0/docs/build/html/_sources/modules.rst.txt
--rw-r--r--   0        0        0     4418 2023-03-03 15:36:20.920153 confattr-0.9.0/docs/build/html/_static/_sphinx_javascript_frameworks_compat.js
--rw-r--r--   0        0        0    14813 2023-03-06 11:58:30.580027 confattr-0.9.0/docs/build/html/_static/basic.css
--rw-r--r--   0        0        0     3229 2023-03-03 15:36:20.920153 confattr-0.9.0/docs/build/html/_static/css/badge_only.css
--rw-r--r--   0        0        0    87624 2023-03-03 15:36:20.920153 confattr-0.9.0/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff
--rw-r--r--   0        0        0    67312 2023-03-03 15:36:20.920153 confattr-0.9.0/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff2
--rw-r--r--   0        0        0    86288 2023-03-03 15:36:20.920153 confattr-0.9.0/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff
--rw-r--r--   0        0        0    66444 2023-03-03 15:36:20.920153 confattr-0.9.0/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff2
--rw-r--r--   0        0        0   165742 2023-03-03 15:36:20.923487 confattr-0.9.0/docs/build/html/_static/css/fonts/fontawesome-webfont.eot
--rw-r--r--   0        0        0   444379 2023-03-03 15:36:20.923487 confattr-0.9.0/docs/build/html/_static/css/fonts/fontawesome-webfont.svg
--rw-r--r--   0        0        0   165548 2023-03-03 15:36:20.926820 confattr-0.9.0/docs/build/html/_static/css/fonts/fontawesome-webfont.ttf
--rw-r--r--   0        0        0    98024 2023-03-03 15:36:20.926820 confattr-0.9.0/docs/build/html/_static/css/fonts/fontawesome-webfont.woff
--rw-r--r--   0        0        0    77160 2023-03-03 15:36:20.926820 confattr-0.9.0/docs/build/html/_static/css/fonts/fontawesome-webfont.woff2
--rw-r--r--   0        0        0   323344 2023-03-03 15:36:20.926820 confattr-0.9.0/docs/build/html/_static/css/fonts/lato-bold-italic.woff
--rw-r--r--   0        0        0   193308 2023-03-03 15:36:20.926820 confattr-0.9.0/docs/build/html/_static/css/fonts/lato-bold-italic.woff2
--rw-r--r--   0        0        0   309728 2023-03-03 15:36:20.930154 confattr-0.9.0/docs/build/html/_static/css/fonts/lato-bold.woff
--rw-r--r--   0        0        0   184912 2023-03-03 15:36:20.930154 confattr-0.9.0/docs/build/html/_static/css/fonts/lato-bold.woff2
--rw-r--r--   0        0        0   328412 2023-03-03 15:36:20.930154 confattr-0.9.0/docs/build/html/_static/css/fonts/lato-normal-italic.woff
--rw-r--r--   0        0        0   195704 2023-03-03 15:36:20.933487 confattr-0.9.0/docs/build/html/_static/css/fonts/lato-normal-italic.woff2
--rw-r--r--   0        0        0   309192 2023-03-03 15:36:20.933487 confattr-0.9.0/docs/build/html/_static/css/fonts/lato-normal.woff
--rw-r--r--   0        0        0   182708 2023-03-03 15:36:20.933487 confattr-0.9.0/docs/build/html/_static/css/fonts/lato-normal.woff2
--rw-r--r--   0        0        0   135235 2023-03-06 11:58:30.580027 confattr-0.9.0/docs/build/html/_static/css/theme.css
--rw-r--r--   0        0        0     4472 2023-03-06 11:58:30.580027 confattr-0.9.0/docs/build/html/_static/doctools.js
--rw-r--r--   0        0        0      421 2023-03-06 11:58:30.580027 confattr-0.9.0/docs/build/html/_static/documentation_options.js
--rw-r--r--   0        0        0      286 2023-03-03 15:36:20.933487 confattr-0.9.0/docs/build/html/_static/file.png
--rw-r--r--   0        0        0   288580 2023-03-03 15:36:20.936820 confattr-0.9.0/docs/build/html/_static/jquery-3.6.0.js
--rw-r--r--   0        0        0    89501 2023-03-03 15:36:20.936820 confattr-0.9.0/docs/build/html/_static/jquery.js
--rw-r--r--   0        0        0      934 2023-03-03 15:36:20.936820 confattr-0.9.0/docs/build/html/_static/js/badge_only.js
--rw-r--r--   0        0        0     4370 2023-03-03 15:36:20.936820 confattr-0.9.0/docs/build/html/_static/js/html5shiv-printshiv.min.js
--rw-r--r--   0        0        0     2734 2023-03-03 15:36:20.936820 confattr-0.9.0/docs/build/html/_static/js/html5shiv.min.js
--rw-r--r--   0        0        0     5023 2023-03-03 15:36:20.936820 confattr-0.9.0/docs/build/html/_static/js/theme.js
--rw-r--r--   0        0        0     4758 2023-03-06 11:58:30.580027 confattr-0.9.0/docs/build/html/_static/language_data.js
--rw-r--r--   0        0        0       90 2023-03-03 15:36:20.936820 confattr-0.9.0/docs/build/html/_static/minus.png
--rw-r--r--   0        0        0     4208 2023-03-03 15:36:20.936820 confattr-0.9.0/docs/build/html/_static/nature.css
--rw-r--r--   0        0        0       46 2023-03-03 15:36:20.936820 confattr-0.9.0/docs/build/html/_static/no-ligatures-in-code.css
--rw-r--r--   0        0        0       90 2023-03-03 15:36:20.936820 confattr-0.9.0/docs/build/html/_static/plus.png
--rw-r--r--   0        0        0     4819 2023-03-06 11:42:15.143336 confattr-0.9.0/docs/build/html/_static/pygments.css
--rw-r--r--   0        0        0    18215 2023-03-06 11:58:30.580027 confattr-0.9.0/docs/build/html/_static/searchtools.js
--rw-r--r--   0        0        0     4712 2023-03-03 15:36:20.936820 confattr-0.9.0/docs/build/html/_static/sphinx_highlight.js
--rw-r--r--   0        0        0      204 2023-03-03 15:36:20.936820 confattr-0.9.0/docs/build/html/_static/sphinx_paramlinks.css
--rw-r--r--   0        0        0      117 2023-03-03 15:36:20.936820 confattr-0.9.0/docs/build/html/_static/tab-size.css
--rw-r--r--   0        0        0    68420 2023-03-03 15:36:20.940154 confattr-0.9.0/docs/build/html/_static/underscore-1.13.1.js
--rw-r--r--   0        0        0    19530 2023-03-03 15:36:20.940154 confattr-0.9.0/docs/build/html/_static/underscore.js
--rw-r--r--   0        0        0   113972 2023-03-06 11:58:30.580027 confattr-0.9.0/docs/build/html/confattr.config.html
--rw-r--r--   0        0        0   294536 2023-03-06 11:58:30.583360 confattr-0.9.0/docs/build/html/confattr.configfile.html
--rw-r--r--   0        0        0   411588 2023-03-06 11:58:30.583360 confattr-0.9.0/docs/build/html/confattr.html
--rw-r--r--   0        0        0    13482 2023-03-06 11:58:30.583360 confattr-0.9.0/docs/build/html/confattr.subprocess_pipe.html
--rw-r--r--   0        0        0    47974 2023-03-06 11:58:30.583360 confattr-0.9.0/docs/build/html/confattr.types.html
--rw-r--r--   0        0        0    42108 2023-03-06 11:58:30.583360 confattr-0.9.0/docs/build/html/confattr.utils.html
--rw-r--r--   0        0        0    90501 2023-03-06 11:58:30.583360 confattr-0.9.0/docs/build/html/genindex.html
--rw-r--r--   0        0        0    22315 2023-03-06 11:58:30.583360 confattr-0.9.0/docs/build/html/index.html
--rw-r--r--   0        0        0   165380 2023-03-06 11:58:30.586693 confattr-0.9.0/docs/build/html/intro.html
--rw-r--r--   0        0        0    47023 2023-03-06 11:58:30.586693 confattr-0.9.0/docs/build/html/modules.html
--rw-r--r--   0        0        0     3912 2023-03-06 11:58:30.586693 confattr-0.9.0/docs/build/html/objects.inv
--rw-r--r--   0        0        0     5971 2023-03-06 11:58:30.586693 confattr-0.9.0/docs/build/html/py-modindex.html
--rw-r--r--   0        0        0     4701 2023-03-06 11:58:30.586693 confattr-0.9.0/docs/build/html/search.html
--rw-r--r--   0        0        0    89819 2023-03-06 11:58:30.586693 confattr-0.9.0/docs/build/html/searchindex.js
--rw-r--r--   0        0        0      804 2023-02-17 06:19:22.683340 confattr-0.9.0/docs/make.bat
--rw-r--r--   0        0        0      152 2023-02-17 06:19:22.683340 confattr-0.9.0/docs/source/_static/.gitignore
--rw-r--r--   0        0        0       46 2023-02-17 20:06:23.486904 confattr-0.9.0/docs/source/_static/no-ligatures-in-code.css
--rw-r--r--   0        0        0      117 2023-02-18 08:27:48.050112 confattr-0.9.0/docs/source/_static/tab-size.css
--rw-r--r--   0        0        0     2564 2023-03-06 11:58:30.586693 confattr-0.9.0/docs/source/conf.py
--rw-r--r--   0        0        0      133 2023-02-17 06:19:22.683340 confattr-0.9.0/docs/source/confattr.config.rst
--rw-r--r--   0        0        0      145 2023-02-17 06:19:22.683340 confattr-0.9.0/docs/source/confattr.configfile.rst
--rw-r--r--   0        0        0      289 2023-02-17 06:19:22.683340 confattr-0.9.0/docs/source/confattr.rst
--rw-r--r--   0        0        0      162 2023-02-17 06:19:22.683340 confattr-0.9.0/docs/source/confattr.subprocess_pipe.rst
--rw-r--r--   0        0        0      130 2023-02-17 06:19:22.683340 confattr-0.9.0/docs/source/confattr.types.rst
--rw-r--r--   0        0        0      130 2023-02-17 06:19:22.843340 confattr-0.9.0/docs/source/confattr.utils.rst
--rw-r--r--   0        0        0        0 2023-02-17 06:19:22.816674 confattr-0.9.0/docs/source/examples/_easy_to_use/__init__.py
--rw-r--r--   0        0        0       16 2023-02-17 06:19:22.816674 confattr-0.9.0/docs/source/examples/_easy_to_use/config
--rw-r--r--   0        0        0      318 2023-02-17 06:19:22.936674 confattr-0.9.0/docs/source/examples/_easy_to_use/example.py
--rw-r--r--   0        0        0        6 2023-02-17 06:19:22.816674 confattr-0.9.0/docs/source/examples/_easy_to_use/output.txt
--rw-r--r--   0        0        0      487 2023-02-17 06:19:22.936674 confattr-0.9.0/docs/source/examples/_easy_to_use/test_example.py
--rw-r--r--   0        0        0        0 2023-02-17 06:19:22.790007 confattr-0.9.0/docs/source/examples/config_and_configfile/__init__.py
--rw-r--r--   0        0        0       33 2023-02-17 06:19:22.790007 confattr-0.9.0/docs/source/examples/config_and_configfile/config
--rw-r--r--   0        0        0     1420 2023-02-18 08:27:48.050112 confattr-0.9.0/docs/source/examples/config_and_configfile/example.py
--rw-r--r--   0        0        0      570 2023-02-18 08:27:48.050112 confattr-0.9.0/docs/source/examples/config_and_configfile/expected-config
--rw-r--r--   0        0        0      570 2023-03-06 11:42:02.633336 confattr-0.9.0/docs/source/examples/config_and_configfile/exported-config
--rw-r--r--   0        0        0       16 2023-02-17 06:19:22.790007 confattr-0.9.0/docs/source/examples/config_and_configfile/output.txt
--rw-r--r--   0        0        0     1306 2023-02-17 06:19:22.936674 confattr-0.9.0/docs/source/examples/config_and_configfile/test_example.py
--rw-r--r--   0        0        0        0 2023-02-17 06:19:22.790007 confattr-0.9.0/docs/source/examples/config_same_value/__init__.py
--rw-r--r--   0        0        0      309 2023-02-17 06:19:22.936674 confattr-0.9.0/docs/source/examples/config_same_value/example.py
--rw-r--r--   0        0        0       12 2023-02-17 06:19:22.790007 confattr-0.9.0/docs/source/examples/config_same_value/output.txt
--rw-r--r--   0        0        0      487 2023-02-17 06:19:22.936674 confattr-0.9.0/docs/source/examples/config_same_value/test_example.py
--rw-r--r--   0        0        0        0 2023-02-17 06:19:22.790007 confattr-0.9.0/docs/source/examples/config_without_classes/__init__.py
--rw-r--r--   0        0        0       27 2023-02-17 06:19:22.790007 confattr-0.9.0/docs/source/examples/config_without_classes/config
--rw-r--r--   0        0        0      310 2023-02-18 08:27:48.050112 confattr-0.9.0/docs/source/examples/config_without_classes/example.py
--rw-r--r--   0        0        0        7 2023-02-17 06:19:22.790007 confattr-0.9.0/docs/source/examples/config_without_classes/output.txt
--rw-r--r--   0        0        0      486 2023-02-17 06:19:22.936674 confattr-0.9.0/docs/source/examples/config_without_classes/test_example.py
--rw-r--r--   0        0        0        0 2023-02-17 06:19:22.790007 confattr-0.9.0/docs/source/examples/custom_set/__init__.py
--rw-r--r--   0        0        0       98 2023-02-17 06:19:22.790007 confattr-0.9.0/docs/source/examples/custom_set/config
--rw-r--r--   0        0        0       28 2023-02-17 06:19:22.790007 confattr-0.9.0/docs/source/examples/custom_set/config2
--rw-r--r--   0        0        0     1387 2023-02-18 08:27:48.050112 confattr-0.9.0/docs/source/examples/custom_set/example.py
--rw-r--r--   0        0        0      375 2023-02-18 08:27:48.050112 confattr-0.9.0/docs/source/examples/custom_set/example_no_include.py
--rw-r--r--   0        0        0     1007 2023-02-18 08:27:48.050112 confattr-0.9.0/docs/source/examples/custom_set/example_save.py
--rw-r--r--   0        0        0       19 2023-02-17 06:19:22.790007 confattr-0.9.0/docs/source/examples/custom_set/output.txt
--rw-r--r--   0        0        0       86 2023-02-18 08:27:48.050112 confattr-0.9.0/docs/source/examples/custom_set/output_no_include.txt
--rw-r--r--   0        0        0     1214 2023-02-17 14:58:19.840013 confattr-0.9.0/docs/source/examples/custom_set/test_example.py
--rw-r--r--   0        0        0        0 2023-02-17 06:19:22.936674 confattr-0.9.0/docs/source/examples/env/__init__.py
--rw-r--r--   0        0        0      233 2023-02-17 06:19:22.936674 confattr-0.9.0/docs/source/examples/env/example.py
--rw-r--r--   0        0        0      324 2023-02-17 06:19:22.936674 confattr-0.9.0/docs/source/examples/env/example.sh
--rw-r--r--   0        0        0       18 2023-02-17 06:19:22.936674 confattr-0.9.0/docs/source/examples/env/expected_output.txt
--rw-r--r--   0        0        0      511 2023-02-17 06:19:22.936674 confattr-0.9.0/docs/source/examples/env/test_example.py
--rw-r--r--   0        0        0        0 2023-02-17 06:19:22.843340 confattr-0.9.0/docs/source/examples/generating_help/__init__.py
--rwxr-xr-x   0        0        0      683 2023-02-17 06:19:22.843340 confattr-0.9.0/docs/source/examples/generating_help/example.py
--rwxr-xr-x   0        0        0      310 2023-02-17 06:19:22.936674 confattr-0.9.0/docs/source/examples/generating_help/example_config.py
--rwxr-xr-x   0        0        0      390 2023-02-17 06:19:22.936674 confattr-0.9.0/docs/source/examples/generating_help/example_raw_config.py
--rwxr-xr-x   0        0        0      336 2023-02-17 06:19:22.936674 confattr-0.9.0/docs/source/examples/generating_help/example_raw_help.py
--rw-r--r--   0        0        0     1129 2023-03-06 11:58:30.586693 confattr-0.9.0/docs/source/examples/generating_help/expected-config
--rw-r--r--   0        0        0      601 2023-03-06 11:58:30.586693 confattr-0.9.0/docs/source/examples/generating_help/expected-no-multi-config
--rw-r--r--   0        0        0     2540 2023-03-06 11:58:30.586693 confattr-0.9.0/docs/source/examples/generating_help/expected-no-multi-help.txt
--rw-r--r--   0        0        0     1121 2023-03-06 11:58:30.586693 confattr-0.9.0/docs/source/examples/generating_help/expected-raw-config
--rw-r--r--   0        0        0     3847 2023-02-17 06:19:22.986674 confattr-0.9.0/docs/source/examples/generating_help/expected-raw-help.txt
--rwxr-xr-x   0        0        0      563 2023-03-06 11:58:30.586693 confattr-0.9.0/docs/source/examples/generating_help/no_multi_example.py
--rwxr-xr-x   0        0        0      328 2023-03-06 11:58:30.586693 confattr-0.9.0/docs/source/examples/generating_help/no_multi_example_config.py
--rw-r--r--   0        0        0     3989 2023-02-17 06:19:22.986674 confattr-0.9.0/docs/source/examples/generating_help/output.txt
--rwxr-xr-x   0        0        0     3026 2023-03-06 11:58:30.586693 confattr-0.9.0/docs/source/examples/generating_help/test_example.py
--rw-r--r--   0        0        0        0 2023-02-17 06:19:22.843340 confattr-0.9.0/docs/source/examples/include/__init__.py
--rw-r--r--   0        0        0      261 2023-02-17 16:34:32.050155 confattr-0.9.0/docs/source/examples/include/config
--rw-r--r--   0        0        0     4016 2023-02-18 08:27:48.050112 confattr-0.9.0/docs/source/examples/include/example.py
--rw-r--r--   0        0        0       27 2023-02-17 06:19:22.843340 confattr-0.9.0/docs/source/examples/include/mirror
--rw-r--r--   0        0        0      260 2023-02-17 06:19:22.843340 confattr-0.9.0/docs/source/examples/include/output.txt
--rw-r--r--   0        0        0      436 2023-02-17 16:33:58.936821 confattr-0.9.0/docs/source/examples/include/test_example.py
--rw-r--r--   0        0        0       24 2023-02-17 06:19:22.843340 confattr-0.9.0/docs/source/examples/include/two-way
--rw-r--r--   0        0        0        0 2023-02-17 06:19:22.790007 confattr-0.9.0/docs/source/examples/map/__init__.py
--rw-r--r--   0        0        0       54 2023-02-17 16:34:55.703489 confattr-0.9.0/docs/source/examples/map/config
--rw-r--r--   0        0        0     2256 2023-03-04 11:24:53.693360 confattr-0.9.0/docs/source/examples/map/example.py
--rw-r--r--   0        0        0      252 2023-02-17 06:19:22.843340 confattr-0.9.0/docs/source/examples/map/example_print_help.py
--rw-r--r--   0        0        0      153 2023-02-17 06:19:22.790007 confattr-0.9.0/docs/source/examples/map/output_help.txt
--rw-r--r--   0        0        0       21 2023-02-17 06:19:22.790007 confattr-0.9.0/docs/source/examples/map/requirements.txt
--rw-r--r--   0        0        0      506 2023-02-17 06:19:22.936674 confattr-0.9.0/docs/source/examples/map/test_print_help.py
--rw-r--r--   0        0        0        0 2023-02-17 06:19:22.790007 confattr-0.9.0/docs/source/examples/map_save/__init__.py
--rw-r--r--   0        0        0      123 2023-03-06 11:58:30.586693 confattr-0.9.0/docs/source/examples/map_save/config
--rw-r--r--   0        0        0      123 2023-03-06 11:58:30.586693 confattr-0.9.0/docs/source/examples/map_save/config_expected
--rw-r--r--   0        0        0     1357 2023-02-17 06:19:22.936674 confattr-0.9.0/docs/source/examples/map_save/example_1.py
--rw-r--r--   0        0        0     1780 2023-02-17 06:19:22.936674 confattr-0.9.0/docs/source/examples/map_save/example_3.py
--rw-r--r--   0        0        0      939 2023-02-17 06:19:22.846674 confattr-0.9.0/docs/source/examples/map_save/test_example_3.py
--rw-r--r--   0        0        0        0 2023-02-17 06:19:22.790007 confattr-0.9.0/docs/source/examples/multiconfig/__init__.py
--rw-r--r--   0        0        0      100 2023-02-17 06:19:22.790007 confattr-0.9.0/docs/source/examples/multiconfig/config
--rw-r--r--   0        0        0      122 2023-02-17 06:19:22.790007 confattr-0.9.0/docs/source/examples/multiconfig/config2
--rw-r--r--   0        0        0      899 2023-02-18 08:27:48.050112 confattr-0.9.0/docs/source/examples/multiconfig/example.py
--rw-r--r--   0        0        0       95 2023-02-17 06:19:22.790007 confattr-0.9.0/docs/source/examples/multiconfig/output.txt
--rw-r--r--   0        0        0      125 2023-02-17 06:19:22.790007 confattr-0.9.0/docs/source/examples/multiconfig/output2.txt
--rw-r--r--   0        0        0      942 2023-02-17 06:19:22.936674 confattr-0.9.0/docs/source/examples/multiconfig/test_example.py
--rw-r--r--   0        0        0        0 2023-03-06 11:58:30.586693 confattr-0.9.0/docs/source/examples/multiconfig_reset/__init__.py
--rw-r--r--   0        0        0      651 2023-03-06 11:58:30.586693 confattr-0.9.0/docs/source/examples/multiconfig_reset/example.py
--rw-r--r--   0        0        0       29 2023-03-06 11:58:30.586693 confattr-0.9.0/docs/source/examples/multiconfig_reset/expected-config
--rw-r--r--   0        0        0      780 2023-03-06 11:58:30.586693 confattr-0.9.0/docs/source/examples/multiconfig_reset/test_example.py
--rw-r--r--   0        0        0        0 2023-02-17 06:19:22.790007 confattr-0.9.0/docs/source/examples/regex/__init__.py
--rw-r--r--   0        0        0      811 2023-03-06 11:42:06.940003 confattr-0.9.0/docs/source/examples/regex/config
--rw-r--r--   0        0        0     1144 2023-02-18 08:27:48.050112 confattr-0.9.0/docs/source/examples/regex/example.py
--rw-r--r--   0        0        0      811 2023-02-18 08:27:48.050112 confattr-0.9.0/docs/source/examples/regex/expected-config
--rw-r--r--   0        0        0     1002 2023-02-17 06:19:22.936674 confattr-0.9.0/docs/source/examples/regex/test_example.py
--rw-r--r--   0        0        0        0 2023-02-17 06:19:22.936674 confattr-0.9.0/docs/source/examples/testing_monkeypatch_config/__init__.py
--rw-r--r--   0        0        0     1164 2023-02-17 06:19:22.936674 confattr-0.9.0/docs/source/examples/testing_monkeypatch_config/example.py
--rwxr-xr-x   0        0        0      256 2023-02-17 06:19:22.936674 confattr-0.9.0/docs/source/examples/testing_monkeypatch_config/test_example.py
--rw-r--r--   0        0        0        0 2023-02-17 06:19:22.936674 confattr-0.9.0/docs/source/examples/testing_monkeypatch_multiconfig/__init__.py
--rw-r--r--   0        0        0     1252 2023-02-17 06:19:22.936674 confattr-0.9.0/docs/source/examples/testing_monkeypatch_multiconfig/example.py
--rwxr-xr-x   0        0        0      256 2023-02-17 06:19:22.936674 confattr-0.9.0/docs/source/examples/testing_monkeypatch_multiconfig/test_example.py
--rw-r--r--   0        0        0        0 2023-02-17 06:19:22.936674 confattr-0.9.0/docs/source/examples/testing_tmp_path/__init__.py
--rw-r--r--   0        0        0      299 2023-02-17 06:19:22.936674 confattr-0.9.0/docs/source/examples/testing_tmp_path/example.py
--rw-r--r--   0        0        0      600 2023-02-17 06:19:22.940007 confattr-0.9.0/docs/source/examples/testing_tmp_path/test_example.py
--rw-r--r--   0        0        0     2811 2023-03-06 11:42:08.923336 confattr-0.9.0/docs/source/index.rst
--rw-r--r--   0        0        0    24838 2023-03-06 11:58:30.586693 confattr-0.9.0/docs/source/intro.rst
--rw-r--r--   0        0        0       61 2023-02-17 06:19:22.683340 confattr-0.9.0/docs/source/modules.rst
--rw-r--r--   0        0        0      456 2023-02-17 06:19:22.940007 confattr-0.9.0/mypy.ini
--rw-r--r--   0        0        0     4135 2023-02-18 08:27:48.050112 confattr-0.9.0/prepare_for_gitlab_pages.py
--rw-r--r--   0        0        0      819 2023-02-17 06:19:22.790007 confattr-0.9.0/pyproject.toml
--rwxr-xr-x   0        0        0    12469 2023-03-06 11:58:30.586693 confattr-0.9.0/release.sh
--rw-r--r--   0        0        0      224 2023-02-17 06:19:22.790007 confattr-0.9.0/requirements-py36.txt
--rw-r--r--   0        0        0       56 2023-03-03 15:36:34.580154 confattr-0.9.0/requirements-release.txt
--rw-r--r--   0        0        0      134 2023-02-17 06:19:22.793340 confattr-0.9.0/requirements-test.txt
--rw-r--r--   0        0        0       17 2023-02-17 06:19:22.683340 confattr-0.9.0/requirements.txt
--rw-r--r--   0        0        0      917 2023-03-06 11:58:30.586693 confattr-0.9.0/src/confattr/__init__.py
--rw-r--r--   0        0        0    22394 2023-03-06 11:58:30.586693 confattr-0.9.0/src/confattr/config.py
--rw-r--r--   0        0        0    63644 2023-03-06 11:58:30.590027 confattr-0.9.0/src/confattr/configfile.py
--rw-r--r--   0        0        0        0 2022-11-21 06:04:24.790000 confattr-0.9.0/src/confattr/py.typed
--rwxr-xr-x   0        0        0      142 2023-02-17 06:19:22.793340 confattr-0.9.0/src/confattr/runmodule.sh
--rw-r--r--   0        0        0     2176 2023-02-17 06:19:22.686674 confattr-0.9.0/src/confattr/subprocess_pipe.py
--rw-r--r--   0        0        0     7005 2023-02-18 08:27:48.053446 confattr-0.9.0/src/confattr/types.py
--rw-r--r--   0        0        0    11553 2023-03-06 11:58:30.590027 confattr-0.9.0/src/confattr/utils.py
--rwxr-xr-x   0        0        0    51173 2023-03-06 11:58:30.590027 confattr-0.9.0/tests/test_config.py
--rwxr-xr-x   0        0        0     3971 2023-02-17 06:19:22.846674 confattr-0.9.0/tests/test_custom_commands.py
--rw-r--r--   0        0        0     2714 2023-03-06 11:58:30.590027 confattr-0.9.0/tests/test_error.py
--rwxr-xr-x   0        0        0     1168 2023-02-17 06:19:22.846674 confattr-0.9.0/tests/test_formatted_writer.py
--rw-r--r--   0        0        0     1840 2023-02-18 08:27:48.053446 confattr-0.9.0/tests/test_message.py
--rwxr-xr-x   0        0        0      971 2022-11-21 06:04:24.790000 confattr-0.9.0/tests/test_subprocess_pipe.py
--rwxr-xr-x   0        0        0    14602 2023-02-18 08:27:48.053446 confattr-0.9.0/tests/test_utils.py
--rw-r--r--   0        0        0      554 2023-03-06 11:58:30.590027 confattr-0.9.0/tox.ini
--rw-r--r--   0        0        0      947 1970-01-01 00:00:00.000000 confattr-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0      417 2023-03-06 18:53:55.080496 confattr-0.9.1/.coveragerc
+-rw-r--r--   0        0        0      348 2023-03-06 18:53:55.080496 confattr-0.9.1/.gitignore
+-rw-r--r--   0        0        0      119 2023-03-06 18:04:37.317089 confattr-0.9.1/.gitlab-ci.yml
+-rw-r--r--   0        0        0      657 2022-11-21 06:04:24.790000 confattr-0.9.1/LICENSE
+-rw-r--r--   0        0        0      173 2023-03-06 17:56:17.923744 confattr-0.9.1/README.md
+-rw-r--r--   0        0        0      213 2023-03-06 17:56:18.123744 confattr-0.9.1/conftest.py
+-rw-r--r--   0        0        0      638 2023-03-06 17:56:17.873744 confattr-0.9.1/docs/Makefile
+-rw-r--r--   0        0        0      133 2023-03-06 17:56:17.873744 confattr-0.9.1/docs/build/html/_sources/confattr.config.rst.txt
+-rw-r--r--   0        0        0      145 2023-03-06 17:56:17.873744 confattr-0.9.1/docs/build/html/_sources/confattr.configfile.rst.txt
+-rw-r--r--   0        0        0      289 2023-03-06 17:56:17.873744 confattr-0.9.1/docs/build/html/_sources/confattr.rst.txt
+-rw-r--r--   0        0        0      162 2023-03-06 17:56:17.873744 confattr-0.9.1/docs/build/html/_sources/confattr.subprocess_pipe.rst.txt
+-rw-r--r--   0        0        0      130 2023-03-06 17:56:17.873744 confattr-0.9.1/docs/build/html/_sources/confattr.types.rst.txt
+-rw-r--r--   0        0        0      130 2023-03-06 17:56:18.033743 confattr-0.9.1/docs/build/html/_sources/confattr.utils.rst.txt
+-rw-r--r--   0        0        0     2857 2023-03-06 18:53:55.080496 confattr-0.9.1/docs/build/html/_sources/index.rst.txt
+-rw-r--r--   0        0        0    24838 2023-03-06 17:56:18.273743 confattr-0.9.1/docs/build/html/_sources/intro.rst.txt
+-rw-r--r--   0        0        0       61 2023-03-06 17:56:17.873744 confattr-0.9.1/docs/build/html/_sources/modules.rst.txt
+-rw-r--r--   0        0        0     4418 2023-03-06 17:56:17.873744 confattr-0.9.1/docs/build/html/_static/_sphinx_javascript_frameworks_compat.js
+-rw-r--r--   0        0        0    14813 2023-03-06 18:52:26.000494 confattr-0.9.1/docs/build/html/_static/basic.css
+-rw-r--r--   0        0        0     3229 2023-03-06 17:56:18.063743 confattr-0.9.1/docs/build/html/_static/css/badge_only.css
+-rw-r--r--   0        0        0    87624 2023-03-06 17:56:18.063743 confattr-0.9.1/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff
+-rw-r--r--   0        0        0    67312 2023-03-06 17:56:18.063743 confattr-0.9.1/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff2
+-rw-r--r--   0        0        0    86288 2023-03-06 17:56:18.063743 confattr-0.9.1/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff
+-rw-r--r--   0        0        0    66444 2023-03-06 17:56:18.063743 confattr-0.9.1/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff2
+-rw-r--r--   0        0        0   165742 2023-03-06 17:56:18.067077 confattr-0.9.1/docs/build/html/_static/css/fonts/fontawesome-webfont.eot
+-rw-r--r--   0        0        0   444379 2023-03-06 17:56:18.067077 confattr-0.9.1/docs/build/html/_static/css/fonts/fontawesome-webfont.svg
+-rw-r--r--   0        0        0   165548 2023-03-06 17:56:18.070410 confattr-0.9.1/docs/build/html/_static/css/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0        0        0    98024 2023-03-06 17:56:18.070410 confattr-0.9.1/docs/build/html/_static/css/fonts/fontawesome-webfont.woff
+-rw-r--r--   0        0        0    77160 2023-03-06 17:56:18.070410 confattr-0.9.1/docs/build/html/_static/css/fonts/fontawesome-webfont.woff2
+-rw-r--r--   0        0        0   323344 2023-03-06 17:56:18.070410 confattr-0.9.1/docs/build/html/_static/css/fonts/lato-bold-italic.woff
+-rw-r--r--   0        0        0   193308 2023-03-06 17:56:18.073743 confattr-0.9.1/docs/build/html/_static/css/fonts/lato-bold-italic.woff2
+-rw-r--r--   0        0        0   309728 2023-03-06 17:56:18.073743 confattr-0.9.1/docs/build/html/_static/css/fonts/lato-bold.woff
+-rw-r--r--   0        0        0   184912 2023-03-06 17:56:18.073743 confattr-0.9.1/docs/build/html/_static/css/fonts/lato-bold.woff2
+-rw-r--r--   0        0        0   328412 2023-03-06 17:56:18.077077 confattr-0.9.1/docs/build/html/_static/css/fonts/lato-normal-italic.woff
+-rw-r--r--   0        0        0   195704 2023-03-06 17:56:18.077077 confattr-0.9.1/docs/build/html/_static/css/fonts/lato-normal-italic.woff2
+-rw-r--r--   0        0        0   309192 2023-03-06 17:56:18.077077 confattr-0.9.1/docs/build/html/_static/css/fonts/lato-normal.woff
+-rw-r--r--   0        0        0   182708 2023-03-06 17:56:18.080410 confattr-0.9.1/docs/build/html/_static/css/fonts/lato-normal.woff2
+-rw-r--r--   0        0        0   135235 2023-03-06 17:56:18.273743 confattr-0.9.1/docs/build/html/_static/css/theme.css
+-rw-r--r--   0        0        0     4472 2023-03-06 17:56:18.273743 confattr-0.9.1/docs/build/html/_static/doctools.js
+-rw-r--r--   0        0        0      421 2023-03-06 18:53:55.080496 confattr-0.9.1/docs/build/html/_static/documentation_options.js
+-rw-r--r--   0        0        0      286 2023-03-06 17:56:17.873744 confattr-0.9.1/docs/build/html/_static/file.png
+-rw-r--r--   0        0        0   288580 2023-03-06 17:56:17.877077 confattr-0.9.1/docs/build/html/_static/jquery-3.6.0.js
+-rw-r--r--   0        0        0    89501 2023-03-06 17:56:17.877077 confattr-0.9.1/docs/build/html/_static/jquery.js
+-rw-r--r--   0        0        0      934 2023-03-06 17:56:18.080410 confattr-0.9.1/docs/build/html/_static/js/badge_only.js
+-rw-r--r--   0        0        0     4370 2023-03-06 17:56:18.080410 confattr-0.9.1/docs/build/html/_static/js/html5shiv-printshiv.min.js
+-rw-r--r--   0        0        0     2734 2023-03-06 17:56:18.080410 confattr-0.9.1/docs/build/html/_static/js/html5shiv.min.js
+-rw-r--r--   0        0        0     5023 2023-03-06 17:56:18.080410 confattr-0.9.1/docs/build/html/_static/js/theme.js
+-rw-r--r--   0        0        0     4758 2023-03-06 18:52:26.007160 confattr-0.9.1/docs/build/html/_static/language_data.js
+-rw-r--r--   0        0        0       90 2023-03-06 17:56:17.877077 confattr-0.9.1/docs/build/html/_static/minus.png
+-rw-r--r--   0        0        0     4208 2023-03-06 17:56:18.037077 confattr-0.9.1/docs/build/html/_static/nature.css
+-rw-r--r--   0        0        0       46 2023-03-06 17:56:18.080410 confattr-0.9.1/docs/build/html/_static/no-ligatures-in-code.css
+-rw-r--r--   0        0        0       90 2023-03-06 17:56:17.877077 confattr-0.9.1/docs/build/html/_static/plus.png
+-rw-r--r--   0        0        0     4819 2023-03-06 18:52:25.993827 confattr-0.9.1/docs/build/html/_static/pygments.css
+-rw-r--r--   0        0        0    18215 2023-03-06 17:56:18.277077 confattr-0.9.1/docs/build/html/_static/searchtools.js
+-rw-r--r--   0        0        0     4712 2023-03-06 17:56:17.877077 confattr-0.9.1/docs/build/html/_static/sphinx_highlight.js
+-rw-r--r--   0        0        0      204 2023-03-06 17:56:17.990410 confattr-0.9.1/docs/build/html/_static/sphinx_paramlinks.css
+-rw-r--r--   0        0        0      117 2023-03-06 17:56:18.223744 confattr-0.9.1/docs/build/html/_static/tab-size.css
+-rw-r--r--   0        0        0    68420 2023-03-06 17:56:17.877077 confattr-0.9.1/docs/build/html/_static/underscore-1.13.1.js
+-rw-r--r--   0        0        0    19530 2023-03-06 17:56:17.877077 confattr-0.9.1/docs/build/html/_static/underscore.js
+-rw-r--r--   0        0        0   113972 2023-03-06 18:50:28.383824 confattr-0.9.1/docs/build/html/confattr.config.html
+-rw-r--r--   0        0        0   294536 2023-03-06 18:50:28.387158 confattr-0.9.1/docs/build/html/confattr.configfile.html
+-rw-r--r--   0        0        0   411588 2023-03-06 18:50:28.387158 confattr-0.9.1/docs/build/html/confattr.html
+-rw-r--r--   0        0        0    13482 2023-03-06 18:50:28.387158 confattr-0.9.1/docs/build/html/confattr.subprocess_pipe.html
+-rw-r--r--   0        0        0    47974 2023-03-06 18:50:28.387158 confattr-0.9.1/docs/build/html/confattr.types.html
+-rw-r--r--   0        0        0    42108 2023-03-06 18:50:28.387158 confattr-0.9.1/docs/build/html/confattr.utils.html
+-rw-r--r--   0        0        0    20650 2023-03-06 18:53:55.083829 confattr-0.9.1/docs/build/html/coverage/coverage_html.js
+-rw-r--r--   0        0        0    13775 2023-03-06 18:53:55.083829 confattr-0.9.1/docs/build/html/coverage/d_0dd2fbccdefb184f___init___py.html
+-rw-r--r--   0        0        0   181571 2023-03-06 18:53:55.083829 confattr-0.9.1/docs/build/html/coverage/d_0dd2fbccdefb184f_config_py.html
+-rw-r--r--   0        0        0   458963 2023-03-06 18:53:55.083829 confattr-0.9.1/docs/build/html/coverage/d_0dd2fbccdefb184f_configfile_py.html
+-rw-r--r--   0        0        0    22463 2023-03-06 18:53:55.083829 confattr-0.9.1/docs/build/html/coverage/d_0dd2fbccdefb184f_subprocess_pipe_py.html
+-rw-r--r--   0        0        0    67860 2023-03-06 18:53:55.083829 confattr-0.9.1/docs/build/html/coverage/d_0dd2fbccdefb184f_types_py.html
+-rw-r--r--   0        0        0    86399 2023-03-06 18:53:55.087163 confattr-0.9.1/docs/build/html/coverage/d_0dd2fbccdefb184f_utils_py.html
+-rw-r--r--   0        0        0     1732 2023-03-06 18:53:55.087163 confattr-0.9.1/docs/build/html/coverage/favicon_32.png
+-rw-r--r--   0        0        0     5680 2023-03-06 18:53:55.087163 confattr-0.9.1/docs/build/html/coverage/index.html
+-rw-r--r--   0        0        0     9004 2023-03-06 18:53:55.087163 confattr-0.9.1/docs/build/html/coverage/keybd_closed.png
+-rw-r--r--   0        0        0     9003 2023-03-06 18:53:55.087163 confattr-0.9.1/docs/build/html/coverage/keybd_open.png
+-rw-r--r--   0        0        0     1585 2023-03-06 18:53:55.087163 confattr-0.9.1/docs/build/html/coverage/status.json
+-rw-r--r--   0        0        0    12429 2023-03-06 18:53:55.087163 confattr-0.9.1/docs/build/html/coverage/style.css
+-rw-r--r--   0        0        0    90501 2023-03-06 18:53:55.087163 confattr-0.9.1/docs/build/html/genindex.html
+-rw-r--r--   0        0        0    22411 2023-03-06 18:53:55.087163 confattr-0.9.1/docs/build/html/index.html
+-rw-r--r--   0        0        0   165380 2023-03-06 18:53:55.087163 confattr-0.9.1/docs/build/html/intro.html
+-rw-r--r--   0        0        0    47023 2023-03-06 18:50:28.390491 confattr-0.9.1/docs/build/html/modules.html
+-rw-r--r--   0        0        0     3912 2023-03-06 18:52:26.027160 confattr-0.9.1/docs/build/html/objects.inv
+-rw-r--r--   0        0        0     5971 2023-03-06 18:53:55.087163 confattr-0.9.1/docs/build/html/py-modindex.html
+-rw-r--r--   0        0        0     4701 2023-03-06 18:53:55.087163 confattr-0.9.1/docs/build/html/search.html
+-rw-r--r--   0        0        0    50204 2023-03-06 18:53:55.087163 confattr-0.9.1/docs/build/html/searchindex.js
+-rw-r--r--   0        0        0      804 2023-03-06 17:56:17.880410 confattr-0.9.1/docs/make.bat
+-rw-r--r--   0        0        0      152 2023-03-06 17:56:17.880410 confattr-0.9.1/docs/source/_static/.gitignore
+-rw-r--r--   0        0        0       46 2023-03-06 17:56:18.083743 confattr-0.9.1/docs/source/_static/no-ligatures-in-code.css
+-rw-r--r--   0        0        0      117 2023-03-06 17:56:18.230410 confattr-0.9.1/docs/source/_static/tab-size.css
+-rw-r--r--   0        0        0     2564 2023-03-06 18:53:55.087163 confattr-0.9.1/docs/source/conf.py
+-rw-r--r--   0        0        0      133 2023-03-06 17:56:17.880410 confattr-0.9.1/docs/source/confattr.config.rst
+-rw-r--r--   0        0        0      145 2023-03-06 17:56:17.880410 confattr-0.9.1/docs/source/confattr.configfile.rst
+-rw-r--r--   0        0        0      289 2023-03-06 17:56:17.880410 confattr-0.9.1/docs/source/confattr.rst
+-rw-r--r--   0        0        0      162 2023-03-06 17:56:17.880410 confattr-0.9.1/docs/source/confattr.subprocess_pipe.rst
+-rw-r--r--   0        0        0      130 2023-03-06 17:56:17.880410 confattr-0.9.1/docs/source/confattr.types.rst
+-rw-r--r--   0        0        0      130 2023-03-06 17:56:18.040410 confattr-0.9.1/docs/source/confattr.utils.rst
+-rw-r--r--   0        0        0        0 2023-03-06 17:56:18.017077 confattr-0.9.1/docs/source/examples/_easy_to_use/__init__.py
+-rw-r--r--   0        0        0       16 2023-03-06 17:56:18.017077 confattr-0.9.1/docs/source/examples/_easy_to_use/config
+-rw-r--r--   0        0        0      318 2023-03-06 17:56:18.130410 confattr-0.9.1/docs/source/examples/_easy_to_use/example.py
+-rw-r--r--   0        0        0        6 2023-03-06 17:56:18.017077 confattr-0.9.1/docs/source/examples/_easy_to_use/output.txt
+-rw-r--r--   0        0        0      487 2023-03-06 17:56:18.130410 confattr-0.9.1/docs/source/examples/_easy_to_use/test_example.py
+-rw-r--r--   0        0        0        0 2023-03-06 17:56:17.993744 confattr-0.9.1/docs/source/examples/config_and_configfile/__init__.py
+-rw-r--r--   0        0        0       33 2023-03-06 17:56:17.993744 confattr-0.9.1/docs/source/examples/config_and_configfile/config
+-rw-r--r--   0        0        0     1420 2023-03-06 17:56:18.230410 confattr-0.9.1/docs/source/examples/config_and_configfile/example.py
+-rw-r--r--   0        0        0      570 2023-03-06 17:56:18.230410 confattr-0.9.1/docs/source/examples/config_and_configfile/expected-config
+-rw-r--r--   0        0        0      570 2023-03-06 18:52:20.973827 confattr-0.9.1/docs/source/examples/config_and_configfile/exported-config
+-rw-r--r--   0        0        0       16 2023-03-06 17:56:17.993744 confattr-0.9.1/docs/source/examples/config_and_configfile/output.txt
+-rw-r--r--   0        0        0     1306 2023-03-06 17:56:18.130410 confattr-0.9.1/docs/source/examples/config_and_configfile/test_example.py
+-rw-r--r--   0        0        0        0 2023-03-06 17:56:17.993744 confattr-0.9.1/docs/source/examples/config_same_value/__init__.py
+-rw-r--r--   0        0        0      309 2023-03-06 17:56:18.130410 confattr-0.9.1/docs/source/examples/config_same_value/example.py
+-rw-r--r--   0        0        0       12 2023-03-06 17:56:17.993744 confattr-0.9.1/docs/source/examples/config_same_value/output.txt
+-rw-r--r--   0        0        0      487 2023-03-06 17:56:18.130410 confattr-0.9.1/docs/source/examples/config_same_value/test_example.py
+-rw-r--r--   0        0        0        0 2023-03-06 17:56:17.993744 confattr-0.9.1/docs/source/examples/config_without_classes/__init__.py
+-rw-r--r--   0        0        0       27 2023-03-06 17:56:17.993744 confattr-0.9.1/docs/source/examples/config_without_classes/config
+-rw-r--r--   0        0        0      310 2023-03-06 17:56:18.230410 confattr-0.9.1/docs/source/examples/config_without_classes/example.py
+-rw-r--r--   0        0        0        7 2023-03-06 17:56:17.993744 confattr-0.9.1/docs/source/examples/config_without_classes/output.txt
+-rw-r--r--   0        0        0      486 2023-03-06 17:56:18.130410 confattr-0.9.1/docs/source/examples/config_without_classes/test_example.py
+-rw-r--r--   0        0        0        0 2023-03-06 17:56:17.993744 confattr-0.9.1/docs/source/examples/custom_set/__init__.py
+-rw-r--r--   0        0        0       98 2023-03-06 17:56:17.993744 confattr-0.9.1/docs/source/examples/custom_set/config
+-rw-r--r--   0        0        0       28 2023-03-06 17:56:17.993744 confattr-0.9.1/docs/source/examples/custom_set/config2
+-rw-r--r--   0        0        0     1387 2023-03-06 17:56:18.230410 confattr-0.9.1/docs/source/examples/custom_set/example.py
+-rw-r--r--   0        0        0      375 2023-03-06 17:56:18.230410 confattr-0.9.1/docs/source/examples/custom_set/example_no_include.py
+-rw-r--r--   0        0        0     1007 2023-03-06 17:56:18.230410 confattr-0.9.1/docs/source/examples/custom_set/example_save.py
+-rw-r--r--   0        0        0       19 2023-03-06 17:56:17.993744 confattr-0.9.1/docs/source/examples/custom_set/output.txt
+-rw-r--r--   0        0        0       86 2023-03-06 17:56:18.230410 confattr-0.9.1/docs/source/examples/custom_set/output_no_include.txt
+-rw-r--r--   0        0        0     1214 2023-03-06 17:56:18.130410 confattr-0.9.1/docs/source/examples/custom_set/test_example.py
+-rw-r--r--   0        0        0        0 2023-03-06 17:56:18.130410 confattr-0.9.1/docs/source/examples/env/__init__.py
+-rw-r--r--   0        0        0      233 2023-03-06 17:56:18.130410 confattr-0.9.1/docs/source/examples/env/example.py
+-rw-r--r--   0        0        0      324 2023-03-06 17:56:18.130410 confattr-0.9.1/docs/source/examples/env/example.sh
+-rw-r--r--   0        0        0       18 2023-03-06 17:56:18.130410 confattr-0.9.1/docs/source/examples/env/expected_output.txt
+-rw-r--r--   0        0        0      511 2023-03-06 17:56:18.130410 confattr-0.9.1/docs/source/examples/env/test_example.py
+-rw-r--r--   0        0        0        0 2023-03-06 17:56:18.040410 confattr-0.9.1/docs/source/examples/generating_help/__init__.py
+-rwxr-xr-x   0        0        0      683 2023-03-06 17:56:18.040410 confattr-0.9.1/docs/source/examples/generating_help/example.py
+-rwxr-xr-x   0        0        0      310 2023-03-06 17:56:18.130410 confattr-0.9.1/docs/source/examples/generating_help/example_config.py
+-rwxr-xr-x   0        0        0      390 2023-03-06 17:56:18.130410 confattr-0.9.1/docs/source/examples/generating_help/example_raw_config.py
+-rwxr-xr-x   0        0        0      336 2023-03-06 17:56:18.130410 confattr-0.9.1/docs/source/examples/generating_help/example_raw_help.py
+-rw-r--r--   0        0        0     1129 2023-03-06 17:56:18.280410 confattr-0.9.1/docs/source/examples/generating_help/expected-config
+-rw-r--r--   0        0        0      601 2023-03-06 17:56:18.280410 confattr-0.9.1/docs/source/examples/generating_help/expected-no-multi-config
+-rw-r--r--   0        0        0     2540 2023-03-06 17:56:18.280410 confattr-0.9.1/docs/source/examples/generating_help/expected-no-multi-help.txt
+-rw-r--r--   0        0        0     1121 2023-03-06 17:56:18.280410 confattr-0.9.1/docs/source/examples/generating_help/expected-raw-config
+-rw-r--r--   0        0        0     3847 2023-03-06 17:56:18.180410 confattr-0.9.1/docs/source/examples/generating_help/expected-raw-help.txt
+-rwxr-xr-x   0        0        0      563 2023-03-06 17:56:18.280410 confattr-0.9.1/docs/source/examples/generating_help/no_multi_example.py
+-rwxr-xr-x   0        0        0      328 2023-03-06 17:56:18.280410 confattr-0.9.1/docs/source/examples/generating_help/no_multi_example_config.py
+-rw-r--r--   0        0        0     3989 2023-03-06 17:56:18.180410 confattr-0.9.1/docs/source/examples/generating_help/output.txt
+-rwxr-xr-x   0        0        0     3026 2023-03-06 17:56:18.280410 confattr-0.9.1/docs/source/examples/generating_help/test_example.py
+-rw-r--r--   0        0        0        0 2023-03-06 17:56:18.040410 confattr-0.9.1/docs/source/examples/include/__init__.py
+-rw-r--r--   0        0        0      261 2023-03-06 17:56:18.040410 confattr-0.9.1/docs/source/examples/include/config
+-rw-r--r--   0        0        0     4016 2023-03-06 17:56:18.230410 confattr-0.9.1/docs/source/examples/include/example.py
+-rw-r--r--   0        0        0       27 2023-03-06 17:56:18.040410 confattr-0.9.1/docs/source/examples/include/mirror
+-rw-r--r--   0        0        0      260 2023-03-06 17:56:18.040410 confattr-0.9.1/docs/source/examples/include/output.txt
+-rw-r--r--   0        0        0      436 2023-03-06 17:56:18.130410 confattr-0.9.1/docs/source/examples/include/test_example.py
+-rw-r--r--   0        0        0       24 2023-03-06 17:56:18.040410 confattr-0.9.1/docs/source/examples/include/two-way
+-rw-r--r--   0        0        0        0 2023-03-06 17:56:17.993744 confattr-0.9.1/docs/source/examples/map/__init__.py
+-rw-r--r--   0        0        0       54 2023-03-06 17:56:17.993744 confattr-0.9.1/docs/source/examples/map/config
+-rw-r--r--   0        0        0     2256 2023-03-06 17:56:18.230410 confattr-0.9.1/docs/source/examples/map/example.py
+-rw-r--r--   0        0        0      252 2023-03-06 17:56:18.040410 confattr-0.9.1/docs/source/examples/map/example_print_help.py
+-rw-r--r--   0        0        0      153 2023-03-06 17:56:17.997077 confattr-0.9.1/docs/source/examples/map/output_help.txt
+-rw-r--r--   0        0        0       21 2023-03-06 17:56:17.997077 confattr-0.9.1/docs/source/examples/map/requirements.txt
+-rw-r--r--   0        0        0      506 2023-03-06 17:56:18.130410 confattr-0.9.1/docs/source/examples/map/test_print_help.py
+-rw-r--r--   0        0        0        0 2023-03-06 17:56:17.997077 confattr-0.9.1/docs/source/examples/map_save/__init__.py
+-rw-r--r--   0        0        0      123 2023-03-06 18:52:22.073827 confattr-0.9.1/docs/source/examples/map_save/config
+-rw-r--r--   0        0        0      123 2023-03-06 17:56:18.283743 confattr-0.9.1/docs/source/examples/map_save/config_expected
+-rw-r--r--   0        0        0     1357 2023-03-06 17:56:18.133744 confattr-0.9.1/docs/source/examples/map_save/example_1.py
+-rw-r--r--   0        0        0     1780 2023-03-06 17:56:18.133744 confattr-0.9.1/docs/source/examples/map_save/example_3.py
+-rw-r--r--   0        0        0      939 2023-03-06 17:56:18.040410 confattr-0.9.1/docs/source/examples/map_save/test_example_3.py
+-rw-r--r--   0        0        0        0 2023-03-06 17:56:17.997077 confattr-0.9.1/docs/source/examples/multiconfig/__init__.py
+-rw-r--r--   0        0        0      100 2023-03-06 17:56:17.997077 confattr-0.9.1/docs/source/examples/multiconfig/config
+-rw-r--r--   0        0        0      122 2023-03-06 17:56:17.997077 confattr-0.9.1/docs/source/examples/multiconfig/config2
+-rw-r--r--   0        0        0      899 2023-03-06 17:56:18.230410 confattr-0.9.1/docs/source/examples/multiconfig/example.py
+-rw-r--r--   0        0        0       95 2023-03-06 17:56:17.997077 confattr-0.9.1/docs/source/examples/multiconfig/output.txt
+-rw-r--r--   0        0        0      125 2023-03-06 17:56:17.997077 confattr-0.9.1/docs/source/examples/multiconfig/output2.txt
+-rw-r--r--   0        0        0      942 2023-03-06 17:56:18.133744 confattr-0.9.1/docs/source/examples/multiconfig/test_example.py
+-rw-r--r--   0        0        0        0 2023-03-06 17:56:18.283743 confattr-0.9.1/docs/source/examples/multiconfig_reset/__init__.py
+-rw-r--r--   0        0        0      651 2023-03-06 17:56:18.283743 confattr-0.9.1/docs/source/examples/multiconfig_reset/example.py
+-rw-r--r--   0        0        0       29 2023-03-06 17:56:18.283743 confattr-0.9.1/docs/source/examples/multiconfig_reset/expected-config
+-rw-r--r--   0        0        0      780 2023-03-06 17:56:18.283743 confattr-0.9.1/docs/source/examples/multiconfig_reset/test_example.py
+-rw-r--r--   0        0        0        0 2023-03-06 17:56:17.997077 confattr-0.9.1/docs/source/examples/regex/__init__.py
+-rw-r--r--   0        0        0      811 2023-03-06 18:52:22.313827 confattr-0.9.1/docs/source/examples/regex/config
+-rw-r--r--   0        0        0     1144 2023-03-06 17:56:18.230410 confattr-0.9.1/docs/source/examples/regex/example.py
+-rw-r--r--   0        0        0      811 2023-03-06 17:56:18.230410 confattr-0.9.1/docs/source/examples/regex/expected-config
+-rw-r--r--   0        0        0     1002 2023-03-06 17:56:18.133744 confattr-0.9.1/docs/source/examples/regex/test_example.py
+-rw-r--r--   0        0        0        0 2023-03-06 17:56:18.133744 confattr-0.9.1/docs/source/examples/testing_monkeypatch_config/__init__.py
+-rw-r--r--   0        0        0     1164 2023-03-06 17:56:18.133744 confattr-0.9.1/docs/source/examples/testing_monkeypatch_config/example.py
+-rwxr-xr-x   0        0        0      256 2023-03-06 17:56:18.133744 confattr-0.9.1/docs/source/examples/testing_monkeypatch_config/test_example.py
+-rw-r--r--   0        0        0        0 2023-03-06 17:56:18.133744 confattr-0.9.1/docs/source/examples/testing_monkeypatch_multiconfig/__init__.py
+-rw-r--r--   0        0        0     1252 2023-03-06 17:56:18.133744 confattr-0.9.1/docs/source/examples/testing_monkeypatch_multiconfig/example.py
+-rwxr-xr-x   0        0        0      256 2023-03-06 17:56:18.133744 confattr-0.9.1/docs/source/examples/testing_monkeypatch_multiconfig/test_example.py
+-rw-r--r--   0        0        0        0 2023-03-06 17:56:18.133744 confattr-0.9.1/docs/source/examples/testing_tmp_path/__init__.py
+-rw-r--r--   0        0        0      299 2023-03-06 17:56:18.133744 confattr-0.9.1/docs/source/examples/testing_tmp_path/example.py
+-rw-r--r--   0        0        0      600 2023-03-06 17:56:18.133744 confattr-0.9.1/docs/source/examples/testing_tmp_path/test_example.py
+-rw-r--r--   0        0        0     2857 2023-03-06 18:53:55.087163 confattr-0.9.1/docs/source/index.rst
+-rw-r--r--   0        0        0    24838 2023-03-06 17:56:18.283743 confattr-0.9.1/docs/source/intro.rst
+-rw-r--r--   0        0        0       61 2023-03-06 17:56:17.883744 confattr-0.9.1/docs/source/modules.rst
+-rw-r--r--   0        0        0      456 2023-03-06 17:56:18.133744 confattr-0.9.1/mypy.ini
+-rw-r--r--   0        0        0     4135 2023-03-06 18:04:04.233755 confattr-0.9.1/prepare_for_gitlab_pages.py
+-rw-r--r--   0        0        0      819 2023-03-06 17:56:17.997077 confattr-0.9.1/pyproject.toml
+-rwxr-xr-x   0        0        0    13096 2023-03-06 18:53:55.087163 confattr-0.9.1/release.sh
+-rw-r--r--   0        0        0      224 2023-03-06 17:56:17.997077 confattr-0.9.1/requirements-py36.txt
+-rw-r--r--   0        0        0       56 2023-03-06 17:56:18.083743 confattr-0.9.1/requirements-release.txt
+-rw-r--r--   0        0        0      145 2023-03-06 18:53:55.087163 confattr-0.9.1/requirements-test.txt
+-rw-r--r--   0        0        0       17 2023-03-06 17:56:17.883744 confattr-0.9.1/requirements.txt
+-rw-r--r--   0        0        0      917 2023-03-06 18:53:55.090496 confattr-0.9.1/src/confattr/__init__.py
+-rw-r--r--   0        0        0    22394 2023-03-06 17:56:18.283743 confattr-0.9.1/src/confattr/config.py
+-rw-r--r--   0        0        0    63644 2023-03-06 17:56:18.283743 confattr-0.9.1/src/confattr/configfile.py
+-rw-r--r--   0        0        0        0 2022-11-21 06:04:24.790000 confattr-0.9.1/src/confattr/py.typed
+-rwxr-xr-x   0        0        0      142 2023-03-06 17:56:17.997077 confattr-0.9.1/src/confattr/runmodule.sh
+-rw-r--r--   0        0        0     2176 2023-03-06 17:56:17.883744 confattr-0.9.1/src/confattr/subprocess_pipe.py
+-rw-r--r--   0        0        0     7005 2023-03-06 17:56:18.233744 confattr-0.9.1/src/confattr/types.py
+-rw-r--r--   0        0        0    11553 2023-03-06 17:56:18.283743 confattr-0.9.1/src/confattr/utils.py
+-rwxr-xr-x   0        0        0    51173 2023-03-06 17:56:18.283743 confattr-0.9.1/tests/test_config.py
+-rwxr-xr-x   0        0        0     3971 2023-03-06 17:56:18.043743 confattr-0.9.1/tests/test_custom_commands.py
+-rw-r--r--   0        0        0     2714 2023-03-06 17:56:18.283743 confattr-0.9.1/tests/test_error.py
+-rwxr-xr-x   0        0        0     1168 2023-03-06 17:56:18.043743 confattr-0.9.1/tests/test_formatted_writer.py
+-rw-r--r--   0        0        0     1840 2023-03-06 17:56:18.233744 confattr-0.9.1/tests/test_message.py
+-rwxr-xr-x   0        0        0      971 2022-11-21 06:04:24.790000 confattr-0.9.1/tests/test_subprocess_pipe.py
+-rwxr-xr-x   0        0        0    14602 2023-03-06 17:56:18.233744 confattr-0.9.1/tests/test_utils.py
+-rw-r--r--   0        0        0      667 2023-03-06 18:53:55.090496 confattr-0.9.1/tox.ini
+-rw-r--r--   0        0        0      947 1970-01-01 00:00:00.000000 confattr-0.9.1/PKG-INFO
```

### Comparing `confattr-0.9.0/LICENSE` & `confattr-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `confattr-0.9.0/docs/Makefile` & `confattr-0.9.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `confattr-0.9.0/docs/build/html/_sources/index.rst.txt` & `confattr-0.9.1/docs/build/html/_sources/index.rst.txt`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
   Replace it with :python:`color = Config('color', 'red', allowed_values=['red', 'green', 'blue'])` and call :meth:`ConfigFile.load` (after the attribute has been created but before it's value is used).
   Then a user can create a config file in the :meth:`expected location <ConfigFile.iter_config_paths>` and can change the attribute with ``set color=green``.
   You don't need to change the usage of the attribute because :class:`Config` implements the `descriptor protocol <https://docs.python.org/3/reference/datamodel.html#implementing-descriptors>`_.
 - It is easy to add custom commands by subclassing :class:`ConfigFileCommand`. :ref:`[example] <exp-extend>`
 - It can be used to parse single lines, e.g. from a command line, too, with :meth:`ConfigFile.parse_line`.
 - It is well documented.
 - Includes an example for test automation. :ref:`[example] <exp-pytest>`
+- `Test coverage: 91% <coverage/index.html>`_
 
 
 Introduction and examples
 =========================
 
 .. toctree::
    :maxdepth: 2
```

### Comparing `confattr-0.9.0/docs/build/html/_sources/intro.rst.txt` & `confattr-0.9.1/docs/build/html/_sources/intro.rst.txt`

 * *Files identical despite different names*

### Comparing `confattr-0.9.0/docs/build/html/_static/_sphinx_javascript_frameworks_compat.js` & `confattr-0.9.1/docs/build/html/_static/_sphinx_javascript_frameworks_compat.js`

 * *Files identical despite different names*

### Comparing `confattr-0.9.0/docs/build/html/_static/basic.css` & `confattr-0.9.1/docs/build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `confattr-0.9.0/docs/build/html/_static/css/badge_only.css` & `confattr-0.9.1/docs/build/html/_static/css/badge_only.css`

 * *Files identical despite different names*

### Comparing `confattr-0.9.0/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff` & `confattr-0.9.1/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff`

 * *Files identical despite different names*

### Comparing `confattr-0.9.0/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff2` & `confattr-0.9.1/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff2`

 * *Files identical despite different names*

### Comparing `confattr-0.9.0/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff` & `confattr-0.9.1/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff`

 * *Files identical despite different names*

### Comparing `confattr-0.9.0/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff2` & `confattr-0.9.1/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff2`

 * *Files identical despite different names*

### Comparing `confattr-0.9.0/docs/build/html/_static/css/fonts/fontawesome-webfont.eot` & `confattr-0.9.1/docs/build/html/_static/css/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `confattr-0.9.0/docs/build/html/_static/css/fonts/fontawesome-webfont.svg` & `confattr-0.9.1/docs/build/html/_static/css/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `confattr-0.9.0/docs/build/html/_static/css/fonts/fontawesome-webfont.ttf` & `confattr-0.9.1/docs/build/html/_static/css/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `confattr-0.9.0/docs/build/html/_static/css/fonts/fontawesome-webfont.woff` & `confattr-0.9.1/docs/build/html/_static/css/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `confattr-0.9.0/docs/build/html/_static/css/fonts/fontawesome-webfont.woff2` & `confattr-0.9.1/docs/build/html/_static/css/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `confattr-0.9.0/docs/build/html/_static/css/fonts/lato-bold-italic.woff` & `confattr-0.9.1/docs/build/html/_static/css/fonts/lato-bold-italic.woff`

 * *Files identical despite different names*

### Comparing `confattr-0.9.0/docs/build/html/_static/css/fonts/lato-bold-italic.woff2` & `confattr-0.9.1/docs/build/html/_static/css/fonts/lato-bold-italic.woff2`

 * *Files identical despite different names*

### Comparing `confattr-0.9.0/docs/build/html/_static/css/fonts/lato-bold.woff` & `confattr-0.9.1/docs/build/html/_static/css/fonts/lato-bold.woff`

 * *Files identical despite different names*

### Comparing `confattr-0.9.0/docs/build/html/_static/css/fonts/lato-bold.woff2` & `confattr-0.9.1/docs/build/html/_static/css/fonts/lato-bold.woff2`

 * *Files identical despite different names*

### Comparing `confattr-0.9.0/docs/build/html/_static/css/fonts/lato-normal-italic.woff` & `confattr-0.9.1/docs/build/html/_static/css/fonts/lato-normal-italic.woff`

 * *Files identical despite different names*

### Comparing `confattr-0.9.0/docs/build/html/_static/css/fonts/lato-normal-italic.woff2` & `confattr-0.9.1/docs/build/html/_static/css/fonts/lato-normal-italic.woff2`

 * *Files identical despite different names*

### Comparing `confattr-0.9.0/docs/build/html/_static/css/fonts/lato-normal.woff` & `confattr-0.9.1/docs/build/html/_static/css/fonts/lato-normal.woff`

 * *Files identical despite different names*

### Comparing `confattr-0.9.0/docs/build/html/_static/css/fonts/lato-normal.woff2` & `confattr-0.9.1/docs/build/html/_static/css/fonts/lato-normal.woff2`

 * *Files identical despite different names*

### Comparing `confattr-0.9.0/docs/build/html/_static/css/theme.css` & `confattr-0.9.1/docs/build/html/_static/css/theme.css`

 * *Files identical despite different names*

### Comparing `confattr-0.9.0/docs/build/html/_static/doctools.js` & `confattr-0.9.1/docs/build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `confattr-0.9.0/docs/build/html/_static/jquery-3.6.0.js` & `confattr-0.9.1/docs/build/html/_static/jquery-3.6.0.js`

 * *Files identical despite different names*

### Comparing `confattr-0.9.0/docs/build/html/_static/jquery.js` & `confattr-0.9.1/docs/build/html/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `confattr-0.9.0/docs/build/html/_static/js/badge_only.js` & `confattr-0.9.1/docs/build/html/_static/js/badge_only.js`

 * *Files identical despite different names*

### Comparing `confattr-0.9.0/docs/build/html/_static/js/html5shiv-printshiv.min.js` & `confattr-0.9.1/docs/build/html/_static/js/html5shiv-printshiv.min.js`

 * *Files identical despite different names*

### Comparing `confattr-0.9.0/docs/build/html/_static/js/html5shiv.min.js` & `confattr-0.9.1/docs/build/html/_static/js/html5shiv.min.js`

 * *Files identical despite different names*

### Comparing `confattr-0.9.0/docs/build/html/_static/js/theme.js` & `confattr-0.9.1/docs/build/html/_static/js/theme.js`

 * *Files identical despite different names*

### Comparing `confattr-0.9.0/docs/build/html/_static/language_data.js` & `confattr-0.9.1/docs/build/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `confattr-0.9.0/docs/build/html/_static/nature.css` & `confattr-0.9.1/docs/build/html/_static/nature.css`

 * *Files identical despite different names*

### Comparing `confattr-0.9.0/docs/build/html/_static/pygments.css` & `confattr-0.9.1/docs/build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `confattr-0.9.0/docs/build/html/_static/searchtools.js` & `confattr-0.9.1/docs/build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `confattr-0.9.0/docs/build/html/_static/sphinx_highlight.js` & `confattr-0.9.1/docs/build/html/_static/sphinx_highlight.js`

 * *Files identical despite different names*

### Comparing `confattr-0.9.0/docs/build/html/_static/underscore-1.13.1.js` & `confattr-0.9.1/docs/build/html/_static/underscore-1.13.1.js`

 * *Files identical despite different names*

### Comparing `confattr-0.9.0/docs/build/html/_static/underscore.js` & `confattr-0.9.1/docs/build/html/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `confattr-0.9.0/docs/build/html/confattr.config.html` & `confattr-0.9.1/docs/build/html/confattr.config.html`

 * *Files identical despite different names*

### Comparing `confattr-0.9.0/docs/build/html/confattr.configfile.html` & `confattr-0.9.1/docs/build/html/confattr.configfile.html`

 * *Files identical despite different names*

### Comparing `confattr-0.9.0/docs/build/html/confattr.html` & `confattr-0.9.1/docs/build/html/confattr.html`

 * *Files identical despite different names*

### Comparing `confattr-0.9.0/docs/build/html/confattr.subprocess_pipe.html` & `confattr-0.9.1/docs/build/html/confattr.subprocess_pipe.html`

 * *Files identical despite different names*

### Comparing `confattr-0.9.0/docs/build/html/confattr.types.html` & `confattr-0.9.1/docs/build/html/confattr.types.html`

 * *Files identical despite different names*

### Comparing `confattr-0.9.0/docs/build/html/confattr.utils.html` & `confattr-0.9.1/docs/build/html/confattr.utils.html`

 * *Files identical despite different names*

### Comparing `confattr-0.9.0/docs/build/html/genindex.html` & `confattr-0.9.1/docs/build/html/genindex.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" />
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Index &mdash; confattr v0.9.0 documentation</title>
+  <title>Index &mdash; confattr v0.9.1 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
       <link rel="stylesheet" href="_static/sphinx_paramlinks.css" type="text/css" />
       <link rel="stylesheet" href="_static/no-ligatures-in-code.css" type="text/css" />
       <link rel="stylesheet" href="_static/tab-size.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="_static/js/html5shiv.min.js"></script>
@@ -30,15 +30,15 @@
 
           
           
           <a href="index.html" class="icon icon-home">
             confattr
           </a>
               <div class="version">
-                v0.9.0
+                v0.9.1
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
```

#### html2text {}

```diff
@@ -3,15 +3,15 @@
 
 
 
 
 
 
 confattr
-v0.9.0
+v0.9.1
 [q                   ]
     * Introduction_and_examples
     * confattr_package
     * confattr.config_module
     * confattr.configfile_module
     * confattr.subprocess_pipe_module
     * confattr.types_module
```

### Comparing `confattr-0.9.0/docs/build/html/index.html` & `confattr-0.9.1/docs/build/html/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Welcome to confattr’s documentation &mdash; confattr v0.9.0 documentation</title>
+  <title>Welcome to confattr’s documentation &mdash; confattr v0.9.1 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
       <link rel="stylesheet" href="_static/sphinx_paramlinks.css" type="text/css" />
       <link rel="stylesheet" href="_static/no-ligatures-in-code.css" type="text/css" />
       <link rel="stylesheet" href="_static/tab-size.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="_static/js/html5shiv.min.js"></script>
@@ -32,15 +32,15 @@
 
           
           
           <a href="#" class="icon icon-home">
             confattr
           </a>
               <div class="version">
-                v0.9.0
+                v0.9.1
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
@@ -96,14 +96,15 @@
 Replace it with <code class="code highlight python docutils literal highlight-python"><span class="n">color</span> <span class="o">=</span> <span class="n">Config</span><span class="p">(</span><span class="s1">&#39;color&#39;</span><span class="p">,</span> <span class="s1">&#39;red&#39;</span><span class="p">,</span> <span class="n">allowed_values</span><span class="o">=</span><span class="p">[</span><span class="s1">&#39;red&#39;</span><span class="p">,</span> <span class="s1">&#39;green&#39;</span><span class="p">,</span> <span class="s1">&#39;blue&#39;</span><span class="p">])</span></code> and call <a class="reference internal" href="confattr.html#confattr.ConfigFile.load" title="confattr.ConfigFile.load"><code class="xref py py-meth docutils literal notranslate"><span class="pre">ConfigFile.load()</span></code></a> (after the attribute has been created but before it’s value is used).
 Then a user can create a config file in the <a class="reference internal" href="confattr.html#confattr.ConfigFile.iter_config_paths" title="confattr.ConfigFile.iter_config_paths"><code class="xref py py-meth docutils literal notranslate"><span class="pre">expected</span> <span class="pre">location</span></code></a> and can change the attribute with <code class="docutils literal notranslate"><span class="pre">set</span> <span class="pre">color=green</span></code>.
 You don’t need to change the usage of the attribute because <a class="reference internal" href="confattr.html#confattr.Config" title="confattr.Config"><code class="xref py py-class docutils literal notranslate"><span class="pre">Config</span></code></a> implements the <a class="reference external" href="https://docs.python.org/3/reference/datamodel.html#implementing-descriptors">descriptor protocol</a>.</p></li>
 <li><p>It is easy to add custom commands by subclassing <a class="reference internal" href="confattr.html#confattr.ConfigFileCommand" title="confattr.ConfigFileCommand"><code class="xref py py-class docutils literal notranslate"><span class="pre">ConfigFileCommand</span></code></a>. <a class="reference internal" href="intro.html#exp-extend"><span class="std std-ref">[example]</span></a></p></li>
 <li><p>It can be used to parse single lines, e.g. from a command line, too, with <a class="reference internal" href="confattr.html#confattr.ConfigFile.parse_line" title="confattr.ConfigFile.parse_line"><code class="xref py py-meth docutils literal notranslate"><span class="pre">ConfigFile.parse_line()</span></code></a>.</p></li>
 <li><p>It is well documented.</p></li>
 <li><p>Includes an example for test automation. <a class="reference internal" href="intro.html#exp-pytest"><span class="std std-ref">[example]</span></a></p></li>
+<li><p><a class="reference external" href="coverage/index.html">Test coverage: 91%</a></p></li>
 </ul>
 <section id="introduction-and-examples">
 <h2>Introduction and examples<a class="headerlink" href="#introduction-and-examples" title="Permalink to this heading"></a></h2>
 <div class="toctree-wrapper compound">
 <ul>
 <li class="toctree-l1"><a class="reference internal" href="intro.html">Introduction and examples</a><ul>
 <li class="toctree-l2"><a class="reference internal" href="intro.html#config-and-configfile">Config and ConfigFile</a></li>
```

#### html2text {}

```diff
@@ -4,15 +4,15 @@
 
 
 
 
 
 
 confattr
-v0.9.0
+v0.9.1
 [q                   ]
     * Introduction_and_examples
     * confattr_package
     * confattr.config_module
     * confattr.configfile_module
     * confattr.subprocess_pipe_module
     * confattr.types_module
@@ -43,14 +43,15 @@
       usage of the attribute because Config implements the descriptor_protocol.
     * It is easy to add custom commands by subclassing ConfigFileCommand.
       [example]
     * It can be used to parse single lines, e.g. from a command line, too, with
       ConfigFile.parse_line().
     * It is well documented.
     * Includes an example for test automation. [example]
+    * Test_coverage:_91%
 ***** Introduction and examplesï *****
     * Introduction_and_examples
           o Config_and_ConfigFile
           o Config_file_syntax
           o Different_values_for_different_objects
           o MultiConfig.reset
           o Include
```

### Comparing `confattr-0.9.0/docs/build/html/intro.html` & `confattr-0.9.1/docs/build/html/intro.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Introduction and examples &mdash; confattr v0.9.0 documentation</title>
+  <title>Introduction and examples &mdash; confattr v0.9.1 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
       <link rel="stylesheet" href="_static/sphinx_paramlinks.css" type="text/css" />
       <link rel="stylesheet" href="_static/no-ligatures-in-code.css" type="text/css" />
       <link rel="stylesheet" href="_static/tab-size.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="_static/js/html5shiv.min.js"></script>
@@ -33,15 +33,15 @@
 
           
           
           <a href="index.html" class="icon icon-home">
             confattr
           </a>
               <div class="version">
-                v0.9.0
+                v0.9.1
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
```

#### html2text {}

```diff
@@ -5,15 +5,15 @@
 
 
 
 
 
 
 confattr
-v0.9.0
+v0.9.1
 [q                   ]
     * Introduction_and_examples
           o Config_and_ConfigFile
           o Config_file_syntax
           o Different_values_for_different_objects
           o MultiConfig.reset
           o Include
```

### Comparing `confattr-0.9.0/docs/build/html/modules.html` & `confattr-0.9.1/docs/build/html/modules.html`

 * *Files identical despite different names*

### Comparing `confattr-0.9.0/docs/build/html/objects.inv` & `confattr-0.9.1/docs/build/html/objects.inv`

 * *Files identical despite different names*

### Comparing `confattr-0.9.0/docs/build/html/py-modindex.html` & `confattr-0.9.1/docs/build/html/py-modindex.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" />
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Python Module Index &mdash; confattr v0.9.0 documentation</title>
+  <title>Python Module Index &mdash; confattr v0.9.1 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
       <link rel="stylesheet" href="_static/sphinx_paramlinks.css" type="text/css" />
       <link rel="stylesheet" href="_static/no-ligatures-in-code.css" type="text/css" />
       <link rel="stylesheet" href="_static/tab-size.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="_static/js/html5shiv.min.js"></script>
@@ -33,15 +33,15 @@
 
           
           
           <a href="index.html" class="icon icon-home">
             confattr
           </a>
               <div class="version">
-                v0.9.0
+                v0.9.1
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
```

#### html2text {}

```diff
@@ -3,15 +3,15 @@
 
 
 
 
 
 
 confattr
-v0.9.0
+v0.9.1
 [q                   ]
     * Introduction_and_examples
     * confattr_package
     * confattr.config_module
     * confattr.configfile_module
     * confattr.subprocess_pipe_module
     * confattr.types_module
```

### Comparing `confattr-0.9.0/docs/build/html/search.html` & `confattr-0.9.1/docs/build/html/search.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" />
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Search &mdash; confattr v0.9.0 documentation</title>
+  <title>Search &mdash; confattr v0.9.1 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
       <link rel="stylesheet" href="_static/sphinx_paramlinks.css" type="text/css" />
       <link rel="stylesheet" href="_static/no-ligatures-in-code.css" type="text/css" />
       <link rel="stylesheet" href="_static/tab-size.css" type="text/css" />
     
   <!--[if lt IE 9]>
@@ -33,15 +33,15 @@
 
           
           
           <a href="index.html" class="icon icon-home">
             confattr
           </a>
               <div class="version">
-                v0.9.0
+                v0.9.1
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="#" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
```

#### html2text {}

```diff
@@ -3,15 +3,15 @@
 
 
 
 
 
 
 confattr
-v0.9.0
+v0.9.1
 [q                   ]
     * Introduction_and_examples
     * confattr_package
     * confattr.config_module
     * confattr.configfile_module
     * confattr.subprocess_pipe_module
     * confattr.types_module
```

### Comparing `confattr-0.9.0/docs/make.bat` & `confattr-0.9.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `confattr-0.9.0/docs/source/conf.py` & `confattr-0.9.1/docs/source/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 
 project = 'confattr'
 copyright = '2022, erzo'
 author = 'erzo'
-release = 'v0.9.0'
+release = 'v0.9.1'
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = ['sphinx.ext.autodoc', 'sphinx.ext.intersphinx', 'sphinx_paramlinks']
 
 templates_path = ['_templates']
```

### Comparing `confattr-0.9.0/docs/source/examples/config_and_configfile/example.py` & `confattr-0.9.1/docs/source/examples/config_and_configfile/example.py`

 * *Files identical despite different names*

### Comparing `confattr-0.9.0/docs/source/examples/config_and_configfile/expected-config` & `confattr-0.9.1/docs/source/examples/config_and_configfile/expected-config`

 * *Files identical despite different names*

### Comparing `confattr-0.9.0/docs/source/examples/config_and_configfile/exported-config` & `confattr-0.9.1/docs/source/examples/config_and_configfile/exported-config`

 * *Files identical despite different names*

### Comparing `confattr-0.9.0/docs/source/examples/config_and_configfile/test_example.py` & `confattr-0.9.1/docs/source/examples/config_and_configfile/test_example.py`

 * *Files identical despite different names*

### Comparing `confattr-0.9.0/docs/source/examples/custom_set/example.py` & `confattr-0.9.1/docs/source/examples/custom_set/example.py`

 * *Files identical despite different names*

### Comparing `confattr-0.9.0/docs/source/examples/custom_set/example_save.py` & `confattr-0.9.1/docs/source/examples/custom_set/example_save.py`

 * *Files identical despite different names*

### Comparing `confattr-0.9.0/docs/source/examples/custom_set/test_example.py` & `confattr-0.9.1/docs/source/examples/custom_set/test_example.py`

 * *Files identical despite different names*

### Comparing `confattr-0.9.0/docs/source/examples/generating_help/example.py` & `confattr-0.9.1/docs/source/examples/generating_help/example.py`

 * *Files identical despite different names*

### Comparing `confattr-0.9.0/docs/source/examples/generating_help/expected-config` & `confattr-0.9.1/docs/source/examples/generating_help/expected-config`

 * *Files identical despite different names*

### Comparing `confattr-0.9.0/docs/source/examples/generating_help/expected-no-multi-config` & `confattr-0.9.1/docs/source/examples/generating_help/expected-no-multi-config`

 * *Files identical despite different names*

### Comparing `confattr-0.9.0/docs/source/examples/generating_help/expected-no-multi-help.txt` & `confattr-0.9.1/docs/source/examples/generating_help/expected-no-multi-help.txt`

 * *Files identical despite different names*

### Comparing `confattr-0.9.0/docs/source/examples/generating_help/expected-raw-config` & `confattr-0.9.1/docs/source/examples/generating_help/expected-raw-config`

 * *Files identical despite different names*

### Comparing `confattr-0.9.0/docs/source/examples/generating_help/expected-raw-help.txt` & `confattr-0.9.1/docs/source/examples/generating_help/expected-raw-help.txt`

 * *Files identical despite different names*

### Comparing `confattr-0.9.0/docs/source/examples/generating_help/no_multi_example.py` & `confattr-0.9.1/docs/source/examples/generating_help/no_multi_example.py`

 * *Files identical despite different names*

### Comparing `confattr-0.9.0/docs/source/examples/generating_help/output.txt` & `confattr-0.9.1/docs/source/examples/generating_help/output.txt`

 * *Files identical despite different names*

### Comparing `confattr-0.9.0/docs/source/examples/generating_help/test_example.py` & `confattr-0.9.1/docs/source/examples/generating_help/test_example.py`

 * *Files identical despite different names*

### Comparing `confattr-0.9.0/docs/source/examples/include/example.py` & `confattr-0.9.1/docs/source/examples/include/example.py`

 * *Files identical despite different names*

### Comparing `confattr-0.9.0/docs/source/examples/map/example.py` & `confattr-0.9.1/docs/source/examples/map/example.py`

 * *Files identical despite different names*

### Comparing `confattr-0.9.0/docs/source/examples/map_save/example_1.py` & `confattr-0.9.1/docs/source/examples/map_save/example_1.py`

 * *Files identical despite different names*

### Comparing `confattr-0.9.0/docs/source/examples/map_save/example_3.py` & `confattr-0.9.1/docs/source/examples/map_save/example_3.py`

 * *Files identical despite different names*

### Comparing `confattr-0.9.0/docs/source/examples/map_save/test_example_3.py` & `confattr-0.9.1/docs/source/examples/map_save/test_example_3.py`

 * *Files identical despite different names*

### Comparing `confattr-0.9.0/docs/source/examples/multiconfig/example.py` & `confattr-0.9.1/docs/source/examples/multiconfig/example.py`

 * *Files identical despite different names*

### Comparing `confattr-0.9.0/docs/source/examples/multiconfig/test_example.py` & `confattr-0.9.1/docs/source/examples/multiconfig/test_example.py`

 * *Files identical despite different names*

### Comparing `confattr-0.9.0/docs/source/examples/multiconfig_reset/example.py` & `confattr-0.9.1/docs/source/examples/multiconfig_reset/example.py`

 * *Files identical despite different names*

### Comparing `confattr-0.9.0/docs/source/examples/multiconfig_reset/test_example.py` & `confattr-0.9.1/docs/source/examples/multiconfig_reset/test_example.py`

 * *Files identical despite different names*

### Comparing `confattr-0.9.0/docs/source/examples/regex/config` & `confattr-0.9.1/docs/source/examples/regex/config`

 * *Files identical despite different names*

### Comparing `confattr-0.9.0/docs/source/examples/regex/example.py` & `confattr-0.9.1/docs/source/examples/regex/example.py`

 * *Files identical despite different names*

### Comparing `confattr-0.9.0/docs/source/examples/regex/expected-config` & `confattr-0.9.1/docs/source/examples/regex/expected-config`

 * *Files identical despite different names*

### Comparing `confattr-0.9.0/docs/source/examples/regex/test_example.py` & `confattr-0.9.1/docs/source/examples/regex/test_example.py`

 * *Files identical despite different names*

### Comparing `confattr-0.9.0/docs/source/examples/testing_monkeypatch_config/example.py` & `confattr-0.9.1/docs/source/examples/testing_monkeypatch_config/example.py`

 * *Files identical despite different names*

### Comparing `confattr-0.9.0/docs/source/examples/testing_monkeypatch_multiconfig/example.py` & `confattr-0.9.1/docs/source/examples/testing_monkeypatch_multiconfig/example.py`

 * *Files identical despite different names*

### Comparing `confattr-0.9.0/docs/source/examples/testing_tmp_path/test_example.py` & `confattr-0.9.1/docs/source/examples/testing_tmp_path/test_example.py`

 * *Files identical despite different names*

### Comparing `confattr-0.9.0/docs/source/index.rst` & `confattr-0.9.1/docs/source/index.rst`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
   Replace it with :python:`color = Config('color', 'red', allowed_values=['red', 'green', 'blue'])` and call :meth:`ConfigFile.load` (after the attribute has been created but before it's value is used).
   Then a user can create a config file in the :meth:`expected location <ConfigFile.iter_config_paths>` and can change the attribute with ``set color=green``.
   You don't need to change the usage of the attribute because :class:`Config` implements the `descriptor protocol <https://docs.python.org/3/reference/datamodel.html#implementing-descriptors>`_.
 - It is easy to add custom commands by subclassing :class:`ConfigFileCommand`. :ref:`[example] <exp-extend>`
 - It can be used to parse single lines, e.g. from a command line, too, with :meth:`ConfigFile.parse_line`.
 - It is well documented.
 - Includes an example for test automation. :ref:`[example] <exp-pytest>`
+- `Test coverage: 91% <coverage/index.html>`_
 
 
 Introduction and examples
 =========================
 
 .. toctree::
    :maxdepth: 2
```

### Comparing `confattr-0.9.0/docs/source/intro.rst` & `confattr-0.9.1/docs/source/intro.rst`

 * *Files identical despite different names*

### Comparing `confattr-0.9.0/prepare_for_gitlab_pages.py` & `confattr-0.9.1/prepare_for_gitlab_pages.py`

 * *Files identical despite different names*

### Comparing `confattr-0.9.0/pyproject.toml` & `confattr-0.9.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `confattr-0.9.0/release.sh` & `confattr-0.9.1/release.sh`

 * *Files 2% similar despite different names*

```diff
@@ -303,56 +303,70 @@
 if [ "$update_venv" = 'true' ]; then
 	exit
 fi
 
 
 # ---------- run tests ----------
 
+COVERAGE_HTML_OUTPUT_PATH=htmlcov
 if [ "$run_tests" = "true" ]; then
 	tox_exit_code=0
-	tox || tox_exit_code=$?
+	if [ -e "$COVERAGE_HTML_OUTPUT_PATH" ]; then
+		rm -r "$COVERAGE_HTML_OUTPUT_PATH"
+	fi
+	tox -e py36,cov || tox_exit_code=$?
 
 	if [ "$tox_exit_code" = 2 -a "$has_downloaded_dependencies" != 'true' ]; then
 		echo
 		echo "tox failed with return code $tox_exit_code"
 		echo "try ./release.sh --update-venv"
 		exit $tox_exit_code
 	elif [ "$tox_exit_code" != "0" ]; then
 		exit $tox_exit_code
 	fi
+
+	test_coverage="$(.tox/cov/bin/coverage report | sed -En 's/TOTAL.* ([0-9]+%)/\1/p')"
 fi
 
 
 # ---------- build wheel ----------
 
 if [ "$only_build_wheel" = 'true' ]; then
 	flit build
 	exit
 fi
 
 
 # ---------- build documentation ----------
 
+DOCS_BUILD_COVERAGE='docs/build/html/coverage'
+
 fn_tag="tag"
 fn_version="src/confattr/__init__.py"
 
 branchname="$(git branch | sed -En 's/^\* (.*)$/\1/p')"
 lastversion="$(git tag --list 'v*' --sort=version:refname | tail -1)"
 newversion="$(increment_version "$lastversion")"
 
 
 if [ "$build_doc" = 'true' ]; then
 	echo "${color_cmd}running sphinx$color_reset"
 	if [ "$dont_publish" = 'true' ]; then
 		newversion="$lastversion-dev"
+		if [ "${test_coverage:-}" = '' ]; then
+			test_coverage='xxx%'
+		fi
 	else
 		echo "Make sure none of the files is opened anymore (to make sure that there are no unsaved changes)"
 		check_clean
 	fi
 
+	# update test coverage
+	sed -Ei "s/Test coverage: .*%/Test coverage: $test_coverage/" 'docs/source/index.rst'
+
 	# update version number
 	echo "setting version in documentation to $newversion"
 	sed -Ei "s/(release = ')[^']*(')/\\1$newversion\\2/" 'docs/source/conf.py'
 
 	# update table of contents
 	modules="$(find src/confattr/ -name '*.py' -type f | sed -E 's:src/confattr/(.*)\.py:confattr.\1:' | sed 's:/:.:g' | sed 's/confattr.__init__/confattr/' | sed 's/^/   /' | sort)"
 	newline="$(printf '\n ')"  # the space is required to protect the newline. it does not seem to be inserted into the file.
@@ -360,14 +374,19 @@
 	sed -i "/^Reference/,/^[A-Z]/ { /^\.\. toctree::/,/^$/ { /^$/a \\${modules//$newline/\\$newline}$newline} }" 'docs/source/index.rst'
 
 	# build documentation
 	sphinx-apidoc --separate -o 'docs/source' 'src/confattr'
 	sphinx-build -M html 'docs/source' 'docs/build'
 
 	if [ "$dont_publish" != 'true' ]; then
+		if [ -e "$DOCS_BUILD_COVERAGE" ]; then
+			rm -r "$DOCS_BUILD_COVERAGE"
+		fi
+		cp -r "$COVERAGE_HTML_OUTPUT_PATH" "$DOCS_BUILD_COVERAGE"
+		rm "$DOCS_BUILD_COVERAGE/.gitignore"
 		git add docs
 		if ! ask_yes_no 'Commit the new build of the html documentation?'; then
 			exit 0
 		fi
 		git commit --allow-empty --message 'updated html docs'
 	fi
 fi
```

### Comparing `confattr-0.9.0/src/confattr/__init__.py` & `confattr-0.9.1/src/confattr/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 '''
 Config Attributes
 
 A python library to read and write config files
 with a syntax inspired by vimrc and ranger config.
 '''
 
-__version__ = '0.9.0'
+__version__ = '0.9.1'
 
 from .config import *
 from .configfile import *
 
 __all__ = [
 	# -------- for normal usage -------
 	# imported from config
```

### Comparing `confattr-0.9.0/src/confattr/config.py` & `confattr-0.9.1/src/confattr/config.py`

 * *Files identical despite different names*

### Comparing `confattr-0.9.0/src/confattr/configfile.py` & `confattr-0.9.1/src/confattr/configfile.py`

 * *Files identical despite different names*

### Comparing `confattr-0.9.0/src/confattr/subprocess_pipe.py` & `confattr-0.9.1/src/confattr/subprocess_pipe.py`

 * *Files identical despite different names*

### Comparing `confattr-0.9.0/src/confattr/types.py` & `confattr-0.9.1/src/confattr/types.py`

 * *Files identical despite different names*

### Comparing `confattr-0.9.0/src/confattr/utils.py` & `confattr-0.9.1/src/confattr/utils.py`

 * *Files identical despite different names*

### Comparing `confattr-0.9.0/tests/test_config.py` & `confattr-0.9.1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `confattr-0.9.0/tests/test_custom_commands.py` & `confattr-0.9.1/tests/test_custom_commands.py`

 * *Files identical despite different names*

### Comparing `confattr-0.9.0/tests/test_error.py` & `confattr-0.9.1/tests/test_error.py`

 * *Files identical despite different names*

### Comparing `confattr-0.9.0/tests/test_formatted_writer.py` & `confattr-0.9.1/tests/test_formatted_writer.py`

 * *Files identical despite different names*

### Comparing `confattr-0.9.0/tests/test_message.py` & `confattr-0.9.1/tests/test_message.py`

 * *Files identical despite different names*

### Comparing `confattr-0.9.0/tests/test_subprocess_pipe.py` & `confattr-0.9.1/tests/test_subprocess_pipe.py`

 * *Files identical despite different names*

### Comparing `confattr-0.9.0/tests/test_utils.py` & `confattr-0.9.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `confattr-0.9.0/tox.ini` & `confattr-0.9.1/tox.ini`

 * *Files 21% similar despite different names*

```diff
@@ -16,7 +16,14 @@
     pudb
     py3: mypy>=1.0.1
     py3: types-appdirs
 commands =
     py3: mypy
     pytest {posargs}
 install_command = python -m pip install {opts} --no-index --find-links .package-store {packages}
+
+[testenv:cov]
+deps =
+	{[testenv]deps}
+	pytest-cov
+commands =
+	pytest --cov=confattr --cov-report=html {posargs}
```

### Comparing `confattr-0.9.0/PKG-INFO` & `confattr-0.9.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: confattr
-Version: 0.9.0
+Version: 0.9.1
 Summary: Config Attributes
 Author-email: erzo <erzo@posteo.de>
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Developers
 Classifier: Typing :: Typed
```

