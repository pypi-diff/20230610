# Comparing `tmp/alicechess-2.2.1.tar.gz` & `tmp/alicechess-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alicechess-2.2.1.tar", max compression
+gzip compressed data, was "alicechess-2.3.0.tar", max compression
```

## Comparing `alicechess-2.2.1.tar` & `alicechess-2.3.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0     1067 2023-06-09 03:51:57.624891 alicechess-2.2.1/LICENSE
--rw-r--r--   0        0        0     5315 2023-06-10 03:29:37.027018 alicechess-2.2.1/README.md
--rw-r--r--   0        0        0     1042 2023-06-10 03:30:24.402283 alicechess-2.2.1/pyproject.toml
--rw-r--r--   0        0        0      208 2023-06-09 04:36:24.042041 alicechess-2.2.1/src/alicechess/__init__.py
--rw-r--r--   0        0        0     1787 2023-06-10 02:56:39.981320 alicechess-2.2.1/src/alicechess/__main__.py
--rw-r--r--   0        0        0      117 2023-06-10 03:30:49.031195 alicechess-2.2.1/src/alicechess/__version__.py
--rw-r--r--   0        0        0    15734 2023-06-09 21:17:42.280201 alicechess-2.2.1/src/alicechess/_moves_calculator.py
--rw-r--r--   0        0        0     3520 2023-06-09 04:37:00.369033 alicechess-2.2.1/src/alicechess/bots.py
--rw-r--r--   0        0        0     2339 2023-06-09 23:39:53.191583 alicechess-2.2.1/src/alicechess/game.py
--rw-r--r--   0        0        0    37803 2023-06-09 23:44:47.925060 alicechess-2.2.1/src/alicechess/game_state.py
--rwxr-xr-x   0        0        0     3888 2019-11-03 22:51:44.000000 alicechess-2.2.1/src/alicechess/pictures/BB.png
--rwxr-xr-x   0        0        0     4963 2019-11-03 22:48:46.000000 alicechess-2.2.1/src/alicechess/pictures/BK.png
--rwxr-xr-x   0        0        0     3933 2019-11-03 22:52:38.000000 alicechess-2.2.1/src/alicechess/pictures/BN.png
--rwxr-xr-x   0        0        0     8848 2019-11-03 23:06:38.000000 alicechess-2.2.1/src/alicechess/pictures/BP.png
--rwxr-xr-x   0        0        0     5831 2019-11-03 23:07:30.000000 alicechess-2.2.1/src/alicechess/pictures/BQ.png
--rwxr-xr-x   0        0        0     2324 2019-11-03 22:51:08.000000 alicechess-2.2.1/src/alicechess/pictures/BR.png
--rwxr-xr-x   0        0        0     5161 2019-11-03 22:57:12.000000 alicechess-2.2.1/src/alicechess/pictures/WB.png
--rwxr-xr-x   0        0        0     4866 2019-11-03 22:49:20.000000 alicechess-2.2.1/src/alicechess/pictures/WK.png
--rwxr-xr-x   0        0        0     4540 2019-11-03 22:57:50.000000 alicechess-2.2.1/src/alicechess/pictures/WN.png
--rwxr-xr-x   0        0        0     9840 2019-11-03 23:09:48.000000 alicechess-2.2.1/src/alicechess/pictures/WP.png
--rwxr-xr-x   0        0        0     6825 2019-11-03 22:56:10.000000 alicechess-2.2.1/src/alicechess/pictures/WQ.png
--rwxr-xr-x   0        0        0     3235 2019-11-03 23:09:06.000000 alicechess-2.2.1/src/alicechess/pictures/WR.png
--rw-r--r--   0        0        0     2129 2023-06-09 04:32:36.557471 alicechess-2.2.1/src/alicechess/pieces/__init__.py
--rw-r--r--   0        0        0     2566 2023-06-09 04:32:19.713301 alicechess-2.2.1/src/alicechess/pieces/king.py
--rw-r--r--   0        0        0     1396 2023-06-09 04:32:48.125403 alicechess-2.2.1/src/alicechess/pieces/pawn.py
--rw-r--r--   0        0        0     8089 2023-06-09 04:32:57.403280 alicechess-2.2.1/src/alicechess/pieces/piece.py
--rw-r--r--   0        0        0     2178 2023-06-09 04:37:41.423231 alicechess-2.2.1/src/alicechess/player.py
--rw-r--r--   0        0        0    10169 2023-06-09 22:53:13.388268 alicechess-2.2.1/src/alicechess/position.py
--rw-r--r--   0        0        0     3105 2023-06-09 18:53:33.342379 alicechess-2.2.1/src/alicechess/utils.py
--rw-r--r--   0        0        0    26547 2023-06-09 23:44:20.909184 alicechess-2.2.1/src/alicechess/window.py
--rw-r--r--   0        0        0     6235 1970-01-01 00:00:00.000000 alicechess-2.2.1/setup.py
--rw-r--r--   0        0        0     6071 1970-01-01 00:00:00.000000 alicechess-2.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-06-09 03:51:57.624891 alicechess-2.3.0/LICENSE
+-rw-r--r--   0        0        0     5315 2023-06-10 03:29:37.027018 alicechess-2.3.0/README.md
+-rw-r--r--   0        0        0     1042 2023-06-10 17:25:28.133796 alicechess-2.3.0/pyproject.toml
+-rw-r--r--   0        0        0      208 2023-06-09 04:36:24.042041 alicechess-2.3.0/src/alicechess/__init__.py
+-rw-r--r--   0        0        0     1787 2023-06-10 02:56:39.981320 alicechess-2.3.0/src/alicechess/__main__.py
+-rw-r--r--   0        0        0      117 2023-06-10 17:25:47.914557 alicechess-2.3.0/src/alicechess/__version__.py
+-rw-r--r--   0        0        0    15734 2023-06-09 21:17:42.280201 alicechess-2.3.0/src/alicechess/_moves_calculator.py
+-rw-r--r--   0        0        0     3520 2023-06-09 04:37:00.369033 alicechess-2.3.0/src/alicechess/bots.py
+-rw-r--r--   0        0        0     2339 2023-06-09 23:39:53.191583 alicechess-2.3.0/src/alicechess/game.py
+-rw-r--r--   0        0        0    37803 2023-06-09 23:44:47.925060 alicechess-2.3.0/src/alicechess/game_state.py
+-rwxr-xr-x   0        0        0     3888 2019-11-03 22:51:44.000000 alicechess-2.3.0/src/alicechess/pictures/BB.png
+-rwxr-xr-x   0        0        0     4963 2019-11-03 22:48:46.000000 alicechess-2.3.0/src/alicechess/pictures/BK.png
+-rwxr-xr-x   0        0        0     3933 2019-11-03 22:52:38.000000 alicechess-2.3.0/src/alicechess/pictures/BN.png
+-rwxr-xr-x   0        0        0     8848 2019-11-03 23:06:38.000000 alicechess-2.3.0/src/alicechess/pictures/BP.png
+-rwxr-xr-x   0        0        0     5831 2019-11-03 23:07:30.000000 alicechess-2.3.0/src/alicechess/pictures/BQ.png
+-rwxr-xr-x   0        0        0     2324 2019-11-03 22:51:08.000000 alicechess-2.3.0/src/alicechess/pictures/BR.png
+-rwxr-xr-x   0        0        0     5161 2019-11-03 22:57:12.000000 alicechess-2.3.0/src/alicechess/pictures/WB.png
+-rwxr-xr-x   0        0        0     4866 2019-11-03 22:49:20.000000 alicechess-2.3.0/src/alicechess/pictures/WK.png
+-rwxr-xr-x   0        0        0     4540 2019-11-03 22:57:50.000000 alicechess-2.3.0/src/alicechess/pictures/WN.png
+-rwxr-xr-x   0        0        0     9840 2019-11-03 23:09:48.000000 alicechess-2.3.0/src/alicechess/pictures/WP.png
+-rwxr-xr-x   0        0        0     6825 2019-11-03 22:56:10.000000 alicechess-2.3.0/src/alicechess/pictures/WQ.png
+-rwxr-xr-x   0        0        0     3235 2019-11-03 23:09:06.000000 alicechess-2.3.0/src/alicechess/pictures/WR.png
+-rw-r--r--   0        0        0     2129 2023-06-09 04:32:36.557471 alicechess-2.3.0/src/alicechess/pieces/__init__.py
+-rw-r--r--   0        0        0     2566 2023-06-09 04:32:19.713301 alicechess-2.3.0/src/alicechess/pieces/king.py
+-rw-r--r--   0        0        0     1396 2023-06-09 04:32:48.125403 alicechess-2.3.0/src/alicechess/pieces/pawn.py
+-rw-r--r--   0        0        0     8089 2023-06-09 04:32:57.403280 alicechess-2.3.0/src/alicechess/pieces/piece.py
+-rw-r--r--   0        0        0     2178 2023-06-09 04:37:41.423231 alicechess-2.3.0/src/alicechess/player.py
+-rw-r--r--   0        0        0    10169 2023-06-09 22:53:13.388268 alicechess-2.3.0/src/alicechess/position.py
+-rw-r--r--   0        0        0     3105 2023-06-09 18:53:33.342379 alicechess-2.3.0/src/alicechess/utils.py
+-rw-r--r--   0        0        0    26547 2023-06-09 23:44:20.909184 alicechess-2.3.0/src/alicechess/window.py
+-rw-r--r--   0        0        0     6235 1970-01-01 00:00:00.000000 alicechess-2.3.0/setup.py
+-rw-r--r--   0        0        0     6071 1970-01-01 00:00:00.000000 alicechess-2.3.0/PKG-INFO
```

### Comparing `alicechess-2.2.1/LICENSE` & `alicechess-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alicechess-2.2.1/README.md` & `alicechess-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `alicechess-2.2.1/pyproject.toml` & `alicechess-2.3.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 profile = "black"
 # Just setting the profile will use the `black` default line length of 88, so
 # need to override line length as well
 line_length = 79
 
 [tool.poetry]
 name = "alicechess"
-version = "2.2.1"
+version = "2.3.0"
 description = "A Python package to play Alice Chess"
 authors = ["Joseph Lou <joseph.d.lou@gmail.com>"]
 license = "MIT License"
 readme = "README.md"
 homepage = "https://github.com/josephlou5/alicechess"
 repository = "https://github.com/josephlou5/alicechess"
 classifiers = [
```

