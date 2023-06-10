# Comparing `tmp/irails-1.3.39.tar.gz` & `tmp/irails-1.3.40.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "irails-1.3.39.tar", last modified: Wed Jun  7 14:00:27 2023, max compression
+gzip compressed data, was "irails-1.3.40.tar", last modified: Sat Jun 10 07:22:56 2023, max compression
```

## Comparing `irails-1.3.39.tar` & `irails-1.3.40.tar`

### file list

```diff
@@ -1,105 +1,106 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 14:00:27.244583 irails-1.3.39/
--rw-rw-rw-   0        0        0       83 2023-05-04 04:10:30.000000 irails-1.3.39/MANIFEST.in
--rw-rw-rw-   0        0        0     4979 2023-06-07 14:00:27.242588 irails-1.3.39/PKG-INFO
--rw-rw-rw-   0        0        0     4174 2023-05-27 12:12:58.000000 irails-1.3.39/README.md
-drwxrwxrwx   0        0        0        0 2023-06-07 14:00:27.094717 irails-1.3.39/irails/
--rw-rw-rw-   0        0        0      307 2023-06-07 13:59:55.000000 irails-1.3.39/irails/__init__.py
--rw-rw-rw-   0        0        0     7048 2023-06-07 13:53:06.000000 irails-1.3.39/irails/_i18n.py
--rw-rw-rw-   0        0        0     4450 2023-06-01 06:04:06.000000 irails-1.3.39/irails/_loader.py
--rw-rw-rw-   0        0        0     6271 2023-06-06 11:58:47.000000 irails-1.3.39/irails/_utils.py
--rw-rw-rw-   0        0        0    15361 2023-06-07 11:59:43.000000 irails-1.3.39/irails/auth.py
--rw-rw-rw-   0        0        0    13554 2023-06-07 13:24:34.000000 irails-1.3.39/irails/base_controller.py
-drwxrwxrwx   0        0        0        0 2023-06-07 14:00:27.102690 irails-1.3.39/irails/casbin_adapters/
-drwxrwxrwx   0        0        0        0 2023-06-07 14:00:27.104683 irails-1.3.39/irails/casbin_adapters/__pycache__/
--rw-rw-rw-   0        0        0     9337 2023-05-31 14:37:50.000000 irails-1.3.39/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-310.pyc
--rw-rw-rw-   0        0        0    17834 2023-04-30 14:29:09.000000 irails-1.3.39/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc
--rw-rw-rw-   0        0        0    10665 2023-05-31 14:37:46.000000 irails-1.3.39/irails/casbin_adapters/sqlalchemy_adapter.py
--rw-rw-rw-   0        0        0     4381 2023-02-25 09:43:32.000000 irails-1.3.39/irails/cbv.py
--rw-rw-rw-   0        0        0     6357 2023-05-25 10:46:48.000000 irails-1.3.39/irails/config.py
--rw-rw-rw-   0        0        0    13203 2023-05-26 14:20:32.000000 irails-1.3.39/irails/controller_utils.py
--rw-rw-rw-   0        0        0    26975 2023-06-06 12:15:32.000000 irails-1.3.39/irails/core.py
--rw-rw-rw-   0        0        0    21544 2023-06-06 12:23:20.000000 irails-1.3.39/irails/database.py
--rw-rw-rw-   0        0        0     1592 2023-05-25 14:19:01.000000 irails-1.3.39/irails/log.py
--rw-rw-rw-   0        0        0     8910 2023-06-05 12:15:01.000000 irails-1.3.39/irails/midware.py
--rw-rw-rw-   0        0        0     9175 2023-06-01 06:44:57.000000 irails-1.3.39/irails/midware_session.py
--rw-rw-rw-   0        0        0     4336 2023-06-01 06:22:43.000000 irails-1.3.39/irails/mvc_router.py
-drwxrwxrwx   0        0        0        0 2023-06-07 14:00:27.116530 irails-1.3.39/irails/scripts/
--rw-rw-rw-   0        0        0        0 2023-04-26 07:44:41.000000 irails-1.3.39/irails/scripts/__init__.py
--rw-rw-rw-   0        0        0     7862 2023-05-13 15:04:27.000000 irails-1.3.39/irails/scripts/_app.py
--rw-rw-rw-   0        0        0     6892 2023-05-19 07:21:20.000000 irails-1.3.39/irails/scripts/_controller.py
--rw-rw-rw-   0        0        0     7763 2023-05-21 13:57:03.000000 irails-1.3.39/irails/scripts/_i18n.py
--rw-rw-rw-   0        0        0     1332 2023-05-21 08:39:33.000000 irails-1.3.39/irails/scripts/_migrate.py
--rw-rw-rw-   0        0        0     3774 2023-05-14 13:34:33.000000 irails-1.3.39/irails/scripts/_model.py
--rw-rw-rw-   0        0        0     2301 2023-05-03 14:35:33.000000 irails-1.3.39/irails/scripts/_project.py
--rw-rw-rw-   0        0        0     1399 2023-05-26 14:27:13.000000 irails-1.3.39/irails/scripts/_run.py
--rw-rw-rw-   0        0        0     2288 2023-05-11 14:15:32.000000 irails-1.3.39/irails/scripts/_shell.py
--rw-rw-rw-   0        0        0     5750 2023-05-29 06:31:52.000000 irails-1.3.39/irails/scripts/_test.py
--rw-rw-rw-   0        0        0     2900 2023-05-21 08:16:21.000000 irails-1.3.39/irails/scripts/main.py
-drwxrwxrwx   0        0        0        0 2023-06-07 14:00:27.066143 irails-1.3.39/irails/scripts/tpls/
-drwxrwxrwx   0        0        0        0 2023-06-07 14:00:27.128502 irails-1.3.39/irails/scripts/tpls/app/
--rw-rw-rw-   0        0        0      223 2023-05-09 15:18:47.000000 irails-1.3.39/irails/scripts/tpls/app/controller.tpl
--rw-rw-rw-   0        0        0        0 2023-04-28 06:03:05.000000 irails-1.3.39/irails/scripts/tpls/app/css.tpl
--rw-rw-rw-   0        0        0      791 2023-04-25 10:42:10.000000 irails-1.3.39/irails/scripts/tpls/app/home.css.tpl
--rw-rw-rw-   0        0        0     1293 2023-05-05 10:16:42.000000 irails-1.3.39/irails/scripts/tpls/app/home.tpl
--rw-rw-rw-   0        0        0     1023 2023-05-19 12:27:03.000000 irails-1.3.39/irails/scripts/tpls/app/model.jinja
--rw-rw-rw-   0        0        0      197 2023-05-24 11:06:24.000000 irails-1.3.39/irails/scripts/tpls/app/service.jinja
--rw-rw-rw-   0        0        0      237 2023-05-13 13:54:20.000000 irails-1.3.39/irails/scripts/tpls/app/test_controller.jinja
--rw-rw-rw-   0        0        0      908 2023-05-24 14:14:47.000000 irails-1.3.39/irails/scripts/tpls/app/test_service.jinja
--rw-rw-rw-   0        0        0       18 2023-05-02 08:56:04.000000 irails-1.3.39/irails/scripts/tpls/app/view.tpl
-drwxrwxrwx   0        0        0        0 2023-06-07 14:00:27.130492 irails-1.3.39/irails/scripts/tpls/project/
--rw-rw-rw-   0        0        0      139 2023-04-23 09:46:24.000000 irails-1.3.39/irails/scripts/tpls/project/.gitignore
-drwxrwxrwx   0        0        0        0 2023-06-07 14:00:27.131491 irails-1.3.39/irails/scripts/tpls/project/apps/
--rw-rw-rw-   0        0        0        0 2023-04-26 09:58:51.000000 irails-1.3.39/irails/scripts/tpls/project/apps/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-07 14:00:27.186344 irails-1.3.39/irails/scripts/tpls/project/configs/
--rw-rw-rw-   0        0        0      746 2023-05-09 06:45:34.000000 irails-1.3.39/irails/scripts/tpls/project/configs/alembic.ini
--rw-rw-rw-   0        0        0      323 2023-05-30 07:17:46.000000 irails-1.3.39/irails/scripts/tpls/project/configs/authencation.yaml
--rw-rw-rw-   0        0        0        0 2023-03-06 08:27:07.000000 irails-1.3.39/irails/scripts/tpls/project/configs/cache.yaml
--rw-rw-rw-   0        0        0      104 2023-05-04 05:06:32.000000 irails-1.3.39/irails/scripts/tpls/project/configs/casbin-adapter.csv
--rw-rw-rw-   0        0        0      302 2023-05-04 05:24:51.000000 irails-1.3.39/irails/scripts/tpls/project/configs/casbin-model.conf
-drwxrwxrwx   0        0        0        0 2023-06-07 14:00:27.202301 irails-1.3.39/irails/scripts/tpls/project/configs/casbin_templates/
--rw-rw-rw-   0        0        0      204 2023-05-18 07:46:03.000000 irails-1.3.39/irails/scripts/tpls/project/configs/casbin_templates/ALC.conf
--rw-rw-rw-   0        0        0       37 2023-05-18 07:46:03.000000 irails-1.3.39/irails/scripts/tpls/project/configs/casbin_templates/ALC.csv
--rw-rw-rw-   0        0        0      236 2023-05-18 07:46:03.000000 irails-1.3.39/irails/scripts/tpls/project/configs/casbin_templates/RBAC.conf
--rw-rw-rw-   0        0        0      125 2023-05-18 07:46:03.000000 irails-1.3.39/irails/scripts/tpls/project/configs/casbin_templates/RBAC.csv
--rw-rw-rw-   0        0        0      249 2023-05-18 07:46:03.000000 irails-1.3.39/irails/scripts/tpls/project/configs/casbin_templates/RBACR.conf
--rw-rw-rw-   0        0        0      159 2023-05-18 07:46:03.000000 irails-1.3.39/irails/scripts/tpls/project/configs/casbin_templates/RBACR.csv
--rw-rw-rw-   0        0        0      319 2023-05-29 12:26:50.000000 irails-1.3.39/irails/scripts/tpls/project/configs/casbin_templates/RBACT.conf
--rw-rw-rw-   0        0        0      178 2023-05-18 07:46:03.000000 irails-1.3.39/irails/scripts/tpls/project/configs/casbin_templates/RBACT.csv
--rw-rw-rw-   0        0        0      222 2023-05-18 07:46:03.000000 irails-1.3.39/irails/scripts/tpls/project/configs/casbin_templates/RESTFUL.conf
--rw-rw-rw-   0        0        0      152 2023-05-18 07:46:03.000000 irails-1.3.39/irails/scripts/tpls/project/configs/casbin_templates/RESTFUL.csv
--rw-rw-rw-   0        0        0      817 2023-05-10 10:45:36.000000 irails-1.3.39/irails/scripts/tpls/project/configs/database.yaml
--rw-rw-rw-   0        0        0      748 2023-05-11 05:35:06.000000 irails-1.3.39/irails/scripts/tpls/project/configs/general.yaml
--rw-rw-rw-   0        0        0      337 2023-04-22 10:54:12.000000 irails-1.3.39/irails/scripts/tpls/project/configs/session.yaml
--rw-rw-rw-   0        0        0      272 2023-05-09 06:44:59.000000 irails-1.3.39/irails/scripts/tpls/project/configs/upload.yaml
-drwxrwxrwx   0        0        0        0 2023-06-07 14:00:27.069121 irails-1.3.39/irails/scripts/tpls/project/data/
-drwxrwxrwx   0        0        0        0 2023-06-07 14:00:27.208286 irails-1.3.39/irails/scripts/tpls/project/data/alembic/
--rw-rw-rw-   0        0        0       38 2023-04-09 12:01:20.000000 irails-1.3.39/irails/scripts/tpls/project/data/alembic/README
--rw-rw-rw-   0        0        0     2144 2023-04-30 09:03:04.000000 irails-1.3.39/irails/scripts/tpls/project/data/alembic/env.py
--rw-rw-rw-   0        0        0      510 2023-04-09 12:01:20.000000 irails-1.3.39/irails/scripts/tpls/project/data/alembic/script.py.mako
--rw-rw-rw-   0        0        0      231 2023-05-11 15:42:13.000000 irails-1.3.39/irails/scripts/tpls/project/main.py
-drwxrwxrwx   0        0        0        0 2023-06-07 14:00:27.214269 irails-1.3.39/irails/scripts/tpls/project/public/
--rw-rw-rw-   0        0        0     1233 2023-05-02 08:46:22.000000 irails-1.3.39/irails/scripts/tpls/project/public/error_404.html
--rw-rw-rw-   0        0        0     1083 2023-05-02 08:46:46.000000 irails-1.3.39/irails/scripts/tpls/project/public/error_500.html
-drwxrwxrwx   0        0        0        0 2023-06-07 14:00:27.218260 irails-1.3.39/irails/scripts/tpls/project/public/libs/
-drwxrwxrwx   0        0        0        0 2023-06-07 14:00:27.071117 irails-1.3.39/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/
-drwxrwxrwx   0        0        0        0 2023-06-07 14:00:27.226709 irails-1.3.39/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/
--rw-rw-rw-   0        0        0  1970121 2023-04-23 08:02:36.000000 irails-1.3.39/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js
-drwxrwxrwx   0        0        0        0 2023-06-07 14:00:27.235109 irails-1.3.39/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/
--rw-rw-rw-   0        0        0   323666 2023-04-23 08:04:13.000000 irails-1.3.39/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css
--rw-rw-rw-   0        0        0      725 2023-04-21 12:39:53.000000 irails-1.3.39/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js
--rw-rw-rw-   0        0        0  1441055 2023-04-21 07:36:37.000000 irails-1.3.39/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js
-drwxrwxrwx   0        0        0        0 2023-06-07 14:00:27.072115 irails-1.3.39/irails/scripts/tpls/project/public/vue@3.2.36/
-drwxrwxrwx   0        0        0        0 2023-06-07 14:00:27.237998 irails-1.3.39/irails/scripts/tpls/project/public/vue@3.2.36/dist/
--rw-rw-rw-   0        0        0   640610 2023-04-21 07:36:07.000000 irails-1.3.39/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js
--rw-rw-rw-   0        0        0     1048 2023-05-30 07:13:21.000000 irails-1.3.39/irails/scripts/tpls/project/public/vue_home.html
--rw-rw-rw-   0        0        0     1731 2023-05-29 05:12:03.000000 irails-1.3.39/irails/unit_test.py
--rw-rw-rw-   0        0        0     3053 2023-05-30 07:10:08.000000 irails-1.3.39/irails/view.py
-drwxrwxrwx   0        0        0        0 2023-06-07 14:00:27.100693 irails-1.3.39/irails.egg-info/
--rw-rw-rw-   0        0        0     4979 2023-06-07 14:00:26.000000 irails-1.3.39/irails.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3209 2023-06-07 14:00:27.000000 irails-1.3.39/irails.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 14:00:26.000000 irails-1.3.39/irails.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2023-06-07 14:00:26.000000 irails-1.3.39/irails.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      367 2023-06-07 14:00:26.000000 irails-1.3.39/irails.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-07 14:00:26.000000 irails-1.3.39/irails.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-07 14:00:27.244583 irails-1.3.39/setup.cfg
--rw-rw-rw-   0        0        0     2551 2023-05-09 11:27:27.000000 irails-1.3.39/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-10 07:22:56.714215 irails-1.3.40/
+-rw-rw-rw-   0        0        0       83 2023-05-04 04:10:30.000000 irails-1.3.40/MANIFEST.in
+-rw-rw-rw-   0        0        0     4956 2023-06-10 07:22:56.713219 irails-1.3.40/PKG-INFO
+-rw-rw-rw-   0        0        0     4174 2023-05-27 12:12:58.000000 irails-1.3.40/README.md
+drwxrwxrwx   0        0        0        0 2023-06-10 07:22:56.619320 irails-1.3.40/irails/
+-rw-rw-rw-   0        0        0      327 2023-06-10 07:22:51.000000 irails-1.3.40/irails/__init__.py
+-rw-rw-rw-   0        0        0     7048 2023-06-07 13:53:06.000000 irails-1.3.40/irails/_i18n.py
+-rw-rw-rw-   0        0        0     6804 2023-06-10 06:57:35.000000 irails-1.3.40/irails/_loader.py
+-rw-rw-rw-   0        0        0     8782 2023-06-10 07:10:22.000000 irails-1.3.40/irails/_utils.py
+-rw-rw-rw-   0        0        0    15361 2023-06-07 11:59:43.000000 irails-1.3.40/irails/auth.py
+-rw-rw-rw-   0        0        0    13740 2023-06-09 06:23:19.000000 irails-1.3.40/irails/base_controller.py
+drwxrwxrwx   0        0        0        0 2023-06-10 07:22:56.632076 irails-1.3.40/irails/casbin_adapters/
+drwxrwxrwx   0        0        0        0 2023-06-10 07:22:56.635068 irails-1.3.40/irails/casbin_adapters/__pycache__/
+-rw-rw-rw-   0        0        0     9337 2023-05-31 14:37:50.000000 irails-1.3.40/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-310.pyc
+-rw-rw-rw-   0        0        0    17834 2023-04-30 14:29:09.000000 irails-1.3.40/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc
+-rw-rw-rw-   0        0        0    10665 2023-05-31 14:37:46.000000 irails-1.3.40/irails/casbin_adapters/sqlalchemy_adapter.py
+-rw-rw-rw-   0        0        0     4381 2023-02-25 09:43:32.000000 irails-1.3.40/irails/cbv.py
+-rw-rw-rw-   0        0        0     6357 2023-05-25 10:46:48.000000 irails-1.3.40/irails/config.py
+-rw-rw-rw-   0        0        0    13203 2023-05-26 14:20:32.000000 irails-1.3.40/irails/controller_utils.py
+-rw-rw-rw-   0        0        0    27348 2023-06-09 14:14:08.000000 irails-1.3.40/irails/core.py
+-rw-rw-rw-   0        0        0    21544 2023-06-06 12:23:20.000000 irails-1.3.40/irails/database.py
+-rw-rw-rw-   0        0        0     1592 2023-05-25 14:19:01.000000 irails-1.3.40/irails/log.py
+-rw-rw-rw-   0        0        0     9284 2023-06-09 13:46:46.000000 irails-1.3.40/irails/midware.py
+-rw-rw-rw-   0        0        0     9175 2023-06-01 06:44:57.000000 irails-1.3.40/irails/midware_session.py
+-rw-rw-rw-   0        0        0     4336 2023-06-01 06:22:43.000000 irails-1.3.40/irails/mvc_router.py
+drwxrwxrwx   0        0        0        0 2023-06-10 07:22:56.647394 irails-1.3.40/irails/scripts/
+-rw-rw-rw-   0        0        0        0 2023-04-26 07:44:41.000000 irails-1.3.40/irails/scripts/__init__.py
+-rw-rw-rw-   0        0        0     7278 2023-06-10 07:10:17.000000 irails-1.3.40/irails/scripts/_app.py
+-rw-rw-rw-   0        0        0     7095 2023-06-09 07:51:49.000000 irails-1.3.40/irails/scripts/_controller.py
+-rw-rw-rw-   0        0        0     7763 2023-05-21 13:57:03.000000 irails-1.3.40/irails/scripts/_i18n.py
+-rw-rw-rw-   0        0        0     1336 2023-06-09 05:34:08.000000 irails-1.3.40/irails/scripts/_migrate.py
+-rw-rw-rw-   0        0        0     4080 2023-06-09 08:02:27.000000 irails-1.3.40/irails/scripts/_model.py
+-rw-rw-rw-   0        0        0     2301 2023-05-03 14:35:33.000000 irails-1.3.40/irails/scripts/_project.py
+-rw-rw-rw-   0        0        0     1399 2023-05-26 14:27:13.000000 irails-1.3.40/irails/scripts/_run.py
+-rw-rw-rw-   0        0        0     2288 2023-05-11 14:15:32.000000 irails-1.3.40/irails/scripts/_shell.py
+-rw-rw-rw-   0        0        0     5765 2023-06-09 05:34:08.000000 irails-1.3.40/irails/scripts/_test.py
+-rw-rw-rw-   0        0        0     2900 2023-05-21 08:16:21.000000 irails-1.3.40/irails/scripts/main.py
+drwxrwxrwx   0        0        0        0 2023-06-10 07:22:56.545516 irails-1.3.40/irails/scripts/tpls/
+drwxrwxrwx   0        0        0        0 2023-06-10 07:22:56.660359 irails-1.3.40/irails/scripts/tpls/app/
+-rw-rw-rw-   0        0        0      223 2023-05-09 15:18:47.000000 irails-1.3.40/irails/scripts/tpls/app/controller.tpl
+-rw-rw-rw-   0        0        0        0 2023-04-28 06:03:05.000000 irails-1.3.40/irails/scripts/tpls/app/css.tpl
+-rw-rw-rw-   0        0        0      791 2023-04-25 10:42:10.000000 irails-1.3.40/irails/scripts/tpls/app/home.css.tpl
+-rw-rw-rw-   0        0        0     1293 2023-05-05 10:16:42.000000 irails-1.3.40/irails/scripts/tpls/app/home.tpl
+-rw-rw-rw-   0        0        0      179 2023-06-09 07:16:16.000000 irails-1.3.40/irails/scripts/tpls/app/manifest.jinja
+-rw-rw-rw-   0        0        0      999 2023-06-09 05:47:40.000000 irails-1.3.40/irails/scripts/tpls/app/model.jinja
+-rw-rw-rw-   0        0        0      197 2023-05-24 11:06:24.000000 irails-1.3.40/irails/scripts/tpls/app/service.jinja
+-rw-rw-rw-   0        0        0      237 2023-05-13 13:54:20.000000 irails-1.3.40/irails/scripts/tpls/app/test_controller.jinja
+-rw-rw-rw-   0        0        0      908 2023-05-24 14:14:47.000000 irails-1.3.40/irails/scripts/tpls/app/test_service.jinja
+-rw-rw-rw-   0        0        0       18 2023-05-02 08:56:04.000000 irails-1.3.40/irails/scripts/tpls/app/view.tpl
+drwxrwxrwx   0        0        0        0 2023-06-10 07:22:56.662353 irails-1.3.40/irails/scripts/tpls/project/
+-rw-rw-rw-   0        0        0      139 2023-04-23 09:46:24.000000 irails-1.3.40/irails/scripts/tpls/project/.gitignore
+drwxrwxrwx   0        0        0        0 2023-06-10 07:22:56.663351 irails-1.3.40/irails/scripts/tpls/project/apps/
+-rw-rw-rw-   0        0        0        0 2023-04-26 09:58:51.000000 irails-1.3.40/irails/scripts/tpls/project/apps/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-10 07:22:56.677315 irails-1.3.40/irails/scripts/tpls/project/configs/
+-rw-rw-rw-   0        0        0      746 2023-05-09 06:45:34.000000 irails-1.3.40/irails/scripts/tpls/project/configs/alembic.ini
+-rw-rw-rw-   0        0        0      323 2023-05-30 07:17:46.000000 irails-1.3.40/irails/scripts/tpls/project/configs/authencation.yaml
+-rw-rw-rw-   0        0        0        0 2023-03-06 08:27:07.000000 irails-1.3.40/irails/scripts/tpls/project/configs/cache.yaml
+-rw-rw-rw-   0        0        0      104 2023-05-04 05:06:32.000000 irails-1.3.40/irails/scripts/tpls/project/configs/casbin-adapter.csv
+-rw-rw-rw-   0        0        0      302 2023-05-04 05:24:51.000000 irails-1.3.40/irails/scripts/tpls/project/configs/casbin-model.conf
+drwxrwxrwx   0        0        0        0 2023-06-10 07:22:56.690279 irails-1.3.40/irails/scripts/tpls/project/configs/casbin_templates/
+-rw-rw-rw-   0        0        0      204 2023-05-18 07:46:03.000000 irails-1.3.40/irails/scripts/tpls/project/configs/casbin_templates/ALC.conf
+-rw-rw-rw-   0        0        0       37 2023-05-18 07:46:03.000000 irails-1.3.40/irails/scripts/tpls/project/configs/casbin_templates/ALC.csv
+-rw-rw-rw-   0        0        0      236 2023-05-18 07:46:03.000000 irails-1.3.40/irails/scripts/tpls/project/configs/casbin_templates/RBAC.conf
+-rw-rw-rw-   0        0        0      125 2023-05-18 07:46:03.000000 irails-1.3.40/irails/scripts/tpls/project/configs/casbin_templates/RBAC.csv
+-rw-rw-rw-   0        0        0      249 2023-05-18 07:46:03.000000 irails-1.3.40/irails/scripts/tpls/project/configs/casbin_templates/RBACR.conf
+-rw-rw-rw-   0        0        0      159 2023-05-18 07:46:03.000000 irails-1.3.40/irails/scripts/tpls/project/configs/casbin_templates/RBACR.csv
+-rw-rw-rw-   0        0        0      319 2023-05-29 12:26:50.000000 irails-1.3.40/irails/scripts/tpls/project/configs/casbin_templates/RBACT.conf
+-rw-rw-rw-   0        0        0      178 2023-05-18 07:46:03.000000 irails-1.3.40/irails/scripts/tpls/project/configs/casbin_templates/RBACT.csv
+-rw-rw-rw-   0        0        0      222 2023-05-18 07:46:03.000000 irails-1.3.40/irails/scripts/tpls/project/configs/casbin_templates/RESTFUL.conf
+-rw-rw-rw-   0        0        0      152 2023-05-18 07:46:03.000000 irails-1.3.40/irails/scripts/tpls/project/configs/casbin_templates/RESTFUL.csv
+-rw-rw-rw-   0        0        0      817 2023-05-10 10:45:36.000000 irails-1.3.40/irails/scripts/tpls/project/configs/database.yaml
+-rw-rw-rw-   0        0        0      748 2023-05-11 05:35:06.000000 irails-1.3.40/irails/scripts/tpls/project/configs/general.yaml
+-rw-rw-rw-   0        0        0      337 2023-04-22 10:54:12.000000 irails-1.3.40/irails/scripts/tpls/project/configs/session.yaml
+-rw-rw-rw-   0        0        0      272 2023-05-09 06:44:59.000000 irails-1.3.40/irails/scripts/tpls/project/configs/upload.yaml
+drwxrwxrwx   0        0        0        0 2023-06-10 07:22:56.549506 irails-1.3.40/irails/scripts/tpls/project/data/
+drwxrwxrwx   0        0        0        0 2023-06-10 07:22:56.694269 irails-1.3.40/irails/scripts/tpls/project/data/alembic/
+-rw-rw-rw-   0        0        0       38 2023-04-09 12:01:20.000000 irails-1.3.40/irails/scripts/tpls/project/data/alembic/README
+-rw-rw-rw-   0        0        0     2144 2023-04-30 09:03:04.000000 irails-1.3.40/irails/scripts/tpls/project/data/alembic/env.py
+-rw-rw-rw-   0        0        0      510 2023-04-09 12:01:20.000000 irails-1.3.40/irails/scripts/tpls/project/data/alembic/script.py.mako
+-rw-rw-rw-   0        0        0      231 2023-05-11 15:42:13.000000 irails-1.3.40/irails/scripts/tpls/project/main.py
+drwxrwxrwx   0        0        0        0 2023-06-10 07:22:56.698257 irails-1.3.40/irails/scripts/tpls/project/public/
+-rw-rw-rw-   0        0        0     1233 2023-05-02 08:46:22.000000 irails-1.3.40/irails/scripts/tpls/project/public/error_404.html
+-rw-rw-rw-   0        0        0     1083 2023-05-02 08:46:46.000000 irails-1.3.40/irails/scripts/tpls/project/public/error_500.html
+drwxrwxrwx   0        0        0        0 2023-06-10 07:22:56.700253 irails-1.3.40/irails/scripts/tpls/project/public/libs/
+drwxrwxrwx   0        0        0        0 2023-06-10 07:22:56.552498 irails-1.3.40/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/
+drwxrwxrwx   0        0        0        0 2023-06-10 07:22:56.705238 irails-1.3.40/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/
+-rw-rw-rw-   0        0        0  1970121 2023-04-23 08:02:36.000000 irails-1.3.40/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js
+drwxrwxrwx   0        0        0        0 2023-06-10 07:22:56.708230 irails-1.3.40/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/
+-rw-rw-rw-   0        0        0   323666 2023-04-23 08:04:13.000000 irails-1.3.40/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css
+-rw-rw-rw-   0        0        0      725 2023-04-21 12:39:53.000000 irails-1.3.40/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js
+-rw-rw-rw-   0        0        0  1441055 2023-04-21 07:36:37.000000 irails-1.3.40/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js
+drwxrwxrwx   0        0        0        0 2023-06-10 07:22:56.553496 irails-1.3.40/irails/scripts/tpls/project/public/vue@3.2.36/
+drwxrwxrwx   0        0        0        0 2023-06-10 07:22:56.710225 irails-1.3.40/irails/scripts/tpls/project/public/vue@3.2.36/dist/
+-rw-rw-rw-   0        0        0   640610 2023-04-21 07:36:07.000000 irails-1.3.40/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js
+-rw-rw-rw-   0        0        0     1048 2023-05-30 07:13:21.000000 irails-1.3.40/irails/scripts/tpls/project/public/vue_home.html
+-rw-rw-rw-   0        0        0     1733 2023-06-09 05:34:08.000000 irails-1.3.40/irails/unit_test.py
+-rw-rw-rw-   0        0        0     3053 2023-05-30 07:10:08.000000 irails-1.3.40/irails/view.py
+drwxrwxrwx   0        0        0        0 2023-06-10 07:22:56.630079 irails-1.3.40/irails.egg-info/
+-rw-rw-rw-   0        0        0     4956 2023-06-10 07:22:56.000000 irails-1.3.40/irails.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3248 2023-06-10 07:22:56.000000 irails-1.3.40/irails.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-10 07:22:56.000000 irails-1.3.40/irails.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-06-10 07:22:56.000000 irails-1.3.40/irails.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      367 2023-06-10 07:22:56.000000 irails-1.3.40/irails.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-10 07:22:56.000000 irails-1.3.40/irails.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-10 07:22:56.714215 irails-1.3.40/setup.cfg
+-rw-rw-rw-   0        0        0     2551 2023-05-09 11:27:27.000000 irails-1.3.40/setup.py
```

### Comparing `irails-1.3.39/PKG-INFO` & `irails-1.3.40/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: irails
-Version: 1.3.39
+Version: 1.3.40
 Summary: Simple and elegant use of FastApi in MVC mode
 Home-page: https://github.com/smjkzsl/irails
 Author: Bruce chou
 Author-email: smjkzsl@gmail.com
 License: Apache License 2.0
 Keywords: web framework,mvc framework,fastapi framework
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -84,9 +83,7 @@
     +---uploads                             ## Others dir(if your need or not)
 ```
 ## Extras commands
 * `irails i18n gettext`  --generate i18n in irails app dir
 * `irails shell`         --run python interpreter with buildin support contexts 
 * `irails test`          --run project tests 
 * `irails migrate`       --run database migrations
-
-
```

