# Comparing `tmp/backgammon-1.0.0.tar.gz` & `tmp/backgammon-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\backgammon-1.0.0.tar", last modified: Fri Jul  2 23:15:01 2021, max compression
+gzip compressed data, was "backgammon-1.1.0.tar", last modified: Sat Jun 10 19:21:23 2023, max compression
```

## Comparing `backgammon-1.0.0.tar` & `backgammon-1.1.0.tar`

### file list

```diff
@@ -1,22 +1,21 @@
-drwxrwxrwx   0        0        0        0 2021-07-02 23:15:01.000000 backgammon-1.0.0/
--rw-rw-rw-   0        0        0    11558 2019-10-26 21:43:34.000000 backgammon-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     4539 2021-07-02 23:15:01.000000 backgammon-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     4032 2020-11-21 22:17:19.000000 backgammon-1.0.0/README.rst
-drwxrwxrwx   0        0        0        0 2021-07-02 23:15:01.000000 backgammon-1.0.0/backgammon/
--rw-rw-rw-   0        0        0      638 2020-11-20 00:35:44.000000 backgammon-1.0.0/backgammon/__init__.py
--rw-rw-rw-   0        0        0     3273 2021-05-27 02:53:07.000000 backgammon-1.0.0/backgammon/__main__.py
--rw-rw-rw-   0        0        0    13867 2021-06-24 18:54:25.000000 backgammon-1.0.0/backgammon/backgammon.py
--rw-rw-rw-   0        0        0     5750 2021-06-24 19:41:37.000000 backgammon-1.0.0/backgammon/match.py
--rw-rw-rw-   0        0        0     7951 2021-06-01 17:07:47.000000 backgammon-1.0.0/backgammon/position.py
-drwxrwxrwx   0        0        0        0 2021-07-02 23:15:01.000000 backgammon-1.0.0/backgammon.egg-info/
--rw-rw-rw-   0        0        0     4539 2021-07-02 23:15:00.000000 backgammon-1.0.0/backgammon.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      363 2021-07-02 23:15:00.000000 backgammon-1.0.0/backgammon.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-07-02 23:15:00.000000 backgammon-1.0.0/backgammon.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2021-07-02 23:15:00.000000 backgammon-1.0.0/backgammon.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2021-07-02 23:15:01.000000 backgammon-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1298 2021-07-02 22:55:29.000000 backgammon-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2021-07-02 23:15:01.000000 backgammon-1.0.0/tests/
--rw-rw-rw-   0        0        0      590 2021-05-15 22:26:47.000000 backgammon-1.0.0/tests/__init__.py
--rw-rw-rw-   0        0        0    15877 2021-06-24 19:52:09.000000 backgammon-1.0.0/tests/test_backgammon.py
--rw-rw-rw-   0        0        0     3503 2021-06-24 19:23:26.000000 backgammon-1.0.0/tests/test_match.py
--rw-rw-rw-   0        0        0     7225 2021-05-27 03:02:35.000000 backgammon-1.0.0/tests/test_position.py
+drwxrwxrwx   0 sam       (1000) sam       (1000)        0 2023-06-10 19:21:23.432068 backgammon-1.1.0/
+-rwxrwxrwx   0 sam       (1000) sam       (1000)     4956 2023-06-10 19:21:23.431068 backgammon-1.1.0/PKG-INFO
+-rwxrwxrwx   0 sam       (1000) sam       (1000)     4044 2023-06-10 19:10:26.000000 backgammon-1.1.0/README.rst
+drwxrwxrwx   0 sam       (1000) sam       (1000)        0 2023-06-10 19:21:23.417922 backgammon-1.1.0/backgammon/
+-rwxrwxrwx   0 sam       (1000) sam       (1000)      638 2023-06-10 01:39:59.000000 backgammon-1.1.0/backgammon/__init__.py
+-rwxrwxrwx   0 sam       (1000) sam       (1000)     3241 2023-06-10 18:30:52.000000 backgammon-1.1.0/backgammon/__main__.py
+-rwxrwxrwx   0 sam       (1000) sam       (1000)    14856 2023-06-10 01:39:59.000000 backgammon-1.1.0/backgammon/backgammon.py
+-rwxrwxrwx   0 sam       (1000) sam       (1000)     5748 2023-06-10 01:39:59.000000 backgammon-1.1.0/backgammon/match.py
+-rwxrwxrwx   0 sam       (1000) sam       (1000)     7951 2023-06-10 01:39:59.000000 backgammon-1.1.0/backgammon/position.py
+drwxrwxrwx   0 sam       (1000) sam       (1000)        0 2023-06-10 19:21:23.421027 backgammon-1.1.0/backgammon.egg-info/
+-rwxrwxrwx   0 sam       (1000) sam       (1000)     4956 2023-06-10 19:21:23.000000 backgammon-1.1.0/backgammon.egg-info/PKG-INFO
+-rwxrwxrwx   0 sam       (1000) sam       (1000)      355 2023-06-10 19:21:23.000000 backgammon-1.1.0/backgammon.egg-info/SOURCES.txt
+-rwxrwxrwx   0 sam       (1000) sam       (1000)        1 2023-06-10 19:21:23.000000 backgammon-1.1.0/backgammon.egg-info/dependency_links.txt
+-rwxrwxrwx   0 sam       (1000) sam       (1000)       17 2023-06-10 19:21:23.000000 backgammon-1.1.0/backgammon.egg-info/top_level.txt
+-rwxrwxrwx   0 sam       (1000) sam       (1000)       38 2023-06-10 19:21:23.432068 backgammon-1.1.0/setup.cfg
+-rwxrwxrwx   0 sam       (1000) sam       (1000)     1298 2023-06-10 19:18:14.000000 backgammon-1.1.0/setup.py
+drwxrwxrwx   0 sam       (1000) sam       (1000)        0 2023-06-10 19:21:23.430189 backgammon-1.1.0/tests/
+-rwxrwxrwx   0 sam       (1000) sam       (1000)      590 2023-06-10 01:39:59.000000 backgammon-1.1.0/tests/__init__.py
+-rwxrwxrwx   0 sam       (1000) sam       (1000)    15901 2023-06-10 02:27:48.000000 backgammon-1.1.0/tests/test_backgammon.py
+-rwxrwxrwx   0 sam       (1000) sam       (1000)     3503 2023-06-10 01:39:59.000000 backgammon-1.1.0/tests/test_match.py
+-rwxrwxrwx   0 sam       (1000) sam       (1000)     7225 2023-06-10 01:39:59.000000 backgammon-1.1.0/tests/test_position.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `backgammon-1.0.0/PKG-INFO` & `backgammon-1.1.0/README.rst`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,11 @@
-Metadata-Version: 2.1
-Name: backgammon
-Version: 1.0.0
-Summary: Backgammon engine for the Backgammon Network.
-Home-page: https://github.com/softwerks/backgammon
-Author: Softwerks
-Author-email: info@softwerks.com
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/x-rst
-License-File: LICENSE
-
 backgammon
 ==========
 
