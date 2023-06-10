# Comparing `tmp/alicechess-2.1.0.tar.gz` & `tmp/alicechess-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alicechess-2.1.0.tar", max compression
+gzip compressed data, was "alicechess-2.2.0.tar", max compression
```

## Comparing `alicechess-2.1.0.tar` & `alicechess-2.2.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0     1067 2023-06-09 03:51:57.624891 alicechess-2.1.0/LICENSE
--rw-r--r--   0        0        0     4279 2023-06-09 07:07:55.894301 alicechess-2.1.0/README.md
--rw-r--r--   0        0        0     1042 2023-06-09 17:42:29.149110 alicechess-2.1.0/pyproject.toml
--rw-r--r--   0        0        0      208 2023-06-09 04:36:24.042041 alicechess-2.1.0/src/alicechess/__init__.py
--rw-r--r--   0        0        0      593 2023-06-09 17:41:11.497466 alicechess-2.1.0/src/alicechess/__main__.py
--rw-r--r--   0        0        0       65 2023-06-09 17:42:56.232815 alicechess-2.1.0/src/alicechess/__version__.py
--rw-r--r--   0        0        0    15265 2023-06-09 04:36:45.923112 alicechess-2.1.0/src/alicechess/_moves_calculator.py
--rw-r--r--   0        0        0     3520 2023-06-09 04:37:00.369033 alicechess-2.1.0/src/alicechess/bots.py
--rw-r--r--   0        0        0     1950 2023-06-09 04:38:27.983773 alicechess-2.1.0/src/alicechess/game.py
--rw-r--r--   0        0        0    36291 2023-06-09 04:37:28.559970 alicechess-2.1.0/src/alicechess/game_state.py
--rwxr-xr-x   0        0        0     3888 2019-11-03 22:51:44.000000 alicechess-2.1.0/src/alicechess/pictures/BB.png
--rwxr-xr-x   0        0        0     4963 2019-11-03 22:48:46.000000 alicechess-2.1.0/src/alicechess/pictures/BK.png
--rwxr-xr-x   0        0        0     3933 2019-11-03 22:52:38.000000 alicechess-2.1.0/src/alicechess/pictures/BN.png
--rwxr-xr-x   0        0        0     8848 2019-11-03 23:06:38.000000 alicechess-2.1.0/src/alicechess/pictures/BP.png
--rwxr-xr-x   0        0        0     5831 2019-11-03 23:07:30.000000 alicechess-2.1.0/src/alicechess/pictures/BQ.png
--rwxr-xr-x   0        0        0     2324 2019-11-03 22:51:08.000000 alicechess-2.1.0/src/alicechess/pictures/BR.png
--rwxr-xr-x   0        0        0     5161 2019-11-03 22:57:12.000000 alicechess-2.1.0/src/alicechess/pictures/WB.png
--rwxr-xr-x   0        0        0     4866 2019-11-03 22:49:20.000000 alicechess-2.1.0/src/alicechess/pictures/WK.png
--rwxr-xr-x   0        0        0     4540 2019-11-03 22:57:50.000000 alicechess-2.1.0/src/alicechess/pictures/WN.png
--rwxr-xr-x   0        0        0     9840 2019-11-03 23:09:48.000000 alicechess-2.1.0/src/alicechess/pictures/WP.png
--rwxr-xr-x   0        0        0     6825 2019-11-03 22:56:10.000000 alicechess-2.1.0/src/alicechess/pictures/WQ.png
--rwxr-xr-x   0        0        0     3235 2019-11-03 23:09:06.000000 alicechess-2.1.0/src/alicechess/pictures/WR.png
--rw-r--r--   0        0        0     2129 2023-06-09 04:32:36.557471 alicechess-2.1.0/src/alicechess/pieces/__init__.py
--rw-r--r--   0        0        0     2566 2023-06-09 04:32:19.713301 alicechess-2.1.0/src/alicechess/pieces/king.py
--rw-r--r--   0        0        0     1396 2023-06-09 04:32:48.125403 alicechess-2.1.0/src/alicechess/pieces/pawn.py
--rw-r--r--   0        0        0     8089 2023-06-09 04:32:57.403280 alicechess-2.1.0/src/alicechess/pieces/piece.py
--rw-r--r--   0        0        0     2178 2023-06-09 04:37:41.423231 alicechess-2.1.0/src/alicechess/player.py
--rw-r--r--   0        0        0    10036 2023-06-09 07:12:48.581884 alicechess-2.1.0/src/alicechess/position.py
--rw-r--r--   0        0        0     2644 2023-06-09 04:26:49.101173 alicechess-2.1.0/src/alicechess/utils.py
--rw-r--r--   0        0        0    24426 2023-06-09 17:41:56.223271 alicechess-2.1.0/src/alicechess/window.py
--rw-r--r--   0        0        0     5183 1970-01-01 00:00:00.000000 alicechess-2.1.0/setup.py
--rw-r--r--   0        0        0     5035 1970-01-01 00:00:00.000000 alicechess-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-06-09 03:51:57.624891 alicechess-2.2.0/LICENSE
+-rw-r--r--   0        0        0     5015 2023-06-09 21:19:21.526526 alicechess-2.2.0/README.md
+-rw-r--r--   0        0        0     1042 2023-06-09 21:21:30.662001 alicechess-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0      208 2023-06-09 04:36:24.042041 alicechess-2.2.0/src/alicechess/__init__.py
+-rw-r--r--   0        0        0     1780 2023-06-09 18:02:35.867083 alicechess-2.2.0/src/alicechess/__main__.py
+-rw-r--r--   0        0        0       65 2023-06-09 21:21:34.190732 alicechess-2.2.0/src/alicechess/__version__.py
+-rw-r--r--   0        0        0    15734 2023-06-09 21:17:42.280201 alicechess-2.2.0/src/alicechess/_moves_calculator.py
+-rw-r--r--   0        0        0     3520 2023-06-09 04:37:00.369033 alicechess-2.2.0/src/alicechess/bots.py
+-rw-r--r--   0        0        0     1950 2023-06-09 04:38:27.983773 alicechess-2.2.0/src/alicechess/game.py
+-rw-r--r--   0        0        0    36913 2023-06-09 20:59:57.983334 alicechess-2.2.0/src/alicechess/game_state.py
+-rwxr-xr-x   0        0        0     3888 2019-11-03 22:51:44.000000 alicechess-2.2.0/src/alicechess/pictures/BB.png
+-rwxr-xr-x   0        0        0     4963 2019-11-03 22:48:46.000000 alicechess-2.2.0/src/alicechess/pictures/BK.png
+-rwxr-xr-x   0        0        0     3933 2019-11-03 22:52:38.000000 alicechess-2.2.0/src/alicechess/pictures/BN.png
+-rwxr-xr-x   0        0        0     8848 2019-11-03 23:06:38.000000 alicechess-2.2.0/src/alicechess/pictures/BP.png
+-rwxr-xr-x   0        0        0     5831 2019-11-03 23:07:30.000000 alicechess-2.2.0/src/alicechess/pictures/BQ.png
+-rwxr-xr-x   0        0        0     2324 2019-11-03 22:51:08.000000 alicechess-2.2.0/src/alicechess/pictures/BR.png
+-rwxr-xr-x   0        0        0     5161 2019-11-03 22:57:12.000000 alicechess-2.2.0/src/alicechess/pictures/WB.png
+-rwxr-xr-x   0        0        0     4866 2019-11-03 22:49:20.000000 alicechess-2.2.0/src/alicechess/pictures/WK.png
+-rwxr-xr-x   0        0        0     4540 2019-11-03 22:57:50.000000 alicechess-2.2.0/src/alicechess/pictures/WN.png
+-rwxr-xr-x   0        0        0     9840 2019-11-03 23:09:48.000000 alicechess-2.2.0/src/alicechess/pictures/WP.png
+-rwxr-xr-x   0        0        0     6825 2019-11-03 22:56:10.000000 alicechess-2.2.0/src/alicechess/pictures/WQ.png
+-rwxr-xr-x   0        0        0     3235 2019-11-03 23:09:06.000000 alicechess-2.2.0/src/alicechess/pictures/WR.png
+-rw-r--r--   0        0        0     2129 2023-06-09 04:32:36.557471 alicechess-2.2.0/src/alicechess/pieces/__init__.py
+-rw-r--r--   0        0        0     2566 2023-06-09 04:32:19.713301 alicechess-2.2.0/src/alicechess/pieces/king.py
+-rw-r--r--   0        0        0     1396 2023-06-09 04:32:48.125403 alicechess-2.2.0/src/alicechess/pieces/pawn.py
+-rw-r--r--   0        0        0     8089 2023-06-09 04:32:57.403280 alicechess-2.2.0/src/alicechess/pieces/piece.py
+-rw-r--r--   0        0        0     2178 2023-06-09 04:37:41.423231 alicechess-2.2.0/src/alicechess/player.py
+-rw-r--r--   0        0        0    10036 2023-06-09 07:12:48.581884 alicechess-2.2.0/src/alicechess/position.py
+-rw-r--r--   0        0        0     3105 2023-06-09 18:53:33.342379 alicechess-2.2.0/src/alicechess/utils.py
+-rw-r--r--   0        0        0    24382 2023-06-09 18:51:47.441006 alicechess-2.2.0/src/alicechess/window.py
+-rw-r--r--   0        0        0     5929 1970-01-01 00:00:00.000000 alicechess-2.2.0/setup.py
+-rw-r--r--   0        0        0     5771 1970-01-01 00:00:00.000000 alicechess-2.2.0/PKG-INFO
```

### Comparing `alicechess-2.1.0/LICENSE` & `alicechess-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alicechess-2.1.0/README.md` & `alicechess-2.2.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -14,31 +14,40 @@
 
 Here is a [description of the concept and rules][rules].
 
 [rules]: https://www.chessvariants.com/other.dir/alice.html
 
 Notable game rules:
 