### Comparing `irails-1.3.39/README.md` & `irails-1.3.40/README.md`

 * *Files identical despite different names*

### Comparing `irails-1.3.39/irails/_i18n.py` & `irails-1.3.40/irails/_i18n.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.39/irails/auth.py` & `irails-1.3.40/irails/auth.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.39/irails/base_controller.py` & `irails-1.3.40/irails/base_controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from fastapi.responses import RedirectResponse,HTMLResponse,PlainTextResponse
 from .view import _View
 from ._utils import get_controller_name,get_snaked_name
 from .config import config,ROOT_PATH
 from .log import _log
 import os,uuid
 from hashlib import md5
-from typing import Dict
+from typing import Dict, Type
 from logging import Logger
 import inspect
 import datetime
 from irails._i18n import load_app_translations,_
 
 __session_config = config.get('session') 
 _session_key = "session_id"
@@ -108,23 +108,29 @@
     @property
     def response(self)->Response :
         return self._response
     def __getitem__(self,key):
         """
             return the request param by name
         """
-        return self.get_param(key) 
-    def get_param(self,key):
+        return self.params(key) 
+    def params(self,key,defalut=None,value_type:Type=str):
+        v = defalut
         if key in self._form:
-            return self._form[key]
+            v = self._form[key]
         if key in self._json:
-            return self._json[key]
+            v = self._json[key]
         if key in self._query:
-            return self._query[key]
-        return None 
+            v = self._query[key]
+        if value_type:
+            v=value_type(v)
+        elif defalut:
+            value_type = type(defalut)
+            v=value_type(v)
+        return v
      
     @property
     def session(self)->Dict:
         """
             the session object
         """
         return self._session
```

### Comparing `irails-1.3.39/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-310.pyc` & `irails-1.3.40/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `irails-1.3.39/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc` & `irails-1.3.40/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `irails-1.3.39/irails/casbin_adapters/sqlalchemy_adapter.py` & `irails-1.3.40/irails/casbin_adapters/sqlalchemy_adapter.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.39/irails/cbv.py` & `irails-1.3.40/irails/cbv.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.39/irails/config.py` & `irails-1.3.40/irails/config.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.39/irails/controller_utils.py` & `irails-1.3.40/irails/controller_utils.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.39/irails/core.py` & `irails-1.3.40/irails/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from .mvc_router import create_controller, Api as api,   register_controllers_to_app
 from .controller_utils import AUTH_KEY, DEFAULT_KEY,  get_docs
 from .config import config, ROOT_PATH, _project_name
 from .log import _log
 from . import midware
 from . import auth
 from . import database
