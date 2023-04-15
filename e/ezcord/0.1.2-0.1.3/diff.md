# Comparing `tmp/ezcord-0.1.2.tar.gz` & `tmp/ezcord-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ezcord-0.1.2.tar", last modified: Sat Apr  1 14:07:45 2023, max compression
+gzip compressed data, was "ezcord-0.1.3.tar", last modified: Sat Apr 15 22:09:38 2023, max compression
```

## Comparing `ezcord-0.1.2.tar` & `ezcord-0.1.3.tar`

### file list

```diff
@@ -1,24 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 14:07:45.736007 ezcord-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-01 14:07:26.000000 ezcord-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-04-01 14:07:45.736007 ezcord-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-04-01 14:07:26.000000 ezcord-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 14:07:45.736007 ezcord-0.1.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-01 14:07:26.000000 ezcord-0.1.2/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-04-01 14:07:26.000000 ezcord-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-01 14:07:26.000000 ezcord-0.1.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-01 14:07:45.736007 ezcord-0.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 14:07:45.732006 ezcord-0.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 14:07:45.736007 ezcord-0.1.2/src/ezcord/
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-01 14:07:26.000000 ezcord-0.1.2/src/ezcord/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6451 2023-04-01 14:07:26.000000 ezcord-0.1.2/src/ezcord/bot.py
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-04-01 14:07:26.000000 ezcord-0.1.2/src/ezcord/emb.py
--rw-r--r--   0 runner    (1001) docker     (123)     4658 2023-04-01 14:07:26.000000 ezcord-0.1.2/src/ezcord/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-04-01 14:07:26.000000 ezcord-0.1.2/src/ezcord/times.py
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-04-01 14:07:26.000000 ezcord-0.1.2/src/ezcord/translation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-04-01 14:07:26.000000 ezcord-0.1.2/src/ezcord/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 14:07:45.736007 ezcord-0.1.2/src/ezcord.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-04-01 14:07:45.000000 ezcord-0.1.2/src/ezcord.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-01 14:07:45.000000 ezcord-0.1.2/src/ezcord.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-01 14:07:45.000000 ezcord-0.1.2/src/ezcord.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-01 14:07:45.000000 ezcord-0.1.2/src/ezcord.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-01 14:07:45.000000 ezcord-0.1.2/src/ezcord.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 22:09:38.609271 ezcord-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-15 22:09:24.000000 ezcord-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-04-15 22:09:38.609271 ezcord-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-04-15 22:09:24.000000 ezcord-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-15 22:09:24.000000 ezcord-0.1.3/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 22:09:38.605271 ezcord-0.1.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-15 22:09:24.000000 ezcord-0.1.3/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-04-15 22:09:24.000000 ezcord-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-15 22:09:24.000000 ezcord-0.1.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 22:09:38.609271 ezcord-0.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 22:09:38.601271 ezcord-0.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 22:09:38.605271 ezcord-0.1.3/src/ezcord/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-15 22:09:24.000000 ezcord-0.1.3/src/ezcord/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7131 2023-04-15 22:09:24.000000 ezcord-0.1.3/src/ezcord/bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-04-15 22:09:24.000000 ezcord-0.1.3/src/ezcord/emb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 22:09:38.609271 ezcord-0.1.3/src/ezcord/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-04-15 22:09:24.000000 ezcord-0.1.3/src/ezcord/internal/languages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-04-15 22:09:24.000000 ezcord-0.1.3/src/ezcord/internal/translation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-04-15 22:09:24.000000 ezcord-0.1.3/src/ezcord/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-04-15 22:09:24.000000 ezcord-0.1.3/src/ezcord/times.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-04-15 22:09:24.000000 ezcord-0.1.3/src/ezcord/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 22:09:38.609271 ezcord-0.1.3/src/ezcord.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-04-15 22:09:38.000000 ezcord-0.1.3/src/ezcord.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-15 22:09:38.000000 ezcord-0.1.3/src/ezcord.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 22:09:38.000000 ezcord-0.1.3/src/ezcord.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-15 22:09:38.000000 ezcord-0.1.3/src/ezcord.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-15 22:09:38.000000 ezcord-0.1.3/src/ezcord.egg-info/top_level.txt
```

### Comparing `ezcord-0.1.2/LICENSE` & `ezcord-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ezcord-0.1.2/PKG-INFO` & `ezcord-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezcord
-Version: 0.1.2
+Version: 0.1.3
 Summary: An easy-to-use extension for the Pycord library
 Author: tibue99
 License: MIT
 Project-URL: GitHub, https://github.com/tibue99/ezcord
 Project-URL: Documentation, https://ezcord.readthedocs.io
 Keywords: discord,pycord,py-cord
 Classifier: Development Status :: 5 - Production/Stable
