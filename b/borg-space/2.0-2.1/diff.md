# Comparing `tmp/borg_space-2.0.tar.gz` & `tmp/borg_space-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "borg_space-2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "borg_space-2.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `borg_space-2.0.tar` & `borg_space-2.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    35149 2022-10-22 21:26:19.370225 borg_space-2.0/LICENSE
--rw-r--r--   0        0        0     8785 2023-05-16 05:57:30.537517 borg_space-2.0/README.rst
--rw-r--r--   0        0        0        0 2023-05-05 05:24:18.834041 borg_space-2.0/borg_space/__init__.py
--rw-r--r--   0        0        0     6943 2023-05-16 04:24:30.512097 borg_space-2.0/borg_space/config.py
--rw-r--r--   0        0        0    10680 2023-05-16 05:57:30.536517 borg_space-2.0/borg_space/main.py
--rw-r--r--   0        0        0     2978 2023-05-16 04:26:51.372451 borg_space-2.0/borg_space/trees.py
--rw-r--r--   0        0        0     1183 2023-05-16 05:57:30.535517 borg_space-2.0/pyproject.toml
--rw-r--r--   0        0        0     9842 1970-01-01 00:00:00.000000 borg_space-2.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2022-10-22 21:26:19.370225 borg_space-2.1/LICENSE
+-rw-r--r--   0        0        0    11958 2023-06-09 22:55:49.182337 borg_space-2.1/README.rst
+-rw-r--r--   0        0        0        0 2023-05-05 05:24:18.834041 borg_space-2.1/borg_space/__init__.py
+-rw-r--r--   0        0        0     8694 2023-06-09 01:54:28.616901 borg_space-2.1/borg_space/config.py
+-rw-r--r--   0        0        0    10733 2023-06-09 22:55:49.180337 borg_space-2.1/borg_space/main.py
+-rw-r--r--   0        0        0     3089 2023-06-07 00:28:49.138158 borg_space-2.1/borg_space/trees.py
+-rw-r--r--   0        0        0     1183 2023-06-09 22:55:49.179337 borg_space-2.1/pyproject.toml
+-rw-r--r--   0        0        0    13015 1970-01-01 00:00:00.000000 borg_space-2.1/PKG-INFO
```

### Comparing `borg_space-2.0/LICENSE` & `borg_space-2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `borg_space-2.0/README.rst` & `borg_space-2.1/README.rst`

 * *Files 19% similar despite different names*

