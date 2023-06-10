# Comparing `tmp/gbpcli-1.5.0.tar.gz` & `tmp/gbpcli-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gbpcli-1.5.0.tar", last modified: Thu Jun  8 23:06:32 2023, max compression
+gzip compressed data, was "gbpcli-1.5.1.tar", last modified: Fri Jun  9 23:57:03 2023, max compression
```

## Comparing `gbpcli-1.5.0.tar` & `gbpcli-1.5.1.tar`

### file list

```diff
@@ -1,87 +1,87 @@
--rw-r--r--   0        0        0      654 2023-02-25 13:20:56.364600 gbpcli-1.5.0/LICENSE
--rw-r--r--   0        0        0     3707 2023-02-25 13:20:56.365600 gbpcli-1.5.0/README.md
--rw-r--r--   0        0        0     1835 2023-06-08 23:06:32.073585 gbpcli-1.5.0/pyproject.toml
--rw-r--r--   0        0        0    11601 2023-06-04 23:31:11.836617 gbpcli-1.5.0/src/gbpcli/__init__.py
--rw-r--r--   0        0        0      108 2022-09-05 18:14:24.258925 gbpcli-1.5.0/src/gbpcli/__main__.py
--rw-r--r--   0        0        0     2369 2023-03-19 20:53:02.457971 gbpcli-1.5.0/src/gbpcli/graphql.py
--rw-r--r--   0        0        0        0 2022-09-05 18:14:24.258925 gbpcli-1.5.0/src/gbpcli/py.typed
--rw-r--r--   0        0        0      195 2023-01-02 21:58:07.125538 gbpcli-1.5.0/src/gbpcli/queries/build.graphql
--rw-r--r--   0        0        0      144 2022-10-04 22:58:21.349383 gbpcli-1.5.0/src/gbpcli/queries/builds.graphql
--rw-r--r--   0        0        0      215 2022-10-12 12:48:42.261841 gbpcli-1.5.0/src/gbpcli/queries/builds_with_packages.graphql
--rw-r--r--   0        0        0       90 2022-09-05 18:14:24.259925 gbpcli-1.5.0/src/gbpcli/queries/create_note.graphql
--rw-r--r--   0        0        0      256 2022-09-05 18:14:24.259925 gbpcli-1.5.0/src/gbpcli/queries/diff.graphql
--rw-r--r--   0        0        0       60 2022-09-05 18:14:24.259925 gbpcli-1.5.0/src/gbpcli/queries/keep_build.graphql
--rw-r--r--   0        0        0       71 2022-09-05 18:14:24.259925 gbpcli-1.5.0/src/gbpcli/queries/latest.graphql
--rw-r--r--   0        0        0       53 2022-09-05 18:14:24.259925 gbpcli-1.5.0/src/gbpcli/queries/logs.graphql
--rw-r--r--   0        0        0       39 2022-10-12 12:48:42.261841 gbpcli-1.5.0/src/gbpcli/queries/machine_names.graphql
--rw-r--r--   0        0        0      103 2022-10-03 11:17:00.242651 gbpcli-1.5.0/src/gbpcli/queries/machines.graphql
--rw-r--r--   0        0        0       57 2022-09-05 18:14:24.260925 gbpcli-1.5.0/src/gbpcli/queries/packages.graphql
--rw-r--r--   0        0        0       85 2022-09-05 18:14:24.260925 gbpcli-1.5.0/src/gbpcli/queries/publish.graphql
--rw-r--r--   0        0        0       61 2022-09-05 18:14:24.260925 gbpcli-1.5.0/src/gbpcli/queries/pull.graphql
--rw-r--r--   0        0        0       63 2022-09-05 18:14:24.260925 gbpcli-1.5.0/src/gbpcli/queries/release_build.graphql
--rw-r--r--   0        0        0      106 2022-09-05 18:14:24.261925 gbpcli-1.5.0/src/gbpcli/queries/resolve_tag.graphql
--rw-r--r--   0        0        0       68 2022-09-05 18:14:24.261925 gbpcli-1.5.0/src/gbpcli/queries/schedule_build.graphql
--rw-r--r--   0        0        0      252 2023-03-20 02:47:01.244810 gbpcli-1.5.0/src/gbpcli/queries/search.graphql
--rw-r--r--   0        0        0       91 2022-09-05 18:14:24.261925 gbpcli-1.5.0/src/gbpcli/queries/tag_build.graphql
--rw-r--r--   0        0        0      110 2022-09-05 18:14:24.261925 gbpcli-1.5.0/src/gbpcli/queries/untag_build.graphql
--rw-r--r--   0        0        0     3707 2023-03-19 17:24:48.975558 gbpcli-1.5.0/src/gbpcli/render.py
--rw-r--r--   0        0        0     1383 2023-06-04 16:18:21.948227 gbpcli-1.5.0/src/gbpcli/subcommands/__init__.py
--rw-r--r--   0        0        0      456 2023-06-04 23:31:11.836617 gbpcli-1.5.0/src/gbpcli/subcommands/build.py
--rw-r--r--   0        0        0     3021 2023-06-04 16:18:21.948227 gbpcli-1.5.0/src/gbpcli/subcommands/diff.py
--rw-r--r--   0        0        0     3863 2023-06-04 16:18:21.948227 gbpcli-1.5.0/src/gbpcli/subcommands/inspect.py
--rw-r--r--   0        0        0      790 2023-06-04 16:18:21.948227 gbpcli-1.5.0/src/gbpcli/subcommands/keep.py
--rw-r--r--   0        0        0      622 2023-06-04 16:18:21.948227 gbpcli-1.5.0/src/gbpcli/subcommands/latest.py
--rw-r--r--   0        0        0     1593 2023-06-04 16:18:21.948227 gbpcli-1.5.0/src/gbpcli/subcommands/list.py
--rw-r--r--   0        0        0     1301 2023-06-04 16:18:21.948227 gbpcli-1.5.0/src/gbpcli/subcommands/logs.py
--rw-r--r--   0        0        0     1561 2023-06-04 16:18:21.948227 gbpcli-1.5.0/src/gbpcli/subcommands/machines.py
--rw-r--r--   0        0        0     2912 2023-06-04 16:18:21.948227 gbpcli-1.5.0/src/gbpcli/subcommands/notes.py
--rw-r--r--   0        0        0      755 2023-06-04 16:18:21.948227 gbpcli-1.5.0/src/gbpcli/subcommands/packages.py
--rw-r--r--   0        0        0      657 2023-06-04 16:18:21.948227 gbpcli-1.5.0/src/gbpcli/subcommands/publish.py
--rw-r--r--   0        0        0      529 2023-06-04 16:18:21.948227 gbpcli-1.5.0/src/gbpcli/subcommands/pull.py
--rw-r--r--   0        0        0     2567 2023-06-04 16:18:21.948227 gbpcli-1.5.0/src/gbpcli/subcommands/status.py
--rw-r--r--   0        0        0     1178 2023-06-04 16:18:21.948227 gbpcli-1.5.0/src/gbpcli/subcommands/tag.py
--rw-r--r--   0        0        0     1480 2023-02-28 03:19:35.708985 gbpcli-1.5.0/src/gbpcli/theme.py
--rw-r--r--   0        0        0     1460 2023-05-06 15:20:54.186681 gbpcli-1.5.0/src/gbpcli/utils.py
--rw-r--r--   0        0        0     4161 2023-06-04 16:18:21.949227 gbpcli-1.5.0/tests/__init__.py
--rw-r--r--   0        0        0       51 2021-11-09 18:24:04.826960 gbpcli-1.5.0/tests/data/create_note.json
--rw-r--r--   0        0        0     1770 2022-10-03 14:06:49.960295 gbpcli-1.5.0/tests/data/diff.json
--rw-r--r--   0        0        0      405 2022-02-15 12:17:15.614583 gbpcli-1.5.0/tests/data/diff_no_content.json
--rw-r--r--   0        0        0    10329 2022-10-12 12:48:42.261841 gbpcli-1.5.0/tests/data/inspect.ndjson
--rw-r--r--   0        0        0       76 2021-11-09 18:24:04.826960 gbpcli-1.5.0/tests/data/keep_build.json
--rw-r--r--   0        0        0       84 2022-02-15 12:17:42.117647 gbpcli-1.5.0/tests/data/latest.json
--rw-r--r--   0        0        0      355 2023-01-03 00:09:05.307268 gbpcli-1.5.0/tests/data/lighthouse.12672.json
--rw-r--r--   0        0        0    16680 2022-10-03 14:06:49.960295 gbpcli-1.5.0/tests/data/list.json
--rw-r--r--   0        0        0    12865 2022-08-09 01:32:16.919583 gbpcli-1.5.0/tests/data/list_with_packages.json
--rw-r--r--   0        0        0       85 2021-10-11 10:44:26.503390 gbpcli-1.5.0/tests/data/logs.json
--rw-r--r--   0        0        0     1499 2022-10-03 12:25:21.908033 gbpcli-1.5.0/tests/data/machines.json
--rw-r--r--   0        0        0    11936 2021-11-20 13:43:30.858627 gbpcli-1.5.0/tests/data/packages.json
--rw-r--r--   0        0        0     6959 2021-11-09 18:24:04.826960 gbpcli-1.5.0/tests/data/packages.txt
--rw-r--r--   0        0        0      129 2022-02-15 12:18:55.829810 gbpcli-1.5.0/tests/data/publish.json
--rw-r--r--   0        0        0       77 2021-11-09 18:24:04.826960 gbpcli-1.5.0/tests/data/pull.json
--rw-r--r--   0        0        0       80 2021-11-09 18:24:04.826960 gbpcli-1.5.0/tests/data/release_build.json
--rw-r--r--   0        0        0       83 2021-10-11 10:44:26.504390 gbpcli-1.5.0/tests/data/schedule_build.json
--rw-r--r--   0        0        0      468 2023-03-20 02:47:01.244810 gbpcli-1.5.0/tests/data/search_notes.json
--rw-r--r--   0        0        0      584 2022-10-03 00:09:10.558796 gbpcli-1.5.0/tests/data/status.json
--rw-r--r--   0        0        0       89 2022-08-08 03:06:02.871203 gbpcli-1.5.0/tests/data/tag_build.json
--rw-r--r--   0        0        0       89 2022-08-08 03:09:13.886678 gbpcli-1.5.0/tests/data/untag_build.json
--rw-r--r--   0        0        0      614 2023-06-04 16:18:21.949227 gbpcli-1.5.0/tests/test_build.py
--rw-r--r--   0        0        0     4922 2023-06-04 16:18:21.949227 gbpcli-1.5.0/tests/test_diff.py
--rw-r--r--   0        0        0     2833 2023-05-20 22:14:10.519712 gbpcli-1.5.0/tests/test_entrypoint.py
--rw-r--r--   0        0        0     1964 2023-03-20 02:47:01.244810 gbpcli-1.5.0/tests/test_gbp.py
--rw-r--r--   0        0        0     2330 2023-02-28 00:30:55.388901 gbpcli-1.5.0/tests/test_graphql.py
--rw-r--r--   0        0        0    11320 2023-06-04 16:18:21.949227 gbpcli-1.5.0/tests/test_inspect.py
--rw-r--r--   0        0        0     1654 2023-06-04 16:18:21.949227 gbpcli-1.5.0/tests/test_keep.py
--rw-r--r--   0        0        0     1107 2023-06-04 16:18:21.949227 gbpcli-1.5.0/tests/test_latest.py
--rw-r--r--   0        0        0     1973 2023-06-04 16:18:21.949227 gbpcli-1.5.0/tests/test_list.py
--rw-r--r--   0        0        0     1658 2023-06-04 16:18:21.949227 gbpcli-1.5.0/tests/test_logs.py
--rw-r--r--   0        0        0     2219 2023-06-04 16:18:21.949227 gbpcli-1.5.0/tests/test_machines.py
--rw-r--r--   0        0        0     5386 2023-06-04 16:18:21.949227 gbpcli-1.5.0/tests/test_notes.py
--rw-r--r--   0        0        0     1100 2023-06-04 16:18:21.949227 gbpcli-1.5.0/tests/test_packages.py
--rw-r--r--   0        0        0     1126 2023-06-04 16:18:21.949227 gbpcli-1.5.0/tests/test_publish.py
--rw-r--r--   0        0        0      606 2023-05-20 22:10:39.185359 gbpcli-1.5.0/tests/test_pull.py
--rw-r--r--   0        0        0     1386 2023-03-19 18:37:19.694606 gbpcli-1.5.0/tests/test_render.py
--rw-r--r--   0        0        0     2629 2023-06-04 16:18:21.949227 gbpcli-1.5.0/tests/test_status.py
--rw-r--r--   0        0        0     1699 2023-06-04 16:18:21.949227 gbpcli-1.5.0/tests/test_tag.py
--rw-r--r--   0        0        0     2320 2023-02-28 03:24:47.008778 gbpcli-1.5.0/tests/test_theme.py
--rw-r--r--   0        0        0     4161 2023-04-29 21:56:57.622759 gbpcli-1.5.0/tests/test_utils.py
--rw-r--r--   0        0        0     4440 1970-01-01 00:00:00.000000 gbpcli-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0      654 2023-02-25 13:20:56.364600 gbpcli-1.5.1/LICENSE
+-rw-r--r--   0        0        0     3707 2023-02-25 13:20:56.365600 gbpcli-1.5.1/README.md
+-rw-r--r--   0        0        0     1835 2023-06-09 23:57:03.166796 gbpcli-1.5.1/pyproject.toml
+-rw-r--r--   0        0        0    11680 2023-06-09 20:11:06.354757 gbpcli-1.5.1/src/gbpcli/__init__.py
+-rw-r--r--   0        0        0      108 2022-09-05 18:14:24.258925 gbpcli-1.5.1/src/gbpcli/__main__.py
+-rw-r--r--   0        0        0     2639 2023-06-09 23:42:36.550592 gbpcli-1.5.1/src/gbpcli/graphql.py
+-rw-r--r--   0        0        0        0 2022-09-05 18:14:24.258925 gbpcli-1.5.1/src/gbpcli/py.typed
+-rw-r--r--   0        0        0      195 2023-01-02 21:58:07.125538 gbpcli-1.5.1/src/gbpcli/queries/build.graphql
+-rw-r--r--   0        0        0      144 2022-10-04 22:58:21.349383 gbpcli-1.5.1/src/gbpcli/queries/builds.graphql
+-rw-r--r--   0        0        0      215 2022-10-12 12:48:42.261841 gbpcli-1.5.1/src/gbpcli/queries/builds_with_packages.graphql
+-rw-r--r--   0        0        0       90 2022-09-05 18:14:24.259925 gbpcli-1.5.1/src/gbpcli/queries/create_note.graphql
+-rw-r--r--   0        0        0      256 2022-09-05 18:14:24.259925 gbpcli-1.5.1/src/gbpcli/queries/diff.graphql
+-rw-r--r--   0        0        0       60 2022-09-05 18:14:24.259925 gbpcli-1.5.1/src/gbpcli/queries/keep_build.graphql
+-rw-r--r--   0        0        0       71 2022-09-05 18:14:24.259925 gbpcli-1.5.1/src/gbpcli/queries/latest.graphql
+-rw-r--r--   0        0        0       53 2022-09-05 18:14:24.259925 gbpcli-1.5.1/src/gbpcli/queries/logs.graphql
+-rw-r--r--   0        0        0       39 2022-10-12 12:48:42.261841 gbpcli-1.5.1/src/gbpcli/queries/machine_names.graphql
+-rw-r--r--   0        0        0      103 2022-10-03 11:17:00.242651 gbpcli-1.5.1/src/gbpcli/queries/machines.graphql
+-rw-r--r--   0        0        0       57 2022-09-05 18:14:24.260925 gbpcli-1.5.1/src/gbpcli/queries/packages.graphql
+-rw-r--r--   0        0        0       85 2022-09-05 18:14:24.260925 gbpcli-1.5.1/src/gbpcli/queries/publish.graphql
+-rw-r--r--   0        0        0       61 2022-09-05 18:14:24.260925 gbpcli-1.5.1/src/gbpcli/queries/pull.graphql
+-rw-r--r--   0        0        0       63 2022-09-05 18:14:24.260925 gbpcli-1.5.1/src/gbpcli/queries/release_build.graphql
+-rw-r--r--   0        0        0      106 2022-09-05 18:14:24.261925 gbpcli-1.5.1/src/gbpcli/queries/resolve_tag.graphql
+-rw-r--r--   0        0        0       68 2022-09-05 18:14:24.261925 gbpcli-1.5.1/src/gbpcli/queries/schedule_build.graphql
+-rw-r--r--   0        0        0      252 2023-03-20 02:47:01.244810 gbpcli-1.5.1/src/gbpcli/queries/search.graphql
+-rw-r--r--   0        0        0       91 2022-09-05 18:14:24.261925 gbpcli-1.5.1/src/gbpcli/queries/tag_build.graphql
+-rw-r--r--   0        0        0      110 2022-09-05 18:14:24.261925 gbpcli-1.5.1/src/gbpcli/queries/untag_build.graphql
+-rw-r--r--   0        0        0     3707 2023-03-19 17:24:48.975558 gbpcli-1.5.1/src/gbpcli/render.py
+-rw-r--r--   0        0        0     1383 2023-06-04 16:18:21.948227 gbpcli-1.5.1/src/gbpcli/subcommands/__init__.py
+-rw-r--r--   0        0        0      456 2023-06-04 23:31:11.836617 gbpcli-1.5.1/src/gbpcli/subcommands/build.py
+-rw-r--r--   0        0        0     3021 2023-06-04 16:18:21.948227 gbpcli-1.5.1/src/gbpcli/subcommands/diff.py
+-rw-r--r--   0        0        0     3863 2023-06-04 16:18:21.948227 gbpcli-1.5.1/src/gbpcli/subcommands/inspect.py
+-rw-r--r--   0        0        0      790 2023-06-04 16:18:21.948227 gbpcli-1.5.1/src/gbpcli/subcommands/keep.py
+-rw-r--r--   0        0        0      622 2023-06-04 16:18:21.948227 gbpcli-1.5.1/src/gbpcli/subcommands/latest.py
+-rw-r--r--   0        0        0     1593 2023-06-04 16:18:21.948227 gbpcli-1.5.1/src/gbpcli/subcommands/list.py
+-rw-r--r--   0        0        0     1301 2023-06-04 16:18:21.948227 gbpcli-1.5.1/src/gbpcli/subcommands/logs.py
+-rw-r--r--   0        0        0     1561 2023-06-04 16:18:21.948227 gbpcli-1.5.1/src/gbpcli/subcommands/machines.py
+-rw-r--r--   0        0        0     2912 2023-06-04 16:18:21.948227 gbpcli-1.5.1/src/gbpcli/subcommands/notes.py
+-rw-r--r--   0        0        0      755 2023-06-04 16:18:21.948227 gbpcli-1.5.1/src/gbpcli/subcommands/packages.py
+-rw-r--r--   0        0        0      657 2023-06-04 16:18:21.948227 gbpcli-1.5.1/src/gbpcli/subcommands/publish.py
+-rw-r--r--   0        0        0      529 2023-06-04 16:18:21.948227 gbpcli-1.5.1/src/gbpcli/subcommands/pull.py
+-rw-r--r--   0        0        0     2567 2023-06-04 16:18:21.948227 gbpcli-1.5.1/src/gbpcli/subcommands/status.py
+-rw-r--r--   0        0        0     1178 2023-06-04 16:18:21.948227 gbpcli-1.5.1/src/gbpcli/subcommands/tag.py
+-rw-r--r--   0        0        0     1480 2023-02-28 03:19:35.708985 gbpcli-1.5.1/src/gbpcli/theme.py
+-rw-r--r--   0        0        0     1460 2023-05-06 15:20:54.186681 gbpcli-1.5.1/src/gbpcli/utils.py
+-rw-r--r--   0        0        0     4161 2023-06-04 16:18:21.949227 gbpcli-1.5.1/tests/__init__.py
+-rw-r--r--   0        0        0       51 2021-11-09 18:24:04.826960 gbpcli-1.5.1/tests/data/create_note.json
+-rw-r--r--   0        0        0     1770 2022-10-03 14:06:49.960295 gbpcli-1.5.1/tests/data/diff.json
+-rw-r--r--   0        0        0      405 2022-02-15 12:17:15.614583 gbpcli-1.5.1/tests/data/diff_no_content.json
+-rw-r--r--   0        0        0    10329 2022-10-12 12:48:42.261841 gbpcli-1.5.1/tests/data/inspect.ndjson
+-rw-r--r--   0        0        0       76 2021-11-09 18:24:04.826960 gbpcli-1.5.1/tests/data/keep_build.json
+-rw-r--r--   0        0        0       84 2022-02-15 12:17:42.117647 gbpcli-1.5.1/tests/data/latest.json
+-rw-r--r--   0        0        0      355 2023-01-03 00:09:05.307268 gbpcli-1.5.1/tests/data/lighthouse.12672.json
+-rw-r--r--   0        0        0    16680 2022-10-03 14:06:49.960295 gbpcli-1.5.1/tests/data/list.json
+-rw-r--r--   0        0        0    12865 2022-08-09 01:32:16.919583 gbpcli-1.5.1/tests/data/list_with_packages.json
+-rw-r--r--   0        0        0       85 2021-10-11 10:44:26.503390 gbpcli-1.5.1/tests/data/logs.json
+-rw-r--r--   0        0        0     1499 2022-10-03 12:25:21.908033 gbpcli-1.5.1/tests/data/machines.json
+-rw-r--r--   0        0        0    11936 2021-11-20 13:43:30.858627 gbpcli-1.5.1/tests/data/packages.json
+-rw-r--r--   0        0        0     6959 2021-11-09 18:24:04.826960 gbpcli-1.5.1/tests/data/packages.txt
+-rw-r--r--   0        0        0      129 2022-02-15 12:18:55.829810 gbpcli-1.5.1/tests/data/publish.json
+-rw-r--r--   0        0        0       77 2021-11-09 18:24:04.826960 gbpcli-1.5.1/tests/data/pull.json
+-rw-r--r--   0        0        0       80 2021-11-09 18:24:04.826960 gbpcli-1.5.1/tests/data/release_build.json
+-rw-r--r--   0        0        0       83 2021-10-11 10:44:26.504390 gbpcli-1.5.1/tests/data/schedule_build.json
+-rw-r--r--   0        0        0      468 2023-03-20 02:47:01.244810 gbpcli-1.5.1/tests/data/search_notes.json
+-rw-r--r--   0        0        0      584 2022-10-03 00:09:10.558796 gbpcli-1.5.1/tests/data/status.json
+-rw-r--r--   0        0        0       89 2022-08-08 03:06:02.871203 gbpcli-1.5.1/tests/data/tag_build.json
+-rw-r--r--   0        0        0       89 2022-08-08 03:09:13.886678 gbpcli-1.5.1/tests/data/untag_build.json
+-rw-r--r--   0        0        0      614 2023-06-04 16:18:21.949227 gbpcli-1.5.1/tests/test_build.py
+-rw-r--r--   0        0        0     4922 2023-06-04 16:18:21.949227 gbpcli-1.5.1/tests/test_diff.py
+-rw-r--r--   0        0        0     2833 2023-05-20 22:14:10.519712 gbpcli-1.5.1/tests/test_entrypoint.py
+-rw-r--r--   0        0        0     1964 2023-03-20 02:47:01.244810 gbpcli-1.5.1/tests/test_gbp.py
+-rw-r--r--   0        0        0     2360 2023-06-09 23:41:40.986195 gbpcli-1.5.1/tests/test_graphql.py
+-rw-r--r--   0        0        0    11320 2023-06-04 16:18:21.949227 gbpcli-1.5.1/tests/test_inspect.py
+-rw-r--r--   0        0        0     1654 2023-06-04 16:18:21.949227 gbpcli-1.5.1/tests/test_keep.py
+-rw-r--r--   0        0        0     1107 2023-06-04 16:18:21.949227 gbpcli-1.5.1/tests/test_latest.py
+-rw-r--r--   0        0        0     1973 2023-06-04 16:18:21.949227 gbpcli-1.5.1/tests/test_list.py
+-rw-r--r--   0        0        0     1658 2023-06-04 16:18:21.949227 gbpcli-1.5.1/tests/test_logs.py
+-rw-r--r--   0        0        0     2219 2023-06-04 16:18:21.949227 gbpcli-1.5.1/tests/test_machines.py
+-rw-r--r--   0        0        0     5386 2023-06-04 16:18:21.949227 gbpcli-1.5.1/tests/test_notes.py
+-rw-r--r--   0        0        0     1100 2023-06-04 16:18:21.949227 gbpcli-1.5.1/tests/test_packages.py
+-rw-r--r--   0        0        0     1126 2023-06-04 16:18:21.949227 gbpcli-1.5.1/tests/test_publish.py
+-rw-r--r--   0        0        0      606 2023-05-20 22:10:39.185359 gbpcli-1.5.1/tests/test_pull.py
+-rw-r--r--   0        0        0     1386 2023-03-19 18:37:19.694606 gbpcli-1.5.1/tests/test_render.py
+-rw-r--r--   0        0        0     2629 2023-06-04 16:18:21.949227 gbpcli-1.5.1/tests/test_status.py
+-rw-r--r--   0        0        0     1699 2023-06-04 16:18:21.949227 gbpcli-1.5.1/tests/test_tag.py
+-rw-r--r--   0        0        0     2320 2023-02-28 03:24:47.008778 gbpcli-1.5.1/tests/test_theme.py
+-rw-r--r--   0        0        0     4161 2023-04-29 21:56:57.622759 gbpcli-1.5.1/tests/test_utils.py
+-rw-r--r--   0        0        0     4440 1970-01-01 00:00:00.000000 gbpcli-1.5.1/PKG-INFO
```

### Comparing `gbpcli-1.5.0/LICENSE` & `gbpcli-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gbpcli-1.5.0/README.md` & `gbpcli-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `gbpcli-1.5.0/pyproject.toml` & `gbpcli-1.5.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 classifiers = [
     "Environment :: Console",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
     "Operating System :: POSIX :: Linux",
     "Topic :: System :: Software Distribution",
     "Programming Language :: Python :: 3",
 ]
-version = "1.5.0"
+version = "1.5.1"
 
 [project.license]
 text = "GPL3+"
 
 [project.urls]
 homepage = "https://github.com/enku/gbpcli"
 repository = "https://github.com/enku/gbpcli"
```