-Backgammon engine for the `Backgammon Network <https://www.bkgmn.net>`_.
+.. image:: https://github.com/softwerks/backgammon/actions/workflows/ci.yml/badge.svg
 
 Installation
 ------------
 
 .. code-block:: bash
 
     $ pip install backgammon
@@ -45,35 +29,34 @@
     v|                  |BAR|                  |
      |                  |   | X                |
      | O                |   | X                |
      | O           X    |   | X                |
      | O           X    |   | X              O |
      | O  X        X    | X | X              O |
      +12-11-10--9--8--7-------6--5--4--3--2--1-+
+
     >>> for play in b.generate_plays():
-    ...     print(play.moves)
-    ...     print(play.position)
+    ...    print(play.moves)
+    ...    print(play.position)
     ...
-    (Move(pips=3, source=None, destination=22), Move(pips=2, source=13, destination=11))
-    Position(board_points=(-2, 0, 0, 0, 0, 5, 0, 3, 0, 0, 2, -4, 3, 0, 0, 0, -3, -1, -5, 0, 0, 1, 0, 1), player_bar=0, player_off=1, opponent_bar=0, opponent_off=0)
-    (Move(pips=2, source=None, destination=23), Move(pips=3, source=24, destination=21))
-    Position(board_points=(-2, 0, 0, 0, 0, 5, 0, 3, 0, 0, 1, -4, 4, 0, 0, 0, -3, -1, -5, 0, 1, 0, 1, 0), player_bar=0, player_off=1, opponent_bar=0, opponent_off=0)
-    (Move(pips=3, source=None, destination=22), Move(pips=2, source=11, destination=9))
-    Position(board_points=(-2, 0, 0, 0, 0, 5, 0, 3, 1, 0, 0, -4, 4, 0, 0, 0, -3, -1, -5, 0, 0, 1, 0, 1), player_bar=0, player_off=1, opponent_bar=0, opponent_off=0)
-    (Move(pips=3, source=None, destination=22), Move(pips=2, source=22, destination=20))
-    Position(board_points=(-2, 0, 0, 0, 0, 5, 0, 3, 0, 0, 1, -4, 4, 0, 0, 0, -3, -1, -5, 1, 0, 0, 0, 1), player_bar=0, player_off=1, opponent_bar=0, opponent_off=0)
-    (Move(pips=2, source=None, destination=23), Move(pips=3, source=13, destination=10))
-    Position(board_points=(-2, 0, 0, 0, 0, 5, 0, 3, 0, 1, 1, -4, 3, 0, 0, 0, -3, -1, -5, 0, 0, 0, 1, 1), player_bar=0, player_off=1, opponent_bar=0, opponent_off=0)
-    (Move(pips=2, source=None, destination=23), Move(pips=3, source=8, destination=5))
-    Position(board_points=(-2, 0, 0, 0, 1, 5, 0, 2, 0, 0, 1, -4, 4, 0, 0, 0, -3, -1, -5, 0, 0, 0, 1, 1), player_bar=0, player_off=1, opponent_bar=0, opponent_off=0)
-    (Move(pips=3, source=None, destination=22), Move(pips=2, source=24, destination=22))
-    Position(board_points=(-2, 0, 0, 0, 0, 5, 0, 3, 0, 0, 1, -4, 4, 0, 0, 0, -3, -1, -5, 0, 0, 2, 0, 0), player_bar=0, player_off=1, opponent_bar=0, opponent_off=0)
-    (Move(pips=3, source=None, destination=22), Move(pips=2, source=6, destination=4))
-    Position(board_points=(-2, 0, 0, 1, 0, 4, 0, 3, 0, 0, 1, -4, 4, 0, 0, 0, -3, -1, -5, 0, 0, 1, 0, 1), player_bar=0, player_off=1, opponent_bar=0, opponent_off=0)
-    (Move(pips=2, source=None, destination=23), Move(pips=3, source=6, destination=3))
-    Position(board_points=(-2, 0, 1, 0, 0, 4, 0, 3, 0, 0, 1, -4, 4, 0, 0, 0, -3, -1, -5, 0, 0, 0, 1, 1), player_bar=0, player_off=1, opponent_bar=0, opponent_off=0)
-    (Move(pips=2, source=None, destination=23), Move(pips=3, source=11, destination=8))
-    Position(board_points=(-2, 0, 0, 0, 0, 5, 0, 4, 0, 0, 0, -4, 4, 0, 0, 0, -3, -1, -5, 0, 0, 0, 1, 1), player_bar=0, player_off=1, opponent_bar=0, opponent_off=0)
-    (Move(pips=3, source=None, destination=22), Move(pips=2, source=8, destination=6))
-    Position(board_points=(-2, 0, 0, 0, 0, 6, 0, 2, 0, 0, 1, -4, 4, 0, 0, 0, -3, -1, -5, 0, 0, 1, 0, 1), player_bar=0, player_off=1, opponent_bar=0, opponent_off=0)
-
-
+    (Move(pips=3, source=None, destination=21), Move(pips=2, source=5, destination=3))
+    Position(board_points=(-2, 0, 0, 1, 0, 4, 0, 3, 0, 0, 1, -4, 4, 0, 0, 0, -3, -1, -5, 0, 0, 1, 0, 1), player_bar=0, player_off=0, opponent_bar=0, opponent_off=0)
+    (Move(pips=2, source=None, destination=22), Move(pips=3, source=12, destination=9))
+    Position(board_points=(-2, 0, 0, 0, 0, 5, 0, 3, 0, 1, 1, -4, 3, 0, 0, 0, -3, -1, -5, 0, 0, 0, 1, 1), player_bar=0, player_off=0, opponent_bar=0, opponent_off=0)
+    (Move(pips=2, source=None, destination=22), Move(pips=3, source=5, destination=2))
+    Position(board_points=(-2, 0, 1, 0, 0, 4, 0, 3, 0, 0, 1, -4, 4, 0, 0, 0, -3, -1, -5, 0, 0, 0, 1, 1), player_bar=0, player_off=0, opponent_bar=0, opponent_off=0)
+    (Move(pips=3, source=None, destination=21), Move(pips=2, source=23, destination=21))
+    Position(board_points=(-2, 0, 0, 0, 0, 5, 0, 3, 0, 0, 1, -4, 4, 0, 0, 0, -3, -1, -5, 0, 0, 2, 0, 0), player_bar=0, player_off=0, opponent_bar=0, opponent_off=0)
+    (Move(pips=2, source=None, destination=22), Move(pips=3, source=10, destination=7))
+    Position(board_points=(-2, 0, 0, 0, 0, 5, 0, 4, 0, 0, 0, -4, 4, 0, 0, 0, -3, -1, -5, 0, 0, 0, 1, 1), player_bar=0, player_off=0, opponent_bar=0, opponent_off=0)
+    (Move(pips=3, source=None, destination=21), Move(pips=2, source=21, destination=19))
+    Position(board_points=(-2, 0, 0, 0, 0, 5, 0, 3, 0, 0, 1, -4, 4, 0, 0, 0, -3, -1, -5, 1, 0, 0, 0, 1), player_bar=0, player_off=0, opponent_bar=0, opponent_off=0)
+    (Move(pips=3, source=None, destination=21), Move(pips=2, source=10, destination=8))
+    Position(board_points=(-2, 0, 0, 0, 0, 5, 0, 3, 1, 0, 0, -4, 4, 0, 0, 0, -3, -1, -5, 0, 0, 1, 0, 1), player_bar=0, player_off=0, opponent_bar=0, opponent_off=0)
+    (Move(pips=2, source=None, destination=22), Move(pips=3, source=23, destination=20))
+    Position(board_points=(-2, 0, 0, 0, 0, 5, 0, 3, 0, 0, 1, -4, 4, 0, 0, 0, -3, -1, -5, 0, 1, 0, 1, 0), player_bar=0, player_off=0, opponent_bar=0, opponent_off=0)
+    (Move(pips=2, source=None, destination=22), Move(pips=3, source=7, destination=4))
+    Position(board_points=(-2, 0, 0, 0, 1, 5, 0, 2, 0, 0, 1, -4, 4, 0, 0, 0, -3, -1, -5, 0, 0, 0, 1, 1), player_bar=0, player_off=0, opponent_bar=0, opponent_off=0)
+    (Move(pips=3, source=None, destination=21), Move(pips=2, source=7, destination=5))
+    Position(board_points=(-2, 0, 0, 0, 0, 6, 0, 2, 0, 0, 1, -4, 4, 0, 0, 0, -3, -1, -5, 0, 0, 1, 0, 1), player_bar=0, player_off=0, opponent_bar=0, opponent_off=0)
+    (Move(pips=3, source=None, destination=21), Move(pips=2, source=12, destination=10))
+    Position(board_points=(-2, 0, 0, 0, 0, 5, 0, 3, 0, 0, 2, -4, 3, 0, 0, 0, -3, -1, -5, 0, 0, 1, 0, 1), player_bar=0, player_off=0, opponent_bar=0, opponent_off=0)
```

### Comparing `backgammon-1.0.0/backgammon/__init__.py` & `backgammon-1.1.0/backgammon/__init__.py`

 * *Files identical despite different names*

### Comparing `backgammon-1.0.0/backgammon/__main__.py` & `backgammon-1.1.0/backgammon/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 
     def do_move(self, arg: str) -> None:
         """Make a backgammon move: move <from> <to> ..."""
         Moves = Tuple[Tuple[Optional[int], Optional[int]], ...]
 
         def parse_arg(arg: str) -> Moves:
             arg_ints: List[Optional[int]] = list(
-                map(lambda n: int(n) if n.isdigit() else None, arg.split())
+                map(lambda n: int(n) - 1 if n.isdigit() else None, arg.split())
             )
 
             if len(arg_ints) % 2 == 1:
                 raise ValueError("Incomplete move.")
             if len(arg_ints) > 8:
                 raise ValueError("Too many moves.")
 
