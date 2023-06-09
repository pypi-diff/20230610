# Comparing `tmp/click-option-group-0.5.5.tar.gz` & `tmp/click-option-group-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "click-option-group-0.5.5.tar", last modified: Wed Oct 12 12:11:38 2022, max compression
+gzip compressed data, was "click-option-group-0.5.6.tar", last modified: Fri Jun  9 22:15:42 2023, max compression
```

## Comparing `click-option-group-0.5.5.tar` & `click-option-group-0.5.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2022-10-12 12:11:38.767334 click-option-group-0.5.5/
--rw-rw-rw-   0        0        0     2327 2022-10-12 12:10:45.000000 click-option-group-0.5.5/CHANGELOG.md
--rw-rw-rw-   0        0        0     1552 2021-10-12 10:37:33.000000 click-option-group-0.5.5/LICENSE
--rw-rw-rw-   0        0        0       72 2022-10-12 12:09:21.000000 click-option-group-0.5.5/MANIFEST.in
--rw-rw-rw-   0        0        0     7754 2022-10-12 12:11:38.767334 click-option-group-0.5.5/PKG-INFO
--rw-rw-rw-   0        0        0     4090 2021-10-12 10:37:33.000000 click-option-group-0.5.5/README.md
-drwxrwxrwx   0        0        0        0 2022-10-12 12:11:38.761334 click-option-group-0.5.5/click_option_group/
--rw-rw-rw-   0        0        0      764 2021-10-12 10:37:33.000000 click-option-group-0.5.5/click_option_group/__init__.py
--rw-rw-rw-   0        0        0    14574 2022-10-12 11:46:29.000000 click-option-group-0.5.5/click_option_group/_core.py
--rw-rw-rw-   0        0        0     7428 2021-10-12 10:37:33.000000 click-option-group-0.5.5/click_option_group/_decorators.py
--rw-rw-rw-   0        0        0     1368 2021-10-12 10:37:33.000000 click-option-group-0.5.5/click_option_group/_helpers.py
--rw-rw-rw-   0        0        0       50 2022-10-12 12:09:48.000000 click-option-group-0.5.5/click_option_group/_version.py
--rw-rw-rw-   0        0        0        0 2022-10-12 11:46:29.000000 click-option-group-0.5.5/click_option_group/py.typed
-drwxrwxrwx   0        0        0        0 2022-10-12 12:11:38.765334 click-option-group-0.5.5/click_option_group.egg-info/
--rw-rw-rw-   0        0        0     7754 2022-10-12 12:11:38.000000 click-option-group-0.5.5/click_option_group.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      504 2022-10-12 12:11:38.000000 click-option-group-0.5.5/click_option_group.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-10-12 12:11:38.000000 click-option-group-0.5.5/click_option_group.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      132 2022-10-12 12:11:38.000000 click-option-group-0.5.5/click_option_group.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2022-10-12 12:11:38.000000 click-option-group-0.5.5/click_option_group.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       80 2022-10-12 12:11:38.768334 click-option-group-0.5.5/setup.cfg
--rw-rw-rw-   0        0        0     2350 2022-10-12 12:09:21.000000 click-option-group-0.5.5/setup.py
-drwxrwxrwx   0        0        0        0 2022-10-12 12:11:38.766333 click-option-group-0.5.5/tests/
--rw-rw-rw-   0        0        0      159 2021-10-12 10:37:33.000000 click-option-group-0.5.5/tests/conftest.py
--rw-rw-rw-   0        0        0    24783 2021-10-12 10:37:33.000000 click-option-group-0.5.5/tests/test_click_option_group.py
+drwxrwxrwx   0        0        0        0 2023-06-09 22:15:42.220123 click-option-group-0.5.6/
+-rw-rw-rw-   0        0        0     2614 2023-06-09 22:10:10.000000 click-option-group-0.5.6/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1552 2021-10-12 10:37:33.000000 click-option-group-0.5.6/LICENSE
+-rw-rw-rw-   0        0        0       72 2022-10-12 12:09:21.000000 click-option-group-0.5.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     8093 2023-06-09 22:15:42.220123 click-option-group-0.5.6/PKG-INFO
+-rw-rw-rw-   0        0        0     4090 2021-10-12 10:37:33.000000 click-option-group-0.5.6/README.md
+drwxrwxrwx   0        0        0        0 2023-06-09 22:15:42.214122 click-option-group-0.5.6/click_option_group/
+-rw-rw-rw-   0        0        0      764 2021-10-12 10:37:33.000000 click-option-group-0.5.6/click_option_group/__init__.py
+-rw-rw-rw-   0        0        0    14550 2023-06-09 22:00:09.000000 click-option-group-0.5.6/click_option_group/_core.py
+-rw-rw-rw-   0        0        0     8376 2023-06-09 21:22:06.000000 click-option-group-0.5.6/click_option_group/_decorators.py
+-rw-rw-rw-   0        0        0     1421 2023-06-09 21:22:06.000000 click-option-group-0.5.6/click_option_group/_helpers.py
+-rw-rw-rw-   0        0        0       50 2023-06-09 22:10:10.000000 click-option-group-0.5.6/click_option_group/_version.py
+-rw-rw-rw-   0        0        0        0 2022-10-12 11:46:29.000000 click-option-group-0.5.6/click_option_group/py.typed
+drwxrwxrwx   0        0        0        0 2023-06-09 22:15:42.218123 click-option-group-0.5.6/click_option_group.egg-info/
+-rw-rw-rw-   0        0        0     8093 2023-06-09 22:15:42.000000 click-option-group-0.5.6/click_option_group.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      504 2023-06-09 22:15:42.000000 click-option-group-0.5.6/click_option_group.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 22:15:42.000000 click-option-group-0.5.6/click_option_group.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      122 2023-06-09 22:15:42.000000 click-option-group-0.5.6/click_option_group.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-06-09 22:15:42.000000 click-option-group-0.5.6/click_option_group.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       80 2023-06-09 22:15:42.221122 click-option-group-0.5.6/setup.cfg
+-rw-rw-rw-   0        0        0     2389 2023-06-09 22:01:34.000000 click-option-group-0.5.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 22:15:42.219123 click-option-group-0.5.6/tests/
+-rw-rw-rw-   0        0        0      159 2021-10-12 10:37:33.000000 click-option-group-0.5.6/tests/conftest.py
+-rw-rw-rw-   0        0        0    25562 2023-06-09 22:00:09.000000 click-option-group-0.5.6/tests/test_click_option_group.py
```

### Comparing `click-option-group-0.5.5/CHANGELOG.md` & `click-option-group-0.5.6/CHANGELOG.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,16 @@
 # Changelog
 