```diff
@@ -1,202 +1,280 @@
-Borg-Space — Report and track the size of your Borg repositories
-================================================================
+Borg-Space — Report and track the size of your Emborg repositories
+==================================================================
 
 .. image:: https://pepy.tech/badge/borg-space/month
     :target: https://pepy.tech/project/borg-space
 
 .. image:: https://img.shields.io/pypi/v/borg-space.svg
     :target: https://pypi.python.org/pypi/borg-space
 
 .. image:: https://img.shields.io/pypi/pyversions/borg-space.svg
     :target: https://pypi.python.org/pypi/borg-space/
 
 :Author: Ken Kundert
-:Version: 2.0
-:Released: 2023-05-15
+:Version: 2.1
+:Released: 2023-06-09
 
 *Borg-Space* is an accessory for Emborg_.  It reports on the space consumed by 
-your *BorgBackup* repositories.  You can get this information using the ``emborg 
-info`` command, but there are several reasons to prefer *Borg-Space*.
+your *BorgBackup* repositories.  You can get this information using the
+``emborg info`` command, but there are several reasons to prefer *Borg-Space*.
 
-#. *Borg-Space* reports on many repositories at once.
+#. *Borg-Space* is capable of reporting on many repositories at once.
 #. The *Emborg* *info* command gives a great deal of information,
    whereas *Borg-Space* only reports the space consumed by the repository,
    so is much more compact.
 #. The report is user customizable.
 #. *Borg-Space* can record the size of your repositories each time it is run
    so you can track the space requirements over time.
 #. Finally, *Borg-Space* can graph the recorded values.
 
 To show the size of one or more repositories, simply run::
 
     # borg-space home
     home: 12.81 GB
 
-You can specify any number of repositories, and they can be composite
-configs::
+You can specify any number of repositories, and they can be composites.  In the 
+following example, *home* is an alias that expands to *borgbase* and *rsync*::
 
     > borg-space home cache
     borgbase: 2.44 GB
     cache: 801 MB
     rsync: 2.81 GB
 
 You can specify repositories that are owned by others or that are on remote 
 machines.  In this case you will need permission to read the *Emborg* data 
 directory for the repository. Specifically, 
 ❬host❭:~❬user❭/.local/share/emborg/❬config❭.latest.nt must be accessible.
+❬config❭ is the name of the *Emborg* configuration to be reported on, ❬host❭ is 
+the name of the host on which the *Emborg create* command was run, and ❬user❭ is 
+the name of the user that ran the command.
+
 To specify these repositories, a special naming scheme is used::
 
     ❬config❭@❬host❭~❬user❭
 
-Thus the *Emborg* configuration named *primary* owned by *root* on the host with 
-the SSH name *neptune* is accessed with::
+This is referred to as the full repository specification, or repository spec.  
+Both ``@❬host❭`` and ``~❬user❭`` are optional, ❬host❭ is not needed when 
+referring to the local host and ❬user❭ is not needed when referring to the 
+current user.  Thus the *Emborg* configuration named *primary* owned by *root* 
+on the host with the SSH name *neptune* is accessed with::
 
     # borg-space primary@neptune~root
     primary@neptune~root: 57.74 GB
 
 
 Usage
 -----
 
 *Borg-Space* supports the following command line arguments::
 
     Usage:
-        borg-space [--quiet] [--style <style>] [--record] [<repo>...]
-        borg-space [--graph] [--svg <file>] [--log-y] [<repo>...]
+        borg-space [--quiet] [--style <style>] [--record] [<spec>...]
+        borg-space [--graph] [--svg <file>] [--log-y] [--record] [<spec>...]
 
     Options:
         -r, --record                 save the result
         -q, --quiet                  do not output the size message
         -s <style>, --style <style>  the report style
-                                     choose from compact, normal, tree, nt, json
+                                     choose from compact, table, tree, nt, json
         -g, --graph                  graph the previously recorded sizes over time
         -l, --log-y                  use a logarithmic Y-axis when graphing
         -S <file>, --svg <file>      produce plot as SVG file rather than display it
 
+Repository specs take the form ``❬name❭`` or ``❬config❭[@❬host❭][~❬user❭]``.  
+Items in brackets are optional and ❬name❭ is the name given for a repository the
+repositories setting.
+
+The available styles are *compact*, *table*, *tree*, *nt* or *nestedtext*, or 
+*json*.  If you specify something other than the these, what you give is taken 
+to be a *compact format* specification.
+
+Results are saved to ~/.local/share/borg-space/<full_spec>.nt.
+Settings are held in ~/.config/borg-space/settings.nt.
 
 
 Settings
 --------
 
 You can create a NestedText_ settings file to specify default behaviors and 
 define composite repositories.  For example::
 
     default repository: home
     report style: tree
-    compact format: {repo}: {size:{fmt}}.  Last back up: {last_create:ddd, MMM DD}.  Last squeeze: {last_squeeze:ddd, MMM DD}.
-    normal format: {host:<8} {user:<5} {config:<9} {size:<8.2b} {last_create:ddd, MMM DD}
-    normal header: HOST     USER  CONFIG    SIZE     LAST BACK UP
+    compact format: {name}: {size:{fmt}}.  Last back up: {last_create:ddd, MMM DD}.  Last squeeze: {last_squeeze:ddd, MMM DD}.
+    table format: {host:<8} {user:<5} {config:<9} {size:<8.2b} {last_create:ddd, MMM DD}
+    table header: HOST     USER  CONFIG    SIZE     LAST BACK UP
     report fields: size last_create last_squeeze
     tree report fields: size
     date format: D MMMM YYYY
     size format: .b
-    nestedtext size format: .3b
 
     repositories:
+        # define some convenient aliases
+        root: root~root
+        dev: root@dev~root
+        mail: root@mail~root
+        files: root@files~root
+        bastion: root@bastion~root
+        media: root@media~root
+        web: root@web~root
+        cluster: home@cluster
+
+        # define useful combinations
         home:
-            children: rsync borgbase
+            children: rsync borgbase cluster
         servers:
             children:
-                - root@dev~root
-                - root@mail~root
-                - root@files~root
-                - root@bastion~root
-                - root@media~root
-                - root@web~root
+                - dev
+                - mail
+                - files
+                - bastion
+                - media
+                - web
         all:
-            children: home servers
+            children: home servers root
 
 default repository:
-    The name of the repository to be used if one is not given on the command 
-    line.
+    The name of the repository to be used if none are given on the command line.
 
 report style:
     The report style to be used if none is specified on the command line.  
-    Choose from *compact*, *normal*, *tree*, *nestedtext* or *nt*, or *json*.
+    Choose from *compact*, *table*, *tree*, *nestedtext* or *nt*, or *json*.
 
 compact format:
     The format to be used for the line when the requested report style is 
-    *compact*.
-    The *repo*, *size*, *fmt*, *last_create*, *last_prune*, *last_compact* and 
-    *last_squeeze*  fields will be replaced by the corresponding values.
-    *last_squeeze* is simply the later of *last_prune* and *last_compact*.  
-    *size* is a QuantiPhy_ *Quantity* and the *last_* fields are all Arrow_ 
-    objects.  The remaining field values are strings.
+    *compact*.  The *name*, *spec*, *full_spec*, *config*, *host*, *user*, 
+    *size*, *fmt*, *last_create*, *last_prune*, *last_compact* and 
+    *last_squeeze*  fields are replaced by the corresponding values.  *name* is 
+    the name given the repository in the *repositories* setting.  *spec* is the 
+    specification given as specified, and *full_spec* is the full specification 
+    (any pieces missing from *spec* are filled in).  If a name is not available, 
+    *name* becomes the same as *spec*.  *last_squeeze* is simply the later of 
+    *last_prune* and *last_compact*.  *size* is a QuantiPhy_ *Quantity* and the 
+    *last_* fields are all Arrow_ objects (see the example in the next section 
+    for examples on how to specify formatting on *QuantiPhy* and *Arrow* 
+    objects).  The remaining field values are strings.
 
     The default is::
 
-        {repo}: {size:{fmt}}
+        {name}: {size:{fmt}}
 
-normal format:
+table format:
     The format to be used for the line when the requested report style is 
-    *normal*.  The *host*, *user*, *config*, *size*, *fmt*, *last_create*, 
-    *last_prune*, *last_compact* and *last_squeeze*  fields will be replaced by 
-    the corresponding values.  *last_squeeze* is simply the later of 
-    *last_prune* and *last_compact*.  *size* is a QuantiPhy_ *Quantity* and the 
-    *last_* fields are all Arrow_ objects.  The remaining field values are 
+    *table*.  The *name*, *spec*, *host*, *user*, *config*, *size*, *fmt*, 
+    *last_create*, *last_prune*, *last_compact* and *last_squeeze*  fields will 
+    be replaced by the corresponding values.  *last_squeeze* is simply the later 
+    of *last_prune* and *last_compact*.  *size* is a QuantiPhy_ *Quantity* and 
+    the *last_* fields are all Arrow_ objects.  The remaining field values are 
     strings.
 
     The default is::
 
         {host:8} {user:8} {config:8} {size:<8.2b}  {last_create:ddd, MMM DD}
 
-normal header:
-    The header to be printed just before the normal report.  It is used to give 
+table header:
+    The header to be printed just before the table report.  It is used to give 
     column headers.  Leave empty to suppress the header.
 
     The default is::
 
         HOST     USER     CONFIG   SIZE      LAST BACK UP
 
 report fields:
     The fields to include in *tree*, *nestedtext* and *json* style reports by 
     default.  Default is *size*, *last_create*, and *last_squeeze*.
 
 tree report fields:
-    The fields to include in *tree* style reports.
-    default.  If not given it defaults to the value of  *report fields*.
+    The fields to include in *tree* style reports.  If not given it defaults to 
+    the value of *report fields*.
 
 nestedtext report fields:
-    The fields to include in *nestedtext* style reports.
-    default.  If not given it defaults to the value of *report fields*.
+    The fields to include in *nestedtext* style reports.  If not given it 
+    defaults to the value of *report fields*.
 
 json report fields:
-    The fields to include in *json* style reports.
-    default.  If not given it defaults to the value of  *report fields*.
+    The fields to include in *json* style reports.  If not given it defaults to 
+    all available size and date fields.
 
 size format:
     The format to be used when giving the size of the repository.  This is 
     a QuantiPhy_ format string.  In the example, ``.2b`` means that a binary 
     format with two extra digits is used (one digit is required. so ``.2b`` 
-    prints with three digits of precision.  If not give, it defaults to ``.2b``.
-
-nestedtext size format:
-    The format to be used for the size of the repository when the requested 
-    report style is jnestedtext*.  This is a QuantiPhy_ format string.  If not 
-    given, it defaults to *size format*.
+    prints with three digits of precision.  If not given, it defaults to 
+    ``.2b``.
 
 date format:
     The Arrow_ format to be used for the date when the requested report style is 
     *tree* or *nestedtext*.  If not given, it defaults to ``D MMMM YYYY``.
 
 repositories:
-    Predefines available repositories.  This generally used to define composite 
-    repositories.  In this way, one name can be used for many repositories.
+    Defines repository aliases and composite repositories.  Given as 
+    a collection of name:value pairs.  The value may contain zero or more 
+    repository specifications.  The specifications may be a strings or 
+    dictionaries.  The following forms are accepted::
+
+        repositiories:
+            home:
+                # home becomes an alias for home on localhost for current user
+
+        repositiories:
+            home: home-primary
+                # home becomes an alias for home-primary on localhost for current user
+
+        repositiories:
+            home: home@host~user
+                # home becomes an alias for home@host~user
+
+        repositiories:
+            home:
+                # home becomes an alias for home@host~user
+                config: home
+                host: host
+                user: user
+
+        repositiories:
+            all: home@host~user work@host~user
+                # all contains home@host~user and work@host~user
+
+        repositiories:
+            all:
+                # all contains home@host~user and work@host~user
+                - home@host~user
+                - work@host~user
+
+        repositiories:
+            all:
+                # all contains home@host~user and work@host~user
+                -
+                    config: home
+                    host: host
+                    user: user
+                -
+                    config: work
+                    host: host
+                    user: user
+
+        repositiories:
+            home: home@host~user
+                # home becomes an alias for home@host~user
+            work: work@host~user
+                # work becomes an alias for work@host~user
+            all: home work
+                # all contains home and work
 
 
 Graphing
 --------
 
 To graph the size of a repository over time you must first routinely record its 
 size.  You can record the sizes with::
 
     > borg-space -r home
 
-The sizes are added to the file ``~/.local/share/borg-space/❬repo❭.nt``.
+The sizes are added to the file ``~/.local/share/borg-space/❬full_spec❭.nt``.
 
 Typically you do not manually run *Borg-Space* to record the sizes of your
 repositories.  Instead, you can record sizes automatically in two different
 ways.  In the first, you simply use crontab to automatically record the sizes at
 fixed times::
 
     00 12 * * *  borg-space -q -r home
@@ -228,15 +306,15 @@
 
     > borg-space -l all
 
 
 Installation
 ------------
 
-*Borg-Space* requires *Emborg* version 1.36 or newer.
+*Borg-Space* requires *Emborg* version 1.37 or newer.
 
 Install with::
 
     > pip3 install borg-space
 
 
 .. _emborg: https://emborg.readthedocs.io
```

