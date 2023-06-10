# Comparing `tmp/pud-1.0.2-py3-none-any.whl.zip` & `tmp/pud-1.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,16 @@
-Zip file size: 6374 bytes, number of entries: 12
+Zip file size: 7314 bytes, number of entries: 14
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-07 14:07 pud/__init__.py
 -rw-rw-rw-  2.0 fat      100 b- defN 23-Jun-09 12:58 pud/__main__.py
--rw-rw-rw-  2.0 fat     8009 b- defN 23-Jun-09 11:22 pud/app.py
+-rw-rw-rw-  2.0 fat     7365 b- defN 23-Jun-10 08:51 pud/app.py
 -rw-rw-rw-  2.0 fat      779 b- defN 23-Jun-09 08:33 pud/entity.py
--rw-rw-rw-  2.0 fat      285 b- defN 23-Jun-08 15:03 pud/main.py
+-rw-rw-rw-  2.0 fat      285 b- defN 23-Jun-10 06:16 pud/main.py
 -rw-rw-rw-  2.0 fat      545 b- defN 23-Jun-09 12:58 pud/options.py
--rw-rw-rw-  2.0 fat     1070 b- defN 23-Jun-09 13:02 pud-1.0.2.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      997 b- defN 23-Jun-09 13:02 pud-1.0.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-09 13:02 pud-1.0.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       39 b- defN 23-Jun-09 13:02 pud-1.0.2.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat        4 b- defN 23-Jun-09 13:02 pud-1.0.2.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      868 b- defN 23-Jun-09 13:02 pud-1.0.2.dist-info/RECORD
-12 files, 12788 bytes uncompressed, 4934 bytes compressed:  61.4%
+-rw-rw-rw-  2.0 fat       42 b- defN 23-Jun-10 08:45 pud/handlers/__init__.py
+-rw-rw-rw-  2.0 fat     1540 b- defN 23-Jun-10 08:50 pud/handlers/directory.py
+-rw-rw-rw-  2.0 fat     1070 b- defN 23-Jun-10 09:00 pud-1.0.3.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1157 b- defN 23-Jun-10 09:00 pud-1.0.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-10 09:00 pud-1.0.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       39 b- defN 23-Jun-10 09:00 pud-1.0.3.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat        4 b- defN 23-Jun-10 09:00 pud-1.0.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1030 b- defN 23-Jun-10 09:00 pud-1.0.3.dist-info/RECORD
+14 files, 14048 bytes uncompressed, 5624 bytes compressed:  60.0%
```

## zipnote {}

```diff
@@ -12,26 +12,32 @@
 
 Filename: pud/main.py
 Comment: 
 
 Filename: pud/options.py
 Comment: 
 
-Filename: pud-1.0.2.dist-info/LICENSE
+Filename: pud/handlers/__init__.py
 Comment: 
 
-Filename: pud-1.0.2.dist-info/METADATA
+Filename: pud/handlers/directory.py
 Comment: 
 
-Filename: pud-1.0.2.dist-info/WHEEL
+Filename: pud-1.0.3.dist-info/LICENSE
 Comment: 
 
-Filename: pud-1.0.2.dist-info/entry_points.txt
+Filename: pud-1.0.3.dist-info/METADATA
 Comment: 
 
-Filename: pud-1.0.2.dist-info/top_level.txt
+Filename: pud-1.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: pud-1.0.2.dist-info/RECORD
+Filename: pud-1.0.3.dist-info/entry_points.txt
+Comment: 
+
+Filename: pud-1.0.3.dist-info/top_level.txt
+Comment: 
+
+Filename: pud-1.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pud/app.py

