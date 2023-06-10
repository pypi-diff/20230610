# Comparing `tmp/lamindb_setup-0.47.3.tar.gz` & `tmp/lamindb_setup-0.47.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lamindb_setup-0.47.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "lamindb_setup-0.47.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `lamindb_setup-0.47.3.tar` & `lamindb_setup-0.47.4.tar`

### file list

```diff
@@ -1,91 +1,91 @@
--rw-r--r--   0        0        0     4010 2023-06-05 07:30:18.302219 lamindb_setup-0.47.3/.github/workflows/build.yml
--rw-r--r--   0        0        0      133 2023-06-01 15:58:18.274054 lamindb_setup-0.47.3/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      597 2023-06-01 15:58:18.274134 lamindb_setup-0.47.3/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1204 2023-06-01 15:58:18.274221 lamindb_setup-0.47.3/.gitignore
--rw-r--r--   0        0        0      100 2023-06-01 15:58:18.274299 lamindb_setup-0.47.3/.gitmodules
--rw-r--r--   0        0        0     1798 2023-06-05 07:30:18.302425 lamindb_setup-0.47.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0    11324 2023-06-01 15:58:18.274545 lamindb_setup-0.47.3/LICENSE
--rw-r--r--   0        0        0      318 2023-06-05 07:30:18.302530 lamindb_setup-0.47.3/README.md
--rw-r--r--   0        0        0    53846 2023-06-10 19:27:01.812820 lamindb_setup-0.47.3/docs/changelog.md
--rw-r--r--   0        0        0     6341 2023-06-05 07:30:18.302966 lamindb_setup-0.47.3/docs/faq/edge-cases-login-init.ipynb
--rw-r--r--   0        0        0       96 2023-06-05 07:30:18.303105 lamindb_setup-0.47.3/docs/faq/index.md
--rw-r--r--   0        0        0     3323 2023-06-01 15:58:18.275949 lamindb_setup-0.47.3/docs/faq/switch-environment.ipynb
--rw-r--r--   0        0        0     6590 2023-06-07 16:09:22.842055 lamindb_setup-0.47.3/docs/faq/test-sqlite-sync.ipynb
--rw-r--r--   0        0        0     8164 2023-06-08 13:53:23.373767 lamindb_setup-0.47.3/docs/guide/01-init-instance.ipynb
--rw-r--r--   0        0        0     4362 2023-06-08 13:53:23.373956 lamindb_setup-0.47.3/docs/guide/02-load-instance.ipynb
--rw-r--r--   0        0        0     5750 2023-06-08 13:53:23.374226 lamindb_setup-0.47.3/docs/guide/03-set-storage.ipynb
--rw-r--r--   0        0        0     3293 2023-06-10 10:42:49.132865 lamindb_setup-0.47.3/docs/guide/04-schema-modules.ipynb
--rw-r--r--   0        0        0      114 2023-06-08 18:13:52.871462 lamindb_setup-0.47.3/docs/guide/index.md
--rw-r--r--   0        0        0      409 2023-06-08 18:13:52.872258 lamindb_setup-0.47.3/docs/guide/migrate.md
--rw-r--r--   0        0        0     1250 2023-06-08 13:53:23.374760 lamindb_setup-0.47.3/docs/guide/setup-user.md
--rw-r--r--   0        0        0      132 2023-06-08 13:53:23.374929 lamindb_setup-0.47.3/docs/index.md
--rw-r--r--   0        0        0       61 2023-06-08 13:53:23.375035 lamindb_setup-0.47.3/docs/reference.md
--rw-r--r--   0        0        0      365 2023-06-01 15:58:18.277034 lamindb_setup-0.47.3/docs/test_notebooks.py
--rw-r--r--   0        0        0      142 2023-06-04 07:57:01.647274 lamindb_setup-0.47.3/lamin-project.yaml
--rw-r--r--   0        0        0     2715 2023-06-10 19:26:49.513102 lamindb_setup-0.47.3/lamindb_setup/__init__.py
--rw-r--r--   0        0        0     5346 2023-06-07 20:38:59.482711 lamindb_setup-0.47.3/lamindb_setup/__main__.py
--rw-r--r--   0        0        0     1410 2023-06-05 07:31:41.044617 lamindb_setup-0.47.3/lamindb_setup/_check_instance_setup.py
--rw-r--r--   0        0        0      661 2023-06-09 20:32:18.168808 lamindb_setup-0.47.3/lamindb_setup/_close.py
--rw-r--r--   0        0        0     2006 2023-06-07 16:09:22.843059 lamindb_setup-0.47.3/lamindb_setup/_delete.py
--rw-r--r--   0        0        0      585 2023-06-05 07:30:18.304343 lamindb_setup-0.47.3/lamindb_setup/_docstrings.py
--rw-r--r--   0        0        0      329 2023-06-01 15:58:18.277912 lamindb_setup-0.47.3/lamindb_setup/_info.py
--rw-r--r--   0        0        0     6835 2023-06-10 18:56:23.117926 lamindb_setup-0.47.3/lamindb_setup/_init_instance.py
--rw-r--r--   0        0        0     5411 2023-06-09 20:04:14.225151 lamindb_setup-0.47.3/lamindb_setup/_load_instance.py
--rw-r--r--   0        0        0      322 2023-06-05 07:30:18.304745 lamindb_setup-0.47.3/lamindb_setup/_migrate.py
--rw-r--r--   0        0        0     1692 2023-06-03 14:25:55.266155 lamindb_setup-0.47.3/lamindb_setup/_notebook.py
--rw-r--r--   0        0        0      825 2023-06-05 07:30:18.304849 lamindb_setup-0.47.3/lamindb_setup/_register_instance.py
--rw-r--r--   0        0        0     1057 2023-06-05 07:30:18.305060 lamindb_setup-0.47.3/lamindb_setup/_schema.py
--rw-r--r--   0        0        0     1891 2023-06-07 20:38:59.483389 lamindb_setup-0.47.3/lamindb_setup/_set.py
--rw-r--r--   0        0        0     2247 2023-06-01 15:58:18.279311 lamindb_setup-0.47.3/lamindb_setup/_settings.py
--rw-r--r--   0        0        0       87 2023-06-01 15:58:18.279395 lamindb_setup-0.47.3/lamindb_setup/_settings_load.py
--rw-r--r--   0        0        0       72 2023-06-01 15:58:18.279466 lamindb_setup-0.47.3/lamindb_setup/_settings_store.py
--rw-r--r--   0        0        0     3548 2023-06-05 07:30:18.305347 lamindb_setup-0.47.3/lamindb_setup/_setup_user.py
--rw-r--r--   0        0        0      785 2023-06-05 07:30:18.305424 lamindb_setup-0.47.3/lamindb_setup/_silence_loggers.py
--rw-r--r--   0        0        0      456 2023-06-01 15:58:18.279648 lamindb_setup-0.47.3/lamindb_setup/dev/__init__.py
--rw-r--r--   0        0        0     5385 2023-06-07 16:33:24.023221 lamindb_setup-0.47.3/lamindb_setup/dev/_cloud_sqlite_locker.py
--rw-r--r--   0        0        0     2491 2023-06-01 15:58:18.279932 lamindb_setup-0.47.3/lamindb_setup/dev/_deprecated.py
--rw-r--r--   0        0        0     2905 2023-06-08 18:13:52.872904 lamindb_setup-0.47.3/lamindb_setup/dev/_django.py
--rw-r--r--   0        0        0      240 2023-06-01 15:58:18.280089 lamindb_setup-0.47.3/lamindb_setup/dev/_docs.py
--rw-r--r--   0        0        0     9315 2023-06-08 18:13:52.873426 lamindb_setup-0.47.3/lamindb_setup/dev/_settings_instance.py
--rw-r--r--   0        0        0     2597 2023-06-01 15:58:18.280386 lamindb_setup-0.47.3/lamindb_setup/dev/_settings_load.py
--rw-r--r--   0        0        0     2061 2023-06-01 15:58:18.280470 lamindb_setup-0.47.3/lamindb_setup/dev/_settings_save.py
--rw-r--r--   0        0        0     2318 2023-06-05 07:30:18.305825 lamindb_setup-0.47.3/lamindb_setup/dev/_settings_store.py
--rw-r--r--   0        0        0     1088 2023-06-01 15:58:18.280631 lamindb_setup-0.47.3/lamindb_setup/dev/_settings_user.py
--rw-r--r--   0        0        0     2162 2023-06-10 19:26:14.501079 lamindb_setup-0.47.3/lamindb_setup/dev/_setup_bionty_sources.py
--rw-r--r--   0        0        0     2140 2023-06-05 07:31:41.044990 lamindb_setup-0.47.3/lamindb_setup/dev/_setup_schema.py
--rw-r--r--   0        0        0     5057 2023-06-05 07:30:18.306219 lamindb_setup-0.47.3/lamindb_setup/dev/_storage.py
--rw-r--r--   0        0        0     2670 2023-06-08 18:13:52.874452 lamindb_setup-0.47.3/lamindb_setup/dev/upath.py
--rw-r--r--   0        0        0     2811 2023-06-05 11:32:22.995643 lamindb_setup-0.47.3/lnschema-core/.github/workflows/build.yml
--rw-r--r--   0        0        0      133 2023-06-05 11:32:22.995738 lamindb_setup-0.47.3/lnschema-core/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      597 2023-06-05 11:32:22.995812 lamindb_setup-0.47.3/lnschema-core/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1381 2023-06-05 11:32:22.995890 lamindb_setup-0.47.3/lnschema-core/.gitignore
--rw-r--r--   0        0        0        0 2023-06-05 11:32:22.995916 lamindb_setup-0.47.3/lnschema-core/.gitmodules
--rw-r--r--   0        0        0     1836 2023-06-05 11:32:22.996008 lamindb_setup-0.47.3/lnschema-core/.pre-commit-config.yaml
--rw-r--r--   0        0        0    11324 2023-06-05 11:32:22.996105 lamindb_setup-0.47.3/lnschema-core/LICENSE
--rw-r--r--   0        0        0      364 2023-06-05 11:32:22.996173 lamindb_setup-0.47.3/lnschema-core/README.md
--rw-r--r--   0        0        0    25740 2023-06-05 11:32:22.996389 lamindb_setup-0.47.3/lnschema-core/docs/changelog.md
--rw-r--r--   0        0        0     1485 2023-06-05 11:32:22.996551 lamindb_setup-0.47.3/lnschema-core/docs/guide/core-schema.ipynb
--rw-r--r--   0        0        0       52 2023-06-05 11:32:22.996748 lamindb_setup-0.47.3/lnschema-core/docs/guide/index.md
--rw-r--r--   0        0        0      112 2023-06-05 11:32:22.996845 lamindb_setup-0.47.3/lnschema-core/docs/index.md
--rw-r--r--   0        0        0      202 2023-06-05 11:32:22.996914 lamindb_setup-0.47.3/lnschema-core/lamin-project.yaml
--rw-r--r--   0        0        0      592 2023-06-05 11:32:22.997066 lamindb_setup-0.47.3/lnschema-core/lnschema_core/__init__.py
--rw-r--r--   0        0        0     1515 2023-06-05 11:32:22.997223 lamindb_setup-0.47.3/lnschema-core/lnschema_core/_lookup.py
--rw-r--r--   0        0        0      756 2023-06-05 11:32:22.997329 lamindb_setup-0.47.3/lnschema-core/lnschema_core/_types.py
--rw-r--r--   0        0        0      349 2023-06-05 11:32:22.997395 lamindb_setup-0.47.3/lnschema-core/lnschema_core/_users.py
--rw-r--r--   0        0        0     2810 2023-06-05 11:32:22.997546 lamindb_setup-0.47.3/lnschema-core/lnschema_core/ids.py
--rw-r--r--   0        0        0    11504 2023-06-05 11:32:22.997705 lamindb_setup-0.47.3/lnschema-core/lnschema_core/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-06-05 11:32:22.997742 lamindb_setup-0.47.3/lnschema-core/lnschema_core/migrations/__init__.py
--rw-r--r--   0        0        0    24760 2023-06-05 11:32:22.997959 lamindb_setup-0.47.3/lnschema-core/lnschema_core/models.py
--rw-r--r--   0        0        0      180 2023-06-05 11:32:22.998145 lamindb_setup-0.47.3/lnschema-core/lnschema_core/types.py
--rw-r--r--   0        0        0     1299 2023-06-05 11:32:22.998461 lamindb_setup-0.47.3/lnschema-core/noxfile.py
--rw-r--r--   0        0        0      850 2023-06-05 11:32:22.998642 lamindb_setup-0.47.3/lnschema-core/pyproject.toml
--rw-r--r--   0        0        0      475 2023-06-05 11:32:22.998792 lamindb_setup-0.47.3/lnschema-core/tests/test_notebooks.py
--rw-r--r--   0        0        0     1911 2023-06-07 16:33:24.024562 lamindb_setup-0.47.3/noxfile.py
--rw-r--r--   0        0        0     1337 2023-06-10 19:26:14.501478 lamindb_setup-0.47.3/pyproject.toml
--rw-r--r--   0        0        0      672 2023-06-05 07:30:18.308956 lamindb_setup-0.47.3/tests/test_bionty.py
--rw-r--r--   0        0        0     3041 2023-06-01 15:58:18.282108 lamindb_setup-0.47.3/tests/test_init_instance.py
--rw-r--r--   0        0        0      655 2023-06-01 15:58:18.282187 lamindb_setup-0.47.3/tests/test_load_instance.py
--rw-r--r--   0        0        0      501 2023-06-08 13:53:23.375191 lamindb_setup-0.47.3/tests/test_login.py
--rw-r--r--   0        0        0      243 2023-06-01 15:58:18.282270 lamindb_setup-0.47.3/tests/test_set_storage.py
--rw-r--r--   0        0        0      125 2023-06-08 13:53:23.375328 lamindb_setup-0.47.3/tests/test_signup.py
--rw-r--r--   0        0        0     1366 1970-01-01 00:00:00.000000 lamindb_setup-0.47.3/PKG-INFO
+-rw-r--r--   0        0        0     4010 2023-06-05 07:30:18.302219 lamindb_setup-0.47.4/.github/workflows/build.yml
+-rw-r--r--   0        0        0      133 2023-06-01 15:58:18.274054 lamindb_setup-0.47.4/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      597 2023-06-01 15:58:18.274134 lamindb_setup-0.47.4/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1204 2023-06-01 15:58:18.274221 lamindb_setup-0.47.4/.gitignore
+-rw-r--r--   0        0        0      100 2023-06-01 15:58:18.274299 lamindb_setup-0.47.4/.gitmodules
+-rw-r--r--   0        0        0     1798 2023-06-05 07:30:18.302425 lamindb_setup-0.47.4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    11324 2023-06-01 15:58:18.274545 lamindb_setup-0.47.4/LICENSE
+-rw-r--r--   0        0        0      318 2023-06-05 07:30:18.302530 lamindb_setup-0.47.4/README.md
+-rw-r--r--   0        0        0    54030 2023-06-10 19:43:58.322358 lamindb_setup-0.47.4/docs/changelog.md
+-rw-r--r--   0        0        0     6341 2023-06-05 07:30:18.302966 lamindb_setup-0.47.4/docs/faq/edge-cases-login-init.ipynb
+-rw-r--r--   0        0        0       96 2023-06-05 07:30:18.303105 lamindb_setup-0.47.4/docs/faq/index.md
+-rw-r--r--   0        0        0     3323 2023-06-01 15:58:18.275949 lamindb_setup-0.47.4/docs/faq/switch-environment.ipynb
+-rw-r--r--   0        0        0     6590 2023-06-07 16:09:22.842055 lamindb_setup-0.47.4/docs/faq/test-sqlite-sync.ipynb
+-rw-r--r--   0        0        0     8164 2023-06-08 13:53:23.373767 lamindb_setup-0.47.4/docs/guide/01-init-instance.ipynb
+-rw-r--r--   0        0        0     4362 2023-06-08 13:53:23.373956 lamindb_setup-0.47.4/docs/guide/02-load-instance.ipynb
+-rw-r--r--   0        0        0     5750 2023-06-08 13:53:23.374226 lamindb_setup-0.47.4/docs/guide/03-set-storage.ipynb
+-rw-r--r--   0        0        0     3293 2023-06-10 10:42:49.132865 lamindb_setup-0.47.4/docs/guide/04-schema-modules.ipynb
+-rw-r--r--   0        0        0      114 2023-06-08 18:13:52.871462 lamindb_setup-0.47.4/docs/guide/index.md
+-rw-r--r--   0        0        0      409 2023-06-08 18:13:52.872258 lamindb_setup-0.47.4/docs/guide/migrate.md
+-rw-r--r--   0        0        0     1250 2023-06-08 13:53:23.374760 lamindb_setup-0.47.4/docs/guide/setup-user.md
+-rw-r--r--   0        0        0      132 2023-06-08 13:53:23.374929 lamindb_setup-0.47.4/docs/index.md
+-rw-r--r--   0        0        0       61 2023-06-08 13:53:23.375035 lamindb_setup-0.47.4/docs/reference.md
+-rw-r--r--   0        0        0      365 2023-06-01 15:58:18.277034 lamindb_setup-0.47.4/docs/test_notebooks.py
+-rw-r--r--   0        0        0      142 2023-06-04 07:57:01.647274 lamindb_setup-0.47.4/lamin-project.yaml
+-rw-r--r--   0        0        0     2715 2023-06-10 19:43:44.432746 lamindb_setup-0.47.4/lamindb_setup/__init__.py
+-rw-r--r--   0        0        0     5346 2023-06-07 20:38:59.482711 lamindb_setup-0.47.4/lamindb_setup/__main__.py
+-rw-r--r--   0        0        0     1410 2023-06-05 07:31:41.044617 lamindb_setup-0.47.4/lamindb_setup/_check_instance_setup.py
+-rw-r--r--   0        0        0      661 2023-06-09 20:32:18.168808 lamindb_setup-0.47.4/lamindb_setup/_close.py
+-rw-r--r--   0        0        0     2006 2023-06-07 16:09:22.843059 lamindb_setup-0.47.4/lamindb_setup/_delete.py
+-rw-r--r--   0        0        0      585 2023-06-05 07:30:18.304343 lamindb_setup-0.47.4/lamindb_setup/_docstrings.py
+-rw-r--r--   0        0        0      329 2023-06-01 15:58:18.277912 lamindb_setup-0.47.4/lamindb_setup/_info.py
+-rw-r--r--   0        0        0     6835 2023-06-10 18:56:23.117926 lamindb_setup-0.47.4/lamindb_setup/_init_instance.py
+-rw-r--r--   0        0        0     5411 2023-06-09 20:04:14.225151 lamindb_setup-0.47.4/lamindb_setup/_load_instance.py
+-rw-r--r--   0        0        0      322 2023-06-05 07:30:18.304745 lamindb_setup-0.47.4/lamindb_setup/_migrate.py
+-rw-r--r--   0        0        0     1692 2023-06-03 14:25:55.266155 lamindb_setup-0.47.4/lamindb_setup/_notebook.py
+-rw-r--r--   0        0        0      825 2023-06-05 07:30:18.304849 lamindb_setup-0.47.4/lamindb_setup/_register_instance.py
+-rw-r--r--   0        0        0     1057 2023-06-05 07:30:18.305060 lamindb_setup-0.47.4/lamindb_setup/_schema.py
+-rw-r--r--   0        0        0     1891 2023-06-07 20:38:59.483389 lamindb_setup-0.47.4/lamindb_setup/_set.py
+-rw-r--r--   0        0        0     2247 2023-06-01 15:58:18.279311 lamindb_setup-0.47.4/lamindb_setup/_settings.py
+-rw-r--r--   0        0        0       87 2023-06-01 15:58:18.279395 lamindb_setup-0.47.4/lamindb_setup/_settings_load.py
+-rw-r--r--   0        0        0       72 2023-06-01 15:58:18.279466 lamindb_setup-0.47.4/lamindb_setup/_settings_store.py
+-rw-r--r--   0        0        0     3548 2023-06-05 07:30:18.305347 lamindb_setup-0.47.4/lamindb_setup/_setup_user.py
+-rw-r--r--   0        0        0      785 2023-06-05 07:30:18.305424 lamindb_setup-0.47.4/lamindb_setup/_silence_loggers.py
+-rw-r--r--   0        0        0      456 2023-06-01 15:58:18.279648 lamindb_setup-0.47.4/lamindb_setup/dev/__init__.py
+-rw-r--r--   0        0        0     5385 2023-06-07 16:33:24.023221 lamindb_setup-0.47.4/lamindb_setup/dev/_cloud_sqlite_locker.py
+-rw-r--r--   0        0        0     2491 2023-06-01 15:58:18.279932 lamindb_setup-0.47.4/lamindb_setup/dev/_deprecated.py
+-rw-r--r--   0        0        0     2905 2023-06-08 18:13:52.872904 lamindb_setup-0.47.4/lamindb_setup/dev/_django.py
+-rw-r--r--   0        0        0      240 2023-06-01 15:58:18.280089 lamindb_setup-0.47.4/lamindb_setup/dev/_docs.py
+-rw-r--r--   0        0        0     9315 2023-06-08 18:13:52.873426 lamindb_setup-0.47.4/lamindb_setup/dev/_settings_instance.py
+-rw-r--r--   0        0        0     2597 2023-06-01 15:58:18.280386 lamindb_setup-0.47.4/lamindb_setup/dev/_settings_load.py
+-rw-r--r--   0        0        0     2061 2023-06-01 15:58:18.280470 lamindb_setup-0.47.4/lamindb_setup/dev/_settings_save.py
+-rw-r--r--   0        0        0     2318 2023-06-05 07:30:18.305825 lamindb_setup-0.47.4/lamindb_setup/dev/_settings_store.py
+-rw-r--r--   0        0        0     1088 2023-06-01 15:58:18.280631 lamindb_setup-0.47.4/lamindb_setup/dev/_settings_user.py
+-rw-r--r--   0        0        0     2224 2023-06-10 19:43:06.748471 lamindb_setup-0.47.4/lamindb_setup/dev/_setup_bionty_sources.py
+-rw-r--r--   0        0        0     2140 2023-06-05 07:31:41.044990 lamindb_setup-0.47.4/lamindb_setup/dev/_setup_schema.py
+-rw-r--r--   0        0        0     5057 2023-06-05 07:30:18.306219 lamindb_setup-0.47.4/lamindb_setup/dev/_storage.py
+-rw-r--r--   0        0        0     2670 2023-06-08 18:13:52.874452 lamindb_setup-0.47.4/lamindb_setup/dev/upath.py
+-rw-r--r--   0        0        0     2811 2023-06-05 11:32:22.995643 lamindb_setup-0.47.4/lnschema-core/.github/workflows/build.yml
+-rw-r--r--   0        0        0      133 2023-06-05 11:32:22.995738 lamindb_setup-0.47.4/lnschema-core/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      597 2023-06-05 11:32:22.995812 lamindb_setup-0.47.4/lnschema-core/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1381 2023-06-05 11:32:22.995890 lamindb_setup-0.47.4/lnschema-core/.gitignore
+-rw-r--r--   0        0        0        0 2023-06-05 11:32:22.995916 lamindb_setup-0.47.4/lnschema-core/.gitmodules
+-rw-r--r--   0        0        0     1836 2023-06-05 11:32:22.996008 lamindb_setup-0.47.4/lnschema-core/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    11324 2023-06-05 11:32:22.996105 lamindb_setup-0.47.4/lnschema-core/LICENSE
+-rw-r--r--   0        0        0      364 2023-06-05 11:32:22.996173 lamindb_setup-0.47.4/lnschema-core/README.md
+-rw-r--r--   0        0        0    25740 2023-06-05 11:32:22.996389 lamindb_setup-0.47.4/lnschema-core/docs/changelog.md
+-rw-r--r--   0        0        0     1485 2023-06-05 11:32:22.996551 lamindb_setup-0.47.4/lnschema-core/docs/guide/core-schema.ipynb
+-rw-r--r--   0        0        0       52 2023-06-05 11:32:22.996748 lamindb_setup-0.47.4/lnschema-core/docs/guide/index.md
+-rw-r--r--   0        0        0      112 2023-06-05 11:32:22.996845 lamindb_setup-0.47.4/lnschema-core/docs/index.md
+-rw-r--r--   0        0        0      202 2023-06-05 11:32:22.996914 lamindb_setup-0.47.4/lnschema-core/lamin-project.yaml
+-rw-r--r--   0        0        0      592 2023-06-05 11:32:22.997066 lamindb_setup-0.47.4/lnschema-core/lnschema_core/__init__.py
+-rw-r--r--   0        0        0     1515 2023-06-05 11:32:22.997223 lamindb_setup-0.47.4/lnschema-core/lnschema_core/_lookup.py
+-rw-r--r--   0        0        0      756 2023-06-05 11:32:22.997329 lamindb_setup-0.47.4/lnschema-core/lnschema_core/_types.py
+-rw-r--r--   0        0        0      349 2023-06-05 11:32:22.997395 lamindb_setup-0.47.4/lnschema-core/lnschema_core/_users.py
+-rw-r--r--   0        0        0     2810 2023-06-05 11:32:22.997546 lamindb_setup-0.47.4/lnschema-core/lnschema_core/ids.py
+-rw-r--r--   0        0        0    11504 2023-06-05 11:32:22.997705 lamindb_setup-0.47.4/lnschema-core/lnschema_core/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-06-05 11:32:22.997742 lamindb_setup-0.47.4/lnschema-core/lnschema_core/migrations/__init__.py
+-rw-r--r--   0        0        0    24760 2023-06-05 11:32:22.997959 lamindb_setup-0.47.4/lnschema-core/lnschema_core/models.py
+-rw-r--r--   0        0        0      180 2023-06-05 11:32:22.998145 lamindb_setup-0.47.4/lnschema-core/lnschema_core/types.py
+-rw-r--r--   0        0        0     1299 2023-06-05 11:32:22.998461 lamindb_setup-0.47.4/lnschema-core/noxfile.py
+-rw-r--r--   0        0        0      850 2023-06-05 11:32:22.998642 lamindb_setup-0.47.4/lnschema-core/pyproject.toml
+-rw-r--r--   0        0        0      475 2023-06-05 11:32:22.998792 lamindb_setup-0.47.4/lnschema-core/tests/test_notebooks.py
+-rw-r--r--   0        0        0     1911 2023-06-07 16:33:24.024562 lamindb_setup-0.47.4/noxfile.py
+-rw-r--r--   0        0        0     1337 2023-06-10 19:26:14.501478 lamindb_setup-0.47.4/pyproject.toml
+-rw-r--r--   0        0        0      672 2023-06-05 07:30:18.308956 lamindb_setup-0.47.4/tests/test_bionty.py
+-rw-r--r--   0        0        0     3041 2023-06-01 15:58:18.282108 lamindb_setup-0.47.4/tests/test_init_instance.py
+-rw-r--r--   0        0        0      655 2023-06-01 15:58:18.282187 lamindb_setup-0.47.4/tests/test_load_instance.py
+-rw-r--r--   0        0        0      501 2023-06-08 13:53:23.375191 lamindb_setup-0.47.4/tests/test_login.py
+-rw-r--r--   0        0        0      243 2023-06-01 15:58:18.282270 lamindb_setup-0.47.4/tests/test_set_storage.py
+-rw-r--r--   0        0        0      125 2023-06-08 13:53:23.375328 lamindb_setup-0.47.4/tests/test_signup.py
+-rw-r--r--   0        0        0     1366 1970-01-01 00:00:00.000000 lamindb_setup-0.47.4/PKG-INFO
```