### Comparing `borg_space-2.0/borg_space/config.py` & `borg_space-2.1/borg_space/config.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,176 +1,272 @@
+# Process settings file
+
+# IMPORTS {{{1
 from appdirs import user_config_dir
 from inform import (
-    Error, error, fatal, full_stop, is_str, is_mapping, os_error, terminate
+    Error, conjoin, error, fatal, full_stop,
+    is_str, is_mapping, is_collection, plural, os_error, terminate
 )
 from quantiphy import Quantity
-from voluptuous import Schema, Required, Invalid, MultipleInvalid
-import nestedtext as nt
+from shlib import to_path, Run, set_prefs
+from voluptuous import Schema, Invalid, MultipleInvalid
 import arrow
 import getpass
-from shlib import to_path, Run, set_prefs
-set_prefs(use_inform=True)
+import nestedtext as nt
+import os
+import pwd
+import socket
+
+
+# TESTING MODS {{{1
+# this code overrides the home directory (only used for testing)
+new_home = os.environ.get('_BORG_SPACE__OVERRIDE_HOME_FOR_TESTING_')
+if new_home:  # pragma: no cover
+    true_home = os.environ['HOME'].rstrip('/') + '/'
+    unaltered_to_path = to_path
+    def to_path(arg):
+        full_path = unaltered_to_path(arg).resolve()
+        as_str = str(full_path)
+        if as_str.startswith(true_home):
+            full_path = unaltered_to_path(new_home, as_str[len(true_home):])
+        return full_path
 
