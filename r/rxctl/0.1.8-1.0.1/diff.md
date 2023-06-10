# Comparing `tmp/rxctl-0.1.8.tar.gz` & `tmp/rxctl-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rxctl-0.1.8.tar", max compression
+gzip compressed data, was "rxctl-1.0.1.tar", max compression
```

## Comparing `rxctl-0.1.8.tar` & `rxctl-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    11357 2023-06-07 16:18:25.633562 rxctl-0.1.8/LICENSE
--rw-r--r--   0        0        0     4462 2023-03-03 08:32:21.460839 rxctl-0.1.8/README.md
--rw-r--r--   0        0        0      590 2023-06-07 16:19:06.142349 rxctl-0.1.8/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-07 14:22:03.305033 rxctl-0.1.8/rxctl/__init__.py
--rw-r--r--   0        0        0       38 2023-06-07 16:19:06.142349 rxctl-0.1.8/rxctl/__version__.py
--rw-r--r--   0        0        0      262 2022-12-12 10:21:43.256203 rxctl-0.1.8/rxctl/bin/__init
--rwxr-xr-x   0        0        0      356 2022-12-16 14:17:41.837487 rxctl-0.1.8/rxctl/bin/__run
--rwxr-xr-x   0        0        0      626 2022-12-21 06:45:47.235315 rxctl-0.1.8/rxctl/bin/__wait
--rwxr-xr-x   0        0        0     3986 2023-01-30 08:09:39.963436 rxctl-0.1.8/rxctl/lib/ansible.sh
--rw-r--r--   0        0        0      428 2023-03-03 08:36:35.590713 rxctl-0.1.8/rxctl/lib/links.json
--rw-r--r--   0        0        0      703 2023-06-07 15:01:53.479017 rxctl-0.1.8/rxctl/lib/links.py
--rwxr-xr-x   0        0        0     3096 2023-06-07 15:07:50.442648 rxctl-0.1.8/rxctl/lib/log.py
--rw-r--r--   0        0        0    14813 2023-06-07 16:16:28.179133 rxctl-0.1.8/rxctl/lib/main.py
--rwxr-xr-x   0        0        0      439 2023-01-03 10:08:29.507259 rxctl-0.1.8/rxctl/lib/scp.sh
--rw-r--r--   0        0        0     2188 2023-06-07 15:15:48.552838 rxctl-0.1.8/rxctl/lib/utils.py
--rw-r--r--   0        0        0     5061 1970-01-01 00:00:00.000000 rxctl-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-10 18:16:45.666422 rxctl-1.0.1/LICENSE
+-rw-r--r--   0        0        0     4798 2023-06-10 18:16:45.666422 rxctl-1.0.1/README.md
+-rw-r--r--   0        0        0      590 2023-06-10 18:17:01.094470 rxctl-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-10 18:16:45.666422 rxctl-1.0.1/rxctl/__init__.py
+-rw-r--r--   0        0        0       38 2023-06-10 18:17:01.098470 rxctl-1.0.1/rxctl/__version__.py
+-rw-r--r--   0        0        0      262 2023-06-10 18:16:45.666422 rxctl-1.0.1/rxctl/bin/__init
+-rwxr-xr-x   0        0        0      356 2023-06-10 18:16:45.666422 rxctl-1.0.1/rxctl/bin/__run
+-rwxr-xr-x   0        0        0      626 2023-06-10 18:16:45.666422 rxctl-1.0.1/rxctl/bin/__wait
+-rwxr-xr-x   0        0        0     3986 2023-06-10 18:16:45.666422 rxctl-1.0.1/rxctl/lib/ansible.sh
+-rw-r--r--   0        0        0      428 2023-06-10 18:16:45.666422 rxctl-1.0.1/rxctl/lib/links.json
+-rw-r--r--   0        0        0      703 2023-06-10 18:16:45.666422 rxctl-1.0.1/rxctl/lib/links.py
+-rwxr-xr-x   0        0        0     3096 2023-06-10 18:16:45.666422 rxctl-1.0.1/rxctl/lib/log.py
+-rw-r--r--   0        0        0    14879 2023-06-10 18:16:45.666422 rxctl-1.0.1/rxctl/lib/main.py
+-rwxr-xr-x   0        0        0      439 2023-06-10 18:16:45.666422 rxctl-1.0.1/rxctl/lib/scp.sh
+-rw-r--r--   0        0        0     2188 2023-06-10 18:16:45.666422 rxctl-1.0.1/rxctl/lib/utils.py
+-rw-r--r--   0        0        0     5397 1970-01-01 00:00:00.000000 rxctl-1.0.1/PKG-INFO
```

### Comparing `rxctl-0.1.8/LICENSE` & `rxctl-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rxctl-0.1.8/README.md` & `rxctl-1.0.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -21,29 +21,34 @@
   --use-ssh-password      Ask for ssh password
   --use-sudo-password     Ask for sudo password
   --ssh-opt TEXT          SSH options  [default: -o ControlMaster=auto -o
                           ControlPath=/dev/shm/rx-ssh-%h -o ControlPersist=5m
                           -o ConnectTimeout=1]
   --password-envvar TEXT  Environment variable used to pass password to sudo
                           [default: LC_PASSWD]
