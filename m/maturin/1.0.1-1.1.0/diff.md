# Comparing `tmp/maturin-1.0.1.tar.gz` & `tmp/maturin-1.1.0.tar.gz`

## Comparing `maturin-1.0.1.tar` & `maturin-1.1.0.tar`

### file list

```diff
@@ -1,64 +1,64 @@
--rw-r--r--   0        0        0     4559 1970-01-01 00:00:00.000000 maturin-1.0.1/Cargo.toml
--rw-r--r--   0     1001      123     1681 2023-05-28 02:31:17.000000 maturin-1.0.1/.cirrus.yml
--rw-r--r--   0     1001      123       94 2023-05-28 02:31:17.000000 maturin-1.0.1/.codespellrc
--rw-r--r--   0     1001      123      252 2023-05-28 02:31:17.000000 maturin-1.0.1/.config/nextest.toml
--rw-r--r--   0     1001      123      488 2023-05-28 02:31:17.000000 maturin-1.0.1/.devcontainer/devcontainer.json
--rwxr-xr-x   0     1001      123      351 2023-05-28 02:31:17.000000 maturin-1.0.1/.devcontainer/post_create.sh
--rw-r--r--   0     1001      123      180 2023-05-28 02:31:17.000000 maturin-1.0.1/.dockerignore
--rw-r--r--   0     1001      123      184 2023-05-28 02:31:17.000000 maturin-1.0.1/.gitignore
--rw-r--r--   0     1001      123    69147 2023-05-28 02:31:17.000000 maturin-1.0.1/Cargo.lock
--rw-r--r--   0     1001      123    57326 2023-05-28 02:31:17.000000 maturin-1.0.1/Changelog.md
--rw-r--r--   0     1001      123     3228 2023-05-28 02:31:17.000000 maturin-1.0.1/Code-of-Conduct.md
--rw-r--r--   0     1001      123     2386 2023-05-28 02:31:17.000000 maturin-1.0.1/Dockerfile
--rw-r--r--   0     1001      123      245 2023-05-28 02:31:17.000000 maturin-1.0.1/MANIFEST.in
--rw-r--r--   0     1001      123    16809 2023-05-28 02:31:17.000000 maturin-1.0.1/README.md
--rw-r--r--   0     1001      123       16 2023-05-28 02:31:17.000000 maturin-1.0.1/clippy.toml
--rw-r--r--   0     1001      123     9936 2023-05-28 02:31:17.000000 maturin-1.0.1/deny.toml
--rw-r--r--   0     1001      123    10847 2023-05-28 02:31:17.000000 maturin-1.0.1/license-apache
--rw-r--r--   0     1001      123     1051 2023-05-28 02:31:17.000000 maturin-1.0.1/license-mit
--rw-r--r--   0     1001      123     6739 2023-05-28 02:31:17.000000 maturin-1.0.1/maturin/__init__.py
--rw-r--r--   0     1001      123      956 2023-05-28 02:31:17.000000 maturin-1.0.1/maturin/__main__.py
--rw-r--r--   0     1001      123     5162 2023-05-28 02:31:17.000000 maturin-1.0.1/maturin/import_hook.py
--rw-r--r--   0     1001      123      200 2023-05-28 02:31:17.000000 maturin-1.0.1/netlify.toml
--rw-r--r--   0     1001      123     2170 2023-05-28 02:31:17.000000 maturin-1.0.1/noxfile.py
--rw-r--r--   0     1001      123     1290 2023-05-28 02:31:17.000000 maturin-1.0.1/pyproject.toml
--rw-r--r--   0     1001      123     2890 2023-05-28 02:31:17.000000 maturin-1.0.1/setup.py
--rw-r--r--   0     1001      123    19534 2023-05-28 02:31:17.000000 maturin-1.0.1/src/auditwheel/audit.rs
--rw-r--r--   0     1001      123    53261 2023-05-28 02:31:17.000000 maturin-1.0.1/src/auditwheel/manylinux-policy.json
--rw-r--r--   0     1001      123      242 2023-05-28 02:31:17.000000 maturin-1.0.1/src/auditwheel/mod.rs
--rw-r--r--   0     1001      123     1862 2023-05-28 02:31:17.000000 maturin-1.0.1/src/auditwheel/musllinux-policy.json
--rw-r--r--   0     1001      123     1389 2023-05-28 02:31:17.000000 maturin-1.0.1/src/auditwheel/musllinux.rs
--rw-r--r--   0     1001      123     3777 2023-05-28 02:31:17.000000 maturin-1.0.1/src/auditwheel/patchelf.rs
--rw-r--r--   0     1001      123     4602 2023-05-28 02:31:17.000000 maturin-1.0.1/src/auditwheel/platform_tag.rs
--rw-r--r--   0     1001      123     5393 2023-05-28 02:31:17.000000 maturin-1.0.1/src/auditwheel/policy.rs
--rw-r--r--   0     1001      123     1169 2023-05-28 02:31:17.000000 maturin-1.0.1/src/auditwheel/repair.rs
--rw-r--r--   0     1001      123    47638 2023-05-28 02:31:17.000000 maturin-1.0.1/src/build_context.rs
--rw-r--r--   0     1001      123    57614 2023-05-28 02:31:17.000000 maturin-1.0.1/src/build_options.rs
--rw-r--r--   0     1001      123     5407 2023-05-28 02:31:17.000000 maturin-1.0.1/src/cargo_toml.rs
--rw-r--r--   0     1001      123    33723 2023-05-28 02:31:17.000000 maturin-1.0.1/src/ci.rs
--rw-r--r--   0     1001      123    24173 2023-05-28 02:31:17.000000 maturin-1.0.1/src/compile.rs
--rw-r--r--   0     1001      123     8342 2023-05-28 02:31:17.000000 maturin-1.0.1/src/cross_compile.rs
--rw-r--r--   0     1001      123     6092 2023-05-28 02:31:17.000000 maturin-1.0.1/src/develop.rs
--rw-r--r--   0     1001      123     2233 2023-05-28 02:31:17.000000 maturin-1.0.1/src/lib.rs
--rw-r--r--   0     1001      123    17816 2023-05-28 02:31:17.000000 maturin-1.0.1/src/main.rs
--rw-r--r--   0     1001      123    32462 2023-05-28 02:31:17.000000 maturin-1.0.1/src/metadata.rs
--rw-r--r--   0     1001      123    45608 2023-05-28 02:31:17.000000 maturin-1.0.1/src/module_writer.rs
--rw-r--r--   0     1001      123     8203 2023-05-28 02:31:17.000000 maturin-1.0.1/src/new_project.rs
--rw-r--r--   0     1001      123    16869 2023-05-28 02:31:17.000000 maturin-1.0.1/src/project_layout.rs
--rw-r--r--   0     1001      123    18607 2023-05-28 02:31:17.000000 maturin-1.0.1/src/pyproject_toml.rs
--rw-r--r--   0     1001      123    28354 2023-05-28 02:31:17.000000 maturin-1.0.1/src/python_interpreter/config.rs
--rw-r--r--   0     1001      123     1595 2023-05-28 02:31:17.000000 maturin-1.0.1/src/python_interpreter/get_interpreter_metadata.py
--rw-r--r--   0     1001      123    35318 2023-05-28 02:31:17.000000 maturin-1.0.1/src/python_interpreter/mod.rs
--rw-r--r--   0     1001      123    35086 2023-05-28 02:31:17.000000 maturin-1.0.1/src/source_distribution.rs
--rw-r--r--   0     1001      123    18602 2023-05-28 02:31:17.000000 maturin-1.0.1/src/target.rs
--rw-r--r--   0     1001      123      686 2023-05-28 02:31:17.000000 maturin-1.0.1/src/templates/.gitignore.j2
--rw-r--r--   0     1001      123      518 2023-05-28 02:31:17.000000 maturin-1.0.1/src/templates/Cargo.toml.j2
--rw-r--r--   0     1001      123      149 2023-05-28 02:31:17.000000 maturin-1.0.1/src/templates/__init__.py.j2
--rw-r--r--   0     1001      123      123 2023-05-28 02:31:17.000000 maturin-1.0.1/src/templates/build.rs.j2
--rw-r--r--   0     1001      123       47 2023-05-28 02:31:17.000000 maturin-1.0.1/src/templates/example.udl.j2
--rw-r--r--   0     1001      123      722 2023-05-28 02:31:17.000000 maturin-1.0.1/src/templates/lib.rs.j2
--rw-r--r--   0     1001      123       45 2023-05-28 02:31:17.000000 maturin-1.0.1/src/templates/main.rs.j2
--rw-r--r--   0     1001      123      859 2023-05-28 02:31:17.000000 maturin-1.0.1/src/templates/pyproject.toml.j2
--rw-r--r--   0     1001      123    22914 2023-05-28 02:31:17.000000 maturin-1.0.1/src/upload.rs
--rwxr-xr-x   0     1001      123      974 2023-05-28 02:31:17.000000 maturin-1.0.1/test-dockerfile.sh
--rw-r--r--   0        0        0    17988 1970-01-01 00:00:00.000000 maturin-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     4559 1970-01-01 00:00:00.000000 maturin-1.1.0/Cargo.toml
+-rw-r--r--   0     1001      123     1681 2023-06-10 12:17:57.000000 maturin-1.1.0/.cirrus.yml
+-rw-r--r--   0     1001      123       94 2023-06-10 12:17:57.000000 maturin-1.1.0/.codespellrc
+-rw-r--r--   0     1001      123      252 2023-06-10 12:17:57.000000 maturin-1.1.0/.config/nextest.toml
+-rw-r--r--   0     1001      123      488 2023-06-10 12:17:57.000000 maturin-1.1.0/.devcontainer/devcontainer.json
+-rwxr-xr-x   0     1001      123      351 2023-06-10 12:17:57.000000 maturin-1.1.0/.devcontainer/post_create.sh
+-rw-r--r--   0     1001      123      180 2023-06-10 12:17:57.000000 maturin-1.1.0/.dockerignore
+-rw-r--r--   0     1001      123      184 2023-06-10 12:17:57.000000 maturin-1.1.0/.gitignore
+-rw-r--r--   0     1001      123    68354 2023-06-10 12:17:57.000000 maturin-1.1.0/Cargo.lock
+-rw-r--r--   0     1001      123    57800 2023-06-10 12:17:57.000000 maturin-1.1.0/Changelog.md
+-rw-r--r--   0     1001      123     3228 2023-06-10 12:17:57.000000 maturin-1.1.0/Code-of-Conduct.md
+-rw-r--r--   0     1001      123     2386 2023-06-10 12:17:57.000000 maturin-1.1.0/Dockerfile
+-rw-r--r--   0     1001      123      245 2023-06-10 12:17:57.000000 maturin-1.1.0/MANIFEST.in
+-rw-r--r--   0     1001      123    16951 2023-06-10 12:17:57.000000 maturin-1.1.0/README.md
+-rw-r--r--   0     1001      123       16 2023-06-10 12:17:57.000000 maturin-1.1.0/clippy.toml
+-rw-r--r--   0     1001      123     9882 2023-06-10 12:17:57.000000 maturin-1.1.0/deny.toml
+-rw-r--r--   0     1001      123    10847 2023-06-10 12:17:57.000000 maturin-1.1.0/license-apache
+-rw-r--r--   0     1001      123     1051 2023-06-10 12:17:57.000000 maturin-1.1.0/license-mit
+-rw-r--r--   0     1001      123     6739 2023-06-10 12:17:57.000000 maturin-1.1.0/maturin/__init__.py
+-rw-r--r--   0     1001      123      956 2023-06-10 12:17:57.000000 maturin-1.1.0/maturin/__main__.py
+-rw-r--r--   0     1001      123     5162 2023-06-10 12:17:57.000000 maturin-1.1.0/maturin/import_hook.py
+-rw-r--r--   0     1001      123      200 2023-06-10 12:17:57.000000 maturin-1.1.0/netlify.toml
+-rw-r--r--   0     1001      123     2170 2023-06-10 12:17:57.000000 maturin-1.1.0/noxfile.py
+-rw-r--r--   0     1001      123     1290 2023-06-10 12:17:57.000000 maturin-1.1.0/pyproject.toml
+-rw-r--r--   0     1001      123     2890 2023-06-10 12:17:57.000000 maturin-1.1.0/setup.py
+-rw-r--r--   0     1001      123    19534 2023-06-10 12:17:57.000000 maturin-1.1.0/src/auditwheel/audit.rs
+-rw-r--r--   0     1001      123    53261 2023-06-10 12:17:57.000000 maturin-1.1.0/src/auditwheel/manylinux-policy.json
+-rw-r--r--   0     1001      123      242 2023-06-10 12:17:57.000000 maturin-1.1.0/src/auditwheel/mod.rs
+-rw-r--r--   0     1001      123     1862 2023-06-10 12:17:57.000000 maturin-1.1.0/src/auditwheel/musllinux-policy.json
+-rw-r--r--   0     1001      123     1389 2023-06-10 12:17:57.000000 maturin-1.1.0/src/auditwheel/musllinux.rs
+-rw-r--r--   0     1001      123     3777 2023-06-10 12:17:57.000000 maturin-1.1.0/src/auditwheel/patchelf.rs
+-rw-r--r--   0     1001      123     4602 2023-06-10 12:17:57.000000 maturin-1.1.0/src/auditwheel/platform_tag.rs
+-rw-r--r--   0     1001      123     5393 2023-06-10 12:17:57.000000 maturin-1.1.0/src/auditwheel/policy.rs
+-rw-r--r--   0     1001      123     1169 2023-06-10 12:17:57.000000 maturin-1.1.0/src/auditwheel/repair.rs
+-rw-r--r--   0     1001      123    47737 2023-06-10 12:17:57.000000 maturin-1.1.0/src/build_context.rs
+-rw-r--r--   0     1001      123    57656 2023-06-10 12:17:57.000000 maturin-1.1.0/src/build_options.rs
+-rw-r--r--   0     1001      123     5407 2023-06-10 12:17:57.000000 maturin-1.1.0/src/cargo_toml.rs
+-rw-r--r--   0     1001      123    34506 2023-06-10 12:17:57.000000 maturin-1.1.0/src/ci.rs
+-rw-r--r--   0     1001      123    24297 2023-06-10 12:17:57.000000 maturin-1.1.0/src/compile.rs
+-rw-r--r--   0     1001      123     8342 2023-06-10 12:17:57.000000 maturin-1.1.0/src/cross_compile.rs
+-rw-r--r--   0     1001      123     7375 2023-06-10 12:17:57.000000 maturin-1.1.0/src/develop.rs
+-rw-r--r--   0     1001      123     2251 2023-06-10 12:17:57.000000 maturin-1.1.0/src/lib.rs
+-rw-r--r--   0     1001      123    16822 2023-06-10 12:17:57.000000 maturin-1.1.0/src/main.rs
+-rw-r--r--   0     1001      123    32462 2023-06-10 12:17:57.000000 maturin-1.1.0/src/metadata.rs
+-rw-r--r--   0     1001      123    45502 2023-06-10 12:17:57.000000 maturin-1.1.0/src/module_writer.rs
+-rw-r--r--   0     1001      123     8203 2023-06-10 12:17:57.000000 maturin-1.1.0/src/new_project.rs
+-rw-r--r--   0     1001      123    16869 2023-06-10 12:17:57.000000 maturin-1.1.0/src/project_layout.rs
+-rw-r--r--   0     1001      123    18607 2023-06-10 12:17:57.000000 maturin-1.1.0/src/pyproject_toml.rs
+-rw-r--r--   0     1001      123    27618 2023-06-10 12:17:57.000000 maturin-1.1.0/src/python_interpreter/config.rs
+-rw-r--r--   0     1001      123     1514 2023-06-10 12:17:57.000000 maturin-1.1.0/src/python_interpreter/get_interpreter_metadata.py
+-rw-r--r--   0     1001      123    38393 2023-06-10 12:17:57.000000 maturin-1.1.0/src/python_interpreter/mod.rs
+-rw-r--r--   0     1001      123    35086 2023-06-10 12:17:57.000000 maturin-1.1.0/src/source_distribution.rs
+-rw-r--r--   0     1001      123    18929 2023-06-10 12:17:57.000000 maturin-1.1.0/src/target.rs
+-rw-r--r--   0     1001      123      686 2023-06-10 12:17:57.000000 maturin-1.1.0/src/templates/.gitignore.j2
+-rw-r--r--   0     1001      123      518 2023-06-10 12:17:57.000000 maturin-1.1.0/src/templates/Cargo.toml.j2
+-rw-r--r--   0     1001      123      149 2023-06-10 12:17:57.000000 maturin-1.1.0/src/templates/__init__.py.j2
+-rw-r--r--   0     1001      123      123 2023-06-10 12:17:57.000000 maturin-1.1.0/src/templates/build.rs.j2
+-rw-r--r--   0     1001      123       47 2023-06-10 12:17:57.000000 maturin-1.1.0/src/templates/example.udl.j2
+-rw-r--r--   0     1001      123      722 2023-06-10 12:17:57.000000 maturin-1.1.0/src/templates/lib.rs.j2
+-rw-r--r--   0     1001      123       45 2023-06-10 12:17:57.000000 maturin-1.1.0/src/templates/main.rs.j2
+-rw-r--r--   0     1001      123      859 2023-06-10 12:17:57.000000 maturin-1.1.0/src/templates/pyproject.toml.j2
+-rw-r--r--   0     1001      123    22914 2023-06-10 12:17:57.000000 maturin-1.1.0/src/upload.rs
+-rwxr-xr-x   0     1001      123      974 2023-06-10 12:17:57.000000 maturin-1.1.0/test-dockerfile.sh
+-rw-r--r--   0        0        0    18130 1970-01-01 00:00:00.000000 maturin-1.1.0/PKG-INFO
```

