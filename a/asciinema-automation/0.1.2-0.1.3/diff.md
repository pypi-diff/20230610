# Comparing `tmp/asciinema-automation-0.1.2.tar.gz` & `tmp/asciinema-automation-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asciinema-automation-0.1.2.tar", last modified: Wed Mar 29 16:43:22 2023, max compression
+gzip compressed data, was "asciinema-automation-0.1.3.tar", last modified: Sat Jun 10 14:29:20 2023, max compression
```

## Comparing `asciinema-automation-0.1.2.tar` & `asciinema-automation-0.1.3.tar`

### file list

```diff
@@ -1,19 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 16:43:22.021851 asciinema-automation-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-03-29 16:43:12.000000 asciinema-automation-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-03-29 16:43:22.021851 asciinema-automation-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-03-29 16:43:12.000000 asciinema-automation-0.1.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 16:43:22.021851 asciinema-automation-0.1.2/asciinema_automation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 16:43:12.000000 asciinema-automation-0.1.2/asciinema_automation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-03-29 16:43:12.000000 asciinema-automation-0.1.2/asciinema_automation/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-03-29 16:43:12.000000 asciinema-automation-0.1.2/asciinema_automation/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4128 2023-03-29 16:43:12.000000 asciinema-automation-0.1.2/asciinema_automation/instruction.py
--rw-r--r--   0 runner    (1001) docker     (123)     6751 2023-03-29 16:43:12.000000 asciinema-automation-0.1.2/asciinema_automation/script.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 16:43:22.021851 asciinema-automation-0.1.2/asciinema_automation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-03-29 16:43:22.000000 asciinema-automation-0.1.2/asciinema_automation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-03-29 16:43:22.000000 asciinema-automation-0.1.2/asciinema_automation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-29 16:43:22.000000 asciinema-automation-0.1.2/asciinema_automation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-03-29 16:43:22.000000 asciinema-automation-0.1.2/asciinema_automation.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-29 16:43:22.000000 asciinema-automation-0.1.2/asciinema_automation.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-29 16:43:22.000000 asciinema-automation-0.1.2/asciinema_automation.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-03-29 16:43:22.021851 asciinema-automation-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-29 16:43:12.000000 asciinema-automation-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 14:29:20.901801 asciinema-automation-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-10 14:29:05.000000 asciinema-automation-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-06-10 14:29:20.901801 asciinema-automation-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-06-10 14:29:05.000000 asciinema-automation-0.1.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 14:29:20.901801 asciinema-automation-0.1.3/asciinema_automation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 14:29:05.000000 asciinema-automation-0.1.3/asciinema_automation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-10 14:29:05.000000 asciinema-automation-0.1.3/asciinema_automation/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-06-10 14:29:05.000000 asciinema-automation-0.1.3/asciinema_automation/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4006 2023-06-10 14:29:05.000000 asciinema-automation-0.1.3/asciinema_automation/instruction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6750 2023-06-10 14:29:05.000000 asciinema-automation-0.1.3/asciinema_automation/script.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 14:29:20.901801 asciinema-automation-0.1.3/asciinema_automation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-06-10 14:29:20.000000 asciinema-automation-0.1.3/asciinema_automation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-06-10 14:29:20.000000 asciinema-automation-0.1.3/asciinema_automation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 14:29:20.000000 asciinema-automation-0.1.3/asciinema_automation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-10 14:29:20.000000 asciinema-automation-0.1.3/asciinema_automation.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-10 14:29:20.000000 asciinema-automation-0.1.3/asciinema_automation.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-10 14:29:20.000000 asciinema-automation-0.1.3/asciinema_automation.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-06-10 14:29:05.000000 asciinema-automation-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 14:29:20.901801 asciinema-automation-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-10 14:29:05.000000 asciinema-automation-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 14:29:20.901801 asciinema-automation-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-06-10 14:29:05.000000 asciinema-automation-0.1.3/tests/test_regression.py
```

### Comparing `asciinema-automation-0.1.2/LICENSE` & `asciinema-automation-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `asciinema-automation-0.1.2/PKG-INFO` & `asciinema-automation-0.1.3/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,19 @@
-Metadata-Version: 2.1
-Name: asciinema-automation
-Version: 0.1.2
-Summary: CLI utility to automate asciinema
-Home-page: https://github.com/PierreMarchand20/asciinema_automation
-Author: Pierre Marchand
-License: MIT
-Keywords: asciinema
-License-File: LICENSE
-
 asciinema-automation
 ####################
 
 .. image:: https://badge.fury.io/py/asciinema-automation.svg
     :target: https://badge.fury.io/py/asciinema-automation
 
+.. image:: https://github.com/PierreMarchand20/asciinema_automation/actions/workflows/CI.yml/badge.svg
+   :target: https://github.com/PierreMarchand20/asciinema_automation/actions/workflows/CI.yml
+   
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+   :target: https://github.com/psf/black
+
 Asciinema-Automation is a Python package which provides a small CLI utility to automate `asciinema <https://asciinema.org>`_ recordings. The only dependencies are asciinema and `Pexpect <https://pexpect.readthedocs.io/>`_.
 
 Example
 -------
 
 .. image:: https://raw.githubusercontent.com/PierreMarchand20/asciinema_automation/main/demo.gif
     :alt: Demo