-  -u, --user TEXT         SSH user  [default: current user]
-  -P, --parallel INTEGER  How many threads to use to run hosts in parallel
-                          [default: 1]
+  -u, --user TEXT         SSH user  [default: mcraiu]
+  -P, --parallel          Run hosts in parallel
+  --max-parallel INTEGER  How many threads to use to run hosts in parallel, 0
+                          - run everything in parralel  [default: 0]
   -A, --ad-hoc            Task list is a remote ad-hoc command
-  -I, --inventory         Show environment inventory
+  -I, --inventory         With -S shows the list of hosts, by itself shows the
+                          inventory summary.
   -c, --check-only        Show valid inventory
   -l, --task-list         List tasks in local directory
   -t, --task-help TEXT    Show help for a task
   -w, --warning-only      Don't exit if a host fails check, evict host from
                           inventory
   -x, --exclude TEXT      Comma separated list of host to exclude from
                           inventory (can be used multiple times)
+  -i, --inline-check      Don't check hosts before tasks, do it for each host
+                          at the begining of the task list
   --set-env TEXT          Set environment variable (can be used multiple
                           times)
   -v, --verbosity         Verbosity level, up to 3
+  -V, --version           Show the version and exit.
   --help                  Show this message and exit.
 ```
 
 ## Environment script
 The environment script (default ```./environment```) is used to overwrite rxctl parameters and to generate the list of host (inventory) on which to run the tasks:
 - ```environment check```, should produce a JSON dictionary of parameters you want to overwrite,
 - ```environment inventory```, free text which is displayed when you run ```rxctl -I``` without any other parameter,
```

### Comparing `rxctl-0.1.8/pyproject.toml` & `rxctl-1.0.1/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rxctl"
-version = "0.1.8"
+version = "1.0.1"
 description = "Linux remote execution tool"
 authors = ["mihaiush <mihaiush@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/mihaiush/rxctl"
 
 [tool.poetry.dependencies]
 python = "^3.7"
```

### Comparing `rxctl-0.1.8/rxctl/bin/__wait` & `rxctl-1.0.1/rxctl/bin/__wait`

 * *Files identical despite different names*

### Comparing `rxctl-0.1.8/rxctl/lib/ansible.sh` & `rxctl-1.0.1/rxctl/lib/ansible.sh`

 * *Files identical despite different names*

### Comparing `rxctl-0.1.8/rxctl/lib/links.py` & `rxctl-1.0.1/rxctl/lib/links.py`

 * *Files identical despite different names*

### Comparing `rxctl-0.1.8/rxctl/lib/log.py` & `rxctl-1.0.1/rxctl/lib/log.py`

 * *Files identical despite different names*

### Comparing `rxctl-0.1.8/rxctl/lib/main.py` & `rxctl-1.0.1/rxctl/lib/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -54,19 +54,20 @@
               help='Environment variable used to pass password to sudo')
 @click.option('-u', '--user', default=os.environ['USER'], show_default=True,
               help='SSH user')
 @click.option('-P', '--parallel', default=False, is_flag=True,
               help='Run hosts in parallel')
 @click.option('--max-parallel', default=0, show_default=True,
               help='How many threads to use to run hosts in parallel,'
-              ' 0 - run everithing in parralel')
+              ' 0 - run everything in parralel')
 @click.option('-A', '--ad-hoc', default=False, is_flag=True,
               help='Task list is a remote ad-hoc command')
 @click.option('-I', '--inventory', default=False, is_flag=True,
-              help='Show environment inventory')
+              help='With -S shows the list of hosts,'
+              ' by itself shows the inventory summary.')
 @click.option('-c', '--check-only', default=False, is_flag=True,
               help='Show valid inventory')
 @click.option('-l', '--task-list', default=False, is_flag=True,
               help='List tasks in local directory')
 @click.option('-t', '--task-help', default=None,
               help='Show help for a task')
 @click.option('-w', '--warning-only', default=False, is_flag=True,
@@ -380,17 +381,17 @@
                 'Task terminated with error, aborting', reverse=True))
             sys.exit(1)
     else:
         LOG.info(click.style('OK', reverse=True))
 
 
 def check(host, ctx):
