# Comparing `tmp/SomeTools-0.1.39.tar.gz` & `tmp/SomeTools-0.1.40.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SomeTools-0.1.39.tar", last modified: Thu May 26 03:33:41 2022, max compression
+gzip compressed data, was "SomeTools-0.1.40.tar", last modified: Sat Jun 10 15:59:48 2023, max compression
```

## Comparing `SomeTools-0.1.39.tar` & `SomeTools-0.1.40.tar`

### file list

```diff
@@ -1,74 +1,82 @@
-drwxrwxrwx   0        0        0        0 2022-05-26 03:33:41.512000 SomeTools-0.1.39/
--rw-rw-rw-   0        0        0     1091 2022-01-04 06:56:33.000000 SomeTools-0.1.39/LICENSE
--rw-rw-rw-   0        0        0    52772 2022-05-26 03:33:41.511000 SomeTools-0.1.39/PKG-INFO
--rw-rw-rw-   0        0        0    52033 2022-05-26 03:30:56.000000 SomeTools-0.1.39/README.md
-drwxrwxrwx   0        0        0        0 2022-05-26 03:33:41.494000 SomeTools-0.1.39/SomeTools.egg-info/
--rw-rw-rw-   0        0        0    52772 2022-05-26 03:33:41.000000 SomeTools-0.1.39/SomeTools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2127 2022-05-26 03:33:41.000000 SomeTools-0.1.39/SomeTools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-05-26 03:33:41.000000 SomeTools-0.1.39/SomeTools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      167 2022-05-26 03:33:41.000000 SomeTools-0.1.39/SomeTools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2022-05-26 03:33:41.000000 SomeTools-0.1.39/SomeTools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-05-26 03:33:41.513000 SomeTools-0.1.39/setup.cfg
--rw-rw-rw-   0        0        0     2144 2022-05-26 03:33:29.000000 SomeTools-0.1.39/setup.py
-drwxrwxrwx   0        0        0        0 2022-05-26 03:33:41.495000 SomeTools-0.1.39/sometools/
--rw-rw-rw-   0        0        0     1304 2022-05-26 03:21:40.000000 SomeTools-0.1.39/sometools/__init__.py
-drwxrwxrwx   0        0        0        0 2022-05-26 03:33:41.495000 SomeTools-0.1.39/sometools/async_tools/
--rw-rw-rw-   0        0        0      550 2022-03-07 02:13:15.000000 SomeTools-0.1.39/sometools/async_tools/__init__.py
-drwxrwxrwx   0        0        0        0 2022-05-26 03:33:41.496000 SomeTools-0.1.39/sometools/async_tools/base/
--rw-rw-rw-   0        0        0       42 2022-01-04 06:56:33.000000 SomeTools-0.1.39/sometools/async_tools/base/__init__.py
--rw-rw-rw-   0        0        0      181 2022-01-04 06:56:33.000000 SomeTools-0.1.39/sometools/async_tools/base/base.py
-drwxrwxrwx   0        0        0        0 2022-05-26 03:33:41.497000 SomeTools-0.1.39/sometools/async_tools/bloom_filter/
--rw-rw-rw-   0        0        0       90 2022-01-04 06:56:33.000000 SomeTools-0.1.39/sometools/async_tools/bloom_filter/__init__.py
--rw-rw-rw-   0        0        0     3632 2022-03-08 06:14:11.000000 SomeTools-0.1.39/sometools/async_tools/bloom_filter/async_bloomfilter_tool.py
-drwxrwxrwx   0        0        0        0 2022-05-26 03:33:41.497000 SomeTools-0.1.39/sometools/async_tools/database_tools/
--rw-rw-rw-   0        0        0        0 2022-03-07 01:58:48.000000 SomeTools-0.1.39/sometools/async_tools/database_tools/__init__.py
-drwxrwxrwx   0        0        0        0 2022-05-26 03:33:41.498000 SomeTools-0.1.39/sometools/async_tools/database_tools/mysql_tools/
--rw-rw-rw-   0        0        0        0 2022-03-07 01:59:04.000000 SomeTools-0.1.39/sometools/async_tools/database_tools/mysql_tools/__init__.py
--rw-rw-rw-   0        0        0    14159 2022-03-08 06:10:51.000000 SomeTools-0.1.39/sometools/async_tools/database_tools/mysql_tools/async_mysql_orm.py
-drwxrwxrwx   0        0        0        0 2022-05-26 03:33:41.499000 SomeTools-0.1.39/sometools/async_tools/redis_tools/
--rw-rw-rw-   0        0        0       78 2022-01-04 06:56:33.000000 SomeTools-0.1.39/sometools/async_tools/redis_tools/__init__.py
--rw-rw-rw-   0        0        0     1227 2022-02-11 05:55:29.000000 SomeTools-0.1.39/sometools/async_tools/redis_tools/async_io_redis.py
-drwxrwxrwx   0        0        0        0 2022-05-26 03:33:41.499000 SomeTools-0.1.39/sometools/sync_tools/
--rw-rw-rw-   0        0        0        0 2022-01-04 06:56:33.000000 SomeTools-0.1.39/sometools/sync_tools/__init__.py
-drwxrwxrwx   0        0        0        0 2022-05-26 03:33:41.500000 SomeTools-0.1.39/sometools/sync_tools/base/
--rw-rw-rw-   0        0        0       42 2022-01-04 06:56:33.000000 SomeTools-0.1.39/sometools/sync_tools/base/__init__.py
--rw-rw-rw-   0        0        0      196 2022-01-04 06:56:33.000000 SomeTools-0.1.39/sometools/sync_tools/base/base.py
-drwxrwxrwx   0        0        0        0 2022-05-26 03:33:41.500000 SomeTools-0.1.39/sometools/sync_tools/calendar_tools/
--rw-rw-rw-   0        0        0       69 2022-05-26 03:19:51.000000 SomeTools-0.1.39/sometools/sync_tools/calendar_tools/__init__.py
--rw-rw-rw-   0        0        0     5465 2022-05-26 03:25:52.000000 SomeTools-0.1.39/sometools/sync_tools/calendar_tools/calendar_tool.py
-drwxrwxrwx   0        0        0        0 2022-05-26 03:33:41.501000 SomeTools-0.1.39/sometools/sync_tools/char_tools/
--rw-rw-rw-   0        0        0       58 2022-01-04 06:56:33.000000 SomeTools-0.1.39/sometools/sync_tools/char_tools/__init__.py
--rw-rw-rw-   0        0        0      895 2022-03-09 01:30:06.000000 SomeTools-0.1.39/sometools/sync_tools/char_tools/char_tools.py
-drwxrwxrwx   0        0        0        0 2022-05-26 03:33:41.502000 SomeTools-0.1.39/sometools/sync_tools/chinese_to_pinyin_acronym/
--rw-rw-rw-   0        0        0      121 2022-01-04 06:56:33.000000 SomeTools-0.1.39/sometools/sync_tools/chinese_to_pinyin_acronym/__init__.py
--rw-rw-rw-   0        0        0     3448 2022-01-04 06:56:33.000000 SomeTools-0.1.39/sometools/sync_tools/chinese_to_pinyin_acronym/chinese_to_pinyin.py
-drwxrwxrwx   0        0        0        0 2022-05-26 03:33:41.503000 SomeTools-0.1.39/sometools/sync_tools/datetime_tools/
--rw-rw-rw-   0        0        0       71 2022-01-04 06:56:33.000000 SomeTools-0.1.39/sometools/sync_tools/datetime_tools/__init__.py
--rw-rw-rw-   0        0        0    12057 2022-02-23 08:15:43.000000 SomeTools-0.1.39/sometools/sync_tools/datetime_tools/date_conversion.py
-drwxrwxrwx   0        0        0        0 2022-05-26 03:33:41.504000 SomeTools-0.1.39/sometools/sync_tools/image_tools/
--rw-rw-rw-   0        0        0       61 2022-01-04 06:56:33.000000 SomeTools-0.1.39/sometools/sync_tools/image_tools/__init__.py
--rw-rw-rw-   0        0        0     2575 2022-02-11 05:52:24.000000 SomeTools-0.1.39/sometools/sync_tools/image_tools/image_tools.py
-drwxrwxrwx   0        0        0        0 2022-05-26 03:33:41.505000 SomeTools-0.1.39/sometools/sync_tools/ip_tools/
--rw-rw-rw-   0        0        0       51 2022-05-26 02:19:51.000000 SomeTools-0.1.39/sometools/sync_tools/ip_tools/__init__.py
--rw-rw-rw-   0        0        0      538 2022-05-26 02:19:51.000000 SomeTools-0.1.39/sometools/sync_tools/ip_tools/ip_tool.py
-drwxrwxrwx   0        0        0        0 2022-05-26 03:33:41.506000 SomeTools-0.1.39/sometools/sync_tools/log_tools/
--rw-rw-rw-   0        0        0       57 2022-01-04 06:56:33.000000 SomeTools-0.1.39/sometools/sync_tools/log_tools/__init__.py
--rw-rw-rw-   0        0        0     3758 2022-01-04 06:56:33.000000 SomeTools-0.1.39/sometools/sync_tools/log_tools/logger_main.py
-drwxrwxrwx   0        0        0        0 2022-05-26 03:33:41.506000 SomeTools-0.1.39/sometools/sync_tools/os_tools/
--rw-rw-rw-   0        0        0       52 2022-01-04 06:56:33.000000 SomeTools-0.1.39/sometools/sync_tools/os_tools/__init__.py
--rw-rw-rw-   0        0        0     3566 2022-01-04 06:56:33.000000 SomeTools-0.1.39/sometools/sync_tools/os_tools/os_tools.py
-drwxrwxrwx   0        0        0        0 2022-05-26 03:33:41.507000 SomeTools-0.1.39/sometools/sync_tools/re_tools/
--rw-rw-rw-   0        0        0       80 2022-01-04 06:56:33.000000 SomeTools-0.1.39/sometools/sync_tools/re_tools/__init__.py
--rw-rw-rw-   0        0        0     2551 2022-01-04 06:56:33.000000 SomeTools-0.1.39/sometools/sync_tools/re_tools/extract_string.py
-drwxrwxrwx   0        0        0        0 2022-05-26 03:33:41.508000 SomeTools-0.1.39/sometools/sync_tools/redis_tools/
--rw-rw-rw-   0        0        0       60 2022-01-04 06:56:33.000000 SomeTools-0.1.39/sometools/sync_tools/redis_tools/__init__.py
--rw-rw-rw-   0        0        0      916 2022-01-04 06:56:33.000000 SomeTools-0.1.39/sometools/sync_tools/redis_tools/redis_main.py
-drwxrwxrwx   0        0        0        0 2022-05-26 03:33:41.509000 SomeTools-0.1.39/sometools/sync_tools/string_tools/
--rw-rw-rw-   0        0        0       67 2022-01-04 06:56:33.000000 SomeTools-0.1.39/sometools/sync_tools/string_tools/__init__.py
--rw-rw-rw-   0        0        0     1761 2022-01-04 06:56:33.000000 SomeTools-0.1.39/sometools/sync_tools/string_tools/string_cleaning.py
-drwxrwxrwx   0        0        0        0 2022-05-26 03:33:41.510000 SomeTools-0.1.39/sometools/sync_tools/traditional_simplified_chinese_conversion/
--rw-rw-rw-   0        0        0      148 2022-01-04 06:56:33.000000 SomeTools-0.1.39/sometools/sync_tools/traditional_simplified_chinese_conversion/__init__.py
--rw-rw-rw-   0        0        0     1955 2022-01-04 06:56:33.000000 SomeTools-0.1.39/sometools/sync_tools/traditional_simplified_chinese_conversion/traditional_simplified_chinese.py
-drwxrwxrwx   0        0        0        0 2022-05-26 03:33:41.511000 SomeTools-0.1.39/sometools/sync_tools/url_tools/
--rw-rw-rw-   0        0        0       87 2022-01-04 06:56:33.000000 SomeTools-0.1.39/sometools/sync_tools/url_tools/__init__.py
--rw-rw-rw-   0        0        0     1875 2022-01-04 06:56:33.000000 SomeTools-0.1.39/sometools/sync_tools/url_tools/url_encode_decode.py
+drwxrwxrwx   0        0        0        0 2023-06-10 15:59:48.356298 SomeTools-0.1.40/
+-rw-rw-rw-   0        0        0     1091 2023-06-10 10:45:04.000000 SomeTools-0.1.40/LICENSE
+-rw-rw-rw-   0        0        0     2244 2023-06-10 15:59:48.354263 SomeTools-0.1.40/PKG-INFO
+-rw-rw-rw-   0        0        0     1527 2023-06-10 15:49:43.000000 SomeTools-0.1.40/README.md
+drwxrwxrwx   0        0        0        0 2023-06-10 15:59:48.331031 SomeTools-0.1.40/SomeTools.egg-info/
+-rw-rw-rw-   0        0        0     2244 2023-06-10 15:59:48.000000 SomeTools-0.1.40/SomeTools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2426 2023-06-10 15:59:48.000000 SomeTools-0.1.40/SomeTools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-10 15:59:48.000000 SomeTools-0.1.40/SomeTools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      188 2023-06-10 15:59:48.000000 SomeTools-0.1.40/SomeTools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-10 15:59:48.000000 SomeTools-0.1.40/SomeTools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-10 15:59:48.356298 SomeTools-0.1.40/setup.cfg
+-rw-rw-rw-   0        0        0     2179 2023-06-10 15:53:26.000000 SomeTools-0.1.40/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-10 15:59:48.331031 SomeTools-0.1.40/sometools/
+-rw-rw-rw-   0        0        0     1545 2023-06-10 15:43:30.000000 SomeTools-0.1.40/sometools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-10 15:59:48.332032 SomeTools-0.1.40/sometools/async_tools/
+-rw-rw-rw-   0        0        0      550 2023-06-10 10:45:04.000000 SomeTools-0.1.40/sometools/async_tools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-10 15:59:48.333032 SomeTools-0.1.40/sometools/async_tools/base/
+-rw-rw-rw-   0        0        0       42 2023-06-10 10:45:04.000000 SomeTools-0.1.40/sometools/async_tools/base/__init__.py
+-rw-rw-rw-   0        0        0      181 2023-06-10 10:45:04.000000 SomeTools-0.1.40/sometools/async_tools/base/base.py
+drwxrwxrwx   0        0        0        0 2023-06-10 15:59:48.334031 SomeTools-0.1.40/sometools/async_tools/bloom_filter/
+-rw-rw-rw-   0        0        0       90 2023-06-10 10:45:04.000000 SomeTools-0.1.40/sometools/async_tools/bloom_filter/__init__.py
+-rw-rw-rw-   0        0        0     3632 2023-06-10 10:45:04.000000 SomeTools-0.1.40/sometools/async_tools/bloom_filter/async_bloomfilter_tool.py
+drwxrwxrwx   0        0        0        0 2023-06-10 15:59:48.334031 SomeTools-0.1.40/sometools/async_tools/database_tools/
+-rw-rw-rw-   0        0        0        0 2023-06-10 10:45:04.000000 SomeTools-0.1.40/sometools/async_tools/database_tools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-10 15:59:48.336033 SomeTools-0.1.40/sometools/async_tools/database_tools/mysql_tools/
+-rw-rw-rw-   0        0        0        0 2023-06-10 10:45:04.000000 SomeTools-0.1.40/sometools/async_tools/database_tools/mysql_tools/__init__.py
+-rw-rw-rw-   0        0        0    14159 2023-06-10 10:45:04.000000 SomeTools-0.1.40/sometools/async_tools/database_tools/mysql_tools/async_mysql_orm.py
+drwxrwxrwx   0        0        0        0 2023-06-10 15:59:48.337260 SomeTools-0.1.40/sometools/async_tools/redis_tools/
+-rw-rw-rw-   0        0        0       78 2023-06-10 10:45:04.000000 SomeTools-0.1.40/sometools/async_tools/redis_tools/__init__.py
+-rw-rw-rw-   0        0        0     1227 2023-06-10 10:45:04.000000 SomeTools-0.1.40/sometools/async_tools/redis_tools/async_io_redis.py
+drwxrwxrwx   0        0        0        0 2023-06-10 15:59:48.337260 SomeTools-0.1.40/sometools/sync_tools/
+-rw-rw-rw-   0        0        0        0 2023-06-10 10:45:04.000000 SomeTools-0.1.40/sometools/sync_tools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-10 15:59:48.339263 SomeTools-0.1.40/sometools/sync_tools/base/
+-rw-rw-rw-   0        0        0       42 2023-06-10 10:45:04.000000 SomeTools-0.1.40/sometools/sync_tools/base/__init__.py
+-rw-rw-rw-   0        0        0      196 2023-06-10 10:45:04.000000 SomeTools-0.1.40/sometools/sync_tools/base/base.py
+drwxrwxrwx   0        0        0        0 2023-06-10 15:59:48.340264 SomeTools-0.1.40/sometools/sync_tools/calendar_tools/
+-rw-rw-rw-   0        0        0       69 2023-06-10 10:45:04.000000 SomeTools-0.1.40/sometools/sync_tools/calendar_tools/__init__.py
+-rw-rw-rw-   0        0        0     2785 2023-06-10 10:45:04.000000 SomeTools-0.1.40/sometools/sync_tools/calendar_tools/calendar_tool.py
+drwxrwxrwx   0        0        0        0 2023-06-10 15:59:48.341263 SomeTools-0.1.40/sometools/sync_tools/char_tools/
+-rw-rw-rw-   0        0        0       58 2023-06-10 10:45:04.000000 SomeTools-0.1.40/sometools/sync_tools/char_tools/__init__.py
+-rw-rw-rw-   0        0        0      895 2023-06-10 10:45:04.000000 SomeTools-0.1.40/sometools/sync_tools/char_tools/char_tools.py
+drwxrwxrwx   0        0        0        0 2023-06-10 15:59:48.342264 SomeTools-0.1.40/sometools/sync_tools/chinese_to_pinyin_acronym/
+-rw-rw-rw-   0        0        0      121 2023-06-10 10:45:04.000000 SomeTools-0.1.40/sometools/sync_tools/chinese_to_pinyin_acronym/__init__.py
+-rw-rw-rw-   0        0        0     3448 2023-06-10 10:45:04.000000 SomeTools-0.1.40/sometools/sync_tools/chinese_to_pinyin_acronym/chinese_to_pinyin.py
+drwxrwxrwx   0        0        0        0 2023-06-10 15:59:48.342264 SomeTools-0.1.40/sometools/sync_tools/database_tools/
+-rw-rw-rw-   0        0        0        0 2023-06-10 10:45:04.000000 SomeTools-0.1.40/sometools/sync_tools/database_tools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-10 15:59:48.343263 SomeTools-0.1.40/sometools/sync_tools/database_tools/mysql_tools/
+-rw-rw-rw-   0        0        0        0 2023-06-10 10:45:04.000000 SomeTools-0.1.40/sometools/sync_tools/database_tools/mysql_tools/__init__.py
+-rw-rw-rw-   0        0        0     2608 2023-06-10 10:45:04.000000 SomeTools-0.1.40/sometools/sync_tools/database_tools/mysql_tools/conn_pool.py
+drwxrwxrwx   0        0        0        0 2023-06-10 15:59:48.344263 SomeTools-0.1.40/sometools/sync_tools/datetime_tools/
+-rw-rw-rw-   0        0        0       71 2023-06-10 10:45:04.000000 SomeTools-0.1.40/sometools/sync_tools/datetime_tools/__init__.py
+-rw-rw-rw-   0        0        0    12057 2023-06-10 10:45:04.000000 SomeTools-0.1.40/sometools/sync_tools/datetime_tools/date_conversion.py
+drwxrwxrwx   0        0        0        0 2023-06-10 15:59:48.345263 SomeTools-0.1.40/sometools/sync_tools/encryption_and_decryption_tools/
+-rw-rw-rw-   0        0        0       88 2023-06-10 11:04:14.000000 SomeTools-0.1.40/sometools/sync_tools/encryption_and_decryption_tools/__init__.py
+-rw-rw-rw-   0        0        0     5434 2023-06-10 15:34:27.000000 SomeTools-0.1.40/sometools/sync_tools/encryption_and_decryption_tools/aes_tool.py
+drwxrwxrwx   0        0        0        0 2023-06-10 15:59:48.346263 SomeTools-0.1.40/sometools/sync_tools/image_tools/
+-rw-rw-rw-   0        0        0       61 2023-06-10 10:45:04.000000 SomeTools-0.1.40/sometools/sync_tools/image_tools/__init__.py
+-rw-rw-rw-   0        0        0     2575 2023-06-10 10:45:04.000000 SomeTools-0.1.40/sometools/sync_tools/image_tools/image_tools.py
+drwxrwxrwx   0        0        0        0 2023-06-10 15:59:48.347263 SomeTools-0.1.40/sometools/sync_tools/ip_tools/
+-rw-rw-rw-   0        0        0       51 2023-06-10 10:45:04.000000 SomeTools-0.1.40/sometools/sync_tools/ip_tools/__init__.py
+-rw-rw-rw-   0        0        0      538 2023-06-10 10:45:04.000000 SomeTools-0.1.40/sometools/sync_tools/ip_tools/ip_tool.py
+drwxrwxrwx   0        0        0        0 2023-06-10 15:59:48.348263 SomeTools-0.1.40/sometools/sync_tools/log_tools/
+-rw-rw-rw-   0        0        0       57 2023-06-10 10:45:04.000000 SomeTools-0.1.40/sometools/sync_tools/log_tools/__init__.py
+-rw-rw-rw-   0        0        0     3758 2023-06-10 10:45:04.000000 SomeTools-0.1.40/sometools/sync_tools/log_tools/logger_main.py
+drwxrwxrwx   0        0        0        0 2023-06-10 15:59:48.348263 SomeTools-0.1.40/sometools/sync_tools/os_tools/
+-rw-rw-rw-   0        0        0       52 2023-06-10 10:45:04.000000 SomeTools-0.1.40/sometools/sync_tools/os_tools/__init__.py
+-rw-rw-rw-   0        0        0     3566 2023-06-10 10:45:04.000000 SomeTools-0.1.40/sometools/sync_tools/os_tools/os_tools.py
+drwxrwxrwx   0        0        0        0 2023-06-10 15:59:48.350263 SomeTools-0.1.40/sometools/sync_tools/re_tools/
+-rw-rw-rw-   0        0        0       80 2023-06-10 10:45:04.000000 SomeTools-0.1.40/sometools/sync_tools/re_tools/__init__.py
+-rw-rw-rw-   0        0        0     2551 2023-06-10 10:45:04.000000 SomeTools-0.1.40/sometools/sync_tools/re_tools/extract_string.py
+drwxrwxrwx   0        0        0        0 2023-06-10 15:59:48.351263 SomeTools-0.1.40/sometools/sync_tools/redis_tools/
+-rw-rw-rw-   0        0        0       60 2023-06-10 10:45:04.000000 SomeTools-0.1.40/sometools/sync_tools/redis_tools/__init__.py
+-rw-rw-rw-   0        0        0      916 2023-06-10 10:45:04.000000 SomeTools-0.1.40/sometools/sync_tools/redis_tools/redis_main.py
+drwxrwxrwx   0        0        0        0 2023-06-10 15:59:48.352263 SomeTools-0.1.40/sometools/sync_tools/string_tools/
+-rw-rw-rw-   0        0        0       67 2023-06-10 10:45:04.000000 SomeTools-0.1.40/sometools/sync_tools/string_tools/__init__.py
+-rw-rw-rw-   0        0        0     1761 2023-06-10 10:45:04.000000 SomeTools-0.1.40/sometools/sync_tools/string_tools/string_cleaning.py
+drwxrwxrwx   0        0        0        0 2023-06-10 15:59:48.353263 SomeTools-0.1.40/sometools/sync_tools/traditional_simplified_chinese_conversion/
+-rw-rw-rw-   0        0        0      148 2023-06-10 10:45:04.000000 SomeTools-0.1.40/sometools/sync_tools/traditional_simplified_chinese_conversion/__init__.py
+-rw-rw-rw-   0        0        0     1955 2023-06-10 10:45:04.000000 SomeTools-0.1.40/sometools/sync_tools/traditional_simplified_chinese_conversion/traditional_simplified_chinese.py
+drwxrwxrwx   0        0        0        0 2023-06-10 15:59:48.354263 SomeTools-0.1.40/sometools/sync_tools/url_tools/
+-rw-rw-rw-   0        0        0       87 2023-06-10 10:45:04.000000 SomeTools-0.1.40/sometools/sync_tools/url_tools/__init__.py
+-rw-rw-rw-   0        0        0     1875 2023-06-10 10:45:04.000000 SomeTools-0.1.40/sometools/sync_tools/url_tools/url_encode_decode.py
```

### Comparing `SomeTools-0.1.39/LICENSE` & `SomeTools-0.1.40/LICENSE`

 * *Files identical despite different names*

### Comparing `SomeTools-0.1.39/SomeTools.egg-info/SOURCES.txt` & `SomeTools-0.1.40/SomeTools.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -22,16 +22,21 @@
 sometools/sync_tools/base/base.py
 sometools/sync_tools/calendar_tools/__init__.py
 sometools/sync_tools/calendar_tools/calendar_tool.py
 sometools/sync_tools/char_tools/__init__.py
 sometools/sync_tools/char_tools/char_tools.py
 sometools/sync_tools/chinese_to_pinyin_acronym/__init__.py
 sometools/sync_tools/chinese_to_pinyin_acronym/chinese_to_pinyin.py
