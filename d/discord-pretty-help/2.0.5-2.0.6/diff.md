# Comparing `tmp/discord_pretty_help-2.0.5.tar.gz` & `tmp/discord_pretty_help-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discord_pretty_help-2.0.5.tar", max compression
+gzip compressed data, was "discord_pretty_help-2.0.6.tar", max compression
```

## Comparing `discord_pretty_help-2.0.5.tar` & `discord_pretty_help-2.0.6.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1090 2023-04-29 11:31:31.530107 discord_pretty_help-2.0.5/LICENSE
--rw-r--r--   0        0        0      105 2023-05-26 22:10:20.050937 discord_pretty_help-2.0.5/pretty_help/__init__.py
--rw-r--r--   0        0        0      500 2023-04-29 11:31:31.540118 discord_pretty_help-2.0.5/pretty_help/abc_menu.py
--rw-r--r--   0        0        0     4685 2023-05-26 22:08:01.160304 discord_pretty_help-2.0.5/pretty_help/app_menu.py
--rw-r--r--   0        0        0     5332 2023-04-29 11:31:31.540118 discord_pretty_help-2.0.5/pretty_help/emoji_menu.py
--rw-r--r--   0        0        0    23111 2023-05-14 10:49:47.368955 discord_pretty_help-2.0.5/pretty_help/pretty_help.py
--rw-r--r--   0        0        0      748 2023-05-26 22:10:05.024664 discord_pretty_help-2.0.5/pyproject.toml
--rw-r--r--   0        0        0     3952 2023-05-14 10:49:13.991504 discord_pretty_help-2.0.5/README.md
--rw-r--r--   0        0        0     4626 1970-01-01 00:00:00.000000 discord_pretty_help-2.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1090 2023-05-14 13:13:36.042000 discord_pretty_help-2.0.6/LICENSE
+-rw-r--r--   0        0        0      105 2023-06-10 15:53:42.320360 discord_pretty_help-2.0.6/pretty_help/__init__.py
+-rw-r--r--   0        0        0      500 2023-05-14 13:13:36.051000 discord_pretty_help-2.0.6/pretty_help/abc_menu.py
+-rw-r--r--   0        0        0     4685 2023-06-10 14:38:43.906306 discord_pretty_help-2.0.6/pretty_help/app_menu.py
+-rw-r--r--   0        0        0     5332 2023-05-14 13:13:36.051999 discord_pretty_help-2.0.6/pretty_help/emoji_menu.py
+-rw-r--r--   0        0        0    23742 2023-06-10 15:52:34.016006 discord_pretty_help-2.0.6/pretty_help/pretty_help.py
+-rw-r--r--   0        0        0      748 2023-06-10 15:53:28.812099 discord_pretty_help-2.0.6/pyproject.toml
+-rw-r--r--   0        0        0     3952 2023-05-14 13:13:36.042000 discord_pretty_help-2.0.6/README.md
+-rw-r--r--   0        0        0     4626 1970-01-01 00:00:00.000000 discord_pretty_help-2.0.6/PKG-INFO
```

### Comparing `discord_pretty_help-2.0.5/LICENSE` & `discord_pretty_help-2.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `discord_pretty_help-2.0.5/pretty_help/app_menu.py` & `discord_pretty_help-2.0.6/pretty_help/app_menu.py`

 * *Files identical despite different names*

### Comparing `discord_pretty_help-2.0.5/pretty_help/emoji_menu.py` & `discord_pretty_help-2.0.6/pretty_help/emoji_menu.py`

 * *Files identical despite different names*

### Comparing `discord_pretty_help-2.0.5/pretty_help/pretty_help.py` & `discord_pretty_help-2.0.6/pretty_help/pretty_help.py`

 * *Files 3% similar despite different names*