@@ -87,16 +87,14 @@
             return
 
         if self.game.match.game_state is GameState.GAME_OVER:
             print(f"P{1 if self.game.match.player is Player.ZERO else 2} wins")
             print(self.game)
             del self.game
         else:
-            self.game.end_turn()
-
             die_1, die_2 = self.game.roll()
             print(f"Rolled {die_1} {die_2}")
             print(self.game)
 
     def do_quit(self, arg: str) -> bool:
         """Exit the program."""
         return True
```

### Comparing `backgammon-1.0.0/backgammon/backgammon.py` & `backgammon-1.1.0/backgammon/backgammon.py`

 * *Files 6% similar despite different names*

```diff
@@ -209,19 +209,15 @@
                     if (
                         self.position.opponent_bar > 0
                         or sum(self.position.board_points[:POINTS_PER_QUADRANT]) != 0
                     ):
                         multiplier = 3
                     else:
                         multiplier = 2
-                self.match.update_score(multiplier)
-                if self.match.game_state is GameState.PLAYING:
-                    self.match.reset_cube()
-                    self.position = backgammon.position.decode(STARTING_POSITION_ID)
-                    self.first_roll()
+                self.end_game(multiplier)
             else:
                 self.end_turn()
 
         else:
             position_id: str = self.position.encode()
             match_id: str = self.match.encode()
             raise BackgammonError(f"Invalid move: {position_id}:{match_id} {moves}")