+# GLOBALS {{{1
+set_prefs(use_inform=True)
 settings_file = to_path(user_config_dir('borg-space')) / 'settings.nt'
-
 voluptuous_error_msg_mappings = {
     "extra keys not allowed": ("unknown key", "key"),
-    "expected a dictionary": ("expected key-value pair", "value"),
+    "expected a dictionary": ("expected key:value pair", "value"),
 }
+hostname = socket.gethostname().split('.')[0]
+    # version of the hostname (the hostname without any domain name)
+username = pwd.getpwuid(os.getuid()).pw_name
 
+
+# REPOSITORY {{{1
+# Repository class {{{2
 class Repository:
-    def __init__(self, config=None, host=None, user=None):
-        self.config = config
-        self.host = host
-        self.user = user
+    def __init__(self, spec, name=None):
+        prefix, _, user = spec.partition('~')
+        config, _, host = prefix.partition('@')
+        if not config:
+            raise Error("spec is missing Emborg config name.", culprit=spec)
+        if not name:
+            name = spec
+
+        self.spec = spec
+        self.name = name
+        self.config = a_name(config)
+        self.host = a_name(host) or hostname
+        self.user = a_name(user) or username
         self.latest = None
 
     def __str__(self):
-        name = self.__class__.__name__
-        args = ', '.join(f'{k}={v}' for k, v in self.__dict__.items() if v)
-        return f"{name}({args})"
+        return f"{self.config}@{self.host}~{self.user}"
+
+    def __repr__(self):
+        return f'{self.__class__.__name__}("{str(self)}")'
 
-    __repr__ = __str__
+    def __getitem__(self, key):
+        if self.latest and key in self.latest:
+            return self.latest[key]
+        return self.__dict__[key]
+
+    def get(self, key, default=None):
+        try:
+            return self[key]
+        except KeyError:
+            return default
+
+    def as_dict(self):
+        info = dict(
+            name = self.name,
+            spec = self.spec,
+            config = self.config,
+            host = self.host,
+            user = self.user,
+            full_spec = str(self)
+        )
+        info.update(self.latest)
+        return info
 
-    def get_path(self, key=None):
+    def get_path(self):
         user = self.user if self.user else getpass.getuser()
-        config = self.config if self.config else key
+        config = self.config
+        assert config
         path = f"~{user}/.local/share/emborg/{config}.latest.nt"
         return (self.host, path)
 
-    def get_name(self, key=None):
-        name = self.config if self.config else key
-        if self.host:
-            name += '@' + self.host
-        if self.user:
-            name += '~' + self.user
-        return name
-
-    def get_repo(self):
+    def get_latest(self):
         if self.latest:
             return self.latest
-        path = self.get_path(None)[1]
-        if self.host:
-            cmd = ['ssh', self.host, f"cat {path}"]
+        host, path = self.get_path()
+        if host != hostname:
+            cmd = ['ssh', host, f"cat {path}"]
             ssh = Run(cmd, modes='sOEW')
             content = ssh.stdout
         else:
             try:
                 content = to_path(path).read_text()
             except FileNotFoundError:
-                raise Error('unknown configuration.', culprit=self.get_name(None))
+                raise Error('unknown repository.', culprit=str(self))
         raw_data = nt.loads(content)
         self.latest = data = {}
         if 'repository size' in raw_data:
             data['size'] = Quantity(raw_data['repository size'], 'B')
         if 'create last run' in raw_data:
             data['last_create'] = arrow.get(raw_data['create last run'])
         if 'prune last run' in raw_data:
             data['last_prune'] = arrow.get(raw_data['prune last run'])
         if 'compact last run' in raw_data:
             data['last_compact'] = arrow.get(raw_data['compact last run'])
         if 'last_prune' in data and 'last_compact' in data:
             data['last_squeeze'] = max(data['last_prune'], data['last_compact'])
         return data
 
+# get_repos() {{{2
+def get_repos(spec):
+    if not spec:
+        spec = settings.get('default_repository')
+    if not spec:
+        raise Error('there is no default repository.')
+
+    try:
+        children = repositories[spec]
+    except (TypeError, KeyError):
+        # not found in repositories specified in settings file.
+        # see if it exists on local machine
+        children = [Repository(spec)]
+
+    results = {}
+    for child in children:
+        host, path = child.get_path()
+        name = str(child)
+        try:
+            child.get_latest()
+            results[name] = child
+        except Error as e:
+            e.report(culprit=name)
+        except OSError as e:
+            error(os_error(e), culprit=name)
+    return results
+
+
+# SCHEMA {{{1
+# to_snake_case() {{{2
 def to_snake_case(text):
     return '_'.join(text.lower().split())
 
+# normalize_key() {{{2
 def normalize_key(key, parent_keys):
     if len(parent_keys) == 1:
         return key
     return to_snake_case(key.replace('_', ' '))
 
-def must_be_identifier(arg):
-    if not arg:
-        return arg
-    if not is_str(arg):
-        raise Invalid("expected string")
-    if arg and not arg.isidentifier():
-        raise Invalid(f"{arg}: expected identifier")
-    return arg
-
-def as_list(args):
+# to_list() {{{2
+def to_list(args):
     if is_str(args):
         args = args.split()
     if is_mapping(args):
         raise Invalid(f"{args}: expected list or string")
     return args
 
-def split_repo_name(arg):
-    # extract components from: config@host~user
-    try:
-        config, _, user = arg.partition('~')
-        config, _, host = config.partition('@')
-        return (
-            must_be_identifier(config),
-            must_be_identifier(host),
-            must_be_identifier(user)
-        )
-    except AttributeError:
-        raise ValueError("expected string")
+# a_name() {{{2
+def a_name(arg):
+    # names are expected to be identifiers except that dashes are allowed
+    if not arg:
+        return arg
+    if not is_str(arg):
+        raise Invalid("expected string")
+    cleaned = arg.replace('-', '0')
+    if not cleaned.isidentifier():
+        raise Invalid(f"{arg}: expected a name")
+    return arg
 