### Comparing `maturin-1.0.1/Cargo.toml` & `maturin-1.1.0/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [package]
 authors = ["konstin <konstin@mailbox.org>", "messense <messense@icloud.com>"]
 name = "maturin"
-version = "1.0.1"
+version = "1.1.0"
 description = "Build and publish crates with pyo3, rust-cpython and cffi bindings as well as rust binaries as python packages"
 exclude = ["test-crates/**/*", "sysconfig/*", "test-data/*", "ci/*", "tests/*", "guide/*", ".github/*"]
 homepage = "https://github.com/pyo3/maturin"
 readme = "README.md"
 repository = "https://github.com/pyo3/maturin"
 license = "MIT OR Apache-2.0"
 keywords = ["python", "cffi", "packaging", "pypi", "pyo3"]
@@ -43,25 +43,25 @@
 fs-err = "2.5.0"
 fat-macho = { version = "0.4.6", default-features = false }
 once_cell = "1.7.2"
 rustc_version = "0.4.0"
 semver = "1.0.13"
 target-lexicon = "0.12.0"
 indexmap = "1.9.3"
-pyproject-toml = "0.6.0"
+pyproject-toml = "0.6.1"
 python-pkginfo = "0.5.5"
 textwrap = "0.16.0"
 ignore = "0.4.20"
 itertools = "0.10.5"
 lddtree = "0.3.2"
 cc = "1.0.72"
 dunce = "1.0.2"
 normpath = "1.0.0"
-pep440_rs = { version = "0.3.3", features = ["serde"] }
-pep508_rs = { version = "0.1.1", features = ["serde"] }
+pep440_rs = { version = "0.3.6", features = ["serde"] }
+pep508_rs = { version = "0.2.1", features = ["serde"] }
 same-file = "1.0.6"
 time = "0.3.17"
 
 # cli
 clap = { version = "4.0.0", features = ["derive", "env", "wrap_help"] }
 clap_complete_command = { version = "0.5.1", optional = true }
 
@@ -72,15 +72,15 @@
 # log
 tracing = "0.1.36"
 tracing-subscriber = { version = "0.3.15", features = ["env-filter"], optional = true }
 
 # project scaffolding, maturin new/init/generate-ci
 dialoguer = { version = "0.10.2", default-features = false, optional = true }
 console = { version = "0.15.4", optional = true }
-minijinja = { version = "0.33.0", optional = true }
+minijinja = { version = "0.34.0", optional = true }
 
 # upload
 bytesize = { version = "1.0.1", optional = true }
 configparser = { version = "3.0.0", optional = true }
 dirs = { version = "5.0.0", optional = true }
 multipart = { version = "0.18.0", features = ["client"], default-features = false, optional = true }
 ureq = { version = "2.6.1", features = ["gzip", "json", "socks-proxy"], default-features = false, optional = true }
```

### Comparing `maturin-1.0.1/.cirrus.yml` & `maturin-1.1.0/.cirrus.yml`

 * *Files identical despite different names*

### Comparing `maturin-1.0.1/Cargo.lock` & `maturin-1.1.0/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -226,17 +226,17 @@
  "serde",
  "serde_json",
  "thiserror",
 ]
 
 [[package]]
 name = "cbindgen"
-version = "0.24.3"
+version = "0.24.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a6358dedf60f4d9b8db43ad187391afe959746101346fe51bb978126bec61dfb"
+checksum = "4b922faaf31122819ec80c4047cc684c6979a087366c069611e33649bf98e18d"
 dependencies = [
  "heck",
  "indexmap",
  "log",
  "proc-macro2",
  "quote",
  "serde",
@@ -261,17 +261,17 @@
  "byteorder",
  "fnv",
  "uuid",
 ]
 
 [[package]]
 name = "cfg-expr"
-version = "0.15.1"
+version = "0.15.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c8790cf1286da485c72cf5fc7aeba308438800036ec67d89425924c4807268c9"
+checksum = "e70d3ad08698a0568b0562f22710fe6bfc1f4a61a367c77d0398c562eadd453a"
 dependencies = [
  "smallvec",
 ]
 
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
@@ -613,25 +613,14 @@
 checksum = "071a31f4ee85403370b58aca746f01041ede6f0da2730960ad001edc2b71b394"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
 name = "errno"