+- A piece's move must be valid on the board it is on, which means that a piece
+  on Board B can block a check on Board A after teleporting (since the move was
+  valid on Board B, and the move overall was legal because the king is not
+  staying in check). See the above link for a more detailed argument on this.
 - **Castling**: A king and rook may only castle if neither has moved already,
-  the king is not in check, all squares between them are vacant on both boards,
-  and the king does not move through check or into check. After the castle, both
-  pieces will teleport to the other board.
+  the king is not in check, the squares they will move to are vacant on both
+  boards, and the king does not move through check (on Board A) or into check.
+  After the castle, both pieces will teleport to the other board.
 - **En passant**: A pawn may capture another pawn through en passant if your
-  pawn is on board B and the enemy pawn advances two spaces, teleporting to the
-  space right next to yours on board B. (This results in a situation that looks
+  pawn is on Board B and the enemy pawn advances two spaces, teleporting to the
+  space right next to yours on Board B. (This results in a situation that looks
   like regular en passant.) Note that due to teleporting to the other board
   after each move, this can only be achieved by a pawn that _does not_ advance
-  two squares on its first move.
+  two squares on its first move. Also, if there is a piece on Board B where the
+  en passant move would go (i.e., your pawn can already capture a piece
+  normally), then en passant will not take place.
 - **Fifty move rule**: If both players have made 50 moves each where no piece
   has been captured or no pawn moved, then a player may claim a draw. However,
   to simplify this case, the game will be automatically ended with a draw
-  (rather than allowing a player to claim a draw), although this is not the
-  official rule. This therefore overshadows the 75-move rule, where a draw is
-  automatically applied after 75 moves by both players with no captures or pawn
-  movements.
+  (rather than allowing a player to claim a draw). This therefore overshadows
+  the 75-move rule, where a draw is automatically applied after 75 moves by both
+  players with no captures or pawn movements.
+- **Threefold repetition rule**: If a board position appears three times in a
+  game (not necessarily in a row), then a player may claim a draw. However, to
+  simplify this case, the game will be automatically ended with a draw (rather
+  than allowing a player to claim a draw).
 
 ## How to play
 
 To start a game between two human players, you can easily just run the package
 on the command line:
 
 ```bash
```

### Comparing `alicechess-2.1.0/pyproject.toml` & `alicechess-2.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 profile = "black"
 # Just setting the profile will use the `black` default line length of 88, so
 # need to override line length as well
 line_length = 79
 
 [tool.poetry]
 name = "alicechess"
-version = "2.1.0"
+version = "2.2.0"
 description = "A Python package to play Alice Chess"
 authors = ["Joseph Lou <joseph.d.lou@gmail.com>"]
 license = "MIT License"
 readme = "README.md"
 homepage = "https://github.com/josephlou5/alicechess"
 repository = "https://github.com/josephlou5/alicechess"
 classifiers = [
```

### Comparing `alicechess-2.1.0/src/alicechess/_moves_calculator.py` & `alicechess-2.2.0/src/alicechess/_moves_calculator.py`

 * *Files 1% similar despite different names*

```diff
@@ -214,26 +214,27 @@
                 if rc < kc:
                     # left rook: king will move to the left
                     dc = -1
                 else:  # kc < rc
                     # right rook: king will move to the right
                     dc = 1
                 valid_castle = True
-                # check that all the spaces in the middle are empty on
-                # both boards
+                # check that the spaces in the middle are empty
                 c = kc + dc
                 while c != rc:
                     if (bn, kr, c) in self._board:
-                        # there's a piece there
-                        valid_castle = False
-                        break
-                    if (1 - bn, kr, c) in self._board:
-                        # there's a piece there on the other board
+                        # there's a piece there on this board
                         valid_castle = False
                         break
+                    if abs(c - kc) <= 2:
+                        # the spaces being landed on must be empty on
+                        # the other board as well
+                        if (1 - bn, kr, c) in self._board:
+                            valid_castle = False
+                            break
                     c += dc
                 if not valid_castle:
                     continue
                 # check that the spaces the king moves through are not
                 # threatened on this board
                 c = kc
                 for _ in range(2):
@@ -267,14 +268,17 @@
                     # cannot capture a piece on the other board
                     continue
                 if not (r == pr and abs(c - pc) == 1):
                     # pawn is not adjacent to advanced pawn
                     continue
                 capture_r = r + pawn.dr
                 capture_pos = (capture_r, pc)
+                if any((bn, *capture_pos) in self._board for bn in range(2)):
+                    # there's a piece there; no en passant
+                    continue
                 if self._move_in_check(
                     pawn.pos, capture_pos, en_passant=(pr, pc)
                 ):
                     continue
                 pawn._add_en_passant(pc)
 
         for piece in self._board.values():
@@ -343,16 +347,20 @@
 
         # make sure move is valid on current board
         board[here_target_pos] = board.pop(pos).move_to(here_target_pos)
         if moving_king:
             check_pos = here_target_pos
         else:
             check_pos = king.pos
-        if _is_threatened(board, enemy_color, *check_pos):
-            return True
+        if moving_king or pos.bn == king.pos.bn:
+            # if the king is moving, can't move into check
+            # otherwise, if on the same board as the king, can't let the
+            # king be in check
+            if _is_threatened(board, enemy_color, *check_pos):
+                return True
         # make sure move is valid after teleporting
         board[there_target_pos] = board.pop(here_target_pos).move_to(
             there_target_pos
         )
         if moving_king:
             check_pos = there_target_pos
         else:
```

### Comparing `alicechess-2.1.0/src/alicechess/bots.py` & `alicechess-2.2.0/src/alicechess/bots.py`

 * *Files identical despite different names*

### Comparing `alicechess-2.1.0/src/alicechess/game.py` & `alicechess-2.2.0/src/alicechess/game.py`

 * *Files identical despite different names*

### Comparing `alicechess-2.1.0/src/alicechess/game_state.py` & `alicechess-2.2.0/src/alicechess/game_state.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 GameState class.
 """
 
 # =============================================================================
 
 import math
+from collections import Counter
 from itertools import count, zip_longest
 from typing import Dict, Iterable, Iterator, Optional, Self, Type
 
 from alicechess import pieces
 from alicechess._moves_calculator import BoardDict, MovesCalculator
 from alicechess.pieces import Piece, make_promoted
 from alicechess.player import AnyPlayer
@@ -44,14 +45,16 @@
         black (Player): The black player.
 
         prev (Optional[GameState]): The previous GameState, or None if
             this is the first state.
         move (Optional[PieceMoved]): The move from the previous
             GameState, or None if this is the first state.
 
+        end_game_state (Optional[EndGameState]): The end game state.
+
         current_color (Color): The color of the current player.
         current_player (Player): The current player.
 
         half_move_clock (int): The number of half-moves since the last
             capture or the last pawn moved.
         num_moves (int): The number of full moves played in the entire
             game.
@@ -69,18 +72,16 @@
             draw).
         is_in_checkmate() -> bool
             Returns whether the current player is in checkmate.
         winner() -> Optional[Color]
             Returns the winner of the game (for checkmate).
         is_in_stalemate() -> bool
             Returns whether the current player is in stalemate.
-        is_kings_draw() -> bool
-            Returns whether the game is a draw by only having kings.
         is_draw() -> bool
-            Returns whether the game is a draw (by the fifty move rule).
+            Returns whether the game is a draw.
 
         is_in_check() -> bool
             Returns whether the current player is in check.
         needs_promotion() -> bool
             Returns whether the state is waiting for a promotion for the
             last moved pawn.
         promote(promote_type) -> GameState
@@ -157,14 +158,19 @@
         else:
             self._first_state = prev._first_state
         self._prev = prev
 
         self._half_move_clock = half_move_clock
         self._num_moves = num_moves
 
+        if prev is None:
+            self._seen_positions = Counter()
+        else:
+            self._seen_positions = prev._seen_positions.copy()
+
         self._captured = tuple(captured)
 
         # construct board
         self._board: BoardDict = {}
         self._kings = [None, None]
         seen_piece_ids = set()
         unmoved_rooks = ([], [])
@@ -280,31 +286,41 @@
         # en passant target
         if en_passant_pawn is None:
             fen.append("-")
         else:
             _, r, c = en_passant_pawn.pos
             r -= en_passant_pawn.dr
             fen.append(Position(r, c).code)
+        # seen position (basically fen without the move counters)
+        board_position = tuple(fen)
+        self._seen_positions[board_position] += 1
         # half move clock
         fen.append(str(self._half_move_clock))
         # full move number
         fen.append(str(self._num_moves))
         # combine
         self._fen = " ".join(fen)
 
+        self._is_in_check = False
+        # some draws could technically happen at the same time, so this
+        # order is arbitrary
         if len(self._board) == 2:
             # only two kings are left
-            self._is_in_check = False
-            self._end_game_state = EndGameState.ONLY_KINGS_DRAW
+            # there could be more cases for this, but not sure what they
+            # are for alice chess
+            self._end_game_state = EndGameState.INSUFFICIENT_MATERIAL_DRAW
             return
         if self._half_move_clock >= 100:
             # 50 move rule
-            self._is_in_check = False
             self._end_game_state = EndGameState.FIFTY_MOVE_DRAW
             return
+        if self._seen_positions[board_position] >= 3:
+            # threefold repetition rule
+            self._end_game_state = EndGameState.THREEFOLD_REPETITION_DRAW
+            return
 
         # calculate all the possible moves
         calculator = MovesCalculator(
             self._board, self._kings, unmoved_rooks, en_passant_pawn
         )
 
         self._is_in_check = calculator.is_in_check(self._current_color)
@@ -319,20 +335,20 @@
         else:
             self._end_game_state = None
 
     def debug(self):
         print("=" * 50)
         print(self.fen())
         print(self.board_to_str())
-        print(self.moves_to_str())
         if self.is_game_over():
             print("end game state:", self._end_game_state)
             if self.is_in_checkmate():
                 print("winner:", self.winner())
         else:
+            print(self.moves_to_str())
             print("in check:", self.is_in_check())
 
     @classmethod
     def new(cls, *, white: Type[AnyPlayer], black: Type[AnyPlayer]) -> Self:
         """Initializes the first GameState of a game."""
         initial_fen = (
             # initial board position
@@ -576,14 +592,19 @@
     def move(self) -> Optional[PieceMoved]:
         """The move from the previous GameState, or None if this is the
         first state.
         """
         return self._move
 
     @property
+    def end_game_state(self) -> Optional[EndGameState]:
+        """The end game state."""
+        return self._end_game_state
+
+    @property
     def current_color(self) -> Color:
         """The color of the current player."""
         return self._current_color
 
     @property
     def current_player(self) -> AnyPlayer:
         """The current player."""
@@ -733,21 +754,19 @@
         # checkmate
         return self._current_color.other()
 
     def is_in_stalemate(self) -> bool:
         """Returns whether the current player is in stalemate."""
         return self._end_game_state is EndGameState.STALEMATE
 
-    def is_kings_draw(self) -> bool:
-        """Returns whether the game is a draw by only having kings."""
-        return self._end_game_state is EndGameState.ONLY_KINGS_DRAW
-
     def is_draw(self) -> bool:
-        """Returns whether the game is a draw (by the fifty move rule)."""
-        return self._end_game_state is EndGameState.FIFTY_MOVE_DRAW
+        """Returns whether the game is a draw."""
+        return (
+            self._end_game_state is not None and self._end_game_state.is_draw()
+        )
 
     def is_in_check(self) -> bool:
         """Returns whether the current player is in check."""
         return self._is_in_check
 
     def needs_promotion(self) -> bool:
         """Returns whether the state is waiting for a promotion for the
```

### Comparing `alicechess-2.1.0/src/alicechess/pictures/BB.png` & `alicechess-2.2.0/src/alicechess/pictures/BB.png`

 * *Files identical despite different names*

### Comparing `alicechess-2.1.0/src/alicechess/pictures/BK.png` & `alicechess-2.2.0/src/alicechess/pictures/BK.png`

 * *Files identical despite different names*

### Comparing `alicechess-2.1.0/src/alicechess/pictures/BN.png` & `alicechess-2.2.0/src/alicechess/pictures/BN.png`

 * *Files identical despite different names*

### Comparing `alicechess-2.1.0/src/alicechess/pictures/BP.png` & `alicechess-2.2.0/src/alicechess/pictures/BP.png`

 * *Files identical despite different names*

### Comparing `alicechess-2.1.0/src/alicechess/pictures/BQ.png` & `alicechess-2.2.0/src/alicechess/pictures/BQ.png`

 * *Files identical despite different names*

### Comparing `alicechess-2.1.0/src/alicechess/pictures/BR.png` & `alicechess-2.2.0/src/alicechess/pictures/BR.png`

 * *Files identical despite different names*

### Comparing `alicechess-2.1.0/src/alicechess/pictures/WB.png` & `alicechess-2.2.0/src/alicechess/pictures/WB.png`

 * *Files identical despite different names*

### Comparing `alicechess-2.1.0/src/alicechess/pictures/WK.png` & `alicechess-2.2.0/src/alicechess/pictures/WK.png`

 * *Files identical despite different names*

### Comparing `alicechess-2.1.0/src/alicechess/pictures/WN.png` & `alicechess-2.2.0/src/alicechess/pictures/WN.png`

 * *Files identical despite different names*

### Comparing `alicechess-2.1.0/src/alicechess/pictures/WP.png` & `alicechess-2.2.0/src/alicechess/pictures/WP.png`

 * *Files identical despite different names*

### Comparing `alicechess-2.1.0/src/alicechess/pictures/WQ.png` & `alicechess-2.2.0/src/alicechess/pictures/WQ.png`

 * *Files identical despite different names*

### Comparing `alicechess-2.1.0/src/alicechess/pictures/WR.png` & `alicechess-2.2.0/src/alicechess/pictures/WR.png`

 * *Files identical despite different names*

### Comparing `alicechess-2.1.0/src/alicechess/pieces/__init__.py` & `alicechess-2.2.0/src/alicechess/pieces/__init__.py`

 * *Files identical despite different names*

### Comparing `alicechess-2.1.0/src/alicechess/pieces/king.py` & `alicechess-2.2.0/src/alicechess/pieces/king.py`

 * *Files identical despite different names*

### Comparing `alicechess-2.1.0/src/alicechess/pieces/pawn.py` & `alicechess-2.2.0/src/alicechess/pieces/pawn.py`

 * *Files identical despite different names*

### Comparing `alicechess-2.1.0/src/alicechess/pieces/piece.py` & `alicechess-2.2.0/src/alicechess/pieces/piece.py`

 * *Files identical despite different names*

### Comparing `alicechess-2.1.0/src/alicechess/player.py` & `alicechess-2.2.0/src/alicechess/player.py`

 * *Files identical despite different names*

### Comparing `alicechess-2.1.0/src/alicechess/position.py` & `alicechess-2.2.0/src/alicechess/position.py`

 * *Files identical despite different names*

### Comparing `alicechess-2.1.0/src/alicechess/utils.py` & `alicechess-2.2.0/src/alicechess/utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -72,16 +72,29 @@
 
 
 class EndGameState(_enum.Enum):
     """The possible states for the end of the game."""
 
     CHECKMATE = _enum.auto()
     STALEMATE = _enum.auto()
-    ONLY_KINGS_DRAW = _enum.auto()
+    INSUFFICIENT_MATERIAL_DRAW = _enum.auto()
     FIFTY_MOVE_DRAW = _enum.auto()
+    THREEFOLD_REPETITION_DRAW = _enum.auto()
+
+    def human_readable(self) -> str:
+        """Returns a human-readable name of this state."""
+        return self.name.replace("_", " ").title()
+
+    def is_draw(self) -> bool:
+        """Returns whether the current state is a type of draw."""
+        return self in (
+            self.INSUFFICIENT_MATERIAL_DRAW,
+            self.FIFTY_MOVE_DRAW,
+            self.THREEFOLD_REPETITION_DRAW,
+        )
 
 
 # =============================================================================
 
 
 def check_brc(bn=None, r=None, c=None, tr=None, tc=None):
     """Checks that all the given args are within the proper bounds.
```

### Comparing `alicechess-2.1.0/src/alicechess/window.py` & `alicechess-2.2.0/src/alicechess/window.py`

 * *Files 1% similar despite different names*

```diff
@@ -731,18 +731,16 @@
         if game.is_game_over():
             # no more pause
             self._hide("pause")
             if game.is_in_checkmate():
                 text = f"Checkmate. {game.winner().title()} won!"
             elif game.is_in_stalemate():
                 text = "Stalemate."
-            elif game.is_kings_draw():
-                text = "Draw."
             elif game.is_draw():
-                text = "Draw (50 moves rule)."
+                text = f"Draw ({game.end_game_state.human_readable()})."
             self._show(self._state_text, text=text)
             return
 
         # check for check
         if game.is_in_check():
             self._show(
                 self._state_text,
```

### Comparing `alicechess-2.1.0/setup.py` & `alicechess-2.2.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 {'': ['*'], 'alicechess': ['pictures/*']}
 
 install_requires = \
 ['Pillow>=9.5.0,<10.0.0']
 
 setup_kwargs = {
     'name': 'alicechess',
-    'version': '2.1.0',
+    'version': '2.2.0',
     'description': 'A Python package to play Alice Chess',
-    'long_description': '# Alice Chess\n\nThis project allows you to play Alice Chess, a variant of chess.\n\n## Installation\n\nThe package may be installed through `pip`:\n\n```bash\n$ pip install alicechess\n```\n\n## Rules\n\nHere is a [description of the concept and rules][rules].\n\n[rules]: https://www.chessvariants.com/other.dir/alice.html\n\nNotable game rules:\n\n- **Castling**: A king and rook may only castle if neither has moved already,\n  the king is not in check, all squares between them are vacant on both boards,\n  and the king does not move through check or into check. After the castle, both\n  pieces will teleport to the other board.\n- **En passant**: A pawn may capture another pawn through en passant if your\n  pawn is on board B and the enemy pawn advances two spaces, teleporting to the\n  space right next to yours on board B. (This results in a situation that looks\n  like regular en passant.) Note that due to teleporting to the other board\n  after each move, this can only be achieved by a pawn that _does not_ advance\n  two squares on its first move.\n- **Fifty move rule**: If both players have made 50 moves each where no piece\n  has been captured or no pawn moved, then a player may claim a draw. However,\n  to simplify this case, the game will be automatically ended with a draw\n  (rather than allowing a player to claim a draw), although this is not the\n  official rule. This therefore overshadows the 75-move rule, where a draw is\n  automatically applied after 75 moves by both players with no captures or pawn\n  movements.\n\n## How to play\n\nTo start a game between two human players, you can easily just run the package\non the command line:\n\n```bash\n$ python -m alicechess\n```\n\nA window will come up where the game can be played.\n\n## Playing against bots\n\nTo play a game against a bot or between bots, you must write your own script.\nYou should initialize a `Game` object with the appropriate players, then call\neither the `start()` or `start_window()` method. To write your own bot, see the\n[Writing a bot](#writing-a-bot) section.\n\nHere is an example:\n\n```python\n"""\nPlays a game between a human and a bot that plays randomly.\n"""\n\nfrom alicechess import Game, HumanPlayer\nfrom alicechess.bots import RandomPlayer\n\nif __name__ == "__main__":\n    Game(white=HumanPlayer, black=RandomPlayer).start_window()\n```\n\nNote that the class names (not instances) are passed to the `Game` constructor.\n\nThe `start_window()` method will, as implied, start an interactive window where\nthe game can be played. However, you can also opt to use the `start()` method\ninstead, which will return the first `GameState` of the game, and then use\nanother way to ask the user for input and play the game; for instance, you could\nmake the game entirely textual with user input provided with the keyboard. See\nthe [API Documentation][docs] for more information.\n\nIn the interactive window, there is a 3 second delay for non-human player moves,\nto simulate realism. This can be changed by passing a value for\n`non_human_player_delay` to the `start_window()` method.\n\nIt is also possible for two bots to play against each other.\n\n### Writing a bot\n\nThe code is factored in a way to make it very easy for you to code your own bots\nto play against. Simply extend the `Player` class and implement the two abstract\nmethods for making a move and promoting a pawn. This class (not an instance) can\nthen be passed into the `Game` constructor to start a game. See the\n[API Documentation][docs] for more information.\n\nHere is an example:\n\n```python\n"""\nPlays a game between a human and a bot (that I wrote).\n"""\n\nfrom alicechess import Game, HumanPlayer, Player, PromoteType\n\nclass Bot(Player):\n    """A very good bot that I wrote."""\n\n    def make_move(self, game_state):\n        for piece in game_state.yield_player_pieces():\n            for move in piece.yield_moves():\n                return move\n\n    def promote(self, game_state):\n        return PromoteType.QUEEN\n\nif __name__ == "__main__":\n    Game(white=HumanPlayer, black=Bot).start_window()\n```\n\n[docs]: https://github.com/josephlou5/alicechess/blob/main/Documentation.md\n\n## Credit\n\nThank you to Artyom Lisitsyn for inspiring me to pursue this project and to\nTrung Phan for being my chess consultant and answering all my questions on rules\nand technicalities.\n',
+    'long_description': '# Alice Chess\n\nThis project allows you to play Alice Chess, a variant of chess.\n\n## Installation\n\nThe package may be installed through `pip`:\n\n```bash\n$ pip install alicechess\n```\n\n## Rules\n\nHere is a [description of the concept and rules][rules].\n\n[rules]: https://www.chessvariants.com/other.dir/alice.html\n\nNotable game rules:\n\n- A piece\'s move must be valid on the board it is on, which means that a piece\n  on Board B can block a check on Board A after teleporting (since the move was\n  valid on Board B, and the move overall was legal because the king is not\n  staying in check). See the above link for a more detailed argument on this.\n- **Castling**: A king and rook may only castle if neither has moved already,\n  the king is not in check, the squares they will move to are vacant on both\n  boards, and the king does not move through check (on Board A) or into check.\n  After the castle, both pieces will teleport to the other board.\n- **En passant**: A pawn may capture another pawn through en passant if your\n  pawn is on Board B and the enemy pawn advances two spaces, teleporting to the\n  space right next to yours on Board B. (This results in a situation that looks\n  like regular en passant.) Note that due to teleporting to the other board\n  after each move, this can only be achieved by a pawn that _does not_ advance\n  two squares on its first move. Also, if there is a piece on Board B where the\n  en passant move would go (i.e., your pawn can already capture a piece\n  normally), then en passant will not take place.\n- **Fifty move rule**: If both players have made 50 moves each where no piece\n  has been captured or no pawn moved, then a player may claim a draw. However,\n  to simplify this case, the game will be automatically ended with a draw\n  (rather than allowing a player to claim a draw). This therefore overshadows\n  the 75-move rule, where a draw is automatically applied after 75 moves by both\n  players with no captures or pawn movements.\n- **Threefold repetition rule**: If a board position appears three times in a\n  game (not necessarily in a row), then a player may claim a draw. However, to\n  simplify this case, the game will be automatically ended with a draw (rather\n  than allowing a player to claim a draw).\n\n## How to play\n\nTo start a game between two human players, you can easily just run the package\non the command line:\n\n```bash\n$ python -m alicechess\n```\n\nA window will come up where the game can be played.\n\n## Playing against bots\n\nTo play a game against a bot or between bots, you must write your own script.\nYou should initialize a `Game` object with the appropriate players, then call\neither the `start()` or `start_window()` method. To write your own bot, see the\n[Writing a bot](#writing-a-bot) section.\n\nHere is an example:\n\n```python\n"""\nPlays a game between a human and a bot that plays randomly.\n"""\n\nfrom alicechess import Game, HumanPlayer\nfrom alicechess.bots import RandomPlayer\n\nif __name__ == "__main__":\n    Game(white=HumanPlayer, black=RandomPlayer).start_window()\n```\n\nNote that the class names (not instances) are passed to the `Game` constructor.\n\nThe `start_window()` method will, as implied, start an interactive window where\nthe game can be played. However, you can also opt to use the `start()` method\ninstead, which will return the first `GameState` of the game, and then use\nanother way to ask the user for input and play the game; for instance, you could\nmake the game entirely textual with user input provided with the keyboard. See\nthe [API Documentation][docs] for more information.\n\nIn the interactive window, there is a 3 second delay for non-human player moves,\nto simulate realism. This can be changed by passing a value for\n`non_human_player_delay` to the `start_window()` method.\n\nIt is also possible for two bots to play against each other.\n\n### Writing a bot\n\nThe code is factored in a way to make it very easy for you to code your own bots\nto play against. Simply extend the `Player` class and implement the two abstract\nmethods for making a move and promoting a pawn. This class (not an instance) can\nthen be passed into the `Game` constructor to start a game. See the\n[API Documentation][docs] for more information.\n\nHere is an example:\n\n```python\n"""\nPlays a game between a human and a bot (that I wrote).\n"""\n\nfrom alicechess import Game, HumanPlayer, Player, PromoteType\n\nclass Bot(Player):\n    """A very good bot that I wrote."""\n\n    def make_move(self, game_state):\n        for piece in game_state.yield_player_pieces():\n            for move in piece.yield_moves():\n                return move\n\n    def promote(self, game_state):\n        return PromoteType.QUEEN\n\nif __name__ == "__main__":\n    Game(white=HumanPlayer, black=Bot).start_window()\n```\n\n[docs]: https://github.com/josephlou5/alicechess/blob/main/Documentation.md\n\n## Credit\n\nThank you to Artyom Lisitsyn for inspiring me to pursue this project and to\nTrung Phan for being my chess consultant and answering all my questions on rules\nand technicalities.\n',
     'author': 'Joseph Lou',
     'author_email': 'joseph.d.lou@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/josephlou5/alicechess',
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `alicechess-2.1.0/PKG-INFO` & `alicechess-2.2.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alicechess
-Version: 2.1.0
+Version: 2.2.0
 Summary: A Python package to play Alice Chess
 Home-page: https://github.com/josephlou5/alicechess
 License: MIT
 Author: Joseph Lou
 Author-email: joseph.d.lou@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -34,31 +34,40 @@
 
 Here is a [description of the concept and rules][rules].
 
 [rules]: https://www.chessvariants.com/other.dir/alice.html
 
 Notable game rules:
 
+- A piece's move must be valid on the board it is on, which means that a piece
+  on Board B can block a check on Board A after teleporting (since the move was
+  valid on Board B, and the move overall was legal because the king is not
+  staying in check). See the above link for a more detailed argument on this.
 - **Castling**: A king and rook may only castle if neither has moved already,
-  the king is not in check, all squares between them are vacant on both boards,
-  and the king does not move through check or into check. After the castle, both
-  pieces will teleport to the other board.
+  the king is not in check, the squares they will move to are vacant on both
+  boards, and the king does not move through check (on Board A) or into check.
+  After the castle, both pieces will teleport to the other board.
 - **En passant**: A pawn may capture another pawn through en passant if your
-  pawn is on board B and the enemy pawn advances two spaces, teleporting to the
-  space right next to yours on board B. (This results in a situation that looks
+  pawn is on Board B and the enemy pawn advances two spaces, teleporting to the
+  space right next to yours on Board B. (This results in a situation that looks
   like regular en passant.) Note that due to teleporting to the other board
   after each move, this can only be achieved by a pawn that _does not_ advance
-  two squares on its first move.
+  two squares on its first move. Also, if there is a piece on Board B where the
+  en passant move would go (i.e., your pawn can already capture a piece
+  normally), then en passant will not take place.
 - **Fifty move rule**: If both players have made 50 moves each where no piece
   has been captured or no pawn moved, then a player may claim a draw. However,
   to simplify this case, the game will be automatically ended with a draw
-  (rather than allowing a player to claim a draw), although this is not the
-  official rule. This therefore overshadows the 75-move rule, where a draw is
-  automatically applied after 75 moves by both players with no captures or pawn
-  movements.
+  (rather than allowing a player to claim a draw). This therefore overshadows
+  the 75-move rule, where a draw is automatically applied after 75 moves by both
+  players with no captures or pawn movements.
+- **Threefold repetition rule**: If a board position appears three times in a
+  game (not necessarily in a row), then a player may claim a draw. However, to
+  simplify this case, the game will be automatically ended with a draw (rather
+  than allowing a player to claim a draw).
 
 ## How to play
 
 To start a game between two human players, you can easily just run the package
 on the command line:
 
 ```bash
```

