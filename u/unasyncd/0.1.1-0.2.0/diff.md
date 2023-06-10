# Comparing `tmp/unasyncd-0.1.1.tar.gz` & `tmp/unasyncd-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unasyncd-0.1.1.tar", max compression
+gzip compressed data, was "unasyncd-0.2.0.tar", max compression
```

## Comparing `unasyncd-0.1.1.tar` & `unasyncd-0.2.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1073 2023-06-08 18:10:22.032836 unasyncd-0.1.1/LICENSE
--rw-r--r--   0        0        0    14752 2023-06-08 18:10:22.032836 unasyncd-0.1.1/README.md
--rw-r--r--   0        0        0      814 2023-06-08 18:10:22.032836 unasyncd-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-08 18:10:22.032836 unasyncd-0.1.1/unasyncd/__init__.py
--rw-r--r--   0        0        0     3693 2023-06-08 18:10:22.032836 unasyncd-0.1.1/unasyncd/cli.py
--rw-r--r--   0        0        0     2475 2023-06-08 18:10:22.032836 unasyncd-0.1.1/unasyncd/config.py
--rw-r--r--   0        0        0    10308 2023-06-08 18:10:22.032836 unasyncd-0.1.1/unasyncd/main.py
--rw-r--r--   0        0        0    34690 2023-06-08 18:10:22.032836 unasyncd-0.1.1/unasyncd/transformers.py
--rw-r--r--   0        0        0    15347 1970-01-01 00:00:00.000000 unasyncd-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-06-10 09:21:40.873681 unasyncd-0.2.0/LICENSE
+-rw-r--r--   0        0        0    16076 2023-06-10 09:21:40.873681 unasyncd-0.2.0/README.md
+-rw-r--r--   0        0        0      908 2023-06-10 09:21:40.873681 unasyncd-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-10 09:21:40.873681 unasyncd-0.2.0/unasyncd/__init__.py
+-rw-r--r--   0        0        0     3836 2023-06-10 09:21:40.873681 unasyncd-0.2.0/unasyncd/cli.py
+-rw-r--r--   0        0        0     2482 2023-06-10 09:21:40.873681 unasyncd-0.2.0/unasyncd/config.py
+-rw-r--r--   0        0        0    10306 2023-06-10 09:21:40.873681 unasyncd-0.2.0/unasyncd/main.py
+-rw-r--r--   0        0        0    37782 2023-06-10 09:21:40.873681 unasyncd-0.2.0/unasyncd/transformers.py
+-rw-r--r--   0        0        0    16786 1970-01-01 00:00:00.000000 unasyncd-0.2.0/PKG-INFO
```

### Comparing `unasyncd-0.1.1/LICENSE` & `unasyncd-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `unasyncd-0.1.1/README.md` & `unasyncd-0.2.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -4,50 +4,56 @@
 
 ## Why?
 
 Unasyncd is largely inspired by [unasync](https://github.com/python-trio/unasync), and
 a detailed discussion about this approach can be found
 [here](https://github.com/urllib3/urllib3/issues/1323).
 
-The goal is essentially to reduce to burden of having to maintain both a synchronous and
-an asynchronous version of otherwise functionally identical code. The idea behind
-simply "taking out the async" is that often, synchronous and asynchronous code only
-differ very slightly: A few `await`s, `async def`s and `async with`s, and a couple of
-different method names. The unasync approach makes use of this and provides a way to
-use the asynchronous version as a source of truth from wich the synchronous version can
-be generated.
+Its purpose is to reduce to burden of having to maintain both a synchronous and an
+asynchronous version of otherwise functionally identical code. The idea behind simply
+"taking out the async" is that often, synchronous and asynchronous code only differ
+slightly: A few `await`s, `async def`s, `async with`s, and a couple of different method
+names. The unasync approach makes use of this by treating the asynchronous version as a
+source of truth from wich the synchronous version is then generated.
 
 ## Why unasyncd?
 
-The original [unasync](https://github.com/python-trio/unasync) takes a very simplistic
-approach and works by replacing tokens. This works well enough for most basic use cases,
-but can be somewhat restrictive in the way the code can be written. More complex cases
-such as exclusion of functions / classes or transformations such as `AsyncExitStack` to
-`ExitStack` are not possible, which leads to the introduction of shims, introducing
-additional complexity.
+The original [unasync](https://github.com/python-trio/unasync) works by simply replacing
+certain token, which is enough for most basic use cases, but can be somewhat restrictive
+in the way the code can be written. More complex cases such as exclusion of functions /
+classes or transformations (such as `AsyncExitStack` to `ExitStack` wich have not only
+different names but also different method names that then need to be replaced only
+within a certain scope) are not possible. This can lead to the introduction of shims,
+introducing additional complexity.
+
+Unasyncd's goal is to impose as little restrictions as possible to the way the
+asynchronous code can be written, as long as it maps to a functionally equivalent
+synchronous version.
 
-Unasyncd leverages [libcst](https://libcst.readthedocs.io/), enabling a more granular
-control and more complex transformations.
+To achieve this, unasyncd leverages [libcst](https://libcst.readthedocs.io/), enabling a
+more granular control and complex transformations.
 
 Unasyncd features:
 
 1. Transformation of arbitrary modules, not bound to any specific directory structure
 2. (Per-file) Exclusion of (nested) functions, classes and methods
-3. Optional transformation of docstring
+3. Optional transformation of docstrings
 4. Replacements based on fully qualified names
    (e.g. `typing.AsyncGenerator` is different than `foo.typing.AsyncGenerator`)
 5. Transformation of constructs like `asyncio.TaskGroup` to a thread based equivalent
 
-*A full list of available transformations is available below.*
+*A full list of supported transformations is available below.*
 
 ## Table of contents
 
+<!-- TOC -->
 * [Unasync](#unasync)
   * [Why?](#why)
   * [Why unasyncd?](#why-unasyncd)
+  * [Table of contents](#table-of-contents)
   * [What can be transformed?](#what-can-be-transformed)
     * [Asynchronous functions](#asynchronous-functions)
     * [`await`](#await)
     * [Asynchronous iterators, iterables and generators](#asynchronous-iterators-iterables-and-generators)
     * [Asynchronous iteration](#asynchronous-iteration)
     * [Asynchronous context managers](#asynchronous-context-managers)
     * [`contextlib.AsyncExitStack`](#contextlibasyncexitstack)
@@ -57,15 +63,16 @@
     * [Type annotations](#type-annotations)
     * [Docstrings](#docstrings)
   * [Usage](#usage)
     * [Installation](#installation)
     * [CLI](#cli)
     * [As a pre-commit hook](#as-a-pre-commit-hook)
     * [Configuration](#configuration)
-      * [Options](#options)
+      * [File](#file)
+      * [CLI options](#cli-options)
       * [Exclusions](#exclusions)
       * [Extending name replacements](#extending-name-replacements)
     * [Handling of imports](#handling-of-imports)
     * [Integration with linters and formatters](#integration-with-linters-and-formatters)
     * [Limitations](#limitations)
     * [Disclaimer](#disclaimer)
 <!-- TOC -->
@@ -73,154 +80,171 @@
 ## What can be transformed?
 
 Unasyncd supports a wide variety of transformation, ranging from simple name
 replacements to more complex transformations such as task groups.
 
 ### Asynchronous functions
 
-Asynchronous functions and methods are replaced with a synchronous version:
-
+*Async*
 ```python
 async def foo() -> str:
     return "hello"
 ```
 
+*Sync*
 ```python
 def foo() -> str:
     return "hello"
 ```
 
 ### `await`
 
-`await` expressions will be unwrapped:
-
+*Async*
 ```python
 await foo()
 ```
 
+*Sync*
 ```python
 foo()
 ```
 
 ### Asynchronous iterators, iterables and generators
 
+*Async*
 ```python
 from typing import AsyncGenerator
 
 async def foo() -> AsyncGenerator[str, None]:
     yield "hello"
 ```
 
+*Sync*
 ```python
 from typing import Generator
 
 def foo() -> Generator[str, None, None]:
     yield "hello"
 ```
 
+*Async*
 ```python
 from typing import AsyncIterator
 
 class Foo:
     async def __aiter__(self) -> AsyncIterator[str]:
         ...
 
     async def __anext__(self) -> str:
         raise StopAsyncIteration
 ```
 
+*Sync*
 ```python
 from typing import Iterator
 
 class Foo:
     def __next__(self) -> str:
         raise StopIteration
 
     def __iter__(self) -> Iterator[str]:
         ...
 ```
 
+*Async*
 ```python
 x = aiter(foo)
 ```
 
+*Sync*
 ```python
 x = iter(foo)
 ```
 
+*Async*
 ```python
 x = await anext(foo)
 ```
 
+*Sync*
 ```python
 x = next(foo)
 ```
 
 ### Asynchronous iteration
 
+*Async*
 ```python
 async for x in foo():
     pass
 ```
 
+*Sync*
 ```python
 for x in foo():
     pass
 ```
 
 ### Asynchronous context managers
 
+*Async*
 ```python
 async with foo() as something:
     pass
 ```
 
+*Sync*
 ```python
 with foo() as something:
     pass
 ```
 
+*Async*
 ```python
 class Foo:
     async def __aenter__(self):
         ...
 
     async def __aexit__(self, exc_type, exc_val, exc_tb):
         ...
 ```
 
+*Sync*
 ```python
 class Foo:
     def __enter__(self):
         ...
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         ...
 ```
 
+*Async*
 ```python
 from contextlib import asynccontextmanager
 from typing import AsyncGenerator
 
 @asynccontextmanager
 async def foo() -> AsyncGenerator[str, None]:
     yield "hello"
 ```
 
+*Sync*
 ```python
 from contextlib import contextmanager
 from typing import Generator
 
 @contextmanager
 def foo() -> Generator[str, None, None]:
     yield "hello"
 ```
 
 ### `contextlib.AsyncExitStack`
 
+*Async*
 ```python
 import contextlib
 
 async with contextlib.AsyncExitStack() as exit_stack:
     exit_stack.enter_context(context_manager_one())
     exit_stack.push(callback_one)
     exit_stack.callback(on_exit_one)