```

### Comparing `asciinema-automation-0.1.2/asciinema_automation/cli.py` & `asciinema-automation-0.1.3/asciinema_automation/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,61 +1,95 @@
 import argparse
 import logging
 import pathlib
-from asciinema_automation.script import Script
 
+from asciinema_automation.script import Script
 
-def cli():
 
+def cli(argv=None):
     # Command line arguments
     parser = argparse.ArgumentParser()
     parser.add_argument(
-        'inputfile', help="file containing list of instructions", type=str)
-    parser.add_argument(
-        'outputfile', help="file containing recording", type=str)
+        "inputfile", help="file containing list of instructions", type=str
+    )
+    parser.add_argument("outputfile", help="file containing recording", type=str)
 
-    parser.add_argument('-aa', '--asciinema-arguments', type=str,
-                        default="", help="arguments to be passed to asciinema")
-    parser.add_argument('-dt', '--delay', type=int, default=150,
-                        help="mean for gaussian used to generate time between key strokes")
-    parser.add_argument('-wt', '--wait', type=int, default=80,
-                        help="time between each instructions")
-    parser.add_argument('-sd', '--standart-deviation', type=int, default=60,
-                        help="standart deviation for gaussian used to generate time between key strokes")
-    parser.add_argument('-t', '--timeout', type=int, default=30,
-                        help="timeout for a command output to come through")
+    parser.add_argument(
+        "-aa",
+        "--asciinema-arguments",
+        type=str,
+        default="",
+        help="arguments to be passed to asciinema",
+    )
+    parser.add_argument(
+        "-dt",
+        "--delay",
+        type=int,
+        default=150,
+        help="mean for gaussian used to generate time between key strokes",
+    )
+    parser.add_argument(
+        "-wt", "--wait", type=int, default=80, help="time between each instructions"
+    )
+    parser.add_argument(
+        "-sd",
+        "--standart-deviation",
+        type=int,
+        default=60,
+        help="standart deviation for gaussian used to generate time between key strokes",
+    )
+    parser.add_argument(
+        "-t",
+        "--timeout",
+        type=int,
+        default=30,
+        help="timeout for a command output to come through",
+    )
     group = parser.add_mutually_exclusive_group()
     group.add_argument(
-        '-d', '--debug',
+        "-d",
+        "--debug",
         help="set loglevel to DEBUG and output to 'outputfile.log'. Default loglevel to ERROR.",
-        action="store_const", dest="loglevel", const=logging.DEBUG,
+        action="store_const",
+        dest="loglevel",
+        const=logging.DEBUG,
         default=logging.ERROR,
     )
     group.add_argument(
-        '-v', '--verbose',
+        "-v",
+        "--verbose",
         help="set loglevel to INFO and output to 'outputfile.log'. Default loglevel to ERROR.",
-        action="store_const", dest="loglevel", const=logging.INFO,
+        action="store_const",
+        dest="loglevel",
+        const=logging.INFO,
     )
 
     # Command line inputs