-def as_repo(arg):
-    config, host, user = split_repo_name(arg)
-    return Repository(config, host, user)
-
-def as_list_of_repos(repos):
-    if is_str(repos):
-        repos = repos.split()
-    if is_mapping(repos):
-        return must_be_a_repo(repos)
-    return [as_repo(repo) for repo in repos]
-
-def must_be_a_repo(repo):
-    if is_str(repo):
-        return [as_repo(repo)]
-    if is_mapping(repo):
-        if 'children' in repo:
-            children = as_list_of_repos(repo.pop('children'))
-            if repo:
-                raise Invalid("children cannot be used with other fields")
-            return children
-        must_be_identifier(repo.get('config'))
-        must_be_identifier(repo.get('host'))
-        must_be_identifier(repo.get('user'))
-        return [Repository(**repo)]
-    raise Invalid("must me a string or a dictionary")
+# a_spec() {{{2
+def a_spec(arg):
+    if is_str(arg):
+        return arg
+    if is_mapping(arg):
+        unknown_keys = arg.keys() - set(['config', 'host', 'user'])
+        if unknown_keys:
+            raise Invalid(f"unknown {plural(unknown_keys):key}: {conjoin(unknown_keys)}.")
+        if 'config' not in arg:
+            raise Invalid("config is a required key.")
+        spec = arg.get('config')
+        if arg.get('host'):
+            spec = f"{spec}@{arg.get('host')}"
+        if arg.get('user'):
+            spec = f"{spec}~{arg.get('user')}"
+        return spec
+    raise Invalid("expected a specification")
+
+# to_specs() {{{2
+def to_specs(arg):
+    if is_str(arg):
+        return [a_spec(r) for r in arg.split()]
+    if is_mapping(arg):
+        unknown_keys = arg.keys() - set(['config', 'host', 'user'])
+        if unknown_keys:
+            raise Invalid(f"unknown {plural(unknown_keys):key}: {conjoin(unknown_keys)}.")
+        return [a_spec(arg)]
+    if is_collection(arg):
+        return [a_spec(r) for r in arg]
+    raise Invalid("expected a repository specification")
 
+# validate_settings {{{2
 validate_settings = Schema({
-    Required('repositories'): {str: must_be_a_repo},
+    'repositories': {a_name: to_specs},
     'default_repository': str,
     'report_style': str,
     'compact_format': str,
-    'normal_format': str,
-    'normal_header': str,
-    'report_fields': as_list,
-    'tree_report_fields': as_list,
-    'nestedtext_report_fields': as_list,
-    'nestedtext_size_format': str,
-    'json_report_fields': as_list,
+    'table_format': str,
+    'table_header': str,
+    'report_fields': to_list,
+    'tree_report_fields': to_list,
+    'nestedtext_report_fields': to_list,
+    'json_report_fields': to_list,
     'size_format': str,
     'date_format': str,
 })
 
+# READ SETTINGS FILE {{{1
 try:
     # load tables from file
     keymap = {}
     settings = nt.load(
         settings_file,
         top = 'dict',
         normalize_key = normalize_key,
         keymap = keymap,
     )
 
-    # check structure of the file contends
     settings = validate_settings(settings)
-    repositories = settings['repositories']
+    specifications = settings.get('repositories', {})
+
+    # convert from specifications to Repository objects
+    repositories = {}
+    for name, specs in specifications.items():
+        if specs:
+            repositories[name] = []
+            alias = name if len(specs) <= 1 else None
+            for spec in specs:
+                if spec in repositories and spec != name:
+                    # this is a known (previously defined) repository
+                    repositories[name].extend(repositories[spec])
+                else:
+                    repositories[name].append(Repository(spec, alias))
+        else:
+            repositories[name] = [Repository(name)]
 
 except nt.NestedTextError as e:
     e.terminate()
+except FileNotFoundError:
+    settings = {}
+    repositories = {}
 except OSError as e:
     fatal(os_error(e), culprit=settings_file)
 except MultipleInvalid as e:  # report schema violations
     for err in e.errors:
         msg, flag = voluptuous_error_msg_mappings.get(
             err.msg, (err.msg, 'value')
         )
@@ -178,50 +274,8 @@
         codicil = loc.as_line(flag) if loc else None
         keys = nt.join_keys(err.path, keymap=keymap)
         error(
             full_stop(msg),
             culprit = (settings_file, keys),
             codicil = codicil
         )