### Comparing `gbpcli-1.5.0/src/gbpcli/__init__.py` & `gbpcli-1.5.1/src/gbpcli/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -135,16 +135,18 @@
     out: rich.console.Console
     err: rich.console.Console
 
 
 class GBP:
     """Python wrapper for the Gentoo Build Publisher API"""
 
-    def __init__(self, url: str) -> None:
-        self.query = graphql.Queries(yarl.URL(url) / "graphql")
+    def __init__(self, url: str, distribution: str = "gbpcli") -> None:
+        self.query = graphql.Queries(
+            yarl.URL(url) / "graphql", distribution=distribution
+        )
 
     def machines(self) -> list[tuple[str, int, dict]]:
         """Handler for subcommand"""
         data = graphql.check(self.query.machines())
 
         return [
             (i["machine"], i["buildCount"], i["latestBuild"]) for i in data["machines"]
```

### Comparing `gbpcli-1.5.0/src/gbpcli/graphql.py` & `gbpcli-1.5.1/src/gbpcli/graphql.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     """Interface to a graphql query.
 
     It can be called as a normal Python function.
 
     For example::
 
         >>> qs = "query ($machine: String!) { latest(machine: $machine) { id } }"
-        >>> query = Query(s, "https://gbp/graphql", requests.Session())
+        >>> query = Query(qs, "https://gbp/graphql", requests.Session())
         >>> query(machine="lighthouse")
         ({'latest': {'id': 'lighthouse.14205'}}, None)
     """
 
     headers = {"Accept-Encoding": "gzip, deflate"}
 
     def __init__(self, query: str, url, session) -> None:
@@ -47,30 +47,36 @@
 
         return response_json.get("data"), response_json.get("errors")
 
 
 class Queries:
     """Python interface to raw queries/*.graphql files"""
 
-    def __init__(self, url: yarl.URL) -> None:
+    def __init__(self, url: yarl.URL, distribution: str = "gbpcli") -> None:
+        """A namespace for queries.
+
+        url: the url to the graphql endpoint
+        distribution: name of python package to search for queries/*.graphql files
+        """
         self._url = str(url)
         self._session = requests.Session()
+        self._distribution = distribution
 
     def __getattr__(self, name: str) -> Query:
-        query_file = resources.files("gbpcli") / "queries" / f"{name}.graphql"
+        query_file = resources.files(self._distribution) / "queries" / f"{name}.graphql"
         try:
             query_str = query_file.read_text(encoding="UTF-8")
         except FileNotFoundError:
             raise AttributeError(name) from None
 
         return Query(query_str, self._url, self._session)
 
     def to_dict(self) -> dict[str, str]:
         """Return the queries as a dict"""
-        files = (resources.files("gbpcli") / "queries").iterdir()
+        files = (resources.files(self._distribution) / "queries").iterdir()
 
         return {
             filename.name[:-8]: getattr(self, filename.name[:-8])
             for filename in files
             if filename.name.endswith(".graphql")
         }
```

### Comparing `gbpcli-1.5.0/src/gbpcli/render.py` & `gbpcli-1.5.1/src/gbpcli/render.py`

 * *Files identical despite different names*

### Comparing `gbpcli-1.5.0/src/gbpcli/subcommands/__init__.py` & `gbpcli-1.5.1/src/gbpcli/subcommands/__init__.py`

 * *Files identical despite different names*

### Comparing `gbpcli-1.5.0/src/gbpcli/subcommands/diff.py` & `gbpcli-1.5.1/src/gbpcli/subcommands/diff.py`

 * *Files identical despite different names*

### Comparing `gbpcli-1.5.0/src/gbpcli/subcommands/inspect.py` & `gbpcli-1.5.1/src/gbpcli/subcommands/inspect.py`

 * *Files identical despite different names*

### Comparing `gbpcli-1.5.0/src/gbpcli/subcommands/keep.py` & `gbpcli-1.5.1/src/gbpcli/subcommands/keep.py`

 * *Files identical despite different names*

### Comparing `gbpcli-1.5.0/src/gbpcli/subcommands/latest.py` & `gbpcli-1.5.1/src/gbpcli/subcommands/latest.py`

 * *Files identical despite different names*

### Comparing `gbpcli-1.5.0/src/gbpcli/subcommands/list.py` & `gbpcli-1.5.1/src/gbpcli/subcommands/list.py`

 * *Files identical despite different names*

### Comparing `gbpcli-1.5.0/src/gbpcli/subcommands/logs.py` & `gbpcli-1.5.1/src/gbpcli/subcommands/logs.py`

 * *Files identical despite different names*

### Comparing `gbpcli-1.5.0/src/gbpcli/subcommands/machines.py` & `gbpcli-1.5.1/src/gbpcli/subcommands/machines.py`

 * *Files identical despite different names*

### Comparing `gbpcli-1.5.0/src/gbpcli/subcommands/notes.py` & `gbpcli-1.5.1/src/gbpcli/subcommands/notes.py`

 * *Files identical despite different names*

### Comparing `gbpcli-1.5.0/src/gbpcli/subcommands/packages.py` & `gbpcli-1.5.1/src/gbpcli/subcommands/packages.py`

 * *Files identical despite different names*

### Comparing `gbpcli-1.5.0/src/gbpcli/subcommands/publish.py` & `gbpcli-1.5.1/src/gbpcli/subcommands/publish.py`

 * *Files identical despite different names*

### Comparing `gbpcli-1.5.0/src/gbpcli/subcommands/pull.py` & `gbpcli-1.5.1/src/gbpcli/subcommands/pull.py`

 * *Files identical despite different names*

### Comparing `gbpcli-1.5.0/src/gbpcli/subcommands/status.py` & `gbpcli-1.5.1/src/gbpcli/subcommands/status.py`

 * *Files identical despite different names*

### Comparing `gbpcli-1.5.0/src/gbpcli/subcommands/tag.py` & `gbpcli-1.5.1/src/gbpcli/subcommands/tag.py`

 * *Files identical despite different names*

### Comparing `gbpcli-1.5.0/src/gbpcli/theme.py` & `gbpcli-1.5.1/src/gbpcli/theme.py`

 * *Files identical despite different names*

### Comparing `gbpcli-1.5.0/src/gbpcli/utils.py` & `gbpcli-1.5.1/src/gbpcli/utils.py`

 * *Files identical despite different names*

### Comparing `gbpcli-1.5.0/tests/__init__.py` & `gbpcli-1.5.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gbpcli-1.5.0/tests/data/diff.json` & `gbpcli-1.5.1/tests/data/diff.json`

 * *Files identical despite different names*

### Comparing `gbpcli-1.5.0/tests/data/inspect.ndjson` & `gbpcli-1.5.1/tests/data/inspect.ndjson`

 * *Files identical despite different names*

### Comparing `gbpcli-1.5.0/tests/data/list.json` & `gbpcli-1.5.1/tests/data/list.json`

 * *Files identical despite different names*

### Comparing `gbpcli-1.5.0/tests/data/list_with_packages.json` & `gbpcli-1.5.1/tests/data/list_with_packages.json`

 * *Files identical despite different names*

### Comparing `gbpcli-1.5.0/tests/data/machines.json` & `gbpcli-1.5.1/tests/data/machines.json`

 * *Files identical despite different names*

### Comparing `gbpcli-1.5.0/tests/data/packages.json` & `gbpcli-1.5.1/tests/data/packages.json`

 * *Files identical despite different names*

### Comparing `gbpcli-1.5.0/tests/data/packages.txt` & `gbpcli-1.5.1/tests/data/packages.txt`

 * *Files identical despite different names*

### Comparing `gbpcli-1.5.0/tests/data/status.json` & `gbpcli-1.5.1/tests/data/status.json`

 * *Files identical despite different names*

### Comparing `gbpcli-1.5.0/tests/test_build.py` & `gbpcli-1.5.1/tests/test_build.py`

 * *Files identical despite different names*

### Comparing `gbpcli-1.5.0/tests/test_diff.py` & `gbpcli-1.5.1/tests/test_diff.py`

 * *Files identical despite different names*

### Comparing `gbpcli-1.5.0/tests/test_entrypoint.py` & `gbpcli-1.5.1/tests/test_entrypoint.py`

 * *Files identical despite different names*

### Comparing `gbpcli-1.5.0/tests/test_gbp.py` & `gbpcli-1.5.1/tests/test_gbp.py`

 * *Files identical despite different names*

### Comparing `gbpcli-1.5.0/tests/test_graphql.py` & `gbpcli-1.5.1/tests/test_graphql.py`

 * *Files 5% similar despite different names*

```diff
@@ -44,29 +44,29 @@
         self.assertEqual(response, ({"foo": "bar"}, [{"this": "that"}]))
 
 
 class QueriesTestCase(unittest.TestCase):
     """Tests for the Queries wrapper"""
 
     def test_returns_query_on_attribute_access(self):
-        queries = graphql.Queries(URL("https://gbp.invalid"))
+        queries = graphql.Queries(URL("https://gbp.invalid"), "gbpcli")
 
         logs_query = queries.logs
 
         self.assertEqual(
             logs_query.query,
             "query ($id: ID!) {\n  build(id: $id) {\n    logs\n  }\n}\n",
         )
 
     def test_raises_attribute_error_when_file_not_found(self):
-        queries = graphql.Queries(URL("https://gbp.invalid"))
+        queries = graphql.Queries(URL("https://gbp.invalid"), "gbpcli")
 
         with self.assertRaises(AttributeError):
             print(queries.bogus)
 
     def test_to_dict_returns_dict(self):
-        queries = graphql.Queries(URL("https://gbp.invalid"))
+        queries = graphql.Queries(URL("https://gbp.invalid"), "gbpcli")
 
         as_dict = queries.to_dict()
 
         self.assertIsInstance(as_dict, dict)
         self.assertIn("logs", as_dict)
```

### Comparing `gbpcli-1.5.0/tests/test_inspect.py` & `gbpcli-1.5.1/tests/test_inspect.py`

 * *Files identical despite different names*

### Comparing `gbpcli-1.5.0/tests/test_keep.py` & `gbpcli-1.5.1/tests/test_keep.py`

 * *Files identical despite different names*

### Comparing `gbpcli-1.5.0/tests/test_latest.py` & `gbpcli-1.5.1/tests/test_latest.py`

 * *Files identical despite different names*

### Comparing `gbpcli-1.5.0/tests/test_list.py` & `gbpcli-1.5.1/tests/test_list.py`

 * *Files identical despite different names*

### Comparing `gbpcli-1.5.0/tests/test_logs.py` & `gbpcli-1.5.1/tests/test_logs.py`

 * *Files identical despite different names*

### Comparing `gbpcli-1.5.0/tests/test_machines.py` & `gbpcli-1.5.1/tests/test_machines.py`

 * *Files identical despite different names*

### Comparing `gbpcli-1.5.0/tests/test_notes.py` & `gbpcli-1.5.1/tests/test_notes.py`

 * *Files identical despite different names*

### Comparing `gbpcli-1.5.0/tests/test_packages.py` & `gbpcli-1.5.1/tests/test_packages.py`

 * *Files identical despite different names*

### Comparing `gbpcli-1.5.0/tests/test_publish.py` & `gbpcli-1.5.1/tests/test_publish.py`

 * *Files identical despite different names*

### Comparing `gbpcli-1.5.0/tests/test_pull.py` & `gbpcli-1.5.1/tests/test_pull.py`

 * *Files identical despite different names*

### Comparing `gbpcli-1.5.0/tests/test_render.py` & `gbpcli-1.5.1/tests/test_render.py`

 * *Files identical despite different names*

### Comparing `gbpcli-1.5.0/tests/test_status.py` & `gbpcli-1.5.1/tests/test_status.py`

 * *Files identical despite different names*

### Comparing `gbpcli-1.5.0/tests/test_tag.py` & `gbpcli-1.5.1/tests/test_tag.py`

 * *Files identical despite different names*

### Comparing `gbpcli-1.5.0/tests/test_theme.py` & `gbpcli-1.5.1/tests/test_theme.py`

 * *Files identical despite different names*

### Comparing `gbpcli-1.5.0/tests/test_utils.py` & `gbpcli-1.5.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `gbpcli-1.5.0/PKG-INFO` & `gbpcli-1.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gbpcli
-Version: 1.5.0
+Version: 1.5.1
 Summary: Gentoo Build Publisher Command-Line Interface
 Home-page: https://github.com/enku/gbpcli
 Author-Email: Albert Hopkins <marduk@letterboxes.org>
 License: GPL3+
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: POSIX :: Linux
```