-from ._loader import _load_apps
+from ._loader import collect_apps
 from ._utils import get_controller_name, get_snaked_name, copy_attr, singleton, add_redirect_param
 from ._i18n import _
 
 __is_debug = config.get('debug', False)
 auto_refresh_token = config.get("session").get('auto_refresh_token', True)
 
 
@@ -271,14 +271,17 @@
     def _wapper(targetController):
         _controller_hash = app_dir.replace(os.sep, ".").lstrip(
             ".") + "." + targetController.__name__ + "@" + version
 
         if not app_name in application.apps:
             application.apps[app_name] = {'routes': {}, 'view_dirs': {}}
 
+        if not 'app_dir' in application.apps[app_name]:
+            application.apps[app_name]['app_dir'] = abs_path
+
         if not _controller_hash in application.apps[app_name]['routes']:
             application.apps[app_name]['routes'][_controller_hash] = {
                 'label': 'new', 'obj': _controllerBase}
 
         class puppetController(targetController, _controllerBase):
             '''puppet class inherited by the User defined controller class '''
 
@@ -387,15 +390,17 @@
 
         # for generate url_for function
         url_path = path
         controller_path_name = get_snaked_name(
             get_controller_name(targetController.__name__))
         _view_url_path: str = url_path.replace(
             "{controller}", controller_path_name).replace("{version}", version)