-    terminate("borg-space: terminated due to previously reported errors.")
-
-def gather(repo):
-    try:
-        name = repo.get_name(None)
-    except TypeError:
-        return [repo]
-    if name.isidentifier() and name in repositories:
-        return repositories[name]
-    return [repo]
-
-def get_repos(repo):
-    if not repo:
-        repo = settings.get('default_repository')
-    if not repo:
-        raise Error('there is no default repository.')
-
-    try:
-        children = repositories[repo]
-    except KeyError:
-        # not found in repositories specified in settings file.
-        # see if it exist on local machine
-        try:
-            children = [as_repo(repo)]
-        except Invalid as e:
-            raise Error(str(e))
-
-    results = {}
-
-    to_process = []
-    for child in children:
-        to_process.extend(gather(child))
-
-    for child in to_process:
-        host, path = child.get_path(repo)
-        name = child.get_name(repo)
-        try:
-            results[name] = child.get_repo()
-        except Error as e:
-            e.report(culprit=name)
-        except OSError as e:
-            error(os_error(e), culprit=name)
-    return results
+    terminate()
```

### Comparing `borg_space-2.0/borg_space/main.py` & `borg_space-2.1/borg_space/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,106 +2,140 @@
 # description {{{1
 """
 Borg Space
 
 Reports on the current size of one or more Borg repositories managed by Emborg.
 
 Usage:
-    borg-space [--quiet] [--style <style>] [--record] [<repo>...]
-    borg-space [--graph] [--svg <file>] [--log-y] [<repo>...]
+    borg-space [--quiet] [--style <style>] [--record] [<spec>...]
+    borg-space [--graph] [--svg <file>] [--log-y] [--record] [<spec>...]
 
 Options:
     -r, --record                 save the result
     -q, --quiet                  do not output the size message
     -s <style>, --style <style>  the report style
-                                 choose from compact, normal, tree, nt, json
+                                 choose from compact, table, tree, nt, json
     -g, --graph                  graph the previously recorded sizes over time
     -l, --log-y                  use a logarithmic Y-axis when graphing
     -S <file>, --svg <file>      produce plot as SVG file rather than display it
 
-Results are saved to ~/.local/share/borg-space/<config>.nt.
+Repository specs take the form ❬name❭ or ❬config❭[@❬host❭][~❬user❭]. Items in
+brackets are optional and ❬name❭ is the name given for a repository the
+repositories setting.
+
+The available styles are compact, table, tree, nt or nestedtext, or json.
+If you specify something other than the these, what you give is taken to be a
+compact format specification.
+
+Results are saved to ~/.local/share/borg-space/<full-spec>.nt.
+Settings are held in ~/.config/borg-space/settings.nt.
 """
 
 # imports {{{1
-from .config import settings, get_repos, split_repo_name
+from .config import settings, get_repos
 from .trees import tree
 import arrow
 from appdirs import user_data_dir
 from docopt import docopt
-from inform import Error, display, error, os_error
+from inform import Error, display, error, os_error, warn
 from pathlib import Path
 from quantiphy import Quantity
 import json
 import nestedtext as nt
 import matplotlib
 import matplotlib.pyplot as plt
 from matplotlib.dates import AutoDateFormatter, AutoDateLocator
 from matplotlib.ticker import FuncFormatter
-import os
-import socket
-import pwd
 
 # globals {{{1
 data_dir = Path(user_data_dir('borg-space'))
 now = str(arrow.now())
 Quantity.set_prefs(prec='full')
-__version__ = "2.0"
-__released__ = "2023-05-15"
+__version__ = "2.1"
+__released__ = "2023-06-09"
 date_format = settings.get('date_format', 'D MMMM YYYY')
 size_format = settings.get('size_format', '.2b')
 nestedtext_size_format = settings.get('nestedtext_size_format', size_format)
-size_fields = ['size',]  # must be a single value
+size_fields = ['size',]  # must contain only one value
 date_fields = ['last_create', 'last_prune', 'last_compact', 'last_squeeze']
+all_fields = size_fields + date_fields
 report_fields = settings.get('report_fields', size_fields)
-
-# gethostname {{{1
-# returns short version of the hostname (the hostname without any domain name)
-def gethostname():
-    return socket.gethostname().split('.')[0]
-
-# getusername {{{1
-def getusername():
-    return pwd.getpwuid(os.getuid()).pw_name
+not_available = "⟪not available⟫"
 
 # collect_repos() {{{1
 def collect_repos(requests, record_size):
     repos = {}
     for request in requests:
-        repos = get_repos(request)
-        repos.update(repos)
+        new_repos = get_repos(request)
+        repos.update(new_repos)
 
     # record the size if requested {{{3
     if record_size:
         for name, repo in repos.items():
 
             # read previously recorded sizes
             data_path = Path(data_dir / f'{name}.nt')
             try:
                 data = nt.load(data_path, top=dict)
             except FileNotFoundError:
+                data_path.parent.mkdir(parents=True, exist_ok=True)
                 data = {}
 
-            # append new size
-            data[now] = repo['size'].fixed()
+            latest = repo.get_latest()
+            try:
+                # append new size
+                data[now] = latest['size'].fixed()
 
-            # write out sizes
-            nt.dump(data, data_path)
+                # write out sizes
+                nt.dump(data, data_path)
+            except KeyError:
+                warn('size not found, not recording.', culprit=name)
 
     return repos
 
+# formatter() {{{1
+def formatter(repo, fields, missing):
+    # formats the values of a repository field
+
+    def format(value, format):
+        if value is None:
+            return missing
+        if not format:
+            return str(value)
+        return value.format(format)
+
+    to_output = {}
+    for field in fields:
+        value = repo.get(field)
+        if field in size_fields:
+            value = format(value, size_format)
+        elif field in date_fields:
+            value = format(value, date_format)
+        to_output[field.replace('_', ' ')] = value
+    if len(to_output) == 1:
+        # output as a scalar if there is only one value
+        to_output = next(iter(to_output.values()))
+    return to_output
+
 # generate_graph() {{{1
 def generate_graph(repos, svg_file, log_scale):
     if svg_file:
         matplotlib.use('SVG')
 
     # determine size history of each config's repository {{{2
     traces = []
     for name in repos:
         data_path = data_dir / f'{name}.nt'
-        data = nt.load(data_path, top=dict)
+        try:
+            data = nt.load(data_path, top=dict)
+        except OSError as e:
+            raise Error(
+                os_error(e),
+                codicil="No history is available to plot, have you run with --record?"
+            )
         sizes = []
         dates = []
         for date, size in data.items():
             dates.append(arrow.get(date))
             sizes.append(Quantity(size, 'B').real)
         traces.append((name, Quantity(size, 'B'), dates, sizes))
 
@@ -121,19 +155,19 @@
     largest = 0
     smallest = 1e100
     for entry in sorted(traces, key=lambda d: d[1], reverse=True):
         name, last_size, dates, sizes = entry
         largest = max(largest, *sizes)
         smallest = min(smallest, *sizes)
         trace, = ax.plot_date(dates, sizes, "-")
