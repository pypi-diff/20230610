# Comparing `tmp/winloop-0.0.3.tar.gz` & `tmp/winloop-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "winloop-0.0.3.tar", last modified: Sat Jun 10 00:19:14 2023, max compression
+gzip compressed data, was "winloop-0.0.4.tar", last modified: Sat Jun 10 00:54:10 2023, max compression
```

## Comparing `winloop-0.0.3.tar` & `winloop-0.0.4.tar`

### file list

```diff
@@ -1,96 +1,96 @@
-drwxrwxrwx   0        0        0        0 2023-06-10 00:19:14.157048 winloop-0.0.3/
--rw-rw-rw-   0        0        0    11478 2023-06-09 20:31:23.000000 winloop-0.0.3/LICENSE-APACHE
--rw-rw-rw-   0        0        0     1124 2023-06-05 05:12:27.000000 winloop-0.0.3/LICENSE-MIT
--rw-rw-rw-   0        0        0      155 2023-06-10 00:15:41.000000 winloop-0.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0     9013 2023-06-10 00:19:14.149666 winloop-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     8422 2023-06-09 20:38:45.000000 winloop-0.0.3/README.md
--rw-rw-rw-   0        0        0       42 2023-06-10 00:19:14.157048 winloop-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     2957 2023-06-10 00:18:52.000000 winloop-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-10 00:19:11.747250 winloop-0.0.3/winloop/
--rw-rw-rw-   0        0        0     1591 2023-05-19 19:29:29.000000 winloop-0.0.3/winloop/__init__.py
--rw-rw-rw-   0        0        0       88 2023-05-18 18:45:23.000000 winloop-0.0.3/winloop/_noop.py
--rw-rw-rw-   0        0        0    15429 2023-06-06 00:54:18.000000 winloop-0.0.3/winloop/_testbase.py
--rw-rw-rw-   0        0        0      789 2023-05-19 02:16:25.000000 winloop-0.0.3/winloop/cbhandles.pxd
--rw-rw-rw-   0        0        0    12547 2023-05-16 20:27:16.000000 winloop-0.0.3/winloop/cbhandles.pyx
--rw-rw-rw-   0        0        0    15105 2023-05-19 19:33:41.000000 winloop-0.0.3/winloop/dns.pyx
--rw-rw-rw-   0        0        0     3258 2023-06-01 16:31:49.000000 winloop-0.0.3/winloop/errors.pyx
-drwxrwxrwx   0        0        0        0 2023-06-10 00:19:13.496704 winloop-0.0.3/winloop/handles/
--rw-rw-rw-   0        0        0      252 2023-01-15 16:27:26.000000 winloop-0.0.3/winloop/handles/async_.pxd
--rw-rw-rw-   0        0        0     1500 2023-01-15 16:27:26.000000 winloop-0.0.3/winloop/handles/async_.pyx
--rw-rw-rw-   0        0        0     1357 2023-05-16 23:36:49.000000 winloop-0.0.3/winloop/handles/basetransport.pxd
--rw-rw-rw-   0        0        0     9553 2023-01-15 16:27:26.000000 winloop-0.0.3/winloop/handles/basetransport.pyx
--rw-rw-rw-   0        0        0      276 2023-01-15 16:27:26.000000 winloop-0.0.3/winloop/handles/check.pxd
--rw-rw-rw-   0        0        0     1865 2023-01-15 16:27:26.000000 winloop-0.0.3/winloop/handles/check.pyx
--rw-rw-rw-   0        0        0      326 2023-05-18 18:40:06.000000 winloop-0.0.3/winloop/handles/fsevent.pxd
--rw-rw-rw-   0        0        0     2842 2023-05-18 18:40:01.000000 winloop-0.0.3/winloop/handles/fsevent.pyx
--rw-rw-rw-   0        0        0     1189 2023-01-15 16:27:26.000000 winloop-0.0.3/winloop/handles/handle.pxd
--rw-rw-rw-   0        0        0    13219 2023-01-15 16:27:26.000000 winloop-0.0.3/winloop/handles/handle.pyx
--rw-rw-rw-   0        0        0      274 2023-01-15 16:27:26.000000 winloop-0.0.3/winloop/handles/idle.pxd
--rw-rw-rw-   0        0        0     1843 2023-01-15 16:27:26.000000 winloop-0.0.3/winloop/handles/idle.pyx
--rw-rw-rw-   0        0        0      999 2023-05-18 18:51:45.000000 winloop-0.0.3/winloop/handles/pipe.pxd
--rw-rw-rw-   0        0        0     7026 2023-06-01 21:07:42.000000 winloop-0.0.3/winloop/handles/pipe.pyx
--rw-rw-rw-   0        0        0      566 2023-05-17 19:12:56.000000 winloop-0.0.3/winloop/handles/poll.pxd
--rw-rw-rw-   0        0        0     6800 2023-05-27 20:29:03.000000 winloop-0.0.3/winloop/handles/poll.pyx
--rw-rw-rw-   0        0        0     2467 2023-05-31 02:16:54.000000 winloop-0.0.3/winloop/handles/process.pxd
--rw-rw-rw-   0        0        0    28304 2023-06-03 00:49:50.000000 winloop-0.0.3/winloop/handles/process.pyx
--rw-rw-rw-   0        0        0     1535 2023-01-15 16:27:26.000000 winloop-0.0.3/winloop/handles/stream.pxd
--rw-rw-rw-   0        0        0    33531 2023-06-03 18:06:42.000000 winloop-0.0.3/winloop/handles/stream.pyx
--rw-rw-rw-   0        0        0      786 2023-01-15 16:27:26.000000 winloop-0.0.3/winloop/handles/streamserver.pxd
--rw-rw-rw-   0        0        0     4650 2023-01-15 16:27:26.000000 winloop-0.0.3/winloop/handles/streamserver.pyx
--rw-rw-rw-   0        0        0     1038 2023-05-19 19:34:25.000000 winloop-0.0.3/winloop/handles/tcp.pxd
--rw-rw-rw-   0        0        0     7500 2023-05-18 18:41:59.000000 winloop-0.0.3/winloop/handles/tcp.pyx
--rw-rw-rw-   0        0        0      488 2023-05-19 02:16:51.000000 winloop-0.0.3/winloop/handles/timer.pxd
--rw-rw-rw-   0        0        0     2487 2023-05-16 20:31:22.000000 winloop-0.0.3/winloop/handles/timer.pyx
--rw-rw-rw-   0        0        0      704 2023-05-18 18:44:00.000000 winloop-0.0.3/winloop/handles/udp.pxd
--rw-rw-rw-   0        0        0    12035 2023-05-10 19:07:46.000000 winloop-0.0.3/winloop/handles/udp.pyx
-drwxrwxrwx   0        0        0        0 2023-06-10 00:19:13.770486 winloop-0.0.3/winloop/includes/
--rw-rw-rw-   0        0        0      361 2023-01-15 16:27:26.000000 winloop-0.0.3/winloop/includes/__init__.py
--rw-rw-rw-   0        0        0      819 2023-05-27 18:58:15.000000 winloop-0.0.3/winloop/includes/_python.pxd
--rw-rw-rw-   0        0        0     6963 2023-06-04 22:27:27.000000 winloop-0.0.3/winloop/includes/_stdlib.pxi
--rw-rw-rw-   0        0        0      687 2023-01-15 16:27:26.000000 winloop-0.0.3/winloop/includes/consts.pxi
--rw-rw-rw-   0        0        0      717 2023-05-21 02:39:56.000000 winloop-0.0.3/winloop/includes/context.h
--rw-rw-rw-   0        0        0       51 2023-05-19 02:33:37.000000 winloop-0.0.3/winloop/includes/debug.h
--rw-rw-rw-   0        0        0       63 2023-05-16 20:46:46.000000 winloop-0.0.3/winloop/includes/debug.pxd
--rw-rw-rw-   0        0        0      459 2023-05-16 23:34:31.000000 winloop-0.0.3/winloop/includes/flowcontrol.pxd
--rw-rw-rw-   0        0        0      425 2023-06-02 01:05:27.000000 winloop-0.0.3/winloop/includes/nfork_handler.h
--rw-rw-rw-   0        0        0     7013 2023-06-02 02:09:18.000000 winloop-0.0.3/winloop/includes/socketpair.h
--rw-rw-rw-   0        0        0     3002 2023-06-02 01:53:51.000000 winloop-0.0.3/winloop/includes/system.pxd
--rw-rw-rw-   0        0        0      670 2023-06-03 00:25:11.000000 winloop-0.0.3/winloop/includes/tcp.h
--rw-rw-rw-   0        0        0    18436 2023-06-03 18:23:26.000000 winloop-0.0.3/winloop/includes/uv.pxd
--rw-rw-rw-   0        0        0  7297948 2023-06-09 20:16:02.000000 winloop-0.0.3/winloop/loop.c
--rw-rw-rw-   0        0        0     6431 2023-06-05 17:57:17.000000 winloop-0.0.3/winloop/loop.pxd
--rw-rw-rw-   0        0        0    10449 2023-01-15 16:27:26.000000 winloop-0.0.3/winloop/loop.pyi
--rw-rw-rw-   0        0        0   121804 2023-06-05 00:13:20.000000 winloop-0.0.3/winloop/loop.pyx
--rw-rw-rw-   0        0        0     2423 2023-05-18 18:55:24.000000 winloop-0.0.3/winloop/lru.pyx
--rw-rw-rw-   0        0        0     5383 2023-01-15 16:27:26.000000 winloop-0.0.3/winloop/pseudosock.pyx
--rw-rw-rw-   0        0        0      145 2023-05-18 18:43:09.000000 winloop-0.0.3/winloop/request.pxd
--rw-rw-rw-   0        0        0     2415 2023-05-18 18:43:19.000000 winloop-0.0.3/winloop/request.pyx
--rw-rw-rw-   0        0        0      394 2023-01-15 16:27:26.000000 winloop-0.0.3/winloop/server.pxd
--rw-rw-rw-   0        0        0     3623 2023-01-15 16:27:26.000000 winloop-0.0.3/winloop/server.pyx
--rw-rw-rw-   0        0        0     3534 2023-05-16 23:33:29.000000 winloop-0.0.3/winloop/sslproto.pxd
--rw-rw-rw-   0        0        0    35914 2023-05-16 23:33:44.000000 winloop-0.0.3/winloop/sslproto.pyx
-drwxrwxrwx   0        0        0        0 2023-06-10 00:19:13.791486 winloop-0.0.3/winloop/vendor/
-drwxrwxrwx   0        0        0        0 2023-06-10 00:19:13.810487 winloop-0.0.3/winloop/vendor/include/
-drwxrwxrwx   0        0        0        0 2023-06-10 00:19:14.141666 winloop-0.0.3/winloop/vendor/include/uv/
--rw-rw-rw-   0        0        0     1615 2022-07-12 16:16:33.000000 winloop-0.0.3/winloop/vendor/include/uv/aix.h
--rw-rw-rw-   0        0        0     1641 2022-07-12 16:16:33.000000 winloop-0.0.3/winloop/vendor/include/uv/bsd.h
--rw-rw-rw-   0        0        0     3213 2022-07-12 16:16:33.000000 winloop-0.0.3/winloop/vendor/include/uv/darwin.h
--rw-rw-rw-   0        0        0    10643 2022-07-12 16:16:33.000000 winloop-0.0.3/winloop/vendor/include/uv/errno.h
--rw-rw-rw-   0        0        0     1781 2022-07-12 16:16:33.000000 winloop-0.0.3/winloop/vendor/include/uv/linux.h
--rw-rw-rw-   0        0        0     1553 2022-07-12 16:16:33.000000 winloop-0.0.3/winloop/vendor/include/uv/os390.h
--rw-rw-rw-   0        0        0     1606 2022-07-12 16:16:33.000000 winloop-0.0.3/winloop/vendor/include/uv/posix.h
--rw-rw-rw-   0        0        0     7728 2022-07-12 16:16:33.000000 winloop-0.0.3/winloop/vendor/include/uv/stdint-msvc2008.h
--rw-rw-rw-   0        0        0     1985 2022-07-12 16:16:33.000000 winloop-0.0.3/winloop/vendor/include/uv/sunos.h
--rw-rw-rw-   0        0        0     1497 2022-07-12 16:16:33.000000 winloop-0.0.3/winloop/vendor/include/uv/threadpool.h
--rw-rw-rw-   0        0        0    52889 2022-07-12 16:16:33.000000 winloop-0.0.3/winloop/vendor/include/uv/tree.h
--rw-rw-rw-   0        0        0    19504 2022-07-12 16:16:33.000000 winloop-0.0.3/winloop/vendor/include/uv/unix.h
--rw-rw-rw-   0        0        0     1831 2022-07-12 16:16:33.000000 winloop-0.0.3/winloop/vendor/include/uv/version.h
--rw-rw-rw-   0        0        0    33252 2022-07-12 16:16:33.000000 winloop-0.0.3/winloop/vendor/include/uv/win.h
--rw-rw-rw-   0        0        0    67239 2022-07-12 16:16:33.000000 winloop-0.0.3/winloop/vendor/include/uv.h
--rw-rw-rw-   0        0        0   728242 2023-02-28 22:32:41.000000 winloop-0.0.3/winloop/vendor/uv_a.lib
-drwxrwxrwx   0        0        0        0 2023-06-10 00:19:12.333113 winloop-0.0.3/winloop.egg-info/
--rw-rw-rw-   0        0        0     9013 2023-06-10 00:19:09.000000 winloop-0.0.3/winloop.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2234 2023-06-10 00:19:10.000000 winloop-0.0.3/winloop.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-10 00:19:09.000000 winloop-0.0.3/winloop.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-06-10 00:19:09.000000 winloop-0.0.3/winloop.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-10 00:19:09.000000 winloop-0.0.3/winloop.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-10 00:54:10.215541 winloop-0.0.4/
+-rw-rw-rw-   0        0        0    11478 2023-06-09 20:31:23.000000 winloop-0.0.4/LICENSE-APACHE
+-rw-rw-rw-   0        0        0     1124 2023-06-05 05:12:27.000000 winloop-0.0.4/LICENSE-MIT
+-rw-rw-rw-   0        0        0      155 2023-06-10 00:15:41.000000 winloop-0.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     9013 2023-06-10 00:54:10.213542 winloop-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     8422 2023-06-09 20:38:45.000000 winloop-0.0.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-10 00:54:10.216541 winloop-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     2993 2023-06-10 00:51:40.000000 winloop-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-10 00:54:07.999487 winloop-0.0.4/winloop/
+-rw-rw-rw-   0        0        0     1591 2023-05-19 19:29:29.000000 winloop-0.0.4/winloop/__init__.py
+-rw-rw-rw-   0        0        0       88 2023-05-18 18:45:23.000000 winloop-0.0.4/winloop/_noop.py
+-rw-rw-rw-   0        0        0    15429 2023-06-06 00:54:18.000000 winloop-0.0.4/winloop/_testbase.py
+-rw-rw-rw-   0        0        0      789 2023-05-19 02:16:25.000000 winloop-0.0.4/winloop/cbhandles.pxd
+-rw-rw-rw-   0        0        0    12547 2023-05-16 20:27:16.000000 winloop-0.0.4/winloop/cbhandles.pyx
+-rw-rw-rw-   0        0        0    15105 2023-05-19 19:33:41.000000 winloop-0.0.4/winloop/dns.pyx
+-rw-rw-rw-   0        0        0     3258 2023-06-01 16:31:49.000000 winloop-0.0.4/winloop/errors.pyx
+drwxrwxrwx   0        0        0        0 2023-06-10 00:54:08.798893 winloop-0.0.4/winloop/handles/
+-rw-rw-rw-   0        0        0      252 2023-01-15 16:27:26.000000 winloop-0.0.4/winloop/handles/async_.pxd
+-rw-rw-rw-   0        0        0     1500 2023-01-15 16:27:26.000000 winloop-0.0.4/winloop/handles/async_.pyx
+-rw-rw-rw-   0        0        0     1357 2023-05-16 23:36:49.000000 winloop-0.0.4/winloop/handles/basetransport.pxd
+-rw-rw-rw-   0        0        0     9553 2023-01-15 16:27:26.000000 winloop-0.0.4/winloop/handles/basetransport.pyx
+-rw-rw-rw-   0        0        0      276 2023-01-15 16:27:26.000000 winloop-0.0.4/winloop/handles/check.pxd
+-rw-rw-rw-   0        0        0     1865 2023-01-15 16:27:26.000000 winloop-0.0.4/winloop/handles/check.pyx
+-rw-rw-rw-   0        0        0      326 2023-05-18 18:40:06.000000 winloop-0.0.4/winloop/handles/fsevent.pxd
+-rw-rw-rw-   0        0        0     2842 2023-05-18 18:40:01.000000 winloop-0.0.4/winloop/handles/fsevent.pyx
+-rw-rw-rw-   0        0        0     1189 2023-01-15 16:27:26.000000 winloop-0.0.4/winloop/handles/handle.pxd
+-rw-rw-rw-   0        0        0    13219 2023-01-15 16:27:26.000000 winloop-0.0.4/winloop/handles/handle.pyx
+-rw-rw-rw-   0        0        0      274 2023-01-15 16:27:26.000000 winloop-0.0.4/winloop/handles/idle.pxd
+-rw-rw-rw-   0        0        0     1843 2023-01-15 16:27:26.000000 winloop-0.0.4/winloop/handles/idle.pyx
+-rw-rw-rw-   0        0        0      999 2023-05-18 18:51:45.000000 winloop-0.0.4/winloop/handles/pipe.pxd
+-rw-rw-rw-   0        0        0     7026 2023-06-01 21:07:42.000000 winloop-0.0.4/winloop/handles/pipe.pyx
+-rw-rw-rw-   0        0        0      566 2023-05-17 19:12:56.000000 winloop-0.0.4/winloop/handles/poll.pxd
+-rw-rw-rw-   0        0        0     6800 2023-05-27 20:29:03.000000 winloop-0.0.4/winloop/handles/poll.pyx
+-rw-rw-rw-   0        0        0     2467 2023-05-31 02:16:54.000000 winloop-0.0.4/winloop/handles/process.pxd
+-rw-rw-rw-   0        0        0    28304 2023-06-03 00:49:50.000000 winloop-0.0.4/winloop/handles/process.pyx
+-rw-rw-rw-   0        0        0     1535 2023-01-15 16:27:26.000000 winloop-0.0.4/winloop/handles/stream.pxd
+-rw-rw-rw-   0        0        0    33531 2023-06-03 18:06:42.000000 winloop-0.0.4/winloop/handles/stream.pyx
+-rw-rw-rw-   0        0        0      786 2023-01-15 16:27:26.000000 winloop-0.0.4/winloop/handles/streamserver.pxd
+-rw-rw-rw-   0        0        0     4650 2023-01-15 16:27:26.000000 winloop-0.0.4/winloop/handles/streamserver.pyx
+-rw-rw-rw-   0        0        0     1038 2023-05-19 19:34:25.000000 winloop-0.0.4/winloop/handles/tcp.pxd
+-rw-rw-rw-   0        0        0     7500 2023-05-18 18:41:59.000000 winloop-0.0.4/winloop/handles/tcp.pyx
+-rw-rw-rw-   0        0        0      488 2023-05-19 02:16:51.000000 winloop-0.0.4/winloop/handles/timer.pxd
+-rw-rw-rw-   0        0        0     2487 2023-05-16 20:31:22.000000 winloop-0.0.4/winloop/handles/timer.pyx
+-rw-rw-rw-   0        0        0      704 2023-05-18 18:44:00.000000 winloop-0.0.4/winloop/handles/udp.pxd
+-rw-rw-rw-   0        0        0    12035 2023-05-10 19:07:46.000000 winloop-0.0.4/winloop/handles/udp.pyx
+drwxrwxrwx   0        0        0        0 2023-06-10 00:54:09.274523 winloop-0.0.4/winloop/includes/
+-rw-rw-rw-   0        0        0      361 2023-01-15 16:27:26.000000 winloop-0.0.4/winloop/includes/__init__.py
+-rw-rw-rw-   0        0        0      819 2023-05-27 18:58:15.000000 winloop-0.0.4/winloop/includes/_python.pxd
+-rw-rw-rw-   0        0        0     6963 2023-06-04 22:27:27.000000 winloop-0.0.4/winloop/includes/_stdlib.pxi
+-rw-rw-rw-   0        0        0      687 2023-01-15 16:27:26.000000 winloop-0.0.4/winloop/includes/consts.pxi
+-rw-rw-rw-   0        0        0      717 2023-05-21 02:39:56.000000 winloop-0.0.4/winloop/includes/context.h
+-rw-rw-rw-   0        0        0       51 2023-05-19 02:33:37.000000 winloop-0.0.4/winloop/includes/debug.h
+-rw-rw-rw-   0        0        0       63 2023-05-16 20:46:46.000000 winloop-0.0.4/winloop/includes/debug.pxd
+-rw-rw-rw-   0        0        0      459 2023-05-16 23:34:31.000000 winloop-0.0.4/winloop/includes/flowcontrol.pxd
+-rw-rw-rw-   0        0        0      425 2023-06-02 01:05:27.000000 winloop-0.0.4/winloop/includes/nfork_handler.h
+-rw-rw-rw-   0        0        0     7013 2023-06-02 02:09:18.000000 winloop-0.0.4/winloop/includes/socketpair.h
+-rw-rw-rw-   0        0        0     3002 2023-06-02 01:53:51.000000 winloop-0.0.4/winloop/includes/system.pxd
+-rw-rw-rw-   0        0        0      670 2023-06-03 00:25:11.000000 winloop-0.0.4/winloop/includes/tcp.h
+-rw-rw-rw-   0        0        0    18436 2023-06-03 18:23:26.000000 winloop-0.0.4/winloop/includes/uv.pxd
+-rw-rw-rw-   0        0        0  7297948 2023-06-09 20:16:02.000000 winloop-0.0.4/winloop/loop.c
+-rw-rw-rw-   0        0        0     6431 2023-06-05 17:57:17.000000 winloop-0.0.4/winloop/loop.pxd
+-rw-rw-rw-   0        0        0    10449 2023-01-15 16:27:26.000000 winloop-0.0.4/winloop/loop.pyi
+-rw-rw-rw-   0        0        0   121804 2023-06-05 00:13:20.000000 winloop-0.0.4/winloop/loop.pyx
+-rw-rw-rw-   0        0        0     2423 2023-05-18 18:55:24.000000 winloop-0.0.4/winloop/lru.pyx
+-rw-rw-rw-   0        0        0     5383 2023-01-15 16:27:26.000000 winloop-0.0.4/winloop/pseudosock.pyx
+-rw-rw-rw-   0        0        0      145 2023-05-18 18:43:09.000000 winloop-0.0.4/winloop/request.pxd
+-rw-rw-rw-   0        0        0     2415 2023-05-18 18:43:19.000000 winloop-0.0.4/winloop/request.pyx
+-rw-rw-rw-   0        0        0      394 2023-01-15 16:27:26.000000 winloop-0.0.4/winloop/server.pxd
+-rw-rw-rw-   0        0        0     3623 2023-01-15 16:27:26.000000 winloop-0.0.4/winloop/server.pyx
+-rw-rw-rw-   0        0        0     3534 2023-05-16 23:33:29.000000 winloop-0.0.4/winloop/sslproto.pxd
+-rw-rw-rw-   0        0        0    35914 2023-05-16 23:33:44.000000 winloop-0.0.4/winloop/sslproto.pyx
+drwxrwxrwx   0        0        0        0 2023-06-10 00:54:09.332523 winloop-0.0.4/winloop/vendor/
+drwxrwxrwx   0        0        0        0 2023-06-10 00:54:09.535522 winloop-0.0.4/winloop/vendor/include/
+drwxrwxrwx   0        0        0        0 2023-06-10 00:54:10.188383 winloop-0.0.4/winloop/vendor/include/uv/
+-rw-rw-rw-   0        0        0     1615 2022-07-12 16:16:33.000000 winloop-0.0.4/winloop/vendor/include/uv/aix.h
+-rw-rw-rw-   0        0        0     1641 2022-07-12 16:16:33.000000 winloop-0.0.4/winloop/vendor/include/uv/bsd.h
+-rw-rw-rw-   0        0        0     3213 2022-07-12 16:16:33.000000 winloop-0.0.4/winloop/vendor/include/uv/darwin.h
+-rw-rw-rw-   0        0        0    10643 2022-07-12 16:16:33.000000 winloop-0.0.4/winloop/vendor/include/uv/errno.h
+-rw-rw-rw-   0        0        0     1781 2022-07-12 16:16:33.000000 winloop-0.0.4/winloop/vendor/include/uv/linux.h
+-rw-rw-rw-   0        0        0     1553 2022-07-12 16:16:33.000000 winloop-0.0.4/winloop/vendor/include/uv/os390.h
+-rw-rw-rw-   0        0        0     1606 2022-07-12 16:16:33.000000 winloop-0.0.4/winloop/vendor/include/uv/posix.h
+-rw-rw-rw-   0        0        0     7728 2022-07-12 16:16:33.000000 winloop-0.0.4/winloop/vendor/include/uv/stdint-msvc2008.h
+-rw-rw-rw-   0        0        0     1985 2022-07-12 16:16:33.000000 winloop-0.0.4/winloop/vendor/include/uv/sunos.h
+-rw-rw-rw-   0        0        0     1497 2022-07-12 16:16:33.000000 winloop-0.0.4/winloop/vendor/include/uv/threadpool.h
+-rw-rw-rw-   0        0        0    52889 2022-07-12 16:16:33.000000 winloop-0.0.4/winloop/vendor/include/uv/tree.h
+-rw-rw-rw-   0        0        0    19504 2022-07-12 16:16:33.000000 winloop-0.0.4/winloop/vendor/include/uv/unix.h
+-rw-rw-rw-   0        0        0     1831 2022-07-12 16:16:33.000000 winloop-0.0.4/winloop/vendor/include/uv/version.h
+-rw-rw-rw-   0        0        0    33252 2022-07-12 16:16:33.000000 winloop-0.0.4/winloop/vendor/include/uv/win.h
+-rw-rw-rw-   0        0        0    67239 2022-07-12 16:16:33.000000 winloop-0.0.4/winloop/vendor/include/uv.h
+-rw-rw-rw-   0        0        0   728242 2023-02-28 22:32:41.000000 winloop-0.0.4/winloop/vendor/uv_a.lib
+drwxrwxrwx   0        0        0        0 2023-06-10 00:54:08.075935 winloop-0.0.4/winloop.egg-info/
+-rw-rw-rw-   0        0        0     9013 2023-06-10 00:54:06.000000 winloop-0.0.4/winloop.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2234 2023-06-10 00:54:06.000000 winloop-0.0.4/winloop.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-10 00:54:06.000000 winloop-0.0.4/winloop.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-06-10 00:54:06.000000 winloop-0.0.4/winloop.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-10 00:54:06.000000 winloop-0.0.4/winloop.egg-info/top_level.txt
```

### Comparing `winloop-0.0.3/LICENSE-APACHE` & `winloop-0.0.4/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `winloop-0.0.3/LICENSE-MIT` & `winloop-0.0.4/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `winloop-0.0.3/PKG-INFO` & `winloop-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: winloop
-Version: 0.0.3
+Version: 0.0.4
 Summary: An Alternative library for uvloop compatability with windows
 Author: Vizonex
 License: MIT
 Keywords: winloop,libuv,windows,cython,fast-asyncio,uvloop-alternative
 Platform: Microsoft Windows
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `winloop-0.0.3/README.md` & `winloop-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `winloop-0.0.3/setup.py` & `winloop-0.0.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     print("please install cython first")
     sys.exit(1)
 
 
 
 HERE = pathlib.Path("winloop")
 