### Comparing `alicechess-2.2.1/src/alicechess/__main__.py` & `alicechess-2.3.0/src/alicechess/__main__.py`

 * *Files identical despite different names*

### Comparing `alicechess-2.2.1/src/alicechess/_moves_calculator.py` & `alicechess-2.3.0/src/alicechess/_moves_calculator.py`

 * *Files identical despite different names*

### Comparing `alicechess-2.2.1/src/alicechess/bots.py` & `alicechess-2.3.0/src/alicechess/bots.py`

 * *Files identical despite different names*

### Comparing `alicechess-2.2.1/src/alicechess/game.py` & `alicechess-2.3.0/src/alicechess/game.py`

 * *Files identical despite different names*

### Comparing `alicechess-2.2.1/src/alicechess/game_state.py` & `alicechess-2.3.0/src/alicechess/game_state.py`

 * *Files identical despite different names*

### Comparing `alicechess-2.2.1/src/alicechess/pictures/BB.png` & `alicechess-2.3.0/src/alicechess/pictures/BB.png`

 * *Files identical despite different names*

### Comparing `alicechess-2.2.1/src/alicechess/pictures/BK.png` & `alicechess-2.3.0/src/alicechess/pictures/BK.png`

 * *Files identical despite different names*

### Comparing `alicechess-2.2.1/src/alicechess/pictures/BN.png` & `alicechess-2.3.0/src/alicechess/pictures/BN.png`

 * *Files identical despite different names*