### Comparing `lamindb_setup-0.47.3/.github/workflows/build.yml` & `lamindb_setup-0.47.4/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.3/.github/workflows/latest-changes.yml` & `lamindb_setup-0.47.4/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.3/.gitignore` & `lamindb_setup-0.47.4/.gitignore`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.3/.pre-commit-config.yaml` & `lamindb_setup-0.47.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.3/LICENSE` & `lamindb_setup-0.47.4/LICENSE`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.3/docs/changelog.md` & `lamindb_setup-0.47.4/docs/changelog.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Changelog
 
 <!-- prettier-ignore -->
 Name | PR | Developer | Date | Version
 --- | --- | --- | --- | ---
+🚑 Only delete bionty sources when bionty is installed | [414](https://github.com/laminlabs/lamindb-setup/pull/414) | [sunnyosun](https://github.com/sunnyosun) | 2023-06-10 | 0.47.4
 🚚 Rename source_key to source | [413](https://github.com/laminlabs/lamindb-setup/pull/413) | [sunnyosun](https://github.com/sunnyosun) | 2023-06-10 | 0.47.3
 ⬆️ Rename bionty variables | [412](https://github.com/laminlabs/lamindb-setup/pull/412) | [sunnyosun](https://github.com/sunnyosun) | 2023-06-10 | 0.47.2
 🚑 Removed `LAMINDB_INSTANCE_LOADED` env variable | [411](https://github.com/laminlabs/lamindb-setup/pull/411) | [sunnyosun](https://github.com/sunnyosun) | 2023-06-09 | 0.47.1
 ⬆️ Adapt to bionty naming in 0.18.0 | [410](https://github.com/laminlabs/lamindb-setup/pull/410) | [sunnyosun](https://github.com/sunnyosun) | 2023-06-09 |
 🚸 Warn about migrations | [409](https://github.com/laminlabs/lamindb-setup/pull/409) | [falexwolf](https://github.com/falexwolf) | 2023-06-08 | 0.47.0
 📝 Refactor guide | [408](https://github.com/laminlabs/lamindb-setup/pull/408) | [falexwolf](https://github.com/falexwolf) | 2023-06-08 |
 ✅ More testing of Bionty | [405](https://github.com/laminlabs/lamindb-setup/pull/405) | [falexwolf](https://github.com/falexwolf) | 2023-06-07 | 0.46a5
```

### Comparing `lamindb_setup-0.47.3/docs/faq/edge-cases-login-init.ipynb` & `lamindb_setup-0.47.4/docs/faq/edge-cases-login-init.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.3/docs/faq/switch-environment.ipynb` & `lamindb_setup-0.47.4/docs/faq/switch-environment.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.3/docs/faq/test-sqlite-sync.ipynb` & `lamindb_setup-0.47.4/docs/faq/test-sqlite-sync.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.3/docs/guide/01-init-instance.ipynb` & `lamindb_setup-0.47.4/docs/guide/01-init-instance.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.3/docs/guide/02-load-instance.ipynb` & `lamindb_setup-0.47.4/docs/guide/02-load-instance.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.3/docs/guide/03-set-storage.ipynb` & `lamindb_setup-0.47.4/docs/guide/03-set-storage.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.3/docs/guide/04-schema-modules.ipynb` & `lamindb_setup-0.47.4/docs/guide/04-schema-modules.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.3/docs/guide/setup-user.md` & `lamindb_setup-0.47.4/docs/guide/setup-user.md`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.3/lamindb_setup/__init__.py` & `lamindb_setup-0.47.4/lamindb_setup/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 .. autosummary::
    :toctree:
 
    dev
 """
 
 
-__version__ = "0.47.3"  # denote a release candidate for 0.1.0 with 0.1rc1
+__version__ = "0.47.4"  # denote a release candidate for 0.1.0 with 0.1rc1
 
 import builtins
 import sys
 from os import name as _os_name
 
 from . import dev
 from ._check_instance_setup import check_instance_setup as _check_instance_setup  # noqa
```

### Comparing `lamindb_setup-0.47.3/lamindb_setup/__main__.py` & `lamindb_setup-0.47.4/lamindb_setup/__main__.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.3/lamindb_setup/_check_instance_setup.py` & `lamindb_setup-0.47.4/lamindb_setup/_check_instance_setup.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.3/lamindb_setup/_close.py` & `lamindb_setup-0.47.4/lamindb_setup/_close.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.3/lamindb_setup/_delete.py` & `lamindb_setup-0.47.4/lamindb_setup/_delete.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.3/lamindb_setup/_docstrings.py` & `lamindb_setup-0.47.4/lamindb_setup/_docstrings.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.3/lamindb_setup/_init_instance.py` & `lamindb_setup-0.47.4/lamindb_setup/_init_instance.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.3/lamindb_setup/_load_instance.py` & `lamindb_setup-0.47.4/lamindb_setup/_load_instance.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.3/lamindb_setup/_notebook.py` & `lamindb_setup-0.47.4/lamindb_setup/_notebook.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.3/lamindb_setup/_register_instance.py` & `lamindb_setup-0.47.4/lamindb_setup/_register_instance.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.3/lamindb_setup/_schema.py` & `lamindb_setup-0.47.4/lamindb_setup/_schema.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.3/lamindb_setup/_set.py` & `lamindb_setup-0.47.4/lamindb_setup/_set.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.3/lamindb_setup/_settings.py` & `lamindb_setup-0.47.4/lamindb_setup/_settings.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.3/lamindb_setup/_setup_user.py` & `lamindb_setup-0.47.4/lamindb_setup/_setup_user.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.3/lamindb_setup/_silence_loggers.py` & `lamindb_setup-0.47.4/lamindb_setup/_silence_loggers.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.3/lamindb_setup/dev/_cloud_sqlite_locker.py` & `lamindb_setup-0.47.4/lamindb_setup/dev/_cloud_sqlite_locker.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.3/lamindb_setup/dev/_deprecated.py` & `lamindb_setup-0.47.4/lamindb_setup/dev/_deprecated.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.3/lamindb_setup/dev/_django.py` & `lamindb_setup-0.47.4/lamindb_setup/dev/_django.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.3/lamindb_setup/dev/_settings_instance.py` & `lamindb_setup-0.47.4/lamindb_setup/dev/_settings_instance.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.3/lamindb_setup/dev/_settings_load.py` & `lamindb_setup-0.47.4/lamindb_setup/dev/_settings_load.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.3/lamindb_setup/dev/_settings_save.py` & `lamindb_setup-0.47.4/lamindb_setup/dev/_settings_save.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.3/lamindb_setup/dev/_settings_store.py` & `lamindb_setup-0.47.4/lamindb_setup/dev/_settings_store.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.3/lamindb_setup/dev/_settings_user.py` & `lamindb_setup-0.47.4/lamindb_setup/dev/_settings_user.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.3/lamindb_setup/dev/_setup_bionty_sources.py` & `lamindb_setup-0.47.4/lamindb_setup/dev/_setup_bionty_sources.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,10 +55,13 @@
 
         write_yaml(parse_currently_used_sources(active_records), LAMINDB_SOURCES)
         logger.hint("Configured default bionty sources from BiontySource table")
 
 
 def delete_bionty_sources_yaml():
     """Delete LAMINDB_SOURCES_PATH in bionty."""
-    from bionty.dev._handle_sources import LAMINDB_SOURCES
+    try:
+        from bionty.dev._handle_sources import LAMINDB_SOURCES
 
-    LAMINDB_SOURCES.unlink(missing_ok=True)
+        LAMINDB_SOURCES.unlink(missing_ok=True)
+    except ModuleNotFoundError:
+        pass
```

### Comparing `lamindb_setup-0.47.3/lamindb_setup/dev/_setup_schema.py` & `lamindb_setup-0.47.4/lamindb_setup/dev/_setup_schema.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.3/lamindb_setup/dev/_storage.py` & `lamindb_setup-0.47.4/lamindb_setup/dev/_storage.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.3/lamindb_setup/dev/upath.py` & `lamindb_setup-0.47.4/lamindb_setup/dev/upath.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.3/lnschema-core/.github/workflows/build.yml` & `lamindb_setup-0.47.4/lnschema-core/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.3/lnschema-core/.github/workflows/latest-changes.yml` & `lamindb_setup-0.47.4/lnschema-core/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.3/lnschema-core/.gitignore` & `lamindb_setup-0.47.4/lnschema-core/.gitignore`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.3/lnschema-core/.pre-commit-config.yaml` & `lamindb_setup-0.47.4/lnschema-core/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.3/lnschema-core/LICENSE` & `lamindb_setup-0.47.4/lnschema-core/LICENSE`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.3/lnschema-core/docs/changelog.md` & `lamindb_setup-0.47.4/lnschema-core/docs/changelog.md`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.3/lnschema-core/docs/guide/core-schema.ipynb` & `lamindb_setup-0.47.4/lnschema-core/docs/guide/core-schema.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.3/lnschema-core/lnschema_core/__init__.py` & `lamindb_setup-0.47.4/lnschema-core/lnschema_core/__init__.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.3/lnschema-core/lnschema_core/_lookup.py` & `lamindb_setup-0.47.4/lnschema-core/lnschema_core/_lookup.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.3/lnschema-core/lnschema_core/_types.py` & `lamindb_setup-0.47.4/lnschema-core/lnschema_core/_types.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.3/lnschema-core/lnschema_core/ids.py` & `lamindb_setup-0.47.4/lnschema-core/lnschema_core/ids.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.3/lnschema-core/lnschema_core/migrations/0001_initial.py` & `lamindb_setup-0.47.4/lnschema-core/lnschema_core/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.3/lnschema-core/lnschema_core/models.py` & `lamindb_setup-0.47.4/lnschema-core/lnschema_core/models.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.3/lnschema-core/noxfile.py` & `lamindb_setup-0.47.4/lnschema-core/noxfile.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.3/lnschema-core/pyproject.toml` & `lamindb_setup-0.47.4/lnschema-core/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.3/noxfile.py` & `lamindb_setup-0.47.4/noxfile.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.3/pyproject.toml` & `lamindb_setup-0.47.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.3/tests/test_bionty.py` & `lamindb_setup-0.47.4/tests/test_bionty.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.3/tests/test_init_instance.py` & `lamindb_setup-0.47.4/tests/test_init_instance.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.3/tests/test_load_instance.py` & `lamindb_setup-0.47.4/tests/test_load_instance.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.3/PKG-INFO` & `lamindb_setup-0.47.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lamindb_setup
-Version: 0.47.3
+Version: 0.47.4
 Summary: LaminDB setup.
 Author-email: Lamin Labs <laminlabs@gmail.com>
 Description-Content-Type: text/markdown
 Requires-Dist: lnhub_rest==0.9.10
 Requires-Dist: sqlmodel
 Requires-Dist: lnschema_core>=0.35.4
 Requires-Dist: lamin_logger>=0.3.3
```