+sometools/sync_tools/database_tools/__init__.py
+sometools/sync_tools/database_tools/mysql_tools/__init__.py
+sometools/sync_tools/database_tools/mysql_tools/conn_pool.py
 sometools/sync_tools/datetime_tools/__init__.py
 sometools/sync_tools/datetime_tools/date_conversion.py
+sometools/sync_tools/encryption_and_decryption_tools/__init__.py
+sometools/sync_tools/encryption_and_decryption_tools/aes_tool.py
 sometools/sync_tools/image_tools/__init__.py
 sometools/sync_tools/image_tools/image_tools.py
 sometools/sync_tools/ip_tools/__init__.py
 sometools/sync_tools/ip_tools/ip_tool.py
 sometools/sync_tools/log_tools/__init__.py
 sometools/sync_tools/log_tools/logger_main.py
 sometools/sync_tools/os_tools/__init__.py
```

### Comparing `SomeTools-0.1.39/setup.py` & `SomeTools-0.1.40/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 from setuptools import find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(name='SomeTools',
-      version='0.1.39',
+      version='0.1.40',
       description="Some python tools",
       author="zhangkun",
       author_email="zk.kyle@foxmail.com",
       project_urls={
           'Documentation': 'https://github.com/584807419/SomeTools',
           'Funding': 'https://github.com/584807419/SomeTools',
           'Source': 'https://github.com/584807419/SomeTools',
@@ -34,14 +34,15 @@
           "redis==4.0.2",
           "aioredis==2.0.1",
           "pillow==8.4.0",
           "chardet==4.0.0",
           "psutil==5.9.0",
           "aiomysql==0.0.22",
           "pymysql==0.9.3",
+          "pycryptodome==3.18.0",
           # "orjson",  # 底层使用了rust，Python下最快的json库,比 ujson 快 3 倍，比 json 快 6 倍
       ],
       py_modules=['sometools'],
       include_package_data=True,
       platforms="any",
       scripts=[],
       )