-    inputfile = pathlib.Path(parser.parse_args().inputfile)
-    outputfile = pathlib.Path(parser.parse_args().outputfile)
-    delay = parser.parse_args().delay
-    wait = parser.parse_args().wait
-    asciinema_arguments = parser.parse_args().asciinema_arguments
-    standart_deviation = parser.parse_args().standart_deviation
-    loglevel = parser.parse_args().loglevel
-    timeout = parser.parse_args().timeout
+    args = parser.parse_args(argv)
+    inputfile = pathlib.Path(args.inputfile)
+    outputfile = pathlib.Path(args.outputfile)
+    delay = args.delay
+    wait = args.wait
+    asciinema_arguments = args.asciinema_arguments
+    standart_deviation = args.standart_deviation
+    loglevel = args.loglevel
+    timeout = args.timeout
 
     # Setup logger
     logfile = None
     if loglevel < logging.ERROR:
-        logfile = outputfile.with_suffix(
-            ".log")
+        logfile = outputfile.with_suffix(".log")
     logging.basicConfig(filename=logfile, level=loglevel)
 
     # Script
-    script = Script(inputfile, outputfile, asciinema_arguments,
-                    wait, delay, standart_deviation, timeout)
+    script = Script(
+        inputfile,
+        outputfile,
+        asciinema_arguments,
+        wait,
+        delay,
+        standart_deviation,
+        timeout,
+    )
 
     #
     script.execute()
```

### Comparing `asciinema-automation-0.1.2/asciinema_automation/instruction.py` & `asciinema-automation-0.1.3/asciinema_automation/instruction.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,143 +1,139 @@
-
 import logging
-import time
 import random
+import re
+import time
 
+logger = logging.getLogger(__name__)
 
-class Instruction:
 
+class Instruction:
     def run(self, script):
-        logging.info(self.__class__.__name__)
+        logger.info(self.__class__.__name__)
 
 
 class ChangeWaitInstruction(Instruction):
     def __init__(self, wait):
         super().__init__()
         self.wait = wait
 
     def run(self, script):
         super().run(script)
-        logging.debug("%s->%s", script.wait, self.wait)
+        logger.debug("%s->%s", script.wait, self.wait)
         script.wait = self.wait
 
 
 class ChangeDelayInstruction(Instruction):
     def __init__(self, delay):
         super().__init__()
         self.delay = delay
 
     def run(self, script):
         super().run(script)
-        logging.debug("%s->%s", script.delay, self.delay)
+        logger.debug("%s->%s", script.delay, self.delay)
         script.delay = self.delay
 
 
 class ExpectInstruction(Instruction):
     def __init__(self, expect_value: str, timeout: int):
         super().__init__()
         self.expect_value = expect_value
         self.timeout = timeout
 
     def run(self, script):
         super().run(script)
-        logging.debug("Expect %s", repr(self.expect_value))
+        logger.debug("Expect %s", repr(self.expect_value))
         script.process.expect(self.expect_value, timeout=self.timeout)
 
 
 class SendInstruction(Instruction):
     def __init__(self, send_value):
         super().__init__()
         self.send_value = send_value
 
     def run(self, script):
         super().run(script)
-        logging.debug("Send %s", repr(self.send_value))
+        logger.debug("Send %s", repr(self.send_value))
         self.receive_value = self.send_value
 
         # Check for special character
-        if "\\" in self.send_value:
-            self.receive_value = [character if character !=
-                                  '\\' else character+'\\' for character in list(self.send_value)]
+        self.receive_value = [re.escape(c) for c in list(self.send_value)]
 
         # Write intruction
