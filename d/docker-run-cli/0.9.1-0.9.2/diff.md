# Comparing `tmp/docker-run-cli-0.9.1.tar.gz` & `tmp/docker-run-cli-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/work/data01/reiher/git/ops/docker-run/docker-run/dist/.tmp-2azkfucz/docker-run-cli-0.9.1.tar", last modified: Tue May 30 10:53:29 2023, max compression
+gzip compressed data, was "/work/data01/reiher/git/ops/docker-run/docker-run/dist/.tmp-a2_n4ilg/docker-run-cli-0.9.2.tar", last modified: Sat Jun 10 17:15:52 2023, max compression
```

## Comparing `docker-run-cli-0.9.1.tar` & `docker-run-cli-0.9.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwsr-x   0 reiher   (16171) fb-5     (12389)        0 2023-05-30 10:53:29.000000 docker-run-cli-0.9.1/
--rw-rw-r--   0 reiher   (16171) fb-5     (12389)     1123 2023-05-29 13:04:51.000000 docker-run-cli-0.9.1/LICENSE
--rw-rw-r--   0 reiher   (16171) fb-5     (12389)       51 2023-05-29 13:04:41.000000 docker-run-cli-0.9.1/MANIFEST.in
--rw-rw-r--   0 reiher   (16171) fb-5     (12389)     7348 2023-05-30 10:53:29.000000 docker-run-cli-0.9.1/PKG-INFO
--rw-rw-r--   0 reiher   (16171) fb-5     (12389)     5151 2023-05-30 10:21:45.000000 docker-run-cli-0.9.1/README.md
--rw-rw-r--   0 reiher   (16171) fb-5     (12389)     1420 2023-05-30 10:51:17.000000 docker-run-cli-0.9.1/pyproject.toml
-drwxrwsr-x   0 reiher   (16171) fb-5     (12389)        0 2023-05-30 10:53:29.000000 docker-run-cli-0.9.1/scripts/
--rwxrwxr-x   0 reiher   (16171) fb-5     (12389)     1620 2023-05-29 13:04:41.000000 docker-run-cli-0.9.1/scripts/activate-python-docker-run-shell-completion
--rwxrwxr-x   0 reiher   (16171) fb-5     (12389)     1102 2023-05-29 13:04:41.000000 docker-run-cli-0.9.1/scripts/docker-run
--rw-rw-r--   0 reiher   (16171) fb-5     (12389)       38 2023-05-30 10:53:29.000000 docker-run-cli-0.9.1/setup.cfg
-drwxrwsr-x   0 reiher   (16171) fb-5     (12389)        0 2023-05-30 10:53:29.000000 docker-run-cli-0.9.1/src/
-drwxrwsr-x   0 reiher   (16171) fb-5     (12389)        0 2023-05-30 10:53:29.000000 docker-run-cli-0.9.1/src/docker_run/
--rw-rw-r--   0 reiher   (16171) fb-5     (12389)       45 2023-05-30 10:51:33.000000 docker-run-cli-0.9.1/src/docker_run/__init__.py
--rw-rw-r--   0 reiher   (16171) fb-5     (12389)      107 2023-05-29 13:04:41.000000 docker-run-cli-0.9.1/src/docker_run/__main__.py
-drwxrwsr-x   0 reiher   (16171) fb-5     (12389)        0 2023-05-30 10:53:29.000000 docker-run-cli-0.9.1/src/docker_run/bash_completion.d/
--rw-rw-r--   0 reiher   (16171) fb-5     (12389)     2886 2023-05-29 13:04:41.000000 docker-run-cli-0.9.1/src/docker_run/bash_completion.d/docker-run
--rw-rw-r--   0 reiher   (16171) fb-5     (12389)     6110 2023-05-29 13:04:41.000000 docker-run-cli-0.9.1/src/docker_run/core.py
-drwxrwsr-x   0 reiher   (16171) fb-5     (12389)        0 2023-05-30 10:53:29.000000 docker-run-cli-0.9.1/src/docker_run/plugins/
--rw-rw-r--   0 reiher   (16171) fb-5     (12389)        0 2023-05-29 13:04:41.000000 docker-run-cli-0.9.1/src/docker_run/plugins/__init__.py
--rw-rw-r--   0 reiher   (16171) fb-5     (12389)     4566 2023-05-29 13:04:41.000000 docker-run-cli-0.9.1/src/docker_run/plugins/core.py
--rw-rw-r--   0 reiher   (16171) fb-5     (12389)      520 2023-05-29 13:04:41.000000 docker-run-cli-0.9.1/src/docker_run/plugins/plugin.py
--rw-rw-r--   0 reiher   (16171) fb-5     (12389)      758 2023-05-29 13:04:41.000000 docker-run-cli-0.9.1/src/docker_run/utils.py
-drwxrwsr-x   0 reiher   (16171) fb-5     (12389)        0 2023-05-30 10:53:29.000000 docker-run-cli-0.9.1/src/docker_run_cli.egg-info/
--rw-rw-r--   0 reiher   (16171) fb-5     (12389)     7348 2023-05-30 10:53:29.000000 docker-run-cli-0.9.1/src/docker_run_cli.egg-info/PKG-INFO
--rw-rw-r--   0 reiher   (16171) fb-5     (12389)      568 2023-05-30 10:53:29.000000 docker-run-cli-0.9.1/src/docker_run_cli.egg-info/SOURCES.txt
--rw-rw-r--   0 reiher   (16171) fb-5     (12389)        1 2023-05-30 10:53:29.000000 docker-run-cli-0.9.1/src/docker_run_cli.egg-info/dependency_links.txt
--rw-rw-r--   0 reiher   (16171) fb-5     (12389)      151 2023-05-30 10:53:29.000000 docker-run-cli-0.9.1/src/docker_run_cli.egg-info/requires.txt
--rw-rw-r--   0 reiher   (16171) fb-5     (12389)       11 2023-05-30 10:53:29.000000 docker-run-cli-0.9.1/src/docker_run_cli.egg-info/top_level.txt
+drwxrwsr-x   0 reiher   (16171) fb-5     (12389)        0 2023-06-10 17:15:52.000000 docker-run-cli-0.9.2/
+-rw-rw-r--   0 reiher   (16171) fb-5     (12389)     1123 2023-05-29 13:04:51.000000 docker-run-cli-0.9.2/LICENSE
+-rw-rw-r--   0 reiher   (16171) fb-5     (12389)       51 2023-05-29 13:04:41.000000 docker-run-cli-0.9.2/MANIFEST.in
+-rw-rw-r--   0 reiher   (16171) fb-5     (12389)     7799 2023-06-10 17:15:52.000000 docker-run-cli-0.9.2/PKG-INFO
+-rw-rw-r--   0 reiher   (16171) fb-5     (12389)     5602 2023-06-10 17:14:01.000000 docker-run-cli-0.9.2/README.md
+-rw-rw-r--   0 reiher   (16171) fb-5     (12389)     1420 2023-06-10 17:14:01.000000 docker-run-cli-0.9.2/pyproject.toml
+drwxrwsr-x   0 reiher   (16171) fb-5     (12389)        0 2023-06-10 17:15:52.000000 docker-run-cli-0.9.2/scripts/
+-rwxrwxr-x   0 reiher   (16171) fb-5     (12389)     1620 2023-05-29 13:04:41.000000 docker-run-cli-0.9.2/scripts/activate-python-docker-run-shell-completion
+-rwxrwxr-x   0 reiher   (16171) fb-5     (12389)     1091 2023-06-10 17:14:01.000000 docker-run-cli-0.9.2/scripts/docker-run
+-rw-rw-r--   0 reiher   (16171) fb-5     (12389)       38 2023-06-10 17:15:52.000000 docker-run-cli-0.9.2/setup.cfg
+drwxrwsr-x   0 reiher   (16171) fb-5     (12389)        0 2023-06-10 17:15:52.000000 docker-run-cli-0.9.2/src/
+drwxrwsr-x   0 reiher   (16171) fb-5     (12389)        0 2023-06-10 17:15:52.000000 docker-run-cli-0.9.2/src/docker_run/
+-rw-rw-r--   0 reiher   (16171) fb-5     (12389)       45 2023-06-10 17:14:01.000000 docker-run-cli-0.9.2/src/docker_run/__init__.py
+-rw-rw-r--   0 reiher   (16171) fb-5     (12389)      107 2023-05-29 13:04:41.000000 docker-run-cli-0.9.2/src/docker_run/__main__.py
+drwxrwsr-x   0 reiher   (16171) fb-5     (12389)        0 2023-06-10 17:15:52.000000 docker-run-cli-0.9.2/src/docker_run/bash_completion.d/
+-rw-rw-r--   0 reiher   (16171) fb-5     (12389)     2886 2023-05-29 13:04:41.000000 docker-run-cli-0.9.2/src/docker_run/bash_completion.d/docker-run
+-rw-rw-r--   0 reiher   (16171) fb-5     (12389)     6110 2023-05-29 13:04:41.000000 docker-run-cli-0.9.2/src/docker_run/core.py
+drwxrwsr-x   0 reiher   (16171) fb-5     (12389)        0 2023-06-10 17:15:52.000000 docker-run-cli-0.9.2/src/docker_run/plugins/
+-rw-rw-r--   0 reiher   (16171) fb-5     (12389)        0 2023-05-29 13:04:41.000000 docker-run-cli-0.9.2/src/docker_run/plugins/__init__.py
+-rw-rw-r--   0 reiher   (16171) fb-5     (12389)     4566 2023-05-29 13:04:41.000000 docker-run-cli-0.9.2/src/docker_run/plugins/core.py
+-rw-rw-r--   0 reiher   (16171) fb-5     (12389)      520 2023-05-29 13:04:41.000000 docker-run-cli-0.9.2/src/docker_run/plugins/plugin.py
+-rw-rw-r--   0 reiher   (16171) fb-5     (12389)      758 2023-05-29 13:04:41.000000 docker-run-cli-0.9.2/src/docker_run/utils.py
+drwxrwsr-x   0 reiher   (16171) fb-5     (12389)        0 2023-06-10 17:15:52.000000 docker-run-cli-0.9.2/src/docker_run_cli.egg-info/
+-rw-rw-r--   0 reiher   (16171) fb-5     (12389)     7799 2023-06-10 17:15:52.000000 docker-run-cli-0.9.2/src/docker_run_cli.egg-info/PKG-INFO
+-rw-rw-r--   0 reiher   (16171) fb-5     (12389)      568 2023-06-10 17:15:52.000000 docker-run-cli-0.9.2/src/docker_run_cli.egg-info/SOURCES.txt
+-rw-rw-r--   0 reiher   (16171) fb-5     (12389)        1 2023-06-10 17:15:52.000000 docker-run-cli-0.9.2/src/docker_run_cli.egg-info/dependency_links.txt
+-rw-rw-r--   0 reiher   (16171) fb-5     (12389)      151 2023-06-10 17:15:52.000000 docker-run-cli-0.9.2/src/docker_run_cli.egg-info/requires.txt
+-rw-rw-r--   0 reiher   (16171) fb-5     (12389)       11 2023-06-10 17:15:52.000000 docker-run-cli-0.9.2/src/docker_run_cli.egg-info/top_level.txt
```

### Comparing `docker-run-cli-0.9.1/LICENSE` & `docker-run-cli-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `docker-run-cli-0.9.1/PKG-INFO` & `docker-run-cli-0.9.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docker-run-cli
-Version: 0.9.1
+Version: 0.9.2
 Summary: 'docker run' and 'docker exec' with useful defaults
 Author-email: Lennart Reiher <lennart.reiher@rwth-aachen.de>, Jean-Pierre Busch <jean-pierre.busch@rwth-aachen.de>
 Maintainer-email: Lennart Reiher <lennart.reiher@rwth-aachen.de>, Jean-Pierre Busch <jean-pierre.busch@rwth-aachen.de>
 License: MIT License
         
         Copyright (c) 2023 Institute for Automotive Engineering (ika), RWTH Aachen University
         
@@ -45,19 +45,22 @@
 
 # *docker-run* – ``docker run`` and ``docker exec`` with useful defaults
 
 <p align="center">
   <img src="https://img.shields.io/github/v/release/ika-rwth-aachen/docker-run"/></a>
   <img src="https://img.shields.io/github/license/ika-rwth-aachen/docker-run"/>
   <a href="https://pypi.org/project/docker-run-cli/"><img src="https://img.shields.io/pypi/dm/docker-run-cli?color=blue&label=PyPI%20downloads"/>
-  <a href="https://github.com/ika-rwth-aachen/docker-run"><img src="https://img.shields.io/github/stars/ika-rwth-aachen/docker-run?style=social"/></a>
 </p>
 
 *docker-run* is a CLI tool for simplified interaction with Docker images. Use it to easily start and attach to Docker containers with useful predefined arguments.
 
+<p align="center">
+  <img src="https://github.com/ika-rwth-aachen/docker-run/raw/main/assets/teaser.png" width=550>
+</p>
+
 While *docker-run* can be used with any Docker image, we recommend to also check out our other tools for Docker and ROS.
 - [*docker-ros*](https://github.com/ika-rwth-aachen/docker-ros) automatically builds minimal container images of ROS applications <a href="https://github.com/ika-rwth-aachen/docker-ros"><img src="https://img.shields.io/github/stars/ika-rwth-aachen/docker-ros?style=social"/></a>
 - [*docker-ros-ml-images*](https://github.com/ika-rwth-aachen/docker-ros-ml-images) provides machine learning-enabled ROS Docker images <a href="https://github.com/ika-rwth-aachen/docker-ros-ml-images"><img src="https://img.shields.io/github/stars/ika-rwth-aachen/docker-ros-ml-images?style=social"/></a>
 
 
 ## Quick Demo
 
@@ -87,26 +90,33 @@
 
 If a container with matching name is already running, `docker-run` will execute a command in that container via `docker exec` instead. This lets you quickly attach to a running container without passing any command, e.g.
 
 ```bash
 docker-run --name my-running-container
 ```
 
-Unlike with `docker run`, you can also set the Docker image and command via `--image` and `--cmd` arguments, see [Usage](#usage). This may be required for more complex use cases.
+Unlike with `docker run`, you can also set the Docker image via the `--image` arguments, see [Usage](#usage). This may be required for more complex use cases.
 
 
 ## Installation
 
 ```bash
 pip install docker-run-cli
 
 # (optional) shell auto-completion
 source $(activate-python-docker-run-shell-completion 2> /dev/null)
 ```
 
+> **Warning**  
+> Outside of a virtual environment, *pip* may default to a user-site installation of executables to `~/.local/bin`, which may not be present in your shell's `PATH`.  If running `docker-run` errors with `docker-run: command not found`, add the directory to your path. [*(More information)*](https://packaging.python.org/en/latest/tutorials/installing-packages/#installing-to-the-user-site)  
+> ```bash
+> echo "export PATH=$HOME/.local/bin:$PATH" >> ~/.bashrc
+> source ~/.bashrc
+> ```
+
 
 ## Usage
 
 ```
 usage: docker-run [--help] [--image IMAGE] [--mwd] [--name NAME] [--no-gpu]
                   [--no-it] [--no-loc] [--no-name] [--no-rm] [--no-tz]
                   [--no-x11] [--verbose] [--version]
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: docker-run-cli Version: 0.9.1 Summary: 'docker run'
+Metadata-Version: 2.1 Name: docker-run-cli Version: 0.9.2 Summary: 'docker run'
 and 'docker exec' with useful defaults Author-email: Lennart Reiher
 reiher@rwth-aachen.de>, Jean-Pierre Busch
 busch@rwth-aachen.de> Maintainer-email: Lennart Reiher
 reiher@rwth-aachen.de>, Jean-Pierre Busch
 busch@rwth-aachen.de> License: MIT License Copyright (c) 2023 Institute for
 Automotive Engineering (ika), RWTH Aachen University Permission is hereby
 granted, free of charge, to any person obtaining a copy of this software and