```diff
@@ -1,12 +1,14 @@
-import os
+from __future__ import annotations
+
 import curses
 from pathlib import Path
 
 from .entity import Entity, GoBack
+from .handlers import DirectoryExplorer
 
 
 KEY_UP = (curses.KEY_UP, 450, ord('w'))
 KEY_DOWN = (curses.KEY_DOWN, 456, ord('s'))
 ENTER = (curses.KEY_ENTER, ord('\n'), ord('\r'))
 SCROLL_UP = (65536,)
 SCROLL_DOWN = (2097152,)
@@ -28,49 +30,44 @@
 
     offset:
         The offset of the display screen from the top of the file.
 
     screen_idx:
         The index of the cursor on the screen.
 
-    cwd:
-        The current working directory.
+    explorer:
+        The directory handler.
 
     cursor_stack:
         The cursor stack used to 'remember' the past cursor placement before
-        entering a new directory. It is a tuple of 4 items.
-        (part, offset, index, screen_index)
+        entering a new directory. It is a tuple of 3 items.
+        (offset, index, screen_index)
 
-        `part` is the folder name.
         `offset` is the offset of the display screen from the top of the file list.
         `index` is the index of the cursor.
         `screen_index` is the index of the cursor on the screen.
 
-    files:
-        The list of files on the current working directory.
-
     screen:
         A curses window.
 
     coords:
         The coords of current file entries on the screen.
     """
 
     screen: "curses._CursesWindow"
-    coords: list[tuple[str, int, int]]
+    coords: list[tuple[str, range, int]]
 
     def __init__(self, cursor: str, keep_cursor_state: bool):
         self.cursor = cursor.strip()
         self.keep_cursor_state = keep_cursor_state
         self.idx = 0
         self.offset = 0
         self.screen_idx = 0
-        self.cwd = Path().cwd()
-        self.cursor_stack = [(part, 0, 0, 0) for part in self.cwd.parts]
-        self.files = self.get_files()
+        self.explorer = DirectoryExplorer(Path().cwd())
+        self.cursor_stack = [(0, 0, 0) for _ in self.explorer.cwd.parts]
 
     def __call__(self, screen: "curses._CursesWindow"):
         curses.curs_set(0)
         curses.mousemask(-1)
         screen.keypad(True)
         self.screen = screen
 
@@ -86,42 +83,36 @@
         self.offset = 0
         self.screen_idx = 0
 
     def get_files(self) -> tuple[tuple[int, GoBack | Entity], ...]:
         """Gets all the files from the current working directory and stores it in a list."""
 
         back = [GoBack()]
-        ret = []
+        files = self.explorer.list_files()
 
-        try:
-            files = list(self.cwd.iterdir())
-        except PermissionError:
+        if files is None:
+            files = []
             message = "Permission Denied."
             maxy, maxx = self.screen.getmaxyx()
-            files = []
-
             self.screen.addstr(maxy // 2, (maxx // 2) - (len(message) // 2), message)
 
-        for file in files:
-            ret.append(Entity(file.name, is_file=file.is_file()))
-
-        ret = sorted(ret, key=lambda f: f.is_file)
+        ret = sorted(files, key=lambda f: f.is_file)
         return tuple(enumerate(back + ret))
 
     def draw_screen(self) -> None:
         """Draws all the folders/files into the screen."""
 
         self.screen.clear()
 
         y = 0
         self.maxy, maxx = self.screen.getmaxyx()
         self.maxy -= 4
         files = self.get_files()
 
-        self.screen.addstr(y, 1, f"Current Directory: {self.cwd}")
+        self.screen.addstr(y, 1, f"Current Directory: {self.explorer.cwd}")
         y += 1
         self.screen.addstr(y, 1, "Press CTRL + C or Esc or q to exit.")
         y += 1
 
         files = files[self.offset:self.maxy + self.offset]
         coords = []
 
@@ -135,15 +126,15 @@
 
             self.screen.addnstr(y, 1, file_display, maxx - 2)
             coords.append((file.name, range(1, len(file_display)), y))
 
         self.coords = coords
         self.screen.refresh()
 
-    def get_key(self) -> str | int:
+    def get_key(self) -> int:
         """Returns a pressed key."""
 
         return self.screen.getch()
 
     def move_up(self) -> None:
         """Adjusts the indexes and offset if possible.
 
@@ -161,15 +152,15 @@
 
     def move_down(self) -> None:
         """Adjusts the indexes and offsets if possible.
 
         This makes the cursor go down.
         """
 
-        if self.idx < len(self.files) - 1:
+        if self.idx < len(self.get_files()) - 1:
             self.idx += 1
 
             if self.screen_idx >= self.maxy - 1:
                 self.offset += 1
 
             if self.screen_idx < self.maxy - 1:
                 self.screen_idx += 1
@@ -178,20 +169,14 @@
         """Pops the cursor stack and returns it."""
 
         if len(self.cursor_stack) > 1:
             return self.cursor_stack.pop()
 
         return self.cursor_stack[0]
 
-    def refresh_cwd(self):
-        """Refreshes the current working directory."""
-
-        self.cwd = Path().cwd()
-        self.files = self.get_files()
-
     def execute_by_key(self, key: int) -> None:
         """Executes an action based on the key.
 
         key:
             The key returned by `get_key`.
         """
 
@@ -202,80 +187,66 @@
             self.move_up()
 
         if key in KEY_DOWN:
             self.move_down()
 
         if key in ENTER:
             if self.idx == 0:
-                selected = self.cwd.parent
-
-                os.chdir(selected)
+                self.explorer.go_back()
 
                 if self.keep_cursor_state:
-                    _, offset, index, screen_index = self.pop_cursor_stack()
+                    offset, index, screen_index = self.pop_cursor_stack()
 
                     self.offset = offset
                     self.idx = index
                     self.screen_idx = screen_index
 
             else:
-                selected = self.cwd / str(self.files[self.idx][1].name)
+                files = self.get_files()
+                selected = files[self.idx][1].name
+
+                entered = self.explorer.enter(selected)
 
-                if selected.is_file():
+                if not entered:
                     return
 
-                state = (None, None, None, None)
+                state = (0, 0, 0)
 
                 if self.keep_cursor_state:
                     state = (
-                        self.cwd.name,
                         self.offset,
                         self.idx,
                         self.screen_idx
                     )
 
                 self.cursor_stack.append(state)
-
-                os.chdir(selected)
-
                 self.reset_state()
 
-        self.refresh_cwd()
-
     def handle_mouse_event(self) -> None:
         """Handles a mouse event."""
 
-        clicked = None
         _, x, y, _, bstate = curses.getmouse()
 
         is_double_click = bstate & curses.BUTTON1_DOUBLE_CLICKED
 
         if is_double_click:
             for name, c_x, c_y in self.coords:
                 # Check if the coordinates clicked
                 # matches any of the folder coordinates on
                 # the screen.
                 if not (x in c_x and y == c_y):
                     continue
 
                 if name == "Back":
-                    clicked = self.cwd.parent
+                    self.explorer.go_back()
                     break
 
-                clicked = self.cwd / name
-
-                if clicked.is_file():
-                    return
-
+                self.explorer.enter(name)
                 self.reset_state()
 
-            if clicked:
-                os.chdir(clicked)
-                self.refresh_cwd()
-
         if bstate in SCROLL_UP:
             self.move_up()
 
         if bstate in SCROLL_DOWN:
             self.move_down()
 
     def _run(self):
```

