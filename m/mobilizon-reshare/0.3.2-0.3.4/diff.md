# Comparing `tmp/mobilizon-reshare-0.3.2.tar.gz` & `tmp/mobilizon-reshare-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mobilizon-reshare-0.3.2.tar", max compression
+gzip compressed data, was "mobilizon-reshare-0.3.4.tar", max compression
```

## Comparing `mobilizon-reshare-0.3.2.tar` & `mobilizon-reshare-0.3.4.tar`

### file list

```diff
@@ -1,87 +1,107 @@
--rw-r--r--   0        0        0    29018 2022-01-03 20:42:30.699596 mobilizon-reshare-0.3.2/LICENSE
--rw-r--r--   0        0        0     2614 2022-06-05 17:08:37.572932 mobilizon-reshare-0.3.2/README.md
--rw-r--r--   0        0        0      884 2022-04-23 20:51:58.470562 mobilizon-reshare-0.3.2/mobilizon_reshare/.secrets.toml
--rw-r--r--   0        0        0        5 2022-06-05 17:12:05.995865 mobilizon-reshare-0.3.2/mobilizon_reshare/VERSION
--rw-r--r--   0        0        0        0 2022-01-03 20:42:30.703595 mobilizon-reshare-0.3.2/mobilizon_reshare/__init__.py
--rw-r--r--   0        0        0       89 2022-04-23 20:51:58.470562 mobilizon-reshare-0.3.2/mobilizon_reshare/aerich.ini
--rw-r--r--   0        0        0      848 2022-04-23 20:51:58.470562 mobilizon-reshare-0.3.2/mobilizon_reshare/cli/__init__.py
--rw-r--r--   0        0        0     6594 2022-05-17 21:59:32.529136 mobilizon-reshare-0.3.2/mobilizon_reshare/cli/cli.py
--rw-r--r--   0        0        0        0 2022-01-07 23:10:25.294923 mobilizon-reshare-0.3.2/mobilizon_reshare/cli/commands/__init__.py
--rw-r--r--   0        0        0        0 2022-01-07 23:10:25.294923 mobilizon-reshare-0.3.2/mobilizon_reshare/cli/commands/format/__init__.py
--rw-r--r--   0        0        0      640 2022-04-23 20:51:58.470562 mobilizon-reshare-0.3.2/mobilizon_reshare/cli/commands/format/format.py
--rw-r--r--   0        0        0        0 2022-04-23 20:51:58.470562 mobilizon-reshare-0.3.2/mobilizon_reshare/cli/commands/list/__init__.py
--rw-r--r--   0        0        0     2176 2022-04-23 20:51:58.470562 mobilizon-reshare-0.3.2/mobilizon_reshare/cli/commands/list/list_event.py
--rw-r--r--   0        0        0     1540 2022-04-23 20:51:58.470562 mobilizon-reshare-0.3.2/mobilizon_reshare/cli/commands/list/list_publication.py
--rw-r--r--   0        0        0        0 2022-04-23 20:51:58.470562 mobilizon-reshare-0.3.2/mobilizon_reshare/cli/commands/publish/__init__.py
--rw-r--r--   0        0        0      356 2022-05-17 21:59:32.529136 mobilizon-reshare-0.3.2/mobilizon_reshare/cli/commands/publish/main.py
--rw-r--r--   0        0        0        0 2022-04-23 20:51:58.470562 mobilizon-reshare-0.3.2/mobilizon_reshare/cli/commands/pull/__init__.py
--rw-r--r--   0        0        0      141 2022-04-23 20:51:58.474562 mobilizon-reshare-0.3.2/mobilizon_reshare/cli/commands/pull/main.py
--rw-r--r--   0        0        0        0 2022-01-07 23:10:25.294923 mobilizon-reshare-0.3.2/mobilizon_reshare/cli/commands/recap/__init__.py
--rw-r--r--   0        0        0      220 2022-04-23 20:51:58.474562 mobilizon-reshare-0.3.2/mobilizon_reshare/cli/commands/recap/main.py
--rw-r--r--   0        0        0        0 2022-04-23 20:51:58.474562 mobilizon-reshare-0.3.2/mobilizon_reshare/cli/commands/retry/__init__.py
--rw-r--r--   0        0        0      374 2022-05-16 23:50:55.144670 mobilizon-reshare-0.3.2/mobilizon_reshare/cli/commands/retry/main.py
--rw-r--r--   0        0        0        0 2022-03-08 22:37:48.136023 mobilizon-reshare-0.3.2/mobilizon_reshare/cli/commands/start/__init__.py
--rw-r--r--   0        0        0      196 2022-04-23 20:51:58.474562 mobilizon-reshare-0.3.2/mobilizon_reshare/cli/commands/start/main.py
--rw-r--r--   0        0        0        0 2022-01-03 20:42:30.703595 mobilizon-reshare-0.3.2/mobilizon_reshare/config/__init__.py
--rw-r--r--   0        0        0     4850 2022-04-23 20:51:58.474562 mobilizon-reshare-0.3.2/mobilizon_reshare/config/config.py
--rw-r--r--   0        0        0     1849 2022-04-23 20:51:58.474562 mobilizon-reshare-0.3.2/mobilizon_reshare/config/notifiers.py
--rw-r--r--   0        0        0     3325 2022-04-23 20:51:58.474562 mobilizon-reshare-0.3.2/mobilizon_reshare/config/publishers.py
--rw-r--r--   0        0        0      343 2022-01-03 20:42:30.703595 mobilizon-reshare-0.3.2/mobilizon_reshare/config/strategies.py
--rw-r--r--   0        0        0        0 2022-01-03 20:42:30.703595 mobilizon-reshare-0.3.2/mobilizon_reshare/event/__init__.py
--rw-r--r--   0        0        0     1535 2022-04-23 20:51:58.474562 mobilizon-reshare-0.3.2/mobilizon_reshare/event/event.py
--rw-r--r--   0        0        0     3090 2022-05-17 21:59:32.529136 mobilizon-reshare-0.3.2/mobilizon_reshare/event/event_selection_strategies.py
--rw-r--r--   0        0        0        0 2022-01-03 20:42:30.703595 mobilizon-reshare-0.3.2/mobilizon_reshare/formatting/__init__.py
--rw-r--r--   0        0        0      789 2022-04-23 20:51:58.474562 mobilizon-reshare-0.3.2/mobilizon_reshare/formatting/description.py
--rw-r--r--   0        0        0        0 2022-01-07 23:10:25.294923 mobilizon-reshare-0.3.2/mobilizon_reshare/main/__init__.py
--rw-r--r--   0        0        0     2123 2022-05-17 21:59:32.529136 mobilizon-reshare-0.3.2/mobilizon_reshare/main/publish.py
--rw-r--r--   0        0        0      780 2022-04-23 20:51:58.474562 mobilizon-reshare-0.3.2/mobilizon_reshare/main/pull.py
--rw-r--r--   0        0        0     1759 2022-04-23 20:51:58.474562 mobilizon-reshare-0.3.2/mobilizon_reshare/main/recap.py
--rw-r--r--   0        0        0     1681 2022-05-17 21:59:32.529136 mobilizon-reshare-0.3.2/mobilizon_reshare/main/retry.py
--rw-r--r--   0        0        0      445 2022-05-17 21:59:32.529136 mobilizon-reshare-0.3.2/mobilizon_reshare/main/start.py
--rw-r--r--   0        0        0     1396 2022-04-23 20:51:58.474562 mobilizon-reshare-0.3.2/mobilizon_reshare/migrations/models/0_20211207110159_init.sql
--rw-r--r--   0        0        0      155 2022-04-23 20:51:58.474562 mobilizon-reshare-0.3.2/mobilizon_reshare/migrations/models/1_20211218165547_add column last_update_time for event.sql
--rw-r--r--   0        0        0        0 2022-01-03 20:42:30.703595 mobilizon-reshare-0.3.2/mobilizon_reshare/mobilizon/__init__.py
--rw-r--r--   0        0        0     3259 2022-04-23 20:51:58.474562 mobilizon-reshare-0.3.2/mobilizon_reshare/mobilizon/events.py
--rw-r--r--   0        0        0        0 2022-01-03 20:42:30.703595 mobilizon-reshare-0.3.2/mobilizon_reshare/models/__init__.py
--rw-r--r--   0        0        0     1258 2022-04-23 20:51:58.474562 mobilizon-reshare-0.3.2/mobilizon_reshare/models/event.py
--rw-r--r--   0        0        0      693 2022-01-03 20:42:30.703595 mobilizon-reshare-0.3.2/mobilizon_reshare/models/notification.py
--rw-r--r--   0        0        0      621 2022-04-23 20:51:58.474562 mobilizon-reshare-0.3.2/mobilizon_reshare/models/publication.py
--rw-r--r--   0        0        0      401 2022-01-03 20:42:30.703595 mobilizon-reshare-0.3.2/mobilizon_reshare/models/publisher.py
--rw-r--r--   0        0        0      371 2022-01-03 20:42:30.703595 mobilizon-reshare-0.3.2/mobilizon_reshare/publishers/__init__.py
--rw-r--r--   0        0        0     5947 2022-04-23 20:51:58.474562 mobilizon-reshare-0.3.2/mobilizon_reshare/publishers/abstract.py
--rw-r--r--   0        0        0     6800 2022-05-17 21:59:32.529136 mobilizon-reshare-0.3.2/mobilizon_reshare/publishers/coordinator.py
--rw-r--r--   0        0        0      911 2022-04-23 20:51:58.474562 mobilizon-reshare-0.3.2/mobilizon_reshare/publishers/exceptions.py
--rw-r--r--   0        0        0        0 2022-01-07 23:10:25.298923 mobilizon-reshare-0.3.2/mobilizon_reshare/publishers/platforms/__init__.py
--rw-r--r--   0        0        0     2922 2022-04-23 20:51:58.474562 mobilizon-reshare-0.3.2/mobilizon_reshare/publishers/platforms/facebook.py
--rw-r--r--   0        0        0     3211 2022-04-23 20:51:58.474562 mobilizon-reshare-0.3.2/mobilizon_reshare/publishers/platforms/mastodon.py
--rw-r--r--   0        0        0     1783 2022-04-23 20:51:58.474562 mobilizon-reshare-0.3.2/mobilizon_reshare/publishers/platforms/platform_mapping.py
--rw-r--r--   0        0        0     4342 2022-04-23 20:51:58.474562 mobilizon-reshare-0.3.2/mobilizon_reshare/publishers/platforms/telegram.py
--rw-r--r--   0        0        0     2644 2022-04-23 20:51:58.474562 mobilizon-reshare-0.3.2/mobilizon_reshare/publishers/platforms/twitter.py
--rw-r--r--   0        0        0     4023 2022-04-23 20:51:58.474562 mobilizon-reshare-0.3.2/mobilizon_reshare/publishers/platforms/zulip.py
--rw-r--r--   0        0        0        0 2022-01-03 20:42:30.703595 mobilizon-reshare-0.3.2/mobilizon_reshare/publishers/templates/__init__.py
--rw-r--r--   0        0        0      263 2022-04-23 20:51:58.474562 mobilizon-reshare-0.3.2/mobilizon_reshare/publishers/templates/facebook.tmpl.j2
--rw-r--r--   0        0        0      244 2022-04-23 20:51:58.474562 mobilizon-reshare-0.3.2/mobilizon_reshare/publishers/templates/facebook_recap.tmpl.j2
--rw-r--r--   0        0        0       20 2022-04-23 20:51:58.474562 mobilizon-reshare-0.3.2/mobilizon_reshare/publishers/templates/facebook_recap_header.tmpl.j2
--rw-r--r--   0        0        0      238 2022-04-23 20:51:58.474562 mobilizon-reshare-0.3.2/mobilizon_reshare/publishers/templates/mastodon.tmpl.j2
--rw-r--r--   0        0        0      234 2022-04-23 20:51:58.474562 mobilizon-reshare-0.3.2/mobilizon_reshare/publishers/templates/mastodon_recap.tmpl.j2
--rw-r--r--   0        0        0       20 2022-01-07 23:10:25.298923 mobilizon-reshare-0.3.2/mobilizon_reshare/publishers/templates/mastodon_recap_header.tmpl.j2
--rw-r--r--   0        0        0      290 2022-04-23 20:51:58.474562 mobilizon-reshare-0.3.2/mobilizon_reshare/publishers/templates/telegram.tmpl.j2
--rw-r--r--   0        0        0      270 2022-04-23 20:51:58.474562 mobilizon-reshare-0.3.2/mobilizon_reshare/publishers/templates/telegram_recap.tmpl.j2
--rw-r--r--   0        0        0       20 2022-04-23 20:51:58.474562 mobilizon-reshare-0.3.2/mobilizon_reshare/publishers/templates/telegram_recap_header.tmpl.j2
--rw-r--r--   0        0        0      239 2022-04-23 20:51:58.474562 mobilizon-reshare-0.3.2/mobilizon_reshare/publishers/templates/twitter.tmpl.j2
--rw-r--r--   0        0        0      236 2022-04-23 20:51:58.474562 mobilizon-reshare-0.3.2/mobilizon_reshare/publishers/templates/twitter_recap.tmpl.j2
--rw-r--r--   0        0        0       20 2022-04-23 20:51:58.474562 mobilizon-reshare-0.3.2/mobilizon_reshare/publishers/templates/twitter_recap_header.tmpl.j2
--rw-r--r--   0        0        0      267 2022-04-23 20:51:58.474562 mobilizon-reshare-0.3.2/mobilizon_reshare/publishers/templates/zulip.tmpl.j2
--rw-r--r--   0        0        0      248 2022-04-23 20:51:58.474562 mobilizon-reshare-0.3.2/mobilizon_reshare/publishers/templates/zulip_recap.tmpl.j2
--rw-r--r--   0        0        0       20 2022-04-23 20:51:58.474562 mobilizon-reshare-0.3.2/mobilizon_reshare/publishers/templates/zulip_recap_header.tmpl.j2
--rw-r--r--   0        0        0      956 2022-04-23 20:51:58.474562 mobilizon-reshare-0.3.2/mobilizon_reshare/settings.toml
--rw-r--r--   0        0        0        0 2022-01-03 20:42:30.703595 mobilizon-reshare-0.3.2/mobilizon_reshare/storage/__init__.py
--rw-r--r--   0        0        0     2425 2022-04-23 20:51:58.474562 mobilizon-reshare-0.3.2/mobilizon_reshare/storage/db.py
--rw-r--r--   0        0        0       76 2022-04-23 20:51:58.474562 mobilizon-reshare-0.3.2/mobilizon_reshare/storage/query/__init__.py
--rw-r--r--   0        0        0     3063 2022-04-23 20:51:58.474562 mobilizon-reshare-0.3.2/mobilizon_reshare/storage/query/converter.py
--rw-r--r--   0        0        0      181 2022-04-23 20:51:58.474562 mobilizon-reshare-0.3.2/mobilizon_reshare/storage/query/exceptions.py
--rw-r--r--   0        0        0     6620 2022-05-17 21:59:32.529136 mobilizon-reshare-0.3.2/mobilizon_reshare/storage/query/read.py
--rw-r--r--   0        0        0     3471 2022-04-23 20:51:58.474562 mobilizon-reshare-0.3.2/mobilizon_reshare/storage/query/write.py
--rw-r--r--   0        0        0     1149 2022-06-05 17:12:05.995865 mobilizon-reshare-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     4638 2022-06-05 17:12:09.536411 mobilizon-reshare-0.3.2/setup.py
--rw-r--r--   0        0        0     3774 2022-06-05 17:12:09.536670 mobilizon-reshare-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0    29018 2022-12-22 21:26:57.662251 mobilizon-reshare-0.3.4/LICENSE
+-rw-r--r--   0        0        0     2601 2023-06-09 22:02:31.511598 mobilizon-reshare-0.3.4/README.md
+-rw-r--r--   0        0        0      884 2022-12-22 21:26:57.662251 mobilizon-reshare-0.3.4/mobilizon_reshare/.secrets.toml
+-rw-r--r--   0        0        0        5 2023-06-10 21:12:54.492721 mobilizon-reshare-0.3.4/mobilizon_reshare/VERSION
+-rw-r--r--   0        0        0        0 2022-12-22 21:26:57.662251 mobilizon-reshare-0.3.4/mobilizon_reshare/__init__.py
+-rw-r--r--   0        0        0      786 2023-06-09 22:02:31.543598 mobilizon-reshare-0.3.4/mobilizon_reshare/cli/__init__.py
+-rw-r--r--   0        0        0     7120 2023-06-09 22:02:31.519598 mobilizon-reshare-0.3.4/mobilizon_reshare/cli/cli.py
+-rw-r--r--   0        0        0       75 2023-06-09 22:02:31.503598 mobilizon-reshare-0.3.4/mobilizon_reshare/cli/commands/__init__.py
+-rw-r--r--   0        0        0        0 2022-12-22 21:26:57.662251 mobilizon-reshare-0.3.4/mobilizon_reshare/cli/commands/format/__init__.py
+-rw-r--r--   0        0        0      635 2023-06-09 22:02:31.511598 mobilizon-reshare-0.3.4/mobilizon_reshare/cli/commands/format/format.py
+-rw-r--r--   0        0        0        0 2022-12-22 21:26:57.662251 mobilizon-reshare-0.3.4/mobilizon_reshare/cli/commands/list/__init__.py
+-rw-r--r--   0        0        0     2265 2023-06-09 22:02:31.491598 mobilizon-reshare-0.3.4/mobilizon_reshare/cli/commands/list/list_event.py
+-rw-r--r--   0        0        0     1540 2023-06-09 22:02:31.491598 mobilizon-reshare-0.3.4/mobilizon_reshare/cli/commands/list/list_publication.py
+-rw-r--r--   0        0        0        0 2022-12-22 21:26:57.662251 mobilizon-reshare-0.3.4/mobilizon_reshare/cli/commands/publish/__init__.py
+-rw-r--r--   0        0        0      356 2023-06-09 22:02:31.535598 mobilizon-reshare-0.3.4/mobilizon_reshare/cli/commands/publish/main.py
+-rw-r--r--   0        0        0        0 2022-12-22 21:26:57.662251 mobilizon-reshare-0.3.4/mobilizon_reshare/cli/commands/pull/__init__.py
+-rw-r--r--   0        0        0      141 2023-06-09 22:02:31.527598 mobilizon-reshare-0.3.4/mobilizon_reshare/cli/commands/pull/main.py
+-rw-r--r--   0        0        0        0 2022-12-22 21:26:57.662251 mobilizon-reshare-0.3.4/mobilizon_reshare/cli/commands/recap/__init__.py
+-rw-r--r--   0        0        0      453 2023-06-09 22:02:31.523598 mobilizon-reshare-0.3.4/mobilizon_reshare/cli/commands/recap/main.py
+-rw-r--r--   0        0        0        0 2022-12-22 21:26:57.662251 mobilizon-reshare-0.3.4/mobilizon_reshare/cli/commands/retry/__init__.py
+-rw-r--r--   0        0        0      374 2023-06-09 22:02:31.519598 mobilizon-reshare-0.3.4/mobilizon_reshare/cli/commands/retry/main.py
+-rw-r--r--   0        0        0        0 2022-12-22 21:26:57.662251 mobilizon-reshare-0.3.4/mobilizon_reshare/cli/commands/start/__init__.py
+-rw-r--r--   0        0        0      429 2023-06-09 22:02:31.523598 mobilizon-reshare-0.3.4/mobilizon_reshare/cli/commands/start/main.py
+-rw-r--r--   0        0        0        0 2022-12-22 21:26:57.662251 mobilizon-reshare-0.3.4/mobilizon_reshare/config/__init__.py
+-rw-r--r--   0        0        0      118 2023-06-09 22:02:31.547598 mobilizon-reshare-0.3.4/mobilizon_reshare/config/command.py
+-rw-r--r--   0        0        0     4918 2023-06-09 22:02:31.531598 mobilizon-reshare-0.3.4/mobilizon_reshare/config/config.py
+-rw-r--r--   0        0        0     1849 2022-12-22 21:26:57.662251 mobilizon-reshare-0.3.4/mobilizon_reshare/config/notifiers.py
+-rw-r--r--   0        0        0     3325 2022-12-22 21:26:57.662251 mobilizon-reshare-0.3.4/mobilizon_reshare/config/publishers.py
+-rw-r--r--   0        0        0      343 2022-12-22 21:26:57.662251 mobilizon-reshare-0.3.4/mobilizon_reshare/config/strategies.py
+-rw-r--r--   0        0        0      445 2023-06-09 22:02:31.547598 mobilizon-reshare-0.3.4/mobilizon_reshare/dataclasses/__init__.py
+-rw-r--r--   0        0        0     5478 2023-06-09 22:02:31.531598 mobilizon-reshare-0.3.4/mobilizon_reshare/dataclasses/event.py
+-rw-r--r--   0        0        0      805 2023-06-09 22:02:31.531598 mobilizon-reshare-0.3.4/mobilizon_reshare/dataclasses/event_publication_status.py
+-rw-r--r--   0        0        0     2282 2023-06-09 22:02:31.539598 mobilizon-reshare-0.3.4/mobilizon_reshare/dataclasses/publication.py
+-rw-r--r--   0        0        0        0 2022-12-22 21:26:57.666251 mobilizon-reshare-0.3.4/mobilizon_reshare/event/__init__.py
+-rw-r--r--   0        0        0     3090 2023-06-09 22:02:31.547598 mobilizon-reshare-0.3.4/mobilizon_reshare/event/event_selection_strategies.py
+-rw-r--r--   0        0        0        0 2022-12-22 21:26:57.666251 mobilizon-reshare-0.3.4/mobilizon_reshare/formatting/__init__.py
+-rw-r--r--   0        0        0      789 2023-06-09 22:02:31.531598 mobilizon-reshare-0.3.4/mobilizon_reshare/formatting/description.py
+-rw-r--r--   0        0        0        0 2022-12-22 21:26:57.666251 mobilizon-reshare-0.3.4/mobilizon_reshare/main/__init__.py
+-rw-r--r--   0        0        0     2972 2023-06-09 22:02:31.535598 mobilizon-reshare-0.3.4/mobilizon_reshare/main/publish.py
+-rw-r--r--   0        0        0      770 2023-06-09 22:02:31.499598 mobilizon-reshare-0.3.4/mobilizon_reshare/main/pull.py
+-rw-r--r--   0        0        0     2309 2023-06-09 22:02:31.523598 mobilizon-reshare-0.3.4/mobilizon_reshare/main/recap.py
+-rw-r--r--   0        0        0     1875 2023-06-09 22:02:31.551598 mobilizon-reshare-0.3.4/mobilizon_reshare/main/retry.py
+-rw-r--r--   0        0        0      547 2023-06-09 22:02:31.523598 mobilizon-reshare-0.3.4/mobilizon_reshare/main/start.py
+-rwxr-xr-x   0        0        0     1488 2023-06-09 22:02:31.495598 mobilizon-reshare-0.3.4/mobilizon_reshare/migrations/postgres/models/0_20221006223256_init.sql
+-rw-r--r--   0        0        0      108 2023-06-09 22:02:31.539598 mobilizon-reshare-0.3.4/mobilizon_reshare/migrations/postgres/pyproject.toml
+-rw-r--r--   0        0        0     1396 2022-12-22 21:26:57.666251 mobilizon-reshare-0.3.4/mobilizon_reshare/migrations/sqlite/models/0_20211207110159_init.sql
+-rw-r--r--   0        0        0      155 2023-06-09 22:02:31.503598 mobilizon-reshare-0.3.4/mobilizon_reshare/migrations/sqlite/models/1_20211218165547_add column last_update_time for event.sql
+-rw-r--r--   0        0        0      107 2023-06-09 22:02:31.527598 mobilizon-reshare-0.3.4/mobilizon_reshare/migrations/sqlite/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-12-22 21:26:57.666251 mobilizon-reshare-0.3.4/mobilizon_reshare/mobilizon/__init__.py
+-rw-r--r--   0        0        0     3261 2023-06-09 22:02:31.551598 mobilizon-reshare-0.3.4/mobilizon_reshare/mobilizon/events.py
+-rw-r--r--   0        0        0      169 2023-06-09 22:02:31.547598 mobilizon-reshare-0.3.4/mobilizon_reshare/models/__init__.py
+-rw-r--r--   0        0        0     1843 2023-06-09 22:02:31.507598 mobilizon-reshare-0.3.4/mobilizon_reshare/models/event.py
+-rw-r--r--   0        0        0      638 2023-06-09 22:02:31.491598 mobilizon-reshare-0.3.4/mobilizon_reshare/models/notification.py
+-rw-r--r--   0        0        0      686 2023-06-09 22:02:31.551598 mobilizon-reshare-0.3.4/mobilizon_reshare/models/publication.py
+-rw-r--r--   0        0        0      401 2022-12-22 21:26:57.666251 mobilizon-reshare-0.3.4/mobilizon_reshare/models/publisher.py
+-rw-r--r--   0        0        0      434 2023-06-09 22:02:31.531598 mobilizon-reshare-0.3.4/mobilizon_reshare/publishers/__init__.py
+-rw-r--r--   0        0        0     5590 2023-06-09 22:02:31.519598 mobilizon-reshare-0.3.4/mobilizon_reshare/publishers/abstract.py
+-rw-r--r--   0        0        0        0 2022-12-22 21:26:57.666251 mobilizon-reshare-0.3.4/mobilizon_reshare/publishers/coordinator.py
+-rw-r--r--   0        0        0      731 2023-06-09 22:02:31.527598 mobilizon-reshare-0.3.4/mobilizon_reshare/publishers/coordinators/__init__.py
+-rw-r--r--   0        0        0     2298 2023-06-09 22:02:31.527598 mobilizon-reshare-0.3.4/mobilizon_reshare/publishers/coordinators/event_publishing/__init__.py
+-rw-r--r--   0        0        0      915 2023-06-09 22:02:31.491598 mobilizon-reshare-0.3.4/mobilizon_reshare/publishers/coordinators/event_publishing/dry_run.py
+-rw-r--r--   0        0        0     4213 2023-06-09 22:02:31.527598 mobilizon-reshare-0.3.4/mobilizon_reshare/publishers/coordinators/event_publishing/notify.py
+-rw-r--r--   0        0        0     2895 2023-06-09 22:02:31.515598 mobilizon-reshare-0.3.4/mobilizon_reshare/publishers/coordinators/event_publishing/publish.py
+-rw-r--r--   0        0        0        0 2022-12-22 21:26:57.666251 mobilizon-reshare-0.3.4/mobilizon_reshare/publishers/coordinators/recap_publishing/__init__.py
+-rw-r--r--   0        0        0      637 2023-06-09 22:02:31.515598 mobilizon-reshare-0.3.4/mobilizon_reshare/publishers/coordinators/recap_publishing/dry_run.py
+-rw-r--r--   0        0        0     2620 2023-06-09 22:02:31.535598 mobilizon-reshare-0.3.4/mobilizon_reshare/publishers/coordinators/recap_publishing/recap.py
+-rw-r--r--   0        0        0      911 2023-06-09 22:02:31.499598 mobilizon-reshare-0.3.4/mobilizon_reshare/publishers/exceptions.py
+-rw-r--r--   0        0        0        0 2022-12-22 21:26:57.666251 mobilizon-reshare-0.3.4/mobilizon_reshare/publishers/platforms/__init__.py
+-rw-r--r--   0        0        0     2922 2023-06-09 22:02:31.543598 mobilizon-reshare-0.3.4/mobilizon_reshare/publishers/platforms/facebook.py
+-rw-r--r--   0        0        0     3211 2023-06-09 22:02:31.519598 mobilizon-reshare-0.3.4/mobilizon_reshare/publishers/platforms/mastodon.py
+-rw-r--r--   0        0        0     1783 2022-12-22 21:26:57.666251 mobilizon-reshare-0.3.4/mobilizon_reshare/publishers/platforms/platform_mapping.py
+-rw-r--r--   0        0        0     4378 2023-06-09 22:02:31.535598 mobilizon-reshare-0.3.4/mobilizon_reshare/publishers/platforms/telegram.py
+-rw-r--r--   0        0        0     2644 2023-06-09 22:02:31.487598 mobilizon-reshare-0.3.4/mobilizon_reshare/publishers/platforms/twitter.py
+-rw-r--r--   0        0        0     4028 2023-06-09 22:02:31.519598 mobilizon-reshare-0.3.4/mobilizon_reshare/publishers/platforms/zulip.py
+-rw-r--r--   0        0        0        0 2022-12-22 21:26:57.666251 mobilizon-reshare-0.3.4/mobilizon_reshare/publishers/templates/__init__.py
+-rw-r--r--   0        0        0      263 2023-06-09 22:02:31.519598 mobilizon-reshare-0.3.4/mobilizon_reshare/publishers/templates/facebook.tmpl.j2
+-rw-r--r--   0        0        0      244 2023-06-09 22:02:31.519598 mobilizon-reshare-0.3.4/mobilizon_reshare/publishers/templates/facebook_recap.tmpl.j2
+-rw-r--r--   0        0        0       20 2022-12-22 21:26:57.666251 mobilizon-reshare-0.3.4/mobilizon_reshare/publishers/templates/facebook_recap_header.tmpl.j2
+-rw-r--r--   0        0        0      238 2023-06-09 22:02:31.543598 mobilizon-reshare-0.3.4/mobilizon_reshare/publishers/templates/mastodon.tmpl.j2
+-rw-r--r--   0        0        0      234 2023-06-09 22:02:31.519598 mobilizon-reshare-0.3.4/mobilizon_reshare/publishers/templates/mastodon_recap.tmpl.j2
+-rw-r--r--   0        0        0       20 2022-12-22 21:26:57.666251 mobilizon-reshare-0.3.4/mobilizon_reshare/publishers/templates/mastodon_recap_header.tmpl.j2
+-rw-r--r--   0        0        0      290 2023-06-09 22:02:31.519598 mobilizon-reshare-0.3.4/mobilizon_reshare/publishers/templates/telegram.tmpl.j2
+-rw-r--r--   0        0        0      270 2023-06-09 22:02:31.531598 mobilizon-reshare-0.3.4/mobilizon_reshare/publishers/templates/telegram_recap.tmpl.j2
+-rw-r--r--   0        0        0       20 2022-12-22 21:26:57.666251 mobilizon-reshare-0.3.4/mobilizon_reshare/publishers/templates/telegram_recap_header.tmpl.j2
+-rw-r--r--   0        0        0      239 2023-06-09 22:02:31.527598 mobilizon-reshare-0.3.4/mobilizon_reshare/publishers/templates/twitter.tmpl.j2
+-rw-r--r--   0        0        0      236 2023-06-09 22:02:31.515598 mobilizon-reshare-0.3.4/mobilizon_reshare/publishers/templates/twitter_recap.tmpl.j2
+-rw-r--r--   0        0        0       20 2022-12-22 21:26:57.666251 mobilizon-reshare-0.3.4/mobilizon_reshare/publishers/templates/twitter_recap_header.tmpl.j2
+-rw-r--r--   0        0        0      267 2023-06-09 22:02:31.499598 mobilizon-reshare-0.3.4/mobilizon_reshare/publishers/templates/zulip.tmpl.j2
+-rw-r--r--   0        0        0      248 2023-06-09 22:02:31.499598 mobilizon-reshare-0.3.4/mobilizon_reshare/publishers/templates/zulip_recap.tmpl.j2
+-rw-r--r--   0        0        0       20 2022-12-22 21:26:57.666251 mobilizon-reshare-0.3.4/mobilizon_reshare/publishers/templates/zulip_recap_header.tmpl.j2
+-rw-r--r--   0        0        0      929 2023-06-09 22:02:31.543598 mobilizon-reshare-0.3.4/mobilizon_reshare/settings.toml
+-rw-r--r--   0        0        0        0 2022-12-22 21:26:57.666251 mobilizon-reshare-0.3.4/mobilizon_reshare/storage/__init__.py
+-rw-r--r--   0        0        0     3010 2023-06-09 22:02:31.535598 mobilizon-reshare-0.3.4/mobilizon_reshare/storage/db.py
+-rw-r--r--   0        0        0        0 2022-12-22 21:26:57.666251 mobilizon-reshare-0.3.4/mobilizon_reshare/storage/query/__init__.py
+-rw-r--r--   0        0        0      181 2023-06-09 22:02:31.511598 mobilizon-reshare-0.3.4/mobilizon_reshare/storage/query/exceptions.py
+-rw-r--r--   0        0        0     2960 2023-06-09 22:02:31.499598 mobilizon-reshare-0.3.4/mobilizon_reshare/storage/query/read.py
+-rw-r--r--   0        0        0     4036 2023-06-09 22:02:31.543598 mobilizon-reshare-0.3.4/mobilizon_reshare/storage/query/write.py
+-rw-r--r--   0        0        0        0 2022-12-22 21:26:57.666251 mobilizon-reshare-0.3.4/mobilizon_reshare/web/__init__.py
+-rw-r--r--   0        0        0        0 2022-12-22 21:26:57.666251 mobilizon-reshare-0.3.4/mobilizon_reshare/web/backend/__init__.py
+-rw-r--r--   0        0        0        0 2022-12-22 21:26:57.666251 mobilizon-reshare-0.3.4/mobilizon_reshare/web/backend/events/__init__.py
+-rw-r--r--   0        0        0      341 2023-06-09 22:02:31.531598 mobilizon-reshare-0.3.4/mobilizon_reshare/web/backend/events/endpoints.py
+-rw-r--r--   0        0        0     1077 2023-06-09 22:02:31.519598 mobilizon-reshare-0.3.4/mobilizon_reshare/web/backend/main.py
+-rw-r--r--   0        0        0        0 2022-12-22 21:26:57.666251 mobilizon-reshare-0.3.4/mobilizon_reshare/web/backend/publications/__init__.py
+-rw-r--r--   0        0        0      391 2023-06-09 22:02:31.523598 mobilizon-reshare-0.3.4/mobilizon_reshare/web/backend/publications/endpoints.py
+-rw-r--r--   0        0        0     1269 2023-06-10 21:12:54.496721 mobilizon-reshare-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0     5234 2023-06-10 21:13:08.238247 mobilizon-reshare-0.3.4/setup.py
+-rw-r--r--   0        0        0     3901 2023-06-10 21:13:08.238526 mobilizon-reshare-0.3.4/PKG-INFO
```

### Comparing `mobilizon-reshare-0.3.2/LICENSE` & `mobilizon-reshare-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mobilizon-reshare-0.3.2/README.md` & `mobilizon-reshare-0.3.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 The tool is designed to work in combination with a scheduler that executes it at
 regular intervals. `mobilizon_reshare` allows fine-grained control over the logic to decide when
 to publish an event, with the minimization of human effort as its first priority.
 
 ## Installation
 