@@ -228,14 +252,15 @@
     await exit_stack.enter_async_context(context_manager_two())
     exit_stack.push_async_exit(on_exit_two)
     exit_stack.push_async_callback(callback_two)
 
     await exit_stack.aclose()
 ```
 
+*Sync*
 ```python
 import contextlib
 
 with contextlib.ExitStack() as exit_stack:
     exit_stack.enter_context(context_manager_one())
     exit_stack.push(callback_one)
     exit_stack.callback(on_exit_one)
@@ -247,59 +272,65 @@
     exit_stack.close()
 ```
 
 See [limitations](#limitations)
 
 ### `asyncio.TaskGroup`
 
+*Async*
 ```python
 import asyncio
 
 async with asyncio.TaskGroup() as task_group:
     task_group.create_task(something(1, 2, 3, this="that"))
 ```
 
+*Sync*
 ```python
 import concurrent.futures
 
 with concurrent.futures.ThreadPoolExecutor() as executor:
     executor.submit(something, 1, 2, 3, this="that")
 ```
 
 See [limitations](#limitations)
 
 
 ### `anyio.create_task_group`
 
+*Async*
 ```python
 import anyio
 
 async with anyio.create_task_group() as task_group:
     task_group.start_soon(something, 1, 2, 3)
 ```
 
+*Sync*
 ```python
 import concurrent.futures
 
 with concurrent.futures.ThreadPoolExecutor() as executor:
     executor.submit(something, 1, 2, 3)
 ```
 
 See [limitations](#limitations)
 
 ### `asyncio.sleep` / `anyio.sleep`
 
 Calls to `asyncio.sleep` and `anyio.sleep` will be replaced with calls to `time.sleep`:
 
+*Async*
 ```python
 import asyncio
 
 await asyncio.sleep(1)
 ```
 
+*Sync*
 ```python
 import time
 
 time.sleep(1)
 ```
 
 If the call argument is `0`, the call will be replaced entirely:
@@ -319,21 +350,23 @@
 | `typing.AsyncGenerator[int, str]` | `typing.Generator[int, str, None]` |
 
 
 ### Docstrings
 
 Simply token replacement is available in docstrings:
 
+*Async*
 ```python
 async def foo():
     """This calls ``await bar()`` and ``asyncio.sleep``"""
 ```
 
+*Sync*
 ```python
-async def foo():
+def foo():
     """This calls ``bar()`` and ``time.sleep``"""
 ```
 
 
 ## Usage
 
 ### Installation
@@ -371,29 +404,28 @@
 ```
 
 ### Configuration
 
 Unasyncd can be configured via a `pyproject.toml` file, a dedicated `.unasyncd.toml`
 file or the command line interface.
 
-#### Options
+#### File
 
-| config file key             | CLI                             | default | description                                                                        |
-|-----------------------------|---------------------------------|---------|------------------------------------------------------------------------------------|
-| `files`                     |                                 | -       | A table mapping source file names / directories to target file names / directories |
-| `exclude`                   | N/A                             | -       | An array of names to exclude from transformation                                   |
-| `per_file_exclude`          | N/A                             | -       | A table mapping files names to an array of names to exclude from transformation    |
-| `add_replacements`          | N/A                             | -       | A table of additional name replacements                                            |
-| `per_file_add_replacements` | N/A                             | -       | A table mapping file names to tables of additional replacements                    |
-| `transform_docstrings`      | `-d` / `--transform-docstrings` | false   | Enable transformation of docstrings                                                |
-| `add_editors_note`          | `--add-editors-note`            | false   | Add a note on top of the generated files                                           |
-| `remove_unuse_imports`      | `--remove-unused-imports`       | false   | Remove imports that have become unused after the transformation                    |
-| `no_cache`                  | `--no-cache`                    | false   | Disable caching                                                                    |
-| `force_regen`               | `--force-regen`                 | false   | Always regenerate files, regardless if their content has changed                   |
-| N/A                         | `-c` / `--config``              | -       | Specify an alternative configuration file                                          |
+| config file key               | type  | default | description                                                                        |
+|-------------------------------|-------|---------|------------------------------------------------------------------------------------|
+| `files`                       | table | -       | A table mapping source file names / directories to target file names / directories |
+| `exclude`                     | array | -       | An array of names to exclude from transformation                                   |
+| `per_file_exclude`            | table | -       | A table mapping files names to an array of names to exclude from transformation    |
+| `add_replacements`            | table | -       | A table of additional name replacements                                            |
+| `per_file_add_replacements`   | table | -       | A table mapping file names to tables of additional replacements                    |
+| `transform_docstrings`        | bool  | false   | Enable transformation of docstrings                                                |
+| `add_editors_note`            | bool  | false   | Add a note on top of the generated files                                           |
+| `infer_type_checking_imports` | bool  | true    | Infer if new imports should be added to an 'if TYPE_CHECKING' block                |
+| `cache`                       | bool  | true    | Cache transformation results                                                       |
+| `force_regen`                 | bool  | false   | Always regenerate files, regardless if their content has changed                   |
 
 **Example**
 
 ```toml
 [tool.unasyncd]
 files = { "async_thing.py" = "sync_thing.py", "foo.py" = "bar.py" }
 exclude = ["Something", "SomethingElse.within"]
@@ -403,14 +435,43 @@
 transform_docstrings = true
 remove_unused_imports = false
 no_cache = false
 no_cache = false
 force_regen = false
 ```
 
+#### CLI options
+
+*Feature flags corresponding to configuration values*
+
+| option                             | description                                                         |
+|------------------------------------|---------------------------------------------------------------------|
+| `--cache`                          | Cache transformation results                                        |
+| `--no-cache `                      | Don't cache transformation results                                  |
+| `--transform-docstrings`           | Enable transformation of docstrings                                 |
+| `--no-transform-docstrings`        | Inverse of `--transform-docstrings`                                 |
+| `--infer-type-checking-imports`    | Infer if new imports should be added to an 'if TYPE_CHECKING' block |
+| `--no-infer-type-checking-imports` | Inverse of `infer-type-checking-imports`                            |
+| `--add-editors-note`               | Add a note on top of each generated file                            |
+| `--no-add-editors-note`            | Inverse of `--add-editors-note`                                     |
+| `--force`                          | Always regenerate files, regardless if their content has changed    |
+| `--no-force`                       | Inverse of `--force`                                                |
+| `--check`                          | Don't write changes back to files                                   |
+| `--write`                          | Inverse of `--check`                                                |
+
+
+*Additional CLI options*
+
+| option      | description                          |
+|-------------|--------------------------------------|
+| `--config`  | Alternative configuration file       |
+| `--verbose` | Increase verbosity of console output |
+| `--quiet`   | Suppress all console output          |
+
+
 #### Exclusions
 
 It is possible to exclude specific functions classes and methods from the
 transformation. This can be achieved by adding their fully qualified name
 (relative to the transformed module) under the `exclude` key:
 
 ```toml
