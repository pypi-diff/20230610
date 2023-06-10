# Comparing `tmp/rp2040_pio_emulator-0.80.0.tar.gz` & `tmp/rp2040_pio_emulator-0.81.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rp2040_pio_emulator-0.80.0.tar", max compression
+gzip compressed data, was "rp2040_pio_emulator-0.81.0.tar", max compression
```

## Comparing `rp2040_pio_emulator-0.80.0.tar` & `rp2040_pio_emulator-0.81.0.tar`

### file list

```diff
@@ -1,16 +1,19 @@
--rw-r--r--   0        0        0    11357 2023-04-16 12:08:06.174736 rp2040_pio_emulator-0.80.0/LICENSE
--rw-r--r--   0        0        0     2860 2023-04-16 12:08:06.174736 rp2040_pio_emulator-0.80.0/README.md
--rw-r--r--   0        0        0      755 2023-04-16 12:08:06.182736 rp2040_pio_emulator-0.80.0/pioemu/__init__.py
--rw-r--r--   0        0        0     2257 2023-04-16 12:08:06.182736 rp2040_pio_emulator-0.80.0/pioemu/conditions.py
--rw-r--r--   0        0        0     6292 2023-04-16 12:08:06.182736 rp2040_pio_emulator-0.80.0/pioemu/emulation.py
--rw-r--r--   0        0        0     1028 2023-04-16 12:08:06.182736 rp2040_pio_emulator-0.80.0/pioemu/instruction.py
--rw-r--r--   0        0        0     9794 2023-04-16 12:08:06.182736 rp2040_pio_emulator-0.80.0/pioemu/instruction_decoder.py
--rw-r--r--   0        0        0      682 2023-04-16 12:08:06.182736 rp2040_pio_emulator-0.80.0/pioemu/instructions/__init__.py
--rw-r--r--   0        0        0     1472 2023-04-16 12:08:06.182736 rp2040_pio_emulator-0.80.0/pioemu/instructions/pull.py
--rw-r--r--   0        0        0     1260 2023-04-16 12:08:06.182736 rp2040_pio_emulator-0.80.0/pioemu/instructions/push.py
--rw-r--r--   0        0        0     4658 2023-04-16 12:08:06.182736 rp2040_pio_emulator-0.80.0/pioemu/primitive_operations.py
--rw-r--r--   0        0        0     3795 2023-04-16 12:08:06.182736 rp2040_pio_emulator-0.80.0/pioemu/shift_register.py
--rw-r--r--   0        0        0     1251 2023-04-16 12:08:06.182736 rp2040_pio_emulator-0.80.0/pioemu/state.py
--rw-r--r--   0        0        0      672 2023-04-16 12:08:06.182736 rp2040_pio_emulator-0.80.0/pyproject.toml
--rw-r--r--   0        0        0     3555 1970-01-01 00:00:00.000000 rp2040_pio_emulator-0.80.0/setup.py
--rw-r--r--   0        0        0     3465 1970-01-01 00:00:00.000000 rp2040_pio_emulator-0.80.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-16 12:08:06.174736 rp2040_pio_emulator-0.81.0/LICENSE
+-rw-r--r--   0        0        0     3300 2023-06-10 14:33:35.641924 rp2040_pio_emulator-0.81.0/README.md
+-rw-r--r--   0        0        0      755 2023-05-26 05:21:56.326167 rp2040_pio_emulator-0.81.0/pioemu/__init__.py
+-rw-r--r--   0        0        0     2257 2023-05-26 05:21:56.326167 rp2040_pio_emulator-0.81.0/pioemu/conditions.py
+-rw-r--r--   0        0        0     6416 2023-06-10 14:39:23.565575 rp2040_pio_emulator-0.81.0/pioemu/emulation.py
+-rw-r--r--   0        0        0     1028 2023-05-26 05:21:56.326167 rp2040_pio_emulator-0.81.0/pioemu/instruction.py
+-rw-r--r--   0        0        0     9794 2023-05-26 05:21:56.326167 rp2040_pio_emulator-0.81.0/pioemu/instruction_decoder.py
+-rw-r--r--   0        0        0      682 2023-05-26 05:21:56.330167 rp2040_pio_emulator-0.81.0/pioemu/instructions/__init__.py
+-rw-r--r--   0        0        0      370 2023-06-10 13:22:34.978550 rp2040_pio_emulator-0.81.0/pioemu/instructions/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1507 2023-06-10 13:22:34.978550 rp2040_pio_emulator-0.81.0/pioemu/instructions/__pycache__/pull.cpython-311.pyc
+-rw-r--r--   0        0        0     1382 2023-06-10 13:22:34.978550 rp2040_pio_emulator-0.81.0/pioemu/instructions/__pycache__/push.cpython-311.pyc
+-rw-r--r--   0        0        0     1472 2023-05-26 05:21:56.330167 rp2040_pio_emulator-0.81.0/pioemu/instructions/pull.py
+-rw-r--r--   0        0        0     1260 2023-05-26 05:21:56.330167 rp2040_pio_emulator-0.81.0/pioemu/instructions/push.py
+-rw-r--r--   0        0        0     4658 2023-05-26 05:21:56.330167 rp2040_pio_emulator-0.81.0/pioemu/primitive_operations.py
+-rw-r--r--   0        0        0     3795 2023-05-26 05:21:56.330167 rp2040_pio_emulator-0.81.0/pioemu/shift_register.py
+-rw-r--r--   0        0        0     1251 2023-05-26 05:21:56.330167 rp2040_pio_emulator-0.81.0/pioemu/state.py
+-rw-r--r--   0        0        0      672 2023-05-26 05:21:56.330167 rp2040_pio_emulator-0.81.0/pyproject.toml
+-rw-r--r--   0        0        0     4002 1970-01-01 00:00:00.000000 rp2040_pio_emulator-0.81.0/setup.py
+-rw-r--r--   0        0        0     3905 1970-01-01 00:00:00.000000 rp2040_pio_emulator-0.81.0/PKG-INFO
```

### Comparing `rp2040_pio_emulator-0.80.0/LICENSE` & `rp2040_pio_emulator-0.81.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rp2040_pio_emulator-0.80.0/README.md` & `rp2040_pio_emulator-0.81.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -22,14 +22,20 @@
 
 generator = emulate(program, stop_when=lambda _, state: state.x_register < 0)
 
 for before, after in generator:
   print(f"X register: {before.x_register} -> {after.x_register}")
 ```
 
+## Documentation
+A [Tour of pioemu](./docs/Tour%20of%20pioemu.md) provides a more detailed explanation than the
+[Quick Start Guide](./docs/Quick%20Start%20Guide.md) offers. However, if neither of these provides
+you with the information that you seek then please consider creating a
+[new issue](https://github.com/NathanY3G/rp2040-pio-emulator/issues) - thanks!
+
 ## Additional Examples
 Some additional examples include:
 
 1. Visualisation of square wave program using Jupyter Notebooks within the `examples/` directory.
 
 1. TDD example for the Pimoroni Blinkt! within the `examples/` directory.
 
@@ -59,7 +65,8 @@
 1. Pin-sets do not wrap after GPIO 31.
 
 1. No direct support for the concurrent running of multiple PIO programs;
    a single State Machine is emulated and not an entire PIO block.
 
 ## Thanks To
 * [aaronjamt](https://github.com/aaronjamt) for contributing features and fixes.
+* [winnylourson](https://github.com/winnylourson) for contributing a bug fix.
```