-        trace.set_label(f'{name} ({last_size})')
+        trace.set_label(f'{name} ({last_size:{size_format}})')
 
     # use SI scale factors on Y-axis
-    def bytes(y, pos=None):
-        return Quantity(y, 'B').render()
+    def bytes(value, pos=None):
+        return Quantity(value, 'B').render()
     ax.yaxis.set_major_formatter(FuncFormatter(bytes))
     if largest / smallest > 10:
         ax.yaxis.set_minor_formatter("")
     else:
         ax.yaxis.set_minor_formatter(FuncFormatter(bytes))
 
     # draw the graph {{{3
@@ -144,200 +178,166 @@
         plt.show()
 
 # print_report() {{{1
 def print_report(repos, style):
     if not style:
         style = settings.get('report_style', 'compact')
     if style == 'compact':
-        print_compact_report(repos)
-    elif style == 'normal':
-        print_normal_report(repos)
+        print_compact_report(repos, None)
+    elif style == 'table':
+        print_table_report(repos)
     elif style == 'tree':
         print_tree_report(repos)
     elif style in ['nt', 'nestedtext']:
         print_nestedtext_report(repos)
     elif style == 'json':
         print_json_report(repos)
     else:
-        raise Error(
-            "unknown style",
-            "choose from compact, normal, tree, nt or nestedtext, or json",
-            culprit = style
-        )
+        print_compact_report(repos, style)
 
 # print_compact_report() {{{1
-def print_compact_report(repos):
+def print_compact_report(repos, style):
     # most compact, but has awkward config labels
 
     fmt = size_format
-    msg_fmt = settings.get(
-        'compact_format',
-        '{config}: {size:{fmt}}'
-    )
+    if style:
+        msg_fmt = style
+    else:
+        msg_fmt = settings.get('compact_format', '{name}: {size:{fmt}}')
 
     # report the sizes
     for name in sorted(repos):
         repo = repos[name]
-        msg = msg_fmt.format(repo=name, fmt=fmt, **repo)
-        display(msg)
+        try:
+            msg = msg_fmt.format(fmt=fmt, **repo.as_dict())
+            display(msg)
+        except KeyError as e:
+            warn('not available.', culprit=(name, e))
 
-# print_normal_report() {{{1
-def print_normal_report(repos):
+# print_table_report() {{{1
+def print_table_report(repos):
     # same number of lines as compact, but a bit more verbose
 
     fmt = size_format
-    hostname = gethostname()
-    username = getusername()
     msg_fmt = settings.get(
-        'normal_format',
+        'table_format',
         '{host:8} {user:8} {config:8} {size:<8.2b}  {last_create:ddd, MMM DD}'
     )
 
-    # split config name, then sort by host, user, then config
-    repos = sorted(
-        (split_repo_name(name) + (repo,) for name, repo in repos.items()),
-        key = lambda k: (k[2], k[1], k[0])
-    )
-
     # report the sizes
     header = settings.get(
-        'normal_header',
+        'table_header',
         'HOST     USER     CONFIG   SIZE      LAST BACK UP'
     )
     if header:
         display(header)
 
-    for cfg, hst, usr, repo in repos:
-        hst = hst or hostname
-        usr = usr or username
-        msg = msg_fmt.format(host=hst, user=usr, config=cfg, fmt=fmt, **repo)
-        display(msg)
+    for name in sorted(repos):
+        repo = repos[name]
+        try:
+            msg = msg_fmt.format(fmt=fmt, **repo.as_dict())
+            display(msg)
+        except KeyError as e:
+            warn('not available.', culprit=(name, e))
 
 # as_hierarchy() {{{1
-def as_hierarchy(repos, fmt, squeeze):
-    hostname = gethostname()
-    username = getusername()
-
-    # split config name, then sort by host, user, then config
-    repos = sorted(
-        (split_repo_name(name) + (repo,) for name, repo in repos.items()),
-        key = lambda k: (k[1], k[2], k[0])
-    )
-
+def as_hierarchy(repos, fmt, fields, missing):
     # convert hierarchy levels to dictionaries
-    if squeeze:
-        # lowest level is a list of strings rather than a dictionary
-        hierarchy = {}
-        for cfg, hst, usr, repo in repos:
-            hst = hst or hostname
-            usr = usr or username
-            if hst not in hierarchy:
-                hierarchy[hst] = {}
-            if usr not in hierarchy[hst]:
-                hierarchy[hst][usr] = [] if squeeze else {}
-            if cfg not in hierarchy[hst][usr]:
-                hierarchy[hst][usr].append(f"{cfg}: {fmt(repo)}")
-    else:
-        hierarchy = {}
-        # all levels are dictionaries, lowest level is dictionary of strings
-        for cfg, hst, usr, repo in repos:
-            hst = hst or hostname
-            usr = usr or username
-            if hst not in hierarchy:
-                hierarchy[hst] = {}
-            if usr not in hierarchy[hst]:
-                hierarchy[hst][usr] = [] if squeeze else {}
-            if cfg not in hierarchy[hst][usr]:
-                hierarchy[hst][usr][cfg] = fmt(repo)
-
+    hierarchy = {}
+    # all levels are dictionaries, lowest level is dictionary of strings
+    for name in sorted(repos):
+        repo = repos[name]
+        if repo.host not in hierarchy:
+            hierarchy[repo.host] = {}
+        if repo.user not in hierarchy[repo.host]:
+            hierarchy[repo.host][repo.user] = {}
+        if repo.config not in hierarchy[repo.host][repo.user]:
+            hierarchy[repo.host][repo.user][repo.config] = fmt(repo, fields, missing)
     return hierarchy
 
 # print_tree_report() {{{1
 def print_tree_report(repos):
     # longer than previous formats
     # good when there are many repos per host & user
     fields = settings.get('tree_report_fields', report_fields)
 