-        for send_character, receive_character in zip(self.send_value, self.receive_value):
+        for send_character, receive_character in zip(
+            self.send_value, self.receive_value
+        ):
             if script.standart_deviation is None:
                 time.sleep(script.delay)
             else:
-                time.sleep(abs(random.gauss(
-                    script.delay, script.standart_deviation)))
+                time.sleep(abs(random.gauss(script.delay, script.standart_deviation)))
             script.process.send(str(send_character))
             script.process.expect(str(receive_character))
 
         # End instruction
         if script.standart_deviation is None:
             time.sleep(script.delay)
         else:
-            time.sleep(abs(random.gauss(
-                script.delay, script.standart_deviation)))
+            time.sleep(abs(random.gauss(script.delay, script.standart_deviation)))
 
 
 class SendCharacterInstruction(Instruction):
     def __init__(self, send_value):
         super().__init__()
         self.send_value = send_value
 
     def run(self, script):
         super().run(script)
-        logging.debug("Send '%s'", self.send_value)
+        logger.debug("Send '%s'", self.send_value)
         script.process.send(self.send_value)
 
 
 class SendShellInstruction(SendInstruction):
-
     def __init__(self, command):
         super().__init__(command)
 
     def run(self, script):
         super().run(script)
-        logging.debug("Send '\\n'")
+        logger.debug("Send '\\n'")
         script.process.send("\n")
 
 
 class SendControlInstruction(Instruction):
     def __init__(self, control):
         super().__init__()
         self.control = control
 
     def run(self, script):
         super().run(script)
-        logging.debug("Send ctrl+%s", self.control)
+        logger.debug("Send ctrl+%s", self.control)
         script.process.sendcontrol(self.control)
 
 
 class SendArrowInstruction(Instruction):
-
-    KEY_UP = '\x1b[A'
-    KEY_DOWN = '\x1b[B'
-    KEY_RIGHT = '\x1b[C'
-    KEY_LEFT = '\x1b[D'
+    KEY_UP = "\x1b[A"
+    KEY_DOWN = "\x1b[B"
+    KEY_RIGHT = "\x1b[C"
+    KEY_LEFT = "\x1b[D"
 
     def __init__(self, send, num, enter=False):
         super().__init__()
         self.mapping = dict()
-        self.mapping["up"] = '\x1b[A'
-        self.mapping["down"] = '\x1b[B'
-        self.mapping["right"] = '\x1b[C'
-        self.mapping["left"] = '\x1b[D'
+        self.mapping["up"] = "\x1b[A"
+        self.mapping["down"] = "\x1b[B"
+        self.mapping["right"] = "\x1b[C"
+        self.mapping["left"] = "\x1b[D"
         self.send = send
         self.num = num
         self.enter = enter
 
     def run(self, script):
         super().run(script)
-        logging.debug("Send %s arrow %i times", self.send, self.num)
+        logger.debug("Send %s arrow %i times", self.send, self.num)
         for _ in range(self.num):
             if script.standart_deviation is None:
                 time.sleep(script.delay)
             else:
-                time.sleep(abs(random.gauss(
-                    script.delay, script.standart_deviation)))
+                time.sleep(abs(random.gauss(script.delay, script.standart_deviation)))
             if self.enter:
                 script.process.sendline(self.mapping[self.send])
             else:
                 script.process.send(self.mapping[self.send])
```

### Comparing `asciinema-automation-0.1.2/asciinema_automation/script.py` & `asciinema-automation-0.1.3/asciinema_automation/script.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,157 +1,174 @@
 import codecs
+import logging
 import pathlib
 import re
 import time
+
 import pexpect