-version = "0.2.8"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f639046355ee4f37944e44f60642c6f3a7efa3cf6b78c78a0d989a8ce6c396a1"
-dependencies = [
- "errno-dragonfly",
- "libc",
- "winapi",
-]
-
-[[package]]
-name = "errno"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4bcfec3a70f97c962c307b2d2c56e358cf1d00b558d74262b5f929ee8cc7e73a"
 dependencies = [
  "errno-dragonfly",
  "libc",
  "windows-sys 0.48.0",
@@ -669,15 +658,15 @@
 name = "filetime"
 version = "0.2.21"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5cbc844cecaee9d4443931972e1289c8ff485cb4cc2767cb03ca139ed6885153"
 dependencies = [
  "cfg-if",
  "libc",
- "redox_syscall",
+ "redox_syscall 0.2.16",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "flate2"
 version = "1.0.26"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -706,17 +695,17 @@
 name = "foreign-types-shared"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "00b0228411908ca8685dba7fc2cdd70ec9990a6e753e89b6ac91a84c40fbaf4b"
 
 [[package]]
 name = "form_urlencoded"
-version = "1.1.0"
+version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a9c384f161156f5260c24a097c56119f9be8c798586aecc13afbcbe7b7e26bf8"
+checksum = "a62bc1cf6f830c2ec14a513a9fb124d0a213a629668a4186f329db21fe045652"
 dependencies = [
  "percent-encoding",
 ]
 
 [[package]]
 name = "fs-err"
 version = "2.9.0"
@@ -731,17 +720,17 @@
 dependencies = [
  "typenum",
  "version_check",
 ]
 
 [[package]]
 name = "getrandom"
-version = "0.2.9"
+version = "0.2.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c85e1d9ab2eadba7e5040d4e09cbd6d072b76a557ad64e797c2cb9d4da21d7e4"
+checksum = "be4136b2a15dd319360be1c07d9933517ccf0be8f16bf62a3bee4f0d618df427"
 dependencies = [
  "cfg-if",
  "libc",
  "wasi",
 ]
 
 [[package]]
@@ -827,17 +816,17 @@
 dependencies = [
  "humantime",
  "serde",
 ]
 
 [[package]]
 name = "idna"
-version = "0.3.0"
+version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e14ddfc70884202db2244c223200c204c2bda1bc6e0998d11b5e024d657209e6"
+checksum = "7d20d6b07bfbc108882d88ed8e37d39636dcc260e15e30c45e6ba089610b917c"
 dependencies = [
  "unicode-bidi",
  "unicode-normalization",
 ]
 
 [[package]]
 name = "ignore"
@@ -865,21 +854,22 @@
  "autocfg",
  "hashbrown",
  "serde",
 ]
 
 [[package]]
 name = "indicatif"
-version = "0.17.3"
+version = "0.17.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cef509aa9bc73864d6756f0d34d35504af3cf0844373afe9b8669a5b8005a729"
+checksum = "8ff8cc23a7393a397ed1d7f56e6365cba772aba9f9912ab968b03043c395d057"
 dependencies = [
  "console",
+ "instant",
  "number_prefix",
- "portable-atomic 0.3.20",
+ "portable-atomic",
  "unicode-width",
 ]
 
 [[package]]
 name = "indoc"
 version = "2.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -909,15 +899,15 @@
 name = "is-terminal"
 version = "0.4.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "adcf93614601c8129ddf72e2d5633df827ba6551541c6d8c59520a371475be1f"
 dependencies = [
  "hermit-abi 0.3.1",
  "io-lifetimes",
- "rustix 0.37.19",
+ "rustix",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "itertools"
 version = "0.10.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -969,36 +959,30 @@
  "fs-err",
  "glob",
  "goblin",
 ]
 
 [[package]]
 name = "libc"
-version = "0.2.144"
+version = "0.2.146"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2b00cc1c228a6782d0f076e7b232802e0c5689d41bb5df366f2a6b6621cfdfe1"
+checksum = "f92be4933c13fd498862a9e02a3055f8a8d9c039ce33db97306fd5a6caa7f29b"
 
 [[package]]
 name = "linux-keyutils"
 version = "0.2.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3f27bb67f6dd1d0bb5ab582868e4f65052e58da6401188a08f0da09cf512b84b"
 dependencies = [
  "bitflags",
  "libc",
 ]
 
 [[package]]
 name = "linux-raw-sys"
-version = "0.1.4"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f051f77a7c8e6957c0696eac88f26b0117e54f52d3fc682ab19397a8812846a4"
-
-[[package]]
-name = "linux-raw-sys"
 version = "0.3.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ef53942eb7bf7ff43a617b3e2c1c4a5ecf5944a7c1bc12d7ee39bbb15e5c1519"
 
 [[package]]
 name = "lock_api"
 version = "0.4.9"
@@ -1007,20 +991,17 @@
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "log"
-version = "0.4.17"
+version = "0.4.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "abb12e687cfb44aa40f41fc3978ef76448f9b6038cad6aef4259d3c095a2382e"
-dependencies = [
- "cfg-if",
-]
+checksum = "518ef76f2f87365916b142844c16d8fefd85039bc5699050210a7778ee1cd1de"
 
 [[package]]
 name = "lzxd"
 version = "0.1.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "784462f20dddd9dfdb45de963fa4ad4a288cb10a7889ac5d2c34fb6481c6b213"
 
@@ -1042,15 +1023,15 @@
 checksum = "8263075bb86c5a1b1427b5ae862e8889656f126e9f77c484496e8b47cf5c5558"
 dependencies = [
  "regex-automata",
 ]
 
 [[package]]
 name = "maturin"
-version = "1.0.1"
+version = "1.1.0"
 dependencies = [
  "anyhow",
  "base64 0.21.2",
  "bytesize",
  "cargo-config2",
  "cargo-options",
  "cargo-xwin",
@@ -1144,17 +1125,17 @@
 dependencies = [
  "mime",
  "unicase",
 ]
 
 [[package]]
 name = "minijinja"
-version = "0.33.0"
+version = "0.34.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "933dc6e6e1f909926a2f6bf72ba8b8d6e38ab4f92778c77ea898001e044a30eb"
+checksum = "75aa91cba87dcad6af3e53bc7adb9c99755eba2d49b6c5f10dbcc79d4727c1bd"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "minimal-lexical"
 version = "0.2.1"
@@ -1262,23 +1243,23 @@
 name = "number_prefix"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "830b246a0e5f20af87141b25c173cd1b609bd7779a4617d6ec582abaf90870f3"
 
 [[package]]
 name = "once_cell"
-version = "1.17.1"
+version = "1.18.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b7e5500299e16ebb147ae15a00a942af264cf3688f47923b8fc2cd5858f23ad3"
+checksum = "dd8b5dd2ae5ed71462c540258bedcb51965123ad7e7ccf4b9a8cafaa4a63576d"
 
 [[package]]
 name = "openssl"
-version = "0.10.52"
+version = "0.10.54"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "01b8574602df80f7b85fdfc5392fa884a4e3b3f4f35402c070ab34c3d3f78d56"
+checksum = "69b3f656a17a6cbc115b5c7a40c616947d213ba182135b014d6051b73ab6f019"
 dependencies = [
  "bitflags",
  "cfg-if",
  "foreign-types",
  "libc",
  "once_cell",
  "openssl-macros",
@@ -1300,26 +1281,26 @@
 name = "openssl-probe"
 version = "0.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ff011a302c396a5197692431fc1948019154afc178baf7d8e37367442a4601cf"
 
 [[package]]
 name = "openssl-src"
-version = "111.25.3+1.1.1t"
+version = "111.26.0+1.1.1u"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "924757a6a226bf60da5f7dd0311a34d2b52283dd82ddeb103208ddc66362f80c"
+checksum = "efc62c9f12b22b8f5208c23a7200a442b2e5999f8bdf80233852122b5a4f6f37"
 dependencies = [
  "cc",
 ]
 
 [[package]]
 name = "openssl-sys"
-version = "0.9.87"
+version = "0.9.88"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8e17f59264b2809d77ae94f0e1ebabc434773f370d6ca667bd223ea10e06cc7e"
+checksum = "c2ce0f250f34a308dcfdbb351f511359857d4ed2134ba715a4eadd46e1ffd617"
 dependencies = [
  "cc",
  "libc",
  "openssl-src",
  "pkg-config",
  "vcpkg",
 ]
@@ -1369,15 +1350,15 @@
 name = "parking_lot_core"
 version = "0.9.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ba1ef8814b5c993410bb3adfad7a5ed269563e4a2f90c41f5d85be7fb47133bf"
 dependencies = [
  "cfg-if",
  "libc",
- "redox_syscall",
+ "redox_syscall 0.2.16",
  "smallvec",
  "windows-sys 0.42.0",
 ]
 
 [[package]]
 name = "path-slash"
 version = "0.2.1"
@@ -1395,33 +1376,33 @@
  "serde",
  "tracing",
  "unicode-width",
 ]
 
 [[package]]
 name = "pep508_rs"
-version = "0.1.5"
+version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "969679a29dfdc8278a449f75b3dd45edf57e649bd59f7502429c2840751c46d8"
+checksum = "c0713d7bb861ca2b7d4c50a38e1f31a4b63a2e2df35ef1e5855cc29e108453e2"
 dependencies = [
  "once_cell",
  "pep440_rs",
  "regex",
  "serde",
  "thiserror",
  "tracing",
  "unicode-width",
  "url",
 ]
 
 [[package]]
 name = "percent-encoding"
-version = "2.2.0"
+version = "2.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "478c572c3d73181ff3c2539045f6eb99e5491218eae919370993b890cdbdd98e"
+checksum = "9b2a4787296e9989611394c33f193f676704af1686e70b8f8033ab5ba9a35a94"
 
 [[package]]
 name = "pin-project-lite"
 version = "0.2.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e0a7ae3ac2f1173085d398531c705756c94a4c56843785df85a60c1a0afac116"
 
@@ -1445,26 +1426,17 @@
 dependencies = [
  "libc",
  "winapi",
 ]
 
 [[package]]
 name = "portable-atomic"
-version = "0.3.20"
+version = "1.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e30165d31df606f5726b090ec7592c308a0eaf61721ff64c9a3018e344a8753e"
-dependencies = [
- "portable-atomic 1.3.2",
-]
-
-[[package]]
-name = "portable-atomic"
-version = "1.3.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dc59d1bcc64fc5d021d67521f818db868368028108d37f0e98d74e33f68297b5"
+checksum = "767eb9f07d4a5ebcb39bbf2d452058a93c011373abf6832e24194a1c3f004794"
 
 [[package]]
 name = "ppv-lite86"
 version = "0.2.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b40af805b3121feab8a3c29f04d8ad262fa8e0561883e7653e024ae4479e6de"
 
@@ -1478,17 +1450,17 @@
  "diff",
  "output_vt100",
  "yansi",
 ]
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.59"
+version = "1.0.60"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6aeca18b86b413c660b781aa319e4e2648a3e6f9eadc9b47e9038e6fe9f3451b"
+checksum = "dec2b086b7a862cf4de201096214fa870344cf922b2b30c167badb3af3195406"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "psm"
 version = "0.1.21"
@@ -1496,17 +1468,17 @@
 checksum = "5787f7cda34e3033a72192c018bc5883100330f362ef279a8cbccfce8bb4e874"
 dependencies = [
  "cc",
 ]
 
 [[package]]
 name = "pyproject-toml"
-version = "0.6.0"
+version = "0.6.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f04dbbb336bd88583943c7cd973a32fed323578243a7569f40cb0c7da673321b"
+checksum = "ee79feaa9d31e1c417e34219e610b67db4e786ce9b49d77dda549640abb9dc5f"
 dependencies = [
  "indexmap",
  "pep440_rs",
  "pep508_rs",
  "serde",
  "toml 0.7.4",
 ]
@@ -1599,21 +1571,30 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fb5a58c1855b4b6819d59012155603f0b22ad30cad752600aadfcb695265519a"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
+name = "redox_syscall"
+version = "0.3.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "567664f262709473930a4bf9e51bf2ebf3348f2e748ccc50dea20646858f8f29"
+dependencies = [
+ "bitflags",
+]
+
+[[package]]
 name = "redox_users"
 version = "0.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b033d837a7cf162d7993aded9304e30a83213c648b6e389db233191f891e5c2b"
 dependencies = [
  "getrandom",
- "redox_syscall",
+ "redox_syscall 0.2.16",
  "thiserror",
 ]
 
 [[package]]
 name = "regex"
 version = "1.7.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -1675,37 +1656,23 @@
 checksum = "bfa0f585226d2e68097d4f95d113b15b83a82e819ab25717ec0590d9584ef366"
 dependencies = [
  "semver",
 ]
 
 [[package]]
 name = "rustix"
-version = "0.36.7"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d4fdebc4b395b7fbb9ab11e462e20ed9051e7b16e42d24042c776eca0ac81b03"
-dependencies = [
- "bitflags",
- "errno 0.2.8",
- "io-lifetimes",
- "libc",
- "linux-raw-sys 0.1.4",
- "windows-sys 0.42.0",
-]
-
-[[package]]
-name = "rustix"
 version = "0.37.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "acf8729d8542766f1b2cf77eb034d52f40d375bb8b615d0b147089946e16613d"
 dependencies = [
  "bitflags",
- "errno 0.3.1",
+ "errno",
  "io-lifetimes",
  "libc",
- "linux-raw-sys 0.3.8",
+ "linux-raw-sys",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "rustls"
 version = "0.20.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -1822,26 +1789,26 @@
 checksum = "bebd363326d05ec3e2f532ab7660680f3b02130d780c299bca73469d521bc0ed"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "serde"
-version = "1.0.163"
+version = "1.0.164"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2113ab51b87a539ae008b5c6c02dc020ffa39afd2d83cffcb3f4eb2722cebec2"
+checksum = "9e8c8cf938e98f769bc164923b06dce91cea1751522f46f8466461af04c9027d"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.163"
+version = "1.0.164"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8c805777e3930c8883389c602315a24224bcc738b63905ef87cd1420353ea93e"
+checksum = "d9735b638ccc51c28bf6914d90a2e9725b377144fc612c49a611fddd1b631d68"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 2.0.18",
 ]
 
 [[package]]
@@ -1940,17 +1907,17 @@
  "walkdir",
  "windows-sys 0.42.0",
  "yansi",
 ]
 
 [[package]]
 name = "snapbox-macros"