-
+        if not _view_url_path:
+            _view_url_path = f"/{controller_path_name}"
+            
         controller_current_view_path = abs_path + '/views/' + controller_path_name
         if version:
             controller_current_view_path += '/' + version
         setattr(puppetController, "__view_url__", _view_url_path)
         if 'default' in allargs:
             default_method = allargs['default']
             setattr(targetController, DEFAULT_KEY, default_method)
@@ -419,23 +424,24 @@
         ret = getattr(ret, '__wrapped__')
     return ret
 
 
 def _register_controllers():
     global __is_debug
     controller_count = 0
+    is_startup = True
     for app_name in application.apps:
         for hash, dict_obj in application.apps[app_name]['routes'].items():
             controller_count += 1
             if dict_obj['label'] == 'new':
                 if __is_debug:
                     _log.info(hash+" mountting...")
                 app_router = register_controllers_to_app(
                     application, dict_obj['obj'])
-
+                
                 application.apps[app_name]['router'] = app_router
                 dict_obj['label'] = 'mounted'
 
                 for r in app_router.routes:
                     funcname = str(r.endpoint).split(
                         '<function ')[1].split(" at ")[0]
                     end_point_abs = get_wrapped_endpoint(r.endpoint)
@@ -449,20 +455,24 @@
                         methods = r.name
                     if __is_debug:
                         _log.info((str(methods), r.path, funcname))
                     if not 'route_map' in application.apps[app_name]:
                         application.apps[app_name]['route_map'] = {}
                     application.apps[app_name]['route_map'][funcname] = {
                         'path': r.path, 'methods': methods, 'doc': doc_map, 'auth': auth_type, "endpoint": r.endpoint}