-`mobilizon_reshare` is distributed through [Pypi](https://pypi.org/project/mobilizon-reshare/) and [DockerHub](https://hub.docker.com/r/fishinthecalculator/mobilizon-reshare). Use
+`mobilizon_reshare` is distributed through [Pypi](https://pypi.org/project/mobilizon-reshare/) and [DockerHub](https://hub.docker.com/r/twcita/mobilizon-reshare). Use
 
 ```shell
 $ pip install mobilizon-reshare
 ```
 
 to install the tool in your system or virtualenv.
```

### Comparing `mobilizon-reshare-0.3.2/mobilizon_reshare/.secrets.toml` & `mobilizon-reshare-0.3.4/mobilizon_reshare/.secrets.toml`

 * *Files identical despite different names*

### Comparing `mobilizon-reshare-0.3.2/mobilizon_reshare/cli/cli.py` & `mobilizon-reshare-0.3.4/mobilizon_reshare/cli/cli.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 import functools
 
 import click
+import uvicorn
 from click import pass_context
 
 from mobilizon_reshare.cli import safe_execution
 from mobilizon_reshare.cli.commands.format.format import format_event
 from mobilizon_reshare.cli.commands.list.list_event import list_events
 from mobilizon_reshare.cli.commands.list.list_publication import list_publications
-from mobilizon_reshare.cli.commands.recap.main import recap_command as recap_main
-from mobilizon_reshare.cli.commands.start.main import start_command as start_main
-from mobilizon_reshare.cli.commands.pull.main import pull_command as pull_main
 from mobilizon_reshare.cli.commands.publish.main import publish_command as publish_main
-from mobilizon_reshare.config.config import current_version, get_settings
-from mobilizon_reshare.config.publishers import publisher_names
-from mobilizon_reshare.event.event import EventPublicationStatus
+from mobilizon_reshare.cli.commands.pull.main import pull_command as pull_main
+from mobilizon_reshare.cli.commands.recap.main import recap_command as recap_main
 from mobilizon_reshare.cli.commands.retry.main import (
     retry_event_command,
     retry_publication_command,
 )
+from mobilizon_reshare.cli.commands.start.main import start_command as start_main
+from mobilizon_reshare.config.command import CommandConfig
+from mobilizon_reshare.config.config import current_version, get_settings
+from mobilizon_reshare.config.publishers import publisher_names
+from mobilizon_reshare.dataclasses.event import _EventPublicationStatus
 from mobilizon_reshare.models.publication import PublicationStatus
 from mobilizon_reshare.publishers import get_active_publishers
 
 
 def test_settings(ctx, param, value):
     if not value or ctx.resilient_parsing:
         return
@@ -43,18 +45,18 @@
     for platform in get_active_publishers():
         click.echo(platform)
     ctx.exit()
 
 
 status_name_to_enum = {
     "event": {
-        "waiting": EventPublicationStatus.WAITING,
-        "completed": EventPublicationStatus.COMPLETED,
-        "failed": EventPublicationStatus.FAILED,
-        "partial": EventPublicationStatus.PARTIAL,
+        "waiting": _EventPublicationStatus.WAITING,
+        "completed": _EventPublicationStatus.COMPLETED,
+        "failed": _EventPublicationStatus.FAILED,
+        "partial": _EventPublicationStatus.PARTIAL,
         "all": None,
     },
     "publication": {
         "completed": PublicationStatus.COMPLETED,
         "failed": PublicationStatus.FAILED,
         "all": None,
     },
@@ -140,52 +142,54 @@
 def mobilizon_reshare(obj):
     pass
 
 
 @mobilizon_reshare.command(
     help="Synchronize and publish events. It is equivalent to running consecutively pull and then publish."
 )
-@pass_context
-def start(
-    ctx,
-):
-    ctx.ensure_object(dict)
-    safe_execution(
-        start_main,
-    )
+@click.option(
+    "--dry-run",
+    is_flag=True,
+    help="Prevents data to be published to platforms. WARNING: it will download and write new events to the database",
+    default=False,
+)
+def start(dry_run):
+
+    safe_execution(start_main, CommandConfig(dry_run=dry_run))
 
 
 @mobilizon_reshare.command(help="Publish a recap of already published events.")
-def recap():
-    safe_execution(
-        recap_main,
-    )
+@click.option(
+    "--dry-run",
+    "dry_run",
+    is_flag=True,
+    help="Prevents data to be published to platforms. WARNING: it will download and write new events to the database",
+    default=False,
+)
+def recap(dry_run):
+    safe_execution(recap_main, CommandConfig(dry_run=dry_run))
 
 
 @mobilizon_reshare.command(
     help="Fetch the latest events from Mobilizon, store them if they are unknown, "
     "update them if they are known and changed."
 )
 def pull():
-    safe_execution(
-        pull_main,
-    )
+    safe_execution(pull_main,)
 
 
 @mobilizon_reshare.command(
     help="Select an event with the current configured strategy"
     " and publish it to all active platforms."
 )
 @event_uuid_option
 @publication_uuid_option
 @platform_name_option
 def publish():
-    safe_execution(
-        publish_main,
-    )
+    safe_execution(publish_main,)
 
 
 @mobilizon_reshare.group(help="Operations that pertain to events")
 def event():
     pass
 
 
@@ -198,18 +202,15 @@
 @event_status_argument
 @from_date_option
 @to_date_option
 def event_list(status, begin, end):
 
     safe_execution(
         functools.partial(
-            list_events,
-            status_name_to_enum["event"][status],
-            frm=begin,
-            to=end,
+            list_events, status_name_to_enum["event"][status], frm=begin, to=end,
         ),
     )
 
 
 @publication.command(help="Query for publications in the database.", name="list")
 @publication_status_argument
 @from_date_option
@@ -228,33 +229,33 @@
 @event.command(
     help="Format and print event with EVENT-ID using the publisher's format named "
     "PUBLISHER."
 )
 @click.argument("event-id", type=click.UUID)
 @click.argument("publisher", type=click.Choice(publisher_names))
 def format(
-    event_id,
-    publisher,
+    event_id, publisher,
 ):
-    safe_execution(
-        functools.partial(format_event, event_id, publisher),
-    )
+    safe_execution(functools.partial(format_event, event_id, publisher),)
 
 
 @event.command(name="retry", help="Retries all the failed publications")
 @click.argument("event-id", type=click.UUID)
 def event_retry(event_id):
-    safe_execution(
-        functools.partial(retry_event_command, event_id),
-    )
+    safe_execution(functools.partial(retry_event_command, event_id),)
 
 
 @publication.command(name="retry", help="Retries a specific publication")
 @click.argument("publication-id", type=click.UUID)
 def publication_retry(publication_id):
-    safe_execution(
-        functools.partial(retry_publication_command, publication_id),
+    safe_execution(functools.partial(retry_publication_command, publication_id),)
+
+
+@mobilizon_reshare.command("web")
+def web():
+    uvicorn.run(
+        "mobilizon_reshare.web.backend.main:app", host="0.0.0.0", port=8000, reload=True
     )
 
 
 if __name__ == "__main__":
     mobilizon_reshare(obj={})
```

### Comparing `mobilizon-reshare-0.3.2/mobilizon_reshare/cli/commands/format/format.py` & `mobilizon-reshare-0.3.4/mobilizon_reshare/cli/commands/format/format.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import click
 
+from mobilizon_reshare.dataclasses import MobilizonEvent
 from mobilizon_reshare.models.event import Event
 from mobilizon_reshare.publishers.platforms.platform_mapping import get_formatter_class
-from mobilizon_reshare.storage.query.converter import event_from_model
 
 
 async def format_event(event_id, publisher_name: str):
     event = await Event.get_or_none(mobilizon_id=event_id).prefetch_related(
         "publications__publisher"
     )
     if not event:
         click.echo(f"Event with mobilizon_id {event_id} not found.")
         return
-    event = event_from_model(event)
+    event = MobilizonEvent.from_model(event)
     message = get_formatter_class(publisher_name)().get_message_from_event(event)
     click.echo(message)
```

### Comparing `mobilizon-reshare-0.3.2/mobilizon_reshare/cli/commands/list/list_event.py` & `mobilizon-reshare-0.3.4/mobilizon_reshare/cli/commands/list/list_event.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from datetime import datetime
 from typing import Iterable, Optional
 
 import click
 from arrow import Arrow
 
-from mobilizon_reshare.event.event import EventPublicationStatus
-from mobilizon_reshare.event.event import MobilizonEvent
-from mobilizon_reshare.event.event_selection_strategies import select_unpublished_events
-from mobilizon_reshare.storage.query.read import (
+from mobilizon_reshare.dataclasses import MobilizonEvent
+from mobilizon_reshare.dataclasses.event import (
+    _EventPublicationStatus,
+    get_all_mobilizon_events,
     get_published_events,
-    events_with_status,
-    get_all_events,
-    events_without_publications,
+    get_mobilizon_events_with_status,
+    get_mobilizon_events_without_publications,
 )
+from mobilizon_reshare.event.event_selection_strategies import select_unpublished_events
 
 status_to_color = {
-    EventPublicationStatus.COMPLETED: "green",
-    EventPublicationStatus.FAILED: "red",
-    EventPublicationStatus.PARTIAL: "yellow",
-    EventPublicationStatus.WAITING: "white",
+    _EventPublicationStatus.COMPLETED: "green",
+    _EventPublicationStatus.FAILED: "red",
+    _EventPublicationStatus.PARTIAL: "yellow",
+    _EventPublicationStatus.WAITING: "white",
 }
 
 
 def show_events(events: Iterable[MobilizonEvent]):
     click.echo_via_pager("\n".join(map(pretty, events)))
 
 
@@ -34,32 +34,36 @@
         f"{event.end_datetime.to('local').isoformat()}"
     )
 
 
 async def list_unpublished_events(frm: Arrow = None, to: Arrow = None):
     return select_unpublished_events(
         list(await get_published_events(from_date=frm, to_date=to)),
-        list(await events_without_publications(from_date=frm, to_date=to)),
+        list(
+            await get_mobilizon_events_without_publications(from_date=frm, to_date=to)
+        ),
     )
 
 
 async def list_events(
-    status: Optional[EventPublicationStatus] = None,
+    status: Optional[_EventPublicationStatus] = None,
     frm: Optional[datetime] = None,
     to: Optional[datetime] = None,
 ):
 
     frm = Arrow.fromdatetime(frm) if frm else None
     to = Arrow.fromdatetime(to) if to else None
     if status is None:
-        events = await get_all_events(from_date=frm, to_date=to)
-    elif status == EventPublicationStatus.WAITING:
+        events = await get_all_mobilizon_events(from_date=frm, to_date=to)
+    elif status == _EventPublicationStatus.WAITING:
         events = await list_unpublished_events(frm=frm, to=to)
     else:
-        events = await events_with_status([status], from_date=frm, to_date=to)
+        events = await get_mobilizon_events_with_status(
+            [status], from_date=frm, to_date=to
+        )
     events = list(events)
     if events:
         show_events(events)
     else:
         message = (
             f"No event found with status: {status.name}"
             if status is not None
```

### Comparing `mobilizon-reshare-0.3.2/mobilizon_reshare/cli/commands/list/list_publication.py` & `mobilizon-reshare-0.3.4/mobilizon_reshare/cli/commands/list/list_publication.py`

 * *Files identical despite different names*

### Comparing `mobilizon-reshare-0.3.2/mobilizon_reshare/config/config.py` & `mobilizon-reshare-0.3.4/mobilizon_reshare/config/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 base_validators = [
     # strategy to decide events to publish
     Validator("selection.strategy", must_exist=True, is_type_of=str),
     # url of the main Mobilizon instance to download events from
     Validator("source.mobilizon.url", must_exist=True, is_type_of=str),
     Validator("source.mobilizon.group", must_exist=True, is_type_of=str),
-    Validator("db_path", must_exist=True, is_type_of=str),
+    Validator("db_url", must_exist=True, is_type_of=str),
     Validator("locale", must_exist=True, is_type_of=str, default="en-us"),
 ]
 
 activeness_validators = [
     Validator(f"publisher.{publisher_name}.active", must_exist=True, is_type_of=bool)
     for publisher_name in publisher_names
 ] + [
@@ -126,7 +126,11 @@
     @classmethod
     def clear(cls):
         cls._instance = None
 
 
 def get_settings():
     return CustomConfig.get_instance().settings
+
+
+def get_settings_without_validation():
+    return build_settings()
```

### Comparing `mobilizon-reshare-0.3.2/mobilizon_reshare/config/notifiers.py` & `mobilizon-reshare-0.3.4/mobilizon_reshare/config/notifiers.py`

 * *Files identical despite different names*

### Comparing `mobilizon-reshare-0.3.2/mobilizon_reshare/config/publishers.py` & `mobilizon-reshare-0.3.4/mobilizon_reshare/config/publishers.py`

 * *Files identical despite different names*

### Comparing `mobilizon-reshare-0.3.2/mobilizon_reshare/event/event_selection_strategies.py` & `mobilizon-reshare-0.3.4/mobilizon_reshare/event/event_selection_strategies.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 from abc import ABC, abstractmethod
 from typing import List, Optional
 
 import arrow
 
 from mobilizon_reshare.config.config import get_settings
-from mobilizon_reshare.event.event import MobilizonEvent
+from mobilizon_reshare.dataclasses import MobilizonEvent
 
 logger = logging.getLogger(__name__)
 
 
 class EventSelectionStrategy(ABC):
     def select(
         self,
```

### Comparing `mobilizon-reshare-0.3.2/mobilizon_reshare/formatting/description.py` & `mobilizon-reshare-0.3.4/mobilizon_reshare/formatting/description.py`

 * *Files identical despite different names*

### Comparing `mobilizon-reshare-0.3.2/mobilizon_reshare/main/publish.py` & `mobilizon-reshare-0.3.4/mobilizon_reshare/main/publish.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,68 +1,89 @@
 import logging.config
-from typing import Optional
+from typing import Optional, Iterator
 
-from mobilizon_reshare.event.event import MobilizonEvent
+from mobilizon_reshare.config.command import CommandConfig
+from mobilizon_reshare.dataclasses import MobilizonEvent
+from mobilizon_reshare.dataclasses.event import (
+    get_published_events,
+    get_mobilizon_events_without_publications,
+)
+from mobilizon_reshare.dataclasses.publication import (
+    _EventPublication,
+    build_publications_for_event,
+)
 from mobilizon_reshare.event.event_selection_strategies import select_event_to_publish
 from mobilizon_reshare.publishers import get_active_publishers
-from mobilizon_reshare.publishers.abstract import EventPublication
-from mobilizon_reshare.publishers.coordinator import (
+from mobilizon_reshare.publishers.coordinators.event_publishing.dry_run import (
+    DryRunPublisherCoordinator,
+)
+from mobilizon_reshare.publishers.coordinators.event_publishing.notify import (
     PublicationFailureNotifiersCoordinator,
+)
+from mobilizon_reshare.publishers.coordinators.event_publishing.publish import (
     PublisherCoordinatorReport,
+    PublisherCoordinator,
 )
-from mobilizon_reshare.publishers.coordinator import PublisherCoordinator
-from mobilizon_reshare.storage.query.read import (
-    get_published_events,
-    build_publications,
-    events_without_publications,
+from mobilizon_reshare.storage.query.write import (
+    save_publication_report,
+    save_notification_report,
 )
-from mobilizon_reshare.storage.query.write import save_publication_report
 
 logger = logging.getLogger(__name__)
 
 
 async def publish_publications(
-    publications: list[EventPublication],
+    publications: list[_EventPublication],
 ) -> PublisherCoordinatorReport:
-    report = PublisherCoordinator(publications).run()
+    publishers_report = PublisherCoordinator(publications).run()
+    await save_publication_report(publishers_report)
+
+    for publication_report in publishers_report.reports:
+        if not publication_report.successful:
+            notifiers_report = PublicationFailureNotifiersCoordinator(publication_report,).notify_failure()
+            if notifiers_report:
+                await save_notification_report(notifiers_report)
 
-    await save_publication_report(report)
-    for publication_report in report.reports:
-        if not publication_report.succesful:
-            PublicationFailureNotifiersCoordinator(
-                publication_report,
-            ).notify_failure()
+    return publishers_report
 
-    return report
+
+def perform_dry_run(publications: list[_EventPublication]):
+    return DryRunPublisherCoordinator(publications).run()
 
 
 async def publish_event(
-    event: MobilizonEvent, publishers: Optional[list[Optional[str]]] = None
+    event: MobilizonEvent,
+    command_config: CommandConfig,
+    publishers: Optional[Iterator[str]] = None,
 ) -> PublisherCoordinatorReport:
     logger.info(f"Event to publish found: {event.name}")
 
     if not (publishers and all(publishers)):
         publishers = get_active_publishers()
 
-    publications = await build_publications(event, publishers)
-    return await publish_publications(publications)
+    publications = await build_publications_for_event(event, publishers)
+    if command_config.dry_run:
+        logger.info("Executing in dry run mode. No event is going to be published.")
+        return perform_dry_run(publications)
+    else:
+        return await publish_publications(publications)
 
 
 async def select_and_publish(
+    command_config: CommandConfig,
     unpublished_events: Optional[list[MobilizonEvent]] = None,
 ) -> Optional[PublisherCoordinatorReport]:
     """
     STUB
     :return:
     """
     if unpublished_events is None:
-        unpublished_events = await events_without_publications()
+        unpublished_events = await get_mobilizon_events_without_publications()
 
     event = select_event_to_publish(
-        list(await get_published_events()),
-        unpublished_events,
+        list(await get_published_events()), unpublished_events,
     )
 
     if event:
-        return await publish_event(event)
+        return await publish_event(event, command_config)
     else:
         logger.info("No event to publish found")
```

### Comparing `mobilizon-reshare-0.3.2/mobilizon_reshare/main/pull.py` & `mobilizon-reshare-0.3.4/mobilizon_reshare/main/pull.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 import logging.config
 
-from mobilizon_reshare.event.event import MobilizonEvent
+from mobilizon_reshare.dataclasses import MobilizonEvent
 from mobilizon_reshare.mobilizon.events import get_mobilizon_future_events
-
-from mobilizon_reshare.storage.query.write import (
-    create_unpublished_events,
-)
+from mobilizon_reshare.storage.query.write import create_unpublished_events
 
 logger = logging.getLogger(__name__)
 
 
 async def pull() -> list[MobilizonEvent]:
     """
     Fetches the latest events from Mobilizon and stores them.
```

### Comparing `mobilizon-reshare-0.3.2/mobilizon_reshare/main/recap.py` & `mobilizon-reshare-0.3.4/mobilizon_reshare/publishers/coordinators/event_publishing/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,52 +1,66 @@
+import dataclasses
 import logging
-from typing import Optional, List
+from dataclasses import dataclass
+from typing import List, Optional, Sequence
 
-from arrow import now
-
-from mobilizon_reshare.event.event import EventPublicationStatus, MobilizonEvent
-from mobilizon_reshare.publishers import get_active_publishers
-from mobilizon_reshare.publishers.abstract import RecapPublication
-from mobilizon_reshare.publishers.coordinator import (
-    RecapCoordinator,
-    PublicationFailureNotifiersCoordinator,
-    BaseCoordinatorReport,
-)
-from mobilizon_reshare.publishers.platforms.platform_mapping import (
-    get_publisher_class,
-    get_formatter_class,
-)
-from mobilizon_reshare.storage.query.read import events_with_status
+from mobilizon_reshare.dataclasses.publication import _EventPublication
+from mobilizon_reshare.models.publication import PublicationStatus
+from mobilizon_reshare.publishers.coordinators import BasePublicationReport
 
 logger = logging.getLogger(__name__)
 
 
-async def select_events_to_recap() -> List[MobilizonEvent]:
-    return list(
-        await events_with_status(
-            status=[EventPublicationStatus.COMPLETED], from_date=now()
+@dataclass
+class EventPublicationReport(BasePublicationReport):
+    publication: _EventPublication
+    published_content: Optional[str] = dataclasses.field(default=None)
+
+    def get_failure_message(self):
+        if not self.reason:
+            logger.error("Report of failure without reason.", exc_info=True)
+
+        return (
+            f"Publication {self.publication.id} failed with status: {self.status.name}.\n"
+            f"Reason: {self.reason}\n"
+            f"Publisher: {self.publication.publisher.name}\n"
+            f"Event: {self.publication.event.name}"
         )
-    )
 
 
-async def recap() -> Optional[BaseCoordinatorReport]:
-    # I want to recap only the events that have been successfully published and that haven't happened yet
-    events_to_recap = await select_events_to_recap()
-
-    if events_to_recap:
-        logger.info(f"Found {len(events_to_recap)} events to recap.")
-        recap_publications = [
-            RecapPublication(
-                get_publisher_class(publisher)(),
-                get_formatter_class(publisher)(),
-                events_to_recap,
+class BaseEventPublishingCoordinator:
+    def __init__(self, publications: List[_EventPublication]):
+        self.publications = publications
+
+    def _safe_run(self, reasons, f, *args, **kwargs):
+        try:
+            f(*args, **kwargs)
+            return reasons
+        except Exception as e:
+            return reasons + [str(e)]
+
+    def _validate(self) -> List[EventPublicationReport]:
+        errors = []
+
+        for publication in self.publications:
+            reasons = []
+            reasons = self._safe_run(
+                reasons, publication.publisher.validate_credentials,
+            )
+            reasons = self._safe_run(
+                reasons, publication.formatter.validate_event, publication.event
             )
-            for publisher in get_active_publishers()
-        ]
-        reports = RecapCoordinator(recap_publications).run()
-
-        for report in reports.reports:
-            if report.status == EventPublicationStatus.FAILED:
-                PublicationFailureNotifiersCoordinator(report).notify_failure()
-        return reports
-    else:
-        logger.info("Found no events")
+
+            if len(reasons) > 0:
+                errors.append(
+                    EventPublicationReport(
+                        status=PublicationStatus.FAILED,
+                        reason=", ".join(reasons),
+                        publication=publication,
+                    )
+                )
+
+        return errors
+
+    def _filter_publications(self, errors: Sequence[EventPublicationReport]) -> List[_EventPublication]:
+        publishers_with_errors = set(e.publication.publisher for e in errors)
+        return [p for p in self.publications if p.publisher not in publishers_with_errors]
```

### Comparing `mobilizon-reshare-0.3.2/mobilizon_reshare/main/retry.py` & `mobilizon-reshare-0.3.4/mobilizon_reshare/main/retry.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 import logging
 from typing import Optional
 from uuid import UUID
 
+from tortoise.exceptions import DoesNotExist
+
+from mobilizon_reshare.dataclasses import MobilizonEvent, EventPublication
+from mobilizon_reshare.dataclasses.publication import get_failed_publications_for_event
 from mobilizon_reshare.main.publish import publish_publications
-from mobilizon_reshare.publishers.coordinator import (
+from mobilizon_reshare.publishers.coordinators.event_publishing.publish import (
     PublisherCoordinatorReport,
 )
 from mobilizon_reshare.storage.query.exceptions import EventNotFound
-from mobilizon_reshare.storage.query.read import (
-    get_failed_publications_for_event,
-    get_publication,
-)
 
 logger = logging.getLogger(__name__)
 
 
 async def retry_event_publications(event_id) -> Optional[PublisherCoordinatorReport]:
-
-    failed_publications = await get_failed_publications_for_event(event_id)
+    event = await MobilizonEvent.retrieve(event_id)
+    failed_publications = await get_failed_publications_for_event(event)
     if not failed_publications:
         logger.info("No failed publications found.")
         return
 
     logger.info(f"Found {len(failed_publications)} publications.")
     return await publish_publications(failed_publications)
 
 
 async def retry_publication(publication_id) -> Optional[PublisherCoordinatorReport]:
-    publication = await get_publication(publication_id)
-    if not publication:
+    try:
+        publication = await EventPublication.retrieve(publication_id)
+    except DoesNotExist:
         logger.info(f"Publication {publication_id} not found.")
         return
 
     logger.info(f"Publication {publication_id} found.")
     return await publish_publications([publication])
```

### Comparing `mobilizon-reshare-0.3.2/mobilizon_reshare/migrations/models/0_20211207110159_init.sql` & `mobilizon-reshare-0.3.4/mobilizon_reshare/migrations/sqlite/models/0_20211207110159_init.sql`

 * *Files identical despite different names*

### Comparing `mobilizon-reshare-0.3.2/mobilizon_reshare/mobilizon/events.py` & `mobilizon-reshare-0.3.4/mobilizon_reshare/mobilizon/events.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from typing import List, Optional
 from uuid import UUID
 
 import arrow
 import requests
 
 from mobilizon_reshare.config.config import get_settings
-from mobilizon_reshare.event.event import MobilizonEvent, EventPublicationStatus
+from mobilizon_reshare.dataclasses import MobilizonEvent, _EventPublicationStatus
 
 logger = logging.getLogger(__name__)
 
 
 class MobilizonRequestFailed(Exception):
     # TODO move to an error module
     pass
@@ -39,15 +39,15 @@
         begin_datetime=arrow.get(data["beginsOn"]) if "beginsOn" in data else None,
         end_datetime=arrow.get(data["endsOn"]) if "endsOn" in data else None,
         mobilizon_link=data.get("url", None),
         mobilizon_id=UUID(data["uuid"]),
         thumbnail_link=parse_picture(data),
         location=parse_location(data),
         publication_time=None,
-        status=EventPublicationStatus.WAITING,
+        status=_EventPublicationStatus.WAITING,
         last_update_time=arrow.get(data["updatedAt"]) if "updatedAt" in data else None,
     )
 
 
 query_future_events = """{{
             group(preferredUsername: "{group}") {{
               organizedEvents(page:{page}, afterDatetime:"{afterDatetime}"){{
```

### Comparing `mobilizon-reshare-0.3.2/mobilizon_reshare/models/event.py` & `mobilizon-reshare-0.3.4/mobilizon_reshare/models/event.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,19 @@
+from typing import Iterator
+
 from tortoise import fields
 from tortoise.models import Model
+from tortoise.transactions import atomic
 
+from mobilizon_reshare.models import WithPydantic
 from mobilizon_reshare.models.publication import PublicationStatus, Publication
 from mobilizon_reshare.models.publisher import Publisher
 
 
-class Event(Model):
+class Event(Model, WithPydantic):
     id = fields.UUIDField(pk=True)
     name = fields.TextField()
     description = fields.TextField(null=True)
 
     mobilizon_id = fields.UUIDField()
     mobilizon_link = fields.TextField()
     thumbnail_link = fields.TextField(null=True)
@@ -37,7 +41,21 @@
         publisher = await Publisher.filter(name=publisher_name).first()
         return Publication(
             status=status,
             event_id=self.id,
             publisher_id=publisher.id,
             publisher=publisher,
         )
+
+    async def build_publications(self, publishers: Iterator[str]):
+        return [
+            await self.build_publication_by_publisher_name(name) for name in publishers
+        ]
+
+    @atomic()
+    async def get_failed_publications(self,) -> list[Publication]:
+        return list(
+            filter(
+                lambda publications: publications.status == PublicationStatus.FAILED,
+                self.publications,
+            )
+        )
```

### Comparing `mobilizon-reshare-0.3.2/mobilizon_reshare/models/notification.py` & `mobilizon-reshare-0.3.4/mobilizon_reshare/models/notification.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,29 +1,25 @@
 from enum import IntEnum
 
 from tortoise import fields
 from tortoise.models import Model
 
 
 class NotificationStatus(IntEnum):
-    WAITING = 1
-    FAILED = 2
-    PARTIAL = 3
-    COMPLETED = 4
+    FAILED = 0
+    COMPLETED = 1
 
 
 class Notification(Model):
     id = fields.UUIDField(pk=True)
     status = fields.IntEnumField(NotificationStatus)
 
     message = fields.TextField()
 
-    target = fields.ForeignKeyField(
-        "models.Publisher", related_name="notifications", null=True
-    )
+    target = fields.ForeignKeyField("models.Publisher", null=True, related_name=False,)
 
     publication = fields.ForeignKeyField(
         "models.Publication", related_name="notifications", null=True
     )
 
     def __str__(self):
         return f"[{self.status}] {self.message}"
```

### Comparing `mobilizon-reshare-0.3.2/mobilizon_reshare/models/publication.py` & `mobilizon-reshare-0.3.4/mobilizon_reshare/models/publication.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 from enum import IntEnum
 
 from tortoise import fields
 from tortoise.models import Model
 
+from mobilizon_reshare.models import WithPydantic
+
 
 class PublicationStatus(IntEnum):
     FAILED = 0
     COMPLETED = 1
 
 
-class Publication(Model):
+class Publication(Model, WithPydantic):
     id = fields.UUIDField(pk=True)
     status = fields.IntEnumField(PublicationStatus)
 
     timestamp = fields.DatetimeField()
     reason = fields.TextField(null=True)
 
     event = fields.ForeignKeyField("models.Event", related_name="publications")
```

### Comparing `mobilizon-reshare-0.3.2/mobilizon_reshare/publishers/abstract.py` & `mobilizon-reshare-0.3.4/mobilizon_reshare/publishers/abstract.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 import inspect
 import logging
 from abc import ABC, abstractmethod
-from dataclasses import dataclass
-from typing import List, Optional
-from uuid import UUID
+from typing import Optional
 
 from dynaconf.utils.boxing import DynaBox
 from jinja2 import Environment, FileSystemLoader, Template
 
 from mobilizon_reshare.config.config import get_settings
-from mobilizon_reshare.event.event import MobilizonEvent
 from .exceptions import InvalidAttribute
+from ..dataclasses import _MobilizonEvent
 
 JINJA_ENV = Environment(loader=FileSystemLoader("/"))
 
 logger = logging.getLogger(__name__)
 
 
 class LoggerMixin:
@@ -79,18 +77,18 @@
 
     @property
     @abstractmethod
     def name(self):
         pass
 
     @abstractmethod
-    def _send(self, message: str, event: Optional[MobilizonEvent] = None):
+    def _send(self, message: str, event: Optional[_MobilizonEvent] = None):
         raise NotImplementedError  # pragma: no cover
 
-    def send(self, message: str, event: Optional[MobilizonEvent] = None):
+    def send(self, message: str, event: Optional[_MobilizonEvent] = None):
         """
         Sends a message to the target channel
         """
         response = self._send(message, event)
         self._validate_response(response)
 
     @abstractmethod
@@ -105,15 +103,15 @@
         credentials are not valid.
         """
         raise NotImplementedError  # pragma: no cover
 
 
 class AbstractEventFormatter(LoggerMixin, ConfLoaderMixin):
     @abstractmethod
-    def _validate_event(self, event: MobilizonEvent) -> None:
+    def _validate_event(self, event: _MobilizonEvent) -> None:
         """
         Validates publisher's event.
         Should raise ``PublisherError`` (or one of its subclasses) if event
         is not valid.
         """
         raise NotImplementedError  # pragma: no cover
 
@@ -122,26 +120,26 @@
         """
         Validates notifier's message.
         Should raise ``PublisherError`` (or one of its subclasses) if message
         is not valid.
         """
         raise NotImplementedError  # pragma: no cover
 
-    def validate_event(self, event: MobilizonEvent) -> None:
+    def validate_event(self, event: _MobilizonEvent) -> None:
         self._validate_event(event)
         self._validate_message(self.get_message_from_event(event))
 
     @abstractmethod
     def _preprocess_event(self, event):
         """
         Allows publishers to preprocess events before feeding them to the template
         """
         return event
 
-    def get_message_from_event(self, event: MobilizonEvent) -> str:
+    def get_message_from_event(self, event: _MobilizonEvent) -> str:
         """
         Retrieves a message from the event itself.
         """
         event = self._preprocess_event(event)
         message = event.format(self.get_message_template())
         message = self._preprocess_message(message)
         return message
@@ -162,33 +160,16 @@
 
     def get_recap_fragment_template(self) -> Template:
         template_path = (
             self.conf.recap_template_path or self.default_recap_template_path
         )
         return JINJA_ENV.get_template(template_path)
 
-    def get_recap_fragment(self, event: MobilizonEvent) -> str:
+    def get_recap_fragment(self, event: _MobilizonEvent) -> str:
         """
         Retrieves the fragment that describes a single event inside the event recap.
         """
         event = self._preprocess_event(event)
         return event.format(self.get_recap_fragment_template())
 
     def _preprocess_message(self, message: str):
         return message
-
-
-@dataclass
-class BasePublication:
-    publisher: AbstractPlatform
-    formatter: AbstractEventFormatter
-
-
-@dataclass
-class EventPublication(BasePublication):
-    event: MobilizonEvent
-    id: UUID
-
-
-@dataclass
-class RecapPublication(BasePublication):
-    events: List[MobilizonEvent]
```

### Comparing `mobilizon-reshare-0.3.2/mobilizon_reshare/publishers/exceptions.py` & `mobilizon-reshare-0.3.4/mobilizon_reshare/publishers/exceptions.py`

 * *Files identical despite different names*

### Comparing `mobilizon-reshare-0.3.2/mobilizon_reshare/publishers/platforms/facebook.py` & `mobilizon-reshare-0.3.4/mobilizon_reshare/publishers/platforms/facebook.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Optional
 
 import facebook
 import pkg_resources
 from facebook import GraphAPIError
 
-from mobilizon_reshare.event.event import MobilizonEvent
+from mobilizon_reshare.dataclasses import MobilizonEvent
 from mobilizon_reshare.formatting.description import html_to_plaintext
 from mobilizon_reshare.publishers.abstract import (
     AbstractPlatform,
     AbstractEventFormatter,
 )
 from mobilizon_reshare.publishers.exceptions import (
     InvalidCredentials,
```

### Comparing `mobilizon-reshare-0.3.2/mobilizon_reshare/publishers/platforms/mastodon.py` & `mobilizon-reshare-0.3.4/mobilizon_reshare/publishers/platforms/mastodon.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Optional
 from urllib.parse import urljoin
 
 import pkg_resources
 import requests
 from requests import Response
 
-from mobilizon_reshare.event.event import MobilizonEvent
+from mobilizon_reshare.dataclasses import MobilizonEvent
 from mobilizon_reshare.publishers.abstract import (
     AbstractPlatform,
     AbstractEventFormatter,
 )
 from mobilizon_reshare.publishers.exceptions import (
     InvalidBot,
     InvalidEvent,
```

### Comparing `mobilizon-reshare-0.3.2/mobilizon_reshare/publishers/platforms/platform_mapping.py` & `mobilizon-reshare-0.3.4/mobilizon_reshare/publishers/platforms/platform_mapping.py`

 * *Files identical despite different names*

### Comparing `mobilizon-reshare-0.3.2/mobilizon_reshare/publishers/platforms/telegram.py` & `mobilizon-reshare-0.3.4/mobilizon_reshare/publishers/platforms/telegram.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import Optional
 
 import pkg_resources
 import requests
 from bs4 import BeautifulSoup
 from requests import Response
 
-from mobilizon_reshare.event.event import MobilizonEvent
+from mobilizon_reshare.dataclasses import MobilizonEvent
 from mobilizon_reshare.publishers.abstract import (
     AbstractEventFormatter,
     AbstractPlatform,
 )
 from mobilizon_reshare.publishers.exceptions import (
     InvalidBot,
     InvalidEvent,
@@ -31,19 +31,21 @@
     default_recap_header_template_path = pkg_resources.resource_filename(
         "mobilizon_reshare.publishers.templates", "telegram_recap_header.tmpl.j2"
     )
 
     _conf = ("publisher", "telegram")
 
     def _validate_event(self, event: MobilizonEvent) -> None:
+
         description = event.description
         if not (description and description.strip()):
             self._log_error("No description was found", raise_error=InvalidEvent)
 
     def _validate_message(self, message: str) -> None:
+
         if (
             len("".join(BeautifulSoup(message, "html.parser").findAll(text=True)))
             >= 4096
         ):
             self._log_error("Message is too long", raise_error=InvalidMessage)
 
     def _preprocess_message(self, message: str) -> str:
@@ -70,15 +72,16 @@
             tag.unwrap()
         # replacing list elements with dots
         for tag in html.findAll(["li"]):
             tag.insert(0, "• ")
             tag.unwrap()
         # cleaning html trailing whitespace
         for tag in html.findAll("a"):
-            tag["href"] = tag["href"].replace(" ", "").strip().lstrip()
+            if "href" in tag:
+                tag["href"] = tag["href"].replace(" ", "").strip().lstrip()
         s = str(html)
         return re.sub(r"\n{2,}", "\n\n", s).strip()  # remove multiple newlines
 
 
 class TelegramPlatform(AbstractPlatform):
     """
     Telegram publisher class.
@@ -99,24 +102,24 @@
         return requests.post(
             url=f"https://api.telegram.org/bot{self.conf.token}/sendMessage",
             json={"chat_id": self.conf.chat_id, "text": message, "parse_mode": "html"},
         )
 
     def _validate_response(self, res):
         try:
-
             res.raise_for_status()
         except requests.exceptions.HTTPError as e:
             self._log_error(
                 f"Server returned invalid data: {str(e)}\n{res.text}",
                 raise_error=InvalidResponse,
             )
 
         try:
             data = res.json()
+
         except Exception as e:
             self._log_error(
                 f"Server returned invalid json data: {str(e)}",
                 raise_error=InvalidResponse,
             )
 
         if not data.get("ok"):
```

### Comparing `mobilizon-reshare-0.3.2/mobilizon_reshare/publishers/platforms/twitter.py` & `mobilizon-reshare-0.3.4/mobilizon_reshare/publishers/platforms/twitter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Optional
 
 import pkg_resources
 from tweepy import OAuthHandler, API, TweepyException
 from tweepy.models import Status
 
-from mobilizon_reshare.event.event import MobilizonEvent
+from mobilizon_reshare.dataclasses import MobilizonEvent
 from mobilizon_reshare.publishers.abstract import (
     AbstractPlatform,
     AbstractEventFormatter,
 )
 from mobilizon_reshare.publishers.exceptions import (
     InvalidCredentials,
     PublisherError,
```

### Comparing `mobilizon-reshare-0.3.2/mobilizon_reshare/publishers/platforms/zulip.py` & `mobilizon-reshare-0.3.4/mobilizon_reshare/publishers/platforms/zulip.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from urllib.parse import urljoin
 
 import pkg_resources
 import requests
 from requests import Response
 from requests.auth import HTTPBasicAuth
 
-from mobilizon_reshare.event.event import MobilizonEvent
+from mobilizon_reshare.dataclasses import MobilizonEvent
 from mobilizon_reshare.formatting.description import html_to_markdown
 from mobilizon_reshare.publishers.abstract import (
     AbstractPlatform,
     AbstractEventFormatter,
 )
 from mobilizon_reshare.publishers.exceptions import (
     InvalidBot,
@@ -98,15 +98,15 @@
                 raise_error=InvalidBot,
             )
 
     def _validate_response(self, response: Response) -> dict:
         try:
             response.raise_for_status()
         except requests.exceptions.HTTPError as e:
-            self._log_debug(str(response))
+            self._log_debug(str(response.text))
             self._log_error(
                 str(e), raise_error=HTTPResponseError,
             )
 
         # See https://zulip.com/api/rest-error-handling
         try:
             data = response.json()
```

### Comparing `mobilizon-reshare-0.3.2/mobilizon_reshare/settings.toml` & `mobilizon-reshare-0.3.4/mobilizon_reshare/settings.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 [default]
 local_state_dir = "/var/mobilizon_reshare"
-db_name = "events.db"
-db_path = "@format {this.local_state_dir}/{this.db_name}"
+db_url = "sqlite:///var/mobilizon_reshare/events.db"
 locale= "en-us"
 
 [default.source.mobilizon]
 url="https://some_mobilizon"
 group="my_group"
 
 [default.selection]
```

### Comparing `mobilizon-reshare-0.3.2/mobilizon_reshare/storage/db.py` & `mobilizon-reshare-0.3.4/mobilizon_reshare/storage/db.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,36 +1,34 @@
 import logging
+from logging.config import dictConfig
 from pathlib import Path
 
 import pkg_resources
-from tortoise import Tortoise
+import urllib3.util
 from aerich import Command
+from tortoise import Tortoise
+
+from mobilizon_reshare.config.config import (
+    get_settings,
+    get_settings_without_validation,
+)
 from mobilizon_reshare.config.publishers import publisher_names
 from mobilizon_reshare.storage.query.write import update_publishers
 
-from mobilizon_reshare.config.config import get_settings
-
 logger = logging.getLogger(__name__)
 
 
-def get_db_url():
-    """gets db url from settings
-
-    Returns:
-        str : db url
-    """
-    settings = get_settings()
-    db_path = Path(settings.db_path)
-    db_url = f"sqlite:///{db_path}"
-    return db_url
+def get_db_url() -> urllib3.util.Url:
+    return urllib3.util.parse_url(get_settings_without_validation().db_url)
 
 
 def get_tortoise_orm():
+
     return {
-        "connections": {"default": get_db_url()},
+        "connections": {"default": get_db_url().url},
         "apps": {
             "models": {
                 "models": [
                     "mobilizon_reshare.models.event",
                     "mobilizon_reshare.models.notification",
                     "mobilizon_reshare.models.publication",
                     "mobilizon_reshare.models.publisher",
@@ -44,43 +42,65 @@
     }
 
 
 TORTOISE_ORM = get_tortoise_orm()
 
 
 class MoReDB:
-    def __init__(self, path: Path):
-        self.path = path
-        # TODO: Check if DB is openable/"queriable"
-        self.is_init = self.path.exists() and (not self.path.is_dir())
-        if not self.is_init:
-            self.path.parent.mkdir(parents=True, exist_ok=True)
+    def get_migration_location(self):
+        scheme = get_db_url().scheme
+        return pkg_resources.resource_filename(
+            "mobilizon_reshare", f"migrations/{scheme}"
+        )
 
     async def _implement_db_changes(self):
-        migration_queries_location = pkg_resources.resource_filename(
-            "mobilizon_reshare", "migrations"
-        )
+        logging.info("Performing aerich migrations.")
         command = Command(
-            tortoise_config=TORTOISE_ORM,
+            tortoise_config=get_tortoise_orm(),
             app="models",
-            location=migration_queries_location,
+            location=self.get_migration_location(),
         )
         await command.init()
         migrations = await command.upgrade()
         if migrations:
-            logging.warning("Updated database to latest version")
+            logging.info("Updated database to latest version")
 
     async def setup(self):
-        await self._implement_db_changes()
-        await Tortoise.init(
-            config=TORTOISE_ORM,
+        tortoise_config = get_tortoise_orm()
+        Tortoise.init_models(
+            tortoise_config["apps"]["models"]["models"], "models", _init_relations=True
         )
-        if not self.is_init:
-            await Tortoise.generate_schemas()
-            self.is_init = True
-            logger.info(f"Successfully initialized database at {self.path}")
-
+        await self._implement_db_changes()
+        await Tortoise.init(config=tortoise_config)
+        await Tortoise.generate_schemas()
         await update_publishers(publisher_names)
 
 
+class MoReSQLiteDB(MoReDB):
+    def __init__(self):
+
+        if (
+            get_db_url().path
+        ):  # if in-memory sqlite there's no path so nothing has to be initialized
+            self.path = Path(get_db_url().path)
+            # TODO: Check if DB is openable/"queriable"
+            self.is_init = self.path.exists() and (not self.path.is_dir())
+            if not self.is_init:
+                self.path.parent.mkdir(parents=True, exist_ok=True)
+
+
 async def tear_down():
     return await Tortoise.close_connections()
+
+
+async def init(init_logging=True):
+
+    if init_logging:
+        dictConfig(get_settings()["logging"])
+
+    # init storage
+    url = get_db_url()
+    if url.scheme == "sqlite":
+        db = MoReSQLiteDB()
+    else:
+        db = MoReDB()
+    await db.setup()
```

### Comparing `mobilizon-reshare-0.3.2/mobilizon_reshare/storage/query/write.py` & `mobilizon-reshare-0.3.4/mobilizon_reshare/storage/query/write.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,37 +1,40 @@
 import logging
-from typing import Iterable, Optional
+from typing import Iterable
 
 import arrow
 from tortoise.transactions import atomic
 
-from mobilizon_reshare.event.event import MobilizonEvent
+from mobilizon_reshare.dataclasses import MobilizonEvent
+from mobilizon_reshare.dataclasses.event import (
+    get_mobilizon_events_without_publications,
+)
 from mobilizon_reshare.models.event import Event
+from mobilizon_reshare.models.notification import Notification
 from mobilizon_reshare.models.publication import Publication
 from mobilizon_reshare.models.publisher import Publisher
-from mobilizon_reshare.publishers.coordinator import PublisherCoordinatorReport
-from mobilizon_reshare.storage.query import CONNECTION_NAME
-from mobilizon_reshare.storage.query.converter import event_to_model
-from mobilizon_reshare.storage.query.read import (
-    events_without_publications,
-    is_known,
-    get_publisher_by_name,
-    get_event,
+from mobilizon_reshare.publishers.coordinators.event_publishing import (
+    EventPublicationReport,
 )
+from mobilizon_reshare.publishers.coordinators.event_publishing.notify import (
+    NotifierCoordinatorReport,
+)
+from mobilizon_reshare.publishers.coordinators.event_publishing.publish import (
+    PublisherCoordinatorReport,
+)
+from mobilizon_reshare.storage.query.read import get_event
 
 
-async def create_publisher(name: str, account_ref: Optional[str] = None) -> None:
-    await Publisher.create(name=name, account_ref=account_ref)
-
-
-@atomic(CONNECTION_NAME)
-async def upsert_publication(publication_report, event):
+@atomic()
+async def upsert_publication(
+    publication_report: EventPublicationReport, event: Event
+):
 
-    publisher = await get_publisher_by_name(
-        name=publication_report.publication.publisher.name
+    publisher_model = await (
+        Publisher.get(name=publication_report.publication.publisher.name).first()
     )
     old_publication = await Publication.filter(
         id=publication_report.publication.id
     ).first()
     if old_publication:
         # I update the existing publication with the new report
         old_publication.timestamp = arrow.now().datetime
@@ -40,61 +43,77 @@
 
         await old_publication.save(force_update=True)
     else:
         # I create a new publication
         await Publication.create(
             id=publication_report.publication.id,
             event_id=event.id,
-            publisher_id=publisher.id,
+            publisher_id=publisher_model.id,
             status=publication_report.status,
             reason=publication_report.reason,
             timestamp=arrow.now().datetime,
         )
 
 
-@atomic(CONNECTION_NAME)
+@atomic()
 async def save_publication_report(
     coordinator_report: PublisherCoordinatorReport,
 ) -> None:
     """
     Store a publication process outcome
     """
     for publication_report in coordinator_report.reports:
         event = await Event.filter(
             mobilizon_id=publication_report.publication.event.mobilizon_id
         ).first()
         await upsert_publication(publication_report, event)
 
 
-@atomic(CONNECTION_NAME)
+@atomic()
+async def save_notification_report(
+    coordinator_report: NotifierCoordinatorReport,
+) -> None:
+    """
+    Store a notification process outcome
+    """
+    for report in coordinator_report.reports:
+        publisher = await Publisher.filter(name=report.notification.publisher.name).first()
+
+        await Notification.create(
+            publication_id=report.notification.publication.id,
+            target_id=publisher.id,
+            status=report.status,
+            message=report.reason,
+        )
+
+
+@atomic()
 async def create_unpublished_events(
     events_from_mobilizon: Iterable[MobilizonEvent],
 ) -> list[MobilizonEvent]:
     """
     Computes the difference between remote and local events and store it.
 
     Returns the unpublished events merged state.
     """
     # There are three cases:
     for event in events_from_mobilizon:
-        if not await is_known(event):
+        if not await Event.exists(mobilizon_id=event.mobilizon_id):
             # Either an event is unknown
-            await event_to_model(event).save()
+            await event.to_model().save()
         else:
             # Or it's known and changed
             event_model = await get_event(event.mobilizon_id)
             if event.last_update_time > event_model.last_update_time:
-                await event_to_model(event=event, db_id=event_model.id).save(
-                    force_update=True
-                )
+                await event.to_model(db_id=event_model.id).save(force_update=True)
             # Or it's known and unchanged, in which case we do nothing.
 
-    return await events_without_publications()
+    return await get_mobilizon_events_without_publications()
 
 
-@atomic(CONNECTION_NAME)
+@atomic()
 async def update_publishers(names: Iterable[str],) -> None:
     names = set(names)
     known_publisher_names = set(p.name for p in await Publisher.all())
     for name in names.difference(known_publisher_names):
         logging.info(f"Creating {name} publisher")
-        await create_publisher(name)
+        await Publisher.create(name=name, account_ref=None)
```

### Comparing `mobilizon-reshare-0.3.2/pyproject.toml` & `mobilizon-reshare-0.3.4/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,44 +1,50 @@
 [tool.poetry]
 name = "mobilizon-reshare"
-version = "0.3.2"
+version = "0.3.4"
 description = "A suite to reshare Mobilizon events on a broad selection of platforms"
 readme = "README.md"
 homepage = "https://github.com/Tech-Workers-Coalition-Italia/mobilizon-reshare"
 repository = "https://github.com/Tech-Workers-Coalition-Italia/mobilizon-reshare"
 authors = ["Simone Robutti <simone.robutti@protonmail.com>"]
 license = "Coopyleft"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 dynaconf = "~3.1"
-tortoise-orm = "~0.18"
+tortoise-orm = {extras = ["asyncpg"], version = "~0.19"}
 aiosqlite = "~0.17"
 Jinja2 = "~3.1"
-requests = "~2.26"
+requests = "~2.28"
 arrow = "~1.1"
-click = "~8.0"
-beautifulsoup4 = "~4.10"
+click = "~8.1"
+beautifulsoup4 = "~4.11"
 markdownify = "~0.10"
 appdirs = "~1.4"
-tweepy = "~4.4"
+tweepy = "~4.13"
 facebook-sdk = "~3.1"
 aerich = "~0.6"
+fastapi = "~0.85"
+uvicorn = "~0.17"
+fastapi-pagination = "^0.11.0"
 
 [tool.poetry.dev-dependencies]
 responses = "~0.13"
 pytest-asyncio = "~0.15"
 asynctest = "~0.13"
 pytest = "~6.2"
-pytest-cov = "~2.8"
+pytest-cov = "~3.0"
 pytest-lazy-fixture = "~0.6"
 Sphinx = "~4.4"
 sphinxcontrib-napoleon = "~0.7"
 sphinx-material = "~0.0"
 sphinx-autodoc-typehints = "~1.17"
+httpx = "~0.23"
+
+
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 mobilizon-reshare="mobilizon_reshare.cli.cli:mobilizon_reshare"
```

### Comparing `mobilizon-reshare-0.3.2/setup.py` & `mobilizon-reshare-0.3.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,52 +9,67 @@
  'mobilizon_reshare.cli.commands.list',
  'mobilizon_reshare.cli.commands.publish',
  'mobilizon_reshare.cli.commands.pull',
  'mobilizon_reshare.cli.commands.recap',
  'mobilizon_reshare.cli.commands.retry',
  'mobilizon_reshare.cli.commands.start',
  'mobilizon_reshare.config',
+ 'mobilizon_reshare.dataclasses',
  'mobilizon_reshare.event',
  'mobilizon_reshare.formatting',
  'mobilizon_reshare.main',
  'mobilizon_reshare.mobilizon',
  'mobilizon_reshare.models',
  'mobilizon_reshare.publishers',
+ 'mobilizon_reshare.publishers.coordinators',
+ 'mobilizon_reshare.publishers.coordinators.event_publishing',
+ 'mobilizon_reshare.publishers.coordinators.recap_publishing',
  'mobilizon_reshare.publishers.platforms',
  'mobilizon_reshare.publishers.templates',
  'mobilizon_reshare.storage',
- 'mobilizon_reshare.storage.query']
+ 'mobilizon_reshare.storage.query',
+ 'mobilizon_reshare.web',
+ 'mobilizon_reshare.web.backend',
+ 'mobilizon_reshare.web.backend.events',
+ 'mobilizon_reshare.web.backend.publications']
 
 package_data = \
-{'': ['*'], 'mobilizon_reshare': ['migrations/models/*']}
+{'': ['*'],
+ 'mobilizon_reshare': ['migrations/postgres/*',
+                       'migrations/postgres/models/*',
+                       'migrations/sqlite/*',
+                       'migrations/sqlite/models/*']}
 
 install_requires = \
 ['Jinja2>=3.1,<3.2',
  'aerich>=0.6,<0.7',
  'aiosqlite>=0.17,<0.18',
  'appdirs>=1.4,<1.5',
  'arrow>=1.1,<1.2',
- 'beautifulsoup4>=4.10,<4.11',
- 'click>=8.0,<8.1',
+ 'beautifulsoup4>=4.11,<4.12',
+ 'click>=8.1,<8.2',
  'dynaconf>=3.1,<3.2',
  'facebook-sdk>=3.1,<3.2',
+ 'fastapi-pagination>=0.11.0,<0.12.0',
+ 'fastapi>=0.85,<0.86',
  'markdownify>=0.10,<0.11',
- 'requests>=2.26,<2.27',
- 'tortoise-orm>=0.18,<0.19',
- 'tweepy>=4.4,<4.5']
+ 'requests>=2.28,<2.29',
+ 'tortoise-orm[asyncpg]>=0.19,<0.20',
+ 'tweepy>=4.13,<4.14',
+ 'uvicorn>=0.17,<0.18']
 
 entry_points = \
 {'console_scripts': ['mobilizon-reshare = '
                      'mobilizon_reshare.cli.cli:mobilizon_reshare']}
 
 setup_kwargs = {
     'name': 'mobilizon-reshare',
-    'version': '0.3.2',
+    'version': '0.3.4',
     'description': 'A suite to reshare Mobilizon events on a broad selection of platforms',
-    'long_description': "[![CI](https://github.com/Tech-Workers-Coalition-Italia/mobilizon-reshare/actions/workflows/main.yml/badge.svg?branch=master)](https://github.com/Tech-Workers-Coalition-Italia/mobilizon-reshare/actions/workflows/main.yml)\n\nThe goal of `mobilizon_reshare` is to provide a suite to reshare Mobilizon events on a broad selection of platforms. This\ntool enables an organization to automate their social media strategy in regards\nto events and their promotion. \n\n# Platforms\n\n`mobilizon-reshare` currently supports the following social platforms:\n\n- Facebook\n- Mastodon\n- Twitter\n- Telegram\n- Zulip\n\n# Usage\n\n## Scheduling and temporal logic\n\nThe tool is designed to work in combination with a scheduler that executes it at\nregular intervals. `mobilizon_reshare` allows fine-grained control over the logic to decide when\nto publish an event, with the minimization of human effort as its first priority.\n\n## Installation\n\n`mobilizon_reshare` is distributed through [Pypi](https://pypi.org/project/mobilizon-reshare/) and [DockerHub](https://hub.docker.com/r/fishinthecalculator/mobilizon-reshare). Use\n\n```shell\n$ pip install mobilizon-reshare\n```\n\nto install the tool in your system or virtualenv.\n\nThis should install the command `mobilizon-reshare` in your system. Use it to access the CLI and discover the available\ncommands and their description.\n\n### Guix package\n\nIf you run Guix you can install `mobilizon-reshare` by adding our [Guix channel](https://github.com/fishinthecalculator/mobilizon-reshare-guix#configure) to your `.config/guix/channels.scm`.\n\n\n\n\nTo run `mobilizon-reshare` from master you can run the following command from the root of the repository:\n\n``` shell\n$ guix time-machine -C channels-lock.scm -- install -L . mobilizon-reshare.git\n```\n\n## Run on your local system\n\nOnce you have installed `mobilizon_reshare` you can schedule the refresh from Mobilizon with your system's `cron`:\n\n```bash\n$ sudo crontab -l\n*/15 * * * * mobilizon-reshare start\n```\n\n## Deploying through Docker Compose\n\nTo run `mobilizon_reshare` in a production environment you can use the image published to DockerHub. We also provide an example [`docker-compose.yml`](https://github.com/Tech-Workers-Coalition-Italia/mobilizon-reshare/blob/master/docker-compose.yml).\n\n# Contributing\n\nWe welcome contributions from anybody. Currently our process is not structured but feel free to open or take issues through Github in case you want to help us. We have setup some instructions to setup a development environment [here](https://github.com/Tech-Workers-Coalition-Italia/mobilizon-reshare/blob/master/doc/contributing.md).\n",
+    'long_description': "[![CI](https://github.com/Tech-Workers-Coalition-Italia/mobilizon-reshare/actions/workflows/main.yml/badge.svg?branch=master)](https://github.com/Tech-Workers-Coalition-Italia/mobilizon-reshare/actions/workflows/main.yml)\n\nThe goal of `mobilizon_reshare` is to provide a suite to reshare Mobilizon events on a broad selection of platforms. This\ntool enables an organization to automate their social media strategy in regards\nto events and their promotion. \n\n# Platforms\n\n`mobilizon-reshare` currently supports the following social platforms:\n\n- Facebook\n- Mastodon\n- Twitter\n- Telegram\n- Zulip\n\n# Usage\n\n## Scheduling and temporal logic\n\nThe tool is designed to work in combination with a scheduler that executes it at\nregular intervals. `mobilizon_reshare` allows fine-grained control over the logic to decide when\nto publish an event, with the minimization of human effort as its first priority.\n\n## Installation\n\n`mobilizon_reshare` is distributed through [Pypi](https://pypi.org/project/mobilizon-reshare/) and [DockerHub](https://hub.docker.com/r/twcita/mobilizon-reshare). Use\n\n```shell\n$ pip install mobilizon-reshare\n```\n\nto install the tool in your system or virtualenv.\n\nThis should install the command `mobilizon-reshare` in your system. Use it to access the CLI and discover the available\ncommands and their description.\n\n### Guix package\n\nIf you run Guix you can install `mobilizon-reshare` by adding our [Guix channel](https://github.com/fishinthecalculator/mobilizon-reshare-guix#configure) to your `.config/guix/channels.scm`.\n\n\n\n\nTo run `mobilizon-reshare` from master you can run the following command from the root of the repository:\n\n``` shell\n$ guix time-machine -C channels-lock.scm -- install -L . mobilizon-reshare.git\n```\n\n## Run on your local system\n\nOnce you have installed `mobilizon_reshare` you can schedule the refresh from Mobilizon with your system's `cron`:\n\n```bash\n$ sudo crontab -l\n*/15 * * * * mobilizon-reshare start\n```\n\n## Deploying through Docker Compose\n\nTo run `mobilizon_reshare` in a production environment you can use the image published to DockerHub. We also provide an example [`docker-compose.yml`](https://github.com/Tech-Workers-Coalition-Italia/mobilizon-reshare/blob/master/docker-compose.yml).\n\n# Contributing\n\nWe welcome contributions from anybody. Currently our process is not structured but feel free to open or take issues through Github in case you want to help us. We have setup some instructions to setup a development environment [here](https://github.com/Tech-Workers-Coalition-Italia/mobilizon-reshare/blob/master/doc/contributing.md).\n",
     'author': 'Simone Robutti',
     'author_email': 'simone.robutti@protonmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/Tech-Workers-Coalition-Italia/mobilizon-reshare',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `mobilizon-reshare-0.3.2/PKG-INFO` & `mobilizon-reshare-0.3.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mobilizon-reshare
-Version: 0.3.2
+Version: 0.3.4
 Summary: A suite to reshare Mobilizon events on a broad selection of platforms
 Home-page: https://github.com/Tech-Workers-Coalition-Italia/mobilizon-reshare
 License: Coopyleft
 Author: Simone Robutti
 Author-email: simone.robutti@protonmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
@@ -12,22 +12,25 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: Jinja2 (>=3.1,<3.2)
 Requires-Dist: aerich (>=0.6,<0.7)
 Requires-Dist: aiosqlite (>=0.17,<0.18)
 Requires-Dist: appdirs (>=1.4,<1.5)
 Requires-Dist: arrow (>=1.1,<1.2)
-Requires-Dist: beautifulsoup4 (>=4.10,<4.11)
-Requires-Dist: click (>=8.0,<8.1)
+Requires-Dist: beautifulsoup4 (>=4.11,<4.12)
+Requires-Dist: click (>=8.1,<8.2)
 Requires-Dist: dynaconf (>=3.1,<3.2)
 Requires-Dist: facebook-sdk (>=3.1,<3.2)
+Requires-Dist: fastapi (>=0.85,<0.86)
+Requires-Dist: fastapi-pagination (>=0.11.0,<0.12.0)
 Requires-Dist: markdownify (>=0.10,<0.11)
-Requires-Dist: requests (>=2.26,<2.27)
-Requires-Dist: tortoise-orm (>=0.18,<0.19)
-Requires-Dist: tweepy (>=4.4,<4.5)
+Requires-Dist: requests (>=2.28,<2.29)
+Requires-Dist: tortoise-orm[asyncpg] (>=0.19,<0.20)
+Requires-Dist: tweepy (>=4.13,<4.14)
+Requires-Dist: uvicorn (>=0.17,<0.18)
 Project-URL: Repository, https://github.com/Tech-Workers-Coalition-Italia/mobilizon-reshare
 Description-Content-Type: text/markdown
 
 [![CI](https://github.com/Tech-Workers-Coalition-Italia/mobilizon-reshare/actions/workflows/main.yml/badge.svg?branch=master)](https://github.com/Tech-Workers-Coalition-Italia/mobilizon-reshare/actions/workflows/main.yml)
 
 The goal of `mobilizon_reshare` is to provide a suite to reshare Mobilizon events on a broad selection of platforms. This
 tool enables an organization to automate their social media strategy in regards
@@ -49,15 +52,15 @@
 
 The tool is designed to work in combination with a scheduler that executes it at
 regular intervals. `mobilizon_reshare` allows fine-grained control over the logic to decide when
 to publish an event, with the minimization of human effort as its first priority.
 
 ## Installation
 
-`mobilizon_reshare` is distributed through [Pypi](https://pypi.org/project/mobilizon-reshare/) and [DockerHub](https://hub.docker.com/r/fishinthecalculator/mobilizon-reshare). Use
+`mobilizon_reshare` is distributed through [Pypi](https://pypi.org/project/mobilizon-reshare/) and [DockerHub](https://hub.docker.com/r/twcita/mobilizon-reshare). Use
 
 ```shell
 $ pip install mobilizon-reshare
 ```
 
 to install the tool in your system or virtualenv.
```