```diff
@@ -148,15 +148,15 @@
                 self.prefix,
                 self.suffix,
             ):
                 self._add_page(embed)
                 embed = self._new_page(page_title, embed.description)
 
             embed.add_field(
-                name=command_name, 
+                name=command_name,
                 value=f'{self.prefix}{short_doc or "No Description"}{self.suffix}',
                 inline=False,
             )
 
         self._add_page(embed)
 
     @staticmethod
@@ -353,20 +353,19 @@
         dm_help: Optional[bool] = False,
         ending_note: Optional[str] = "",
         image_url: Optional[str] = None,
         index_title: Optional[str] = "Categories",
         menu: Optional[PrettyMenu] = AppMenu(),
         no_category: Optional[str] = "No Category",
         paginator: Optional[Paginator] = None,
-        send_typing:Optional[bool] = True,
+        send_typing: Optional[bool] = True,
         show_index: Optional[bool] = True,
         sort_commands: Optional[bool] = True,
         thumbnail_url: Optional[str] = None,
         **options,
-
     ):
         self.dm_help = dm_help
         self.index_title = index_title
         self.no_category = no_category
         self.sort_commands = sort_commands
         self.menu = menu
         self.paginator = paginator or Paginator(
@@ -402,14 +401,33 @@
     ):
         """Application help command"""
         bot = interaction.client
         ctx = await commands.Context.from_interaction(interaction)
         ctx.bot = bot
         await ctx.invoke(bot.get_command("help"), command=command)
 
+    @_app_command_callback.autocomplete("command")
+    async def __help_autocomplete(
+        self, interaction: discord.Interaction, current: str
+    ) -> List[app_commands.Choice[str]]:
+        cmds = [*self.bot.all_commands.keys(), *self.bot.cogs.keys()]
+        cmds += [
+            app_cmd.name
+            for app_cmd in self.bot.tree.get_commands(
+                type=discord.AppCommandType.chat_input,
+                guild=interaction.guild,
+            )
+        ]
+
+        return [
+            app_commands.Choice(name=cmd, value=cmd)
+            for cmd in cmds
+            if current.lower() in cmd.lower()
+        ][:24]
+
     async def filter_app_commands(
         self, app_commands: List[app_commands.AppCommand], sort: bool = True
     ):
         """Filter Application Commands and optionally sort them"""
         if sort:
             app_commands.sort(key=lambda x: x.name)
         return app_commands
@@ -577,17 +595,15 @@
         if filtered:
             self.paginator.add_command(command, self.get_command_signature(command))
             await self.send_pages()
 
     async def send_group_help(self, group: commands.Group):
         if self.send_typing:
             await self.get_destination().typing()
-        filtered = await self.filter_commands(
-            group.commands, sort=self.sort_commands
-        )
+        filtered = await self.filter_commands(group.commands, sort=self.sort_commands)
         self.paginator.add_group(group, filtered)
         await self.send_pages()
 
     async def send_cog_help(self, cog: commands.Cog):
         if self.send_typing:
             await self.get_destination().typing()
         filtered = await self.filter_commands(
```

### Comparing `discord_pretty_help-2.0.5/pyproject.toml` & `discord_pretty_help-2.0.6/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "discord-pretty-help"
-version = "2.0.5"
+version = "2.0.6"
 description = "And nicer looking interactive help menu for discord.py"
 authors = ["CasuallyCalm <29642143+casuallycalm@users.noreply.github.com>"]
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/casuallycalm/discord-pretty-help"
 keywords=["discord", "discord.py", "discord bot"]
 packages = [
```

### Comparing `discord_pretty_help-2.0.5/README.md` & `discord_pretty_help-2.0.6/README.md`

 * *Files identical despite different names*

### Comparing `discord_pretty_help-2.0.5/PKG-INFO` & `discord_pretty_help-2.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discord-pretty-help
-Version: 2.0.5
+Version: 2.0.6
 Summary: And nicer looking interactive help menu for discord.py
 Home-page: https://github.com/casuallycalm/discord-pretty-help
 License: MIT
 Keywords: discord,discord.py,discord bot
 Author: CasuallyCalm
 Author-email: 29642143+casuallycalm@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
```