+            elif dict_obj['label'] != 'new':
+                is_startup = False
 
     if not (controller_count) > 0:
         raise RuntimeError(_("not found any controller class"))
 
     _log.info(_("static files mouting..."))
-    midware.init(app=application, debug=__is_debug)
+
+    if is_startup:
+        midware.init(app=application, debug=__is_debug)
 
 
 def check_db_migrate():
     db_cfg = config.get("database")
     if not db_cfg:
         return
     if __is_debug:
@@ -505,15 +515,15 @@
 
 def generate_mvc_app():
     global __is_debug
 
     application.title = _project_name
 
     _log.info(_("loading irails apps..."))
-    loaded, unloaded = _load_apps(debug=__is_debug, application=application)
+    loaded, unloaded = collect_apps(debug=__is_debug, application=application)
 
     _log.info(_('Load Apps Completed,%s loaded,%s unloaded') %
               (loaded, unloaded))
 
     _register_controllers()
 
     _log.info(_("checking database configure..."))
```

### Comparing `irails-1.3.39/irails/database.py` & `irails-1.3.40/irails/database.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.39/irails/log.py` & `irails-1.3.40/irails/log.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.39/irails/midware.py` & `irails-1.3.40/irails/midware.py`

 * *Files 4% similar despite different names*

```diff
@@ -71,37 +71,45 @@
                 full_path,
                 stat_result,
                 scope,
                 status_code=status_code,
 
             )
 
-
+def mount_app_statics(app,app_name,debug=False):
+    __roots = {}
+    for _dir in app.apps[app_name]['view_dirs']: 
+        _url: str = app.apps[app_name]['view_dirs'][_dir]
+        if not _url.startswith('/'):
+            _url = '/'+_url
+        _dir = os.path.normpath(_dir)
+        if os.path.exists(_dir):
+            if _url == '/':
+                __roots[_dir] = _url
+            else:
+                if not _url.endswith("/"):
+                    _url += "/"
+                _url = _url.lower()
+                if debug:
+                    _log.info(f"StaticDir:{_dir} mounted: {_url}")
+                app.mount(_url, MvcStaticFiles(directory=_dir), name=_dir)
+        else:
+            _log.warn(f"StaticDir:{_dir} do not exists!")
+    return __roots
 def mount_statics(app, debug=False):
     __roots = {}
+    root_app = ""
     for app_name in app.apps:
-
-        for _dir in app.apps[app_name]['view_dirs']:
-
-            _url: str = app.apps[app_name]['view_dirs'][_dir]
-            if not _url.startswith('/'):
-                _url = '/'+_url
-            _dir = os.path.normpath(_dir)
-            if os.path.exists(_dir):
-                if _url == '/':
-                    __roots[_dir] = _url
-                else:
-                    if not _url.endswith("/"):
-                        _url += "/"
-                    _url = _url.lower()
-                    if debug:
-                        _log.info(f"StaticDir:{_dir} mounted: {_url}")
-                    app.mount(_url, MvcStaticFiles(directory=_dir), name=_dir)
-            else:
-                _log.warn(f"StaticDir:{_dir} do not exists!")
+        
+        app__roots = mount_app_statics(app,app_name,debug)
+        if not __roots and app__roots:
+            __roots = app__roots
+            root_app = app_name
+        elif root_app and app__roots :
+            raise RuntimeError("Mount statics error,Duplicate definition of ROOT(`/`) path,`{root_app}` already defined")
     # mount public resources
     public_dir = config.get("public_dir")
     public_dir = os.path.abspath(os.path.join(ROOT_PATH, public_dir))
     if not os.path.exists(public_dir):
         os.makedirs(public_dir)
     app.mount('/public/',  MvcStaticFiles(directory=public_dir), name='public')
```

### Comparing `irails-1.3.39/irails/midware_session.py` & `irails-1.3.40/irails/midware_session.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.39/irails/mvc_router.py` & `irails-1.3.40/irails/mvc_router.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.39/irails/scripts/_app.py` & `irails-1.3.40/irails/scripts/_app.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,51 +1,26 @@
 import argparse
 import sys,os
 from typing import Any
 from jinja2 import Template
-from irails._utils import is_valid_filename,get_controller_name,get_snaked_name
+from irails._utils import is_valid_filename,get_controller_name,get_snaked_name,update_manifest,enable_app
 from  irails.config import IS_IN_irails
 
 class Generator():
     def __init__(self,args) -> None:
         self.args=args
         pass
     def gen_common(self):
         '''#todo: check configs dir
                   check data dir
 
         '''
         pass
      
-    def add_enabled_to_app(self,app_name):
-        import yaml
-        try:
-            file = './configs/general.yaml'
- 
-            with open(file, "r") as f:
-                data = yaml.load(f, Loader=yaml.FullLoader)
- 
-            enabled = data['app']['enabled']
-            if not enabled:
-                return True
-                enabled = [app_name]
-            else:
-                if isinstance(enabled,list):
-                    enabled.append(app_name) 
-            new_enabled = list(set(enabled))
-
-            data['app']['enabled'] = new_enabled
-            with open(file, "w") as f:
-                yaml.dump(data, f)
-            print(f"configs/general.yaml app.enabled has been added {app_name}!")
-            return True
-        except Exception as e:
-            print(f'an error raised {e.args}')
-            print(f"now please open configs/general.yaml to modify app.enabled to add {app_name}!")
-            return
+    
         
     def set_root_controller_to_config(self,app_dir,app_name):
         import yaml
         try:
             file = './configs/general.yaml' 
             with open(file, "r") as f:
                 data = yaml.load(f, Loader=yaml.FullLoader) 