### Comparing `alicechess-2.2.1/src/alicechess/pictures/BP.png` & `alicechess-2.3.0/src/alicechess/pictures/BP.png`

 * *Files identical despite different names*

### Comparing `alicechess-2.2.1/src/alicechess/pictures/BQ.png` & `alicechess-2.3.0/src/alicechess/pictures/BQ.png`

 * *Files identical despite different names*

### Comparing `alicechess-2.2.1/src/alicechess/pictures/BR.png` & `alicechess-2.3.0/src/alicechess/pictures/BR.png`

 * *Files identical despite different names*

### Comparing `alicechess-2.2.1/src/alicechess/pictures/WB.png` & `alicechess-2.3.0/src/alicechess/pictures/WB.png`

 * *Files identical despite different names*

### Comparing `alicechess-2.2.1/src/alicechess/pictures/WK.png` & `alicechess-2.3.0/src/alicechess/pictures/WK.png`

 * *Files identical despite different names*

### Comparing `alicechess-2.2.1/src/alicechess/pictures/WN.png` & `alicechess-2.3.0/src/alicechess/pictures/WN.png`

 * *Files identical despite different names*

### Comparing `alicechess-2.2.1/src/alicechess/pictures/WP.png` & `alicechess-2.3.0/src/alicechess/pictures/WP.png`

 * *Files identical despite different names*