```

### Comparing `SomeTools-0.1.39/sometools/__init__.py` & `SomeTools-0.1.40/sometools/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,19 +4,22 @@
 from sometools.sync_tools.string_tools import StringMixIn
 from sometools.sync_tools.log_tools import LogMixIn
 from sometools.sync_tools.datetime_tools import DatetimeMixIn
 from sometools.sync_tools.chinese_to_pinyin_acronym import ChineseToPinyinMixIn
 from sometools.sync_tools.traditional_simplified_chinese_conversion import TraditionalSimplifiedChineseMixIn
 from sometools.sync_tools.url_tools import UrlEncodeDecodeMixIn
 from sometools.sync_tools.redis_tools import RedisMixIn
+from sometools.sync_tools.database_tools.mysql_tools.conn_pool import MysqlPoolMixIn
 from sometools.sync_tools.re_tools import ExtractStringMixIn
 from sometools.sync_tools.image_tools import ImageMixin
 from sometools.sync_tools.char_tools import CharMixin
 from sometools.sync_tools.os_tools import OsMixin
 from sometools.sync_tools.ip_tools import IpMixIn
 from sometools.sync_tools.calendar_tools import CalendarMixIn
+from sometools.sync_tools.encryption_and_decryption_tools import EncryptionDecryptionMixIn
 
 
 class Common_tools(ChineseToPinyinMixIn, TraditionalSimplifiedChineseMixIn, UrlEncodeDecodeMixIn, DatetimeMixIn,
-                   StringMixIn, IpMixIn, CalendarMixIn, ImageMixin, CharMixin, ExtractStringMixIn, OsMixin, LogMixIn, RedisMixIn):
+                   StringMixIn, IpMixIn, CalendarMixIn, ImageMixin, CharMixin, ExtractStringMixIn, OsMixin, LogMixIn,
+                   RedisMixIn, MysqlPoolMixIn, EncryptionDecryptionMixIn):
     def __init__(self, *args, **kwargs):
         super(Common_tools, self).__init__(*args, **kwargs)