@@ -161,25 +136,30 @@
                 'tests'
             ]
             context = {'app':app_name}
             for dir in dirs_items:
                 _current_dir = os.path.join(store_dir,dir)
                 print(f"creating {_current_dir}")
                 os.makedirs(_current_dir,exist_ok=True)
-                 
+            
+            manifest_path = os.path.join(store_dir,'manifest.yaml')
+            manifest_tpl_file = os.path.dirname(__file__)+"/tpls/app/manifest.jinja"
+            self.do_copy(manifest_tpl_file,manifest_path,True,context=context)   
+             
             # _init_file = os.path.normpath(os.path.join(store_dir,'__init__.py'))
             # with open(_init_file,'w') as f: #root path of app's dir
             #     f.write(f"from .controllers import *")
             
             # print(f"create {_init_file}")
 
-            self.add_enabled_to_app(app_name)
+            enable_app(app_name)
             if self.set_root_controller_to_config(self.args.dir,app_name):
                 self.add_home_controller(self.args.dir,app_name)
                 self.add_home_view(self.args.dir,app_name)
+                update_manifest(manifest_path=manifest_path,section = 'packages',value= 'controllers',append=True)
             cnt += 1
         if cnt:
             print(f"now ,you can cd to {self.args.dir}/{app_name} and run `irails controller \"controller's name`\" to create controllers")
             print(f"now ,you can also run `burcelee run` to run project")
         print(f"Done! created {cnt} app[s]")
     pass
```

### Comparing `irails-1.3.39/irails/scripts/_controller.py` & `irails-1.3.40/irails/scripts/_controller.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import argparse
 import sys,os,re
 from typing import Any
 from jinja2 import Template
-from irails._utils import is_valid_filename,get_controller_name,get_snaked_name,to_camel_case,ensure_line
+from irails._utils import is_valid_filename,get_controller_name,get_snaked_name,to_camel_case,ensure_line,update_manifest
 from  irails.config import is_in_irails,is_in_app
 
 class Generator():
     def __init__(self,args,dir) -> None:
         self.args = args
         self.dir = dir
         pass
@@ -105,14 +105,17 @@
                     dest = os.path.join(_current_dir , item['dest'])
                     micro = item['micro']
                     #controller file will generate last time
                     self.gen_tpl(tpl_file=tpl,dest=dest,context=context,use_micro=micro,dir_only=True) 
             controller_file = os.path.join(_current_dir,'controllers',f"{controler_path_name}_controller.py")
             __init_file = os.path.join(_current_dir,'controllers','__init__.py')
             ensure_line(__init_file,f"from . import {controler_path_name}_controller")