@@ -17,14 +17,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: docs
+Provides-Extra: dev
 License-File: LICENSE
 
 # EzCord
 [![](https://img.shields.io/discord/1010915072694046794?label=discord&style=for-the-badge&logo=discord&color=5865F2&logoColor=white)](https://discord.gg/zfvbjTEzv6)
 [![](https://img.shields.io/pypi/v/ezcord.svg?style=for-the-badge&logo=pypi&color=yellow&logoColor=white)](https://pypi.org/project/ezcord/)
 [![](https://img.shields.io/pypi/l/ezcord?style=for-the-badge)]()
 [![](https://aschey.tech/tokei/github/tibue99/ezcord?style=for-the-badge)](https://github.com/tibue99/ezcord)
@@ -32,15 +33,15 @@
 An easy-to-use extension for the [Pycord](https://github.com/Pycord-Development/pycord) library with some utility functions.
 
 ## Installing
 Python 3.8 or higher is required.
 ```
 pip install ezcord
 ```
-You can also install the latest version from GitHub. Note that this version may be unstable 
+You can also install the latest version from GitHub. Note that this version may be unstable
 and requires [git](https://git-scm.com/downloads) to be installed.
 ```
 pip install git+https://github.com/tibue99/ezcord
 ```
 
 ## Useful Links
 - [Documentation](https://ezcord.readthedocs.io/)
```

### Comparing `ezcord-0.1.2/README.md` & `ezcord-0.1.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 An easy-to-use extension for the [Pycord](https://github.com/Pycord-Development/pycord) library with some utility functions.
 
 ## Installing
 Python 3.8 or higher is required.
 ```
 pip install ezcord
 ```
-You can also install the latest version from GitHub. Note that this version may be unstable 
+You can also install the latest version from GitHub. Note that this version may be unstable
 and requires [git](https://git-scm.com/downloads) to be installed.
 ```
 pip install git+https://github.com/tibue99/ezcord
 ```
 
 ## Useful Links
 - [Documentation](https://ezcord.readthedocs.io/)
@@ -41,8 +41,8 @@
 
 ## Contributing
 I am always happy to receive contributions. Here is how to do it:
 1. Fork this repository
 2. Make changes
 3. Create a pull request
 
-You can also [create an issue](https://github.com/tibue99/ezcord/issues/new) if you find any bugs.
+You can also [create an issue](https://github.com/tibue99/ezcord/issues/new) if you find any bugs.
```

### Comparing `ezcord-0.1.2/pyproject.toml` & `ezcord-0.1.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -25,15 +25,16 @@
 
 [tool.setuptools.dynamic]
 dependencies = {file = "requirements.txt"}
 version = {attr = "ezcord.__version__"}
 
 [tool.setuptools.dynamic.optional-dependencies]
 docs = {file = "docs/requirements.txt"}
+dev = {file = "dev-requirements.txt"}
 
 [project.urls]
 GitHub = "https://github.com/tibue99/ezcord"
 Documentation = "https://ezcord.readthedocs.io"
 
 [build-system]
 requires = ["setuptools>=43.0.0", "wheel"]
-build-backend = "setuptools.build_meta"
+build-backend = "setuptools.build_meta"
```

### Comparing `ezcord-0.1.2/src/ezcord/bot.py` & `ezcord-0.1.3/src/ezcord/bot.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,23 @@
+from __future__ import annotations
+
 import logging
 import os
 import traceback
-from typing import Literal, List, Any
 import warnings
+from pathlib import Path
+from typing import Any, Literal
 
+import aiohttp
 import discord
 from discord.ext import commands
-import aiohttp
 
-from .logs import set_log, DEFAULT_LOG
+from .internal.translation import set_lang, t
+from .logs import DEFAULT_LOG, set_log
 from .times import convert_time
-from .utils import t, set_lang
 
 
 class Bot(discord.Bot):
     """Bot class that extends from :class:`discord.Bot`.
 
     Parameters
     ----------
@@ -30,24 +33,25 @@
         .. note::
             You need to enable the error handler for the webhook to work.
     ignored_errors:
         A list of error types to ignore. Defaults to ``None``.
     language:
         The language to use for the bot. Defaults to ``en``.
     """
+
     def __init__(
-            self,
-            intents: discord.Intents = discord.Intents.default(),
-            debug: bool = True,
-            error_handler: bool = True,
-            error_webhook_url: str = None,
-            ignored_errors: List[Any] = None,
-            language: Literal["en", "de"] = "en",
-            *args,
-            **kwargs
+        self,
+        intents: discord.Intents = discord.Intents.default(),
+        debug: bool = True,
+        error_handler: bool = True,
+        error_webhook_url: str | None = None,
+        ignored_errors: list[Any] | None = None,
+        language: Literal["en", "de"] = "en",
+        *args,
+        **kwargs,
     ):
         super().__init__(intents=intents, *args, **kwargs)
 
         if debug:
             self.logger = set_log(DEFAULT_LOG)
         else:
             self.logger = logging.getLogger(DEFAULT_LOG)
@@ -58,15 +62,22 @@
         set_lang(language)
 
         if error_handler:
             self.add_listener(self._error_event, "on_application_command_error")
         elif error_webhook_url:
             warnings.warn("You need to enable the error handler for the webhook to work.")
 
-    def load_cogs(self, *directories: str, subdirectories: bool = False, ignored_cogs: List[str] = None):
+        self.add_listener(self.ready_event, "on_ready")
+
+    def load_cogs(
+        self,
+        *directories: str,
+        subdirectories: bool = False,
+        ignored_cogs: list[str] | None = None,
+    ):
         """Load all cogs in the given directories.
 
         Parameters
         ----------
         *directories:
             Names of the directories to load cogs from.
             Defaults to ``cogs``.
@@ -74,37 +85,43 @@
             Whether to load cogs from subdirectories.
             Defaults to ``False``.
         ignored_cogs:
             A list of cogs to ignore. Defaults to ``None``.
         """
         ignored_cogs = ignored_cogs or []
         if not directories:
-            directories = ["cogs"]
+            directories = ("cogs",)
 
         for directory in directories:
-            if not subdirectories:
-                for filename in os.listdir(f"./{directory}"):
-                    if filename.endswith(".py") and filename not in ignored_cogs:
-                        self.load_extension(f'{directory}.{filename[:-3]}')
-            else:
+            path = Path(directory)
+
+            for filename in os.listdir(directory):
+                if filename.endswith(".py") and filename not in ignored_cogs:
+                    self.load_extension(f"{'.'.join(path.parts)}.{filename[:-3]}")
+                    self.logger.debug(f"Loaded {filename[:-3]}")
+
+            if subdirectories:
                 for element in os.scandir(directory):
                     if element.is_dir():
                         for sub_file in os.scandir(element.path):
                             if sub_file.name.endswith(".py") and sub_file.name not in ignored_cogs:
-                                self.load_extension(f"{directory}.{element.name}.{sub_file.name[:-3]}")
+                                self.load_extension(
+                                    f"{'.'.join(path.parts)}.{element.name}.{sub_file.name[:-3]}"
+                                )
+                                self.logger.debug(f"Loaded {element.name}.{sub_file.name[:-3]}")
 
-    async def on_ready(self):
+    async def ready_event(self):
         """Prints the bot's information when it's ready."""
         infos = [
             f"User:     {self.user}",
             f"ID:       {self.user.id}",
             f"Pycord:   {discord.__version__}",
             f"Commands: {len(self.commands):,}",
             f"Guilds:   {len(self.guilds):,}",
-            f"Latency:  {round(self.latency * 1000):,}ms"
+            f"Latency:  {round(self.latency * 1000):,}ms",
         ]
 
         longest = max([str(i) for i in infos], key=len)
         formatter = f"<{len(longest)}"
 
         start_txt = "Bot is online!"
         start_txt += f"\n╔{(len(longest) + 2) * '═'}╗\n"
@@ -115,55 +132,60 @@
 
     async def _error_event(self, ctx: discord.ApplicationContext, error: discord.DiscordException):
         """The event that handles application command errors."""
         if type(error) in self.ignored_errors:
             return
 
         embed = discord.Embed(
-            title="Error",
-            description=f"{t('error')}: ```{error}```",
-            color=discord.Color.red()
+            title="Error", description=f"{t('error')}: ```{error}```", color=discord.Color.red()
         )
 
         if isinstance(error, commands.CommandOnCooldown):
             seconds = round(ctx.command.get_cooldown_retry_after(ctx))
             embed.title = "Cooldown"
             embed.description = t("cooldown", convert_time(seconds))
             await ctx.respond(embed=embed, ephemeral=True)
 
         elif isinstance(error, commands.BotMissingPermissions):
             perms = "\n".join(error.missing_permissions)
             embed.title = t("no_perm_title")
-            embed.description = f"{t('no_perm_desc')}" \
-                                f"```\n{perms}```"
+            embed.description = f"{t('no_perm_desc')} ```\n{perms}```"
             await ctx.respond(embed=embed, ephemeral=True)
 
         else:
             try:
                 await ctx.respond(embed=embed, ephemeral=True)
             except discord.HTTPException:
                 raise error
 
             if self.error_webhook_url:
                 async with aiohttp.ClientSession() as session:
                     webhook = discord.Webhook.from_url(
-                        self.error_webhook_url,
-                        session=session,
-                        bot_token=self.http.token
+                        self.error_webhook_url, session=session, bot_token=self.http.token
+                    )
+                    error_txt = "".join(
+                        traceback.format_exception(type(error), error, error.__traceback__)
+                    )
+                    guild_txt = (
+                        f"\n\n`Guild:` {ctx.guild.name} ({ctx.guild.id})" if ctx.guild else ""
                     )
-                    error_txt = "".join(traceback.format_exception(type(error), error, error.__traceback__))
-                    guild_txt = f"\n\n`Guild:` {ctx.guild.name} ({ctx.guild.id})" if ctx.guild else ""
                     user_txt = f"\n\n`User:` {ctx.author} ({ctx.author.id})" if ctx.author else ""
 
                     embed = discord.Embed(
                         title="Error Report",
                         description=f"`Command:` /{ctx.command.name}"
-                                    f"{guild_txt}{user_txt}"
-                                    f"```{error_txt[:3500]}```",
-                        color=discord.Color.red()
-                    )
-                    await webhook.send(
-                        embed=embed,
-                        username=f"{self.user.name} Error Report",
-                        avatar_url=self.user.display_avatar.url,
+                        f"{guild_txt}{user_txt}"
+                        f"```{error_txt[:3500]}```",
+                        color=discord.Color.red(),
                     )
+                    try:
+                        await webhook.send(
+                            embed=embed,
+                            username=f"{self.user.name} Error Report",
+                            avatar_url=self.user.display_avatar.url,
+                        )
+                    except discord.HTTPException:
+                        self.logger.error(
+                            "Error while sending error report to webhook. "
+                            "Please check if you the URL is correct."
+                        )
             raise error
```

### Comparing `ezcord-0.1.2/src/ezcord/emb.py` & `ezcord-0.1.3/src/ezcord/emb.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,76 +10,77 @@
     bot = Bot()
 
     @bot.slash_command()
     async def hey(ctx):
         await emb.success(ctx, "Success!")
 """
 
-from typing import Union
+from __future__ import annotations
 
 import discord
-from discord import Embed, Color
+from discord import Color, Embed
 
 
 async def _send_embed(
-        ctx: Union[discord.ApplicationContext, discord.Interaction],
-        embed: discord.Embed,
-        view: discord.ui.View = None
+    interaction: discord.ApplicationContext | discord.Interaction,
+    embed: discord.Embed,
+    ephemeral: bool = True,
+    **kwargs,
 ):
-    if view is None:
-        try:
-            await ctx.response.send_message(embed=embed, ephemeral=True)
-        except discord.InteractionResponded:
-            await ctx.followup.send(embed=embed, ephemeral=True)
-    else:
-        try:
-            await ctx.response.send_message(embed=embed, ephemeral=True, view=view)
-        except discord.InteractionResponded:
-            await ctx.followup.send(embed=embed, ephemeral=True, view=view)
+    """Send an embed to the user. If the interaction has already been responded to,
+    the message will be sent as a followup.
+
+    Parameters
+    ----------
+    interaction:
+        The application context or the interaction to send the message to.
+    embed:
+        The embed to send.
+    ephemeral:
+        Whether the message should be ephemeral.
+    """
+    try:
+        await interaction.response.send_message(embed=embed, ephemeral=ephemeral, **kwargs)
+    except discord.InteractionResponded:
+        await interaction.followup.send(embed=embed, ephemeral=ephemeral, **kwargs)
 
 
 async def error(
-        ctx: Union[discord.ApplicationContext, discord.Interaction],
-        txt: str,
-        view: discord.ui.View = None
+    ctx: discord.ApplicationContext | discord.Interaction,
+    txt: str,
+    ephemeral: bool = True,
+    **kwargs,
 ):
     """Send an error message.
 
     Parameters
     ----------
     ctx:
         The application context or the interaction to send the message to.
     txt:
         The text to send.
-    view:
-        The view to send with the message.
-
+    ephemeral:
+        Whether the message should be ephemeral.
     """
-    embed = Embed(
-        description=txt,
-        color=Color.red()
-    )
-    await _send_embed(ctx, embed, view)
+    embed = Embed(description=txt, color=Color.red())
+    await _send_embed(ctx, embed, ephemeral, **kwargs)
 
 
 async def success(
-        ctx: Union[discord.ApplicationContext, discord.Interaction],
-        txt: str,
-        view: discord.ui.View = None
+    ctx: discord.ApplicationContext | discord.Interaction,
+    txt: str,
+    ephemeral: bool = True,
+    **kwargs,
 ):
     """Send a success message.
 
     Parameters
     ----------
     ctx:
         The application context or the interaction to send the message to.
     txt:
         The text to send.
-    view:
-        The view to send with the message.
-
+    ephemeral:
+        Whether the message should be ephemeral.
     """
-    embed = Embed(
-        description=txt,
-        color=Color.green()
-    )
-    await _send_embed(ctx, embed, view)
+    embed = Embed(description=txt, color=Color.green())
+    await _send_embed(ctx, embed, ephemeral, **kwargs)
```

### Comparing `ezcord-0.1.2/src/ezcord/logs.py` & `ezcord-0.1.3/src/ezcord/logs.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,60 +1,65 @@
 """Some logging utilities that are used for bot logs."""
 
-from typing import Union, Dict
-from colorama import Fore
-from enum import Enum
+from __future__ import annotations
 
 import logging
 import os
 import sys
+from enum import Enum
+
+from colorama import Fore
 
 DEFAULT_LOG = "ezcord"
 log = logging.getLogger(DEFAULT_LOG)
 
 
-DEFAULT_LOG_COLORS = {
+DEFAULT_LOG_COLORS: dict[int, str] = {
     logging.DEBUG: Fore.WHITE,
     logging.INFO: Fore.CYAN,
     logging.WARNING: Fore.YELLOW,
     logging.ERROR: Fore.LIGHTRED_EX,
     logging.CRITICAL: Fore.RED,
 }
 
 
 class LogFormat(str, Enum):
     """Presets for logging formats that can be used in :func:`set_log`.
 
     ``{color_start}`` and ``{color_end}`` are used to add colors to parts of the log message.
     If they are not used, the whole log message will be colored.
     """
+
     default = "[%(asctime)s] %(levelname)s: %(message)s"
     color_level = "[{color_start}%(name)s{color_end}] %(message)s"
     color_name = "[{color_start}%(levelname)s{color_end}] %(message)s"
 
     def __str__(self):
         return self.value
 
 
-def _format_colors(log_format: str, colors: Union[Dict[int, str], str] = None):
+def _format_colors(log_format: str, colors: dict[int, str] | str | None = None):
     """Overwrite the default colors for the given log levels in the given format."""
 
     final_colors = DEFAULT_LOG_COLORS.copy()
     if colors is None:
         colors = final_colors
 
-    for level in colors:
-        final_colors[level] = colors[level]
+    if isinstance(colors, str):
+        for level in final_colors:
+            final_colors[level] = colors
+    else:
+        for level in colors:
+            final_colors[level] = colors[level]
 
     color_formats = {}
     if "{color_start}" in log_format and "{color_end}" in log_format:
         for level in final_colors:
             color_formats[level] = log_format.format(
-                color_start=final_colors[level],
-                color_end=Fore.RESET
+                color_start=final_colors[level], color_end=Fore.RESET
             )
     else:
         for level in final_colors:
             color_formats[level] = final_colors[level] + log_format + Fore.RESET
 
     return color_formats
 
@@ -69,22 +74,23 @@
     log_format:
         The log format.
     time_format:
         The time format.
     colors:
         Colors for the log levels.
     """
+
     def __init__(
-            self,
-            file: bool,
-            log_format: str,
-            time_format: str,
-            colors: Union[Dict[int, str], str] = None,
-            *args,
-            **kwargs
+        self,
+        file: bool,
+        log_format: str,
+        time_format: str,
+        colors: dict[int, str] | str | None = None,
+        *args,
+        **kwargs,
     ):
         super().__init__(*args, **kwargs)
 
         self.file = file
         self.LOG_FORMAT = log_format
         self.TIME_FORMAT = time_format
         self.COLOR_FORMATS = _format_colors(log_format, colors)
@@ -96,29 +102,29 @@
         else:
             log_format = self.COLOR_FORMATS.get(record.levelno)
             formatter = logging.Formatter(log_format, self.TIME_FORMAT)
         return formatter.format(record)
 
 
 def set_log(
-        name: str = DEFAULT_LOG,
-        log_level: int = logging.DEBUG,
-        file: bool = False,
-        log_format: Union[str, LogFormat] = LogFormat.default,
-        time_format: str = "%Y-%m-%d %H:%M:%S",
-        colors: Union[Dict[int, str], str] = None
+    name: str = DEFAULT_LOG,
+    log_level: int = logging.INFO,
+    file: bool = False,
+    log_format: str | LogFormat = LogFormat.default,
+    time_format: str = "%Y-%m-%d %H:%M:%S",
+    colors: dict[int, str] | str | None = None,
 ):
     """Creates a logger. If this logger already exists, it will return the existing logger.
 
     Parameters
     ----------
     name:
         The name of the logger.
     log_level:
-        Whether to enable debug logs. Defaults to ``logging.DEBUG``.
+        Whether to enable debug logs. Defaults to ``logging.INFO``.
     file:
         Whether to log to a file. Defaults to ``False``.
     log_format:
         The log format. Defaults to :attr:`LogFormat.default`.
     time_format:
         The time format. Defaults to ``%Y-%m-%d %H:%M:%S``.
     colors:
@@ -135,25 +141,30 @@
 
             colors = {
                 logging.DEBUG: Fore.GREEN,
                 logging.INFO: Fore.CYAN,
             }
 
             ezcord.set_log(colors=colors)
+
+    Returns
+    -------
+    :class:`logging.Logger`
     """
     logger = logging.getLogger(name)
     if logger.handlers:
         return logger
 
     logger.setLevel(log_level)
 
+    handler: logging.FileHandler | logging.StreamHandler
     if file:
-        if not os.path.exists('logs'):
-            os.mkdir('logs')
+        if not os.path.exists("logs"):
+            os.mkdir("logs")
         filename = name.split(".")[-1]
-        handler = logging.FileHandler(f"logs/{filename}.log", mode="w", encoding='utf-8')
+        handler = logging.FileHandler(f"logs/{filename}.log", mode="w", encoding="utf-8")
     else:
         handler = logging.StreamHandler(sys.stdout)
 
     handler.setFormatter(ColorFormatter(file, log_format, time_format, colors))
     logger.addHandler(handler)
     return logger
```

### Comparing `ezcord-0.1.2/src/ezcord/times.py` & `ezcord-0.1.3/src/ezcord/times.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,16 @@
-from datetime import timezone, datetime, timedelta
-from typing import Literal
+from __future__ import annotations
+
 import re
+from datetime import datetime, timedelta, timezone
+from typing import Literal
 
 from discord.utils import format_dt, utcnow
 
-from .utils import tp
+from .internal.translation import tp
 
 
 def set_utc(dt: datetime) -> datetime:
     """Set the timezone of a datetime object to UTC.
 
     Parameters
     ----------
@@ -18,15 +20,15 @@
     Returns
     -------
     :class:`datetime.datetime`
     """
     return dt.replace(tzinfo=timezone.utc)
 
 
-def convert_time(seconds: int, relative: bool = True) -> str:
+def convert_time(seconds: int | float, relative: bool = True) -> str:
     """Convert seconds to a human-readable time.
 
     Parameters
     ----------
     seconds:
         The amount of seconds to convert.
     relative: :class:`bool`
@@ -49,18 +51,39 @@
     hours = minutes / 60
     if hours < 24:
         return f"{round(hours)} {tp('hour', round(hours))}"
     days = hours / 24
     return f"{round(days)} {tp('day', round(days), relative=relative)}"
 
 
-def dc_timestamp(
-        seconds: int,
-        style: Literal["t", "T", "d", "D", "f", "F", "R"] = "R"
-) -> str:
+def convert_dt(dt: datetime | timedelta, relative: bool = True) -> str:
+    """Convert :class:`datetime` or :class:`timedelta` to a human-readable relative time.
+
+    This function calls :func:`convert_time`.
+
+    Parameters
+    ----------
+    dt:
+        The datetime or timedelta object to convert.
+    relative: :class:`bool`
+        Whether to use relative time. Defaults to ``True``.
+
+    Returns
+    -------
+    :class:`str`
+        A human-readable time.
+    """
+    if isinstance(dt, timedelta):
+        return convert_time(abs(dt.total_seconds()), relative)
+
+    if isinstance(dt, datetime):
+        return convert_time(abs((dt - utcnow()).total_seconds()), relative)
+
+
+def dc_timestamp(seconds: int, style: Literal["t", "T", "d", "D", "f", "F", "R"] = "R") -> str:
     """Convert seconds to a Discord timestamp.
 
     Parameters
     ----------
     seconds:
         The amount of seconds to convert.
     style: :class:`str`
@@ -85,12 +108,16 @@
         The string to convert.
 
     Returns
     -------
     :class:`int`
         The amount of seconds.
     """
-    units = {'s': 'seconds', 'm': 'minutes', 'h': 'hours', 'd': 'days', 'w': 'weeks'}
-    return int(timedelta(**{
-        units.get(m.group('unit').lower(), 'seconds'): float(m.group('val'))
-        for m in re.finditer(r'(?P<val>\d+(\.\d+)?)(?P<unit>[smhdw]?)', s, flags=re.I)
-    }).total_seconds())
+    units = {"s": "seconds", "m": "minutes", "h": "hours", "d": "days", "w": "weeks"}
+    return int(
+        timedelta(
+            **{
+                units.get(m.group("unit").lower(), "seconds"): float(m.group("val"))
+                for m in re.finditer(r"(?P<val>\d+(\.\d+)?)(?P<unit>[smhdw]?)", s, flags=re.I)
+            }
+        ).total_seconds()
+    )
```

### Comparing `ezcord-0.1.2/src/ezcord/translation.py` & `ezcord-0.1.3/src/ezcord/internal/languages.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,25 +5,25 @@
         "hour": "Stunde",
         "day": "Tag",
     },
     "bot": {
         "error": "Der folgende Fehler ist aufgetreten",
         "cooldown": "Versuche es in `{}` erneut.",
         "no_perm_title": "Fehlende Berechtigung",
-        "no_perm_desc": "Mir fehlen die folgenden Berechtigungen, um diesen Befehl auszuführen."
+        "no_perm_desc": "Mir fehlen die folgenden Berechtigungen, um diesen Befehl auszuführen.",
     },
 }
 
 en = {
     "times": {
         "min": "minute",
         "sec": "second",
         "hour": "hour",
         "day": "day",
     },
     "bot": {
         "error": "The following error occurred",
         "cooldown": "Try again in `{}`.",
         "no_perm_title": "Missing permission",
-        "no_perm_desc": "I'm missing the following permissions to execute this command."
+        "no_perm_desc": "I'm missing the following permissions to execute this command.",
     },
 }
```

### Comparing `ezcord-0.1.2/src/ezcord/utils.py` & `ezcord-0.1.3/src/ezcord/internal/translation.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,16 @@
-"""
-.. warning::
-    These utilities are only used by the library itself and
-    are **not** meant to be used directly.
-"""
-import os
+"""Internal language utilities for the library."""
+
 import inspect
-from typing import Literal
+import os
 from configparser import ConfigParser
 from pathlib import Path
+from typing import Literal
 
-from .translation import *
+from .languages import *
 
 
 def plural_de(amount: int, word: str, relative: bool = True) -> str:
     """Pluralize a given word (German).
 
     Parameters
     ----------
```

### Comparing `ezcord-0.1.2/src/ezcord.egg-info/PKG-INFO` & `ezcord-0.1.3/src/ezcord.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezcord
-Version: 0.1.2
+Version: 0.1.3
 Summary: An easy-to-use extension for the Pycord library
 Author: tibue99
 License: MIT
 Project-URL: GitHub, https://github.com/tibue99/ezcord
 Project-URL: Documentation, https://ezcord.readthedocs.io
 Keywords: discord,pycord,py-cord
 Classifier: Development Status :: 5 - Production/Stable
@@ -17,14 +17,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: docs
+Provides-Extra: dev
 License-File: LICENSE
 
 # EzCord
 [![](https://img.shields.io/discord/1010915072694046794?label=discord&style=for-the-badge&logo=discord&color=5865F2&logoColor=white)](https://discord.gg/zfvbjTEzv6)
 [![](https://img.shields.io/pypi/v/ezcord.svg?style=for-the-badge&logo=pypi&color=yellow&logoColor=white)](https://pypi.org/project/ezcord/)
 [![](https://img.shields.io/pypi/l/ezcord?style=for-the-badge)]()
 [![](https://aschey.tech/tokei/github/tibue99/ezcord?style=for-the-badge)](https://github.com/tibue99/ezcord)
@@ -32,15 +33,15 @@
 An easy-to-use extension for the [Pycord](https://github.com/Pycord-Development/pycord) library with some utility functions.
 
 ## Installing
 Python 3.8 or higher is required.
 ```
 pip install ezcord
 ```
-You can also install the latest version from GitHub. Note that this version may be unstable 
+You can also install the latest version from GitHub. Note that this version may be unstable
 and requires [git](https://git-scm.com/downloads) to be installed.
 ```
 pip install git+https://github.com/tibue99/ezcord
 ```
 
 ## Useful Links
 - [Documentation](https://ezcord.readthedocs.io/)
```