## Comparing `pud-1.0.2.dist-info/LICENSE` & `pud-1.0.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pud-1.0.2.dist-info/METADATA` & `pud-1.0.3.dist-info/METADATA`

 * *Files 9% similar despite different names*

```diff
@@ -1,30 +1,40 @@
 Metadata-Version: 2.1
 Name: pud
-Version: 1.0.2
+Version: 1.0.3
 Summary: A command-line tool for navigating directories.
 Home-page: https://github.com/Jedddy/pud
 Author: Jedddy
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: windows-curses (==2.3.1) ; sys_platform == "win32"
 
-
 Pud
 ===
+
+![PyPI](https://img.shields.io/pypi/v/pud)
+![PyPI - Downloads](https://img.shields.io/pypi/dd/pud)
+
+
 Pud is a mini command-line tool to navigate directories.
 
 Installation
 ===
+PIP:
+```
+pip install pud
+```
+
+GIT (Dev Version):
 ```
 git clone https://github.com/Jedddy/pud.git
 
 python setup.py install
 ```
 
 Usage
```

## Comparing `pud-1.0.2.dist-info/RECORD` & `pud-1.0.3.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 pud/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pud/__main__.py,sha256=X86mONAr_BaFTmbpJgWB4SAQ3SW7AICSzrbLkyDJob0,100
-pud/app.py,sha256=GjfSHi-yongnY3533wkqugTvyfvYJq9PUqTgBaxFnKs,8009
+pud/app.py,sha256=ODBDVIUmY0rTxER5JgFXbbVwOlBnJ3j_FZe427Bl9Mc,7365
 pud/entity.py,sha256=T_JEtQdEZEo3vDEx5pYj6q4dwXsSFjSw2tyLzo60XUM,779
 pud/main.py,sha256=YajWrXJIvtbQY4wM1EqyfzrUk0eMHymWB0CW7k3xbc0,285
 pud/options.py,sha256=NHGSE_KIl9gvUKbj1wlVVsVR_d8kuQy5n3T6W--1nZ8,545
-pud-1.0.2.dist-info/LICENSE,sha256=v0PHLuz3Fx7aA5ulQVj5i2V9OObeeStZrZ1ZDb65ChE,1070
-pud-1.0.2.dist-info/METADATA,sha256=xAtmEVJv2Ha00fzkMPO4ArcgdLYut2KEop9EnJhAV8o,997
-pud-1.0.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-pud-1.0.2.dist-info/entry_points.txt,sha256=ZICpIyMhM1UpeUR8s2Lt4pe9BBo7XHAUwBDPodR6Ltw,39
-pud-1.0.2.dist-info/top_level.txt,sha256=bzTwibMohuSeyMWwBz7PqNY87HyQ-ywUmdG_wog_UV8,4
-pud-1.0.2.dist-info/RECORD,,
+pud/handlers/__init__.py,sha256=Grm4Xu5XbBij463ZRqW3rJGffsYOH2bS_8pNKCzDxww,42
+pud/handlers/directory.py,sha256=FE-UROTFsA_zjdfb7Han24ZwTYj_5qIOtmpv4P9miuM,1540
+pud-1.0.3.dist-info/LICENSE,sha256=v0PHLuz3Fx7aA5ulQVj5i2V9OObeeStZrZ1ZDb65ChE,1070
+pud-1.0.3.dist-info/METADATA,sha256=lA9Z7WNypS2hc4AqUyUVF4RwWW-YmZLUFNNDwEmsZFs,1157
+pud-1.0.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+pud-1.0.3.dist-info/entry_points.txt,sha256=ZICpIyMhM1UpeUR8s2Lt4pe9BBo7XHAUwBDPodR6Ltw,39
+pud-1.0.3.dist-info/top_level.txt,sha256=bzTwibMohuSeyMWwBz7PqNY87HyQ-ywUmdG_wog_UV8,4
+pud-1.0.3.dist-info/RECORD,,
```