-    def formatter(repo):
-        to_output = {}
-        for field in fields:
-            value = repo[field]
-            if field in size_fields:
-                value = value.format(size_format)
-            elif field in date_fields:
-                value = value.format(date_format) if date_format else str(value)
-            to_output[field] = value
-        return to_output
-
-    squeeze = fields == size_fields
-    if squeeze:
-        formatter = lambda r: r['size'].format(size_format)
-
-    display(tree(as_hierarchy(repos, fmt=formatter, squeeze=squeeze)))
+    display(
+        tree(
+            as_hierarchy(
+                repos,
+                fmt = formatter,
+                fields = fields,
+                missing = not_available,
+            )
+        )
+    )
 
 # print_nestedtext_report() {{{1
 def print_nestedtext_report(repos):
     # same number of lines as tree, but both computer & human readable
     fields = settings.get('nestedtext_report_fields', report_fields)
 
-    def formatter(repo):
-        to_output = {}
-        for field in fields:
-            value = repo[field]
-            if field in size_fields:
-                value = value.format(nestedtext_size_format)
-            elif field in date_fields:
-                value = value.format(date_format) if date_format else str(value)
-            to_output[field] = value
-        return to_output
-
-    display(nt.dumps(as_hierarchy(repos, fmt=formatter, squeeze=False)))
+    display(
+        nt.dumps(
+            as_hierarchy(
+                repos,
+                fmt = formatter,
+                fields = fields,
+                missing = not_available,
+            )
+        )
+    )
 
 # print_json_report() {{{1
 def print_json_report(repos):
     # easily computer readable, but awkward for people
-    fields = settings.get('json_report_fields', report_fields)
+    fields = settings.get('json_report_fields', all_fields)
 
-    def formatter(repo):
+    def formatter(repo, fields, missing):
         to_output = {}
+        info = repo.as_dict()
         for field in fields:
-            value = repo[field]
-            if field in size_fields:
+            value = info.get(field)
+            if value is None:
+                value = missing
+            elif field in size_fields:
                 value = int(value)
             elif field in date_fields:
                 value = str(value)
             to_output[field] = value
         return to_output
 
     display(
         json.dumps(
-            as_hierarchy(repos, fmt=formatter, squeeze=False),
-            indent=4,
-            separators=(',', ': '),
-            ensure_ascii=False
+            as_hierarchy(
+                repos,
+                fmt = formatter,
+                fields = fields,
+                missing = None
+            ),
+            indent = 4,
+            separators = (',', ': '),
+            ensure_ascii = False
         )
     )
 
 # main() {{{1
 def main():
     cmdline = docopt(__doc__, version=__version__)
 
-    requests = cmdline['<repo>']
+    requests = cmdline['<spec>']
     if not requests:
         requests = ['']  # this gets the default config
 
     try:
         repos = collect_repos(requests, cmdline['--record'])
-
-        if cmdline['--graph'] or cmdline['--svg'] or cmdline['--log-y']:
-            generate_graph(repos, cmdline['--svg'], cmdline['--log-y'])
-        elif not cmdline['--quiet']:
-            print_report(repos, cmdline['--style'])
+        if repos:
+            if cmdline['--graph'] or cmdline['--svg'] or cmdline['--log-y']:
+                generate_graph(repos, cmdline['--svg'], cmdline['--log-y'])
+            elif not cmdline['--quiet']:
+                print_report(repos, cmdline['--style'])
     except (Error, nt.NestedTextError) as e:
         e.report()
     except OSError as e:
         error(os_error(e))
     except KeyboardInterrupt:
         pass
-
-if __name__ == '__main__':
-    main()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `borg_space-2.0/borg_space/trees.py` & `borg_space-2.1/borg_space/trees.py`

 * *Files 20% similar despite different names*

```diff
@@ -47,35 +47,37 @@
     return _tree(data, key_suffix, top=True)
 
 def _tree(data, key_suffix, top=False, leader=''):
     lines = []
     if hasattr(data, 'items'):
         last = len(data) - 1
         for i, item in enumerate(data.items()):
-            k, v = item
+            key, value = item
             # determine key-leader-supplement and item-leader-supplement
             if top:
                 kls = ''
                 ils = ''
             elif i < last:
                 kls = connectors.item
                 ils = connectors.lead
-            elif i == last:
-                kls = connectors.last_item
-                ils = connectors.last_lead
             else:
-                raise NotImplementedError
-                kls = connectors.last_lead
+                kls = connectors.last_item
                 ils = connectors.last_lead
 
-            # append dictionary to those already processed
-            lines += [
-                leader + kls + k + key_suffix,
-                _tree(v, key_suffix, leader = leader + ils) if v else None
-            ]
+            if is_collection(value):
+                # append dictionary to those already processed
+                lines += [
+                    leader + kls + key + key_suffix,
+                    _tree(value, key_suffix, leader = leader + ils) if value else None
+                ]
+            else:
+                # the value is a scalar, so squeeze key & value on one line
+                lines += [
+                    leader + kls + key + ': ' + value,
+                ]
         return '\n'.join(l for l in lines if l)
 
     elif not is_collection(data):
         data = [str(data)]
 
     if top:
         joiner = '\n'
```

### Comparing `borg_space-2.0/pyproject.toml` & `borg_space-2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "borg_space"
 dist-name = "borg-space"
-version = "2.0"
+version = "2.1"
 description = "Accessory for Emborg used to report and track the size of your Borg repositories"
 readme = "README.rst"
 requires-python = ">=3.6"
 license = {file = "LICENSE"}
 keywords = ["emborg", "borg", "backups"]
 authors = [{name = "Ken Kundert", email = "emborg@nurdletech.com"}]
 classifiers = [
```