```

### Comparing `SomeTools-0.1.39/sometools/async_tools/__init__.py` & `SomeTools-0.1.40/sometools/async_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `SomeTools-0.1.39/sometools/async_tools/bloom_filter/async_bloomfilter_tool.py` & `SomeTools-0.1.40/sometools/async_tools/bloom_filter/async_bloomfilter_tool.py`

 * *Files identical despite different names*

### Comparing `SomeTools-0.1.39/sometools/async_tools/database_tools/mysql_tools/async_mysql_orm.py` & `SomeTools-0.1.40/sometools/async_tools/database_tools/mysql_tools/async_mysql_orm.py`

 * *Files identical despite different names*

### Comparing `SomeTools-0.1.39/sometools/async_tools/redis_tools/async_io_redis.py` & `SomeTools-0.1.40/sometools/async_tools/redis_tools/async_io_redis.py`

 * *Files identical despite different names*

### Comparing `SomeTools-0.1.39/sometools/sync_tools/char_tools/char_tools.py` & `SomeTools-0.1.40/sometools/sync_tools/char_tools/char_tools.py`

 * *Files identical despite different names*

### Comparing `SomeTools-0.1.39/sometools/sync_tools/chinese_to_pinyin_acronym/chinese_to_pinyin.py` & `SomeTools-0.1.40/sometools/sync_tools/chinese_to_pinyin_acronym/chinese_to_pinyin.py`

 * *Files identical despite different names*