### Comparing `rp2040_pio_emulator-0.80.0/pioemu/__init__.py` & `rp2040_pio_emulator-0.81.0/pioemu/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,13 +7,13 @@
 #    https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-__version__ = "0.80.0"
+__version__ = "0.81.0"
 
 from .conditions import clock_cycles_reached
 from .emulation import emulate
 from .shift_register import ShiftRegister
 from .state import State
```

### Comparing `rp2040_pio_emulator-0.80.0/pioemu/conditions.py` & `rp2040_pio_emulator-0.81.0/pioemu/conditions.py`

 * *Files identical despite different names*

### Comparing `rp2040_pio_emulator-0.80.0/pioemu/emulation.py` & `rp2040_pio_emulator-0.81.0/pioemu/emulation.py`

 * *Files 3% similar despite different names*

```diff
@@ -76,18 +76,19 @@
     current_state = initial_state
     stalled = False
 
     while not stop_when(opcodes[current_state.program_counter], current_state):
         previous_state = current_state
 
         if input_source:
+            masked_values = current_state.pin_values & current_state.pin_directions
+            masked_input = input_source(current_state.clock) & ~current_state.pin_directions
             current_state = replace(
                 current_state,
-                pin_values=input_source(current_state.clock)
-                & ~current_state.pin_directions,
+                pin_values=masked_values | masked_input,
             )
 
         opcode = opcodes[current_state.program_counter]
 
         (side_set_value, delay_value) = _extract_delay_and_side_set_from_opcode(
             opcode, side_set_count
         )