### Comparing `alicechess-2.2.1/src/alicechess/pictures/WQ.png` & `alicechess-2.3.0/src/alicechess/pictures/WQ.png`

 * *Files identical despite different names*

### Comparing `alicechess-2.2.1/src/alicechess/pictures/WR.png` & `alicechess-2.3.0/src/alicechess/pictures/WR.png`

 * *Files identical despite different names*

### Comparing `alicechess-2.2.1/src/alicechess/pieces/__init__.py` & `alicechess-2.3.0/src/alicechess/pieces/__init__.py`

 * *Files identical despite different names*

### Comparing `alicechess-2.2.1/src/alicechess/pieces/king.py` & `alicechess-2.3.0/src/alicechess/pieces/king.py`

 * *Files identical despite different names*

### Comparing `alicechess-2.2.1/src/alicechess/pieces/pawn.py` & `alicechess-2.3.0/src/alicechess/pieces/pawn.py`

 * *Files identical despite different names*

### Comparing `alicechess-2.2.1/src/alicechess/pieces/piece.py` & `alicechess-2.3.0/src/alicechess/pieces/piece.py`

 * *Files identical despite different names*

### Comparing `alicechess-2.2.1/src/alicechess/player.py` & `alicechess-2.3.0/src/alicechess/player.py`

 * *Files identical despite different names*

### Comparing `alicechess-2.2.1/src/alicechess/position.py` & `alicechess-2.3.0/src/alicechess/position.py`

 * *Files identical despite different names*

### Comparing `alicechess-2.2.1/src/alicechess/utils.py` & `alicechess-2.3.0/src/alicechess/utils.py`

 * *Files identical despite different names*

### Comparing `alicechess-2.2.1/src/alicechess/window.py` & `alicechess-2.3.0/src/alicechess/window.py`

 * *Files identical despite different names*