-import logging
-from asciinema_automation.instruction import ChangeDelayInstruction, ChangeWaitInstruction, ExpectInstruction, SendInstruction, SendShellInstruction, SendControlInstruction, SendArrowInstruction, SendCharacterInstruction
+
+from asciinema_automation.instruction import (
+    ChangeDelayInstruction,
+    ChangeWaitInstruction,
+    ExpectInstruction,
+    SendArrowInstruction,
+    SendCharacterInstruction,
+    SendControlInstruction,
+    SendInstruction,
+    SendShellInstruction,
+)
 
 # To read escaped character from instructions
 # https://stackoverflow.com/a/24519338/5913047
-ESCAPE_SEQUENCE_RE = re.compile(r'''
+ESCAPE_SEQUENCE_RE = re.compile(
+    r"""
     ( \\U........      # 8-digit hex escapes
     | \\u....          # 4-digit hex escapes
     | \\x..            # 2-digit hex escapes
     | \\[0-7]{1,3}     # Octal escapes
     | \\N\{[^}]+\}     # Unicode characters by name
     | \\[\\'"abfnrtv]  # Single-character escapes
-    )''', re.UNICODE | re.VERBOSE)
+    )""",
+    re.UNICODE | re.VERBOSE,
+)
+
+logger = logging.getLogger(__name__)
 
 
 def decode_escapes(s):
     def decode_match(match):
-        return codecs.decode(match.group(0), 'unicode-escape')
+        return codecs.decode(match.group(0), "unicode-escape")
 
     return ESCAPE_SEQUENCE_RE.sub(decode_match, s)
 
 
 class Script:
-
-    def __init__(self, inputfile: pathlib.Path, outputfile: pathlib.Path, asciinema_arguments: str, wait, delay, standart_deviation, timeout):
-
+    def __init__(
+        self,
+        inputfile: pathlib.Path,
+        outputfile: pathlib.Path,
+        asciinema_arguments: str,
+        wait,
+        delay,
+        standart_deviation,
+        timeout,
+    ):
         # Set members from arguments
         self.inputfile = inputfile
         self.outputfile = outputfile
         self.asciinema_arguments = asciinema_arguments
-        self.delay = delay/1000.
-        self.wait = wait/1000.
-        self.standart_deviation = standart_deviation/1000.
+        self.delay = delay / 1000.0
+        self.wait = wait / 1000.0
+        self.standart_deviation = standart_deviation / 1000.0
 
         # Default values for data members
         self.expected = "\n"
         self.send = "\n"
 
         # Create data members
         self.instructions = []
         self.process = None
 
         # Compile regex
-        wait_time_regex = re.compile(r'^#\$ wait (\d*)(?!\S)')
-        delay_time_regex = re.compile(r'^#\$ delay (\d*)(?!\S)')
-        sendcontrol_command_regex = re.compile(
-            r'^#\$ sendcontrol ([a-z])(?!\S)')
-        sendcharacter_command_regex = re.compile(
-            r'^#\$ sendcharacter (.*)(?!\S)')
-        expect_regex = re.compile(
-            r'^#\$ expect (.*)(?!\S)')
-        send_regex = re.compile(
-            r'^#\$ send (.*)(?!\S)')
+        wait_time_regex = re.compile(r"^#\$ wait (\d*)(?!\S)")
+        delay_time_regex = re.compile(r"^#\$ delay (\d*)(?!\S)")
+        sendcontrol_command_regex = re.compile(r"^#\$ sendcontrol ([a-z])(?!\S)")
+        sendcharacter_command_regex = re.compile(r"^#\$ sendcharacter (.*)(?!\S)")
+        expect_regex = re.compile(r"^#\$ expect (.*)(?!\S)")
+        send_regex = re.compile(r"^#\$ send (.*)(?!\S)")
         arrow_command_regex = re.compile(
-            r'^#\$ sendarrow (down|up|left|right)(?:\s([\d]+))?(?!\S)')
+            r"^#\$ sendarrow (down|up|left|right)(?:\s([\d]+))?(?!\S)"
+        )
         arrow_sendline_command_regex = re.compile(
-            r'^#\$ sendlinearrow (down|up|left|right)(?:\s([\d]+))?(?!\S)')
+            r"^#\$ sendlinearrow (down|up|left|right)(?:\s([\d]+))?(?!\S)"
+        )
 
         # Read script
         with open(inputfile) as f:
             lines = [line.rstrip() for line in f.readlines() if line.strip()]
 
         previous_line = ""
         for line in lines:
             if line.startswith("#$ wait"):
                 wait_time = wait_time_regex.search(line, 0).group(1)
-                self.instructions.append(
-                    ChangeWaitInstruction(int(wait_time)/1000))
+                self.instructions.append(ChangeWaitInstruction(int(wait_time) / 1000))
             elif line.startswith("#$ delay"):
                 delay_time = delay_time_regex.search(line, 0).group(1)
-                self.instructions.append(
-                    ChangeDelayInstruction(int(delay_time)/1000))
+                self.instructions.append(ChangeDelayInstruction(int(delay_time) / 1000))
             elif line.startswith("#$ sendcontrol"):
-                sendcontrol_command = sendcontrol_command_regex.search(
-                    line, 0).group(1)
-                self.instructions.append(
-                    SendControlInstruction(sendcontrol_command))
+                sendcontrol_command = sendcontrol_command_regex.search(line, 0).group(1)
+                self.instructions.append(SendControlInstruction(sendcontrol_command))
             elif line.startswith("#$ sendcharacter"):
                 sendcharacter_command = sendcharacter_command_regex.search(
-                    line, 0).group(1)
+                    line, 0
+                ).group(1)
                 self.instructions.append(
-                    SendCharacterInstruction(sendcharacter_command))
+                    SendCharacterInstruction(sendcharacter_command)
+                )
             elif line.startswith("#$ sendarrow"):
-                arrow_command = arrow_command_regex.search(
-                    line, 0).group(1)
-                arrow_num = arrow_command_regex.search(
-                    line, 0).group(2)
+                arrow_command = arrow_command_regex.search(line, 0).group(1)
+                arrow_num = arrow_command_regex.search(line, 0).group(2)
                 if arrow_num is None:
                     arrow_num = 1
                 self.instructions.append(
-                    SendArrowInstruction(arrow_command, int(arrow_num), False))
+                    SendArrowInstruction(arrow_command, int(arrow_num), False)
+                )
             elif line.startswith("#$ sendlinearrow"):
-                arrow_command = arrow_sendline_command_regex.search(
-                    line, 0).group(1)
-                arrow_num = arrow_sendline_command_regex.search(
-                    line, 0).group(2)
+                arrow_command = arrow_sendline_command_regex.search(line, 0).group(1)
+                arrow_num = arrow_sendline_command_regex.search(line, 0).group(2)
                 if arrow_num is None:
                     arrow_num = 1
                 self.instructions.append(
-                    SendArrowInstruction(arrow_command, int(arrow_num), True))
+                    SendArrowInstruction(arrow_command, int(arrow_num), True)
+                )
             elif line.startswith("#$ expect"):
                 expect_value = ""
                 if expect_regex.search(line, 0) is not None:
                     expect_value = expect_regex.search(line, 0).group(1)
                     expect_value = decode_escapes(expect_value)
-                self.instructions.append(
-                    ExpectInstruction(expect_value, timeout))
+                self.instructions.append(ExpectInstruction(expect_value, timeout))
             elif line.startswith("#$ send"):
                 send_value = ""
                 if send_regex.search(line, 0) is not None:
                     send_value = send_regex.search(line, 0).group(1)
                     send_value = decode_escapes(send_value)
                 self.instructions.append(SendInstruction(send_value))
             elif line.startswith("#"):
                 pass
             else:
                 if line.endswith("\\"):
-                    previous_line += line+"\n"
+                    previous_line += line + "\n"
                 else:
-                    self.instructions.append(
-                        SendShellInstruction(previous_line+line))
+                    self.instructions.append(SendShellInstruction(previous_line + line))
                     previous_line = ""
 
     def execute(self):
-        spawn_command = "asciinema rec " + \
-            str(self.outputfile) + " "+self.asciinema_arguments
-        logging.info(spawn_command)
-        self.process = pexpect.spawn(spawn_command,
-                                     logfile=None)
+        spawn_command = (
+            "asciinema rec " + str(self.outputfile) + " " + self.asciinema_arguments
+        )
+        logger.info(spawn_command)
+        self.process = pexpect.spawn(spawn_command, logfile=None)
 
         self.process.expect("\n")
-        logging.debug(self.process.before)
-        if not ("recording asciicast to test.cast" in str(self.process.before)):
+        logger.debug(self.process.before)
+        if not (
+            "recording asciicast to " + str(self.outputfile) in str(self.process.before)
+        ):
             self.process.expect(pexpect.EOF)
             self.process.close()
-            logging.debug("Exit status:"+str(self.process.exitstatus))
-            logging.debug("Signal status:" + str(self.process.signalstatus))
+            logger.debug("Exit status:" + str(self.process.exitstatus))
+            logger.debug("Signal status:" + str(self.process.signalstatus))
         else:
             self.process.expect("\n")
-            logging.debug(self.process.before)
-            logging.debug(self.process.after)
-            logging.info("Start reading instructions")
+            logger.debug(self.process.before)
+            logger.debug(self.process.after)
+            logger.info("Start reading instructions")
             for instruction in self.instructions:
                 time.sleep(self.wait)
                 instruction.run(self)
             time.sleep(self.wait)
-            logging.info("Finished reading instructions")
-            self.process.sendcontrol('d')
+            logger.info("Finished reading instructions")
+            self.process.sendcontrol("d")
             self.process.expect(pexpect.EOF)
             self.process.close()
-            logging.debug("Exit status:"+str(self.process.exitstatus))
-            logging.debug("Signal status:" + str(self.process.signalstatus))
+            logger.debug("Exit status:" + str(self.process.exitstatus))
+            logger.debug("Signal status:" + str(self.process.signalstatus))
```

### Comparing `asciinema-automation-0.1.2/asciinema_automation.egg-info/PKG-INFO` & `asciinema-automation-0.1.3/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,38 @@
 Metadata-Version: 2.1
 Name: asciinema-automation
-Version: 0.1.2
+Version: 0.1.3
 Summary: CLI utility to automate asciinema
-Home-page: https://github.com/PierreMarchand20/asciinema_automation
-Author: Pierre Marchand
-License: MIT
+Author-email: Pierre Marchand <test@test.com>
+License: MIT License
+Project-URL: Homepage, https://github.com/PierreMarchand20/asciinema_automation
+Project-URL: Bug Tracker, https://github.com/PierreMarchand20/asciinema_automation/issues
 Keywords: asciinema
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: MacOS
+Classifier: Operating System :: Unix
+Requires-Python: >=3.7
+Description-Content-Type: text/x-rst
+Provides-Extra: dev
+Provides-Extra: test
 License-File: LICENSE
 
 asciinema-automation
 ####################
 
 .. image:: https://badge.fury.io/py/asciinema-automation.svg
     :target: https://badge.fury.io/py/asciinema-automation
 
+.. image:: https://github.com/PierreMarchand20/asciinema_automation/actions/workflows/CI.yml/badge.svg
+   :target: https://github.com/PierreMarchand20/asciinema_automation/actions/workflows/CI.yml
+   
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+   :target: https://github.com/psf/black
+
 Asciinema-Automation is a Python package which provides a small CLI utility to automate `asciinema <https://asciinema.org>`_ recordings. The only dependencies are asciinema and `Pexpect <https://pexpect.readthedocs.io/>`_.
 
 Example
 -------
 
 .. image:: https://raw.githubusercontent.com/PierreMarchand20/asciinema_automation/main/demo.gif
     :alt: Demo
```