```

### Comparing `rp2040_pio_emulator-0.80.0/pioemu/instruction.py` & `rp2040_pio_emulator-0.81.0/pioemu/instruction.py`

 * *Files identical despite different names*

### Comparing `rp2040_pio_emulator-0.80.0/pioemu/instruction_decoder.py` & `rp2040_pio_emulator-0.81.0/pioemu/instruction_decoder.py`

 * *Files identical despite different names*

### Comparing `rp2040_pio_emulator-0.80.0/pioemu/instructions/__init__.py` & `rp2040_pio_emulator-0.81.0/pioemu/instructions/__init__.py`

 * *Files identical despite different names*

### Comparing `rp2040_pio_emulator-0.80.0/pioemu/instructions/pull.py` & `rp2040_pio_emulator-0.81.0/pioemu/instructions/pull.py`

 * *Files identical despite different names*

### Comparing `rp2040_pio_emulator-0.80.0/pioemu/instructions/push.py` & `rp2040_pio_emulator-0.81.0/pioemu/instructions/push.py`

 * *Files identical despite different names*

### Comparing `rp2040_pio_emulator-0.80.0/pioemu/primitive_operations.py` & `rp2040_pio_emulator-0.81.0/pioemu/primitive_operations.py`

 * *Files identical despite different names*

### Comparing `rp2040_pio_emulator-0.80.0/pioemu/shift_register.py` & `rp2040_pio_emulator-0.81.0/pioemu/shift_register.py`

 * *Files identical despite different names*

### Comparing `rp2040_pio_emulator-0.80.0/pioemu/state.py` & `rp2040_pio_emulator-0.81.0/pioemu/state.py`

 * *Files identical despite different names*

### Comparing `rp2040_pio_emulator-0.80.0/pyproject.toml` & `rp2040_pio_emulator-0.81.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rp2040-pio-emulator"
-version = "0.80.0"
+version = "0.81.0"
 description = "RP2040 emulator for the testing and debugging of PIO programs"
 authors = ["Nathan Young"]
 license = "Apache-2.0"
 repository = "https://github.com/NathanY3G/rp2040-pio-emulator"
 readme = "README.md"
 packages = [
     { include = "pioemu" }
```

### Comparing `rp2040_pio_emulator-0.80.0/setup.py` & `rp2040_pio_emulator-0.81.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 ['pioemu', 'pioemu.instructions']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'rp2040-pio-emulator',
-    'version': '0.80.0',
+    'version': '0.81.0',
     'description': 'RP2040 emulator for the testing and debugging of PIO programs',
-    'long_description': '# Emulator for the PIO Blocks within the RP2040 Microcontroller (Python Edition)\n\n![Build Status](https://github.com/NathanY3G/rp2040-pio-emulator/actions/workflows/package-ci.yml/badge.svg) ![Coverage](./docs/images/coverage-badge.svg) [![PyPI](https://img.shields.io/pypi/v/rp2040-pio-emulator?color=informational)](https://pypi.org/project/rp2040-pio-emulator/)\n\n## Introduction\nAn emulator for the Programmable Input/Output (PIO) blocks that are present\nwithin the Raspberry Pi Foundation\'s RP2040 Microcontroller. It is designed\nto assist in the analysis of PIO programs and to help you by:\n\n* Enabling unit tests to be written.\n* Answering questions such as: How many clock cycles are being consumed?\n* Supporting the visualization of GPIO outputs over time.\n* Providing alternatives to debugging on real hardware, which can be time consuming.\n\n## Quick Start\nBelow is a slight variation of the example used within the [Quick Start Guide](./docs/Quick%20Start%20Guide.md).\n\n```python\nfrom pioemu import emulate\n\nprogram = [0xE029, 0x0041, 0x2080]  # Count down from 9 using X register\n\ngenerator = emulate(program, stop_when=lambda _, state: state.x_register < 0)\n\nfor before, after in generator:\n  print(f"X register: {before.x_register} -> {after.x_register}")\n```\n\n## Additional Examples\nSome additional examples include:\n\n1. Visualisation of square wave program using Jupyter Notebooks within the `examples/` directory.\n\n1. TDD example for the Pimoroni Blinkt! within the `examples/` directory.\n\n1. [pico-pio-examples](https://github.com/NathanY3G/pico-pio-examples)\n\n## Supported Instructions\n\nInstruction | Supported                         | Notes\n:-----------| :---------------------------------| :----\nJMP         | :heavy_check_mark:                | \nWAIT        | :heavy_check_mark: :warning:      | IRQ variant is not supported\nIN          | :heavy_check_mark:                |\nOUT         | :heavy_check_mark: :construction: | EXEC destination not implemented\nPUSH        | :heavy_check_mark:                | \nPULL        | :heavy_check_mark:                | \nMOV         | :heavy_check_mark: :construction: | Some variants and operations not implemented\nIRQ         | :heavy_multiplication_x:          |\nSET         | :heavy_check_mark:                |\n\n## Known Limitations\nThis software is under development and currently has limitations - the notable ones are:\n\n1. Not all of the available instructions are supported - please refer to the table above.\n\n1. No support for pin-sets associated with OUT, SET or IN; all pin numbers are with respect to GPIO 0.\n\n1. Pin-sets do not wrap after GPIO 31.\n\n1. No direct support for the concurrent running of multiple PIO programs;\n   a single State Machine is emulated and not an entire PIO block.\n\n## Thanks To\n* [aaronjamt](https://github.com/aaronjamt) for contributing features and fixes.\n',
+    'long_description': '# Emulator for the PIO Blocks within the RP2040 Microcontroller (Python Edition)\n\n![Build Status](https://github.com/NathanY3G/rp2040-pio-emulator/actions/workflows/package-ci.yml/badge.svg) ![Coverage](./docs/images/coverage-badge.svg) [![PyPI](https://img.shields.io/pypi/v/rp2040-pio-emulator?color=informational)](https://pypi.org/project/rp2040-pio-emulator/)\n\n## Introduction\nAn emulator for the Programmable Input/Output (PIO) blocks that are present\nwithin the Raspberry Pi Foundation\'s RP2040 Microcontroller. It is designed\nto assist in the analysis of PIO programs and to help you by:\n\n* Enabling unit tests to be written.\n* Answering questions such as: How many clock cycles are being consumed?\n* Supporting the visualization of GPIO outputs over time.\n* Providing alternatives to debugging on real hardware, which can be time consuming.\n\n## Quick Start\nBelow is a slight variation of the example used within the [Quick Start Guide](./docs/Quick%20Start%20Guide.md).\n\n```python\nfrom pioemu import emulate\n\nprogram = [0xE029, 0x0041, 0x2080]  # Count down from 9 using X register\n\ngenerator = emulate(program, stop_when=lambda _, state: state.x_register < 0)\n\nfor before, after in generator:\n  print(f"X register: {before.x_register} -> {after.x_register}")\n```\n\n## Documentation\nA [Tour of pioemu](./docs/Tour%20of%20pioemu.md) provides a more detailed explanation than the\n[Quick Start Guide](./docs/Quick%20Start%20Guide.md) offers. However, if neither of these provides\nyou with the information that you seek then please consider creating a\n[new issue](https://github.com/NathanY3G/rp2040-pio-emulator/issues) - thanks!\n\n## Additional Examples\nSome additional examples include:\n\n1. Visualisation of square wave program using Jupyter Notebooks within the `examples/` directory.\n\n1. TDD example for the Pimoroni Blinkt! within the `examples/` directory.\n\n1. [pico-pio-examples](https://github.com/NathanY3G/pico-pio-examples)\n\n## Supported Instructions\n\nInstruction | Supported                         | Notes\n:-----------| :---------------------------------| :----\nJMP         | :heavy_check_mark:                | \nWAIT        | :heavy_check_mark: :warning:      | IRQ variant is not supported\nIN          | :heavy_check_mark:                |\nOUT         | :heavy_check_mark: :construction: | EXEC destination not implemented\nPUSH        | :heavy_check_mark:                | \nPULL        | :heavy_check_mark:                | \nMOV         | :heavy_check_mark: :construction: | Some variants and operations not implemented\nIRQ         | :heavy_multiplication_x:          |\nSET         | :heavy_check_mark:                |\n\n## Known Limitations\nThis software is under development and currently has limitations - the notable ones are:\n\n1. Not all of the available instructions are supported - please refer to the table above.\n\n1. No support for pin-sets associated with OUT, SET or IN; all pin numbers are with respect to GPIO 0.\n\n1. Pin-sets do not wrap after GPIO 31.\n\n1. No direct support for the concurrent running of multiple PIO programs;\n   a single State Machine is emulated and not an entire PIO block.\n\n## Thanks To\n* [aaronjamt](https://github.com/aaronjamt) for contributing features and fixes.\n* [winnylourson](https://github.com/winnylourson) for contributing a bug fix.\n',
     'author': 'Nathan Young',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/NathanY3G/rp2040-pio-emulator',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `rp2040_pio_emulator-0.80.0/PKG-INFO` & `rp2040_pio_emulator-0.81.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rp2040-pio-emulator
-Version: 0.80.0
+Version: 0.81.0
 Summary: RP2040 emulator for the testing and debugging of PIO programs
 Home-page: https://github.com/NathanY3G/rp2040-pio-emulator
 License: Apache-2.0
 Keywords: rp2040,raspberry-pi-pico,testing,tdd,debugging
 Author: Nathan Young
 Requires-Python: >=3.10.10,<4.0.0
 Classifier: License :: OSI Approved :: Apache Software License
@@ -37,14 +37,20 @@
 
 generator = emulate(program, stop_when=lambda _, state: state.x_register < 0)
 
 for before, after in generator:
   print(f"X register: {before.x_register} -> {after.x_register}")
 ```
 
+## Documentation
+A [Tour of pioemu](./docs/Tour%20of%20pioemu.md) provides a more detailed explanation than the
+[Quick Start Guide](./docs/Quick%20Start%20Guide.md) offers. However, if neither of these provides
+you with the information that you seek then please consider creating a
+[new issue](https://github.com/NathanY3G/rp2040-pio-emulator/issues) - thanks!
+
 ## Additional Examples
 Some additional examples include:
 
 1. Visualisation of square wave program using Jupyter Notebooks within the `examples/` directory.
 
 1. TDD example for the Pimoroni Blinkt! within the `examples/` directory.
 
@@ -74,8 +80,9 @@
 1. Pin-sets do not wrap after GPIO 31.
 
 1. No direct support for the concurrent running of multiple PIO programs;
    a single State Machine is emulated and not an entire PIO block.
 
 ## Thanks To
 * [aaronjamt](https://github.com/aaronjamt) for contributing features and fixes.
+* [winnylourson](https://github.com/winnylourson) for contributing a bug fix.
```