-    cmd_template = 'set -x ; LOG=$(mktemp -p /tmp rx-XXXXXXXX) ; \
-        exec 3>&1 4>&2 1>$LOG 2>&1 ; {} ; RC=$? ; exec 1>&3 2>&4 ; \
-        cat $LOG ; rm -fv $LOG ; exit $RC'
+    cmd_template = 'set -x ; LOG=$(mktemp -p /tmp rx-XXXXXXXX) ;' \
+        'exec 3>&1 4>&2 1>$LOG 2>&1 ; {} ; RC=$? ; exec 1>&3 2>&4 ;' \
+        'cat $LOG ; rm -fv $LOG ; exit $RC'
     valid_host = True
     cmd = '{} -v {} true'.format(ctx.ssh_cmd, host)
     cmd = cmd_template.format(cmd)
     LOG.debug('SSH:\n{}'.format(cmd))
     p = subprocess.run(cmd, shell=True, encoding='utf-8',
                        errors='ignore', bufsize=0,
                        stdout=subprocess.PIPE,
```

### Comparing `rxctl-0.1.8/rxctl/lib/utils.py` & `rxctl-1.0.1/rxctl/lib/utils.py`

 * *Files identical despite different names*

### Comparing `rxctl-0.1.8/PKG-INFO` & `rxctl-1.0.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rxctl
-Version: 0.1.8
+Version: 1.0.1
 Summary: Linux remote execution tool
 Home-page: https://github.com/mihaiush/rxctl
 Author: mihaiush
 Author-email: mihaiush@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -39,29 +39,34 @@
   --use-ssh-password      Ask for ssh password
   --use-sudo-password     Ask for sudo password
   --ssh-opt TEXT          SSH options  [default: -o ControlMaster=auto -o
                           ControlPath=/dev/shm/rx-ssh-%h -o ControlPersist=5m
                           -o ConnectTimeout=1]
   --password-envvar TEXT  Environment variable used to pass password to sudo
                           [default: LC_PASSWD]
-  -u, --user TEXT         SSH user  [default: current user]
-  -P, --parallel INTEGER  How many threads to use to run hosts in parallel
-                          [default: 1]
+  -u, --user TEXT         SSH user  [default: mcraiu]
+  -P, --parallel          Run hosts in parallel
+  --max-parallel INTEGER  How many threads to use to run hosts in parallel, 0
+                          - run everything in parralel  [default: 0]
   -A, --ad-hoc            Task list is a remote ad-hoc command
-  -I, --inventory         Show environment inventory
+  -I, --inventory         With -S shows the list of hosts, by itself shows the
+                          inventory summary.
   -c, --check-only        Show valid inventory
   -l, --task-list         List tasks in local directory
   -t, --task-help TEXT    Show help for a task
   -w, --warning-only      Don't exit if a host fails check, evict host from
                           inventory
   -x, --exclude TEXT      Comma separated list of host to exclude from
                           inventory (can be used multiple times)
+  -i, --inline-check      Don't check hosts before tasks, do it for each host
+                          at the begining of the task list
   --set-env TEXT          Set environment variable (can be used multiple
                           times)
   -v, --verbosity         Verbosity level, up to 3
+  -V, --version           Show the version and exit.
   --help                  Show this message and exit.
 ```
 
 ## Environment script
 The environment script (default ```./environment```) is used to overwrite rxctl parameters and to generate the list of host (inventory) on which to run the tasks:
 - ```environment check```, should produce a JSON dictionary of parameters you want to overwrite,
 - ```environment inventory```, free text which is displayed when you run ```rxctl -I``` without any other parameter,
```