@@ -460,35 +521,21 @@
    `from typing import Generator`
 2. Existing imports will be updated if possible, for instance `from time import time`
    would become `from time import time, sleep` if `sleep` has been added by unasyncd
    during the transformation
 3. New imports are added before the first non-import block that's not a docstring or a
    comment
 
-By default, unasyncd will not remove imports that have become unused as a result of the
-applied transformations. This is because tracking of usages is a complex task and best
-left to tools made specifically for this job like [ruff](https://beta.ruff.rs/docs) or
-[autoflake](https://github.com/PyCQA/autoflake). It can also be a performance benefit
-of not doing this work twice, e.g. when employing one of the aforementioned tools either
-way.
-
-
-### Integration with linters and formatters
-
-Unasyncd should be run **after** tools that change the AST (e.g. isort, ruff), and
-**before** tools that apply transformations in a way that does not change the AST
-(e.g. black).
-
-The reason for this is to avoid multiple passes being required until a stable state is
-reached. Since unasyncd will only re-apply transformations to files which are no longer
-AST equivalent, running it after tools that break AST equivalence solve this issue.
-
-In practice this means all transformations aside from comments and formatting should be
-applied before unasyncd.
+Unasyncd will not remove imports that have become unused as a result of the applied
+transformations. This is because tracking of usages is a complex task and best left to
+tools made specifically for this job like [ruff](https://beta.ruff.rs/docs) or
+[autoflake](https://github.com/PyCQA/autoflake).
 
+Not doing this work twice - e.g. employing a tool to automatically remove unused
+imports alongside unasyncd - can also be a significant performance improvement.
 
 ### Limitations
 
 Transformations for `contextlib.AsyncContextManager`, `asyncio.TaskGroup` and
 `anyio.create_task_group` only work when they're being called in a `with` statement
 directly. This is due to the fact that unasyncd does not track assignments or support
 type inference. Support for these usages might be added in a future version.
```

### Comparing `unasyncd-0.1.1/pyproject.toml` & `unasyncd-0.2.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 [tool.poetry]
 name = "unasyncd"
-version = "0.1.1"
-description = ""
+version = "0.2.0"
+description = "A tool to transform asynchronous Python code to synchronous Python code."
 authors = ["Janek Nouvertné <j.a.nouvertne@posteo.de>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 libcst = "^1.0.0"
 click = "^8.1.3"
 rich = "^13.4.1"
 anyio = "^3.7.0"
 msgspec = "^0.15.1"
 tomli-w = "^1.0.0"
+rich-click = "^1.6.1"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
 pre-commit = "^3.3.2"
 pytest-mock = "^3.10.0"
```

### Comparing `unasyncd-0.1.1/unasyncd/cli.py` & `unasyncd-0.2.0/unasyncd/cli.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import asyncio
 import time
 from pathlib import Path
 
-import click
 import rich
+import rich_click as click
 
 from .config import Config, load_config
 from .main import unasync_files
 
 
 async def _run(*, config: Config, check_only: bool, verbose: bool) -> bool:
     console = rich.get_console()
@@ -43,62 +43,70 @@
         "left unchanged"
     )
 
     return files_changed > 0
 
 
 @click.command()
-@click.option("--no-cache", is_flag=True, help="Disable caching", default=None)
 @click.option(
-    "-d",
-    "--transform-docstrings",
+    "--cache/--no-cache",
     is_flag=True,
+    help="Cache transformation results",
     default=None,
-    help="Transform module, class, method and function docstrings. CST mode only",
 )
 @click.option(
-    "-i",
-    "--remove-unused-imports",
+    "--transform-docstrings/--no-transform-docstrings",
     is_flag=True,
     default=None,
-    help="Remove imports that are unused as a result of the transformation. CST mode "
-    "only",
+    help="Transform module, class, method and function docstrings",
 )
 @click.option(
-    "--add-editors-note",
+    "--infer-type-checking-imports/--no-infer-type-checking-imports",
     is_flag=True,
     default=None,
-    help="Don't add an editors note to the generated files",
+    help="Infer if new imports should be added to an 'if TYPE_CHECKING' block",
+)
+@click.option(
+    "--add-editors-note/--no-add-editors-note",
+    is_flag=True,
+    default=None,
+    help="Add an editors note to the generated files",
+)
+@click.option(
+    "--check/--write",
+    "check_only",
+    is_flag=True,
+    default=None,
+    help="Write changes back",
 )
-@click.option("--check", "check_only", is_flag=True, help="Don't write changes back")
 @click.option(
     "-c",
     "--config",
     "config_file",
     help="Configuration file. If not given defaults to pyproject.toml",
     type=click.Path(dir_okay=False, path_type=Path),
 )
 @click.option(
-    "-f",
-    "--force",
+    "-f/-F",
+    "--force/--no-force",
     "force_regen",
     help="Force regeneration regardless of changes",
     is_flag=True,
     default=None,
 )
 @click.option(
     "-v", "--verbose", is_flag=True, help="Increase verbosity of console output"
 )
 @click.option("-q", "--quiet", is_flag=True, help="Suppress all console output")
 @click.argument("files", nargs=-1)
 def main(
     files: tuple[str, ...],
-    no_cache: bool | None,
+    cache: bool | None,
     transform_docstrings: bool | None,
-    remove_unused_imports: bool | None,
+    infer_type_checking_imports: bool | None,
     check_only: bool,
     add_editors_note: bool | None,
     config_file: Path | None,
     force_regen: bool | None,
     verbose: bool,
     quiet: bool,
 ) -> None:
@@ -112,21 +120,21 @@
                 config_file = path
 
     if config_file:
         console.print(f"[cyan]Config file: [yellow][b]{config_file}")
 
     config = load_config(
         path=config_file,
-        no_cache=no_cache,
+        cache=cache,
         transform_docstrings=transform_docstrings,
-        remove_unused_imports=remove_unused_imports,
         add_editors_note=add_editors_note,
         files=dict(f.split(":", 1) for f in files) if files else None,
         check_only=check_only,
         force_regen=force_regen,
+        infer_type_checking_imports=infer_type_checking_imports,
     )
 
     if not config.files:
         console.print("[red]No files selected. Quitting")
     else:
         quit(
             int(
```

### Comparing `unasyncd-0.1.1/unasyncd/config.py` & `unasyncd-0.2.0/unasyncd/config.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 
 import msgspec
 
 
 class Config(msgspec.Struct):
     add_editors_note: bool
     transform_docstrings: bool
-    remove_unused_imports: bool
-    no_cache: bool
+    cache: bool
     extra_replacements: dict[str, dict[str, str]]
     exclude: dict[str, list[str]]
     files: dict[str, str]
     force_regen: bool
     check_only: bool
+    infer_type_checking_imports: bool
 
     def key(self) -> str:
         return hashlib.sha1(msgspec.json.encode(self)).hexdigest()
 
 
 def _collect_paths(file_names: dict[str, str]) -> dict[str, str]:
     files = {}
@@ -65,13 +65,13 @@
             for file in itertools.chain(files, per_file_extra_replacements)
         },
         exclude={
             file: [*exclude, *per_file_exclude.get(file, [])]
             for file in itertools.chain(files, per_file_exclude)
         },
         add_editors_note=raw_config.get("add_editors_note", False),
-        remove_unused_imports=raw_config.get("remove_unused_imports", False),
         transform_docstrings=raw_config.get("transform_docstrings", False),
-        no_cache=raw_config.get("no_cache", False),
+        cache=raw_config.get("cache", True),
         check_only=raw_config.get("check_only", False),
         force_regen=raw_config.get("force_regen", False),
+        infer_type_checking_imports=raw_config.get("infer_type_checking_imports", True),
     )
```

### Comparing `unasyncd-0.1.1/unasyncd/main.py` & `unasyncd-0.2.0/unasyncd/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -172,16 +172,16 @@
         configuration
         """
         from .transformers import TreeTransformer
 
         transformer = TreeTransformer(
             exclude=self.config.exclude.get(str(file), set()),
             transform_docstrings=self.config.transform_docstrings,
-            remove_unused_imports=self.config.remove_unused_imports,
             extra_name_replacements=self.config.extra_replacements.get(str(file), {}),
+            infer_type_checking_imports=self.config.infer_type_checking_imports,
         )
 
         content = await file.get_content()
         loop = asyncio.get_running_loop()
         transformed = await loop.run_in_executor(self._executor, transformer, content)
         if self.config.add_editors_note:
             note = (
@@ -243,15 +243,15 @@
         target_file = File(target_path)
 
         if not await self.files_diverged(source_file, target_file):
             return TransformationResult(
                 source=source_file, target=target_file, transformed=False
             )
 
-        if not self.config.no_cache:
+        if self.config.cache:
             if await self._restore_from_cache(source_file, target_file):
                 return TransformationResult(
                     source=source_file, target=target_file, transformed=True
                 )
 
         await self.set_meta(source_file)
 
@@ -271,15 +271,15 @@
             ):
                 await target_file.parent.mkdir(parents=True, exist_ok=True)
                 await target_file.write_text(transformed_content)
                 transformation_result.transformed = True
 
             await self.set_meta(target_file)
 
-        if not self.config.no_cache:
+        if self.config.cache:
             await self.cache.set(
                 await self._cache_key_for(source_file), transformed_content
             )
 
         return transformation_result
 
     async def unasync_files(self) -> AsyncGenerator[TransformationResult, None]:
```

### Comparing `unasyncd-0.1.1/unasyncd/transformers.py` & `unasyncd-0.2.0/unasyncd/transformers.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
+import dataclasses
 import itertools
 import re
 from collections import defaultdict
 from collections.abc import Iterable, Sequence
-from dataclasses import dataclass
 from typing import Any, TypeVar
 
 import libcst as cst
 import libcst.matchers as m
 from libcst import MetadataWrapper
 from libcst.metadata import QualifiedName, ScopeProvider
 from libcst.native import parse_module
@@ -45,27 +45,26 @@
     **NAME_REPLACEMENTS,
 }
 
 
 ASYNC_GEN_RE = re.compile(r"AsyncGenerator\[(.+,.+)]")
 
 
-@dataclass
+@dataclasses.dataclass
 class TransformerMeta:
-    module_imports: dict[str, AnyImport]
     needs_from_import: defaultdict[str, set[str]]
     needs_module_import: set[str]
     exclude: set[tuple[str, ...]]
     removed_names: defaultdict[str, set[str]]
 
 
-@dataclass
+@dataclasses.dataclass
 class ImportMeta:
-    module_imports: dict[str, cst.Import]
-    from_imports: dict[str, cst.ImportFrom]
+    module_imports: dict[str, cst.Import] = dataclasses.field(default_factory=dict)
+    from_imports: dict[str, cst.ImportFrom] = dataclasses.field(default_factory=dict)
 
 
 class StringTransformer:
     """A simple string based transformer"""
 
     def __init__(self, extra_name_replacements: dict[str, str] | None = None) -> None:
         self.replacements = {**UNASYNC_REPLACEMENTS, **(extra_name_replacements or {})}
@@ -126,43 +125,58 @@
     val = expr.value
     if isinstance(val, cst.SimpleString | cst.ConcatenatedString):
         return val
 
     return None
 
 
+def _get_full_name_for_import_from(node: cst.ImportFrom) -> str:
+    return (
+        cst.helpers.get_full_name_for_node_or_raise(node.module)
+        if node.module
+        else "." * len(node.relative)
+    )
+
+
+def _create_import_from(module_name: str, names: Iterable[str]) -> cst.ImportFrom:
+    return cst.ImportFrom(
+        module=_create_name_or_attr(module_name),
+        names=[cst.ImportAlias(cst.Name(name)) for name in names],
+    )
+
+
 class TreeTransformer:
     """libcst based transformer"""
 
     def __init__(
         self,
         exclude: Iterable[str] | None = None,
         transform_docstrings: bool = True,
         extra_name_replacements: dict[str, str] | None = None,
-        remove_unused_imports: bool = False,
+        infer_type_checking_imports: bool = True,
     ) -> None:
         self.exclude = exclude
         self.transform_docstrings = transform_docstrings
         self.name_replacements = {
             **NAME_REPLACEMENTS,
             **(extra_name_replacements or {}),
         }
-        self.remove_unused_imports = remove_unused_imports
+        self.infer_type_checking_imports = infer_type_checking_imports
 
     def __call__(self, source: str) -> str:
         if not source:
             return ""
 
         wrapper = MetadataWrapper(parse_module(source), unsafe_skip_copy=True)
         result = wrapper.visit(
             _AsyncTransformer(
                 exclude=self.exclude,
                 name_replacements=self.name_replacements,
                 transform_docstrings=self.transform_docstrings,
-                remove_unused_imports=self.remove_unused_imports,
+                infer_type_checking_imports=self.infer_type_checking_imports,
             )
         )
         output = result.code
 
         # newlines at the end can get lost so ensure we have one
         if source[-1] == result.default_newline and not result.has_trailing_newline:
             output += result.default_newline
@@ -356,50 +370,75 @@
 
     def __init__(
         self,
         *,
         exclude: Iterable[str] | None = None,
         name_replacements: dict[str, str],
         transform_docstrings: bool,
-        remove_unused_imports: bool,
+        infer_type_checking_imports: bool = True,
     ):
         """
 
         :param exclude: Iterable of fully qualified names of classes, methods and
             functions to exclude
         :param name_replacements: Mapping of fully qualified names to their replacements
         :param transform_docstrings: If ``True``, transform docstrings
-        :param remove_unused_imports:  If ``True`` remove module level imports that have
-            become unused due to the transformation
         """
         super().__init__()
-        self._current_scop_name: tuple[str, ...] = tuple()
-        self._name_replacements = name_replacements
         self._should_transform_docstrings = transform_docstrings
-        self.meta = TransformerMeta(
-            module_imports={},
-            needs_from_import=defaultdict(set),
-            exclude={tuple(p.split(".")) for p in exclude or []},
-            removed_names=defaultdict(set),
-            needs_module_import=set(),
-        )
-        self._in_import = False
-        self.attribute_replacements = {
+        self._should_infer_type_checking_imports = infer_type_checking_imports
+        self._name_replacements = name_replacements
+        self._attribute_replacements = {
             name: replacement
             for name, replacement in name_replacements.items()
             if "." in name
         }
-        self.expressions_to_remove: set[cst.Expr] = set()
-        self.scoped_node_imports: defaultdict[cst.CSTNode, ImportMeta] = defaultdict(
+
+        self._scoped_node_imports: defaultdict[cst.CSTNode, ImportMeta] = defaultdict(
             lambda: ImportMeta(module_imports={}, from_imports={})
         )
-        self._scope_nodes: list[cst.CSTNode] = []
-        self.remove_unused_imports = remove_unused_imports
+
+        self._expressions_to_remove: set[cst.Expr] = set()
         self._string_transformer = StringTransformer()
 
+        self._current_scop_name: tuple[str, ...] = tuple()
+        self._scope_nodes: list[cst.CSTNode] = []
+
+        self._if_type_checking_node: cst.If | None = None
+        self._if_type_checking_imports: set[AnyImport] = set()
+        self._in_if_type_checking_block: bool = False
+        self._in_import = False
+
+        self.meta = TransformerMeta(
+            needs_from_import=defaultdict(set),
+            needs_module_import=set(),
+            removed_names=defaultdict(set),
+            exclude={tuple(p.split(".")) for p in exclude or []},
+        )
+
+    def visit_If(self, node: cst.If) -> bool | None:
+        if (
+            isinstance(node.test, cst.Name)
+            and self.get_qualified_name(node.test) == "typing.TYPE_CHECKING"
+        ):
+            self._if_type_checking_node = node
+            self._in_if_type_checking_block = True
+
+        return None
+
+    def leave_If(self, original_node: cst.If, updated_node: cst.If) -> Any:
+        if original_node is self._if_type_checking_node:
+            self._in_if_type_checking_block = False
+
+            # replace with the updated node, so we can check for identity later on when
+            # performing transformations
+            self._if_type_checking_node = updated_node
+
+        return updated_node
+
     @property
     def current_scope_node(self) -> cst.CSTNode | None:
         """The parent node of the current scope (excludes comprehension scope)"""
         if self._scope_nodes:
             return self._scope_nodes[-1]
         return None
 
@@ -488,14 +527,42 @@
             updated_node = updated_node.with_deep_changes(  # type: ignore[assignment]
                 docstring_node,
                 value=quote + updated_docstring + quote,
             )
 
         return updated_node
 
+    def _register_import(self, node: cst.Import | cst.ImportFrom) -> None:
+        if not self.current_scope_node:
+            return
+
+        node_imports = self._scoped_node_imports[self.current_scope_node]
+        if isinstance(node, cst.Import):
+            for name in node.names:
+                node_imports.module_imports[name.evaluated_name] = node
+            return None
+
+        module_name = _get_full_name_for_import_from(node)
+        node_imports.from_imports[module_name] = node
+
+    def _leave_any_import(
+        self, original_node: AnyImport, updated_node: AnyImport
+    ) -> (
+        cst.BaseSmallStatement
+        | cst.FlattenSentinel[cst.BaseSmallStatement]
+        | cst.RemovalSentinel
+    ):
+        self._in_import = False
+
+        self._register_import(updated_node)
+        if self._in_if_type_checking_block:
+            self._if_type_checking_imports.add(updated_node)
+
+        return updated_node
+
     def visit_ImportFrom(self, node: cst.ImportFrom) -> bool:
         self._in_import = True
         return True
 
     def visit_Import(self, node: cst.Import) -> bool | None:
         self._in_import = True
         return None
@@ -503,53 +570,32 @@
     def leave_ImportFrom(
         self, original_node: cst.ImportFrom, updated_node: cst.ImportFrom
     ) -> (
         cst.BaseSmallStatement
         | cst.FlattenSentinel[cst.BaseSmallStatement]
         | cst.RemovalSentinel
     ):
-        self._in_import = False
-        self.register_import(updated_node)
-        return updated_node
+        return self._leave_any_import(original_node, updated_node)
 
     def leave_Import(
         self, original_node: cst.Import, updated_node: cst.Import
     ) -> (
         cst.BaseSmallStatement
         | cst.FlattenSentinel[cst.BaseSmallStatement]
         | cst.RemovalSentinel
     ):
-        self._in_import = False
-        self.register_import(updated_node)
-        return updated_node
-
-    def register_import(self, node: cst.Import | cst.ImportFrom) -> None:
-        if not self.current_scope_node:
-            return
-
-        node_imports = self.scoped_node_imports[self.current_scope_node]
-        if isinstance(node, cst.Import):
-            for name in node.names:
-                node_imports.module_imports[name.evaluated_name] = node
-            return None
-
-        module_name = (
-            cst.helpers.get_full_name_for_node_or_raise(node.module)
-            if node.module
-            else "." * len(node.relative)
-        )
-        node_imports.from_imports[module_name] = node
+        return self._leave_any_import(original_node, updated_node)
 
     def leave_Attribute(
         self, original_node: cst.Attribute, updated_node: cst.Attribute
     ) -> cst.BaseExpression:
         if not (qualified_name := self.get_qualified_name(original_node)):
             return updated_node
 
-        if not (replacement := self.attribute_replacements.get(qualified_name)):
+        if not (replacement := self._attribute_replacements.get(qualified_name)):
             return updated_node
 
         module_name, attr = qualified_name.rsplit(".", 1)
         self.meta.removed_names[module_name].add(attr)
         self.meta.needs_module_import.add(replacement.rsplit(".", 1)[0])
 
         return _create_name_or_attr(replacement)
@@ -657,25 +703,25 @@
             qualified_name = self.get_qualified_name(call)
             if qualified_name not in {"asyncio.sleep", "anyio.sleep"}:
                 return True
 
             if m.matches(
                 call, m.Call(args=[m.AtLeastN(m.Arg(m.Integer(value="0")), n=1)])
             ):
-                self.expressions_to_remove.add(node)
+                self._expressions_to_remove.add(node)
                 removed_mod, removed_name = qualified_name.split(".")
                 self.meta.removed_names[removed_mod].add(removed_name)
                 return False
         return True
 
     def leave_Expr(
         self, original_node: cst.Expr, updated_node: cst.Expr
     ) -> cst.BaseSmallStatement | cst.RemovalSentinel:
         """Remove expressions registered to be removed"""
-        if original_node in self.expressions_to_remove:
+        if original_node in self._expressions_to_remove:
             return cst.RemoveFromParent()
         return updated_node
 
     def leave_Await(
         self, original_node: cst.Await, updated_node: cst.Await
     ) -> cst.BaseExpression | Any:
         """Unwrap await: ``await foo`` > ``foo``"""
@@ -706,75 +752,14 @@
 
         none_element = cst.SubscriptElement(slice=cst.Index(cst.Name("None")))
         updated_node = updated_node.with_changes(
             slice=[*updated_node.slice, none_element]
         )
         return updated_node
 
-    def _get_imports_from_module(
-        self, wrapper: MetadataWrapper
-    ) -> tuple[
-        dict[str, cst.Import], dict[str, cst.ImportFrom], dict[AnyImport, set[str]]
-    ]:
-        """Gather information about module level imports.
-
-        Return a tuple of:
-            - ``Import`` statements
-            - ``ImportFrom`` statements
-            - Imported names that have become unused due to the applied transformations
-        """
-        from_imports: dict[str, cst.ImportFrom] = {}
-        module_imports: dict[str, cst.Import] = {}
-        imports_to_remove: defaultdict[AnyImport, set[str]] = defaultdict(set)
-        scopes = set(
-            s
-            for s in wrapper.resolve(ScopeProvider).values()
-            if isinstance(s, cst.metadata.GlobalScope)
-        )
-        scope = scopes.pop()
-
-        for assignment in scope.assignments:
-            if not isinstance(assignment, cst.metadata.Assignment):
-                continue
-
-            node = assignment.node
-
-            if isinstance(node, cst.Import):
-                module_imports[assignment.name] = node
-
-                if assignment.references:
-                    continue
-
-                removed_names = self.meta.removed_names.get(assignment.name)
-                if removed_names:
-                    imports_to_remove[node].add(assignment.name)
-
-            elif isinstance(node, cst.ImportFrom):
-                module_name = (
-                    cst.helpers.get_full_name_for_node_or_raise(node.module)
-                    if node.module
-                    else "." * len(node.relative)
-                )
-                from_imports[module_name] = node
-
-                if assignment.references:
-                    continue
-
-                if not (removed_names := self.meta.removed_names.get(module_name)):
-                    continue
-
-                if isinstance(node.names, cst.ImportStar):
-                    continue
-
-                imported_names = {alias.evaluated_name for alias in node.names}
-                if names_to_remove := imported_names.intersection(removed_names):
-                    imports_to_remove[node].update(names_to_remove)
-
-        return module_imports, from_imports, imports_to_remove
-
     def _find_first_non_import_line(self, updated_node: cst.Module) -> int:
         """Get the index of the first line of the module that is not an import,
         skipping module level docstrings and comments.
         """
         import_matcher = m.SimpleStatementLine(
             body=[m.AtLeastN(m.OneOf(m.Import(), m.ImportFrom()), n=1)]
         )
@@ -782,151 +767,245 @@
         for i, node in enumerate(updated_node.body):
             if m.matches(node, string_matcher):
                 continue
             if not m.matches(node, import_matcher):
                 return i
         return 0
 
+    def _extract_if_type_checking_imports(
+        self, existing_imports: dict[str, AnyImportT]
+    ) -> dict[str, set[str]]:
+        type_checking_imports: dict[str, set[str]] = defaultdict(set)
+        for module_name, import_ in existing_imports.items():
+            if import_ not in self._if_type_checking_imports:
+                continue
+            if not isinstance(import_.names, cst.ImportStar):
+                type_checking_imports[module_name].update(
+                    [n.evaluated_alias or n.evaluated_name for n in import_.names]
+                )
+        return type_checking_imports
+
     def _create_from_imports(
-        self, existing_from_imports: dict[str, cst.ImportFrom]
+        self,
+        existing_from_imports: dict[str, cst.ImportFrom],
+        replaced_names: dict[str, dict[str, str]],
+        new_type_checking_imports: set[AnyImport],
     ) -> tuple[dict[cst.ImportFrom, set[str]], list[cst.ImportFrom]]:
         """Return a tuple of ``FromImport``s to update and ``FromImport``s to add"""
         from_imports_to_update: defaultdict[cst.ImportFrom, set[str]] = defaultdict(set)
         from_imports_to_add: defaultdict[str, set[str]] = defaultdict(set)
+        existing_if_type_checking_imports = self._extract_if_type_checking_imports(
+            existing_from_imports
+        )
 
         for module_name, names in self.meta.needs_from_import.items():
             if _import := existing_from_imports.get(module_name):
                 if isinstance(_import.names, cst.ImportStar):
                     continue
                 existing_names = {
                     alias.evaluated_alias or alias.evaluated_name
                     for alias in _import.names
                 }
                 from_imports_to_update[_import].update(names - existing_names)
             else:
                 from_imports_to_add[module_name].update(names)
 
-        new_from_imports = [
-            cst.ImportFrom(
-                module=_create_name_or_attr(module_name),
-                names=[cst.ImportAlias(cst.Name(name)) for name in names],
-            )
-            for module_name, names in from_imports_to_add.items()
-        ]
-        return from_imports_to_update, new_from_imports
+        new_imports = []
+        for module_name, names in from_imports_to_add.items():
+            new_import_names = set()
+            new_type_checking_import_names = set()
+
+            if replaced_imports := replaced_names.get(module_name):
+                # we have replaced names, so we check for the ones that exist
+                # exclusively within an if TYPE_CHECKING block to ensure we only add
+                # those there
+                for new_name in names:
+                    original_fq_name = replaced_imports[new_name]
+                    orig_module_name, orig_name = original_fq_name.rsplit(".", 1)
+                    if orig_name in existing_if_type_checking_imports.get(
+                        orig_module_name, []
+                    ):
+                        new_type_checking_import_names.add(new_name)
+                    else:
+                        new_import_names.add(new_name)
+            else:
+                new_import_names.update(names)
+
+            if new_import_names:
+                new_imports.append(_create_import_from(module_name, new_import_names))
+
+            if new_type_checking_import_names:
+                new_type_checking_imports.add(
+                    _create_import_from(module_name, new_type_checking_import_names)
+                )
+
+        return from_imports_to_update, new_imports
 
     def _create_module_imports(
-        self, existing_module_import: dict[str, cst.Import]
-    ) -> list[cst.Import]:
+        self,
+        existing_module_imports: dict[str, cst.Import],
+        replaced_names: dict[str, dict[str, str]],
+        type_checking_imports: set[AnyImport],
+    ) -> set[cst.Import]:
         """Return a list of ``Import``s to add"""
-        return [
-            cst.Import(names=[cst.ImportAlias(name=_create_name_or_attr(module_name))])
-            for module_name in self.meta.needs_module_import
-            if not (_import := existing_module_import.get(module_name))
-            and not isinstance(_import, cst.ImportFrom)
-        ]
+        new_imports: set[cst.Import] = set()
+        existing_tc_import = self._extract_if_type_checking_imports(
+            existing_module_imports
+        )
+        for module_name in self.meta.needs_module_import:
+            if _import := existing_module_imports.get(module_name):
+                continue
+
+            if isinstance(_import, cst.ImportFrom):
+                continue
+
+            new_import = cst.Import(
+                names=[cst.ImportAlias(name=_create_name_or_attr(module_name))]
+            )
+
+            maybe_replaced_imports = replaced_names.get(module_name)
+            if not maybe_replaced_imports:
+                new_imports.add(new_import)
+                continue
+
+            for new_name, original_fq_name in maybe_replaced_imports.items():
+                orig_module_name, _ = original_fq_name.rsplit(".", 1)
+                if orig_module_name in existing_tc_import:
+                    type_checking_imports.add(new_import)
+                else:
+                    new_imports.add(new_import)
+
+        return new_imports
 
     def _fix_module_imports(
         self,
         *,
         node: cst.Module | MetadataWrapper,
         from_imports: dict[str, cst.ImportFrom],
         module_imports: dict[str, cst.Import],
-        imports_to_remove: dict[AnyImport, set[str]],
     ) -> cst.Module:
         """Modify a module's imports.
 
         - Update existing imports with names that have been requested by a
           transformation
         - Add new imports that have not been covered in the previous step
         - Remove names from imports specified in ``imports_to_remove``. If an import has
           no names left, it is removed entirely
         """
+        maybe_replaced_names: dict[str, dict[str, str]] = defaultdict(dict)
+        add_to_typechecking_import: set[AnyImport] = set()
+
+        for name, replacement in self._name_replacements.items():
+            if "." not in name:
+                continue
+            module_name, replacement = replacement.rsplit(".", 1)
+            maybe_replaced_names[module_name][replacement] = name
+
         from_imports_to_update, new_from_imports = self._create_from_imports(
-            from_imports
+            from_imports,
+            replaced_names=maybe_replaced_names,
+            new_type_checking_imports=add_to_typechecking_import,
+        )
+        new_module_imports = self._create_module_imports(
+            module_imports,
+            replaced_names=maybe_replaced_names,
+            type_checking_imports=add_to_typechecking_import,
         )
 
+        imports_to_add: Iterable[AnyImport] = itertools.chain(
+            new_from_imports, new_module_imports
+        )
+
+        if not self._should_infer_type_checking_imports:
+            imports_to_add = itertools.chain(imports_to_add, add_to_typechecking_import)
+            add_to_typechecking_import = set()
+
         updated_node = node.visit(
             _ImportTransformer(
-                unused_imports=imports_to_remove,
                 imports_to_update=from_imports_to_update,
+                if_type_checking_node=self._if_type_checking_node,
+                type_checking_imports_to_add=add_to_typechecking_import,
             )
         )
 
-        new_module_imports = self._create_module_imports(module_imports)
         import_offset = self._find_first_non_import_line(updated_node)
+
         new_module_body = [
             *updated_node.body[:import_offset],
-            *[
-                cst.SimpleStatementLine(body=[new_import])
-                for new_import in itertools.chain(new_module_imports, new_from_imports)
-            ],
+            *[cst.SimpleStatementLine([new_import]) for new_import in imports_to_add],
             *updated_node.body[import_offset:],
         ]
-        updated_node = updated_node.with_changes(body=new_module_body)
 
-        if self._should_transform_docstrings and self._should_transform_current_node:
-            updated_node = self._transform_docstring(updated_node)
+        updated_node = updated_node.with_changes(body=new_module_body)
 
         return updated_node
 
     def leave_Module(
         self, original_node: cst.Module, updated_node: cst.Module
     ) -> cst.Module:
-        if self.remove_unused_imports and self.meta.removed_names:
-            wrapper = MetadataWrapper(updated_node)
-            (
-                module_imports,
-                from_imports,
-                imports_to_remove,
-            ) = self._get_imports_from_module(wrapper)
-            return self._fix_module_imports(
-                node=wrapper,
-                module_imports=module_imports,
-                from_imports=from_imports,
-                imports_to_remove=imports_to_remove,
-            )
-
-        import_meta = self.scoped_node_imports[original_node]
-        return self._fix_module_imports(
+        import_meta = self._scoped_node_imports[original_node]
+        updated_node = self._fix_module_imports(
             node=updated_node,
             module_imports=import_meta.module_imports,
             from_imports=import_meta.from_imports,
-            imports_to_remove={},
         )
 
+        if self._should_transform_docstrings and self._should_transform_current_node:
+            updated_node = self._transform_docstring(updated_node)
+
+        return updated_node
+
 
 class _ImportTransformer(cst.CSTTransformer):
-    # taken from
+    # partly taken from
     # https://cst.readthedocs.io/en/latest/scope_tutorial.html#Automatically-Remove-Unused-Import
 
     def __init__(
         self,
         *,
-        unused_imports: dict[AnyImport, set[str]],
         imports_to_update: dict[cst.ImportFrom, set[str]],
+        if_type_checking_node: cst.If | None,
+        type_checking_imports_to_add: Iterable[AnyImport],
     ) -> None:
         super().__init__()
-        self.unused_imports = unused_imports
         self.imports_to_update = imports_to_update
+        self.if_type_checking_node = if_type_checking_node
+        self.type_checking_imports_to_add = type_checking_imports_to_add
+
+    def leave_If(
+        self, original_node: cst.If, updated_node: cst.If
+    ) -> (
+        cst.BaseStatement | cst.FlattenSentinel[cst.BaseStatement] | cst.RemovalSentinel
+    ):
+        if not self.if_type_checking_node:
+            return updated_node
+
+        if original_node is not self.if_type_checking_node:
+            return updated_node
+
+        return updated_node.with_deep_changes(
+            updated_node.body,
+            body=[
+                *updated_node.body.body,
+                *[
+                    cst.SimpleStatementLine([import_])
+                    for import_ in self.type_checking_imports_to_add
+                ],
+            ],
+        )
 
     def leave_import_alike(
         self, original_node: AnyImportT, updated_node: AnyImportT
     ) -> AnyImportT | cst.RemovalSentinel:
-        if original_node not in self.unused_imports or isinstance(
-            updated_node.names, cst.ImportStar
-        ):
+        if isinstance(updated_node.names, cst.ImportStar):
             return updated_node
 
         names_to_keep = []
         for name in updated_node.names:
-            name_value = name.name.value
-
-            if name_value not in self.unused_imports[original_node]:
-                names_to_keep.append(name.with_changes(comma=cst.MaybeSentinel.DEFAULT))
+            names_to_keep.append(name.with_changes(comma=cst.MaybeSentinel.DEFAULT))
 
         if len(names_to_keep) == 0:
             return cst.RemoveFromParent()
         else:
             return updated_node.with_changes(names=names_to_keep)  # type: ignore[return-value]  # noqa: E501
 
     def leave_Import(
```

### Comparing `unasyncd-0.1.1/PKG-INFO` & `unasyncd-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,72 +1,79 @@
 Metadata-Version: 2.1
 Name: unasyncd
-Version: 0.1.1
-Summary: 
+Version: 0.2.0
+Summary: A tool to transform asynchronous Python code to synchronous Python code.
 License: MIT
 Author: Janek Nouvertné
 Author-email: j.a.nouvertne@posteo.de
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: anyio (>=3.7.0,<4.0.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: libcst (>=1.0.0,<2.0.0)
 Requires-Dist: msgspec (>=0.15.1,<0.16.0)
 Requires-Dist: rich (>=13.4.1,<14.0.0)
+Requires-Dist: rich-click (>=1.6.1,<2.0.0)
 Requires-Dist: tomli-w (>=1.0.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 # Unasync
 
 A tool to transform asynchronous Python code to synchronous Python code.
 
 ## Why?
 
 Unasyncd is largely inspired by [unasync](https://github.com/python-trio/unasync), and
 a detailed discussion about this approach can be found
 [here](https://github.com/urllib3/urllib3/issues/1323).
 
-The goal is essentially to reduce to burden of having to maintain both a synchronous and
-an asynchronous version of otherwise functionally identical code. The idea behind
-simply "taking out the async" is that often, synchronous and asynchronous code only
-differ very slightly: A few `await`s, `async def`s and `async with`s, and a couple of
-different method names. The unasync approach makes use of this and provides a way to
-use the asynchronous version as a source of truth from wich the synchronous version can
-be generated.
+Its purpose is to reduce to burden of having to maintain both a synchronous and an
+asynchronous version of otherwise functionally identical code. The idea behind simply
+"taking out the async" is that often, synchronous and asynchronous code only differ
+slightly: A few `await`s, `async def`s, `async with`s, and a couple of different method
+names. The unasync approach makes use of this by treating the asynchronous version as a
+source of truth from wich the synchronous version is then generated.
 
 ## Why unasyncd?
 
-The original [unasync](https://github.com/python-trio/unasync) takes a very simplistic
-approach and works by replacing tokens. This works well enough for most basic use cases,
-but can be somewhat restrictive in the way the code can be written. More complex cases
-such as exclusion of functions / classes or transformations such as `AsyncExitStack` to
-`ExitStack` are not possible, which leads to the introduction of shims, introducing
-additional complexity.
+The original [unasync](https://github.com/python-trio/unasync) works by simply replacing
+certain token, which is enough for most basic use cases, but can be somewhat restrictive
+in the way the code can be written. More complex cases such as exclusion of functions /
+classes or transformations (such as `AsyncExitStack` to `ExitStack` wich have not only
+different names but also different method names that then need to be replaced only
+within a certain scope) are not possible. This can lead to the introduction of shims,
+introducing additional complexity.
+
+Unasyncd's goal is to impose as little restrictions as possible to the way the
+asynchronous code can be written, as long as it maps to a functionally equivalent
+synchronous version.
 
-Unasyncd leverages [libcst](https://libcst.readthedocs.io/), enabling a more granular
-control and more complex transformations.
+To achieve this, unasyncd leverages [libcst](https://libcst.readthedocs.io/), enabling a
+more granular control and complex transformations.
 
 Unasyncd features:
 
 1. Transformation of arbitrary modules, not bound to any specific directory structure
 2. (Per-file) Exclusion of (nested) functions, classes and methods
-3. Optional transformation of docstring
+3. Optional transformation of docstrings
 4. Replacements based on fully qualified names
    (e.g. `typing.AsyncGenerator` is different than `foo.typing.AsyncGenerator`)
 5. Transformation of constructs like `asyncio.TaskGroup` to a thread based equivalent
 
-*A full list of available transformations is available below.*
+*A full list of supported transformations is available below.*
 
 ## Table of contents
 
+<!-- TOC -->
 * [Unasync](#unasync)
   * [Why?](#why)
   * [Why unasyncd?](#why-unasyncd)
+  * [Table of contents](#table-of-contents)
   * [What can be transformed?](#what-can-be-transformed)
     * [Asynchronous functions](#asynchronous-functions)
     * [`await`](#await)
     * [Asynchronous iterators, iterables and generators](#asynchronous-iterators-iterables-and-generators)
     * [Asynchronous iteration](#asynchronous-iteration)
     * [Asynchronous context managers](#asynchronous-context-managers)
     * [`contextlib.AsyncExitStack`](#contextlibasyncexitstack)
@@ -76,15 +83,16 @@
     * [Type annotations](#type-annotations)
     * [Docstrings](#docstrings)
   * [Usage](#usage)
     * [Installation](#installation)
     * [CLI](#cli)
     * [As a pre-commit hook](#as-a-pre-commit-hook)
     * [Configuration](#configuration)
-      * [Options](#options)
+      * [File](#file)
+      * [CLI options](#cli-options)
       * [Exclusions](#exclusions)
       * [Extending name replacements](#extending-name-replacements)
     * [Handling of imports](#handling-of-imports)
     * [Integration with linters and formatters](#integration-with-linters-and-formatters)
     * [Limitations](#limitations)
     * [Disclaimer](#disclaimer)
 <!-- TOC -->
@@ -92,154 +100,171 @@
 ## What can be transformed?
 
 Unasyncd supports a wide variety of transformation, ranging from simple name
 replacements to more complex transformations such as task groups.
 
 ### Asynchronous functions
 
-Asynchronous functions and methods are replaced with a synchronous version:
-
+*Async*
 ```python
 async def foo() -> str:
     return "hello"
 ```
 
+*Sync*
 ```python
 def foo() -> str:
     return "hello"
 ```
 
 ### `await`
 
-`await` expressions will be unwrapped:
-
+*Async*
 ```python
 await foo()
 ```
 
+*Sync*
 ```python
 foo()
 ```
 
 ### Asynchronous iterators, iterables and generators
 
+*Async*
 ```python
 from typing import AsyncGenerator
 
 async def foo() -> AsyncGenerator[str, None]:
     yield "hello"
 ```
 
+*Sync*
 ```python
 from typing import Generator
 
 def foo() -> Generator[str, None, None]:
     yield "hello"
 ```
 
+*Async*
 ```python
 from typing import AsyncIterator
 
 class Foo:
     async def __aiter__(self) -> AsyncIterator[str]:
         ...
 
     async def __anext__(self) -> str:
         raise StopAsyncIteration
 ```
 
+*Sync*
 ```python
 from typing import Iterator
 
 class Foo:
     def __next__(self) -> str:
         raise StopIteration
 
     def __iter__(self) -> Iterator[str]:
         ...
 ```
 
+*Async*
 ```python
 x = aiter(foo)
 ```
 
+*Sync*
 ```python
 x = iter(foo)
 ```
 
+*Async*
 ```python
 x = await anext(foo)
 ```
 
+*Sync*
 ```python
 x = next(foo)
 ```
 
 ### Asynchronous iteration
 
+*Async*
 ```python
 async for x in foo():
     pass
 ```
 
+*Sync*
 ```python
 for x in foo():
     pass
 ```
 
 ### Asynchronous context managers
 
+*Async*
 ```python
 async with foo() as something:
     pass
 ```
 
+*Sync*
 ```python
 with foo() as something:
     pass
 ```
 
+*Async*
 ```python
 class Foo:
     async def __aenter__(self):
         ...
 
     async def __aexit__(self, exc_type, exc_val, exc_tb):
         ...
 ```
 
+*Sync*
 ```python
 class Foo:
     def __enter__(self):
         ...
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         ...
 ```
 
+*Async*
 ```python
 from contextlib import asynccontextmanager
 from typing import AsyncGenerator
 
 @asynccontextmanager
 async def foo() -> AsyncGenerator[str, None]:
     yield "hello"
 ```
 
+*Sync*
 ```python
 from contextlib import contextmanager
 from typing import Generator
 
 @contextmanager
 def foo() -> Generator[str, None, None]:
     yield "hello"
 ```
 
 ### `contextlib.AsyncExitStack`
 
+*Async*
 ```python
 import contextlib
 
 async with contextlib.AsyncExitStack() as exit_stack:
     exit_stack.enter_context(context_manager_one())
     exit_stack.push(callback_one)
     exit_stack.callback(on_exit_one)
@@ -247,14 +272,15 @@
     await exit_stack.enter_async_context(context_manager_two())
     exit_stack.push_async_exit(on_exit_two)
     exit_stack.push_async_callback(callback_two)
 
     await exit_stack.aclose()
 ```
 
+*Sync*
 ```python
 import contextlib
 
 with contextlib.ExitStack() as exit_stack:
     exit_stack.enter_context(context_manager_one())
     exit_stack.push(callback_one)
     exit_stack.callback(on_exit_one)
@@ -266,59 +292,65 @@
     exit_stack.close()
 ```
 
 See [limitations](#limitations)
 
 ### `asyncio.TaskGroup`
 
+*Async*
 ```python
 import asyncio
 
 async with asyncio.TaskGroup() as task_group:
     task_group.create_task(something(1, 2, 3, this="that"))
 ```
 
+*Sync*
 ```python
 import concurrent.futures
 
 with concurrent.futures.ThreadPoolExecutor() as executor:
     executor.submit(something, 1, 2, 3, this="that")
 ```
 
 See [limitations](#limitations)
 
 
 ### `anyio.create_task_group`
 
+*Async*
 ```python
 import anyio
 
 async with anyio.create_task_group() as task_group:
     task_group.start_soon(something, 1, 2, 3)
 ```
 
+*Sync*
 ```python
 import concurrent.futures
 
 with concurrent.futures.ThreadPoolExecutor() as executor:
     executor.submit(something, 1, 2, 3)
 ```
 
 See [limitations](#limitations)
 
 ### `asyncio.sleep` / `anyio.sleep`
 
 Calls to `asyncio.sleep` and `anyio.sleep` will be replaced with calls to `time.sleep`:
 
+*Async*
 ```python
 import asyncio
 
 await asyncio.sleep(1)
 ```
 
+*Sync*
 ```python
 import time
 
 time.sleep(1)
 ```
 
 If the call argument is `0`, the call will be replaced entirely:
@@ -338,21 +370,23 @@
 | `typing.AsyncGenerator[int, str]` | `typing.Generator[int, str, None]` |
 
 
 ### Docstrings
 
 Simply token replacement is available in docstrings:
 
+*Async*
 ```python
 async def foo():
     """This calls ``await bar()`` and ``asyncio.sleep``"""
 ```
 
+*Sync*
 ```python
-async def foo():
+def foo():
     """This calls ``bar()`` and ``time.sleep``"""
 ```
 
 
 ## Usage
 
 ### Installation
@@ -390,29 +424,28 @@
 ```
 
 ### Configuration
 
 Unasyncd can be configured via a `pyproject.toml` file, a dedicated `.unasyncd.toml`
 file or the command line interface.
 
-#### Options
+#### File
 
-| config file key             | CLI                             | default | description                                                                        |
-|-----------------------------|---------------------------------|---------|------------------------------------------------------------------------------------|
-| `files`                     |                                 | -       | A table mapping source file names / directories to target file names / directories |
-| `exclude`                   | N/A                             | -       | An array of names to exclude from transformation                                   |
-| `per_file_exclude`          | N/A                             | -       | A table mapping files names to an array of names to exclude from transformation    |
-| `add_replacements`          | N/A                             | -       | A table of additional name replacements                                            |
-| `per_file_add_replacements` | N/A                             | -       | A table mapping file names to tables of additional replacements                    |
-| `transform_docstrings`      | `-d` / `--transform-docstrings` | false   | Enable transformation of docstrings                                                |
-| `add_editors_note`          | `--add-editors-note`            | false   | Add a note on top of the generated files                                           |
-| `remove_unuse_imports`      | `--remove-unused-imports`       | false   | Remove imports that have become unused after the transformation                    |
-| `no_cache`                  | `--no-cache`                    | false   | Disable caching                                                                    |
-| `force_regen`               | `--force-regen`                 | false   | Always regenerate files, regardless if their content has changed                   |
-| N/A                         | `-c` / `--config``              | -       | Specify an alternative configuration file                                          |
+| config file key               | type  | default | description                                                                        |
+|-------------------------------|-------|---------|------------------------------------------------------------------------------------|
+| `files`                       | table | -       | A table mapping source file names / directories to target file names / directories |
+| `exclude`                     | array | -       | An array of names to exclude from transformation                                   |
+| `per_file_exclude`            | table | -       | A table mapping files names to an array of names to exclude from transformation    |
+| `add_replacements`            | table | -       | A table of additional name replacements                                            |
+| `per_file_add_replacements`   | table | -       | A table mapping file names to tables of additional replacements                    |
+| `transform_docstrings`        | bool  | false   | Enable transformation of docstrings                                                |
+| `add_editors_note`            | bool  | false   | Add a note on top of the generated files                                           |
+| `infer_type_checking_imports` | bool  | true    | Infer if new imports should be added to an 'if TYPE_CHECKING' block                |
+| `cache`                       | bool  | true    | Cache transformation results                                                       |
+| `force_regen`                 | bool  | false   | Always regenerate files, regardless if their content has changed                   |
 
 **Example**
 
 ```toml
 [tool.unasyncd]
 files = { "async_thing.py" = "sync_thing.py", "foo.py" = "bar.py" }
 exclude = ["Something", "SomethingElse.within"]
@@ -422,14 +455,43 @@
 transform_docstrings = true
 remove_unused_imports = false
 no_cache = false
 no_cache = false
 force_regen = false
 ```
 
+#### CLI options
+
+*Feature flags corresponding to configuration values*
+
+| option                             | description                                                         |
+|------------------------------------|---------------------------------------------------------------------|
+| `--cache`                          | Cache transformation results                                        |
+| `--no-cache `                      | Don't cache transformation results                                  |
+| `--transform-docstrings`           | Enable transformation of docstrings                                 |
+| `--no-transform-docstrings`        | Inverse of `--transform-docstrings`                                 |
+| `--infer-type-checking-imports`    | Infer if new imports should be added to an 'if TYPE_CHECKING' block |
+| `--no-infer-type-checking-imports` | Inverse of `infer-type-checking-imports`                            |
+| `--add-editors-note`               | Add a note on top of each generated file                            |
+| `--no-add-editors-note`            | Inverse of `--add-editors-note`                                     |
+| `--force`                          | Always regenerate files, regardless if their content has changed    |
+| `--no-force`                       | Inverse of `--force`                                                |
+| `--check`                          | Don't write changes back to files                                   |
+| `--write`                          | Inverse of `--check`                                                |
+
+
+*Additional CLI options*
+
+| option      | description                          |
+|-------------|--------------------------------------|
+| `--config`  | Alternative configuration file       |
+| `--verbose` | Increase verbosity of console output |
+| `--quiet`   | Suppress all console output          |
+
+
 #### Exclusions
 
 It is possible to exclude specific functions classes and methods from the
 transformation. This can be achieved by adding their fully qualified name
 (relative to the transformed module) under the `exclude` key:
 
 ```toml
@@ -479,35 +541,21 @@
    `from typing import Generator`
 2. Existing imports will be updated if possible, for instance `from time import time`
    would become `from time import time, sleep` if `sleep` has been added by unasyncd
    during the transformation
 3. New imports are added before the first non-import block that's not a docstring or a
    comment
 
-By default, unasyncd will not remove imports that have become unused as a result of the
-applied transformations. This is because tracking of usages is a complex task and best
-left to tools made specifically for this job like [ruff](https://beta.ruff.rs/docs) or
-[autoflake](https://github.com/PyCQA/autoflake). It can also be a performance benefit
-of not doing this work twice, e.g. when employing one of the aforementioned tools either
-way.
-
-
-### Integration with linters and formatters
-
-Unasyncd should be run **after** tools that change the AST (e.g. isort, ruff), and
-**before** tools that apply transformations in a way that does not change the AST
-(e.g. black).
-
-The reason for this is to avoid multiple passes being required until a stable state is
-reached. Since unasyncd will only re-apply transformations to files which are no longer
-AST equivalent, running it after tools that break AST equivalence solve this issue.
-
-In practice this means all transformations aside from comments and formatting should be
-applied before unasyncd.
+Unasyncd will not remove imports that have become unused as a result of the applied
+transformations. This is because tracking of usages is a complex task and best left to
+tools made specifically for this job like [ruff](https://beta.ruff.rs/docs) or
+[autoflake](https://github.com/PyCQA/autoflake).
 
+Not doing this work twice - e.g. employing a tool to automatically remove unused
+imports alongside unasyncd - can also be a significant performance improvement.
 
 ### Limitations
 
 Transformations for `contextlib.AsyncContextManager`, `asyncio.TaskGroup` and
 `anyio.create_task_group` only work when they're being called in a `with` statement
 directly. This is due to the fact that unasyncd does not track assignments or support
 type inference. Support for these usages might be added in a future version.
```