+## v0.5.6 (09.06.2023)
+
+* Add `optgroup.help_option` decorator to add help option to the group (PR [#50](https://github.com/click-contrib/click-option-group/pull/50))
+* Use GitHub Actions instead of Travis CI for CI
+* Delete tox runner
+* Add Python 3.11 to the setup classifiers
+
 ## v0.5.5 (12.10.2022)
 
 * Add `tests/` directory to tarball
 * Add `tests_cov` extra dependencies for testing with coverage
 
 ## v0.5.4 (12.10.2022)
```

### Comparing `click-option-group-0.5.5/LICENSE` & `click-option-group-0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `click-option-group-0.5.5/PKG-INFO` & `click-option-group-0.5.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: click-option-group
-Version: 0.5.5
+Version: 0.5.6
 Summary: Option groups missing in Click
 Home-page: https://github.com/click-contrib/click-option-group
 Author: Eugene Prilepin
 Author-email: esp.home@gmail.com
 License: BSD-3-Clause
 Project-URL: Code, https://github.com/click-contrib/click-option-group
 Project-URL: Issue tracker, https://github.com/click-contrib/click-option-group/issues
@@ -19,14 +19,15 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6,<4
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 Provides-Extra: tests
 Provides-Extra: tests_cov
 License-File: LICENSE
 
@@ -124,14 +125,21 @@
 
 ## Documentation
 
 https://click-option-group.readthedocs.io
 
 # Changelog
 
+## v0.5.6 (09.06.2023)
+
+* Add `optgroup.help_option` decorator to add help option to the group (PR [#50](https://github.com/click-contrib/click-option-group/pull/50))
+* Use GitHub Actions instead of Travis CI for CI
+* Delete tox runner
+* Add Python 3.11 to the setup classifiers
+
 ## v0.5.5 (12.10.2022)
 
 * Add `tests/` directory to tarball
 * Add `tests_cov` extra dependencies for testing with coverage
 
 ## v0.5.4 (12.10.2022)
```

### Comparing `click-option-group-0.5.5/README.md` & `click-option-group-0.5.6/README.md`

 * *Files identical despite different names*

### Comparing `click-option-group-0.5.5/click_option_group/__init__.py` & `click-option-group-0.5.6/click_option_group/__init__.py`

 * *Files identical despite different names*

### Comparing `click-option-group-0.5.5/click_option_group/_core.py` & `click-option-group-0.5.6/click_option_group/_core.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 
 import collections
 import inspect
 import weakref
-from collections.abc import Callable
 from typing import (
     Any,
+    Callable,
     Dict,
     List,
     Mapping,
     Optional,
     Sequence,
     Set,
     Tuple,
@@ -169,15 +169,15 @@
 
         if not name and not help_:
             return None
 
         return name, help_
 
     def option(self, *param_decls: str, **attrs: Any) -> Callable:
-        """Decorator attaches an grouped option to the command
+        """Decorator attaches a grouped option to the command
 
         The decorator is used for adding options to the group and to the Click-command
         """
 
         def decorator(func: FC) -> FC:
             option_attrs = attrs.copy()
             option_attrs.setdefault('cls', GroupedOption)
```

### Comparing `click-option-group-0.5.5/click_option_group/_decorators.py` & `click-option-group-0.5.6/click_option_group/_decorators.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 # -*- coding: utf-8 -*-
 
-from typing import Optional, NamedTuple, List, Tuple, Dict, Any, Type
+from typing import (Callable, Optional, NamedTuple, List,
+                    Tuple, Dict, Any, Type, TypeVar)
 
-import collections.abc as abc
 import collections
 import warnings
 import inspect
 
 import click
 
 from ._core import OptionGroup
 from ._helpers import (
     get_callback_and_params,
     raise_mixing_decorators_error,
 )
 
+T = TypeVar('T')
+F = TypeVar('F', bound=Callable)
+
+Decorator = Callable[[F], F]
+
 
 class OptionStackItem(NamedTuple):
     param_decls: Tuple[str, ...]
     attrs: Dict[str, Any]
     param_count: int
 
 
@@ -58,16 +63,16 @@
         @optgroup.option('--bar')
         @optgroup.group('Group 2', help='option group 2')
         @optgroup.option('--spam')
         ...
     """
 
     def __init__(self) -> None:
-        self._decorating_state: Dict[abc.Callable, List[OptionStackItem]] = collections.defaultdict(list)
-        self._not_attached_options: Dict[abc.Callable, List[click.Option]] = collections.defaultdict(list)
+        self._decorating_state: Dict[Callable, List[OptionStackItem]] = collections.defaultdict(list)
+        self._not_attached_options: Dict[Callable, List[click.Option]] = collections.defaultdict(list)
         self._outer_frame_index = 1
 
     def __call__(self,
                  name: Optional[str] = None, *,
                  help: Optional[str] = None,
                  cls: Optional[Type[OptionGroup]] = None, **attrs):
         """Creates a new group and collects its options
@@ -136,15 +141,15 @@
             for item in option_stack:
                 func = option_group.option(*item.param_decls, **item.attrs)(func)
 
             return func
 
         return decorator
 
-    def option(self, *param_decls, **attrs):
+    def option(self, *param_decls, **attrs) -> Decorator:
         """The decorator adds a new option to the group
 
         The decorator is lazy. It adds option decls and attrs.
         All options will be registered by `group` decorator.
 
         :param param_decls: option declaration tuple
         :param attrs: additional option attributes and parameters
@@ -160,26 +165,49 @@
             self._add_not_attached_option(func, param_decls)
             option_stack.append(OptionStackItem(param_decls, attrs, len(params)))
 
             return func
 
         return decorator
 
-    def _add_not_attached_option(self, func, param_decls):
+    def help_option(self, *param_decls, **attrs) -> Decorator:
+        """This decorator adds a help option to the group, which prints
+        the command's help text and exits.
+        """
+        if not param_decls:
+            param_decls = ('--help',)
+
+        attrs.setdefault('is_flag', True)
+        attrs.setdefault('is_eager', True)
+        attrs.setdefault('expose_value', False)
+        attrs.setdefault('help', 'Show this message and exit.')
+
+        if 'callback' not in attrs:
+            def callback(ctx, _, value):
+                if not value or ctx.resilient_parsing:
+                    return
+                click.echo(ctx.get_help(), color=ctx.color)
+                ctx.exit()
+
+            attrs['callback'] = callback
+
+        return self.option(*param_decls, **attrs)
+
+    def _add_not_attached_option(self, func, param_decls) -> None:
         click.option(
             *param_decls,
             all_not_attached_options=self._not_attached_options,
             cls=_NotAttachedOption
         )(func)
 
         callback, params = get_callback_and_params(func)
         self._not_attached_options[callback].append(params[-1])
 
     @staticmethod
-    def _filter_not_attached(options):
+    def _filter_not_attached(options: List[T]) -> List[T]:
         return [opt for opt in options if not isinstance(opt, _NotAttachedOption)]
 
     @staticmethod
     def _check_mixing_decorators(callback, options_stack, params):
         if options_stack:
             last_state = options_stack[-1]
```

### Comparing `click-option-group-0.5.5/click_option_group/_helpers.py` & `click-option-group-0.5.6/click_option_group/_helpers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 # -*- coding: utf-8 -*-
 
-from typing import List, Tuple
+from typing import Callable, Tuple, List, TypeVar, NoReturn
 
-import collections.abc as abc
 import random
 import string
 
 import click
 
 
+F = TypeVar('F', bound=Callable)
+
 FAKE_OPT_NAME_LEN = 30
 
 
-def get_callback_and_params(func) -> Tuple[abc.Callable, List[click.Option]]:
+def get_callback_and_params(func) -> Tuple[Callable, List[click.Option]]:
     """Returns callback function and its parameters list
 
     :param func: decorated function or click Command
     :return: (callback, params)
     """
     if isinstance(func, click.Command):
         params = func.params
@@ -24,23 +25,23 @@
     else:
         params = getattr(func, '__click_params__', [])
 
     func = resolve_wrappers(func)
     return func, params
 
 
-def get_fake_option_name(name_len: int = FAKE_OPT_NAME_LEN, prefix: str = 'fake'):
+def get_fake_option_name(name_len: int = FAKE_OPT_NAME_LEN, prefix: str = 'fake') -> str:
     return f'--{prefix}-' + ''.join(random.choices(string.ascii_lowercase, k=name_len))
 
 
-def raise_mixing_decorators_error(wrong_option: click.Option, callback: abc.Callable):
+def raise_mixing_decorators_error(wrong_option: click.Option, callback: Callable) -> NoReturn:
     error_hint = wrong_option.opts or [wrong_option.name]
 
     raise TypeError((
         "Grouped options must not be mixed with regular parameters while adding by decorator. "
         f"Check decorator position for {error_hint} option in '{callback.__name__}'."
     ))
 
 
-def resolve_wrappers(f):
+def resolve_wrappers(f: F) -> F:
     """Get the underlying function behind any level of function wrappers."""
     return resolve_wrappers(f.__wrapped__) if hasattr(f, "__wrapped__") else f
```

### Comparing `click-option-group-0.5.5/click_option_group.egg-info/PKG-INFO` & `click-option-group-0.5.6/click_option_group.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: click-option-group
-Version: 0.5.5
+Version: 0.5.6
 Summary: Option groups missing in Click
 Home-page: https://github.com/click-contrib/click-option-group
 Author: Eugene Prilepin
 Author-email: esp.home@gmail.com
 License: BSD-3-Clause
 Project-URL: Code, https://github.com/click-contrib/click-option-group
 Project-URL: Issue tracker, https://github.com/click-contrib/click-option-group/issues
@@ -19,14 +19,15 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6,<4
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 Provides-Extra: tests
 Provides-Extra: tests_cov
 License-File: LICENSE
 
@@ -124,14 +125,21 @@
 
 ## Documentation
 
 https://click-option-group.readthedocs.io
 
 # Changelog
 
+## v0.5.6 (09.06.2023)
+
+* Add `optgroup.help_option` decorator to add help option to the group (PR [#50](https://github.com/click-contrib/click-option-group/pull/50))
+* Use GitHub Actions instead of Travis CI for CI
+* Delete tox runner
+* Add Python 3.11 to the setup classifiers
+
 ## v0.5.5 (12.10.2022)
 
 * Add `tests/` directory to tarball
 * Add `tests_cov` extra dependencies for testing with coverage
 
 ## v0.5.4 (12.10.2022)
```

### Comparing `click-option-group-0.5.5/setup.py` & `click-option-group-0.5.6/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,17 +33,17 @@
     },
     include_package_data=True,
     python_requires='>=3.6,<4',
     install_requires=[
         'Click>=7.0,<9',
     ],
     extras_require={
-        'docs': ['sphinx>=3.0, <6', 'Pallets-Sphinx-Themes', 'm2r2'],
+        'docs': ['sphinx', 'Pallets-Sphinx-Themes', 'm2r2'],
         'tests': ['pytest'],
-        'tests_cov': ['pytest', 'pytest-cov', 'coverage <6', 'coveralls'],
+        'tests_cov': ['pytest', 'pytest-cov', 'coverage', 'coveralls'],
     },
     url='https://github.com/click-contrib/click-option-group',
     project_urls={
         "Code": 'https://github.com/click-contrib/click-option-group',
         "Issue tracker": 'https://github.com/click-contrib/click-option-group/issues',
         "Documentation": 'https://click-option-group.readthedocs.io',
     },
@@ -64,9 +64,10 @@
         'Programming Language :: Python :: 3 :: Only',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
     ],
 )
```

### Comparing `click-option-group-0.5.5/tests/test_click_option_group.py` & `click-option-group-0.5.6/tests/test_click_option_group.py`

 * *Files 1% similar despite different names*

```diff
@@ -729,14 +729,38 @@
     result = runner.invoke(cli, ['--help'])
     assert not result.exception
     assert "Group 1" in result.output
     assert "foo" in result.output
     assert "bar" not in result.output
 
 
+@pytest.mark.parametrize('param_decls, options, output', [
+    ((), ['--help'], '--help'),
+    (('-h', '--help'), ['-h'], '-h, --help'),
+    (('-h', '--help'), ['--help'], '-h, --help'),
+])
+def test_help_option(runner, param_decls, options, output):
+    @click.command()
+    @optgroup('Help Options')
+    @optgroup.help_option(*param_decls)
+    def cli() -> None:
+        click.echo('Running command.')
+
+    result = runner.invoke(cli)
+    assert not result.exception
+    assert 'Running command.' in result.output
+    assert 'Usage:' not in result.output
+
+    result = runner.invoke(cli, options)
+    assert not result.exception
+    assert 'Running command.' not in result.output
+    assert 'Usage:' in result.output
+    assert output in result.output
+
+
 def test_wrapped_functions(runner):
     def make_z():
         """A unified option interface for making a `z`."""
 
         def decorator(f):
             @optgroup.group("Group xyz")
             @optgroup.option("-x", type=int)
```