@@ -237,16 +233,16 @@
         ):
             raise BackgammonError("Cannot double: not cube holder")
         elif self.match.double:
             raise BackgammonError("Cannot double: already doubled")
         elif (
             self.match.player_0_score
             if self.match.player is Player.ZERO
-            else self.match.player_1_score + self.match.cube_value >= self.match.length
-        ):
+            else self.match.player_1_score
+        ) + self.match.cube_value >= self.match.length:
             raise BackgammonError("Cannot double: dead cube")
         elif self.match.crawford:
             raise BackgammonError("Cannot double: crawford game")
 
         self.match.double = True
         self.match.swap_turn()
 
@@ -273,14 +269,40 @@
                 self.position = backgammon.position.decode(STARTING_POSITION_ID)
                 self.first_roll()
         else:
             raise BackgammonError("Cannot reject double: double not offered")
 
         return self
 
+    def resign(self, resign_type: Resign) -> "Backgammon":
+        if self.match.resign is Resign.NONE:
+            self.match.resign = resign_type
+            self.match.swap_turn()
+        else:
+            raise BackgammonError("Resignation has already been offered.")
+
+        return self
+
+    def accept_resignation(self) -> "Backgammon":
+        if self.match.resign is not Resign.NONE:
+            self.end_game(self.match.resign.value)
+        else:
+            raise BackgammonError("Resignation hasn't been offered")
+
+        return self
+
+    def reject_resignation(self) -> "Backgammon":
+        if self.match.resign is not Resign.NONE:
+            self.match.resign = Resign.NONE
+            self.match.swap_turn()
+        else:
+            raise BackgammonError("Resignation hasn't been offered")
+
+        return self
+
     def skip(self) -> "Backgammon":
         num_plays: int = len(self.generate_plays())
         if num_plays == 0:
             self.end_turn()
         else:
             raise BackgammonError(f"Cannot skip turn: {num_plays} possible plays")
 