### Comparing `alicechess-2.2.1/setup.py` & `alicechess-2.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 {'': ['*'], 'alicechess': ['pictures/*']}
 
 install_requires = \
 ['Pillow>=9.5.0,<10.0.0']
 
 setup_kwargs = {
     'name': 'alicechess',
-    'version': '2.2.1',
+    'version': '2.3.0',
     'description': 'A Python package to play Alice Chess',
     'long_description': '# Alice Chess\n\nThis project allows you to play Alice Chess, a variant of chess.\n\n## Installation\n\nThe package may be installed through `pip`:\n\n```bash\n$ pip install alicechess\n```\n\n## Rules\n\nHere is a [description of the concept and rules][rules].\n\n[rules]: https://www.chessvariants.com/other.dir/alice.html\n\nNotable game rules:\n\n- A piece\'s move must be valid on the board it is on, which means that a piece\n  on Board B can block a check on Board A after teleporting (since the move was\n  valid on Board B, and the move overall was legal because the king is not\n  staying in check). See the above link for a more detailed argument on this.\n- **Castling**: A king and rook may only castle if neither has moved already,\n  the king is not in check, the squares they will move to are vacant on both\n  boards, and the king does not move through check (on Board A) or into check.\n  After the castle, both pieces will teleport to the other board.\n- **En passant**: A pawn may capture another pawn through en passant if your\n  pawn is on Board B and the enemy pawn advances two spaces, teleporting to the\n  space right next to yours on Board B. (This results in a situation that looks\n  like regular en passant.) Note that due to teleporting to the other board\n  after each move, this can only be achieved by a pawn that _does not_ advance\n  two squares on its first move. Also, if there is a piece on Board B where the\n  en passant move would go (i.e., your pawn can already capture a piece\n  normally), then en passant will not take place.\n- **Fifty move rule**: If both players have made 50 moves each where no piece\n  has been captured or no pawn moved, then a player may claim a draw. However,\n  to simplify this case, the game will be automatically ended with a draw\n  (rather than allowing a player to claim a draw). This therefore overshadows\n  the 75-move rule, where a draw is automatically applied after 75 moves by both\n  players with no captures or pawn movements.\n- **Threefold repetition rule**: If a board position appears three times in a\n  game (not necessarily in a row), then a player may claim a draw. However, to\n  simplify this case, the game will be automatically ended with a draw (rather\n  than allowing a player to claim a draw).\n\n## How to play\n\n### Command Line\n\nTo start a game between two human players, you can run the package on the\ncommand line:\n\n```bash\n$ python -m alicechess\n```\n\nA window will come up where the game can be played.\n\nYou can also change the players you want to play with by specifying any two of\nthe builtin players (`HumanPlayer` or any of the bots defined in `bots.py`):\n\n```bash\n$ python -m alicechess HumanPlayer RandomPlayer\n```\n\nSee `python -m alicechess --help` for a list of the possible players.\n\n### Script\n\nYou can also use a script to run a game. You must initialize a `Game` object\nwith the appropriate players, then call the `start_window()` or `start()`\nmethod.\n\nHere is an example:\n\n```python\nfrom alicechess import Game, HumanPlayer\nfrom alicechess.bots import RandomPlayer\n\nif __name__ == "__main__":\n    Game(white=HumanPlayer, black=RandomPlayer).start_window()\n```\n\nNote that the class names (not instances) are passed to the `Game` constructor.\n\nThe `start_window()` method will, as implied, start an interactive window where\nthe game can be played. However, you can also opt to use the `start()` method\ninstead, which will return the first `GameState` of the game, and then use\nanother way to ask the user(s) for input and play the game; for instance, you\ncould make the game entirely textual with user input provided with the keyboard.\nSee the [API Documentation][docs] for more information on `GameState` objects,\nand check out [`window.py`][] for how the windowed game is handled.\n\nIn the interactive window, there is a 3 second delay for non-human player moves,\nto simulate realism. This can be changed by passing a value for\n`non_human_player_delay` to the `start_window()` method.\n\nTo play against your own bot, see the [Writing a bot](#writing-a-bot) section.\n\nIt is also possible for two bots to play against each other.\n\n### Writing a bot\n\nThe code is factored in a way to make it very easy for you to code your own bots\nto play against. Simply extend the `Player` class and implement the two abstract\nmethods for making a move and promoting a pawn. This class (not an instance) can\nthen be passed into the `Game` constructor to start a game. See the\n[API Documentation][docs] for more information.\n\nHere is an example:\n\n```python\nfrom alicechess import Game, HumanPlayer, Player, PromoteType\n\nclass MyBot(Player):\n    """A very good bot that I wrote."""\n\n    def make_move(self, game_state):\n        for piece in game_state.yield_player_pieces():\n            for move in piece.yield_moves():\n                return move\n\n    def promote(self, game_state):\n        return PromoteType.QUEEN\n\nif __name__ == "__main__":\n    Game(white=HumanPlayer, black=MyBot).start_window()\n```\n\n## Credit\n\nThank you to Artyom Lisitsyn for inspiring me to pursue this project and to\nTrung Phan for being my chess consultant and answering all my questions on rules\nand technicalities.\n\n[docs]: https://github.com/josephlou5/alicechess/blob/main/Documentation.md\n[`window.py`]: https://github.com/josephlou5/alicechess/blob/main/src/alicechess/window.py\n',
     'author': 'Joseph Lou',
     'author_email': 'joseph.d.lou@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/josephlou5/alicechess',
```

### Comparing `alicechess-2.2.1/PKG-INFO` & `alicechess-2.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alicechess
-Version: 2.2.1
+Version: 2.3.0
 Summary: A Python package to play Alice Chess
 Home-page: https://github.com/josephlou5/alicechess
 License: MIT
 Author: Joseph Lou
 Author-email: joseph.d.lou@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

