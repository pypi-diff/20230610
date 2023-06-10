# Comparing `tmp/deta-discord-interactions-0.1.0.tar.gz` & `tmp/deta-discord-interactions-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deta-discord-interactions-0.1.0.tar", last modified: Thu Jun  1 01:14:19 2023, max compression
+gzip compressed data, was "deta-discord-interactions-0.1.1.tar", last modified: Sat Jun 10 21:26:45 2023, max compression
```

## Comparing `deta-discord-interactions-0.1.0.tar` & `deta-discord-interactions-0.1.1.tar`

### file list

```diff
@@ -1,72 +1,75 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 01:14:19.851996 deta-discord-interactions-0.1.0/
--rw-rw-rw-   0        0        0     1096 2022-08-22 23:01:27.000000 deta-discord-interactions-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     1489 2023-06-01 01:14:19.849991 deta-discord-interactions-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      746 2023-06-01 01:13:01.000000 deta-discord-interactions-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-01 01:14:19.401510 deta-discord-interactions-0.1.0/deta_discord_interactions/
--rw-rw-rw-   0        0        0     1722 2022-08-28 00:25:18.000000 deta-discord-interactions-0.1.0/deta_discord_interactions/__init__.py
--rw-rw-rw-   0        0        0     5605 2023-06-01 01:13:01.000000 deta-discord-interactions-0.1.0/deta_discord_interactions/client.py
--rw-rw-rw-   0        0        0    19166 2023-06-01 01:13:01.000000 deta-discord-interactions-0.1.0/deta_discord_interactions/command.py
--rw-rw-rw-   0        0        0    17819 2023-06-01 01:13:01.000000 deta-discord-interactions-0.1.0/deta_discord_interactions/context.py
--rw-rw-rw-   0        0        0    26503 2023-06-01 01:13:01.000000 deta-discord-interactions-0.1.0/deta_discord_interactions/discord.py
-drwxrwxrwx   0        0        0        0 2023-06-01 01:14:19.456840 deta-discord-interactions-0.1.0/deta_discord_interactions/enums/
--rw-rw-rw-   0        0        0      199 2022-09-04 14:09:17.000000 deta-discord-interactions-0.1.0/deta_discord_interactions/enums/__init__.py
--rw-rw-rw-   0        0        0     1315 2022-09-04 14:09:10.000000 deta-discord-interactions-0.1.0/deta_discord_interactions/enums/permissions.py
--rw-rw-rw-   0        0        0      295 2022-08-28 00:25:18.000000 deta-discord-interactions-0.1.0/deta_discord_interactions/enums/response_types.py
--rw-rw-rw-   0        0        0     4339 2023-06-01 01:13:01.000000 deta-discord-interactions-0.1.0/deta_discord_interactions/http.py
-drwxrwxrwx   0        0        0        0 2023-06-01 01:14:19.523985 deta-discord-interactions-0.1.0/deta_discord_interactions/models/
--rw-rw-rw-   0        0        0     1721 2022-08-28 00:25:18.000000 deta-discord-interactions-0.1.0/deta_discord_interactions/models/__init__.py
--rw-rw-rw-   0        0        0     1246 2022-08-28 00:25:18.000000 deta-discord-interactions-0.1.0/deta_discord_interactions/models/attachment.py
--rw-rw-rw-   0        0        0     2655 2023-06-01 01:13:01.000000 deta-discord-interactions-0.1.0/deta_discord_interactions/models/autocomplete.py
--rw-rw-rw-   0        0        0     1387 2023-06-01 01:13:01.000000 deta-discord-interactions-0.1.0/deta_discord_interactions/models/channel.py
--rw-rw-rw-   0        0        0      150 2022-08-28 00:25:18.000000 deta-discord-interactions-0.1.0/deta_discord_interactions/models/command.py
--rw-rw-rw-   0        0        0     8596 2023-06-01 01:13:01.000000 deta-discord-interactions-0.1.0/deta_discord_interactions/models/component.py
--rw-rw-rw-   0        0        0     2806 2023-06-01 01:13:01.000000 deta-discord-interactions-0.1.0/deta_discord_interactions/models/embed.py
--rw-rw-rw-   0        0        0      822 2022-08-28 00:25:18.000000 deta-discord-interactions-0.1.0/deta_discord_interactions/models/interaction.py
--rw-rw-rw-   0        0        0     8113 2023-06-01 01:13:01.000000 deta-discord-interactions-0.1.0/deta_discord_interactions/models/message.py
--rw-rw-rw-   0        0        0     2932 2023-06-01 01:13:01.000000 deta-discord-interactions-0.1.0/deta_discord_interactions/models/modal.py
--rw-rw-rw-   0        0        0     5550 2022-08-29 00:04:37.000000 deta-discord-interactions-0.1.0/deta_discord_interactions/models/option.py
--rw-rw-rw-   0        0        0     2385 2022-08-28 00:25:18.000000 deta-discord-interactions-0.1.0/deta_discord_interactions/models/permission.py
--rw-rw-rw-   0        0        0     1234 2023-06-01 01:13:01.000000 deta-discord-interactions-0.1.0/deta_discord_interactions/models/role.py
--rw-rw-rw-   0        0        0     5159 2023-06-01 01:13:01.000000 deta-discord-interactions-0.1.0/deta_discord_interactions/models/user.py
--rw-rw-rw-   0        0        0     3505 2023-06-01 01:13:01.000000 deta-discord-interactions-0.1.0/deta_discord_interactions/models/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-01 01:14:19.760570 deta-discord-interactions-0.1.0/deta_discord_interactions/tests/
--rw-rw-rw-   0        0        0        0 2022-08-28 00:25:18.000000 deta-discord-interactions-0.1.0/deta_discord_interactions/tests/__init__.py
--rw-rw-rw-   0        0        0     1288 2023-06-01 01:13:01.000000 deta-discord-interactions-0.1.0/deta_discord_interactions/tests/conftest.py
--rw-rw-rw-   0        0        0     1900 2022-08-28 00:25:18.000000 deta-discord-interactions-0.1.0/deta_discord_interactions/tests/test_command.py
--rw-rw-rw-   0        0        0     5026 2023-06-01 01:13:01.000000 deta-discord-interactions-0.1.0/deta_discord_interactions/tests/test_component.py
--rw-rw-rw-   0        0        0     9573 2023-06-01 01:13:01.000000 deta-discord-interactions-0.1.0/deta_discord_interactions/tests/test_context.py
--rw-rw-rw-   0        0        0     8984 2023-06-01 01:13:01.000000 deta-discord-interactions-0.1.0/deta_discord_interactions/tests/test_database.py
--rw-rw-rw-   0        0        0     2991 2023-06-01 01:13:01.000000 deta-discord-interactions-0.1.0/deta_discord_interactions/tests/test_handler.py
--rw-rw-rw-   0        0        0     3151 2023-06-01 01:13:01.000000 deta-discord-interactions-0.1.0/deta_discord_interactions/tests/test_http.py
--rw-rw-rw-   0        0        0     2142 2023-06-01 01:13:01.000000 deta-discord-interactions-0.1.0/deta_discord_interactions/tests/test_oauth.py
--rw-rw-rw-   0        0        0     4064 2022-08-28 00:25:18.000000 deta-discord-interactions-0.1.0/deta_discord_interactions/tests/test_options.py
--rw-rw-rw-   0        0        0      301 2023-03-05 07:47:55.000000 deta-discord-interactions-0.1.0/deta_discord_interactions/tests/test_ping.py
--rw-rw-rw-   0        0        0     1986 2023-06-01 01:13:01.000000 deta-discord-interactions-0.1.0/deta_discord_interactions/tests/test_register.py
--rw-rw-rw-   0        0        0     2687 2023-06-01 01:13:01.000000 deta-discord-interactions-0.1.0/deta_discord_interactions/tests/test_response.py
--rw-rw-rw-   0        0        0     3042 2022-08-28 00:25:18.000000 deta-discord-interactions-0.1.0/deta_discord_interactions/tests/test_subcommand.py
--rw-rw-rw-   0        0        0     1549 2023-06-01 01:13:01.000000 deta-discord-interactions-0.1.0/deta_discord_interactions/tests/test_wsgi.py
-drwxrwxrwx   0        0        0        0 2023-06-01 01:14:19.764645 deta-discord-interactions-0.1.0/deta_discord_interactions/utils/
--rw-rw-rw-   0        0        0        0 2023-06-01 01:13:01.000000 deta-discord-interactions-0.1.0/deta_discord_interactions/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-01 01:14:19.777267 deta-discord-interactions-0.1.0/deta_discord_interactions/utils/cooldown/
--rw-rw-rw-   0        0        0     2745 2023-06-01 01:13:01.000000 deta-discord-interactions-0.1.0/deta_discord_interactions/utils/cooldown/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-01 01:14:19.833987 deta-discord-interactions-0.1.0/deta_discord_interactions/utils/database/
--rw-rw-rw-   0        0        0      400 2023-06-01 01:13:01.000000 deta-discord-interactions-0.1.0/deta_discord_interactions/utils/database/__init__.py
--rw-rw-rw-   0        0        0     6439 2023-06-01 01:13:01.000000 deta-discord-interactions-0.1.0/deta_discord_interactions/utils/database/_local_base.py
--rw-rw-rw-   0        0        0     1469 2023-06-01 01:13:01.000000 deta-discord-interactions-0.1.0/deta_discord_interactions/utils/database/bound_meta.py
--rw-rw-rw-   0        0        0    17784 2023-06-01 01:13:01.000000 deta-discord-interactions-0.1.0/deta_discord_interactions/utils/database/database.py
--rw-rw-rw-   0        0        0      468 2023-06-01 01:13:01.000000 deta-discord-interactions-0.1.0/deta_discord_interactions/utils/database/exceptions.py
--rw-rw-rw-   0        0        0     4838 2023-06-01 01:13:01.000000 deta-discord-interactions-0.1.0/deta_discord_interactions/utils/database/query.py
-drwxrwxrwx   0        0        0        0 2023-06-01 01:14:19.846978 deta-discord-interactions-0.1.0/deta_discord_interactions/utils/oauth/
--rw-rw-rw-   0        0        0      506 2023-06-01 01:13:01.000000 deta-discord-interactions-0.1.0/deta_discord_interactions/utils/oauth/__init__.py
--rw-rw-rw-   0        0        0    10089 2023-06-01 01:13:01.000000 deta-discord-interactions-0.1.0/deta_discord_interactions/utils/oauth/model.py
--rw-rw-rw-   0        0        0     9292 2023-06-01 01:13:01.000000 deta-discord-interactions-0.1.0/deta_discord_interactions/utils/oauth/oauth.py
-drwxrwxrwx   0        0        0        0 2023-06-01 01:14:19.444738 deta-discord-interactions-0.1.0/deta_discord_interactions.egg-info/
--rw-rw-rw-   0        0        0     1489 2023-06-01 01:14:19.000000 deta-discord-interactions-0.1.0/deta_discord_interactions.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2630 2023-06-01 01:14:19.000000 deta-discord-interactions-0.1.0/deta_discord_interactions.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 01:14:19.000000 deta-discord-interactions-0.1.0/deta_discord_interactions.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-08-27 15:46:21.000000 deta-discord-interactions-0.1.0/deta_discord_interactions.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       39 2023-06-01 01:14:19.000000 deta-discord-interactions-0.1.0/deta_discord_interactions.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2023-06-01 01:14:19.000000 deta-discord-interactions-0.1.0/deta_discord_interactions.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      797 2023-06-01 01:13:01.000000 deta-discord-interactions-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-01 01:14:19.852995 deta-discord-interactions-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      983 2023-06-01 01:13:01.000000 deta-discord-interactions-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-10 21:26:45.458335 deta-discord-interactions-0.1.1/
+-rw-rw-rw-   0        0        0     1096 2022-08-22 23:01:27.000000 deta-discord-interactions-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     2221 2023-06-10 21:26:45.456219 deta-discord-interactions-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1478 2023-06-03 22:21:55.000000 deta-discord-interactions-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-10 21:26:45.288437 deta-discord-interactions-0.1.1/deta_discord_interactions/
+-rw-rw-rw-   0        0        0     1722 2022-08-28 00:25:18.000000 deta-discord-interactions-0.1.1/deta_discord_interactions/__init__.py
+-rw-rw-rw-   0        0        0     5804 2023-06-10 21:26:10.000000 deta-discord-interactions-0.1.1/deta_discord_interactions/client.py
+-rw-rw-rw-   0        0        0    19166 2023-06-01 01:13:01.000000 deta-discord-interactions-0.1.1/deta_discord_interactions/command.py
+-rw-rw-rw-   0        0        0    17881 2023-06-03 18:57:19.000000 deta-discord-interactions-0.1.1/deta_discord_interactions/context.py
+-rw-rw-rw-   0        0        0    26503 2023-06-03 16:38:40.000000 deta-discord-interactions-0.1.1/deta_discord_interactions/discord.py
+drwxrwxrwx   0        0        0        0 2023-06-10 21:26:45.329589 deta-discord-interactions-0.1.1/deta_discord_interactions/enums/
+-rw-rw-rw-   0        0        0      199 2022-09-04 14:09:17.000000 deta-discord-interactions-0.1.1/deta_discord_interactions/enums/__init__.py
+-rw-rw-rw-   0        0        0     1315 2022-09-04 14:09:10.000000 deta-discord-interactions-0.1.1/deta_discord_interactions/enums/permissions.py
+-rw-rw-rw-   0        0        0      295 2022-08-28 00:25:18.000000 deta-discord-interactions-0.1.1/deta_discord_interactions/enums/response_types.py
+-rw-rw-rw-   0        0        0     4339 2023-06-01 01:13:01.000000 deta-discord-interactions-0.1.1/deta_discord_interactions/http.py
+drwxrwxrwx   0        0        0        0 2023-06-10 21:26:45.372474 deta-discord-interactions-0.1.1/deta_discord_interactions/models/
+-rw-rw-rw-   0        0        0     1721 2022-08-28 00:25:18.000000 deta-discord-interactions-0.1.1/deta_discord_interactions/models/__init__.py
+-rw-rw-rw-   0        0        0     1246 2022-08-28 00:25:18.000000 deta-discord-interactions-0.1.1/deta_discord_interactions/models/attachment.py
+-rw-rw-rw-   0        0        0     2656 2023-06-10 21:26:10.000000 deta-discord-interactions-0.1.1/deta_discord_interactions/models/autocomplete.py
+-rw-rw-rw-   0        0        0     1387 2023-06-01 01:13:01.000000 deta-discord-interactions-0.1.1/deta_discord_interactions/models/channel.py
+-rw-rw-rw-   0        0        0      150 2022-08-28 00:25:18.000000 deta-discord-interactions-0.1.1/deta_discord_interactions/models/command.py
+-rw-rw-rw-   0        0        0     8568 2023-06-10 21:26:10.000000 deta-discord-interactions-0.1.1/deta_discord_interactions/models/component.py
+-rw-rw-rw-   0        0        0     2806 2023-06-01 01:13:01.000000 deta-discord-interactions-0.1.1/deta_discord_interactions/models/embed.py
+-rw-rw-rw-   0        0        0      822 2022-08-28 00:25:18.000000 deta-discord-interactions-0.1.1/deta_discord_interactions/models/interaction.py
+-rw-rw-rw-   0        0        0     8113 2023-06-01 01:13:01.000000 deta-discord-interactions-0.1.1/deta_discord_interactions/models/message.py
+-rw-rw-rw-   0        0        0     2932 2023-06-01 01:13:01.000000 deta-discord-interactions-0.1.1/deta_discord_interactions/models/modal.py
+-rw-rw-rw-   0        0        0     5550 2022-08-29 00:04:37.000000 deta-discord-interactions-0.1.1/deta_discord_interactions/models/option.py
+-rw-rw-rw-   0        0        0     2385 2022-08-28 00:25:18.000000 deta-discord-interactions-0.1.1/deta_discord_interactions/models/permission.py
+-rw-rw-rw-   0        0        0     1234 2023-06-01 01:13:01.000000 deta-discord-interactions-0.1.1/deta_discord_interactions/models/role.py
+-rw-rw-rw-   0        0        0     5159 2023-06-01 01:13:01.000000 deta-discord-interactions-0.1.1/deta_discord_interactions/models/user.py
+-rw-rw-rw-   0        0        0     3505 2023-06-01 01:13:01.000000 deta-discord-interactions-0.1.1/deta_discord_interactions/models/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-10 21:26:45.416423 deta-discord-interactions-0.1.1/deta_discord_interactions/tests/
+-rw-rw-rw-   0        0        0        0 2022-08-28 00:25:18.000000 deta-discord-interactions-0.1.1/deta_discord_interactions/tests/__init__.py
+-rw-rw-rw-   0        0        0     1288 2023-06-01 01:13:01.000000 deta-discord-interactions-0.1.1/deta_discord_interactions/tests/conftest.py
+-rw-rw-rw-   0        0        0     1900 2022-08-28 00:25:18.000000 deta-discord-interactions-0.1.1/deta_discord_interactions/tests/test_command.py
+-rw-rw-rw-   0        0        0     5026 2023-06-01 01:13:01.000000 deta-discord-interactions-0.1.1/deta_discord_interactions/tests/test_component.py
+-rw-rw-rw-   0        0        0     9573 2023-06-01 01:13:01.000000 deta-discord-interactions-0.1.1/deta_discord_interactions/tests/test_context.py
+-rw-rw-rw-   0        0        0     9016 2023-06-10 21:26:10.000000 deta-discord-interactions-0.1.1/deta_discord_interactions/tests/test_database.py
+-rw-rw-rw-   0        0        0     5825 2023-06-10 21:26:10.000000 deta-discord-interactions-0.1.1/deta_discord_interactions/tests/test_drive.py
+-rw-rw-rw-   0        0        0     2991 2023-06-01 01:13:01.000000 deta-discord-interactions-0.1.1/deta_discord_interactions/tests/test_handler.py
+-rw-rw-rw-   0        0        0     3151 2023-06-01 01:13:01.000000 deta-discord-interactions-0.1.1/deta_discord_interactions/tests/test_http.py
+-rw-rw-rw-   0        0        0     2142 2023-06-01 01:13:01.000000 deta-discord-interactions-0.1.1/deta_discord_interactions/tests/test_oauth.py
+-rw-rw-rw-   0        0        0     4064 2022-08-28 00:25:18.000000 deta-discord-interactions-0.1.1/deta_discord_interactions/tests/test_options.py
+-rw-rw-rw-   0        0        0      301 2023-03-05 07:47:55.000000 deta-discord-interactions-0.1.1/deta_discord_interactions/tests/test_ping.py
+-rw-rw-rw-   0        0        0     1986 2023-06-01 01:13:01.000000 deta-discord-interactions-0.1.1/deta_discord_interactions/tests/test_register.py
+-rw-rw-rw-   0        0        0     2687 2023-06-01 01:13:01.000000 deta-discord-interactions-0.1.1/deta_discord_interactions/tests/test_response.py
+-rw-rw-rw-   0        0        0     3042 2022-08-28 00:25:18.000000 deta-discord-interactions-0.1.1/deta_discord_interactions/tests/test_subcommand.py
+-rw-rw-rw-   0        0        0     1549 2023-06-01 01:13:01.000000 deta-discord-interactions-0.1.1/deta_discord_interactions/tests/test_wsgi.py
+drwxrwxrwx   0        0        0        0 2023-06-10 21:26:45.419453 deta-discord-interactions-0.1.1/deta_discord_interactions/utils/
+-rw-rw-rw-   0        0        0        0 2023-06-01 01:13:01.000000 deta-discord-interactions-0.1.1/deta_discord_interactions/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-10 21:26:45.420970 deta-discord-interactions-0.1.1/deta_discord_interactions/utils/cooldown/
+-rw-rw-rw-   0        0        0     2745 2023-06-01 01:13:01.000000 deta-discord-interactions-0.1.1/deta_discord_interactions/utils/cooldown/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-10 21:26:45.443136 deta-discord-interactions-0.1.1/deta_discord_interactions/utils/database/
+-rw-rw-rw-   0        0        0      540 2023-06-10 21:26:10.000000 deta-discord-interactions-0.1.1/deta_discord_interactions/utils/database/__init__.py
+-rw-rw-rw-   0        0        0     6439 2023-06-01 01:13:01.000000 deta-discord-interactions-0.1.1/deta_discord_interactions/utils/database/_local_base.py
+-rw-rw-rw-   0        0        0     4873 2023-06-10 21:26:10.000000 deta-discord-interactions-0.1.1/deta_discord_interactions/utils/database/_local_drive.py
+-rw-rw-rw-   0        0        0     1469 2023-06-01 01:13:01.000000 deta-discord-interactions-0.1.1/deta_discord_interactions/utils/database/bound_meta.py
+-rw-rw-rw-   0        0        0    17734 2023-06-10 21:26:10.000000 deta-discord-interactions-0.1.1/deta_discord_interactions/utils/database/database.py
+-rw-rw-rw-   0        0        0    13740 2023-06-10 21:26:10.000000 deta-discord-interactions-0.1.1/deta_discord_interactions/utils/database/drive.py
+-rw-rw-rw-   0        0        0      572 2023-06-10 21:26:10.000000 deta-discord-interactions-0.1.1/deta_discord_interactions/utils/database/exceptions.py
+-rw-rw-rw-   0        0        0     4838 2023-06-01 01:13:01.000000 deta-discord-interactions-0.1.1/deta_discord_interactions/utils/database/query.py
+drwxrwxrwx   0        0        0        0 2023-06-10 21:26:45.452963 deta-discord-interactions-0.1.1/deta_discord_interactions/utils/oauth/
+-rw-rw-rw-   0        0        0      506 2023-06-01 01:13:01.000000 deta-discord-interactions-0.1.1/deta_discord_interactions/utils/oauth/__init__.py
+-rw-rw-rw-   0        0        0    10089 2023-06-01 01:13:01.000000 deta-discord-interactions-0.1.1/deta_discord_interactions/utils/oauth/model.py
+-rw-rw-rw-   0        0        0     9351 2023-06-03 20:57:34.000000 deta-discord-interactions-0.1.1/deta_discord_interactions/utils/oauth/oauth.py
+drwxrwxrwx   0        0        0        0 2023-06-10 21:26:45.323410 deta-discord-interactions-0.1.1/deta_discord_interactions.egg-info/
+-rw-rw-rw-   0        0        0     2221 2023-06-10 21:26:45.000000 deta-discord-interactions-0.1.1/deta_discord_interactions.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2783 2023-06-10 21:26:45.000000 deta-discord-interactions-0.1.1/deta_discord_interactions.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-10 21:26:45.000000 deta-discord-interactions-0.1.1/deta_discord_interactions.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2022-08-27 15:46:21.000000 deta-discord-interactions-0.1.1/deta_discord_interactions.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       39 2023-06-10 21:26:45.000000 deta-discord-interactions-0.1.1/deta_discord_interactions.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2023-06-10 21:26:45.000000 deta-discord-interactions-0.1.1/deta_discord_interactions.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      797 2023-06-10 21:26:10.000000 deta-discord-interactions-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-10 21:26:45.458335 deta-discord-interactions-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      983 2023-06-10 21:26:10.000000 deta-discord-interactions-0.1.1/setup.py
```

### Comparing `deta-discord-interactions-0.1.0/LICENSE` & `deta-discord-interactions-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `deta-discord-interactions-0.1.0/PKG-INFO` & `deta-discord-interactions-0.1.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deta-discord-interactions
-Version: 0.1.0
+Version: 0.1.1
 Summary: A web framework for Discord interactions specialized for usage in https://deta.sh
 Home-page: https://github.com/etrotta/flask-discord-interactions/tree/deta
 Author: etrotta
 Author-email: etrotta <etrotta@duck.com>
 License: MIT
 Project-URL: Homepage, https://github.com/etrotta/flask-discord-interactions/tree/deta
 Project-URL: Bug Tracker, https://github.com/etrotta/flask-discord-interactions/issues
@@ -27,7 +27,19 @@
 def ping(ctx):
     "Respond with a friendly 'pong'!"
     return "Pong!"
 ```
 
 The documentation of the original library is available on [readthedocs](https://flask-discord-interactions.readthedocs.io/).
 The documentation of the Fork is still Work in Progress.
+
+
+
+## Known issues
+- No good way to defer nor follow up (any spawned threads are killed as soon as the main function returns)
+- The Deta Space changes made it a quite few times more complicated to setup than Cloud used to be
+- Not particularly beginner friendly
+- Poorly documented
+
+## As far as security goes
+The `http.server` module of the standard library that `deta_discord_interactions.http` relies on is not recommended for production usage. Use it at your own risk.
+Any server that supports [PEP 3333](https://peps.python.org/pep-3333/) and works in serverless environments should work, so you may want to use something like https://gunicorn.org/ instead of the `deta_discord_interactions.http` used in Examples.
```

### Comparing `deta-discord-interactions-0.1.0/deta_discord_interactions/__init__.py` & `deta-discord-interactions-0.1.1/deta_discord_interactions/__init__.py`

 * *Files identical despite different names*

### Comparing `deta-discord-interactions-0.1.0/deta_discord_interactions/client.py` & `deta-discord-interactions-0.1.1/deta_discord_interactions/client.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import copy
 from contextlib import contextmanager
 import typing
 
 from deta_discord_interactions.context import Context
 from deta_discord_interactions.models import Message
+from deta_discord_interactions.models import Modal
 from deta_discord_interactions.models import AutocompleteResult, Option
 from deta_discord_interactions.command import SlashCommandSubgroup
 from deta_discord_interactions.models.command import ApplicationCommandType
 
 if typing.TYPE_CHECKING:
     from deta_discord_interactions.discord import DiscordInteractions
 
@@ -47,15 +48,15 @@
         else:
             self.current_context = Context()
         try:
             yield self.current_context
         finally:
             self.current_context = Context()
 
-    def run(self, *names, **params):
+    def run(self, *names, **params) -> typing.Union[Message, Modal]:
         """
         Run a specified Application Command.
 
         Parameters
         ----------
         *names
             The names of the command, subcommand group, and subcommand (if
@@ -72,27 +73,27 @@
             for i in range(1, len(names)):
                 if not isinstance(command, SlashCommandSubgroup):
                     break
                 command = command.subcommands[names[i]]
             else:
                 i += 1
 
-            return Message.from_return_value(
-                command.run(self.current_context, *names[i:], **params)
-            )
+            result = command.run(self.current_context, *names[i:], **params)
         elif command.type == ApplicationCommandType.MESSAGE:
-            return Message.from_return_value(
-                command.run(self.current_context, self.current_context.target_message)
-            )
+            result = command.run(self.current_context, self.current_context.target_message)
         elif command.type == ApplicationCommandType.USER:
-            return Message.from_return_value(
-                command.run(self.current_context, self.current_context.target_user)
-            )
+            result = command.run(self.current_context, self.current_context.target_user)
+        else:
+            raise Exception("Invalid command type")
+
+        if isinstance(result, Modal):
+            return result
+        return Message.from_return_value(result)
 
-    def run_handler(self, custom_id: str, *args):
+    def run_handler(self, custom_id: str, *args) -> typing.Union[Message, Modal]:
         """
         Run a specified custom ID handler.
 
         Parameters
         ----------
         custom_id
             The ID of the handler function to run.
@@ -104,16 +105,17 @@
 
         new_context.custom_id = "\n".join((custom_id, *args))
         new_context.parse_custom_id()
 
         handler = self.discord.custom_id_handlers[new_context.primary_id]
 
         args = new_context.create_handler_args(handler)
-
         response = handler(new_context, *args)
+        if isinstance(response, Modal):
+            return response
         return Message.from_return_value(response)
 
 
     def run_autocomplete(self, *names, **params):
         """
         Run the Autocomplete for a specified Application Command.
```

### Comparing `deta-discord-interactions-0.1.0/deta_discord_interactions/command.py` & `deta-discord-interactions-0.1.1/deta_discord_interactions/command.py`

 * *Files identical despite different names*

### Comparing `deta-discord-interactions-0.1.0/deta_discord_interactions/context.py` & `deta-discord-interactions-0.1.1/deta_discord_interactions/context.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,15 +86,15 @@
     type: int = None
     command_type: int = None
     token: str = None
     channel_id: str = None
     guild_id: str = None
     options: list = None
     values: list = None
-    components: list = None
+    components: list = None  # TODO check load/parse when loading from base?
     resolved: dict = None
     command_name: str = None
     command_id: str = None
     members: Optional[list[Member]] = None
     channels: Optional[list[Channel]] = None
     roles: Optional[list[Role]] = None
     message: Optional[Message] = None
@@ -510,15 +510,15 @@
             return self.command_id
         else:
             try:
                 return self.discord.discord_commands[command_name].id
             except KeyError:
                 raise ValueError(f"Unknown command: {command_name}")
 
-    def get_component(self, component_id: str):
+    def get_component(self, component_id: str) -> Component:
         """
         Get a Component, only available for Modal Contexts.
         If the component was not found, raises a LookupError.
 
         Parameters
         ----------
         component_id: str
```

### Comparing `deta-discord-interactions-0.1.0/deta_discord_interactions/discord.py` & `deta-discord-interactions-0.1.1/deta_discord_interactions/discord.py`

 * *Files identical despite different names*

### Comparing `deta-discord-interactions-0.1.0/deta_discord_interactions/enums/permissions.py` & `deta-discord-interactions-0.1.1/deta_discord_interactions/enums/permissions.py`

 * *Files identical despite different names*

### Comparing `deta-discord-interactions-0.1.0/deta_discord_interactions/http.py` & `deta-discord-interactions-0.1.1/deta_discord_interactions/http.py`

 * *Files identical despite different names*

### Comparing `deta-discord-interactions-0.1.0/deta_discord_interactions/models/__init__.py` & `deta-discord-interactions-0.1.1/deta_discord_interactions/models/__init__.py`

 * *Files identical despite different names*

### Comparing `deta-discord-interactions-0.1.0/deta_discord_interactions/models/attachment.py` & `deta-discord-interactions-0.1.1/deta_discord_interactions/models/attachment.py`

 * *Files identical despite different names*

### Comparing `deta-discord-interactions-0.1.0/deta_discord_interactions/models/autocomplete.py` & `deta-discord-interactions-0.1.1/deta_discord_interactions/models/autocomplete.py`

 * *Files 9% similar despite different names*

```diff
@@ -34,30 +34,30 @@
     Represents the result of an autocomplete handler.
 
     Parameters
     ----------
     choices
         A list of dicts representing the choices to be presented to the user.
     """
-    choices: list[dict]
+    choices: list[Choice]
 
     def encode(self):
         """
         Return this result as a complete interaction response.
 
         Returns
         -------
         bytes
             The encoded JSON object.
         str
             The mimetype of the response (``application/json``).
         """
         data = {
             "type": ResponseType.APPLICATION_COMMAND_AUTOCOMPLETE_RESULT,
-            "data": {"choices": self.choices},
+            "data": {"choices": [choice.dump() for choice in self.choices]},
         }
 
         return json.dumps(data).encode("UTF-8"), "application/json"
 
     @classmethod
     def from_return_value(cls, value: Union[dict, list, "AutocompleteResult"]):
         """
@@ -73,20 +73,17 @@
         -------
         AutocompleteResult
             The AutocompleteResult that corresponds to the return value.
         """
         if isinstance(value, AutocompleteResult):
             return value
         elif isinstance(value, dict):
-            return cls([value])
-        elif isinstance(value, list) and all(
-            isinstance(choice, dict) for choice in value
-        ):
-            return cls(value)
-        elif isinstance(value, list) and all(
-            isinstance(choice, Choice) for choice in value
-        ):
-            return cls([choice.dump() for choice in value])
+            return cls([Choice(name=key, value=val) for key, val in value.items()])
         elif isinstance(value, list):
-            return cls(
-                [{"name": str(choice), "value": choice} for choice in value]
-            )
+            if all(isinstance(x, Choice) for x in value):
+                return cls(value)
+            elif all(isinstance(x, dict) for x in value):
+                return cls([Choice(d["name"], d["value"], d.get("name_localizations")) for d in value])
+        
+        return cls(
+            [Choice(str(choice), choice) for choice in value]
+        )
```

### Comparing `deta-discord-interactions-0.1.0/deta_discord_interactions/models/channel.py` & `deta-discord-interactions-0.1.1/deta_discord_interactions/models/channel.py`

 * *Files identical despite different names*

### Comparing `deta-discord-interactions-0.1.0/deta_discord_interactions/models/component.py` & `deta-discord-interactions-0.1.1/deta_discord_interactions/models/component.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,15 +149,15 @@
         if self.style == ButtonStyles.LINK:
             if self.url is None or self.label is None:
                 raise ValueError("Link buttons must have an url and label")
         else:
             if self.custom_id is None:
                 raise ValueError("Buttons must have a custom_id")
 
-        if isinstance(self.custom_id, list) or isinstance(self.custom_id, tuple):
+        if isinstance(self.custom_id, (list, tuple)):
             self.custom_id = "\n".join(str(item) for item in self.custom_id)
 
         if self.custom_id and len(self.custom_id) > 100:
             raise ValueError("custom_id has maximum 100 characters")
 
 
 @dataclass
```

### Comparing `deta-discord-interactions-0.1.0/deta_discord_interactions/models/embed.py` & `deta-discord-interactions-0.1.1/deta_discord_interactions/models/embed.py`

 * *Files identical despite different names*

### Comparing `deta-discord-interactions-0.1.0/deta_discord_interactions/models/interaction.py` & `deta-discord-interactions-0.1.1/deta_discord_interactions/models/interaction.py`

 * *Files identical despite different names*

### Comparing `deta-discord-interactions-0.1.0/deta_discord_interactions/models/message.py` & `deta-discord-interactions-0.1.1/deta_discord_interactions/models/message.py`

 * *Files identical despite different names*

### Comparing `deta-discord-interactions-0.1.0/deta_discord_interactions/models/modal.py` & `deta-discord-interactions-0.1.1/deta_discord_interactions/models/modal.py`

 * *Files identical despite different names*

### Comparing `deta-discord-interactions-0.1.0/deta_discord_interactions/models/option.py` & `deta-discord-interactions-0.1.1/deta_discord_interactions/models/option.py`

 * *Files identical despite different names*

### Comparing `deta-discord-interactions-0.1.0/deta_discord_interactions/models/permission.py` & `deta-discord-interactions-0.1.1/deta_discord_interactions/models/permission.py`

 * *Files identical despite different names*

### Comparing `deta-discord-interactions-0.1.0/deta_discord_interactions/models/role.py` & `deta-discord-interactions-0.1.1/deta_discord_interactions/models/role.py`

 * *Files identical despite different names*

### Comparing `deta-discord-interactions-0.1.0/deta_discord_interactions/models/user.py` & `deta-discord-interactions-0.1.1/deta_discord_interactions/models/user.py`

 * *Files identical despite different names*

### Comparing `deta-discord-interactions-0.1.0/deta_discord_interactions/models/utils.py` & `deta-discord-interactions-0.1.1/deta_discord_interactions/models/utils.py`

 * *Files identical despite different names*

### Comparing `deta-discord-interactions-0.1.0/deta_discord_interactions/tests/conftest.py` & `deta-discord-interactions-0.1.1/deta_discord_interactions/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `deta-discord-interactions-0.1.0/deta_discord_interactions/tests/test_command.py` & `deta-discord-interactions-0.1.1/deta_discord_interactions/tests/test_command.py`

 * *Files identical despite different names*

### Comparing `deta-discord-interactions-0.1.0/deta_discord_interactions/tests/test_component.py` & `deta-discord-interactions-0.1.1/deta_discord_interactions/tests/test_component.py`

 * *Files identical despite different names*

### Comparing `deta-discord-interactions-0.1.0/deta_discord_interactions/tests/test_context.py` & `deta-discord-interactions-0.1.1/deta_discord_interactions/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `deta-discord-interactions-0.1.0/deta_discord_interactions/tests/test_database.py` & `deta-discord-interactions-0.1.1/deta_discord_interactions/tests/test_database.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 @dataclasses.dataclass
 class Mini(LoadableDataclass):
     a: int
     b: float
 
 @dataclasses.dataclass
-class TestRecord(LoadableDataclass):
+class MyTestRecord(LoadableDataclass):
     name: str
     number: int
     date: datetime.datetime
     func: typing.Callable
     nested: Mini
 
 @dataclasses.dataclass
@@ -27,19 +27,19 @@
     nested_list: list[Mini]
     keys: set
     nested_dict: dict[str, Mini]
 
 
 @pytest.fixture()
 def database():
-    return Database("test_database", record_type=TestRecord, base_mode="MEMORY")
+    return Database("test_database", record_type=MyTestRecord, base_mode="MEMORY")
 
 @pytest.fixture()
 def disk_database(tmp_path):
-    return Database("test_database", record_type=TestRecord, base_mode="DISK", base_folder=tmp_path)
+    return Database("test_database", record_type=MyTestRecord, base_mode="DISK", base_folder=tmp_path)
 
 @pytest.fixture()
 def weird_disk_database(tmp_path):
     return Database("weird_test_database", record_type=WeirdTestRecord, base_mode="DISK", base_folder=tmp_path)
 
 @pytest.fixture()
 def foo_func(database: Database, disk_database: Database):
@@ -51,15 +51,15 @@
 
 @pytest.fixture()
 def mini_rec():
     return Mini(1, 2.0)
 
 @pytest.fixture()
 def foo_rec(foo_func, mini_rec):
-    foo = TestRecord(
+    foo = MyTestRecord(
         "foo",
         1,
         datetime.datetime.fromisoformat("2020-01-01"),
         foo_func,
         mini_rec,
     )
     return foo
@@ -76,18 +76,18 @@
         {1: mini_rec, "a": mini_rec, "b": mini_rec},
     )
     return rec
 
 DATE = datetime.datetime.fromisoformat("2020-01-01")
 
 def test_encode_decode(
-        database: Database[str, TestRecord],
+        database: Database[str, MyTestRecord],
         mini_rec: Mini,
         foo_func: typing.Callable,
-        foo_rec: TestRecord,
+        foo_rec: MyTestRecord,
         weird_rec: WeirdTestRecord,
     ):
     # Part 1) to_dict()
     assert mini_rec.to_dict() == {"a": 1, "b": 2.0}
     assert foo_rec.to_dict() == {
         "name": "foo",
         "number": 1,
@@ -128,15 +128,15 @@
     }
 
     # Part 3) database decoding
     assert database.decode_entry(database.encode_entry(mini_rec.to_dict())) == mini_rec.to_dict()
     assert database.decode_entry(database.encode_entry(foo_rec.to_dict())) == foo_rec.to_dict()
     assert database.decode_entry(database.encode_entry(weird_rec.to_dict())) == weird_rec.to_dict()
 
-def test_record_loading(database: Database[str, TestRecord], foo_rec: TestRecord, mini_rec: Mini, weird_rec: WeirdTestRecord):
+def test_record_loading(database: Database[str, MyTestRecord], foo_rec: MyTestRecord, mini_rec: Mini, weird_rec: WeirdTestRecord):
     # Part 4) record loading
     assert mini_rec.from_dict(mini_rec.to_dict()) == mini_rec
     assert foo_rec.from_dict(foo_rec.to_dict()) == foo_rec
     assert weird_rec.from_dict(weird_rec.to_dict()) == weird_rec
     
     # Check that the nested things also work
     assert foo_rec.from_dict(foo_rec.to_dict()).nested == foo_rec.nested
@@ -148,15 +148,15 @@
     assert foo_rec.from_dict(database.decode_entry(database.encode_entry(foo_rec.to_dict()))) == foo_rec
     assert weird_rec.from_dict(database.decode_entry(database.encode_entry(weird_rec.to_dict()))) == weird_rec
     
     # Check that the nested things also work
     assert foo_rec.from_dict(database.decode_entry(database.encode_entry(foo_rec.to_dict()))).nested == foo_rec.nested
     assert foo_rec.from_dict(database.decode_entry(database.encode_entry(foo_rec.to_dict()))).func() == foo_rec.func()
 
-def test_record_storing(database: Database[str, TestRecord], foo_rec: TestRecord):
+def test_record_storing(database: Database[str, MyTestRecord], foo_rec: MyTestRecord):
     # Part 6) storing and retrieving
     # not gonna lie, may have skipped a few steps, but whatever
     # Currently this uses an in-memory proxy-ish database
     # in the future it may be better to use monkeypatching 
     # and make sure that the requests it makes to the API look right
     database["foo"] = foo_rec
     assert database["foo"] == foo_rec
@@ -182,15 +182,15 @@
     database.put_many([foo_rec], key_source="name")
     assert database.get("foo") == foo_rec
 
     del database["foo"]
     database.put_many({"foo": foo_rec})
     assert database.get("foo") == foo_rec
 
-def test_queries(database: Database[str, TestRecord], foo_rec: TestRecord):
+def test_queries(database: Database[str, MyTestRecord], foo_rec: MyTestRecord):
     # Currently this uses an in-memory proxy-ish database
     # in the future it may be better to use monkeypatching 
     # and make sure that the requests it makes to the API look right
     database["foo"] = foo_rec
 
     # Basic usage working properly...
     records = database.fetch()
@@ -213,18 +213,18 @@
     records = database.fetch(Query(Field("key") == "bar"))
     assert records == []
     records = database.fetch(Query(Field("number") == 2, Field("date") == DATE))
     assert records == []
 
 
 def test_disk_database(
-        disk_database: Database[str, TestRecord],
-        foo_rec: TestRecord,
+        disk_database: Database[str, MyTestRecord],
+        foo_rec: MyTestRecord,
         weird_disk_database: Database[str, WeirdTestRecord],
-        weird_rec: TestRecord,
+        weird_rec: MyTestRecord,
 ):
     disk_database["foo"] = foo_rec
     weird_disk_database["foo"] = weird_rec
     assert disk_database["foo"] == foo_rec
     assert weird_disk_database["foo"] == weird_rec
 
     # Part 7) Other methods
@@ -235,15 +235,15 @@
     disk_database.put("foo", foo_rec)
     assert disk_database["foo"].number == 1
     
     foo_rec.number = 2
     disk_database.put("foo", foo_rec)
 
     _path = disk_database._Database__base.inventory._path
-    copy = Database("test_database", record_type=TestRecord, base_mode="DISK", base_folder=_path.parent)
+    copy = Database("test_database", record_type=MyTestRecord, base_mode="DISK", base_folder=_path.parent)
     copy.remember_function(foo_rec.func)
     assert copy["foo"].number == 2
     del copy
 
     foo_rec.number = 3
     with pytest.raises(Exception):
         disk_database.insert("foo", foo_rec)
```

### Comparing `deta-discord-interactions-0.1.0/deta_discord_interactions/tests/test_handler.py` & `deta-discord-interactions-0.1.1/deta_discord_interactions/tests/test_handler.py`

 * *Files identical despite different names*

### Comparing `deta-discord-interactions-0.1.0/deta_discord_interactions/tests/test_http.py` & `deta-discord-interactions-0.1.1/deta_discord_interactions/tests/test_http.py`

 * *Files identical despite different names*

### Comparing `deta-discord-interactions-0.1.0/deta_discord_interactions/tests/test_oauth.py` & `deta-discord-interactions-0.1.1/deta_discord_interactions/tests/test_oauth.py`

 * *Files identical despite different names*

### Comparing `deta-discord-interactions-0.1.0/deta_discord_interactions/tests/test_options.py` & `deta-discord-interactions-0.1.1/deta_discord_interactions/tests/test_options.py`

 * *Files identical despite different names*

### Comparing `deta-discord-interactions-0.1.0/deta_discord_interactions/tests/test_register.py` & `deta-discord-interactions-0.1.1/deta_discord_interactions/tests/test_register.py`

 * *Files identical despite different names*

### Comparing `deta-discord-interactions-0.1.0/deta_discord_interactions/tests/test_response.py` & `deta-discord-interactions-0.1.1/deta_discord_interactions/tests/test_response.py`

 * *Files identical despite different names*

### Comparing `deta-discord-interactions-0.1.0/deta_discord_interactions/tests/test_subcommand.py` & `deta-discord-interactions-0.1.1/deta_discord_interactions/tests/test_subcommand.py`

 * *Files identical despite different names*

### Comparing `deta-discord-interactions-0.1.0/deta_discord_interactions/tests/test_wsgi.py` & `deta-discord-interactions-0.1.1/deta_discord_interactions/tests/test_wsgi.py`

 * *Files identical despite different names*

### Comparing `deta-discord-interactions-0.1.0/deta_discord_interactions/utils/cooldown/__init__.py` & `deta-discord-interactions-0.1.1/deta_discord_interactions/utils/cooldown/__init__.py`

 * *Files identical despite different names*

### Comparing `deta-discord-interactions-0.1.0/deta_discord_interactions/utils/database/_local_base.py` & `deta-discord-interactions-0.1.1/deta_discord_interactions/utils/database/_local_base.py`

 * *Files identical despite different names*

### Comparing `deta-discord-interactions-0.1.0/deta_discord_interactions/utils/database/bound_meta.py` & `deta-discord-interactions-0.1.1/deta_discord_interactions/utils/database/bound_meta.py`

 * *Files identical despite different names*

### Comparing `deta-discord-interactions-0.1.0/deta_discord_interactions/utils/database/database.py` & `deta-discord-interactions-0.1.1/deta_discord_interactions/utils/database/database.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,35 +30,35 @@
         """Deta Base wrapper | ORM
         
         Parameters
         ----------
         name : str
             Which name to use for the Deta Base
         record_type : Type[LoadableDataclass]
-            User defined record model (must inherit LoadableDataclass)
-        base_mode: Optional[str], support values: "DETA_BASE", "MEMORY", "DISK"
+            Record model (must inherit LoadableDataclass)
+        base_mode: Optional[str], support values: "DETA", "MEMORY", "DISK"
             Which mode to use for the database.
-            DETA_BASE: Uses Deta Base
+            DETA: Uses Deta Base
             DISK: Saves the data to a local file instead of using Deta Base.
             MEMORY: Keep the data in memory but do not save at all.
-            By default, uses the `DETA_ORM_DATABASE_MODE` environment variable, or "DETA_BASE" if unset
+            By default, uses the `DETA_ORM_DATABASE_MODE` environment variable, or "DETA" if unset
         base_folder : str
             If using `base_mode = "DISK"`, you can use this to specify where the database should be stored.
             If missing, expects for the `DETA_ORM_FOLDER` environment variable to be set.
         """
         if base_mode is None:
-            base_mode = os.getenv("DETA_ORM_DATABASE_MODE", "DETA_BASE")
-        if base_mode == "DETA_BASE":
+            base_mode = os.getenv("DETA_ORM_DATABASE_MODE", "DETA")
+        if base_mode.startswith("DETA"):
             self.__base = Base(name)
         elif base_mode == "MEMORY":
             self.__base = LocalBase(name, sync_disk=False)
         elif base_mode == "DISK":
             self.__base = LocalBase(name, sync_disk=True, folder=base_folder)
         else:
-            raise Exception("Invalid value for DETA_ORM_DATABASE_MODE environment variable")
+            raise Exception("Invalid value for DETA_ORM_DATABASE_MODE")
 
         self._record_type = record_type
         self.__known_functions = {}
     
     def remember_function(self, function: Callable):
         """Use as a decorator to be able to save/load a function reference in LoadableDataclasses."""
         self.__known_functions[function.__name__] = function
```

### Comparing `deta-discord-interactions-0.1.0/deta_discord_interactions/utils/database/query.py` & `deta-discord-interactions-0.1.1/deta_discord_interactions/utils/database/query.py`

 * *Files identical despite different names*

### Comparing `deta-discord-interactions-0.1.0/deta_discord_interactions/utils/oauth/model.py` & `deta-discord-interactions-0.1.1/deta_discord_interactions/utils/oauth/model.py`

 * *Files identical despite different names*

### Comparing `deta-discord-interactions-0.1.0/deta_discord_interactions/utils/oauth/oauth.py` & `deta-discord-interactions-0.1.1/deta_discord_interactions/utils/oauth/oauth.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,19 @@
     pending_oauth: PendingOAuth
 
 
 pending_oauths = Database(name="_discord_interactions_pending_oauths", record_type=PendingRecord)
 remember_callback = pending_oauths.remember_function
 
 def enable_oauth(app: DiscordInteractions, /, *, path: str = "/oauth") -> None:
-    "Allows for the app to receive and process OAuth and create Webhooks"
+    """Allows for the app to receive and process OAuth and create Webhooks    
+
+    Usage:
+    `app = enable_oauth(app)`
+    """
     app.route(path)(_handle_oauth)
 
 
 class Callback(Protocol):
     "Just to make it easier to identifity the signature the callback must have"
     def __call__(self, token: Optional[OAuthToken], ctx: Context, *args, **kwargs) -> str: ...
```

### Comparing `deta-discord-interactions-0.1.0/deta_discord_interactions.egg-info/PKG-INFO` & `deta-discord-interactions-0.1.1/deta_discord_interactions.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deta-discord-interactions
-Version: 0.1.0
+Version: 0.1.1
 Summary: A web framework for Discord interactions specialized for usage in https://deta.sh
 Home-page: https://github.com/etrotta/flask-discord-interactions/tree/deta
 Author: etrotta
 Author-email: etrotta <etrotta@duck.com>
 License: MIT
 Project-URL: Homepage, https://github.com/etrotta/flask-discord-interactions/tree/deta
 Project-URL: Bug Tracker, https://github.com/etrotta/flask-discord-interactions/issues
@@ -27,7 +27,19 @@
 def ping(ctx):
     "Respond with a friendly 'pong'!"
     return "Pong!"
 ```
 
 The documentation of the original library is available on [readthedocs](https://flask-discord-interactions.readthedocs.io/).
 The documentation of the Fork is still Work in Progress.
+
+
+
+## Known issues
+- No good way to defer nor follow up (any spawned threads are killed as soon as the main function returns)
+- The Deta Space changes made it a quite few times more complicated to setup than Cloud used to be
+- Not particularly beginner friendly
+- Poorly documented
+
+## As far as security goes
+The `http.server` module of the standard library that `deta_discord_interactions.http` relies on is not recommended for production usage. Use it at your own risk.
+Any server that supports [PEP 3333](https://peps.python.org/pep-3333/) and works in serverless environments should work, so you may want to use something like https://gunicorn.org/ instead of the `deta_discord_interactions.http` used in Examples.
```

### Comparing `deta-discord-interactions-0.1.0/deta_discord_interactions.egg-info/SOURCES.txt` & `deta-discord-interactions-0.1.1/deta_discord_interactions.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -34,27 +34,30 @@
 deta_discord_interactions/models/utils.py
 deta_discord_interactions/tests/__init__.py
 deta_discord_interactions/tests/conftest.py
 deta_discord_interactions/tests/test_command.py
 deta_discord_interactions/tests/test_component.py
 deta_discord_interactions/tests/test_context.py
 deta_discord_interactions/tests/test_database.py
+deta_discord_interactions/tests/test_drive.py
 deta_discord_interactions/tests/test_handler.py
 deta_discord_interactions/tests/test_http.py
 deta_discord_interactions/tests/test_oauth.py
 deta_discord_interactions/tests/test_options.py
 deta_discord_interactions/tests/test_ping.py
 deta_discord_interactions/tests/test_register.py
 deta_discord_interactions/tests/test_response.py
 deta_discord_interactions/tests/test_subcommand.py
 deta_discord_interactions/tests/test_wsgi.py
 deta_discord_interactions/utils/__init__.py
 deta_discord_interactions/utils/cooldown/__init__.py
 deta_discord_interactions/utils/database/__init__.py
 deta_discord_interactions/utils/database/_local_base.py
+deta_discord_interactions/utils/database/_local_drive.py
 deta_discord_interactions/utils/database/bound_meta.py
 deta_discord_interactions/utils/database/database.py
+deta_discord_interactions/utils/database/drive.py
 deta_discord_interactions/utils/database/exceptions.py
 deta_discord_interactions/utils/database/query.py
 deta_discord_interactions/utils/oauth/__init__.py
 deta_discord_interactions/utils/oauth/model.py
 deta_discord_interactions/utils/oauth/oauth.py
```

### Comparing `deta-discord-interactions-0.1.0/pyproject.toml` & `deta-discord-interactions-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "deta-discord-interactions"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="etrotta", email="etrotta@duck.com" },
 ]
 description = "A web framework for Discord interactions specialized for usage in https://deta.sh"
 readme = "README.md"
 license = { text = "MIT" }
 requires-python = ">=3.9"
```

### Comparing `deta-discord-interactions-0.1.0/setup.py` & `deta-discord-interactions-0.1.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 with open("README.md") as file:
     readme = file.read()
 
 
 setup(
     name="Deta-Discord-Interactions",
-    version="0.1.0",
+    version="0.1.1",
     url="https://github.com/etrotta/flask-discord-interactions/tree/deta",
     author="etrotta",
     author_email="etrotta@duck.com",
     description="A web framework for Discord interactions specialized for deta.",
     long_description=readme,
     long_description_content_type="text/markdown",
     packages=find_packages(),
```