@@ -26,20 +26,21 @@
 Linux Requires-Python: >=3.7 Description-Content-Type: text/markdown Provides-
 Extra: dev Provides-Extra: docker-ros Provides-Extra: plugins Provides-Extra:
 all License-File: LICENSE [https://github.com/ika-rwth-aachen/docker-run/raw/
 main/assets/logo.png] # *docker-run* â ``docker run`` and ``docker exec``
 with useful defaults
      [https://img.shields.io/github/v/release/ika-rwth-aachen/docker-run]
  [https://img.shields.io/github/license/ika-rwth-aachen/docker-run] [https://
-img.shields.io/pypi/dm/docker-run-cli?color=blue&label=PyPI%20downloads]_
-[https://img.shields.io/github/stars/ika-rwth-aachen/docker-run?style=social]
+img.shields.io/pypi/dm/docker-run-cli?color=blue&label=PyPI%20downloads]
 *docker-run* is a CLI tool for simplified interaction with Docker images. Use
 it to easily start and attach to Docker containers with useful predefined
-arguments. While *docker-run* can be used with any Docker image, we recommend
-to also check out our other tools for Docker and ROS. - [*docker-ros*](https://
+arguments.
+  [https://github.com/ika-rwth-aachen/docker-run/raw/main/assets/teaser.png]
+While *docker-run* can be used with any Docker image, we recommend to also
+check out our other tools for Docker and ROS. - [*docker-ros*](https://
 github.com/ika-rwth-aachen/docker-ros) automatically builds minimal container
 images of ROS applications [https://img.shields.io/github/stars/ika-rwth-
 aachen/docker-ros?style=social] - [*docker-ros-ml-images*](https://github.com/
 ika-rwth-aachen/docker-ros-ml-images) provides machine learning-enabled ROS
 Docker images [https://img.shields.io/github/stars/ika-rwth-aachen/docker-ros-
 ml-images?style=social] ## Quick Demo The following quickly launches the GUI
 application `xeyes` to demonstrate how `docker-run` takes care of X11
@@ -55,34 +56,40 @@
 default. Each of these default features can be disabled, see [Usage](#usage). -
 container removal after exit (`--rm`) - interactive tty (`--interactive --tty`)
 - current directory name as container name (`--name`) - GPU support (`--gpus
 all` / `--runtime nvidia`) - X11 GUI forwarding If a container with matching
 name is already running, `docker-run` will execute a command in that container
 via `docker exec` instead. This lets you quickly attach to a running container
 without passing any command, e.g. ```bash docker-run --name my-running-
-container ``` Unlike with `docker run`, you can also set the Docker image and
-command via `--image` and `--cmd` arguments, see [Usage](#usage). This may be
-required for more complex use cases. ## Installation ```bash pip install
-docker-run-cli # (optional) shell auto-completion source $(activate-python-
-docker-run-shell-completion 2> /dev/null) ``` ## Usage ``` usage: docker-run [-
--help] [--image IMAGE] [--mwd] [--name NAME] [--no-gpu] [--no-it] [--no-loc] [-
--no-name] [--no-rm] [--no-tz] [--no-x11] [--verbose] [--version] Executes
-`docker run` with the following features enabled by default, each of which can
-be disabled individually: container removal after exit, interactive tty,
-current directory name as container name, GPU support, X11 GUI forwarding.
-Passes any additional arguments to `docker run`. Executes `docker exec` instead
-if a container with the specified name (`--name`) is already running. optional
-arguments: --help show this help message and exit --image IMAGE image name (may
-also be specified without --image as last argument before command) --mwd mount
-current directory at same path --name NAME container name; generates `docker
-exec` command if already running --no-gpu disable automatic GPU support --no-it
-disable automatic interactive tty --no-loc disable automatic locale --no-name
-disable automatic container name (current directory) --no-rm disable automatic
-container removal --no-tz disable automatic timezone --no-x11 disable automatic
-X11 GUI forwarding --verbose print generated command --version show program's
-version number and exit ``` ## Plugins `docker-run` can be extended through
-plugins. Plugins are installed as optional dependencies. ```bash # install
-specific plugin  pip install docker-run-cli[] # install all plugins pip install
-docker-run-cli[plugins] ``` | Plugin | Description | | --- | --- | | [`docker-
-ros`](https://pypi.org/project/docker-run-docker-ros) | extra functionality for
-Docker images built by [*docker-ros*](https://github.com/ika-rwth-aachen/
-docker-ros) |
+container ``` Unlike with `docker run`, you can also set the Docker image via
+the `--image` arguments, see [Usage](#usage). This may be required for more
+complex use cases. ## Installation ```bash pip install docker-run-cli #
+(optional) shell auto-completion source $(activate-python-docker-run-shell-
+completion 2> /dev/null) ``` > **Warning** > Outside of a virtual environment,
+*pip* may default to a user-site installation of executables to `~/.local/bin`,
+which may not be present in your shell's `PATH`. If running `docker-run` errors
+with `docker-run: command not found`, add the directory to your path. [*(More
+information)*](https://packaging.python.org/en/latest/tutorials/installing-
+packages/#installing-to-the-user-site) > ```bash > echo "export
+PATH=$HOME/.local/bin:$PATH" >> ~/.bashrc > source ~/.bashrc > ``` ## Usage ```
+usage: docker-run [--help] [--image IMAGE] [--mwd] [--name NAME] [--no-gpu] [--
+no-it] [--no-loc] [--no-name] [--no-rm] [--no-tz] [--no-x11] [--verbose] [--
+version] Executes `docker run` with the following features enabled by default,
+each of which can be disabled individually: container removal after exit,
+interactive tty, current directory name as container name, GPU support, X11 GUI
+forwarding. Passes any additional arguments to `docker run`. Executes `docker
+exec` instead if a container with the specified name (`--name`) is already
+running. optional arguments: --help show this help message and exit --image
+IMAGE image name (may also be specified without --image as last argument before
+command) --mwd mount current directory at same path --name NAME container name;
+generates `docker exec` command if already running --no-gpu disable automatic
+GPU support --no-it disable automatic interactive tty --no-loc disable
+automatic locale --no-name disable automatic container name (current directory)
+--no-rm disable automatic container removal --no-tz disable automatic timezone
+--no-x11 disable automatic X11 GUI forwarding --verbose print generated command
+--version show program's version number and exit ``` ## Plugins `docker-run`
+can be extended through plugins. Plugins are installed as optional
+dependencies. ```bash # install specific plugin  pip install docker-run-cli[] #
+install all plugins pip install docker-run-cli[plugins] ``` | Plugin |
+Description | | --- | --- | | [`docker-ros`](https://pypi.org/project/docker-
+run-docker-ros) | extra functionality for Docker images built by [*docker-ros*]
+(https://github.com/ika-rwth-aachen/docker-ros) |
```

### Comparing `docker-run-cli-0.9.1/README.md` & `docker-run-cli-0.9.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -2,19 +2,22 @@
 
 # *docker-run* – ``docker run`` and ``docker exec`` with useful defaults
 
 <p align="center">
   <img src="https://img.shields.io/github/v/release/ika-rwth-aachen/docker-run"/></a>
   <img src="https://img.shields.io/github/license/ika-rwth-aachen/docker-run"/>
   <a href="https://pypi.org/project/docker-run-cli/"><img src="https://img.shields.io/pypi/dm/docker-run-cli?color=blue&label=PyPI%20downloads"/>
-  <a href="https://github.com/ika-rwth-aachen/docker-run"><img src="https://img.shields.io/github/stars/ika-rwth-aachen/docker-run?style=social"/></a>
 </p>
 
 *docker-run* is a CLI tool for simplified interaction with Docker images. Use it to easily start and attach to Docker containers with useful predefined arguments.
 
+<p align="center">
+  <img src="https://github.com/ika-rwth-aachen/docker-run/raw/main/assets/teaser.png" width=550>
+</p>
+
 While *docker-run* can be used with any Docker image, we recommend to also check out our other tools for Docker and ROS.
 - [*docker-ros*](https://github.com/ika-rwth-aachen/docker-ros) automatically builds minimal container images of ROS applications <a href="https://github.com/ika-rwth-aachen/docker-ros"><img src="https://img.shields.io/github/stars/ika-rwth-aachen/docker-ros?style=social"/></a>
 - [*docker-ros-ml-images*](https://github.com/ika-rwth-aachen/docker-ros-ml-images) provides machine learning-enabled ROS Docker images <a href="https://github.com/ika-rwth-aachen/docker-ros-ml-images"><img src="https://img.shields.io/github/stars/ika-rwth-aachen/docker-ros-ml-images?style=social"/></a>
 
 
 ## Quick Demo
 
@@ -44,26 +47,33 @@
 
 If a container with matching name is already running, `docker-run` will execute a command in that container via `docker exec` instead. This lets you quickly attach to a running container without passing any command, e.g.
 
 ```bash
 docker-run --name my-running-container
 ```
 
-Unlike with `docker run`, you can also set the Docker image and command via `--image` and `--cmd` arguments, see [Usage](#usage). This may be required for more complex use cases.
+Unlike with `docker run`, you can also set the Docker image via the `--image` arguments, see [Usage](#usage). This may be required for more complex use cases.
 
 
 ## Installation
 
 ```bash
 pip install docker-run-cli
 
 # (optional) shell auto-completion
 source $(activate-python-docker-run-shell-completion 2> /dev/null)
 ```
 
+> **Warning**  
+> Outside of a virtual environment, *pip* may default to a user-site installation of executables to `~/.local/bin`, which may not be present in your shell's `PATH`.  If running `docker-run` errors with `docker-run: command not found`, add the directory to your path. [*(More information)*](https://packaging.python.org/en/latest/tutorials/installing-packages/#installing-to-the-user-site)  
+> ```bash
+> echo "export PATH=$HOME/.local/bin:$PATH" >> ~/.bashrc
+> source ~/.bashrc
+> ```
+
 
 ## Usage
 
 ```
 usage: docker-run [--help] [--image IMAGE] [--mwd] [--name NAME] [--no-gpu]
                   [--no-it] [--no-loc] [--no-name] [--no-rm] [--no-tz]
                   [--no-x11] [--verbose] [--version]
```

#### html2text {}

```diff
@@ -1,17 +1,18 @@
 [https://github.com/ika-rwth-aachen/docker-run/raw/main/assets/logo.png] #
 *docker-run* â ``docker run`` and ``docker exec`` with useful defaults
      [https://img.shields.io/github/v/release/ika-rwth-aachen/docker-run]
  [https://img.shields.io/github/license/ika-rwth-aachen/docker-run] [https://
-img.shields.io/pypi/dm/docker-run-cli?color=blue&label=PyPI%20downloads]_
-[https://img.shields.io/github/stars/ika-rwth-aachen/docker-run?style=social]
+img.shields.io/pypi/dm/docker-run-cli?color=blue&label=PyPI%20downloads]
 *docker-run* is a CLI tool for simplified interaction with Docker images. Use
 it to easily start and attach to Docker containers with useful predefined
-arguments. While *docker-run* can be used with any Docker image, we recommend
-to also check out our other tools for Docker and ROS. - [*docker-ros*](https://
+arguments.
+  [https://github.com/ika-rwth-aachen/docker-run/raw/main/assets/teaser.png]
+While *docker-run* can be used with any Docker image, we recommend to also
+check out our other tools for Docker and ROS. - [*docker-ros*](https://
 github.com/ika-rwth-aachen/docker-ros) automatically builds minimal container
 images of ROS applications [https://img.shields.io/github/stars/ika-rwth-
 aachen/docker-ros?style=social] - [*docker-ros-ml-images*](https://github.com/
 ika-rwth-aachen/docker-ros-ml-images) provides machine learning-enabled ROS
 Docker images [https://img.shields.io/github/stars/ika-rwth-aachen/docker-ros-
 ml-images?style=social] ## Quick Demo The following quickly launches the GUI
 application `xeyes` to demonstrate how `docker-run` takes care of X11
@@ -27,34 +28,40 @@
 default. Each of these default features can be disabled, see [Usage](#usage). -
 container removal after exit (`--rm`) - interactive tty (`--interactive --tty`)
 - current directory name as container name (`--name`) - GPU support (`--gpus
 all` / `--runtime nvidia`) - X11 GUI forwarding If a container with matching
 name is already running, `docker-run` will execute a command in that container
 via `docker exec` instead. This lets you quickly attach to a running container
 without passing any command, e.g. ```bash docker-run --name my-running-
-container ``` Unlike with `docker run`, you can also set the Docker image and
-command via `--image` and `--cmd` arguments, see [Usage](#usage). This may be
-required for more complex use cases. ## Installation ```bash pip install
-docker-run-cli # (optional) shell auto-completion source $(activate-python-
-docker-run-shell-completion 2> /dev/null) ``` ## Usage ``` usage: docker-run [-
--help] [--image IMAGE] [--mwd] [--name NAME] [--no-gpu] [--no-it] [--no-loc] [-
--no-name] [--no-rm] [--no-tz] [--no-x11] [--verbose] [--version] Executes
-`docker run` with the following features enabled by default, each of which can
-be disabled individually: container removal after exit, interactive tty,
-current directory name as container name, GPU support, X11 GUI forwarding.
-Passes any additional arguments to `docker run`. Executes `docker exec` instead
-if a container with the specified name (`--name`) is already running. optional
-arguments: --help show this help message and exit --image IMAGE image name (may
-also be specified without --image as last argument before command) --mwd mount
-current directory at same path --name NAME container name; generates `docker
-exec` command if already running --no-gpu disable automatic GPU support --no-it
-disable automatic interactive tty --no-loc disable automatic locale --no-name
-disable automatic container name (current directory) --no-rm disable automatic
-container removal --no-tz disable automatic timezone --no-x11 disable automatic
-X11 GUI forwarding --verbose print generated command --version show program's
-version number and exit ``` ## Plugins `docker-run` can be extended through
-plugins. Plugins are installed as optional dependencies. ```bash # install
-specific plugin  pip install docker-run-cli[] # install all plugins pip install
-docker-run-cli[plugins] ``` | Plugin | Description | | --- | --- | | [`docker-
-ros`](https://pypi.org/project/docker-run-docker-ros) | extra functionality for
-Docker images built by [*docker-ros*](https://github.com/ika-rwth-aachen/
-docker-ros) |
+container ``` Unlike with `docker run`, you can also set the Docker image via
+the `--image` arguments, see [Usage](#usage). This may be required for more
+complex use cases. ## Installation ```bash pip install docker-run-cli #
+(optional) shell auto-completion source $(activate-python-docker-run-shell-
+completion 2> /dev/null) ``` > **Warning** > Outside of a virtual environment,
+*pip* may default to a user-site installation of executables to `~/.local/bin`,
+which may not be present in your shell's `PATH`. If running `docker-run` errors
+with `docker-run: command not found`, add the directory to your path. [*(More
+information)*](https://packaging.python.org/en/latest/tutorials/installing-
+packages/#installing-to-the-user-site) > ```bash > echo "export
+PATH=$HOME/.local/bin:$PATH" >> ~/.bashrc > source ~/.bashrc > ``` ## Usage ```
+usage: docker-run [--help] [--image IMAGE] [--mwd] [--name NAME] [--no-gpu] [--
+no-it] [--no-loc] [--no-name] [--no-rm] [--no-tz] [--no-x11] [--verbose] [--
+version] Executes `docker run` with the following features enabled by default,
+each of which can be disabled individually: container removal after exit,
+interactive tty, current directory name as container name, GPU support, X11 GUI
+forwarding. Passes any additional arguments to `docker run`. Executes `docker
+exec` instead if a container with the specified name (`--name`) is already
+running. optional arguments: --help show this help message and exit --image
+IMAGE image name (may also be specified without --image as last argument before
+command) --mwd mount current directory at same path --name NAME container name;
+generates `docker exec` command if already running --no-gpu disable automatic
+GPU support --no-it disable automatic interactive tty --no-loc disable
+automatic locale --no-name disable automatic container name (current directory)
+--no-rm disable automatic container removal --no-tz disable automatic timezone
+--no-x11 disable automatic X11 GUI forwarding --verbose print generated command
+--version show program's version number and exit ``` ## Plugins `docker-run`
+can be extended through plugins. Plugins are installed as optional
+dependencies. ```bash # install specific plugin  pip install docker-run-cli[] #
+install all plugins pip install docker-run-cli[plugins] ``` | Plugin |
+Description | | --- | --- | | [`docker-ros`](https://pypi.org/project/docker-
+run-docker-ros) | extra functionality for Docker images built by [*docker-ros*]
+(https://github.com/ika-rwth-aachen/docker-ros) |
```

### Comparing `docker-run-cli-0.9.1/pyproject.toml` & `docker-run-cli-0.9.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "docker-run-cli"
-version = "0.9.1"
+version = "0.9.2"
 description = "'docker run' and 'docker exec' with useful defaults"
 license = {file = "LICENSE"}
 readme = "README.md"
 authors = [
     {name = "Lennart Reiher", email = "lennart.reiher@rwth-aachen.de"},
     {name = "Jean-Pierre Busch", email = "jean-pierre.busch@rwth-aachen.de"},
 ]
```

### Comparing `docker-run-cli-0.9.1/scripts/activate-python-docker-run-shell-completion` & `docker-run-cli-0.9.2/scripts/activate-python-docker-run-shell-completion`

 * *Files identical despite different names*

### Comparing `docker-run-cli-0.9.1/scripts/docker-run` & `docker-run-cli-0.9.2/scripts/docker-run`

 * *Files 15% similar despite different names*

```diff
@@ -7,27 +7,26 @@
 
 # check if user is in docker group
 if [[ $OS != "Darwin" ]]; then
   if ! groups | grep -q "\bdocker\b"; then
     echo "User '${USER}' must be in 'docker' group to run containers."
     echo "User can be added via: sudo usermod -aG docker ${USER}"
     echo "Afterwards, the user may need to logout and login again."
-    exit 1
   fi
 fi
 
 # check operating system and architecture
 if ! { [[ $OS = "Linux" && $ARCH = "x86_64" ]] || [[ $OS = "Darwin" && $ARCH = "arm64" ]] || [[ $OS = "Linux" && $ARCH = "aarch64" ]]; }; then
-  >&2 echo "This script does not support $OS with $ARCH architecture."
+  >&2 echo "docker-run does not support $OS with $ARCH architecture."
   exit 1
 fi
 
 # generate docker run/exec command
 CMD_FILE=$(mktemp)
-python -m docker_run "${@}" 2>&1 >$CMD_FILE
+python3 -m docker_run "${@}" 2>&1 >$CMD_FILE
 CMD=$(cat $CMD_FILE)
 rm $CMD_FILE
 
 # execute command
 if [[ ! -z "$CMD" ]]; then
   echo -e "================================================================================\n"
   exec $CMD
```

### Comparing `docker-run-cli-0.9.1/src/docker_run/bash_completion.d/docker-run` & `docker-run-cli-0.9.2/src/docker_run/bash_completion.d/docker-run`

 * *Files identical despite different names*

### Comparing `docker-run-cli-0.9.1/src/docker_run/core.py` & `docker-run-cli-0.9.2/src/docker_run/core.py`

 * *Files identical despite different names*

### Comparing `docker-run-cli-0.9.1/src/docker_run/plugins/core.py` & `docker-run-cli-0.9.2/src/docker_run/plugins/core.py`

 * *Files identical despite different names*

### Comparing `docker-run-cli-0.9.1/src/docker_run/plugins/plugin.py` & `docker-run-cli-0.9.2/src/docker_run/plugins/plugin.py`

 * *Files identical despite different names*

### Comparing `docker-run-cli-0.9.1/src/docker_run/utils.py` & `docker-run-cli-0.9.2/src/docker_run/utils.py`

 * *Files identical despite different names*

### Comparing `docker-run-cli-0.9.1/src/docker_run_cli.egg-info/PKG-INFO` & `docker-run-cli-0.9.2/src/docker_run_cli.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docker-run-cli
-Version: 0.9.1
+Version: 0.9.2
 Summary: 'docker run' and 'docker exec' with useful defaults
 Author-email: Lennart Reiher <lennart.reiher@rwth-aachen.de>, Jean-Pierre Busch <jean-pierre.busch@rwth-aachen.de>
 Maintainer-email: Lennart Reiher <lennart.reiher@rwth-aachen.de>, Jean-Pierre Busch <jean-pierre.busch@rwth-aachen.de>
 License: MIT License
         
         Copyright (c) 2023 Institute for Automotive Engineering (ika), RWTH Aachen University
         
@@ -45,19 +45,22 @@
 
 # *docker-run* – ``docker run`` and ``docker exec`` with useful defaults
 
 <p align="center">
   <img src="https://img.shields.io/github/v/release/ika-rwth-aachen/docker-run"/></a>
   <img src="https://img.shields.io/github/license/ika-rwth-aachen/docker-run"/>
   <a href="https://pypi.org/project/docker-run-cli/"><img src="https://img.shields.io/pypi/dm/docker-run-cli?color=blue&label=PyPI%20downloads"/>
-  <a href="https://github.com/ika-rwth-aachen/docker-run"><img src="https://img.shields.io/github/stars/ika-rwth-aachen/docker-run?style=social"/></a>
 </p>
 
 *docker-run* is a CLI tool for simplified interaction with Docker images. Use it to easily start and attach to Docker containers with useful predefined arguments.
 
+<p align="center">
+  <img src="https://github.com/ika-rwth-aachen/docker-run/raw/main/assets/teaser.png" width=550>
+</p>
+
 While *docker-run* can be used with any Docker image, we recommend to also check out our other tools for Docker and ROS.
 - [*docker-ros*](https://github.com/ika-rwth-aachen/docker-ros) automatically builds minimal container images of ROS applications <a href="https://github.com/ika-rwth-aachen/docker-ros"><img src="https://img.shields.io/github/stars/ika-rwth-aachen/docker-ros?style=social"/></a>
 - [*docker-ros-ml-images*](https://github.com/ika-rwth-aachen/docker-ros-ml-images) provides machine learning-enabled ROS Docker images <a href="https://github.com/ika-rwth-aachen/docker-ros-ml-images"><img src="https://img.shields.io/github/stars/ika-rwth-aachen/docker-ros-ml-images?style=social"/></a>
 
 
 ## Quick Demo
 
@@ -87,26 +90,33 @@
 
 If a container with matching name is already running, `docker-run` will execute a command in that container via `docker exec` instead. This lets you quickly attach to a running container without passing any command, e.g.
 
 ```bash
 docker-run --name my-running-container
 ```
 
-Unlike with `docker run`, you can also set the Docker image and command via `--image` and `--cmd` arguments, see [Usage](#usage). This may be required for more complex use cases.
+Unlike with `docker run`, you can also set the Docker image via the `--image` arguments, see [Usage](#usage). This may be required for more complex use cases.
 
 
 ## Installation
 
 ```bash
 pip install docker-run-cli
 
 # (optional) shell auto-completion
 source $(activate-python-docker-run-shell-completion 2> /dev/null)
 ```
 
+> **Warning**  
+> Outside of a virtual environment, *pip* may default to a user-site installation of executables to `~/.local/bin`, which may not be present in your shell's `PATH`.  If running `docker-run` errors with `docker-run: command not found`, add the directory to your path. [*(More information)*](https://packaging.python.org/en/latest/tutorials/installing-packages/#installing-to-the-user-site)  
+> ```bash
+> echo "export PATH=$HOME/.local/bin:$PATH" >> ~/.bashrc
+> source ~/.bashrc
+> ```
+
 
 ## Usage
 
 ```
 usage: docker-run [--help] [--image IMAGE] [--mwd] [--name NAME] [--no-gpu]
                   [--no-it] [--no-loc] [--no-name] [--no-rm] [--no-tz]
                   [--no-x11] [--verbose] [--version]
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: docker-run-cli Version: 0.9.1 Summary: 'docker run'
+Metadata-Version: 2.1 Name: docker-run-cli Version: 0.9.2 Summary: 'docker run'
 and 'docker exec' with useful defaults Author-email: Lennart Reiher
 reiher@rwth-aachen.de>, Jean-Pierre Busch
 busch@rwth-aachen.de> Maintainer-email: Lennart Reiher
 reiher@rwth-aachen.de>, Jean-Pierre Busch
 busch@rwth-aachen.de> License: MIT License Copyright (c) 2023 Institute for
 Automotive Engineering (ika), RWTH Aachen University Permission is hereby
 granted, free of charge, to any person obtaining a copy of this software and
@@ -26,20 +26,21 @@
 Linux Requires-Python: >=3.7 Description-Content-Type: text/markdown Provides-
 Extra: dev Provides-Extra: docker-ros Provides-Extra: plugins Provides-Extra:
 all License-File: LICENSE [https://github.com/ika-rwth-aachen/docker-run/raw/
 main/assets/logo.png] # *docker-run* â ``docker run`` and ``docker exec``
 with useful defaults
      [https://img.shields.io/github/v/release/ika-rwth-aachen/docker-run]
  [https://img.shields.io/github/license/ika-rwth-aachen/docker-run] [https://
-img.shields.io/pypi/dm/docker-run-cli?color=blue&label=PyPI%20downloads]_
-[https://img.shields.io/github/stars/ika-rwth-aachen/docker-run?style=social]
+img.shields.io/pypi/dm/docker-run-cli?color=blue&label=PyPI%20downloads]
 *docker-run* is a CLI tool for simplified interaction with Docker images. Use
 it to easily start and attach to Docker containers with useful predefined
-arguments. While *docker-run* can be used with any Docker image, we recommend
-to also check out our other tools for Docker and ROS. - [*docker-ros*](https://
+arguments.
+  [https://github.com/ika-rwth-aachen/docker-run/raw/main/assets/teaser.png]
+While *docker-run* can be used with any Docker image, we recommend to also
+check out our other tools for Docker and ROS. - [*docker-ros*](https://
 github.com/ika-rwth-aachen/docker-ros) automatically builds minimal container
 images of ROS applications [https://img.shields.io/github/stars/ika-rwth-
 aachen/docker-ros?style=social] - [*docker-ros-ml-images*](https://github.com/
 ika-rwth-aachen/docker-ros-ml-images) provides machine learning-enabled ROS
 Docker images [https://img.shields.io/github/stars/ika-rwth-aachen/docker-ros-
 ml-images?style=social] ## Quick Demo The following quickly launches the GUI
 application `xeyes` to demonstrate how `docker-run` takes care of X11
@@ -55,34 +56,40 @@
 default. Each of these default features can be disabled, see [Usage](#usage). -
 container removal after exit (`--rm`) - interactive tty (`--interactive --tty`)
 - current directory name as container name (`--name`) - GPU support (`--gpus
 all` / `--runtime nvidia`) - X11 GUI forwarding If a container with matching
 name is already running, `docker-run` will execute a command in that container
 via `docker exec` instead. This lets you quickly attach to a running container
 without passing any command, e.g. ```bash docker-run --name my-running-
-container ``` Unlike with `docker run`, you can also set the Docker image and
-command via `--image` and `--cmd` arguments, see [Usage](#usage). This may be
-required for more complex use cases. ## Installation ```bash pip install
-docker-run-cli # (optional) shell auto-completion source $(activate-python-
-docker-run-shell-completion 2> /dev/null) ``` ## Usage ``` usage: docker-run [-
--help] [--image IMAGE] [--mwd] [--name NAME] [--no-gpu] [--no-it] [--no-loc] [-
--no-name] [--no-rm] [--no-tz] [--no-x11] [--verbose] [--version] Executes
-`docker run` with the following features enabled by default, each of which can
-be disabled individually: container removal after exit, interactive tty,
-current directory name as container name, GPU support, X11 GUI forwarding.
-Passes any additional arguments to `docker run`. Executes `docker exec` instead
-if a container with the specified name (`--name`) is already running. optional
-arguments: --help show this help message and exit --image IMAGE image name (may
-also be specified without --image as last argument before command) --mwd mount
-current directory at same path --name NAME container name; generates `docker
-exec` command if already running --no-gpu disable automatic GPU support --no-it
-disable automatic interactive tty --no-loc disable automatic locale --no-name
-disable automatic container name (current directory) --no-rm disable automatic
-container removal --no-tz disable automatic timezone --no-x11 disable automatic
-X11 GUI forwarding --verbose print generated command --version show program's
-version number and exit ``` ## Plugins `docker-run` can be extended through
-plugins. Plugins are installed as optional dependencies. ```bash # install
-specific plugin  pip install docker-run-cli[] # install all plugins pip install
-docker-run-cli[plugins] ``` | Plugin | Description | | --- | --- | | [`docker-
-ros`](https://pypi.org/project/docker-run-docker-ros) | extra functionality for
-Docker images built by [*docker-ros*](https://github.com/ika-rwth-aachen/
-docker-ros) |
+container ``` Unlike with `docker run`, you can also set the Docker image via
+the `--image` arguments, see [Usage](#usage). This may be required for more
+complex use cases. ## Installation ```bash pip install docker-run-cli #
+(optional) shell auto-completion source $(activate-python-docker-run-shell-
+completion 2> /dev/null) ``` > **Warning** > Outside of a virtual environment,
+*pip* may default to a user-site installation of executables to `~/.local/bin`,
+which may not be present in your shell's `PATH`. If running `docker-run` errors
+with `docker-run: command not found`, add the directory to your path. [*(More
+information)*](https://packaging.python.org/en/latest/tutorials/installing-
+packages/#installing-to-the-user-site) > ```bash > echo "export
+PATH=$HOME/.local/bin:$PATH" >> ~/.bashrc > source ~/.bashrc > ``` ## Usage ```
+usage: docker-run [--help] [--image IMAGE] [--mwd] [--name NAME] [--no-gpu] [--
+no-it] [--no-loc] [--no-name] [--no-rm] [--no-tz] [--no-x11] [--verbose] [--
+version] Executes `docker run` with the following features enabled by default,
+each of which can be disabled individually: container removal after exit,
+interactive tty, current directory name as container name, GPU support, X11 GUI
+forwarding. Passes any additional arguments to `docker run`. Executes `docker
+exec` instead if a container with the specified name (`--name`) is already
+running. optional arguments: --help show this help message and exit --image
+IMAGE image name (may also be specified without --image as last argument before
+command) --mwd mount current directory at same path --name NAME container name;
+generates `docker exec` command if already running --no-gpu disable automatic
+GPU support --no-it disable automatic interactive tty --no-loc disable
+automatic locale --no-name disable automatic container name (current directory)
+--no-rm disable automatic container removal --no-tz disable automatic timezone
+--no-x11 disable automatic X11 GUI forwarding --verbose print generated command
+--version show program's version number and exit ``` ## Plugins `docker-run`
+can be extended through plugins. Plugins are installed as optional
+dependencies. ```bash # install specific plugin  pip install docker-run-cli[] #
+install all plugins pip install docker-run-cli[plugins] ``` | Plugin |
+Description | | --- | --- | | [`docker-ros`](https://pypi.org/project/docker-
+run-docker-ros) | extra functionality for Docker images built by [*docker-ros*]
+(https://github.com/ika-rwth-aachen/docker-ros) |
```

### Comparing `docker-run-cli-0.9.1/src/docker_run_cli.egg-info/SOURCES.txt` & `docker-run-cli-0.9.2/src/docker_run_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