-__version__ = "0.0.3"
+__version__ = "0.0.4"
 
 
 
 # This is a temporary test Solution and is not the official file yet but this is to display/show what 
 # I'm currently using to compile the winloop library...
 def do_installation():
     try:
@@ -64,14 +64,15 @@
             "winloop", 
             "libuv", 
             "windows", 
             "cython",
             "fast-asyncio",
             "uvloop-alternative"
         ],
+        include_package_data=True,
         long_description_content_type='text/markdown',
         long_description=long_description,
         classifiers=[
             'Programming Language :: Python :: 3.9',
             'Programming Language :: Python :: 3.10',
             'Programming Language :: Python :: 3.11',
             'Intended Audience :: Developers',
```

### Comparing `winloop-0.0.3/winloop/__init__.py` & `winloop-0.0.4/winloop/__init__.py`

 * *Files identical despite different names*

### Comparing `winloop-0.0.3/winloop/_testbase.py` & `winloop-0.0.4/winloop/_testbase.py`

 * *Files identical despite different names*

### Comparing `winloop-0.0.3/winloop/cbhandles.pxd` & `winloop-0.0.4/winloop/cbhandles.pxd`

 * *Files identical despite different names*

### Comparing `winloop-0.0.3/winloop/cbhandles.pyx` & `winloop-0.0.4/winloop/cbhandles.pyx`

 * *Files identical despite different names*

### Comparing `winloop-0.0.3/winloop/dns.pyx` & `winloop-0.0.4/winloop/dns.pyx`

 * *Files identical despite different names*

### Comparing `winloop-0.0.3/winloop/errors.pyx` & `winloop-0.0.4/winloop/errors.pyx`

 * *Files identical despite different names*

### Comparing `winloop-0.0.3/winloop/handles/async_.pyx` & `winloop-0.0.4/winloop/handles/async_.pyx`

 * *Files identical despite different names*

### Comparing `winloop-0.0.3/winloop/handles/basetransport.pxd` & `winloop-0.0.4/winloop/handles/basetransport.pxd`

 * *Files identical despite different names*

### Comparing `winloop-0.0.3/winloop/handles/basetransport.pyx` & `winloop-0.0.4/winloop/handles/basetransport.pyx`

 * *Files identical despite different names*

### Comparing `winloop-0.0.3/winloop/handles/check.pyx` & `winloop-0.0.4/winloop/handles/check.pyx`

 * *Files identical despite different names*

### Comparing `winloop-0.0.3/winloop/handles/fsevent.pyx` & `winloop-0.0.4/winloop/handles/fsevent.pyx`

 * *Files identical despite different names*

### Comparing `winloop-0.0.3/winloop/handles/handle.pxd` & `winloop-0.0.4/winloop/handles/handle.pxd`

 * *Files identical despite different names*

### Comparing `winloop-0.0.3/winloop/handles/handle.pyx` & `winloop-0.0.4/winloop/handles/handle.pyx`

 * *Files identical despite different names*

### Comparing `winloop-0.0.3/winloop/handles/idle.pyx` & `winloop-0.0.4/winloop/handles/idle.pyx`

 * *Files identical despite different names*

### Comparing `winloop-0.0.3/winloop/handles/pipe.pxd` & `winloop-0.0.4/winloop/handles/pipe.pxd`

 * *Files identical despite different names*

### Comparing `winloop-0.0.3/winloop/handles/pipe.pyx` & `winloop-0.0.4/winloop/handles/pipe.pyx`

 * *Files identical despite different names*

### Comparing `winloop-0.0.3/winloop/handles/poll.pxd` & `winloop-0.0.4/winloop/handles/poll.pxd`

 * *Files identical despite different names*

### Comparing `winloop-0.0.3/winloop/handles/poll.pyx` & `winloop-0.0.4/winloop/handles/poll.pyx`

 * *Files identical despite different names*

### Comparing `winloop-0.0.3/winloop/handles/process.pxd` & `winloop-0.0.4/winloop/handles/process.pxd`

 * *Files identical despite different names*

### Comparing `winloop-0.0.3/winloop/handles/process.pyx` & `winloop-0.0.4/winloop/handles/process.pyx`

 * *Files identical despite different names*

### Comparing `winloop-0.0.3/winloop/handles/stream.pxd` & `winloop-0.0.4/winloop/handles/stream.pxd`

 * *Files identical despite different names*

### Comparing `winloop-0.0.3/winloop/handles/stream.pyx` & `winloop-0.0.4/winloop/handles/stream.pyx`

 * *Files identical despite different names*

### Comparing `winloop-0.0.3/winloop/handles/streamserver.pxd` & `winloop-0.0.4/winloop/handles/streamserver.pxd`

 * *Files identical despite different names*

### Comparing `winloop-0.0.3/winloop/handles/streamserver.pyx` & `winloop-0.0.4/winloop/handles/streamserver.pyx`

 * *Files identical despite different names*

### Comparing `winloop-0.0.3/winloop/handles/tcp.pxd` & `winloop-0.0.4/winloop/handles/tcp.pxd`

 * *Files identical despite different names*

### Comparing `winloop-0.0.3/winloop/handles/tcp.pyx` & `winloop-0.0.4/winloop/handles/tcp.pyx`

 * *Files identical despite different names*

### Comparing `winloop-0.0.3/winloop/handles/timer.pyx` & `winloop-0.0.4/winloop/handles/timer.pyx`

 * *Files identical despite different names*

### Comparing `winloop-0.0.3/winloop/handles/udp.pxd` & `winloop-0.0.4/winloop/handles/udp.pxd`

 * *Files identical despite different names*

### Comparing `winloop-0.0.3/winloop/handles/udp.pyx` & `winloop-0.0.4/winloop/handles/udp.pyx`

 * *Files identical despite different names*

### Comparing `winloop-0.0.3/winloop/includes/_python.pxd` & `winloop-0.0.4/winloop/includes/_python.pxd`

 * *Files identical despite different names*

### Comparing `winloop-0.0.3/winloop/includes/_stdlib.pxi` & `winloop-0.0.4/winloop/includes/_stdlib.pxi`

 * *Files identical despite different names*

### Comparing `winloop-0.0.3/winloop/includes/consts.pxi` & `winloop-0.0.4/winloop/includes/consts.pxi`

 * *Files identical despite different names*

### Comparing `winloop-0.0.3/winloop/includes/context.h` & `winloop-0.0.4/winloop/includes/context.h`

 * *Files identical despite different names*

### Comparing `winloop-0.0.3/winloop/includes/socketpair.h` & `winloop-0.0.4/winloop/includes/socketpair.h`

 * *Files identical despite different names*

### Comparing `winloop-0.0.3/winloop/includes/system.pxd` & `winloop-0.0.4/winloop/includes/system.pxd`

 * *Files identical despite different names*

### Comparing `winloop-0.0.3/winloop/includes/tcp.h` & `winloop-0.0.4/winloop/includes/tcp.h`

 * *Files identical despite different names*

### Comparing `winloop-0.0.3/winloop/includes/uv.pxd` & `winloop-0.0.4/winloop/includes/uv.pxd`

 * *Files identical despite different names*

### Comparing `winloop-0.0.3/winloop/loop.c` & `winloop-0.0.4/winloop/loop.c`

 * *Files identical despite different names*

### Comparing `winloop-0.0.3/winloop/loop.pxd` & `winloop-0.0.4/winloop/loop.pxd`

 * *Files identical despite different names*

### Comparing `winloop-0.0.3/winloop/loop.pyi` & `winloop-0.0.4/winloop/loop.pyi`

 * *Files identical despite different names*

### Comparing `winloop-0.0.3/winloop/loop.pyx` & `winloop-0.0.4/winloop/loop.pyx`

 * *Files identical despite different names*

### Comparing `winloop-0.0.3/winloop/lru.pyx` & `winloop-0.0.4/winloop/lru.pyx`

 * *Files identical despite different names*

### Comparing `winloop-0.0.3/winloop/pseudosock.pyx` & `winloop-0.0.4/winloop/pseudosock.pyx`

 * *Files identical despite different names*

### Comparing `winloop-0.0.3/winloop/request.pyx` & `winloop-0.0.4/winloop/request.pyx`

 * *Files identical despite different names*

### Comparing `winloop-0.0.3/winloop/server.pyx` & `winloop-0.0.4/winloop/server.pyx`

 * *Files identical despite different names*

### Comparing `winloop-0.0.3/winloop/sslproto.pxd` & `winloop-0.0.4/winloop/sslproto.pxd`

 * *Files identical despite different names*

### Comparing `winloop-0.0.3/winloop/sslproto.pyx` & `winloop-0.0.4/winloop/sslproto.pyx`

 * *Files identical despite different names*

### Comparing `winloop-0.0.3/winloop/vendor/include/uv/aix.h` & `winloop-0.0.4/winloop/vendor/include/uv/aix.h`

 * *Files identical despite different names*

### Comparing `winloop-0.0.3/winloop/vendor/include/uv/bsd.h` & `winloop-0.0.4/winloop/vendor/include/uv/bsd.h`

 * *Files identical despite different names*

### Comparing `winloop-0.0.3/winloop/vendor/include/uv/darwin.h` & `winloop-0.0.4/winloop/vendor/include/uv/darwin.h`

 * *Files identical despite different names*

### Comparing `winloop-0.0.3/winloop/vendor/include/uv/errno.h` & `winloop-0.0.4/winloop/vendor/include/uv/errno.h`

 * *Files identical despite different names*

### Comparing `winloop-0.0.3/winloop/vendor/include/uv/linux.h` & `winloop-0.0.4/winloop/vendor/include/uv/linux.h`

 * *Files identical despite different names*

### Comparing `winloop-0.0.3/winloop/vendor/include/uv/os390.h` & `winloop-0.0.4/winloop/vendor/include/uv/os390.h`

 * *Files identical despite different names*

### Comparing `winloop-0.0.3/winloop/vendor/include/uv/posix.h` & `winloop-0.0.4/winloop/vendor/include/uv/posix.h`

 * *Files identical despite different names*

### Comparing `winloop-0.0.3/winloop/vendor/include/uv/stdint-msvc2008.h` & `winloop-0.0.4/winloop/vendor/include/uv/stdint-msvc2008.h`

 * *Files identical despite different names*

### Comparing `winloop-0.0.3/winloop/vendor/include/uv/sunos.h` & `winloop-0.0.4/winloop/vendor/include/uv/sunos.h`

 * *Files identical despite different names*

### Comparing `winloop-0.0.3/winloop/vendor/include/uv/threadpool.h` & `winloop-0.0.4/winloop/vendor/include/uv/threadpool.h`

 * *Files identical despite different names*

### Comparing `winloop-0.0.3/winloop/vendor/include/uv/tree.h` & `winloop-0.0.4/winloop/vendor/include/uv/tree.h`

 * *Files identical despite different names*

### Comparing `winloop-0.0.3/winloop/vendor/include/uv/unix.h` & `winloop-0.0.4/winloop/vendor/include/uv/unix.h`

 * *Files identical despite different names*

### Comparing `winloop-0.0.3/winloop/vendor/include/uv/version.h` & `winloop-0.0.4/winloop/vendor/include/uv/version.h`

 * *Files identical despite different names*

### Comparing `winloop-0.0.3/winloop/vendor/include/uv/win.h` & `winloop-0.0.4/winloop/vendor/include/uv/win.h`

 * *Files identical despite different names*

### Comparing `winloop-0.0.3/winloop/vendor/include/uv.h` & `winloop-0.0.4/winloop/vendor/include/uv.h`

 * *Files identical despite different names*

### Comparing `winloop-0.0.3/winloop/vendor/uv_a.lib` & `winloop-0.0.4/winloop/vendor/uv_a.lib`

 * *Files identical despite different names*

### Comparing `winloop-0.0.3/winloop.egg-info/PKG-INFO` & `winloop-0.0.4/winloop.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: winloop
-Version: 0.0.3
+Version: 0.0.4
 Summary: An Alternative library for uvloop compatability with windows
 Author: Vizonex
 License: MIT
 Keywords: winloop,libuv,windows,cython,fast-asyncio,uvloop-alternative
 Platform: Microsoft Windows
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `winloop-0.0.3/winloop.egg-info/SOURCES.txt` & `winloop-0.0.4/winloop.egg-info/SOURCES.txt`

 * *Files identical despite different names*