-version = "0.3.1"
+version = "0.3.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "485e65c1203eb37244465e857d15a26d3a85a5410648ccb53b18bd44cb3a7336"
+checksum = "eaaf09df9f0eeae82be96290918520214530e738a7fe5a351b0f24cf77c0ca31"
 
 [[package]]
 name = "socks"
 version = "0.3.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f0c3dbbd9ae980613c6dd8e28a9407b50509d3803b57624d5dfe8315218cd58b"
 dependencies = [
@@ -2027,23 +1994,24 @@
 name = "target-lexicon"
 version = "0.12.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fd1ba337640d60c3e96bc6f0638a939b9c9a7f2c316a1598c279828b3d1dc8c5"
 
 [[package]]
 name = "tempfile"
-version = "3.4.0"
+version = "3.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "af18f7ae1acd354b992402e9ec5864359d693cd8a79dcbef59f76891701c1e95"
+checksum = "31c0432476357e58790aaa47a8efb0c5138f137343f3b5f23bd36a27e3b0a6d6"
 dependencies = [
+ "autocfg",
  "cfg-if",
  "fastrand",
- "redox_syscall",
- "rustix 0.36.7",
- "windows-sys 0.42.0",
+ "redox_syscall 0.3.5",
+ "rustix",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "termcolor"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "be55cf8942feac5c765c2c993422806843c9a9a45d4d5c407ad6dd2ea95eb9b6"
@@ -2053,15 +2021,15 @@
 
 [[package]]
 name = "terminal_size"
 version = "0.2.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8e6bf6f19e9f8ed8d4048dc22981458ebcf406d67e94cd422e5ecd73d63b3237"
 dependencies = [
- "rustix 0.37.19",
+ "rustix",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "textwrap"
 version = "0.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -2365,17 +2333,17 @@
  "url",
  "webpki",
  "webpki-roots",
 ]
 
 [[package]]
 name = "url"
-version = "2.3.1"
+version = "2.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0d68c799ae75762b8c3fe375feb6600ef5602c883c5d21eb51c09f22b83c4643"
+checksum = "50bff7831e19200a85b17131d085c25d7811bc4e186efdaf54bbd132994a88cb"
 dependencies = [
  "form_urlencoded",
  "idna",
  "percent-encoding",
  "serde",
 ]
```

### Comparing `maturin-1.0.1/Changelog.md` & `maturin-1.1.0/Changelog.md`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,21 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html) (for the cli, not for the crate).
 
 ## [Unreleased]
 
+## [1.1.0] - 2023-06-10
+
+* Add basic support for GraalPy in [#1645](https://github.com/PyO3/maturin/pull/1645)
+* Refactor abi tag to use `EXT_SUFFIX` in [#1648](https://github.com/PyO3/maturin/pull/1648)
+* Add Linux loongarch64 architecture support in [#1653](https://github.com/PyO3/maturin/pull/1653)
+* Add `--skip-install` option to `maturin develop` in [#1654](https://github.com/PyO3/maturin/pull/1654)
+
 ## [1.0.1] - 2023-05-28
 
 * Add more Python 3.12 sysconfigs in [#1629](https://github.com/PyO3/maturin/pull/1629)
 * Fix panicking when no cargo build targets are selected in [#1635](https://github.com/PyO3/maturin/pull/1635)
 
 ## [1.0.0] - 2023-05-23
 
@@ -874,15 +881,16 @@
 
  * Show a progress bar for cargo's compile progress
 
 ## 0.1.0 - 2018-08-22
 
  * Initial Release
 
-[Unreleased]: https://github.com/pyo3/maturin/compare/v1.0.1...HEAD
+[Unreleased]: https://github.com/pyo3/maturin/compare/v1.1.0...HEAD
+[1.1.0]: https://github.com/pyo3/maturin/compare/v1.0.1...v1.1.0
 [1.0.1]: https://github.com/pyo3/maturin/compare/v1.0.0...v1.0.1
 [1.0.0]: https://github.com/pyo3/maturin/compare/v0.15.3...v1.0.0
 [0.15.3]: https://github.com/pyo3/maturin/compare/v0.15.2...v0.15.3
 [0.15.2]: https://github.com/pyo3/maturin/compare/v0.15.1...v0.15.2
 [0.15.1]: https://github.com/pyo3/maturin/compare/v0.15.0...v0.15.1
 [0.15.0]: https://github.com/pyo3/maturin/compare/v0.14.17...v0.15.0
 [0.14.17]: https://github.com/pyo3/maturin/compare/v0.14.16...v0.14.17
```

### Comparing `maturin-1.0.1/Code-of-Conduct.md` & `maturin-1.1.0/Code-of-Conduct.md`

 * *Files identical despite different names*

### Comparing `maturin-1.0.1/Dockerfile` & `maturin-1.1.0/Dockerfile`

 * *Files identical despite different names*

### Comparing `maturin-1.0.1/README.md` & `maturin-1.1.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 [![PyPI](https://img.shields.io/pypi/v/maturin.svg?logo=python&style=flat-square)](https://pypi.org/project/maturin)
 [![Maturin User Guide](https://img.shields.io/badge/user-guide-brightgreen?logo=readthedocs&style=flat-square)](https://maturin.rs)
 [![Chat on Gitter](https://img.shields.io/gitter/room/nwjs/nw.js.svg?logo=gitter&style=flat-square)](https://gitter.im/PyO3/Lobby)
 
 Build and publish crates with pyo3, rust-cpython, cffi and uniffi bindings as well as rust binaries as python packages.
 
 This project is meant as a zero configuration replacement for [setuptools-rust](https://github.com/PyO3/setuptools-rust) and [milksnake](https://github.com/getsentry/milksnake).
-It supports building wheels for python 3.5+ on windows, linux, mac and freebsd, can upload them to [pypi](https://pypi.org/) and has basic pypy support.
+It supports building wheels for python 3.5+ on windows, linux, mac and freebsd, can upload them to [pypi](https://pypi.org/) and has basic pypy and graalpy support.
 
 Check out the [User Guide](https://maturin.rs/)!
 
 ## Usage
 
 You can either download binaries from the [latest release](https://github.com/PyO3/maturin/releases/latest) or install it with pip:
 
@@ -270,14 +270,15 @@
 
 ## Examples
 
 * [ballista-python](https://github.com/apache/arrow-ballista-python) - A Python library that binds to Apache Arrow distributed query engine Ballista
 * [connector-x](https://github.com/sfu-db/connector-x/tree/main/connectorx-python) - ConnectorX enables you to load data from databases into Python in the fastest and most memory efficient way
 * [datafusion-python](https://github.com/apache/arrow-datafusion-python) - a Python library that binds to Apache Arrow in-memory query engine DataFusion
 * [deltalake-python](https://github.com/delta-io/delta-rs/tree/main/python) - Native Delta Lake Python binding based on delta-rs with Pandas integration
+* [opendal](https://github.com/apache/incubator-opendal/tree/main/bindings/python) - OpenDAL Python Binding to access data freely
 * [orjson](https://github.com/ijl/orjson) - A fast, correct JSON library for Python
 * [polars](https://github.com/pola-rs/polars/tree/master/py-polars) - Fast multi-threaded DataFrame library in Rust | Python | Node.js
 * [pydantic-core](https://github.com/pydantic/pydantic-core) - Core validation logic for pydantic written in Rust
 * [pyrus-cramjam](https://github.com/milesgranger/pyrus-cramjam) - Thin Python wrapper to de/compression algorithms in Rust
 * [pyxel](https://github.com/kitao/pyxel) - A retro game engine for Python
 * [roapi](https://github.com/roapi/roapi) - ROAPI automatically spins up read-only APIs for static datasets without requiring you to write a single line of code
 * [robyn](https://github.com/sansyrox/robyn) -  A fast and extensible async python web server with a Rust runtime
```

### Comparing `maturin-1.0.1/deny.toml` & `maturin-1.1.0/deny.toml`

 * *Files 1% similar despite different names*

```diff
@@ -181,15 +181,14 @@
     #{ name = "ansi_term", version = "=0.11.0" },
     { name = "base64", version = "0.13.1" },
     # from cbindgen
     { name = "toml", version = "0.5.11" },
     { name = "syn" },
     { name = "rustix", version = "0.36.7" },
     { name = "linux-raw-sys", version = "0.1.4" },
-    { name = "portable-atomic", version = "0.3.20" },
 ]
 # Similarly to `skip` allows you to skip certain crates during duplicate
 # detection. Unlike skip, it also includes the entire tree of transitive
 # dependencies starting at the specified crate, up to a certain depth, which is
 # by default infinite
 skip-tree = [
     #{ name = "ansi_term", version = "=0.11.0", depth = 20 },
```

### Comparing `maturin-1.0.1/license-apache` & `maturin-1.1.0/license-apache`

 * *Files identical despite different names*

### Comparing `maturin-1.0.1/license-mit` & `maturin-1.1.0/license-mit`

 * *Files identical despite different names*

### Comparing `maturin-1.0.1/maturin/__init__.py` & `maturin-1.1.0/maturin/__init__.py`

 * *Files identical despite different names*

### Comparing `maturin-1.0.1/maturin/__main__.py` & `maturin-1.1.0/maturin/__main__.py`

 * *Files identical despite different names*

### Comparing `maturin-1.0.1/maturin/import_hook.py` & `maturin-1.1.0/maturin/import_hook.py`

 * *Files identical despite different names*

### Comparing `maturin-1.0.1/noxfile.py` & `maturin-1.1.0/noxfile.py`

 * *Files identical despite different names*

### Comparing `maturin-1.0.1/pyproject.toml` & `maturin-1.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `maturin-1.0.1/setup.py` & `maturin-1.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `maturin-1.0.1/src/auditwheel/audit.rs` & `maturin-1.1.0/src/auditwheel/audit.rs`

 * *Files identical despite different names*

### Comparing `maturin-1.0.1/src/auditwheel/manylinux-policy.json` & `maturin-1.1.0/src/auditwheel/manylinux-policy.json`

 * *Files identical despite different names*

### Comparing `maturin-1.0.1/src/auditwheel/musllinux-policy.json` & `maturin-1.1.0/src/auditwheel/musllinux-policy.json`

 * *Files identical despite different names*

### Comparing `maturin-1.0.1/src/auditwheel/musllinux.rs` & `maturin-1.1.0/src/auditwheel/musllinux.rs`

 * *Files identical despite different names*

### Comparing `maturin-1.0.1/src/auditwheel/patchelf.rs` & `maturin-1.1.0/src/auditwheel/patchelf.rs`

 * *Files identical despite different names*

### Comparing `maturin-1.0.1/src/auditwheel/platform_tag.rs` & `maturin-1.1.0/src/auditwheel/platform_tag.rs`

 * *Files identical despite different names*

### Comparing `maturin-1.0.1/src/auditwheel/policy.rs` & `maturin-1.1.0/src/auditwheel/policy.rs`

 * *Files identical despite different names*

### Comparing `maturin-1.0.1/src/auditwheel/repair.rs` & `maturin-1.1.0/src/auditwheel/repair.rs`

 * *Files identical despite different names*

### Comparing `maturin-1.0.1/src/build_context.rs` & `maturin-1.1.0/src/build_context.rs`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     /// The String is the name of the bindings
     /// providing crate, e.g. pyo3, the number is the minimum minor python version
     Bin(Option<(String, usize)>),
     /// A native module with pyo3 or rust-cpython bindings. The String is the name of the bindings
     /// providing crate, e.g. pyo3, the number is the minimum minor python version
     Bindings(String, usize),
     /// `Bindings`, but specifically for pyo3 with feature flags that allow building a single wheel
-    /// for all cpython versions (pypy still needs multiple versions).
+    /// for all cpython versions (pypy & graalpy still need multiple versions).
     /// The numbers are the minimum major and minor version
     BindingsAbi3(u8, u8),
     /// A native module with c bindings, i.e. `#[no_mangle] extern "C" <some item>`
     Cffi,
     /// A native module generated from uniffi
     UniFfi,
 }
@@ -230,15 +230,17 @@
                         *minor,
                     )?);
                 }
                 if !non_abi3_interps.is_empty() {
                     let interp_names: HashSet<_> = non_abi3_interps
                         .iter()
                         .map(|interp| match interp.interpreter_kind {
-                            InterpreterKind::CPython => interp.implementation_name.to_string(),
+                            InterpreterKind::CPython | InterpreterKind::GraalPy => {
+                                interp.implementation_name.to_string()
+                            }
                             InterpreterKind::PyPy => "PyPy".to_string(),
                         })
                         .collect();
                     eprintln!(
                         "⚠️ Warning: {} does not yet support abi3 so the build artifacts will be version-specific.",
                         interp_names.iter().join(", ")
                     );
```

### Comparing `maturin-1.0.1/src/build_options.rs` & `maturin-1.1.0/src/build_options.rs`

 * *Files 1% similar despite different names*

```diff
@@ -257,35 +257,34 @@
                             .get("ABIFLAGS")
                             .map(ToString::to_string)
                             .unwrap_or_default();
                         let ext_suffix = sysconfig_data
                             .get("EXT_SUFFIX")
                             .context("syconfig didn't define an `EXT_SUFFIX` ಠ_ಠ")?;
                         let soabi = sysconfig_data.get("SOABI");
-                        let abi_tag =
-                            soabi.and_then(|abi| abi.split('-').nth(1).map(ToString::to_string));
                         let interpreter_kind = soabi
                             .and_then(|tag| {
                                 if tag.starts_with("pypy") {
                                     Some(InterpreterKind::PyPy)
                                 } else if tag.starts_with("cpython") {
                                     Some(InterpreterKind::CPython)
+                                } else if tag.starts_with("graalpy") {
+                                    Some(InterpreterKind::GraalPy)
                                 } else {
                                     None
                                 }
                             })
                             .context("unsupported Python interpreter")?;
                         interpreters.push(PythonInterpreter {
                             config: InterpreterConfig {
                                 major,
                                 minor,
                                 interpreter_kind,
                                 abiflags,
                                 ext_suffix: ext_suffix.to_string(),
-                                abi_tag,
                                 pointer_width: None,
                             },
                             executable: PathBuf::new(),
                             platform: None,
                             runnable: false,
                             implementation_name: interpreter_kind.to_string().to_ascii_lowercase(),
                             soabi: soabi.cloned(),
@@ -345,15 +344,14 @@
                         Ok(vec![PythonInterpreter {
                             config: InterpreterConfig {
                                 major: *major as usize,
                                 minor: *minor as usize,
                                 interpreter_kind: InterpreterKind::CPython,
                                 abiflags: "".to_string(),
                                 ext_suffix: ".pyd".to_string(),
-                                abi_tag: None,
                                 pointer_width: None,
                             },
                             executable: PathBuf::new(),
                             platform: None,
                             runnable: false,
                             implementation_name: "cpython".to_string(),
                             soabi: None,
@@ -372,15 +370,14 @@
                         Ok(vec![PythonInterpreter {
                             config: InterpreterConfig {
                                 major: *major as usize,
                                 minor: *minor as usize,
                                 interpreter_kind: InterpreterKind::CPython,
                                 abiflags: "".to_string(),
                                 ext_suffix: ".pyd".to_string(),
-                                abi_tag: None,
                                 pointer_width: None,
                             },
                             executable: PathBuf::new(),
                             platform: None,
                             runnable: false,
                             implementation_name: "cpython".to_string(),
                             soabi: None,
@@ -412,15 +409,14 @@
                         Ok(vec![PythonInterpreter {
                             config: InterpreterConfig {
                                 major: *major as usize,
                                 minor: *minor as usize,
                                 interpreter_kind: InterpreterKind::CPython,
                                 abiflags: "".to_string(),
                                 ext_suffix: "".to_string(),
-                                abi_tag: None,
                                 pointer_width: None,
                             },
                             executable: PathBuf::new(),
                             platform: None,
                             runnable: false,
                             implementation_name: "cpython".to_string(),
                             soabi: None,
@@ -559,14 +555,16 @@
                         Some(python) => vec![python.into()],
                         None => vec![PathBuf::from("python3")],
                     }
                 } else {
                     vec![PathBuf::from("python3")]
                 }
             } else {
+                // XXX: False positive clippy warning
+                #[allow(clippy::redundant_clone)]
                 self.interpreter.clone()
             };
             self.find_interpreters(&bridge, &interpreter, &target, None, generate_import_lib)?
         };
 
         if cargo_options.args.is_empty() {
             // if not supplied on command line, try pyproject.toml
@@ -1097,16 +1095,15 @@
 fn find_interpreter_in_host(
     bridge: &BridgeModel,
     interpreter: &[PathBuf],
     target: &Target,
     requires_python: Option<&VersionSpecifiers>,
 ) -> Result<Vec<PythonInterpreter>> {
     let interpreters = if !interpreter.is_empty() {
-        PythonInterpreter::check_executables(interpreter, target, bridge)
-            .context("The given list of python interpreters is invalid")?
+        PythonInterpreter::check_executables(interpreter, target, bridge)?
     } else {
         PythonInterpreter::find_all(target, bridge, requires_python)
             .context("Finding python interpreters failed")?
     };
 
     if interpreters.is_empty() {
         if let Some(requires_python) = requires_python {
@@ -1128,14 +1125,19 @@
         return Ok(PythonInterpreter::find_by_target(target, requires_python));
     }
     let mut interpreters = Vec::new();
     for interp in interpreter {
         let python = interp.display().to_string();
         let (python_impl, python_ver) = if let Some(ver) = python.strip_prefix("pypy") {
             (InterpreterKind::PyPy, ver.strip_prefix('-').unwrap_or(ver))
+        } else if let Some(ver) = python.strip_prefix("graalpy") {
+            (
+                InterpreterKind::GraalPy,
+                ver.strip_prefix('-').unwrap_or(ver),
+            )
         } else if let Some(ver) = python.strip_prefix("python") {
             (
                 InterpreterKind::CPython,
                 ver.strip_prefix('-').unwrap_or(ver),
             )
         } else if python
             .chars()
```

### Comparing `maturin-1.0.1/src/cargo_toml.rs` & `maturin-1.1.0/src/cargo_toml.rs`

 * *Files identical despite different names*

### Comparing `maturin-1.0.1/src/ci.rs` & `maturin-1.1.0/src/ci.rs`

 * *Files 2% similar despite different names*

```diff
@@ -236,43 +236,60 @@
                 ));
             }
             // job steps
             conf.push_str(
                 "    steps:
       - uses: actions/checkout@v3\n",
             );
-            // setup python on demand
-            if setup_python {
-                conf.push_str(
-                    "      - uses: actions/setup-python@v4
-        with:
-          python-version: '3.10'\n",
-                );
-                if matches!(platform, Platform::Windows) {
-                    conf.push_str("          architecture: ${{ matrix.target }}\n");
-                }
-            }
 
             // install pyodide-build for emscripten
             if matches!(platform, Platform::Emscripten) {
+                // install stable pyodide-build
                 conf.push_str("      - run: pip install pyodide-build\n");
-                conf.push_str("      - shell: bash\n        run: echo EMSCRIPTEN_VERSION=$(pyodide config get emscripten_version) >> $GITHUB_ENV\n");
+                // get the current python version for the installed pyodide-build
+                conf.push_str(
+                    "      - name: Get Emscripten and Python version info
+        shell: bash
+        run: |
+          echo EMSCRIPTEN_VERSION=$(pyodide config get emscripten_version) >> $GITHUB_ENV
+          echo PYTHON_VERSION=$(pyodide config get python_version | cut -d '.' -f 1-2) >> $GITHUB_ENV
+          pip uninstall -y pyodide-build\n",
+                );
                 conf.push_str(
                     "      - uses: mymindstorm/setup-emsdk@v12
         with:
           version: ${{ env.EMSCRIPTEN_VERSION }}
           actions-cache-folder: emsdk-cache\n",
                 );
+                conf.push_str(
+                    "      - uses: actions/setup-python@v4
+        with:
+          python-version: ${{ env.PYTHON_VERSION }}\n",
+                );
+                // install pyodide-build again in the right Python version
+                conf.push_str("      - run: pip install pyodide-build\n");
+            } else {
+                // setup python on demand
+                if setup_python {
+                    conf.push_str(
+                        "      - uses: actions/setup-python@v4
+        with:
+          python-version: '3.10'\n",
+                    );
+                    if matches!(platform, Platform::Windows) {
+                        conf.push_str("          architecture: ${{ matrix.target }}\n");
+                    }
+                }
             }
 
             // build wheels
             let mut maturin_args = if is_abi3 || (is_bin && !setup_python) {
                 Vec::new()
             } else if matches!(platform, Platform::Emscripten) {
-                vec!["-i".to_string(), "3.10".to_string()]
+                vec!["-i".to_string(), "${{ env.PYTHON_VERSION }}".to_string()]
             } else {
                 vec!["--find-interpreter".to_string()]
             };
             if let Some(manifest_path) = self.manifest_path.as_ref() {
                 if manifest_path != Path::new("Cargo.toml") {
                     maturin_args.push("--manifest-path".to_string());
                     maturin_args.push(manifest_path.display().to_string())
```

### Comparing `maturin-1.0.1/src/compile.rs` & `maturin-1.1.0/src/compile.rs`

 * *Files 1% similar despite different names*

```diff
@@ -346,18 +346,18 @@
         .stderr(Stdio::inherit());
 
     if !rustflags.flags.is_empty() {
         build_command.env("CARGO_ENCODED_RUSTFLAGS", rustflags.encode()?);
     }
 
     if let BridgeModel::BindingsAbi3(_, _) = bridge_model {
-        let is_pypy = python_interpreter
-            .map(|p| p.interpreter_kind.is_pypy())
+        let is_pypy_or_graalpy = python_interpreter
+            .map(|p| p.interpreter_kind.is_pypy() || p.interpreter_kind.is_graalpy())
             .unwrap_or(false);
-        if !is_pypy && !target.is_windows() {
+        if !is_pypy_or_graalpy && !target.is_windows() {
             let pyo3_ver = pyo3_version(&context.cargo_metadata)
                 .context("Failed to get pyo3 version from cargo metadata")?;
             if pyo3_ver < PYO3_ABI3_NO_PYTHON_VERSION {
                 // This will make old pyo3's build script only set some predefined linker
                 // arguments without trying to read any python configuration
                 build_command.env("PYO3_NO_PYTHON", "1");
             }
@@ -385,15 +385,16 @@
             }
 
             // rust-cpython, and legacy pyo3 versions
             build_command.env("PYTHON_SYS_EXECUTABLE", &interpreter.executable);
         } else if (bridge_model.is_bindings("pyo3")
             || bridge_model.is_bindings("pyo3-ffi")
             || (matches!(bridge_model, BridgeModel::BindingsAbi3(_, _))
-                && interpreter.interpreter_kind.is_pypy()))
+                && (interpreter.interpreter_kind.is_pypy()
+                    || interpreter.interpreter_kind.is_graalpy())))
             && env::var_os("PYO3_CONFIG_FILE").is_none()
         {
             let pyo3_config = interpreter.pyo3_config_file();
             let maturin_target_dir = context.target_dir.join("maturin");
             let config_file = maturin_target_dir.join(format!(
                 "pyo3-config-{}-{}.{}.txt",
                 target_triple, interpreter.major, interpreter.minor
```

### Comparing `maturin-1.0.1/src/cross_compile.rs` & `maturin-1.1.0/src/cross_compile.rs`

 * *Files identical despite different names*

### Comparing `maturin-1.0.1/src/develop.rs` & `maturin-1.1.0/src/develop.rs`

 * *Files 21% similar despite different names*

```diff
@@ -6,27 +6,65 @@
 use crate::Target;
 use anyhow::{anyhow, bail, Context, Result};
 use pep508_rs::{MarkerExpression, MarkerOperator, MarkerTree, MarkerValue};
 use std::path::Path;
 use std::process::Command;
 use tempfile::TempDir;
 
+/// Install the crate as module in the current virtualenv
+#[derive(Debug, clap::Parser)]
+pub struct DevelopOptions {
+    /// Which kind of bindings to use
+    #[arg(
+        short = 'b',
+        long = "bindings",
+        alias = "binding-crate",
+        value_parser = ["pyo3", "pyo3-ffi", "rust-cpython", "cffi", "uniffi", "bin"]
+    )]
+    pub bindings: Option<String>,
+    /// Pass --release to cargo
+    #[arg(short = 'r', long)]
+    pub release: bool,
+    /// Strip the library for minimum file size
+    #[arg(long)]
+    pub strip: bool,
+    /// Install extra requires aka. optional dependencies
+    ///
+    /// Use as `--extras=extra1,extra2`
+    #[arg(
+        short = 'E',
+        long,
+        value_delimiter = ',',
+        action = clap::ArgAction::Append
+    )]
+    pub extras: Vec<String>,
+    /// Skip installation, only build the extension module inplace
+    ///
+    /// Only works with mixed Rust/Python project layout
+    #[arg(long)]
+    pub skip_install: bool,
+    /// `cargo rustc` options
+    #[command(flatten)]
+    pub cargo_options: CargoOptions,
+}
+
 /// Installs a crate by compiling it and copying the shared library to site-packages.
 /// Also adds the dist-info directory to make sure pip and other tools detect the library
 ///
 /// Works only in a virtualenv.
 #[allow(clippy::too_many_arguments)]
-pub fn develop(
-    bindings: Option<String>,
-    cargo_options: CargoOptions,
-    venv_dir: &Path,
-    release: bool,
-    strip: bool,
-    extras: Vec<String>,
-) -> Result<()> {
+pub fn develop(develop_options: DevelopOptions, venv_dir: &Path) -> Result<()> {
+    let DevelopOptions {
+        bindings,
+        release,
+        strip,
+        extras,
+        skip_install,
+        cargo_options,
+    } = develop_options;
     let mut target_triple = cargo_options.target.as_ref().map(|x| x.to_string());
     let target = Target::from_target_triple(cargo_options.target)?;
     let python = target.get_venv_python(venv_dir);
 
     // check python platform and architecture
     if !target.user_specified {
         match Command::new(&python)
@@ -113,46 +151,48 @@
             .context("Failed to run pip install")?;
         if !status.success() {
             bail!(r#"pip install finished with "{}""#, status)
         }
     }
 
     let wheels = build_context.build_wheels()?;
-    for (filename, _supported_version) in wheels.iter() {
-        let command = [
-            "-m",
-            "pip",
-            "--disable-pip-version-check",
-            "install",
-            "--no-deps",
-            "--force-reinstall",
-        ];
-        let output = Command::new(&python)
-            .args(command)
-            .arg(dunce::simplified(filename))
-            .output()
-            .context(format!("pip install failed with {python:?}"))?;
-        if !output.status.success() {
-            bail!(
+    if !skip_install {
+        for (filename, _supported_version) in wheels.iter() {
+            let command = [
+                "-m",
+                "pip",
+                "--disable-pip-version-check",
+                "install",
+                "--no-deps",
+                "--force-reinstall",
+            ];
+            let output = Command::new(&python)
+                .args(command)
+                .arg(dunce::simplified(filename))
+                .output()
+                .context(format!("pip install failed with {python:?}"))?;
+            if !output.status.success() {
+                bail!(
                 "pip install in {} failed running {:?}: {}\n--- Stdout:\n{}\n--- Stderr:\n{}\n---\n",
                 venv_dir.display(),
                 &command,
                 output.status,
                 String::from_utf8_lossy(&output.stdout).trim(),
                 String::from_utf8_lossy(&output.stderr).trim(),
             );
-        }
-        if !output.stderr.is_empty() {
+            }
+            if !output.stderr.is_empty() {
+                eprintln!(
+                    "⚠️ Warning: pip raised a warning running {:?}:\n{}",
+                    &command,
+                    String::from_utf8_lossy(&output.stderr).trim(),
+                );
+            }
             eprintln!(
-                "⚠️ Warning: pip raised a warning running {:?}:\n{}",
-                &command,
-                String::from_utf8_lossy(&output.stderr).trim(),
+                "🛠 Installed {}-{}",
+                build_context.metadata21.name, build_context.metadata21.version
             );
         }
-        eprintln!(
-            "🛠 Installed {}-{}",
-            build_context.metadata21.name, build_context.metadata21.version
-        );
     }
 
     Ok(())
 }
```

### Comparing `maturin-1.0.1/src/lib.rs` & `maturin-1.1.0/src/lib.rs`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 #![deny(missing_docs)]
 
 pub use crate::build_context::{BridgeModel, BuildContext, BuiltWheelMetadata};
 pub use crate::build_options::{BuildOptions, CargoOptions};
 pub use crate::cargo_toml::CargoToml;
 pub use crate::compile::{compile, BuildArtifact};
-pub use crate::develop::develop;
+pub use crate::develop::{develop, DevelopOptions};
 pub use crate::metadata::{Metadata21, WheelMetadata};
 pub use crate::module_writer::{
     write_dist_info, ModuleWriter, PathWriter, SDistWriter, WheelWriter,
 };
 #[cfg(feature = "scaffolding")]
 pub use crate::new_project::{init_project, new_project, GenerateProjectOptions};
 pub use crate::pyproject_toml::PyProjectToml;
```

### Comparing `maturin-1.0.1/src/main.rs` & `maturin-1.1.0/src/main.rs`

 * *Files 4% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 use cargo_zigbuild::Zig;
 #[cfg(feature = "cli-completion")]
 use clap::CommandFactory;
 use clap::{Parser, Subcommand};
 #[cfg(feature = "scaffolding")]
 use maturin::{ci::GenerateCI, init_project, new_project, GenerateProjectOptions};
 use maturin::{
-    develop, write_dist_info, BridgeModel, BuildOptions, CargoOptions, PathWriter, PlatformTag,
-    PythonInterpreter, Target,
+    develop, write_dist_info, BridgeModel, BuildOptions, CargoOptions, DevelopOptions, PathWriter,
+    PlatformTag, PythonInterpreter, Target,
 };
 #[cfg(feature = "upload")]
 use maturin::{upload_ui, PublishOpt};
 use std::env;
 use std::path::PathBuf;
 use tracing::debug;
 
@@ -69,44 +69,15 @@
     /// Search and list the available python installations
     ListPython {
         #[arg(long)]
         target: Option<String>,
     },
     #[command(name = "develop", alias = "dev")]
     /// Install the crate as module in the current virtualenv
-    ///
-    /// Note that this command doesn't create entrypoints
-    Develop {
-        /// Which kind of bindings to use
-        #[arg(
-            short = 'b',
-            long = "bindings",
-            alias = "binding-crate",
-            value_parser = ["pyo3", "pyo3-ffi", "rust-cpython", "cffi", "uniffi", "bin"]
-        )]
-        bindings: Option<String>,
-        /// Pass --release to cargo
-        #[arg(short = 'r', long)]
-        release: bool,
-        /// Strip the library for minimum file size
-        #[arg(long)]
-        strip: bool,
-        /// Install extra requires aka. optional dependencies
-        ///
-        /// Use as `--extras=extra1,extra2`
-        #[arg(
-            short = 'E',
-            long,
-            value_delimiter = ',',
-            action = clap::ArgAction::Append
-        )]
-        extras: Vec<String>,
-        #[command(flatten)]
-        cargo_options: CargoOptions,
-    },
+    Develop(DevelopOptions),
     /// Build only a source distribution (sdist) without compiling.
     ///
     /// Building a source distribution requires a pyproject.toml with a `[build-system]` table.
     ///
     /// This command is a workaround for [pypa/pip#6041](https://github.com/pypa/pip/issues/6041)
     #[command(name = "sdist")]
     SDist {
@@ -400,24 +371,18 @@
                 PythonInterpreter::find_all(&target, &BridgeModel::Cffi, None)?
             };
             eprintln!("🐍 {} python interpreter found:", found.len());
             for interpreter in found {
                 eprintln!(" - {interpreter}");
             }
         }
-        Opt::Develop {
-            bindings,
-            release,
-            strip,
-            extras,
-            cargo_options,
-        } => {
-            let target = Target::from_target_triple(cargo_options.target.clone())?;
+        Opt::Develop(develop_options) => {
+            let target = Target::from_target_triple(develop_options.cargo_options.target.clone())?;
             let venv_dir = detect_venv(&target)?;
-            develop(bindings, cargo_options, &venv_dir, release, strip, extras)?;
+            develop(develop_options, &venv_dir)?;
         }
         Opt::SDist { manifest_path, out } => {
             let build_options = BuildOptions {
                 out,
                 cargo: CargoOptions {
                     manifest_path,
                     ..Default::default()
```

### Comparing `maturin-1.0.1/src/metadata.rs` & `maturin-1.1.0/src/metadata.rs`

 * *Files identical despite different names*

### Comparing `maturin-1.0.1/src/module_writer.rs` & `maturin-1.1.0/src/module_writer.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1158,17 +1158,16 @@
                     .expect("No files found for pattern")
                     .filter_map(Result::ok)
                 {
                     let target = source.strip_prefix(pyproject_dir)?.to_path_buf();
                     if source.is_dir() {
                         writer.add_directory(target)?;
                     } else {
-                        let permissions = source.metadata()?.permissions();
                         #[cfg(unix)]
-                        let mode = permissions.mode();
+                        let mode = source.metadata()?.permissions().mode();
                         #[cfg(not(unix))]
                         let mode = 0o644;
                         writer.add_file_with_permissions(target, source, mode)?;
                     }
                 }
             }
         }
@@ -1250,17 +1249,16 @@
             debug!("Adding data from {}", subdir.path().display());
             (|| {
                 for file in WalkBuilder::new(subdir.path())
                     .standard_filters(false)
                     .build()
                 {
                     let file = file?;
-                    let permissions = file.metadata()?.permissions();
                     #[cfg(unix)]
-                    let mode = permissions.mode();
+                    let mode = file.metadata()?.permissions().mode();
                     #[cfg(not(unix))]
                     let mode = 0o644;
                     let relative = file.path().strip_prefix(data.parent().unwrap()).unwrap();
 
                     if file.path_is_symlink() {
                         // Copy the actual file contents, not the link, so that you can create a
                         // data directory by joining different data sources
```

### Comparing `maturin-1.0.1/src/new_project.rs` & `maturin-1.1.0/src/new_project.rs`

 * *Files identical despite different names*

### Comparing `maturin-1.0.1/src/project_layout.rs` & `maturin-1.1.0/src/project_layout.rs`

 * *Files identical despite different names*

### Comparing `maturin-1.0.1/src/pyproject_toml.rs` & `maturin-1.1.0/src/pyproject_toml.rs`

 * *Files identical despite different names*

### Comparing `maturin-1.0.1/src/python_interpreter/config.rs` & `maturin-1.1.0/src/python_interpreter/config.rs`

 * *Files 3% similar despite different names*

```diff
@@ -5,37 +5,34 @@
 use fs_err as fs;
 use serde::Deserialize;
 use std::fmt::Write as _;
 use std::io::{BufRead, BufReader};
 use std::path::Path;
 
 const PYPY_ABI_TAG: &str = "pp73";
+const GRAALPY_ABI_TAG: &str = "graalpy230_310_native";
 
 /// Some of the sysconfigdata of Python interpreter we care about
 #[derive(Debug, Clone, Deserialize, Eq, PartialEq)]
 pub struct InterpreterConfig {
     /// Python's major version
     pub major: usize,
     /// Python's minor version
     pub minor: usize,
-    /// cpython or pypy
+    /// cpython, pypy, or graalpy
     #[serde(rename = "interpreter")]
     pub interpreter_kind: InterpreterKind,
     /// For linux and mac, this contains the value of the abiflags, e.g. "m"
     /// for python3.7m or "dm" for python3.6dm. Since python3.8, the value is
     /// empty. On windows, the value was always None.
     ///
     /// See PEP 261 and PEP 393 for details
     pub abiflags: String,
     /// Suffix to use for extension modules as given by sysconfig.
     pub ext_suffix: String,
-    /// Part of sysconfig's SOABI specifying {major}{minor}{abiflags}
-    ///
-    /// Note that this always `None` on windows
-    pub abi_tag: Option<String>,
     /// Pointer width
     pub pointer_width: Option<usize>,
 }
 
 impl InterpreterConfig {
     /// Lookup a wellknown sysconfig for a given Python interpreter
     pub fn lookup_one(
@@ -64,82 +61,74 @@
             CPython => {
                 if python_version >= (3, 11) {
                     target.target_env().to_string()
                 } else {
                     target.target_env().to_string().replace("musl", "gnu")
                 }
             }
-            PyPy => "gnu".to_string(),
+            PyPy | GraalPy => "gnu".to_string(),
         };
         match (target.target_os(), python_impl) {
             (Os::Linux, CPython) => {
                 let abiflags = if python_version < (3, 8) {
                     "m".to_string()
                 } else {
                     "".to_string()
                 };
-                let abi_tag = format!("{}{}{}", major, minor, abiflags);
+                let ldversion = format!("{}{}{}", major, minor, abiflags);
                 let ext_suffix = format!(
                     ".cpython-{}-{}-linux-{}.so",
-                    abi_tag, python_arch, target_env
+                    ldversion, python_arch, target_env
                 );
                 Some(Self {
                     major,
                     minor,
                     interpreter_kind: CPython,
                     abiflags,
                     ext_suffix,
-                    abi_tag: Some(abi_tag),
                     pointer_width: Some(target.pointer_width()),
                 })
             }
             (Os::Linux, PyPy) => {
-                let abi_tag = PYPY_ABI_TAG.to_string();
-                let ext_suffix = format!(
-                    ".pypy{}{}-{}-{}-linux-{}.so",
-                    major, minor, abi_tag, python_arch, target_env
-                );
+                let abi_tag = format!("pypy{}{}-{}", major, minor, PYPY_ABI_TAG);
+                let ext_suffix = format!(".{}-{}-linux-{}.so", abi_tag, python_arch, target_env);
                 Some(Self {
                     major,
                     minor,
                     interpreter_kind: PyPy,
                     abiflags: String::new(),
                     ext_suffix,
-                    abi_tag: Some(abi_tag),
                     pointer_width: Some(target.pointer_width()),
                 })
             }
             (Os::Macos, CPython) => {
                 let abiflags = if python_version < (3, 8) {
                     "m".to_string()
                 } else {
                     "".to_string()
                 };
-                let abi_tag = format!("{}{}{}", major, minor, abiflags);
-                let ext_suffix = format!(".cpython-{}-darwin.so", abi_tag);
+                let ldversion = format!("{}{}{}", major, minor, abiflags);
+                let ext_suffix = format!(".cpython-{}-darwin.so", ldversion);
                 Some(Self {
                     major,
                     minor,
                     interpreter_kind: CPython,
                     abiflags,
                     ext_suffix,
-                    abi_tag: Some(abi_tag),
                     pointer_width: Some(target.pointer_width()),
                 })
             }
             (Os::Macos, PyPy) => {
-                let abi_tag = PYPY_ABI_TAG.to_string();
-                let ext_suffix = format!(".pypy{}{}-{}-darwin.so", major, minor, abi_tag);
+                let ext_suffix = format!(".pypy{}{}-{}-darwin.so", major, minor, PYPY_ABI_TAG);
                 Some(Self {
                     major,
                     minor,
                     interpreter_kind: PyPy,
                     abiflags: String::new(),
                     ext_suffix,
-                    abi_tag: Some(abi_tag),
                     pointer_width: Some(target.pointer_width()),
                 })
             }
             (Os::Windows, CPython) => {
                 let ext_suffix = if python_version < (3, 8) {
                     ".pyd".to_string()
                 } else {
@@ -153,88 +142,79 @@
                 };
                 Some(Self {
                     major,
                     minor,
                     interpreter_kind: CPython,
                     abiflags: String::new(),
                     ext_suffix,
-                    abi_tag: None,
                     pointer_width: Some(target.pointer_width()),
                 })
             }
             (Os::Windows, PyPy) => {
                 if target.target_arch() != Arch::X86_64 {
                     // PyPy on Windows only supports x86_64
                     return None;
                 }
-                let abi_tag = PYPY_ABI_TAG.to_string();
-                let ext_suffix = format!(".pypy{}{}-{}-win_amd64.pyd", major, minor, abi_tag);
+                let ext_suffix = format!(".pypy{}{}-{}-win_amd64.pyd", major, minor, PYPY_ABI_TAG);
                 Some(Self {
                     major,
                     minor,
                     interpreter_kind: PyPy,
                     abiflags: String::new(),
                     ext_suffix,
-                    abi_tag: Some(abi_tag),
                     pointer_width: Some(target.pointer_width()),
                 })
             }
             (Os::FreeBsd, CPython) => {
                 let (abiflags, ext_suffix) = if python_version < (3, 8) {
                     ("m".to_string(), ".so".to_string())
                 } else {
                     ("".to_string(), format!(".cpython-{}{}.so", major, minor))
                 };
-                let abi_tag = format!("{}{}{}", major, minor, abiflags);
                 Some(Self {
                     major,
                     minor,
                     interpreter_kind: CPython,
                     abiflags,
                     ext_suffix,
-                    abi_tag: Some(abi_tag),
                     pointer_width: Some(target.pointer_width()),
                 })
             }
             (Os::NetBsd, CPython) => {
-                let abi_tag = format!("{}{}", major, minor);
                 let ext_suffix = ".so".to_string();
                 Some(Self {
                     major,
                     minor,
                     interpreter_kind: CPython,
                     abiflags: String::new(),
                     ext_suffix,
-                    abi_tag: Some(abi_tag),
                     pointer_width: Some(target.pointer_width()),
                 })
             }
             (Os::OpenBsd, CPython) => {
-                let abi_tag = format!("{}{}", major, minor);
-                let ext_suffix = format!(".cpython-{}.so", abi_tag);
+                let ldversion = format!("{}{}", major, minor);
+                let ext_suffix = format!(".cpython-{}.so", ldversion);
                 Some(Self {
                     major,
                     minor,
                     interpreter_kind: CPython,
                     abiflags: String::new(),
                     ext_suffix,
-                    abi_tag: Some(abi_tag),
                     pointer_width: Some(target.pointer_width()),
                 })
             }
             (Os::Emscripten, CPython) => {
-                let abi_tag = format!("{}{}", major, minor);
-                let ext_suffix = format!(".cpython-{}-{}-emscripten.so", abi_tag, python_arch);
+                let ldversion = format!("{}{}", major, minor);
+                let ext_suffix = format!(".cpython-{}-{}-emscripten.so", ldversion, python_arch);
                 Some(Self {
                     major,
                     minor,
                     interpreter_kind: CPython,
                     abiflags: String::new(),
                     ext_suffix,
-                    abi_tag: Some(abi_tag),
                     pointer_width: Some(target.pointer_width()),
                 })
             }
             (_, _) => None,
         }
     }
 
@@ -312,14 +292,15 @@
                 if (major, minor) >= (3, 8) {
                     abi_tag.unwrap_or_else(|| format!("{major}{minor}"))
                 } else {
                     abi_tag.unwrap_or_else(|| format!("{major}{minor}m"))
                 }
             }
             InterpreterKind::PyPy => abi_tag.unwrap_or_else(|| PYPY_ABI_TAG.to_string()),
+            InterpreterKind::GraalPy => abi_tag.unwrap_or_else(|| GRAALPY_ABI_TAG.to_string()),
         };
         let file_ext = if target.is_windows() { "pyd" } else { "so" };
         let ext_suffix = if target.is_linux() || target.is_macos() {
             // See https://github.com/pypa/auditwheel/issues/349
             let target_env = if (major, minor) >= (3, 11) {
                 target.target_env().to_string()
             } else {
@@ -346,14 +327,24 @@
                         abi_tag,
                         target.get_python_arch(),
                         target.get_python_os(),
                         target_env,
                         file_ext,
                     )
                 }),
+                InterpreterKind::GraalPy => ext_suffix.unwrap_or_else(|| {
+                    // e.g. .graalpy230-310-native-x86_64-linux.so
+                    format!(
+                        ".{}-{}-{}.{}",
+                        abi_tag.replace('_', "-"),
+                        target.get_python_arch(),
+                        target.get_python_os(),
+                        file_ext,
+                    )
+                }),
             }
         } else if target.is_emscripten() && matches!(interpreter_kind, InterpreterKind::CPython) {
             ext_suffix.unwrap_or_else(|| {
                 format!(
                     ".cpython-{}-{}-{}.{}",
                     abi_tag,
                     target.get_python_arch(),
@@ -366,15 +357,14 @@
         };
         Ok(Self {
             major,
             minor,
             interpreter_kind,
             abiflags: abiflags.unwrap_or_default(),
             ext_suffix,
-            abi_tag: Some(abi_tag),
             pointer_width,
         })
     }
 
     /// Generate pyo3 config file content
     pub fn pyo3_config_file(&self) -> String {
         let mut content = format!(
@@ -466,15 +456,14 @@
         let sysconfig = InterpreterConfig::lookup_one(
             &Target::from_target_triple(Some("x86_64-unknown-linux-gnu".to_string())).unwrap(),
             InterpreterKind::PyPy,
             (3, 9),
         )
         .unwrap();
         assert_eq!(sysconfig.abiflags, "");
-        assert_eq!(sysconfig.abi_tag.as_deref(), Some("pp73"));
         assert_eq!(sysconfig.ext_suffix, ".pypy39-pp73-x86_64-linux-gnu.so");
 
         let sysconfig = InterpreterConfig::lookup_one(
             &Target::from_target_triple(Some("i686-unknown-linux-gnu".to_string())).unwrap(),
             InterpreterKind::PyPy,
             (3, 9),
         )
@@ -544,26 +533,24 @@
         let sysconfig = InterpreterConfig::lookup_one(
             &Target::from_target_triple(Some("x86_64-apple-darwin".to_string())).unwrap(),
             InterpreterKind::CPython,
             (3, 7),
         )
         .unwrap();
         assert_eq!(sysconfig.abiflags, "m");
-        assert_eq!(sysconfig.abi_tag.as_deref(), Some("37m"));
         assert_eq!(sysconfig.ext_suffix, ".cpython-37m-darwin.so");
 
         // PyPy
         let sysconfig = InterpreterConfig::lookup_one(
             &Target::from_target_triple(Some("x86_64-apple-darwin".to_string())).unwrap(),
             InterpreterKind::PyPy,
             (3, 9),
         )
         .unwrap();
         assert_eq!(sysconfig.abiflags, "");
-        assert_eq!(sysconfig.abi_tag.as_deref(), Some("pp73"));
         assert_eq!(sysconfig.ext_suffix, ".pypy39-pp73-darwin.so");
 
         let sysconfig = InterpreterConfig::lookup_one(
             &Target::from_target_triple(Some("aarch64-apple-darwin".to_string())).unwrap(),
             InterpreterKind::PyPy,
             (3, 9),
         )
@@ -614,25 +601,23 @@
         let sysconfig = InterpreterConfig::lookup_one(
             &Target::from_target_triple(Some("x86_64-unknown-freebsd".to_string())).unwrap(),
             InterpreterKind::CPython,
             (3, 7),
         )
         .unwrap();
         assert_eq!(sysconfig.abiflags, "m");
-        assert_eq!(sysconfig.abi_tag.as_deref(), Some("37m"));
         assert_eq!(sysconfig.ext_suffix, ".so");
 
         let sysconfig = InterpreterConfig::lookup_one(
             &Target::from_target_triple(Some("x86_64-unknown-freebsd".to_string())).unwrap(),
             InterpreterKind::CPython,
             (3, 10),
         )
         .unwrap();
         assert_eq!(sysconfig.abiflags, "");
-        assert_eq!(sysconfig.abi_tag.as_deref(), Some("310"));
         assert_eq!(sysconfig.ext_suffix, ".cpython-310.so");
 
         let sysconfig = InterpreterConfig::lookup_one(
             &Target::from_target_triple(Some("i686-unknown-freebsd".to_string())).unwrap(),
             InterpreterKind::CPython,
             (3, 10),
         )
@@ -662,15 +647,14 @@
         let sysconfig = InterpreterConfig::lookup_one(
             &Target::from_target_triple(Some("x86_64-unknown-netbsd".to_string())).unwrap(),
             InterpreterKind::CPython,
             (3, 7),
         )
         .unwrap();
         assert_eq!(sysconfig.abiflags, "");
-        assert_eq!(sysconfig.abi_tag.as_deref(), Some("37"));
         assert_eq!(sysconfig.ext_suffix, ".so");
 
         let sysconfig = InterpreterConfig::lookup_one(
             &Target::from_target_triple(Some("x86_64-unknown-netbsd".to_string())).unwrap(),
             InterpreterKind::CPython,
             (3, 10),
         )
@@ -712,15 +696,14 @@
         let sysconfig = InterpreterConfig::lookup_one(
             &Target::from_target_triple(Some("wasm32-unknown-emscripten".to_string())).unwrap(),
             InterpreterKind::CPython,
             (3, 10),
         )
         .unwrap();
         assert_eq!(sysconfig.abiflags, "");
-        assert_eq!(sysconfig.abi_tag.as_deref(), Some("310"));
         assert_eq!(sysconfig.ext_suffix, ".cpython-310-wasm32-emscripten.so");
     }
 
     #[test]
     fn test_pyo3_config_file() {
         let sysconfig = InterpreterConfig::lookup_one(
             &Target::from_target_triple(Some("x86_64-unknown-linux-gnu".to_string())).unwrap(),
```

### Comparing `maturin-1.0.1/src/python_interpreter/get_interpreter_metadata.py` & `maturin-1.1.0/src/python_interpreter/get_interpreter_metadata.py`

 * *Files 17% similar despite different names*

```diff
@@ -26,15 +26,14 @@
     "executable": sys.executable or None,
     "major": sys.version_info.major,
     "minor": sys.version_info.minor,
     "abiflags": sysconfig.get_config_var("ABIFLAGS"),
     "interpreter": platform.python_implementation().lower(),
     "ext_suffix": ext_suffix,
     "soabi": sysconfig.get_config_var("SOABI") or None,
-    "abi_tag": (sysconfig.get_config_var("SOABI") or "-").split("-")[1] or None,
     "platform": sysconfig.get_platform(),
     # This one isn't technically necessary, but still very useful for sanity checks
     "system": platform.system().lower(),
     # This one is for generating a config file for pyo3
     "pointer_width": struct.calcsize("P") * 8,
 }
```

### Comparing `maturin-1.0.1/src/python_interpreter/mod.rs` & `maturin-1.1.0/src/python_interpreter/mod.rs`

 * *Files 4% similar despite different names*

```diff
@@ -273,58 +273,65 @@
         };
         Ok(Some(InterpreterConfig {
             major,
             minor,
             interpreter_kind: InterpreterKind::CPython,
             abiflags: String::new(),
             ext_suffix: String::new(),
-            abi_tag: None,
             pointer_width: Some(pointer_width),
         }))
     } else {
         Ok(None)
     }
 }
 
 #[derive(Debug, Clone, Copy, Eq, PartialEq, Deserialize, clap::ValueEnum)]
 #[serde(rename_all = "lowercase")]
 #[clap(rename_all = "lower")]
 pub enum InterpreterKind {
     CPython,
     PyPy,
+    GraalPy,
 }
 
 impl InterpreterKind {
     /// Is this a CPython interpreter?
     pub fn is_cpython(&self) -> bool {
         matches!(self, InterpreterKind::CPython)
     }
 
     /// Is this a PyPy interpreter?
     pub fn is_pypy(&self) -> bool {
         matches!(self, InterpreterKind::PyPy)
     }
+
+    /// Is this a GraalPy interpreter?
+    pub fn is_graalpy(&self) -> bool {
+        matches!(self, InterpreterKind::GraalPy)
+    }
 }
 
 impl fmt::Display for InterpreterKind {
     fn fmt(&self, f: &mut fmt::Formatter) -> fmt::Result {
         match *self {
             InterpreterKind::CPython => write!(f, "CPython"),
             InterpreterKind::PyPy => write!(f, "PyPy"),
+            InterpreterKind::GraalPy => write!(f, "GraalPy"),
         }
     }
 }
 
 impl FromStr for InterpreterKind {
     type Err = String;
 
     fn from_str(s: &str) -> Result<Self, Self::Err> {
         match s.to_ascii_lowercase().as_str() {
             "cpython" => Ok(InterpreterKind::CPython),
             "pypy" => Ok(InterpreterKind::PyPy),
+            "graalvm" | "graalpy" => Ok(InterpreterKind::GraalPy),
             unknown => Err(format!("Unknown interpreter kind '{unknown}'")),
         }
     }
 }
 
 /// The output format of [GET_INTERPRETER_METADATA]
 #[derive(Deserialize)]
@@ -337,15 +344,14 @@
     interpreter: String,
     ext_suffix: Option<String>,
     // comes from `sysconfig.get_platform()`
     platform: String,
     // comes from `platform.system()`
     system: String,
     soabi: Option<String>,
-    abi_tag: Option<String>,
 }
 
 /// The location and version of an interpreter
 #[derive(Debug, Clone, Eq, PartialEq)]
 pub struct PythonInterpreter {
     /// Python's sysconfig
     /// Python's major version
@@ -403,16 +409,16 @@
         bail!(
             "Only python >= 3.5 is supported, while you're using python {}.{}",
             message.major,
             message.minor
         );
     }
 
-    if message.interpreter == "pypy" {
-        // pypy does not specify abi flags
+    if message.interpreter == "pypy" || message.interpreter == "graalvm" {
+        // pypy and graalpy do not specify abi flags
         Ok("".to_string())
     } else if message.system == "windows" {
         if matches!(message.abiflags.as_deref(), Some("") | None) {
             Ok("".to_string())
         } else {
             bail!("A python 3 interpreter on windows does not define abiflags in its sysconfig ಠ_ಠ")
         }
@@ -434,15 +440,15 @@
     /// Does this interpreter have PEP 384 stable api aka. abi3 support?
     pub fn has_stable_api(&self) -> bool {
         if self.implementation_name.parse::<InterpreterKind>().is_err() {
             false
         } else {
             match self.interpreter_kind {
                 InterpreterKind::CPython => true,
-                InterpreterKind::PyPy => false,
+                InterpreterKind::PyPy | InterpreterKind::GraalPy => false,
             }
         }
     }
 
     /// Returns the supported python environment in the PEP 425 format used for the wheel filename:
     /// {python tag}-{abi tag}-{platform tag}
     ///
@@ -501,25 +507,37 @@
                         )
                     }
                 }
                 InterpreterKind::PyPy => {
                     // pypy uses its version as part of the ABI, e.g.
                     // pypy 3.7 7.3 => numpy-1.20.1-pp37-pypy37_pp73-manylinux2014_x86_64.whl
                     format!(
-                        "pp{major}{minor}-pypy{major}{minor}_{abi_tag}-{platform}",
+                        "pp{major}{minor}-{abi_tag}-{platform}",
                         major = self.major,
                         minor = self.minor,
-                        // TODO: Proper tag handling for pypy
-                        abi_tag = self
-                            .abi_tag
-                            .clone()
-                            .expect("PyPy's syconfig didn't define an `SOABI` ಠ_ಠ"),
+                        abi_tag = calculate_abi_tag(&self.ext_suffix)
+                            .expect("PyPy's syconfig didn't define a valid `EXT_SUFFIX` ಠ_ಠ"),
                         platform = platform,
                     )
                 }
+                InterpreterKind::GraalPy => {
+                    // GraalPy suffers from pypa/packaging#614, where
+                    // packaging misdetects it as a 32-bit implementation,
+                    // so GraalPy adds the correct platform itself, e.g.
+                    // graalpy 3.10 23.1 => numpy-1.23.5-graalpy310-graalpy231_310_native_x86_64_linux-linux_i686.whl
+                    format!(
+                        "graalpy{major}{minor}-{abi_tag}_{arch}_{os}-{os}_i686",
+                        major = self.major,
+                        minor = self.minor,
+                        abi_tag = calculate_abi_tag(&self.ext_suffix)
+                            .expect("GraalPy's syconfig didn't define a valid `EXT_SUFFIX` ಠ_ಠ"),
+                        os = target.get_python_os(),
+                        arch = target.get_python_arch(),
+                    )
+                }
             }
         };
         Ok(tag)
     }
 
     /// Adds the ext_suffix we read from python or know (.pyd/.abi3.so) and adds it to the base name
     ///
@@ -631,14 +649,15 @@
             );
             return Ok(None);
         }
 
         let interpreter = match message.interpreter.as_str() {
             "cpython" => InterpreterKind::CPython,
             "pypy" => InterpreterKind::PyPy,
+            "graalvm" | "graalpy" => InterpreterKind::GraalPy,
             other => {
                 bail!("Unsupported interpreter {}", other);
             }
         };
 
         let abiflags = fun_with_abiflags(&message, target, bridge).context(format_err!(
             "Failed to get information from the python interpreter at {}",
@@ -666,15 +685,14 @@
                 major: message.major,
                 minor: message.minor,
                 interpreter_kind: interpreter,
                 abiflags,
                 ext_suffix: message
                     .ext_suffix
                     .context("syconfig didn't define an `EXT_SUFFIX` ಠ_ಠ")?,
-                abi_tag: message.abi_tag,
                 pointer_width: None,
             },
             executable,
             platform,
             runnable: true,
             implementation_name: message.implementation_name,
             soabi: message.soabi,
@@ -884,15 +902,15 @@
     }
 
     /// Returns the site-packages directory inside a venv e.g.
     /// {venv_base}/lib/python{x}.{y} on unix or {venv_base}/Lib on window
     pub fn get_venv_site_package(&self, venv_base: impl AsRef<Path>, target: &Target) -> PathBuf {
         if target.is_unix() {
             match self.interpreter_kind {
-                InterpreterKind::CPython => {
+                InterpreterKind::CPython | InterpreterKind::GraalPy => {
                     let python_dir = format!("python{}.{}", self.major, self.minor);
                     venv_base
                         .as_ref()
                         .join("lib")
                         .join(python_dir)
                         .join("site-packages")
                 }
@@ -925,14 +943,43 @@
                 self.config.minor,
                 self.config.abiflags,
             )
         }
     }
 }
 
+/// Calculate the ABI tag from EXT_SUFFIX
+fn calculate_abi_tag(ext_suffix: &str) -> Option<String> {
+    let parts = ext_suffix.split('.').collect::<Vec<_>>();
+    if parts.len() < 3 {
+        // CPython3.7 and earlier uses ".pyd" on Windows.
+        return None;
+    }
+    let soabi = parts[1];
+    let mut soabi_split = soabi.split('-');
+    let abi = if soabi.starts_with("cpython") {
+        // non-windows
+        format!("cp{}", soabi_split.nth(1).unwrap())
+    } else if soabi.starts_with("cp") {
+        // windows
+        soabi_split.next().unwrap().to_string()
+    } else if soabi.starts_with("pypy") {
+        soabi_split.take(2).collect::<Vec<_>>().join("-")
+    } else if soabi.starts_with("graalpy") {
+        soabi_split.take(3).collect::<Vec<_>>().join("-")
+    } else if !soabi.is_empty() {
+        // pyston, ironpython, others?
+        soabi_split.nth(1).unwrap().to_string()
+    } else {
+        return None;
+    };
+    let abi_tag = abi.replace(['.', '-', ' '], "_");
+    Some(abi_tag)
+}
+
 #[cfg(test)]
 mod tests {
     use super::*;
 
     #[test]
     fn test_find_interpreter_by_target() {
         let target =
@@ -948,8 +995,32 @@
 
         let pythons = PythonInterpreter::find_by_target(
             &target,
             Some(&VersionSpecifiers::from_str(">=3.10").unwrap()),
         );
         assert_eq!(pythons.len(), 4);
     }
+
+    #[test]
+    fn test_calculate_abi_tag() {
+        let cases = vec![
+            (".cpython-37m-x86_64-linux-gnu.so", Some("cp37m")),
+            (".cpython-310-x86_64-linux-gnu.so", Some("cp310")),
+            (".cpython-310-darwin.so", Some("cp310")),
+            (".cp310-win_amd64.pyd", Some("cp310")),
+            (".cp39-mingw_x86_64.pyd", Some("cp39")),
+            (".cpython-312-wasm32-wasi.so", Some("cp312")),
+            (".cpython-38.so", Some("cp38")),
+            (".pyd", None),
+            (".so", None),
+            (".pypy38-pp73-x86_64-linux-gnu.so", Some("pypy38_pp73")),
+            (
+                ".graalpy-38-native-x86_64-darwin.dylib",
+                Some("graalpy_38_native"),
+            ),
+            (".pyston-23-x86_64-linux-gnu.so", Some("23")),
+        ];
+        for (ext_suffix, expected) in cases {
+            assert_eq!(calculate_abi_tag(ext_suffix).as_deref(), expected);
+        }
+    }
 }
```

### Comparing `maturin-1.0.1/src/source_distribution.rs` & `maturin-1.1.0/src/source_distribution.rs`

 * *Files identical despite different names*

### Comparing `maturin-1.0.1/src/target.rs` & `maturin-1.1.0/src/target.rs`

 * *Files 2% similar despite different names*

```diff
@@ -69,14 +69,15 @@
     X86_64,
     S390X,
     Wasm32,
     Riscv64,
     Mips64el,
     Mipsel,
     Sparc64,
+    LoongArch64,
 }
 
 impl fmt::Display for Arch {
     fn fmt(&self, f: &mut fmt::Formatter) -> fmt::Result {
         match *self {
             Arch::Aarch64 => write!(f, "aarch64"),
             Arch::Armv6L => write!(f, "armv6l"),
@@ -88,14 +89,15 @@
             Arch::X86_64 => write!(f, "x86_64"),
             Arch::S390X => write!(f, "s390x"),
             Arch::Wasm32 => write!(f, "wasm32"),
             Arch::Riscv64 => write!(f, "riscv64"),
             Arch::Mips64el => write!(f, "mips64el"),
             Arch::Mipsel => write!(f, "mipsel"),
             Arch::Sparc64 => write!(f, "sparc64"),
+            Arch::LoongArch64 => write!(f, "loongarch64"),
         }
     }
 }
 
 impl Arch {
     /// Represents the hardware platform.
     ///
@@ -111,14 +113,15 @@
             Arch::X86_64 => "amd64",
             Arch::Riscv64 => "riscv",
             Arch::Mips64el | Arch::Mipsel => "mips",
             // sparc64 is unsupported since FreeBSD 13.0
             Arch::Sparc64 => "sparc64",
             Arch::Wasm32 => "wasm32",
             Arch::S390X => "s390x",
+            Arch::LoongArch64 => "loongarch64",
         }
     }
 }
 
 // Returns the set of supported architectures for each operating system
 fn get_supported_architectures(os: &Os) -> Vec<Arch> {
     match os {
@@ -132,14 +135,15 @@
             Arch::S390X,
             Arch::X86,
             Arch::X86_64,
             Arch::Riscv64,
             Arch::Mips64el,
             Arch::Mipsel,
             Arch::Sparc64,
+            Arch::LoongArch64,
         ],
         Os::Windows => vec![Arch::X86, Arch::X86_64, Arch::Aarch64],
         Os::Macos => vec![Arch::Aarch64, Arch::X86_64],
         Os::FreeBsd | Os::NetBsd => vec![
             Arch::Aarch64,
             Arch::Armv6L,
             Arch::Armv7L,
@@ -239,14 +243,15 @@
             Architecture::Powerpc64le => Arch::Powerpc64Le,
             Architecture::S390x => Arch::S390X,
             Architecture::Wasm32 => Arch::Wasm32,
             Architecture::Riscv64(_) => Arch::Riscv64,
             Architecture::Mips64(Mips64Architecture::Mips64el) => Arch::Mips64el,
             Architecture::Mips32(Mips32Architecture::Mipsel) => Arch::Mipsel,
             Architecture::Sparc64 => Arch::Sparc64,
+            Architecture::LoongArch64 => Arch::LoongArch64,
             unsupported => bail!("The architecture {} is not supported", unsupported),
         };
 
         if !get_supported_architectures(&os).contains(&arch) {
             bail!("{} is not supported on {}", arch, os);
         }
 
@@ -319,14 +324,15 @@
             Arch::S390X => "s390x",
             Arch::Wasm32 => "wasm32",
             Arch::Riscv64 => "riscv64",
             // It's kinda surprising that Python doesn't include the `el` suffix
             Arch::Mips64el => "mips64",
             Arch::Mipsel => "mips",
             Arch::Sparc64 => "sparc64",
+            Arch::LoongArch64 => "loongarch64",
         }
     }
 
     /// Returns the name python uses in `sys.platform` for this os
     pub fn get_python_os(&self) -> &str {
         match self.os {
             Os::Windows => "windows",
@@ -362,29 +368,31 @@
             }
             Arch::Armv6L
             | Arch::Wasm32
             | Arch::Riscv64
             | Arch::Mips64el
             | Arch::Mipsel
             | Arch::Powerpc
-            | Arch::Sparc64 => PlatformTag::Linux,
+            | Arch::Sparc64
+            | Arch::LoongArch64 => PlatformTag::Linux,
         }
     }
 
     /// Returns whether the platform is 64 bit or 32 bit
     pub fn pointer_width(&self) -> usize {
         match self.arch {
             Arch::Aarch64
             | Arch::Powerpc64
             | Arch::Powerpc64Le
             | Arch::X86_64
             | Arch::S390X
             | Arch::Riscv64
             | Arch::Mips64el
-            | Arch::Sparc64 => 64,
+            | Arch::Sparc64
+            | Arch::LoongArch64 => 64,
             Arch::Armv6L
             | Arch::Armv7L
             | Arch::X86
             | Arch::Wasm32
             | Arch::Mipsel
             | Arch::Powerpc => 32,
         }
```

### Comparing `maturin-1.0.1/src/templates/.gitignore.j2` & `maturin-1.1.0/src/templates/.gitignore.j2`

 * *Files identical despite different names*

### Comparing `maturin-1.0.1/src/templates/Cargo.toml.j2` & `maturin-1.1.0/src/templates/Cargo.toml.j2`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 [lib]
 name = "{{ crate_name }}"
 crate-type = ["cdylib"]
 {%- endif %}
 
 [dependencies]
 {% if bindings == "pyo3" -%}
-pyo3 = "0.18.3"
+pyo3 = "0.19.0"
 {% elif bindings == "rust-cpython" -%}
 cpython = "0.7.1"
 {% elif bindings == "uniffi" -%}
 uniffi = "0.23.0"
 
 [build-dependencies]
 uniffi = { version = "0.23.0", features = ["build"] }
```

### Comparing `maturin-1.0.1/src/templates/lib.rs.j2` & `maturin-1.1.0/src/templates/lib.rs.j2`

 * *Files identical despite different names*

### Comparing `maturin-1.0.1/src/templates/pyproject.toml.j2` & `maturin-1.1.0/src/templates/pyproject.toml.j2`

 * *Files identical despite different names*

### Comparing `maturin-1.0.1/src/upload.rs` & `maturin-1.1.0/src/upload.rs`

 * *Files identical despite different names*

### Comparing `maturin-1.0.1/test-dockerfile.sh` & `maturin-1.1.0/test-dockerfile.sh`

 * *Files identical despite different names*

### Comparing `maturin-1.0.1/PKG-INFO` & `maturin-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maturin
-Version: 1.0.1
+Version: 1.1.0
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: tomli >=1.1.0 ; python_version < '3.11'
 Requires-Dist: ziglang ~=0.10.0 ; extra == 'zig'
 Requires-Dist: patchelf ; extra == 'patchelf'
@@ -33,15 +33,15 @@
 [![PyPI](https://img.shields.io/pypi/v/maturin.svg?logo=python&style=flat-square)](https://pypi.org/project/maturin)
 [![Maturin User Guide](https://img.shields.io/badge/user-guide-brightgreen?logo=readthedocs&style=flat-square)](https://maturin.rs)
 [![Chat on Gitter](https://img.shields.io/gitter/room/nwjs/nw.js.svg?logo=gitter&style=flat-square)](https://gitter.im/PyO3/Lobby)
 
 Build and publish crates with pyo3, rust-cpython, cffi and uniffi bindings as well as rust binaries as python packages.
 
 This project is meant as a zero configuration replacement for [setuptools-rust](https://github.com/PyO3/setuptools-rust) and [milksnake](https://github.com/getsentry/milksnake).
-It supports building wheels for python 3.5+ on windows, linux, mac and freebsd, can upload them to [pypi](https://pypi.org/) and has basic pypy support.
+It supports building wheels for python 3.5+ on windows, linux, mac and freebsd, can upload them to [pypi](https://pypi.org/) and has basic pypy and graalpy support.
 
 Check out the [User Guide](https://maturin.rs/)!
 
 ## Usage
 
 You can either download binaries from the [latest release](https://github.com/PyO3/maturin/releases/latest) or install it with pip:
 
@@ -295,14 +295,15 @@
 
 ## Examples
 
 * [ballista-python](https://github.com/apache/arrow-ballista-python) - A Python library that binds to Apache Arrow distributed query engine Ballista
 * [connector-x](https://github.com/sfu-db/connector-x/tree/main/connectorx-python) - ConnectorX enables you to load data from databases into Python in the fastest and most memory efficient way
 * [datafusion-python](https://github.com/apache/arrow-datafusion-python) - a Python library that binds to Apache Arrow in-memory query engine DataFusion
 * [deltalake-python](https://github.com/delta-io/delta-rs/tree/main/python) - Native Delta Lake Python binding based on delta-rs with Pandas integration
+* [opendal](https://github.com/apache/incubator-opendal/tree/main/bindings/python) - OpenDAL Python Binding to access data freely
 * [orjson](https://github.com/ijl/orjson) - A fast, correct JSON library for Python
 * [polars](https://github.com/pola-rs/polars/tree/master/py-polars) - Fast multi-threaded DataFrame library in Rust | Python | Node.js
 * [pydantic-core](https://github.com/pydantic/pydantic-core) - Core validation logic for pydantic written in Rust
 * [pyrus-cramjam](https://github.com/milesgranger/pyrus-cramjam) - Thin Python wrapper to de/compression algorithms in Rust
 * [pyxel](https://github.com/kitao/pyxel) - A retro game engine for Python
 * [roapi](https://github.com/roapi/roapi) - ROAPI automatically spins up read-only APIs for static datasets without requiring you to write a single line of code
 * [robyn](https://github.com/sansyrox/robyn) -  A fast and extensible async python web server with a Rust runtime
```