### Comparing `SomeTools-0.1.39/sometools/sync_tools/datetime_tools/date_conversion.py` & `SomeTools-0.1.40/sometools/sync_tools/datetime_tools/date_conversion.py`

 * *Files identical despite different names*

### Comparing `SomeTools-0.1.39/sometools/sync_tools/image_tools/image_tools.py` & `SomeTools-0.1.40/sometools/sync_tools/image_tools/image_tools.py`

 * *Files identical despite different names*

### Comparing `SomeTools-0.1.39/sometools/sync_tools/ip_tools/ip_tool.py` & `SomeTools-0.1.40/sometools/sync_tools/ip_tools/ip_tool.py`

 * *Files identical despite different names*

### Comparing `SomeTools-0.1.39/sometools/sync_tools/log_tools/logger_main.py` & `SomeTools-0.1.40/sometools/sync_tools/log_tools/logger_main.py`

 * *Files identical despite different names*

### Comparing `SomeTools-0.1.39/sometools/sync_tools/os_tools/os_tools.py` & `SomeTools-0.1.40/sometools/sync_tools/os_tools/os_tools.py`

 * *Files identical despite different names*

### Comparing `SomeTools-0.1.39/sometools/sync_tools/re_tools/extract_string.py` & `SomeTools-0.1.40/sometools/sync_tools/re_tools/extract_string.py`

 * *Files identical despite different names*

### Comparing `SomeTools-0.1.39/sometools/sync_tools/redis_tools/redis_main.py` & `SomeTools-0.1.40/sometools/sync_tools/redis_tools/redis_main.py`

 * *Files identical despite different names*

### Comparing `SomeTools-0.1.39/sometools/sync_tools/string_tools/string_cleaning.py` & `SomeTools-0.1.40/sometools/sync_tools/string_tools/string_cleaning.py`

 * *Files identical despite different names*

### Comparing `SomeTools-0.1.39/sometools/sync_tools/traditional_simplified_chinese_conversion/traditional_simplified_chinese.py` & `SomeTools-0.1.40/sometools/sync_tools/traditional_simplified_chinese_conversion/traditional_simplified_chinese.py`

 * *Files identical despite different names*

### Comparing `SomeTools-0.1.39/sometools/sync_tools/url_tools/url_encode_decode.py` & `SomeTools-0.1.40/sometools/sync_tools/url_tools/url_encode_decode.py`

 * *Files identical despite different names*

