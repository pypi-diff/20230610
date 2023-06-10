# Comparing `tmp/discord_pretty_help-2.0.6.tar.gz` & `tmp/discord_pretty_help-2.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discord_pretty_help-2.0.6.tar", max compression
+gzip compressed data, was "discord_pretty_help-2.0.7.tar", max compression
```

## Comparing `discord_pretty_help-2.0.6.tar` & `discord_pretty_help-2.0.7.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1090 2023-05-14 13:13:36.042000 discord_pretty_help-2.0.6/LICENSE
--rw-r--r--   0        0        0      105 2023-06-10 15:53:42.320360 discord_pretty_help-2.0.6/pretty_help/__init__.py
--rw-r--r--   0        0        0      500 2023-05-14 13:13:36.051000 discord_pretty_help-2.0.6/pretty_help/abc_menu.py
--rw-r--r--   0        0        0     4685 2023-06-10 14:38:43.906306 discord_pretty_help-2.0.6/pretty_help/app_menu.py
--rw-r--r--   0        0        0     5332 2023-05-14 13:13:36.051999 discord_pretty_help-2.0.6/pretty_help/emoji_menu.py
--rw-r--r--   0        0        0    23742 2023-06-10 15:52:34.016006 discord_pretty_help-2.0.6/pretty_help/pretty_help.py
--rw-r--r--   0        0        0      748 2023-06-10 15:53:28.812099 discord_pretty_help-2.0.6/pyproject.toml
--rw-r--r--   0        0        0     3952 2023-05-14 13:13:36.042000 discord_pretty_help-2.0.6/README.md
--rw-r--r--   0        0        0     4626 1970-01-01 00:00:00.000000 discord_pretty_help-2.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1090 2023-05-14 13:13:36.042000 discord_pretty_help-2.0.7/LICENSE
+-rw-r--r--   0        0        0      105 2023-06-10 17:08:52.982240 discord_pretty_help-2.0.7/pretty_help/__init__.py
+-rw-r--r--   0        0        0      500 2023-05-14 13:13:36.051000 discord_pretty_help-2.0.7/pretty_help/abc_menu.py
+-rw-r--r--   0        0        0     4685 2023-06-10 14:38:43.906306 discord_pretty_help-2.0.7/pretty_help/app_menu.py
+-rw-r--r--   0        0        0     5332 2023-05-14 13:13:36.051999 discord_pretty_help-2.0.7/pretty_help/emoji_menu.py
+-rw-r--r--   0        0        0    23744 2023-06-10 17:07:47.636192 discord_pretty_help-2.0.7/pretty_help/pretty_help.py
+-rw-r--r--   0        0        0      748 2023-06-10 17:09:03.945259 discord_pretty_help-2.0.7/pyproject.toml
+-rw-r--r--   0        0        0     3952 2023-05-14 13:13:36.042000 discord_pretty_help-2.0.7/README.md
+-rw-r--r--   0        0        0     4626 1970-01-01 00:00:00.000000 discord_pretty_help-2.0.7/PKG-INFO
```

### Comparing `discord_pretty_help-2.0.6/LICENSE` & `discord_pretty_help-2.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `discord_pretty_help-2.0.6/pretty_help/app_menu.py` & `discord_pretty_help-2.0.7/pretty_help/app_menu.py`

 * *Files identical despite different names*

### Comparing `discord_pretty_help-2.0.6/pretty_help/emoji_menu.py` & `discord_pretty_help-2.0.7/pretty_help/emoji_menu.py`

 * *Files identical despite different names*

### Comparing `discord_pretty_help-2.0.6/pretty_help/pretty_help.py` & `discord_pretty_help-2.0.7/pretty_help/pretty_help.py`

 * *Files 1% similar despite different names*

```diff
@@ -405,15 +405,15 @@
         ctx.bot = bot
         await ctx.invoke(bot.get_command("help"), command=command)
 
     @_app_command_callback.autocomplete("command")
     async def __help_autocomplete(
         self, interaction: discord.Interaction, current: str
     ) -> List[app_commands.Choice[str]]:
-        cmds = [*self.bot.all_commands.keys(), *self.bot.cogs.keys()]
+        cmds = [cmd.qualified_name for cmd in self.bot.walk_commands()]
         cmds += [
             app_cmd.name
             for app_cmd in self.bot.tree.get_commands(
                 type=discord.AppCommandType.chat_input,
                 guild=interaction.guild,
             )
         ]
```

### Comparing `discord_pretty_help-2.0.6/pyproject.toml` & `discord_pretty_help-2.0.7/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "discord-pretty-help"
-version = "2.0.6"
+version = "2.0.7"
 description = "And nicer looking interactive help menu for discord.py"
 authors = ["CasuallyCalm <29642143+casuallycalm@users.noreply.github.com>"]
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/casuallycalm/discord-pretty-help"
 keywords=["discord", "discord.py", "discord bot"]
 packages = [
```

### Comparing `discord_pretty_help-2.0.6/README.md` & `discord_pretty_help-2.0.7/README.md`

 * *Files identical despite different names*

### Comparing `discord_pretty_help-2.0.6/PKG-INFO` & `discord_pretty_help-2.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discord-pretty-help
-Version: 2.0.6
+Version: 2.0.7
 Summary: And nicer looking interactive help menu for discord.py
 Home-page: https://github.com/casuallycalm/discord-pretty-help
 License: MIT
 Keywords: discord,discord.py,discord bot
 Author: CasuallyCalm
 Author-email: 29642143+casuallycalm@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
```