+
+            manifest_path = os.path.join(_current_dir,'manifest.yaml')
+            update_manifest(manifest_path=manifest_path,section = 'packages',value = 'controllers',append=True)
             # __init_file = os.path.join(_current_dir,'models','__init__.py')
             # ensure_line(__init_file,f"from . import {controler_path_name}_model")
             # __init_file = os.path.join(_current_dir,'services','__init__.py')
             # ensure_line(__init_file,f"from . import {controler_path_name}_service")
             
             for action in actions:
                 acts.append(f"""
```

### Comparing `irails-1.3.39/irails/scripts/_i18n.py` & `irails-1.3.40/irails/scripts/_i18n.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.39/irails/scripts/_migrate.py` & `irails-1.3.40/irails/scripts/_migrate.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import argparse
 import os, sys
 import uvicorn
 from irails.config import IS_IN_irails
-from irails._loader import _load_apps
+from irails._loader import collect_apps
  
 from irails.config import config
 
 def main():
      
     if not IS_IN_irails:
         print(f"`migrate` command must run in the directory of irails project")
@@ -27,14 +27,14 @@
     else:
         parser.print_usage()
         exit()
     from irails.database import check_migration,init_database
     db_cfg = config.get("database")
     db_uri = db_cfg.get("uri")
     alembic_ini = db_cfg.get('alembic_ini')
-    _load_apps()
+    collect_apps()
     engine = init_database(db_uri,debug=True,cfg = db_cfg)
     if engine:
         check_migration(engine=engine,uri= db_uri,alembic_ini= alembic_ini,upgrade=is_up)
```

### Comparing `irails-1.3.39/irails/scripts/_model.py` & `irails-1.3.40/irails/scripts/_model.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import argparse
 import sys
 import os
 from jinja2 import Template
-from irails._utils import get_snaked_name, to_camel_case, get_plural_name,ensure_line
+from irails._utils import get_snaked_name, to_camel_case, get_plural_name,ensure_line,update_manifest
 import typing
 
 from irails.config import is_in_app, is_in_irails
 cur_dir = os.path.abspath(os.curdir)
 
 
 def render_tpl(src_tpl, dest_file, context: typing.Dict):
@@ -35,52 +35,57 @@
 def get_app_name():
     app_dir = os.path.basename(cur_dir)
      
     return f"{app_dir}"
 
 
 def generate(args):
+    ret = False
     app_name = get_app_name()
     if not args.name:
         print(f'controller name is empty,exit!')
         exit()
     name = args.name.pop(0)
     model_name = to_camel_case(name)
     model_path_name = get_snaked_name(name)
     model_plural_name = get_plural_name(model_name).lower()
     context = {"model_name": model_name,
                "model_path_name": model_path_name,
                "model_plural_name": model_plural_name,
                "app_name": app_name,
                }
     columns = []
-    if not len(args.name) > 0:
-        args.name.append("id")
+    # if not len(args.name) > 0:
+    #     args.name.append("id")
     columns = args.name
     context["columns"] = columns
     dest_file = os.path.join(cur_dir, "models", model_path_name+'.py')
     src_tpl = "model.jinja"
+    manifest_path = os.path.join(cur_dir,'manifest.yaml')
+
     if render_tpl(src_tpl=src_tpl, dest_file=dest_file, context=context): #model file
         __init_file = os.path.join(cur_dir,'models','__init__.py')
         ensure_line(__init_file,f"from .{model_path_name} import *")
-
+        update_manifest(manifest_path=manifest_path,section='packages',value='models',append=True)
         service_path_name = model_path_name+'_service'
         dest_file = os.path.join(cur_dir, "services", service_path_name+'.py')
         context['service_name'] = f"{model_name}Service"
         context['service_path_name'] = service_path_name
         if render_tpl(src_tpl="service.jinja", dest_file=dest_file, context=context):#service file
             __init_file = os.path.join(cur_dir,'services','__init__.py')
             ensure_line(__init_file,f"from .{service_path_name} import *")
-
+            update_manifest(manifest_path=manifest_path,section='packages',value='services',append=True)
             dest_file = os.path.join(
                 cur_dir, "tests", f"test_{service_path_name}.py")
             if render_tpl(src_tpl="test_service.jinja", dest_file=dest_file, context=context):#test service file
                 print("Done!")
-                return True
-    return False
+                ret = True
+     
+
+    return ret
 
 
 def main():
     root_path = os.path.abspath(os.path.join(cur_dir, "../.."))
     if os.path.exists(root_path) and os.path.isdir(root_path):
         if not is_in_irails(root_path) or not is_in_app(cur_dir):
             print(f"Please exec in irails project's app dir ,like `apps/app`")
```

### Comparing `irails-1.3.39/irails/scripts/_project.py` & `irails-1.3.40/irails/scripts/_project.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.39/irails/scripts/_run.py` & `irails-1.3.40/irails/scripts/_run.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.39/irails/scripts/_shell.py` & `irails-1.3.40/irails/scripts/_shell.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.39/irails/scripts/_test.py` & `irails-1.3.40/irails/scripts/_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,25 +55,25 @@
     for name in test_files:
         print(f"Starting test {test_files[name]}")
         do_test_file(app_dir, test_files[name])
     
     sys.path.remove(app_package_dir)
 
 def get_all_enabled_apps():
-    from irails._loader import _load_apps
-    apps = _load_apps(do_load=False)
+    from irails._loader import collect_apps
+    apps = collect_apps(do_load=False)
     return apps
 def do_test_project(print_out=None): 
      
     response = input("Do you want to continue to test all apps? (y/n)")
     if response.lower() == "y":
          
         apps = get_all_enabled_apps() 
         for app in apps:
-            dirs = app.split('.')
+            dirs = app['package'].split('.')
             if len(dirs)==2:
                 app_dir = os.path.join(curdir,dirs[0],dirs[1])
                 do_test_app(app_dir=app_dir, print_out=print_out)
          
     elif response.lower() == "n":
         print("User chose to cancel.")
     else:
```

### Comparing `irails-1.3.39/irails/scripts/main.py` & `irails-1.3.40/irails/scripts/main.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.39/irails/scripts/tpls/app/home.css.tpl` & `irails-1.3.40/irails/scripts/tpls/app/home.css.tpl`

 * *Files identical despite different names*

### Comparing `irails-1.3.39/irails/scripts/tpls/app/home.tpl` & `irails-1.3.40/irails/scripts/tpls/app/home.tpl`

 * *Files identical despite different names*

### Comparing `irails-1.3.39/irails/scripts/tpls/app/model.jinja` & `irails-1.3.40/irails/scripts/tpls/app/model.jinja`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from irails import database
 from sqlalchemy import Table,Column,ForeignKey,String,Integer
 from sqlalchemy.orm import Mapped,mapped_column,relationship
  
 class {{model_name}}(database.Base):
-    __tablename__ = f"{database.table_prefix}{{model_plural_name}}" 
+    __tablename__ = "{{model_plural_name}}" 
     {% if not 'id' in columns -%}
     id: Mapped[int] = mapped_column(primary_key=True) 
     {%- endif -%} 
     {%- for col in columns -%}
         {% if ':' in col %}
             {% set col_type = col.split(":")[1]+'()' %}
             {% if col_type == 'int()' %}
```

### Comparing `irails-1.3.39/irails/scripts/tpls/app/test_service.jinja` & `irails-1.3.40/irails/scripts/tpls/app/test_service.jinja`

 * *Files identical despite different names*

### Comparing `irails-1.3.39/irails/scripts/tpls/project/configs/alembic.ini` & `irails-1.3.40/irails/scripts/tpls/project/configs/alembic.ini`

 * *Files identical despite different names*

### Comparing `irails-1.3.39/irails/scripts/tpls/project/configs/database.yaml` & `irails-1.3.40/irails/scripts/tpls/project/configs/database.yaml`

 * *Files identical despite different names*

### Comparing `irails-1.3.39/irails/scripts/tpls/project/configs/general.yaml` & `irails-1.3.40/irails/scripts/tpls/project/configs/general.yaml`

 * *Files identical despite different names*

### Comparing `irails-1.3.39/irails/scripts/tpls/project/data/alembic/env.py` & `irails-1.3.40/irails/scripts/tpls/project/data/alembic/env.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.39/irails/scripts/tpls/project/public/error_404.html` & `irails-1.3.40/irails/scripts/tpls/project/public/error_404.html`

 * *Files identical despite different names*

### Comparing `irails-1.3.39/irails/scripts/tpls/project/public/error_500.html` & `irails-1.3.40/irails/scripts/tpls/project/public/error_500.html`

 * *Files identical despite different names*

### Comparing `irails-1.3.39/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js` & `irails-1.3.40/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js`

 * *Files identical despite different names*

### Comparing `irails-1.3.39/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css` & `irails-1.3.40/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css`

 * *Files identical despite different names*

### Comparing `irails-1.3.39/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js` & `irails-1.3.40/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js`

 * *Files identical despite different names*

### Comparing `irails-1.3.39/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js` & `irails-1.3.40/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js`

 * *Files identical despite different names*

### Comparing `irails-1.3.39/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js` & `irails-1.3.40/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js`

 * *Files identical despite different names*

### Comparing `irails-1.3.39/irails/scripts/tpls/project/public/vue_home.html` & `irails-1.3.40/irails/scripts/tpls/project/public/vue_home.html`

 * *Files identical despite different names*

### Comparing `irails-1.3.39/irails/unit_test.py` & `irails-1.3.40/irails/unit_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         
     pass
 
 class ServiceTest(_BaseUnitTest):
     def __init__(self,*args,**kwargv) -> None:
         super().__init__(*args,**kwargv)
         from .config import config
-        from ._loader import _load_apps
+        from ._loader import collect_apps
         from irails.database import Service,engine,Session,init_database
         from irails.database import check_migration
         from irails.core import check_init_auth
         # _load_apps()
         if not hasattr(ServiceTest,'engine'):
             db_cfg = config.get("database")
             db_uri = db_cfg.get("uri")
```

### Comparing `irails-1.3.39/irails/view.py` & `irails-1.3.40/irails/view.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.39/irails.egg-info/PKG-INFO` & `irails-1.3.40/irails.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: irails
-Version: 1.3.39
+Version: 1.3.40
 Summary: Simple and elegant use of FastApi in MVC mode
 Home-page: https://github.com/smjkzsl/irails
 Author: Bruce chou
 Author-email: smjkzsl@gmail.com
 License: Apache License 2.0
 Keywords: web framework,mvc framework,fastapi framework
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -84,9 +83,7 @@
     +---uploads                             ## Others dir(if your need or not)
 ```
 ## Extras commands
 * `irails i18n gettext`  --generate i18n in irails app dir
 * `irails shell`         --run python interpreter with buildin support contexts 
 * `irails test`          --run project tests 
 * `irails migrate`       --run database migrations
-
-
```

### Comparing `irails-1.3.39/irails.egg-info/SOURCES.txt` & `irails-1.3.40/irails.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 irails/scripts/_shell.py
 irails/scripts/_test.py
 irails/scripts/main.py
 irails/scripts/tpls/app/controller.tpl
 irails/scripts/tpls/app/css.tpl
 irails/scripts/tpls/app/home.css.tpl
 irails/scripts/tpls/app/home.tpl
+irails/scripts/tpls/app/manifest.jinja
 irails/scripts/tpls/app/model.jinja
 irails/scripts/tpls/app/service.jinja
 irails/scripts/tpls/app/test_controller.jinja
 irails/scripts/tpls/app/test_service.jinja
 irails/scripts/tpls/app/view.tpl
 irails/scripts/tpls/project/.gitignore
 irails/scripts/tpls/project/main.py
```

### Comparing `irails-1.3.39/setup.py` & `irails-1.3.40/setup.py`

 * *Files identical despite different names*