@@ -289,14 +311,26 @@
     def end_turn(self) -> "Backgammon":
         self.position = self.position.swap_players()
         self.match.swap_players()
         self.match.reset_dice()
 
         return self
 
+    def end_game(self, multiplier: int) -> "Backgammon":
+        self.match.update_score(multiplier)
+
+        self.match.resign = Resign.NONE
+
+        if self.match.game_state is GameState.PLAYING:
+            self.match.reset_cube()
+            self.position = backgammon.position.decode(STARTING_POSITION_ID)
+            self.first_roll()
+
+        return self
+
     def encode(self) -> str:
         return f"{self.position.encode()}:{self.match.encode()}"
 
     def __repr__(self):
         position_id: str = self.position.encode()
         match_id: str = self.match.encode()
         return f"{__name__}.{self.__class__.__name__}('{position_id}', '{match_id}')"
```

### Comparing `backgammon-1.0.0/backgammon/match.py` & `backgammon-1.1.0/backgammon/match.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,15 +96,15 @@
         return self
 
     def update_score(self, multiplier: int) -> "Match":
         points: int = self.cube_value * multiplier
 
         self.crawford = False
 
-        if self.player is Player.ZERO:
+        if self.turn is Player.ZERO:
             self.player_0_score += points
             if (
                 self.length - self.player_0_score == 1
                 and self.length - self.player_1_score > 1
             ):
                 self.crawford = True
         else:
```

### Comparing `backgammon-1.0.0/backgammon/position.py` & `backgammon-1.1.0/backgammon/position.py`

 * *Files identical despite different names*

### Comparing `backgammon-1.0.0/setup.py` & `backgammon-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from setuptools import setup, find_packages
 
 with open("README.rst", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="backgammon",
-    version="1.0.0",
+    version="1.1.0",
     author="Softwerks",
     author_email="info@softwerks.com",
     description="Backgammon engine for the Backgammon Network.",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url="https://github.com/softwerks/backgammon",
     packages=find_packages(),
```

### Comparing `backgammon-1.0.0/tests/__init__.py` & `backgammon-1.1.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `backgammon-1.0.0/tests/test_backgammon.py` & `backgammon-1.1.0/tests/test_backgammon.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         # -----19-20-21-22-23-24-+
         # |   | O     O  O  O  O |
         # |   | O        O  O  O |
         # |   |                  |
         # |BAR|      (5, 4)      |
         # | X |                  |
         self.assertEqual(
-            backgammon.Backgammon("2zIAAAAAAAQAAA", "cInyAAAAAAAE").generate_plays(),
+            sorted(backgammon.Backgammon("2zIAAAAAAAQAAA", "cInyAAAAAAAE").generate_plays()),
             [
                 Play(
                     moves=(
                         Move(pips=4, source=None, destination=20),
                         Move(pips=5, source=20, destination=15),
                     ),
                     position=Position(
@@ -97,15 +97,15 @@
         )
 
         # |      (4, 2)
         # |             X  O |
         # |       X     X  O |
         # --6--5--4--3--2--1-+
         self.assertEqual(
-            backgammon.Backgammon("AACAMQEAAAAAAA", "cAnqAAAAAAAE").generate_plays(),
+            sorted(backgammon.Backgammon("AACAMQEAAAAAAA", "cAnqAAAAAAAE").generate_plays()),
             [
                 Play(
                     moves=(
                         Move(pips=2, source=3, destination=1),
                         Move(pips=4, source=1, destination=None),
                     ),
                     position=Position(
@@ -223,49 +223,49 @@
 
         # +13-14-15-16-17-18------19-20-21-22-23-24-+
         # | O  O     O  O  X |   |       O  O  O  X |
         # |    O     O  O    |   |       O     O    |
         # |          O       |   |       O     O    |
         # |                  |   |      (3, 2)      |
         self.assertEqual(
-            backgammon.Backgammon("rsPOAgAAAAIBAA", "cImpAAAAAAAE").generate_plays(),
+            sorted(backgammon.Backgammon("rsPOAgAAAAIBAA", "cImpAAAAAAAE").generate_plays()),
             [
                 Play(
                     moves=(
-                        Move(pips=3, source=17, destination=14),
-                        Move(pips=2, source=14, destination=12),
+                        Move(pips=2, source=23, destination=21),
+                        Move(pips=3, source=21, destination=18),
                     ),
                     position=Position(
-                        board_points=(0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1, -2, 0, -3, -2, 0, 0, 0, -3, -1, -3, 1),
+                        board_points=(0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, -1, -2, 0, -3, -2, 1, 1, 0, -3, 0, -3, 0),
                         player_bar=0,
                         player_off=13,
                         opponent_bar=1,
                         opponent_off=0,
                     ),
                 ),
                 Play(
                     moves=(
                         Move(pips=3, source=17, destination=14),
-                        Move(pips=2, source=23, destination=21),
+                        Move(pips=2, source=14, destination=12),
                     ),
                     position=Position(
-                        board_points=(0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, -1, -2, 1, -3, -2, 0, 0, 0, -3, 1, -3, 0),
+                        board_points=(0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1, -2, 0, -3, -2, 0, 0, 0, -3, -1, -3, 1),
                         player_bar=0,
                         player_off=13,
                         opponent_bar=1,
                         opponent_off=0,
                     ),
                 ),
                 Play(
                     moves=(
+                        Move(pips=3, source=17, destination=14),
                         Move(pips=2, source=23, destination=21),
-                        Move(pips=3, source=21, destination=18),
                     ),
                     position=Position(
-                        board_points=(0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, -1, -2, 0, -3, -2, 1, 1, 0, -3, 0, -3, 0),
+                        board_points=(0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, -1, -2, 1, -3, -2, 0, 0, 0, -3, 1, -3, 0),
                         player_bar=0,
                         player_off=13,
                         opponent_bar=1,
                         opponent_off=0,
                     ),
                 ),
             ],
```

### Comparing `backgammon-1.0.0/tests/test_match.py` & `backgammon-1.1.0/tests/test_match.py`

 * *Files identical despite different names*

### Comparing `backgammon-1.0.0/tests/test_position.py` & `backgammon-1.1.0/tests/test_position.py`

 * *Files identical despite different names*

